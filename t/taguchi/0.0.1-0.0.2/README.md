# Comparing `tmp/taguchi-0.0.1.tar.gz` & `tmp/taguchi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taguchi-0.0.1.tar", last modified: Sun May  5 00:45:38 2024, max compression
+gzip compressed data, was "taguchi-0.0.2.tar", last modified: Sun May  5 00:56:00 2024, max compression
```

## Comparing `taguchi-0.0.1.tar` & `taguchi-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-05 00:45:38.751482 taguchi-0.0.1/
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)      929 2024-05-05 00:45:38.751482 taguchi-0.0.1/PKG-INFO
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)      587 2024-05-04 04:32:49.000000 taguchi-0.0.1/README.md
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)      103 2024-05-04 04:45:54.000000 taguchi-0.0.1/pyproject.toml
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)      669 2024-05-05 00:45:38.752482 taguchi-0.0.1/setup.cfg
-drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-05 00:45:38.751482 taguchi-0.0.1/taguchi/
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)       17 2024-05-04 04:46:38.000000 taguchi-0.0.1/taguchi/__init__.py
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)     1396 2024-05-04 04:37:38.000000 taguchi-0.0.1/taguchi/__main__.py
-drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-05 00:45:38.751482 taguchi-0.0.1/taguchi.egg-info/
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)      929 2024-05-05 00:45:38.000000 taguchi-0.0.1/taguchi.egg-info/PKG-INFO
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)      262 2024-05-05 00:45:38.000000 taguchi-0.0.1/taguchi.egg-info/SOURCES.txt
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)        1 2024-05-05 00:45:38.000000 taguchi-0.0.1/taguchi.egg-info/dependency_links.txt
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)       54 2024-05-05 00:45:38.000000 taguchi-0.0.1/taguchi.egg-info/entry_points.txt
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)        1 2024-05-04 04:46:44.000000 taguchi-0.0.1/taguchi.egg-info/not-zip-safe
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)        8 2024-05-05 00:45:38.000000 taguchi-0.0.1/taguchi.egg-info/top_level.txt
+drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-05 00:56:00.508794 taguchi-0.0.2/
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)     1016 2024-05-05 00:56:00.508794 taguchi-0.0.2/PKG-INFO
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)      587 2024-05-04 04:32:49.000000 taguchi-0.0.2/README.md
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)      103 2024-05-04 04:45:54.000000 taguchi-0.0.2/pyproject.toml
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)      757 2024-05-05 00:56:00.509794 taguchi-0.0.2/setup.cfg
+drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-05 00:56:00.507794 taguchi-0.0.2/taguchi/
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)       17 2024-05-05 00:55:50.000000 taguchi-0.0.2/taguchi/__init__.py
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)     1396 2024-05-04 04:37:38.000000 taguchi-0.0.2/taguchi/__main__.py
+drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-05 00:56:00.508794 taguchi-0.0.2/taguchi.egg-info/
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)     1016 2024-05-05 00:56:00.000000 taguchi-0.0.2/taguchi.egg-info/PKG-INFO
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)      262 2024-05-05 00:56:00.000000 taguchi-0.0.2/taguchi.egg-info/SOURCES.txt
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)        1 2024-05-05 00:56:00.000000 taguchi-0.0.2/taguchi.egg-info/dependency_links.txt
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)       54 2024-05-05 00:56:00.000000 taguchi-0.0.2/taguchi.egg-info/entry_points.txt
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)        1 2024-05-04 04:46:44.000000 taguchi-0.0.2/taguchi.egg-info/not-zip-safe
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)        8 2024-05-05 00:56:00.000000 taguchi-0.0.2/taguchi.egg-info/top_level.txt
```

### Comparing `taguchi-0.0.1/README.md` & `taguchi-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `taguchi-0.0.1/setup.cfg` & `taguchi-0.0.2/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 [metadata]
 name = taguchi
 version = attr: taguchi.VERSION
 author = Jesse Cranney
 author_email = jesse.cranney@anu.edu.au
 description = A tool for optimising systems parameterised by environment variables, based on Taguchi/orthogonal array systems of experiments.
 long_description = file: README.md
+long_description_content_type = text/markdown
 license = MIT license
 classifiers = 
 	Programming Language :: Python :: 3
+url = https://github.com/jcranney/taguchi
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 python_requires = >=3.8
```

### Comparing `taguchi-0.0.1/taguchi/__main__.py` & `taguchi-0.0.2/taguchi/__main__.py`

 * *Files identical despite different names*

