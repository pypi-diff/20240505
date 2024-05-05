# Comparing `tmp/fewerai-2.0.0.tar.gz` & `tmp/fewerai-3.0.0.tar.gz`

## Comparing `fewerai-2.0.0.tar` & `fewerai-3.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 fewerai-2.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 fewerai-2.0.0/src/fewerai/__init__.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 fewerai-2.0.0/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 fewerai-2.0.0/LICENSE
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 fewerai-2.0.0/README.md
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 fewerai-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 fewerai-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 fewerai-3.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     5609 2020-02-02 00:00:00.000000 fewerai-3.0.0/src/fewerai/__init__.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 fewerai-3.0.0/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 fewerai-3.0.0/LICENSE
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 fewerai-3.0.0/README.md
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 fewerai-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 fewerai-3.0.0/PKG-INFO
```

### Comparing `fewerai-2.0.0/.github/workflows/python-publish.yml` & `fewerai-3.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fewerai-2.0.0/LICENSE` & `fewerai-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fewerai-2.0.0/pyproject.toml` & `fewerai-3.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "requests"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fewerai"
-version = "2.0.0"
+version = "3.0.0"
 authors = [
   { name="FewerElk", email="fewerelk@gmail.com" },
 ]
 description = "A simple ai"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `fewerai-2.0.0/PKG-INFO` & `fewerai-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fewerai
-Version: 2.0.0
+Version: 3.0.0
 Summary: A simple ai
 Project-URL: Homepage, https://github.com/FewerElk/FewerAI
 Project-URL: Issues, https://github.com/FewerElk/FewerAI/issues
 Author-email: FewerElk <fewerelk@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

