# Comparing `tmp/Tavin-1.1.7.tar.gz` & `tmp/Tavin-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Tavin-1.1.7.tar", last modified: Tue Feb 20 12:26:37 2024, max compression
+gzip compressed data, was "Tavin-1.1.8.tar", last modified: Sun May  5 03:18:31 2024, max compression
```

## Comparing `Tavin-1.1.7.tar` & `Tavin-1.1.8.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-02-20 12:26:36.800000 Tavin-1.1.7/
--rw-rw-rw-   0        0        0      698 2024-02-20 12:26:38.000000 Tavin-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      298 2024-02-18 12:43:26.000000 Tavin-1.1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-02-20 12:26:36.840000 Tavin-1.1.7/Tavin/
--rw-rw-rw-   0        0        0      525 2024-02-20 12:26:26.000000 Tavin-1.1.7/Tavin/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-20 12:26:36.880000 Tavin-1.1.7/Tavin.egg-info/
--rw-rw-rw-   0        0        0     1092 2024-02-18 04:25:36.000000 Tavin-1.1.7/Tavin.egg-info/LICENSE.txt
--rw-rw-rw-   0        0        0      698 2024-02-20 12:26:38.000000 Tavin-1.1.7/Tavin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2024-02-18 04:24:52.000000 Tavin-1.1.7/Tavin.egg-info/README.md
--rw-rw-rw-   0        0        0      245 2024-02-20 12:26:38.000000 Tavin-1.1.7/Tavin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-20 12:26:38.000000 Tavin-1.1.7/Tavin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-02-20 12:26:38.000000 Tavin-1.1.7/Tavin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-02-20 12:26:38.000000 Tavin-1.1.7/Tavin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-20 12:26:38.000000 Tavin-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0      643 2024-02-20 12:26:36.000000 Tavin-1.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-20 12:26:36.940000 Tavin-1.1.7/test/
--rw-rw-rw-   0        0        0      525 2024-02-19 12:10:14.000000 Tavin-1.1.7/test/test.py
+drwxrwxrwx   0        0        0        0 2024-05-05 03:18:31.634462 Tavin-1.1.8/
+-rw-rw-rw-   0        0        0      698 2024-05-05 03:18:31.634462 Tavin-1.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-02-20 12:26:52.000000 Tavin-1.1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 03:18:31.627952 Tavin-1.1.8/Tavin/
+-rw-rw-rw-   0        0        0      333 2024-05-05 03:18:09.000000 Tavin-1.1.8/Tavin/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 03:18:31.634462 Tavin-1.1.8/Tavin.egg-info/
+-rw-rw-rw-   0        0        0      698 2024-05-05 03:18:31.000000 Tavin-1.1.8/Tavin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2024-05-05 03:18:31.000000 Tavin-1.1.8/Tavin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 03:18:31.000000 Tavin-1.1.8/Tavin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-05 03:18:31.000000 Tavin-1.1.8/Tavin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-05 03:18:31.000000 Tavin-1.1.8/Tavin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-05 03:18:31.634462 Tavin-1.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      626 2024-05-05 03:18:27.000000 Tavin-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 03:18:31.634462 Tavin-1.1.8/test/
+-rw-rw-rw-   0        0        0      501 2024-02-20 12:26:52.000000 Tavin-1.1.8/test/test.py
```

### Comparing `Tavin-1.1.7/PKG-INFO` & `Tavin-1.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Tavin
-Version: 1.1.7
+Version: 1.1.8
 Summary: A concise application framework.
 Home-page: https://github.com/lemonorangeapple/Tavin
 Author: lemonorangeapple
 Author-email: jcj1947725596@hotmail.com
 License: MIT
 Description: # Tavin
```

### Comparing `Tavin-1.1.7/Tavin.egg-info/PKG-INFO` & `Tavin-1.1.8/Tavin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Tavin
-Version: 1.1.7
+Version: 1.1.8
 Summary: A concise application framework.
 Home-page: https://github.com/lemonorangeapple/Tavin
 Author: lemonorangeapple
 Author-email: jcj1947725596@hotmail.com
 License: MIT
 Description: # Tavin
```

