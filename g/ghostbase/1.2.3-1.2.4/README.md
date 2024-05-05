# Comparing `tmp/ghostbase-1.2.3-py3-none-any.whl.zip` & `tmp/ghostbase-1.2.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3029 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat       27 b- defN 24-May-05 07:10 ghostbase/__init__.py
--rw-rw-rw-  2.0 fat     2588 b- defN 24-May-05 07:10 ghostbase/main.py
--rw-rw-rw-  2.0 fat     2805 b- defN 24-May-05 07:11 ghostbase-1.2.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-05 07:11 ghostbase-1.2.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 24-May-05 07:11 ghostbase-1.2.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      456 b- defN 24-May-05 07:11 ghostbase-1.2.3.dist-info/RECORD
-6 files, 5978 bytes uncompressed, 2203 bytes compressed:  63.1%
+Zip file size: 3335 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat      891 b- defN 24-May-05 07:12 ghostbase/__init__.py
+-rw-rw-rw-  2.0 fat     2509 b- defN 24-May-05 07:12 ghostbase/main.py
+-rw-rw-rw-  2.0 fat     2805 b- defN 24-May-05 07:13 ghostbase-1.2.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-05 07:13 ghostbase-1.2.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 24-May-05 07:13 ghostbase-1.2.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      457 b- defN 24-May-05 07:13 ghostbase-1.2.4.dist-info/RECORD
+6 files, 6764 bytes uncompressed, 2509 bytes compressed:  62.9%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: ghostbase/__init__.py
 Comment: 
 
 Filename: ghostbase/main.py
 Comment: 
 
-Filename: ghostbase-1.2.3.dist-info/METADATA
+Filename: ghostbase-1.2.4.dist-info/METADATA
 Comment: 
 
-Filename: ghostbase-1.2.3.dist-info/WHEEL
+Filename: ghostbase-1.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: ghostbase-1.2.3.dist-info/top_level.txt
+Filename: ghostbase-1.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: ghostbase-1.2.3.dist-info/RECORD
+Filename: ghostbase-1.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ghostbase/__init__.py

```diff
@@ -1,3 +1,32 @@
 from .main import *
 
-    
+__all__ = ["create_database", "add_user", "validate_user", "edit_user_pro_status", "delete_user", "return_pro_status"]
+
+class GhostBase:
+    def __init__(self):
+        self._url = None
+        self._apikey = None
+
+    @property
+    def url(self):
+        return self._url
+
+    @url.setter
+    def url(self, value):
+        self._url = value
+
+    @property
+    def apikey(self):
+        return self._apikey
+
+    @apikey.setter
+    def apikey(self, value):
+        self._apikey = value
+
+    def __getattr__(self, name):
+        if name == 'url' or name == 'apikey':
+            raise AttributeError(f"'GhostBase' object has no attribute '{name}'. You need to set the URL and API key explicitly.")
+        raise AttributeError(f"module 'ghostbase' has no attribute '{name}'")
+
+# Instantiate GhostBase as a singleton
+ghostbase = GhostBase()
```

## ghostbase/main.py

```diff
@@ -1,16 +1,15 @@
 import requests
 
 # Base URL of the Flask server
 # Example base url - Needs to be set by the client - base_url = "http://localhost:5000"
-url = "https://db.ghostai.me/"
+url = None
 
 # API key for authentication
-apikey = "8dab6627008b162e707171789c0c98c5dc5ef82c"
-
+apikey = None
 # Create a SQLite database
 def create_database(db_name):
     global url, apikey  # Import global variables
     endpoint_url = f"{url}/create_db"
     headers = {'X-API-Key': apikey}
     data = {'db_name': db_name}
     response = requests.post(endpoint_url, json=data, headers=headers)
@@ -64,9 +63,7 @@
     pro_status = result.get('pro_status')  # Get the value of 'pro_status' from the response
     if pro_status == [1]:  # Assuming 'pro_status' is a list containing a single integer
         print("True")
     else:
         print("False")
 
 
-
-create_database()
```

## Comparing `ghostbase-1.2.3.dist-info/METADATA` & `ghostbase-1.2.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghostbase
-Version: 1.2.3
+Version: 1.2.4
 Summary: SelfHosted DB
 Home-page: https://github.com/CyberZenDev/ghostbase
 Author: CyberZenDev
 Author-email: cyberzendev@gmail.com
 License: MIT
 Keywords: flask sqlite database
 Classifier: Development Status :: 5 - Production/Stable
```

