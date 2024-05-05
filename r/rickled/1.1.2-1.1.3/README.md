# Comparing `tmp/rickled-1.1.2.tar.gz` & `tmp/rickled-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\rickled-1.1.2.tar", last modified: Tue Apr 23 21:30:35 2024, max compression
+gzip compressed data, was "dist\rickled-1.1.3.tar", last modified: Sun May  5 15:47:11 2024, max compression
```

## Comparing `rickled-1.1.2.tar` & `rickled-1.1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 21:30:35.000000 rickled-1.1.2/
--rw-rw-rw-   0        0        0    11357 2021-12-06 14:18:08.000000 rickled-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     4790 2024-04-23 21:30:35.000000 rickled-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     5086 2024-04-23 21:25:49.000000 rickled-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 21:30:35.000000 rickled-1.1.2/rickled/
--rw-rw-rw-   0        0        0    56442 2024-04-20 17:00:51.000000 rickled-1.1.2/rickled/__init__.py
--rw-rw-rw-   0        0        0       48 2024-04-23 21:30:34.000000 rickled-1.1.2/rickled/__version__.py
--rw-rw-rw-   0        0        0    27437 2024-04-20 16:50:34.000000 rickled-1.1.2/rickled/cli.py
--rw-rw-rw-   0        0        0     3906 2024-04-20 13:17:12.000000 rickled-1.1.2/rickled/net.py
--rw-rw-rw-   0        0        0    15674 2024-04-18 21:18:48.000000 rickled-1.1.2/rickled/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-23 21:30:35.000000 rickled-1.1.2/rickled.egg-info/
--rw-rw-rw-   0        0        0     4790 2024-04-23 21:30:35.000000 rickled-1.1.2/rickled.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      590 2024-04-23 21:30:35.000000 rickled-1.1.2/rickled.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 21:30:35.000000 rickled-1.1.2/rickled.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-04-23 21:30:35.000000 rickled-1.1.2/rickled.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-23 21:30:35.000000 rickled-1.1.2/rickled.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       58 2024-04-23 21:30:35.000000 rickled-1.1.2/rickled.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-23 21:30:35.000000 rickled-1.1.2/rickled.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       95 2024-04-23 21:30:35.000000 rickled-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     2195 2024-04-09 19:28:11.000000 rickled-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 21:30:35.000000 rickled-1.1.2/tests/
-drwxrwxrwx   0        0        0        0 2024-04-23 21:30:35.000000 rickled-1.1.2/tests/integration/
--rw-rw-rw-   0        0        0        0 2021-12-06 14:18:08.000000 rickled-1.1.2/tests/integration/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 21:30:35.000000 rickled-1.1.2/tests/unittest/
--rw-rw-rw-   0        0        0        0 2022-03-13 15:27:46.000000 rickled-1.1.2/tests/unittest/__init__.py
--rw-rw-rw-   0        0        0     9041 2024-04-20 16:57:44.000000 rickled-1.1.2/tests/unittest/test_advanced.py
--rw-rw-rw-   0        0        0        0 2023-09-14 16:37:08.000000 rickled-1.1.2/tests/unittest/test_cli.py
--rw-rw-rw-   0        0        0        0 2023-07-21 00:44:56.000000 rickled-1.1.2/tests/unittest/test_net.py
--rw-rw-rw-   0        0        0     1717 2024-04-09 19:28:11.000000 rickled-1.1.2/tests/unittest/test_object_rickler.py
--rw-rw-rw-   0        0        0    12510 2024-04-20 16:59:01.000000 rickled-1.1.2/tests/unittest/test_rickle.py
--rw-rw-rw-   0        0        0     6174 2024-04-09 19:28:11.000000 rickled-1.1.2/tests/unittest/test_schema_tool.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:47:11.000000 rickled-1.1.3/
+-rw-rw-rw-   0        0        0    11357 2021-12-06 14:18:08.000000 rickled-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0     4790 2024-05-05 15:47:11.000000 rickled-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5086 2024-04-25 15:13:57.000000 rickled-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 15:47:11.000000 rickled-1.1.3/rickled/
+-rw-rw-rw-   0        0        0    60004 2024-04-25 17:29:08.000000 rickled-1.1.3/rickled/__init__.py
+-rw-rw-rw-   0        0        0       48 2024-05-05 15:47:10.000000 rickled-1.1.3/rickled/__version__.py
+-rw-rw-rw-   0        0        0    28702 2024-04-25 17:05:57.000000 rickled-1.1.3/rickled/cli.py
+-rw-rw-rw-   0        0        0     4479 2024-04-25 17:10:22.000000 rickled-1.1.3/rickled/net.py
+-rw-rw-rw-   0        0        0    17144 2024-04-25 17:12:02.000000 rickled-1.1.3/rickled/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:47:11.000000 rickled-1.1.3/rickled.egg-info/
+-rw-rw-rw-   0        0        0     4790 2024-05-05 15:47:11.000000 rickled-1.1.3/rickled.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      590 2024-05-05 15:47:11.000000 rickled-1.1.3/rickled.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 15:47:11.000000 rickled-1.1.3/rickled.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-05-05 15:47:11.000000 rickled-1.1.3/rickled.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-05 15:47:11.000000 rickled-1.1.3/rickled.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      100 2024-05-05 15:47:11.000000 rickled-1.1.3/rickled.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-05 15:47:11.000000 rickled-1.1.3/rickled.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       95 2024-05-05 15:47:11.000000 rickled-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     2237 2024-04-25 16:00:37.000000 rickled-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:47:11.000000 rickled-1.1.3/tests/
+drwxrwxrwx   0        0        0        0 2024-05-05 15:47:11.000000 rickled-1.1.3/tests/integration/
+-rw-rw-rw-   0        0        0        0 2021-12-06 14:18:08.000000 rickled-1.1.3/tests/integration/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:47:11.000000 rickled-1.1.3/tests/unittest/
+-rw-rw-rw-   0        0        0        0 2022-03-13 15:27:46.000000 rickled-1.1.3/tests/unittest/__init__.py
+-rw-rw-rw-   0        0        0     9041 2024-04-25 15:13:57.000000 rickled-1.1.3/tests/unittest/test_advanced.py
+-rw-rw-rw-   0        0        0        0 2023-09-14 16:37:08.000000 rickled-1.1.3/tests/unittest/test_cli.py
+-rw-rw-rw-   0        0        0        0 2023-07-21 00:44:56.000000 rickled-1.1.3/tests/unittest/test_net.py
+-rw-rw-rw-   0        0        0     1717 2024-04-09 19:28:11.000000 rickled-1.1.3/tests/unittest/test_object_rickler.py
+-rw-rw-rw-   0        0        0    12893 2024-05-05 15:46:50.000000 rickled-1.1.3/tests/unittest/test_rickle.py
+-rw-rw-rw-   0        0        0     6174 2024-04-09 19:28:11.000000 rickled-1.1.3/tests/unittest/test_schema_tool.py
```

### Comparing `rickled-1.1.2/LICENSE` & `rickled-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rickled-1.1.2/PKG-INFO` & `rickled-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rickled
-Version: 1.1.2
+Version: 1.1.3
 Summary: Tools for pickling Python objects in a completely different way
 Home-page: https://github.com/Zipfian-Science/rickle
 Download-URL: https://github.com/Zipfian-Science/rickle/archive/v_01.tar.gz
 Author: Zipfian Science
 Author-email: about@zipfian.science
 License: Apache 2.0
 Keywords: Pickle,Python,YAML,JSON
@@ -124,10 +124,10 @@
 'hell world!'
 ```
 
 ## Release
 
 See the version history in [changelog](https://zipfian.science/docs/rickle/changelog.html).
 
-- Date: 2024-04-23
-- Version: 1.1.2
+- Date: 2024-05-05
+- Version: 1.1.3
```

### Comparing `rickled-1.1.2/README.md` & `rickled-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `rickled-1.1.2/rickled/__init__.py` & `rickled-1.1.3/rickled/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 from .__version__ import __version__, __date__
 import os
 import json
 import copy
 import warnings
 from typing import Union, TypeVar
-from io import TextIOWrapper
+from io import TextIOWrapper, BytesIO
 import yaml
 import base64
 import types
 import re
 import inspect
 from functools import partial
 import uuid
+import sys
+import tomli_w as tomlw
 
 try:
     import requests
 except ModuleNotFoundError as exc:
     warnings.warn(f"The module requests is not installed. This will break API calls.")
 
+if sys.version_info < (3, 11):
+    import tomli as toml
+else:
+    import tomllib as toml
+
+from rickled.tools import toml_null_stripper
+
 class ObjectRickler:
     """
     A class to convert Python objects to Rickle objects, deconstruct objects, create objects from Rickle objects.
 
     Notes:
         - `tuple` types are deconstructed as lists
 
@@ -270,16 +279,18 @@
             self._iternalize(base, deep, **init_args)
             return
 
         if isinstance(base, TextIOWrapper):
             stringed = base.read()
         elif isinstance(base, list):
             for file in base:
-                with open(file, 'r') as f:
-                    stringed = f'{stringed}\n{f.read()}'
+                if os.path.isfile(file):
+                    with open(file, 'r') as f:
+                        stringed = f'{stringed}\n{f.read()}'
+
         elif os.path.isfile(base):
             with open(base, 'r') as f:
                 stringed = f.read()
         elif isinstance(base, str):
             try:
                 from urllib3.util import parse_url
                 try:
@@ -297,28 +308,37 @@
             stringed = base
 
         if not init_args is None:
             for k, v in init_args.items():
                 _k = f'_|{k}|_'
                 stringed = stringed.replace(_k, json.dumps(v))
 
+        error_list = list()
         try:
             dict_data = yaml.safe_load(stringed)
             self._iternalize(dict_data, deep, **init_args)
             return
         except Exception as exc:
-            print("Tried YAML: {}".format(exc))
+            error_list.append(f"YAML: {exc}")
         try:
-            dict_data = json.loads(base)
+            dict_data = json.loads(stringed)
             self._iternalize(dict_data, deep, **init_args)
             return
         except Exception as exc:
-            print("Tried JSON: {}".format(exc))
+            error_list.append(f"JSON: {exc}")
+        try:
+            dict_data = toml.loads(stringed)
+            self._iternalize(dict_data, deep, **init_args)
+            return
+        except Exception as exc:
+            error_list.append(f"TOML: {exc}")
 
 
+        for error in error_list:
+            print(error)
         raise ValueError('Base object could not be internalized, type {} not handled'.format(type(base)))
 
     def __repr__(self):
         keys = self.__dict__
         items = ("{}={!r}".format(k, self.__dict__[k]) for k in keys if not str(k).__contains__(self.__class__.__name__) and not str(k).endswith('__meta_info') )
         return "{}({})".format(type(self).__name__, ", ".join(items))
 
@@ -689,16 +709,86 @@
             try:
                 self._recursive_search(self.dict(), key)
                 return True
             except StopIteration:
                 return False
         return False
 
+    def to_yaml(self, output: Union[str, TextIOWrapper] = None, serialised: bool = False):
+        """
+        Does a self dump to a YAML file or returns as string.
+
+        Args:
+            output (str, TextIOWrapper): File path or stream (default = None).
+            serialised (bool): Give a Python dictionary in serialised (True) form or deserialised (default = False).
+
+        Notes:
+            Functions and lambdas are always given in serialised form.
+        """
+
+        self_as_dict = self.dict(serialised=serialised)
+
+        if output:
+            if isinstance(output, TextIOWrapper):
+                yaml.safe_dump(self_as_dict, output)
+            elif isinstance(output, str):
+                with open(output, 'w', encoding='utf-8') as fs:
+                    yaml.safe_dump(self_as_dict, fs)
+        else:
+            return yaml.safe_dump(self_as_dict, None)
+
+    def to_json(self, output: Union[str, TextIOWrapper] = None, serialised: bool = False):
+        """
+        Does a self dump to a JSON file or returns as string.
+
+        Args:
+            output (str, TextIOWrapper): File path or stream (default = None).
+            serialised (bool): Give a Python dictionary in serialised (True) form or deserialised (default = False).
+
+        Notes:
+            Functions and lambdas are always given in serialised form.
+        """
+        self_as_dict = self.dict(serialised=serialised)
+
+        if output:
+            if isinstance(output, TextIOWrapper):
+                json.dump(self_as_dict, output)
+            elif isinstance(output, str):
+                with open(output, 'w', encoding='utf-8') as fs:
+                    json.dump(self_as_dict, fs)
+        else:
+            return json.dumps(self_as_dict)
+
+    def to_toml(self, output: Union[str, BytesIO] = None, serialised: bool = False):
+        """
+        Does a self dump to a TOML file or returns as string.
+
+        Args:
+            output (str, TextIOWrapper): File path or stream (default = None).
+            serialised (bool): Give a Python dictionary in serialised (True) form or deserialised (default = False).
+
+        Notes:
+            Functions and lambdas are always given in serialised form.
+            IO stream "output" needs to be BytesIO object
+        """
+
+        self_as_dict = toml_null_stripper(self.dict(serialised=serialised))
+
+        if output:
+            if isinstance(output, BytesIO):
+                tomlw.dump(self_as_dict, output)
+            elif isinstance(output, str):
+                with open(output, 'wb', encoding='utf-8') as fs:
+                    tomlw.dump(self_as_dict, fs)
+        else:
+            return tomlw.dumps(self_as_dict)
+
     def to_yaml_file(self, file_path : str, serialised : bool = False):
         """
+        (DEPRECATED) After version 1.5.0 this will be removed, use ``to_yaml`` instead.
         Does a self dump to a YAML file.
 
         Args:
             file_path (str): File path.
             serialised (bool): Give a Python dictionary in serialised (True) form or deserialised (default = False).
 
         Notes:
@@ -706,14 +796,15 @@
         """
         self_as_dict = self.dict(serialised=serialised)
         with open(file_path, 'w', encoding='utf-8') as fs:
             yaml.safe_dump(self_as_dict, fs)
 
     def to_yaml_string(self, serialised : bool = False):
         """
+        (DEPRECATED) After version 1.5.0 this will be removed, use ``to_yaml`` instead.
         Dumps self to YAML string.
 
         Args:
             serialised (bool): Give a Python dictionary in serialised (True) form or deserialised (default = False).
 
         Notes:
             Functions and lambdas are always given in serialised form.
@@ -722,14 +813,15 @@
             str: YAML representation.
         """
         self_as_dict = self.dict(serialised=serialised)
         return yaml.safe_dump(self_as_dict, None)
 
     def to_json_file(self, file_path: str, serialised : bool = False):
         """
+        (DEPRECATED) After version 1.5.0 this will be removed, use ``to_json`` instead.
         Does a self dump to a JSON file.
 
         Args:
             file_path (str): File path.
             serialised (bool): Give a Python dictionary in serialised (True) form or deserialised (default = False).
 
         Notes:
@@ -737,14 +829,15 @@
         """
         self_as_dict = self.dict(serialised=serialised)
         with open(file_path, 'w', encoding='utf-8') as fs:
             json.dump(self_as_dict, fs)
 
     def to_json_string(self, serialised : bool = False):
         """
+        (DEPRECATED) After version 1.5.0 this will be removed, use ``to_json`` instead.
         Dumps self to YAML string.
 
         Args:
             serialised (bool): Give a Python dictionary in serialised (True) form or deserialised (default = False).
 
         Notes:
             Functions and lambdas are always given in serialised form.
@@ -756,15 +849,15 @@
         return json.dumps(self_as_dict)
 
     def meta(self, name):
         """
         Get the metadata for a property.
 
         Args:
-            name (str): The name of the proprty.
+            name (str): The name of the property.
 
         Returns:
             dict: The metadata as a dict.
         """
         return self.__meta_info[name]
 
     def add_attr(self, name, value):
```

### Comparing `rickled-1.1.2/rickled/cli.py` & `rickled-1.1.3/rickled/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,24 @@
 from enum import Enum
 
 import rickled.__version__ as ver
 import argparse
 from rickled.tools import cli_bcolors
 from rickled.tools import Schema
 from rickled.tools import Converter
+from rickled.tools import toml_null_stripper
 
 from rickled import Rickle
 import re
 import json
 import yaml
 import ast
 
+import tomli_w as tomlw
+
 GITHUB_DOCS_URL = "https://github.com/Zipfian-Science/rickled/blob/master/docs/source/cli_tools.rst#cli-tools"
 
 class CLIError(Exception):
 
     class CLITool(Enum):
         CONV = 1
         OBJ = 2
@@ -53,72 +56,96 @@
         raise CLIError(message=str(exc), cli_tool=CLIError.CLITool.CONV)
 
 def obj_get(args):
     try:
         if args:
             r = Rickle(args.i, load_lambda=args.l)
             v = r.get(args.key)
+            dump_type = args.t.lower()
+
             if isinstance(v, Rickle):
-                v = v.dict()
+                v = toml_null_stripper(v.dict())
+            if isinstance(v, dict):
+                v = toml_null_stripper(v)
             elif v is None:
                 v = ''
 
             if args.o:
-                with open(args.o, 'w') as fp:
-                    if args.t.lower() == 'json':
+
+                if dump_type == 'json':
+                    with open(args.o, 'w') as fp:
                         json.dump(v, fp)
-                    else:
+                elif dump_type == 'toml':
+                    with open(args.o, 'wb') as fp:
+                        tomlw.dump(v, fp)
+                else:
+                    with open(args.o, 'w') as fp:
                         yaml.safe_dump(v, fp)
+
+
             else:
-                if args.t.lower() == 'json':
+                if dump_type == 'json':
                     print(json.dumps(v))
+                elif dump_type == 'toml':
+                    print(tomlw.dumps(v))
                 else:
                     print(yaml.safe_dump(v))
 
+
     except Exception as exc:
         raise CLIError(message=str(exc), cli_tool=CLIError.CLITool.OBJ_GET)
 
 
 
 def obj_set(args):
     try:
         if args:
             r = Rickle(args.i)
             r.set(args.key, args.value)
+            dump_type = args.t.lower()
 
             if args.o:
-                if args.t.lower() == 'json':
-                    r.to_json_file(args.o)
+                if dump_type == 'json':
+                    r.to_json(output=args.o)
+                elif dump_type == 'toml':
+                    r.to_toml(output=args.o)
                 else:
-                    r.to_yaml_file(args.o)
+                    r.to_yaml(output=args.o)
             else:
-                if args.t.lower() == 'json':
-                    print(r.to_json_string())
+                if dump_type == 'json':
+                    print(r.to_json())
+                elif dump_type == 'toml':
+                    print(r.to_toml())
                 else:
-                    print(r.to_yaml_string())
+                    print(r.to_yaml())
     except Exception as exc:
         raise CLIError(message=str(exc), cli_tool=CLIError.CLITool.OBJ_SET)
 
 
 def obj_del(args):
     try:
         if args:
             r = Rickle(args.i)
             r.remove(args.key)
+            dump_type = args.t.lower()
 
             if args.o:
-                if args.t.lower() == 'json':
-                    r.to_json_file(args.o)
+                if dump_type == 'json':
+                    r.to_json(output=args.o)
+                elif dump_type == 'toml':
+                    r.to_toml(output=args.o)
                 else:
-                    r.to_yaml_file(args.o)
+                    r.to_yaml(output=args.o)
             else:
-                if args.t.lower() == 'json':
-                    print(r.to_json_string())
+                if dump_type == 'json':
+                    print(r.to_json())
+                elif dump_type == 'toml':
+                    print(r.to_toml())
                 else:
-                    print(r.to_yaml_string())
+                    print(r.to_yaml())
     except Exception as exc:
         raise CLIError(message=str(exc), cli_tool=CLIError.CLITool.OBJ_DEL)
 
 def obj_type(args):
     try:
         if args:
             r = Rickle(args.i, load_lambda=args.l)
@@ -171,14 +198,15 @@
         else:
             raise ValueError('Could not interpret type, only str, int, float, bool, list, dict accepted.')
 
     try:
         re_pat = re.compile(r"(.+?)=(.+)")
         if args:
             r = Rickle(args.i, load_lambda=args.l)
+            dump_type = args.t.lower()
 
             params = dict()
             if args.params:
                 for p in args.params:
                     m = re_pat.match(p)
                     param_name = m.group(1)
                     param_value = m.group(2)
@@ -189,21 +217,25 @@
                         param_value = guess_parse(param_value)
 
                     params[param_name] = param_value
             v = r(args.key, **params)
 
             if not v is None:
                 if isinstance(v, Rickle):
-                    if args.t.lower() == 'json':
-                        print(v.to_json_string())
+                    if dump_type == 'json':
+                        print(v.to_json())
+                    elif dump_type == 'toml':
+                        print(v.to_toml())
                     else:
-                        print(v.to_yaml_string())
+                        print(v.to_yaml())
                 elif isinstance(v, dict):
-                    if args.t.lower() == 'json':
+                    if dump_type == 'json':
                         print(json.dumps(v))
+                    elif dump_type == 'toml':
+                        print(tomlw.dumps(v))
                     else:
                         print(yaml.safe_dump(v))
                 else:
                     print(v)
     except Exception as exc:
         raise CLIError(message=str(exc), cli_tool=CLIError.CLITool.OBJ_FUNC)
 
@@ -272,15 +304,20 @@
 ██████╗ ██╗ ██████╗██╗  ██╗██╗     ███████╗
 ██╔══██╗██║██╔════╝██║ ██╔╝██║     ██╔════╝
 ██████╔╝██║██║     █████╔╝ ██║     █████╗  
 ██╔══██╗██║██║     ██╔═██╗ ██║     ██╔══╝  
 ██║  ██║██║╚██████╗██║  ██╗███████╗███████╗
 ╚═╝  ╚═╝╚═╝ ╚═════╝╚═╝  ╚═╝╚══════╝╚══════╝{cli_bcolors.ENDC}
 
-{cli_bcolors.HEADER}YAML tools for Python{cli_bcolors.ENDC} (version {ver}).
+{cli_bcolors.HEADER}YAML (+JSON, TOML...) tools for Python{cli_bcolors.ENDC} (version {ver}).
+---------------------------------------------------------------------------------------------
+Supported file types ({cli_bcolors.OKBLUE}-t{cli_bcolors.ENDC}) include:
+- {cli_bcolors.OKBLUE}YAML{cli_bcolors.ENDC}
+- {cli_bcolors.OKBLUE}JSON{cli_bcolors.ENDC}
+- {cli_bcolors.OKBLUE}TOML{cli_bcolors.ENDC}
 ---------------------------------------------------------------------------------------------
 """,
         epilog=f"""
 ---------------------------------------------------------------------------------------------
 \nFor usage examples, visit:\n{cli_bcolors.UNDERLINE}{GITHUB_DOCS_URL}{cli_bcolors.ENDC}\n\n
 ---------------------------------------------------------------------------------------------
         """
@@ -589,16 +626,15 @@
     parser_schema_gen.set_defaults(func=gen)
 
     #################################################
     # Making a bit more friendly for debugging
     try:
         args = parser.parse_args()
         args.func(args)
-    except AttributeError as exc:
-        sys.stderr.write(f'\n{cli_bcolors.FAIL}error: {exc}{cli_bcolors.ENDC}\n\n')
+    except AttributeError:
         parser.print_help(sys.stderr)
         sys.exit(2)
     except CLIError as cli_exc:
         sys.stderr.write(f'\n{cli_bcolors.FAIL}error: {cli_exc.message}{cli_bcolors.ENDC}\n\n')
         if cli_exc.cli_tool == CLIError.CLITool.CONV:
             parser_conv.print_help(sys.stderr)
         elif cli_exc.cli_tool == CLIError.CLITool.OBJ:
```

### Comparing `rickled-1.1.2/rickled/net.py` & `rickled-1.1.3/rickled/net.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 import sys
 import traceback
 import warnings
 import json
 
 import yaml
 
-from rickled import Rickle
+import tomli_w as tomlw
+if sys.version_info < (3, 11):
+    import tomli as toml
+else:
+    import tomllib as toml
+
+from rickled import Rickle, toml_null_stripper
 
 try:
     from twisted.web import server, resource
     from twisted.internet import reactor, endpoints, ssl
     from twisted.python import log
 except ModuleNotFoundError as exc:
     warnings.warn('Required Python package not found.', ImportWarning)
@@ -48,22 +54,28 @@
 
         request.setResponseCode(200)
         try:
             if isinstance(content, Rickle):
                 response = content.dict(self.serialised)
                 if self.output_type == 'json':
                     request.setHeader(b"content-type", b"application/json")
-                    response = json.dumps(response)
+                    response = content.to_json(serialised=self.serialised)
+                elif self.output_type == 'toml':
+                    request.setHeader(b"content-type", b"application/toml")
+                    response = content.to_toml(serialised=self.serialised)
                 else:
                     request.setHeader(b"content-type", b"application/yaml")
-                    response = yaml.safe_dump(response)
+                    response = content.to_yaml(serialised=self.serialised)
             elif isinstance(content, dict) or isinstance(content, list):
                 if self.output_type == 'json':
                     request.setHeader(b"content-type", b"application/json")
                     response = json.dumps(content)
+                elif self.output_type == 'toml':
+                    request.setHeader(b"content-type", b"application/toml")
+                    response = tomlw.dumps(toml_null_stripper(content))
                 else:
                     request.setHeader(b"content-type", b"application/yaml")
                     response = yaml.safe_dump(content)
             elif isinstance(content, bytes):
                 request.setHeader(b"content-type", b"application/x-binary")
                 return content
             elif isinstance(content, str):
```

### Comparing `rickled-1.1.2/rickled/tools.py` & `rickled-1.1.3/rickled/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,39 @@
 from typing import List, Union
 from pathlib import Path
 import yaml
 import json
 import os
+import sys
+
+import tomli_w as tomlw
+if sys.version_info < (3, 11):
+    import tomli as toml
+else:
+    import tomllib as toml
+
+def toml_null_stripper(d):
+    new_dict = {}
+    for k, v in d.items():
+        if isinstance(v, dict):
+            v = toml_null_stripper(v)
+        if v not in (u"", None, {}):
+            new_dict[k] = v
+    return new_dict
 
 class cli_bcolors:
     HEADER = '\033[95m'
     OKBLUE = '\033[94m'
     OKGREEN = '\033[92m'
     WARNING = '\033[93m'
     FAIL = '\033[91m'
     ENDC = '\033[0m'
     BOLD = '\033[1m'
     UNDERLINE = '\033[4m'
 
-
 class Schema:
     """
     Tool for inferring schemas from Python dicts and validating schemas.
 
     Args:
         input_files (list): List of input file paths (default = None).
         input_directories (list): List of directories (default = None).
@@ -45,30 +60,33 @@
             self.schema = schema
 
         self.output_files = output_files
 
         self.output_dir = output_dir
 
         self.silent = silent
-
-        self.default_output_type = default_output_type
+        if default_output_type.strip().lower() == 'yml':
+            default_output_type = 'yaml'
+        self.default_output_type = default_output_type.strip().lower()
 
     def do_generation(self):
         """
         Generates schema files for the given input files.
         """
         if self.input_files is None and self.input_directories is None:
             raise ValueError("Either input_files or input_directories must be defined!")
 
         if self.input_files is None and not self.input_directories is None:
             self.input_files = list()
             for d in self.input_directories:
                 dir_path = Path(d)
                 self.input_files.extend(list(dir_path.glob("*.yaml")))
+                self.input_files.extend(list(dir_path.glob("*.yml")))
                 self.input_files.extend(list(dir_path.glob("*.json")))
+                self.input_files.extend(list(dir_path.glob("*.toml")))
 
         if self.output_files is None:
             self.output_files = list()
             out_dir = f"{self.output_dir}/" if self.output_dir else './'
             for input_file in self.input_files:
                 self.output_files.append(f"{out_dir}{os.path.splitext(input_file)[0]}.schema.{self.default_output_type.lower()}")
 
@@ -88,14 +106,18 @@
                     with output_file.open("w") as fout:
                         yaml.safe_dump(schema, fout)
 
                 if suffix == '.json':
                     with output_file.open("w") as fout:
                         json.dump(schema, fout)
 
+                if suffix == '.toml':
+                    with output_file.open("wb") as fout:
+                        tomlw.dump(toml_null_stripper(schema), fout)
+
                 if not self.silent:
                     print(f"{cli_bcolors.OKBLUE}{pair[0]}{cli_bcolors.ENDC} -> {cli_bcolors.OKBLUE}{pair[1]}{cli_bcolors.ENDC}")
                 continue
             except Exception as exc:
                 if not self.silent:
                     print(f"{cli_bcolors.FAIL}{str(exc)}{cli_bcolors.ENDC}")
                 continue
@@ -112,15 +134,17 @@
             raise ValueError("Either input_files or input_directories must be defined!")
 
         if self.input_files is None and not self.input_directories is None:
             self.input_files = list()
             for d in self.input_directories:
                 dir_path = Path(d)
                 self.input_files.extend(list(dir_path.glob("*.yaml")))
+                self.input_files.extend(list(dir_path.glob("*.yml")))
                 self.input_files.extend(list(dir_path.glob("*.json")))
+                self.input_files.extend(list(dir_path.glob("*.toml")))
 
         for file in self.input_files:
             try:
                 input_data = Converter.infer_read_file_type(file)
 
                 passed = Schema.schema_validation(input_data, self.schema, no_print=self.silent)
 
@@ -342,24 +366,34 @@
             with input_file.open("r") as fin:
                 return json.load(fin)
 
         if suffix in ['.yaml', '.yml']:
             with input_file.open("r") as fin:
                 return yaml.safe_load(fin)
 
+        if suffix == '.toml':
+            with input_file.open("rb") as fin:
+                return toml.load(fin)
+
         try:
             with input_file.open("r") as fin:
                 return json.load(fin)
         except:
             pass
 
         try:
             with input_file.open("r") as fin:
                 return yaml.safe_load(fin)
         except:
+            pass
+
+        try:
+            with input_file.open("rb") as fin:
+                return toml.load(fin)
+        except:
             raise ValueError(f"Input file {input_file.name} could not be inferred")
 
     def do_convert(self):
         """
         Converts all input files to output type(s).
         """
         if self.input_files is None and self.input_directories is None:
@@ -369,15 +403,17 @@
             # set output to none as it should not be defined in this scenario
             self.output_files = None
             self.input_files = list()
             for d in self.input_directories:
                 dir_path = Path(d)
                 # TODO extend glo range here if expanding
                 self.input_files.extend(list(dir_path.glob("*.yaml")))
+                self.input_files.extend(list(dir_path.glob("*.yml")))
                 self.input_files.extend(list(dir_path.glob("*.json")))
+                self.input_files.extend(list(dir_path.glob("*.toml")))
 
 
         if self.output_files is None:
             self.output_files = list()
             for input_file in self.input_files:
                 self.output_files.append(f"{os.path.splitext(input_file)[0]}.{self.default_output_type.lower()}")
 
@@ -395,14 +431,18 @@
                     with output_file.open("w") as fout:
                         yaml.safe_dump(input_data, fout)
 
                 if suffix == '.json':
                     with output_file.open("w") as fout:
                         json.dump(input_data, fout)
 
+                if suffix == '.toml':
+                    with output_file.open("wb") as fout:
+                        tomlw.dump(toml_null_stripper(input_data), fout)
+
                 if not self.silent:
                     print(f"{cli_bcolors.OKBLUE}{pair[0]}{cli_bcolors.ENDC} -> {cli_bcolors.OKBLUE}{pair[1]}{cli_bcolors.ENDC}")
                 continue
             except Exception as exc:
                 if not self.silent:
                     print(f"{cli_bcolors.FAIL}{str(exc)}{cli_bcolors.ENDC}")
                 continue
```

### Comparing `rickled-1.1.2/rickled.egg-info/PKG-INFO` & `rickled-1.1.3/rickled.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rickled
-Version: 1.1.2
+Version: 1.1.3
 Summary: Tools for pickling Python objects in a completely different way
 Home-page: https://github.com/Zipfian-Science/rickle
 Download-URL: https://github.com/Zipfian-Science/rickle/archive/v_01.tar.gz
 Author: Zipfian Science
 Author-email: about@zipfian.science
 License: Apache 2.0
 Keywords: Pickle,Python,YAML,JSON
@@ -124,10 +124,10 @@
 'hell world!'
 ```
 
 ## Release
 
 See the version history in [changelog](https://zipfian.science/docs/rickle/changelog.html).
 
-- Date: 2024-04-23
-- Version: 1.1.2
+- Date: 2024-05-05
+- Version: 1.1.3
```

### Comparing `rickled-1.1.2/rickled.egg-info/SOURCES.txt` & `rickled-1.1.3/rickled.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rickled-1.1.2/setup.py` & `rickled-1.1.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 if os.path.isfile(os.path.join(here, 'requirements.txt')):
     with open(os.path.join(here, 'requirements.txt'), encoding='utf-8') as f:
         pipreq = f.readlines()
         # remove pip flag
         if '-i http' in pipreq[0]:
             pipreq.pop(0)
 else:
-    pipreq = ['pyyaml', 'requests']
+    pipreq = ['pyyaml', 'requests', "tomli;python_version<'3.11'", "tomli-w"]
 
 setup(
     name="rickled",
     version=about["__version__"],
     description='Tools for pickling Python objects in a completely different way',
     long_description_content_type='text/markdown',
     long_description=long_description,
```

### Comparing `rickled-1.1.2/tests/unittest/test_advanced.py` & `rickled-1.1.3/tests/unittest/test_advanced.py`

 * *Files identical despite different names*

### Comparing `rickled-1.1.2/tests/unittest/test_object_rickler.py` & `rickled-1.1.3/tests/unittest/test_object_rickler.py`

 * *Files identical despite different names*

### Comparing `rickled-1.1.2/tests/unittest/test_rickle.py` & `rickled-1.1.3/tests/unittest/test_rickle.py`

 * *Files 2% similar despite different names*

```diff
@@ -447,8 +447,30 @@
         self.assertTrue(True)
 
     def test_load_from_url(self):
         url = 'https://official-joke-api.appspot.com/random_joke'
 
         r = Rickle(url)
 
-        self.assertTrue(True)
+        self.assertTrue(True)
+
+
+    def test_toml_load(self):
+
+        toml_str = """
+[[players]]
+name = "Lehtinen"
+number = 26
+
+[[players]]
+name = "Numminen"
+number = 27
+        """
+
+
+        rick = BaseRickle(toml_str)
+
+        expected_dict = {
+            "players": [{"name": "Lehtinen", "number": 26}, {"name": "Numminen", "number": 27}]
+        }
+
+        self.assertDictEqual(rick.dict(), expected_dict)
```

### Comparing `rickled-1.1.2/tests/unittest/test_schema_tool.py` & `rickled-1.1.3/tests/unittest/test_schema_tool.py`

 * *Files identical despite different names*

