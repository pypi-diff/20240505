# Comparing `tmp/congress_transaction_scraper-0.0.5.tar.gz` & `tmp/congress_transaction_scraper-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "congress_transaction_scraper-0.0.5.tar", last modified: Sun May  5 20:02:59 2024, max compression
+gzip compressed data, was "congress_transaction_scraper-0.0.6.tar", last modified: Sun May  5 20:07:28 2024, max compression
```

## Comparing `congress_transaction_scraper-0.0.5.tar` & `congress_transaction_scraper-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 mkm        (501) staff       (20)        0 2024-05-05 20:02:59.013706 congress_transaction_scraper-0.0.5/
--rw-r--r--   0 mkm        (501) staff       (20)    35149 2023-12-29 17:09:27.000000 congress_transaction_scraper-0.0.5/LICENSE
--rw-r--r--   0 mkm        (501) staff       (20)      817 2024-05-05 20:02:59.013416 congress_transaction_scraper-0.0.5/PKG-INFO
--rw-r--r--   0 mkm        (501) staff       (20)       94 2023-05-07 21:02:14.000000 congress_transaction_scraper-0.0.5/README.md
--rw-r--r--   0 mkm        (501) staff       (20)      680 2024-05-05 20:02:47.000000 congress_transaction_scraper-0.0.5/pyproject.toml
--rw-r--r--   0 mkm        (501) staff       (20)       38 2024-05-05 20:02:59.013759 congress_transaction_scraper-0.0.5/setup.cfg
-drwxr-xr-x   0 mkm        (501) staff       (20)        0 2024-05-05 20:02:59.010367 congress_transaction_scraper-0.0.5/src/
--rw-r--r--   0 mkm        (501) staff       (20)        0 2023-12-29 17:09:27.000000 congress_transaction_scraper-0.0.5/src/__init__.py
-drwxr-xr-x   0 mkm        (501) staff       (20)        0 2024-05-05 20:02:59.012988 congress_transaction_scraper-0.0.5/src/congress_transaction_scraper.egg-info/
--rw-r--r--   0 mkm        (501) staff       (20)      817 2024-05-05 20:02:59.000000 congress_transaction_scraper-0.0.5/src/congress_transaction_scraper.egg-info/PKG-INFO
--rw-r--r--   0 mkm        (501) staff       (20)      457 2024-05-05 20:02:59.000000 congress_transaction_scraper-0.0.5/src/congress_transaction_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 mkm        (501) staff       (20)        1 2024-05-05 20:02:59.000000 congress_transaction_scraper-0.0.5/src/congress_transaction_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 mkm        (501) staff       (20)       44 2024-05-05 20:02:59.000000 congress_transaction_scraper-0.0.5/src/congress_transaction_scraper.egg-info/requires.txt
--rw-r--r--   0 mkm        (501) staff       (20)       24 2024-05-05 20:02:59.000000 congress_transaction_scraper-0.0.5/src/congress_transaction_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 mkm        (501) staff       (20)        0 2024-05-05 20:02:59.011547 congress_transaction_scraper-0.0.5/src/scrapers/
--rw-r--r--   0 mkm        (501) staff       (20)        0 2023-12-29 17:24:19.000000 congress_transaction_scraper-0.0.5/src/scrapers/__init__.py
--rw-r--r--   0 mkm        (501) staff       (20)      187 2024-05-05 20:02:37.000000 congress_transaction_scraper-0.0.5/src/scrapers/base.py
--rw-r--r--   0 mkm        (501) staff       (20)     4446 2024-01-07 20:10:14.000000 congress_transaction_scraper-0.0.5/src/scrapers/senate.py
-drwxr-xr-x   0 mkm        (501) staff       (20)        0 2024-05-05 20:02:59.012590 congress_transaction_scraper-0.0.5/src/utils/
--rw-r--r--   0 mkm        (501) staff       (20)      105 2024-01-07 20:12:24.000000 congress_transaction_scraper-0.0.5/src/utils/__init__.py
--rw-r--r--   0 mkm        (501) staff       (20)     1116 2023-12-29 17:28:13.000000 congress_transaction_scraper-0.0.5/src/utils/data.py
--rw-r--r--   0 mkm        (501) staff       (20)     1127 2023-12-29 17:33:08.000000 congress_transaction_scraper-0.0.5/src/utils/session.py
+drwxr-xr-x   0 mkm        (501) staff       (20)        0 2024-05-05 20:07:28.169854 congress_transaction_scraper-0.0.6/
+-rw-r--r--   0 mkm        (501) staff       (20)    35149 2023-12-29 17:09:27.000000 congress_transaction_scraper-0.0.6/LICENSE
+-rw-r--r--   0 mkm        (501) staff       (20)      817 2024-05-05 20:07:28.169654 congress_transaction_scraper-0.0.6/PKG-INFO
+-rw-r--r--   0 mkm        (501) staff       (20)       94 2023-05-07 21:02:14.000000 congress_transaction_scraper-0.0.6/README.md
+-rw-r--r--   0 mkm        (501) staff       (20)      680 2024-05-05 20:07:14.000000 congress_transaction_scraper-0.0.6/pyproject.toml
+-rw-r--r--   0 mkm        (501) staff       (20)       38 2024-05-05 20:07:28.169896 congress_transaction_scraper-0.0.6/setup.cfg
+drwxr-xr-x   0 mkm        (501) staff       (20)        0 2024-05-05 20:07:28.167163 congress_transaction_scraper-0.0.6/src/
+-rw-r--r--   0 mkm        (501) staff       (20)        0 2023-12-29 17:09:27.000000 congress_transaction_scraper-0.0.6/src/__init__.py
+drwxr-xr-x   0 mkm        (501) staff       (20)        0 2024-05-05 20:07:28.169408 congress_transaction_scraper-0.0.6/src/congress_transaction_scraper.egg-info/
+-rw-r--r--   0 mkm        (501) staff       (20)      817 2024-05-05 20:07:28.000000 congress_transaction_scraper-0.0.6/src/congress_transaction_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 mkm        (501) staff       (20)      457 2024-05-05 20:07:28.000000 congress_transaction_scraper-0.0.6/src/congress_transaction_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 mkm        (501) staff       (20)        1 2024-05-05 20:07:28.000000 congress_transaction_scraper-0.0.6/src/congress_transaction_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 mkm        (501) staff       (20)       44 2024-05-05 20:07:28.000000 congress_transaction_scraper-0.0.6/src/congress_transaction_scraper.egg-info/requires.txt
+-rw-r--r--   0 mkm        (501) staff       (20)       24 2024-05-05 20:07:28.000000 congress_transaction_scraper-0.0.6/src/congress_transaction_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 mkm        (501) staff       (20)        0 2024-05-05 20:07:28.168443 congress_transaction_scraper-0.0.6/src/scrapers/
+-rw-r--r--   0 mkm        (501) staff       (20)        0 2023-12-29 17:24:19.000000 congress_transaction_scraper-0.0.6/src/scrapers/__init__.py
+-rw-r--r--   0 mkm        (501) staff       (20)      187 2024-05-05 20:02:37.000000 congress_transaction_scraper-0.0.6/src/scrapers/base.py
+-rw-r--r--   0 mkm        (501) staff       (20)     4474 2024-05-05 20:07:05.000000 congress_transaction_scraper-0.0.6/src/scrapers/senate.py
+drwxr-xr-x   0 mkm        (501) staff       (20)        0 2024-05-05 20:07:28.169058 congress_transaction_scraper-0.0.6/src/utils/
+-rw-r--r--   0 mkm        (501) staff       (20)      105 2024-01-07 20:12:24.000000 congress_transaction_scraper-0.0.6/src/utils/__init__.py
+-rw-r--r--   0 mkm        (501) staff       (20)     1116 2023-12-29 17:28:13.000000 congress_transaction_scraper-0.0.6/src/utils/data.py
+-rw-r--r--   0 mkm        (501) staff       (20)     1127 2023-12-29 17:33:08.000000 congress_transaction_scraper-0.0.6/src/utils/session.py
```

### Comparing `congress_transaction_scraper-0.0.5/LICENSE` & `congress_transaction_scraper-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `congress_transaction_scraper-0.0.5/PKG-INFO` & `congress_transaction_scraper-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: congress-transaction-scraper
-Version: 0.0.5
+Version: 0.0.6
 Summary: Congressional transaction scraper
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/antidipyramid/congressional-transaction-scraper
 Project-URL: Issues, https://github.com/antidipyramid/congressional-transaction-scraper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `congress_transaction_scraper-0.0.5/pyproject.toml` & `congress_transaction_scraper-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "congress-transaction-scraper"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "Congressional transaction scraper"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [
```

### Comparing `congress_transaction_scraper-0.0.5/src/congress_transaction_scraper.egg-info/PKG-INFO` & `congress_transaction_scraper-0.0.6/src/congress_transaction_scraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: congress-transaction-scraper
-Version: 0.0.5
+Version: 0.0.6
 Summary: Congressional transaction scraper
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/antidipyramid/congressional-transaction-scraper
 Project-URL: Issues, https://github.com/antidipyramid/congressional-transaction-scraper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `congress_transaction_scraper-0.0.5/src/scrapers/senate.py` & `congress_transaction_scraper-0.0.6/src/scrapers/senate.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import time
 from bs4 import BeautifulSoup
 from collections.abc import Generator
 from urllib.parse import urlparse
 from io import StringIO
 
 from .base import TransactionScraper
-from ..utils import CSRFSession, ScrapedDisclosure, ScrapedTransaction
+from utils.session import CSRFSession
+from utils.data import ScrapedDisclosure, ScrapedTransaction
 
 
 class SenateTransactionScraper(TransactionScraper, CSRFSession):
     BASE_URL = "https://efdsearch.senate.gov/"
     LANDING_PATH = "/search/home/"
     HOME_PATH = "/search/"
     SEARCH_PATH = "/search/report/data/"
```

### Comparing `congress_transaction_scraper-0.0.5/src/utils/data.py` & `congress_transaction_scraper-0.0.6/src/utils/data.py`

 * *Files identical despite different names*

### Comparing `congress_transaction_scraper-0.0.5/src/utils/session.py` & `congress_transaction_scraper-0.0.6/src/utils/session.py`

 * *Files identical despite different names*

