# Comparing `tmp/flashgeotext-0.5.2.tar.gz` & `tmp/flashgeotext-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flashgeotext-0.5.2.tar", max compression
+gzip compressed data, was "flashgeotext-0.5.3.tar", max compression
```

## Comparing `flashgeotext-0.5.2.tar` & `flashgeotext-0.5.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1060 2024-02-19 14:13:53.710558 flashgeotext-0.5.2/LICENSE
--rw-r--r--   0        0        0       22 2024-02-19 14:13:54.502556 flashgeotext-0.5.2/flashgeotext/__init__.py
--rw-r--r--   0        0        0      343 2024-02-19 14:13:53.714558 flashgeotext-0.5.2/flashgeotext/config.py
--rw-r--r--   0        0        0     5552 2024-02-19 14:13:53.714558 flashgeotext-0.5.2/flashgeotext/geotext.py
--rw-r--r--   0        0        0     7727 2024-02-19 14:13:53.714558 flashgeotext-0.5.2/flashgeotext/lookup.py
--rw-r--r--   0        0        0  1503911 2024-02-19 14:13:53.742558 flashgeotext-0.5.2/flashgeotext/resources/cities.json
--rw-r--r--   0        0        0    17030 2024-02-19 14:13:53.742558 flashgeotext-0.5.2/flashgeotext/resources/countries.json
--rw-r--r--   0        0        0    46940 2024-02-19 14:13:53.742558 flashgeotext-0.5.2/flashgeotext/resources/scripts.json
--rw-r--r--   0        0        0      408 2024-02-19 14:13:53.742558 flashgeotext-0.5.2/flashgeotext/settings.py
--rw-r--r--   0        0        0     2934 2024-02-19 14:13:54.502556 flashgeotext-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     3012 2024-02-19 14:13:53.742558 flashgeotext-0.5.2/readme.md
--rw-r--r--   0        0        0     4136 1970-01-01 00:00:00.000000 flashgeotext-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-05-05 07:51:42.751096 flashgeotext-0.5.3/LICENSE
+-rw-r--r--   0        0        0       22 2024-05-05 07:51:44.335097 flashgeotext-0.5.3/flashgeotext/__init__.py
+-rw-r--r--   0        0        0      343 2024-05-05 07:51:42.751096 flashgeotext-0.5.3/flashgeotext/config.py
+-rw-r--r--   0        0        0     5552 2024-05-05 07:51:42.751096 flashgeotext-0.5.3/flashgeotext/geotext.py
+-rw-r--r--   0        0        0     7727 2024-05-05 07:51:42.755096 flashgeotext-0.5.3/flashgeotext/lookup.py
+-rw-r--r--   0        0        0  1503911 2024-05-05 07:51:42.779096 flashgeotext-0.5.3/flashgeotext/resources/cities.json
+-rw-r--r--   0        0        0    17030 2024-05-05 07:51:42.779096 flashgeotext-0.5.3/flashgeotext/resources/countries.json
+-rw-r--r--   0        0        0    46940 2024-05-05 07:51:42.779096 flashgeotext-0.5.3/flashgeotext/resources/scripts.json
+-rw-r--r--   0        0        0      408 2024-05-05 07:51:42.779096 flashgeotext-0.5.3/flashgeotext/settings.py
+-rw-r--r--   0        0        0     2985 2024-05-05 07:51:44.335097 flashgeotext-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     3012 2024-05-05 07:51:42.779096 flashgeotext-0.5.3/readme.md
+-rw-r--r--   0        0        0     4136 1970-01-01 00:00:00.000000 flashgeotext-0.5.3/PKG-INFO
```

### Comparing `flashgeotext-0.5.2/LICENSE` & `flashgeotext-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flashgeotext-0.5.2/flashgeotext/geotext.py` & `flashgeotext-0.5.3/flashgeotext/geotext.py`

 * *Files identical despite different names*

### Comparing `flashgeotext-0.5.2/flashgeotext/lookup.py` & `flashgeotext-0.5.3/flashgeotext/lookup.py`

 * *Files identical despite different names*

### Comparing `flashgeotext-0.5.2/flashgeotext/resources/cities.json` & `flashgeotext-0.5.3/flashgeotext/resources/cities.json`

 * *Files identical despite different names*

### Comparing `flashgeotext-0.5.2/flashgeotext/resources/countries.json` & `flashgeotext-0.5.3/flashgeotext/resources/countries.json`

 * *Files identical despite different names*

### Comparing `flashgeotext-0.5.2/flashgeotext/resources/scripts.json` & `flashgeotext-0.5.3/flashgeotext/resources/scripts.json`

 * *Files identical despite different names*

### Comparing `flashgeotext-0.5.2/pyproject.toml` & `flashgeotext-0.5.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flashgeotext"
-version = "0.5.2"
+version = "0.5.3"
 description = "Extract and count countries and cities (+their synonyms) from text"
 authors = ["Benjamin Ramser <ahoi@iwpnd.pw>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://flashgeotext.iwpnd.pw"
 repository = "https://github.com/iwpnd/flashgeotext"
 keywords = ["geonames", "nlp", "text extraction"]
@@ -24,56 +24,62 @@
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10.0"
 flashtext = "^2.7"
 loguru = ">=0.5.3"
-pydantic = "^2.6.1"
+pydantic = "^2.7.1"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^8.0.1"
-pytest-cov = "^4.0.0"
-pre-commit = "^3.6.2"
-black = "^24.2.0"
+pytest = "^8.2.0"
+pytest-cov = "^5.0.0"
+pre-commit = "^3.7.0"
 gitlint = ">=0.18,<0.20"
 isort = "^5.10.1"
-poethepoet = ">=0.16.4,<0.25.0"
-python-semantic-release = "^9.1.0"
-ruff = "^0.2.2"
+poethepoet = "^0.26.1"
+python-semantic-release = "^9.6.0"
+ruff = "^0.4.3"
+idna = "^3.7"
 
 [tool.semantic_release]
 version_variables = [
     "flashgeotext/__init__.py:__version__",
     "pyproject.toml:version",
 ]
 
 commit_subject = "ci: release v{version}"
 branch = "master"
 upload_to_release = true
 build_command = "pip install poetry --upgrade && poetry build"
 
 [tool.semantic_release.commit_parser_options]
 allowed_tags = [
-    "build",
+    "feat",
+    "fix",
+    "refactor",
     "chore",
+    "build",
     "ci",
     "docs",
-    "feat",
-    "fix",
     "perf",
     "style",
-    "refactor",
     "test",
 ]
 minor_tags = ["feat"]
-patch_tags = ["fix", "perf"]
+patch_tags = ["fix", "perf", "docs"]
 
 [tool.semantic_release.changelog]
-exclude_commit_patterns = ["build(deps-dev)", "chore(deps-dev)", "chore:", "ci:"]
+exclude_commit_patterns = [
+  "chore\\(release\\):",
+  "chore\\(deps-dev\\):",
+  "build\\(deps-dev\\):",
+  "build\\(deps\\):",
+  "ci:",
+]
 
 [tool.mypy]
 ignore_missing_imports = true
 
 [tool.ruff]
 line-length = 88
```

### Comparing `flashgeotext-0.5.2/readme.md` & `flashgeotext-0.5.3/readme.md`

 * *Files identical despite different names*

### Comparing `flashgeotext-0.5.2/PKG-INFO` & `flashgeotext-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashgeotext
-Version: 0.5.2
+Version: 0.5.3
 Summary: Extract and count countries and cities (+their synonyms) from text
 Home-page: https://flashgeotext.iwpnd.pw
 License: MIT
 Keywords: geonames,nlp,text extraction
 Author: Benjamin Ramser
 Author-email: ahoi@iwpnd.pw
 Requires-Python: >=3.10.0,<4.0.0
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: flashtext (>=2.7,<3.0)
 Requires-Dist: loguru (>=0.5.3)
-Requires-Dist: pydantic (>=2.6.1,<3.0.0)
+Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Project-URL: Repository, https://github.com/iwpnd/flashgeotext
 Description-Content-Type: text/markdown
 
 <p align="center">
 <a href="https://github.com/iwpnd/flashgeotext/actions" target="_blank">
     <img src="https://github.com/iwpnd/flashgeotext/workflows/CI/badge.svg?branch=master" alt="Build Status">
 </a>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: flashgeotext Version: 0.5.2 Summary: Extract and
+Metadata-Version: 2.1 Name: flashgeotext Version: 0.5.3 Summary: Extract and
 count countries and cities (+their synonyms) from text Home-page: https://
 flashgeotext.iwpnd.pw License: MIT Keywords: geonames,nlp,text extraction
 Author: Benjamin Ramser Author-email: ahoi@iwpnd.pw Requires-Python:
 >=3.10.0,<4.0.0 Classifier: Intended Audience :: Developers Classifier: License
 :: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
 Software Development :: Libraries :: Python Modules Classifier: Typing :: Typed
 Requires-Dist: flashtext (>=2.7,<3.0) Requires-Dist: loguru (>=0.5.3) Requires-
-Dist: pydantic (>=2.6.1,<3.0.0) Project-URL: Repository, https://github.com/
+Dist: pydantic (>=2.7.1,<3.0.0) Project-URL: Repository, https://github.com/
 iwpnd/flashgeotext Description-Content-Type: text/markdown
                            _[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_C_o_v_e_r_a_g_e_]
 --- # flashgeotext :zap::earth_africa: Extract and count countries and cities
 (+their synonyms) from text, like [GeoText](https://github.com/elyase/geotext)
 on steroids using [FlashText](https://github.com/vi3k6i5/flashtext/), a Aho-
 Corasick implementation. Flashgeotext is a fast, batteries-included (and BYOD)
 and native python library that extracts one or more sets of given city and
```

