# Comparing `tmp/memory_machine-0.0.1.tar.gz` & `tmp/memory_machine-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memory_machine-0.0.1.tar", last modified: Sun Apr 21 19:07:01 2024, max compression
+gzip compressed data, was "memory_machine-0.0.2.tar", last modified: Sun May  5 11:47:46 2024, max compression
```

## Comparing `memory_machine-0.0.1.tar` & `memory_machine-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-04-21 19:07:01.395765 memory_machine-0.0.1/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1074 2024-04-21 18:53:59.000000 memory_machine-0.0.1/LICENSE
--rw-r--r--   0 alxfed    (1001) alxfed    (1001)      746 2024-04-21 19:07:01.395765 memory_machine-0.0.1/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      169 2024-04-21 19:06:06.000000 memory_machine-0.0.1/README.md
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      657 2024-04-21 19:06:06.000000 memory_machine-0.0.1/pyproject.toml
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2024-04-21 19:07:01.395765 memory_machine-0.0.1/setup.cfg
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-04-21 19:07:01.395765 memory_machine-0.0.1/src/
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-04-21 19:07:01.395765 memory_machine-0.0.1/src/memory_machine/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2024-04-21 18:53:59.000000 memory_machine-0.0.1/src/memory_machine/__init__.py
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-04-21 19:07:01.395765 memory_machine-0.0.1/src/memory_machine.egg-info/
--rw-r--r--   0 alxfed    (1001) alxfed    (1001)      746 2024-04-21 19:07:01.000000 memory_machine-0.0.1/src/memory_machine.egg-info/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      231 2024-04-21 19:07:01.000000 memory_machine-0.0.1/src/memory_machine.egg-info/SOURCES.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2024-04-21 19:07:01.000000 memory_machine-0.0.1/src/memory_machine.egg-info/dependency_links.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       15 2024-04-21 19:07:01.000000 memory_machine-0.0.1/src/memory_machine.egg-info/top_level.txt
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-05 11:47:46.191682 memory_machine-0.0.2/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1074 2024-04-21 18:53:59.000000 memory_machine-0.0.2/LICENSE
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       33 2024-05-05 11:45:16.000000 memory_machine-0.0.2/MANIFEST.in
+-rw-r--r--   0 alxfed    (1001) alxfed    (1001)      802 2024-05-05 11:47:46.191682 memory_machine-0.0.2/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      165 2024-05-05 11:43:10.000000 memory_machine-0.0.2/README.md
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      767 2024-05-05 11:43:10.000000 memory_machine-0.0.2/pyproject.toml
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2024-05-05 11:47:46.191682 memory_machine-0.0.2/setup.cfg
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-05 11:47:46.191682 memory_machine-0.0.2/src/
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-05 11:47:46.191682 memory_machine-0.0.2/src/memory_machine/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      839 2024-05-05 11:43:10.000000 memory_machine-0.0.2/src/memory_machine/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1792 2024-05-04 20:39:41.000000 memory_machine-0.0.2/src/memory_machine/githf.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       78 2024-05-05 11:36:16.000000 memory_machine-0.0.2/src/memory_machine/machina.yaml
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-05 11:47:46.191682 memory_machine-0.0.2/src/memory_machine.egg-info/
+-rw-r--r--   0 alxfed    (1001) alxfed    (1001)      802 2024-05-05 11:47:46.000000 memory_machine-0.0.2/src/memory_machine.egg-info/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      344 2024-05-05 11:47:46.000000 memory_machine-0.0.2/src/memory_machine.egg-info/SOURCES.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2024-05-05 11:47:46.000000 memory_machine-0.0.2/src/memory_machine.egg-info/dependency_links.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       30 2024-05-05 11:47:46.000000 memory_machine-0.0.2/src/memory_machine.egg-info/requires.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       15 2024-05-05 11:47:46.000000 memory_machine-0.0.2/src/memory_machine.egg-info/top_level.txt
```

### Comparing `memory_machine-0.0.1/LICENSE` & `memory_machine-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `memory_machine-0.0.1/PKG-INFO` & `memory_machine-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: memory-machine
-Version: 0.0.1
+Version: 0.0.2
 Summary: State machine enhancing the memory function of Abstract Intellect.
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/memory-machine/memory-machine
 Project-URL: Bug Tracker, https://github.com/memory-machine/memory-machine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: PyGithub>=2.3.0
+Requires-Dist: PyYAML>=6.0.1
 
 # Memory Machine
-State machine enhancing the memory function of Abstract Intellect.
+A machine enhancing the memory function of Abstract Intellect.
 <pre>
   pip install memory-machine
 </pre>
 Then:
 ```Python
   import memory_machine
 ```
```

### Comparing `memory_machine-0.0.1/pyproject.toml` & `memory_machine-0.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 [build-system]
-requires = ["setuptools>=67.0"]
+requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
+
+[tool.setuptools.packages.find]
+where = ["src"]
+
 [project]
 name = "memory-machine"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     {name="Alexander Fedotov", email="alex.fedotov@aol.com"},
 ]
 description = "State machine enhancing the memory function of Abstract Intellect."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
 ]
+dependencies = [
+    "PyGithub >= 2.3.0",
+    "PyYAML >= 6.0.1"
+]
 [project.urls]
 "Homepage" = "https://github.com/memory-machine/memory-machine"
 "Bug Tracker" = "https://github.com/memory-machine/memory-machine/issues"
```

### Comparing `memory_machine-0.0.1/src/memory_machine.egg-info/PKG-INFO` & `memory_machine-0.0.2/src/memory_machine.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: memory-machine
-Version: 0.0.1
+Version: 0.0.2
 Summary: State machine enhancing the memory function of Abstract Intellect.
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/memory-machine/memory-machine
 Project-URL: Bug Tracker, https://github.com/memory-machine/memory-machine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: PyGithub>=2.3.0
+Requires-Dist: PyYAML>=6.0.1
 
 # Memory Machine
-State machine enhancing the memory function of Abstract Intellect.
+A machine enhancing the memory function of Abstract Intellect.
 <pre>
   pip install memory-machine
 </pre>
 Then:
 ```Python
   import memory_machine
 ```
```

