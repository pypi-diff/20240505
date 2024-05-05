# Comparing `tmp/flops_utils-0.3.3.tar.gz` & `tmp/flops_utils-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flops_utils-0.3.3.tar", max compression
+gzip compressed data, was "flops_utils-0.3.4.tar", max compression
```

## Comparing `flops_utils-0.3.3.tar` & `flops_utils-0.3.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        5 2024-04-24 16:17:22.069103 flops_utils-0.3.3/README.md
--rw-r--r--   0        0        0     2632 2024-05-05 08:11:33.371300 flops_utils-0.3.3/flops_utils/flops_ml_repo_templates.py
--rw-r--r--   0        0        0     1700 2024-04-25 13:42:32.054488 flops_utils-0.3.3/flops_utils/logging.py
--rw-r--r--   0        0        0      676 2024-05-04 13:58:57.723410 flops_utils-0.3.3/flops_utils/ml_model_flavor_wrapper.py
--rw-r--r--   0        0        0      500 2024-05-04 14:02:04.855413 flops_utils-0.3.3/flops_utils/ml_repo_files_wrapper.py
--rw-r--r--   0        0        0     1393 2024-04-24 16:17:22.077103 flops_utils-0.3.3/flops_utils/notifications.py
--rw-r--r--   0        0        0      395 2024-05-03 14:36:34.589614 flops_utils-0.3.3/flops_utils/types.py
--rw-r--r--   0        0        0      433 2024-05-05 08:11:43.651300 flops_utils-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 flops_utils-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0        5 2024-04-24 16:17:22.069103 flops_utils-0.3.4/README.md
+-rw-r--r--   0        0        0     1700 2024-04-25 13:42:32.054488 flops_utils-0.3.4/flops_utils/logging.py
+-rw-r--r--   0        0        0      676 2024-05-04 13:58:57.723410 flops_utils-0.3.4/flops_utils/ml_model_flavor_wrapper.py
+-rw-r--r--   0        0        0      500 2024-05-04 14:02:04.855413 flops_utils-0.3.4/flops_utils/ml_repo_files_wrapper.py
+-rw-r--r--   0        0        0     2632 2024-05-05 08:12:54.263299 flops_utils-0.3.4/flops_utils/ml_repo_templates.py
+-rw-r--r--   0        0        0     1393 2024-04-24 16:17:22.077103 flops_utils-0.3.4/flops_utils/notifications.py
+-rw-r--r--   0        0        0      395 2024-05-03 14:36:34.589614 flops_utils-0.3.4/flops_utils/types.py
+-rw-r--r--   0        0        0      433 2024-05-05 08:13:01.063299 flops_utils-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 flops_utils-0.3.4/PKG-INFO
```

### Comparing `flops_utils-0.3.3/flops_utils/flops_ml_repo_templates.py` & `flops_utils-0.3.4/flops_utils/ml_repo_templates.py`

 * *Files identical despite different names*

### Comparing `flops_utils-0.3.3/flops_utils/logging.py` & `flops_utils-0.3.4/flops_utils/logging.py`

 * *Files identical despite different names*

### Comparing `flops_utils-0.3.3/flops_utils/ml_model_flavor_wrapper.py` & `flops_utils-0.3.4/flops_utils/ml_model_flavor_wrapper.py`

 * *Files identical despite different names*

### Comparing `flops_utils-0.3.3/flops_utils/notifications.py` & `flops_utils-0.3.4/flops_utils/notifications.py`

 * *Files identical despite different names*

### Comparing `flops_utils-0.3.3/PKG-INFO` & `flops_utils-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flops_utils
-Version: 0.3.3
+Version: 0.3.4
 Summary: A library containing commong utilities for FLOps
 Author: Alexander Malyuk
 Author-email: malyuk.alexander1999@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

