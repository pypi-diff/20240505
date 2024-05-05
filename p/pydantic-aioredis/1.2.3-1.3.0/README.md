# Comparing `tmp/pydantic_aioredis-1.2.3.tar.gz` & `tmp/pydantic_aioredis-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_aioredis-1.2.3.tar", max compression
+gzip compressed data, was "pydantic_aioredis-1.3.0.tar", max compression
```

## Comparing `pydantic_aioredis-1.2.3.tar` & `pydantic_aioredis-1.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1262 2023-03-30 03:34:29.896730 pydantic_aioredis-1.2.3/LICENSE
--rw-r--r--   0        0        0     9389 2023-03-30 03:34:29.896730 pydantic_aioredis-1.2.3/README.md
--rw-r--r--   0        0        0      337 2023-03-30 03:34:29.900730 pydantic_aioredis-1.2.3/pydantic_aioredis/__init__.py
--rw-r--r--   0        0        0     5001 2023-03-30 03:34:29.900730 pydantic_aioredis-1.2.3/pydantic_aioredis/abstract.py
--rw-r--r--   0        0        0      756 2023-03-30 03:34:29.900730 pydantic_aioredis-1.2.3/pydantic_aioredis/config.py
--rw-r--r--   0        0        0      442 2023-03-30 03:34:29.900730 pydantic_aioredis-1.2.3/pydantic_aioredis/ext/FastAPI/__init__.py
--rw-r--r--   0        0        0     4026 2023-03-30 03:34:29.900730 pydantic_aioredis-1.2.3/pydantic_aioredis/ext/FastAPI/crudrouter.py
--rw-r--r--   0        0        0      926 2023-03-30 03:34:29.900730 pydantic_aioredis-1.2.3/pydantic_aioredis/ext/FastAPI/model.py
--rw-r--r--   0        0        0        0 2023-03-30 03:34:29.900730 pydantic_aioredis-1.2.3/pydantic_aioredis/ext/__init__.py
--rw-r--r--   0        0        0     9718 2023-03-30 03:34:29.900730 pydantic_aioredis-1.2.3/pydantic_aioredis/model.py
--rw-r--r--   0        0        0     1610 2023-03-30 03:34:29.900730 pydantic_aioredis-1.2.3/pydantic_aioredis/store.py
--rw-r--r--   0        0        0     1087 2023-03-30 03:34:29.900730 pydantic_aioredis-1.2.3/pydantic_aioredis/types.py
--rw-r--r--   0        0        0      178 2023-03-30 03:34:29.900730 pydantic_aioredis-1.2.3/pydantic_aioredis/utils.py
--rw-r--r--   0        0        0     2604 2023-03-30 03:34:29.900730 pydantic_aioredis-1.2.3/pyproject.toml
--rw-r--r--   0        0        0    11104 1970-01-01 00:00:00.000000 pydantic_aioredis-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1262 2024-05-05 20:23:09.205113 pydantic_aioredis-1.3.0/LICENSE
+-rw-r--r--   0        0        0     9916 2024-05-05 20:23:09.205113 pydantic_aioredis-1.3.0/README.md
+-rw-r--r--   0        0        0      338 2024-05-05 20:23:09.209113 pydantic_aioredis-1.3.0/pydantic_aioredis/__init__.py
+-rw-r--r--   0        0        0     4988 2024-05-05 20:23:09.209113 pydantic_aioredis-1.3.0/pydantic_aioredis/abstract.py
+-rw-r--r--   0        0        0      757 2024-05-05 20:23:09.209113 pydantic_aioredis-1.3.0/pydantic_aioredis/config.py
+-rw-r--r--   0        0        0      442 2024-05-05 20:23:09.209113 pydantic_aioredis-1.3.0/pydantic_aioredis/ext/FastAPI/__init__.py
+-rw-r--r--   0        0        0     4026 2024-05-05 20:23:09.209113 pydantic_aioredis-1.3.0/pydantic_aioredis/ext/FastAPI/crudrouter.py
+-rw-r--r--   0        0        0      960 2024-05-05 20:23:09.209113 pydantic_aioredis-1.3.0/pydantic_aioredis/ext/FastAPI/model.py
+-rw-r--r--   0        0        0        0 2024-05-05 20:23:09.209113 pydantic_aioredis-1.3.0/pydantic_aioredis/ext/__init__.py
+-rw-r--r--   0        0        0     9705 2024-05-05 20:23:09.209113 pydantic_aioredis-1.3.0/pydantic_aioredis/model.py
+-rw-r--r--   0        0        0     1581 2024-05-05 20:23:09.209113 pydantic_aioredis-1.3.0/pydantic_aioredis/store.py
+-rw-r--r--   0        0        0     1087 2024-05-05 20:23:09.209113 pydantic_aioredis-1.3.0/pydantic_aioredis/types.py
+-rw-r--r--   0        0        0      178 2024-05-05 20:23:09.209113 pydantic_aioredis-1.3.0/pydantic_aioredis/utils.py
+-rw-r--r--   0        0        0     2671 2024-05-05 20:23:09.209113 pydantic_aioredis-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0    11428 1970-01-01 00:00:00.000000 pydantic_aioredis-1.3.0/PKG-INFO
```

### Comparing `pydantic_aioredis-1.2.3/LICENSE` & `pydantic_aioredis-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_aioredis-1.2.3/README.md` & `pydantic_aioredis-1.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
   # oops, there was a typo. Fix it
   # Update is an async context manager and will update redis with all changes in one operations
   async with this_book.update():
     this_book.author = "Herman Melville"
     this_book.published_on=date(year=1851, month=10, day=18)
   this_book_from_redis = await Book.select(ids=["Moby Dick"])
   assert this_book_from_redis[0].author == "Herman Melville"
-  assert this_book_from_redis[0].author == date(year=1851, month=10, day=18)
+  assert this_book_from_redis[0].published_on == date(year=1851, month=10, day=18)
 
   # Delete any number of items
   await Library.delete(ids=["The Grand Library"])
 
 # Now run these updates
 loop = asyncio.get_event_loop()
 loop.run_until_complete(work_with_orm())
@@ -148,20 +148,21 @@
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
   <tbody>
     <tr>
-      <td align="center"><a href="https://github.com/andrewthetechie"><img src="https://avatars.githubusercontent.com/u/1377314?v=4?s=100" width="100px;" alt="Andrew"/><br /><sub><b>Andrew</b></sub></a><br /><a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=andrewthetechie" title="Code">💻</a> <a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=andrewthetechie" title="Documentation">📖</a></td>
-      <td align="center"><a href="https://github.com/Tinitto"><img src="https://avatars.githubusercontent.com/u/21363733??v=4?s=100" width="100px;" alt="Martin Ahindura"/><br /><sub><b>Martin Ahindura</b></sub></a><br /><a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=Tinitto" title="Code">💻</a> <a href="#ideas-Tinitto" title="Ideas, Planning, & Feedback">🤔</a></td>
-      <td align="center"><a href="https://github.com/david-wahlstedt"><img src="https://avatars.githubusercontent.com/u/66391333?v=4?s=100" width="100px;" alt="david-wahlstedt"/><br /><sub><b>david-wahlstedt</b></sub></a><br /><a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=david-wahlstedt" title="Tests">⚠️</a> <a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=david-wahlstedt" title="Documentation">📖</a> <a href="https://github.com/andrewthetechie/pydantic-aioredis/pulls?q=is%3Apr+reviewed-by%3Adavid-wahlstedt" title="Reviewed Pull Requests">👀</a></td>
-      <td align="center"><a href="https://blog.gtmanfred.com"><img src="https://avatars.githubusercontent.com/u/732321?v=4?s=100" width="100px;" alt="Daniel Wallace"/><br /><sub><b>Daniel Wallace</b></sub></a><br /><a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=gtmanfred" title="Tests">⚠️</a></td>
-      <td align="center"><a href="https://derwen.ai/paco"><img src="https://avatars.githubusercontent.com/u/57973?v=4?s=100" width="100px;" alt="Paco Nathan"/><br /><sub><b>Paco Nathan</b></sub></a><br /><a href="#example-ceteri" title="Examples">💡</a></td>
-      <td align="center"><a href="https://www.linkedin.com/in/andreas-brodersen-1b955b100/"><img src="https://avatars.githubusercontent.com/u/43907402?v=4?s=100" width="100px;" alt="Andreas Brodersen"/><br /><sub><b>Andreas Brodersen</b></sub></a><br /><a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=AndreasPB" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/andrewthetechie"><img src="https://avatars.githubusercontent.com/u/1377314?v=4?s=100" width="100px;" alt="Andrew"/><br /><sub><b>Andrew</b></sub></a><br /><a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=andrewthetechie" title="Code">💻</a> <a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=andrewthetechie" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Tinitto"><img src="https://avatars.githubusercontent.com/u/21363733??v=4?s=100" width="100px;" alt="Martin Ahindura"/><br /><sub><b>Martin Ahindura</b></sub></a><br /><a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=Tinitto" title="Code">💻</a> <a href="#ideas-Tinitto" title="Ideas, Planning, & Feedback">🤔</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/david-wahlstedt"><img src="https://avatars.githubusercontent.com/u/66391333?v=4?s=100" width="100px;" alt="david-wahlstedt"/><br /><sub><b>david-wahlstedt</b></sub></a><br /><a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=david-wahlstedt" title="Tests">⚠️</a> <a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=david-wahlstedt" title="Documentation">📖</a> <a href="https://github.com/andrewthetechie/pydantic-aioredis/pulls?q=is%3Apr+reviewed-by%3Adavid-wahlstedt" title="Reviewed Pull Requests">👀</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://blog.gtmanfred.com"><img src="https://avatars.githubusercontent.com/u/732321?v=4?s=100" width="100px;" alt="Daniel Wallace"/><br /><sub><b>Daniel Wallace</b></sub></a><br /><a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=gtmanfred" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://derwen.ai/paco"><img src="https://avatars.githubusercontent.com/u/57973?v=4?s=100" width="100px;" alt="Paco Nathan"/><br /><sub><b>Paco Nathan</b></sub></a><br /><a href="#example-ceteri" title="Examples">💡</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://www.linkedin.com/in/andreas-brodersen-1b955b100/"><img src="https://avatars.githubusercontent.com/u/43907402?v=4?s=100" width="100px;" alt="Andreas Brodersen"/><br /><sub><b>Andreas Brodersen</b></sub></a><br /><a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=AndreasPB" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/kraczak"><img src="https://avatars.githubusercontent.com/u/58468064?v=4?s=100" width="100px;" alt="kraczak"/><br /><sub><b>kraczak</b></sub></a><br /><a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=kraczak" title="Documentation">📖</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `pydantic_aioredis-1.2.3/pydantic_aioredis/abstract.py` & `pydantic_aioredis-1.3.0/pydantic_aioredis/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module containing the main base classes"""
+
 import json
 from datetime import date
 from datetime import datetime
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
@@ -126,17 +127,15 @@
 
     @classmethod
     async def delete(cls, ids: Union[Any, List[Any]]):  # pragma: no cover
         """Delete a key from the redis store"""
         raise NotImplementedError("delete should be implemented")
 
     @classmethod
-    async def select(
-        cls, columns: Optional[List[str]] = None, ids: Optional[List[Any]] = None
-    ):  # pragma: no cover
+    async def select(cls, columns: Optional[List[str]] = None, ids: Optional[List[Any]] = None):  # pragma: no cover
         """Select one or more object from the redis store"""
         raise NotImplementedError("select should be implemented")
 
     class Config:
         """Pydantic schema config for _AbstractModel"""
 
         arbitrary_types_allowed = True
```

### Comparing `pydantic_aioredis-1.2.3/pydantic_aioredis/config.py` & `pydantic_aioredis-1.3.0/pydantic_aioredis/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module containing the main config classes"""
+
 from typing import Optional
 
 from pydantic import BaseModel
 
 
 class RedisConfig(BaseModel):
     """A config object for connecting to redis"""
```

### Comparing `pydantic_aioredis-1.2.3/pydantic_aioredis/ext/FastAPI/crudrouter.py` & `pydantic_aioredis-1.3.0/pydantic_aioredis/ext/FastAPI/crudrouter.py`

 * *Files identical despite different names*

### Comparing `pydantic_aioredis-1.2.3/pydantic_aioredis/ext/FastAPI/model.py` & `pydantic_aioredis-1.3.0/pydantic_aioredis/ext/FastAPI/model.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,11 +22,13 @@
     ):
         """
         Selects given rows or sets of rows in the table.
         Raises a HTTPException with a 404 if there is no result
         """
         result = await cls.select(columns=columns, ids=ids)
         if result is None:
-            raise HTTPException(
-                status_code=404, detail=f"{cls.__name__} not found"
-            ) if custom_exception is None else custom_exception
+            raise (
+                HTTPException(status_code=404, detail=f"{cls.__name__} not found")
+                if custom_exception is None
+                else custom_exception
+            )
         return result
```

### Comparing `pydantic_aioredis-1.2.3/pydantic_aioredis/model.py` & `pydantic_aioredis-1.3.0/pydantic_aioredis/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module containing the model classes"""
+
 import asyncio
 from contextlib import asynccontextmanager
 from functools import lru_cache
 from sys import version_info
 from typing import Any
 from typing import List
 from typing import Optional
@@ -135,17 +136,15 @@
 
     @classmethod
     def get_table_index_key(cls):
         """Returns the key in which the primary keys of the given table have been saved"""
         return f"{cls._get_prefix()}{cls._get_tablename()}{cls._get_separator()}__index"
 
     @classmethod
-    async def _ids_to_primary_keys(
-        cls, ids: Optional[Union[Any, List[Any]]] = None
-    ) -> Tuple[List[Optional[str]], str]:
+    async def _ids_to_primary_keys(cls, ids: Optional[Union[Any, List[Any]]] = None) -> Tuple[List[Optional[str]], str]:
         """Turn passed in ids into primary key values"""
         table_index_key = cls.get_table_index_key()
         if ids is None:
             keys_generator = cls._store.redis_store.sscan_iter(name=table_index_key)
             keys = [key async for key in keys_generator]
         else:
             if not isinstance(ids, list):
```

### Comparing `pydantic_aioredis-1.2.3/pydantic_aioredis/store.py` & `pydantic_aioredis-1.3.0/pydantic_aioredis/store.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module containing the store classes"""
+
 from typing import Any
 from typing import Dict
 from typing import Optional
 
 from pydantic_aioredis.abstract import _AbstractStore
 from pydantic_aioredis.config import RedisConfig
 from pydantic_aioredis.model import Model
@@ -36,17 +37,15 @@
             encoding=self.redis_config.encoding,
             decode_responses=True,
         )
 
     def register_model(self, model_class: type(Model)):
         """Registers the model to this store"""
         if not isinstance(model_class.get_primary_key_field(), str):
-            raise NotImplementedError(
-                f"{model_class.__name__} should have a _primary_key_field"
-            )
+            raise NotImplementedError(f"{model_class.__name__} should have a _primary_key_field")
 
         model_class._store = self
         self.models[model_class.__name__.lower()] = model_class
 
     def model(self, name: str) -> Model:
         """Gets a model by name: case insensitive"""
         return self.models[name.lower()]
```

### Comparing `pydantic_aioredis-1.2.3/pydantic_aioredis/types.py` & `pydantic_aioredis-1.3.0/pydantic_aioredis/types.py`

 * *Files identical despite different names*

### Comparing `pydantic_aioredis-1.2.3/pyproject.toml` & `pydantic_aioredis-1.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-aioredis"
-version = "1.2.3"
+version = "1.3.0"
 description = "Use your pydantic models as an ORM, storing data in Redis."
 authors = ["Andrew Herrington <andrew.the.techie@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/andrewthetechie/pydantic-aioredis"
 repository = "https://github.com/andrewthetechie/pydantic-aioredis"
 documentation = "https://pydantic-aioredis.readthedocs.io/en/latest/"
@@ -21,72 +21,73 @@
 	"Framework :: AsyncIO"
 ]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/andrewthetechie/pydantic-aioredis/releases"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 pydantic = "^1.10.2"
 redis = "^4.4.4"
 anyio = "^3.6.2"
 nest-asyncio = "^1.5.6"
-fastapi = {version = ">=0.91,<0.96", optional = true}
+fastapi = {version = ">=0.110", optional = true}
 fastapi-crudrouter = {version = "^0.8.6", optional = true}
 
 [tool.poetry.extras]
 FastAPI= ['fastapi']
 fastapi-crudrouter=['fastapi-crudrouter']
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 coverage = {extras = ["toml"], version = ">=6.5,<8.0"}
 safety = "^2.3.1"
-mypy = ">=0.991,<1.2"
+mypy = ">=0.991,<1.5"
 xdoctest = {extras = ["colors"], version = "^1.1.0"}
 sphinx = ">=4.3.2,<6.0.0"
 sphinx-autobuild = ">=2021.3.14"
 pre-commit = ">=2.12.1"
 pep8-naming = "^0.13.2"
 reorder-python-imports = "^3.9.0"
 pre-commit-hooks = "^4.2.0"
 Pygments = "^2.13.0"
 pyupgrade = "^3.3.1"
 furo = ">=2021.11.12"
 pytest-cov = "^4.0.0"
-types-croniter = "^1.3.2"
+types-croniter = ">=1.3.2,<3.0.0"
 pytest_async = "^0.1.1"
 pytest-asyncio = ">=0.20.1,<0.22.0"
 pytest-mock = "^3.10.0"
 pytest-lazy-fixture = "^0.6.3"
 fastapi = ">=0.6.3"
 fastapi-crudrouter = ">=0.8.4"
-httpx = "^0.23.0"
+httpx = ">=0.23,<0.25"
 pytest-env = "^0.8.1"
-pytest-mockservers = "^0.6.0"
 pytest-xdist = "^3.1.0"
-bandit = "^1.7.4"
-fakeredis = {extras = ["json"], version = "2.2.0"}
+bandit = "^1.7.8"
+fakeredis = {extras = ["json"], version = "2.22.0"}
 hypothesis = "^6.61.0"
-pytest-rerunfailures = "^11.1"
-ruff = ">=0.0.249,<0.0.260"
+pytest-rerunfailures = ">=11.1,<13.0"
+ruff = "^0.4.2"
 
 [tool.mypy]
 strict = true
 warn_unreachable = true
 pretty = true
 show_column_numbers = true
 show_error_codes = true
 show_error_context = true
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
+[tool.bandit]
+exclude_dirs = ["test", "noxfile.py", ".github/scripts", "dist", "examples/*"]
 
 [tool.pytest.ini_options]
 addopts = "-n 4 --ignore examples --cov=pydantic_aioredis --cov-report xml:.coverage.xml --cov-report=term-missing --cov-fail-under 91"
 
 [tool.ruff]
 line-length = 120
 target-version = "py37"
```

### Comparing `pydantic_aioredis-1.2.3/PKG-INFO` & `pydantic_aioredis-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 Metadata-Version: 2.1
 Name: pydantic-aioredis
-Version: 1.2.3
+Version: 1.3.0
 Summary: Use your pydantic models as an ORM, storing data in Redis.
 Home-page: https://github.com/andrewthetechie/pydantic-aioredis
 License: MIT
 Author: Andrew Herrington
 Author-email: andrew.the.techie@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: fastapi
 Provides-Extra: fastapi-crudrouter
 Requires-Dist: anyio (>=3.6.2,<4.0.0)
-Requires-Dist: fastapi (>=0.91,<0.96) ; extra == "fastapi"
+Requires-Dist: fastapi (>=0.110) ; extra == "fastapi"
 Requires-Dist: fastapi-crudrouter (>=0.8.6,<0.9.0) ; extra == "fastapi-crudrouter"
 Requires-Dist: nest-asyncio (>=1.5.6,<2.0.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: redis (>=4.4.4,<5.0.0)
 Project-URL: Changelog, https://github.com/andrewthetechie/pydantic-aioredis/releases
 Project-URL: Documentation, https://pydantic-aioredis.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/andrewthetechie/pydantic-aioredis
@@ -146,15 +142,15 @@
   # oops, there was a typo. Fix it
   # Update is an async context manager and will update redis with all changes in one operations
   async with this_book.update():
     this_book.author = "Herman Melville"
     this_book.published_on=date(year=1851, month=10, day=18)
   this_book_from_redis = await Book.select(ids=["Moby Dick"])
   assert this_book_from_redis[0].author == "Herman Melville"
-  assert this_book_from_redis[0].author == date(year=1851, month=10, day=18)
+  assert this_book_from_redis[0].published_on == date(year=1851, month=10, day=18)
 
   # Delete any number of items
   await Library.delete(ids=["The Grand Library"])
 
 # Now run these updates
 loop = asyncio.get_event_loop()
 loop.run_until_complete(work_with_orm())
@@ -186,20 +182,21 @@
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
   <tbody>
     <tr>
-      <td align="center"><a href="https://github.com/andrewthetechie"><img src="https://avatars.githubusercontent.com/u/1377314?v=4?s=100" width="100px;" alt="Andrew"/><br /><sub><b>Andrew</b></sub></a><br /><a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=andrewthetechie" title="Code">💻</a> <a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=andrewthetechie" title="Documentation">📖</a></td>
-      <td align="center"><a href="https://github.com/Tinitto"><img src="https://avatars.githubusercontent.com/u/21363733??v=4?s=100" width="100px;" alt="Martin Ahindura"/><br /><sub><b>Martin Ahindura</b></sub></a><br /><a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=Tinitto" title="Code">💻</a> <a href="#ideas-Tinitto" title="Ideas, Planning, & Feedback">🤔</a></td>
-      <td align="center"><a href="https://github.com/david-wahlstedt"><img src="https://avatars.githubusercontent.com/u/66391333?v=4?s=100" width="100px;" alt="david-wahlstedt"/><br /><sub><b>david-wahlstedt</b></sub></a><br /><a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=david-wahlstedt" title="Tests">⚠️</a> <a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=david-wahlstedt" title="Documentation">📖</a> <a href="https://github.com/andrewthetechie/pydantic-aioredis/pulls?q=is%3Apr+reviewed-by%3Adavid-wahlstedt" title="Reviewed Pull Requests">👀</a></td>
-      <td align="center"><a href="https://blog.gtmanfred.com"><img src="https://avatars.githubusercontent.com/u/732321?v=4?s=100" width="100px;" alt="Daniel Wallace"/><br /><sub><b>Daniel Wallace</b></sub></a><br /><a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=gtmanfred" title="Tests">⚠️</a></td>
-      <td align="center"><a href="https://derwen.ai/paco"><img src="https://avatars.githubusercontent.com/u/57973?v=4?s=100" width="100px;" alt="Paco Nathan"/><br /><sub><b>Paco Nathan</b></sub></a><br /><a href="#example-ceteri" title="Examples">💡</a></td>
-      <td align="center"><a href="https://www.linkedin.com/in/andreas-brodersen-1b955b100/"><img src="https://avatars.githubusercontent.com/u/43907402?v=4?s=100" width="100px;" alt="Andreas Brodersen"/><br /><sub><b>Andreas Brodersen</b></sub></a><br /><a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=AndreasPB" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/andrewthetechie"><img src="https://avatars.githubusercontent.com/u/1377314?v=4?s=100" width="100px;" alt="Andrew"/><br /><sub><b>Andrew</b></sub></a><br /><a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=andrewthetechie" title="Code">💻</a> <a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=andrewthetechie" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Tinitto"><img src="https://avatars.githubusercontent.com/u/21363733??v=4?s=100" width="100px;" alt="Martin Ahindura"/><br /><sub><b>Martin Ahindura</b></sub></a><br /><a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=Tinitto" title="Code">💻</a> <a href="#ideas-Tinitto" title="Ideas, Planning, & Feedback">🤔</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/david-wahlstedt"><img src="https://avatars.githubusercontent.com/u/66391333?v=4?s=100" width="100px;" alt="david-wahlstedt"/><br /><sub><b>david-wahlstedt</b></sub></a><br /><a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=david-wahlstedt" title="Tests">⚠️</a> <a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=david-wahlstedt" title="Documentation">📖</a> <a href="https://github.com/andrewthetechie/pydantic-aioredis/pulls?q=is%3Apr+reviewed-by%3Adavid-wahlstedt" title="Reviewed Pull Requests">👀</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://blog.gtmanfred.com"><img src="https://avatars.githubusercontent.com/u/732321?v=4?s=100" width="100px;" alt="Daniel Wallace"/><br /><sub><b>Daniel Wallace</b></sub></a><br /><a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=gtmanfred" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://derwen.ai/paco"><img src="https://avatars.githubusercontent.com/u/57973?v=4?s=100" width="100px;" alt="Paco Nathan"/><br /><sub><b>Paco Nathan</b></sub></a><br /><a href="#example-ceteri" title="Examples">💡</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://www.linkedin.com/in/andreas-brodersen-1b955b100/"><img src="https://avatars.githubusercontent.com/u/43907402?v=4?s=100" width="100px;" alt="Andreas Brodersen"/><br /><sub><b>Andreas Brodersen</b></sub></a><br /><a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=AndreasPB" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/kraczak"><img src="https://avatars.githubusercontent.com/u/58468064?v=4?s=100" width="100px;" alt="kraczak"/><br /><sub><b>kraczak</b></sub></a><br /><a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=kraczak" title="Documentation">📖</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

