# Comparing `tmp/magic_extract-0.2.2.tar.gz` & `tmp/magic_extract-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magic_extract-0.2.2.tar", last modified: Thu Jul 21 21:02:38 2022, max compression
+gzip compressed data, was "magic_extract-0.3.0.tar", last modified: Sun May  5 20:16:36 2024, max compression
```

## Comparing `magic_extract-0.2.2.tar` & `magic_extract-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 jeffwu     (501) staff       (20)        0 2022-07-21 21:02:38.030531 magic_extract-0.2.2/
--rw-r--r--   0 jeffwu     (501) staff       (20)       42 2021-05-13 22:03:29.000000 magic_extract-0.2.2/.gitignore
--rw-r--r--   0 jeffwu     (501) staff       (20)     1080 2021-05-13 22:03:29.000000 magic_extract-0.2.2/LICENSE
--rw-r--r--   0 jeffwu     (501) staff       (20)      336 2022-07-21 21:02:38.030205 magic_extract-0.2.2/PKG-INFO
--rw-r--r--   0 jeffwu     (501) staff       (20)      704 2022-01-07 06:22:44.000000 magic_extract-0.2.2/README.md
--rw-r--r--   0 jeffwu     (501) staff       (20)      124 2021-05-13 22:05:06.000000 magic_extract-0.2.2/development.md
-drwxr-xr-x   0 jeffwu     (501) staff       (20)        0 2022-07-21 21:02:37.986449 magic_extract-0.2.2/magic_extract/
--rw-r--r--   0 jeffwu     (501) staff       (20)     2602 2022-01-07 06:24:07.000000 magic_extract-0.2.2/magic_extract/__init__.py
-drwxr-xr-x   0 jeffwu     (501) staff       (20)        0 2022-07-21 21:02:38.029626 magic_extract-0.2.2/magic_extract.egg-info/
--rw-r--r--   0 jeffwu     (501) staff       (20)      336 2022-07-21 21:02:37.000000 magic_extract-0.2.2/magic_extract.egg-info/PKG-INFO
--rw-r--r--   0 jeffwu     (501) staff       (20)      226 2022-07-21 21:02:37.000000 magic_extract-0.2.2/magic_extract.egg-info/SOURCES.txt
--rw-r--r--   0 jeffwu     (501) staff       (20)        1 2022-07-21 21:02:37.000000 magic_extract-0.2.2/magic_extract.egg-info/dependency_links.txt
--rw-r--r--   0 jeffwu     (501) staff       (20)       14 2022-07-21 21:02:37.000000 magic_extract-0.2.2/magic_extract.egg-info/top_level.txt
--rw-r--r--   0 jeffwu     (501) staff       (20)       38 2022-07-21 21:02:38.030618 magic_extract-0.2.2/setup.cfg
--rw-r--r--   0 jeffwu     (501) staff       (20)      382 2022-07-21 21:02:31.000000 magic_extract-0.2.2/setup.py
+drwxr-xr-x   0 jeffwu     (502) staff       (20)        0 2024-05-05 20:16:36.930153 magic_extract-0.3.0/
+-rw-r--r--   0 jeffwu     (502) staff       (20)     1080 2021-05-13 22:03:29.000000 magic_extract-0.3.0/LICENSE
+-rw-r--r--   0 jeffwu     (502) staff       (20)      291 2024-05-05 20:16:36.929675 magic_extract-0.3.0/PKG-INFO
+-rw-r--r--   0 jeffwu     (502) staff       (20)      704 2022-01-07 06:22:44.000000 magic_extract-0.3.0/README.md
+drwxr-xr-x   0 jeffwu     (502) staff       (20)        0 2024-05-05 20:16:36.927887 magic_extract-0.3.0/magic_extract/
+-rw-r--r--   0 jeffwu     (502) staff       (20)     5410 2024-05-05 20:14:22.000000 magic_extract-0.3.0/magic_extract/__init__.py
+-rw-r--r--   0 jeffwu     (502) staff       (20)      269 2024-05-05 20:15:11.000000 magic_extract-0.3.0/magic_extract/test_basic.py
+drwxr-xr-x   0 jeffwu     (502) staff       (20)        0 2024-05-05 20:16:36.929248 magic_extract-0.3.0/magic_extract.egg-info/
+-rw-r--r--   0 jeffwu     (502) staff       (20)      291 2024-05-05 20:16:36.000000 magic_extract-0.3.0/magic_extract.egg-info/PKG-INFO
+-rw-r--r--   0 jeffwu     (502) staff       (20)      228 2024-05-05 20:16:36.000000 magic_extract-0.3.0/magic_extract.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffwu     (502) staff       (20)        1 2024-05-05 20:16:36.000000 magic_extract-0.3.0/magic_extract.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffwu     (502) staff       (20)       14 2024-05-05 20:16:36.000000 magic_extract-0.3.0/magic_extract.egg-info/top_level.txt
+-rw-r--r--   0 jeffwu     (502) staff       (20)       38 2024-05-05 20:16:36.930226 magic_extract-0.3.0/setup.cfg
+-rw-r--r--   0 jeffwu     (502) staff       (20)      382 2024-05-05 20:16:30.000000 magic_extract-0.3.0/setup.py
```

### Comparing `magic_extract-0.2.2/LICENSE` & `magic_extract-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `magic_extract-0.2.2/README.md` & `magic_extract-0.3.0/README.md`

 * *Files identical despite different names*

