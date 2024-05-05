# Comparing `tmp/pkscreener-0.44.20240504.333.tar.gz` & `tmp/pkscreener-0.44.20240505.334.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240504.333.tar", last modified: Sat May  4 08:16:15 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240505.334.tar", last modified: Sun May  5 06:48:31 2024, max compression
```

## Comparing `pkscreener-0.44.20240504.333.tar` & `pkscreener-0.44.20240505.334.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 08:16:15.555037 pkscreener-0.44.20240504.333/
--rw-rw-rw-   0        0        0     1086 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-04 08:16:15.555037 pkscreener-0.44.20240504.333/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 08:16:15.539412 pkscreener-0.44.20240504.333/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 08:16:15.555037 pkscreener-0.44.20240504.333/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    25810 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     7690 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    29461 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    22090 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    21218 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8158 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18443 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   119213 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    52127 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    82053 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-04 08:16:04.000000 pkscreener-0.44.20240504.333/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   124183 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/globals.py
--rw-rw-rw-   0        0        0      595 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    42912 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    26410 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-04 08:16:15.539412 pkscreener-0.44.20240504.333/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-04 08:16:15.000000 pkscreener-0.44.20240504.333/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-04 08:16:15.000000 pkscreener-0.44.20240504.333/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 08:16:15.000000 pkscreener-0.44.20240504.333/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-04 08:16:15.000000 pkscreener-0.44.20240504.333/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-04 08:16:15.000000 pkscreener-0.44.20240504.333/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-04 08:16:15.000000 pkscreener-0.44.20240504.333/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-04 08:16:15.555037 pkscreener-0.44.20240504.333/setup.cfg
--rw-rw-rw-   0        0        0     4727 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 06:48:31.971868 pkscreener-0.44.20240505.334/
+-rw-rw-rw-   0        0        0     1086 2024-05-05 06:44:22.000000 pkscreener-0.44.20240505.334/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-05 06:44:22.000000 pkscreener-0.44.20240505.334/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-05 06:48:31.971868 pkscreener-0.44.20240505.334/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-05 06:44:22.000000 pkscreener-0.44.20240505.334/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 06:48:31.956242 pkscreener-0.44.20240505.334/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-05 06:44:22.000000 pkscreener-0.44.20240505.334/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 06:48:31.971868 pkscreener-0.44.20240505.334/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-05 06:44:22.000000 pkscreener-0.44.20240505.334/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-05 06:44:22.000000 pkscreener-0.44.20240505.334/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-05 06:44:22.000000 pkscreener-0.44.20240505.334/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-05 06:44:22.000000 pkscreener-0.44.20240505.334/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-05-05 06:44:22.000000 pkscreener-0.44.20240505.334/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    26892 2024-05-05 06:44:22.000000 pkscreener-0.44.20240505.334/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-05 06:44:22.000000 pkscreener-0.44.20240505.334/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     7857 2024-05-05 06:44:22.000000 pkscreener-0.44.20240505.334/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-05 06:44:22.000000 pkscreener-0.44.20240505.334/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    29489 2024-05-05 06:44:22.000000 pkscreener-0.44.20240505.334/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-05-05 06:44:22.000000 pkscreener-0.44.20240505.334/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    22090 2024-05-05 06:44:22.000000 pkscreener-0.44.20240505.334/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    21218 2024-05-05 06:44:22.000000 pkscreener-0.44.20240505.334/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-05 06:44:22.000000 pkscreener-0.44.20240505.334/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8158 2024-05-05 06:44:22.000000 pkscreener-0.44.20240505.334/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-05 06:44:22.000000 pkscreener-0.44.20240505.334/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-05 06:44:22.000000 pkscreener-0.44.20240505.334/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18443 2024-05-05 06:44:22.000000 pkscreener-0.44.20240505.334/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-05 06:44:22.000000 pkscreener-0.44.20240505.334/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-05 06:44:22.000000 pkscreener-0.44.20240505.334/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   119213 2024-05-05 06:44:22.000000 pkscreener-0.44.20240505.334/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    52127 2024-05-05 06:44:22.000000 pkscreener-0.44.20240505.334/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-05-05 06:44:22.000000 pkscreener-0.44.20240505.334/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    82261 2024-05-05 06:44:22.000000 pkscreener-0.44.20240505.334/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-05-05 06:44:22.000000 pkscreener-0.44.20240505.334/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-05 06:48:24.000000 pkscreener-0.44.20240505.334/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-05-05 06:44:22.000000 pkscreener-0.44.20240505.334/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-05 06:44:22.000000 pkscreener-0.44.20240505.334/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   124696 2024-05-05 06:44:22.000000 pkscreener-0.44.20240505.334/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      867 2024-05-05 06:44:23.000000 pkscreener-0.44.20240505.334/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    42917 2024-05-05 06:44:23.000000 pkscreener-0.44.20240505.334/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    26476 2024-05-05 06:44:23.000000 pkscreener-0.44.20240505.334/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-05 06:48:31.956242 pkscreener-0.44.20240505.334/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-05 06:48:31.000000 pkscreener-0.44.20240505.334/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-05 06:48:31.000000 pkscreener-0.44.20240505.334/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 06:48:31.000000 pkscreener-0.44.20240505.334/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-05 06:48:31.000000 pkscreener-0.44.20240505.334/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-05 06:48:31.000000 pkscreener-0.44.20240505.334/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-05 06:48:31.000000 pkscreener-0.44.20240505.334/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-05 06:48:31.971868 pkscreener-0.44.20240505.334/setup.cfg
+-rw-rw-rw-   0        0        0     4727 2024-05-05 06:44:23.000000 pkscreener-0.44.20240505.334/setup.py
```

### Comparing `pkscreener-0.44.20240504.333/LICENSE` & `pkscreener-0.44.20240505.334/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.333/LICENSE-Others` & `pkscreener-0.44.20240505.334/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.333/PKG-INFO` & `pkscreener-0.44.20240505.334/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240504.333
+Version: 0.44.20240505.334
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240504.333.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240505.334.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.332/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.333/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.332/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.333/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.332/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.333/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240504.333/README.md` & `pkscreener-0.44.20240505.334/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.332/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.333/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.332/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.333/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.332/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.333/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240504.333/pkscreener/__init__.py` & `pkscreener-0.44.20240505.334/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.333/pkscreener/classes/ArtTexts.py` & `pkscreener-0.44.20240505.334/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.333/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240505.334/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.333/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240505.334/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.333/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240505.334/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.333/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240505.334/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.333/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240505.334/pkscreener/classes/ConfigManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,17 +69,18 @@
         self.morninganalysiscandleduration = '1m'
         self.logger = None
         self.showPastStrategyData = False
         # This determines how many days apart the backtest calculations are run.
         # For example, for weekly backtest calculations, set this to 5 (5 days = 1 week)
         # For fortnightly, set this to 10 and so on (10 trading sessions = 2 weeks)
         self.backtestPeriodFactor = 1
-        self.maxDashboardWidgetsPerRow = 6
+        self.maxDashboardWidgetsPerRow = 3
+        self.maxNumResultRowsInMonitor = 2
         self.calculatersiintraday = False
-        self.defaultMonitorOptions = "X:12:9:2.5,|X:0:5:0:40:i 1m,X:12:27,X:12:28,X:12:23,X:12:5:0:30,X:12:6:3,X:12:6:7:1,X:12:6:8,X:12:6:9,X:12:6:10:1,X:12:7:3:.02:1,X:12:7:6:1,X:12:17,X:12:2,X:12:24,X:12:12:i 5m,X:12:13:i 1m"
+        self.defaultMonitorOptions = ""#"X:12:9:2.5,|X:0:5:0:40:i 1m,X:12:27,X:12:28,X:12:23,X:12:5:0:30,X:12:6:3,X:12:6:7:1,X:12:6:8,X:12:6:9,X:12:6:10:1,X:12:7:3:.02:1,X:12:7:6:1,X:12:17,X:12:2,X:12:24,X:12:12:i 5m,X:12:13:i 1m"
 
         self.daysToLookback = 22 * self.backtestPeriodFactor  # 1 month
         self.periods = [1,2,3,4,5,10,15,22,30]
         if self.maxBacktestWindow > self.periods[-1]:
             self.periods.extend(self.maxBacktestWindow)
 
     @property
@@ -164,14 +165,17 @@
             parser.set("config", "maxNetworkRetryCount", str(self.maxNetworkRetryCount))
             parser.set("config", "backtestPeriod", str(self.backtestPeriod))
             parser.set("config", "maxBacktestWindow", str(self.maxBacktestWindow))
             parser.set("config", "morninganalysiscandlenumber", str(self.morninganalysiscandlenumber))
             parser.set("config", "morninganalysiscandleduration", self.morninganalysiscandleduration)
             parser.set("config", "minimumVolume", str(self.minVolume))
             parser.set("config", "backtestPeriodFactor", str(self.backtestPeriodFactor))
+            parser.set("config", "maxDashboardWidgetsPerRow", str(self.maxDashboardWidgetsPerRow))
+            parser.set("config", "maxNumResultRowsInMonitor", str(self.maxNumResultRowsInMonitor))
+            parser.set("config", "defaultMonitorOptions", "X:12:9:2.5,|X:0:5:0:40:i 1m,X:12:27,X:12:28,X:12:23,X:12:5:0:30,X:12:6:3,X:12:6:7:1,X:12:6:8,X:12:6:9,X:12:6:10:1,X:12:7:3:.02:1,X:12:7:6:1,X:12:17,X:12:2,X:12:24,X:12:12:i 5m,X:12:13:i 1m")
             try:
                 fp = open("pkscreener.ini", "w")
                 parser.write(fp)
                 fp.close()
                 if showFileCreatedText:
                     OutputControls().printOutput(
                         colorText.BOLD
@@ -321,14 +325,17 @@
             parser.set("config", "maxNetworkRetryCount", self.maxNetworkRetryCount)
             parser.set("config", "backtestPeriod", self.backtestPeriod)
             parser.set("config", "maxBacktestWindow", self.maxBacktestWindow)
             parser.set("config", "morninganalysiscandlenumber", self.morninganalysiscandlenumber)
             parser.set("config", "morninganalysiscandleduration", self.morninganalysiscandleduration + "m")
             parser.set("config", "minimumVolume", self.minVolume)
             parser.set("config", "backtestPeriodFactor", self.backtestPeriodFactor)
+            parser.set("config", "defaultMonitorOptions", self.defaultMonitorOptions)
+            parser.set("config", "maxDashboardWidgetsPerRow", self.maxDashboardWidgetsPerRow)
+            parser.set("config", "maxNumResultRowsInMonitor", self.maxNumResultRowsInMonitor)
             # delete stock data due to config change
             self.deleteFileWithPattern()
             OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.FAIL
                 + "[+] Cached Stock Data Deleted."
                 + colorText.END
@@ -424,14 +431,17 @@
                 )
                 self.backtestPeriod = int(parser.get("config", "backtestPeriod"))
                 self.maxBacktestWindow = int(parser.get("config", "maxBacktestWindow"))
                 self.morninganalysiscandlenumber = int(parser.get("config", "morninganalysiscandlenumber"))
                 self.morninganalysiscandleduration = parser.get("config", "morninganalysiscandleduration")
                 self.minVolume = int(parser.get("config", "minimumVolume"))
                 self.backtestPeriodFactor = int(parser.get("config", "backtestPeriodFactor"))
+                self.defaultMonitorOptions = str(parser.get("config", "defaultMonitorOptions"))
+                self.maxDashboardWidgetsPerRow = int(parser.get("config", "maxDashboardWidgetsPerRow"))
+                self.maxNumResultRowsInMonitor = int(parser.get("config", "maxNumResultRowsInMonitor"))
             except configparser.NoOptionError as e:# pragma: no cover
                 self.default_logger.debug(e, exc_info=True)
                 # input(colorText.BOLD + colorText.FAIL +
                 #       '[+] pkscreener requires user configuration again. Press enter to continue..' + colorText.END)
                 parser.remove_section("config")
                 self.setConfig(parser, default=True, showFileCreatedText=False)
             except Exception as e:  # pragma: no cover
```

### Comparing `pkscreener-0.44.20240504.333/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240505.334/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.333/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240505.334/pkscreener/classes/MarketMonitor.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,30 +26,32 @@
 import pandas as pd
 import numpy as np
 from PKDevTools.classes.Singleton import SingletonType, SingletonMixin
 from PKDevTools.classes.OutputControls import OutputControls
 from PKDevTools.classes.ColorText import colorText
 
 class MarketMonitor(SingletonMixin, metaclass=SingletonType):
-    def __init__(self,monitors=[], maxNumResultsPerRow=5,maxNumColsInEachResult=6,maxNumRowsInEachResult=10):
+    def __init__(self,monitors=[], maxNumResultsPerRow=3,maxNumColsInEachResult=6,maxNumRowsInEachResult=10,maxNumResultRowsInMonitor=2):
         super(MarketMonitor, self).__init__()
         if monitors is not None and len(monitors) > 0:
-            self.monitors = monitors
+            
+            self.monitors = monitors[:maxNumResultRowsInMonitor*maxNumResultsPerRow]
             self.monitorIndex = 0
             self.monitorPositions = {}
             # self.monitorNames = {}
             # We are going to present the dataframes in a 3x3 matrix with limited set of columns
             rowIndex = 0
             colIndex = 0
+            self.maxNumResultRowsInMonitor = maxNumResultRowsInMonitor
             self.maxNumRowsInEachResult = maxNumRowsInEachResult
             self.maxNumColsInEachResult = maxNumColsInEachResult
             self.maxNumResultsPerRow = maxNumResultsPerRow
             maxColIndex = self.maxNumColsInEachResult * self.maxNumResultsPerRow - 1
             self.lines = 0
-            for monitorKey in monitors:
+            for monitorKey in self.monitors:
                 self.monitorPositions[monitorKey] = [rowIndex,colIndex]
                 # self.monitorNames[monitorKey] = ""
                 colIndex += self.maxNumColsInEachResult
                 if colIndex > maxColIndex:
                     colIndex = 0
                     rowIndex += self.maxNumRowsInEachResult
             columns = []
```

### Comparing `pkscreener-0.44.20240504.333/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240505.334/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.333/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240505.334/pkscreener/classes/MenuOptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,21 +29,22 @@
 from PKDevTools.classes.OutputControls import OutputControls
 import pkscreener.classes.ConfigManager as ConfigManager
 
 configManager = ConfigManager.tools()
 
 level0MenuDict = {
     "X": "Scanners",
+    "M": "Monitor Intraday",
     "S": "Strategies",
     "B": "Backtests",
-    # "G": "Growth of 10k",
+    "G": "Growth of 10k",
+    "C": "Analyse morning vs close outcomes",
     "T": "~",
     "E": "Edit user configuration",
     "Y": "View your user configuration",
-    "C": "Analyse morning vs close outcomes",
     "U": "Check for software update",
     "H": "Help / About Developer",
     "Z": "Exit (Ctrl + C)",
 }
 level1_S_MenuDict = {
     "S": "Summary",
     "M": "Back to the Top/Main menu",
```

### Comparing `pkscreener-0.44.20240504.333/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240505.334/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.333/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240505.334/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.333/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240505.334/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.333/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240505.334/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.333/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240505.334/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.333/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240505.334/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.333/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240505.334/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.333/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240505.334/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.333/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240505.334/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.333/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240505.334/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.333/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240505.334/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.333/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240505.334/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.333/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240505.334/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.333/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240505.334/pkscreener/classes/Utility.py`

 * *Files 0% similar despite different names*

```diff
@@ -1069,14 +1069,17 @@
                                     if not isTrading:
                                         stockDict[stock] = df_or_dict
                             except:
                                     # Probably, the "stock" got removed from the latest download
                                     # and so, was not found in stockDict
                                 continue
                         stockDataLoaded = True
+                        # Remove the progress bar now!
+                        sys.stdout.write("\x1b[1A")  # cursor up one line
+                        sys.stdout.write("\x1b[2K")  # delete the last line
                 except Exception as e:  # pragma: no cover
                     default_logger().debug(e, exc_info=True)
                     f.close()
                     OutputControls().printOutput("[!] Download Error - " + str(e))
             else:
                 default_logger().debug(
                         f"Stock data cache file:{cache_file} on server has length ->{filesize}{chunksize}"
```

### Comparing `pkscreener-0.44.20240504.333/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240505.334/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.333/pkscreener/classes/keys.py` & `pkscreener-0.44.20240505.334/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.333/pkscreener/courbd.ttf` & `pkscreener-0.44.20240505.334/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.333/pkscreener/globals.py` & `pkscreener-0.44.20240505.334/pkscreener/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -421,15 +421,15 @@
                 input(
                     colorText.BOLD
                     + colorText.FAIL
                     + "[+] Press <Enter> to Exit!"
                     + colorText.END
                 )
                 sys.exit(0)
-            elif selectedMenu.menuKey in ["B", "C", "G", "H", "U", "T", "S", "E", "X", "Y"]:
+            elif selectedMenu.menuKey in ["B", "C", "G", "H", "U", "T", "S", "E", "X", "Y", "M"]:
                 Utility.tools.clearScreen()
                 selectedChoice["0"] = selectedMenu.menuKey
                 return selectedMenu
     except KeyboardInterrupt:
         raise KeyboardInterrupt
     except Exception as e:  # pragma: no cover
         default_logger().debug(e, exc_info=True)
@@ -688,15 +688,22 @@
     screenResults, saveResults = PKScanRunner.initDataframes()
     options, menuOption, indexOption, executeOption = getTopLevelMenuChoices(
         startupoptions, testBuild, downloadOnly, defaultAnswer=defaultAnswer
     )
     # Print Level 1 menu options
     selectedMenu = initExecution(menuOption=menuOption)
     menuOption = selectedMenu.menuKey
-    if menuOption in ["X", "T", "E", "Y", "U", "H", "C"]:
+    if menuOption in ["M"]:
+        launcher = sys.argv[0]
+        launcher = f"python3.11 {launcher}" if launcher.endswith(".py") else launcher
+        print(f"{colorText.GREEN}Launching PKScreener in monitoring mode. If it does not launch, please try with the following:{colorText.END}\n{colorText.FAIL}{launcher} -a Y -m 'X'{colorText.END}\n{colorText.WARN}Press Ctrl + C to exit monitoring mode.{colorText.END}")
+        sleep(2)
+        os.system(f"{launcher} -a Y -m 'X'")
+        sys.exit(0)
+    elif menuOption in ["X", "T", "E", "Y", "U", "H", "C"]:
         # Print Level 2 menu options
         menuOption, indexOption, executeOption, selectedChoice = getScannerMenuChoices(
             testBuild or testing,
             downloadOnly,
             startupoptions,
             menuOption=menuOption,
             indexOption=indexOption,
```

### Comparing `pkscreener-0.44.20240504.333/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240505.334/pkscreener/pkscreenerbot.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
 m0 = menus()
 m1 = menus()
 m2 = menus()
 m3 = menus()
 
 TOP_LEVEL_SCANNER_MENUS = ["X", "B"]
-TOP_LEVEL_SCANNER_SKIP_MENUS = ["S", "T", "E", "U", "Z", "C", "G"]
+TOP_LEVEL_SCANNER_SKIP_MENUS = ["M", "S", "G", "C", "T", "E", "U", "Z"]
 INDEX_SKIP_MENUS = ["W","E","M","Z","0","2","3","4","6","7","9","10","13"]
 SCANNER_SKIP_MENUS_1_TO_7 = ["0","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28","29","30","42","M","Z"]
 SCANNER_SKIP_MENUS_8_TO_13 = ["0","1","2","3","4","5","6","7","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28","29","30","42","M","Z"]
 SCANNER_SKIP_MENUS_14_TO_19 = ["0","1","2","3","4","5","6","7","8","9","10","11","12","13","20","21","22","23","24","25","26","27","28","29","30","42","M","Z"]
 SCANNER_SKIP_MENUS_20_TO_27 = ["0","1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","19","22","28","29","30","42","M","Z"]
 SCANNER_MENUS_WITH_NO_SUBMENUS = ["1","2","3","10","11","12","13","14","15","16","17","18","19","20","21","23","24","25","26","27"]
 SCANNER_MENUS_WITH_SUBMENU_SUPPORT = ["6", "7", "21"]
```

### Comparing `pkscreener-0.44.20240504.333/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240505.334/pkscreener/pkscreenercli.py`

 * *Files 1% similar despite different names*

```diff
@@ -628,8 +628,11 @@
         )
         sleep(int(args.croninterval) if not args.testbuild else 3)
     runApplication()
     cron_runs += 1
 
 
 if __name__ == "__main__":
-    pkscreenercli()
+    try:
+        pkscreenercli()
+    except KeyboardInterrupt:
+        sys.exit(0)
```

### Comparing `pkscreener-0.44.20240504.333/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240505.334/pkscreener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240504.333
+Version: 0.44.20240505.334
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240504.333.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240505.334.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.332/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.333/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.332/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.333/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.332/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.333/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240504.333/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240505.334/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.333/setup.py` & `pkscreener-0.44.20240505.334/setup.py`

 * *Files identical despite different names*

