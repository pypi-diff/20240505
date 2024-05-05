# Comparing `tmp/pkscreener-0.44.20240505.335.tar.gz` & `tmp/pkscreener-0.44.20240505.336.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240505.335.tar", last modified: Sun May  5 07:31:57 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240505.336.tar", last modified: Sun May  5 08:21:51 2024, max compression
```

## Comparing `pkscreener-0.44.20240505.335.tar` & `pkscreener-0.44.20240505.336.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 07:31:57.211139 pkscreener-0.44.20240505.335/
--rw-rw-rw-   0        0        0     1086 2024-05-05 07:27:46.000000 pkscreener-0.44.20240505.335/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-05 07:27:46.000000 pkscreener-0.44.20240505.335/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-05 07:31:57.211139 pkscreener-0.44.20240505.335/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-05 07:27:46.000000 pkscreener-0.44.20240505.335/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 07:31:57.195515 pkscreener-0.44.20240505.335/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-05 07:27:46.000000 pkscreener-0.44.20240505.335/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 07:31:57.211139 pkscreener-0.44.20240505.335/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-05 07:27:46.000000 pkscreener-0.44.20240505.335/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-05 07:27:46.000000 pkscreener-0.44.20240505.335/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-05 07:27:46.000000 pkscreener-0.44.20240505.335/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-05 07:27:47.000000 pkscreener-0.44.20240505.335/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-05-05 07:27:47.000000 pkscreener-0.44.20240505.335/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    26892 2024-05-05 07:27:47.000000 pkscreener-0.44.20240505.335/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-05 07:27:47.000000 pkscreener-0.44.20240505.335/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     7857 2024-05-05 07:27:47.000000 pkscreener-0.44.20240505.335/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-05 07:27:47.000000 pkscreener-0.44.20240505.335/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    29724 2024-05-05 07:27:47.000000 pkscreener-0.44.20240505.335/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    11375 2024-05-05 07:27:47.000000 pkscreener-0.44.20240505.335/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    22090 2024-05-05 07:27:47.000000 pkscreener-0.44.20240505.335/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    21218 2024-05-05 07:27:47.000000 pkscreener-0.44.20240505.335/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-05 07:27:47.000000 pkscreener-0.44.20240505.335/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8158 2024-05-05 07:27:47.000000 pkscreener-0.44.20240505.335/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-05 07:27:47.000000 pkscreener-0.44.20240505.335/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-05 07:27:47.000000 pkscreener-0.44.20240505.335/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18443 2024-05-05 07:27:47.000000 pkscreener-0.44.20240505.335/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-05 07:27:47.000000 pkscreener-0.44.20240505.335/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-05 07:27:47.000000 pkscreener-0.44.20240505.335/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   119213 2024-05-05 07:27:47.000000 pkscreener-0.44.20240505.335/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    52127 2024-05-05 07:27:47.000000 pkscreener-0.44.20240505.335/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-05-05 07:27:47.000000 pkscreener-0.44.20240505.335/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    82261 2024-05-05 07:27:47.000000 pkscreener-0.44.20240505.335/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-05-05 07:27:47.000000 pkscreener-0.44.20240505.335/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-05 07:31:48.000000 pkscreener-0.44.20240505.335/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-05-05 07:27:47.000000 pkscreener-0.44.20240505.335/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-05 07:27:47.000000 pkscreener-0.44.20240505.335/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   124696 2024-05-05 07:27:47.000000 pkscreener-0.44.20240505.335/pkscreener/globals.py
--rw-rw-rw-   0        0        0      867 2024-05-05 07:27:47.000000 pkscreener-0.44.20240505.335/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    42917 2024-05-05 07:27:47.000000 pkscreener-0.44.20240505.335/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    26476 2024-05-05 07:27:47.000000 pkscreener-0.44.20240505.335/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-05 07:31:57.195515 pkscreener-0.44.20240505.335/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-05 07:31:57.000000 pkscreener-0.44.20240505.335/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-05 07:31:57.000000 pkscreener-0.44.20240505.335/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 07:31:57.000000 pkscreener-0.44.20240505.335/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-05 07:31:57.000000 pkscreener-0.44.20240505.335/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-05 07:31:57.000000 pkscreener-0.44.20240505.335/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-05 07:31:57.000000 pkscreener-0.44.20240505.335/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-05 07:31:57.211139 pkscreener-0.44.20240505.335/setup.cfg
--rw-rw-rw-   0        0        0     4727 2024-05-05 07:27:47.000000 pkscreener-0.44.20240505.335/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 08:21:51.501858 pkscreener-0.44.20240505.336/
+-rw-rw-rw-   0        0        0     1086 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-05 08:21:51.501858 pkscreener-0.44.20240505.336/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 08:21:51.486237 pkscreener-0.44.20240505.336/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 08:21:51.501858 pkscreener-0.44.20240505.336/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    26892 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     7857 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    29724 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    11375 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    22090 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    21218 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8158 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18443 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   119213 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    52127 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    82261 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-05 08:21:43.000000 pkscreener-0.44.20240505.336/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   124696 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      867 2024-05-05 08:16:53.000000 pkscreener-0.44.20240505.336/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    42917 2024-05-05 08:16:53.000000 pkscreener-0.44.20240505.336/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    26476 2024-05-05 08:16:53.000000 pkscreener-0.44.20240505.336/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-05 08:21:51.486237 pkscreener-0.44.20240505.336/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-05 08:21:51.000000 pkscreener-0.44.20240505.336/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-05 08:21:51.000000 pkscreener-0.44.20240505.336/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 08:21:51.000000 pkscreener-0.44.20240505.336/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-05 08:21:51.000000 pkscreener-0.44.20240505.336/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-05 08:21:51.000000 pkscreener-0.44.20240505.336/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-05 08:21:51.000000 pkscreener-0.44.20240505.336/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-05 08:21:51.501858 pkscreener-0.44.20240505.336/setup.cfg
+-rw-rw-rw-   0        0        0     4765 2024-05-05 08:16:53.000000 pkscreener-0.44.20240505.336/setup.py
```

### Comparing `pkscreener-0.44.20240505.335/LICENSE` & `pkscreener-0.44.20240505.336/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.335/LICENSE-Others` & `pkscreener-0.44.20240505.336/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.335/PKG-INFO` & `pkscreener-0.44.20240505.336/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240505.335
+Version: 0.44.20240505.336
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240505.335.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240505.336.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.334/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.335/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.334/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.335/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.334/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.335/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240505.335/README.md` & `pkscreener-0.44.20240505.336/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.334/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.335/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.334/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.335/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.334/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.335/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240505.335/pkscreener/__init__.py` & `pkscreener-0.44.20240505.336/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.335/pkscreener/classes/ArtTexts.py` & `pkscreener-0.44.20240505.336/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.335/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240505.336/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.335/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240505.336/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.335/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240505.336/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.335/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240505.336/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.335/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240505.336/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.335/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240505.336/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.335/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240505.336/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.335/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240505.336/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.335/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240505.336/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.335/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240505.336/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.335/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240505.336/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.335/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240505.336/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.335/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240505.336/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.335/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240505.336/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.335/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240505.336/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.335/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240505.336/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.335/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240505.336/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.335/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240505.336/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.335/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240505.336/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.335/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240505.336/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.335/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240505.336/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.335/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240505.336/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.335/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240505.336/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.335/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240505.336/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.335/pkscreener/classes/keys.py` & `pkscreener-0.44.20240505.336/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.335/pkscreener/courbd.ttf` & `pkscreener-0.44.20240505.336/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.335/pkscreener/globals.py` & `pkscreener-0.44.20240505.336/pkscreener/globals.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.335/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240505.336/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.335/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240505.336/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.335/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240505.336/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.335/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240505.336/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240505.335
+Version: 0.44.20240505.336
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240505.335.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240505.336.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.334/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.335/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.334/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.335/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.334/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.335/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240505.335/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240505.336/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.335/setup.py` & `pkscreener-0.44.20240505.336/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,16 +49,16 @@
     install_requires.append("advanced_ta")
 
 if "Windows" in platform.system():
     install_requires = [
         ".github/dependencies/TA_Lib-0.4.28-cp311-cp311-win_amd64.whl"
     ].extend(install_requires)
 elif "Linux" in platform.system():
-    subprocess.Popen(["chmod", "+x", ".github/dependencies/talib.sh"])
-    subprocess.Popen("start .github/dependencies/talib.sh", shell=True)
+    subprocess.Popen(["chmod", "+x", ".github/dependencies/build_tools/github/talib.sh"])
+    subprocess.Popen("start .github/dependencies/build_tools/github/talib.sh", shell=True)
 # For Darwin, brew install ta-lib will work
 
 SYS_MAJOR_VERSION = str(sys.version_info.major)
 SYS_VERSION = SYS_MAJOR_VERSION + "." + str(sys.version_info.minor)
 
 WHEEL_NAME = (
     __PACKAGENAME__ + "-" + VERSION + "-py" + SYS_MAJOR_VERSION + "-none-any.whl"
```

