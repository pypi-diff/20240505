# Comparing `tmp/python_trading212-2.0.1.tar.gz` & `tmp/python_trading212-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_trading212-2.0.1.tar", max compression
+gzip compressed data, was "python_trading212-2.0.2.tar", max compression
```

## Comparing `python_trading212-2.0.1.tar` & `python_trading212-2.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2024-05-05 20:21:21.476584 python_trading212-2.0.1/LICENSE.md
--rw-r--r--   0        0        0     2225 2024-05-05 20:21:21.476584 python_trading212-2.0.1/README.md
--rw-r--r--   0        0        0     1098 2024-05-05 20:21:21.476584 python_trading212-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      310 2024-05-05 20:21:21.476584 python_trading212-2.0.1/trading212/__init__.py
--rw-r--r--   0        0        0     5287 2024-05-05 20:21:21.476584 python_trading212-2.0.1/trading212/models.py
--rw-r--r--   0        0        0    12522 2024-05-05 20:21:21.476584 python_trading212-2.0.1/trading212/trading212.py
--rw-r--r--   0        0        0     3200 1970-01-01 00:00:00.000000 python_trading212-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-05 20:33:13.742837 python_trading212-2.0.2/LICENSE.md
+-rw-r--r--   0        0        0     2225 2024-05-05 20:33:13.742837 python_trading212-2.0.2/README.md
+-rw-r--r--   0        0        0     1098 2024-05-05 20:33:13.742837 python_trading212-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0      310 2024-05-05 20:33:13.742837 python_trading212-2.0.2/trading212/__init__.py
+-rw-r--r--   0        0        0     5287 2024-05-05 20:33:13.742837 python_trading212-2.0.2/trading212/models.py
+-rw-r--r--   0        0        0    12525 2024-05-05 20:33:13.742837 python_trading212-2.0.2/trading212/trading212.py
+-rw-r--r--   0        0        0     3200 1970-01-01 00:00:00.000000 python_trading212-2.0.2/PKG-INFO
```

### Comparing `python_trading212-2.0.1/LICENSE.md` & `python_trading212-2.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `python_trading212-2.0.1/README.md` & `python_trading212-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `python_trading212-2.0.1/pyproject.toml` & `python_trading212-2.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-trading212"
-version = "2.0.1"
+version = "2.0.2"
 description = "An unofficial client for the official Trading212 API"
 authors = ["José Coelho <16445494+jcoelho93@users.noreply.github.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/jcoelho93/python-trading212"
 repository = "https://github.com/jcoelho93/python-trading212"
 documentation = "https://github.com/jcoelho93/python-trading212"
```

### Comparing `python_trading212-2.0.1/trading212/models.py` & `python_trading212-2.0.2/trading212/models.py`

 * *Files identical despite different names*

### Comparing `python_trading212-2.0.1/trading212/trading212.py` & `python_trading212-2.0.2/trading212/trading212.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,29 +126,29 @@
         """Deletes a pie by ID
 
         https://t212public-api-docs.redoc.ly/#operation/delete
 
         Args:
             id (int): the ID of the pie
         """
-        endpoint = self.url + f"equity/pie/{id}"
+        endpoint = self.url + f"equity/pies/{id}"
         return self._delete(endpoint)
 
     def fetch_pie(self, id: int) -> Pie:
         """Fetches a pies for the account with detailed information
 
         https://t212public-api-docs.redoc.ly/#operation/getDetailed
 
         Args:
             id (int): the ID of the pie
 
         Returns:
             Pie: the pie
         """
-        endpoint = self.url + f"equity/pie/{id}"
+        endpoint = self.url + f"equity/pies/{id}"
         response = self._get(endpoint)
 
         return Pie(**response)
 
     def update_pie(self, id: int, pie: Pie) -> Pie:
         """Updates a pie by ID
 
@@ -157,15 +157,15 @@
         Args:
             id (int): the ID of the pie
             pie (Pie): the new pie
 
         Returns:
             Pie: the new pie
         """
-        endpoint = self.url + f"equity/pie/{id}"
+        endpoint = self.url + f"equity/pies/{id}"
         response = self._post(endpoint, pie.model_dump())
 
         return Pie(**response)
 
     def fetch_all_orders(self) -> List[Order]:
         """ Fetches all orders
```

### Comparing `python_trading212-2.0.1/PKG-INFO` & `python_trading212-2.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-trading212
-Version: 2.0.1
+Version: 2.0.2
 Summary: An unofficial client for the official Trading212 API
 Home-page: https://github.com/jcoelho93/python-trading212
 License: MIT
 Keywords: python,trading212,api,client,unofficial,finance,stocks,trading
 Author: José Coelho
 Author-email: 16445494+jcoelho93@users.noreply.github.com
 Requires-Python: >=3.12,<4.0
```

