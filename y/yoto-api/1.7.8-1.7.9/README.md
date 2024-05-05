# Comparing `tmp/yoto_api-1.7.8.tar.gz` & `tmp/yoto_api-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yoto_api-1.7.8.tar", last modified: Sat Apr 27 22:44:20 2024, max compression
+gzip compressed data, was "yoto_api-1.7.9.tar", last modified: Sun May  5 21:37:00 2024, max compression
```

## Comparing `yoto_api-1.7.8.tar` & `yoto_api-1.7.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:44:20.890488 yoto_api-1.7.8/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-27 22:43:58.000000 yoto_api-1.7.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-27 22:43:58.000000 yoto_api-1.7.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-27 22:43:58.000000 yoto_api-1.7.8/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-27 22:43:58.000000 yoto_api-1.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-27 22:43:58.000000 yoto_api-1.7.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-27 22:44:20.890488 yoto_api-1.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-27 22:43:58.000000 yoto_api-1.7.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-27 22:43:58.000000 yoto_api-1.7.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 22:44:20.890488 yoto_api-1.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-27 22:44:14.000000 yoto_api-1.7.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:44:20.890488 yoto_api-1.7.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:43:58.000000 yoto_api-1.7.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-27 22:43:58.000000 yoto_api-1.7.8/tests/login_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:44:20.890488 yoto_api-1.7.8/yoto_api/
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-27 22:43:58.000000 yoto_api-1.7.8/yoto_api/Card.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-27 22:43:58.000000 yoto_api-1.7.8/yoto_api/Token.py
--rw-r--r--   0 runner    (1001) docker     (127)    27726 2024-04-27 22:43:58.000000 yoto_api-1.7.8/yoto_api/YotoAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-27 22:43:58.000000 yoto_api-1.7.8/yoto_api/YotoManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-27 22:43:58.000000 yoto_api-1.7.8/yoto_api/YotoPlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-27 22:43:58.000000 yoto_api-1.7.8/yoto_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-27 22:43:58.000000 yoto_api-1.7.8/yoto_api/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:44:20.890488 yoto_api-1.7.8/yoto_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-27 22:44:20.000000 yoto_api-1.7.8/yoto_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-27 22:44:20.000000 yoto_api-1.7.8/yoto_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 22:44:20.000000 yoto_api-1.7.8/yoto_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 22:44:20.000000 yoto_api-1.7.8/yoto_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-27 22:44:20.000000 yoto_api-1.7.8/yoto_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-27 22:44:20.000000 yoto_api-1.7.8/yoto_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:37:00.541927 yoto_api-1.7.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-05 21:36:39.000000 yoto_api-1.7.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-05-05 21:36:39.000000 yoto_api-1.7.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-05 21:36:39.000000 yoto_api-1.7.9/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-05 21:36:39.000000 yoto_api-1.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-05 21:36:39.000000 yoto_api-1.7.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-05 21:37:00.541927 yoto_api-1.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-05 21:36:39.000000 yoto_api-1.7.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-05 21:36:39.000000 yoto_api-1.7.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 21:37:00.541927 yoto_api-1.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-05 21:36:54.000000 yoto_api-1.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:37:00.537927 yoto_api-1.7.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 21:36:39.000000 yoto_api-1.7.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-05 21:36:39.000000 yoto_api-1.7.9/tests/login_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:37:00.537927 yoto_api-1.7.9/yoto_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-05 21:36:39.000000 yoto_api-1.7.9/yoto_api/Card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-05 21:36:39.000000 yoto_api-1.7.9/yoto_api/Token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27730 2024-05-05 21:36:39.000000 yoto_api-1.7.9/yoto_api/YotoAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-05 21:36:39.000000 yoto_api-1.7.9/yoto_api/YotoManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-05 21:36:39.000000 yoto_api-1.7.9/yoto_api/YotoPlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-05 21:36:39.000000 yoto_api-1.7.9/yoto_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-05 21:36:39.000000 yoto_api-1.7.9/yoto_api/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:37:00.541927 yoto_api-1.7.9/yoto_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-05 21:37:00.000000 yoto_api-1.7.9/yoto_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-05 21:37:00.000000 yoto_api-1.7.9/yoto_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 21:37:00.000000 yoto_api-1.7.9/yoto_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 21:37:00.000000 yoto_api-1.7.9/yoto_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-05 21:37:00.000000 yoto_api-1.7.9/yoto_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-05 21:37:00.000000 yoto_api-1.7.9/yoto_api.egg-info/top_level.txt
```

### Comparing `yoto_api-1.7.8/CONTRIBUTING.rst` & `yoto_api-1.7.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.8/LICENSE` & `yoto_api-1.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.8/PKG-INFO` & `yoto_api-1.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.7.8
+Version: 1.7.9
 Summary: A python package that makes it a bit easier to work with the yoto play API. Not associated with Yoto in any way.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `yoto_api-1.7.8/README.rst` & `yoto_api-1.7.9/README.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.8/setup.py` & `yoto_api-1.7.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     include_package_data=True,
     keywords="yoto_api",
     name="yoto_api",
     packages=find_packages(include=["yoto_api", "yoto_api.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/cdnninja/yoto_api",
-    version="1.7.8",
+    version="1.7.9",
     zip_safe=False,
 )
```

### Comparing `yoto_api-1.7.8/yoto_api/Card.py` & `yoto_api-1.7.9/yoto_api/Card.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.8/yoto_api/YotoAPI.py` & `yoto_api-1.7.9/yoto_api/YotoAPI.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,23 +175,23 @@
         payload["audience"] = self.BASE_URL
         payload["client_id"] = self.CLIENT_ID
         payload["grant_type"] = "refresh_token"
         payload["refresh_token"] = token.refresh_token
         payload["scope"] = "openid email profile offline_access"
         headers = {"Content-Type": "application/x-www-form-urlencoded"}
         response = requests.post(url, data=payload, headers=headers).json()
-        _LOGGER.debug(f"{DOMAIN} - Sign In Response {response}")
+        _LOGGER.debug(f"{DOMAIN} - Refresh TokenResponse {response}")
         valid_until = datetime.datetime.now(pytz.utc) + timedelta(
             seconds=response["expires_in"]
         )
         return Token(
             username=token.username,
             password=token.password,
             access_token=response["access_token"],
-            refresh_token=response["id_token"],
+            refresh_token=token.refresh_token,
             token_type=response["token_type"],
             scope=token.scope,
             valid_until=valid_until,
         )
 
     def _get_devices(self, token: Token) -> None:
         url = self.BASE_URL + "/device-v2/devices/mine"
```

### Comparing `yoto_api-1.7.8/yoto_api/YotoManager.py` & `yoto_api-1.7.9/yoto_api/YotoManager.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.8/yoto_api/YotoPlayer.py` & `yoto_api-1.7.9/yoto_api/YotoPlayer.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.8/yoto_api.egg-info/PKG-INFO` & `yoto_api-1.7.9/yoto_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.7.8
+Version: 1.7.9
 Summary: A python package that makes it a bit easier to work with the yoto play API. Not associated with Yoto in any way.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

