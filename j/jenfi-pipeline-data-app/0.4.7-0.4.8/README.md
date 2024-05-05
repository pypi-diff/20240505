# Comparing `tmp/jenfi_pipeline_data_app-0.4.7.tar.gz` & `tmp/jenfi_pipeline_data_app-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jenfi_pipeline_data_app-0.4.7.tar", max compression
+gzip compressed data, was "jenfi_pipeline_data_app-0.4.8.tar", max compression
```

## Comparing `jenfi_pipeline_data_app-0.4.7.tar` & `jenfi_pipeline_data_app-0.4.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      510 2024-05-03 11:43:49.429369 jenfi_pipeline_data_app-0.4.7/README.md
--rw-r--r--   0        0        0     1313 2023-01-16 02:40:26.715779 jenfi_pipeline_data_app-0.4.7/jenfi_pipeline_data_app/API.md
--rw-r--r--   0        0        0     1571 2024-05-03 17:01:00.436031 jenfi_pipeline_data_app-0.4.7/jenfi_pipeline_data_app/__init__.py
--rw-r--r--   0        0        0      354 2023-05-30 09:11:12.213698 jenfi_pipeline_data_app-0.4.7/jenfi_pipeline_data_app/_pdoc.py
--rw-r--r--   0        0        0     2367 2024-05-02 16:14:34.857722 jenfi_pipeline_data_app-0.4.7/jenfi_pipeline_data_app/app.py
--rw-r--r--   0        0        0      345 2023-05-30 09:11:12.214511 jenfi_pipeline_data_app-0.4.7/jenfi_pipeline_data_app/app_funcs/_constants.py
--rw-r--r--   0        0        0     1107 2024-02-22 07:39:24.264183 jenfi_pipeline_data_app-0.4.7/jenfi_pipeline_data_app/app_funcs/_db_handler.py
--rw-r--r--   0        0        0     1066 2023-01-16 02:40:26.716191 jenfi_pipeline_data_app-0.4.7/jenfi_pipeline_data_app/app_funcs/_exit_program.py
--rw-r--r--   0        0        0     1074 2023-05-30 09:11:12.215285 jenfi_pipeline_data_app-0.4.7/jenfi_pipeline_data_app/app_funcs/_models_s3.py
--rw-r--r--   0        0        0     1323 2023-05-30 09:11:12.216581 jenfi_pipeline_data_app-0.4.7/jenfi_pipeline_data_app/app_funcs/_parameters.py
--rw-r--r--   0        0        0     1282 2023-05-30 09:11:12.216967 jenfi_pipeline_data_app-0.4.7/jenfi_pipeline_data_app/app_funcs/_query.py
--rw-r--r--   0        0        0     2896 2023-05-30 09:11:12.217328 jenfi_pipeline_data_app-0.4.7/jenfi_pipeline_data_app/app_funcs/_result.py
--rw-r--r--   0        0        0      569 2023-05-30 09:11:12.217681 jenfi_pipeline_data_app-0.4.7/jenfi_pipeline_data_app/app_funcs/_test_funcs.py
--rw-r--r--   0        0        0     1419 2024-02-22 07:14:05.283471 jenfi_pipeline_data_app-0.4.7/jenfi_pipeline_data_app/config/db.py
--rw-r--r--   0        0        0      395 2023-05-30 09:11:12.218386 jenfi_pipeline_data_app-0.4.7/jenfi_pipeline_data_app/config/s3.py
--rw-r--r--   0        0        0       43 2023-05-30 09:11:12.218741 jenfi_pipeline_data_app-0.4.7/jenfi_pipeline_data_app/db_cache/__init__.py
--rw-r--r--   0        0        0     3838 2023-05-30 09:11:12.219328 jenfi_pipeline_data_app-0.4.7/jenfi_pipeline_data_app/db_cache/cacher.py
--rw-r--r--   0        0        0     1973 2024-05-03 11:14:13.782052 jenfi_pipeline_data_app-0.4.7/jenfi_pipeline_data_app/db_cache/db_cache.py
--rw-r--r--   0        0        0     3899 2024-05-03 16:45:19.804405 jenfi_pipeline_data_app-0.4.7/jenfi_pipeline_data_app/db_models.py
--rw-r--r--   0        0        0     1002 2024-05-03 17:01:06.721437 jenfi_pipeline_data_app-0.4.7/pyproject.toml
--rw-r--r--   0        0        0     1430 1970-01-01 00:00:00.000000 jenfi_pipeline_data_app-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0      510 2024-05-03 11:43:49.429369 jenfi_pipeline_data_app-0.4.8/README.md
+-rw-r--r--   0        0        0     1313 2023-01-16 02:40:26.715779 jenfi_pipeline_data_app-0.4.8/jenfi_pipeline_data_app/API.md
+-rw-r--r--   0        0        0     1612 2024-05-05 13:25:49.078254 jenfi_pipeline_data_app-0.4.8/jenfi_pipeline_data_app/__init__.py
+-rw-r--r--   0        0        0      354 2023-05-30 09:11:12.213698 jenfi_pipeline_data_app-0.4.8/jenfi_pipeline_data_app/_pdoc.py
+-rw-r--r--   0        0        0     2367 2024-05-02 16:14:34.857722 jenfi_pipeline_data_app-0.4.8/jenfi_pipeline_data_app/app.py
+-rw-r--r--   0        0        0      345 2023-05-30 09:11:12.214511 jenfi_pipeline_data_app-0.4.8/jenfi_pipeline_data_app/app_funcs/_constants.py
+-rw-r--r--   0        0        0     1107 2024-02-22 07:39:24.264183 jenfi_pipeline_data_app-0.4.8/jenfi_pipeline_data_app/app_funcs/_db_handler.py
+-rw-r--r--   0        0        0     1066 2023-01-16 02:40:26.716191 jenfi_pipeline_data_app-0.4.8/jenfi_pipeline_data_app/app_funcs/_exit_program.py
+-rw-r--r--   0        0        0     1074 2023-05-30 09:11:12.215285 jenfi_pipeline_data_app-0.4.8/jenfi_pipeline_data_app/app_funcs/_models_s3.py
+-rw-r--r--   0        0        0     1323 2023-05-30 09:11:12.216581 jenfi_pipeline_data_app-0.4.8/jenfi_pipeline_data_app/app_funcs/_parameters.py
+-rw-r--r--   0        0        0     1282 2023-05-30 09:11:12.216967 jenfi_pipeline_data_app-0.4.8/jenfi_pipeline_data_app/app_funcs/_query.py
+-rw-r--r--   0        0        0     2896 2023-05-30 09:11:12.217328 jenfi_pipeline_data_app-0.4.8/jenfi_pipeline_data_app/app_funcs/_result.py
+-rw-r--r--   0        0        0      569 2023-05-30 09:11:12.217681 jenfi_pipeline_data_app-0.4.8/jenfi_pipeline_data_app/app_funcs/_test_funcs.py
+-rw-r--r--   0        0        0     1419 2024-02-22 07:14:05.283471 jenfi_pipeline_data_app-0.4.8/jenfi_pipeline_data_app/config/db.py
+-rw-r--r--   0        0        0      395 2023-05-30 09:11:12.218386 jenfi_pipeline_data_app-0.4.8/jenfi_pipeline_data_app/config/s3.py
+-rw-r--r--   0        0        0       43 2023-05-30 09:11:12.218741 jenfi_pipeline_data_app-0.4.8/jenfi_pipeline_data_app/db_cache/__init__.py
+-rw-r--r--   0        0        0     3838 2023-05-30 09:11:12.219328 jenfi_pipeline_data_app-0.4.8/jenfi_pipeline_data_app/db_cache/cacher.py
+-rw-r--r--   0        0        0     1973 2024-05-03 11:14:13.782052 jenfi_pipeline_data_app-0.4.8/jenfi_pipeline_data_app/db_cache/db_cache.py
+-rw-r--r--   0        0        0     3899 2024-05-03 16:45:19.804405 jenfi_pipeline_data_app-0.4.8/jenfi_pipeline_data_app/db_models.py
+-rw-r--r--   0        0        0     1002 2024-05-05 13:25:53.618816 jenfi_pipeline_data_app-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0     1430 1970-01-01 00:00:00.000000 jenfi_pipeline_data_app-0.4.8/PKG-INFO
```

### Comparing `jenfi_pipeline_data_app-0.4.7/jenfi_pipeline_data_app/API.md` & `jenfi_pipeline_data_app-0.4.8/jenfi_pipeline_data_app/API.md`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.7/jenfi_pipeline_data_app/__init__.py` & `jenfi_pipeline_data_app-0.4.8/jenfi_pipeline_data_app/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-__version__ = "0.4.7"
+__version__ = "0.4.8"
 
 # from ._pdoc import __pdoc__
 from .app import Application
+import os
 
 PipelineDataApp = Application()
 
 PipelineDataApp.boot()
 
+core_app_name = os.getenv("CORE_APP_NAME", None)
+
 print()
 print()
 print(f"Welcome to the Jenfi Data App! v{__version__}")
-print(f"{os.getenv("CORE_APP_NAME", None)}")
+print(f"{core_app_name}")
 print("https://jenfi-eng.github.io/pipeline-data-app")
 print(
     "------------------------------------------------------------------------------------"
 )
 print()
 print("!!REQUIRED!! variables in `parameters` tagged cell.")
 print()
```

### Comparing `jenfi_pipeline_data_app-0.4.7/jenfi_pipeline_data_app/app.py` & `jenfi_pipeline_data_app-0.4.8/jenfi_pipeline_data_app/app.py`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.7/jenfi_pipeline_data_app/app_funcs/_db_handler.py` & `jenfi_pipeline_data_app-0.4.8/jenfi_pipeline_data_app/app_funcs/_db_handler.py`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.7/jenfi_pipeline_data_app/app_funcs/_exit_program.py` & `jenfi_pipeline_data_app-0.4.8/jenfi_pipeline_data_app/app_funcs/_exit_program.py`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.7/jenfi_pipeline_data_app/app_funcs/_models_s3.py` & `jenfi_pipeline_data_app-0.4.8/jenfi_pipeline_data_app/app_funcs/_models_s3.py`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.7/jenfi_pipeline_data_app/app_funcs/_parameters.py` & `jenfi_pipeline_data_app-0.4.8/jenfi_pipeline_data_app/app_funcs/_parameters.py`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.7/jenfi_pipeline_data_app/app_funcs/_query.py` & `jenfi_pipeline_data_app-0.4.8/jenfi_pipeline_data_app/app_funcs/_query.py`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.7/jenfi_pipeline_data_app/app_funcs/_result.py` & `jenfi_pipeline_data_app-0.4.8/jenfi_pipeline_data_app/app_funcs/_result.py`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.7/jenfi_pipeline_data_app/app_funcs/_test_funcs.py` & `jenfi_pipeline_data_app-0.4.8/jenfi_pipeline_data_app/app_funcs/_test_funcs.py`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.7/jenfi_pipeline_data_app/config/db.py` & `jenfi_pipeline_data_app-0.4.8/jenfi_pipeline_data_app/config/db.py`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.7/jenfi_pipeline_data_app/db_cache/cacher.py` & `jenfi_pipeline_data_app-0.4.8/jenfi_pipeline_data_app/db_cache/cacher.py`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.7/jenfi_pipeline_data_app/db_cache/db_cache.py` & `jenfi_pipeline_data_app-0.4.8/jenfi_pipeline_data_app/db_cache/db_cache.py`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.7/jenfi_pipeline_data_app/db_models.py` & `jenfi_pipeline_data_app-0.4.8/jenfi_pipeline_data_app/db_models.py`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.7/pyproject.toml` & `jenfi_pipeline_data_app-0.4.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jenfi-pipeline-data-app"
-version = "0.4.7"
+version = "0.4.8"
 description = ""
 readme = "README.md"
 authors = ["Justin Louie <224840+nitsujri@users.noreply.github.com>"]
 
 [tool.poetry.dependencies]
 python = "~3.10"
 SQLAlchemy = "^1.4.40"
```

### Comparing `jenfi_pipeline_data_app-0.4.7/PKG-INFO` & `jenfi_pipeline_data_app-0.4.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jenfi-pipeline-data-app
-Version: 0.4.7
+Version: 0.4.8
 Summary: 
 Author: Justin Louie
 Author-email: 224840+nitsujri@users.noreply.github.com
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: SQLAlchemy (>=1.4.40,<2.0.0)
```

