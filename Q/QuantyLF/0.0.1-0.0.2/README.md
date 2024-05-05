# Comparing `tmp/quantylf-0.0.1.tar.gz` & `tmp/quantylf-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantylf-0.0.1.tar", last modified: Sun May  5 05:26:25 2024, max compression
+gzip compressed data, was "quantylf-0.0.2.tar", last modified: Sun May  5 05:38:32 2024, max compression
```

## Comparing `quantylf-0.0.1.tar` & `quantylf-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 05:26:25.958650 quantylf-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-05 05:26:17.000000 quantylf-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-05 05:26:25.958650 quantylf-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-05 05:26:17.000000 quantylf-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-05 05:26:17.000000 quantylf-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-05 05:26:25.958650 quantylf-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 05:26:25.954650 quantylf-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 05:26:25.954650 quantylf-0.0.1/src/QuantyLF/
--rw-r--r--   0 runner    (1001) docker     (127)    18551 2024-05-05 05:26:17.000000 quantylf-0.0.1/src/QuantyLF/QuantyLF.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 05:26:17.000000 quantylf-0.0.1/src/QuantyLF/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 05:26:25.958650 quantylf-0.0.1/src/QuantyLF.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-05 05:26:25.000000 quantylf-0.0.1/src/QuantyLF.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-05 05:26:25.000000 quantylf-0.0.1/src/QuantyLF.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 05:26:25.000000 quantylf-0.0.1/src/QuantyLF.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-05 05:26:25.000000 quantylf-0.0.1/src/QuantyLF.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-05 05:26:25.000000 quantylf-0.0.1/src/QuantyLF.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 05:38:32.317323 quantylf-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-05 05:38:28.000000 quantylf-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-05 05:38:32.317323 quantylf-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-05 05:38:28.000000 quantylf-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-05 05:38:28.000000 quantylf-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-05 05:38:32.321323 quantylf-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 05:38:32.317323 quantylf-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 05:38:32.317323 quantylf-0.0.2/src/QuantyLF/
+-rw-r--r--   0 runner    (1001) docker     (127)    18551 2024-05-05 05:38:28.000000 quantylf-0.0.2/src/QuantyLF/QuantyLF.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 05:38:28.000000 quantylf-0.0.2/src/QuantyLF/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 05:38:32.317323 quantylf-0.0.2/src/QuantyLF.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-05 05:38:32.000000 quantylf-0.0.2/src/QuantyLF.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-05 05:38:32.000000 quantylf-0.0.2/src/QuantyLF.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 05:38:32.000000 quantylf-0.0.2/src/QuantyLF.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-05 05:38:32.000000 quantylf-0.0.2/src/QuantyLF.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-05 05:38:32.000000 quantylf-0.0.2/src/QuantyLF.egg-info/top_level.txt
```

### Comparing `quantylf-0.0.1/LICENSE` & `quantylf-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quantylf-0.0.1/PKG-INFO` & `quantylf-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantyLF
-Version: 0.0.1
+Version: 0.0.2
 Summary: QuantyLF is a libary to help manage Liegand Field simulations in Quanty.
 Home-page: https://github.com/CMM02/XPlotLib
 Author: Carl Magnus Meier
 Author-email: magnus.meier@outook.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quantylf-0.0.1/setup.cfg` & `quantylf-0.0.2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [metadata]
 name = QuantyLF
-version = 0.0.1
+version = 0.0.2
 author = Carl Magnus Meier
 author_email = magnus.meier@outook.de
 description = QuantyLF is a libary to help manage Liegand Field simulations in Quanty.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CMM02/XPlotLib
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
+include_package_data = True
 packages = find:
 python_requires = >=3.10
 install_requires = 
 	numpy
 
 [options.packages.find]
 where = src
```

### Comparing `quantylf-0.0.1/src/QuantyLF/QuantyLF.py` & `quantylf-0.0.2/src/QuantyLF/QuantyLF.py`

 * *Files identical despite different names*

### Comparing `quantylf-0.0.1/src/QuantyLF.egg-info/PKG-INFO` & `quantylf-0.0.2/src/QuantyLF.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantyLF
-Version: 0.0.1
+Version: 0.0.2
 Summary: QuantyLF is a libary to help manage Liegand Field simulations in Quanty.
 Home-page: https://github.com/CMM02/XPlotLib
 Author: Carl Magnus Meier
 Author-email: magnus.meier@outook.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

