# Comparing `tmp/pkscreener-0.44.20240504.332.tar.gz` & `tmp/pkscreener-0.44.20240504.333.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240504.332.tar", last modified: Sat May  4 07:09:21 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240504.333.tar", last modified: Sat May  4 08:16:15 2024, max compression
```

## Comparing `pkscreener-0.44.20240504.332.tar` & `pkscreener-0.44.20240504.333.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 07:09:21.693017 pkscreener-0.44.20240504.332/
--rw-rw-rw-   0        0        0     1086 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-04 07:09:21.693017 pkscreener-0.44.20240504.332/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 07:09:21.677395 pkscreener-0.44.20240504.332/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 07:09:21.693017 pkscreener-0.44.20240504.332/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    25810 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     7690 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    29461 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    22090 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    21218 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8158 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18443 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   119213 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    52127 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    80732 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-04 07:09:15.000000 pkscreener-0.44.20240504.332/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   124033 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/pkscreener/globals.py
--rw-rw-rw-   0        0        0      595 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    42912 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    26410 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-04 07:09:21.677395 pkscreener-0.44.20240504.332/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-04 07:09:21.000000 pkscreener-0.44.20240504.332/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-04 07:09:21.000000 pkscreener-0.44.20240504.332/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 07:09:21.000000 pkscreener-0.44.20240504.332/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-04 07:09:21.000000 pkscreener-0.44.20240504.332/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-04 07:09:21.000000 pkscreener-0.44.20240504.332/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-04 07:09:21.000000 pkscreener-0.44.20240504.332/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-04 07:09:21.693017 pkscreener-0.44.20240504.332/setup.cfg
--rw-rw-rw-   0        0        0     4727 2024-05-04 07:06:18.000000 pkscreener-0.44.20240504.332/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 08:16:15.555037 pkscreener-0.44.20240504.333/
+-rw-rw-rw-   0        0        0     1086 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-04 08:16:15.555037 pkscreener-0.44.20240504.333/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 08:16:15.539412 pkscreener-0.44.20240504.333/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 08:16:15.555037 pkscreener-0.44.20240504.333/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    25810 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     7690 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    29461 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    22090 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    21218 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8158 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18443 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   119213 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    52127 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    82053 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-04 08:16:04.000000 pkscreener-0.44.20240504.333/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   124183 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      595 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    42912 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    26410 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-04 08:16:15.539412 pkscreener-0.44.20240504.333/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-04 08:16:15.000000 pkscreener-0.44.20240504.333/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-04 08:16:15.000000 pkscreener-0.44.20240504.333/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 08:16:15.000000 pkscreener-0.44.20240504.333/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-04 08:16:15.000000 pkscreener-0.44.20240504.333/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-04 08:16:15.000000 pkscreener-0.44.20240504.333/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-04 08:16:15.000000 pkscreener-0.44.20240504.333/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-04 08:16:15.555037 pkscreener-0.44.20240504.333/setup.cfg
+-rw-rw-rw-   0        0        0     4727 2024-05-04 08:11:07.000000 pkscreener-0.44.20240504.333/setup.py
```

### Comparing `pkscreener-0.44.20240504.332/LICENSE` & `pkscreener-0.44.20240504.333/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.332/LICENSE-Others` & `pkscreener-0.44.20240504.333/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.332/PKG-INFO` & `pkscreener-0.44.20240504.333/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240504.332
+Version: 0.44.20240504.333
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240504.332.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240504.333.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.330/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.332/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.330/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.332/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.330/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.332/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240504.332/README.md` & `pkscreener-0.44.20240504.333/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.330/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.332/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.330/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.332/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.330/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.332/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240504.332/pkscreener/__init__.py` & `pkscreener-0.44.20240504.333/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.332/pkscreener/classes/ArtTexts.py` & `pkscreener-0.44.20240504.333/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.332/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240504.333/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.332/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240504.333/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.332/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240504.333/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.332/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240504.333/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.332/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240504.333/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.332/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240504.333/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.332/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240504.333/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.332/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240504.333/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.332/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240504.333/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.332/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240504.333/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.332/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240504.333/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.332/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240504.333/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.332/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240504.333/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.332/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240504.333/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.332/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240504.333/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.332/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240504.333/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.332/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240504.333/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.332/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240504.333/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.332/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240504.333/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.332/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240504.333/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.332/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240504.333/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.332/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240504.333/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.332/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240504.333/pkscreener/classes/Utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,27 +43,14 @@
 import numpy as np
 import pytz
 from genericpath import isfile
 from PKDevTools.classes.log import default_logger
 from PKDevTools.classes.ColorText import colorText
 from pkscreener import Imports
 
-if Imports["keras"]:
-    try:
-        import keras
-    except:
-        print("The installation will fail. Please install 'keras' library on your machine!")
-        print(
-                colorText.BOLD
-                + colorText.FAIL
-                + "[+] 'Keras' library is not installed. You may wish to follow instructions from\n[+] https://github.com/pkjmesra/PKScreener/"
-                + colorText.END
-            )
-        pass
-
 import warnings
 from time import sleep
 
 warnings.simplefilter("ignore", DeprecationWarning)
 warnings.simplefilter("ignore", FutureWarning)
 import pandas as pd
 from alive_progress import alive_bar
@@ -1108,15 +1095,15 @@
                         isIntraday = isIntraday,
                         forceRedownload=forceRedownload
                     )
                 
         return stockDict,stockDataLoaded
 
     # Save screened results to excel
-    def promptSaveResults(df, defaultAnswer=None):
+    def promptSaveResults(sheetName,df, defaultAnswer=None):
         """
         Tries to save the dataframe output into an excel file.
 
         It will first try to save to the current-working-directory/results/
 
         If it fails to save, it will then try to save to Desktop and then eventually into
         a temporary directory.
@@ -1144,42 +1131,57 @@
             )
             desktop = os.path.expanduser("~/Desktop")
             # # the above is valid on Windows (after 7) but if you want it in os normalized form:
             desktop = os.path.normpath(os.path.expanduser("~/Desktop"))
             filePath = ""
             try:
                 filePath = os.path.join(Archiver.get_user_outputs_dir(), filename)
-                df.to_excel(filePath, engine="xlsxwriter")  # openpyxl throws an error exporting % sign.
+                # Create a Pandas Excel writer using XlsxWriter as the engine.
+                writer = pd.ExcelWriter(filePath, engine='xlsxwriter') # openpyxl throws an error exporting % sign.
+                # Convert the dataframe to an XlsxWriter Excel object.
+                df.to_excel(writer, sheet_name=sheetName)
+                # Close the Pandas Excel writer and output the Excel file.
+                writer.close()
                 isSaved = True
             except Exception as e:  # pragma: no cover
                 default_logger().debug(e, exc_info=True)
                 OutputControls().printOutput(
                     colorText.FAIL
                     + (
                         "[+] Error saving file at %s"
                         % filePath
                     )
                     + colorText.END
                 )
                 try:
                     filePath = os.path.join(desktop, filename)
-                    df.to_excel(filePath, engine="xlsxwriter")  # openpyxl throws an error exporting % sign.
+                    # Create a Pandas Excel writer using XlsxWriter as the engine.
+                    writer = pd.ExcelWriter(filePath, engine='xlsxwriter') # openpyxl throws an error exporting % sign.
+                    # Convert the dataframe to an XlsxWriter Excel object.
+                    df.to_excel(writer, sheet_name=sheetName)
+                    # Close the Pandas Excel writer and output the Excel file.
+                    writer.close()
                     isSaved = True
                 except Exception as ex:  # pragma: no cover
                     default_logger().debug(ex, exc_info=True)
                     OutputControls().printOutput(
                         colorText.FAIL
                         + (
                             "[+] Error saving file at %s"
                             % filePath
                         )
                         + colorText.END
                     )
                     filePath = os.path.join(tempfile.gettempdir(), filename)
-                    df.to_excel(filePath,engine="xlsxwriter")
+                    # Create a Pandas Excel writer using XlsxWriter as the engine.
+                    writer = pd.ExcelWriter(filePath, engine='xlsxwriter') # openpyxl throws an error exporting % sign.
+                    # Convert the dataframe to an XlsxWriter Excel object.
+                    df.to_excel(writer, sheet_name=sheetName)
+                    # Close the Pandas Excel writer and output the Excel file.
+                    writer.close()
                     isSaved = True
             OutputControls().printOutput(
                 colorText.BOLD
                 + (colorText.GREEN if isSaved else colorText.FAIL)
                 + (("[+] Results saved to %s" % filePath) if isSaved else "[+] Failed saving results into Excel file!")
                 + colorText.END
             )
@@ -1500,14 +1502,26 @@
                     except Exception as e:  # pragma: no cover
                         default_logger().debug(e, exc_info=True)
                         OutputControls().printOutput("[!] Download Error - " + str(e))
             time.sleep(3)
         try:
             if os.path.isfile(files[0]) and os.path.isfile(files[1]):
                 pkl = joblib.load(files[1])
+                if Imports["keras"]:
+                    try:
+                        import keras
+                    except:
+                        print("This installation might not work well, especially for NIFTY prediction. Please install 'keras' library on your machine!")
+                        print(
+                                colorText.BOLD
+                                + colorText.FAIL
+                                + "[+] 'Keras' library is not installed. You may wish to follow instructions from\n[+] https://github.com/pkjmesra/PKScreener/"
+                                + colorText.END
+                            )
+                        pass
                 model = keras.models.load_model(files[0]) if Imports["keras"] else None
         except Exception as e:  # pragma: no cover
             default_logger().debug(e, exc_info=True)
             os.remove(files[0])
             os.remove(files[1])
             if not retrial:
                 tools.getNiftyModel(retrial=True)
```

### Comparing `pkscreener-0.44.20240504.332/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240504.333/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.332/pkscreener/classes/keys.py` & `pkscreener-0.44.20240504.333/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.332/pkscreener/courbd.ttf` & `pkscreener-0.44.20240504.333/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.332/pkscreener/globals.py` & `pkscreener-0.44.20240504.333/pkscreener/globals.py`

 * *Files 1% similar despite different names*

```diff
@@ -2321,37 +2321,38 @@
     else:
         OutputControls().printOutput(colorText.BOLD + colorText.GREEN + "[+] Skipped Saving!" + colorText.END)
 
 
 def saveNotifyResultsFile(
     screenResults, saveResults, defaultAnswer, menuChoiceHierarchy, user=None
 ):
-    global userPassedArgs, elapsed_time
+    global userPassedArgs, elapsed_time, selectedChoice
     if user is None and userPassedArgs.user is not None:
         user = userPassedArgs.user
     caption = f'<b>{menuChoiceHierarchy.split(">")[-1]}</b>'
     if screenResults is not None and len(screenResults) >= 1:
-        filename = Utility.tools.promptSaveResults(
+        choices = PKScanRunner.getFormattedChoices(userPassedArgs,selectedChoice)
+        filename = Utility.tools.promptSaveResults(choices,
             saveResults, defaultAnswer=defaultAnswer
         )
         # if filename is not None:
         #     sendMessageToTelegramChannel(
         #         document_filePath=filename, caption=caption, user=user
         #     )
         OutputControls().printOutput(
             colorText.BOLD
             + colorText.WARN
-            + "[+] Note: Trend calculation is based on number of days 'daysToLookBack' to scan as per your configuration."
+            + "[+] Notes:1.Trend calculation is based on 'daysToLookBack'. See configuration. 2.Reduce the console font size to fit all columns on screen."
             + colorText.END
         )
-        try:
-            if filename is not None:
-                os.remove(filename)
-        except Exception as e:  # pragma: no cover
-            default_logger().debug(e, exc_info=True)
+        # try:
+        #     if filename is not None:
+        #         os.remove(filename)
+        # except Exception as e:  # pragma: no cover
+        #     default_logger().debug(e, exc_info=True)
     if userPassedArgs.monitor is None:
         OutputControls().printOutput(
             colorText.BOLD
             + colorText.GREEN
             + f"[+] Screening Completed. Found {len(screenResults) if screenResults is not None else 0} results in {round(elapsed_time,2)} sec.! Press Enter to Continue.."
             + colorText.END
             , enableMultipleLineOutput=True
```

### Comparing `pkscreener-0.44.20240504.332/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240504.333/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.332/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240504.333/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.332/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240504.333/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.332/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240504.333/pkscreener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240504.332
+Version: 0.44.20240504.333
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240504.332.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240504.333.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.330/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.332/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.330/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.332/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.330/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.332/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240504.332/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240504.333/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.332/setup.py` & `pkscreener-0.44.20240504.333/setup.py`

 * *Files identical despite different names*

