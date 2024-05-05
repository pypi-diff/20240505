# Comparing `tmp/a5-0.0.3.tar.gz` & `tmp/a5-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "a5-0.0.3.tar", last modified: Sun May  5 19:05:21 2024, max compression
+gzip compressed data, was "a5-0.0.4.tar", last modified: Sun May  5 21:07:59 2024, max compression
```

## Comparing `a5-0.0.3.tar` & `a5-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,30 @@
-drwxrwxr-x   0 aapeli    (1000) aapeli    (1000)        0 2024-05-05 19:05:21.212215 a5-0.0.3/
--rw-r--r--   0 aapeli    (1000) aapeli    (1000)      217 2024-05-05 19:05:21.212215 a5-0.0.3/PKG-INFO
-drwxrwxr-x   0 aapeli    (1000) aapeli    (1000)        0 2024-05-05 19:05:21.208215 a5-0.0.3/a5/
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)        0 2024-05-05 18:49:21.000000 a5-0.0.3/a5/__init__.py
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)        6 2024-05-05 19:05:18.000000 a5-0.0.3/a5/version
-drwxrwxr-x   0 aapeli    (1000) aapeli    (1000)        0 2024-05-05 19:05:21.208215 a5-0.0.3/a5/web/
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)        0 2024-05-05 18:49:32.000000 a5-0.0.3/a5/web/__init__.py
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)     1309 2024-05-05 19:01:16.000000 a5-0.0.3/a5/web/basic_web_server.py
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)     1399 2024-05-05 18:50:15.000000 a5-0.0.3/a5/web/cookies.py
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)     1752 2024-05-05 18:49:32.000000 a5-0.0.3/a5/web/http_status_codes.py
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)      977 2024-05-05 18:51:04.000000 a5-0.0.3/a5/web/static_file_server.py
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)      937 2024-05-05 18:49:32.000000 a5-0.0.3/a5/web/tiny_web_server.py
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)     3487 2024-05-05 19:01:00.000000 a5-0.0.3/a5/web/tls.py
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)      689 2024-05-05 18:49:32.000000 a5-0.0.3/a5/web/wsgi_server.py
-drwxrwxr-x   0 aapeli    (1000) aapeli    (1000)        0 2024-05-05 19:05:21.212215 a5-0.0.3/a5.egg-info/
--rw-r--r--   0 aapeli    (1000) aapeli    (1000)      217 2024-05-05 19:05:21.000000 a5-0.0.3/a5.egg-info/PKG-INFO
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)      381 2024-05-05 19:05:21.000000 a5-0.0.3/a5.egg-info/SOURCES.txt
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)        1 2024-05-05 19:05:21.000000 a5-0.0.3/a5.egg-info/dependency_links.txt
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)       25 2024-05-05 19:05:21.000000 a5-0.0.3/a5.egg-info/requires.txt
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)        3 2024-05-05 19:05:21.000000 a5-0.0.3/a5.egg-info/top_level.txt
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)      330 2024-05-05 18:58:17.000000 a5-0.0.3/pyproject.toml
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)       38 2024-05-05 19:05:21.212215 a5-0.0.3/setup.cfg
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)      487 2024-05-05 19:03:56.000000 a5-0.0.3/setup.py
+drwxrwxr-x   0 aapeli    (1000) aapeli    (1000)        0 2024-05-05 21:07:58.997839 a5-0.0.4/
+-rw-r--r--   0 aapeli    (1000) aapeli    (1000)      239 2024-05-05 21:07:58.997839 a5-0.0.4/PKG-INFO
+drwxrwxr-x   0 aapeli    (1000) aapeli    (1000)        0 2024-05-05 21:07:58.997839 a5-0.0.4/a5/
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)        0 2024-05-05 18:49:21.000000 a5-0.0.4/a5/__init__.py
+drwxrwxr-x   0 aapeli    (1000) aapeli    (1000)        0 2024-05-05 21:07:58.997839 a5-0.0.4/a5/grpc/
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)        0 2024-05-05 19:16:57.000000 a5-0.0.4/a5/grpc/__init__.py
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)        0 2024-05-05 19:21:13.000000 a5-0.0.4/a5/grpc/reflection_utils.py
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)     3300 2024-05-05 19:20:13.000000 a5-0.0.4/a5/grpc/rpc_utils.py
+drwxrwxr-x   0 aapeli    (1000) aapeli    (1000)        0 2024-05-05 21:07:58.997839 a5-0.0.4/a5/security/
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)        0 2024-05-05 21:06:01.000000 a5-0.0.4/a5/security/__init__.py
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)     3130 2024-05-05 21:06:28.000000 a5-0.0.4/a5/security/crypto.py
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)        6 2024-05-05 21:07:14.000000 a5-0.0.4/a5/version
+drwxrwxr-x   0 aapeli    (1000) aapeli    (1000)        0 2024-05-05 21:07:58.997839 a5-0.0.4/a5/web/
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)        0 2024-05-05 18:49:32.000000 a5-0.0.4/a5/web/__init__.py
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)     1309 2024-05-05 19:01:16.000000 a5-0.0.4/a5/web/basic_web_server.py
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)     1399 2024-05-05 18:50:15.000000 a5-0.0.4/a5/web/cookies.py
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)     1752 2024-05-05 18:49:32.000000 a5-0.0.4/a5/web/http_status_codes.py
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)      977 2024-05-05 18:51:04.000000 a5-0.0.4/a5/web/static_file_server.py
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)      937 2024-05-05 18:49:32.000000 a5-0.0.4/a5/web/tiny_web_server.py
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)     3487 2024-05-05 19:01:00.000000 a5-0.0.4/a5/web/tls.py
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)      689 2024-05-05 18:49:32.000000 a5-0.0.4/a5/web/wsgi_server.py
+drwxrwxr-x   0 aapeli    (1000) aapeli    (1000)        0 2024-05-05 21:07:58.997839 a5-0.0.4/a5.egg-info/
+-rw-r--r--   0 aapeli    (1000) aapeli    (1000)      239 2024-05-05 21:07:58.000000 a5-0.0.4/a5.egg-info/PKG-INFO
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)      506 2024-05-05 21:07:58.000000 a5-0.0.4/a5.egg-info/SOURCES.txt
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)        1 2024-05-05 21:07:58.000000 a5-0.0.4/a5.egg-info/dependency_links.txt
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)       32 2024-05-05 21:07:58.000000 a5-0.0.4/a5.egg-info/requires.txt
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)        3 2024-05-05 21:07:58.000000 a5-0.0.4/a5.egg-info/top_level.txt
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)      330 2024-05-05 18:58:17.000000 a5-0.0.4/pyproject.toml
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)       38 2024-05-05 21:07:58.997839 a5-0.0.4/setup.cfg
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)      505 2024-05-05 21:07:05.000000 a5-0.0.4/setup.py
```

### Comparing `a5-0.0.3/a5/web/basic_web_server.py` & `a5-0.0.4/a5/web/basic_web_server.py`

 * *Files identical despite different names*

### Comparing `a5-0.0.3/a5/web/cookies.py` & `a5-0.0.4/a5/web/cookies.py`

 * *Files identical despite different names*

### Comparing `a5-0.0.3/a5/web/http_status_codes.py` & `a5-0.0.4/a5/web/http_status_codes.py`

 * *Files identical despite different names*

### Comparing `a5-0.0.3/a5/web/static_file_server.py` & `a5-0.0.4/a5/web/static_file_server.py`

 * *Files identical despite different names*

### Comparing `a5-0.0.3/a5/web/tiny_web_server.py` & `a5-0.0.4/a5/web/tiny_web_server.py`

 * *Files identical despite different names*

### Comparing `a5-0.0.3/a5/web/tls.py` & `a5-0.0.4/a5/web/tls.py`

 * *Files identical despite different names*

### Comparing `a5-0.0.3/a5/web/wsgi_server.py` & `a5-0.0.4/a5/web/wsgi_server.py`

 * *Files identical despite different names*

