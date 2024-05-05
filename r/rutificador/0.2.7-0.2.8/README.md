# Comparing `tmp/rutificador-0.2.7.tar.gz` & `tmp/rutificador-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rutificador-0.2.7.tar", max compression
+gzip compressed data, was "rutificador-0.2.8.tar", max compression
```

## Comparing `rutificador-0.2.7.tar` & `rutificador-0.2.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1112 2024-05-04 19:32:50.055369 rutificador-0.2.7/LICENSE
--rw-r--r--   0        0        0     4452 2024-05-04 19:32:50.055369 rutificador-0.2.7/README.md
--rw-r--r--   0        0        0     1147 2024-05-04 19:32:50.055369 rutificador-0.2.7/pyproject.toml
--rw-r--r--   0        0        0      101 2024-05-04 19:32:50.055369 rutificador-0.2.7/rutificador/__init__.py
--rw-r--r--   0        0        0     9142 2024-05-04 19:32:50.055369 rutificador-0.2.7/rutificador/main.py
--rw-r--r--   0        0        0     5427 1970-01-01 00:00:00.000000 rutificador-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1112 2024-05-05 19:03:15.301237 rutificador-0.2.8/LICENSE
+-rw-r--r--   0        0        0     4616 2024-05-05 19:03:15.301237 rutificador-0.2.8/README.md
+-rw-r--r--   0        0        0     1147 2024-05-05 19:03:15.301237 rutificador-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0      101 2024-05-05 19:03:15.301237 rutificador-0.2.8/rutificador/__init__.py
+-rw-r--r--   0        0        0     9142 2024-05-05 19:03:15.301237 rutificador-0.2.8/rutificador/main.py
+-rw-r--r--   0        0        0     5591 1970-01-01 00:00:00.000000 rutificador-0.2.8/PKG-INFO
```

### Comparing `rutificador-0.2.7/LICENSE` & `rutificador-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rutificador-0.2.7/README.md` & `rutificador-0.2.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [![PyPI version](https://img.shields.io/pypi/v/rutificador.svg)](https://pypi.org/project/rutificador/)
 [![Python](https://img.shields.io/badge/Python-3.9%2B-blue)](https://www.python.org/)
 [![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Build](https://github.com/cortega26/rutificador/actions/workflows/ci.yml/badge.svg)](https://github.com/cortega26/rutificador/actions/workflows/ci.yml)
+[![Pylint](https://github.com/cortega26/rutificador/actions/workflows/pylint.yml/badge.svg)](https://github.com/cortega26/rutificador/actions/workflows/pylint.yml)
 
 # Rutificador
 
 Una biblioteca Python para validar y formatear RUTs (Rol Único Tributario) chilenos.
 
 ## Características
```

### Comparing `rutificador-0.2.7/pyproject.toml` & `rutificador-0.2.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rutificador"
-version = "0.2.7"
+version = "0.2.8"
 description = "Esta librería proporciona una implementación en Python para validar y formatear el Rol Único Tributario (RUT) utilizado en Chile."
 authors = ["Carlos Ortega González <carlosortega77@gmail.com>"]
 license = "MIT"
 homepage = "https://pypi.org/project/rutificador/"
 repository = "https://github.com/cortega26/Rutificador"
 keywords = ["RUT", "Chile", "validación", "formateo", "librería", "id", "rutificador", "rut-chile"]
 classifiers = [
```

### Comparing `rutificador-0.2.7/rutificador/main.py` & `rutificador-0.2.8/rutificador/main.py`

 * *Files identical despite different names*

### Comparing `rutificador-0.2.7/PKG-INFO` & `rutificador-0.2.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rutificador
-Version: 0.2.7
+Version: 0.2.8
 Summary: Esta librería proporciona una implementación en Python para validar y formatear el Rol Único Tributario (RUT) utilizado en Chile.
 Home-page: https://pypi.org/project/rutificador/
 License: MIT
 Keywords: RUT,Chile,validación,formateo,librería,id,rutificador,rut-chile
 Author: Carlos Ortega González
 Author-email: carlosortega77@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -21,14 +21,15 @@
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://img.shields.io/pypi/v/rutificador.svg)](https://pypi.org/project/rutificador/)
 [![Python](https://img.shields.io/badge/Python-3.9%2B-blue)](https://www.python.org/)
 [![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Build](https://github.com/cortega26/rutificador/actions/workflows/ci.yml/badge.svg)](https://github.com/cortega26/rutificador/actions/workflows/ci.yml)
+[![Pylint](https://github.com/cortega26/rutificador/actions/workflows/pylint.yml/badge.svg)](https://github.com/cortega26/rutificador/actions/workflows/pylint.yml)
 
 # Rutificador
 
 Una biblioteca Python para validar y formatear RUTs (Rol Único Tributario) chilenos.
 
 ## Características
```

