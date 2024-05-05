# Comparing `tmp/PKNSETools-0.1.20240421.94.tar.gz` & `tmp/PKNSETools-0.1.20240505.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKNSETools-0.1.20240421.94.tar", last modified: Sun Apr 21 23:06:16 2024, max compression
+gzip compressed data, was "PKNSETools-0.1.20240505.96.tar", last modified: Sun May  5 06:18:50 2024, max compression
```

## Comparing `PKNSETools-0.1.20240421.94.tar` & `PKNSETools-0.1.20240505.96.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 23:06:16.276698 PKNSETools-0.1.20240421.94/
--rw-rw-rw-   0        0        0     2661 2024-04-21 23:06:16.276698 PKNSETools-0.1.20240421.94/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-21 23:06:16.261072 PKNSETools-0.1.20240421.94/PKNSETools/
-drwxrwxrwx   0        0        0        0 2024-04-21 23:06:16.261072 PKNSETools-0.1.20240421.94/PKNSETools/Benny/
--rw-rw-rw-   0        0        0    34274 2024-04-21 23:04:19.000000 PKNSETools-0.1.20240421.94/PKNSETools/Benny/NSE.py
--rw-rw-rw-   0        0        0     1198 2024-04-21 23:04:19.000000 PKNSETools-0.1.20240421.94/PKNSETools/Benny/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 23:06:16.261072 PKNSETools-0.1.20240421.94/PKNSETools/Nasdaq/
--rw-rw-rw-   0        0        0     3392 2024-04-21 23:04:19.000000 PKNSETools-0.1.20240421.94/PKNSETools/Nasdaq/PKNasdaqIndex.py
--rw-rw-rw-   0        0        0     1225 2024-04-21 23:04:19.000000 PKNSETools-0.1.20240421.94/PKNSETools/Nasdaq/__init__.py
--rw-rw-rw-   0        0        0     4806 2024-04-21 23:04:19.000000 PKNSETools-0.1.20240421.94/PKNSETools/PKAllStocks.py
--rw-rw-rw-   0        0        0    10032 2024-04-21 23:04:19.000000 PKNSETools-0.1.20240421.94/PKNSETools/PKCompanyGeneral.py
--rw-rw-rw-   0        0        0     3303 2024-04-21 23:04:19.000000 PKNSETools-0.1.20240421.94/PKNSETools/PKCompanyStock.py
--rw-rw-rw-   0        0        0     2223 2024-04-21 23:04:19.000000 PKNSETools-0.1.20240421.94/PKNSETools/PKConstants.py
--rw-rw-rw-   0        0        0     5168 2024-04-21 23:04:19.000000 PKNSETools-0.1.20240421.94/PKNSETools/PKIntraDay.py
--rw-rw-rw-   0        0        0     6446 2024-04-21 23:04:19.000000 PKNSETools-0.1.20240421.94/PKNSETools/PKMultiProcessorClient.py
--rw-rw-rw-   0        0        0    12688 2024-04-21 23:04:19.000000 PKNSETools-0.1.20240421.94/PKNSETools/PKNSEStockDataFetcher.py
--rw-rw-rw-   0        0        0       30 2024-04-21 23:06:11.000000 PKNSETools-0.1.20240421.94/PKNSETools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 23:06:16.276698 PKNSETools-0.1.20240421.94/PKNSETools/morningstartools/
--rw-rw-rw-   0        0        0     1830 2024-04-21 23:04:19.000000 PKNSETools-0.1.20240421.94/PKNSETools/morningstartools/NSEStockDB.py
--rw-rw-rw-   0        0        0     1848 2024-04-21 23:04:19.000000 PKNSETools-0.1.20240421.94/PKNSETools/morningstartools/NSEStockFairValueDB.py
--rw-rw-rw-   0        0        0     1836 2024-04-21 23:04:19.000000 PKNSETools-0.1.20240421.94/PKNSETools/morningstartools/NSEStockMFIDB.py
--rw-rw-rw-   0        0        0    61965 2024-04-21 23:04:19.000000 PKNSETools-0.1.20240421.94/PKNSETools/morningstartools/PKMorningstarDataFetcher.py
--rw-rw-rw-   0        0        0     1378 2024-04-21 23:04:19.000000 PKNSETools-0.1.20240421.94/PKNSETools/morningstartools/__init__.py
--rw-rw-rw-   0        0        0     2000 2024-04-21 23:04:19.000000 PKNSETools-0.1.20240421.94/PKNSETools/morningstartools/error.py
--rw-rw-rw-   0        0        0    40060 2024-04-21 23:04:19.000000 PKNSETools-0.1.20240421.94/PKNSETools/morningstartools/funds.py
--rw-rw-rw-   0        0        0    22038 2024-04-21 23:04:19.000000 PKNSETools-0.1.20240421.94/PKNSETools/morningstartools/search.py
--rw-rw-rw-   0        0        0    13495 2024-04-21 23:04:19.000000 PKNSETools-0.1.20240421.94/PKNSETools/morningstartools/security.py
--rw-rw-rw-   0        0        0    29930 2024-04-21 23:04:19.000000 PKNSETools-0.1.20240421.94/PKNSETools/morningstartools/stock.py
--rw-rw-rw-   0        0        0    23246 2024-04-21 23:04:19.000000 PKNSETools-0.1.20240421.94/PKNSETools/morningstartools/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-21 23:06:16.261072 PKNSETools-0.1.20240421.94/PKNSETools.egg-info/
--rw-rw-rw-   0        0        0     2661 2024-04-21 23:06:16.000000 PKNSETools-0.1.20240421.94/PKNSETools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1041 2024-04-21 23:06:16.000000 PKNSETools-0.1.20240421.94/PKNSETools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 23:06:16.000000 PKNSETools-0.1.20240421.94/PKNSETools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-21 23:06:09.000000 PKNSETools-0.1.20240421.94/PKNSETools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       79 2024-04-21 23:06:16.000000 PKNSETools-0.1.20240421.94/PKNSETools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-21 23:06:16.000000 PKNSETools-0.1.20240421.94/PKNSETools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1884 2024-04-21 23:04:19.000000 PKNSETools-0.1.20240421.94/README.md
--rw-rw-rw-   0        0        0       86 2024-04-21 23:06:16.276698 PKNSETools-0.1.20240421.94/setup.cfg
--rw-rw-rw-   0        0        0     3832 2024-04-21 23:04:19.000000 PKNSETools-0.1.20240421.94/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 06:18:50.313278 PKNSETools-0.1.20240505.96/
+-rw-rw-rw-   0        0        0     2661 2024-05-05 06:18:50.313278 PKNSETools-0.1.20240505.96/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-05 06:18:50.297650 PKNSETools-0.1.20240505.96/PKNSETools/
+drwxrwxrwx   0        0        0        0 2024-05-05 06:18:50.297650 PKNSETools-0.1.20240505.96/PKNSETools/Benny/
+-rw-rw-rw-   0        0        0    34274 2024-05-05 06:16:43.000000 PKNSETools-0.1.20240505.96/PKNSETools/Benny/NSE.py
+-rw-rw-rw-   0        0        0     1198 2024-05-05 06:16:43.000000 PKNSETools-0.1.20240505.96/PKNSETools/Benny/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 06:18:50.297650 PKNSETools-0.1.20240505.96/PKNSETools/Nasdaq/
+-rw-rw-rw-   0        0        0     3386 2024-05-05 06:16:43.000000 PKNSETools-0.1.20240505.96/PKNSETools/Nasdaq/PKNasdaqIndex.py
+-rw-rw-rw-   0        0        0     1225 2024-05-05 06:16:43.000000 PKNSETools-0.1.20240505.96/PKNSETools/Nasdaq/__init__.py
+-rw-rw-rw-   0        0        0     4806 2024-05-05 06:16:43.000000 PKNSETools-0.1.20240505.96/PKNSETools/PKAllStocks.py
+-rw-rw-rw-   0        0        0    10032 2024-05-05 06:16:43.000000 PKNSETools-0.1.20240505.96/PKNSETools/PKCompanyGeneral.py
+-rw-rw-rw-   0        0        0     3303 2024-05-05 06:16:43.000000 PKNSETools-0.1.20240505.96/PKNSETools/PKCompanyStock.py
+-rw-rw-rw-   0        0        0     2223 2024-05-05 06:16:43.000000 PKNSETools-0.1.20240505.96/PKNSETools/PKConstants.py
+-rw-rw-rw-   0        0        0     5168 2024-05-05 06:16:43.000000 PKNSETools-0.1.20240505.96/PKNSETools/PKIntraDay.py
+-rw-rw-rw-   0        0        0     6446 2024-05-05 06:16:43.000000 PKNSETools-0.1.20240505.96/PKNSETools/PKMultiProcessorClient.py
+-rw-rw-rw-   0        0        0    12688 2024-05-05 06:16:43.000000 PKNSETools-0.1.20240505.96/PKNSETools/PKNSEStockDataFetcher.py
+-rw-rw-rw-   0        0        0       30 2024-05-05 06:18:45.000000 PKNSETools-0.1.20240505.96/PKNSETools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 06:18:50.313278 PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/
+-rw-rw-rw-   0        0        0     1830 2024-05-05 06:16:43.000000 PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/NSEStockDB.py
+-rw-rw-rw-   0        0        0     1848 2024-05-05 06:16:43.000000 PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/NSEStockFairValueDB.py
+-rw-rw-rw-   0        0        0     1836 2024-05-05 06:16:44.000000 PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/NSEStockMFIDB.py
+-rw-rw-rw-   0        0        0    61961 2024-05-05 06:16:44.000000 PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/PKMorningstarDataFetcher.py
+-rw-rw-rw-   0        0        0     1378 2024-05-05 06:16:44.000000 PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/__init__.py
+-rw-rw-rw-   0        0        0     2000 2024-05-05 06:16:44.000000 PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/error.py
+-rw-rw-rw-   0        0        0    40060 2024-05-05 06:16:44.000000 PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/funds.py
+-rw-rw-rw-   0        0        0    22038 2024-05-05 06:16:44.000000 PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/search.py
+-rw-rw-rw-   0        0        0    13495 2024-05-05 06:16:44.000000 PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/security.py
+-rw-rw-rw-   0        0        0    29916 2024-05-05 06:16:44.000000 PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/stock.py
+-rw-rw-rw-   0        0        0    23246 2024-05-05 06:16:44.000000 PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-05 06:18:50.297650 PKNSETools-0.1.20240505.96/PKNSETools.egg-info/
+-rw-rw-rw-   0        0        0     2661 2024-05-05 06:18:50.000000 PKNSETools-0.1.20240505.96/PKNSETools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1041 2024-05-05 06:18:50.000000 PKNSETools-0.1.20240505.96/PKNSETools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 06:18:50.000000 PKNSETools-0.1.20240505.96/PKNSETools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-05 06:18:43.000000 PKNSETools-0.1.20240505.96/PKNSETools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       79 2024-05-05 06:18:50.000000 PKNSETools-0.1.20240505.96/PKNSETools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-05 06:18:50.000000 PKNSETools-0.1.20240505.96/PKNSETools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1884 2024-05-05 06:16:44.000000 PKNSETools-0.1.20240505.96/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-05 06:18:50.313278 PKNSETools-0.1.20240505.96/setup.cfg
+-rw-rw-rw-   0        0        0     3832 2024-05-05 06:16:44.000000 PKNSETools-0.1.20240505.96/setup.py
```

### Comparing `PKNSETools-0.1.20240421.94/PKG-INFO` & `PKNSETools-0.1.20240505.96/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKNSETools
-Version: 0.1.20240421.94
+Version: 0.1.20240505.96
 Summary: A Python-based data downloader for NSE, India
 Home-page: https://github.com/pkjmesra/PKNSETools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240421.94.zip
+Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240505.96.zip
 Keywords: NSE,Stocks,Data Download
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKNSETools-0.1.20240421.94/PKNSETools/Benny/NSE.py` & `PKNSETools-0.1.20240505.96/PKNSETools/Benny/NSE.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240421.94/PKNSETools/Benny/__init__.py` & `PKNSETools-0.1.20240505.96/PKNSETools/Benny/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240421.94/PKNSETools/Nasdaq/PKNasdaqIndex.py` & `PKNSETools-0.1.20240505.96/PKNSETools/Nasdaq/PKNasdaqIndex.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             default_logger().debug(e, exc_info=True)
         return listStockCodes
 
     def refreshTokens(self):
             if self.cookieHelper is None:
                 self.cookieHelper = CookieHelper(download_folder=Archiver.get_user_outputs_dir(),
                                                     baseCookieUrl="https://www.nasdaq.com/market-activity/stocks/screener",
-                                                    cookieStoreName="nasdaq",
+                                                    cookieStoreName="nda",
                                                     baseHtmlUrl="https://www.nasdaq.com/market-activity/stocks/screener",
-                                                    htmlStoreName="nasdaq")
+                                                    htmlStoreName="nda")
             else:
                 self.cookieHelper.resetCookies()
                 self.cookieHelper.resetMetas()
             self.session.cookies.update(self.cookieHelper.cookies)
             self.defaultCookies = self.cookieHelper.cookies
```

### Comparing `PKNSETools-0.1.20240421.94/PKNSETools/Nasdaq/__init__.py` & `PKNSETools-0.1.20240505.96/PKNSETools/Nasdaq/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240421.94/PKNSETools/PKAllStocks.py` & `PKNSETools-0.1.20240505.96/PKNSETools/PKAllStocks.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240421.94/PKNSETools/PKCompanyGeneral.py` & `PKNSETools-0.1.20240505.96/PKNSETools/PKCompanyGeneral.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240421.94/PKNSETools/PKCompanyStock.py` & `PKNSETools-0.1.20240505.96/PKNSETools/PKCompanyStock.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240421.94/PKNSETools/PKConstants.py` & `PKNSETools-0.1.20240505.96/PKNSETools/PKConstants.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240421.94/PKNSETools/PKIntraDay.py` & `PKNSETools-0.1.20240505.96/PKNSETools/PKIntraDay.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240421.94/PKNSETools/PKMultiProcessorClient.py` & `PKNSETools-0.1.20240505.96/PKNSETools/PKMultiProcessorClient.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240421.94/PKNSETools/PKNSEStockDataFetcher.py` & `PKNSETools-0.1.20240505.96/PKNSETools/PKNSEStockDataFetcher.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240421.94/PKNSETools/morningstartools/NSEStockDB.py` & `PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/NSEStockDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240421.94/PKNSETools/morningstartools/NSEStockFairValueDB.py` & `PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/NSEStockFairValueDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240421.94/PKNSETools/morningstartools/NSEStockMFIDB.py` & `PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/NSEStockMFIDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240421.94/PKNSETools/morningstartools/PKMorningstarDataFetcher.py` & `PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/PKMorningstarDataFetcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -300,17 +300,17 @@
             "Host": "www.barodaetrade.com",
             "Referer": "https://www.barodaetrade.com/Markettracker/Dividend_Declared",
             "Upgrade-Insecure-Requests": "1",
             "User-Agent": random_user_agent()
         }
         cookieHelper = CookieHelper(download_folder=Archiver.get_user_outputs_dir(),
                                                  baseCookieUrl="https://www.barodaetrade.com/Markettracker/Dividend_Declared",
-                                                 cookieStoreName="bobcaps",
+                                                 cookieStoreName="bcaps",
                                                  baseHtmlUrl="https://www.barodaetrade.com/Markettracker/Dividend_Declared",
-                                                 htmlStoreName="bobcaps")
+                                                 htmlStoreName="bcaps")
         self.session.headers.update(default_headers)
         self.session.cookies.update(cookieHelper.cookies)
 
     def getCorporateActions(self):
         self.refreshBobCapsTokens()
         dividends_df = pd.DataFrame([{"Company Name":""}])
         bonus_df = pd.DataFrame([{"Company Name":""}])
```

### Comparing `PKNSETools-0.1.20240421.94/PKNSETools/morningstartools/__init__.py` & `PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240421.94/PKNSETools/morningstartools/error.py` & `PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/error.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240421.94/PKNSETools/morningstartools/funds.py` & `PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/funds.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240421.94/PKNSETools/morningstartools/search.py` & `PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/search.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240421.94/PKNSETools/morningstartools/security.py` & `PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/security.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240421.94/PKNSETools/morningstartools/stock.py` & `PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/stock.py`

 * *Files 0% similar despite different names*

```diff
@@ -707,17 +707,17 @@
                 pass
         return {"latestFairValue":fv} if fv is not None else fv
 
     def refreshMorningstarTokens(self, params, headers):
         if self.cookieHelper is None:
             self.cookieHelper = CookieHelper(download_folder=Archiver.get_user_outputs_dir(),
                                                  baseCookieUrl="https://morningstar.in/stocks/0p0000c3nz/nse-hdfc-bank-ltd/overview.aspx",
-                                                 cookieStoreName="morningstar",
+                                                 cookieStoreName="msta",
                                                  baseHtmlUrl="https://morningstar.in/stocks/0p0000c3nz/nse-hdfc-bank-ltd/overview.aspx",
-                                                 htmlStoreName="morningstar")
+                                                 htmlStoreName="msta")
         else:
             self.cookieHelper.resetCookies()
             self.cookieHelper.resetMetas()
         params["access_token"] = self.cookieHelper.html_metas["accessToken"]
         headers["X-Api-Realtime-E"] = self.cookieHelper.html_metas["realTimeToken"]
         self.fetcher.session.cookies.update(self.cookieHelper.cookies)
         self.defaultCookies = self.cookieHelper.cookies
```

### Comparing `PKNSETools-0.1.20240421.94/PKNSETools/morningstartools/utils.py` & `PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/utils.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240421.94/PKNSETools.egg-info/PKG-INFO` & `PKNSETools-0.1.20240505.96/PKNSETools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKNSETools
-Version: 0.1.20240421.94
+Version: 0.1.20240505.96
 Summary: A Python-based data downloader for NSE, India
 Home-page: https://github.com/pkjmesra/PKNSETools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240421.94.zip
+Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240505.96.zip
 Keywords: NSE,Stocks,Data Download
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKNSETools-0.1.20240421.94/PKNSETools.egg-info/SOURCES.txt` & `PKNSETools-0.1.20240505.96/PKNSETools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240421.94/README.md` & `PKNSETools-0.1.20240505.96/README.md`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240421.94/setup.py` & `PKNSETools-0.1.20240505.96/setup.py`

 * *Files identical despite different names*

