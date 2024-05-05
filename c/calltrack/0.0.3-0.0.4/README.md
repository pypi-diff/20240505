# Comparing `tmp/calltrack-0.0.3.tar.gz` & `tmp/calltrack-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calltrack-0.0.3.tar", max compression
+gzip compressed data, was "calltrack-0.0.4.tar", max compression
```

## Comparing `calltrack-0.0.3.tar` & `calltrack-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,10 @@
--rw-r--r--   0        0        0      265 2024-05-04 20:04:39.940522 calltrack-0.0.3/README.md
--rw-r--r--   0        0        0     2659 2024-05-04 19:50:07.168310 calltrack-0.0.3/calltrack/__init__.py
--rw-r--r--   0        0        0     2828 2024-05-04 18:25:03.741535 calltrack-0.0.3/calltrack/calltrack.py
--rw-r--r--   0        0        0      284 2024-05-04 20:01:07.985579 calltrack-0.0.3/calltrack/cli.py
--rw-r--r--   0        0        0      169 2024-05-04 19:49:55.631820 calltrack-0.0.3/calltrack/dependencies.py
--rw-r--r--   0        0        0      488 2024-05-04 18:25:58.918897 calltrack-0.0.3/calltrack/log_queue.py
--rw-r--r--   0        0        0     2843 2024-05-04 19:52:18.673281 calltrack-0.0.3/calltrack/logs/log_20240504_215218_677136.json
--rw-r--r--   0        0        0     2846 2024-05-04 19:52:24.881490 calltrack-0.0.3/calltrack/logs/log_20240504_215224_885928.json
--rw-r--r--   0        0        0    11541 2024-05-04 12:17:01.246119 calltrack-0.0.3/calltrack/main.ipynb
--rw-r--r--   0        0        0       97 2024-05-03 10:07:38.552167 calltrack-0.0.3/calltrack/setup.py
--rw-r--r--   0        0        0      398 2024-05-04 12:26:22.259699 calltrack-0.0.3/calltrack/utils.py
--rw-r--r--   0        0        0     1781 2024-05-04 19:56:36.056440 calltrack-0.0.3/calltrack/view.py
--rw-r--r--   0        0        0      455 2024-05-04 20:02:23.978718 calltrack-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      785 1970-01-01 00:00:00.000000 calltrack-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      857 2024-05-05 09:42:30.678232 calltrack-0.0.4/README.md
+-rw-r--r--   0        0        0     2928 2024-05-05 09:38:28.235386 calltrack-0.0.4/calltrack/__init__.py
+-rw-r--r--   0        0        0     2828 2024-05-04 18:25:03.741535 calltrack-0.0.4/calltrack/calltrack.py
+-rw-r--r--   0        0        0      377 2024-05-05 09:10:17.150249 calltrack-0.0.4/calltrack/cli.py
+-rw-r--r--   0        0        0      220 2024-05-05 09:17:40.059196 calltrack-0.0.4/calltrack/dependencies.py
+-rw-r--r--   0        0        0      488 2024-05-04 18:25:58.918897 calltrack-0.0.4/calltrack/log_queue.py
+-rw-r--r--   0        0        0       97 2024-05-03 10:07:38.552167 calltrack-0.0.4/calltrack/setup.py
+-rw-r--r--   0        0        0      661 2024-05-05 09:32:17.702430 calltrack-0.0.4/calltrack/utils.py
+-rw-r--r--   0        0        0      456 2024-05-05 09:43:41.483313 calltrack-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1377 1970-01-01 00:00:00.000000 calltrack-0.0.4/PKG-INFO
```

### Comparing `calltrack-0.0.3/calltrack/__init__.py` & `calltrack-0.0.4/calltrack/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import atexit
 import functools
+import inspect
+import json
 import time
 import uuid
 from datetime import datetime
 from typing import Callable
 
 from .calltrack import ConsoleCalltrack, JSONCalltrack
 from .dependencies import json_calltrack
+from .utils import CustomJSONEncoder
 
 atexit.register(lambda: json_calltrack.flush() if json_calltrack.queue.queue else None)
 
 
 def consolelog(func: Callable):
     @functools.wraps(func)
     def consolelog_wrapper(*args, **kwargs):
@@ -49,33 +52,35 @@
         calltrack = json_calltrack
 
     def jsonlog_decorator(func: Callable, calltrack: JSONCalltrack):
         @functools.wraps(func)
         def jsonlog_wrapper(*args, **kwargs):
             args_repr = [repr(a) for a in args]
             kwargs_repr = [f"{k}={repr(v)}" for k, v in kwargs.items()]
-            signature = ", ".join(args_repr + kwargs_repr)
 
             uuidv1 = uuid.uuid1()
 
             timestamp = datetime.now()
             start_time = time.perf_counter()
 
             output = func(*args, **kwargs)
 
             end_time = time.perf_counter()
             run_time = end_time - start_time
 
             calltrack.append(
                 log={
                     str(uuidv1): {
+                        "call": f"{func.__name__}( {', '.join([f'{arg}={val}' for arg, val in zip(inspect.signature(func).parameters, args)])}, {kwargs_repr} )",
                         "name": func.__name__,
                         "args": args_repr,
                         "kwargs": kwargs_repr,
-                        "signature": signature,
+                        "annotations": json.dumps(
+                            func.__annotations__, cls=CustomJSONEncoder
+                        ),
                         "output": repr(output),
                         "run_time": run_time,
                         "timestamp": str(timestamp),
                     }
                 }
             )
             if calltrack.autoflush:
```

### Comparing `calltrack-0.0.3/calltrack/calltrack.py` & `calltrack-0.0.4/calltrack/calltrack.py`

 * *Files identical despite different names*

