# Comparing `tmp/yuag-0.0.66.tar.gz` & `tmp/yuag-0.0.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yuag-0.0.66.tar", last modified: Sat Apr 13 21:15:27 2024, max compression
+gzip compressed data, was "yuag-0.0.67.tar", last modified: Sun May  5 13:54:32 2024, max compression
```

## Comparing `yuag-0.0.66.tar` & `yuag-0.0.67.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 21:15:27.084455 yuag-0.0.66/
--rw-rw-rw-   0        0        0       52 2024-04-13 21:15:27.081457 yuag-0.0.66/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-13 21:15:27.084455 yuag-0.0.66/setup.cfg
--rw-rw-rw-   0        0        0      249 2024-04-13 21:15:04.000000 yuag-0.0.66/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-13 21:15:27.049478 yuag-0.0.66/yuag/
--rw-rw-rw-   0        0        0     2814 2024-04-05 13:35:34.000000 yuag-0.0.66/yuag/__init__.py
--rw-rw-rw-   0        0        0    42525 2024-04-13 21:14:57.000000 yuag-0.0.66/yuag/yuag.py
-drwxrwxrwx   0        0        0        0 2024-04-13 21:15:27.079461 yuag-0.0.66/yuag.egg-info/
--rw-rw-rw-   0        0        0       52 2024-04-13 21:15:26.000000 yuag-0.0.66/yuag.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      150 2024-04-13 21:15:26.000000 yuag-0.0.66/yuag.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 21:15:26.000000 yuag-0.0.66/yuag.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-13 21:15:26.000000 yuag-0.0.66/yuag.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-05 13:54:32.257105 yuag-0.0.67/
+-rw-rw-rw-   0        0        0       52 2024-05-05 13:54:32.255106 yuag-0.0.67/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-05 13:54:32.257105 yuag-0.0.67/setup.cfg
+-rw-rw-rw-   0        0        0      249 2024-05-05 13:51:38.000000 yuag-0.0.67/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 13:54:32.238118 yuag-0.0.67/yuag/
+-rw-rw-rw-   0        0        0     2838 2024-05-05 13:20:05.000000 yuag-0.0.67/yuag/__init__.py
+-rw-rw-rw-   0        0        0    42998 2024-05-05 13:21:47.000000 yuag-0.0.67/yuag/yuag.py
+drwxrwxrwx   0        0        0        0 2024-05-05 13:54:32.253108 yuag-0.0.67/yuag.egg-info/
+-rw-rw-rw-   0        0        0       52 2024-05-05 13:54:32.000000 yuag-0.0.67/yuag.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      150 2024-05-05 13:54:32.000000 yuag-0.0.67/yuag.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 13:54:32.000000 yuag-0.0.67/yuag.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-05 13:54:32.000000 yuag-0.0.67/yuag.egg-info/top_level.txt
```

### Comparing `yuag-0.0.66/yuag/__init__.py` & `yuag-0.0.67/yuag/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,14 +193,15 @@
 ```
 \n\n
 
 دوال تحويل الملفات لروابط:
 -----------------
 ```
 imageLink_to_dataurl()
+imageFile_to_dataurl()
 videoFile_to_dataurl()
 ```
 \n\n
 
 رسالة الإنتهاء:
 -----------------
 ```
```

### Comparing `yuag-0.0.66/yuag/yuag.py` & `yuag-0.0.67/yuag/yuag.py`

 * *Files 1% similar despite different names*

```diff
@@ -1477,14 +1477,28 @@
     # التحقق من أن الاستجابة صحيحة
     if response.status_code == 200:
         data_url = f'data:image/{extension};base64,' + base64.b64encode(response.content).decode('utf-8')
         return data_url
     else:
         return error
 
+def imageFile_to_dataurl(image_path, extension="png", error=404):
+    import base64
+
+    try:
+        # قراءة محتوى الملف كبايتس
+        with open(image_path, "rb") as file:
+            image_data = file.read()
+
+        # التحويل إلى رابط data URL
+        data_url = f"data:image/{extension};base64," + base64.b64encode(image_data).decode("utf-8")
+        return data_url
+    except FileNotFoundError:
+        return error
+
 def videoFile_to_dataurl(video_path, error = 404):
     import base64
 
     try:
         # قراءة ملف الفيديو كتسلسل بيانات
         with open(video_path, "rb") as video_file:
             video_data = video_file.read()
```

