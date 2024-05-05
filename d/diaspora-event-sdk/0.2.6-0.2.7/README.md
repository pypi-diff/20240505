# Comparing `tmp/diaspora-event-sdk-0.2.6.tar.gz` & `tmp/diaspora-event-sdk-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diaspora-event-sdk-0.2.6.tar", last modified: Sun May  5 03:07:32 2024, max compression
+gzip compressed data, was "diaspora-event-sdk-0.2.7.tar", last modified: Sun May  5 03:15:27 2024, max compression
```

## Comparing `diaspora-event-sdk-0.2.6.tar` & `diaspora-event-sdk-0.2.7.tar`

### file list

```diff
@@ -1,41 +1,49 @@
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-05 03:07:32.089226 diaspora-event-sdk-0.2.6/
--rw-r--r--   0 haochen    (501) staff       (20)    11357 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.6/LICENSE
--rw-r--r--   0 haochen    (501) staff       (20)       58 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.6/MANIFEST.in
--rw-r--r--   0 haochen    (501) staff       (20)     2108 2024-05-05 03:07:32.089098 diaspora-event-sdk-0.2.6/PKG-INFO
--rw-r--r--   0 haochen    (501) staff       (20)     1735 2024-05-03 15:59:19.000000 diaspora-event-sdk-0.2.6/README.md
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-05 03:07:32.086136 diaspora-event-sdk-0.2.6/diaspora_event_sdk/
--rw-r--r--   0 haochen    (501) staff       (20)      457 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/__init__.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-05 03:07:32.087563 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/
--rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/__init__.py
--rw-r--r--   0 haochen    (501) staff       (20)      204 2024-04-07 17:27:11.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/_environments.py
--rw-r--r--   0 haochen    (501) staff       (20)     3942 2024-05-05 02:43:38.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/aws_iam_msk.py
--rw-r--r--   0 haochen    (501) staff       (20)     8541 2024-05-03 15:08:27.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/client.py
--rw-r--r--   0 haochen    (501) staff       (20)      884 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/decorators.py
--rw-r--r--   0 haochen    (501) staff       (20)     4286 2024-05-05 02:43:19.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/kafka_client.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-05 03:07:32.088531 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/login_manager/
--rw-r--r--   0 haochen    (501) staff       (20)      239 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/login_manager/__init__.py
--rw-r--r--   0 haochen    (501) staff       (20)     1835 2024-04-08 03:36:21.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/login_manager/client_login.py
--rw-r--r--   0 haochen    (501) staff       (20)     1047 2024-04-08 03:39:08.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/login_manager/decorators.py
--rw-r--r--   0 haochen    (501) staff       (20)      430 2024-04-08 03:40:29.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/login_manager/globus_auth.py
--rw-r--r--   0 haochen    (501) staff       (20)      977 2024-04-08 03:45:19.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/login_manager/login_flow.py
--rw-r--r--   0 haochen    (501) staff       (20)     7040 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/login_manager/manager.py
--rw-r--r--   0 haochen    (501) staff       (20)      710 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/login_manager/protocol.py
--rw-r--r--   0 haochen    (501) staff       (20)     2094 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/login_manager/tokenstore.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-05 03:07:32.088740 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/utils/
--rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/utils/__init__.py
--rw-r--r--   0 haochen    (501) staff       (20)      470 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/utils/uuid_like.py
--rw-r--r--   0 haochen    (501) staff       (20)     4770 2024-05-03 14:59:36.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/web_client.py
--rw-r--r--   0 haochen    (501) staff       (20)       22 2024-05-05 03:06:39.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/version.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-05 03:07:32.086671 diaspora-event-sdk-0.2.6/diaspora_event_sdk.egg-info/
--rw-r--r--   0 haochen    (501) staff       (20)     2108 2024-05-05 03:07:32.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk.egg-info/PKG-INFO
--rw-r--r--   0 haochen    (501) staff       (20)     1106 2024-05-05 03:07:32.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 haochen    (501) staff       (20)        1 2024-05-05 03:07:32.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 haochen    (501) staff       (20)      110 2024-05-05 03:07:32.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk.egg-info/requires.txt
--rw-r--r--   0 haochen    (501) staff       (20)       25 2024-05-05 03:07:32.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk.egg-info/top_level.txt
--rw-r--r--   0 haochen    (501) staff       (20)       38 2024-05-05 03:07:32.089270 diaspora-event-sdk-0.2.6/setup.cfg
--rw-r--r--   0 haochen    (501) staff       (20)     1358 2024-05-05 03:05:11.000000 diaspora-event-sdk-0.2.6/setup.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-05 03:07:32.088846 diaspora-event-sdk-0.2.6/tests/
--rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.6/tests/__init__.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-05 03:07:32.088939 diaspora-event-sdk-0.2.6/tests/unit/
--rw-r--r--   0 haochen    (501) staff       (20)     3019 2024-04-08 02:07:35.000000 diaspora-event-sdk-0.2.6/tests/unit/test_client.py
--rw-r--r--   0 haochen    (501) staff       (20)      241 2024-04-08 03:50:13.000000 diaspora-event-sdk-0.2.6/tox.ini
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-05 03:15:27.504507 diaspora-event-sdk-0.2.7/
+-rw-r--r--   0 haochen    (501) staff       (20)    11357 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.7/LICENSE
+-rw-r--r--   0 haochen    (501) staff       (20)       58 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.7/MANIFEST.in
+-rw-r--r--   0 haochen    (501) staff       (20)     2108 2024-05-05 03:15:27.504381 diaspora-event-sdk-0.2.7/PKG-INFO
+-rw-r--r--   0 haochen    (501) staff       (20)     1735 2024-05-03 15:59:19.000000 diaspora-event-sdk-0.2.7/README.md
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-05 03:15:27.500461 diaspora-event-sdk-0.2.7/diaspora_event_sdk/
+-rw-r--r--   0 haochen    (501) staff       (20)      457 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.7/diaspora_event_sdk/__init__.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-05 03:15:27.501897 diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/
+-rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/__init__.py
+-rw-r--r--   0 haochen    (501) staff       (20)      204 2024-04-07 17:27:11.000000 diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/_environments.py
+-rw-r--r--   0 haochen    (501) staff       (20)     3942 2024-05-05 02:43:38.000000 diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/aws_iam_msk.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-05 03:15:27.502872 diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/botocore/
+-rw-r--r--   0 haochen    (501) staff       (20)        0 2024-05-05 03:13:17.000000 diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/botocore/__init__.py
+-rw-r--r--   0 haochen    (501) staff       (20)    18699 2024-05-05 02:53:21.000000 diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/botocore/auth.py
+-rw-r--r--   0 haochen    (501) staff       (20)     9344 2024-05-05 02:54:55.000000 diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/botocore/awsrequest.py
+-rw-r--r--   0 haochen    (501) staff       (20)    11055 2024-05-05 02:55:23.000000 diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/botocore/compat.py
+-rw-r--r--   0 haochen    (501) staff       (20)     2455 2024-05-05 02:55:47.000000 diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/botocore/credentials.py
+-rw-r--r--   0 haochen    (501) staff       (20)     2002 2024-05-05 02:55:55.000000 diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/botocore/exceptions.py
+-rw-r--r--   0 haochen    (501) staff       (20)     5370 2024-05-05 02:57:08.000000 diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/botocore/utils.py
+-rw-r--r--   0 haochen    (501) staff       (20)     8541 2024-05-03 15:08:27.000000 diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/client.py
+-rw-r--r--   0 haochen    (501) staff       (20)      884 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/decorators.py
+-rw-r--r--   0 haochen    (501) staff       (20)     4286 2024-05-05 02:43:19.000000 diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/kafka_client.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-05 03:15:27.503793 diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/login_manager/
+-rw-r--r--   0 haochen    (501) staff       (20)      239 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/login_manager/__init__.py
+-rw-r--r--   0 haochen    (501) staff       (20)     1835 2024-04-08 03:36:21.000000 diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/login_manager/client_login.py
+-rw-r--r--   0 haochen    (501) staff       (20)     1047 2024-04-08 03:39:08.000000 diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/login_manager/decorators.py
+-rw-r--r--   0 haochen    (501) staff       (20)      430 2024-04-08 03:40:29.000000 diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/login_manager/globus_auth.py
+-rw-r--r--   0 haochen    (501) staff       (20)      977 2024-04-08 03:45:19.000000 diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/login_manager/login_flow.py
+-rw-r--r--   0 haochen    (501) staff       (20)     7040 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/login_manager/manager.py
+-rw-r--r--   0 haochen    (501) staff       (20)      710 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/login_manager/protocol.py
+-rw-r--r--   0 haochen    (501) staff       (20)     2094 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/login_manager/tokenstore.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-05 03:15:27.504012 diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/utils/
+-rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/utils/__init__.py
+-rw-r--r--   0 haochen    (501) staff       (20)      470 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/utils/uuid_like.py
+-rw-r--r--   0 haochen    (501) staff       (20)     4770 2024-05-03 14:59:36.000000 diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/web_client.py
+-rw-r--r--   0 haochen    (501) staff       (20)       22 2024-05-05 03:15:22.000000 diaspora-event-sdk-0.2.7/diaspora_event_sdk/version.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-05 03:15:27.501029 diaspora-event-sdk-0.2.7/diaspora_event_sdk.egg-info/
+-rw-r--r--   0 haochen    (501) staff       (20)     2108 2024-05-05 03:15:27.000000 diaspora-event-sdk-0.2.7/diaspora_event_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 haochen    (501) staff       (20)     1412 2024-05-05 03:15:27.000000 diaspora-event-sdk-0.2.7/diaspora_event_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 haochen    (501) staff       (20)        1 2024-05-05 03:15:27.000000 diaspora-event-sdk-0.2.7/diaspora_event_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 haochen    (501) staff       (20)      110 2024-05-05 03:15:27.000000 diaspora-event-sdk-0.2.7/diaspora_event_sdk.egg-info/requires.txt
+-rw-r--r--   0 haochen    (501) staff       (20)       25 2024-05-05 03:15:27.000000 diaspora-event-sdk-0.2.7/diaspora_event_sdk.egg-info/top_level.txt
+-rw-r--r--   0 haochen    (501) staff       (20)       38 2024-05-05 03:15:27.504549 diaspora-event-sdk-0.2.7/setup.cfg
+-rw-r--r--   0 haochen    (501) staff       (20)     1358 2024-05-05 03:05:11.000000 diaspora-event-sdk-0.2.7/setup.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-05 03:15:27.504117 diaspora-event-sdk-0.2.7/tests/
+-rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.7/tests/__init__.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-05 03:15:27.504214 diaspora-event-sdk-0.2.7/tests/unit/
+-rw-r--r--   0 haochen    (501) staff       (20)     3019 2024-04-08 02:07:35.000000 diaspora-event-sdk-0.2.7/tests/unit/test_client.py
+-rw-r--r--   0 haochen    (501) staff       (20)      241 2024-04-08 03:50:13.000000 diaspora-event-sdk-0.2.7/tox.ini
```

### Comparing `diaspora-event-sdk-0.2.6/LICENSE` & `diaspora-event-sdk-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.6/PKG-INFO` & `diaspora-event-sdk-0.2.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diaspora-event-sdk
-Version: 0.2.6
+Version: 0.2.7
 Summary: SDK of Diaspora Event Fabric: Resilience-enabling services for science from HPC to edge
 Home-page: https://github.com/globus-labs/diaspora-event-sdk
 License: Apache 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: kafka-python
 Provides-Extra: test
```

### Comparing `diaspora-event-sdk-0.2.6/README.md` & `diaspora-event-sdk-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/aws_iam_msk.py` & `diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/aws_iam_msk.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/client.py` & `diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/client.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/decorators.py` & `diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/decorators.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/kafka_client.py` & `diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/kafka_client.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/login_manager/client_login.py` & `diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/login_manager/client_login.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/login_manager/decorators.py` & `diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/login_manager/decorators.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/login_manager/login_flow.py` & `diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/login_manager/login_flow.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/login_manager/manager.py` & `diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/login_manager/manager.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/login_manager/protocol.py` & `diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/login_manager/protocol.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/login_manager/tokenstore.py` & `diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/login_manager/tokenstore.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/web_client.py` & `diaspora-event-sdk-0.2.7/diaspora_event_sdk/sdk/web_client.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.6/diaspora_event_sdk.egg-info/PKG-INFO` & `diaspora-event-sdk-0.2.7/diaspora_event_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diaspora-event-sdk
-Version: 0.2.6
+Version: 0.2.7
 Summary: SDK of Diaspora Event Fabric: Resilience-enabling services for science from HPC to edge
 Home-page: https://github.com/globus-labs/diaspora-event-sdk
 License: Apache 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: kafka-python
 Provides-Extra: test
```

### Comparing `diaspora-event-sdk-0.2.6/diaspora_event_sdk.egg-info/SOURCES.txt` & `diaspora-event-sdk-0.2.7/diaspora_event_sdk.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,21 @@
 diaspora_event_sdk/sdk/__init__.py
 diaspora_event_sdk/sdk/_environments.py
 diaspora_event_sdk/sdk/aws_iam_msk.py
 diaspora_event_sdk/sdk/client.py
 diaspora_event_sdk/sdk/decorators.py
 diaspora_event_sdk/sdk/kafka_client.py
 diaspora_event_sdk/sdk/web_client.py
+diaspora_event_sdk/sdk/botocore/__init__.py
+diaspora_event_sdk/sdk/botocore/auth.py
+diaspora_event_sdk/sdk/botocore/awsrequest.py
+diaspora_event_sdk/sdk/botocore/compat.py
+diaspora_event_sdk/sdk/botocore/credentials.py
+diaspora_event_sdk/sdk/botocore/exceptions.py
+diaspora_event_sdk/sdk/botocore/utils.py
 diaspora_event_sdk/sdk/login_manager/__init__.py
 diaspora_event_sdk/sdk/login_manager/client_login.py
 diaspora_event_sdk/sdk/login_manager/decorators.py
 diaspora_event_sdk/sdk/login_manager/globus_auth.py
 diaspora_event_sdk/sdk/login_manager/login_flow.py
 diaspora_event_sdk/sdk/login_manager/manager.py
 diaspora_event_sdk/sdk/login_manager/protocol.py
```

### Comparing `diaspora-event-sdk-0.2.6/setup.py` & `diaspora-event-sdk-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.6/tests/unit/test_client.py` & `diaspora-event-sdk-0.2.7/tests/unit/test_client.py`

 * *Files identical despite different names*

