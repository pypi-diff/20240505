# Comparing `tmp/stigg_sidecar_sdk-1.58.3.tar.gz` & `tmp/stigg_sidecar_sdk-1.98.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_sidecar_sdk-1.58.3.tar", max compression
+gzip compressed data, was "stigg_sidecar_sdk-1.98.3.tar", max compression
```

## Comparing `stigg_sidecar_sdk-1.58.3.tar` & `stigg_sidecar_sdk-1.98.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     5127 2024-03-06 19:48:41.589942 stigg_sidecar_sdk-1.58.3/LICENSE
--rw-r--r--   0        0        0     1924 2024-03-06 19:48:41.589942 stigg_sidecar_sdk-1.58.3/README.md
--rw-r--r--   0        0        0      807 2024-03-06 19:49:21.498450 stigg_sidecar_sdk-1.58.3/pyproject.toml
--rw-r--r--   0        0        0       99 2024-03-06 19:48:41.589942 stigg_sidecar_sdk-1.58.3/stigg_sidecar_sdk/__init__.py
--rw-r--r--   0        0        0     1834 2024-03-06 19:49:18.506415 stigg_sidecar_sdk-1.58.3/stigg_sidecar_sdk/certs/root-ca.pem
--rw-r--r--   0        0        0        0 2024-03-06 19:49:19.926431 stigg_sidecar_sdk-1.58.3/stigg_sidecar_sdk/generated/__init__.py
--rw-r--r--   0        0        0        0 2024-03-06 19:49:19.926431 stigg_sidecar_sdk-1.58.3/stigg_sidecar_sdk/generated/stigg/__init__.py
--rw-r--r--   0        0        0        0 2024-03-06 19:49:19.926431 stigg_sidecar_sdk-1.58.3/stigg_sidecar_sdk/generated/stigg/sidecar/__init__.py
--rw-r--r--   0        0        0    22816 2024-03-06 19:49:19.926431 stigg_sidecar_sdk-1.58.3/stigg_sidecar_sdk/generated/stigg/sidecar/v1/__init__.py
--rw-r--r--   0        0        0     5625 2024-03-06 19:48:41.589942 stigg_sidecar_sdk-1.58.3/stigg_sidecar_sdk/sdk.py
--rw-r--r--   0        0        0     2556 1970-01-01 00:00:00.000000 stigg_sidecar_sdk-1.58.3/PKG-INFO
+-rw-r--r--   0        0        0     5127 2024-04-01 07:58:37.564435 stigg_sidecar_sdk-1.98.3/LICENSE
+-rw-r--r--   0        0        0     1924 2024-04-01 07:58:37.564435 stigg_sidecar_sdk-1.98.3/README.md
+-rw-r--r--   0        0        0      760 2024-04-01 07:59:15.624458 stigg_sidecar_sdk-1.98.3/pyproject.toml
+-rw-r--r--   0        0        0       99 2024-04-01 07:58:37.564435 stigg_sidecar_sdk-1.98.3/stigg_sidecar_sdk/__init__.py
+-rw-r--r--   0        0        0     1834 2024-04-01 07:59:13.204457 stigg_sidecar_sdk-1.98.3/stigg_sidecar_sdk/certs/root-ca.pem
+-rw-r--r--   0        0        0        0 2024-04-01 07:59:14.276458 stigg_sidecar_sdk-1.98.3/stigg_sidecar_sdk/generated/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 07:59:14.276458 stigg_sidecar_sdk-1.98.3/stigg_sidecar_sdk/generated/stigg/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 07:59:14.276458 stigg_sidecar_sdk-1.98.3/stigg_sidecar_sdk/generated/stigg/sidecar/__init__.py
+-rw-r--r--   0        0        0    22816 2024-04-01 07:59:14.276458 stigg_sidecar_sdk-1.98.3/stigg_sidecar_sdk/generated/stigg/sidecar/v1/__init__.py
+-rw-r--r--   0        0        0     5625 2024-04-01 07:58:37.564435 stigg_sidecar_sdk-1.98.3/stigg_sidecar_sdk/sdk.py
+-rw-r--r--   0        0        0     2521 1970-01-01 00:00:00.000000 stigg_sidecar_sdk-1.98.3/PKG-INFO
```

### Comparing `stigg_sidecar_sdk-1.58.3/LICENSE` & `stigg_sidecar_sdk-1.98.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stigg_sidecar_sdk-1.58.3/README.md` & `stigg_sidecar_sdk-1.98.3/README.md`

 * *Files identical despite different names*

### Comparing `stigg_sidecar_sdk-1.58.3/pyproject.toml` & `stigg_sidecar_sdk-1.98.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stigg-sidecar-sdk"
-version = "1.58.3"
+version = "1.98.3"
 description = ""
 authors = ["Stigg <support@stigg.io>"]
 readme = "README.md"
 packages = [
     { include = "stigg_sidecar_sdk" },
 ]
 include = [
@@ -12,23 +12,21 @@
     "stigg_sidecar_sdk/generated/**/*",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 tenacity = "^8.2.2"
 httpx = "0.24.1"
-pydantic = "1.10.8"
 betterproto = { extras = ["compiler"], version = "^2.0.0b6", allow-prereleases = true }
 grpcio-tools = "^1.59.0"
 stigg-api-client-v2 = "*"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^5.0"
 black = "^22.8"
-ariadne-codegen = "^0.7.0"
 pytest = "^7.4.3"
 pytest-asyncio = "^0.21.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `stigg_sidecar_sdk-1.58.3/stigg_sidecar_sdk/certs/root-ca.pem` & `stigg_sidecar_sdk-1.98.3/stigg_sidecar_sdk/certs/root-ca.pem`

 * *Files identical despite different names*

### Comparing `stigg_sidecar_sdk-1.58.3/stigg_sidecar_sdk/generated/stigg/sidecar/v1/__init__.py` & `stigg_sidecar_sdk-1.98.3/stigg_sidecar_sdk/generated/stigg/sidecar/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `stigg_sidecar_sdk-1.58.3/stigg_sidecar_sdk/sdk.py` & `stigg_sidecar_sdk-1.98.3/stigg_sidecar_sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `stigg_sidecar_sdk-1.58.3/PKG-INFO` & `stigg_sidecar_sdk-1.98.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: stigg-sidecar-sdk
-Version: 1.58.3
+Version: 1.98.3
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: betterproto[compiler] (>=2.0.0b6,<3.0.0)
 Requires-Dist: grpcio-tools (>=1.59.0,<2.0.0)
 Requires-Dist: httpx (==0.24.1)
-Requires-Dist: pydantic (==1.10.8)
 Requires-Dist: stigg-api-client-v2
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Description-Content-Type: text/markdown
 
 # stigg-sidecar-sdk 
 
 Stigg Python SDK makes it easier to interact with Stigg Sidecar
```

