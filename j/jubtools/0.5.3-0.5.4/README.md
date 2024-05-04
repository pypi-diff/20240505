# Comparing `tmp/jubtools-0.5.3.tar.gz` & `tmp/jubtools-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jubtools-0.5.3.tar", last modified: Sat May  4 22:02:54 2024, max compression
+gzip compressed data, was "jubtools-0.5.4.tar", last modified: Sat May  4 22:48:06 2024, max compression
```

## Comparing `jubtools-0.5.3.tar` & `jubtools-0.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-04 22:02:54.855430 jubtools-0.5.3/
--rw-r--r--   0 andy       (501) staff       (20)    35149 2023-11-25 11:26:03.000000 jubtools-0.5.3/LICENSE
--rw-r--r--   0 andy       (501) staff       (20)    41184 2024-05-04 22:02:54.855209 jubtools-0.5.3/PKG-INFO
--rw-r--r--   0 andy       (501) staff       (20)      183 2024-05-03 12:01:13.000000 jubtools-0.5.3/README.md
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-04 22:02:54.853305 jubtools-0.5.3/jubtools/
--rw-r--r--   0 andy       (501) staff       (20)        0 2023-11-25 11:26:03.000000 jubtools-0.5.3/jubtools/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)     1695 2024-05-04 19:58:54.000000 jubtools-0.5.3/jubtools/config.py
--rw-r--r--   0 andy       (501) staff       (20)     1295 2024-05-04 19:57:40.000000 jubtools-0.5.3/jubtools/httptools.py
--rw-r--r--   0 andy       (501) staff       (20)      370 2024-05-03 13:10:41.000000 jubtools-0.5.3/jubtools/misctools.py
--rw-r--r--   0 andy       (501) staff       (20)     4861 2024-05-04 20:07:22.000000 jubtools-0.5.3/jubtools/psql.py
--rw-r--r--   0 andy       (501) staff       (20)        0 2024-05-01 16:00:18.000000 jubtools-0.5.3/jubtools/py.typed
--rw-r--r--   0 andy       (501) staff       (20)     1143 2024-05-03 11:07:09.000000 jubtools-0.5.3/jubtools/sqlt.py
--rw-r--r--   0 andy       (501) staff       (20)     3966 2024-05-04 22:01:14.000000 jubtools-0.5.3/jubtools/systemtools.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-04 22:02:54.854781 jubtools-0.5.3/jubtools.egg-info/
--rw-r--r--   0 andy       (501) staff       (20)    41184 2024-05-04 22:02:54.000000 jubtools-0.5.3/jubtools.egg-info/PKG-INFO
--rw-r--r--   0 andy       (501) staff       (20)      422 2024-05-04 22:02:54.000000 jubtools-0.5.3/jubtools.egg-info/SOURCES.txt
--rw-r--r--   0 andy       (501) staff       (20)        1 2024-05-04 22:02:54.000000 jubtools-0.5.3/jubtools.egg-info/dependency_links.txt
--rw-r--r--   0 andy       (501) staff       (20)       64 2024-05-04 22:02:54.000000 jubtools-0.5.3/jubtools.egg-info/requires.txt
--rw-r--r--   0 andy       (501) staff       (20)        9 2024-05-04 22:02:54.000000 jubtools-0.5.3/jubtools.egg-info/top_level.txt
--rw-r--r--   0 andy       (501) staff       (20)      598 2024-05-04 22:01:54.000000 jubtools-0.5.3/pyproject.toml
--rw-r--r--   0 andy       (501) staff       (20)       38 2024-05-04 22:02:54.855489 jubtools-0.5.3/setup.cfg
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-04 22:02:54.854533 jubtools-0.5.3/tests/
--rw-r--r--   0 andy       (501) staff       (20)     1214 2024-05-01 16:00:18.000000 jubtools-0.5.3/tests/test_config.py
--rw-r--r--   0 andy       (501) staff       (20)      260 2024-05-03 13:16:29.000000 jubtools-0.5.3/tests/test_misctools.py
--rw-r--r--   0 andy       (501) staff       (20)      352 2024-05-03 13:31:23.000000 jubtools-0.5.3/tests/test_systemtools.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-04 22:48:06.739797 jubtools-0.5.4/
+-rw-r--r--   0 andy       (501) staff       (20)    35149 2023-11-25 11:26:03.000000 jubtools-0.5.4/LICENSE
+-rw-r--r--   0 andy       (501) staff       (20)    41184 2024-05-04 22:48:06.739567 jubtools-0.5.4/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)      183 2024-05-03 12:01:13.000000 jubtools-0.5.4/README.md
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-04 22:48:06.737942 jubtools-0.5.4/jubtools/
+-rw-r--r--   0 andy       (501) staff       (20)        0 2023-11-25 11:26:03.000000 jubtools-0.5.4/jubtools/__init__.py
+-rw-r--r--   0 andy       (501) staff       (20)     1695 2024-05-04 19:58:54.000000 jubtools-0.5.4/jubtools/config.py
+-rw-r--r--   0 andy       (501) staff       (20)     1295 2024-05-04 19:57:40.000000 jubtools-0.5.4/jubtools/httptools.py
+-rw-r--r--   0 andy       (501) staff       (20)      370 2024-05-03 13:10:41.000000 jubtools-0.5.4/jubtools/misctools.py
+-rw-r--r--   0 andy       (501) staff       (20)     4861 2024-05-04 22:46:34.000000 jubtools-0.5.4/jubtools/psql.py
+-rw-r--r--   0 andy       (501) staff       (20)        0 2024-05-01 16:00:18.000000 jubtools-0.5.4/jubtools/py.typed
+-rw-r--r--   0 andy       (501) staff       (20)     1143 2024-05-03 11:07:09.000000 jubtools-0.5.4/jubtools/sqlt.py
+-rw-r--r--   0 andy       (501) staff       (20)     4018 2024-05-04 22:32:16.000000 jubtools-0.5.4/jubtools/systemtools.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-04 22:48:06.739127 jubtools-0.5.4/jubtools.egg-info/
+-rw-r--r--   0 andy       (501) staff       (20)    41184 2024-05-04 22:48:06.000000 jubtools-0.5.4/jubtools.egg-info/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)      422 2024-05-04 22:48:06.000000 jubtools-0.5.4/jubtools.egg-info/SOURCES.txt
+-rw-r--r--   0 andy       (501) staff       (20)        1 2024-05-04 22:48:06.000000 jubtools-0.5.4/jubtools.egg-info/dependency_links.txt
+-rw-r--r--   0 andy       (501) staff       (20)       64 2024-05-04 22:48:06.000000 jubtools-0.5.4/jubtools.egg-info/requires.txt
+-rw-r--r--   0 andy       (501) staff       (20)        9 2024-05-04 22:48:06.000000 jubtools-0.5.4/jubtools.egg-info/top_level.txt
+-rw-r--r--   0 andy       (501) staff       (20)      597 2024-05-04 22:46:49.000000 jubtools-0.5.4/pyproject.toml
+-rw-r--r--   0 andy       (501) staff       (20)       38 2024-05-04 22:48:06.739850 jubtools-0.5.4/setup.cfg
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-04 22:48:06.738964 jubtools-0.5.4/tests/
+-rw-r--r--   0 andy       (501) staff       (20)     1214 2024-05-01 16:00:18.000000 jubtools-0.5.4/tests/test_config.py
+-rw-r--r--   0 andy       (501) staff       (20)      260 2024-05-03 13:16:29.000000 jubtools-0.5.4/tests/test_misctools.py
+-rw-r--r--   0 andy       (501) staff       (20)      352 2024-05-03 13:31:23.000000 jubtools-0.5.4/tests/test_systemtools.py
```

### Comparing `jubtools-0.5.3/LICENSE` & `jubtools-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jubtools-0.5.3/PKG-INFO` & `jubtools-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jubtools
-Version: 0.5.3
+Version: 0.5.4
 Summary: Shared tools for my own work
 Author-email: Andrew Morcom <jubulani@fastmail.fm>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `jubtools-0.5.3/jubtools/config.py` & `jubtools-0.5.4/jubtools/config.py`

 * *Files identical despite different names*

### Comparing `jubtools-0.5.3/jubtools/httptools.py` & `jubtools-0.5.4/jubtools/httptools.py`

 * *Files identical despite different names*

### Comparing `jubtools-0.5.3/jubtools/psql.py` & `jubtools-0.5.4/jubtools/psql.py`

 * *Files identical despite different names*

### Comparing `jubtools-0.5.3/jubtools/sqlt.py` & `jubtools-0.5.4/jubtools/sqlt.py`

 * *Files identical despite different names*

### Comparing `jubtools-0.5.3/jubtools/systemtools.py` & `jubtools-0.5.4/jubtools/systemtools.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,14 +63,15 @@
             from jubtools import sqlt
             app.add_middleware(sqlt.ConnMiddleware)
 
         case DBModule.POSTGRES:
             from jubtools import psql
             app.add_event_handler("startup", psql.init)
             app.add_event_handler("shutdown", psql.shutdown)
+            app.add_middleware(psql.ConnMiddleware)
 
         case _:
             raise ValueError(f"Unknown db_module: {db_module}")
 
 
 class HealthResponse(BaseModel):
     request_ts: dt.datetime
```

### Comparing `jubtools-0.5.3/jubtools.egg-info/PKG-INFO` & `jubtools-0.5.4/jubtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jubtools
-Version: 0.5.3
+Version: 0.5.4
 Summary: Shared tools for my own work
 Author-email: Andrew Morcom <jubulani@fastmail.fm>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `jubtools-0.5.3/pyproject.toml` & `jubtools-0.5.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [project]
 name = "jubtools"
 description = "Shared tools for my own work"
 readme = "README.md"
 license = { file = "LICENSE" }
-version = "0.5.3"
+version = "0.5.4"
 authors = [{ name = "Andrew Morcom", email = "jubulani@fastmail.fm" }]
 requires-python = ">=3.10"
 dependencies = ["fastapi"]
 
 [project.optional-dependencies]
 test = [
     "async_asgi_testclient >= 1.4",
     "pytest-asyncio >= 0.23"
 ]
 
 [project.urls]
 Repository = "https://github.com/Jubulani/jubtools.git"
 
 [build-system]
-requires = ["setuptools>=68.0.0."]
+requires = ["setuptools>=68.0.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.package-data]
 "jubtools" = ["py.typed"]
```

### Comparing `jubtools-0.5.3/tests/test_config.py` & `jubtools-0.5.4/tests/test_config.py`

 * *Files identical despite different names*

