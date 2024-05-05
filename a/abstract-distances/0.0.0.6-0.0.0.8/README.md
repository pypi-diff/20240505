# Comparing `tmp/abstract_distances-0.0.0.6.tar.gz` & `tmp/abstract_distances-0.0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_distances-0.0.0.6.tar", last modified: Sun May  5 09:05:11 2024, max compression
+gzip compressed data, was "abstract_distances-0.0.0.8.tar", last modified: Sun May  5 09:06:20 2024, max compression
```

## Comparing `abstract_distances-0.0.0.6.tar` & `abstract_distances-0.0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-05 09:05:11.835801 abstract_distances-0.0.0.6/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      613 2024-05-05 09:05:11.835801 abstract_distances-0.0.0.6/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_distances-0.0.0.6/README.md
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-05 09:05:11.835801 abstract_distances-0.0.0.6/setup.cfg
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      982 2024-05-05 09:04:43.000000 abstract_distances-0.0.0.6/setup.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-05 09:05:11.835801 abstract_distances-0.0.0.6/src/
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-05 09:05:11.835801 abstract_distances-0.0.0.6/src/abstract_distances/
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       24 2024-05-05 09:04:35.000000 abstract_distances-0.0.0.6/src/abstract_distances/__init__.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    10114 2024-04-25 03:57:30.000000 abstract_distances-0.0.0.6/src/abstract_distances/char_compar.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     9511 2024-05-05 09:03:34.000000 abstract_distances-0.0.0.6/src/abstract_distances/distance_cals.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     8631 2024-04-26 22:25:41.000000 abstract_distances-0.0.0.6/src/abstract_distances/do_distance.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     8233 2024-05-05 09:03:20.000000 abstract_distances-0.0.0.6/src/abstract_distances/functions.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     8858 2024-04-26 22:24:51.000000 abstract_distances-0.0.0.6/src/abstract_distances/word_compare.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-05 09:05:11.835801 abstract_distances-0.0.0.6/src/abstract_distances.egg-info/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      613 2024-05-05 09:05:11.000000 abstract_distances-0.0.0.6/src/abstract_distances.egg-info/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      473 2024-05-05 09:05:11.000000 abstract_distances-0.0.0.6/src/abstract_distances.egg-info/SOURCES.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-05 09:05:11.000000 abstract_distances-0.0.0.6/src/abstract_distances.egg-info/dependency_links.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       62 2024-05-05 09:05:11.000000 abstract_distances-0.0.0.6/src/abstract_distances.egg-info/requires.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       19 2024-05-05 09:05:11.000000 abstract_distances-0.0.0.6/src/abstract_distances.egg-info/top_level.txt
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-05 09:06:20.146313 abstract_distances-0.0.0.8/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      651 2024-05-05 09:06:20.146313 abstract_distances-0.0.0.8/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_distances-0.0.0.8/README.md
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-05 09:06:20.146313 abstract_distances-0.0.0.8/setup.cfg
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     1005 2024-05-05 09:06:04.000000 abstract_distances-0.0.0.8/setup.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-05 09:06:20.146313 abstract_distances-0.0.0.8/src/
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-05 09:06:20.146313 abstract_distances-0.0.0.8/src/abstract_distances/
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       24 2024-05-05 09:04:35.000000 abstract_distances-0.0.0.8/src/abstract_distances/__init__.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    10114 2024-04-25 03:57:30.000000 abstract_distances-0.0.0.8/src/abstract_distances/char_compar.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     9511 2024-05-05 09:03:34.000000 abstract_distances-0.0.0.8/src/abstract_distances/distance_cals.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     8631 2024-04-26 22:25:41.000000 abstract_distances-0.0.0.8/src/abstract_distances/do_distance.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     8233 2024-05-05 09:03:20.000000 abstract_distances-0.0.0.8/src/abstract_distances/functions.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     8858 2024-04-26 22:24:51.000000 abstract_distances-0.0.0.8/src/abstract_distances/word_compare.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-05 09:06:20.146313 abstract_distances-0.0.0.8/src/abstract_distances.egg-info/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      651 2024-05-05 09:06:20.000000 abstract_distances-0.0.0.8/src/abstract_distances.egg-info/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      473 2024-05-05 09:06:20.000000 abstract_distances-0.0.0.8/src/abstract_distances.egg-info/SOURCES.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-05 09:06:20.000000 abstract_distances-0.0.0.8/src/abstract_distances.egg-info/dependency_links.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       85 2024-05-05 09:06:20.000000 abstract_distances-0.0.0.8/src/abstract_distances.egg-info/requires.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       19 2024-05-05 09:06:20.000000 abstract_distances-0.0.0.8/src/abstract_distances.egg-info/top_level.txt
```

### Comparing `abstract_distances-0.0.0.6/PKG-INFO` & `abstract_distances-0.0.0.8/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: abstract_distances
-Version: 0.0.0.6
+Version: 0.0.0.8
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: abstract_utilities
-Requires-Dist: pandas
-Requires-Dist: openpyxl
 Requires-Dist: abstract_security
+Requires-Dist: abstract_pandas
 Requires-Dist: requests
+Requires-Dist: openlocationcode
+Requires-Dist: numpy
 
 #magnets... how do they work? who invented them?
```

### Comparing `abstract_distances-0.0.0.6/setup.py` & `abstract_distances-0.0.0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_distances',
-    version='0.0.0.6',
+    version='0.0.0.8',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description="",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
           'Development Status :: 3 - Alpha',
           'Intended Audience :: Developers',
           'License :: OSI Approved :: MIT License',
           'Programming Language :: Python :: 3',
           'Programming Language :: Python :: 3.11',
       ],
-    install_requires=['abstract_utilities', 'pandas', 'openpyxl','abstract_security','requests'],
+    install_requires=['abstract_utilities','abstract_security','abstract_pandas','requests','openlocationcode','numpy'],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.6",
     # Add this line to include wheel format in your distribution
     setup_requires=['wheel'],
 )
```

### Comparing `abstract_distances-0.0.0.6/src/abstract_distances/char_compar.py` & `abstract_distances-0.0.0.8/src/abstract_distances/char_compar.py`

 * *Files identical despite different names*

### Comparing `abstract_distances-0.0.0.6/src/abstract_distances/distance_cals.py` & `abstract_distances-0.0.0.8/src/abstract_distances/distance_cals.py`

 * *Files identical despite different names*

### Comparing `abstract_distances-0.0.0.6/src/abstract_distances/do_distance.py` & `abstract_distances-0.0.0.8/src/abstract_distances/do_distance.py`

 * *Files identical despite different names*

### Comparing `abstract_distances-0.0.0.6/src/abstract_distances/functions.py` & `abstract_distances-0.0.0.8/src/abstract_distances/functions.py`

 * *Files identical despite different names*

### Comparing `abstract_distances-0.0.0.6/src/abstract_distances/word_compare.py` & `abstract_distances-0.0.0.8/src/abstract_distances/word_compare.py`

 * *Files identical despite different names*

### Comparing `abstract_distances-0.0.0.6/src/abstract_distances.egg-info/PKG-INFO` & `abstract_distances-0.0.0.8/src/abstract_distances.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: abstract_distances
-Version: 0.0.0.6
+Version: 0.0.0.8
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: abstract_utilities
-Requires-Dist: pandas
-Requires-Dist: openpyxl
 Requires-Dist: abstract_security
+Requires-Dist: abstract_pandas
 Requires-Dist: requests
+Requires-Dist: openlocationcode
+Requires-Dist: numpy
 
 #magnets... how do they work? who invented them?
```

