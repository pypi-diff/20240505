# Comparing `tmp/ABCParse-0.0.7rc1.tar.gz` & `tmp/abcparse-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ABCParse-0.0.7rc1.tar", last modified: Mon Nov  6 17:11:11 2023, max compression
+gzip compressed data, was "abcparse-0.0.8.tar", last modified: Sun May  5 03:50:28 2024, max compression
```

## Comparing `ABCParse-0.0.7rc1.tar` & `abcparse-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 17:11:11.968531 ABCParse-0.0.7rc1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 17:11:11.968531 ABCParse-0.0.7rc1/ABCParse/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2023-11-06 17:11:03.000000 ABCParse-0.0.7rc1/ABCParse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5073 2023-11-06 17:11:03.000000 ABCParse-0.0.7rc1/ABCParse/_abc_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2023-11-06 17:11:03.000000 ABCParse-0.0.7rc1/ABCParse/_as_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2023-11-06 17:11:03.000000 ABCParse-0.0.7rc1/ABCParse/_function_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2023-11-06 17:11:03.000000 ABCParse-0.0.7rc1/ABCParse/_info_message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 17:11:11.968531 ABCParse-0.0.7rc1/ABCParse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2023-11-06 17:11:11.000000 ABCParse-0.0.7rc1/ABCParse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      297 2023-11-06 17:11:11.000000 ABCParse-0.0.7rc1/ABCParse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-06 17:11:11.000000 ABCParse-0.0.7rc1/ABCParse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-06 17:11:11.000000 ABCParse-0.0.7rc1/ABCParse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2023-11-06 17:11:03.000000 ABCParse-0.0.7rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2023-11-06 17:11:11.968531 ABCParse-0.0.7rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      725 2023-11-06 17:11:03.000000 ABCParse-0.0.7rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-06 17:11:11.968531 ABCParse-0.0.7rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      743 2023-11-06 17:11:03.000000 ABCParse-0.0.7rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 17:11:11.968531 ABCParse-0.0.7rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2023-11-06 17:11:03.000000 ABCParse-0.0.7rc1/tests/test_ABCParse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:50:28.694360 abcparse-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:50:28.690360 abcparse-0.0.8/ABCParse/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-05 03:50:18.000000 abcparse-0.0.8/ABCParse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-05 03:50:18.000000 abcparse-0.0.8/ABCParse/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-05-05 03:50:18.000000 abcparse-0.0.8/ABCParse/_abc_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-05 03:50:18.000000 abcparse-0.0.8/ABCParse/_as_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-05 03:50:18.000000 abcparse-0.0.8/ABCParse/_function_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-05 03:50:18.000000 abcparse-0.0.8/ABCParse/_info_message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:50:28.694360 abcparse-0.0.8/ABCParse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-05 03:50:28.000000 abcparse-0.0.8/ABCParse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-05 03:50:28.000000 abcparse-0.0.8/ABCParse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 03:50:28.000000 abcparse-0.0.8/ABCParse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-05 03:50:28.000000 abcparse-0.0.8/ABCParse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-05 03:50:28.000000 abcparse-0.0.8/ABCParse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-05 03:50:18.000000 abcparse-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-05 03:50:28.694360 abcparse-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-05 03:50:18.000000 abcparse-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 03:50:28.694360 abcparse-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-05 03:50:18.000000 abcparse-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:50:28.694360 abcparse-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-05 03:50:18.000000 abcparse-0.0.8/tests/test_ABCParse.py
```

### Comparing `ABCParse-0.0.7rc1/ABCParse/_abc_parse.py` & `abcparse-0.0.8/ABCParse/_abc_parse.py`

 * *Files identical despite different names*

### Comparing `ABCParse-0.0.7rc1/ABCParse/_as_list.py` & `abcparse-0.0.8/ABCParse/_as_list.py`

 * *Files identical despite different names*

### Comparing `ABCParse-0.0.7rc1/ABCParse/_function_kwargs.py` & `abcparse-0.0.8/ABCParse/_function_kwargs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 # -- import packages: --------------------------------------------------------------------
-from typing import Union, Dict, List
+from typing import Any, Callable, Dict, List, Union
 import inspect
 
 
 # -- operational class: ------------------------------------------------------------------
 class KwargExtractor:
     def __init__(self, func):
         self.func = func
@@ -65,29 +65,32 @@
         self._ignore = ignore
         self.__parse__(kwargs, parse_ignore=["self"])
 
         return self.query()
 
 
 # -- API-facing function: ----------------------------------------------------------------
-def function_kwargs(func, kwargs=None, obj=None, ignore=["self"]):
+def function_kwargs(
+    func: Callable,
+    kwargs: Dict[str,Any] = None,
+    obj: Any = None,
+    ignore: List[str] = ["self", "kwargs"],
+):
     """
     Returns the subset of kwargs that can be used in the func.
 
-    Parameters:
-    -----------
-    func
-
-    kwargs
-        if obj is passed, this argument is overridden.
-
-    obj
-        if kwargs is passed, obj overrides.
+    Args:
+        func (Callable): 
+    
+        kwargs
+            if obj is passed, this argument is overridden.
+    
+        obj
+            if kwargs is passed, obj overrides.
 
     Returns:
-    --------
-    function_kwargs
-        type: list
+        function_kwargs
+            type: list
     """
 
-    kwarg_extractor = KwargExtractor(func)
-    return kwarg_extractor(kwargs, obj)
+    kwarg_extractor = KwargExtractor(func=func)
+    return kwarg_extractor(kwargs=kwargs, obj=obj, ignore=ignore)
```

### Comparing `ABCParse-0.0.7rc1/ABCParse/_info_message.py` & `abcparse-0.0.8/ABCParse/_info_message.py`

 * *Files identical despite different names*

### Comparing `ABCParse-0.0.7rc1/ABCParse.egg-info/PKG-INFO` & `abcparse-0.0.8/ABCParse.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: ABCParse
-Version: 0.0.7rc1
+Version: 0.0.8
 Summary: A better base class to automatically parse local args.
 Author: Michael E. Vinyard
 Author-email: mvinyard.ai@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: licorice_font
 
 # ABCParse
 
 ![Python Tests](https://github.com/mvinyard/ABCParse/actions/workflows/python-tests.yml/badge.svg)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/ABCParse.svg)](https://pypi.python.org/pypi/ABCParse/)
 [![PyPI version](https://badge.fury.io/py/ABCParse.svg)](https://badge.fury.io/py/ABCParse)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `ABCParse-0.0.7rc1/LICENSE` & `abcparse-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ABCParse-0.0.7rc1/PKG-INFO` & `abcparse-0.0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: ABCParse
-Version: 0.0.7rc1
+Version: 0.0.8
 Summary: A better base class to automatically parse local args.
 Author: Michael E. Vinyard
 Author-email: mvinyard.ai@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: licorice_font
 
 # ABCParse
 
 ![Python Tests](https://github.com/mvinyard/ABCParse/actions/workflows/python-tests.yml/badge.svg)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/ABCParse.svg)](https://pypi.python.org/pypi/ABCParse/)
 [![PyPI version](https://badge.fury.io/py/ABCParse.svg)](https://badge.fury.io/py/ABCParse)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `ABCParse-0.0.7rc1/README.md` & `abcparse-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ABCParse-0.0.7rc1/tests/test_ABCParse.py` & `abcparse-0.0.8/tests/test_ABCParse.py`

 * *Files identical despite different names*

