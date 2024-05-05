# Comparing `tmp/inspyre_toolbox-1.4.3.tar.gz` & `tmp/inspyre_toolbox-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inspyre_toolbox-1.4.3.tar", max compression
+gzip compressed data, was "inspyre_toolbox-1.5.0.tar", max compression
```

## Comparing `inspyre_toolbox-1.4.3.tar` & `inspyre_toolbox-1.5.0.tar`

### file list

```diff
@@ -1,41 +1,45 @@
--rw-r--r--   0        0        0      209 2024-04-30 20:45:10.403940 inspyre_toolbox-1.4.3/inspyre_toolbox/__about__.py
--rw-r--r--   0        0        0     2639 2024-04-30 20:44:59.194115 inspyre_toolbox-1.4.3/inspyre_toolbox/__init__.py
--rw-r--r--   0        0        0       16 2024-04-30 20:45:10.403940 inspyre_toolbox-1.4.3/inspyre_toolbox/api_changes.ini
--rw-r--r--   0        0        0        0 2024-04-30 20:45:10.405306 inspyre_toolbox-1.4.3/inspyre_toolbox/cli/__init__.py
--rw-r--r--   0        0        0     3005 2024-04-30 20:45:10.405306 inspyre_toolbox-1.4.3/inspyre_toolbox/cli/ist_bytes_converter/__init__.py
--rw-r--r--   0        0        0     3388 2024-04-30 20:45:10.405306 inspyre_toolbox-1.4.3/inspyre_toolbox/cli/ist_bytes_converter/arguments.py
--rw-r--r--   0        0        0     1425 2024-04-30 20:45:10.406705 inspyre_toolbox-1.4.3/inspyre_toolbox/cli/ist_bytes_converter/helpers.py
--rw-r--r--   0        0        0        0 2024-04-30 20:45:10.406705 inspyre_toolbox-1.4.3/inspyre_toolbox/common/__init__.py
--rw-r--r--   0        0        0      931 2024-05-02 23:40:50.594372 inspyre_toolbox-1.4.3/inspyre_toolbox/common/meta.py
--rw-r--r--   0        0        0     2808 2024-04-30 20:44:59.194115 inspyre_toolbox-1.4.3/inspyre_toolbox/console_kit/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 20:44:59.195113 inspyre_toolbox-1.4.3/inspyre_toolbox/conversions/__init__.py
--rw-r--r--   0        0        0     4240 2024-04-30 20:45:10.407939 inspyre_toolbox-1.4.3/inspyre_toolbox/conversions/bytes/__init__.py
--rw-r--r--   0        0        0     5299 2024-04-30 20:45:10.407939 inspyre_toolbox-1.4.3/inspyre_toolbox/conversions/roman_numerals/__init__.py
--rw-r--r--   0        0        0     1143 2024-04-30 20:44:59.196112 inspyre_toolbox-1.4.3/inspyre_toolbox/conversions/roman_numerals/errors.py
--rw-r--r--   0        0        0        0 2024-04-30 20:44:59.196112 inspyre_toolbox-1.4.3/inspyre_toolbox/core/errors/__init__.py
--rw-r--r--   0        0        0     2636 2024-04-30 20:44:59.196112 inspyre_toolbox-1.4.3/inspyre_toolbox/core/errors/version.py
--rw-r--r--   0        0        0       97 2024-04-30 20:44:59.197472 inspyre_toolbox-1.4.3/inspyre_toolbox/core_helpers/__init__.py
--rw-r--r--   0        0        0      424 2024-04-30 20:44:59.197472 inspyre_toolbox-1.4.3/inspyre_toolbox/core_helpers/debugging.py
--rw-r--r--   0        0        0     4065 2024-04-30 20:45:10.409300 inspyre_toolbox-1.4.3/inspyre_toolbox/core_helpers/logging.py
--rw-r--r--   0        0        0     1951 2024-04-30 20:45:10.409300 inspyre_toolbox-1.4.3/inspyre_toolbox/docs/conversions/bytes.md
--rw-r--r--   0        0        0     3413 2024-04-30 20:45:10.410790 inspyre_toolbox-1.4.3/inspyre_toolbox/generations/__init__.py
--rw-r--r--   0        0        0    22944 2024-04-30 20:45:10.410790 inspyre_toolbox-1.4.3/inspyre_toolbox/humanize/__init__.py
--rw-r--r--   0        0        0      262 2024-04-30 20:44:59.198686 inspyre_toolbox-1.4.3/inspyre_toolbox/humanize/errors/__init__.py
--rw-r--r--   0        0        0     1927 2024-04-30 20:44:59.199745 inspyre_toolbox-1.4.3/inspyre_toolbox/humanize/errors/numerical.py
--rw-r--r--   0        0        0    10359 2024-05-02 22:55:50.816773 inspyre_toolbox-1.4.3/inspyre_toolbox/live_timer/__init__.py
--rw-r--r--   0        0        0     1100 2024-04-30 20:44:59.200756 inspyre_toolbox-1.4.3/inspyre_toolbox/live_timer/errors.py
--rw-r--r--   0        0        0     2596 2024-05-02 22:30:57.895734 inspyre_toolbox-1.4.3/inspyre_toolbox/live_timer/history.py
--rw-r--r--   0        0        0    11458 2024-04-30 20:45:10.412229 inspyre_toolbox-1.4.3/inspyre_toolbox/proc_man/__init__.py
--rw-r--r--   0        0        0      689 2024-04-30 20:44:59.202755 inspyre_toolbox-1.4.3/inspyre_toolbox/proc_man/errors.py
--rw-r--r--   0        0        0        0 2024-04-30 20:44:59.202755 inspyre_toolbox-1.4.3/inspyre_toolbox/pypi/__init__.py
--rw-r--r--   0        0        0      900 2024-04-30 20:44:59.203757 inspyre_toolbox-1.4.3/inspyre_toolbox/pypi/packages.py
--rw-r--r--   0        0        0      596 2024-04-30 20:44:59.203757 inspyre_toolbox-1.4.3/inspyre_toolbox/settings.py
--rw-r--r--   0        0        0     1868 2024-04-30 20:45:10.412229 inspyre_toolbox-1.4.3/inspyre_toolbox/solve_kit/__init__.py
--rw-r--r--   0        0        0      175 2024-04-30 20:44:59.204758 inspyre_toolbox-1.4.3/inspyre_toolbox/spanners/__init__.py
--rw-r--r--   0        0        0     2210 2024-04-30 20:44:59.204758 inspyre_toolbox-1.4.3/inspyre_toolbox/spanners/span_arg_parse.py
--rw-r--r--   0        0        0     1014 2024-04-30 20:44:59.204758 inspyre_toolbox-1.4.3/inspyre_toolbox/syntactic_sweets/__init__.py
--rw-r--r--   0        0        0     2265 2024-04-30 20:44:59.205757 inspyre_toolbox-1.4.3/inspyre_toolbox/sys_man/__init__.py
--rw-r--r--   0        0        0     6999 2024-04-30 20:45:10.413573 inspyre_toolbox-1.4.3/inspyre_toolbox/version.py
--rw-r--r--   0        0        0     1122 2024-04-30 20:45:10.401205 inspyre_toolbox-1.4.3/LICENSE
--rw-r--r--   0        0        0     1637 2024-05-02 23:39:08.529283 inspyre_toolbox-1.4.3/pyproject.toml
--rw-r--r--   0        0        0     1552 1970-01-01 00:00:00.000000 inspyre_toolbox-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0      209 2024-04-30 20:45:10.403940 inspyre_toolbox-1.5.0/inspyre_toolbox/__about__.py
+-rw-r--r--   0        0        0     2639 2024-04-30 20:44:59.194115 inspyre_toolbox-1.5.0/inspyre_toolbox/__init__.py
+-rw-r--r--   0        0        0       16 2024-04-30 20:45:10.403940 inspyre_toolbox-1.5.0/inspyre_toolbox/api_changes.ini
+-rw-r--r--   0        0        0        0 2024-04-30 20:45:10.405306 inspyre_toolbox-1.5.0/inspyre_toolbox/cli/__init__.py
+-rw-r--r--   0        0        0     3005 2024-04-30 20:45:10.405306 inspyre_toolbox-1.5.0/inspyre_toolbox/cli/ist_bytes_converter/__init__.py
+-rw-r--r--   0        0        0     3388 2024-04-30 20:45:10.405306 inspyre_toolbox-1.5.0/inspyre_toolbox/cli/ist_bytes_converter/arguments.py
+-rw-r--r--   0        0        0     1425 2024-04-30 20:45:10.406705 inspyre_toolbox-1.5.0/inspyre_toolbox/cli/ist_bytes_converter/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:45:10.406705 inspyre_toolbox-1.5.0/inspyre_toolbox/common/__init__.py
+-rw-r--r--   0        0        0      931 2024-05-04 23:02:20.270738 inspyre_toolbox-1.5.0/inspyre_toolbox/common/meta.py
+-rw-r--r--   0        0        0     2808 2024-04-30 20:44:59.194115 inspyre_toolbox-1.5.0/inspyre_toolbox/console_kit/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:44:59.195113 inspyre_toolbox-1.5.0/inspyre_toolbox/conversions/__init__.py
+-rw-r--r--   0        0        0     4240 2024-04-30 20:45:10.407939 inspyre_toolbox-1.5.0/inspyre_toolbox/conversions/bytes/__init__.py
+-rw-r--r--   0        0        0     5299 2024-04-30 20:45:10.407939 inspyre_toolbox-1.5.0/inspyre_toolbox/conversions/roman_numerals/__init__.py
+-rw-r--r--   0        0        0     1143 2024-04-30 20:44:59.196112 inspyre_toolbox-1.5.0/inspyre_toolbox/conversions/roman_numerals/errors.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:44:59.196112 inspyre_toolbox-1.5.0/inspyre_toolbox/core/errors/__init__.py
+-rw-r--r--   0        0        0     2636 2024-04-30 20:44:59.196112 inspyre_toolbox-1.5.0/inspyre_toolbox/core/errors/version.py
+-rw-r--r--   0        0        0       97 2024-04-30 20:44:59.197472 inspyre_toolbox-1.5.0/inspyre_toolbox/core_helpers/__init__.py
+-rw-r--r--   0        0        0      424 2024-04-30 20:44:59.197472 inspyre_toolbox-1.5.0/inspyre_toolbox/core_helpers/debugging.py
+-rw-r--r--   0        0        0     4065 2024-04-30 20:45:10.409300 inspyre_toolbox-1.5.0/inspyre_toolbox/core_helpers/logging.py
+-rw-r--r--   0        0        0     1951 2024-04-30 20:45:10.409300 inspyre_toolbox-1.5.0/inspyre_toolbox/docs/conversions/bytes.md
+-rw-r--r--   0        0        0     3413 2024-04-30 20:45:10.410790 inspyre_toolbox-1.5.0/inspyre_toolbox/generations/__init__.py
+-rw-r--r--   0        0        0    22944 2024-04-30 20:45:10.410790 inspyre_toolbox-1.5.0/inspyre_toolbox/humanize/__init__.py
+-rw-r--r--   0        0        0      262 2024-04-30 20:44:59.198686 inspyre_toolbox-1.5.0/inspyre_toolbox/humanize/errors/__init__.py
+-rw-r--r--   0        0        0     1927 2024-04-30 20:44:59.199745 inspyre_toolbox-1.5.0/inspyre_toolbox/humanize/errors/numerical.py
+-rw-r--r--   0        0        0    10359 2024-05-02 22:55:50.816773 inspyre_toolbox-1.5.0/inspyre_toolbox/live_timer/__init__.py
+-rw-r--r--   0        0        0     1100 2024-04-30 20:44:59.200756 inspyre_toolbox-1.5.0/inspyre_toolbox/live_timer/errors.py
+-rw-r--r--   0        0        0     2596 2024-05-02 22:30:57.895734 inspyre_toolbox-1.5.0/inspyre_toolbox/live_timer/history.py
+-rw-r--r--   0        0        0    11458 2024-04-30 20:45:10.412229 inspyre_toolbox-1.5.0/inspyre_toolbox/proc_man/__init__.py
+-rw-r--r--   0        0        0      689 2024-04-30 20:44:59.202755 inspyre_toolbox-1.5.0/inspyre_toolbox/proc_man/errors.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:44:59.202755 inspyre_toolbox-1.5.0/inspyre_toolbox/pypi/__init__.py
+-rw-r--r--   0        0        0      900 2024-04-30 20:44:59.203757 inspyre_toolbox-1.5.0/inspyre_toolbox/pypi/packages.py
+-rw-r--r--   0        0        0      596 2024-04-30 20:44:59.203757 inspyre_toolbox-1.5.0/inspyre_toolbox/settings.py
+-rw-r--r--   0        0        0     1868 2024-04-30 20:45:10.412229 inspyre_toolbox-1.5.0/inspyre_toolbox/solve_kit/__init__.py
+-rw-r--r--   0        0        0      175 2024-04-30 20:44:59.204758 inspyre_toolbox-1.5.0/inspyre_toolbox/spanners/__init__.py
+-rw-r--r--   0        0        0     2210 2024-04-30 20:44:59.204758 inspyre_toolbox-1.5.0/inspyre_toolbox/spanners/span_arg_parse.py
+-rw-r--r--   0        0        0     1014 2024-04-30 20:44:59.204758 inspyre_toolbox-1.5.0/inspyre_toolbox/syntactic_sweets/__init__.py
+-rw-r--r--   0        0        0      269 2024-05-05 01:23:41.221040 inspyre_toolbox-1.5.0/inspyre_toolbox/syntactic_sweets/properties/__init__.py
+-rw-r--r--   0        0        0     5849 2024-05-05 01:23:41.212036 inspyre_toolbox-1.5.0/inspyre_toolbox/syntactic_sweets/properties/decorators.py
+-rw-r--r--   0        0        0     9502 2024-05-05 01:23:41.216040 inspyre_toolbox-1.5.0/inspyre_toolbox/syntactic_sweets/properties/descriptors/__init__.py
+-rw-r--r--   0        0        0      425 2024-05-05 01:23:41.226038 inspyre_toolbox-1.5.0/inspyre_toolbox/syntactic_sweets/properties/descriptors/errors.py
+-rw-r--r--   0        0        0     2265 2024-04-30 20:44:59.205757 inspyre_toolbox-1.5.0/inspyre_toolbox/sys_man/__init__.py
+-rw-r--r--   0        0        0     6999 2024-04-30 20:45:10.413573 inspyre_toolbox-1.5.0/inspyre_toolbox/version.py
+-rw-r--r--   0        0        0     1122 2024-04-30 20:45:10.401205 inspyre_toolbox-1.5.0/LICENSE
+-rw-r--r--   0        0        0     1636 2024-05-05 13:09:32.419337 inspyre_toolbox-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1545 1970-01-01 00:00:00.000000 inspyre_toolbox-1.5.0/PKG-INFO
```

### Comparing `inspyre_toolbox-1.4.3/inspyre_toolbox/__init__.py` & `inspyre_toolbox-1.5.0/inspyre_toolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.3/inspyre_toolbox/cli/ist_bytes_converter/__init__.py` & `inspyre_toolbox-1.5.0/inspyre_toolbox/cli/ist_bytes_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.3/inspyre_toolbox/cli/ist_bytes_converter/arguments.py` & `inspyre_toolbox-1.5.0/inspyre_toolbox/cli/ist_bytes_converter/arguments.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.3/inspyre_toolbox/cli/ist_bytes_converter/helpers.py` & `inspyre_toolbox-1.5.0/inspyre_toolbox/cli/ist_bytes_converter/helpers.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.3/inspyre_toolbox/common/meta.py` & `inspyre_toolbox-1.5.0/inspyre_toolbox/common/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,13 +30,13 @@
     'final': 'Final Release Build'
 }
 """The release map for the project."""
 
 
 VERSION = {
     'major': 1,
-    'minor': 4,
-    'patch': 3,
+    'minor': 5,
+    'patch': 0,
     'release': 'final',
     'release_num': 0
 }
 """The version information for the project."""
```

### Comparing `inspyre_toolbox-1.4.3/inspyre_toolbox/console_kit/__init__.py` & `inspyre_toolbox-1.5.0/inspyre_toolbox/console_kit/__init__.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.3/inspyre_toolbox/conversions/bytes/__init__.py` & `inspyre_toolbox-1.5.0/inspyre_toolbox/conversions/bytes/__init__.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.3/inspyre_toolbox/conversions/roman_numerals/__init__.py` & `inspyre_toolbox-1.5.0/inspyre_toolbox/conversions/roman_numerals/__init__.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.3/inspyre_toolbox/conversions/roman_numerals/errors.py` & `inspyre_toolbox-1.5.0/inspyre_toolbox/conversions/roman_numerals/errors.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.3/inspyre_toolbox/core/errors/version.py` & `inspyre_toolbox-1.5.0/inspyre_toolbox/core/errors/version.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.3/inspyre_toolbox/core_helpers/logging.py` & `inspyre_toolbox-1.5.0/inspyre_toolbox/core_helpers/logging.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.3/inspyre_toolbox/docs/conversions/bytes.md` & `inspyre_toolbox-1.5.0/inspyre_toolbox/docs/conversions/bytes.md`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.3/inspyre_toolbox/generations/__init__.py` & `inspyre_toolbox-1.5.0/inspyre_toolbox/generations/__init__.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.3/inspyre_toolbox/humanize/__init__.py` & `inspyre_toolbox-1.5.0/inspyre_toolbox/humanize/__init__.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.3/inspyre_toolbox/humanize/errors/numerical.py` & `inspyre_toolbox-1.5.0/inspyre_toolbox/humanize/errors/numerical.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.3/inspyre_toolbox/live_timer/__init__.py` & `inspyre_toolbox-1.5.0/inspyre_toolbox/live_timer/__init__.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.3/inspyre_toolbox/live_timer/errors.py` & `inspyre_toolbox-1.5.0/inspyre_toolbox/live_timer/errors.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.3/inspyre_toolbox/live_timer/history.py` & `inspyre_toolbox-1.5.0/inspyre_toolbox/live_timer/history.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.3/inspyre_toolbox/proc_man/__init__.py` & `inspyre_toolbox-1.5.0/inspyre_toolbox/proc_man/__init__.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.3/inspyre_toolbox/proc_man/errors.py` & `inspyre_toolbox-1.5.0/inspyre_toolbox/proc_man/errors.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.3/inspyre_toolbox/pypi/packages.py` & `inspyre_toolbox-1.5.0/inspyre_toolbox/pypi/packages.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.3/inspyre_toolbox/settings.py` & `inspyre_toolbox-1.5.0/inspyre_toolbox/settings.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.3/inspyre_toolbox/solve_kit/__init__.py` & `inspyre_toolbox-1.5.0/inspyre_toolbox/solve_kit/__init__.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.3/inspyre_toolbox/spanners/span_arg_parse.py` & `inspyre_toolbox-1.5.0/inspyre_toolbox/spanners/span_arg_parse.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.3/inspyre_toolbox/syntactic_sweets/__init__.py` & `inspyre_toolbox-1.5.0/inspyre_toolbox/syntactic_sweets/__init__.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.3/inspyre_toolbox/sys_man/__init__.py` & `inspyre_toolbox-1.5.0/inspyre_toolbox/sys_man/__init__.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.3/inspyre_toolbox/version.py` & `inspyre_toolbox-1.5.0/inspyre_toolbox/version.py`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.3/LICENSE` & `inspyre_toolbox-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inspyre_toolbox-1.4.3/pyproject.toml` & `inspyre_toolbox-1.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "inspyre-toolbox"
-version = "v1.4.3"
+version = "v1.5.0"
 description = "A toolbox containing some useful tools for Inspyre Softworks packages. Generally useful to some programmers too."
 authors = [ "T Blackstone <t.blackstone@inspyre.tech>",]
 license = "MIT"
 classifiers = [ "Intended Audience :: Developers", "License :: OSI Approved :: MIT License", "Natural Language :: English", "Operating System :: OS Independent", "Programming Language :: Python :: 3", "Programming Language :: Python :: 3.6", "Programming Language :: Python :: 3.7", "Programming Language :: Python :: 3.8", "Programming Language :: Python :: 3.9", "Programming Language :: Python :: 3 :: Only", "Topic :: Scientific/Engineering :: Mathematics", "Topic :: Software Development", "Topic :: Software Development :: Build Tools", "Topic :: Software Development :: Libraries :: Python Modules", "Topic :: Terminals", "Topic :: Utilities",]
 keywords = [ "toolbox", "timer", "commify", "strings", "elapsed",]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 inflect = "^5.3.0"
 psutil = "^5.8.0"
 DateTime = "^4.3"
 pypattyrn = "^1.2"
 tqdm = "^4.64.0"
 inspyred-print = "^1.2.1"
-inspy-logger = "^3.1.0.dev4"
+inspy-logger = "3.1.0-dev4"
 
 [tool.poetry.scripts]
 ist-bytes-converter = "inspyre_toolbox.cli.ist_bytes_converter:main"
 
 [tool.poetry.group.dev.dependencies]
 ptipython = "^1.0.1"
 prompt-toolkit = "^3.0.43"
```

### Comparing `inspyre_toolbox-1.4.3/PKG-INFO` & `inspyre_toolbox-1.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspyre-toolbox
-Version: 1.4.3
+Version: 1.5.0
 Summary: A toolbox containing some useful tools for Inspyre Softworks packages. Generally useful to some programmers too.
 License: MIT
 Keywords: toolbox,timer,commify,strings,elapsed
 Author: T Blackstone
 Author-email: t.blackstone@inspyre.tech
 Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Developers
@@ -24,12 +24,12 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Terminals
 Classifier: Topic :: Utilities
 Requires-Dist: DateTime (>=4.3,<5.0)
 Requires-Dist: inflect (>=5.3.0,<6.0.0)
-Requires-Dist: inspy-logger (>=3.1.0.dev4,<4.0.0)
+Requires-Dist: inspy-logger (==3.1.0-dev4)
 Requires-Dist: inspyred-print (>=1.2.1,<2.0.0)
 Requires-Dist: psutil (>=5.8.0,<6.0.0)
 Requires-Dist: pypattyrn (>=1.2,<2.0)
 Requires-Dist: tqdm (>=4.64.0,<5.0.0)
```

