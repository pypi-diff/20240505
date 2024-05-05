# Comparing `tmp/search_content_gcs-0.1.0.tar.gz` & `tmp/search_content_gcs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "search_content_gcs-0.1.0.tar", max compression
+gzip compressed data, was "search_content_gcs-0.1.1.tar", max compression
```

## Comparing `search_content_gcs-0.1.0.tar` & `search_content_gcs-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      289 2024-05-05 09:54:28.361808 search_content_gcs-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      447 2024-05-05 10:38:22.895763 search_content_gcs-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-05 09:54:28.356084 search_content_gcs-0.1.0/search_content_gcs/__init__.py
--rw-r--r--   0        0        0     1118 2024-05-05 10:27:26.728402 search_content_gcs-0.1.0/search_content_gcs/api.py
--rw-r--r--   0        0        0     5857 2024-05-05 10:20:20.139344 search_content_gcs-0.1.0/search_content_gcs/client.py
--rw-r--r--   0        0        0      344 2024-05-05 10:07:48.367159 search_content_gcs-0.1.0/search_content_gcs/error.py
--rw-r--r--   0        0        0     2138 2024-05-05 10:06:31.813634 search_content_gcs-0.1.0/search_content_gcs/exception.py
--rw-r--r--   0        0        0      423 2024-05-05 10:11:46.692863 search_content_gcs-0.1.0/search_content_gcs/models/__init__.py
--rw-r--r--   0        0        0      499 2024-05-05 10:27:16.052416 search_content_gcs-0.1.0/search_content_gcs/models/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2553 2024-05-05 10:27:16.055414 search_content_gcs-0.1.0/search_content_gcs/models/__pycache__/google_custom_search.cpython-310.pyc
--rw-r--r--   0        0        0      724 2024-05-05 10:27:16.219416 search_content_gcs-0.1.0/search_content_gcs/models/__pycache__/simple_youtube_data.cpython-310.pyc
--rw-r--r--   0        0        0        0 2024-05-05 10:01:49.443962 search_content_gcs-0.1.0/search_content_gcs/models/gcs_api_key.py
--rw-r--r--   0        0        0     1520 2024-05-05 13:51:46.531535 search_content_gcs-0.1.0/search_content_gcs/models/google_custom_search.py
--rw-r--r--   0        0        0      283 2024-05-05 09:49:21.798994 search_content_gcs-0.1.0/search_content_gcs/models/simple_youtube_data.py
--rw-r--r--   0        0        0     1103 2024-05-05 10:31:38.298623 search_content_gcs-0.1.0/search_content_gcs/parser/__init__.py
--rw-r--r--   0        0        0     1083 2024-05-05 10:27:16.050414 search_content_gcs-0.1.0/search_content_gcs/parser/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        0 2024-05-05 07:56:01.075010 search_content_gcs-0.1.0/search_content_gcs/utils/__init__.py
--rw-r--r--   0        0        0      229 2024-05-05 10:27:16.223415 search_content_gcs-0.1.0/search_content_gcs/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      775 2024-05-05 10:27:16.227415 search_content_gcs-0.1.0/search_content_gcs/utils/__pycache__/youtube_url.cpython-310.pyc
--rw-r--r--   0        0        0      667 2024-05-05 10:32:24.731312 search_content_gcs-0.1.0/search_content_gcs/utils/youtube_url.py
--rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 search_content_gcs-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      289 2024-05-05 13:52:41.001708 search_content_gcs-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      447 2024-05-05 10:38:22.895763 search_content_gcs-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-05 09:54:28.356084 search_content_gcs-0.1.1/search_content_gcs/__init__.py
+-rw-r--r--   0        0        0     1118 2024-05-05 10:27:26.728402 search_content_gcs-0.1.1/search_content_gcs/api.py
+-rw-r--r--   0        0        0     5857 2024-05-05 10:20:20.139344 search_content_gcs-0.1.1/search_content_gcs/client.py
+-rw-r--r--   0        0        0      344 2024-05-05 10:07:48.367159 search_content_gcs-0.1.1/search_content_gcs/error.py
+-rw-r--r--   0        0        0     2138 2024-05-05 10:06:31.813634 search_content_gcs-0.1.1/search_content_gcs/exception.py
+-rw-r--r--   0        0        0      423 2024-05-05 10:11:46.692863 search_content_gcs-0.1.1/search_content_gcs/models/__init__.py
+-rw-r--r--   0        0        0      499 2024-05-05 10:27:16.052416 search_content_gcs-0.1.1/search_content_gcs/models/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2553 2024-05-05 10:27:16.055414 search_content_gcs-0.1.1/search_content_gcs/models/__pycache__/google_custom_search.cpython-310.pyc
+-rw-r--r--   0        0        0      724 2024-05-05 10:27:16.219416 search_content_gcs-0.1.1/search_content_gcs/models/__pycache__/simple_youtube_data.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2024-05-05 10:01:49.443962 search_content_gcs-0.1.1/search_content_gcs/models/gcs_api_key.py
+-rw-r--r--   0        0        0     1520 2024-05-05 13:51:46.531535 search_content_gcs-0.1.1/search_content_gcs/models/google_custom_search.py
+-rw-r--r--   0        0        0      283 2024-05-05 09:49:21.798994 search_content_gcs-0.1.1/search_content_gcs/models/simple_youtube_data.py
+-rw-r--r--   0        0        0     1103 2024-05-05 10:31:38.298623 search_content_gcs-0.1.1/search_content_gcs/parser/__init__.py
+-rw-r--r--   0        0        0     1083 2024-05-05 10:27:16.050414 search_content_gcs-0.1.1/search_content_gcs/parser/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2024-05-05 07:56:01.075010 search_content_gcs-0.1.1/search_content_gcs/utils/__init__.py
+-rw-r--r--   0        0        0      229 2024-05-05 10:27:16.223415 search_content_gcs-0.1.1/search_content_gcs/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      775 2024-05-05 10:27:16.227415 search_content_gcs-0.1.1/search_content_gcs/utils/__pycache__/youtube_url.cpython-310.pyc
+-rw-r--r--   0        0        0      667 2024-05-05 10:32:24.731312 search_content_gcs-0.1.1/search_content_gcs/utils/youtube_url.py
+-rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 search_content_gcs-0.1.1/PKG-INFO
```

### Comparing `search_content_gcs-0.1.0/search_content_gcs/api.py` & `search_content_gcs-0.1.1/search_content_gcs/api.py`

 * *Files identical despite different names*

### Comparing `search_content_gcs-0.1.0/search_content_gcs/client.py` & `search_content_gcs-0.1.1/search_content_gcs/client.py`

 * *Files identical despite different names*

### Comparing `search_content_gcs-0.1.0/search_content_gcs/exception.py` & `search_content_gcs-0.1.1/search_content_gcs/exception.py`

 * *Files identical despite different names*

### Comparing `search_content_gcs-0.1.0/search_content_gcs/models/__pycache__/google_custom_search.cpython-310.pyc` & `search_content_gcs-0.1.1/search_content_gcs/models/__pycache__/google_custom_search.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `search_content_gcs-0.1.0/search_content_gcs/models/__pycache__/simple_youtube_data.cpython-310.pyc` & `search_content_gcs-0.1.1/search_content_gcs/models/__pycache__/simple_youtube_data.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `search_content_gcs-0.1.0/search_content_gcs/models/google_custom_search.py` & `search_content_gcs-0.1.1/search_content_gcs/models/google_custom_search.py`

 * *Files identical despite different names*

### Comparing `search_content_gcs-0.1.0/search_content_gcs/parser/__init__.py` & `search_content_gcs-0.1.1/search_content_gcs/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `search_content_gcs-0.1.0/search_content_gcs/parser/__pycache__/__init__.cpython-310.pyc` & `search_content_gcs-0.1.1/search_content_gcs/parser/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `search_content_gcs-0.1.0/search_content_gcs/utils/__pycache__/youtube_url.cpython-310.pyc` & `search_content_gcs-0.1.1/search_content_gcs/utils/__pycache__/youtube_url.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `search_content_gcs-0.1.0/search_content_gcs/utils/youtube_url.py` & `search_content_gcs-0.1.1/search_content_gcs/utils/youtube_url.py`

 * *Files identical despite different names*

### Comparing `search_content_gcs-0.1.0/PKG-INFO` & `search_content_gcs-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: search-content-gcs
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: heeya8876
 Author-email: heeya8876@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

