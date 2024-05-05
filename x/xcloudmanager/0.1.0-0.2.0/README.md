# Comparing `tmp/xcloudmanager-0.1.0.tar.gz` & `tmp/xcloudmanager-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcloudmanager-0.1.0.tar", last modified: Sat May  4 10:48:40 2024, max compression
+gzip compressed data, was "xcloudmanager-0.2.0.tar", last modified: Sat May  4 11:29:41 2024, max compression
```

## Comparing `xcloudmanager-0.1.0.tar` & `xcloudmanager-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 10:48:40.528251 xcloudmanager-0.1.0/
--rw-rw-rw-   0        0        0       36 2024-05-04 06:49:01.000000 xcloudmanager-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      468 2024-05-04 10:48:40.527252 xcloudmanager-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      134 2024-05-04 06:57:04.000000 xcloudmanager-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-04 10:48:40.529252 xcloudmanager-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      685 2024-05-04 10:45:34.000000 xcloudmanager-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:48:40.461519 xcloudmanager-0.1.0/xcloudmanager/
--rw-rw-rw-   0        0        0      141 2024-05-04 06:22:56.000000 xcloudmanager-0.1.0/xcloudmanager/__init__.py
--rw-rw-rw-   0        0        0      761 2024-04-16 17:50:26.000000 xcloudmanager-0.1.0/xcloudmanager/readscripts.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:48:40.523254 xcloudmanager-0.1.0/xcloudmanager/resources/
--rw-rw-rw-   0        0        0  1358472 2021-10-15 08:05:30.000000 xcloudmanager-0.1.0/xcloudmanager/resources/XCloudJDBC-2.10.6.7.jar
--rw-rw-rw-   0        0        0   275539 2021-10-15 08:05:26.000000 xcloudmanager-0.1.0/xcloudmanager/resources/XCloudJDBC_SP_Procedure_Parser-0.1.3.jar
--rw-rw-rw-   0        0        0   227712 2019-07-16 09:51:20.000000 xcloudmanager-0.1.0/xcloudmanager/resources/libthrift-0.9.2.jar
--rw-rw-rw-   0        0        0   489884 2019-07-16 09:51:20.000000 xcloudmanager-0.1.0/xcloudmanager/resources/log4j-1.2.17.jar
--rw-rw-rw-   0        0        0   236880 2019-07-16 09:51:20.000000 xcloudmanager-0.1.0/xcloudmanager/resources/lz4-1.3.0.jar
--rw-rw-rw-   0        0        0    26084 2018-10-10 07:16:32.000000 xcloudmanager-0.1.0/xcloudmanager/resources/slf4j-api-1.7.5.jar
--rw-rw-rw-   0        0        0     8869 2021-10-15 08:05:28.000000 xcloudmanager-0.1.0/xcloudmanager/resources/slf4j-log4j12-1.7.5.jar
--rw-rw-rw-   0        0        0    10680 2019-09-11 10:52:28.000000 xcloudmanager-0.1.0/xcloudmanager/resources/slf4j-simple-1.7.5.jar
--rw-rw-rw-   0        0        0      107 2024-05-04 08:36:14.000000 xcloudmanager-0.1.0/xcloudmanager/test.py
--rw-rw-rw-   0        0        0     8741 2024-05-04 08:38:09.000000 xcloudmanager-0.1.0/xcloudmanager/xcloudmanager.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:48:40.482054 xcloudmanager-0.1.0/xcloudmanager.egg-info/
--rw-rw-rw-   0        0        0      468 2024-05-04 10:48:39.000000 xcloudmanager-0.1.0/xcloudmanager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      697 2024-05-04 10:48:40.000000 xcloudmanager-0.1.0/xcloudmanager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 10:48:39.000000 xcloudmanager-0.1.0/xcloudmanager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-04 10:48:39.000000 xcloudmanager-0.1.0/xcloudmanager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-04 10:48:39.000000 xcloudmanager-0.1.0/xcloudmanager.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 11:29:41.625442 xcloudmanager-0.2.0/
+-rw-rw-rw-   0        0        0       36 2024-05-04 06:49:01.000000 xcloudmanager-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      468 2024-05-04 11:29:41.622839 xcloudmanager-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      134 2024-05-04 06:57:04.000000 xcloudmanager-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-04 11:29:41.625992 xcloudmanager-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      685 2024-05-04 11:28:47.000000 xcloudmanager-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 11:29:41.517274 xcloudmanager-0.2.0/xcloudmanager/
+-rw-rw-rw-   0        0        0      541 2024-05-04 11:28:36.000000 xcloudmanager-0.2.0/xcloudmanager/__init__.py
+-rw-rw-rw-   0        0        0      761 2024-04-16 17:50:26.000000 xcloudmanager-0.2.0/xcloudmanager/readscripts.py
+drwxrwxrwx   0        0        0        0 2024-05-04 11:29:41.616400 xcloudmanager-0.2.0/xcloudmanager/resources/
+-rw-rw-rw-   0        0        0  1358472 2021-10-15 08:05:30.000000 xcloudmanager-0.2.0/xcloudmanager/resources/XCloudJDBC-2.10.6.7.jar
+-rw-rw-rw-   0        0        0   275539 2021-10-15 08:05:26.000000 xcloudmanager-0.2.0/xcloudmanager/resources/XCloudJDBC_SP_Procedure_Parser-0.1.3.jar
+-rw-rw-rw-   0        0        0   227712 2019-07-16 09:51:20.000000 xcloudmanager-0.2.0/xcloudmanager/resources/libthrift-0.9.2.jar
+-rw-rw-rw-   0        0        0   489884 2019-07-16 09:51:20.000000 xcloudmanager-0.2.0/xcloudmanager/resources/log4j-1.2.17.jar
+-rw-rw-rw-   0        0        0   236880 2019-07-16 09:51:20.000000 xcloudmanager-0.2.0/xcloudmanager/resources/lz4-1.3.0.jar
+-rw-rw-rw-   0        0        0    26084 2018-10-10 07:16:32.000000 xcloudmanager-0.2.0/xcloudmanager/resources/slf4j-api-1.7.5.jar
+-rw-rw-rw-   0        0        0     8869 2021-10-15 08:05:28.000000 xcloudmanager-0.2.0/xcloudmanager/resources/slf4j-log4j12-1.7.5.jar
+-rw-rw-rw-   0        0        0    10680 2019-09-11 10:52:28.000000 xcloudmanager-0.2.0/xcloudmanager/resources/slf4j-simple-1.7.5.jar
+-rw-rw-rw-   0        0        0      107 2024-05-04 08:36:14.000000 xcloudmanager-0.2.0/xcloudmanager/test.py
+-rw-rw-rw-   0        0        0     8394 2024-05-04 11:28:12.000000 xcloudmanager-0.2.0/xcloudmanager/xcloudmanager.py
+drwxrwxrwx   0        0        0        0 2024-05-04 11:29:41.553772 xcloudmanager-0.2.0/xcloudmanager.egg-info/
+-rw-rw-rw-   0        0        0      468 2024-05-04 11:29:39.000000 xcloudmanager-0.2.0/xcloudmanager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      697 2024-05-04 11:29:41.000000 xcloudmanager-0.2.0/xcloudmanager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 11:29:39.000000 xcloudmanager-0.2.0/xcloudmanager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-04 11:29:40.000000 xcloudmanager-0.2.0/xcloudmanager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-04 11:29:40.000000 xcloudmanager-0.2.0/xcloudmanager.egg-info/top_level.txt
```

### Comparing `xcloudmanager-0.1.0/setup.py` & `xcloudmanager-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xcloudmanager',
-    version='0.1.0',
+    version='0.2.0',
     packages=find_packages(),
     package_data={
         'xcloudmanager': ['resources/*.jar'],
     },
     include_package_data=True,
     install_requires=[
         'JayDeBeApi==1.2.3',  # 添加你的依赖项
```

### Comparing `xcloudmanager-0.1.0/xcloudmanager/readscripts.py` & `xcloudmanager-0.2.0/xcloudmanager/readscripts.py`

 * *Files identical despite different names*

### Comparing `xcloudmanager-0.1.0/xcloudmanager/resources/XCloudJDBC-2.10.6.7.jar` & `xcloudmanager-0.2.0/xcloudmanager/resources/XCloudJDBC-2.10.6.7.jar`

 * *Files identical despite different names*

### Comparing `xcloudmanager-0.1.0/xcloudmanager/resources/XCloudJDBC_SP_Procedure_Parser-0.1.3.jar` & `xcloudmanager-0.2.0/xcloudmanager/resources/XCloudJDBC_SP_Procedure_Parser-0.1.3.jar`

 * *Files identical despite different names*

### Comparing `xcloudmanager-0.1.0/xcloudmanager/resources/libthrift-0.9.2.jar` & `xcloudmanager-0.2.0/xcloudmanager/resources/libthrift-0.9.2.jar`

 * *Files identical despite different names*

### Comparing `xcloudmanager-0.1.0/xcloudmanager/resources/log4j-1.2.17.jar` & `xcloudmanager-0.2.0/xcloudmanager/resources/log4j-1.2.17.jar`

 * *Files identical despite different names*

### Comparing `xcloudmanager-0.1.0/xcloudmanager/resources/lz4-1.3.0.jar` & `xcloudmanager-0.2.0/xcloudmanager/resources/lz4-1.3.0.jar`

 * *Files identical despite different names*

### Comparing `xcloudmanager-0.1.0/xcloudmanager/resources/slf4j-api-1.7.5.jar` & `xcloudmanager-0.2.0/xcloudmanager/resources/slf4j-api-1.7.5.jar`

 * *Files identical despite different names*

### Comparing `xcloudmanager-0.1.0/xcloudmanager/resources/slf4j-log4j12-1.7.5.jar` & `xcloudmanager-0.2.0/xcloudmanager/resources/slf4j-log4j12-1.7.5.jar`

 * *Files identical despite different names*

### Comparing `xcloudmanager-0.1.0/xcloudmanager/resources/slf4j-simple-1.7.5.jar` & `xcloudmanager-0.2.0/xcloudmanager/resources/slf4j-simple-1.7.5.jar`

 * *Files identical despite different names*

### Comparing `xcloudmanager-0.1.0/xcloudmanager/xcloudmanager.py` & `xcloudmanager-0.2.0/xcloudmanager/xcloudmanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from concurrent.futures import ProcessPoolExecutor, as_completed
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from threading import Semaphore
 import jpype
 import jpype.imports
 from jpype.types import *
 import os
+from . import JAR_FILES
 
 class DatabaseClient:
     def __init__(self, host, username, password, max_cursors=10,if_header_included = False):
         self.host = host
         self.username = username
         self.password = password
         self.connection = self.get_connection()
@@ -36,22 +37,15 @@
     def get_connection(self):
         try:
             """
             建立与数据库的连接
             """
             driver = 'com.bonc.xcloud.jdbc.XCloudDriver'
             url = f'jdbc:xcloud:@{self.host}/SERVER_DATA?connectRetry=3&socketTimeOut=43200000&connectDirect=true&buffMemory=33554432'
-            jarFile = ['XCloudJDBC-2.10.6.7.jar','slf4j-api-1.7.5.jar','slf4j-log4j12-1.7.5.jar','slf4j-simple-1.7.5.jar','log4j-1.2.17.jar','libthrift-0.9.2.jar',
-            'XCloudJDBC_SP_Procedure_Parser-0.1.3.jar'
-            ,'lz4-1.3.0.jar'
-            ]
-
-            jarFile = [os.path.join('.','resources',jar_path) for jar_path in jarFile]
-                
-            conn = jaydebeapi.connect(jclassname=driver, url=url, driver_args=[self.username, self.password], jars=jarFile)
+            conn = jaydebeapi.connect(jclassname=driver, url=url, driver_args=[self.username, self.password], jars=JAR_FILES)
             return conn
         except jaydebeapi.DatabaseError as e:
             print(f'the connection was not consistent ,because of {e}')
             raise
 
 
     def execute_query(self, query):
```

### Comparing `xcloudmanager-0.1.0/xcloudmanager.egg-info/SOURCES.txt` & `xcloudmanager-0.2.0/xcloudmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

