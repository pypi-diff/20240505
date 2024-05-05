# Comparing `tmp/RTS-WebUIBuilder-0.5.tar.gz` & `tmp/RTS-WebUIBuilder-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RTS-WebUIBuilder-0.5.tar", last modified: Fri May  3 22:15:57 2024, max compression
+gzip compressed data, was "RTS-WebUIBuilder-0.6.tar", last modified: Sun May  5 15:21:13 2024, max compression
```

## Comparing `RTS-WebUIBuilder-0.5.tar` & `RTS-WebUIBuilder-0.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 22:15:57.808917 RTS-WebUIBuilder-0.5/
--rw-rw-rw-   0        0        0     1349 2024-04-01 09:09:39.000000 RTS-WebUIBuilder-0.5/LICENCE
--rw-rw-rw-   0        0        0      823 2024-05-03 22:15:57.808415 RTS-WebUIBuilder-0.5/PKG-INFO
--rw-rw-rw-   0        0        0       92 2024-04-29 16:57:15.000000 RTS-WebUIBuilder-0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 22:15:57.796918 RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/
--rw-rw-rw-   0        0        0     1055 2024-04-15 18:28:33.000000 RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/RAdditions.py
--rw-rw-rw-   0        0        0     2282 2024-04-29 16:01:41.000000 RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/RBody.py
--rw-rw-rw-   0        0        0     2718 2024-04-28 15:20:36.000000 RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/RBox.py
--rw-rw-rw-   0        0        0     3233 2024-04-29 15:07:44.000000 RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/RDocument.py
--rw-rw-rw-   0        0        0     2320 2024-04-13 14:53:29.000000 RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/RFrame.py
--rw-rw-rw-   0        0        0    10637 2024-04-24 17:48:28.000000 RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/RGroupStyle.py
--rw-rw-rw-   0        0        0     1261 2024-04-13 14:44:52.000000 RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/RHead.py
--rw-rw-rw-   0        0        0       92 2024-04-13 18:50:09.000000 RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/RImage.py
--rw-rw-rw-   0        0        0     2754 2024-04-21 08:51:23.000000 RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/RInput.py
--rw-rw-rw-   0        0        0      839 2024-04-26 21:26:34.000000 RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/RLabel.py
--rw-rw-rw-   0        0        0      326 2024-04-27 16:51:27.000000 RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/RQuickScripts.py
--rw-rw-rw-   0        0        0    10454 2024-04-24 17:44:53.000000 RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/RStyle.py
--rw-rw-rw-   0        0        0      796 2024-04-28 18:56:26.000000 RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/RTitle.py
--rw-rw-rw-   0        0        0     6174 2024-05-03 21:50:55.000000 RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/RWebserver.py
--rw-rw-rw-   0        0        0     3523 2024-04-29 16:16:05.000000 RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/RpyColorizer.py
--rw-rw-rw-   0        0        0      516 2024-05-03 22:15:42.000000 RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/__init__.py
--rw-rw-rw-   0        0        0      370 2024-04-13 17:25:24.000000 RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/cache.py
--rw-rw-rw-   0        0        0      888 2024-04-29 15:07:12.000000 RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/exeptional.py
--rw-rw-rw-   0        0        0     1015 2024-04-21 15:08:22.000000 RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/privatizehead.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:15:57.807419 RTS-WebUIBuilder-0.5/RTS_WebUIBuilder.egg-info/
--rw-rw-rw-   0        0        0      823 2024-05-03 22:15:57.000000 RTS-WebUIBuilder-0.5/RTS_WebUIBuilder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      775 2024-05-03 22:15:57.000000 RTS-WebUIBuilder-0.5/RTS_WebUIBuilder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 22:15:57.000000 RTS-WebUIBuilder-0.5/RTS_WebUIBuilder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-03 22:15:57.000000 RTS-WebUIBuilder-0.5/RTS_WebUIBuilder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-03 22:15:57.000000 RTS-WebUIBuilder-0.5/RTS_WebUIBuilder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 22:15:57.808917 RTS-WebUIBuilder-0.5/setup.cfg
--rw-rw-rw-   0        0        0      922 2024-05-03 22:15:54.000000 RTS-WebUIBuilder-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:21:13.843918 RTS-WebUIBuilder-0.6/
+-rw-rw-rw-   0        0        0     1349 2024-04-01 09:09:39.000000 RTS-WebUIBuilder-0.6/LICENCE
+-rw-rw-rw-   0        0        0      823 2024-05-05 15:21:13.843412 RTS-WebUIBuilder-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       92 2024-04-29 16:57:15.000000 RTS-WebUIBuilder-0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 15:21:13.828733 RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/
+-rw-rw-rw-   0        0        0     1055 2024-04-15 18:28:33.000000 RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/RAdditions.py
+-rw-rw-rw-   0        0        0     2282 2024-04-29 16:01:41.000000 RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/RBody.py
+-rw-rw-rw-   0        0        0     2718 2024-04-28 15:20:36.000000 RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/RBox.py
+-rw-rw-rw-   0        0        0     3233 2024-04-29 15:07:44.000000 RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/RDocument.py
+-rw-rw-rw-   0        0        0     2320 2024-04-13 14:53:29.000000 RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/RFrame.py
+-rw-rw-rw-   0        0        0    10637 2024-04-24 17:48:28.000000 RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/RGroupStyle.py
+-rw-rw-rw-   0        0        0     1261 2024-04-13 14:44:52.000000 RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/RHead.py
+-rw-rw-rw-   0        0        0       92 2024-04-13 18:50:09.000000 RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/RImage.py
+-rw-rw-rw-   0        0        0     2754 2024-04-21 08:51:23.000000 RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/RInput.py
+-rw-rw-rw-   0        0        0      839 2024-04-26 21:26:34.000000 RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/RLabel.py
+-rw-rw-rw-   0        0        0      326 2024-04-27 16:51:27.000000 RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/RQuickScripts.py
+-rw-rw-rw-   0        0        0    10454 2024-04-24 17:44:53.000000 RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/RStyle.py
+-rw-rw-rw-   0        0        0      796 2024-04-28 18:56:26.000000 RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/RTitle.py
+-rw-rw-rw-   0        0        0     6174 2024-05-03 21:50:55.000000 RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/RWebserver.py
+-rw-rw-rw-   0        0        0     3523 2024-04-29 16:16:05.000000 RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/RpyColorizer.py
+-rw-rw-rw-   0        0        0      516 2024-05-03 22:15:42.000000 RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/__init__.py
+-rw-rw-rw-   0        0        0      370 2024-04-13 17:25:24.000000 RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/cache.py
+-rw-rw-rw-   0        0        0      888 2024-04-29 15:07:12.000000 RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/exeptional.py
+-rw-rw-rw-   0        0        0     1015 2024-04-21 15:08:22.000000 RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/privatizehead.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:21:13.842408 RTS-WebUIBuilder-0.6/RTS_WebUIBuilder.egg-info/
+-rw-rw-rw-   0        0        0      823 2024-05-05 15:21:13.000000 RTS-WebUIBuilder-0.6/RTS_WebUIBuilder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      775 2024-05-05 15:21:13.000000 RTS-WebUIBuilder-0.6/RTS_WebUIBuilder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 15:21:13.000000 RTS-WebUIBuilder-0.6/RTS_WebUIBuilder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-05 15:21:13.000000 RTS-WebUIBuilder-0.6/RTS_WebUIBuilder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-05 15:21:13.000000 RTS-WebUIBuilder-0.6/RTS_WebUIBuilder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-05 15:21:13.843918 RTS-WebUIBuilder-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      922 2024-05-05 15:21:11.000000 RTS-WebUIBuilder-0.6/setup.py
```

### Comparing `RTS-WebUIBuilder-0.5/LICENCE` & `RTS-WebUIBuilder-0.6/LICENCE`

 * *Files identical despite different names*

### Comparing `RTS-WebUIBuilder-0.5/PKG-INFO` & `RTS-WebUIBuilder-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RTS-WebUIBuilder
-Version: 0.5
+Version: 0.6
 Summary: A simple webserver with a simple webui builder.
 Home-page: https://github.com/RandomTimeLP/RTS_Webbuilder
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: MIT with required credit to the author.
 Keywords: WebUIBuilder,Webserver,Work In Progress
 Platform: UNKNOWN
```

### Comparing `RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/RAdditions.py` & `RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/RAdditions.py`

 * *Files identical despite different names*

### Comparing `RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/RBody.py` & `RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/RBody.py`

 * *Files identical despite different names*

### Comparing `RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/RBox.py` & `RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/RBox.py`

 * *Files identical despite different names*

### Comparing `RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/RDocument.py` & `RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/RDocument.py`

 * *Files identical despite different names*

### Comparing `RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/RFrame.py` & `RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/RFrame.py`

 * *Files identical despite different names*

### Comparing `RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/RGroupStyle.py` & `RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/RGroupStyle.py`

 * *Files identical despite different names*

### Comparing `RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/RHead.py` & `RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/RHead.py`

 * *Files identical despite different names*

### Comparing `RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/RInput.py` & `RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/RInput.py`

 * *Files identical despite different names*

### Comparing `RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/RLabel.py` & `RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/RLabel.py`

 * *Files identical despite different names*

### Comparing `RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/RStyle.py` & `RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/RStyle.py`

 * *Files identical despite different names*

### Comparing `RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/RTitle.py` & `RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/RTitle.py`

 * *Files identical despite different names*

### Comparing `RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/RWebserver.py` & `RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/RWebserver.py`

 * *Files identical despite different names*

### Comparing `RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/RpyColorizer.py` & `RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/RpyColorizer.py`

 * *Files identical despite different names*

### Comparing `RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/__init__.py` & `RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/__init__.py`

 * *Files identical despite different names*

### Comparing `RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/exeptional.py` & `RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/exeptional.py`

 * *Files identical despite different names*

### Comparing `RTS-WebUIBuilder-0.5/RTS_WebUIBuilder/privatizehead.py` & `RTS-WebUIBuilder-0.6/RTS_WebUIBuilder/privatizehead.py`

 * *Files identical despite different names*

### Comparing `RTS-WebUIBuilder-0.5/RTS_WebUIBuilder.egg-info/PKG-INFO` & `RTS-WebUIBuilder-0.6/RTS_WebUIBuilder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RTS-WebUIBuilder
-Version: 0.5
+Version: 0.6
 Summary: A simple webserver with a simple webui builder.
 Home-page: https://github.com/RandomTimeLP/RTS_Webbuilder
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: MIT with required credit to the author.
 Keywords: WebUIBuilder,Webserver,Work In Progress
 Platform: UNKNOWN
```

### Comparing `RTS-WebUIBuilder-0.5/RTS_WebUIBuilder.egg-info/SOURCES.txt` & `RTS-WebUIBuilder-0.6/RTS_WebUIBuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RTS-WebUIBuilder-0.5/setup.py` & `RTS-WebUIBuilder-0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='RTS-WebUIBuilder',
-    version='0.5',
+    version='0.6',
     packages=find_packages(),
     description='A simple webserver with a simple webui builder.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='RandomTimeTV',
     author_email='dergepanzerte1@gmail.com',
     license='MIT with required credit to the author.',
```
