# Comparing `tmp/calltrack-0.0.2.tar.gz` & `tmp/calltrack-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calltrack-0.0.2.tar", max compression
+gzip compressed data, was "calltrack-0.0.3.tar", max compression
```

## Comparing `calltrack-0.0.2.tar` & `calltrack-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0        0 2024-05-03 08:28:05.244987 calltrack-0.0.2/README.md
--rw-r--r--   0        0        0     2657 2024-05-04 17:04:49.376399 calltrack-0.0.2/calltrack/__init__.py
--rw-r--r--   0        0        0       97 2024-05-03 10:07:38.552167 calltrack-0.0.2/calltrack/setup.py
--rw-r--r--   0        0        0        0 2024-05-03 10:05:16.395151 calltrack-0.0.2/calltrack/src/__init__.py
--rw-r--r--   0        0        0     2874 2024-05-04 17:07:17.388848 calltrack-0.0.2/calltrack/src/calltrack.py
--rw-r--r--   0        0        0     2648 2024-05-04 12:15:06.335788 calltrack-0.0.2/calltrack/src/decorators.py
--rw-r--r--   0        0        0      433 2024-05-04 12:05:40.058066 calltrack-0.0.2/calltrack/src/log_queue.py
--rw-r--r--   0        0        0      398 2024-05-04 12:26:22.259699 calltrack-0.0.2/calltrack/src/utils.py
--rw-r--r--   0        0        0        0 2024-05-03 10:05:50.791422 calltrack-0.0.2/calltrack/tests/__init__.py
--rw-r--r--   0        0        0     2025 2024-05-03 10:22:28.846390 calltrack-0.0.2/calltrack/tests/test_log_writer.py
--rw-r--r--   0        0        0      395 2024-05-04 17:09:23.930612 calltrack-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      520 1970-01-01 00:00:00.000000 calltrack-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      265 2024-05-04 20:04:39.940522 calltrack-0.0.3/README.md
+-rw-r--r--   0        0        0     2659 2024-05-04 19:50:07.168310 calltrack-0.0.3/calltrack/__init__.py
+-rw-r--r--   0        0        0     2828 2024-05-04 18:25:03.741535 calltrack-0.0.3/calltrack/calltrack.py
+-rw-r--r--   0        0        0      284 2024-05-04 20:01:07.985579 calltrack-0.0.3/calltrack/cli.py
+-rw-r--r--   0        0        0      169 2024-05-04 19:49:55.631820 calltrack-0.0.3/calltrack/dependencies.py
+-rw-r--r--   0        0        0      488 2024-05-04 18:25:58.918897 calltrack-0.0.3/calltrack/log_queue.py
+-rw-r--r--   0        0        0     2843 2024-05-04 19:52:18.673281 calltrack-0.0.3/calltrack/logs/log_20240504_215218_677136.json
+-rw-r--r--   0        0        0     2846 2024-05-04 19:52:24.881490 calltrack-0.0.3/calltrack/logs/log_20240504_215224_885928.json
+-rw-r--r--   0        0        0    11541 2024-05-04 12:17:01.246119 calltrack-0.0.3/calltrack/main.ipynb
+-rw-r--r--   0        0        0       97 2024-05-03 10:07:38.552167 calltrack-0.0.3/calltrack/setup.py
+-rw-r--r--   0        0        0      398 2024-05-04 12:26:22.259699 calltrack-0.0.3/calltrack/utils.py
+-rw-r--r--   0        0        0     1781 2024-05-04 19:56:36.056440 calltrack-0.0.3/calltrack/view.py
+-rw-r--r--   0        0        0      455 2024-05-04 20:02:23.978718 calltrack-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      785 1970-01-01 00:00:00.000000 calltrack-0.0.3/PKG-INFO
```

### Comparing `calltrack-0.0.2/calltrack/__init__.py` & `calltrack-0.0.3/calltrack/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,18 @@
+import atexit
 import functools
-import os
 import time
 import uuid
 from datetime import datetime
 from typing import Callable
 
-from .src.calltrack import ConsoleCalltrack, JSONCalltrack
-from .src.log_queue import LogQueue
+from .calltrack import ConsoleCalltrack, JSONCalltrack
+from .dependencies import json_calltrack
 
-json_calltrack = JSONCalltrack(
-    log_queue=LogQueue(), save_dir=os.getcwd(), autoflush=False
-)
+atexit.register(lambda: json_calltrack.flush() if json_calltrack.queue.queue else None)
 
 
 def consolelog(func: Callable):
     @functools.wraps(func)
     def consolelog_wrapper(*args, **kwargs):
         calltrack = ConsoleCalltrack()
 
@@ -41,15 +39,15 @@
 
     return consolelog_wrapper
 
 
 def jsonlog(
     _func=None,
     *,
-    calltrack: JSONCalltrack = None,
+    calltrack: JSONCalltrack | None = None,
 ):
     if not calltrack:
         calltrack = json_calltrack
 
     def jsonlog_decorator(func: Callable, calltrack: JSONCalltrack):
         @functools.wraps(func)
         def jsonlog_wrapper(*args, **kwargs):
```

### Comparing `calltrack-0.0.2/calltrack/src/calltrack.py` & `calltrack-0.0.3/calltrack/calltrack.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,20 +8,23 @@
 from .log_queue import LogQueue
 from .utils import is_path_creatable
 
 
 class Calltrack(ABC):
     """Calltrack Abstract Class"""
 
-    def __init__(self, log_queue: LogQueue):
-        self.log_queue = log_queue
+    def __init__(self, queue: LogQueue = LogQueue()):
+        self.queue = queue
 
     def flush(self) -> None:
-        while self.log_queue.queue:
-            self.write(self.log_queue.popleft())
+        while self.queue.queue:
+            self.write(self.queue.popleft())
+
+    def append(self, log: dict) -> None:
+        self.queue.append(log)
 
     @abstractmethod
     def write(
         self,
         log: Any,
     ) -> None:
         """Write logs"""
@@ -30,17 +33,17 @@
 class ConsoleCalltrack(Calltrack):
     def write(self, log: Any) -> None:
         print(log)
 
 
 class JSONCalltrack(Calltrack):
     def __init__(
-        self, log_queue: LogQueue, save_dir: str, autoflush: bool = False
+        self, save_dir: str, queue: LogQueue = LogQueue(), autoflush: bool = False
     ) -> None:
-        super().__init__(log_queue=log_queue)
+        super().__init__(queue=queue)
         self._save_dir = save_dir
         self.autoflush = autoflush
 
         self._prepare_dir()
 
     @property
     def save_dir(self):
@@ -52,43 +55,40 @@
             self._save_dir = path
             self._prepare_dir()
         else:
             warnings.warn("The provided path is ill-formed.")
 
     def flush(self, filename: str | None = None):
         concat_log = {}
-        while self.log_queue.queue:
-            log = self.log_queue.queue.popleft()
+        while self.queue.queue:
+            log = self.queue.queue.popleft()
             self._check_log(log)
             concat_log.update(log)
         self.write(concat_log, filename)
 
     def write(self, log: dict, filename: str | None = None) -> None:
         self._check_log(log)
         """Assuming the log is well formatted"""
         self._export_log(log, filename)
 
-    def append(self, log: dict) -> None:
-        self.log_queue.append(log)
-
     def _export_log(self, log: dict, filename: str | None = None) -> None:
         """Export the logs to a JSON file.
 
         Args:
         ----
             file_path (str, optional): The file path to save the logs. If not provided, a default file path will be used.
 
         """
         if not filename:
             filename = self._default_filename()
         if not filename.endswith(".json"):
             filename = filename + ".json"
 
         filepath = os.path.join(self.save_dir, filename)
-        print(log, filepath)
+
         with open(filepath, "w") as file:
             json.dump(log, file, indent=4)
 
     def _default_filename(self) -> str:
         timestamp = datetime.now().strftime("%Y%m%d_%H%M%S_%f")
         return f"log_{timestamp}.json"
```

