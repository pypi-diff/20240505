# Comparing `tmp/mkt-retv-1.414.tar.gz` & `tmp/mkt-retv-1.415.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkt-retv-1.414.tar", last modified: Sun May  5 12:41:22 2024, max compression
+gzip compressed data, was "mkt-retv-1.415.tar", last modified: Sun May  5 13:46:53 2024, max compression
```

## Comparing `mkt-retv-1.414.tar` & `mkt-retv-1.415.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 12:41:22.371388 mkt-retv-1.414/
--rw-rw-rw-   0        0        0      697 2024-05-05 12:41:22.371388 mkt-retv-1.414/PKG-INFO
--rw-rw-rw-   0        0        0     1637 2024-01-28 21:55:38.000000 mkt-retv-1.414/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 12:41:21.897092 mkt-retv-1.414/market_research/
--rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.414/market_research/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 12:41:21.976021 mkt-retv-1.414/market_research/analysis/
--rw-rw-rw-   0        0        0      167 2024-01-28 14:21:17.000000 mkt-retv-1.414/market_research/analysis/__init__.py
--rw-rw-rw-   0        0        0     1285 2023-11-23 12:49:10.000000 mkt-retv-1.414/market_research/analysis/_analysis_scheme.py
--rw-rw-rw-   0        0        0    10414 2024-01-30 11:22:46.000000 mkt-retv-1.414/market_research/analysis/imgemanger.py
--rw-rw-rw-   0        0        0    11047 2023-12-02 10:26:16.000000 mkt-retv-1.414/market_research/analysis/sentimentmanager.py
--rw-rw-rw-   0        0        0     6080 2024-04-27 23:25:08.000000 mkt-retv-1.414/market_research/analysis/textmanager.py
-drwxrwxrwx   0        0        0        0 2024-05-05 12:41:22.024232 mkt-retv-1.414/market_research/scraper/
--rw-rw-rw-   0        0        0      538 2024-05-05 09:44:35.000000 mkt-retv-1.414/market_research/scraper/__init__.py
--rw-rw-rw-   0        0        0     2145 2023-11-21 13:39:46.000000 mkt-retv-1.414/market_research/scraper/_scaper_scheme.py
--rw-rw-rw-   0        0        0      497 2023-11-21 16:22:41.000000 mkt-retv-1.414/market_research/scraper/_visualizer_scheme.py
-drwxrwxrwx   0        0        0        0 2024-05-05 12:41:22.024232 mkt-retv-1.414/market_research/scraper/models/
--rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.414/market_research/scraper/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 12:41:22.039974 mkt-retv-1.414/market_research/scraper/models/lge/
--rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.414/market_research/scraper/models/lge/__init__.py
--rw-rw-rw-   0        0        0    12646 2024-05-05 12:41:04.000000 mkt-retv-1.414/market_research/scraper/models/lge/spec_l.py
-drwxrwxrwx   0        0        0        0 2024-05-05 12:41:22.080503 mkt-retv-1.414/market_research/scraper/models/pana/
--rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.414/market_research/scraper/models/pana/__init__.py
--rw-rw-rw-   0        0        0     6486 2024-04-25 15:07:33.000000 mkt-retv-1.414/market_research/scraper/models/pana/spec_p.py
--rw-rw-rw-   0        0        0    12572 2024-04-25 15:07:18.000000 mkt-retv-1.414/market_research/scraper/models/pana/spec_pjp.py
-drwxrwxrwx   0        0        0        0 2024-05-05 12:41:22.134231 mkt-retv-1.414/market_research/scraper/models/sony/
--rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.414/market_research/scraper/models/sony/__init__.py
--rw-rw-rw-   0        0        0     5267 2024-05-05 05:49:12.000000 mkt-retv-1.414/market_research/scraper/models/sony/cleanup_s.py
--rw-rw-rw-   0        0        0    10235 2024-04-25 15:08:00.000000 mkt-retv-1.414/market_research/scraper/models/sony/sepc_sjp.py
--rw-rw-rw-   0        0        0    12190 2024-05-05 12:03:01.000000 mkt-retv-1.414/market_research/scraper/models/sony/spec_s.py
--rw-rw-rw-   0        0        0     4387 2024-05-05 00:51:17.000000 mkt-retv-1.414/market_research/scraper/models/sony/visualizer_s.py
-drwxrwxrwx   0        0        0        0 2024-05-05 12:41:22.212492 mkt-retv-1.414/market_research/scraper/rtings/
--rw-rw-rw-   0        0        0      106 2023-11-19 08:24:51.000000 mkt-retv-1.414/market_research/scraper/rtings/__init__.py
--rw-rw-rw-   0        0        0    10290 2023-11-23 09:57:43.000000 mkt-retv-1.414/market_research/scraper/rtings/rtings.py
--rw-rw-rw-   0        0        0     6309 2023-11-26 10:28:52.000000 mkt-retv-1.414/market_research/scraper/rtings/rurlsearcher.py
--rw-rw-rw-   0        0        0    13793 2023-11-23 12:05:59.000000 mkt-retv-1.414/market_research/scraper/rtings/rvisualizer.py
-drwxrwxrwx   0        0        0        0 2024-05-05 12:41:22.307469 mkt-retv-1.414/market_research/tools/
--rw-rw-rw-   0        0        0      206 2023-11-16 08:38:53.000000 mkt-retv-1.414/market_research/tools/__init__.py
--rw-rw-rw-   0        0        0     1003 2023-11-18 14:03:46.000000 mkt-retv-1.414/market_research/tools/aimanager.py
--rw-rw-rw-   0        0        0     3371 2023-11-19 12:13:44.000000 mkt-retv-1.414/market_research/tools/filemanager.py
--rw-rw-rw-   0        0        0     3818 2023-11-14 14:05:22.000000 mkt-retv-1.414/market_research/tools/installer.py
--rw-rw-rw-   0        0        0     5509 2023-11-15 11:16:47.000000 mkt-retv-1.414/market_research/tools/webdriver.py
-drwxrwxrwx   0        0        0        0 2024-05-05 12:41:22.354932 mkt-retv-1.414/mkt_retv.egg-info/
--rw-rw-rw-   0        0        0      697 2024-05-05 12:41:21.000000 mkt-retv-1.414/mkt_retv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1443 2024-05-05 12:41:21.000000 mkt-retv-1.414/mkt_retv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 12:41:21.000000 mkt-retv-1.414/mkt_retv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-05-05 12:41:21.000000 mkt-retv-1.414/mkt_retv.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      129 2024-05-05 12:41:21.000000 mkt-retv-1.414/mkt_retv.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-05 12:41:21.000000 mkt-retv-1.414/mkt_retv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-05 12:41:22.371388 mkt-retv-1.414/setup.cfg
--rw-rw-rw-   0        0        0      959 2024-05-05 12:41:17.000000 mkt-retv-1.414/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 13:46:53.812066 mkt-retv-1.415/
+-rw-rw-rw-   0        0        0      697 2024-05-05 13:46:53.807612 mkt-retv-1.415/PKG-INFO
+-rw-rw-rw-   0        0        0     1637 2024-01-28 21:55:38.000000 mkt-retv-1.415/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 13:46:53.698839 mkt-retv-1.415/market_research/
+-rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.415/market_research/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 13:46:53.707695 mkt-retv-1.415/market_research/analysis/
+-rw-rw-rw-   0        0        0      167 2024-01-28 14:21:17.000000 mkt-retv-1.415/market_research/analysis/__init__.py
+-rw-rw-rw-   0        0        0     1285 2023-11-23 12:49:10.000000 mkt-retv-1.415/market_research/analysis/_analysis_scheme.py
+-rw-rw-rw-   0        0        0    10414 2024-01-30 11:22:46.000000 mkt-retv-1.415/market_research/analysis/imgemanger.py
+-rw-rw-rw-   0        0        0    11047 2023-12-02 10:26:16.000000 mkt-retv-1.415/market_research/analysis/sentimentmanager.py
+-rw-rw-rw-   0        0        0     6080 2024-04-27 23:25:08.000000 mkt-retv-1.415/market_research/analysis/textmanager.py
+drwxrwxrwx   0        0        0        0 2024-05-05 13:46:53.716244 mkt-retv-1.415/market_research/scraper/
+-rw-rw-rw-   0        0        0      538 2024-05-05 09:44:35.000000 mkt-retv-1.415/market_research/scraper/__init__.py
+-rw-rw-rw-   0        0        0     2145 2023-11-21 13:39:46.000000 mkt-retv-1.415/market_research/scraper/_scaper_scheme.py
+-rw-rw-rw-   0        0        0      497 2023-11-21 16:22:41.000000 mkt-retv-1.415/market_research/scraper/_visualizer_scheme.py
+drwxrwxrwx   0        0        0        0 2024-05-05 13:46:53.716244 mkt-retv-1.415/market_research/scraper/models/
+-rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.415/market_research/scraper/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 13:46:53.716244 mkt-retv-1.415/market_research/scraper/models/lge/
+-rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.415/market_research/scraper/models/lge/__init__.py
+-rw-rw-rw-   0        0        0    12830 2024-05-05 13:45:10.000000 mkt-retv-1.415/market_research/scraper/models/lge/spec_l.py
+drwxrwxrwx   0        0        0        0 2024-05-05 13:46:53.726100 mkt-retv-1.415/market_research/scraper/models/pana/
+-rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.415/market_research/scraper/models/pana/__init__.py
+-rw-rw-rw-   0        0        0     6868 2024-05-05 13:45:10.000000 mkt-retv-1.415/market_research/scraper/models/pana/spec_p.py
+-rw-rw-rw-   0        0        0    12938 2024-05-05 13:45:10.000000 mkt-retv-1.415/market_research/scraper/models/pana/spec_pjp.py
+drwxrwxrwx   0        0        0        0 2024-05-05 13:46:53.734269 mkt-retv-1.415/market_research/scraper/models/sony/
+-rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.415/market_research/scraper/models/sony/__init__.py
+-rw-rw-rw-   0        0        0     5267 2024-05-05 05:49:12.000000 mkt-retv-1.415/market_research/scraper/models/sony/cleanup_s.py
+-rw-rw-rw-   0        0        0    10590 2024-05-05 13:45:10.000000 mkt-retv-1.415/market_research/scraper/models/sony/sepc_sjp.py
+-rw-rw-rw-   0        0        0    12370 2024-05-05 13:45:10.000000 mkt-retv-1.415/market_research/scraper/models/sony/spec_s.py
+-rw-rw-rw-   0        0        0     4387 2024-05-05 00:51:17.000000 mkt-retv-1.415/market_research/scraper/models/sony/visualizer_s.py
+drwxrwxrwx   0        0        0        0 2024-05-05 13:46:53.734269 mkt-retv-1.415/market_research/scraper/rtings/
+-rw-rw-rw-   0        0        0      106 2023-11-19 08:24:51.000000 mkt-retv-1.415/market_research/scraper/rtings/__init__.py
+-rw-rw-rw-   0        0        0    10290 2023-11-23 09:57:43.000000 mkt-retv-1.415/market_research/scraper/rtings/rtings.py
+-rw-rw-rw-   0        0        0     6309 2023-11-26 10:28:52.000000 mkt-retv-1.415/market_research/scraper/rtings/rurlsearcher.py
+-rw-rw-rw-   0        0        0    13793 2023-11-23 12:05:59.000000 mkt-retv-1.415/market_research/scraper/rtings/rvisualizer.py
+drwxrwxrwx   0        0        0        0 2024-05-05 13:46:53.744319 mkt-retv-1.415/market_research/tools/
+-rw-rw-rw-   0        0        0      206 2023-11-16 08:38:53.000000 mkt-retv-1.415/market_research/tools/__init__.py
+-rw-rw-rw-   0        0        0     1003 2023-11-18 14:03:46.000000 mkt-retv-1.415/market_research/tools/aimanager.py
+-rw-rw-rw-   0        0        0     3371 2023-11-19 12:13:44.000000 mkt-retv-1.415/market_research/tools/filemanager.py
+-rw-rw-rw-   0        0        0     3818 2023-11-14 14:05:22.000000 mkt-retv-1.415/market_research/tools/installer.py
+-rw-rw-rw-   0        0        0     5509 2023-11-15 11:16:47.000000 mkt-retv-1.415/market_research/tools/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-05-05 13:46:53.791961 mkt-retv-1.415/mkt_retv.egg-info/
+-rw-rw-rw-   0        0        0      697 2024-05-05 13:46:53.000000 mkt-retv-1.415/mkt_retv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1443 2024-05-05 13:46:53.000000 mkt-retv-1.415/mkt_retv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 13:46:53.000000 mkt-retv-1.415/mkt_retv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-05-05 13:46:53.000000 mkt-retv-1.415/mkt_retv.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      129 2024-05-05 13:46:53.000000 mkt-retv-1.415/mkt_retv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-05 13:46:53.000000 mkt-retv-1.415/mkt_retv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-05 13:46:53.812066 mkt-retv-1.415/setup.cfg
+-rw-rw-rw-   0        0        0      959 2024-05-05 13:46:48.000000 mkt-retv-1.415/setup.py
```

### Comparing `mkt-retv-1.414/PKG-INFO` & `mkt-retv-1.415/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkt-retv
-Version: 1.414
+Version: 1.415
 Summary: market research TV 
 Home-page: https://github.com/xikest/research_market_tv
 Author: xikest
 Project-URL: Source, https://github.com/xikest/research_market_tv
 Project-URL: Bug Tracker, https://github.com/xikest/research_market_tv/issues
 Requires-Python: >=3.7
 Requires-Dist: numpy
```

### Comparing `mkt-retv-1.414/README.md` & `mkt-retv-1.415/README.md`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.414/market_research/analysis/_analysis_scheme.py` & `mkt-retv-1.415/market_research/analysis/_analysis_scheme.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.414/market_research/analysis/imgemanger.py` & `mkt-retv-1.415/market_research/analysis/imgemanger.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.414/market_research/analysis/sentimentmanager.py` & `mkt-retv-1.415/market_research/analysis/sentimentmanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.414/market_research/analysis/textmanager.py` & `mkt-retv-1.415/market_research/analysis/textmanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.414/market_research/scraper/__init__.py` & `mkt-retv-1.415/market_research/scraper/__init__.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.414/market_research/scraper/_scaper_scheme.py` & `mkt-retv-1.415/market_research/scraper/_scaper_scheme.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.414/market_research/scraper/models/lge/spec_l.py` & `mkt-retv-1.415/market_research/scraper/models/lge/spec_l.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from tqdm import tqdm
 import re
 from selenium.webdriver.common.by import By
 from market_research.tools import FileManager
 from market_research.scraper._scaper_scheme import Scraper
 
 
+
+
 class ModelScraper_l(Scraper):
     def __init__(self, enable_headless=True,
                  export_prefix="sony_model_info_web", intput_folder_path="input", output_folder_path="results",
                  verbose: bool = False, wait_time=2):
 
         super().__init__(enable_headless=enable_headless, export_prefix=export_prefix,
                          intput_folder_path=intput_folder_path, output_folder_path=output_folder_path)
@@ -34,25 +36,29 @@
         print("number of total model:", len(url_series_dict))
         if fastmode:
             model_list = list(url_series_dict.keys())
             return model_list
         print("collecting spec")
         visit_url_dict = {}
         dict_models = {}
-        for key, url_model in tqdm(url_series_dict.items()):
-            try:
-                dict_info = self._get_model_info(url_model)
-                dict_models[key] = dict_info
-                dict_spec = self._get_global_spec(url=url_model)
-                dict_models[key].update(dict_spec)
-                visit_url_dict[key] = url_model
-            except Exception as e:
-                print(f"Failed to get info from {key}")
-                print(e)
-                pass
+        cnt_loop=2
+        for cnt in range(cnt_loop):#main try
+            for key, url_model in tqdm(url_series_dict.items()):
+                try:
+                    dict_info = self._get_model_info(url_model)
+                    dict_models[key] = dict_info
+                    dict_spec = self._get_global_spec(url=url_model)
+                    dict_models[key].update(dict_spec)
+                    visit_url_dict[key] = url_model
+                except Exception as e:
+                    if cnt == cnt_loop:
+                        print(f"\nFailed to get info from {key}")
+                        print(e)
+                    pass
+            break
         print("\n")
         for model, url in visit_url_dict.items():  print(f"{model}: {url}")
 
         if format_df:
             df_models = pd.DataFrame.from_dict(dict_models).T
             FileManager.df_to_excel(df_models.reset_index(), file_name=self.output_xlsx_name, sheet_name="raw_na",
                                     mode='w')
```

### Comparing `mkt-retv-1.414/market_research/scraper/models/pana/spec_p.py` & `mkt-retv-1.415/market_research/scraper/models/pana/spec_p.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,24 +16,34 @@
         self.wait_time = wait_time
 
 
     def get_models_info(self, foramt_output="df"):
         print("collecting models")
         setUrlSeries = self._get_spec_series()
         ## 웹페이지의 모든 모델 url을 추출
+        print("collecting spec")
         visit_url_dict = {}
         dictModels = OrderedDict()
-        print("collecting spec")
-        for model, url in tqdm(setUrlSeries.items()):
-            # print(model,":", url)
-            modelspec = self._get_spec_global(url=url)
-            modelspec["url"] = url
-            dictModels[model] = modelspec
+        cnt_loop=2
+        for cnt in range(cnt_loop):#main try
+            for model, url in tqdm(setUrlSeries.items()):
+                try:
+                    # print(model,":", url)
+                    modelspec = self._get_spec_global(url=url)
+                    modelspec["url"] = url
+                    dictModels[model] = modelspec
 
-            visit_url_dict[model] = url
+                    visit_url_dict[model] = url
+                except Exception as e:
+                    if cnt == cnt_loop:
+                        print(f"\nFailed to get info from {model}")
+                        print(e)
+                    pass
+            break
+        print("\n")
         for model, url in visit_url_dict.items():  print(f"{model}: {url}")
         # print("Number of all Series:", len(dictModels))
 
         if foramt_output == "df":
             df_models = pd.DataFrame.from_dict(dictModels).T
             FileManager.df_to_excel(df_models.reset_index(), file_name=self.output_xlsx_name, sheet_name="raw_na", mode='w')
             return df_models
```

### Comparing `mkt-retv-1.414/market_research/scraper/models/pana/spec_pjp.py` & `mkt-retv-1.415/market_research/scraper/models/pana/spec_pjp.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,18 +25,28 @@
         specs_dict = {}
         url_model_dict = self._get_model_series(step=1000)
         print("collecting models")
         for model, url in tqdm(url_model_dict.items()):
             specs_dict.update(self._get_spec_series(url=url,step=3000))
         print("collecting spec")
         visit_url_dict = {}
-        for model, url in tqdm(specs_dict.items()):
-            visit_url_dict[model] = url
-            modelspec = self._get_spec(model = model, url=url)
-            models_dict[model] = modelspec
+        cnt_loop=2
+        for cnt in range(cnt_loop):#main try
+            for model, url in tqdm(specs_dict.items()):
+                try:
+                    visit_url_dict[model] = url
+                    modelspec = self._get_spec(model = model, url=url)
+                    models_dict[model] = modelspec
+                except Exception as e:
+                    if cnt == cnt_loop:
+                        print(f"\nFailed to get info from {model}")
+                        print(e)
+                    pass
+            break
+        print("\n")
         for model, url in visit_url_dict.items(): print(f"{model}: {url}")
 
         if foramt_output == "df":
             df_models = pd.DataFrame.from_dict(models_dict).T
             FileManager.df_to_excel(df_models.reset_index(), file_name=self.output_xlsx_name, sheet_name="raw_jp", mode='w')
             return df_models
         else:
```

### Comparing `mkt-retv-1.414/market_research/scraper/models/sony/cleanup_s.py` & `mkt-retv-1.415/market_research/scraper/models/sony/cleanup_s.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.414/market_research/scraper/models/sony/sepc_sjp.py` & `mkt-retv-1.415/market_research/scraper/models/sony/sepc_sjp.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,22 +18,31 @@
         self.wait_time = wait_time
         self.file_manager = FileManager
 
 
     def get_models_info(self, foramt_output="df"):
         print("collecting models")
         url_series_dict = self._get_spec_series()
+        print("collecting spec")
         models_dict = {}
         visit_url_dict = {}
-        print("collecting spec")
-        for model, url in tqdm(url_series_dict.items()):
-            # print(f"{model}: {url}")
-            modelspec = self._get_spec(url=url)
-            models_dict.update(modelspec)
-            visit_url_dict[model] = url
+        cnt_loop=2
+        for cnt in range(cnt_loop):#main try
+            for model, url in tqdm(url_series_dict.items()):
+                try:
+                    # print(f"{model}: {url}")
+                    modelspec = self._get_spec(url=url)
+                    models_dict.update(modelspec)
+                    visit_url_dict[model] = url
+                except Exception as e:
+                    if cnt == cnt_loop:
+                        print(f"\nFailed to get info from {model}")
+                        print(e)
+                    pass
+        print("\n")
         for model, url in visit_url_dict.items():  print(f"{model}: {url}")
         # print("Number of all Series:", len(models_dict))
 
         if foramt_output == "df":
             df_models = pd.DataFrame.from_dict(models_dict).T
             FileManager.df_to_excel(df_models.reset_index(), file_name=self.output_xlsx_name, sheet_name="raw_na", mode='w')
             return df_models
```

### Comparing `mkt-retv-1.414/market_research/scraper/models/sony/spec_s.py` & `mkt-retv-1.415/market_research/scraper/models/sony/spec_s.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,26 +33,29 @@
         print("number of total model:", len(url_series_dict))
         if fastmode:
             model_list = list(url_series_dict.keys())
             return model_list
         print("collecting spec")
         visit_url_dict = {}
         dict_models = {}
-        for key, url_model in tqdm(url_series_dict.items()):
-            try:
-                dict_info = self._get_model_info(url_model)
-                dict_models[key] = dict_info
-                dict_spec = self._get_global_spec(url=url_model)
-                dict_models[key].update(dict_spec)
-                visit_url_dict[key] = url_model
-            except Exception as e:
-                print(f"Failed to get info from {key}")
-                print(e)
-                pass
-
+        cnt_loop=2
+        for cnt in range(cnt_loop):#main try
+            for key, url_model in tqdm(url_series_dict.items()):
+                try:
+                    dict_info = self._get_model_info(url_model)
+                    dict_models[key] = dict_info
+                    dict_spec = self._get_global_spec(url=url_model)
+                    dict_models[key].update(dict_spec)
+                    visit_url_dict[key] = url_model
+                except Exception as e:
+                    if cnt == cnt_loop:
+                        print(f"\nFailed to get info from {key}")
+                        print(e)
+                    pass
+        print("\n")
         for model, url in visit_url_dict.items():  print(f"{model}: {url}")
 
         if format_df:
             df_models = pd.DataFrame.from_dict(dict_models).T
             if temporary_year_marking:
                 df_models['year'] = df_models['year'].fillna("2024") ## 임시
             FileManager.df_to_excel(df_models.reset_index(), file_name=self.output_xlsx_name, sheet_name="raw_na", mode='w')
```

### Comparing `mkt-retv-1.414/market_research/scraper/models/sony/visualizer_s.py` & `mkt-retv-1.415/market_research/scraper/models/sony/visualizer_s.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.414/market_research/scraper/rtings/rtings.py` & `mkt-retv-1.415/market_research/scraper/rtings/rtings.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.414/market_research/scraper/rtings/rurlsearcher.py` & `mkt-retv-1.415/market_research/scraper/rtings/rurlsearcher.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.414/market_research/scraper/rtings/rvisualizer.py` & `mkt-retv-1.415/market_research/scraper/rtings/rvisualizer.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.414/market_research/tools/aimanager.py` & `mkt-retv-1.415/market_research/tools/aimanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.414/market_research/tools/filemanager.py` & `mkt-retv-1.415/market_research/tools/filemanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.414/market_research/tools/installer.py` & `mkt-retv-1.415/market_research/tools/installer.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.414/market_research/tools/webdriver.py` & `mkt-retv-1.415/market_research/tools/webdriver.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.414/mkt_retv.egg-info/PKG-INFO` & `mkt-retv-1.415/mkt_retv.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkt-retv
-Version: 1.414
+Version: 1.415
 Summary: market research TV 
 Home-page: https://github.com/xikest/research_market_tv
 Author: xikest
 Project-URL: Source, https://github.com/xikest/research_market_tv
 Project-URL: Bug Tracker, https://github.com/xikest/research_market_tv/issues
 Requires-Python: >=3.7
 Requires-Dist: numpy
```

### Comparing `mkt-retv-1.414/mkt_retv.egg-info/SOURCES.txt` & `mkt-retv-1.415/mkt_retv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.414/setup.py` & `mkt-retv-1.415/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mkt-retv',
-    version='1.414',
+    version='1.415',
     author='xikest',
     description='market research TV ',
     packages=find_packages(),
     python_requires='>=3.7',
     install_requires=[
         'numpy', 'pandas',
         'selenium','beautifulsoup4','requests',
```

