# Comparing `tmp/fnug-0.0.8.tar.gz` & `tmp/fnug-0.0.9.tar.gz`

## Comparing `fnug-0.0.8.tar` & `fnug-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fnug-0.0.8/.fnug.yaml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 fnug-0.0.8/.python-version
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 fnug-0.0.8/requirements-dev.lock
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 fnug-0.0.8/requirements.lock
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 fnug-0.0.8/src/fnug/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fnug-0.0.8/src/fnug/__main__.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 fnug-0.0.8/src/fnug/cli.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 fnug-0.0.8/src/fnug/config.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 fnug-0.0.8/src/fnug/git.py
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 fnug-0.0.8/src/fnug/terminal_emulator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fnug-0.0.8/src/fnug/ui/__init__.py
--rw-r--r--   0        0        0     6243 2020-02-02 00:00:00.000000 fnug-0.0.8/src/fnug/ui/app.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 fnug-0.0.8/src/fnug/ui/app.tcss
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fnug-0.0.8/src/fnug/ui/components/__init__.py
--rw-r--r--   0        0        0    13535 2020-02-02 00:00:00.000000 fnug-0.0.8/src/fnug/ui/components/lint_tree.py
--rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 fnug-0.0.8/src/fnug/ui/components/terminal.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fnug-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 fnug-0.0.8/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 fnug-0.0.8/LICENSE
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 fnug-0.0.8/README.md
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 fnug-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 fnug-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 fnug-0.0.9/.fnug.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 fnug-0.0.9/.python-version
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 fnug-0.0.9/requirements-dev.lock
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 fnug-0.0.9/requirements.lock
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 fnug-0.0.9/src/fnug/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fnug-0.0.9/src/fnug/__main__.py
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 fnug-0.0.9/src/fnug/cli.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 fnug-0.0.9/src/fnug/config.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 fnug-0.0.9/src/fnug/git.py
+-rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 fnug-0.0.9/src/fnug/terminal_emulator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fnug-0.0.9/src/fnug/ui/__init__.py
+-rw-r--r--   0        0        0     6243 2020-02-02 00:00:00.000000 fnug-0.0.9/src/fnug/ui/app.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 fnug-0.0.9/src/fnug/ui/app.tcss
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fnug-0.0.9/src/fnug/ui/components/__init__.py
+-rw-r--r--   0        0        0    13535 2020-02-02 00:00:00.000000 fnug-0.0.9/src/fnug/ui/components/lint_tree.py
+-rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 fnug-0.0.9/src/fnug/ui/components/terminal.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fnug-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 fnug-0.0.9/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 fnug-0.0.9/LICENSE
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 fnug-0.0.9/README.md
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 fnug-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 fnug-0.0.9/PKG-INFO
```

### Comparing `fnug-0.0.8/.fnug.yaml` & `fnug-0.0.9/.fnug.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -12,17 +12,17 @@
         cmd: rye run black .
       - name: pyright
         cmd: rye run pyright src
       - name: ruff
         cmd: rye run ruff --fix src
   - name: fnug-test
     commands:
-      - name: test
-        cmd: cat src/fnug/terminal_emulator.py
-      - name: A very very very long name
+      - name: htop
+        cmd: htop
+      - name: A very very very long file
         autorun: true
         cmd: cat src/fnug/terminal_emulator.py ; cat src/fnug/terminal_emulator.py ; cat
           src/fnug/terminal_emulator.py
     children:
       - name: fnug-test-2
         commands:
           - name: test
```

### Comparing `fnug-0.0.8/requirements-dev.lock` & `fnug-0.0.9/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `fnug-0.0.8/src/fnug/cli.py` & `fnug-0.0.9/src/fnug/cli.py`

 * *Files identical despite different names*

### Comparing `fnug-0.0.8/src/fnug/config.py` & `fnug-0.0.9/src/fnug/config.py`

 * *Files identical despite different names*

### Comparing `fnug-0.0.8/src/fnug/git.py` & `fnug-0.0.9/src/fnug/git.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 import subprocess
 from functools import cache
 from pathlib import Path
 
 
 @cache
 def _git_status(repo_path: Path, sub_path: Path | None = None) -> list[str]:
+    absolute_repo_path = repo_path.resolve()
     cmd = [
         "git",
         "-C",
-        repo_path.as_posix(),
+        absolute_repo_path.as_posix(),
         "status",
         "--porcelain=v1",
     ]
 
     if sub_path:
         cmd.append(sub_path.as_posix())
```

### Comparing `fnug-0.0.8/src/fnug/terminal_emulator.py` & `fnug-0.0.9/src/fnug/terminal_emulator.py`

 * *Files identical despite different names*

### Comparing `fnug-0.0.8/src/fnug/ui/app.py` & `fnug-0.0.9/src/fnug/ui/app.py`

 * *Files identical despite different names*

### Comparing `fnug-0.0.8/src/fnug/ui/app.tcss` & `fnug-0.0.9/src/fnug/ui/app.tcss`

 * *Files identical despite different names*

### Comparing `fnug-0.0.8/src/fnug/ui/components/lint_tree.py` & `fnug-0.0.9/src/fnug/ui/components/lint_tree.py`

 * *Files identical despite different names*

### Comparing `fnug-0.0.8/src/fnug/ui/components/terminal.py` & `fnug-0.0.9/src/fnug/ui/components/terminal.py`

 * *Files identical despite different names*

### Comparing `fnug-0.0.8/.gitignore` & `fnug-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `fnug-0.0.8/LICENSE` & `fnug-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fnug-0.0.8/pyproject.toml` & `fnug-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fnug"
-version = "0.0.8"
+version = "0.0.9"
 description = "A nice lint runner"
 authors = [
     { name = "Nickolaj Jepsen", email = "nickolaj@fireproof.website" }
 ]
 dependencies = [
     "click>=8.1.7",
     "textual>=0.40.0",
```

### Comparing `fnug-0.0.8/PKG-INFO` & `fnug-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnug
-Version: 0.0.8
+Version: 0.0.9
 Summary: A nice lint runner
 Project-URL: Repository, https://github.com/nickolaj-jepsen/fnug.git
 Project-URL: Issues, https://github.com/nickolaj-jepsen/fnug/issues
 Author-email: Nickolaj Jepsen <nickolaj@fireproof.website>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
 Requires-Python: >=3.11
```

