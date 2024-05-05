# Comparing `tmp/snakestream-0.3.0.tar.gz` & `tmp/snakestream-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakestream-0.3.0.tar", last modified: Wed May  1 10:19:22 2024, max compression
+gzip compressed data, was "snakestream-0.3.1.tar", last modified: Sun May  5 20:35:51 2024, max compression
```

## Comparing `snakestream-0.3.0.tar` & `snakestream-0.3.1.tar`

### file list

```diff
@@ -1,56 +1,58 @@
-drwxr-xr-x   0 tommy     (1000) tommy     (1000)        0 2024-05-01 10:19:22.813450 snakestream-0.3.0/
--rw-r--r--   0 tommy     (1000) tommy     (1000)      594 2022-11-14 20:54:45.000000 snakestream-0.3.0/.coveragerc
-drwxr-xr-x   0 tommy     (1000) tommy     (1000)        0 2024-05-01 10:19:22.805450 snakestream-0.3.0/.github/
-drwxr-xr-x   0 tommy     (1000) tommy     (1000)        0 2024-05-01 10:19:22.809450 snakestream-0.3.0/.github/workflows/
--rw-r--r--   0 tommy     (1000) tommy     (1000)     1128 2024-05-01 10:17:01.000000 snakestream-0.3.0/.github/workflows/check.yml
--rw-r--r--   0 tommy     (1000) tommy     (1000)      917 2024-05-01 10:17:01.000000 snakestream-0.3.0/.github/workflows/deliver.yml
--rw-r--r--   0 tommy     (1000) tommy     (1000)      572 2022-11-14 20:54:45.000000 snakestream-0.3.0/.gitignore
--rw-r--r--   0 tommy     (1000) tommy     (1000)      490 2022-11-14 20:54:45.000000 snakestream-0.3.0/.readthedocs.yml
--rw-r--r--   0 tommy     (1000) tommy     (1000)     1081 2022-11-14 20:54:45.000000 snakestream-0.3.0/LICENSE.txt
--rw-r--r--   0 tommy     (1000) tommy     (1000)     3704 2024-05-01 10:19:22.813450 snakestream-0.3.0/PKG-INFO
--rw-r--r--   0 tommy     (1000) tommy     (1000)     2965 2024-05-01 10:17:01.000000 snakestream-0.3.0/README.md
--rw-r--r--   0 tommy     (1000) tommy     (1000)      346 2022-11-14 20:54:45.000000 snakestream-0.3.0/pyproject.toml
--rw-r--r--   0 tommy     (1000) tommy     (1000)      149 2024-04-28 17:38:11.000000 snakestream-0.3.0/requirements-dev.txt
--rw-r--r--   0 tommy     (1000) tommy     (1000)       52 2023-01-15 20:46:44.000000 snakestream-0.3.0/requirements.txt
--rw-r--r--   0 tommy     (1000) tommy     (1000)     1163 2024-05-01 10:19:22.813450 snakestream-0.3.0/setup.cfg
--rw-r--r--   0 tommy     (1000) tommy     (1000)      964 2023-02-05 22:06:05.000000 snakestream-0.3.0/setup.py
-drwxr-xr-x   0 tommy     (1000) tommy     (1000)        0 2024-05-01 10:19:22.805450 snakestream-0.3.0/src/
-drwxr-xr-x   0 tommy     (1000) tommy     (1000)        0 2024-05-01 10:19:22.809450 snakestream-0.3.0/src/snakestream/
--rw-r--r--   0 tommy     (1000) tommy     (1000)      614 2024-05-01 10:17:01.000000 snakestream-0.3.0/src/snakestream/__init__.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)      484 2023-01-29 23:14:42.000000 snakestream-0.3.0/src/snakestream/collector.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)    10270 2024-05-01 10:17:01.000000 snakestream-0.3.0/src/snakestream/core.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)       48 2022-12-18 20:26:15.000000 snakestream-0.3.0/src/snakestream/exception.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)      644 2023-01-22 22:20:19.000000 snakestream-0.3.0/src/snakestream/sort.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)      439 2023-09-03 17:08:29.000000 snakestream-0.3.0/src/snakestream/stream_builder.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)     3555 2024-04-28 17:38:11.000000 snakestream-0.3.0/src/snakestream/type.py
-drwxr-xr-x   0 tommy     (1000) tommy     (1000)        0 2024-05-01 10:19:22.813450 snakestream-0.3.0/src/snakestream.egg-info/
--rw-r--r--   0 tommy     (1000) tommy     (1000)     3704 2024-05-01 10:19:22.000000 snakestream-0.3.0/src/snakestream.egg-info/PKG-INFO
--rw-r--r--   0 tommy     (1000) tommy     (1000)     1109 2024-05-01 10:19:22.000000 snakestream-0.3.0/src/snakestream.egg-info/SOURCES.txt
--rw-r--r--   0 tommy     (1000) tommy     (1000)        1 2024-05-01 10:19:22.000000 snakestream-0.3.0/src/snakestream.egg-info/dependency_links.txt
--rw-r--r--   0 tommy     (1000) tommy     (1000)        1 2022-12-18 20:51:22.000000 snakestream-0.3.0/src/snakestream.egg-info/not-zip-safe
--rw-r--r--   0 tommy     (1000) tommy     (1000)      101 2024-05-01 10:19:22.000000 snakestream-0.3.0/src/snakestream.egg-info/requires.txt
--rw-r--r--   0 tommy     (1000) tommy     (1000)       12 2024-05-01 10:19:22.000000 snakestream-0.3.0/src/snakestream.egg-info/top_level.txt
-drwxr-xr-x   0 tommy     (1000) tommy     (1000)        0 2024-05-01 10:19:22.813450 snakestream-0.3.0/tests/
--rw-r--r--   0 tommy     (1000) tommy     (1000)     1103 2023-02-05 22:06:05.000000 snakestream-0.3.0/tests/conftest.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)     1001 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_all_match.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)     1012 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_any_match.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)      594 2023-09-03 17:08:29.000000 snakestream-0.3.0/tests/test_builder.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)     1663 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_collect.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)     1312 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_concat.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)      648 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_count.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)     1163 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_distinct.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)      295 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_empty.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)     1362 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_filter.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)      823 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_find_any.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)     1444 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_flat_map.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)      710 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_for_each.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)     2216 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_inputs.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)      533 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_integration.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)     1418 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_map.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)     2049 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_max.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)     2047 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_min.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)     1005 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_none_match.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)     1246 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_parallel.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)     2489 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_peek.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)     1094 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_reduce.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)     1671 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_sorted.py
+drwxr-xr-x   0 tommy     (1000) tommy     (1000)        0 2024-05-05 20:35:51.290648 snakestream-0.3.1/
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      594 2022-11-14 20:54:45.000000 snakestream-0.3.1/.coveragerc
+drwxr-xr-x   0 tommy     (1000) tommy     (1000)        0 2024-05-05 20:35:51.282648 snakestream-0.3.1/.github/
+drwxr-xr-x   0 tommy     (1000) tommy     (1000)        0 2024-05-05 20:35:51.282648 snakestream-0.3.1/.github/workflows/
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     1128 2024-05-01 10:17:01.000000 snakestream-0.3.1/.github/workflows/check.yml
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      917 2024-05-01 10:17:01.000000 snakestream-0.3.1/.github/workflows/deliver.yml
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      572 2022-11-14 20:54:45.000000 snakestream-0.3.1/.gitignore
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      490 2022-11-14 20:54:45.000000 snakestream-0.3.1/.readthedocs.yml
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     1081 2022-11-14 20:54:45.000000 snakestream-0.3.1/LICENSE.txt
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     4441 2024-05-05 20:35:51.290648 snakestream-0.3.1/PKG-INFO
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     3702 2024-05-05 20:31:58.000000 snakestream-0.3.1/README.md
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      346 2022-11-14 20:54:45.000000 snakestream-0.3.1/pyproject.toml
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      161 2024-05-05 20:31:58.000000 snakestream-0.3.1/requirements-dev.txt
+-rw-r--r--   0 tommy     (1000) tommy     (1000)       52 2023-01-15 20:46:44.000000 snakestream-0.3.1/requirements.txt
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     1163 2024-05-05 20:35:51.290648 snakestream-0.3.1/setup.cfg
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      964 2023-02-05 22:06:05.000000 snakestream-0.3.1/setup.py
+drwxr-xr-x   0 tommy     (1000) tommy     (1000)        0 2024-05-05 20:35:51.282648 snakestream-0.3.1/src/
+drwxr-xr-x   0 tommy     (1000) tommy     (1000)        0 2024-05-05 20:35:51.286648 snakestream-0.3.1/src/snakestream/
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      614 2024-05-01 10:17:01.000000 snakestream-0.3.1/src/snakestream/__init__.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      484 2023-01-29 23:14:42.000000 snakestream-0.3.1/src/snakestream/collector.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)    10650 2024-05-05 20:31:58.000000 snakestream-0.3.1/src/snakestream/core.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)       48 2022-12-18 20:26:15.000000 snakestream-0.3.1/src/snakestream/exception.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      644 2023-01-22 22:20:19.000000 snakestream-0.3.1/src/snakestream/sort.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      439 2023-09-03 17:08:29.000000 snakestream-0.3.1/src/snakestream/stream_builder.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     3691 2024-05-05 20:31:58.000000 snakestream-0.3.1/src/snakestream/type.py
+drwxr-xr-x   0 tommy     (1000) tommy     (1000)        0 2024-05-05 20:35:51.290648 snakestream-0.3.1/src/snakestream.egg-info/
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     4441 2024-05-05 20:35:51.000000 snakestream-0.3.1/src/snakestream.egg-info/PKG-INFO
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     1154 2024-05-05 20:35:51.000000 snakestream-0.3.1/src/snakestream.egg-info/SOURCES.txt
+-rw-r--r--   0 tommy     (1000) tommy     (1000)        1 2024-05-05 20:35:51.000000 snakestream-0.3.1/src/snakestream.egg-info/dependency_links.txt
+-rw-r--r--   0 tommy     (1000) tommy     (1000)        1 2022-12-18 20:51:22.000000 snakestream-0.3.1/src/snakestream.egg-info/not-zip-safe
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      101 2024-05-05 20:35:51.000000 snakestream-0.3.1/src/snakestream.egg-info/requires.txt
+-rw-r--r--   0 tommy     (1000) tommy     (1000)       12 2024-05-05 20:35:51.000000 snakestream-0.3.1/src/snakestream.egg-info/top_level.txt
+drwxr-xr-x   0 tommy     (1000) tommy     (1000)        0 2024-05-05 20:35:51.290648 snakestream-0.3.1/tests/
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     1103 2023-02-05 22:06:05.000000 snakestream-0.3.1/tests/conftest.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     1001 2024-05-01 10:17:01.000000 snakestream-0.3.1/tests/test_all_match.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     1012 2024-05-01 10:17:01.000000 snakestream-0.3.1/tests/test_any_match.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      594 2023-09-03 17:08:29.000000 snakestream-0.3.1/tests/test_builder.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     1774 2024-05-05 20:31:58.000000 snakestream-0.3.1/tests/test_close.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     1663 2024-05-01 10:17:01.000000 snakestream-0.3.1/tests/test_collect.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     1312 2024-05-01 10:17:01.000000 snakestream-0.3.1/tests/test_concat.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      648 2024-05-01 10:17:01.000000 snakestream-0.3.1/tests/test_count.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     1163 2024-05-01 10:17:01.000000 snakestream-0.3.1/tests/test_distinct.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      295 2024-05-01 10:17:01.000000 snakestream-0.3.1/tests/test_empty.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     1362 2024-05-01 10:17:01.000000 snakestream-0.3.1/tests/test_filter.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      823 2024-05-01 10:17:01.000000 snakestream-0.3.1/tests/test_find_any.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     1609 2024-05-05 20:31:58.000000 snakestream-0.3.1/tests/test_flat_map.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      710 2024-05-01 10:17:01.000000 snakestream-0.3.1/tests/test_for_each.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     2798 2024-05-05 20:31:58.000000 snakestream-0.3.1/tests/test_inputs.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      533 2024-05-01 10:17:01.000000 snakestream-0.3.1/tests/test_integration.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     1418 2024-05-01 10:17:01.000000 snakestream-0.3.1/tests/test_map.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     2049 2024-05-01 10:17:01.000000 snakestream-0.3.1/tests/test_max.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     2047 2024-05-01 10:17:01.000000 snakestream-0.3.1/tests/test_min.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     1005 2024-05-01 10:17:01.000000 snakestream-0.3.1/tests/test_none_match.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     1658 2024-05-05 20:31:58.000000 snakestream-0.3.1/tests/test_parallel.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     2489 2024-05-01 10:17:01.000000 snakestream-0.3.1/tests/test_peek.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     1094 2024-05-01 10:17:01.000000 snakestream-0.3.1/tests/test_reduce.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      879 2024-05-05 20:31:58.000000 snakestream-0.3.1/tests/test_sequential.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     1671 2024-05-01 10:17:01.000000 snakestream-0.3.1/tests/test_sorted.py
```

### Comparing `snakestream-0.3.0/.coveragerc` & `snakestream-0.3.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `snakestream-0.3.0/.github/workflows/check.yml` & `snakestream-0.3.1/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `snakestream-0.3.0/.github/workflows/deliver.yml` & `snakestream-0.3.1/.github/workflows/deliver.yml`

 * *Files identical despite different names*

### Comparing `snakestream-0.3.0/.gitignore` & `snakestream-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `snakestream-0.3.0/LICENSE.txt` & `snakestream-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snakestream-0.3.0/PKG-INFO` & `snakestream-0.3.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: snakestream
-Version: 0.3.0
-Summary: Java like streams for snakes
-Home-page: https://github.com/carby/snakestream
-Author: Tommy Derngren
-Author-email: tommy.derngren@hiq.se
-License: MIT
-Project-URL: Documentation, https://github.com/carby/snakestream/wiki
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: importlib-metadata; python_version < "3.8"
-Provides-Extra: testing
-Requires-Dist: setuptools; extra == "testing"
-Requires-Dist: pytest; extra == "testing"
-Requires-Dist: pytest-cov; extra == "testing"
-Requires-Dist: pytest-asyncio; extra == "testing"
-
 # Snakestream
 **Java like streams for snakes**
 
 This is a python streaming api with witch you can get a similar experience as with the Java streams api from Java 8. There is no feature parity, what has been done so far is a beginning, and we will see where the road takes us.
 
 ### Features
 - Create a stream from a List, Generator or AsyncGenerator.
@@ -83,27 +61,40 @@
 Then in the shell
 ```shell
 ~/t/test> python test.py
 d
 e
 ```
 
+### Auto Close
+Contextlib already supports something that is very similar to the AutoClose from Java. Just as long as your class has the .close() attribute it will be called. In this case it's very fortunate that the Java API and contextlib play so nice together. Here is an example:
+
+```
+from contextlib import closing
+
+with closing(Stream.of([1, 2, 3, 4, 1, 2, 3, 4])) as stream:
+    it = await stream \
+        .map(lambda x: int_2_letter[x]) \
+        .distinct() \
+        .collect(to_list)
+```
+
+This can be especially useful if you are subclassing Stream to do something that is kinda like IO related and you have some resource that needs to get relased after the stream. You would then just add the logic to do that in your .close() method and contextlib will handle the rest
+
 ### Migration
 These are a list of the known breaking changes. Until release 1.0.0 focus will be on implementing features and changing things that does not align with how streams work in java.
-- **0.2.4 -> 0.2.5:** stream_of() has been removed in favour of Stream.of() for getting closer to the java api.
+- **0.2.4 -> 0.3.0:** stream_of() has been removed in favour of Stream.of() for getting closer to the java api.
 - **0.1.0 -> 0.2.0:** The `unique()` function has been renamed `distinct()`. So rename all imports of that function, and it should be OK
 - **0.0.5 -> 0.0.6:** The `stream()` function has been renamed `stream_of()`. So rename all imports of that function, and it should be OK
 
 ### Left to do:
 
 BaseStream:
-close()
 isParallel()
 iterator()
-onClose(Runnable closeHandler)
 spliterator()
 unordered()
 
 Stream:
 collect(Supplier<R> supplier, BiConsumer<R,? super T> accumulator, BiConsumer<R,R> combiner)
 flatMapToDouble(Function<? super T,? extends DoubleStream> mapper)
 flatMapToInt(Function<? super T,? extends IntStream> mapper)
@@ -111,14 +102,13 @@
 forEachOrdered(Consumer<? super T> action)
 generate(Supplier<T> s)
 iterate(T seed, UnaryOperator<T> f)
 limit(long maxSize)
 mapToDouble(ToDoubleFunction<? super T> mapper)
 mapToInt(ToIntFunction<? super T> mapper)
 mapToLong(ToLongFunction<? super T> mapper)
-of(T t)
 
 reduce(BinaryOperator<T> accumulator) // have done the one with the identity
 skip(long n)
 sorted() // have done the one with a comparator
 toArray()
 toArray(IntFunction<A[]> generator)
```

### Comparing `snakestream-0.3.0/setup.cfg` & `snakestream-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `snakestream-0.3.0/setup.py` & `snakestream-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `snakestream-0.3.0/src/snakestream/__init__.py` & `snakestream-0.3.1/src/snakestream/__init__.py`

 * *Files identical despite different names*

### Comparing `snakestream-0.3.0/src/snakestream/core.py` & `snakestream-0.3.1/src/snakestream/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,111 +5,89 @@
 from inspect import iscoroutinefunction
 from typing import Callable, Optional, AsyncIterable, List, \
     Union, AsyncGenerator, Any
 
 from snakestream.collector import to_generator
 from snakestream.exception import StreamBuildException
 from snakestream.sort import merge_sort
-from snakestream.type import R, T, AbstractStream, AbstractStreamBuilder, Accumulator, Comparator, Consumer, \
-    FlatMapper, Mapper, Predicate, Streamable
+from snakestream.type import R, T, AbstractStream, AbstractStreamBuilder, Accumulator, CloseHandler, Comparator, Consumer, \
+    FlatMapper, Mapper, Predicate
 
 
 PROCESSES: int = 4
 
 
-async def _normalize(iterable: Streamable) -> AsyncGenerator:
-    for i in iterable:
-        yield i
+async def _normalize(source: Any) -> AsyncGenerator:
+    if hasattr(source, '__iter__') or hasattr(source, '__next__'):
+        for i in source:
+            yield i
+    else:
+        yield source
+
+
+def _accept(source: Any) -> Optional[AsyncGenerator]:
+    if isinstance(source, AsyncGenerator) or isinstance(source, AsyncIterable):
+        return source
+    return None
 
 
 async def _concat(a: 'Stream', b: 'Stream') -> AsyncGenerator:
     async for i in a._compose():
         yield i
     async for j in b._compose():
         yield j
 
 
 class BaseStream():
-    def __init__(self, streamable: Streamable) -> None:
-        if isinstance(streamable, AsyncGenerator) or isinstance(streamable, AsyncIterable):
-            self._stream = streamable
-        else:
-            self._stream: AsyncGenerator = _normalize(streamable)
+    def __init__(self, source: Any) -> None:
+        self._stream = _accept(source) or _normalize(source)
         self._chain: List[Callable] = []
         self.is_parallel = False
+        self._close_handlers = []
 
     def _sequential(self, intermediaries: List[Callable], iterable: AsyncGenerator) -> AsyncGenerator:
         if len(intermediaries) == 0:
             return iterable
         if len(intermediaries) == 1:
             fn = intermediaries.pop(0)
             return fn(iterable)
         fn = intermediaries.pop(0)
         return self._sequential(intermediaries, fn(iterable))
 
-    async def _parallel(
-        self,
-        intermediaries: List[Callable],
-        iterable: AsyncGenerator,
-        processes: int = PROCESSES
-    ) -> AsyncGenerator:
-        async_iterators = [self._sequential(intermediaries[:], iterable) for n in range(processes)]
-        tasks = [asyncio.ensure_future(n.__anext__()) for n in async_iterators]
-
-        while any([n is not None for n in tasks]):
-
-            waitlist = filter(lambda n: n is not None, tasks)
-            done, _ = await asyncio.wait(waitlist, return_when=asyncio.FIRST_COMPLETED)
-
-            for task in done:
-                task_idx = tasks.index(task)
-                try:
-                    result = tasks[task_idx].result()
-                    tasks[task_idx] = asyncio.ensure_future(async_iterators[task_idx].__anext__())
-                    yield result
-                except StopAsyncIteration:
-                    tasks[task_idx] = None
-
     def _compose(self) -> AsyncGenerator:
-        if self.is_parallel:
-            return self._parallel(self._chain, self._stream)
-        else:
-            return self._sequential(self._chain, self._stream)
+        return self._sequential(self._chain, self._stream)
 
     def sequential(self) -> 'Stream':
-        self.stream = self._compose()
-        self.is_parallel = False
-
-        async def fn(iterable: AsyncGenerator) -> AsyncGenerator:
-            async for i in iterable:
-                yield i
-        self._chain = [fn]
-        return self
+        new_source = self._compose()
+        return Stream(new_source, self._close_handlers)
 
     def parallel(self) -> 'Stream':
-        self.stream = self._compose()
-        self.is_parallel = True
+        new_source = self._compose()
+        return ParallelStream(new_source, self._close_handlers)
 
-        async def fn(iterable: AsyncGenerator) -> AsyncGenerator:
-            async for i in iterable:
-                yield i
-        self._chain = [fn]
+    def on_close(self, close_handler: CloseHandler) -> 'Stream':
+        self._close_handlers.append(close_handler)
         return self
 
+    def close(self) -> None:
+        for close_handler in self._close_handlers:
+            close_handler()
+
 
 #
 # If you add a method here, also add it to AbstractStream
 #
 class Stream(BaseStream, AbstractStream):
-    def __init__(self, streamable: Streamable) -> None:
-        super().__init__(streamable)
+    def __init__(self, source: Any, close_handlers: Optional[List[CloseHandler]] = None) -> None:
+        super().__init__(source)
+        self._close_handlers = close_handlers or []
 
     @staticmethod
-    def of(iterable: Streamable) -> 'Stream':
-        return Stream(iterable)
+    def of(source: Any) -> 'Stream':
+        return Stream(source)
 
     @staticmethod
     def empty() -> 'Stream':
         return Stream([])
 
     @staticmethod
     async def concat(a: 'Stream', b: 'Stream') -> 'Stream':
@@ -312,7 +290,39 @@
         return False
 
     async def count(self) -> int:
         c = 0
         async for _ in self._compose():
             c += 1
         return c
+
+
+class ParallelStream(Stream):
+    def __init__(self, source: Any, close_handlers: Optional[List[CloseHandler]] = None) -> None:
+        super().__init__(source)
+        self._close_handlers = close_handlers or []
+
+    def _compose(self) -> AsyncGenerator:
+        return self._parallel(self._chain, self._stream)
+
+    async def _parallel(
+        self,
+        intermediaries: List[Callable],
+        iterable: AsyncGenerator,
+        processes: int = PROCESSES
+    ) -> AsyncGenerator:
+        async_iterators = [self._sequential(intermediaries[:], iterable) for n in range(processes)]
+        tasks = [asyncio.ensure_future(n.__anext__()) for n in async_iterators]
+
+        while any([n is not None for n in tasks]):
+
+            waitlist = filter(lambda n: n is not None, tasks)
+            done, _ = await asyncio.wait(waitlist, return_when=asyncio.FIRST_COMPLETED)
+
+            for task in done:
+                task_idx = tasks.index(task)
+                try:
+                    result = tasks[task_idx].result()
+                    tasks[task_idx] = asyncio.ensure_future(async_iterators[task_idx].__anext__())
+                    yield result
+                except StopAsyncIteration:
+                    tasks[task_idx] = None
```

### Comparing `snakestream-0.3.0/src/snakestream/sort.py` & `snakestream-0.3.1/src/snakestream/sort.py`

 * *Files identical despite different names*

### Comparing `snakestream-0.3.0/src/snakestream/type.py` & `snakestream-0.3.1/src/snakestream/type.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,36 +4,40 @@
 
 #
 # Generic types
 #
 T = TypeVar('T')
 R = TypeVar('R')
 
-Streamable = Union[Iterable, AsyncIterable, Generator, AsyncGenerator]
-
 Predicate = Callable[[T], Union[bool, Awaitable[bool]]]
 
 # Intermediaries
 Filterer = Callable[[T], T]
 Mapper = Callable[[T], Optional[R]]
-FlatMapper = Callable[[Streamable], 'AbstractStream']
+FlatMapper = Callable[[Union[Iterable, AsyncIterable, Generator, AsyncGenerator]], 'AbstractStream']
 Comparator = Callable[[T, T], Union[bool, Awaitable[bool]]]
 Consumer = Callable[[T], T]
+CloseHandler = Callable[[], None]
 
 # Terminals
 Accumulator = Callable[[T, Union[T, R]], Union[T, R]]
 
 
 #
 # Classes
 #
 class AbstractStream(metaclass=abc.ABCMeta):
 
     @staticmethod
     @abc.abstractclassmethod
+    def of(source: Any) -> 'AbstractStream':
+        raise NotImplementedError
+
+    @staticmethod
+    @abc.abstractclassmethod
     def empty() -> 'AbstractStream':
         raise NotImplementedError
 
     @staticmethod
     @abc.abstractclassmethod
     async def concat(a: 'AbstractStream', b: 'AbstractStream') -> 'AbstractStream':
         raise NotImplementedError
```

### Comparing `snakestream-0.3.0/src/snakestream.egg-info/PKG-INFO` & `snakestream-0.3.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakestream
-Version: 0.3.0
+Version: 0.3.1
 Summary: Java like streams for snakes
 Home-page: https://github.com/carby/snakestream
 Author: Tommy Derngren
 Author-email: tommy.derngren@hiq.se
 License: MIT
 Project-URL: Documentation, https://github.com/carby/snakestream/wiki
 Platform: any
@@ -83,27 +83,40 @@
 Then in the shell
 ```shell
 ~/t/test> python test.py
 d
 e
 ```
 
+### Auto Close
+Contextlib already supports something that is very similar to the AutoClose from Java. Just as long as your class has the .close() attribute it will be called. In this case it's very fortunate that the Java API and contextlib play so nice together. Here is an example:
+
+```
+from contextlib import closing
+
+with closing(Stream.of([1, 2, 3, 4, 1, 2, 3, 4])) as stream:
+    it = await stream \
+        .map(lambda x: int_2_letter[x]) \
+        .distinct() \
+        .collect(to_list)
+```
+
+This can be especially useful if you are subclassing Stream to do something that is kinda like IO related and you have some resource that needs to get relased after the stream. You would then just add the logic to do that in your .close() method and contextlib will handle the rest
+
 ### Migration
 These are a list of the known breaking changes. Until release 1.0.0 focus will be on implementing features and changing things that does not align with how streams work in java.
-- **0.2.4 -> 0.2.5:** stream_of() has been removed in favour of Stream.of() for getting closer to the java api.
+- **0.2.4 -> 0.3.0:** stream_of() has been removed in favour of Stream.of() for getting closer to the java api.
 - **0.1.0 -> 0.2.0:** The `unique()` function has been renamed `distinct()`. So rename all imports of that function, and it should be OK
 - **0.0.5 -> 0.0.6:** The `stream()` function has been renamed `stream_of()`. So rename all imports of that function, and it should be OK
 
 ### Left to do:
 
 BaseStream:
-close()
 isParallel()
 iterator()
-onClose(Runnable closeHandler)
 spliterator()
 unordered()
 
 Stream:
 collect(Supplier<R> supplier, BiConsumer<R,? super T> accumulator, BiConsumer<R,R> combiner)
 flatMapToDouble(Function<? super T,? extends DoubleStream> mapper)
 flatMapToInt(Function<? super T,? extends IntStream> mapper)
@@ -111,14 +124,13 @@
 forEachOrdered(Consumer<? super T> action)
 generate(Supplier<T> s)
 iterate(T seed, UnaryOperator<T> f)
 limit(long maxSize)
 mapToDouble(ToDoubleFunction<? super T> mapper)
 mapToInt(ToIntFunction<? super T> mapper)
 mapToLong(ToLongFunction<? super T> mapper)
-of(T t)
 
 reduce(BinaryOperator<T> accumulator) // have done the one with the identity
 skip(long n)
 sorted() // have done the one with a comparator
 toArray()
 toArray(IntFunction<A[]> generator)
```

### Comparing `snakestream-0.3.0/src/snakestream.egg-info/SOURCES.txt` & `snakestream-0.3.1/src/snakestream.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 src/snakestream.egg-info/not-zip-safe
 src/snakestream.egg-info/requires.txt
 src/snakestream.egg-info/top_level.txt
 tests/conftest.py
 tests/test_all_match.py
 tests/test_any_match.py
 tests/test_builder.py
+tests/test_close.py
 tests/test_collect.py
 tests/test_concat.py
 tests/test_count.py
 tests/test_distinct.py
 tests/test_empty.py
 tests/test_filter.py
 tests/test_find_any.py
@@ -41,8 +42,9 @@
 tests/test_map.py
 tests/test_max.py
 tests/test_min.py
 tests/test_none_match.py
 tests/test_parallel.py
 tests/test_peek.py
 tests/test_reduce.py
+tests/test_sequential.py
 tests/test_sorted.py
```

### Comparing `snakestream-0.3.0/tests/conftest.py` & `snakestream-0.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `snakestream-0.3.0/tests/test_all_match.py` & `snakestream-0.3.1/tests/test_all_match.py`

 * *Files identical despite different names*

### Comparing `snakestream-0.3.0/tests/test_any_match.py` & `snakestream-0.3.1/tests/test_any_match.py`

 * *Files identical despite different names*

### Comparing `snakestream-0.3.0/tests/test_builder.py` & `snakestream-0.3.1/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `snakestream-0.3.0/tests/test_collect.py` & `snakestream-0.3.1/tests/test_collect.py`

 * *Files identical despite different names*

### Comparing `snakestream-0.3.0/tests/test_concat.py` & `snakestream-0.3.1/tests/test_concat.py`

 * *Files identical despite different names*

### Comparing `snakestream-0.3.0/tests/test_count.py` & `snakestream-0.3.1/tests/test_count.py`

 * *Files identical despite different names*

### Comparing `snakestream-0.3.0/tests/test_distinct.py` & `snakestream-0.3.1/tests/test_distinct.py`

 * *Files identical despite different names*

### Comparing `snakestream-0.3.0/tests/test_filter.py` & `snakestream-0.3.1/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `snakestream-0.3.0/tests/test_find_any.py` & `snakestream-0.3.1/tests/test_find_any.py`

 * *Files identical despite different names*

### Comparing `snakestream-0.3.0/tests/test_flat_map.py` & `snakestream-0.3.1/tests/test_flat_map.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,27 +28,31 @@
     except StopAsyncIteration:
         pass
     else:
         assert False
 
 
 @pytest.mark.asyncio
-async def test_flat_map_no_mixed_list() -> None:
-    it = Stream.of([[1, 2], [3, 4], 5]) \
+async def test_flat_map_mixed_list() -> None:
+    it = Stream.of([[1, 2], [3, 4], 5, [6, 7], 8]) \
         .flat_map(lambda x: Stream.of(x)) \
         .collect(to_generator)
 
     # then
     assert await it.__anext__() == 1
     assert await it.__anext__() == 2
     assert await it.__anext__() == 3
     assert await it.__anext__() == 4
+    assert await it.__anext__() == 5
+    assert await it.__anext__() == 6
+    assert await it.__anext__() == 7
+    assert await it.__anext__() == 8
     try:
         await it.__anext__()
-    except TypeError:
+    except StopAsyncIteration:
         pass
     else:
         assert False
 
 
 @pytest.mark.asyncio
 async def test_flat_map_async_function() -> None:
```

### Comparing `snakestream-0.3.0/tests/test_for_each.py` & `snakestream-0.3.1/tests/test_for_each.py`

 * *Files identical despite different names*

### Comparing `snakestream-0.3.0/tests/test_inputs.py` & `snakestream-0.3.1/tests/test_inputs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 # pylint: disable=missing-module-docstring
 # pylint: disable=missing-class-docstring
 # pylint: disable=missing-function-docstring
 # pylint: disable=invalid-name
 
-from typing import AsyncGenerator
+from typing import AsyncGenerator, Generator
 import pytest
 
 from snakestream import Stream
 from snakestream.collector import to_generator, to_list
 
 
 async def async_generator() -> AsyncGenerator:
     for i in range(1, 6):
         yield i
 
 
+def generator() -> Generator:
+    for i in range(1, 6):
+        yield i
+
+
 class AsyncIteratorImpl:
     def __init__(self, end_range):
         self.end = end_range
         self.start = -1
 
     def __aiter__(self):
         return self
@@ -87,10 +92,34 @@
     else:
         assert False
 
 
 @pytest.mark.asyncio
 async def test_null_input() -> None:
     # when
-    with pytest.raises(TypeError):
-        await Stream.of(None) \
-            .collect(to_list)
+    it = await Stream.of(None) \
+        .collect(to_list)
+    assert [None] == it
+
+
+@pytest.mark.asyncio
+async def test_single_var_input() -> None:
+    # when
+    it = await Stream.of(1) \
+        .collect(to_list)
+    assert [1] == it
+
+
+@pytest.mark.asyncio
+async def test_single_generator_input() -> None:
+    # when
+    it = await Stream.of(generator()) \
+        .collect(to_list)
+    assert [1, 2, 3, 4, 5] == it
+
+
+@pytest.mark.asyncio
+async def test_single_list_input() -> None:
+    # when
+    it = await Stream.of([4, 3, 2, 1]) \
+        .collect(to_list)
+    assert [4, 3, 2, 1] == it
```

### Comparing `snakestream-0.3.0/tests/test_integration.py` & `snakestream-0.3.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `snakestream-0.3.0/tests/test_map.py` & `snakestream-0.3.1/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `snakestream-0.3.0/tests/test_max.py` & `snakestream-0.3.1/tests/test_max.py`

 * *Files identical despite different names*

### Comparing `snakestream-0.3.0/tests/test_min.py` & `snakestream-0.3.1/tests/test_min.py`

 * *Files identical despite different names*

### Comparing `snakestream-0.3.0/tests/test_none_match.py` & `snakestream-0.3.1/tests/test_none_match.py`

 * *Files identical despite different names*

### Comparing `snakestream-0.3.0/tests/test_parallel.py` & `snakestream-0.3.1/tests/test_parallel.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,7 +45,24 @@
         .collect(to_list)
     end_sequential = time.time()
     time_sequential = end_sequential - start_sequential
 
     # then
     # usually something like 0,2 compared to 0.8
     assert (time_parallel) < (time_sequential)
+
+
+@pytest.mark.asyncio
+async def test_sequential_switch_to_sequential(int_2_letter) -> None:
+    # when
+    it = await Stream.of([1, 2, 3, 4, 1, 2, 3, 4]) \
+        .sequential() \
+        .map(lambda x: int_2_letter[x]) \
+        .parallel() \
+        .distinct() \
+        .collect(to_list)
+    # then
+    assert 4 == len(it)
+    assert 'a' in it
+    assert 'b' in it
+    assert 'c' in it
+    assert 'd' in it
```

### Comparing `snakestream-0.3.0/tests/test_peek.py` & `snakestream-0.3.1/tests/test_peek.py`

 * *Files identical despite different names*

### Comparing `snakestream-0.3.0/tests/test_reduce.py` & `snakestream-0.3.1/tests/test_reduce.py`

 * *Files identical despite different names*

### Comparing `snakestream-0.3.0/tests/test_sorted.py` & `snakestream-0.3.1/tests/test_sorted.py`

 * *Files identical despite different names*

