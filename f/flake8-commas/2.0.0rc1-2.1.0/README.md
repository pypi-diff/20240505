# Comparing `tmp/flake8-commas-2.0.0rc1.tar.gz` & `tmp/flake8-commas-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flake8-commas-2.0.0rc1.tar", last modified: Mon Mar 19 12:01:39 2018, max compression
+gzip compressed data, was "flake8-commas-2.1.0.tar", last modified: Wed Oct 13 19:25:35 2021, max compression
```

## Comparing `flake8-commas-2.0.0rc1.tar` & `flake8-commas-2.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 graingert  (1001) graingert  (1001)        0 2018-03-19 12:01:39.000000 flake8-commas-2.0.0rc1/
-drwxrwxr-x   0 graingert  (1001) graingert  (1001)        0 2018-03-19 12:01:39.000000 flake8-commas-2.0.0rc1/test/
--rw-rw-r--   0 graingert  (1001) graingert  (1001)      418 2018-03-19 12:01:38.000000 flake8-commas-2.0.0rc1/test/test_flake8.py
--rw-rw-r--   0 graingert  (1001) graingert  (1001)     9982 2018-03-19 12:01:38.000000 flake8-commas-2.0.0rc1/test/test_checks.py
--rw-rw-r--   0 graingert  (1001) graingert  (1001)     1305 2018-03-19 12:01:38.000000 flake8-commas-2.0.0rc1/README.rst
--rw-rw-r--   0 graingert  (1001) graingert  (1001)      103 2018-03-19 12:01:39.000000 flake8-commas-2.0.0rc1/setup.cfg
--rw-rw-r--   0 graingert  (1001) graingert  (1001)      101 2018-03-19 12:01:38.000000 flake8-commas-2.0.0rc1/MANIFEST.in
-drwxrwxr-x   0 graingert  (1001) graingert  (1001)        0 2018-03-19 12:01:39.000000 flake8-commas-2.0.0rc1/flake8_commas/
--rw-rw-r--   0 graingert  (1001) graingert  (1001)    10535 2018-03-19 12:01:38.000000 flake8-commas-2.0.0rc1/flake8_commas/_base.py
--rw-rw-r--   0 graingert  (1001) graingert  (1001)      123 2018-03-19 12:01:38.000000 flake8-commas-2.0.0rc1/flake8_commas/__init__.py
--rw-rw-r--   0 graingert  (1001) graingert  (1001)     1761 2018-03-19 12:01:38.000000 flake8-commas-2.0.0rc1/setup.py
--rw-rw-r--   0 graingert  (1001) graingert  (1001)     3499 2018-03-19 12:01:38.000000 flake8-commas-2.0.0rc1/CHANGES.rst
-drwxrwxr-x   0 graingert  (1001) graingert  (1001)        0 2018-03-19 12:01:39.000000 flake8-commas-2.0.0rc1/flake8_commas.egg-info/
--rw-rw-r--   0 graingert  (1001) graingert  (1001)       53 2018-03-19 12:01:38.000000 flake8-commas-2.0.0rc1/flake8_commas.egg-info/entry_points.txt
--rw-rw-r--   0 graingert  (1001) graingert  (1001)        1 2018-03-19 12:01:38.000000 flake8-commas-2.0.0rc1/flake8_commas.egg-info/dependency_links.txt
--rw-rw-r--   0 graingert  (1001) graingert  (1001)       14 2018-03-19 12:01:38.000000 flake8-commas-2.0.0rc1/flake8_commas.egg-info/top_level.txt
--rw-rw-r--   0 graingert  (1001) graingert  (1001)       17 2018-03-19 12:01:38.000000 flake8-commas-2.0.0rc1/flake8_commas.egg-info/requires.txt
--rw-rw-r--   0 graingert  (1001) graingert  (1001)      366 2018-03-19 12:01:38.000000 flake8-commas-2.0.0rc1/flake8_commas.egg-info/SOURCES.txt
--rw-rw-r--   0 graingert  (1001) graingert  (1001)     6972 2018-03-19 12:01:38.000000 flake8-commas-2.0.0rc1/flake8_commas.egg-info/PKG-INFO
--rw-rw-r--   0 graingert  (1001) graingert  (1001)     6972 2018-03-19 12:01:39.000000 flake8-commas-2.0.0rc1/PKG-INFO
+drwxrwxr-x   0 graingert  (1000) graingert  (1000)        0 2021-10-13 19:25:35.320993 flake8-commas-2.1.0/
+-rw-rw-r--   0 graingert  (1000) graingert  (1000)     3901 2021-10-13 19:25:35.000000 flake8-commas-2.1.0/CHANGES.rst
+-rw-rw-r--   0 graingert  (1000) graingert  (1000)      101 2021-10-13 19:25:35.000000 flake8-commas-2.1.0/MANIFEST.in
+-rw-rw-r--   0 graingert  (1000) graingert  (1000)     8501 2021-10-13 19:25:35.320993 flake8-commas-2.1.0/PKG-INFO
+-rw-rw-r--   0 graingert  (1000) graingert  (1000)     2005 2021-10-13 19:25:35.000000 flake8-commas-2.1.0/README.rst
+drwxrwxr-x   0 graingert  (1000) graingert  (1000)        0 2021-10-13 19:25:35.320993 flake8-commas-2.1.0/flake8_commas/
+-rw-rw-r--   0 graingert  (1000) graingert  (1000)      123 2021-10-13 19:25:35.000000 flake8-commas-2.1.0/flake8_commas/__init__.py
+-rw-rw-r--   0 graingert  (1000) graingert  (1000)    10535 2021-10-13 19:25:35.000000 flake8-commas-2.1.0/flake8_commas/_base.py
+drwxrwxr-x   0 graingert  (1000) graingert  (1000)        0 2021-10-13 19:25:35.320993 flake8-commas-2.1.0/flake8_commas.egg-info/
+-rw-rw-r--   0 graingert  (1000) graingert  (1000)     8501 2021-10-13 19:25:35.000000 flake8-commas-2.1.0/flake8_commas.egg-info/PKG-INFO
+-rw-rw-r--   0 graingert  (1000) graingert  (1000)      366 2021-10-13 19:25:35.000000 flake8-commas-2.1.0/flake8_commas.egg-info/SOURCES.txt
+-rw-rw-r--   0 graingert  (1000) graingert  (1000)        1 2021-10-13 19:25:35.000000 flake8-commas-2.1.0/flake8_commas.egg-info/dependency_links.txt
+-rw-rw-r--   0 graingert  (1000) graingert  (1000)       53 2021-10-13 19:25:35.000000 flake8-commas-2.1.0/flake8_commas.egg-info/entry_points.txt
+-rw-rw-r--   0 graingert  (1000) graingert  (1000)       10 2021-10-13 19:25:35.000000 flake8-commas-2.1.0/flake8_commas.egg-info/requires.txt
+-rw-rw-r--   0 graingert  (1000) graingert  (1000)       14 2021-10-13 19:25:35.000000 flake8-commas-2.1.0/flake8_commas.egg-info/top_level.txt
+-rw-rw-r--   0 graingert  (1000) graingert  (1000)      103 2021-10-13 19:25:35.320993 flake8-commas-2.1.0/setup.cfg
+-rw-rw-r--   0 graingert  (1000) graingert  (1000)     1897 2021-10-13 19:25:35.000000 flake8-commas-2.1.0/setup.py
+drwxrwxr-x   0 graingert  (1000) graingert  (1000)        0 2021-10-13 19:25:35.320993 flake8-commas-2.1.0/test/
+-rw-rw-r--   0 graingert  (1000) graingert  (1000)     9785 2021-10-13 19:25:35.000000 flake8-commas-2.1.0/test/test_checks.py
+-rw-rw-r--   0 graingert  (1000) graingert  (1000)      418 2021-10-13 19:25:35.000000 flake8-commas-2.1.0/test/test_flake8.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `flake8-commas-2.0.0rc1/test/test_checks.py` & `flake8-commas-2.1.0/test/test_checks.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     get_tokens, get_noqa_lines, get_comma_errors,
 )
 
 C813 = 'C813 missing trailing comma in Python 3'
 C814 = 'C814 missing trailing comma in Python 2'
 C815 = 'C815 missing trailing comma in Python 3.5+'
 C816 = 'C816 missing trailing comma in Python 3.6+'
+C818 = 'C818 trailing comma on bare tuple prohibited'
 
 
 def test_get_noqa_lines():
     filename = get_absolute_path('data/no_qa.py')
     assert get_noqa_lines(get_tokens(filename)) == [2]
 
 
@@ -244,24 +245,19 @@
     ]
 
 
 def test_bare():
     # Tests inspired by flake8_tuple https://git.io/vxstN
     filename = get_absolute_path('data/bare.py')
     assert list(get_comma_errors(get_tokens(filename))) == [
-       {'col': 8, 'line': 7,
-        'message': 'C818 trailing comma on bare tuple prohibited'},
-       {'col': 19, 'line': 9,
-        'message': 'C818 trailing comma on bare tuple prohibited'},
-       {'col': 8, 'line': 16,
-        'message': 'C818 trailing comma on bare tuple prohibited'},
-       {'col': 10, 'line': 20,
-        'message': 'C818 trailing comma on bare tuple prohibited'},
-       {'col': 32, 'line': 27,
-        'message': 'C818 trailing comma on bare tuple prohibited'},
-       {'col': 26, 'line': 29,
-        'message': 'C818 trailing comma on bare tuple prohibited'},
+       {'col': 8, 'line': 7, 'message': C818},
+       {'col': 19, 'line': 9, 'message': C818},
+       {'col': 8, 'line': 16, 'message': C818},
+       {'col': 10, 'line': 20, 'message': C818},
+       {'col': 32, 'line': 27, 'message': C818},
+       {'col': 26, 'line': 29, 'message': C818},
+       {'col': 17, 'line': 32, 'message': C818},
     ]
 
 
 def get_absolute_path(filepath):
     return os.path.join(os.path.dirname(__file__), filepath)
```

### Comparing `flake8-commas-2.0.0rc1/flake8_commas/_base.py` & `flake8-commas-2.1.0/flake8_commas/_base.py`

 * *Files identical despite different names*

### Comparing `flake8-commas-2.0.0rc1/CHANGES.rst` & `flake8-commas-2.1.0/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,19 @@
-2.0.0rc1 (2018-03-19)
----------------------
+2.1.0 (2021-10-13)
+------------------
+
+- Remove upper bound on flake8.
+  (`Issue #67 <https://github.com/PyCQA/flake8-commas/issues/67>`_)
+- Note: this project is no longer maintained, and now black
+  or https://github.com/asottile/add-trailing-comma is recommended instead.
+  (`Issue #63 <https://github.com/PyCQA/flake8-commas/pull/63>`_)
+  (`Issue #69 <https://github.com/PyCQA/flake8-commas/pull/69>`_)
+
+2.0.0 (2018-03-19)
+------------------
 
 - Hide ._base from flake8 --version.
   (`Issue #45 <https://github.com/PyCQA/flake8-commas/issue/45>`_)
 - Update URL to https://github.com/PyCQA/flake8-commas/.
   (`Issue #51 <https://github.com/PyCQA/flake8-commas/pull/51>`_)
 - Add check for trailing commas on bare tuples - C818, thanks to
   `Chris AtLee <https://github.com/catlee>`_ and
```

### Comparing `flake8-commas-2.0.0rc1/flake8_commas.egg-info/PKG-INFO` & `flake8-commas-2.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 Metadata-Version: 1.2
 Name: flake8-commas
-Version: 2.0.0rc1
+Version: 2.1.0
 Summary: Flake8 lint for trailing commas.
 Home-page: https://github.com/PyCQA/flake8-commas/
 Author: Trevor Creech
 Author-email: trevor@trevorcreech.com
 Maintainer: Thomas Grainger
 Maintainer-email: flake8-commas@graingert.co.uk
 License: UNKNOWN
 Description: Flake8 Extension to enforce better comma placement.
         ===================================================
         
+        .. image:: https://unmaintained.tech/badge.svg
+          :target: https://unmaintained.tech
+          :alt: No Maintenance Intended
+          
+        
+        **Note:** `Black <https://pypi.org/project/black/>`_, the uncompromising Python code
+        formatter, or  `add-trailing-comma <https://github.com/asottile/add-trailing-comma>`_
+        can do all this comma insertion automatically. We recommend you use one of those tools
+        instead.
+        
         Usage
         -----
         
         If you are using flake8 it's as easy as:
         
         .. code:: shell
         
@@ -42,17 +52,42 @@
         | C816 | missing trailing comma in Python 3.6+   |
         +------+-----------------------------------------+
         | C818 | trailing comma on bare tuple prohibited |
         +------+-----------------------------------------+
         | C819 | trailing comma prohibited               |
         +------+-----------------------------------------+
         
+        Examples
+        --------
+        
+        .. code:: Python
+        
+            lookup_table = {
+                'key1': 'value',
+                'key2': 'something'  # <-- missing a trailing comma
+            }
+        
+            json_data = json.dumps({
+                "key": "value",
+            }),                      # <-- incorrect trailing comma. json_data is now a tuple. Likely by accident.
+        
         
-        2.0.0rc1 (2018-03-19)
-        ---------------------
+        
+        2.1.0 (2021-10-13)
+        ------------------
+        
+        - Remove upper bound on flake8.
+          (`Issue #67 <https://github.com/PyCQA/flake8-commas/issues/67>`_)
+        - Note: this project is no longer maintained, and now black
+          or https://github.com/asottile/add-trailing-comma is recommended instead.
+          (`Issue #63 <https://github.com/PyCQA/flake8-commas/pull/63>`_)
+          (`Issue #69 <https://github.com/PyCQA/flake8-commas/pull/69>`_)
+        
+        2.0.0 (2018-03-19)
+        ------------------
         
         - Hide ._base from flake8 --version.
           (`Issue #45 <https://github.com/PyCQA/flake8-commas/issue/45>`_)
         - Update URL to https://github.com/PyCQA/flake8-commas/.
           (`Issue #51 <https://github.com/PyCQA/flake8-commas/pull/51>`_)
         - Add check for trailing commas on bare tuples - C818, thanks to
           `Chris AtLee <https://github.com/catlee>`_ and
@@ -160,10 +195,13 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Framework :: Flake8
```

### Comparing `flake8-commas-2.0.0rc1/PKG-INFO` & `flake8-commas-2.1.0/flake8_commas.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 Metadata-Version: 1.2
 Name: flake8-commas
-Version: 2.0.0rc1
+Version: 2.1.0
 Summary: Flake8 lint for trailing commas.
 Home-page: https://github.com/PyCQA/flake8-commas/
 Author: Trevor Creech
 Author-email: trevor@trevorcreech.com
 Maintainer: Thomas Grainger
 Maintainer-email: flake8-commas@graingert.co.uk
 License: UNKNOWN
 Description: Flake8 Extension to enforce better comma placement.
         ===================================================
         
+        .. image:: https://unmaintained.tech/badge.svg
+          :target: https://unmaintained.tech
+          :alt: No Maintenance Intended
+          
+        
+        **Note:** `Black <https://pypi.org/project/black/>`_, the uncompromising Python code
+        formatter, or  `add-trailing-comma <https://github.com/asottile/add-trailing-comma>`_
+        can do all this comma insertion automatically. We recommend you use one of those tools
+        instead.
+        
         Usage
         -----
         
         If you are using flake8 it's as easy as:
         
         .. code:: shell
         
@@ -42,17 +52,42 @@
         | C816 | missing trailing comma in Python 3.6+   |
         +------+-----------------------------------------+
         | C818 | trailing comma on bare tuple prohibited |
         +------+-----------------------------------------+
         | C819 | trailing comma prohibited               |
         +------+-----------------------------------------+
         
+        Examples
+        --------
+        
+        .. code:: Python
+        
+            lookup_table = {
+                'key1': 'value',
+                'key2': 'something'  # <-- missing a trailing comma
+            }
+        
+            json_data = json.dumps({
+                "key": "value",
+            }),                      # <-- incorrect trailing comma. json_data is now a tuple. Likely by accident.
+        
         
-        2.0.0rc1 (2018-03-19)
-        ---------------------
+        
+        2.1.0 (2021-10-13)
+        ------------------
+        
+        - Remove upper bound on flake8.
+          (`Issue #67 <https://github.com/PyCQA/flake8-commas/issues/67>`_)
+        - Note: this project is no longer maintained, and now black
+          or https://github.com/asottile/add-trailing-comma is recommended instead.
+          (`Issue #63 <https://github.com/PyCQA/flake8-commas/pull/63>`_)
+          (`Issue #69 <https://github.com/PyCQA/flake8-commas/pull/69>`_)
+        
+        2.0.0 (2018-03-19)
+        ------------------
         
         - Hide ._base from flake8 --version.
           (`Issue #45 <https://github.com/PyCQA/flake8-commas/issue/45>`_)
         - Update URL to https://github.com/PyCQA/flake8-commas/.
           (`Issue #51 <https://github.com/PyCQA/flake8-commas/pull/51>`_)
         - Add check for trailing commas on bare tuples - C818, thanks to
           `Chris AtLee <https://github.com/catlee>`_ and
@@ -160,10 +195,13 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Framework :: Flake8
```

