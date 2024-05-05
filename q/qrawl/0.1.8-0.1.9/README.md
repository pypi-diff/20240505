# Comparing `tmp/qrawl-0.1.8.tar.gz` & `tmp/qrawl-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qrawl-0.1.8.tar", max compression
+gzip compressed data, was "qrawl-0.1.9.tar", max compression
```

## Comparing `qrawl-0.1.8.tar` & `qrawl-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11558 2024-04-10 20:13:30.588327 qrawl-0.1.8/LICENSE
--rw-r--r--   0        0        0      794 2024-05-01 07:17:30.215877 qrawl-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       23 2024-04-09 08:01:21.111154 qrawl-0.1.8/qrawl/__init__.py
--rw-r--r--   0        0        0     1267 2024-04-09 07:59:51.136473 qrawl-0.1.8/qrawl/common.py
--rw-r--r--   0        0        0      322 2024-05-01 06:43:35.164934 qrawl-0.1.8/qrawl/exceptions.py
--rw-r--r--   0        0        0       28 2024-04-05 07:23:15.121016 qrawl-0.1.8/qrawl/google_sheets/__init__.py
--rw-r--r--   0        0        0     2224 2024-04-10 20:17:48.321751 qrawl-0.1.8/qrawl/google_sheets/column.py
--rw-r--r--   0        0        0       56 2024-04-09 23:05:42.684682 qrawl-0.1.8/qrawl/playwright/async_api/__init__.py
--rw-r--r--   0        0        0     4002 2024-04-10 20:18:37.778395 qrawl-0.1.8/qrawl/playwright/async_api/async_playwright.py
--rw-r--r--   0        0        0      663 2024-04-05 06:47:08.312708 qrawl-0.1.8/qrawl/playwright/async_api/common.py
--rw-r--r--   0        0        0       55 2024-04-09 23:05:16.406743 qrawl-0.1.8/qrawl/playwright/sync_api/__init__.py
--rw-r--r--   0        0        0      587 2024-04-09 23:01:33.394056 qrawl-0.1.8/qrawl/playwright/sync_api/common.py
--rw-r--r--   0        0        0     3933 2024-04-11 06:02:26.308965 qrawl-0.1.8/qrawl/playwright/sync_api/sync_playwright.py
--rw-r--r--   0        0        0        0 2024-04-03 00:46:13.447864 qrawl-0.1.8/qrawl/scrapy/__init__.py
--rw-r--r--   0        0        0       33 2024-04-10 20:18:05.787009 qrawl-0.1.8/qrawl/selenium/__init__.py
--rw-r--r--   0        0        0     6558 2024-05-01 07:17:11.664631 qrawl-0.1.8/qrawl/selenium/browsermob_proxy_wrapper.py
--rw-r--r--   0        0        0     1667 2024-05-01 06:44:39.479457 qrawl-0.1.8/qrawl/selenium/exceptions.py
--rw-r--r--   0        0        0    15799 2024-05-01 06:29:28.782685 qrawl-0.1.8/qrawl/selenium/selenium.py
--rw-r--r--   0        0        0     1321 2024-04-05 07:18:07.077122 qrawl-0.1.8/qrawl/xpath.py
--rw-r--r--   0        0        0       37 2024-04-10 20:13:30.588327 qrawl-0.1.8/README.md
--rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 qrawl-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11558 2024-04-10 20:13:30.588327 qrawl-0.1.9/LICENSE
+-rw-r--r--   0        0        0      794 2024-05-01 07:29:17.131925 qrawl-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       23 2024-04-09 08:01:21.111154 qrawl-0.1.9/qrawl/__init__.py
+-rw-r--r--   0        0        0     1267 2024-04-09 07:59:51.136473 qrawl-0.1.9/qrawl/common.py
+-rw-r--r--   0        0        0      322 2024-05-01 06:43:35.164934 qrawl-0.1.9/qrawl/exceptions.py
+-rw-r--r--   0        0        0       28 2024-04-05 07:23:15.121016 qrawl-0.1.9/qrawl/google_sheets/__init__.py
+-rw-r--r--   0        0        0     2224 2024-04-10 20:17:48.321751 qrawl-0.1.9/qrawl/google_sheets/column.py
+-rw-r--r--   0        0        0       56 2024-04-09 23:05:42.684682 qrawl-0.1.9/qrawl/playwright/async_api/__init__.py
+-rw-r--r--   0        0        0     4002 2024-04-10 20:18:37.778395 qrawl-0.1.9/qrawl/playwright/async_api/async_playwright.py
+-rw-r--r--   0        0        0      663 2024-04-05 06:47:08.312708 qrawl-0.1.9/qrawl/playwright/async_api/common.py
+-rw-r--r--   0        0        0       55 2024-04-09 23:05:16.406743 qrawl-0.1.9/qrawl/playwright/sync_api/__init__.py
+-rw-r--r--   0        0        0      587 2024-04-09 23:01:33.394056 qrawl-0.1.9/qrawl/playwright/sync_api/common.py
+-rw-r--r--   0        0        0     3933 2024-04-11 06:02:26.308965 qrawl-0.1.9/qrawl/playwright/sync_api/sync_playwright.py
+-rw-r--r--   0        0        0        0 2024-04-03 00:46:13.447864 qrawl-0.1.9/qrawl/scrapy/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-10 20:18:05.787009 qrawl-0.1.9/qrawl/selenium/__init__.py
+-rw-r--r--   0        0        0     6692 2024-05-01 07:28:34.269298 qrawl-0.1.9/qrawl/selenium/browsermob_proxy_wrapper.py
+-rw-r--r--   0        0        0     1948 2024-05-01 07:26:17.833098 qrawl-0.1.9/qrawl/selenium/exceptions.py
+-rw-r--r--   0        0        0    15799 2024-05-01 06:29:28.782685 qrawl-0.1.9/qrawl/selenium/selenium.py
+-rw-r--r--   0        0        0     1321 2024-04-05 07:18:07.077122 qrawl-0.1.9/qrawl/xpath.py
+-rw-r--r--   0        0        0       37 2024-04-10 20:13:30.588327 qrawl-0.1.9/README.md
+-rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 qrawl-0.1.9/PKG-INFO
```

### Comparing `qrawl-0.1.8/LICENSE` & `qrawl-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.8/pyproject.toml` & `qrawl-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qrawl"
-version = "0.1.8"
+version = "0.1.9"
 description = "Python Crawling Utilities."
 authors = ["GGLionCross"]
 license = "Apache 2.0"
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
```

### Comparing `qrawl-0.1.8/qrawl/common.py` & `qrawl-0.1.9/qrawl/common.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.8/qrawl/google_sheets/column.py` & `qrawl-0.1.9/qrawl/google_sheets/column.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.8/qrawl/playwright/async_api/async_playwright.py` & `qrawl-0.1.9/qrawl/playwright/async_api/async_playwright.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.8/qrawl/playwright/async_api/common.py` & `qrawl-0.1.9/qrawl/playwright/async_api/common.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.8/qrawl/playwright/sync_api/common.py` & `qrawl-0.1.9/qrawl/playwright/sync_api/common.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.8/qrawl/playwright/sync_api/sync_playwright.py` & `qrawl-0.1.9/qrawl/playwright/sync_api/sync_playwright.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.8/qrawl/selenium/browsermob_proxy_wrapper.py` & `qrawl-0.1.9/qrawl/selenium/browsermob_proxy_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,22 +17,26 @@
 
 try:
     import psutil  # type: ignore
 except ModuleNotFoundError:
     psutil = None
 
 # Local Libraries
-from .exceptions import BrowsermobProxyNotInstalled, MissingBrowsermobProxyPath
+from .exceptions import BrowsermobProxyNotInstalled
+from .exceptions import MissingBrowsermobProxyPath
+from .exceptions import PsutilNotInstalled
 
 
 class BrowsermobProxyWrapper:
     def __init__(self, browsermob_proxy_path: str, port=9090, debug: bool = False):
         self._debug = debug
         if Server is None:
             raise BrowsermobProxyNotInstalled
+        if psutil is None:
+            raise PsutilNotInstalled
         if not browsermob_proxy_path:
             raise MissingBrowsermobProxyPath
 
         options = {"port": port}
 
         if self._debug:
             cprint(f"<y>DEBUG: BMP browsermob_proxy_path = {browsermob_proxy_path}")
```

### Comparing `qrawl-0.1.8/qrawl/selenium/exceptions.py` & `qrawl-0.1.9/qrawl/selenium/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,24 @@
         self,
         message="<y>'browsermob_proxy_path' is empty. Check your proxy configuration.",
     ):
         self.message = ctext(message)
         super().__init__(self.message)
 
 
+class PsutilNotInstalled(Exception):
+    # Raise this when undetected_chromedriver is not installed
+    def __init__(
+        self,
+        message="<y>Module 'psutil' not installed.",
+    ):
+        self.message = ctext(message)
+        super().__init__(self.message)
+
+
 class SeleniumWireAndUndetectedChromedriverIncompatible(Exception):
     # Raise this when undetected_chromedriver is not installed
     def __init__(
         self,
         message="<y>Selenium Wire and Undetected Chromedriver are incompatible. Please only set 'use_selenium_wire' OR 'use_undetected_chromedriver'.",
     ):
         self.message = ctext(message)
```

### Comparing `qrawl-0.1.8/qrawl/selenium/selenium.py` & `qrawl-0.1.9/qrawl/selenium/selenium.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.8/qrawl/xpath.py` & `qrawl-0.1.9/qrawl/xpath.py`

 * *Files identical despite different names*

