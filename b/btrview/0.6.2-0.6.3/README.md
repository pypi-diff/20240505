# Comparing `tmp/btrview-0.6.2.tar.gz` & `tmp/btrview-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btrview-0.6.2.tar", last modified: Fri May  3 19:17:20 2024, max compression
+gzip compressed data, was "btrview-0.6.3.tar", last modified: Sun May  5 15:28:05 2024, max compression
```

## Comparing `btrview-0.6.2.tar` & `btrview-0.6.3.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-03 19:17:20.926136 btrview-0.6.2/
--rw-r--r--   0 chris     (1000) chris     (1000)     1069 2024-04-18 05:35:32.000000 btrview-0.6.2/LICENSE.md
--rw-r--r--   0 chris     (1000) chris     (1000)     6296 2024-05-03 19:17:20.926136 btrview-0.6.2/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)     4284 2024-05-03 19:16:33.000000 btrview-0.6.2/README.md
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-03 19:17:20.926136 btrview-0.6.2/btrview/
--rw-r--r--   0 chris     (1000) chris     (1000)       86 2024-05-03 19:17:07.000000 btrview-0.6.2/btrview/__init__.py
--rwxr-xr-x   0 chris     (1000) chris     (1000)     2172 2024-04-18 03:01:25.000000 btrview-0.6.2/btrview/__main__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3665 2024-05-03 19:13:38.000000 btrview-0.6.2/btrview/btr_dict.py
--rw-r--r--   0 chris     (1000) chris     (1000)     7362 2024-04-18 03:01:25.000000 btrview-0.6.2/btrview/btrfs.py
--rw-r--r--   0 chris     (1000) chris     (1000)     6906 2024-05-03 19:13:42.000000 btrview-0.6.2/btrview/rich_output.py
--rw-r--r--   0 chris     (1000) chris     (1000)     5914 2024-05-03 19:13:38.000000 btrview-0.6.2/btrview/subvolume.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1254 2024-04-10 13:31:52.000000 btrview-0.6.2/btrview/utils.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-03 19:17:20.926136 btrview-0.6.2/btrview.egg-info/
--rw-r--r--   0 chris     (1000) chris     (1000)     6296 2024-05-03 19:17:20.000000 btrview-0.6.2/btrview.egg-info/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)      361 2024-05-03 19:17:20.000000 btrview-0.6.2/btrview.egg-info/SOURCES.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        1 2024-05-03 19:17:20.000000 btrview-0.6.2/btrview.egg-info/dependency_links.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       57 2024-05-03 19:17:20.000000 btrview-0.6.2/btrview.egg-info/entry_points.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       64 2024-05-03 19:17:20.000000 btrview-0.6.2/btrview.egg-info/requires.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        8 2024-05-03 19:17:20.000000 btrview-0.6.2/btrview.egg-info/top_level.txt
--rw-r--r--   0 chris     (1000) chris     (1000)     1197 2024-05-03 19:17:07.000000 btrview-0.6.2/pyproject.toml
--rw-r--r--   0 chris     (1000) chris     (1000)       38 2024-05-03 19:17:20.926136 btrview-0.6.2/setup.cfg
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-05 15:28:05.678496 btrview-0.6.3/
+-rw-r--r--   0 chris     (1000) chris     (1000)     1069 2024-04-18 05:35:32.000000 btrview-0.6.3/LICENSE.md
+-rw-r--r--   0 chris     (1000) chris     (1000)     6296 2024-05-05 15:28:05.675163 btrview-0.6.3/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)     4284 2024-05-03 19:16:33.000000 btrview-0.6.3/README.md
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-05 15:28:05.675163 btrview-0.6.3/btrview/
+-rw-r--r--   0 chris     (1000) chris     (1000)       86 2024-05-05 15:27:53.000000 btrview-0.6.3/btrview/__init__.py
+-rwxr-xr-x   0 chris     (1000) chris     (1000)     2172 2024-04-18 03:01:25.000000 btrview-0.6.3/btrview/__main__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     3665 2024-05-05 15:16:06.000000 btrview-0.6.3/btrview/btr_dict.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     7362 2024-04-18 03:01:25.000000 btrview-0.6.3/btrview/btrfs.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     6906 2024-05-05 15:24:51.000000 btrview-0.6.3/btrview/rich_output.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-05 15:28:05.675163 btrview-0.6.3/btrview/scripts/
+-rwxr-xr-x   0 chris     (1000) chris     (1000)     2172 2024-04-18 03:01:25.000000 btrview-0.6.3/btrview/scripts/btrview.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     5914 2024-05-05 13:39:59.000000 btrview-0.6.3/btrview/subvolume.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1254 2024-04-10 13:31:52.000000 btrview-0.6.3/btrview/utils.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-05 15:28:05.675163 btrview-0.6.3/btrview.egg-info/
+-rw-r--r--   0 chris     (1000) chris     (1000)     6296 2024-05-05 15:28:05.000000 btrview-0.6.3/btrview.egg-info/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)      388 2024-05-05 15:28:05.000000 btrview-0.6.3/btrview.egg-info/SOURCES.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        1 2024-05-05 15:28:05.000000 btrview-0.6.3/btrview.egg-info/dependency_links.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)       57 2024-05-05 15:28:05.000000 btrview-0.6.3/btrview.egg-info/entry_points.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)       64 2024-05-05 15:28:05.000000 btrview-0.6.3/btrview.egg-info/requires.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        8 2024-05-05 15:28:05.000000 btrview-0.6.3/btrview.egg-info/top_level.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)     1215 2024-05-05 15:27:53.000000 btrview-0.6.3/pyproject.toml
+-rw-r--r--   0 chris     (1000) chris     (1000)       38 2024-05-05 15:28:05.678496 btrview-0.6.3/setup.cfg
```

### Comparing `btrview-0.6.2/LICENSE.md` & `btrview-0.6.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `btrview-0.6.2/PKG-INFO` & `btrview-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btrview
-Version: 0.6.2
+Version: 0.6.3
 Summary: View btrfs snapshot trees
 Author: Chris Copley
 License: MIT License
         
         Copyright (c) 2024 Chris Copley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `btrview-0.6.2/README.md` & `btrview-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `btrview-0.6.2/btrview/__main__.py` & `btrview-0.6.3/btrview/__main__.py`

 * *Files identical despite different names*

### Comparing `btrview-0.6.2/btrview/btr_dict.py` & `btrview-0.6.3/btrview/btr_dict.py`

 * *Files identical despite different names*

### Comparing `btrview-0.6.2/btrview/btrfs.py` & `btrview-0.6.3/btrview/btrfs.py`

 * *Files identical despite different names*

### Comparing `btrview-0.6.2/btrview/rich_output.py` & `btrview-0.6.3/btrview/rich_output.py`

 * *Files identical despite different names*

### Comparing `btrview-0.6.2/btrview/subvolume.py` & `btrview-0.6.3/btrview/subvolume.py`

 * *Files identical despite different names*

### Comparing `btrview-0.6.2/btrview/utils.py` & `btrview-0.6.3/btrview/utils.py`

 * *Files identical despite different names*

### Comparing `btrview-0.6.2/btrview.egg-info/PKG-INFO` & `btrview-0.6.3/btrview.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btrview
-Version: 0.6.2
+Version: 0.6.3
 Summary: View btrfs snapshot trees
 Author: Chris Copley
 License: MIT License
         
         Copyright (c) 2024 Chris Copley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `btrview-0.6.2/pyproject.toml` & `btrview-0.6.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "btrview"
-version = "0.6.2"
+version = "0.6.3"
 description = "View btrfs snapshot trees"
 readme = "README.md"
 authors = [{name = "Chris Copley"}]
 license = {file = "LICENSE.md"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -29,24 +29,24 @@
 Issues = "https://github.com/CopOnTheRun/btrview/issues"
 
 [build-system]
 requires      = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.bumpver]
-current_version = "0.6.2"
+current_version = "0.6.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.setuptools]
-packages = ["btrview"]
+packages = ["btrview","btrview.scripts"]
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
     'current_version = "{version}"',
     'version = "{version}"',
 ]
 "btrview/__init__.py" = ["{version}"]
```

