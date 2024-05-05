# Comparing `tmp/tmticket-0.1.5.tar.gz` & `tmp/tmticket-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmticket-0.1.5.tar", last modified: Sun May  5 03:50:46 2024, max compression
+gzip compressed data, was "tmticket-0.1.6.tar", last modified: Sun May  5 19:03:22 2024, max compression
```

## Comparing `tmticket-0.1.5.tar` & `tmticket-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 03:50:46.225741 tmticket-0.1.5/
--rw-r--r--   0 root         (0) root         (0)      278 2024-05-05 03:50:46.225741 tmticket-0.1.5/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 03:50:46.223741 tmticket-0.1.5/pytmtickets/
--rw-r--r--   0 root         (0) root         (0)      363 2024-05-05 03:40:04.000000 tmticket-0.1.5/pytmtickets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5702 2024-05-05 03:40:04.000000 tmticket-0.1.5/pytmtickets/client.py
--rw-r--r--   0 root         (0) root         (0)    13241 2024-05-05 03:40:04.000000 tmticket-0.1.5/pytmtickets/model.py
--rw-r--r--   0 root         (0) root         (0)     4525 2024-05-05 03:40:01.000000 tmticket-0.1.5/pytmtickets/query.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-05 03:50:46.225741 tmticket-0.1.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      538 2024-05-05 03:50:12.000000 tmticket-0.1.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 03:50:46.225741 tmticket-0.1.5/tmticket.egg-info/
--rw-r--r--   0 root         (0) root         (0)      278 2024-05-05 03:50:45.000000 tmticket-0.1.5/tmticket.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      255 2024-05-05 03:50:46.000000 tmticket-0.1.5/tmticket.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 03:50:45.000000 tmticket-0.1.5/tmticket.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-05 03:50:45.000000 tmticket-0.1.5/tmticket.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-05-05 03:50:45.000000 tmticket-0.1.5/tmticket.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 19:03:22.354499 tmticket-0.1.6/
+-rw-r--r--   0 root         (0) root         (0)      278 2024-05-05 19:03:22.354499 tmticket-0.1.6/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 19:03:22.351499 tmticket-0.1.6/pytmtickets/
+-rw-r--r--   0 root         (0) root         (0)      363 2024-05-05 03:40:04.000000 tmticket-0.1.6/pytmtickets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5702 2024-05-05 03:40:04.000000 tmticket-0.1.6/pytmtickets/client.py
+-rw-r--r--   0 root         (0) root         (0)    13241 2024-05-05 03:40:04.000000 tmticket-0.1.6/pytmtickets/model.py
+-rw-r--r--   0 root         (0) root         (0)     4525 2024-05-05 03:40:01.000000 tmticket-0.1.6/pytmtickets/query.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-05 19:03:22.355499 tmticket-0.1.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      521 2024-05-05 19:01:52.000000 tmticket-0.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 19:03:22.353500 tmticket-0.1.6/tmticket.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      278 2024-05-05 19:03:21.000000 tmticket-0.1.6/tmticket.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      255 2024-05-05 19:03:22.000000 tmticket-0.1.6/tmticket.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 19:03:21.000000 tmticket-0.1.6/tmticket.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-05 19:03:21.000000 tmticket-0.1.6/tmticket.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-05 19:03:21.000000 tmticket-0.1.6/tmticket.egg-info/top_level.txt
```

### Comparing `tmticket-0.1.5/pytmtickets/client.py` & `tmticket-0.1.6/pytmtickets/client.py`

 * *Files identical despite different names*

### Comparing `tmticket-0.1.5/pytmtickets/model.py` & `tmticket-0.1.6/pytmtickets/model.py`

 * *Files identical despite different names*

### Comparing `tmticket-0.1.5/pytmtickets/query.py` & `tmticket-0.1.6/pytmtickets/query.py`

 * *Files identical despite different names*

### Comparing `tmticket-0.1.5/setup.py` & `tmticket-0.1.6/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from setuptools import setup
 import os
-#import tmticket
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='tmticket',
-    version='0.1.5',
+    version='0.1.6',
     author='hokiebrian',
     author_email='hokiebrian@gmail.com',
     description="Python wrapper for the Ticketmaster Discovery API",
 #    long_description=read('README.rst'),
     license='MIT',
     keywords='Ticketmaster',
     url='https://github.com/hokiebrian/pytmtickets',
```

