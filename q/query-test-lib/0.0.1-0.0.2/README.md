# Comparing `tmp/query_test_lib-0.0.1.tar.gz` & `tmp/query_test_lib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "query_test_lib-0.0.1.tar", last modified: Sat May  4 17:38:41 2024, max compression
+gzip compressed data, was "query_test_lib-0.0.2.tar", last modified: Sun May  5 06:17:39 2024, max compression
```

## Comparing `query_test_lib-0.0.1.tar` & `query_test_lib-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 ankitjangid   (501) staff       (20)        0 2024-05-04 17:38:41.593969 query_test_lib-0.0.1/
--rw-r--r--   0 ankitjangid   (501) staff       (20)      256 2024-05-04 17:38:41.592940 query_test_lib-0.0.1/PKG-INFO
--rw-r--r--   0 ankitjangid   (501) staff       (20)        0 2024-05-04 16:23:17.000000 query_test_lib-0.0.1/README.md
--rw-r--r--   0 ankitjangid   (501) staff       (20)      346 2024-05-04 17:38:33.000000 query_test_lib-0.0.1/pyproject.toml
-drwxr-xr-x   0 ankitjangid   (501) staff       (20)        0 2024-05-04 17:38:41.591906 query_test_lib-0.0.1/query_test_lib.egg-info/
--rw-r--r--   0 ankitjangid   (501) staff       (20)      256 2024-05-04 17:38:41.000000 query_test_lib-0.0.1/query_test_lib.egg-info/PKG-INFO
--rw-r--r--   0 ankitjangid   (501) staff       (20)      213 2024-05-04 17:38:41.000000 query_test_lib-0.0.1/query_test_lib.egg-info/SOURCES.txt
--rw-r--r--   0 ankitjangid   (501) staff       (20)        1 2024-05-04 17:38:41.000000 query_test_lib-0.0.1/query_test_lib.egg-info/dependency_links.txt
--rw-r--r--   0 ankitjangid   (501) staff       (20)       56 2024-05-04 17:38:41.000000 query_test_lib-0.0.1/query_test_lib.egg-info/requires.txt
--rw-r--r--   0 ankitjangid   (501) staff       (20)        1 2024-05-04 17:38:41.000000 query_test_lib-0.0.1/query_test_lib.egg-info/top_level.txt
--rw-r--r--   0 ankitjangid   (501) staff       (20)       38 2024-05-04 17:38:41.594128 query_test_lib-0.0.1/setup.cfg
+drwxr-xr-x   0 ankitjangid   (501) staff       (20)        0 2024-05-05 06:17:39.594123 query_test_lib-0.0.2/
+-rw-r--r--   0 ankitjangid   (501) staff       (20)      302 2024-05-05 06:17:39.592965 query_test_lib-0.0.2/PKG-INFO
+-rw-r--r--   0 ankitjangid   (501) staff       (20)        0 2024-05-04 16:23:17.000000 query_test_lib-0.0.2/README.md
+-rw-r--r--   0 ankitjangid   (501) staff       (20)      375 2024-05-05 06:17:29.000000 query_test_lib-0.0.2/pyproject.toml
+drwxr-xr-x   0 ankitjangid   (501) staff       (20)        0 2024-05-05 06:17:39.591774 query_test_lib-0.0.2/query_test_lib.egg-info/
+-rw-r--r--   0 ankitjangid   (501) staff       (20)      302 2024-05-05 06:17:39.000000 query_test_lib-0.0.2/query_test_lib.egg-info/PKG-INFO
+-rw-r--r--   0 ankitjangid   (501) staff       (20)      213 2024-05-05 06:17:39.000000 query_test_lib-0.0.2/query_test_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 ankitjangid   (501) staff       (20)        1 2024-05-05 06:17:39.000000 query_test_lib-0.0.2/query_test_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 ankitjangid   (501) staff       (20)       72 2024-05-05 06:17:39.000000 query_test_lib-0.0.2/query_test_lib.egg-info/requires.txt
+-rw-r--r--   0 ankitjangid   (501) staff       (20)        1 2024-05-05 06:17:39.000000 query_test_lib-0.0.2/query_test_lib.egg-info/top_level.txt
+-rw-r--r--   0 ankitjangid   (501) staff       (20)       38 2024-05-05 06:17:39.594310 query_test_lib-0.0.2/setup.cfg
```

