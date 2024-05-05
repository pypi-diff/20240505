# Comparing `tmp/rfproto-0.0.2.tar.gz` & `tmp/rfproto-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfproto-0.0.2.tar", last modified: Thu Apr 25 02:13:44 2024, max compression
+gzip compressed data, was "rfproto-0.0.6.tar", last modified: Sun May  5 21:02:25 2024, max compression
```

## Comparing `rfproto-0.0.2.tar` & `rfproto-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:13:44.243052 rfproto-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-25 02:13:35.000000 rfproto-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-25 02:13:44.239052 rfproto-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-25 02:13:35.000000 rfproto-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-25 02:13:35.000000 rfproto-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:13:44.239052 rfproto-0.0.2/rfproto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 02:13:35.000000 rfproto-0.0.2/rfproto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-25 02:13:35.000000 rfproto-0.0.2/rfproto/hello.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:13:44.239052 rfproto-0.0.2/rfproto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-25 02:13:44.000000 rfproto-0.0.2/rfproto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-25 02:13:44.000000 rfproto-0.0.2/rfproto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 02:13:44.000000 rfproto-0.0.2/rfproto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-25 02:13:44.000000 rfproto-0.0.2/rfproto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 02:13:44.000000 rfproto-0.0.2/rfproto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 02:13:44.243052 rfproto-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:02:25.128839 rfproto-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-05 21:02:20.000000 rfproto-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-05 21:02:25.128839 rfproto-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-05 21:02:20.000000 rfproto-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-05 21:02:20.000000 rfproto-0.0.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:02:25.124839 rfproto-0.0.6/rfproto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 21:02:20.000000 rfproto-0.0.6/rfproto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-05 21:02:20.000000 rfproto-0.0.6/rfproto/hello.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:02:25.124839 rfproto-0.0.6/rfproto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-05 21:02:25.000000 rfproto-0.0.6/rfproto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-05 21:02:25.000000 rfproto-0.0.6/rfproto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 21:02:25.000000 rfproto-0.0.6/rfproto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-05 21:02:25.000000 rfproto-0.0.6/rfproto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-05 21:02:25.000000 rfproto-0.0.6/rfproto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 21:02:25.128839 rfproto-0.0.6/setup.cfg
```

### Comparing `rfproto-0.0.2/LICENSE` & `rfproto-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rfproto-0.0.2/pyproject.toml` & `rfproto-0.0.6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -3,29 +3,45 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools-git-versioning]
 enabled = true
 
 [project]
 name = "rfproto"
+description = "Python for RF and SDR prototyping."
 dynamic = ["version"]
 authors = [
   { name="John Gentile", email="johncgentile17@gmail.com" },
 ]
-dependencies = [
-  "numpy",
-  "matplotlib",
-  "scipy",
-]
-description = "Python for RF and SDR prototyping."
 keywords = ["RF", "SDR", "prototyping"]
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
+dependencies = [
+  "numpy",
+  "matplotlib",
+  "scipy",
+]
+
+[project.optional-dependencies]
+docs = [
+  "mkdocs",
+  "mkdocstrings[python]",
+  "mkdocs-material",
+]
+test = [
+  "black",
+  "mypy",
+  "pytest",
+  "pytest-cov",
+]
+
 [project.urls]
 Homepage = "https://github.com/JohnnyGOX17/rfproto"
+Documentation = "https://johnnygox17.github.io/rfproto/"
 Issues = "https://github.com/JohnnyGOX17/rfproto/issues"
+Repository = "https://github.com/JohnnyGOX17/rfproto.git"
```

