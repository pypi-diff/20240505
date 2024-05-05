# Comparing `tmp/ghostbase-1.2.1-py3-none-any.whl.zip` & `tmp/ghostbase-1.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3289 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat      688 b- defN 24-May-05 07:01 ghostbase/__init__.py
+Zip file size: 3280 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat      771 b- defN 24-May-05 07:08 ghostbase/__init__.py
 -rw-rw-rw-  2.0 fat     2530 b- defN 24-May-05 07:06 ghostbase/main.py
--rw-rw-rw-  2.0 fat     2805 b- defN 24-May-05 07:06 ghostbase-1.2.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-05 07:06 ghostbase-1.2.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 24-May-05 07:06 ghostbase-1.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      457 b- defN 24-May-05 07:06 ghostbase-1.2.1.dist-info/RECORD
-6 files, 6582 bytes uncompressed, 2463 bytes compressed:  62.6%
+-rw-rw-rw-  2.0 fat     2805 b- defN 24-May-05 07:09 ghostbase-1.2.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-05 07:09 ghostbase-1.2.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 24-May-05 07:09 ghostbase-1.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      457 b- defN 24-May-05 07:09 ghostbase-1.2.2.dist-info/RECORD
+6 files, 6665 bytes uncompressed, 2454 bytes compressed:  63.2%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: ghostbase/__init__.py
 Comment: 
 
 Filename: ghostbase/main.py
 Comment: 
 
-Filename: ghostbase-1.2.1.dist-info/METADATA
+Filename: ghostbase-1.2.2.dist-info/METADATA
 Comment: 
 
-Filename: ghostbase-1.2.1.dist-info/WHEEL
+Filename: ghostbase-1.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: ghostbase-1.2.1.dist-info/top_level.txt
+Filename: ghostbase-1.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: ghostbase-1.2.1.dist-info/RECORD
+Filename: ghostbase-1.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ghostbase/__init__.py

```diff
@@ -1,25 +1,31 @@
 from .main import *
-import sys
 
 
-__all__ = ["create_database","add_user","validate_user","edit_user_pro_status","delete_user","return_pro_status"]
-
 class GhostBase:
     def __init__(self):
         self._url = None
-        self.apikey = None
+        self._apikey = None
 
     @property
     def url(self):
         return self._url
 
     @url.setter
     def url(self, value):
         self._url = value
 
+    @property
+    def apikey(self):
+        return self._apikey
+
+    @apikey.setter
+    def apikey(self, value):
+        self._apikey = value
+
     def __getattr__(self, name):
-        if name == 'url':
-            raise AttributeError(f"'GhostBase' object has no attribute '{name}'. You need to set the URL explicitly.")
+        if name == 'url' or name == 'apikey':
+            raise AttributeError(f"'GhostBase' object has no attribute '{name}'. You need to set the URL and API key explicitly.")
         raise AttributeError(f"module 'ghostbase' has no attribute '{name}'")
 
-sys.modules[__name__] = GhostBase()
+# Instantiate GhostBase as a singleton
+ghostbase = GhostBase()
```

## Comparing `ghostbase-1.2.1.dist-info/METADATA` & `ghostbase-1.2.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghostbase
-Version: 1.2.1
+Version: 1.2.2
 Summary: SelfHosted DB
 Home-page: https://github.com/CyberZenDev/ghostbase
 Author: CyberZenDev
 Author-email: cyberzendev@gmail.com
 License: MIT
 Keywords: flask sqlite database
 Classifier: Development Status :: 5 - Production/Stable
```

