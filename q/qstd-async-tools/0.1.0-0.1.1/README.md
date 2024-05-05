# Comparing `tmp/qstd_async_tools-0.1.0.tar.gz` & `tmp/qstd_async_tools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qstd_async_tools-0.1.0.tar", last modified: Sun Apr  7 17:46:10 2024, max compression
+gzip compressed data, was "qstd_async_tools-0.1.1.tar", last modified: Sun May  5 15:22:11 2024, max compression
```

## Comparing `qstd_async_tools-0.1.0.tar` & `qstd_async_tools-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-07 17:46:10.119601 qstd_async_tools-0.1.0/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1054 2024-03-24 20:15:12.000000 qstd_async_tools-0.1.0/LICENSE
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      331 2024-04-07 17:46:10.119601 qstd_async_tools-0.1.0/PKG-INFO
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       15 2024-04-07 17:45:38.000000 qstd_async_tools-0.1.0/README.md
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-07 17:46:10.119601 qstd_async_tools-0.1.0/qstd_async_tools/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      243 2024-03-30 12:24:10.000000 qstd_async_tools-0.1.0/qstd_async_tools/__init__.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      703 2024-03-31 08:08:21.000000 qstd_async_tools-0.1.0/qstd_async_tools/background.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      934 2024-03-30 11:50:48.000000 qstd_async_tools-0.1.0/qstd_async_tools/call_limit.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2039 2024-03-30 11:50:31.000000 qstd_async_tools-0.1.0/qstd_async_tools/call_limit_time.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      549 2024-03-30 11:52:08.000000 qstd_async_tools-0.1.0/qstd_async_tools/gather.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      449 2024-03-30 12:23:32.000000 qstd_async_tools-0.1.0/qstd_async_tools/shield.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2235 2024-03-31 08:16:14.000000 qstd_async_tools-0.1.0/qstd_async_tools/trace.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-07 17:46:10.119601 qstd_async_tools-0.1.0/qstd_async_tools.egg-info/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      331 2024-04-07 17:46:10.000000 qstd_async_tools-0.1.0/qstd_async_tools.egg-info/PKG-INFO
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      403 2024-04-07 17:46:10.000000 qstd_async_tools-0.1.0/qstd_async_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)        1 2024-04-07 17:46:10.000000 qstd_async_tools-0.1.0/qstd_async_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       17 2024-04-07 17:46:10.000000 qstd_async_tools-0.1.0/qstd_async_tools.egg-info/top_level.txt
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       38 2024-04-07 17:46:10.119601 qstd_async_tools-0.1.0/setup.cfg
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      588 2024-04-07 17:45:49.000000 qstd_async_tools-0.1.0/setup.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-05 15:22:11.306490 qstd_async_tools-0.1.1/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1054 2024-03-24 20:15:12.000000 qstd_async_tools-0.1.1/LICENSE
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      331 2024-05-05 15:22:11.306490 qstd_async_tools-0.1.1/PKG-INFO
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       15 2024-04-07 17:45:38.000000 qstd_async_tools-0.1.1/README.md
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-05 15:22:11.306490 qstd_async_tools-0.1.1/qstd_async_tools/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      243 2024-03-30 12:24:10.000000 qstd_async_tools-0.1.1/qstd_async_tools/__init__.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      703 2024-03-31 08:08:21.000000 qstd_async_tools-0.1.1/qstd_async_tools/background.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      934 2024-03-30 11:50:48.000000 qstd_async_tools-0.1.1/qstd_async_tools/call_limit.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2039 2024-03-30 11:50:31.000000 qstd_async_tools-0.1.1/qstd_async_tools/call_limit_time.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      519 2024-05-05 15:20:51.000000 qstd_async_tools-0.1.1/qstd_async_tools/gather.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      449 2024-03-30 12:23:32.000000 qstd_async_tools-0.1.1/qstd_async_tools/shield.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2235 2024-03-31 08:16:14.000000 qstd_async_tools-0.1.1/qstd_async_tools/trace.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-05 15:22:11.306490 qstd_async_tools-0.1.1/qstd_async_tools.egg-info/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      331 2024-05-05 15:22:11.000000 qstd_async_tools-0.1.1/qstd_async_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      403 2024-05-05 15:22:11.000000 qstd_async_tools-0.1.1/qstd_async_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)        1 2024-05-05 15:22:11.000000 qstd_async_tools-0.1.1/qstd_async_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       17 2024-05-05 15:22:11.000000 qstd_async_tools-0.1.1/qstd_async_tools.egg-info/top_level.txt
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       38 2024-05-05 15:22:11.306490 qstd_async_tools-0.1.1/setup.cfg
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      588 2024-05-05 15:21:44.000000 qstd_async_tools-0.1.1/setup.py
```

### Comparing `qstd_async_tools-0.1.0/LICENSE` & `qstd_async_tools-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qstd_async_tools-0.1.0/qstd_async_tools/background.py` & `qstd_async_tools-0.1.1/qstd_async_tools/background.py`

 * *Files identical despite different names*

### Comparing `qstd_async_tools-0.1.0/qstd_async_tools/call_limit.py` & `qstd_async_tools-0.1.1/qstd_async_tools/call_limit.py`

 * *Files identical despite different names*

### Comparing `qstd_async_tools-0.1.0/qstd_async_tools/call_limit_time.py` & `qstd_async_tools-0.1.1/qstd_async_tools/call_limit_time.py`

 * *Files identical despite different names*

### Comparing `qstd_async_tools-0.1.0/qstd_async_tools/gather.py` & `qstd_async_tools-0.1.1/qstd_async_tools/gather.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,13 @@
 async def _wrapper(coroutine: typing.Coroutine, trace_ids: typing.List[str]):
     if trace_ids:
         add_trace_id(trace_ids)
     with trace_id():
         return await coroutine
 
 
-def gather(*coroutines: typing.Coroutine, loop=None, return_exceptions=False):
+def gather(*coroutines: typing.Coroutine, return_exceptions=False):
     trace_ids = get_trace_ids()
     return asyncio.gather(
         *[_wrapper(coroutine, trace_ids) for coroutine in coroutines],
-        loop=loop,
         return_exceptions=return_exceptions
     )
```

### Comparing `qstd_async_tools-0.1.0/qstd_async_tools/trace.py` & `qstd_async_tools-0.1.1/qstd_async_tools/trace.py`

 * *Files identical despite different names*

### Comparing `qstd_async_tools-0.1.0/setup.py` & `qstd_async_tools-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='qstd_async_tools',
-    version='0.1.0',
+    version='0.1.1',
     author='QuisEgoSum',
     author_email='subbotin.evdokim@gmail.com',
     description='Async tools',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/QuisEgoSum/qstd-async-tools',
     packages=find_packages(exclude=['tmp', 'example', '*test*']),
```

