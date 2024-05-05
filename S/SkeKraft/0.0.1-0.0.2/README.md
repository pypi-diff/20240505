# Comparing `tmp/skekraft-0.0.1.tar.gz` & `tmp/skekraft-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skekraft-0.0.1.tar", last modified: Wed May  1 20:25:03 2024, max compression
+gzip compressed data, was "skekraft-0.0.2.tar", last modified: Sun May  5 06:32:58 2024, max compression
```

## Comparing `skekraft-0.0.1.tar` & `skekraft-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,17 @@
-drwxr-xr-x   0 veulsan  (2037719458) 1135428931        0 2024-05-01 20:25:03.866979 skekraft-0.0.1/
--rw-r--r--   0 veulsan  (2037719458) 1135428931    35149 2024-05-01 07:22:39.000000 skekraft-0.0.1/LICENSE
--rw-r--r--   0 veulsan  (2037719458) 1135428931     1926 2024-05-01 20:25:03.866718 skekraft-0.0.1/PKG-INFO
--rw-r--r--   0 veulsan  (2037719458) 1135428931     1354 2024-05-01 07:46:21.000000 skekraft-0.0.1/README.md
--rw-r--r--   0 veulsan  (2037719458) 1135428931       87 2024-05-01 20:22:09.000000 skekraft-0.0.1/pyproject.toml
--rw-r--r--   0 veulsan  (2037719458) 1135428931      699 2024-05-01 20:25:03.870554 skekraft-0.0.1/setup.cfg
-drwxr-xr-x   0 veulsan  (2037719458) 1135428931        0 2024-05-01 20:25:03.850869 skekraft-0.0.1/src/
-drwxr-xr-x   0 veulsan  (2037719458) 1135428931        0 2024-05-01 20:25:03.866286 skekraft-0.0.1/src/SkeKraft.egg-info/
--rw-r--r--   0 veulsan  (2037719458) 1135428931     1926 2024-05-01 20:25:03.000000 skekraft-0.0.1/src/SkeKraft.egg-info/PKG-INFO
--rw-r--r--   0 veulsan  (2037719458) 1135428931      186 2024-05-01 20:25:03.000000 skekraft-0.0.1/src/SkeKraft.egg-info/SOURCES.txt
--rw-r--r--   0 veulsan  (2037719458) 1135428931        1 2024-05-01 20:25:03.000000 skekraft-0.0.1/src/SkeKraft.egg-info/dependency_links.txt
--rw-r--r--   0 veulsan  (2037719458) 1135428931        1 2024-05-01 20:25:03.000000 skekraft-0.0.1/src/SkeKraft.egg-info/top_level.txt
+drwxr-xr-x   0 veulsan  (2037719458) 1135428931        0 2024-05-05 06:32:58.577843 skekraft-0.0.2/
+-rw-r--r--   0 veulsan  (2037719458) 1135428931    35149 2024-05-01 07:22:39.000000 skekraft-0.0.2/LICENSE.txt
+-rw-r--r--   0 veulsan  (2037719458) 1135428931    37046 2024-05-05 06:32:58.577529 skekraft-0.0.2/PKG-INFO
+-rw-r--r--   0 veulsan  (2037719458) 1135428931     1320 2024-05-05 06:27:42.000000 skekraft-0.0.2/README.md
+-rw-r--r--   0 veulsan  (2037719458) 1135428931       87 2024-05-01 20:22:09.000000 skekraft-0.0.2/pyproject.toml
+-rw-r--r--   0 veulsan  (2037719458) 1135428931      699 2024-05-05 06:32:58.579230 skekraft-0.0.2/setup.cfg
+drwxr-xr-x   0 veulsan  (2037719458) 1135428931        0 2024-05-05 06:32:58.556716 skekraft-0.0.2/src/
+drwxr-xr-x   0 veulsan  (2037719458) 1135428931        0 2024-05-05 06:32:58.577095 skekraft-0.0.2/src/SkeKraft.egg-info/
+-rw-r--r--   0 veulsan  (2037719458) 1135428931    37046 2024-05-05 06:32:58.000000 skekraft-0.0.2/src/SkeKraft.egg-info/PKG-INFO
+-rw-r--r--   0 veulsan  (2037719458) 1135428931      428 2024-05-05 06:32:58.000000 skekraft-0.0.2/src/SkeKraft.egg-info/SOURCES.txt
+-rw-r--r--   0 veulsan  (2037719458) 1135428931        1 2024-05-05 06:32:58.000000 skekraft-0.0.2/src/SkeKraft.egg-info/dependency_links.txt
+-rw-r--r--   0 veulsan  (2037719458) 1135428931        9 2024-05-05 06:32:58.000000 skekraft-0.0.2/src/SkeKraft.egg-info/top_level.txt
+drwxr-xr-x   0 veulsan  (2037719458) 1135428931        0 2024-05-05 06:32:58.570107 skekraft-0.0.2/src/skekraft/
+-rw-r--r--   0 veulsan  (2037719458) 1135428931     5097 2024-05-05 06:29:37.000000 skekraft-0.0.2/src/skekraft/HttpClient.py
+-rw-r--r--   0 veulsan  (2037719458) 1135428931       83 2024-05-05 06:26:53.000000 skekraft-0.0.2/src/skekraft/__init__.py
+-rw-r--r--   0 veulsan  (2037719458) 1135428931     4509 2024-05-05 06:29:46.000000 skekraft-0.0.2/src/skekraft/api.py
+-rw-r--r--   0 veulsan  (2037719458) 1135428931     1273 2024-05-05 06:25:49.000000 skekraft-0.0.2/src/skekraft/const.py
```

### Comparing `skekraft-0.0.1/LICENSE` & `skekraft-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `skekraft-0.0.1/README.md` & `skekraft-0.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Skellefteå Kraft API
 This is a simple API for Skellefteå Kraft and requires username & password as a login method
 .
 If you do not have it you can go to mina sidor, https://minasidor.skekraft.se/login, login with bankid and create one by going to **Mitt Konto** and then **Inloggning**.
 
 ### Examples
 Simple example on how to login with username & password:
+
 ```python
-from external.skekraft.api import SkekraftAPI
+from api import SkekraftAPI
 import asyncio
 
 base_url = "https://externalapi.skekraft.se/api/MySkekraft"
 skekraft_api = SkekraftAPI(base_url)
 login_response = await skekraft_api.login("username", "password")
 if login_response is not None and int(login_response['ErrNumber']) == 1:
     print(f"Login successful. Token: {login_response['Dst']}")
@@ -19,16 +20,17 @@
     await skekraft_api.logout()
     exit(-1)
         login_response = await skekraft_api.login("username", "password")
 
 ```
 
 You can also use a token if you have one. Do remember to refresh it regurlary do not invalide it:
+
 ```python
-from external.skekraft.api import SkekraftAPI
+from api import SkekraftAPI
 import asyncio
 
 base_url = "https://externalapi.skekraft.se/api/MySkekraft"
 skekraft_api = SkekraftAPI(base_url)
 token = "your-token-here"
 token = await skekraft_api.refresh(token)
 log(f"Response: {token}")
```

### Comparing `skekraft-0.0.1/setup.cfg` & `skekraft-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = SkeKraft
-version = 0.0.1
+version = 0.0.2
 author = Ulrik Sannsell
 author_email = ulrik@sannsell.se
 description = Skellefteå Kraft API package
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://gitlab.com/veulsan/energiinfo
 project_urls =
```

