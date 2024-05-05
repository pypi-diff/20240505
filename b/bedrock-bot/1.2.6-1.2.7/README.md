# Comparing `tmp/bedrock_bot-1.2.6.tar.gz` & `tmp/bedrock_bot-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bedrock_bot-1.2.6.tar", max compression
+gzip compressed data, was "bedrock_bot-1.2.7.tar", max compression
```

## Comparing `bedrock_bot-1.2.6.tar` & `bedrock_bot-1.2.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1068 2024-05-01 02:13:58.771954 bedrock_bot-1.2.6/LICENSE
--rw-r--r--   0        0        0     4039 2024-05-01 02:13:58.771954 bedrock_bot-1.2.6/README.md
--rw-r--r--   0        0        0      120 2024-05-01 02:13:58.771954 bedrock_bot-1.2.6/bedrock_bot/__init__.py
--rw-r--r--   0        0        0     4619 2024-05-01 02:13:58.771954 bedrock_bot-1.2.6/bedrock_bot/cli.py
--rw-r--r--   0        0        0      143 2024-05-01 02:13:58.771954 bedrock_bot-1.2.6/bedrock_bot/models/__init__.py
--rw-r--r--   0        0        0     2220 2024-05-01 02:13:58.771954 bedrock_bot-1.2.6/bedrock_bot/models/base_model.py
--rw-r--r--   0        0        0     1610 2024-05-01 02:13:58.771954 bedrock_bot-1.2.6/bedrock_bot/models/claude.py
--rw-r--r--   0        0        0     1326 2024-05-01 02:13:58.771954 bedrock_bot-1.2.6/bedrock_bot/models/mistral.py
--rw-r--r--   0        0        0      188 2024-05-01 02:13:58.771954 bedrock_bot-1.2.6/bedrock_bot/util.py
--rw-r--r--   0        0        0      633 2024-05-01 02:13:58.771954 bedrock_bot-1.2.6/pyproject.toml
--rw-r--r--   0        0        0     4542 1970-01-01 00:00:00.000000 bedrock_bot-1.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-05 07:05:07.795351 bedrock_bot-1.2.7/LICENSE
+-rw-r--r--   0        0        0     4039 2024-05-05 07:05:07.795351 bedrock_bot-1.2.7/README.md
+-rw-r--r--   0        0        0      120 2024-05-05 07:05:07.795351 bedrock_bot-1.2.7/bedrock_bot/__init__.py
+-rw-r--r--   0        0        0     4619 2024-05-05 07:05:07.795351 bedrock_bot-1.2.7/bedrock_bot/cli.py
+-rw-r--r--   0        0        0      143 2024-05-05 07:05:07.795351 bedrock_bot-1.2.7/bedrock_bot/models/__init__.py
+-rw-r--r--   0        0        0     2220 2024-05-05 07:05:07.795351 bedrock_bot-1.2.7/bedrock_bot/models/base_model.py
+-rw-r--r--   0        0        0     3128 2024-05-05 07:05:07.795351 bedrock_bot-1.2.7/bedrock_bot/models/claude.py
+-rw-r--r--   0        0        0     1326 2024-05-05 07:05:07.795351 bedrock_bot-1.2.7/bedrock_bot/models/mistral.py
+-rw-r--r--   0        0        0      188 2024-05-05 07:05:07.795351 bedrock_bot-1.2.7/bedrock_bot/util.py
+-rw-r--r--   0        0        0      633 2024-05-05 07:05:07.795351 bedrock_bot-1.2.7/pyproject.toml
+-rw-r--r--   0        0        0     4542 1970-01-01 00:00:00.000000 bedrock_bot-1.2.7/PKG-INFO
```

### Comparing `bedrock_bot-1.2.6/LICENSE` & `bedrock_bot-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.2.6/README.md` & `bedrock_bot-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.2.6/bedrock_bot/cli.py` & `bedrock_bot-1.2.7/bedrock_bot/cli.py`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.2.6/bedrock_bot/models/base_model.py` & `bedrock_bot-1.2.7/bedrock_bot/models/base_model.py`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.2.6/bedrock_bot/models/mistral.py` & `bedrock_bot-1.2.7/bedrock_bot/models/mistral.py`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.2.6/pyproject.toml` & `bedrock_bot-1.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bedrock-bot"
-version = "1.2.6"
+version = "1.2.7"
 description = ""
 authors = ["Justin Dray <justin@dray.be>"]
 readme = "README.md"
 
 [tool.ruff.lint]
 select = ["ALL"]
 ignore = ["D100", "D101", "D103", "D104", "D105", "D107", "ANN101", "G004"]
```

### Comparing `bedrock_bot-1.2.6/PKG-INFO` & `bedrock_bot-1.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bedrock-bot
-Version: 1.2.6
+Version: 1.2.7
 Summary: 
 Author: Justin Dray
 Author-email: justin@dray.be
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

