# Comparing `tmp/python_immutable-1.0.5.tar.gz` & `tmp/python_immutable-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_immutable-1.0.5.tar", max compression
+gzip compressed data, was "python_immutable-1.0.6.tar", max compression
```

## Comparing `python_immutable-1.0.5.tar` & `python_immutable-1.0.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2024-03-15 21:36:46.162793 python_immutable-1.0.5/LICENSE
--rw-r--r--   0        0        0     1215 2024-03-15 21:36:46.162793 python_immutable-1.0.5/README.md
--rw-r--r--   0        0        0      152 2024-03-15 21:36:46.166793 python_immutable-1.0.5/immutable/__init__.py
--rw-r--r--   0        0        0     1025 2024-03-15 21:36:46.166793 python_immutable-1.0.5/immutable/main.py
--rw-r--r--   0        0        0     1085 2024-03-15 21:36:46.166793 python_immutable-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     1848 1970-01-01 00:00:00.000000 python_immutable-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-05 11:57:11.816613 python_immutable-1.0.6/LICENSE
+-rw-r--r--   0        0        0     1215 2024-05-05 11:57:11.816613 python_immutable-1.0.6/README.md
+-rw-r--r--   0        0        0      186 2024-05-05 11:57:11.816613 python_immutable-1.0.6/immutable/__init__.py
+-rw-r--r--   0        0        0     1306 2024-05-05 11:57:11.816613 python_immutable-1.0.6/immutable/main.py
+-rw-r--r--   0        0        0     1085 2024-05-05 11:57:11.820613 python_immutable-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1848 1970-01-01 00:00:00.000000 python_immutable-1.0.6/PKG-INFO
```

### Comparing `python_immutable-1.0.5/LICENSE` & `python_immutable-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `python_immutable-1.0.5/README.md` & `python_immutable-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `python_immutable-1.0.5/immutable/main.py` & `python_immutable-1.0.6/immutable/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # ruff: noqa: A003, D100, D101, D102, D103, D104, D105, D107
 from __future__ import annotations
 
 import sys
-from dataclasses import dataclass
-from typing import Any, Mapping, TypeGuard, TypeVar
+from dataclasses import dataclass, make_dataclass
+from typing import Any, Iterable, Mapping, TypeGuard, TypeVar
 
 from typing_extensions import dataclass_transform
 
 _T = TypeVar('_T')
 
 
 @dataclass_transform(kw_only_default=True, frozen_default=True)
@@ -30,7 +30,15 @@
 
 def is_immutable(obj: object) -> TypeGuard[Immutable]:
     return (
         hasattr(obj, '__dataclass_fields__')
         and hasattr(obj, '__dataclass_params__')
         and getattr(getattr(obj, '__dataclass_params__', None), 'frozen', False)
     )
+
+
+@dataclass_transform(kw_only_default=True, frozen_default=True)
+def make_immutable(
+    cls_name: str,
+    fields: Iterable[str | tuple[str, Any] | tuple[str, Any, Any]],
+) -> type:
+    return make_dataclass(cls_name, fields, frozen=True, kw_only=True)
```

### Comparing `python_immutable-1.0.5/pyproject.toml` & `python_immutable-1.0.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-immutable"
-version = "1.0.5"
+version = "1.0.6"
 description = "Immutable implementation for Python using dataclasses"
 authors = ["Sassan Haradji <sassanh@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "immutable" }]
 
 [tool.poetry.dependencies]
@@ -13,16 +13,16 @@
 
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 poethepoet = "^0.24.3"
-pyright = "^1.1.352"
-ruff = "^0.3.0"
+pyright = "^1.1.361"
+ruff = "^0.4.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 demo = "demo:main"
```

### Comparing `python_immutable-1.0.5/PKG-INFO` & `python_immutable-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-immutable
-Version: 1.0.5
+Version: 1.0.6
 Summary: Immutable implementation for Python using dataclasses
 License: Apache-2.0
 Author: Sassan Haradji
 Author-email: sassanh@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

