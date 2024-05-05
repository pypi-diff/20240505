# Comparing `tmp/pchjlib-0.0.3.7.tar.gz` & `tmp/pchjlib-0.0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pchjlib-0.0.3.7.tar", last modified: Sat May  4 15:02:57 2024, max compression
+gzip compressed data, was "pchjlib-0.0.3.8.tar", last modified: Sun May  5 11:00:24 2024, max compression
```

## Comparing `pchjlib-0.0.3.7.tar` & `pchjlib-0.0.3.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 15:02:57.796834 pchjlib-0.0.3.7/
--rw-rw-rw-   0        0        0       10 2024-02-20 13:43:18.000000 pchjlib-0.0.3.7/COPYRIGHT.txt
--rw-rw-rw-   0        0        0     1086 2024-02-18 13:43:57.000000 pchjlib-0.0.3.7/LICENSE.txt
--rw-rw-rw-   0        0        0       59 2024-02-18 13:46:41.000000 pchjlib-0.0.3.7/MANIFEST.in
--rw-rw-rw-   0        0        0    17270 2024-05-04 15:02:57.796834 pchjlib-0.0.3.7/PKG-INFO
--rw-rw-rw-   0        0        0    15737 2024-05-04 15:00:56.000000 pchjlib-0.0.3.7/README.md
--rw-rw-rw-   0        0        0      365 2024-05-04 15:02:57.796834 pchjlib-0.0.3.7/setup.cfg
--rw-rw-rw-   0        0        0     4061 2024-05-04 15:01:53.000000 pchjlib-0.0.3.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-04 15:02:57.787634 pchjlib-0.0.3.7/src/
-drwxrwxrwx   0        0        0        0 2024-05-04 15:02:57.796834 pchjlib-0.0.3.7/src/pchjlib.egg-info/
--rw-rw-rw-   0        0        0    17270 2024-05-04 15:02:57.000000 pchjlib-0.0.3.7/src/pchjlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-05-04 15:02:57.000000 pchjlib-0.0.3.7/src/pchjlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 15:02:57.000000 pchjlib-0.0.3.7/src/pchjlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-05-04 15:02:57.000000 pchjlib-0.0.3.7/src/pchjlib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       12 2024-05-04 15:02:57.000000 pchjlib-0.0.3.7/src/pchjlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-04 15:02:57.000000 pchjlib-0.0.3.7/src/pchjlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-05-04 15:02:57.000000 pchjlib-0.0.3.7/src/pchjlib.egg-info/zip-safe
--rw-rw-rw-   0        0        0    46545 2024-05-04 15:01:16.000000 pchjlib-0.0.3.7/src/pchjlib.py
+drwxrwxrwx   0        0        0        0 2024-05-05 11:00:24.083849 pchjlib-0.0.3.8/
+-rw-rw-rw-   0        0        0       10 2024-02-20 13:43:18.000000 pchjlib-0.0.3.8/COPYRIGHT.txt
+-rw-rw-rw-   0        0        0     1086 2024-02-18 13:43:57.000000 pchjlib-0.0.3.8/LICENSE.txt
+-rw-rw-rw-   0        0        0       59 2024-02-18 13:46:41.000000 pchjlib-0.0.3.8/MANIFEST.in
+-rw-rw-rw-   0        0        0    17780 2024-05-05 11:00:24.083849 pchjlib-0.0.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0    16253 2024-05-05 10:58:32.000000 pchjlib-0.0.3.8/README.md
+-rw-rw-rw-   0        0        0      365 2024-05-05 11:00:24.083849 pchjlib-0.0.3.8/setup.cfg
+-rw-rw-rw-   0        0        0     4061 2024-05-05 10:52:36.000000 pchjlib-0.0.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 11:00:24.067834 pchjlib-0.0.3.8/src/
+drwxrwxrwx   0        0        0        0 2024-05-05 11:00:24.083849 pchjlib-0.0.3.8/src/pchjlib.egg-info/
+-rw-rw-rw-   0        0        0    17780 2024-05-05 11:00:24.000000 pchjlib-0.0.3.8/src/pchjlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-05-05 11:00:24.000000 pchjlib-0.0.3.8/src/pchjlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 11:00:24.000000 pchjlib-0.0.3.8/src/pchjlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-05 11:00:24.000000 pchjlib-0.0.3.8/src/pchjlib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       12 2024-05-05 11:00:24.000000 pchjlib-0.0.3.8/src/pchjlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-05 11:00:24.000000 pchjlib-0.0.3.8/src/pchjlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-05-05 11:00:23.000000 pchjlib-0.0.3.8/src/pchjlib.egg-info/zip-safe
+-rw-rw-rw-   0        0        0    47062 2024-05-05 10:59:34.000000 pchjlib-0.0.3.8/src/pchjlib.py
```

### Comparing `pchjlib-0.0.3.7/LICENSE.txt` & `pchjlib-0.0.3.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pchjlib-0.0.3.7/PKG-INFO` & `pchjlib-0.0.3.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pchjlib
-Version: 0.0.3.7
+Version: 0.0.3.8
 Summary: Thư viện này có thể thực hiện các phép tính, thuật toán, xử lí chuỗi, mảng, . . .
 Home-page: https://github.com/Joesifer/pchjlib
 Author: Joesifer
 License: MIT License
 Keywords: pchjlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -374,37 +374,55 @@
 
 ### Ham mo phong qua trinh "LOADING...".
 ``` python
 - mp_loading(n):
 >> LOADING...
 ```
 
-### Ham mo phong cay thong.
+### Ham mo phong cay thong cho VSCode.
 ``` python
-- mp_christmas_tree():
+- mp_christmas_tree_cho_VSCode():
 - Nhap chieu cao cay thong: 8
         *
        * *
       * * *
      * * * *
     * * * * *
    * * * * * *
   * * * * * * *
  * * * * * * * *
-        â–®
-        â–®
+        H
+        H
+```
+
+### Ham mo phong cay thong cho TEXT.
+``` python
+- mp_christmas_tree_cho_TEXT():
+- Nhap chieu cao cay thong: 8
+                 *  
+               *  *   
+             *  *  *    
+           *  *  *  *     
+         *  *  *  *  *      
+       *  *  *  *  *  *       
+     *  *  *  *  *  *  *        
+   *  *  *  *  *  *  *  *
+                H
+                H
 ```
 
 # Ham ho tro tinh toan dac biet:
 ### Ham tinh toan cac cong thuc vat ly.
 ``` python
 - tinh_toan_vat_ly_8().
 >> Mot bang lua chon cac cong thuc vat ly 8 chuong trinh GDPT 2018 sach CTST HK1;
 >>
 
+
+
                    >>>>> NHAP TEN CONG THUC BAN MUON DE ADMIN TINH <<<<<               
                            ~~~ ! Luu y: Nhap theo yeu cau ! ~~~                        
                                                                                        
           --> 1. Cong thuc tinh: Khoi luong rieng      (ki hieu D, Kg/m^3)             
           --> 2. Cong thuc tinh: Trong luong rieng     (ki hieu d, don vi N/m^3)       
           --> 3. Cong thuc tinh: Luc day Archimedes    (ki hieu Fa, don vi N)         
           --> 4. Cong thuc tinh: Trong luong           (ki hieu P, don vi N)           
@@ -471,14 +489,17 @@
 ``` python
 - one_two_three().
 >> Nhung su lua chon de ban choi keo bua bao voi A.I;
 ```
 
 # NHUNG BAN CAP NHAT
 
+### 0.0.3.8 - (5/5/2024).
+- ***Cap nhat "mp_christmas_tree_cho_VSCode" vÃ  "mp_christmas_tree_cho_TEXT".***
+
 ### 0.0.3.7 - (4/5/2024).
 - ***Cap nhat "mp_christmas_tree".***
 
 ### 0.0.3.6 - (03/03/2024).
 - ***Thu nghiem.***
 
 ### 0.0.3.5 - (01/03/2024).
```

### Comparing `pchjlib-0.0.3.7/README.md` & `pchjlib-0.0.3.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -345,37 +345,55 @@
 
 ### Ham mo phong qua trinh "LOADING...".
 ``` python
 - mp_loading(n):
 >> LOADING...
 ```
 
-### Ham mo phong cay thong.
+### Ham mo phong cay thong cho VSCode.
 ``` python
-- mp_christmas_tree():
+- mp_christmas_tree_cho_VSCode():
 - Nhap chieu cao cay thong: 8
         *
        * *
       * * *
      * * * *
     * * * * *
    * * * * * *
   * * * * * * *
  * * * * * * * *
-        ▮
-        ▮
+        H
+        H
+```
+
+### Ham mo phong cay thong cho TEXT.
+``` python
+- mp_christmas_tree_cho_TEXT():
+- Nhap chieu cao cay thong: 8
+                 *  
+               *  *   
+             *  *  *    
+           *  *  *  *     
+         *  *  *  *  *      
+       *  *  *  *  *  *       
+     *  *  *  *  *  *  *        
+   *  *  *  *  *  *  *  *
+                H
+                H
 ```
 
 # Ham ho tro tinh toan dac biet:
 ### Ham tinh toan cac cong thuc vat ly.
 ``` python
 - tinh_toan_vat_ly_8().
 >> Mot bang lua chon cac cong thuc vat ly 8 chuong trinh GDPT 2018 sach CTST HK1;
 >>
 
+
+
                    >>>>> NHAP TEN CONG THUC BAN MUON DE ADMIN TINH <<<<<               
                            ~~~ ! Luu y: Nhap theo yeu cau ! ~~~                        
                                                                                        
           --> 1. Cong thuc tinh: Khoi luong rieng      (ki hieu D, Kg/m^3)             
           --> 2. Cong thuc tinh: Trong luong rieng     (ki hieu d, don vi N/m^3)       
           --> 3. Cong thuc tinh: Luc day Archimedes    (ki hieu Fa, don vi N)         
           --> 4. Cong thuc tinh: Trong luong           (ki hieu P, don vi N)           
@@ -442,14 +460,17 @@
 ``` python
 - one_two_three().
 >> Nhung su lua chon de ban choi keo bua bao voi A.I;
 ```
 
 # NHUNG BAN CAP NHAT
 
+### 0.0.3.8 - (5/5/2024).
+- ***Cap nhat "mp_christmas_tree_cho_VSCode" và "mp_christmas_tree_cho_TEXT".***
+
 ### 0.0.3.7 - (4/5/2024).
 - ***Cap nhat "mp_christmas_tree".***
 
 ### 0.0.3.6 - (03/03/2024).
 - ***Thu nghiem.***
 
 ### 0.0.3.5 - (01/03/2024).
```

### Comparing `pchjlib-0.0.3.7/setup.py` & `pchjlib-0.0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from setuptools import setup
 
 
 desc = open(r"C:\Users\LAPTOP DELL\Desktop\pchjlib_admin\README.md").read()
 
 setup(
     name="pchjlib",
-    version="0.0.3.7",
+    version="0.0.3.8",
     author="Joesifer",
     description="Thư viện này có thể thực hiện các phép tính, thuật toán, xử lí chuỗi, mảng, . . .",
     long_description=desc,
     long_description_content_type="text/markdown",
     license="MIT License",
     keywords="pchjlib",
     classifiers=[
```

### Comparing `pchjlib-0.0.3.7/src/pchjlib.egg-info/PKG-INFO` & `pchjlib-0.0.3.8/src/pchjlib.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pchjlib
-Version: 0.0.3.7
+Version: 0.0.3.8
 Summary: Thư viện này có thể thực hiện các phép tính, thuật toán, xử lí chuỗi, mảng, . . .
 Home-page: https://github.com/Joesifer/pchjlib
 Author: Joesifer
 License: MIT License
 Keywords: pchjlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -374,37 +374,55 @@
 
 ### Ham mo phong qua trinh "LOADING...".
 ``` python
 - mp_loading(n):
 >> LOADING...
 ```
 
-### Ham mo phong cay thong.
+### Ham mo phong cay thong cho VSCode.
 ``` python
-- mp_christmas_tree():
+- mp_christmas_tree_cho_VSCode():
 - Nhap chieu cao cay thong: 8
         *
        * *
       * * *
      * * * *
     * * * * *
    * * * * * *
   * * * * * * *
  * * * * * * * *
-        â–®
-        â–®
+        H
+        H
+```
+
+### Ham mo phong cay thong cho TEXT.
+``` python
+- mp_christmas_tree_cho_TEXT():
+- Nhap chieu cao cay thong: 8
+                 *  
+               *  *   
+             *  *  *    
+           *  *  *  *     
+         *  *  *  *  *      
+       *  *  *  *  *  *       
+     *  *  *  *  *  *  *        
+   *  *  *  *  *  *  *  *
+                H
+                H
 ```
 
 # Ham ho tro tinh toan dac biet:
 ### Ham tinh toan cac cong thuc vat ly.
 ``` python
 - tinh_toan_vat_ly_8().
 >> Mot bang lua chon cac cong thuc vat ly 8 chuong trinh GDPT 2018 sach CTST HK1;
 >>
 
+
+
                    >>>>> NHAP TEN CONG THUC BAN MUON DE ADMIN TINH <<<<<               
                            ~~~ ! Luu y: Nhap theo yeu cau ! ~~~                        
                                                                                        
           --> 1. Cong thuc tinh: Khoi luong rieng      (ki hieu D, Kg/m^3)             
           --> 2. Cong thuc tinh: Trong luong rieng     (ki hieu d, don vi N/m^3)       
           --> 3. Cong thuc tinh: Luc day Archimedes    (ki hieu Fa, don vi N)         
           --> 4. Cong thuc tinh: Trong luong           (ki hieu P, don vi N)           
@@ -471,14 +489,17 @@
 ``` python
 - one_two_three().
 >> Nhung su lua chon de ban choi keo bua bao voi A.I;
 ```
 
 # NHUNG BAN CAP NHAT
 
+### 0.0.3.8 - (5/5/2024).
+- ***Cap nhat "mp_christmas_tree_cho_VSCode" vÃ  "mp_christmas_tree_cho_TEXT".***
+
 ### 0.0.3.7 - (4/5/2024).
 - ***Cap nhat "mp_christmas_tree".***
 
 ### 0.0.3.6 - (03/03/2024).
 - ***Thu nghiem.***
 
 ### 0.0.3.5 - (01/03/2024).
```

### Comparing `pchjlib-0.0.3.7/src/pchjlib.py` & `pchjlib-0.0.3.8/src/pchjlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,22 +23,22 @@
 # SOFTWARE.                                                                                    #
 #                                                                                              #
 ################################################################################################
 
 """
 PCHJLIB
 ===========
-
+---------------------------------------------------------
 Tác giả
 ---------------------------------------------------------
 - Joesifer.
 
 Phiên bản
 ---------------------------------------------------------
-- 0.0.3.7.
+- 0.0.3.8.
 
 Ngày đăng
 ---------------------------------------------------------
 - ngày 14 tháng Hai, năm 2024.
 
 Bản quyền
 ---------------------------------------------------------
@@ -971,15 +971,15 @@
             sys.stdout.flush()
             time.sleep(0.4)
         sys.stdout.write("\b\b\b   \b\b\b")
         sys.stdout.flush()
 
 
 # Ham mo phong cay thong
-def mp_christmas_tree():
+def mp_christmas_tree_cho_VSCode():
     n = int(input("- Nhập chiều cao cây thông: "))
     tree, dem = [], n
     for i in range(n):
         tree.append("* " * (i + 1) + " " * (i + 1))
 
     for i in range(n):
         tree[i] = " " * dem + tree[i]
@@ -988,14 +988,35 @@
     for i in range(n // 3):
         tree.append(" " * n + "▮")
 
     for i in range(len(tree)):
         print(tree[i])
 
 
+# Ham mo phong cay thong
+def mp_christmas_tree_cho_TEXT():
+    n = int(input("- Nhập chiều cao cây thông: "))
+    tree, dem = [], n
+    for i in range(n):
+        tree.append(" * " * (i + 1) + " " * (i + 1))
+
+    for i in range(n):
+        tree[i] = "  " * dem + tree[i]
+        dem -= 1
+
+    for i in range(n // 3):
+        tree.append("  " * n + "▮")
+
+    for i in range(len(tree)):
+        print(tree[i])
+
+
+mp_christmas_tree_cho_TEXT()
+
+
 # # Ham ho tro tinh toan dac biet
 # Ham tinh toan cac cong thuc vat ly
 def tinh_toan_vat_ly_8():
     print(
         "\n",
         " —————————————————————————————————————————————————————————————————————————————————————",
         "\n",
```

