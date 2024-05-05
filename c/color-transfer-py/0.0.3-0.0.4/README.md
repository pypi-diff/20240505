# Comparing `tmp/color_transfer_py-0.0.3.tar.gz` & `tmp/color_transfer_py-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "color_transfer_py-0.0.3.tar", last modified: Sat May  4 14:59:12 2024, max compression
+gzip compressed data, was "color_transfer_py-0.0.4.tar", last modified: Sat May  4 16:32:11 2024, max compression
```

## Comparing `color_transfer_py-0.0.3.tar` & `color_transfer_py-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 14:59:12.595951 color_transfer_py-0.0.3/
--rw-rw-rw-   0        0        0     1085 2024-05-04 12:51:43.000000 color_transfer_py-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     2142 2024-05-04 14:59:12.595951 color_transfer_py-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1560 2024-05-04 13:24:29.000000 color_transfer_py-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 14:59:12.595951 color_transfer_py-0.0.3/color_transfer_py.egg-info/
--rw-rw-rw-   0        0        0     2142 2024-05-04 14:59:12.000000 color_transfer_py-0.0.3/color_transfer_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2024-05-04 14:59:12.000000 color_transfer_py-0.0.3/color_transfer_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 14:59:12.000000 color_transfer_py-0.0.3/color_transfer_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-04 14:59:12.000000 color_transfer_py-0.0.3/color_transfer_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 14:59:12.000000 color_transfer_py-0.0.3/color_transfer_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      202 2024-05-04 12:50:39.000000 color_transfer_py-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-04 14:59:12.595951 color_transfer_py-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1003 2024-05-04 14:58:01.000000 color_transfer_py-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 16:32:11.791743 color_transfer_py-0.0.4/
+-rw-rw-rw-   0        0        0     1085 2024-05-04 12:51:43.000000 color_transfer_py-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     2142 2024-05-04 16:32:11.789739 color_transfer_py-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1560 2024-05-04 13:24:29.000000 color_transfer_py-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 16:32:11.761155 color_transfer_py-0.0.4/color_transfer/
+-rw-rw-rw-   0        0        0       80 2024-05-04 12:01:25.000000 color_transfer_py-0.0.4/color_transfer/__init__.py
+-rw-rw-rw-   0        0        0      933 2024-05-04 12:01:25.000000 color_transfer_py-0.0.4/color_transfer/numpy.py
+-rw-rw-rw-   0        0        0     2893 2024-05-04 12:01:25.000000 color_transfer_py-0.0.4/color_transfer/pytorch.py
+-rw-rw-rw-   0        0        0     8250 2024-05-04 12:01:25.000000 color_transfer_py-0.0.4/color_transfer/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-04 16:32:11.788737 color_transfer_py-0.0.4/color_transfer_py.egg-info/
+-rw-rw-rw-   0        0        0     2142 2024-05-04 16:32:11.000000 color_transfer_py-0.0.4/color_transfer_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2024-05-04 16:32:11.000000 color_transfer_py-0.0.4/color_transfer_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 16:32:11.000000 color_transfer_py-0.0.4/color_transfer_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-04 16:32:11.000000 color_transfer_py-0.0.4/color_transfer_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-04 16:32:11.000000 color_transfer_py-0.0.4/color_transfer_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      202 2024-05-04 12:50:39.000000 color_transfer_py-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-04 16:32:11.791743 color_transfer_py-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2024-05-04 16:31:59.000000 color_transfer_py-0.0.4/setup.py
```

### Comparing `color_transfer_py-0.0.3/LICENSE.txt` & `color_transfer_py-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `color_transfer_py-0.0.3/PKG-INFO` & `color_transfer_py-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: color_transfer_py
-Version: 0.0.3
+Version: 0.0.4
 Summary: Color transfer between images
 Home-page: https://github.com/ptran1203/color_transfer
 Author: Phat Tran
 Author-email: phatth1203@gmail.com
 Project-URL: Bug Tracker, https://github.com/ptran1203/color_transfer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `color_transfer_py-0.0.3/README.md` & `color_transfer_py-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `color_transfer_py-0.0.3/color_transfer_py.egg-info/PKG-INFO` & `color_transfer_py-0.0.4/color_transfer_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: color_transfer_py
-Version: 0.0.3
+Version: 0.0.4
 Summary: Color transfer between images
 Home-page: https://github.com/ptran1203/color_transfer
 Author: Phat Tran
 Author-email: phatth1203@gmail.com
 Project-URL: Bug Tracker, https://github.com/ptran1203/color_transfer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `color_transfer_py-0.0.3/setup.py` & `color_transfer_py-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "color_transfer_py",
-    version = "0.0.3",
+    version = "0.0.4",
     author = "Phat Tran",
     author_email = "phatth1203@gmail.com",
     description = "Color transfer between images",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/ptran1203/color_transfer",
     project_urls = {
```

