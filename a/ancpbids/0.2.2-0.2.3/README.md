# Comparing `tmp/ancpbids-0.2.2.tar.gz` & `tmp/ancpbids-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ancpbids-0.2.2.tar", last modified: Wed May 10 14:56:13 2023, max compression
+gzip compressed data, was "ancpbids-0.2.3.tar", last modified: Sun May  5 13:01:30 2024, max compression
```

## Comparing `ancpbids-0.2.2.tar` & `ancpbids-0.2.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:13.618826 ancpbids-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-10 14:56:02.000000 ancpbids-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-10 14:56:02.000000 ancpbids-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-10 14:56:13.618826 ancpbids-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-10 14:56:02.000000 ancpbids-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:13.618826 ancpbids-0.2.2/ancpbids/
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-05-10 14:56:02.000000 ancpbids-0.2.2/ancpbids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-10 14:56:13.618826 ancpbids-0.2.2/ancpbids/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    32110 2023-05-10 14:56:02.000000 ancpbids-0.2.2/ancpbids/model_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    47198 2023-05-10 14:56:02.000000 ancpbids-0.2.2/ancpbids/model_v1_8_0.py
--rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-05-10 14:56:02.000000 ancpbids-0.2.2/ancpbids/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:13.614825 ancpbids-0.2.2/ancpbids/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:02.000000 ancpbids-0.2.2/ancpbids/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10839 2023-05-10 14:56:02.000000 ancpbids-0.2.2/ancpbids/plugins/plugin_dsloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-05-10 14:56:02.000000 ancpbids-0.2.2/ancpbids/plugins/plugin_dssaver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-10 14:56:02.000000 ancpbids-0.2.2/ancpbids/plugins/plugin_dsvalidator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-10 14:56:02.000000 ancpbids-0.2.2/ancpbids/plugins/plugin_files_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-10 14:56:02.000000 ancpbids-0.2.2/ancpbids/plugins/plugin_metadata_inheritance_principle.py
--rw-r--r--   0 runner    (1001) docker     (123)    12168 2023-05-10 14:56:02.000000 ancpbids-0.2.2/ancpbids/plugins/plugin_schema_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-10 14:56:02.000000 ancpbids-0.2.2/ancpbids/pybids_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-05-10 14:56:02.000000 ancpbids-0.2.2/ancpbids/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-05-10 14:56:02.000000 ancpbids-0.2.2/ancpbids/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:13.610825 ancpbids-0.2.2/ancpbids.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-10 14:56:13.000000 ancpbids-0.2.2/ancpbids.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-10 14:56:13.000000 ancpbids-0.2.2/ancpbids.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 14:56:13.000000 ancpbids-0.2.2/ancpbids.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 14:56:13.000000 ancpbids-0.2.2/ancpbids.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-10 14:56:02.000000 ancpbids-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:02.000000 ancpbids-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-10 14:56:13.618826 ancpbids-0.2.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      821 2023-05-10 14:56:02.000000 ancpbids-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:13.614825 ancpbids-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:02.000000 ancpbids-0.2.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:13.618826 ancpbids-0.2.2/tests/auto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:02.000000 ancpbids-0.2.2/tests/auto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-05-10 14:56:02.000000 ancpbids-0.2.2/tests/auto/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-10 14:56:02.000000 ancpbids-0.2.2/tests/auto/test_derivative.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-10 14:56:02.000000 ancpbids-0.2.2/tests/auto/test_fetch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-10 14:56:02.000000 ancpbids-0.2.2/tests/auto/test_ignored_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-05-10 14:56:02.000000 ancpbids-0.2.2/tests/auto/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-10 14:56:02.000000 ancpbids-0.2.2/tests/auto/test_regressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-10 14:56:02.000000 ancpbids-0.2.2/tests/auto/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-10 14:56:02.000000 ancpbids-0.2.2/tests/auto/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-05-10 14:56:02.000000 ancpbids-0.2.2/tests/auto/test_writing.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-10 14:56:02.000000 ancpbids-0.2.2/tests/base_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:13.618826 ancpbids-0.2.2/tests/manual/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:02.000000 ancpbids-0.2.2/tests/manual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-10 14:56:02.000000 ancpbids-0.2.2/tests/manual/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-10 14:56:02.000000 ancpbids-0.2.2/tests/manual/test_performance_regressions.py
--rw-r--r--   0 runner    (1001) docker     (123)    78254 2023-05-10 14:56:02.000000 ancpbids-0.2.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:01:30.710224 ancpbids-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-05 13:01:21.000000 ancpbids-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-05 13:01:21.000000 ancpbids-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-05 13:01:30.714224 ancpbids-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-05 13:01:21.000000 ancpbids-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:01:30.714224 ancpbids-0.2.3/ancpbids/
+-rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-05-05 13:01:21.000000 ancpbids-0.2.3/ancpbids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-05 13:01:30.714224 ancpbids-0.2.3/ancpbids/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32110 2024-05-05 13:01:21.000000 ancpbids-0.2.3/ancpbids/model_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47198 2024-05-05 13:01:21.000000 ancpbids-0.2.3/ancpbids/model_v1_8_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-05-05 13:01:21.000000 ancpbids-0.2.3/ancpbids/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:01:30.710224 ancpbids-0.2.3/ancpbids/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 13:01:21.000000 ancpbids-0.2.3/ancpbids/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10839 2024-05-05 13:01:21.000000 ancpbids-0.2.3/ancpbids/plugins/plugin_dsloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-05-05 13:01:21.000000 ancpbids-0.2.3/ancpbids/plugins/plugin_dssaver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-05 13:01:21.000000 ancpbids-0.2.3/ancpbids/plugins/plugin_dsvalidator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-05 13:01:21.000000 ancpbids-0.2.3/ancpbids/plugins/plugin_files_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-05 13:01:21.000000 ancpbids-0.2.3/ancpbids/plugins/plugin_metadata_inheritance_principle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12168 2024-05-05 13:01:21.000000 ancpbids-0.2.3/ancpbids/plugins/plugin_schema_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-05-05 13:01:21.000000 ancpbids-0.2.3/ancpbids/pybids_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12077 2024-05-05 13:01:21.000000 ancpbids-0.2.3/ancpbids/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-05-05 13:01:21.000000 ancpbids-0.2.3/ancpbids/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:01:30.710224 ancpbids-0.2.3/ancpbids.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-05 13:01:30.000000 ancpbids-0.2.3/ancpbids.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-05 13:01:30.000000 ancpbids-0.2.3/ancpbids.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 13:01:30.000000 ancpbids-0.2.3/ancpbids.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-05 13:01:30.000000 ancpbids-0.2.3/ancpbids.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-05 13:01:21.000000 ancpbids-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 13:01:21.000000 ancpbids-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-05 13:01:30.714224 ancpbids-0.2.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      821 2024-05-05 13:01:21.000000 ancpbids-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:01:30.710224 ancpbids-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 13:01:21.000000 ancpbids-0.2.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:01:30.710224 ancpbids-0.2.3/tests/auto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 13:01:21.000000 ancpbids-0.2.3/tests/auto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8429 2024-05-05 13:01:21.000000 ancpbids-0.2.3/tests/auto/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-05 13:01:21.000000 ancpbids-0.2.3/tests/auto/test_derivative.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-05 13:01:21.000000 ancpbids-0.2.3/tests/auto/test_fetch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-05 13:01:21.000000 ancpbids-0.2.3/tests/auto/test_ignored_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5496 2024-05-05 13:01:21.000000 ancpbids-0.2.3/tests/auto/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-05 13:01:21.000000 ancpbids-0.2.3/tests/auto/test_regressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-05 13:01:21.000000 ancpbids-0.2.3/tests/auto/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-05 13:01:21.000000 ancpbids-0.2.3/tests/auto/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-05-05 13:01:21.000000 ancpbids-0.2.3/tests/auto/test_writing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-05 13:01:21.000000 ancpbids-0.2.3/tests/base_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:01:30.710224 ancpbids-0.2.3/tests/manual/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 13:01:22.000000 ancpbids-0.2.3/tests/manual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-05 13:01:22.000000 ancpbids-0.2.3/tests/manual/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-05 13:01:22.000000 ancpbids-0.2.3/tests/manual/test_performance_regressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78254 2024-05-05 13:01:22.000000 ancpbids-0.2.3/versioneer.py
```

### Comparing `ancpbids-0.2.2/LICENSE` & `ancpbids-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.2/PKG-INFO` & `ancpbids-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ancpbids
-Version: 0.2.2
+Version: 0.2.3
 Summary: Read/write/validate/query BIDS datasets
 Home-page: https://github.com/ANCPLabOldenburg/ancp-bids
 Author: Erdal Karaca
 Author-email: erdal.karaca.de@gmail.com
 Maintainer: ANCP Lab, University of Oldenburg
 Maintainer-email: currentancp@listserv.uni-oldenburg.de
 License: MIT
```

### Comparing `ancpbids-0.2.2/README.md` & `ancpbids-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.2/ancpbids/__init__.py` & `ancpbids-0.2.3/ancpbids/__init__.py`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.2/ancpbids/model_base.py` & `ancpbids-0.2.3/ancpbids/model_base.py`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.2/ancpbids/model_v1_8_0.py` & `ancpbids-0.2.3/ancpbids/model_v1_8_0.py`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.2/ancpbids/plugin.py` & `ancpbids-0.2.3/ancpbids/plugin.py`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.2/ancpbids/plugins/plugin_dsloader.py` & `ancpbids-0.2.3/ancpbids/plugins/plugin_dsloader.py`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.2/ancpbids/plugins/plugin_dssaver.py` & `ancpbids-0.2.3/ancpbids/plugins/plugin_dssaver.py`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.2/ancpbids/plugins/plugin_dsvalidator.py` & `ancpbids-0.2.3/ancpbids/plugins/plugin_dsvalidator.py`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.2/ancpbids/plugins/plugin_files_handlers.py` & `ancpbids-0.2.3/ancpbids/plugins/plugin_files_handlers.py`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.2/ancpbids/plugins/plugin_metadata_inheritance_principle.py` & `ancpbids-0.2.3/ancpbids/plugins/plugin_metadata_inheritance_principle.py`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.2/ancpbids/plugins/plugin_schema_patches.py` & `ancpbids-0.2.3/ancpbids/plugins/plugin_schema_patches.py`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.2/ancpbids/pybids_compat.py` & `ancpbids-0.2.3/ancpbids/pybids_compat.py`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.2/ancpbids/query.py` & `ancpbids-0.2.3/ancpbids/query.py`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.2/ancpbids/utils.py` & `ancpbids-0.2.3/ancpbids/utils.py`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.2/ancpbids.egg-info/PKG-INFO` & `ancpbids-0.2.3/ancpbids.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ancpbids
-Version: 0.2.2
+Version: 0.2.3
 Summary: Read/write/validate/query BIDS datasets
 Home-page: https://github.com/ANCPLabOldenburg/ancp-bids
 Author: Erdal Karaca
 Author-email: erdal.karaca.de@gmail.com
 Maintainer: ANCP Lab, University of Oldenburg
 Maintainer-email: currentancp@listserv.uni-oldenburg.de
 License: MIT
```

### Comparing `ancpbids-0.2.2/ancpbids.egg-info/SOURCES.txt` & `ancpbids-0.2.3/ancpbids.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.2/setup.cfg` & `ancpbids-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.2/setup.py` & `ancpbids-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.2/tests/auto/test_basic.py` & `ancpbids-0.2.3/tests/auto/test_basic.py`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.2/tests/auto/test_derivative.py` & `ancpbids-0.2.3/tests/auto/test_derivative.py`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.2/tests/auto/test_fetch_dataset.py` & `ancpbids-0.2.3/tests/auto/test_fetch_dataset.py`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.2/tests/auto/test_ignored_resources.py` & `ancpbids-0.2.3/tests/auto/test_ignored_resources.py`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.2/tests/auto/test_query.py` & `ancpbids-0.2.3/tests/auto/test_query.py`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.2/tests/auto/test_regressions.py` & `ancpbids-0.2.3/tests/auto/test_regressions.py`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.2/tests/auto/test_schema.py` & `ancpbids-0.2.3/tests/auto/test_schema.py`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.2/tests/auto/test_validation.py` & `ancpbids-0.2.3/tests/auto/test_validation.py`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.2/tests/auto/test_writing.py` & `ancpbids-0.2.3/tests/auto/test_writing.py`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.2/tests/base_test_case.py` & `ancpbids-0.2.3/tests/base_test_case.py`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.2/tests/manual/test_benchmark.py` & `ancpbids-0.2.3/tests/manual/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `ancpbids-0.2.2/versioneer.py` & `ancpbids-0.2.3/versioneer.py`

 * *Files identical despite different names*

