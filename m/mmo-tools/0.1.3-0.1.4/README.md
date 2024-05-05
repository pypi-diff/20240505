# Comparing `tmp/mmo_tools-0.1.3.tar.gz` & `tmp/mmo_tools-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmo_tools-0.1.3.tar", last modified: Sat May  4 13:24:18 2024, max compression
+gzip compressed data, was "mmo_tools-0.1.4.tar", last modified: Sat May  4 13:27:08 2024, max compression
```

## Comparing `mmo_tools-0.1.3.tar` & `mmo_tools-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 13:24:18.915803 mmo_tools-0.1.3/
--rw-rw-rw-   0        0        0     2481 2024-05-04 13:24:18.915803 mmo_tools-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1455 2024-05-04 13:23:51.000000 mmo_tools-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-04 13:24:18.916805 mmo_tools-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1235 2024-05-04 13:24:01.000000 mmo_tools-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-04 13:24:18.893803 mmo_tools-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-04 13:24:18.903801 mmo_tools-0.1.3/src/mmo_tools/
--rw-rw-rw-   0        0        0      183 2024-05-04 13:04:59.000000 mmo_tools-0.1.3/src/mmo_tools/__init__.py
--rw-rw-rw-   0        0        0     2640 2024-05-04 13:23:00.000000 mmo_tools-0.1.3/src/mmo_tools/core.py
--rw-rw-rw-   0        0        0     1836 2024-05-04 13:02:48.000000 mmo_tools-0.1.3/src/mmo_tools/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-04 13:24:18.913801 mmo_tools-0.1.3/src/mmo_tools.egg-info/
--rw-rw-rw-   0        0        0     2481 2024-05-04 13:24:18.000000 mmo_tools-0.1.3/src/mmo_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2024-05-04 13:24:18.000000 mmo_tools-0.1.3/src/mmo_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 13:24:18.000000 mmo_tools-0.1.3/src/mmo_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-04 13:24:18.000000 mmo_tools-0.1.3/src/mmo_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 13:27:08.943275 mmo_tools-0.1.4/
+-rw-rw-rw-   0        0        0     2481 2024-05-04 13:27:08.942276 mmo_tools-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1455 2024-05-04 13:23:51.000000 mmo_tools-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-04 13:27:08.943275 mmo_tools-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1235 2024-05-04 13:26:57.000000 mmo_tools-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 13:27:08.921276 mmo_tools-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-04 13:27:08.932276 mmo_tools-0.1.4/src/mmo_tools/
+-rw-rw-rw-   0        0        0      183 2024-05-04 13:04:59.000000 mmo_tools-0.1.4/src/mmo_tools/__init__.py
+-rw-rw-rw-   0        0        0     2667 2024-05-04 13:26:49.000000 mmo_tools-0.1.4/src/mmo_tools/core.py
+-rw-rw-rw-   0        0        0     1836 2024-05-04 13:02:48.000000 mmo_tools-0.1.4/src/mmo_tools/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-04 13:27:08.942276 mmo_tools-0.1.4/src/mmo_tools.egg-info/
+-rw-rw-rw-   0        0        0     2481 2024-05-04 13:27:08.000000 mmo_tools-0.1.4/src/mmo_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2024-05-04 13:27:08.000000 mmo_tools-0.1.4/src/mmo_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 13:27:08.000000 mmo_tools-0.1.4/src/mmo_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-04 13:27:08.000000 mmo_tools-0.1.4/src/mmo_tools.egg-info/top_level.txt
```

### Comparing `mmo_tools-0.1.3/PKG-INFO` & `mmo_tools-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmo_tools
-Version: 0.1.3
+Version: 0.1.4
 Summary: Thư Viện Hỗ Trợ Viết Tool Facebook Nhanh
 Home-page: UNKNOWN
 Author: Lam Dinh
 Author-email: ldl.contact.booking@gmail.com
 License: UNKNOWN
 Description: # mmo_tools
         Đây là một thư viện Python chứa các hàm tiện ích để chuyển đổi dữ liệu và cấu hình proxy .
```

### Comparing `mmo_tools-0.1.3/README.md` & `mmo_tools-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mmo_tools-0.1.3/setup.py` & `mmo_tools-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
     name='mmo_tools',  # Tên thư viện của bạn
-    version='0.1.3',  # Phiên bản đầu tiên
+    version='0.1.4',  # Phiên bản đầu tiên
     packages=find_packages('src'),  # Tìm tất cả các packages trong thư mục src
     package_dir={'': 'src'},  # Chỉ định thư mục chứa các packages
     author='Lam Dinh',
     author_email='ldl.contact.booking@gmail.com',
     description='Thư Viện Hỗ Trợ Viết Tool Facebook Nhanh',
     long_description=open('README.md','r',encoding='utf-8').read(),  # Đọc nội dung README nếu có
     long_description_content_type='text/markdown',  # Định dạng của long description
```

### Comparing `mmo_tools-0.1.3/src/mmo_tools/core.py` & `mmo_tools-0.1.4/src/mmo_tools/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from . import utils
 import os , re , requests
 
 def convert_data(file) -> str:
    
     try:
-        data_r =  open(file , "r",encoding="UTF-8").readlines()
+        data_r =  [key.strip("\n") for key in open(file , "r",encoding="UTF-8").readlines()]
     except Exception as error:
         return error
     data   = []
     for r in data_r:
-
         rp = utils.dict_typ()
         r = r + "||"
         if ("c_user" in r) and ("i_user" not in r):user =  r.split("c_user=")[1].split(";")[0]
         elif "i_user" in r:user =  r.split("i_user=")[1].split(";")[0]
         else:user = ""
         
         rp.update({"c_user":user}) # => user id
```

### Comparing `mmo_tools-0.1.3/src/mmo_tools/utils.py` & `mmo_tools-0.1.4/src/mmo_tools/utils.py`

 * *Files identical despite different names*

### Comparing `mmo_tools-0.1.3/src/mmo_tools.egg-info/PKG-INFO` & `mmo_tools-0.1.4/src/mmo_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmo-tools
-Version: 0.1.3
+Version: 0.1.4
 Summary: Thư Viện Hỗ Trợ Viết Tool Facebook Nhanh
 Home-page: UNKNOWN
 Author: Lam Dinh
 Author-email: ldl.contact.booking@gmail.com
 License: UNKNOWN
 Description: # mmo_tools
         Đây là một thư viện Python chứa các hàm tiện ích để chuyển đổi dữ liệu và cấu hình proxy .
```

