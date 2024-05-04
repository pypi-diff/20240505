# Comparing `tmp/aiomql-3.20.tar.gz` & `tmp/aiomql-3.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiomql-3.20.tar", last modified: Tue Feb 13 13:06:41 2024, max compression
+gzip compressed data, was "aiomql-3.21.tar", last modified: Sat May  4 23:10:05 2024, max compression
```

## Comparing `aiomql-3.20.tar` & `aiomql-3.21.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxrwxrwx   0        0        0        0 2024-02-13 13:06:41.272404 aiomql-3.20/
--rw-rw-rw-   0        0        0     1092 2023-04-10 06:55:09.000000 aiomql-3.20/LICENSE
--rw-rw-rw-   0        0        0     4921 2024-02-13 13:06:41.271402 aiomql-3.20/PKG-INFO
--rw-rw-rw-   0        0        0     4193 2024-02-12 19:33:09.000000 aiomql-3.20/README.md
--rw-rw-rw-   0        0        0      817 2024-02-13 13:05:42.000000 aiomql-3.20/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-13 13:06:41.273404 aiomql-3.20/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-04-10 06:55:09.000000 aiomql-3.20/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-13 13:06:40.378240 aiomql-3.20/src/
-drwxrwxrwx   0        0        0        0 2024-02-13 13:06:40.993399 aiomql-3.20/src/aiomql/
--rw-rw-rw-   0        0        0      623 2024-02-13 12:55:20.000000 aiomql-3.20/src/aiomql/__init__.py
--rw-rw-rw-   0        0        0     3694 2024-02-12 18:54:21.000000 aiomql-3.20/src/aiomql/account.py
--rw-rw-rw-   0        0        0     5474 2024-02-12 18:54:21.000000 aiomql-3.20/src/aiomql/bot_builder.py
--rw-rw-rw-   0        0        0    10145 2024-02-12 19:02:36.000000 aiomql-3.20/src/aiomql/candle.py
-drwxrwxrwx   0        0        0        0 2024-02-13 13:06:41.168403 aiomql-3.20/src/aiomql/core/
--rw-rw-rw-   0        0        0      227 2024-02-12 18:34:51.000000 aiomql-3.20/src/aiomql/core/__init__.py
--rw-rw-rw-   0        0        0     4487 2024-02-12 18:54:21.000000 aiomql-3.20/src/aiomql/core/base.py
--rw-rw-rw-   0        0        0     5692 2024-02-12 18:54:21.000000 aiomql-3.20/src/aiomql/core/config.py
--rw-rw-rw-   0        0        0    36149 2024-02-12 18:54:21.000000 aiomql-3.20/src/aiomql/core/constants.py
--rw-rw-rw-   0        0        0     1136 2024-02-12 18:54:21.000000 aiomql-3.20/src/aiomql/core/errors.py
--rw-rw-rw-   0        0        0      574 2024-01-24 23:56:43.000000 aiomql-3.20/src/aiomql/core/exceptions.py
--rw-rw-rw-   0        0        0    15586 2024-02-12 18:54:21.000000 aiomql-3.20/src/aiomql/core/meta_trader.py
--rw-rw-rw-   0        0        0    15024 2024-02-12 18:54:21.000000 aiomql-3.20/src/aiomql/core/models.py
--rw-rw-rw-   0        0        0     1451 2024-02-12 18:54:21.000000 aiomql-3.20/src/aiomql/core/task_queue.py
--rw-rw-rw-   0        0        0     3343 2024-02-12 19:02:36.000000 aiomql-3.20/src/aiomql/executor.py
--rw-rw-rw-   0        0        0     5663 2024-02-12 19:02:36.000000 aiomql-3.20/src/aiomql/history.py
-drwxrwxrwx   0        0        0        0 2024-02-13 13:06:41.180404 aiomql-3.20/src/aiomql/lib/
--rw-rw-rw-   0        0        0       75 2024-01-24 23:56:43.000000 aiomql-3.20/src/aiomql/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-13 13:06:41.207402 aiomql-3.20/src/aiomql/lib/strategies/
--rw-rw-rw-   0        0        0       67 2024-02-12 19:18:28.000000 aiomql-3.20/src/aiomql/lib/strategies/__init__.py
--rw-rw-rw-   0        0        0     5361 2024-02-13 13:02:25.000000 aiomql-3.20/src/aiomql/lib/strategies/finger_trap.py
--rw-rw-rw-   0        0        0     1136 2024-02-11 20:59:21.000000 aiomql-3.20/src/aiomql/lib/strategies/tracker.py
-drwxrwxrwx   0        0        0        0 2024-02-13 13:06:41.235406 aiomql-3.20/src/aiomql/lib/symbols/
--rw-rw-rw-   0        0        0       39 2024-01-24 23:56:43.000000 aiomql-3.20/src/aiomql/lib/symbols/__init__.py
--rw-rw-rw-   0        0        0     4265 2024-02-12 19:30:57.000000 aiomql-3.20/src/aiomql/lib/symbols/forex_symbol.py
-drwxrwxrwx   0        0        0        0 2024-02-13 13:06:41.264403 aiomql-3.20/src/aiomql/lib/traders/
--rw-rw-rw-   0        0        0       41 2024-02-12 19:30:57.000000 aiomql-3.20/src/aiomql/lib/traders/__init__.py
--rw-rw-rw-   0        0        0     1971 2024-02-12 19:30:57.000000 aiomql-3.20/src/aiomql/lib/traders/simple_trader.py
--rw-rw-rw-   0        0        0     4865 2024-02-12 19:02:36.000000 aiomql-3.20/src/aiomql/order.py
--rw-rw-rw-   0        0        0     4410 2024-02-12 19:02:36.000000 aiomql-3.20/src/aiomql/positions.py
--rw-rw-rw-   0        0        0     1920 2024-02-12 19:02:36.000000 aiomql-3.20/src/aiomql/ram.py
--rw-rw-rw-   0        0        0     4338 2024-02-12 19:18:28.000000 aiomql-3.20/src/aiomql/records.py
--rw-rw-rw-   0        0        0     2067 2024-02-13 12:49:46.000000 aiomql-3.20/src/aiomql/result.py
--rw-rw-rw-   0        0        0     8753 2024-02-12 19:18:28.000000 aiomql-3.20/src/aiomql/sessions.py
--rw-rw-rw-   0        0        0     2993 2024-02-03 13:05:20.000000 aiomql-3.20/src/aiomql/strategy.py
--rw-rw-rw-   0        0        0    17986 2024-02-12 19:18:28.000000 aiomql-3.20/src/aiomql/symbol.py
--rw-rw-rw-   0        0        0     2803 2024-02-12 19:18:28.000000 aiomql-3.20/src/aiomql/terminal.py
--rw-rw-rw-   0        0        0     5615 2024-02-12 19:18:28.000000 aiomql-3.20/src/aiomql/ticks.py
--rw-rw-rw-   0        0        0     5609 2024-02-12 19:18:28.000000 aiomql-3.20/src/aiomql/trader.py
--rw-rw-rw-   0        0        0     1413 2024-02-12 20:00:12.000000 aiomql-3.20/src/aiomql/utils.py
-drwxrwxrwx   0        0        0        0 2024-02-13 13:06:41.268404 aiomql-3.20/src/aiomql.egg-info/
--rw-rw-rw-   0        0        0     4921 2024-02-13 13:06:40.000000 aiomql-3.20/src/aiomql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1145 2024-02-13 13:06:40.000000 aiomql-3.20/src/aiomql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-13 13:06:40.000000 aiomql-3.20/src/aiomql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-02-13 13:06:40.000000 aiomql-3.20/src/aiomql.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-02-13 13:06:40.000000 aiomql-3.20/src/aiomql.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 23:10:05.304194 aiomql-3.21/
+-rw-rw-rw-   0        0        0     1092 2023-04-10 06:55:09.000000 aiomql-3.21/LICENSE
+-rw-rw-rw-   0        0        0     5059 2024-05-04 23:10:05.301197 aiomql-3.21/PKG-INFO
+-rw-rw-rw-   0        0        0     4252 2024-05-04 23:06:46.000000 aiomql-3.21/README.md
+-rw-rw-rw-   0        0        0      870 2024-04-27 10:38:39.000000 aiomql-3.21/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-04 23:10:05.304194 aiomql-3.21/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-04-10 06:55:09.000000 aiomql-3.21/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 23:10:05.020059 aiomql-3.21/src/
+drwxrwxrwx   0        0        0        0 2024-05-04 23:10:05.119129 aiomql-3.21/src/aiomql/
+-rw-rw-rw-   0        0        0      664 2024-04-10 01:11:51.000000 aiomql-3.21/src/aiomql/__init__.py
+-rw-rw-rw-   0        0        0     3696 2024-04-27 10:38:39.000000 aiomql-3.21/src/aiomql/account.py
+-rw-rw-rw-   0        0        0     5721 2024-04-27 10:38:39.000000 aiomql-3.21/src/aiomql/bot_builder.py
+-rw-rw-rw-   0        0        0    11834 2024-04-28 22:35:40.000000 aiomql-3.21/src/aiomql/candle.py
+drwxrwxrwx   0        0        0        0 2024-05-04 23:10:05.221470 aiomql-3.21/src/aiomql/core/
+-rw-rw-rw-   0        0        0      227 2024-02-12 18:34:51.000000 aiomql-3.21/src/aiomql/core/__init__.py
+-rw-rw-rw-   0        0        0     4487 2024-02-12 18:54:21.000000 aiomql-3.21/src/aiomql/core/base.py
+-rw-rw-rw-   0        0        0     6140 2024-04-27 22:17:47.000000 aiomql-3.21/src/aiomql/core/config.py
+-rw-rw-rw-   0        0        0    36149 2024-02-12 18:54:21.000000 aiomql-3.21/src/aiomql/core/constants.py
+-rw-rw-rw-   0        0        0     1136 2024-02-12 18:54:21.000000 aiomql-3.21/src/aiomql/core/errors.py
+-rw-rw-rw-   0        0        0      574 2024-01-24 23:56:43.000000 aiomql-3.21/src/aiomql/core/exceptions.py
+-rw-rw-rw-   0        0        0    15519 2024-04-29 12:23:17.000000 aiomql-3.21/src/aiomql/core/meta_trader.py
+-rw-rw-rw-   0        0        0    15024 2024-02-12 18:54:21.000000 aiomql-3.21/src/aiomql/core/models.py
+-rw-rw-rw-   0        0        0     1509 2024-05-04 12:54:41.000000 aiomql-3.21/src/aiomql/core/task_queue.py
+-rw-rw-rw-   0        0        0     3343 2024-02-12 19:02:36.000000 aiomql-3.21/src/aiomql/executor.py
+-rw-rw-rw-   0        0        0    11512 2024-04-29 12:22:52.000000 aiomql-3.21/src/aiomql/history.py
+drwxrwxrwx   0        0        0        0 2024-05-04 23:10:05.232647 aiomql-3.21/src/aiomql/lib/
+-rw-rw-rw-   0        0        0       75 2024-01-24 23:56:43.000000 aiomql-3.21/src/aiomql/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 23:10:05.249775 aiomql-3.21/src/aiomql/lib/strategies/
+-rw-rw-rw-   0        0        0       67 2024-02-12 19:18:28.000000 aiomql-3.21/src/aiomql/lib/strategies/__init__.py
+-rw-rw-rw-   0        0        0     5270 2024-05-04 13:19:33.000000 aiomql-3.21/src/aiomql/lib/strategies/finger_trap.py
+-rw-rw-rw-   0        0        0     1136 2024-02-11 20:59:21.000000 aiomql-3.21/src/aiomql/lib/strategies/tracker.py
+drwxrwxrwx   0        0        0        0 2024-05-04 23:10:05.283192 aiomql-3.21/src/aiomql/lib/symbols/
+-rw-rw-rw-   0        0        0       39 2024-01-24 23:56:43.000000 aiomql-3.21/src/aiomql/lib/symbols/__init__.py
+-rw-rw-rw-   0        0        0     4265 2024-02-12 19:30:57.000000 aiomql-3.21/src/aiomql/lib/symbols/forex_symbol.py
+drwxrwxrwx   0        0        0        0 2024-05-04 23:10:05.297197 aiomql-3.21/src/aiomql/lib/traders/
+-rw-rw-rw-   0        0        0       41 2024-02-12 19:30:57.000000 aiomql-3.21/src/aiomql/lib/traders/__init__.py
+-rw-rw-rw-   0        0        0     1971 2024-02-12 19:30:57.000000 aiomql-3.21/src/aiomql/lib/traders/simple_trader.py
+-rw-rw-rw-   0        0        0     5778 2024-04-22 12:13:27.000000 aiomql-3.21/src/aiomql/order.py
+-rw-rw-rw-   0        0        0     5681 2024-04-22 13:08:33.000000 aiomql-3.21/src/aiomql/positions.py
+-rw-rw-rw-   0        0        0     2484 2024-04-29 08:17:47.000000 aiomql-3.21/src/aiomql/ram.py
+-rw-rw-rw-   0        0        0     4400 2024-04-01 00:45:04.000000 aiomql-3.21/src/aiomql/records.py
+-rw-rw-rw-   0        0        0     3512 2024-04-22 14:36:06.000000 aiomql-3.21/src/aiomql/result.py
+-rw-rw-rw-   0        0        0     8753 2024-02-12 19:18:28.000000 aiomql-3.21/src/aiomql/sessions.py
+-rw-rw-rw-   0        0        0     2993 2024-02-03 13:05:20.000000 aiomql-3.21/src/aiomql/strategy.py
+-rw-rw-rw-   0        0        0    17986 2024-02-12 19:18:28.000000 aiomql-3.21/src/aiomql/symbol.py
+-rw-rw-rw-   0        0        0     2803 2024-02-12 19:18:28.000000 aiomql-3.21/src/aiomql/terminal.py
+-rw-rw-rw-   0        0        0     8323 2024-04-28 22:45:31.000000 aiomql-3.21/src/aiomql/ticks.py
+-rw-rw-rw-   0        0        0     5931 2024-04-10 10:12:59.000000 aiomql-3.21/src/aiomql/trade_records.py
+-rw-rw-rw-   0        0        0     5777 2024-04-27 10:45:41.000000 aiomql-3.21/src/aiomql/trader.py
+-rw-rw-rw-   0        0        0     1413 2024-02-12 20:00:12.000000 aiomql-3.21/src/aiomql/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-04 23:10:05.299196 aiomql-3.21/src/aiomql.egg-info/
+-rw-rw-rw-   0        0        0     5059 2024-05-04 23:10:04.000000 aiomql-3.21/src/aiomql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1173 2024-05-04 23:10:05.000000 aiomql-3.21/src/aiomql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 23:10:04.000000 aiomql-3.21/src/aiomql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2024-05-04 23:10:04.000000 aiomql-3.21/src/aiomql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-04 23:10:04.000000 aiomql-3.21/src/aiomql.egg-info/top_level.txt
```

### Comparing `aiomql-3.20/LICENSE` & `aiomql-3.21/LICENSE`

 * *Files identical despite different names*

### Comparing `aiomql-3.20/PKG-INFO` & `aiomql-3.21/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: aiomql
-Version: 3.20
-Summary: Asynchronous MetaTrader5 library and Bot Building Framework
+Version: 3.21
+Summary: Asynchronous MetaTrader5 library and Algorithmic Trading Framework
 Author-email: Ichinga Samuel <ichingasamuel@gmail.com>
 Project-URL: Homepage, https://github.com/Ichinga-Samuel/aiomql
 Project-URL: Bug Tracker, https://github.com/Ichinga-Samuel/aiomql/issues
 Keywords: MetaTrader5,Asynchronous,Algorithmic Trading,Trading Bot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: MetaTrader5>=5.0.37
 Requires-Dist: pandas>=1.5.0
 Requires-Dist: pandas-ta>=0.3.14b0
+Requires-Dist: matplotlib>=3.8.4
+Requires-Dist: mplfinance>=0.12.10b0
 
 # Aiomql - Bot Building Framework and Asynchronous MetaTrader5 Library
 ![GitHub](https://img.shields.io/github/license/ichinga-samuel/aiomql?style=plastic)
 ![GitHub issues](https://img.shields.io/github/issues/ichinga-samuel/aiomql?style=plastic)
 ![PyPI](https://img.shields.io/pypi/v/aiomql)
 
 ### Installation
@@ -31,14 +33,15 @@
 - Asynchronous Bot Building Framework
 - Build bots for trading in different financial markets using a bot factory
 - Use threadpool executors to run multiple strategies on multiple instruments concurrently
 - Records and keep track of trades and strategies in csv files.
 - Helper classes for Bot Building. Easy to use and extend.
 - Compatible with pandas-ta.
 - Sample Pre-Built strategies
+- Visualization of charts using matplotlib and mplfinance
 - Manage Trading periods using Sessions
 - Risk Management
 - Run multiple bots concurrently with different accounts from the same broker or different brokers
 
 ### As an asynchronous MetaTrader5 Libray
 ```python
 import asyncio
```

### Comparing `aiomql-3.20/README.md` & `aiomql-3.21/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 - Asynchronous Bot Building Framework
 - Build bots for trading in different financial markets using a bot factory
 - Use threadpool executors to run multiple strategies on multiple instruments concurrently
 - Records and keep track of trades and strategies in csv files.
 - Helper classes for Bot Building. Easy to use and extend.
 - Compatible with pandas-ta.
 - Sample Pre-Built strategies
+- Visualization of charts using matplotlib and mplfinance
 - Manage Trading periods using Sessions
 - Risk Management
 - Run multiple bots concurrently with different accounts from the same broker or different brokers
 
 ### As an asynchronous MetaTrader5 Libray
 ```python
 import asyncio
```

### Comparing `aiomql-3.20/pyproject.toml` & `aiomql-3.21/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -3,23 +3,23 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aiomql"
-version = "3.20"
+version = "3.21"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 keywords = ['MetaTrader5', 'Asynchronous', 'Algorithmic Trading', 'Trading Bot']
-dependencies = ["MetaTrader5>=5.0.37", "pandas>=1.5.0", "pandas-ta>=0.3.14b0"]
+dependencies = ["MetaTrader5>=5.0.37", "pandas>=1.5.0", "pandas-ta>=0.3.14b0", "matplotlib>=3.8.4", "mplfinance>=0.12.10b0"]
 authors = [{name = "Ichinga Samuel", email = "ichingasamuel@gmail.com"}]
-description = "Asynchronous MetaTrader5 library and Bot Building Framework"
+description = "Asynchronous MetaTrader5 library and Algorithmic Trading Framework"
 
 [project.urls]
 "Homepage" = "https://github.com/Ichinga-Samuel/aiomql"
 "Bug Tracker" = "https://github.com/Ichinga-Samuel/aiomql/issues"
```

### Comparing `aiomql-3.20/src/aiomql/account.py` & `aiomql-3.21/src/aiomql/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
             return False
         ini = await self.mt5.initialize(**acc, path=self.config.path)
         if ini:
             res = await self.mt5.login(**acc)
         if ini and res:
             return True
         else:
-            await asyncio.sleep(tries)
+            await asyncio.sleep(5+tries)
             return await self._login(acc=acc, tries=tries-1)
 
     def has_symbol(self, symbol: str | SymbolInfo):
         """Checks to see if a symbol is available for a trading account.
 
         Args:
             symbol (str | SymbolInfo):
```

### Comparing `aiomql-3.20/src/aiomql/bot_builder.py` & `aiomql-3.21/src/aiomql/bot_builder.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,19 +33,24 @@
     def __init__(self):
         self.config = Config()
         self.account = Account()
         self.symbols = set()
         self.executor = Executor()
 
     @classmethod
-    def run_bots(cls, bots: dict[Callable: dict] = None, num_workers: int = None):
-        """Run multiple bots at the same time."""
-        num_workers = num_workers or len(bots) * 2
+    def run_bots(cls, funcs: dict[Callable: dict] = None, num_workers: int = None):
+        """Run multiple scripts or bots in parallel with different accounts.
+
+        Args:
+            funcs (dict): A dictionary of functions to run with their respective keyword arguments as a dictionary
+            num_workers (int): Number of workers to run the functions
+        """
+        num_workers = num_workers or len(funcs) * 2
         with ProcessPoolExecutor(max_workers=num_workers) as executor:
-            for bot, kwargs in bots.items():
+            for bot, kwargs in funcs.items():
                 executor.submit(bot, **kwargs)
 
     async def initialize(self):
         """Prepares the bot by signing in to the trading account and initializing the symbols for the trading session.
         Starts the global task queue.
 
         Raises:
```

### Comparing `aiomql-3.20/src/aiomql/candle.py` & `aiomql-3.21/src/aiomql/candle.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,67 @@
 """Candle and Candles classes for handling bars from the MetaTrader 5 terminal."""
 
 from typing import Type, TypeVar, Generic, Iterable
 from logging import getLogger
 
 from pandas import DataFrame, Series
+import pandas as pd
 import pandas_ta as ta
+import mplfinance as mplt
 
 from .core.constants import TimeFrame
 
 logger = getLogger(__name__)
 
 
 class Candle:
-    """A class representing bars from the MetaTrader 5 terminal as a customized class analogous to Japanese
+    """A customized class representing rates from the MetaTrader 5 terminal analogous to Japanese
     Candlesticks. You can subclass this class for added customization.
 
     Attributes:
         time (int): Period start time.
         open (int): Open price
         high (float): The highest price of the period
         low (float): The lowest price of the period
         close (float): Close price
         tick_volume (float): Tick volume
         real_volume (float): Trade volume
         spread (float): Spread
         Index (int): Custom attribute representing the position of the candle in a sequence.
-        mid (float): The median of the high and low price.
     """
     time: float
     open: float
     high: float
     low: float
     close: float
     real_volume: float
     spread: float
     tick_volume: float
     Index: int
-    mid: float
 
     def __init__(self, **kwargs):
         """Create a Candle object from keyword arguments. This class must always be instantiated with open, high, low
          and close prices.
 
         Keyword Args:
             **kwargs: Candle attributes and values as keyword arguments.
         """
         if not all(i in kwargs for i in ['open', 'high', 'low', 'close']):
             raise ValueError("Candle must be instantiated with open, high, low and close prices")
         self.time = kwargs.pop('time', 0)
         self.Index = kwargs.pop('Index', 0)
-        self.mid = kwargs.pop('mid', (kwargs['high'] + kwargs['low']) / 2)
         self.set_attributes(**kwargs)
 
     def __repr__(self):
-        return ("%(class)s(Index=%(Index)s, time=%(time)s, open=%(open)s, high=%(high)s, low=%(low)s, close=%(close)s,"
-                " mid=%(mid)s)") % {"class": self.__class__.__name__, "open": self.open, "high": self.high,
-                                    "low": self.low, "close": self.close, "time": self.time, "mid": self.mid,
-                                    'Index': self.Index}
+        return ("%(class)s(Index=%(Index)s, time=%(time)s, open=%(open)s, high=%(high)s, low=%(low)s, close=%(close)s)"
+                % {"class": self.__class__.__name__, "open": self.open, "high": self.high,
+                   "low": self.low, "close": self.close, "time": self.time, 'Index': self.Index})
 
     def __str__(self):
-        return self.dict()
+        return str(self.dict())
 
     def __eq__(self, other: "Candle"):
         return self.time == other.time
 
     def __hash__(self):
         return hash(self.time)
 
@@ -148,15 +146,14 @@
     open: Series
     high: Series
     low: Series
     close: Series
     tick_volume: Series
     real_volume: Series
     spread: Series
-    mid: Series
     Candle: Type[Candle]
     timeframe: TimeFrame
     _data: DataFrame
 
     def __init__(self, *, data: DataFrame | _Candles | Iterable, flip=False, candle_class: Type[_Candle] = None):
         """A container class of Candle objects in chronological order.
 
@@ -173,17 +170,14 @@
             data = DataFrame(data.data)
         elif isinstance(data, Iterable):
             data = DataFrame(data)
         else:
             raise ValueError(f"Cannot create DataFrame from object of {type(data)}")
 
         self._data = data.loc[::-1].reset_index(drop=True) if flip else data
-        if 'mid' not in self._data.columns.values:
-            mid = (self._data['high'] + self._data['low']) / 2
-            self._data.insert(0, 'mid', mid)
         self.Candle = candle_class or Candle
 
     def __repr__(self):
         return self._data.__repr__()
 
     def __len__(self):
         return len(self._data.index)
@@ -264,7 +258,42 @@
             **kwargs: The new names of the columns
 
         Returns:
             Candles: A new instance of the class with the renamed columns if inplace is False else the modified instance
         """
         res = self._data.rename(columns=kwargs, inplace=inplace)
         return self if inplace else self.__class__(data=res)
+
+    def make_addplot(self, *, count: int = 50, columns: list = None, **kwargs) -> dict:
+        """
+        Make subplots for adding to the main plot
+
+        Args:
+            count (int): The numbers of candles to make the addplot for. Defaults to 50.
+            columns (list[str]): The columns to make the plot from. Defaults to None.
+            **kwargs: Valid arguments for the mplfinance make_addplot function
+        """
+        columns = columns or []
+        data = self._data[-count:]
+        data.index = pd.to_datetime(data['time'], unit='s')
+        return mplt.make_addplot(data[columns], **kwargs)
+
+    def visualize(self, *, count: int = 50, type='candle', savefig: str | dict = None, addplot: dict = None,
+                  style: str = 'charles', ylabel: str = 'Price', title: str = 'Chart', **kwargs):
+        """Visualize the candles using the mplfinance library.
+        Args:
+            count (int): The number of candles to visualize, counting from behind, i.e the most recent candles.
+             Defaults to 50.
+            type: Type of chart, defaults to candle
+            savefig (str|dict): The path to save the figure or a dictionary of parameters to pass to the savefig method.
+            addplot: Additional plots to add to the chart. Defaults to None. They should match the dimension of the
+              original data which is specified via the count parameter.
+            style (str): The style of the chart. Defaults to 'charles'.
+            ylabel (str): The label of the y-axis. Defaults to 'Price'.
+            title (str): The title of the chart. Defaults to 'Chart'.
+            kwargs: valid kwargs for the plot function.
+        """
+        kwargs |= {key: arg for key, arg in (('savefig', savefig), ('addplot', addplot), ('style', style),
+                                             ('ylabel', ylabel), ('title', title), ('type', type)) if arg}
+        data = self._data[-count:]
+        data.index = pd.to_datetime(data['time'], unit='s')
+        mplt.plot(data, **kwargs)
```

### Comparing `aiomql-3.20/src/aiomql/core/base.py` & `aiomql-3.21/src/aiomql/core/base.py`

 * *Files identical despite different names*

### Comparing `aiomql-3.20/src/aiomql/core/config.py` & `aiomql-3.21/src/aiomql/core/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import os
 from pathlib import Path
-from typing import Iterator
+from typing import Iterator, Literal, TypeVar
 import json
 from logging import getLogger
 
 from .task_queue import TaskQueue
 
 logger = getLogger(__name__)
+Bot = TypeVar("Bot")
 
 
 class Config:
     """A class for handling configuration settings for the aiomql package.
 
     Attributes:
         record_trades (bool): Whether to keep record of trades or not.
+        trade_record_mode: How to save trade, json or csv. Defaults to json
         filename (str): Name of the config file
         records_dir (str): Path to the directory where trade records are saved
         login (int): Trading account number
         password (str): Trading account password
         server (str): Broker server
         path (str): Path to terminal file
         timeout (int): Timeout for terminal connection
@@ -27,50 +29,48 @@
     Notes:
         By default, the config class looks for a file named aiomql.json.
         You can change this by passing the filename and/or the config_dir keyword argument(s) to the constructor
         or the load_config method.
         By passing reload=True to the load_config method, you can reload and search again for the config file.
     """
     login: int = 0
+    trade_record_mode: Literal['csv', 'json'] = 'csv'
     password: str = ""
     server: str = ""
     path: str | Path = ""
     timeout: int = 60000
     record_trades: bool = True
     filename: str = "aiomql.json"
-    win_percentage: float = 0.85
-    records_dir: str | Path = 'records'
-    config_dir: str = ''
     _initialize = True
     state: dict = {}
-    root_dir: Path = Path('.').absolute().resolve()
+    root: Path
+    root_dir: Path
+    records_dir: Path
+    config_dir: str = ''
     task_queue: TaskQueue = TaskQueue()
-    bot: 'Bot' = None
+    bot: Bot = None
     _instance: 'Config'
 
     def __new__(cls, *args, **kwargs):
         if not hasattr(cls, "_instance"):
             cls._instance = super().__new__(cls)
         return cls._instance
 
     def __init__(self, **kwargs):
         reload = kwargs.pop('reload', False)
-        root_dir = kwargs.pop('root_dir', None)
-        setattr(self, 'root_dir', root_dir) if root_dir else ...
-        [setattr(self, key, value) for key, value in kwargs.items()]
-        self.load_config(reload=reload)
+        self.load_config(reload=reload, **kwargs)
+
+    def set_root(self, *, root: str | Path):
+        root = Path(root) if str else root
+        self.root = root.absolute().resolve()
+        self.root_dir = self.root
 
     def __setattr__(self, key, value):
-        if key == 'root_dir':
-            value = Path(value).absolute().resolve()
-        if key == 'records_dir':
-            self.create_records_dir(records_dir=value)
-            return
         if key == 'path':
-            value = self.root_dir / Path(value) if not Path(value).exists() else value
+            value = str(self.root_dir / Path(value).absolute().resolve())
         super().__setattr__(key, value)
 
     @staticmethod
     def walk_to_root(path: str | Path) -> Iterator[str]:
         if not os.path.exists(path):
             raise IOError("Starting path not found")
 
@@ -92,48 +92,61 @@
                 if os.path.isfile(check_path):
                     return check_path
             return None
         except Exception as _:
             return
 
     def create_records_dir(self, *, records_dir: str | Path = 'records'):
-        """Create records directory if it does not exist. Relative to the root directory of the project.
+        """Create records directory if it does not exist. By default, it is relative to the root directory of the
+         project unless an absolute path is provided.
+
         Keyword Args:
-            records_dir (str|Path): The name of the directory to create
+            records_dir (str|Path): The directory to save trade records. Default is 'records'
         """
         try:
-            records_dir = Path(records_dir) if isinstance(records_dir, str) else records_dir
-            records_dir = self.root_dir / records_dir
+            if isinstance(records_dir, str):
+                records_dir = self.root_dir / records_dir
+            elif isinstance(records_dir, Path):
+                records_dir = records_dir.absolute().resolve()
             records_dir.mkdir(parents=True, exist_ok=True)
-            super().__setattr__('records_dir', records_dir)
-            return records_dir
+            self.records_dir = records_dir
         except Exception as err:
             logger.warning(f"{err}: Unable to create records directory")
 
-    def load_config(self, *, file: str = None, reload: bool = True, filename: str = None, config_dir: str = ''):
+    def load_config(self, *, file: str = None, reload: bool = True, filename: str = None,
+                    config_dir: str = '', **kwargs):
         """Load configuration settings from a file.
         Keyword Args:
             file (str): The path to the file to load. If not provided, the file is searched for
             reload (bool): Whether to reload the config object. Default is True
             filename (str): The name of the file to load. If not provided, the default filename is used
             config_dir (str): The name of the directory to search for the file. Default is the root directory
+            root_dir (str): The root directory of the project
+            kwargs: Additional keyword arguments
         """
         if not (self._initialize or reload):
             return
-        self._initialize = False
         data = {}
         self.filename = filename or self.filename
         self.config_dir = config_dir or self.config_dir
+        root_dir = kwargs.pop('root_dir', None)
+        records_dir = kwargs.pop('records_dir', 'records')
+        if self._initialize or (root_dir is not None):
+            self.set_root(root=(root_dir or '.'))
+            self.create_records_dir(records_dir=records_dir)
+
         if (file := (file or self.find_config())) is None:
             logger.warning("No Config File Found")
         else:
             fh = open(file, mode="r")
             data = json.load(fh)
             fh.close()
+        data |= kwargs
         [setattr(self, key, value) for key, value in data.items()]
+        self._initialize = False
 
     def account_info(self) -> dict[str, int | str]:
         """Returns Account login details as found in the config object if available
 
         Returns:
             dict: A dictionary of login details
         """
```

### Comparing `aiomql-3.20/src/aiomql/core/constants.py` & `aiomql-3.21/src/aiomql/core/constants.py`

 * *Files identical despite different names*

### Comparing `aiomql-3.20/src/aiomql/core/errors.py` & `aiomql-3.21/src/aiomql/core/errors.py`

 * *Files identical despite different names*

### Comparing `aiomql-3.20/src/aiomql/core/exceptions.py` & `aiomql-3.21/src/aiomql/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiomql-3.20/src/aiomql/core/meta_trader.py` & `aiomql-3.21/src/aiomql/core/meta_trader.py`

 * *Files 2% similar despite different names*

```diff
@@ -306,47 +306,46 @@
 
     async def order_send(self, request: dict) -> OrderSendResult:
         return await asyncio.to_thread(self._order_send, request)
 
     async def positions_total(self) -> int:
         return await asyncio.to_thread(self._positions_total)
 
-    async def positions_get(self, group: str = "", ticket: int = 0, symbol: str = "") -> tuple[TradePosition] | None:
+    async def positions_get(self, group: str = "", ticket: int = None, symbol: str = "") -> tuple[TradePosition] | None:
         kwargs = {key: value for key, value in (('group', group), ('ticket', ticket), ('symbol', symbol)) if value}
         res = await asyncio.to_thread(self._positions_get, **kwargs)
         if res is None:
             err = await self.last_error()
             self.error = Error(*err)
             logger.warning(f'Error in obtaining open positions.{self.error.description}')
             return res
         return res
 
     async def history_orders_total(self, date_from: datetime | float, date_to: datetime | float) -> int:
         return await asyncio.to_thread(self._history_orders_total, date_from, date_to)
 
     async def history_orders_get(self, date_from: datetime | float = None, date_to: datetime | float = None,
-                                 group: str = '',
-                                 ticket: int = 0, position: int = 0) -> tuple[TradeOrder] | None:
-        kwargs = {key: value for key, value in (('date_from', date_from), ('date_to', date_to), ('group', group),
-                                                ('ticket', ticket), ('position', position)) if value}
-        res = await asyncio.to_thread(self._history_orders_get, **kwargs)
+                                 group: str = '', ticket: int = None, position: int = None) -> tuple[TradeOrder] | None:
+        kwargs = {key: value for key, value in (('group', group), ('ticket', ticket), ('position', position)) if value}
+        args = tuple(arg for arg in (date_from, date_to) if arg)
+        res = await asyncio.to_thread(self._history_orders_get, *args, **kwargs)
         if res is None:
             err = await self.last_error()
             self.error = Error(*err)
             logger.warning(f'Error in getting orders.{self.error.description}')
             return res
         return res
 
     async def history_deals_total(self, date_from: datetime | float, date_to: datetime | float) -> int:
         return await asyncio.to_thread(self._history_deals_total, date_from, date_to)
 
     async def history_deals_get(self, date_from: datetime | float = None, date_to: datetime | float = None,
-                                group: str = '', ticket: int = 0, position: int = 0) -> tuple[TradeDeal] | None:
-        kwargs = {key: value for key, value in (('date_from', date_from), ('date_to', date_to), ('group', group),
-                                                ('ticket', ticket), ('position', position)) if value}
-        res = await asyncio.to_thread(self._history_deals_get, **kwargs)
+                                group: str = '', ticket: int = None, position: int = None) -> tuple[TradeDeal] | None:
+        kwargs = {key: value for key, value in (('group', group), ('ticket', ticket), ('position', position)) if value}
+        args = tuple(arg for arg in (date_from, date_to) if arg)
+        res = await asyncio.to_thread(self._history_deals_get, *args, **kwargs)
         if res is None:
             err = await self.last_error()
             self.error = Error(*err)
             logger.warning(f'Error in getting deals.{self.error.description}')
             return res
         return res
```

### Comparing `aiomql-3.20/src/aiomql/core/models.py` & `aiomql-3.21/src/aiomql/core/models.py`

 * *Files identical despite different names*

### Comparing `aiomql-3.20/src/aiomql/core/task_queue.py` & `aiomql-3.21/src/aiomql/core/task_queue.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,16 @@
     async def run(self):
         try:
             if asyncio.iscoroutinefunction(self.task):
                 return await self.task(*self.args, **self.kwargs)
             else:
                 return self.task(*self.args, **self.kwargs)
         except Exception as err:
-            logger.error(f'Error in running {self.task.__name__} with {str(self.args)}, {self.kwargs}: {err}')
+            logger.error(f"Error in running {getattr(self.task, '__name__', str(self.task))}"
+                         f" with {str(self.args)}, {self.kwargs}: {err}")
 
 
 class TaskQueue:
     def __init__(self):
         self.queue = asyncio.Queue()
 
     def add(self, item: QueueItem):
```

### Comparing `aiomql-3.20/src/aiomql/executor.py` & `aiomql-3.21/src/aiomql/executor.py`

 * *Files identical despite different names*

### Comparing `aiomql-3.20/src/aiomql/history.py` & `aiomql-3.21/src/aiomql/order.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,133 +1,137 @@
 import asyncio
-from datetime import datetime
 from logging import getLogger
 
-from .core.config import Config
-from .core.meta_trader import MetaTrader
-from .core.models import TradeDeal, TradeOrder
-
+from .core.models import TradeRequest, OrderSendResult, OrderCheckResult, TradeOrder
+from .core.constants import TradeAction, OrderTime, OrderFilling
+from .core.exceptions import OrderError
 logger = getLogger(__name__)
 
 
-class History:
-    """The history class handles completed trade deals and trade orders in the trading history of an account.
+class Order(TradeRequest):
+    """Trade order related functions and properties. Subclass of TradeRequest."""
 
-    Attributes:
-        deals (list[TradeDeal]): Iterable of trade deals
-        orders (list[TradeOrder]): Iterable of trade orders
-        total_deals: Total number of deals
-        total_orders (int): Total number orders
-        group (str): Filter for selecting history by symbols.
-        ticket (int): Filter for selecting history by ticket number
-        position (int): Filter for selecting history deals by position
-        initialized (bool): check if initial request has been sent to the terminal to get history.
-        mt5 (MetaTrader): MetaTrader instance
-        config (Config): Config instance
-    """
-    mt5: MetaTrader
-    config: Config
+    def __init__(self, **kwargs):
+        """Initialize the order object with keyword arguments, symbol must be provided.
+        Provide default values for action, type_time and type_filling if not provided.
 
-    def __init__(self, *, date_from: datetime | float = None, date_to: datetime | float = None,
-                 group: str = "", ticket: int = 0, position: int = 0):
-        """
         Args:
-            date_from (datetime, float): Date the orders are requested from. Set by the 'datetime' object or as a
-                number of seconds elapsed since 1970.01.01. Defaults to twenty-four hours from the current time in 'utc'
+            **kwargs: Keyword arguments must match the attributes of TradeRequest as well as the attributes of
+             Order class as specified in the annotations in the class definition.
 
-            date_to (datetime, float): Date up to which the orders are requested. Set by the 'datetime' object or as a
-                number of seconds elapsed since 1970.01.01. Defaults to the current time in "utc"
+        Default Values:
+            action (TradeAction.DEAL): Trade action
+            type_time (OrderTime.DAY): Order time
+            type_filling (OrderFilling.FOK): Order filling
+        """
+        if 'symbol' in kwargs:
+            kwargs['symbol'] = str(kwargs['symbol'])
+        self.action = kwargs.pop('action', TradeAction.DEAL)
+        self.type_time = kwargs.pop('type_time', OrderTime.DAY)
+        self.type_filling = kwargs.pop('type_filling', OrderFilling.FOK)
+        super().__init__(**kwargs)
 
-            group (str): Filter for selecting history by symbols.
-            ticket (int): Filter for selecting history by ticket number
-            position (int): Filter for selecting history deals by position
-        """
-        self.config = Config()
-        self.mt5 = MetaTrader()
-        self.date_from = date_from
-        self.date_to = date_to
-        self.group = group
-        self.ticket = ticket
-        self.position = position
-        self.deals: list[TradeDeal] = []
-        self.orders: list[TradeOrder] = []
-        self.total_deals: int = 0
-        self.total_orders: int = 0
-        self.initialized = False
-
-    async def init(self, deals=True, orders=True) -> bool:
-        """Get history deals and orders
-
-        Keyword Args:
-            deals (bool): If true get history deals during initial request to terminal
-            orders (bool): If true get history orders during initial request to terminal
+    async def orders_total(self):
+        """Get the number of active orders.
 
         Returns:
-            bool: True if all requests were successful else False
+            (int): total number of active orders
         """
-        tasks = []
-        tasks.append(self.get_deals()) if deals else ...
-        tasks.append(self.get_orders()) if orders else ...
-        res = await asyncio.gather(*tasks)
-        self.initialized = all(res)
-        return self.initialized
+        return await self.mt5.orders_total()
 
-    async def get_deals(self, retries=3) -> list[TradeDeal]:
-        """Get deals from trading history using the parameters set in the constructor.
+    async def get_order(self, *, ticket: int, retries: int = 3) -> TradeOrder:
+        """
+        Get the order by ticket number.
+        Args:
+            ticket (int): Order ticket number
+            retries (int): Number of retries
+        Returns:
+        """
+        if retries < 1:
+            raise OrderError(f'Failed to get orders for {self.symbol}: {self.mt5.error}')
+        orders = await self.mt5.orders_get(ticket=ticket)
+        if orders is not None:
+            order = TradeOrder(**orders[0]._asdict())
+            assert order.ticket == ticket, f'Order ticket mismatch {order.ticket} != {ticket}'
+            return order
+        if self.mt5.error.is_connection_error():
+            await asyncio.sleep(retries)
+            return await self.get_order(ticket=ticket, retries=retries-1)
+        raise OrderError(f'Failed to get orders for {self.symbol}: {self.mt5.error}')
 
+    async def get_orders(self, *, ticket: int = 0, symbol: str = '', group: str = '', retries=3)\
+            -> tuple[TradeOrder, ...]:
+        """Get the list of active orders for the current symbol.
+        Keyword Args:
+            ticket (int): Order ticket number
+            symbol (str): Symbol name
+            group (str): Group name
         Returns:
-            list[TradeDeal]: A list of trade deals
+            tuple[TradeOrder]: A Tuple of active trade orders as TradeOrder objects
         """
         if retries < 1:
-            logger.warning(f'Failed to get deals: {self.mt5.error}')
-            return []
-        deals = await self.mt5.history_deals_get(date_from=self.date_from, date_to=self.date_to, position=self.position,
-                                                 group=self.group, ticket=self.ticket)
-        if deals is not None:
-            self.deals = [TradeDeal(**deal._asdict()) for deal in deals]
-            self.total_deals = len(self.deals)
-            return self.deals
+            raise OrderError(f'Failed to get orders for {self.symbol}: {self.mt5.error}')
+        symbol = getattr(self, 'symbol', symbol)
+        orders = await self.mt5.orders_get(symbol=symbol, ticket=ticket, group=group)
+        if orders is not None:
+            orders = (TradeOrder(**order._asdict()) for order in orders)
+            return tuple(orders)
         if self.mt5.error.is_connection_error():
             await asyncio.sleep(retries)
-            return await self.get_deals(retries=retries - 1)
+            return await self.get_orders(ticket=ticket, symbol=symbol, group=group, retries=retries-1)
+        raise OrderError(f'Failed to get orders for {self.symbol}: {self.mt5.error}')
 
-        logger.warning(f'Failed to get deals: {self.mt5.error}')
-        return []
+    async def check(self) -> OrderCheckResult:
+        """Check funds sufficiency for performing a required trading operation and the possibility of executing it.
 
-    async def deals_total(self) -> int:
-        """Get total number of deals within the specified period in the constructor.
+        Returns:
+            OrderCheckResult: An OrderCheckResult object
+
+        Raises:
+            OrderError: If not successful
+        """
+        res = await self.mt5.order_check(self.dict)
+        if res is None:
+            raise OrderError(f'Failed to check order due to {self.mt5.error.description}')
+        return OrderCheckResult(**res._asdict())
+
+    async def send(self) -> OrderSendResult:
+        """Send a request to perform a trading operation from the terminal to the trade server.
 
         Returns:
-            int: Total number of Deals
+             OrderSendResult: An OrderSendResult object
+
+        Raises:
+            OrderError: If not successful
         """
-        self.total_deals = await self.mt5.history_deals_total(self.date_from, self.date_to)
-        return self.total_deals
+        res = await self.mt5.order_send(self.dict)
+        if res is None:
+            raise OrderError(f'Failed to send order {self.symbol} due to {self.mt5.error.description}')
+        return OrderSendResult(**res._asdict())
 
-    async def get_orders(self, retries=3) -> list[TradeOrder]:
-        """Get orders from trading history using the parameters set in the constructor.
+    async def calc_margin(self) -> float:
+        """Return the required margin in the account currency to perform a specified trading operation.
 
         Returns:
-            list[TradeOrder]: A list of trade orders
+            float: Returns float value if successful
+
+        Raises:
+            OrderError: If not successful
         """
-        if retries < 1:
-            logger.warning(f'Failed to get orders: {self.mt5.error}')
-            return []
-        orders = await self.mt5.history_orders_get(date_from=self.date_from, date_to=self.date_to, group=self.group,
-                                                   position=self.position, ticket=self.ticket)
-        if orders is not None:
-            self.orders = [TradeOrder(**order._asdict()) for order in orders]
-            self.total_orders = len(self.orders)
-            return self.orders
-        if self.mt5.error.is_connection_error():
-            await asyncio.sleep(retries)
-            return await self.get_orders(retries=retries - 1)
-        logger.warning(f'Failed to get orders: {self.mt5.error}')
-        return []
+        res = await self.mt5.order_calc_margin(self.type, self.symbol, self.volume, self.price)
+        if res is None:
+            raise OrderError(f'Failed to calculate margin for {self.symbol} due to {self.mt5.error.description}')
+        return res
 
-    async def orders_total(self) -> int:
-        """Get total number of orders within the specified period in the constructor.
+    async def calc_profit(self) -> float:
+        """Return profit in the account currency for a specified trading operation.
 
         Returns:
-            int: Total number of orders
+            float: Returns float value if successful
+
+        Raises:
+            OrderError: If not successful
         """
-        self.total_orders = await self.mt5.history_orders_total(self.date_from, self.date_to)
-        return self.total_orders
+        res = await self.mt5.order_calc_profit(self.type, self.symbol, self.volume, self.price, self.tp)
+        if res is None:
+            raise OrderError(f'Failed to calculate profit for {self.symbol} due to {self.mt5.error.description}')
+        return res
```

### Comparing `aiomql-3.20/src/aiomql/lib/strategies/finger_trap.py` & `aiomql-3.21/src/aiomql/lib/strategies/finger_trap.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,23 +65,21 @@
             candles = await self.symbol.copy_rates_from_pos(timeframe=self.etf, count=self.ecc)
             if not ((current := candles[-1].time) >= self.tracker.entry_time):
                 self.tracker.update(new=False, order_type=None)
                 return
             self.tracker.update(new=True, entry_time=current)
             candles.ta.ema(length=self.entry_ema, append=True)
             candles.rename(**{f"EMA_{self.entry_ema}": "ema"})
-            cae = candles.ta_lib.cross(candles.close, candles.ema)
-            cbe = candles.ta_lib.cross(candles.close, candles.ema, above=False)
-            trend = self.ttf.time // self.etf.time
-            bull_trend = cae.iloc[-trend:]
-            bear_trend = cbe.iloc[-trend:]
-            if self.tracker.bullish and any(bull_trend):
+            candles['cae'] = candles.ta_lib.cross(candles.close, candles.ema)
+            candles['cbe'] = candles.ta_lib.cross(candles.close, candles.ema, above=False)
+            current = candles[-1]
+            if self.tracker.bullish and current.cae:
                 sl = find_bullish_fractal(candles).low
                 self.tracker.update(snooze=self.ttf.time, order_type=OrderType.BUY, sl=sl)
-            elif self.tracker.bearish and any(bear_trend):
+            elif self.tracker.bearish and current.cbe:
                 sl = find_bearish_fractal(candles).high
                 self.tracker.update(snooze=self.ttf.time, order_type=OrderType.SELL, sl=sl)
             else:
                 self.tracker.update(snooze=self.etf.time, order_type=None)
         except Exception as err:
             logger.error(f"{err} for {self.symbol} in {self.__class__.__name__}.confirm_trend")
             self.tracker.update(snooze=self.etf.time, order_type=None)
```

### Comparing `aiomql-3.20/src/aiomql/lib/strategies/tracker.py` & `aiomql-3.21/src/aiomql/lib/strategies/tracker.py`

 * *Files identical despite different names*

### Comparing `aiomql-3.20/src/aiomql/lib/symbols/forex_symbol.py` & `aiomql-3.21/src/aiomql/lib/symbols/forex_symbol.py`

 * *Files identical despite different names*

### Comparing `aiomql-3.20/src/aiomql/lib/traders/simple_trader.py` & `aiomql-3.21/src/aiomql/lib/traders/simple_trader.py`

 * *Files identical despite different names*

### Comparing `aiomql-3.20/src/aiomql/order.py` & `aiomql-3.21/src/aiomql/trader.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,117 +1,133 @@
-import asyncio
+"""Trader class module. Handles the creation of an order and the placing of trades"""
+from abc import ABC, abstractmethod
+from datetime import datetime
+from typing import TypeVar
 from logging import getLogger
+from zoneinfo import ZoneInfo
 
-from .core.models import TradeRequest, OrderSendResult, OrderCheckResult, TradeOrder
-from .core.constants import TradeAction, OrderTime, OrderFilling
-from .core.exceptions import OrderError
-logger = getLogger(__name__)
-
-
-class Order(TradeRequest):
-    """Trade order related functions and properties. Subclass of TradeRequest."""
-
-    def __init__(self, **kwargs):
-        """Initialize the order object with keyword arguments, symbol must be provided.
-        Provide default values for action, type_time and type_filling if not provided.
+from .order import Order
+from .symbol import Symbol as _Symbol
+from .ticks import Tick
+from .ram import RAM
+from .core.models import OrderType, OrderSendResult
+from .core.config import Config
+from .utils import dict_to_string
+from .result import Result
 
-        Args:
-            **kwargs: Keyword arguments must match the attributes of TradeRequest as well as the attributes of
-             Order class as specified in the annotations in the class definition.
-
-        Default Values:
-            action (TradeAction.DEAL): Trade action
-            type_time (OrderTime.DAY): Order time
-            type_filling (OrderFilling.FOK): Order filling
-        """
-        if 'symbol' in kwargs:
-            kwargs['symbol'] = str(kwargs['symbol'])
-        self.action = kwargs.pop('action', TradeAction.DEAL)
-        self.type_time = kwargs.pop('type_time', OrderTime.DAY)
-        self.type_filling = kwargs.pop('type_filling', OrderFilling.FOK)
-        super().__init__(**kwargs)
+logger = getLogger(__name__)
+Symbol = TypeVar("Symbol", bound=_Symbol)
 
-    async def orders_total(self):
-        """Get the number of active orders.
 
-        Returns:
-            (int): total number of active orders
-        """
-        return await self.mt5.orders_total()
+class Trader(ABC):
+    """Base class for creating a Trader object. Handles the creation of an order and the placing of trades.
 
-    async def get_orders(self, *, ticket: int = 0, symbol: str = '', group: str = '', retries=3)\
-            -> tuple[TradeOrder, ...]:
-        """Get the list of active orders for the current symbol.
-        Keyword Args:
-            ticket (int): Order ticket number
-            symbol (str): Symbol name
-            group (str): Group name
-        Returns:
-            tuple[TradeOrder]: A Tuple of active trade orders as TradeOrder objects
-        """
-        if retries < 1:
-            raise OrderError(f'Failed to get orders for {self.symbol}: {self.mt5.error}')
-        symbol = getattr(self, 'symbol', symbol)
-        orders = await self.mt5.orders_get(symbol=symbol, ticket=ticket, group=group)
-        if orders is not None:
-            orders = (TradeOrder(**order._asdict()) for order in orders)
-            return tuple(orders)
-        if self.mt5.error.is_connection_error():
-            await asyncio.sleep(retries)
-            return await self.get_orders(ticket=ticket, symbol=symbol, group=group, retries=retries-1)
-        raise OrderError(f'Failed to get orders for {self.symbol}: {self.mt5.error}')
+    Attributes:
+        symbol (Symbol): The financial instrument.
+        ram (RAM): RAM instance
+        order (Order): Trade order
 
-    async def check(self) -> OrderCheckResult:
-        """Check funds sufficiency for performing a required trading operation and the possibility of executing it.
+    Class Attributes:
+        config (Config): Config instance.
+    """
+    config: Config
 
-        Returns:
-            OrderCheckResult: An OrderCheckResult object
+    def __init__(self, *, symbol: Symbol, ram: RAM = None):
+        """Initializes the order object and RAM instance
 
-        Raises:
-            OrderError: If not successful
+        Args:
+            symbol (Symbol): Financial instrument
+            ram (RAM): Risk Assessment and Management instance
         """
-        res = await self.mt5.order_check(self.dict)
-        if res is None:
-            raise OrderError(f'Failed to check order due to {self.mt5.error.description}')
-        return OrderCheckResult(**res._asdict())
-
-    async def send(self) -> OrderSendResult:
-        """Send a request to perform a trading operation from the terminal to the trade server.
+        self.config = Config()
+        self.symbol = symbol
+        self.order = Order(symbol=symbol.name)
+        self.ram = ram or RAM()
+        self.parameters = {}
 
-        Returns:
-             OrderSendResult: An OrderSendResult object
+    def set_order_limits(self, *, pips: float, tick: Tick):
+        """Sets the stop loss and take profit for the order. This method uses pips as defined for forex instruments.
 
-        Raises:
-            OrderError: If not successful
+        Args:
+            pips: Target pips
+            tick: Tick object
         """
-        res = await self.mt5.order_send(self.dict)
-        if res is None:
-            raise OrderError(f'Failed to send order {self.symbol} due to {self.mt5.error.description}')
-        return OrderSendResult(**res._asdict())
-
-    async def calc_margin(self) -> float:
-        """Return the required margin in the account currency to perform a specified trading operation.
+        pips = pips * self.symbol.pip
+        sl, tp = pips, pips * self.ram.risk_to_reward
+        if self.order.type == OrderType.BUY:
+            self.order.sl, self.order.tp = round(tick.ask - sl, self.symbol.digits), round(tick.ask + tp,
+                                                                                           self.symbol.digits)
+            self.order.price = tick.ask
+        elif self.order.type == OrderType.SELL:
+            self.order.sl, self.order.tp = round(tick.bid + sl, self.symbol.digits), round(tick.bid - tp,
+                                                                                           self.symbol.digits)
+            self.order.price = tick.bid
+        else:
+            raise ValueError(f"Invalid order type: {self.order.type}")
 
-        Returns:
-            float: Returns float value if successful
+    def set_trade_stop_levels(self, *, points: float, tick: Tick):
+        """Set the stop loss and take profit levels of the order based on the points and price tick.
 
-        Raises:
-            OrderError: If not successful
+        Args:
+            points: Target points
+            tick: Tick object
         """
-        res = await self.mt5.order_calc_margin(self.type, self.symbol, self.volume, self.price)
-        if res is None:
-            raise OrderError(f'Failed to calculate margin for {self.symbol} due to {self.mt5.error.description}')
-        return res
-
-    async def calc_profit(self) -> float:
-        """Return profit in the account currency for a specified trading operation.
-
-        Returns:
-            float: Returns float value if successful
+        points = points * self.symbol.point
+        sl, tp = points, points * self.ram.risk_to_reward
+        if self.order.type == OrderType.BUY:
+            self.order.sl, self.order.tp = round(tick.ask - sl, self.symbol.digits), round(tick.ask + tp,
+                                                                                           self.symbol.digits)
+            self.order.price = tick.ask
+        else:
+            self.order.sl, self.order.tp = round(tick.bid + sl, self.symbol.digits), round(tick.bid - tp,
+                                                                                           self.symbol.digits)
+            self.order.price = tick.bid
+
+    async def check_order(self) -> bool:
+        """Check order before sending it to the broker.
+
+        Returns:
+            bool: True if order can go through else false
+        """
+        check = await self.order.check()
+        if check.retcode != 0:
+            req = check.request._asdict() | check.get_dict(include={'comment', 'retcode'})
+            logger.warning(f"Invalid order for {self.symbol}: {dict_to_string(req)}")
+            return False
+        return True
+
+    async def send_order(self) -> OrderSendResult:
+        """Send the order to the broker."""
+        result = await self.order.send()
+        if result.retcode != 10009:
+            req = result.request._asdict() | result.get_dict(include={'comment', 'retcode'})
+            logger.warning(f"Unable to place order for {self.symbol}: {dict_to_string(req)}")
+            return result
+        res = result.get_dict(exclude={'request', 'retcode_external', 'retcode', 'request_id'})
+        logger.info(f"Placed Trade for {self.symbol}: {dict_to_string(res)}")
+        await self.record_trade(result, parameters=self.parameters.copy())
+        return result
 
-        Raises:
-            OrderError: If not successful
-        """
-        res = await self.mt5.order_calc_profit(self.type, self.symbol, self.volume, self.price, self.tp)
-        if res is None:
-            raise OrderError(f'Failed to calculate profit for {self.symbol} due to {self.mt5.error.description}')
-        return res
+    async def record_trade(self, result: OrderSendResult, parameters: dict = None, name: str = '', exclude: set = None):
+        """Record the trade in csv or json.
+        Args:
+            result (OrderSendResult): Result of the order send
+            parameters: parameters of the trading strategy used to place the trade
+            name: Name of the trading strategy
+            exclude: Exclude these fields from the recorded trade
+        """
+        if result.retcode != 10009 or not self.config.record_trades:
+            return
+        params = parameters or self.parameters.copy()
+        params = {k: v for k, v in params.items() if k not in (exclude or set())}
+        profit = await self.order.calc_profit()
+        params["expected_profit"] = profit
+        date = datetime.utcnow()
+        date = date.replace(tzinfo=ZoneInfo("UTC"))
+        params["date"] = str(date.date())
+        params["time"] = str(date.time())
+        res = Result(result=result, parameters=params, name=name)
+        self.config.task_queue.add_task(res.save)
+
+    @abstractmethod
+    async def place_trade(self, *args, **kwargs):
+        """Places a trade based on the order_type."""
```

### Comparing `aiomql-3.20/src/aiomql/positions.py` & `aiomql-3.21/src/aiomql/positions.py`

 * *Files 17% similar despite different names*

```diff
@@ -64,36 +64,63 @@
             return [TradePosition(**pos._asdict()) for pos in positions]
         if self.mt5.error.is_connection_error():
             await asyncio.sleep(retries)
             return await self.positions_get(symbol, group, ticket, retries - 1)
         logger.warning(f'Failed to get positions for {symbol or self.symbol}. {self.mt5.error}')
         return []
 
-    async def close(self, *, ticket: int, symbol: str, price: float, volume: float, order_type: OrderType):
-        """Close an open position for the trading account."""
+    async def position_get(self, *, ticket: int) -> TradePosition:
+        """Get an open position by ticket.
+        Args:
+            ticket (int): Position ticket.
+
+        Returns:
+            TradePosition: Return an open position
+        """
+        positions = await self.positions_get(ticket=ticket)
+        position = positions[0] if positions else None
+        if position is None:
+            raise ValueError(f'Position with ticket {ticket} not found')
+        assert position.ticket == ticket, f'Position with ticket {ticket} not found'
+        return position
 
+    async def close(self, *, ticket: int, symbol: str, price: float, volume: float, order_type: OrderType):
+        """Close an open position for the trading account using the ticket and other parameters.
+        Args:
+            ticket (int): Position ticket.
+            symbol (str): Financial instrument name.
+            price (float): Closing price.
+            volume (float): Volume to close.
+            order_type (OrderType): Order type.
+        """
         order = Order(action=TradeAction.DEAL, price=price, position=ticket, symbol=symbol, volume=volume,
                       type=order_type.opposite)
         return await order.send()
 
     async def close_by(self, pos: TradePosition):
         """Close an open position for the trading account."""
         order = Order(position=pos.ticket, symbol=pos.symbol, volume=pos.volume, type=pos.type.opposite,
                       price=pos.price_current)
         return await order.send()
 
+    async def close_position(self, *, position: TradePosition):
+        """Close an open position for the trading account. Using a position object."""
+        order = Order(position=position.ticket, symbol=position.symbol, volume=position.volume,
+                      type=position.type.opposite, price=position.price_current)
+        return await order.send()
+
     async def close_all(self, symbol: str = '', group: str = '') -> int:
         """Close all open positions for the trading account. Specify a symbol or group to filter positions.
 
         Keyword Args:
             symbol (str): Financial instrument name.
             group (str): The filter for specifying a group of symbols.
 
         Returns:
             int: Return number of positions closed.
         """
         symbol = symbol or self.symbol
         group = group or self.group
         positions = [pos for pos in await self.positions_get(symbol=symbol, group=group)]
-        orders = [self.close_by(pos) for pos in positions]
+        orders = [self.close_position(position=pos) for pos in positions]
         results = await asyncio.gather(*[order for order in orders], return_exceptions=True)
         return len([res for res in results if (res and res.retcode) == 10009])
```

### Comparing `aiomql-3.20/src/aiomql/ram.py` & `aiomql-3.21/src/aiomql/ram.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 
 class RAM:
     account: Account
     risk_to_reward: float
     risk: float
     points: float
     pips: float
-    min_amount: float
-    max_amount: float
-    balance_level: float = 10
+    min_amount: float = 0
+    max_amount: float = 0
+    risk_level: float = 50
     loss_limit: int = 3
+    open_limit: int = 6
 
     def __init__(self, *, risk_to_reward: float = 1, risk: float = 0.01, **kwargs):
         """Initialize Risk Assessment and Management with the provided keyword arguments.
 
         Keyword Args:
             risk_to_reward (float): Risk to reward ratio. Defaults to 1
             risk (float): Percentage of account balance to risk per trade 0.01 # 1%
@@ -24,27 +25,42 @@
         """
         self.risk_to_reward = risk_to_reward
         self.risk = risk
         self.account = Account()
         [setattr(self, key, value) for key, value in kwargs.items()]
 
     async def get_amount(self) -> float:
-        """Calculate the amount to risk per trade as a percentage of balance.
+        """Calculate the amount to risk per trade as a percentage of equity.
 
         Returns:
             float: Amount to risk per trade
         """
         await self.account.refresh()
-        return self.account.balance * self.risk
+        amount = self.account.margin_free * self.risk
+        if self.min_amount and self.max_amount:
+            return max(self.min_amount, min(self.max_amount, amount))
+        return amount
 
-    async def check_losing_positions(self) -> bool:
-        """Check if the number of losing positions is greater than or equal the loss limit."""
-        positions = await Positions().positions_get()
-        positions.sort(key=lambda pos: pos.time_msc)
+    async def check_losing_positions(self, *, symbol: str = '') -> bool:
+        """Check if the number of losing positions is greater than or equal the loss limit.
+
+        Args:
+            symbol (str): Symbol to check. Defaults to ''.
+        """
+        positions = await Positions().positions_get(symbol=symbol)
         loosing = [trade for trade in positions if trade.profit <= 0]
         return len(loosing) >= self.loss_limit
 
-    async def check_balance_level(self) -> bool:
-        """Check if the balance level is greater than or equal to the balance level."""
+    async def check_open_positions(self, *, symbol: str = '') -> bool:
+        """Check if the number of open positions is greater than or equal the loss limit.
+
+        Args:
+            symbol (str): Symbol to check. Defaults to ''.
+        """
+        positions = await Positions().positions_get(symbol=symbol)
+        return len(positions) >= self.open_limit
+
+    async def check_risk_level(self) -> bool:
+        """Check the risk level."""
         await self.account.refresh()
-        balance_level = (self.account.margin / self.account.balance) * 100
-        return balance_level >= self.balance_level
+        risk_level = (1 - (self.account.margin_free / self.account.equity)) * 100
+        return risk_level >= self.risk_level
```

### Comparing `aiomql-3.20/src/aiomql/records.py` & `aiomql-3.21/src/aiomql/records.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """This module contains the Records class, which is used to read and update trade records from csv files."""
 
 import asyncio
 from pathlib import Path
 import csv
 import logging
+from typing import Iterable
 
 from .core import Config, MetaTrader
 
 logger = logging.getLogger(__name__)
 
 
 class Records:
@@ -46,15 +47,15 @@
         """Read and update trade records
 
         Args:
             file: Trade record file
         """
         try:
             fr = open(file, mode='r', newline='')
-            reader = csv.DictReader(fr)
+            reader: Iterable[dict] | csv.DictReader = csv.DictReader(fr)
             rows = [row for row in reader]
             rows = await self.update_rows(rows)
             fr.close()
             fw = open(file, mode='w', newline='')
             writer = csv.DictWriter(fw, fieldnames=reader.fieldnames, extrasaction='ignore', restval=None)
             writer.writeheader()
             writer.writerows(rows)
```

### Comparing `aiomql-3.20/src/aiomql/result.py` & `aiomql-3.21/src/aiomql/result.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import csv
+import json
 from logging import getLogger
-from threading import RLock
-from pathlib import Path
+from typing import Iterable, Literal
 
 from .core import Config
 from .core.models import OrderSendResult
 
 logger = getLogger(__name__)
 
 
@@ -27,30 +27,68 @@
             parameters:
             name:
         """
         self.config = Config()
         self.parameters = parameters or {}
         self.result = result
         self.name = name or parameters.get('name', 'Trades')
-        if not Path(self.config.records_dir).exists():
-            Path(self.config.records_dir).mkdir(parents=True, exist_ok=True)
 
     def get_data(self) -> dict:
         res = self.result.get_dict(exclude={'retcode', 'comment', 'retcode_external', 'request_id', 'request'})
         return self.parameters | res | {'actual_profit': 0, 'closed': False, 'win': False}
 
+    async def save(self, *, trade_record_mode: Literal['csv', 'json'] = None):
+        """Record trade results as a csv or json file
+        Args:
+            trade_record_mode (Literal['csv'|'json']): Mode of saving trade records
+        """
+        trade_record_mode = trade_record_mode or self.config.trade_record_mode
+        if trade_record_mode == 'csv':
+            await self.to_csv()
+        else:
+            await self.to_json()
+
     async def to_csv(self):
         """Record trade results and associated parameters as a csv file
         """
         try:
             data = self.get_data()
             file = self.config.records_dir / f"{self.name}.csv"
-            exists = file.exists()
-            with RLock():
-                with open(file, 'a', newline='') as fh:
-                    f_names = sorted(list(data.keys()))
-                    writer = csv.DictWriter(fh, fieldnames=f_names, extrasaction='ignore', restval=None)
-                    if not exists:
-                        writer.writeheader()
-                    writer.writerow(data)
+            file.touch(exist_ok=True) if not file.exists() else ...
+            reader: Iterable[dict] = csv.DictReader(file.open('r', newline=''))
+            rows: list[dict] = []
+            headers = set()
+            [(rows.append(row), headers.update(row.keys())) for row in reader]
+            rows.append(data)
+            headers.update(data.keys())
+            writer = csv.DictWriter(file.open('w', newline=''), fieldnames=headers, restval=None,
+                                    extrasaction='ignore')
+            writer.writeheader()
+            writer.writerows(rows)
+        except Exception as err:
+            logger.error(f'Unable to save to csv: {err}')
+
+    @staticmethod
+    def serialize(value) -> str:
+        """Serialize the trade records and strategy parameters
+        """
+        try:
+            return str(value)
+        except (ValueError, TypeError) as _:
+            return ""
+
+    async def to_json(self):
+        """Save trades and strategy parameters in a json file
+        """
+        try:
+            file = self.config.records_dir / f"{self.name}.json"
+            data = self.get_data()
+            exists = file.touch(exist_ok=True) if not file.exists() else True
+            if not exists:
+                json.dump([], file.open('w'))
+            with file.open('r') as fh:
+                rows = json.load(fh)
+            rows.append(data)
+            with file.open('w') as fh:
+                json.dump(rows, fh, indent=2, skipkeys=True, default=self.serialize)
         except Exception as err:
-            logger.error(f'Error: {err}. Unable to save trade results')
+            logger.error(f"Unable to save as json file: {err}")
```

### Comparing `aiomql-3.20/src/aiomql/sessions.py` & `aiomql-3.21/src/aiomql/sessions.py`

 * *Files identical despite different names*

### Comparing `aiomql-3.20/src/aiomql/strategy.py` & `aiomql-3.21/src/aiomql/strategy.py`

 * *Files identical despite different names*

### Comparing `aiomql-3.20/src/aiomql/symbol.py` & `aiomql-3.21/src/aiomql/symbol.py`

 * *Files identical despite different names*

### Comparing `aiomql-3.20/src/aiomql/terminal.py` & `aiomql-3.21/src/aiomql/terminal.py`

 * *Files identical despite different names*

### Comparing `aiomql-3.20/src/aiomql/utils.py` & `aiomql-3.21/src/aiomql/utils.py`

 * *Files identical despite different names*

### Comparing `aiomql-3.20/src/aiomql.egg-info/PKG-INFO` & `aiomql-3.21/src/aiomql.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: aiomql
-Version: 3.20
-Summary: Asynchronous MetaTrader5 library and Bot Building Framework
+Version: 3.21
+Summary: Asynchronous MetaTrader5 library and Algorithmic Trading Framework
 Author-email: Ichinga Samuel <ichingasamuel@gmail.com>
 Project-URL: Homepage, https://github.com/Ichinga-Samuel/aiomql
 Project-URL: Bug Tracker, https://github.com/Ichinga-Samuel/aiomql/issues
 Keywords: MetaTrader5,Asynchronous,Algorithmic Trading,Trading Bot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: MetaTrader5>=5.0.37
 Requires-Dist: pandas>=1.5.0
 Requires-Dist: pandas-ta>=0.3.14b0
+Requires-Dist: matplotlib>=3.8.4
+Requires-Dist: mplfinance>=0.12.10b0
 
 # Aiomql - Bot Building Framework and Asynchronous MetaTrader5 Library
 ![GitHub](https://img.shields.io/github/license/ichinga-samuel/aiomql?style=plastic)
 ![GitHub issues](https://img.shields.io/github/issues/ichinga-samuel/aiomql?style=plastic)
 ![PyPI](https://img.shields.io/pypi/v/aiomql)
 
 ### Installation
@@ -31,14 +33,15 @@
 - Asynchronous Bot Building Framework
 - Build bots for trading in different financial markets using a bot factory
 - Use threadpool executors to run multiple strategies on multiple instruments concurrently
 - Records and keep track of trades and strategies in csv files.
 - Helper classes for Bot Building. Easy to use and extend.
 - Compatible with pandas-ta.
 - Sample Pre-Built strategies
+- Visualization of charts using matplotlib and mplfinance
 - Manage Trading periods using Sessions
 - Risk Management
 - Run multiple bots concurrently with different accounts from the same broker or different brokers
 
 ### As an asynchronous MetaTrader5 Libray
 ```python
 import asyncio
```

### Comparing `aiomql-3.20/src/aiomql.egg-info/SOURCES.txt` & `aiomql-3.21/src/aiomql.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 src/aiomql/records.py
 src/aiomql/result.py
 src/aiomql/sessions.py
 src/aiomql/strategy.py
 src/aiomql/symbol.py
 src/aiomql/terminal.py
 src/aiomql/ticks.py
+src/aiomql/trade_records.py
 src/aiomql/trader.py
 src/aiomql/utils.py
 src/aiomql.egg-info/PKG-INFO
 src/aiomql.egg-info/SOURCES.txt
 src/aiomql.egg-info/dependency_links.txt
 src/aiomql.egg-info/requires.txt
 src/aiomql.egg-info/top_level.txt
```

