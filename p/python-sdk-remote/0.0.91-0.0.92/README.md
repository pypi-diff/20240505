# Comparing `tmp/python_sdk_remote-0.0.91.tar.gz` & `tmp/python_sdk_remote-0.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_sdk_remote-0.0.91.tar", last modified: Thu May  2 04:06:52 2024, max compression
+gzip compressed data, was "python_sdk_remote-0.0.92.tar", last modified: Sun May  5 08:19:47 2024, max compression
```

## Comparing `python_sdk_remote-0.0.91.tar` & `python_sdk_remote-0.0.92.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 04:06:52.888249 python_sdk_remote-0.0.91/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-02 04:06:52.888249 python_sdk_remote-0.0.91/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-02 04:06:39.000000 python_sdk_remote-0.0.91/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-02 04:06:39.000000 python_sdk_remote-0.0.91/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 04:06:52.884249 python_sdk_remote-0.0.91/python_sdk_remote/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 04:06:52.884249 python_sdk_remote-0.0.91/python_sdk_remote/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 04:06:39.000000 python_sdk_remote-0.0.91/python_sdk_remote/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-02 04:06:39.000000 python_sdk_remote-0.0.91/python_sdk_remote/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-02 04:06:39.000000 python_sdk_remote-0.0.91/python_sdk_remote/src/item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-02 04:06:39.000000 python_sdk_remote-0.0.91/python_sdk_remote/src/mini_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-02 04:06:39.000000 python_sdk_remote-0.0.91/python_sdk_remote/src/our_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-02 04:06:39.000000 python_sdk_remote-0.0.91/python_sdk_remote/src/unified_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    12325 2024-05-02 04:06:39.000000 python_sdk_remote-0.0.91/python_sdk_remote/src/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-02 04:06:39.000000 python_sdk_remote-0.0.91/python_sdk_remote/src/valid_json_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-02 04:06:39.000000 python_sdk_remote-0.0.91/python_sdk_remote/src/validate_environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 04:06:52.888249 python_sdk_remote-0.0.91/python_sdk_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-02 04:06:52.000000 python_sdk_remote-0.0.91/python_sdk_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-02 04:06:52.000000 python_sdk_remote-0.0.91/python_sdk_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 04:06:52.000000 python_sdk_remote-0.0.91/python_sdk_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-02 04:06:52.000000 python_sdk_remote-0.0.91/python_sdk_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 04:06:52.000000 python_sdk_remote-0.0.91/python_sdk_remote.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 04:06:52.888249 python_sdk_remote-0.0.91/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-02 04:06:39.000000 python_sdk_remote-0.0.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:19:47.066531 python_sdk_remote-0.0.92/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-05 08:19:47.066531 python_sdk_remote-0.0.92/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-05 08:19:34.000000 python_sdk_remote-0.0.92/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-05 08:19:34.000000 python_sdk_remote-0.0.92/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:19:47.062531 python_sdk_remote-0.0.92/python_sdk_remote/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:19:47.066531 python_sdk_remote-0.0.92/python_sdk_remote/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 08:19:34.000000 python_sdk_remote-0.0.92/python_sdk_remote/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-05 08:19:34.000000 python_sdk_remote-0.0.92/python_sdk_remote/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-05-05 08:19:34.000000 python_sdk_remote-0.0.92/python_sdk_remote/src/http_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-05 08:19:34.000000 python_sdk_remote-0.0.92/python_sdk_remote/src/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-05 08:19:34.000000 python_sdk_remote-0.0.92/python_sdk_remote/src/mini_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-05 08:19:34.000000 python_sdk_remote-0.0.92/python_sdk_remote/src/our_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-05 08:19:34.000000 python_sdk_remote-0.0.92/python_sdk_remote/src/unified_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-05-05 08:19:34.000000 python_sdk_remote-0.0.92/python_sdk_remote/src/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-05 08:19:34.000000 python_sdk_remote-0.0.92/python_sdk_remote/src/valid_json_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-05 08:19:34.000000 python_sdk_remote-0.0.92/python_sdk_remote/src/validate_environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:19:47.066531 python_sdk_remote-0.0.92/python_sdk_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-05 08:19:47.000000 python_sdk_remote-0.0.92/python_sdk_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-05 08:19:47.000000 python_sdk_remote-0.0.92/python_sdk_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 08:19:47.000000 python_sdk_remote-0.0.92/python_sdk_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-05 08:19:47.000000 python_sdk_remote-0.0.92/python_sdk_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-05 08:19:47.000000 python_sdk_remote-0.0.92/python_sdk_remote.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 08:19:47.066531 python_sdk_remote-0.0.92/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-05 08:19:34.000000 python_sdk_remote-0.0.92/setup.py
```

### Comparing `python_sdk_remote-0.0.91/PKG-INFO` & `python_sdk_remote-0.0.92/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sdk-remote
-Version: 0.0.91
+Version: 0.0.92
 Summary: PyPI Package for Circles Python SDK Local Python
 Home-page: https://github.com/circles-zone/python-sdk-remote-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `python_sdk_remote-0.0.91/README.md` & `python_sdk_remote-0.0.92/README.md`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.91/python_sdk_remote/src/constants.py` & `python_sdk_remote-0.0.92/python_sdk_remote/src/constants.py`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.91/python_sdk_remote/src/mini_logger.py` & `python_sdk_remote-0.0.92/python_sdk_remote/src/mini_logger.py`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.91/python_sdk_remote/src/our_object.py` & `python_sdk_remote-0.0.92/python_sdk_remote/src/our_object.py`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.91/python_sdk_remote/src/unified_json.py` & `python_sdk_remote-0.0.92/python_sdk_remote/src/unified_json.py`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.91/python_sdk_remote/src/utilities.py` & `python_sdk_remote-0.0.92/python_sdk_remote/src/utilities.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-import json
 import os
 from datetime import date, datetime, time, timedelta
 from dotenv import load_dotenv
 from url_remote.environment_name_enum import EnvironmentName
 from urllib.parse import urlparse
-from http_constants import status
 
+from .http_response import (create_authorization_http_headers, get_user_jwt_from_event,  # noqa - used for backwards compatibility
+                            create_return_http_headers, create_error_http_response, create_ok_http_response,
+                            create_http_body)
 from .mini_logger import MiniLogger as logger
 
 load_dotenv()
 
 
 def timedelta_to_time_format(time_delta: timedelta) -> str:
     """
@@ -47,86 +48,79 @@
     return formatted_time
 
 
 def is_valid_time_range(time_range: tuple) -> bool:
     """
     Validate that the time range is in the format 'HH:MM:SS'.
     """
-    IS_VALID_TIME_RANGE_METHOD_NAME = "is_valid_time_range"
-    logger.start(IS_VALID_TIME_RANGE_METHOD_NAME, object={
-        "time_range": time_range.__str__()})
+    logger.start(object={"time_range": time_range.__str__()})
     if len(time_range) != 2:
-        logger.end(IS_VALID_TIME_RANGE_METHOD_NAME, object={
-            "is_valid_time_range_result": False, "reason": "len(time_range) != 2"})
+        logger.end(object={"is_valid_time_range_result": False, "reason": "len(time_range) != 2"})
         return False
 
     for time_obj in time_range:
         if not isinstance(time_obj, time):
-            logger.end(IS_VALID_TIME_RANGE_METHOD_NAME, object={
+            logger.end(object={
                 "is_valid_time_range_result": False, "reason": "time_range contains non-time objects"})
             return False
         time_str = time_obj.strftime('%H:%M:%S')
         if time_obj.strftime('%H:%M:%S') != time_str:
-            logger.end(IS_VALID_TIME_RANGE_METHOD_NAME, object={
+            logger.end(object={
                 "is_valid_time_range_result": False, "reason": "time_range contains invalid time format"})
             return False
 
-    logger.end(IS_VALID_TIME_RANGE_METHOD_NAME, object={
-        "is_valid_time_range_result": True})
+    logger.end(object={"is_valid_time_range_result": True})
     return True
 
 
+# TODO shall we also use Url type and not only str? - Strongly Type which I prefer
+#   (if yes we should change it also in all the calls to this function)
 def validate_url(url: str):
+    logger.start(object={"url": url})
     if url is not None or url != "":
         parsed_url = urlparse(url)
-        return parsed_url.scheme and parsed_url.netloc
-    return True
+        is_valid_url = parsed_url.scheme and parsed_url.netloc
+    else:
+        is_valid_url = True
+    logger.end(object={"is_valid_url": is_valid_url})
+    return is_valid_url
 
 
 def is_valid_date_range(date_range: tuple) -> bool:
     """
     Validate that the date range is in the format 'YYYY-MM-DD'.
     """
-    IS_VALID_DATE_RANGE_METHOD_NAME = "is_valid_date_range"
-    logger.start(IS_VALID_DATE_RANGE_METHOD_NAME, object={
-        "date_range": date_range.__str__()})
+    logger.start(object={"date_range": date_range.__str__()})
     if len(date_range) != 2:
-        logger.end(IS_VALID_DATE_RANGE_METHOD_NAME, object={
-            "is_valid_date_range_result": False, "reason": "len(date_range) != 2"})
+        logger.end(object={"is_valid_date_range_result": False, "reason": "len(date_range) != 2"})
         return False
 
     for date_obj in date_range:
         if not isinstance(date_obj, date):
-            logger.end(IS_VALID_DATE_RANGE_METHOD_NAME, object={
+            logger.end(object={
                 "is_valid_date_range_result": False, "reason": "date_range contains non-date objects"})
             return False
-    logger.end(IS_VALID_DATE_RANGE_METHOD_NAME, object={
-        "is_valid_date_range_result": True})
+    logger.end(object={"is_valid_date_range_result": True})
     return True
 
 
 def is_valid_datetime_range(datetime_range: tuple) -> bool:
     """
     Validate that the datetime range is in the format 'YYYY-MM-DD HH:MM:SS'.
     """
-    IS_VALID_DATETIME_RANGE_METHOD_NAME = "is_valid_datetime_range"
-    logger.start(IS_VALID_DATETIME_RANGE_METHOD_NAME, object={
-        "datetime_range": datetime_range.__str__()})
+    logger.start(object={"datetime_range": datetime_range.__str__()})
     if len(datetime_range) != 2:
-        logger.end(IS_VALID_DATETIME_RANGE_METHOD_NAME, object={
-            "is_valid_datetime_range_result": False, "reason": "len(datetime_range) != 2"})
+        logger.end(object={"is_valid_datetime_range_result": False, "reason": "len(datetime_range) != 2"})
         return False
 
     for datetime_obj in datetime_range:
         if not isinstance(datetime_obj, datetime):
-            logger.end(IS_VALID_DATETIME_RANGE_METHOD_NAME, object={
-                "is_valid_datetime_range_result": False, "reason": "datetime_range contains non-datetime objects"})
+            logger.end(object={"is_valid_datetime_range_result": False, "reason": "datetime_range contains non-datetime objects"})
             return False
-    logger.end(IS_VALID_DATETIME_RANGE_METHOD_NAME, object={
-        "is_valid_datetime_range_result": True})
+    logger.end(object={"is_valid_datetime_range_result": True})
     return True
 
 
 def is_list_of_dicts(obj: object) -> bool:
     """
     Check if an object is a list of dictionaries.
 
@@ -144,58 +138,55 @@
 
         >>> is_list_of_dicts([1, 2, 3])
         False
 
         >>> is_list_of_dicts(1)
         False
     """
-    IS_LIST_OF_DICTS_FUNCTION_NAME = "is_list_of_dicts"
-    logger.start(IS_LIST_OF_DICTS_FUNCTION_NAME, object={"obj": obj})
+    logger.start(object={"obj": obj})
     try:
         if not isinstance(obj, list):
             is_list_of_dicts_result = False
-            logger.end(IS_LIST_OF_DICTS_FUNCTION_NAME, object={
-                "is_list_of_dicts_result": is_list_of_dicts_result})
+            logger.end(object={"is_list_of_dicts_result": is_list_of_dicts_result})
             return is_list_of_dicts_result
         for item in obj:
             if not isinstance(item, dict):
                 is_list_of_dicts_result = False
-                logger.end(IS_LIST_OF_DICTS_FUNCTION_NAME, object={
+                logger.end(object={
                     "is_list_of_dicts_result": is_list_of_dicts_result})
                 return is_list_of_dicts_result
         is_list_of_dicts_result = True
-        logger.end(IS_LIST_OF_DICTS_FUNCTION_NAME, object={
+        logger.end(object={
             "is_list_of_dicts_result": is_list_of_dicts_result})
         return is_list_of_dicts_result
     except Exception as exception:
-        logger.exception(IS_LIST_OF_DICTS_FUNCTION_NAME, exception)
-        logger.end(IS_LIST_OF_DICTS_FUNCTION_NAME)
+        logger.exception(object=exception)
+        logger.end()
         raise
 
 
 def is_time_in_time_range(check_time: time, time_range: tuple) -> bool:
     """
     Check if the given time is within the specified time range.
 
     Parameters:
         check_time (str): The time to check in 'HH:MM:SS' format.
         time_range (tuple): A tuple containing start and end times in 'HH:MM:SS' format.
 
     Returns:
         bool: True if the check_time is within the time range, False otherwise.
     """
-    IS_TIME_IN_TIME_RANGE_METHOD_NAME = "is_time_in_time_range"
-    logger.start(IS_TIME_IN_TIME_RANGE_METHOD_NAME, object={
+    logger.start(object={
         "check_time": check_time.__str__(), "time_range": time_range.__str__()})
     if not is_valid_time_range(time_range) or not isinstance(check_time, time):
-        logger.end(IS_TIME_IN_TIME_RANGE_METHOD_NAME, object={
+        logger.end(object={
             "is_time_in_time_range_result": False})
         return False
     start_time, end_time = time_range
-    logger.end(IS_TIME_IN_TIME_RANGE_METHOD_NAME, object={
+    logger.end(object={
         "is_time_in_time_range_result": start_time <= check_time <= end_time})
     return start_time <= check_time <= end_time
 
 
 def is_date_in_date_range(check_date: date, date_range: tuple) -> bool:
     """
     Check if the given date is within the specified date range.
@@ -203,24 +194,23 @@
     Parameters:
         check_date (str): The date to check in 'YYYY-MM-DD' format.
         date_range (tuple): A tuple containing start and end dates in 'YYYY-MM-DD' format.
 
     Returns:
         bool: True if the check_date is within the date range, False otherwise.
     """
-    IS_DATE_IN_DATE_RANGE_METHOD_NAME = "is_date_in_date_range"
-    logger.start(IS_DATE_IN_DATE_RANGE_METHOD_NAME, object={
+    logger.start(object={
         "check_date": check_date.__str__(), "date_range": date_range.__str__()})
     if not is_valid_date_range(date_range) or not isinstance(check_date, date):
-        logger.end(IS_DATE_IN_DATE_RANGE_METHOD_NAME, object={
+        logger.end(object={
             "is_date_in_date_range_result": False})
         return False
 
     start_date, end_date = date_range
-    logger.end(IS_DATE_IN_DATE_RANGE_METHOD_NAME, object={
+    logger.end(object={
         "is_date_in_date_range_result": start_date <= check_date <= end_date})
     return start_date <= check_date <= end_date
 
 
 def is_datetime_in_datetime_range(check_datetime: datetime, datetime_range: tuple) -> bool:
     """
     Check if the given datetime is within the specified datetime range.
@@ -228,90 +218,44 @@
     Parameters:
         check_datetime (str): The datetime to check in 'YYYY-MM-DD HH:MM:SS' format.
         datetime_range (tuple): A tuple containing start and end datetimes in 'YYYY-MM-DD HH:MM:SS' format.
 
     Returns:
         bool: True if the check_datetime is within the datetime range, False otherwise.
     """
-    IS_DATETIME_IN_DATETIME_RANGE_METHOD_NAME = "is_datetime_in_datetime_range"
-    logger.start(IS_DATETIME_IN_DATETIME_RANGE_METHOD_NAME)
+    logger.start()
     if not is_valid_datetime_range(datetime_range) or not isinstance(check_datetime, datetime):
-        logger.end(IS_DATETIME_IN_DATETIME_RANGE_METHOD_NAME, object={
+        logger.end(object={
             "is_valid_datetime_range": False})
         return False
 
     start_datetime, end_datetime = datetime_range
     is_datetime_in_datetime_range_result = start_datetime <= check_datetime <= end_datetime
-    logger.end(IS_DATETIME_IN_DATETIME_RANGE_METHOD_NAME, object={
+    logger.end(object={
         "is_datetime_in_datetime_range_result": is_datetime_in_datetime_range_result})
     return is_datetime_in_datetime_range_result
 
 
-# TODO Align those methods with typescript-sdk https://github.com/circles-zone/typescript-sdk-remote-typescript-package/blob/dev/typescript-sdk/src/utils/index.ts  # noqa501
-# TODO Take those three functions to a separate file http_response.py
-# TODO Shall we create also createInternalServerErrorHttpResponse(), createOkHttpResponse() like we have in TypeScript?
-
-# Former name was create_http_headers()
-def create_authorization_http_headers(user_jwt: str) -> dict:
-    return {
-        'Content-Type': 'application/json',
-        'Authorization': f'Bearer {user_jwt}',
-    }
-
-
-def get_user_jwt_from_event(event: dict) -> str:
-    auth_header = event.get('headers', {}).get('authorization')
-    if auth_header is None:
-        auth_header = event.get('headers', {}).get('Authorization')
-    return auth_header.split('Bearer ')[1]
-
-
-def create_return_http_headers() -> dict:
-    return {
-        "Content-Type": "application/json",
-        "Access-Control-Allow-Origin": "*",
-    }
-
-def create_error_http_response(exception: Exception) -> dict:
-    return {
-            "statusCode": status.BAD_GATEWAY,
-            "headers": create_return_http_headers(),
-            "body": create_http_body({"error": str(exception)})
-        }
-
-def create_ok_http_response(body: dict) -> dict:
-    return {
-        "statusCode": status.OK,
-        "headers": create_return_http_headers(),
-        "body": create_http_body(body)
-    }
-
-
-# https://google.github.io/styleguide/jsoncstyleguide.xml?showone=Property_Name_Format#Property_Name_Format
-def create_http_body(body: dict) -> str:
-    # TODO console.warning() if the body is not a valid camelCase JSON
-    # https://stackoverflow.com/questions/17156078/converting-identifier-naming-between-camelcase-and-underscores-during-json-seria
-    return json.dumps(body)
-
-
 def get_brand_name() -> str:
     return our_get_env("BRAND_NAME")
 
 
 def get_environment_name() -> str:
     environment_name = our_get_env("ENVIRONMENT_NAME")
     EnvironmentName(environment_name)  # if invalid, raises ValueError: x is not a valid EnvironmentName
     return environment_name
 
 
 def our_get_env(key: str, default: str = None, raise_if_not_found: bool = True) -> str:
-    result = os.getenv(key, default)
-    if raise_if_not_found and result is None:
+    logger.start(object={"key": key, "default": default, "raise_if_not_found": raise_if_not_found})
+    env_var = os.getenv(key, default)
+    if raise_if_not_found and env_var is None:
         raise Exception(f"Environment variable {key} not found")
-    return result
+    logger.end(object={"env_var": env_var})
+    return env_var
 
 
 def get_sql_hostname() -> str:
     return our_get_env("RDS_HOSTNAME")
 
 
 def get_sql_username() -> str:
```

### Comparing `python_sdk_remote-0.0.91/python_sdk_remote/src/validate_environment.py` & `python_sdk_remote-0.0.92/python_sdk_remote/src/validate_environment.py`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.91/python_sdk_remote.egg-info/PKG-INFO` & `python_sdk_remote-0.0.92/python_sdk_remote.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sdk-remote
-Version: 0.0.91
+Version: 0.0.92
 Summary: PyPI Package for Circles Python SDK Local Python
 Home-page: https://github.com/circles-zone/python-sdk-remote-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `python_sdk_remote-0.0.91/python_sdk_remote.egg-info/SOURCES.txt` & `python_sdk_remote-0.0.92/python_sdk_remote.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 python_sdk_remote.egg-info/PKG-INFO
 python_sdk_remote.egg-info/SOURCES.txt
 python_sdk_remote.egg-info/dependency_links.txt
 python_sdk_remote.egg-info/requires.txt
 python_sdk_remote.egg-info/top_level.txt
 python_sdk_remote/src/__init__.py
 python_sdk_remote/src/constants.py
+python_sdk_remote/src/http_response.py
 python_sdk_remote/src/item.py
 python_sdk_remote/src/mini_logger.py
 python_sdk_remote/src/our_object.py
 python_sdk_remote/src/unified_json.py
 python_sdk_remote/src/utilities.py
 python_sdk_remote/src/valid_json_versions.py
 python_sdk_remote/src/validate_environment.py
```

### Comparing `python_sdk_remote-0.0.91/setup.py` & `python_sdk_remote-0.0.92/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 PACKAGE_NAME = "python-sdk-remote"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.91',  # https://pypi.org/project/python-sdk-remote/
+    version='0.0.92',  # https://pypi.org/project/python-sdk-remote/
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles Python SDK Local Python",
     long_description="This is a package for sharing common functions used in different repositories",
     long_description_content_type="text/markdown",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
```

