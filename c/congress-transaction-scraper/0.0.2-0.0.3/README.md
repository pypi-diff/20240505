# Comparing `tmp/congress_transaction_scraper-0.0.2.tar.gz` & `tmp/congress_transaction_scraper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "congress_transaction_scraper-0.0.2.tar", last modified: Sun May  5 19:49:36 2024, max compression
+gzip compressed data, was "congress_transaction_scraper-0.0.3.tar", last modified: Sun May  5 19:59:01 2024, max compression
```

## Comparing `congress_transaction_scraper-0.0.2.tar` & `congress_transaction_scraper-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 mkm        (501) staff       (20)        0 2024-05-05 19:49:36.686994 congress_transaction_scraper-0.0.2/
--rw-r--r--   0 mkm        (501) staff       (20)    35149 2023-12-29 17:09:27.000000 congress_transaction_scraper-0.0.2/LICENSE
--rw-r--r--   0 mkm        (501) staff       (20)      817 2024-05-05 19:49:36.686787 congress_transaction_scraper-0.0.2/PKG-INFO
--rw-r--r--   0 mkm        (501) staff       (20)       94 2023-05-07 21:02:14.000000 congress_transaction_scraper-0.0.2/README.md
--rw-r--r--   0 mkm        (501) staff       (20)      680 2024-05-05 19:48:27.000000 congress_transaction_scraper-0.0.2/pyproject.toml
--rw-r--r--   0 mkm        (501) staff       (20)       38 2024-05-05 19:49:36.687045 congress_transaction_scraper-0.0.2/setup.cfg
-drwxr-xr-x   0 mkm        (501) staff       (20)        0 2024-05-05 19:49:36.683644 congress_transaction_scraper-0.0.2/src/
--rw-r--r--   0 mkm        (501) staff       (20)        0 2023-12-29 17:09:27.000000 congress_transaction_scraper-0.0.2/src/__init__.py
-drwxr-xr-x   0 mkm        (501) staff       (20)        0 2024-05-05 19:49:36.686502 congress_transaction_scraper-0.0.2/src/congress_transaction_scraper.egg-info/
--rw-r--r--   0 mkm        (501) staff       (20)      817 2024-05-05 19:49:36.000000 congress_transaction_scraper-0.0.2/src/congress_transaction_scraper.egg-info/PKG-INFO
--rw-r--r--   0 mkm        (501) staff       (20)      457 2024-05-05 19:49:36.000000 congress_transaction_scraper-0.0.2/src/congress_transaction_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 mkm        (501) staff       (20)        1 2024-05-05 19:49:36.000000 congress_transaction_scraper-0.0.2/src/congress_transaction_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 mkm        (501) staff       (20)       44 2024-05-05 19:49:36.000000 congress_transaction_scraper-0.0.2/src/congress_transaction_scraper.egg-info/requires.txt
--rw-r--r--   0 mkm        (501) staff       (20)       24 2024-05-05 19:49:36.000000 congress_transaction_scraper-0.0.2/src/congress_transaction_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 mkm        (501) staff       (20)        0 2024-05-05 19:49:36.685124 congress_transaction_scraper-0.0.2/src/scrapers/
--rw-r--r--   0 mkm        (501) staff       (20)        0 2023-12-29 17:24:19.000000 congress_transaction_scraper-0.0.2/src/scrapers/__init__.py
--rw-r--r--   0 mkm        (501) staff       (20)      184 2024-01-07 20:11:00.000000 congress_transaction_scraper-0.0.2/src/scrapers/base.py
--rw-r--r--   0 mkm        (501) staff       (20)     4446 2024-01-07 20:10:14.000000 congress_transaction_scraper-0.0.2/src/scrapers/senate.py
-drwxr-xr-x   0 mkm        (501) staff       (20)        0 2024-05-05 19:49:36.686066 congress_transaction_scraper-0.0.2/src/utils/
--rw-r--r--   0 mkm        (501) staff       (20)      105 2024-01-07 20:12:24.000000 congress_transaction_scraper-0.0.2/src/utils/__init__.py
--rw-r--r--   0 mkm        (501) staff       (20)     1116 2023-12-29 17:28:13.000000 congress_transaction_scraper-0.0.2/src/utils/data.py
--rw-r--r--   0 mkm        (501) staff       (20)     1127 2023-12-29 17:33:08.000000 congress_transaction_scraper-0.0.2/src/utils/session.py
+drwxr-xr-x   0 mkm        (501) staff       (20)        0 2024-05-05 19:59:01.299647 congress_transaction_scraper-0.0.3/
+-rw-r--r--   0 mkm        (501) staff       (20)    35149 2023-12-29 17:09:27.000000 congress_transaction_scraper-0.0.3/LICENSE
+-rw-r--r--   0 mkm        (501) staff       (20)      817 2024-05-05 19:59:01.299420 congress_transaction_scraper-0.0.3/PKG-INFO
+-rw-r--r--   0 mkm        (501) staff       (20)       94 2023-05-07 21:02:14.000000 congress_transaction_scraper-0.0.3/README.md
+-rw-r--r--   0 mkm        (501) staff       (20)      680 2024-05-05 19:58:43.000000 congress_transaction_scraper-0.0.3/pyproject.toml
+-rw-r--r--   0 mkm        (501) staff       (20)       38 2024-05-05 19:59:01.299694 congress_transaction_scraper-0.0.3/setup.cfg
+drwxr-xr-x   0 mkm        (501) staff       (20)        0 2024-05-05 19:59:01.284914 congress_transaction_scraper-0.0.3/src/
+-rw-r--r--   0 mkm        (501) staff       (20)        0 2023-12-29 17:09:27.000000 congress_transaction_scraper-0.0.3/src/__init__.py
+drwxr-xr-x   0 mkm        (501) staff       (20)        0 2024-05-05 19:59:01.299169 congress_transaction_scraper-0.0.3/src/congress_transaction_scraper.egg-info/
+-rw-r--r--   0 mkm        (501) staff       (20)      817 2024-05-05 19:59:01.000000 congress_transaction_scraper-0.0.3/src/congress_transaction_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 mkm        (501) staff       (20)      457 2024-05-05 19:59:01.000000 congress_transaction_scraper-0.0.3/src/congress_transaction_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 mkm        (501) staff       (20)        1 2024-05-05 19:59:01.000000 congress_transaction_scraper-0.0.3/src/congress_transaction_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 mkm        (501) staff       (20)       44 2024-05-05 19:59:01.000000 congress_transaction_scraper-0.0.3/src/congress_transaction_scraper.egg-info/requires.txt
+-rw-r--r--   0 mkm        (501) staff       (20)       24 2024-05-05 19:59:01.000000 congress_transaction_scraper-0.0.3/src/congress_transaction_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 mkm        (501) staff       (20)        0 2024-05-05 19:59:01.290134 congress_transaction_scraper-0.0.3/src/scrapers/
+-rw-r--r--   0 mkm        (501) staff       (20)        0 2023-12-29 17:24:19.000000 congress_transaction_scraper-0.0.3/src/scrapers/__init__.py
+-rw-r--r--   0 mkm        (501) staff       (20)      187 2024-05-05 19:58:28.000000 congress_transaction_scraper-0.0.3/src/scrapers/base.py
+-rw-r--r--   0 mkm        (501) staff       (20)     4446 2024-01-07 20:10:14.000000 congress_transaction_scraper-0.0.3/src/scrapers/senate.py
+drwxr-xr-x   0 mkm        (501) staff       (20)        0 2024-05-05 19:59:01.297243 congress_transaction_scraper-0.0.3/src/utils/
+-rw-r--r--   0 mkm        (501) staff       (20)      105 2024-01-07 20:12:24.000000 congress_transaction_scraper-0.0.3/src/utils/__init__.py
+-rw-r--r--   0 mkm        (501) staff       (20)     1116 2023-12-29 17:28:13.000000 congress_transaction_scraper-0.0.3/src/utils/data.py
+-rw-r--r--   0 mkm        (501) staff       (20)     1127 2023-12-29 17:33:08.000000 congress_transaction_scraper-0.0.3/src/utils/session.py
```

### Comparing `congress_transaction_scraper-0.0.2/LICENSE` & `congress_transaction_scraper-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `congress_transaction_scraper-0.0.2/PKG-INFO` & `congress_transaction_scraper-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: congress-transaction-scraper
-Version: 0.0.2
+Version: 0.0.3
 Summary: Congressional transaction scraper
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/antidipyramid/congressional-transaction-scraper
 Project-URL: Issues, https://github.com/antidipyramid/congressional-transaction-scraper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `congress_transaction_scraper-0.0.2/pyproject.toml` & `congress_transaction_scraper-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "congress-transaction-scraper"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "Congressional transaction scraper"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [
```

### Comparing `congress_transaction_scraper-0.0.2/src/congress_transaction_scraper.egg-info/PKG-INFO` & `congress_transaction_scraper-0.0.3/src/congress_transaction_scraper.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: congress-transaction-scraper
-Version: 0.0.2
+Version: 0.0.3
 Summary: Congressional transaction scraper
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/antidipyramid/congressional-transaction-scraper
 Project-URL: Issues, https://github.com/antidipyramid/congressional-transaction-scraper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `congress_transaction_scraper-0.0.2/src/scrapers/senate.py` & `congress_transaction_scraper-0.0.3/src/scrapers/senate.py`

 * *Files identical despite different names*

### Comparing `congress_transaction_scraper-0.0.2/src/utils/data.py` & `congress_transaction_scraper-0.0.3/src/utils/data.py`

 * *Files identical despite different names*

### Comparing `congress_transaction_scraper-0.0.2/src/utils/session.py` & `congress_transaction_scraper-0.0.3/src/utils/session.py`

 * *Files identical despite different names*

