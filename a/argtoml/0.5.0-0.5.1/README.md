# Comparing `tmp/argtoml-0.5.0.tar.gz` & `tmp/argtoml-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argtoml-0.5.0.tar", last modified: Wed Apr 24 13:24:24 2024, max compression
+gzip compressed data, was "argtoml-0.5.1.tar", last modified: Sun May  5 16:25:20 2024, max compression
```

## Comparing `argtoml-0.5.0.tar` & `argtoml-0.5.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 gum       (1001) gum       (1001)        0 2024-04-24 13:24:24.796624 argtoml-0.5.0/
--rw-r--r--   0 gum       (1001) gum       (1001)     1069 2023-11-17 14:23:09.000000 argtoml-0.5.0/LICENSE
--rw-r--r--   0 gum       (1001) gum       (1001)     3731 2024-04-24 13:24:24.796624 argtoml-0.5.0/PKG-INFO
--rw-r--r--   0 gum       (1001) gum       (1001)     3218 2023-12-26 14:25:11.000000 argtoml-0.5.0/README.md
-drwxr-xr-x   0 gum       (1001) gum       (1001)        0 2024-04-24 13:24:24.796624 argtoml-0.5.0/argtoml/
--rw-r--r--   0 gum       (1001) gum       (1001)       57 2024-01-22 12:17:21.000000 argtoml-0.5.0/argtoml/__init__.py
--rw-r--r--   0 gum       (1001) gum       (1001)     2802 2024-02-18 11:46:36.000000 argtoml-0.5.0/argtoml/__main__.py
--rw-r--r--   0 gum       (1001) gum       (1001)     3076 2024-01-22 13:41:14.000000 argtoml-0.5.0/argtoml/locate.py
--rw-r--r--   0 gum       (1001) gum       (1001)    10953 2024-01-21 19:47:11.000000 argtoml-0.5.0/argtoml/main.py
--rw-r--r--   0 gum       (1001) gum       (1001)     4920 2024-01-22 15:05:51.000000 argtoml-0.5.0/argtoml/opt.py
-drwxr-xr-x   0 gum       (1001) gum       (1001)        0 2024-04-24 13:24:24.796624 argtoml-0.5.0/argtoml.egg-info/
--rw-r--r--   0 gum       (1001) gum       (1001)     3731 2024-04-24 13:24:24.000000 argtoml-0.5.0/argtoml.egg-info/PKG-INFO
--rw-r--r--   0 gum       (1001) gum       (1001)      273 2024-04-24 13:24:24.000000 argtoml-0.5.0/argtoml.egg-info/SOURCES.txt
--rw-r--r--   0 gum       (1001) gum       (1001)        1 2024-04-24 13:24:24.000000 argtoml-0.5.0/argtoml.egg-info/dependency_links.txt
--rw-r--r--   0 gum       (1001) gum       (1001)        8 2024-04-24 13:24:24.000000 argtoml-0.5.0/argtoml.egg-info/top_level.txt
--rw-r--r--   0 gum       (1001) gum       (1001)      951 2024-01-22 12:17:53.000000 argtoml-0.5.0/pyproject.toml
--rw-r--r--   0 gum       (1001) gum       (1001)       38 2024-04-24 13:24:24.796624 argtoml-0.5.0/setup.cfg
--rw-r--r--   0 gum       (1001) gum       (1001)       61 2023-11-17 14:23:09.000000 argtoml-0.5.0/setup.py
-drwxr-xr-x   0 gum       (1001) gum       (1001)        0 2024-04-24 13:24:24.796624 argtoml-0.5.0/tests/
--rw-r--r--   0 gum       (1001) gum       (1001)      218 2023-11-17 14:23:09.000000 argtoml-0.5.0/tests/test_main.py
+drwxr-xr-x   0 jo3       (1000) jo3       (1000)        0 2024-05-05 16:25:20.986922 argtoml-0.5.1/
+-rw-r--r--   0 jo3       (1000) jo3       (1000)     1069 2023-07-23 14:09:52.000000 argtoml-0.5.1/LICENSE
+-rw-r--r--   0 jo3       (1000) jo3       (1000)     3731 2024-05-05 16:25:20.986922 argtoml-0.5.1/PKG-INFO
+-rw-r--r--   0 jo3       (1000) jo3       (1000)     3218 2024-01-02 10:21:38.000000 argtoml-0.5.1/README.md
+drwxr-xr-x   0 jo3       (1000) jo3       (1000)        0 2024-05-05 16:25:20.986922 argtoml-0.5.1/argtoml/
+-rw-r--r--   0 jo3       (1000) jo3       (1000)       57 2024-02-13 08:37:22.000000 argtoml-0.5.1/argtoml/__init__.py
+-rw-r--r--   0 jo3       (1000) jo3       (1000)     2802 2024-02-18 11:11:25.000000 argtoml-0.5.1/argtoml/__main__.py
+-rw-r--r--   0 jo3       (1000) jo3       (1000)     3076 2024-02-13 08:37:22.000000 argtoml-0.5.1/argtoml/locate.py
+-rw-r--r--   0 jo3       (1000) jo3       (1000)    10953 2024-02-13 08:37:22.000000 argtoml-0.5.1/argtoml/main.py
+-rw-r--r--   0 jo3       (1000) jo3       (1000)     4948 2024-05-05 15:53:40.000000 argtoml-0.5.1/argtoml/opt.py
+drwxr-xr-x   0 jo3       (1000) jo3       (1000)        0 2024-05-05 16:25:20.986922 argtoml-0.5.1/argtoml.egg-info/
+-rw-r--r--   0 jo3       (1000) jo3       (1000)     3731 2024-05-05 16:25:20.000000 argtoml-0.5.1/argtoml.egg-info/PKG-INFO
+-rw-r--r--   0 jo3       (1000) jo3       (1000)      273 2024-05-05 16:25:20.000000 argtoml-0.5.1/argtoml.egg-info/SOURCES.txt
+-rw-r--r--   0 jo3       (1000) jo3       (1000)        1 2024-05-05 16:25:20.000000 argtoml-0.5.1/argtoml.egg-info/dependency_links.txt
+-rw-r--r--   0 jo3       (1000) jo3       (1000)        8 2024-05-05 16:25:20.000000 argtoml-0.5.1/argtoml.egg-info/top_level.txt
+-rw-r--r--   0 jo3       (1000) jo3       (1000)      951 2024-05-05 16:23:36.000000 argtoml-0.5.1/pyproject.toml
+-rw-r--r--   0 jo3       (1000) jo3       (1000)       38 2024-05-05 16:25:20.986922 argtoml-0.5.1/setup.cfg
+-rw-r--r--   0 jo3       (1000) jo3       (1000)       61 2023-07-23 14:09:52.000000 argtoml-0.5.1/setup.py
+drwxr-xr-x   0 jo3       (1000) jo3       (1000)        0 2024-05-05 16:25:20.986922 argtoml-0.5.1/tests/
+-rw-r--r--   0 jo3       (1000) jo3       (1000)      218 2023-07-23 14:09:52.000000 argtoml-0.5.1/tests/test_main.py
```

### Comparing `argtoml-0.5.0/LICENSE` & `argtoml-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `argtoml-0.5.0/PKG-INFO` & `argtoml-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argtoml
-Version: 0.5.0
+Version: 0.5.1
 Summary: Add the keys from a .toml file to your CLI as arguments. Their values default to the values in the .toml file.
 Author-email: Jochem Hölscher <a.fake@e.mail>
 Project-URL: homepage, https://github.com/JJJHolscher/argtoml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `argtoml-0.5.0/README.md` & `argtoml-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `argtoml-0.5.0/argtoml/__main__.py` & `argtoml-0.5.1/argtoml/__main__.py`

 * *Files identical despite different names*

### Comparing `argtoml-0.5.0/argtoml/locate.py` & `argtoml-0.5.1/argtoml/locate.py`

 * *Files identical despite different names*

### Comparing `argtoml-0.5.0/argtoml/main.py` & `argtoml-0.5.1/argtoml/main.py`

 * *Files identical despite different names*

### Comparing `argtoml-0.5.0/argtoml/opt.py` & `argtoml-0.5.1/argtoml/opt.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     elif type(opt) is dict:
         for k, v in opt.items():
             yield k, v
     else:
         raise TypeError
 
 
-def string_to_path(string: str, prefix: Path) -> Path:
+def string_to_path(string: str, prefix: Path) -> Union[str, Path]:
     """
     Convert a string to a Path object.
     """
     if string == "~":
         return Path.home()
 
     elif string == ".":
@@ -43,32 +43,33 @@
 
     elif len(string) > 1 and string[0:2] == "./":
         return prefix / string[2:]
 
     elif len(string) > 2 and string[0:3] == "../":
         return prefix.parent / string[3:]
 
-    raise ValueError
+    return string
 
 
 def merge_opts(old: Opt, add: Opt, path: Optional[Path]):
     new = copy.deepcopy(old)
 
     for k, v in iter_opt(add):
-        if v is str and path is not None:
+        t = type(v)
+        if t is str and path is not None:
             v = string_to_path(v, path)
 
-        if k not in old:
-            new[k] = v
-            continue
+        if k in old:
+            assert type(old[k]) is t
+            old_v = old[k]
+        else:
+            old_v = {}
 
-        t = type(v)
-        assert type(old[k]) is t
         if isinstance(v, get_args(Opt)):
-            new[k] = merge_opts(old[k], v, path)
+            new[k] = merge_opts(old_v, v, path)
         else:
             new[k] = v
 
     return new
 
 
 def opt_to_argument_parser(
```

### Comparing `argtoml-0.5.0/argtoml.egg-info/PKG-INFO` & `argtoml-0.5.1/argtoml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argtoml
-Version: 0.5.0
+Version: 0.5.1
 Summary: Add the keys from a .toml file to your CLI as arguments. Their values default to the values in the .toml file.
 Author-email: Jochem Hölscher <a.fake@e.mail>
 Project-URL: homepage, https://github.com/JJJHolscher/argtoml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `argtoml-0.5.0/pyproject.toml` & `argtoml-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "argtoml"
-version = "0.5.0"
+version = "0.5.1"
 description = "Add the keys from a .toml file to your CLI as arguments. Their values default to the values in the .toml file."
 dynamic = ["readme"]
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

