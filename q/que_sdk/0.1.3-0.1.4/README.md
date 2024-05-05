# Comparing `tmp/que_sdk-0.1.3.tar.gz` & `tmp/que_sdk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "que_sdk-0.1.3.tar", max compression
+gzip compressed data, was "que_sdk-0.1.4.tar", max compression
```

## Comparing `que_sdk-0.1.3.tar` & `que_sdk-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1060 2024-04-12 14:53:33.472804 que_sdk-0.1.3/LICENSE
--rw-r--r--   0        0        0       10 2024-04-19 17:17:10.806057 que_sdk-0.1.3/README.md
--rw-r--r--   0        0        0     1130 2024-04-27 21:02:31.215152 que_sdk-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      435 2024-04-20 08:19:42.640114 que_sdk-0.1.3/que_sdk/__init__.py
--rw-r--r--   0        0        0       65 2024-04-18 19:15:55.848369 que_sdk-0.1.3/que_sdk/_internal/__init__.py
--rw-r--r--   0        0        0      367 2024-04-13 18:33:05.063314 que_sdk-0.1.3/que_sdk/_internal/auth.py
--rw-r--r--   0        0        0     2257 2024-04-19 18:42:30.920224 que_sdk-0.1.3/que_sdk/_internal/base.py
--rw-r--r--   0        0        0     6339 2024-04-20 08:19:42.654293 que_sdk-0.1.3/que_sdk/client.py
--rw-r--r--   0        0        0     5575 2024-04-27 21:02:10.142041 que_sdk-0.1.3/que_sdk/clients.py
--rw-r--r--   0        0        0        0 2024-04-12 19:15:10.383938 que_sdk-0.1.3/que_sdk/py.typed.py
--rw-r--r--   0        0        0     1008 2024-04-23 08:59:04.018042 que_sdk-0.1.3/que_sdk/schemas.py
--rw-r--r--   0        0        0      329 2024-04-19 17:19:02.229326 que_sdk-0.1.3/que_sdk/types.py
--rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 que_sdk-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-04-12 14:53:33.472804 que_sdk-0.1.4/LICENSE
+-rw-r--r--   0        0        0       10 2024-04-19 17:17:10.806057 que_sdk-0.1.4/README.md
+-rw-r--r--   0        0        0     1130 2024-05-05 18:07:10.930563 que_sdk-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      435 2024-04-20 08:19:42.640114 que_sdk-0.1.4/que_sdk/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-18 19:15:55.848369 que_sdk-0.1.4/que_sdk/_internal/__init__.py
+-rw-r--r--   0        0        0      367 2024-04-13 18:33:05.063314 que_sdk-0.1.4/que_sdk/_internal/auth.py
+-rw-r--r--   0        0        0     2255 2024-05-05 18:05:55.876531 que_sdk-0.1.4/que_sdk/_internal/base.py
+-rw-r--r--   0        0        0     6339 2024-04-20 08:19:42.654293 que_sdk-0.1.4/que_sdk/client.py
+-rw-r--r--   0        0        0     5575 2024-04-27 21:02:10.142041 que_sdk-0.1.4/que_sdk/clients.py
+-rw-r--r--   0        0        0        0 2024-04-12 19:15:10.383938 que_sdk-0.1.4/que_sdk/py.typed.py
+-rw-r--r--   0        0        0     1008 2024-04-23 08:59:04.018042 que_sdk-0.1.4/que_sdk/schemas.py
+-rw-r--r--   0        0        0      329 2024-04-19 17:19:02.229326 que_sdk-0.1.4/que_sdk/types.py
+-rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 que_sdk-0.1.4/PKG-INFO
```

### Comparing `que_sdk-0.1.3/LICENSE` & `que_sdk-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `que_sdk-0.1.3/pyproject.toml` & `que_sdk-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "que_sdk"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["DavidRomanovizc"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `que_sdk-0.1.3/que_sdk/_internal/base.py` & `que_sdk-0.1.4/que_sdk/_internal/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 )
 
 __all__ = ("BaseClient",)
 
 
 class BaseClient:
     def __init__(self) -> None:
-        self._base_url = "http://127.0.0.1:8080/api/v1"
+        self._base_url = "http://0.0.0.0:8080/api/v1"
         self.log = logging.getLogger(self.__class__.__name__)
 
     @backoff.on_exception(
         backoff.expo,
         httpx.ConnectError,
         max_time=60,
     )
```

### Comparing `que_sdk-0.1.3/que_sdk/client.py` & `que_sdk-0.1.4/que_sdk/client.py`

 * *Files identical despite different names*

### Comparing `que_sdk-0.1.3/que_sdk/clients.py` & `que_sdk-0.1.4/que_sdk/clients.py`

 * *Files identical despite different names*

### Comparing `que_sdk-0.1.3/que_sdk/schemas.py` & `que_sdk-0.1.4/que_sdk/schemas.py`

 * *Files identical despite different names*

