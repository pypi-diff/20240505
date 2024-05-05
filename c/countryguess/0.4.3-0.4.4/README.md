# Comparing `tmp/countryguess-0.4.3.tar.gz` & `tmp/countryguess-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "countryguess-0.4.3.tar", last modified: Sat Dec 16 13:56:25 2023, max compression
+gzip compressed data, was "countryguess-0.4.4.tar", last modified: Sun May  5 12:30:10 2024, max compression
```

## Comparing `countryguess-0.4.3.tar` & `countryguess-0.4.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwx------   0 ich       (1000) ich       (1000)        0 2023-12-16 13:56:25.510414 countryguess-0.4.3/
--rw-------   0 ich       (1000) ich       (1000)    35149 2022-10-10 15:59:38.000000 countryguess-0.4.3/LICENSE
--rw-r--r--   0 ich       (1000) ich       (1000)     8219 2023-12-16 13:56:25.510414 countryguess-0.4.3/PKG-INFO
--rw-------   0 ich       (1000) ich       (1000)     7105 2023-12-16 13:48:35.000000 countryguess-0.4.3/README.md
-drwx------   0 ich       (1000) ich       (1000)        0 2023-12-16 13:56:25.506414 countryguess-0.4.3/countryguess/
--rw-------   0 ich       (1000) ich       (1000)      137 2023-12-16 13:49:55.000000 countryguess-0.4.3/countryguess/__init__.py
--rw-------   0 ich       (1000) ich       (1000)       31 2022-10-10 15:59:38.000000 countryguess-0.4.3/countryguess/__main__.py
--rw-------   0 ich       (1000) ich       (1000)     1166 2022-10-10 15:59:38.000000 countryguess-0.4.3/countryguess/_cli.py
--rw-------   0 ich       (1000) ich       (1000)   274703 2023-12-16 13:48:34.000000 countryguess-0.4.3/countryguess/_countrydata.json
--rw-------   0 ich       (1000) ich       (1000)     6074 2023-03-12 11:09:04.000000 countryguess-0.4.3/countryguess/_countrydata.py
--rw-------   0 ich       (1000) ich       (1000)      655 2023-03-05 16:31:28.000000 countryguess-0.4.3/countryguess/_guess_country.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-12-16 13:56:25.506414 countryguess-0.4.3/countryguess.egg-info/
--rw-r--r--   0 ich       (1000) ich       (1000)     8219 2023-12-16 13:56:25.000000 countryguess-0.4.3/countryguess.egg-info/PKG-INFO
--rw-------   0 ich       (1000) ich       (1000)      466 2023-12-16 13:56:25.000000 countryguess-0.4.3/countryguess.egg-info/SOURCES.txt
--rw-------   0 ich       (1000) ich       (1000)        1 2023-12-16 13:56:25.000000 countryguess-0.4.3/countryguess.egg-info/dependency_links.txt
--rw-------   0 ich       (1000) ich       (1000)       55 2023-12-16 13:56:25.000000 countryguess-0.4.3/countryguess.egg-info/entry_points.txt
--rw-------   0 ich       (1000) ich       (1000)       56 2023-12-16 13:56:25.000000 countryguess-0.4.3/countryguess.egg-info/requires.txt
--rw-------   0 ich       (1000) ich       (1000)       29 2023-12-16 13:56:25.000000 countryguess-0.4.3/countryguess.egg-info/top_level.txt
--rw-------   0 ich       (1000) ich       (1000)     1441 2023-11-10 14:15:54.000000 countryguess-0.4.3/pyproject.toml
--rw-------   0 ich       (1000) ich       (1000)       38 2023-12-16 13:56:25.510414 countryguess-0.4.3/setup.cfg
-drwx------   0 ich       (1000) ich       (1000)        0 2023-12-16 13:56:25.506414 countryguess-0.4.3/tests/
--rw-------   0 ich       (1000) ich       (1000)    13993 2023-03-12 11:05:00.000000 countryguess-0.4.3/tests/countrydata_test.py
--rw-------   0 ich       (1000) ich       (1000)     2032 2023-03-05 16:30:33.000000 countryguess-0.4.3/tests/guess_country_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-05-05 12:30:10.617973 countryguess-0.4.4/
+-rw-------   0 ich       (1000) ich       (1000)    35149 2022-10-10 15:59:38.000000 countryguess-0.4.4/LICENSE
+-rw-r--r--   0 ich       (1000) ich       (1000)     8262 2024-05-05 12:30:10.617973 countryguess-0.4.4/PKG-INFO
+-rw-------   0 ich       (1000) ich       (1000)     7105 2024-05-05 12:00:55.000000 countryguess-0.4.4/README.md
+drwx------   0 ich       (1000) ich       (1000)        0 2024-05-05 12:30:10.613973 countryguess-0.4.4/countryguess/
+-rw-------   0 ich       (1000) ich       (1000)      137 2024-05-05 12:27:40.000000 countryguess-0.4.4/countryguess/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)       31 2022-10-10 15:59:38.000000 countryguess-0.4.4/countryguess/__main__.py
+-rw-------   0 ich       (1000) ich       (1000)     1166 2022-10-10 15:59:38.000000 countryguess-0.4.4/countryguess/_cli.py
+-rw-------   0 ich       (1000) ich       (1000)   274696 2024-05-05 12:00:55.000000 countryguess-0.4.4/countryguess/_countrydata.json
+-rw-------   0 ich       (1000) ich       (1000)     6074 2023-03-12 11:09:04.000000 countryguess-0.4.4/countryguess/_countrydata.py
+-rw-------   0 ich       (1000) ich       (1000)      655 2023-03-05 16:31:28.000000 countryguess-0.4.4/countryguess/_guess_country.py
+drwx------   0 ich       (1000) ich       (1000)        0 2024-05-05 12:30:10.617973 countryguess-0.4.4/countryguess.egg-info/
+-rw-r--r--   0 ich       (1000) ich       (1000)     8262 2024-05-05 12:30:10.000000 countryguess-0.4.4/countryguess.egg-info/PKG-INFO
+-rw-------   0 ich       (1000) ich       (1000)      466 2024-05-05 12:30:10.000000 countryguess-0.4.4/countryguess.egg-info/SOURCES.txt
+-rw-------   0 ich       (1000) ich       (1000)        1 2024-05-05 12:30:10.000000 countryguess-0.4.4/countryguess.egg-info/dependency_links.txt
+-rw-------   0 ich       (1000) ich       (1000)       55 2024-05-05 12:30:10.000000 countryguess-0.4.4/countryguess.egg-info/entry_points.txt
+-rw-------   0 ich       (1000) ich       (1000)       68 2024-05-05 12:30:10.000000 countryguess-0.4.4/countryguess.egg-info/requires.txt
+-rw-------   0 ich       (1000) ich       (1000)       29 2024-05-05 12:30:10.000000 countryguess-0.4.4/countryguess.egg-info/top_level.txt
+-rw-------   0 ich       (1000) ich       (1000)     1520 2024-05-05 12:06:06.000000 countryguess-0.4.4/pyproject.toml
+-rw-------   0 ich       (1000) ich       (1000)       38 2024-05-05 12:30:10.617973 countryguess-0.4.4/setup.cfg
+drwx------   0 ich       (1000) ich       (1000)        0 2024-05-05 12:30:10.617973 countryguess-0.4.4/tests/
+-rw-------   0 ich       (1000) ich       (1000)    13993 2023-03-12 11:05:00.000000 countryguess-0.4.4/tests/countrydata_test.py
+-rw-------   0 ich       (1000) ich       (1000)     2032 2023-03-05 16:30:33.000000 countryguess-0.4.4/tests/guess_country_test.py
```

### Comparing `countryguess-0.4.3/LICENSE` & `countryguess-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `countryguess-0.4.3/PKG-INFO` & `countryguess-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countryguess
-Version: 0.4.3
+Version: 0.4.4
 Summary: Fuzzy lookup of country information
 Author-email: plotski <plotski@example.org>
 License: GPL-3.0-or-later
 Project-URL: Repository, https://codeberg.org/plotski/countryguess
 Project-URL: Bug Tracker, https://codeberg.org/plotski/countryguess/issues
 Project-URL: Changelog, https://codeberg.org/plotski/countryguess/raw/branch/master/NEWS
 Classifier: Programming Language :: Python :: 3.8
@@ -17,14 +17,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pytest-mock; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 
 **countryguess** looks up country information by country codes or name matching.
 It tries to be lean (but not mean) and fast: All dependencies are in the Python
 Standard Library and country data is loaded lazily on demand.
```

### Comparing `countryguess-0.4.3/README.md` & `countryguess-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `countryguess-0.4.3/countryguess/_cli.py` & `countryguess-0.4.4/countryguess/_cli.py`

 * *Files identical despite different names*

### Comparing `countryguess-0.4.3/countryguess/_countrydata.json` & `countryguess-0.4.4/countryguess/_countrydata.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998828124999999%*

 * *Differences: {'32': "{'iso2': 'BQ', 'iso3': 'ATB'}", '89': "{'iso2': 'GR'}"}*

```diff
@@ -1694,16 +1694,16 @@
         "g20": "",
         "g7": "",
         "gbdcode": "",
         "gwcode": "",
         "iea": "",
         "image": "",
         "ioc": "",
-        "iso2": "B1",
-        "iso3": "BA1",
+        "iso2": "BQ",
+        "iso3": "ATB",
         "isonumeric": "",
         "message": "",
         "name_official": "British Antarctic Territories",
         "name_short": "British Antarctic Territories",
         "obsolete": "1979",
         "oecd": "",
         "regex": "br.*antarctic.?territ.*",
@@ -4658,15 +4658,15 @@
         "g20": "G20",
         "g7": "",
         "gbdcode": "82",
         "gwcode": "350",
         "iea": "Greece",
         "image": "Western Europe",
         "ioc": "GRE",
-        "iso2": "^GR$|^EL$",
+        "iso2": "GR",
         "iso3": "GRC",
         "isonumeric": "300",
         "message": "WEU",
         "name_official": "Hellenic Republic",
         "name_short": "Greece",
         "obsolete": "",
         "oecd": "1961",
```

### Comparing `countryguess-0.4.3/countryguess/_countrydata.py` & `countryguess-0.4.4/countryguess/_countrydata.py`

 * *Files identical despite different names*

### Comparing `countryguess-0.4.3/countryguess/_guess_country.py` & `countryguess-0.4.4/countryguess/_guess_country.py`

 * *Files identical despite different names*

### Comparing `countryguess-0.4.3/countryguess.egg-info/PKG-INFO` & `countryguess-0.4.4/countryguess.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countryguess
-Version: 0.4.3
+Version: 0.4.4
 Summary: Fuzzy lookup of country information
 Author-email: plotski <plotski@example.org>
 License: GPL-3.0-or-later
 Project-URL: Repository, https://codeberg.org/plotski/countryguess
 Project-URL: Bug Tracker, https://codeberg.org/plotski/countryguess/issues
 Project-URL: Changelog, https://codeberg.org/plotski/countryguess/raw/branch/master/NEWS
 Classifier: Programming Language :: Python :: 3.8
@@ -17,14 +17,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pytest-mock; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 
 **countryguess** looks up country information by country codes or name matching.
 It tries to be lean (but not mean) and fast: All dependencies are in the Python
 Standard Library and country data is loaded lazily on demand.
```

### Comparing `countryguess-0.4.3/pyproject.toml` & `countryguess-0.4.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 dev = [
     "pytest",
 
     "tox",
 
     "coverage",
     "pytest-cov",
+    "pytest-mock",
 
     "ruff",
     "flake8",
     "isort",
 ]
 
 [project.scripts]
@@ -48,9 +49,12 @@
 
 # For some unknown reason, we need to specify explicity to scan the project
 # directory with default parameters or setuptools gets confused about
 # directories like "docs" or "venv".
 [tool.setuptools.packages]
 find = {}
 
+[tool.setuptools.package-data]
+"*" = ["_countrydata.json"]
+
 [tool.setuptools.dynamic]
 version = {attr = "countryguess.__version__"}
```

### Comparing `countryguess-0.4.3/tests/countrydata_test.py` & `countryguess-0.4.4/tests/countrydata_test.py`

 * *Files identical despite different names*

### Comparing `countryguess-0.4.3/tests/guess_country_test.py` & `countryguess-0.4.4/tests/guess_country_test.py`

 * *Files identical despite different names*

