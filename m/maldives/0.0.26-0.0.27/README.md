# Comparing `tmp/maldives-0.0.26.tar.gz` & `tmp/maldives-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maldives-0.0.26.tar", last modified: Thu Mar 21 20:49:57 2024, max compression
+gzip compressed data, was "maldives-0.0.27.tar", last modified: Sun May  5 04:38:21 2024, max compression
```

## Comparing `maldives-0.0.26.tar` & `maldives-0.0.27.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 20:49:57.774482 maldives-0.0.26/
--rw-rw-rw-   0        0        0     1063 2023-11-21 22:45:27.000000 maldives-0.0.26/LICENSE
--rw-rw-rw-   0        0        0      869 2024-03-21 20:49:57.770957 maldives-0.0.26/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-11-21 22:32:31.000000 maldives-0.0.26/README.md
--rw-rw-rw-   0        0        0      878 2024-03-09 00:55:35.000000 maldives-0.0.26/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-21 20:49:57.775030 maldives-0.0.26/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-21 20:49:57.608750 maldives-0.0.26/src/
-drwxrwxrwx   0        0        0        0 2024-03-21 20:49:57.641159 maldives-0.0.26/src/maldives/
--rw-rw-rw-   0        0        0       22 2024-03-21 20:49:34.000000 maldives-0.0.26/src/maldives/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-21 20:49:57.694990 maldives-0.0.26/src/maldives/api/
--rw-rw-rw-   0        0        0       94 2023-11-28 01:46:50.000000 maldives-0.0.26/src/maldives/api/__init__.py
--rw-rw-rw-   0        0        0      609 2023-11-22 02:02:45.000000 maldives-0.0.26/src/maldives/api/fred.py
--rw-rw-rw-   0        0        0     1934 2024-01-19 16:51:41.000000 maldives-0.0.26/src/maldives/api/options.py
--rw-rw-rw-   0        0        0    10366 2023-12-19 07:30:42.000000 maldives-0.0.26/src/maldives/api/usda.py
-drwxrwxrwx   0        0        0        0 2024-03-21 20:49:57.702568 maldives-0.0.26/src/maldives/backtest/
--rw-rw-rw-   0        0        0       80 2023-12-19 05:17:27.000000 maldives-0.0.26/src/maldives/backtest/__init__.py
--rw-rw-rw-   0        0        0     3545 2023-12-19 07:55:20.000000 maldives-0.0.26/src/maldives/backtest/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-21 20:49:57.710694 maldives-0.0.26/src/maldives/commodities/
--rw-rw-rw-   0        0        0       70 2023-12-19 07:13:43.000000 maldives-0.0.26/src/maldives/commodities/__init__.py
--rw-rw-rw-   0        0        0     3577 2024-03-09 00:55:29.000000 maldives-0.0.26/src/maldives/commodities/cattle.py
--rw-rw-rw-   0        0        0     3124 2024-03-21 20:43:49.000000 maldives-0.0.26/src/maldives/commodities/gold.py
--rw-rw-rw-   0        0        0      130 2023-11-23 04:00:31.000000 maldives-0.0.26/src/maldives/env.py
-drwxrwxrwx   0        0        0        0 2024-03-21 20:49:57.718319 maldives-0.0.26/src/maldives/maths/
--rw-rw-rw-   0        0        0       83 2023-11-27 08:06:52.000000 maldives-0.0.26/src/maldives/maths/__init__.py
--rw-rw-rw-   0        0        0     2328 2023-11-23 04:02:35.000000 maldives-0.0.26/src/maldives/maths/numerical.py
--rw-rw-rw-   0        0        0     1361 2023-11-23 01:00:36.000000 maldives-0.0.26/src/maldives/maths/smoothing.py
-drwxrwxrwx   0        0        0        0 2024-03-21 20:49:57.727011 maldives-0.0.26/src/maldives/options/
--rw-rw-rw-   0        0        0       53 2023-11-28 01:46:50.000000 maldives-0.0.26/src/maldives/options/__init__.py
--rw-rw-rw-   0        0        0     1563 2023-11-28 01:46:50.000000 maldives-0.0.26/src/maldives/options/implied_distribution.py
-drwxrwxrwx   0        0        0        0 2024-03-21 20:49:57.730558 maldives-0.0.26/src/maldives/regression/
--rw-rw-rw-   0        0        0       41 2023-11-27 08:06:52.000000 maldives-0.0.26/src/maldives/regression/__init__.py
--rw-rw-rw-   0        0        0     3945 2023-12-14 03:25:48.000000 maldives-0.0.26/src/maldives/regression/linear_model.py
-drwxrwxrwx   0        0        0        0 2024-03-21 20:49:57.738680 maldives-0.0.26/src/maldives/timeseries/
--rw-rw-rw-   0        0        0       36 2023-11-27 08:06:52.000000 maldives-0.0.26/src/maldives/timeseries/__init__.py
--rw-rw-rw-   0        0        0       54 2023-11-22 01:06:19.000000 maldives-0.0.26/src/maldives/timeseries/timeseries.py
-drwxrwxrwx   0        0        0        0 2024-03-21 20:49:57.746838 maldives-0.0.26/src/maldives/tuning/
--rw-rw-rw-   0        0        0        0 2023-11-23 19:25:11.000000 maldives-0.0.26/src/maldives/tuning/__init__.py
--rw-rw-rw-   0        0        0     3301 2023-11-23 18:44:16.000000 maldives-0.0.26/src/maldives/tuning/function.py
--rw-rw-rw-   0        0        0      769 2023-11-23 19:43:03.000000 maldives-0.0.26/src/maldives/tuning/loss.py
-drwxrwxrwx   0        0        0        0 2024-03-21 20:49:57.764356 maldives-0.0.26/src/maldives/utils/
--rw-rw-rw-   0        0        0       96 2023-11-27 08:06:52.000000 maldives-0.0.26/src/maldives/utils/__init__.py
--rw-rw-rw-   0        0        0      771 2023-11-27 08:06:52.000000 maldives-0.0.26/src/maldives/utils/array.py
--rw-rw-rw-   0        0        0        0 2023-11-27 08:06:52.000000 maldives-0.0.26/src/maldives/utils/io.py
--rw-rw-rw-   0        0        0      890 2023-11-23 19:22:59.000000 maldives-0.0.26/src/maldives/utils/plotting.py
--rw-rw-rw-   0        0        0     2442 2023-12-19 06:03:40.000000 maldives-0.0.26/src/maldives/utils/scrapping.py
-drwxrwxrwx   0        0        0        0 2024-03-21 20:49:57.766930 maldives-0.0.26/src/maldives.egg-info/
--rw-rw-rw-   0        0        0      869 2024-03-21 20:49:57.000000 maldives-0.0.26/src/maldives.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1095 2024-03-21 20:49:57.000000 maldives-0.0.26/src/maldives.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 20:49:57.000000 maldives-0.0.26/src/maldives.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      123 2024-03-21 20:49:57.000000 maldives-0.0.26/src/maldives.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-03-21 20:49:57.000000 maldives-0.0.26/src/maldives.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-05 04:38:21.360110 maldives-0.0.27/
+-rw-rw-rw-   0        0        0     1063 2023-11-21 22:45:27.000000 maldives-0.0.27/LICENSE
+-rw-rw-rw-   0        0        0      869 2024-05-05 04:38:21.358102 maldives-0.0.27/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-11-21 22:32:31.000000 maldives-0.0.27/README.md
+-rw-rw-rw-   0        0        0      878 2024-03-09 00:55:35.000000 maldives-0.0.27/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-05 04:38:21.360110 maldives-0.0.27/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-05 04:38:21.300985 maldives-0.0.27/src/
+drwxrwxrwx   0        0        0        0 2024-05-05 04:38:21.310342 maldives-0.0.27/src/maldives/
+-rw-rw-rw-   0        0        0       22 2024-05-05 04:38:00.000000 maldives-0.0.27/src/maldives/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 04:38:21.332041 maldives-0.0.27/src/maldives/api/
+-rw-rw-rw-   0        0        0       94 2023-11-28 01:46:50.000000 maldives-0.0.27/src/maldives/api/__init__.py
+-rw-rw-rw-   0        0        0      609 2023-11-22 02:02:45.000000 maldives-0.0.27/src/maldives/api/fred.py
+-rw-rw-rw-   0        0        0     1934 2024-01-19 16:51:41.000000 maldives-0.0.27/src/maldives/api/options.py
+-rw-rw-rw-   0        0        0    10366 2023-12-19 07:30:42.000000 maldives-0.0.27/src/maldives/api/usda.py
+drwxrwxrwx   0        0        0        0 2024-05-05 04:38:21.334425 maldives-0.0.27/src/maldives/backtest/
+-rw-rw-rw-   0        0        0       80 2023-12-19 05:17:27.000000 maldives-0.0.27/src/maldives/backtest/__init__.py
+-rw-rw-rw-   0        0        0     3545 2023-12-19 07:55:20.000000 maldives-0.0.27/src/maldives/backtest/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-05 04:38:21.337427 maldives-0.0.27/src/maldives/commodities/
+-rw-rw-rw-   0        0        0       57 2024-05-05 04:34:44.000000 maldives-0.0.27/src/maldives/commodities/__init__.py
+-rw-rw-rw-   0        0        0     3577 2024-03-09 00:55:29.000000 maldives-0.0.27/src/maldives/commodities/cattle.py
+-rw-rw-rw-   0        0        0      978 2024-05-05 04:30:46.000000 maldives-0.0.27/src/maldives/commodities/gold.py
+-rw-rw-rw-   0        0        0      130 2023-11-23 04:00:31.000000 maldives-0.0.27/src/maldives/env.py
+drwxrwxrwx   0        0        0        0 2024-05-05 04:38:21.341038 maldives-0.0.27/src/maldives/maths/
+-rw-rw-rw-   0        0        0       83 2023-11-27 08:06:52.000000 maldives-0.0.27/src/maldives/maths/__init__.py
+-rw-rw-rw-   0        0        0     2328 2023-11-23 04:02:35.000000 maldives-0.0.27/src/maldives/maths/numerical.py
+-rw-rw-rw-   0        0        0     1361 2023-11-23 01:00:36.000000 maldives-0.0.27/src/maldives/maths/smoothing.py
+drwxrwxrwx   0        0        0        0 2024-05-05 04:38:21.343444 maldives-0.0.27/src/maldives/options/
+-rw-rw-rw-   0        0        0       53 2023-11-28 01:46:50.000000 maldives-0.0.27/src/maldives/options/__init__.py
+-rw-rw-rw-   0        0        0     1563 2023-11-28 01:46:50.000000 maldives-0.0.27/src/maldives/options/implied_distribution.py
+drwxrwxrwx   0        0        0        0 2024-05-05 04:38:21.345736 maldives-0.0.27/src/maldives/regression/
+-rw-rw-rw-   0        0        0       58 2024-05-05 04:33:50.000000 maldives-0.0.27/src/maldives/regression/__init__.py
+-rw-rw-rw-   0        0        0     6316 2024-05-05 04:30:50.000000 maldives-0.0.27/src/maldives/regression/linear_model.py
+drwxrwxrwx   0        0        0        0 2024-05-05 04:38:21.347084 maldives-0.0.27/src/maldives/timeseries/
+-rw-rw-rw-   0        0        0       36 2023-11-27 08:06:52.000000 maldives-0.0.27/src/maldives/timeseries/__init__.py
+-rw-rw-rw-   0        0        0       54 2023-11-22 01:06:19.000000 maldives-0.0.27/src/maldives/timeseries/timeseries.py
+drwxrwxrwx   0        0        0        0 2024-05-05 04:38:21.350447 maldives-0.0.27/src/maldives/tuning/
+-rw-rw-rw-   0        0        0        0 2023-11-23 19:25:11.000000 maldives-0.0.27/src/maldives/tuning/__init__.py
+-rw-rw-rw-   0        0        0     3301 2023-11-23 18:44:16.000000 maldives-0.0.27/src/maldives/tuning/function.py
+-rw-rw-rw-   0        0        0      769 2023-11-23 19:43:03.000000 maldives-0.0.27/src/maldives/tuning/loss.py
+drwxrwxrwx   0        0        0        0 2024-05-05 04:38:21.355801 maldives-0.0.27/src/maldives/utils/
+-rw-rw-rw-   0        0        0       96 2023-11-27 08:06:52.000000 maldives-0.0.27/src/maldives/utils/__init__.py
+-rw-rw-rw-   0        0        0      771 2023-11-27 08:06:52.000000 maldives-0.0.27/src/maldives/utils/array.py
+-rw-rw-rw-   0        0        0        0 2023-11-27 08:06:52.000000 maldives-0.0.27/src/maldives/utils/io.py
+-rw-rw-rw-   0        0        0      890 2023-11-23 19:22:59.000000 maldives-0.0.27/src/maldives/utils/plotting.py
+-rw-rw-rw-   0        0        0     2442 2023-12-19 06:03:40.000000 maldives-0.0.27/src/maldives/utils/scrapping.py
+drwxrwxrwx   0        0        0        0 2024-05-05 04:38:21.356916 maldives-0.0.27/src/maldives.egg-info/
+-rw-rw-rw-   0        0        0      869 2024-05-05 04:38:21.000000 maldives-0.0.27/src/maldives.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1095 2024-05-05 04:38:21.000000 maldives-0.0.27/src/maldives.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 04:38:21.000000 maldives-0.0.27/src/maldives.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      123 2024-05-05 04:38:21.000000 maldives-0.0.27/src/maldives.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-05 04:38:21.000000 maldives-0.0.27/src/maldives.egg-info/top_level.txt
```

### Comparing `maldives-0.0.26/LICENSE` & `maldives-0.0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `maldives-0.0.26/PKG-INFO` & `maldives-0.0.27/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maldives
-Version: 0.0.26
+Version: 0.0.27
 Summary: Tools for systematic commodities analysis.
 Author-email: To Chin Yu <ytc@alum.mit.edu>
 Project-URL: Homepage, https://github.com/ytcs/maldives
 Project-URL: Issues, https://github.com/ytcs/maldives/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `maldives-0.0.26/pyproject.toml` & `maldives-0.0.27/pyproject.toml`

 * *Files identical despite different names*

### Comparing `maldives-0.0.26/src/maldives/api/fred.py` & `maldives-0.0.27/src/maldives/api/fred.py`

 * *Files identical despite different names*

### Comparing `maldives-0.0.26/src/maldives/api/options.py` & `maldives-0.0.27/src/maldives/api/options.py`

 * *Files identical despite different names*

### Comparing `maldives-0.0.26/src/maldives/api/usda.py` & `maldives-0.0.27/src/maldives/api/usda.py`

 * *Files identical despite different names*

### Comparing `maldives-0.0.26/src/maldives/backtest/utils.py` & `maldives-0.0.27/src/maldives/backtest/utils.py`

 * *Files identical despite different names*

### Comparing `maldives-0.0.26/src/maldives/commodities/cattle.py` & `maldives-0.0.27/src/maldives/commodities/cattle.py`

 * *Files identical despite different names*

### Comparing `maldives-0.0.26/src/maldives/maths/numerical.py` & `maldives-0.0.27/src/maldives/maths/numerical.py`

 * *Files identical despite different names*

### Comparing `maldives-0.0.26/src/maldives/maths/smoothing.py` & `maldives-0.0.27/src/maldives/maths/smoothing.py`

 * *Files identical despite different names*

### Comparing `maldives-0.0.26/src/maldives/options/implied_distribution.py` & `maldives-0.0.27/src/maldives/options/implied_distribution.py`

 * *Files identical despite different names*

### Comparing `maldives-0.0.26/src/maldives/tuning/function.py` & `maldives-0.0.27/src/maldives/tuning/function.py`

 * *Files identical despite different names*

### Comparing `maldives-0.0.26/src/maldives/tuning/loss.py` & `maldives-0.0.27/src/maldives/tuning/loss.py`

 * *Files identical despite different names*

### Comparing `maldives-0.0.26/src/maldives/utils/array.py` & `maldives-0.0.27/src/maldives/utils/array.py`

 * *Files identical despite different names*

### Comparing `maldives-0.0.26/src/maldives/utils/plotting.py` & `maldives-0.0.27/src/maldives/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `maldives-0.0.26/src/maldives/utils/scrapping.py` & `maldives-0.0.27/src/maldives/utils/scrapping.py`

 * *Files identical despite different names*

### Comparing `maldives-0.0.26/src/maldives.egg-info/PKG-INFO` & `maldives-0.0.27/src/maldives.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maldives
-Version: 0.0.26
+Version: 0.0.27
 Summary: Tools for systematic commodities analysis.
 Author-email: To Chin Yu <ytc@alum.mit.edu>
 Project-URL: Homepage, https://github.com/ytcs/maldives
 Project-URL: Issues, https://github.com/ytcs/maldives/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `maldives-0.0.26/src/maldives.egg-info/SOURCES.txt` & `maldives-0.0.27/src/maldives.egg-info/SOURCES.txt`

 * *Files identical despite different names*

