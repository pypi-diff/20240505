# Comparing `tmp/pyauth0-0.1.3a2.tar.gz` & `tmp/pyauth0-0.1.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyauth0-0.1.3a2.tar", max compression
+gzip compressed data, was "pyauth0-0.1.4a0.tar", max compression
```

## Comparing `pyauth0-0.1.3a2.tar` & `pyauth0-0.1.4a0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2024-05-04 15:37:35.931397 pyauth0-0.1.3a2/LICENSE
--rw-r--r--   0        0        0     2009 2024-05-04 15:37:35.931397 pyauth0-0.1.3a2/README.md
--rw-r--r--   0        0        0      147 2024-05-04 15:37:35.931397 pyauth0-0.1.3a2/pyauth0/__init__.py
--rw-r--r--   0        0        0      241 2024-05-04 15:37:35.931397 pyauth0-0.1.3a2/pyauth0/errors.py
--rw-r--r--   0        0        0     3352 2024-05-04 15:37:35.931397 pyauth0-0.1.3a2/pyauth0/token_provider.py
--rw-r--r--   0        0        0     5273 2024-05-04 15:37:35.931397 pyauth0-0.1.3a2/pyauth0/token_verifier.py
--rw-r--r--   0        0        0      659 2024-05-04 15:37:35.931397 pyauth0-0.1.3a2/pyproject.toml
--rw-r--r--   0        0        0     2752 1970-01-01 00:00:00.000000 pyauth0-0.1.3a2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-04 17:35:17.026207 pyauth0-0.1.4a0/LICENSE
+-rw-r--r--   0        0        0     2746 2024-05-04 17:35:17.026207 pyauth0-0.1.4a0/README.md
+-rw-r--r--   0        0        0      147 2024-05-04 17:35:17.026207 pyauth0-0.1.4a0/pyauth0/__init__.py
+-rw-r--r--   0        0        0      241 2024-05-04 17:35:17.026207 pyauth0-0.1.4a0/pyauth0/errors.py
+-rw-r--r--   0        0        0     4647 2024-05-04 17:35:17.026207 pyauth0-0.1.4a0/pyauth0/token_provider.py
+-rw-r--r--   0        0        0     5273 2024-05-04 17:35:17.026207 pyauth0-0.1.4a0/pyauth0/token_verifier.py
+-rw-r--r--   0        0        0      809 2024-05-04 17:35:17.026207 pyauth0-0.1.4a0/pyproject.toml
+-rw-r--r--   0        0        0     3616 1970-01-01 00:00:00.000000 pyauth0-0.1.4a0/PKG-INFO
```

### Comparing `pyauth0-0.1.3a2/LICENSE` & `pyauth0-0.1.4a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyauth0-0.1.3a2/README.md` & `pyauth0-0.1.4a0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -5,45 +5,76 @@
 [![PyPI version](https://badge.fury.io/py/pyauth0.svg)](https://badge.fury.io/py/pyauth0)
 
 Python utilities for [Auth0](https://auth0.com/).
 
 - [Install](#install)
 - [Usage](#usage)
   - [Get a machine-to-machine token](#get-a-machine-to-machine-token)
+  - [Get a machine-to-machine token asynchronously](#get-a-machine-to-machine-token-asynchronously)
   - [Verify a token](#verify-a-token)
 - [Contribute](#contribute)
 
 ## Install
 
 ```shell
 pip install pyauth0
 ```
 
+Or, if you plan to use async features:
+
+```shell
+pip install pyauth0[async]
+```
+
 ## Usage
 
 ### Get a machine-to-machine token
 
 ```python
-from pyauth0 import TokenProvider
+import pyauth0
 from urllib.request import Request, urlopen
 
-token_provider = TokenProvider(
+token_provider = pyauth0.TokenProvider(
     issuer="your-domain.auth0.com",
     audience="https://api.your-domain.com",
     client_id="1234",
     client_secret="secret"
 )
 
 # Machine to machine request
+token: pyauth0.GetTokenResponse = token_provider.get_token()
 response = urlopen(Request(
     "https://api.your-domain.com",
-    headers={"authorization": token_provider.get_token().get_authorization()},
+    headers={"authorization": token.get_authorization()},
 ))
 ```
 
+### Get a machine-to-machine token asynchronously
+
+```python
+import httpx
+
+import pyauth0
+
+token_provider = pyauth0.TokenProvider(
+  issuer="your-domain.auth0.com",
+  audience="https://api.your-domain.com",
+  client_id="1234",
+  client_secret="secret"
+)
+
+# Machine to machine request
+token: pyauth0.GetTokenResponse = await token_provider.aget_token()
+async with httpx.AsyncClient() as client:
+  response = await client.get(
+    "https://api.your-domain.com",
+    headers={"authorization": token.get_authorization()},
+  )
+```
+
 ### Verify a token
 
 ```python
 from pyauth0 import TokenVerifier, Auth0Error
 
 token_verifier = TokenVerifier(
     issuer="your-domain.auth0.com",
```

### Comparing `pyauth0-0.1.3a2/pyauth0/token_provider.py` & `pyauth0-0.1.4a0/pyauth0/token_provider.py`

 * *Files 27% similar despite different names*

```diff
@@ -53,48 +53,76 @@
         self._client_id = client_id
         self._client_secret = client_secret
         self._payload_customizer = payload_customizer
         self._cache: typing.Optional[GetTokenResponse] = None
 
     def get_token(self) -> GetTokenResponse:
         if self._cache is None or self._cache.is_expired():
-            url = f"https://{self._issuer}/oauth/token"
-            payload = {
-                "grant_type": "client_credentials",
-                "audience": self._audience,
-                "client_id": self._client_id,
-                "client_secret": self._client_secret,
-            }
-            if self._payload_customizer:
-                payload = self._payload_customizer(payload)
-
-            request_data = json.dumps(payload)
-            request = Request(
-                url,
-                method="POST",
-                data=request_data.encode("utf-8"),
-                headers={"content-type": "application/json"},
-            )
-
+            url, method, request_bytes, headers = self._prepare_request()
             try:
-                response = urlopen(request)
+                response = urlopen(
+                    Request(
+                        url,
+                        method=method,
+                        data=request_bytes,
+                        headers=headers,
+                    )
+                )
             except HTTPError as error:
                 raise RuntimeError(
-                    f"Invalid response POST {url} {request_data} >> {error.code}"
+                    f"Invalid response {method} {url} {request_bytes} >> {error.code}"
                 )
-
-            response_data = response.read().decode("utf-8")
+            response_bytes = response.read()
             if response.status != 200:
                 raise RuntimeError(
-                    f"Invalid response POST {url} {request_data} >> {response.status} {response_data}"
+                    f"Invalid response {method} {url} {request_bytes} >> {response.status} {response_bytes}"
                 )
+            self._accept_response_bytes(response_bytes)
+        return self._cache
 
-            response_dict = json.loads(response_data)
-            self._cache = GetTokenResponse(
-                response_body=response_dict,
-                access_token=response_dict.get("access_token"),
-                token_type=response_dict.get("token_type"),
-                expires_at=datetime.datetime.now()
-                + datetime.timedelta(seconds=response_dict.get("expires_in")),
-            )
+    async def aget_token(self) -> GetTokenResponse:
+        if self._cache is None or self._cache.is_expired():
+            url, method, request_bytes, headers = self._prepare_request()
+            try:
+                import httpx
 
+                async with httpx.AsyncClient() as client:
+                    response = await client.post(
+                        url,
+                        data=request_bytes,
+                        headers=headers,
+                    )
+            except Exception as error:
+                raise RuntimeError(
+                    f"Invalid response {method} {url} {request_bytes} >> {error}"
+                )
+            response_bytes = response.content
+            if response.status_code != 200:
+                raise RuntimeError(
+                    f"Invalid response {method} {url} {request_bytes} >> {response.status_code} {response_bytes}"
+                )
+            self._accept_response_bytes(response_bytes)
         return self._cache
+
+    def _prepare_request(self) -> (str, str, bytes, dict):
+        url = f"https://{self._issuer}/oauth/token"
+        payload = {
+            "grant_type": "client_credentials",
+            "audience": self._audience,
+            "client_id": self._client_id,
+            "client_secret": self._client_secret,
+        }
+        if self._payload_customizer:
+            payload = self._payload_customizer(payload)
+        request_bytes = json.dumps(payload).encode()
+        headers = {"content-type": "application/json"}
+        return url, "POST", request_bytes, headers
+
+    def _accept_response_bytes(self, response_bytes: bytes):
+        response_dict = json.loads(response_bytes.decode())
+        self._cache = GetTokenResponse(
+            response_body=response_dict,
+            access_token=response_dict.get("access_token"),
+            token_type=response_dict.get("token_type"),
+            expires_at=datetime.datetime.now()
+            + datetime.timedelta(seconds=response_dict.get("expires_in")),
+        )
```

### Comparing `pyauth0-0.1.3a2/pyauth0/token_verifier.py` & `pyauth0-0.1.4a0/pyauth0/token_verifier.py`

 * *Files identical despite different names*

### Comparing `pyauth0-0.1.3a2/pyproject.toml` & `pyauth0-0.1.4a0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 [tool.poetry]
 name = "pyauth0"
-version = "0.1.3a2"
+version = "0.1.4a0"
 description = "Python utilities for Auth0"
 authors = ["svaponi <10941963+svaponi@users.noreply.github.com>"]
 readme = "README.md"
-homepage = "https://github.com/svaponi/pyauth0"
+homepage = "https://svaponi.github.io/pyauth0"
+repository = "https://github.com/svaponi/pyauth0"
 license = "MIT"
-classifiers = ['Development Status :: 5 - Production/Stable']
+classifiers = ['Development Status :: 4 - Beta']
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.13"
 python-jose = "^3.3.0"
-
+httpx = { version = "^0.27.0", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.0"
 python-dotenv = "^1.0.1"
+pytest-asyncio = "^0.23.6"
 
+[tool.poetry.extras]
+async = ["httpx"]
 
 [tool.poetry.group.coverage]
 optional = true
 
 [tool.poetry.group.coverage.dependencies]
 coveralls = "^4.0.0"
```

