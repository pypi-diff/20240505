# Comparing `tmp/coherent_build-0.1.1.tar.gz` & `tmp/coherent_build-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coherent_build-0.1.1.tar", last modified: Thu May  2 16:07:03 2024, max compression
+gzip compressed data, was "coherent_build-0.2.0.tar", last modified: Sat May  4 23:45:39 2024, max compression
```

## Comparing `coherent_build-0.1.1.tar` & `coherent_build-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,16 @@
-drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-02 15:29:00.932139 coherent_build-0.1.1/
--rw-r--r--   0 jaraco     (501) staff       (20)     6148 2024-05-02 15:28:09.027061 coherent_build-0.1.1/.DS_Store
--rw-r--r--   0 jaraco     (501) staff       (20)     3757 2024-05-02 16:03:50.243978 coherent_build-0.1.1/__init__.py
--rw-r--r--   0 jaraco     (501) staff       (20)      495 2024-05-02 02:13:39.559121 coherent_build-0.1.1/__main__.py
--rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-05-02 15:12:07.306572 coherent_build-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       58 2024-05-02 16:07:03.560052 coherent_build-0.1.1/PKG-INFO
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-04 23:38:36.570179 coherent_build-0.2.0/
+-rw-r--r--   0 jaraco     (501) staff       (20)     6148 2024-05-02 15:28:09.027061 coherent_build-0.2.0/.DS_Store
+drwx------   0 jaraco     (501) staff       (20)        0 2024-05-04 14:50:05.883440 coherent_build-0.2.0/.pytest_cache/
+-rw-r--r--   0 jaraco     (501) staff       (20)       37 2024-05-04 14:50:05.883209 coherent_build-0.2.0/.pytest_cache/.gitignore
+-rw-r--r--   0 jaraco     (501) staff       (20)      191 2024-05-04 14:50:05.883265 coherent_build-0.2.0/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0 jaraco     (501) staff       (20)      302 2024-05-04 14:50:05.883131 coherent_build-0.2.0/.pytest_cache/README.md
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-04 14:50:05.883467 coherent_build-0.2.0/.pytest_cache/v/
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-04 14:50:05.883703 coherent_build-0.2.0/.pytest_cache/v/cache/
+-rw-r--r--   0 jaraco     (501) staff       (20)       44 2024-05-04 14:50:22.199138 coherent_build-0.2.0/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0 jaraco     (501) staff       (20)       38 2024-05-04 14:50:22.198661 coherent_build-0.2.0/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0 jaraco     (501) staff       (20)        2 2024-05-04 14:50:22.199390 coherent_build-0.2.0/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0 jaraco     (501) staff       (20)      129 2024-05-04 14:42:38.291197 coherent_build-0.2.0/README.md
+-rw-r--r--   0 jaraco     (501) staff       (20)     6631 2024-05-04 23:44:23.475853 coherent_build-0.2.0/__init__.py
+-rw-r--r--   0 jaraco     (501) staff       (20)      495 2024-05-02 02:13:39.559121 coherent_build-0.2.0/__main__.py
+-rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-05-02 15:12:07.306572 coherent_build-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      362 2024-05-04 23:45:39.363094 coherent_build-0.2.0/PKG-INFO
```

### Comparing `coherent_build-0.1.1/.DS_Store` & `coherent_build-0.2.0/.DS_Store`

 * *Files identical despite different names*

