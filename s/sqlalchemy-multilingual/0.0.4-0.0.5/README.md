# Comparing `tmp/sqlalchemy-multilingual-0.0.4.tar.gz` & `tmp/sqlalchemy-multilingual-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-multilingual-0.0.4.tar", last modified: Sun May  5 20:22:19 2024, max compression
+gzip compressed data, was "sqlalchemy-multilingual-0.0.5.tar", last modified: Sun May  5 20:29:48 2024, max compression
```

## Comparing `sqlalchemy-multilingual-0.0.4.tar` & `sqlalchemy-multilingual-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2024-05-05 20:22:19.703226 sqlalchemy-multilingual-0.0.4/
--rw-r--r--   0 vitya      (501) staff       (20)     1063 2024-05-05 20:11:04.000000 sqlalchemy-multilingual-0.0.4/LICENSE.txt
--rw-r--r--   0 vitya      (501) staff       (20)       34 2023-06-27 13:11:56.000000 sqlalchemy-multilingual-0.0.4/MANIFEST.in
--rw-r--r--   0 vitya      (501) staff       (20)      607 2024-05-05 20:22:19.703141 sqlalchemy-multilingual-0.0.4/PKG-INFO
--rw-r--r--   0 vitya      (501) staff       (20)        0 2024-05-05 19:57:01.000000 sqlalchemy-multilingual-0.0.4/README.md
--rw-r--r--   0 vitya      (501) staff       (20)      835 2024-05-05 20:22:17.000000 sqlalchemy-multilingual-0.0.4/pyproject.toml
--rw-r--r--   0 vitya      (501) staff       (20)      579 2024-05-05 20:22:19.703481 sqlalchemy-multilingual-0.0.4/setup.cfg
--rw-r--r--   0 vitya      (501) staff       (20)      235 2024-05-05 20:15:00.000000 sqlalchemy-multilingual-0.0.4/setup.py
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2024-05-05 20:22:19.702875 sqlalchemy-multilingual-0.0.4/sqlalchemy_multilingual.egg-info/
--rw-r--r--   0 vitya      (501) staff       (20)      607 2024-05-05 20:22:19.000000 sqlalchemy-multilingual-0.0.4/sqlalchemy_multilingual.egg-info/PKG-INFO
--rw-r--r--   0 vitya      (501) staff       (20)      301 2024-05-05 20:22:19.000000 sqlalchemy-multilingual-0.0.4/sqlalchemy_multilingual.egg-info/SOURCES.txt
--rw-r--r--   0 vitya      (501) staff       (20)        1 2024-05-05 20:22:19.000000 sqlalchemy-multilingual-0.0.4/sqlalchemy_multilingual.egg-info/dependency_links.txt
--rw-r--r--   0 vitya      (501) staff       (20)       43 2024-05-05 20:22:19.000000 sqlalchemy-multilingual-0.0.4/sqlalchemy_multilingual.egg-info/requires.txt
--rw-r--r--   0 vitya      (501) staff       (20)        1 2024-05-05 20:22:19.000000 sqlalchemy-multilingual-0.0.4/sqlalchemy_multilingual.egg-info/top_level.txt
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2024-05-05 20:29:48.126256 sqlalchemy-multilingual-0.0.5/
+-rw-r--r--   0 vitya      (501) staff       (20)     1063 2024-05-05 20:11:04.000000 sqlalchemy-multilingual-0.0.5/LICENSE.txt
+-rw-r--r--   0 vitya      (501) staff       (20)       34 2023-06-27 13:11:56.000000 sqlalchemy-multilingual-0.0.5/MANIFEST.in
+-rw-r--r--   0 vitya      (501) staff       (20)      607 2024-05-05 20:29:48.126166 sqlalchemy-multilingual-0.0.5/PKG-INFO
+-rw-r--r--   0 vitya      (501) staff       (20)        0 2024-05-05 19:57:01.000000 sqlalchemy-multilingual-0.0.5/README.md
+-rw-r--r--   0 vitya      (501) staff       (20)      835 2024-05-05 20:29:45.000000 sqlalchemy-multilingual-0.0.5/pyproject.toml
+-rw-r--r--   0 vitya      (501) staff       (20)      579 2024-05-05 20:29:48.126494 sqlalchemy-multilingual-0.0.5/setup.cfg
+-rw-r--r--   0 vitya      (501) staff       (20)      235 2024-05-05 20:29:38.000000 sqlalchemy-multilingual-0.0.5/setup.py
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2024-05-05 20:29:48.125948 sqlalchemy-multilingual-0.0.5/sqlalchemy_multilingual.egg-info/
+-rw-r--r--   0 vitya      (501) staff       (20)      607 2024-05-05 20:29:48.000000 sqlalchemy-multilingual-0.0.5/sqlalchemy_multilingual.egg-info/PKG-INFO
+-rw-r--r--   0 vitya      (501) staff       (20)      301 2024-05-05 20:29:48.000000 sqlalchemy-multilingual-0.0.5/sqlalchemy_multilingual.egg-info/SOURCES.txt
+-rw-r--r--   0 vitya      (501) staff       (20)        1 2024-05-05 20:29:48.000000 sqlalchemy-multilingual-0.0.5/sqlalchemy_multilingual.egg-info/dependency_links.txt
+-rw-r--r--   0 vitya      (501) staff       (20)       43 2024-05-05 20:29:48.000000 sqlalchemy-multilingual-0.0.5/sqlalchemy_multilingual.egg-info/requires.txt
+-rw-r--r--   0 vitya      (501) staff       (20)        1 2024-05-05 20:29:48.000000 sqlalchemy-multilingual-0.0.5/sqlalchemy_multilingual.egg-info/top_level.txt
```

### Comparing `sqlalchemy-multilingual-0.0.4/LICENSE.txt` & `sqlalchemy-multilingual-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sqlalchemy-multilingual-0.0.4/PKG-INFO` & `sqlalchemy-multilingual-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-multilingual
-Version: 0.0.4
+Version: 0.0.5
 Author: Kosenko Viktor
 Author-email: oxpaoff <kosenkoviktor11@gmail.com>
 Project-URL: Homepage, https://github.com/oxpaoff/sqlalchemy-multilingual
 Project-URL: Bug Tracker, https://github.com/oxpaoff/sqlalchemy-multilingual/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sqlalchemy-multilingual-0.0.4/pyproject.toml` & `sqlalchemy-multilingual-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sqlalchemy-multilingual"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     { name = "oxpaoff", email = "kosenkoviktor11@gmail.com" },
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `sqlalchemy-multilingual-0.0.4/setup.cfg` & `sqlalchemy-multilingual-0.0.5/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sqlalchemy-multilingual
-version = 0.0.4
+version = 0.0.5
 description = ""
 long_description = file: README.md
 author = Kosenko Viktor
 author_email = kosenkoviktor11@gmail.com
 classifiers = 
 	Environment :: Web Environment
 	Intended Audience :: Developers
```

### Comparing `sqlalchemy-multilingual-0.0.4/sqlalchemy_multilingual.egg-info/PKG-INFO` & `sqlalchemy-multilingual-0.0.5/sqlalchemy_multilingual.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-multilingual
-Version: 0.0.4
+Version: 0.0.5
 Author: Kosenko Viktor
 Author-email: oxpaoff <kosenkoviktor11@gmail.com>
 Project-URL: Homepage, https://github.com/oxpaoff/sqlalchemy-multilingual
 Project-URL: Bug Tracker, https://github.com/oxpaoff/sqlalchemy-multilingual/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

