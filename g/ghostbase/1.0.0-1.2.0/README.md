# Comparing `tmp/ghostbase-1.0.0-py3-none-any.whl.zip` & `tmp/ghostbase-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3031 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat      140 b- defN 24-May-05 06:11 ghostbase/__init__.py
--rw-rw-rw-  2.0 fat     2472 b- defN 24-May-05 06:09 ghostbase/main.py
--rw-rw-rw-  2.0 fat     2805 b- defN 24-May-05 06:39 ghostbase-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-05 06:39 ghostbase-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 24-May-05 06:39 ghostbase-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      457 b- defN 24-May-05 06:39 ghostbase-1.0.0.dist-info/RECORD
-6 files, 5976 bytes uncompressed, 2205 bytes compressed:  63.1%
+Zip file size: 3270 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat      688 b- defN 24-May-05 07:01 ghostbase/__init__.py
+-rw-rw-rw-  2.0 fat     2493 b- defN 24-May-05 06:54 ghostbase/main.py
+-rw-rw-rw-  2.0 fat     2805 b- defN 24-May-05 07:01 ghostbase-1.2.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-05 07:01 ghostbase-1.2.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 24-May-05 07:01 ghostbase-1.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      457 b- defN 24-May-05 07:01 ghostbase-1.2.0.dist-info/RECORD
+6 files, 6545 bytes uncompressed, 2444 bytes compressed:  62.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: ghostbase/__init__.py
 Comment: 
 
 Filename: ghostbase/main.py
 Comment: 
 
-Filename: ghostbase-1.0.0.dist-info/METADATA
+Filename: ghostbase-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: ghostbase-1.0.0.dist-info/WHEEL
+Filename: ghostbase-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: ghostbase-1.0.0.dist-info/top_level.txt
+Filename: ghostbase-1.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: ghostbase-1.0.0.dist-info/RECORD
+Filename: ghostbase-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ghostbase/__init__.py

```diff
@@ -1,4 +1,25 @@
 from .main import *
+import sys
+
 
 __all__ = ["create_database","add_user","validate_user","edit_user_pro_status","delete_user","return_pro_status"]
 
+class GhostBase:
+    def __init__(self):
+        self._url = None
+        self.apikey = None
+
+    @property
+    def url(self):
+        return self._url
+
+    @url.setter
+    def url(self, value):
+        self._url = value
+
+    def __getattr__(self, name):
+        if name == 'url':
+            raise AttributeError(f"'GhostBase' object has no attribute '{name}'. You need to set the URL explicitly.")
+        raise AttributeError(f"module 'ghostbase' has no attribute '{name}'")
+
+sys.modules[__name__] = GhostBase()
```

## ghostbase/main.py

```diff
@@ -62,7 +62,10 @@
     result = response.json()  # Extract JSON content from response
     pro_status = result.get('pro_status')  # Get the value of 'pro_status' from the response
     if pro_status == [1]:  # Assuming 'pro_status' is a list containing a single integer
         print("True")
     else:
         print("False")
 
+
+
+create_database()
```

## Comparing `ghostbase-1.0.0.dist-info/METADATA` & `ghostbase-1.2.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghostbase
-Version: 1.0.0
+Version: 1.2.0
 Summary: SelfHosted DB
 Home-page: https://github.com/CyberZenDev/ghostbase
 Author: CyberZenDev
 Author-email: cyberzendev@gmail.com
 License: MIT
 Keywords: flask sqlite database
 Classifier: Development Status :: 5 - Production/Stable
```

