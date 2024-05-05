# Comparing `tmp/mxersion-0.2.tar.gz` & `tmp/mxersion-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mxersion-0.2.tar", last modified: Sun May  5 11:54:58 2024, max compression
+gzip compressed data, was "mxersion-0.3.tar", last modified: Sun May  5 12:16:17 2024, max compression
```

## Comparing `mxersion-0.2.tar` & `mxersion-0.3.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:54:58.637823 mxersion-0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-05 11:54:50.000000 mxersion-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-05 11:54:58.637823 mxersion-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-05 11:54:50.000000 mxersion-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:54:58.637823 mxersion-0.2/mxersion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-05 11:54:58.000000 mxersion-0.2/mxersion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-05 11:54:58.000000 mxersion-0.2/mxersion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 11:54:58.000000 mxersion-0.2/mxersion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 11:54:58.000000 mxersion-0.2/mxersion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 11:54:58.637823 mxersion-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-05 11:54:50.000000 mxersion-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:16:17.735751 mxersion-0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-05 12:16:05.000000 mxersion-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-05 12:16:17.735751 mxersion-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-05 12:16:05.000000 mxersion-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:16:17.731751 mxersion-0.3/mxersion/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-05 12:16:05.000000 mxersion-0.3/mxersion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-05 12:16:05.000000 mxersion-0.3/mxersion/hello.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:16:17.735751 mxersion-0.3/mxersion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-05 12:16:17.000000 mxersion-0.3/mxersion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-05 12:16:17.000000 mxersion-0.3/mxersion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 12:16:17.000000 mxersion-0.3/mxersion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-05 12:16:17.000000 mxersion-0.3/mxersion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 12:16:17.735751 mxersion-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-05 12:16:05.000000 mxersion-0.3/setup.py
```

### Comparing `mxersion-0.2/LICENSE` & `mxersion-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mxersion-0.2/setup.py` & `mxersion-0.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mxersion',
-    version='0.2',
+    version='0.3',
     packages=find_packages(),
     install_requires=[
         # list your dependencies here
     ],
     author='Mxytyu',
     author_email='mersion@gmail.com',
     description='mxersion is an package to interact with mxersion s api and features',
```

