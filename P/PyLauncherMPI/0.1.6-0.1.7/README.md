# Comparing `tmp/pylaunchermpi-0.1.6.tar.gz` & `tmp/pylaunchermpi-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylaunchermpi-0.1.6.tar", last modified: Sat May  4 13:01:23 2024, max compression
+gzip compressed data, was "pylaunchermpi-0.1.7.tar", last modified: Sun May  5 16:43:30 2024, max compression
```

## Comparing `pylaunchermpi-0.1.6.tar` & `pylaunchermpi-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-04 13:01:23.259848 pylaunchermpi-0.1.6/
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)     1081 2024-05-01 12:21:07.000000 pylaunchermpi-0.1.6/LICENSE
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)     2565 2024-05-04 13:01:23.259848 pylaunchermpi-0.1.6/PKG-INFO
-drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-04 13:01:23.259848 pylaunchermpi-0.1.6/PyLauncherMPI.egg-info/
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)     2565 2024-05-04 13:01:23.000000 pylaunchermpi-0.1.6/PyLauncherMPI.egg-info/PKG-INFO
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      298 2024-05-04 13:01:23.000000 pylaunchermpi-0.1.6/PyLauncherMPI.egg-info/SOURCES.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)        1 2024-05-04 13:01:23.000000 pylaunchermpi-0.1.6/PyLauncherMPI.egg-info/dependency_links.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)       58 2024-05-04 13:01:23.000000 pylaunchermpi-0.1.6/PyLauncherMPI.egg-info/entry_points.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)        7 2024-05-04 13:01:23.000000 pylaunchermpi-0.1.6/PyLauncherMPI.egg-info/requires.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)       14 2024-05-04 13:01:23.000000 pylaunchermpi-0.1.6/PyLauncherMPI.egg-info/top_level.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)     1726 2024-05-01 13:26:59.000000 pylaunchermpi-0.1.6/README.md
-drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-04 13:01:23.259848 pylaunchermpi-0.1.6/pylaunchermpi/
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)        0 2024-05-01 13:09:05.000000 pylaunchermpi-0.1.6/pylaunchermpi/__init__.py
--rw-------   0 john_vm   (1000) john_vm   (1000)     3080 2024-05-04 12:56:47.000000 pylaunchermpi-0.1.6/pylaunchermpi/main.py
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)       38 2024-05-04 13:01:23.259848 pylaunchermpi-0.1.6/setup.cfg
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)     1195 2024-05-04 12:59:26.000000 pylaunchermpi-0.1.6/setup.py
+drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-05 16:43:30.442691 pylaunchermpi-0.1.7/
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)     1081 2024-05-01 12:21:07.000000 pylaunchermpi-0.1.7/LICENSE
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)     2565 2024-05-05 16:43:30.442691 pylaunchermpi-0.1.7/PKG-INFO
+drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-05 16:43:30.442691 pylaunchermpi-0.1.7/PyLauncherMPI.egg-info/
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)     2565 2024-05-05 16:43:30.000000 pylaunchermpi-0.1.7/PyLauncherMPI.egg-info/PKG-INFO
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      298 2024-05-05 16:43:30.000000 pylaunchermpi-0.1.7/PyLauncherMPI.egg-info/SOURCES.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)        1 2024-05-05 16:43:30.000000 pylaunchermpi-0.1.7/PyLauncherMPI.egg-info/dependency_links.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)       58 2024-05-05 16:43:30.000000 pylaunchermpi-0.1.7/PyLauncherMPI.egg-info/entry_points.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)        7 2024-05-05 16:43:30.000000 pylaunchermpi-0.1.7/PyLauncherMPI.egg-info/requires.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)       14 2024-05-05 16:43:30.000000 pylaunchermpi-0.1.7/PyLauncherMPI.egg-info/top_level.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)     1726 2024-05-01 13:26:59.000000 pylaunchermpi-0.1.7/README.md
+drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-05 16:43:30.442691 pylaunchermpi-0.1.7/pylaunchermpi/
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)        0 2024-05-01 13:09:05.000000 pylaunchermpi-0.1.7/pylaunchermpi/__init__.py
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)     3832 2024-05-05 16:39:30.000000 pylaunchermpi-0.1.7/pylaunchermpi/main.py
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)       38 2024-05-05 16:43:30.442691 pylaunchermpi-0.1.7/setup.cfg
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)     1195 2024-05-05 16:39:05.000000 pylaunchermpi-0.1.7/setup.py
```

### Comparing `pylaunchermpi-0.1.6/LICENSE` & `pylaunchermpi-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pylaunchermpi-0.1.6/PKG-INFO` & `pylaunchermpi-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyLauncherMPI
-Version: 0.1.6
+Version: 0.1.7
 Summary: A simple MPI-based task scheduler for dynamically distributing commands across MPI processes.
 Home-page: https://github.com/ioannis-vm/PyLauncherMPI
 Author: John Vouvakis Manousakis
 Author-email: ioannis_vm@berkeley.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `pylaunchermpi-0.1.6/PyLauncherMPI.egg-info/PKG-INFO` & `pylaunchermpi-0.1.7/PyLauncherMPI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyLauncherMPI
-Version: 0.1.6
+Version: 0.1.7
 Summary: A simple MPI-based task scheduler for dynamically distributing commands across MPI processes.
 Home-page: https://github.com/ioannis-vm/PyLauncherMPI
 Author: John Vouvakis Manousakis
 Author-email: ioannis_vm@berkeley.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `pylaunchermpi-0.1.6/README.md` & `pylaunchermpi-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pylaunchermpi-0.1.6/setup.py` & `pylaunchermpi-0.1.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='PyLauncherMPI',
-    version='0.1.6',
+    version='0.1.7',
     author='John Vouvakis Manousakis',
     author_email='ioannis_vm@berkeley.edu',
     description=(
         'A simple MPI-based task scheduler for dynamically '
         'distributing commands across MPI processes.'
     ),
     long_description=open('README.md').read(),
```

