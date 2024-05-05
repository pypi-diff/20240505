# Comparing `tmp/pkscreener-0.44.20240505.336.tar.gz` & `tmp/pkscreener-0.44.20240505.337.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240505.336.tar", last modified: Sun May  5 08:21:51 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240505.337.tar", last modified: Sun May  5 10:33:41 2024, max compression
```

## Comparing `pkscreener-0.44.20240505.336.tar` & `pkscreener-0.44.20240505.337.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 08:21:51.501858 pkscreener-0.44.20240505.336/
--rw-rw-rw-   0        0        0     1086 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-05 08:21:51.501858 pkscreener-0.44.20240505.336/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 08:21:51.486237 pkscreener-0.44.20240505.336/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 08:21:51.501858 pkscreener-0.44.20240505.336/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    26892 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     7857 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    29724 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    11375 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    22090 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    21218 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8158 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18443 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   119213 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    52127 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    82261 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-05 08:21:43.000000 pkscreener-0.44.20240505.336/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   124696 2024-05-05 08:16:52.000000 pkscreener-0.44.20240505.336/pkscreener/globals.py
--rw-rw-rw-   0        0        0      867 2024-05-05 08:16:53.000000 pkscreener-0.44.20240505.336/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    42917 2024-05-05 08:16:53.000000 pkscreener-0.44.20240505.336/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    26476 2024-05-05 08:16:53.000000 pkscreener-0.44.20240505.336/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-05 08:21:51.486237 pkscreener-0.44.20240505.336/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-05 08:21:51.000000 pkscreener-0.44.20240505.336/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-05 08:21:51.000000 pkscreener-0.44.20240505.336/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 08:21:51.000000 pkscreener-0.44.20240505.336/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-05 08:21:51.000000 pkscreener-0.44.20240505.336/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-05 08:21:51.000000 pkscreener-0.44.20240505.336/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-05 08:21:51.000000 pkscreener-0.44.20240505.336/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-05 08:21:51.501858 pkscreener-0.44.20240505.336/setup.cfg
--rw-rw-rw-   0        0        0     4765 2024-05-05 08:16:53.000000 pkscreener-0.44.20240505.336/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 10:33:41.986603 pkscreener-0.44.20240505.337/
+-rw-rw-rw-   0        0        0     1086 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-05 10:33:41.986603 pkscreener-0.44.20240505.337/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 10:33:41.970979 pkscreener-0.44.20240505.337/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 10:33:41.986603 pkscreener-0.44.20240505.337/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    26892 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     7857 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    30385 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    11375 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    22090 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    21218 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8158 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18443 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   119213 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    52127 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    82261 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-05 10:33:33.000000 pkscreener-0.44.20240505.337/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     5262 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   124696 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      867 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    44575 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    26476 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-05 10:33:41.970979 pkscreener-0.44.20240505.337/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-05 10:33:41.000000 pkscreener-0.44.20240505.337/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-05 10:33:41.000000 pkscreener-0.44.20240505.337/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 10:33:41.000000 pkscreener-0.44.20240505.337/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-05 10:33:41.000000 pkscreener-0.44.20240505.337/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-05 10:33:41.000000 pkscreener-0.44.20240505.337/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-05 10:33:41.000000 pkscreener-0.44.20240505.337/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-05 10:33:41.986603 pkscreener-0.44.20240505.337/setup.cfg
+-rw-rw-rw-   0        0        0     4765 2024-05-05 10:30:02.000000 pkscreener-0.44.20240505.337/setup.py
```

### Comparing `pkscreener-0.44.20240505.336/LICENSE` & `pkscreener-0.44.20240505.337/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.336/LICENSE-Others` & `pkscreener-0.44.20240505.337/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.336/PKG-INFO` & `pkscreener-0.44.20240505.337/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240505.336
+Version: 0.44.20240505.337
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240505.336.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240505.337.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.335/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.336/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.335/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.336/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.335/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.336/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240505.336/README.md` & `pkscreener-0.44.20240505.337/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.335/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.336/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.335/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.336/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.335/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.336/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240505.336/pkscreener/__init__.py` & `pkscreener-0.44.20240505.337/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.336/pkscreener/classes/ArtTexts.py` & `pkscreener-0.44.20240505.337/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.336/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240505.337/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.336/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240505.337/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.336/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240505.337/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.336/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240505.337/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.336/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240505.337/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.336/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240505.337/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.336/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240505.337/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.336/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240505.337/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.336/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240505.337/pkscreener/classes/MenuOptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 from PKDevTools.classes.log import default_logger
 from PKDevTools.classes.OutputControls import OutputControls
 import pkscreener.classes.ConfigManager as ConfigManager
 from pkscreener.classes.OtaUpdater import OTAUpdater
 from pkscreener.classes import VERSION
 
 configManager = ConfigManager.tools()
+MENU_SEPARATOR = ""
+LINE_SEPARATOR = "\n"
 
 level0MenuDict = {
     "X": "Scanners",
     "M": "Monitor Intraday",
     "S": "Strategies",
     "B": "Backtests",
     "G": "Growth of 10k",
@@ -63,17 +65,17 @@
     "4": "Nifty 200         ",
     "5": "Nifty 500         ",
     "6": "Nifty Smallcap 50 ",
     "7": "Nifty Smallcap 100",
     "8": "Nifty Smallcap 250",
     "9": "Nifty Midcap 50   ",
     "10": "Nifty Midcap 100",
-    "11": "Nifty Midcap 150",
+    "11": "Nifty Midcap 150 ",
     "12": "Nifty (All Stocks)",
-    "13": "Newly Listed (IPOs in last 2 Year)        ",
+    "13": "Newly Listed (IPOs in last 2 Year)           ",
     "14": "F&O Stocks Only",
     "15": "NASDAQ",
     "M": "Back to the Top/Main menu",
     "Z": "Exit (Ctrl + C)",
 }
 level2_X_MenuDict = {
     "0": "Full Screening (Shows Technical Parameters without any criterion)",
@@ -97,15 +99,15 @@
     "18": "Bullish Aroon(14) Crossover",
     "19": "MACD Histogram x below 0 (Sell) ",
     "20": "Bullish for next day",
     "21": "MF/FIIs Popular Stocks         ",
     "22": "View Stock Performance         ",
     "23": "Breaking out now               ",
     "24": "Higher Highs,Lows & Close (SuperTrend)",
-    "25": "Lower Highs,Lows (Sell/Watch for Rev.)",
+    "25": "Lower Highs,Lows (Watch for Rev.)",
     "26": "Stocks with stock-split/bonus/dividends",
     "27": "ATR Cross                      ",
     "28": "Higher Opens                   ",
     # "27": "Intraday Momentum Build-up      ",
     # "28": "Extremely bullish daily close      ",
     # "29": "Rising RSI                      ",
     # "30": "RSI entering bullish territory",
@@ -191,25 +193,29 @@
         self.menuKey = ""
         self.menuText = ""
         self.submenu = None
         self.level = 0
         self.isException = None
         self.hasLeftSibling = False
         self.parent = None
+        self.line = 0
+        self.lineIndex = 0
 
     def create(self, key, text, level=0, isException=False, parent=None):
         self.menuKey = str(key)
         self.menuText = text
         self.level = level
         self.isException = isException
         self.parent = parent
+        self.line = 0
+        self.lineIndex = 0
         return self
 
     def keyTextLabel(self):
-        return f"{self.menuKey} > {self.menuText}"
+        return f"{MENU_SEPARATOR}{self.menuKey} > {self.menuText}"
 
     def commandTextKey(self, hasChildren=False):
         cmdText = ""
         if self.parent is None:
             cmdText = f"/{self.menuKey}"
             return cmdText
         else:
@@ -309,28 +315,44 @@
         renderStyle=MenuRenderStyle.STANDALONE,
         renderExceptionKeys=[],
         skip=[],
         parent=None,
     ):
         tabLevel = 0
         self.menuDict = {}
+        line = 0
+        lineIndex = 1
         for key in rawDictionary:
             if skip is not None and key in skip:
                 continue
             m = menu()
             m.create(
                 str(key).upper(), rawDictionary[key], level=self.level, parent=parent
             )
             if key in renderExceptionKeys:
                 m.isException = True
+                line += 2
+                lineIndex = 1
+                m.line = line
+                m.lineIndex = lineIndex
             elif str(key).isnumeric():
                 m.hasLeftSibling = False if tabLevel == 0 else True
+                if tabLevel == 0:
+                    line += 1
+                lineIndex = tabLevel + 1
+                m.line = line
+                m.lineIndex = lineIndex
                 tabLevel = tabLevel + 1
                 if tabLevel >= renderStyle.value:
                     tabLevel = 0
+            else:
+                line += 1
+                lineIndex = 1
+                m.line = line
+                m.lineIndex = lineIndex
             self.menuDict[str(key).upper()] = m
         return self
 
     def render(self, asList=False, coloredValues=[]):
         menuText = [] if asList else ""
         for k in self.menuDict.keys():
             m = self.menuDict[k]
```

### Comparing `pkscreener-0.44.20240505.336/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240505.337/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.336/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240505.337/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.336/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240505.337/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.336/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240505.337/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.336/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240505.337/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.336/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240505.337/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.336/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240505.337/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.336/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240505.337/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.336/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240505.337/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.336/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240505.337/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.336/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240505.337/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.336/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240505.337/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.336/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240505.337/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.336/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240505.337/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.336/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240505.337/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.336/pkscreener/classes/keys.py` & `pkscreener-0.44.20240505.337/pkscreener/classes/keys.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,28 +55,36 @@
 # -----
 
 def draw_menu(menuItems, selectedIndex):
     #  window.erase()
     window.clear()
 
     # Print a vertical menu.
+    line = 1
     for i in range(len(menuItems)):
         window.addstr(' ')
-        window.addstr(menuItems[i], black if i == selectedIndex else white)
-        window.addstr('\n\n')
+        newLines = ""
+        menu = menuItems[i]
+        menuText = menu.keyTextLabel()
+        if line != menu.line:
+          window.addstr('\n')
+          line += 1
+        window.addstr(f"{menuText}\n", black if i == selectedIndex else white)
+        #   line += 1
+        line += 1
+
+    # # Print a dividing line.
+    # window.addstr(('-' * 80) + '\n')
+
+    # # Print a horizontal menu.
+    # for i in range(len(menuItems)):
+    #     window.addstr(' ')
+    #     window.addstr(menuItems[i], black if i == selectedIndex else white)
 
-    # Print a dividing line.
-    window.addstr(('-' * 80) + '\n')
-
-    # Print a horizontal menu.
-    for i in range(len(menuItems)):
-        window.addstr(' ')
-        window.addstr(menuItems[i], black if i == selectedIndex else white)
-
-    window.addstr('\n')
+    # window.addstr('\n')
 
 # -----
 
 def process_input(menuItems, selectedIndex):
     userInput = window.getch()
 
     if userInput == curses.KEY_LEFT or userInput == curses.KEY_UP:
@@ -92,19 +100,19 @@
         # If the last option, exit, is selected.
         if selectedIndex == len(menuItems) - 1:
             wait_for_any_keypress()
             curses.endwin() # De-initialize the library, and return terminal to normal status.    <-- Works without this on Windows, however in Linux you can't type in the terminal after exiting without this :P
             exit(0)
 
         window.addstr('\n Selected index: {}\n'.format(selectedIndex))
-        wait_for_any_keypress()
+        # wait_for_any_keypress()
 
     else:
         window.addstr("\n The pressed key '{}' {} is not associated with a menu function.\n".format(chr(userInput), userInput))
-        wait_for_any_keypress()
+        # wait_for_any_keypress()
 
     return selectedIndex
 
 # -----
 
 def wait_for_any_keypress():
     window.addstr('\n Press any key to continue . . . ')
@@ -114,16 +122,20 @@
 
 def main():
     selectedIndex = 0
     while True:
         draw_menu(MENU_ITEMS, selectedIndex)
         selectedIndex = process_input(MENU_ITEMS, selectedIndex)
 
-MENU_ITEMS = [
-    ' Option 1 ',
-    ' Option 2 ',
-    ' Option 3 ',
-    ' Exit ',
-]
+from pkscreener.classes.MenuOptions import menus
+m = menus()
+
+MENU_ITEMS = m.renderForMenu(asList=True)
+#[
+#     ' Option 1 ',
+#     ' Option 2 ',
+#     ' Option 3 ',
+#     ' Exit ',
+# ]
 
 if __name__ == '__main__':
     main()
```

### Comparing `pkscreener-0.44.20240505.336/pkscreener/courbd.ttf` & `pkscreener-0.44.20240505.337/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.336/pkscreener/globals.py` & `pkscreener-0.44.20240505.337/pkscreener/globals.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.336/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240505.337/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.336/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240505.337/pkscreener/pkscreenerbot.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,32 +99,41 @@
 m1 = menus()
 m2 = menus()
 m3 = menus()
 
 TOP_LEVEL_SCANNER_MENUS = ["X", "B"]
 TOP_LEVEL_SCANNER_SKIP_MENUS = ["M", "S", "G", "C", "T", "E", "U", "Z"]
 INDEX_SKIP_MENUS = ["W","E","M","Z","0","2","3","4","6","7","9","10","13"]
-SCANNER_SKIP_MENUS_1_TO_7 = ["0","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28","29","30","42","M","Z"]
-SCANNER_SKIP_MENUS_8_TO_13 = ["0","1","2","3","4","5","6","7","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28","29","30","42","M","Z"]
-SCANNER_SKIP_MENUS_14_TO_19 = ["0","1","2","3","4","5","6","7","8","9","10","11","12","13","20","21","22","23","24","25","26","27","28","29","30","42","M","Z"]
-SCANNER_SKIP_MENUS_20_TO_27 = ["0","1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","19","22","28","29","30","42","M","Z"]
-SCANNER_MENUS_WITH_NO_SUBMENUS = ["1","2","3","10","11","12","13","14","15","16","17","18","19","20","21","23","24","25","26","27"]
+SCANNER_SKIP_MENUS_1_TO_6 = ["0","7","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28","29","30","42","M","Z"]
+SCANNER_SKIP_MENUS_7_TO_12 = ["0","1","2","3","4","5","6","13","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28","29","30","42","M","Z"]
+SCANNER_SKIP_MENUS_13_TO_18 = ["0","1","2","3","4","5","6","7","8","9","10","11","12","19","20","21","22","23","24","25","26","27","28","29","30","42","M","Z"]
+SCANNER_SKIP_MENUS_19_TO_25 = ["0","1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","22","26","27","28","29","30","42","M","Z"]
+SCANNER_SKIP_MENUS_26_TO_31 = ["0","1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","29","30","42","M","Z"]
+SCANNER_MENUS_WITH_NO_SUBMENUS = ["1","2","3","10","11","12","13","14","15","16","17","18","19","20","21","23","24","25","26","27","28"]
 SCANNER_MENUS_WITH_SUBMENU_SUPPORT = ["6", "7", "21"]
 
 INDEX_COMMANDS_SKIP_MENUS_SCANNER = ["W", "E", "M", "Z"]
 INDEX_COMMANDS_SKIP_MENUS_BACKTEST = ["W", "E", "M", "Z", "N", "0", "15"]
-UNSUPPORTED_COMMAND_MENUS =["22","28","29","30","42","M","Z"]
-SUPPORTED_COMMAND_MENUS = ["1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","26","27"]
+UNSUPPORTED_COMMAND_MENUS =["22","29","30","42","M","Z"]
+SUPPORTED_COMMAND_MENUS = ["1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28"]
 
 async def start(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
     """Send message on `/start`."""
-    if update is None or update.message is None:
+    updateCarrier = None
+    if update is None:
         return
+    else:
+        if update.callback_query is not None:
+            updateCarrier = update.callback_query
+        if update.message is not None:
+            updateCarrier = update.message
+        if updateCarrier is None:
+            return
     # Get user that sent /start and log his name
-    user = update.message.from_user
+    user = updateCarrier.from_user
     logger.info("User %s started the conversation.", user.first_name)
     # Build InlineKeyboard where each button has a displayed text
     # and a string as callback_data
     # The keyboard is a list of button rows, where each row is in turn
     # a list (hence `[[...]]`).
     mns = m0.renderForMenu(asList=True)
     inlineMenus = []
@@ -143,19 +152,25 @@
         skip=TOP_LEVEL_SCANNER_SKIP_MENUS,
         asList=True,
         renderStyle=MenuRenderStyle.STANDALONE,
     )
     cmdText = ""
     for cmd in cmds:
         cmdText = f"{cmdText}\n\n{cmd.commandTextKey()} for {cmd.commandTextLabel()}"
+    menuText = f"Welcome {user.first_name}, {(user.username)}! Please choose a menu option by selecting a button from below.\n\nYou can also explore a wide variety of all other scanners by typing in \n{cmdText}\n\n OR just use the buttons below to choose."
     # Send message with text and appended InlineKeyboard
-    await update.message.reply_text(
-        f"Welcome {user.first_name}, {(user.username)}! Please choose a menu option by selecting a button from below.\n\nYou can also explore a wide variety of all other scanners by typing in \n{cmdText}\n\n OR just use the buttons below to choose.",
-        reply_markup=reply_markup,
-    )
+    if update.callback_query is not None:
+        await sendUpdatedMenu(
+            menuText=menuText, update=update, context=context, reply_markup=reply_markup
+        )
+    elif update.message is not None:
+        await update.message.reply_text(
+            menuText,
+            reply_markup=reply_markup,
+        )
     await context.bot.send_message(
         chat_id=int(f"-{Channel_Id}"),
         text=f"Name: {user.first_name}, Username:@{user.username} with ID: {str(user.id)} started using the bot!",
         parse_mode=ParseMode.HTML,
     )
     # Tell ConversationHandler that we're in state `FIRST` now
     return START_ROUTES
@@ -177,19 +192,21 @@
             renderStyle=MenuRenderStyle.STANDALONE,
         )
         .replace("     ", "")
         .replace("    ", "")
         .replace("\t", "")
         .replace(colorText.FAIL,"").replace(colorText.END,"")
     )
+    menuText = menuText + "\n\nH > Home"
     mns = m1.renderForMenu(
         m0.find(data),
         skip=skipMenus,
         asList=True,
     )
+    mns.append(menu().create("H", "Home", 2))
     inlineMenus = []
     await query.answer()
     for mnu in mns:
         inlineMenus.append(
             InlineKeyboardButton(
                 mnu.menuKey, callback_data=str(f"{query.data}_{mnu.menuKey}")
             )
@@ -208,81 +225,103 @@
     query = update.callback_query
     await query.answer()
     preSelection = (
         query.data.upper().replace("CX", "X").replace("CB", "B").replace("CG", "G")
     )
     selection = preSelection.split("_")
     preSelection = f"{selection[0]}_{selection[1]}"
-    if selection[0].upper() not in TOP_LEVEL_SCANNER_MENUS:
-        return start(update, context)
+    if (selection[0].upper() not in TOP_LEVEL_SCANNER_MENUS):
+        await start(update, context)
+        return START_ROUTES
+    if selection[len(selection)-1].upper() == "H":
+        await start(update, context)
+        return START_ROUTES
     if len(selection) == 2 or (len(selection) == 3 and selection[2] == "P"):
         if str(selection[1]).isnumeric():
             # It's only level 2
             menuText = m2.renderForMenu(
                 m1.find(selection[1]),
-                skip=SCANNER_SKIP_MENUS_1_TO_7,
+                skip=SCANNER_SKIP_MENUS_1_TO_6,
                 renderStyle=MenuRenderStyle.STANDALONE,
             )
             menuText = menuText + "\n\nN > More options"
+            menuText = menuText + "\n\nH > Home"
             mns = m2.renderForMenu(
                 m1.find(selection[1]),
-                skip=SCANNER_SKIP_MENUS_1_TO_7,
+                skip=SCANNER_SKIP_MENUS_1_TO_6,
                 asList=True,
                 renderStyle=MenuRenderStyle.STANDALONE,
             )
             mns.append(menu().create("N", "More Options", 2))
+            mns.append(menu().create("H", "Home", 2))
         elif selection[1] == "N":
             selection.extend(["", ""])
     elif len(selection) == 3:
         if selection[2] == "N":
             menuText = m2.renderForMenu(
                 m1.find(selection[1]),
-                skip=SCANNER_SKIP_MENUS_8_TO_13,
+                skip=SCANNER_SKIP_MENUS_7_TO_12,
                 renderStyle=MenuRenderStyle.STANDALONE,
             )
-            menuText = menuText + "\n\nP > Previous Options"
             menuText = menuText + "\nM > More Options"
+            menuText = menuText + "\n\nH > Home"
             mns = m2.renderForMenu(
                 m1.find(selection[1]),
-                skip=SCANNER_SKIP_MENUS_8_TO_13,
+                skip=SCANNER_SKIP_MENUS_7_TO_12,
                 asList=True,
                 renderStyle=MenuRenderStyle.STANDALONE,
             )
-            mns.append(menu().create("P", "Previous Options", 2))
             mns.append(menu().create("M", "More Options", 2))
+            mns.append(menu().create("H", "Home", 2))
         elif selection[2] == "M":
             menuText = m2.renderForMenu(
                 m1.find(selection[1]),
-                skip=SCANNER_SKIP_MENUS_14_TO_19,
+                skip=SCANNER_SKIP_MENUS_13_TO_18,
                 renderStyle=MenuRenderStyle.STANDALONE,
             )
-            menuText = menuText + "\n\nP > Previous Options"
             menuText = menuText + "\n>> More Options"
+            menuText = menuText + "\n\nH > Home"
             mns = m2.renderForMenu(
                 m1.find(selection[1]),
-                skip=SCANNER_SKIP_MENUS_14_TO_19,
+                skip=SCANNER_SKIP_MENUS_13_TO_18,
                 asList=True,
                 renderStyle=MenuRenderStyle.STANDALONE,
             )
-            mns.append(menu().create("P", "Previous Options", 2))
             mns.append(menu().create(">>", "More Options", 2))
+            mns.append(menu().create("H", "Home", 2))
         elif selection[2] == ">>":
             menuText = m2.renderForMenu(
                 m1.find(selection[1]),
-                skip=SCANNER_SKIP_MENUS_20_TO_27,
+                skip=SCANNER_SKIP_MENUS_19_TO_25,
+                renderStyle=MenuRenderStyle.STANDALONE,
+            )
+            menuText = menuText + "\nR > More Options"
+            menuText = menuText + "\n\nH > Home"
+            mns = m2.renderForMenu(
+                m1.find(selection[1]),
+                skip=SCANNER_SKIP_MENUS_19_TO_25,
+                asList=True,
+                renderStyle=MenuRenderStyle.STANDALONE,
+            )
+            mns.append(menu().create("R", "More Options", 2))
+            mns.append(menu().create("H", "Home", 2))
+        elif selection[2] == "R":
+            menuText = m2.renderForMenu(
+                m1.find(selection[1]),
+                skip=SCANNER_SKIP_MENUS_26_TO_31,
                 renderStyle=MenuRenderStyle.STANDALONE,
             )
-            menuText = menuText + "\n\nP > Previous Options"
+            menuText = menuText + "\n\nH > Home"
             mns = m2.renderForMenu(
                 m1.find(selection[1]),
-                skip=SCANNER_SKIP_MENUS_20_TO_27,
+                skip=SCANNER_SKIP_MENUS_26_TO_31,
                 asList=True,
                 renderStyle=MenuRenderStyle.STANDALONE,
             )
-            mns.append(menu().create("P", "Previous Options", 2))
+            mns.append(menu().create("H", "Home", 2))
         elif str(selection[2]).isnumeric():
             preSelection = f"{selection[0]}_{selection[1]}_{selection[2]}"
             if selection[2] in SCANNER_MENUS_WITH_SUBMENU_SUPPORT:
                 menuText = m3.renderForMenu(
                     m2.find(selection[2]),
                     renderStyle=MenuRenderStyle.STANDALONE,
                     skip=["0"],
```

### Comparing `pkscreener-0.44.20240505.336/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240505.337/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.336/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240505.337/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240505.336
+Version: 0.44.20240505.337
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240505.336.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240505.337.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.335/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.336/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.335/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.336/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.335/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.336/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240505.336/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240505.337/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.336/setup.py` & `pkscreener-0.44.20240505.337/setup.py`

 * *Files identical despite different names*

