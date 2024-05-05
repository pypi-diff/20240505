# Comparing `tmp/fredapi-0.5.1.tar.gz` & `tmp/fredapi-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fredapi-0.5.1.tar", last modified: Sat Jul 22 10:32:26 2023, max compression
+gzip compressed data, was "fredapi-0.5.2.tar", last modified: Sun May  5 11:40:52 2024, max compression
```

## Comparing `fredapi-0.5.1.tar` & `fredapi-0.5.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mortadamehyar   (501) staff       (20)        0 2023-07-22 10:32:26.211425 fredapi-0.5.1/
--rw-r--r--   0 mortadamehyar   (501) staff       (20)     4088 2015-03-02 17:50:16.000000 fredapi-0.5.1/DESCRIPTION.rst
--rw-r--r--   0 mortadamehyar   (501) staff       (20)    11324 2014-09-14 21:07:19.000000 fredapi-0.5.1/LICENSE
--rw-r--r--   0 mortadamehyar   (501) staff       (20)       43 2019-01-19 06:53:28.000000 fredapi-0.5.1/MANIFEST.in
--rw-r--r--   0 mortadamehyar   (501) staff       (20)     5004 2023-07-22 10:32:26.211296 fredapi-0.5.1/PKG-INFO
--rw-r--r--   0 mortadamehyar   (501) staff       (20)     8508 2019-01-19 06:53:28.000000 fredapi-0.5.1/README.md
-drwxr-xr-x   0 mortadamehyar   (501) staff       (20)        0 2023-07-22 10:32:26.210383 fredapi-0.5.1/fredapi/
--rw-r--r--   0 mortadamehyar   (501) staff       (20)       82 2015-05-20 16:41:21.000000 fredapi-0.5.1/fredapi/__init__.py
--rw-r--r--   0 mortadamehyar   (501) staff       (20)    19658 2023-07-22 09:55:59.000000 fredapi-0.5.1/fredapi/fred.py
--rw-r--r--   0 mortadamehyar   (501) staff       (20)       19 2023-07-22 09:55:59.000000 fredapi-0.5.1/fredapi/version.py
-drwxr-xr-x   0 mortadamehyar   (501) staff       (20)        0 2023-07-22 10:32:26.211104 fredapi-0.5.1/fredapi.egg-info/
--rw-r--r--   0 mortadamehyar   (501) staff       (20)     5004 2023-07-22 10:32:26.000000 fredapi-0.5.1/fredapi.egg-info/PKG-INFO
--rw-r--r--   0 mortadamehyar   (501) staff       (20)      263 2023-07-22 10:32:26.000000 fredapi-0.5.1/fredapi.egg-info/SOURCES.txt
--rw-r--r--   0 mortadamehyar   (501) staff       (20)        1 2023-07-22 10:32:26.000000 fredapi-0.5.1/fredapi.egg-info/dependency_links.txt
--rw-r--r--   0 mortadamehyar   (501) staff       (20)        7 2023-07-22 10:32:26.000000 fredapi-0.5.1/fredapi.egg-info/requires.txt
--rw-r--r--   0 mortadamehyar   (501) staff       (20)        8 2023-07-22 10:32:26.000000 fredapi-0.5.1/fredapi.egg-info/top_level.txt
--rw-r--r--   0 mortadamehyar   (501) staff       (20)       38 2023-07-22 10:32:26.211458 fredapi-0.5.1/setup.cfg
--rw-r--r--   0 mortadamehyar   (501) staff       (20)     1387 2017-09-03 02:31:48.000000 fredapi-0.5.1/setup.py
+drwxr-xr-x   0 mortadamehyar   (501) staff       (20)        0 2024-05-05 11:40:52.597680 fredapi-0.5.2/
+-rw-r--r--   0 mortadamehyar   (501) staff       (20)     4088 2015-03-02 17:50:16.000000 fredapi-0.5.2/DESCRIPTION.rst
+-rw-r--r--   0 mortadamehyar   (501) staff       (20)    11324 2014-09-14 21:07:19.000000 fredapi-0.5.2/LICENSE
+-rw-r--r--   0 mortadamehyar   (501) staff       (20)       43 2019-01-19 06:53:28.000000 fredapi-0.5.2/MANIFEST.in
+-rw-r--r--   0 mortadamehyar   (501) staff       (20)     5004 2024-05-05 11:40:52.597562 fredapi-0.5.2/PKG-INFO
+-rw-r--r--   0 mortadamehyar   (501) staff       (20)     9024 2024-05-05 11:33:46.000000 fredapi-0.5.2/README.md
+drwxr-xr-x   0 mortadamehyar   (501) staff       (20)        0 2024-05-05 11:40:52.596792 fredapi-0.5.2/fredapi/
+-rw-r--r--   0 mortadamehyar   (501) staff       (20)       82 2015-05-20 16:41:21.000000 fredapi-0.5.2/fredapi/__init__.py
+-rw-r--r--   0 mortadamehyar   (501) staff       (20)    20463 2024-05-05 11:33:46.000000 fredapi-0.5.2/fredapi/fred.py
+-rw-r--r--   0 mortadamehyar   (501) staff       (20)       19 2024-05-05 11:36:42.000000 fredapi-0.5.2/fredapi/version.py
+drwxr-xr-x   0 mortadamehyar   (501) staff       (20)        0 2024-05-05 11:40:52.597372 fredapi-0.5.2/fredapi.egg-info/
+-rw-r--r--   0 mortadamehyar   (501) staff       (20)     5004 2024-05-05 11:40:52.000000 fredapi-0.5.2/fredapi.egg-info/PKG-INFO
+-rw-r--r--   0 mortadamehyar   (501) staff       (20)      263 2024-05-05 11:40:52.000000 fredapi-0.5.2/fredapi.egg-info/SOURCES.txt
+-rw-r--r--   0 mortadamehyar   (501) staff       (20)        1 2024-05-05 11:40:52.000000 fredapi-0.5.2/fredapi.egg-info/dependency_links.txt
+-rw-r--r--   0 mortadamehyar   (501) staff       (20)        7 2024-05-05 11:40:52.000000 fredapi-0.5.2/fredapi.egg-info/requires.txt
+-rw-r--r--   0 mortadamehyar   (501) staff       (20)        8 2024-05-05 11:40:52.000000 fredapi-0.5.2/fredapi.egg-info/top_level.txt
+-rw-r--r--   0 mortadamehyar   (501) staff       (20)       38 2024-05-05 11:40:52.597728 fredapi-0.5.2/setup.cfg
+-rw-r--r--   0 mortadamehyar   (501) staff       (20)     1387 2017-09-03 02:31:48.000000 fredapi-0.5.2/setup.py
```

### Comparing `fredapi-0.5.1/DESCRIPTION.rst` & `fredapi-0.5.2/DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `fredapi-0.5.1/LICENSE` & `fredapi-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fredapi-0.5.1/PKG-INFO` & `fredapi-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fredapi
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python API for Federal Reserve Economic Data (FRED) from St. Louis Fed
 Home-page: https://github.com/mortada/fredapi
 Author: Mortada Mehyar
 Platform: Any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
```

### Comparing `fredapi-0.5.1/README.md` & `fredapi-0.5.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 
 # fredapi: Python API for FRED (Federal Reserve Economic Data)
 
+[![Build and test GitHub](https://github.com/mortada/fredapi/actions/workflows/main.yml/badge.svg)](https://github.com/mortada/fredapi/actions)
+[![version](https://img.shields.io/badge/version-0.5.1-success.svg)](#)
+[![PyPI Latest Release](https://img.shields.io/pypi/v/fredapi.svg)](https://pypi.org/project/fredapi/)
+[![Downloads](https://static.pepy.tech/personalized-badge/fredapi?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads)](https://pepy.tech/project/fredapi)
+
 `fredapi` is a Python API for the [FRED](http://research.stlouisfed.org/fred2/) data provided by the
 Federal Reserve Bank of St. Louis. `fredapi` provides a wrapper in python to the 
 [FRED web service](http://api.stlouisfed.org/docs/fred/), and also provides several convenient methods
 for parsing and analyzing point-in-time data (i.e. historic data revisions) from [ALFRED](http://research.stlouisfed.org/tips/alfred/)
 
 `fredapi` makes use of `pandas` and returns data to you in a `pandas` `Series` or `DataFrame`
```

### Comparing `fredapi-0.5.1/fredapi/fred.py` & `fredapi-0.5.2/fredapi/fred.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,30 +14,39 @@
 import pandas as pd
 
 urlopen = url_request.urlopen
 quote_plus = url_parse.quote_plus
 urlencode = url_parse.urlencode
 HTTPError = url_error.HTTPError
 
-
 class Fred:
     earliest_realtime_start = '1776-07-04'
     latest_realtime_end = '9999-12-31'
     nan_char = '.'
     max_results_per_request = 1000
     root_url = 'https://api.stlouisfed.org/fred'
 
     def __init__(self,
                  api_key=None,
-                 api_key_file=None):
+                 api_key_file=None,
+                 proxies=None):
         """
         Initialize the Fred class that provides useful functions to query the Fred dataset. You need to specify a valid
         API key in one of 3 ways: pass the string via api_key, or set api_key_file to a file with the api key in the
-        first line, or set the environment variable 'FRED_API_KEY' to the value of your api key. You can sign up for a
-        free api key on the Fred website at http://research.stlouisfed.org/fred2/
+        first line, or set the environment variable 'FRED_API_KEY' to the value of your api key.
+
+        Parameters
+        ----------
+        api_key : str
+            API key. A free api key can be obtained on the Fred website at http://research.stlouisfed.org/fred2/.
+        api_key_file : str
+            Path to a file containing the api key.
+        proxies : dict
+            Proxies specifications: a dictionary mapping protocol names (e.g. 'http', 'https') to proxy URLs. If not provided, environment variables 'HTTP_PROXY', 'HTTPS_PROXY' are used.
+
         """
         self.api_key = None
         if api_key is not None:
             self.api_key = api_key
         elif api_key_file is not None:
             f = open(api_key_file, 'r')
             self.api_key = f.readline().strip()
@@ -51,14 +60,25 @@
                     You need to set a valid API key. You can set it in 3 ways:
                     pass the string with api_key, or set api_key_file to a
                     file with the api key in the first line, or set the
                     environment variable 'FRED_API_KEY' to the value of your
                     api key. You can sign up for a free api key on the Fred
                     website at http://research.stlouisfed.org/fred2/"""))
 
+        if not proxies:
+            http_proxy, https_proxy = os.getenv('HTTP_PROXY'), os.getenv('HTTPS_PROXY')
+            if http_proxy or https_proxy:
+                proxies = {'http': http_proxy, 'https': https_proxy}
+
+        self.proxies = proxies
+
+        if self.proxies:
+            opener = url_request.build_opener(url_request.ProxyHandler(self.proxies))
+            url_request.install_opener(opener)
+
     def __fetch_data(self, url):
         """
         helper function for fetching data given a request URL
         """
         url += '&api_key=' + self.api_key
         try:
             response = urlopen(url)
```

### Comparing `fredapi-0.5.1/fredapi.egg-info/PKG-INFO` & `fredapi-0.5.2/fredapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fredapi
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python API for Federal Reserve Economic Data (FRED) from St. Louis Fed
 Home-page: https://github.com/mortada/fredapi
 Author: Mortada Mehyar
 Platform: Any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
```

### Comparing `fredapi-0.5.1/setup.py` & `fredapi-0.5.2/setup.py`

 * *Files identical despite different names*

