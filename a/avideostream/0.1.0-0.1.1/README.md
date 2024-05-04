# Comparing `tmp/avideostream-0.1.0.tar.gz` & `tmp/avideostream-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avideostream-0.1.0.tar", last modified: Mon Mar 25 05:33:33 2024, max compression
+gzip compressed data, was "avideostream-0.1.1.tar", last modified: Sat May  4 22:44:26 2024, max compression
```

## Comparing `avideostream-0.1.0.tar` & `avideostream-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 javad     (1000) javad     (1001)        0 2024-03-25 05:33:33.681657 avideostream-0.1.0/
--rw-r--r--   0 javad     (1000) javad     (1001)     1071 2024-03-24 21:32:21.000000 avideostream-0.1.0/LICENSE
--rw-r--r--   0 javad     (1000) javad     (1001)       16 2024-03-25 05:19:10.000000 avideostream-0.1.0/MANIFEST.in
--rw-r--r--   0 javad     (1000) javad     (1001)     2010 2024-03-25 05:33:33.681657 avideostream-0.1.0/PKG-INFO
--rw-r--r--   0 javad     (1000) javad     (1001)      108 2024-03-25 05:22:25.000000 avideostream-0.1.0/README.md
-drwxr-xr-x   0 javad     (1000) javad     (1001)        0 2024-03-25 05:33:33.681657 avideostream-0.1.0/avideostream.egg-info/
--rw-r--r--   0 javad     (1000) javad     (1001)     2010 2024-03-25 05:33:33.000000 avideostream-0.1.0/avideostream.egg-info/PKG-INFO
--rw-r--r--   0 javad     (1000) javad     (1001)      339 2024-03-25 05:33:33.000000 avideostream-0.1.0/avideostream.egg-info/SOURCES.txt
--rw-r--r--   0 javad     (1000) javad     (1001)        1 2024-03-25 05:33:33.000000 avideostream-0.1.0/avideostream.egg-info/dependency_links.txt
--rw-r--r--   0 javad     (1000) javad     (1001)       17 2024-03-25 05:33:33.000000 avideostream-0.1.0/avideostream.egg-info/top_level.txt
--rw-r--r--   0 javad     (1000) javad     (1001)      734 2024-03-25 05:28:12.000000 avideostream-0.1.0/pyproject.toml
--rw-r--r--   0 javad     (1000) javad     (1001)       38 2024-03-25 05:33:33.681657 avideostream-0.1.0/setup.cfg
--rw-r--r--   0 javad     (1000) javad     (1001)      891 2024-03-25 05:28:33.000000 avideostream-0.1.0/setup.py
-drwxr-xr-x   0 javad     (1000) javad     (1001)        0 2024-03-25 05:33:33.681657 avideostream-0.1.0/src/
--rw-r--r--   0 javad     (1000) javad     (1001)     2488 2024-03-25 05:19:10.000000 avideostream-0.1.0/src/FrameEncoding.c
--rw-r--r--   0 javad     (1000) javad     (1001)      665 2024-03-25 05:19:10.000000 avideostream-0.1.0/src/FrameEncoding.h
--rw-r--r--   0 javad     (1000) javad     (1001)      199 2024-03-25 05:19:10.000000 avideostream-0.1.0/src/Utils.h
--rw-r--r--   0 javad     (1000) javad     (1001)     4943 2024-03-25 05:19:11.000000 avideostream-0.1.0/src/VideoStream.c
--rw-r--r--   0 javad     (1000) javad     (1001)      810 2024-03-25 05:19:11.000000 avideostream-0.1.0/src/VideoStream.h
--rw-r--r--   0 javad     (1000) javad     (1001)        0 2024-03-25 05:19:10.000000 avideostream-0.1.0/src/__init__.py
--rw-r--r--   0 javad     (1000) javad     (1001)     5223 2024-03-25 05:24:29.000000 avideostream-0.1.0/src/avideostream.c
--rw-r--r--   0 javad     (1000) javad     (1001)      417 2024-03-25 05:19:10.000000 avideostream-0.1.0/src/avideostream.h
+drwxr-xr-x   0 javad     (1000) javad     (1001)        0 2024-05-04 22:44:26.035144 avideostream-0.1.1/
+-rw-r--r--   0 javad     (1000) javad     (1001)      498 2024-03-25 05:19:11.000000 avideostream-0.1.1/.gitignore
+-rw-r--r--   0 javad     (1000) javad     (1001)      917 2024-03-25 05:26:13.000000 avideostream-0.1.1/CMakeLists.txt
+-rw-r--r--   0 javad     (1000) javad     (1001)     1071 2024-03-24 21:32:21.000000 avideostream-0.1.1/LICENSE
+-rw-r--r--   0 javad     (1000) javad     (1001)       16 2024-03-25 05:19:10.000000 avideostream-0.1.1/MANIFEST.in
+-rw-r--r--   0 javad     (1000) javad     (1001)     2010 2024-05-04 22:44:26.031811 avideostream-0.1.1/PKG-INFO
+-rw-r--r--   0 javad     (1000) javad     (1001)      108 2024-03-25 05:22:25.000000 avideostream-0.1.1/README.md
+drwxr-xr-x   0 javad     (1000) javad     (1001)        0 2024-05-04 22:44:26.031811 avideostream-0.1.1/avideostream.egg-info/
+-rw-r--r--   0 javad     (1000) javad     (1001)     2010 2024-05-04 22:44:24.000000 avideostream-0.1.1/avideostream.egg-info/PKG-INFO
+-rw-r--r--   0 javad     (1000) javad     (1001)      376 2024-05-04 22:44:24.000000 avideostream-0.1.1/avideostream.egg-info/SOURCES.txt
+-rw-r--r--   0 javad     (1000) javad     (1001)        1 2024-05-04 22:44:24.000000 avideostream-0.1.1/avideostream.egg-info/dependency_links.txt
+-rw-r--r--   0 javad     (1000) javad     (1001)       17 2024-05-04 22:44:24.000000 avideostream-0.1.1/avideostream.egg-info/top_level.txt
+-rw-r--r--   0 javad     (1000) javad     (1001)      734 2024-05-04 22:44:09.000000 avideostream-0.1.1/pyproject.toml
+-rw-r--r--   0 javad     (1000) javad     (1001)       38 2024-05-04 22:44:26.035144 avideostream-0.1.1/setup.cfg
+-rw-r--r--   0 javad     (1000) javad     (1001)      891 2024-05-04 22:44:09.000000 avideostream-0.1.1/setup.py
+drwxr-xr-x   0 javad     (1000) javad     (1001)        0 2024-05-04 22:44:26.031811 avideostream-0.1.1/src/
+-rw-r--r--   0 javad     (1000) javad     (1001)     2488 2024-03-25 05:19:10.000000 avideostream-0.1.1/src/FrameEncoding.c
+-rw-r--r--   0 javad     (1000) javad     (1001)      665 2024-03-25 05:19:10.000000 avideostream-0.1.1/src/FrameEncoding.h
+-rw-r--r--   0 javad     (1000) javad     (1001)      199 2024-03-25 05:19:10.000000 avideostream-0.1.1/src/Utils.h
+-rw-r--r--   0 javad     (1000) javad     (1001)     4943 2024-03-25 05:19:11.000000 avideostream-0.1.1/src/VideoStream.c
+-rw-r--r--   0 javad     (1000) javad     (1001)      810 2024-03-25 05:19:11.000000 avideostream-0.1.1/src/VideoStream.h
+-rw-r--r--   0 javad     (1000) javad     (1001)        0 2024-03-25 05:19:10.000000 avideostream-0.1.1/src/__init__.py
+-rw-r--r--   0 javad     (1000) javad     (1001)     5223 2024-03-25 05:24:29.000000 avideostream-0.1.1/src/avideostream.c
+-rw-r--r--   0 javad     (1000) javad     (1001)      417 2024-03-25 05:19:10.000000 avideostream-0.1.1/src/avideostream.h
+-rw-r--r--   0 javad     (1000) javad     (1001)     1187 2024-03-25 05:19:11.000000 avideostream-0.1.1/src/main.c
```

### Comparing `avideostream-0.1.0/LICENSE` & `avideostream-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `avideostream-0.1.0/PKG-INFO` & `avideostream-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avideostream
-Version: 0.1.0
+Version: 0.1.1
 Summary: Directly use libav (ffmpeg) to read RTSP streams with python bindings.
 Author: SimplyPrint
 Author-email: SimplyPrint <javad.asgari@simplyprint.io>
 License: MIT License
         
         Copyright (c) 2024 Javad Shafique
```

### Comparing `avideostream-0.1.0/avideostream.egg-info/PKG-INFO` & `avideostream-0.1.1/avideostream.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avideostream
-Version: 0.1.0
+Version: 0.1.1
 Summary: Directly use libav (ffmpeg) to read RTSP streams with python bindings.
 Author: SimplyPrint
 Author-email: SimplyPrint <javad.asgari@simplyprint.io>
 License: MIT License
         
         Copyright (c) 2024 Javad Shafique
```

### Comparing `avideostream-0.1.0/pyproject.toml` & `avideostream-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "avideostream"
-version = "0.1.0"
+version = "0.1.1"
 authors = [{ name = "SimplyPrint", email = "javad.asgari@simplyprint.io" }]
 description = "Directly use libav (ffmpeg) to read RTSP streams with python bindings."
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = ["video", "streaming", "ffmpeg"]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `avideostream-0.1.0/setup.py` & `avideostream-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, Extension, find_packages
 
 setup(
     name="avideostream",
-    version="0.1.0",
+    version="0.1.1",
     author="SimplyPrint",
     author_email="javad.asgari@simplyprint.io",
     description="Directly use libav (ffmpeg) to read RTSP streams with python bindings.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `avideostream-0.1.0/src/FrameEncoding.c` & `avideostream-0.1.1/src/FrameEncoding.c`

 * *Files identical despite different names*

### Comparing `avideostream-0.1.0/src/FrameEncoding.h` & `avideostream-0.1.1/src/FrameEncoding.h`

 * *Files identical despite different names*

### Comparing `avideostream-0.1.0/src/VideoStream.c` & `avideostream-0.1.1/src/VideoStream.c`

 * *Files identical despite different names*

### Comparing `avideostream-0.1.0/src/VideoStream.h` & `avideostream-0.1.1/src/VideoStream.h`

 * *Files identical despite different names*

### Comparing `avideostream-0.1.0/src/avideostream.c` & `avideostream-0.1.1/src/avideostream.c`

 * *Files identical despite different names*

