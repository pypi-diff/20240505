# Comparing `tmp/hugo-0.125.5.tar.gz` & `tmp/hugo-0.125.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugo-0.125.5.tar", last modified: Wed May  1 17:57:58 2024, max compression
+gzip compressed data, was "hugo-0.125.6.tar", last modified: Sun May  5 12:10:51 2024, max compression
```

## Comparing `hugo-0.125.5.tar` & `hugo-0.125.6.tar`

### file list

```diff
@@ -1,16 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:57:58.416972 hugo-0.125.5/
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-05-01 17:57:53.000000 hugo-0.125.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-05-01 17:57:53.000000 hugo-0.125.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 17:57:53.000000 hugo-0.125.5/LICENSE-hugo.txt
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-01 17:57:53.000000 hugo-0.125.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    21575 2024-05-01 17:57:58.416972 hugo-0.125.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19941 2024-05-01 17:57:53.000000 hugo-0.125.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-01 17:57:53.000000 hugo-0.125.5/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:57:58.416972 hugo-0.125.5/hugo/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-01 17:57:53.000000 hugo-0.125.5/hugo/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:57:58.416972 hugo-0.125.5/hugo/binaries/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 17:57:53.000000 hugo-0.125.5/hugo/binaries/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-01 17:57:53.000000 hugo-0.125.5/hugo/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-01 17:57:53.000000 hugo-0.125.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-01 17:57:58.416972 hugo-0.125.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    18799 2024-05-01 17:57:53.000000 hugo-0.125.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:10:51.836034 hugo-0.125.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-05-05 12:10:46.000000 hugo-0.125.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-05 12:10:46.000000 hugo-0.125.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-05 12:10:46.000000 hugo-0.125.6/LICENSE-hugo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-05 12:10:46.000000 hugo-0.125.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    21575 2024-05-05 12:10:51.836034 hugo-0.125.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19941 2024-05-05 12:10:46.000000 hugo-0.125.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-05 12:10:46.000000 hugo-0.125.6/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:10:51.832034 hugo-0.125.6/hugo/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-05 12:10:46.000000 hugo-0.125.6/hugo/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:10:51.836034 hugo-0.125.6/hugo/binaries/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-05 12:10:46.000000 hugo-0.125.6/hugo/binaries/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-05 12:10:46.000000 hugo-0.125.6/hugo/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:10:51.836034 hugo-0.125.6/hugo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21575 2024-05-05 12:10:51.000000 hugo-0.125.6/hugo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-05 12:10:51.000000 hugo-0.125.6/hugo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 12:10:51.000000 hugo-0.125.6/hugo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-05 12:10:51.000000 hugo-0.125.6/hugo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-05 12:10:51.000000 hugo-0.125.6/hugo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-05 12:10:46.000000 hugo-0.125.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-05 12:10:51.836034 hugo-0.125.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    18799 2024-05-05 12:10:46.000000 hugo-0.125.6/setup.py
```

### Comparing `hugo-0.125.5/CODE_OF_CONDUCT.md` & `hugo-0.125.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hugo-0.125.5/LICENSE` & `hugo-0.125.6/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
    1. Definitions.
@@ -183,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2023 Agriya Khetarpal
+   Copyright [yyyy] [name of copyright owner]
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `hugo-0.125.5/LICENSE-hugo.txt` & `hugo-0.125.6/LICENSE-hugo.txt`

 * *Files identical despite different names*

### Comparing `hugo-0.125.5/PKG-INFO` & `hugo-0.125.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugo
-Version: 0.125.5
+Version: 0.125.6
 Summary: Binaries for the Hugo static site generator, installable with pip
 Author-email: Agriya Khetarpal <agriyakhetarpal@outlook.com>
 Maintainer-email: Agriya Khetarpal <agriyakhetarpal@outlook.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/agriyakhetarpal/hugo-python-distributions
 Project-URL: Issues, https://github.com/agriyakhetarpal/hugo-python-distributions/issues
 Project-URL: Changelog, https://github.com/agriyakhetarpal/hugo-python-distributions/releases
```

### Comparing `hugo-0.125.5/README.md` & `hugo-0.125.6/README.md`

 * *Files identical despite different names*

### Comparing `hugo-0.125.5/SECURITY.md` & `hugo-0.125.6/SECURITY.md`

 * *Files identical despite different names*

### Comparing `hugo-0.125.5/hugo/cli.py` & `hugo-0.125.6/hugo/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 hugo: Binaries for the Hugo static site generator, installable with pip
 """
 
 from __future__ import annotations
 
 # Reduce expenses for various imports
 from functools import lru_cache
-from os import execvp, path
+from os import execv, path
 from platform import machine
 from subprocess import check_call
 from sys import argv, maxsize
 from sys import platform as sysplatform
 
 with open(path.join(path.dirname(__file__), "VERSION")) as f:  # noqa: PTH123, PTH120, PTH118
     HUGO_VERSION = f.read().strip()
@@ -66,8 +66,8 @@
     """
     if sysplatform == "win32":
         # execvp broken on Windows, use subprocess instead to not launch a new shell
         print(f"\033[95m{MESSAGE}\033[0m")
         check_call([hugo_executable(), *argv[1:]])
     else:
         print(f"\033[95m{MESSAGE}\033[0m")
-        execvp(hugo_executable(), ["hugo", *argv[1:]])
+        execv(hugo_executable(), ["hugo", *argv[1:]])
```

### Comparing `hugo-0.125.5/pyproject.toml` & `hugo-0.125.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hugo-0.125.5/setup.py` & `hugo-0.125.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import Command, Extension, setup
 from setuptools.command.build_ext import build_ext
 from setuptools.command.build_py import build_py
 from wheel.bdist_wheel import bdist_wheel
 
 # ------ Hugo build configuration and constants ------------------------------------
 
-HUGO_VERSION = "0.125.5"
+HUGO_VERSION = "0.125.6"
 # The Go toolchain will download the tarball into the hugo_cache/ directory.
 # We will point the build command to that location to build Hugo from source
 HUGO_CACHE_DIR = "hugo_cache"
 FILE_EXT = (
     ".exe" if (sys.platform == "win32" or os.environ.get("GOOS") == "windows") else ""
 )
 # The vendor name is used to set the vendorInfo variable in the Hugo binary
```

