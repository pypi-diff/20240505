# Comparing `tmp/jupyterdartkernel-0.1.0.tar.gz` & `tmp/jupyterdartkernel-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterdartkernel-0.1.0.tar", last modified: Sun May  5 14:28:43 2024, max compression
+gzip compressed data, was "jupyterdartkernel-0.1.1.tar", last modified: Sun May  5 14:30:50 2024, max compression
```

## Comparing `jupyterdartkernel-0.1.0.tar` & `jupyterdartkernel-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-05 14:28:43.065837 jupyterdartkernel-0.1.0/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      248 2024-05-05 14:28:43.065837 jupyterdartkernel-0.1.0/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       36 2024-05-05 14:26:40.000000 jupyterdartkernel-0.1.0/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      457 2024-05-05 14:28:38.000000 jupyterdartkernel-0.1.0/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-05 14:28:43.065837 jupyterdartkernel-0.1.0/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-05 14:28:43.065837 jupyterdartkernel-0.1.0/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-05 14:28:43.065837 jupyterdartkernel-0.1.0/src/jupyterdart/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       23 2024-05-05 14:27:00.000000 jupyterdartkernel-0.1.0/src/jupyterdart/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      151 2024-05-05 14:26:56.000000 jupyterdartkernel-0.1.0/src/jupyterdart/__main__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3609 2024-05-05 14:26:56.000000 jupyterdartkernel-0.1.0/src/jupyterdart/install_kernelspec.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4534 2024-05-05 14:26:56.000000 jupyterdartkernel-0.1.0/src/jupyterdart/kernel.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-05 14:28:43.065837 jupyterdartkernel-0.1.0/src/jupyterdartkernel.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      248 2024-05-05 14:28:43.000000 jupyterdartkernel-0.1.0/src/jupyterdartkernel.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      324 2024-05-05 14:28:43.000000 jupyterdartkernel-0.1.0/src/jupyterdartkernel.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-05 14:28:43.000000 jupyterdartkernel-0.1.0/src/jupyterdartkernel.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       12 2024-05-05 14:28:43.000000 jupyterdartkernel-0.1.0/src/jupyterdartkernel.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-05 14:30:50.275835 jupyterdartkernel-0.1.1/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      248 2024-05-05 14:30:50.275835 jupyterdartkernel-0.1.1/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       36 2024-05-05 14:26:40.000000 jupyterdartkernel-0.1.1/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      457 2024-05-05 14:30:48.000000 jupyterdartkernel-0.1.1/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-05 14:30:50.275835 jupyterdartkernel-0.1.1/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-05 14:30:50.275835 jupyterdartkernel-0.1.1/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-05 14:30:50.275835 jupyterdartkernel-0.1.1/src/jupyterdartkernel/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       23 2024-05-05 14:27:00.000000 jupyterdartkernel-0.1.1/src/jupyterdartkernel/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      151 2024-05-05 14:26:56.000000 jupyterdartkernel-0.1.1/src/jupyterdartkernel/__main__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3609 2024-05-05 14:26:56.000000 jupyterdartkernel-0.1.1/src/jupyterdartkernel/install_kernelspec.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4534 2024-05-05 14:26:56.000000 jupyterdartkernel-0.1.1/src/jupyterdartkernel/kernel.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-05 14:30:50.275835 jupyterdartkernel-0.1.1/src/jupyterdartkernel.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      248 2024-05-05 14:30:50.000000 jupyterdartkernel-0.1.1/src/jupyterdartkernel.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      348 2024-05-05 14:30:50.000000 jupyterdartkernel-0.1.1/src/jupyterdartkernel.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-05 14:30:50.000000 jupyterdartkernel-0.1.1/src/jupyterdartkernel.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       18 2024-05-05 14:30:50.000000 jupyterdartkernel-0.1.1/src/jupyterdartkernel.egg-info/top_level.txt
```

### Comparing `jupyterdartkernel-0.1.0/src/jupyterdart/install_kernelspec.py` & `jupyterdartkernel-0.1.1/src/jupyterdartkernel/install_kernelspec.py`

 * *Files identical despite different names*

### Comparing `jupyterdartkernel-0.1.0/src/jupyterdart/kernel.py` & `jupyterdartkernel-0.1.1/src/jupyterdartkernel/kernel.py`

 * *Files identical despite different names*

