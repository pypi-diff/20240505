# Comparing `tmp/kaiju_jsonrpc-0.1.0-py3-none-any.whl.zip` & `tmp/kaiju_jsonrpc-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 5544 bytes, number of entries: 7
--rw-r--r--  2.0 unx      243 b- defN 24-May-01 13:47 kaiju_jsonrpc/__init__.py
--rw-r--r--  2.0 unx     5349 b- defN 24-May-01 13:47 kaiju_jsonrpc/parser.py
--rw-r--r--  2.0 unx     5214 b- defN 24-May-02 14:01 kaiju_jsonrpc/router.py
--rw-r--r--  2.0 unx     2589 b- defN 24-May-02 15:15 kaiju_jsonrpc-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-02 15:15 kaiju_jsonrpc-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 24-May-02 15:15 kaiju_jsonrpc-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      563 b- defN 24-May-02 15:15 kaiju_jsonrpc-0.1.0.dist-info/RECORD
-7 files, 14064 bytes uncompressed, 4544 bytes compressed:  67.7%
+Zip file size: 5977 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      244 b- defN 24-May-05 17:33 kaiju_jsonrpc/__init__.py
+-rw-r--r--  2.0 unx     6143 b- defN 24-May-05 17:31 kaiju_jsonrpc/parser.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-02 20:45 kaiju_jsonrpc/py.typed
+-rw-r--r--  2.0 unx     5464 b- defN 24-May-05 17:32 kaiju_jsonrpc/router.py
+-rw-r--r--  2.0 unx     2640 b- defN 24-May-05 17:35 kaiju_jsonrpc-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-05 17:35 kaiju_jsonrpc-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 24-May-05 17:35 kaiju_jsonrpc-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      639 b- defN 24-May-05 17:35 kaiju_jsonrpc-0.1.1.dist-info/RECORD
+8 files, 15236 bytes uncompressed, 4857 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -1,22 +1,25 @@
 Filename: kaiju_jsonrpc/__init__.py
 Comment: 
 
 Filename: kaiju_jsonrpc/parser.py
 Comment: 
 
+Filename: kaiju_jsonrpc/py.typed
+Comment: 
+
 Filename: kaiju_jsonrpc/router.py
 Comment: 
 
-Filename: kaiju_jsonrpc-0.1.0.dist-info/METADATA
+Filename: kaiju_jsonrpc-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: kaiju_jsonrpc-0.1.0.dist-info/WHEEL
+Filename: kaiju_jsonrpc-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: kaiju_jsonrpc-0.1.0.dist-info/top_level.txt
+Filename: kaiju_jsonrpc-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: kaiju_jsonrpc-0.1.0.dist-info/RECORD
+Filename: kaiju_jsonrpc-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kaiju_jsonrpc/__init__.py

```diff
@@ -1,8 +1,9 @@
 """RPC server for kaiju-app libraries."""
+
 from kaiju_jsonrpc.parser import *
 from kaiju_jsonrpc.router import *
 
-__python_version__ = "3.12"
+__python_version__ = "3.11"
 __author__ = "violetblackdev@gmail.com"
 __license__ = "Apache Software License"
-__version__ = "0.1.0"
+__version__ = "0.1.1"
```

## kaiju_jsonrpc/parser.py

```diff
@@ -1,57 +1,70 @@
 """Request parser types."""
-from collections.abc import Mapping
+
 from time import time
-from typing import (Any, Awaitable, Callable, Collection, NamedTuple,
-                    TypeAlias, TypedDict, cast, final)
+from typing import Any, Awaitable, Callable, Collection, NamedTuple, TypeAlias, TypedDict, cast, final, Mapping
 
 from kaiju_app import Error as BaseError
 
 from kaiju_jsonrpc.router import Router
 
-__all__ = ['HTTPHeader', 'JSONHeader', 'RequestHeaders', 'MethodNotFound', 'InvalidRequest', 'InvalidParams', 'Parser',
-           'Request', 'RequestId', 'Response', 'Error', 'ErrorData', 'BatchRequest', 'BatchResponse', 'RPCError']
+__all__ = [
+    "Header",
+    "TypeId",
+    "RequestHeaders",
+    "MethodNotFound",
+    "InvalidRequest",
+    "InvalidParams",
+    "Parser",
+    "Request",
+    "RequestId",
+    "Response",
+    "Error",
+    "ErrorData",
+    "BatchRequest",
+    "BatchResponse",
+    "AnyResponse",
+    "RPCError",
+]
 
 _Func: TypeAlias = Callable[..., Awaitable[Any]]
 
 
 @final
-class HTTPHeader:
-    """Set of standard RPC headers."""
-
-    rpc_timeout = b"timeout"
-    rpc_deadline = b"deadline"
-    rpc_batch_abort_on_error = b"rpc-batch-abort-on-error"
-    rpc_retries = b"rpc-retries"
-
-
-@final
-class JSONHeader:
+class Header:
     """Set of standard RPC headers."""
 
+    correlation_id = 'correlation-id'
     rpc_timeout = "timeout"
     rpc_deadline = "deadline"
-    rpc_retries = "rpc-retries"
     rpc_batch_abort_on_error = "rpc-batch-abort-on-error"
+    rpc_retries = "rpc-retries"
+
+
+@final
+class TypeId:
+    request = 17
+    response = 18
+    error = 19
 
 
 class RequestHeaders(NamedTuple):
     timeout_s: float
     deadline: int | None
     retries: int
     batch_abort_on_error: bool
 
 
-RequestId: TypeAlias = int | str | bytes | None
+RequestId: TypeAlias = int | None
 
 
 class Request(TypedDict):
     id: RequestId
     method: str
-    params: dict | None
+    params: Mapping[str, Any] | None
 
 
 class Response(TypedDict):
     id: RequestId
     result: Any
 
 
@@ -63,15 +76,23 @@
 
 class Error(TypedDict):
     id: RequestId
     error: ErrorData
 
 
 BatchRequest: TypeAlias = Collection[Request]
-BatchResponse: TypeAlias = Collection[Response]
+BatchResponse: TypeAlias = Collection[Response | Error]
+AnyResponse: TypeAlias = BatchResponse | Response | Error
+RequestTuple: TypeAlias = tuple[int, RequestId, str, Mapping[str, Any] | None]
+ResponseTuple: TypeAlias = tuple[int, RequestId, Any]
+ErrorTuple: TypeAlias = tuple[int, RequestId, int, str, dict[str, Any] | None]
+BatchRequestTuple: TypeAlias = Collection[RequestTuple]
+BatchResponseTuple: TypeAlias = Collection[ResponseTuple | ErrorTuple]
+AnyRequestTuple: TypeAlias = RequestTuple | BatchRequestTuple
+AnyResponseTuple: TypeAlias = ResponseTuple | ErrorTuple | BatchResponseTuple
 
 
 class RPCError(BaseError):
     code = -32603
 
 
 class MethodNotFound(RPCError):
@@ -87,79 +108,87 @@
 
 
 class Parser:
     """RPC request header and body parser."""
 
     @staticmethod
     def get_request_headers_json(
-            headers: Mapping[str, Any], *,
-            default_request_timeout_s: float, max_request_timeout_s: float, max_request_retries: int,
+        headers: Mapping[str, Any],
+        *,
+        default_request_timeout_s: float,
+        max_request_timeout_s: float,
+        max_request_retries: int,
     ) -> RequestHeaders:
         """Parse request headers with JSON compatible data types."""
-        if JSONHeader.rpc_timeout in headers:
-            timeout = max(0., min(max_request_timeout_s, headers[JSONHeader.rpc_timeout]))
+        if Header.rpc_timeout in headers:
+            timeout = max(0.0, min(max_request_timeout_s, headers[Header.rpc_timeout]))
         else:
             timeout = default_request_timeout_s
-        deadline = headers.get(JSONHeader.rpc_deadline)
+        deadline = headers.get(Header.rpc_deadline)
         if deadline:
             timeout = min(deadline - time(), timeout)
-        if JSONHeader.rpc_retries in headers:
-            retries = max(0, min(max_request_retries, headers[JSONHeader.rpc_retries]))
+        if Header.rpc_retries in headers:
+            retries = max(0, min(max_request_retries, headers[Header.rpc_retries]))
         else:
             retries = 0
-        abort_on_error = headers.get(JSONHeader.rpc_batch_abort_on_error, True)
+        abort_on_error = headers.get(Header.rpc_batch_abort_on_error, True)
         return RequestHeaders(timeout, deadline, retries, abort_on_error)
 
     @staticmethod
     def get_request_headers_http(
-            headers: Mapping[bytes, bytes], *,
-            default_request_timeout_s: float, max_request_timeout_s: float, max_request_retries: int,
+        headers: Mapping[str, bytes | str],
+        *,
+        default_request_timeout_s: float,
+        max_request_timeout_s: float,
+        max_request_retries: int,
     ) -> RequestHeaders:
         """Parse request headers with HTTP binary strings."""
-        if HTTPHeader.rpc_timeout in headers:
-            timeout = max(0., min(max_request_timeout_s, float(headers[HTTPHeader.rpc_timeout])))
+        if Header.rpc_timeout in headers:
+            timeout = max(0.0, min(max_request_timeout_s, float(headers[Header.rpc_timeout])))
         else:
             timeout = default_request_timeout_s
-        if HTTPHeader.rpc_deadline in headers:
-            deadline = int(headers[HTTPHeader.rpc_deadline])
+        if Header.rpc_deadline in headers:
+            deadline = int(headers[Header.rpc_deadline])
             timeout = min(deadline - time(), timeout)
         else:
             deadline = None
-        if HTTPHeader.rpc_retries in headers:
-            retries = max(0, min(max_request_retries, int(headers[HTTPHeader.rpc_retries])))
+        if Header.rpc_retries in headers:
+            retries = max(0, min(max_request_retries, int(headers[Header.rpc_retries])))
         else:
             retries = 0
-        if HTTPHeader.rpc_batch_abort_on_error in headers:
-            abort_on_error = bool(int(headers[HTTPHeader.rpc_batch_abort_on_error]))
+        if Header.rpc_batch_abort_on_error in headers:
+            abort_on_error = bool(int(headers[Header.rpc_batch_abort_on_error]))
         else:
             abort_on_error = True
         return RequestHeaders(timeout, deadline, retries, abort_on_error)
 
+    @classmethod
+    def get_request_params(cls, request_body: Mapping[str, Any], /) -> tuple[RequestId, str, dict[str, Any] | None]:
+        request_id = request_body['id'] if 'id' in request_body else None
+        if type(request_id) is not int:
+            raise InvalidRequest('Request id must be integer')
+        if 'method' not in request_body:
+            raise InvalidRequest("Missing method parameter")
+        method_name = request_body['method']
+        if type(method_name) is not str:
+            raise InvalidRequest("Method must be a string")
+        params = request_body.get('params')
+        if params is not None and not hasattr(params, '__getitem__'):
+            raise InvalidRequest('Request params must be a mapping (dictionary object)')
+        return request_id, method_name, params
+
     @staticmethod
-    def get_request_call_args(router: Router, method: str, params: Any, permission: int) -> tuple[_Func, dict]:
-        """Get server call args."""
+    def get_server_call_args(router: Router, method: str, params: Mapping[str, Any] | None, permission: int) -> tuple[_Func, Mapping[str, Any]]:
         method_data = router.get(method)
         if method_data is None or method_data.permission < permission:
-            raise MethodNotFound(method) from None
-        if params is None:
-            params = {}
-            if method_data.keys_required:
-                raise InvalidParams(
-                    f'Missing required input params.', missing_keys=list(method_data.keys_required)
-                ) from None
-        elif not isinstance(params, Mapping):
-            raise InvalidRequest(
-                'Method params must be either null or an object.'
-            ) from None
-        else:
-            if not method_data.keys_required.issubset(params) or not method_data.keys.issuperset(params):
-                raise InvalidParams(
-                    'Invalid request params.',
-                    required_keys=method_data.keys_required,
-                    allowed_keys=method_data.keys
-                ) from None
+            raise MethodNotFound(method)
+        kws = {k: v for k, v in params.items() if not k.startswith('_')} if params else {}
+        if not method_data.keys_required.issubset(kws) or not method_data.keys.issuperset(kws):
+            raise InvalidParams(
+                "Invalid request params.", required_keys=method_data.keys_required, allowed_keys=method_data.keys
+            )
         if method_data.validator:
             try:
-                params = method_data.validator(params)
+                kws = method_data.validator(kws)
             except Exception as exc:
                 raise InvalidParams(str(exc), method=method, params=params, schema=method_data.schema)
-        return method_data.func, cast(dict, params)
+        return method_data.func, cast(dict, kws)
```

## kaiju_jsonrpc/router.py

```diff
@@ -1,25 +1,26 @@
 """RPC router."""
+
 import inspect
 from abc import abstractmethod
 from collections.abc import Collection
 from dataclasses import dataclass, field
 from fnmatch import fnmatch
-from typing import (Any, Awaitable, Callable, ClassVar, Mapping, NamedTuple,
-                    Protocol, TypeAlias, TypeGuard, cast, final)
+from typing import Any, Awaitable, Callable, ClassVar, Mapping, NamedTuple, Protocol, TypeAlias, TypeGuard, cast, final
 
 from fastjsonschema import compile as compile_schema
 from jsonschema_gen import Parser as AnnotationParser
-from jsonschema_gen.schema import JSONSchemaObject, JSONSchemaType
+from jsonschema_gen.schema import Object, JSONSchemaObject
 from kaiju_app import Application
 
-__all__ = ["Router", 'Method', "RPCInterface", "is_rpc_interface"]
+__all__ = ["Router", "Method", "RPCInterface", "is_rpc_interface"]
 
 
-ValidatorType: TypeAlias = Callable[[Mapping[str, Any]], Mapping[str, Any]] | JSONSchemaType
+ValidatorFunction: TypeAlias = Callable[[Mapping[str, Any]], dict[str, Any]]
+ValidatorType: TypeAlias = ValidatorFunction | Object
 
 
 @final
 class Method(NamedTuple):
     func: Callable[..., Awaitable]
     permission: int = 0
     validator: ValidatorType | None = None
@@ -40,26 +41,26 @@
 
 @final
 class _Method(NamedTuple):
     func: Callable[..., Awaitable]
     keys: frozenset[str]
     keys_required: frozenset[str]
     permission: int
-    schema: JSONSchemaType
-    validator: ValidatorType | None
+    schema: Object | None
+    validator: ValidatorFunction | None
 
 
 @dataclass
 class Router(Mapping[str, _Method]):
     """Router for RPC methods.
 
     It contains a map of RPC routes to Python methods, validators, permissions, etc.
     """
 
-    private_key_prefix: ClassVar[str] = '_'
+    private_key_prefix: ClassVar[str] = "_"
     """Ignore method input parameters starting with such prefix."""
 
     auto_create_validators: bool = True
     """Auto-create validators for methods with missing validators."""
 
     whitelist_routes: Collection[str] = field(default=tuple())
     """Whitelist of routes or route patterns, by default it's all of them."""
@@ -76,20 +77,20 @@
     def __iter__(self):
         return iter(self._routes)
 
     def clear(self):
         self._routes.clear()
 
     def json_repr(self) -> dict[str, Any]:
-        routes = [
-            {"id": route, "permission": method.permission, "schema": method.schema}
-            for route, method in self._routes.items()
-        ]
-        routes.sort(key=lambda route: route["id"])
-        return {"routes": routes}
+        return {
+            "routes": [
+                {"id": route, "permission": method.permission, "schema": method.schema}
+                for route, method in sorted(self._routes.items())
+            ]
+        }
 
     def add_routes_from_app(self, app: Application, /) -> None:
         for name, service in app.services.items():
             if is_rpc_interface(service):
                 self.add_routes_from_interface(cast(RPCInterface, service), name=name)
 
     def add_routes_from_interface(self, interface: RPCInterface, /, name: str | None = None) -> None:
@@ -100,16 +101,20 @@
             if not self.is_in_whitelist(full_route):
                 continue
             if not isinstance(method, Method):
                 method = Method(func=method)
             schema, validator = self._create_method_validator(interface, method)
             keys, keys_required = self._get_method_kws(method.func)
             self._routes[full_route] = _Method(
-                func=method.func, permission=method.permission, schema=schema, validator=validator,
-                keys=keys, keys_required=keys_required
+                func=method.func,
+                permission=method.permission,
+                schema=schema,
+                validator=validator,
+                keys=keys,
+                keys_required=keys_required,
             )
 
     def is_in_whitelist(self, route: str, /) -> bool:
         """Check if a route is allowed."""
         if not self.whitelist_routes:
             return True
         for pattern in self.whitelist_routes:
@@ -130,19 +135,26 @@
             keys.append(key.name)
             if key.default is key.empty:
                 keys_required.append(key.name)
         return frozenset(keys), frozenset(keys_required)
 
     def _create_method_validator(
         self, interface: RPCInterface, method: Method, /
-    ) -> tuple[JSONSchemaType, ValidatorType]:
-        validator = method.validator
+    ) -> tuple[Object | None, ValidatorFunction | None]:
         try:
-            schema = self._parser.parse_function(method.func, type(interface))
+            schema = self._parser.parse_function(method.func, type(interface)).kwargs
         except Exception:
-            schema = JSONSchemaObject(title="!unsupported type")
-        else:
-            if self.auto_create_validators and method.validator is None:
-                validator = schema
+            keys, keys_required = self._get_method_kws(method.func)
+            schema = Object(
+                {arg: JSONSchemaObject(title="unknown type") for arg in keys},
+                additionalProperties=False,
+                required=list(keys_required),
+            )
+
+        validator = method.validator
+        if validator is None and self.auto_create_validators:
+            validator = schema
+
         if validator is not None and hasattr(validator, "json_repr"):
             validator = compile_schema(validator.json_repr())
+
         return schema, validator
```

## Comparing `kaiju_jsonrpc-0.1.0.dist-info/METADATA` & `kaiju_jsonrpc-0.1.1.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: kaiju-jsonrpc
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python asyncio JSONRPC tools for kaiju applications
 Home-page: https://github.com/violet-black/kaiju-jsonrpc
 Author: violetblackdev@gmail.com
 License: Apache Software License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.12
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: kaiju-app
 Requires-Dist: fastjsonschema
 Requires-Dist: jsonschema-gen
 Provides-Extra: dev
 Requires-Dist: pip-tools ; extra == 'dev'
 Requires-Dist: tox ; extra == 'dev'
```

