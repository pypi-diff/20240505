# Comparing `tmp/thingking_machine-0.0.1.tar.gz` & `tmp/thingking_machine-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thingking_machine-0.0.1.tar", last modified: Sat May  4 20:42:57 2024, max compression
+gzip compressed data, was "thingking_machine-0.0.2.tar", last modified: Sun May  5 11:48:30 2024, max compression
```

## Comparing `thingking_machine-0.0.1.tar` & `thingking_machine-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 20:42:57.075581 thingking_machine-0.0.1/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1074 2024-05-04 20:30:59.000000 thingking_machine-0.0.1/LICENSE
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       36 2024-05-04 20:37:28.000000 thingking_machine-0.0.1/MANIFEST.in
--rw-r--r--   0 alxfed    (1001) alxfed    (1001)      769 2024-05-04 20:42:57.075581 thingking_machine-0.0.1/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      158 2024-05-04 20:37:28.000000 thingking_machine-0.0.1/README.md
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      748 2024-05-04 20:37:28.000000 thingking_machine-0.0.1/pyproject.toml
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2024-05-04 20:42:57.075581 thingking_machine-0.0.1/setup.cfg
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 20:42:57.071581 thingking_machine-0.0.1/src/
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 20:42:57.075581 thingking_machine-0.0.1/src/thingking_machine/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      875 2024-05-04 20:37:28.000000 thingking_machine-0.0.1/src/thingking_machine/__init__.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1792 2024-05-04 20:39:41.000000 thingking_machine-0.0.1/src/thingking_machine/githf.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       64 2024-05-04 20:39:41.000000 thingking_machine-0.0.1/src/thingking_machine/machina.yaml
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 20:42:57.075581 thingking_machine-0.0.1/src/thingking_machine.egg-info/
--rw-r--r--   0 alxfed    (1001) alxfed    (1001)      769 2024-05-04 20:42:57.000000 thingking_machine-0.0.1/src/thingking_machine.egg-info/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      368 2024-05-04 20:42:57.000000 thingking_machine-0.0.1/src/thingking_machine.egg-info/SOURCES.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2024-05-04 20:42:57.000000 thingking_machine-0.0.1/src/thingking_machine.egg-info/dependency_links.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       30 2024-05-04 20:42:57.000000 thingking_machine-0.0.1/src/thingking_machine.egg-info/requires.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       18 2024-05-04 20:42:57.000000 thingking_machine-0.0.1/src/thingking_machine.egg-info/top_level.txt
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-05 11:48:30.584351 thingking_machine-0.0.2/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1074 2024-05-04 20:30:59.000000 thingking_machine-0.0.2/LICENSE
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       36 2024-05-04 20:37:28.000000 thingking_machine-0.0.2/MANIFEST.in
+-rw-r--r--   0 alxfed    (1001) alxfed    (1001)      769 2024-05-05 11:48:30.584351 thingking_machine-0.0.2/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      158 2024-05-04 20:37:28.000000 thingking_machine-0.0.2/README.md
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      748 2024-05-05 11:46:49.000000 thingking_machine-0.0.2/pyproject.toml
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2024-05-05 11:48:30.584351 thingking_machine-0.0.2/setup.cfg
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-05 11:48:30.564351 thingking_machine-0.0.2/src/
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-05 11:48:30.584351 thingking_machine-0.0.2/src/thingking_machine/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      873 2024-05-05 11:43:10.000000 thingking_machine-0.0.2/src/thingking_machine/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1792 2024-05-04 20:39:41.000000 thingking_machine-0.0.2/src/thingking_machine/githf.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       64 2024-05-05 11:34:43.000000 thingking_machine-0.0.2/src/thingking_machine/machina.yaml
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-05 11:48:30.584351 thingking_machine-0.0.2/src/thingking_machine.egg-info/
+-rw-r--r--   0 alxfed    (1001) alxfed    (1001)      769 2024-05-05 11:48:30.000000 thingking_machine-0.0.2/src/thingking_machine.egg-info/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      368 2024-05-05 11:48:30.000000 thingking_machine-0.0.2/src/thingking_machine.egg-info/SOURCES.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2024-05-05 11:48:30.000000 thingking_machine-0.0.2/src/thingking_machine.egg-info/dependency_links.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       30 2024-05-05 11:48:30.000000 thingking_machine-0.0.2/src/thingking_machine.egg-info/requires.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       18 2024-05-05 11:48:30.000000 thingking_machine-0.0.2/src/thingking_machine.egg-info/top_level.txt
```

### Comparing `thingking_machine-0.0.1/LICENSE` & `thingking_machine-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `thingking_machine-0.0.1/PKG-INFO` & `thingking_machine-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thingking-machine
-Version: 0.0.1
+Version: 0.0.2
 Summary: Description of the Machine
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/thingking-machine/thingking-machine
 Project-URL: Bug Tracker, https://github.com/thingking-machine/thingking-machine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `thingking_machine-0.0.1/pyproject.toml` & `thingking_machine-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "thingking-machine"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     {name="Alexander Fedotov", email="alex.fedotov@aol.com"},
 ]
 description = "Description of the Machine"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers=[
```

### Comparing `thingking_machine-0.0.1/src/thingking_machine/__init__.py` & `thingking_machine-0.0.2/src/thingking_machine/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,8 +20,8 @@
     MACHINE_YAML = githf.read_file(repository=gh, file_path='machina.yaml')
 
 except Exception as e:
     machina_path = os.path.join(os.path.dirname(__file__), 'machina.yaml')
     with open(machina_path, 'r') as yaml_file:
         MACHINE_YAML = yaml_file.read()
 
-NAME_OF_THE_MACHINE = yaml.load(MACHINE_YAML, Loader=yaml.FullLoader)
+THINGKING_MACHINE = yaml.load(MACHINE_YAML, Loader=yaml.FullLoader)
```

### Comparing `thingking_machine-0.0.1/src/thingking_machine/githf.py` & `thingking_machine-0.0.2/src/thingking_machine/githf.py`

 * *Files identical despite different names*

### Comparing `thingking_machine-0.0.1/src/thingking_machine.egg-info/PKG-INFO` & `thingking_machine-0.0.2/src/thingking_machine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thingking-machine
-Version: 0.0.1
+Version: 0.0.2
 Summary: Description of the Machine
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/thingking-machine/thingking-machine
 Project-URL: Bug Tracker, https://github.com/thingking-machine/thingking-machine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

