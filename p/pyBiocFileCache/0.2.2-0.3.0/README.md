# Comparing `tmp/pyBiocFileCache-0.2.2.tar.gz` & `tmp/pybiocfilecache-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyBiocFileCache-0.2.2.tar", last modified: Mon Jun  5 17:43:07 2023, max compression
+gzip compressed data, was "pybiocfilecache-0.3.0.tar", last modified: Sun May  5 16:25:47 2024, max compression
```

## Comparing `pyBiocFileCache-0.2.2.tar` & `pybiocfilecache-0.3.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:07.165129 pyBiocFileCache-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:07.145129 pyBiocFileCache-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:07.153129 pyBiocFileCache-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    13950 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-05 17:43:07.165129 pyBiocFileCache-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:07.157129 pyBiocFileCache-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:07.157129 pyBiocFileCache-0.2.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-05 17:43:07.165129 pyBiocFileCache-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:07.145129 pyBiocFileCache-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:07.157129 pyBiocFileCache-0.2.2/src/pyBiocFileCache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-05 17:43:07.000000 pyBiocFileCache-0.2.2/src/pyBiocFileCache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-05 17:43:07.000000 pyBiocFileCache-0.2.2/src/pyBiocFileCache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:43:07.000000 pyBiocFileCache-0.2.2/src/pyBiocFileCache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:42:24.000000 pyBiocFileCache-0.2.2/src/pyBiocFileCache.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-05 17:43:07.000000 pyBiocFileCache-0.2.2/src/pyBiocFileCache.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-05 17:43:07.000000 pyBiocFileCache-0.2.2/src/pyBiocFileCache.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:07.161129 pyBiocFileCache-0.2.2/src/pybiocfilecache/
--rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/src/pybiocfilecache/BiocFileCache.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/src/pybiocfilecache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/src/pybiocfilecache/_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:07.161129 pyBiocFileCache-0.2.2/src/pybiocfilecache/db/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/src/pybiocfilecache/db/Base.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/src/pybiocfilecache/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/src/pybiocfilecache/db/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/src/pybiocfilecache/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/temp.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:07.161129 pyBiocFileCache-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:07.165129 pyBiocFileCache-0.2.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/tests/data/test1.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/tests/data/test2.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-05 17:42:15.000000 pyBiocFileCache-0.2.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:25:47.055834 pybiocfilecache-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:25:47.043834 pybiocfilecache-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:25:47.047834 pybiocfilecache-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-05 16:25:47.055834 pybiocfilecache-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:25:47.051834 pybiocfilecache-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:25:47.051834 pybiocfilecache-0.3.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10327 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-05 16:25:47.055834 pybiocfilecache-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:25:47.043834 pybiocfilecache-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:25:47.055834 pybiocfilecache-0.3.0/src/pyBiocFileCache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-05 16:25:47.000000 pybiocfilecache-0.3.0/src/pyBiocFileCache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-05 16:25:47.000000 pybiocfilecache-0.3.0/src/pyBiocFileCache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 16:25:47.000000 pybiocfilecache-0.3.0/src/pyBiocFileCache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 16:25:12.000000 pybiocfilecache-0.3.0/src/pyBiocFileCache.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-05 16:25:47.000000 pybiocfilecache-0.3.0/src/pyBiocFileCache.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-05 16:25:47.000000 pybiocfilecache-0.3.0/src/pyBiocFileCache.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:25:47.051834 pybiocfilecache-0.3.0/src/pybiocfilecache/
+-rw-r--r--   0 runner    (1001) docker     (127)     8130 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/src/pybiocfilecache/BiocFileCache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/src/pybiocfilecache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/src/pybiocfilecache/_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:25:47.055834 pybiocfilecache-0.3.0/src/pybiocfilecache/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/src/pybiocfilecache/db/Base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/src/pybiocfilecache/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/src/pybiocfilecache/db/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/src/pybiocfilecache/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:25:47.055834 pybiocfilecache-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:25:47.055834 pybiocfilecache-0.3.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/tests/data/test1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/tests/data/test2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/tox.ini
```

### Comparing `pyBiocFileCache-0.2.2/.coveragerc` & `pybiocfilecache-0.3.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `pyBiocFileCache-0.2.2/.github/workflows/pypi-publish.yml` & `pybiocfilecache-0.3.0/.github/workflows/pypi-publish.yml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -44,8 +44,8 @@
     - name: Build Project and Publish
       run: |
         python -m tox -e clean,build
     - name: Publish package
       uses: pypa/gh-action-pypi-publish@27b31702a0e7fc50959f5ad993c78deac1bdfc29
       with:
         user: __token__
-        password: ${{ secrets.PYPI_PASSWORD }}
+        password: ${{ secrets.PYPI_PASSWORD }}
```

### Comparing `pyBiocFileCache-0.2.2/.github/workflows/pypi-test.yml` & `pybiocfilecache-0.3.0/.github/workflows/pypi-test.yml`

 * *Files 18% similar despite different names*

```diff
@@ -9,27 +9,32 @@
   pull_request:
     branches: [ main ]
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        python-version: [ '3.8', '3.9', '3.10', '3.11', '3.12' ]
 
+    name: Python ${{ matrix.python-version }}
     steps:
     - uses: actions/checkout@v2
-    - name: Set up Python 3.9
+    - name: Setup Python
       uses: actions/setup-python@v2
       with:
-        python-version: 3.9
+        python-version: ${{ matrix.python-version }}
+        cache: 'pip'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install flake8 pytest tox
     # - name: Lint with flake8
     #   run: |
     #     # stop the build if there are Python syntax errors or undefined names
     #     flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
     #     # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
     #     # flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
     - name: Test with tox
       run: |
-        tox
+        tox
```

### Comparing `pyBiocFileCache-0.2.2/.gitignore` & `pybiocfilecache-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyBiocFileCache-0.2.2/CONTRIBUTING.rst` & `pybiocfilecache-0.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyBiocFileCache-0.2.2/LICENSE.txt` & `pybiocfilecache-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyBiocFileCache-0.2.2/PKG-INFO` & `pybiocfilecache-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 Metadata-Version: 2.1
 Name: pyBiocFileCache
-Version: 0.2.2
+Version: 0.3.0
 Summary: File based cache for resources and metadata
 Home-page: https://github.com/epiviz/pyBiocFileCache
 Author: jkanche
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Provides-Extra: testing
 License-File: LICENSE.txt
 License-File: AUTHORS.md
+Requires-Dist: importlib-metadata; python_version < "3.8"
+Requires-Dist: sqlalchemy<2.1,>=2
+Provides-Extra: testing
+Requires-Dist: setuptools; extra == "testing"
+Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest-cov; extra == "testing"
+
+[![Project generated with PyScaffold](https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold)](https://pyscaffold.org/)
+[![PyPI-Server](https://img.shields.io/pypi/v/pyBiocFileCache.svg)](https://pypi.org/project/pyBiocFileCache/)
+![Unit tests](https://github.com/BiocPy/pyBiocFileCache/actions/workflows/pypi-test.yml/badge.svg)
 
 # pyBiocFileCache
 
 File system based cache for resources & metadata. Compatible with [BiocFileCache R package](https://github.com/Bioconductor/BiocFileCache)
 
 ***Note: Package is in development. Use with caution!!***
 
@@ -25,15 +34,15 @@
 
 Package is published to [PyPI](https://pypi.org/project/pyBiocFileCache/)
 
 ```
 pip install pybiocfilecache
 ```
 
-#### Initialize a cache directory 
+#### Initialize a cache directory
 
 ```
 from pybiocfilecache import BiocFileCache
 import os
 
 bfc = BiocFileCache(cache_dir = os.getcwd() + "/cache")
 ```
```

### Comparing `pyBiocFileCache-0.2.2/README.md` & `pybiocfilecache-0.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+[![Project generated with PyScaffold](https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold)](https://pyscaffold.org/)
+[![PyPI-Server](https://img.shields.io/pypi/v/pyBiocFileCache.svg)](https://pypi.org/project/pyBiocFileCache/)
+![Unit tests](https://github.com/BiocPy/pyBiocFileCache/actions/workflows/pypi-test.yml/badge.svg)
+
 # pyBiocFileCache
 
 File system based cache for resources & metadata. Compatible with [BiocFileCache R package](https://github.com/Bioconductor/BiocFileCache)
 
 ***Note: Package is in development. Use with caution!!***
 
 ### Installation
 
 Package is published to [PyPI](https://pypi.org/project/pyBiocFileCache/)
 
 ```
 pip install pybiocfilecache
 ```
 
-#### Initialize a cache directory 
+#### Initialize a cache directory
 
 ```
 from pybiocfilecache import BiocFileCache
 import os
 
 bfc = BiocFileCache(cache_dir = os.getcwd() + "/cache")
 ```
```

### Comparing `pyBiocFileCache-0.2.2/docs/Makefile` & `pybiocfilecache-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyBiocFileCache-0.2.2/docs/conf.py` & `pybiocfilecache-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyBiocFileCache-0.2.2/docs/index.md` & `pybiocfilecache-0.3.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `pyBiocFileCache-0.2.2/docs/readme.md` & `pybiocfilecache-0.3.0/docs/readme.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+[![Project generated with PyScaffold](https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold)](https://pyscaffold.org/)
+[![PyPI-Server](https://img.shields.io/pypi/v/pyBiocFileCache.svg)](https://pypi.org/project/pyBiocFileCache/)
+![Unit tests](https://github.com/BiocPy/pyBiocFileCache/actions/workflows/pypi-test.yml/badge.svg)
+
 # pyBiocFileCache
 
 File system based cache for resources & metadata. Compatible with [BiocFileCache R package](https://github.com/Bioconductor/BiocFileCache)
 
 ***Note: Package is in development. Use with caution!!***
 
 ### Installation
 
 Package is published to [PyPI](https://pypi.org/project/pyBiocFileCache/)
 
 ```
 pip install pybiocfilecache
 ```
 
-#### Initialize a cache directory 
+#### Initialize a cache directory
 
 ```
 from pybiocfilecache import BiocFileCache
 import os
 
 bfc = BiocFileCache(cache_dir = os.getcwd() + "/cache")
 ```
```

### Comparing `pyBiocFileCache-0.2.2/setup.cfg` & `pybiocfilecache-0.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 install_requires = 
 	importlib-metadata; python_version<"3.8"
-	sqlalchemy>=1.4,<2.0
+	sqlalchemy>=2,<2.1
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
```

### Comparing `pyBiocFileCache-0.2.2/setup.py` & `pybiocfilecache-0.3.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-"""
-    Setup file for pyBiocFileCache.
-    Use setup.cfg to configure your project.
+"""Setup file for pyBiocFileCache. Use setup.cfg to configure your project.
 
-    This file was generated with PyScaffold 4.1.
-    PyScaffold helps you to put up the scaffold of your new Python project.
-    Learn more under: https://pyscaffold.org/
+This file was generated with PyScaffold 4.1.
+PyScaffold helps you to put up the scaffold of your new Python project.
+Learn more under: https://pyscaffold.org/
 """
+
 from setuptools import setup
 
 if __name__ == "__main__":
     try:
         setup(use_scm_version={"version_scheme": "no-guess-dev"})
     except:  # noqa
         print(
```

### Comparing `pyBiocFileCache-0.2.2/src/pyBiocFileCache.egg-info/PKG-INFO` & `pybiocfilecache-0.3.0/src/pyBiocFileCache.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 Metadata-Version: 2.1
 Name: pyBiocFileCache
-Version: 0.2.2
+Version: 0.3.0
 Summary: File based cache for resources and metadata
 Home-page: https://github.com/epiviz/pyBiocFileCache
 Author: jkanche
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Provides-Extra: testing
 License-File: LICENSE.txt
 License-File: AUTHORS.md
+Requires-Dist: importlib-metadata; python_version < "3.8"
+Requires-Dist: sqlalchemy<2.1,>=2
+Provides-Extra: testing
+Requires-Dist: setuptools; extra == "testing"
+Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest-cov; extra == "testing"
+
+[![Project generated with PyScaffold](https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold)](https://pyscaffold.org/)
+[![PyPI-Server](https://img.shields.io/pypi/v/pyBiocFileCache.svg)](https://pypi.org/project/pyBiocFileCache/)
+![Unit tests](https://github.com/BiocPy/pyBiocFileCache/actions/workflows/pypi-test.yml/badge.svg)
 
 # pyBiocFileCache
 
 File system based cache for resources & metadata. Compatible with [BiocFileCache R package](https://github.com/Bioconductor/BiocFileCache)
 
 ***Note: Package is in development. Use with caution!!***
 
@@ -25,15 +34,15 @@
 
 Package is published to [PyPI](https://pypi.org/project/pyBiocFileCache/)
 
 ```
 pip install pybiocfilecache
 ```
 
-#### Initialize a cache directory 
+#### Initialize a cache directory
 
 ```
 from pybiocfilecache import BiocFileCache
 import os
 
 bfc = BiocFileCache(cache_dir = os.getcwd() + "/cache")
 ```
```

### Comparing `pyBiocFileCache-0.2.2/src/pyBiocFileCache.egg-info/SOURCES.txt` & `pybiocfilecache-0.3.0/src/pyBiocFileCache.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 .coveragerc
 .gitignore
+.pre-commit-config.yaml
 .readthedocs.yml
 AUTHORS.md
 CHANGELOG.md
 CONTRIBUTING.rst
 LICENSE.txt
 README.md
 pyproject.toml
 setup.cfg
 setup.py
-temp.txt
 tox.ini
 .github/workflows/pypi-publish.yml
 .github/workflows/pypi-test.yml
 docs/Makefile
 docs/authors.md
 docs/changelog.md
 docs/conf.py
```

### Comparing `pyBiocFileCache-0.2.2/src/pybiocfilecache/BiocFileCache.py` & `pybiocfilecache-0.3.0/src/pybiocfilecache/BiocFileCache.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Python Implementation of BiocFileCache
-"""
+"""Python Implementation of BiocFileCache."""
 
 import os
 from pathlib import Path
 from time import sleep, time
 from typing import List, Optional, Union
 
 from sqlalchemy import func
@@ -17,17 +15,15 @@
 
 __author__ = "jkanche"
 __copyright__ = "jkanche"
 __license__ = "MIT"
 
 
 class BiocFileCache:
-    """
-    Class to manage and cache files.
-    """
+    """Class to manage and cache files."""
 
     def __init__(self, cacheDirOrPath: Union[str, Path] = create_tmp_dir()):
         """Initialize BiocFileCache.
 
         Args:
             cacheDirOrPath (Union[str, Path], optional): Path to cache.
                 directory. Defaults to tmp location, `create_tmp_dir()`.
@@ -86,15 +82,21 @@
             raise NoFpathError(f"Resource at {fpath} does not exist.")
 
         rid = generate_id()
         rpath = f"{self.cache}/{rid}" + (f".{fpath.suffix}" if ext else "")
 
         # create new record in the database
         res = Resource(
-            **dict(rid=rid, rname=rname, rpath=rpath, rtype=rtype, fpath=str(fpath),)
+            **dict(
+                rid=rid,
+                rname=rname,
+                rpath=rpath,
+                rtype=rtype,
+                fpath=str(fpath),
+            )
         )
 
         # If this was higher up a parallel process could have added the key to
         # the cache in the meantime as the above takes a bit, so checking here
         # reduces the odds of this happening
         # Redirecting to update was removed as it is a scenario better handled
         # by the caller.
@@ -160,15 +162,15 @@
                         f"after {timeout} seconds."
                     )
                 sleep(0.1)
 
         return resource
 
     def get(self, rname: str) -> Optional[Resource]:
-        """get resource by name from cache.
+        """Get resource by name from cache.
 
         Args:
             rname (str): Name of the file to search.
 
         Returns:
             Optional[Resource]: matched resource from cache if exists.
         """
```

### Comparing `pyBiocFileCache-0.2.2/src/pybiocfilecache/__init__.py` & `pybiocfilecache-0.3.0/src/pybiocfilecache/__init__.py`

 * *Files identical despite different names*

### Comparing `pyBiocFileCache-0.2.2/src/pybiocfilecache/db/Base.py` & `pybiocfilecache-0.3.0/src/pybiocfilecache/db/Base.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 __copyright__ = "jkanche"
 __license__ = "MIT"
 
 Base = declarative_base()
 
 
 def create_schema(cache_dir: str) -> Tuple[Engine, sessionmaker]:
-    """Create the schema in the sqlite database
+    """Create the schema in the sqlite database.
 
     Args:
         cache_dir (str): Location where the cache directory
 
     Returns:
         a tuple of sqlalchemy engine and session maker
     """
```

### Comparing `pyBiocFileCache-0.2.2/src/pybiocfilecache/db/schema.py` & `pybiocfilecache-0.3.0/src/pybiocfilecache/db/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,8 +29,7 @@
     fpath = Column(String())
     last_modified_time = Column(DateTime, onupdate=func.now())
     etag = Column(String())
     expires = Column(DateTime)
 
     def __repr__(self):
         return "<Resource(id='%s', rname='%s')>" % (self.id, self.rname)
-
```

### Comparing `pyBiocFileCache-0.2.2/src/pybiocfilecache/utils.py` & `pybiocfilecache-0.3.0/src/pybiocfilecache/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from typing import Union
 import logging
 import sys
 
 
 def create_tmp_dir() -> str:
-    """create a temporary directory.
+    """Create a temporary directory.
 
     Returns:
         str: path to the directory
     """
     return tempfile.mkdtemp()
 
 
@@ -53,15 +53,15 @@
     except Exception as e:
         raise Exception(
             f"Error storing resource: '{rname}' from: '{source}' in '{target}'",
         ) from e
 
 
 def setup_logging(loglevel):
-    """Setup basic logging
+    """Setup basic logging.
 
     Args:
       loglevel (int): minimum loglevel for emitting messages
     """
     logformat = "[%(asctime)s] %(levelname)s:%(name)s:%(message)s"
     logging.basicConfig(
         level=loglevel, stream=sys.stdout, format=logformat, datefmt="%Y-%m-%d %H:%M:%S"
```

### Comparing `pyBiocFileCache-0.2.2/tests/test_cache.py` & `pybiocfilecache-0.3.0/tests/test_cache.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,54 @@
 import os
-import shutil
 
 from pybiocfilecache.BiocFileCache import BiocFileCache
 
 __author__ = "jkanche"
 __copyright__ = "jkanche"
 __license__ = "MIT"
 
 CACHE_DIR = os.getcwd() + "/cache"
 
 
 def test_create_cache():
     bfc = BiocFileCache(CACHE_DIR)
-    assert os.path.exists(CACHE_DIR == True)
+    assert os.path.exists(CACHE_DIR)
 
     bfc.purge()
 
 
 def test_add_get_operations():
     bfc = BiocFileCache(CACHE_DIR)
 
     bfc.add("test1", os.getcwd() + "/tests/data/test1.txt")
     rec1 = bfc.get("test1")
-    assert rec1 != None
+    assert rec1 is not None
 
     bfc.add("test2", os.getcwd() + "/tests/data/test2.txt")
     rec2 = bfc.get("test2")
-    assert rec2 != None
+    assert rec2 is not None
 
-    frec1 = open(rec1.rpath, "r").read()
+    frec1 = open(rec1.rpath, "r").read().strip()
     assert frec1 == "test1"
 
-    frec2 = open(rec2.rpath, "r").read()
+    frec2 = open(rec2.rpath, "r").read().strip()
     assert frec2 == "test2"
 
     bfc.purge()
 
 
 def test_remove_operations():
     bfc = BiocFileCache(CACHE_DIR)
 
     bfc.add("test1", os.getcwd() + "/tests/data/test1.txt")
     rec1 = bfc.get("test1")
-    assert rec1 != None
+    assert rec1 is not None
 
     bfc.add("test2", os.getcwd() + "/tests/data/test2.txt")
     rec2 = bfc.get("test2")
-    assert rec2 != None
+    assert rec2 is not None
 
     bfc.remove("test1")
     rec1 = bfc.get("test1")
-    assert rec1 == None
+    assert rec1 is None
 
     bfc.purge()
```

### Comparing `pyBiocFileCache-0.2.2/tox.ini` & `pybiocfilecache-0.3.0/tox.ini`

 * *Files identical despite different names*

