# Comparing `tmp/prionet-0.0.0.tar.gz` & `tmp/prionet-0.0.1.tar.gz`

## Comparing `prionet-0.0.0.tar` & `prionet-0.0.1.tar`

### file list

```diff
@@ -1,6 +1,10 @@
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 prionet-0.0.0/src/PrioNet/__init__.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 prionet-0.0.0/src/PrioNet/example.py
--rw-r--r--   0        0        0    34502 2020-02-02 00:00:00.000000 prionet-0.0.0/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 prionet-0.0.0/README.md
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 prionet-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 prionet-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 prionet-0.0.1/src/PrioNet/__init__.py
+-rw-r--r--   0        0        0     4766 2020-02-02 00:00:00.000000 prionet-0.0.1/src/PrioNet/bybit.py
+-rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 prionet-0.0.1/src/PrioNet/log.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 prionet-0.0.1/src/PrioNet/telegram.py
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 prionet-0.0.1/tests/log.ipynb
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 prionet-0.0.1/.gitignore
+-rw-r--r--   0        0        0    34502 2020-02-02 00:00:00.000000 prionet-0.0.1/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 prionet-0.0.1/README.md
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 prionet-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 prionet-0.0.1/PKG-INFO
```

### Comparing `prionet-0.0.0/LICENSE` & `prionet-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prionet-0.0.0/pyproject.toml` & `prionet-0.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "PrioNet"
-version = "0.0.0"
+version = "0.0.1"
 authors = [
   { name="Giuseppe Priolo", email="priopio7@gmail.com" },
 ]
 description = "A package for analyizing financial data"
 readme = "README.md"
 requires-python = ">=3"
 classifiers = [
```

