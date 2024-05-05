# Comparing `tmp/gradescope-tool-0.0.2.tar.gz` & `tmp/gradescope-tool-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gradescope-tool-0.0.2.tar", last modified: Thu Apr 25 22:32:52 2024, max compression
+gzip compressed data, was "gradescope-tool-0.1.0.tar", last modified: Sun May  5 02:01:38 2024, max compression
```

## Comparing `gradescope-tool-0.0.2.tar` & `gradescope-tool-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 nitro      (501) staff       (20)        0 2024-04-25 22:32:52.284085 gradescope-tool-0.0.2/
--rw-r--r--   0 nitro      (501) staff       (20)     1091 2024-04-25 19:40:47.000000 gradescope-tool-0.0.2/LICENSE
--rw-r--r--   0 nitro      (501) staff       (20)     1558 2024-04-25 22:32:52.284165 gradescope-tool-0.0.2/PKG-INFO
--rw-r--r--   0 nitro      (501) staff       (20)      992 2024-04-25 22:31:21.000000 gradescope-tool-0.0.2/README.md
-drwxr-xr-x   0 nitro      (501) staff       (20)        0 2024-04-25 22:32:52.283404 gradescope-tool-0.0.2/gradescope/
--rw-r--r--   0 nitro      (501) staff       (20)      270 2024-04-25 19:38:11.000000 gradescope-tool-0.0.2/gradescope/__init__.py
--rw-r--r--   0 nitro      (501) staff       (20)      441 2024-04-23 01:07:33.000000 gradescope-tool-0.0.2/gradescope/constants.py
--rw-r--r--   0 nitro      (501) staff       (20)     1629 2024-04-25 22:14:50.000000 gradescope-tool-0.0.2/gradescope/dataclass.py
--rw-r--r--   0 nitro      (501) staff       (20)      524 2024-04-25 19:38:03.000000 gradescope-tool-0.0.2/gradescope/errors.py
--rw-r--r--   0 nitro      (501) staff       (20)    11141 2024-04-25 22:19:34.000000 gradescope-tool-0.0.2/gradescope/gradescope.py
--rw-r--r--   0 nitro      (501) staff       (20)      776 2024-04-25 17:53:16.000000 gradescope-tool-0.0.2/gradescope/utils.py
-drwxr-xr-x   0 nitro      (501) staff       (20)        0 2024-04-25 22:32:52.283962 gradescope-tool-0.0.2/gradescope_tool.egg-info/
--rw-r--r--   0 nitro      (501) staff       (20)     1558 2024-04-25 22:32:52.000000 gradescope-tool-0.0.2/gradescope_tool.egg-info/PKG-INFO
--rw-r--r--   0 nitro      (501) staff       (20)      329 2024-04-25 22:32:52.000000 gradescope-tool-0.0.2/gradescope_tool.egg-info/SOURCES.txt
--rw-r--r--   0 nitro      (501) staff       (20)        1 2024-04-25 22:32:52.000000 gradescope-tool-0.0.2/gradescope_tool.egg-info/dependency_links.txt
--rw-r--r--   0 nitro      (501) staff       (20)       11 2024-04-25 22:32:52.000000 gradescope-tool-0.0.2/gradescope_tool.egg-info/top_level.txt
--rw-r--r--   0 nitro      (501) staff       (20)       79 2024-04-25 22:32:52.284409 gradescope-tool-0.0.2/setup.cfg
--rw-r--r--   0 nitro      (501) staff       (20)      812 2024-04-25 22:32:11.000000 gradescope-tool-0.0.2/setup.py
+drwxr-xr-x   0 nitro      (501) staff       (20)        0 2024-05-05 02:01:38.414529 gradescope-tool-0.1.0/
+-rw-r--r--   0 nitro      (501) staff       (20)     1091 2024-04-25 19:40:47.000000 gradescope-tool-0.1.0/LICENSE
+-rw-r--r--   0 nitro      (501) staff       (20)     9390 2024-05-05 02:01:38.414625 gradescope-tool-0.1.0/PKG-INFO
+-rw-r--r--   0 nitro      (501) staff       (20)     8825 2024-05-05 01:57:29.000000 gradescope-tool-0.1.0/README.md
+drwxr-xr-x   0 nitro      (501) staff       (20)        0 2024-05-05 02:01:38.413782 gradescope-tool-0.1.0/gradescope/
+-rw-r--r--   0 nitro      (501) staff       (20)      270 2024-04-25 19:38:11.000000 gradescope-tool-0.1.0/gradescope/__init__.py
+-rw-r--r--   0 nitro      (501) staff       (20)      441 2024-04-25 22:39:25.000000 gradescope-tool-0.1.0/gradescope/constants.py
+-rw-r--r--   0 nitro      (501) staff       (20)     2136 2024-04-25 23:06:44.000000 gradescope-tool-0.1.0/gradescope/dataclass.py
+-rw-r--r--   0 nitro      (501) staff       (20)      537 2024-04-25 23:05:16.000000 gradescope-tool-0.1.0/gradescope/errors.py
+-rw-r--r--   0 nitro      (501) staff       (20)    15676 2024-04-25 23:06:39.000000 gradescope-tool-0.1.0/gradescope/gradescope.py
+-rw-r--r--   0 nitro      (501) staff       (20)     1783 2024-04-25 23:06:41.000000 gradescope-tool-0.1.0/gradescope/utils.py
+drwxr-xr-x   0 nitro      (501) staff       (20)        0 2024-05-05 02:01:38.414381 gradescope-tool-0.1.0/gradescope_tool.egg-info/
+-rw-r--r--   0 nitro      (501) staff       (20)     9390 2024-05-05 02:01:38.000000 gradescope-tool-0.1.0/gradescope_tool.egg-info/PKG-INFO
+-rw-r--r--   0 nitro      (501) staff       (20)      329 2024-05-05 02:01:38.000000 gradescope-tool-0.1.0/gradescope_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 nitro      (501) staff       (20)        1 2024-05-05 02:01:38.000000 gradescope-tool-0.1.0/gradescope_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 nitro      (501) staff       (20)       11 2024-05-05 02:01:38.000000 gradescope-tool-0.1.0/gradescope_tool.egg-info/top_level.txt
+-rw-r--r--   0 nitro      (501) staff       (20)       79 2024-05-05 02:01:38.414900 gradescope-tool-0.1.0/setup.cfg
+-rw-r--r--   0 nitro      (501) staff       (20)      812 2024-05-05 01:59:33.000000 gradescope-tool-0.1.0/setup.py
```

### Comparing `gradescope-tool-0.0.2/LICENSE` & `gradescope-tool-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gradescope-tool-0.0.2/gradescope/errors.py` & `gradescope-tool-0.1.0/gradescope/errors.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# errors.py
+
 class GradescopeError(Exception):
     def __init__(self, msg: str):
         self.msg = msg
 
     def __str__(self):
         return self.msg
```

### Comparing `gradescope-tool-0.0.2/setup.py` & `gradescope-tool-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-VERSION = '0.0.2'
+VERSION = '0.1.0'
 
 
 with open('README.md', 'r', encoding='utf8') as f:
     long_description = f.read()
 
 
 setuptools.setup(
```

