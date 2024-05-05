# Comparing `tmp/abstract_distances-0.0.0.8.tar.gz` & `tmp/abstract_distances-0.0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_distances-0.0.0.8.tar", last modified: Sun May  5 09:06:20 2024, max compression
+gzip compressed data, was "abstract_distances-0.0.0.9.tar", last modified: Sun May  5 09:12:53 2024, max compression
```

## Comparing `abstract_distances-0.0.0.8.tar` & `abstract_distances-0.0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-05 09:06:20.146313 abstract_distances-0.0.0.8/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      651 2024-05-05 09:06:20.146313 abstract_distances-0.0.0.8/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_distances-0.0.0.8/README.md
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-05 09:06:20.146313 abstract_distances-0.0.0.8/setup.cfg
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     1005 2024-05-05 09:06:04.000000 abstract_distances-0.0.0.8/setup.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-05 09:06:20.146313 abstract_distances-0.0.0.8/src/
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-05 09:06:20.146313 abstract_distances-0.0.0.8/src/abstract_distances/
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       24 2024-05-05 09:04:35.000000 abstract_distances-0.0.0.8/src/abstract_distances/__init__.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    10114 2024-04-25 03:57:30.000000 abstract_distances-0.0.0.8/src/abstract_distances/char_compar.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     9511 2024-05-05 09:03:34.000000 abstract_distances-0.0.0.8/src/abstract_distances/distance_cals.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     8631 2024-04-26 22:25:41.000000 abstract_distances-0.0.0.8/src/abstract_distances/do_distance.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     8233 2024-05-05 09:03:20.000000 abstract_distances-0.0.0.8/src/abstract_distances/functions.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     8858 2024-04-26 22:24:51.000000 abstract_distances-0.0.0.8/src/abstract_distances/word_compare.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-05 09:06:20.146313 abstract_distances-0.0.0.8/src/abstract_distances.egg-info/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      651 2024-05-05 09:06:20.000000 abstract_distances-0.0.0.8/src/abstract_distances.egg-info/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      473 2024-05-05 09:06:20.000000 abstract_distances-0.0.0.8/src/abstract_distances.egg-info/SOURCES.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-05 09:06:20.000000 abstract_distances-0.0.0.8/src/abstract_distances.egg-info/dependency_links.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       85 2024-05-05 09:06:20.000000 abstract_distances-0.0.0.8/src/abstract_distances.egg-info/requires.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       19 2024-05-05 09:06:20.000000 abstract_distances-0.0.0.8/src/abstract_distances.egg-info/top_level.txt
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-05 09:12:53.414381 abstract_distances-0.0.0.9/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      651 2024-05-05 09:12:53.410381 abstract_distances-0.0.0.9/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_distances-0.0.0.9/README.md
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-05 09:12:53.414381 abstract_distances-0.0.0.9/setup.cfg
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     1005 2024-05-05 09:12:44.000000 abstract_distances-0.0.0.9/setup.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-05 09:12:53.410381 abstract_distances-0.0.0.9/src/
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-05 09:12:53.410381 abstract_distances-0.0.0.9/src/abstract_distances/
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       29 2024-05-05 09:12:33.000000 abstract_distances-0.0.0.9/src/abstract_distances/__init__.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    10114 2024-04-25 03:57:30.000000 abstract_distances-0.0.0.9/src/abstract_distances/char_compar.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     9511 2024-05-05 09:03:34.000000 abstract_distances-0.0.0.9/src/abstract_distances/distance_cals.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     8631 2024-04-26 22:25:41.000000 abstract_distances-0.0.0.9/src/abstract_distances/do_distance.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     8233 2024-05-05 09:03:20.000000 abstract_distances-0.0.0.9/src/abstract_distances/functions.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     8858 2024-04-26 22:24:51.000000 abstract_distances-0.0.0.9/src/abstract_distances/word_compare.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-05 09:12:53.410381 abstract_distances-0.0.0.9/src/abstract_distances.egg-info/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      651 2024-05-05 09:12:53.000000 abstract_distances-0.0.0.9/src/abstract_distances.egg-info/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      473 2024-05-05 09:12:53.000000 abstract_distances-0.0.0.9/src/abstract_distances.egg-info/SOURCES.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-05 09:12:53.000000 abstract_distances-0.0.0.9/src/abstract_distances.egg-info/dependency_links.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       85 2024-05-05 09:12:53.000000 abstract_distances-0.0.0.9/src/abstract_distances.egg-info/requires.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       19 2024-05-05 09:12:53.000000 abstract_distances-0.0.0.9/src/abstract_distances.egg-info/top_level.txt
```

### Comparing `abstract_distances-0.0.0.8/PKG-INFO` & `abstract_distances-0.0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_distances
-Version: 0.0.0.8
+Version: 0.0.0.9
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `abstract_distances-0.0.0.8/setup.py` & `abstract_distances-0.0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_distances',
-    version='0.0.0.8',
+    version='0.0.0.9',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description="",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
           'Development Status :: 3 - Alpha',
```

### Comparing `abstract_distances-0.0.0.8/src/abstract_distances/char_compar.py` & `abstract_distances-0.0.0.9/src/abstract_distances/char_compar.py`

 * *Files identical despite different names*

### Comparing `abstract_distances-0.0.0.8/src/abstract_distances/distance_cals.py` & `abstract_distances-0.0.0.9/src/abstract_distances/distance_cals.py`

 * *Files identical despite different names*

### Comparing `abstract_distances-0.0.0.8/src/abstract_distances/do_distance.py` & `abstract_distances-0.0.0.9/src/abstract_distances/do_distance.py`

 * *Files identical despite different names*

### Comparing `abstract_distances-0.0.0.8/src/abstract_distances/functions.py` & `abstract_distances-0.0.0.9/src/abstract_distances/functions.py`

 * *Files identical despite different names*

### Comparing `abstract_distances-0.0.0.8/src/abstract_distances/word_compare.py` & `abstract_distances-0.0.0.9/src/abstract_distances/word_compare.py`

 * *Files identical despite different names*

### Comparing `abstract_distances-0.0.0.8/src/abstract_distances.egg-info/PKG-INFO` & `abstract_distances-0.0.0.9/src/abstract_distances.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_distances
-Version: 0.0.0.8
+Version: 0.0.0.9
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

