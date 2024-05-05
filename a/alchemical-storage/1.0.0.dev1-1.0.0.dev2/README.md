# Comparing `tmp/alchemical_storage-1.0.0.dev1.tar.gz` & `tmp/alchemical_storage-1.0.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alchemical_storage-1.0.0.dev1.tar", max compression
+gzip compressed data, was "alchemical_storage-1.0.0.dev2.tar", max compression
```

## Comparing `alchemical_storage-1.0.0.dev1.tar` & `alchemical_storage-1.0.0.dev2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0     1095 2023-08-14 21:02:31.726524 alchemical_storage-1.0.0.dev1/LICENSE
--rw-r--r--   0        0        0     2073 2023-08-25 04:54:31.634064 alchemical_storage-1.0.0.dev1/README.md
--rw-r--r--   0        0        0       69 2023-09-15 19:54:45.612620 alchemical_storage-1.0.0.dev1/alchemical_storage/__init__.py
--rw-r--r--   0        0        0      166 2023-09-02 19:40:22.868508 alchemical_storage-1.0.0.dev1/alchemical_storage/filter/__init__.py
--rw-r--r--   0        0        0      144 2023-08-14 19:23:37.214316 alchemical_storage-1.0.0.dev1/alchemical_storage/filter/exc.py
--rw-r--r--   0        0        0     5137 2023-09-02 19:40:22.968507 alchemical_storage-1.0.0.dev1/alchemical_storage/filter/filter.py
--rw-r--r--   0        0        0     2386 2023-09-02 19:40:22.932507 alchemical_storage-1.0.0.dev1/alchemical_storage/join.py
--rw-r--r--   0        0        0        0 2023-09-15 19:53:36.041459 alchemical_storage-1.0.0.dev1/alchemical_storage/py.typed
--rw-r--r--   0        0        0      128 2023-09-02 19:40:22.868508 alchemical_storage-1.0.0.dev1/alchemical_storage/storage/__init__.py
--rw-r--r--   0        0        0      159 2023-08-13 07:12:39.101699 alchemical_storage-1.0.0.dev1/alchemical_storage/storage/exc.py
--rw-r--r--   0        0        0     7295 2023-09-02 19:40:23.036506 alchemical_storage-1.0.0.dev1/alchemical_storage/storage/storage.py
--rw-r--r--   0        0        0      939 2023-09-02 19:40:22.892508 alchemical_storage-1.0.0.dev1/alchemical_storage/visitor.py
--rw-r--r--   0        0        0      948 2023-09-15 20:10:12.153755 alchemical_storage-1.0.0.dev1/pyproject.toml
--rw-r--r--   0        0        0     2642 1970-01-01 00:00:00.000000 alchemical_storage-1.0.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-01-13 18:42:53.116289 alchemical_storage-1.0.0.dev2/LICENSE
+-rw-r--r--   0        0        0     2073 2024-01-13 18:42:53.116289 alchemical_storage-1.0.0.dev2/README.md
+-rw-r--r--   0        0        0       69 2024-01-13 18:42:53.116289 alchemical_storage-1.0.0.dev2/alchemical_storage/__init__.py
+-rw-r--r--   0        0        0      166 2024-01-13 18:42:53.116289 alchemical_storage-1.0.0.dev2/alchemical_storage/filter/__init__.py
+-rw-r--r--   0        0        0      144 2024-01-13 18:42:53.116289 alchemical_storage-1.0.0.dev2/alchemical_storage/filter/exc.py
+-rw-r--r--   0        0        0     5129 2024-01-13 18:42:53.116289 alchemical_storage-1.0.0.dev2/alchemical_storage/filter/filter.py
+-rw-r--r--   0        0        0       13 2024-01-13 18:42:53.116289 alchemical_storage-1.0.0.dev2/alchemical_storage/index/__init__.py
+-rw-r--r--   0        0        0     1720 2024-01-13 18:42:53.116289 alchemical_storage-1.0.0.dev2/alchemical_storage/index/index.py
+-rw-r--r--   0        0        0     2380 2024-01-13 18:42:53.116289 alchemical_storage-1.0.0.dev2/alchemical_storage/join.py
+-rw-r--r--   0        0        0        0 2024-01-13 18:42:53.116289 alchemical_storage-1.0.0.dev2/alchemical_storage/py.typed
+-rw-r--r--   0        0        0      128 2024-01-13 18:42:53.116289 alchemical_storage-1.0.0.dev2/alchemical_storage/storage/__init__.py
+-rw-r--r--   0        0        0      162 2024-01-13 18:42:53.116289 alchemical_storage-1.0.0.dev2/alchemical_storage/storage/exc.py
+-rw-r--r--   0        0        0     7220 2024-01-13 18:42:53.116289 alchemical_storage-1.0.0.dev2/alchemical_storage/storage/storage.py
+-rw-r--r--   0        0        0      931 2024-01-13 18:42:53.116289 alchemical_storage-1.0.0.dev2/alchemical_storage/visitor.py
+-rw-r--r--   0        0        0     1106 2024-01-13 18:42:53.116289 alchemical_storage-1.0.0.dev2/pyproject.toml
+-rw-r--r--   0        0        0     2694 1970-01-01 00:00:00.000000 alchemical_storage-1.0.0.dev2/PKG-INFO
```

### Comparing `alchemical_storage-1.0.0.dev1/LICENSE` & `alchemical_storage-1.0.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `alchemical_storage-1.0.0.dev1/README.md` & `alchemical_storage-1.0.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `alchemical_storage-1.0.0.dev1/alchemical_storage/filter/filter.py` & `alchemical_storage-1.0.0.dev2/alchemical_storage/filter/filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-"""
-Build upon the ``alchemical_storage.visitor`` module to create a classes that can be used to map
-filters and order_by attributes to sqlalchemy statements.
-"""
+"""Build upon the ``alchemical_storage.visitor`` module to create a classes
+that can be used to map filters and order_by attributes to sqlalchemy
+statements."""
 
 import functools
 import importlib
 import operator
 from typing import Any, Callable, Generator
 
 from sqlalchemy.sql.expression import desc
@@ -13,16 +12,15 @@
 from alchemical_storage.filter.exc import OrderByException
 from alchemical_storage.visitor import StatementVisitor, T
 
 # pylint: disable=too-few-public-methods
 
 
 class FilterMap(StatementVisitor):
-    """
-    Initialize the filter mapper
+    """Initialize the filter mapper.
 
     Args:
         filters (dict[str, Any]): A dictionary of filters
         import_from (str): The module to import Model classes from
 
     Example:
         ::
@@ -55,17 +53,17 @@
                 if not get_by:
                     get_by = getattr(self.__module, child)
                 else:
                     get_by = getattr(get_by, child)
             self.filters[filter_] = functools.partial(op_, get_by)
 
     def visit_statement(self, statement: T, params: dict[str, Any]):
-        """
-        Apply filters to an sqlalchemy query. Each key in ``params`` corresponds to a filter
-        in ``self.filters``. If the key is not in ``self.filters``, it is ignored.
+        """Apply filters to an sqlalchemy query. Each key in ``params``
+        corresponds to a filter in ``self.filters``. If the key is not in
+        ``self.filters``, it is ignored.
 
         Args:
             statement (T): The sqlalchemy statement to apply filters to
             params (dict[str, Any]): The filters to apply
 
         Returns:
             T: The filtered sqlalchemy statement
@@ -82,16 +80,16 @@
     ) -> Generator[Any, None, None]:
         for attr, filtered_by in given_filters.items():
             if attr in self.filters:
                 yield self.filters[attr](filtered_by)
 
 
 class OrderByMap(StatementVisitor):
-    """
-    A mapper to convert order_by attributes to sqlalchemy order_by expressions
+    """A mapper to convert order_by attributes to sqlalchemy order_by
+    expressions.
 
     Args:
         order_by_attributes (dict[str, Any]): A dictionary of order_by attributes, where
             the key is the attribute name and the value is the column or label to order by.
         import_from (str): The module to import Model classes from
 
     Example:
@@ -114,16 +112,16 @@
                 order_by = getattr(getattr(module, model), model_attr)
             else:
                 order_by = column
 
             self.order_by_attributes[attr] = order_by
 
     def visit_statement(self, statement, params: dict[str, Any]):
-        """
-        Apply order_by to an sqlalchemy query. Ignores order_by if not given in params.
+        """Apply order_by to an sqlalchemy query. Ignores order_by if not given
+        in params.
 
         Args:
             statement (T): The sqlalchemy statement to apply order_by to
             params (dict[str, Any]): The filters to apply
 
         Returns:
             (T): The order_by sqlalchemy statement
```

### Comparing `alchemical_storage-1.0.0.dev1/alchemical_storage/join.py` & `alchemical_storage-1.0.0.dev2/alchemical_storage/join.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 
 from alchemical_storage.visitor import StatementVisitor, T
 
 JoinExpression = str | tuple[Any, ...]
 
 
 class JoinMap(StatementVisitor):
-    """
-    Class for adding joins to sqlalchemy queries.
+    """Class for adding joins to sqlalchemy queries.
 
     Args:
         import_from (str): The module to import the models/entities from.
         param_names (tuple[str, ...]): The names of the parameters that will trigger the join.
             Any of these parameters being in the ``params`` dict passed to ``visit_statement``
             will trigger the join.
         *joins (str | tuple[Any, ...]): The joins to add to the query.
@@ -24,15 +23,14 @@
 
             from alchemical_storage.join import JoinMap
             from tests.models import Model, RelatedToModel
 
             join_map = JoinMap(
                 'tests.models', ('join_param', ), ('RelatedToModel', )
             )
-
     """
 
     joins: tuple[tuple[Any, ...], ...]
 
     def __init__(
         self,
         import_from: str,
```

### Comparing `alchemical_storage-1.0.0.dev1/alchemical_storage/storage/storage.py` & `alchemical_storage-1.0.0.dev2/alchemical_storage/storage/storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Module defining storage services"""
+"""Module defining storage services."""
 
 import abc
 import functools
 from typing import Any, Generic, Iterable, Optional, Sequence, Type, TypeVar
 
 import sqlalchemy as sql
 from marshmallow_sqlalchemy import SQLAlchemySchema
@@ -12,100 +12,92 @@
 
 from .exc import ConflictError, NotFoundError
 
 AlchemyModel = TypeVar("AlchemyModel", bound=DeclarativeBase)
 
 
 class StorageABC(abc.ABC, Generic[AlchemyModel]):
-    """Resource storage protocol"""
+    """Resource storage protocol."""
 
     @abc.abstractmethod
     def get(self, identity: Any) -> AlchemyModel:
-        """
-        Get a resource from storage
+        """Get a resource from storage.
 
         Args:
             identity (Any): The description
 
         Returns:
             AlchemyModel: Object that can be serialized to output for api
         """
 
     @abc.abstractmethod
     def index(self, **kwargs) -> list[AlchemyModel]:
-        """
-        Get a list resources from storage
+        """Get a list resources from storage.
 
         Returns:
             list[AlchemyModel]: List of objects that can be serialized to output for api
         """
 
     @abc.abstractmethod
     def count_index(self, **kwargs) -> int:
-        """
-        Get a list resources from storage
+        """Get a list resources from storage.
 
         Returns:
             int: Count of objects in given set
         """
 
     @abc.abstractmethod
     def put(self, identity: Any, data: dict[str, Any]) -> AlchemyModel:
-        """
-        Put a new resource to storage
+        """Put a new resource to storage.
 
         Args:
             identity (Any): The resource identifier
             data (dict[str, Any]): Data that can be deserialized to Any for create
 
         Returns:
             AlchemyModel: Object that can be serialized to output for api
         """
 
     @abc.abstractmethod
     def patch(self, identity: Any, data: dict[str, Any]) -> AlchemyModel:
-        """
-        Update a resource in storage
+        """Update a resource in storage.
 
         Args:
             identity (Any): The resource identifier
             data (dict[str, Any]): Data that can be deserialized to Any for update
 
         Returns:
             AlchemyModel: Object that can be serialized to output for api
         """
 
     @abc.abstractmethod
     def delete(self, identity: Any) -> AlchemyModel:
-        """
-        Delete a resource from storage
+        """Delete a resource from storage.
 
         Args:
             identity (Any): The resource identifier
 
         Returns:
             AlchemyModel: Object that can be serialized to output for api
         """
 
     @abc.abstractmethod
     def __contains__(self, identity: Any) -> bool:
-        """
-        Checks if resource identified by identity eAny
+        """Checks if resource identified by identity eAny.
 
         Args:
             identity (Any): The resource identifier
 
         Returns:
             bool: Whether the resource exists
         """
 
 
 class DatabaseStorage(StorageABC, Generic[AlchemyModel]):
-    """
-    SQLAlchemy model storage in sql database
+    """SQLAlchemy model storage in sql database.
 
     Args:
         session (Session): The SQLAlchemy session to use for database operations
         entity (Type[AlchemyModel]): The SQLAlchemy model to use for database operations
         storage_schema (SQLAlchemySchema): The marshmallow schema to use for serialization
         primary_key (str|Sequence[str]): The primary key of the entity (Optional, defaults to
             "slug")
@@ -132,18 +124,16 @@
         if isinstance(primary_key, str):
             self._attr = [primary_key]
         else:
             self._attr = list(primary_key)
 
     @staticmethod
     def _convert_identity(func):
-        """
-        Ensures that the identity of the resource is passed to
-        the decorated function as a tuple
-        """
+        """Ensures that the identity of the resource is passed to the decorated
+        function as a tuple."""
 
         @functools.wraps(func)
         def decorator(*args, **kwargs):
             argslist = list(args)
             identity_index = int(isinstance(args[0], StorageABC))
             identity = args[identity_index]
             if not isinstance(identity, Iterable) or isinstance(identity, (str, bytes)):
```

### Comparing `alchemical_storage-1.0.0.dev1/alchemical_storage/visitor.py` & `alchemical_storage-1.0.0.dev2/alchemical_storage/visitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,23 @@
-"""
-Contains the visitor interface for sqlalchemy statements
-"""
+"""Contains the visitor interface for sqlalchemy statements."""
 
 import abc
 from typing import Any, TypeVar
 
 import sqlalchemy as sql
 
 T = TypeVar("T", sql.Select, sql.ColumnElement)
 
 
 class StatementVisitor(abc.ABC):
-    """Visitor class for sqlalchemy statements"""
+    """Visitor class for sqlalchemy statements."""
 
     @abc.abstractmethod
     def visit_statement(self, statement: T, params: dict[str, Any]) -> T:
-        """
-        Visit a statement
+        """Visit a statement.
 
         Args:
             statement (T): The statement to visit
             params (dict[str, Any]): The parameters passed by the
                 alchemical_storage.storage.DatabaseStorage when this method is called
 
         Returns:
```

### Comparing `alchemical_storage-1.0.0.dev1/pyproject.toml` & `alchemical_storage-1.0.0.dev2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 [tool.poetry]
 name = "alchemical-storage"
-version = "1.0.0-dev1"
+version = "1.0.0-dev2"
 description = "Storage based off of sqlalchemy_marshmallow"
 authors = ["Cory Laughlin <corylcomposinger@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "alchemical_storage"}]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = ">=3.10,<3.13"
 sqlalchemy = "^2.0.19"
 marshmallow-sqlalchemy = "^0.29.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 mypy = "^1.5.0"
 pytest-cov = "^4.1.0"
 pytest-mock = "^3.11.1"
 pylint = "^2.17.5"
 esbonio = "^0.16.1"
 black = "^23.7.0"
 isort = "^5.12.0"
 autoflake = "^2.2.1"
+docformatter = "^1.7.5"
+pre-commit = "^3.6.0"
 
 
 [tool.poetry.group.doc.dependencies]
 sphinx = "^7.2.3"
 m2r2 = "^0.3.3.post2"
 
 [build-system]
@@ -35,11 +37,17 @@
 
 [tool.pytest.ini_options]
 addopts = "--cov=alchemical_storage --cov-branch --cov-report xml --cov-report html -vvv"
 
 [tool.autoflake]
 recursive = true
 in_place = true
+remove_all_unused_imports = true
 
 
 [tool.isort]
 profile = "black"
+
+[tool.coverage.report]
+exclude_also = [
+    "if TYPE_CHECKING:",
+    ]
```

### Comparing `alchemical_storage-1.0.0.dev1/PKG-INFO` & `alchemical_storage-1.0.0.dev2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: alchemical-storage
-Version: 1.0.0.dev1
+Version: 1.0.0.dev2
 Summary: Storage based off of sqlalchemy_marshmallow
 License: MIT
 Author: Cory Laughlin
 Author-email: corylcomposinger@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: marshmallow-sqlalchemy (>=0.29.0,<0.30.0)
 Requires-Dist: sqlalchemy (>=2.0.19,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Quickstart
```

