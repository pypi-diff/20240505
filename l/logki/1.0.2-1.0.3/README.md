# Comparing `tmp/logki-1.0.2.tar.gz` & `tmp/logki-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logki-1.0.2.tar", last modified: Sat Apr 20 13:52:53 2024, max compression
+gzip compressed data, was "logki-1.0.3.tar", last modified: Sun May  5 10:18:21 2024, max compression
```

## Comparing `logki-1.0.2.tar` & `logki-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:52:53.444033 logki-1.0.2/
--rwxr-xr-x   0 runner    (1001) docker     (127)      403 2024-04-20 13:52:35.000000 logki-1.0.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-20 13:52:35.000000 logki-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    46122 2024-04-20 13:52:53.444033 logki-1.0.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     4485 2024-04-20 13:52:35.000000 logki-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:52:53.440033 logki-1.0.2/logki/
--rwxr-xr-x   0 runner    (1001) docker     (127)      147 2024-04-20 13:52:35.000000 logki-1.0.2/logki/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13923 2024-04-20 13:52:35.000000 logki-1.0.2/logki/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:52:53.444033 logki-1.0.2/logki.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    46122 2024-04-20 13:52:53.000000 logki-1.0.2/logki.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-20 13:52:53.000000 logki-1.0.2/logki.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 13:52:53.000000 logki-1.0.2/logki.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-20 13:52:53.000000 logki-1.0.2/logki.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-20 13:52:53.000000 logki-1.0.2/logki.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-20 13:52:53.000000 logki-1.0.2/logki.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     2173 2024-04-20 13:52:35.000000 logki-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 13:52:53.444033 logki-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:52:53.444033 logki-1.0.2/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)      616 2024-04-20 13:52:35.000000 logki-1.0.2/tests/test_logki.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:18:21.977562 logki-1.0.3/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      403 2024-05-05 10:17:51.000000 logki-1.0.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-05 10:17:51.000000 logki-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    46122 2024-05-05 10:18:21.977562 logki-1.0.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4485 2024-05-05 10:17:51.000000 logki-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:18:21.973562 logki-1.0.3/logki/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      147 2024-05-05 10:17:51.000000 logki-1.0.3/logki/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7892 2024-05-05 10:17:51.000000 logki-1.0.3/logki/app.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5725 2024-05-05 10:17:51.000000 logki-1.0.3/logki/logic.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3808 2024-05-05 10:17:51.000000 logki-1.0.3/logki/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:18:21.977562 logki-1.0.3/logki.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    46122 2024-05-05 10:18:21.000000 logki-1.0.3/logki.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-05 10:18:21.000000 logki-1.0.3/logki.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 10:18:21.000000 logki-1.0.3/logki.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-05 10:18:21.000000 logki-1.0.3/logki.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-05 10:18:21.000000 logki-1.0.3/logki.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-05 10:18:21.000000 logki-1.0.3/logki.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2173 2024-05-05 10:17:51.000000 logki-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 10:18:21.977562 logki-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:18:21.977562 logki-1.0.3/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      694 2024-05-05 10:17:51.000000 logki-1.0.3/tests/test_logki.py
```

### Comparing `logki-1.0.2/LICENSE` & `logki-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `logki-1.0.2/PKG-INFO` & `logki-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logki
-Version: 1.0.2
+Version: 1.0.3
 Summary: logki: Log Analysis Kit
 Author-email: Tomas Fiedor <TomasFiedor@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `logki-1.0.2/README.md` & `logki-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `logki-1.0.2/logki.egg-info/PKG-INFO` & `logki-1.0.3/logki.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logki
-Version: 1.0.2
+Version: 1.0.3
 Summary: logki: Log Analysis Kit
 Author-email: Tomas Fiedor <TomasFiedor@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `logki-1.0.2/pyproject.toml` & `logki-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     # Other
     "prompt_toolkit>=3.0.43",
 
     # Plotting / visualization / output
     "tabulate>=0.9",
 ]
-version = "1.0.2"
+version = "1.0.3"
 
 [project.optional-dependencies]
 docs = [
     # Sphinx 7.2 dropped support for Python 3.8
     "Sphinx>=7.1",
     "sphinx-click>=5.0",
 ]
```

### Comparing `logki-1.0.2/tests/test_logki.py` & `logki-1.0.3/tests/test_logki.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,20 +4,23 @@
 import os
 
 # Third-Party Imports
 from prompt_toolkit.input import create_pipe_input
 from prompt_toolkit.output import DummyOutput
 
 # Logki imports
-import logki.app as logki
+from logki import app
+from logki.utils import BufferedLog
 
 
 def test_app():
     with create_pipe_input() as pipe_input:
-        pipe_input.send_text('q\n')
-        with logki.BufferedLog(os.path.join(os.path.dirname(__file__), "workloads", "example.log")) as buffered_log:
-            app = logki.create_app(buffered_log)
-            app.input = pipe_input
-            app.output = DummyOutput()
+        pipe_input.send_text("q\n")
+        with BufferedLog(
+            os.path.join(os.path.dirname(__file__), "workloads", "example.log")
+        ) as buffered_log:
+            application = app.create_app(buffered_log)
+            application.input = pipe_input
+            application.output = DummyOutput()
 
             # Run the application
-            app.run()
+            application.run()
```

