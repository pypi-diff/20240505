# Comparing `tmp/python_trading212-2.0.0.tar.gz` & `tmp/python_trading212-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_trading212-2.0.0.tar", max compression
+gzip compressed data, was "python_trading212-2.0.1.tar", max compression
```

## Comparing `python_trading212-2.0.0.tar` & `python_trading212-2.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2024-05-01 08:27:35.956775 python_trading212-2.0.0/LICENSE.md
--rw-r--r--   0        0        0     2083 2024-05-01 08:27:35.956775 python_trading212-2.0.0/README.md
--rw-r--r--   0        0        0      507 2024-05-01 08:27:35.956775 python_trading212-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      310 2024-05-01 08:27:35.956775 python_trading212-2.0.0/trading212/__init__.py
--rw-r--r--   0        0        0     5287 2024-05-01 08:27:35.956775 python_trading212-2.0.0/trading212/models.py
--rw-r--r--   0        0        0    12521 2024-05-01 08:27:35.956775 python_trading212-2.0.0/trading212/trading212.py
--rw-r--r--   0        0        0     2538 1970-01-01 00:00:00.000000 python_trading212-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-05 20:21:21.476584 python_trading212-2.0.1/LICENSE.md
+-rw-r--r--   0        0        0     2225 2024-05-05 20:21:21.476584 python_trading212-2.0.1/README.md
+-rw-r--r--   0        0        0     1098 2024-05-05 20:21:21.476584 python_trading212-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0      310 2024-05-05 20:21:21.476584 python_trading212-2.0.1/trading212/__init__.py
+-rw-r--r--   0        0        0     5287 2024-05-05 20:21:21.476584 python_trading212-2.0.1/trading212/models.py
+-rw-r--r--   0        0        0    12522 2024-05-05 20:21:21.476584 python_trading212-2.0.1/trading212/trading212.py
+-rw-r--r--   0        0        0     3200 1970-01-01 00:00:00.000000 python_trading212-2.0.1/PKG-INFO
```

### Comparing `python_trading212-2.0.0/LICENSE.md` & `python_trading212-2.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `python_trading212-2.0.0/README.md` & `python_trading212-2.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # python-trading212
 
 ![CICD Status](https://img.shields.io/github/actions/workflow/status/jcoelho93/python-trading212/ci.yml?label=cicd)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/python-trading212)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/python-trading212?logo=pypi&link=https%3A%2F%2Fpypi.org%2Fproject%2Fpython-trading212%2F)
 ![GitHub License](https://img.shields.io/github/license/jcoelho93/python-trading212)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/python-trading212)
-![PyPI - Version](https://img.shields.io/pypi/v/python-trading212)
+![PyPI - Version](https://img.shields.io/pypi/v/python-trading212?logo=pypi&link=https%3A%2F%2Fpypi.org%2Fproject%2Fpython-trading212%2F)
 
 
 A client for the [Trading212 API](https://t212public-api-docs.redoc.ly/)
 
 ## Installation
 
 ```bash
```

### Comparing `python_trading212-2.0.0/trading212/models.py` & `python_trading212-2.0.1/trading212/models.py`

 * *Files identical despite different names*

### Comparing `python_trading212-2.0.0/trading212/trading212.py` & `python_trading212-2.0.1/trading212/trading212.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
         Args:
             pie (Pie): the new pie to create
 
         Returns:
             Pie: the new pie
         """
-        endpoint = self.url + "equity/pie"
+        endpoint = self.url + "equity/pies"
         response = self._post(endpoint, pie.model_dump())
 
         return Pie(**response)
 
     def delete_pie(self, id: int) -> None:
         """Deletes a pie by ID
```

### Comparing `python_trading212-2.0.0/PKG-INFO` & `python_trading212-2.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 Metadata-Version: 2.1
 Name: python-trading212
-Version: 2.0.0
+Version: 2.0.1
 Summary: An unofficial client for the official Trading212 API
+Home-page: https://github.com/jcoelho93/python-trading212
+License: MIT
+Keywords: python,trading212,api,client,unofficial,finance,stocks,trading
 Author: José Coelho
 Author-email: 16445494+jcoelho93@users.noreply.github.com
 Requires-Python: >=3.12,<4.0
+Classifier: Framework :: Pydantic
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Office/Business :: Financial :: Investment
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Project-URL: Bug Tracker, https://github.com/jcoelho93/python-trading212/issues
+Project-URL: Documentation, https://github.com/jcoelho93/python-trading212
+Project-URL: Repository, https://github.com/jcoelho93/python-trading212
 Description-Content-Type: text/markdown
 
 # python-trading212
 
 ![CICD Status](https://img.shields.io/github/actions/workflow/status/jcoelho93/python-trading212/ci.yml?label=cicd)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/python-trading212)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/python-trading212?logo=pypi&link=https%3A%2F%2Fpypi.org%2Fproject%2Fpython-trading212%2F)
 ![GitHub License](https://img.shields.io/github/license/jcoelho93/python-trading212)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/python-trading212)
-![PyPI - Version](https://img.shields.io/pypi/v/python-trading212)
+![PyPI - Version](https://img.shields.io/pypi/v/python-trading212?logo=pypi&link=https%3A%2F%2Fpypi.org%2Fproject%2Fpython-trading212%2F)
 
 
 A client for the [Trading212 API](https://t212public-api-docs.redoc.ly/)
 
 ## Installation
 
 ```bash
```

