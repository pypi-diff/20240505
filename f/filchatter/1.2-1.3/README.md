# Comparing `tmp/filchatter-1.2.tar.gz` & `tmp/filchatter-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filchatter-1.2.tar", last modified: Sat May  4 06:33:04 2024, max compression
+gzip compressed data, was "filchatter-1.3.tar", last modified: Sat May  4 06:43:16 2024, max compression
```

## Comparing `filchatter-1.2.tar` & `filchatter-1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 06:33:04.508418 filchatter-1.2/
-drwxrwxrwx   0        0        0        0 2024-05-04 06:33:04.489469 filchatter-1.2/Filchatter/
--rw-rw-rw-   0        0        0       63 2024-05-04 06:28:04.000000 filchatter-1.2/Filchatter/__init__.py
--rw-rw-rw-   0        0        0     1026 2024-05-04 05:01:05.000000 filchatter-1.2/Filchatter/filchatter.py
--rw-rw-rw-   0        0        0     1070 2024-05-04 05:07:58.000000 filchatter-1.2/LICENSE.md
--rw-rw-rw-   0        0        0      106 2024-05-04 06:33:04.507423 filchatter-1.2/PKG-INFO
--rw-rw-rw-   0        0        0      208 2024-05-04 05:10:02.000000 filchatter-1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 06:33:04.506425 filchatter-1.2/filchatter.egg-info/
--rw-rw-rw-   0        0        0      106 2024-05-04 06:33:04.000000 filchatter-1.2/filchatter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2024-05-04 06:33:04.000000 filchatter-1.2/filchatter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 06:33:04.000000 filchatter-1.2/filchatter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-05-04 06:33:04.000000 filchatter-1.2/filchatter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-05-04 06:33:04.000000 filchatter-1.2/filchatter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-04 06:33:04.000000 filchatter-1.2/filchatter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-04 06:33:04.508418 filchatter-1.2/setup.cfg
--rw-rw-rw-   0        0        0      278 2024-05-04 06:27:39.000000 filchatter-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 06:43:16.385155 filchatter-1.3/
+drwxrwxrwx   0        0        0        0 2024-05-04 06:43:16.366207 filchatter-1.3/Filchatter/
+-rw-rw-rw-   0        0        0       62 2024-05-04 06:42:16.000000 filchatter-1.3/Filchatter/__init__.py
+-rw-rw-rw-   0        0        0     1026 2024-05-04 06:43:09.000000 filchatter-1.3/Filchatter/filchatter.py
+-rw-rw-rw-   0        0        0     1070 2024-05-04 05:07:58.000000 filchatter-1.3/LICENSE.md
+-rw-rw-rw-   0        0        0      106 2024-05-04 06:43:16.384158 filchatter-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2024-05-04 05:10:02.000000 filchatter-1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 06:43:16.383161 filchatter-1.3/filchatter.egg-info/
+-rw-rw-rw-   0        0        0      106 2024-05-04 06:43:16.000000 filchatter-1.3/filchatter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2024-05-04 06:43:16.000000 filchatter-1.3/filchatter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 06:43:16.000000 filchatter-1.3/filchatter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-05-04 06:43:16.000000 filchatter-1.3/filchatter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-05-04 06:43:16.000000 filchatter-1.3/filchatter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-04 06:43:16.000000 filchatter-1.3/filchatter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 06:43:16.386154 filchatter-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      278 2024-05-04 06:42:50.000000 filchatter-1.3/setup.py
```

### Comparing `filchatter-1.2/Filchatter/filchatter.py` & `filchatter-1.3/Filchatter/filchatter.py`

 * *Files identical despite different names*

### Comparing `filchatter-1.2/LICENSE.md` & `filchatter-1.3/LICENSE.md`

 * *Files identical despite different names*

