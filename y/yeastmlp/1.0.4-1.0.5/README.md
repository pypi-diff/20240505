# Comparing `tmp/yeastmlp-1.0.4.tar.gz` & `tmp/yeastmlp-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeastmlp-1.0.4.tar", last modified: Fri May  3 22:13:57 2024, max compression
+gzip compressed data, was "yeastmlp-1.0.5.tar", last modified: Sun May  5 11:53:38 2024, max compression
```

## Comparing `yeastmlp-1.0.4.tar` & `yeastmlp-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-05-03 22:13:57.216770 yeastmlp-1.0.4/
--rw-r--r--   0 k23030440   (504) staff       (20)     1065 2024-05-03 21:25:43.000000 yeastmlp-1.0.4/LICENSE
--rw-r--r--   0 k23030440   (504) staff       (20)      700 2024-05-03 22:13:57.216526 yeastmlp-1.0.4/PKG-INFO
--rw-r--r--   0 k23030440   (504) staff       (20)     1331 2024-05-03 21:25:43.000000 yeastmlp-1.0.4/README.md
--rw-r--r--   0 k23030440   (504) staff       (20)       38 2024-05-03 22:13:57.216840 yeastmlp-1.0.4/setup.cfg
--rw-r--r--   0 k23030440   (504) staff       (20)     1015 2024-05-03 22:13:53.000000 yeastmlp-1.0.4/setup.py
-drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-05-03 22:13:57.215116 yeastmlp-1.0.4/yeastmlp/
--rw-r--r--   0 k23030440   (504) staff       (20)        0 2024-05-03 21:25:43.000000 yeastmlp-1.0.4/yeastmlp/__init__.py
--rw-r--r--   0 k23030440   (504) staff       (20)    21283 2024-05-03 22:09:50.000000 yeastmlp-1.0.4/yeastmlp/adhesion.py
--rwxr-xr-x   0 k23030440   (504) staff       (20)     6394 2024-05-03 22:09:55.000000 yeastmlp-1.0.4/yeastmlp/flocculation.py
-drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-05-03 22:13:57.216197 yeastmlp-1.0.4/yeastmlp.egg-info/
--rw-r--r--   0 k23030440   (504) staff       (20)      700 2024-05-03 22:13:57.000000 yeastmlp-1.0.4/yeastmlp.egg-info/PKG-INFO
--rw-r--r--   0 k23030440   (504) staff       (20)      252 2024-05-03 22:13:57.000000 yeastmlp-1.0.4/yeastmlp.egg-info/SOURCES.txt
--rw-r--r--   0 k23030440   (504) staff       (20)        1 2024-05-03 22:13:57.000000 yeastmlp-1.0.4/yeastmlp.egg-info/dependency_links.txt
--rw-r--r--   0 k23030440   (504) staff       (20)       43 2024-05-03 22:13:57.000000 yeastmlp-1.0.4/yeastmlp.egg-info/requires.txt
--rw-r--r--   0 k23030440   (504) staff       (20)        9 2024-05-03 22:13:57.000000 yeastmlp-1.0.4/yeastmlp.egg-info/top_level.txt
+drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-05-05 11:53:38.231966 yeastmlp-1.0.5/
+-rw-r--r--   0 k23030440   (504) staff       (20)     1065 2024-05-03 21:25:43.000000 yeastmlp-1.0.5/LICENSE
+-rw-r--r--   0 k23030440   (504) staff       (20)      700 2024-05-05 11:53:38.231428 yeastmlp-1.0.5/PKG-INFO
+-rw-r--r--   0 k23030440   (504) staff       (20)     1331 2024-05-03 21:25:43.000000 yeastmlp-1.0.5/README.md
+-rw-r--r--   0 k23030440   (504) staff       (20)       38 2024-05-05 11:53:38.232168 yeastmlp-1.0.5/setup.cfg
+-rw-r--r--   0 k23030440   (504) staff       (20)     1015 2024-05-05 11:53:07.000000 yeastmlp-1.0.5/setup.py
+drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-05-05 11:53:38.227258 yeastmlp-1.0.5/yeastmlp/
+-rw-r--r--   0 k23030440   (504) staff       (20)        0 2024-05-03 21:25:43.000000 yeastmlp-1.0.5/yeastmlp/__init__.py
+-rw-r--r--   0 k23030440   (504) staff       (20)    22460 2024-05-05 11:51:22.000000 yeastmlp-1.0.5/yeastmlp/adhesion.py
+-rwxr-xr-x   0 k23030440   (504) staff       (20)     6394 2024-05-05 11:52:46.000000 yeastmlp-1.0.5/yeastmlp/flocculation.py
+drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-05-05 11:53:38.230378 yeastmlp-1.0.5/yeastmlp.egg-info/
+-rw-r--r--   0 k23030440   (504) staff       (20)      700 2024-05-05 11:53:38.000000 yeastmlp-1.0.5/yeastmlp.egg-info/PKG-INFO
+-rw-r--r--   0 k23030440   (504) staff       (20)      252 2024-05-05 11:53:38.000000 yeastmlp-1.0.5/yeastmlp.egg-info/SOURCES.txt
+-rw-r--r--   0 k23030440   (504) staff       (20)        1 2024-05-05 11:53:38.000000 yeastmlp-1.0.5/yeastmlp.egg-info/dependency_links.txt
+-rw-r--r--   0 k23030440   (504) staff       (20)       43 2024-05-05 11:53:38.000000 yeastmlp-1.0.5/yeastmlp.egg-info/requires.txt
+-rw-r--r--   0 k23030440   (504) staff       (20)        9 2024-05-05 11:53:38.000000 yeastmlp-1.0.5/yeastmlp.egg-info/top_level.txt
```

### Comparing `yeastmlp-1.0.4/LICENSE` & `yeastmlp-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yeastmlp-1.0.4/PKG-INFO` & `yeastmlp-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yeastmlp
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python package for analysis of Multicellular-like phenotype formation in yeast species
 Author: Bence Kover
 Author-email: <kover.bence@gmail.com>
 Keywords: python,yeast,biology,multicellularity,adhesion,flocculation
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yeastmlp-1.0.4/README.md` & `yeastmlp-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `yeastmlp-1.0.4/setup.py` & `yeastmlp-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #this is a setup.py file
 from setuptools import setup, find_packages
 
 
 
 
-VERSION = '1.0.4'
+VERSION = '1.0.5'
 DESCRIPTION = 'Python package for analysis of Multicellular-like phenotype formation in yeast species'
 LONG_DESCRIPTION = 'Python package for analysis of Multicellular-like phenotype formation in yeast, for more information see https://github.com/BKover99/yeastmlp'
 
 
 setup(
     name="yeastmlp",
     version=VERSION,
```

### Comparing `yeastmlp-1.0.4/yeastmlp/flocculation.py` & `yeastmlp-1.0.5/yeastmlp/flocculation.py`

 * *Files identical despite different names*

### Comparing `yeastmlp-1.0.4/yeastmlp.egg-info/PKG-INFO` & `yeastmlp-1.0.5/yeastmlp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yeastmlp
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python package for analysis of Multicellular-like phenotype formation in yeast species
 Author: Bence Kover
 Author-email: <kover.bence@gmail.com>
 Keywords: python,yeast,biology,multicellularity,adhesion,flocculation
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

