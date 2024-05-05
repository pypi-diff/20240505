# Comparing `tmp/sponge-0.0.7.tar.gz` & `tmp/sponge-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sponge-0.0.7.tar", last modified: Sat Apr 20 09:39:21 2024, max compression
+gzip compressed data, was "sponge-0.0.8.tar", last modified: Sun May  5 03:38:31 2024, max compression
```

## Comparing `sponge-0.0.7.tar` & `sponge-0.0.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 william    (502) staff       (20)        0 2024-04-20 09:39:21.390813 sponge-0.0.7/
--rw-r--r--   0 william    (502) staff       (20)    35147 2024-04-19 04:29:01.000000 sponge-0.0.7/LICENSE
--rw-r--r--   0 william    (502) staff       (20)     2189 2024-04-20 09:39:21.390595 sponge-0.0.7/PKG-INFO
--rw-r--r--   0 william    (502) staff       (20)     1275 2024-04-19 04:29:01.000000 sponge-0.0.7/README.rst
--rw-r--r--   0 william    (502) staff       (20)       38 2024-04-20 09:39:21.390877 sponge-0.0.7/setup.cfg
--rw-r--r--   0 william    (502) staff       (20)     1348 2024-04-19 04:29:01.000000 sponge-0.0.7/setup.py
-drwxr-xr-x   0 william    (502) staff       (20)        0 2024-04-20 09:39:21.385362 sponge-0.0.7/sponge/
--rw-r--r--   0 william    (502) staff       (20)      324 2024-04-20 09:39:05.000000 sponge-0.0.7/sponge/__init__.py
-drwxr-xr-x   0 william    (502) staff       (20)        0 2024-04-20 09:39:21.388461 sponge-0.0.7/sponge/drivers/
--rw-r--r--   0 william    (502) staff       (20)      172 2024-04-19 04:29:01.000000 sponge-0.0.7/sponge/drivers/__init__.py
--rw-r--r--   0 william    (502) staff       (20)      624 2024-04-19 04:29:01.000000 sponge-0.0.7/sponge/drivers/driver.py
--rw-r--r--   0 william    (502) staff       (20)     1393 2024-04-19 04:29:01.000000 sponge-0.0.7/sponge/drivers/memory.py
--rw-r--r--   0 william    (502) staff       (20)     1252 2024-04-19 04:29:01.000000 sponge-0.0.7/sponge/drivers/redis.py
--rw-r--r--   0 william    (502) staff       (20)     1842 2024-04-19 05:45:58.000000 sponge-0.0.7/sponge/drivers/sqlite.py
--rw-r--r--   0 william    (502) staff       (20)     1549 2024-04-19 05:44:20.000000 sponge-0.0.7/sponge/manager.py
-drwxr-xr-x   0 william    (502) staff       (20)        0 2024-04-20 09:39:21.386797 sponge-0.0.7/sponge.egg-info/
--rw-r--r--   0 william    (502) staff       (20)     2189 2024-04-20 09:39:21.000000 sponge-0.0.7/sponge.egg-info/PKG-INFO
--rw-r--r--   0 william    (502) staff       (20)      435 2024-04-20 09:39:21.000000 sponge-0.0.7/sponge.egg-info/SOURCES.txt
--rw-r--r--   0 william    (502) staff       (20)        1 2024-04-20 09:39:21.000000 sponge-0.0.7/sponge.egg-info/dependency_links.txt
--rw-r--r--   0 william    (502) staff       (20)       14 2024-04-20 09:39:21.000000 sponge-0.0.7/sponge.egg-info/requires.txt
--rw-r--r--   0 william    (502) staff       (20)       13 2024-04-20 09:39:21.000000 sponge-0.0.7/sponge.egg-info/top_level.txt
-drwxr-xr-x   0 william    (502) staff       (20)        0 2024-04-20 09:39:21.390103 sponge-0.0.7/tests/
--rw-r--r--   0 william    (502) staff       (20)      172 2024-04-19 04:29:01.000000 sponge-0.0.7/tests/__init__.py
--rw-r--r--   0 william    (502) staff       (20)     2137 2024-04-19 04:29:01.000000 sponge-0.0.7/tests/driver.py
--rw-r--r--   0 william    (502) staff       (20)      380 2024-04-19 04:29:01.000000 sponge-0.0.7/tests/test_memory.py
--rw-r--r--   0 william    (502) staff       (20)      379 2024-04-19 04:29:01.000000 sponge-0.0.7/tests/test_redis.py
--rw-r--r--   0 william    (502) staff       (20)     2291 2024-04-19 04:51:57.000000 sponge-0.0.7/tests/test_sqlite.py
+drwxr-xr-x   0 william    (502) staff       (20)        0 2024-05-05 03:38:31.179429 sponge-0.0.8/
+-rw-r--r--   0 william    (502) staff       (20)    35147 2024-04-19 04:29:01.000000 sponge-0.0.8/LICENSE
+-rw-r--r--   0 william    (502) staff       (20)     2189 2024-05-05 03:38:31.179166 sponge-0.0.8/PKG-INFO
+-rw-r--r--   0 william    (502) staff       (20)     1275 2024-04-19 04:29:01.000000 sponge-0.0.8/README.rst
+-rw-r--r--   0 william    (502) staff       (20)       38 2024-05-05 03:38:31.179495 sponge-0.0.8/setup.cfg
+-rw-r--r--   0 william    (502) staff       (20)     1348 2024-04-19 04:29:01.000000 sponge-0.0.8/setup.py
+drwxr-xr-x   0 william    (502) staff       (20)        0 2024-05-05 03:38:31.161203 sponge-0.0.8/sponge/
+-rw-r--r--   0 william    (502) staff       (20)      324 2024-05-05 03:36:31.000000 sponge-0.0.8/sponge/__init__.py
+drwxr-xr-x   0 william    (502) staff       (20)        0 2024-05-05 03:38:31.176082 sponge-0.0.8/sponge/drivers/
+-rw-r--r--   0 william    (502) staff       (20)      172 2024-04-19 04:29:01.000000 sponge-0.0.8/sponge/drivers/__init__.py
+-rw-r--r--   0 william    (502) staff       (20)      624 2024-04-19 04:29:01.000000 sponge-0.0.8/sponge/drivers/driver.py
+-rw-r--r--   0 william    (502) staff       (20)     1393 2024-04-19 04:29:01.000000 sponge-0.0.8/sponge/drivers/memory.py
+-rw-r--r--   0 william    (502) staff       (20)     1252 2024-04-19 04:29:01.000000 sponge-0.0.8/sponge/drivers/redis.py
+-rw-r--r--   0 william    (502) staff       (20)     1842 2024-04-19 05:45:58.000000 sponge-0.0.8/sponge/drivers/sqlite.py
+-rw-r--r--   0 william    (502) staff       (20)     1610 2024-05-05 03:35:45.000000 sponge-0.0.8/sponge/manager.py
+drwxr-xr-x   0 william    (502) staff       (20)        0 2024-05-05 03:38:31.162868 sponge-0.0.8/sponge.egg-info/
+-rw-r--r--   0 william    (502) staff       (20)     2189 2024-05-05 03:38:31.000000 sponge-0.0.8/sponge.egg-info/PKG-INFO
+-rw-r--r--   0 william    (502) staff       (20)      435 2024-05-05 03:38:31.000000 sponge-0.0.8/sponge.egg-info/SOURCES.txt
+-rw-r--r--   0 william    (502) staff       (20)        1 2024-05-05 03:38:31.000000 sponge-0.0.8/sponge.egg-info/dependency_links.txt
+-rw-r--r--   0 william    (502) staff       (20)       14 2024-05-05 03:38:31.000000 sponge-0.0.8/sponge.egg-info/requires.txt
+-rw-r--r--   0 william    (502) staff       (20)       13 2024-05-05 03:38:31.000000 sponge-0.0.8/sponge.egg-info/top_level.txt
+drwxr-xr-x   0 william    (502) staff       (20)        0 2024-05-05 03:38:31.178601 sponge-0.0.8/tests/
+-rw-r--r--   0 william    (502) staff       (20)      172 2024-04-19 04:29:01.000000 sponge-0.0.8/tests/__init__.py
+-rw-r--r--   0 william    (502) staff       (20)     2137 2024-04-19 04:29:01.000000 sponge-0.0.8/tests/driver.py
+-rw-r--r--   0 william    (502) staff       (20)      380 2024-04-19 04:29:01.000000 sponge-0.0.8/tests/test_memory.py
+-rw-r--r--   0 william    (502) staff       (20)      379 2024-04-19 04:29:01.000000 sponge-0.0.8/tests/test_redis.py
+-rw-r--r--   0 william    (502) staff       (20)     2291 2024-04-19 04:51:57.000000 sponge-0.0.8/tests/test_sqlite.py
```

### Comparing `sponge-0.0.7/LICENSE` & `sponge-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sponge-0.0.7/PKG-INFO` & `sponge-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sponge
-Version: 0.0.7
+Version: 0.0.8
 Summary: An elegant cache library for python
 Home-page: https://github.com/IamBusy/sponge
 Author: William Wei
 Author-email: 1342247033@qq.com
 Maintainer: William Wei
 Maintainer-email: 1342247033@qq.com
 License: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `sponge-0.0.7/README.rst` & `sponge-0.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `sponge-0.0.7/setup.py` & `sponge-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `sponge-0.0.7/sponge/drivers/driver.py` & `sponge-0.0.8/sponge/drivers/driver.py`

 * *Files identical despite different names*

### Comparing `sponge-0.0.7/sponge/drivers/memory.py` & `sponge-0.0.8/sponge/drivers/memory.py`

 * *Files identical despite different names*

### Comparing `sponge-0.0.7/sponge/drivers/redis.py` & `sponge-0.0.8/sponge/drivers/redis.py`

 * *Files identical despite different names*

### Comparing `sponge-0.0.7/sponge/drivers/sqlite.py` & `sponge-0.0.8/sponge/drivers/sqlite.py`

 * *Files identical despite different names*

### Comparing `sponge-0.0.7/sponge/manager.py` & `sponge-0.0.8/sponge/manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 @author: william
 @contact: 1342247033@qq.com
 @site: http://www.xiaolewei.com
 @file: manager.py
 @time: 22/05/2018 16:03
 """
 import importlib
+from sponge.drivers.driver import Driver
 
 
 class CacheManager(object):
     _supported_stores = ('redis', 'memory', 'sqlite')
 
     def __init__(self, cfg):
         self._cfg = cfg
@@ -24,28 +25,28 @@
                 self._cfg['default'] = keys[0]
             else:
                 raise Exception('None config is not allowed for CacheManager')
         else:
             self._resolve(cfg['default'])
             self._stores['default'] = self._stores[cfg['default']]
 
-    def store(self, name='default'):
+    def store(self, name='default') -> Driver:
         '''
         :param name:
         :return: sponge.Driver
         '''
         if name in self._stores:
             return self._stores[name]
         elif name in self._supported_stores:
             if name in self._cfg:
                 return self._resolve(name)
         else:
             raise Exception('Not supported driver [%s]' % name)
 
-    def _resolve(self, name):
+    def _resolve(self, name) -> Driver:
         '''
         :param name:
         :param cfg:
         :return: sponge.Driver
         '''
         if name not in self._cfg:
             raise Exception('Empty config for %s driver' % name)
```

### Comparing `sponge-0.0.7/sponge.egg-info/PKG-INFO` & `sponge-0.0.8/sponge.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sponge
-Version: 0.0.7
+Version: 0.0.8
 Summary: An elegant cache library for python
 Home-page: https://github.com/IamBusy/sponge
 Author: William Wei
 Author-email: 1342247033@qq.com
 Maintainer: William Wei
 Maintainer-email: 1342247033@qq.com
 License: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `sponge-0.0.7/tests/driver.py` & `sponge-0.0.8/tests/driver.py`

 * *Files identical despite different names*

### Comparing `sponge-0.0.7/tests/test_sqlite.py` & `sponge-0.0.8/tests/test_sqlite.py`

 * *Files identical despite different names*

