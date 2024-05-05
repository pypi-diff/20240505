# Comparing `tmp/total_connect_client-2024.4.tar.gz` & `tmp/total_connect_client-2024.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "total_connect_client-2024.4.tar", last modified: Sun Apr 28 23:00:17 2024, max compression
+gzip compressed data, was "total_connect_client-2024.5.tar", last modified: Sun May  5 00:13:23 2024, max compression
```

## Comparing `total_connect_client-2024.4.tar` & `total_connect_client-2024.5.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-28 23:00:17.119065 total_connect_client-2024.4/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1075 2023-02-24 21:24:49.000000 total_connect_client-2024.4/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7532 2024-04-28 23:00:17.119065 total_connect_client-2024.4/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6893 2023-11-30 02:02:31.000000 total_connect_client-2024.4/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3275 2024-04-28 23:00:07.000000 total_connect_client-2024.4/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2024-04-28 23:00:17.119065 total_connect_client-2024.4/setup.cfg
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-28 23:00:17.118065 total_connect_client-2024.4/tests/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7368 2023-06-29 00:24:30.000000 total_connect_client-2024.4/tests/test_client_arm_disarm.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2774 2023-02-24 21:24:49.000000 total_connect_client-2024.4/tests/test_client_authenticate.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2705 2023-02-24 21:24:49.000000 total_connect_client-2024.4/tests/test_client_get_panel_meta_data.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3445 2023-06-29 00:24:30.000000 total_connect_client-2024.4/tests/test_client_init.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2481 2023-04-29 22:02:21.000000 total_connect_client-2024.4/tests/test_client_misc.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6616 2023-06-29 00:24:30.000000 total_connect_client-2024.4/tests/test_client_request.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1867 2023-02-24 21:24:49.000000 total_connect_client-2024.4/tests/test_client_validate_usercode.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3332 2023-11-30 02:02:31.000000 total_connect_client-2024.4/tests/test_client_zone_bypass.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      467 2023-02-24 21:24:49.000000 total_connect_client-2024.4/tests/test_device.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8037 2024-04-28 22:08:42.000000 total_connect_client-2024.4/tests/test_location.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1996 2023-11-30 02:02:31.000000 total_connect_client-2024.4/tests/test_location_arm_disarm.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4071 2023-06-29 00:24:30.000000 total_connect_client-2024.4/tests/test_partition.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1299 2023-02-24 21:24:49.000000 total_connect_client-2024.4/tests/test_user.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14210 2023-11-30 02:02:31.000000 total_connect_client-2024.4/tests/test_zone.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-28 23:00:17.118065 total_connect_client-2024.4/total_connect_client/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      699 2023-02-24 21:24:49.000000 total_connect_client-2024.4/total_connect_client/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      516 2023-02-24 21:24:49.000000 total_connect_client-2024.4/total_connect_client/__main__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      823 2023-02-24 21:24:49.000000 total_connect_client-2024.4/total_connect_client/arm.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1219 2023-11-30 02:02:31.000000 total_connect_client-2024.4/total_connect_client/bypass_all.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    15022 2023-02-24 22:00:19.000000 total_connect_client-2024.4/total_connect_client/client.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5732 2024-04-28 22:07:55.000000 total_connect_client-2024.4/total_connect_client/const.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2951 2023-12-02 01:55:12.000000 total_connect_client-2024.4/total_connect_client/device.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      600 2023-02-24 21:24:49.000000 total_connect_client-2024.4/total_connect_client/disarm.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1370 2023-02-24 21:59:19.000000 total_connect_client-2024.4/total_connect_client/exceptions.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-28 23:00:17.119065 total_connect_client-2024.4/total_connect_client/live/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      762 2023-02-24 21:24:49.000000 total_connect_client-2024.4/total_connect_client/live/auto_bypass.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4081 2023-12-02 02:37:34.000000 total_connect_client-2024.4/total_connect_client/live/experimental.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1710 2023-11-30 02:02:31.000000 total_connect_client-2024.4/total_connect_client/live/zwave.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    18745 2023-12-02 02:40:27.000000 total_connect_client-2024.4/total_connect_client/location.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2236 2023-02-24 21:24:49.000000 total_connect_client-2024.4/total_connect_client/partition.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      889 2023-05-06 16:48:15.000000 total_connect_client-2024.4/total_connect_client/sync.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2095 2023-02-24 21:24:49.000000 total_connect_client-2024.4/total_connect_client/user.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9604 2023-11-30 02:02:31.000000 total_connect_client-2024.4/total_connect_client/zone.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-28 23:00:17.119065 total_connect_client-2024.4/total_connect_client.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7532 2024-04-28 23:00:17.000000 total_connect_client-2024.4/total_connect_client.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1210 2024-04-28 23:00:17.000000 total_connect_client-2024.4/total_connect_client.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-04-28 23:00:17.000000 total_connect_client-2024.4/total_connect_client.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       12 2024-04-28 23:00:17.000000 total_connect_client-2024.4/total_connect_client.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       21 2024-04-28 23:00:17.000000 total_connect_client-2024.4/total_connect_client.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-05 00:13:23.549923 total_connect_client-2024.5/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1075 2023-02-24 21:24:49.000000 total_connect_client-2024.5/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7533 2024-05-05 00:13:23.549923 total_connect_client-2024.5/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6893 2023-11-30 02:02:31.000000 total_connect_client-2024.5/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3348 2024-05-05 00:13:10.000000 total_connect_client-2024.5/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2024-05-05 00:13:23.549923 total_connect_client-2024.5/setup.cfg
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-05 00:13:23.548923 total_connect_client-2024.5/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7368 2023-06-29 00:24:30.000000 total_connect_client-2024.5/tests/test_client_arm_disarm.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2774 2023-02-24 21:24:49.000000 total_connect_client-2024.5/tests/test_client_authenticate.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2705 2023-02-24 21:24:49.000000 total_connect_client-2024.5/tests/test_client_get_panel_meta_data.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3445 2023-06-29 00:24:30.000000 total_connect_client-2024.5/tests/test_client_init.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2481 2023-04-29 22:02:21.000000 total_connect_client-2024.5/tests/test_client_misc.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6616 2023-06-29 00:24:30.000000 total_connect_client-2024.5/tests/test_client_request.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1867 2023-02-24 21:24:49.000000 total_connect_client-2024.5/tests/test_client_validate_usercode.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3332 2023-11-30 02:02:31.000000 total_connect_client-2024.5/tests/test_client_zone_bypass.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      467 2023-02-24 21:24:49.000000 total_connect_client-2024.5/tests/test_device.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8037 2024-04-28 22:08:42.000000 total_connect_client-2024.5/tests/test_location.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1996 2023-11-30 02:02:31.000000 total_connect_client-2024.5/tests/test_location_arm_disarm.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4071 2023-06-29 00:24:30.000000 total_connect_client-2024.5/tests/test_partition.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1299 2023-02-24 21:24:49.000000 total_connect_client-2024.5/tests/test_user.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    14210 2023-11-30 02:02:31.000000 total_connect_client-2024.5/tests/test_zone.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-05 00:13:23.548923 total_connect_client-2024.5/total_connect_client/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      699 2023-02-24 21:24:49.000000 total_connect_client-2024.5/total_connect_client/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      516 2023-02-24 21:24:49.000000 total_connect_client-2024.5/total_connect_client/__main__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      823 2023-02-24 21:24:49.000000 total_connect_client-2024.5/total_connect_client/arm.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1219 2023-11-30 02:02:31.000000 total_connect_client-2024.5/total_connect_client/bypass_all.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-05 00:13:23.549923 total_connect_client-2024.5/total_connect_client/cache/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    19204 2005-06-27 09:39:48.000000 total_connect_client-2024.5/total_connect_client/cache/soap-encodings-schemas.xmlsoap.org.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    15786 2024-05-04 06:53:27.000000 total_connect_client-2024.5/total_connect_client/client.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5732 2024-04-28 22:07:55.000000 total_connect_client-2024.5/total_connect_client/const.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2951 2023-12-02 01:55:12.000000 total_connect_client-2024.5/total_connect_client/device.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      600 2023-02-24 21:24:49.000000 total_connect_client-2024.5/total_connect_client/disarm.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1370 2023-02-24 21:59:19.000000 total_connect_client-2024.5/total_connect_client/exceptions.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-05 00:13:23.549923 total_connect_client-2024.5/total_connect_client/live/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      762 2023-02-24 21:24:49.000000 total_connect_client-2024.5/total_connect_client/live/auto_bypass.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4081 2023-12-02 02:37:34.000000 total_connect_client-2024.5/total_connect_client/live/experimental.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1710 2023-11-30 02:02:31.000000 total_connect_client-2024.5/total_connect_client/live/zwave.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    18745 2023-12-02 02:40:27.000000 total_connect_client-2024.5/total_connect_client/location.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2236 2023-02-24 21:24:49.000000 total_connect_client-2024.5/total_connect_client/partition.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      889 2023-05-06 16:48:15.000000 total_connect_client-2024.5/total_connect_client/sync.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2095 2023-02-24 21:24:49.000000 total_connect_client-2024.5/total_connect_client/user.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9604 2023-11-30 02:02:31.000000 total_connect_client-2024.5/total_connect_client/zone.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-05 00:13:23.549923 total_connect_client-2024.5/total_connect_client.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7533 2024-05-05 00:13:23.000000 total_connect_client-2024.5/total_connect_client.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1276 2024-05-05 00:13:23.000000 total_connect_client-2024.5/total_connect_client.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-05-05 00:13:23.000000 total_connect_client-2024.5/total_connect_client.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       12 2024-05-05 00:13:23.000000 total_connect_client-2024.5/total_connect_client.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       21 2024-05-05 00:13:23.000000 total_connect_client-2024.5/total_connect_client.egg-info/top_level.txt
```

### Comparing `total_connect_client-2024.4/LICENSE` & `total_connect_client-2024.5/LICENSE`

 * *Files identical despite different names*

### Comparing `total_connect_client-2024.4/PKG-INFO` & `total_connect_client-2024.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: total_connect_client
-Version: 2024.4
+Version: 2024.5
 Summary: Interact with Total Connect 2 alarm systems
 Author-email: "Craig J. Midwinter" <craig.j.midwinter@gmail.com>
 Project-URL: Homepage, https://github.com/craigjmidwinter/total-connect-client
 Project-URL: Bug Tracker, https://github.com/craigjmidwinter/total-connect-client/issues
 Keywords: alarm,TotalConnect
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: zeep>=4.2.1
 
 # Total-Connect-Client
 Total-Connect-Client is a python client for interacting with the [TotalConnect2](https://totalconnect2.com) alarm system.
```

### Comparing `total_connect_client-2024.4/README.md` & `total_connect_client-2024.5/README.md`

 * *Files identical despite different names*

### Comparing `total_connect_client-2024.4/pyproject.toml` & `total_connect_client-2024.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name="total_connect_client"
-version="2024.4"
+version="2024.5"
 authors = [
   { name="Craig J. Midwinter", email="craig.j.midwinter@gmail.com" },
 ]
 description="Interact with Total Connect 2 alarm systems"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 keywords=["alarm", "TotalConnect"]
 dependencies=["zeep>=4.2.1"]
@@ -29,26 +29,29 @@
 omit = [
     "total_connect_client/live*.py"
 ]
 
 [tool.pylint."messages control"]
 disable = ["use-symbolic-message-instead", "too-few-public-methods", "too-many-instance-attributes", "logging-fstring-interpolation", "missing-function-docstring", "missing-class-docstring", "protected-access", "line-too-long", "duplicate-code"]
 
+[tool.setuptools.package-data]
+total_connect_client = ["cache/*.txt"]
+
 [tool.tox]
 legacy_tox_ini = """
 
    [tox]
     requires = 
       tox>=4
       virtualenv>=20.26
 
     env_list = 
         build
         lint
-        py{39,310,311,312}
+        py{310,311,312,313}
 
     #skip_missing_interpreters = True
 
     [testenv]
     setenv =
         LANG=en_US.UTF-8
         PYTHONPATH = {toxinidir}
```

### Comparing `total_connect_client-2024.4/tests/test_client_arm_disarm.py` & `total_connect_client-2024.5/tests/test_client_arm_disarm.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2024.4/tests/test_client_authenticate.py` & `total_connect_client-2024.5/tests/test_client_authenticate.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2024.4/tests/test_client_get_panel_meta_data.py` & `total_connect_client-2024.5/tests/test_client_get_panel_meta_data.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2024.4/tests/test_client_init.py` & `total_connect_client-2024.5/tests/test_client_init.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2024.4/tests/test_client_misc.py` & `total_connect_client-2024.5/tests/test_client_misc.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2024.4/tests/test_client_request.py` & `total_connect_client-2024.5/tests/test_client_request.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2024.4/tests/test_client_validate_usercode.py` & `total_connect_client-2024.5/tests/test_client_validate_usercode.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2024.4/tests/test_client_zone_bypass.py` & `total_connect_client-2024.5/tests/test_client_zone_bypass.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2024.4/tests/test_location.py` & `total_connect_client-2024.5/tests/test_location.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2024.4/tests/test_location_arm_disarm.py` & `total_connect_client-2024.5/tests/test_location_arm_disarm.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2024.4/tests/test_partition.py` & `total_connect_client-2024.5/tests/test_partition.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2024.4/tests/test_user.py` & `total_connect_client-2024.5/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2024.4/tests/test_zone.py` & `total_connect_client-2024.5/tests/test_zone.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2024.4/total_connect_client/__init__.py` & `total_connect_client-2024.5/total_connect_client/__init__.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2024.4/total_connect_client/__main__.py` & `total_connect_client-2024.5/total_connect_client/__main__.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2024.4/total_connect_client/arm.py` & `total_connect_client-2024.5/total_connect_client/arm.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2024.4/total_connect_client/bypass_all.py` & `total_connect_client-2024.5/total_connect_client/bypass_all.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2024.4/total_connect_client/client.py` & `total_connect_client-2024.5/total_connect_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,24 @@
 for location in client.locations:
     ### do stuff with this location
 """
 
 import logging
 import ssl
 import time
+from importlib import resources as impresources
 
+import requests
+import urllib3.poolmanager
 import zeep
 import zeep.cache
-from zeep.exceptions import Fault as ZeepFault
 import zeep.transports
-import requests
-import urllib3.poolmanager
+from zeep.exceptions import Fault as ZeepFault
 
+from . import cache as cache_folder
 from .const import ArmType, _ResultCode
 from .exceptions import (
     AuthenticationError,
     BadResultCodeError,
     FailedToBypassZone,
     FeatureNotSupportedError,
     InvalidSessionError,
@@ -33,35 +35,43 @@
     UsercodeUnavailable,
 )
 from .location import TotalConnectLocation
 from .user import TotalConnectUser
 
 DEFAULT_USERCODE = "-1"
 
+SCHEMAS_TO_CACHE = {
+    "https://schemas.xmlsoap.org/soap/encoding/": "soap-encodings-schemas.xmlsoap.org.txt",
+}
+
 LOGGER = logging.getLogger(__name__)
 
 
 class _SslContextAdapter(requests.adapters.HTTPAdapter):
     """Makes Zeep use our ssl_context."""
+
     def __init__(self, ssl_context, **kwargs):
         self.ssl_context = ssl_context
         super().__init__(**kwargs)
 
     def init_poolmanager(self, num_pools, maxsize, block=False):
         self.poolmanager = urllib3.poolmanager.PoolManager(
-            num_pools=num_pools, maxsize=maxsize,
-            block=block, ssl_context=self.ssl_context)
+            num_pools=num_pools,
+            maxsize=maxsize,
+            block=block,
+            ssl_context=self.ssl_context,
+        )
 
 
 class TotalConnectClient:
     """Client for Total Connect."""
 
     TIMEOUT = 60  # seconds until SOAP I/O will fail
 
-    def __init__(         # pylint: disable=too-many-arguments
+    def __init__(  # pylint: disable=too-many-arguments
         self,
         username,
         password,
         usercodes=None,
         auto_bypass_battery=False,
         retry_delay=6,  # seconds between retries
     ):
@@ -91,15 +101,15 @@
     def locations(self):
         """Raises an exception if the panel cannot be reached to retrieve
         metadata or details. This can be retried later and will succeed
         if/when the panel becomes reachable.
         """
         # to_fetch is needed because items() is invalidated by del
         to_fetch = list(self._locations_unfetched.items())
-        for (locationid, location) in to_fetch:
+        for locationid, location in to_fetch:
             try:
                 location.get_partition_details()
                 location.get_zone_details()
                 location.get_panel_meta_data()
                 # if we get here, it has been fetched successfully
                 del self._locations_unfetched[locationid]
             except Exception:
@@ -150,42 +160,43 @@
         if rc == _ResultCode.INVALID_SESSIONID:
             raise InvalidSessionError("invalid session ID", response)
         if rc == _ResultCode.CONNECTION_ERROR:
             raise RetryableTotalConnectError("connection error", response)
         if rc == _ResultCode.FAILED_TO_CONNECT:
             raise RetryableTotalConnectError("failed to connect with panel", response)
         if rc == _ResultCode.AUTHENTICATION_FAILED:
-            raise RetryableTotalConnectError("temporary authentication failure", response)
+            raise RetryableTotalConnectError(
+                "temporary authentication failure", response
+            )
         if rc == _ResultCode.BAD_OBJECT_REFERENCE:
             raise RetryableTotalConnectError("bad object reference", response)
 
-
     def raise_for_resultcode(self, response):
         """If response.ResultCode indicates success, return and do nothing.
         If it indicates an authentication error, raise AuthenticationError.
         """
         rc = _ResultCode.from_response(response)
         if rc in (
-                _ResultCode.SUCCESS,
-                _ResultCode.ARM_SUCCESS,
-                _ResultCode.DISARM_SUCCESS,
-                _ResultCode.SESSION_INITIATED,
+            _ResultCode.SUCCESS,
+            _ResultCode.ARM_SUCCESS,
+            _ResultCode.DISARM_SUCCESS,
+            _ResultCode.SESSION_INITIATED,
         ):
             return
         self._raise_for_retry(response)
         if rc == _ResultCode.BAD_USER_OR_PASSWORD:
             raise AuthenticationError(rc.name, response)
         if rc == _ResultCode.USER_CODE_UNAVAILABLE:
             raise UsercodeUnavailable(rc.name, response)
         if rc == _ResultCode.USER_CODE_INVALID:
             raise UsercodeInvalid(rc.name, response)
         if rc == _ResultCode.FEATURE_NOT_SUPPORTED:
             raise FeatureNotSupportedError(rc.name, response)
         if rc == _ResultCode.FAILED_TO_BYPASS_ZONE:
-            raise FailedToBypassZone(rc.name, response)            
+            raise FailedToBypassZone(rc.name, response)
         raise BadResultCodeError(rc.name, response)
 
     def _send_one_request(self, operation_name, args):
         LOGGER.debug(f"sending API request {operation_name}{args}")
         operation_proxy = self.soap_client.service[operation_name]
         return zeep.helpers.serialize_object(operation_proxy(*args))
 
@@ -202,51 +213,69 @@
         if not self.soap_client:
             # the server doesn't support RFC 5746 secure renegotiation, which
             # causes OpenSSL to fail by default. here we override the default.
             # if they fix their server, we should revert this change to ctx.options
             session = requests.Session()
             ctx = ssl.create_default_context(ssl.Purpose.SERVER_AUTH)
             ctx.options |= 0x04  # ssl.OP_LEGACY_SERVER_CONNECT once that exists
-            session.mount('https://', _SslContextAdapter(ctx))
+            session.mount("https://", _SslContextAdapter(ctx))
+            cache = zeep.cache.InMemoryCache()
+            for url, filename in SCHEMAS_TO_CACHE.items():
+                cache_file = impresources.files(cache_folder) / filename
+                with cache_file.open() as file:
+                    cache.add(url, file.read())
             transport = zeep.transports.Transport(
                 session=session,
-                cache=zeep.cache.InMemoryCache(timeout=3600),
+                cache=cache,
                 timeout=self.TIMEOUT,  # for loading WSDL and xsd documents
                 operation_timeout=self.TIMEOUT,  # for operations (POST/GET)
             )
             self.soap_client = zeep.Client(self.API_ENDPOINT, transport=transport)
         try:
             response = self._send_one_request(operation_name, args)
             self._raise_for_retry(response)
             return response
         # To retry an exception that could be raised during the
         # request, add it to an except block here, depending on what
         # you want to have happen. The first block just retries and
         # logs. The second block causes reauthentication.
-        except (RetryableTotalConnectError, requests.exceptions.RequestException) as err:
+        except (
+            RetryableTotalConnectError,
+            requests.exceptions.RequestException,
+        ) as err:
             if attempts_remaining <= 0:
                 raise
             if isinstance(err, RetryableTotalConnectError):
-                msg = f"{self.username} {operation_name}{args} {err.args[0]} on response"
+                msg = (
+                    f"{self.username} {operation_name}{args} {err.args[0]} on response"
+                )
             else:
                 msg = f"{self.username} {operation_name}{args} {err} on request"
             if is_first_request:
                 LOGGER.info(f"{msg}: {attempts_remaining} retries remaining")
             else:
                 LOGGER.debug(f"{msg}: {attempts_remaining} retries remaining")
             time.sleep(self.retry_delay)
-        except ZeepFault as err:
+        except (ZeepFault, requests.exceptions.HTTPError) as err:
             if attempts_remaining <= 0:
-                raise ServiceUnavailable(f"Error connecting to Total Connect service: {err}") from err
-            LOGGER.debug(f"Error connecting to Total Connect service: {attempts_remaining} retries remaining")
+                raise ServiceUnavailable(
+                    f"Error connecting to Total Connect service: {err}"
+                ) from err
+            LOGGER.debug(
+                f"Error connecting to Total Connect service: {attempts_remaining} retries remaining"
+            )
             time.sleep(self.retry_delay)
         except InvalidSessionError as err:
             if attempts_remaining <= 0:
-                raise ServiceUnavailable(f"Invalid Session after multiple retries: {err}") from err
-            LOGGER.info(f"reauthenticating {self.username}: {attempts_remaining} retries remaining")
+                raise ServiceUnavailable(
+                    f"Invalid Session after multiple retries: {err}"
+                ) from err
+            LOGGER.info(
+                f"reauthenticating {self.username}: {attempts_remaining} retries remaining"
+            )
             old_token = self.token
             self.token = None
             self.authenticate()
             args = [self.token if old_token == arg else arg for arg in args]
         return self.request(operation_name, args, attempts_remaining)
 
     def authenticate(self):
@@ -260,17 +289,18 @@
                 f"not authenticating: password already failed for user {self.username}"
             )
 
         # LoginAndGetSessionDetails is very slow, so only use it when necessary
         operation_name = (
             "AuthenticateUserLogin" if self._locations else "LoginAndGetSessionDetails"
         )
-        response = self.request(operation_name, (
-            self.username, self.password, self.API_APP_ID, self.API_APP_VERSION
-        ))
+        response = self.request(
+            operation_name,
+            (self.username, self.password, self.API_APP_ID, self.API_APP_VERSION),
+        )
         try:
             self.raise_for_resultcode(response)
         except AuthenticationError:
             self._invalid_credentials = True
             self.token = None
             raise
 
@@ -285,15 +315,17 @@
             if not self._locations:
                 raise TotalConnectError("no locations found", response)
         LOGGER.info(f"{self.username} authenticated: {len(self._locations)} locations")
         self.times["authenticate()"] = time.time() - start_time
 
     def validate_usercode(self, device_id, usercode):
         """Return True if the usercode is valid for the device."""
-        response = self.request("ValidateUserCode", (self.token, device_id, str(usercode)))
+        response = self.request(
+            "ValidateUserCode", (self.token, device_id, str(usercode))
+        )
         try:
             self.raise_for_resultcode(response)
         except UsercodeInvalid:
             LOGGER.warning(f"usercode {usercode} invalid for device {device_id}")
             return False
         except UsercodeUnavailable:
             LOGGER.warning(f"usercode {usercode} unavailable for device {device_id}")
@@ -332,16 +364,17 @@
             location = TotalConnectLocation(locationinfo, self)
             new_locations[location_id] = location
 
             location.auto_bypass_low_battery = self.auto_bypass_low_battery
 
             # set the usercode for the location
             usercode = (
-                self.usercodes.get(location_id) or  # noqa: W504
-                self.usercodes.get(str(location_id)) or self.usercodes.get("default")
+                self.usercodes.get(location_id)  # noqa: W504
+                or self.usercodes.get(str(location_id))
+                or self.usercodes.get("default")
             )
             if usercode:
                 location.usercode = usercode
             else:
                 LOGGER.warning(f"no usercode for location {location_id}")
                 location.usercode = DEFAULT_USERCODE
```

### Comparing `total_connect_client-2024.4/total_connect_client/const.py` & `total_connect_client-2024.5/total_connect_client/const.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2024.4/total_connect_client/device.py` & `total_connect_client-2024.5/total_connect_client/device.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2024.4/total_connect_client/disarm.py` & `total_connect_client-2024.5/total_connect_client/disarm.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2024.4/total_connect_client/exceptions.py` & `total_connect_client-2024.5/total_connect_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2024.4/total_connect_client/live/auto_bypass.py` & `total_connect_client-2024.5/total_connect_client/live/auto_bypass.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2024.4/total_connect_client/live/experimental.py` & `total_connect_client-2024.5/total_connect_client/live/experimental.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2024.4/total_connect_client/live/zwave.py` & `total_connect_client-2024.5/total_connect_client/live/zwave.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2024.4/total_connect_client/location.py` & `total_connect_client-2024.5/total_connect_client/location.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2024.4/total_connect_client/partition.py` & `total_connect_client-2024.5/total_connect_client/partition.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2024.4/total_connect_client/sync.py` & `total_connect_client-2024.5/total_connect_client/sync.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2024.4/total_connect_client/user.py` & `total_connect_client-2024.5/total_connect_client/user.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2024.4/total_connect_client/zone.py` & `total_connect_client-2024.5/total_connect_client/zone.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2024.4/total_connect_client.egg-info/PKG-INFO` & `total_connect_client-2024.5/total_connect_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: total_connect_client
-Version: 2024.4
+Version: 2024.5
 Summary: Interact with Total Connect 2 alarm systems
 Author-email: "Craig J. Midwinter" <craig.j.midwinter@gmail.com>
 Project-URL: Homepage, https://github.com/craigjmidwinter/total-connect-client
 Project-URL: Bug Tracker, https://github.com/craigjmidwinter/total-connect-client/issues
 Keywords: alarm,TotalConnect
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: zeep>=4.2.1
 
 # Total-Connect-Client
 Total-Connect-Client is a python client for interacting with the [TotalConnect2](https://totalconnect2.com) alarm system.
```

### Comparing `total_connect_client-2024.4/total_connect_client.egg-info/SOURCES.txt` & `total_connect_client-2024.5/total_connect_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,10 +30,11 @@
 total_connect_client/user.py
 total_connect_client/zone.py
 total_connect_client.egg-info/PKG-INFO
 total_connect_client.egg-info/SOURCES.txt
 total_connect_client.egg-info/dependency_links.txt
 total_connect_client.egg-info/requires.txt
 total_connect_client.egg-info/top_level.txt
+total_connect_client/cache/soap-encodings-schemas.xmlsoap.org.txt
 total_connect_client/live/auto_bypass.py
 total_connect_client/live/experimental.py
 total_connect_client/live/zwave.py
```

