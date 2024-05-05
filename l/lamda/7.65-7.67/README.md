# Comparing `tmp/lamda-7.65.tar.gz` & `tmp/lamda-7.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lamda-7.65.tar", last modified: Sun Apr 21 03:11:32 2024, max compression
+gzip compressed data, was "dist/lamda-7.67.tar", last modified: Sun May  5 08:14:16 2024, max compression
```

## Comparing `lamda-7.65.tar` & `lamda-7.67.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 whoami    (1000) whoami    (1000)        0 2024-04-21 03:11:32.624092 lamda-7.65/
--rw-r--r--   0 whoami    (1000) whoami    (1000)      949 2024-04-21 03:11:32.624092 lamda-7.65/PKG-INFO
--rw-r--r--   0 whoami    (1000) whoami    (1000)     4295 2024-04-14 04:55:14.000000 lamda-7.65/README.md
-drwxrwxr-x   0 whoami    (1000) whoami    (1000)        0 2024-04-21 03:11:32.620092 lamda-7.65/lamda/
--rw-r--r--   0 whoami    (1000) whoami    (1000)      205 2024-04-21 03:02:42.000000 lamda-7.65/lamda/__init__.py
--rw-r--r--   0 whoami    (1000) whoami    (1000)      894 2023-12-11 03:08:30.000000 lamda-7.65/lamda/bcast.proto
--rw-r--r--   0 whoami    (1000) whoami    (1000)    73463 2024-04-08 07:40:06.000000 lamda-7.65/lamda/client.py
--rw-r--r--   0 whoami    (1000) whoami    (1000)     3167 2023-03-16 03:06:14.000000 lamda-7.65/lamda/const.py
--rw-r--r--   0 whoami    (1000) whoami    (1000)     1603 2023-12-11 03:24:23.000000 lamda-7.65/lamda/exceptions.py
-drwxrwxr-x   0 whoami    (1000) whoami    (1000)        0 2024-04-21 03:11:32.620092 lamda-7.65/lamda/google/
-drwxrwxr-x   0 whoami    (1000) whoami    (1000)        0 2024-04-21 03:11:32.624092 lamda-7.65/lamda/google/protobuf/
--rw-r--r--   0 whoami    (1000) whoami    (1000)     5916 2022-10-31 08:21:43.000000 lamda-7.65/lamda/google/protobuf/any.proto
--rw-r--r--   0 whoami    (1000) whoami    (1000)     7734 2022-10-31 08:21:43.000000 lamda-7.65/lamda/google/protobuf/api.proto
-drwxrwxr-x   0 whoami    (1000) whoami    (1000)        0 2024-04-21 03:11:32.624092 lamda-7.65/lamda/google/protobuf/compiler/
--rw-r--r--   0 whoami    (1000) whoami    (1000)     8754 2022-10-31 08:21:43.000000 lamda-7.65/lamda/google/protobuf/compiler/plugin.proto
--rw-r--r--   0 whoami    (1000) whoami    (1000)    37969 2022-10-31 08:21:43.000000 lamda-7.65/lamda/google/protobuf/descriptor.proto
--rw-r--r--   0 whoami    (1000) whoami    (1000)     4895 2022-10-31 08:21:43.000000 lamda-7.65/lamda/google/protobuf/duration.proto
--rw-r--r--   0 whoami    (1000) whoami    (1000)     2429 2022-10-31 08:21:43.000000 lamda-7.65/lamda/google/protobuf/empty.proto
--rw-r--r--   0 whoami    (1000) whoami    (1000)     8185 2022-10-31 08:21:43.000000 lamda-7.65/lamda/google/protobuf/field_mask.proto
--rw-r--r--   0 whoami    (1000) whoami    (1000)     2341 2022-10-31 08:21:43.000000 lamda-7.65/lamda/google/protobuf/source_context.proto
--rw-r--r--   0 whoami    (1000) whoami    (1000)     3778 2022-10-31 08:21:43.000000 lamda-7.65/lamda/google/protobuf/struct.proto
--rw-r--r--   0 whoami    (1000) whoami    (1000)     6459 2022-10-31 08:21:43.000000 lamda-7.65/lamda/google/protobuf/timestamp.proto
--rw-r--r--   0 whoami    (1000) whoami    (1000)     6126 2022-10-31 08:21:43.000000 lamda-7.65/lamda/google/protobuf/type.proto
--rw-r--r--   0 whoami    (1000) whoami    (1000)     4042 2022-10-31 08:21:43.000000 lamda-7.65/lamda/google/protobuf/wrappers.proto
-drwxrwxr-x   0 whoami    (1000) whoami    (1000)        0 2024-04-21 03:11:32.624092 lamda-7.65/lamda/rpc/
--rw-r--r--   0 whoami    (1000) whoami    (1000)     2393 2024-03-17 15:58:16.000000 lamda-7.65/lamda/rpc/application.proto
--rw-r--r--   0 whoami    (1000) whoami    (1000)      327 2024-04-08 07:34:20.000000 lamda-7.65/lamda/rpc/debug.proto
--rw-r--r--   0 whoami    (1000) whoami    (1000)      710 2024-01-06 00:45:39.000000 lamda-7.65/lamda/rpc/file.proto
--rw-r--r--   0 whoami    (1000) whoami    (1000)      391 2024-01-10 15:26:13.000000 lamda-7.65/lamda/rpc/policy.proto
--rw-r--r--   0 whoami    (1000) whoami    (1000)     2672 2024-01-13 06:01:07.000000 lamda-7.65/lamda/rpc/proxy.proto
--rw-r--r--   0 whoami    (1000) whoami    (1000)    11708 2024-04-08 07:39:31.000000 lamda-7.65/lamda/rpc/services.proto
--rw-r--r--   0 whoami    (1000) whoami    (1000)      478 2024-01-10 15:26:13.000000 lamda-7.65/lamda/rpc/settings.proto
--rw-r--r--   0 whoami    (1000) whoami    (1000)      609 2024-01-10 15:26:13.000000 lamda-7.65/lamda/rpc/shell.proto
--rw-r--r--   0 whoami    (1000) whoami    (1000)     2046 2024-01-10 15:26:13.000000 lamda-7.65/lamda/rpc/status.proto
--rw-r--r--   0 whoami    (1000) whoami    (1000)      393 2023-12-11 03:09:19.000000 lamda-7.65/lamda/rpc/storage.proto
--rw-r--r--   0 whoami    (1000) whoami    (1000)      434 2024-01-10 15:26:13.000000 lamda-7.65/lamda/rpc/types.proto
--rw-r--r--   0 whoami    (1000) whoami    (1000)    19642 2024-04-04 09:53:04.000000 lamda-7.65/lamda/rpc/uiautomator.proto
--rw-r--r--   0 whoami    (1000) whoami    (1000)     1299 2024-01-10 15:26:13.000000 lamda-7.65/lamda/rpc/util.proto
--rw-r--r--   0 whoami    (1000) whoami    (1000)     1935 2024-01-10 15:26:13.000000 lamda-7.65/lamda/rpc/wifi.proto
--rw-r--r--   0 whoami    (1000) whoami    (1000)     1007 2023-12-11 03:11:52.000000 lamda-7.65/lamda/types.py
-drwxrwxr-x   0 whoami    (1000) whoami    (1000)        0 2024-04-21 03:11:32.624092 lamda-7.65/lamda.egg-info/
--rw-r--r--   0 whoami    (1000) whoami    (1000)      949 2024-04-21 03:11:32.000000 lamda-7.65/lamda.egg-info/PKG-INFO
--rw-rw-r--   0 whoami    (1000) whoami    (1000)     1062 2024-04-21 03:11:32.000000 lamda-7.65/lamda.egg-info/SOURCES.txt
--rw-rw-r--   0 whoami    (1000) whoami    (1000)        1 2024-04-21 03:11:32.000000 lamda-7.65/lamda.egg-info/dependency_links.txt
--rw-rw-r--   0 whoami    (1000) whoami    (1000)        1 2024-04-21 03:11:32.000000 lamda-7.65/lamda.egg-info/not-zip-safe
--rw-rw-r--   0 whoami    (1000) whoami    (1000)      229 2024-04-21 03:11:32.000000 lamda-7.65/lamda.egg-info/requires.txt
--rw-rw-r--   0 whoami    (1000) whoami    (1000)        6 2024-04-21 03:11:32.000000 lamda-7.65/lamda.egg-info/top_level.txt
--rw-rw-r--   0 whoami    (1000) whoami    (1000)       38 2024-04-21 03:11:32.624092 lamda-7.65/setup.cfg
--rw-r--r--   0 whoami    (1000) whoami    (1000)     1635 2024-03-05 09:30:03.000000 lamda-7.65/setup.py
+drwxrwxr-x   0 whoami    (1000) whoami    (1000)        0 2024-05-05 08:14:16.539316 lamda-7.67/
+-rw-r--r--   0 whoami    (1000) whoami    (1000)      949 2024-05-05 08:14:16.539316 lamda-7.67/PKG-INFO
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     4295 2024-04-14 04:55:14.000000 lamda-7.67/README.md
+drwxrwxr-x   0 whoami    (1000) whoami    (1000)        0 2024-05-05 08:14:16.535316 lamda-7.67/lamda/
+-rw-r--r--   0 whoami    (1000) whoami    (1000)      205 2024-05-05 08:04:47.000000 lamda-7.67/lamda/__init__.py
+-rw-r--r--   0 whoami    (1000) whoami    (1000)      894 2023-12-11 03:08:30.000000 lamda-7.67/lamda/bcast.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)    73463 2024-04-08 07:40:06.000000 lamda-7.67/lamda/client.py
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     3167 2023-03-16 03:06:14.000000 lamda-7.67/lamda/const.py
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     1603 2023-12-11 03:24:23.000000 lamda-7.67/lamda/exceptions.py
+drwxrwxr-x   0 whoami    (1000) whoami    (1000)        0 2024-05-05 08:14:16.535316 lamda-7.67/lamda/google/
+drwxrwxr-x   0 whoami    (1000) whoami    (1000)        0 2024-05-05 08:14:16.539316 lamda-7.67/lamda/google/protobuf/
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     5916 2022-10-31 08:21:43.000000 lamda-7.67/lamda/google/protobuf/any.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     7734 2022-10-31 08:21:43.000000 lamda-7.67/lamda/google/protobuf/api.proto
+drwxrwxr-x   0 whoami    (1000) whoami    (1000)        0 2024-05-05 08:14:16.539316 lamda-7.67/lamda/google/protobuf/compiler/
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     8754 2022-10-31 08:21:43.000000 lamda-7.67/lamda/google/protobuf/compiler/plugin.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)    37969 2022-10-31 08:21:43.000000 lamda-7.67/lamda/google/protobuf/descriptor.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     4895 2022-10-31 08:21:43.000000 lamda-7.67/lamda/google/protobuf/duration.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     2429 2022-10-31 08:21:43.000000 lamda-7.67/lamda/google/protobuf/empty.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     8185 2022-10-31 08:21:43.000000 lamda-7.67/lamda/google/protobuf/field_mask.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     2341 2022-10-31 08:21:43.000000 lamda-7.67/lamda/google/protobuf/source_context.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     3778 2022-10-31 08:21:43.000000 lamda-7.67/lamda/google/protobuf/struct.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     6459 2022-10-31 08:21:43.000000 lamda-7.67/lamda/google/protobuf/timestamp.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     6126 2022-10-31 08:21:43.000000 lamda-7.67/lamda/google/protobuf/type.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     4042 2022-10-31 08:21:43.000000 lamda-7.67/lamda/google/protobuf/wrappers.proto
+drwxrwxr-x   0 whoami    (1000) whoami    (1000)        0 2024-05-05 08:14:16.539316 lamda-7.67/lamda/rpc/
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     2393 2024-03-17 15:58:16.000000 lamda-7.67/lamda/rpc/application.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)      327 2024-04-08 07:34:20.000000 lamda-7.67/lamda/rpc/debug.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)      710 2024-01-06 00:45:39.000000 lamda-7.67/lamda/rpc/file.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)      391 2024-01-10 15:26:13.000000 lamda-7.67/lamda/rpc/policy.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     2672 2024-01-13 06:01:07.000000 lamda-7.67/lamda/rpc/proxy.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)    11708 2024-04-08 07:39:31.000000 lamda-7.67/lamda/rpc/services.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)      478 2024-01-10 15:26:13.000000 lamda-7.67/lamda/rpc/settings.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)      609 2024-01-10 15:26:13.000000 lamda-7.67/lamda/rpc/shell.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     2046 2024-01-10 15:26:13.000000 lamda-7.67/lamda/rpc/status.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)      393 2023-12-11 03:09:19.000000 lamda-7.67/lamda/rpc/storage.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)      434 2024-01-10 15:26:13.000000 lamda-7.67/lamda/rpc/types.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)    19642 2024-04-04 09:53:04.000000 lamda-7.67/lamda/rpc/uiautomator.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     1299 2024-01-10 15:26:13.000000 lamda-7.67/lamda/rpc/util.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     1935 2024-01-10 15:26:13.000000 lamda-7.67/lamda/rpc/wifi.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     1007 2023-12-11 03:11:52.000000 lamda-7.67/lamda/types.py
+drwxrwxr-x   0 whoami    (1000) whoami    (1000)        0 2024-05-05 08:14:16.539316 lamda-7.67/lamda.egg-info/
+-rw-r--r--   0 whoami    (1000) whoami    (1000)      949 2024-05-05 08:14:16.000000 lamda-7.67/lamda.egg-info/PKG-INFO
+-rw-rw-r--   0 whoami    (1000) whoami    (1000)     1062 2024-05-05 08:14:16.000000 lamda-7.67/lamda.egg-info/SOURCES.txt
+-rw-rw-r--   0 whoami    (1000) whoami    (1000)        1 2024-05-05 08:14:16.000000 lamda-7.67/lamda.egg-info/dependency_links.txt
+-rw-rw-r--   0 whoami    (1000) whoami    (1000)        1 2024-05-05 08:14:16.000000 lamda-7.67/lamda.egg-info/not-zip-safe
+-rw-rw-r--   0 whoami    (1000) whoami    (1000)      229 2024-05-05 08:14:16.000000 lamda-7.67/lamda.egg-info/requires.txt
+-rw-rw-r--   0 whoami    (1000) whoami    (1000)        6 2024-05-05 08:14:16.000000 lamda-7.67/lamda.egg-info/top_level.txt
+-rw-rw-r--   0 whoami    (1000) whoami    (1000)       38 2024-05-05 08:14:16.539316 lamda-7.67/setup.cfg
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     1635 2024-03-05 09:30:03.000000 lamda-7.67/setup.py
```

### Comparing `lamda-7.65/PKG-INFO` & `lamda-7.67/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamda
-Version: 7.65
+Version: 7.67
 Summary: Android reverse engineering & automation framework
 Home-page: https://github.com/rev1si0n/lamda
 Author: rev1si0n
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
```

### Comparing `lamda-7.65/README.md` & `lamda-7.67/README.md`

 * *Files identical despite different names*

### Comparing `lamda-7.65/lamda/bcast.proto` & `lamda-7.67/lamda/bcast.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.65/lamda/client.py` & `lamda-7.67/lamda/client.py`

 * *Files identical despite different names*

### Comparing `lamda-7.65/lamda/const.py` & `lamda-7.67/lamda/const.py`

 * *Files identical despite different names*

### Comparing `lamda-7.65/lamda/exceptions.py` & `lamda-7.67/lamda/exceptions.py`

 * *Files identical despite different names*

### Comparing `lamda-7.65/lamda/google/protobuf/any.proto` & `lamda-7.67/lamda/google/protobuf/any.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.65/lamda/google/protobuf/api.proto` & `lamda-7.67/lamda/google/protobuf/api.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.65/lamda/google/protobuf/compiler/plugin.proto` & `lamda-7.67/lamda/google/protobuf/compiler/plugin.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.65/lamda/google/protobuf/descriptor.proto` & `lamda-7.67/lamda/google/protobuf/descriptor.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.65/lamda/google/protobuf/duration.proto` & `lamda-7.67/lamda/google/protobuf/duration.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.65/lamda/google/protobuf/empty.proto` & `lamda-7.67/lamda/google/protobuf/empty.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.65/lamda/google/protobuf/field_mask.proto` & `lamda-7.67/lamda/google/protobuf/field_mask.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.65/lamda/google/protobuf/source_context.proto` & `lamda-7.67/lamda/google/protobuf/source_context.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.65/lamda/google/protobuf/struct.proto` & `lamda-7.67/lamda/google/protobuf/struct.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.65/lamda/google/protobuf/timestamp.proto` & `lamda-7.67/lamda/google/protobuf/timestamp.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.65/lamda/google/protobuf/type.proto` & `lamda-7.67/lamda/google/protobuf/type.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.65/lamda/google/protobuf/wrappers.proto` & `lamda-7.67/lamda/google/protobuf/wrappers.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.65/lamda/rpc/application.proto` & `lamda-7.67/lamda/rpc/application.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.65/lamda/rpc/file.proto` & `lamda-7.67/lamda/rpc/file.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.65/lamda/rpc/proxy.proto` & `lamda-7.67/lamda/rpc/proxy.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.65/lamda/rpc/services.proto` & `lamda-7.67/lamda/rpc/services.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.65/lamda/rpc/shell.proto` & `lamda-7.67/lamda/rpc/shell.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.65/lamda/rpc/status.proto` & `lamda-7.67/lamda/rpc/status.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.65/lamda/rpc/uiautomator.proto` & `lamda-7.67/lamda/rpc/uiautomator.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.65/lamda/rpc/util.proto` & `lamda-7.67/lamda/rpc/util.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.65/lamda/rpc/wifi.proto` & `lamda-7.67/lamda/rpc/wifi.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.65/lamda/types.py` & `lamda-7.67/lamda/types.py`

 * *Files identical despite different names*

### Comparing `lamda-7.65/lamda.egg-info/PKG-INFO` & `lamda-7.67/lamda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamda
-Version: 7.65
+Version: 7.67
 Summary: Android reverse engineering & automation framework
 Home-page: https://github.com/rev1si0n/lamda
 Author: rev1si0n
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
```

### Comparing `lamda-7.65/lamda.egg-info/SOURCES.txt` & `lamda-7.67/lamda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lamda-7.65/setup.py` & `lamda-7.67/setup.py`

 * *Files identical despite different names*

