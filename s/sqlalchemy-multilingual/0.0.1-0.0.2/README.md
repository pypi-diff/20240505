# Comparing `tmp/sqlalchemy-multilingual-0.0.1.tar.gz` & `tmp/sqlalchemy-multilingual-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-multilingual-0.0.1.tar", last modified: Sun May  5 19:57:24 2024, max compression
+gzip compressed data, was "sqlalchemy-multilingual-0.0.2.tar", last modified: Sun May  5 20:17:50 2024, max compression
```

## Comparing `sqlalchemy-multilingual-0.0.1.tar` & `sqlalchemy-multilingual-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,14 @@
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2024-05-05 19:57:24.142505 sqlalchemy-multilingual-0.0.1/
--rw-r--r--   0 vitya      (501) staff       (20)      588 2024-05-05 19:57:24.142447 sqlalchemy-multilingual-0.0.1/PKG-INFO
--rw-r--r--   0 vitya      (501) staff       (20)        0 2024-05-05 19:57:01.000000 sqlalchemy-multilingual-0.0.1/README.md
--rw-r--r--   0 vitya      (501) staff       (20)      639 2024-05-05 19:57:24.142739 sqlalchemy-multilingual-0.0.1/setup.cfg
--rw-r--r--   0 vitya      (501) staff       (20)      235 2024-05-05 19:57:17.000000 sqlalchemy-multilingual-0.0.1/setup.py
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2024-05-05 19:57:24.142228 sqlalchemy-multilingual-0.0.1/sqlalchemy_multilingual.egg-info/
--rw-r--r--   0 vitya      (501) staff       (20)      588 2024-05-05 19:57:24.000000 sqlalchemy-multilingual-0.0.1/sqlalchemy_multilingual.egg-info/PKG-INFO
--rw-r--r--   0 vitya      (501) staff       (20)      216 2024-05-05 19:57:24.000000 sqlalchemy-multilingual-0.0.1/sqlalchemy_multilingual.egg-info/SOURCES.txt
--rw-r--r--   0 vitya      (501) staff       (20)        1 2024-05-05 19:57:24.000000 sqlalchemy-multilingual-0.0.1/sqlalchemy_multilingual.egg-info/dependency_links.txt
--rw-r--r--   0 vitya      (501) staff       (20)        1 2024-05-05 19:57:24.000000 sqlalchemy-multilingual-0.0.1/sqlalchemy_multilingual.egg-info/top_level.txt
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2024-05-05 20:17:50.606390 sqlalchemy-multilingual-0.0.2/
+-rw-r--r--   0 vitya      (501) staff       (20)     1063 2024-05-05 20:11:04.000000 sqlalchemy-multilingual-0.0.2/LICENSE.txt
+-rw-r--r--   0 vitya      (501) staff       (20)       34 2023-06-27 13:11:56.000000 sqlalchemy-multilingual-0.0.2/MANIFEST.in
+-rw-r--r--   0 vitya      (501) staff       (20)      608 2024-05-05 20:17:50.606320 sqlalchemy-multilingual-0.0.2/PKG-INFO
+-rw-r--r--   0 vitya      (501) staff       (20)        0 2024-05-05 19:57:01.000000 sqlalchemy-multilingual-0.0.2/README.md
+-rw-r--r--   0 vitya      (501) staff       (20)      836 2024-05-05 20:16:03.000000 sqlalchemy-multilingual-0.0.2/pyproject.toml
+-rw-r--r--   0 vitya      (501) staff       (20)      579 2024-05-05 20:17:50.606612 sqlalchemy-multilingual-0.0.2/setup.cfg
+-rw-r--r--   0 vitya      (501) staff       (20)      235 2024-05-05 20:15:00.000000 sqlalchemy-multilingual-0.0.2/setup.py
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2024-05-05 20:17:50.606151 sqlalchemy-multilingual-0.0.2/sqlalchemy_multilingual.egg-info/
+-rw-r--r--   0 vitya      (501) staff       (20)      608 2024-05-05 20:17:50.000000 sqlalchemy-multilingual-0.0.2/sqlalchemy_multilingual.egg-info/PKG-INFO
+-rw-r--r--   0 vitya      (501) staff       (20)      301 2024-05-05 20:17:50.000000 sqlalchemy-multilingual-0.0.2/sqlalchemy_multilingual.egg-info/SOURCES.txt
+-rw-r--r--   0 vitya      (501) staff       (20)        1 2024-05-05 20:17:50.000000 sqlalchemy-multilingual-0.0.2/sqlalchemy_multilingual.egg-info/dependency_links.txt
+-rw-r--r--   0 vitya      (501) staff       (20)       44 2024-05-05 20:17:50.000000 sqlalchemy-multilingual-0.0.2/sqlalchemy_multilingual.egg-info/requires.txt
+-rw-r--r--   0 vitya      (501) staff       (20)        1 2024-05-05 20:17:50.000000 sqlalchemy-multilingual-0.0.2/sqlalchemy_multilingual.egg-info/top_level.txt
```

### Comparing `sqlalchemy-multilingual-0.0.1/setup.cfg` & `sqlalchemy-multilingual-0.0.2/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 [metadata]
 name = sqlalchemy-multilingual
-version = 0.0.1
+version = 0.0.2
 description = ""
 long_description = file: README.md
-url = https://github.com/DJWOMS/GSpot
 author = Kosenko Viktor
 author_email = kosenkoviktor11@gmail.com
-license = MIT License
 classifiers = 
 	Environment :: Web Environment
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3.11
```

