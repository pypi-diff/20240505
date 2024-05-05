# Comparing `tmp/setuptools-protobuf-0.1.8.tar.gz` & `tmp/setuptools-protobuf-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools-protobuf-0.1.8.tar", last modified: Tue Sep  5 23:01:13 2023, max compression
+gzip compressed data, was "setuptools-protobuf-0.1.9.tar", last modified: Wed Sep  6 00:14:33 2023, max compression
```

## Comparing `setuptools-protobuf-0.1.8.tar` & `setuptools-protobuf-0.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2023-09-05 23:01:13.593128 setuptools-protobuf-0.1.8/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       16 2023-09-05 23:01:02.000000 setuptools-protobuf-0.1.8/.flake8
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2023-09-05 23:01:13.589128 setuptools-protobuf-0.1.8/.github/
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2023-09-05 23:01:13.589128 setuptools-protobuf-0.1.8/.github/workflows/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      188 2023-09-05 23:01:02.000000 setuptools-protobuf-0.1.8/.github/workflows/disperse.yml
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      928 2023-09-05 23:01:02.000000 setuptools-protobuf-0.1.8/.github/workflows/pythontest.yml
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       69 2023-09-05 23:01:02.000000 setuptools-protobuf-0.1.8/.gitignore
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    11358 2023-09-05 23:01:02.000000 setuptools-protobuf-0.1.8/LICENSE
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1929 2023-09-05 23:01:13.593128 setuptools-protobuf-0.1.8/PKG-INFO
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      980 2023-09-05 23:01:02.000000 setuptools-protobuf-0.1.8/README.md
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      220 2023-09-05 23:01:02.000000 setuptools-protobuf-0.1.8/disperse.conf
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1774 2023-09-05 23:01:02.000000 setuptools-protobuf-0.1.8/pyproject.toml
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       38 2023-09-05 23:01:13.593128 setuptools-protobuf-0.1.8/setup.cfg
--rwxr-xr-x   0 jelmer    (1000) jelmer    (1000)       58 2023-09-05 23:01:02.000000 setuptools-protobuf-0.1.8/setup.py
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2023-09-05 23:01:13.589128 setuptools-protobuf-0.1.8/setuptools_protobuf/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     3692 2023-09-05 23:01:03.000000 setuptools-protobuf-0.1.8/setuptools_protobuf/__init__.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)        0 2023-09-05 23:01:02.000000 setuptools-protobuf-0.1.8/setuptools_protobuf/py.typed
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2023-09-05 23:01:13.589128 setuptools-protobuf-0.1.8/setuptools_protobuf.egg-info/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1929 2023-09-05 23:01:13.000000 setuptools-protobuf-0.1.8/setuptools_protobuf.egg-info/PKG-INFO
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      528 2023-09-05 23:01:13.000000 setuptools-protobuf-0.1.8/setuptools_protobuf.egg-info/SOURCES.txt
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)        1 2023-09-05 23:01:13.000000 setuptools-protobuf-0.1.8/setuptools_protobuf.egg-info/dependency_links.txt
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      302 2023-09-05 23:01:13.000000 setuptools-protobuf-0.1.8/setuptools_protobuf.egg-info/entry_points.txt
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       80 2023-09-05 23:01:13.000000 setuptools-protobuf-0.1.8/setuptools_protobuf.egg-info/requires.txt
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       20 2023-09-05 23:01:13.000000 setuptools-protobuf-0.1.8/setuptools_protobuf.egg-info/top_level.txt
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)        1 2023-09-05 23:01:08.000000 setuptools-protobuf-0.1.8/setuptools_protobuf.egg-info/zip-safe
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2023-09-05 23:01:13.589128 setuptools-protobuf-0.1.8/tests/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      173 2023-09-05 23:01:02.000000 setuptools-protobuf-0.1.8/tests/test_protobuf.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       85 2023-09-05 23:01:02.000000 setuptools-protobuf-0.1.8/tox.ini
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2023-09-06 00:14:33.915875 setuptools-protobuf-0.1.9/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       16 2023-09-06 00:14:24.000000 setuptools-protobuf-0.1.9/.flake8
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2023-09-06 00:14:33.911875 setuptools-protobuf-0.1.9/.github/
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2023-09-06 00:14:33.911875 setuptools-protobuf-0.1.9/.github/workflows/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      188 2023-09-06 00:14:24.000000 setuptools-protobuf-0.1.9/.github/workflows/disperse.yml
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      928 2023-09-06 00:14:24.000000 setuptools-protobuf-0.1.9/.github/workflows/pythontest.yml
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       69 2023-09-06 00:14:24.000000 setuptools-protobuf-0.1.9/.gitignore
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    11358 2023-09-06 00:14:24.000000 setuptools-protobuf-0.1.9/LICENSE
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1929 2023-09-06 00:14:33.915875 setuptools-protobuf-0.1.9/PKG-INFO
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      980 2023-09-06 00:14:24.000000 setuptools-protobuf-0.1.9/README.md
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      220 2023-09-06 00:14:24.000000 setuptools-protobuf-0.1.9/disperse.conf
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1774 2023-09-06 00:14:24.000000 setuptools-protobuf-0.1.9/pyproject.toml
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       38 2023-09-06 00:14:33.915875 setuptools-protobuf-0.1.9/setup.cfg
+-rwxr-xr-x   0 jelmer    (1000) jelmer    (1000)       58 2023-09-06 00:14:24.000000 setuptools-protobuf-0.1.9/setup.py
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2023-09-06 00:14:33.911875 setuptools-protobuf-0.1.9/setuptools_protobuf/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     3740 2023-09-06 00:14:25.000000 setuptools-protobuf-0.1.9/setuptools_protobuf/__init__.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)        0 2023-09-06 00:14:24.000000 setuptools-protobuf-0.1.9/setuptools_protobuf/py.typed
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2023-09-06 00:14:33.915875 setuptools-protobuf-0.1.9/setuptools_protobuf.egg-info/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1929 2023-09-06 00:14:33.000000 setuptools-protobuf-0.1.9/setuptools_protobuf.egg-info/PKG-INFO
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      528 2023-09-06 00:14:33.000000 setuptools-protobuf-0.1.9/setuptools_protobuf.egg-info/SOURCES.txt
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)        1 2023-09-06 00:14:33.000000 setuptools-protobuf-0.1.9/setuptools_protobuf.egg-info/dependency_links.txt
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      302 2023-09-06 00:14:33.000000 setuptools-protobuf-0.1.9/setuptools_protobuf.egg-info/entry_points.txt
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       80 2023-09-06 00:14:33.000000 setuptools-protobuf-0.1.9/setuptools_protobuf.egg-info/requires.txt
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       20 2023-09-06 00:14:33.000000 setuptools-protobuf-0.1.9/setuptools_protobuf.egg-info/top_level.txt
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)        1 2023-09-06 00:14:28.000000 setuptools-protobuf-0.1.9/setuptools_protobuf.egg-info/zip-safe
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2023-09-06 00:14:33.915875 setuptools-protobuf-0.1.9/tests/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      173 2023-09-06 00:14:24.000000 setuptools-protobuf-0.1.9/tests/test_protobuf.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       85 2023-09-06 00:14:24.000000 setuptools-protobuf-0.1.9/tox.ini
```

### Comparing `setuptools-protobuf-0.1.8/.github/workflows/pythontest.yml` & `setuptools-protobuf-0.1.9/.github/workflows/pythontest.yml`

 * *Files identical despite different names*

### Comparing `setuptools-protobuf-0.1.8/LICENSE` & `setuptools-protobuf-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools-protobuf-0.1.8/PKG-INFO` & `setuptools-protobuf-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-protobuf
-Version: 0.1.8
+Version: 0.1.9
 Summary: Setuptools protobuf extension plugin
 Author-email: Jelmer Vernooĳ <jelmer@jelmer.uk>
 License: Apachev2
 Project-URL: homepage, https://github.com/jelmer/setuptools-protobuf
 Keywords: distutils,setuptools,protobuf
 Classifier: Topic :: Software Development :: Version Control
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `setuptools-protobuf-0.1.8/README.md` & `setuptools-protobuf-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `setuptools-protobuf-0.1.8/pyproject.toml` & `setuptools-protobuf-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `setuptools-protobuf-0.1.8/setuptools_protobuf/__init__.py` & `setuptools-protobuf-0.1.9/setuptools_protobuf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from setuptools import Command
 from setuptools.dist import Distribution
 from setuptools.errors import ExecError, PlatformError  # type: ignore
 import distutils.command.build
 import distutils.command.clean
 
-__version__ = (0, 1, 8)
+__version__ = (0, 1, 9)
 
 
 def has_protobuf(command):
     return bool(getattr(command.distribution, 'protobufs', []))
 
 
 class build_protobuf(Command):
@@ -72,14 +72,17 @@
         for protobuf in getattr(self, 'protobufs', []):
             for output in protobuf.outputs():
                 try:
                     os.unlink(output)
                 except FileNotFoundError:
                     pass
 
+    def initialize_options(self):
+        pass
+
     def finalize_options(self):
         pass
 
 
 def pyprojecttoml_config(dist: Distribution) -> None:
     if sys.version_info[:2] >= (3, 11):
         from tomllib import load as toml_load
```

### Comparing `setuptools-protobuf-0.1.8/setuptools_protobuf.egg-info/PKG-INFO` & `setuptools-protobuf-0.1.9/setuptools_protobuf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-protobuf
-Version: 0.1.8
+Version: 0.1.9
 Summary: Setuptools protobuf extension plugin
 Author-email: Jelmer Vernooĳ <jelmer@jelmer.uk>
 License: Apachev2
 Project-URL: homepage, https://github.com/jelmer/setuptools-protobuf
 Keywords: distutils,setuptools,protobuf
 Classifier: Topic :: Software Development :: Version Control
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `setuptools-protobuf-0.1.8/setuptools_protobuf.egg-info/SOURCES.txt` & `setuptools-protobuf-0.1.9/setuptools_protobuf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

