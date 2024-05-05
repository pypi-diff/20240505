# Comparing `tmp/mongopersistence-0.3.0.tar.gz` & `tmp/mongopersistence-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongopersistence-0.3.0.tar", max compression
+gzip compressed data, was "mongopersistence-0.3.1.tar", max compression
```

## Comparing `mongopersistence-0.3.0.tar` & `mongopersistence-0.3.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2023-04-15 11:26:21.541175 mongopersistence-0.3.0/LICENSE
--rw-r--r--   0        0        0     2492 2023-04-15 11:26:21.541350 mongopersistence-0.3.0/README.md
--rw-r--r--   0        0        0       80 2023-04-15 11:26:21.541580 mongopersistence-0.3.0/mongopersistence/__init__.py
--rw-r--r--   0        0        0    13729 2023-04-15 11:26:21.541800 mongopersistence-0.3.0/mongopersistence/persistence.py
--rw-r--r--   0        0        0      874 2023-04-15 11:26:21.542619 mongopersistence-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3055 1970-01-01 00:00:00.000000 mongopersistence-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-15 11:26:21.541175 mongopersistence-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2508 2024-05-05 14:50:27.553605 mongopersistence-0.3.1/README.md
+-rw-r--r--   0        0        0       58 2024-05-05 14:50:27.554111 mongopersistence-0.3.1/mongopersistence/__init__.py
+-rw-r--r--   0        0        0    13666 2024-05-05 14:50:27.554665 mongopersistence-0.3.1/mongopersistence/persistence.py
+-rw-r--r--   0        0        0      938 2024-05-05 14:50:27.556033 mongopersistence-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3065 1970-01-01 00:00:00.000000 mongopersistence-0.3.1/PKG-INFO
```

### Comparing `mongopersistence-0.3.0/LICENSE` & `mongopersistence-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mongopersistence-0.3.0/README.md` & `mongopersistence-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -66,7 +66,9 @@
 ```
 
 ## Roadmap
 
 Search all the TODOs in this repo to see how you can contribute to this package, but in general:
 
 - Add support for make persistent callback data.
+
+- Create tests
```

### Comparing `mongopersistence-0.3.0/mongopersistence/persistence.py` & `mongopersistence-0.3.1/mongopersistence/persistence.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,15 @@
 from copy import deepcopy
 from dataclasses import dataclass, field
 from typing import Any, Generic, TypeVar
 
 from motor.motor_asyncio import AsyncIOMotorClient, AsyncIOMotorCollection, AsyncIOMotorDatabase
 from pymongo.errors import CollectionInvalid
 from telegram.ext import BasePersistence, PersistenceInput
-
-# noinspection PyProtectedMember
-from telegram.ext._utils.types import (
-    BD,
-    CD,
-    UD,
-    CDCData,
-    ConversationDict,
-    ConversationKey,
-)
+from telegram.ext._utils.types import BD, CD, UD, CDCData, ConversationDict, ConversationKey
 
 BOT_DATA_KEY = 0
 
 NEW_DATA = BD | CD | UD | CDCData | ConversationDict
 
 logger = logging.getLogger(__name__)
 D = TypeVar("D", bound=dict)
```

### Comparing `mongopersistence-0.3.0/pyproject.toml` & `mongopersistence-0.3.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,42 @@
 [tool.poetry]
 name = "mongopersistence"
-version = "0.3.0"
+version = "0.3.1"
 description = "Package to add persistence to your telegram bot using pymongo"
 authors = ["LucaSforza <lucasforza1234@icloud.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-python-telegram-bot = "^20.1"
+python-telegram-bot = ">=20.1"
 motor = "^3.1.2"
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.3.0"
-pre-commit = "^2.20.0"
-ruff = "^0.0.261"
+pre-commit = "*"
+ruff = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.black]
-line-length = 120
-include = '\.pyi?$'
-force-exclude = '''
-/(
-    \.git
-  | \.hg
-  | \.mypy_cache
-  | \.ruff_cache
-  | locales/.*
-)/
-'''
 
 [tool.ruff]
 line-length = 120
 target-version = "py310"
+exclude = ["*locales*"]
+
+[tool.ruff.lint]
 select = [
     "E", # pyflakes
     "F", # pycodestyle errors
     "W", # pycodestyle warnings
     "UP", # pyupgrade
     "I", # isort
     "C4", # flake8-comprehensions
 ]
+ignore = ["E501"]
+ignore-init-module-imports = true
+
+[tool.ruff.lint.per-file-ignores]
+"__init__.py" = ["E402", "F401", "F403", "F405", "F811"]
+"__main__.py" = ["E402", "F401", "F403", "F405", "F811"]
```

### Comparing `mongopersistence-0.3.0/PKG-INFO` & `mongopersistence-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: mongopersistence
-Version: 0.3.0
+Version: 0.3.1
 Summary: Package to add persistence to your telegram bot using pymongo
 License: MIT
 Author: LucaSforza
 Author-email: lucasforza1234@icloud.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: motor (>=3.1.2,<4.0.0)
-Requires-Dist: python-telegram-bot (>=20.1,<21.0)
+Requires-Dist: python-telegram-bot (>=20.1)
 Description-Content-Type: text/markdown
 
 # MongoPersistence
 
 Package to add persistence to your telegram bot in a mongodb database.
 
 ATTENTION: MongoPersistence is a new project, it should work, but if you encounter any bugs, please report them in
@@ -83,7 +83,9 @@
 
 ## Roadmap
 
 Search all the TODOs in this repo to see how you can contribute to this package, but in general:
 
 - Add support for make persistent callback data.
 
+- Create tests
+
```

