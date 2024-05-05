# Comparing `tmp/mxersion-0.1.tar.gz` & `tmp/mxersion-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mxersion-0.1.tar", last modified: Sun May  5 10:29:06 2024, max compression
+gzip compressed data, was "mxersion-0.2.tar", last modified: Sun May  5 11:54:58 2024, max compression
```

## Comparing `mxersion-0.1.tar` & `mxersion-0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:29:06.973322 mxersion-0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-05 10:28:54.000000 mxersion-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-05 10:29:06.969322 mxersion-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-05 10:28:54.000000 mxersion-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:29:06.969322 mxersion-0.1/mxersion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-05 10:29:06.000000 mxersion-0.1/mxersion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-05 10:29:06.000000 mxersion-0.1/mxersion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 10:29:06.000000 mxersion-0.1/mxersion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 10:29:06.000000 mxersion-0.1/mxersion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 10:29:06.973322 mxersion-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-05 10:28:54.000000 mxersion-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:54:58.637823 mxersion-0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-05 11:54:50.000000 mxersion-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-05 11:54:58.637823 mxersion-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-05 11:54:50.000000 mxersion-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:54:58.637823 mxersion-0.2/mxersion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-05 11:54:58.000000 mxersion-0.2/mxersion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-05 11:54:58.000000 mxersion-0.2/mxersion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 11:54:58.000000 mxersion-0.2/mxersion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 11:54:58.000000 mxersion-0.2/mxersion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 11:54:58.637823 mxersion-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-05 11:54:50.000000 mxersion-0.2/setup.py
```

### Comparing `mxersion-0.1/LICENSE` & `mxersion-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mxersion-0.1/setup.py` & `mxersion-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mxersion',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     install_requires=[
         # list your dependencies here
     ],
     author='Mxytyu',
     author_email='mersion@gmail.com',
     description='mxersion is an package to interact with mxersion s api and features',
```

