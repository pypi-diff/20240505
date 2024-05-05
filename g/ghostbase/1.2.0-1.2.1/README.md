# Comparing `tmp/ghostbase-1.2.0-py3-none-any.whl.zip` & `tmp/ghostbase-1.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3270 bytes, number of entries: 6
+Zip file size: 3289 bytes, number of entries: 6
 -rw-rw-rw-  2.0 fat      688 b- defN 24-May-05 07:01 ghostbase/__init__.py
--rw-rw-rw-  2.0 fat     2493 b- defN 24-May-05 06:54 ghostbase/main.py
--rw-rw-rw-  2.0 fat     2805 b- defN 24-May-05 07:01 ghostbase-1.2.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-05 07:01 ghostbase-1.2.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 24-May-05 07:01 ghostbase-1.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      457 b- defN 24-May-05 07:01 ghostbase-1.2.0.dist-info/RECORD
-6 files, 6545 bytes uncompressed, 2444 bytes compressed:  62.7%
+-rw-rw-rw-  2.0 fat     2530 b- defN 24-May-05 07:06 ghostbase/main.py
+-rw-rw-rw-  2.0 fat     2805 b- defN 24-May-05 07:06 ghostbase-1.2.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-05 07:06 ghostbase-1.2.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 24-May-05 07:06 ghostbase-1.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      457 b- defN 24-May-05 07:06 ghostbase-1.2.1.dist-info/RECORD
+6 files, 6582 bytes uncompressed, 2463 bytes compressed:  62.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: ghostbase/__init__.py
 Comment: 
 
 Filename: ghostbase/main.py
 Comment: 
 
-Filename: ghostbase-1.2.0.dist-info/METADATA
+Filename: ghostbase-1.2.1.dist-info/METADATA
 Comment: 
 
-Filename: ghostbase-1.2.0.dist-info/WHEEL
+Filename: ghostbase-1.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: ghostbase-1.2.0.dist-info/top_level.txt
+Filename: ghostbase-1.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: ghostbase-1.2.0.dist-info/RECORD
+Filename: ghostbase-1.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ghostbase/main.py

```diff
@@ -5,21 +5,22 @@
 url = None
 
 # API key for authentication
 apikey = None
 
 # Create a SQLite database
 def create_database(db_name):
-    global url
+    global url, apikey  # Import global variables
     endpoint_url = f"{url}/create_db"
     headers = {'X-API-Key': apikey}
     data = {'db_name': db_name}
     response = requests.post(endpoint_url, json=data, headers=headers)
     print(response.text)
 
+
 # Validate a user
 def validate_user(db_name, username, password):
     global url
     endpoint_url = f"{url}/validate_user"
     headers = {'X-API-Key': apikey}
     data = {'db_name': db_name, 'username': username, 'password': password}
     response = requests.post(endpoint_url, json=data, headers=headers)
```

## Comparing `ghostbase-1.2.0.dist-info/METADATA` & `ghostbase-1.2.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghostbase
-Version: 1.2.0
+Version: 1.2.1
 Summary: SelfHosted DB
 Home-page: https://github.com/CyberZenDev/ghostbase
 Author: CyberZenDev
 Author-email: cyberzendev@gmail.com
 License: MIT
 Keywords: flask sqlite database
 Classifier: Development Status :: 5 - Production/Stable
```

