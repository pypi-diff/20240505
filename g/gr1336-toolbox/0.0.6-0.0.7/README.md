# Comparing `tmp/gr1336_toolbox-0.0.6.tar.gz` & `tmp/gr1336_toolbox-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gr1336_toolbox-0.0.6.tar", last modified: Sat May  4 02:16:06 2024, max compression
+gzip compressed data, was "gr1336_toolbox-0.0.7.tar", last modified: Sat May  4 18:25:19 2024, max compression
```

## Comparing `gr1336_toolbox-0.0.6.tar` & `gr1336_toolbox-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 02:16:06.298386 gr1336_toolbox-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-04 02:15:58.000000 gr1336_toolbox-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-04 02:16:06.298386 gr1336_toolbox-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-04 02:15:58.000000 gr1336_toolbox-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 02:16:06.298386 gr1336_toolbox-0.0.6/gr1336_toolbox/
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-04 02:15:58.000000 gr1336_toolbox-0.0.6/gr1336_toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-04 02:15:58.000000 gr1336_toolbox-0.0.6/gr1336_toolbox/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-05-04 02:15:58.000000 gr1336_toolbox-0.0.6/gr1336_toolbox/misc_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-04 02:15:58.000000 gr1336_toolbox-0.0.6/gr1336_toolbox/test_even_odd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-04 02:15:58.000000 gr1336_toolbox-0.0.6/gr1336_toolbox/text_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-05-04 02:15:58.000000 gr1336_toolbox-0.0.6/gr1336_toolbox/types_check.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 02:16:06.298386 gr1336_toolbox-0.0.6/gr1336_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-04 02:16:06.000000 gr1336_toolbox-0.0.6/gr1336_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-04 02:16:06.000000 gr1336_toolbox-0.0.6/gr1336_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 02:16:06.000000 gr1336_toolbox-0.0.6/gr1336_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-04 02:16:06.000000 gr1336_toolbox-0.0.6/gr1336_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-04 02:16:06.000000 gr1336_toolbox-0.0.6/gr1336_toolbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 02:16:06.298386 gr1336_toolbox-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-04 02:15:58.000000 gr1336_toolbox-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:25:19.537483 gr1336_toolbox-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-04 18:25:15.000000 gr1336_toolbox-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-04 18:25:19.537483 gr1336_toolbox-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-04 18:25:15.000000 gr1336_toolbox-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:25:19.533483 gr1336_toolbox-0.0.7/gr1336_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-04 18:25:15.000000 gr1336_toolbox-0.0.7/gr1336_toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-05-04 18:25:15.000000 gr1336_toolbox-0.0.7/gr1336_toolbox/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-05-04 18:25:15.000000 gr1336_toolbox-0.0.7/gr1336_toolbox/misc_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-04 18:25:15.000000 gr1336_toolbox-0.0.7/gr1336_toolbox/text_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-04 18:25:15.000000 gr1336_toolbox-0.0.7/gr1336_toolbox/txt_split_fnc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-05-04 18:25:15.000000 gr1336_toolbox-0.0.7/gr1336_toolbox/types_check.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:25:19.537483 gr1336_toolbox-0.0.7/gr1336_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-04 18:25:19.000000 gr1336_toolbox-0.0.7/gr1336_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-04 18:25:19.000000 gr1336_toolbox-0.0.7/gr1336_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 18:25:19.000000 gr1336_toolbox-0.0.7/gr1336_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-04 18:25:19.000000 gr1336_toolbox-0.0.7/gr1336_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-04 18:25:19.000000 gr1336_toolbox-0.0.7/gr1336_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 18:25:19.537483 gr1336_toolbox-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-04 18:25:15.000000 gr1336_toolbox-0.0.7/setup.py
```

### Comparing `gr1336_toolbox-0.0.6/LICENSE` & `gr1336_toolbox-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gr1336_toolbox-0.0.6/PKG-INFO` & `gr1336_toolbox-0.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gr1336_toolbox
-Version: 0.0.6
+Version: 0.0.7
 Summary: Personal collection of reusable tools in python.
 Home-page: https://github.com/gr1336/gr1336_toolbox/
 Author: gr1336
 License:  Apache Software License
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Testing
```

### Comparing `gr1336_toolbox-0.0.6/gr1336_toolbox/__init__.py` & `gr1336_toolbox-0.0.7/gr1336_toolbox/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     save_parquet,
     save_text,
     save_yaml,
     get_dirs,
     get_files,
     move_to,
     create_path,
+    delete_path,
 )
 from .types_check import (
     _path,
     _dict,
     _array,
     _float,
     _number,
@@ -34,44 +35,49 @@
     _int,
 )
 from .text_tools import (
     unescape,
     trimincompletesentence,
     simplify_quotes,
     blob_split,
+    txtsplit,
+    clear_empty,
 )
 
 __all__ = [
     "_str",
     "_int",
     "_path",
     "_dict",
     "_array",
     "_float",
     "_numpy",
     "_number",
     "move_to",
     "np_list",
+    "txtsplit",
     "_compare",
     "unescape",
     "try_call",
-    "clipboard",
     "get_dirs",
+    "clipboard",
     "get_files",
     "load_text",
     "save_text",
     "load_yaml",
     "save_yaml",
     "blob_split",
     "filter_list",
     "create_path",
+    "delete_path",
     "dict_to_list",
     "load_parquet",
     "current_time",
     "flatten_list",
     "save_parquet",
     "simplify_quotes",
     "import_functions",
     "recursive_replacer",
     "percentage_difference",
     "trimincompletesentence",
+    "clear_empty",
 ]
```

### Comparing `gr1336_toolbox-0.0.6/gr1336_toolbox/file_manager.py` & `gr1336_toolbox-0.0.7/gr1336_toolbox/file_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,23 +12,30 @@
 def get_dirs(path: str | Path) -> list[Path]:
     if not _path(path):
         return []
     return [x for x in Path(path).glob("*") if x.is_dir()]
 
 
 def get_files(
-    path: str | Path, extensions: str | None = None
+    path: str | Path, extensions: str | list[str] | tuple[str, ...] | None = None
 ) -> list[Path]:
-
     if not _path(path):
         return []
-    if not extensions:
+    elif not extensions:
         return [x for x in Path(path).glob("*") if x.is_file()]
-    if _str(path):
+    elif _str(extensions):
+        if extensions[0] == ".":
+            extensions = extensions[1:]
         return [x for x in Path(path).glob(f"*.{extensions}") if x.is_file()]
+    elif _array(extensions):
+        results = []
+        for y in extensions:
+            if _str(y):
+                results.extend(get_files(path, y))
+        return results
     return []
 
 
 def create_path(path: str | Path):
     Path(path).parent.mkdir(parents=True, exist_ok=True)
 
 
@@ -101,7 +108,14 @@
 def move_to(source_path: str | Path, destination_path: str | Path):
     assert (
         str(source_path).strip() and Path(source_path).exists()
     ), "Source path does not exists!"
 
     os.makedirs(str(destination_path), exist_ok=True)
     shutil.move(source_path, destination_path)
+
+
+def delete_path(path: str | Path | list[str | Path] | tuple[str | Path, ...]):
+    if _str(path) and Path(path).exists():
+        shutil.rmtree(path)
+    elif _array(path):
+        delete_path(path)
```

### Comparing `gr1336_toolbox-0.0.6/gr1336_toolbox/misc_tools.py` & `gr1336_toolbox-0.0.7/gr1336_toolbox/misc_tools.py`

 * *Files identical despite different names*

### Comparing `gr1336_toolbox-0.0.6/gr1336_toolbox/types_check.py` & `gr1336_toolbox-0.0.7/gr1336_toolbox/types_check.py`

 * *Files identical despite different names*

### Comparing `gr1336_toolbox-0.0.6/gr1336_toolbox.egg-info/PKG-INFO` & `gr1336_toolbox-0.0.7/gr1336_toolbox.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gr1336_toolbox
-Version: 0.0.6
+Version: 0.0.7
 Summary: Personal collection of reusable tools in python.
 Home-page: https://github.com/gr1336/gr1336_toolbox/
 Author: gr1336
 License:  Apache Software License
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Testing
```

### Comparing `gr1336_toolbox-0.0.6/setup.py` & `gr1336_toolbox-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
-    version="0.0.6",
+    version="0.0.7",
     name="gr1336_toolbox",
     description="Personal collection of reusable tools in python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gr1336/gr1336_toolbox/",
     install_requires=["numpy", "pyperclip", "textblob", "pyyaml", "pyarrow"],
     author="gr1336",
@@ -17,8 +17,8 @@
         "Topic :: Software Development",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Testing",
         "Topic :: Software Development :: Pre-processors",
         "Topic :: Utilities",
         "License :: OSI Approved :: Apache Software License",
     ],
-)
+)
```

