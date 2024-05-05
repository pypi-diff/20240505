# Comparing `tmp/miner_ai_beta-0.1.1.tar.gz` & `tmp/miner_ai_beta-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miner_ai_beta-0.1.1.tar", max compression
+gzip compressed data, was "miner_ai_beta-0.1.2.tar", max compression
```

## Comparing `miner_ai_beta-0.1.1.tar` & `miner_ai_beta-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11357 2024-05-04 16:49:23.857900 miner_ai_beta-0.1.1/LICENSE
--rw-r--r--   0        0        0      242 2024-05-04 16:03:49.421708 miner_ai_beta-0.1.1/miner_ai_beta/loader/__init__.py
--rw-r--r--   0        0        0      473 2024-05-04 16:04:57.185499 miner_ai_beta-0.1.1/miner_ai_beta/loader/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     3042 2024-05-04 15:17:18.873214 miner_ai_beta-0.1.1/miner_ai_beta/loader/__pycache__/docs.cpython-311.pyc
--rw-r--r--   0        0        0     2372 2024-05-04 16:04:57.189700 miner_ai_beta-0.1.1/miner_ai_beta/loader/__pycache__/docs.cpython-312.pyc
--rw-r--r--   0        0        0     2299 2024-05-04 16:04:58.283790 miner_ai_beta-0.1.1/miner_ai_beta/loader/__pycache__/excels.cpython-312.pyc
--rw-r--r--   0        0        0     3252 2024-05-04 15:17:18.945722 miner_ai_beta-0.1.1/miner_ai_beta/loader/__pycache__/pages.cpython-311.pyc
--rw-r--r--   0        0        0     2566 2024-05-04 15:17:18.984762 miner_ai_beta-0.1.1/miner_ai_beta/loader/__pycache__/pages.cpython-312.pyc
--rw-r--r--   0        0        0     3161 2024-05-04 15:17:19.027542 miner_ai_beta-0.1.1/miner_ai_beta/loader/__pycache__/pdfs.cpython-311.pyc
--rw-r--r--   0        0        0     2309 2024-05-04 16:05:00.319553 miner_ai_beta-0.1.1/miner_ai_beta/loader/__pycache__/pdfs.cpython-312.pyc
--rw-r--r--   0        0        0     2165 2024-05-04 16:05:00.402279 miner_ai_beta-0.1.1/miner_ai_beta/loader/__pycache__/ppts.cpython-312.pyc
--rw-r--r--   0        0        0     2343 2024-05-04 16:05:00.331906 miner_ai_beta-0.1.1/miner_ai_beta/loader/__pycache__/tubes.cpython-312.pyc
--rw-r--r--   0        0        0      711 2024-05-04 16:05:00.626643 miner_ai_beta-0.1.1/miner_ai_beta/loader/__pycache__/union.cpython-312.pyc
--rw-r--r--   0        0        0     2455 2024-05-04 16:05:00.139759 miner_ai_beta-0.1.1/miner_ai_beta/loader/__pycache__/web_pages.cpython-312.pyc
--rw-r--r--   0        0        0     2928 2024-05-04 15:17:19.188416 miner_ai_beta-0.1.1/miner_ai_beta/loader/__pycache__/xlss.cpython-311.pyc
--rw-r--r--   0        0        0     2490 2024-05-04 15:17:19.226637 miner_ai_beta-0.1.1/miner_ai_beta/loader/__pycache__/xlss.cpython-312.pyc
--rw-r--r--   0        0        0     1737 2024-05-04 16:30:59.578915 miner_ai_beta-0.1.1/miner_ai_beta/loader/docs.py
--rw-r--r--   0        0        0     1731 2024-05-04 16:03:01.249647 miner_ai_beta-0.1.1/miner_ai_beta/loader/excels.py
--rw-r--r--   0        0        0     1697 2024-05-04 16:03:04.629094 miner_ai_beta-0.1.1/miner_ai_beta/loader/pdfs.py
--rw-r--r--   0        0        0     1782 2024-05-04 16:30:53.122384 miner_ai_beta-0.1.1/miner_ai_beta/loader/ppts.py
--rw-r--r--   0        0        0     1792 2024-05-04 16:03:14.578345 miner_ai_beta-0.1.1/miner_ai_beta/loader/tubes.py
--rw-r--r--   0        0        0      361 2024-05-04 15:52:12.917924 miner_ai_beta-0.1.1/miner_ai_beta/loader/union.py
--rw-r--r--   0        0        0     1857 2024-05-04 16:30:42.678525 miner_ai_beta-0.1.1/miner_ai_beta/loader/web_pages.py
--rw-r--r--   0        0        0      532 2024-05-04 16:51:27.948588 miner_ai_beta-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2731 2024-05-04 16:48:48.051972 miner_ai_beta-0.1.1/README.md
--rw-r--r--   0        0        0     3398 1970-01-01 00:00:00.000000 miner_ai_beta-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-04 16:49:23.857900 miner_ai_beta-0.1.2/LICENSE
+-rw-r--r--   0        0        0      242 2024-05-04 16:59:21.199649 miner_ai_beta-0.1.2/miner_ai_beta/loader/__init__.py
+-rw-r--r--   0        0        0      473 2024-05-04 16:04:57.185499 miner_ai_beta-0.1.2/miner_ai_beta/loader/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     3042 2024-05-04 15:17:18.873214 miner_ai_beta-0.1.2/miner_ai_beta/loader/__pycache__/docs.cpython-311.pyc
+-rw-r--r--   0        0        0     2372 2024-05-04 16:04:57.189700 miner_ai_beta-0.1.2/miner_ai_beta/loader/__pycache__/docs.cpython-312.pyc
+-rw-r--r--   0        0        0     2299 2024-05-04 16:04:58.283790 miner_ai_beta-0.1.2/miner_ai_beta/loader/__pycache__/excels.cpython-312.pyc
+-rw-r--r--   0        0        0     3252 2024-05-04 15:17:18.945722 miner_ai_beta-0.1.2/miner_ai_beta/loader/__pycache__/pages.cpython-311.pyc
+-rw-r--r--   0        0        0     2566 2024-05-04 15:17:18.984762 miner_ai_beta-0.1.2/miner_ai_beta/loader/__pycache__/pages.cpython-312.pyc
+-rw-r--r--   0        0        0     3161 2024-05-04 15:17:19.027542 miner_ai_beta-0.1.2/miner_ai_beta/loader/__pycache__/pdfs.cpython-311.pyc
+-rw-r--r--   0        0        0     2309 2024-05-04 16:05:00.319553 miner_ai_beta-0.1.2/miner_ai_beta/loader/__pycache__/pdfs.cpython-312.pyc
+-rw-r--r--   0        0        0     2165 2024-05-04 16:05:00.402279 miner_ai_beta-0.1.2/miner_ai_beta/loader/__pycache__/ppts.cpython-312.pyc
+-rw-r--r--   0        0        0     2343 2024-05-04 16:05:00.331906 miner_ai_beta-0.1.2/miner_ai_beta/loader/__pycache__/tubes.cpython-312.pyc
+-rw-r--r--   0        0        0      711 2024-05-04 16:05:00.626643 miner_ai_beta-0.1.2/miner_ai_beta/loader/__pycache__/union.cpython-312.pyc
+-rw-r--r--   0        0        0     2455 2024-05-04 16:05:00.139759 miner_ai_beta-0.1.2/miner_ai_beta/loader/__pycache__/web_pages.cpython-312.pyc
+-rw-r--r--   0        0        0     2928 2024-05-04 15:17:19.188416 miner_ai_beta-0.1.2/miner_ai_beta/loader/__pycache__/xlss.cpython-311.pyc
+-rw-r--r--   0        0        0     2490 2024-05-04 15:17:19.226637 miner_ai_beta-0.1.2/miner_ai_beta/loader/__pycache__/xlss.cpython-312.pyc
+-rw-r--r--   0        0        0     1737 2024-05-04 16:30:59.578915 miner_ai_beta-0.1.2/miner_ai_beta/loader/docs.py
+-rw-r--r--   0        0        0     1731 2024-05-04 16:03:01.249647 miner_ai_beta-0.1.2/miner_ai_beta/loader/excels.py
+-rw-r--r--   0        0        0     1697 2024-05-04 16:03:04.629094 miner_ai_beta-0.1.2/miner_ai_beta/loader/pdfs.py
+-rw-r--r--   0        0        0     1782 2024-05-04 16:30:53.122384 miner_ai_beta-0.1.2/miner_ai_beta/loader/ppts.py
+-rw-r--r--   0        0        0     1792 2024-05-04 16:03:14.578345 miner_ai_beta-0.1.2/miner_ai_beta/loader/tubes.py
+-rw-r--r--   0        0        0      361 2024-05-04 15:52:12.917924 miner_ai_beta-0.1.2/miner_ai_beta/loader/union.py
+-rw-r--r--   0        0        0     1857 2024-05-04 16:30:42.678525 miner_ai_beta-0.1.2/miner_ai_beta/loader/web_pages.py
+-rw-r--r--   0        0        0      532 2024-05-04 16:59:37.530984 miner_ai_beta-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2731 2024-05-04 16:48:48.051972 miner_ai_beta-0.1.2/README.md
+-rw-r--r--   0        0        0     3398 1970-01-01 00:00:00.000000 miner_ai_beta-0.1.2/PKG-INFO
```

### Comparing `miner_ai_beta-0.1.1/LICENSE` & `miner_ai_beta-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.1/miner_ai_beta/loader/__pycache__/docs.cpython-311.pyc` & `miner_ai_beta-0.1.2/miner_ai_beta/loader/__pycache__/docs.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.1/miner_ai_beta/loader/__pycache__/docs.cpython-312.pyc` & `miner_ai_beta-0.1.2/miner_ai_beta/loader/__pycache__/docs.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.1/miner_ai_beta/loader/__pycache__/excels.cpython-312.pyc` & `miner_ai_beta-0.1.2/miner_ai_beta/loader/__pycache__/excels.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.1/miner_ai_beta/loader/__pycache__/pages.cpython-311.pyc` & `miner_ai_beta-0.1.2/miner_ai_beta/loader/__pycache__/pages.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.1/miner_ai_beta/loader/__pycache__/pages.cpython-312.pyc` & `miner_ai_beta-0.1.2/miner_ai_beta/loader/__pycache__/pages.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.1/miner_ai_beta/loader/__pycache__/pdfs.cpython-311.pyc` & `miner_ai_beta-0.1.2/miner_ai_beta/loader/__pycache__/pdfs.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.1/miner_ai_beta/loader/__pycache__/pdfs.cpython-312.pyc` & `miner_ai_beta-0.1.2/miner_ai_beta/loader/__pycache__/pdfs.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.1/miner_ai_beta/loader/__pycache__/ppts.cpython-312.pyc` & `miner_ai_beta-0.1.2/miner_ai_beta/loader/__pycache__/ppts.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.1/miner_ai_beta/loader/__pycache__/tubes.cpython-312.pyc` & `miner_ai_beta-0.1.2/miner_ai_beta/loader/__pycache__/tubes.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.1/miner_ai_beta/loader/__pycache__/union.cpython-312.pyc` & `miner_ai_beta-0.1.2/miner_ai_beta/loader/__pycache__/union.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.1/miner_ai_beta/loader/__pycache__/web_pages.cpython-312.pyc` & `miner_ai_beta-0.1.2/miner_ai_beta/loader/__pycache__/web_pages.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.1/miner_ai_beta/loader/__pycache__/xlss.cpython-311.pyc` & `miner_ai_beta-0.1.2/miner_ai_beta/loader/__pycache__/xlss.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.1/miner_ai_beta/loader/__pycache__/xlss.cpython-312.pyc` & `miner_ai_beta-0.1.2/miner_ai_beta/loader/__pycache__/xlss.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.1/miner_ai_beta/loader/docs.py` & `miner_ai_beta-0.1.2/miner_ai_beta/loader/docs.py`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.1/miner_ai_beta/loader/excels.py` & `miner_ai_beta-0.1.2/miner_ai_beta/loader/excels.py`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.1/miner_ai_beta/loader/pdfs.py` & `miner_ai_beta-0.1.2/miner_ai_beta/loader/pdfs.py`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.1/miner_ai_beta/loader/ppts.py` & `miner_ai_beta-0.1.2/miner_ai_beta/loader/ppts.py`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.1/miner_ai_beta/loader/tubes.py` & `miner_ai_beta-0.1.2/miner_ai_beta/loader/tubes.py`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.1/miner_ai_beta/loader/web_pages.py` & `miner_ai_beta-0.1.2/miner_ai_beta/loader/web_pages.py`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.1/pyproject.toml` & `miner_ai_beta-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "miner-ai-beta"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Valerio Domenici <valeriodomenici93@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 tqdm = "^4.66.4"
```

### Comparing `miner_ai_beta-0.1.1/README.md` & `miner_ai_beta-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.1/PKG-INFO` & `miner_ai_beta-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miner-ai-beta
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Valerio Domenici
 Author-email: valeriodomenici93@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: bs4 (>=0.0.2,<0.0.3)
```

