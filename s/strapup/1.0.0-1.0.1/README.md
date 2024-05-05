# Comparing `tmp/strapup-1.0.0.tar.gz` & `tmp/strapup-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strapup-1.0.0.tar", max compression
+gzip compressed data, was "strapup-1.0.1.tar", max compression
```

## Comparing `strapup-1.0.0.tar` & `strapup-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2024-05-04 13:39:30.020296 strapup-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0      530 2024-05-05 06:57:17.865270 strapup-1.0.0/README.txt
--rw-r--r--   0        0        0      284 2024-05-05 07:31:23.146925 strapup-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      451 2024-05-05 07:31:23.166925 strapup-1.0.0/src/strapup/__init__.py
--rw-r--r--   0        0        0     4078 2024-05-05 06:54:34.535154 strapup-1.0.0/src/strapup/logger.py
--rw-r--r--   0        0        0     1882 2024-05-05 07:31:23.196926 strapup-1.0.0/src/strapup/pystrap.py
--rw-r--r--   0        0        0     1179 1970-01-01 00:00:00.000000 strapup-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-04 13:39:30.020296 strapup-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0      562 2024-05-05 07:41:12.517413 strapup-1.0.1/README.txt
+-rw-r--r--   0        0        0      284 2024-05-05 07:42:12.266431 strapup-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      451 2024-05-05 07:31:23.166925 strapup-1.0.1/src/strapup/__init__.py
+-rw-r--r--   0        0        0     4089 2024-05-05 07:39:34.277949 strapup-1.0.1/src/strapup/logger.py
+-rw-r--r--   0        0        0     1882 2024-05-05 07:31:23.196926 strapup-1.0.1/src/strapup/pystrap.py
+-rw-r--r--   0        0        0     1211 1970-01-01 00:00:00.000000 strapup-1.0.1/PKG-INFO
```

### Comparing `strapup-1.0.0/LICENSE.txt` & `strapup-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `strapup-1.0.0/README.txt` & `strapup-1.0.1/README.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 
 Update pythonpath as need on startup of script. Create a custom logger, which can log to terminal and file at the same time, by simply choosing a name.
 
+python3 -m build
+python3 -m twine upload --verbose --skip-existing --repository pypi dist/*
+
 # python3 -m twine upload --repository testpypi dist/*
 # python3 -m twine upload --repository pypi dist/*
-# python3 -m twine upload --verbose --repository pypi dist/*
 
 # python3 -m pip install --upgrade build
 # python3 -m build
 
 # python3 -m pip install --upgrade twine
 # python3 -m twine upload --repository testpypi dist/*
 # python3 -m twine upload --repository pypi dist/*
```

### Comparing `strapup-1.0.0/src/strapup/logger.py` & `strapup-1.0.1/src/strapup/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 
+import os
 import logging
 import sys
 from datetime import datetime
 
 
 class Logger(logging.getLoggerClass()):
     def __init__(self, name, log_level='info', log_to_file=False, log_dir=None):
```

### Comparing `strapup-1.0.0/src/strapup/pystrap.py` & `strapup-1.0.1/src/strapup/pystrap.py`

 * *Files identical despite different names*

### Comparing `strapup-1.0.0/PKG-INFO` & `strapup-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strapup
-Version: 1.0.0
+Version: 1.0.1
 Summary: 
 License: MIT
 Author: Karl Rittner
 Author-email: k.rittner@hotmail.de
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,17 +16,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/plain
 
 
 Update pythonpath as need on startup of script. Create a custom logger, which can log to terminal and file at the same time, by simply choosing a name.
 
+python3 -m build
+python3 -m twine upload --verbose --skip-existing --repository pypi dist/*
+
 # python3 -m twine upload --repository testpypi dist/*
 # python3 -m twine upload --repository pypi dist/*
-# python3 -m twine upload --verbose --repository pypi dist/*
 
 # python3 -m pip install --upgrade build
 # python3 -m build
 
 # python3 -m pip install --upgrade twine
 # python3 -m twine upload --repository testpypi dist/*
 # python3 -m twine upload --repository pypi dist/*
```

