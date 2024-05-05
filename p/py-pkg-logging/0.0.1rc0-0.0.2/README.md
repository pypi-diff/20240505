# Comparing `tmp/py_pkg_logging-0.0.1rc0.tar.gz` & `tmp/py_pkg_logging-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_pkg_logging-0.0.1rc0.tar", last modified: Sun Apr 14 18:14:27 2024, max compression
+gzip compressed data, was "py_pkg_logging-0.0.2.tar", last modified: Sun May  5 15:34:42 2024, max compression
```

## Comparing `py_pkg_logging-0.0.1rc0.tar` & `py_pkg_logging-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:14:27.385337 py_pkg_logging-0.0.1rc0/
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-14 18:14:27.385337 py_pkg_logging-0.0.1rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-14 18:14:17.000000 py_pkg_logging-0.0.1rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:14:27.385337 py_pkg_logging-0.0.1rc0/py_pkg_logging/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-14 18:14:17.000000 py_pkg_logging-0.0.1rc0/py_pkg_logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-14 18:14:17.000000 py_pkg_logging-0.0.1rc0/py_pkg_logging/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-14 18:14:17.000000 py_pkg_logging-0.0.1rc0/py_pkg_logging/_log_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-14 18:14:17.000000 py_pkg_logging-0.0.1rc0/py_pkg_logging/_log_function_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:14:27.385337 py_pkg_logging-0.0.1rc0/py_pkg_logging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-14 18:14:27.000000 py_pkg_logging-0.0.1rc0/py_pkg_logging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-14 18:14:27.000000 py_pkg_logging-0.0.1rc0/py_pkg_logging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 18:14:27.000000 py_pkg_logging-0.0.1rc0/py_pkg_logging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-14 18:14:27.000000 py_pkg_logging-0.0.1rc0/py_pkg_logging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 18:14:27.389337 py_pkg_logging-0.0.1rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-14 18:14:17.000000 py_pkg_logging-0.0.1rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:34:42.507604 py_pkg_logging-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-05 15:34:42.507604 py_pkg_logging-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-05 15:34:33.000000 py_pkg_logging-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:34:42.503605 py_pkg_logging-0.0.2/py_pkg_logging/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-05 15:34:33.000000 py_pkg_logging-0.0.2/py_pkg_logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-05 15:34:33.000000 py_pkg_logging-0.0.2/py_pkg_logging/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-05 15:34:33.000000 py_pkg_logging-0.0.2/py_pkg_logging/_log_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-05 15:34:33.000000 py_pkg_logging-0.0.2/py_pkg_logging/_log_function_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:34:42.507604 py_pkg_logging-0.0.2/py_pkg_logging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-05 15:34:42.000000 py_pkg_logging-0.0.2/py_pkg_logging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-05 15:34:42.000000 py_pkg_logging-0.0.2/py_pkg_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 15:34:42.000000 py_pkg_logging-0.0.2/py_pkg_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-05 15:34:42.000000 py_pkg_logging-0.0.2/py_pkg_logging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 15:34:42.507604 py_pkg_logging-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-05 15:34:33.000000 py_pkg_logging-0.0.2/setup.py
```

### Comparing `py_pkg_logging-0.0.1rc0/py_pkg_logging/_log_config.py` & `py_pkg_logging-0.0.2/py_pkg_logging/_log_config.py`

 * *Files identical despite different names*

### Comparing `py_pkg_logging-0.0.1rc0/py_pkg_logging/_log_function_call.py` & `py_pkg_logging-0.0.2/py_pkg_logging/_log_function_call.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 
+# -- import packages: ---------------------------------------------------------
 import ABCParse
 import inspect
 from functools import wraps
 import logging
 import numpy as np
 
+
+# -- set typing: --------------------------------------------------------------
 from typing import Callable
 
 
+# -- Operational class: -------------------------------------------------------
 class FunctionCallLogger(ABCParse.ABCParse):
     def __init__(self, logger):
         """"""
         self.__parse__(locals())
         self._ARGS_IGNORE = ['self']
 
     @property
     def arg_values(self):
         return self.bound.arguments
 
     @property
     def cls_method(self):
-        return self._args and hasattr(self._args[0], self._func.__name__)
+        return self._args and hasattr(self._args[0], self._logged_func.__name__)
 
     @property
     def bound(self):
         if self.cls_method:
-            self._bound = inspect.signature(self._func).bind(*self._args, **self._kwargs)
+            self._bound = inspect.signature(self._logged_func).bind(*self._args, **self._kwargs)
         else:
-            self._bound = inspect.signature(self._func).bind_partial(*self._args, **self._kwargs)
+            self._bound = inspect.signature(self._logged_func).bind_partial(*self._args, **self._kwargs)
         self._bound.apply_defaults()
         return self._bound
 
     @property
     def func_name(self):
         if "self" in self.arg_values:
             cls = self.arg_values.pop("self").__class__.__name__
-            return f"{cls}.{self._func.__name__}"
-        return self._func.__name__
+            return f"{cls}.{self._logged_func.__name__}"
+        return self._logged_func.__name__
     
     @property
     def _arg_message(self):
         return_str = ""
         for key, val in self.arg_values.items():
             if not key in self._ARGS_IGNORE:
                 if isinstance(val, np.ndarray):
@@ -49,24 +53,37 @@
         return return_str[:-2] # rm final comma
     
     @property
     def log_message(self):
         return f"Called: {self.func_name} with args: {self._arg_message}"
 
 
-    def __call__(self, func, *args, **kwargs):
+    def __call__(self, logged_func: Callable, *args, **kwargs):
         """ """
         self.__update__(locals())
         self._logger.debug(self.log_message)
 
 
+# -- API-facing decorator function: -------------------------------------------
 def log_function_call(logger):
-    def decorator(func: Callable):
-        @wraps(func)
+    """
+    Args:
+        logger
+    """
+    def decorator(logged_func: Callable):
+        """
+        Args:
+            logged_func (Callable)
+        """
+        @wraps(logged_func)
         def wrapper(*args, **kwargs):
-            
+            """
+            Args:
+                *args
+                **kwargs
+            """
             function_call_logger = FunctionCallLogger(logger = logger)
-            function_call_logger(func, *args, **kwargs)
+            function_call_logger(logged_func=logged_func, *args, **kwargs)
             
-            return func(*args, **kwargs)
+            return logged_func(*args, **kwargs)
         return wrapper
     return decorator
```

### Comparing `py_pkg_logging-0.0.1rc0/setup.py` & `py_pkg_logging-0.0.2/setup.py`

 * *Files identical despite different names*

