# Comparing `tmp/vodesfunc-1.6.0.tar.gz` & `tmp/vodesfunc-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vodesfunc-1.6.0.tar", last modified: Sun May  5 15:28:14 2024, max compression
+gzip compressed data, was "vodesfunc-1.6.1.tar", last modified: Sun May  5 20:27:19 2024, max compression
```

## Comparing `vodesfunc-1.6.0.tar` & `vodesfunc-1.6.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:28:14.735282 vodesfunc-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-05 15:28:06.000000 vodesfunc-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-05 15:28:06.000000 vodesfunc-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-05 15:28:14.735282 vodesfunc-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-05 15:28:06.000000 vodesfunc-1.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-05 15:28:06.000000 vodesfunc-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 15:28:14.735282 vodesfunc-1.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:28:14.735282 vodesfunc-1.6.0/vodesfunc/
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-05 15:28:06.000000 vodesfunc-1.6.0/vodesfunc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-05-05 15:28:06.000000 vodesfunc-1.6.0/vodesfunc/aa.py
--rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-05-05 15:28:06.000000 vodesfunc-1.6.0/vodesfunc/denoise.py
--rw-r--r--   0 runner    (1001) docker     (127)    21732 2024-05-05 15:28:06.000000 vodesfunc-1.6.0/vodesfunc/descale.py
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-05 15:28:06.000000 vodesfunc-1.6.0/vodesfunc/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7403 2024-05-05 15:28:06.000000 vodesfunc-1.6.0/vodesfunc/noise.py
--rw-r--r--   0 runner    (1001) docker     (127)    16866 2024-05-05 15:28:06.000000 vodesfunc-1.6.0/vodesfunc/rescale.py
--rw-r--r--   0 runner    (1001) docker     (127)    13347 2024-05-05 15:28:06.000000 vodesfunc-1.6.0/vodesfunc/scale.py
--rw-r--r--   0 runner    (1001) docker     (127)     6746 2024-05-05 15:28:06.000000 vodesfunc-1.6.0/vodesfunc/spikefinder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-05-05 15:28:06.000000 vodesfunc-1.6.0/vodesfunc/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:28:14.735282 vodesfunc-1.6.0/vodesfunc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-05 15:28:14.000000 vodesfunc-1.6.0/vodesfunc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-05 15:28:14.000000 vodesfunc-1.6.0/vodesfunc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 15:28:14.000000 vodesfunc-1.6.0/vodesfunc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-05 15:28:14.000000 vodesfunc-1.6.0/vodesfunc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-05 15:28:14.000000 vodesfunc-1.6.0/vodesfunc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:27:19.284858 vodesfunc-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-05 20:27:08.000000 vodesfunc-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-05 20:27:08.000000 vodesfunc-1.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-05 20:27:19.284858 vodesfunc-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-05 20:27:08.000000 vodesfunc-1.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-05 20:27:08.000000 vodesfunc-1.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 20:27:19.284858 vodesfunc-1.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:27:19.284858 vodesfunc-1.6.1/vodesfunc/
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-05 20:27:08.000000 vodesfunc-1.6.1/vodesfunc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-05-05 20:27:08.000000 vodesfunc-1.6.1/vodesfunc/aa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-05-05 20:27:08.000000 vodesfunc-1.6.1/vodesfunc/denoise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21732 2024-05-05 20:27:08.000000 vodesfunc-1.6.1/vodesfunc/descale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-05 20:27:08.000000 vodesfunc-1.6.1/vodesfunc/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7403 2024-05-05 20:27:08.000000 vodesfunc-1.6.1/vodesfunc/noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16866 2024-05-05 20:27:08.000000 vodesfunc-1.6.1/vodesfunc/rescale.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13347 2024-05-05 20:27:08.000000 vodesfunc-1.6.1/vodesfunc/scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6746 2024-05-05 20:27:08.000000 vodesfunc-1.6.1/vodesfunc/spikefinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-05-05 20:27:08.000000 vodesfunc-1.6.1/vodesfunc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:27:19.284858 vodesfunc-1.6.1/vodesfunc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-05 20:27:19.000000 vodesfunc-1.6.1/vodesfunc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-05 20:27:19.000000 vodesfunc-1.6.1/vodesfunc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 20:27:19.000000 vodesfunc-1.6.1/vodesfunc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-05 20:27:19.000000 vodesfunc-1.6.1/vodesfunc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-05 20:27:19.000000 vodesfunc-1.6.1/vodesfunc.egg-info/top_level.txt
```

### Comparing `vodesfunc-1.6.0/LICENSE` & `vodesfunc-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.6.0/PKG-INFO` & `vodesfunc-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: vodesfunc
-Version: 1.6.0
+Version: 1.6.1
 Summary: Vodes' random Vapoursynth Functions.
 Author-email: Vodes <vodes.imp@gmail.com>
 License: MPL 2.0
 Project-URL: Source Code, https://github.com/Vodes/vodesfunc
 Project-URL: Contact, https://discord.gg/Kf94Nv6WVN
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Typing :: Typed
 Classifier: Topic :: Multimedia :: Video
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Vapoursynth>=61
 Requires-Dist: vsscale>=1.0.1
 Requires-Dist: vsrgtools>=1.3.0
 Requires-Dist: vskernels>=1.2.0
 Requires-Dist: vstools>=1.6.2
```

### Comparing `vodesfunc-1.6.0/pyproject.toml` & `vodesfunc-1.6.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "vodesfunc"
-version = "1.6.0"
+version = "1.6.1"
 description = "Vodes' random Vapoursynth Functions."
 authors = [{ name = "Vodes", email = "vodes.imp@gmail.com" }]
 dependencies = [
     "Vapoursynth>=61",
     "vsscale>=1.0.1",
     "vsrgtools>=1.3.0",
     "vskernels>=1.2.0",
@@ -13,21 +13,21 @@
     "vsmasktools>=1.1.0",
     "vsmuxtools>=0.1.0"
 ]
 classifiers = [
     "Natural Language :: English",
     "Intended Audience :: Developers",
     "Intended Audience :: End Users/Desktop",
-    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
     "Typing :: Typed",
     "Topic :: Multimedia :: Video",
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
 ]
-requires-python = ">=3.10"
+requires-python = ">=3.11"
 readme = "README.md"
 license = { text = "MPL 2.0" }
 
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
```

### Comparing `vodesfunc-1.6.0/vodesfunc/aa.py` & `vodesfunc-1.6.1/vodesfunc/aa.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.6.0/vodesfunc/denoise.py` & `vodesfunc-1.6.1/vodesfunc/denoise.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.6.0/vodesfunc/descale.py` & `vodesfunc-1.6.1/vodesfunc/descale.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.6.0/vodesfunc/misc.py` & `vodesfunc-1.6.1/vodesfunc/misc.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.6.0/vodesfunc/noise.py` & `vodesfunc-1.6.1/vodesfunc/noise.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.6.0/vodesfunc/rescale.py` & `vodesfunc-1.6.1/vodesfunc/rescale.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.6.0/vodesfunc/scale.py` & `vodesfunc-1.6.1/vodesfunc/scale.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.6.0/vodesfunc/spikefinder.py` & `vodesfunc-1.6.1/vodesfunc/spikefinder.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.6.0/vodesfunc/util.py` & `vodesfunc-1.6.1/vodesfunc/util.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.6.0/vodesfunc.egg-info/PKG-INFO` & `vodesfunc-1.6.1/vodesfunc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: vodesfunc
-Version: 1.6.0
+Version: 1.6.1
 Summary: Vodes' random Vapoursynth Functions.
 Author-email: Vodes <vodes.imp@gmail.com>
 License: MPL 2.0
 Project-URL: Source Code, https://github.com/Vodes/vodesfunc
 Project-URL: Contact, https://discord.gg/Kf94Nv6WVN
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Typing :: Typed
 Classifier: Topic :: Multimedia :: Video
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Vapoursynth>=61
 Requires-Dist: vsscale>=1.0.1
 Requires-Dist: vsrgtools>=1.3.0
 Requires-Dist: vskernels>=1.2.0
 Requires-Dist: vstools>=1.6.2
```

