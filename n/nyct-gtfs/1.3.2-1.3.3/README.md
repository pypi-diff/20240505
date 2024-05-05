# Comparing `tmp/nyct-gtfs-1.3.2.tar.gz` & `tmp/nyct_gtfs-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nyct-gtfs-1.3.2.tar", last modified: Sat Dec  2 04:08:42 2023, max compression
+gzip compressed data, was "nyct_gtfs-1.3.3.tar", last modified: Sun May  5 00:55:38 2024, max compression
```

## Comparing `nyct-gtfs-1.3.2.tar` & `nyct_gtfs-1.3.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 andrewjd   (504) staff       (20)        0 2023-12-02 04:08:42.026687 nyct-gtfs-1.3.2/
--rw-r--r--   0 andrewjd   (504) staff       (20)     1073 2023-11-24 02:22:03.000000 nyct-gtfs-1.3.2/LICENSE.txt
--rw-r--r--   0 andrewjd   (504) staff       (20)    13213 2023-12-02 04:08:42.026242 nyct-gtfs-1.3.2/PKG-INFO
--rw-r--r--   0 andrewjd   (504) staff       (20)    12682 2023-11-24 02:22:03.000000 nyct-gtfs-1.3.2/README.md
-drwxr-xr-x   0 andrewjd   (504) staff       (20)        0 2023-12-02 04:08:42.021494 nyct-gtfs-1.3.2/nyct_gtfs/
--rw-r--r--   0 andrewjd   (504) staff       (20)      182 2023-11-24 02:22:03.000000 nyct-gtfs-1.3.2/nyct_gtfs/__init__.py
-drwxr-xr-x   0 andrewjd   (504) staff       (20)        0 2023-12-02 04:08:42.022984 nyct-gtfs-1.3.2/nyct_gtfs/compiled_gtfs/
--rw-r--r--   0 andrewjd   (504) staff       (20)        0 2023-11-24 02:22:03.000000 nyct-gtfs-1.3.2/nyct_gtfs/compiled_gtfs/__init__.py
--rw-r--r--   0 andrewjd   (504) staff       (20)    15436 2023-11-24 02:22:03.000000 nyct-gtfs-1.3.2/nyct_gtfs/compiled_gtfs/gtfs_realtime_pb2.py
--rw-r--r--   0 andrewjd   (504) staff       (20)     4593 2023-11-24 02:22:03.000000 nyct-gtfs-1.3.2/nyct_gtfs/compiled_gtfs/nyct_subway_pb2.py
--rw-r--r--   0 andrewjd   (504) staff       (20)     4914 2023-11-24 02:22:03.000000 nyct-gtfs-1.3.2/nyct_gtfs/cpp_parser_wrapper.py
--rw-r--r--   0 andrewjd   (504) staff       (20)    14313 2023-11-24 02:22:03.000000 nyct-gtfs-1.3.2/nyct_gtfs/feed.py
-drwxr-xr-x   0 andrewjd   (504) staff       (20)        0 2023-12-02 04:08:42.023673 nyct-gtfs-1.3.2/nyct_gtfs/gtfs_static/
--rw-r--r--   0 andrewjd   (504) staff       (20)    71961 2023-11-24 02:22:03.000000 nyct-gtfs-1.3.2/nyct_gtfs/gtfs_static/stops.txt
--rw-r--r--   0 andrewjd   (504) staff       (20)  1883488 2023-11-24 02:22:03.000000 nyct-gtfs-1.3.2/nyct_gtfs/gtfs_static/trips.txt
--rw-r--r--   0 andrewjd   (504) staff       (20)     3324 2023-11-24 02:22:03.000000 nyct-gtfs-1.3.2/nyct_gtfs/gtfs_static_types.py
--rw-r--r--   0 andrewjd   (504) staff       (20)     8615 2023-11-24 02:22:03.000000 nyct-gtfs-1.3.2/nyct_gtfs/stop_time_update.py
--rw-r--r--   0 andrewjd   (504) staff       (20)    17293 2023-12-02 04:08:15.000000 nyct-gtfs-1.3.2/nyct_gtfs/trip.py
-drwxr-xr-x   0 andrewjd   (504) staff       (20)        0 2023-12-02 04:08:42.025829 nyct-gtfs-1.3.2/nyct_gtfs.egg-info/
--rw-r--r--   0 andrewjd   (504) staff       (20)    13213 2023-12-02 04:08:42.000000 nyct-gtfs-1.3.2/nyct_gtfs.egg-info/PKG-INFO
--rw-r--r--   0 andrewjd   (504) staff       (20)      587 2023-12-02 04:08:42.000000 nyct-gtfs-1.3.2/nyct_gtfs.egg-info/SOURCES.txt
--rw-r--r--   0 andrewjd   (504) staff       (20)        1 2023-12-02 04:08:42.000000 nyct-gtfs-1.3.2/nyct_gtfs.egg-info/dependency_links.txt
--rw-r--r--   0 andrewjd   (504) staff       (20)       24 2023-12-02 04:08:42.000000 nyct-gtfs-1.3.2/nyct_gtfs.egg-info/requires.txt
--rw-r--r--   0 andrewjd   (504) staff       (20)       10 2023-12-02 04:08:42.000000 nyct-gtfs-1.3.2/nyct_gtfs.egg-info/top_level.txt
--rw-r--r--   0 andrewjd   (504) staff       (20)       38 2023-12-02 04:08:42.026755 nyct-gtfs-1.3.2/setup.cfg
--rw-r--r--   0 andrewjd   (504) staff       (20)      966 2023-12-02 04:08:15.000000 nyct-gtfs-1.3.2/setup.py
-drwxr-xr-x   0 andrewjd   (504) staff       (20)        0 2023-12-02 04:08:42.025422 nyct-gtfs-1.3.2/tests/
--rw-r--r--   0 andrewjd   (504) staff       (20)    18051 2023-12-02 04:08:15.000000 nyct-gtfs-1.3.2/tests/test_feed_parse.py
--rw-r--r--   0 andrewjd   (504) staff       (20)    17586 2023-11-24 02:22:03.000000 nyct-gtfs-1.3.2/tests/test_feed_parse_cpp.py
+drwxr-xr-x   0 andrewjd   (504) staff       (20)        0 2024-05-05 00:55:38.926884 nyct_gtfs-1.3.3/
+-rw-r--r--   0 andrewjd   (504) staff       (20)     1073 2023-11-24 02:22:03.000000 nyct_gtfs-1.3.3/LICENSE.txt
+-rw-r--r--   0 andrewjd   (504) staff       (20)    13221 2024-05-05 00:55:38.926464 nyct_gtfs-1.3.3/PKG-INFO
+-rw-r--r--   0 andrewjd   (504) staff       (20)    12682 2023-11-24 02:22:03.000000 nyct_gtfs-1.3.3/README.md
+drwxr-xr-x   0 andrewjd   (504) staff       (20)        0 2024-05-05 00:55:38.919930 nyct_gtfs-1.3.3/nyct_gtfs/
+-rw-r--r--   0 andrewjd   (504) staff       (20)      182 2023-11-24 02:22:03.000000 nyct_gtfs-1.3.3/nyct_gtfs/__init__.py
+drwxr-xr-x   0 andrewjd   (504) staff       (20)        0 2024-05-05 00:55:38.922084 nyct_gtfs-1.3.3/nyct_gtfs/compiled_gtfs/
+-rw-r--r--   0 andrewjd   (504) staff       (20)        0 2023-11-24 02:22:03.000000 nyct_gtfs-1.3.3/nyct_gtfs/compiled_gtfs/__init__.py
+-rw-r--r--   0 andrewjd   (504) staff       (20)    15436 2023-11-24 02:22:03.000000 nyct_gtfs-1.3.3/nyct_gtfs/compiled_gtfs/gtfs_realtime_pb2.py
+-rw-r--r--   0 andrewjd   (504) staff       (20)     4593 2023-11-24 02:22:03.000000 nyct_gtfs-1.3.3/nyct_gtfs/compiled_gtfs/nyct_subway_pb2.py
+-rw-r--r--   0 andrewjd   (504) staff       (20)     4914 2023-11-24 02:22:03.000000 nyct_gtfs-1.3.3/nyct_gtfs/cpp_parser_wrapper.py
+-rw-r--r--   0 andrewjd   (504) staff       (20)    14313 2023-11-24 02:22:03.000000 nyct_gtfs-1.3.3/nyct_gtfs/feed.py
+drwxr-xr-x   0 andrewjd   (504) staff       (20)        0 2024-05-05 00:55:38.922843 nyct_gtfs-1.3.3/nyct_gtfs/gtfs_static/
+-rw-r--r--   0 andrewjd   (504) staff       (20)    71961 2023-11-24 02:22:03.000000 nyct_gtfs-1.3.3/nyct_gtfs/gtfs_static/stops.txt
+-rw-r--r--   0 andrewjd   (504) staff       (20)  1883488 2023-11-24 02:22:03.000000 nyct_gtfs-1.3.3/nyct_gtfs/gtfs_static/trips.txt
+-rw-r--r--   0 andrewjd   (504) staff       (20)     3324 2023-11-24 02:22:03.000000 nyct_gtfs-1.3.3/nyct_gtfs/gtfs_static_types.py
+-rw-r--r--   0 andrewjd   (504) staff       (20)     8615 2023-11-24 02:22:03.000000 nyct_gtfs-1.3.3/nyct_gtfs/stop_time_update.py
+-rw-r--r--   0 andrewjd   (504) staff       (20)    17293 2023-12-02 04:08:15.000000 nyct_gtfs-1.3.3/nyct_gtfs/trip.py
+drwxr-xr-x   0 andrewjd   (504) staff       (20)        0 2024-05-05 00:55:38.925986 nyct_gtfs-1.3.3/nyct_gtfs.egg-info/
+-rw-r--r--   0 andrewjd   (504) staff       (20)    13221 2024-05-05 00:55:38.000000 nyct_gtfs-1.3.3/nyct_gtfs.egg-info/PKG-INFO
+-rw-r--r--   0 andrewjd   (504) staff       (20)      587 2024-05-05 00:55:38.000000 nyct_gtfs-1.3.3/nyct_gtfs.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewjd   (504) staff       (20)        1 2024-05-05 00:55:38.000000 nyct_gtfs-1.3.3/nyct_gtfs.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewjd   (504) staff       (20)       32 2024-05-05 00:55:38.000000 nyct_gtfs-1.3.3/nyct_gtfs.egg-info/requires.txt
+-rw-r--r--   0 andrewjd   (504) staff       (20)       10 2024-05-05 00:55:38.000000 nyct_gtfs-1.3.3/nyct_gtfs.egg-info/top_level.txt
+-rw-r--r--   0 andrewjd   (504) staff       (20)       38 2024-05-05 00:55:38.926942 nyct_gtfs-1.3.3/setup.cfg
+-rw-r--r--   0 andrewjd   (504) staff       (20)      974 2024-05-05 00:54:23.000000 nyct_gtfs-1.3.3/setup.py
+drwxr-xr-x   0 andrewjd   (504) staff       (20)        0 2024-05-05 00:55:38.925310 nyct_gtfs-1.3.3/tests/
+-rw-r--r--   0 andrewjd   (504) staff       (20)    18051 2023-12-02 04:08:15.000000 nyct_gtfs-1.3.3/tests/test_feed_parse.py
+-rw-r--r--   0 andrewjd   (504) staff       (20)    17586 2023-11-24 02:22:03.000000 nyct_gtfs-1.3.3/tests/test_feed_parse_cpp.py
```

### Comparing `nyct-gtfs-1.3.2/LICENSE.txt` & `nyct_gtfs-1.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nyct-gtfs-1.3.2/PKG-INFO` & `nyct_gtfs-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: nyct-gtfs
-Version: 1.3.2
+Version: 1.3.3
 Summary: Real-time NYC subway data parsing for humans
 Home-page: https://github.com/Andrew-Dickinson/nyct-gtfs
 Author: Andrew Dickinson
 Author-email: andrew.dickinson.0216@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: requests
-Requires-Dist: protobuf
+Requires-Dist: protobuf==4.25.3
 Requires-Dist: httpx
 
 
 # NYCT-GTFS - Real-time NYC subway data parsing for humans
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 [![Stargazers][stars-shield]][stars-url]
```

### Comparing `nyct-gtfs-1.3.2/README.md` & `nyct_gtfs-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `nyct-gtfs-1.3.2/nyct_gtfs/compiled_gtfs/gtfs_realtime_pb2.py` & `nyct_gtfs-1.3.3/nyct_gtfs/compiled_gtfs/gtfs_realtime_pb2.py`

 * *Files identical despite different names*

### Comparing `nyct-gtfs-1.3.2/nyct_gtfs/compiled_gtfs/nyct_subway_pb2.py` & `nyct_gtfs-1.3.3/nyct_gtfs/compiled_gtfs/nyct_subway_pb2.py`

 * *Files identical despite different names*

### Comparing `nyct-gtfs-1.3.2/nyct_gtfs/cpp_parser_wrapper.py` & `nyct_gtfs-1.3.3/nyct_gtfs/cpp_parser_wrapper.py`

 * *Files identical despite different names*

### Comparing `nyct-gtfs-1.3.2/nyct_gtfs/feed.py` & `nyct_gtfs-1.3.3/nyct_gtfs/feed.py`

 * *Files identical despite different names*

### Comparing `nyct-gtfs-1.3.2/nyct_gtfs/gtfs_static/stops.txt` & `nyct_gtfs-1.3.3/nyct_gtfs/gtfs_static/stops.txt`

 * *Files identical despite different names*

### Comparing `nyct-gtfs-1.3.2/nyct_gtfs/gtfs_static/trips.txt` & `nyct_gtfs-1.3.3/nyct_gtfs/gtfs_static/trips.txt`

 * *Files identical despite different names*

### Comparing `nyct-gtfs-1.3.2/nyct_gtfs/gtfs_static_types.py` & `nyct_gtfs-1.3.3/nyct_gtfs/gtfs_static_types.py`

 * *Files identical despite different names*

### Comparing `nyct-gtfs-1.3.2/nyct_gtfs/stop_time_update.py` & `nyct_gtfs-1.3.3/nyct_gtfs/stop_time_update.py`

 * *Files identical despite different names*

### Comparing `nyct-gtfs-1.3.2/nyct_gtfs/trip.py` & `nyct_gtfs-1.3.3/nyct_gtfs/trip.py`

 * *Files identical despite different names*

### Comparing `nyct-gtfs-1.3.2/nyct_gtfs.egg-info/PKG-INFO` & `nyct_gtfs-1.3.3/nyct_gtfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: nyct-gtfs
-Version: 1.3.2
+Version: 1.3.3
 Summary: Real-time NYC subway data parsing for humans
 Home-page: https://github.com/Andrew-Dickinson/nyct-gtfs
 Author: Andrew Dickinson
 Author-email: andrew.dickinson.0216@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: requests
-Requires-Dist: protobuf
+Requires-Dist: protobuf==4.25.3
 Requires-Dist: httpx
 
 
 # NYCT-GTFS - Real-time NYC subway data parsing for humans
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 [![Stargazers][stars-shield]][stars-url]
```

### Comparing `nyct-gtfs-1.3.2/nyct_gtfs.egg-info/SOURCES.txt` & `nyct_gtfs-1.3.3/nyct_gtfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nyct-gtfs-1.3.2/setup.py` & `nyct_gtfs-1.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="nyct-gtfs",
-    version="1.3.2",
+    version="1.3.3",
     description="Real-time NYC subway data parsing for humans",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Andrew-Dickinson/nyct-gtfs",
     author="Andrew Dickinson",
     author_email="andrew.dickinson.0216@gmail.com",
     license="MIT",
@@ -24,9 +24,9 @@
         "Operating System :: OS Independent"
     ],
     packages=["nyct_gtfs", "nyct_gtfs.compiled_gtfs"],
     include_package_data=True,
     package_data={
         "nyct_gtfs": ["gtfs_static/*.txt"]
     },
-    install_requires=["requests", "protobuf", "httpx"]
+    install_requires=["requests", "protobuf==4.25.3", "httpx"]
 )
```

### Comparing `nyct-gtfs-1.3.2/tests/test_feed_parse.py` & `nyct_gtfs-1.3.3/tests/test_feed_parse.py`

 * *Files identical despite different names*

### Comparing `nyct-gtfs-1.3.2/tests/test_feed_parse_cpp.py` & `nyct_gtfs-1.3.3/tests/test_feed_parse_cpp.py`

 * *Files identical despite different names*

