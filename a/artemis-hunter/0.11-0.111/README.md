# Comparing `tmp/artemis_hunter-0.11-py3-none-any.whl.zip` & `tmp/artemis_hunter-0.111-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,7 @@
-Zip file size: 6612 bytes, number of entries: 6
--rwxr-xr-x  2.0 unx    17731 b- defN 24-May-05 05:46 artemis_hunter-0.11.data/scripts/main.py
--rwxrwxrwx  2.0 unx     1069 b- defN 24-May-05 05:46 artemis_hunter-0.11.dist-info/LICENSE
--rw-r--r--  2.0 unx      686 b- defN 24-May-05 05:46 artemis_hunter-0.11.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-05 05:46 artemis_hunter-0.11.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-May-05 05:46 artemis_hunter-0.11.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      512 b- defN 24-May-05 05:46 artemis_hunter-0.11.dist-info/RECORD
-6 files, 20091 bytes uncompressed, 5676 bytes compressed:  71.7%
+Zip file size: 2151 bytes, number of entries: 5
+-rwxrwxrwx  2.0 unx     1069 b- defN 24-May-05 13:37 artemis_hunter-0.111.dist-info/LICENSE
+-rw-r--r--  2.0 unx      687 b- defN 24-May-05 13:37 artemis_hunter-0.111.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-05 13:37 artemis_hunter-0.111.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-May-05 13:37 artemis_hunter-0.111.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      419 b- defN 24-May-05 13:37 artemis_hunter-0.111.dist-info/RECORD
+5 files, 2268 bytes uncompressed, 1361 bytes compressed:  40.0%
```

## zipnote {}

```diff
@@ -1,19 +1,16 @@
-Filename: artemis_hunter-0.11.data/scripts/main.py
+Filename: artemis_hunter-0.111.dist-info/LICENSE
 Comment: 
 
-Filename: artemis_hunter-0.11.dist-info/LICENSE
+Filename: artemis_hunter-0.111.dist-info/METADATA
 Comment: 
 
-Filename: artemis_hunter-0.11.dist-info/METADATA
+Filename: artemis_hunter-0.111.dist-info/WHEEL
 Comment: 
 
-Filename: artemis_hunter-0.11.dist-info/WHEEL
+Filename: artemis_hunter-0.111.dist-info/top_level.txt
 Comment: 
 
-Filename: artemis_hunter-0.11.dist-info/top_level.txt
-Comment: 
-
-Filename: artemis_hunter-0.11.dist-info/RECORD
+Filename: artemis_hunter-0.111.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `artemis_hunter-0.11.dist-info/LICENSE` & `artemis_hunter-0.111.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `artemis_hunter-0.11.dist-info/METADATA` & `artemis_hunter-0.111.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artemis-hunter
-Version: 0.11
+Version: 0.111
 Summary: This package does automated vulnerability enumeration and recommends exploits
 Home-page: https://github.com/sudouser2010/artemis
 Author: Hadron Davinci
 Project-URL: Bug Tracker, https://github.com/sudouser2010/artemis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

