# Comparing `tmp/beancount_black-1.0.1.tar.gz` & `tmp/beancount_black-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beancount_black-1.0.1.tar", max compression
+gzip compressed data, was "beancount_black-1.0.2.tar", max compression
```

## Comparing `beancount_black-1.0.1.tar` & `beancount_black-1.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2024-04-18 08:12:10.851392 beancount_black-1.0.1/LICENSE
--rw-r--r--   0        0        0     4247 2024-04-18 08:12:10.851392 beancount_black-1.0.1/README.md
--rw-r--r--   0        0        0        0 2024-04-18 08:12:10.851392 beancount_black-1.0.1/beancount_black/__init__.py
--rw-r--r--   0        0        0    27221 2024-04-18 08:12:10.851392 beancount_black-1.0.1/beancount_black/formatter.py
--rw-r--r--   0        0        0     3208 2024-04-18 08:12:10.851392 beancount_black-1.0.1/beancount_black/main.py
--rw-r--r--   0        0        0      629 2024-04-18 08:12:10.855392 beancount_black-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     5018 1970-01-01 00:00:00.000000 beancount_black-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-05 17:24:36.818875 beancount_black-1.0.2/LICENSE
+-rw-r--r--   0        0        0     4247 2024-05-05 17:24:36.818875 beancount_black-1.0.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-05 17:24:36.818875 beancount_black-1.0.2/beancount_black/__init__.py
+-rw-r--r--   0        0        0    27221 2024-05-05 17:24:36.818875 beancount_black-1.0.2/beancount_black/formatter.py
+-rw-r--r--   0        0        0     3208 2024-05-05 17:24:36.818875 beancount_black-1.0.2/beancount_black/main.py
+-rw-r--r--   0        0        0      619 2024-05-05 17:24:36.818875 beancount_black-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5018 1970-01-01 00:00:00.000000 beancount_black-1.0.2/PKG-INFO
```

### Comparing `beancount_black-1.0.1/LICENSE` & `beancount_black-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `beancount_black-1.0.1/README.md` & `beancount_black-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `beancount_black-1.0.1/beancount_black/formatter.py` & `beancount_black-1.0.2/beancount_black/formatter.py`

 * *Files identical despite different names*

### Comparing `beancount_black-1.0.1/beancount_black/main.py` & `beancount_black-1.0.2/beancount_black/main.py`

 * *Files identical despite different names*

### Comparing `beancount_black-1.0.1/pyproject.toml` & `beancount_black-1.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "beancount-black"
-version = "1.0.1"
+version = "1.0.2"
 description = "Opinioned code formatter, just like Python's black code formatter but for Beancount"
 authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
 license = "MIT"
 repository = "https://github.com/LaunchPlatform/beancount-black"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-beancount-parser = ">= 1.0.0, <2.0.0"
+beancount-parser = "^1.0.1"
 click = ">=7.0.0, <9.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.1"
 
 [tool.poetry.scripts]
 bean-black = 'beancount_black.main:main'
```

### Comparing `beancount_black-1.0.1/PKG-INFO` & `beancount_black-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: beancount-black
-Version: 1.0.1
+Version: 1.0.2
 Summary: Opinioned code formatter, just like Python's black code formatter but for Beancount
 Home-page: https://github.com/LaunchPlatform/beancount-black
 License: MIT
 Author: Fang-Pen Lin
 Author-email: fangpen@launchplatform.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: beancount-parser (>=1.0.0,<2.0.0)
+Requires-Dist: beancount-parser (>=1.0.1,<2.0.0)
 Requires-Dist: click (>=7.0.0,<9.0.0)
 Project-URL: Repository, https://github.com/LaunchPlatform/beancount-black
 Description-Content-Type: text/markdown
 
 # beancount-black [![CircleCI](https://circleci.com/gh/LaunchPlatform/beancount-black/tree/master.svg?style=svg)](https://circleci.com/gh/LaunchPlatform/beancount-black/tree/master)
 Opinionated code formatter, just like Python's [black](https://pypi.org/project/black/) code formatter but for Beancount
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: beancount-black Version: 1.0.1 Summary: Opinioned
+Metadata-Version: 2.1 Name: beancount-black Version: 1.0.2 Summary: Opinioned
 code formatter, just like Python's black code formatter but for Beancount Home-
 page: https://github.com/LaunchPlatform/beancount-black License: MIT Author:
 Fang-Pen Lin Author-email: fangpen@launchplatform.com Requires-Python:
 >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: beancount-parser
-(>=1.0.0,<2.0.0) Requires-Dist: click (>=7.0.0,<9.0.0) Project-URL: Repository,
+(>=1.0.1,<2.0.0) Requires-Dist: click (>=7.0.0,<9.0.0) Project-URL: Repository,
 https://github.com/LaunchPlatform/beancount-black Description-Content-Type:
 text/markdown # beancount-black [![CircleCI](https://circleci.com/gh/
 LaunchPlatform/beancount-black/tree/master.svg?style=svg)](https://
 circleci.com/gh/LaunchPlatform/beancount-black/tree/master) Opinionated code
 formatter, just like Python's [black](https://pypi.org/project/black/) code
 formatter but for Beancount Try it out online [here](https://app.beanhub.io/
 tools/beancount-formatter) ## Features - **MIT licensed** - based on
```

