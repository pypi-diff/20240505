# Comparing `tmp/astrometry_net_client-0.3.1.tar.gz` & `tmp/astrometry_net_client-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrometry_net_client-0.3.1.tar", last modified: Tue Jan 30 12:22:46 2024, max compression
+gzip compressed data, was "astrometry_net_client-0.4.0.tar", last modified: Sun May  5 12:28:02 2024, max compression
```

## Comparing `astrometry_net_client-0.3.1.tar` & `astrometry_net_client-0.4.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 sten      (1000) sten      (1000)        0 2024-01-30 12:22:46.013599 astrometry_net_client-0.3.1/
--rw-r--r--   0 sten      (1000) sten      (1000)     1067 2023-04-15 14:58:19.000000 astrometry_net_client-0.3.1/LICENSE
--rw-r--r--   0 sten      (1000) sten      (1000)     6375 2024-01-30 12:22:46.013599 astrometry_net_client-0.3.1/PKG-INFO
--rw-r--r--   0 sten      (1000) sten      (1000)     5396 2023-04-15 14:58:19.000000 astrometry_net_client-0.3.1/README.rst
-drwxr-xr-x   0 sten      (1000) sten      (1000)        0 2024-01-30 12:22:46.010266 astrometry_net_client-0.3.1/astrometry_net_client/
--rw-r--r--   0 sten      (1000) sten      (1000)      345 2023-04-15 14:58:19.000000 astrometry_net_client-0.3.1/astrometry_net_client/__init__.py
--rw-r--r--   0 sten      (1000) sten      (1000)     8524 2024-01-30 09:53:39.000000 astrometry_net_client-0.3.1/astrometry_net_client/client.py
--rw-r--r--   0 sten      (1000) sten      (1000)      490 2024-01-30 11:50:39.000000 astrometry_net_client-0.3.1/astrometry_net_client/config.py
--rw-r--r--   0 sten      (1000) sten      (1000)      663 2023-04-15 14:58:19.000000 astrometry_net_client-0.3.1/astrometry_net_client/exceptions.py
--rw-r--r--   0 sten      (1000) sten      (1000)     6658 2024-01-30 09:53:39.000000 astrometry_net_client-0.3.1/astrometry_net_client/request.py
--rw-r--r--   0 sten      (1000) sten      (1000)     5036 2023-04-15 14:58:19.000000 astrometry_net_client-0.3.1/astrometry_net_client/session.py
--rw-r--r--   0 sten      (1000) sten      (1000)     8088 2024-01-30 09:53:39.000000 astrometry_net_client-0.3.1/astrometry_net_client/settings.py
--rw-r--r--   0 sten      (1000) sten      (1000)    16640 2024-01-30 11:50:39.000000 astrometry_net_client-0.3.1/astrometry_net_client/statusables.py
--rw-r--r--   0 sten      (1000) sten      (1000)     5028 2024-01-30 11:50:39.000000 astrometry_net_client-0.3.1/astrometry_net_client/uploads.py
-drwxr-xr-x   0 sten      (1000) sten      (1000)        0 2024-01-30 12:22:46.013599 astrometry_net_client-0.3.1/astrometry_net_client.egg-info/
--rw-r--r--   0 sten      (1000) sten      (1000)     6375 2024-01-30 12:22:45.000000 astrometry_net_client-0.3.1/astrometry_net_client.egg-info/PKG-INFO
--rw-r--r--   0 sten      (1000) sten      (1000)      731 2024-01-30 12:22:45.000000 astrometry_net_client-0.3.1/astrometry_net_client.egg-info/SOURCES.txt
--rw-r--r--   0 sten      (1000) sten      (1000)        1 2024-01-30 12:22:45.000000 astrometry_net_client-0.3.1/astrometry_net_client.egg-info/dependency_links.txt
--rw-r--r--   0 sten      (1000) sten      (1000)       17 2024-01-30 12:22:45.000000 astrometry_net_client-0.3.1/astrometry_net_client.egg-info/requires.txt
--rw-r--r--   0 sten      (1000) sten      (1000)       22 2024-01-30 12:22:45.000000 astrometry_net_client-0.3.1/astrometry_net_client.egg-info/top_level.txt
--rw-r--r--   0 sten      (1000) sten      (1000)      273 2024-01-30 12:22:46.013599 astrometry_net_client-0.3.1/setup.cfg
--rw-r--r--   0 sten      (1000) sten      (1000)     1190 2024-01-30 11:50:39.000000 astrometry_net_client-0.3.1/setup.py
-drwxr-xr-x   0 sten      (1000) sten      (1000)        0 2024-01-30 12:22:46.013599 astrometry_net_client-0.3.1/tests/
--rw-r--r--   0 sten      (1000) sten      (1000)     2992 2023-04-15 14:58:19.000000 astrometry_net_client-0.3.1/tests/test.py
--rw-r--r--   0 sten      (1000) sten      (1000)     1660 2024-01-30 09:53:39.000000 astrometry_net_client-0.3.1/tests/test_client.py
--rw-r--r--   0 sten      (1000) sten      (1000)     2489 2023-04-15 14:58:19.000000 astrometry_net_client-0.3.1/tests/test_job.py
--rw-r--r--   0 sten      (1000) sten      (1000)     2352 2024-01-30 09:53:39.000000 astrometry_net_client-0.3.1/tests/test_online.py
--rw-r--r--   0 sten      (1000) sten      (1000)     1736 2023-04-15 14:58:19.000000 astrometry_net_client-0.3.1/tests/test_session.py
--rw-r--r--   0 sten      (1000) sten      (1000)     3673 2023-04-15 14:58:19.000000 astrometry_net_client-0.3.1/tests/test_settings.py
--rw-r--r--   0 sten      (1000) sten      (1000)     2987 2023-04-15 14:58:19.000000 astrometry_net_client-0.3.1/tests/test_statusables.py
--rw-r--r--   0 sten      (1000) sten      (1000)     1618 2024-01-30 11:50:39.000000 astrometry_net_client-0.3.1/tests/test_upload.py
+drwxr-xr-x   0 sten      (1000) sten      (1000)        0 2024-05-05 12:28:02.256003 astrometry_net_client-0.4.0/
+-rw-r--r--   0 sten      (1000) sten      (1000)     1067 2022-08-30 07:13:54.000000 astrometry_net_client-0.4.0/LICENSE
+-rw-r--r--   0 sten      (1000) sten      (1000)     6382 2024-05-05 12:28:02.256003 astrometry_net_client-0.4.0/PKG-INFO
+-rw-r--r--   0 sten      (1000) sten      (1000)     5396 2022-08-30 09:48:22.000000 astrometry_net_client-0.4.0/README.rst
+drwxr-xr-x   0 sten      (1000) sten      (1000)        0 2024-05-05 12:28:02.252670 astrometry_net_client-0.4.0/astrometry_net_client/
+-rw-r--r--   0 sten      (1000) sten      (1000)      345 2022-11-02 18:32:15.000000 astrometry_net_client-0.4.0/astrometry_net_client/__init__.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     8524 2023-07-23 10:22:46.000000 astrometry_net_client-0.4.0/astrometry_net_client/client.py
+-rw-r--r--   0 sten      (1000) sten      (1000)      490 2024-02-18 13:44:35.000000 astrometry_net_client-0.4.0/astrometry_net_client/config.py
+-rw-r--r--   0 sten      (1000) sten      (1000)      663 2022-11-02 18:32:13.000000 astrometry_net_client-0.4.0/astrometry_net_client/exceptions.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     6658 2023-07-23 10:22:46.000000 astrometry_net_client-0.4.0/astrometry_net_client/request.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     5036 2022-11-02 18:32:23.000000 astrometry_net_client-0.4.0/astrometry_net_client/session.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     8088 2023-07-23 10:22:46.000000 astrometry_net_client-0.4.0/astrometry_net_client/settings.py
+-rw-r--r--   0 sten      (1000) sten      (1000)    16640 2024-02-18 13:44:35.000000 astrometry_net_client-0.4.0/astrometry_net_client/statusables.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     5028 2024-02-18 13:44:35.000000 astrometry_net_client-0.4.0/astrometry_net_client/uploads.py
+drwxr-xr-x   0 sten      (1000) sten      (1000)        0 2024-05-05 12:28:02.256003 astrometry_net_client-0.4.0/astrometry_net_client.egg-info/
+-rw-r--r--   0 sten      (1000) sten      (1000)     6382 2024-05-05 12:28:02.000000 astrometry_net_client-0.4.0/astrometry_net_client.egg-info/PKG-INFO
+-rw-r--r--   0 sten      (1000) sten      (1000)      731 2024-05-05 12:28:02.000000 astrometry_net_client-0.4.0/astrometry_net_client.egg-info/SOURCES.txt
+-rw-r--r--   0 sten      (1000) sten      (1000)        1 2024-05-05 12:28:02.000000 astrometry_net_client-0.4.0/astrometry_net_client.egg-info/dependency_links.txt
+-rw-r--r--   0 sten      (1000) sten      (1000)       24 2024-05-05 12:28:02.000000 astrometry_net_client-0.4.0/astrometry_net_client.egg-info/requires.txt
+-rw-r--r--   0 sten      (1000) sten      (1000)       22 2024-05-05 12:28:02.000000 astrometry_net_client-0.4.0/astrometry_net_client.egg-info/top_level.txt
+-rw-r--r--   0 sten      (1000) sten      (1000)      273 2024-05-05 12:28:02.256003 astrometry_net_client-0.4.0/setup.cfg
+-rw-r--r--   0 sten      (1000) sten      (1000)     1197 2024-05-05 12:23:34.000000 astrometry_net_client-0.4.0/setup.py
+drwxr-xr-x   0 sten      (1000) sten      (1000)        0 2024-05-05 12:28:02.256003 astrometry_net_client-0.4.0/tests/
+-rw-r--r--   0 sten      (1000) sten      (1000)     2992 2022-08-30 07:13:54.000000 astrometry_net_client-0.4.0/tests/test.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     1660 2023-07-23 10:22:46.000000 astrometry_net_client-0.4.0/tests/test_client.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     2489 2022-08-30 07:13:54.000000 astrometry_net_client-0.4.0/tests/test_job.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     2352 2023-07-23 10:22:46.000000 astrometry_net_client-0.4.0/tests/test_online.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     1736 2022-08-30 07:13:54.000000 astrometry_net_client-0.4.0/tests/test_session.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     3673 2022-08-30 07:13:54.000000 astrometry_net_client-0.4.0/tests/test_settings.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     2987 2022-08-30 07:13:54.000000 astrometry_net_client-0.4.0/tests/test_statusables.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     1618 2024-02-18 13:44:35.000000 astrometry_net_client-0.4.0/tests/test_upload.py
```

### Comparing `astrometry_net_client-0.3.1/LICENSE` & `astrometry_net_client-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.3.1/PKG-INFO` & `astrometry_net_client-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrometry_net_client
-Version: 0.3.1
+Version: 0.4.0
 Summary: A Python interface for the Astrometry.net API.
 Home-page: https://github.com/StenSipma/astrometry_net_client
 Author: Sten Sipma
 Author-email: sten.sipma@ziggo.nl
 Keywords: astronomy astrometry client coordinates wcs api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -16,15 +16,15 @@
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Natural Language :: English
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: astropy
+Requires-Dist: astropy<=5.3.4
 Requires-Dist: requests
 
 *********************
 Astrometry.net Client
 *********************
 
 .. image:: https://readthedocs.org/projects/astrometry-net-client/badge/?version=latest
```

### Comparing `astrometry_net_client-0.3.1/README.rst` & `astrometry_net_client-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.3.1/astrometry_net_client/client.py` & `astrometry_net_client-0.4.0/astrometry_net_client/client.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.3.1/astrometry_net_client/exceptions.py` & `astrometry_net_client-0.4.0/astrometry_net_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.3.1/astrometry_net_client/request.py` & `astrometry_net_client-0.4.0/astrometry_net_client/request.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.3.1/astrometry_net_client/session.py` & `astrometry_net_client-0.4.0/astrometry_net_client/session.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.3.1/astrometry_net_client/settings.py` & `astrometry_net_client-0.4.0/astrometry_net_client/settings.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.3.1/astrometry_net_client/statusables.py` & `astrometry_net_client-0.4.0/astrometry_net_client/statusables.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.3.1/astrometry_net_client/uploads.py` & `astrometry_net_client-0.4.0/astrometry_net_client/uploads.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.3.1/astrometry_net_client.egg-info/PKG-INFO` & `astrometry_net_client-0.4.0/astrometry_net_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrometry_net_client
-Version: 0.3.1
+Version: 0.4.0
 Summary: A Python interface for the Astrometry.net API.
 Home-page: https://github.com/StenSipma/astrometry_net_client
 Author: Sten Sipma
 Author-email: sten.sipma@ziggo.nl
 Keywords: astronomy astrometry client coordinates wcs api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -16,15 +16,15 @@
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Natural Language :: English
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: astropy
+Requires-Dist: astropy<=5.3.4
 Requires-Dist: requests
 
 *********************
 Astrometry.net Client
 *********************
 
 .. image:: https://readthedocs.org/projects/astrometry-net-client/badge/?version=latest
```

### Comparing `astrometry_net_client-0.3.1/astrometry_net_client.egg-info/SOURCES.txt` & `astrometry_net_client-0.4.0/astrometry_net_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.3.1/setup.py` & `astrometry_net_client-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.rst", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="astrometry_net_client",
-    version="0.3.1",
+    version="0.4.0",
     author="Sten Sipma",
     author_email="sten.sipma@ziggo.nl",
     description="A Python interface for the Astrometry.net API.",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/StenSipma/astrometry_net_client",
     packages=["astrometry_net_client"],
-    install_requires=["astropy", "requests"],
+    install_requires=["astropy<=5.3.4", "requests"],
     keywords="astronomy astrometry client coordinates wcs api",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

### Comparing `astrometry_net_client-0.3.1/tests/test.py` & `astrometry_net_client-0.4.0/tests/test.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.3.1/tests/test_client.py` & `astrometry_net_client-0.4.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.3.1/tests/test_job.py` & `astrometry_net_client-0.4.0/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.3.1/tests/test_online.py` & `astrometry_net_client-0.4.0/tests/test_online.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.3.1/tests/test_session.py` & `astrometry_net_client-0.4.0/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.3.1/tests/test_settings.py` & `astrometry_net_client-0.4.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.3.1/tests/test_statusables.py` & `astrometry_net_client-0.4.0/tests/test_statusables.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.3.1/tests/test_upload.py` & `astrometry_net_client-0.4.0/tests/test_upload.py`

 * *Files identical despite different names*

