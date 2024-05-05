# Comparing `tmp/pchjlib-0.0.3.8.tar.gz` & `tmp/pchjlib-0.0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pchjlib-0.0.3.8.tar", last modified: Sun May  5 11:00:24 2024, max compression
+gzip compressed data, was "pchjlib-0.0.3.9.tar", last modified: Sun May  5 11:12:49 2024, max compression
```

## Comparing `pchjlib-0.0.3.8.tar` & `pchjlib-0.0.3.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 11:00:24.083849 pchjlib-0.0.3.8/
--rw-rw-rw-   0        0        0       10 2024-02-20 13:43:18.000000 pchjlib-0.0.3.8/COPYRIGHT.txt
--rw-rw-rw-   0        0        0     1086 2024-02-18 13:43:57.000000 pchjlib-0.0.3.8/LICENSE.txt
--rw-rw-rw-   0        0        0       59 2024-02-18 13:46:41.000000 pchjlib-0.0.3.8/MANIFEST.in
--rw-rw-rw-   0        0        0    17780 2024-05-05 11:00:24.083849 pchjlib-0.0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0    16253 2024-05-05 10:58:32.000000 pchjlib-0.0.3.8/README.md
--rw-rw-rw-   0        0        0      365 2024-05-05 11:00:24.083849 pchjlib-0.0.3.8/setup.cfg
--rw-rw-rw-   0        0        0     4061 2024-05-05 10:52:36.000000 pchjlib-0.0.3.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 11:00:24.067834 pchjlib-0.0.3.8/src/
-drwxrwxrwx   0        0        0        0 2024-05-05 11:00:24.083849 pchjlib-0.0.3.8/src/pchjlib.egg-info/
--rw-rw-rw-   0        0        0    17780 2024-05-05 11:00:24.000000 pchjlib-0.0.3.8/src/pchjlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-05-05 11:00:24.000000 pchjlib-0.0.3.8/src/pchjlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 11:00:24.000000 pchjlib-0.0.3.8/src/pchjlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-05-05 11:00:24.000000 pchjlib-0.0.3.8/src/pchjlib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       12 2024-05-05 11:00:24.000000 pchjlib-0.0.3.8/src/pchjlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-05 11:00:24.000000 pchjlib-0.0.3.8/src/pchjlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-05-05 11:00:23.000000 pchjlib-0.0.3.8/src/pchjlib.egg-info/zip-safe
--rw-rw-rw-   0        0        0    47062 2024-05-05 10:59:34.000000 pchjlib-0.0.3.8/src/pchjlib.py
+drwxrwxrwx   0        0        0        0 2024-05-05 11:12:49.610066 pchjlib-0.0.3.9/
+-rw-rw-rw-   0        0        0       10 2024-02-20 13:43:18.000000 pchjlib-0.0.3.9/COPYRIGHT.txt
+-rw-rw-rw-   0        0        0     1086 2024-02-18 13:43:57.000000 pchjlib-0.0.3.9/LICENSE.txt
+-rw-rw-rw-   0        0        0       59 2024-02-18 13:46:41.000000 pchjlib-0.0.3.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    17950 2024-05-05 11:12:49.610066 pchjlib-0.0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0    16414 2024-05-05 11:12:14.000000 pchjlib-0.0.3.9/README.md
+-rw-rw-rw-   0        0        0      365 2024-05-05 11:12:49.610066 pchjlib-0.0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     4061 2024-05-05 11:11:21.000000 pchjlib-0.0.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 11:12:49.596109 pchjlib-0.0.3.9/src/
+drwxrwxrwx   0        0        0        0 2024-05-05 11:12:49.610066 pchjlib-0.0.3.9/src/pchjlib.egg-info/
+-rw-rw-rw-   0        0        0    17950 2024-05-05 11:12:49.000000 pchjlib-0.0.3.9/src/pchjlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-05-05 11:12:49.000000 pchjlib-0.0.3.9/src/pchjlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 11:12:49.000000 pchjlib-0.0.3.9/src/pchjlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-05 11:12:49.000000 pchjlib-0.0.3.9/src/pchjlib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       12 2024-05-05 11:12:49.000000 pchjlib-0.0.3.9/src/pchjlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-05 11:12:49.000000 pchjlib-0.0.3.9/src/pchjlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-05-05 11:12:48.000000 pchjlib-0.0.3.9/src/pchjlib.egg-info/zip-safe
+-rw-rw-rw-   0        0        0    47031 2024-05-05 11:11:16.000000 pchjlib-0.0.3.9/src/pchjlib.py
```

### Comparing `pchjlib-0.0.3.8/LICENSE.txt` & `pchjlib-0.0.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pchjlib-0.0.3.8/PKG-INFO` & `pchjlib-0.0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pchjlib
-Version: 0.0.3.8
+Version: 0.0.3.9
 Summary: Thư viện này có thể thực hiện các phép tính, thuật toán, xử lí chuỗi, mảng, . . .
 Home-page: https://github.com/Joesifer/pchjlib
 Author: Joesifer
 License: MIT License
 Keywords: pchjlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -489,14 +489,19 @@
 ``` python
 - one_two_three().
 >> Nhung su lua chon de ban choi keo bua bao voi A.I;
 ```
 
 # NHUNG BAN CAP NHAT
 
+### 0.0.3.9 - (5/5/2024).
+- ***Sá»­a lá»—i.***
+
+### 0.0.3.8 - (5/5/2024).
+- ***Cap nhat "mp_christmas_tree_cho_VSCode" vÃ  "mp_christmas_tree_cho_TEXT".***
 ### 0.0.3.8 - (5/5/2024).
 - ***Cap nhat "mp_christmas_tree_cho_VSCode" vÃ  "mp_christmas_tree_cho_TEXT".***
 
 ### 0.0.3.7 - (4/5/2024).
 - ***Cap nhat "mp_christmas_tree".***
 
 ### 0.0.3.6 - (03/03/2024).
```

### Comparing `pchjlib-0.0.3.8/README.md` & `pchjlib-0.0.3.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -460,14 +460,19 @@
 ``` python
 - one_two_three().
 >> Nhung su lua chon de ban choi keo bua bao voi A.I;
 ```
 
 # NHUNG BAN CAP NHAT
 
+### 0.0.3.9 - (5/5/2024).
+- ***Sửa lỗi.***
+
+### 0.0.3.8 - (5/5/2024).
+- ***Cap nhat "mp_christmas_tree_cho_VSCode" và "mp_christmas_tree_cho_TEXT".***
 ### 0.0.3.8 - (5/5/2024).
 - ***Cap nhat "mp_christmas_tree_cho_VSCode" và "mp_christmas_tree_cho_TEXT".***
 
 ### 0.0.3.7 - (4/5/2024).
 - ***Cap nhat "mp_christmas_tree".***
 
 ### 0.0.3.6 - (03/03/2024).
```

### Comparing `pchjlib-0.0.3.8/setup.py` & `pchjlib-0.0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from setuptools import setup
 
 
 desc = open(r"C:\Users\LAPTOP DELL\Desktop\pchjlib_admin\README.md").read()
 
 setup(
     name="pchjlib",
-    version="0.0.3.8",
+    version="0.0.3.9",
     author="Joesifer",
     description="Thư viện này có thể thực hiện các phép tính, thuật toán, xử lí chuỗi, mảng, . . .",
     long_description=desc,
     long_description_content_type="text/markdown",
     license="MIT License",
     keywords="pchjlib",
     classifiers=[
```

### Comparing `pchjlib-0.0.3.8/src/pchjlib.egg-info/PKG-INFO` & `pchjlib-0.0.3.9/src/pchjlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pchjlib
-Version: 0.0.3.8
+Version: 0.0.3.9
 Summary: Thư viện này có thể thực hiện các phép tính, thuật toán, xử lí chuỗi, mảng, . . .
 Home-page: https://github.com/Joesifer/pchjlib
 Author: Joesifer
 License: MIT License
 Keywords: pchjlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -489,14 +489,19 @@
 ``` python
 - one_two_three().
 >> Nhung su lua chon de ban choi keo bua bao voi A.I;
 ```
 
 # NHUNG BAN CAP NHAT
 
+### 0.0.3.9 - (5/5/2024).
+- ***Sá»­a lá»—i.***
+
+### 0.0.3.8 - (5/5/2024).
+- ***Cap nhat "mp_christmas_tree_cho_VSCode" vÃ  "mp_christmas_tree_cho_TEXT".***
 ### 0.0.3.8 - (5/5/2024).
 - ***Cap nhat "mp_christmas_tree_cho_VSCode" vÃ  "mp_christmas_tree_cho_TEXT".***
 
 ### 0.0.3.7 - (4/5/2024).
 - ***Cap nhat "mp_christmas_tree".***
 
 ### 0.0.3.6 - (03/03/2024).
```

### Comparing `pchjlib-0.0.3.8/src/pchjlib.py` & `pchjlib-0.0.3.9/src/pchjlib.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 ---------------------------------------------------------
 Tác giả
 ---------------------------------------------------------
 - Joesifer.
 
 Phiên bản
 ---------------------------------------------------------
-- 0.0.3.8.
+- 0.0.3.9.
 
 Ngày đăng
 ---------------------------------------------------------
 - ngày 14 tháng Hai, năm 2024.
 
 Bản quyền
 ---------------------------------------------------------
@@ -1006,17 +1006,14 @@
     for i in range(n // 3):
         tree.append("  " * n + "▮")
 
     for i in range(len(tree)):
         print(tree[i])
 
 
-mp_christmas_tree_cho_TEXT()
-
-
 # # Ham ho tro tinh toan dac biet
 # Ham tinh toan cac cong thuc vat ly
 def tinh_toan_vat_ly_8():
     print(
         "\n",
         " —————————————————————————————————————————————————————————————————————————————————————",
         "\n",
```

