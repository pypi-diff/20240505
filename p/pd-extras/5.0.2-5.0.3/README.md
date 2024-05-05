# Comparing `tmp/pd_extras-5.0.2.tar.gz` & `tmp/pd_extras-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pd_extras-5.0.2.tar", max compression
+gzip compressed data, was "pd_extras-5.0.3.tar", max compression
```

## Comparing `pd_extras-5.0.2.tar` & `pd_extras-5.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1069 2024-05-05 13:00:18.946226 pd_extras-5.0.2/LICENSE
--rw-r--r--   0        0        0     2248 2024-05-05 13:00:18.946226 pd_extras-5.0.2/README.md
--rw-r--r--   0        0        0        0 2024-05-05 13:00:18.946226 pd_extras-5.0.2/pd_extras/__init__.py
--rw-r--r--   0        0        0        0 2024-05-05 13:00:18.946226 pd_extras-5.0.2/pd_extras/check/__init__.py
--rw-r--r--   0        0        0     3245 2024-05-05 13:00:18.946226 pd_extras-5.0.2/pd_extras/check/sanitize.py
--rw-r--r--   0        0        0        0 2024-05-05 13:00:18.946226 pd_extras-5.0.2/pd_extras/extra/__init__.py
--rw-r--r--   0        0        0     3794 2024-05-05 13:00:18.946226 pd_extras-5.0.2/pd_extras/extra/flattener.py
--rw-r--r--   0        0        0     2635 2024-05-05 13:00:18.946226 pd_extras-5.0.2/pd_extras/extra/operations.py
--rw-r--r--   0        0        0        0 2024-05-05 13:00:18.946226 pd_extras-5.0.2/pd_extras/optimize/__init__.py
--rw-r--r--   0        0        0     1775 2024-05-05 13:00:18.946226 pd_extras-5.0.2/pd_extras/optimize/df_ops.py
--rw-r--r--   0        0        0        0 2024-05-05 13:00:18.950226 pd_extras-5.0.2/pd_extras/write/__init__.py
--rw-r--r--   0        0        0     1388 2024-05-05 13:00:18.950226 pd_extras-5.0.2/pd_extras/write/common.py
--rw-r--r--   0        0        0     5682 2024-05-05 13:00:18.950226 pd_extras-5.0.2/pd_extras/write/nosql_writer.py
--rw-r--r--   0        0        0     8962 2024-05-05 13:00:18.950226 pd_extras-5.0.2/pd_extras/write/sql_writer.py
--rw-r--r--   0        0        0      724 2024-05-05 13:00:18.950226 pd_extras-5.0.2/pyproject.toml
--rw-r--r--   0        0        0     3262 1970-01-01 00:00:00.000000 pd_extras-5.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-05 15:20:25.108617 pd_extras-5.0.3/LICENSE
+-rw-r--r--   0        0        0     2270 2024-05-05 15:20:25.108617 pd_extras-5.0.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-05 15:20:25.108617 pd_extras-5.0.3/pd_extras/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:20:25.108617 pd_extras-5.0.3/pd_extras/check/__init__.py
+-rw-r--r--   0        0        0     3245 2024-05-05 15:20:25.108617 pd_extras-5.0.3/pd_extras/check/sanitize.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:20:25.108617 pd_extras-5.0.3/pd_extras/extra/__init__.py
+-rw-r--r--   0        0        0     3794 2024-05-05 15:20:25.108617 pd_extras-5.0.3/pd_extras/extra/flattener.py
+-rw-r--r--   0        0        0     2635 2024-05-05 15:20:25.108617 pd_extras-5.0.3/pd_extras/extra/operations.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:20:25.108617 pd_extras-5.0.3/pd_extras/optimize/__init__.py
+-rw-r--r--   0        0        0     1775 2024-05-05 15:20:25.108617 pd_extras-5.0.3/pd_extras/optimize/df_ops.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:20:25.108617 pd_extras-5.0.3/pd_extras/write/__init__.py
+-rw-r--r--   0        0        0     1388 2024-05-05 15:20:25.108617 pd_extras-5.0.3/pd_extras/write/common.py
+-rw-r--r--   0        0        0     5682 2024-05-05 15:20:25.108617 pd_extras-5.0.3/pd_extras/write/nosql_writer.py
+-rw-r--r--   0        0        0     8962 2024-05-05 15:20:25.108617 pd_extras-5.0.3/pd_extras/write/sql_writer.py
+-rw-r--r--   0        0        0      724 2024-05-05 15:20:25.108617 pd_extras-5.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3284 1970-01-01 00:00:00.000000 pd_extras-5.0.3/PKG-INFO
```

### Comparing `pd_extras-5.0.2/LICENSE` & `pd_extras-5.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pd_extras-5.0.2/README.md` & `pd_extras-5.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 [![codecov](https://codecov.io/gh/proafxin/pd-extras/graph/badge.svg?token=AQA0IJY4N1)](https://codecov.io/gh/proafxin/pd-extras)
 [![Documentation Status](https://readthedocs.org/projects/pd-extras/badge/?version=latest)](https://pd-extras.readthedocs.io/en/latest/?badge=latest)
 
 Some functions on top of pandas.
 
 ## Install Environment
 
-Run `python -m pip install -U pip` and `pip install -U pip poetry`. Then run `poetry install`. If you are facing issues installing `mysqlclient` or `psycopg2` on Ubuntu, it's because you are missing some libraries. Please check their pages. Usually for `psycopg2`, it's `libpq-dev` and for `mysqlclient`, it's `python3-dev default-libmysqlclient-dev build-essential`. Check the pages for more specific and accurate commands.
+For local development:
+
+- Run `python -m pip install -U pip` and `pip install -U pip poetry`
+- Run `poetry install`. If you are facing issues installing `mysqlclient` or `psycopg2` on Ubuntu, it's because you are missing some libraries. Please check their pages. Usually for `psycopg2`, it's `libpq-dev` and for `mysqlclient`, it's `python3-dev default-libmysqlclient-dev build-essential`. Check the pages for more specific and accurate commands.
 
 ## Testing
 
 Run `docker compose up` then `tox`. Obviously you need docker and tox installed.
 
 ## Generate Documentation Source Files
```

### Comparing `pd_extras-5.0.2/pd_extras/check/sanitize.py` & `pd_extras-5.0.3/pd_extras/check/sanitize.py`

 * *Files identical despite different names*

### Comparing `pd_extras-5.0.2/pd_extras/extra/flattener.py` & `pd_extras-5.0.3/pd_extras/extra/flattener.py`

 * *Files identical despite different names*

### Comparing `pd_extras-5.0.2/pd_extras/extra/operations.py` & `pd_extras-5.0.3/pd_extras/extra/operations.py`

 * *Files identical despite different names*

### Comparing `pd_extras-5.0.2/pd_extras/optimize/df_ops.py` & `pd_extras-5.0.3/pd_extras/optimize/df_ops.py`

 * *Files identical despite different names*

### Comparing `pd_extras-5.0.2/pd_extras/write/common.py` & `pd_extras-5.0.3/pd_extras/write/common.py`

 * *Files identical despite different names*

### Comparing `pd_extras-5.0.2/pd_extras/write/nosql_writer.py` & `pd_extras-5.0.3/pd_extras/write/nosql_writer.py`

 * *Files identical despite different names*

### Comparing `pd_extras-5.0.2/pd_extras/write/sql_writer.py` & `pd_extras-5.0.3/pd_extras/write/sql_writer.py`

 * *Files identical despite different names*

### Comparing `pd_extras-5.0.2/pyproject.toml` & `pd_extras-5.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pd-extras"
-version = "5.0.2"
+version = "5.0.3"
 description = "Some utility functions on top of pandas."
 authors = ["Masum Billal <billalmasum93@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/proafxin/pd-extras"
 documentation = "https://pd-extras.readthedocs.io/en/latest/"
```

### Comparing `pd_extras-5.0.2/PKG-INFO` & `pd_extras-5.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pd-extras
-Version: 5.0.2
+Version: 5.0.3
 Summary: Some utility functions on top of pandas.
 Home-page: https://github.com/proafxin/pd-extras
 License: MIT
 Author: Masum Billal
 Author-email: billalmasum93@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -30,15 +30,18 @@
 [![codecov](https://codecov.io/gh/proafxin/pd-extras/graph/badge.svg?token=AQA0IJY4N1)](https://codecov.io/gh/proafxin/pd-extras)
 [![Documentation Status](https://readthedocs.org/projects/pd-extras/badge/?version=latest)](https://pd-extras.readthedocs.io/en/latest/?badge=latest)
 
 Some functions on top of pandas.
 
 ## Install Environment
 
-Run `python -m pip install -U pip` and `pip install -U pip poetry`. Then run `poetry install`. If you are facing issues installing `mysqlclient` or `psycopg2` on Ubuntu, it's because you are missing some libraries. Please check their pages. Usually for `psycopg2`, it's `libpq-dev` and for `mysqlclient`, it's `python3-dev default-libmysqlclient-dev build-essential`. Check the pages for more specific and accurate commands.
+For local development:
+
+- Run `python -m pip install -U pip` and `pip install -U pip poetry`
+- Run `poetry install`. If you are facing issues installing `mysqlclient` or `psycopg2` on Ubuntu, it's because you are missing some libraries. Please check their pages. Usually for `psycopg2`, it's `libpq-dev` and for `mysqlclient`, it's `python3-dev default-libmysqlclient-dev build-essential`. Check the pages for more specific and accurate commands.
 
 ## Testing
 
 Run `docker compose up` then `tox`. Obviously you need docker and tox installed.
 
 ## Generate Documentation Source Files
```

