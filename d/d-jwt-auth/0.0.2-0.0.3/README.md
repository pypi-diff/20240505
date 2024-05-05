# Comparing `tmp/d_jwt_auth-0.0.2.tar.gz` & `tmp/d_jwt_auth-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "d_jwt_auth-0.0.2.tar", last modified: Wed May  1 04:48:23 2024, max compression
+gzip compressed data, was "d_jwt_auth-0.0.3.tar", last modified: Sun May  5 19:55:14 2024, max compression
```

## Comparing `d_jwt_auth-0.0.2.tar` & `d_jwt_auth-0.0.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-05-01 04:48:22.970930 d_jwt_auth-0.0.2/
--rw-rw-r--   0 ali       (1000) ali       (1000)     1069 2024-04-19 07:51:05.000000 d_jwt_auth-0.0.2/LICENSE
--rw-rw-r--   0 ali       (1000) ali       (1000)    11696 2024-05-01 04:48:22.970930 d_jwt_auth-0.0.2/PKG-INFO
--rw-rw-r--   0 ali       (1000) ali       (1000)    10360 2024-05-01 04:36:53.000000 d_jwt_auth-0.0.2/README.md
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-05-01 04:48:22.946929 d_jwt_auth-0.0.2/config/
--rw-rw-r--   0 ali       (1000) ali       (1000)        0 2024-04-19 18:54:17.000000 d_jwt_auth-0.0.2/config/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      389 2024-04-19 18:54:17.000000 d_jwt_auth-0.0.2/config/asgi.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     3465 2024-05-01 04:31:50.000000 d_jwt_auth-0.0.2/config/settings.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      762 2024-04-19 18:54:17.000000 d_jwt_auth-0.0.2/config/urls.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      389 2024-04-19 18:54:17.000000 d_jwt_auth-0.0.2/config/wsgi.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-05-01 04:48:22.950929 d_jwt_auth-0.0.2/d_jwt_auth/
--rw-rw-r--   0 ali       (1000) ali       (1000)        0 2024-04-19 18:34:36.000000 d_jwt_auth-0.0.2/d_jwt_auth/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      144 2024-04-19 03:20:09.000000 d_jwt_auth-0.0.2/d_jwt_auth/admin.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     2024 2024-05-01 02:17:28.000000 d_jwt_auth-0.0.2/d_jwt_auth/app_settings.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      150 2024-04-19 18:21:44.000000 d_jwt_auth-0.0.2/d_jwt_auth/apps.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     1594 2024-04-19 05:10:17.000000 d_jwt_auth-0.0.2/d_jwt_auth/authenticate.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      560 2024-04-18 01:51:55.000000 d_jwt_auth-0.0.2/d_jwt_auth/cache.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      803 2024-04-18 03:51:03.000000 d_jwt_auth-0.0.2/d_jwt_auth/client.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      183 2024-05-01 04:29:12.000000 d_jwt_auth-0.0.2/d_jwt_auth/constants.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     1225 2024-04-18 15:23:34.000000 d_jwt_auth-0.0.2/d_jwt_auth/encryption.py
--rw-rw-r--   0 ali       (1000) ali       (1000)       84 2024-04-18 03:06:06.000000 d_jwt_auth-0.0.2/d_jwt_auth/exceptions.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-05-01 04:48:22.950929 d_jwt_auth-0.0.2/d_jwt_auth/migrations/
--rw-rw-r--   0 ali       (1000) ali       (1000)     1048 2024-05-01 02:45:10.000000 d_jwt_auth-0.0.2/d_jwt_auth/migrations/0001_initial.py
--rw-rw-r--   0 ali       (1000) ali       (1000)        0 2023-11-27 10:37:30.000000 d_jwt_auth-0.0.2/d_jwt_auth/migrations/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      970 2024-05-01 02:29:31.000000 d_jwt_auth-0.0.2/d_jwt_auth/models.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     2919 2024-05-01 04:11:40.000000 d_jwt_auth-0.0.2/d_jwt_auth/services.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     6124 2024-05-01 04:30:10.000000 d_jwt_auth-0.0.2/d_jwt_auth/token.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-05-01 04:48:22.950929 d_jwt_auth-0.0.2/d_jwt_auth.egg-info/
--rw-rw-r--   0 ali       (1000) ali       (1000)    11696 2024-05-01 04:48:22.000000 d_jwt_auth-0.0.2/d_jwt_auth.egg-info/PKG-INFO
--rw-rw-r--   0 ali       (1000) ali       (1000)      835 2024-05-01 04:48:22.000000 d_jwt_auth-0.0.2/d_jwt_auth.egg-info/SOURCES.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)        1 2024-05-01 04:48:22.000000 d_jwt_auth-0.0.2/d_jwt_auth.egg-info/dependency_links.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)        1 2024-05-01 04:48:22.000000 d_jwt_auth-0.0.2/d_jwt_auth.egg-info/not-zip-safe
--rw-rw-r--   0 ali       (1000) ali       (1000)      108 2024-05-01 04:48:22.000000 d_jwt_auth-0.0.2/d_jwt_auth.egg-info/requires.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)       18 2024-05-01 04:48:22.000000 d_jwt_auth-0.0.2/d_jwt_auth.egg-info/top_level.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)       38 2024-05-01 04:48:22.970930 d_jwt_auth-0.0.2/setup.cfg
--rw-rw-r--   0 ali       (1000) ali       (1000)     1854 2024-05-01 04:44:33.000000 d_jwt_auth-0.0.2/setup.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-05-01 04:48:22.970930 d_jwt_auth-0.0.2/tests/
--rw-rw-r--   0 ali       (1000) ali       (1000)     2650 2024-04-19 18:51:44.000000 d_jwt_auth-0.0.2/tests/test_app_settings.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     1239 2024-04-19 18:51:44.000000 d_jwt_auth-0.0.2/tests/test_cache.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     6909 2024-04-19 18:51:44.000000 d_jwt_auth-0.0.2/tests/test_client.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     1439 2024-04-19 18:51:44.000000 d_jwt_auth-0.0.2/tests/test_encryption.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      811 2024-04-19 18:51:44.000000 d_jwt_auth-0.0.2/tests/test_models.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     6823 2024-05-01 02:59:28.000000 d_jwt_auth-0.0.2/tests/test_services.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    12791 2024-05-01 04:30:31.000000 d_jwt_auth-0.0.2/tests/test_token.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-05-05 19:55:14.280539 d_jwt_auth-0.0.3/
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1069 2024-04-19 07:51:05.000000 d_jwt_auth-0.0.3/LICENSE
+-rw-rw-r--   0 ali       (1000) ali       (1000)    11696 2024-05-05 19:55:14.280539 d_jwt_auth-0.0.3/PKG-INFO
+-rw-rw-r--   0 ali       (1000) ali       (1000)    10360 2024-05-01 04:36:53.000000 d_jwt_auth-0.0.3/README.md
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-05-05 19:55:14.096446 d_jwt_auth-0.0.3/config/
+-rw-rw-r--   0 ali       (1000) ali       (1000)        0 2024-04-19 18:54:17.000000 d_jwt_auth-0.0.3/config/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      389 2024-04-19 18:54:17.000000 d_jwt_auth-0.0.3/config/asgi.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     3970 2024-05-05 19:48:37.000000 d_jwt_auth-0.0.3/config/settings.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      762 2024-04-19 18:54:17.000000 d_jwt_auth-0.0.3/config/urls.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      389 2024-04-19 18:54:17.000000 d_jwt_auth-0.0.3/config/wsgi.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-05-05 19:55:14.236517 d_jwt_auth-0.0.3/d_jwt_auth/
+-rw-rw-r--   0 ali       (1000) ali       (1000)        0 2024-04-19 18:34:36.000000 d_jwt_auth-0.0.3/d_jwt_auth/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      144 2024-04-19 03:20:09.000000 d_jwt_auth-0.0.3/d_jwt_auth/admin.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     2024 2024-05-01 02:17:28.000000 d_jwt_auth-0.0.3/d_jwt_auth/app_settings.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      150 2024-04-19 18:21:44.000000 d_jwt_auth-0.0.3/d_jwt_auth/apps.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1594 2024-04-19 05:10:17.000000 d_jwt_auth-0.0.3/d_jwt_auth/authenticate.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      560 2024-04-18 01:51:55.000000 d_jwt_auth-0.0.3/d_jwt_auth/cache.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      803 2024-04-18 03:51:03.000000 d_jwt_auth-0.0.3/d_jwt_auth/client.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      183 2024-05-01 04:29:12.000000 d_jwt_auth-0.0.3/d_jwt_auth/constants.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1225 2024-04-18 15:23:34.000000 d_jwt_auth-0.0.3/d_jwt_auth/encryption.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)       84 2024-04-18 03:06:06.000000 d_jwt_auth-0.0.3/d_jwt_auth/exceptions.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-05-05 19:55:14.252525 d_jwt_auth-0.0.3/d_jwt_auth/migrations/
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1048 2024-05-01 02:45:10.000000 d_jwt_auth-0.0.3/d_jwt_auth/migrations/0001_initial.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)        0 2023-11-27 10:37:30.000000 d_jwt_auth-0.0.3/d_jwt_auth/migrations/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      970 2024-05-01 02:29:31.000000 d_jwt_auth-0.0.3/d_jwt_auth/models.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     2919 2024-05-01 04:11:40.000000 d_jwt_auth-0.0.3/d_jwt_auth/services.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     6423 2024-05-05 19:45:28.000000 d_jwt_auth-0.0.3/d_jwt_auth/token.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-05-05 19:55:14.240519 d_jwt_auth-0.0.3/d_jwt_auth.egg-info/
+-rw-rw-r--   0 ali       (1000) ali       (1000)    11696 2024-05-05 19:55:13.000000 d_jwt_auth-0.0.3/d_jwt_auth.egg-info/PKG-INFO
+-rw-rw-r--   0 ali       (1000) ali       (1000)      835 2024-05-05 19:55:13.000000 d_jwt_auth-0.0.3/d_jwt_auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)        1 2024-05-05 19:55:13.000000 d_jwt_auth-0.0.3/d_jwt_auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)        1 2024-05-05 19:55:13.000000 d_jwt_auth-0.0.3/d_jwt_auth.egg-info/not-zip-safe
+-rw-rw-r--   0 ali       (1000) ali       (1000)       92 2024-05-05 19:55:13.000000 d_jwt_auth-0.0.3/d_jwt_auth.egg-info/requires.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)       18 2024-05-05 19:55:13.000000 d_jwt_auth-0.0.3/d_jwt_auth.egg-info/top_level.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)       38 2024-05-05 19:55:14.280539 d_jwt_auth-0.0.3/setup.cfg
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1835 2024-05-05 19:51:39.000000 d_jwt_auth-0.0.3/setup.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-05-05 19:55:14.280539 d_jwt_auth-0.0.3/tests/
+-rw-rw-r--   0 ali       (1000) ali       (1000)     2650 2024-04-19 18:51:44.000000 d_jwt_auth-0.0.3/tests/test_app_settings.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1239 2024-04-19 18:51:44.000000 d_jwt_auth-0.0.3/tests/test_cache.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     6909 2024-04-19 18:51:44.000000 d_jwt_auth-0.0.3/tests/test_client.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1439 2024-04-19 18:51:44.000000 d_jwt_auth-0.0.3/tests/test_encryption.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      811 2024-04-19 18:51:44.000000 d_jwt_auth-0.0.3/tests/test_models.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     6823 2024-05-01 02:59:28.000000 d_jwt_auth-0.0.3/tests/test_services.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    12791 2024-05-01 04:30:31.000000 d_jwt_auth-0.0.3/tests/test_token.py
```

### Comparing `d_jwt_auth-0.0.2/LICENSE` & `d_jwt_auth-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.2/PKG-INFO` & `d_jwt_auth-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d_jwt_auth
-Version: 0.0.2
+Version: 0.0.3
 Summary: django-jwt-auth is an application for authenticating users with jwt in Django.
 Home-page: https://github.com/alireza-fa/django-jwt-auth
 Author: Alireza Feizi
 Author-email: alirezafeyze44@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/alireza-fa/django-jwt-auth
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `d_jwt_auth-0.0.2/README.md` & `d_jwt_auth-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.2/config/settings.py` & `d_jwt_auth-0.0.3/config/settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 For more information on this file, see
 https://docs.djangoproject.com/en/4.2/topics/settings/
 
 For the full list of settings and their values, see
 https://docs.djangoproject.com/en/4.2/ref/settings/
 """
-
+from datetime import timedelta
 from pathlib import Path
 
 # Build paths inside the project like this: BASE_DIR / 'subdir'.
 BASE_DIR = Path(__file__).resolve().parent.parent
 
 
 # Quick-start development settings - unsuitable for production
@@ -128,7 +128,24 @@
 if JWT_AUTH_CACHE_USING:
     CACHES = {
         "default": {
             "BACKEND": "django.core.cache.backends.redis.RedisCache",
             "LOCATION": "redis://127.0.0.1:6379",
         }
     }
+
+JWT_AUTH_DEVICE_LIMIT = 2
+JWT_AUTH_ENCRYPT_KEY = b'\x87\xd4\xc9\xe4\xb8\x9c\xc9w\x83@j\xbd\xb4\n\xcaq\x85\x9c: \x94\xc5d\x1d\xcc\xeb=c_\xf2\xdde'
+JWT_AUTH_ACCESS_TOKEN_LIFETIME = timedelta(days=7)
+JWT_AUTH_REFRESH_TOKEN_LIFETIME = timedelta(days=30)
+
+JWT_AUTH_ACCESS_TOKEN_CLAIMS = {
+    "username": "",
+    "email": "",
+    "is_superuser": False,
+}
+
+JWT_AUTH_ACCESS_TOKEN_USER_FIELD_CLAIMS = {
+    **JWT_AUTH_ACCESS_TOKEN_CLAIMS
+}
+
+JWT_AUTH_GET_USER_BY_ACCESS_TOKEN = True
```

### Comparing `d_jwt_auth-0.0.2/config/urls.py` & `d_jwt_auth-0.0.3/config/urls.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.2/d_jwt_auth/app_settings.py` & `d_jwt_auth-0.0.3/d_jwt_auth/app_settings.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.2/d_jwt_auth/authenticate.py` & `d_jwt_auth-0.0.3/d_jwt_auth/authenticate.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.2/d_jwt_auth/cache.py` & `d_jwt_auth-0.0.3/d_jwt_auth/cache.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.2/d_jwt_auth/client.py` & `d_jwt_auth-0.0.3/d_jwt_auth/client.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.2/d_jwt_auth/encryption.py` & `d_jwt_auth-0.0.3/d_jwt_auth/encryption.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.2/d_jwt_auth/migrations/0001_initial.py` & `d_jwt_auth-0.0.3/d_jwt_auth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.2/d_jwt_auth/models.py` & `d_jwt_auth-0.0.3/d_jwt_auth/models.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.2/d_jwt_auth/services.py` & `d_jwt_auth-0.0.3/d_jwt_auth/services.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.2/d_jwt_auth/token.py` & `d_jwt_auth-0.0.3/d_jwt_auth/token.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import Dict
+from datetime import datetime
 
 from django.http import HttpRequest
 from rest_framework_simplejwt.tokens import Token, UntypedToken
 from rest_framework_simplejwt.tokens import TokenError as BaseTokenError
 from django.utils.timezone import now
 from django.contrib.auth import get_user_model
+from django.db.models.fields.files import File
 
 from .app_settings import app_setting
 from .constants import ACCESS_TOKEN, REFRESH_TOKEN, UUID_FIELD, USER_ID, TOKEN_TYPE, DEVICE_NAME, IP_ADDRESS
 from .encryption import encrypt, decrypt
 from .exceptions import TokenError
 from .client import get_client_info
 from .services import get_user_auth_uuid, update_user_auth_uuid, get_user_auth
@@ -28,14 +30,20 @@
 
 
 def set_token_claims(*, token: Token, claims: Dict, **kwargs):
     for key in claims:
         claims[key] = kwargs[key]
 
     for key, value in claims.items():
+        if isinstance(value, File):
+            token[key] = value.url
+        elif isinstance(value, File):
+            token[key] = value.url
+        elif isinstance(value, datetime):
+            token[key] = str(value)
         token[key] = value
 
 
 def get_token_claims(*, token: Token, claims: Dict):
     for key in claims:
         claims[key] = token.get(key)
```

### Comparing `d_jwt_auth-0.0.2/d_jwt_auth.egg-info/PKG-INFO` & `d_jwt_auth-0.0.3/d_jwt_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d-jwt-auth
-Version: 0.0.2
+Version: 0.0.3
 Summary: django-jwt-auth is an application for authenticating users with jwt in Django.
 Home-page: https://github.com/alireza-fa/django-jwt-auth
 Author: Alireza Feizi
 Author-email: alirezafeyze44@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/alireza-fa/django-jwt-auth
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `d_jwt_auth-0.0.2/d_jwt_auth.egg-info/SOURCES.txt` & `d_jwt_auth-0.0.3/d_jwt_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.2/setup.py` & `d_jwt_auth-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 def read(f):
     with open(f, 'r', encoding='utf-8') as file:
         return file.read()
 
 
 setup(
     name='d_jwt_auth',
-    version="0.0.2",
+    version="0.0.3",
     url='https://github.com/alireza-fa/django-jwt-auth',
     license='MIT',
     description='django-jwt-auth is an application for authenticating users with jwt in Django.',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     author='Alireza Feizi',
     author_email='alirezafeyze44@gmail.com',
     packages=find_packages(exclude=['tests*']),
     include_package_data=True,
-    install_requires=["django>=3.2", "djangorestframework>=3.0", "djangorestframework-simplejwt>=5.0", "pycryptodome>=3.0", "model-bakery>=1.0"],
+    install_requires=["django>=3.2", "djangorestframework>=3.0", "djangorestframework-simplejwt>=5.3.0", "pycryptodome>=3.0"],
     python_requires=">=3.9",
     zip_safe=False,
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Framework :: Django',
         'Framework :: Django :: 3.2',
```

### Comparing `d_jwt_auth-0.0.2/tests/test_app_settings.py` & `d_jwt_auth-0.0.3/tests/test_app_settings.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.2/tests/test_cache.py` & `d_jwt_auth-0.0.3/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.2/tests/test_client.py` & `d_jwt_auth-0.0.3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.2/tests/test_encryption.py` & `d_jwt_auth-0.0.3/tests/test_encryption.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.2/tests/test_models.py` & `d_jwt_auth-0.0.3/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.2/tests/test_services.py` & `d_jwt_auth-0.0.3/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.2/tests/test_token.py` & `d_jwt_auth-0.0.3/tests/test_token.py`

 * *Files identical despite different names*

