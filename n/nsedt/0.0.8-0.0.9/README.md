# Comparing `tmp/nsedt-0.0.8.tar.gz` & `tmp/nsedt-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsedt-0.0.8.tar", last modified: Sat Sep 16 23:44:55 2023, max compression
+gzip compressed data, was "nsedt-0.0.9.tar", last modified: Sun Sep 17 00:14:10 2023, max compression
```

## Comparing `nsedt-0.0.8.tar` & `nsedt-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-16 23:44:55.089712 nsedt-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-09-16 23:44:43.000000 nsedt-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5456 2023-09-16 23:44:55.089712 nsedt-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2023-09-16 23:44:43.000000 nsedt-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-16 23:44:55.089712 nsedt-0.0.8/nsedt/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2023-09-16 23:44:43.000000 nsedt-0.0.8/nsedt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7290 2023-09-16 23:44:43.000000 nsedt-0.0.8/nsedt/equity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2023-09-16 23:44:43.000000 nsedt-0.0.8/nsedt/indices.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-16 23:44:55.089712 nsedt-0.0.8/nsedt/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-16 23:44:43.000000 nsedt-0.0.8/nsedt/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2023-09-16 23:44:43.000000 nsedt-0.0.8/nsedt/resources/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-16 23:44:55.089712 nsedt-0.0.8/nsedt/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2023-09-16 23:44:43.000000 nsedt-0.0.8/nsedt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2023-09-16 23:44:43.000000 nsedt-0.0.8/nsedt/utils/data_format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-16 23:44:55.089712 nsedt-0.0.8/nsedt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5456 2023-09-16 23:44:55.000000 nsedt-0.0.8/nsedt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      339 2023-09-16 23:44:55.000000 nsedt-0.0.8/nsedt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-16 23:44:55.000000 nsedt-0.0.8/nsedt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-09-16 23:44:55.000000 nsedt-0.0.8/nsedt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-09-16 23:44:55.000000 nsedt-0.0.8/nsedt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-09-16 23:44:55.089712 nsedt-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      898 2023-09-16 23:44:43.000000 nsedt-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 00:14:10.679097 nsedt-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-09-17 00:14:01.000000 nsedt-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5456 2023-09-17 00:14:10.679097 nsedt-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2023-09-17 00:14:01.000000 nsedt-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 00:14:10.675097 nsedt-0.0.9/nsedt/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2023-09-17 00:14:01.000000 nsedt-0.0.9/nsedt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2023-09-17 00:14:01.000000 nsedt-0.0.9/nsedt/equity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2023-09-17 00:14:01.000000 nsedt-0.0.9/nsedt/indices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 00:14:10.675097 nsedt-0.0.9/nsedt/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-17 00:14:01.000000 nsedt-0.0.9/nsedt/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2023-09-17 00:14:01.000000 nsedt-0.0.9/nsedt/resources/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 00:14:10.679097 nsedt-0.0.9/nsedt/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2023-09-17 00:14:01.000000 nsedt-0.0.9/nsedt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2023-09-17 00:14:01.000000 nsedt-0.0.9/nsedt/utils/data_format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 00:14:10.675097 nsedt-0.0.9/nsedt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5456 2023-09-17 00:14:10.000000 nsedt-0.0.9/nsedt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2023-09-17 00:14:10.000000 nsedt-0.0.9/nsedt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-17 00:14:10.000000 nsedt-0.0.9/nsedt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2023-09-17 00:14:10.000000 nsedt-0.0.9/nsedt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2023-09-17 00:14:10.000000 nsedt-0.0.9/nsedt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2023-09-17 00:14:10.679097 nsedt-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2023-09-17 00:14:01.000000 nsedt-0.0.9/setup.py
```

### Comparing `nsedt-0.0.8/LICENSE` & `nsedt-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nsedt-0.0.8/PKG-INFO` & `nsedt-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsedt
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library to collect NSE data in pandas dataframe
 Home-page: https://github.com/pratik141/nsedt
 Author: Pratik Anand
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nsedt-0.0.8/README.md` & `nsedt-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `nsedt-0.0.8/nsedt/equity.py` & `nsedt-0.0.9/nsedt/equity.py`

 * *Files identical despite different names*

### Comparing `nsedt-0.0.8/nsedt/indices.py` & `nsedt-0.0.9/nsedt/indices.py`

 * *Files identical despite different names*

### Comparing `nsedt-0.0.8/nsedt/resources/constants.py` & `nsedt-0.0.9/nsedt/resources/constants.py`

 * *Files identical despite different names*

### Comparing `nsedt-0.0.8/nsedt/utils/__init__.py` & `nsedt-0.0.9/nsedt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nsedt-0.0.8/nsedt/utils/data_format.py` & `nsedt-0.0.9/nsedt/utils/data_format.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,20 +76,21 @@
                 "EOD_CLOSE_INDEX_VAL": "Close Price",
                 "EOD_LOW_INDEX_VAL": "Low Price",
                 "EOD_TIMESTAMP": "Date",
             }
         )
     )
 
-    data_turnover_df = (
-        pd.DataFrame(data_json["data"]["indexTurnoverRecords"])
-        .drop(columns=["_id", "HIT_INDEX_NAME_UPPER", "HIT_TIMESTAMP"])
-        .rename(
-            columns={
-                "HIT_TRADED_QTY": "Total Traded Quantity",
-                "HIT_TURN_OVER": "Total Traded Value",
-                "TIMESTAMP": "Date",
-            }
-        )
-    )
-
-    return pd.merge(data_close_df, data_turnover_df, on="Date", how="inner")
+    ## Mismatch values
+    # data_turnover_df = (
+    #     pd.DataFrame(d["data"]["indexTurnoverRecords"])
+    #     .drop(columns=["_id", "HIT_INDEX_NAME_UPPER", "HIT_TIMESTAMP"])
+    #     .rename(
+    #         columns={
+    #             "HIT_TRADED_QTY": "Total Traded Quantity",
+    #             "HIT_TURN_OVER": "Total Traded Value",
+    #             "TIMESTAMP": "Date",
+    #         }
+    #     )
+    # )
+    return data_close_df
+    # return pd.merge(data_close_df, data_turnover_df, on="Date", how="inner")
```

### Comparing `nsedt-0.0.8/nsedt.egg-info/PKG-INFO` & `nsedt-0.0.9/nsedt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsedt
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library to collect NSE data in pandas dataframe
 Home-page: https://github.com/pratik141/nsedt
 Author: Pratik Anand
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

