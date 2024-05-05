# Comparing `tmp/quantylf-0.0.4.tar.gz` & `tmp/quantylf-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantylf-0.0.4.tar", last modified: Sun May  5 05:47:00 2024, max compression
+gzip compressed data, was "quantylf-0.0.5.tar", last modified: Sun May  5 05:49:54 2024, max compression
```

## Comparing `quantylf-0.0.4.tar` & `quantylf-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 05:47:00.777302 quantylf-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-05 05:46:52.000000 quantylf-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-05 05:47:00.777302 quantylf-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-05 05:46:52.000000 quantylf-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-05 05:46:52.000000 quantylf-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-05 05:47:00.777302 quantylf-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 05:47:00.777302 quantylf-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 05:47:00.777302 quantylf-0.0.4/src/QuantyLF/
--rw-r--r--   0 runner    (1001) docker     (127)    18551 2024-05-05 05:46:52.000000 quantylf-0.0.4/src/QuantyLF/QuantyLF.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 05:46:52.000000 quantylf-0.0.4/src/QuantyLF/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 05:47:00.777302 quantylf-0.0.4/src/QuantyLF.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-05 05:47:00.000000 quantylf-0.0.4/src/QuantyLF.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-05 05:47:00.000000 quantylf-0.0.4/src/QuantyLF.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 05:47:00.000000 quantylf-0.0.4/src/QuantyLF.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-05 05:47:00.000000 quantylf-0.0.4/src/QuantyLF.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-05 05:47:00.000000 quantylf-0.0.4/src/QuantyLF.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 05:49:54.786143 quantylf-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-05 05:49:50.000000 quantylf-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-05 05:49:54.786143 quantylf-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-05 05:49:50.000000 quantylf-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-05 05:49:50.000000 quantylf-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-05 05:49:54.790143 quantylf-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 05:49:54.786143 quantylf-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 05:49:54.786143 quantylf-0.0.5/src/QuantyLF/
+-rw-r--r--   0 runner    (1001) docker     (127)    18551 2024-05-05 05:49:50.000000 quantylf-0.0.5/src/QuantyLF/QuantyLF.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 05:49:50.000000 quantylf-0.0.5/src/QuantyLF/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 05:49:54.786143 quantylf-0.0.5/src/QuantyLF.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-05 05:49:54.000000 quantylf-0.0.5/src/QuantyLF.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-05 05:49:54.000000 quantylf-0.0.5/src/QuantyLF.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 05:49:54.000000 quantylf-0.0.5/src/QuantyLF.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-05 05:49:54.000000 quantylf-0.0.5/src/QuantyLF.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-05 05:49:54.000000 quantylf-0.0.5/src/QuantyLF.egg-info/top_level.txt
```

### Comparing `quantylf-0.0.4/LICENSE` & `quantylf-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `quantylf-0.0.4/PKG-INFO` & `quantylf-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantyLF
-Version: 0.0.4
+Version: 0.0.5
 Summary: QuantyLF is a libary to help manage Liegand Field simulations in Quanty.
 Home-page: https://github.com/CMM02/XPlotLib
 Author: Carl Magnus Meier
 Author-email: magnus.meier@outook.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quantylf-0.0.4/setup.cfg` & `quantylf-0.0.5/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = QuantyLF
-version = 0.0.4
+version = 0.0.5
 author = Carl Magnus Meier
 author_email = magnus.meier@outook.de
 description = QuantyLF is a libary to help manage Liegand Field simulations in Quanty.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CMM02/XPlotLib
 classifiers = 
@@ -20,15 +20,15 @@
 install_requires = 
 	numpy
 
 [options.packages.find]
 where = src
 
 [options.package_data]
-mypkg = 
+QuantyLF.cases = 
 	*.txt
 	*.lua
 
 [options.extras_require]
 dev = 
 	pytest
 	pytest-cov
```

### Comparing `quantylf-0.0.4/src/QuantyLF/QuantyLF.py` & `quantylf-0.0.5/src/QuantyLF/QuantyLF.py`

 * *Files identical despite different names*

### Comparing `quantylf-0.0.4/src/QuantyLF.egg-info/PKG-INFO` & `quantylf-0.0.5/src/QuantyLF.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantyLF
-Version: 0.0.4
+Version: 0.0.5
 Summary: QuantyLF is a libary to help manage Liegand Field simulations in Quanty.
 Home-page: https://github.com/CMM02/XPlotLib
 Author: Carl Magnus Meier
 Author-email: magnus.meier@outook.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```
