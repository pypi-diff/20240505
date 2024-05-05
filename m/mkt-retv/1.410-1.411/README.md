# Comparing `tmp/mkt-retv-1.410.tar.gz` & `tmp/mkt-retv-1.411.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkt-retv-1.410.tar", last modified: Sun May  5 10:26:11 2024, max compression
+gzip compressed data, was "mkt-retv-1.411.tar", last modified: Sun May  5 10:40:06 2024, max compression
```

## Comparing `mkt-retv-1.410.tar` & `mkt-retv-1.411.tar`

### file list

```diff
@@ -1,12 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 10:26:11.119930 mkt-retv-1.410/
--rw-rw-rw-   0        0        0      697 2024-05-05 10:26:11.119930 mkt-retv-1.410/PKG-INFO
--rw-rw-rw-   0        0        0     1637 2024-01-28 21:55:38.000000 mkt-retv-1.410/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 10:26:11.119930 mkt-retv-1.410/mkt_retv.egg-info/
--rw-rw-rw-   0        0        0      697 2024-05-05 10:26:10.000000 mkt-retv-1.410/mkt_retv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2024-05-05 10:26:10.000000 mkt-retv-1.410/mkt_retv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 10:26:10.000000 mkt-retv-1.410/mkt_retv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-05-05 10:26:10.000000 mkt-retv-1.410/mkt_retv.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      129 2024-05-05 10:26:10.000000 mkt-retv-1.410/mkt_retv.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 10:26:10.000000 mkt-retv-1.410/mkt_retv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-05 10:26:11.119930 mkt-retv-1.410/setup.cfg
--rw-rw-rw-   0        0        0      959 2024-05-05 10:22:06.000000 mkt-retv-1.410/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 10:40:06.072848 mkt-retv-1.411/
+-rw-rw-rw-   0        0        0      697 2024-05-05 10:40:06.071853 mkt-retv-1.411/PKG-INFO
+-rw-rw-rw-   0        0        0     1637 2024-01-28 21:55:38.000000 mkt-retv-1.411/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 10:40:05.992855 mkt-retv-1.411/market_research/
+-rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.411/market_research/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 10:40:06.000846 mkt-retv-1.411/market_research/analysis/
+-rw-rw-rw-   0        0        0      167 2024-01-28 14:21:17.000000 mkt-retv-1.411/market_research/analysis/__init__.py
+-rw-rw-rw-   0        0        0     1285 2023-11-23 12:49:10.000000 mkt-retv-1.411/market_research/analysis/_analysis_scheme.py
+-rw-rw-rw-   0        0        0    10414 2024-01-30 11:22:46.000000 mkt-retv-1.411/market_research/analysis/imgemanger.py
+-rw-rw-rw-   0        0        0    11047 2023-12-02 10:26:16.000000 mkt-retv-1.411/market_research/analysis/sentimentmanager.py
+-rw-rw-rw-   0        0        0     6080 2024-04-27 23:25:08.000000 mkt-retv-1.411/market_research/analysis/textmanager.py
+drwxrwxrwx   0        0        0        0 2024-05-05 10:40:06.005863 mkt-retv-1.411/market_research/scraper/
+-rw-rw-rw-   0        0        0      538 2024-05-05 09:44:35.000000 mkt-retv-1.411/market_research/scraper/__init__.py
+-rw-rw-rw-   0        0        0     2145 2023-11-21 13:39:46.000000 mkt-retv-1.411/market_research/scraper/_scaper_scheme.py
+-rw-rw-rw-   0        0        0      497 2023-11-21 16:22:41.000000 mkt-retv-1.411/market_research/scraper/_visualizer_scheme.py
+drwxrwxrwx   0        0        0        0 2024-05-05 10:40:06.011799 mkt-retv-1.411/market_research/scraper/rtings/
+-rw-rw-rw-   0        0        0      106 2023-11-19 08:24:51.000000 mkt-retv-1.411/market_research/scraper/rtings/__init__.py
+-rw-rw-rw-   0        0        0    10290 2023-11-23 09:57:43.000000 mkt-retv-1.411/market_research/scraper/rtings/rtings.py
+-rw-rw-rw-   0        0        0     6309 2023-11-26 10:28:52.000000 mkt-retv-1.411/market_research/scraper/rtings/rurlsearcher.py
+-rw-rw-rw-   0        0        0    13793 2023-11-23 12:05:59.000000 mkt-retv-1.411/market_research/scraper/rtings/rvisualizer.py
+drwxrwxrwx   0        0        0        0 2024-05-05 10:40:06.018790 mkt-retv-1.411/market_research/tools/
+-rw-rw-rw-   0        0        0      206 2023-11-16 08:38:53.000000 mkt-retv-1.411/market_research/tools/__init__.py
+-rw-rw-rw-   0        0        0     1003 2023-11-18 14:03:46.000000 mkt-retv-1.411/market_research/tools/aimanager.py
+-rw-rw-rw-   0        0        0     3371 2023-11-19 12:13:44.000000 mkt-retv-1.411/market_research/tools/filemanager.py
+-rw-rw-rw-   0        0        0     3818 2023-11-14 14:05:22.000000 mkt-retv-1.411/market_research/tools/installer.py
+-rw-rw-rw-   0        0        0     5509 2023-11-15 11:16:47.000000 mkt-retv-1.411/market_research/tools/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-05-05 10:40:06.069859 mkt-retv-1.411/mkt_retv.egg-info/
+-rw-rw-rw-   0        0        0      697 2024-05-05 10:40:05.000000 mkt-retv-1.411/mkt_retv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      923 2024-05-05 10:40:05.000000 mkt-retv-1.411/mkt_retv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 10:40:05.000000 mkt-retv-1.411/mkt_retv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-05-05 10:40:05.000000 mkt-retv-1.411/mkt_retv.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      129 2024-05-05 10:40:05.000000 mkt-retv-1.411/mkt_retv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-05 10:40:05.000000 mkt-retv-1.411/mkt_retv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-05 10:40:06.072848 mkt-retv-1.411/setup.cfg
+-rw-rw-rw-   0        0        0      959 2024-05-05 10:40:02.000000 mkt-retv-1.411/setup.py
```

### Comparing `mkt-retv-1.410/PKG-INFO` & `mkt-retv-1.411/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkt-retv
-Version: 1.410
+Version: 1.411
 Summary: market research TV 
 Home-page: https://github.com/xikest/research_market_tv
 Author: xikest
 Project-URL: Source, https://github.com/xikest/research_market_tv
 Project-URL: Bug Tracker, https://github.com/xikest/research_market_tv/issues
 Requires-Python: >=3.7
 Requires-Dist: numpy
```

### Comparing `mkt-retv-1.410/README.md` & `mkt-retv-1.411/README.md`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.410/mkt_retv.egg-info/PKG-INFO` & `mkt-retv-1.411/mkt_retv.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkt-retv
-Version: 1.410
+Version: 1.411
 Summary: market research TV 
 Home-page: https://github.com/xikest/research_market_tv
 Author: xikest
 Project-URL: Source, https://github.com/xikest/research_market_tv
 Project-URL: Bug Tracker, https://github.com/xikest/research_market_tv/issues
 Requires-Python: >=3.7
 Requires-Dist: numpy
```

### Comparing `mkt-retv-1.410/setup.py` & `mkt-retv-1.411/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mkt-retv',
-    version='1.410',
+    version='1.411',
     author='xikest',
     description='market research TV ',
     packages=find_packages(),
     python_requires='>=3.7',
     install_requires=[
         'numpy', 'pandas',
         'selenium','beautifulsoup4','requests',
```

