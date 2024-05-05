# Comparing `tmp/taguchi-0.0.2.tar.gz` & `tmp/taguchi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taguchi-0.0.2.tar", last modified: Sun May  5 00:56:00 2024, max compression
+gzip compressed data, was "taguchi-0.0.3.tar", last modified: Sun May  5 05:55:17 2024, max compression
```

## Comparing `taguchi-0.0.2.tar` & `taguchi-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-05 00:56:00.508794 taguchi-0.0.2/
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)     1016 2024-05-05 00:56:00.508794 taguchi-0.0.2/PKG-INFO
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)      587 2024-05-04 04:32:49.000000 taguchi-0.0.2/README.md
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)      103 2024-05-04 04:45:54.000000 taguchi-0.0.2/pyproject.toml
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)      757 2024-05-05 00:56:00.509794 taguchi-0.0.2/setup.cfg
-drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-05 00:56:00.507794 taguchi-0.0.2/taguchi/
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)       17 2024-05-05 00:55:50.000000 taguchi-0.0.2/taguchi/__init__.py
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)     1396 2024-05-04 04:37:38.000000 taguchi-0.0.2/taguchi/__main__.py
-drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-05 00:56:00.508794 taguchi-0.0.2/taguchi.egg-info/
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)     1016 2024-05-05 00:56:00.000000 taguchi-0.0.2/taguchi.egg-info/PKG-INFO
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)      262 2024-05-05 00:56:00.000000 taguchi-0.0.2/taguchi.egg-info/SOURCES.txt
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)        1 2024-05-05 00:56:00.000000 taguchi-0.0.2/taguchi.egg-info/dependency_links.txt
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)       54 2024-05-05 00:56:00.000000 taguchi-0.0.2/taguchi.egg-info/entry_points.txt
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)        1 2024-05-04 04:46:44.000000 taguchi-0.0.2/taguchi.egg-info/not-zip-safe
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)        8 2024-05-05 00:56:00.000000 taguchi-0.0.2/taguchi.egg-info/top_level.txt
+drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-05 05:55:17.294633 taguchi-0.0.3/
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)     1016 2024-05-05 05:55:17.294633 taguchi-0.0.3/PKG-INFO
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)      587 2024-05-04 04:32:49.000000 taguchi-0.0.3/README.md
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)      103 2024-05-04 04:45:54.000000 taguchi-0.0.3/pyproject.toml
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)      757 2024-05-05 05:55:17.298633 taguchi-0.0.3/setup.cfg
+drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-05 05:55:17.289632 taguchi-0.0.3/taguchi/
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)       17 2024-05-05 05:54:34.000000 taguchi-0.0.3/taguchi/__init__.py
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)     1834 2024-05-05 05:54:11.000000 taguchi-0.0.3/taguchi/__main__.py
+drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-05 05:55:17.292632 taguchi-0.0.3/taguchi.egg-info/
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)     1016 2024-05-05 05:55:17.000000 taguchi-0.0.3/taguchi.egg-info/PKG-INFO
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)      262 2024-05-05 05:55:17.000000 taguchi-0.0.3/taguchi.egg-info/SOURCES.txt
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)        1 2024-05-05 05:55:17.000000 taguchi-0.0.3/taguchi.egg-info/dependency_links.txt
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)       54 2024-05-05 05:55:17.000000 taguchi-0.0.3/taguchi.egg-info/entry_points.txt
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)        1 2024-05-04 04:46:44.000000 taguchi-0.0.3/taguchi.egg-info/not-zip-safe
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)        8 2024-05-05 05:55:17.000000 taguchi-0.0.3/taguchi.egg-info/top_level.txt
```

### Comparing `taguchi-0.0.2/PKG-INFO` & `taguchi-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taguchi
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool for optimising systems parameterised by environment variables, based on Taguchi/orthogonal array systems of experiments.
 Home-page: https://github.com/jcranney/taguchi
 Author: Jesse Cranney
 Author-email: jesse.cranney@anu.edu.au
 License: MIT license
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `taguchi-0.0.2/README.md` & `taguchi-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `taguchi-0.0.2/setup.cfg` & `taguchi-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `taguchi-0.0.2/taguchi/__main__.py` & `taguchi-0.0.3/taguchi/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 #/usr/bin/env python
-
 import os
 import yaml
 import subprocess
+import argparse
 
+parser = argparse.ArgumentParser(
+                    prog='taguchi',
+                    description='performs taguchi based experiments',
+                    epilog='see https://github.com/jcranney/taguchi for more info.')
+
+parser.add_argument('-v', '--verbose',
+            action='count', default=0)  # on/off flag
+args = parser.parse_args()
+verbose = args.verbose
 
 with open("./taguchi.yaml","r") as f:
     a : dict = yaml.full_load(f)
 
 #print(a)
 
 command = a.pop("command")
@@ -31,14 +40,17 @@
 
 results = []
 for experiment in array:
     for param,state in zip(params,experiment):
         os.environ[param] = str(a[param][state])
     proc = subprocess.Popen(command, stdout=subprocess.PIPE, shell=True)
     (out, err) = proc.communicate()
+    if verbose:
+        print(out)
+        print(err)
     out = out.decode().split("\n")
     result = None
     for o in out:
         try:
             result = float(o)
         except ValueError:
             pass
```

### Comparing `taguchi-0.0.2/taguchi.egg-info/PKG-INFO` & `taguchi-0.0.3/taguchi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taguchi
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool for optimising systems parameterised by environment variables, based on Taguchi/orthogonal array systems of experiments.
 Home-page: https://github.com/jcranney/taguchi
 Author: Jesse Cranney
 Author-email: jesse.cranney@anu.edu.au
 License: MIT license
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

