# Comparing `tmp/ghostbase-1.2.4-py3-none-any.whl.zip` & `tmp/ghostbase-1.2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3335 bytes, number of entries: 6
+Zip file size: 3304 bytes, number of entries: 6
 -rw-rw-rw-  2.0 fat      891 b- defN 24-May-05 07:12 ghostbase/__init__.py
--rw-rw-rw-  2.0 fat     2509 b- defN 24-May-05 07:12 ghostbase/main.py
--rw-rw-rw-  2.0 fat     2805 b- defN 24-May-05 07:13 ghostbase-1.2.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-05 07:13 ghostbase-1.2.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 24-May-05 07:13 ghostbase-1.2.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      457 b- defN 24-May-05 07:13 ghostbase-1.2.4.dist-info/RECORD
-6 files, 6764 bytes uncompressed, 2509 bytes compressed:  62.9%
+-rw-rw-rw-  2.0 fat     2495 b- defN 24-May-05 07:15 ghostbase/main.py
+-rw-rw-rw-  2.0 fat     2805 b- defN 24-May-05 07:15 ghostbase-1.2.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-05 07:15 ghostbase-1.2.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 24-May-05 07:15 ghostbase-1.2.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      457 b- defN 24-May-05 07:15 ghostbase-1.2.5.dist-info/RECORD
+6 files, 6750 bytes uncompressed, 2478 bytes compressed:  63.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: ghostbase/__init__.py
 Comment: 
 
 Filename: ghostbase/main.py
 Comment: 
 
-Filename: ghostbase-1.2.4.dist-info/METADATA
+Filename: ghostbase-1.2.5.dist-info/METADATA
 Comment: 
 
-Filename: ghostbase-1.2.4.dist-info/WHEEL
+Filename: ghostbase-1.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: ghostbase-1.2.4.dist-info/top_level.txt
+Filename: ghostbase-1.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: ghostbase-1.2.4.dist-info/RECORD
+Filename: ghostbase-1.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ghostbase/main.py

```diff
@@ -1,69 +1,66 @@
 import requests
 
 # Base URL of the Flask server
 # Example base url - Needs to be set by the client - base_url = "http://localhost:5000"
-url = None
+url = "https://db.ghostai.me/"
 
-# API key for authentication
-apikey = None
 # Create a SQLite database
-def create_database(db_name):
-    global url, apikey  # Import global variables
+def create_database(db_name, apikey):
+    global url
     endpoint_url = f"{url}/create_db"
     headers = {'X-API-Key': apikey}
     data = {'db_name': db_name}
     response = requests.post(endpoint_url, json=data, headers=headers)
     print(response.text)
 
 
 # Validate a user
-def validate_user(db_name, username, password):
+def validate_user(db_name, username, password, apikey):
     global url
     endpoint_url = f"{url}/validate_user"
     headers = {'X-API-Key': apikey}
     data = {'db_name': db_name, 'username': username, 'password': password}
     response = requests.post(endpoint_url, json=data, headers=headers)
     print(response.text)
 
 # Add a new user
-def add_user(db_name, username, email, password, pro_status):
+def add_user(db_name, username, email, password, pro_status, apikey):
     global url
     endpoint_url = f"{url}/add_user"
     headers = {'X-API-Key': apikey}
     data = {'db_name': db_name, 'username': username, 'email': email, 'password': password, 'pro_status': pro_status}
     response = requests.post(endpoint_url, json=data, headers=headers)
     print(response.text)
 
 # Delete a user
-def delete_user(db_name, username):
+def delete_user(db_name, username, apikey):
     global url
     endpoint_url = f"{url}/delete_user"
     headers = {'X-API-Key': apikey}
     data = {'db_name': db_name, 'username': username}
     response = requests.post(endpoint_url, json=data, headers=headers)
     print(response.text)
 
 # Edit user's pro status
-def edit_user_pro_status(db_name, username, pro_status):
+def edit_user_pro_status(db_name, username, pro_status, apikey):
     global url
     endpoint_url = f"{url}/edit_user_pro_status"
     headers = {'X-API-Key': apikey}
     data = {'db_name': db_name, 'username': username, 'pro_status': pro_status}
     response = requests.post(endpoint_url, json=data, headers=headers)
     print(response.text)
 
 
-def return_pro_status(db_name, username):
+def return_pro_status(db_name, username, apikey):
     global url
     endpoint_url = f"{url}/return_pro_status"
     headers = {'X-API-Key': apikey}
     data = {'db_name': db_name, 'username': username}
     response = requests.post(endpoint_url, json=data, headers=headers)
     result = response.json()  # Extract JSON content from response
     pro_status = result.get('pro_status')  # Get the value of 'pro_status' from the response
     if pro_status == [1]:  # Assuming 'pro_status' is a list containing a single integer
         print("True")
     else:
         print("False")
 
-
```

## Comparing `ghostbase-1.2.4.dist-info/METADATA` & `ghostbase-1.2.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghostbase
-Version: 1.2.4
+Version: 1.2.5
 Summary: SelfHosted DB
 Home-page: https://github.com/CyberZenDev/ghostbase
 Author: CyberZenDev
 Author-email: cyberzendev@gmail.com
 License: MIT
 Keywords: flask sqlite database
 Classifier: Development Status :: 5 - Production/Stable
```

