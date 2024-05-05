# Comparing `tmp/LegacyNeuralNetworks-0.1.0.tar.gz` & `tmp/LegacyNeuralNetworks-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LegacyNeuralNetworks-0.1.0.tar", last modified: Mon Nov  6 03:47:50 2023, max compression
+gzip compressed data, was "LegacyNeuralNetworks-0.1.1.tar", last modified: Sun May  5 05:41:52 2024, max compression
```

## Comparing `LegacyNeuralNetworks-0.1.0.tar` & `LegacyNeuralNetworks-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-11-06 03:47:50.040556 LegacyNeuralNetworks-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-11-06 03:47:49.993677 LegacyNeuralNetworks-0.1.0/LegacyNeuralNetworks/
--rw-rw-rw-   0        0        0    29128 2023-11-04 16:24:36.000000 LegacyNeuralNetworks-0.1.0/LegacyNeuralNetworks/Fill.py
--rw-rw-rw-   0        0        0    19189 2023-05-27 08:44:43.000000 LegacyNeuralNetworks-0.1.0/LegacyNeuralNetworks/LegacyNeuralNetworks.py
--rw-rw-rw-   0        0        0      240 2023-11-05 05:31:12.000000 LegacyNeuralNetworks-0.1.0/LegacyNeuralNetworks/__init__.py
--rw-rw-rw-   0        0        0    14578 2023-05-27 14:39:19.000000 LegacyNeuralNetworks-0.1.0/LegacyNeuralNetworks/ann_fill.py
--rw-rw-rw-   0        0        0    24250 2023-11-06 03:47:14.000000 LegacyNeuralNetworks-0.1.0/LegacyNeuralNetworks/cl1.py
--rw-rw-rw-   0        0        0     9677 2023-05-28 16:18:51.000000 LegacyNeuralNetworks-0.1.0/LegacyNeuralNetworks/ds_fill.py
--rw-rw-rw-   0        0        0    40084 2023-11-05 15:27:55.000000 LegacyNeuralNetworks-0.1.0/LegacyNeuralNetworks/precarious.py
-drwxrwxrwx   0        0        0        0 2023-11-06 03:47:50.040556 LegacyNeuralNetworks-0.1.0/LegacyNeuralNetworks.egg-info/
--rw-rw-rw-   0        0        0     4398 2023-11-06 03:47:49.000000 LegacyNeuralNetworks-0.1.0/LegacyNeuralNetworks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      472 2023-11-06 03:47:49.000000 LegacyNeuralNetworks-0.1.0/LegacyNeuralNetworks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-06 03:47:49.000000 LegacyNeuralNetworks-0.1.0/LegacyNeuralNetworks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-11-06 03:47:49.000000 LegacyNeuralNetworks-0.1.0/LegacyNeuralNetworks.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-11-06 03:47:49.000000 LegacyNeuralNetworks-0.1.0/LegacyNeuralNetworks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4398 2023-11-06 03:47:50.040556 LegacyNeuralNetworks-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3284 2023-05-27 14:44:31.000000 LegacyNeuralNetworks-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-11-06 03:47:50.040556 LegacyNeuralNetworks-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      893 2023-11-06 03:47:30.000000 LegacyNeuralNetworks-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 05:41:52.422965 LegacyNeuralNetworks-0.1.1/
+drwxrwxrwx   0        0        0        0 2024-05-05 05:41:52.341708 LegacyNeuralNetworks-0.1.1/LegacyNeuralNetworks/
+-rw-rw-rw-   0        0        0     1466 2023-11-08 13:34:19.000000 LegacyNeuralNetworks-0.1.1/LegacyNeuralNetworks/02.py
+-rw-rw-rw-   0        0        0     1647 2023-11-08 13:33:26.000000 LegacyNeuralNetworks-0.1.1/LegacyNeuralNetworks/03.py
+-rw-rw-rw-   0        0        0    21401 2024-05-05 05:39:56.000000 LegacyNeuralNetworks-0.1.1/LegacyNeuralNetworks/Fill.py
+-rw-rw-rw-   0        0        0    19189 2023-05-27 08:44:43.000000 LegacyNeuralNetworks-0.1.1/LegacyNeuralNetworks/LegacyNeuralNetworks.py
+-rw-rw-rw-   0        0        0      240 2023-11-05 05:31:12.000000 LegacyNeuralNetworks-0.1.1/LegacyNeuralNetworks/__init__.py
+-rw-rw-rw-   0        0        0    14578 2023-05-27 14:39:19.000000 LegacyNeuralNetworks-0.1.1/LegacyNeuralNetworks/ann_fill.py
+-rw-rw-rw-   0        0        0    24250 2023-11-06 03:47:14.000000 LegacyNeuralNetworks-0.1.1/LegacyNeuralNetworks/cl1.py
+-rw-rw-rw-   0        0        0    16887 2024-05-05 05:41:08.000000 LegacyNeuralNetworks-0.1.1/LegacyNeuralNetworks/ds_fill.py
+-rw-rw-rw-   0        0        0    40084 2023-11-05 15:27:55.000000 LegacyNeuralNetworks-0.1.1/LegacyNeuralNetworks/precarious.py
+drwxrwxrwx   0        0        0        0 2024-05-05 05:41:52.379310 LegacyNeuralNetworks-0.1.1/LegacyNeuralNetworks.egg-info/
+-rw-rw-rw-   0        0        0     4398 2024-05-05 05:41:52.000000 LegacyNeuralNetworks-0.1.1/LegacyNeuralNetworks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      526 2024-05-05 05:41:52.000000 LegacyNeuralNetworks-0.1.1/LegacyNeuralNetworks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 05:41:52.000000 LegacyNeuralNetworks-0.1.1/LegacyNeuralNetworks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-05 05:41:52.000000 LegacyNeuralNetworks-0.1.1/LegacyNeuralNetworks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-05-05 05:41:52.000000 LegacyNeuralNetworks-0.1.1/LegacyNeuralNetworks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4398 2024-05-05 05:41:52.422965 LegacyNeuralNetworks-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3284 2023-05-27 14:44:31.000000 LegacyNeuralNetworks-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-05 05:41:52.422965 LegacyNeuralNetworks-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      893 2024-05-05 05:39:22.000000 LegacyNeuralNetworks-0.1.1/setup.py
```

### Comparing `LegacyNeuralNetworks-0.1.0/LegacyNeuralNetworks/LegacyNeuralNetworks.py` & `LegacyNeuralNetworks-0.1.1/LegacyNeuralNetworks/LegacyNeuralNetworks.py`

 * *Files identical despite different names*

### Comparing `LegacyNeuralNetworks-0.1.0/LegacyNeuralNetworks/ann_fill.py` & `LegacyNeuralNetworks-0.1.1/LegacyNeuralNetworks/ann_fill.py`

 * *Files identical despite different names*

### Comparing `LegacyNeuralNetworks-0.1.0/LegacyNeuralNetworks/cl1.py` & `LegacyNeuralNetworks-0.1.1/LegacyNeuralNetworks/cl1.py`

 * *Files identical despite different names*

### Comparing `LegacyNeuralNetworks-0.1.0/LegacyNeuralNetworks/precarious.py` & `LegacyNeuralNetworks-0.1.1/LegacyNeuralNetworks/precarious.py`

 * *Files identical despite different names*

### Comparing `LegacyNeuralNetworks-0.1.0/LegacyNeuralNetworks.egg-info/PKG-INFO` & `LegacyNeuralNetworks-0.1.1/LegacyNeuralNetworks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LegacyNeuralNetworks
-Version: 0.1.0
+Version: 0.1.1
 Summary: Legacy Neural Networks
 Home-page: UNKNOWN
 Author: Hrushikesh Kachgunde
 Author-email: <hrushiskachgunde@gmail.com>
 License: UNKNOWN
 Description: # Legacy Neural Networks
```

### Comparing `LegacyNeuralNetworks-0.1.0/PKG-INFO` & `LegacyNeuralNetworks-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LegacyNeuralNetworks
-Version: 0.1.0
+Version: 0.1.1
 Summary: Legacy Neural Networks
 Home-page: UNKNOWN
 Author: Hrushikesh Kachgunde
 Author-email: <hrushiskachgunde@gmail.com>
 License: UNKNOWN
 Description: # Legacy Neural Networks
```

### Comparing `LegacyNeuralNetworks-0.1.0/README.md` & `LegacyNeuralNetworks-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `LegacyNeuralNetworks-0.1.0/setup.py` & `LegacyNeuralNetworks-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'Legacy Neural Networks'
  
 # Setting up
 setup(
     name="LegacyNeuralNetworks",
     version=VERSION,
     author="Hrushikesh Kachgunde",
```

