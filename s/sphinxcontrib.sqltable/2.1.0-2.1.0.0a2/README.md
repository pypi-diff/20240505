# Comparing `tmp/sphinxcontrib_sqltable-2.1.0.tar.gz` & `tmp/sphinxcontrib_sqltable-2.1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib_sqltable-2.1.0.tar", last modified: Sun May  5 13:17:09 2024, max compression
+gzip compressed data, was "sphinxcontrib_sqltable-2.1.0.0a2.tar", last modified: Sun May  5 13:15:39 2024, max compression
```

## Comparing `sphinxcontrib_sqltable-2.1.0.tar` & `sphinxcontrib_sqltable-2.1.0.0a2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:17:09.759058 sphinxcontrib_sqltable-2.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:17:09.751058 sphinxcontrib_sqltable-2.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:17:09.755058 sphinxcontrib_sqltable-2.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-05 13:16:51.000000 sphinxcontrib_sqltable-2.1.0/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-05 13:16:51.000000 sphinxcontrib_sqltable-2.1.0/.github/workflows/python-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-05 13:16:51.000000 sphinxcontrib_sqltable-2.1.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-05 13:16:51.000000 sphinxcontrib_sqltable-2.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-05 13:16:51.000000 sphinxcontrib_sqltable-2.1.0/.hgignore
--rw-r--r--   0 runner    (1001) docker     (127)     8780 2024-05-05 13:16:51.000000 sphinxcontrib_sqltable-2.1.0/.hgtags
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-05 13:16:51.000000 sphinxcontrib_sqltable-2.1.0/.mergify.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-05 13:16:51.000000 sphinxcontrib_sqltable-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-05 13:16:51.000000 sphinxcontrib_sqltable-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-05 13:16:51.000000 sphinxcontrib_sqltable-2.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-05 13:17:09.759058 sphinxcontrib_sqltable-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-05 13:16:51.000000 sphinxcontrib_sqltable-2.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-05 13:16:51.000000 sphinxcontrib_sqltable-2.1.0/announce.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:17:09.755058 sphinxcontrib_sqltable-2.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-05 13:16:51.000000 sphinxcontrib_sqltable-2.1.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:17:09.755058 sphinxcontrib_sqltable-2.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 13:16:51.000000 sphinxcontrib_sqltable-2.1.0/docs/_static/.placeholder
--rw-r--r--   0 runner    (1001) docker     (127)     8544 2024-05-05 13:16:51.000000 sphinxcontrib_sqltable-2.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-05 13:16:51.000000 sphinxcontrib_sqltable-2.1.0/docs/customize.rst
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-05 13:16:51.000000 sphinxcontrib_sqltable-2.1.0/docs/developers.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-05 13:16:51.000000 sphinxcontrib_sqltable-2.1.0/docs/example.rst
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-05 13:16:51.000000 sphinxcontrib_sqltable-2.1.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-05 13:16:51.000000 sphinxcontrib_sqltable-2.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-05 13:16:51.000000 sphinxcontrib_sqltable-2.1.0/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-05 13:16:51.000000 sphinxcontrib_sqltable-2.1.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-05 13:16:51.000000 sphinxcontrib_sqltable-2.1.0/docs/sampledata.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-05 13:16:51.000000 sphinxcontrib_sqltable-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-05 13:16:51.000000 sphinxcontrib_sqltable-2.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 13:17:09.759058 sphinxcontrib_sqltable-2.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:17:09.755058 sphinxcontrib_sqltable-2.1.0/sphinxcontrib/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-05 13:16:51.000000 sphinxcontrib_sqltable-2.1.0/sphinxcontrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-05-05 13:16:51.000000 sphinxcontrib_sqltable-2.1.0/sphinxcontrib/sqltable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:17:09.759058 sphinxcontrib_sqltable-2.1.0/sphinxcontrib.sqltable.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-05 13:17:09.000000 sphinxcontrib_sqltable-2.1.0/sphinxcontrib.sqltable.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-05 13:17:09.000000 sphinxcontrib_sqltable-2.1.0/sphinxcontrib.sqltable.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 13:17:09.000000 sphinxcontrib_sqltable-2.1.0/sphinxcontrib.sqltable.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-05 13:17:09.000000 sphinxcontrib_sqltable-2.1.0/sphinxcontrib.sqltable.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-05 13:17:09.000000 sphinxcontrib_sqltable-2.1.0/sphinxcontrib.sqltable.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-05 13:16:51.000000 sphinxcontrib_sqltable-2.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:15:39.286709 sphinxcontrib_sqltable-2.1.0.0a2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:15:39.278709 sphinxcontrib_sqltable-2.1.0.0a2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:15:39.282709 sphinxcontrib_sqltable-2.1.0.0a2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/.github/workflows/python-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/.hgignore
+-rw-r--r--   0 runner    (1001) docker     (127)     8780 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/.hgtags
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/.mergify.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-05-05 13:15:39.286709 sphinxcontrib_sqltable-2.1.0.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/announce.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:15:39.282709 sphinxcontrib_sqltable-2.1.0.0a2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:15:39.286709 sphinxcontrib_sqltable-2.1.0.0a2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/docs/_static/.placeholder
+-rw-r--r--   0 runner    (1001) docker     (127)     8544 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/docs/customize.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/docs/developers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/docs/example.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/docs/sampledata.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 13:15:39.286709 sphinxcontrib_sqltable-2.1.0.0a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:15:39.286709 sphinxcontrib_sqltable-2.1.0.0a2/sphinxcontrib/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/sphinxcontrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/sphinxcontrib/sqltable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:15:39.286709 sphinxcontrib_sqltable-2.1.0.0a2/sphinxcontrib.sqltable.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-05-05 13:15:39.000000 sphinxcontrib_sqltable-2.1.0.0a2/sphinxcontrib.sqltable.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-05 13:15:39.000000 sphinxcontrib_sqltable-2.1.0.0a2/sphinxcontrib.sqltable.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 13:15:39.000000 sphinxcontrib_sqltable-2.1.0.0a2/sphinxcontrib.sqltable.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-05 13:15:39.000000 sphinxcontrib_sqltable-2.1.0.0a2/sphinxcontrib.sqltable.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-05 13:15:39.000000 sphinxcontrib_sqltable-2.1.0.0a2/sphinxcontrib.sqltable.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/tox.ini
```

### Comparing `sphinxcontrib_sqltable-2.1.0/.github/workflows/check.yml` & `sphinxcontrib_sqltable-2.1.0.0a2/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_sqltable-2.1.0/.github/workflows/python-publish.yaml` & `sphinxcontrib_sqltable-2.1.0.0a2/.github/workflows/python-publish.yaml`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_sqltable-2.1.0/.github/workflows/test.yml` & `sphinxcontrib_sqltable-2.1.0.0a2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_sqltable-2.1.0/.hgtags` & `sphinxcontrib_sqltable-2.1.0.0a2/.hgtags`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_sqltable-2.1.0/.mergify.yml` & `sphinxcontrib_sqltable-2.1.0.0a2/.mergify.yml`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_sqltable-2.1.0/LICENSE` & `sphinxcontrib_sqltable-2.1.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_sqltable-2.1.0/Makefile` & `sphinxcontrib_sqltable-2.1.0.0a2/Makefile`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_sqltable-2.1.0/PKG-INFO` & `sphinxcontrib_sqltable-2.1.0.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib.sqltable
-Version: 2.1.0
+Version: 2.1.0.0a2
 Summary: Sphinx extension for embedding database content in documents
 Author-email: Doug Hellmann <doug@doughellmann.com>
 Project-URL: homepage, https://sphinxcontrib-sqltable.readthedocs.io/en/latest/
 Project-URL: repository, http://github.com/sphinx-contrib/sqltable
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

### Comparing `sphinxcontrib_sqltable-2.1.0/README.rst` & `sphinxcontrib_sqltable-2.1.0.0a2/README.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_sqltable-2.1.0/announce.rst` & `sphinxcontrib_sqltable-2.1.0.0a2/announce.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_sqltable-2.1.0/docs/Makefile` & `sphinxcontrib_sqltable-2.1.0.0a2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_sqltable-2.1.0/docs/conf.py` & `sphinxcontrib_sqltable-2.1.0.0a2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_sqltable-2.1.0/docs/customize.rst` & `sphinxcontrib_sqltable-2.1.0.0a2/docs/customize.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_sqltable-2.1.0/docs/developers.rst` & `sphinxcontrib_sqltable-2.1.0.0a2/docs/developers.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_sqltable-2.1.0/docs/example.rst` & `sphinxcontrib_sqltable-2.1.0.0a2/docs/example.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_sqltable-2.1.0/docs/index.rst` & `sphinxcontrib_sqltable-2.1.0.0a2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_sqltable-2.1.0/docs/install.rst` & `sphinxcontrib_sqltable-2.1.0.0a2/docs/install.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_sqltable-2.1.0/pyproject.toml` & `sphinxcontrib_sqltable-2.1.0.0a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_sqltable-2.1.0/sphinxcontrib/sqltable.py` & `sphinxcontrib_sqltable-2.1.0.0a2/sphinxcontrib/sqltable.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_sqltable-2.1.0/sphinxcontrib.sqltable.egg-info/PKG-INFO` & `sphinxcontrib_sqltable-2.1.0.0a2/sphinxcontrib.sqltable.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib.sqltable
-Version: 2.1.0
+Version: 2.1.0.0a2
 Summary: Sphinx extension for embedding database content in documents
 Author-email: Doug Hellmann <doug@doughellmann.com>
 Project-URL: homepage, https://sphinxcontrib-sqltable.readthedocs.io/en/latest/
 Project-URL: repository, http://github.com/sphinx-contrib/sqltable
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

### Comparing `sphinxcontrib_sqltable-2.1.0/sphinxcontrib.sqltable.egg-info/SOURCES.txt` & `sphinxcontrib_sqltable-2.1.0.0a2/sphinxcontrib.sqltable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_sqltable-2.1.0/tox.ini` & `sphinxcontrib_sqltable-2.1.0.0a2/tox.ini`

 * *Files identical despite different names*

