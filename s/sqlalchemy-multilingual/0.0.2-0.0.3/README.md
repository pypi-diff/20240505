# Comparing `tmp/sqlalchemy-multilingual-0.0.2.tar.gz` & `tmp/sqlalchemy-multilingual-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-multilingual-0.0.2.tar", last modified: Sun May  5 20:17:50 2024, max compression
+gzip compressed data, was "sqlalchemy-multilingual-0.0.3.tar", last modified: Sun May  5 20:20:21 2024, max compression
```

## Comparing `sqlalchemy-multilingual-0.0.2.tar` & `sqlalchemy-multilingual-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2024-05-05 20:17:50.606390 sqlalchemy-multilingual-0.0.2/
--rw-r--r--   0 vitya      (501) staff       (20)     1063 2024-05-05 20:11:04.000000 sqlalchemy-multilingual-0.0.2/LICENSE.txt
--rw-r--r--   0 vitya      (501) staff       (20)       34 2023-06-27 13:11:56.000000 sqlalchemy-multilingual-0.0.2/MANIFEST.in
--rw-r--r--   0 vitya      (501) staff       (20)      608 2024-05-05 20:17:50.606320 sqlalchemy-multilingual-0.0.2/PKG-INFO
--rw-r--r--   0 vitya      (501) staff       (20)        0 2024-05-05 19:57:01.000000 sqlalchemy-multilingual-0.0.2/README.md
--rw-r--r--   0 vitya      (501) staff       (20)      836 2024-05-05 20:16:03.000000 sqlalchemy-multilingual-0.0.2/pyproject.toml
--rw-r--r--   0 vitya      (501) staff       (20)      579 2024-05-05 20:17:50.606612 sqlalchemy-multilingual-0.0.2/setup.cfg
--rw-r--r--   0 vitya      (501) staff       (20)      235 2024-05-05 20:15:00.000000 sqlalchemy-multilingual-0.0.2/setup.py
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2024-05-05 20:17:50.606151 sqlalchemy-multilingual-0.0.2/sqlalchemy_multilingual.egg-info/
--rw-r--r--   0 vitya      (501) staff       (20)      608 2024-05-05 20:17:50.000000 sqlalchemy-multilingual-0.0.2/sqlalchemy_multilingual.egg-info/PKG-INFO
--rw-r--r--   0 vitya      (501) staff       (20)      301 2024-05-05 20:17:50.000000 sqlalchemy-multilingual-0.0.2/sqlalchemy_multilingual.egg-info/SOURCES.txt
--rw-r--r--   0 vitya      (501) staff       (20)        1 2024-05-05 20:17:50.000000 sqlalchemy-multilingual-0.0.2/sqlalchemy_multilingual.egg-info/dependency_links.txt
--rw-r--r--   0 vitya      (501) staff       (20)       44 2024-05-05 20:17:50.000000 sqlalchemy-multilingual-0.0.2/sqlalchemy_multilingual.egg-info/requires.txt
--rw-r--r--   0 vitya      (501) staff       (20)        1 2024-05-05 20:17:50.000000 sqlalchemy-multilingual-0.0.2/sqlalchemy_multilingual.egg-info/top_level.txt
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2024-05-05 20:20:21.878595 sqlalchemy-multilingual-0.0.3/
+-rw-r--r--   0 vitya      (501) staff       (20)     1063 2024-05-05 20:11:04.000000 sqlalchemy-multilingual-0.0.3/LICENSE.txt
+-rw-r--r--   0 vitya      (501) staff       (20)       34 2023-06-27 13:11:56.000000 sqlalchemy-multilingual-0.0.3/MANIFEST.in
+-rw-r--r--   0 vitya      (501) staff       (20)      607 2024-05-05 20:20:21.878540 sqlalchemy-multilingual-0.0.3/PKG-INFO
+-rw-r--r--   0 vitya      (501) staff       (20)        0 2024-05-05 19:57:01.000000 sqlalchemy-multilingual-0.0.3/README.md
+-rw-r--r--   0 vitya      (501) staff       (20)      835 2024-05-05 20:20:18.000000 sqlalchemy-multilingual-0.0.3/pyproject.toml
+-rw-r--r--   0 vitya      (501) staff       (20)      579 2024-05-05 20:20:21.878813 sqlalchemy-multilingual-0.0.3/setup.cfg
+-rw-r--r--   0 vitya      (501) staff       (20)      235 2024-05-05 20:15:00.000000 sqlalchemy-multilingual-0.0.3/setup.py
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2024-05-05 20:20:21.878364 sqlalchemy-multilingual-0.0.3/sqlalchemy_multilingual.egg-info/
+-rw-r--r--   0 vitya      (501) staff       (20)      607 2024-05-05 20:20:21.000000 sqlalchemy-multilingual-0.0.3/sqlalchemy_multilingual.egg-info/PKG-INFO
+-rw-r--r--   0 vitya      (501) staff       (20)      301 2024-05-05 20:20:21.000000 sqlalchemy-multilingual-0.0.3/sqlalchemy_multilingual.egg-info/SOURCES.txt
+-rw-r--r--   0 vitya      (501) staff       (20)        1 2024-05-05 20:20:21.000000 sqlalchemy-multilingual-0.0.3/sqlalchemy_multilingual.egg-info/dependency_links.txt
+-rw-r--r--   0 vitya      (501) staff       (20)       43 2024-05-05 20:20:21.000000 sqlalchemy-multilingual-0.0.3/sqlalchemy_multilingual.egg-info/requires.txt
+-rw-r--r--   0 vitya      (501) staff       (20)        1 2024-05-05 20:20:21.000000 sqlalchemy-multilingual-0.0.3/sqlalchemy_multilingual.egg-info/top_level.txt
```

### Comparing `sqlalchemy-multilingual-0.0.2/LICENSE.txt` & `sqlalchemy-multilingual-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sqlalchemy-multilingual-0.0.2/PKG-INFO` & `sqlalchemy-multilingual-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-multilingual
-Version: 0.0.2
+Version: 0.0.3
 Author: Kosenko Viktor
 Author-email: oxpaoff <kosenkoviktor11@gmail.com>
 Project-URL: Homepage, https://github.com/oxpaoff/sqlalchemy-multilingual
 Project-URL: Bug Tracker, https://github.com/oxpaoff/sqlalchemy-multilingual/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: SQLAlchemy==2.0.29
+Requires-Dist: SQLAlchemy>=2.0.0
 Requires-Dist: typing_extensions==4.6.3
```

### Comparing `sqlalchemy-multilingual-0.0.2/pyproject.toml` & `sqlalchemy-multilingual-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sqlalchemy-multilingual"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name = "oxpaoff", email = "kosenkoviktor11@gmail.com" },
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "SQLAlchemy==2.0.29",
+    "SQLAlchemy>=2.0.0",
     "typing_extensions==4.6.3",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/oxpaoff/sqlalchemy-multilingual"
 "Bug Tracker" = "https://github.com/oxpaoff/sqlalchemy-multilingual/issues"
```

### Comparing `sqlalchemy-multilingual-0.0.2/setup.cfg` & `sqlalchemy-multilingual-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `sqlalchemy-multilingual-0.0.2/sqlalchemy_multilingual.egg-info/PKG-INFO` & `sqlalchemy-multilingual-0.0.3/sqlalchemy_multilingual.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-multilingual
-Version: 0.0.2
+Version: 0.0.3
 Author: Kosenko Viktor
 Author-email: oxpaoff <kosenkoviktor11@gmail.com>
 Project-URL: Homepage, https://github.com/oxpaoff/sqlalchemy-multilingual
 Project-URL: Bug Tracker, https://github.com/oxpaoff/sqlalchemy-multilingual/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: SQLAlchemy==2.0.29
+Requires-Dist: SQLAlchemy>=2.0.0
 Requires-Dist: typing_extensions==4.6.3
```

