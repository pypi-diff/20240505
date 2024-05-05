# Comparing `tmp/itunizer-1.0.5.tar.gz` & `tmp/itunizer-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itunizer-1.0.5.tar", max compression
+gzip compressed data, was "itunizer-1.0.6.tar", max compression
```

## Comparing `itunizer-1.0.5.tar` & `itunizer-1.0.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35147 2024-05-05 16:55:39.804868 itunizer-1.0.5/LICENSE
--rw-r--r--   0        0        0     1558 2024-05-05 16:55:39.805276 itunizer-1.0.5/README.md
--rw-r--r--   0        0        0        1 2024-05-05 16:55:39.805480 itunizer-1.0.5/itunizer/__init__.py
--rw-r--r--   0        0        0       35 2024-05-05 16:55:39.805570 itunizer-1.0.5/itunizer/__main__.py
--rw-r--r--   0        0        0     6250 2024-05-05 17:41:30.888830 itunizer-1.0.5/itunizer/itunizer.py
--rw-r--r--   0        0        0    24902 2024-05-05 17:00:26.877153 itunizer-1.0.5/itunizer/nginx.json
--rw-r--r--   0        0        0      630 2024-05-05 17:49:17.848430 itunizer-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     2436 1970-01-01 00:00:00.000000 itunizer-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    35147 2024-05-05 16:55:39.804868 itunizer-1.0.6/LICENSE
+-rw-r--r--   0        0        0     1558 2024-05-05 16:55:39.805276 itunizer-1.0.6/README.md
+-rw-r--r--   0        0        0        1 2024-05-05 16:55:39.805480 itunizer-1.0.6/itunizer/__init__.py
+-rw-r--r--   0        0        0       35 2024-05-05 16:55:39.805570 itunizer-1.0.6/itunizer/__main__.py
+-rw-r--r--   0        0        0     6250 2024-05-05 17:59:26.868402 itunizer-1.0.6/itunizer/itunizer.py
+-rw-r--r--   0        0        0    24902 2024-05-05 17:00:26.877153 itunizer-1.0.6/itunizer/nginx.json
+-rw-r--r--   0        0        0      630 2024-05-05 17:59:35.122992 itunizer-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2436 1970-01-01 00:00:00.000000 itunizer-1.0.6/PKG-INFO
```

### Comparing `itunizer-1.0.5/LICENSE` & `itunizer-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `itunizer-1.0.5/README.md` & `itunizer-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `itunizer-1.0.5/itunizer/itunizer.py` & `itunizer-1.0.6/itunizer/itunizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from pprint import pprint
 from statistics import mean, median
 
 import pandas as pd
 import requests
 
 # globals
-__version__ = "1.0.5"
+__version__ = "1.0.6"
 logo = """
 ┌────────────────────────┐
 │            ┌───▶       │
 │        ┌───┘   │       │
 │        │   ┌───▶       │
 │        │───┘   │       │
 │        │       │       │
```

### Comparing `itunizer-1.0.5/itunizer/nginx.json` & `itunizer-1.0.6/itunizer/nginx.json`

 * *Files identical despite different names*

### Comparing `itunizer-1.0.5/pyproject.toml` & `itunizer-1.0.6/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "itunizer"
-version = "1.0.5"
+version = "1.0.6"
 description = "A command line tool to search and compare prices of apps and music on the Apple Store"
 authors = ["James Campbell <james@jamescampbell.us>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 argparse = "^1.4.0"
```

### Comparing `itunizer-1.0.5/PKG-INFO` & `itunizer-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itunizer
-Version: 1.0.5
+Version: 1.0.6
 Summary: A command line tool to search and compare prices of apps and music on the Apple Store
 Author: James Campbell
 Author-email: james@jamescampbell.us
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

