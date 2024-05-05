# Comparing `tmp/lapa_file_store-0.0.8.tar.gz` & `tmp/lapa_file_store-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lapa_file_store-0.0.8.tar", last modified: Fri Apr 12 17:16:01 2024, max compression
+gzip compressed data, was "lapa_file_store-0.0.9.tar", last modified: Sun May  5 14:51:17 2024, max compression
```

## Comparing `lapa_file_store-0.0.8.tar` & `lapa_file_store-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:16:01.002038 lapa_file_store-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-12 17:16:01.002038 lapa_file_store-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-12 17:15:52.000000 lapa_file_store-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:16:00.998038 lapa_file_store-0.0.8/lapa_file_store/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:15:52.000000 lapa_file_store-0.0.8/lapa_file_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-12 17:15:52.000000 lapa_file_store-0.0.8/lapa_file_store/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:16:01.002038 lapa_file_store-0.0.8/lapa_file_store/data/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-12 17:15:52.000000 lapa_file_store-0.0.8/lapa_file_store/data/config.ini
--rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-04-12 17:15:52.000000 lapa_file_store-0.0.8/lapa_file_store/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:16:01.002038 lapa_file_store-0.0.8/lapa_file_store/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-12 17:15:52.000000 lapa_file_store-0.0.8/lapa_file_store/utils/Helper.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:15:52.000000 lapa_file_store-0.0.8/lapa_file_store/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:16:01.002038 lapa_file_store-0.0.8/lapa_file_store.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-12 17:16:00.000000 lapa_file_store-0.0.8/lapa_file_store.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-12 17:16:00.000000 lapa_file_store-0.0.8/lapa_file_store.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:16:00.000000 lapa_file_store-0.0.8/lapa_file_store.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-12 17:16:00.000000 lapa_file_store-0.0.8/lapa_file_store.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-12 17:16:00.000000 lapa_file_store-0.0.8/lapa_file_store.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 17:16:01.002038 lapa_file_store-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-12 17:15:52.000000 lapa_file_store-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:51:17.862229 lapa_file_store-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-05 14:51:17.862229 lapa_file_store-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-05 14:51:08.000000 lapa_file_store-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:51:17.858229 lapa_file_store-0.0.9/lapa_file_store/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 14:51:08.000000 lapa_file_store-0.0.9/lapa_file_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-05 14:51:08.000000 lapa_file_store-0.0.9/lapa_file_store/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:51:17.858229 lapa_file_store-0.0.9/lapa_file_store/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-05 14:51:08.000000 lapa_file_store-0.0.9/lapa_file_store/data/config.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     6921 2024-05-05 14:51:08.000000 lapa_file_store-0.0.9/lapa_file_store/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:51:17.862229 lapa_file_store-0.0.9/lapa_file_store/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-05-05 14:51:08.000000 lapa_file_store-0.0.9/lapa_file_store/utils/Helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 14:51:08.000000 lapa_file_store-0.0.9/lapa_file_store/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:51:17.858229 lapa_file_store-0.0.9/lapa_file_store.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-05 14:51:17.000000 lapa_file_store-0.0.9/lapa_file_store.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-05 14:51:17.000000 lapa_file_store-0.0.9/lapa_file_store.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 14:51:17.000000 lapa_file_store-0.0.9/lapa_file_store.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-05 14:51:17.000000 lapa_file_store-0.0.9/lapa_file_store.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-05 14:51:17.000000 lapa_file_store-0.0.9/lapa_file_store.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 14:51:17.862229 lapa_file_store-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-05 14:51:08.000000 lapa_file_store-0.0.9/setup.py
```

### Comparing `lapa_file_store-0.0.8/PKG-INFO` & `lapa_file_store-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: lapa_file_store
-Version: 0.0.8
+Version: 0.0.9
 Summary: file storage layer for my personal server.
 Home-page: https://github.com/adityashetty35/lapa_file_store
-Author: Aaditya sangishetty, thePmSquare
-Author-email: adityashetty35@gmail.com, thepmsquare@gmail.com
+Author: Aaditya sangishetty, thePmSquare, Amish Palkar
+Author-email: adityashetty35@gmail.com, thepmsquare@gmail.com, amishpalkar302001@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -31,14 +31,18 @@
 
 ## env
 
 - python>=3.12.0
 
 ## changelog
 
+### v0.0.9
+
+- Added /delete_file endpoint.
+
 ### v0.0.8
 
 - update import logic from lapa_database_structure.
 
 ### v0.0.7
 
 - bug fix in utils->Helper.py import.
```

### Comparing `lapa_file_store-0.0.8/README.md` & `lapa_file_store-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 
 ## env
 
 - python>=3.12.0
 
 ## changelog
 
+### v0.0.9
+
+- Added /delete_file endpoint.
+
 ### v0.0.8
 
 - update import logic from lapa_database_structure.
 
 ### v0.0.7
 
 - bug fix in utils->Helper.py import.
```

### Comparing `lapa_file_store-0.0.8/lapa_file_store/configuration.py` & `lapa_file_store-0.0.9/lapa_file_store/configuration.py`

 * *Files identical despite different names*

### Comparing `lapa_file_store-0.0.8/lapa_file_store/main.py` & `lapa_file_store-0.0.9/lapa_file_store/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import mimetypes
 import os
 import uuid
-from typing import Annotated
+from typing import Annotated, List
 
 from fastapi import FastAPI, UploadFile, status, Form
 from fastapi.exceptions import HTTPException
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.responses import FileResponse, JSONResponse
 from uvicorn import run
 
 from lapa_file_store.configuration import (
     config_int_host_port,
     config_str_host_ip,
     global_absolute_path_local_storage,
     global_object_square_logger,
     config_str_module_name
 )
-from lapa_file_store.utils.Helper import create_entry_in_file_store, get_file_row
+from lapa_file_store.utils.Helper import create_entry_in_file_store, get_file_row, edit_file_delete_status
 
 app = FastAPI()
 
 app.add_middleware(
     CORSMiddleware,
     allow_origins=["*"],
     allow_methods=["*"],
@@ -110,18 +110,20 @@
     try:
         local_dict_file_row = get_file_row(file_storage_token)
         local_string_system_absolute_file_path = os.path.join(
             global_absolute_path_local_storage,
             os.sep.join(local_dict_file_row["file_system_relative_path"].split("/")),
             local_dict_file_row["file_system_file_name_with_extension"],
         )
-        # Get content type
-        content_type, _ = mimetypes.guess_type(local_string_system_absolute_file_path)
 
-        if local_string_system_absolute_file_path:
+        # check file is deleted
+        if not local_dict_file_row["file_is_deleted"] and local_string_system_absolute_file_path:
+            # Get content type
+            content_type, _ = mimetypes.guess_type(local_string_system_absolute_file_path)
+
             return FileResponse(
                 local_string_system_absolute_file_path,
                 media_type=content_type,
                 filename=local_dict_file_row["file_name_with_extension"],
             )
         else:
             raise HTTPException(
@@ -130,13 +132,49 @@
     except HTTPException:
         raise
     except Exception as e:
         raise HTTPException(
             status_code=status.HTTP_500_INTERNAL_SERVER_ERROR, detail=str(e)
         )
 
+
+@app.delete("/delete_file", status_code=status.HTTP_200_OK)
+@global_object_square_logger.async_auto_logger
+async def delete_file(list_file_storage_token: List[str]):
+    deleted_file_storage_token = []
+    try:
+        for file_storage_token in list_file_storage_token:
+            # get file path
+            local_dict_file_row = get_file_row(file_storage_token)
+            local_string_system_absolute_file_path = os.path.join(
+                global_absolute_path_local_storage,
+                os.sep.join(local_dict_file_row["file_system_relative_path"].split("/")),
+                local_dict_file_row["file_system_file_name_with_extension"],
+            )
+
+            # delete file
+            if os.path.exists(local_string_system_absolute_file_path):
+                os.remove(local_string_system_absolute_file_path)
+
+            # update file deleted status and timestamp
+            update_status_response = edit_file_delete_status(file_storage_token)
+
+            deleted_file_storage_token.append(file_storage_token)
+
+        # Additional information you want to include
+        additional_info = {"DeletedFileStorageToken": deleted_file_storage_token}
+
+        # Return JSONResponse additional information
+        return JSONResponse(content={"additional_info": additional_info})
+    except HTTPException:
+        raise
+    except Exception as e:
+        raise HTTPException(
+            status_code=status.HTTP_500_INTERNAL_SERVER_ERROR, detail=str(e)
+        )
+
 
 if __name__ == "__main__":
     try:
         run(app, host=config_str_host_ip, port=config_int_host_port)
     except Exception as exc:
         global_object_square_logger.logger.critical(exc, exc_info=True)
```

### Comparing `lapa_file_store-0.0.8/lapa_file_store/utils/Helper.py` & `lapa_file_store-0.0.9/lapa_file_store/utils/Helper.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from datetime import datetime, timezone
+
 from fastapi import status
 from fastapi.exceptions import HTTPException
 from lapa_database_helper.main import LAPADatabaseHelper
 from lapa_database_structure.lapa.file_storage.tables import local_string_database_name, local_string_schema_name, File
 
 from lapa_file_store.configuration import global_object_square_logger
 
@@ -65,7 +67,54 @@
             raise HTTPException(
                 status_code=status.HTTP_400_BAD_REQUEST,
                 detail=f"incorrect file_storage_token:{file_storage_token}",
             )
 
     except Exception as e:
         raise e
+
+
+def edit_file_delete_status(file_storage_token):
+    try:
+        filters = {File.file_storage_token.name: file_storage_token}
+
+        # Get the current timestamp
+        timestamp = datetime.now(timezone.utc)
+        formatted_timestamp = timestamp.strftime("%Y-%m-%d %H:%M:%S.%f+00")
+
+        data = {File.file_is_deleted.name: True, File.file_date_deleted.name: formatted_timestamp}
+
+        response = local_object_lapa_database_helper.edit_rows(
+            filters=filters,
+            data=data,
+            database_name=local_string_database_name,
+            schema_name=local_string_schema_name,
+            table_name=File.__tablename__,
+            ignore_filters_and_edit_all=False
+        )
+
+        if isinstance(response, list) and len(response) == 1 and response[0]:
+            file_data = response[0]
+            if File.file_storage_token.name in file_data and file_data[
+                File.file_storage_token.name] == file_storage_token:
+                return file_data
+            else:
+                raise HTTPException(
+                    status_code=status.HTTP_400_BAD_REQUEST,
+                    detail=f"incorrect file_storage_token:{file_storage_token}",
+                )
+        elif len(response) > 1:
+            global_object_square_logger.logger.warning(
+                f"Multiple files with same file_storage_token: {file_storage_token}"
+            )
+
+            raise HTTPException(
+                status_code=status.HTTP_400_BAD_REQUEST,
+                detail=f"incorrect file_storage_token:{file_storage_token}",
+            )
+        else:
+            raise HTTPException(
+                status_code=status.HTTP_400_BAD_REQUEST,
+                detail=f"incorrect file_storage_token:{file_storage_token}",
+            )
+    except Exception as e:
+        raise e
```

### Comparing `lapa_file_store-0.0.8/lapa_file_store.egg-info/PKG-INFO` & `lapa_file_store-0.0.9/lapa_file_store.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: lapa-file-store
-Version: 0.0.8
+Version: 0.0.9
 Summary: file storage layer for my personal server.
 Home-page: https://github.com/adityashetty35/lapa_file_store
-Author: Aaditya sangishetty, thePmSquare
-Author-email: adityashetty35@gmail.com, thepmsquare@gmail.com
+Author: Aaditya sangishetty, thePmSquare, Amish Palkar
+Author-email: adityashetty35@gmail.com, thepmsquare@gmail.com, amishpalkar302001@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -31,14 +31,18 @@
 
 ## env
 
 - python>=3.12.0
 
 ## changelog
 
+### v0.0.9
+
+- Added /delete_file endpoint.
+
 ### v0.0.8
 
 - update import logic from lapa_database_structure.
 
 ### v0.0.7
 
 - bug fix in utils->Helper.py import.
```

### Comparing `lapa_file_store-0.0.8/setup.py` & `lapa_file_store-0.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from setuptools import find_packages, setup
 
 package_name = "lapa_file_store"
 
 setup(
     name=package_name,
-    version="0.0.8",
+    version="0.0.9",
     packages=find_packages(),
     package_data={
         package_name: ["data/*", "pydantic_models/*"],
     },
     install_requires=[
         "uvicorn>=0.24.0.post1",
         "fastapi>=0.104.1",
         "python-multipart>=0.0.6",
         "square_logger~=1.0",
         "pydantic>=2.5.3",
         "lapa_database_helper>=0.0.3",
         "lapa_commons>=0.0.1",
         "lapa_database_structure>=0.0.6"
     ],
-    author="Aaditya sangishetty, thePmSquare",
-    author_email="adityashetty35@gmail.com, thepmsquare@gmail.com",
+    author="Aaditya sangishetty, thePmSquare, Amish Palkar",
+    author_email="adityashetty35@gmail.com, thepmsquare@gmail.com, amishpalkar302001@gmail.com",
     description="file storage layer for my personal server.",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     url=f"https://github.com/adityashetty35/{package_name}",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
```

