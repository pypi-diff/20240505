# Comparing `tmp/ddeutil-0.3.1.tar.gz` & `tmp/ddeutil-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddeutil-0.3.1.tar", last modified: Sun Apr 28 06:33:08 2024, max compression
+gzip compressed data, was "ddeutil-0.3.2.tar", last modified: Sun May  5 07:13:16 2024, max compression
```

## Comparing `ddeutil-0.3.1.tar` & `ddeutil-0.3.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:33:08.343832 ddeutil-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-28 06:33:02.000000 ddeutil-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-28 06:33:08.343832 ddeutil-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-28 06:33:02.000000 ddeutil-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-28 06:33:02.000000 ddeutil-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 06:33:08.343832 ddeutil-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:33:08.339832 ddeutil-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:33:08.339832 ddeutil-0.3.1/src/ddeutil/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:33:08.339832 ddeutil-0.3.1/src/ddeutil/core/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-28 06:33:02.000000 ddeutil-0.3.1/src/ddeutil/core/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-28 06:33:02.000000 ddeutil-0.3.1/src/ddeutil/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-04-28 06:33:02.000000 ddeutil-0.3.1/src/ddeutil/core/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-28 06:33:02.000000 ddeutil-0.3.1/src/ddeutil/core/dtutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-28 06:33:02.000000 ddeutil-0.3.1/src/ddeutil/core/threader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:33:08.339832 ddeutil-0.3.1/src/ddeutil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-28 06:33:08.000000 ddeutil-0.3.1/src/ddeutil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-28 06:33:08.000000 ddeutil-0.3.1/src/ddeutil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 06:33:08.000000 ddeutil-0.3.1/src/ddeutil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-28 06:33:08.000000 ddeutil-0.3.1/src/ddeutil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-28 06:33:08.000000 ddeutil-0.3.1/src/ddeutil.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:33:08.339832 ddeutil-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-28 06:33:02.000000 ddeutil-0.3.1/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-28 06:33:02.000000 ddeutil-0.3.1/tests/test_dtutils.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-28 06:33:02.000000 ddeutil-0.3.1/tests/test_randomly.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:13:16.713090 ddeutil-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-05 07:13:12.000000 ddeutil-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-05 07:13:16.713090 ddeutil-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-05 07:13:12.000000 ddeutil-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-05-05 07:13:12.000000 ddeutil-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 07:13:16.713090 ddeutil-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:13:16.705090 ddeutil-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:13:16.705090 ddeutil-0.3.2/src/ddeutil/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:13:16.709090 ddeutil-0.3.2/src/ddeutil/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-05 07:13:12.000000 ddeutil-0.3.2/src/ddeutil/core/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-05 07:13:12.000000 ddeutil-0.3.2/src/ddeutil/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-05-05 07:13:12.000000 ddeutil-0.3.2/src/ddeutil/core/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-05 07:13:12.000000 ddeutil-0.3.2/src/ddeutil/core/dtutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-05-05 07:13:12.000000 ddeutil-0.3.2/src/ddeutil/core/threader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:13:16.709090 ddeutil-0.3.2/src/ddeutil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-05 07:13:16.000000 ddeutil-0.3.2/src/ddeutil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-05 07:13:16.000000 ddeutil-0.3.2/src/ddeutil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 07:13:16.000000 ddeutil-0.3.2/src/ddeutil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-05 07:13:16.000000 ddeutil-0.3.2/src/ddeutil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-05 07:13:16.000000 ddeutil-0.3.2/src/ddeutil.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:13:16.709090 ddeutil-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-05 07:13:12.000000 ddeutil-0.3.2/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-05 07:13:12.000000 ddeutil-0.3.2/tests/test_dtutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-05 07:13:12.000000 ddeutil-0.3.2/tests/test_randomly.py
```

### Comparing `ddeutil-0.3.1/LICENSE` & `ddeutil-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ddeutil-0.3.1/PKG-INFO` & `ddeutil-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddeutil
-Version: 0.3.1
+Version: 0.3.2
 Summary: Data Developer & Engineer Core Utility Objects
 Author-email: korawica <korawich.anu@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/ddeutils/ddeutil/
 Project-URL: Source Code, https://github.com/ddeutils/ddeutil/
 Keywords: data,utility
 Classifier: Topic :: Utilities
@@ -21,16 +21,16 @@
 Requires-Python: >=3.9.13
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ujson==5.9.0
 Requires-Dist: tzdata==2024.1
 Requires-Dist: python-dateutil==2.9.0.post0
 Provides-Extra: dev
-Requires-Dist: clishelf==0.2.0; extra == "dev"
-Requires-Dist: pytest==8.1.1; extra == "dev"
+Requires-Dist: clishelf==0.2.1; extra == "dev"
+Requires-Dist: pytest==8.2.0; extra == "dev"
 Requires-Dist: types-python-dateutil==2.9.0.20240316; extra == "dev"
 Provides-Extra: perf
 Requires-Dist: memory_profiler==0.61.0; extra == "perf"
 Requires-Dist: perfplot<1.0.0,==0.10.2; extra == "perf"
 
 # Data Utility Packages: _Core_
```

### Comparing `ddeutil-0.3.1/README.md` & `ddeutil-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ddeutil-0.3.1/pyproject.toml` & `ddeutil-0.3.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 
 [project.urls]
 Homepage = "https://github.com/ddeutils/ddeutil/"
 "Source Code" = "https://github.com/ddeutils/ddeutil/"
 
 [project.optional-dependencies]
 dev = [
-    "clishelf==0.2.0",
-    "pytest==8.1.1",
+    "clishelf==0.2.1",
+    "pytest==8.2.0",
     "types-python-dateutil==2.9.0.20240316",
 ]
 perf = [
     "memory_profiler==0.61.0",
     "perfplot==0.10.2,<1.0.0",
 ]
```

### Comparing `ddeutil-0.3.1/src/ddeutil/core/__init__.py` & `ddeutil-0.3.2/src/ddeutil/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ddeutil-0.3.1/src/ddeutil/core/decorator.py` & `ddeutil-0.3.2/src/ddeutil/core/decorator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,31 @@
+from __future__ import annotations
+
 import contextlib
 import copy
 from functools import wraps
 from time import (
     sleep,
     time,
 )
+from typing import TYPE_CHECKING, Any, Callable, TypeVar
+
+if TYPE_CHECKING:
+    import sys
+
+    if sys.version_info >= (3, 10):
+        from typing import ParamSpec
+    else:
+        from typing_extensions import ParamSpec
 
+    P = ParamSpec("P")
+    T = TypeVar("T")
 
-def deepcopy(func):
+
+def deepcopy(func: Callable[P, T]) -> Callable[P, T]:
     """Deep copy method
 
     EExamples:
         >>> @deepcopy
         ... def foo(a, b, c=None):
         ...     c = c or {}
         ...     a[1] = 3
@@ -25,24 +39,24 @@
         ({1: 3}, {2: 4}, {3: 5})
 
         >>> (aa, bb, cc)
         ({1: 2}, {2: 3}, {3: 4})
 
     """
 
-    def func_get(*args, **kwargs):
+    def func_get(*args: P.args, **kwargs: P.kwargs) -> T:
         return func(
             *(copy.deepcopy(x) for x in args),
             **{k: copy.deepcopy(v) for k, v in kwargs.items()},
         )
 
     return func_get
 
 
-def deepcopy_args(func):
+def deepcopy_args(func: Callable[[object, P], T]) -> Callable[[object, P], T]:
     """Deep copy method
 
     Examples:
         >>> class Foo:
         ...
         ...     @deepcopy_args
         ...     def foo(self, a, b=None):
@@ -57,62 +71,61 @@
         ({1: 4}, {2: 5})
 
         >>> (aa, bb)
         ({1: 2}, {2: 3})
 
     """
 
-    def func_get(self, *args, **kwargs):
+    def func_get(self: object, *args: P.args, **kwargs: P.kwargs) -> T:
         return func(
             self,
             *(copy.deepcopy(x) for x in args),
             **{k: copy.deepcopy(v) for k, v in kwargs.items()},
         )
 
     return func_get
 
 
-def timer(func):
+def timer(func: Callable[P, T]) -> Callable[P, T]:
     """
     Examples:
         >>> import time
         >>> @timer
         ... def will_sleep():
         ...     time.sleep(2)
         ...     return
         >>> will_sleep()
         Execution time: 2.003119945526123 seconds
     """
 
-    def wrapper(*args, **kwargs):
+    def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
         start_time = time()
         result = func(*args, **kwargs)
-        end_time = time()
-        execution_time = end_time - start_time
+        execution_time = time() - start_time
         print(f"Execution time: {execution_time} seconds")
         return result
 
     return wrapper
 
 
-def timing(name: str):
+def timing(name: str) -> Callable[[Callable[P, T]], Callable[P, T]]:
     """
     Examples:
         >>> import time
         >>> @timing("Sleep")
         ... def will_sleep():
         ...     time.sleep(2)
         ...     return
         >>> will_sleep()
         Sleep ....................................................... 2.01s
     """
 
-    def timing_internal(func):
+    def timing_internal(func: Callable[P, T]) -> Callable[P, T]:
         @wraps(func)
-        def wrap(*args, **kw):
+        def wrap(*args: P.args, **kw: P.kwargs) -> T:
             ts = time()
             result = func(*args, **kw)
             padded_name: str = f"{name} ".ljust(60, ".")
             padded_time: str = f" {(time() - ts):0.2f}".rjust(6, ".")
             print(f"{padded_name}{padded_time}s", flush=True)
             return result
 
@@ -134,49 +147,53 @@
     yield
     te = time()
     padded_name: str = f"{title} ".ljust(60, ".")
     padded_time: str = f" {(te - ts):0.2f}".rjust(6, ".")
     print(f"{padded_name}{padded_time}s", flush=True)
 
 
-def debug(func):
+def debug(func: Callable[P, T]) -> Callable[P, T]:
     """
     Examples:
         >>> @debug
         ... def add_numbers(x, y):
         ...     return x + y
         >>> add_numbers(7, y=5, )
         Calling add_numbers with args: (7,) kwargs: {'y': 5}
         add_numbers returned: 12
         12
     """
 
-    def wrapper(*args, **kwargs):
+    @wraps(func)
+    def wrapper(*args: P.args, **kwargs: P.kwargs):
         print(f"Calling {func.__name__} with args: {args} kwargs: {kwargs}")
         result = func(*args, **kwargs)
         print(f"{func.__name__} returned: {result}")
         return result
 
     return wrapper
 
 
-def validate_input(*validations):
+def validate_input(
+    *validations: tuple[Callable[[Any], bool]],
+) -> Callable[[Callable[P, T]], Callable[P, T]]:
     """
     Examples:
         >>> @validate_input(lambda x: x > 0, lambda y: isinstance(y, str))
         ... def divide_and_print(x: int, message: str):
         ...     print(message)
         ...     return 1 / x
         >>> divide_and_print(5, "Hello!")
         Hello!
         0.2
     """
 
-    def decorator(func):
-        def wrapper(*args, **kwargs):
+    def decorator(func: Callable[P, T]) -> Callable[P, T]:
+        @wraps(func)
+        def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
             for i, val in enumerate(args):
                 if i < len(validations) and not validations[i](val):
                     raise ValueError(f"Invalid argument: {val}")
             for key, val in kwargs.items():
                 if key in validations[len(args) :] and not validations[
                     len(args) :
                 ][key](val):
@@ -185,17 +202,17 @@
 
         return wrapper
 
     return decorator
 
 
 def retry(
-    max_attempts,
+    max_attempts: int,
     delay: int = 1,
-):
+) -> Callable[[Callable[P, T]], Callable[P, T]]:
     """Retry decorator with sequencial.
     Examples:
         >>> @retry(max_attempts=3, delay=2)
         ... def fetch_data(url):
         ...     print("Fetching the data ...")
         ...     raise TimeoutError("Server is not responding.")
         >>> fetch_data("https://example.com/data")
@@ -204,16 +221,17 @@
         Fetching the data ...
         Attempt 2 failed: Server is not responding.
         Fetching the data ...
         Attempt 3 failed: Server is not responding.
         Function `fetch_data` failed after 3 attempts
     """
 
-    def decorator(func):
-        def wrapper(*args, **kwargs):
+    def decorator(func: Callable[P, T]) -> Callable[P, T]:
+        @wraps(func)
+        def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
             _attempts: int = 0
             while _attempts < max_attempts:
                 try:
                     return func(*args, **kwargs)
                 except Exception as e:
                     _attempts += 1
                     print(f"Attempt {_attempts} failed: {e}")
```

### Comparing `ddeutil-0.3.1/src/ddeutil/core/dtutils.py` & `ddeutil-0.3.2/src/ddeutil/core/dtutils.py`

 * *Files identical despite different names*

### Comparing `ddeutil-0.3.1/src/ddeutil/core/threader.py` & `ddeutil-0.3.2/src/ddeutil/core/threader.py`

 * *Files identical despite different names*

### Comparing `ddeutil-0.3.1/src/ddeutil.egg-info/PKG-INFO` & `ddeutil-0.3.2/src/ddeutil.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddeutil
-Version: 0.3.1
+Version: 0.3.2
 Summary: Data Developer & Engineer Core Utility Objects
 Author-email: korawica <korawich.anu@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/ddeutils/ddeutil/
 Project-URL: Source Code, https://github.com/ddeutils/ddeutil/
 Keywords: data,utility
 Classifier: Topic :: Utilities
@@ -21,16 +21,16 @@
 Requires-Python: >=3.9.13
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ujson==5.9.0
 Requires-Dist: tzdata==2024.1
 Requires-Dist: python-dateutil==2.9.0.post0
 Provides-Extra: dev
-Requires-Dist: clishelf==0.2.0; extra == "dev"
-Requires-Dist: pytest==8.1.1; extra == "dev"
+Requires-Dist: clishelf==0.2.1; extra == "dev"
+Requires-Dist: pytest==8.2.0; extra == "dev"
 Requires-Dist: types-python-dateutil==2.9.0.20240316; extra == "dev"
 Provides-Extra: perf
 Requires-Dist: memory_profiler==0.61.0; extra == "perf"
 Requires-Dist: perfplot<1.0.0,==0.10.2; extra == "perf"
 
 # Data Utility Packages: _Core_
```

### Comparing `ddeutil-0.3.1/tests/test_randomly.py` & `ddeutil-0.3.2/tests/test_randomly.py`

 * *Files identical despite different names*

