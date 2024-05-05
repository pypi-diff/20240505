# Comparing `tmp/string_fixer-0.1.0.tar.gz` & `tmp/string_fixer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "string_fixer-0.1.0.tar", last modified: Sun Apr 28 21:12:05 2024, max compression
+gzip compressed data, was "string_fixer-0.2.0.tar", last modified: Sun May  5 10:45:12 2024, max compression
```

## Comparing `string_fixer-0.1.0.tar` & `string_fixer-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:12:05.490187 string_fixer-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-28 21:12:05.490187 string_fixer-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-28 21:12:03.000000 string_fixer-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-28 21:11:49.000000 string_fixer-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 21:12:05.490187 string_fixer-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:12:05.486187 string_fixer-0.1.0/string_fixer/
--rw-r--r--   0 runner    (1001) docker     (127)    10230 2024-04-28 21:11:49.000000 string_fixer-0.1.0/string_fixer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-28 21:11:49.000000 string_fixer-0.1.0/string_fixer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-28 21:11:49.000000 string_fixer-0.1.0/string_fixer/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:12:05.486187 string_fixer-0.1.0/string_fixer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-28 21:12:05.000000 string_fixer-0.1.0/string_fixer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-28 21:12:05.000000 string_fixer-0.1.0/string_fixer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 21:12:05.000000 string_fixer-0.1.0/string_fixer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-28 21:12:05.000000 string_fixer-0.1.0/string_fixer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-28 21:12:05.000000 string_fixer-0.1.0/string_fixer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:12:05.486187 string_fixer-0.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-28 21:11:49.000000 string_fixer-0.1.0/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:45:12.606168 string_fixer-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-05-05 10:45:12.606168 string_fixer-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-05 10:45:10.000000 string_fixer-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-05 10:44:55.000000 string_fixer-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 10:45:12.606168 string_fixer-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:45:12.606168 string_fixer-0.2.0/string_fixer/
+-rw-r--r--   0 runner    (1001) docker     (127)     9083 2024-05-05 10:44:55.000000 string_fixer-0.2.0/string_fixer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-05 10:44:55.000000 string_fixer-0.2.0/string_fixer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-05 10:44:55.000000 string_fixer-0.2.0/string_fixer/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-05-05 10:44:55.000000 string_fixer-0.2.0/string_fixer/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:45:12.606168 string_fixer-0.2.0/string_fixer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-05-05 10:45:12.000000 string_fixer-0.2.0/string_fixer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-05 10:45:12.000000 string_fixer-0.2.0/string_fixer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 10:45:12.000000 string_fixer-0.2.0/string_fixer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-05 10:45:12.000000 string_fixer-0.2.0/string_fixer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-05 10:45:12.000000 string_fixer-0.2.0/string_fixer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:45:12.606168 string_fixer-0.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-05 10:44:55.000000 string_fixer-0.2.0/test/test_main.py
```

### Comparing `string_fixer-0.1.0/PKG-INFO` & `string_fixer-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: string_fixer
-Version: 0.1.0
+Version: 0.2.0
 Summary: Change quote style in Python files
 Author-email: Crozzers <captaincrozzers@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/Crozzers/string-fixer
 Project-URL: Issues, https://github.com/Crozzers/string-fixer/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -65,16 +65,29 @@
 [tool.string-fixer]
 # file or folder to format
 target = "./"
 # set to true to print planned changes but not modify any files (overrides `output` config)
 dry_run = false
 # write a copy of the files to this directory, rather than modifying them inplace
 output = "./"
-# list of glob patterns for files to ignore
-ignore = []
+# list of glob patterns for files to ignore. this value is autopopulated from `.gitignore` files as well
+# as a few default values. anything you put in this list will be added to this set, rather than replacing
+# it. Use the `include` option to override
+ignore = [
+    # these are the defaults
+    "./**/.*",
+    "./**/site-packages",
+    "./**/node_modules",
+    "./**/build",
+    "./**/dist",
+    "./**/__pycache__",
+    "./**/venv"
+]
+# list of glob patterns for files to include. This setting overrides `ignore`
+include = []
 # extend and override options in another pyproject.toml file
 extends = ""
 # python version to target for compatibility (defaults to current python version)
 # this must be a string because `float("3.10") == 3.1`
 target_version = "3.12"
 ```
```

### Comparing `string_fixer-0.1.0/README.md` & `string_fixer-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -34,16 +34,29 @@
 [tool.string-fixer]
 # file or folder to format
 target = "./"
 # set to true to print planned changes but not modify any files (overrides `output` config)
 dry_run = false
 # write a copy of the files to this directory, rather than modifying them inplace
 output = "./"
-# list of glob patterns for files to ignore
-ignore = []
+# list of glob patterns for files to ignore. this value is autopopulated from `.gitignore` files as well
+# as a few default values. anything you put in this list will be added to this set, rather than replacing
+# it. Use the `include` option to override
+ignore = [
+    # these are the defaults
+    "./**/.*",
+    "./**/site-packages",
+    "./**/node_modules",
+    "./**/build",
+    "./**/dist",
+    "./**/__pycache__",
+    "./**/venv"
+]
+# list of glob patterns for files to include. This setting overrides `ignore`
+include = []
 # extend and override options in another pyproject.toml file
 extends = ""
 # python version to target for compatibility (defaults to current python version)
 # this must be a string because `float("3.10") == 3.1`
 target_version = "3.12"
 ```
```

### Comparing `string_fixer-0.1.0/pyproject.toml` & `string_fixer-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `string_fixer-0.1.0/string_fixer/__init__.py` & `string_fixer-0.2.0/string_fixer/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,17 @@
 import os
 import re
 import sys
-from functools import lru_cache
 from pathlib import Path
-from typing import Dict, List, Optional, TypedDict, Union
+from typing import Dict, List, Optional
 
 import libcst as cst
-import tomli
 from libcst import FormattedString, parse_module
 
-
-class Config(TypedDict):
-    target: Path
-    dry_run: bool
-    output: Optional[Path]
-    ignore: Optional[List[Path]]
-    extends: Optional[Path]
-    target_version: Optional[str]
-
-
-DEFAULT_CONFIG: Config = {
-    'target': Path('./'),
-    'dry_run': False,
-    'output': None,
-    'ignore': None,
-    'extends': None,
-    'target_version': f'{sys.version_info.major}.{sys.version_info.minor}'
-}
+from .config import Config
 
 
 def version_lt(a: str, b: str):
     '''
     Minimal version check for python versions
 
     Returns:
@@ -67,44 +48,46 @@
             original_node: the node being visited
             updated_node: a deep clone of `original_node` where transformations can be applied
             quote_override: override what kind of quote we are assigning to the string. Useful for
                 nested f-strings where quote re-use is not allowed
         '''
         quote = quote_override or '\''
         anti = '\'' if quote[0] == '"' else '"'
+        prefix = original_node.prefix
         quote_len = max(len(quote), len(updated_node.quote))
 
         if anti not in original_node.quote:
             return updated_node
 
         # remove start and end quotes
-        text = updated_node.value[len(updated_node.quote) : -len(updated_node.quote)]
+        text = updated_node.value[len(updated_node.quote) + len(prefix) : -len(updated_node.quote)]
 
         text = re.sub(
             r'(\\*)(["\']{%d,})' % quote_len,
             self._escape_quote,
             text,
             flags=re.MULTILINE,
         )
 
         new_quote = quote[0] * quote_len
-        return updated_node.with_changes(value=f'{new_quote}{text}{new_quote}')
+        return updated_node.with_changes(value=f'{prefix}{new_quote}{text}{new_quote}')
 
     def leave_FormattedString(
         self, original_node: cst.FormattedString, updated_node: cst.FormattedString,
-        depth = 1, meta: Dict[str, int] = {}
+        depth = 1, meta: Optional[Dict[str, int]] = None
     ) -> cst.BaseExpression:
         '''
         Args:
             original_node: the node being visited
             updated_node: a deep clone of `original_node` where transformations can be applied
             depth: current recursion depth
             meta: dict used to keep track of info across recursions (eg: max recursion depth)
                 without corrupting the return signature
         '''
+        meta = meta if meta is not None else {}
         meta['max_depth'] = max(meta.get('max_depth', 1), depth)
 
         def get_quote(depth):
             '''Get appropriate quote given the f-string nest depth'''
             if meta['max_depth'] <= 2:
                 quote_order = ['\'', '"']
             elif meta['max_depth'] == 3:
@@ -150,117 +133,60 @@
                         if not isinstance(slice.slice, cst.Index):
                             new_slices.append(slice)
                             continue
 
                         value = slice.slice.value
                         new_value = value
                         if isinstance(value, cst.SimpleString):
+                            # bump max_depth because simple string is another layer
+                            meta['max_depth'] = max(meta.get('max_depth', 1), depth + 1)
                             new_value = self.leave_SimpleString(
                                 value, value.deep_clone(), get_quote(depth + 1)
                             )
                         elif isinstance(value, FormattedString):
                             new_value = self.leave_FormattedString(
-                                value, value.deep_clone()
+                                value, value.deep_clone(), depth + 1, meta
                             )
 
                         new_slices.append(slice.with_changes(
                             slice=slice.slice.with_changes(
                                 value=new_value
                             )
                         ))
                     new_parts.append(
                         part.with_changes(
                             expression=expression.with_changes(slice=new_slices)
                         )
                     )
                 elif isinstance(expression, cst.SimpleString):
+                    # bump max_depth because simple string is another layer
+                    meta['max_depth'] = max(meta.get('max_depth', 1), depth + 1)
                     new_parts.append(
                         part.with_changes(
                             expression=self.leave_SimpleString(
                                 expression, expression.deep_clone(), get_quote(depth + 1)
                             )
                         )
                     )
                 else:
                     new_parts.append(part)
             else:
                 new_parts.append(part)
 
         quote = get_quote(depth)
-        return updated_node.with_changes(parts=new_parts, start=f'f{quote}', end=quote)
+        return updated_node.with_changes(parts=new_parts, start=f'{original_node.prefix}{quote}', end=quote)
 
 
 def replace_quotes(code: str, target_python: Optional[str] = None) -> str:
     module = parse_module(code)
     transformer = QuoteTransformer(target_python)
     modified_module = module.visit(transformer)
     return modified_module.code
 
 
-def load_config_from_file(file: Path) -> Union[Config, None]:
-    if not file.exists():
-        return
-
-    with open(file, 'rb') as f:
-        toml = tomli.load(f)
-    if 'tool' not in toml or 'string-fixer' not in toml['tool']:
-        return
-
-    config = toml['tool']['string-fixer']
-
-    if extends := config.get('extends', None):
-        extends = (file.parent / extends).resolve()
-        config['extends'] = extends
-        extends = extends.parent if extends.is_file() else extends
-
-        config = {**load_config_from_dir(extends), **config}
-
-    for key, value in DEFAULT_CONFIG.items():
-        config.setdefault(key, value)
-
-    if target := config.get('target'):
-        config['target'] = (file.parent / target).resolve()
-
-    if output := config.get('output'):
-        config['output'] = (file.parent / output).resolve()
-
-    if config.get('ignore', []):
-        ignore = []
-        for pattern in config['ignore']:
-            ignore.extend(file.parent.glob(pattern))
-        config['ignore'] = ignore
-
-    if target_version := config.get('target_version', None):
-        if not isinstance(target_version, str):
-            raise TypeError('target_version must be string')
-
-    return config  # type: ignore
-
-
-@lru_cache
-def load_config_from_dir(path: Path, limit: Optional[Path] = None) -> Config:
-    '''
-    Loads closest config file to `path` in directory tree, up to `limit`.
-
-    Args:
-        path: The dir to start from when loading config files
-        limit: Don't go higher than this dir
-
-    Returns:
-        Config from closest config file, or default config if N/A
-    '''
-    path = path.parent if path.is_file() else path
-    file = path / 'pyproject.toml'
-    if config := load_config_from_file(file):
-        return config
-    if limit and path != limit:
-        return load_config_from_dir(path.parent)
-    return DEFAULT_CONFIG
-
-
 def process_file(file: Path, config: Config, base_dir: Optional[Path] = None):
     assert file.is_file()
     base_dir = base_dir or file.parent
     print('Processing:', file)
     print('Conf', config)
     with open(file) as f:
         code = f.read()
@@ -274,7 +200,29 @@
     else:
         if config['output']:
             file = Path(config['output']).joinpath(*file.parts[len(base_dir.parts) :])
             print('Writing to:', file)
             os.makedirs(file.parent, exist_ok=True)
         with open(file, 'w') as f:
             f.write(modified)
+
+
+def file_is_ignored(file: Path, ignore: Optional[List[Path]], include: Optional[List[Path]]):
+    file = file.absolute()
+    is_ignored = False
+    is_included = False
+
+    if ignore:
+        for ignore_path in ignore:
+            ignore_path = ignore_path.absolute()
+            if ignore_path == file or ignore_path in file.parents:
+                is_ignored = True
+                break
+
+    if include:
+        for include_path in include:
+            include_path = include_path.absolute()
+            if include_path == file or include_path in file.parents:
+                is_included = True
+                break
+
+    return is_ignored and not is_included
```

### Comparing `string_fixer-0.1.0/string_fixer/__main__.py` & `string_fixer-0.2.0/string_fixer/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import argparse
 import os
 import sys
 from pathlib import Path
 
-from . import load_config_from_dir, process_file
+from . import file_is_ignored, process_file
 from ._version import __version__
+from .config import load_config_from_dir
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(
         'string-fixer',
         description='Simple tool to replace "double quotes" with \'single quotes\' in Python files',
     )
     parser.add_argument(
@@ -31,14 +32,19 @@
     )
     parser.add_argument(
         '-c',
         '--config-root',
         type=str,
         help='Override base directory to load configs from',
     )
+    parser.add_argument(
+        '--target-version',
+        type=str,
+        help='Python version to target for compatibility'
+    )
     parser.add_argument('--version', action='store_true', help='Print version info')
     args = parser.parse_args()
 
     if args.version:
         print(__version__)
         sys.exit(0)
 
@@ -66,14 +72,16 @@
                 else load_config_from_dir(target, limit=config_root)
             ),
         )
     else:
         for root, _, files in os.walk(target):
             root = Path(root)
             config = load_config_from_dir(root, limit=config_root)
+            if file_is_ignored(root, config['ignore'], config['include']):
+                continue
             for file in files:
                 file = root / file
-                if file in (config.get('ignore') or []):
-                    continue
                 if not file.suffix == '.py':
                     continue
+                if file_is_ignored(file, config['ignore'], config['include']):
+                    continue
                 process_file(file, config, base_dir=target)
```

### Comparing `string_fixer-0.1.0/string_fixer.egg-info/PKG-INFO` & `string_fixer-0.2.0/string_fixer.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: string_fixer
-Version: 0.1.0
+Version: 0.2.0
 Summary: Change quote style in Python files
 Author-email: Crozzers <captaincrozzers@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/Crozzers/string-fixer
 Project-URL: Issues, https://github.com/Crozzers/string-fixer/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -65,16 +65,29 @@
 [tool.string-fixer]
 # file or folder to format
 target = "./"
 # set to true to print planned changes but not modify any files (overrides `output` config)
 dry_run = false
 # write a copy of the files to this directory, rather than modifying them inplace
 output = "./"
-# list of glob patterns for files to ignore
-ignore = []
+# list of glob patterns for files to ignore. this value is autopopulated from `.gitignore` files as well
+# as a few default values. anything you put in this list will be added to this set, rather than replacing
+# it. Use the `include` option to override
+ignore = [
+    # these are the defaults
+    "./**/.*",
+    "./**/site-packages",
+    "./**/node_modules",
+    "./**/build",
+    "./**/dist",
+    "./**/__pycache__",
+    "./**/venv"
+]
+# list of glob patterns for files to include. This setting overrides `ignore`
+include = []
 # extend and override options in another pyproject.toml file
 extends = ""
 # python version to target for compatibility (defaults to current python version)
 # this must be a string because `float("3.10") == 3.1`
 target_version = "3.12"
 ```
```

