# Comparing `tmp/mkt-retv-1.409.tar.gz` & `tmp/mkt-retv-1.410.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkt-retv-1.409.tar", last modified: Fri Apr 26 10:00:44 2024, max compression
+gzip compressed data, was "mkt-retv-1.410.tar", last modified: Sun May  5 10:26:11 2024, max compression
```

## Comparing `mkt-retv-1.409.tar` & `mkt-retv-1.410.tar`

### file list

```diff
@@ -1,47 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 10:00:44.595711 mkt-retv-1.409/
--rw-rw-rw-   0        0        0      697 2024-04-26 10:00:44.592712 mkt-retv-1.409/PKG-INFO
--rw-rw-rw-   0        0        0     1637 2024-01-28 21:55:38.000000 mkt-retv-1.409/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 10:00:44.148626 mkt-retv-1.409/market_research/
--rw-rw-rw-   0        0        0        2 2023-11-21 12:45:19.000000 mkt-retv-1.409/market_research/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 10:00:44.237388 mkt-retv-1.409/market_research/analysis/
--rw-rw-rw-   0        0        0      167 2024-01-28 14:21:17.000000 mkt-retv-1.409/market_research/analysis/__init__.py
--rw-rw-rw-   0        0        0     1285 2023-11-23 12:49:10.000000 mkt-retv-1.409/market_research/analysis/_analysis_scheme.py
--rw-rw-rw-   0        0        0    10414 2024-01-30 11:22:46.000000 mkt-retv-1.409/market_research/analysis/imgemanger.py
--rw-rw-rw-   0        0        0    11047 2023-12-02 10:26:16.000000 mkt-retv-1.409/market_research/analysis/sentimentmanager.py
--rw-rw-rw-   0        0        0     4939 2024-01-28 14:17:23.000000 mkt-retv-1.409/market_research/analysis/textmanager.py
-drwxrwxrwx   0        0        0        0 2024-04-26 10:00:44.283154 mkt-retv-1.409/market_research/scraper/
--rw-rw-rw-   0        0        0      451 2024-01-24 12:15:44.000000 mkt-retv-1.409/market_research/scraper/__init__.py
--rw-rw-rw-   0        0        0     2145 2023-11-21 13:39:46.000000 mkt-retv-1.409/market_research/scraper/_scaper_scheme.py
--rw-rw-rw-   0        0        0      497 2023-11-21 16:22:41.000000 mkt-retv-1.409/market_research/scraper/_visualizer_scheme.py
-drwxrwxrwx   0        0        0        0 2024-04-26 10:00:44.284131 mkt-retv-1.409/market_research/scraper/models/
--rw-rw-rw-   0        0        0        0 2023-11-21 12:44:57.000000 mkt-retv-1.409/market_research/scraper/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 10:00:44.323218 mkt-retv-1.409/market_research/scraper/models/pana/
--rw-rw-rw-   0        0        0        0 2023-11-21 12:44:12.000000 mkt-retv-1.409/market_research/scraper/models/pana/__init__.py
--rw-rw-rw-   0        0        0     6486 2024-04-25 15:07:33.000000 mkt-retv-1.409/market_research/scraper/models/pana/spec_p.py
--rw-rw-rw-   0        0        0    12572 2024-04-25 15:07:18.000000 mkt-retv-1.409/market_research/scraper/models/pana/spec_pjp.py
-drwxrwxrwx   0        0        0        0 2024-04-26 10:00:44.392514 mkt-retv-1.409/market_research/scraper/models/sony/
--rw-rw-rw-   0        0        0        4 2023-11-21 12:44:57.000000 mkt-retv-1.409/market_research/scraper/models/sony/__init__.py
--rw-rw-rw-   0        0        0     5265 2024-04-25 14:52:31.000000 mkt-retv-1.409/market_research/scraper/models/sony/cleanup_s.py
--rw-rw-rw-   0        0        0    10235 2024-04-25 15:08:00.000000 mkt-retv-1.409/market_research/scraper/models/sony/sepc_sjp.py
--rw-rw-rw-   0        0        0    12132 2024-04-26 09:59:41.000000 mkt-retv-1.409/market_research/scraper/models/sony/spec_s.py
--rw-rw-rw-   0        0        0     4189 2024-04-25 14:57:40.000000 mkt-retv-1.409/market_research/scraper/models/sony/visualizer_s.py
-drwxrwxrwx   0        0        0        0 2024-04-26 10:00:44.461043 mkt-retv-1.409/market_research/scraper/rtings/
--rw-rw-rw-   0        0        0      106 2023-11-19 08:24:51.000000 mkt-retv-1.409/market_research/scraper/rtings/__init__.py
--rw-rw-rw-   0        0        0    10290 2023-11-23 09:57:43.000000 mkt-retv-1.409/market_research/scraper/rtings/rtings.py
--rw-rw-rw-   0        0        0     6309 2023-11-26 10:28:52.000000 mkt-retv-1.409/market_research/scraper/rtings/rurlsearcher.py
--rw-rw-rw-   0        0        0    13793 2023-11-23 12:05:59.000000 mkt-retv-1.409/market_research/scraper/rtings/rvisualizer.py
-drwxrwxrwx   0        0        0        0 2024-04-26 10:00:44.529839 mkt-retv-1.409/market_research/tools/
--rw-rw-rw-   0        0        0      206 2023-11-16 08:38:53.000000 mkt-retv-1.409/market_research/tools/__init__.py
--rw-rw-rw-   0        0        0     1003 2023-11-18 14:03:46.000000 mkt-retv-1.409/market_research/tools/aimanager.py
--rw-rw-rw-   0        0        0     3371 2023-11-19 12:13:44.000000 mkt-retv-1.409/market_research/tools/filemanager.py
--rw-rw-rw-   0        0        0     3818 2023-11-14 14:05:22.000000 mkt-retv-1.409/market_research/tools/installer.py
--rw-rw-rw-   0        0        0     5509 2023-11-15 11:16:47.000000 mkt-retv-1.409/market_research/tools/webdriver.py
-drwxrwxrwx   0        0        0        0 2024-04-26 10:00:44.589717 mkt-retv-1.409/mkt_retv.egg-info/
--rw-rw-rw-   0        0        0      697 2024-04-26 10:00:43.000000 mkt-retv-1.409/mkt_retv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1351 2024-04-26 10:00:44.000000 mkt-retv-1.409/mkt_retv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 10:00:43.000000 mkt-retv-1.409/mkt_retv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-04-26 10:00:43.000000 mkt-retv-1.409/mkt_retv.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      129 2024-04-26 10:00:43.000000 mkt-retv-1.409/mkt_retv.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-26 10:00:43.000000 mkt-retv-1.409/mkt_retv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 10:00:44.595711 mkt-retv-1.409/setup.cfg
--rw-rw-rw-   0        0        0      959 2024-04-26 10:00:04.000000 mkt-retv-1.409/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 10:26:11.119930 mkt-retv-1.410/
+-rw-rw-rw-   0        0        0      697 2024-05-05 10:26:11.119930 mkt-retv-1.410/PKG-INFO
+-rw-rw-rw-   0        0        0     1637 2024-01-28 21:55:38.000000 mkt-retv-1.410/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 10:26:11.119930 mkt-retv-1.410/mkt_retv.egg-info/
+-rw-rw-rw-   0        0        0      697 2024-05-05 10:26:10.000000 mkt-retv-1.410/mkt_retv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2024-05-05 10:26:10.000000 mkt-retv-1.410/mkt_retv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 10:26:10.000000 mkt-retv-1.410/mkt_retv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-05-05 10:26:10.000000 mkt-retv-1.410/mkt_retv.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      129 2024-05-05 10:26:10.000000 mkt-retv-1.410/mkt_retv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 10:26:10.000000 mkt-retv-1.410/mkt_retv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-05 10:26:11.119930 mkt-retv-1.410/setup.cfg
+-rw-rw-rw-   0        0        0      959 2024-05-05 10:22:06.000000 mkt-retv-1.410/setup.py
```

### Comparing `mkt-retv-1.409/PKG-INFO` & `mkt-retv-1.410/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkt-retv
-Version: 1.409
+Version: 1.410
 Summary: market research TV 
 Home-page: https://github.com/xikest/research_market_tv
 Author: xikest
 Project-URL: Source, https://github.com/xikest/research_market_tv
 Project-URL: Bug Tracker, https://github.com/xikest/research_market_tv/issues
 Requires-Python: >=3.7
 Requires-Dist: numpy
```

### Comparing `mkt-retv-1.409/README.md` & `mkt-retv-1.410/README.md`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.409/mkt_retv.egg-info/PKG-INFO` & `mkt-retv-1.410/mkt_retv.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkt-retv
-Version: 1.409
+Version: 1.410
 Summary: market research TV 
 Home-page: https://github.com/xikest/research_market_tv
 Author: xikest
 Project-URL: Source, https://github.com/xikest/research_market_tv
 Project-URL: Bug Tracker, https://github.com/xikest/research_market_tv/issues
 Requires-Python: >=3.7
 Requires-Dist: numpy
```

### Comparing `mkt-retv-1.409/setup.py` & `mkt-retv-1.410/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mkt-retv',
-    version='1.409',
+    version='1.410',
     author='xikest',
     description='market research TV ',
     packages=find_packages(),
     python_requires='>=3.7',
     install_requires=[
         'numpy', 'pandas',
         'selenium','beautifulsoup4','requests',
```

