# Comparing `tmp/dmocker-0.0.1.tar.gz` & `tmp/dmocker-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmocker-0.0.1.tar", last modified: Mon Apr 29 09:26:25 2024, max compression
+gzip compressed data, was "dmocker-0.0.2.tar", last modified: Sun May  5 15:46:53 2024, max compression
```

## Comparing `dmocker-0.0.1.tar` & `dmocker-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 strecobyasha   (501) staff       (20)        0 2024-04-29 09:26:25.912639 dmocker-0.0.1/
--rw-r--r--   0 strecobyasha   (501) staff       (20)     1083 2024-04-29 08:58:23.000000 dmocker-0.0.1/LICENSE
--rw-r--r--   0 strecobyasha   (501) staff       (20)     2734 2024-04-29 09:26:25.912472 dmocker-0.0.1/PKG-INFO
--rw-r--r--   0 strecobyasha   (501) staff       (20)     2232 2024-04-29 09:03:01.000000 dmocker-0.0.1/README.md
-drwxr-xr-x   0 strecobyasha   (501) staff       (20)        0 2024-04-29 09:26:25.904091 dmocker-0.0.1/dmocker/
--rw-r--r--   0 strecobyasha   (501) staff       (20)       32 2024-04-29 03:32:29.000000 dmocker-0.0.1/dmocker/__init__.py
-drwxr-xr-x   0 strecobyasha   (501) staff       (20)        0 2024-04-29 09:26:25.905125 dmocker-0.0.1/dmocker/exceptions/
--rw-r--r--   0 strecobyasha   (501) staff       (20)     1758 2024-04-28 14:04:51.000000 dmocker-0.0.1/dmocker/exceptions/custom.py
--rw-r--r--   0 strecobyasha   (501) staff       (20)     1184 2024-04-29 07:23:56.000000 dmocker-0.0.1/dmocker/exceptions/validator.py
--rw-r--r--   0 strecobyasha   (501) staff       (20)     1902 2024-04-29 08:13:48.000000 dmocker-0.0.1/dmocker/main.py
-drwxr-xr-x   0 strecobyasha   (501) staff       (20)        0 2024-04-29 09:26:25.905913 dmocker-0.0.1/dmocker/src/
--rw-r--r--   0 strecobyasha   (501) staff       (20)     1869 2024-04-29 08:49:53.000000 dmocker-0.0.1/dmocker/src/arguments.py
--rw-r--r--   0 strecobyasha   (501) staff       (20)      692 2024-04-29 07:28:58.000000 dmocker-0.0.1/dmocker/src/container_info.py
--rw-r--r--   0 strecobyasha   (501) staff       (20)     1817 2024-04-29 07:31:59.000000 dmocker-0.0.1/dmocker/src/fetcher.py
-drwxr-xr-x   0 strecobyasha   (501) staff       (20)        0 2024-04-29 09:26:25.912298 dmocker-0.0.1/dmocker.egg-info/
--rw-r--r--   0 strecobyasha   (501) staff       (20)     2734 2024-04-29 09:26:25.000000 dmocker-0.0.1/dmocker.egg-info/PKG-INFO
--rw-r--r--   0 strecobyasha   (501) staff       (20)      441 2024-04-29 09:26:25.000000 dmocker-0.0.1/dmocker.egg-info/SOURCES.txt
--rw-r--r--   0 strecobyasha   (501) staff       (20)        1 2024-04-29 09:26:25.000000 dmocker-0.0.1/dmocker.egg-info/dependency_links.txt
--rw-r--r--   0 strecobyasha   (501) staff       (20)       43 2024-04-29 09:26:25.000000 dmocker-0.0.1/dmocker.egg-info/entry_points.txt
--rw-r--r--   0 strecobyasha   (501) staff       (20)        8 2024-04-29 09:26:25.000000 dmocker-0.0.1/dmocker.egg-info/top_level.txt
--rw-r--r--   0 strecobyasha   (501) staff       (20)      618 2024-04-29 08:23:22.000000 dmocker-0.0.1/pyproject.toml
--rw-r--r--   0 strecobyasha   (501) staff       (20)       38 2024-04-29 09:26:25.912675 dmocker-0.0.1/setup.cfg
-drwxr-xr-x   0 strecobyasha   (501) staff       (20)        0 2024-04-29 09:26:25.911915 dmocker-0.0.1/tests/
--rw-r--r--   0 strecobyasha   (501) staff       (20)     3511 2024-04-29 04:48:15.000000 dmocker-0.0.1/tests/test_arg_parser_container_logs.py
--rw-r--r--   0 strecobyasha   (501) staff       (20)     3114 2024-04-29 03:33:14.000000 dmocker-0.0.1/tests/test_arg_parser_containers.py
+drwxr-xr-x   0 strecobyasha   (501) staff       (20)        0 2024-05-05 15:46:53.490657 dmocker-0.0.2/
+-rw-r--r--   0 strecobyasha   (501) staff       (20)     1083 2024-04-29 08:58:23.000000 dmocker-0.0.2/LICENSE
+-rw-r--r--   0 strecobyasha   (501) staff       (20)     2734 2024-05-05 15:46:53.490476 dmocker-0.0.2/PKG-INFO
+-rw-r--r--   0 strecobyasha   (501) staff       (20)     2232 2024-04-29 09:03:01.000000 dmocker-0.0.2/README.md
+drwxr-xr-x   0 strecobyasha   (501) staff       (20)        0 2024-05-05 15:46:53.487691 dmocker-0.0.2/dmocker/
+-rw-r--r--   0 strecobyasha   (501) staff       (20)       32 2024-04-29 03:32:29.000000 dmocker-0.0.2/dmocker/__init__.py
+drwxr-xr-x   0 strecobyasha   (501) staff       (20)        0 2024-05-05 15:46:53.488813 dmocker-0.0.2/dmocker/exceptions/
+-rw-r--r--   0 strecobyasha   (501) staff       (20)     1758 2024-04-28 14:04:51.000000 dmocker-0.0.2/dmocker/exceptions/custom.py
+-rw-r--r--   0 strecobyasha   (501) staff       (20)     1243 2024-04-29 13:28:20.000000 dmocker-0.0.2/dmocker/exceptions/validator.py
+-rw-r--r--   0 strecobyasha   (501) staff       (20)     1902 2024-04-29 08:13:48.000000 dmocker-0.0.2/dmocker/main.py
+drwxr-xr-x   0 strecobyasha   (501) staff       (20)        0 2024-05-05 15:46:53.489529 dmocker-0.0.2/dmocker/src/
+-rw-r--r--   0 strecobyasha   (501) staff       (20)     1869 2024-04-29 08:49:53.000000 dmocker-0.0.2/dmocker/src/arguments.py
+-rw-r--r--   0 strecobyasha   (501) staff       (20)      692 2024-04-29 07:28:58.000000 dmocker-0.0.2/dmocker/src/container_info.py
+-rw-r--r--   0 strecobyasha   (501) staff       (20)     2722 2024-05-05 15:44:54.000000 dmocker-0.0.2/dmocker/src/fetcher.py
+drwxr-xr-x   0 strecobyasha   (501) staff       (20)        0 2024-05-05 15:46:53.490303 dmocker-0.0.2/dmocker.egg-info/
+-rw-r--r--   0 strecobyasha   (501) staff       (20)     2734 2024-05-05 15:46:53.000000 dmocker-0.0.2/dmocker.egg-info/PKG-INFO
+-rw-r--r--   0 strecobyasha   (501) staff       (20)      441 2024-05-05 15:46:53.000000 dmocker-0.0.2/dmocker.egg-info/SOURCES.txt
+-rw-r--r--   0 strecobyasha   (501) staff       (20)        1 2024-05-05 15:46:53.000000 dmocker-0.0.2/dmocker.egg-info/dependency_links.txt
+-rw-r--r--   0 strecobyasha   (501) staff       (20)       43 2024-05-05 15:46:53.000000 dmocker-0.0.2/dmocker.egg-info/entry_points.txt
+-rw-r--r--   0 strecobyasha   (501) staff       (20)        8 2024-05-05 15:46:53.000000 dmocker-0.0.2/dmocker.egg-info/top_level.txt
+-rw-r--r--   0 strecobyasha   (501) staff       (20)      618 2024-05-05 15:46:50.000000 dmocker-0.0.2/pyproject.toml
+-rw-r--r--   0 strecobyasha   (501) staff       (20)       38 2024-05-05 15:46:53.490705 dmocker-0.0.2/setup.cfg
+drwxr-xr-x   0 strecobyasha   (501) staff       (20)        0 2024-05-05 15:46:53.490002 dmocker-0.0.2/tests/
+-rw-r--r--   0 strecobyasha   (501) staff       (20)     3257 2024-04-29 13:20:35.000000 dmocker-0.0.2/tests/test_arg_parser_container_logs.py
+-rw-r--r--   0 strecobyasha   (501) staff       (20)     2756 2024-04-29 13:20:35.000000 dmocker-0.0.2/tests/test_arg_parser_containers.py
```

### Comparing `dmocker-0.0.1/LICENSE` & `dmocker-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dmocker-0.0.1/PKG-INFO` & `dmocker-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmocker
-Version: 0.0.1
+Version: 0.0.2
 Summary: Remote Docker control
 Author-email: strecobyasha <strecobyasha@protonmail.com>
 Project-URL: Homepage, https://github.com/strecobyasha/dmocker
 Project-URL: Issues, https://github.com/strecobyasha/dmocker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dmocker-0.0.1/README.md` & `dmocker-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dmocker-0.0.1/dmocker/exceptions/custom.py` & `dmocker-0.0.2/dmocker/exceptions/custom.py`

 * *Files identical despite different names*

### Comparing `dmocker-0.0.1/dmocker/exceptions/validator.py` & `dmocker-0.0.2/dmocker/exceptions/validator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """
 Validate parameters, that were passed to the main function.
 """
-from .custom import WrongFlagException, TooManyFlagsException, NotEnoughArgsException, LogsNumberException, \
-    LogsFollowException, TooManyParamsException, TooManyServersException
+from .custom import (LogsFollowException, LogsNumberException,
+                     NotEnoughArgsException, TooManyFlagsException,
+                     TooManyParamsException, TooManyServersException,
+                     WrongFlagException)
 
 
 def validate(args):
     if (task := args.task[0]) == 'ps':
         # Task format: dmocker server1 server2... serverN -t ps [a]
         if len(args.task) == 2 and args.task[1] != 'a':
             raise WrongFlagException(args.task[1])
```

### Comparing `dmocker-0.0.1/dmocker/main.py` & `dmocker-0.0.2/dmocker/main.py`

 * *Files identical despite different names*

### Comparing `dmocker-0.0.1/dmocker/src/arguments.py` & `dmocker-0.0.2/dmocker/src/arguments.py`

 * *Files identical despite different names*

### Comparing `dmocker-0.0.1/dmocker/src/container_info.py` & `dmocker-0.0.2/dmocker/src/container_info.py`

 * *Files identical despite different names*

### Comparing `dmocker-0.0.1/dmocker.egg-info/PKG-INFO` & `dmocker-0.0.2/dmocker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmocker
-Version: 0.0.1
+Version: 0.0.2
 Summary: Remote Docker control
 Author-email: strecobyasha <strecobyasha@protonmail.com>
 Project-URL: Homepage, https://github.com/strecobyasha/dmocker
 Project-URL: Issues, https://github.com/strecobyasha/dmocker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dmocker-0.0.1/pyproject.toml` & `dmocker-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dmocker"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="strecobyasha", email="strecobyasha@protonmail.com" },
 ]
 description = "Remote Docker control"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `dmocker-0.0.1/tests/test_arg_parser_container_logs.py` & `dmocker-0.0.2/tests/test_arg_parser_container_logs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """
 Test options to get the list of containers.
 """
 import sys
 import unittest
-from unittest.mock import patch
 
+import dmocker
 from dmocker import router
-from dmocker.exceptions.custom import TooManyServersException, NotEnoughArgsException, LogsNumberException, \
-    LogsFollowException, TooManyParamsException
+from dmocker.exceptions.custom import (LogsFollowException,
+                                       LogsNumberException,
+                                       NotEnoughArgsException,
+                                       TooManyParamsException,
+                                       TooManyServersException)
 
 result = None
 CONTAINER_ID = 'f077a7bcd77f'
 
 
 class MockFetcher:
 
@@ -25,70 +28,62 @@
 
 
 class TestArgParser(unittest.TestCase):
 
     def setUp(self):
         global result
         result = None
+        dmocker.main.Fetcher = MockFetcher
 
-    @patch('dmocker.main.Fetcher', MockFetcher)
     def test_get_logs(self):
         sys.argv = ['local.py', 'server1', '-t', 'logs', CONTAINER_ID]
         router()
         self.assertTrue(result == (CONTAINER_ID, 10, False))
 
-    @patch('dmocker.main.Fetcher', MockFetcher)
     def test_get_logs_number(self):
         sys.argv = ['local.py', 'server1', '-t', 'logs', CONTAINER_ID, '20']
         router()
         self.assertTrue(result == (CONTAINER_ID, 20, False))
 
-    @patch('dmocker.main.Fetcher', MockFetcher)
     def test_get_logs_number_follow(self):
         sys.argv = ['local.py', 'server1', '-t', 'logs', CONTAINER_ID, '20', 'f']
         router()
         self.assertTrue(result == (CONTAINER_ID, 20, True))
 
-    @patch('dmocker.main.Fetcher', MockFetcher)
     def test_get_logs_follow(self):
         sys.argv = ['local.py', 'server1', '-t', 'logs', CONTAINER_ID, 'f']
         router()
         self.assertTrue(result == (CONTAINER_ID, 10, True))
 
-    @patch('dmocker.main.Fetcher', MockFetcher)
     def test_get_logs_many_servers(self):
         servers = ['server1', 'server2']
         sys.argv = ['local.py', *servers, '-t', 'logs']
         with self.assertRaises(TooManyServersException) as context:
             router()
         self.assertTrue(context.exception.args == TooManyServersException(servers).args)
 
-    @patch('dmocker.main.Fetcher', MockFetcher)
     def test_get_logs_missed_container_id(self):
         sys.argv = ['local.py', 'server1', '-t', 'logs']
         with self.assertRaises(NotEnoughArgsException) as context:
             router()
         self.assertTrue(context.exception.args == NotEnoughArgsException().args)
 
-    @patch('dmocker.main.Fetcher', MockFetcher)
     def test_get_logs_number_value_error(self):
         logs_number = '10s'
         sys.argv = ['local.py', 'server1', '-t', 'logs', CONTAINER_ID, logs_number]
         with self.assertRaises(LogsNumberException) as context:
             router()
         self.assertTrue(context.exception.args == LogsNumberException(logs_number).args)
 
-    @patch('dmocker.main.Fetcher', MockFetcher)
     def test_get_logs_follow_value_error(self):
         follow_value = 'true'
         sys.argv = ['local.py', 'server1', '-t', 'logs', CONTAINER_ID, '20', follow_value]
         with self.assertRaises(LogsFollowException) as context:
             router()
         self.assertTrue(context.exception.args == LogsFollowException(follow_value).args)
 
-    @patch('dmocker.main.Fetcher', MockFetcher)
     def test_get_logs_too_many_params(self):
         params = [CONTAINER_ID, '20', 'f', 'another_param']
         sys.argv = ['local.py', 'server1', '-t', 'logs', *params]
         with self.assertRaises(TooManyParamsException) as context:
             router()
         self.assertTrue(context.exception.args == TooManyParamsException(params).args)
```

### Comparing `dmocker-0.0.1/tests/test_arg_parser_containers.py` & `dmocker-0.0.2/tests/test_arg_parser_containers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Test options to get the list of containers.
 """
 import sys
 import unittest
-from unittest.mock import patch
 
+import dmocker
+from dmocker.exceptions.custom import TooManyFlagsException, WrongFlagException
 from dmocker.main import router
-from dmocker.exceptions.custom import WrongFlagException, TooManyFlagsException
 
 result = None
 GET_RUNNING_MSG = 'get running containers'
 GET_ALL_MSG = 'get all containers'
 GET_RUNNING_FILTERED_MSG = 'get running containers filtered by name'
 GET_ALL_FILTERED_MSG = 'get all containers filtered by name'
 
@@ -30,59 +30,52 @@
 
 
 class TestArgParser(unittest.TestCase):
 
     def setUp(self):
         global result
         result = None
+        dmocker.main.Fetcher = MockFetcher
 
-    @patch('dmocker.main.Fetcher', MockFetcher)
     def test_get_running_containers(self):
         sys.argv = ['local.py', 'server1', 'server2']
         router()
         self.assertTrue(result == GET_RUNNING_MSG)
 
-    @patch('dmocker.main.Fetcher', MockFetcher)
     def test_get_running_filtered_containers(self):
         sys.argv = ['local.py', 'server1', 'server2', '-n', 'container_name']
         router()
         self.assertTrue(result == GET_RUNNING_FILTERED_MSG)
 
-    @patch('dmocker.main.Fetcher', MockFetcher)
     def test_get_running_containers_task(self):
         sys.argv = ['local.py', 'server1', 'server2', '-t', 'ps']
         router()
         self.assertTrue(result == GET_RUNNING_MSG)
 
-    @patch('dmocker.main.Fetcher', MockFetcher)
     def test_get_running_containers_filtered_task(self):
         sys.argv = ['local.py', 'server1', 'server2', '-t', 'ps', '-n', 'container_name']
         router()
         self.assertTrue(result == GET_RUNNING_FILTERED_MSG)
 
-    @patch('dmocker.main.Fetcher', MockFetcher)
     def test_get_all_containers(self):
         sys.argv = ['local.py', 'server1', 'server2', '-t', 'ps', 'a']
         router()
         self.assertTrue(result == GET_ALL_MSG)
 
-    @patch('dmocker.main.Fetcher', MockFetcher)
     def test_get_all_containers_filtered(self):
         sys.argv = ['local.py', 'server1', 'server2', '-t', 'ps', 'a', '-n', 'container_name']
         router()
         self.assertTrue(result == GET_ALL_FILTERED_MSG)
 
-    @patch('dmocker.main.Fetcher', MockFetcher)
     def test_get_containers_wrong_flag(self):
         flag = 'b'
         sys.argv = ['local.py', 'server1', 'server2', '-t', 'ps', flag]
         with self.assertRaises(WrongFlagException) as context:
             router()
         self.assertTrue(context.exception.args == WrongFlagException(flag).args)
 
-    @patch('dmocker.main.Fetcher', MockFetcher)
     def test_get_containers_too_many_flags(self):
         flags = ['a', 'b']
         sys.argv = ['local.py', 'server1', 'server2', '-t', 'ps', *flags]
         with self.assertRaises(TooManyFlagsException) as context:
             router()
         self.assertTrue(context.exception.args == TooManyFlagsException(flags).args)
```

