# Comparing `tmp/coherent_build-0.2.0.tar.gz` & `tmp/coherent_build-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coherent_build-0.2.0.tar", last modified: Sat May  4 23:45:39 2024, max compression
+gzip compressed data, was "coherent_build-0.2.1.tar", last modified: Sun May  5 13:53:55 2024, max compression
```

## Comparing `coherent_build-0.2.0.tar` & `coherent_build-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-04 23:38:36.570179 coherent_build-0.2.0/
--rw-r--r--   0 jaraco     (501) staff       (20)     6148 2024-05-02 15:28:09.027061 coherent_build-0.2.0/.DS_Store
-drwx------   0 jaraco     (501) staff       (20)        0 2024-05-04 14:50:05.883440 coherent_build-0.2.0/.pytest_cache/
--rw-r--r--   0 jaraco     (501) staff       (20)       37 2024-05-04 14:50:05.883209 coherent_build-0.2.0/.pytest_cache/.gitignore
--rw-r--r--   0 jaraco     (501) staff       (20)      191 2024-05-04 14:50:05.883265 coherent_build-0.2.0/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0 jaraco     (501) staff       (20)      302 2024-05-04 14:50:05.883131 coherent_build-0.2.0/.pytest_cache/README.md
-drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-04 14:50:05.883467 coherent_build-0.2.0/.pytest_cache/v/
-drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-04 14:50:05.883703 coherent_build-0.2.0/.pytest_cache/v/cache/
--rw-r--r--   0 jaraco     (501) staff       (20)       44 2024-05-04 14:50:22.199138 coherent_build-0.2.0/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0 jaraco     (501) staff       (20)       38 2024-05-04 14:50:22.198661 coherent_build-0.2.0/.pytest_cache/v/cache/nodeids
--rw-r--r--   0 jaraco     (501) staff       (20)        2 2024-05-04 14:50:22.199390 coherent_build-0.2.0/.pytest_cache/v/cache/stepwise
--rw-r--r--   0 jaraco     (501) staff       (20)      129 2024-05-04 14:42:38.291197 coherent_build-0.2.0/README.md
--rw-r--r--   0 jaraco     (501) staff       (20)     6631 2024-05-04 23:44:23.475853 coherent_build-0.2.0/__init__.py
--rw-r--r--   0 jaraco     (501) staff       (20)      495 2024-05-02 02:13:39.559121 coherent_build-0.2.0/__main__.py
--rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-05-02 15:12:07.306572 coherent_build-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      362 2024-05-04 23:45:39.363094 coherent_build-0.2.0/PKG-INFO
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-05 13:41:58.251794 coherent_build-0.2.1/
+-rw-r--r--   0 jaraco     (501) staff       (20)     6148 2024-05-02 15:28:09.027061 coherent_build-0.2.1/.DS_Store
+drwx------   0 jaraco     (501) staff       (20)        0 2024-05-04 14:50:05.883440 coherent_build-0.2.1/.pytest_cache/
+-rw-r--r--   0 jaraco     (501) staff       (20)       37 2024-05-04 14:50:05.883209 coherent_build-0.2.1/.pytest_cache/.gitignore
+-rw-r--r--   0 jaraco     (501) staff       (20)      191 2024-05-04 14:50:05.883265 coherent_build-0.2.1/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0 jaraco     (501) staff       (20)      302 2024-05-04 14:50:05.883131 coherent_build-0.2.1/.pytest_cache/README.md
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-04 14:50:05.883467 coherent_build-0.2.1/.pytest_cache/v/
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-04 14:50:05.883703 coherent_build-0.2.1/.pytest_cache/v/cache/
+-rw-r--r--   0 jaraco     (501) staff       (20)        2 2024-05-05 13:52:14.326103 coherent_build-0.2.1/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0 jaraco     (501) staff       (20)       38 2024-05-05 13:52:14.325637 coherent_build-0.2.1/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0 jaraco     (501) staff       (20)        2 2024-05-05 13:52:14.326323 coherent_build-0.2.1/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0 jaraco     (501) staff       (20)      129 2024-05-04 14:42:38.291197 coherent_build-0.2.1/README.md
+-rw-r--r--   0 jaraco     (501) staff       (20)     6962 2024-05-05 13:52:41.339984 coherent_build-0.2.1/__init__.py
+-rw-r--r--   0 jaraco     (501) staff       (20)      495 2024-05-02 02:13:39.559121 coherent_build-0.2.1/__main__.py
+-rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-05-02 15:12:07.306572 coherent_build-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       58 2024-05-05 13:53:55.201039 coherent_build-0.2.1/PKG-INFO
```

### Comparing `coherent_build-0.2.0/.DS_Store` & `coherent_build-0.2.1/.DS_Store`

 * *Files identical despite different names*

### Comparing `coherent_build-0.2.0/__init__.py` & `coherent_build-0.2.1/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,27 +3,31 @@
     "pip-run",
     "setuptools_scm",
     "build",
     "git-fame",
     "jaraco.context",
 ]
 
+import functools
 import importlib.metadata
 import io
 import json
 import mimetypes
 import os
 import pathlib
 import posixpath
 import re
 import subprocess
 import tarfile
 import time
 import types
+
+from collections.abc import Mapping
 from email.message import Message
+from typing import Iterable
 
 import setuptools_scm
 from wheel.wheelfile import WheelFile
 from pip_run import scripts
 from jaraco.context import suppress
 
 
@@ -160,27 +164,39 @@
             {**name_contrib, **email_contrib}
             for name_contrib, email_contrib in zip(names_contribs, emails_contribs)
         )
     )
     return next(contribs).combined_detail
 
 
+@functools.singledispatch
+def always_items(
+    values: Mapping | Iterable[tuple[str, str]],
+) -> Iterable[tuple[str, str]]:
+    return values
+
+
+@always_items.register
+def _(values: Mapping) -> Iterable[tuple[str, str]]:
+    return values.items()
+
+
 class Metadata(Message):
     """
     >>> md = Metadata.discover()
     >>> md['Summary']
     'A zero-config Python project build backend'
     """
 
     def __init__(self, values):
         super().__init__()
         if isinstance(values, Message):
             self._headers = values._headers
             return
-        for item in dict(values).items():
+        for item in always_items(values):
             self.add_header(*item)
 
     def _description_in_payload(self):
         if "Description" in self:
             self.set_payload(self["Description"])
             del self["Description"]
```

