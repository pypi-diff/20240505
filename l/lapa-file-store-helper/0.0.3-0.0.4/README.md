# Comparing `tmp/lapa_file_store_helper-0.0.3.tar.gz` & `tmp/lapa_file_store_helper-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lapa_file_store_helper-0.0.3.tar", last modified: Mon Feb  5 04:01:26 2024, max compression
+gzip compressed data, was "lapa_file_store_helper-0.0.4.tar", last modified: Sun May  5 18:48:03 2024, max compression
```

## Comparing `lapa_file_store_helper-0.0.3.tar` & `lapa_file_store_helper-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 04:01:26.585482 lapa_file_store_helper-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-02-05 04:01:26.585482 lapa_file_store_helper-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-02-05 04:01:17.000000 lapa_file_store_helper-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 04:01:26.585482 lapa_file_store_helper-0.0.3/lapa_file_store_helper/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-05 04:01:17.000000 lapa_file_store_helper-0.0.3/lapa_file_store_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-02-05 04:01:17.000000 lapa_file_store_helper-0.0.3/lapa_file_store_helper/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 04:01:26.585482 lapa_file_store_helper-0.0.3/lapa_file_store_helper/data/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-05 04:01:17.000000 lapa_file_store_helper-0.0.3/lapa_file_store_helper/data/config.ini
--rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-02-05 04:01:17.000000 lapa_file_store_helper-0.0.3/lapa_file_store_helper/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 04:01:26.585482 lapa_file_store_helper-0.0.3/lapa_file_store_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-02-05 04:01:26.000000 lapa_file_store_helper-0.0.3/lapa_file_store_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-02-05 04:01:26.000000 lapa_file_store_helper-0.0.3/lapa_file_store_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 04:01:26.000000 lapa_file_store_helper-0.0.3/lapa_file_store_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-05 04:01:26.000000 lapa_file_store_helper-0.0.3/lapa_file_store_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-05 04:01:26.000000 lapa_file_store_helper-0.0.3/lapa_file_store_helper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-05 04:01:26.585482 lapa_file_store_helper-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-02-05 04:01:17.000000 lapa_file_store_helper-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:48:03.795062 lapa_file_store_helper-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-05 18:48:03.795062 lapa_file_store_helper-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-05 18:47:55.000000 lapa_file_store_helper-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:48:03.795062 lapa_file_store_helper-0.0.4/lapa_file_store_helper/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-05 18:47:55.000000 lapa_file_store_helper-0.0.4/lapa_file_store_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-05 18:47:55.000000 lapa_file_store_helper-0.0.4/lapa_file_store_helper/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:48:03.795062 lapa_file_store_helper-0.0.4/lapa_file_store_helper/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-05 18:47:55.000000 lapa_file_store_helper-0.0.4/lapa_file_store_helper/data/config.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-05 18:47:55.000000 lapa_file_store_helper-0.0.4/lapa_file_store_helper/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:48:03.795062 lapa_file_store_helper-0.0.4/lapa_file_store_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-05 18:48:03.000000 lapa_file_store_helper-0.0.4/lapa_file_store_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-05 18:48:03.000000 lapa_file_store_helper-0.0.4/lapa_file_store_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 18:48:03.000000 lapa_file_store_helper-0.0.4/lapa_file_store_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-05 18:48:03.000000 lapa_file_store_helper-0.0.4/lapa_file_store_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-05 18:48:03.000000 lapa_file_store_helper-0.0.4/lapa_file_store_helper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 18:48:03.795062 lapa_file_store_helper-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-05 18:47:55.000000 lapa_file_store_helper-0.0.4/setup.py
```

### Comparing `lapa_file_store_helper-0.0.3/PKG-INFO` & `lapa_file_store_helper-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: lapa_file_store_helper
-Version: 0.0.3
+Version: 0.0.4
 Summary: helper to access the file store layer for my personal server.
 Home-page: https://github.com/thepmsquare/lapa_file_store_helper
-Author: thePmSquare, Lav Sharma
-Author-email: thepmsquare@gmail.com, lavsharma2016@gmail.com
+Author: thePmSquare, Lav Sharma, Amish Palkar
+Author-email: thepmsquare@gmail.com, lavsharma2016@gmail.com, amishpalkar302001@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -34,14 +34,18 @@
 
 ## env
 
 - python>=3.12.0
 
 ## changelog
 
+### v0.0.4
+
+- Added helper function for /delete_file api call.
+
 ### v0.0.3
 
 - Status code check and error raise.
 
 ### v0.0.2
 
 - Configuration is now being read with the help of lapa_commons.
```

### Comparing `lapa_file_store_helper-0.0.3/README.md` & `lapa_file_store_helper-0.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,18 @@
 
 ## env
 
 - python>=3.12.0
 
 ## changelog
 
+### v0.0.4
+
+- Added helper function for /delete_file api call.
+
 ### v0.0.3
 
 - Status code check and error raise.
 
 ### v0.0.2
 
 - Configuration is now being read with the help of lapa_commons.
```

### Comparing `lapa_file_store_helper-0.0.3/lapa_file_store_helper/configuration.py` & `lapa_file_store_helper-0.0.4/lapa_file_store_helper/configuration.py`

 * *Files identical despite different names*

### Comparing `lapa_file_store_helper-0.0.3/lapa_file_store_helper/main.py` & `lapa_file_store_helper-0.0.4/lapa_file_store_helper/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,18 +19,18 @@
                 f"{config_str_lapa_file_store_protocol}://"
                 f"{config_str_lapa_file_store_ip}:{config_int_lapa_file_store_port}"
             )
         except Exception:
             raise
 
     def upload_file_using_file_path(
-        self,
-        file_path: str,
-        file_purpose: str | None = None,
-        system_relative_path: str = "others/misc",
+            self,
+            file_path: str,
+            file_purpose: str | None = None,
+            system_relative_path: str = "others/misc",
     ):
         try:
             endpoint = "upload_file"
             payload = {
                 "file_purpose": file_purpose,
                 "system_relative_pat": system_relative_path,
             }
@@ -45,18 +45,18 @@
                     return response.json()
                 else:
                     response.raise_for_status()
         except Exception:
             raise
 
     def upload_file_using_binary_io(
-        self,
-        file: BinaryIO,
-        file_purpose: str | None = None,
-        system_relative_path: str = "others/misc",
+            self,
+            file: BinaryIO,
+            file_purpose: str | None = None,
+            system_relative_path: str = "others/misc",
     ):
         try:
             endpoint = "upload_file"
             payload = {
                 "file_purpose": file_purpose,
                 "system_relative_path": system_relative_path,
             }
@@ -113,7 +113,29 @@
                     file.write(response.content)
 
                 return downloaded_file_path
             else:
                 response.raise_for_status()
         except Exception:
             raise
+
+    def delete_file(self, list_file_storage_token: list) -> str:
+        """
+        :param list_file_storage_token:
+        :return: filepath
+        """
+        try:
+            endpoint = "delete_file"
+            payload = {
+                "list_file_storage_token": list_file_storage_token,
+            }
+
+            response = requests.delete(
+                self.global_str_lapa_file_store_url_base + "/" + endpoint,
+                params=payload,
+            )
+            if response.status_code == 200:
+                return response.json()
+            else:
+                response.raise_for_status()
+        except Exception:
+            raise
```

### Comparing `lapa_file_store_helper-0.0.3/lapa_file_store_helper.egg-info/PKG-INFO` & `lapa_file_store_helper-0.0.4/lapa_file_store_helper.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: lapa-file-store-helper
-Version: 0.0.3
+Version: 0.0.4
 Summary: helper to access the file store layer for my personal server.
 Home-page: https://github.com/thepmsquare/lapa_file_store_helper
-Author: thePmSquare, Lav Sharma
-Author-email: thepmsquare@gmail.com, lavsharma2016@gmail.com
+Author: thePmSquare, Lav Sharma, Amish Palkar
+Author-email: thepmsquare@gmail.com, lavsharma2016@gmail.com, amishpalkar302001@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -34,14 +34,18 @@
 
 ## env
 
 - python>=3.12.0
 
 ## changelog
 
+### v0.0.4
+
+- Added helper function for /delete_file api call.
+
 ### v0.0.3
 
 - Status code check and error raise.
 
 ### v0.0.2
 
 - Configuration is now being read with the help of lapa_commons.
```

### Comparing `lapa_file_store_helper-0.0.3/setup.py` & `lapa_file_store_helper-0.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import find_packages, setup
 
 package_name = "lapa_file_store_helper"
 
 setup(
     name=package_name,
-    version="0.0.3",
+    version="0.0.4",
     packages=find_packages(),
     package_data={
         package_name: ["data/*"],
     },
     install_requires=[
         "requests>=2.31.0",
         "kiss_headers>=2.4.3",
         "lapa_commons>=0.0.1"
     ],
-    author="thePmSquare, Lav Sharma",
-    author_email="thepmsquare@gmail.com, lavsharma2016@gmail.com",
+    author="thePmSquare, Lav Sharma, Amish Palkar",
+    author_email="thepmsquare@gmail.com, lavsharma2016@gmail.com, amishpalkar302001@gmail.com",
     description="helper to access the file store layer for my personal server.",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     url=f"https://github.com/thepmsquare/{package_name}",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
```

