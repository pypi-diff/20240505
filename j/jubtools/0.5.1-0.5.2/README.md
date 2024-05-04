# Comparing `tmp/jubtools-0.5.1.tar.gz` & `tmp/jubtools-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jubtools-0.5.1.tar", last modified: Sat May  4 20:08:27 2024, max compression
+gzip compressed data, was "jubtools-0.5.2.tar", last modified: Sat May  4 21:28:35 2024, max compression
```

## Comparing `jubtools-0.5.1.tar` & `jubtools-0.5.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-04 20:08:27.876503 jubtools-0.5.1/
--rw-r--r--   0 andy       (501) staff       (20)    35149 2023-11-25 11:26:03.000000 jubtools-0.5.1/LICENSE
--rw-r--r--   0 andy       (501) staff       (20)    41184 2024-05-04 20:08:27.876292 jubtools-0.5.1/PKG-INFO
--rw-r--r--   0 andy       (501) staff       (20)      183 2024-05-03 12:01:13.000000 jubtools-0.5.1/README.md
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-04 20:08:27.874666 jubtools-0.5.1/jubtools/
--rw-r--r--   0 andy       (501) staff       (20)        0 2023-11-25 11:26:03.000000 jubtools-0.5.1/jubtools/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)     1695 2024-05-04 19:58:54.000000 jubtools-0.5.1/jubtools/config.py
--rw-r--r--   0 andy       (501) staff       (20)     1295 2024-05-04 19:57:40.000000 jubtools-0.5.1/jubtools/httptools.py
--rw-r--r--   0 andy       (501) staff       (20)      370 2024-05-03 13:10:41.000000 jubtools-0.5.1/jubtools/misctools.py
--rw-r--r--   0 andy       (501) staff       (20)     4861 2024-05-04 20:07:22.000000 jubtools-0.5.1/jubtools/psql.py
--rw-r--r--   0 andy       (501) staff       (20)        0 2024-05-01 16:00:18.000000 jubtools-0.5.1/jubtools/py.typed
--rw-r--r--   0 andy       (501) staff       (20)     1143 2024-05-03 11:07:09.000000 jubtools-0.5.1/jubtools/sqlt.py
--rw-r--r--   0 andy       (501) staff       (20)     3757 2024-05-03 13:08:52.000000 jubtools-0.5.1/jubtools/systemtools.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-04 20:08:27.875823 jubtools-0.5.1/jubtools.egg-info/
--rw-r--r--   0 andy       (501) staff       (20)    41184 2024-05-04 20:08:27.000000 jubtools-0.5.1/jubtools.egg-info/PKG-INFO
--rw-r--r--   0 andy       (501) staff       (20)      422 2024-05-04 20:08:27.000000 jubtools-0.5.1/jubtools.egg-info/SOURCES.txt
--rw-r--r--   0 andy       (501) staff       (20)        1 2024-05-04 20:08:27.000000 jubtools-0.5.1/jubtools.egg-info/dependency_links.txt
--rw-r--r--   0 andy       (501) staff       (20)       64 2024-05-04 20:08:27.000000 jubtools-0.5.1/jubtools.egg-info/requires.txt
--rw-r--r--   0 andy       (501) staff       (20)        9 2024-05-04 20:08:27.000000 jubtools-0.5.1/jubtools.egg-info/top_level.txt
--rw-r--r--   0 andy       (501) staff       (20)      598 2024-05-04 20:07:28.000000 jubtools-0.5.1/pyproject.toml
--rw-r--r--   0 andy       (501) staff       (20)       38 2024-05-04 20:08:27.876556 jubtools-0.5.1/setup.cfg
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-04 20:08:27.875651 jubtools-0.5.1/tests/
--rw-r--r--   0 andy       (501) staff       (20)     1214 2024-05-01 16:00:18.000000 jubtools-0.5.1/tests/test_config.py
--rw-r--r--   0 andy       (501) staff       (20)      260 2024-05-03 13:16:29.000000 jubtools-0.5.1/tests/test_misctools.py
--rw-r--r--   0 andy       (501) staff       (20)      352 2024-05-03 13:31:23.000000 jubtools-0.5.1/tests/test_systemtools.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-04 21:28:35.980802 jubtools-0.5.2/
+-rw-r--r--   0 andy       (501) staff       (20)    35149 2023-11-25 11:26:03.000000 jubtools-0.5.2/LICENSE
+-rw-r--r--   0 andy       (501) staff       (20)    41184 2024-05-04 21:28:35.980578 jubtools-0.5.2/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)      183 2024-05-03 12:01:13.000000 jubtools-0.5.2/README.md
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-04 21:28:35.978510 jubtools-0.5.2/jubtools/
+-rw-r--r--   0 andy       (501) staff       (20)        0 2023-11-25 11:26:03.000000 jubtools-0.5.2/jubtools/__init__.py
+-rw-r--r--   0 andy       (501) staff       (20)     1695 2024-05-04 19:58:54.000000 jubtools-0.5.2/jubtools/config.py
+-rw-r--r--   0 andy       (501) staff       (20)     1295 2024-05-04 19:57:40.000000 jubtools-0.5.2/jubtools/httptools.py
+-rw-r--r--   0 andy       (501) staff       (20)      370 2024-05-03 13:10:41.000000 jubtools-0.5.2/jubtools/misctools.py
+-rw-r--r--   0 andy       (501) staff       (20)     4861 2024-05-04 20:07:22.000000 jubtools-0.5.2/jubtools/psql.py
+-rw-r--r--   0 andy       (501) staff       (20)        0 2024-05-01 16:00:18.000000 jubtools-0.5.2/jubtools/py.typed
+-rw-r--r--   0 andy       (501) staff       (20)     1143 2024-05-03 11:07:09.000000 jubtools-0.5.2/jubtools/sqlt.py
+-rw-r--r--   0 andy       (501) staff       (20)     3854 2024-05-04 21:26:55.000000 jubtools-0.5.2/jubtools/systemtools.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-04 21:28:35.980140 jubtools-0.5.2/jubtools.egg-info/
+-rw-r--r--   0 andy       (501) staff       (20)    41184 2024-05-04 21:28:35.000000 jubtools-0.5.2/jubtools.egg-info/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)      422 2024-05-04 21:28:35.000000 jubtools-0.5.2/jubtools.egg-info/SOURCES.txt
+-rw-r--r--   0 andy       (501) staff       (20)        1 2024-05-04 21:28:35.000000 jubtools-0.5.2/jubtools.egg-info/dependency_links.txt
+-rw-r--r--   0 andy       (501) staff       (20)       64 2024-05-04 21:28:35.000000 jubtools-0.5.2/jubtools.egg-info/requires.txt
+-rw-r--r--   0 andy       (501) staff       (20)        9 2024-05-04 21:28:35.000000 jubtools-0.5.2/jubtools.egg-info/top_level.txt
+-rw-r--r--   0 andy       (501) staff       (20)      598 2024-05-04 21:27:41.000000 jubtools-0.5.2/pyproject.toml
+-rw-r--r--   0 andy       (501) staff       (20)       38 2024-05-04 21:28:35.980847 jubtools-0.5.2/setup.cfg
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-04 21:28:35.979877 jubtools-0.5.2/tests/
+-rw-r--r--   0 andy       (501) staff       (20)     1214 2024-05-01 16:00:18.000000 jubtools-0.5.2/tests/test_config.py
+-rw-r--r--   0 andy       (501) staff       (20)      260 2024-05-03 13:16:29.000000 jubtools-0.5.2/tests/test_misctools.py
+-rw-r--r--   0 andy       (501) staff       (20)      352 2024-05-03 13:31:23.000000 jubtools-0.5.2/tests/test_systemtools.py
```

### Comparing `jubtools-0.5.1/LICENSE` & `jubtools-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jubtools-0.5.1/PKG-INFO` & `jubtools-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jubtools
-Version: 0.5.1
+Version: 0.5.2
 Summary: Shared tools for my own work
 Author-email: Andrew Morcom <jubulani@fastmail.fm>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `jubtools-0.5.1/jubtools/config.py` & `jubtools-0.5.2/jubtools/config.py`

 * *Files identical despite different names*

### Comparing `jubtools-0.5.1/jubtools/httptools.py` & `jubtools-0.5.2/jubtools/httptools.py`

 * *Files identical despite different names*

### Comparing `jubtools-0.5.1/jubtools/psql.py` & `jubtools-0.5.2/jubtools/psql.py`

 * *Files identical despite different names*

### Comparing `jubtools-0.5.1/jubtools/sqlt.py` & `jubtools-0.5.2/jubtools/sqlt.py`

 * *Files identical despite different names*

### Comparing `jubtools-0.5.1/jubtools/systemtools.py` & `jubtools-0.5.2/jubtools/systemtools.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,19 @@
     global APP_ENV
     global APP_VERSION
     global APP_START_TIME
 
     APP_ENV = env
     APP_VERSION = version
 
-    fastapi_args: dict[str, Any] = {"title": config.get("app_name")}
+    fastapi_args: dict[str, Any] = {
+        "title": config.get("app_name"),
+        "version": version,
+        "root_path": config.get("fastapi.root_path"),
+    }
     if config.get("fastapi.disable_docs"):
         fastapi_args["openapi_url"] = None
     app = FastAPI(**fastapi_args)
 
     APP_START_TIME = dt.datetime.now()
     app.add_api_route("/health", health_handler, methods=["GET"])
```

### Comparing `jubtools-0.5.1/jubtools.egg-info/PKG-INFO` & `jubtools-0.5.2/jubtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jubtools
-Version: 0.5.1
+Version: 0.5.2
 Summary: Shared tools for my own work
 Author-email: Andrew Morcom <jubulani@fastmail.fm>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `jubtools-0.5.1/pyproject.toml` & `jubtools-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "jubtools"
 description = "Shared tools for my own work"
 readme = "README.md"
 license = { file = "LICENSE" }
-version = "0.5.1"
+version = "0.5.2"
 authors = [{ name = "Andrew Morcom", email = "jubulani@fastmail.fm" }]
 requires-python = ">=3.10"
 dependencies = ["fastapi"]
 
 [project.optional-dependencies]
 test = [
     "async_asgi_testclient >= 1.4",
```

### Comparing `jubtools-0.5.1/tests/test_config.py` & `jubtools-0.5.2/tests/test_config.py`

 * *Files identical despite different names*

