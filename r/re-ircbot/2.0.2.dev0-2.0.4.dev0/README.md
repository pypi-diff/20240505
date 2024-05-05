# Comparing `tmp/re_ircbot-2.0.2.dev0.tar.gz` & `tmp/re_ircbot-2.0.4.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "re_ircbot-2.0.2.dev0.tar", last modified: Sat May  4 23:20:17 2024, max compression
+gzip compressed data, was "re_ircbot-2.0.4.dev0.tar", last modified: Sat May  4 23:48:39 2024, max compression
```

## Comparing `re_ircbot-2.0.2.dev0.tar` & `re_ircbot-2.0.4.dev0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-04 23:20:17.808748 re_ircbot-2.0.2.dev0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1072 2024-05-04 23:20:09.000000 re_ircbot-2.0.2.dev0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14099 2024-05-04 23:20:17.808748 re_ircbot-2.0.2.dev0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13331 2024-05-04 23:20:09.000000 re_ircbot-2.0.2.dev0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-04 23:20:17.804748 re_ircbot-2.0.2.dev0/ircbot/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      125 2024-05-04 23:20:09.000000 re_ircbot-2.0.2.dev0/ircbot/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    53399 2024-05-04 23:20:09.000000 re_ircbot-2.0.2.dev0/ircbot/client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5384 2024-05-04 23:20:09.000000 re_ircbot-2.0.2.dev0/ircbot/dcc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17833 2024-05-04 23:20:09.000000 re_ircbot-2.0.2.dev0/ircbot/hooks.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3039 2024-05-04 23:20:09.000000 re_ircbot-2.0.2.dev0/ircbot/message.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1972 2024-05-04 23:20:09.000000 re_ircbot-2.0.2.dev0/ircbot/shortest_prefix.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11380 2024-05-04 23:20:09.000000 re_ircbot-2.0.2.dev0/ircbot/sqlitedb.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1426 2024-05-04 23:20:09.000000 re_ircbot-2.0.2.dev0/ircbot/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-04 23:20:17.808748 re_ircbot-2.0.2.dev0/re_ircbot.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14099 2024-05-04 23:20:17.000000 re_ircbot-2.0.2.dev0/re_ircbot.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      335 2024-05-04 23:20:17.000000 re_ircbot-2.0.2.dev0/re_ircbot.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-04 23:20:17.000000 re_ircbot-2.0.2.dev0/re_ircbot.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2024-05-04 23:20:17.000000 re_ircbot-2.0.2.dev0/re_ircbot.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-05-04 23:20:17.000000 re_ircbot-2.0.2.dev0/re_ircbot.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-04 23:20:17.808748 re_ircbot-2.0.2.dev0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1869 2024-05-04 23:20:09.000000 re_ircbot-2.0.2.dev0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-04 23:48:39.752266 re_ircbot-2.0.4.dev0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1072 2024-05-04 23:48:32.000000 re_ircbot-2.0.4.dev0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14099 2024-05-04 23:48:39.752266 re_ircbot-2.0.4.dev0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13331 2024-05-04 23:48:32.000000 re_ircbot-2.0.4.dev0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-04 23:48:39.752266 re_ircbot-2.0.4.dev0/ircbot/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      125 2024-05-04 23:48:33.000000 re_ircbot-2.0.4.dev0/ircbot/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    53399 2024-05-04 23:48:33.000000 re_ircbot-2.0.4.dev0/ircbot/client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5384 2024-05-04 23:48:33.000000 re_ircbot-2.0.4.dev0/ircbot/dcc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17845 2024-05-04 23:48:33.000000 re_ircbot-2.0.4.dev0/ircbot/hooks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3039 2024-05-04 23:48:33.000000 re_ircbot-2.0.4.dev0/ircbot/message.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1972 2024-05-04 23:48:33.000000 re_ircbot-2.0.4.dev0/ircbot/shortest_prefix.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11380 2024-05-04 23:48:33.000000 re_ircbot-2.0.4.dev0/ircbot/sqlitedb.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1426 2024-05-04 23:48:33.000000 re_ircbot-2.0.4.dev0/ircbot/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-04 23:48:39.752266 re_ircbot-2.0.4.dev0/re_ircbot.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14099 2024-05-04 23:48:39.000000 re_ircbot-2.0.4.dev0/re_ircbot.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      335 2024-05-04 23:48:39.000000 re_ircbot-2.0.4.dev0/re_ircbot.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-04 23:48:39.000000 re_ircbot-2.0.4.dev0/re_ircbot.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2024-05-04 23:48:39.000000 re_ircbot-2.0.4.dev0/re_ircbot.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-05-04 23:48:39.000000 re_ircbot-2.0.4.dev0/re_ircbot.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-04 23:48:39.752266 re_ircbot-2.0.4.dev0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1869 2024-05-04 23:48:33.000000 re_ircbot-2.0.4.dev0/setup.py
```

### Comparing `re_ircbot-2.0.2.dev0/LICENSE` & `re_ircbot-2.0.4.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.2.dev0/PKG-INFO` & `re_ircbot-2.0.4.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re-ircbot
-Version: 2.0.2.dev0
+Version: 2.0.4.dev0
 Summary: A simple async irc bot framework with regex command definitions and data permanency
 Home-page: https://github.com/matheusfillipe/ircbot
 Author: Matheus Fillipe
 Author-email: mattf@tilde.club
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `re_ircbot-2.0.2.dev0/README.md` & `re_ircbot-2.0.4.dev0/README.md`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.2.dev0/ircbot/client.py` & `re_ircbot-2.0.4.dev0/ircbot/client.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.2.dev0/ircbot/dcc.py` & `re_ircbot-2.0.4.dev0/ircbot/dcc.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.2.dev0/ircbot/hooks.py` & `re_ircbot-2.0.4.dev0/ircbot/hooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
     _command_max_arguments: int = 25
 
     simplify_arg_commands: bool = True
 
     def re_command(self, cmd, acccept_pms=True, pass_data=False, **kwargs):
         non_space: str = r"\S"
         return self.regex_cmd_with_messsage(
-            f"^{self.command_prefix}{cmd}{f'(?: +({non_space}+))?'*self._command_max_arguments} *$",
+            rf"^{re.escape(self.command_prefix)}{cmd}{f'(?: +({non_space}+))?'*self._command_max_arguments} *$",
             acccept_pms,
             pass_data,
             **kwargs,
         )
 
     def set_simplify_commands(self, simplify: bool) -> Self:
         self.simplify_arg_commands = simplify
```

### Comparing `re_ircbot-2.0.2.dev0/ircbot/message.py` & `re_ircbot-2.0.4.dev0/ircbot/message.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.2.dev0/ircbot/shortest_prefix.py` & `re_ircbot-2.0.4.dev0/ircbot/shortest_prefix.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.2.dev0/ircbot/sqlitedb.py` & `re_ircbot-2.0.4.dev0/ircbot/sqlitedb.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.2.dev0/ircbot/utils.py` & `re_ircbot-2.0.4.dev0/ircbot/utils.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.2.dev0/re_ircbot.egg-info/PKG-INFO` & `re_ircbot-2.0.4.dev0/re_ircbot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re-ircbot
-Version: 2.0.2.dev0
+Version: 2.0.4.dev0
 Summary: A simple async irc bot framework with regex command definitions and data permanency
 Home-page: https://github.com/matheusfillipe/ircbot
 Author: Matheus Fillipe
 Author-email: mattf@tilde.club
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `re_ircbot-2.0.2.dev0/setup.py` & `re_ircbot-2.0.4.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 import subprocess
 
 import setuptools
 
-VERSION = "2.0.2-dev"
+VERSION = "2.0.4-dev"
 BRANCH = "v2"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 def requirements():
```

