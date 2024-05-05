# Comparing `tmp/doglib-0.1.1.tar.gz` & `tmp/doglib-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doglib-0.1.1.tar", last modified: Mon Feb 12 21:31:47 2024, max compression
+gzip compressed data, was "doglib-0.1.2.tar", last modified: Sun May  5 09:57:19 2024, max compression
```

## Comparing `doglib-0.1.1.tar` & `doglib-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2024-02-12 21:31:47.426656 doglib-0.1.1/
--rw-r--r--   0 anton      (501) staff       (20)        0 2024-02-12 20:59:01.000000 doglib-0.1.1/LICENSE
--rw-r--r--   0 anton      (501) staff       (20)      650 2024-02-12 21:31:47.426345 doglib-0.1.1/PKG-INFO
--rw-r--r--   0 anton      (501) staff       (20)      215 2024-02-12 21:07:25.000000 doglib-0.1.1/README.md
--rw-r--r--   0 anton      (501) staff       (20)      103 2024-02-12 21:02:00.000000 doglib-0.1.1/pyproject.toml
--rw-r--r--   0 anton      (501) staff       (20)      559 2024-02-12 21:31:47.427702 doglib-0.1.1/setup.cfg
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2024-02-12 21:31:47.415540 doglib-0.1.1/src/
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2024-02-12 21:31:47.420272 doglib-0.1.1/src/doglib/
--rw-r--r--   0 anton      (501) staff       (20)       52 2024-02-12 21:25:15.000000 doglib-0.1.1/src/doglib/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)     1133 2024-02-12 17:59:32.000000 doglib-0.1.1/src/doglib/main.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2024-02-12 21:31:47.425108 doglib-0.1.1/src/doglib.egg-info/
--rw-r--r--   0 anton      (501) staff       (20)      650 2024-02-12 21:31:47.000000 doglib-0.1.1/src/doglib.egg-info/PKG-INFO
--rw-r--r--   0 anton      (501) staff       (20)      220 2024-02-12 21:31:47.000000 doglib-0.1.1/src/doglib.egg-info/SOURCES.txt
--rw-r--r--   0 anton      (501) staff       (20)        1 2024-02-12 21:31:47.000000 doglib-0.1.1/src/doglib.egg-info/dependency_links.txt
--rw-r--r--   0 anton      (501) staff       (20)        7 2024-02-12 21:31:47.000000 doglib-0.1.1/src/doglib.egg-info/top_level.txt
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2024-05-05 09:57:19.730446 doglib-0.1.2/
+-rw-r--r--   0 anton      (501) staff       (20)     1064 2024-05-05 08:55:09.000000 doglib-0.1.2/LICENSE
+-rw-r--r--   0 anton      (501) staff       (20)     2501 2024-05-05 09:57:19.729998 doglib-0.1.2/PKG-INFO
+-rw-r--r--   0 anton      (501) staff       (20)     1946 2024-05-05 08:55:09.000000 doglib-0.1.2/README.md
+-rw-r--r--   0 anton      (501) staff       (20)      103 2024-05-05 09:06:00.000000 doglib-0.1.2/pyproject.toml
+-rw-r--r--   0 anton      (501) staff       (20)      685 2024-05-05 09:57:19.731996 doglib-0.1.2/setup.cfg
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2024-05-05 09:57:19.706299 doglib-0.1.2/src/
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2024-05-05 09:57:19.719666 doglib-0.1.2/src/doglib/
+-rw-r--r--   0 anton      (501) staff       (20)      105 2024-05-05 08:55:19.000000 doglib-0.1.2/src/doglib/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)     3903 2024-05-05 08:55:19.000000 doglib-0.1.2/src/doglib/catlib.py
+-rw-r--r--   0 anton      (501) staff       (20)     3813 2024-05-05 08:55:19.000000 doglib-0.1.2/src/doglib/main.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2024-05-05 09:57:19.726282 doglib-0.1.2/src/doglib.egg-info/
+-rw-r--r--   0 anton      (501) staff       (20)     2501 2024-05-05 09:57:19.000000 doglib-0.1.2/src/doglib.egg-info/PKG-INFO
+-rw-r--r--   0 anton      (501) staff       (20)      274 2024-05-05 09:57:19.000000 doglib-0.1.2/src/doglib.egg-info/SOURCES.txt
+-rw-r--r--   0 anton      (501) staff       (20)        1 2024-05-05 09:57:19.000000 doglib-0.1.2/src/doglib.egg-info/dependency_links.txt
+-rw-r--r--   0 anton      (501) staff       (20)        6 2024-05-05 09:57:19.000000 doglib-0.1.2/src/doglib.egg-info/requires.txt
+-rw-r--r--   0 anton      (501) staff       (20)        7 2024-05-05 09:57:19.000000 doglib-0.1.2/src/doglib.egg-info/top_level.txt
```

