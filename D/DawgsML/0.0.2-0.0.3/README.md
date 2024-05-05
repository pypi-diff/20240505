# Comparing `tmp/dawgsml-0.0.2.tar.gz` & `tmp/dawgsml-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dawgsml-0.0.2.tar", last modified: Sat May  4 03:40:47 2024, max compression
+gzip compressed data, was "dawgsml-0.0.3.tar", last modified: Sun May  5 14:17:50 2024, max compression
```

## Comparing `dawgsml-0.0.2.tar` & `dawgsml-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 03:40:47.509451 dawgsml-0.0.2/
-drwxrwxrwx   0        0        0        0 2024-05-04 03:40:47.508452 dawgsml-0.0.2/DawgsML.egg-info/
--rw-rw-rw-   0        0        0     1190 2024-05-04 03:40:47.000000 dawgsml-0.0.2/DawgsML.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2024-05-04 03:40:47.000000 dawgsml-0.0.2/DawgsML.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 03:40:47.000000 dawgsml-0.0.2/DawgsML.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-04 03:40:47.000000 dawgsml-0.0.2/DawgsML.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1084 2024-05-04 02:01:47.000000 dawgsml-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1190 2024-05-04 03:40:47.508452 dawgsml-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       64 2024-05-04 02:01:47.000000 dawgsml-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 03:40:47.501453 dawgsml-0.0.2/dawgs_ml/
--rw-rw-rw-   0        0        0        2 2024-05-04 02:01:47.000000 dawgsml-0.0.2/dawgs_ml/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 03:40:47.503455 dawgsml-0.0.2/dawgs_ml/dataframe/
--rw-rw-rw-   0        0        0        0 2024-05-04 02:04:46.000000 dawgsml-0.0.2/dawgs_ml/dataframe/__init__.py
--rw-rw-rw-   0        0        0    16304 2024-05-04 02:09:39.000000 dawgsml-0.0.2/dawgs_ml/dataframe/dataframe.py
--rw-rw-rw-   0        0        0     6083 2024-05-04 02:21:02.000000 dawgsml-0.0.2/dawgs_ml/models.py
--rw-rw-rw-   0        0        0      679 2024-05-04 02:19:12.000000 dawgsml-0.0.2/dawgs_ml/preprocess.py
-drwxrwxrwx   0        0        0        0 2024-05-04 03:40:47.506451 dawgsml-0.0.2/dawgs_ml/utils/
--rw-rw-rw-   0        0        0        0 2024-05-04 02:12:21.000000 dawgsml-0.0.2/dawgs_ml/utils/__init__.py
--rw-rw-rw-   0        0        0    14184 2024-05-04 02:19:12.000000 dawgsml-0.0.2/dawgs_ml/utils/model_utils.py
--rw-rw-rw-   0        0        0      585 2024-05-04 02:19:12.000000 dawgsml-0.0.2/dawgs_ml/utils/utils.py
--rw-rw-rw-   0        0        0       42 2024-05-04 03:40:47.509451 dawgsml-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1386 2024-05-04 03:38:36.000000 dawgsml-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 14:17:50.728064 dawgsml-0.0.3/
+drwxrwxrwx   0        0        0        0 2024-05-05 14:17:50.725065 dawgsml-0.0.3/DawgsML.egg-info/
+-rw-rw-rw-   0        0        0     2731 2024-05-05 14:17:50.000000 dawgsml-0.0.3/DawgsML.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2024-05-05 14:17:50.000000 dawgsml-0.0.3/DawgsML.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 14:17:50.000000 dawgsml-0.0.3/DawgsML.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-05 14:17:50.000000 dawgsml-0.0.3/DawgsML.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1084 2024-05-04 02:01:47.000000 dawgsml-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2731 2024-05-05 14:17:50.726063 dawgsml-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1605 2024-05-05 14:15:35.000000 dawgsml-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 14:17:50.716666 dawgsml-0.0.3/dawgs_ml/
+-rw-rw-rw-   0        0        0        2 2024-05-04 02:01:47.000000 dawgsml-0.0.3/dawgs_ml/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 14:17:50.719057 dawgsml-0.0.3/dawgs_ml/dataframe/
+-rw-rw-rw-   0        0        0        0 2024-05-04 02:04:46.000000 dawgsml-0.0.3/dawgs_ml/dataframe/__init__.py
+-rw-rw-rw-   0        0        0    16304 2024-05-04 02:09:39.000000 dawgsml-0.0.3/dawgs_ml/dataframe/dataframe.py
+-rw-rw-rw-   0        0        0     6083 2024-05-04 02:21:02.000000 dawgsml-0.0.3/dawgs_ml/models.py
+-rw-rw-rw-   0        0        0      679 2024-05-04 02:19:12.000000 dawgsml-0.0.3/dawgs_ml/preprocess.py
+drwxrwxrwx   0        0        0        0 2024-05-05 14:17:50.723065 dawgsml-0.0.3/dawgs_ml/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-04 02:12:21.000000 dawgsml-0.0.3/dawgs_ml/utils/__init__.py
+-rw-rw-rw-   0        0        0    14184 2024-05-04 02:19:12.000000 dawgsml-0.0.3/dawgs_ml/utils/model_utils.py
+-rw-rw-rw-   0        0        0      585 2024-05-04 02:19:12.000000 dawgsml-0.0.3/dawgs_ml/utils/utils.py
+-rw-rw-rw-   0        0        0       42 2024-05-05 14:17:50.728064 dawgsml-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1524 2024-05-05 14:16:51.000000 dawgsml-0.0.3/setup.py
```

### Comparing `dawgsml-0.0.2/LICENSE` & `dawgsml-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dawgsml-0.0.2/dawgs_ml/dataframe/dataframe.py` & `dawgsml-0.0.3/dawgs_ml/dataframe/dataframe.py`

 * *Files identical despite different names*

### Comparing `dawgsml-0.0.2/dawgs_ml/models.py` & `dawgsml-0.0.3/dawgs_ml/models.py`

 * *Files identical despite different names*

### Comparing `dawgsml-0.0.2/dawgs_ml/preprocess.py` & `dawgsml-0.0.3/dawgs_ml/preprocess.py`

 * *Files identical despite different names*

### Comparing `dawgsml-0.0.2/dawgs_ml/utils/model_utils.py` & `dawgsml-0.0.3/dawgs_ml/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `dawgsml-0.0.2/dawgs_ml/utils/utils.py` & `dawgsml-0.0.3/dawgs_ml/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dawgsml-0.0.2/setup.py` & `dawgsml-0.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 from setuptools import setup, find_packages
 
+
+def read_readme():
+    with open('README.md', 'r', encoding='utf-8') as f:
+        long_description = f.read()
+    return long_description
+
+
 setup(
     name='DawgsML',
-    version='0.0.2',
+    version='0.0.3',
     author='Andrea Marchi',
     author_email='andreaphilly@hotmail.com',
     description='A simple library for machine learning without a requirements.txt',
-    long_description=open('README.md').read(),
+    long_description=read_readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/Doriasamp/DawgsML.git',
     packages=find_packages(),
     install_requires=[],  # nothing here
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

