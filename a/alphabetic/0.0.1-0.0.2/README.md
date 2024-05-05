# Comparing `tmp/alphabetic-0.0.1.tar.gz` & `tmp/alphabetic-0.0.2.tar.gz`

## Comparing `alphabetic-0.0.1.tar` & `alphabetic-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,12 @@
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 alphabetic-0.0.1/Demo.ipynb
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 alphabetic-0.0.1/.ipynb_checkpoints/Demo-checkpoint.ipynb
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 alphabetic-0.0.1/alphabetic/__init__.py
--rw-r--r--   0        0        0     5590 2020-02-02 00:00:00.000000 alphabetic-0.0.1/alphabetic/core.py
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 alphabetic-0.0.1/LICENSE
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 alphabetic-0.0.1/README.md
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 alphabetic-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 alphabetic-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     8364 2020-02-02 00:00:00.000000 alphabetic-0.0.2/Demo.ipynb
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 alphabetic-0.0.2/requirements.txt
+-rw-r--r--   0        0        0     9233 2020-02-02 00:00:00.000000 alphabetic-0.0.2/.ipynb_checkpoints/Demo-checkpoint.ipynb
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 alphabetic-0.0.2/alphabetic/__init__.py
+-rw-r--r--   0        0        0    21129 2020-02-02 00:00:00.000000 alphabetic-0.0.2/alphabetic/core.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 alphabetic-0.0.2/alphabetic/requirements.txt
+-rw-r--r--   0        0        0    22412 2020-02-02 00:00:00.000000 alphabetic-0.0.2/alphabetic/data/language_data - Kopie.json
+-rw-r--r--   0        0        0    26666 2020-02-02 00:00:00.000000 alphabetic-0.0.2/alphabetic/data/language_data.json
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 alphabetic-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 alphabetic-0.0.2/README.md
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 alphabetic-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 alphabetic-0.0.2/PKG-INFO
```

### Comparing `alphabetic-0.0.1/LICENSE` & `alphabetic-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alphabetic-0.0.1/pyproject.toml` & `alphabetic-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "alphabetic"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Oren Halvani" }
 ]
 description = "A lightweight Python library for querying the alphabet of languages."
 readme = "README.md"
 requires-python = ">=3.10"
```

