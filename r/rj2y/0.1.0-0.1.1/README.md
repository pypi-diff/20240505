# Comparing `tmp/rj2y-0.1.0.tar.gz` & `tmp/rj2y-0.1.1.tar.gz`

## Comparing `rj2y-0.1.0.tar` & `rj2y-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 rj2y-0.1.0/.python-version
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 rj2y-0.1.0/Makefile
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 rj2y-0.1.0/requirements-dev.lock
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 rj2y-0.1.0/requirements.lock
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 rj2y-0.1.0/tmp.json
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 rj2y-0.1.0/tmp.yaml
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 rj2y-0.1.0/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rj2y-0.1.0/src/rj2y/__init__.py
--rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 rj2y-0.1.0/src/rj2y/main.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 rj2y-0.1.0/tests/unittest/test_main.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 rj2y-0.1.0/.gitignore
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 rj2y-0.1.0/README.md
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 rj2y-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 rj2y-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 rj2y-0.1.1/.python-version
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 rj2y-0.1.1/Makefile
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 rj2y-0.1.1/requirements-dev.lock
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 rj2y-0.1.1/requirements.lock
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 rj2y-0.1.1/tmp.json
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 rj2y-0.1.1/tmp.yaml
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 rj2y-0.1.1/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rj2y-0.1.1/src/rj2y/__init__.py
+-rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 rj2y-0.1.1/src/rj2y/main.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 rj2y-0.1.1/tests/unittest/test_main.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 rj2y-0.1.1/.gitignore
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 rj2y-0.1.1/README.md
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 rj2y-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 rj2y-0.1.1/PKG-INFO
```

### Comparing `rj2y-0.1.0/tmp.json` & `rj2y-0.1.1/tmp.json`

 * *Files identical despite different names*

### Comparing `rj2y-0.1.0/tmp.yaml` & `rj2y-0.1.1/tmp.yaml`

 * *Files identical despite different names*

### Comparing `rj2y-0.1.0/src/rj2y/main.py` & `rj2y-0.1.1/src/rj2y/main.py`

 * *Files identical despite different names*

### Comparing `rj2y-0.1.0/tests/unittest/test_main.py` & `rj2y-0.1.1/tests/unittest/test_main.py`

 * *Files identical despite different names*

### Comparing `rj2y-0.1.0/pyproject.toml` & `rj2y-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rj2y"
-version = "0.1.0"
+version = "0.1.1"
 description = "Recursively convert JSON including json-string to YAML"
 authors = [{ name = "pollenjp", email = "polleninjp@gmail.com" }]
 dependencies = ["click>=8.1.7"]
 readme = "README.md"
 requires-python = ">= 3.10"
 classifiers = [
     "Development Status :: 1 - Planning",
```

