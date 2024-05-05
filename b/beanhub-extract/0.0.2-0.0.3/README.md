# Comparing `tmp/beanhub_extract-0.0.2.tar.gz` & `tmp/beanhub_extract-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beanhub_extract-0.0.2.tar", max compression
+gzip compressed data, was "beanhub_extract-0.0.3.tar", max compression
```

## Comparing `beanhub_extract-0.0.2.tar` & `beanhub_extract-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1072 2024-05-05 00:26:26.608346 beanhub_extract-0.0.2/LICENSE
--rw-r--r--   0        0        0      165 2024-05-05 00:26:26.608346 beanhub_extract-0.0.2/README.md
--rw-r--r--   0        0        0        0 2024-05-05 00:26:26.608346 beanhub_extract-0.0.2/beanhub_extract/__init__.py
--rw-r--r--   0        0        0     1502 2024-05-05 00:26:26.608346 beanhub_extract-0.0.2/beanhub_extract/data_types.py
--rw-r--r--   0        0        0        0 2024-05-05 00:26:26.608346 beanhub_extract-0.0.2/beanhub_extract/extractors/__init__.py
--rw-r--r--   0        0        0     1774 2024-05-05 00:26:26.608346 beanhub_extract-0.0.2/beanhub_extract/extractors/mercury.py
--rw-r--r--   0        0        0      977 2024-05-05 00:26:26.608346 beanhub_extract-0.0.2/beanhub_extract/utils.py
--rw-r--r--   0        0        0      595 2024-05-05 00:26:26.608346 beanhub_extract-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      853 1970-01-01 00:00:00.000000 beanhub_extract-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-05 06:34:17.640603 beanhub_extract-0.0.3/LICENSE
+-rw-r--r--   0        0        0      165 2024-05-05 06:34:17.640603 beanhub_extract-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-05 06:34:17.640603 beanhub_extract-0.0.3/beanhub_extract/__init__.py
+-rw-r--r--   0        0        0     1502 2024-05-05 06:34:17.640603 beanhub_extract-0.0.3/beanhub_extract/data_types.py
+-rw-r--r--   0        0        0      115 2024-05-05 06:34:17.640603 beanhub_extract-0.0.3/beanhub_extract/extractors/__init__.py
+-rw-r--r--   0        0        0     1774 2024-05-05 06:34:17.640603 beanhub_extract-0.0.3/beanhub_extract/extractors/mercury.py
+-rw-r--r--   0        0        0      977 2024-05-05 06:34:17.640603 beanhub_extract-0.0.3/beanhub_extract/utils.py
+-rw-r--r--   0        0        0      578 2024-05-05 06:34:17.640603 beanhub_extract-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 beanhub_extract-0.0.3/PKG-INFO
```

### Comparing `beanhub_extract-0.0.2/LICENSE` & `beanhub_extract-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `beanhub_extract-0.0.2/beanhub_extract/data_types.py` & `beanhub_extract-0.0.3/beanhub_extract/data_types.py`

 * *Files identical despite different names*

### Comparing `beanhub_extract-0.0.2/beanhub_extract/extractors/mercury.py` & `beanhub_extract-0.0.3/beanhub_extract/extractors/mercury.py`

 * *Files identical despite different names*

### Comparing `beanhub_extract-0.0.2/beanhub_extract/utils.py` & `beanhub_extract-0.0.3/beanhub_extract/utils.py`

 * *Files identical despite different names*

### Comparing `beanhub_extract-0.0.2/pyproject.toml` & `beanhub_extract-0.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 [tool.poetry]
 name = "beanhub-extract"
-version = "0.0.2"
+version = "0.0.3"
 description = "The simple library for extracting all kind of bank account transaction export files, mostly for beanhub-import to inject and generate transactions"
 authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-click = "^8.1.7"
 pytz = "^2024.1"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.1"
 pytest-mock = "^3.11.1"
```

### Comparing `beanhub_extract-0.0.2/PKG-INFO` & `beanhub_extract-0.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: beanhub-extract
-Version: 0.0.2
+Version: 0.0.3
 Summary: The simple library for extracting all kind of bank account transaction export files, mostly for beanhub-import to inject and generate transactions
 License: MIT
 Author: Fang-Pen Lin
 Author-email: fangpen@launchplatform.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: pytz (>=2024.1,<2025.0)
 Description-Content-Type: text/markdown
 
 # beanhub-extract
 The simple library for extracting all kind of bank account transaction export files, mostly for beanhub-import to inject and generate transactions
```

