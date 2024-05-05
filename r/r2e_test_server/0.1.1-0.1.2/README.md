# Comparing `tmp/r2e_test_server-0.1.1.tar.gz` & `tmp/r2e_test_server-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r2e_test_server-0.1.1.tar", max compression
+gzip compressed data, was "r2e_test_server-0.1.2.tar", max compression
```

## Comparing `r2e_test_server-0.1.1.tar` & `r2e_test_server-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1060 2024-04-27 00:14:08.782149 r2e_test_server-0.1.1/LICENSE
--rw-r--r--   0        0        0     1020 2024-05-02 05:33:55.087500 r2e_test_server-0.1.1/README.md
--rw-r--r--   0        0        0      601 2024-05-04 20:58:53.322507 r2e_test_server-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-28 05:56:33.718445 r2e_test_server-0.1.1/r2e_test_server/ast/__init__.py
--rw-r--r--   0        0        0     3062 2024-04-29 00:05:15.445367 r2e_test_server-0.1.1/r2e_test_server/ast/transformer.py
--rw-r--r--   0        0        0      757 2024-04-29 00:05:15.445367 r2e_test_server-0.1.1/r2e_test_server/cli.py
--rw-r--r--   0        0        0      130 2024-04-29 00:05:15.445367 r2e_test_server-0.1.1/r2e_test_server/instrument/__init__.py
--rw-r--r--   0        0        0     7431 2024-05-04 20:52:36.474257 r2e_test_server-0.1.1/r2e_test_server/instrument/arguments.py
--rw-r--r--   0        0        0     1824 2024-04-29 00:05:15.445367 r2e_test_server-0.1.1/r2e_test_server/instrument/base.py
--rw-r--r--   0        0        0        0 2024-04-28 05:56:33.718445 r2e_test_server-0.1.1/r2e_test_server/modules/__init__.py
--rw-r--r--   0        0        0     4767 2024-04-28 05:56:33.718445 r2e_test_server-0.1.1/r2e_test_server/modules/explorer.py
--rw-r--r--   0        0        0     4286 2024-05-04 20:52:36.474257 r2e_test_server-0.1.1/r2e_test_server/server.py
--rw-r--r--   0        0        0     2094 2024-04-28 05:56:33.718445 r2e_test_server-0.1.1/r2e_test_server/testing/cleaner.py
--rw-r--r--   0        0        0     5052 2024-04-29 00:05:15.445367 r2e_test_server-0.1.1/r2e_test_server/testing/codecov.py
--rw-r--r--   0        0        0     2466 2024-04-29 00:05:15.445367 r2e_test_server-0.1.1/r2e_test_server/testing/loader.py
--rw-r--r--   0        0        0     9549 2024-05-04 20:52:36.474257 r2e_test_server-0.1.1/r2e_test_server/testing/r2e_testprogram.py
--rw-r--r--   0        0        0     2947 2024-04-28 05:56:33.718445 r2e_test_server-0.1.1/r2e_test_server/testing/result.py
--rw-r--r--   0        0        0      354 2024-04-28 05:56:33.718445 r2e_test_server-0.1.1/r2e_test_server/testing/runner.py
--rw-r--r--   0        0        0     1839 1970-01-01 00:00:00.000000 r2e_test_server-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-04-27 00:14:08.782149 r2e_test_server-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1020 2024-05-02 05:33:55.087500 r2e_test_server-0.1.2/README.md
+-rw-r--r--   0        0        0      601 2024-05-05 04:10:44.880094 r2e_test_server-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-28 05:56:33.718445 r2e_test_server-0.1.2/r2e_test_server/ast/__init__.py
+-rw-r--r--   0        0        0     3062 2024-04-29 00:05:15.445367 r2e_test_server-0.1.2/r2e_test_server/ast/transformer.py
+-rw-r--r--   0        0        0      757 2024-04-29 00:05:15.445367 r2e_test_server-0.1.2/r2e_test_server/cli.py
+-rw-r--r--   0        0        0      130 2024-04-29 00:05:15.445367 r2e_test_server-0.1.2/r2e_test_server/instrument/__init__.py
+-rw-r--r--   0        0        0     7431 2024-05-04 20:52:36.474257 r2e_test_server-0.1.2/r2e_test_server/instrument/arguments.py
+-rw-r--r--   0        0        0     1824 2024-04-29 00:05:15.445367 r2e_test_server-0.1.2/r2e_test_server/instrument/base.py
+-rw-r--r--   0        0        0        0 2024-04-28 05:56:33.718445 r2e_test_server-0.1.2/r2e_test_server/modules/__init__.py
+-rw-r--r--   0        0        0     4767 2024-04-28 05:56:33.718445 r2e_test_server-0.1.2/r2e_test_server/modules/explorer.py
+-rw-r--r--   0        0        0     4286 2024-05-04 20:52:36.474257 r2e_test_server-0.1.2/r2e_test_server/server.py
+-rw-r--r--   0        0        0     2094 2024-04-28 05:56:33.718445 r2e_test_server-0.1.2/r2e_test_server/testing/cleaner.py
+-rw-r--r--   0        0        0     5052 2024-04-29 00:05:15.445367 r2e_test_server-0.1.2/r2e_test_server/testing/codecov.py
+-rw-r--r--   0        0        0     2466 2024-04-29 00:05:15.445367 r2e_test_server-0.1.2/r2e_test_server/testing/loader.py
+-rw-r--r--   0        0        0    10084 2024-05-05 04:10:38.948093 r2e_test_server-0.1.2/r2e_test_server/testing/r2e_testprogram.py
+-rw-r--r--   0        0        0     2947 2024-04-28 05:56:33.718445 r2e_test_server-0.1.2/r2e_test_server/testing/result.py
+-rw-r--r--   0        0        0      354 2024-04-28 05:56:33.718445 r2e_test_server-0.1.2/r2e_test_server/testing/runner.py
+-rw-r--r--   0        0        0     1839 1970-01-01 00:00:00.000000 r2e_test_server-0.1.2/PKG-INFO
```

### Comparing `r2e_test_server-0.1.1/LICENSE` & `r2e_test_server-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `r2e_test_server-0.1.1/README.md` & `r2e_test_server-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `r2e_test_server-0.1.1/pyproject.toml` & `r2e_test_server-0.1.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "r2e_test_server"
-version = "0.1.1"
+version = "0.1.2"
 description = "Test Server For R2E"
 authors = ["Naman Jain <naman_jain@berkeley.com>", "Manish Shetty <manishs@berkeley.edu>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/r2e-project/r2e-test-server"
 
 [tool.poetry.dependencies]
```

### Comparing `r2e_test_server-0.1.1/r2e_test_server/ast/transformer.py` & `r2e_test_server-0.1.2/r2e_test_server/ast/transformer.py`

 * *Files identical despite different names*

### Comparing `r2e_test_server-0.1.1/r2e_test_server/cli.py` & `r2e_test_server-0.1.2/r2e_test_server/cli.py`

 * *Files identical despite different names*

### Comparing `r2e_test_server-0.1.1/r2e_test_server/instrument/arguments.py` & `r2e_test_server-0.1.2/r2e_test_server/instrument/arguments.py`

 * *Files identical despite different names*

### Comparing `r2e_test_server-0.1.1/r2e_test_server/instrument/base.py` & `r2e_test_server-0.1.2/r2e_test_server/instrument/base.py`

 * *Files identical despite different names*

### Comparing `r2e_test_server-0.1.1/r2e_test_server/modules/explorer.py` & `r2e_test_server-0.1.2/r2e_test_server/modules/explorer.py`

 * *Files identical despite different names*

### Comparing `r2e_test_server-0.1.1/r2e_test_server/server.py` & `r2e_test_server-0.1.2/r2e_test_server/server.py`

 * *Files identical despite different names*

### Comparing `r2e_test_server-0.1.1/r2e_test_server/testing/cleaner.py` & `r2e_test_server-0.1.2/r2e_test_server/testing/cleaner.py`

 * *Files identical despite different names*

### Comparing `r2e_test_server-0.1.1/r2e_test_server/testing/codecov.py` & `r2e_test_server-0.1.2/r2e_test_server/testing/codecov.py`

 * *Files identical despite different names*

### Comparing `r2e_test_server-0.1.1/r2e_test_server/testing/loader.py` & `r2e_test_server-0.1.2/r2e_test_server/testing/loader.py`

 * *Files identical despite different names*

### Comparing `r2e_test_server-0.1.1/r2e_test_server/testing/r2e_testprogram.py` & `r2e_test_server-0.1.2/r2e_test_server/testing/r2e_testprogram.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import ast
 import sys
 import json
 import coverage
 import importlib
 import importlib.util
 from copy import deepcopy
@@ -30,22 +31,23 @@
         repo_id: str,
         repo_path: str,
         funclass_names: list[str],
         file_path: str,
         generated_tests: dict[str, str],
         codegen_mode: bool = False,
     ):
+        ## file_path should be relative to repo_path
         self.repo_id = repo_id
-        self.repo_path = f"/repos/{repo_id}"
+        self.repo_path = repo_path  # f"/repos/{repo_id}"
         self.funclass_names = funclass_names
-        self.file_path = file_path
+        self.file_path = os.path.join(self.repo_path, file_path)
         self.generated_tests = generated_tests
         self.codegen_mode = codegen_mode
 
-        with open(file_path, "r") as file:
+        with open(self.file_path, "r") as file:
             self.orig_file_content = file.read()
             self.orig_file_ast = ast.parse(self.orig_file_content)
 
         # setup the env for testing
         # creates: fut_module and fut_module_deps
         self.setupEnv()
 
@@ -212,21 +214,29 @@
             FUT (FunctionUnderTest): function under test.
 
         Returns:
             tuple[ModuleType, dict[str, Any]]: module and its dependencies.
         """
 
         try:
-            if self.repo_path not in sys.path:
-                sys.path.insert(0, self.repo_path)
+            all_repo_to_file_paths: list[str] = [self.repo_path]
+            curr_path = os.path.dirname(self.file_path)
+            while curr_path != self.repo_path:
+                all_repo_to_file_paths.append(curr_path)
+                curr_path = os.path.dirname(curr_path)
+
+            for repo_to_file_path in all_repo_to_file_paths:
+                if repo_to_file_path not in sys.path:
+                    sys.path.insert(0, repo_to_file_path)
 
             fut_module = self.import_module_dynamic("fut_module", self.file_path)
             fut_module_deps = ModuleExplorer.get_dependencies(self.file_path)
 
-            sys.path.remove(self.repo_path)
+            for repo_to_file_path in all_repo_to_file_paths:
+                sys.path.remove(repo_to_file_path)
         except ModuleNotFoundError as e:
             print(f"[ERROR] {str(e)}: Library not installed?")
             raise
         except Exception as e:
             print("[ERROR] Bug in the imported FUT module?")
             raise
```

### Comparing `r2e_test_server-0.1.1/r2e_test_server/testing/result.py` & `r2e_test_server-0.1.2/r2e_test_server/testing/result.py`

 * *Files identical despite different names*

### Comparing `r2e_test_server-0.1.1/PKG-INFO` & `r2e_test_server-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r2e_test_server
-Version: 0.1.1
+Version: 0.1.2
 Summary: Test Server For R2E
 Home-page: https://github.com/r2e-project/r2e-test-server
 License: MIT
 Author: Naman Jain
 Author-email: naman_jain@berkeley.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

