# Comparing `tmp/missil-0.1.6b0.tar.gz` & `tmp/missil-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "missil-0.1.6b0.tar", last modified: Mon Jan 29 21:59:54 2024, max compression
+gzip compressed data, was "missil-0.1.7.tar", last modified: Sun May  5 02:22:29 2024, max compression
```

## Comparing `missil-0.1.6b0.tar` & `missil-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1077 2024-01-29 21:58:57.661474 missil-0.1.6b0/LICENSE
--rw-r--r--   0        0        0     3095 2024-01-29 21:58:57.661474 missil-0.1.6b0/README.md
--rw-r--r--   0        0        0      952 2024-01-29 21:58:57.665474 missil-0.1.6b0/missil/__init__.py
--rw-r--r--   0        0        0     5211 2024-01-29 21:58:57.665474 missil-0.1.6b0/missil/bearers.py
--rw-r--r--   0        0        0     1523 2024-01-29 21:58:57.665474 missil-0.1.6b0/missil/exceptions.py
--rw-r--r--   0        0        0     2555 2024-01-29 21:58:57.665474 missil-0.1.6b0/missil/jwt_utilities.py
--rw-r--r--   0        0        0     3124 2024-01-29 21:58:57.665474 missil-0.1.6b0/missil/routers.py
--rw-r--r--   0        0        0     5652 2024-01-29 21:58:57.665474 missil-0.1.6b0/missil/rules.py
--rw-r--r--   0        0        0     4609 2024-01-29 21:59:54.853633 missil-0.1.6b0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-29 21:56:14.420907 missil-0.1.6b0/tests/__init__.py
--rw-r--r--   0        0        0      380 2024-01-29 21:58:57.665474 missil-0.1.6b0/tests/conftest.py
--rw-r--r--   0        0        0     5123 2024-01-29 21:58:57.665474 missil-0.1.6b0/tests/test_jwt_utilities.py
--rw-r--r--   0        0        0     1419 2024-01-29 21:58:57.665474 missil-0.1.6b0/tests/test_sample_api.py
--rw-r--r--   0        0        0      301 2024-01-29 21:58:57.665474 missil-0.1.6b0/tests/utils.py
--rw-r--r--   0        0        0     4607 1970-01-01 00:00:00.000000 missil-0.1.6b0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-05-05 02:11:55.446725 missil-0.1.7/LICENSE
+-rw-r--r--   0        0        0     3095 2024-05-05 02:11:55.446725 missil-0.1.7/README.md
+-rw-r--r--   0        0        0     1003 2024-05-05 02:11:55.446725 missil-0.1.7/missil/__init__.py
+-rw-r--r--   0        0        0     5972 2024-05-05 02:11:55.446725 missil-0.1.7/missil/bearers.py
+-rw-r--r--   0        0        0     1578 2024-05-05 02:11:55.446725 missil-0.1.7/missil/exceptions.py
+-rw-r--r--   0        0        0     2650 2024-05-05 02:11:55.446725 missil-0.1.7/missil/jwt_utilities.py
+-rw-r--r--   0        0        0     3102 2024-05-05 02:11:55.446725 missil-0.1.7/missil/routers.py
+-rw-r--r--   0        0        0     6442 2024-05-05 02:11:55.446725 missil-0.1.7/missil/rules.py
+-rw-r--r--   0        0        0     5009 2024-05-05 02:22:29.076828 missil-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-05 02:11:55.446725 missil-0.1.7/tests/__init__.py
+-rw-r--r--   0        0        0      756 2024-05-05 02:11:55.446725 missil-0.1.7/tests/conftest.py
+-rw-r--r--   0        0        0     5121 2024-05-05 02:11:55.446725 missil-0.1.7/tests/test_jwt_utilities.py
+-rw-r--r--   0        0        0     1158 2024-05-05 02:11:55.446725 missil-0.1.7/tests/test_rules.py
+-rw-r--r--   0        0        0     1755 2024-05-05 02:11:55.446725 missil-0.1.7/tests/test_sample_api.py
+-rw-r--r--   0        0        0      300 2024-05-05 02:11:55.446725 missil-0.1.7/tests/utils.py
+-rw-r--r--   0        0        0     4566 1970-01-01 00:00:00.000000 missil-0.1.7/PKG-INFO
```

### Comparing `missil-0.1.6b0/LICENSE` & `missil-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `missil-0.1.6b0/README.md` & `missil-0.1.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center">
-  <a href="https://ericmiguel.github.io/missil"><img src="https://github.com/ericmiguel/missil/assets/12076399/c7841626-706e-425f-99d6-c91fd6fb3455" alt="Missil"></a>
+  <a href="https://ericmiguel.github.io/missil"><img src="https://github.com/ericmiguel/missil/assets/12076399/dfe4a649-a226-42b4-851d-698fbb664bc7" alt="Missil"></a>
 </p>
 <p align="center">
     <em>Simple <a href="https://fastapi.tiangolo.com/">FastAPI</a> declarative endpoint-level access control, somewhat inspired by <a href="https://docs.pylonsproject.org/projects/pyramid/en/latest/narr/security.html">Pyramid</a>.</em>
 </p>
 <p align="center">
     <span><a href="https://ericmiguel.github.io/missil/" target="_blank">[DOCS]</a></span>
     <span><a href="https://github.com/ericmiguel/missil" target="_blank">[SOURCE]</a></span>
```

### Comparing `missil-0.1.6b0/missil/__init__.py` & `missil-0.1.7/missil/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 """Simple FastAPI declarative endpoint-level access control."""
 
-
 from missil.bearers import CookieTokenBearer
 from missil.bearers import FlexibleTokenBearer
 from missil.bearers import HTTPTokenBearer
 from missil.bearers import TokenBearer
 from missil.exceptions import PermissionErrorException
 from missil.exceptions import TokenErrorException
 from missil.jwt_utilities import decode_jwt_token
 from missil.jwt_utilities import encode_jwt_token
 from missil.routers import QualifiedRouter
 from missil.rules import DENY
 from missil.rules import READ
 from missil.rules import WRITE
 from missil.rules import Rule
+from missil.rules import make_rule
 from missil.rules import make_rules
 
 
 __all__ = [
     "PermissionErrorException",
     "TokenErrorException",
     "TokenBearer",
     "encode_jwt_token",
     "decode_jwt_token",
     "CookieTokenBearer",
     "HTTPTokenBearer",
     "FlexibleTokenBearer",
     "Rule",
+    "make_rule",
     "make_rules",
     "QualifiedRouter",
     "READ",
     "WRITE",
     "DENY",
 ]
```

### Comparing `missil-0.1.6b0/missil/bearers.py` & `missil-0.1.7/missil/bearers.py`

 * *Files 20% similar despite different names*

```diff
@@ -41,16 +41,16 @@
 
             Supposing the following decoded token claim:
             ```python
             {
                 "username": "John Doe",
                 "permissions": {  # user_permissions_key
                     "finances": 0,
-                    "it": 0
-                }
+                    "it": 0,
+                },
             }
             ```
 
         algorithms : str, optional
             JWT token decode algorithm, by default "HS256". See Python-jose docs
             for more details.
         """
@@ -91,68 +91,76 @@
         return self.split_token_str(token)
 
     def decode_jwt(self, token: str) -> dict[str, int]:
         """Decode a retrieved token value and return the user permissions."""
         decoded_token = decode_jwt_token(
             token, self.token_secret_key, algorithm=self.algorithm
         )
+        return decoded_token
+
+    def decode_from_cookies(self, request: Request) -> dict[str, Any]:
+        """Get token from cookies and decode it."""
+        token = self.get_token_from_cookies(request)
+        return self.decode_jwt(token)
 
+    def decode_from_header(self, request: Request) -> dict[str, Any]:
+        """Get token from headers and decode it."""
+        token = self.get_token_from_header(request)
+        return self.decode_jwt(token)
+
+    def get_user_permissions(self, decoded_token: dict[str, Any]) -> dict[str, int]:
+        """Get user permissions from a decoded token."""
         if self.user_permissions_key:
             try:
                 user_permissions: dict[str, int] = decoded_token[
                     self.user_permissions_key
                 ]
-            except KeyError:
+            except KeyError as ke:
                 raise TokenErrorException(
                     401,
                     (
                         "User permissions not found at token key "
                         f"'{self.user_permissions_key}'"
                     ),
-                )
+                ) from ke
             else:
                 return user_permissions
 
-        return decoded_token
-
-    async def __call__(self, *args: Any, **kwds: Any) -> dict[str, int]:
-        """Declared just to avoid code checking alerts."""
-        return {"": 0}
+        raise TokenErrorException(500, "User permissions key not provided.")
 
 
 class CookieTokenBearer(TokenBearer):
     """Read JWT token from http cookies."""
 
-    async def __call__(
-        self, request: Request, *args: Any, **kwds: Any
-    ) -> dict[str, int]:
+    async def __call__(self, request: Request) -> tuple[dict[str, Any], dict[str, int]]:
         """Fastapi FastAPIDependsFunc will call this method."""
-        token = self.get_token_from_cookies(request)
-        return self.decode_jwt(token)
+        decoded_token = self.decode_from_cookies(request)
+        user_permissions = self.get_user_permissions(decoded_token)
+        return decoded_token, user_permissions
 
 
 class HTTPTokenBearer(TokenBearer):
     """Read JWT token from the request header."""
 
-    async def __call__(
-        self, request: Request, *args: Any, **kwds: Any
-    ) -> dict[str, int]:
+    async def __call__(self, request: Request) -> tuple[dict[str, Any], dict[str, int]]:
         """Fastapi FastAPIDependsFunc will call this method."""
-        token = self.get_token_from_header(request)
-        return self.decode_jwt(token)
+        decoded_token = self.decode_from_header(request)
+        user_permissions = self.get_user_permissions(decoded_token)
+        return decoded_token, user_permissions
 
 
 class FlexibleTokenBearer(TokenBearer):
     """Tries to read the token from the cookies or from request headers."""
 
-    async def __call__(self, request: Request) -> dict[str, int]:
+    async def __call__(self, request: Request) -> tuple[dict[str, Any], dict[str, int]]:
         """Fastapi FastAPIDependsFunc will call this method."""
         try:
-            token = self.get_token_from_cookies(request)
+            decoded_token = self.decode_from_cookies(request)
         except TokenErrorException:
-            token = self.get_token_from_header(request)
-        except Exception:
+            decoded_token = self.decode_from_header(request)
+        except Exception as e:
             raise TokenErrorException(
                 status.HTTP_417_EXPECTATION_FAILED, "Token not found."
-            )
+            ) from e
 
-        return self.decode_jwt(token)
+        user_permissions = self.get_user_permissions(decoded_token)
+        return decoded_token, user_permissions
```

### Comparing `missil-0.1.6b0/missil/exceptions.py` & `missil-0.1.7/missil/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,55 +1,57 @@
 """Missil custom exceptions."""
 
 from fastapi import HTTPException
 
 
 class PermissionErrorException(HTTPException):
-    """
-    An HTTP exception you can raise in your own code to show errors to the client.
-
-    Mainly for client errors, invalid authentication, invalid data, etc.
-    """
+    """HTTP Exception you can raise to show on permission-related errors."""
 
     def __init__(
         self,
         status_code: int,
         detail: str,
-        headers: dict[str, str] | None = {"WWW-Authenticate": "Bearer"},
+        headers: dict[str, str] | None = None,
     ) -> None:
         """
-        A HTTPException.
+        Initialize a PermissionErrorException.
 
         Parameters
         ----------
         status_code : int
             HTTP status code.
         detail : str
             Exception description.
         headers : _type_, optional
             Response headers, by default {"WWW-Authenticate": "Bearer"}
         """
+        if headers is None:
+            headers = {"WWW-Authenticate": "Bearer"}
+
         super().__init__(status_code=status_code, detail=detail, headers=headers)
 
 
 class TokenErrorException(HTTPException):
     """HTTP Exception you can raise to show on JWT token-related errors."""
 
     def __init__(
         self,
         status_code: int,
         detail: str,
-        headers: dict[str, str] | None = {"WWW-Authenticate": "Bearer"},
+        headers: dict[str, str] | None = None,
     ) -> None:
         """
-        A HTTPException.
+        Initialize a TokenErrorException.
 
         Parameters
         ----------
         status_code : int
             HTTP status code.
         detail : str
             Exception description.
         headers : _type_, optional
             Response headers, by default {"WWW-Authenticate": "Bearer"}
         """
+        if headers is None:
+            headers = {"WWW-Authenticate": "Bearer"}
+
         super().__init__(status_code=status_code, detail=detail, headers=headers)
```

### Comparing `missil-0.1.6b0/missil/jwt_utilities.py` & `missil-0.1.7/missil/jwt_utilities.py`

 * *Files 18% similar despite different names*

```diff
@@ -43,35 +43,35 @@
     TokenErrorException
         Generalist exception. The token signature is invalid.
     TokenErrorException
         Most generalist exception. The token is invalid.
     """
     try:
         decoded_token = jwt.decode(token, secret_key, algorithms=algorithm)
-    except ExpiredSignatureError:
+    except ExpiredSignatureError as ese:
         raise TokenErrorException(
             status.HTTP_403_FORBIDDEN, "The token signature has expired."
-        )
-    except JWTClaimsError:
+        ) from ese
+    except JWTClaimsError as jce:
         raise TokenErrorException(
             status.HTTP_403_FORBIDDEN, "The token claim is invalid."
-        )
-    except JWTError:  # generalist exception handler
+        ) from jce
+    except JWTError as je:  # generalist exception handler
         raise TokenErrorException(
             status.HTTP_403_FORBIDDEN, "The token signature is invalid."
-        )
+        ) from je
 
     return decoded_token
 
 
 def encode_jwt_token(
     claims: dict[str, Any],
     secret: str,
     exp: int,
-    base: datetime = datetime.now(timezone.utc),
+    base: datetime | None = None,
     algorithm: str = "HS256",
 ) -> str:
     """
     Create a JWT token.
 
     Parameters
     ----------
@@ -88,10 +88,13 @@
         Encode algorithm, by default "HS256"
 
     Returns
     -------
     str
         _description_
     """
+    if base is None:
+        base = datetime.now(timezone.utc)
+
     to_encode = claims.copy()
     to_encode.update({"exp": base + timedelta(exp)})
     return jwt.encode(to_encode, key=secret, algorithm=algorithm)
```

### Comparing `missil-0.1.6b0/missil/routers.py` & `missil-0.1.7/missil/routers.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         on_shutdown: Sequence[Callable[[], Any]] | None = None,
         lifespan: Lifespan[Any] | None = None,
         deprecated: bool | None = None,
         include_in_schema: bool = True,
         generate_unique_id_function: Callable[[APIRoute], str] = generate_unique_id,
     ) -> None:
         """
-        Same parameters as in FastAPI APIRouter class, plus an extra rules parameter.
+        FastAPI APIRouter class, plus an extra rules parameter.
 
         It can be used to avoid multiple redudant rule declarations in same
         business area endpoints.
 
         Example:
 
         ```python
```

### Comparing `missil-0.1.6b0/missil/rules.py` & `missil-0.1.7/missil/rules.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,28 +52,41 @@
         self.use_cache = use_cache
 
     @property
     def dependency(self) -> Callable[..., Any] | None:
         """Allows Missil to pass a FastAPI dependency that gets correctly evaluated."""
 
         def check_user_permissions(
-            claims: Annotated[dict[str, int], FastAPIDependsFunc(self.bearer)]
-        ) -> None:
+            claims: Annotated[
+                tuple[
+                    dict[str, Any],  ## full claims
+                    dict[str, int],  ## user permissions
+                ],
+                FastAPIDependsFunc(self.bearer),
+            ],
+        ) -> dict[str, Any]:
             """
             Run JWT claims against an declared endpoint rule.
 
             If claims contains the asked business area and sufficient access level,
-            the endpoint access is granted to the user.
+            the endpoint access is granted to the user and the full claims are returned.
 
             Parameters
             ----------
-            claims : Annotated[dict[str, int], FastAPIDependsFunc
+            claims : Annotated[
+                    tuple[
+                        dict[str, Any],
+                        dict[str, int]
+                    ],
+                    FastAPIDependsFunc
+                ]
+
                 Content decoded from a JWT Token, obtained after FastAPI resolves
-                the TokenBearer dependency. Missil expects an dict using the
-                following structure:
+                the TokenBearer dependency. Missil expects a permission dict like the
+                following example structure:
 
                 ```python
                 {
                     'business area name': READ,
                     'business area name': WRITE,
                     'business area name 2': READ
                     'business area name 2': WRITE
@@ -83,26 +96,28 @@
             Raises
             ------
             PermissionErrorException
                 Business area not listed on claims.
             PermissionErrorException
                 Insufficient access level.
             """
-            if self.area not in claims:
+            if self.area not in claims[1]:
                 raise PermissionErrorException(
                     status.HTTP_403_FORBIDDEN, f"'{self.area}' not in user permissions."
                 )
 
-            if not claims[self.area] >= self.level:
+            if not claims[1][self.area] >= self.level:
                 raise PermissionErrorException(
                     status.HTTP_403_FORBIDDEN,
                     "insufficient access level: "
-                    f"({claims[self.area]}/{self.level}) on {self.area}.",
+                    f"({claims[1][self.area]}/{self.level}) on {self.area}.",
                 )
 
+            return claims[0]
+
         return check_user_permissions
 
     if TYPE_CHECKING:
 
         @dependency.setter
         def dependency(self, _: Any) -> None:
             """
@@ -117,25 +132,25 @@
     Business area.
 
     A business area instance holds up READ and WRITE rules as attributes, which
     can be injected as a FastAPI endpoint dependency. For example:
 
     ```python
     bearer = ...
-    finances = Area('finances', bearer)
+    finances = Area("finances", bearer)
+
 
     @app.get("/finances/read", dependencies=[finances.READ])
-    def finances_read() -> dict[str, str]:
-        ...
+    def finances_read() -> dict[str, str]: ...
     ```
     """
 
     def __init__(self, name: str, bearer: TokenBearer) -> None:
         """
-        Creates a business area object.
+        Create a business area object.
 
         Parameters
         ----------
         name : str
             Business area name.
         bearer : TokenBearer
             JWT token source source. See Bearers module.
@@ -170,16 +185,15 @@
     }
     ```
 
     So, one can pass like a FastAPI dependency, as shown in the following example:
 
     ```python
     @app.get("/items/{item_id}", dependencies=[rules["finances"].READ])
-    def read_item(item_id: int, q: Union[str, None] = None):
-        ...
+    def read_item(item_id: int, q: Union[str, None] = None): ...
     ```
 
     See the sample API (sample/main.py) to a folly working usage example.
 
     Parameters
     ----------
     bearer : TokenBearer
@@ -187,7 +201,26 @@
 
     Returns
     -------
     dict[str, Area]
         Dict containing endpoint-appliable rules.
     """
     return {area: Area(area, bearer) for area in areas}
+
+
+def make_rule(bearer: TokenBearer, area: str) -> Area:
+    """
+    Create a single Missil rule.
+
+    Parameters
+    ----------
+    bearer : TokenBearer
+        JWT token source source. See Bearers module.
+    area : str
+        A business area name.
+
+    Returns
+    -------
+    Area
+        Business area object, containing READ and WRITE rules.
+    """
+    return Area(area, bearer)
```

### Comparing `missil-0.1.6b0/tests/test_jwt_utilities.py` & `missil-0.1.7/tests/test_jwt_utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-import logging
-
 from datetime import datetime
 from datetime import timedelta
 from datetime import timezone
-
-import pytest
+import logging
 
 from jose import jwt
+import pytest
 
 from missil import jwt_utilities
 from missil.exceptions import TokenErrorException
 from tests.utils import ignore_warnings
 
 
 log = logging.getLogger(__name__)
```

### Comparing `missil-0.1.6b0/tests/test_sample_api.py` & `missil-0.1.7/tests/test_sample_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,7 +42,20 @@
     ],
 )
 def test_write_access(api_url, response_msg, test_app, bearer_token):
     response = test_app.get(api_url, headers={"Authorization": bearer_token})
 
     assert response.status_code == 403
     assert response.json() == {"detail": response_msg}
+
+
+@ignore_warnings
+@pytest.mark.parametrize(
+    "api_url",
+    [
+        "/user-profile",
+    ],
+)
+def test_get_current_user(api_url, test_app, bearer_token, decoded_token):
+    response = test_app.get(api_url, headers={"Authorization": bearer_token})
+    assert response.status_code == 200
+    assert response.json() == decoded_token
```

### Comparing `missil-0.1.6b0/PKG-INFO` & `missil-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: missil
-Version: 0.1.6b0
+Version: 0.1.7
 Summary: Simple FastAPI declarative endpoint-level access control.
 Author-Email: Eric Miguel <eric.mrib@gmail.com>
 License: MIT
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -16,30 +16,29 @@
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO
 Classifier: Framework :: FastAPI
 Classifier: Framework :: Pydantic
-Classifier: Framework :: Pydantic :: 1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.10
 Requires-Dist: fastapi>=0.104.1
 Requires-Dist: python-jose[cryptography]>=3.3.0
 Description-Content-Type: text/markdown
 
 <p align="center">
-  <a href="https://ericmiguel.github.io/missil"><img src="https://github.com/ericmiguel/missil/assets/12076399/c7841626-706e-425f-99d6-c91fd6fb3455" alt="Missil"></a>
+  <a href="https://ericmiguel.github.io/missil"><img src="https://github.com/ericmiguel/missil/assets/12076399/dfe4a649-a226-42b4-851d-698fbb664bc7" alt="Missil"></a>
 </p>
 <p align="center">
     <em>Simple <a href="https://fastapi.tiangolo.com/">FastAPI</a> declarative endpoint-level access control, somewhat inspired by <a href="https://docs.pylonsproject.org/projects/pyramid/en/latest/narr/security.html">Pyramid</a>.</em>
 </p>
 <p align="center">
     <span><a href="https://ericmiguel.github.io/missil/" target="_blank">[DOCS]</a></span>
     <span><a href="https://github.com/ericmiguel/missil" target="_blank">[SOURCE]</a></span>
```

