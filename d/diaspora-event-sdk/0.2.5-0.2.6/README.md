# Comparing `tmp/diaspora-event-sdk-0.2.5.tar.gz` & `tmp/diaspora-event-sdk-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diaspora-event-sdk-0.2.5.tar", last modified: Fri May  3 15:59:45 2024, max compression
+gzip compressed data, was "diaspora-event-sdk-0.2.6.tar", last modified: Sun May  5 03:07:32 2024, max compression
```

## Comparing `diaspora-event-sdk-0.2.5.tar` & `diaspora-event-sdk-0.2.6.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-03 15:59:45.162057 diaspora-event-sdk-0.2.5/
--rw-r--r--   0 haochen    (501) staff       (20)    11357 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.5/LICENSE
--rw-r--r--   0 haochen    (501) staff       (20)       58 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.5/MANIFEST.in
--rw-r--r--   0 haochen    (501) staff       (20)     2105 2024-05-03 15:59:45.161919 diaspora-event-sdk-0.2.5/PKG-INFO
--rw-r--r--   0 haochen    (501) staff       (20)     1735 2024-05-03 15:59:19.000000 diaspora-event-sdk-0.2.5/README.md
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-03 15:59:45.159171 diaspora-event-sdk-0.2.5/diaspora_event_sdk/
--rw-r--r--   0 haochen    (501) staff       (20)      457 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/__init__.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-03 15:59:45.160408 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/
--rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/__init__.py
--rw-r--r--   0 haochen    (501) staff       (20)      204 2024-04-07 17:27:11.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/_environments.py
--rw-r--r--   0 haochen    (501) staff       (20)     8541 2024-05-03 15:08:27.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/client.py
--rw-r--r--   0 haochen    (501) staff       (20)      884 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/decorators.py
--rw-r--r--   0 haochen    (501) staff       (20)     4361 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/kafka_client.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-03 15:59:45.161369 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/login_manager/
--rw-r--r--   0 haochen    (501) staff       (20)      239 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/login_manager/__init__.py
--rw-r--r--   0 haochen    (501) staff       (20)     1835 2024-04-08 03:36:21.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/login_manager/client_login.py
--rw-r--r--   0 haochen    (501) staff       (20)     1047 2024-04-08 03:39:08.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/login_manager/decorators.py
--rw-r--r--   0 haochen    (501) staff       (20)      430 2024-04-08 03:40:29.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/login_manager/globus_auth.py
--rw-r--r--   0 haochen    (501) staff       (20)      977 2024-04-08 03:45:19.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/login_manager/login_flow.py
--rw-r--r--   0 haochen    (501) staff       (20)     7040 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/login_manager/manager.py
--rw-r--r--   0 haochen    (501) staff       (20)      710 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/login_manager/protocol.py
--rw-r--r--   0 haochen    (501) staff       (20)     2094 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/login_manager/tokenstore.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-03 15:59:45.161565 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/utils/
--rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/utils/__init__.py
--rw-r--r--   0 haochen    (501) staff       (20)      470 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/utils/uuid_like.py
--rw-r--r--   0 haochen    (501) staff       (20)     4770 2024-05-03 14:59:36.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/web_client.py
--rw-r--r--   0 haochen    (501) staff       (20)       22 2024-05-03 14:44:05.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk/version.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-03 15:59:45.159692 diaspora-event-sdk-0.2.5/diaspora_event_sdk.egg-info/
--rw-r--r--   0 haochen    (501) staff       (20)     2105 2024-05-03 15:59:45.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk.egg-info/PKG-INFO
--rw-r--r--   0 haochen    (501) staff       (20)     1068 2024-05-03 15:59:45.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 haochen    (501) staff       (20)        1 2024-05-03 15:59:45.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 haochen    (501) staff       (20)      141 2024-05-03 15:59:45.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk.egg-info/requires.txt
--rw-r--r--   0 haochen    (501) staff       (20)       25 2024-05-03 15:59:45.000000 diaspora-event-sdk-0.2.5/diaspora_event_sdk.egg-info/top_level.txt
--rw-r--r--   0 haochen    (501) staff       (20)       38 2024-05-03 15:59:45.162103 diaspora-event-sdk-0.2.5/setup.cfg
--rw-r--r--   0 haochen    (501) staff       (20)     1389 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.5/setup.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-03 15:59:45.161672 diaspora-event-sdk-0.2.5/tests/
--rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.5/tests/__init__.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-03 15:59:45.161757 diaspora-event-sdk-0.2.5/tests/unit/
--rw-r--r--   0 haochen    (501) staff       (20)     3019 2024-04-08 02:07:35.000000 diaspora-event-sdk-0.2.5/tests/unit/test_client.py
--rw-r--r--   0 haochen    (501) staff       (20)      241 2024-04-08 03:50:13.000000 diaspora-event-sdk-0.2.5/tox.ini
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-05 03:07:32.089226 diaspora-event-sdk-0.2.6/
+-rw-r--r--   0 haochen    (501) staff       (20)    11357 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.6/LICENSE
+-rw-r--r--   0 haochen    (501) staff       (20)       58 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.6/MANIFEST.in
+-rw-r--r--   0 haochen    (501) staff       (20)     2108 2024-05-05 03:07:32.089098 diaspora-event-sdk-0.2.6/PKG-INFO
+-rw-r--r--   0 haochen    (501) staff       (20)     1735 2024-05-03 15:59:19.000000 diaspora-event-sdk-0.2.6/README.md
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-05 03:07:32.086136 diaspora-event-sdk-0.2.6/diaspora_event_sdk/
+-rw-r--r--   0 haochen    (501) staff       (20)      457 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/__init__.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-05 03:07:32.087563 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/
+-rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/__init__.py
+-rw-r--r--   0 haochen    (501) staff       (20)      204 2024-04-07 17:27:11.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/_environments.py
+-rw-r--r--   0 haochen    (501) staff       (20)     3942 2024-05-05 02:43:38.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/aws_iam_msk.py
+-rw-r--r--   0 haochen    (501) staff       (20)     8541 2024-05-03 15:08:27.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/client.py
+-rw-r--r--   0 haochen    (501) staff       (20)      884 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/decorators.py
+-rw-r--r--   0 haochen    (501) staff       (20)     4286 2024-05-05 02:43:19.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/kafka_client.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-05 03:07:32.088531 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/login_manager/
+-rw-r--r--   0 haochen    (501) staff       (20)      239 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/login_manager/__init__.py
+-rw-r--r--   0 haochen    (501) staff       (20)     1835 2024-04-08 03:36:21.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/login_manager/client_login.py
+-rw-r--r--   0 haochen    (501) staff       (20)     1047 2024-04-08 03:39:08.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/login_manager/decorators.py
+-rw-r--r--   0 haochen    (501) staff       (20)      430 2024-04-08 03:40:29.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/login_manager/globus_auth.py
+-rw-r--r--   0 haochen    (501) staff       (20)      977 2024-04-08 03:45:19.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/login_manager/login_flow.py
+-rw-r--r--   0 haochen    (501) staff       (20)     7040 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/login_manager/manager.py
+-rw-r--r--   0 haochen    (501) staff       (20)      710 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/login_manager/protocol.py
+-rw-r--r--   0 haochen    (501) staff       (20)     2094 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/login_manager/tokenstore.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-05 03:07:32.088740 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/utils/
+-rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/utils/__init__.py
+-rw-r--r--   0 haochen    (501) staff       (20)      470 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/utils/uuid_like.py
+-rw-r--r--   0 haochen    (501) staff       (20)     4770 2024-05-03 14:59:36.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/web_client.py
+-rw-r--r--   0 haochen    (501) staff       (20)       22 2024-05-05 03:06:39.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk/version.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-05 03:07:32.086671 diaspora-event-sdk-0.2.6/diaspora_event_sdk.egg-info/
+-rw-r--r--   0 haochen    (501) staff       (20)     2108 2024-05-05 03:07:32.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 haochen    (501) staff       (20)     1106 2024-05-05 03:07:32.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 haochen    (501) staff       (20)        1 2024-05-05 03:07:32.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 haochen    (501) staff       (20)      110 2024-05-05 03:07:32.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk.egg-info/requires.txt
+-rw-r--r--   0 haochen    (501) staff       (20)       25 2024-05-05 03:07:32.000000 diaspora-event-sdk-0.2.6/diaspora_event_sdk.egg-info/top_level.txt
+-rw-r--r--   0 haochen    (501) staff       (20)       38 2024-05-05 03:07:32.089270 diaspora-event-sdk-0.2.6/setup.cfg
+-rw-r--r--   0 haochen    (501) staff       (20)     1358 2024-05-05 03:05:11.000000 diaspora-event-sdk-0.2.6/setup.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-05 03:07:32.088846 diaspora-event-sdk-0.2.6/tests/
+-rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.6/tests/__init__.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-05 03:07:32.088939 diaspora-event-sdk-0.2.6/tests/unit/
+-rw-r--r--   0 haochen    (501) staff       (20)     3019 2024-04-08 02:07:35.000000 diaspora-event-sdk-0.2.6/tests/unit/test_client.py
+-rw-r--r--   0 haochen    (501) staff       (20)      241 2024-04-08 03:50:13.000000 diaspora-event-sdk-0.2.6/tox.ini
```

### Comparing `diaspora-event-sdk-0.2.5/LICENSE` & `diaspora-event-sdk-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.5/PKG-INFO` & `diaspora-event-sdk-0.2.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: diaspora-event-sdk
-Version: 0.2.5
+Version: 0.2.6
 Summary: SDK of Diaspora Event Fabric: Resilience-enabling services for science from HPC to edge
 Home-page: https://github.com/globus-labs/diaspora-event-sdk
-License: LICENSE
+License: Apache 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: kafka-python
 Provides-Extra: test
 License-File: LICENSE
 
 # Diaspora: Hybrid Event-Driven Architecture for Distributed Scientific Computing
```

### Comparing `diaspora-event-sdk-0.2.5/README.md` & `diaspora-event-sdk-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/client.py` & `diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/client.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/decorators.py` & `diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/decorators.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/kafka_client.py` & `diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/kafka_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import json
 from typing import Dict, Any
 import warnings
 import time
 
 from .client import Client
+from .aws_iam_msk import generate_auth_token
 
 # If kafka-python is not installed, Kafka functionality is not available through diaspora-event-sdk.
 kafka_available = True
 try:
     from kafka import KafkaProducer as KProd  # type: ignore[import,import-not-found]
     from kafka import KafkaConsumer as KCons  # type: ignore[import,import-not-found]
-    from aws_msk_iam_sasl_signer import MSKAuthTokenProvider  # type: ignore[import,import-not-found]
     import os
 
     class MSKTokenProvider:
         def token(self):
-            token, _ = MSKAuthTokenProvider.generate_auth_token("us-east-1")
+            token, _ = generate_auth_token("us-east-1")
             return token
-except ImportError:
+except Exception as e:
     kafka_available = False
 
 
 def get_diaspora_config(extra_configs: Dict[str, Any] = {}) -> Dict[str, Any]:
     """
     Retrieve default Diaspora event fabric connection configurations for Kafka clients.
     Merges default configurations with custom ones provided.
```

### Comparing `diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/login_manager/client_login.py` & `diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/login_manager/client_login.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/login_manager/decorators.py` & `diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/login_manager/decorators.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/login_manager/login_flow.py` & `diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/login_manager/login_flow.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/login_manager/manager.py` & `diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/login_manager/manager.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/login_manager/protocol.py` & `diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/login_manager/protocol.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/login_manager/tokenstore.py` & `diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/login_manager/tokenstore.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.5/diaspora_event_sdk/sdk/web_client.py` & `diaspora-event-sdk-0.2.6/diaspora_event_sdk/sdk/web_client.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.5/diaspora_event_sdk.egg-info/PKG-INFO` & `diaspora-event-sdk-0.2.6/diaspora_event_sdk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: diaspora-event-sdk
-Version: 0.2.5
+Version: 0.2.6
 Summary: SDK of Diaspora Event Fabric: Resilience-enabling services for science from HPC to edge
 Home-page: https://github.com/globus-labs/diaspora-event-sdk
-License: LICENSE
+License: Apache 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: kafka-python
 Provides-Extra: test
 License-File: LICENSE
 
 # Diaspora: Hybrid Event-Driven Architecture for Distributed Scientific Computing
```

### Comparing `diaspora-event-sdk-0.2.5/diaspora_event_sdk.egg-info/SOURCES.txt` & `diaspora-event-sdk-0.2.6/diaspora_event_sdk.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 diaspora_event_sdk.egg-info/PKG-INFO
 diaspora_event_sdk.egg-info/SOURCES.txt
 diaspora_event_sdk.egg-info/dependency_links.txt
 diaspora_event_sdk.egg-info/requires.txt
 diaspora_event_sdk.egg-info/top_level.txt
 diaspora_event_sdk/sdk/__init__.py
 diaspora_event_sdk/sdk/_environments.py
+diaspora_event_sdk/sdk/aws_iam_msk.py
 diaspora_event_sdk/sdk/client.py
 diaspora_event_sdk/sdk/decorators.py
 diaspora_event_sdk/sdk/kafka_client.py
 diaspora_event_sdk/sdk/web_client.py
 diaspora_event_sdk/sdk/login_manager/__init__.py
 diaspora_event_sdk/sdk/login_manager/client_login.py
 diaspora_event_sdk/sdk/login_manager/decorators.py
```

### Comparing `diaspora-event-sdk-0.2.5/setup.py` & `diaspora-event-sdk-0.2.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,17 +29,17 @@
     name="diaspora-event-sdk",
     version=parse_version(),
     description="SDK of Diaspora Event Fabric: Resilience-enabling services for science from HPC to edge",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     include_package_data=True,
-    license="LICENSE",
+    license="Apache 2.0",
     url="https://github.com/globus-labs/diaspora-event-sdk",
     install_requires=[
         "globus-sdk>=3.20.1,<4",
     ],
     extras_require={
-        "kafka-python": ["kafka-python", "aws-msk-iam-sasl-signer-python"],
+        "kafka-python": ["kafka-python"],
         "test": TEST_REQUIRES,
     },
 )
```

### Comparing `diaspora-event-sdk-0.2.5/tests/unit/test_client.py` & `diaspora-event-sdk-0.2.6/tests/unit/test_client.py`

 * *Files identical despite different names*

