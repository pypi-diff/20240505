# Comparing `tmp/pytilpack-0.2.3.tar.gz` & `tmp/pytilpack-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytilpack-0.2.3.tar", max compression
+gzip compressed data, was "pytilpack-0.3.0.tar", max compression
```

## Comparing `pytilpack-0.2.3.tar` & `pytilpack-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,13 @@
--rw-r--r--   0        0        0     1061 2024-05-04 10:20:38.680437 pytilpack-0.2.3/LICENSE
--rw-r--r--   0        0        0      503 2024-05-04 10:20:38.680437 pytilpack-0.2.3/README.md
--rw-r--r--   0        0        0     2182 2024-05-04 10:20:54.532510 pytilpack-0.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-04 10:20:38.684437 pytilpack-0.2.3/pytilpack/__init__.py
--rw-r--r--   0        0        0     1920 2024-05-04 10:20:38.684437 pytilpack-0.2.3/pytilpack/flask_.py
--rw-r--r--   0        0        0     4444 2024-05-04 10:20:38.684437 pytilpack-0.2.3/pytilpack/openai_.py
--rw-r--r--   0        0        0      690 2024-05-04 10:20:38.684437 pytilpack-0.2.3/pytilpack/python_.py
--rw-r--r--   0        0        0     2392 2024-05-04 10:20:38.684437 pytilpack-0.2.3/pytilpack/sqlalchemy_.py
--rw-r--r--   0        0        0      523 2024-05-04 10:20:38.684437 pytilpack-0.2.3/pytilpack/tqdm_.py
--rw-r--r--   0        0        0     1621 1970-01-01 00:00:00.000000 pytilpack-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-05-05 13:35:01.448651 pytilpack-0.3.0/LICENSE
+-rw-r--r--   0        0        0      503 2024-05-05 13:35:01.448651 pytilpack-0.3.0/README.md
+-rw-r--r--   0        0        0     2409 2024-05-05 13:35:15.004858 pytilpack-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-05 13:35:01.448651 pytilpack-0.3.0/pytilpack/__init__.py
+-rw-r--r--   0        0        0      942 2024-05-05 13:35:01.448651 pytilpack-0.3.0/pytilpack/csv_.py
+-rw-r--r--   0        0        0     1920 2024-05-05 13:35:01.448651 pytilpack-0.3.0/pytilpack/flask_.py
+-rw-r--r--   0        0        0     4556 2024-05-05 13:35:01.448651 pytilpack-0.3.0/pytilpack/openai_.py
+-rw-r--r--   0        0        0      566 2024-05-05 13:35:01.448651 pytilpack-0.3.0/pytilpack/pathlib_.py
+-rw-r--r--   0        0        0      690 2024-05-05 13:35:01.448651 pytilpack-0.3.0/pytilpack/python_.py
+-rw-r--r--   0        0        0     2392 2024-05-05 13:35:01.448651 pytilpack-0.3.0/pytilpack/sqlalchemy_.py
+-rw-r--r--   0        0        0     8055 2024-05-05 13:35:01.448651 pytilpack-0.3.0/pytilpack/tiktoken_.py
+-rw-r--r--   0        0        0      523 2024-05-05 13:35:01.448651 pytilpack-0.3.0/pytilpack/tqdm_.py
+-rw-r--r--   0        0        0     1864 1970-01-01 00:00:00.000000 pytilpack-0.3.0/PKG-INFO
```

### Comparing `pytilpack-0.2.3/LICENSE` & `pytilpack-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytilpack-0.2.3/pyproject.toml` & `pytilpack-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytilpack"
-version = "0.2.3"  # using poetry-dynamic-versioning
+version = "0.3.0"  # using poetry-dynamic-versioning
 description = "Python Utility Pack"
 license = "MIT"
 authors = ["aki. <mark@aur.ll.to>"]
 readme = "README.md"
 homepage = "https://github.com/ak110/pytilpack"
 classifiers = [
     "Environment :: Console",
@@ -16,32 +16,39 @@
 [tool.poetry-dynamic-versioning]
 enable = false
 style = "pep440"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 flask = {version = ">=2.2", optional = true}
+httpx = {version = "*", optional = true}
 openai = {version = ">=1.25", optional = true}
+pillow = {version = "*", optional = true}
 sqlalchemy = {version = ">=2.0", optional = true}
+tiktoken = {version = ">=0.6", optional = true}
 tqdm = {version = ">=4.66", optional = true}
 typing-extensions = ">=4.0"
 
 [tool.poetry.group.dev.dependencies]
 pyfltr = "*"
 
 [tool.poetry.extras]
 all = [
     "flask",
+    "httpx",
     "openai",
+    "pillow",
     "sqlalchemy",
+    "tiktoken",
     "tqdm",
 ]
 flask = ["flask"]
 openai = ["openai"]
 sqlalchemy = ["sqlalchemy"]
+tiktoken = ["tiktoken", "openai", "httpx", "pillow"]
 tqdm = ["tqdm"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.pyfltr]
```

### Comparing `pytilpack-0.2.3/pytilpack/flask_.py` & `pytilpack-0.3.0/pytilpack/flask_.py`

 * *Files identical despite different names*

### Comparing `pytilpack-0.2.3/pytilpack/openai_.py` & `pytilpack-0.3.0/pytilpack/openai_.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 """OpenAI Python Library用のユーティリティ集。"""
 
+import logging
+
 import openai
 import openai.types.chat
 
 import pytilpack.python_
 
+logger = logging.getLogger(__name__)
+
 
 def gather_chunks(
     chunks: list[openai.types.chat.ChatCompletionChunk],
 ) -> openai.types.chat.ChatCompletion:
     """ストリーミングのチャンクを結合する。"""
     max_choices = max(len(chunk.choices) for chunk in chunks)
     choices = [_make_choice(chunks, i) for i in range(max_choices)]
     return openai.types.chat.ChatCompletion(
         id=chunks[0].id,
         choices=choices,
         created=chunks[0].created,
         model=chunks[0].model,
         object="chat.completion",
-        system_fingerprint=chunks[0].system_fingerprint,
+        system_fingerprint=pytilpack.python_.coalesce(
+            c.system_fingerprint for c in chunks
+        ),
     )
 
 
 def _make_choice(
     chunks: list[openai.types.chat.ChatCompletionChunk], i: int
 ) -> openai.types.chat.chat_completion.Choice:
     """ストリーミングのチャンクからChoiceを作成する。"""
```

### Comparing `pytilpack-0.2.3/pytilpack/python_.py` & `pytilpack-0.3.0/pytilpack/python_.py`

 * *Files identical despite different names*

### Comparing `pytilpack-0.2.3/pytilpack/sqlalchemy_.py` & `pytilpack-0.3.0/pytilpack/sqlalchemy_.py`

 * *Files identical despite different names*

### Comparing `pytilpack-0.2.3/pytilpack/tqdm_.py` & `pytilpack-0.3.0/pytilpack/tqdm_.py`

 * *Files identical despite different names*

### Comparing `pytilpack-0.2.3/PKG-INFO` & `pytilpack-0.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytilpack
-Version: 0.2.3
+Version: 0.3.0
 Summary: Python Utility Pack
 Home-page: https://github.com/ak110/pytilpack
 License: MIT
 Author: aki.
 Author-email: mark@aur.ll.to
 Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Console
@@ -16,18 +16,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Provides-Extra: all
 Provides-Extra: flask
 Provides-Extra: openai
 Provides-Extra: sqlalchemy
+Provides-Extra: tiktoken
 Provides-Extra: tqdm
 Requires-Dist: flask (>=2.2) ; extra == "all" or extra == "flask"
-Requires-Dist: openai (>=1.25) ; extra == "all" or extra == "openai"
+Requires-Dist: httpx ; extra == "all" or extra == "tiktoken"
+Requires-Dist: openai (>=1.25) ; extra == "all" or extra == "openai" or extra == "tiktoken"
+Requires-Dist: pillow ; extra == "all" or extra == "tiktoken"
 Requires-Dist: sqlalchemy (>=2.0) ; extra == "all" or extra == "sqlalchemy"
+Requires-Dist: tiktoken (>=0.6) ; extra == "all" or extra == "tiktoken"
 Requires-Dist: tqdm (>=4.66) ; extra == "all" or extra == "tqdm"
 Requires-Dist: typing-extensions (>=4.0)
 Description-Content-Type: text/markdown
 
 # pytilpack
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

