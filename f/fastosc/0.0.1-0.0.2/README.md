# Comparing `tmp/fastosc-0.0.1.tar.gz` & `tmp/fastosc-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/sahlen/repositories/oslo1989/fastosc/dist/.tmp-2yucp96h/fastosc-0.0.1.tar", last modified: Sun May  5 13:24:40 2024, max compression
+gzip compressed data, was "/Users/sahlen/repositories/oslo1989/fastosc/dist/.tmp-kd_1fa88/fastosc-0.0.2.tar", last modified: Sun May  5 14:24:01 2024, max compression
```

## Comparing `fastosc-0.0.1.tar` & `fastosc-0.0.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 13:24:40.000000 fastosc-0.0.1/
--rw-r--r--   0 sahlen     (501) staff       (20)      370 2024-05-05 13:24:40.000000 fastosc-0.0.1/PKG-INFO
--rw-r--r--   0 sahlen     (501) staff       (20)      280 2024-05-05 12:26:24.000000 fastosc-0.0.1/README.md
--rw-r--r--   0 sahlen     (501) staff       (20)      475 2024-05-05 12:22:42.000000 fastosc-0.0.1/pyproject.toml
--rw-r--r--   0 sahlen     (501) staff       (20)       38 2024-05-05 13:24:40.000000 fastosc-0.0.1/setup.cfg
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 13:24:40.000000 fastosc-0.0.1/src/
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 13:24:40.000000 fastosc-0.0.1/src/fastosc/
--rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-01-13 16:36:43.000000 fastosc-0.0.1/src/fastosc/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 13:24:40.000000 fastosc-0.0.1/src/fastosc/dispatcher/
--rw-r--r--   0 sahlen     (501) staff       (20)     5937 2024-01-20 18:59:40.000000 fastosc-0.0.1/src/fastosc/dispatcher/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)      250 2024-01-20 18:33:22.000000 fastosc-0.0.1/src/fastosc/dispatcher/handler.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 13:24:40.000000 fastosc-0.0.1/src/fastosc/docs/
--rw-r--r--   0 sahlen     (501) staff       (20)      313 2024-01-20 18:35:02.000000 fastosc-0.0.1/src/fastosc/docs/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 13:24:40.000000 fastosc-0.0.1/src/fastosc/message/
--rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-01-13 21:23:05.000000 fastosc-0.0.1/src/fastosc/message/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9145 2024-01-20 16:18:06.000000 fastosc-0.0.1/src/fastosc/message/arg_value.py
--rw-r--r--   0 sahlen     (501) staff       (20)      457 2024-01-20 16:19:12.000000 fastosc-0.0.1/src/fastosc/message/convert.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3767 2024-01-19 08:45:29.000000 fastosc-0.0.1/src/fastosc/message/osc_bundle.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1960 2024-01-19 08:45:18.000000 fastosc-0.0.1/src/fastosc/message/osc_bundle_builder.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4587 2024-01-19 08:44:11.000000 fastosc-0.0.1/src/fastosc/message/osc_message.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7152 2024-01-20 19:54:40.000000 fastosc-0.0.1/src/fastosc/message/osc_message_builder.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 13:24:40.000000 fastosc-0.0.1/src/fastosc/message/parsing/
--rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-01-08 21:16:09.000000 fastosc-0.0.1/src/fastosc/message/parsing/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1845 2024-01-13 21:33:36.000000 fastosc-0.0.1/src/fastosc/message/parsing/ntp.py
--rw-r--r--   0 sahlen     (501) staff       (20)    15342 2024-01-19 07:40:48.000000 fastosc-0.0.1/src/fastosc/message/parsing/osc_types.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 13:24:40.000000 fastosc-0.0.1/src/fastosc/router/
--rw-r--r--   0 sahlen     (501) staff       (20)    11175 2024-01-20 19:00:31.000000 fastosc-0.0.1/src/fastosc/router/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 13:24:40.000000 fastosc-0.0.1/src/fastosc/server/
--rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-01-19 10:51:55.000000 fastosc-0.0.1/src/fastosc/server/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)      442 2024-01-20 10:37:22.000000 fastosc-0.0.1/src/fastosc/server/dispatcher_server.py
--rw-r--r--   0 sahlen     (501) staff       (20)      960 2024-01-20 10:37:22.000000 fastosc-0.0.1/src/fastosc/server/server_base.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 13:24:40.000000 fastosc-0.0.1/src/fastosc/server/udp/
--rw-r--r--   0 sahlen     (501) staff       (20)     2645 2024-01-19 13:17:58.000000 fastosc-0.0.1/src/fastosc/server/udp/udp_pull_server.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1447 2024-01-19 14:04:48.000000 fastosc-0.0.1/src/fastosc/server/udp/udp_server_base.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 13:24:40.000000 fastosc-0.0.1/src/fastosc.egg-info/
--rw-r--r--   0 sahlen     (501) staff       (20)      370 2024-05-05 13:24:40.000000 fastosc-0.0.1/src/fastosc.egg-info/PKG-INFO
--rw-r--r--   0 sahlen     (501) staff       (20)      872 2024-05-05 13:24:40.000000 fastosc-0.0.1/src/fastosc.egg-info/SOURCES.txt
--rw-r--r--   0 sahlen     (501) staff       (20)        1 2024-05-05 13:24:40.000000 fastosc-0.0.1/src/fastosc.egg-info/dependency_links.txt
--rw-r--r--   0 sahlen     (501) staff       (20)        8 2024-05-05 13:24:40.000000 fastosc-0.0.1/src/fastosc.egg-info/top_level.txt
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 fastosc-0.0.2/
+-rw-r--r--   0 sahlen     (501) staff       (20)      611 2024-05-05 14:24:01.000000 fastosc-0.0.2/PKG-INFO
+-rw-r--r--   0 sahlen     (501) staff       (20)      280 2024-05-05 12:26:24.000000 fastosc-0.0.2/README.md
+-rw-r--r--   0 sahlen     (501) staff       (20)      930 2024-05-05 14:14:28.000000 fastosc-0.0.2/pyproject.toml
+-rw-r--r--   0 sahlen     (501) staff       (20)       38 2024-05-05 14:24:01.000000 fastosc-0.0.2/setup.cfg
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 fastosc-0.0.2/src/
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 fastosc-0.0.2/src/fastosc/
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-01-13 16:36:43.000000 fastosc-0.0.2/src/fastosc/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 fastosc-0.0.2/src/fastosc/dispatcher/
+-rw-r--r--   0 sahlen     (501) staff       (20)     5937 2024-01-20 18:59:40.000000 fastosc-0.0.2/src/fastosc/dispatcher/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      250 2024-01-20 18:33:22.000000 fastosc-0.0.2/src/fastosc/dispatcher/handler.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 fastosc-0.0.2/src/fastosc/docs/
+-rw-r--r--   0 sahlen     (501) staff       (20)      313 2024-01-20 18:35:02.000000 fastosc-0.0.2/src/fastosc/docs/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 fastosc-0.0.2/src/fastosc/message/
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-01-13 21:23:05.000000 fastosc-0.0.2/src/fastosc/message/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9145 2024-01-20 16:18:06.000000 fastosc-0.0.2/src/fastosc/message/arg_value.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      457 2024-01-20 16:19:12.000000 fastosc-0.0.2/src/fastosc/message/convert.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3767 2024-01-19 08:45:29.000000 fastosc-0.0.2/src/fastosc/message/osc_bundle.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1960 2024-01-19 08:45:18.000000 fastosc-0.0.2/src/fastosc/message/osc_bundle_builder.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4587 2024-01-19 08:44:11.000000 fastosc-0.0.2/src/fastosc/message/osc_message.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     7152 2024-01-20 19:54:40.000000 fastosc-0.0.2/src/fastosc/message/osc_message_builder.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 fastosc-0.0.2/src/fastosc/message/parsing/
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-01-08 21:16:09.000000 fastosc-0.0.2/src/fastosc/message/parsing/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1845 2024-01-13 21:33:36.000000 fastosc-0.0.2/src/fastosc/message/parsing/ntp.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    15342 2024-01-19 07:40:48.000000 fastosc-0.0.2/src/fastosc/message/parsing/osc_types.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 fastosc-0.0.2/src/fastosc/router/
+-rw-r--r--   0 sahlen     (501) staff       (20)    11175 2024-01-20 19:00:31.000000 fastosc-0.0.2/src/fastosc/router/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 fastosc-0.0.2/src/fastosc/server/
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-01-19 10:51:55.000000 fastosc-0.0.2/src/fastosc/server/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      442 2024-01-20 10:37:22.000000 fastosc-0.0.2/src/fastosc/server/dispatcher_server.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      960 2024-01-20 10:37:22.000000 fastosc-0.0.2/src/fastosc/server/server_base.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 fastosc-0.0.2/src/fastosc/server/udp/
+-rw-r--r--   0 sahlen     (501) staff       (20)     2645 2024-01-19 13:17:58.000000 fastosc-0.0.2/src/fastosc/server/udp/udp_pull_server.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1447 2024-01-19 14:04:48.000000 fastosc-0.0.2/src/fastosc/server/udp/udp_server_base.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 fastosc-0.0.2/src/fastosc.egg-info/
+-rw-r--r--   0 sahlen     (501) staff       (20)      611 2024-05-05 14:24:01.000000 fastosc-0.0.2/src/fastosc.egg-info/PKG-INFO
+-rw-r--r--   0 sahlen     (501) staff       (20)      872 2024-05-05 14:24:01.000000 fastosc-0.0.2/src/fastosc.egg-info/SOURCES.txt
+-rw-r--r--   0 sahlen     (501) staff       (20)        1 2024-05-05 14:24:01.000000 fastosc-0.0.2/src/fastosc.egg-info/dependency_links.txt
+-rw-r--r--   0 sahlen     (501) staff       (20)        8 2024-05-05 14:24:01.000000 fastosc-0.0.2/src/fastosc.egg-info/top_level.txt
```

### Comparing `fastosc-0.0.1/src/fastosc/dispatcher/__init__.py` & `fastosc-0.0.2/src/fastosc/dispatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `fastosc-0.0.1/src/fastosc/message/arg_value.py` & `fastosc-0.0.2/src/fastosc/message/arg_value.py`

 * *Files identical despite different names*

### Comparing `fastosc-0.0.1/src/fastosc/message/osc_bundle.py` & `fastosc-0.0.2/src/fastosc/message/osc_bundle.py`

 * *Files identical despite different names*

### Comparing `fastosc-0.0.1/src/fastosc/message/osc_bundle_builder.py` & `fastosc-0.0.2/src/fastosc/message/osc_bundle_builder.py`

 * *Files identical despite different names*

### Comparing `fastosc-0.0.1/src/fastosc/message/osc_message.py` & `fastosc-0.0.2/src/fastosc/message/osc_message.py`

 * *Files identical despite different names*

### Comparing `fastosc-0.0.1/src/fastosc/message/osc_message_builder.py` & `fastosc-0.0.2/src/fastosc/message/osc_message_builder.py`

 * *Files identical despite different names*

### Comparing `fastosc-0.0.1/src/fastosc/message/parsing/ntp.py` & `fastosc-0.0.2/src/fastosc/message/parsing/ntp.py`

 * *Files identical despite different names*

### Comparing `fastosc-0.0.1/src/fastosc/message/parsing/osc_types.py` & `fastosc-0.0.2/src/fastosc/message/parsing/osc_types.py`

 * *Files identical despite different names*

### Comparing `fastosc-0.0.1/src/fastosc/router/__init__.py` & `fastosc-0.0.2/src/fastosc/router/__init__.py`

 * *Files identical despite different names*

### Comparing `fastosc-0.0.1/src/fastosc/server/server_base.py` & `fastosc-0.0.2/src/fastosc/server/server_base.py`

 * *Files identical despite different names*

### Comparing `fastosc-0.0.1/src/fastosc/server/udp/udp_pull_server.py` & `fastosc-0.0.2/src/fastosc/server/udp/udp_pull_server.py`

 * *Files identical despite different names*

### Comparing `fastosc-0.0.1/src/fastosc/server/udp/udp_server_base.py` & `fastosc-0.0.2/src/fastosc/server/udp/udp_server_base.py`

 * *Files identical despite different names*

### Comparing `fastosc-0.0.1/src/fastosc.egg-info/SOURCES.txt` & `fastosc-0.0.2/src/fastosc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

