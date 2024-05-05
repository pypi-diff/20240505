# Comparing `tmp/simpleworktime-0.1.0.tar.gz` & `tmp/simpleworktime-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleworktime-0.1.0.tar", last modified: Sun May  5 14:52:19 2024, max compression
+gzip compressed data, was "simpleworktime-0.2.0.tar", last modified: Sun May  5 15:08:06 2024, max compression
```

## Comparing `simpleworktime-0.1.0.tar` & `simpleworktime-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-05 14:52:19.495327 simpleworktime-0.1.0/
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)    35149 2024-05-05 14:46:09.000000 simpleworktime-0.1.0/LICENSE
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      786 2024-05-05 14:52:19.495327 simpleworktime-0.1.0/PKG-INFO
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)       57 2024-05-05 14:46:09.000000 simpleworktime-0.1.0/README.md
-drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-05 14:52:19.495327 simpleworktime-0.1.0/SimpleWorkTime.egg-info/
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      786 2024-05-05 14:52:19.000000 simpleworktime-0.1.0/SimpleWorkTime.egg-info/PKG-INFO
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      247 2024-05-05 14:52:19.000000 simpleworktime-0.1.0/SimpleWorkTime.egg-info/SOURCES.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)        1 2024-05-05 14:52:19.000000 simpleworktime-0.1.0/SimpleWorkTime.egg-info/dependency_links.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)       54 2024-05-05 14:52:19.000000 simpleworktime-0.1.0/SimpleWorkTime.egg-info/entry_points.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)        4 2024-05-05 14:52:19.000000 simpleworktime-0.1.0/SimpleWorkTime.egg-info/top_level.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)       38 2024-05-05 14:52:19.495327 simpleworktime-0.1.0/setup.cfg
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      990 2024-05-05 14:49:09.000000 simpleworktime-0.1.0/setup.py
-drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-05 14:52:19.495327 simpleworktime-0.1.0/src/
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)        0 2024-05-05 14:46:34.000000 simpleworktime-0.1.0/src/__init__.py
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      963 2024-05-05 14:47:33.000000 simpleworktime-0.1.0/src/main.py
+drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-05 15:08:06.190879 simpleworktime-0.2.0/
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)    35149 2024-05-05 14:46:09.000000 simpleworktime-0.2.0/LICENSE
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      786 2024-05-05 15:08:06.190879 simpleworktime-0.2.0/PKG-INFO
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)       57 2024-05-05 14:46:09.000000 simpleworktime-0.2.0/README.md
+drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-05 15:08:06.190879 simpleworktime-0.2.0/SimpleWorkTime.egg-info/
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      786 2024-05-05 15:08:06.000000 simpleworktime-0.2.0/SimpleWorkTime.egg-info/PKG-INFO
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      247 2024-05-05 15:08:06.000000 simpleworktime-0.2.0/SimpleWorkTime.egg-info/SOURCES.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)        1 2024-05-05 15:08:06.000000 simpleworktime-0.2.0/SimpleWorkTime.egg-info/dependency_links.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)       54 2024-05-05 15:08:06.000000 simpleworktime-0.2.0/SimpleWorkTime.egg-info/entry_points.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)        4 2024-05-05 15:08:06.000000 simpleworktime-0.2.0/SimpleWorkTime.egg-info/top_level.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)       38 2024-05-05 15:08:06.190879 simpleworktime-0.2.0/setup.cfg
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      990 2024-05-05 15:06:54.000000 simpleworktime-0.2.0/setup.py
+drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-05 15:08:06.190879 simpleworktime-0.2.0/src/
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)        0 2024-05-05 14:46:34.000000 simpleworktime-0.2.0/src/__init__.py
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)     1170 2024-05-05 14:56:11.000000 simpleworktime-0.2.0/src/main.py
```

### Comparing `simpleworktime-0.1.0/LICENSE` & `simpleworktime-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simpleworktime-0.1.0/PKG-INFO` & `simpleworktime-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleWorkTime
-Version: 0.1.0
+Version: 0.2.0
 Summary: A simple command-line work time tracker
 Author: John Vouvakis Manousakis
 Author-email: ioannis_vm@berkeley.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `simpleworktime-0.1.0/SimpleWorkTime.egg-info/PKG-INFO` & `simpleworktime-0.2.0/SimpleWorkTime.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleWorkTime
-Version: 0.1.0
+Version: 0.2.0
 Summary: A simple command-line work time tracker
 Author: John Vouvakis Manousakis
 Author-email: ioannis_vm@berkeley.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `simpleworktime-0.1.0/setup.py` & `simpleworktime-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='SimpleWorkTime',
-    version='0.1.0',
+    version='0.2.0',
     packages=find_packages(),
     description='A simple command-line work time tracker',
     author='John Vouvakis Manousakis',
     author_email='ioannis_vm@berkeley.edu',
     entry_points={
         'console_scripts': [
             'simpleworktime=src.main:run_timer'
```

### Comparing `simpleworktime-0.1.0/src/main.py` & `simpleworktime-0.2.0/src/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,19 +13,26 @@
     )
 
     total_time: float = 0.0
     working: bool = False
     start_time: float = 0.0
 
     while True:
-        user_input: str = input()
-        if user_input.lower() == 'exit':
+        try:
+            user_input: str = input()
+            if user_input.lower() == 'exit':
+                if working:
+                    total_time += time.time() - start_time
+                break
+        except EOFError:
+            print("\nCtrl-D detected, exiting...")
             if working:
                 total_time += time.time() - start_time
             break
+
         if working:
             total_time += time.time() - start_time
             working = False
             print("Work paused. Press Enter to resume.")
         else:
             start_time = time.time()
             working = True
```

