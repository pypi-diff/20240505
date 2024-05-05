# Comparing `tmp/fastapi_openid_google-0.0.1.dev1.tar.gz` & `tmp/fastapi_openid_google-0.0.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_openid_google-0.0.1.dev1.tar", last modified: Sun Mar 24 18:00:31 2024, max compression
+gzip compressed data, was "fastapi_openid_google-0.0.1.dev2.tar", max compression
```

## Comparing `fastapi_openid_google-0.0.1.dev1.tar` & `fastapi_openid_google-0.0.1.dev2.tar`

### file list

```diff
@@ -1,19 +1,5 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:00:31.112517 fastapi_openid_google-0.0.1.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-24 18:00:22.000000 fastapi_openid_google-0.0.1.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-24 18:00:22.000000 fastapi_openid_google-0.0.1.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-24 18:00:31.112517 fastapi_openid_google-0.0.1.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-03-24 18:00:22.000000 fastapi_openid_google-0.0.1.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-24 18:00:22.000000 fastapi_openid_google-0.0.1.dev1/USAGE.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-24 18:00:22.000000 fastapi_openid_google-0.0.1.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 18:00:31.112517 fastapi_openid_google-0.0.1.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-03-24 18:00:22.000000 fastapi_openid_google-0.0.1.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:00:31.108518 fastapi_openid_google-0.0.1.dev1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:00:31.108518 fastapi_openid_google-0.0.1.dev1/src/fastapi_openid_google/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-24 18:00:22.000000 fastapi_openid_google-0.0.1.dev1/src/fastapi_openid_google/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)    10334 2024-03-24 18:00:22.000000 fastapi_openid_google-0.0.1.dev1/src/fastapi_openid_google/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:00:31.108518 fastapi_openid_google-0.0.1.dev1/src/fastapi_openid_google.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-24 18:00:31.000000 fastapi_openid_google-0.0.1.dev1/src/fastapi_openid_google.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-24 18:00:31.000000 fastapi_openid_google-0.0.1.dev1/src/fastapi_openid_google.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 18:00:31.000000 fastapi_openid_google-0.0.1.dev1/src/fastapi_openid_google.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-24 18:00:31.000000 fastapi_openid_google-0.0.1.dev1/src/fastapi_openid_google.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-24 18:00:31.000000 fastapi_openid_google-0.0.1.dev1/src/fastapi_openid_google.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1073 2024-05-05 16:10:18.851624 fastapi_openid_google-0.0.1.dev2/LICENSE
+-rw-r--r--   0        0        0      436 2024-05-05 16:10:18.851624 fastapi_openid_google-0.0.1.dev2/README.md
+-rw-r--r--   0        0        0      682 2024-05-05 16:10:18.851624 fastapi_openid_google-0.0.1.dev2/pyproject.toml
+-rw-r--r--   0        0        0    10334 2024-05-05 16:10:18.855624 fastapi_openid_google-0.0.1.dev2/src/fastapi_openid_google/__init__.py
+-rw-r--r--   0        0        0     1365 1970-01-01 00:00:00.000000 fastapi_openid_google-0.0.1.dev2/PKG-INFO
```

### Comparing `fastapi_openid_google-0.0.1.dev1/LICENSE` & `fastapi_openid_google-0.0.1.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_openid_google-0.0.1.dev1/PKG-INFO` & `fastapi_openid_google-0.0.1.dev2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
-Name: fastapi_openid_google
-Version: 0.0.1.dev1
+Name: fastapi-openid-google
+Version: 0.0.1.dev2
 Summary: Google OpenID integration for FastAPI
-Home-page: https://github.com/svaponi/fastapi_openid_google
+Home-page: https://svaponi.github.io/fastapi_openid_google
+License: MIT
 Author: svaponi
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
+Author-email: 10941963+svaponi@users.noreply.github.com
+Requires-Python: >=3.8,<3.13
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: fastapi (>=0.111.0,<0.112.0)
+Requires-Dist: oauthlib (>=3.2.2,<4.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Project-URL: Repository, https://github.com/svaponi/fastapi_openid_google
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: fastapi
-Requires-Dist: oauthlib
-Requires-Dist: requests
-Provides-Extra: local
-Requires-Dist: uvicorn; extra == "local"
-Requires-Dist: python-dotenv; extra == "local"
 
 # fastapi-openid-google
 
 Google OpenID integration for FastAPI.
 
 ## Usage
 
@@ -41,7 +44,8 @@
         return {
             "current_user": request.state.user,
             "logout": f"/logout",
         }
     else:
         return {"login": f"/login"}
 ```
+
```

### Comparing `fastapi_openid_google-0.0.1.dev1/src/fastapi_openid_google/__init__.py` & `fastapi_openid_google-0.0.1.dev2/src/fastapi_openid_google/__init__.py`

 * *Files identical despite different names*

