# Comparing `tmp/threadxpools-1.0.tar.gz` & `tmp/threadxpools-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threadxpools-1.0.tar", last modified: Sun May  5 19:05:43 2024, max compression
+gzip compressed data, was "threadxpools-1.1.tar", last modified: Sun May  5 19:10:32 2024, max compression
```

## Comparing `threadxpools-1.0.tar` & `threadxpools-1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 19:05:43.858246 threadxpools-1.0/
--rw-rw-rw-   0        0        0      351 2024-05-05 19:05:43.855248 threadxpools-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-05 19:05:43.858246 threadxpools-1.0/setup.cfg
--rw-rw-rw-   0        0        0      513 2024-05-05 18:43:41.000000 threadxpools-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 19:05:43.817273 threadxpools-1.0/threadxpools/
--rw-rw-rw-   0        0        0       58 2024-05-05 18:48:03.000000 threadxpools-1.0/threadxpools/__init__.py
--rw-rw-rw-   0        0        0   100690 2024-05-05 19:04:37.000000 threadxpools-1.0/threadxpools/main.py
-drwxrwxrwx   0        0        0        0 2024-05-05 19:05:43.853249 threadxpools-1.0/threadxpools.egg-info/
--rw-rw-rw-   0        0        0      351 2024-05-05 19:05:43.000000 threadxpools-1.0/threadxpools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2024-05-05 19:05:43.000000 threadxpools-1.0/threadxpools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 19:05:43.000000 threadxpools-1.0/threadxpools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-05 19:05:43.000000 threadxpools-1.0/threadxpools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-05 19:10:32.801631 threadxpools-1.1/
+-rw-rw-rw-   0        0        0      351 2024-05-05 19:10:32.798631 threadxpools-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-05 19:10:32.802630 threadxpools-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      513 2024-05-05 19:08:38.000000 threadxpools-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 19:10:32.765638 threadxpools-1.1/threadxpools/
+-rw-rw-rw-   0        0        0       58 2024-05-05 18:48:03.000000 threadxpools-1.1/threadxpools/__init__.py
+-rw-rw-rw-   0        0        0   100528 2024-05-05 19:08:29.000000 threadxpools-1.1/threadxpools/main.py
+drwxrwxrwx   0        0        0        0 2024-05-05 19:10:32.796633 threadxpools-1.1/threadxpools.egg-info/
+-rw-rw-rw-   0        0        0      351 2024-05-05 19:10:32.000000 threadxpools-1.1/threadxpools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2024-05-05 19:10:32.000000 threadxpools-1.1/threadxpools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 19:10:32.000000 threadxpools-1.1/threadxpools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-05 19:10:32.000000 threadxpools-1.1/threadxpools.egg-info/top_level.txt
```

### Comparing `threadxpools-1.0/setup.py` & `threadxpools-1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='threadxpools',
-    version='1.0',
+    version='1.1',
     packages=find_packages(),
     include_package_data=True,
     description='Una librería para ayudar a emjorar el rendimiento de threading',
     author='jenifer',
     author_email='jenifercodingf@gmail.com',
     license='MIT',
     classifiers=[
```
