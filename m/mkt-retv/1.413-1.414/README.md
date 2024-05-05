# Comparing `tmp/mkt-retv-1.413.tar.gz` & `tmp/mkt-retv-1.414.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkt-retv-1.413.tar", last modified: Sun May  5 10:51:44 2024, max compression
+gzip compressed data, was "mkt-retv-1.414.tar", last modified: Sun May  5 12:41:22 2024, max compression
```

## Comparing `mkt-retv-1.413.tar` & `mkt-retv-1.414.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 10:51:44.504028 mkt-retv-1.413/
--rw-rw-rw-   0        0        0      697 2024-05-05 10:51:44.502128 mkt-retv-1.413/PKG-INFO
--rw-rw-rw-   0        0        0     1637 2024-01-28 21:55:38.000000 mkt-retv-1.413/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 10:51:44.402515 mkt-retv-1.413/market_research/
--rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.413/market_research/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 10:51:44.418088 mkt-retv-1.413/market_research/analysis/
--rw-rw-rw-   0        0        0      167 2024-01-28 14:21:17.000000 mkt-retv-1.413/market_research/analysis/__init__.py
--rw-rw-rw-   0        0        0     1285 2023-11-23 12:49:10.000000 mkt-retv-1.413/market_research/analysis/_analysis_scheme.py
--rw-rw-rw-   0        0        0    10414 2024-01-30 11:22:46.000000 mkt-retv-1.413/market_research/analysis/imgemanger.py
--rw-rw-rw-   0        0        0    11047 2023-12-02 10:26:16.000000 mkt-retv-1.413/market_research/analysis/sentimentmanager.py
--rw-rw-rw-   0        0        0     6080 2024-04-27 23:25:08.000000 mkt-retv-1.413/market_research/analysis/textmanager.py
-drwxrwxrwx   0        0        0        0 2024-05-05 10:51:44.423098 mkt-retv-1.413/market_research/scraper/
--rw-rw-rw-   0        0        0      538 2024-05-05 09:44:35.000000 mkt-retv-1.413/market_research/scraper/__init__.py
--rw-rw-rw-   0        0        0     2145 2023-11-21 13:39:46.000000 mkt-retv-1.413/market_research/scraper/_scaper_scheme.py
--rw-rw-rw-   0        0        0      497 2023-11-21 16:22:41.000000 mkt-retv-1.413/market_research/scraper/_visualizer_scheme.py
-drwxrwxrwx   0        0        0        0 2024-05-05 10:51:44.423098 mkt-retv-1.413/market_research/scraper/models/
--rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.413/market_research/scraper/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 10:51:44.423098 mkt-retv-1.413/market_research/scraper/models/lge/
--rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.413/market_research/scraper/models/lge/__init__.py
--rw-rw-rw-   0        0        0    12620 2024-05-05 10:21:26.000000 mkt-retv-1.413/market_research/scraper/models/lge/spec_l.py
-drwxrwxrwx   0        0        0        0 2024-05-05 10:51:44.423098 mkt-retv-1.413/market_research/scraper/models/pana/
--rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.413/market_research/scraper/models/pana/__init__.py
--rw-rw-rw-   0        0        0     6486 2024-04-25 15:07:33.000000 mkt-retv-1.413/market_research/scraper/models/pana/spec_p.py
--rw-rw-rw-   0        0        0    12572 2024-04-25 15:07:18.000000 mkt-retv-1.413/market_research/scraper/models/pana/spec_pjp.py
-drwxrwxrwx   0        0        0        0 2024-05-05 10:51:44.443228 mkt-retv-1.413/market_research/scraper/models/sony/
--rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.413/market_research/scraper/models/sony/__init__.py
--rw-rw-rw-   0        0        0     5267 2024-05-05 05:49:12.000000 mkt-retv-1.413/market_research/scraper/models/sony/cleanup_s.py
--rw-rw-rw-   0        0        0    10235 2024-04-25 15:08:00.000000 mkt-retv-1.413/market_research/scraper/models/sony/sepc_sjp.py
--rw-rw-rw-   0        0        0    12164 2024-05-05 10:21:26.000000 mkt-retv-1.413/market_research/scraper/models/sony/spec_s.py
--rw-rw-rw-   0        0        0     4387 2024-05-05 00:51:17.000000 mkt-retv-1.413/market_research/scraper/models/sony/visualizer_s.py
-drwxrwxrwx   0        0        0        0 2024-05-05 10:51:44.443228 mkt-retv-1.413/market_research/scraper/rtings/
--rw-rw-rw-   0        0        0      106 2023-11-19 08:24:51.000000 mkt-retv-1.413/market_research/scraper/rtings/__init__.py
--rw-rw-rw-   0        0        0    10290 2023-11-23 09:57:43.000000 mkt-retv-1.413/market_research/scraper/rtings/rtings.py
--rw-rw-rw-   0        0        0     6309 2023-11-26 10:28:52.000000 mkt-retv-1.413/market_research/scraper/rtings/rurlsearcher.py
--rw-rw-rw-   0        0        0    13793 2023-11-23 12:05:59.000000 mkt-retv-1.413/market_research/scraper/rtings/rvisualizer.py
-drwxrwxrwx   0        0        0        0 2024-05-05 10:51:44.460061 mkt-retv-1.413/market_research/tools/
--rw-rw-rw-   0        0        0      206 2023-11-16 08:38:53.000000 mkt-retv-1.413/market_research/tools/__init__.py
--rw-rw-rw-   0        0        0     1003 2023-11-18 14:03:46.000000 mkt-retv-1.413/market_research/tools/aimanager.py
--rw-rw-rw-   0        0        0     3371 2023-11-19 12:13:44.000000 mkt-retv-1.413/market_research/tools/filemanager.py
--rw-rw-rw-   0        0        0     3818 2023-11-14 14:05:22.000000 mkt-retv-1.413/market_research/tools/installer.py
--rw-rw-rw-   0        0        0     5509 2023-11-15 11:16:47.000000 mkt-retv-1.413/market_research/tools/webdriver.py
-drwxrwxrwx   0        0        0        0 2024-05-05 10:51:44.486326 mkt-retv-1.413/mkt_retv.egg-info/
--rw-rw-rw-   0        0        0      697 2024-05-05 10:51:44.000000 mkt-retv-1.413/mkt_retv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1443 2024-05-05 10:51:44.000000 mkt-retv-1.413/mkt_retv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 10:51:44.000000 mkt-retv-1.413/mkt_retv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-05-05 10:51:44.000000 mkt-retv-1.413/mkt_retv.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      129 2024-05-05 10:51:44.000000 mkt-retv-1.413/mkt_retv.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-05 10:51:44.000000 mkt-retv-1.413/mkt_retv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-05 10:51:44.504028 mkt-retv-1.413/setup.cfg
--rw-rw-rw-   0        0        0      959 2024-05-05 10:51:35.000000 mkt-retv-1.413/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 12:41:22.371388 mkt-retv-1.414/
+-rw-rw-rw-   0        0        0      697 2024-05-05 12:41:22.371388 mkt-retv-1.414/PKG-INFO
+-rw-rw-rw-   0        0        0     1637 2024-01-28 21:55:38.000000 mkt-retv-1.414/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 12:41:21.897092 mkt-retv-1.414/market_research/
+-rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.414/market_research/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 12:41:21.976021 mkt-retv-1.414/market_research/analysis/
+-rw-rw-rw-   0        0        0      167 2024-01-28 14:21:17.000000 mkt-retv-1.414/market_research/analysis/__init__.py
+-rw-rw-rw-   0        0        0     1285 2023-11-23 12:49:10.000000 mkt-retv-1.414/market_research/analysis/_analysis_scheme.py
+-rw-rw-rw-   0        0        0    10414 2024-01-30 11:22:46.000000 mkt-retv-1.414/market_research/analysis/imgemanger.py
+-rw-rw-rw-   0        0        0    11047 2023-12-02 10:26:16.000000 mkt-retv-1.414/market_research/analysis/sentimentmanager.py
+-rw-rw-rw-   0        0        0     6080 2024-04-27 23:25:08.000000 mkt-retv-1.414/market_research/analysis/textmanager.py
+drwxrwxrwx   0        0        0        0 2024-05-05 12:41:22.024232 mkt-retv-1.414/market_research/scraper/
+-rw-rw-rw-   0        0        0      538 2024-05-05 09:44:35.000000 mkt-retv-1.414/market_research/scraper/__init__.py
+-rw-rw-rw-   0        0        0     2145 2023-11-21 13:39:46.000000 mkt-retv-1.414/market_research/scraper/_scaper_scheme.py
+-rw-rw-rw-   0        0        0      497 2023-11-21 16:22:41.000000 mkt-retv-1.414/market_research/scraper/_visualizer_scheme.py
+drwxrwxrwx   0        0        0        0 2024-05-05 12:41:22.024232 mkt-retv-1.414/market_research/scraper/models/
+-rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.414/market_research/scraper/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 12:41:22.039974 mkt-retv-1.414/market_research/scraper/models/lge/
+-rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.414/market_research/scraper/models/lge/__init__.py
+-rw-rw-rw-   0        0        0    12646 2024-05-05 12:41:04.000000 mkt-retv-1.414/market_research/scraper/models/lge/spec_l.py
+drwxrwxrwx   0        0        0        0 2024-05-05 12:41:22.080503 mkt-retv-1.414/market_research/scraper/models/pana/
+-rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.414/market_research/scraper/models/pana/__init__.py
+-rw-rw-rw-   0        0        0     6486 2024-04-25 15:07:33.000000 mkt-retv-1.414/market_research/scraper/models/pana/spec_p.py
+-rw-rw-rw-   0        0        0    12572 2024-04-25 15:07:18.000000 mkt-retv-1.414/market_research/scraper/models/pana/spec_pjp.py
+drwxrwxrwx   0        0        0        0 2024-05-05 12:41:22.134231 mkt-retv-1.414/market_research/scraper/models/sony/
+-rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.414/market_research/scraper/models/sony/__init__.py
+-rw-rw-rw-   0        0        0     5267 2024-05-05 05:49:12.000000 mkt-retv-1.414/market_research/scraper/models/sony/cleanup_s.py
+-rw-rw-rw-   0        0        0    10235 2024-04-25 15:08:00.000000 mkt-retv-1.414/market_research/scraper/models/sony/sepc_sjp.py
+-rw-rw-rw-   0        0        0    12190 2024-05-05 12:03:01.000000 mkt-retv-1.414/market_research/scraper/models/sony/spec_s.py
+-rw-rw-rw-   0        0        0     4387 2024-05-05 00:51:17.000000 mkt-retv-1.414/market_research/scraper/models/sony/visualizer_s.py
+drwxrwxrwx   0        0        0        0 2024-05-05 12:41:22.212492 mkt-retv-1.414/market_research/scraper/rtings/
+-rw-rw-rw-   0        0        0      106 2023-11-19 08:24:51.000000 mkt-retv-1.414/market_research/scraper/rtings/__init__.py
+-rw-rw-rw-   0        0        0    10290 2023-11-23 09:57:43.000000 mkt-retv-1.414/market_research/scraper/rtings/rtings.py
+-rw-rw-rw-   0        0        0     6309 2023-11-26 10:28:52.000000 mkt-retv-1.414/market_research/scraper/rtings/rurlsearcher.py
+-rw-rw-rw-   0        0        0    13793 2023-11-23 12:05:59.000000 mkt-retv-1.414/market_research/scraper/rtings/rvisualizer.py
+drwxrwxrwx   0        0        0        0 2024-05-05 12:41:22.307469 mkt-retv-1.414/market_research/tools/
+-rw-rw-rw-   0        0        0      206 2023-11-16 08:38:53.000000 mkt-retv-1.414/market_research/tools/__init__.py
+-rw-rw-rw-   0        0        0     1003 2023-11-18 14:03:46.000000 mkt-retv-1.414/market_research/tools/aimanager.py
+-rw-rw-rw-   0        0        0     3371 2023-11-19 12:13:44.000000 mkt-retv-1.414/market_research/tools/filemanager.py
+-rw-rw-rw-   0        0        0     3818 2023-11-14 14:05:22.000000 mkt-retv-1.414/market_research/tools/installer.py
+-rw-rw-rw-   0        0        0     5509 2023-11-15 11:16:47.000000 mkt-retv-1.414/market_research/tools/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-05-05 12:41:22.354932 mkt-retv-1.414/mkt_retv.egg-info/
+-rw-rw-rw-   0        0        0      697 2024-05-05 12:41:21.000000 mkt-retv-1.414/mkt_retv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1443 2024-05-05 12:41:21.000000 mkt-retv-1.414/mkt_retv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 12:41:21.000000 mkt-retv-1.414/mkt_retv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-05-05 12:41:21.000000 mkt-retv-1.414/mkt_retv.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      129 2024-05-05 12:41:21.000000 mkt-retv-1.414/mkt_retv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-05 12:41:21.000000 mkt-retv-1.414/mkt_retv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-05 12:41:22.371388 mkt-retv-1.414/setup.cfg
+-rw-rw-rw-   0        0        0      959 2024-05-05 12:41:17.000000 mkt-retv-1.414/setup.py
```

### Comparing `mkt-retv-1.413/PKG-INFO` & `mkt-retv-1.414/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkt-retv
-Version: 1.413
+Version: 1.414
 Summary: market research TV 
 Home-page: https://github.com/xikest/research_market_tv
 Author: xikest
 Project-URL: Source, https://github.com/xikest/research_market_tv
 Project-URL: Bug Tracker, https://github.com/xikest/research_market_tv/issues
 Requires-Python: >=3.7
 Requires-Dist: numpy
```

### Comparing `mkt-retv-1.413/README.md` & `mkt-retv-1.414/README.md`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.413/market_research/analysis/_analysis_scheme.py` & `mkt-retv-1.414/market_research/analysis/_analysis_scheme.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.413/market_research/analysis/imgemanger.py` & `mkt-retv-1.414/market_research/analysis/imgemanger.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.413/market_research/analysis/sentimentmanager.py` & `mkt-retv-1.414/market_research/analysis/sentimentmanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.413/market_research/analysis/textmanager.py` & `mkt-retv-1.414/market_research/analysis/textmanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.413/market_research/scraper/__init__.py` & `mkt-retv-1.414/market_research/scraper/__init__.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.413/market_research/scraper/_scaper_scheme.py` & `mkt-retv-1.414/market_research/scraper/_scaper_scheme.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.413/market_research/scraper/models/lge/spec_l.py` & `mkt-retv-1.414/market_research/scraper/models/lge/spec_l.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,15 @@
                 dict_info = self._get_model_info(url_model)
                 dict_models[key] = dict_info
                 dict_spec = self._get_global_spec(url=url_model)
                 dict_models[key].update(dict_spec)
                 visit_url_dict[key] = url_model
             except Exception as e:
                 print(f"Failed to get info from {key}")
+                print(e)
                 pass
         print("\n")
         for model, url in visit_url_dict.items():  print(f"{model}: {url}")
 
         if format_df:
             df_models = pd.DataFrame.from_dict(dict_models).T
             FileManager.df_to_excel(df_models.reset_index(), file_name=self.output_xlsx_name, sheet_name="raw_na",
```

### Comparing `mkt-retv-1.413/market_research/scraper/models/pana/spec_p.py` & `mkt-retv-1.414/market_research/scraper/models/pana/spec_p.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.413/market_research/scraper/models/pana/spec_pjp.py` & `mkt-retv-1.414/market_research/scraper/models/pana/spec_pjp.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.413/market_research/scraper/models/sony/cleanup_s.py` & `mkt-retv-1.414/market_research/scraper/models/sony/cleanup_s.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.413/market_research/scraper/models/sony/sepc_sjp.py` & `mkt-retv-1.414/market_research/scraper/models/sony/sepc_sjp.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.413/market_research/scraper/models/sony/spec_s.py` & `mkt-retv-1.414/market_research/scraper/models/sony/spec_s.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
                 dict_info = self._get_model_info(url_model)
                 dict_models[key] = dict_info
                 dict_spec = self._get_global_spec(url=url_model)
                 dict_models[key].update(dict_spec)
                 visit_url_dict[key] = url_model
             except Exception as e:
                 print(f"Failed to get info from {key}")
+                print(e)
                 pass
 
         for model, url in visit_url_dict.items():  print(f"{model}: {url}")
 
         if format_df:
             df_models = pd.DataFrame.from_dict(dict_models).T
             if temporary_year_marking:
```

### Comparing `mkt-retv-1.413/market_research/scraper/models/sony/visualizer_s.py` & `mkt-retv-1.414/market_research/scraper/models/sony/visualizer_s.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.413/market_research/scraper/rtings/rtings.py` & `mkt-retv-1.414/market_research/scraper/rtings/rtings.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.413/market_research/scraper/rtings/rurlsearcher.py` & `mkt-retv-1.414/market_research/scraper/rtings/rurlsearcher.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.413/market_research/scraper/rtings/rvisualizer.py` & `mkt-retv-1.414/market_research/scraper/rtings/rvisualizer.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.413/market_research/tools/aimanager.py` & `mkt-retv-1.414/market_research/tools/aimanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.413/market_research/tools/filemanager.py` & `mkt-retv-1.414/market_research/tools/filemanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.413/market_research/tools/installer.py` & `mkt-retv-1.414/market_research/tools/installer.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.413/market_research/tools/webdriver.py` & `mkt-retv-1.414/market_research/tools/webdriver.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.413/mkt_retv.egg-info/PKG-INFO` & `mkt-retv-1.414/mkt_retv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkt-retv
-Version: 1.413
+Version: 1.414
 Summary: market research TV 
 Home-page: https://github.com/xikest/research_market_tv
 Author: xikest
 Project-URL: Source, https://github.com/xikest/research_market_tv
 Project-URL: Bug Tracker, https://github.com/xikest/research_market_tv/issues
 Requires-Python: >=3.7
 Requires-Dist: numpy
```

### Comparing `mkt-retv-1.413/mkt_retv.egg-info/SOURCES.txt` & `mkt-retv-1.414/mkt_retv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.413/setup.py` & `mkt-retv-1.414/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mkt-retv',
-    version='1.413',
+    version='1.414',
     author='xikest',
     description='market research TV ',
     packages=find_packages(),
     python_requires='>=3.7',
     install_requires=[
         'numpy', 'pandas',
         'selenium','beautifulsoup4','requests',
```

