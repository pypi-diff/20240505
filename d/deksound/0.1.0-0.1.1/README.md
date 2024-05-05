# Comparing `tmp/deksound-0.1.0.tar.gz` & `tmp/deksound-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deksound-0.1.0.tar", last modified: Sat Mar 30 05:16:45 2024, max compression
+gzip compressed data, was "deksound-0.1.1.tar", last modified: Sun May  5 08:35:37 2024, max compression
```

## Comparing `deksound-0.1.0.tar` & `deksound-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-03-30 05:16:44.310257 deksound-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-03-30 05:16:44.310257 deksound-0.1.0/deksound/__init__.py
--rw-r--r--   0        0        0       42 2024-03-30 05:16:44.310257 deksound-0.1.0/deksound/click/__entry__.py
--rw-r--r--   0        0        0      217 2024-03-30 05:16:44.310257 deksound-0.1.0/deksound/click/__init__.py
--rw-r--r--   0        0        0      629 2024-03-30 05:16:44.310257 deksound-0.1.0/deksound/core/__init__.py
--rw-r--r--   0        0        0    26156 2024-03-30 05:16:44.310257 deksound-0.1.0/deksound/core/res/failure.mp3
--rw-r--r--   0        0        0    31808 2024-03-30 05:16:44.310257 deksound-0.1.0/deksound/core/res/success.mp3
--rw-r--r--   0        0        0      474 2024-03-30 05:16:45.654249 deksound-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      239 1970-01-01 00:00:00.000000 deksound-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-05 08:35:36.120226 deksound-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-05 08:35:36.120226 deksound-0.1.1/deksound/__init__.py
+-rw-r--r--   0        0        0       42 2024-05-05 08:35:36.120226 deksound-0.1.1/deksound/click/__entry__.py
+-rw-r--r--   0        0        0      217 2024-05-05 08:35:36.120226 deksound-0.1.1/deksound/click/__init__.py
+-rw-r--r--   0        0        0     1143 2024-05-05 08:35:36.120226 deksound-0.1.1/deksound/core/__init__.py
+-rw-r--r--   0        0        0    26156 2024-05-05 08:35:36.120226 deksound-0.1.1/deksound/core/res/failure.mp3
+-rw-r--r--   0        0        0    31808 2024-05-05 08:35:36.120226 deksound-0.1.1/deksound/core/res/success.mp3
+-rw-r--r--   0        0        0      474 2024-05-05 08:35:37.536221 deksound-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      239 1970-01-01 00:00:00.000000 deksound-0.1.1/PKG-INFO
```

### Comparing `deksound-0.1.0/deksound/core/res/failure.mp3` & `deksound-0.1.1/deksound/core/res/failure.mp3`

 * *Files identical despite different names*

### Comparing `deksound-0.1.0/deksound/core/res/success.mp3` & `deksound-0.1.1/deksound/core/res/success.mp3`

 * *Files identical despite different names*

