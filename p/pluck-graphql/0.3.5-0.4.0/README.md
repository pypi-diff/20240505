# Comparing `tmp/pluck_graphql-0.3.5.tar.gz` & `tmp/pluck_graphql-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pluck_graphql-0.3.5.tar", max compression
+gzip compressed data, was "pluck_graphql-0.4.0.tar", max compression
```

## Comparing `pluck_graphql-0.3.5.tar` & `pluck_graphql-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-09-30 07:52:47.581188 pluck_graphql-0.3.5/LICENSE
--rw-r--r--   0        0        0    12685 2023-10-14 19:05:52.528538 pluck_graphql-0.3.5/README.md
--rw-r--r--   0        0        0     1123 2024-03-03 08:21:36.573480 pluck_graphql-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      633 2023-10-14 13:58:54.472399 pluck_graphql-0.3.5/src/pluck/__init__.py
--rw-r--r--   0        0        0      454 2023-09-30 07:52:47.582075 pluck_graphql-0.3.5/src/pluck/_decorators.py
--rw-r--r--   0        0        0     6494 2024-03-03 08:21:36.573701 pluck_graphql-0.3.5/src/pluck/_execution.py
--rw-r--r--   0        0        0     3727 2024-03-03 08:12:08.887570 pluck_graphql-0.3.5/src/pluck/_json.py
--rw-r--r--   0        0        0      745 2023-10-14 13:58:54.472584 pluck_graphql-0.3.5/src/pluck/_libraries.py
--rw-r--r--   0        0        0     2746 2024-03-03 08:12:08.888002 pluck_graphql-0.3.5/src/pluck/_normalization.py
--rw-r--r--   0        0        0     2426 2023-09-30 07:52:47.582635 pluck_graphql-0.3.5/src/pluck/_parser.py
--rw-r--r--   0        0        0     3918 2023-10-21 09:46:05.599650 pluck_graphql-0.3.5/src/pluck/_pluck.py
--rw-r--r--   0        0        0     2986 2023-10-14 14:35:15.040960 pluck_graphql-0.3.5/src/pluck/client.py
--rw-r--r--   0        0        0    13599 1970-01-01 00:00:00.000000 pluck_graphql-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-09-30 07:52:47.581188 pluck_graphql-0.4.0/LICENSE
+-rw-r--r--   0        0        0    12685 2023-10-14 19:05:52.528538 pluck_graphql-0.4.0/README.md
+-rw-r--r--   0        0        0     1161 2024-05-05 19:38:52.841908 pluck_graphql-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      633 2024-05-05 19:39:25.498320 pluck_graphql-0.4.0/src/pluck/__init__.py
+-rw-r--r--   0        0        0      454 2023-09-30 07:52:47.582075 pluck_graphql-0.4.0/src/pluck/_decorators.py
+-rw-r--r--   0        0        0     6960 2024-05-05 19:39:25.498588 pluck_graphql-0.4.0/src/pluck/_execution.py
+-rw-r--r--   0        0        0     4043 2024-05-05 19:39:34.001331 pluck_graphql-0.4.0/src/pluck/_json.py
+-rw-r--r--   0        0        0      745 2023-10-14 13:58:54.472584 pluck_graphql-0.4.0/src/pluck/_libraries.py
+-rw-r--r--   0        0        0     3670 2024-05-05 19:39:25.499019 pluck_graphql-0.4.0/src/pluck/_normalization.py
+-rw-r--r--   0        0        0     4012 2024-05-05 19:39:34.001401 pluck_graphql-0.4.0/src/pluck/_parser.py
+-rw-r--r--   0        0        0     3918 2024-05-05 19:39:25.499416 pluck_graphql-0.4.0/src/pluck/_pluck.py
+-rw-r--r--   0        0        0     2948 2024-05-05 19:29:32.359405 pluck_graphql-0.4.0/src/pluck/client.py
+-rw-r--r--   0        0        0    13599 1970-01-01 00:00:00.000000 pluck_graphql-0.4.0/PKG-INFO
```

### Comparing `pluck_graphql-0.3.5/LICENSE` & `pluck_graphql-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pluck_graphql-0.3.5/README.md` & `pluck_graphql-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pluck_graphql-0.3.5/pyproject.toml` & `pluck_graphql-0.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pluck-graphql"
-version = "0.3.5"
+version = "0.4.0"
 description = "Transform GraphQL queries into Pandas data-frames."
 readme = "README.md"
 authors = ["Martin Galpin <galpin@gmail.com>"]
 license = "MIT License"
 repository = "https://github.com/galpin/pluck"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -26,18 +26,21 @@
 pandas = ">=1.4"
 graphql-core = "^3.2.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 httpretty = "^1.1.4"
 isort = "^5.10.1"
-black = "^22.6.0"
 twine = "^4.0.1"
 
 [tool.poetry.group.dev.dependencies]
 jupyter = "^1.0.0"
 nbconvert = "^7.9.2"
 tabulate = "^0.9.0"
+ruff = "^0.4.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.ruff.lint]
+extend-select = ["I"]
```

### Comparing `pluck_graphql-0.3.5/src/pluck/__init__.py` & `pluck_graphql-0.4.0/src/pluck/__init__.py`

 * *Files identical despite different names*

### Comparing `pluck_graphql-0.3.5/src/pluck/_execution.py` & `pluck_graphql-0.4.0/src/pluck/_execution.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 )
 from ._normalization import normalize
 from ._parser import ParsedQuery, QueryParser
 from ._decorators import timeit
 from .client import GraphQLClient, GraphQLRequest, GraphQLResponse, UrllibGraphQLClient
 from ._libraries import DataFrame, DataFrameLibrary, PandasDataFrameLibrary
 
-ExecutorResult = Tuple[Dict, List, Dict[str, DataFrame]]
+ExecutorResult = Tuple[Optional[Dict], Optional[List], Dict[str, DataFrame]]
 EMPTY = tuple()
 
 
 @dataclass
 class ExecutorOptions:
     separator: str
     client: Optional[GraphQLClient]
@@ -46,15 +46,15 @@
 
     @timeit
     def execute(self, request: GraphQLRequest) -> ExecutorResult:
         parsed_query = QueryParser(request.query).parse()
         new_request = request.replace(query=parsed_query.query)
         response = self._execute(new_request)
         extracted = self._extract(parsed_query, response)
-        frames = self._normalize(extracted)
+        frames = self._normalize(extracted, parsed_query)
         frames = self._rename_columns(frames)
         return response.data, response.errors, frames
 
     @timeit
     def _execute(self, new_request):
         return self._options.client.execute(new_request)
 
@@ -65,20 +65,37 @@
             return {"default": [response.data]}
         context = FrameExtractorContext(query)
         visit(response.data, FrameExtractor(context))
         found = context.frame_data
         return {f.name: found.get(f.name, EMPTY) for f in query.frames}
 
     @timeit
-    def _normalize(self, frame_data: Dict[str, JsonValue]) -> Dict[str, Any]:
+    def _normalize(
+        self,
+        frame_data: Dict[str, JsonValue],
+        query: ParsedQuery,
+    ) -> Dict[str, Any]:
         separator = self._options.separator
         frames = {}
         for name, data in frame_data.items():
+            selection_set = (
+                query.selection_set
+                if query.is_implicit_mode
+                else query.frame(name).selection_set
+            )
             data = itertools.chain(
-                *[normalize(x, separator, fallback=name) for x in data]
+                *[
+                    normalize(
+                        x,
+                        separator,
+                        fallback=name,
+                        selection_set=selection_set,
+                    )
+                    for x in data
+                ]
             )
             frames[name] = self._create_data_frame(data)
         return frames
 
     @timeit
     def _create_data_frame(self, data) -> DataFrame:
         return self._options.library.create(data)
```

### Comparing `pluck_graphql-0.3.5/src/pluck/_json.py` & `pluck_graphql-0.4.0/src/pluck/_json.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,16 +8,28 @@
 JsonObject = Dict[str, Any]
 JsonArray = List[Any]
 JsonScalar = Union[str, float, int, bool]
 JsonValue = Union[JsonObject, JsonArray, JsonScalar, None]
 
 
 class JsonPath(tuple):
-    def add(self, value: str):
-        return JsonPath(self + (value,))
+    def __new__(cls, *values: str):
+        return super(JsonPath, cls).__new__(cls, tuple(values))
+
+    def add(self, *values: str) -> JsonPath:
+        return JsonPath(*self, *values)
+
+    def pop_right(self):
+        return JsonPath(*self[:-1])
+
+    def join(self, separator: str) -> str:
+        return separator.join(self)
+
+    def __str__(self):
+        return self.join(".")
 
 
 class JsonVisitorAction(enum.Enum):
     STOP = 1
 
 
 STOP = JsonVisitorAction.STOP
@@ -105,39 +117,45 @@
 
 
 class JsonSerializer(ABC):
     @staticmethod
     def create_fastest() -> JsonSerializer:
         try:
             import orjson
+
             return OrJsonSerializer()
         except ImportError:
             import json
+
             return BuiltinJsonSerializer()
 
     @abstractmethod
     def serialize(self, obj: JsonValue, encoding: str) -> bytes:
         raise NotImplementedError()
 
     @abstractmethod
     def deserialize(self, fp: TextIO) -> JsonValue:
         raise NotImplementedError()
 
 
 class BuiltinJsonSerializer(JsonSerializer):
     def serialize(self, obj: JsonValue, encoding: str) -> bytes:
         import json
+
         return json.dumps(obj).encode(encoding)
 
     def deserialize(self, fp: TextIO) -> JsonValue:
         import json
+
         return json.load(fp)
 
 
 class OrJsonSerializer(JsonSerializer):
     def serialize(self, obj: JsonValue, encoding: str) -> bytes:
         import orjson
+
         return orjson.dumps(obj)
 
     def deserialize(self, fp: TextIO) -> JsonValue:
         import orjson
+
         return orjson.loads(fp.read())
```

### Comparing `pluck_graphql-0.3.5/src/pluck/_libraries.py` & `pluck_graphql-0.4.0/src/pluck/_libraries.py`

 * *Files identical despite different names*

### Comparing `pluck_graphql-0.3.5/src/pluck/_normalization.py` & `pluck_graphql-0.4.0/src/pluck/_normalization.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,93 @@
+from __future__ import annotations
+
 import itertools
-from dataclasses import dataclass
-from typing import Dict, Generator, Iterable, List, Optional
+from dataclasses import dataclass, replace
+from typing import Dict, Generator, Iterable, List, Optional, Set, Tuple
 
 from ._json import STOP, JsonArray, JsonPath, JsonScalar, JsonValue, JsonVisitor, visit
 
 NormalizeResult = List[Dict[str, JsonValue]]
 
 
 def normalize(
     obj: JsonValue,
     separator: str = ".",
     fallback: Optional[str] = "?",
+    selection_set: Optional[Set[JsonPath]] = None,
 ) -> NormalizeResult:
     assert separator
-    options = JsonNormalizerOptions(separator, fallback)
-    return JsonNormalizer(options).normalize(obj)
+    options = JsonNormalizerOptions(separator, fallback, selection_set=selection_set)
+    result = JsonNormalizer(options).normalize(obj)
+    return result.rows
 
 
-@dataclass
+@dataclass(frozen=True)
 class JsonNormalizerOptions:
     separator: str
     fallback: str
+    initial_path: Optional[JsonPath] = None
+    selection_set: Optional[Set[JsonPath]] = None
+
+    def replace(self, **kwargs) -> JsonNormalizerOptions:
+        return replace(self, **kwargs)
+
+
+@dataclass(frozen=True)
+class JsonNormalizerResult:
+    rows: List[Dict[str, JsonValue]]
+    paths: Set[JsonPath]
 
 
 class JsonNormalizer:
-    def __init__(
-        self,
-        options: JsonNormalizerOptions,
-        initial_path: Optional[JsonPath] = None,
-    ):
+    def __init__(self, options: JsonNormalizerOptions):
         self._options = options
-        self._initial_path = initial_path
 
-    def normalize(self, obj: JsonValue) -> NormalizeResult:
+    def normalize(self, obj: JsonValue) -> JsonNormalizerResult:
         ctx = JsonNormalizerContext(self._options)
         visitor = JsonNormalizerVisitor(ctx)
-        visit(obj, visitor, self._initial_path)
-        return ctx.rows
+        visit(obj, visitor, self._options.initial_path)
+        return JsonNormalizerResult(ctx.rows, ctx.paths)
 
 
 class JsonNormalizerContext:
     def __init__(self, options: JsonNormalizerOptions):
         self._options = options
-        self._rows = [{}]
+        self._rows: List[JsonValue] = [{}]
+        self._paths: Set[JsonPath] = set()
 
     @property
-    def rows(self):
+    def options(self) -> JsonNormalizerOptions:
+        return self._options
+
+    @property
+    def rows(self) -> List[JsonValue]:
         return self._rows
 
+    @property
+    def paths(self) -> Set[JsonPath]:
+        return self._paths
+
     def set(self, path: JsonPath, value: JsonValue):
         for row in reversed(self._rows):
             name = self._generate_name(path)
             row[name] = value
+        self._paths.add(path)
 
     def _generate_name(self, path: JsonPath) -> str:
         separator = self._options.separator
         fallback = self._options.fallback
         name = separator.join(path)
         return fallback if not name and fallback else name
 
     def normalize(self, path: JsonPath, other: JsonValue):
-        normalizer = JsonNormalizer(self._options, path)
-        return normalizer.normalize(other)
+        normalizer = JsonNormalizer(self._options.replace(initial_path=path))
+        result = normalizer.normalize(other)
+        self._paths.update(result.paths)
+        return result
 
     def cross_join(self, other: Generator):
         if other := _spy(other):
             self._rows = [x | y for x, y in itertools.product(self._rows, other)]
 
 
 class JsonNormalizerVisitor(JsonVisitor):
@@ -75,18 +97,22 @@
     def on_scalar(self, path: JsonPath, value: JsonScalar):
         self._set(path, value)
 
     def on_null(self, path: JsonPath):
         self._set(path, None)
 
     def _set(self, path: JsonPath, value: JsonValue):
-        self._ctx.set(path, value)
+        selection_set = self._ctx.options.selection_set
+        if not selection_set or path in selection_set:
+            self._ctx.set(path, value)
 
     def enter_array(self, path: JsonPath, value: JsonArray):
-        rows = (self._ctx.normalize(path, item) for item in value if item is not None)
+        rows = (
+            self._ctx.normalize(path, item).rows for item in value if item is not None
+        )
         other = itertools.chain(*rows)
         self._ctx.cross_join(other)
         return STOP
 
 
 def _spy(generator: Generator) -> Optional[Iterable]:
     try:
```

### Comparing `pluck_graphql-0.3.5/src/pluck/_pluck.py` & `pluck_graphql-0.4.0/src/pluck/_pluck.py`

 * *Files identical despite different names*

### Comparing `pluck_graphql-0.3.5/src/pluck/client.py` & `pluck_graphql-0.4.0/src/pluck/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import dataclasses
 import urllib.request
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, Optional
 
 from ._json import JsonSerializer
 
 __all__ = ("GraphQLRequest", "GraphQLResponse", "GraphQLClient", "UrllibGraphQLClient")
 
 
 @dataclass(frozen=True)
@@ -43,15 +43,15 @@
     A GraphQL response.
 
     Args:
         data: The data returned by the query.
         errors: The errors returned by the query.
     """
 
-    data: Union[Dict, List, int, str, bool, None]
+    data: Optional[Dict]
     errors: Optional[Dict]
 
     @classmethod
     def from_dict(cls, response: Dict) -> "GraphQLResponse":
         return cls(response.get("data"), response.get("errors"))
```

### Comparing `pluck_graphql-0.3.5/PKG-INFO` & `pluck_graphql-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluck-graphql
-Version: 0.3.5
+Version: 0.4.0
 Summary: Transform GraphQL queries into Pandas data-frames.
 Home-page: https://github.com/galpin/pluck
 License: MIT
 Author: Martin Galpin
 Author-email: galpin@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

