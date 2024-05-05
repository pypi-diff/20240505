# Comparing `tmp/fons-0.3.1.tar.gz` & `tmp/fons-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\fons-0.3.1.tar", last modified: Tue Jun  8 09:24:32 2021, max compression
+gzip compressed data, was "fons-0.4.0.tar", last modified: Sun May  5 07:54:30 2024, max compression
```

## Comparing `fons-0.3.1.tar` & `fons-0.4.0.tar`

### file list

```diff
@@ -1,67 +1,73 @@
-drwxrwxrwx   0        0        0        0 2021-06-08 09:24:32.000000 fons-0.3.1/
-drwxrwxrwx   0        0        0        0 2021-06-08 09:24:32.000000 fons-0.3.1/fons/
--rw-rw-rw-   0        0        0     4075 2020-05-02 03:25:56.000000 fons-0.3.1/fons/aio.py
--rw-rw-rw-   0        0        0     3899 2020-12-13 15:05:34.000000 fons-0.3.1/fons/all.py
--rw-rw-rw-   0        0        0     9241 2020-12-13 15:05:34.000000 fons-0.3.1/fons/argv.py
--rw-rw-rw-   0        0        0     3673 2020-05-02 03:26:02.000000 fons-0.3.1/fons/crypto.py
--rw-rw-rw-   0        0        0     5697 2020-05-02 03:25:15.000000 fons-0.3.1/fons/debug.py
--rw-rw-rw-   0        0        0     6394 2020-05-02 03:25:59.000000 fons-0.3.1/fons/dict_ops.py
-drwxrwxrwx   0        0        0        0 2021-06-08 09:24:32.000000 fons-0.3.1/fons/dtype/
--rw-rw-rw-   0        0        0    13912 2020-05-18 19:49:56.000000 fons-0.3.1/fons/dtype/dtype.py
--rw-rw-rw-   0        0        0     6683 2020-05-02 03:25:15.000000 fons-0.3.1/fons/dtype/merging.py
--rw-rw-rw-   0        0        0    16871 2020-05-18 19:07:21.000000 fons-0.3.1/fons/dtype/store.py
--rw-rw-rw-   0        0        0       37 2020-05-02 03:25:15.000000 fons-0.3.1/fons/dtype/__init__.py
--rw-rw-rw-   0        0        0     4992 2020-10-29 16:16:49.000000 fons-0.3.1/fons/errors.py
--rw-rw-rw-   0        0        0    33530 2020-05-02 03:26:06.000000 fons-0.3.1/fons/event.py
--rw-rw-rw-   0        0        0    10429 2020-10-28 12:52:11.000000 fons-0.3.1/fons/fsync.py
--rw-rw-rw-   0        0        0    27209 2020-05-02 03:25:57.000000 fons-0.3.1/fons/func.py
--rw-rw-rw-   0        0        0    19299 2020-12-13 15:05:28.000000 fons-0.3.1/fons/gui.py
--rw-rw-rw-   0        0        0     3154 2020-05-02 03:25:15.000000 fons-0.3.1/fons/host.py
--rw-rw-rw-   0        0        0    21682 2020-09-06 09:12:25.000000 fons-0.3.1/fons/io.py
--rw-rw-rw-   0        0        0    10890 2020-05-02 03:25:55.000000 fons-0.3.1/fons/iter.py
--rw-rw-rw-   0        0        0    28230 2020-12-13 15:05:28.000000 fons-0.3.1/fons/log.py
-drwxrwxrwx   0        0        0        0 2021-06-08 09:24:32.000000 fons-0.3.1/fons/math/
--rw-rw-rw-   0        0        0     2074 2020-05-02 03:26:10.000000 fons-0.3.1/fons/math/graph.py
--rw-rw-rw-   0        0        0     1835 2020-05-02 03:25:15.000000 fons-0.3.1/fons/math/round.py
--rw-rw-rw-   0        0        0    23022 2020-05-18 15:38:57.000000 fons-0.3.1/fons/math/series.py
--rw-rw-rw-   0        0        0       36 2020-05-02 03:25:15.000000 fons-0.3.1/fons/math/__init__.py
--rw-rw-rw-   0        0        0     1713 2020-05-02 03:25:15.000000 fons-0.3.1/fons/nan.py
-drwxrwxrwx   0        0        0        0 2021-06-08 09:24:32.000000 fons-0.3.1/fons/net/
--rw-rw-rw-   0        0        0     9982 2019-11-07 15:11:36.000000 fons-0.3.1/fons/net/url.py
--rw-rw-rw-   0        0        0     7541 2019-11-07 15:09:14.000000 fons-0.3.1/fons/net/urlstr.py
--rw-rw-rw-   0        0        0     2178 2020-04-12 00:55:56.000000 fons-0.3.1/fons/net/__init__.py
--rw-rw-rw-   0        0        0     8468 2021-06-07 08:47:04.000000 fons-0.3.1/fons/os.py
--rw-rw-rw-   0        0        0     3641 2020-05-02 03:25:15.000000 fons-0.3.1/fons/processes.py
--rw-rw-rw-   0        0        0     2860 2020-05-02 03:25:15.000000 fons-0.3.1/fons/py.py
--rw-rw-rw-   0        0        0     5532 2020-05-02 03:25:52.000000 fons-0.3.1/fons/pyops.py
--rw-rw-rw-   0        0        0      881 2020-05-02 03:25:15.000000 fons-0.3.1/fons/reg.py
--rw-rw-rw-   0        0        0    58604 2020-05-02 03:26:04.000000 fons-0.3.1/fons/sched.py
--rw-rw-rw-   0        0        0     5192 2020-05-02 03:25:15.000000 fons-0.3.1/fons/threads.py
--rw-rw-rw-   0        0        0    22052 2020-05-02 03:25:15.000000 fons-0.3.1/fons/time.py
--rw-rw-rw-   0        0        0    62629 2020-10-29 17:05:17.000000 fons-0.3.1/fons/verify.py
--rw-rw-rw-   0        0        0    23363 2020-05-02 03:25:15.000000 fons-0.3.1/fons/verify_old.py
--rw-rw-rw-   0        0        0     1931 2021-06-07 08:47:04.000000 fons-0.3.1/fons/__init__.py
-drwxrwxrwx   0        0        0        0 2021-06-08 09:24:32.000000 fons-0.3.1/fons.egg-info/
--rw-rw-rw-   0        0        0        1 2021-06-08 09:24:31.000000 fons-0.3.1/fons.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2371 2021-06-08 09:24:31.000000 fons-0.3.1/fons.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      118 2021-06-08 09:24:31.000000 fons-0.3.1/fons.egg-info/requires.txt
--rw-rw-rw-   0        0        0      996 2021-06-08 09:24:31.000000 fons-0.3.1/fons.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        5 2021-06-08 09:24:31.000000 fons-0.3.1/fons.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2371 2021-06-08 09:24:32.000000 fons-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1722 2020-05-02 03:25:29.000000 fons-0.3.1/README.md
--rw-rw-rw-   0        0        0       42 2021-06-08 09:24:32.000000 fons-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1004 2021-06-07 08:47:04.000000 fons-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2021-06-08 09:24:32.000000 fons-0.3.1/test/
--rw-rw-rw-   0        0        0      601 2020-05-02 03:25:15.000000 fons-0.3.1/test/test_aio.py
--rw-rw-rw-   0        0        0      735 2019-11-10 14:46:32.000000 fons-0.3.1/test/test_crypto.py
--rw-rw-rw-   0        0        0      410 2020-01-23 23:30:16.000000 fons-0.3.1/test/test_event.py
--rw-rw-rw-   0        0        0     5258 2020-05-02 03:25:15.000000 fons-0.3.1/test/test_func.py
--rw-rw-rw-   0        0        0     6051 2020-08-12 03:50:03.000000 fons-0.3.1/test/test_io.py
--rw-rw-rw-   0        0        0     5502 2020-05-02 03:25:55.000000 fons-0.3.1/test/test_iter.py
--rw-rw-rw-   0        0        0     1228 2020-05-02 03:25:15.000000 fons-0.3.1/test/test_pyops.py
--rw-rw-rw-   0        0        0    10414 2020-05-02 03:25:15.000000 fons-0.3.1/test/test_sched.py
--rw-rw-rw-   0        0        0      586 2020-05-02 03:25:15.000000 fons-0.3.1/test/test_threads.py
--rw-rw-rw-   0        0        0     4454 2020-05-02 03:25:15.000000 fons-0.3.1/test/test_time.py
--rw-rw-rw-   0        0        0     2669 2019-11-07 15:18:46.000000 fons-0.3.1/test/test_url.py
--rw-rw-rw-   0        0        0    19914 2020-10-29 16:16:49.000000 fons-0.3.1/test/test_verify.py
--rw-rw-rw-   0        0        0     9597 2020-05-02 03:25:15.000000 fons-0.3.1/test/test_verify_old.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:54:30.865913 fons-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-05 07:54:27.000000 fons-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-05 07:54:30.865913 fons-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-05 07:54:27.000000 fons-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:54:30.857913 fons-0.4.0/fons/
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-05 07:54:27.000000 fons-0.4.0/fons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-05 07:54:27.000000 fons-0.4.0/fons/aio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-05 07:54:27.000000 fons-0.4.0/fons/all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8592 2024-05-05 07:54:27.000000 fons-0.4.0/fons/argv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-05 07:54:27.000000 fons-0.4.0/fons/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-05-05 07:54:27.000000 fons-0.4.0/fons/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-05-05 07:54:27.000000 fons-0.4.0/fons/dict_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:54:30.861913 fons-0.4.0/fons/dtype/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-05 07:54:27.000000 fons-0.4.0/fons/dtype/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15099 2024-05-05 07:54:27.000000 fons-0.4.0/fons/dtype/dtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6833 2024-05-05 07:54:27.000000 fons-0.4.0/fons/dtype/merging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16954 2024-05-05 07:54:27.000000 fons-0.4.0/fons/dtype/store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-05-05 07:54:27.000000 fons-0.4.0/fons/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32106 2024-05-05 07:54:27.000000 fons-0.4.0/fons/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10146 2024-05-05 07:54:27.000000 fons-0.4.0/fons/fsync.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25852 2024-05-05 07:54:27.000000 fons-0.4.0/fons/func.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19185 2024-05-05 07:54:27.000000 fons-0.4.0/fons/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-05-05 07:54:27.000000 fons-0.4.0/fons/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20474 2024-05-05 07:54:27.000000 fons-0.4.0/fons/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-05-05 07:54:27.000000 fons-0.4.0/fons/iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27631 2024-05-05 07:54:27.000000 fons-0.4.0/fons/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-05-05 07:54:27.000000 fons-0.4.0/fons/log311.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-05 07:54:27.000000 fons-0.4.0/fons/log35.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-05 07:54:27.000000 fons-0.4.0/fons/log38.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:54:30.861913 fons-0.4.0/fons/math/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-05 07:54:27.000000 fons-0.4.0/fons/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-05 07:54:27.000000 fons-0.4.0/fons/math/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-05 07:54:27.000000 fons-0.4.0/fons/math/round.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22941 2024-05-05 07:54:27.000000 fons-0.4.0/fons/math/series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-05 07:54:27.000000 fons-0.4.0/fons/nan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:54:30.861913 fons-0.4.0/fons/net/
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-05 07:54:27.000000 fons-0.4.0/fons/net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10521 2024-05-05 07:54:27.000000 fons-0.4.0/fons/net/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-05-05 07:54:27.000000 fons-0.4.0/fons/net/urlstr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-05-05 07:54:27.000000 fons-0.4.0/fons/os.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-05-05 07:54:27.000000 fons-0.4.0/fons/processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-05-05 07:54:27.000000 fons-0.4.0/fons/py.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-05-05 07:54:27.000000 fons-0.4.0/fons/pyops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-05 07:54:27.000000 fons-0.4.0/fons/reg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57822 2024-05-05 07:54:27.000000 fons-0.4.0/fons/sched.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-05-05 07:54:27.000000 fons-0.4.0/fons/threads.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21572 2024-05-05 07:54:27.000000 fons-0.4.0/fons/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60700 2024-05-05 07:54:27.000000 fons-0.4.0/fons/verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23457 2024-05-05 07:54:27.000000 fons-0.4.0/fons/verify_old.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:54:30.865913 fons-0.4.0/fons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-05 07:54:30.000000 fons-0.4.0/fons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-05 07:54:30.000000 fons-0.4.0/fons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 07:54:30.000000 fons-0.4.0/fons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-05 07:54:30.000000 fons-0.4.0/fons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-05 07:54:30.000000 fons-0.4.0/fons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-05 07:54:27.000000 fons-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 07:54:30.865913 fons-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-05 07:54:27.000000 fons-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:54:30.865913 fons-0.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-05 07:54:27.000000 fons-0.4.0/test/test_aio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-05 07:54:27.000000 fons-0.4.0/test/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-05 07:54:27.000000 fons-0.4.0/test/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-05 07:54:27.000000 fons-0.4.0/test/test_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-05-05 07:54:27.000000 fons-0.4.0/test/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-05-05 07:54:27.000000 fons-0.4.0/test/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-05 07:54:27.000000 fons-0.4.0/test/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-05 07:54:27.000000 fons-0.4.0/test/test_pyops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11023 2024-05-05 07:54:27.000000 fons-0.4.0/test/test_sched.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-05 07:54:27.000000 fons-0.4.0/test/test_threads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-05-05 07:54:27.000000 fons-0.4.0/test/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-05 07:54:27.000000 fons-0.4.0/test/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18758 2024-05-05 07:54:27.000000 fons-0.4.0/test/test_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8513 2024-05-05 07:54:27.000000 fons-0.4.0/test/test_verify_old.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fons-0.3.1/fons/all.py` & `fons-0.4.0/fons/all.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,97 +1,185 @@
 """
     This module is meant to be used as a convenient namespace.
 """
 
-from fons import (__version__, __author__)
+from fons import __version__, __author__
 
 import fons.log as log
-from fons.log import (setup_logging, standard_logging, get_standard_5, 
-                      get_standard_logger, getFonsLogger, multi_module_logging,
-                      quick_logging)
+from fons.log import (
+    setup_logging,
+    standard_logging,
+    get_standard_5,
+    get_standard_logger,
+    getFonsLogger,
+    multi_module_logging,
+    quick_logging,
+)
 
 import fons.gui as gui
-from fons.gui import (TkThread, NbGUI, TkLogiProcessComplex)
+from fons.gui import TkThread, NbGUI, TkLogiProcessComplex
 
 import fons.debug as _debug
-from fons.debug import (debug, set_pm_hook, trylog, asyncTryLog, aTryLog, 
-                        safeTry, safeAsyncTry, safeATry, wrap_trylog,
-                        safewait)
+from fons.debug import (
+    debug,
+    set_pm_hook,
+    trylog,
+    asyncTryLog,
+    aTryLog,
+    safeTry,
+    safeAsyncTry,
+    safeATry,
+    wrap_trylog,
+    safewait,
+)
 
 import fons.aio as aio
 import fons.event as event
 import fons.host as host
 import fons.processes as processes
 import fons.reg as reg
 import fons.sched as sched
 import fons.threads as threads
-from fons.aio import (call_via_loop, call_via_loop_afut, wrap_with_future, lrc)
-from fons.event import (force_put, empty_queue, Station, QueueTransmitter, EventTransmitter,
-                        Node, NodeHandler, RelayInfo, RelayPackage, NodeExit)
+from fons.aio import call_via_loop, call_via_loop_afut, wrap_with_future, lrc
+from fons.event import (
+    force_put,
+    empty_queue,
+    Station,
+    QueueTransmitter,
+    EventTransmitter,
+    Node,
+    NodeHandler,
+    RelayInfo,
+    RelayPackage,
+    NodeExit,
+)
 from fons.host import Server
-from fons.processes import (LogiProcess, TkLogiProcess, pool_processes)
+from fons.processes import LogiProcess, TkLogiProcess, pool_processes
 from fons.reg import create_name
-from fons.sched import (Ticker, TickManager, AsyncTicker, AsyncTickManager,
-                        BaseTicker, AsyncBaseTicker, ScheduleTicker, Routine)
-from fons.threads import (EliThread, LoopingThread)
+from fons.sched import (
+    Ticker,
+    TickManager,
+    AsyncTicker,
+    AsyncTickManager,
+    BaseTicker,
+    AsyncBaseTicker,
+    ScheduleTicker,
+    Routine,
+)
+from fons.threads import EliThread, LoopingThread
 
 import fons.math as math
 import fons.math.graph as graph
 import fons.math.series as series
 import fons.math.round as _round
-from fons.math.round import (round_sd, ignore_half_round, round)
-from fons.math.graph import (find_shortest_path, create_graph)
+from fons.math.round import round_sd, ignore_half_round, round
+from fons.math.graph import find_shortest_path, create_graph
 
 import fons.crypto as crypto
-from fons.crypto import (nonce, nonce_ms, sign, password_encrypt, password_decrypt)
+from fons.crypto import nonce, nonce_ms, sign, password_encrypt, password_decrypt
 
 import fons.argv as argv
 import fons.dict_ops as dict_ops
 import fons.dtype as _dtype
 import fons.dtype.dtype as dtype
 import fons.dtype.merging as merging
 import fons.dtype.store as store
 import fons.iter as iter
 import fons.verify as verify
 
-from fons.argv import (parse_argv, parse_parentheses)
-from fons.dtype.dtype import (DType, ShadowMerger)
-from fons.iter import (flatten, flatten2, flatten_dict, fliter, is_flat, unique, consume,
-                       sequence_insert)
-from fons.dict_ops import (nt_to_od, od_to_nt, apply_until_get, deep_get, deep_update)
-from fons.verify import (init_data, verify_data)
+from fons.argv import parse_argv, parse_parentheses
+from fons.dtype.dtype import DType, ShadowMerger
+from fons.iter import (
+    flatten,
+    flatten2,
+    flatten_dict,
+    fliter,
+    is_flat,
+    unique,
+    consume,
+    sequence_insert,
+)
+from fons.dict_ops import nt_to_od, od_to_nt, apply_until_get, deep_get, deep_update
+from fons.verify import init_data, verify_data
 
 import fons.time as time
-from fons.time import (dt_tuple, dt_indexing, dt_get, dt_assign, dt_round_to_digit,
-                         dt_isround, dt_round, dt_round2, dt_round_freq, dt_synced,
-                         _dt_round_bh, freq_to_td, freq_to_str, freq_to_offset,
-                         dt_round_strf, dt_strp, _set_win_time, get_utctime,
-                         _get_epoch, pydt, pydt_from_ms, timestamp, timestamp_ms,
-                         ctime, ctime_ms, DT_FIELDS, TD_FIELDS, _FREQS, _EPOCH)
+from fons.time import (
+    dt_tuple,
+    dt_indexing,
+    dt_get,
+    dt_assign,
+    dt_round_to_digit,
+    dt_isround,
+    dt_round,
+    dt_round2,
+    ts_round,
+    ms_round,
+    dt_round_freq,
+    dt_synced,
+    _dt_round_bh,
+    freq_to_td,
+    freq_to_str,
+    freq_to_offset,
+    dt_round_strf,
+    dt_strp,
+    _set_win_time,
+    get_utctime,
+    _get_epoch,
+    pydt,
+    pydt_from_ms,
+    timestamp,
+    timestamp_ms,
+    ctime,
+    ctime_ms,
+    DT_FIELDS,
+    TD_FIELDS,
+    _FREQS,
+    _EPOCH,
+)
 
 import fons.io as io
-from fons.io import (DateTimeEncoder, DateTimeEncoderNumeric, 
-                     get_params, read_params, save_params,
-                     wait_filelock, SafeFileLock, update_settings, _META_NORM as META_NORM)
+from fons.io import (
+    DateTimeEncoder,
+    DateTimeEncoderNumeric,
+    get_params,
+    read_params,
+    save_params,
+    wait_filelock,
+    SafeFileLock,
+    update_settings,
+    _META_NORM as META_NORM,
+)
 import fons.os as os
-from fons.os import (search, search_in_file, delete_empty_dirs, make_dirpath, zip_contents)
+from fons.os import (
+    search,
+    search_in_file,
+    delete_empty_dirs,
+    make_dirpath,
+    zip_contents,
+)
 
 
 import fons.net as net
 import fons.net.url as url
 import fons.net.urlstr as urlstr
-from fons.net import (fetch, init_session, get_session, close_sessions)
+from fons.net import fetch, init_session, get_session, close_sessions
 
 
-from fons.func import (limitcalls, limitcalls_f, limitcalls_m,
-                       async_limitcalls, async_limitcalls_f, async_limitcalls_m,
-                       get_arg_count)
+from fons.func import (
+    limitcalls,
+    limitcalls_f,
+    limitcalls_m,
+    async_limitcalls,
+    async_limitcalls_f,
+    async_limitcalls_m,
+    get_arg_count,
+)
 
 import fons.py as py
-from fons.py import (mro, rreload)
+from fons.py import mro, rreload
 
 import fons.pyops as pyops
 from fons.pyops import exec_op
 
 import fons.errors as e
 
-logger,logger2,tlogger,tloggers,tlogger0 = log.get_standard_5(__name__)
+logger, logger2, tlogger, tloggers, tlogger0 = log.get_standard_5(__name__)
```

### Comparing `fons-0.3.1/fons/argv.py` & `fons-0.4.0/fons/argv.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,315 +1,314 @@
-from collections import defaultdict
-import itertools
-import copy as _copy
-
-from fons.iter import unique
-
-
-class Argv:
-    def __init__(self, argv, apply={}):
-        self.argv, self.map, self.non_mapped, self.indexes = \
-                                            self.parse(argv)
-        self.apply(apply, True)
-    
-    
-    @staticmethod
-    def parse(argv):
-        new_argv = []
-        map = {}
-        non_mapped = []
-        indexes = defaultdict(list)
-        i = 0
-        argv = tuple(argv)
-        ln_argv = len(argv)
-        var_count = 0
-        _null = object()
-        
-        while i < ln_argv:
-            x = argv[i]
-            value = _null
-            is_unique = True
-            add_i = 0
-            
-            if x.startswith('--'):
-                x = x[2:]
-            
-            if x.startswith('-'):
-                var = x[1:]
-                try: value = argv[i+1]
-                except IndexError:
-                    raise ValueError('Incorrectly formatted argv: {}'.format(argv))
-                add_i = 1
-            elif '=' in x:
-                j = x.find('=')
-                var, value = x[:j], x[j+1:]
-            else:
-                var = x
-            
-            if value is not _null:
-                is_unique = var not in map
-                map[var] = value
-            else:
-                non_mapped.append(x)
-            
-            is_key = value is not _null
-            add_to_argv = '{}={}'.format(var, value) if is_key else var
-            
-            if not is_unique:
-                raise ValueError('Contains duplicate keyword: {}'.format(var))
-            
-            indexes[var].append((var_count, is_key))
-            var_count += 1
-            new_argv.append(add_to_argv)
-            #else:
-            #    _argv[indexes[var][0]] = add_to_argv
-            i += (1 + add_i)
-            
-             
-        return new_argv, map, non_mapped, indexes
-    
-    
-    def contains(self, *vars, set=None):
-        _sets = {None: (self.map, self.non_mapped),
-                'mapped': (self.map,),
-                'map': (self.map,),
-                'non_mapped': (self.non_mapped,),
-                'non-mapped': (self.non_mapped,),
-                'nonmapped': (self.non_mapped,),}
-            
-        try: sets = _sets[set]
-        except KeyError:
-            raise ValueError(set)
-        
-        return any(any(x in _set for _set in sets) for x in vars)
-    
-    
-    def which(self, vars, default=None, *, set=None):
-        return next((x for x in vars if self.contains(x, set=set)), default)
-    
-    
-    def apply(self, f_map, inplace=True):
-        new_map = self.map.copy() if not inplace else self.map
-        
-        for k,f in f_map.items():
-            if k in new_map:
-                new_map[k] = f(new_map[k])
-
-        return new_map
-    
-    
-    def add(self, var, *value, index=None):
-        _ln = len(value)
-        argv, map, non_mapped, indexes = self._fetch_attrs()
-        
-        if _ln > 2:
-            raise ValueError(value)
-        
-        is_key = (_ln == 1)
-        
-        if is_key:
-            if var in map:
-                if index is None:
-                    index = next(x[0] for x in self.indexes[var] if x[1])
-                self.drop(var, set='mapped')
-            map[var] = value[0]
-            txt = '{}={}'.format(var, value[0])
-        else:
-            non_mapped.append(var)
-            txt = var
-        
-        ln_argv = len(argv)
-        
-        if index is None:
-            index = ln_argv
-        else:
-            index = self._resolve_positions((index,), ln_argv, type='insert')[0]
-
-        argv.insert(index, txt)
-            
-        self._readjust_indexes(var, indexes, ((index, is_key),), 'add')
-            
-        
-    def drop(self, var, *, set=None, position=None):
-        argv, map, non_mapped, indexes = self._fetch_attrs()
-        is_both = set is None
-        is_map = set in ('map','mapped')
-        is_nonmapped = set in ('non_mapped','non-mapped','nonmapped')
-
-        if not self.contains(var, set=set):
-            return
-        
-        eligible = [x for x in indexes[var]
-                    if x[1] and not is_nonmapped or not x[1] and not is_map]
-        
-        s = sorted(eligible, key=lambda x: x[0])
-        
-        if isinstance(position, int):
-            position = (position,)
-            
-        if position is not None:
-            position = self._resolve_positions(position, len(s), type='resolve')
-            s = [s[j] for j in position]
-        
-        s = sorted(s, reverse=True, key=lambda x: x[0])
-        
-        for i, is_key in s:
-            argv.pop(i)
-            if is_key:
-                del map[var]
-            else:
-                non_mapped.remove(var)
-        
-        self._readjust_indexes(var, indexes, s, 'drop')
-    
-    
-    def drop_key(self, var):
-        return self.drop(var, set='key')
-    
-    
-    def drop_value(self, var):
-        return self.drop(self, var, set='value')
-                         
-                
-    @staticmethod
-    def _readjust_indexes(var, indexes, changed, action='add'):
-        if action not in ('add','drop'):
-            raise ValueError(action)
-        is_drop = (action=='drop')
-        diff = -1 if is_drop else 1
-        
-        if is_drop and var in indexes:
-            indexes[var] = [x for x in indexes[var] 
-                            if not any(y[0]==x[0] for y in changed)]
-            if not len(indexes[var]):
-                del indexes[var]
-        
-        for c,is_key in sorted(changed, reverse=True, key=lambda x: x[0]):
-            
-            for inds in list(indexes.values()):
-                for j in range(len(inds)):
-                    index,_is_key = inds[j]
-                    if index >= c:
-                        inds[j] = (index+diff, _is_key)
-                        
-            if not is_drop:
-                indexes[var].append((c, is_key))
-             
-        return indexes
-    
-    
-    @staticmethod
-    def _resolve_positions(positions, length, type='resolve'):
-        if type not in ('resolve','insert'):
-            raise ValueError(type)
-        is_drop = (type=='resolve')
-        diff = 0 if type=='resolve' else -1
-        resolved = []
-        
-        for index in positions:
-            if index > length:
-                if is_drop: continue
-                else: index = length
-            elif index < 0:
-                if index < -length and is_drop:
-                    continue
-                index = max(0, (length+diff)+index)
-            resolved.append(index)
-        
-        return tuple(unique(resolved))
-    
-        
-    def _fetch_attrs(self, copy=False):
-        argv = self.argv[:] if copy else self.argv
-        map = self.map.copy() if copy else self.map
-        non_mapped = self.non_mapped[:] if copy else self.non_mapped
-        indexes = _copy.deepcopy(self.indexes) if copy else self.indexes
-        
-        return argv, map, non_mapped, indexes
-    
-    
-    def copy(self):
-        attr_values = self._fetch_attrs(True)
-        new = Argv([])
-        for a,v in zip(('argv','map','non_mapped','indexes'), attr_values):
-            setattr(new, a, v)
-            
-        return new
-    
-        
-    def __getitem__(self, key):
-        return self.map[key]
-    
-    def __iter__(self):
-        return itertools.chain(self.mapped, self.non_mapped)
-    
-    def __contains__(self, key):
-        return self.contains(key)
-    
-        
-    @property
-    def get(self):
-        return self.map.get
-    
-    @property
-    def mapped(self):
-        return self.map
-
-
-def parse_argv(argv, apply={}):
-    return Argv(argv, apply)
-
-
-def is_positional(x):
-    return not x.startswith('-') and ('=') not in x
-
-
-def _push(obj, l, depth):
-    while depth:
-        l = l[-1]
-        depth -= 1
-    
-    l.append(obj)
-
-
-def _flatten(groups):
-    new_list = []
-    unjoined_chars = []
-    
-    for x in groups:
-        if not isinstance(x, str):
-            if unjoined_chars:
-                new_list.append(''.join(unjoined_chars))
-                unjoined_chars = []
-            new_list.append(_flatten(x))
-        else:
-            unjoined_chars.append(x)
-    
-    if unjoined_chars:
-        new_list.append(''.join(unjoined_chars))
-    
-    return new_list
-
-
-def parse_parentheses(s, definition='()'):
-    """a(b(cd)f) -> ['a', ['b', ['cd'], 'f']]"""
-    # https://stackoverflow.com/a/50702934
-    groups = []
-    depth = 0
-    left, right = definition
-    
-    try:
-        for char in s:
-            if char == left:
-                _push([], groups, depth)
-                depth += 1
-            elif char == right:
-                depth -= 1
-            else:
-                _push(char, groups, depth)
-    except IndexError:
-        raise ValueError('Parentheses mismatch')
-    
-    if depth > 0:
-        raise ValueError('Parentheses mismatch')
-    else:
-        return _flatten(groups)
+from collections import defaultdict
+import itertools
+import copy as _copy
+
+from fons.iter import unique
+
+"""
+The problem of this is that it has no enforced members or default values
+(like the commonly used `argparse` module does).
+Everything is dynamic.
+"""
+
+
+class Argv:
+    def __init__(self, argv, apply={}):
+        self.argv, self.map, self.non_mapped, self.indexes = self.parse(argv)
+        self.apply(apply, True)
+
+    @staticmethod
+    def parse(argv):
+        new_argv = []
+        map = {}
+        non_mapped = []
+        indexes = defaultdict(list)
+        i = 0
+        argv = tuple(argv)
+        ln_argv = len(argv)
+        var_count = 0
+        _null = object()
+
+        while i < ln_argv:
+            x = argv[i]
+            value = _null
+            is_unique = True
+            add_i = 0
+
+            if x.startswith("--"):
+                x = x[2:]
+
+            if x.startswith("-"):
+                var = x[1:]
+                try:
+                    value = argv[i + 1]
+                except IndexError:
+                    raise ValueError("Incorrectly formatted argv: {}".format(argv))
+                add_i = 1
+            elif "=" in x:
+                j = x.find("=")
+                var, value = x[:j], x[j + 1 :]
+            else:
+                var = x
+
+            if value is not _null:
+                is_unique = var not in map
+                map[var] = value
+            else:
+                non_mapped.append(x)
+
+            is_key = value is not _null
+            add_to_argv = "{}={}".format(var, value) if is_key else var
+
+            if not is_unique:
+                raise ValueError("Contains duplicate keyword: {}".format(var))
+
+            indexes[var].append((var_count, is_key))
+            var_count += 1
+            new_argv.append(add_to_argv)
+            # else:
+            #    _argv[indexes[var][0]] = add_to_argv
+            i += 1 + add_i
+
+        return new_argv, map, non_mapped, indexes
+
+    def contains(self, *vars, set=None):
+        _sets = {
+            None: (self.map, self.non_mapped),
+            "mapped": (self.map,),
+            "map": (self.map,),
+            "non_mapped": (self.non_mapped,),
+            "non-mapped": (self.non_mapped,),
+            "nonmapped": (self.non_mapped,),
+        }
+
+        try:
+            sets = _sets[set]
+        except KeyError:
+            raise ValueError(set)
+
+        return any(any(x in _set for _set in sets) for x in vars)
+
+    def which(self, vars, default=None, *, set=None):
+        return next((x for x in vars if self.contains(x, set=set)), default)
+
+    def apply(self, f_map, inplace=True):
+        new_map = self.map.copy() if not inplace else self.map
+
+        for k, f in f_map.items():
+            if k in new_map:
+                new_map[k] = f(new_map[k])
+
+        return new_map
+
+    def add(self, var, *value, index=None):
+        _ln = len(value)
+        argv, map, non_mapped, indexes = self._fetch_attrs()
+
+        if _ln > 2:
+            raise ValueError(value)
+
+        is_key = _ln == 1
+
+        if is_key:
+            if var in map:
+                if index is None:
+                    index = next(x[0] for x in self.indexes[var] if x[1])
+                self.drop(var, set="mapped")
+            map[var] = value[0]
+            txt = "{}={}".format(var, value[0])
+        else:
+            non_mapped.append(var)
+            txt = var
+
+        ln_argv = len(argv)
+
+        if index is None:
+            index = ln_argv
+        else:
+            index = self._resolve_positions((index,), ln_argv, type="insert")[0]
+
+        argv.insert(index, txt)
+
+        self._readjust_indexes(var, indexes, ((index, is_key),), "add")
+
+    def drop(self, var, *, set=None, position=None):
+        argv, map, non_mapped, indexes = self._fetch_attrs()
+        is_both = set is None
+        is_map = set in ("map", "mapped")
+        is_nonmapped = set in ("non_mapped", "non-mapped", "nonmapped")
+
+        if not self.contains(var, set=set):
+            return
+
+        eligible = [
+            x
+            for x in indexes[var]
+            if x[1] and not is_nonmapped or not x[1] and not is_map
+        ]
+
+        s = sorted(eligible, key=lambda x: x[0])
+
+        if isinstance(position, int):
+            position = (position,)
+
+        if position is not None:
+            position = self._resolve_positions(position, len(s), type="resolve")
+            s = [s[j] for j in position]
+
+        s = sorted(s, reverse=True, key=lambda x: x[0])
+
+        for i, is_key in s:
+            argv.pop(i)
+            if is_key:
+                del map[var]
+            else:
+                non_mapped.remove(var)
+
+        self._readjust_indexes(var, indexes, s, "drop")
+
+    def drop_key(self, var):
+        return self.drop(var, set="key")
+
+    def drop_value(self, var):
+        return self.drop(self, var, set="value")
+
+    @staticmethod
+    def _readjust_indexes(var, indexes, changed, action="add"):
+        if action not in ("add", "drop"):
+            raise ValueError(action)
+        is_drop = action == "drop"
+        diff = -1 if is_drop else 1
+
+        if is_drop and var in indexes:
+            indexes[var] = [
+                x for x in indexes[var] if not any(y[0] == x[0] for y in changed)
+            ]
+            if not len(indexes[var]):
+                del indexes[var]
+
+        for c, is_key in sorted(changed, reverse=True, key=lambda x: x[0]):
+            for inds in list(indexes.values()):
+                for j in range(len(inds)):
+                    index, _is_key = inds[j]
+                    if index >= c:
+                        inds[j] = (index + diff, _is_key)
+
+            if not is_drop:
+                indexes[var].append((c, is_key))
+
+        return indexes
+
+    @staticmethod
+    def _resolve_positions(positions, length, type="resolve"):
+        if type not in ("resolve", "insert"):
+            raise ValueError(type)
+        is_drop = type == "resolve"
+        diff = 0 if type == "resolve" else -1
+        resolved = []
+
+        for index in positions:
+            if index > length:
+                if is_drop:
+                    continue
+                else:
+                    index = length
+            elif index < 0:
+                if index < -length and is_drop:
+                    continue
+                index = max(0, (length + diff) + index)
+            resolved.append(index)
+
+        return tuple(unique(resolved))
+
+    def _fetch_attrs(self, copy=False):
+        argv = self.argv[:] if copy else self.argv
+        map = self.map.copy() if copy else self.map
+        non_mapped = self.non_mapped[:] if copy else self.non_mapped
+        indexes = _copy.deepcopy(self.indexes) if copy else self.indexes
+
+        return argv, map, non_mapped, indexes
+
+    def copy(self):
+        attr_values = self._fetch_attrs(True)
+        new = Argv([])
+        for a, v in zip(("argv", "map", "non_mapped", "indexes"), attr_values):
+            setattr(new, a, v)
+
+        return new
+
+    def __getitem__(self, key):
+        return self.map[key]
+
+    def __iter__(self):
+        return itertools.chain(self.mapped, self.non_mapped)
+
+    def __contains__(self, key):
+        return self.contains(key)
+
+    @property
+    def get(self):
+        return self.map.get
+
+    @property
+    def mapped(self):
+        return self.map
+
+
+def parse_argv(argv, apply={}):
+    return Argv(argv, apply)
+
+
+def is_positional(x):
+    return not x.startswith("-") and ("=") not in x
+
+
+def _push(obj, l, depth):
+    while depth:
+        l = l[-1]
+        depth -= 1
+
+    l.append(obj)
+
+
+def _flatten(groups):
+    new_list = []
+    unjoined_chars = []
+
+    for x in groups:
+        if not isinstance(x, str):
+            if unjoined_chars:
+                new_list.append("".join(unjoined_chars))
+                unjoined_chars = []
+            new_list.append(_flatten(x))
+        else:
+            unjoined_chars.append(x)
+
+    if unjoined_chars:
+        new_list.append("".join(unjoined_chars))
+
+    return new_list
+
+
+def parse_parentheses(s, definition="()"):
+    """a(b(cd)f) -> ['a', ['b', ['cd'], 'f']]"""
+    # https://stackoverflow.com/a/50702934
+    groups = []
+    depth = 0
+    left, right = definition
+
+    try:
+        for char in s:
+            if char == left:
+                _push([], groups, depth)
+                depth += 1
+            elif char == right:
+                depth -= 1
+            else:
+                _push(char, groups, depth)
+    except IndexError:
+        raise ValueError("Parentheses mismatch")
+
+    if depth > 0:
+        raise ValueError("Parentheses mismatch")
+    else:
+        return _flatten(groups)
```

### Comparing `fons-0.3.1/fons/crypto.py` & `fons-0.4.0/fons/crypto.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,112 +1,119 @@
-import hmac
-import hashlib
-import os
-from base64 import urlsafe_b64encode as b64e, urlsafe_b64decode as b64d, b64encode
-from cryptography.fernet import Fernet
-from cryptography.hazmat.backends import default_backend
-from cryptography.hazmat.primitives import hashes
-from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
-import random
-import string
-import time
-
-backend = default_backend()
-iterations = 100*1000
-
-ALPHA = string.ascii_lowercase
-DIGITS =  string.digits
-ALNUM = ALPHA + DIGITS
-HEX = DIGITS + 'abcdef'
-SETS = {'alpha': ALPHA,
-        'num': DIGITS,
-        'alnum': ALNUM,
-        'hex': HEX}
-
-_len = len
-
-def nonce(len=35, set='alnum', uppers=True, lowers=True, custom_set=None):
-    set = SETS[set] if custom_set is None else custom_set
-    if not lowers: set = set.upper()
-    elif uppers: set += ''.join(x.upper() for x in set if x.isalpha())
-    len_set = _len(set)
-    if not len_set:
-        raise IndexError('Got empty set.')
-    nonce = ''.join(set[random.randint(0,len_set-1)] for _ in range(len))
-    return nonce
-
-
-def nonce_ms():
-    return int(time.time() * 1000)
-
-
-def sign(key, msg=None, digestmod='sha256', hexdigest=True, base64=False):
-    sig = hmac.new(
-        key.encode('utf-8'),
-        msg=msg.encode('utf-8') if msg is not None else msg,
-        digestmod=getattr(hashlib,digestmod) if isinstance(digestmod,str) else digestmod
-    )
-    sig = sig.hexdigest() if hexdigest else sig.digest()
-    if base64:
-        sig = b64encode(sig)
-        sig = sig.decode()
-    return sig
-
-
-def _derive_key(password, salt, iterations=iterations):
-    """
-    Derive a secret key from a given password and salt
-    :type password: bytes
-    :type salt: bytes
-    :type iterations: int
-    :returns: bytes
-    """
-    kdf = PBKDF2HMAC(
-        algorithm=hashes.SHA256(), length=32, salt=salt,
-        iterations=iterations, backend=backend)
-    return b64e(kdf.derive(password))
-
-
-def password_encrypt(message, password, iterations=iterations, encoding='utf-8'):
-    """
-    Encrypt message with a password. Uses PBKDF2 to derive the key
-    from password and random salt, then encrypts the message bytes with the key.
-    Quite secure (with high enough iterations (>=100) and strong password),
-    but if used with a small circuit and very little RAM, may expose to brute forcing.
-    Weaknesses: https://en.wikipedia.org/wiki/PBKDF2#Alternatives_to_PBKDF2
-    Source: https://stackoverflow.com/a/55147077/10492167
-    
-    To later decrypt the message use password_decrypt(token, password), where
-    `token` is the output of this function.
-    
-    :type message: bytes or str
-    :type password: str
-    :type iterations: int
-    :returns: bytes
-    """
-    if isinstance(message, str):
-        message = message.encode(encoding)
-    salt = os.urandom(16)
-    key = _derive_key(password.encode(), salt, iterations)
-    return b64e(
-        b'%b%b%b' % (
-            salt,
-            iterations.to_bytes(4, 'big'),
-            b64d(Fernet(key).encrypt(message)),
-        )
-    )
-
-
-def password_decrypt(token, password):
-    """
-    Decrypts the token back to the bytes form of message.
-    (`token` is the result of `password_encrypt(message, password)`)
-    :type token: bytes
-    :param token: the result of password_encrypt()
-    :type password: str
-    :returns: bytes
-    """
-    decoded = b64d(token)
-    salt, iter, token = decoded[:16], decoded[16:20], b64e(decoded[20:])
-    iterations = int.from_bytes(iter, 'big')
-    key = _derive_key(password.encode(), salt, iterations)
-    return Fernet(key).decrypt(token)
+import hmac
+import hashlib
+import os
+from base64 import urlsafe_b64encode as b64e, urlsafe_b64decode as b64d, b64encode
+from cryptography.fernet import Fernet
+from cryptography.hazmat.backends import default_backend
+from cryptography.hazmat.primitives import hashes
+from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
+import random
+import string
+import time
+
+backend = default_backend()
+iterations = 100 * 1000
+
+ALPHA = string.ascii_lowercase
+DIGITS = string.digits
+ALNUM = ALPHA + DIGITS
+HEX = DIGITS + "abcdef"
+SETS = {"alpha": ALPHA, "num": DIGITS, "alnum": ALNUM, "hex": HEX}
+
+_len = len
+
+
+def nonce(len=35, set="alnum", uppers=True, lowers=True, custom_set=None):
+    set = SETS[set] if custom_set is None else custom_set
+    if not lowers:
+        set = set.upper()
+    elif uppers:
+        set += "".join(x.upper() for x in set if x.isalpha())
+    len_set = _len(set)
+    if not len_set:
+        raise IndexError("Got empty set.")
+    nonce = "".join(set[random.randint(0, len_set - 1)] for _ in range(len))
+    return nonce
+
+
+def nonce_ms():
+    return int(time.time() * 1000)
+
+
+def sign(key, msg=None, digestmod="sha256", hexdigest=True, base64=False):
+    sig = hmac.new(
+        key.encode("utf-8"),
+        msg=msg.encode("utf-8") if msg is not None else msg,
+        digestmod=getattr(hashlib, digestmod)
+        if isinstance(digestmod, str)
+        else digestmod,
+    )
+    sig = sig.hexdigest() if hexdigest else sig.digest()
+    if base64:
+        sig = b64encode(sig)
+        sig = sig.decode()
+    return sig
+
+
+def _derive_key(password, salt, iterations=iterations):
+    """
+    Derive a secret key from a given password and salt
+    :type password: bytes
+    :type salt: bytes
+    :type iterations: int
+    :returns: bytes
+    """
+    kdf = PBKDF2HMAC(
+        algorithm=hashes.SHA256(),
+        length=32,
+        salt=salt,
+        iterations=iterations,
+        backend=backend,
+    )
+    return b64e(kdf.derive(password))
+
+
+def password_encrypt(message, password, iterations=iterations, encoding="utf-8"):
+    """
+    Encrypt message with a password. Uses PBKDF2 to derive the key
+    from password and random salt, then encrypts the message bytes with the key.
+    Quite secure (with high enough iterations (>=100) and strong password),
+    but if used with a small circuit and very little RAM, may expose to brute forcing.
+    Weaknesses: https://en.wikipedia.org/wiki/PBKDF2#Alternatives_to_PBKDF2
+    Source: https://stackoverflow.com/a/55147077/10492167
+
+    To later decrypt the message use password_decrypt(token, password), where
+    `token` is the output of this function.
+
+    :type message: bytes or str
+    :type password: str
+    :type iterations: int
+    :returns: bytes
+    """
+    if isinstance(message, str):
+        message = message.encode(encoding)
+    salt = os.urandom(16)
+    key = _derive_key(password.encode(), salt, iterations)
+    return b64e(
+        b"%b%b%b"
+        % (
+            salt,
+            iterations.to_bytes(4, "big"),
+            b64d(Fernet(key).encrypt(message)),
+        )
+    )
+
+
+def password_decrypt(token, password):
+    """
+    Decrypts the token back to the bytes form of message.
+    (`token` is the result of `password_encrypt(message, password)`)
+    :type token: bytes
+    :param token: the result of password_encrypt()
+    :type password: str
+    :returns: bytes
+    """
+    decoded = b64d(token)
+    salt, iter, token = decoded[:16], decoded[16:20], b64e(decoded[20:])
+    iterations = int.from_bytes(iter, "big")
+    key = _derive_key(password.encode(), salt, iterations)
+    return Fernet(key).decrypt(token)
```

### Comparing `fons-0.3.1/fons/dict_ops.py` & `fons-0.4.0/fons/dict_ops.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,226 +1,230 @@
-import copy as _copy
-from collections import namedtuple, OrderedDict
-
-class DelType:
-    def __call__(self, other):
-        return isinstance(other, DelType)
-    def __copy__(self):
-        return self
-    def __deepcopy__(self, memo):
-        return self
-    
-#This object as a dict value signifies that 
-#its key is to be deleted in deep_update()
-DEL = DelType()
-
-
-def nt_to_od(namedtuple_or_form, fill=None):
-    nf = namedtuple_or_form
-    od = OrderedDict()
-    
-    try:
-        #test if any values assigned to nf
-        nf[0]
-    except TypeError:
-        #nf was template/form
-        od = OrderedDict(zip(nf._fields,[fill]*len(nf._fields)))
-    else:
-        for i,k in enumerate(nf._fields):
-            od[k] = nf[i]
-
-    return od
-
-
-def od_to_nt(ordereddict, nt_classname=None, return_form=False):
-    od = ordereddict
-
-    fields = list(od.keys())
-    values = list(od.values())
-
-    if nt_classname is None:
-        nt_classname = 'a_namedtuple'
-
-    nt_form = namedtuple(nt_classname,fields)
-    nt = nt_form(values)
-
-    if return_form:
-        return nt, nt_form
-    
-    return nt
-
-
-def apply_until_get(objs, f, condition='is not None', **kw):
-    if condition == 'is not None':
-        condition = lambda x: x is not None
-        
-    i = 0
-    for o in objs:
-        v = f(o)
-        if condition(v):
-            return v
-        i += 1
-    
-    if not i:
-        raise ValueError('No objs provided')
-    
-    if 'return2' in kw:
-        return kw['return2']
-    else:
-        return v
-
-
-def deep_get(objs, keywords, condition='is not None', errors=None, **kw):
-    if isinstance(keywords,str):
-        keywords = [keywords]
-    if errors not in (None, 'ignore', 'raise'):
-        raise ValueError(errors)
-    was_found = False
-    notFound = object()
-    
-    return_first = (condition == 'first')
-    if return_first:
-        condition = lambda x: x is not notFound
-    
-    
-    def recursive_get(obj, keywords=keywords):
-        nonlocal was_found
-        keywords = iter(keywords)
-        k = next(keywords)
-        if obj is None:
-            return None if not return_first else notFound
-        try: v = obj[k]
-        except KeyError:
-            return None if not return_first else notFound
-        try: return recursive_get(v, keywords)
-        except StopIteration:
-            was_found = True
-            return v
-    
-    v = apply_until_get(objs, recursive_get, condition, **kw)
-    
-    if not was_found and errors=='raise':
-        raise KeyError(keywords)
-    
-    if v is notFound:
-        return None
-    return v
-        
-
-def _matches_new_value(x, new_value):
-    """x is a key of hierarchy"""
-    if isinstance(x, type):
-        if isinstance(new_value, x):
-            return True
-        
-    elif new_value == x:
-        return True
-    
-    return False
-    
-    
-def _is_dominant(new_value, old_value, hierarchy):
-    type_old = type(old_value)
-    hierarchy_mathes = [x for x in hierarchy if _matches_new_value(x, new_value)]
-    doms_map = {'any': False, 'all': False, 'none': True}
-    subs_map = {'any': True, 'all': True, 'none': False}
-    
-    for m in hierarchy_mathes:
-        item = hierarchy[m]
-        subs = doms = ()
-        if item is None:
-            continue
-        elif isinstance(item, dict):
-            subs = item.get('subs')
-            doms = item.get('doms')
-        elif isinstance(item, str):
-            doms = item
-        else:
-            doms = item
-            
-        for name,x,map in [('doms', doms, doms_map),
-                           ('subs',subs, subs_map)]:
-            if isinstance(x, str) and x in map:
-                return map[x]
-            elif isinstance(x, tuple):
-                if issubclass(type_old, x):
-                    return name == 'subs'
-            else:
-                raise ValueError({m: item})
-            
-    return True
-
-
-def _is_shallow(key, shallow):
-    if not isinstance(shallow, dict):
-        return key in shallow
-    else:
-        x = shallow[key]
-        if hasattr(x, '__iter__') or hasattr(x, '__getitem__'):
-            return False
-        else:
-            return bool(x)
-        
-
-def _drop_dels(d, copy=False):
-    if not isinstance(d, dict):
-        return d if not copy else _copy.deepcopy(d)
-    elif copy:
-        dict_class = type(d)
-        return dict_class((k, _drop_dels(v, copy))
-                          for k,v in d.items() if not DEL(v))
-    else:
-        for k,v in tuple(d.items()):
-            if DEL(v):
-                del d[k]
-            else:
-                _drop_dels(v, copy)
-        return d
-        
-    
-def deep_update(obj, new, copy=False, hierarchy={}, **kw):
-    if not isinstance(obj,dict) or not isinstance(new,dict):
-        return _drop_dels(new, copy=copy)
-    
-    shallow = kw.pop('shallow', None)
-    if shallow is not None:
-        shallow_keys = [k for k in new if _is_shallow(k, shallow)]
-    else:
-        shallow_keys = []
-        
-    get_sub_shallow = (lambda k: shallow.get(k)) if isinstance(shallow, dict) else\
-                      (lambda k: None)
-    
-    _is_dom = kw.get('_is_dominant')
-    if _is_dom is None:
-        _is_dom = (lambda x,y,h: True) if not hierarchy else _is_dominant
-        kw['_is_dominant'] = _is_dom
-        
-    new_doms = set(k for k,v in new.items() 
-                    if k not in obj or _is_dom(v, obj[k], hierarchy))
-    
-    _old = obj
-    if copy:
-        must_copy = lambda obj_key: obj_key not in new or \
-                                     obj_key not in new_doms
-        #only deepcopy values that are not overwritten
-        # later anyways
-        obj = {k: (_copy.deepcopy(v) if must_copy(k) else v)
-               for k,v in _old.items()}
-    
-    for kN,vN in new.items():
-        if DEL(vN):
-            try:
-                del obj[kN]
-            except KeyError:
-                pass
-            
-        elif kN in new_doms:
-            if kN in shallow_keys:
-                obj[kN] = _drop_dels(vN, copy)
-            else:
-                
-                obj[kN] = deep_update(_old.get(kN), vN, copy, hierarchy, 
-                                      shallow=get_sub_shallow(kN), **kw)
-        
-        
-    return obj
+import copy as _copy
+from collections import namedtuple, OrderedDict
+
+
+class DelType:
+    def __call__(self, other):
+        return isinstance(other, DelType)
+
+    def __copy__(self):
+        return self
+
+    def __deepcopy__(self, memo):
+        return self
+
+
+# This object as a dict value signifies that
+# its key is to be deleted in deep_update()
+DEL = DelType()
+
+
+def nt_to_od(namedtuple_or_form, fill=None):
+    nf = namedtuple_or_form
+    od = OrderedDict()
+
+    try:
+        # test if any values assigned to nf
+        nf[0]
+    except TypeError:
+        # nf was template/form
+        od = OrderedDict(zip(nf._fields, [fill] * len(nf._fields)))
+    else:
+        for i, k in enumerate(nf._fields):
+            od[k] = nf[i]
+
+    return od
+
+
+def od_to_nt(ordereddict, nt_classname=None, return_form=False):
+    od = ordereddict
+
+    fields = list(od.keys())
+    values = list(od.values())
+
+    if nt_classname is None:
+        nt_classname = "a_namedtuple"
+
+    nt_form = namedtuple(nt_classname, fields)
+    nt = nt_form(values)
+
+    if return_form:
+        return nt, nt_form
+
+    return nt
+
+
+def apply_until_get(objs, f, condition="is not None", **kw):
+    if condition == "is not None":
+        condition = lambda x: x is not None
+
+    i = 0
+    for o in objs:
+        v = f(o)
+        if condition(v):
+            return v
+        i += 1
+
+    if not i:
+        raise ValueError("No objs provided")
+
+    if "default" in kw:
+        return kw["default"]
+    elif "return2" in kw:
+        return kw["return2"]
+    else:
+        return v
+
+
+def deep_get(objs, keywords, condition="is not None", errors=None, **kw):
+    if isinstance(keywords, str):
+        keywords = [keywords]
+    if errors not in (None, "ignore", "raise"):
+        raise ValueError(errors)
+    was_found = False
+    notFound = object()
+
+    return_first = condition == "first"
+    if return_first:
+        condition = lambda x: x is not notFound
+
+    def recursive_get(obj, keywords=keywords):
+        nonlocal was_found
+        keywords = iter(keywords)
+        k = next(keywords)
+        if obj is None:
+            return None if not return_first else notFound
+        try:
+            v = obj[k]
+        except KeyError:
+            return None if not return_first else notFound
+        try:
+            return recursive_get(v, keywords)
+        except StopIteration:
+            was_found = True
+            return v
+
+    v = apply_until_get(objs, recursive_get, condition, **kw)
+
+    if not was_found and errors == "raise":
+        raise KeyError(keywords)
+
+    if v is notFound:
+        return None
+    return v
+
+
+def _matches_new_value(x, new_value):
+    """x is a key of hierarchy"""
+    if isinstance(x, type):
+        if isinstance(new_value, x):
+            return True
+
+    elif new_value == x:
+        return True
+
+    return False
+
+
+def _is_dominant(new_value, old_value, hierarchy):
+    type_old = type(old_value)
+    hierarchy_mathes = [x for x in hierarchy if _matches_new_value(x, new_value)]
+    doms_map = {"any": False, "all": False, "none": True}
+    subs_map = {"any": True, "all": True, "none": False}
+
+    for m in hierarchy_mathes:
+        item = hierarchy[m]
+        subs = doms = ()
+        if item is None:
+            continue
+        elif isinstance(item, dict):
+            subs = item.get("subs")
+            doms = item.get("doms")
+        elif isinstance(item, str):
+            doms = item
+        else:
+            doms = item
+
+        for name, x, map in [("doms", doms, doms_map), ("subs", subs, subs_map)]:
+            if isinstance(x, str) and x in map:
+                return map[x]
+            elif isinstance(x, tuple):
+                if issubclass(type_old, x):
+                    return name == "subs"
+            else:
+                raise ValueError({m: item})
+
+    return True
+
+
+def _is_shallow(key, shallow):
+    if not isinstance(shallow, dict):
+        return key in shallow
+    else:
+        x = shallow[key]
+        if hasattr(x, "__iter__") or hasattr(x, "__getitem__"):
+            return False
+        else:
+            return bool(x)
+
+
+def _drop_dels(d, copy=False):
+    if not isinstance(d, dict):
+        return d if not copy else _copy.deepcopy(d)
+    elif copy:
+        dict_class = type(d)
+        return dict_class((k, _drop_dels(v, copy)) for k, v in d.items() if not DEL(v))
+    else:
+        for k, v in tuple(d.items()):
+            if DEL(v):
+                del d[k]
+            else:
+                _drop_dels(v, copy)
+        return d
+
+
+def deep_update(obj, new, copy=False, hierarchy={}, **kw):
+    if not isinstance(obj, dict) or not isinstance(new, dict):
+        return _drop_dels(new, copy=copy)
+
+    shallow = kw.pop("shallow", None)
+    if shallow is not None:
+        shallow_keys = [k for k in new if _is_shallow(k, shallow)]
+    else:
+        shallow_keys = []
+
+    get_sub_shallow = (
+        (lambda k: shallow.get(k)) if isinstance(shallow, dict) else (lambda k: None)
+    )
+
+    _is_dom = kw.get("_is_dominant")
+    if _is_dom is None:
+        _is_dom = (lambda x, y, h: True) if not hierarchy else _is_dominant
+        kw["_is_dominant"] = _is_dom
+
+    new_doms = set(
+        k for k, v in new.items() if k not in obj or _is_dom(v, obj[k], hierarchy)
+    )
+
+    _old = obj
+    if copy:
+        must_copy = lambda obj_key: obj_key not in new or obj_key not in new_doms
+        # only deepcopy values that are not overwritten
+        # later anyways
+        obj = {k: (_copy.deepcopy(v) if must_copy(k) else v) for k, v in _old.items()}
+
+    for kN, vN in new.items():
+        if DEL(vN):
+            try:
+                del obj[kN]
+            except KeyError:
+                pass
+
+        elif kN in new_doms:
+            if kN in shallow_keys:
+                obj[kN] = _drop_dels(vN, copy)
+            else:
+                obj[kN] = deep_update(
+                    _old.get(kN), vN, copy, hierarchy, shallow=get_sub_shallow(kN), **kw
+                )
+
+    return obj
```

### Comparing `fons-0.3.1/fons/dtype/store.py` & `fons-0.4.0/fons/dtype/store.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,481 +1,535 @@
 import os
 import pandas as pd
 import numpy as np
 import json
 import datetime
+
 dt = datetime.datetime
 td = datetime.timedelta
 
-from fons.os import (delete_empty_dirs, make_dirpath)
+from fons.os import delete_empty_dirs, make_dirpath
 from fons.io import DateTimeEncoder
 import fons.log as _log
 import fons.math.series as du
-from fons.time import (dt_round, dt_isround, freq_to_offset, dt_strp)
+from fons.time import dt_round, dt_isround, freq_to_offset, dt_strp
 from fons.verify import init_data
 
 
-FREQS = ['MS','D','H','T']
+FREQS = ["MS", "D", "H", "T"]
 
-logger,logger2,tlogger,tloggers,tlogger0 = _log.get_standard_5(__name__)
+logger, logger2, tlogger, tloggers, tlogger0 = _log.get_standard_5(__name__)
 
-#-----------------------------------------------------
-    
-DATE_FMT = '%Y-%m-%dT%H-%M-%S-%f'
-OBS_DATE_FMT = '%Y-%m-%dT%H-%M-%S'
-
-DIR_FMTS = {'MS': '%Y-%m',
-            'D': '%d',
-            'H': '%H'}
-FILE_FMTS = {'MS': '%Y-%m',
-             'D': '%Y-%m-%d',
-             'H': '%Y-%m-%dT%H',
-             'T': '%Y-%m-%dT%H-%M'}
+# -----------------------------------------------------
 
-PD_CONVERSIONS = {
-    list: json.loads}
+DATE_FMT = "%Y-%m-%dT%H-%M-%S-%f"
+OBS_DATE_FMT = "%Y-%m-%dT%H-%M-%S"
 
+DIR_FMTS = {"MS": "%Y-%m", "D": "%d", "H": "%H"}
+FILE_FMTS = {"MS": "%Y-%m", "D": "%Y-%m-%d", "H": "%Y-%m-%dT%H", "T": "%Y-%m-%dT%H-%M"}
+
+PD_CONVERSIONS = {list: json.loads}
 
-def _resolve_root(descr, TEST_MODE=None, root=None):
-    if root is not None: return root
-    return descr['root'] if not TEST_MODE else descr['test_root']
 
+def _resolve_root(descr, TEST_MODE=None, root=None):
+    if root is not None:
+        return root
+    return descr["root"] if not TEST_MODE else descr["test_root"]
+
+
+def _dissolve_tp(tp, max_freq="MS"):
+    if tp is None:
+        return []
+    Ttp = [dt_round(x, "T") for x in tp]
+    if Ttp[1] < tp[1]:
+        Ttp = [Ttp[0], Ttp[1] + td(minutes=1)]
+
+    Htp = [dt_round(x, "H") for x in tp]
+    if Htp[0] < tp[0]:
+        Htp = [Htp[0] + td(hours=1), Htp[1]]
+
+    Dtp = [dt_round(x, "D") for x in tp]
+    if Dtp[0] < tp[0]:
+        Dtp = [Dtp[0] + td(1), Dtp[1]]
 
-def _dissolve_tp(tp, max_freq='MS'):
-    if tp is None: return []
-    Ttp = [dt_round(x,'T') for x in tp]
-    if Ttp[1] < tp[1]: Ttp = [Ttp[0], Ttp[1]+td(minutes=1)]
-    
-    Htp = [dt_round(x,'H') for x in tp]
-    if Htp[0] < tp[0]: 
-        Htp = [Htp[0]+td(hours=1), Htp[1]]
-    
-    Dtp = [dt_round(x,'D') for x in tp]
-    if Dtp[0] < tp[0]: 
-        Dtp = [Dtp[0]+td(1), Dtp[1]]
-        
-    Mtp = [dt_round(x,'MS') for x in tp]
+    Mtp = [dt_round(x, "MS") for x in tp]
     if Mtp[0] < tp[0]:
-        Mtp = [Mtp[0]+pd.offsets.MonthBegin(), Mtp[1]]
+        Mtp = [Mtp[0] + pd.offsets.MonthBegin(), Mtp[1]]
+
+    M = pd.date_range(Mtp[0], Mtp[1], freq="1MS", normalize=True)
+    D = pd.date_range(Dtp[0], Dtp[1], freq="1D", normalize=True)
+    H = pd.date_range(Htp[0], Htp[1], freq="1H")
+    T = pd.date_range(Ttp[0], Ttp[1], freq="1T")
 
-    M = pd.date_range(Mtp[0],Mtp[1],freq='1MS', normalize=True)
-    D = pd.date_range(Dtp[0],Dtp[1],freq='1D', normalize=True)
-    H = pd.date_range(Htp[0],Htp[1],freq='1H')
-    T = pd.date_range(Ttp[0],Ttp[1],freq='1T')
-    
-    if max_freq in ('M','MS',None):
+    if max_freq in ("M", "MS", None):
         pass
-    elif max_freq in ('D',):
+    elif max_freq in ("D",):
         M = M[0:0]
-    elif max_freq in ('H',):
+    elif max_freq in ("H",):
         M = M[0:0]
         D = D[0:0]
-    elif max_freq in ('T',):
+    elif max_freq in ("T",):
         M = M[0:0]
         D = D[0:0]
         H = H[0:0]
     else:
         raise ValueError(max_freq)
-        
+
     if M.shape[0]:
         D = D[(D < M[0]) | (D >= M[-1])]
         H = H[(H < M[0]) | (H >= M[-1])]
         T = T[(T < M[0]) | (T >= M[-1])]
-        
+
     if D.shape[0]:
         H = H[(H < D[0]) | (H >= D[-1])]
         T = T[(T < D[0]) | (T >= D[-1])]
-        
+
     if H.shape[0]:
         T = T[(T < H[0]) | (T >= H[-1])]
-    
+
     dr = []
-    
-    offsets = [ pd.offsets.MonthBegin(),
-                pd.offsets.Day(),
-                pd.offsets.Hour(), 
-                pd.offsets.Minute(), ]
-    
-    for x,ofs in zip((M,D,H,T),offsets):
+
+    offsets = [
+        pd.offsets.MonthBegin(),
+        pd.offsets.Day(),
+        pd.offsets.Hour(),
+        pd.offsets.Minute(),
+    ]
+
+    for x, ofs in zip((M, D, H, T), offsets):
         if x.shape[0] < 2:
             continue
-               
+
         for y in x[:-1]:
             dr.append((y, y + ofs))
 
-    return sorted(dr,key=lambda x: x[0])
-    
-    
+    return sorted(dr, key=lambda x: x[0])
+
+
 def _get_higher_freqs(freq):
-    _freq = freq[next((i for i,x in enumerate(freq) if x.isalpha()),0):]
+    _freq = freq[next((i for i, x in enumerate(freq) if x.isalpha()), 0) :]
     if _freq not in FREQS:
-        raise ValueError('Unrecognized freq: {}'.format(freq))
+        raise ValueError("Unrecognized freq: {}".format(freq))
     i = FREQS.index(_freq)
     return FREQS[:i]
-            
-            
-def merge_data(id, descr, tp, freq='MS', include_longer_freqs=True, 
-               delete_shorter_freqs=False, output_root=None,recycler=None, **kw):
-    
-    tlogger.debug('Merging tp:{} freq:{} id:{}'.format(tp,freq,id))
-    
+
+
+def merge_data(
+    id,
+    descr,
+    tp,
+    freq="MS",
+    include_longer_freqs=True,
+    delete_shorter_freqs=False,
+    output_root=None,
+    recycler=None,
+    **kw
+):
+    tlogger.debug("Merging tp:{} freq:{} id:{}".format(tp, freq, id))
+
     try:
         freq_loc = FREQS.index(freq)
     except IndexError:
-        raise ValueError("freq must one of the following: {}. Got '{}'".format(FREQS, freq))
-    
+        raise ValueError(
+            "freq must one of the following: {}. Got '{}'".format(FREQS, freq)
+        )
+
     search_freqs = FREQS if include_longer_freqs else FREQS[freq_loc:]
-    delete_freqs = FREQS[freq_loc+1:] if delete_shorter_freqs else []
-    
-    paths = get_paths(id, descr, tp, freqs=search_freqs, duplicates='include', **kw)
-    #print('freqs:',search_freqs,'paths:,\n',paths,'kw:',kw)
+    delete_freqs = FREQS[freq_loc + 1 :] if delete_shorter_freqs else []
+
+    paths = get_paths(id, descr, tp, freqs=search_freqs, duplicates="include", **kw)
+    # print('freqs:',search_freqs,'paths:,\n',paths,'kw:',kw)
     data = read_data(id, descr, tp, paths=paths, **kw)
-    
+
     kw2 = kw.copy()
     if output_root is not None:
-        kw2['root'] = output_root
+        kw2["root"] = output_root
     paths_saved = save_data(data, id, descr, tp, max_freq=freq, **kw2)
-    
-    #cleanup:
+
+    # cleanup:
     any_removed = False
-        
-    for curfreq,subpaths in paths[delete_freqs].iteritems():
+
+    for curfreq, subpaths in paths[delete_freqs].iteritems():
         for pth in subpaths.dropna():
-            if pth in paths_saved: continue
+            if pth in paths_saved:
+                continue
             any_removed = True
             if recycler is not None:
                 recycler(pth)
                 continue
-            try: os.remove(pth)
-            except FileNotFoundError: pass
+            try:
+                os.remove(pth)
+            except FileNotFoundError:
+                pass
             except OSError as e:
-                logger2.error('Can\'t delete {}'.format(pth))
+                logger2.error("Can't delete {}".format(pth))
                 logger.exception(e)
-                  
+
     if any_removed:
-        trunk = get_trunk(id, descr, **kw) 
+        trunk = get_trunk(id, descr, **kw)
         delete_empty_dirs(trunk, recycler)
-        
+
     if output_root is not None:
         trunk2 = get_trunk(id, descr, **kw2)
         delete_empty_dirs(trunk2, recycler)
-        
 
-def _delete_paths(paths, freqs=[], exclude=[],
-                  delete_empty_dirs=[]):
-    #cleanup:
+
+def _delete_paths(paths, freqs=[], exclude=[], delete_empty_dirs=[]):
+    # cleanup:
     any_removed = False
-        
-    for curfreq,subpaths in paths[freqs].iteritems():
+
+    for curfreq, subpaths in paths[freqs].iteritems():
         for pth in subpaths.dropna():
-            if pth in exclude: continue
+            if pth in exclude:
+                continue
             any_removed = True
-            logger.info('_path_ removing: {}'.format(pth))
-            try: os.remove(pth)
+            logger.info("_path_ removing: {}".format(pth))
+            try:
+                os.remove(pth)
             except OSError as e:
-                logger2.error('Can\'t delete {}'.format(pth))
+                logger2.error("Can't delete {}".format(pth))
                 logger.exception(e)
-             
+
     if any_removed:
         for trunk in delete_empty_dirs:
             delete_empty_dirs(trunk)
-        
+
 
 def _csv_params(descr):
-    converters = descr['converters']
-    temp = descr['template']
+    converters = descr["converters"]
+    temp = descr["template"]
     conv_given = {} if converters is None else converters
-    converters = temp.get('dtypes',{}).copy()
+    converters = temp.get("dtypes", {}).copy()
     converters.update(conv_given)
-    
-    parse_dates = [k for k,v in converters.items() if v == 'datetime64[ns]']
-    converters = {k:v for k,v in converters.items() if v is str or k in conv_given} #doesn't work on csv for some reason (str->dtype:float)
-    
-    index_col = descr['index_col']
-    index_dtype = descr['index_dtype']
-    ic2 = index_col if isinstance(index_col, (list,tuple)) else [index_col]
-    it2 = index_dtype if isinstance(index_col, (list,tuple)) else [index_dtype]
-    #index_dtype in descr or temp?
-    
-    for dtype,col_nr in reversed(list(zip(it2,ic2))):
-        if dtype == 'datetime64[ns]':
-            parse_dates.insert(0,col_nr)
-
-    #print('parse_dates:',parse_dates,'converters:',converters)
-    d = {'index_col': index_col, 'parse_dates': parse_dates, 'converters': converters}#, 'sep': ',', 'decimal': '.'}
-    
+
+    parse_dates = [k for k, v in converters.items() if v == "datetime64[ns]"]
+    converters = {
+        k: v for k, v in converters.items() if v is str or k in conv_given
+    }  # doesn't work on csv for some reason (str->dtype:float)
+
+    index_col = descr["index_col"]
+    index_dtype = descr["index_dtype"]
+    ic2 = index_col if isinstance(index_col, (list, tuple)) else [index_col]
+    it2 = index_dtype if isinstance(index_col, (list, tuple)) else [index_dtype]
+    # index_dtype in descr or temp?
+
+    for dtype, col_nr in reversed(list(zip(it2, ic2))):
+        if dtype == "datetime64[ns]":
+            parse_dates.insert(0, col_nr)
+
+    # print('parse_dates:',parse_dates,'converters:',converters)
+    d = {
+        "index_col": index_col,
+        "parse_dates": parse_dates,
+        "converters": converters,
+    }  # , 'sep': ',', 'decimal': '.'}
+
     return d
-               
+
 
 def read_data(id, descr, tp, **kw):
-    json_load = (descr['ftype'] == 'json')
+    json_load = descr["ftype"] == "json"
     if not json_load:
-        tlogger.debug('getting csv_params')
+        tlogger.debug("getting csv_params")
         csv_params = _csv_params(descr)
-    
-    kw2 = {x:y for x,y in kw.items() if x not in ('paths',)}
-    paths = get_paths(id,descr,tp,**kw2) if kw.get('paths') is None else kw['paths']
+
+    kw2 = {x: y for x, y in kw.items() if x not in ("paths",)}
+    paths = get_paths(id, descr, tp, **kw2) if kw.get("paths") is None else kw["paths"]
     dparts = []
-    decode = descr['decode']
-    init = descr['init_data']
+    decode = descr["decode"]
+    init = descr["init_data"]
     method = dparts.extend if json_load else dparts.append
-    
+
     for ir in paths.iterrows():
-        #tlogger.debug(ir)
+        # tlogger.debug(ir)
         row = ir[1]
-        path = row['path']
-        logger.debug('_path_ loading: {}'.format(path))
+        path = row["path"]
+        logger.debug("_path_ loading: {}".format(path))
         try:
             if json_load:
-                with open(path,encoding='utf-8') as f:
+                with open(path, encoding="utf-8") as f:
                     dat = json.load(f)
-                    if init: dat = init_data(dat)
+                    if init:
+                        dat = init_data(dat)
             else:
-                dat = pd.read_csv(path,**csv_params)
+                dat = pd.read_csv(path, **csv_params)
             if decode is not None:
                 dat = decode(dat)
             method(dat)
         except Exception as e:
             logger.exception(e)
-       
+
     if not len(dparts):
-        #returns empty dataframe/list...
-        return init_data(descr['template'])
-    
+        # returns empty dataframe/list...
+        return init_data(descr["template"])
+
     elif json_load:
-        obj = du.slice_obj(dparts, tp, descr['time_key'])
-    
+        obj = du.slice_obj(dparts, tp, descr["time_key"])
+
     else:
-        conc = pd.concat(dparts, ignore_index=descr['ignore_index'])
-        #print(conc.dtypes)
-        obj = du.slice_obj(conc, tp, descr['time_key'])
+        conc = pd.concat(dparts, ignore_index=descr["ignore_index"])
+        # print(conc.dtypes)
+        obj = du.slice_obj(conc, tp, descr["time_key"])
 
-    ensure_integrity = descr['ensure_integrity']
+    ensure_integrity = descr["ensure_integrity"]
     if ensure_integrity is not None:
         obj = ensure_integrity(obj)
-        
+
     return obj
 
 
-def save_data(obj, id, descr, tp,max_freq='MS', **kw):
-    time_key = descr['time_key']
+def save_data(obj, id, descr, tp, max_freq="MS", **kw):
+    time_key = descr["time_key"]
     tp = du.get_timestamps(tp)
     tp_slices = _dissolve_tp(tp, max_freq)
-      
+
     paths_saved = []
-    root = _resolve_root(descr,**kw)
-    ftype = descr['ftype']
-    encode = descr['encode']
-    if ftype not in ('json','csv'):
+    root = _resolve_root(descr, **kw)
+    ftype = descr["ftype"]
+    encode = descr["encode"]
+    if ftype not in ("json", "csv"):
         raise ValueError(ftype)
-    lenf = lambda x: x.shape[0] if ftype == 'csv' else len(x)
-    
-    ensure_integrity = descr['ensure_integrity']
+    lenf = lambda x: x.shape[0] if ftype == "csv" else len(x)
+
+    ensure_integrity = descr["ensure_integrity"]
     if ensure_integrity is not None:
         obj = ensure_integrity(obj)
-    
+
     for tp_slice in tp_slices:
-        tlogger.debug('{} {}'.format(tp_slice, id))
+        tlogger.debug("{} {}".format(tp_slice, id))
         r = induce_datefmt(tp_slice)
         _dir = get_dir(id, descr, tp_slice, induce_datefmt_r=r, **kw)
-        f_datefmt = r['file']
-        
-        fname = get_fname(id, descr, f_datefmt) + '.{}'.format(ftype)
+        f_datefmt = r["file"]
+
+        fname = get_fname(id, descr, f_datefmt) + ".{}".format(ftype)
         fpath = os.path.join(_dir, fname)
         obj2 = du.slice_obj(obj, tp_slice, time_key)
-        
+
         if not lenf(obj2):
-            logger.debug('{} is empty {}'.format(tp_slice, id))
-            try: os.rmdir(_dir)
-            except Exception: pass
+            logger.debug("{} is empty {}".format(tp_slice, id))
+            try:
+                os.rmdir(_dir)
+            except Exception:
+                pass
             continue
-        
+
         if encode is not None:
             obj2 = encode(obj2)
-            
+
         paths_saved.append(fpath)
-        logger.info('_path_ saving: {}'.format(fpath))
-         
-        if ftype == 'csv':
-            index = descr['index_col'] is not None
-            obj2.to_csv(fpath, index=index, encoding='utf-8')
-            
-        elif ftype == 'json':
-            with open(fpath, 'w', encoding='utf-8') as f:
+        logger.info("_path_ saving: {}".format(fpath))
+
+        if ftype == "csv":
+            index = descr["index_col"] is not None
+            obj2.to_csv(fpath, index=index, encoding="utf-8")
+
+        elif ftype == "json":
+            with open(fpath, "w", encoding="utf-8") as f:
                 json.dump(obj2, f, ensure_ascii=False, cls=DateTimeEncoder)
-        
+
     return paths_saved
 
 
 def get_fname(id, descr, ts_tp_datestr, **kw):
     if isinstance(ts_tp_datestr, str):
         date_str = ts_tp_datestr
-    elif isinstance(ts_tp_datestr, (list,tuple)):
-        r = kw.get('induce_datefmt_r')
-        date_str = induce_datefmt(ts_tp_datestr) if not r else r['file_fmt']
+    elif isinstance(ts_tp_datestr, (list, tuple)):
+        r = kw.get("induce_datefmt_r")
+        date_str = induce_datefmt(ts_tp_datestr) if not r else r["file_fmt"]
     elif isinstance(ts_tp_datestr, dt):
-        date_fmt = DATE_FMT #if d_type != 'obs' else OBS_DATE_FMT
+        date_fmt = DATE_FMT  # if d_type != 'obs' else OBS_DATE_FMT
         date_str = du.format_ts(ts_tp_datestr, date_fmt)
-    else:raise TypeError(ts_tp_datestr)
-    
-    return "_".join([date_str] + [id.get(x) for x in descr['file_fmt']])
+    else:
+        raise TypeError(ts_tp_datestr)
+
+    return "_".join([date_str] + [id.get(x) for x in descr["file_fmt"]])
 
 
-def get_dir(id, descr, tp, **kw):    
-    kw2 = {x:y for x,y in kw.items() if x not in ('induce_datefmt_r',)}
+def get_dir(id, descr, tp, **kw):
+    kw2 = {x: y for x, y in kw.items() if x not in ("induce_datefmt_r",)}
     dir1 = get_trunk(id, descr, **kw2)
-    
-    if not kw.get('induce_datefmt_r'):
+
+    if not kw.get("induce_datefmt_r"):
         r = induce_datefmt(tp)
-    else: r = kw['induce_datefmt_r']
-    
-    date_parts = r['dir']
-    
-    if r['period'] == 'month':
+    else:
+        r = kw["induce_datefmt_r"]
+
+    date_parts = r["dir"]
+
+    if r["period"] == "month":
         return make_dirpath(dir1)
-    elif r['period'] != 'other':
+    elif r["period"] != "other":
         return make_dirpath(dir1, *date_parts)
-    else: return make_dirpath(dir1, 'custom_fmt')
-    
+    else:
+        return make_dirpath(dir1, "custom_fmt")
+
 
 def induce_datefmt(tp):
     if any(not isinstance(x, dt) for x in tp):
-        raise ValueError(tp,'contains non datetime element')
-        
+        raise ValueError(tp, "contains non datetime element")
+
     len_tp = tp[1] - tp[0]
-    
-    if td(28) <= len_tp <= td(31) and dt_isround(tp[0],'month') and tp[1].month != tp[0].month:
-        return {'period': 'month', 
-                'dir': None, 
-                'file': tp[0].strftime(FILE_FMTS['MS'])}
-    
-    elif len_tp == td(1) and dt_isround(tp[0],'day'):
-        return {'period': 'day', 
-                'dir': (tp[0].strftime(DIR_FMTS['MS']),), 
-                'file': tp[0].strftime(FILE_FMTS['D'])}
-    
-    elif len_tp == td(hours=1) and  dt_isround(tp[0],'hour'):
-        return {'period': 'hour', 
-                'dir': (tp[0].strftime(DIR_FMTS['MS']),tp[0].strftime(DIR_FMTS['D'])), 
-                'file': tp[0].strftime(FILE_FMTS['H'])}
-    
-    elif len_tp == td(minutes=1) and  dt_isround(tp[0],'minute'):
-        return {'period': 'minute', 
-                'dir': (tp[0].strftime(DIR_FMTS['MS']),tp[0].strftime(DIR_FMTS['D']),tp[0].strftime(DIR_FMTS['H'])), 
-                'file': tp[0].strftime(FILE_FMTS['T'])}
-    
-    else: return {'period': 'other', 
-                  'dir': None, 
-                  'file': du.format_tp(tp, DATE_FMT)}
-    
-#-------------------------------------------------------------------------------------------
+
+    if (
+        td(28) <= len_tp <= td(31)
+        and dt_isround(tp[0], "month")
+        and tp[1].month != tp[0].month
+    ):
+        return {"period": "month", "dir": None, "file": tp[0].strftime(FILE_FMTS["MS"])}
+
+    elif len_tp == td(1) and dt_isround(tp[0], "day"):
+        return {
+            "period": "day",
+            "dir": (tp[0].strftime(DIR_FMTS["MS"]),),
+            "file": tp[0].strftime(FILE_FMTS["D"]),
+        }
+
+    elif len_tp == td(hours=1) and dt_isround(tp[0], "hour"):
+        return {
+            "period": "hour",
+            "dir": (tp[0].strftime(DIR_FMTS["MS"]), tp[0].strftime(DIR_FMTS["D"])),
+            "file": tp[0].strftime(FILE_FMTS["H"]),
+        }
+
+    elif len_tp == td(minutes=1) and dt_isround(tp[0], "minute"):
+        return {
+            "period": "minute",
+            "dir": (
+                tp[0].strftime(DIR_FMTS["MS"]),
+                tp[0].strftime(DIR_FMTS["D"]),
+                tp[0].strftime(DIR_FMTS["H"]),
+            ),
+            "file": tp[0].strftime(FILE_FMTS["T"]),
+        }
+
+    else:
+        return {"period": "other", "dir": None, "file": du.format_tp(tp, DATE_FMT)}
+
+
+# -------------------------------------------------------------------------------------------
 
 
 def get_trunk(id, descr, assert_existence=False, **kw):
     root = _resolve_root(descr, **kw)
-    order = descr['dir_fmt']
+    order = descr["dir_fmt"]
     parts = [root] + [id.get(x) for x in order]
     trunk = os.path.join(*parts)
     exists = os.path.exists(trunk)
     if not exists:
         if assert_existence:
-            raise OSError('Path {} does not exist'.format(trunk))
+            raise OSError("Path {} does not exist".format(trunk))
         make_dirpath(*parts)
-    
+
     return trunk
 
-              
-def get_paths(id, descr, tp, min_periods=None, duplicates='drop', freqs=FREQS, **kw):
+
+def get_paths(id, descr, tp, min_periods=None, duplicates="drop", freqs=FREQS, **kw):
     tp = du.get_timestamps(tp)
     if any(x not in FREQS for x in freqs):
-        raise ValueError('`freqs` contains not allowed items; got: {}'.format(freqs))
+        raise ValueError("`freqs` contains not allowed items; got: {}".format(freqs))
     elif any(freqs.count(x) > 1 for x in freqs):
-        raise ValueError('`freqs` contains duplicates; got: {}'.format(freqs))   
-    freqs =  [x for x in FREQS if x in freqs]
+        raise ValueError("`freqs` contains duplicates; got: {}".format(freqs))
+    freqs = [x for x in FREQS if x in freqs]
+
+    basedir = get_trunk(
+        id, descr, assert_existence=False, **kw
+    )  # assert_existence=True,
 
-    basedir = get_trunk(id, descr, assert_existence=False, **kw) #assert_existence=True,
-    
     mb = pd.offsets.MonthBegin()
-    start_m, end_m = [dt_round(x,mb) for x in tp]
+    start_m, end_m = [dt_round(x, mb) for x in tp]
     if tp[1] == end_m:
         end_m -= mb
-    
+
     element = freq_to_offset(FREQS[-1])
     start_t, end_t = [dt_round(x, element) for x in tp]
     if tp[1] == end_t:
         end_t -= element
     element_arr = pd.date_range(start_t, end_t, freq=element)
 
-    drop_duplicates = (duplicates == 'drop')
-    ext = '.'+descr['ftype']
-    
+    drop_duplicates = duplicates == "drop"
+    ext = "." + descr["ftype"]
+
     freq_parts = {f: [] for f in FREQS}
-    FREQS2 = ['YS'] + FREQS
-    
+    FREQS2 = ["YS"] + FREQS
+
     def _map_freq(f):
-        return {'M': 'MS', 'Y': 'YS'}.get(f, f)
-    
-    def unit(r,start,dir):
-        try: 
+        return {"M": "MS", "Y": "YS"}.get(f, f)
+
+    def unit(r, start, dir):
+        try:
             freq = FREQS2[r]
-            next_freq = FREQS2[r+1]
+            next_freq = FREQS2[r + 1]
             files = os.listdir(dir)
-        except (IndexError,OSError):
+        except (IndexError, OSError):
             return
-        
+
         ofs = freq_to_offset(_map_freq(freq))
         next_ofs = freq_to_offset(_map_freq(next_freq))
-        
-        end = dt_round(tp[1],ofs)+ofs if not r else start+ofs
-        units = pd.date_range(start, end, freq=next_ofs, closed='left')
-        if not r: units = units[(units >= start_m) & (units <= end_m)]
-        units_str = units.strftime(DIR_FMTS[next_freq]) if next_freq in DIR_FMTS else [None]*units.shape[0]
+
+        end = dt_round(tp[1], ofs) + ofs if not r else start + ofs
+        units = pd.date_range(start, end, freq=next_ofs, closed="left")
+        if not r:
+            units = units[(units >= start_m) & (units <= end_m)]
+        units_str = (
+            units.strftime(DIR_FMTS[next_freq])
+            if next_freq in DIR_FMTS
+            else [None] * units.shape[0]
+        )
         units_str_full = units.strftime(FILE_FMTS[next_freq])
         pnf = freq_parts[next_freq]
-        
+
         for ts, ts_str, ts_str_full in zip(units, units_str, units_str_full):
             fn = get_fname(id, descr, ts_str_full) + ext
             unit_fpth = os.path.join(dir, fn)
-            
+
             if next_freq in freqs and fn in files:
                 unit_fpth = os.path.join(dir, fn)
-                ts_arr = pd.date_range(ts, ts+next_ofs, freq=element_arr.freq, closed='left')
-                ts_arr = ts_arr[(ts_arr>=start_t) & (ts_arr <= end_t)]
+                ts_arr = pd.date_range(
+                    ts, ts + next_ofs, freq=element_arr.freq, closed="left"
+                )
+                ts_arr = ts_arr[(ts_arr >= start_t) & (ts_arr <= end_t)]
 
                 if ts_arr.shape[0]:
                     pnf.append(pd.Series(unit_fpth, index=ts_arr))
                     if drop_duplicates:
                         continue
-            
-            if not ts_str: continue
-            unit(r+1, ts, os.path.join(dir, ts_str))
-        
-    unit (0, dt_round(tp[0],'1YS'), basedir)
-    
-    for f,x in freq_parts.items():
-        if not len(x): continue
+
+            if not ts_str:
+                continue
+            unit(r + 1, ts, os.path.join(dir, ts_str))
+
+    unit(0, dt_round(tp[0], "1YS"), basedir)
+
+    for f, x in freq_parts.items():
+        if not len(x):
+            continue
         if x[0].index[0] > start_t:
-            x.insert(0,pd.Series(np.nan, index=[start_t]))
+            x.insert(0, pd.Series(np.nan, index=[start_t]))
         if x[-1].index[-1] < end_t:
             x.append(pd.Series(np.nan, index=[end_t]))
 
-    freqs_concatted = {f: pd.concat(x) for f,x in freq_parts.items() if x}
-    freqs_resampled = {f: x.resample(element).asfreq() for f,x in freqs_concatted.items()}
+    freqs_concatted = {f: pd.concat(x) for f, x in freq_parts.items() if x}
+    freqs_resampled = {
+        f: x.resample(element).asfreq() for f, x in freqs_concatted.items()
+    }
 
-    paths = pd.DataFrame(freqs_resampled, index=element_arr).dropna(how='all')
+    paths = pd.DataFrame(freqs_resampled, index=element_arr).dropna(how="all")
     paths = paths.reindex(columns=[x for x in FREQS if x in paths.columns])
-    paths['path'] = paths.fillna(method='ffill',axis=1)[paths.columns[-1]] if paths.columns.shape[0] else np.nan
-    paths = paths.reindex(columns=['path']+FREQS)#.dropna(subset=['path'])
-    
+    paths["path"] = (
+        paths.fillna(method="ffill", axis=1)[paths.columns[-1]]
+        if paths.columns.shape[0]
+        else np.nan
+    )
+    paths = paths.reindex(columns=["path"] + FREQS)  # .dropna(subset=['path'])
+
     if min_periods and paths.shape[0] / element_arr.shape[0] < min_periods:
-        raise ValueError('< min periods `{}`'.format(min_periods))
-        
-    paths = paths.drop_duplicates(subset=['path'])
-    
-    return paths
+        raise ValueError("< min periods `{}`".format(min_periods))
 
+    paths = paths.drop_duplicates(subset=["path"])
+
+    return paths
 
 
-if __name__ == '__main__':
-    print(_dissolve_tp((dt(2018, 10, 26, 3, 7,1), dt(2018, 10, 26, 3, 8,5)),'MS'))
-    print(_dissolve_tp((dt(2018, 9, 29, 23, 58, 2), dt(2018, 11, 2, 1, 0, 1)),'MS'))
-    #print(_dissolve_tp((dt(2018, 10, 1), dt(2018, 11, 1)),'H'))
+if __name__ == "__main__":
+    print(_dissolve_tp((dt(2018, 10, 26, 3, 7, 1), dt(2018, 10, 26, 3, 8, 5)), "MS"))
+    print(_dissolve_tp((dt(2018, 9, 29, 23, 58, 2), dt(2018, 11, 2, 1, 0, 1)), "MS"))
+    # print(_dissolve_tp((dt(2018, 10, 1), dt(2018, 11, 1)),'H'))
```

### Comparing `fons-0.3.1/fons/errors.py` & `fons-0.4.0/fons/errors.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,201 +1,210 @@
-import math
-import datetime
-dt = datetime.datetime
-td = datetime.timedelta
-
-from fons.nan import nan
-
-
-class QuitException(Exception):
-    """Raised to terminate an obj
-       Conventions:
-         Obj is assumed to catch it internally.
-         If obj's function was in the process 
-          of returning something, then will return the 
-          args[0] instead (if present)."""
-        
-    _level = 0
-
-
-class WaitException(Exception):
-    def __init__(self,*args,**kw):
-        self.time_initiated = dt.utcnow()
-        
-        time = kw.get('time',0)
-        if 'time' in kw: pass
-        elif not len(args): pass
-        elif isinstance(args[0], bool): pass
-        elif isinstance(args[0], (int,float,td)):
-            time = args[0]
-            args = args[1:]
-        
-        if isinstance(time,td):
-            time /= td(seconds=1)
-        elif not isinstance(time, (int,float)):
-            raise TypeError(type(time))
-        
-        msg = kw.get('msg')
-        if msg is None:
-            msg =  'Wait time of {} seconds is needed'.format(math.ceil(time))
-        
-        self.args = (msg,) + tuple(args)
-        self.wait_time = time
-
-    def get_time_remaining(self):
-        return self.wait_time - (dt.utcnow() - self.time_initiated) / td(seconds=1)
-    
-    _level = 0
-    wait_time = 0
-    time_initiated = dt.utcfromtimestamp(0)
-
-
-class TerminatedException(Exception):
-    _level = 0
-    
-
-#-------------------------------
-
-class BaseVeriError(Exception):
-    pass
-
-class InitError(BaseVeriError):
-    pass
-    
-class BadInstruction(BaseVeriError):
-    pass
-
-
-class VeriError(BaseVeriError):
-    def __init__(self, trace=None, got=nan, expected=nan, custom_msg=nan, *args):
-        if trace is None:
-            trace = []
-        self.trace = trace
-        self._assign_level()
-        
-        self.got = got 
-        self.expected = expected
-        self.custom_msg = custom_msg
-        
-        self.craft_msg()
-    
-    
-    def _assign_level(self):
-        self.level = max(0, len(self.trace) - 1)
-    
-    
-    def craft_msg(self):
-        msg= '{}; '.format(''.join(self.trace))
-
-        parts = []
-        if self.got is not nan:
-            parts.append('{}{}'.format(self._gotstr, repr(self.got)))
-        if self.expected is not nan:
-            parts.append('{}{}'.format(self._expstr, repr(self.expected)))
-        eg = ", ".join(parts)
-        if self.custom_msg is not nan:
-            eg += '; ' + repr(self.custom_msg)
-        
-        msg = (msg + eg).strip()
-        
-        self.msg = msg #'{}; Got:{}, Expected:{}'.format("".join(self.trace), repr(got), repr(expected))
-        #self._strmsg = '{}({})'.format(self.__class__.__name__, msg)
-        
-        #self.args = (self.msg,)
-        
-        
-    def is_faulty(self, subset=None):
-        return True
-        
-        
-    def __str__(self):
-        #return self._strmsg
-        return '{}({})'.format(self.__class__.__name__, self.msg)
-    
-    """def __repr__(self):
-        return self._reprmsg"""
-        
-    _gotstr = 'Got:'
-    _expstr = 'Expected:'
-    type = 'general'
-
-    #__slots__ = ['trace','got','expected','level','msg','_strmsg'] #doesn't do anything, new attributes can still be added
-
-
-class VeriTypeError(VeriError):
-    type = 'type'
-
-class VeriValueError(VeriError):
-    type = 'value'
-    
-
-class VeriWithSubsetsError(VeriError):
-    def is_faulty(self, subset=None):
-        """is_missing = self.expected is not nan
-        is_extra = self.got is not nan"""
-        
-        if subset is None:
-            return {k1: (getattr(self,k0) is not nan) for k0,k1 in self.subsets}
-        
-        
-        gen = (getattr(self,ss[0]) is not nan 
-                for ss in self.subsets
-               if ss[1] == subset)
-        
-        return any(gen)
-    
-    
-    type = 'general'
-    subsets = [('got','extra'),('expected','missing')]
-    _gotstr = 'Extra:'
-    _expstr = 'Missing:'
-    
-
-
-class VeriKeyError(VeriWithSubsetsError):   
-    type = 'key'
-
-class VeriIndexError(VeriWithSubsetsError):
-    type = 'index'
-    _gotstr = 'Size mismatch:'
-
-
-#------------------------------
-
-class TickerException(Exception):
-    pass
-
-
-class TickerAlreadyAdded(TickerException):
-    pass
-
-
-class TickerWaitException(TickerException, WaitException):
-    pass
-
-
-class TickerTerminated(TickerException, TerminatedException):
-    pass
-
-
-class TickerQuitException(TickerException, QuitException):
-    pass
-
-
-class AllTerminated(TickerException):
-    pass
-
-#-----------------------------------------------
-
-class ThreadEndException(Exception):
-    pass
-
-#-----------------------------------------------
-
-class BreakException(Exception):
-    pass
-
-#----------------------------------------------
-
-class ServerError(Exception):
-    def __init__(self,msg):
-        self.msg = msg
+import math
+import datetime
+
+dt = datetime.datetime
+td = datetime.timedelta
+
+from fons.nan import nan
+
+
+class QuitException(Exception):
+    """Raised to terminate an obj
+    Conventions:
+      Obj is assumed to catch it internally.
+      If obj's function was in the process
+       of returning something, then will return the
+       args[0] instead (if present)."""
+
+    _level = 0
+
+
+class WaitException(Exception):
+    def __init__(self, *args, **kw):
+        self.time_initiated = dt.utcnow()
+
+        time = kw.get("time", 0)
+        if "time" in kw:
+            pass
+        elif not len(args):
+            pass
+        elif isinstance(args[0], bool):
+            pass
+        elif isinstance(args[0], (int, float, td)):
+            time = args[0]
+            args = args[1:]
+
+        if isinstance(time, td):
+            time /= td(seconds=1)
+        elif not isinstance(time, (int, float)):
+            raise TypeError(type(time))
+
+        msg = kw.get("msg")
+        if msg is None:
+            msg = "Wait time of {} seconds is needed".format(math.ceil(time))
+
+        self.args = (msg,) + tuple(args)
+        self.wait_time = time
+
+    def get_time_remaining(self):
+        return self.wait_time - (dt.utcnow() - self.time_initiated) / td(seconds=1)
+
+    _level = 0
+    wait_time = 0
+    time_initiated = dt.utcfromtimestamp(0)
+
+
+class TerminatedException(Exception):
+    _level = 0
+
+
+# -------------------------------
+
+
+class BaseVeriError(Exception):
+    pass
+
+
+class InitError(BaseVeriError):
+    pass
+
+
+class BadInstruction(BaseVeriError):
+    pass
+
+
+class VeriError(BaseVeriError):
+    def __init__(self, trace=None, got=nan, expected=nan, custom_msg=nan, *args):
+        if trace is None:
+            trace = []
+        self.trace = trace
+        self._assign_level()
+
+        self.got = got
+        self.expected = expected
+        self.custom_msg = custom_msg
+
+        self.craft_msg()
+
+    def _assign_level(self):
+        self.level = max(0, len(self.trace) - 1)
+
+    def craft_msg(self):
+        msg = "{}; ".format("".join(self.trace))
+
+        parts = []
+        if self.got is not nan:
+            parts.append("{}{}".format(self._gotstr, repr(self.got)))
+        if self.expected is not nan:
+            parts.append("{}{}".format(self._expstr, repr(self.expected)))
+        eg = ", ".join(parts)
+        if self.custom_msg is not nan:
+            eg += "; " + repr(self.custom_msg)
+
+        msg = (msg + eg).strip()
+
+        self.msg = msg  #'{}; Got:{}, Expected:{}'.format("".join(self.trace), repr(got), repr(expected))
+        # self._strmsg = '{}({})'.format(self.__class__.__name__, msg)
+
+        # self.args = (self.msg,)
+
+    def is_faulty(self, subset=None):
+        return True
+
+    def __str__(self):
+        # return self._strmsg
+        return "{}({})".format(self.__class__.__name__, self.msg)
+
+    """def __repr__(self):
+        return self._reprmsg"""
+
+    _gotstr = "Got:"
+    _expstr = "Expected:"
+    type = "general"
+
+    # __slots__ = ['trace','got','expected','level','msg','_strmsg'] #doesn't do anything, new attributes can still be added
+
+
+class VeriTypeError(VeriError):
+    type = "type"
+
+
+class VeriValueError(VeriError):
+    type = "value"
+
+
+class VeriWithSubsetsError(VeriError):
+    def is_faulty(self, subset=None):
+        """is_missing = self.expected is not nan
+        is_extra = self.got is not nan"""
+
+        if subset is None:
+            return {k1: (getattr(self, k0) is not nan) for k0, k1 in self.subsets}
+
+        gen = (
+            getattr(self, ss[0]) is not nan for ss in self.subsets if ss[1] == subset
+        )
+
+        return any(gen)
+
+    type = "general"
+    subsets = [("got", "extra"), ("expected", "missing")]
+    _gotstr = "Extra:"
+    _expstr = "Missing:"
+
+
+class VeriKeyError(VeriWithSubsetsError):
+    type = "key"
+
+
+class VeriIndexError(VeriWithSubsetsError):
+    type = "index"
+    _gotstr = "Size mismatch:"
+
+
+# ------------------------------
+
+
+class TickerException(Exception):
+    pass
+
+
+class TickerAlreadyAdded(TickerException):
+    pass
+
+
+class TickerWaitException(TickerException, WaitException):
+    pass
+
+
+class TickerTerminated(TickerException, TerminatedException):
+    pass
+
+
+class TickerQuitException(TickerException, QuitException):
+    pass
+
+
+class AllTerminated(TickerException):
+    pass
+
+
+# -----------------------------------------------
+
+
+class ThreadEndException(Exception):
+    pass
+
+
+# -----------------------------------------------
+
+
+class BreakException(Exception):
+    pass
+
+
+# ----------------------------------------------
+
+
+class ServerError(Exception):
+    def __init__(self, msg):
+        self.msg = msg
```

### Comparing `fons-0.3.1/fons/event.py` & `fons-0.4.0/fons/event.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,955 +1,965 @@
-import asyncio
-import time
-import functools
-import queue as _queue
-from collections import defaultdict, namedtuple, Counter
-from concurrent.futures import Future
-
-from fons.aio import call_via_loop, call_via_loop_afut
-from fons.func import get_arg_count
-import fons.log as _log
-from fons.reg import create_name
-
-logger,logger2,tlogger,tloggers,tlogger0 = _log.get_standard_5(__name__)
-
-ROOT = 'temporary'
-_STATION_NAMES = set()
-_TRANSMITTER_NAMES = set()
-_NODE_NAMES = set()
-_empty = object()
-_qeitem = namedtuple('qe', 'queue event')
-_node_id = -1
-
-
-def set_root(value):
-    global ROOT
-    ROOT = value
-
-
-class Transmitter:
-    def __init__(self, name=None):
-        self._receptors = []
-        #self._loops = Counter()
-        self.name = create_name(name, self.__class__.__name__, _TRANSMITTER_NAMES)
-        
-
-    #def get_loops(self):
-    #    return [loop for loop, count in self._loops.items() if count]
-    
-    
-    def __iadd__(self, receptor):
-        self.prepare(receptor)
-        self._receptors.append(receptor)
-        #loop = getattr(receptor,'_loop',None)
-        #if isinstance(loop, asyncio.BaseEventLoop):
-        #    self._loops[loop] += 1
-        return self
-
-
-    def __isub__(self, receptor):
-        self._receptors.remove(receptor)
-        #loop = getattr(receptor,'_loop',None)
-        #if isinstance(loop, asyncio.BaseEventLoop):
-        #    self._loops[loop] -= 1
-        return self
-    
-    
-    def prepare(self, receptor):
-        pass
-    
-
-    def fire(self, *args, **kw):
-        raise NotImplementedError
-    
-    
-    @staticmethod
-    def fire_loop_partials(loop_partials):
-        for loop, partials in loop_partials.items():
-            Transmitter._call_loop(loop, partials)
-    
-    @staticmethod
-    def _call_loop(loop, partials):
-        f = functools.partial(Transmitter._call_all, partials)
-        if loop is None:
-            f()
-        elif loop.is_running():
-            loop.call_soon_threadsafe(f)
-        #If loop is not running then thread safety doesn't matter, right?
-        # (or unless multiple threads are accessing the queue simultaneously?)
-        else:
-            f()
-            
-    @staticmethod
-    def _call_all(partials):
-        for f in partials:
-            f()
-
-
-class EventTransmitter(Transmitter):
-    """Contains events"""
-    
-    def fire(self, *, op='set', **kw):
-        """set/clear all events"""
-        if not isinstance(op, str):
-            op = 'set' if bool(op) else 'clear'
-        loop_partials = defaultdict(list)
-                    
-        for event in self._receptors:            
-            loop = event._loop if isinstance(event, asyncio.Event) else None
-            loop_partials[loop].append(getattr(event, op))
-        
-        if kw.get('return_partials'):
-            return loop_partials
-        
-        self.fire_loop_partials(loop_partials)
-
-
-class QueueTransmitter(Transmitter):
-    """Contains queues"""
-    
-    def prepare(self, receptor):
-        receptor.messages_undelivered = 0
-        receptor.messages_behind = 0
-        
-        
-    def fire(self, item, *args, **kw):
-        """put an item to all queues"""
-        loop_partials = defaultdict(list)
-        for queue in self._receptors:
-            loop = queue._loop if isinstance(queue, asyncio.Queue) else None
-            p = functools.partial(self._put_to_queue, queue, item)
-            loop_partials[loop].append(p)
-        
-        if kw.get('return_partials'):
-            return loop_partials
-        
-        self.fire_loop_partials(loop_partials)  
-                
-                
-    def _put_to_queue(self, q, r):
-        nr_forced = force_put(q, r)
-        if nr_forced:
-            qname = getattr(q,'name','')
-            qnstr = " '{}'".format(qname) if qname else ''
-            if getattr(q,'warn',True):
-                logger2.warn('{} - had to discard {} item(s) in queue{}'\
-                             .format(self.name, nr_forced, qnstr))
-            q.messages_undelivered += nr_forced
-        else:
-            q.messages_behind += 1
-            
-    
-class Station:
-    def __init__(self, data=[], default_queue_size=0, 
-                 default_queue_cls=asyncio.Queue, 
-                 default_event_cls=asyncio.Event, *, 
-                 name=None, loops=[]):
-        self.storage = {}
-        self.qtransmitters = {}
-        self.etransmitters = {}
-        self.channels = set()
-        #maxsize 0 is infinite
-        self.default_queue_size = default_queue_size
-        self.default_queue_cls = default_queue_cls
-        self.default_event_cls = default_event_cls
-        self.channel_default_queue_sizes = {}
-        self.name = create_name(name, self.__class__.__name__, _STATION_NAMES)
-        #default loop for adding new queue/event
-        #if left to None, add will use .get_event_loop()
-        self._current_loop_id = 0
-        self.loops = {}
-        if isinstance(loops, dict):
-            for loop_id,loop in loops.items():
-                self.add_loop(loop,loop_id)
-        else:
-            for loop in loops:
-                self.add_loop(loop)
-
-        for item in data:
-            if item['channel'] not in self.channels:
-                self.add_channel(item['channel'], item.get('default_queue_size'))
-            item2 = {x:y for x,y in item.items() if x not in ('default_queue_size',)}
-            #if
-            if 'id' in item2:
-                self.add(**item2)
-        
-        
-    def add_channel(self, channel, default_queue_size=None):
-        if channel in self.channels:
-            raise ValueError('Channel {} already added'.format(channel))
-        self.channels.add(channel)
-        self.qtransmitters[channel] = QueueTransmitter(self.name+'[QT]')
-        self.etransmitters[channel] = EventTransmitter(self.name+'[ET]')
-        self.storage[channel] = defaultdict(dict)
-        self.channel_default_queue_sizes[channel] = default_queue_size
-        
-        
-    def add_loop(self, loop=None, id=None):
-        if id is None:
-            id = self._current_loop_id
-        if loop is None:
-            loop = asyncio.get_event_loop()
-            
-        if id in self.loops:
-            raise ValueError('Already taken id: {}'.format(id))
-        """elif loop in self.loops.values():
-            raise ValueError('Already existing loop: {}'.format(loop))"""
-        
-        self.loops[id] = loop
-        
-        if isinstance(id,int):
-            self._current_loop_id = max(self._current_loop_id, id + 1)
-        return id
-    
-    
-    def add(self, channel, id=None, queue=None, event=None, maxsize=None, loops=None):
-        if maxsize is None: 
-            maxsize = self.channel_default_queue_sizes[channel]
-        if maxsize is None: 
-            maxsize = self.default_queue_size 
-        
-        if queue is not None and event is not None and isinstance(queue, asyncio.Queue) and \
-            isinstance(event, asyncio.Event) and queue._loop is not event._loop:
-                raise ValueError("Queue's loop doesn't match with event's loop")
-            
-        if loops is None:
-            if queue is not None and isinstance(queue, asyncio.Queue):
-                loops = [queue._loop]
-            elif event is not None and isinstance(event, asyncio.Event):
-                loops = [event._loop]
-        loop_ids = self.get_loop_ids(loops, add=True)
-        #if id is None:
-        #    id = getattr(queue,'id',None)
-        if id is None:
-            id = self._create_id(channel, loop_ids)
-            
-        items = {}
-        for loop_id in loop_ids:
-            loop = self.loops[loop_id]
-            _queue,_event = queue,event
-            
-            if queue is False: _queue = None
-            elif queue is None:
-                kw = {'loop': loop} if self.default_queue_cls is asyncio.Queue else {}
-                _queue = self.default_queue_cls(maxsize, **kw)
-            elif isinstance(queue, asyncio.Queue) and queue._loop is not loop:
-                raise ValueError("Loop <{}> doesn't match with provided queue's loop".format(loop_id))
-            
-            if event is False: _event = None
-            elif event is None:
-                kw = {'loop': loop} if self.default_event_cls is asyncio.Event else {}
-                _event = self.default_event_cls(**kw)        
-            elif isinstance(event, asyncio.Event) and event._loop is not loop:
-                raise ValueError("Loop <{}> doesn't match with provided event's loop".format(loop_id))
-            
-            if _queue is None and _event is None:
-                continue
-            
-            new = _qeitem(_queue, _event)
-    
-            if id in self.storage[channel].get(loop_id, {}):
-                raise ValueError('Id "{}" has already been added to channel "{}"'.format(id, channel))
-            
-            if _queue is not None:
-                _queue.id = id
-                self.qtransmitters[channel] += _queue
-            if _event is not None:
-                _event.id = id
-                self.etransmitters[channel] += _event
-                
-            self.storage[channel][loop_id][id] = new
-            items[loop_id] = new
-            
-        return items
-        
-        
-    def add_queue(self, channel, id=None, queue=None, maxsize=None, loops=None):
-        items = self.add(channel,id,queue,False,maxsize,loops=loops)
-        return {loop_id: x.queue for loop_id, x in items.items()}
-    
-    
-    def add_event(self, channel, id=None, event=None, loops=None):
-        items = self.add(channel,id,False,event,loops=loops)
-        return {loop_id: x.event for loop_id, x in items.items()}
-    
-    
-    def remove(self, channel, id, loops=None):
-        """Does NOT raise error on non-existent"""
-        loop_ids = self.get_loop_ids(loops)
-        
-        for loop_id in loop_ids:
-            try: item = self.storage[loop_id].pop(id)
-            except KeyError:
-                continue
-            if item.queue is not None:
-                self.qtransmitters[channel] -= item.queue
-            if item.event is not None:
-                self.etransmitters[channel] -= item.event
-    
-    
-    def broadcast(self, channel, *put, op='set'):
-        if len(put) > 1:
-            raise ValueError(put)
-        if len(put):
-            item = put[0]
-            self.qtransmitters[channel].fire(item)
-        self.etransmitters[channel].fire(op=op)
-        
-        
-    def broadcast_multiple(self, instr):
-        """Ensures that multiple channel instructions with a shared loop 
-            are fired strictly sequentially (no breaks between).
-           :param instr: [{'_': channel, 'put': x, 'op': 'set'}, ...]
-                         keywords "put" and "op" are optional"""
-        loop_partials = defaultdict(list)
-        
-        for d in instr:
-            if 'channel' in d:
-                channel = d['channel']
-            elif '_' in d:
-                channel = d['_']
-            else:
-                raise KeyError('Missing keyword "channel" or "_"; got: {}'.format(d))
-            
-            qt_loop_partials = et_loop_partials = {}
-            
-            if 'put' in d:
-                item = d['put']
-                qt_loop_partials = self.qtransmitters[channel].fire(item, return_partials=True)
-                
-            if 'op' in d:
-                op = d['op']
-                et_loop_partials = self.etransmitters[channel].fire(op=op, return_partials=True)
-                
-            for x_loop_partials in (qt_loop_partials, et_loop_partials):
-                for loop, partials in x_loop_partials.items():
-                    loop_partials[loop] += partials
-                    
-        Transmitter.fire_loop_partials(loop_partials)
-        
-        
-    def get(self, channel, loop=None, ids=None):
-        if loop is None:
-            loop = asyncio.get_event_loop()
-
-        loop_id = self.get_loop_ids([loop])[0]
-        items = self.storage[channel][loop_id]
-        
-        if ids is None:
-            return items
-        elif hasattr(ids,'__iter__') and not isinstance(ids, str):
-            return [items[id] for id in ids]
-        else:
-            return items[ids]
-        
-        
-    def get_queue(self, channel, id, loop=None):
-        return self.get(channel, loop, id).queue
-    
-    
-    def get_event(self, channel, id, loop=None):
-        return self.get(channel, loop, id).event
-    
-    
-    def get_loop_ids(self, items=None, add=False):
-        """Items: keys and/or loops"""
-        if items is None: 
-            return list(self.loops.keys())
-        
-        ids = []
-        for x in items:
-            if isinstance(x, asyncio.BaseEventLoop):
-                try: id = next(id for id,loop in self.loops.items() if loop is x)
-                except StopIteration:
-                    if not add:
-                        raise ValueError('Not existing loop: {}'.format(x))
-                    id = self.add_loop(x)
-            elif x in self.loops:
-                id = x
-            else:
-                raise ValueError('Not existing id: {}'.format(x))
-            ids.append(id)
-            
-        return ids
-    
-    
-    def get_loops(self, items=None):
-        if items is None: 
-            return list(self.loops.values())
-        
-        loops = []
-        for x in items:
-            if not isinstance(x, asyncio.BaseEventLoop):
-                if x not in self.loops:
-                    raise ValueError(x)
-                loop = self.loops[x]
-            elif x in self.loops.values():
-                loop = x
-            else:
-                raise ValueError('Not existing loop: {}'.format(x))
-            loops.append(loop)
-            
-        return loops
-    
-    
-    def _create_id(self, channel, loop_ids):
-        id = 0
-        for loop_id in loop_ids:
-            ids = self.storage[channel].get(loop_id,{}).keys()
-            int_ids = (x for x in ids if isinstance(x,int))
-            try: id = max(id, max(int_ids)+1)
-            except ValueError: pass
-        return id
-    
-    def _print(self):
-        print(self.storage)
-        print({_id: id(loop) for _id,loop in self.loops.items()})
-        
-
-class Event:
-    __slots__ = ('id','type','data','ts')
-    
-    def __init__(self, id, type, data):
-        self.id = id
-        self.type = type
-        self.data = data
-        self.ts = time.time()
-        
-        
-    def __getitem__(self, index):
-        return (self.id, self.type, self.data, self.ts)[index]
-    
-    def __iter__(self):
-        return iter((self.id, self.type, self.data, self.ts))
-
-
-class RelayPackage:
-    __slots__ = ('data','source','handler','channel','current_handler')
-    
-    def __init__(self, data, source=None, handler=None, channel=None, current_handler=None):
-        """
-        :type source: Node
-        :type handler: Handler
-        :type current_handler: Handler
-        """
-        self.data = data
-        self.source = source
-        self.handler = handler
-        self.channel = channel
-        self.current_handler = current_handler
-        
-    def copy(self, **kw):
-        
-        return self.__class__(**dict({'data': self.data,
-                                      'source': self.source,
-                                      'handler': self.handler,
-                                      'channel': self.channel,
-                                      'current_handler': self.current_handler}, 
-                                     **kw))
-
-
-class RelayInfo:
-    __slots__ = ('items',)
-    
-    def __init__(self, items=[]):
-        self.items = list(items)
-        
-    def add_item(self, value, channels):
-        self.items.append((value, channels))
-        
-
-class NodeExit:
-    """Put this into node to signal it to stop listening"""
-    pass
-
-
-class Node:
-    def __init__(self, clients=[], handlers=[], groups=[], *, loop=None, root=None, name=None):
-        """
-        Node ids are negative, as are the station channels reserved for them individually.
-        Channels grouping multiple nodes together must be positive or non-int.
-        Handlers are functions that input the RelayPackage received by the ._queue,
-         output a value, which is then wrapped with RelayPackage and forwarded to
-         all channels associated with the handler.
-        Channel <0> contains all connected nodes, which is also the default channel of the root_handler.
-        :param root:
-            about .root_handler (which forwards the unadulterated data to all connected nodes)
-            ::None: defaults to ROOT ("temporary" by default)
-            ::True: root handler will be added on initiation
-            ::"temporary": -||-, but removed when .add_handler is called the first time
-                           (including in `handlers` argument)
-            ::"temp": == "temporary"
-            ::False: root handler will not be added
-        To start serving:
-            node.serve()
-        """
-        global _node_id
-        
-        if name is None:
-            name = abs(_node_id)
-            
-        self.id = _node_id
-        self.name = create_name(name, default=self.__class__.__name__, registry=_NODE_NAMES)
-        
-        _node_id -= 1
-        
-        # Initiate with channel 0
-        self.station = Station([{'channel': 0}])
-        self._queue = asyncio.Queue(loop=loop)
-        #self._user_queue = asyncio.Queue(maxlen=self.user_maxlen, loop=loop)
-        self.loop = self._queue._loop
-        self.futures = {'serve': None}
-        self.handlers = []
-        
-        # ie nodes that receive from (the handlers of) this node
-        self.clients_by_id = {}
-        # ie the channels that each client receives from
-        self.client_channels = {}
-        
-        self._last_handler_id = -1
-        if root is None:
-            root = ROOT
-        self._root = root
-        self._root_handler_overriden = False
-        # Root handler just forwards the received data to all connected nodes
-        # it will be removed as soon as the first handler is added
-        self.root_handler = NodeHandler(self, lambda x: x.data, [0], id='root')
-        
-        if root:
-            self.handlers.append(self.root_handler)
-        
-        for node_specs in clients:
-            kwargs = node_specs[1] if len(node_specs) > 1 else {}
-            self.connect(*node_specs[0],**kwargs)
-        
-        for group_specs in groups:
-            kwargs = group_specs[1] if len(group_specs) > 1 else {}
-            self.group(*group_specs[0],**kwargs)
-        
-        for handler_specs in handlers:
-            kwargs = handler_specs[1] if len(handler_specs) > 1 else {}
-            self.add_handler(*handler_specs[0],**kwargs)
-    
-    
-    def connect(self, node, *channels):
-        """Add recipient node"""
-        if not isinstance(node, Node):
-            raise TypeError("`node` must be of type Node, got: {}".format(type(node)))
-        if node.id in self.clients_by_id:
-            raise ValueError("Node <{}> has already been added".format(node.id))
-        
-        if node.id not in self.station.channels:
-            self.station.add_channel(node.id)
-        
-        self.clients_by_id[node.id] = node
-        self.station.add_queue(node.id, id=0, queue=node._queue)
-        self.station.add_queue(0, id=node.id, queue=node._queue)
-        
-        for channel in channels:
-            self.group(channel, node)
-        
-        self.client_channels[node.id] = set([node.id])
-    
-    
-    def disconnect(self, node):
-        """Deletes all traces of the node. The channels in handlers' lists remain,
-           but the channel itself just doesn't contain the node any more."""
-        if not isinstance(node, Node):
-            node = self.clients_by_id[node]
-        del self.clients_by_id[node.id]
-        # station.remove doesn't raise error on non-existent
-        self.station.remove(node.id, id=0)
-        self.station.remove(0, id=node.id)
-        client_channels = self.client_channels[node.id]
-        for channel in client_channels:
-            self.station.remove(channel, id=node.id)
-        del self.client_channels[node.id]
-    
-    
-    def group(self, channel, *nodes):
-        """Registers the given nodes under the channel"""
-        if isinstance(channel, int) and channel <= 0:
-            raise ValueError('Channel must be > 0, got: {}'.format(channel))
-        
-        if channel not in self.station.channels:
-            self.station.add_channel(channel)
-        
-        for node in nodes:
-            if not isinstance(node, Node):
-                node = self.clients_by_id[node]
-            self.station.add_queue(channel, id=node.id, queue=node._queue)
-            self.client_channels[node.id].add(channel)
-    
-    
-    def ungroup(self, channel, *nodes):
-        """Disassociates the given nodes from the channel""" 
-           
-        if isinstance(channel, int) and channel < 0:
-            raise ValueError('Channel must be >= 0, got: {}'.format(channel))
-        
-        for node in nodes:
-            if not isinstance(node, Node):
-                node = self.clients_by_id[node]
-            self.station.remove(channel, id=node.id)
-            self.client_channels[node.id].remove(channel)
-    
-    
-    def add_handler(self, f, *recipients, id=None, loop=None, type=None):
-        if loop is None:
-            loop = self.loop
-        if not isinstance(f, NodeHandler):
-            handler = NodeHandler(self, f, id=id, loop=loop, type=type)
-        else:
-            handler = f
-            if handler.node != self:
-                raise ValueError('Handler connected to wrong node.')
-        for rcp in recipients:
-            handler.add_recipient(rcp)
-        if not self._root_handler_overriden and self._root in ('temp','temporary'):
-            try: self.remove_handler(self.root_handler)
-            except ValueError: pass
-            self._root_handler_overriden = True
-        self.handlers.append(handler)
-        
-        return handler
-    
-    
-    def remove_handler(self, handler):
-        """:param handler: NodeHandler or its id"""
-        if not isinstance(handler, NodeHandler):
-            id = handler
-            handler = next((x for x in self.handlers if x.id == id), None)
-            if handler is None:
-                raise ValueError('No handler matching id: {}'.format(id))
-        self.handlers.remove(handler)
-    
-    
-    def has_client(self, node):
-        """:param node: Node or its id"""
-        node_id = node.id if isinstance(node, Node) else node
-        
-        return node_id in self.clients_by_id
-    
-    
-    def serve(self):
-        """Start listening and handling any received."""
-        if self.is_running():
-            return
-        self.futures['serve'] = \
-            call_via_loop_afut(self._serve, loop=self.loop)
-    
-    
-    async def _serve(self):
-        try:
-            while True:
-                inp = await self._queue.get()
-                if isinstance(inp, NodeExit):
-                    break
-                self.handle(inp)
-        finally:
-            for handler in self.handlers:
-                handler.stop()
-    
-    
-    def handle(self, inp):
-        for handler in self.handlers:
-            handler.handle(inp)
-    
-    
-    async def recv(self):
-        """Receive directly, skipping the handlers"""
-        if self.is_running():
-            raise RuntimeError('Cannot receive directly while node is running.')
-        
-        return await self._queue.get()
-    
-    
-    def recv_nowait(self):
-        return self._queue.get_nowait()
-    
-    
-    def relay(self, data, *channels):
-        """Relays directly, skipping the handlers"""
-        if not channels:
-            channels = [0]
-        pks = [RelayPackage(data, self, None, channel)
-               for channel in channels]
-        self.station.broadcast_multiple(
-            [{'channel': pk.channel, 'put': pk} for pk in pks])
-    
-    
-    def put(self, x, ensure_is_packed=True):
-        """
-        Put something into node's input queue
-        (if node is running it is immediately received by all its handlers).
-        :rtype: asyncio.Future
-        """
-        if ensure_is_packed and not isinstance(x, RelayPackage):
-            x = RelayPackage(x, None, None, None)
-        
-        return call_via_loop_afut(self._queue.put, (x,), loop=self._queue._loop)
-    
-    
-    def put_nowait(self, x, ensure_is_packed=True):
-        """:rtype: Future"""
-        if ensure_is_packed and not isinstance(x, RelayPackage):
-            x = RelayPackage(x, None, None, None)
-        
-        return put_via_loop(self._queue, x)
-    
-    
-    def empty(self):
-        return self._queue.empty()
-    
-    
-    def full(self):
-        return self._queue.full()
-    
-    
-    def is_running(self):
-        return self.futures['serve'] is not None \
-            and not self.futures['serve'].done()
-    
-    
-    def stop(self):
-        self.put(NodeExit())
-    
-    
-    def __repr__(self):
-        return '{}(id={},name={})'.format(self.__class__.__name__, self.id, self.name)
-
-
-class NodeHandler:
-    def __init__(self, node, target=None, recipients=[], *, loop=None, id=None, type=None):
-        """
-        :type node: Node
-        Handles the input received by its node.
-        :param type:
-            describes the `target`
-            ::None    - target is synchronous function
-                         - accepts the node input* as its first argument
-                         - returns output (which is then relayed by the handler)
-            ::"async" - a continuous "listener" coroutine function that
-                         - *may* accept `handler` (self) as its first argument
-                         - receives node input by awaiting on handler.recv(), 
-                         - relays the output data independently (handler.relay(data))
-                         - exits on NodeExit()
-            ::"gen"   - a function that returns generator
-                         - function *may* accept `handler` (self) as its first argument
-                        where the generator
-                         - receives node input via `yield` keyword
-                         - yields the output (which is then relayed by the handler)
-                         - exhausts on NodeExit()
-            * node input: The data received by node, which is assumed to be wrapped with RelayPackage,
-                          or will be (in .handle) if not already done so
-        """
-        self.node = node
-        if loop is None:
-            loop = node.loop
-        self._queue = asyncio.Queue(loop=loop)
-        self.loop = self._queue._loop
-        self.channels = []
-        
-        self.target = target
-        if type not in ('async','gen',None):
-            raise ValueError(type)
-        self._type = type
-        #if asyncio.iscoroutinefunction(target):
-        #    self._type = 'async'
-        
-        if id is None:
-            self.node._last_handler_id += 1
-            id = self.node._last_handler_id
-        else:
-            if any(x.id==id for x in self.node.handlers):
-                raise ValueError('A handler with id <{}> already exits'.format(id))
-            if isinstance(id, int):
-                self.node._last_handler_id = max(id, self.node._last_handler_id)
-                
-        self.id = id
-        self._started = False
-        
-        for rcp in recipients:
-            self.add_recipient(rcp)
-    
-    
-    def _start(self):
-        if self._started:
-            return
-        
-        args = (self,) if get_arg_count(self.target) else ()
-        
-        if self._type is None:
-            pass
-        elif self._type == 'gen':
-            self._gen = self.target(*args)
-            self._gen.send(None)
-        else:
-            call_via_loop(self.target, args, loop=self.loop)
-        self._started = True
-    
-    
-    def handle(self, x):
-        if not isinstance(x, RelayPackage):
-            x = RelayPackage(x, None, None, None, self)
-        else:
-            x = x.copy(current_handler=self)
-        
-        if self._type is None:
-            data = self.target(x)
-            self.relay(data)
-        elif self._type == 'gen':
-            # Generator
-            self._start()
-            data = self._gen.send(x)
-            self.relay(data)
-        else:
-            # Asynchronous
-            self._start()
-            self.put(x)
-    
-    
-    async def recv(self):
-        """This is only meant to be used in *asynchronous* target function of the handler"""
-        return await self._queue.get()
-    
-    
-    def recv_nowait(self):
-        return self._queue.get_nowait()
-    
-    
-    def relay(self, data):
-        """Relay the handler-processed data (wrapped with RelayPackage) to handler's nodes"""
-        if isinstance(data, RelayInfo):
-            return self._relay_by_info(data)
-        
-        # Also include the source node (self) and the associated channel
-        pks = [RelayPackage(data, self.node, self, channel)
-               for channel in self.channels]
-        self.node.station.broadcast_multiple(
-            [{'channel': pk.channel, 'put': pk} for pk in pks])
-    
-    
-    def _relay_by_info(self, info):
-        """:type info: RelayInfo"""
-        pks = []
-        
-        for data,to_channels in info.items:
-            for channel in to_channels:
-                pk = RelayPackage(data, self.node, self, channel)
-                pks.append(pk)
-                
-        self.node.station.broadcast_multiple(
-            [{'channel': pk.channel, 'put': pk} for pk in pks])
-    
-    
-    def add_recipient(self, channel, create=False):
-        """:param channel: channel or Node"""
-        node = None
-        if isinstance(channel, Node):
-            node = channel
-            channel = node.id
-            
-        if channel not in self.node.station.channels:
-            if not create:
-                raise ValueError("Channel <{}> hasn't been added yet".format(channel))
-            if node is not None:
-                self.node.connect(node)
-            else:
-                self.node.group(channel)
-        
-        if channel in self.channels:
-            raise ValueError("Channel <{}> already added to handler {}".format(channel, self.id))
-        
-        self.channels.append(channel)
-    
-    
-    def remove_recipient(self, channel):
-        if isinstance(channel, Node):
-            channel = channel.id
-        self.channels.remove(channel)
-    
-    
-    def put(self, x, ensure_is_packed=True):
-        """
-        Put something into handler's input queue 
-        (only received if the handler has asynchronous target)
-        :rtype: asyncio.Future
-        """
-        if ensure_is_packed and not isinstance(x, RelayPackage):
-            x = RelayPackage(x, None, None, None)
-        
-        return call_via_loop_afut(self._queue.put, (x,), loop=self._queue._loop)
-    
-    
-    def put_nowait(self, x, ensure_is_packed=True):
-        """:rtype: Future"""
-        if ensure_is_packed and not isinstance(x, RelayPackage):
-            x = RelayPackage(x, None, None, None)
-        
-        return put_via_loop(self._queue, x)
-    
-    
-    def empty(self):
-        return self._queue.empty()
-    
-    
-    def full(self):
-        return self._queue.full()
-    
-    
-    def is_running(self):
-        return self._started
-    
-     
-    def stop(self):
-        if not self._started:
-            return
-        if self._type is None:
-            pass
-        elif self._type == 'gen':
-            try: self._gen.send(NodeExit())
-            except StopIteration: pass
-        else:
-            self.put(NodeExit())
-        self._started = False
-
-
-
-def force_put(queue, item):
-    nr_removed = 0
-    while True:
-        try: queue.put_nowait(item)
-        #multiprocessing.Queue also raises queue.Full
-        except (_queue.Full,asyncio.QueueFull):
-            try: queue.get_nowait()
-            except (_queue.Full,asyncio.QueueEmpty): pass
-            else: nr_removed += 1
-        else: break
-    return nr_removed
-
-
-def empty_queue(queue, return_items=False):
-    nr_removed = 0
-    received = []
-    try:
-        while True:
-            item = queue.get_nowait()
-            if return_items:
-                received.append(item)
-            else:
-                nr_removed += 1
-    except (_queue.Empty,asyncio.QueueEmpty):
-        pass
-    return received if return_items else nr_removed
-
-
-def put_via_loop(queue, x):
-    """Put something into queue"""
-    p = functools.partial(queue.put_nowait, x)
-    if asyncio.get_event_loop() is queue._loop:
-        f = Future()
-        f.set_result(p())
-        return f
-    else:
-        return call_via_loop(p, loop=queue._loop)
+import asyncio
+import time
+import functools
+import queue as _queue
+from collections import defaultdict, namedtuple, Counter
+from concurrent.futures import Future
+
+from fons.aio import (
+    call_via_loop,
+    call_via_loop_afut,
+    FonsEvent,
+    FonsQueue,
+    _check_is_fons_queue,
+    _check_is_fons_event,
+)
+from fons.func import get_arg_count
+import fons.log as _log
+from fons.reg import create_name
+
+logger, logger2, tlogger, tloggers, tlogger0 = _log.get_standard_5(__name__)
+
+ROOT = "temporary"
+_STATION_NAMES = set()
+_TRANSMITTER_NAMES = set()
+_NODE_NAMES = set()
+_empty = object()
+_qeitem = namedtuple("qe", "queue event")
+_node_id = -1
+
+
+def set_root(value):
+    global ROOT
+    ROOT = value
+
+
+class Transmitter:
+    def __init__(self, name=None):
+        self._receptors = []
+        # self._loops = Counter()
+        self.name = create_name(name, self.__class__.__name__, _TRANSMITTER_NAMES)
+
+    # def get_loops(self):
+    #    return [loop for loop, count in self._loops.items() if count]
+
+    def __iadd__(self, receptor):
+        self.prepare(receptor)
+        self._receptors.append(receptor)
+        # loop = getattr(receptor,'_loop',None)
+        # if isinstance(loop, asyncio.BaseEventLoop):
+        #    self._loops[loop] += 1
+        return self
+
+    def __isub__(self, receptor):
+        self._receptors.remove(receptor)
+        # loop = getattr(receptor,'_loop',None)
+        # if isinstance(loop, asyncio.BaseEventLoop):
+        #    self._loops[loop] -= 1
+        return self
+
+    def prepare(self, receptor):
+        pass
+
+    def fire(self, *args, **kw):
+        raise NotImplementedError
+
+    @staticmethod
+    def fire_loop_partials(loop_partials):
+        for loop, partials in loop_partials.items():
+            Transmitter._call_loop(loop, partials)
+
+    @staticmethod
+    def _call_loop(loop, partials):
+        f = functools.partial(Transmitter._call_all, partials)
+        if loop is None:
+            f()
+        elif loop.is_running():
+            loop.call_soon_threadsafe(f)
+        # If loop is not running then thread safety doesn't matter, right?
+        # (or unless multiple threads are accessing the queue simultaneously?)
+        else:
+            f()
+
+    @staticmethod
+    def _call_all(partials):
+        for f in partials:
+            f()
+
+
+class EventTransmitter(Transmitter):
+    """Contains events"""
+
+    def fire(self, *, op="set", **kw):
+        """set/clear all events"""
+        if not isinstance(op, str):
+            op = "set" if bool(op) else "clear"
+        loop_partials = defaultdict(list)
+
+        for event in self._receptors:
+            loop = event._loop if isinstance(event, asyncio.Event) else None
+            loop_partials[loop].append(getattr(event, op))
+
+        if kw.get("return_partials"):
+            return loop_partials
+
+        self.fire_loop_partials(loop_partials)
+
+
+class QueueTransmitter(Transmitter):
+    """Contains queues"""
+
+    def prepare(self, receptor):
+        receptor.messages_undelivered = 0
+        receptor.messages_behind = 0
+
+    def fire(self, item, *args, **kw):
+        """put an item to all queues"""
+        loop_partials = defaultdict(list)
+        for queue in self._receptors:
+            loop = queue._loop if isinstance(queue, asyncio.Queue) else None
+            p = functools.partial(self._put_to_queue, queue, item)
+            loop_partials[loop].append(p)
+
+        if kw.get("return_partials"):
+            return loop_partials
+
+        self.fire_loop_partials(loop_partials)
+
+    def _put_to_queue(self, q, r):
+        nr_forced = force_put(q, r)
+        if nr_forced:
+            qname = getattr(q, "name", "")
+            qnstr = " '{}'".format(qname) if qname else ""
+            if getattr(q, "warn", True):
+                logger2.warn(
+                    "{} - had to discard {} item(s) in queue{}".format(
+                        self.name, nr_forced, qnstr
+                    )
+                )
+            q.messages_undelivered += nr_forced
+        else:
+            q.messages_behind += 1
+
+
+class Station:
+    def __init__(
+        self,
+        data=[],
+        default_queue_size=0,
+        default_queue_cls=FonsQueue,
+        default_event_cls=FonsEvent,
+        *,
+        name=None,
+        loops=[]
+    ):
+        self.storage = {}
+        self.qtransmitters = {}
+        self.etransmitters = {}
+        self.channels = set()
+        # maxsize 0 is infinite
+        self.default_queue_size = default_queue_size
+        self.default_queue_cls = default_queue_cls
+        self.default_event_cls = default_event_cls
+        self.channel_default_queue_sizes = {}
+        self.name = create_name(name, self.__class__.__name__, _STATION_NAMES)
+        # default loop for adding new queue/event
+        # if left to None, add will use .get_event_loop()
+        self._current_loop_id = 0
+        self.loops = {}
+        if isinstance(loops, dict):
+            for loop_id, loop in loops.items():
+                self.add_loop(loop, loop_id)
+        else:
+            for loop in loops:
+                self.add_loop(loop)
+
+        for item in data:
+            if item["channel"] not in self.channels:
+                self.add_channel(item["channel"], item.get("default_queue_size"))
+            item2 = {x: y for x, y in item.items() if x not in ("default_queue_size",)}
+            # if
+            if "id" in item2:
+                self.add(**item2)
+
+    def add_channel(self, channel, default_queue_size=None):
+        if channel in self.channels:
+            raise ValueError("Channel {} already added".format(channel))
+        self.channels.add(channel)
+        self.qtransmitters[channel] = QueueTransmitter(self.name + "[QT]")
+        self.etransmitters[channel] = EventTransmitter(self.name + "[ET]")
+        self.storage[channel] = defaultdict(dict)
+        self.channel_default_queue_sizes[channel] = default_queue_size
+
+    def add_loop(self, loop=None, id=None):
+        if id is None:
+            id = self._current_loop_id
+        if loop is None:
+            loop = asyncio.get_event_loop()
+
+        if id in self.loops:
+            raise ValueError("Already taken id: {}".format(id))
+        """elif loop in self.loops.values():
+            raise ValueError('Already existing loop: {}'.format(loop))"""
+
+        self.loops[id] = loop
+
+        if isinstance(id, int):
+            self._current_loop_id = max(self._current_loop_id, id + 1)
+        return id
+
+    def add(self, channel, id=None, queue=None, event=None, maxsize=None, loops=None):
+        if maxsize is None:
+            maxsize = self.channel_default_queue_sizes[channel]
+        if maxsize is None:
+            maxsize = self.default_queue_size
+
+        if isinstance(queue, asyncio.Queue):
+            _check_is_fons_queue(queue)
+        if isinstance(event, asyncio.Event):
+            _check_is_fons_event(event)
+
+        if (
+            queue is not None
+            and event is not None
+            and isinstance(queue, asyncio.Queue)
+            and isinstance(event, asyncio.Event)
+            and queue._loop is not event._loop
+        ):
+            raise ValueError("Queue's loop doesn't match with event's loop")
+
+        if loops is None:
+            if queue is not None and isinstance(queue, asyncio.Queue):
+                loops = [queue._loop]
+            elif event is not None and isinstance(event, asyncio.Event):
+                loops = [event._loop]
+        loop_ids = self.get_loop_ids(loops, add=True)
+        # if id is None:
+        #    id = getattr(queue,'id',None)
+        if id is None:
+            id = self._create_id(channel, loop_ids)
+
+        items = {}
+        for loop_id in loop_ids:
+            loop = self.loops[loop_id]
+            _queue, _event = queue, event
+
+            if queue is False:
+                _queue = None
+            elif queue is None:
+                kw = {"loop": loop} if self.default_queue_cls is FonsQueue else {}
+                _queue = self.default_queue_cls(maxsize, **kw)
+            elif isinstance(queue, asyncio.Queue) and queue._loop is not loop:
+                raise ValueError(
+                    "Loop <{}> doesn't match with provided queue's loop".format(loop_id)
+                )
+
+            if event is False:
+                _event = None
+            elif event is None:
+                kw = {"loop": loop} if self.default_event_cls is FonsEvent else {}
+                _event = self.default_event_cls(**kw)
+            elif isinstance(event, asyncio.Event) and event._loop is not loop:
+                raise ValueError(
+                    "Loop <{}> doesn't match with provided event's loop".format(loop_id)
+                )
+
+            if _queue is None and _event is None:
+                continue
+
+            new = _qeitem(_queue, _event)
+
+            if id in self.storage[channel].get(loop_id, {}):
+                raise ValueError(
+                    'Id "{}" has already been added to channel "{}"'.format(id, channel)
+                )
+
+            if _queue is not None:
+                _queue.id = id
+                self.qtransmitters[channel] += _queue
+            if _event is not None:
+                _event.id = id
+                self.etransmitters[channel] += _event
+
+            self.storage[channel][loop_id][id] = new
+            items[loop_id] = new
+
+        return items
+
+    def add_queue(self, channel, id=None, queue=None, maxsize=None, loops=None):
+        items = self.add(channel, id, queue, False, maxsize, loops=loops)
+        return {loop_id: x.queue for loop_id, x in items.items()}
+
+    def add_event(self, channel, id=None, event=None, loops=None):
+        items = self.add(channel, id, False, event, loops=loops)
+        return {loop_id: x.event for loop_id, x in items.items()}
+
+    def remove(self, channel, id, loops=None):
+        """Does NOT raise error on non-existent"""
+        loop_ids = self.get_loop_ids(loops)
+
+        for loop_id in loop_ids:
+            try:
+                item = self.storage[loop_id].pop(id)
+            except KeyError:
+                continue
+            if item.queue is not None:
+                self.qtransmitters[channel] -= item.queue
+            if item.event is not None:
+                self.etransmitters[channel] -= item.event
+
+    def broadcast(self, channel, *put, op="set"):
+        if len(put) > 1:
+            raise ValueError(put)
+        if len(put):
+            item = put[0]
+            self.qtransmitters[channel].fire(item)
+        self.etransmitters[channel].fire(op=op)
+
+    def broadcast_multiple(self, instr):
+        """Ensures that multiple channel instructions with a shared loop
+         are fired strictly sequentially (no breaks between).
+        :param instr: [{'_': channel, 'put': x, 'op': 'set'}, ...]
+                      keywords "put" and "op" are optional"""
+        loop_partials = defaultdict(list)
+
+        for d in instr:
+            if "channel" in d:
+                channel = d["channel"]
+            elif "_" in d:
+                channel = d["_"]
+            else:
+                raise KeyError('Missing keyword "channel" or "_"; got: {}'.format(d))
+
+            qt_loop_partials = et_loop_partials = {}
+
+            if "put" in d:
+                item = d["put"]
+                qt_loop_partials = self.qtransmitters[channel].fire(
+                    item, return_partials=True
+                )
+
+            if "op" in d:
+                op = d["op"]
+                et_loop_partials = self.etransmitters[channel].fire(
+                    op=op, return_partials=True
+                )
+
+            for x_loop_partials in (qt_loop_partials, et_loop_partials):
+                for loop, partials in x_loop_partials.items():
+                    loop_partials[loop] += partials
+
+        Transmitter.fire_loop_partials(loop_partials)
+
+    def get(self, channel, loop=None, ids=None):
+        if loop is None:
+            loop = asyncio.get_event_loop()
+
+        loop_id = self.get_loop_ids([loop])[0]
+        items = self.storage[channel][loop_id]
+
+        if ids is None:
+            return items
+        elif hasattr(ids, "__iter__") and not isinstance(ids, str):
+            return [items[id] for id in ids]
+        else:
+            return items[ids]
+
+    def get_queue(self, channel, id, loop=None):
+        return self.get(channel, loop, id).queue
+
+    def get_event(self, channel, id, loop=None):
+        return self.get(channel, loop, id).event
+
+    def get_loop_ids(self, items=None, add=False):
+        """Items: keys and/or loops"""
+        if items is None:
+            return list(self.loops.keys())
+
+        ids = []
+        for x in items:
+            if isinstance(x, asyncio.BaseEventLoop):
+                try:
+                    id = next(id for id, loop in self.loops.items() if loop is x)
+                except StopIteration:
+                    if not add:
+                        raise ValueError("Not existing loop: {}".format(x))
+                    id = self.add_loop(x)
+            elif x in self.loops:
+                id = x
+            else:
+                raise ValueError("Not existing id: {}".format(x))
+            ids.append(id)
+
+        return ids
+
+    def get_loops(self, items=None):
+        if items is None:
+            return list(self.loops.values())
+
+        loops = []
+        for x in items:
+            if not isinstance(x, asyncio.BaseEventLoop):
+                if x not in self.loops:
+                    raise ValueError(x)
+                loop = self.loops[x]
+            elif x in self.loops.values():
+                loop = x
+            else:
+                raise ValueError("Not existing loop: {}".format(x))
+            loops.append(loop)
+
+        return loops
+
+    def _create_id(self, channel, loop_ids):
+        id = 0
+        for loop_id in loop_ids:
+            ids = self.storage[channel].get(loop_id, {}).keys()
+            int_ids = (x for x in ids if isinstance(x, int))
+            try:
+                id = max(id, max(int_ids) + 1)
+            except ValueError:
+                pass
+        return id
+
+    def _print(self):
+        print(self.storage)
+        print({_id: id(loop) for _id, loop in self.loops.items()})
+
+
+class Event:
+    __slots__ = ("id", "type", "data", "ts")
+
+    def __init__(self, id, type, data):
+        self.id = id
+        self.type = type
+        self.data = data
+        self.ts = time.time()
+
+    def __getitem__(self, index):
+        return (self.id, self.type, self.data, self.ts)[index]
+
+    def __iter__(self):
+        return iter((self.id, self.type, self.data, self.ts))
+
+
+class RelayPackage:
+    __slots__ = ("data", "source", "handler", "channel", "current_handler")
+
+    def __init__(
+        self, data, source=None, handler=None, channel=None, current_handler=None
+    ):
+        """
+        :type source: Node
+        :type handler: Handler
+        :type current_handler: Handler
+        """
+        self.data = data
+        self.source = source
+        self.handler = handler
+        self.channel = channel
+        self.current_handler = current_handler
+
+    def copy(self, **kw):
+        return self.__class__(
+            **dict(
+                {
+                    "data": self.data,
+                    "source": self.source,
+                    "handler": self.handler,
+                    "channel": self.channel,
+                    "current_handler": self.current_handler,
+                },
+                **kw
+            )
+        )
+
+
+class RelayInfo:
+    __slots__ = ("items",)
+
+    def __init__(self, items=[]):
+        self.items = list(items)
+
+    def add_item(self, value, channels):
+        self.items.append((value, channels))
+
+
+class NodeExit:
+    """Put this into node to signal it to stop listening"""
+
+    pass
+
+
+class Node:
+    def __init__(
+        self, clients=[], handlers=[], groups=[], *, loop=None, root=None, name=None
+    ):
+        """
+        Node ids are negative, as are the station channels reserved for them individually.
+        Channels grouping multiple nodes together must be positive or non-int.
+        Handlers are functions that input the RelayPackage received by the ._queue,
+         output a value, which is then wrapped with RelayPackage and forwarded to
+         all channels associated with the handler.
+        Channel <0> contains all connected nodes, which is also the default channel of the root_handler.
+        :param root:
+            about .root_handler (which forwards the unadulterated data to all connected nodes)
+            ::None: defaults to ROOT ("temporary" by default)
+            ::True: root handler will be added on initiation
+            ::"temporary": -||-, but removed when .add_handler is called the first time
+                           (including in `handlers` argument)
+            ::"temp": == "temporary"
+            ::False: root handler will not be added
+        To start serving:
+            node.serve()
+        """
+        global _node_id
+
+        if name is None:
+            name = abs(_node_id)
+
+        self.id = _node_id
+        self.name = create_name(
+            name, default=self.__class__.__name__, registry=_NODE_NAMES
+        )
+
+        _node_id -= 1
+
+        # Initiate with channel 0
+        self.station = Station([{"channel": 0}])
+        self._queue = FonsQueue(loop=loop)
+        # self._user_queue = FonsQueue(maxlen=self.user_maxlen, loop=loop)
+        self.loop = self._queue._loop
+        self.futures = {"serve": None}
+        self.handlers = []
+
+        # ie nodes that receive from (the handlers of) this node
+        self.clients_by_id = {}
+        # ie the channels that each client receives from
+        self.client_channels = {}
+
+        self._last_handler_id = -1
+        if root is None:
+            root = ROOT
+        self._root = root
+        self._root_handler_overriden = False
+        # Root handler just forwards the received data to all connected nodes
+        # it will be removed as soon as the first handler is added
+        self.root_handler = NodeHandler(self, lambda x: x.data, [0], id="root")
+
+        if root:
+            self.handlers.append(self.root_handler)
+
+        for node_specs in clients:
+            kwargs = node_specs[1] if len(node_specs) > 1 else {}
+            self.connect(*node_specs[0], **kwargs)
+
+        for group_specs in groups:
+            kwargs = group_specs[1] if len(group_specs) > 1 else {}
+            self.group(*group_specs[0], **kwargs)
+
+        for handler_specs in handlers:
+            kwargs = handler_specs[1] if len(handler_specs) > 1 else {}
+            self.add_handler(*handler_specs[0], **kwargs)
+
+    def connect(self, node, *channels):
+        """Add recipient node"""
+        if not isinstance(node, Node):
+            raise TypeError("`node` must be of type Node, got: {}".format(type(node)))
+        if node.id in self.clients_by_id:
+            raise ValueError("Node <{}> has already been added".format(node.id))
+
+        if node.id not in self.station.channels:
+            self.station.add_channel(node.id)
+
+        self.clients_by_id[node.id] = node
+        self.station.add_queue(node.id, id=0, queue=node._queue)
+        self.station.add_queue(0, id=node.id, queue=node._queue)
+
+        for channel in channels:
+            self.group(channel, node)
+
+        self.client_channels[node.id] = set([node.id])
+
+    def disconnect(self, node):
+        """Deletes all traces of the node. The channels in handlers' lists remain,
+        but the channel itself just doesn't contain the node any more."""
+        if not isinstance(node, Node):
+            node = self.clients_by_id[node]
+        del self.clients_by_id[node.id]
+        # station.remove doesn't raise error on non-existent
+        self.station.remove(node.id, id=0)
+        self.station.remove(0, id=node.id)
+        client_channels = self.client_channels[node.id]
+        for channel in client_channels:
+            self.station.remove(channel, id=node.id)
+        del self.client_channels[node.id]
+
+    def group(self, channel, *nodes):
+        """Registers the given nodes under the channel"""
+        if isinstance(channel, int) and channel <= 0:
+            raise ValueError("Channel must be > 0, got: {}".format(channel))
+
+        if channel not in self.station.channels:
+            self.station.add_channel(channel)
+
+        for node in nodes:
+            if not isinstance(node, Node):
+                node = self.clients_by_id[node]
+            self.station.add_queue(channel, id=node.id, queue=node._queue)
+            self.client_channels[node.id].add(channel)
+
+    def ungroup(self, channel, *nodes):
+        """Disassociates the given nodes from the channel"""
+
+        if isinstance(channel, int) and channel < 0:
+            raise ValueError("Channel must be >= 0, got: {}".format(channel))
+
+        for node in nodes:
+            if not isinstance(node, Node):
+                node = self.clients_by_id[node]
+            self.station.remove(channel, id=node.id)
+            self.client_channels[node.id].remove(channel)
+
+    def add_handler(self, f, *recipients, id=None, loop=None, type=None):
+        if loop is None:
+            loop = self.loop
+        if not isinstance(f, NodeHandler):
+            handler = NodeHandler(self, f, id=id, loop=loop, type=type)
+        else:
+            handler = f
+            if handler.node != self:
+                raise ValueError("Handler connected to wrong node.")
+        for rcp in recipients:
+            handler.add_recipient(rcp)
+        if not self._root_handler_overriden and self._root in ("temp", "temporary"):
+            try:
+                self.remove_handler(self.root_handler)
+            except ValueError:
+                pass
+            self._root_handler_overriden = True
+        self.handlers.append(handler)
+
+        return handler
+
+    def remove_handler(self, handler):
+        """:param handler: NodeHandler or its id"""
+        if not isinstance(handler, NodeHandler):
+            id = handler
+            handler = next((x for x in self.handlers if x.id == id), None)
+            if handler is None:
+                raise ValueError("No handler matching id: {}".format(id))
+        self.handlers.remove(handler)
+
+    def has_client(self, node):
+        """:param node: Node or its id"""
+        node_id = node.id if isinstance(node, Node) else node
+
+        return node_id in self.clients_by_id
+
+    def serve(self):
+        """Start listening and handling any received."""
+        if self.is_running():
+            return
+        self.futures["serve"] = call_via_loop_afut(self._serve, loop=self.loop)
+
+    async def _serve(self):
+        try:
+            while True:
+                inp = await self._queue.get()
+                if isinstance(inp, NodeExit):
+                    break
+                self.handle(inp)
+        finally:
+            for handler in self.handlers:
+                handler.stop()
+
+    def handle(self, inp):
+        for handler in self.handlers:
+            handler.handle(inp)
+
+    async def recv(self):
+        """Receive directly, skipping the handlers"""
+        if self.is_running():
+            raise RuntimeError("Cannot receive directly while node is running.")
+
+        return await self._queue.get()
+
+    def recv_nowait(self):
+        return self._queue.get_nowait()
+
+    def relay(self, data, *channels):
+        """Relays directly, skipping the handlers"""
+        if not channels:
+            channels = [0]
+        pks = [RelayPackage(data, self, None, channel) for channel in channels]
+        self.station.broadcast_multiple(
+            [{"channel": pk.channel, "put": pk} for pk in pks]
+        )
+
+    def put(self, x, ensure_is_packed=True):
+        """
+        Put something into node's input queue
+        (if node is running it is immediately received by all its handlers).
+        :rtype: asyncio.Future
+        """
+        if ensure_is_packed and not isinstance(x, RelayPackage):
+            x = RelayPackage(x, None, None, None)
+
+        return call_via_loop_afut(self._queue.put, (x,), loop=self._queue._loop)
+
+    def put_nowait(self, x, ensure_is_packed=True):
+        """:rtype: Future"""
+        if ensure_is_packed and not isinstance(x, RelayPackage):
+            x = RelayPackage(x, None, None, None)
+
+        return put_via_loop(self._queue, x)
+
+    def empty(self):
+        return self._queue.empty()
+
+    def full(self):
+        return self._queue.full()
+
+    def is_running(self):
+        return self.futures["serve"] is not None and not self.futures["serve"].done()
+
+    def stop(self):
+        self.put(NodeExit())
+
+    def __repr__(self):
+        return "{}(id={},name={})".format(self.__class__.__name__, self.id, self.name)
+
+
+class NodeHandler:
+    def __init__(
+        self, node, target=None, recipients=[], *, loop=None, id=None, type=None
+    ):
+        """
+        :type node: Node
+        Handles the input received by its node.
+        :param type:
+            describes the `target`
+            ::None    - target is synchronous function
+                         - accepts the node input* as its first argument
+                         - returns output (which is then relayed by the handler)
+            ::"async" - a continuous "listener" coroutine function that
+                         - *may* accept `handler` (self) as its first argument
+                         - receives node input by awaiting on handler.recv(),
+                         - relays the output data independently (handler.relay(data))
+                         - exits on NodeExit()
+            ::"gen"   - a function that returns generator
+                         - function *may* accept `handler` (self) as its first argument
+                        where the generator
+                         - receives node input via `yield` keyword
+                         - yields the output (which is then relayed by the handler)
+                         - exhausts on NodeExit()
+            * node input: The data received by node, which is assumed to be wrapped with RelayPackage,
+                          or will be (in .handle) if not already done so
+        """
+        self.node = node
+        if loop is None:
+            loop = node.loop
+        self._queue = FonsQueue(loop=loop)
+        self.loop = self._queue._loop
+        self.channels = []
+
+        self.target = target
+        if type not in ("async", "gen", None):
+            raise ValueError(type)
+        self._type = type
+        # if asyncio.iscoroutinefunction(target):
+        #    self._type = 'async'
+
+        if id is None:
+            self.node._last_handler_id += 1
+            id = self.node._last_handler_id
+        else:
+            if any(x.id == id for x in self.node.handlers):
+                raise ValueError("A handler with id <{}> already exits".format(id))
+            if isinstance(id, int):
+                self.node._last_handler_id = max(id, self.node._last_handler_id)
+
+        self.id = id
+        self._started = False
+
+        for rcp in recipients:
+            self.add_recipient(rcp)
+
+    def _start(self):
+        if self._started:
+            return
+
+        args = (self,) if get_arg_count(self.target) else ()
+
+        if self._type is None:
+            pass
+        elif self._type == "gen":
+            self._gen = self.target(*args)
+            self._gen.send(None)
+        else:
+            call_via_loop(self.target, args, loop=self.loop)
+        self._started = True
+
+    def handle(self, x):
+        if not isinstance(x, RelayPackage):
+            x = RelayPackage(x, None, None, None, self)
+        else:
+            x = x.copy(current_handler=self)
+
+        if self._type is None:
+            data = self.target(x)
+            self.relay(data)
+        elif self._type == "gen":
+            # Generator
+            self._start()
+            data = self._gen.send(x)
+            self.relay(data)
+        else:
+            # Asynchronous
+            self._start()
+            self.put(x)
+
+    async def recv(self):
+        """This is only meant to be used in *asynchronous* target function of the handler"""
+        return await self._queue.get()
+
+    def recv_nowait(self):
+        return self._queue.get_nowait()
+
+    def relay(self, data):
+        """Relay the handler-processed data (wrapped with RelayPackage) to handler's nodes"""
+        if isinstance(data, RelayInfo):
+            return self._relay_by_info(data)
+
+        # Also include the source node (self) and the associated channel
+        pks = [
+            RelayPackage(data, self.node, self, channel) for channel in self.channels
+        ]
+        self.node.station.broadcast_multiple(
+            [{"channel": pk.channel, "put": pk} for pk in pks]
+        )
+
+    def _relay_by_info(self, info):
+        """:type info: RelayInfo"""
+        pks = []
+
+        for data, to_channels in info.items:
+            for channel in to_channels:
+                pk = RelayPackage(data, self.node, self, channel)
+                pks.append(pk)
+
+        self.node.station.broadcast_multiple(
+            [{"channel": pk.channel, "put": pk} for pk in pks]
+        )
+
+    def add_recipient(self, channel, create=False):
+        """:param channel: channel or Node"""
+        node = None
+        if isinstance(channel, Node):
+            node = channel
+            channel = node.id
+
+        if channel not in self.node.station.channels:
+            if not create:
+                raise ValueError("Channel <{}> hasn't been added yet".format(channel))
+            if node is not None:
+                self.node.connect(node)
+            else:
+                self.node.group(channel)
+
+        if channel in self.channels:
+            raise ValueError(
+                "Channel <{}> already added to handler {}".format(channel, self.id)
+            )
+
+        self.channels.append(channel)
+
+    def remove_recipient(self, channel):
+        if isinstance(channel, Node):
+            channel = channel.id
+        self.channels.remove(channel)
+
+    def put(self, x, ensure_is_packed=True):
+        """
+        Put something into handler's input queue
+        (only received if the handler has asynchronous target)
+        :rtype: asyncio.Future
+        """
+        if ensure_is_packed and not isinstance(x, RelayPackage):
+            x = RelayPackage(x, None, None, None)
+
+        return call_via_loop_afut(self._queue.put, (x,), loop=self._queue._loop)
+
+    def put_nowait(self, x, ensure_is_packed=True):
+        """:rtype: Future"""
+        if ensure_is_packed and not isinstance(x, RelayPackage):
+            x = RelayPackage(x, None, None, None)
+
+        return put_via_loop(self._queue, x)
+
+    def empty(self):
+        return self._queue.empty()
+
+    def full(self):
+        return self._queue.full()
+
+    def is_running(self):
+        return self._started
+
+    def stop(self):
+        if not self._started:
+            return
+        if self._type is None:
+            pass
+        elif self._type == "gen":
+            try:
+                self._gen.send(NodeExit())
+            except StopIteration:
+                pass
+        else:
+            self.put(NodeExit())
+        self._started = False
+
+
+def force_put(queue, item):
+    nr_removed = 0
+    while True:
+        try:
+            queue.put_nowait(item)
+        # multiprocessing.Queue also raises queue.Full
+        except (_queue.Full, asyncio.QueueFull):
+            try:
+                queue.get_nowait()
+            except (_queue.Full, asyncio.QueueEmpty):
+                pass
+            else:
+                nr_removed += 1
+        else:
+            break
+    return nr_removed
+
+
+def empty_queue(queue, return_items=False):
+    nr_removed = 0
+    received = []
+    try:
+        while True:
+            item = queue.get_nowait()
+            if return_items:
+                received.append(item)
+            else:
+                nr_removed += 1
+    except (_queue.Empty, asyncio.QueueEmpty):
+        pass
+    return received if return_items else nr_removed
+
+
+def put_via_loop(queue, x):
+    """Put something into queue"""
+    p = functools.partial(queue.put_nowait, x)
+    if asyncio.get_event_loop() is queue._loop:
+        f = Future()
+        f.set_result(p())
+        return f
+    else:
+        return call_via_loop(p, loop=queue._loop)
```

### Comparing `fons-0.3.1/fons/fsync.py` & `fons-0.4.0/fons/fsync.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,283 +1,283 @@
-import os
-import sys
-from random import randint
-import shutil
-import zipfile
-import time
-
-LETTERS = ''.join(chr(i) for i in range(128) if chr(i).isalpha())
-
-def random_nonce(length):
-    select = [LETTERS[randint(0, len(LETTERS)-1)] for _ in range(length)]
-    return ''.join(select)
-
-ONEDRIVE_POTENTIAL_ROOTS = [
-    'C:\\Users\\remil\\OneDrive',
-    'D:\\OneDrive',
-]
-ONEDRIVE_ROOT = next(x for x in ONEDRIVE_POTENTIAL_ROOTS if os.path.exists(x))
-#DONT_CHANGE = ['.preferences']
-PATHS = {
-    'PC_TEST': 'C:\\PProjects\\.test_updating',
-    'ONEDRIVE_TEST': os.path.join(ONEDRIVE_ROOT, '.test_updating'),
-    'ONEDRIVE_ZIP': os.path.join(ONEDRIVE_ROOT, '.test_updating.zip'),
-    'PRODUCTION': 'C:\\PProjects\\PyProjects_test',
-    'PC': 'C:\\PProjects\\PyProjects_dev',
-    'ONEDRIVE': os.path.join(ONEDRIVE_ROOT, 'PyProjects_test'),
-}
-PATHS['DEV'] = PATHS['PC']
-DONT_UPDATE_CONTENTS = \
-    [PATHS['PC']+'\\crypi\\data\\cyInf',
-     PATHS['PC']+'\\crypi\\data\\cmd\\__cache__',
-     PATHS['ONEDRIVE_TEST']+'\\test_prj\\not_allowed_folder']
-IGNORE_DIRS = ['__pycache__','.pytest_cache']
-IGNORE_FILES = ['geckodriver.log', 'prj.yaml']
-
-source = None
-dest = None
-
-def purge_walk(path):
-    """os.walk path and remove all files&folders"""
-    for root, dirs, files in os.walk(path, topdown=False):
-        for f in files:
-            os.remove(os.path.join(root, f))
-        for d in dirs:
-            os.rmdir(os.path.join(root, d))
-    os.rmdir(path)
-
-
-def force_delete(path):
-    if os.path.isdir(path):
-        os.system('cmd /c @RD /S /Q "{}"'.format(path))
-    else:
-        os.system('cmd /c del "{}" /F'.format(path))
-
-
-def unpack(zip_path):
-    zip_dir = os.path.dirname(zip_path)
-    print('Unpacking {} to {}'.format(zip_path, zip_dir))
-    with zipfile.ZipFile(zip_path, 'r') as z:
-        z.extractall(zip_dir)
-
-def unpack2(zip_path):
-    from fons.time import pydt
-    """Preserves the last modified ts"""
-    zip_dir = os.path.dirname(zip_path)
-    print('Unpacking {} to {}'.format(zip_path, zip_dir))
-    with zipfile.ZipFile(zip_path, 'r') as z:
-        for f in z.infolist():
-            rel_path, date_time = f.filename, f.date_time
-            rel_path = rel_path.replace('/','\\')
-            is_dir = rel_path.endswith('\\')
-            path = os.path.join(zip_dir, rel_path)
-            if is_dir:
-                if not os.path.isdir(path):
-                    os.mkdir(path)
-            else:
-                dir = os.path.dirname(path)
-                if not os.path.isdir(dir):
-                    os.mkdir(dir)
-                with open(path, 'wb') as outFile:
-                    outFile.write(z.open(f).read())
-                # It seems to be a second behind
-                date_time = time.mktime(date_time + (0, 0, -1)) + 1
-                #print(rel_path)
-                #print(date_time)
-                #print(pydt(date_time).isoformat())
-                os.utime(path, (date_time, date_time))
-
-
-def is_allowed(path, is_dir=False):
-    split = path.split('\\')[:(-1 if not is_dir else None)]
-    return not any('\\'.join(split[:i+1]) in DONT_UPDATE_CONTENTS
-                   for i in range(len(split)))
-
-
-def already_added(path, dirs, is_dir=True):
-    split = path.split('\\')[:(-1 if not is_dir else None)]
-    return any('\\'.join(split[:i+1]) in dirs
-               for i in range(len(split)))
-
-
-def get_info(source_path, dest_path):
-    #rn_path = os.path.join(dest_path, random_nonce(16))
-    if not os.path.isdir(dest_path):
-        os.mkdir(dest_path)
-    #else:
-    #    os.path.rename(dest_path, rn_path)
-    len_source_path = len(source_path)
-    len_dest_path = len(dest_path)
-    info = []
-    delete_dirs = []
-    ignore_dirs = []
-
-    def is_file_changed(path, path2):
-        if not os.path.isfile(path2):
-            return True
-
-        if os.path.getsize(path) != os.path.getsize(path2):
-            return True
-        
-        file_last_modified = os.path.getmtime(path)
-        file2_last_modified = os.path.getmtime(path2)
-        
-        if file_last_modified != file2_last_modified:
-            with open(path, 'rb') as f:
-                bytes = f.read()
-            with open(path2, 'rb') as f:
-                bytes2 = f.read()
-            #print(path, path2, 'contents match:', bytes==bytes2)
-            return bytes != bytes2
-
-        return False
-    
-    # CREATE
-    for root, dirs, files in os.walk(source_path, topdown=True):
-        rel_root = root[len_source_path+1:]
-        source_root = root
-        dest_root = os.path.join(dest_path, rel_root)
-        parent_dir_names = rel_root.split('\\')
-        if any(name in IGNORE_DIRS for name in parent_dir_names):
-            if not already_added(root, ignore_dirs, is_dir=True):
-                ignore_dirs.append(root)
-            continue
-        for dir in dirs:
-            source_dir_path = os.path.join(source_root, dir)
-            dest_dir_path = os.path.join(dest_root, dir)
-            if dir in IGNORE_DIRS:
-                info.append(('IGNORE','dir',source_dir_path,dest_dir_path))
-                continue
-            if not os.path.isdir(dest_dir_path):
-                info.append(('MAKE','dir',source_dir_path,dest_dir_path))
-        for f in files:
-            source_file_path = os.path.join(source_root, f)
-            dest_file_path = os.path.join(dest_root, f)
-            if f in IGNORE_FILES:
-                info.append(('IGNORE','file',source_dir_path,dest_dir_path))
-                continue
-            if is_allowed(dest_file_path, is_dir=False) and is_file_changed(source_file_path, dest_file_path):
-                info.append(('MAKE','file',source_file_path,dest_file_path))
-            else:
-                info.append(('IGNORE','file',source_file_path,dest_file_path))
-
-    # REMOVE
-    for root, dirs, files in os.walk(dest_path, topdown=True):
-        rel_root = root[len_dest_path+1:]
-        source_root = os.path.join(source_path, rel_root)
-        dest_root = root
-        parent_dir_names = rel_root.split('\\')
-        if any(name in IGNORE_DIRS for name in parent_dir_names):
-            if not already_added(root, ignore_dirs, is_dir=True):
-                ignore_dirs.append(root)
-            continue
-        for dir in dirs:
-            dest_dir_path = os.path.join(dest_root, dir)
-            source_dir_path = os.path.join(source_root, dir)
-            if dir in IGNORE_DIRS:
-                info.append(('IGNORE','dir',dest_dir_path,source_dir_path))
-                continue
-            if not os.path.isdir(source_dir_path) \
-                   and not already_added(dest_dir_path, delete_dirs, is_dir=True):
-                info.append(('DELETE','dir',source_dir_path,dest_dir_path))
-                delete_dirs.append(dest_dir_path)
-        for f in files:
-            dest_file_path = os.path.join(dest_root, f)
-            source_file_path = os.path.join(source_root, f)
-            if f in IGNORE_FILES:
-                info.append(('IGNORE','file',dest_file_path,source_file_path))
-                continue
-            if not os.path.isfile(source_file_path) \
-                    and not already_added(dest_file_path, delete_dirs, is_dir=False):
-                if is_allowed(dest_file_path, is_dir=False):
-                    info.append(('DELETE','file',source_file_path,dest_file_path))
-                else:
-                    info.append(('IGNORE','file',dest_file_path,source_file_path))
-    
-    return info
-
-
-def operate(item, show_ignore=True):
-    op, type, source, dest = item
-    print_strs = {
-        'IGNORE': 'Ignoring',
-        'MAKE': 'Creating',
-        'DELETE': 'Removing'
-    }
-    path = dest if op!='IGNORE' else source
-    print_str = op #print_strs[op]
-    if op == 'MAKE' and os.path.isfile(path):
-        print_str = 'UPDATE' #'Updating'
-    add_str = '(f)' if type=='file' else '(d)'
-    if op!='IGNORE' or show_ignore:
-        print('{}{} {}'.format(print_str, add_str, path))
-    if op == 'MAKE':
-        if type == 'dir':
-            os.mkdir(path)
-        else:
-            shutil.copy2(source, path)
-    elif op == 'DELETE':
-        if type == 'dir':
-            try:
-                shutil.rmtree(path)
-            except PermissionError as e:
-                print('rmtree on {} failed ({}). Attempting force delete.'.format(path, repr(e)))
-                force_delete(path)
-        else:
-            try:
-                os.remove(path)
-            except PermissionError as e:
-                print('os.remove on {} failed ({}). Attempting force delete.'.format(path, repr(e)))
-                force_delete(path)
-
-
-def update(source, dest, show_ignore=False):
-    info = get_info(source, dest)
-    for item in info:
-        operate(item, show_ignore)
-
-
-def main(argv=sys.argv):
-    source = dest = None
-    source_name = None
-    _from = _to = None
-    txt = '"from:" / "to:" + "onedrive" / "pc" / "production"|| "test"\n'
-    
-    while _from is None or _to is None or _from == _to:
-        inp = input(txt)
-        split = [x.strip() for x in inp.split(':')]
-        if inp == 'test':
-            _from = 'pc_test'
-            _to = 'onedrive_test'
-        elif len(split)!=2 or split[0] not in ('from','to')\
-                 or split[1] not in ('onedrive','pc','production','dev'):
-            print('Incorrect input!')
-        elif split[0] == 'from':
-            _from = split[1]
-        else:
-            _to = split[1]
-        txt = ''
-    
-    source = PATHS[_from.upper()]
-    dest = PATHS[_to.upper()]
-    show_ignore = (_from == 'pc_test')
-    if 'show_ignore' in argv:
-        show_ignore = True
-    
-    if _to == 'onedrive_test':
-        if os.path.isdir(PATHS['ONEDRIVE_TEST']):
-            print('Removing old Onedrive test dir.')
-            shutil.rmtree(PATHS['ONEDRIVE_TEST'])
-        unpack2(PATHS['ONEDRIVE_ZIP'])
-    
-    projects = [x for x in os.listdir(source)
-                if os.path.exists(os.path.join(source, x, '.project'))]
-    
-    for name in projects:
-        print("----------------------------------------")
-        print("Project: '{}'".format(name))
-        update(os.path.join(source, name), os.path.join(dest, name), show_ignore)
-
-
-if __name__ == '__main__':
-    main()
-
+import os
+import sys
+from random import randint
+import shutil
+import zipfile
+import time
+
+LETTERS = ''.join(chr(i) for i in range(128) if chr(i).isalpha())
+
+def random_nonce(length):
+    select = [LETTERS[randint(0, len(LETTERS)-1)] for _ in range(length)]
+    return ''.join(select)
+
+ONEDRIVE_POTENTIAL_ROOTS = [
+    'C:\\Users\\remil\\OneDrive',
+    'D:\\OneDrive',
+]
+ONEDRIVE_ROOT = next(x for x in ONEDRIVE_POTENTIAL_ROOTS if os.path.exists(x))
+#DONT_CHANGE = ['.preferences']
+PATHS = {
+    'PC_TEST': 'C:\\PProjects\\.test_updating',
+    'ONEDRIVE_TEST': os.path.join(ONEDRIVE_ROOT, '.test_updating'),
+    'ONEDRIVE_ZIP': os.path.join(ONEDRIVE_ROOT, '.test_updating.zip'),
+    'PRODUCTION': 'C:\\PProjects\\PyProjects_test',
+    'PC': 'C:\\PProjects\\PyProjects_dev',
+    'ONEDRIVE': os.path.join(ONEDRIVE_ROOT, 'PyProjects_test'),
+}
+PATHS['DEV'] = PATHS['PC']
+DONT_UPDATE_CONTENTS = \
+    [PATHS['PC']+'\\crypi\\data\\cyInf',
+     PATHS['PC']+'\\crypi\\data\\cmd\\__cache__',
+     PATHS['ONEDRIVE_TEST']+'\\test_prj\\not_allowed_folder']
+IGNORE_DIRS = ['__pycache__','.pytest_cache']
+IGNORE_FILES = ['geckodriver.log', 'prj.yaml']
+
+source = None
+dest = None
+
+def purge_walk(path):
+    """os.walk path and remove all files&folders"""
+    for root, dirs, files in os.walk(path, topdown=False):
+        for f in files:
+            os.remove(os.path.join(root, f))
+        for d in dirs:
+            os.rmdir(os.path.join(root, d))
+    os.rmdir(path)
+
+
+def force_delete(path):
+    if os.path.isdir(path):
+        os.system('cmd /c @RD /S /Q "{}"'.format(path))
+    else:
+        os.system('cmd /c del "{}" /F'.format(path))
+
+
+def unpack(zip_path):
+    zip_dir = os.path.dirname(zip_path)
+    print('Unpacking {} to {}'.format(zip_path, zip_dir))
+    with zipfile.ZipFile(zip_path, 'r') as z:
+        z.extractall(zip_dir)
+
+def unpack2(zip_path):
+    from fons.time import pydt
+    """Preserves the last modified ts"""
+    zip_dir = os.path.dirname(zip_path)
+    print('Unpacking {} to {}'.format(zip_path, zip_dir))
+    with zipfile.ZipFile(zip_path, 'r') as z:
+        for f in z.infolist():
+            rel_path, date_time = f.filename, f.date_time
+            rel_path = rel_path.replace('/','\\')
+            is_dir = rel_path.endswith('\\')
+            path = os.path.join(zip_dir, rel_path)
+            if is_dir:
+                if not os.path.isdir(path):
+                    os.mkdir(path)
+            else:
+                dir = os.path.dirname(path)
+                if not os.path.isdir(dir):
+                    os.mkdir(dir)
+                with open(path, 'wb') as outFile:
+                    outFile.write(z.open(f).read())
+                # It seems to be a second behind
+                date_time = time.mktime(date_time + (0, 0, -1)) + 1
+                #print(rel_path)
+                #print(date_time)
+                #print(pydt(date_time).isoformat())
+                os.utime(path, (date_time, date_time))
+
+
+def is_allowed(path, is_dir=False):
+    split = path.split('\\')[:(-1 if not is_dir else None)]
+    return not any('\\'.join(split[:i+1]) in DONT_UPDATE_CONTENTS
+                   for i in range(len(split)))
+
+
+def already_added(path, dirs, is_dir=True):
+    split = path.split('\\')[:(-1 if not is_dir else None)]
+    return any('\\'.join(split[:i+1]) in dirs
+               for i in range(len(split)))
+
+
+def get_info(source_path, dest_path):
+    #rn_path = os.path.join(dest_path, random_nonce(16))
+    if not os.path.isdir(dest_path):
+        os.mkdir(dest_path)
+    #else:
+    #    os.path.rename(dest_path, rn_path)
+    len_source_path = len(source_path)
+    len_dest_path = len(dest_path)
+    info = []
+    delete_dirs = []
+    ignore_dirs = []
+
+    def is_file_changed(path, path2):
+        if not os.path.isfile(path2):
+            return True
+
+        if os.path.getsize(path) != os.path.getsize(path2):
+            return True
+        
+        file_last_modified = os.path.getmtime(path)
+        file2_last_modified = os.path.getmtime(path2)
+        
+        if file_last_modified != file2_last_modified:
+            with open(path, 'rb') as f:
+                bytes = f.read()
+            with open(path2, 'rb') as f:
+                bytes2 = f.read()
+            #print(path, path2, 'contents match:', bytes==bytes2)
+            return bytes != bytes2
+
+        return False
+    
+    # CREATE
+    for root, dirs, files in os.walk(source_path, topdown=True):
+        rel_root = root[len_source_path+1:]
+        source_root = root
+        dest_root = os.path.join(dest_path, rel_root)
+        parent_dir_names = rel_root.split('\\')
+        if any(name in IGNORE_DIRS for name in parent_dir_names):
+            if not already_added(root, ignore_dirs, is_dir=True):
+                ignore_dirs.append(root)
+            continue
+        for dir in dirs:
+            source_dir_path = os.path.join(source_root, dir)
+            dest_dir_path = os.path.join(dest_root, dir)
+            if dir in IGNORE_DIRS:
+                info.append(('IGNORE','dir',source_dir_path,dest_dir_path))
+                continue
+            if not os.path.isdir(dest_dir_path):
+                info.append(('MAKE','dir',source_dir_path,dest_dir_path))
+        for f in files:
+            source_file_path = os.path.join(source_root, f)
+            dest_file_path = os.path.join(dest_root, f)
+            if f in IGNORE_FILES:
+                info.append(('IGNORE','file',source_dir_path,dest_dir_path))
+                continue
+            if is_allowed(dest_file_path, is_dir=False) and is_file_changed(source_file_path, dest_file_path):
+                info.append(('MAKE','file',source_file_path,dest_file_path))
+            else:
+                info.append(('IGNORE','file',source_file_path,dest_file_path))
+
+    # REMOVE
+    for root, dirs, files in os.walk(dest_path, topdown=True):
+        rel_root = root[len_dest_path+1:]
+        source_root = os.path.join(source_path, rel_root)
+        dest_root = root
+        parent_dir_names = rel_root.split('\\')
+        if any(name in IGNORE_DIRS for name in parent_dir_names):
+            if not already_added(root, ignore_dirs, is_dir=True):
+                ignore_dirs.append(root)
+            continue
+        for dir in dirs:
+            dest_dir_path = os.path.join(dest_root, dir)
+            source_dir_path = os.path.join(source_root, dir)
+            if dir in IGNORE_DIRS:
+                info.append(('IGNORE','dir',dest_dir_path,source_dir_path))
+                continue
+            if not os.path.isdir(source_dir_path) \
+                   and not already_added(dest_dir_path, delete_dirs, is_dir=True):
+                info.append(('DELETE','dir',source_dir_path,dest_dir_path))
+                delete_dirs.append(dest_dir_path)
+        for f in files:
+            dest_file_path = os.path.join(dest_root, f)
+            source_file_path = os.path.join(source_root, f)
+            if f in IGNORE_FILES:
+                info.append(('IGNORE','file',dest_file_path,source_file_path))
+                continue
+            if not os.path.isfile(source_file_path) \
+                    and not already_added(dest_file_path, delete_dirs, is_dir=False):
+                if is_allowed(dest_file_path, is_dir=False):
+                    info.append(('DELETE','file',source_file_path,dest_file_path))
+                else:
+                    info.append(('IGNORE','file',dest_file_path,source_file_path))
+    
+    return info
+
+
+def operate(item, show_ignore=True):
+    op, type, source, dest = item
+    print_strs = {
+        'IGNORE': 'Ignoring',
+        'MAKE': 'Creating',
+        'DELETE': 'Removing'
+    }
+    path = dest if op!='IGNORE' else source
+    print_str = op #print_strs[op]
+    if op == 'MAKE' and os.path.isfile(path):
+        print_str = 'UPDATE' #'Updating'
+    add_str = '(f)' if type=='file' else '(d)'
+    if op!='IGNORE' or show_ignore:
+        print('{}{} {}'.format(print_str, add_str, path))
+    if op == 'MAKE':
+        if type == 'dir':
+            os.mkdir(path)
+        else:
+            shutil.copy2(source, path)
+    elif op == 'DELETE':
+        if type == 'dir':
+            try:
+                shutil.rmtree(path)
+            except PermissionError as e:
+                print('rmtree on {} failed ({}). Attempting force delete.'.format(path, repr(e)))
+                force_delete(path)
+        else:
+            try:
+                os.remove(path)
+            except PermissionError as e:
+                print('os.remove on {} failed ({}). Attempting force delete.'.format(path, repr(e)))
+                force_delete(path)
+
+
+def update(source, dest, show_ignore=False):
+    info = get_info(source, dest)
+    for item in info:
+        operate(item, show_ignore)
+
+
+def main(argv=sys.argv):
+    source = dest = None
+    source_name = None
+    _from = _to = None
+    txt = '"from:" / "to:" + "onedrive" / "pc" / "production"|| "test"\n'
+    
+    while _from is None or _to is None or _from == _to:
+        inp = input(txt)
+        split = [x.strip() for x in inp.split(':')]
+        if inp == 'test':
+            _from = 'pc_test'
+            _to = 'onedrive_test'
+        elif len(split)!=2 or split[0] not in ('from','to')\
+                 or split[1] not in ('onedrive','pc','production','dev'):
+            print('Incorrect input!')
+        elif split[0] == 'from':
+            _from = split[1]
+        else:
+            _to = split[1]
+        txt = ''
+    
+    source = PATHS[_from.upper()]
+    dest = PATHS[_to.upper()]
+    show_ignore = (_from == 'pc_test')
+    if 'show_ignore' in argv:
+        show_ignore = True
+    
+    if _to == 'onedrive_test':
+        if os.path.isdir(PATHS['ONEDRIVE_TEST']):
+            print('Removing old Onedrive test dir.')
+            shutil.rmtree(PATHS['ONEDRIVE_TEST'])
+        unpack2(PATHS['ONEDRIVE_ZIP'])
+    
+    projects = [x for x in os.listdir(source)
+                if os.path.exists(os.path.join(source, x, '.project'))]
+    
+    for name in projects:
+        print("----------------------------------------")
+        print("Project: '{}'".format(name))
+        update(os.path.join(source, name), os.path.join(dest, name), show_ignore)
+
+
+if __name__ == '__main__':
+    main()
+
```

### Comparing `fons-0.3.1/fons/func.py` & `fons-0.4.0/fons/func.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,748 +1,764 @@
-from functools import wraps
-from inspect import (currentframe, getargvalues, getfullargspec)
-
-import traceback
-import platform
-import copy
-import time
-import datetime
-dt = datetime.datetime
-td = datetime.timedelta
-
-from collections import deque
-from queue import Queue
-import asyncio
-import math
-import warnings
-import logging
-import inspect
-
-from fons.errors import WaitException, TerminatedException
-
-
-_LIMITCALLS_STORE_GLOBALLY = False
-_LIMITCALLS_PARAMS = {}
-_LIMITCALLS_HISTORY = {}
-
-_LIMITCALLS_LOGGING_LEVEL = logging.WARNING 
-_LIMITCALLS_SLEEP_LOGGING_LEVEL = logging.DEBUG
-_LIMITCALLS_WARN_WHEN_SLEEP = False
-_LIMITCALLS_RETAIN_ORDER = False
-
-_PLATFORM = platform.system()
-
-
-#If method called as static, initializes necessary attributes (passed as kwargs)
-#   to class (instead of instance), without changing the original class attrbs
-#If called as class but without kwargs, assumes class already has those attrbs
-
-class hybridmethod(object):
-    def __init__(self, func):
-        self.func = func
-
-    def __get__(self, obj, cls):
-        context = obj if obj is not None else cls
-
-        #create new class to not overwrite its attrbs
-        if context is cls:
-            class NewoO(context):
-                pass
-            context = NewoO
-            K_name = cls.__name__
-            K_name_part = '__' + K_name + '_'
-            
-            for attr_name in vars(cls):
-                if K_name_part in attr_name and attr_name[-2:] != '__':
-                    attr_short = attr_name.replace(K_name_part, '')
-                    attr_value = getattr(cls, attr_name)
-                    setattr(context, '__' + attr_short, copy.deepcopy(attr_value))
-
-        @wraps(self.func)
-        def hybrid(*args, **kw):
-
-            #inits only if context is class (not self (instance))
-            #offers to not init some kw for class too:
-            init_kw = kw
-            if '_static_vars' in kw:
-                init_kw = {k:v for k,v in kw.items() if k not in kw['_static_vars']}
-                kw = {k:v for k,v in kw.items() if k in kw['_static_vars']}
-                del init_kw['_static_vars']
-            else:
-                init_kw = kw.copy()
-                #kw = {}
-                
-            for k,v in init_kw.items():
-                try:
-                    #checks if is class (don't want to overwrite self attrbs):
-                    if isinstance(context, type):
-                        setattr(context,k,v)    
-                except Exception:
-                    traceback.print_exc()
-                        
-            return self.func(context, *args, **kw)
-
-            #Exceptions (when one *must* use _static_vars):
-            #instance method checks if it has attr which's name also happens to be in its kwargs
-            # (therefore answer would always be "yes" if we init it to class 'New')
-            #if a kwarg happens to be an attr of *class* "context" aswell
-            # (although I can differ an instance from class/static, I can't
-            #  differ class from static (since static is called *from* the class)
-            #  therefore if its a class its attr is overwritten with the kwarg)
-        
-        # optional, mimic methods some more
-        hybrid.__func__ = hybrid.im_func = self.func
-        hybrid.__self__ = hybrid.im_self = context
-
-        return hybrid
-
-def obj_to_class(obj):
-    klass = obj
-    if not isinstance(obj, type):
-        klass = eval(obj.__class__.__name__)
-        
-    return klass
-    
-def mro_without_wrapper(obj):
-    klass = obj_to_class(obj)
-  
-    loc = next((i for i,k in enumerate(klass.mro())
-                    if 'hybridmethod' not in k or 'NewoO' not in k), 0)
-    
-    mro_list = klass.mro()[loc:]
-    
-    return mro_list
-
-
-#like super(klass), except for 'NewoO'-s is returned its grandparent
-def superb(cls):
-    mro_list = mro_without_wrapper(cls)
-    superklass = eval(mro_list[1].__name__)
-    return superklass
-
-    
-def superclasses(obj):
-    klass = obj_to_class(obj)
-
-    if klass is not obj:
-        #method was called from instance
-        loc = 1
-    else:
-        #method was called from class
-        loc = next((i for i,k in enumerate(klass.mro())
-                    if 'hybridmethod' not in k or 'NewoO' not in k), None)
-
-        if loc is None: return
-    
-    
-    superklasses = [eval(k.__name__) for k in klass.mro()[loc:-1] ]
-    #all classes above the class of obj, except the last one ('object')
-    #will they evaluate if in different modules? probably yes
-    
-    return superklasses
-
-def find_all_double_underscore_vars(obj,
-                    var_name, superklasses=None):
-    if not isinstance(superklasses, (tuple,list)):
-        superklasses = superclasses(obj)
-
-    sk = superklasses[:]    
-    sk.insert(0, obj_to_class(obj))
-
-    a_list = []
-    
-    for K in sk:
-        try:
-            a_list.append(eval('K._{}__{}'.format(K.__name__, var_name)))
-        except Exception:
-            pass
-
-    return a_list
-
-
-def get_arg_count(f):
-    argspec = inspect.getfullargspec(f)
-    if argspec.varargs:
-        return math.inf
-    #from_i = 0 if not argspec.args or argspec.args[0] != 'self' else 1
-    #inspect.ismethod is accurate whether or not "self" is first arg,
-    # or when it only has *args; works for classmethods (initated or not) too
-    from_i = 0 if not inspect.ismethod(f) else 1
-    return len(argspec.args[from_i:])
-
-#----------------------------------------------------------------------------
-
-
-def _has_self(f):
-    fas = getfullargspec(f)
-    args = fas[0]
-    
-    if len(args) and args[0] == 'self':
-        return True
-    
-    return False
-
-
-def _resolve_instance(func,args,bound,bound2):
-    if hasattr(bound,'__call__'):
-        instance = bound(args[0])
-        
-    elif bound: 
-        instance = args[0]
-    
-    elif bound2 and not isinstance(args[0],type):
-        #user has left bound=None, and first param is "self"
-        #only accept if args[0] is not cls (accidental classmethod)
-        #(we don't want to *accidentally* use cls as the identifier,
-        # because the cls would differ for subclasses while the function is same)
-        instance = args[0]
-
-    else: instance = None
-
-
-
-    if not hasattr(instance,'__hash__'):
-        first_param = getfullargspec(func)['args'][0]
-        
-        raise TypeError(('Function "{}" is bound, '\
-                        'but its first param "{}" of type {} is not hashable').format(
-                            func.__name__, first_param, type(instance)))
-    
-    
-    return instance
-
-
-
-def _get_msg(func,instance,text):
-    
-    if instance is not None:
-        txt0 = 'Limitcall on method {} of instance {}: '.format(func.__name__, instance)
-    else:txt0 = 'Limitcall on function {}: '.format(func.__name__)
-    
-    msg = txt0 + text.strip()
-    
-    return msg
-
-
-"""class _TimeShort:
-    def __init__(self, deq, interval):
-        self.deq = deq
-        self.interval = interval
-        
-    def __call__(self):
-        nearest_next = self.deq[0] + self.interval
-        self.time_short = time_short = (nearest_next - dt.utcnow())/td(seconds=1)
-        
-        return time_short
-    
-    __slots__ = ['deq','interval','time_short']"""
-    
-
-def _handle_action(action, msg, logging_level, 
-                   exception=None, args=[], kwargs={},
-                   sleep_time=0):
-    
-
-    if action == 'error':
-        raise exception(*args,**kwargs)
-    elif action == 'warn':
-        warnings.warn(msg)
-    elif action == 'log':
-        logging.log(logging_level, msg)
-        
-    elif action ==  'sleep':
-        msg += ' --- sleeping {}s'.format(round(sleep_time, 3))
-        logging.log(logging_level, msg)
-        
-        if _LIMITCALLS_WARN_WHEN_SLEEP:
-            warnings.warn(msg)
-            
-        time.sleep(sleep_time)
-        
-
-def _handle_request(func, PARAMS, QUEUES, HISTORY, instance=None):
-    limit, interval, action, logging_lvl = PARAMS
-    
-    if instance is None: 
-        deq = HISTORY['func']
-        queue = QUEUES['func']
-        
-    elif instance not in HISTORY['instances']:
-        HISTORY['instances'][instance] =  deq = deque(maxlen=limit)
-        QUEUES['instances'][instance] = queue = Queue(1)
-        
-    else: 
-        deq = HISTORY['instances'][instance]
-        queue = QUEUES['instances'][instance]
-        
-    lvl = logging_lvl if queue.full() else 0
-    logging.log(lvl,_get_msg(func, instance, 'waiting on lock'))
-        
-    try:
-        queue.put(None)
-        logging.log(lvl,_get_msg(func, instance, 'lock acquired'))
-        
-        if len(deq) < limit:
-            deq.append(time.time())
-            return
-        elif interval is None:
-            msg = _get_msg(func, instance, 'has reached its total max calls {}'.format(limit))
-            _handle_action(action, msg, logging_lvl, TerminatedException, [msg])
-            return
-        
-        #If action is 'sleep', in every cycle the lock will be released before the sleep,
-        # (so that the other calls don't have to wait), then acquired again
-        # repeated until time_short > 0 
-
-        while True:
-            nearest_next = deq[0] + interval
-            wait_time = nearest_next - time.time()
-            if wait_time <= 0: break 
-            
-            msg = _get_msg(func, instance, 'calls blocked for {}s.'.format(round(wait_time,3)))
-            _handle_action(action, msg, logging_lvl, WaitException, [wait_time],
-                           {'msg':msg}, wait_time)
-            
-            if action != 'sleep': break
-                    
-                    
-        deq.append(time.time())
-            
-            
-    finally:
-        queue.get()
-
-    
-
-#Note: methods of instances of same class have different ids,
-#      but limitcalls makes no difference, since it first wraps
-#      during the time of class initiation
-#      set 'bound' to True (or leave None) for each instance calls 
-#        to method be counted separately
-    
-def limitcalls(limit, interval=None, action='error', bound=None, **kw):
-    
-    """Decorator for counting the calls to the decorated function.
-        Args:
-         limit (int): 
-           number of maximum calls [absolute or periodic] to the function
-           if exceeded, action is taken
-           
-         interval (int,float,timedelta,::None):
-           ::None - limit is absolute (action taken if total > limit)
-           ::<int,float> -> converted to timedelta(seconds(int,float))
-           ::<timedelta> - calls are timestamped, action taken if rate is exceeded in interval (now-timedelta, now)
-           
-         action (str/None):
-           what happens when call rate is exceeded
-           ::error - raises TerminatedException if interval=None and limit exceeded,
-                     raises WaitException if interval!= None and limit exceeded
-           ::sleep - sleeps till nr_calls won't exceed limit in interval, then proceeds
-           ::warn  - warns user with the error message, but proceeds
-           ::log   - logs the error message, but proceeds
-           ::None  - does nothing if call rate exceeded, proceeds with call
-           
-         bound (bool):
-           if method, then whether the calls to are counted separately by each instance
-           IMPORTANT: does not differentiate inherited methods from their source (i.e A.a == B(A).a [if a was inherited])
-           ::True - first arg is assumed to be 'self', calls to func counted separately by each instance
-           ::False - calls to func counted universally
-           ::<callable> - instance is resolved by <callable>(args[0])
-           ::None - auto-detects if the function is defined in class and has 'self' as first param,
-                    if so then bound = True, otherwise False
-                    Fails if: -method *without* "self" as first param (but intended to be bound)
-                              -method was defined outside class (and intended to be bound)
-                              -@staticmethod with "self" as first param
-                              In those cases if you're lazy typing bound=True/False, 
-                               use @limitcalls_f / @limitcalls_m instead
-                    
-        **kw:
-         logging_level (int):
-           logging level for error messages if action == 'log' / 'sleep'
-           DEFAULT: DEBUG for 'sleep' action, WARNING for 'log'
-         f (function):
-           if used not as decorator (@limitcalls), but for converting an existing function,
-           can do new_f = limitcalls(...,f=f) [instead of new_f = limitcalls(...)(f)]"""
-         
-           
-    
-    if isinstance(interval, td):
-        interval = interval.total_seconds()
-        
-    elif interval is None and action=='sleep':
-        raise ValueError('Action cannot be "sleep" if interval not specified.')
-    
-    elif not isinstance(interval, (int, float, type(None))):
-        raise TypeError(type(interval))
-    
-    
-    
-    if not isinstance(limit, int):
-        raise TypeError(type(limit))
-    
-
-
-    if action == 'sleep':
-        logging_lvl = _LIMITCALLS_SLEEP_LOGGING_LEVEL
-    else:logging_lvl = _LIMITCALLS_LOGGING_LEVEL
-    
-    if kw.get('logging_level') is not None:
-        logging_lvl = kw['logging_level']
-        
-        
-    if hasattr(bound,'__call__'): pass   
-    elif not isinstance(bound,(bool,type(None))):
-        raise TypeError(type(bound))
-
-    
-    
-    if not isinstance(action, (str, type(None))):
-        raise TypeError(type(action))
-    
-    elif action not in ('error','sleep','warn','log',None):
-        raise ValueError(action)
-    
-    
-    f = kw.get('f')
-    
-
-       
-    
-    def actual_decorator(func):
-        PARAMS = (limit, interval, action, logging_lvl)
-        QUEUES = {'func': Queue(1), 'instances': {}}
-        HISTORY = {'func': deque(maxlen=limit), 'instances': {}}
-
-        bound2 = bound
-        #note to self:
-        # cannot do: bound = new_value
-        # (for some bound cannot be overwritten, otherwise it is lost from locals)
-        
-        
-        #check if has self (eliminates ordinary funcs and @classmethod/@staticmethod, 
-        #                   assuming user has *not* defined self as first param)
-        #if has "self" as first param, checks if the func is defined in the body of class
-        #  (further eliminates functions defined outside class' [0th level] body )
-        #  --note that __qualname__ may be given in other situations too 
-        #  --but tested that it *wasn't* present if the body was module or function
-        
-        #Note: the functionality still remains even if @classmethod has "self" as first param
-        #  because first input param cls remains the same; however that is only implemented if
-        #  bound = True; if left to None the inherited classmethods will be treated as identical
-        
-        
-        if bound2 is not None: pass
-        elif not _has_self(func): bound2 = False
-        else:
-            #__qualname__ only given if frame is located in the body of a class
-            frame = currentframe().f_back
-            if f: frame = frame.f_back
-
-            #getargvalues returns namedtuple
-            fr_locals = getargvalues(frame).locals
-            #print(fr_locals.get('__qualname__'), '__qualname__' in fr_locals, func.__name__)
-
-            
-            try: bound2 = fr_locals['__qualname__'] is not None
-            except KeyError: bound2 = False
-                
-        
-
-        @wraps(func)
-        def wrapper(*args,**kw):
-            instance = _resolve_instance(func, args, bound, bound2)
-            _handle_request(func, PARAMS, QUEUES, HISTORY, instance)
-
-            return func(*args, **kw)
-
-
-
-        if _LIMITCALLS_STORE_GLOBALLY:
-            _LIMITCALLS_PARAMS[wrapper] = PARAMS
-            _LIMITCALLS_HISTORY[wrapper] =  HISTORY
-            
-    
-        return wrapper
-
-
-
-    
-    if f: return actual_decorator(f)
-    
-    
-    return actual_decorator
-
-
-
-def limitcalls_f(limit, interval=None, action='error', **kw):
-    """For ordinary functions and classmethods/staticmethods, 
-        or if calls to method are not intended do be counted separately for each instance"""
-    return limitcalls(limit, interval, action, bound=False, **kw)
-
-
-def limitcalls_m(limit, interval=None, action='error', **kw):
-    """For methods"""
-    return limitcalls(limit, interval, action, bound=True, **kw)
-
-
-
-#-------------------------------------------------------------------------------------------
-
-async def _async_handle_action(action, msg, logging_level, 
-                   exception=None, args=[], kwargs={},
-                   sleep_time=0, lock=None, retain_order=False):
-    
-
-    if action == 'error':
-        raise exception(*args,**kwargs)
-    elif action == 'warn':
-        warnings.warn(msg)
-    elif action == 'log':
-        logging.log(logging_level, msg)
-        
-    elif action ==  'sleep':
-        msg += ' --- sleeping {}s'.format(round(sleep_time, 2))
-        logging.log(logging_level, msg)
-        
-        if _LIMITCALLS_WARN_WHEN_SLEEP:
-            warnings.warn(msg)
-        
-        if lock is not None and lock.locked() and not retain_order:
-            lock.release()
-        
-        await asyncio.sleep(sleep_time)
-        
-        if lock is not None and not retain_order:
-            await lock.acquire()
-        
-
-async def _async_handle_request(func, PARAMS, LOCKS, HISTORY, instance=None):
-    limit, interval, action, logging_lvl, retain_order = PARAMS
-    
-    if instance is None: 
-        deq = HISTORY['func']
-        lock = LOCKS['func']
-        
-    elif instance not in HISTORY['instances']:
-        HISTORY['instances'][instance] =  deq = deque(maxlen=limit)
-        LOCKS['instances'][instance] = lock = asyncio.Lock()
-        
-    else: 
-        deq = HISTORY['instances'][instance]
-        lock = LOCKS['instances'][instance]
-    
-    lvl = logging_lvl if lock.locked() and retain_order else 0
-    logging.log(lvl, _get_msg(func, instance, 'waiting on lock'))
-    
-    try:
-        await lock.acquire()
-        logging.log(lvl, _get_msg(func, instance, 'lock acquired'))
-        
-        if len(deq) < limit:
-            deq.append(time.time())
-            return
-        elif interval is None:
-            msg = _get_msg(func, instance, 'has reached its total max calls {}'.format(limit))
-            await _async_handle_action(action, msg, logging_lvl, TerminatedException, 
-                                       [msg], retain_order=retain_order)
-            return
-        
-        #If action is 'sleep', in every cycle the lock will be released before the sleep,
-        # (so that the other calls don't have to wait), then acquired again
-        # repeated until time_short > 0 
-        lowest = 0.001 if _PLATFORM != 'Windows' else 0.016
-        
-        while True:
-            nearest_next = deq[0] + interval
-            wait_time = nearest_next - time.time()
-            if wait_time <= 0: break 
-            
-            #Note that on asyncio asleeping nything below 1 ms won't work
-            # and on Windows it may sleep as much as ~15 ms less
-            # However the while loop will eliminate that problem.
-            wait_time = max(lowest, wait_time)
-            msg = _get_msg(func, instance, 'calls blocked for {}s.'.format(round(wait_time, 2)))
-            await _async_handle_action(action, msg, logging_lvl, WaitException, [wait_time],
-                                       {'msg':msg}, wait_time, lock, retain_order=retain_order)
-            
-            if action != 'sleep': break
-                    
-                    
-        deq.append(time.time())
-            
-            
-    finally:
-        lock.release()
-
-
-def async_limitcalls(limit, interval=None, action='error', bound=None, **kw):
-    
-    """Decorator for counting the calls to the decorated function.
-        Args:
-         limit (int): 
-           number of maximum calls [absolute or periodic] to the function
-           if exceeded, action is taken
-           
-         interval (int,float,timedelta,::None):
-           ::None - limit is absolute (action taken if total > limit)
-           ::<int,float> -> converted to timedelta(seconds(int,float))
-           ::<timedelta> - calls are timestamped, action taken if rate is exceeded in interval (now-timedelta, now)
-           
-         action (str/None):
-           what happens when call rate is exceeded
-           ::error - raises TerminatedException if interval=None and limit exceeded,
-                     raises WaitException if interval!= None and limit exceeded
-           ::sleep - sleeps till nr_calls won't exceed limit in interval, then proceeds
-           ::warn  - warns user with the error message, but proceeds
-           ::log   - logs the error message, but proceeds
-           ::None  - does nothing if call rate exceeded, proceeds with call
-           
-         bound (bool):
-           if method, then whether the calls to are counted separately by each instance
-           IMPORTANT: does not differentiate inherited methods from their source (i.e A.a == B(A).a [if a was inherited])
-           ::True - first arg is assumed to be 'self', calls to func counted separately by each instance
-           ::False - calls to func counted universally
-           ::<callable> - instance is resolved by <callable>(args[0])
-           ::None - auto-detects if the function is defined in class and has 'self' as first param,
-                    if so then bound = True, otherwise False
-                    Fails if: -method *without* "self" as first param (but intended to be bound)
-                              -method was defined outside class (and intended to be bound)
-                              -@staticmethod with "self" as first param
-                              In those cases if you're lazy typing bound=True/False, 
-                               use @limitcalls_f / @limitcalls_m instead
-                    
-        **kw:
-         logging_level (int):
-           logging level for error messages if action == 'log' / 'sleep'
-           DEFAULT: DEBUG for 'sleep' action, WARNING for 'log'
-        retain_order (bool):
-           whether or not function call order is retained when blocked by lock
-           DEFAULT: False
-        loop:
-          event loop for the Lock
-         f (function):
-           if used not as decorator (@limitcalls), but for converting an existing function,
-           can do new_f = limitcalls(...,f=f) [instead of new_f = limitcalls(...)(f)]"""
-         
-           
-    
-    if isinstance(interval, td):
-        interval = interval.total_seconds()
-        
-    elif interval is None and action=='sleep':
-        raise ValueError('Action cannot be "sleep" if interval not specified.')
-    
-    elif not isinstance(interval, (int, float, type(None))):
-        raise TypeError(type(interval))
-    
-    
-    
-    if not isinstance(limit,int):
-        raise TypeError(type(limit))
-    
-
-
-    if action == 'sleep':
-        logging_lvl = _LIMITCALLS_SLEEP_LOGGING_LEVEL
-    else:logging_lvl = _LIMITCALLS_LOGGING_LEVEL
-    
-    if kw.get('logging_level') is not None:
-        logging_lvl = kw['logging_level']
-    
-    if kw.get('retain_order') is not None:
-        retain_order = kw['retain_order']
-    else:retain_order = _LIMITCALLS_RETAIN_ORDER
-        
-    if hasattr(bound,'__call__'): pass   
-    elif not isinstance(bound,(bool,type(None))):
-        raise TypeError(type(bound))
-
-    
-    
-    if not isinstance(action,(str,type(None))):
-        raise TypeError(type(action))
-    
-    elif action not in ('error','sleep','warn','log',None):
-        raise ValueError(action)
-    
-    loop = kw.get('loop')
-    f = kw.get('f')
-
-
-       
-    
-    def actual_decorator(func):
-        PARAMS = (limit, interval, action, logging_lvl, retain_order)
-        LOCKS = {'func': asyncio.Lock(loop=loop), 'instances': {}}
-        HISTORY = {'func': deque(maxlen=limit), 'instances': {}}
-
-        bound2 = bound
-        #note to self:
-        # cannot do: bound = new_value
-        # (for some bound cannot be overwritten, otherwise it is lost from locals)
-        
-        
-        #check if has self (eliminates ordinary funcs and @classmethod/@staticmethod, 
-        #                   assuming user has *not* defined self as first param)
-        #if has "self" as first param, checks if the func is defined in the body of class
-        #  (further eliminates functions defined outside class' [0th level] body )
-        #  --note that __qualname__ may be given in other situations too 
-        #  --but tested that it *wasn't* present if the body was module or function
-        
-        #Note: the functionality still remains even if @classmethod has "self" as first param
-        #  because first input param cls remains the same; however that is only implemented if
-        #  bound = True; if left to None the inherited classmethods will be treated as identical
-        
-        
-        if bound2 is not None: pass
-        elif not _has_self(func): bound2 = False
-        else:
-            #__qualname__ only given if frame is located in the body of a class
-            frame = currentframe().f_back
-            if f: frame = frame.f_back
-
-            #getargvalues returns namedtuple
-            fr_locals = getargvalues(frame).locals
-            #print(fr_locals.get('__qualname__'), '__qualname__' in fr_locals, func.__name__)
-
-            
-            try: bound2 = fr_locals['__qualname__'] is not None
-            except KeyError: bound2 = False
-                
-        
-
-        @wraps(func)
-        async def wrapper(*args,**kw):
-            instance = _resolve_instance(func, args, bound, bound2)
-            await _async_handle_request(func, PARAMS, LOCKS, HISTORY, instance)
-
-            return await func(*args, **kw)
-
-
-
-        if _LIMITCALLS_STORE_GLOBALLY:
-            _LIMITCALLS_PARAMS[wrapper] = PARAMS
-            _LIMITCALLS_HISTORY[wrapper] =  HISTORY
-            
-    
-        return wrapper
-
-
-
-    
-    if f: return actual_decorator(f)
-    
-    
-    return actual_decorator
-
-
-
-def async_limitcalls_f(limit, interval=None, action='error', **kw):
-    """For ordinary functions and classmethods/staticmethods, 
-        or if calls to method are not intended do be counted separately for each instance"""
-    return async_limitcalls(limit, interval, action, bound=False, **kw)
-
-
-def async_limitcalls_m(limit, interval=None, action='error', **kw):
-    """For methods"""
-    return async_limitcalls(limit, interval, action, bound=True, **kw)
-    
+from functools import wraps
+from inspect import currentframe, getargvalues, getfullargspec
+
+import traceback
+import platform
+import copy
+import time
+import datetime
+
+dt = datetime.datetime
+td = datetime.timedelta
+
+from collections import deque
+from queue import Queue
+import asyncio
+import math
+import warnings
+import logging
+import inspect
+
+from fons.errors import WaitException, TerminatedException
+
+
+_LIMITCALLS_STORE_GLOBALLY = False
+_LIMITCALLS_PARAMS = {}
+_LIMITCALLS_HISTORY = {}
+
+_LIMITCALLS_LOGGING_LEVEL = logging.WARNING
+_LIMITCALLS_SLEEP_LOGGING_LEVEL = logging.DEBUG
+_LIMITCALLS_WARN_WHEN_SLEEP = False
+_LIMITCALLS_RETAIN_ORDER = False
+
+_PLATFORM = platform.system()
+
+
+# If method called as static, initializes necessary attributes (passed as kwargs)
+#   to class (instead of instance), without changing the original class attrbs
+# If called as class but without kwargs, assumes class already has those attrbs
+
+
+class hybridmethod(object):
+    def __init__(self, func):
+        self.func = func
+
+    def __get__(self, obj, cls):
+        context = obj if obj is not None else cls
+
+        # create new class to not overwrite its attrbs
+        if context is cls:
+
+            class NewoO(context):
+                pass
+
+            context = NewoO
+            K_name = cls.__name__
+            K_name_part = "__" + K_name + "_"
+
+            for attr_name in vars(cls):
+                if K_name_part in attr_name and attr_name[-2:] != "__":
+                    attr_short = attr_name.replace(K_name_part, "")
+                    attr_value = getattr(cls, attr_name)
+                    setattr(context, "__" + attr_short, copy.deepcopy(attr_value))
+
+        @wraps(self.func)
+        def hybrid(*args, **kw):
+            # inits only if context is class (not self (instance))
+            # offers to not init some kw for class too:
+            init_kw = kw
+            if "_static_vars" in kw:
+                init_kw = {k: v for k, v in kw.items() if k not in kw["_static_vars"]}
+                kw = {k: v for k, v in kw.items() if k in kw["_static_vars"]}
+                del init_kw["_static_vars"]
+            else:
+                init_kw = kw.copy()
+                # kw = {}
+
+            for k, v in init_kw.items():
+                try:
+                    # checks if is class (don't want to overwrite self attrbs):
+                    if isinstance(context, type):
+                        setattr(context, k, v)
+                except Exception:
+                    traceback.print_exc()
+
+            return self.func(context, *args, **kw)
+
+            # Exceptions (when one *must* use _static_vars):
+            # instance method checks if it has attr which's name also happens to be in its kwargs
+            # (therefore answer would always be "yes" if we init it to class 'New')
+            # if a kwarg happens to be an attr of *class* "context" aswell
+            # (although I can differ an instance from class/static, I can't
+            #  differ class from static (since static is called *from* the class)
+            #  therefore if its a class its attr is overwritten with the kwarg)
+
+        # optional, mimic methods some more
+        hybrid.__func__ = hybrid.im_func = self.func
+        hybrid.__self__ = hybrid.im_self = context
+
+        return hybrid
+
+
+def obj_to_class(obj):
+    klass = obj
+    if not isinstance(obj, type):
+        klass = eval(obj.__class__.__name__)
+
+    return klass
+
+
+def mro_without_wrapper(obj):
+    klass = obj_to_class(obj)
+
+    loc = next(
+        (
+            i
+            for i, k in enumerate(klass.mro())
+            if "hybridmethod" not in k or "NewoO" not in k
+        ),
+        0,
+    )
+
+    mro_list = klass.mro()[loc:]
+
+    return mro_list
+
+
+# like super(klass), except for 'NewoO'-s is returned its grandparent
+def superb(cls):
+    mro_list = mro_without_wrapper(cls)
+    superklass = eval(mro_list[1].__name__)
+    return superklass
+
+
+def superclasses(obj):
+    klass = obj_to_class(obj)
+
+    if klass is not obj:
+        # method was called from instance
+        loc = 1
+    else:
+        # method was called from class
+        loc = next(
+            (
+                i
+                for i, k in enumerate(klass.mro())
+                if "hybridmethod" not in k or "NewoO" not in k
+            ),
+            None,
+        )
+
+        if loc is None:
+            return
+
+    superklasses = [eval(k.__name__) for k in klass.mro()[loc:-1]]
+    # all classes above the class of obj, except the last one ('object')
+    # will they evaluate if in different modules? probably yes
+
+    return superklasses
+
+
+def find_all_double_underscore_vars(obj, var_name, superklasses=None):
+    if not isinstance(superklasses, (tuple, list)):
+        superklasses = superclasses(obj)
+
+    sk = superklasses[:]
+    sk.insert(0, obj_to_class(obj))
+
+    a_list = []
+
+    for K in sk:
+        try:
+            a_list.append(eval("K._{}__{}".format(K.__name__, var_name)))
+        except Exception:
+            pass
+
+    return a_list
+
+
+def get_arg_count(f):
+    argspec = inspect.getfullargspec(f)
+    if argspec.varargs:
+        return math.inf
+    # from_i = 0 if not argspec.args or argspec.args[0] != 'self' else 1
+    # inspect.ismethod is accurate whether or not "self" is first arg,
+    # or when it only has *args; works for classmethods (initated or not) too
+    from_i = 0 if not inspect.ismethod(f) else 1
+    return len(argspec.args[from_i:])
+
+
+# ----------------------------------------------------------------------------
+
+
+def _has_self(f):
+    fas = getfullargspec(f)
+    args = fas[0]
+
+    if len(args) and args[0] == "self":
+        return True
+
+    return False
+
+
+def _resolve_instance(func, args, bound, bound2):
+    if hasattr(bound, "__call__"):
+        instance = bound(args[0])
+
+    elif bound:
+        instance = args[0]
+
+    elif bound2 and not isinstance(args[0], type):
+        # user has left bound=None, and first param is "self"
+        # only accept if args[0] is not cls (accidental classmethod)
+        # (we don't want to *accidentally* use cls as the identifier,
+        # because the cls would differ for subclasses while the function is same)
+        instance = args[0]
+
+    else:
+        instance = None
+
+    if not hasattr(instance, "__hash__"):
+        first_param = getfullargspec(func)["args"][0]
+
+        raise TypeError(
+            (
+                'Function "{}" is bound, '
+                'but its first param "{}" of type {} is not hashable'
+            ).format(func.__name__, first_param, type(instance))
+        )
+
+    return instance
+
+
+def _get_msg(func, instance, text):
+    if instance is not None:
+        txt0 = "Limitcall on method {} of instance {}: ".format(func.__name__, instance)
+    else:
+        txt0 = "Limitcall on function {}: ".format(func.__name__)
+
+    msg = txt0 + text.strip()
+
+    return msg
+
+
+"""class _TimeShort:
+    def __init__(self, deq, interval):
+        self.deq = deq
+        self.interval = interval
+        
+    def __call__(self):
+        nearest_next = self.deq[0] + self.interval
+        self.time_short = time_short = (nearest_next - dt.utcnow())/td(seconds=1)
+        
+        return time_short
+    
+    __slots__ = ['deq','interval','time_short']"""
+
+
+def _handle_action(
+    action, msg, logging_level, exception=None, args=[], kwargs={}, sleep_time=0
+):
+    if action == "error":
+        raise exception(*args, **kwargs)
+    elif action == "warn":
+        warnings.warn(msg)
+    elif action == "log":
+        logging.log(logging_level, msg)
+
+    elif action == "sleep":
+        msg += " --- sleeping {}s".format(round(sleep_time, 3))
+        logging.log(logging_level, msg)
+
+        if _LIMITCALLS_WARN_WHEN_SLEEP:
+            warnings.warn(msg)
+
+        time.sleep(sleep_time)
+
+
+def _handle_request(func, PARAMS, QUEUES, HISTORY, instance=None):
+    limit, interval, action, logging_lvl = PARAMS
+
+    if instance is None:
+        deq = HISTORY["func"]
+        queue = QUEUES["func"]
+
+    elif instance not in HISTORY["instances"]:
+        HISTORY["instances"][instance] = deq = deque(maxlen=limit)
+        QUEUES["instances"][instance] = queue = Queue(1)
+
+    else:
+        deq = HISTORY["instances"][instance]
+        queue = QUEUES["instances"][instance]
+
+    lvl = logging_lvl if queue.full() else 0
+    logging.log(lvl, _get_msg(func, instance, "waiting on lock"))
+
+    try:
+        queue.put(None)
+        logging.log(lvl, _get_msg(func, instance, "lock acquired"))
+
+        if len(deq) < limit:
+            deq.append(time.time())
+            return
+        elif interval is None:
+            msg = _get_msg(
+                func, instance, "has reached its total max calls {}".format(limit)
+            )
+            _handle_action(action, msg, logging_lvl, TerminatedException, [msg])
+            return
+
+        # If action is 'sleep', in every cycle the lock will be released before the sleep,
+        # (so that the other calls don't have to wait), then acquired again
+        # repeated until time_short > 0
+
+        while True:
+            nearest_next = deq[0] + interval
+            wait_time = nearest_next - time.time()
+            if wait_time <= 0:
+                break
+
+            msg = _get_msg(
+                func, instance, "calls blocked for {}s.".format(round(wait_time, 3))
+            )
+            _handle_action(
+                action,
+                msg,
+                logging_lvl,
+                WaitException,
+                [wait_time],
+                {"msg": msg},
+                wait_time,
+            )
+
+            if action != "sleep":
+                break
+
+        deq.append(time.time())
+
+    finally:
+        queue.get()
+
+
+# Note: methods of instances of same class have different ids,
+#      but limitcalls makes no difference, since it first wraps
+#      during the time of class initiation
+#      set 'bound' to True (or leave None) for each instance calls
+#        to method be counted separately
+
+
+def limitcalls(limit, interval=None, action="error", bound=None, **kw):
+    """Decorator for counting the calls to the decorated function.
+    Args:
+     limit (int):
+       number of maximum calls [absolute or periodic] to the function
+       if exceeded, action is taken
+
+     interval (int,float,timedelta,::None):
+       ::None - limit is absolute (action taken if total > limit)
+       ::<int,float> -> converted to timedelta(seconds(int,float))
+       ::<timedelta> - calls are timestamped, action taken if rate is exceeded in interval (now-timedelta, now)
+
+     action (str/None):
+       what happens when call rate is exceeded
+       ::error - raises TerminatedException if interval=None and limit exceeded,
+                 raises WaitException if interval!= None and limit exceeded
+       ::sleep - sleeps till nr_calls won't exceed limit in interval, then proceeds
+       ::warn  - warns user with the error message, but proceeds
+       ::log   - logs the error message, but proceeds
+       ::None  - does nothing if call rate exceeded, proceeds with call
+
+     bound (bool):
+       if method, then whether the calls to are counted separately by each instance
+       IMPORTANT: does not differentiate inherited methods from their source (i.e A.a == B(A).a [if a was inherited])
+       ::True - first arg is assumed to be 'self', calls to func counted separately by each instance
+       ::False - calls to func counted universally
+       ::<callable> - instance is resolved by <callable>(args[0])
+       ::None - auto-detects if the function is defined in class and has 'self' as first param,
+                if so then bound = True, otherwise False
+                Fails if: -method *without* "self" as first param (but intended to be bound)
+                          -method was defined outside class (and intended to be bound)
+                          -@staticmethod with "self" as first param
+                          In those cases if you're lazy typing bound=True/False,
+                           use @limitcalls_f / @limitcalls_m instead
+
+    **kw:
+     logging_level (int):
+       logging level for error messages if action == 'log' / 'sleep'
+       DEFAULT: DEBUG for 'sleep' action, WARNING for 'log'
+     f (function):
+       if used not as decorator (@limitcalls), but for converting an existing function,
+       can do new_f = limitcalls(...,f=f) [instead of new_f = limitcalls(...)(f)]"""
+
+    if isinstance(interval, td):
+        interval = interval.total_seconds()
+
+    elif interval is None and action == "sleep":
+        raise ValueError('Action cannot be "sleep" if interval not specified.')
+
+    elif not isinstance(interval, (int, float, type(None))):
+        raise TypeError(type(interval))
+
+    if not isinstance(limit, int):
+        raise TypeError(type(limit))
+
+    if action == "sleep":
+        logging_lvl = _LIMITCALLS_SLEEP_LOGGING_LEVEL
+    else:
+        logging_lvl = _LIMITCALLS_LOGGING_LEVEL
+
+    if kw.get("logging_level") is not None:
+        logging_lvl = kw["logging_level"]
+
+    if hasattr(bound, "__call__"):
+        pass
+    elif not isinstance(bound, (bool, type(None))):
+        raise TypeError(type(bound))
+
+    if not isinstance(action, (str, type(None))):
+        raise TypeError(type(action))
+
+    elif action not in ("error", "sleep", "warn", "log", None):
+        raise ValueError(action)
+
+    f = kw.get("f")
+
+    def actual_decorator(func):
+        PARAMS = (limit, interval, action, logging_lvl)
+        QUEUES = {"func": Queue(1), "instances": {}}
+        HISTORY = {"func": deque(maxlen=limit), "instances": {}}
+
+        bound2 = bound
+        # note to self:
+        # cannot do: bound = new_value
+        # (for some bound cannot be overwritten, otherwise it is lost from locals)
+
+        # check if has self (eliminates ordinary funcs and @classmethod/@staticmethod,
+        #                   assuming user has *not* defined self as first param)
+        # if has "self" as first param, checks if the func is defined in the body of class
+        #  (further eliminates functions defined outside class' [0th level] body )
+        #  --note that __qualname__ may be given in other situations too
+        #  --but tested that it *wasn't* present if the body was module or function
+
+        # Note: the functionality still remains even if @classmethod has "self" as first param
+        #  because first input param cls remains the same; however that is only implemented if
+        #  bound = True; if left to None the inherited classmethods will be treated as identical
+
+        if bound2 is not None:
+            pass
+        elif not _has_self(func):
+            bound2 = False
+        else:
+            # __qualname__ only given if frame is located in the body of a class
+            frame = currentframe().f_back
+            if f:
+                frame = frame.f_back
+
+            # getargvalues returns namedtuple
+            fr_locals = getargvalues(frame).locals
+            # print(fr_locals.get('__qualname__'), '__qualname__' in fr_locals, func.__name__)
+
+            try:
+                bound2 = fr_locals["__qualname__"] is not None
+            except KeyError:
+                bound2 = False
+
+        @wraps(func)
+        def wrapper(*args, **kw):
+            instance = _resolve_instance(func, args, bound, bound2)
+            _handle_request(func, PARAMS, QUEUES, HISTORY, instance)
+
+            return func(*args, **kw)
+
+        if _LIMITCALLS_STORE_GLOBALLY:
+            _LIMITCALLS_PARAMS[wrapper] = PARAMS
+            _LIMITCALLS_HISTORY[wrapper] = HISTORY
+
+        return wrapper
+
+    if f:
+        return actual_decorator(f)
+
+    return actual_decorator
+
+
+def limitcalls_f(limit, interval=None, action="error", **kw):
+    """For ordinary functions and classmethods/staticmethods,
+    or if calls to method are not intended do be counted separately for each instance"""
+    return limitcalls(limit, interval, action, bound=False, **kw)
+
+
+def limitcalls_m(limit, interval=None, action="error", **kw):
+    """For methods"""
+    return limitcalls(limit, interval, action, bound=True, **kw)
+
+
+# -------------------------------------------------------------------------------------------
+
+
+async def _async_handle_action(
+    action,
+    msg,
+    logging_level,
+    exception=None,
+    args=[],
+    kwargs={},
+    sleep_time=0,
+    lock=None,
+    retain_order=False,
+):
+    if action == "error":
+        raise exception(*args, **kwargs)
+    elif action == "warn":
+        warnings.warn(msg)
+    elif action == "log":
+        logging.log(logging_level, msg)
+
+    elif action == "sleep":
+        msg += " --- sleeping {}s".format(round(sleep_time, 2))
+        logging.log(logging_level, msg)
+
+        if _LIMITCALLS_WARN_WHEN_SLEEP:
+            warnings.warn(msg)
+
+        if lock is not None and lock.locked() and not retain_order:
+            lock.release()
+
+        await asyncio.sleep(sleep_time)
+
+        if lock is not None and not retain_order:
+            await lock.acquire()
+
+
+async def _async_handle_request(func, PARAMS, LOCKS, HISTORY, instance=None):
+    limit, interval, action, logging_lvl, retain_order = PARAMS
+
+    if instance is None:
+        deq = HISTORY["func"]
+        lock = LOCKS["func"]
+
+    elif instance not in HISTORY["instances"]:
+        HISTORY["instances"][instance] = deq = deque(maxlen=limit)
+        LOCKS["instances"][instance] = lock = asyncio.Lock()
+
+    else:
+        deq = HISTORY["instances"][instance]
+        lock = LOCKS["instances"][instance]
+
+    lvl = logging_lvl if lock.locked() and retain_order else 0
+    logging.log(lvl, _get_msg(func, instance, "waiting on lock"))
+
+    try:
+        await lock.acquire()
+        logging.log(lvl, _get_msg(func, instance, "lock acquired"))
+
+        if len(deq) < limit:
+            deq.append(time.time())
+            return
+        elif interval is None:
+            msg = _get_msg(
+                func, instance, "has reached its total max calls {}".format(limit)
+            )
+            await _async_handle_action(
+                action,
+                msg,
+                logging_lvl,
+                TerminatedException,
+                [msg],
+                retain_order=retain_order,
+            )
+            return
+
+        # If action is 'sleep', in every cycle the lock will be released before the sleep,
+        # (so that the other calls don't have to wait), then acquired again
+        # repeated until time_short > 0
+        lowest = 0.001 if _PLATFORM != "Windows" else 0.016
+
+        while True:
+            nearest_next = deq[0] + interval
+            wait_time = nearest_next - time.time()
+            if wait_time <= 0:
+                break
+
+            # Note that on asyncio asleeping nything below 1 ms won't work
+            # and on Windows it may sleep as much as ~15 ms less
+            # However the while loop will eliminate that problem.
+            wait_time = max(lowest, wait_time)
+            msg = _get_msg(
+                func, instance, "calls blocked for {}s.".format(round(wait_time, 2))
+            )
+            await _async_handle_action(
+                action,
+                msg,
+                logging_lvl,
+                WaitException,
+                [wait_time],
+                {"msg": msg},
+                wait_time,
+                lock,
+                retain_order=retain_order,
+            )
+
+            if action != "sleep":
+                break
+
+        deq.append(time.time())
+
+    finally:
+        lock.release()
+
+
+def async_limitcalls(limit, interval=None, action="error", bound=None, **kw):
+    """Decorator for counting the calls to the decorated function.
+    Args:
+     limit (int):
+       number of maximum calls [absolute or periodic] to the function
+       if exceeded, action is taken
+
+     interval (int,float,timedelta,::None):
+       ::None - limit is absolute (action taken if total > limit)
+       ::<int,float> -> converted to timedelta(seconds(int,float))
+       ::<timedelta> - calls are timestamped, action taken if rate is exceeded in interval (now-timedelta, now)
+
+     action (str/None):
+       what happens when call rate is exceeded
+       ::error - raises TerminatedException if interval=None and limit exceeded,
+                 raises WaitException if interval!= None and limit exceeded
+       ::sleep - sleeps till nr_calls won't exceed limit in interval, then proceeds
+       ::warn  - warns user with the error message, but proceeds
+       ::log   - logs the error message, but proceeds
+       ::None  - does nothing if call rate exceeded, proceeds with call
+
+     bound (bool):
+       if method, then whether the calls to are counted separately by each instance
+       IMPORTANT: does not differentiate inherited methods from their source (i.e A.a == B(A).a [if a was inherited])
+       ::True - first arg is assumed to be 'self', calls to func counted separately by each instance
+       ::False - calls to func counted universally
+       ::<callable> - instance is resolved by <callable>(args[0])
+       ::None - auto-detects if the function is defined in class and has 'self' as first param,
+                if so then bound = True, otherwise False
+                Fails if: -method *without* "self" as first param (but intended to be bound)
+                          -method was defined outside class (and intended to be bound)
+                          -@staticmethod with "self" as first param
+                          In those cases if you're lazy typing bound=True/False,
+                           use @limitcalls_f / @limitcalls_m instead
+
+    **kw:
+     logging_level (int):
+       logging level for error messages if action == 'log' / 'sleep'
+       DEFAULT: DEBUG for 'sleep' action, WARNING for 'log'
+    retain_order (bool):
+       whether or not function call order is retained when blocked by lock
+       DEFAULT: False
+    loop:
+      event loop for the Lock
+     f (function):
+       if used not as decorator (@limitcalls), but for converting an existing function,
+       can do new_f = limitcalls(...,f=f) [instead of new_f = limitcalls(...)(f)]"""
+
+    if isinstance(interval, td):
+        interval = interval.total_seconds()
+
+    elif interval is None and action == "sleep":
+        raise ValueError('Action cannot be "sleep" if interval not specified.')
+
+    elif not isinstance(interval, (int, float, type(None))):
+        raise TypeError(type(interval))
+
+    if not isinstance(limit, int):
+        raise TypeError(type(limit))
+
+    if action == "sleep":
+        logging_lvl = _LIMITCALLS_SLEEP_LOGGING_LEVEL
+    else:
+        logging_lvl = _LIMITCALLS_LOGGING_LEVEL
+
+    if kw.get("logging_level") is not None:
+        logging_lvl = kw["logging_level"]
+
+    if kw.get("retain_order") is not None:
+        retain_order = kw["retain_order"]
+    else:
+        retain_order = _LIMITCALLS_RETAIN_ORDER
+
+    if hasattr(bound, "__call__"):
+        pass
+    elif not isinstance(bound, (bool, type(None))):
+        raise TypeError(type(bound))
+
+    if not isinstance(action, (str, type(None))):
+        raise TypeError(type(action))
+
+    elif action not in ("error", "sleep", "warn", "log", None):
+        raise ValueError(action)
+
+    loop = kw.get("loop")
+    f = kw.get("f")
+
+    def actual_decorator(func):
+        PARAMS = (limit, interval, action, logging_lvl, retain_order)
+        LOCKS = {"func": asyncio.Lock(), "instances": {}}
+        HISTORY = {"func": deque(maxlen=limit), "instances": {}}
+
+        bound2 = bound
+        # note to self:
+        # cannot do: bound = new_value
+        # (for some bound cannot be overwritten, otherwise it is lost from locals)
+
+        # check if has self (eliminates ordinary funcs and @classmethod/@staticmethod,
+        #                   assuming user has *not* defined self as first param)
+        # if has "self" as first param, checks if the func is defined in the body of class
+        #  (further eliminates functions defined outside class' [0th level] body )
+        #  --note that __qualname__ may be given in other situations too
+        #  --but tested that it *wasn't* present if the body was module or function
+
+        # Note: the functionality still remains even if @classmethod has "self" as first param
+        #  because first input param cls remains the same; however that is only implemented if
+        #  bound = True; if left to None the inherited classmethods will be treated as identical
+
+        if bound2 is not None:
+            pass
+        elif not _has_self(func):
+            bound2 = False
+        else:
+            # __qualname__ only given if frame is located in the body of a class
+            frame = currentframe().f_back
+            if f:
+                frame = frame.f_back
+
+            # getargvalues returns namedtuple
+            fr_locals = getargvalues(frame).locals
+            # print(fr_locals.get('__qualname__'), '__qualname__' in fr_locals, func.__name__)
+
+            try:
+                bound2 = fr_locals["__qualname__"] is not None
+            except KeyError:
+                bound2 = False
+
+        @wraps(func)
+        async def wrapper(*args, **kw):
+            instance = _resolve_instance(func, args, bound, bound2)
+            await _async_handle_request(func, PARAMS, LOCKS, HISTORY, instance)
+
+            return await func(*args, **kw)
+
+        if _LIMITCALLS_STORE_GLOBALLY:
+            _LIMITCALLS_PARAMS[wrapper] = PARAMS
+            _LIMITCALLS_HISTORY[wrapper] = HISTORY
+
+        return wrapper
+
+    if f:
+        return actual_decorator(f)
+
+    return actual_decorator
+
+
+def async_limitcalls_f(limit, interval=None, action="error", **kw):
+    """For ordinary functions and classmethods/staticmethods,
+    or if calls to method are not intended do be counted separately for each instance"""
+    return async_limitcalls(limit, interval, action, bound=False, **kw)
+
+
+def async_limitcalls_m(limit, interval=None, action="error", **kw):
+    """For methods"""
+    return async_limitcalls(limit, interval, action, bound=True, **kw)
```

### Comparing `fons-0.3.1/fons/gui.py` & `fons-0.4.0/fons/gui.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,510 +1,563 @@
-"""
-Make sure you have tkinter installed before using the features of this module.
-`sudo apt-get install python3-tk`
-"""
-import json
-from copy import deepcopy
-from collections import OrderedDict
-import multiprocessing
-import time
-import sys
-import shlex
-
-from fons.dict_ops import deep_update
-from fons.errors import QuitException
-from fons.io import update_settings, _META_NORM
-from fons.log import (get_standard_5, init_tab, standard_logging)
-from fons.processes import TkLogiProcess
-from fons.py import rreload
-from fons.sched import Ticker
-from fons.threads import EliThread
-
-
-NON_RESPONSIVE = ('debug*','info*','warning*','error*','critical*','main')
-RRELOAD_BUTTON = False
-
-logger,logger2,tlogger,tloggers,tlogger0 = get_standard_5(__name__)
-
-
-def get_default_CFG(processes, dtypes=None):
-    _process = {
-        '_type_': dict,
-        'default_dtype': None,
-        'dtypes': {
-            'target': {'_type_': str},
-            'args': list,
-            'kwargs': dict,
-            'argv': {'_type_': (str, list), '_defval_': None},
-            'conn': bool,
-            'start': bool,
-        }
-    }
-    if dtypes is None:
-        dtypes = {}
-    return {
-        '_type_': dict,
-        'default_dtype': None,
-        'dtypes': {
-           'processes': {
-               '_type_': dict,
-               # 'keys': list(processes),
-               'unit': _process
-            },
-            '__meta__': deepcopy(_META_NORM),
-            **dtypes,
-        }
-    }
-
-
-class NbGUI:
-    """Notebook styled gui"""
-    def __init__(self, config={}):
-        import tkinter as tk
-        import tkinter.ttk as ttk
-        
-        self.root = tk.Tk()
-        self.root.geometry('975x475')
-        #self.root.resizable(0, 0)
-        
-        if config.get('title') is not None:
-            self.root.title(config['title'])
-        
-        left_frame = tk.Frame(self.root)
-        left_frame.pack(side=tk.LEFT)
-        buttons_frame = tk.Frame(left_frame)
-        buttons_frame.pack()
-        entries_frame = tk.Frame(left_frame)
-        entries_frame.pack(pady=(10, 0))
-        
-        self.nb = ttk.Notebook(self.root)
-        #self.nb.grid(row=1, column=0, columnspan=50, rowspan=49, sticky='NESW')
-        #self.nb.pack_propagate(0) 
-        self.nb.pack(side=tk.LEFT, fill='both', expand=True)
-        
-        self.tabs = []
-        self.tab_selected = None
-        self.variables = {}
-        self.values = {} # by (tab_name, var_name)
-        self.default_values = {} # by var_name
-            
-        buttons = config.get('buttons')
-        if buttons is None: buttons = {}
-        for button_name, specs in buttons.items():
-            callback = self.wrap_button(specs['command']) if specs.get('command') else None
-            text = specs.get('text')
-            b = tk.Button(buttons_frame, text=text, command=callback)
-            b.pack()
-        
-        entries = config.get('entries')
-        if entries is None: entries = {}
-        for var_name, specs in entries.items():
-            label = specs.get('label')
-            width = specs['width'] if specs.get('width') else 12
-            self.default_values[var_name] = value = specs['value'] if specs.get('value') else ''
-            ef = tk.Frame(entries_frame)
-            ef.pack()
-            if label:
-                tk.Label(ef, text=label).pack(side=tk.LEFT)
-            self.variables[var_name] = var = tk.StringVar(value=value)
-            tk.Entry(ef, textvariable=var, width=width).pack(side=tk.LEFT)
-        
-        tabs = _tabs = config.get('tabs')
-        if tabs is None: tabs = {}
-        elif not isinstance(tabs, dict):
-            tabs = {}
-            for item in _tabs:
-                if isinstance(item, dict):
-                    tab_name, specs = item['text'], item
-                else:
-                    tab_name, specs = item, {}
-                tabs[tab_name] = specs
-        
-        for tab_name, specs in tabs.items():
-            values = specs.get('values') # by var_name
-            if values is None:
-                values = {}
-            elif isinstance(values, str):
-                values = dict.fromkeys(self.variables, values)
-            self.add_new_tab(tab_name, values)
-    
-    
-    def add_new_tab(self, tab, variable_values={}):
-        if tab in self.tabs:
-            return
-        self.tabs.append(tab)
-        init_tab(self.nb, tab)
-        for var_name in self.variables:
-            value = variable_values.get(tab)
-            if value is None:
-                value = self.default_values[var_name]
-            self.values[(tab, var_name)] = value
-    
-    
-    def refresh(self, recursive=False):
-        tab_selected = self.nb.tab(self.nb.select(), 'text')
-        if self.tab_selected != tab_selected:
-            for var_name, variable in self.variables.items():
-                value = self.values.get((tab_selected, var_name))
-                if value is None:
-                    value = ''
-                variable.set(value)
-            self.tab_selected = tab_selected
-        
-        for var_name, variable in self.variables.items():
-            self.values[(tab_selected, var_name)] = variable.get()
-        
-        if recursive:
-            self.root.after(recursive, self.refresh, recursive)
-    
-    
-    def wrap_button(self, f):
-        def on_button(*args,**kw):
-            tab_selected = self.nb.tab(self.nb.select(), 'text')
-            return f(tab_selected, *args, **kw)
-        return on_button
-
-
-class TkThread(EliThread):
-    def __init__(self, config, *args, **kw):
-        super().__init__(*args,**kw)
-        self.config = config
-        self.start()
-    
-    def run(self):
-        """It is important that the gui is initiated inside the running thread"""
-        self.gui = NbGUI(self.config)
-        self.gui.refresh(recursive=300)
-        self.gui.root.mainloop()
-
-
-def ignore(f):
-    def check_ignore(*args,**kw):
-        try: name = args[1] # (0 = self)
-        except IndexError:
-            name = kw['name']
-        if name not in NON_RESPONSIVE:
-            return f(*args,**kw)
-    return check_ignore
-
-
-class TkLogiProcessComplex:
-    def __init__(self, processes={}, *, settings_path=None, cfg=None, CFG=None,
-                 functions={}, title='TkLogiProcessComplex', termination_time=60, main_termination_time=75,
-                 logging_dir=None, dpath=None, rreload_button=None):
-        """
-        :type processes: dict
-            {
-                process_name: {
-                    target: function,
-                    args: (...),
-                    kwargs: {...},
-                    argv: 'put something here',      # can also be list ['put', 'something', 'here'] 
-                    conn: <bool>,                    # if True then function must accept `conn` as keyword (Pipe)
-                    start: <bool>                    # whether or not it is started on .start
-                }
-            }
-        about function:
-            may accept `argv` as keyword, should default to sys.argv
-            may accept `conn` as keyword
-        about conn (Pipe):
-            assumed to expect `None` as a cue to end itself (the function)
-            assumed to send `None` back when done
-        :type cfg: dict
-            initial contents of the file located at `settings_path`
-            cfg['processes'] is used to periodically deep update `self.processes`
-            { processes: processes }                 # where processes are equivalent to `processes` argument
-        """
-        self.processes = dict(processes)
-        self.verify_processes(self.processes)
-        self.settings_path = settings_path
-        self.cfg = deepcopy(cfg) if cfg is not None else {}
-        self.CFG = deepcopy(CFG) if CFG is not None else {}
-        self.functions = dict(functions)
-        self.title = title
-        self.termination_time = termination_time
-        self.main_termination_time = main_termination_time
-        self.logging_dir = logging_dir
-        self.dpath = dpath
-        self.rreload_button = rreload_button if rreload_button is not None else RRELOAD_BUTTON
-        
-        self.init_CFG()
-        
-        self._processes = {}
-        self._exit = None
-        self._cfg_updater = None
-        self._gui_thread = None
-        self._gui = None
-        self._nb = None
-        self._response_waiter = None
-    
-    
-    @staticmethod
-    def verify_processes(processes):
-        for name in processes:
-            if name in ('MainProcess', 'main'):
-                raise ValueError("Processname '{}' is not allowed".format(name))
-    
-    
-    def init_CFG(self):
-        self.CFG = deep_update(get_default_CFG(self.processes), self.CFG, copy=True)
-    
-    
-    def update_settings(self, add_new_process_tabs=False):
-        old_processes = self.cfg.get('processes', {})
-        c = self.cfg.get('__meta__', {}).get('counter', 0)
-        update_settings(self.settings_path, self.cfg, self.CFG)
-        c2 = self.cfg['__meta__']['counter']
-        
-        if not c or c2 > c:
-            # update_settings doesn't deep_update automatically
-            self.cfg['processes'] = deep_update(old_processes, self.cfg.get('processes', {}))
-            cfg_processes = self.cfg['processes']
-            if isinstance(cfg_processes, dict):
-                self.verify_processes(cfg_processes)
-                for p in cfg_processes:
-                    if p in self.processes:
-                        self.processes[p].update(cfg_processes[p])
-                    else:
-                        self.processes[p] = dict(cfg_processes[p])
-        
-        if add_new_process_tabs:
-            for p in self.processes:
-                if p not in self._gui.tabs:
-                    self._gui.root.after(1, self._gui.add_new_tab, p)
-    
-    
-    def init_process(self, name):
-        specs = self.processes[name]
-        target = specs['target']
-        
-        if target is None:
-            target = name
-        
-        if isinstance(target, str):
-            target = self.functions[target]
-        
-        argv = self._gui.values.get((name, 'argv'))
-        if not argv:
-            argv = specs.get('argv')
-        
-        if argv is None: pass
-        elif isinstance(argv, str):
-            argv = [''] + shlex.split(argv)
-        else:
-            argv = [''] + list(argv)
-        
-        conn = multiprocessing.Pipe() if specs.get('conn') else None
-        
-        args = tuple(specs['args']) if specs.get('args') is not None else ()
-        kwargs = dict(specs['kwargs']) if specs.get('kwargs') is not None else {}
-        if argv:
-            kwargs['argv'] = argv
-        if conn is not None:
-            kwargs['conn'] = conn[1]
-        
-        p = TkLogiProcess(self._nb,
-                          target=target,
-                          args=args,
-                          kwargs=kwargs,
-                          name=name,
-                          daemon=specs.get('daemon', False)) # this should be False, as it may spawn children
-        self._processes[name] = {'p': p, 'conn': conn, 'args': args,
-                                 'kwargs': kwargs, 'start': None, 'close': None,}
-        return p
-    
-    def del_process(self, name):
-        old = self._processes.get(name)
-        if not old: return
-        conn = old['conn']
-        if conn:
-            conn[0].close()
-            conn[1].close()
-        self._processes[name] = {}
-    
-    
-    def _check_is_not_running(self, name):
-        if not self._processes.get(name, {}).get('p'): pass
-        elif self._processes[name]['p'].is_alive():
-            logger2.error('Cannot start `{}`: is already running'.format(name))
-            return False
-        else:
-            self.del_process(name)
-        return True
-    
-    @ignore
-    def start_process(self, name):
-        if not self._check_is_not_running(name):
-            return
-        p = self.init_process(name)
-        _p = self._processes[name]
-        args_sfx = ' :: {}'.format(_p['args']) if _p['args'] else ''
-        kw_sfx = ' :: {}'.format(_p['kwargs']) if _p['kwargs'] else ''
-        logger2.info('Starting `{}`{}{}'.format(name, args_sfx, kw_sfx))
-        self._processes[name]['start'] = time.time()
-        p.start()
-        logger2.info('Starting of `{}` (pid: {}) successful'.format(name, p.pid))
-    
-    @ignore
-    def start_rl(self, name):
-        if not self._check_is_not_running(name):
-            return 
-        logger2.info('Attempting to reload `{}` modules'.format(name))
-        f = f0 = self.processes[name].get('target')
-        if f is None:
-            f = f0 = name
-        if isinstance(f, str):
-            f = self.functions[f]
-        module = sys.modules[f.__module__]
-        rreload(module)
-        f = getattr(module, f.__name__)
-        if isinstance(f0, str):
-            self.functions[f0] = f
-        else:
-            self.processes[name]['target'] = f
-        self.start_process(name)
-    
-    @ignore 
-    def restart_process(self, name):
-        logger2.info('Attempting to restart `{}`'.format(name))
-        self.stop_process(name)
-        self.start_process(name)
-    
-    
-    @ignore
-    def stop_process(self, name):
-        try: p = self._processes[name]['p']
-        except KeyError:
-            logger2.error('Cannot stop `{}`: has not been initiated'.format(name))
-            return
-        if self._processes[name]['close']:
-            logger2.error('`{}` is already waiting for termination.'.format(name))
-            return
-        if not p.is_alive():
-            logger2.error('Cannot stop `{}`: is not running'.format(name))
-            return
-        logger2.info('Scheduling `{}` for termination'.format(name))
-        self._processes[name]['close'] = time.time()
-        conn = self._processes[name]['conn']
-        if conn:
-            conn[0].send(None)
-        else:
-            self.force_terminate_process(name)
-    
-    
-    def force_terminate_process(self, name):
-        p = self._processes[name]['p']
-        logger2.info('Force terminating `{}`'.format(name))
-        p.terminate()
-        self.del_process(name)
-    
-    
-    def _wait_on_responses(self):
-        all_closed = True
-        for name,d in self._processes.copy().items():
-            p = d.get('p')
-            conn = d.get('conn')
-            start = d.get('start')
-            close = d.get('close')
-            updated = conn and conn[0].poll(0.01)
-            if not updated:
-                if not start or time.time() - start < 2:
-                    pass
-                elif not p.is_alive():
-                    logger2.info('`{}` has terminated.'.format(name))
-                    self.del_process(name)
-                elif close and time.time() - close > self.termination_time:
-                    logger2.info('`{}` has exceeded its allocated termination time. Force terminating.'.format(name))
-                    self.force_terminate_process(name)
-                else:
-                    all_closed = False
-                continue
-            
-            r = conn[0].recv()
-            logger2.info('Received from {}\'s conn: {}'.format(name, r))
-            if r is None:
-                logger2.info('Process `{}` has successfully terminated itself.'.format(name))
-                time.sleep(1)
-                if p.is_alive():
-                    logger2.error('But `{}` is till alive. Attempting force termination.'.format(name))
-                    try: self.force_terminate_process(name)
-                    except Exception as e:
-                        logger2.exception(e)
-                        all_closed = False
-                        continue
-                    time.sleep(0.5)
-                self.del_process(name)
-        
-        if self._exit and all_closed:
-            logger2.info('All subprocesses successfully closed. Exiting main.')
-            raise QuitException
-        elif self._exit and time.time() - self._exit > self.main_termination_time:
-            logger2.error('Some processes could not be closed. Exiting main.')
-            raise QuitException
-    
-    
-    def exit(self, *args):
-        if self._exit:
-            logger2.error('Exit has already been scheduled.')
-            return
-        for n,d in self._processes.items():
-            if not d: continue
-            self.stop_process(n)
-        self._exit = time.time()
-    
-    
-    def start(self):
-        buttons = [
-            # ['restart', {'text': '|', 'command': self.restart_process}],
-            ['stop', {'text': 'OFF', 'command': self.stop_process}],
-            ['start', {'text': 'ON', 'command': self.start_process}],
-            ['exit', {'text': 'EXIT', 'command': self.exit}],
-        ]
-        if self.rreload_button:
-            buttons.insert(2, ['start-rl', {'text': 'ON-rl', 'command': self.start_rl}])
-        
-        config = {
-            'title': self.title,
-            'tabs': ['MainProcess'] + list(self.processes),
-            #'tabs': ['debug*','MainProcess'] + list(self.processes),
-            'buttons': OrderedDict(buttons),
-            'entries': OrderedDict([
-                ['argv', {'label': 'argv'}], #'width': 10
-            ]),
-        }
-        
-        self._gui_thread = TkThread(config, daemon=True)
-        _started = time.time()
-        while getattr(self._gui_thread, 'gui', None) is None and time.time() - _started < 5: # wait till _gui_thread starts
-            time.sleep(0.05)
-        self._gui = self._gui_thread.gui
-        self._nb = self._gui_thread.gui.nb
-        if self.settings_path:
-            try: self.update_settings(True)
-            except FileNotFoundError:
-                with open(self.settings_path, 'w', encoding='utf-8') as f:
-                    json.dump(self.cfg, f)
-        
-        standard_logging(dir=self.logging_dir, f_ending=self.title, dpath=self.dpath)
-        start_by_default = [name for name, specs in self.processes.items() if specs.get('start')]
-        
-        for p in self.processes:
-            self._gui.root.after(1, self._gui.add_new_tab, p)
-        time.sleep(0.2)
-        
-        for name in start_by_default:
-            self.start_process(name)
-        
-        if self.settings_path:
-            self._cfg_updater = Ticker(self.update_settings, lambda: self.cfg['__meta__'].get('interval', 1),
-                                       args=(True,), keepalive={'pause': 30}, name='MainProcess-cfgUpdater')
-            self._cfg_updater.start_thread()
-        
-        self._response_waiter = Ticker(self._wait_on_responses, 1, name='ProcessListener')
-        self._response_waiter.loop()
-        if self._cfg_updater:
-            self._cfg_updater.close()
-        logger2.info('Closing Tkinter window.')
-        self._gui_thread.gui.root.quit()
-        #log.gui.root.destroy()
-        time.sleep(1.5)
-        logger2.info('`{}` terminated'.format(self.title))
+"""
+Make sure you have tkinter installed before using the features of this module.
+`sudo apt-get install python3-tk`
+"""
+import json
+from copy import deepcopy
+from collections import OrderedDict
+import multiprocessing
+import time
+import sys
+import shlex
+
+from fons.dict_ops import deep_update
+from fons.errors import QuitException
+from fons.io import update_settings, _META_NORM
+from fons.log import get_standard_5, init_tab, standard_logging
+from fons.processes import TkLogiProcess
+from fons.py import rreload
+from fons.sched import Ticker
+from fons.threads import EliThread
+
+
+NON_RESPONSIVE = ("debug*", "info*", "warning*", "error*", "critical*", "main")
+RRELOAD_BUTTON = False
+
+logger, logger2, tlogger, tloggers, tlogger0 = get_standard_5(__name__)
+
+
+def get_default_CFG(processes, dtypes=None):
+    _process = {
+        "_type_": dict,
+        "default_dtype": None,
+        "dtypes": {
+            "target": {"_type_": str},
+            "args": list,
+            "kwargs": dict,
+            "argv": {"_type_": (str, list), "_defval_": None},
+            "conn": bool,
+            "start": bool,
+        },
+    }
+    if dtypes is None:
+        dtypes = {}
+    return {
+        "_type_": dict,
+        "default_dtype": None,
+        "dtypes": {
+            "processes": {
+                "_type_": dict,
+                # 'keys': list(processes),
+                "unit": _process,
+            },
+            "__meta__": deepcopy(_META_NORM),
+            **dtypes,
+        },
+    }
+
+
+class NbGUI:
+    """Notebook styled gui"""
+
+    def __init__(self, config={}):
+        import tkinter as tk
+        import tkinter.ttk as ttk
+
+        self.root = tk.Tk()
+        self.root.geometry("975x475")
+        # self.root.resizable(0, 0)
+
+        if config.get("title") is not None:
+            self.root.title(config["title"])
+
+        left_frame = tk.Frame(self.root)
+        left_frame.pack(side=tk.LEFT)
+        buttons_frame = tk.Frame(left_frame)
+        buttons_frame.pack()
+        entries_frame = tk.Frame(left_frame)
+        entries_frame.pack(pady=(10, 0))
+
+        self.nb = ttk.Notebook(self.root)
+        # self.nb.grid(row=1, column=0, columnspan=50, rowspan=49, sticky='NESW')
+        # self.nb.pack_propagate(0)
+        self.nb.pack(side=tk.LEFT, fill="both", expand=True)
+
+        self.tabs = []
+        self.tab_selected = None
+        self.variables = {}
+        self.values = {}  # by (tab_name, var_name)
+        self.default_values = {}  # by var_name
+
+        buttons = config.get("buttons")
+        if buttons is None:
+            buttons = {}
+        for button_name, specs in buttons.items():
+            callback = (
+                self.wrap_button(specs["command"]) if specs.get("command") else None
+            )
+            text = specs.get("text")
+            b = tk.Button(buttons_frame, text=text, command=callback)
+            b.pack()
+
+        entries = config.get("entries")
+        if entries is None:
+            entries = {}
+        for var_name, specs in entries.items():
+            label = specs.get("label")
+            width = specs["width"] if specs.get("width") else 12
+            self.default_values[var_name] = value = (
+                specs["value"] if specs.get("value") else ""
+            )
+            ef = tk.Frame(entries_frame)
+            ef.pack()
+            if label:
+                tk.Label(ef, text=label).pack(side=tk.LEFT)
+            self.variables[var_name] = var = tk.StringVar(value=value)
+            tk.Entry(ef, textvariable=var, width=width).pack(side=tk.LEFT)
+
+        tabs = _tabs = config.get("tabs")
+        if tabs is None:
+            tabs = {}
+        elif not isinstance(tabs, dict):
+            tabs = {}
+            for item in _tabs:
+                if isinstance(item, dict):
+                    tab_name, specs = item["text"], item
+                else:
+                    tab_name, specs = item, {}
+                tabs[tab_name] = specs
+
+        for tab_name, specs in tabs.items():
+            values = specs.get("values")  # by var_name
+            if values is None:
+                values = {}
+            elif isinstance(values, str):
+                values = dict.fromkeys(self.variables, values)
+            self.add_new_tab(tab_name, values)
+
+    def add_new_tab(self, tab, variable_values={}):
+        if tab in self.tabs:
+            return
+        self.tabs.append(tab)
+        init_tab(self.nb, tab)
+        for var_name in self.variables:
+            value = variable_values.get(tab)
+            if value is None:
+                value = self.default_values[var_name]
+            self.values[(tab, var_name)] = value
+
+    def refresh(self, recursive=False):
+        tab_selected = self.nb.tab(self.nb.select(), "text")
+        if self.tab_selected != tab_selected:
+            for var_name, variable in self.variables.items():
+                value = self.values.get((tab_selected, var_name))
+                if value is None:
+                    value = ""
+                variable.set(value)
+            self.tab_selected = tab_selected
+
+        for var_name, variable in self.variables.items():
+            self.values[(tab_selected, var_name)] = variable.get()
+
+        if recursive:
+            self.root.after(recursive, self.refresh, recursive)
+
+    def wrap_button(self, f):
+        def on_button(*args, **kw):
+            tab_selected = self.nb.tab(self.nb.select(), "text")
+            return f(tab_selected, *args, **kw)
+
+        return on_button
+
+
+class TkThread(EliThread):
+    def __init__(self, config, *args, **kw):
+        super().__init__(*args, **kw)
+        self.config = config
+        self.start()
+
+    def run(self):
+        """It is important that the gui is initiated inside the running thread"""
+        self.gui = NbGUI(self.config)
+        self.gui.refresh(recursive=300)
+        self.gui.root.mainloop()
+
+
+def ignore(f):
+    def check_ignore(*args, **kw):
+        try:
+            name = args[1]  # (0 = self)
+        except IndexError:
+            name = kw["name"]
+        if name not in NON_RESPONSIVE:
+            return f(*args, **kw)
+
+    return check_ignore
+
+
+class TkLogiProcessComplex:
+    def __init__(
+        self,
+        processes={},
+        *,
+        settings_path=None,
+        cfg=None,
+        CFG=None,
+        functions={},
+        title="TkLogiProcessComplex",
+        termination_time=60,
+        main_termination_time=75,
+        logging_dir=None,
+        dpath=None,
+        rreload_button=None
+    ):
+        """
+        :type processes: dict
+            {
+                process_name: {
+                    target: function,
+                    args: (...),
+                    kwargs: {...},
+                    argv: 'put something here',      # can also be list ['put', 'something', 'here']
+                    conn: <bool>,                    # if True then function must accept `conn` as keyword (Pipe)
+                    start: <bool>                    # whether or not it is started on .start
+                }
+            }
+        about function:
+            may accept `argv` as keyword, should default to sys.argv
+            may accept `conn` as keyword
+        about conn (Pipe):
+            assumed to expect `None` as a cue to end itself (the function)
+            assumed to send `None` back when done
+        :type cfg: dict
+            initial contents of the file located at `settings_path`
+            cfg['processes'] is used to periodically deep update `self.processes`
+            { processes: processes }                 # where processes are equivalent to `processes` argument
+        """
+        self.processes = dict(processes)
+        self.verify_processes(self.processes)
+        self.settings_path = settings_path
+        self.cfg = deepcopy(cfg) if cfg is not None else {}
+        self.CFG = deepcopy(CFG) if CFG is not None else {}
+        self.functions = dict(functions)
+        self.title = title
+        self.termination_time = termination_time
+        self.main_termination_time = main_termination_time
+        self.logging_dir = logging_dir
+        self.dpath = dpath
+        self.rreload_button = (
+            rreload_button if rreload_button is not None else RRELOAD_BUTTON
+        )
+
+        self.init_CFG()
+
+        self._processes = {}
+        self._exit = None
+        self._cfg_updater = None
+        self._gui_thread = None
+        self._gui = None
+        self._nb = None
+        self._response_waiter = None
+
+    @staticmethod
+    def verify_processes(processes):
+        for name in processes:
+            if name in ("MainProcess", "main"):
+                raise ValueError("Processname '{}' is not allowed".format(name))
+
+    def init_CFG(self):
+        self.CFG = deep_update(get_default_CFG(self.processes), self.CFG, copy=True)
+
+    def update_settings(self, add_new_process_tabs=False):
+        old_processes = self.cfg.get("processes", {})
+        c = self.cfg.get("__meta__", {}).get("counter", 0)
+        update_settings(self.settings_path, self.cfg, self.CFG)
+        c2 = self.cfg["__meta__"]["counter"]
+
+        if not c or c2 > c:
+            # update_settings doesn't deep_update automatically
+            self.cfg["processes"] = deep_update(
+                old_processes, self.cfg.get("processes", {})
+            )
+            cfg_processes = self.cfg["processes"]
+            if isinstance(cfg_processes, dict):
+                self.verify_processes(cfg_processes)
+                for p in cfg_processes:
+                    if p in self.processes:
+                        self.processes[p].update(cfg_processes[p])
+                    else:
+                        self.processes[p] = dict(cfg_processes[p])
+
+        if add_new_process_tabs:
+            for p in self.processes:
+                if p not in self._gui.tabs:
+                    self._gui.root.after(1, self._gui.add_new_tab, p)
+
+    def init_process(self, name):
+        specs = self.processes[name]
+        target = specs["target"]
+
+        if target is None:
+            target = name
+
+        if isinstance(target, str):
+            target = self.functions[target]
+
+        argv = self._gui.values.get((name, "argv"))
+        if not argv:
+            argv = specs.get("argv")
+
+        if argv is None:
+            pass
+        elif isinstance(argv, str):
+            argv = [""] + shlex.split(argv)
+        else:
+            argv = [""] + list(argv)
+
+        conn = multiprocessing.Pipe() if specs.get("conn") else None
+
+        args = tuple(specs["args"]) if specs.get("args") is not None else ()
+        kwargs = dict(specs["kwargs"]) if specs.get("kwargs") is not None else {}
+        if argv:
+            kwargs["argv"] = argv
+        if conn is not None:
+            kwargs["conn"] = conn[1]
+
+        p = TkLogiProcess(
+            self._nb,
+            target=target,
+            args=args,
+            kwargs=kwargs,
+            name=name,
+            daemon=specs.get("daemon", False),
+        )  # this should be False, as it may spawn children
+        self._processes[name] = {
+            "p": p,
+            "conn": conn,
+            "args": args,
+            "kwargs": kwargs,
+            "start": None,
+            "close": None,
+        }
+        return p
+
+    def del_process(self, name):
+        old = self._processes.get(name)
+        if not old:
+            return
+        conn = old["conn"]
+        if conn:
+            conn[0].close()
+            conn[1].close()
+        self._processes[name] = {}
+
+    def _check_is_not_running(self, name):
+        if not self._processes.get(name, {}).get("p"):
+            pass
+        elif self._processes[name]["p"].is_alive():
+            logger2.error("Cannot start `{}`: is already running".format(name))
+            return False
+        else:
+            self.del_process(name)
+        return True
+
+    @ignore
+    def start_process(self, name):
+        if not self._check_is_not_running(name):
+            return
+        p = self.init_process(name)
+        _p = self._processes[name]
+        args_sfx = " :: {}".format(_p["args"]) if _p["args"] else ""
+        kw_sfx = " :: {}".format(_p["kwargs"]) if _p["kwargs"] else ""
+        logger2.info("Starting `{}`{}{}".format(name, args_sfx, kw_sfx))
+        self._processes[name]["start"] = time.time()
+        p.start()
+        logger2.info("Starting of `{}` (pid: {}) successful".format(name, p.pid))
+
+    @ignore
+    def start_rl(self, name):
+        if not self._check_is_not_running(name):
+            return
+        logger2.info("Attempting to reload `{}` modules".format(name))
+        f = f0 = self.processes[name].get("target")
+        if f is None:
+            f = f0 = name
+        if isinstance(f, str):
+            f = self.functions[f]
+        module = sys.modules[f.__module__]
+        rreload(module)
+        f = getattr(module, f.__name__)
+        if isinstance(f0, str):
+            self.functions[f0] = f
+        else:
+            self.processes[name]["target"] = f
+        self.start_process(name)
+
+    @ignore
+    def restart_process(self, name):
+        logger2.info("Attempting to restart `{}`".format(name))
+        self.stop_process(name)
+        self.start_process(name)
+
+    @ignore
+    def stop_process(self, name):
+        try:
+            p = self._processes[name]["p"]
+        except KeyError:
+            logger2.error("Cannot stop `{}`: has not been initiated".format(name))
+            return
+        if self._processes[name]["close"]:
+            logger2.error("`{}` is already waiting for termination.".format(name))
+            return
+        if not p.is_alive():
+            logger2.error("Cannot stop `{}`: is not running".format(name))
+            return
+        logger2.info("Scheduling `{}` for termination".format(name))
+        self._processes[name]["close"] = time.time()
+        conn = self._processes[name]["conn"]
+        if conn:
+            conn[0].send(None)
+        else:
+            self.force_terminate_process(name)
+
+    def force_terminate_process(self, name):
+        p = self._processes[name]["p"]
+        logger2.info("Force terminating `{}`".format(name))
+        p.terminate()
+        self.del_process(name)
+
+    def _wait_on_responses(self):
+        all_closed = True
+        for name, d in self._processes.copy().items():
+            p = d.get("p")
+            conn = d.get("conn")
+            start = d.get("start")
+            close = d.get("close")
+            updated = conn and conn[0].poll(0.01)
+            if not updated:
+                if not start or time.time() - start < 2:
+                    pass
+                elif not p.is_alive():
+                    logger2.info("`{}` has terminated.".format(name))
+                    self.del_process(name)
+                elif close and time.time() - close > self.termination_time:
+                    logger2.info(
+                        "`{}` has exceeded its allocated termination time. Force terminating.".format(
+                            name
+                        )
+                    )
+                    self.force_terminate_process(name)
+                else:
+                    all_closed = False
+                continue
+
+            r = conn[0].recv()
+            logger2.info("Received from {}'s conn: {}".format(name, r))
+            if r is None:
+                logger2.info(
+                    "Process `{}` has successfully terminated itself.".format(name)
+                )
+                time.sleep(1)
+                if p.is_alive():
+                    logger2.error(
+                        "But `{}` is till alive. Attempting force termination.".format(
+                            name
+                        )
+                    )
+                    try:
+                        self.force_terminate_process(name)
+                    except Exception as e:
+                        logger2.exception(e)
+                        all_closed = False
+                        continue
+                    time.sleep(0.5)
+                self.del_process(name)
+
+        if self._exit and all_closed:
+            logger2.info("All subprocesses successfully closed. Exiting main.")
+            raise QuitException
+        elif self._exit and time.time() - self._exit > self.main_termination_time:
+            logger2.error("Some processes could not be closed. Exiting main.")
+            raise QuitException
+
+    def exit(self, *args):
+        if self._exit:
+            logger2.error("Exit has already been scheduled.")
+            return
+        for n, d in self._processes.items():
+            if not d:
+                continue
+            self.stop_process(n)
+        self._exit = time.time()
+
+    def start(self):
+        buttons = [
+            # ['restart', {'text': '|', 'command': self.restart_process}],
+            ["stop", {"text": "OFF", "command": self.stop_process}],
+            ["start", {"text": "ON", "command": self.start_process}],
+            ["exit", {"text": "EXIT", "command": self.exit}],
+        ]
+        if self.rreload_button:
+            buttons.insert(2, ["start-rl", {"text": "ON-rl", "command": self.start_rl}])
+
+        config = {
+            "title": self.title,
+            "tabs": ["MainProcess"] + list(self.processes),
+            #'tabs': ['debug*','MainProcess'] + list(self.processes),
+            "buttons": OrderedDict(buttons),
+            "entries": OrderedDict(
+                [
+                    ["argv", {"label": "argv"}],  #'width': 10
+                ]
+            ),
+        }
+
+        self._gui_thread = TkThread(config, daemon=True)
+        _started = time.time()
+        while (
+            getattr(self._gui_thread, "gui", None) is None
+            and time.time() - _started < 5
+        ):  # wait till _gui_thread starts
+            time.sleep(0.05)
+        self._gui = self._gui_thread.gui
+        self._nb = self._gui_thread.gui.nb
+        if self.settings_path:
+            try:
+                self.update_settings(True)
+            except FileNotFoundError:
+                with open(self.settings_path, "w", encoding="utf-8") as f:
+                    json.dump(self.cfg, f)
+
+        standard_logging(dir=self.logging_dir, f_ending=self.title, dpath=self.dpath)
+        start_by_default = [
+            name for name, specs in self.processes.items() if specs.get("start")
+        ]
+
+        for p in self.processes:
+            self._gui.root.after(1, self._gui.add_new_tab, p)
+        time.sleep(0.2)
+
+        for name in start_by_default:
+            self.start_process(name)
+
+        if self.settings_path:
+            self._cfg_updater = Ticker(
+                self.update_settings,
+                lambda: self.cfg["__meta__"].get("interval", 1),
+                args=(True,),
+                keepalive={"pause": 30},
+                name="MainProcess-cfgUpdater",
+            )
+            self._cfg_updater.start_thread()
+
+        self._response_waiter = Ticker(
+            self._wait_on_responses, 1, name="ProcessListener"
+        )
+        self._response_waiter.loop()
+        if self._cfg_updater:
+            self._cfg_updater.close()
+        logger2.info("Closing Tkinter window.")
+        self._gui_thread.gui.root.quit()
+        # log.gui.root.destroy()
+        time.sleep(1.5)
+        logger2.info("`{}` terminated".format(self.title))
```

### Comparing `fons-0.3.1/fons/host.py` & `fons-0.4.0/fons/host.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,95 +1,116 @@
-import inspect
-
-from fons.errors import ServerError
-import fons.log as _log
-from fons.reg import create_name
-from fons.threads import EliThread
-from fons.verify import verify_data
-
-logger,logger2,tlogger,tloggers,tlogger0 = _log.get_standard_5(__name__)
-
-_SERVER_NAMES = set()
-
-
-class Server(EliThread):
-    def __init__(self, conn, on_success=None, on_exit=None, exit_cmd=None,
-                 verify=None, *, wait=1, name=None, log_error=True, **kw):
-        super().__init__(**kw)
-        self.conn = conn
-        self.verify = verify
-        self.wait = wait
-        self._log_error = log_error
-        
-        self._on_success = on_success
-        self._on_exit = on_exit
-        self._exit_cmd = (lambda x: False) if exit_cmd is None else exit_cmd
-        
-        if name is None and hasattr(self.__class__,'_name'):
-            name = self.__class__._name
-        self._name = create_name(name, default=self.__class__.__name__, registry=_SERVER_NAMES)
-        self._closed = False
-        
-    def run(self):
-        try:
-            while not self._closed:
-                if self.conn.poll(self.wait):
-                    r = self.conn.recv()
-                    if self._exit_cmd(r):
-                        logger.debug('{} - received exit command.'.format(self.name))
-                        self.close()
-                        break
-                    self.handle(r)
-        finally:
-            logger.debug('Closing {}'.format(self.name))
-            self.on_exit()
-                
-                
-    def handle(self, inp):
-        error_msg = self.verify_input(inp)
-        if error_msg:
-            self.send_error(error_msg)
-        else:
-            try: self.on_success(inp)
-            except ServerError as e:
-                self.send_error(e.msg)
-            except Exception as e:
-                logger.exception(e)
-                self.send_error(str(e))
-        
-    def send(self, data, ok=True, msg=None):
-        self.conn.send({'ok': ok, 'msg': msg, 'data': data})
-        
-    def send_error(self, msg):
-        if self._log_error:
-            logger.error(msg)
-        self.send({},ok=False,msg=msg)
-        
-    def on_success(self, inp):
-        self._on_success(inp)
-        
-    def on_exit(self):
-        if self._on_exit is not None:
-            fas = inspect.getfullargspec(self._on_exit)
-            ismethod = inspect.ismethod(self._on_exit) #note: ismethod returns True for classmethods also
-            args = (self.conn,) if len(fas.args[(1 if ismethod else 0):]) or fas.varargs else tuple()
-            self._on_exit(*args)
-        else:
-            self.conn.send(None)
-        
-    def verify_input(self, inp):
-        if self.verify is not None:
-            try: verify_data(inp,self.verify)
-            except Exception as e:
-                return 'Incorrect input: {}'.format(e)
-    
-    def close(self):
-        self._closed = True
-        
-    @property
-    def name(self):
-        return self._name
-    @name.setter
-    def name(self,value):
-        self._name = value
-        
-    _name = None
+import inspect
+
+from fons.errors import ServerError
+import fons.log as _log
+from fons.reg import create_name
+from fons.threads import EliThread
+from fons.verify import verify_data
+
+logger, logger2, tlogger, tloggers, tlogger0 = _log.get_standard_5(__name__)
+
+_SERVER_NAMES = set()
+
+
+class Server(EliThread):
+    def __init__(
+        self,
+        conn,
+        on_success=None,
+        on_exit=None,
+        exit_cmd=None,
+        verify=None,
+        *,
+        wait=1,
+        name=None,
+        log_error=True,
+        **kw
+    ):
+        super().__init__(**kw)
+        self.conn = conn
+        self.verify = verify
+        self.wait = wait
+        self._log_error = log_error
+
+        self._on_success = on_success
+        self._on_exit = on_exit
+        self._exit_cmd = (lambda x: False) if exit_cmd is None else exit_cmd
+
+        if name is None and hasattr(self.__class__, "_name"):
+            name = self.__class__._name
+        self._name = create_name(
+            name, default=self.__class__.__name__, registry=_SERVER_NAMES
+        )
+        self._closed = False
+
+    def run(self):
+        try:
+            while not self._closed:
+                if self.conn.poll(self.wait):
+                    r = self.conn.recv()
+                    if self._exit_cmd(r):
+                        logger.debug("{} - received exit command.".format(self.name))
+                        self.close()
+                        break
+                    self.handle(r)
+        finally:
+            logger.debug("Closing {}".format(self.name))
+            self.on_exit()
+
+    def handle(self, inp):
+        error_msg = self.verify_input(inp)
+        if error_msg:
+            self.send_error(error_msg)
+        else:
+            try:
+                self.on_success(inp)
+            except ServerError as e:
+                self.send_error(e.msg)
+            except Exception as e:
+                logger.exception(e)
+                self.send_error(str(e))
+
+    def send(self, data, ok=True, msg=None):
+        self.conn.send({"ok": ok, "msg": msg, "data": data})
+
+    def send_error(self, msg):
+        if self._log_error:
+            logger.error(msg)
+        self.send({}, ok=False, msg=msg)
+
+    def on_success(self, inp):
+        self._on_success(inp)
+
+    def on_exit(self):
+        if self._on_exit is not None:
+            fas = inspect.getfullargspec(self._on_exit)
+            ismethod = inspect.ismethod(
+                self._on_exit
+            )  # note: ismethod returns True for classmethods also
+            args = (
+                (self.conn,)
+                if len(fas.args[(1 if ismethod else 0) :]) or fas.varargs
+                else tuple()
+            )
+            self._on_exit(*args)
+        else:
+            self.conn.send(None)
+
+    def verify_input(self, inp):
+        if self.verify is not None:
+            try:
+                verify_data(inp, self.verify)
+            except Exception as e:
+                return "Incorrect input: {}".format(e)
+
+    def close(self):
+        self._closed = True
+
+    @property
+    def name(self):
+        return self._name
+
+    @name.setter
+    def name(self, value):
+        self._name = value
+
+    _name = None
```

### Comparing `fons-0.3.1/fons/io.py` & `fons-0.4.0/fons/io.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,681 +1,746 @@
-import os
-from collections import OrderedDict
-import json
-import functools
-import warnings
-import filelock
-import yaml
-import copy as _copy
-import pytz
-import datetime
-from _hashlib import new
-dt = datetime.datetime
-td = datetime.timedelta
-
-from fons.dict_ops import (deep_update, deep_get)
-from fons.iter import unique
-from fons.verify import init_data, normalize, _isnorm, verify_data
-import fons.log as _log
-
-logger,logger2,tlogger,tloggers,tlogger0 = _log.get_standard_5(__name__)
-
-_META_NORM = {
-    '_type_':dict,
-    'default_dtype': None,
-    'dtypes': {
-        'interval': float,
-        '1st_only': {
-            '_type_': list,
-            'unit': {'_type_': str}},
-        'null_overwrite': bool,
-        'init': bool,
-        'deep': bool,
-        'borrow_keys': bool,
-        'borrow_meta': bool,
-        
-        'counter': int,
-        'config': str,
-        'exclude': {
-            '_type_': list,
-            'unit': {'_type_': str}},
-        'last_input': dict,
-        'last_input_meta': dict,
-        'last_modified': {
-            '_type_': dict,
-            'unit': {'_type_': float}},
-    }
-}
-
-_CFG_DTYPES = {
-    '__meta__': _META_NORM,
-}
-normalize(_META_NORM)
-
-
-class DateTimeEncoder(json.JSONEncoder):
-    def default(self, o):
-        if isinstance(o, dt):
-            #return o.isoformat()
-            #"values": [o.year,o.month,o.day,o.hour,o.minute,o.second,o.microsecond]}
-            return {'_type_': 'dt',
-                    'v': o.isoformat()}
-             
-        elif isinstance(o,td):
-            return {'_type_': 'td',
-                    'v': [o.days,o.seconds,o.microseconds]}
-        
-        else: return json.JSONEncoder.default(self, o)
-        
-        
-class DateTimeEncoderNumeric(json.JSONEncoder):
-    def default(self, o):
-        if isinstance(o, dt):
-            #return o.isoformat()
-            #"values": [o.year,o.month,o.day,o.hour,o.minute,o.second,o.microsecond]}
-            if o.tzinfo is None:
-                o = o.replace(tzinfo=pytz.utc)
-                
-            v = dt.timestamp(o) * 1000
-            v = max(int(v), v)
-                
-            return {'_type_': 'dt',
-                    'v': v}
-             
-        elif isinstance(o,td):
-            v = o.total_seconds() * 1000
-            v = max(int(v), v)
-
-            return {'_type_': 'td',
-                    'v': v}
-        
-        else: return json.JSONEncoder.default(self, o)
-    
-    
-def _extract_literal(s):
-    j1 = s.find("<")
-    j2 = s.rfind(">")
-    
-    if j1 == 0 and j2 == len(s)-1:
-        return json.loads(s[j1+1:j2].strip())
-    
-    return s
-    
-    
-def _get_key_value(line):
-    i1 = line.find("[")
-    i2 = line.find("]")
-    
-    if i1 != 0 or i2 == -1:
-        raise ValueError(line)
-    
-    key = line[i1+1:i2].strip()
-    value = line[i2+1:].strip()
-
-    key = _extract_literal(key)
-    #value = json.loads(value)
-      
-    return key,value
-
-
-def get_params(text, keys=[], sep='\n', ordered=False, **kw):
-    """A custom json-like file format for dicts, which supports non-str keys.
-       Example:
-        [param_name] "json value"
-        [<2>] null
-        [<"<2>">] null
-        //comment line 
-         -> {"param_name": "json value", 2: None, "<2>": None}
-      If param_name is surrouned with <>, it is assumed to be json value,
-      otherwise it is interpreted as string."""
-    lines0 = [x.strip() for x in text.split(sep)]
-
-    D = dict() if not ordered else OrderedDict()
-    
-    return_nrs_n_lines = kw.get('return_nrs_n_lines')
-    line_nrs = OrderedDict()
-    init = kw.get('init')
-    missing = kw.get('missing','raise')
-    
-    if keys is not None and len(keys):
-        do_keys, unseen = True, set(keys)
-    else: 
-        do_keys = unseen = None
-    
-    for line_nr,line in enumerate(lines0):
-        if not len(line) or line[:2] == '//':
-            continue
-        
-        try:
-            k,v = _get_key_value(line)
-        except ValueError:
-            warnings.warn('Damaged line ({line_nr}): "{line}"' \
-                          .format(line_nr=line_nr, line=line))
-            continue
-        
-        if do_keys:
-            if k not in keys: continue
-            try: unseen.remove(k)
-            except KeyError: pass
-        
-        v_json = json.loads(v)
-        D[k] = v_json if not init else init_data(v_json)
-        line_nrs[k] = line_nr
-        
-    
-    if do_keys and len(unseen) and missing=='raise':
-        raise KeyError('Missing Keys: {}'.format(list(unseen)))
-        
-    if return_nrs_n_lines:
-        return D, line_nrs, lines0
-    
-    return D
-
-
-def read_params(path, keys=None, ordered=False, update=None, **kw):
-    """Read params from file. 
-       If `keys` is given, only those key-values are returned
-       (if a key is missing then KeyError is raised)."""
-    encoding = kw.get('encoding')
-    if encoding is None: encoding = 'utf-8'
-    
-    with open(path,encoding=encoding) as f:
-        text = f.read()
-    
-    item = get_params(text, keys=keys, ordered=ordered, **kw)
-    
-        
-    if isinstance(update,dict):
-        if kw.get('read_nrs_n_lines'):
-            update.update(item[0])
-        else: update.update(item)
-    
-    return item
-
-
-def save_params(path, D, *, read_path=None, mode='a', **kw):
-    """Save params to a file, while retaining file's previous params and comments.
-       :param read_path: if given, previous params are read from that file
-                         (instead of the file to be overwritten, if exists)
-       :param mode: 'a' -> "append" new params to previous ones found in the file
-                    'w' -> overwrite the file, disregarding its previous content"""
-    line_nrs = {}
-    lines = []
-    
-    cls = kw.get('cls')
-    if cls is None: cls = DateTimeEncoder
-    elif cls == 'DateTimeEncoder': cls = DateTimeEncoder
-    elif cls == 'DateTimeEncoderNumeric': cls = DateTimeEncoderNumeric
-    elif isinstance(cls,str):
-        raise ValueError('Unknown cls: {}'.format(cls))
-    
-    deep = kw.get('deep')
-    init = kw.get('init',True)
-    read_path = path if read_path is None else read_path
-    
-    if os.path.isfile(read_path) and mode in ('a', None):
-        #Note that `D2` and `line_nrs` contain only the requested keys (D.keys()) and their line nrs,
-        # while `lines` contains all lines (in str format) in the file
-        D2, line_nrs, lines = read_params(read_path, list(D.keys()), ordered=True,
-                                          return_nrs_n_lines=True, init=init, missing='ignore')
-        D2.update(D) if not deep else deep_update(D2,D)
-        D = D2
-    
-    
-    llen = len(lines)
-    
-    for k,v in D.items():
-        if isinstance(k, str):
-            k_final = k if not (k.startswith('<') and k.endswith('>')) else '<"{}">'.format(k)
-        else:
-            k_final = '<{}>'.format(k)
-        
-        line = '[{}] {}'.format(k_final, json.dumps(v,cls=cls))
-        
-        line_nr = line_nrs.get(k)
-        
-        if line_nr is not None:
-            lines[line_nr] = line
-        else:
-            lines.append(line)
-    
-    if len(lines) > llen and lines[llen-1][:2] == '//':
-        lines.insert(llen,'')
-        
-    if kw.get('comments'):
-        lines += ['//'+c for c in kw['comments']]
-    
-    encoding = kw.get('encoding')
-    if encoding is None:
-        encoding = 'utf-8'
-    
-    write_txt = '\n'.join(lines)
-    
-    with open(path, 'w', encoding=encoding) as f:
-        f.write(write_txt)
-
-
-class SafeFileLock(filelock.FileLock):
-    def __init__(self, filepath, timeout=-1, poll_interval=0.02, log=True):
-        """NB! '.lock' will be added to filepath"""
-        lock_file = filepath + '.lock'
-        self._poll_interval_given = poll_interval
-        self._log_given = log
-        super().__init__(lock_file, timeout)
-        
-    def acquire(self, timeout=None, poll_interval=None, log=None):
-        if poll_interval is None:
-            poll_interval = self._poll_interval_given
-        if log is None:
-            log = self._log_given
-        
-        try: return super().acquire(timeout,poll_interval)
-        except filelock.Timeout as e:
-            if log: logger.error(e)
-            class ReturnProxy(object):
-                def __init__(self, lock):
-                    self.lock = lock
-                    return None
-                def __enter__(self):
-                    return self.lock
-                def __exit__(self, exc_type, exc_value, traceback):
-                    self.lock.release()
-                    return None
-            return ReturnProxy(lock = self)
-
-
-def wait_filelock(filepath, timeout=0.2, poll_interval=0.02, log=False):
-    with SafeFileLock(filepath,timeout,poll_interval,log):
-        pass
-
-
-#-------------------------------
-
-def _get_force_update(paths, meta, counter, force_update):
-    if not counter or force_update:
-        return True
-    
-    lm = meta['last_modified']
-    
-    #if user decided to change the path of a file
-    if any(p not in lm for p in paths):
-        return True
-        
-    for path,time in lm.items():
-        cur_last_modified = os.path.getmtime(path)
-        if time != cur_last_modified:
-            return True
-    
-    return False
-    
-    
-def _load_settings(path, ftype, create, meta, force_update, return2):
-    if ftype is None:
-        loc = path.rfind('.')
-        if loc != -1:
-            ftype = path[loc+1:].lower()
-    else: ftype = ftype.lower()
-    
-    if os.path.exists(path): pass
-    elif create:
-        with open(path,'w') as f:
-            f.write('')
-    else:
-        raise FileNotFoundError(path)
-    
-    last_modified = os.path.getmtime(path)
-    
-    if not force_update:
-        return return2
-    
-    meta['last_modified'][path] = last_modified
-    
-    if ftype in ('yaml','yml'):
-        with open(path, encoding='utf-8') as f:
-            new = yaml.safe_load(f) or {}
-    elif ftype == 'json':
-        with open(path, encoding='utf-8') as f:
-            new = json.load(f) or {}
-    else:
-        new = read_params(path)
-    #else: raise ValueError('Unknown ftype: {}'.format(ftype))
-    
-    return new
-
-
-def _verify_is_dict(x, param, raise_errors):
-    is_dict = isinstance(x, dict)
-    
-    if not is_dict:
-        msg = '{param} must be dict; got: {type}'.format(param=param, type=type(x).__name__)
-        _handle_error(TypeError(msg), False, None, msg, raise_errors=raise_errors)
-    
-    return is_dict
-
-
-def _handle_error(e, log_as_exception, txt=None, txt2=None, raise_errors=False):
-    if txt:
-        logger2.error(txt)
-    if raise_errors:
-        raise e
-    if txt2:
-        logger2.error(txt)
-    if log_as_exception:
-        logger.exception(e)
-
-
-def _get_param(meta, key, value):
-    if value is None:
-        value = meta.get(key)
-    
-    return value
-
-
-def _get_exclude(meta, new, counter, exclude):
-    if not counter:
-        if exclude is None:
-            exclude = new.get('__exclude__')
-    else:
-        if exclude is not None and exclude != meta.get('exclude'):
-            warnings.warn("`exclude` can't be changed when counter > 0")
-        exclude = meta.get('exclude')
-
-    if exclude is None:
-        exclude = []
-            
-    if not hasattr(exclude, '__getitem__'):
-        raise TypeError('`exclude` must be listlike, got: {}'.format(type(exclude)))
-        
-    meta['exclude'] = exclude
-    
-    return exclude
-    
-
-def _get_config(meta, new, counter, config=None, default=None):
-    if not counter:
-        if default is None:
-            default = new.get('__default__')
-        meta['default'] = default
-    else:
-        if default is not None and default != meta.get('default'):
-            warnings.warn("`default` can't be changed when counter > 0")
-        default = meta.get('default')
-        
-    if not counter:
-        if config is None:
-            config = new.get('__config__')
-        if config is None:
-            config = default
-        meta['config'] = config
-    else:
-        if config is not None and config != meta.get('config'):
-            warnings.warn("`config` can't be changed when counter > 0")
-        config = meta.get('config')
-    
-    return config, default
-
-
-def _get_config_dict(new, config, main_path, _load_args, *vid_args):
-    if config is None:
-        config_dict = new
-    elif config not in new:
-        raise KeyError('config: "{}" is not defined'.format(config))
-    else:
-        config_dict = new[config]
-        
-    if isinstance(config_dict, str):
-        path = path0 = config_dict
-        ftype = None
-        
-        if '|' in path:
-            path, ftype = path.split('|')
-            
-        if ':' not in path:
-            if main_path is None:
-                msg = ("Config '{}' path is relative but the main file's path "
-                       "isn't specified; got: \"{}\"").format(config, path0)
-                raise ValueError(msg)
-            
-            main_path_dir = os.path.dirname(os.path.realpath(main_path))
-            relative_path = path.strip('/').strip('\\')
-            path = os.path.join(main_path_dir, relative_path)
-            
-        config_dict = _load_settings(path, ftype, *_load_args)
-        
-    _verify_is_dict(config_dict, 'config:{}'.format(config), *vid_args)
-    
-    if config_dict is None:
-        config_dict = {}
-        
-    return config_dict
-    
-    
-def _get_meta(old, *args):
-    meta = old.get('__meta__')
-    if meta is None:
-        old['__meta__'] = meta = {}
-
-    if not _verify_is_dict(meta, '__meta__', *args):
-        meta = {}
-    
-    for k,defval in [['counter',0],
-                     ['last_modified',{}],
-                     ['last_input',{}],
-                     ['last_input_meta',{}]]:
-        if meta.get(k) is None:
-            meta[k] = defval
-        
-    return meta
-        
-        
-def _update_meta(meta, config_dict, default_dict, logging_level, raise_errors):
-    
-    def _notify(k, v):
-        logger2.log(logging_level, 'Setting __meta__ param "{}" to `{}`'.format(k,v))
-        
-    meta_default = default_dict.get('__meta__')
-    meta_config = config_dict.get('__meta__')
-        
-    if meta_config is None or not _verify_is_dict(meta_config, 'meta_config', raise_errors):
-        meta_config = {}
-        
-    if meta_default is None or not _verify_is_dict(meta_default, 'meta_default', raise_errors):
-        meta_default = {}
-    
-    #`borrow_keys` and `borrow_meta` themselves are always "borrowed"
-    borrow_keys = deep_get([meta_config, meta_default], 'borrow_keys')
-    borrow_meta = deep_get([meta_config, meta_default], 'borrow_meta')
-    if borrow_meta is None:
-        borrow_meta = borrow_keys
-    
-    for k,v in [['borrow_keys', borrow_keys],
-                ['borrow_meta', borrow_meta]]:
-        if v != meta.get(v):
-            _notify(k,v)
-        meta[k] = v
-            
-    lim = meta['last_input_meta']
-        
-    meta_defvals = {'1st_only': [], 'null_overwrite': True,
-                    'interval': 15, 'init': False, 'deep': None}
-    
-    def _update_value(k, *v):
-        if not v:
-            v = meta_config.get(k)
-            if v is None and borrow_meta:
-                v = meta_default.get(k)
-        else:
-            v = v[0]
-            
-        if k in lim and lim[k] == v:
-            return
-        
-        lim[k] = _copy.deepcopy(v)
-        
-        if v is not None:
-            norm = next(x[1] for x in _META_NORM['items'] if x[0]==k)
-            try: 
-                verify_data(v, norm, missing='ignore', extra='error') #??
-            except Exception as e:
-                logger2.error('__meta__ param "{}" incorrectly formatted.'.format(k))
-                if raise_errors:
-                    raise e
-                logger2.error(e)
-                #raise e
-                v = None
-                
-        if v is None:
-            v = meta_defvals.get(k)
-        
-        _notify(k,v)
-        meta[k] = v
-        
-
-    for k in meta_defvals:
-        _update_value(k)
-        
-
-def _update_keys(meta, old, config_dict, default_dict, counter, 
-                 config, default, exclude, init, verify, v_params,
-                 raise_errors):
-    
-    _handle = functools.partial(_handle_error, raise_errors=raise_errors)
-
-    last_input = meta['last_input']
-    first_only = meta['1st_only'], 
-    null_overwrite = meta['null_overwrite']    
-    borrow_keys = meta['borrow_keys']
-    
-    skip = ['__meta__'] + exclude
-    if default is None:
-        skip += ['__config__','__default__','__exclude__']
-        if config is not None:
-            skip += [config]
-            
-    if not borrow_keys:
-        skip += [k for k in default_dict if k not in config_dict]
-
-    all_keys = list(unique(list(config_dict.keys()) + list(default_dict.keys())))
-    selected_keys = list(filter(lambda x: x not in skip, all_keys))
-    
-    if verify is not None and not _isnorm(verify):
-        verify = normalize(verify)
-        
-    if v_params is None: v_params = {}
-    v_params = dict({'missing': 'ignore', 'extra': 'error'}, **v_params) #??
-    
-    new_dict = {}
-    new_last_input = {}
-    exc = None
-    
-    for k in selected_keys:
-        if counter and k in first_only:
-            continue
-        
-        if k in config_dict or not borrow_keys:
-            new_val = config_dict[k]
-        else: 
-            new_val = default_dict.get(k)
-
-        if new_val is None and k in old and not null_overwrite: continue
-        elif k in last_input and new_val == last_input[k]: continue
-        
-        new_last_input[k] = _copy.deepcopy(new_val)
-        
-        if init:
-            try: new_val = init_data(new_val)
-            except Exception as e:
-                exc = e
-                _handle(exc, True, 'Could not initiate param "{}"'.format(k))
-                break
-        
-        if verify is not None:
-            try: norm = next(x[1] for x in verify['items'] if x[0]==k)
-            except StopIteration as e:
-                exc = KeyError('Unknown param: {}'.format(k))
-                _handle(exc, False, None, 'Unknown param: {}'.format(k))
-                break
-
-            try: verify_data(new_val, norm, **v_params)
-            except Exception as e:
-                exc = e
-                _handle(exc, True, 'Param "{}" incorrectly formatted.'.format(k))
-                break
-            
-        new_dict[k] = new_val
-        
-    return new_dict, new_last_input, exc
-        
-
-def update_settings(new, old=None, verify=None,*, ftype=None,
-                    deep=None, init=False, logging_level='INFO',
-                    create=False, v_params=None, force_update=False,
-                    errors='raise', config=None, default=None, exclude=None):
-    """Update a dict with new values.
-       :param new: dict or path to a file (containing dict)
-       :param old: previous dict, meant to be reused on all calls
-       :param verify: the `norm` dict to be used to verify 
-       :param create: if True and a file doesn't exist, create an empty one;
-       '              otherwise raise FileNotFoundError
-       :param errors: 'ignore', 'raise', 'log' ('ignore' is logged too)
-    """
-    if errors not in ('ignore','raise','log'):
-        raise ValueError(errors)
-    logging_level = _log.level_to_int(logging_level)
-    raise_errors = (errors == 'raise')
-    vid_args = (raise_errors,)
-        
-    if old is None:
-        old = {}
-    
-    meta = _get_meta(old, *vid_args)
-    counter = meta['counter']
-    path = new if isinstance(new, str) else None
-    
-    force_update = _get_force_update([path], meta, counter, force_update)
-
-    if path is not None:
-        new = _load_settings(path, ftype, create, meta, force_update, old)
-        if new is old:
-            return old
-    
-    config, default = _get_config(meta, new, counter, config, default)
-    #print(config, default)
-    exclude = _get_exclude(meta, new, counter, exclude)
-
-    meta['counter'] += 1
-    
-    _load_args = (create, meta, True, {})
-    config_dict = _get_config_dict(new, config, path, _load_args, *vid_args)
-    
-    if config == default:
-        default_dict = config_dict
-    else:
-        default_dict = _get_config_dict(new, default, path, _load_args, *vid_args)
-
-    _update_meta(meta, config_dict, default_dict, logging_level, raise_errors)
-    
-    init = _get_param(meta, 'init', init)
-    deep = _get_param(meta, 'deep', deep)
-    
-    new_dict, new_last_input, exc = \
-                    _update_keys(meta, old, config_dict, default_dict, counter,
-                                 config, default, exclude, init, verify, v_params,
-                                 raise_errors)
-    
-    #We do not want to update only half the params (might cause a fiasco)
-    # either update all or reject and return the old
-    if exc is not None:
-        return old
-    
-    for k,new_val in new_dict.items():
-        logger2.log(logging_level, 'Setting param "{}" to `{}`'.format(k, new_val))
-    
-    if deep:
-        deep_update(old, new_dict)
-    else:
-        old.update(new_dict)
-        
-    meta['last_input'].update(new_last_input)
-    
-    return old
-
+import os
+from collections import OrderedDict
+import json
+import functools
+import warnings
+import filelock
+import yaml
+import copy as _copy
+import pytz
+import datetime
+from _hashlib import new
+
+dt = datetime.datetime
+td = datetime.timedelta
+
+from fons.dict_ops import deep_update, deep_get
+from fons.iter import unique
+from fons.verify import init_data, normalize, _isnorm, verify_data
+import fons.log as _log
+
+logger, logger2, tlogger, tloggers, tlogger0 = _log.get_standard_5(__name__)
+
+_META_NORM = {
+    "_type_": dict,
+    "default_dtype": None,
+    "dtypes": {
+        "interval": float,
+        "1st_only": {"_type_": list, "unit": {"_type_": str}},
+        "null_overwrite": bool,
+        "init": bool,
+        "deep": bool,
+        "borrow_keys": bool,
+        "borrow_meta": bool,
+        "counter": int,
+        "config": str,
+        "exclude": {"_type_": list, "unit": {"_type_": str}},
+        "last_input": dict,
+        "last_input_meta": dict,
+        "last_modified": {"_type_": dict, "unit": {"_type_": float}},
+    },
+}
+
+_CFG_DTYPES = {
+    "__meta__": _META_NORM,
+}
+normalize(_META_NORM)
+
+
+class DateTimeEncoder(json.JSONEncoder):
+    def default(self, o):
+        if isinstance(o, dt):
+            # return o.isoformat()
+            # "values": [o.year,o.month,o.day,o.hour,o.minute,o.second,o.microsecond]}
+            return {"_type_": "dt", "v": o.isoformat()}
+
+        elif isinstance(o, td):
+            return {"_type_": "td", "v": [o.days, o.seconds, o.microseconds]}
+
+        else:
+            return json.JSONEncoder.default(self, o)
+
+
+class DateTimeEncoderNumeric(json.JSONEncoder):
+    def default(self, o):
+        if isinstance(o, dt):
+            # return o.isoformat()
+            # "values": [o.year,o.month,o.day,o.hour,o.minute,o.second,o.microsecond]}
+            if o.tzinfo is None:
+                o = o.replace(tzinfo=pytz.utc)
+
+            v = dt.timestamp(o) * 1000
+            v = max(int(v), v)
+
+            return {"_type_": "dt", "v": v}
+
+        elif isinstance(o, td):
+            v = o.total_seconds() * 1000
+            v = max(int(v), v)
+
+            return {"_type_": "td", "v": v}
+
+        else:
+            return json.JSONEncoder.default(self, o)
+
+
+def _extract_literal(s):
+    j1 = s.find("<")
+    j2 = s.rfind(">")
+
+    if j1 == 0 and j2 == len(s) - 1:
+        return json.loads(s[j1 + 1 : j2].strip())
+
+    return s
+
+
+def _get_key_value(line):
+    i1 = line.find("[")
+    i2 = line.find("]")
+
+    if i1 != 0 or i2 == -1:
+        raise ValueError(line)
+
+    key = line[i1 + 1 : i2].strip()
+    value = line[i2 + 1 :].strip()
+
+    key = _extract_literal(key)
+    # value = json.loads(value)
+
+    return key, value
+
+
+def get_params(text, keys=[], sep="\n", ordered=False, **kw):
+    """A custom json-like file format for dicts, which supports non-str keys.
+     Example:
+      [param_name] "json value"
+      [<2>] null
+      [<"<2>">] null
+      //comment line
+       -> {"param_name": "json value", 2: None, "<2>": None}
+    If param_name is surrouned with <>, it is assumed to be json value,
+    otherwise it is interpreted as string."""
+    lines0 = [x.strip() for x in text.split(sep)]
+
+    D = dict() if not ordered else OrderedDict()
+
+    return_nrs_n_lines = kw.get("return_nrs_n_lines")
+    line_nrs = OrderedDict()
+    init = kw.get("init")
+    missing = kw.get("missing", "raise")
+
+    if keys is not None and len(keys):
+        do_keys, unseen = True, set(keys)
+    else:
+        do_keys = unseen = None
+
+    for line_nr, line in enumerate(lines0):
+        if not len(line) or line[:2] == "//":
+            continue
+
+        try:
+            k, v = _get_key_value(line)
+        except ValueError:
+            warnings.warn(
+                'Damaged line ({line_nr}): "{line}"'.format(line_nr=line_nr, line=line)
+            )
+            continue
+
+        if do_keys:
+            if k not in keys:
+                continue
+            try:
+                unseen.remove(k)
+            except KeyError:
+                pass
+
+        v_json = json.loads(v)
+        D[k] = v_json if not init else init_data(v_json)
+        line_nrs[k] = line_nr
+
+    if do_keys and len(unseen) and missing == "raise":
+        raise KeyError("Missing Keys: {}".format(list(unseen)))
+
+    if return_nrs_n_lines:
+        return D, line_nrs, lines0
+
+    return D
+
+
+def read_params(path, keys=None, ordered=False, update=None, **kw):
+    """Read params from file.
+    If `keys` is given, only those key-values are returned
+    (if a key is missing then KeyError is raised)."""
+    encoding = kw.get("encoding")
+    if encoding is None:
+        encoding = "utf-8"
+
+    with open(path, encoding=encoding) as f:
+        text = f.read()
+
+    item = get_params(text, keys=keys, ordered=ordered, **kw)
+
+    if isinstance(update, dict):
+        if kw.get("read_nrs_n_lines"):
+            update.update(item[0])
+        else:
+            update.update(item)
+
+    return item
+
+
+def save_params(path, D, *, read_path=None, mode="a", **kw):
+    """Save params to a file, while retaining file's previous params and comments.
+    :param read_path: if given, previous params are read from that file
+                      (instead of the file to be overwritten, if exists)
+    :param mode: 'a' -> "append" new params to previous ones found in the file
+                 'w' -> overwrite the file, disregarding its previous content"""
+    line_nrs = {}
+    lines = []
+
+    cls = kw.get("cls")
+    if cls is None:
+        cls = DateTimeEncoder
+    elif cls == "DateTimeEncoder":
+        cls = DateTimeEncoder
+    elif cls == "DateTimeEncoderNumeric":
+        cls = DateTimeEncoderNumeric
+    elif isinstance(cls, str):
+        raise ValueError("Unknown cls: {}".format(cls))
+
+    deep = kw.get("deep")
+    init = kw.get("init", True)
+    read_path = path if read_path is None else read_path
+
+    if os.path.isfile(read_path) and mode in ("a", None):
+        # Note that `D2` and `line_nrs` contain only the requested keys (D.keys()) and their line nrs,
+        # while `lines` contains all lines (in str format) in the file
+        D2, line_nrs, lines = read_params(
+            read_path,
+            list(D.keys()),
+            ordered=True,
+            return_nrs_n_lines=True,
+            init=init,
+            missing="ignore",
+        )
+        D2.update(D) if not deep else deep_update(D2, D)
+        D = D2
+
+    llen = len(lines)
+
+    for k, v in D.items():
+        if isinstance(k, str):
+            k_final = (
+                k if not (k.startswith("<") and k.endswith(">")) else '<"{}">'.format(k)
+            )
+        else:
+            k_final = "<{}>".format(k)
+
+        line = "[{}] {}".format(k_final, json.dumps(v, cls=cls))
+
+        line_nr = line_nrs.get(k)
+
+        if line_nr is not None:
+            lines[line_nr] = line
+        else:
+            lines.append(line)
+
+    if len(lines) > llen and lines[llen - 1][:2] == "//":
+        lines.insert(llen, "")
+
+    if kw.get("comments"):
+        lines += ["//" + c for c in kw["comments"]]
+
+    encoding = kw.get("encoding")
+    if encoding is None:
+        encoding = "utf-8"
+
+    write_txt = "\n".join(lines)
+
+    with open(path, "w", encoding=encoding) as f:
+        f.write(write_txt)
+
+
+class SafeFileLock(filelock.FileLock):
+    def __init__(self, filepath, timeout=-1, poll_interval=0.02, log=True):
+        """NB! '.lock' will be added to filepath"""
+        lock_file = filepath + ".lock"
+        self._poll_interval_given = poll_interval
+        self._log_given = log
+        super().__init__(lock_file, timeout)
+
+    def acquire(self, timeout=None, poll_interval=None, log=None):
+        if poll_interval is None:
+            poll_interval = self._poll_interval_given
+        if log is None:
+            log = self._log_given
+
+        try:
+            return super().acquire(timeout, poll_interval)
+        except filelock.Timeout as e:
+            if log:
+                logger.error(e)
+
+            class ReturnProxy(object):
+                def __init__(self, lock):
+                    self.lock = lock
+                    return None
+
+                def __enter__(self):
+                    return self.lock
+
+                def __exit__(self, exc_type, exc_value, traceback):
+                    self.lock.release()
+                    return None
+
+            return ReturnProxy(lock=self)
+
+
+def wait_filelock(filepath, timeout=0.2, poll_interval=0.02, log=False):
+    with SafeFileLock(filepath, timeout, poll_interval, log):
+        pass
+
+
+# -------------------------------
+
+
+def _get_force_update(paths, meta, counter, force_update):
+    if not counter or force_update:
+        return True
+
+    lm = meta["last_modified"]
+
+    # if user decided to change the path of a file
+    if any(p not in lm for p in paths):
+        return True
+
+    for path, time in lm.items():
+        cur_last_modified = os.path.getmtime(path)
+        if time != cur_last_modified:
+            return True
+
+    return False
+
+
+def _load_settings(path, ftype, create, meta, force_update, return2):
+    if ftype is None:
+        loc = path.rfind(".")
+        if loc != -1:
+            ftype = path[loc + 1 :].lower()
+    else:
+        ftype = ftype.lower()
+
+    if os.path.exists(path):
+        pass
+    elif create:
+        with open(path, "w") as f:
+            f.write("")
+    else:
+        raise FileNotFoundError(path)
+
+    last_modified = os.path.getmtime(path)
+
+    if not force_update:
+        return return2
+
+    meta["last_modified"][path] = last_modified
+
+    if ftype in ("yaml", "yml"):
+        with open(path, encoding="utf-8") as f:
+            new = yaml.safe_load(f) or {}
+    elif ftype == "json":
+        with open(path, encoding="utf-8") as f:
+            new = json.load(f) or {}
+    else:
+        new = read_params(path)
+    # else: raise ValueError('Unknown ftype: {}'.format(ftype))
+
+    return new
+
+
+def _verify_is_dict(x, param, raise_errors):
+    is_dict = isinstance(x, dict)
+
+    if not is_dict:
+        msg = "{param} must be dict; got: {type}".format(
+            param=param, type=type(x).__name__
+        )
+        _handle_error(TypeError(msg), False, None, msg, raise_errors=raise_errors)
+
+    return is_dict
+
+
+def _handle_error(e, log_as_exception, txt=None, txt2=None, raise_errors=False):
+    if txt:
+        logger2.error(txt)
+    if raise_errors:
+        raise e
+    if txt2:
+        logger2.error(txt)
+    if log_as_exception:
+        logger.exception(e)
+
+
+def _get_param(meta, key, value):
+    if value is None:
+        value = meta.get(key)
+
+    return value
+
+
+def _get_exclude(meta, new, counter, exclude):
+    if not counter:
+        if exclude is None:
+            exclude = new.get("__exclude__")
+    else:
+        if exclude is not None and exclude != meta.get("exclude"):
+            warnings.warn("`exclude` can't be changed when counter > 0")
+        exclude = meta.get("exclude")
+
+    if exclude is None:
+        exclude = []
+
+    if not hasattr(exclude, "__getitem__"):
+        raise TypeError("`exclude` must be listlike, got: {}".format(type(exclude)))
+
+    meta["exclude"] = exclude
+
+    return exclude
+
+
+def _get_config(meta, new, counter, config=None, default=None):
+    if not counter:
+        if default is None:
+            default = new.get("__default__")
+        meta["default"] = default
+    else:
+        if default is not None and default != meta.get("default"):
+            warnings.warn("`default` can't be changed when counter > 0")
+        default = meta.get("default")
+
+    if not counter:
+        if config is None:
+            config = new.get("__config__")
+        if config is None:
+            config = default
+        meta["config"] = config
+    else:
+        if config is not None and config != meta.get("config"):
+            warnings.warn("`config` can't be changed when counter > 0")
+        config = meta.get("config")
+
+    return config, default
+
+
+def _get_config_dict(new, config, main_path, _load_args, *vid_args):
+    if config is None:
+        config_dict = new
+    elif config not in new:
+        raise KeyError('config: "{}" is not defined'.format(config))
+    else:
+        config_dict = new[config]
+
+    if isinstance(config_dict, str):
+        path = path0 = config_dict
+        ftype = None
+
+        if "|" in path:
+            path, ftype = path.split("|")
+
+        if ":" not in path:
+            if main_path is None:
+                msg = (
+                    "Config '{}' path is relative but the main file's path "
+                    'isn\'t specified; got: "{}"'
+                ).format(config, path0)
+                raise ValueError(msg)
+
+            main_path_dir = os.path.dirname(os.path.realpath(main_path))
+            relative_path = path.strip("/").strip("\\")
+            path = os.path.join(main_path_dir, relative_path)
+
+        config_dict = _load_settings(path, ftype, *_load_args)
+
+    _verify_is_dict(config_dict, "config:{}".format(config), *vid_args)
+
+    if config_dict is None:
+        config_dict = {}
+
+    return config_dict
+
+
+def _get_meta(old, *args):
+    meta = old.get("__meta__")
+    if meta is None:
+        old["__meta__"] = meta = {}
+
+    if not _verify_is_dict(meta, "__meta__", *args):
+        meta = {}
+
+    for k, defval in [
+        ["counter", 0],
+        ["last_modified", {}],
+        ["last_input", {}],
+        ["last_input_meta", {}],
+    ]:
+        if meta.get(k) is None:
+            meta[k] = defval
+
+    return meta
+
+
+def _update_meta(meta, config_dict, default_dict, logging_level, raise_errors):
+    def _notify(k, v):
+        logger2.log(logging_level, 'Setting __meta__ param "{}" to `{}`'.format(k, v))
+
+    meta_default = default_dict.get("__meta__")
+    meta_config = config_dict.get("__meta__")
+
+    if meta_config is None or not _verify_is_dict(
+        meta_config, "meta_config", raise_errors
+    ):
+        meta_config = {}
+
+    if meta_default is None or not _verify_is_dict(
+        meta_default, "meta_default", raise_errors
+    ):
+        meta_default = {}
+
+    # `borrow_keys` and `borrow_meta` themselves are always "borrowed"
+    borrow_keys = deep_get([meta_config, meta_default], "borrow_keys")
+    borrow_meta = deep_get([meta_config, meta_default], "borrow_meta")
+    if borrow_meta is None:
+        borrow_meta = borrow_keys
+
+    for k, v in [["borrow_keys", borrow_keys], ["borrow_meta", borrow_meta]]:
+        if v != meta.get(v):
+            _notify(k, v)
+        meta[k] = v
+
+    lim = meta["last_input_meta"]
+
+    meta_defvals = {
+        "1st_only": [],
+        "null_overwrite": True,
+        "interval": 15,
+        "init": False,
+        "deep": None,
+    }
+
+    def _update_value(k, *v):
+        if not v:
+            v = meta_config.get(k)
+            if v is None and borrow_meta:
+                v = meta_default.get(k)
+        else:
+            v = v[0]
+
+        if k in lim and lim[k] == v:
+            return
+
+        lim[k] = _copy.deepcopy(v)
+
+        if v is not None:
+            norm = next(x[1] for x in _META_NORM["items"] if x[0] == k)
+            try:
+                verify_data(v, norm, missing="ignore", extra="error")  # ??
+            except Exception as e:
+                logger2.error('__meta__ param "{}" incorrectly formatted.'.format(k))
+                if raise_errors:
+                    raise e
+                logger2.error(e)
+                # raise e
+                v = None
+
+        if v is None:
+            v = meta_defvals.get(k)
+
+        _notify(k, v)
+        meta[k] = v
+
+    for k in meta_defvals:
+        _update_value(k)
+
+
+def _update_keys(
+    meta,
+    old,
+    config_dict,
+    default_dict,
+    counter,
+    config,
+    default,
+    exclude,
+    init,
+    verify,
+    v_params,
+    raise_errors,
+):
+    _handle = functools.partial(_handle_error, raise_errors=raise_errors)
+
+    last_input = meta["last_input"]
+    first_only = (meta["1st_only"],)
+    null_overwrite = meta["null_overwrite"]
+    borrow_keys = meta["borrow_keys"]
+
+    skip = ["__meta__"] + exclude
+    if default is None:
+        skip += ["__config__", "__default__", "__exclude__"]
+        if config is not None:
+            skip += [config]
+
+    if not borrow_keys:
+        skip += [k for k in default_dict if k not in config_dict]
+
+    all_keys = list(unique(list(config_dict.keys()) + list(default_dict.keys())))
+    selected_keys = list(filter(lambda x: x not in skip, all_keys))
+
+    if verify is not None and not _isnorm(verify):
+        verify = normalize(verify)
+
+    if v_params is None:
+        v_params = {}
+    v_params = dict({"missing": "ignore", "extra": "error"}, **v_params)  # ??
+
+    new_dict = {}
+    new_last_input = {}
+    exc = None
+
+    for k in selected_keys:
+        if counter and k in first_only:
+            continue
+
+        if k in config_dict or not borrow_keys:
+            new_val = config_dict[k]
+        else:
+            new_val = default_dict.get(k)
+
+        if new_val is None and k in old and not null_overwrite:
+            continue
+        elif k in last_input and new_val == last_input[k]:
+            continue
+
+        new_last_input[k] = _copy.deepcopy(new_val)
+
+        if init:
+            try:
+                new_val = init_data(new_val)
+            except Exception as e:
+                exc = e
+                _handle(exc, True, 'Could not initiate param "{}"'.format(k))
+                break
+
+        if verify is not None:
+            try:
+                norm = next(x[1] for x in verify["items"] if x[0] == k)
+            except StopIteration as e:
+                exc = KeyError("Unknown param: {}".format(k))
+                _handle(exc, False, None, "Unknown param: {}".format(k))
+                break
+
+            try:
+                verify_data(new_val, norm, **v_params)
+            except Exception as e:
+                exc = e
+                _handle(exc, True, 'Param "{}" incorrectly formatted.'.format(k))
+                break
+
+        new_dict[k] = new_val
+
+    return new_dict, new_last_input, exc
+
+
+def update_settings(
+    new,
+    old=None,
+    verify=None,
+    *,
+    ftype=None,
+    deep=None,
+    init=False,
+    logging_level="INFO",
+    create=False,
+    v_params=None,
+    force_update=False,
+    errors="raise",
+    config=None,
+    default=None,
+    exclude=None
+):
+    """Update a dict with new values.
+    :param new: dict or path to a file (containing dict)
+    :param old: previous dict, meant to be reused on all calls
+    :param verify: the `norm` dict to be used to verify
+    :param create: if True and a file doesn't exist, create an empty one;
+    '              otherwise raise FileNotFoundError
+    :param errors: 'ignore', 'raise', 'log' ('ignore' is logged too)
+    """
+    if errors not in ("ignore", "raise", "log"):
+        raise ValueError(errors)
+    logging_level = _log.level_to_int(logging_level)
+    raise_errors = errors == "raise"
+    vid_args = (raise_errors,)
+
+    if old is None:
+        old = {}
+
+    meta = _get_meta(old, *vid_args)
+    counter = meta["counter"]
+    path = new if isinstance(new, str) else None
+
+    force_update = _get_force_update([path], meta, counter, force_update)
+
+    if path is not None:
+        new = _load_settings(path, ftype, create, meta, force_update, old)
+        if new is old:
+            return old
+
+    config, default = _get_config(meta, new, counter, config, default)
+    # print(config, default)
+    exclude = _get_exclude(meta, new, counter, exclude)
+
+    meta["counter"] += 1
+
+    _load_args = (create, meta, True, {})
+    config_dict = _get_config_dict(new, config, path, _load_args, *vid_args)
+
+    if config == default:
+        default_dict = config_dict
+    else:
+        default_dict = _get_config_dict(new, default, path, _load_args, *vid_args)
+
+    _update_meta(meta, config_dict, default_dict, logging_level, raise_errors)
+
+    init = _get_param(meta, "init", init)
+    deep = _get_param(meta, "deep", deep)
+
+    new_dict, new_last_input, exc = _update_keys(
+        meta,
+        old,
+        config_dict,
+        default_dict,
+        counter,
+        config,
+        default,
+        exclude,
+        init,
+        verify,
+        v_params,
+        raise_errors,
+    )
+
+    # We do not want to update only half the params (might cause a fiasco)
+    # either update all or reject and return the old
+    if exc is not None:
+        return old
+
+    for k, new_val in new_dict.items():
+        logger2.log(logging_level, 'Setting param "{}" to `{}`'.format(k, new_val))
+
+    if deep:
+        deep_update(old, new_dict)
+    else:
+        old.update(new_dict)
+
+    meta["last_input"].update(new_last_input)
+
+    return old
```

### Comparing `fons-0.3.1/fons/iter.py` & `fons-0.4.0/fons/iter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,318 +1,337 @@
-import numpy as np
-import pandas as pd
-import collections
-import itertools
-
-SETLIKE = (set,)
-LISTLIKE = (list, tuple, np.ndarray, pd.Index, collections.deque)
-LISTSETLIKE =  LISTLIKE + SETLIKE
-DICTLIKE = (dict,)
-CONTAINERLIKE = LISTLIKE + SETLIKE + DICTLIKE
-_SAMPLES = [(x for x in []), {}.keys(), {}.values(), {}.items()]
-# This is covered by _is_known_iterator test
-#_SAMPLES2 = [iter([]), iter(tuple()), iter({}), iter({}.keys()), iter({}.values()), iter({}).items(),
-#             iter(set()), iter(str()), iter(range(1,2)),
-#             iter(enumerate([])), iter(pd.Index([])), iter(np.array([]))]
-#Note:
-#type(iter(np.array([]))).__name__ == 'iterator'
-GENLIKE = tuple(map(type,_SAMPLES)) + (range, enumerate, zip, map, filter, itertools.chain)
-LISTGEN = LISTLIKE + GENLIKE
-
-_MAP_LISTLIKE = {tuple: tuple,
-                 list: list,
-                 pd.Index: pd.Index,
-                 np.ndarray: lambda x: np.asarray(tuple(x)),
-                 set: set}
-
-
-def _normalize_args(include_types, ignore_types):
-    ignore_types = tuple(ignore_types)
-    
-    if not isinstance(include_types, str):
-        include_types = tuple(include_types)
-        
-    elif include_types not in ('all','iterable'):
-        raise ValueError(include_types)
-    
-    return include_types, ignore_types
-
-
-def _is_known_iterator(_type, x):
-    try: 
-        return _type.__name__.endswith('iterator') and hasattr(x,'__iter__')
-    except TypeError:
-        return False
-
-
-def _is_iterable(x):
-    try:
-        #return hasattr(x, '__iter__') or hasattr(x, '__getitem__')
-        # __getitem__ does not always make it iterable (if it doesn't start with 0 index) 
-        iter(x)
-    except TypeError:
-        return False
-    else:
-        return True
-    
-    
-def _tests(x, include_types, ignore_types, **kw):
-    _type = type(x)
-    
-    if ignore_types and issubclass(_type, ignore_types):
-        return False
-    
-    # returns self (e.g. next(iter('a')))
-    if 'last' in kw and kw['last'] is x:
-        return False
-    
-    # Just in case the "last" test failed on str (str id-s differ for some reason)
-    if issubclass(_type, str) and len(x) < 2:
-        return False
-    
-    if isinstance(include_types, str) and include_types in ('all','iterable'):
-        return _is_iterable(x)
-       
-    if issubclass(_type, LISTSETLIKE):
-        return True
-    
-    if issubclass(_type, GENLIKE) or _is_known_iterator(_type, x):
-        return True
-    
-    if not isinstance(include_types, str) and include_types and issubclass(_type, include_types):
-        return True
-    
-    return False
-    
-
-def flatten(x, include_types=(), ignore_types=(), astype=None, **kw):
-    """
-       Flattens a "known" iterable (NB! while yet ignoring strings, dicts, custom defined classes)
-        flatten([2, (3,4,{5}), {6: 7}, '89', iter('10'), {11:12}.items()], astype=list) ->
-            ->  [2, 3, 4, 5, {6: 7}, '89', '1', '0', 11, 12]
-       `included_types` / `ignore_types` also applies to subclasses.
-       If `x` itself is "ignored", raises TypeError: flatten(2), flatten('abc')
-       Included by default: list, tuple, deque, set, np.ndarray, pd.Index, 
-                            dict.keys, dict.values, dict.items, filter, map, generator,
-                            any class which name ends with "iterator" and has "__iter__" attr
-                            (for including types like list_iterator, resulting from iter([]))
-       Are NOT included by default:
-                            Custom defined classes with __iter__ / __getitem__,
-                            pd.Series, pd.DataFrame, dict, str, namedtuple
-                            (the reason for ignoring dict, pd.Series, pd.DataFrame is to avoid
-                             accidentally dropping extra information (keys, index, columns))
-       For including ANY iterable, pass `include_types="all", or use `fliter` function instead.
-       
-       Returns: itertools.chain object, or `astype(result)` if `astype` is specified.
-    """
-    r = kw.get('r',0)
-    
-    if not r:
-        include_types, ignore_types = _normalize_args(include_types, ignore_types) 
-    
-    if not _tests(x, include_types, ignore_types, **kw):
-        if r == 0:
-            raise TypeError('Obj must be list(set)like or generator-like; Got: {}'.format(type(x)))
-        return (x,)
-    
-    generators = (flatten(y, include_types, ignore_types, None, r=r+1, last=x) for y in x)
-    flat = itertools.chain.from_iterable(generators)
-    
-    if astype is not None:
-        astype = _MAP_LISTLIKE.get(astype, astype)
-        flat = astype(flat)
-    
-    return flat
-
-
-def flatten2(x, include_types=(), ignore_types=(), astype=None):
-    """
-    Ignores `set` subtypes
-    """
-    ignore_types = tuple(ignore_types) + (set,)
-    
-    return flatten(x, include_types, ignore_types, astype)
-
-
-def flatten_dict(x, include_types=(), ignore_types=(), astype=None):
-    """
-    'Includes `dict` subtypes
-    """
-    if not isinstance(include_types, str):
-        include_types = tuple(include_types) + (dict,)
-        
-    return flatten(x, include_types, ignore_types, astype)
-
-
-def fliter(x, ignore_types=(), astype=None):
-    """
-    Flattens all iterable objects within (including strings!).
-    """
-    return flatten(x, 'all', ignore_types, astype)
-
-
-def is_flat(x, include_types=(), ignore_types=()):
-
-    include_types, ignore_types = _normalize_args(include_types, ignore_types) 
-    
-    if not _tests(x, include_types, ignore_types):
-        raise TypeError('Obj must be list(set)like or generator-like; Got: {}'.format(type(x)))
-    
-    if any(_tests(y, include_types, ignore_types) for y in x):
-        return False
-    
-    return True
-
-
-def is_flit(x, ignore_types=()):
-    return is_flat(x, 'all', ignore_types)
-
-
-def unique(seq, key=None, op=None, astype=None):
-    """
-    :param seq: an iterable
-    :param key: None / <function> / <str> / <object>
-                if <str> (or <object>), `x[key]` is used, 
-                 or `getattr(x, key)` if x does not possess __getitem__
-    :param op: None / lambda x,y: x==y / '__eq__' / '=='
-               function must return positive for match; if left to None then 
-               `x in seen` is used, where `seen` is set (or list, if `x` is not hashable)
-    :returns: iterator, or `astype(result)` if `astype` is specified.
-    """
-
-    keyfunc = key
-    
-    if key is not None and not hasattr(key,'__call__'):
-        def keyfunc(x, key=key):
-            if hasattr(x, '__getitem__'):
-                return x[key]
-            else:
-                return getattr(x, key)
-        
-    if op is None:
-        
-        def is_first(x, seen_set=set(), seen_list=[]):
-            try: hash(x)
-            except TypeError:
-                is_hashable = False
-            else: is_hashable = True
-            
-            if is_hashable:
-                if x not in seen_set:
-                    seen_set.add(x)
-                    return True
-            else:
-                if x not in seen_list:
-                    seen_list.append(x)
-                    return True
-            
-            return False
-        
-    else:
-        op2 = op
-        if isinstance(op, str):
-            if op == '==':
-                op2 = lambda y,x: y==x
-            else:
-                op2 = lambda y,x: getattr(y,op)(x)
-        
-        
-        def compare(y, x, f=op2):
-            v = f(y, x)
-            if v is not NotImplemented:
-                return v
-            
-            v = f(x, y)
-    
-            if v is NotImplemented:
-                return False
-            
-            return v
-        
-        
-        def is_first(x, seen_list=[]):
-            if not any(compare(y,x) for y in seen_list):
-                seen_list.append(x)
-                return True
-            
-            return False
-            
-    
-    if keyfunc is not None:
-        def uniq(x, keyfunc=keyfunc):
-            x2 = keyfunc(x)
-            return is_first(x2)
-    else:
-        uniq = is_first
-
-
-    seq_unique = filter(uniq, seq)
-    
-    if astype is not None:
-        astype = _MAP_LISTLIKE.get(astype, astype)
-        seq_unique = astype(seq_unique)
-    
-    return seq_unique
-
-
-
-def consume(iterator, n=None):
-    "Advance the iterator n-steps ahead. If n is None, consume entirely."
-    # Use functions that consume iterators at C speed.
-    if n is None:
-        # feed the entire iterator into a zero-length deque
-        collections.deque(iterator, maxlen=0)
-    else:
-        # advance to the empty slice starting at position n
-        next(itertools.islice(iterator, n, n), None)
-        
-        
-def sequence_insert(seq, ins_to, *, key=None, duplicates='keep', sort=False):
-    """Inserts sequence items into `ins_to`. Items in both arrays must be sortable (by `key`),
-        and both arrays must be sorted beforehand in ascending order.
-       sequence_insert([{'a': 2},{'a': 5}], [{'a': 2, 'x': 15}, {'a': 4}],
-                                    key=lambda x: x['a'], duplicates='drop') ->
-           -> ins_to = [{'a': 2, 'x': 15}, {'a': 4}, {'a': 5}]
-       
-       :param duplicates: if 'drop', duplicates are dropped, where keep='last';
-                          if 'keep', do [..., old_item, equal_new_item_here, ..]
-       :param sort: if True, first sorts `seq` (not `ins_to`!)
-       :returns: None"""
-    if duplicates not in ('keep','drop'):
-        raise ValueError(duplicates)
-    if sort:
-        seq = sorted(seq, key=key)
-    
-    drop = (duplicates=='drop')
-    is_deque = isinstance(ins_to, collections.deque)
-    key = (lambda x: x) if key is None else key
-    
-    for this in seq:
-        compare_this = key(this)
-        try:
-            i, are_equals = next((-i,key(x)==compare_this) 
-                                        for i,x in enumerate(reversed(ins_to)) 
-                                    if compare_this>=key(x))
-            if i == 0 and (not are_equals or not drop):
-                i = None 
-        except StopIteration:
-            i, are_equals = (0, False)
-            
-        if are_equals and drop:
-            ins_to[i-1] = this
-        else:
-            if i is None:
-                ins_to.append(this)
-            else:
-                #[2,3,4].insert(-1,5) ->
-                #[2,3,5,4]
-                try:
-                    ins_to.insert(i, this)
-                except IndexError as e:
-                    if is_deque:
-                        ins_to.popleft()
-                        ins_to.insert(i, this)
-                    else:
-                        raise e
-                    
-    return None
-
+import numpy as np
+import pandas as pd
+import collections
+import itertools
+
+SETLIKE = (set,)
+LISTLIKE = (list, tuple, np.ndarray, pd.Index, collections.deque)
+LISTSETLIKE = LISTLIKE + SETLIKE
+DICTLIKE = (dict,)
+CONTAINERLIKE = LISTLIKE + SETLIKE + DICTLIKE
+_SAMPLES = [(x for x in []), {}.keys(), {}.values(), {}.items()]
+# This is covered by _is_known_iterator test
+# _SAMPLES2 = [iter([]), iter(tuple()), iter({}), iter({}.keys()), iter({}.values()), iter({}).items(),
+#             iter(set()), iter(str()), iter(range(1,2)),
+#             iter(enumerate([])), iter(pd.Index([])), iter(np.array([]))]
+# Note:
+# type(iter(np.array([]))).__name__ == 'iterator'
+GENLIKE = tuple(map(type, _SAMPLES)) + (
+    range,
+    enumerate,
+    zip,
+    map,
+    filter,
+    itertools.chain,
+)
+LISTGEN = LISTLIKE + GENLIKE
+
+_MAP_LISTLIKE = {
+    tuple: tuple,
+    list: list,
+    pd.Index: pd.Index,
+    np.ndarray: lambda x: np.asarray(tuple(x)),
+    set: set,
+}
+
+
+def _normalize_args(include_types, ignore_types):
+    ignore_types = tuple(ignore_types)
+
+    if not isinstance(include_types, str):
+        include_types = tuple(include_types)
+
+    elif include_types not in ("all", "iterable"):
+        raise ValueError(include_types)
+
+    return include_types, ignore_types
+
+
+def _is_known_iterator(_type, x):
+    try:
+        return _type.__name__.endswith("iterator") and hasattr(x, "__iter__")
+    except TypeError:
+        return False
+
+
+def _is_iterable(x):
+    try:
+        # return hasattr(x, '__iter__') or hasattr(x, '__getitem__')
+        # __getitem__ does not always make it iterable (if it doesn't start with 0 index)
+        iter(x)
+    except TypeError:
+        return False
+    else:
+        return True
+
+
+def _tests(x, include_types, ignore_types, **kw):
+    _type = type(x)
+
+    if ignore_types and issubclass(_type, ignore_types):
+        return False
+
+    # returns self (e.g. next(iter('a')))
+    if "last" in kw and kw["last"] is x:
+        return False
+
+    # Just in case the "last" test failed on str (str id-s differ for some reason)
+    if issubclass(_type, str) and len(x) < 2:
+        return False
+
+    if isinstance(include_types, str) and include_types in ("all", "iterable"):
+        return _is_iterable(x)
+
+    if issubclass(_type, LISTSETLIKE):
+        return True
+
+    if issubclass(_type, GENLIKE) or _is_known_iterator(_type, x):
+        return True
+
+    if (
+        not isinstance(include_types, str)
+        and include_types
+        and issubclass(_type, include_types)
+    ):
+        return True
+
+    return False
+
+
+def flatten(x, include_types=(), ignore_types=(), astype=None, **kw):
+    """
+    Flattens a "known" iterable (NB! while yet ignoring strings, dicts, custom defined classes)
+     flatten([2, (3,4,{5}), {6: 7}, '89', iter('10'), {11:12}.items()], astype=list) ->
+         ->  [2, 3, 4, 5, {6: 7}, '89', '1', '0', 11, 12]
+    `included_types` / `ignore_types` also applies to subclasses.
+    If `x` itself is "ignored", raises TypeError: flatten(2), flatten('abc')
+    Included by default: list, tuple, deque, set, np.ndarray, pd.Index,
+                         dict.keys, dict.values, dict.items, filter, map, generator,
+                         any class which name ends with "iterator" and has "__iter__" attr
+                         (for including types like list_iterator, resulting from iter([]))
+    Are NOT included by default:
+                         Custom defined classes with __iter__ / __getitem__,
+                         pd.Series, pd.DataFrame, dict, str, namedtuple
+                         (the reason for ignoring dict, pd.Series, pd.DataFrame is to avoid
+                          accidentally dropping extra information (keys, index, columns))
+    For including ANY iterable, pass `include_types="all", or use `fliter` function instead.
+
+    Returns: itertools.chain object, or `astype(result)` if `astype` is specified.
+    """
+    r = kw.get("r", 0)
+
+    if not r:
+        include_types, ignore_types = _normalize_args(include_types, ignore_types)
+
+    if not _tests(x, include_types, ignore_types, **kw):
+        if r == 0:
+            raise TypeError(
+                "Obj must be list(set)like or generator-like; Got: {}".format(type(x))
+            )
+        return (x,)
+
+    generators = (
+        flatten(y, include_types, ignore_types, None, r=r + 1, last=x) for y in x
+    )
+    flat = itertools.chain.from_iterable(generators)
+
+    if astype is not None:
+        astype = _MAP_LISTLIKE.get(astype, astype)
+        flat = astype(flat)
+
+    return flat
+
+
+def flatten2(x, include_types=(), ignore_types=(), astype=None):
+    """
+    Ignores `set` subtypes
+    """
+    ignore_types = tuple(ignore_types) + (set,)
+
+    return flatten(x, include_types, ignore_types, astype)
+
+
+def flatten_dict(x, include_types=(), ignore_types=(), astype=None):
+    """
+    'Includes `dict` subtypes
+    """
+    if not isinstance(include_types, str):
+        include_types = tuple(include_types) + (dict,)
+
+    return flatten(x, include_types, ignore_types, astype)
+
+
+def fliter(x, ignore_types=(), astype=None):
+    """
+    Flattens all iterable objects within (including strings!).
+    """
+    return flatten(x, "all", ignore_types, astype)
+
+
+def is_flat(x, include_types=(), ignore_types=()):
+    include_types, ignore_types = _normalize_args(include_types, ignore_types)
+
+    if not _tests(x, include_types, ignore_types):
+        raise TypeError(
+            "Obj must be list(set)like or generator-like; Got: {}".format(type(x))
+        )
+
+    if any(_tests(y, include_types, ignore_types) for y in x):
+        return False
+
+    return True
+
+
+def is_flit(x, ignore_types=()):
+    return is_flat(x, "all", ignore_types)
+
+
+def unique(seq, key=None, op=None, astype=None):
+    """
+    :param seq: an iterable
+    :param key: None / <function> / <str> / <object>
+                if <str> (or <object>), `x[key]` is used,
+                 or `getattr(x, key)` if x does not possess __getitem__
+    :param op: None / lambda x,y: x==y / '__eq__' / '=='
+               function must return positive for match; if left to None then
+               `x in seen` is used, where `seen` is set (or list, if `x` is not hashable)
+    :returns: iterator, or `astype(result)` if `astype` is specified.
+    """
+
+    keyfunc = key
+
+    if key is not None and not hasattr(key, "__call__"):
+
+        def keyfunc(x, key=key):
+            if hasattr(x, "__getitem__"):
+                return x[key]
+            else:
+                return getattr(x, key)
+
+    if op is None:
+
+        def is_first(x, seen_set=set(), seen_list=[]):
+            try:
+                hash(x)
+            except TypeError:
+                is_hashable = False
+            else:
+                is_hashable = True
+
+            if is_hashable:
+                if x not in seen_set:
+                    seen_set.add(x)
+                    return True
+            else:
+                if x not in seen_list:
+                    seen_list.append(x)
+                    return True
+
+            return False
+
+    else:
+        op2 = op
+        if isinstance(op, str):
+            if op == "==":
+                op2 = lambda y, x: y == x
+            else:
+                op2 = lambda y, x: getattr(y, op)(x)
+
+        def compare(y, x, f=op2):
+            v = f(y, x)
+            if v is not NotImplemented:
+                return v
+
+            v = f(x, y)
+
+            if v is NotImplemented:
+                return False
+
+            return v
+
+        def is_first(x, seen_list=[]):
+            if not any(compare(y, x) for y in seen_list):
+                seen_list.append(x)
+                return True
+
+            return False
+
+    if keyfunc is not None:
+
+        def uniq(x, keyfunc=keyfunc):
+            x2 = keyfunc(x)
+            return is_first(x2)
+
+    else:
+        uniq = is_first
+
+    seq_unique = filter(uniq, seq)
+
+    if astype is not None:
+        astype = _MAP_LISTLIKE.get(astype, astype)
+        seq_unique = astype(seq_unique)
+
+    return seq_unique
+
+
+def consume(iterator, n=None):
+    "Advance the iterator n-steps ahead. If n is None, consume entirely."
+    # Use functions that consume iterators at C speed.
+    if n is None:
+        # feed the entire iterator into a zero-length deque
+        collections.deque(iterator, maxlen=0)
+    else:
+        # advance to the empty slice starting at position n
+        next(itertools.islice(iterator, n, n), None)
+
+
+def sequence_insert(seq, ins_to, *, key=None, duplicates="keep", sort=False):
+    """Inserts sequence items into `ins_to`. Items in both arrays must be sortable (by `key`),
+     and both arrays must be sorted beforehand in ascending order.
+    sequence_insert([{'a': 2},{'a': 5}], [{'a': 2, 'x': 15}, {'a': 4}],
+                                 key=lambda x: x['a'], duplicates='drop') ->
+        -> ins_to = [{'a': 2, 'x': 15}, {'a': 4}, {'a': 5}]
+
+    :param duplicates: if 'drop', duplicates are dropped, where keep='last';
+                       if 'keep', do [..., old_item, equal_new_item_here, ..]
+    :param sort: if True, first sorts `seq` (not `ins_to`!)
+    :returns: None"""
+    if duplicates not in ("keep", "drop"):
+        raise ValueError(duplicates)
+    if sort:
+        seq = sorted(seq, key=key)
+
+    drop = duplicates == "drop"
+    is_deque = isinstance(ins_to, collections.deque)
+    key = (lambda x: x) if key is None else key
+
+    for this in seq:
+        compare_this = key(this)
+        try:
+            i, are_equals = next(
+                (-i, key(x) == compare_this)
+                for i, x in enumerate(reversed(ins_to))
+                if compare_this >= key(x)
+            )
+            if i == 0 and (not are_equals or not drop):
+                i = None
+        except StopIteration:
+            i, are_equals = (0, False)
+
+        if are_equals and drop:
+            ins_to[i - 1] = this
+        else:
+            if i is None:
+                ins_to.append(this)
+            else:
+                # [2,3,4].insert(-1,5) ->
+                # [2,3,5,4]
+                try:
+                    ins_to.insert(i, this)
+                except IndexError as e:
+                    if is_deque:
+                        ins_to.popleft()
+                        ins_to.insert(i, this)
+                    else:
+                        raise e
+
+    return None
```

### Comparing `fons-0.3.1/fons/log.py` & `fons-0.4.0/fons/log.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,782 +1,874 @@
-import datetime
-dt = datetime.datetime
-import time
-import sys,os,io
-from collections import namedtuple
-import traceback
-import threading
-import multiprocessing
-import warnings
-import yaml
-import logging
-from logging.handlers import (RotatingFileHandler, QueueHandler)
-OldLoggingFormatter = logging.Formatter
-
-
-class FonsLogger(logging.Logger):  
-    def findCaller(self, stack_info=False):
-        """
-        Find the stack frame of the caller so that we can note the source
-        file name, line number and function name.
-        """
-        f = logging.currentframe()
-        #On some versions of IronPython, currentframe() returns None if
-        #IronPython isn't run with -X:Frames.
-        if f is not None:
-            f = f.f_back
-        rv = "(unknown file)", 0, "(unknown function)", None
-        while hasattr(f, "f_code"):
-            co = f.f_code
-            filename = os.path.normcase(co.co_filename)
-            # added _srcfile2 (this file), so that .llog/.__call__ 
-            # method would not show as caller
-            if filename in (logging._srcfile, getattr(logging, '_srcfile2')):
-                f = f.f_back
-                continue
-            sinfo = None
-            if stack_info:
-                sio = io.StringIO()
-                sio.write('Stack (most recent call last):\n')
-                traceback.print_stack(f, file=sio)
-                sinfo = sio.getvalue()
-                if sinfo[-1] == '\n':
-                    sinfo = sinfo[:-1]
-                sio.close()
-            rv = (co.co_filename, f.f_lineno, co.co_name, sinfo)
-            break
-        return rv
-    
-    def handle(self, record, *args, declude_with_queues=[], **kw):
-        """
-        Call the handlers for the specified record.
-
-        This method is used for unpickled records received from a socket, as
-        well as those created locally. Logger-level filtering is applied.
-        """
-        # `declude_with_queues` is necessary for avoiding infinite recursion
-        # in handling QueueHandler records (QueueHandler is used to connect 
-        # with child processes)
-        if (not self.disabled) and self.filter(record):
-            self.callHandlers(record, declude_with_queues=declude_with_queues)
-    
-    def callHandlers(self, record, *args, declude_with_queues=[], **kw):
-        """
-        Pass a record to all relevant handlers.
-
-        Loop through all handlers for this logger and its parents in the
-        logger hierarchy. If no handler was found, output a one-off error
-        message to sys.stderr. Stop searching up the hierarchy whenever a
-        logger with the "propagate" attribute set to zero is found - that
-        will be the last logger whose handlers are called.
-        """
-        q_check = lambda h: isinstance(h, QueueHandler) and h.queue in declude_with_queues
-        c = self
-        found = 0
-        while c:
-            for hdlr in c.handlers:
-                found = found + 1
-                if q_check(hdlr): pass
-                elif record.levelno >= hdlr.level:
-                    hdlr.handle(record)
-            if not c.propagate:
-                c = None    #break out
-            else:
-                c = c.parent
-        if (found == 0):
-            if logging.lastResort:
-                if q_check(logging.lastResort): pass
-                elif record.levelno >= logging.lastResort.level:
-                    logging.lastResort.handle(record)
-            elif logging.raiseExceptions and not self.manager.emittedNoHandlerWarning:
-                sys.stderr.write("No handlers could be found for logger"
-                                 " \"%s\"\n" % self.name)
-                self.manager.emittedNoHandlerWarning = True
-    
-    
-class EmptyLogger:
-    def debug(self, msg, *args, **kwargs):
-        pass
-    def info(self, msg, *args, **kwargs):
-        pass
-    def warn(self, msg, *args, **kwargs):
-        pass
-    def warning(self, msg, *args, **kwargs):
-        pass
-    def error(self, msg, *args, **kwargs):
-        pass
-    def exception(self, msg, *args, exc_info=True, **kwargs):
-        pass
-    def critical(self, msg, *args, **kwargs):
-        pass
-    def log(self, level, msg, *args, **kwargs):
-        pass
-
-
-SETTINGS_PATH = os.path.abspath(os.path.join(os.path.join(__file__, '..'), 'settings.yaml'))
-
-
-def _read_settings():
-    if os.path.exists(SETTINGS_PATH):
-        with open(SETTINGS_PATH, encoding='utf-8') as f:
-            return yaml.safe_load(f)
-    else:
-        return {}
-
-
-def _save_settings(d, mode='a'):
-    if mode not in ('a','w'):
-        raise ValueError(mode)
-    d_prev = {}
-    if mode == 'a':
-        d_prev = _read_settings()
-    d_prev.update(d)
-    with open(SETTINGS_PATH, 'w', encoding='utf-8') as f:
-        yaml.dump(d_prev, f)
-
-
-def _read_root_dir():
-    root_dir = ''
-    d = _read_settings()
-    if d.get('logging_default_root_dir') is not None:
-        root_dir = d['logging_default_root_dir']
-    if not isinstance(root_dir, str):
-        raise TypeError('Logging root dir in settings file must be of type <str>, got: {}'\
-                        .format(type(root_dir)))
-    return root_dir
-
-
-def set_default_root_dir(path, make_permanent=False):
-    """
-    Set the default directory where file handlers will output their files
-    (=='dir' param in functions 'standard_logging' and 'setup_logging').
-    :param make_permanent: 
-        if True, writes to settings file (will keep defaulting to that during
-        the future python instances)
-    """
-    global DEFAULT_ROOT_DIR
-    if not isinstance(path, str):
-        raise TypeError(type(path))
-    DEFAULT_ROOT_DIR = path
-    if make_permanent:
-        _save_settings({'logging_default_root_dir': path}, 'a')
-
-
-# '' will later resolve to current working directory
-DEFAULT_ROOT_DIR = _read_root_dir()
-
-logging._srcfile2 = os.path.normcase(FonsLogger.findCaller.__code__.co_filename)
-
-# For excluding this module from Logger's record (like logging module does)
-# and fixing infinite recursion caused by LogListener trying to handle 
-# QueueHandler's record (this won't affect user defined QueueHandlers)
-logging.Logger.findCaller = FonsLogger.findCaller
-logging.Logger.handle = FonsLogger.handle
-logging.Logger.callHandlers = FonsLogger.callHandlers
-
-# This was necessary for something. For making compatible with new Logger methods?
-_rhandlers,_rfilters = logging.root.handlers, logging.root.filters
-logging.root = logging.RootLogger(logging.root.level)
-logging.root.handlers = _rhandlers
-logging.root.filters = _rfilters
-
-NR_CONSOLE_LINES = 300
-STREAMING_LOGGERS = ['L2','T2']
-
-_is_logger_overwritten = False
-_default_fmt = '%(asctime)s:%(levelname)s:%(name)s:%(module)s:%(funcName)s(%(lineno)d):%(message)s'
-_queue = multiprocessing.Queue(-1)
-_lock = multiprocessing.Lock()
-_globals = {'queue': _queue,
-            'TEST_MODE': False,
-            'level': 'INFO',
-            'fmt': None,
-            'use_FonsFormatter': True,}
-
-_modules = [__name__]
-_tklogiprocesses = {}
-_sys_stdout_assigned = False
-_mp_logging_enabled = False
-_listener = None
-
-_s5_names = {
-    'logger': 'L1',
-    'logger2': 'L2',
-    'tlogger': 'T1',
-    'tloggers': 'T2',
-    'tlogger0': 'T0'}
-_Standard_5 = namedtuple('StandardLogging_5','logger logger2 tlogger tloggers tlogger0')
-_Standard_5.__new__.__defaults__ = tuple(logging.getLogger(_s5_names[x]) for x in _Standard_5._fields)
- 
-standard_5 = _Standard_5()
-
-# The difference between logger and logger2 (and tlogger / tloggers) is that after calling setup_logging(),
-# logger2 (and tloggers) will *also* stream to console, while logger (and tlogger, tlogger0) only stream to file
-logger = standard_5.logger
-logger2 = standard_5.logger2
-tlogger = standard_5.tlogger
-tloggers = standard_5.tloggers
-tlogger0 = standard_5.tlogger0
-
-
-for _logger in standard_5[:2]:
-    _logger.setLevel(10)
-# Set test loggers' level to 0
-for _logger in standard_5[2:]:
-    _logger.setLevel(0)
-
-
-class TempStreamHandler(logging.StreamHandler):
-    """
-    Only stream if root has not handlers set (to avoid duplication)
-    """
-    def handle(self, record):
-        if not logging.root.handlers and not _mp_logging_enabled:
-            return logging.StreamHandler.handle(self, record)
-
-
-# We want the logger and logger2 to stream only if user has not called basicConfig(),
-# and revoke the streaming when user decides to call it later
-if not logging.root.handlers and not _mp_logging_enabled:
-    _h = TempStreamHandler()
-    _h.setFormatter(logging.Formatter(logging.BASIC_FORMAT))
-    logger.addHandler(_h)
-    logger2.addHandler(_h)
-
-
-#----------------------------------------------
-
-class FonsFormatter(logging.Formatter):
-    converter=dt.utcfromtimestamp
-
-    def formatTime(self, record, datefmt=None):
-        
-        ct = self.converter(record.created)
-        if datefmt:
-            s = ct.strftime(datefmt)
-        else:
-            t = ct.strftime("%Y-%m-%dT%H:%M:%S")
-            s = "%s.%03d" % (t, record.msecs)
-            
-        return s
-    
-    
-class FonsFormatter2(logging.Formatter):
-    converter=time.gmtime
-    default_time_format = "%Y-%m-%d %H:%M:%S"
-    defualt_msec_format = "%s.%03d"
-
-
-def initiate_FonsFormat():
-    logging.Formatter = FonsFormatter
-
-
-#-------------------------------------------
-
-def getFonsLogger(name=None, lvl='DEBUG', streams=True, fmt=None, use_FonsFormatter=True):
-    if name is None:
-        name = __name__
-    logger = logging.getLogger(name)
-    logger.setLevel(lvl)
-    
-    if fmt is None:
-        fmt = '%(asctime)s:%(levelname)s:%(name)s:%(funcName)s: %(message)s'
-    elif fmt == 'simpleformat':
-        fmt = '%(asctime)s %(message)s'
-    
-    remove_stream_handlers(logger)
-    
-    if streams:
-        console = logging.StreamHandler()
-        aFormatter = FonsFormatter if use_FonsFormatter else OldLoggingFormatter
-
-        formatter = aFormatter(fmt=fmt)
-        console.setFormatter(formatter)
-
-        logger.addHandler(console)
-        
-        
-    """if queue is not None:
-        logger.addHandler(QueueHandler(queue))"""
-
-
-    return logger
-
-
-
-class Tee(object):
-    def __init__(self, files=[], lvl=logging.INFO, logger=None):
-        self.files = files
-        
-        if logger is None:
-            self.logger = getFonsLogger('stdout', streams=False, fmt=_globals['fmt'],
-                                      use_FonsFormatter=_globals['use_FonsFormatter'])
-        else: self.logger = logger
-            
-        self.lvl = level_to_int(lvl)
-
-    def write(self, obj):
-        for f in self.files:
-            f.write(obj)
-        self.logger.log(self.lvl, obj)
-        
-    def flush(self):
-        pass
-    
-    
-class TKConsoleHandler(logging.Handler):
-    # This class allows you to log to a Tkinter Text or ScrolledText widget
-    # Adapted from Moshe Kaplan: https://gist.github.com/moshekaplan/c425f861de7bbf28ef06
-
-    def __init__(self, text):
-        import tkinter as tk
-        
-        logging.Handler.__init__(self)
-        self.setFormatter(FonsFormatter(_default_fmt))
-        self.text = text
-        self._tk = tk
-        
-
-    def emit(self, record):
-        msg = self.format(record)
-        def append():
-            self.text.configure(state='normal')
-            self.text.insert(self._tk.END, msg + '\n')
-            self.text.configure(state='disabled')
-            # Autoscroll to the bottom
-            self.text.yview(self._tk.END)
-        # This is necessary because we can't modify the Text from other threads
-        self.text.after(0, append)
-
-        if self.num_lines() > NR_CONSOLE_LINES:
-            self.clear_log()
-
-    def num_lines(self):
-        return int(self.text.index('end').split('.')[0]) - 1
-
-    def clear_log(self):
-        self.text.configure(state='normal')
-        self.text.delete(1.0, 2.0) #tk.END)
-        self.text.configure(state='disabled')
-
-
-def _create_logiGUI_class():
-    import tkinter as tk
-    
-    class LogiGUI(tk.Frame):
-        def __init__(self, parent, *args, loggers=[], **kwargs):
-            tk.Frame.__init__(self, parent, *args, **kwargs)
-            self.root = parent
-            if loggers is None:
-                loggers = []
-            elif isinstance(loggers,str):
-                loggers = [loggers]
-            self.loggers = loggers
-            self.build_gui()
-    
-        def build_gui(self):
-            from tkinter.scrolledtext import ScrolledText
-            # Build GUI
-            #self.root.title(self.l_name)
-            self.root.option_add('*tearOff', 'FALSE')
-            self.grid(column=0, row=0, sticky='nesw')
-            self.grid_columnconfigure(0, weight=1, uniform='a')
-            self.grid_columnconfigure(1, weight=1, uniform='a')
-            self.grid_columnconfigure(2, weight=1, uniform='a')
-            self.grid_columnconfigure(3, weight=1, uniform='a')
-    
-            # Add text widget to display logging info
-            st = ScrolledText(self, state='disabled')
-            st.configure(font='TkFixedFont')
-            #.grid didn't expand vertically for some reason
-            #st.grid(column=0, row=1, sticky='nesw', columnspan=4)
-            st.pack(fill="both", expand=True)
-            
-            # Create textLogger
-            self.text_handler = TKConsoleHandler(st)     
-    
-            # Add the handler to logger
-            for l in self.loggers:
-                logger = l if isinstance(l,logging.Logger) else logging.getLogger(l)      
-                logger.addHandler(self.text_handler)
-    
-    return LogiGUI
-
-
-class LogListener(threading.Thread):
-    def __init__(self, queue):
-        super().__init__(name='LogListener', daemon=True)
-        self.queue = queue
-        
-    def run(self):
-        logger.info('Starting LogListener in \'{}\''.format(multiprocessing.current_process().name))
-        while True:
-            try:
-                record = self.queue.get()
-                if record is None:  # We send this as a sentinel to tell the listener to quit.
-                    break
-                self.handle(record)
-            except Exception:
-                print('Whoops! Problem:', file=sys.stderr)
-                traceback.print_exc(file=sys.stderr)
-                
-    def handle(self, record):
-        p_name = multiprocessing.current_process().name
-        if not hasattr(record,'p_history'):
-            record.p_history = [record.processName]
-        
-        #ordinary child process (non_tkLogiProcess) of main
-        record_is_main = record.processName == 'MainProcess'
-        isin_tk0 = record.p_history[0] in _tklogiprocesses
-        
-        #if we are not in main process or this is non-tk process, we want to record its name
-        if (p_name != 'MainProcess' or record.p_history[0] not in _tklogiprocesses) and record.p_history[0] != p_name:
-            #if (p_name != 'MainProcess') and p_name not in record.p_history:
-            record.p_history.insert(0,p_name)
-        
-        isin_tk = record.p_history[0] in _tklogiprocesses
-        """if not isinstance(logging.root.handlers[0],QueueHandler):
-            print('Received from: {}, Handling: "{}"'.format(record.processName,record.message))#logging.root.handlers[0].format(record)))"""
-
-        display = (record.name in STREAMING_LOGGERS or record.name=='stdout' or p_name==record.processName and 
-                 any(isinstance(x,logging.StreamHandler) for x in logging.getLogger(record.name).handlers))
-        
-        if isin_tk and display:
-            gui_handler = _tklogiprocesses[record.p_history[0]].text_handler
-            gui_handler.emit(record)
-        #we do not want to cause recursive loop 
-        # (if _tklogiprocesses is inited, the logging.root.handlers may contain self.queue 
-        #   [due to 'main' process also having gui notebook], but any other "not-TkLogiProcess" is *not* registered into
-        #  the _tklogiprocesses, with the elif check removed causing infinite recursion;
-        # --although any-non_tklogiprocess will have "MainProcess" as record.p_history[0], which should also ensure eliminate recursion,
-        # -- thus the below is just as a precaution for unforeseen situations (when _gui is located in a child process?))
-        
-        if not record_is_main and not isin_tk0:
-            _logger = logging.getLogger(record.name)
-            #add [self.queue] to eliminate possibility of recursion
-            _logger.handle(record, declude_with_queues=[self.queue])
-            
-        """if '*' in _tklogiprocesses and display:
-            _tklogiprocesses['*'].text_handler.emit(record)"""
-        for i,lname in enumerate(('debug*','info*','warning*','error*','critical*')):
-            if record.levelno < (i+1)*10: break
-            elif lname in _tklogiprocesses:
-                _tklogiprocesses[lname].text_handler.emit(record)
-            
-
-def start_listener():
-    global _listener
-    with _lock:
-        if _globals['queue'] is None: 
-            warnings.warn('u_log._queue is set to `None`. Cannot start LogListener.')
-        if _listener is None:
-            _listener = LogListener(_globals['queue'])
-            _listener.start()
-
-
-def init_tab(nb, processName):
-    """:type nb: tkinter.ttk.Notebook"""
-    LogiGUI = _create_logiGUI_class()
-    fr = LogiGUI(nb)
-    _tklogiprocesses[processName] = fr
-    if _globals['queue'] is None: pass
-    elif (processName == 'MainProcess' and not any(isinstance(x,QueueHandler) and
-         x.queue is _globals['queue'] for x in logging.root.handlers)):
-        logging.root.addHandler(QueueHandler(_globals['queue']))
-    text = processName if processName != 'MainProcess' else 'main'
-    nb.add(fr,text=text)
-    #in case it hasn't been started yet
-    start_listener()
-
-
-def init_main_tab(nb):
-    """:type nb: tkinter.ttk.Notebook"""
-    init_tab(nb,'MainProcess')
-
-
-def remove_stream_handlers(logger):
-    for h in logger.handlers[:]:
-        # FileHandler is subclass of StreamHandler, but here we mean handlers streaming to console
-        if isinstance(h, logging.StreamHandler) and not isinstance(h, logging.FileHandler):
-            logger.handlers.remove(h)
-
-
-def level_to_int(lvl):
-    return lvl if isinstance(lvl,int) else getattr(logging,lvl.upper())
-    #raise TypeError('Level must be either of type <str> or <int>, got {}'.format(type(lvl)))
-
-#--------------------------------------------
-                    
-def multi_module_logging(modules, names, loggers):
-    for mod in modules:
-        if isinstance(mod,str):
-            mod = sys.modules[mod]
-            
-        for name,logger in zip(names,loggers):
-            if not isinstance(mod,dict):
-                setattr(mod,name,logger)
-            else: mod.update({name:logger})
-            
-
-def standard_logging(dir=None, f_ending=None, TEST_MODE=False, modules=None, **kw):
-    """A standardized logging to file"""
-    global _sys_stdout_assigned
-    backup = sys.stdout
-    if dir is None:
-        dpath = kw.get('dpath')
-        if dpath is None:
-            dir = DEFAULT_ROOT_DIR
-        else:
-            dir = os.path.join(dpath,'logs','other')
-        if TEST_MODE:
-            dir += '_TM'
-        os.makedirs(dir, exist_ok=True)
-
-
-    if TEST_MODE and isinstance(f_ending, str) and not f_ending.endswith('_TM'):
-        f_ending += '_TM'
-        
-    params = {'dir': dir,
-              'lvl': 'DEBUG',
-              'use_FonsFormatter':True,
-              'pair_with_fwriters': [sys.stdout],
-              'f_ending': f_ending,
-              'lvl_handlers': ['WARNING', {'lvl': 'INFO', 'use_rotating': True}],
-              'use_rotating':True,
-              'maxBytes':5*1024*1024,
-              'backupCount':5}
-    
-    params.update({k:v for k,v in kw.items() if k in params})
-
-    #--
-    writer = setup_logging(**params)
-    #--
-    
-    if _sys_stdout_assigned: pass
-    elif any(x in params['pair_with_fwriters'] for x in ('sys.stdout',sys.stdout)):
-        sys.stdout = writer
-        _sys_stdout_assigned = True
-    
-    standard_5 = _init_standard_5(TEST_MODE)
-    
-    if modules is not None:
-        for mod in modules:
-            add_module(mod)
-            
-    multi_module_logging(_modules, standard_5._fields, standard_5)
-    
-    _globals.update({
-        #'queue': queue,
-        'TEST_MODE': TEST_MODE,
-        'level': params['lvl'],
-        'use_FonsFormatter': params['use_FonsFormatter'],
-        'fmt': kw.get('fmt')})
-    
-    return standard_5
-
-
-def quick_logging(test=2, add_stream_handlers=False):
-    if add_stream_handlers:
-        remove_stream_handlers(logging.root) # to avoid duplicate streaming
-    else:
-        for _logger in standard_5:
-            remove_stream_handlers(_logger)
-        logging.basicConfig(level=10) # stream via root handler
-    
-    for i,_logger in enumerate(standard_5):
-        level = 10 if i < (2 + test) else 0
-        getFonsLogger(_logger.name, level, add_stream_handlers)
-
-
-def standard_mp_logging(queue, level='INFO', fmt=None, use_FonsFormatter=True, TEST_MODE=False):
-    global _sys_stdout_assigned, _mp_logging_enabled
-    _mp_logging_enabled = True
-
-    if fmt is None:
-        fmt = _default_fmt
-    if use_FonsFormatter:
-        logging.Formatter = FonsFormatter
-    
-    try: _modules[_modules.index('__main__')] = '__mp_main__'
-    except ValueError: pass
-    
-    standard_5 = _init_standard_5(TEST_MODE, False)
-    """print('standard_mp_logging')
-    print(_modules)
-    print([m in sys.modules for m in _modules])
-    print(list(sys.modules)[:20])"""
-    multi_module_logging(_modules, standard_5._fields, standard_5)
-    
-    for h in logging.root.handlers[:]:
-        logging.root.removeHandler(h)
-        
-    logging.basicConfig(level=level,
-                        handlers=[QueueHandler(queue)],
-                        format=fmt)
-    #print('_queue is queue: {}'.format(_queue is queue))
-    _sys_stdout_assigned = True
-    #let's remove sys.stdout altogether (since parent process will print the 'stdout' logger output anyway)
-    sys.stdout = Tee([]) #sys.stdout 
-    """print(sys.modules['__mp_main__'].logger2,sys.modules['__mp_main__'].logger2.name)"""
-
-
-def get_standard_logger(name=None):
-    if name is None:
-        return standard_5[0]
-    
-    elif isinstance(name,int):
-        return standard_5[name]
-    
-    return getattr(standard_5,name)
-
-
-def get_standard_5(module=None):
-    if module is not None:
-        add_module(module)
-        
-    return standard_5
-
-
-def add_module(module):
-    if module not in _modules:
-        _modules.append(module)
-        
-
-def _init_standard_5(TEST_MODE, stream_enabled=None):
-    if stream_enabled is None: 
-        stream_enabled = not _mp_logging_enabled
-    logger = getFonsLogger('L1',streams=False)
-    logger2 = getFonsLogger('L2',streams=stream_enabled)
-    
-    tlogger = getFonsLogger('T1',streams=False) #logger
-    tloggers = getFonsLogger('T2',streams=stream_enabled) #logger2
-    tlogger0 = getFonsLogger('T0',0,streams=False)
-    
-    if not TEST_MODE:
-        [x.setLevel(0) for x in (tlogger,tloggers,tlogger0)]
-    
-    global standard_5
-    standard_5 = _Standard_5(logger,logger2,tlogger,tloggers,tlogger0)
-    
-    return standard_5
-
-#--------------------------------------------
-
-    
-def setup_logging(dir=None, lvl='INFO', pair_with_fwriters=[],
-                  fname=None, f_ending=None, lvl_handlers=[],
-                  use_rotating=True, maxBytes=5*1024*1024, filemode='a',
-                  backupCount=2, fmt=None, use_FonsFormatter=True):
-    """Attaches file handlers to root logger"""
-    if dir is None:
-        dir = ''
-
-    if not fname:
-        fname = dt.utcnow().strftime('%Y-%m-%dT%H-%M-%S')
-    if f_ending: fname += "_" + f_ending
-    
-    if dir is not False:
-        dir = os.path.join(dir,fname)
-        if not os.path.exists(dir):
-            os.mkdir(dir)
-    
-    
-    if not fname.endswith('.log'):
-        fname += '.log'
-    
-    
-    if use_FonsFormatter:
-        logging.Formatter = FonsFormatter
-    
-    if not fmt:
-        fmt = _default_fmt
-    
-    
-    lvl_handlers = lvl_handlers[:]
-    
-    if not any(isinstance(L,dict) and level_to_int(L.get('lvl',L.get('level'))) == level_to_int(lvl)
-               or not isinstance(L,dict) and level_to_int(L) == level_to_int(lvl) for L in lvl_handlers):
-        lvl_handlers.append(lvl)
-    
-    # Removes all previous handlers 
-    # (e.g. if logging.log() called before setup_logging, 
-    #  it automatically adds StreamHandler, and basicConfig(handlers=handlers) won't add the new handlers)
-    keep_handlers = [x for x in logging.root.handlers if isinstance(x,QueueHandler)]
-    for handler in logging.root.handlers[:]:
-        logging.root.removeHandler(handler)
-    
-    handlers = []
-    
-    for L in lvl_handlers:
-        if dir is False:
-            break
-        if not isinstance(L,dict):
-            L={'lvl': L}
-
-        h_lvl = L.get('lvl', L.get('level'))
-        if isinstance(h_lvl,str):
-            h_lvl = h_lvl.upper()
-
-        #h_rotating = L.get('use_rotating',[True,False][level_to_int(h_lvl) > 30])
-        h_filemode = L.get('filemode', filemode)
-        h_backupCount = L.get('backupCount', backupCount)
-        h_max_size = L.get('maxBytes', maxBytes)
-
-            
-        fpth = os.path.join(dir, fname[:-4] + '_{}.log'.format(h_lvl))
-        if use_rotating:
-            h = RotatingFileHandler(fpth, mode=h_filemode, maxBytes=h_max_size, 
-                                     backupCount=h_backupCount, encoding='utf-8', delay=0)
-        else:
-            h = logging.FileHandler(fpth,mode=h_filemode)
-        h.setLevel(h_lvl)
-        
-        handlers.append(h)
-    
-    handlers += keep_handlers
-    
-    logging.basicConfig(#filename=fpath,
-                        format = fmt,
-                        #filemode=filemode,
-                        handlers=handlers,
-                        level=level_to_int(lvl))#,\
-                        #datefmt = '%Y-%m-%dT%H:%M:%S')
-    
-
-    if len(pair_with_fwriters):
-        synched_writer = Tee(pair_with_fwriters, lvl, logging)
-        return synched_writer
-
-
-
-if __name__ == '__main__':
-    logger.debug('first output (from L1)')
-    logdir = os.path.join('_test')
-    backup = sys.stdout
-    # Strange discovery:
-    #  if logging.log used before initiating handlers, handlers will be void 
-    #  (everything is directed to logging module instead of handler)
-    # Don't do:
-    print('Handlers 0: {}'.format(logging.root.handlers)) # []
-    logging.warning('HERE (from root)')
-    print('Handlers now: {}'.format(logging.root.handlers)) # [<StreamHandler <stderr> (NOTSET)>]
-    logger.debug('HERE (from L1)')
-    logging2,sys.stdout = setup_logging(logdir,
-                                      lvl='INFO',
-                                      #lvl_handlers =  [{'lvl':'INFO','maxBytes':0.5*1024*1024},{'lvl':'WARNING','use_rotating':True},'CRITICAL'],
-                                      use_rotating=True,
-                                      use_FonsFormatter=True,
-                                      pair_with_fwriters=[sys.stdout],
-                                      f_ending='main',
-                                      filemode='a',
-                                      maxBytes = 5242880,
-                                      backupCount = 5)
-    
-    print('Handlers after setup: {}'.format(logging2.root.handlers))
-    
-    logger = getFonsLogger('L1',streams=False)
-    logger2 = getFonsLogger('L2',streams=True)
-    logger.info('LOGGER!')
-    logger2.info('LOGGER2!')
-    
-    print('Handlers final: {}'.format(logging.root.handlers))
-    
+# Note: alternatives to logging
+#  - https://eliot.readthedocs.io/en/stable/introduction.html
+#  - https://www.structlog.org/en/stable/
+"""
+How python logging works?
+
+By default, only >=WARNING is printed out (without needing to call logging.basicConfig())
+  logger, logger2, ... have "DEBUG" set, and also don't need logging.basicConfig()
+
+when logging.basicConfig is called, it adds a StreamHandler to root logger, and a formatter (metadata includer) to that streamHandler
+ - now all loggers will print to console (bc every logger has rootLogger set as parent), and duplicate the output if they already
+   have a StreamHandler attached
+
+Manager stores all the loggers
+
+PROBLEMS:
+ 1. with pytest you need to add StreamHandler to all the loggers you want to print out anything at all
+     (this isn't fons.log specific; any logger fails)
+   solution_1: can be initiated with `quick_logging(test=2, add_stream_handlers=True)`
+   solution_2: use --log-cli-level=DEBUG   # https://docs.pytest.org/en/7.1.x/how-to/logging.html
+"""
+import datetime
+
+dt = datetime.datetime
+import time
+import sys, os, io
+from collections import namedtuple
+import traceback
+import threading
+import multiprocessing
+import warnings
+import yaml
+import platform
+import logging
+from logging.handlers import RotatingFileHandler, QueueHandler
+
+OldLoggingFormatter = logging.Formatter
+
+if sys.version_info[1] < 8:
+    from .log35 import FonsLogger
+elif sys.version_info[1] < 11:
+    from .log38 import FonsLogger
+else:
+    from .log311 import FonsLogger
+
+
+class EmptyLogger:
+    def debug(self, msg, *args, **kwargs):
+        pass
+
+    def info(self, msg, *args, **kwargs):
+        pass
+
+    def warn(self, msg, *args, **kwargs):
+        pass
+
+    def warning(self, msg, *args, **kwargs):
+        pass
+
+    def error(self, msg, *args, **kwargs):
+        pass
+
+    def exception(self, msg, *args, exc_info=True, **kwargs):
+        pass
+
+    def critical(self, msg, *args, **kwargs):
+        pass
+
+    def log(self, level, msg, *args, **kwargs):
+        pass
+
+
+SETTINGS_PATH = os.path.abspath(
+    os.path.join(os.path.join(__file__, ".."), "settings.yaml")
+)
+
+
+def _read_settings():
+    if os.path.exists(SETTINGS_PATH):
+        with open(SETTINGS_PATH, encoding="utf-8") as f:
+            return yaml.safe_load(f)
+    else:
+        return {}
+
+
+def _save_settings(d, mode="a"):
+    if mode not in ("a", "w"):
+        raise ValueError(mode)
+    d_prev = {}
+    if mode == "a":
+        d_prev = _read_settings()
+    d_prev.update(d)
+    with open(SETTINGS_PATH, "w", encoding="utf-8") as f:
+        yaml.dump(d_prev, f)
+
+
+def _read_root_dir():
+    root_dir = ""
+    d = _read_settings()
+    if d.get("logging_default_root_dir") is not None:
+        root_dir = d["logging_default_root_dir"]
+        if platform.system() != "Windows":
+            root_dir = os.path.expanduser(root_dir)
+    if not isinstance(root_dir, str):
+        raise TypeError(
+            "Logging root dir in settings file must be of type <str>, got: {}".format(
+                type(root_dir)
+            )
+        )
+    return root_dir
+
+
+def set_default_root_dir(path, make_permanent=False):
+    """
+    Set the default directory where file handlers will output their files
+    (=='dir' param in functions 'standard_logging' and 'setup_logging').
+    :param make_permanent:
+        if True, writes to settings file (will keep defaulting to that during
+        the future python instances)
+    """
+    global DEFAULT_ROOT_DIR
+    if not isinstance(path, str):
+        raise TypeError(type(path))
+    DEFAULT_ROOT_DIR = path
+    if make_permanent:
+        _save_settings({"logging_default_root_dir": path}, "a")
+
+
+# '' will later resolve to current working directory
+DEFAULT_ROOT_DIR = _read_root_dir()
+
+logging._srcfile2 = os.path.normcase(FonsLogger.findCaller.__code__.co_filename)
+
+# For excluding this module from Logger's record (like logging module does)
+# and fixing infinite recursion caused by LogListener trying to handle
+# QueueHandler's record (this won't affect user defined QueueHandlers)
+logging.Logger.findCaller = FonsLogger.findCaller
+logging.Logger.handle = FonsLogger.handle
+logging.Logger.callHandlers = FonsLogger.callHandlers
+
+# The old rootLogger's class RootLogger (subclass of Logger) hasn't been updated to
+# include the new methods attached to Logger above
+# Q: What happens to module-level loggers already initiated?
+# A: ?they should work? .root is a class variable of Logger, it isn't attached to
+#    each instance separately (not ro Logger.manager.root)
+_rhandlers, _rfilters = logging.root.handlers, logging.root.filters
+logging.root = logging.RootLogger(logging.root.level)
+logging.root.handlers = _rhandlers
+logging.root.filters = _rfilters
+
+logging.Logger.root = logging.root
+logging.Logger.manager.root = logging.root
+# Can't reinitiate (nor need to) the manager itself, as it's attached to
+# each Logger instance individually
+
+NR_CONSOLE_LINES = 300
+STREAMING_LOGGERS = ["L2", "T2"]
+
+_is_logger_overwritten = False
+_default_fmt = (
+    # "%(asctime)s:%(name)s:%(levelname)s:%(module)s:%(funcName)s(%(lineno)d):%(message)s"
+    # "%(asctime)s %(name)-2s %(levelname)-2s %(module)-2s %(funcName)-2s(%(lineno)d) :: %(message)s"
+    "%(asctime)s %(name)s %(levelname)s %(module)s:%(funcName)s(%(lineno)d) :: %(message)s"
+)
+_queue = multiprocessing.Queue(-1)
+_lock = multiprocessing.Lock()
+_globals = {
+    "queue": _queue,
+    "TEST_MODE": False,
+    "level": "INFO",
+    "fmt": None,
+    "use_FonsFormatter": True,
+}
+
+_modules = [__name__]
+_tklogiprocesses = {}
+_sys_stdout_assigned = False
+_mp_logging_enabled = False
+_listener = None
+
+_s5_names = {
+    "logger": "L1",
+    "logger2": "L2",
+    "tlogger": "T1",
+    "tloggers": "T2",
+    "tlogger0": "T0",
+}
+_Standard_5 = namedtuple(
+    "StandardLogging_5", "logger logger2 tlogger tloggers tlogger0"
+)
+_Standard_5.__new__.__defaults__ = tuple(
+    logging.getLogger(_s5_names[x]) for x in _Standard_5._fields
+)
+
+standard_5 = _Standard_5()
+
+# The difference between logger and logger2 (and tlogger / tloggers) is that after calling setup_logging(),
+# logger2 (and tloggers) will *also* stream to console, while logger (and tlogger, tlogger0) only stream to file
+logger = standard_5.logger  # level = 10
+logger2 = standard_5.logger2  # ...
+tlogger = standard_5.tlogger  # level = 0
+tloggers = standard_5.tloggers  # ...
+tlogger0 = standard_5.tlogger0  # ...
+
+
+for _logger in standard_5[:2]:
+    _logger.setLevel(10)
+# Set test loggers' level to 0
+for _logger in standard_5[2:]:
+    _logger.setLevel(0)
+
+
+class TempStreamHandler(logging.StreamHandler):
+    """
+    Only stream if root has not handlers set (to avoid duplication)
+    """
+
+    def handle(self, record):
+        if not logging.root.handlers and not _mp_logging_enabled:
+            return logging.StreamHandler.handle(self, record)
+
+
+# We want the logger and logger2 to stream only if user has not called basicConfig(),
+# and revoke the streaming when user decides to call it later
+if not logging.root.handlers and not _mp_logging_enabled:
+    _h = TempStreamHandler()
+    _h.setFormatter(logging.Formatter(logging.BASIC_FORMAT))
+    logger.addHandler(_h)
+    logger2.addHandler(_h)
+
+
+# ----------------------------------------------
+
+
+class FonsFormatter(logging.Formatter):
+    converter = dt.utcfromtimestamp
+
+    def formatTime(self, record, datefmt=None):
+        ct = self.converter(record.created)
+        if datefmt:
+            s = ct.strftime(datefmt)
+        else:
+            t = ct.strftime("%Y-%m-%dT%H:%M:%S")
+            s = "%s.%03d" % (t, record.msecs)
+
+        return s
+
+
+class FonsFormatter2(logging.Formatter):
+    converter = time.gmtime
+    default_time_format = "%Y-%m-%d %H:%M:%S"
+    defualt_msec_format = "%s.%03d"
+
+
+def initiate_FonsFormat():
+    logging.Formatter = FonsFormatter
+
+
+# -------------------------------------------
+
+
+def getFonsLogger(
+    name=None, lvl="DEBUG", streams=True, fmt=None, use_FonsFormatter=True
+):
+    """Initiate a logger.
+    :param streams: if True, adds StreamHandler with default or specified format
+    """
+    if name is None:
+        name = __name__
+    logger = logging.getLogger(name)
+    logger.setLevel(lvl)
+
+    if fmt is None:
+        fmt = _default_fmt
+    elif fmt == "simpleformat":
+        fmt = "%(asctime)s %(message)s"
+
+    remove_stream_handlers(logger)
+
+    if streams:
+        stream_handler = logging.StreamHandler()  # prints to console
+        formatter_cls = FonsFormatter if use_FonsFormatter else OldLoggingFormatter
+
+        formatter = formatter_cls(fmt=fmt)
+        stream_handler.setFormatter(formatter)
+
+        logger.addHandler(stream_handler)
+
+    """if queue is not None:
+        logger.addHandler(QueueHandler(queue))"""
+
+    return logger
+
+
+class Tee(object):
+    """
+    Replace the sys.stdout with this object, pass the original as files=[sys.stdout]
+     - will write to all the "files" it was initialized with (e.g. original sys.stdout)
+     - log to the logger it was initiated with (e.g. L2)
+    I.e. it syncs the original output to multiple streams and logs it to a logger
+    """
+
+    def __init__(self, files=[], lvl=logging.INFO, logger=None):
+        self.files = files
+
+        if logger is None:
+            self.logger = getFonsLogger(
+                "stdout",
+                streams=False,
+                fmt=_globals["fmt"],
+                use_FonsFormatter=_globals["use_FonsFormatter"],
+            )
+        else:
+            self.logger = logger
+
+        self.lvl = level_to_int(lvl)
+
+    def write(self, obj):
+        for f in self.files:
+            f.write(obj)
+        self.logger.log(self.lvl, obj)
+
+    def flush(self):
+        pass
+
+
+class TKConsoleHandler(logging.Handler):
+    # This class allows you to log to a Tkinter Text or ScrolledText widget
+    # Adapted from Moshe Kaplan: https://gist.github.com/moshekaplan/c425f861de7bbf28ef06
+
+    def __init__(self, text):
+        import tkinter as tk
+
+        logging.Handler.__init__(self)
+        self.setFormatter(FonsFormatter(_default_fmt))
+        self.text = text
+        self._tk = tk
+
+    def emit(self, record):
+        msg = self.format(record)
+
+        def append():
+            self.text.configure(state="normal")
+            self.text.insert(self._tk.END, msg + "\n")
+            self.text.configure(state="disabled")
+            # Autoscroll to the bottom
+            self.text.yview(self._tk.END)
+
+        # This is necessary because we can't modify the Text from other threads
+        self.text.after(0, append)
+
+        if self.num_lines() > NR_CONSOLE_LINES:
+            self.clear_log()
+
+    def num_lines(self):
+        return int(self.text.index("end").split(".")[0]) - 1
+
+    def clear_log(self):
+        self.text.configure(state="normal")
+        self.text.delete(1.0, 2.0)  # tk.END)
+        self.text.configure(state="disabled")
+
+
+def _create_logiGUI_class():
+    import tkinter as tk
+
+    class LogiGUI(tk.Frame):
+        def __init__(self, parent, *args, loggers=[], **kwargs):
+            tk.Frame.__init__(self, parent, *args, **kwargs)
+            self.root = parent
+            if loggers is None:
+                loggers = []
+            elif isinstance(loggers, str):
+                loggers = [loggers]
+            self.loggers = loggers
+            self.build_gui()
+
+        def build_gui(self):
+            from tkinter.scrolledtext import ScrolledText
+
+            # Build GUI
+            # self.root.title(self.l_name)
+            self.root.option_add("*tearOff", "FALSE")
+            self.grid(column=0, row=0, sticky="nesw")
+            self.grid_columnconfigure(0, weight=1, uniform="a")
+            self.grid_columnconfigure(1, weight=1, uniform="a")
+            self.grid_columnconfigure(2, weight=1, uniform="a")
+            self.grid_columnconfigure(3, weight=1, uniform="a")
+
+            # Add text widget to display logging info
+            st = ScrolledText(self, state="disabled")
+            st.configure(font="TkFixedFont")
+            # .grid didn't expand vertically for some reason
+            # st.grid(column=0, row=1, sticky='nesw', columnspan=4)
+            st.pack(fill="both", expand=True)
+
+            # Create textLogger
+            self.text_handler = TKConsoleHandler(st)
+
+            # Add the handler to logger
+            for l in self.loggers:
+                logger = l if isinstance(l, logging.Logger) else logging.getLogger(l)
+                logger.addHandler(self.text_handler)
+
+    return LogiGUI
+
+
+class LogListener(threading.Thread):
+    """
+    Handle incloming log records from queue, forwarded by child process'
+    only handler: QueueHandler
+    """
+
+    def __init__(self, queue):
+        super().__init__(name="LogListener", daemon=True)
+        self.queue = queue
+
+    def run(self):
+        logger.info(
+            "Starting LogListener in '{}'".format(
+                multiprocessing.current_process().name
+            )
+        )
+        while True:
+            try:
+                record = self.queue.get()
+                if (
+                    record is None
+                ):  # We send this as a sentinel to tell the listener to quit.
+                    break
+                self.handle(record)
+            except Exception:
+                print("Whoops! Problem:", file=sys.stderr)
+                traceback.print_exc(file=sys.stderr)
+
+    def handle(self, record):
+        try:
+            # Since some python version (3.8?) the QueueHandler seems to already pre-modify the
+            # record's message into its log-output formatted form. We have to strip it
+            msg = record.getMessage()
+            # format the message of the record using rootLogger handler's formatter
+            formatter = logging.root.handlers[0].formatter
+            new_msg = formatter.format(record)
+            added_msg = new_msg[: -len(msg)]
+            if msg[: len(added_msg)] == added_msg:
+                record.msg = msg[len(added_msg) :]
+        except Exception:
+            # traceback.print_exc(file=sys.stderr)
+            pass
+
+        p_name = multiprocessing.current_process().name
+        if not hasattr(record, "p_history"):
+            record.p_history = [record.processName]
+
+        # ordinary child process (non_tkLogiProcess) of main
+        record_is_main = record.processName == "MainProcess"
+        isin_tk0 = record.p_history[0] in _tklogiprocesses
+
+        # if we are not in main process or this is non-tk process, we want to record its name
+        if (
+            p_name != "MainProcess" or record.p_history[0] not in _tklogiprocesses
+        ) and record.p_history[0] != p_name:
+            # if (p_name != 'MainProcess') and p_name not in record.p_history:
+            record.p_history.insert(0, p_name)
+
+        isin_tk = record.p_history[0] in _tklogiprocesses
+        """if not isinstance(logging.root.handlers[0],QueueHandler):
+            print('Received from: {}, Handling: "{}"'.format(record.processName,record.message))#logging.root.handlers[0].format(record)))"""
+
+        display = (
+            record.name in STREAMING_LOGGERS
+            or record.name == "stdout"
+            or p_name == record.processName
+            and any(
+                isinstance(x, logging.StreamHandler)
+                for x in logging.getLogger(record.name).handlers
+            )
+        )
+
+        if isin_tk and display:
+            gui_handler = _tklogiprocesses[record.p_history[0]].text_handler
+            gui_handler.emit(record)
+        # we do not want to cause recursive loop
+        # (if _tklogiprocesses is inited, the logging.root.handlers may contain self.queue
+        #   [due to 'main' process also having gui notebook], but any other "not-TkLogiProcess" is *not* registered into
+        #  the _tklogiprocesses, with the elif check removed causing infinite recursion;
+        # --although any-non_tklogiprocess will have "MainProcess" as record.p_history[0], which should also ensure eliminate recursion,
+        # -- thus the below is just as a precaution for unforeseen situations (when _gui is located in a child process?))
+
+        if not record_is_main and not isin_tk0:
+            """
+            # for debugging:
+            writer = (
+                sys.stdout if not isinstance(sys.stdout, Tee) else sys.stdout.files[0]
+            )
+            writer.write(repr(record))"""
+            _logger = logging.getLogger(record.name)
+            # add [self.queue] to eliminate possibility of recursion
+            _logger.handle(record, declude_with_queues=[self.queue])
+
+        """if '*' in _tklogiprocesses and display:
+            _tklogiprocesses['*'].text_handler.emit(record)"""
+        for i, lname in enumerate(
+            ("debug*", "info*", "warning*", "error*", "critical*")
+        ):
+            if record.levelno < (i + 1) * 10:
+                break
+            elif lname in _tklogiprocesses:
+                _tklogiprocesses[lname].text_handler.emit(record)
+
+
+def start_listener():
+    global _listener
+    with _lock:
+        if _globals["queue"] is None:
+            warnings.warn("u_log._queue is set to `None`. Cannot start LogListener.")
+        if _listener is None:
+            _listener = LogListener(_globals["queue"])
+            _listener.start()
+
+
+def init_tab(nb, processName):
+    """:type nb: tkinter.ttk.Notebook"""
+    LogiGUI = _create_logiGUI_class()
+    fr = LogiGUI(nb)
+    _tklogiprocesses[processName] = fr
+    if _globals["queue"] is None:
+        pass
+    elif processName == "MainProcess" and not any(
+        isinstance(x, QueueHandler) and x.queue is _globals["queue"]
+        for x in logging.root.handlers
+    ):
+        logging.root.addHandler(QueueHandler(_globals["queue"]))
+    text = processName if processName != "MainProcess" else "main"
+    nb.add(fr, text=text)
+    # in case it hasn't been started yet
+    start_listener()
+
+
+def init_main_tab(nb):
+    """:type nb: tkinter.ttk.Notebook"""
+    init_tab(nb, "MainProcess")
+
+
+def remove_stream_handlers(logger):
+    for h in logger.handlers[:]:
+        # FileHandler is subclass of StreamHandler, but here we mean handlers streaming to console
+        if isinstance(h, logging.StreamHandler) and not isinstance(
+            h, logging.FileHandler
+        ):
+            logger.handlers.remove(h)
+
+
+def level_to_int(lvl):
+    return lvl if isinstance(lvl, int) else getattr(logging, lvl.upper())
+    # raise TypeError('Level must be either of type <str> or <int>, got {}'.format(type(lvl)))
+
+
+# --------------------------------------------
+
+
+def multi_module_logging(modules, names, loggers):
+    for mod in modules:
+        if isinstance(mod, str):
+            mod = sys.modules[mod]
+
+        for name, logger in zip(names, loggers):
+            if not isinstance(mod, dict):
+                setattr(mod, name, logger)
+            else:
+                mod.update({name: logger})
+
+
+def standard_logging(dir=None, f_ending=None, TEST_MODE=False, modules=None, **kw):
+    """A standardized logging to file"""
+    global _sys_stdout_assigned
+    backup = sys.stdout
+    if dir is None:
+        dpath = kw.get("dpath")
+        if dpath is None:
+            dir = DEFAULT_ROOT_DIR
+        else:
+            dir = os.path.join(dpath, "logs", "other")
+        if TEST_MODE:
+            dir += "_TM"
+        os.makedirs(dir, exist_ok=True)
+
+    if TEST_MODE and isinstance(f_ending, str) and not f_ending.endswith("_TM"):
+        f_ending += "_TM"
+
+    params = {
+        "dir": dir,
+        "lvl": "DEBUG",
+        "use_FonsFormatter": True,
+        "pair_with_fwriters": [sys.stdout],
+        "f_ending": f_ending,
+        "lvl_handlers": ["WARNING", {"lvl": "INFO", "use_rotating": True}],
+        "use_rotating": True,
+        "maxBytes": 5 * 1024 * 1024,
+        "backupCount": 5,
+    }
+
+    params.update({k: v for k, v in kw.items() if k in params})
+
+    # --
+    writer = setup_logging(**params)
+    # --
+
+    if _sys_stdout_assigned:
+        pass
+    elif any(x in params["pair_with_fwriters"] for x in ("sys.stdout", sys.stdout)):
+        sys.stdout = writer
+        _sys_stdout_assigned = True
+
+    standard_5 = _init_standard_5(TEST_MODE)
+
+    if modules is not None:
+        for mod in modules:
+            add_module(mod)
+
+    multi_module_logging(_modules, standard_5._fields, standard_5)
+
+    _globals.update(
+        {
+            #'queue': queue,
+            "TEST_MODE": TEST_MODE,
+            "level": params["lvl"],
+            "use_FonsFormatter": params["use_FonsFormatter"],
+            "fmt": kw.get("fmt"),
+        }
+    )
+
+    return standard_5
+
+
+def quick_logging(test=2, add_stream_handlers=False):
+    """
+    Add level "DEBUG" to all standard_5 loggers, and also to test loggers if test > 0
+    "If no stream handlers are added, it'll stream via root logger
+    """
+    if add_stream_handlers:
+        # To avoid duplicate streaming
+        remove_stream_handlers(logging.root)
+    else:
+        for _logger in standard_5:
+            remove_stream_handlers(_logger)
+        logging.basicConfig(level=10)  # stream via root handler
+
+    # Initiate the levels and handlers for the standard 5
+    for i, _logger in enumerate(standard_5):
+        level = 10 if i < (2 + test) else 0
+        getFonsLogger(_logger.name, level, streams=add_stream_handlers)
+
+
+def standard_mp_logging(
+    queue, level="INFO", fmt=None, use_FonsFormatter=True, TEST_MODE=False
+):
+    """
+    This will be called by LogiProcess.run(), the params (incl `queue`) passed
+    from the parent process' `_globals`
+    """
+    global _sys_stdout_assigned, _mp_logging_enabled
+    _mp_logging_enabled = True
+
+    if fmt is None:
+        fmt = _default_fmt
+    if use_FonsFormatter:
+        logging.Formatter = FonsFormatter
+
+    try:
+        _modules[_modules.index("__main__")] = "__mp_main__"
+    except ValueError:
+        pass
+
+    standard_5 = _init_standard_5(TEST_MODE, False)
+    """print('standard_mp_logging')
+    print(_modules)
+    print([m in sys.modules for m in _modules])
+    print(list(sys.modules)[:20])"""
+    multi_module_logging(_modules, standard_5._fields, standard_5)
+
+    for h in logging.root.handlers[:]:
+        logging.root.removeHandler(h)
+
+    logging.basicConfig(level=level, handlers=[QueueHandler(queue)], format=fmt)
+    # print('_queue is queue: {}'.format(_queue is queue))
+    _sys_stdout_assigned = True
+    # let's remove sys.stdout altogether (since parent process will print the 'stdout' logger output anyway)
+    sys.stdout = Tee([])  # sys.stdout
+    """print(sys.modules['__mp_main__'].logger2,sys.modules['__mp_main__'].logger2.name)"""
+
+
+def get_standard_logger(name=None):
+    if name is None:
+        return standard_5[0]
+
+    elif isinstance(name, int):
+        return standard_5[name]
+
+    return getattr(standard_5, name)
+
+
+def get_standard_5(module=None):
+    if module is not None:
+        add_module(module)
+
+    return standard_5
+
+
+def add_module(module):
+    if module not in _modules:
+        _modules.append(module)
+
+
+def _init_standard_5(TEST_MODE, stream_enabled=None):
+    if stream_enabled is None:
+        stream_enabled = not _mp_logging_enabled
+    logger = getFonsLogger("L1", streams=False)
+    logger2 = getFonsLogger("L2", streams=stream_enabled)
+
+    tlogger = getFonsLogger("T1", streams=False)  # logger
+    tloggers = getFonsLogger("T2", streams=stream_enabled)  # logger2
+    tlogger0 = getFonsLogger("T0", 0, streams=False)
+
+    if not TEST_MODE:
+        [x.setLevel(0) for x in (tlogger, tloggers, tlogger0)]
+
+    global standard_5
+    standard_5 = _Standard_5(logger, logger2, tlogger, tloggers, tlogger0)
+
+    return standard_5
+
+
+# --------------------------------------------
+
+
+def setup_logging(
+    dir=None,
+    lvl="INFO",
+    pair_with_fwriters=[],
+    fname=None,
+    f_ending=None,
+    lvl_handlers=[],
+    use_rotating=True,
+    maxBytes=5 * 1024 * 1024,
+    filemode="a",
+    backupCount=2,
+    fmt=None,
+    use_FonsFormatter=True,
+):
+    """Attaches file handlers to root logger"""
+    if dir is None:
+        dir = ""
+
+    if not fname:
+        fname = dt.utcnow().strftime("%Y-%m-%dT%H-%M-%S")
+    if f_ending:
+        fname += "_" + f_ending
+
+    if dir is not False:
+        dir = os.path.join(dir, fname)
+        if not os.path.exists(dir):
+            os.mkdir(dir)
+
+    if not fname.endswith(".log"):
+        fname += ".log"
+
+    if use_FonsFormatter:
+        logging.Formatter = FonsFormatter
+
+    if not fmt:
+        fmt = _default_fmt
+
+    lvl_handlers = lvl_handlers[:]
+
+    if not any(
+        isinstance(L, dict)
+        and level_to_int(L.get("lvl", L.get("level"))) == level_to_int(lvl)
+        or not isinstance(L, dict)
+        and level_to_int(L) == level_to_int(lvl)
+        for L in lvl_handlers
+    ):
+        lvl_handlers.append(lvl)
+
+    # Removes all previous handlers
+    # (e.g. if logging.log() called before setup_logging,
+    #  it automatically adds StreamHandler, and basicConfig(handlers=handlers) won't add the new handlers)
+    keep_handlers = [x for x in logging.root.handlers if isinstance(x, QueueHandler)]
+    for handler in logging.root.handlers[:]:
+        logging.root.removeHandler(handler)
+
+    handlers = []
+
+    for L in lvl_handlers:
+        if dir is False:
+            break
+        if not isinstance(L, dict):
+            L = {"lvl": L}
+
+        h_lvl = L.get("lvl", L.get("level"))
+        if isinstance(h_lvl, str):
+            h_lvl = h_lvl.upper()
+
+        # h_rotating = L.get('use_rotating',[True,False][level_to_int(h_lvl) > 30])
+        h_filemode = L.get("filemode", filemode)
+        h_backupCount = L.get("backupCount", backupCount)
+        h_max_size = L.get("maxBytes", maxBytes)
+
+        fpth = os.path.join(dir, fname[:-4] + "_{}.log".format(h_lvl))
+        if use_rotating:
+            h = RotatingFileHandler(
+                fpth,
+                mode=h_filemode,
+                maxBytes=h_max_size,
+                backupCount=h_backupCount,
+                encoding="utf-8",
+                delay=0,
+            )
+        else:
+            h = logging.FileHandler(fpth, mode=h_filemode)
+        h.setLevel(h_lvl)
+
+        handlers.append(h)
+
+    handlers += keep_handlers
+
+    logging.basicConfig(  # filename=fpath,
+        format=fmt,
+        # filemode=filemode,
+        handlers=handlers,
+        level=level_to_int(lvl),
+    )  # ,\
+    # datefmt = '%Y-%m-%dT%H:%M:%S')
+
+    if len(pair_with_fwriters):
+        synched_writer = Tee(pair_with_fwriters, lvl, logging)
+        return synched_writer
+
+
+if __name__ == "__main__":
+    logger.debug("first output (from L1)")
+    logdir = os.path.join("_test")
+    backup = sys.stdout
+    # Strange discovery:
+    #  if logging.log used before initiating handlers, handlers will be void
+    #  (everything is directed to logging module instead of handler)
+    # Don't do:
+    print("Handlers 0: {}".format(logging.root.handlers))  # []
+    logging.warning("HERE (from root)")
+    print(
+        "Handlers now: {}".format(logging.root.handlers)
+    )  # [<StreamHandler <stderr> (NOTSET)>]
+    logger.debug("HERE (from L1)")
+    logging2, sys.stdout = setup_logging(
+        logdir,
+        lvl="INFO",
+        # lvl_handlers =  [{'lvl':'INFO','maxBytes':0.5*1024*1024},{'lvl':'WARNING','use_rotating':True},'CRITICAL'],
+        use_rotating=True,
+        use_FonsFormatter=True,
+        pair_with_fwriters=[sys.stdout],
+        f_ending="main",
+        filemode="a",
+        maxBytes=5242880,
+        backupCount=5,
+    )
+
+    print("Handlers after setup: {}".format(logging2.root.handlers))
+
+    logger = getFonsLogger("L1", streams=False)
+    logger2 = getFonsLogger("L2", streams=True)
+    logger.info("LOGGER!")
+    logger2.info("LOGGER2!")
+
+    print("Handlers final: {}".format(logging.root.handlers))
```

### Comparing `fons-0.3.1/fons/math/graph.py` & `fons-0.4.0/fons/math/graph.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,76 @@
-def find_path(graph, start, end, path=[]):
-        path = path + [start]
-        if start == end:
-            return path
-        if start not in graph.keys():
-            return None
-        for node in graph[start]:
-            if node not in path:
-                newpath = find_path(graph, node, end, path)
-                if newpath: return newpath
-        return None
-    
-
-def find_all_paths(graph, start, end, path=[], max_len=None, *, _l=None):
-    if _l is None: _l = len(path)
-    path = path + [start]
-    _l += 1
-    if max_len is not None and _l > max_len:
-        return []
-    if start == end:
-        return [path]
-    
-    next_l = _l+1
-    if (max_len is not None and next_l > max_len) or start not in graph.keys():
-        return []
-    
-    paths = []
-    for node in graph[start]:
-        if node not in path:
-            newpaths = find_all_paths(graph, node, end, path, max_len, _l=_l)
-            for newpath in newpaths:
-                paths.append(newpath)
-    return paths
-
-
-def find_shortest_path(graph, start, end, path=[]):
-        path = path + [start]
-        if start == end:
-            return path
-        if start not in graph.keys():
-            return None
-        shortest = None
-        for node in graph[start]:
-            if node not in path:
-                newpath = find_shortest_path(graph, node, end, path)
-                if newpath:
-                    if not shortest or len(newpath) < len(shortest):
-                        shortest = newpath
-        return shortest
-
-
-def create_graph(pairs):
-    graph = {}
-    for pair in pairs:
-        p,q = pair
-        try: branch = graph[p]
-        except KeyError:
-            branch = graph[p] = []
-        branch.append(q)
-    return graph        
-    
-
-if __name__ == '__main__':
-        graph = {'A': ['B', 'C'],
-             'B': ['C', 'D'],
-             'C': ['D'],
-             'D': ['C'],
-             'E': ['F'],
-             'F': ['C']}
-
-        print(find_all_paths(graph, 'A', 'D'))
-
-        
+def find_path(graph, start, end, path=[]):
+    path = path + [start]
+    if start == end:
+        return path
+    if start not in graph.keys():
+        return None
+    for node in graph[start]:
+        if node not in path:
+            newpath = find_path(graph, node, end, path)
+            if newpath:
+                return newpath
+    return None
+
+
+def find_all_paths(graph, start, end, path=[], max_len=None, *, _l=None):
+    if _l is None:
+        _l = len(path)
+    path = path + [start]
+    _l += 1
+    if max_len is not None and _l > max_len:
+        return []
+    if start == end:
+        return [path]
+
+    next_l = _l + 1
+    if (max_len is not None and next_l > max_len) or start not in graph.keys():
+        return []
+
+    paths = []
+    for node in graph[start]:
+        if node not in path:
+            newpaths = find_all_paths(graph, node, end, path, max_len, _l=_l)
+            for newpath in newpaths:
+                paths.append(newpath)
+    return paths
+
+
+def find_shortest_path(graph, start, end, path=[]):
+    path = path + [start]
+    if start == end:
+        return path
+    if start not in graph.keys():
+        return None
+    shortest = None
+    for node in graph[start]:
+        if node not in path:
+            newpath = find_shortest_path(graph, node, end, path)
+            if newpath:
+                if not shortest or len(newpath) < len(shortest):
+                    shortest = newpath
+    return shortest
+
+
+def create_graph(pairs):
+    graph = {}
+    for pair in pairs:
+        p, q = pair
+        try:
+            branch = graph[p]
+        except KeyError:
+            branch = graph[p] = []
+        branch.append(q)
+    return graph
+
+
+if __name__ == "__main__":
+    graph = {
+        "A": ["B", "C"],
+        "B": ["C", "D"],
+        "C": ["D"],
+        "D": ["C"],
+        "E": ["F"],
+        "F": ["C"],
+    }
+
+    print(find_all_paths(graph, "A", "D"))
```

### Comparing `fons-0.3.1/fons/math/round.py` & `fons-0.4.0/fons/math/round.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,68 @@
-import math
-import numpy as np
-from builtins import round as _round
-
-
-def round_sd(x, sigdigits=3, method='round', accuracy=None):
-    if np.isnan(x):
-        return np.nan
-    elif x == 0:
-        return 0
-    
-    dist = math.floor(math.log10(abs(x)))
-    n = -dist + sigdigits-1
-    return round(x, n, method, accuracy)
-
-    #q = math.pow(10,-dist+keep-1)
-    #return math.trunc(x*q) / q
-    
-    
-def ignore_half_round(n):
-    if abs(n - int(n)) < 0.5:
-        return math.floor(n) if n>0 else math.ceil(n)
-    else: 
-        return math.ceil(n) if n>0 else math.floor(n)
-    
-
-def round(x, ndigits, method='round', accuracy=None):
-    """`accuracy` only applies to non-"round" methods.
-        Use it to weed out non-precise values:
-         round(2.0000000000000001, 0, 'ceil', 8) -> 2.0"""
-    method = method.lower()
-    if accuracy is None: pass
-    elif not isinstance(accuracy, int):
-        raise TypeError(type(accuracy))
-    elif accuracy < 0:
-        raise ValueError(accuracy)
-    
-    rrounded = _round(x, ndigits)
-    
-    if method == 'round':
-        return rrounded
-    
-    if method in ('down','floor','truncate','int'):
-        f = int
-        f2 = math.ceil
-    elif method in ('up','ceil'):
-        f = math.ceil
-        f2 = int
-    else:
-        raise ValueError(method)
-    
-    # x has no non-zero digits after n (this eliminates errors 
-    # that could otherwise arise due to multiplication)
-    if rrounded == x:
-        return x
-    
-    factor = pow(10, ndigits)
-    p = x*factor
-    
-    # Examples:
-    # round(8.2991, 1, 'floor', 2) -> 8.3
-    # round(8.3001, 1, 'ceil', 2) -> 8.3
-    if accuracy is not None and accuracy != 0:
-        factor2 = pow(10, accuracy)
-        p = f2(p*factor2)/factor2
-        
-    return f(p)/factor
+import math
+import numpy as np
+from builtins import round as _round
+
+
+def round_sd(x, sigdigits=3, method="round", accuracy=None):
+    if np.isnan(x):
+        return np.nan
+    elif x == 0:
+        return 0
+
+    dist = math.floor(math.log10(abs(x)))
+    n = -dist + sigdigits - 1
+    return round(x, n, method, accuracy)
+
+    # q = math.pow(10,-dist+keep-1)
+    # return math.trunc(x*q) / q
+
+
+def ignore_half_round(n):
+    if abs(n - int(n)) < 0.5:
+        return math.floor(n) if n > 0 else math.ceil(n)
+    else:
+        return math.ceil(n) if n > 0 else math.floor(n)
+
+
+def round(x, ndigits, method="round", accuracy=None):
+    """`accuracy` only applies to non-"round" methods.
+    Use it to weed out non-precise values:
+     round(2.0000000000000001, 0, 'ceil', 8) -> 2.0"""
+    method = method.lower()
+    if accuracy is None:
+        pass
+    elif not isinstance(accuracy, int):
+        raise TypeError(type(accuracy))
+    elif accuracy < 0:
+        raise ValueError(accuracy)
+
+    rrounded = _round(x, ndigits)
+
+    if method == "round":
+        return rrounded
+
+    if method in ("down", "floor", "truncate", "int"):
+        f = int
+        f2 = math.ceil
+    elif method in ("up", "ceil"):
+        f = math.ceil
+        f2 = int
+    else:
+        raise ValueError(method)
+
+    # x has no non-zero digits after n (this eliminates errors
+    # that could otherwise arise due to multiplication)
+    if rrounded == x:
+        return x
+
+    factor = pow(10, ndigits)
+    p = x * factor
+
+    # Examples:
+    # round(8.2991, 1, 'floor', 2) -> 8.3
+    # round(8.3001, 1, 'ceil', 2) -> 8.3
+    if accuracy is not None and accuracy != 0:
+        factor2 = pow(10, accuracy)
+        p = f2(p * factor2) / factor2
+
+    return f(p) / factor
```

### Comparing `fons-0.3.1/fons/math/series.py` & `fons-0.4.0/fons/math/series.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,717 +1,841 @@
-import pandas as pd
-import numpy as np
-import datetime
-dt = datetime.datetime
-td = datetime.timedelta
-
-from fons.time import (freq_to_offset, dt_round)
-
-
-_unitTD = {'_type_': td, '_call_': None}
-_unitDT = {'_type_': dt, '_call_': None}
-_multiunit = {'_multi_': [_unitTD,_unitDT]}
-
-TP_TYPES = {'_defval_': {'_type_':type(None),'_value_':None},
-            '_multi_':[{'_type_':tuple, 'unit': _multiunit, '_call_': None},
-                       {'_type_':list, 'unit': _multiunit, '_call_': None},
-                       _unitTD, _unitDT]}
-            
-
-#pd.tslib.Timedelta is ok with both np.datetime64/np.timedelta64 & dt/td
-#np.datetime64/np.timedelta64 & dt/td don't match
-
-def _check_none_borders(borders):
-    if borders is None: return True
-    
-    elif not isinstance(borders,(list,tuple,np.ndarray)):
-        return False
-
-    if not len(borders): return True
-    elif all(x is None for x in borders):
-        return True
-    
-    return False
-
-
-def get_timestamps(time_period, return_fmt=None):
-    tp = time_period
-    end = pd.to_datetime(dt.utcnow())
-    
-    if tp is None:
-        return None
-    
-    if not isinstance(tp,(tuple,list,np.ndarray)):
-        tp = (tp,end)
-    
-    ln = len(tp)
-    if ln > 2:
-        raise ValueError(time_period,"size > 2")
-    elif not ln or all(x is None for x in tp):
-        return None
-    elif ln == 1:
-        tp = (tp[0],end)
-    
-    tp = tuple(x if x is None else (pd.to_datetime(x) if isinstance(x,(dt,np.datetime64)) else freq_to_offset(x)) for x in  tp)
-    dtypes = tuple(x if x is None else ('t' if isinstance(x,dt) else 'd') for x in tp)
-    #print(tp,dtypes)
-    
-    if dtypes == ('d',None):
-        begin = end - tp[0]
-        end = None
-    
-    elif dtypes == (None,'d'):
-        begin = None
-        end -= tp[1]
-        
-    elif dtypes == ('t','d'):
-        begin = tp[0]
-        end = begin + tp[1]
-
-    elif dtypes == ('d','t'):
-        end = tp[1]
-        begin = end - tp[0]
-
-    elif dtypes == ('d','d'):
-        end -= tp[1]
-        begin = end - tp[0]
-        
-    else:
-        begin = tp[0]
-        end = tp[1]
-        
-    timestamps = (begin,end)
-    
-    if return_fmt == 'np.datetime64':
-        #converts both dt and pandas Timestamp
-        timestamps = tuple(np.datetime64(x) if x is not None else x for x in timestamps)
-    elif return_fmt == 'pydatetime':
-        timestamps = tuple(x.to_pydatetime() if x is not None else x for x in timestamps)
-            
-    return timestamps
-
-
-def get_period_entries(start, end, nr_periods=None, freq='D', round_start=False,
-                       exclude_end=False, exclude_noncomplete=False, return_as='DatetimeIndex'):
-    dtrange = None
-    if not isinstance(freq,td):
-        dtrange = pd.date_range(start,end,periods=nr_periods,freq=freq)
-        freq = dtrange.freq._offset * dtrange.freq.n
-    
-    if round_start:
-        start = dt_round(start,freq)
-        dtrange = pd.date_range(start,end,periods=nr_periods,freq=freq)
-    
-    if dtrange is None: dtrange = pd.date_range(start,end,periods=nr_periods,freq=freq)
-    
-        
-    if end is not None and exclude_end:
-        if dtrange[-1] >= end:
-            dtrange = dtrange[:-1]
-        
-        #excludes the last period if it is not "complete"
-        if exclude_noncomplete and dtrange.shape[0]:
-            if dtrange[-1] + freq > end:
-                dtrange = dtrange[:-1]
-    
-    if return_as == 'DatetimeIndex':
-        return dtrange
-    elif return_as == 'PeriodIndex':
-        return dtrange.to_period(freq)
-    elif return_as in ('pydatetime', 'datetime.datetime', 'dt.datetime'):
-        return dtrange.to_pydatetime()
-    else:
-        raise ValueError(return_as)
-
-
-
-def format_ts(ts, strfformat, nr_microsecs=None):
-    #print(ts,strfformat)
-    if isinstance(strfformat,dict):
-        strftime = ts.strftime(strfformat['strf'])
-        nr_microsecs = strfformat.get('nr_microsecs')
-        
-    else: strftime = ts.strftime(strfformat)
-
-    if '%f' in strfformat and nr_microsecs and nr_microsecs < 6:
-        strftime = strftime[:(-6+nr_microsecs)]
-        
-    return strftime
-
-
-#time period or just a single timestamp
-def format_tp(tp, strfformat, nr_microsecs=None):
-    timestamps = get_timestamps(tp)
-
-    strftimes = [format_ts(ts,strfformat,nr_microsecs) for ts in timestamps]
-    
-    timedeltas = [td(days=365),td(days=30),td(days=1),td(hours=1),
-                  td(minutes=1),td(seconds=1),td(milliseconds=1),td(microseconds=1)]
-    delta = timestamps[1] - timestamps[0]
-    
-    if delta in timedeltas:
-        return strftimes[0]
-    else:
-        return 'to'.join(strftimes)
-
-
-def get_fringe_entries(obj, key=None, func=None):
-    key_isfunc = hasattr(key,'__call__')
-    entries = []
-    key0 = key
-    
-    if isinstance(obj,(pd.DataFrame,pd.Series)):
-        if isinstance(obj,pd.DataFrame):
-            if key is not None:
-                _iterable = obj[key] if not key_isfunc else key(obj)
-            else: _iterable = obj.index
-            
-        elif isinstance(obj,pd.Series):
-            if key_isfunc: _iterable = key(obj)
-            elif obj.dtypes.name == 'datetime64[ns]':
-                _iterable = obj
-            else: _iterable = obj.index
-        
-        try:
-            if isinstance(_iterable,pd.Series):
-                entries = [_iterable.iloc[0],_iterable.iloc[-1]]
-            else: 
-                entries = [_iterable[0],_iterable[-1]]
-        except IndexError: 
-            pass
-        
-    else:
-        try: hasgetitem = hasattr(obj[0],'__getitem__')
-        except IndexError: hasgetitem = False
-        
-        if key is None: key = lambda x: x
-        elif key_isfunc: pass
-        elif hasgetitem: key = lambda x: x[key0]
-        else: key = lambda x: getattr(x,key)
-        
-        try: 
-            entries = [key(obj[0]),key(obj[-1])]
-        except IndexError:
-            pass
-        
-    if func:
-        entries = [func(x) for x in entries]
-        
-    return entries
-    
-
-def _apply_key_func(obj, key=None, func=None):
-    key_isfunc = hasattr(key,'__call__')
-    is_gen = False
-    
-    if isinstance(obj,pd.DataFrame):
-        if key is not None:
-            _iterable = obj[key] if not key_isfunc else key(obj)
-        else: _iterable = obj.index
-        
-    elif isinstance(obj,pd.Series):
-        if key_isfunc: _iterable = key(obj)
-        elif obj.dtypes.name == 'datetime64[ns]':
-            _iterable = obj
-        else: _iterable = obj.index
-        
-    else: 
-        try: hasgetitem = hasattr(obj[0],'__getitem__')
-        except IndexError: hasgetitem = False
-
-        if key is None: _iterable = obj
-        elif key_isfunc: _iterable,is_gen = map(key,obj),True
-        elif hasgetitem: _iterable,is_gen = map(lambda x: x[key], obj),True
-        else: _iterable,is_gen = map(lambda x: getattr(x,key), obj),True
-        
-    if not func: pass
-    elif isinstance(_iterable,(pd.Series,pd.Index)): _iterable = _iterable.apply(func)
-    else: _iterable,is_gen = map(func,_iterable),True
-        
-    return _iterable,is_gen
-
-
-def get_time_borders(obj, tp, key=None):
-    tp = get_timestamps(tp,'pd.Timestamp')
-    #temporary, due to supposed 0.21 pandas bug
-    #tp = get_timestamps(tp,'pydatetime')
-    if tp is None: return None
-    
-    begin,end = tp
-    start,finish = None,None
-    
-    _iterable,is_gen = _apply_key_func(obj,key)
-    
-    #temporary:
-    if isinstance(_iterable,np.ndarray): tp = tuple([np.datetime64(x) for x in tp]) 
-        
-    if isinstance(_iterable,(pd.Series,pd.DatetimeIndex,np.ndarray)):
-        b_array = (_iterable >= begin) & (_iterable < end)
-        indexes = b_array.nonzero()[0]
-        
-        if indexes.shape[0]:
-            start = indexes[0]
-            finish = indexes[-1]     
-        
-    else:
-        for i,ts in enumerate(_iterable):
-            if start is None and ts >= begin:
-                start = i
-                
-            if ts < end:
-                finish = i
-            else: break
-    
-    
-    if None in (start,finish):
-        return None
-        
-    return (start,finish)
-
-
-def get_slice_where(obj, borders, key=None, func=None):
-    borders = get_timestamps(borders, return_fmt='pd.Timestamp')
-    if borders is None: return np.arange(0)
-    elif borders is False: return np.arange(0)
-    elif not len(obj): return np.arange(0)
-
-    begin,end = borders
-    _iterable,is_gen = _apply_key_func(obj,key,func)
-    
-    if not isinstance(_iterable,(pd.Series,pd.Index,np.ndarray)):
-        if is_gen: _iterable = tuple(_iterable)
-        _iterable = np.asarray(_iterable)
-    
-    #seems to be necessary (py 3.6, pd 0.22, np 1.14), even if tp consists of pd.TimeStamps
-    if isinstance(_iterable,np.ndarray):
-        begin,end = [np.datetime64(x) if x is not None else None for x in borders]
-    
-    if not begin: b_array = (_iterable < end)
-    elif not end: b_array = (_iterable >= begin)
-    else: b_array = (_iterable >= begin) & (_iterable < end)
-
-    return b_array
-
-
-def get_slice_indexes(obj, borders, key=None, func=None):
-    b_array = get_slice_where(obj, borders, key=key, func=func)
-    indexes = b_array.nonzero()[0]   
-    #the indexes are absolute (iloc), not related to the actual index (of pd.Series)
-    
-    return indexes
-
-
-def slice_obj(obj, tp, key=None, func=None):
-    if _check_none_borders(tp): return obj
-    where = get_slice_where(obj,tp,key,func)
-    
-    if not where.any():
-        obj2 = obj[-1:-1]
-        
-    elif isinstance(obj,(pd.DataFrame,pd.Series)):
-        #if DataFrame without using loc, boolean is automatically applied to index
-        # (other types like int/str.. are applied to columns)
-        obj2 = obj[where]
-    else:
-        try:
-            obj2 = obj[where] 
-        except TypeError:
-            _type = type(obj)
-            obj2 = _type((x for x,b in zip(obj,where) if b))
-            
-    return obj2
-
-
-
-#############################
-def _get_last_nonnan(a):
-    nonnan = a[~np.isnan(a)]
-    if nonnan.shape[0]:
-        return nonnan[-1]
-    return np.nan
-
-def _implement_fill_policy(a, how='previous', fill_remaining=True, if_all='leave', r=0):
-    s = a
-    if not isinstance(a,pd.Series):
-        s = pd.Series(a)
-        
-    if how in ('next',1):
-        s = s[::-1]
-    
-    sp = s.rolling(window=s.shape[0],min_periods=1).agg(_get_last_nonnan)
-    #print(sp,if_all)
-    
-    if not sp.isnull().any():
-        pass
-    elif sp.isnull().all() and if_all == 'drop':
-        sp.dropna(inplace=True)
-    elif fill_remaining and r==0:
-        sp = _implement_fill_policy(sp,'next',fill_remaining,if_all,r=r+1)
-        
-    if how in ('next',1):
-        sp = sp[::-1]
-    
-    #sp2 is copy, does not affect s
-    return sp
-
-
-def implement_nan_policy(a, how='drop',**kw):
-    def_policy = {'how':'drop','fill_remaining':False,'if_all':'drop'}
-    policy = _nan_policy_vars(how, dict(def_policy,**kw))
-    how = policy['how']
-    
-    s = a
-    if not isinstance(a,pd.Series):
-        s = pd.Series(a)
-    
-    s2 = s
-
-    if not s.isnull().any() or how == 'leave':
-        pass
-    elif how == 'drop':
-        s2 = s.dropna()
-    elif how in ('previous','prev','next',-1,1):
-        s2 = _implement_fill_policy(s,**policy)
-    
-    return s2.values
-
-
-def _nan_policy_vars(policy, def_vals):
-    policy2 = def_vals.copy()
-    k = ('how','fill_remaining','if_all')
-    
-    if isinstance(policy,(list,tuple)):
-        for p,v in zip(k,policy):
-            policy2[p] = v
-    elif isinstance(policy,dict):
-        policy2.update(policy)
-    elif policy is not None:
-        policy2[k[0]] = policy
-    
-    return policy2
-
-    
-def undo_cumsum(_iterable, first='drop', negatives='drop', nr=None, nan_policy=None):
-    if not len(_iterable): return np.asarray(_iterable)
-    np.seterr(invalid='ignore')
-    def_policy = {'how':'previous','fill_remaining':True,'if_all':'leave'}
-    nan_policy = _nan_policy_vars(nan_policy,def_policy)
-    #print(nan_policy)
-    
-    a = implement_nan_policy(_iterable,**nan_policy)
-    #print(a)
-    nan_list = ('nan','np.nan','numpy.nan','math.nan')
-
-    ucs = np.concatenate([a[:1], a[1:] - a[:-1]]).astype(float)
-    """first_locs = np.arange(ucs.shape[0]) == 0
-    neg_locs = ucs < 0"""
-    if not ucs.shape[0]: return ucs
-    
-    for n,op in zip(('first','negatives'),(first,negatives)):
-        #ucs < 0 displays RuntimeWarning when encountering nan
-        #locs = np.arange(ucs.shape[0]) == 0 if n=='first' else ucs < 0
-        locs = [0] if n=='first' else np.where(ucs < 0)[0]
-
-        if op =='leave':
-            pass
-        elif op == 'drop':
-            #ucs = ucs[~locs]
-            ucs = np.delete(ucs,locs)
-        elif isinstance(op,(int,float)):
-            ucs[locs] = op
-        elif isinstance(op,str) and op.lower() == 'zero':
-            ucs[locs] = 0
-        elif pd.isnull(op) or op is None or \
-                isinstance(op,str) and op.lower() in nan_list:
-            ucs[locs] = np.nan
-        else: raise ValueError(n,op)
-       
-    if nr:
-        ucs = ucs[-nr:]
-        
-    return ucs
-            
-    """else:
-        #ucs = []
-        for i,v in enumerate(_iterable[:0:-1]):
-            dif = v - _iterable[-2-i]
-            
-            if excl_negatives and dif < 0: continue
-            else: ucs.append(dif)
-            
-            if nr and len(ucs) >= nr:
-                break
-            
-        ucs = ucs[::-1]"""
-        
-
-def _check_limits(limits):
-    if len(limits) != 2:
-        raise ValueError('Limits must contain 2 elements; got: {}'.format(len(limits)))
-    
-    if limits[0] is not None and limits[0] > 0:
-        raise ValueError('First limit must be <= 0; got: {}'.format(limits[0]))
-    
-    if limits[1] is not None and limits[1] < 0:
-        raise ValueError('Second limit must be >= 0; got: {}'.format(limits[1]))
-    
-    if sum(x==0 for x in limits) == 1 and None not in limits:
-        raise ValueError('Either both limits must be 0 or neither of them; got: {}'.format(limits))
-    
-    return True
-
-
-def limiter(A, limits, closed='both'):
-    if closed not in ('both','left','right','neither',None):
-        raise ValueError('`closed` must be one of the following: (both,left,right,neither); got: {}'.format(closed))
-    L0,L1 = limits
-
-    if L0 is not None:
-        op = lambda x,y: x>=y if closed in ('both','left',None) else lambda x,y: x>y
-        A = np.where(op(A,L0),A,np.nan)
-    if L1 is not None:
-        op = lambda x,y: x<=y if closed in ('both','right',None) else lambda x,y: x<y
-        A = np.where(op(A,L1),A,np.nan)
-        
-    if A.ndim > 1:
-        return A[~np.isnan(A).any(axis=1)]
-    else:
-        return A[~np.isnan(A)]
-
-    
-def randomize_summation(_sum, n, limits=(-0.3,0.3), closed='both', *, factor=15, sample_size=10):
-    limit_vs = (None,None)
-    mean = 1/n   
-        
-    if limits is not None:
-        _check_limits(limits)
-        limit_vs = [mean*(1+L) if L is not None else L for L in limits]
-    
-    if all(x==0 for x in limit_vs):
-        if closed not in ('both',None):
-            raise ValueError('`closed` must be \'both\' if both limits are 0; got: {}'.format(closed))
-        return np.ones(n) * mean
-    
-    while True:
-        #A is a 2d array even if sample_size=1
-        A = np.random.dirichlet(np.ones(n)*factor,size=sample_size)
-        
-        A2 = limiter(A,limit_vs,closed=closed)
-        
-        if not A2.shape[0]:
-            factor *= 2
-            #print(factor)
-        else: break
-        
-    return A2[0]*_sum
-
-
-def weight_limiter(A, weight_limits, closed='both'):
-    if closed not in ('both','left','right','neither',None):
-        raise ValueError('`closed` must be one of the following: (both,left,right,neither); got: {}'.format(closed))
-            
-    op1 = (lambda x,y: x>=y) if closed in ('both','left',None) else (lambda x,y: x>y)
-    op2 = (lambda x,y: x<=y) if closed in ('both','right',None) else (lambda x,y: x<y)
-    AT = A.transpose()
-    at = []
-    
-    for i,limits in enumerate(weight_limits):
-        L0,L1 = limits
-        ATi = AT[i]
-        if L0 is not None:
-            ATi = np.where(op1(ATi,L0),ATi,np.nan)
-        if L1 is not None:
-            ATi = np.where(op2(ATi,L1),ATi,np.nan)
-        at.append(ATi)
-        
-    AT = np.asarray(at,dtype=np.float64)
-    A = AT.transpose()
-        
-    if A.ndim > 1:
-        return A[~np.isnan(A).any(axis=1)]
-    else:
-        return A[~np.isnan(A)]
-
-
-def randomize_weights(weights, limits=(-0.3,0.3), closed='both', *, factor=15, sample_size=10):
-    weights = np.asarray(weights,dtype=np.float64)
-    _sum = weights.sum()
-    limit_vs = [(None,None)]*weights.size
-        
-    if limits is not None:
-        _check_limits(limits)
-        limit_vs = [[w*(1+L) if L is not None else L for L in limits] for w in weights]
-    
-    if all(x==0 for x in limit_vs):
-        if closed not in ('both',None):
-            raise ValueError('`closed` must be \'both\' if both limits are 0; got: {}'.format(closed))
-        return weights
-    
-    while True:
-        #A is a 2d array even if sample_size=1
-        A = np.random.dirichlet(weights*factor,size=sample_size)*_sum
-        
-        A2 = weight_limiter(A,limit_vs,closed=closed) if limits is not None else A
-        
-        if not A2.shape[0]:
-            factor *= 2
-            #print(factor)
-        else: break
-        
-    return A2[0]
-
-#----------------------------------------------------------------------------
-def verify_uniqueness(obj, index=True, columns=True, name=None):
-    if isinstance(obj, pd.Series): columns = False
-    
-    if name is None: name_str = ''
-    else: name_str = '{}\'s '
-        
-    for attr,include in (('index',index),('columns',columns)):
-        if not include: continue
-        
-        ind = getattr(obj,attr)
-        ind_duplicated = ind[ind.duplicated()]
-        if not ind_duplicated.shape[0]:
-            continue
-        
-
-        raise ValueError('Duplicates in {}{}: {}'.format(
-                                        name_str,attr,ind_duplicated))
-    
-    
-def _get_valid(obj, valid_col=None, valid_func=None):
-    #last_index = obj[valid_col].last_valid_index()
-    is_series = isinstance(obj,pd.Series)
-
-    if is_series: check_cols = [obj]
-    elif valid_col: check_cols = [obj[valid_col]]
-    else: check_cols = [x[1] for x in obj.iteritems()]
-    
-    last_index = -1
-    obj_index = obj.index
-
-    for s in check_cols:
-        if valid_func:
-            valid_indexes = s.apply(valid_func)
-            if not valid_indexes.shape[0]: continue
-            last_index = max(last_index, obj_index[valid_indexes][-1])
-            continue
-        
-        valid_index = obj.last_valid_index()
-        if valid_index is not None: continue
-        last_index = max(last_index,valid_index)
-    
-    return last_index
-    
-    
-def pd_replace(obj, obj2, start=None, valid_col=None, valid_func=None, simple=True):
-    """If simple=True, then obj nor obj2 must contain non-unique indexes/columns.
-       Otherwise if start has multiple matches in obj.index, last is chosen."""
-    is_series = isinstance(obj, pd.Series)
-    if simple: [verify_uniqueness(objx,columns=b_col,name=name) 
-                for objx,b_col,name in ((obj,True,'obj'),(obj2,False,'obj2'))]
-                
-    if start is None:
-        last_index = _get_valid(obj, valid_col, valid_func)
-            
-        if last_index != -1:
-            entry_iloc = obj.index.get_loc(last_index) + 1
-        else: entry_iloc = 0
-        
-    else: entry_iloc = obj.index.get_loc(start)
-    
-    
-    if isinstance(entry_iloc,np.ndarray):
-        #index was not unique, multiple matches
-        entry_iloc = np.where(entry_iloc)[0][-1]
-    
-    
-    end_iloc = entry_iloc + obj2.shape[0]
-    missing = end_iloc - obj.shape[0]
-    
-    if missing > 0:
-        I = IndexError('Obj short of {} rows'.format(missing))
-        I.missing = missing
-        raise I
-    
-    
-    #Note (example):
-    #obj.index = [0,0] + list(obj.index[2:])
-    #obj.iloc[0:2] = obj2
-    # -> now both rows (0,0) are overwritten with the matching row of obj2
-    #However, if obj2 has duplicates (0,0), it will not work
-
-    if is_series:
-        obj.iloc[entry_iloc:end_iloc] = obj2.values
-    
-    elif simple:
-        ind0 = obj2.index
-        obj2.index = obj.index[entry_iloc:end_iloc]
-        
-        overlapping_cols = np.where(obj.columns.isin(obj2.columns))[0]
-        obj.iloc[entry_iloc:end_iloc, overlapping_cols] = obj2
-        
-        obj2.index = ind0
-    
-    else:
-        obj_cols = obj.columns
-        obj2_cols= obj2.columns
-        obj2_cols_uniq_ind = np.where(~obj2_cols.duplicated())
-        
-        for col2_iloc in obj2_cols_uniq_ind:
-            col2 = obj2_cols[col2_iloc]
-            
-            try: col_iloc = obj_cols.get_loc(col2)
-            except KeyError: continue
-            
-            obj2_values = obj2.iloc[:,col2_iloc].values
-            
-            if isinstance(col_iloc,np.ndarray):
-                col_iloc = np.where(col_iloc)[0]
-                #list of matching columns (with identical name)
-                obj2_values = [obj2_values for x in col_iloc]
-            
-            
-            obj.iloc[entry_iloc:end_iloc,col_iloc] = obj2_values
-
-
-
-if __name__ == '__main__':
-    #print(randomize_summation(15.4,5))
-    weights = [0.2,0.8,0.4,0.6]
-    rw = randomize_weights(weights,limits=(-0.05,0.05))
-    print(rw)
-    
-    tp = get_timestamps([np.timedelta64(td(minutes=60)), td(minutes=30)])
-    print(tp)
-    tp2 = get_timestamps(np.timedelta64(td(minutes=60)))
-    print(tp2)
-    tp3 = get_timestamps(dt(2016,1,1),'np.datetime64')
-    print(tp3)
-    tp4 = get_timestamps([td(days=60),dt(2016,1,1)],'pydatetime')
-    print(tp4)
-    print("\n Get_period_entries:")
-    
-    tp5 = (dt(2000,1,1),dt(2000,1,1,5))
-    pe = get_period_entries(tp5[0],tp5[1],freq=td(hours=1),exclude_end=False)
-    for i,x in enumerate(pe[:-1]):
-        x2 = pe[i+1]
-        print([x,x2])
-        
-        tp6  = get_timestamps((x,x2))
-        print(tp6)
-        
-        tp7 = get_timestamps(tp6,'pd.TimeStamp')
-        begin,end = tp7
-        print((begin,end),"\n")
-    
-    tp8 = get_timestamps(['1D',None])
-    print(tp8)
-    
-    tp9 = get_timestamps([dt(2000,1,1),None])
-    print(tp9)
-        
-    so = slice_obj(pd.Series(np.arange(6),index=pe),(pe[2],td(hours=2)))
-    print(so)
-    so2 = slice_obj(list(pe),(pe[2],td(hours=2)))
-    print(so2)
+import pandas as pd
+import numpy as np
+import datetime
+
+dt = datetime.datetime
+td = datetime.timedelta
+
+from fons.time import freq_to_offset, dt_round
+
+
+_unitTD = {"_type_": td, "_call_": None}
+_unitDT = {"_type_": dt, "_call_": None}
+_multiunit = {"_multi_": [_unitTD, _unitDT]}
+
+TP_TYPES = {
+    "_defval_": {"_type_": type(None), "_value_": None},
+    "_multi_": [
+        {"_type_": tuple, "unit": _multiunit, "_call_": None},
+        {"_type_": list, "unit": _multiunit, "_call_": None},
+        _unitTD,
+        _unitDT,
+    ],
+}
+
+
+# pd.tslib.Timedelta is ok with both np.datetime64/np.timedelta64 & dt/td
+# np.datetime64/np.timedelta64 & dt/td don't match
+
+
+def _check_none_borders(borders):
+    if borders is None:
+        return True
+
+    elif not isinstance(borders, (list, tuple, np.ndarray)):
+        return False
+
+    if not len(borders):
+        return True
+    elif all(x is None for x in borders):
+        return True
+
+    return False
+
+
+def get_timestamps(time_period, return_fmt=None):
+    tp = time_period
+    end = pd.to_datetime(dt.utcnow())
+
+    if tp is None:
+        return None
+
+    if not isinstance(tp, (tuple, list, np.ndarray)):
+        tp = (tp, end)
+
+    ln = len(tp)
+    if ln > 2:
+        raise ValueError(time_period, "size > 2")
+    elif not ln or all(x is None for x in tp):
+        return None
+    elif ln == 1:
+        tp = (tp[0], end)
+
+    tp = tuple(
+        x
+        if x is None
+        else (
+            pd.to_datetime(x)
+            if isinstance(x, (dt, np.datetime64))
+            else freq_to_offset(x)
+        )
+        for x in tp
+    )
+    dtypes = tuple(x if x is None else ("t" if isinstance(x, dt) else "d") for x in tp)
+    # print(tp,dtypes)
+
+    if dtypes == ("d", None):
+        begin = end - tp[0]
+        end = None
+
+    elif dtypes == (None, "d"):
+        begin = None
+        end -= tp[1]
+
+    elif dtypes == ("t", "d"):
+        begin = tp[0]
+        end = begin + tp[1]
+
+    elif dtypes == ("d", "t"):
+        end = tp[1]
+        begin = end - tp[0]
+
+    elif dtypes == ("d", "d"):
+        end -= tp[1]
+        begin = end - tp[0]
+
+    else:
+        begin = tp[0]
+        end = tp[1]
+
+    timestamps = (begin, end)
+
+    if return_fmt == "np.datetime64":
+        # converts both dt and pandas Timestamp
+        timestamps = tuple(np.datetime64(x) if x is not None else x for x in timestamps)
+    elif return_fmt == "pydatetime":
+        timestamps = tuple(
+            x.to_pydatetime() if x is not None else x for x in timestamps
+        )
+
+    return timestamps
+
+
+def get_period_entries(
+    start,
+    end,
+    nr_periods=None,
+    freq="D",
+    round_start=False,
+    exclude_end=False,
+    exclude_noncomplete=False,
+    return_as="DatetimeIndex",
+):
+    dtrange = None
+    if not isinstance(freq, td):
+        dtrange = pd.date_range(start, end, periods=nr_periods, freq=freq)
+        freq = dtrange.freq._offset * dtrange.freq.n
+
+    if round_start:
+        start = dt_round(start, freq)
+        dtrange = pd.date_range(start, end, periods=nr_periods, freq=freq)
+
+    if dtrange is None:
+        dtrange = pd.date_range(start, end, periods=nr_periods, freq=freq)
+
+    if end is not None and exclude_end:
+        if dtrange[-1] >= end:
+            dtrange = dtrange[:-1]
+
+        # excludes the last period if it is not "complete"
+        if exclude_noncomplete and dtrange.shape[0]:
+            if dtrange[-1] + freq > end:
+                dtrange = dtrange[:-1]
+
+    if return_as == "DatetimeIndex":
+        return dtrange
+    elif return_as == "PeriodIndex":
+        return dtrange.to_period(freq)
+    elif return_as in ("pydatetime", "datetime.datetime", "dt.datetime"):
+        return dtrange.to_pydatetime()
+    else:
+        raise ValueError(return_as)
+
+
+def format_ts(ts, strfformat, nr_microsecs=None):
+    # print(ts,strfformat)
+    if isinstance(strfformat, dict):
+        strftime = ts.strftime(strfformat["strf"])
+        nr_microsecs = strfformat.get("nr_microsecs")
+
+    else:
+        strftime = ts.strftime(strfformat)
+
+    if "%f" in strfformat and nr_microsecs and nr_microsecs < 6:
+        strftime = strftime[: (-6 + nr_microsecs)]
+
+    return strftime
+
+
+# time period or just a single timestamp
+def format_tp(tp, strfformat, nr_microsecs=None):
+    timestamps = get_timestamps(tp)
+
+    strftimes = [format_ts(ts, strfformat, nr_microsecs) for ts in timestamps]
+
+    timedeltas = [
+        td(days=365),
+        td(days=30),
+        td(days=1),
+        td(hours=1),
+        td(minutes=1),
+        td(seconds=1),
+        td(milliseconds=1),
+        td(microseconds=1),
+    ]
+    delta = timestamps[1] - timestamps[0]
+
+    if delta in timedeltas:
+        return strftimes[0]
+    else:
+        return "to".join(strftimes)
+
+
+def get_fringe_entries(obj, key=None, func=None):
+    key_isfunc = hasattr(key, "__call__")
+    entries = []
+    key0 = key
+
+    if isinstance(obj, (pd.DataFrame, pd.Series)):
+        if isinstance(obj, pd.DataFrame):
+            if key is not None:
+                _iterable = obj[key] if not key_isfunc else key(obj)
+            else:
+                _iterable = obj.index
+
+        elif isinstance(obj, pd.Series):
+            if key_isfunc:
+                _iterable = key(obj)
+            elif obj.dtypes.name == "datetime64[ns]":
+                _iterable = obj
+            else:
+                _iterable = obj.index
+
+        try:
+            if isinstance(_iterable, pd.Series):
+                entries = [_iterable.iloc[0], _iterable.iloc[-1]]
+            else:
+                entries = [_iterable[0], _iterable[-1]]
+        except IndexError:
+            pass
+
+    else:
+        try:
+            hasgetitem = hasattr(obj[0], "__getitem__")
+        except IndexError:
+            hasgetitem = False
+
+        if key is None:
+            key = lambda x: x
+        elif key_isfunc:
+            pass
+        elif hasgetitem:
+            key = lambda x: x[key0]
+        else:
+            key = lambda x: getattr(x, key)
+
+        try:
+            entries = [key(obj[0]), key(obj[-1])]
+        except IndexError:
+            pass
+
+    if func:
+        entries = [func(x) for x in entries]
+
+    return entries
+
+
+def _apply_key_func(obj, key=None, func=None):
+    key_isfunc = hasattr(key, "__call__")
+    is_gen = False
+
+    if isinstance(obj, pd.DataFrame):
+        if key is not None:
+            _iterable = obj[key] if not key_isfunc else key(obj)
+        else:
+            _iterable = obj.index
+
+    elif isinstance(obj, pd.Series):
+        if key_isfunc:
+            _iterable = key(obj)
+        elif obj.dtypes.name == "datetime64[ns]":
+            _iterable = obj
+        else:
+            _iterable = obj.index
+
+    else:
+        try:
+            hasgetitem = hasattr(obj[0], "__getitem__")
+        except IndexError:
+            hasgetitem = False
+
+        if key is None:
+            _iterable = obj
+        elif key_isfunc:
+            _iterable, is_gen = map(key, obj), True
+        elif hasgetitem:
+            _iterable, is_gen = map(lambda x: x[key], obj), True
+        else:
+            _iterable, is_gen = map(lambda x: getattr(x, key), obj), True
+
+    if not func:
+        pass
+    elif isinstance(_iterable, (pd.Series, pd.Index)):
+        _iterable = _iterable.apply(func)
+    else:
+        _iterable, is_gen = map(func, _iterable), True
+
+    return _iterable, is_gen
+
+
+def get_time_borders(obj, tp, key=None):
+    tp = get_timestamps(tp, "pd.Timestamp")
+    # temporary, due to supposed 0.21 pandas bug
+    # tp = get_timestamps(tp,'pydatetime')
+    if tp is None:
+        return None
+
+    begin, end = tp
+    start, finish = None, None
+
+    _iterable, is_gen = _apply_key_func(obj, key)
+
+    # temporary:
+    if isinstance(_iterable, np.ndarray):
+        tp = tuple([np.datetime64(x) for x in tp])
+
+    if isinstance(_iterable, (pd.Series, pd.DatetimeIndex, np.ndarray)):
+        b_array = (_iterable >= begin) & (_iterable < end)
+        indexes = b_array.nonzero()[0]
+
+        if indexes.shape[0]:
+            start = indexes[0]
+            finish = indexes[-1]
+
+    else:
+        for i, ts in enumerate(_iterable):
+            if start is None and ts >= begin:
+                start = i
+
+            if ts < end:
+                finish = i
+            else:
+                break
+
+    if None in (start, finish):
+        return None
+
+    return (start, finish)
+
+
+def get_slice_where(obj, borders, key=None, func=None):
+    borders = get_timestamps(borders, return_fmt="pd.Timestamp")
+    if borders is None:
+        return np.arange(0)
+    elif borders is False:
+        return np.arange(0)
+    elif not len(obj):
+        return np.arange(0)
+
+    begin, end = borders
+    _iterable, is_gen = _apply_key_func(obj, key, func)
+
+    if not isinstance(_iterable, (pd.Series, pd.Index, np.ndarray)):
+        if is_gen:
+            _iterable = tuple(_iterable)
+        _iterable = np.asarray(_iterable)
+
+    # seems to be necessary (py 3.6, pd 0.22, np 1.14), even if tp consists of pd.TimeStamps
+    if isinstance(_iterable, np.ndarray):
+        begin, end = [np.datetime64(x) if x is not None else None for x in borders]
+
+    if not begin:
+        b_array = _iterable < end
+    elif not end:
+        b_array = _iterable >= begin
+    else:
+        b_array = (_iterable >= begin) & (_iterable < end)
+
+    return b_array
+
+
+def get_slice_indexes(obj, borders, key=None, func=None):
+    b_array = get_slice_where(obj, borders, key=key, func=func)
+    indexes = b_array.nonzero()[0]
+    # the indexes are absolute (iloc), not related to the actual index (of pd.Series)
+
+    return indexes
+
+
+def slice_obj(obj, tp, key=None, func=None):
+    if _check_none_borders(tp):
+        return obj
+    where = get_slice_where(obj, tp, key, func)
+
+    if not where.any():
+        obj2 = obj[-1:-1]
+
+    elif isinstance(obj, (pd.DataFrame, pd.Series)):
+        # if DataFrame without using loc, boolean is automatically applied to index
+        # (other types like int/str.. are applied to columns)
+        obj2 = obj[where]
+    else:
+        try:
+            obj2 = obj[where]
+        except TypeError:
+            _type = type(obj)
+            obj2 = _type((x for x, b in zip(obj, where) if b))
+
+    return obj2
+
+
+#############################
+def _get_last_nonnan(a):
+    nonnan = a[~np.isnan(a)]
+    if nonnan.shape[0]:
+        return nonnan[-1]
+    return np.nan
+
+
+def _implement_fill_policy(a, how="previous", fill_remaining=True, if_all="leave", r=0):
+    s = a
+    if not isinstance(a, pd.Series):
+        s = pd.Series(a)
+
+    if how in ("next", 1):
+        s = s[::-1]
+
+    sp = s.rolling(window=s.shape[0], min_periods=1).agg(_get_last_nonnan)
+    # print(sp,if_all)
+
+    if not sp.isnull().any():
+        pass
+    elif sp.isnull().all() and if_all == "drop":
+        sp.dropna(inplace=True)
+    elif fill_remaining and r == 0:
+        sp = _implement_fill_policy(sp, "next", fill_remaining, if_all, r=r + 1)
+
+    if how in ("next", 1):
+        sp = sp[::-1]
+
+    # sp2 is copy, does not affect s
+    return sp
+
+
+def implement_nan_policy(a, how="drop", **kw):
+    def_policy = {"how": "drop", "fill_remaining": False, "if_all": "drop"}
+    policy = _nan_policy_vars(how, dict(def_policy, **kw))
+    how = policy["how"]
+
+    s = a
+    if not isinstance(a, pd.Series):
+        s = pd.Series(a)
+
+    s2 = s
+
+    if not s.isnull().any() or how == "leave":
+        pass
+    elif how == "drop":
+        s2 = s.dropna()
+    elif how in ("previous", "prev", "next", -1, 1):
+        s2 = _implement_fill_policy(s, **policy)
+
+    return s2.values
+
+
+def _nan_policy_vars(policy, def_vals):
+    policy2 = def_vals.copy()
+    k = ("how", "fill_remaining", "if_all")
+
+    if isinstance(policy, (list, tuple)):
+        for p, v in zip(k, policy):
+            policy2[p] = v
+    elif isinstance(policy, dict):
+        policy2.update(policy)
+    elif policy is not None:
+        policy2[k[0]] = policy
+
+    return policy2
+
+
+def undo_cumsum(_iterable, first="drop", negatives="drop", nr=None, nan_policy=None):
+    if not len(_iterable):
+        return np.asarray(_iterable)
+    np.seterr(invalid="ignore")
+    def_policy = {"how": "previous", "fill_remaining": True, "if_all": "leave"}
+    nan_policy = _nan_policy_vars(nan_policy, def_policy)
+    # print(nan_policy)
+
+    a = implement_nan_policy(_iterable, **nan_policy)
+    # print(a)
+    nan_list = ("nan", "np.nan", "numpy.nan", "math.nan")
+
+    ucs = np.concatenate([a[:1], a[1:] - a[:-1]]).astype(float)
+    """first_locs = np.arange(ucs.shape[0]) == 0
+    neg_locs = ucs < 0"""
+    if not ucs.shape[0]:
+        return ucs
+
+    for n, op in zip(("first", "negatives"), (first, negatives)):
+        # ucs < 0 displays RuntimeWarning when encountering nan
+        # locs = np.arange(ucs.shape[0]) == 0 if n=='first' else ucs < 0
+        locs = [0] if n == "first" else np.where(ucs < 0)[0]
+
+        if op == "leave":
+            pass
+        elif op == "drop":
+            # ucs = ucs[~locs]
+            ucs = np.delete(ucs, locs)
+        elif isinstance(op, (int, float)):
+            ucs[locs] = op
+        elif isinstance(op, str) and op.lower() == "zero":
+            ucs[locs] = 0
+        elif (
+            pd.isnull(op)
+            or op is None
+            or isinstance(op, str)
+            and op.lower() in nan_list
+        ):
+            ucs[locs] = np.nan
+        else:
+            raise ValueError(n, op)
+
+    if nr:
+        ucs = ucs[-nr:]
+
+    return ucs
+
+    """else:
+        #ucs = []
+        for i,v in enumerate(_iterable[:0:-1]):
+            dif = v - _iterable[-2-i]
+            
+            if excl_negatives and dif < 0: continue
+            else: ucs.append(dif)
+            
+            if nr and len(ucs) >= nr:
+                break
+            
+        ucs = ucs[::-1]"""
+
+
+def _check_limits(limits):
+    if len(limits) != 2:
+        raise ValueError("Limits must contain 2 elements; got: {}".format(len(limits)))
+
+    if limits[0] is not None and limits[0] > 0:
+        raise ValueError("First limit must be <= 0; got: {}".format(limits[0]))
+
+    if limits[1] is not None and limits[1] < 0:
+        raise ValueError("Second limit must be >= 0; got: {}".format(limits[1]))
+
+    if sum(x == 0 for x in limits) == 1 and None not in limits:
+        raise ValueError(
+            "Either both limits must be 0 or neither of them; got: {}".format(limits)
+        )
+
+    return True
+
+
+def limiter(A, limits, closed="both"):
+    if closed not in ("both", "left", "right", "neither", None):
+        raise ValueError(
+            "`closed` must be one of the following: (both,left,right,neither); got: {}".format(
+                closed
+            )
+        )
+    L0, L1 = limits
+
+    if L0 is not None:
+        op = (
+            lambda x, y: x >= y
+            if closed in ("both", "left", None)
+            else lambda x, y: x > y
+        )
+        A = np.where(op(A, L0), A, np.nan)
+    if L1 is not None:
+        op = (
+            lambda x, y: x <= y
+            if closed in ("both", "right", None)
+            else lambda x, y: x < y
+        )
+        A = np.where(op(A, L1), A, np.nan)
+
+    if A.ndim > 1:
+        return A[~np.isnan(A).any(axis=1)]
+    else:
+        return A[~np.isnan(A)]
+
+
+def randomize_summation(
+    _sum, n, limits=(-0.3, 0.3), closed="both", *, factor=15, sample_size=10
+):
+    limit_vs = (None, None)
+    mean = 1 / n
+
+    if limits is not None:
+        _check_limits(limits)
+        limit_vs = [mean * (1 + L) if L is not None else L for L in limits]
+
+    if all(x == 0 for x in limit_vs):
+        if closed not in ("both", None):
+            raise ValueError(
+                "`closed` must be 'both' if both limits are 0; got: {}".format(closed)
+            )
+        return np.ones(n) * mean
+
+    while True:
+        # A is a 2d array even if sample_size=1
+        A = np.random.dirichlet(np.ones(n) * factor, size=sample_size)
+
+        A2 = limiter(A, limit_vs, closed=closed)
+
+        if not A2.shape[0]:
+            factor *= 2
+            # print(factor)
+        else:
+            break
+
+    return A2[0] * _sum
+
+
+def weight_limiter(A, weight_limits, closed="both"):
+    if closed not in ("both", "left", "right", "neither", None):
+        raise ValueError(
+            "`closed` must be one of the following: (both,left,right,neither); got: {}".format(
+                closed
+            )
+        )
+
+    op1 = (
+        (lambda x, y: x >= y)
+        if closed in ("both", "left", None)
+        else (lambda x, y: x > y)
+    )
+    op2 = (
+        (lambda x, y: x <= y)
+        if closed in ("both", "right", None)
+        else (lambda x, y: x < y)
+    )
+    AT = A.transpose()
+    at = []
+
+    for i, limits in enumerate(weight_limits):
+        L0, L1 = limits
+        ATi = AT[i]
+        if L0 is not None:
+            ATi = np.where(op1(ATi, L0), ATi, np.nan)
+        if L1 is not None:
+            ATi = np.where(op2(ATi, L1), ATi, np.nan)
+        at.append(ATi)
+
+    AT = np.asarray(at, dtype=np.float64)
+    A = AT.transpose()
+
+    if A.ndim > 1:
+        return A[~np.isnan(A).any(axis=1)]
+    else:
+        return A[~np.isnan(A)]
+
+
+def randomize_weights(
+    weights, limits=(-0.3, 0.3), closed="both", *, factor=15, sample_size=10
+):
+    weights = np.asarray(weights, dtype=np.float64)
+    _sum = weights.sum()
+    limit_vs = [(None, None)] * weights.size
+
+    if limits is not None:
+        _check_limits(limits)
+        limit_vs = [
+            [w * (1 + L) if L is not None else L for L in limits] for w in weights
+        ]
+
+    if all(x == 0 for x in limit_vs):
+        if closed not in ("both", None):
+            raise ValueError(
+                "`closed` must be 'both' if both limits are 0; got: {}".format(closed)
+            )
+        return weights
+
+    while True:
+        # A is a 2d array even if sample_size=1
+        A = np.random.dirichlet(weights * factor, size=sample_size) * _sum
+
+        A2 = weight_limiter(A, limit_vs, closed=closed) if limits is not None else A
+
+        if not A2.shape[0]:
+            factor *= 2
+            # print(factor)
+        else:
+            break
+
+    return A2[0]
+
+
+# ----------------------------------------------------------------------------
+def verify_uniqueness(obj, index=True, columns=True, name=None):
+    if isinstance(obj, pd.Series):
+        columns = False
+
+    if name is None:
+        name_str = ""
+    else:
+        name_str = "{}'s "
+
+    for attr, include in (("index", index), ("columns", columns)):
+        if not include:
+            continue
+
+        ind = getattr(obj, attr)
+        ind_duplicated = ind[ind.duplicated()]
+        if not ind_duplicated.shape[0]:
+            continue
+
+        raise ValueError(
+            "Duplicates in {}{}: {}".format(name_str, attr, ind_duplicated)
+        )
+
+
+def _get_valid(obj, valid_col=None, valid_func=None):
+    # last_index = obj[valid_col].last_valid_index()
+    is_series = isinstance(obj, pd.Series)
+
+    if is_series:
+        check_cols = [obj]
+    elif valid_col:
+        check_cols = [obj[valid_col]]
+    else:
+        check_cols = [x[1] for x in obj.iteritems()]
+
+    last_index = -1
+    obj_index = obj.index
+
+    for s in check_cols:
+        if valid_func:
+            valid_indexes = s.apply(valid_func)
+            if not valid_indexes.shape[0]:
+                continue
+            last_index = max(last_index, obj_index[valid_indexes][-1])
+            continue
+
+        valid_index = obj.last_valid_index()
+        if valid_index is not None:
+            continue
+        last_index = max(last_index, valid_index)
+
+    return last_index
+
+
+def pd_replace(obj, obj2, start=None, valid_col=None, valid_func=None, simple=True):
+    """If simple=True, then obj nor obj2 must contain non-unique indexes/columns.
+    Otherwise if start has multiple matches in obj.index, last is chosen."""
+    is_series = isinstance(obj, pd.Series)
+    if simple:
+        [
+            verify_uniqueness(objx, columns=b_col, name=name)
+            for objx, b_col, name in ((obj, True, "obj"), (obj2, False, "obj2"))
+        ]
+
+    if start is None:
+        last_index = _get_valid(obj, valid_col, valid_func)
+
+        if last_index != -1:
+            entry_iloc = obj.index.get_loc(last_index) + 1
+        else:
+            entry_iloc = 0
+
+    else:
+        entry_iloc = obj.index.get_loc(start)
+
+    if isinstance(entry_iloc, np.ndarray):
+        # index was not unique, multiple matches
+        entry_iloc = np.where(entry_iloc)[0][-1]
+
+    end_iloc = entry_iloc + obj2.shape[0]
+    missing = end_iloc - obj.shape[0]
+
+    if missing > 0:
+        I = IndexError("Obj short of {} rows".format(missing))
+        I.missing = missing
+        raise I
+
+    # Note (example):
+    # obj.index = [0,0] + list(obj.index[2:])
+    # obj.iloc[0:2] = obj2
+    # -> now both rows (0,0) are overwritten with the matching row of obj2
+    # However, if obj2 has duplicates (0,0), it will not work
+
+    if is_series:
+        obj.iloc[entry_iloc:end_iloc] = obj2.values
+
+    elif simple:
+        ind0 = obj2.index
+        obj2.index = obj.index[entry_iloc:end_iloc]
+
+        overlapping_cols = np.where(obj.columns.isin(obj2.columns))[0]
+        obj.iloc[entry_iloc:end_iloc, overlapping_cols] = obj2
+
+        obj2.index = ind0
+
+    else:
+        obj_cols = obj.columns
+        obj2_cols = obj2.columns
+        obj2_cols_uniq_ind = np.where(~obj2_cols.duplicated())
+
+        for col2_iloc in obj2_cols_uniq_ind:
+            col2 = obj2_cols[col2_iloc]
+
+            try:
+                col_iloc = obj_cols.get_loc(col2)
+            except KeyError:
+                continue
+
+            obj2_values = obj2.iloc[:, col2_iloc].values
+
+            if isinstance(col_iloc, np.ndarray):
+                col_iloc = np.where(col_iloc)[0]
+                # list of matching columns (with identical name)
+                obj2_values = [obj2_values for x in col_iloc]
+
+            obj.iloc[entry_iloc:end_iloc, col_iloc] = obj2_values
+
+
+if __name__ == "__main__":
+    # print(randomize_summation(15.4,5))
+    weights = [0.2, 0.8, 0.4, 0.6]
+    rw = randomize_weights(weights, limits=(-0.05, 0.05))
+    print(rw)
+
+    tp = get_timestamps([np.timedelta64(td(minutes=60)), td(minutes=30)])
+    print(tp)
+    tp2 = get_timestamps(np.timedelta64(td(minutes=60)))
+    print(tp2)
+    tp3 = get_timestamps(dt(2016, 1, 1), "np.datetime64")
+    print(tp3)
+    tp4 = get_timestamps([td(days=60), dt(2016, 1, 1)], "pydatetime")
+    print(tp4)
+    print("\n Get_period_entries:")
+
+    tp5 = (dt(2000, 1, 1), dt(2000, 1, 1, 5))
+    pe = get_period_entries(tp5[0], tp5[1], freq=td(hours=1), exclude_end=False)
+    for i, x in enumerate(pe[:-1]):
+        x2 = pe[i + 1]
+        print([x, x2])
+
+        tp6 = get_timestamps((x, x2))
+        print(tp6)
+
+        tp7 = get_timestamps(tp6, "pd.TimeStamp")
+        begin, end = tp7
+        print((begin, end), "\n")
+
+    tp8 = get_timestamps(["1D", None])
+    print(tp8)
+
+    tp9 = get_timestamps([dt(2000, 1, 1), None])
+    print(tp9)
+
+    so = slice_obj(pd.Series(np.arange(6), index=pe), (pe[2], td(hours=2)))
+    print(so)
+    so2 = slice_obj(list(pe), (pe[2], td(hours=2)))
+    print(so2)
```

### Comparing `fons-0.3.1/fons/nan.py` & `fons-0.4.0/fons/nan.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,73 +1,75 @@
-import pandas as pd
-import numpy as np
-import math
-
-from fons.pyops import compare
-
-
-class Implemented:
-    def __init__(self, na_values=[]):
-        self.na_values = tuple(na_values)
-        
-
-    def __call__(self, *args):
-        return self.all(*args)
-    
-
-    def any(self, *args):
-        if not len(args):
-            return False
-        
-        if all(  isinstance(x, Implemented) or
-                 any(compare(x,na) for na in self.na_values) or
-                 type(x) is type and issubclass(x, Implemented)
-               for x in args):
-            return False
-        
-        return True
-
-
-    def all(self, *args):
-        if not len(args):
-            return False
-        
-        if any(  isinstance(x, Implemented) or
-                 any(compare(x,na) for na in self.na_values) or
-                 type(x) is type and issubclass(x, Implemented)
-               for x in args):
-            return False
-        
-        return True
-
-
-    def __bool__(self):
-        return False
-
-    def __str__(self):
-        return 'nan'
-
-
-#Any instance of Implemented is not implemented
-# Impd(Impd) -> False
-#Nor is Implemented class itself implemented
-# Impd(Implemented) -> False
-
-Impd = impd = nan = Implemented()
-nImpd = Implemented([None])
-pdImpd = Implemented([None, math.nan, np.nan, pd.NaT])
-
-
-def is_implemented(*objects, **kw):
-    if 'na_values' in kw:
-        _impd = Implemented(kw['na_values'])
-    else:
-        _impd = Impd
-    return _impd(*objects)
-
-
-if __name__ == '__main__':
-    print(Impd(Implemented))
-    print(Impd(nan))
-    print(Impd(None))
-    print(Impd(None,Implemented))
-    print(Impd(None,nan))
+import pandas as pd
+import numpy as np
+import math
+
+from fons.pyops import compare
+
+
+class Implemented:
+    def __init__(self, na_values=[]):
+        self.na_values = tuple(na_values)
+
+    def __call__(self, *args):
+        return self.all(*args)
+
+    def any(self, *args):
+        if not len(args):
+            return False
+
+        if all(
+            isinstance(x, Implemented)
+            or any(compare(x, na) for na in self.na_values)
+            or type(x) is type
+            and issubclass(x, Implemented)
+            for x in args
+        ):
+            return False
+
+        return True
+
+    def all(self, *args):
+        if not len(args):
+            return False
+
+        if any(
+            isinstance(x, Implemented)
+            or any(compare(x, na) for na in self.na_values)
+            or type(x) is type
+            and issubclass(x, Implemented)
+            for x in args
+        ):
+            return False
+
+        return True
+
+    def __bool__(self):
+        return False
+
+    def __str__(self):
+        return "nan"
+
+
+# Any instance of Implemented is not implemented
+# Impd(Impd) -> False
+# Nor is Implemented class itself implemented
+# Impd(Implemented) -> False
+
+Impd = impd = nan = Implemented()
+nImpd = Implemented([None])
+pdImpd = Implemented([None, math.nan, np.nan, pd.NaT])
+
+
+def is_implemented(*objects, **kw):
+    if "na_values" in kw:
+        _impd = Implemented(kw["na_values"])
+    else:
+        _impd = Impd
+    return _impd(*objects)
+
+
+if __name__ == "__main__":
+    print(Impd(Implemented))
+    print(Impd(nan))
+    print(Impd(None))
+    print(Impd(None, Implemented))
+    print(Impd(None, nan))
```

### Comparing `fons-0.3.1/fons/net/url.py` & `fons-0.4.0/fons/net/url.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,190 +1,252 @@
 from http.client import HTTPConnection
-from urllib.parse import (urlparse, urlunparse)
+from urllib.parse import urlparse, urlunparse
 
 from urllib.request import urlopen
 import requests
 
-from fons.net.urlstr import (find_urls, filter_urls)
+from fons.net.urlstr import find_urls, filter_urls
 
 import datetime
+
 dt = datetime.datetime
 td = datetime.timedelta
 
 import math
-#from threading import Thread
+
+# from threading import Thread
 from concurrent.futures import ThreadPoolExecutor, as_completed
 
 import logging
 
-UTM_QUERY_PARAMS = ['utm_source','utm_medium','utm_campaign','utm_term','utm_content']
-STRIP_PARAMS = ['cmpid%3D','cmpid%2D','cmpid','__source','mod','link','xid','ncid','sr_share','_cookie-check','dcmp','ftag'] + UTM_QUERY_PARAMS
+UTM_QUERY_PARAMS = [
+    "utm_source",
+    "utm_medium",
+    "utm_campaign",
+    "utm_term",
+    "utm_content",
+]
+STRIP_PARAMS = [
+    "cmpid%3D",
+    "cmpid%2D",
+    "cmpid",
+    "__source",
+    "mod",
+    "link",
+    "xid",
+    "ncid",
+    "sr_share",
+    "_cookie-check",
+    "dcmp",
+    "ftag",
+] + UTM_QUERY_PARAMS
 
 
 def expand_url_http(url, limit=5, timeout=None, as_absolute=False, **kw):
-    """The HTTPConnection variant of expand_url. 
-    Does not work on certain urls, e.g. those starting with https://t.co/... """
-    seen = kw.get('seen')
-    if seen is None: seen = []
-    
+    """The HTTPConnection variant of expand_url.
+    Does not work on certain urls, e.g. those starting with https://t.co/..."""
+    seen = kw.get("seen")
+    if seen is None:
+        seen = []
+
     if not len(seen) or seen[-1] != url:
         seen.append(url)
-        logging.debug('Expanding: {}'.format(url))
+        logging.debug("Expanding: {}".format(url))
 
-    return_seen = kw.get('return_seen')
-    if return_seen is None: return_seen = False
-    
-    start = kw.get('start',dt.utcnow())
+    return_seen = kw.get("return_seen")
+    if return_seen is None:
+        return_seen = False
+
+    start = kw.get("start", dt.utcnow())
     timeout_left = timeout
     if timeout is not None and as_absolute:
-        timeout_left = max(0, round(timeout-(dt.utcnow() - start).total_seconds(), 2))
-        
-    exclude_domains = kw.get('exclude_domains')
-    if exclude_domains is None: exclude_domains = []
+        timeout_left = max(0, round(timeout - (dt.utcnow() - start).total_seconds(), 2))
+
+    exclude_domains = kw.get("exclude_domains")
+    if exclude_domains is None:
+        exclude_domains = []
     parsed = urlparse(url)
-    
-    if parsed.netloc in exclude_domains: pass
+
+    if parsed.netloc in exclude_domains:
+        pass
     elif limit is None or limit > 0:
         h = HTTPConnection(parsed.netloc, timeout=timeout_left)
         resource = parsed.path
         if parsed.query != "":
             resource += "?" + parsed.query
-        h.request('HEAD', resource )
+        h.request("HEAD", resource)
         response = h.getresponse()
-    
-        location = response.getheader('Location')
-        #print(response.status,location)
-        
-        if not location: pass
-        elif int(response.status/100) != 3: pass
+
+        location = response.getheader("Location")
+        # print(response.status,location)
+
+        if not location:
+            pass
+        elif int(response.status / 100) != 3:
+            pass
         elif response.status == 302:
-            #301 is sometimes final, 302 seems to be always final
+            # 301 is sometimes final, 302 seems to be always final
             url = location
-            try: assert seen[-1] != url
-            except (IndexError,AssertionError):pass
-            else: seen.append(url)
-            
+            try:
+                assert seen[-1] != url
+            except (IndexError, AssertionError):
+                pass
+            else:
+                seen.append(url)
+
         elif location not in seen:
-            new_limit = limit -1 if limit is not None else None
-            return expand_url_http(location, new_limit, timeout, as_absolute, 
-                              seen=seen, start=start, return_seen=return_seen, exclude_domains=exclude_domains)
-    
+            new_limit = limit - 1 if limit is not None else None
+            return expand_url_http(
+                location,
+                new_limit,
+                timeout,
+                as_absolute,
+                seen=seen,
+                start=start,
+                return_seen=return_seen,
+                exclude_domains=exclude_domains,
+            )
+
     if return_seen:
         return seen
-    
+
     return url
 
 
 def expand_url(url, limit=5, timeout=None, as_absolute=False, **kw):
-    session = kw.get('session')
+    session = kw.get("session")
     if session is None:
         session = requests.session()
-    seen = kw.get('seen')
-    if seen is None: seen = []
-    
+    seen = kw.get("seen")
+    if seen is None:
+        seen = []
+
     if not len(seen) or seen[-1] != url:
         seen.append(url)
-        logging.debug('Expanding: {}'.format(url))
+        logging.debug("Expanding: {}".format(url))
 
-    return_seen = kw.get('return_seen')
-    if return_seen is None: return_seen = False
-    
-    start = kw.get('start',dt.utcnow())
+    return_seen = kw.get("return_seen")
+    if return_seen is None:
+        return_seen = False
+
+    start = kw.get("start", dt.utcnow())
     timeout_left = timeout
     if timeout is not None and as_absolute:
-        timeout_left = max(0, round(timeout-(dt.utcnow() - start).total_seconds(), 2))
-        
-    exclude_domains = kw.get('exclude_domains')
-    if exclude_domains is None: exclude_domains = []
+        timeout_left = max(0, round(timeout - (dt.utcnow() - start).total_seconds(), 2))
+
+    exclude_domains = kw.get("exclude_domains")
+    if exclude_domains is None:
+        exclude_domains = []
     parsed = urlparse(url)
-    
-    if parsed.netloc in exclude_domains: pass
+
+    if parsed.netloc in exclude_domains:
+        pass
     elif limit is None or limit > 0:
-        #response = requests.head(url,allow_redirects=False,timeout=timeout_left)
-        response = session.head(url,allow_redirects=False,timeout=timeout_left)
-        location = response.headers.get('location')
-        #print(response.status_code,location)
-        
-        if not location: pass
-        elif int(response.status_code/100) != 3: pass
+        # response = requests.head(url,allow_redirects=False,timeout=timeout_left)
+        response = session.head(url, allow_redirects=False, timeout=timeout_left)
+        location = response.headers.get("location")
+        # print(response.status_code,location)
+
+        if not location:
+            pass
+        elif int(response.status_code / 100) != 3:
+            pass
         elif response.status_code == 302:
-            #301 is sometimes final, 302 seems to be always final
+            # 301 is sometimes final, 302 seems to be always final
             url = location
-            try: assert seen[-1] != url
-            except (IndexError,AssertionError):pass
-            else: seen.append(url)
-            
+            try:
+                assert seen[-1] != url
+            except (IndexError, AssertionError):
+                pass
+            else:
+                seen.append(url)
+
         elif location not in seen:
-            new_limit = limit -1 if limit is not None else None
-            return expand_url(location, new_limit, timeout, as_absolute, session=session,
-                              seen=seen, start=start, return_seen=return_seen, exclude_domains=exclude_domains)
-    
+            new_limit = limit - 1 if limit is not None else None
+            return expand_url(
+                location,
+                new_limit,
+                timeout,
+                as_absolute,
+                session=session,
+                seen=seen,
+                start=start,
+                return_seen=return_seen,
+                exclude_domains=exclude_domains,
+            )
+
     if return_seen:
         return seen
-    
+
     return url
 
 
 def expand(urls, max_concurrent=50, timeout=20, **kw):
     """It's recommended to NOT set timeout to absolute, due to threads not processing in synchronized manner"""
     """len_urls = len(urls)
     pool_size = min(len_urls,max_concurrent)
     nr_packs = ceil(len_urls/pool_size)"""
-    single = isinstance(urls,str)
-    if single: urls = [urls] 
-    
-    return_seen = kw.get('return_seen')
-    if return_seen is None: return_seen=False
-    
-    seen = kw.get('seen')
-    try: kw.pop('seen')
-    except KeyError: pass
-    
+    single = isinstance(urls, str)
+    if single:
+        urls = [urls]
+
+    return_seen = kw.get("return_seen")
+    if return_seen is None:
+        return_seen = False
+
+    seen = kw.get("seen")
+    try:
+        kw.pop("seen")
+    except KeyError:
+        pass
+
     if seen is None and return_seen:
         seen = []
 
     def get_seen(i):
-        try: 
+        try:
             return seen[i]
-        except (TypeError,IndexError):
+        except (TypeError, IndexError):
             pass
-        
+
         item = []
         if seen is not None:
-            seen.append(item) 
-        
+            seen.append(item)
+
         return item
-        
 
-    #for i in range(nr_packs):
+    # for i in range(nr_packs):
     with ThreadPoolExecutor(max_workers=max_concurrent) as executor:
         future_to_url = {
-            executor.submit(
-                expand_url, url, seen=get_seen(j), timeout=timeout, **kw
-            ): [j,url] for j,url in enumerate(urls)
-        } #[i*pool_size:(i+1)*pool_size]])
-        
+            executor.submit(expand_url, url, seen=get_seen(j), timeout=timeout, **kw): [
+                j,
+                url,
+            ]
+            for j, url in enumerate(urls)
+        }  # [i*pool_size:(i+1)*pool_size]])
+
         for future in as_completed(future_to_url):
             pk = future_to_url[future]
 
             try:
                 data = future.result()
                 pk.append(data)
             except Exception as exc:
                 if return_seen:
                     seen = get_seen(pk[0])
                     seen.append(None)
                     pk.append(seen)
-                else: pk.append(None)
-                #print('%r generated an exception: %s' % (pk[1], exc))
+                else:
+                    pk.append(None)
+                # print('%r generated an exception: %s' % (pk[1], exc))
             """else:
                 print('%r page is %d bytes' % (pk[1], len(data)))"""
-                              
-    expanded = [x[2] for x in sorted(future_to_url.values(), key= lambda x:x[0])]
-    
+
+    expanded = [x[2] for x in sorted(future_to_url.values(), key=lambda x: x[0])]
+
     return expanded if not single else expanded[0]
 
 
 """def expand2(urls,max_concurrent=200,**kw):
     import multiprocessing
 
     len_urls = len(urls)
@@ -203,116 +265,122 @@
     nr_packs = ceil(len_urls/pool_size)
     
     for i in range(nr_packs):
         outputs += pool.map(w_unshorten_url, urls[i*pool_size:(i+1)*pool_size])
         
     return outputs
     #threads = [Thread(target=extend_url,args=[url,levels,timeout]) for url in urls]"""
-    
+
 
 session = None
 
-#Slower version
+
+# Slower version
 def expand_url2(url, timeout=10, **kw):
     global session
     if not session:
         session = requests.session()
-    
+
     r = session.head(url, allow_redirects=True, timeout=timeout)
     e_url = r.url
-        
+
     """"r = urlopen(url,timeout=timeout)
     e_url = r.geturl()"""
 
     return e_url
 
 
 def expand_in_text(text, max_len=None, strip_params=STRIP_PARAMS, **kw):
     match = find_urls(text)
     urls = [x.str for x in match]
     seen = []
-    kw.update({'seen': seen, 
-               'exclude_domains': ['youtu.be']})
-        
+    kw.update({"seen": seen, "exclude_domains": ["youtu.be"]})
+
     expand(urls, **kw)
 
-    _strip = globals()['strip_params']
+    _strip = globals()["strip_params"]
+
     def strip_url(url):
         stripped = _strip(url, strip_params)
         if max_len is not None and len(stripped) > max_len:
             return None
         return stripped
 
     stripped = ([strip_url(y) if y else y for y in x] for x in seen)
     expanded = list(stripped)
-    expanded_last_nonna = [next((y for y in reversed(x) if y),None) for x in expanded]
-            
-    for m,url in reversed(list(zip(match,expanded_last_nonna))):
-        text = '{}{}{}'.format(text[:m.pos],(url if url else m.str),text[m.end:])
+    expanded_last_nonna = [next((y for y in reversed(x) if y), None) for x in expanded]
+
+    for m, url in reversed(list(zip(match, expanded_last_nonna))):
+        text = "{}{}{}".format(text[: m.pos], (url if url else m.str), text[m.end :])
     return text
-        
+
 
 def strip_params(url, params):
     up = urlparse(url)
-    split = up.query.split('&')
-    
+    split = up.query.split("&")
+
     if params is not True:
-        query_new = '&'.join(x for x in split if x[:x.find('=')].lower() not in params)
-    else:query_new = ''
-    
+        query_new = "&".join(x for x in split if x[: x.find("=")].lower() not in params)
+    else:
+        query_new = ""
+
     up2 = up._replace(query=query_new)
-    
+
     return urlunparse(up2)
-    
-    
+
+
 def strip_utm(url):
     return strip_params(url, UTM_QUERY_PARAMS)
 
 
 def strip_www(url):
     low = url.lower()
-    if low.startswith('https://www.') or low.startswith('http://www.'):
-        loc = low.find('www.')
-        url =  url[:loc] + url[loc+len('www.'):]
-    
-    return url
+    if low.startswith("https://www.") or low.startswith("http://www."):
+        loc = low.find("www.")
+        url = url[:loc] + url[loc + len("www.") :]
 
+    return url
 
 
-#The old version of expand_url:
+# The old version of expand_url:
 def extend_url(url, levels=None, timeout=10, **kw):
-    lvl = kw.get('lvl',0)
+    lvl = kw.get("lvl", 0)
     if levels is not None and lvl >= levels:
         return url
     elif len(url) > 32:
         return url
-        
-    r = urlopen(url,timeout=timeout)
+
+    r = urlopen(url, timeout=timeout)
     e_url = r.geturl()
     lvl += 1
-    #print(lvl,e_url)
+    # print(lvl,e_url)
 
     if url != e_url:
-        extend_url(e_url,levels,timeout,lvl=lvl)
+        extend_url(e_url, levels, timeout, lvl=lvl)
 
     return e_url
 
 
-
-
-if __name__ == '__main__':
+if __name__ == "__main__":
     url = "https://t.co/L0t4lQ3hT7"
     e_url = extend_url(url, levels=5)
-    #print(e_url)
+    # print(e_url)
 
     seen = []
     e_url = expand_url(url, limit=5, seen=seen)
-    print('{}\n{}'.format(e_url, seen))
+    print("{}\n{}".format(e_url, seen))
     print(strip_utm(e_url))
-    
+
     seen = []
-    print(expand(['https://bit.ly/2rwwupw','https://bit.ly/2I6HWDu',
-                      'https://t.co/ydBPKn4wO0','http://t.co/hAplNMmSTg',
-                      'http://f-st.co/THHI6hC',
-                      ],seen=seen))
+    print(
+        expand(
+            [
+                "https://bit.ly/2rwwupw",
+                "https://bit.ly/2I6HWDu",
+                "https://t.co/ydBPKn4wO0",
+                "http://t.co/hAplNMmSTg",
+                "http://f-st.co/THHI6hC",
+            ],
+            seen=seen,
+        )
+    )
     print(seen)
-
```

### Comparing `fons-0.3.1/fons/net/urlstr.py` & `fons-0.4.0/fons/net/urlstr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,209 +1,213 @@
 import re
 from collections import namedtuple
+
 try:
     from urllib import urlencode
 except ImportError:
     from urllib.parse import urlencode
 
-match_t = namedtuple('Match', 'pos end str')
+match_t = namedtuple("Match", "pos end str")
 
-asc = ''.join([chr(i) for i in range(128)])
-alphanum = re.sub('[\W_]+','',asc)
-symbols = re.sub('[{}]+'.format(alphanum),'',asc)
+asc = "".join([chr(i) for i in range(128)])
+alphanum = re.sub("[\W_]+", "", asc)
+symbols = re.sub("[{}]+".format(alphanum), "", asc)
 
-PROBABLY_INVALID_END = re.sub('[?+/&]+','',symbols)
-#PROBABLY_INVALID_END = ['.,;:@!?()[]{}=']
+PROBABLY_INVALID_END = re.sub("[?+/&]+", "", symbols)
+# PROBABLY_INVALID_END = ['.,;:@!?()[]{}=']
 
-#if url doesn't end with an alphanum, it is probably not necessary
+# if url doesn't end with an alphanum, it is probably not necessary
 #  (except some rare cases, e.g. it ending with a token containing symbols)
 
-PATTERN = 'http[s]?://(?:[a-zA-Z]|[0-9]|[$-_@.&+~]|[!*\(\),]|(?:%[0-9a-fA-F][0-9a-fA-F]))+'
-URL_SYMBOLS = alphanum + ':/' + '$-_.+!*\'()~#[]@,;=' + '?&='
+PATTERN = (
+    "http[s]?://(?:[a-zA-Z]|[0-9]|[$-_@.&+~]|[!*\(\),]|(?:%[0-9a-fA-F][0-9a-fA-F]))+"
+)
+URL_SYMBOLS = alphanum + ":/" + "$-_.+!*'()~#[]@,;=" + "?&="
 
 
 def correct_old(new_match, correct={}, **kw):
-    if not correct.get('indexes'):
+    if not correct.get("indexes"):
         return
-    
-    old = correct['indexes']
+
+    old = correct["indexes"]
     """for match in old:
         if new_match"""
-    
+
 
 def _get_url_indexes(txt):
     txt2 = txt.lower()
     i = 0
     indexes = []
 
-    check = ('http://','https://','www.')
+    check = ("http://", "https://", "www.")
     lens = [len(c) for c in check]
-    check_itms = list(zip(check,lens))
-    min_address_part = 3 #site http://a.b
-    
+    check_itms = list(zip(check, lens))
+    min_address_part = 3  # site http://a.b
+
     while True:
         len_txt = len(txt)
-        if i +4 > len_txt:
+        if i + 4 > len_txt:
             break
-        #print(i)
-        #print(txt[i:])
+        # print(i)
+        # print(txt[i:])
         detected = False
-        
-        for c,ln in check_itms:
-            #print("AA",txt2[i-ln:i])
-            if i+ln > len_txt:
+
+        for c, ln in check_itms:
+            # print("AA",txt2[i-ln:i])
+            if i + ln > len_txt:
                 continue
-            elif txt2[i:i+ln] != c:
+            elif txt2[i : i + ln] != c:
                 continue
-            
+
             nxt_i = i + ln
-            #print(txt2[i-ln:i])
-            
-            if c in check[:2] and txt2[nxt_i:nxt_i+4] == 'www.':
+            # print(txt2[i-ln:i])
+
+            if c in check[:2] and txt2[nxt_i : nxt_i + 4] == "www.":
                 nxt_i += 4
 
             """if txt[i-1] != " ":
                 txt = txt[:i] + " " + txt[i:]
                 txt2 = txt2[:i] + " " + txt2[i:]
                 nxt_i += 1
                 i + = 1"""
 
             indexes.append(i)
 
-            #nxt_i += min_address_part
+            # nxt_i += min_address_part
             i = nxt_i
             detected = True
             break
 
         if not detected:
-            i+=1
+            i += 1
 
     return indexes
 
 
 def _get_urls(txt):
     indexes = _get_url_indexes(txt)
     len_ind = len(indexes)
-    #print(indexes)
+    # print(indexes)
 
     matches = []
-    
-    for k,i in enumerate(indexes):
-        if k < len_ind-1:
-            i2 = indexes[k+1]
-        else:i2 = len(txt)
+
+    for k, i in enumerate(indexes):
+        if k < len_ind - 1:
+            i2 = indexes[k + 1]
+        else:
+            i2 = len(txt)
 
         txt_part = txt[i:i2]
 
         """space_loc = txt_part.find(" ")
         
         if space_loc != -1:
             part2 = txt_part[:space_loc]
         else:part2 = txt_part"""
 
-        end = next((j for j,x in enumerate(txt_part) if x not in URL_SYMBOLS),len(txt_part))
+        end = next(
+            (j for j, x in enumerate(txt_part) if x not in URL_SYMBOLS), len(txt_part)
+        )
         url = txt_part[:end]
 
-        #eliminating accidental concatenings:
+        # eliminating accidental concatenings:
         url = url.strip(PROBABLY_INVALID_END)
-        #www.goole.com/. Next sentence -> www.goole.com/
-        #www.goole.com/page.Next sentence  -> www.goole.com/page.Next
+        # www.goole.com/. Next sentence -> www.goole.com/
+        # www.goole.com/page.Next sentence  -> www.goole.com/page.Next
         # (in cases similar to that it'd be too difficult to tell if the end is part of the link or not)
 
-        match = match_t(i,i+len(url),url)
-        
+        match = match_t(i, i + len(url), url)
+
         matches.append(match)
 
     return matches
 
 
 def find_urls(txt, return_match=True):
     match = _get_urls(txt)
     if not return_match:
         return [m.str for m in match]
 
     return match
-        
-    
-def filter_urls(txt, replace=':url:', **kw):
-    match = kw.get('match')
+
+
+def filter_urls(txt, replace=":url:", **kw):
+    match = kw.get("match")
     if match is None:
         match = find_urls(txt)
 
     for x in reversed(match):
-        txt = txt[:x[0]] + replace + txt[x[1]:]
+        txt = txt[: x[0]] + replace + txt[x[1] :]
 
     return txt
 
 
-
-#------------------------------------------
-#A DIFFERENT METHOD (excludes www. and non spaced links)
+# ------------------------------------------
+# A DIFFERENT METHOD (excludes www. and non spaced links)
 def _prepare_text(txt):
     txt2 = txt.lower()
-    #indexes = []
+    # indexes = []
     i = len(txt)
 
-    check = ('http://','https://','www.')
+    check = ("http://", "https://", "www.")
     lens = [len(c) for c in check]
-    check_itms = list(zip(check,lens))
-    min_address_part = 3 #site http://a.b
-    
+    check_itms = list(zip(check, lens))
+    min_address_part = 3  # site http://a.b
+
     while True:
         if i - 4 < 0:
             break
-        #print(i)
-        #print(txt[i:])
+        # print(i)
+        # print(txt[i:])
         detected = False
-        
-        for c,ln in check_itms:
-            #print("AA",txt2[i-ln:i])
-            if i-ln < 0:
+
+        for c, ln in check_itms:
+            # print("AA",txt2[i-ln:i])
+            if i - ln < 0:
                 continue
-            elif txt2[i-ln:i] != c:
+            elif txt2[i - ln : i] != c:
                 continue
-            
+
             nxt_i = i - ln
-            #print(txt2[i-ln:i])
-            
-            if c == 'www.':
-                for c2,ln2 in check_itms[:2]:
-                    if nxt_i-ln2 <0: continue
-                    elif txt2[nxt_i-ln2:nxt_i] == c2:
+            # print(txt2[i-ln:i])
+
+            if c == "www.":
+                for c2, ln2 in check_itms[:2]:
+                    if nxt_i - ln2 < 0:
+                        continue
+                    elif txt2[nxt_i - ln2 : nxt_i] == c2:
                         nxt_i -= ln2
                         break
 
-            if nxt_i>0 and txt[nxt_i-1] != " ":
+            if nxt_i > 0 and txt[nxt_i - 1] != " ":
                 txt = txt[:nxt_i] + " " + txt[nxt_i:]
                 txt2 = txt2[:nxt_i] + " " + txt2[nxt_i:]
                 nxt_i -= 1
 
-
             nxt_i -= min_address_part
             i = nxt_i
             detected = True
             break
 
         if not detected:
-            i-=1
+            i -= 1
 
     return txt
 
 
-def filter_links(txt,replace=':url:',filter_end=True):
-    #txt = _prepare_text(txt)
-    
+def filter_links(txt, replace=":url:", filter_end=True):
+    # txt = _prepare_text(txt)
+
     if not filter_end:
-        return re.sub(PATTERN,replace,txt)
+        return re.sub(PATTERN, replace, txt)
 
-        
-    matches = find_links(txt,filter_end=True,is_prepared=True)
+    matches = find_links(txt, filter_end=True, is_prepared=True)
 
     for x in reversed(matches):
-        txt = txt[:x[0]] + replace + txt[x[1]:]
+        txt = txt[: x[0]] + replace + txt[x[1] :]
 
     return txt
 
     """
     len_txt = len(txt)
     for _id in ('http://', 'https://'):
         try:
@@ -211,78 +215,75 @@
                 i = txt.index(_id)
                 end = next((i+j for j,x in enumerate(txt[i:]) if x == " "),len_txt)
                 txt = txt[:i] + replace + txt[end:]
             
         except ValueError: pass
 
     return txt"""
-    
+
 
 def find_links(txt, filter_end=True, return_iter=True, **kw):
-    #if not kw.get('is_prepared'):
-        #txt = _prepare_text(txt)
-        
+    # if not kw.get('is_prepared'):
+    # txt = _prepare_text(txt)
+
     if not return_iter and not filter_end:
-        return re.findall(PATTERN,txt)
-    
-    _iter = re.finditer(PATTERN,txt)
+        return re.findall(PATTERN, txt)
+
+    _iter = re.finditer(PATTERN, txt)
     matches = []
 
     for x in _iter:
         lnk = x.group()
         index = x.span()[0]
         end = x.span()[1]
-        
+
         if filter_end:
             lnk = lnk.strip(PROBABLY_INVALID_END)
             end = index + len(lnk)
 
-        matches.append(match_t(index,end,str))
+        matches.append(match_t(index, end, str))
 
-  
     if not return_iter:
         return [x.str for x in matches]
-    
+
     return matches
-    
 
-#---------------------------------------
+
+# ---------------------------------------
 
 
 def main():
     from urllib.request import urlopen
-    txt = 'http://google.com, go to that site.https://www.goodshopping.info/buy?socks=2. '+\
-          'Finallywww.bookreader.es/new/fiction?author=rowling+publisher=Frameworks~link_end,more_text'+\
-          'http://bookreader.es/new/fiction?author=rowling+publisher=Frameworks~link_end,'+\
-          'https://yahoo.com.https://www.yahoo.com/. And then we wen to.http://yahoo.comhttp://www.yahoo.comwww.yahoo.com'
+
+    txt = (
+        "http://google.com, go to that site.https://www.goodshopping.info/buy?socks=2. "
+        + "Finallywww.bookreader.es/new/fiction?author=rowling+publisher=Frameworks~link_end,more_text"
+        + "http://bookreader.es/new/fiction?author=rowling+publisher=Frameworks~link_end,"
+        + "https://yahoo.com.https://www.yahoo.com/. And then we wen to.http://yahoo.comhttp://www.yahoo.comwww.yahoo.com"
+    )
 
     """urls = find_links(txt,filter_end=False,return_iter=False)
     urls2 = find_links(txt,filter_end=True,return_iter=False)
     urls2b = [u.strip(strip_urlend) for u in urls]"""
 
     urls = find_urls(txt)
     urls_replaced = filter_urls(txt)
-    
-    print(urls,"\n")
-    #print(urls2,"\n")
-    #print(urls2b,"\n")
+
+    print(urls, "\n")
+    # print(urls2,"\n")
+    # print(urls2b,"\n")
 
     print(urls_replaced)
 
     """def decode_urls(urls):
         for u in urls:
             try:
                 print(urlopen(u).geturl())
             except Exception as e:
                 print(e.args[0], u)"""
 
-    #decode_urls(urls2)
-    #decode_urls(urls)
-    
-    
-            
-    
-    
+    # decode_urls(urls2)
+    # decode_urls(urls)
+
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
-
```

### Comparing `fons-0.3.1/fons/os.py` & `fons-0.4.0/fons/os.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,280 +1,287 @@
-import os
-import re
-import tempfile
-import zipfile
-import platform
-
-import fons.log as _log
-
-_PLATFORM = platform.system()
-
-logger,logger2,tlogger,tloggers,tlogger0 = _log.get_standard_5(__name__)
-
-
-def _is_relative(path):
-    return ':' not in path
-
-
-def _resolve(pth, envdir):
-    pth = os.path.normpath(pth)
-    
-    if _is_relative(pth):
-        pth = os.path.join(envdir, pth)
-        
-    pth = os.path.realpath(pth)
-    
-    return pth
-
-
-def search_in_file(path, str, encoding='utf-8'):
-    with open(path, encoding=encoding) as f:
-        txt = f.read()
-        
-    if str in txt:
-        return True
-    
-    return False
-
-
-def search(root, str, filenames=True, contents=True):
-    found = []
-
-    def _search(x,y): return y in x
-
-    if os.path.isfile(root):
-        walkthrough = [(os.path.dirname(root),('',),(os.path.basename(root),))]
-        filenames = False
-    elif os.path.isdir(root):
-        walkthrough = os.walk(root)
-    else:
-        raise FileNotFoundError('Root \'{}\' doesn\'t exist'.format(root))
-        
-    for _root,dirs,files in walkthrough:
-        for fn in files:
-            pth = os.path.join(_root,fn)
-            
-            if filenames and _search(fn,str):
-                found.append(pth)
-            elif contents:
-                try: assert search_in_file(pth,str)
-                except Exception: pass
-                else: found.append(pth)
-
-        if filenames:
-            found += [os.path.join(root,x) for x in dirs if str in x]
-
-    return found
-
-
-def replace(root, str, replace_with):
-
-    def _overwrite(path, new_contents):
-        fd, temp_path = tempfile.mkstemp()
-        bytes = new_contents.encode('utf-8')
-        try:
-            with os.fdopen(fd, 'wb') as tmp:
-                tmp.write(bytes)
-            os.remove(path)
-            os.rename(temp_path, path)
-        finally:
-            if os.path.exists(temp_path):
-                os.remove(temp_path)
-                
-    
-    def _replace(path):
-        with open(path, encoding='utf-8') as f:
-            contents = f.read()
-            
-        if str not in contents:
-            return ''
-        
-        new_contents = re.sub(str, replace_with, contents)
-        _overwrite(path, new_contents)
-        
-        return path
-        
-        
-    if os.path.isfile(root):
-        walkthrough = [(os.path.dirname(root),('',),(os.path.basename(root),))]
-    elif os.path.isdir(root):
-        walkthrough = os.walk(root)
-    else:
-        raise FileNotFoundError('Root \'{}\' doesn\'t exist'.format(root))
-    
-    replaced = []
-    failed = []
-        
-    for _root,dirs,files in walkthrough:
-        for fn in files:
-            pth = os.path.join(_root,fn)
-            try:
-                if _replace(pth):
-                    replaced.append(pth)
-            except Exception:
-                failed.append(pth)
-
-    return replaced, failed
-
-
-def delete_empty_dirs(root, recycler=None):
-    ow = os.walk(root,topdown=False)
-    
-    for root,dirs,files in ow:
-        
-        for _dir in dirs:
-            _dirpth = os.path.join(root,_dir)
-            
-            try: 
-                if len(os.listdir(_dirpth)):
-                    continue
-            except FileNotFoundError:
-                continue
-            
-            if recycler is not None:
-                recycler(_dirpth)
-                continue
-            
-            logger.debug('_dirpth_ removing: {}'.format(_dirpth))
-            
-            try: os.rmdir(_dirpth)
-            except FileNotFoundError: pass
-            except Exception as e:
-                logger.exception(e)
-
-
-def make_dirpath(*args):
-    path = ''
-    for a in args:
-        path = os.path.join(path,a)
-        if not os.path.isdir(path):
-            os.mkdir(path)
-    return path
-
-
-def get_appdata_dir(appname, windows_select='Local', make=False):
-    """https://stackoverflow.com/a/1088459/10492167"""
-    if windows_select not in ['Local','LocalLow','Roaming']:
-        raise ValueError(windows_select)
-    
-    if _PLATFORM == 'Darwin':
-        app_support = os.path.expanduser('~/Library/Application Support')
-        appdata = os.path.join(app_support, appname)
-    elif _PLATFORM == 'Windows':
-        local = os.path.normpath(os.environ['APPDATA']+'/../{}'.format(windows_select))
-        appdata = os.path.join(local, appname)
-    else:
-        appdata = os.path.expanduser(os.path.join("~", "." + appname))
-    
-    if make:
-        make_dirpath(appdata)
-        
-    return appdata
-
-
-def zip_contents(path, destination=None,
-                 compression='ZIP_DEFLATED',
-                 include_pycache=False,
-                 exists='error'):
-    
-    """
-    :param path: path or list of paths.
-                 If a path is directory, all its contents will be zipped under
-                 the name of the directory. Relative paths are assumed to be relative
-                 to the parent directory of the first path in the list, and the first path
-                 to the current working directory.
-                 In case an outermost directory/file already exists in the in-the-making
-                 zip file, the directory/file is renamed to "{original_base}({n}){original_suffix}"
-                 (the suffix is for files only).
-    
-    :param exists: "error" or "rename"
-                The action applies to `destination`.
-    """
-    
-    if isinstance(compression,str):
-        compression = getattr(zipfile, compression)
-        
-    if exists not in (None,'error','rename'):
-        raise ValueError("`exists` must be either 'error' or 'rename'; got: {}".format(exists))
-    
-    paths = [path] if isinstance(path, str) else path
-    paths[0] = main_path = os.path.realpath(paths[0])
-    main_envdir = os.path.dirname(main_path)
-    
-    paths = [paths[0]] + [_resolve(pth, main_envdir) for pth in paths[1:]]
-    
-    if destination is None:
-        destination = os.path.join(main_envdir, os.path.basename(main_path)+'.zip')
-    
-    destination = _resolve(destination, main_envdir)
-
-    if exists in (None,'error') and os.path.exists(exists):
-        raise OSError('Destination {} already exists'.format(destination))    
-
-    i = 0
-    has_zipend = destination.endswith('.zip')
-    body = destination[:-4] if has_zipend else destination
-    
-    while os.path.exists(destination):
-        destination = '{}({}){}'.format(body, i+2, '.zip' if has_zipend else '')
-        i+=1
-        
-    cache = ('__pycache__', '.cache', '.pytest_cache')
-    _contains_cache_dir = lambda tail: any(c in tail for c in cache)
-    
-    ignore = 'geckodriver.log'
-    _filter = lambda files: [f for f in files if f not in ignore]
-    
-    zf = zipfile.ZipFile(destination, 'w', compression)
-    
-    
-    def _rename(pth, is_file=False, zf_outermost_dirs=set(), zf_outermost_files=set()):
-        name = os.path.basename(pth)
-        
-        if is_file and '.' in name:
-            dot_loc = name.rfind('.')
-            body, suffix = name[:dot_loc], name[dot_loc:]
-        else:
-            body, suffix = name, ''
-        
-        reg = zf_outermost_dirs if not is_file else zf_outermost_files  
-        i = 0
-        
-        while name in reg:
-            name = '{}({}){}'.format(body, i+2, suffix)
-            i +=1
-            
-        reg.add(name)
-        
-        return os.path.join(os.path.dirname(pth), name)
-    
-    
-    def _zip_directory(pth):
-        len_pth = len(pth)
-        len_split = len(os.sep)
-                
-        pth2 = _rename(pth)
-        basedir = os.path.basename(pth2)
-        
-        for root, dirs, files in os.walk(pth):
-            tail = root.split(os.sep)[len_split:]
-            if include_pycache: pass
-            elif _contains_cache_dir(tail): continue
-            else: files = _filter(files)
-            
-            rel_path = os.path.join(basedir, root[len_pth+1:])
-                
-            for f in files:
-                zf.write(os.path.join(root,f), os.path.join(rel_path, f))
-    
-    
-    for pth in paths:
-        if os.path.isdir(pth):
-            _zip_directory(pth)
-        else:
-            pth2 = _rename(pth, is_file=True)
-            zf.write(pth, os.path.basename(pth2))
- 
-    zf.close()
-
-
-    return destination
+import os
+import re
+import tempfile
+import zipfile
+import platform
+
+import fons.log as _log
+
+_PLATFORM = platform.system()
+
+logger, logger2, tlogger, tloggers, tlogger0 = _log.get_standard_5(__name__)
+
+
+def _is_relative(path):
+    return ":" not in path
+
+
+def _resolve(pth, envdir):
+    pth = os.path.normpath(pth)
+
+    if _is_relative(pth):
+        pth = os.path.join(envdir, pth)
+
+    pth = os.path.realpath(pth)
+
+    return pth
+
+
+def search_in_file(path, str, encoding="utf-8"):
+    with open(path, encoding=encoding) as f:
+        txt = f.read()
+
+    if str in txt:
+        return True
+
+    return False
+
+
+def search(root, str, filenames=True, contents=True):
+    found = []
+
+    def _search(x, y):
+        return y in x
+
+    if os.path.isfile(root):
+        walkthrough = [(os.path.dirname(root), ("",), (os.path.basename(root),))]
+        filenames = False
+    elif os.path.isdir(root):
+        walkthrough = os.walk(root)
+    else:
+        raise FileNotFoundError("Root '{}' doesn't exist".format(root))
+
+    for _root, dirs, files in walkthrough:
+        for fn in files:
+            pth = os.path.join(_root, fn)
+
+            if filenames and _search(fn, str):
+                found.append(pth)
+            elif contents:
+                try:
+                    assert search_in_file(pth, str)
+                except Exception:
+                    pass
+                else:
+                    found.append(pth)
+
+        if filenames:
+            found += [os.path.join(root, x) for x in dirs if str in x]
+
+    return found
+
+
+def replace(root, str, replace_with):
+    def _overwrite(path, new_contents):
+        fd, temp_path = tempfile.mkstemp()
+        bytes = new_contents.encode("utf-8")
+        try:
+            with os.fdopen(fd, "wb") as tmp:
+                tmp.write(bytes)
+            os.remove(path)
+            os.rename(temp_path, path)
+        finally:
+            if os.path.exists(temp_path):
+                os.remove(temp_path)
+
+    def _replace(path):
+        with open(path, encoding="utf-8") as f:
+            contents = f.read()
+
+        if str not in contents:
+            return ""
+
+        new_contents = re.sub(str, replace_with, contents)
+        _overwrite(path, new_contents)
+
+        return path
+
+    if os.path.isfile(root):
+        walkthrough = [(os.path.dirname(root), ("",), (os.path.basename(root),))]
+    elif os.path.isdir(root):
+        walkthrough = os.walk(root)
+    else:
+        raise FileNotFoundError("Root '{}' doesn't exist".format(root))
+
+    replaced = []
+    failed = []
+
+    for _root, dirs, files in walkthrough:
+        for fn in files:
+            pth = os.path.join(_root, fn)
+            try:
+                if _replace(pth):
+                    replaced.append(pth)
+            except Exception:
+                failed.append(pth)
+
+    return replaced, failed
+
+
+def delete_empty_dirs(root, recycler=None):
+    ow = os.walk(root, topdown=False)
+
+    for root, dirs, files in ow:
+        for _dir in dirs:
+            _dirpth = os.path.join(root, _dir)
+
+            try:
+                if len(os.listdir(_dirpth)):
+                    continue
+            except FileNotFoundError:
+                continue
+
+            if recycler is not None:
+                recycler(_dirpth)
+                continue
+
+            logger.debug("_dirpth_ removing: {}".format(_dirpth))
+
+            try:
+                os.rmdir(_dirpth)
+            except FileNotFoundError:
+                pass
+            except Exception as e:
+                logger.exception(e)
+
+
+def make_dirpath(*args):
+    path = ""
+    for a in args:
+        path = os.path.join(path, a)
+        if not os.path.isdir(path):
+            os.mkdir(path)
+    return path
+
+
+def get_appdata_dir(appname, windows_select="Local", make=False):
+    """https://stackoverflow.com/a/1088459/10492167"""
+    if windows_select not in ["Local", "LocalLow", "Roaming"]:
+        raise ValueError(windows_select)
+
+    if _PLATFORM == "Darwin":
+        app_support = os.path.expanduser("~/Library/Application Support")
+        appdata = os.path.join(app_support, appname)
+    elif _PLATFORM == "Windows":
+        local = os.path.normpath(
+            os.environ["APPDATA"] + "/../{}".format(windows_select)
+        )
+        appdata = os.path.join(local, appname)
+    else:
+        appdata = os.path.expanduser(os.path.join("~", "." + appname))
+
+    if make:
+        make_dirpath(appdata)
+
+    return appdata
+
+
+def zip_contents(
+    path,
+    destination=None,
+    compression="ZIP_DEFLATED",
+    include_pycache=False,
+    exists="error",
+):
+    """
+    :param path: path or list of paths.
+                 If a path is directory, all its contents will be zipped under
+                 the name of the directory. Relative paths are assumed to be relative
+                 to the parent directory of the first path in the list, and the first path
+                 to the current working directory.
+                 In case an outermost directory/file already exists in the in-the-making
+                 zip file, the directory/file is renamed to "{original_base}({n}){original_suffix}"
+                 (the suffix is for files only).
+
+    :param exists: "error" or "rename"
+                The action applies to `destination`.
+    """
+
+    if isinstance(compression, str):
+        compression = getattr(zipfile, compression)
+
+    if exists not in (None, "error", "rename"):
+        raise ValueError(
+            "`exists` must be either 'error' or 'rename'; got: {}".format(exists)
+        )
+
+    paths = [path] if isinstance(path, str) else path
+    paths[0] = main_path = os.path.realpath(paths[0])
+    main_envdir = os.path.dirname(main_path)
+
+    paths = [paths[0]] + [_resolve(pth, main_envdir) for pth in paths[1:]]
+
+    if destination is None:
+        destination = os.path.join(main_envdir, os.path.basename(main_path) + ".zip")
+
+    destination = _resolve(destination, main_envdir)
+
+    if exists in (None, "error") and os.path.exists(exists):
+        raise OSError("Destination {} already exists".format(destination))
+
+    i = 0
+    has_zipend = destination.endswith(".zip")
+    body = destination[:-4] if has_zipend else destination
+
+    while os.path.exists(destination):
+        destination = "{}({}){}".format(body, i + 2, ".zip" if has_zipend else "")
+        i += 1
+
+    cache = ("__pycache__", ".cache", ".pytest_cache")
+    _contains_cache_dir = lambda tail: any(c in tail for c in cache)
+
+    ignore = "geckodriver.log"
+    _filter = lambda files: [f for f in files if f not in ignore]
+
+    zf = zipfile.ZipFile(destination, "w", compression)
+
+    def _rename(pth, is_file=False, zf_outermost_dirs=set(), zf_outermost_files=set()):
+        name = os.path.basename(pth)
+
+        if is_file and "." in name:
+            dot_loc = name.rfind(".")
+            body, suffix = name[:dot_loc], name[dot_loc:]
+        else:
+            body, suffix = name, ""
+
+        reg = zf_outermost_dirs if not is_file else zf_outermost_files
+        i = 0
+
+        while name in reg:
+            name = "{}({}){}".format(body, i + 2, suffix)
+            i += 1
+
+        reg.add(name)
+
+        return os.path.join(os.path.dirname(pth), name)
+
+    def _zip_directory(pth):
+        len_pth = len(pth)
+        len_split = len(os.sep)
+
+        pth2 = _rename(pth)
+        basedir = os.path.basename(pth2)
+
+        for root, dirs, files in os.walk(pth):
+            tail = root.split(os.sep)[len_split:]
+            if include_pycache:
+                pass
+            elif _contains_cache_dir(tail):
+                continue
+            else:
+                files = _filter(files)
+
+            rel_path = os.path.join(basedir, root[len_pth + 1 :])
+
+            for f in files:
+                zf.write(os.path.join(root, f), os.path.join(rel_path, f))
+
+    for pth in paths:
+        if os.path.isdir(pth):
+            _zip_directory(pth)
+        else:
+            pth2 = _rename(pth, is_file=True)
+            zf.write(pth, os.path.basename(pth2))
+
+    zf.close()
+
+    return destination
```

### Comparing `fons-0.3.1/fons/processes.py` & `fons-0.4.0/fons/processes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,94 +1,116 @@
-import time
-import multiprocessing
-from multiprocessing import Process as _Process
-
-import fons.log as _log
-
-logger,logger2,tlogger,tloggers,tlogger0 = _log.get_standard_5(__name__)
-
-
-class Logi(type):
-    def __new__(cls, name, bases, attrs):        
-        def wrap_run(f):
-            def init_logging(self):
-                _log.standard_mp_logging(**self._log_params)
-                return f(self)
-            return init_logging
-        
-        def wrap_start(f):
-            def start_loglisten(self):
-                lp = getattr(self,'_log_params',None)
-                if lp is None: self._log_params = lp = _log._globals.copy()
-                #(if has already been started then ignores)
-                _log.start_listener()
-                return f(self)
-            return start_loglisten
-        
-        if not any(issubclass(x,_Process) for x in bases):
-            raise TypeError("class '{}' must be a subclass of 'multiprocessing.Process'".format(name))
-        
-        if 'run' in attrs:
-            attrs['run'] = wrap_run(attrs['run'])
-        elif not any(issubclass(type(x),Logi) for x in bases):
-            attrs['run'] = wrap_run(_Process.run)
-            
-        if 'start' in attrs:
-            attrs['start'] = wrap_start(attrs['start'])
-        elif not any(issubclass(type(x),Logi) for x in bases):
-            attrs['start'] = wrap_start(_Process.start)
-        
-            
-        return super(Logi, cls).__new__(cls, name, bases, attrs)
-    
-    
-class LogiProcess(_Process, metaclass=Logi):
-    """Starts LogListener in child process with the QueueHandler from parent process"""
-    def __init__(self, *args, log_params=None, **kw):
-        super().__init__(*args,**kw)
-        self._log_params = log_params.copy() if log_params is not None else _log._globals.copy()
-        
-        
-class TkLogiProcess(_Process, metaclass=Logi):
-    def __init__(self, nb, *args, log_params=None, **kw):
-        """nb - tkinter.ttk.NoteBook object"""
-        super().__init__(*args,**kw)
-        self._log_params = log_params.copy() if log_params is not None else _log._globals.copy()
-        
-        if self.name not in _log._tklogiprocesses:
-            _log.init_tab(nb,self.name)
-
-
-    """def __del__(self):
-        try: u_log._tklogiprocesses.remove(self.name)
-        except KeyError: pass
-        super().__del__()"""
-        
-
-def pool_processes(processes, max_concurrent=None, timeout=None, interval=0.05):
-    if max_concurrent is None:
-        max_concurrent = max(1, multiprocessing.cpu_count()-1)
-    p_iter = iter(processes)
-    running = []
-    started = {}
-    #print('max_concurrent: {}'.format(max_concurrent))
-    while True:
-        for p in running:
-            if not p.is_alive(): pass
-            elif timeout is not None and time.time()-started[p] > timeout:
-                logger.debug('Process "{}" (pid: {}) has exceeded its timeout. Terminating.'.format(p.name,p.pid))
-                try: p.terminate()
-                except Exception as e:
-                    logger2.error('Could not terminate process: {} (pid: {})'.format(p.name,p.pid))
-                    logger.exception(e)
-        running = [p for p in running if p.is_alive()]
-        if len(running) >= max_concurrent:
-            time.sleep(interval)
-            continue
-        try: p = next(p_iter)
-        except StopIteration: break
-        #print('p: {}'.format(p))
-        started[p] = time.time()
-        p.start()
-        running.append(p)
-    #print('running: {}'.format(running))
-    [p.join() for p in running]
+import time
+import multiprocessing
+from multiprocessing import Process as _Process
+
+import fons.log as _log
+
+logger, logger2, tlogger, tloggers, tlogger0 = _log.get_standard_5(__name__)
+
+
+class Logi(type):
+    def __new__(cls, name, bases, attrs):
+        def wrap_run(f):
+            def init_logging(self):
+                _log.standard_mp_logging(**self._log_params)
+                return f(self)
+
+            return init_logging
+
+        def wrap_start(f):
+            def start_loglisten(self):
+                lp = getattr(self, "_log_params", None)
+                if lp is None:
+                    self._log_params = lp = _log._globals.copy()
+                # (if has already been started then ignores)
+                _log.start_listener()
+                return f(self)
+
+            return start_loglisten
+
+        if not any(issubclass(x, _Process) for x in bases):
+            raise TypeError(
+                "class '{}' must be a subclass of 'multiprocessing.Process'".format(
+                    name
+                )
+            )
+
+        if "run" in attrs:
+            attrs["run"] = wrap_run(attrs["run"])
+        elif not any(issubclass(type(x), Logi) for x in bases):
+            attrs["run"] = wrap_run(_Process.run)
+
+        if "start" in attrs:
+            attrs["start"] = wrap_start(attrs["start"])
+        elif not any(issubclass(type(x), Logi) for x in bases):
+            attrs["start"] = wrap_start(_Process.start)
+
+        return super(Logi, cls).__new__(cls, name, bases, attrs)
+
+
+class LogiProcess(_Process, metaclass=Logi):
+    """Starts LogListener in child process with the QueueHandler from parent process"""
+
+    def __init__(self, *args, log_params=None, **kw):
+        super().__init__(*args, **kw)
+        self._log_params = (
+            log_params.copy() if log_params is not None else _log._globals.copy()
+        )
+
+
+class TkLogiProcess(_Process, metaclass=Logi):
+    def __init__(self, nb, *args, log_params=None, **kw):
+        """nb - tkinter.ttk.NoteBook object"""
+        super().__init__(*args, **kw)
+        self._log_params = (
+            log_params.copy() if log_params is not None else _log._globals.copy()
+        )
+
+        if self.name not in _log._tklogiprocesses:
+            _log.init_tab(nb, self.name)
+
+    """def __del__(self):
+        try: u_log._tklogiprocesses.remove(self.name)
+        except KeyError: pass
+        super().__del__()"""
+
+
+def pool_processes(processes, max_concurrent=None, timeout=None, interval=0.05):
+    if max_concurrent is None:
+        max_concurrent = max(1, multiprocessing.cpu_count() - 1)
+    p_iter = iter(processes)
+    running = []
+    started = {}
+    # print('max_concurrent: {}'.format(max_concurrent))
+    while True:
+        for p in running:
+            if not p.is_alive():
+                pass
+            elif timeout is not None and time.time() - started[p] > timeout:
+                logger.debug(
+                    'Process "{}" (pid: {}) has exceeded its timeout. Terminating.'.format(
+                        p.name, p.pid
+                    )
+                )
+                try:
+                    p.terminate()
+                except Exception as e:
+                    logger2.error(
+                        "Could not terminate process: {} (pid: {})".format(
+                            p.name, p.pid
+                        )
+                    )
+                    logger.exception(e)
+        running = [p for p in running if p.is_alive()]
+        if len(running) >= max_concurrent:
+            time.sleep(interval)
+            continue
+        try:
+            p = next(p_iter)
+        except StopIteration:
+            break
+        # print('p: {}'.format(p))
+        started[p] = time.time()
+        p.start()
+        running.append(p)
+    # print('running: {}'.format(running))
+    [p.join() for p in running]
```

### Comparing `fons-0.3.1/fons/py.py` & `fons-0.4.0/fons/py.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,89 +1,99 @@
-from types import ModuleType
-from importlib import reload
-import os, sys
-
-
-def mro(*bases):
-    """Calculate the Method Resolution Order of bases using the C3 algorithm.
-
-    Suppose you intended creating a class K with the given base classes. This
-    function returns the MRO which K would have, *excluding* K itself (since
-    it doesn't yet exist), as if you had actually created the class.
-
-    Another way of looking at this, if you pass a single class K, this will
-    return the linearization of K (the MRO of K, *including* itself).
-    """
-    seqs = [list(C.__mro__) for C in bases] + [list(bases)]
-    res = []
-    while True:
-        non_empty = list(filter(None, seqs))
-        if not non_empty:
-            # Nothing left to process, we're done.
-            return tuple(res)
-        for seq in non_empty:  # Find merge candidates among seq heads.
-            candidate = seq[0]
-            not_head = [s for s in non_empty if candidate in s[1:]]
-            if not_head:
-                # Reject the candidate.
-                candidate = None
-            else:
-                break
-        if not candidate:
-            raise TypeError("inconsistent hierarchy, no C3 MRO is possible")
-        res.append(candidate)
-        for seq in non_empty:
-            # Remove candidate.
-            if seq[0] == candidate:
-                del seq[0]
-                
-    return res
-
-
-def rreload2(module, seen=None):
-    """Recursively reload modules."""
-    if seen is None: seen = []
-    if module in seen:
-        return
-    
-    reload(module)
-    seen.append(module)
-    
-    for attribute_name in dir(module):
-        attribute = getattr(module, attribute_name)
-        if type(attribute) is ModuleType:
-            rreload2(attribute,seen)
-            
-            
-def rreload(module, paths=None, mdict=None):
-    """Recursively reload modules."""
-    if paths is None:
-        paths = ['']
-    if mdict is None:
-        mdict = {}
-    if module not in mdict:
-        # modules reloaded from this module
-        mdict[module] = [] 
-    reload(module)
-    for attribute_name in dir(module):
-        attribute = getattr(module, attribute_name)
-        if type(attribute) is ModuleType:
-            if attribute not in mdict[module]:
-                if attribute.__name__ not in sys.builtin_module_names:
-                    if os.path.dirname(attribute.__file__) in paths:
-                        mdict[module].append(attribute)
-                        rreload(attribute, paths, mdict)
-    reload(module)
-    #return mdict
-    
-    
-if __name__ == '__main__':
-    class A: pass
-    class B(A): pass
-    class C(B): pass
-    class D(B): pass
-    class E(C,D): pass
-    print(mro(C,D))
-    print(E.__mro__[1:])
-    #print(object.__dict__)
-              
-    
+from types import ModuleType
+from importlib import reload
+import os, sys
+
+
+def mro(*bases):
+    """Calculate the Method Resolution Order of bases using the C3 algorithm.
+
+    Suppose you intended creating a class K with the given base classes. This
+    function returns the MRO which K would have, *excluding* K itself (since
+    it doesn't yet exist), as if you had actually created the class.
+
+    Another way of looking at this, if you pass a single class K, this will
+    return the linearization of K (the MRO of K, *including* itself).
+    """
+    seqs = [list(C.__mro__) for C in bases] + [list(bases)]
+    res = []
+    while True:
+        non_empty = list(filter(None, seqs))
+        if not non_empty:
+            # Nothing left to process, we're done.
+            return tuple(res)
+        for seq in non_empty:  # Find merge candidates among seq heads.
+            candidate = seq[0]
+            not_head = [s for s in non_empty if candidate in s[1:]]
+            if not_head:
+                # Reject the candidate.
+                candidate = None
+            else:
+                break
+        if not candidate:
+            raise TypeError("inconsistent hierarchy, no C3 MRO is possible")
+        res.append(candidate)
+        for seq in non_empty:
+            # Remove candidate.
+            if seq[0] == candidate:
+                del seq[0]
+
+    return res
+
+
+def rreload2(module, seen=None):
+    """Recursively reload modules."""
+    if seen is None:
+        seen = []
+    if module in seen:
+        return
+
+    reload(module)
+    seen.append(module)
+
+    for attribute_name in dir(module):
+        attribute = getattr(module, attribute_name)
+        if type(attribute) is ModuleType:
+            rreload2(attribute, seen)
+
+
+def rreload(module, paths=None, mdict=None):
+    """Recursively reload modules."""
+    if paths is None:
+        paths = [""]
+    if mdict is None:
+        mdict = {}
+    if module not in mdict:
+        # modules reloaded from this module
+        mdict[module] = []
+    reload(module)
+    for attribute_name in dir(module):
+        attribute = getattr(module, attribute_name)
+        if type(attribute) is ModuleType:
+            if attribute not in mdict[module]:
+                if attribute.__name__ not in sys.builtin_module_names:
+                    if os.path.dirname(attribute.__file__) in paths:
+                        mdict[module].append(attribute)
+                        rreload(attribute, paths, mdict)
+    reload(module)
+    # return mdict
+
+
+if __name__ == "__main__":
+
+    class A:
+        pass
+
+    class B(A):
+        pass
+
+    class C(B):
+        pass
+
+    class D(B):
+        pass
+
+    class E(C, D):
+        pass
+
+    print(mro(C, D))
+    print(E.__mro__[1:])
+    # print(object.__dict__)
```

### Comparing `fons-0.3.1/fons/pyops.py` & `fons-0.4.0/fons/pyops.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,197 +1,202 @@
-import pandas as pd
-import numpy as np
-import copy as _copy
-
-TYPES = ('type','function','module')
-_TYPES = tuple([cls for cls in object.__subclasses__() if cls.__name__ in TYPES])
-IMMUTABLES = (int, float, str, bool, tuple, type(None))
-COPY_METHOD = (pd.DataFrame, pd.Series, pd.DatetimeIndex, pd.Index, np.ndarray)
-
-OPS = {
-    '==': lambda x,y: x==y,
-    '!=': lambda x,y: x!=y,
-    '>': lambda x,y: x>y,
-    '>=': lambda x,y: x>=y,
-    '<=': lambda x,y: x<=y,
-    '<': lambda x,y: x<y,
-    'in': lambda x,y: x in y,
-    'not in': lambda x,y: x not in y,
-    'is': lambda x,y: x is y,
-    'is not': lambda x,y: x is not y,
-}
-
-
-def update_obj(obj, new):
-    istuple = isinstance(obj,tuple)
-    LT = (list,tuple)
-    tO,tN = type(obj),type(new)
-    
-    if isinstance(obj,LT) and isinstance(new,LT):
-        lnO,lnN = len(obj), len(new)
-        
-        #using < vN is '_keep_' > will sometimes evaluate False, specifically when '_keep_' originates from init_data('_keep_')
-        if istuple or tO is not tN:
-            return tN([obj[i] if compare(vN,'_keep_') else (vN if i >= lnO else update_obj(obj[i],vN)) for i,vN in enumerate(new)])
-        
-        if lnO < lnN: obj.extend(new[lnO:])
-        elif lnO > lnN: del obj[lnN:]
-        
-        for i,itm in enumerate(zip(obj,new)):
-            vO,vN = itm
-            if compare(vN,'_keep_'): continue
-            elif vO is vN: continue #compare(vO,vN): continue
-            else: obj[i] = update_obj(vO,vN)
-            
-        return obj
-            
-    
-    elif isinstance(obj,dict) and isinstance(new,dict):
-        for kN,vN in new.items():
-            obj[kN] = update_obj(obj.get(kN),vN)
-            
-        return obj
-        
-        
-    return new
-
-
-#---------------------------------------
-
-def exec_op(x, y, op="=="):
-    function = OPS.get(op)
-    
-    if function is None:
-        if not isinstance(op, str):
-            raise TypeError('Operation is of unknown type: {}'.format(type(op)))
-        else:
-            raise ValueError('Unknown operation: {}'.format(op))
-
-    return function(x, y)
-
-
-def compare(x, norm, type_op='isinstance'):
-    
-    if x is norm:
-        return True
-    
-    if type_op == 'isinstance' and not isinstance(x, type(norm)):
-        return False
-    
-    elif type_op == 'is' and type(x) is not type(norm):
-        return False
-    
-    elif hasattr(norm,'__name__'):
-        if not hasattr(norm,'__name__'):
-            return False
-        elif x.__name__ != norm.__name__:
-            return False
-    
-    
-    try: iter(x)
-    except TypeError: isiter = False
-    else: isiter = not isinstance(x,str)
-    
-    
-    if isinstance(x, (pd.DataFrame, pd.Series, pd.Index, np.ndarray)):
-        try:
-            answ = (x == norm)
-        except ValueError:
-            #different labels
-            return False
-        
-        while not isinstance(answ,np.bool_):
-            #must use np.bool_ (not bool, or np.bool)!
-            answ = answ.all()
-        
-        if not answ:
-            return False
-    
-    
-    elif isinstance(x, dict):
-        """try: _verify_keys(k.keys(),norm.keys())
-        except KeyError: return False"""
-        if x.keys() != norm.keys():
-            return False
-        
-        for k,v in x.items():
-            if not compare(v, norm[k], type_op=type_op):
-                return False
-          
-          
-    elif hasattr(norm,'__dict__'):
-        if not hasattr(x,'__dict__'):
-            return False
-        elif not compare(x.__dict__, norm.__dict__, type_op=type_op):
-            return False
-        
-    
-    elif isinstance(x, set):
-        if x != norm:
-            return False
-            
-            
-    elif isiter:
-        if hasattr(x,'__len__') and hasattr(norm, '__len__'):
-            if len(x) != len(norm):
-                return False
-            
-        it_x = iter(x)
-        it_norm = iter(norm)
-        
-        while True:
-            exhausted = 0
-            
-            try: ix = next(it_x)
-            except StopIteration:
-                exhausted += 1
-                
-            try: inorm = next(it_norm)
-            except StopIteration:
-                exhausted += 1
-
-            if exhausted == 1:
-                return False
-            elif exhausted == 2:
-                break
-            
-            if not compare(ix, inorm, type_op=type_op):
-                return False
-
-                
-    elif pd.isnull(norm):
-        if not(pd.isnull(x)):
-            return False
-    
-        
-    elif x != norm:
-        return False
-    
-    
-    return True
-
-
-#To avoid copy.deepcopy() if possible (faster)
-def copy(obj):
-    _type = type(obj)
-    _name = _type.__name__
-    
-    #copy.deepcopy:
-    # -doesn't work on modules
-    # -functions are not copied (id remains same)
-    # -classes are not copied
-    # -instance's metadata may be lost (e.g copy.deepcopy(df), also df.copy() )
-    # -built-in immutable instances seem to be not copied
-    
-    if _name in TYPES:
-        return obj
-    
-    #user may define '__hash__' = None, but object in fact IS mutable;
-    #therefore it is better to rely on known types to be immutable
-    elif any(issubclass(_type,im) for im in IMMUTABLES):
-        return obj
-        
-    elif any(issubclass(_type,cm) for cm in COPY_METHOD):
-        return obj.copy()
-    
-
-    return _copy.deepcopy(obj)
+import pandas as pd
+import numpy as np
+import copy as _copy
+
+TYPES = ("type", "function", "module")
+_TYPES = tuple([cls for cls in object.__subclasses__() if cls.__name__ in TYPES])
+IMMUTABLES = (int, float, str, bool, tuple, type(None))
+COPY_METHOD = (pd.DataFrame, pd.Series, pd.DatetimeIndex, pd.Index, np.ndarray)
+
+OPS = {
+    "==": lambda x, y: x == y,
+    "!=": lambda x, y: x != y,
+    ">": lambda x, y: x > y,
+    ">=": lambda x, y: x >= y,
+    "<=": lambda x, y: x <= y,
+    "<": lambda x, y: x < y,
+    "in": lambda x, y: x in y,
+    "not in": lambda x, y: x not in y,
+    "is": lambda x, y: x is y,
+    "is not": lambda x, y: x is not y,
+}
+
+
+def update_obj(obj, new):
+    istuple = isinstance(obj, tuple)
+    LT = (list, tuple)
+    tO, tN = type(obj), type(new)
+
+    if isinstance(obj, LT) and isinstance(new, LT):
+        lnO, lnN = len(obj), len(new)
+
+        # using < vN is '_keep_' > will sometimes evaluate False, specifically when '_keep_' originates from init_data('_keep_')
+        if istuple or tO is not tN:
+            return tN(
+                [
+                    obj[i]
+                    if compare(vN, "_keep_")
+                    else (vN if i >= lnO else update_obj(obj[i], vN))
+                    for i, vN in enumerate(new)
+                ]
+            )
+
+        if lnO < lnN:
+            obj.extend(new[lnO:])
+        elif lnO > lnN:
+            del obj[lnN:]
+
+        for i, itm in enumerate(zip(obj, new)):
+            vO, vN = itm
+            if compare(vN, "_keep_"):
+                continue
+            elif vO is vN:
+                continue  # compare(vO,vN): continue
+            else:
+                obj[i] = update_obj(vO, vN)
+
+        return obj
+
+    elif isinstance(obj, dict) and isinstance(new, dict):
+        for kN, vN in new.items():
+            obj[kN] = update_obj(obj.get(kN), vN)
+
+        return obj
+
+    return new
+
+
+# ---------------------------------------
+
+
+def exec_op(x, y, op="=="):
+    function = OPS.get(op)
+
+    if function is None:
+        if not isinstance(op, str):
+            raise TypeError("Operation is of unknown type: {}".format(type(op)))
+        else:
+            raise ValueError("Unknown operation: {}".format(op))
+
+    return function(x, y)
+
+
+def compare(x, norm, type_op="isinstance"):
+    if x is norm:
+        return True
+
+    if type_op == "isinstance" and not isinstance(x, type(norm)):
+        return False
+
+    elif type_op == "is" and type(x) is not type(norm):
+        return False
+
+    elif hasattr(norm, "__name__"):
+        if not hasattr(norm, "__name__"):
+            return False
+        elif x.__name__ != norm.__name__:
+            return False
+
+    try:
+        iter(x)
+    except TypeError:
+        isiter = False
+    else:
+        isiter = not isinstance(x, str)
+
+    if isinstance(x, (pd.DataFrame, pd.Series, pd.Index, np.ndarray)):
+        try:
+            answ = x == norm
+        except ValueError:
+            # different labels
+            return False
+
+        while not isinstance(answ, np.bool_):
+            # must use np.bool_ (not bool, or np.bool)!
+            answ = answ.all()
+
+        if not answ:
+            return False
+
+    elif isinstance(x, dict):
+        """try: _verify_keys(k.keys(),norm.keys())
+        except KeyError: return False"""
+        if x.keys() != norm.keys():
+            return False
+
+        for k, v in x.items():
+            if not compare(v, norm[k], type_op=type_op):
+                return False
+
+    elif hasattr(norm, "__dict__"):
+        if not hasattr(x, "__dict__"):
+            return False
+        elif not compare(x.__dict__, norm.__dict__, type_op=type_op):
+            return False
+
+    elif isinstance(x, set):
+        if x != norm:
+            return False
+
+    elif isiter:
+        if hasattr(x, "__len__") and hasattr(norm, "__len__"):
+            if len(x) != len(norm):
+                return False
+
+        it_x = iter(x)
+        it_norm = iter(norm)
+
+        while True:
+            exhausted = 0
+
+            try:
+                ix = next(it_x)
+            except StopIteration:
+                exhausted += 1
+
+            try:
+                inorm = next(it_norm)
+            except StopIteration:
+                exhausted += 1
+
+            if exhausted == 1:
+                return False
+            elif exhausted == 2:
+                break
+
+            if not compare(ix, inorm, type_op=type_op):
+                return False
+
+    elif pd.isnull(norm):
+        if not (pd.isnull(x)):
+            return False
+
+    elif x != norm:
+        return False
+
+    return True
+
+
+# To avoid copy.deepcopy() if possible (faster)
+def copy(obj):
+    _type = type(obj)
+    _name = _type.__name__
+
+    # copy.deepcopy:
+    # -doesn't work on modules
+    # -functions are not copied (id remains same)
+    # -classes are not copied
+    # -instance's metadata may be lost (e.g copy.deepcopy(df), also df.copy() )
+    # -built-in immutable instances seem to be not copied
+
+    if _name in TYPES:
+        return obj
+
+    # user may define '__hash__' = None, but object in fact IS mutable;
+    # therefore it is better to rely on known types to be immutable
+    elif any(issubclass(_type, im) for im in IMMUTABLES):
+        return obj
+
+    elif any(issubclass(_type, cm) for cm in COPY_METHOD):
+        return obj.copy()
+
+    return _copy.deepcopy(obj)
```

### Comparing `fons-0.3.1/fons/reg.py` & `fons-0.4.0/fons/reg.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,35 @@
-DEFAULT_REGISTRY = set()
-
-
-def create_name(name=None, default=None, registry=None, add_int='always'):
-    if registry is None:
-        registry = DEFAULT_REGISTRY
-    
-    if isinstance(name,str):
-        new_name =  name
-        
-    elif isinstance(name,int):
-        new_name = '{}-{}'.format(default, name) if default is not None else str(name)
-    
-    elif name is None and add_int == 'if_taken' and \
-            default is not None and default not in registry:
-        new_name = default
-        
-    elif name is None:
-        i = 1
-        while True:
-            new_name = '{}-{}'.format(default, i) if default is not None else str(i)
-            if new_name not in registry:
-                break
-            i+=1
-            
-    else: 
-        raise TypeError(type(name))
-    
-    
-    registry.add(new_name)
-    
-    return new_name
+DEFAULT_REGISTRY = set()
+
+
+def create_name(name=None, default=None, registry=None, add_int="always"):
+    if registry is None:
+        registry = DEFAULT_REGISTRY
+
+    if isinstance(name, str):
+        new_name = name
+
+    elif isinstance(name, int):
+        new_name = "{}-{}".format(default, name) if default is not None else str(name)
+
+    elif (
+        name is None
+        and add_int == "if_taken"
+        and default is not None
+        and default not in registry
+    ):
+        new_name = default
+
+    elif name is None:
+        i = 1
+        while True:
+            new_name = "{}-{}".format(default, i) if default is not None else str(i)
+            if new_name not in registry:
+                break
+            i += 1
+
+    else:
+        raise TypeError(type(name))
+
+    registry.add(new_name)
+
+    return new_name
```

### Comparing `fons-0.3.1/fons/sched.py` & `fons-0.4.0/fons/sched.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,1629 +1,1819 @@
-import abc
-import multiprocessing
-import asyncio
-import functools
-from functools import wraps
-import inspect
-
-from collections import deque
-import numpy as np
-import math
-import copy
-import platform
-import warnings
-import datetime
-dt = datetime.datetime
-td = datetime.timedelta
-
-from fons.debug import wrap_trylog
-import fons.log as _log
-from fons.processes import LogiProcess
-from fons.reg import create_name
-from fons.threads import EliThread
-import fons.time as fontime
-from fons.errors import (
-    QuitException, WaitException, TerminatedException,
-    TickerException, TickerAlreadyAdded, AllTerminated,
-    TickerQuitException, TickerWaitException, TickerTerminated
-)
-                    
-
-logger,logger2,tlogger,tloggers,tlogger0 = _log.get_standard_5(__name__)
-
-LOGGING_LEVEL = 10
-_PLATFORM = platform.system()
-_TICKER_NAMES = set()
-_ROUTINE_NAMES = set()
-
-
-#Automatically assigns class attribute " _name" (= the name of class)
-# if user has not specified the attribute itself
-class _AddName(type):
-    def __new__(cls, name, bases, attrs):
-        newattrs = {'_name': name}
-        newattrs.update(attrs)
-            
-        return super(_AddName, cls).__new__(cls, name, bases, newattrs)
-    
-    
-
-def _to_td(value):
-    if isinstance(value,td):
-        return value
-    elif isinstance(value,(int,float)):
-        return td(seconds=value)
-    else: raise TypeError(type(value))
-
-
-def _verify_target(values, add_to=None, target_null=False):
-    if add_to is None:
-        add_to = {}
-        
-    if not len(values):
-        raise ValueError('Target not given')
-    
-    target = values[0]
-    
-    if target_null and target is None: pass
-    elif not hasattr(target,'__call__'):
-        raise TypeError('Target is not callable: {}'.format(target))
-    
-    try: args = values[1]
-    except IndexError: args = None
-    
-    if args is None: args = tuple()
-    elif not hasattr(args,'__iter__'):
-        raise TypeError('Args is not iterable: {}'.format(args))
-    
-    try: kwargs = values[2]
-    except IndexError: kwargs = None
-    
-    if kwargs is None: kwargs = {}
-    elif not isinstance(kwargs,dict):
-        raise TypeError('Kwargs is not dict: {}'.format(kwargs))
-    
-    
-    add_to['target'] = target
-    add_to['args'] = args
-    add_to['kwargs'] = kwargs
-    
-    
-    return add_to
-
-
-def _accepts_args(f):
-    fas = inspect.getfullargspec(f)
-    c_args = fas.args
-    #inspect.ismethod is accurate whether or not "self" is first arg,
-    # or if it only has *args
-    if inspect.ismethod(f):
-        c_args = c_args[1:]
-    return len(c_args) > 0 or fas.varargs
-    
-
-def callback(f):
-    @wraps(f)
-    def wrapper(*args,**kw):
-        self = args[0]
-        callback = self._inf['callback']['target']
-        accepts_arg = self._inf['callback']['accepts_arg']
-        result = f(*args,**kw)
-        
-        if callback is not None:
-            if accepts_arg:
-                callback({'result': result, 'ticker': self, 'ts': dt.utcnow()})
-            else: callback()
-        
-        return result
-    
-    return wrapper
-    
-
-def async_callback(f):
-    @wraps(f)
-    async def wrapper(*args,**kw):
-        self = args[0]
-        callback = self._inf['callback']['target']
-        accepts_arg = self._inf['callback']['accepts_arg']
-        result = await f(*args,**kw)
-        
-        if callback is None: pass
-        elif self._inf['callback']['isCoro']:
-            if accepts_arg: await callback({'result': result, 'ticker': self, 'ts': dt.utcnow()})
-            else: await callback()
-        else: 
-            if accepts_arg: callback({'result': result, 'ticker': self, 'ts': dt.utcnow()})
-            else: callback()
-        
-        return result
-    
-    return wrapper
-
-
-
-
-#----------------------------------------------------------------------
-
-class BaseTicker(metaclass=abc.ABCMeta):
-    def __init__(self, *, callback=None, keepalive=None, name=None, logging_level=None):
-        self._inf = copy.deepcopy(self._inf)
-        self._ui = copy.deepcopy(self._ui)
-        self._hidden = copy.deepcopy(self._hidden)
-        
-        self._inf['callback']['target'] = callback
-        self._supers = set()
-        
-        if callback is not None:
-            self._inf['callback']['accepts_arg'] = _accepts_args(callback)
-            
-        self._inf['keepalive'] = bool(isinstance(keepalive,dict) or keepalive)
-        self._inf['keepalive_params'] = (dict({'attempts':True,'throw':TerminatedException},**keepalive) 
-                if isinstance(keepalive,dict) else {'attempts':True,'throw':TerminatedException})
-        if self._inf['keepalive']:
-            self.loop = wrap_trylog(self.loop,**self._inf['keepalive_params'])
-            
-        self._hidden['closed'] = multiprocessing.Event()
-        self._hidden['updated'] = multiprocessing.Event()
-        self._hidden['lock'] = multiprocessing.Lock()
-        
-        if name is None and hasattr(self.__class__,'_name'):
-            name = self.__class__._name
-        self._name = create_name(name, default=self.__class__.__name__, registry=_TICKER_NAMES)
-        
-        self.logging_level = logging_level if logging_level is not None else LOGGING_LEVEL
-
-    @abc.abstractmethod
-    def tick(self, errors='raise', update_supers=True):
-        pass
-    
-    @abc.abstractmethod
-    def get_time_remaining(self):
-        pass
-    
-    def __call__(self,*args,**kw):
-        return self.tick(*args,**kw)
-    
-    def loop(self, update_supers=True):
-        """Loops the tick method, with `errors` set to 'sleep'"""
-        self._verify_is_open()
-        tlogger.log(self.logging_level,'Starting ticker loop: {}'.format(self.name))
-        try: 
-            while True:
-                try:
-                    self.sleep()
-                    self.tick(errors='sleep', update_supers=update_supers)
-                except TerminatedException as e:
-                    if self._closed: break
-                    else: raise e
-        finally:
-            tlogger.log(self.logging_level,'Ticker loop ended: {}'.format(self.name))
-    
-    def _update_supers(self):
-        for s in self._supers:
-            s._update_timer(self,update_supers=True)
-            
-            
-    def sleep(self, time='remaining'):
-        t0 = time
-        if isinstance(time,dict):
-            t0,time = next(iter(time.items()))
-        
-        event = self._hidden['updated']
-        lock = self._hidden['lock']
-        tlogger0.log(self.logging_level,'Sleeping on ticker {} (time: {})'.format(self.name,time))
-        try:
-            while True:
-                with lock:
-                    self._verify_is_open()
-                    if time == 'updated': 
-                        time = None
-                    elif time == 'remaining':
-                        time = max(0, self.get_time_remaining())
-                        event.clear()
-                
-                if event.wait(time):
-                    event.clear()
-                    self._verify_is_open()
-                    time = t0
-                    if time == 'remaining':
-                        continue  
-                break
-        finally:
-            tlogger0.log(self.logging_level,'Sleep ended: {}'.format(self.name))
-       
-    def close(self):
-        tlogger.log(self.logging_level,'Closing ticker {}'.format(self.name))
-        with self._hidden['lock']:
-            if not self._closed:
-                self._ui['time_closed'] = dt.utcnow()
-                self._closed = True
-                
-            if not self._hidden['closed'].is_set():
-                self._hidden['closed'].set()
-            if not self._hidden['updated'].is_set():
-                self._hidden['updated'].set()
-            
-            
-    def _verify_is_open(self):
-        if self._closed:
-            raise TerminatedException('{} is closed'.format(self._name))
-        return True
-    
-    @property
-    def name(self):
-        return self._name
-    @name.setter
-    def name(self,value):
-        self._name = value
-    
-    _inf = {'callback':{'target':None,'accepts_arg':None},'keepalive':False,'keepalive_params':{}}
-    _ui = {'time_closed': None}
-    _hidden = {'closed':None, 'updated': None, 'lock': None}
-    _closed = False
-    
-
-class AsyncBaseTicker(BaseTicker):
-    def __init__(self, *args, loop=None, **kw):
-        super().__init__(*args,**kw)
-        if loop is None: loop = asyncio.get_event_loop()
-        self._inf['event_loop'] = loop
-        self._hidden['closed'] = asyncio.Event(loop=loop)
-        self._hidden['updated'] = asyncio.Event(loop=loop)
-        #self._hidden['lock'] = asyncio.Lock()
-        self._inf['callback']['isCoro'] = asyncio.iscoroutinefunction(self._inf['callback']['target'])
-        
-
-    async def __call__(self,*args,**kw):
-        return await self.tick(*args,**kw)
-        
-        
-    async def loop(self, update_supers=True):
-        """Loops the tick method, with `errors` set to 'sleep'"""
-        self._verify_is_open()
-        tlogger.log(self.logging_level,'Starting ticker loop: {}'.format(self.name))
-        try:
-            while True:
-                try: await self.tick(errors='sleep', update_supers=update_supers)
-                except TerminatedException as e:
-                    if self._closed: break
-                    raise e
-        finally:
-            tlogger.log(self.logging_level,'Ticker loop ended: {}'.format(self.name))
-    
-    
-    async def sleep(self, time='remaining'):
-        t0 = time
-        if isinstance(time,dict):
-            t0 = next(iter(time))
-            time = next(iter(time.values()))
-            
-        event = self._hidden['updated']
-        lock = self._hidden['lock']
-        loop = self._inf['event_loop']
-        is_windows = _PLATFORM == 'Windows'
-        tlogger0.log(self.logging_level,'Sleeping on ticker {} (time: {})'.format(self.name,time))
-        try:
-            while True:
-                with lock:
-                    self._verify_is_open()
-                    if time == 'updated': 
-                        time = None
-                    elif time == 'remaining':
-                        time = max(0, self.get_time_remaining())
-                        event.clear()
-                
-                if time is not None and time <= 0:
-                    break
-                
-                sleep_time = time
-                if time is not None:
-                    # Anything below 0.001 for non-windows and 0.016 for windows
-                    # may not be slept to the end.
-                    sleep_time = max(0.001, time)
-                    if is_windows:
-                        sleep_time = max(0.016, time)
-                
-                try:
-                    await asyncio.wait_for(event.wait(), sleep_time, loop=loop)
-                    event.clear()
-                    self._verify_is_open()
-                    # Event was set. Break out.
-                    if t0 != 'remaining':
-                        break
-                except asyncio.TimeoutError:
-                    # We can't break out of the loop yet, as asyncio.sleep isn't completely accurate
-                    pass
-                finally:
-                    time = t0
-        finally:
-            tlogger0.log(self.logging_level,'Sleep ended: {}'.format(self.name))
-
-    async def close(self):
-        super().close()
-        
-        
-#############################################################################
-
-class ScheduleTicker(BaseTicker):
-    """For calling targetfunc in time restricted manner,
-       .tick() or simply () attempts to call the target and return its output
-       .loop() cycles the target endlessly
-       .run() creates and runs a new thread with .loop as its target"""
-
-    def __init__(self,target=None, interval=None,
-                 sync=None, args=None, kwargs=None, *, 
-                 delay=None, lock=None, keep=5,
-                 errors='raise',return2=None, return2_call=False,
-                 callback=None, keepalive=None, name=None, **kw):
-
-        """
-        Args [Optional]:
-          target (func):
-            target func
-
-            
-          interval (int,float,timedelta,Ticker,callable,list/tuple):
-            tick interval
-            --<td,int,float,str,DateOffset> -> fontime.freq_to_offset(interval)
-            --<list/tuple> -> [callable, args, kw]
-            if Ticker, its tick() must return interval
-            if callable, must return interval
-            
-        
-          sync (datetime, timedelta,int,float, str: 'first','epoch','epoch-delay','random','interval' / offset-like, Offset)):
-            point in time which measures integer number of intervals passed;
-            ::default: None
-            --<timedelta,int,float,offset-like,DateOffset> -> <datetime || fontime.dt_round(dt.utcnow(), sync)>
-            --<str>: 'epoch'  [epoch is the moment of tick() being called for the 1st time] 
-                     'first'  [first = first_entry, guarantees t(2nd_tick()) - t(1st_tick()) = interval]
-                     'random' [random point of time in tp: (dt_round(dt.utcnow(),interval), interval)]
-                     'interval-<start>..<end>' [dt_round(dt.utcnow(), interval); [OPTIONAL] <start> / <end> floats in range(0,1)]
-                     
-                     
-            if None, each entry is counted from the *end* of the last tick
-             e.g if target takes unusually long, the interval will still be added on top of that
-             --delay must be None
-            otherwise each new entry is synced to the sync point
-              entry = sync + n*interval  || [n E int] || entry < dt.utcnow()
-            
-            ( tick can be called if dt.utcnow() > last_entry + interval + delay )
-                     
-          
-          args (listlike):
-            target func args
-          kwargs (dict):
-            target func kwargs
-                     
-          ---------------------------           
-          
-          delay(timedelta,int,float, str: offset-like, Offset):
-            if sync != None, this will be added to sync [next = last + interval + delay]
-            --<timedelta,int,float,str,DateOffset> -> fontime.freq_to_offset(delay)
-
-            
-
-          
-          lock (datetime, timedelta, float,int, str: 'next'/offset-like, Offset): 
-            forbids updating until the given moment in datetime
-            --<timedelta,int,float,offset-like,DateOffset> -> <datetime || dt.utcnow() + fontime.freq_to_offset(lock)>
-            --<str>
-              'next' - lock is synced to *next* tick() time from dt.utcnow()
-                        [but sync param itself must be None or value (cannot be str variable)]
-            ------------------------
-          errors (str):
-            'raise' - raise WaitError if tick is called prematurely
-            'warn' - warn, and return return2
-            'hide' - return return2
-          return2 (obj):
-            returned by tick() when errors == 'hide'/'warn'
-          return2_call (bool):
-            if True, then return2 is returned as return2()
-             in that case return2 can be passed as [target2,args2,kwargs2]
-          callback (function):
-             a single-argument function to be called after each tick;
-              argument to be passed: {"result": result, "ticker": ticker, "ts": timestamp}
-          name (str,int):
-            name of the Ticker instance, if int then added to the end of cls.__name__
-         
-        **kw
-          return2_copy (bool, func):
-            if True, the .return2() output will be deepcopied before returned
-            if function, this function will be used to copy .return2() before returned
-        """
-        super().__init__(callback=callback, keepalive=keepalive, name=name, logging_level=kw.get('logging_level'))        
-        
-        if interval is None: self.interval = self._interval
-        else: self.interval = interval
-        
-        interval = self._ui['interval']
-        
-        if sync is None: pass
-        elif isinstance(sync,str):
-            repl = sync.replace(' ','').lower()
-            if repl.startswith('random'):
-                range_part = repl[repl.find('-')+1:] if repl.find('-') != -1 else ''
-                ddloc = range_part.find('..')
-                to_float = lambda x,default: default if not len(x) else float(x)
-                try: fa,fb = (0,1) if ddloc==-1 else ( to_float(range_part[:ddloc],0),to_float(range_part[ddloc+2:],1) )
-                except Exception:
-                    raise ValueError('Could not understand `sync`: {}'.format(sync))
-                if fa < 0: raise ValueError('Sync `random` left endpoint must be >= 0; sync: {}'.format(sync))
-                elif fb > 1: raise ValueError('Sync `random` right endpoint must be <= 1; sync: {}'.format(sync))
-                elif fa > fb: raise ValueError('Sync `random` left endpoint must be <= right endpoint; sync: {}'.format(sync))
-                t00 = fontime.dt_round(dt.utcnow(),interval)
-                interval_td = (t00 + interval) - t00
-                t0 = t00 + fa*interval_td
-                t1 = t00 + fb*interval_td
-                rand_td = (t1 - t0) * np.random.random(1)[0]
-                self._ui['sync'] = t0 + rand_td
-            elif repl == 'interval':
-                self._ui['sync'] = fontime.dt_round(dt.utcnow(),interval)
-            elif repl not in ('first','epoch','epoch-delay'):
-                self._ui['sync'] = fontime.dt_round(dt.utcnow(),sync)#fontime.freq_to_td(sync, coerce=True)
-            else: self._ui['sync'] = repl
-        elif isinstance(sync, (td,float,int,fontime.offsets.DateOffset)) and not isinstance(sync,bool):
-            self._ui['sync'] = fontime.dt_round(dt.utcnow(),sync)
-        elif isinstance(sync, dt):
-            self._ui['sync'] = sync
-        else: raise TypeError(type(sync))
-
-        if delay is not None:
-            delay_ofs = fontime.freq_to_offset(delay)
-            if self._ui['sync'] is None and delay_ofs.n:
-                raise ValueError('sync must not be None if delay specified')
-            self._ui['delay'] = delay_ofs
-
-
-        d_target = self._inf['target']
-        _verify_target([target,args,kwargs],add_to=d_target, target_null=True)
-        
-
-        if errors is None: pass
-        elif not isinstance(errors,str):
-            raise TypeError(type(errors))
-        elif errors not in ('raise', 'warn', 'hide'):
-            raise ValueError(errors)
-        else: self._inf['errors'] = errors
-        
-        
-        r2 = self._inf['return2']
-        
-        if return2_call is True:
-            if isinstance(return2,(list,tuple)):
-                _verify_target(return2,add_to=r2)
-            else: _verify_target([return2],add_to=r2)            
-        
-        else: r2['value'] = return2
-        
-        r2_copy = kw.get('return2_copy')
-        if r2_copy is None: pass
-        elif isinstance(r2_copy,bool):
-            r2['copy'] = r2_copy
-        elif hasattr(copy,'__call__'):
-            r2['copy'] = True
-            r2['copyfunc'] = copy
-        else: raise TypeError(type(r2_copy))
-
-        
-        if lock is not None: 
-            self.lock = lock
- 
-        for k in ('entries','ticks','tick_ends','attempts'):
-            self._ui[k] = deque(self._ui[k], maxlen=keep)
-
-        
-        tlogger.log(self.logging_level,'{} interval: {}'.format(self._name, self._ui['_interval_str']))
-        
-        if (self._inf['target']['target'] is None and 
-            self.__class__.target is ScheduleTicker.target):
-            warnings.warn('Ticker\'s initiated target is None, nor has the target method been '
-                          'overriden, henceforth tick() will only return \'return2\'')
-
-
-
-    def _is_tick_time(self):
-        if self.get_time_remaining() > 0:
-            return False
-        return True
-
-
-    def get_time_remaining(self, as_float=True):
-        now = dt.utcnow()
-        _ui = self._ui
-        
-        remaining_lock = _ui['lock'] - now
-        try:
-            remaining = (_ui['entries'][0] + _ui['interval'] + _ui['delay']) - now
-        except IndexError:
-            remaining = td(0)
-        
-        if as_float:
-            remaining_lock = remaining_lock.total_seconds()
-            remaining = remaining.total_seconds()
-
-        return max(remaining_lock, remaining)
-    
-    
-    def _synced(self, stamps):
-        ui = self._ui
-        sync, interval, delay = ui['sync'], ui['interval'], ui['delay']
-        
-        single = not hasattr(stamps,'__iter__')
-        if single: stamps = [stamps]
-        
-        timestamps_synced = [
-            fontime.dt_synced(x-delay,interval,sync) for x in stamps]
-        
-
-        if single:
-            return timestamps_synced[0]
-        
-        return timestamps_synced
-        
-        
-    
-    def _ticktock_1st(self, now):
-        _ui = self._ui
-        _ui['epoch'] = now
-        
-        #later in _ticktock() will be assigned _ui['first'] =  _ui['entries'][0]
-        # because if `sync` was not bound to epoch, 
-        # the first = _ui['entries'][0] != now - _ui['delay'] due to sync difference
-
-        if _ui['sync'] == 'first':
-            _ui['sync'] = now - _ui['delay']
-            
-        elif _ui['sync'] == 'epoch':
-            _ui['sync'] = _ui['epoch']
-        
-        elif _ui['sync'] == 'epoch-delay':
-            _ui['sync'] = _ui['epoch'] - _ui['delay']
-        
-    
-    
-    def _ticktock(self):
-        """Updates `last` and `actual_last` in the beginning of every *valid* tick,
-           i.e only called after _is_tick_time() == True"""
-        
-        ui = self._ui
-        now = dt.utcnow() 
-        ui['ticks'].appendleft(now)
-        
-        if ui['sync'] is None:
-            return
-        
-        
-        counter = ui['counter']
-        if not counter:
-            self._ticktock_1st(now)
-        
-        
-        entry = self._synced(now)
-        ui['entries'].appendleft(entry)
-        
-        if not counter:
-            ui['first'] = entry
-
-
-
-
-    def _ticktock2(self):
-        """Updates `last` and `actual_last` in the *end* of every valid tick,
-           (i.e if _is_tick_time() == True and after target()/return2() completes),
-           ONLY IF sync = None"""
-        ui = self._ui
-        
-        now = dt.utcnow()
-        self._ui['tick_ends'].appendleft(now)
-        
-        counter = ui['counter']
-        ui['counter'] = counter +1
-        
-        if ui['sync'] is not None:
-            return
-        
-        
-        self._ui['entries'].appendleft(now)
-    
-        if not counter:
-            ui['epoch'] = now
-            ui['first'] = now
-            
-
-
-
-    def _interval_updating(self):
-        iu = self._inf['interval_updating']
-        if not iu['enabled']:
-            return
-        
-        try:
-            params = [iu['target'],iu['args'],iu['kwargs']]
-            i0 = self._interval
-            self.interval = params
-            if self._interval != i0:
-                logger.debug('{} new interval: {}'.format(self._name, self._ui['_interval_str']))
-        except (WaitException, TerminatedException):
-            return
-        
-
-    @callback
-    def tick(self, force=False, errors=None, update_supers=True):
-        """Does the "tick", i.e tries to call the target;
-           if Ticker is closed, raises TerminatedException;
-           elif force == True, target is called always;
-           else checks if the time has arrived;
-           
-           if time has not arrived, handles `errors`:
-             'error' - raises WaitException
-             'warn' - warns and returns return2()
-             'hide' - returns return2()
-             'sleep' - sleeps until time has arrived, returns target()
-             
-           else returns .target()
-           
-           
-           If .target() raises QuitException,
-             closes (it)self
-             returns QuitException.value if it has one,
-                     else .return2()
-             
-             
-           Note that QuitException raised from .return2 is not caught.
-           """
-        
-        self._ui['attempts'].appendleft(dt.utcnow())
-           
-        self._verify_is_open()
-
-
-        if errors is None:
-            errors = self._inf['errors']
-        
-        
-        if force is not True:
-            remaining = self.get_time_remaining()
-            
-            if remaining <= 0: pass
-            
-            elif errors == 'hide': 
-                return self.return2()
-            
-            elif errors == 'warn':
-                logger.debug('{} skipping tick() - wait of {} needed'.format(self._name,math.ceil(remaining)))
-                return self.return2()
-            
-            elif errors == 'sleep':
-                self.sleep({'remaining': remaining})
-
-            
-            else: raise WaitException(remaining)
-        
-
-        #update timestamps
-        self._ticktock()
-    
-    
-        try:
-            response = self.target()
-            self._interval_updating()
-        
-        except QuitException as e:
-            #if level > 0, then was raised by return2,
-            # which is not allowed
-            if e._level: raise e
-            elif len(e.args): 
-                response = e.args[0]
-            else: response = self.return2()
-            
-            self.close()
-            
-        except WaitException as e:
-            e._level += 1
-            raise e
-            
-        finally:
-            #update timestamps
-            self._ticktock2()
-            if update_supers:
-                self._update_supers()
-        
-        return response
-        
-        
-        
-
-        
-    def target(self):
-        """Calling the target function, returning its output.
-           This method may be overridden for custom use."""
-        d = self._inf['target']
-        target = d['target']
-        
-        if target is not None:
-            return target(*d['args'],**d['kwargs'])
-        
-        try: return self.return2()
-        except QuitException as e:
-            e._level += 1
-            raise e
-    
-    
-    def return2(self):
-        """Called from tick() if it determines _is_tick_time() == False, with `errors` 
-           set to 'warn' or 'hide'; or from target() if target has not been set.
-           This method may be overridden for custom use."""
-        r2 = self._inf['return2']
-        
-        if r2['target']:
-            value = r2['target'](*r2['args'],**r2['kwargs'])
-        else: value = r2['value']
-        
-        if r2['copy']:
-            #value = _copy(value)
-            value = r2['copyfunc'](value)
-
-        return value
-
-    
-    @property
-    def entries(self):
-        """tick_ends if sync = None, 
-           else ticks (starts) synced."""
-        return self._ui['entries']
-    
-    
-    @property
-    def records(self):
-        """Previous tick times recorded right before .target() started and at tick end."""
-        return list(zip(self._ui['ticks'], self._ui['tick_ends']))
-    
-            
-
-    @property
-    def interval(self):
-        return self._interval
-
-    @interval.setter
-    def interval(self, value):
-        _ui = self._ui
-        #if interval is Ticker, it must be tickeable at this moment
-        func = None
-        
-        if isinstance(value,(list,tuple)):
-            d = _verify_target(value)
-            value = d['target']
-        else: d = {'target':None, 'args': tuple(), 'kwargs': {}}
-        
-        
-        if hasattr(value, '__call__') and not isinstance(value,fontime.offsets.DateOffset):
-            func = value
-            
-            if isinstance(func,ScheduleTicker):
-                assert func._inf['errors'] == 'raise'
-                
-            value = func(*d['args'],**d['kwargs'])
-
-        
-        if value is None:
-            value = 0
-            
-        ofs = fontime.freq_to_offset(value)
-
-        if func is not None:
-            self._inf['interval_updating']['enabled'] = True
-        else: 
-            self._inf['interval_updating']['enabled'] = False
-            
-        d['target'] = func
-        self._inf['interval_updating'].update(d)
-        
-        
-        _ui['interval'] = ofs
-        try: _ui['_interval_str'] = ofs.freqstr
-        except AttributeError:
-            _ui['_interval_str'] = '?'
-        
-        self._interval = ofs
-        
-                
-        #updating sync
-        #(the first wait time will be == interval, but the next one'd be unknown, 
-        # due to entries[0] being synced to the old sync point)
-        if _ui['sync'] is not None and _ui['epoch'] is not None:
-            _ui['sync'] = self.entries[0]
-            
-        
-        self._update_supers()
-        with self._hidden['lock']:  
-            self._hidden['updated'].set()
-        
-        
-        
-    @property
-    def lock(self):
-        return self._ui['lock']
-    
-    @lock.setter
-    def lock(self, value):
-        _ui = self._ui
-        
-        if value is None:
-            value = dt.utcfromtimestamp(0)
-            
-        elif isinstance(value, (int, float, td, fontime.offsets.DateOffset)):
-            value = dt.utcnow() + fontime.freq_to_offset(value)
-            
-        elif isinstance(value,str):
-            if value.lower() not in ('next',):
-                value = dt.utcnow() + fontime.freq_to_offset(value)
-            
-            elif _ui['sync'] is None:
-                try: value = self.entries[0] + _ui['interval']
-                except IndexError: value = dt.utcnow() + _ui['interval']
-                #raise ValueError('For the lock to be synced the sync must not be None')
-            
-            elif not isinstance(_ui['sync'], dt):
-                raise ValueError('Sync is not initiated yet.')
-            
-            else:
-                nearest_synced = self._synced(dt.utcnow())
-                value = nearest_synced + _ui['interval'] + _ui['delay']
-                
-            
-        elif not isinstance(value,dt):
-            raise TypeError(type(value))
-        
-        _ui['lock'] = value
-        
-        self._update_supers()
-        with self._hidden['lock']:
-            self._hidden['updated'].set()
-        
-        
-    
-    def get_last(self,raw=False):
-        if raw: return self._ui['records'][0][1]
-        else: return self._ui['entries'][0]
-    
-    
-    def get_next(self,adjusted=True):
-        ui = self._ui
-        if ui['sync'] is None:
-            raise ValueError('Next cannot be estimated if sync = None')
-        
-        last = self.get_last()
-
-        nxt = last + ui['interval']
-        now = dt.utcnow()
-        
-        if adjusted:
-            nxt_synced = self._synced(now)
-            nxt = max(nxt_synced,nxt)
-        
-        return nxt
-        
-    
-    def get_sleep_time(self):
-        t = self.get_time_remaining(as_float=True)
-        return max(0.0, t)
-    
-    @property
-    def counter(self):
-        return self._ui['counter']
-    
-    @property
-    def args(self):
-        return self._inf['target']['args']
-    @args.setter
-    def args(self, value):
-        self._inf['target']['args'] = value
-        
-    @property
-    def kwargs(self):
-        return self._inf['target']['kwargs']
-    @kwargs.setter
-    def kwargs(self, value):
-        self._inf['target']['kwargs'] = value
-        
-
-    _interval = 0
-    
-    _ui = {'interval': td(0), 'sync':None, 'delay': td(0),
-           '_interval_str': '0S',
-           'lock': dt.utcfromtimestamp(0),
-           
-           'attempts': deque(maxlen=5),
-           'ticks': deque(maxlen=5),
-           'tick_ends': deque(maxlen=5),
-           'entries': deque(maxlen=5),
-           
-           'first': None, 'epoch': None, 'counter': 0, 
-           'time_closed': None, }
-    
-    _inf = {'target': {'target': None, 'args': tuple(), 'kwargs': {}},
-            'errors': 'raise',
-            'return2': {'value': None, 'copy': False, 'copyfunc': copy.deepcopy,
-                        'target':None, 'args':tuple(), 'kwargs':{}},
-            'callback': {'target': None, 'accepts_arg':None},
-            'keepalive': False, 'keepalive_params': {},
-            'interval_updating': {'enabled': False, 'target': None, 'args': tuple(), 'kwargs': {}},}
-
-
-
-class TPMethods:
-    def start_thread(self, join=False, add_to=None, *, trylog=True, keepalive=False, loop=None, daemon=None):
-        if self._thread is None:
-            t = self.to_thread(loop=loop, trylog=trylog, keepalive=keepalive, daemon=daemon)
-        else: t = self._thread
-        
-        if add_to is not None:
-            add_to.append(t)
-        
-        t.start()
-        
-        if join: t.join()
-        
-        return t
-    
-    
-    def to_thread(self, group=None, name=None, *, trylog=True, keepalive=False, loop=None, daemon=None):
-        default =  '({})Thread'.format(self._name) \
-                        if str(self._name)[-1:].isdigit() else \
-                    '{}Thread'.format(self._name)
-        new_name = create_name(name, default=default, add_int='if_taken')
-        #Note that self.loop may already be wrapped in u_errors.trylog if `keepalive` was passed to __init__
-        
-        #if self._inf['keepalive'] is set (self.loop wrapped), then we don't want to extra wrap with trylog
-        # unless specific instructions are passed
-        if not self._inf['keepalive']: pass
-        elif not (isinstance(trylog,dict) and len(trylog)):
-            trylog=False
-            
-        if keepalive is True: keepalive = {'throw': TerminatedException}
-        elif isinstance(keepalive,dict) and 'throw' not in keepalive:
-            keepalive = dict(keepalive, throw=TerminatedException)
-            
-        t = EliThread(group=group, target=self.loop, loop=loop, name=new_name, daemon=daemon, trylog=trylog, keepalive=keepalive)
-        self._thread = t
-        
-        return t
-    
-
-    def start_process(self, join=False, add_to=None):
-        if self._process is None:
-            t = self.to_process()
-        else: t = self._process
-        
-        if add_to is not None:
-            add_to.append(t)
-        
-        t.start()
-        
-        if join: t.join()
-        
-        return t
-    
-    
-    def to_process(self, group=None, name=None, *, daemon=None):
-        default =  '({})Process'.format(self._name) if str(self._name)[-1:].isdigit() else '{}Thread'.format(self._name)
-        new_name = create_name(name, default=default, add_int='if_taken')
-        
-        t = LogiProcess(group=group, target=self.loop, name=new_name, daemon=daemon)
-        
-        self._process = t
-        
-        return t
-    
-    _thread = None
-    _process = None
-    
-
-
-class Ticker(TPMethods, ScheduleTicker):
-    pass
-    
-
-
-class AsyncTicker(AsyncBaseTicker, ScheduleTicker):
-    def __init__(self,*args,loop=None,**kw):
-        super().__init__(*args,loop=loop,**kw)
-        self._inf['target']['isCoro'] = asyncio.iscoroutinefunction(self._inf['target']['target'])
-        self._inf['return2']['isCoro'] = asyncio.iscoroutinefunction(self._inf['return2']['target'])
-    
-    
-    @async_callback
-    async def tick(self, force=False, errors=None, update_supers=True):
-        """Does the "tick", i.e tries to call the target;
-           if Ticker is closed, raises TerminatedException;
-           elif force == True, target is called always;
-           else checks if the time has arrived;
-           
-           if time has not arrived, handles `errors`:
-             'error' - raises WaitException
-             'warn' - warns and returns return2()
-             'hide' - returns return2()
-             'sleep' - sleeps until time has arrived, returns target()
-             
-           else returns .target()
-           
-           
-           If .target() raises QuitException,
-             closes (it)self
-             returns QuitException.value if it has one,
-                     else .return2()
-             
-             
-           Note that QuitException raised from .return2 is not caught.
-           """
-        
-        self._ui['attempts'].appendleft(dt.utcnow())
-           
-        self._verify_is_open()
-
-        
-        if errors is None:
-            errors = self._inf['errors']
-        
-        
-        if force is not True:
-            remaining = self.get_time_remaining()
-            
-            if remaining <= 0: pass
-            
-            elif errors == 'hide': 
-                return await self.return2()
-            
-            elif errors == 'warn':
-                logger.debug('{} skipping tick() - wait of {} needed'.format(self._name,math.ceil(remaining)))
-                return await self.return2()
-            
-            elif errors == 'sleep':
-                await self.sleep({'remaining': remaining})
-                
-            else: raise WaitException(remaining)
-        
-
-        #update timestamps
-        self._ticktock()
-    
-    
-        try:
-            response = await self.target()
-            self._interval_updating()
-        
-        except QuitException as e:
-            #if level > 0, then was raised by return2,
-            # which is not allowed
-            if e._level: raise e
-            elif len(e.args): 
-                response = e.args[0]
-            else: response = await self.return2()
-            
-            await self.close()
-            
-        except WaitException as e:
-            e._level += 1
-            raise e
-            
-        finally:
-            #update timestamps
-            self._ticktock2()
-            if update_supers:
-                self._update_supers()
-
-
-        return response
-    
-
-    async def target(self):
-        """Calling the target function, returning its output.
-           This method may be overridden for custom use."""
-        d = self._inf['target']
-        target = d['target']
-        
-        if target is None: pass
-        elif d['isCoro']:
-            return await target(*d['args'],**d['kwargs'])
-        else:
-            return target(*d['args'],**d['kwargs'])
-        
-        try: return await self.return2()
-        except QuitException as e:
-            e._level += 1
-            raise e
-        
-    
-    async def return2(self):
-        """Called from tick() if it determines _is_tick_time() == False, with `errors` 
-           set to 'warn' or 'hide'; or from target() if target has not been set.
-           This method may be overridden for custom use."""
-        r2 = self._inf['return2']
-        
-        if not r2['target']: 
-            value = r2['value']
-        elif r2['isCoro']:
-            value = await r2['target'](*r2['args'],**r2['kwargs'])
-        else:
-            value = r2['target'](*r2['args'],**r2['kwargs'])
-
-        
-        if r2['copy']:
-            #value = _copy(value)
-            value = r2['copyfunc'](value)
-
-        return value
-    
-    
-################################################################    
-
-class BaseTickManager(BaseTicker):
-    def __init__(self, tickers, *, errors='raise', allterminated='sleep',
-                 callback=None, keepalive=None, name=None, close_subs=False,
-                 logging_level=None, gc_closed=True):
-        """Its tick method ticks the next of its tickers"""
-        super().__init__(callback=callback,keepalive=keepalive,name=name,logging_level=logging_level)
-        
-        if tickers is None: tickers = []
-            
-        self._tickers = {'open': [], 'closed': []}
-        self._timer = {}
-
-        for ticker in tickers:
-            self.add_ticker(ticker)
-
-        if errors is None: errors = 'raise'
-        elif errors not in ('raise','sleep'):
-            raise ValueError(errors)
-        
-        if allterminated is None: allterminated = 'sleep'
-        elif allterminated not in ('sleep','raise','close'):
-            raise ValueError(allterminated)
-
-        
-        self._inf['errors'] = errors 
-        self._inf['allterminated'] = allterminated
-        self._inf['close_subs'] = close_subs
-        self._inf['gc_closed'] = gc_closed
-        
-        
-    def add_ticker(self, ticker):
-        if not isinstance(ticker,BaseTicker):
-            raise TypeError('`ticker` must inherit from BaseTicker; got type: {}'.format(type(ticker)))
-        elif ticker in self._tickers['open'] or ticker in self._tickers['closed']:
-            raise TickerAlreadyAdded('Ticker {} has already been added to {}'.format(ticker._name, self._name))
-        elif ticker._closed:
-            raise TerminatedException('{} is closed. Cannot add to {}'.format(ticker._name,self._name))
-        
-        self._tickers['open'].append(ticker)
-        ticker._supers.add(self)
-        
-        #this will also set self._hidden['updated'], 
-        #causing AllTerminated 'sleep' mode to wake up (if allterminated was set to 'sleep'),
-        #and also all parent tickers to wake up
-        self._update_timer(ticker,True)
-        
-      
-    @callback
-    def tick(self, errors=None, update_supers=True):
-        if errors is None:
-            errors = self._inf['errors']
-        
-        while self._verify_is_open():
-            self._remove_terminated()
-            
-            valid = (x for x in self._timer.items() if x[1] is not None)
-            
-            #AllTerminated will be raised only in the nth (highest) level manager's .tick
-            # assuming that is the only one which's .tick is called
-            # (the sub tickers' .tick called by nth's .tick are all guaranteed to be "valid")
-            try: ticker,earliest = min(valid, key=lambda x: x[1])
-            except ValueError:
-                raise AllTerminated('{} - all tickers are terminated.'.format(self._name))
-            
-                
-            time_remaining = earliest - dt.utcnow()
-            secs = time_remaining.total_seconds()
-            
-            if secs > 0:
-                if errors == 'sleep':
-                    self.sleep(secs)
-                    continue
-                else: raise WaitException(secs)
-
-            try: 
-                ticker.tick(update_supers=update_supers)
-                #self._update_timer(ticker, update_supers)
-                break
-            
-            except AllTerminated as e:
-                e._level += 1
-                raise e
-            
-            except TerminatedException as e:
-                if not e._level: 
-                    continue
-                e._level += 1
-                raise e
-        
-        
-    def loop(self, update_supers=True):
-        self._verify_is_open()
-        tlogger.log(self.logging_level,'Starting ticker loop: {}'.format(self.name))
-        try:
-            while True:
-                try: self.tick(errors='sleep',update_supers=update_supers)
-                except AllTerminated as e:
-                    if e._level: raise e
-                    try: self._handle_all_terminated()
-                    except TerminatedException: break
-                except TerminatedException as e:
-                    if not e._level: break
-                    else: raise e
-        finally:
-            tlogger.log(self.logging_level,'Ticker loop ended: {}'.format(self.name))
-        
-
-    def _remove_terminated(self):
-        open = self._tickers['open']
-        len_tickers = len(open)
-        for i,ticker in enumerate(reversed(open)):
-            if ticker._closed:
-                del open[len_tickers-(i+1)]
-                del self._timer[ticker]
-                if not self._inf['gc_closed']:
-                    self._tickers['closed'].append(ticker)
-   
-   
-    def _handle_all_terminated(self):
-        at = self._inf['allterminated']
-        if at == 'raise':
-            raise AllTerminated('{} - all tickers are terminated.'.format(self._name))
-        elif at == 'close':
-            self.close()
-        else:
-            self.sleep('updated')
-   
-        
-    def _update_timer(self, ticker, update_supers=True):
-        try: _next = ticker.get_time_remaining(as_float=False) + dt.utcnow()
-        except AllTerminated:
-            self._timer[ticker] = None
-        else: self._timer[ticker] = _next
-        
-        with self._hidden['lock']:
-            self._hidden['updated'].set()
-        
-        if update_supers:
-            self._update_supers()
-    
-    
-    def get_earliest(self):
-        vals = (x for x in self._timer.values() if x is not None)
-        try: return min(vals)
-        except ValueError:
-            raise AllTerminated('{} - all tickers are terminated'.format(self._name))
-    
-    def get_time_remaining(self, as_float=True):
-        delta = self.get_earliest() - dt.utcnow()
-        
-        if as_float:
-            return delta.total_seconds()
-        return delta
-        
-
-class TickManager(TPMethods, BaseTickManager):
-    def close(self):
-        super().close()
-        if self._inf['close_subs']:
-            for t in self._tickers['open']:
-                t.close()
-        self._remove_terminated()
-
-
-class AsyncTickManager(AsyncBaseTicker, BaseTickManager):
-    def __init__(self,tickers,*, loop=None, allterminated='sleep', **kw):
-        """Asynchronous version of TickManager."""
-        super().__init__(None, loop=loop, allterminated=allterminated, **kw)
-        
-        self._hidden['queue'] = asyncio.Queue(loop=self._inf['event_loop'])
-
-        if tickers is None:
-            tickers = []
-            
-        for t in tickers:
-            self.add_ticker(t)
-        
-
-    def add_ticker(self, ticker):
-        if not isinstance(ticker,AsyncBaseTicker):
-            raise TypeError('`ticker` must inherit from AsyncBaseTicker; got type: {}'.format(type(ticker)))
-        TickManager.add_ticker(self, ticker)
-        loop = self._inf['event_loop'] #ticker._inf['event_loop']
-        async def put():
-            await self._hidden['queue'].put(ticker)
-            with self._hidden['lock']:
-                self._hidden['updated'].set()
-        f = functools.partial(asyncio.ensure_future, put(), loop=loop)
-        loop.call_soon(f)
-        
-        
-    async def _get_free_ticker(self):
-        ticker = await self._hidden['queue'].get()
-        
-        if isinstance(ticker,QuitException):
-            raise TerminatedException('{} is closed'.format(self._name))
-        
-        return ticker
-    
-    
-    async def _tick_and_release(self, ticker, *args, **kw):
-        try: 
-            await ticker.tick(*args,**kw)
-        except TerminatedException as e:
-            #Note that .tick tries to remove any terminated tickers before calling ._tick_and_release, but sometimes
-            # due to delay the ticker may close *in the meanwhile*, and due to .tick_and_release being called through
-            # loop.call_soon() (not directly await .tick_and_release()), the exception shows up on the log
-            #That's why decided *not* to raise the TerminatedException here
-            """"e._level += 1
-            raise e"""
-            return
-        else:
-            callback = self._inf['callback']['target']
-            if callback is None: pass
-            elif self._inf['callback']['isCoro']:
-                await callback({'result': None, 'ticker': self, 'ts': dt.utcnow()})
-            else: callback({'result': None, 'ticker': self, 'ts': dt.utcnow()})
-                
-            #self._update_timer(ticker, False)
-        finally:
-            await self._hidden['queue'].put(ticker)
-    
-    
-    async def tick(self, errors=NotImplemented, update_supers=True):
-        while self._verify_is_open():
-            self._remove_terminated()
-            
-            if not len(self._tickers['open']):
-                await self._handle_all_terminated()
-            
-            ticker = await self._get_free_ticker()
-            if ticker._closed:
-                continue
-            
-            loop=self._inf['event_loop'] #ticker._inf['event_loop']
-            coro = self._tick_and_release(ticker,errors='sleep',update_supers=update_supers)
-            f = functools.partial(asyncio.ensure_future, coro, loop=loop)
-            loop.call_soon(f)
-            break
-        
-        
-    async def loop(self, update_supers=True):
-        """cours = (ticker.loop() for ticker in self._tickers['open'])
-        await asyncio.gather(*cours, return_exceptions=True)"""
-        self._verify_is_open()
-        tlogger.log(self.logging_level,'Starting ticker loop: {}'.format(self.name))
-        try:
-            while True:
-                try: await self.tick(update_supers=update_supers)
-                except TerminatedException as e:
-                    break
-                    """if not e._level: break
-                    else: raise e"""
-                    #e._level is always 0, 
-                    # because ticker.tick() in self.tick() does not raise
-                """No AllTerminated is needed to be caught, 
-                   as it is already handled in the tick"""
-        finally:
-            tlogger.log(self.logging_level,'Ticker loop ended: {}'.format(self.name))
-    
-    
-    async def _handle_all_terminated(self):
-        at = self._inf['allterminated']
-        if at == 'raise':
-            raise AllTerminated('{} - all tickers are terminated.'.format(self._name))
-        elif at == 'close':
-            await self.close()
-        else:
-            await self.sleep('updated')
-            
-            
-    async def sleep(self, time=None):
-        """This works but is not meant to be used with time=`None`,
-           as calling get_time_remaining() will fail if no tickers are left"""
-        await super().sleep(time)
-        
-            
-    async def close(self):
-        event = self._hidden['closed']
-            
-        if not event.is_set():
-            await self._hidden['queue'].put(QuitException())
-            
-        await super().close()
-        
-        if self._inf['close_subs']:
-            for t in self._tickers['open']:
-                if isinstance(t,AsyncBaseTicker):
-                    await t.close()
-                else: t.close()
-                
-        self._remove_terminated()
-        
-        
-    _hidden = {'closed': None, 'updated':None, 'lock': None, 'queue': None}
-    
-
-
-class Routine:
-    def __init__(self, sched={}, tickmgr={}, *, name=None):
-        self._locks = {-1: asyncio.Lock()}
-        self._events = {}
-        
-        #this contains instructions for creating various tickers,
-        #a dict *key* will later identify 
-        # 1. its corresponding ticker in self._tickers ({key: resulting_ticker}),
-        # 2. its corresponding event in self._events
-        #a dict *value* will be used to create the ticker, and should be in the format 
-        #{
-        # target:method_name_or_function,
-        # args:target_args,
-        # kwargs:target_kwargs,
-        # lock_id:None/<int>/<asyncio.Lock>
-        # no_set_event_on: if target returns this value, event will not be set
-        #  -- (NB! the comparison operator is `is` ("value is no_set_event_on"), therefore strings/ints/floats.. will not do)
-        #  --defaults to False
-        # ..all other arguments that can be passed to AsyncTicker.__init__
-        #}
-        # may be updated manually, calling self.sched.update({..}) in a subclass
-        if not isinstance(sched,dict):
-            raise TypeError(type(sched))
-        self.sched = sched.copy()
-        
-        if name is None and hasattr(self.__class__,'_name'):
-            name = self.__class__._name
-        self._name = create_name(name, default=self.__class__.__name__, registry=_ROUTINE_NAMES)
-        
-        tcm = tickmgr.copy()
-        if tcm.get('close_subs') is None:
-            tcm['close_subs'] = True
-        if 'tickers' not in tcm: tcm['tickers'] = []
-        if tcm.get('name') is None: tcm['name'] = self.name + '-TickManager'
-        
-        self._tickmgr = AsyncTickManager(**tcm)
-        self._tickers = {}
-    
-    
-    def create_schedule(self):
-        """Creates tickers out of .sched attribute.
-        May also be called while Routine is already running (.start has been called)"""
-
-        def wrap_callback(cb,event,**kw):
-            #NB! _accpets_args must be called before wrapping to corotine
-            # due to coroutine() replacing it with *args and **kw
-            cb_is_set = cb is not None
-            accepts_args = cb_is_set and _accepts_args(cb)
-            iscoro = cb_is_set and asyncio.iscoroutinefunction(cb)
-            """if not asyncio.iscoroutinefunction(cb):
-                cb = asyncio.coroutine(cb)"""
-            
-            no_set_event_on = kw.get('no_set_event_on')
-            if no_set_event_on is None: pass
-            elif not hasattr(no_set_event_on,'__call__'):
-                raise TypeError('`no_set_event_on` must be None or have attr "__call__"; got: {}'.format(no_set_event_on)) 
-            
-            async def set_event(*args):
-                #ticker @callback passes {'result': , 'ticker': ,'ts': }
-                #print(cb_is_set,set_event_on,args[0]['result'],set_event_on(args[0]['result']))
-                if no_set_event_on is None or not no_set_event_on(args[0]['result']):
-                    event.set()
-                if not cb_is_set: pass
-                elif accepts_args:
-                    if not iscoro: cb(*args)
-                    else: await cb(*args)
-                else:
-                    if not iscoro: cb()
-                    else: await cb()
-
-            return set_event
-        
-        logger.debug('{} - creating schedule'.format(self.name))
-        max_lock_id = max(self._locks)
-        for n,params in self.sched.items():
-            #Only new schedule items will be added
-            #If want remove from schedule, call .remove(name)
-            if n in self._tickers: continue
-            lock_id = params.get('lock_id')
-            if isinstance(lock_id,asyncio.Lock):
-                try: lock_id = next(x for x,y in self._locks.items() if lock_id is y)
-                except StopIteration:
-                    max_lock_id = max_lock_id + 1
-                    self._locks[max_lock_id] = lock_id
-                    lock_id = max_lock_id   
-            elif lock_id is None: 
-                lock_id = max_lock_id = max_lock_id + 1
-
-            if not isinstance(lock_id,int): 
-                raise TypeError(type(lock_id))
-            elif lock_id not in self._locks:
-                max_lock_id = max(max_lock_id,lock_id)
-                self._locks[lock_id] = asyncio.Lock()
-
-            targkw = [params.get(p) for p in ('target','args','kwargs')]
-            rout_kw = {'lock_id': lock_id}
-            tickConfig = {x:y for x,y in params.items() if x not in ('target','args','kwargs','lock_id','no_set_event_on')} 
-            
-            self._events[n] = event = asyncio.Event()
-            
-            cb = tickConfig.get('callback')
-            nseo = {x:y for x,y in params.items() if x=='no_set_event_on'}
-            tickConfig['callback'] = wrap_callback(cb,event,**nseo)
-            if tickConfig.get('name') is None:
-                tickConfig['name'] = '{}-{}-Ticker'.format(self.name,n)
-
-            ticker = AsyncTicker(self._routine, args=targkw, kwargs=rout_kw, **tickConfig)
-            self._tickmgr.add_ticker(ticker)
-            self._tickers[n] = ticker
-    
-    
-    async def start(self):
-        self._tickmgr._verify_is_open()
-        self.create_schedule()
-        logger.debug('Starting routine {}'.format(self.name))
-        try: await self._tickmgr.loop()
-        finally: tlogger.debug('Routine ended: {}'.format(self.name))
-    
-    
-    async def _routine(self, target, args, kwargs, lock_id):
-        if args is None: args = tuple()
-        if kwargs is None: kwargs = {}
-        method = getattr(self, target) if isinstance(target,str) else target
-        
-        lock = self._locks[lock_id]
-        
-        with await lock:
-            if asyncio.iscoroutinefunction(method):
-                return await method(*args,**kwargs)
-            else:
-                return method(*args,**kwargs)
-    
-    
-    async def remove(self,name,from_sched=True):
-        lock_id = self.get_lock_id(name)
-        await self.get_ticker(name).close()
-        del self._tickers[name]
-        del self._events[name]
-        if lock_id != -1 and not any(self.get_lock_id(n) == lock_id for n in self._tickers):
-            del self._locks[lock_id]
-        if from_sched and name in self.sched:
-            del self.sched[name]
-        #Note that removing all tickers will not cause the running tickmgr to stop,
-        # unless .__init__(..,tickmgr={'allterminated':'close'}) was passed
-    
-    
-    async def close(self):
-        await self._tickmgr.close()
-    
-    
-    def get_ticker(self,name):
-        return self._tickers[name]
-    
-    def get_event(self,name):
-        return self._events[name]
-    
-    def get_lock(self,id):
-        if isinstance(id,str):
-            id = self.get_lock_id(id)
-        elif not isinstance(id,int):
-            raise TypeError(type(id))
-        return self._locks[id]
-    
-    def get_lock_id(self,name):
-        return self.get_ticker(name)._inf['target']['kwargs']['lock_id']
-        
-    @property
-    def name(self):
-        return self._name
-    @name.setter
-    def name(self,value):
-        self._name = value
+import abc
+import multiprocessing
+import asyncio
+import functools
+from functools import wraps
+import inspect
+
+from collections import deque
+import numpy as np
+import math
+import copy
+import platform
+import warnings
+import datetime
+
+dt = datetime.datetime
+td = datetime.timedelta
+
+from fons.aio import FonsEvent, FonsQueue
+from fons.debug import wrap_trylog
+import fons.log as _log
+from fons.processes import LogiProcess
+from fons.reg import create_name
+from fons.threads import EliThread
+import fons.time as fontime
+from fons.errors import (
+    QuitException,
+    WaitException,
+    TerminatedException,
+    TickerException,
+    TickerAlreadyAdded,
+    AllTerminated,
+    TickerQuitException,
+    TickerWaitException,
+    TickerTerminated,
+)
+
+
+logger, logger2, tlogger, tloggers, tlogger0 = _log.get_standard_5(__name__)
+
+LOGGING_LEVEL = 10
+_PLATFORM = platform.system()
+_TICKER_NAMES = set()
+_ROUTINE_NAMES = set()
+
+
+# Automatically assigns class attribute " _name" (= the name of class)
+# if user has not specified the attribute itself
+class _AddName(type):
+    def __new__(cls, name, bases, attrs):
+        newattrs = {"_name": name}
+        newattrs.update(attrs)
+
+        return super(_AddName, cls).__new__(cls, name, bases, newattrs)
+
+
+def _to_td(value):
+    if isinstance(value, td):
+        return value
+    elif isinstance(value, (int, float)):
+        return td(seconds=value)
+    else:
+        raise TypeError(type(value))
+
+
+def _verify_target(values, add_to=None, target_null=False):
+    if add_to is None:
+        add_to = {}
+
+    if not len(values):
+        raise ValueError("Target not given")
+
+    target = values[0]
+
+    if target_null and target is None:
+        pass
+    elif not hasattr(target, "__call__"):
+        raise TypeError("Target is not callable: {}".format(target))
+
+    try:
+        args = values[1]
+    except IndexError:
+        args = None
+
+    if args is None:
+        args = tuple()
+    elif not hasattr(args, "__iter__"):
+        raise TypeError("Args is not iterable: {}".format(args))
+
+    try:
+        kwargs = values[2]
+    except IndexError:
+        kwargs = None
+
+    if kwargs is None:
+        kwargs = {}
+    elif not isinstance(kwargs, dict):
+        raise TypeError("Kwargs is not dict: {}".format(kwargs))
+
+    add_to["target"] = target
+    add_to["args"] = args
+    add_to["kwargs"] = kwargs
+
+    return add_to
+
+
+def _accepts_args(f):
+    fas = inspect.getfullargspec(f)
+    c_args = fas.args
+    # inspect.ismethod is accurate whether or not "self" is first arg,
+    # or if it only has *args
+    if inspect.ismethod(f):
+        c_args = c_args[1:]
+    return len(c_args) > 0 or fas.varargs
+
+
+def callback(f):
+    @wraps(f)
+    def wrapper(*args, **kw):
+        self = args[0]
+        callback = self._inf["callback"]["target"]
+        accepts_arg = self._inf["callback"]["accepts_arg"]
+        result = f(*args, **kw)
+
+        if callback is not None:
+            if accepts_arg:
+                callback({"result": result, "ticker": self, "ts": dt.utcnow()})
+            else:
+                callback()
+
+        return result
+
+    return wrapper
+
+
+def async_callback(f):
+    @wraps(f)
+    async def wrapper(*args, **kw):
+        self = args[0]
+        callback = self._inf["callback"]["target"]
+        accepts_arg = self._inf["callback"]["accepts_arg"]
+        result = await f(*args, **kw)
+
+        if callback is None:
+            pass
+        elif self._inf["callback"]["isCoro"]:
+            if accepts_arg:
+                await callback({"result": result, "ticker": self, "ts": dt.utcnow()})
+            else:
+                await callback()
+        else:
+            if accepts_arg:
+                callback({"result": result, "ticker": self, "ts": dt.utcnow()})
+            else:
+                callback()
+
+        return result
+
+    return wrapper
+
+
+# ----------------------------------------------------------------------
+
+
+class BaseTicker(metaclass=abc.ABCMeta):
+    def __init__(self, *, callback=None, keepalive=None, name=None, logging_level=None):
+        self._inf = copy.deepcopy(self._inf)
+        self._ui = copy.deepcopy(self._ui)
+        self._hidden = copy.deepcopy(self._hidden)
+
+        self._inf["callback"]["target"] = callback
+        self._supers = set()
+
+        if callback is not None:
+            self._inf["callback"]["accepts_arg"] = _accepts_args(callback)
+
+        self._inf["keepalive"] = bool(isinstance(keepalive, dict) or keepalive)
+        self._inf["keepalive_params"] = (
+            dict({"attempts": True, "throw": TerminatedException}, **keepalive)
+            if isinstance(keepalive, dict)
+            else {"attempts": True, "throw": TerminatedException}
+        )
+        if self._inf["keepalive"]:
+            self.loop = wrap_trylog(self.loop, **self._inf["keepalive_params"])
+
+        self._hidden["closed"] = multiprocessing.Event()
+        self._hidden["updated"] = multiprocessing.Event()
+        self._hidden["lock"] = multiprocessing.Lock()
+
+        if name is None and hasattr(self.__class__, "_name"):
+            name = self.__class__._name
+        self._name = create_name(
+            name, default=self.__class__.__name__, registry=_TICKER_NAMES
+        )
+
+        self.logging_level = (
+            logging_level if logging_level is not None else LOGGING_LEVEL
+        )
+
+    @abc.abstractmethod
+    def tick(self, errors="raise", update_supers=True):
+        pass
+
+    @abc.abstractmethod
+    def get_time_remaining(self):
+        pass
+
+    def __call__(self, *args, **kw):
+        return self.tick(*args, **kw)
+
+    def loop(self, update_supers=True):
+        """Loops the tick method, with `errors` set to 'sleep'"""
+        self._verify_is_open()
+        tlogger.log(self.logging_level, "Starting ticker loop: {}".format(self.name))
+        try:
+            while True:
+                try:
+                    self.sleep()
+                    self.tick(errors="sleep", update_supers=update_supers)
+                except TerminatedException as e:
+                    if self._closed:
+                        break
+                    else:
+                        raise e
+        finally:
+            tlogger.log(self.logging_level, "Ticker loop ended: {}".format(self.name))
+
+    def _update_supers(self):
+        for s in self._supers:
+            s._update_timer(self, update_supers=True)
+
+    def sleep(self, time="remaining"):
+        t0 = time
+        if isinstance(time, dict):
+            t0, time = next(iter(time.items()))
+
+        event = self._hidden["updated"]
+        lock = self._hidden["lock"]
+        tlogger0.log(
+            self.logging_level,
+            "Sleeping on ticker {} (time: {})".format(self.name, time),
+        )
+        try:
+            while True:
+                with lock:
+                    self._verify_is_open()
+                    if time == "updated":
+                        time = None
+                    elif time == "remaining":
+                        time = max(0, self.get_time_remaining())
+                        event.clear()
+
+                if event.wait(time):
+                    event.clear()
+                    self._verify_is_open()
+                    time = t0
+                    if time == "remaining":
+                        continue
+                break
+        finally:
+            tlogger0.log(self.logging_level, "Sleep ended: {}".format(self.name))
+
+    def close(self):
+        tlogger.log(self.logging_level, "Closing ticker {}".format(self.name))
+        with self._hidden["lock"]:
+            if not self._closed:
+                self._ui["time_closed"] = dt.utcnow()
+                self._closed = True
+
+            if not self._hidden["closed"].is_set():
+                self._hidden["closed"].set()
+            if not self._hidden["updated"].is_set():
+                self._hidden["updated"].set()
+
+    def _verify_is_open(self):
+        if self._closed:
+            raise TerminatedException("{} is closed".format(self._name))
+        return True
+
+    @property
+    def name(self):
+        return self._name
+
+    @name.setter
+    def name(self, value):
+        self._name = value
+
+    _inf = {
+        "callback": {"target": None, "accepts_arg": None},
+        "keepalive": False,
+        "keepalive_params": {},
+    }
+    _ui = {"time_closed": None}
+    _hidden = {"closed": None, "updated": None, "lock": None}
+    _closed = False
+
+
+class AsyncBaseTicker(BaseTicker):
+    def __init__(self, *args, loop=None, **kw):
+        super().__init__(*args, **kw)
+        if loop is None:
+            loop = asyncio.get_event_loop()
+        self._inf["event_loop"] = loop
+        self._hidden["closed"] = FonsEvent(loop=loop)
+        self._hidden["updated"] = FonsEvent(loop=loop)
+        # self._hidden['lock'] = asyncio.Lock()
+        self._inf["callback"]["isCoro"] = asyncio.iscoroutinefunction(
+            self._inf["callback"]["target"]
+        )
+
+    async def __call__(self, *args, **kw):
+        return await self.tick(*args, **kw)
+
+    async def loop(self, update_supers=True):
+        """Loops the tick method, with `errors` set to 'sleep'"""
+        self._verify_is_open()
+        tlogger.log(self.logging_level, "Starting ticker loop: {}".format(self.name))
+        try:
+            while True:
+                try:
+                    await self.tick(errors="sleep", update_supers=update_supers)
+                except TerminatedException as e:
+                    if self._closed:
+                        break
+                    raise e
+        finally:
+            tlogger.log(self.logging_level, "Ticker loop ended: {}".format(self.name))
+
+    async def sleep(self, time="remaining"):
+        t0 = time
+        if isinstance(time, dict):
+            t0 = next(iter(time))
+            time = next(iter(time.values()))
+
+        event = self._hidden["updated"]
+        lock = self._hidden["lock"]
+        loop = self._inf["event_loop"]
+        is_windows = _PLATFORM == "Windows"
+        tlogger0.log(
+            self.logging_level,
+            "Sleeping on ticker {} (time: {})".format(self.name, time),
+        )
+        try:
+            while True:
+                with lock:
+                    self._verify_is_open()
+                    if time == "updated":
+                        time = None
+                    elif time == "remaining":
+                        time = max(0, self.get_time_remaining())
+                        event.clear()
+
+                if time is not None and time <= 0:
+                    break
+
+                sleep_time = time
+                if time is not None:
+                    # Anything below 0.001 for non-windows and 0.016 for windows
+                    # may not be slept to the end.
+                    sleep_time = max(0.001, time)
+                    if is_windows:
+                        sleep_time = max(0.016, time)
+
+                try:
+                    await asyncio.wait_for(event.wait(), sleep_time)
+                    event.clear()
+                    self._verify_is_open()
+                    # Event was set. Break out.
+                    if t0 != "remaining":
+                        break
+                except asyncio.TimeoutError:
+                    # We can't break out of the loop yet, as asyncio.sleep isn't completely accurate
+                    pass
+                finally:
+                    time = t0
+        finally:
+            tlogger0.log(self.logging_level, "Sleep ended: {}".format(self.name))
+
+    async def close(self):
+        super().close()
+
+
+#############################################################################
+
+
+class ScheduleTicker(BaseTicker):
+    """For calling targetfunc in time restricted manner,
+    .tick() or simply () attempts to call the target and return its output
+    .loop() cycles the target endlessly
+    .run() creates and runs a new thread with .loop as its target"""
+
+    def __init__(
+        self,
+        target=None,
+        interval=None,
+        sync=None,
+        args=None,
+        kwargs=None,
+        *,
+        delay=None,
+        lock=None,
+        keep=5,
+        errors="raise",
+        return2=None,
+        return2_call=False,
+        callback=None,
+        keepalive=None,
+        name=None,
+        **kw
+    ):
+        """
+        Args [Optional]:
+          target (func):
+            target func
+
+
+          interval (int,float,timedelta,Ticker,callable,list/tuple):
+            tick interval
+            --<td,int,float,str,DateOffset> -> fontime.freq_to_offset(interval)
+            --<list/tuple> -> [callable, args, kw]
+            if Ticker, its tick() must return interval
+            if callable, must return interval
+
+
+          sync (datetime, timedelta,int,float, str: 'first','epoch','epoch-delay','random','interval' / offset-like, Offset)):
+            point in time which measures integer number of intervals passed;
+            ::default: None
+            --<timedelta,int,float,offset-like,DateOffset> -> <datetime || fontime.dt_round(dt.utcnow(), sync)>
+            --<str>: 'epoch'  [epoch is the moment of tick() being called for the 1st time]
+                     'first'  [first = first_entry, guarantees t(2nd_tick()) - t(1st_tick()) = interval]
+                     'random' [random point of time in tp: (dt_round(dt.utcnow(),interval), interval)]
+                     'interval-<start>..<end>' [dt_round(dt.utcnow(), interval); [OPTIONAL] <start> / <end> floats in range(0,1)]
+
+
+            if None, each entry is counted from the *end* of the last tick
+             e.g if target takes unusually long, the interval will still be added on top of that
+             --delay must be None
+            otherwise each new entry is synced to the sync point
+              entry = sync + n*interval  || [n E int] || entry < dt.utcnow()
+
+            ( tick can be called if dt.utcnow() > last_entry + interval + delay )
+
+
+          args (listlike):
+            target func args
+          kwargs (dict):
+            target func kwargs
+
+          ---------------------------
+
+          delay(timedelta,int,float, str: offset-like, Offset):
+            if sync != None, this will be added to sync [next = last + interval + delay]
+            --<timedelta,int,float,str,DateOffset> -> fontime.freq_to_offset(delay)
+
+
+
+
+          lock (datetime, timedelta, float,int, str: 'next'/offset-like, Offset):
+            forbids updating until the given moment in datetime
+            --<timedelta,int,float,offset-like,DateOffset> -> <datetime || dt.utcnow() + fontime.freq_to_offset(lock)>
+            --<str>
+              'next' - lock is synced to *next* tick() time from dt.utcnow()
+                        [but sync param itself must be None or value (cannot be str variable)]
+            ------------------------
+          errors (str):
+            'raise' - raise WaitError if tick is called prematurely
+            'warn' - warn, and return return2
+            'hide' - return return2
+          return2 (obj):
+            returned by tick() when errors == 'hide'/'warn'
+          return2_call (bool):
+            if True, then return2 is returned as return2()
+             in that case return2 can be passed as [target2,args2,kwargs2]
+          callback (function):
+             a single-argument function to be called after each tick;
+              argument to be passed: {"result": result, "ticker": ticker, "ts": timestamp}
+          name (str,int):
+            name of the Ticker instance, if int then added to the end of cls.__name__
+
+        **kw
+          return2_copy (bool, func):
+            if True, the .return2() output will be deepcopied before returned
+            if function, this function will be used to copy .return2() before returned
+        """
+        super().__init__(
+            callback=callback,
+            keepalive=keepalive,
+            name=name,
+            logging_level=kw.get("logging_level"),
+        )
+
+        if interval is None:
+            self.interval = self._interval
+        else:
+            self.interval = interval
+
+        interval = self._ui["interval"]
+
+        if sync is None:
+            pass
+        elif isinstance(sync, str):
+            repl = sync.replace(" ", "").lower()
+            if repl.startswith("random"):
+                range_part = repl[repl.find("-") + 1 :] if repl.find("-") != -1 else ""
+                ddloc = range_part.find("..")
+                to_float = lambda x, default: default if not len(x) else float(x)
+                try:
+                    fa, fb = (
+                        (0, 1)
+                        if ddloc == -1
+                        else (
+                            to_float(range_part[:ddloc], 0),
+                            to_float(range_part[ddloc + 2 :], 1),
+                        )
+                    )
+                except Exception:
+                    raise ValueError("Could not understand `sync`: {}".format(sync))
+                if fa < 0:
+                    raise ValueError(
+                        "Sync `random` left endpoint must be >= 0; sync: {}".format(
+                            sync
+                        )
+                    )
+                elif fb > 1:
+                    raise ValueError(
+                        "Sync `random` right endpoint must be <= 1; sync: {}".format(
+                            sync
+                        )
+                    )
+                elif fa > fb:
+                    raise ValueError(
+                        "Sync `random` left endpoint must be <= right endpoint; sync: {}".format(
+                            sync
+                        )
+                    )
+                t00 = fontime.dt_round(dt.utcnow(), interval)
+                interval_td = (t00 + interval) - t00
+                t0 = t00 + fa * interval_td
+                t1 = t00 + fb * interval_td
+                rand_td = (t1 - t0) * np.random.random(1)[0]
+                self._ui["sync"] = t0 + rand_td
+            elif repl == "interval":
+                self._ui["sync"] = fontime.dt_round(dt.utcnow(), interval)
+            elif repl not in ("first", "epoch", "epoch-delay"):
+                self._ui["sync"] = fontime.dt_round(
+                    dt.utcnow(), sync
+                )  # fontime.freq_to_td(sync, coerce=True)
+            else:
+                self._ui["sync"] = repl
+        elif isinstance(
+            sync, (td, float, int, fontime.offsets.DateOffset)
+        ) and not isinstance(sync, bool):
+            self._ui["sync"] = fontime.dt_round(dt.utcnow(), sync)
+        elif isinstance(sync, dt):
+            self._ui["sync"] = sync
+        else:
+            raise TypeError(type(sync))
+
+        if delay is not None:
+            delay_ofs = fontime.freq_to_offset(delay)
+            if self._ui["sync"] is None and delay_ofs.n:
+                raise ValueError("sync must not be None if delay specified")
+            self._ui["delay"] = delay_ofs
+
+        d_target = self._inf["target"]
+        _verify_target([target, args, kwargs], add_to=d_target, target_null=True)
+
+        if errors is None:
+            pass
+        elif not isinstance(errors, str):
+            raise TypeError(type(errors))
+        elif errors not in ("raise", "warn", "hide"):
+            raise ValueError(errors)
+        else:
+            self._inf["errors"] = errors
+
+        r2 = self._inf["return2"]
+
+        if return2_call is True:
+            if isinstance(return2, (list, tuple)):
+                _verify_target(return2, add_to=r2)
+            else:
+                _verify_target([return2], add_to=r2)
+
+        else:
+            r2["value"] = return2
+
+        r2_copy = kw.get("return2_copy")
+        if r2_copy is None:
+            pass
+        elif isinstance(r2_copy, bool):
+            r2["copy"] = r2_copy
+        elif hasattr(copy, "__call__"):
+            r2["copy"] = True
+            r2["copyfunc"] = copy
+        else:
+            raise TypeError(type(r2_copy))
+
+        if lock is not None:
+            self.lock = lock
+
+        for k in ("entries", "ticks", "tick_ends", "attempts"):
+            self._ui[k] = deque(self._ui[k], maxlen=keep)
+
+        tlogger.log(
+            self.logging_level,
+            "{} interval: {}".format(self._name, self._ui["_interval_str"]),
+        )
+
+        if (
+            self._inf["target"]["target"] is None
+            and self.__class__.target is ScheduleTicker.target
+        ):
+            warnings.warn(
+                "Ticker's initiated target is None, nor has the target method been "
+                "overriden, henceforth tick() will only return 'return2'"
+            )
+
+    def _is_tick_time(self):
+        if self.get_time_remaining() > 0:
+            return False
+        return True
+
+    def get_time_remaining(self, as_float=True):
+        now = dt.utcnow()
+        _ui = self._ui
+
+        remaining_lock = _ui["lock"] - now
+        try:
+            remaining = (_ui["entries"][0] + _ui["interval"] + _ui["delay"]) - now
+        except IndexError:
+            remaining = td(0)
+
+        if as_float:
+            remaining_lock = remaining_lock.total_seconds()
+            remaining = remaining.total_seconds()
+
+        return max(remaining_lock, remaining)
+
+    def _synced(self, stamps):
+        ui = self._ui
+        sync, interval, delay = ui["sync"], ui["interval"], ui["delay"]
+
+        single = not hasattr(stamps, "__iter__")
+        if single:
+            stamps = [stamps]
+
+        timestamps_synced = [
+            fontime.dt_synced(x - delay, interval, sync) for x in stamps
+        ]
+
+        if single:
+            return timestamps_synced[0]
+
+        return timestamps_synced
+
+    def _ticktock_1st(self, now):
+        _ui = self._ui
+        _ui["epoch"] = now
+
+        # later in _ticktock() will be assigned _ui['first'] =  _ui['entries'][0]
+        # because if `sync` was not bound to epoch,
+        # the first = _ui['entries'][0] != now - _ui['delay'] due to sync difference
+
+        if _ui["sync"] == "first":
+            _ui["sync"] = now - _ui["delay"]
+
+        elif _ui["sync"] == "epoch":
+            _ui["sync"] = _ui["epoch"]
+
+        elif _ui["sync"] == "epoch-delay":
+            _ui["sync"] = _ui["epoch"] - _ui["delay"]
+
+    def _ticktock(self):
+        """Updates `last` and `actual_last` in the beginning of every *valid* tick,
+        i.e only called after _is_tick_time() == True"""
+
+        ui = self._ui
+        now = dt.utcnow()
+        ui["ticks"].appendleft(now)
+
+        if ui["sync"] is None:
+            return
+
+        counter = ui["counter"]
+        if not counter:
+            self._ticktock_1st(now)
+
+        entry = self._synced(now)
+        ui["entries"].appendleft(entry)
+
+        if not counter:
+            ui["first"] = entry
+
+    def _ticktock2(self):
+        """Updates `last` and `actual_last` in the *end* of every valid tick,
+        (i.e if _is_tick_time() == True and after target()/return2() completes),
+        ONLY IF sync = None"""
+        ui = self._ui
+
+        now = dt.utcnow()
+        self._ui["tick_ends"].appendleft(now)
+
+        counter = ui["counter"]
+        ui["counter"] = counter + 1
+
+        if ui["sync"] is not None:
+            return
+
+        self._ui["entries"].appendleft(now)
+
+        if not counter:
+            ui["epoch"] = now
+            ui["first"] = now
+
+    def _interval_updating(self):
+        iu = self._inf["interval_updating"]
+        if not iu["enabled"]:
+            return
+
+        try:
+            params = [iu["target"], iu["args"], iu["kwargs"]]
+            i0 = self._interval
+            self.interval = params
+            if self._interval != i0:
+                logger.debug(
+                    "{} new interval: {}".format(self._name, self._ui["_interval_str"])
+                )
+        except (WaitException, TerminatedException):
+            return
+
+    @callback
+    def tick(self, force=False, errors=None, update_supers=True):
+        """Does the "tick", i.e tries to call the target;
+        if Ticker is closed, raises TerminatedException;
+        elif force == True, target is called always;
+        else checks if the time has arrived;
+
+        if time has not arrived, handles `errors`:
+          'error' - raises WaitException
+          'warn' - warns and returns return2()
+          'hide' - returns return2()
+          'sleep' - sleeps until time has arrived, returns target()
+
+        else returns .target()
+
+
+        If .target() raises QuitException,
+          closes (it)self
+          returns QuitException.value if it has one,
+                  else .return2()
+
+
+        Note that QuitException raised from .return2 is not caught.
+        """
+
+        self._ui["attempts"].appendleft(dt.utcnow())
+
+        self._verify_is_open()
+
+        if errors is None:
+            errors = self._inf["errors"]
+
+        if force is not True:
+            remaining = self.get_time_remaining()
+
+            if remaining <= 0:
+                pass
+
+            elif errors == "hide":
+                return self.return2()
+
+            elif errors == "warn":
+                logger.debug(
+                    "{} skipping tick() - wait of {} needed".format(
+                        self._name, math.ceil(remaining)
+                    )
+                )
+                return self.return2()
+
+            elif errors == "sleep":
+                self.sleep({"remaining": remaining})
+
+            else:
+                raise WaitException(remaining)
+
+        # update timestamps
+        self._ticktock()
+
+        try:
+            response = self.target()
+            self._interval_updating()
+
+        except QuitException as e:
+            # if level > 0, then was raised by return2,
+            # which is not allowed
+            if e._level:
+                raise e
+            elif len(e.args):
+                response = e.args[0]
+            else:
+                response = self.return2()
+
+            self.close()
+
+        except WaitException as e:
+            e._level += 1
+            raise e
+
+        finally:
+            # update timestamps
+            self._ticktock2()
+            if update_supers:
+                self._update_supers()
+
+        return response
+
+    def target(self):
+        """Calling the target function, returning its output.
+        This method may be overridden for custom use."""
+        d = self._inf["target"]
+        target = d["target"]
+
+        if target is not None:
+            return target(*d["args"], **d["kwargs"])
+
+        try:
+            return self.return2()
+        except QuitException as e:
+            e._level += 1
+            raise e
+
+    def return2(self):
+        """Called from tick() if it determines _is_tick_time() == False, with `errors`
+        set to 'warn' or 'hide'; or from target() if target has not been set.
+        This method may be overridden for custom use."""
+        r2 = self._inf["return2"]
+
+        if r2["target"]:
+            value = r2["target"](*r2["args"], **r2["kwargs"])
+        else:
+            value = r2["value"]
+
+        if r2["copy"]:
+            # value = _copy(value)
+            value = r2["copyfunc"](value)
+
+        return value
+
+    @property
+    def entries(self):
+        """tick_ends if sync = None,
+        else ticks (starts) synced."""
+        return self._ui["entries"]
+
+    @property
+    def records(self):
+        """Previous tick times recorded right before .target() started and at tick end."""
+        return list(zip(self._ui["ticks"], self._ui["tick_ends"]))
+
+    @property
+    def interval(self):
+        return self._interval
+
+    @interval.setter
+    def interval(self, value):
+        _ui = self._ui
+        # if interval is Ticker, it must be tickeable at this moment
+        func = None
+
+        if isinstance(value, (list, tuple)):
+            d = _verify_target(value)
+            value = d["target"]
+        else:
+            d = {"target": None, "args": tuple(), "kwargs": {}}
+
+        if hasattr(value, "__call__") and not isinstance(
+            value, fontime.offsets.DateOffset
+        ):
+            func = value
+
+            if isinstance(func, ScheduleTicker):
+                assert func._inf["errors"] == "raise"
+
+            value = func(*d["args"], **d["kwargs"])
+
+        if value is None:
+            value = 0
+
+        ofs = fontime.freq_to_offset(value)
+
+        if func is not None:
+            self._inf["interval_updating"]["enabled"] = True
+        else:
+            self._inf["interval_updating"]["enabled"] = False
+
+        d["target"] = func
+        self._inf["interval_updating"].update(d)
+
+        _ui["interval"] = ofs
+        try:
+            _ui["_interval_str"] = ofs.freqstr
+        except AttributeError:
+            _ui["_interval_str"] = "?"
+
+        self._interval = ofs
+
+        # updating sync
+        # (the first wait time will be == interval, but the next one'd be unknown,
+        # due to entries[0] being synced to the old sync point)
+        if _ui["sync"] is not None and _ui["epoch"] is not None:
+            _ui["sync"] = self.entries[0]
+
+        self._update_supers()
+        with self._hidden["lock"]:
+            self._hidden["updated"].set()
+
+    @property
+    def lock(self):
+        return self._ui["lock"]
+
+    @lock.setter
+    def lock(self, value):
+        _ui = self._ui
+
+        if value is None:
+            value = dt.utcfromtimestamp(0)
+
+        elif isinstance(value, (int, float, td, fontime.offsets.DateOffset)):
+            value = dt.utcnow() + fontime.freq_to_offset(value)
+
+        elif isinstance(value, str):
+            if value.lower() not in ("next",):
+                value = dt.utcnow() + fontime.freq_to_offset(value)
+
+            elif _ui["sync"] is None:
+                try:
+                    value = self.entries[0] + _ui["interval"]
+                except IndexError:
+                    value = dt.utcnow() + _ui["interval"]
+                # raise ValueError('For the lock to be synced the sync must not be None')
+
+            elif not isinstance(_ui["sync"], dt):
+                raise ValueError("Sync is not initiated yet.")
+
+            else:
+                nearest_synced = self._synced(dt.utcnow())
+                value = nearest_synced + _ui["interval"] + _ui["delay"]
+
+        elif not isinstance(value, dt):
+            raise TypeError(type(value))
+
+        _ui["lock"] = value
+
+        self._update_supers()
+        with self._hidden["lock"]:
+            self._hidden["updated"].set()
+
+    def get_last(self, raw=False):
+        if raw:
+            return self._ui["records"][0][1]
+        else:
+            return self._ui["entries"][0]
+
+    def get_next(self, adjusted=True):
+        ui = self._ui
+        if ui["sync"] is None:
+            raise ValueError("Next cannot be estimated if sync = None")
+
+        last = self.get_last()
+
+        nxt = last + ui["interval"]
+        now = dt.utcnow()
+
+        if adjusted:
+            nxt_synced = self._synced(now)
+            nxt = max(nxt_synced, nxt)
+
+        return nxt
+
+    def get_sleep_time(self):
+        t = self.get_time_remaining(as_float=True)
+        return max(0.0, t)
+
+    @property
+    def counter(self):
+        return self._ui["counter"]
+
+    @property
+    def args(self):
+        return self._inf["target"]["args"]
+
+    @args.setter
+    def args(self, value):
+        self._inf["target"]["args"] = value
+
+    @property
+    def kwargs(self):
+        return self._inf["target"]["kwargs"]
+
+    @kwargs.setter
+    def kwargs(self, value):
+        self._inf["target"]["kwargs"] = value
+
+    _interval = 0
+
+    _ui = {
+        "interval": td(0),
+        "sync": None,
+        "delay": td(0),
+        "_interval_str": "0S",
+        "lock": dt.utcfromtimestamp(0),
+        "attempts": deque(maxlen=5),
+        "ticks": deque(maxlen=5),
+        "tick_ends": deque(maxlen=5),
+        "entries": deque(maxlen=5),
+        "first": None,
+        "epoch": None,
+        "counter": 0,
+        "time_closed": None,
+    }
+
+    _inf = {
+        "target": {"target": None, "args": tuple(), "kwargs": {}},
+        "errors": "raise",
+        "return2": {
+            "value": None,
+            "copy": False,
+            "copyfunc": copy.deepcopy,
+            "target": None,
+            "args": tuple(),
+            "kwargs": {},
+        },
+        "callback": {"target": None, "accepts_arg": None},
+        "keepalive": False,
+        "keepalive_params": {},
+        "interval_updating": {
+            "enabled": False,
+            "target": None,
+            "args": tuple(),
+            "kwargs": {},
+        },
+    }
+
+
+class TPMethods:
+    def start_thread(
+        self,
+        join=False,
+        add_to=None,
+        *,
+        trylog=True,
+        keepalive=False,
+        loop=None,
+        daemon=None
+    ):
+        if self._thread is None:
+            t = self.to_thread(
+                loop=loop, trylog=trylog, keepalive=keepalive, daemon=daemon
+            )
+        else:
+            t = self._thread
+
+        if add_to is not None:
+            add_to.append(t)
+
+        t.start()
+
+        if join:
+            t.join()
+
+        return t
+
+    def to_thread(
+        self,
+        group=None,
+        name=None,
+        *,
+        trylog=True,
+        keepalive=False,
+        loop=None,
+        daemon=None
+    ):
+        default = (
+            "({})Thread".format(self._name)
+            if str(self._name)[-1:].isdigit()
+            else "{}Thread".format(self._name)
+        )
+        new_name = create_name(name, default=default, add_int="if_taken")
+        # Note that self.loop may already be wrapped in u_errors.trylog if `keepalive` was passed to __init__
+
+        # if self._inf['keepalive'] is set (self.loop wrapped), then we don't want to extra wrap with trylog
+        # unless specific instructions are passed
+        if not self._inf["keepalive"]:
+            pass
+        elif not (isinstance(trylog, dict) and len(trylog)):
+            trylog = False
+
+        if keepalive is True:
+            keepalive = {"throw": TerminatedException}
+        elif isinstance(keepalive, dict) and "throw" not in keepalive:
+            keepalive = dict(keepalive, throw=TerminatedException)
+
+        t = EliThread(
+            group=group,
+            target=self.loop,
+            loop=loop,
+            name=new_name,
+            daemon=daemon,
+            trylog=trylog,
+            keepalive=keepalive,
+        )
+        self._thread = t
+
+        return t
+
+    def start_process(self, join=False, add_to=None):
+        if self._process is None:
+            t = self.to_process()
+        else:
+            t = self._process
+
+        if add_to is not None:
+            add_to.append(t)
+
+        t.start()
+
+        if join:
+            t.join()
+
+        return t
+
+    def to_process(self, group=None, name=None, *, daemon=None):
+        default = (
+            "({})Process".format(self._name)
+            if str(self._name)[-1:].isdigit()
+            else "{}Thread".format(self._name)
+        )
+        new_name = create_name(name, default=default, add_int="if_taken")
+
+        t = LogiProcess(group=group, target=self.loop, name=new_name, daemon=daemon)
+
+        self._process = t
+
+        return t
+
+    _thread = None
+    _process = None
+
+
+class Ticker(TPMethods, ScheduleTicker):
+    pass
+
+
+class AsyncTicker(AsyncBaseTicker, ScheduleTicker):
+    def __init__(self, *args, loop=None, **kw):
+        super().__init__(*args, loop=loop, **kw)
+        self._inf["target"]["isCoro"] = asyncio.iscoroutinefunction(
+            self._inf["target"]["target"]
+        )
+        self._inf["return2"]["isCoro"] = asyncio.iscoroutinefunction(
+            self._inf["return2"]["target"]
+        )
+
+    @async_callback
+    async def tick(self, force=False, errors=None, update_supers=True):
+        """Does the "tick", i.e tries to call the target;
+        if Ticker is closed, raises TerminatedException;
+        elif force == True, target is called always;
+        else checks if the time has arrived;
+
+        if time has not arrived, handles `errors`:
+          'error' - raises WaitException
+          'warn' - warns and returns return2()
+          'hide' - returns return2()
+          'sleep' - sleeps until time has arrived, returns target()
+
+        else returns .target()
+
+
+        If .target() raises QuitException,
+          closes (it)self
+          returns QuitException.value if it has one,
+                  else .return2()
+
+
+        Note that QuitException raised from .return2 is not caught.
+        """
+
+        self._ui["attempts"].appendleft(dt.utcnow())
+
+        self._verify_is_open()
+
+        if errors is None:
+            errors = self._inf["errors"]
+
+        if force is not True:
+            remaining = self.get_time_remaining()
+
+            if remaining <= 0:
+                pass
+
+            elif errors == "hide":
+                return await self.return2()
+
+            elif errors == "warn":
+                logger.debug(
+                    "{} skipping tick() - wait of {} needed".format(
+                        self._name, math.ceil(remaining)
+                    )
+                )
+                return await self.return2()
+
+            elif errors == "sleep":
+                await self.sleep({"remaining": remaining})
+
+            else:
+                raise WaitException(remaining)
+
+        # update timestamps
+        self._ticktock()
+
+        try:
+            response = await self.target()
+            self._interval_updating()
+
+        except QuitException as e:
+            # if level > 0, then was raised by return2,
+            # which is not allowed
+            if e._level:
+                raise e
+            elif len(e.args):
+                response = e.args[0]
+            else:
+                response = await self.return2()
+
+            await self.close()
+
+        except WaitException as e:
+            e._level += 1
+            raise e
+
+        finally:
+            # update timestamps
+            self._ticktock2()
+            if update_supers:
+                self._update_supers()
+
+        return response
+
+    async def target(self):
+        """Calling the target function, returning its output.
+        This method may be overridden for custom use."""
+        d = self._inf["target"]
+        target = d["target"]
+
+        if target is None:
+            pass
+        elif d["isCoro"]:
+            return await target(*d["args"], **d["kwargs"])
+        else:
+            return target(*d["args"], **d["kwargs"])
+
+        try:
+            return await self.return2()
+        except QuitException as e:
+            e._level += 1
+            raise e
+
+    async def return2(self):
+        """Called from tick() if it determines _is_tick_time() == False, with `errors`
+        set to 'warn' or 'hide'; or from target() if target has not been set.
+        This method may be overridden for custom use."""
+        r2 = self._inf["return2"]
+
+        if not r2["target"]:
+            value = r2["value"]
+        elif r2["isCoro"]:
+            value = await r2["target"](*r2["args"], **r2["kwargs"])
+        else:
+            value = r2["target"](*r2["args"], **r2["kwargs"])
+
+        if r2["copy"]:
+            # value = _copy(value)
+            value = r2["copyfunc"](value)
+
+        return value
+
+
+################################################################
+
+
+class BaseTickManager(BaseTicker):
+    def __init__(
+        self,
+        tickers,
+        *,
+        errors="raise",
+        allterminated="sleep",
+        callback=None,
+        keepalive=None,
+        name=None,
+        close_subs=False,
+        logging_level=None,
+        gc_closed=True
+    ):
+        """Its tick method ticks the next of its tickers"""
+        super().__init__(
+            callback=callback,
+            keepalive=keepalive,
+            name=name,
+            logging_level=logging_level,
+        )
+
+        if tickers is None:
+            tickers = []
+
+        self._tickers = {"open": [], "closed": []}
+        self._timer = {}
+
+        for ticker in tickers:
+            self.add_ticker(ticker)
+
+        if errors is None:
+            errors = "raise"
+        elif errors not in ("raise", "sleep"):
+            raise ValueError(errors)
+
+        if allterminated is None:
+            allterminated = "sleep"
+        elif allterminated not in ("sleep", "raise", "close"):
+            raise ValueError(allterminated)
+
+        self._inf["errors"] = errors
+        self._inf["allterminated"] = allterminated
+        self._inf["close_subs"] = close_subs
+        self._inf["gc_closed"] = gc_closed
+
+    def add_ticker(self, ticker):
+        if not isinstance(ticker, BaseTicker):
+            raise TypeError(
+                "`ticker` must inherit from BaseTicker; got type: {}".format(
+                    type(ticker)
+                )
+            )
+        elif ticker in self._tickers["open"] or ticker in self._tickers["closed"]:
+            raise TickerAlreadyAdded(
+                "Ticker {} has already been added to {}".format(
+                    ticker._name, self._name
+                )
+            )
+        elif ticker._closed:
+            raise TerminatedException(
+                "{} is closed. Cannot add to {}".format(ticker._name, self._name)
+            )
+
+        self._tickers["open"].append(ticker)
+        ticker._supers.add(self)
+
+        # this will also set self._hidden['updated'],
+        # causing AllTerminated 'sleep' mode to wake up (if allterminated was set to 'sleep'),
+        # and also all parent tickers to wake up
+        self._update_timer(ticker, True)
+
+    @callback
+    def tick(self, errors=None, update_supers=True):
+        if errors is None:
+            errors = self._inf["errors"]
+
+        while self._verify_is_open():
+            self._remove_terminated()
+
+            valid = (x for x in self._timer.items() if x[1] is not None)
+
+            # AllTerminated will be raised only in the nth (highest) level manager's .tick
+            # assuming that is the only one which's .tick is called
+            # (the sub tickers' .tick called by nth's .tick are all guaranteed to be "valid")
+            try:
+                ticker, earliest = min(valid, key=lambda x: x[1])
+            except ValueError:
+                raise AllTerminated(
+                    "{} - all tickers are terminated.".format(self._name)
+                )
+
+            time_remaining = earliest - dt.utcnow()
+            secs = time_remaining.total_seconds()
+
+            if secs > 0:
+                if errors == "sleep":
+                    self.sleep(secs)
+                    continue
+                else:
+                    raise WaitException(secs)
+
+            try:
+                ticker.tick(update_supers=update_supers)
+                # self._update_timer(ticker, update_supers)
+                break
+
+            except AllTerminated as e:
+                e._level += 1
+                raise e
+
+            except TerminatedException as e:
+                if not e._level:
+                    continue
+                e._level += 1
+                raise e
+
+    def loop(self, update_supers=True):
+        self._verify_is_open()
+        tlogger.log(self.logging_level, "Starting ticker loop: {}".format(self.name))
+        try:
+            while True:
+                try:
+                    self.tick(errors="sleep", update_supers=update_supers)
+                except AllTerminated as e:
+                    if e._level:
+                        raise e
+                    try:
+                        self._handle_all_terminated()
+                    except TerminatedException:
+                        break
+                except TerminatedException as e:
+                    if not e._level:
+                        break
+                    else:
+                        raise e
+        finally:
+            tlogger.log(self.logging_level, "Ticker loop ended: {}".format(self.name))
+
+    def _remove_terminated(self):
+        open = self._tickers["open"]
+        len_tickers = len(open)
+        for i, ticker in enumerate(reversed(open)):
+            if ticker._closed:
+                del open[len_tickers - (i + 1)]
+                del self._timer[ticker]
+                if not self._inf["gc_closed"]:
+                    self._tickers["closed"].append(ticker)
+
+    def _handle_all_terminated(self):
+        at = self._inf["allterminated"]
+        if at == "raise":
+            raise AllTerminated("{} - all tickers are terminated.".format(self._name))
+        elif at == "close":
+            self.close()
+        else:
+            self.sleep("updated")
+
+    def _update_timer(self, ticker, update_supers=True):
+        try:
+            _next = ticker.get_time_remaining(as_float=False) + dt.utcnow()
+        except AllTerminated:
+            self._timer[ticker] = None
+        else:
+            self._timer[ticker] = _next
+
+        with self._hidden["lock"]:
+            self._hidden["updated"].set()
+
+        if update_supers:
+            self._update_supers()
+
+    def get_earliest(self):
+        vals = (x for x in self._timer.values() if x is not None)
+        try:
+            return min(vals)
+        except ValueError:
+            raise AllTerminated("{} - all tickers are terminated".format(self._name))
+
+    def get_time_remaining(self, as_float=True):
+        delta = self.get_earliest() - dt.utcnow()
+
+        if as_float:
+            return delta.total_seconds()
+        return delta
+
+
+class TickManager(TPMethods, BaseTickManager):
+    def close(self):
+        super().close()
+        if self._inf["close_subs"]:
+            for t in self._tickers["open"]:
+                t.close()
+        self._remove_terminated()
+
+
+class AsyncTickManager(AsyncBaseTicker, BaseTickManager):
+    def __init__(self, tickers, *, loop=None, allterminated="sleep", **kw):
+        """Asynchronous version of TickManager."""
+        super().__init__(None, loop=loop, allterminated=allterminated, **kw)
+
+        self._hidden["queue"] = FonsQueue(loop=self._inf["event_loop"])
+
+        if tickers is None:
+            tickers = []
+
+        for t in tickers:
+            self.add_ticker(t)
+
+    def add_ticker(self, ticker):
+        if not isinstance(ticker, AsyncBaseTicker):
+            raise TypeError(
+                "`ticker` must inherit from AsyncBaseTicker; got type: {}".format(
+                    type(ticker)
+                )
+            )
+        TickManager.add_ticker(self, ticker)
+        loop = self._inf["event_loop"]  # ticker._inf['event_loop']
+
+        async def put():
+            await self._hidden["queue"].put(ticker)
+            with self._hidden["lock"]:
+                self._hidden["updated"].set()
+
+        f = functools.partial(asyncio.ensure_future, put(), loop=loop)
+        loop.call_soon(f)
+
+    async def _get_free_ticker(self):
+        ticker = await self._hidden["queue"].get()
+
+        if isinstance(ticker, QuitException):
+            raise TerminatedException("{} is closed".format(self._name))
+
+        return ticker
+
+    async def _tick_and_release(self, ticker, *args, **kw):
+        try:
+            await ticker.tick(*args, **kw)
+        except TerminatedException as e:
+            # Note that .tick tries to remove any terminated tickers before calling ._tick_and_release, but sometimes
+            # due to delay the ticker may close *in the meanwhile*, and due to .tick_and_release being called through
+            # loop.call_soon() (not directly await .tick_and_release()), the exception shows up on the log
+            # That's why decided *not* to raise the TerminatedException here
+            """ "e._level += 1
+            raise e"""
+            return
+        else:
+            callback = self._inf["callback"]["target"]
+            if callback is None:
+                pass
+            elif self._inf["callback"]["isCoro"]:
+                await callback({"result": None, "ticker": self, "ts": dt.utcnow()})
+            else:
+                callback({"result": None, "ticker": self, "ts": dt.utcnow()})
+
+            # self._update_timer(ticker, False)
+        finally:
+            await self._hidden["queue"].put(ticker)
+
+    async def tick(self, errors=NotImplemented, update_supers=True):
+        while self._verify_is_open():
+            self._remove_terminated()
+
+            if not len(self._tickers["open"]):
+                await self._handle_all_terminated()
+
+            ticker = await self._get_free_ticker()
+            if ticker._closed:
+                continue
+
+            loop = self._inf["event_loop"]  # ticker._inf['event_loop']
+            coro = self._tick_and_release(
+                ticker, errors="sleep", update_supers=update_supers
+            )
+            f = functools.partial(asyncio.ensure_future, coro, loop=loop)
+            loop.call_soon(f)
+            break
+
+    async def loop(self, update_supers=True):
+        """cours = (ticker.loop() for ticker in self._tickers['open'])
+        await asyncio.gather(*cours, return_exceptions=True)"""
+        self._verify_is_open()
+        tlogger.log(self.logging_level, "Starting ticker loop: {}".format(self.name))
+        try:
+            while True:
+                try:
+                    await self.tick(update_supers=update_supers)
+                except TerminatedException as e:
+                    break
+                    """if not e._level: break
+                    else: raise e"""
+                    # e._level is always 0,
+                    # because ticker.tick() in self.tick() does not raise
+                """No AllTerminated is needed to be caught, 
+                   as it is already handled in the tick"""
+        finally:
+            tlogger.log(self.logging_level, "Ticker loop ended: {}".format(self.name))
+
+    async def _handle_all_terminated(self):
+        at = self._inf["allterminated"]
+        if at == "raise":
+            raise AllTerminated("{} - all tickers are terminated.".format(self._name))
+        elif at == "close":
+            await self.close()
+        else:
+            await self.sleep("updated")
+
+    async def sleep(self, time=None):
+        """This works but is not meant to be used with time=`None`,
+        as calling get_time_remaining() will fail if no tickers are left"""
+        await super().sleep(time)
+
+    async def close(self):
+        event = self._hidden["closed"]
+
+        if not event.is_set():
+            await self._hidden["queue"].put(QuitException())
+
+        await super().close()
+
+        if self._inf["close_subs"]:
+            for t in self._tickers["open"]:
+                if isinstance(t, AsyncBaseTicker):
+                    await t.close()
+                else:
+                    t.close()
+
+        self._remove_terminated()
+
+    _hidden = {"closed": None, "updated": None, "lock": None, "queue": None}
+
+
+class Routine:
+    def __init__(self, sched={}, tickmgr={}, *, name=None):
+        self._locks = {-1: asyncio.Lock()}
+        self._events = {}
+
+        # this contains instructions for creating various tickers,
+        # a dict *key* will later identify
+        # 1. its corresponding ticker in self._tickers ({key: resulting_ticker}),
+        # 2. its corresponding event in self._events
+        # a dict *value* will be used to create the ticker, and should be in the format
+        # {
+        # target:method_name_or_function,
+        # args:target_args,
+        # kwargs:target_kwargs,
+        # lock_id:None/<int>/<asyncio.Lock>
+        # no_set_event_on: if target returns this value, event will not be set
+        #  -- (NB! the comparison operator is `is` ("value is no_set_event_on"), therefore strings/ints/floats.. will not do)
+        #  --defaults to False
+        # ..all other arguments that can be passed to AsyncTicker.__init__
+        # }
+        # may be updated manually, calling self.sched.update({..}) in a subclass
+        if not isinstance(sched, dict):
+            raise TypeError(type(sched))
+        self.sched = sched.copy()
+
+        if name is None and hasattr(self.__class__, "_name"):
+            name = self.__class__._name
+        self._name = create_name(
+            name, default=self.__class__.__name__, registry=_ROUTINE_NAMES
+        )
+
+        tcm = tickmgr.copy()
+        if tcm.get("close_subs") is None:
+            tcm["close_subs"] = True
+        if "tickers" not in tcm:
+            tcm["tickers"] = []
+        if tcm.get("name") is None:
+            tcm["name"] = self.name + "-TickManager"
+
+        self._tickmgr = AsyncTickManager(**tcm)
+        self._tickers = {}
+
+    def create_schedule(self):
+        """Creates tickers out of .sched attribute.
+        May also be called while Routine is already running (.start has been called)"""
+
+        def wrap_callback(cb, event, **kw):
+            # NB! _accpets_args must be called before wrapping to corotine
+            # due to coroutine() replacing it with *args and **kw
+            cb_is_set = cb is not None
+            accepts_args = cb_is_set and _accepts_args(cb)
+            iscoro = cb_is_set and asyncio.iscoroutinefunction(cb)
+            """if not asyncio.iscoroutinefunction(cb):
+                cb = asyncio.coroutine(cb)"""
+
+            no_set_event_on = kw.get("no_set_event_on")
+            if no_set_event_on is None:
+                pass
+            elif not hasattr(no_set_event_on, "__call__"):
+                raise TypeError(
+                    '`no_set_event_on` must be None or have attr "__call__"; got: {}'.format(
+                        no_set_event_on
+                    )
+                )
+
+            async def set_event(*args):
+                # ticker @callback passes {'result': , 'ticker': ,'ts': }
+                # print(cb_is_set,set_event_on,args[0]['result'],set_event_on(args[0]['result']))
+                if no_set_event_on is None or not no_set_event_on(args[0]["result"]):
+                    event.set()
+                if not cb_is_set:
+                    pass
+                elif accepts_args:
+                    if not iscoro:
+                        cb(*args)
+                    else:
+                        await cb(*args)
+                else:
+                    if not iscoro:
+                        cb()
+                    else:
+                        await cb()
+
+            return set_event
+
+        logger.debug("{} - creating schedule".format(self.name))
+        max_lock_id = max(self._locks)
+        for n, params in self.sched.items():
+            # Only new schedule items will be added
+            # If want remove from schedule, call .remove(name)
+            if n in self._tickers:
+                continue
+            lock_id = params.get("lock_id")
+            if isinstance(lock_id, asyncio.Lock):
+                try:
+                    lock_id = next(x for x, y in self._locks.items() if lock_id is y)
+                except StopIteration:
+                    max_lock_id = max_lock_id + 1
+                    self._locks[max_lock_id] = lock_id
+                    lock_id = max_lock_id
+            elif lock_id is None:
+                lock_id = max_lock_id = max_lock_id + 1
+
+            if not isinstance(lock_id, int):
+                raise TypeError(type(lock_id))
+            elif lock_id not in self._locks:
+                max_lock_id = max(max_lock_id, lock_id)
+                self._locks[lock_id] = asyncio.Lock()
+
+            targkw = [params.get(p) for p in ("target", "args", "kwargs")]
+            rout_kw = {"lock_id": lock_id}
+            tickConfig = {
+                x: y
+                for x, y in params.items()
+                if x not in ("target", "args", "kwargs", "lock_id", "no_set_event_on")
+            }
+
+            self._events[n] = event = FonsEvent()
+
+            cb = tickConfig.get("callback")
+            nseo = {x: y for x, y in params.items() if x == "no_set_event_on"}
+            tickConfig["callback"] = wrap_callback(cb, event, **nseo)
+            if tickConfig.get("name") is None:
+                tickConfig["name"] = "{}-{}-Ticker".format(self.name, n)
+
+            ticker = AsyncTicker(
+                self._routine, args=targkw, kwargs=rout_kw, **tickConfig
+            )
+            self._tickmgr.add_ticker(ticker)
+            self._tickers[n] = ticker
+
+    async def start(self):
+        self._tickmgr._verify_is_open()
+        self.create_schedule()
+        logger.debug("Starting routine {}".format(self.name))
+        try:
+            await self._tickmgr.loop()
+        finally:
+            tlogger.debug("Routine ended: {}".format(self.name))
+
+    async def _routine(self, target, args, kwargs, lock_id):
+        if args is None:
+            args = tuple()
+        if kwargs is None:
+            kwargs = {}
+        method = getattr(self, target) if isinstance(target, str) else target
+
+        lock = self._locks[lock_id]
+
+        async with lock:
+            if asyncio.iscoroutinefunction(method):
+                return await method(*args, **kwargs)
+            else:
+                return method(*args, **kwargs)
+
+    async def remove(self, name, from_sched=True):
+        lock_id = self.get_lock_id(name)
+        await self.get_ticker(name).close()
+        del self._tickers[name]
+        del self._events[name]
+        if lock_id != -1 and not any(
+            self.get_lock_id(n) == lock_id for n in self._tickers
+        ):
+            del self._locks[lock_id]
+        if from_sched and name in self.sched:
+            del self.sched[name]
+        # Note that removing all tickers will not cause the running tickmgr to stop,
+        # unless .__init__(..,tickmgr={'allterminated':'close'}) was passed
+
+    async def close(self):
+        await self._tickmgr.close()
+
+    def get_ticker(self, name):
+        return self._tickers[name]
+
+    def get_event(self, name):
+        return self._events[name]
+
+    def get_lock(self, id):
+        if isinstance(id, str):
+            id = self.get_lock_id(id)
+        elif not isinstance(id, int):
+            raise TypeError(type(id))
+        return self._locks[id]
+
+    def get_lock_id(self, name):
+        return self.get_ticker(name)._inf["target"]["kwargs"]["lock_id"]
+
+    @property
+    def name(self):
+        return self._name
+
+    @name.setter
+    def name(self, value):
+        self._name = value
```

### Comparing `fons-0.3.1/fons/threads.py` & `fons-0.4.0/fons/threads.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,156 +1,190 @@
-import datetime
-dt = datetime.datetime
-td = datetime.timedelta
-import time
-import threading
-import asyncio
-
-import fons.debug as debug
-from fons.errors import ThreadEndException
-#from fons.reg import create_name
-
-_THREAD_NAMES = set()
-
-
-class Eli(type):
-    def __new__(cls, name, bases, attrs):
-        def wrap_run(f):
-            def set_event_loop(self):
-                loop = getattr(self,'_loop',None)
-                if loop is None: self._loop = loop = asyncio.new_event_loop()
-                asyncio.set_event_loop(loop)
-                return f(self)
-            return set_event_loop
-        
-        if not any(issubclass(x,threading.Thread) for x in bases):
-            raise TypeError("class '{}' must be a subclass of 'threading.Thread'".format(name))
-          
-        if 'run' in attrs:
-            attrs['run'] = wrap_run(attrs['run'])
-        elif not any(issubclass(type(x),Eli) for x in bases):
-            attrs['run'] = wrap_run(threading.Thread.run)
-            
-        return super(Eli, cls).__new__(cls, name, bases, attrs)
-    
-    
-class EliThread(threading.Thread, metaclass=Eli):
-    """Sets up event loop in the resulting thread. Integrates trylog."""
-    def __init__(self, group=None, target=None, name=None, args=None, kwargs=None, *,
-                 loop=None, trylog=True, keepalive=False, daemon=None):
-        if args is None: args = ()
-        if kwargs is None: kwargs = {}
-        self._loop = loop if loop is not None else asyncio.new_event_loop()
-        self._keepalive = bool(isinstance(keepalive,dict) or keepalive)
-        self._trylog =  bool(isinstance(trylog,dict) or trylog)
-        if not isinstance(trylog,dict): trylog = {}
-        if not isinstance(keepalive,dict): keepalive = {}
-        self._trylog_params = dict({'attempts':True},**keepalive) if self._keepalive else trylog
-        
-        if self._keepalive or self._trylog:
-            args = (target,args,kwargs)
-            kwargs = self._trylog_params
-            target = debug.trylog
-        #print('group: {}, target:{}, daemon: {}'.format(group,target,daemon))
-        super().__init__(group, target, name, args, kwargs, daemon=daemon)
-
-
-#-------------------------------
-
-class LoopingThread(EliThread):
-    def __init__(self, id, name, delay=None, absolute_delay=True, *, loop=None):
-        super().__init__(loop=loop)
-        self.id = id
-        self.name = name
-        
-        if delay is not None:
-            self._delay = {'period': delay, 'absolute': absolute_delay}
-        else: self._delay = {'period': 0, 'absolute': absolute_delay}
-        
-        self._times = dict.fromkeys(['start','next','end'])
-
-    
-    def __init2__(self,_MyThread=[],**kw):
-        values = []
-        names = ['id','name','delay','absolute_delay']
-        
-        args_missed = 0
-        
-        for i,n in enumerate(names):
-            if kw.get(n) is not None:
-                values.append(kw.get(n))
-                args_missed += 1
-                del kw[n]
-            elif 0 <= i-args_missed < len(_MyThread) and _MyThread[i-args_missed] is not None:
-                values.append(_MyThread[i-args_missed])
-            else: values.append(self._base_values[i])
-        
-        LoopingThread.__init__(self,*values,**kw)
-        
-        
-    def startinfo(self):
-        print("Starting " + self.name)
-        ts = dt.utcnow()
-        
-        if self._times['start'] is None:
-            self._times['start'] = ts
-    
-    #In case of relative delay, updates the time before which the next cycle is not allowed to start
-    def update(self):
-        if not self._delay['absolute']:
-            ts = dt.utcnow()
-            self._times['next'] = ts + self._delay['period']
-            
-    def do_this(self):
-        pass
-    
-    def delay(self):
-        ts = dt.utcnow()
-        
-        if not self._delay['absolute']:
-            remaining = ts - self._times['next']
-            
-            if remaining > td(0):
-                time.sleep(remaining)
-                
-        elif self._delay['period']:
-            time.sleep(self._delay['period'])
-    
-    
-    def run(self):
-        self._set_event_loop()
-        self.startinfo()
-
-        while True:
-            self.update()
-            try:
-                self.do_this()
-            except ThreadEndException:
-                self._shutdown = True
-                
-            if self._shutdown:
-                return
-            self.delay()
-
-            
-    _base_values = [1,"LoopingThread",None,True]
-    _shutdown = False
-            
-
-
-if __name__ == '__main__':
-    class A(threading.Thread, metaclass=Eli): pass
-    class B(A): pass
-    print(A.run,type(A))
-    print(B.run,type(B))
-
-    class T(EliThread):
-        def run(self):
-            print('get_loop: {}, loop: {}'.format(id(asyncio.get_event_loop()),id(self._loop)))
-    t = T(loop=asyncio.new_event_loop())
-    t.start()
-    
-    l = asyncio.get_event_loop()
-    print(id(l))
-    t2 = EliThread(target=lambda: print(id(asyncio.get_event_loop())), loop=l)
-    t2.start()
-    
+import datetime
+
+dt = datetime.datetime
+td = datetime.timedelta
+import time
+import threading
+import asyncio
+
+import fons.debug as debug
+from fons.errors import ThreadEndException
+
+# from fons.reg import create_name
+
+_THREAD_NAMES = set()
+
+
+class Eli(type):
+    def __new__(cls, name, bases, attrs):
+        def wrap_run(f):
+            def set_event_loop(self):
+                loop = getattr(self, "_loop", None)
+                if loop is None:
+                    self._loop = loop = asyncio.new_event_loop()
+                asyncio.set_event_loop(loop)
+                return f(self)
+
+            return set_event_loop
+
+        if not any(issubclass(x, threading.Thread) for x in bases):
+            raise TypeError(
+                "class '{}' must be a subclass of 'threading.Thread'".format(name)
+            )
+
+        if "run" in attrs:
+            attrs["run"] = wrap_run(attrs["run"])
+        elif not any(issubclass(type(x), Eli) for x in bases):
+            attrs["run"] = wrap_run(threading.Thread.run)
+
+        return super(Eli, cls).__new__(cls, name, bases, attrs)
+
+
+class EliThread(threading.Thread, metaclass=Eli):
+    """Sets up event loop in the resulting thread. Integrates trylog."""
+
+    def __init__(
+        self,
+        group=None,
+        target=None,
+        name=None,
+        args=None,
+        kwargs=None,
+        *,
+        loop=None,
+        trylog=True,
+        keepalive=False,
+        daemon=None
+    ):
+        if args is None:
+            args = ()
+        if kwargs is None:
+            kwargs = {}
+        self._loop = loop if loop is not None else asyncio.new_event_loop()
+        self._keepalive = bool(isinstance(keepalive, dict) or keepalive)
+        self._trylog = bool(isinstance(trylog, dict) or trylog)
+        if not isinstance(trylog, dict):
+            trylog = {}
+        if not isinstance(keepalive, dict):
+            keepalive = {}
+        self._trylog_params = (
+            dict({"attempts": True}, **keepalive) if self._keepalive else trylog
+        )
+
+        if self._keepalive or self._trylog:
+            args = (target, args, kwargs)
+            kwargs = self._trylog_params
+            target = debug.trylog
+        # print('group: {}, target:{}, daemon: {}'.format(group,target,daemon))
+        super().__init__(group, target, name, args, kwargs, daemon=daemon)
+
+
+# -------------------------------
+
+
+class LoopingThread(EliThread):
+    def __init__(self, id, name, delay=None, absolute_delay=True, *, loop=None):
+        super().__init__(loop=loop)
+        self.id = id
+        self.name = name
+
+        if delay is not None:
+            self._delay = {"period": delay, "absolute": absolute_delay}
+        else:
+            self._delay = {"period": 0, "absolute": absolute_delay}
+
+        self._times = dict.fromkeys(["start", "next", "end"])
+
+    def __init2__(self, _MyThread=[], **kw):
+        values = []
+        names = ["id", "name", "delay", "absolute_delay"]
+
+        args_missed = 0
+
+        for i, n in enumerate(names):
+            if kw.get(n) is not None:
+                values.append(kw.get(n))
+                args_missed += 1
+                del kw[n]
+            elif (
+                0 <= i - args_missed < len(_MyThread)
+                and _MyThread[i - args_missed] is not None
+            ):
+                values.append(_MyThread[i - args_missed])
+            else:
+                values.append(self._base_values[i])
+
+        LoopingThread.__init__(self, *values, **kw)
+
+    def startinfo(self):
+        print("Starting " + self.name)
+        ts = dt.utcnow()
+
+        if self._times["start"] is None:
+            self._times["start"] = ts
+
+    # In case of relative delay, updates the time before which the next cycle is not allowed to start
+    def update(self):
+        if not self._delay["absolute"]:
+            ts = dt.utcnow()
+            self._times["next"] = ts + self._delay["period"]
+
+    def do_this(self):
+        pass
+
+    def delay(self):
+        ts = dt.utcnow()
+
+        if not self._delay["absolute"]:
+            remaining = ts - self._times["next"]
+
+            if remaining > td(0):
+                time.sleep(remaining)
+
+        elif self._delay["period"]:
+            time.sleep(self._delay["period"])
+
+    def run(self):
+        self._set_event_loop()
+        self.startinfo()
+
+        while True:
+            self.update()
+            try:
+                self.do_this()
+            except ThreadEndException:
+                self._shutdown = True
+
+            if self._shutdown:
+                return
+            self.delay()
+
+    _base_values = [1, "LoopingThread", None, True]
+    _shutdown = False
+
+
+if __name__ == "__main__":
+
+    class A(threading.Thread, metaclass=Eli):
+        pass
+
+    class B(A):
+        pass
+
+    print(A.run, type(A))
+    print(B.run, type(B))
+
+    class T(EliThread):
+        def run(self):
+            print(
+                "get_loop: {}, loop: {}".format(
+                    id(asyncio.get_event_loop()), id(self._loop)
+                )
+            )
+
+    t = T(loop=asyncio.new_event_loop())
+    t.start()
+
+    l = asyncio.get_event_loop()
+    print(id(l))
+    t2 = EliThread(target=lambda: print(id(asyncio.get_event_loop())), loop=l)
+    t2.start()
```

### Comparing `fons-0.3.1/fons/verify.py` & `fons-0.4.0/fons/verify.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,1929 +1,1929 @@
-from collections import OrderedDict as OD
-import pandas as pd
-import numpy as np
-import datetime as dt
-from dateutil.parser import parse as parsedate
-import traceback
-import warnings
-import logging
-
-from fons.errors import (BadInstruction, VeriError, VeriTypeError, 
-                         VeriValueError, VeriKeyError, VeriIndexError)
-
-from fons.dict_ops import deep_update
-from fons.iter import (flatten, unique)
-from fons.pyops import (compare, copy as _copy)
-from fons.nan import (nan, Implemented) 
-
-#is_given: nan is NOT implemented
-is_given = Implemented()
-#is_not_null : nan, None and '_nan_' are NOT implemented
-is_not_null = Implemented([None,'_nan_'])
-is_null = lambda x: not is_not_null(x)
-
-
-_EXCEPTIONS = {'type': VeriTypeError,
-               'value': VeriValueError,
-               'key': VeriKeyError,
-               'index': VeriIndexError,
-               'general': VeriError,}
-
-_EXC_MAP = {VeriTypeError: TypeError,
-            VeriValueError: ValueError,
-            VeriKeyError: KeyError,
-            VeriIndexError: IndexError,}
-
-
-_EXC_ORD = [VeriError, VeriTypeError, VeriValueError, VeriKeyError, VeriIndexError]
-
-
-mappings  =  [[['pd.DataFrame','pandas.DataFrame','pandas.core.frame.DataFrame'],pd.DataFrame],
-              [['pd.Series','pandas.Series','pandas.core.series.Series'],pd.Series],
-              [['list'],list],
-              [['tuple'],tuple],
-              [['dict','dictionary'],dict],
-              [['OrderedDict'],OD],
-              [['set'],set],
-              [['string','str'],str],
-              [['int','int8','int16','int32','int64','integer'],int],
-              [['float','float16','float32','float64'],float],
-              [['np.ndarray','numpy.ndarray'],np.array],
-              [['np.ndarray','numpy.ndarray'],np.array],
-              [['dt.date','datetime.date','date'],dt.date],
-              [['dt','dt.datetime','datetime.datetime','datetime','datetime64[ns]'],dt.datetime],
-              [['td','dt.timedelta','datetime.timedelta','timedelta','timedelta64[ns]'],dt.timedelta],
-              [['object'],str],
-              [['type'],type],
-              [['listlike'],(list,tuple,np.ndarray,pd.Index)],
-              [['dictlike'],(dict,OD)]]
-
-
-MAP = {}
-for strnames,func in mappings:
-    MAP.update(dict.fromkeys(strnames, func))
-    MAP.update({func: func})
-    
-    
-EQUALS = {np.datetime64: pd.Timestamp,
-          dt.datetime: pd.Timestamp,
-          np.timedelta64: pd.Timedelta,
-          dt.timedelta: pd.Timedelta,
-          int: np.int32,
-          #type(None): pd._libs.tslib.NaTType,
-          float: (np.float64, int, np.int32),}
-
-#For checking random objs agains pandas objs
-PD_EQUALS = {np.datetime64: pd.Timestamp,
-             dt.datetime: pd.Timestamp,
-             np.timedelta64: pd.Timedelta,
-             dt.timedelta: pd.Timedelta,
-             int: float}
-
-"""for k,v in list(EQUALS.items()):
-    EQUALS[v] = k"""
-    
-PD_STRING = {dt.datetime: 'datetime64[ns]',
-             np.datetime64: 'datetime64[ns]',
-             pd.Timestamp: 'datetime64[ns]',
-             dt.timedelta: 'timedelta64[ns]',
-             np.timedelta64: 'timedelta64[ns]',
-             pd.Timedelta: 'timedelta64[ns]',}
-
-
-
-TYPES = ('type','function','module')
-_TYPES = tuple([cls for cls in object.__subclasses__() if cls.__name__ in TYPES])
-
-DEFAULT_ARGUMENTS = {dt.date: [(0,0,0),{}],
-                     dt.datetime: [(0,0,0),{}],
-                     dt.timedelta: [(0,),{}]}
-
-DO_NOT_CALL_BY_DEFAULT = (dt.date, dt.datetime, dt.timedelta)
-
-#may contain dicts of instructions; later are packed into list([inited])/tuple([inited])
-#if e.g np.ndarray is preferred, must use {'_type_': np.ndarray, '_call_': np.asarray, 'value'/'_value_': [..instructions..], _kw={'dtype': x}} instead
-HANDLEABLES = (list, tuple, set) #?? does `set` belong here?
-
-IMMUTABLES = (int, float, str, bool, tuple, type(None))
-CONTAINERS = (dict, list, tuple, set, pd.Series, pd.DataFrame, pd.Index, np.ndarray)
-COPY_METHOD = (pd.DataFrame, pd.Series, pd.DatetimeIndex, pd.Index, np.ndarray)
-
-
-RESERVED = ('_type_', '_call_', '_value_', '_multival_', '_defval_', '_copy_', '_isnorm_', '_multi_', '_vfy_')
-NORM_EXTRA = {'_type_':str,
-              '_value_': '_keep_'}
-
-
-def _map(item, *default, **kw):
-    if not isinstance(item, str):
-        if kw.get('pd_dtype'):
-            return _map_pd_dtype(item)
-        return item
-    
-    obj = None
-    
-    if item in MAP:
-        obj = MAP[item]
-    elif __name__ == '__main__':
-        obj = getattr(__builtins__, item, None)
-    else:
-        obj = __builtins__.get(item, None)
-    
-    obj_t = (obj,) if not isinstance(obj, tuple) else obj
-    
-    if any(x is None or type(x).__name__ not in TYPES for x in obj_t):
-        if not len(default):
-            raise BadInstruction('Item {} not known.'.format(item))
-        else:
-            return default[0]
-    
-    if kw.get('pd_dtype'):
-        obj = _map_pd_dtype(obj)
-    
-    #if isinstance(obj,str) and obj != 'datetime64[ns]': raise OSError(obj)
-    
-    return obj
-
-
-def _map_pd_dtype(obj):
-    try:
-        obj = PD_STRING.get(obj, obj)
-    except TypeError:
-        pass
-    return obj
-
-
-def _isinstructions(x):
-    if isinstance(x, Element):
-        return True
-    elif not isinstance(x, dict):
-        return False
-    elif not any(k in RESERVED for k in x.keys()):
-        return False
-    
-    return True 
-
-
-def _isnorm(x):
-    if isinstance(x, dict):
-        return bool(x.get('_isnorm_'))
-    elif isinstance(x, Element):
-        return bool(getattr(x, 'isnorm', False))
-    
-    return False
-
-#---------------------
-
-def normalize(data):
-    init_data(data)
-    normalized = normalize_element(data)
-    
-    return normalized
-
-
-def fill(x, norm, **kw):
-    return verify_data(x,norm,mode='fill',**kw)
-
-#----------------------------------------
-
-def init_data(x, copy=True):
-    obj = None
-    _type = type(x)
-    _name = _type.__name__
-    
-    if issubclass(_type, Element):
-        x = x.to_dict()
-        _type = dict
-    
-    if issubclass(_type, dict):
-        obj = _init_from_dict(x)
-        if copy: obj = _copy(obj)
-    
-    elif _type not in HANDLEABLES:
-        if copy: obj = _copy(x)
-        else: obj = x
-
-    else:
-        #isinstr = any(_isintruction(y) for y in x)
-        #may still contain instructions at a sub-level
-        alist = [init_data(y, copy=copy) for y in x]
-      
-        try:
-            call = _map(_name)
-            obj = call(alist)
-                
-        except ValueError:
-            obj = alist
-            
-        except Exception:
-            traceback.print_exc()
-            obj = alist
-        
-    return obj
-
-
-
-def _init_from_dict(D, copy=True):
-    add_to = {}
-    if _isinstructions(D):
-        return _init_instructions(D, copy=copy)
-    
-    #initiating its values (plus making copy of the dict)
-    for n,v in D.items():
-        obj = init_data(v, copy=copy)
-        add_to[n] = obj
-        #keys are always? immutable, no need to copy
-    
-    return add_to 
-
-
-
-def _init_instructions(D, copy=True):
-    normalize_element(D)
-    
-    if '_copy_' in D:
-        if copy:
-            return _copy(D['_copy_'])
-        else:
-            return D['_copy_']
-    
-    _type_ = D.get('_type_')
-    
-    if isinstance(_type_, tuple):
-        _type0_ = _type_[0]
-    else:
-        _type0_ = _type_
-    
-    
-    if '_defval_' in D:
-        return init_data(D['_defval_'], copy=copy)
-    
-    elif '_multi_' in D:
-        return init_data(D['_multi_'][0], copy=copy)
-    
-    elif _type0_ in _TYPES:
-        #return _map(D.get('_value_'))
-        return D.get('_value_')
-    
-    elif '_value_' in D:
-        D['_copy_'] = _copy(D['_value_'])
-        return _init_instructions(D, copy=copy)
-    
-    elif '_multival_' in D:
-        D['_copy_'] = _copy(D['_multival_'][0])
-        return _init_instructions(D, copy=copy)
-    
-    
-    return _init_by_call(_type0_, D, copy=copy)
-    
-
-
-def _init_by_call(_type_, D, copy=True):
-    
-    _call0_ = D.get('_call_',nan)
-
-    if is_given(_call0_):
-        if is_null(_call0_):
-            return nan
-            #raise BadInstruction('Wrong _call_: {}'.format(_call0_))
-    elif is_null(_type_):
-        #return nan
-        raise BadInstruction('_type_ is null')
-    
-
-    #_value_ is used for not using _call_() or _type_() 
-    
-    args,kw,_call2_ = [],{},_type_
-    
-    """if is_null(D.get('args')) and is_null(D.get('kwargs')) and \
-            _type_ in DO_NOT_CALL_BY_DEFAULT:
-        return nan"""
-        
-    
-    if isinstance(D.get('args'),(list,tuple)):
-        args = init_data(D['args'])
-    
-    if isinstance(D.get('kwargs'),dict):
-        kw = init_data(D['kwargs'])
-    
-
-    if is_given(_type_) and (not len(args) or not len(kw)): #??
-        args2,kw2,_call2_ = _known_types(_type_, D, copy=copy)
-        if not len(args):
-            args = args2
-        kw2.update(kw)
-        kw = kw2
-
-
-    if is_given(_call0_): 
-        _call_ = _call0_
-    else: 
-        _call_ = _call2_
-            
-    #print(_type.__name__,'args:',args,'kw:',kw)
-    obj = _call_(*args,**kw)
-    
-    
-    D['_copy_'] = _copy(obj)
-
-    return obj
-
-
-
-def _known_types(_type_, D, copy=True):
-    
-    #vname = vtype.__name__
-    args = []
-    kw = {}
-    call = _type_
-    
-    
-    if issubclass(_type_, (pd.Series, pd.DataFrame)):
-        data = init_data(D.get('data'),copy=False)
-        index = init_data(D.get('index'),copy=False)
-        dtype = MAP.get(D.get('dtype'))
-        
-        name = init_data(D.get('name'),copy=False)
-        columns = init_data(D.get('columns'),copy=False)
-        dtypes = D.get('dtypes')
-        
-        if _type_ is pd.DataFrame:
-            if dtypes:
-                if not isinstance(data,dict):
-                    data = OD([[c,pd.Series(data, index=index, dtype=_map(d,None,pd_dtype=True))] for c,d in D['dtypes'].items()])
-                else:
-                    data = OD([[c,pd.Series(data.get(c), index=index, dtype=_map(d,None,pd_dtype=True))] for c,d in D['dtypes'].items()])
-            
-                if not columns:
-                    D['columns'] = list(dtypes.keys())
-            
-            kw.update({'data':data,'index':index,'columns':columns,'dtype':dtype})
-        
-        else:
-            kw.update({'data':data,'index':index,'name':name,'dtype':dtype})
-    
-    
-    elif issubclass(_type_, dict):
-        new_d = {}
-        items = []
-        
-        if is_not_null(D.get('items', nan)):
-            items = D['items']
-            if isinstance(items,dict):
-                items = list(items.items())
-        
-        elif is_not_null(D.get('keys', nan)):
-            keys = D['keys']
-            if 'values' in D:
-                values = D['values']
-            elif 'value' in D or 'v' in D:
-                values = [D.get('value',D.get('v'))] * len(keys)
-            else:
-                values = [D.get('unit')] * len(keys)
-            
-            items = list(zip(keys,values))
-        
-        new_d = init_data(items, copy=copy)
-        args.append(new_d)
-        
-        if True:
-            D['keys'] = [itm[0] for itm in new_d]
-            #For being able to verify_data later (itm[1] -> {'_type_':type(itm[1]),_value_: itm[1])}
-            items = [[itm[0],normalize_element(itm[1])] for itm in items]
-            D['items'] = items #the instr dicts in items have been normalized due to init_data(items)
-            init_data(D.get('unit'), copy=False) #??
-    
-    
-    elif issubclass(_type_, dt.datetime):
-        value = D.get('value', D.get('v'))
-        
-        if isinstance(value,str):
-            args.append(value)
-            
-            if D.get('format'):
-                call = dt.datetime.strptime
-                args.append(D['format'])
-            else:
-                call = parsedate
-        
-        elif isinstance(value, dt.datetime):
-            args.extend([value.year, value.month, value.day, value.hour,
-                         value.minute, value.second, value.microsecond])
-        
-        elif isinstance(value,(list,tuple)):
-            args.extend(value)
-        
-        elif isinstance(value,(int,float)):
-            call = dt.datetime.utcfromtimestamp
-            args.append(value/1000)
-        
-        else:
-            raise BadInstruction(_type_, D, value)
-    
-    
-    elif issubclass(_type_, dt.timedelta):
-        value = D.get('value', D.get('v'))
-        
-        if isinstance(value,(list,tuple)):
-            args.extend(value)
-            
-        elif isinstance(value,(int,float)):
-            #microseconds
-            args.extend([0,0,value*1000])
-            
-        else:
-            raise BadInstruction(_type_, D, value)  
-    
-    
-    elif issubclass(_type_, (list,tuple,set)):
-        value = D.get('value', D.get('values', D.get('v', nan)))
-        _range = D.get('range', nan)
-        size = D.get('size', nan)
-        
-        if is_not_null(value):
-            args.append(init_data(value, copy=copy))
-            """if is_null(size):
-                D['size'] = {'==': (len(value),)}"""
-        
-        elif is_not_null(_range) and not isinstance(_range, str):
-            arange = list(range(*_range)) #np.arange(*range)
-            args.append(arange)
-            """if not is_not_null(size):
-                D['size'] = {'==': (len(arange),)}"""
-            
-            if not is_given(value):
-                D['value'] = arange
-            
-            init_data(D.get('unit'), copy=False) #??
-    
-    
-    elif issubclass(_type_, (str,int,float)):
-        value = D.get('value', D.get('v'))
-        if is_not_null(value):
-            args.append(init_data(value))
-            D['_value_'] = args[-1]
-            #del D['value']
-        elif issubclass(_type_, (int, float)) and isinstance(D.get('range'), str):
-            limit0, limit1 = D['_range']
-            if None not in D['_range']:
-                args.append((limit0 + limit1) / 2)
-            elif limit0 is not None:
-                args.append(limit0)
-            elif limit1 is not None:
-                args.append(limit1)
-    
-    else: 
-        pass #args.append(init_data(_type_))
-    
-    #print('args_now:',args)    
-    
-    return args, kw, call
-
-
-
-#--------------------------------------------
-
-def normalize_element(x, default=nan):
-    if _isnorm(x): return x
-    
-    #the corresponding keys' values are treated as literal (if they are present in the x):
-    # _defval_, _value_, value, unit, 
-    #_call_  :: return _value_/_multival,_defval_ if those present; 
-    #            otherwise if _call_ in (None, _nan_ ): return None, else _call_(args), 
-    #                and if not given _call_ = _type_. or return None if not is_not_null(_type_)
-    
-    x_initial = x
-    is_element = isinstance(x, Element)
-    if is_element:
-        x = x.to_dict()
-    
-    if _isinstructions(x):
-        d = x
-        _normalize_type(d)
-    else:
-        d = {'_type_': type(x),
-             '_value_': x}
-        
-    _normalize_defval(d, default)
-    
-    _normalize_multi(d)
-    
-    _normalize_value(d)
-
-    _normalize_call(d)
-        
-    _normalize_size(d)
-    _normalize_range(d)
-    
-    _normalize_unit(d)
-    
-    _normalize_dtypes(d)
-    _normalize_opt_req(d)
-    
-    _normalize_vfy(d)
-    
-    _type_ = d.get('_type_',nan)
-    if is_given(_type_):
-        if isinstance(_type_, tuple):
-            _type_ = _type_[0]
-        
-        if not issubclass(_type_, (dt.datetime, dt.timedelta)):
-            _known_types(_type_, d, copy=False)
-    
-    d['_isnorm_'] = True
-    
-    if is_element:
-        x_initial.update(d, normalize=False)
-        return x_initial
-    
-    return d
-
-
-def _normalize_type(d):
-    _type_ = d.get('_type_')
-        
-    if is_null(_type_):
-        d.pop('_type_',-1)
-        return
-            
-    if isinstance(_type_, MAP['listlike']):
-        _type_ = tuple((_map(t) for t in _type_))
-    else:
-        _type_ = _map(_type_)
-    
-    if isinstance(_type_, tuple):
-        for t in _type_:
-            _verify_is_type(t)
-    else:
-        _verify_is_type(_type_)
-    
-    d['_type_'] = _type_
-
-
-def _normalize_defval(d, default):
-    if default is not nan:
-        d['_defval_'] = normalize_element(default)
-    elif '_defval_' in d:
-        d['_defval_'] = normalize_element(d['_defval_'])
-
-
-def _normalize_multi(d):
-    _multi_ = d.get('_multi_',nan)
-    if is_null(_multi_): 
-        d.pop('_multi_', -1)
-    elif isinstance(_multi_, MAP['listlike']):
-        if len(_multi_):
-            _multi_ = list(_multi_)
-            for i,d2 in enumerate(_multi_):
-                _multi_[i] = normalize_element(d2)
-                init_data(_multi_[i], copy=False)
-        else:
-            del d['_multi_']
-    else:
-        raise BadInstruction('Defective "_multi_": {}'.format(_multi_))
-
-
-def _normalize_value(d):
-    if _isinstructions(d.get('_value_')):
-        d['_value_'] = init_data(d['_value_'], copy=False)
-    
-    has_type_key = '_type_' in d
-    _type_ = d.get('_type_')
-    
-    add_types = []
-    sub_allowed = d.get('sub', d.get('sub_allowed')) is not False
-    
-    #Value can be anything but fons.nan.nan
-    if '_value_' in d and not is_given(d['_value_']):
-        d.pop('_value_',-1)
-    
-    _value_ = d.get('_value_')
-    
-    if '_value_' in d:
-        if is_not_null(_value_) and has_type_key:
-            d['_value_'] = _map_value_if_str(_type_, _value_)
-            
-        add_types.append(type(d['_value_']))
-        
-        
-    _multival_ = d.get('_multival_',nan)
-    if is_null(_multival_):
-        d.pop('_multival_',-1)
-    elif isinstance(_multival_, MAP['listlike']):
-        if len(_multival_):
-            inited = [init_data(v, copy=False) for v in _multival_]
-            multival = [_map_value_if_str(_type_, v) 
-                            if has_type_key and is_not_null(v) else 
-                        v for v in inited]
-            add_types += [type(x) for x in multival]
-            if '_value_' in d:
-                multival.insert(d['_value_'], 0)
-                del d['_value_']
-            d['_multival_'] = multival
-        else:
-            del d['_multival_']
-    else:
-        raise BadInstruction('Defective "_multival_": {}'.format(_multival_))
-    
-    
-    if add_types:
-        types = ((_type_,) if not isinstance(_type_, tuple) else _type_)  if has_type_key else ()
-        for x in add_types:
-            if not types : pass
-            elif sub_allowed and not issubclass(x, types): pass
-            elif not sub_allowed and x not in types: pass
-            else: continue
-            types += (x,)
-        
-        if types:
-            d['_type_'] = types if len(types) > 1 else types[0]
-
-
-def _map_value_if_str(_type_, _value_):
-    if is_null(_type_):
-        return _value_
-    #to map e.g {'_type_: type, '_value_': 'list'} to {'_value_': list} 
-    # for (normalized) init and compare purposes
-    t_types = _type_ if isinstance(_type_,tuple) else (_type_,)
-    if isinstance(_value_, str) and not any(issubclass(t,str) for t in t_types):
-        return _map(_value_)
-    else:
-        return _value_
-
-
-def _normalize_call(d):
-    if '_call_' not in d: pass
-    elif is_not_null(d['_call_']): #??
-        d['_call_'] = _map(d['_call_'])
-
-
-def _normalize_size(d):
-    size = _size = d.get('size', nan)
-    if is_null(size):
-        d.pop('size', -1)
-    elif not isinstance(size, (int, dict, str)):
-        raise BadInstruction('"size" must be int/dict/str; got: {}'.format(type(size)))
-    elif isinstance(size, int):
-        d['size'] = {'exact': size}
-    elif isinstance(size, str):
-        _range = _parse_str_range(size, num_type=int)
-        _min = max(0, _range[0] if size.startswith('[') else _range[0]+1) if _range[0] is not None else None
-        _max = max(0, _range[1] if size.endswith(']') else _range[1]-1) if _range[1] is not None else None
-        d['size'] = {'min': _min, 'max': _max}
-    
-    size = d.get('size', nan)
-    if is_not_null(size):
-        for k in ('min','max','exact'):
-            value = size.get(k)
-            if is_null(value):
-                size.pop(k, -1)
-            elif not isinstance(value, int):
-                raise BadInstruction('"size" keyword "{}" must be of type <int>; got: {}; size: {}'.format(k, type(value), _size))
-            elif value < 0:
-                raise BadInstruction('"size" keyword "{}" must be >= 0; got: {}; size: {}'.format(k, value, _size))
-        _min, _max, _exact = size.get('min'), size.get('max'), size.get('exact')
-        if _min is not None and _max is not None and _min > _max:
-            raise BadInstruction('"size" keyword "min" < "max" is not satisfied; size: {}'.format(_size))
-        if _min is not None and _exact is not None:
-            raise BadInstruction('"size" must not have both "min" and "exact" keywords; size: {}'.format(_size))
-        if _max is not None and _exact is not None:
-            raise BadInstruction('"size" must not have both "max" and "exact" keywords; size: {}'.format(_size))
-
-
-def _parse_number(x, num_type=float):
-    if not x or x=='null':
-        return None
-    try: 
-        return num_type(x)
-    except ValueError:
-        return '?'
-
-
-def _parse_str_range(range, num_type=float):
-    first, middle, last = range[:1], range[1:-1], range[-1:]
-    _range = tuple(_parse_number(x.strip(), num_type) for x in middle.split(','))
-    correct = '?' not in _range
-    all_num = all(isinstance(x, num_type) for x in _range)
-    if not range or first not in '[(' or last not in '])' or len(_range)!=2 or not correct \
-            or all_num and _range[0]>_range[1]:
-        raise BadInstruction('Not understood {} range: {}'.format(num_type.__name__, range))
-    return _range
-
-
-def _normalize_range(d):
-    range = d.get('range',nan)
-    if is_null(range):
-        d.pop('range',-1)
-    # range for verifying int/float
-    elif isinstance(range,str):
-        d['_range'] = _parse_str_range(range)
-    # range for list/tuple/set initiation
-    elif isinstance(range,int):
-        d['range'] = (0,range)
-    elif not isinstance(range, MAP['listlike']):
-        raise BadInstruction('Wrong type for "range": {}'.format(type(range)))
-    elif len(range) != 2:
-        raise BadInstruction('Wrong size for "range": {}'.format(len(range)))
-    elif not isinstance(range[0],int) or not isinstance(range[1],int):
-        raise BadInstruction('"range" contains non-int type: {}'.format([type(y) for y in range]))
-
-
-def _normalize_unit(d):
-    if 'unit' in d:
-        d['unit'] = normalize_element(d['unit'])
-        init_data(d['unit'], copy=False)
-
-
-def _normalize_dtypes(d):
-    dtypes = d.get('dtypes', nan)
-    if is_null(dtypes):
-        if 'dtypes' in d:
-            del d['dtypes']
-        return
-    if is_null(d.get('_type_', nan)):
-        raise BadInstruction('_type_ must be given if "dtypes" is defined; d: {}'.format(d))
-    _type = _map(d['_type_'])
-    if not isinstance(_type, tuple):
-        _type = (_type,)
-    for_dict = any(issubclass(x, dict) for x in _type)
-    for_pandas = any(issubclass(x, (pd.Series, pd.DataFrame)) for x in _type)
-    items = []
-    default_dtype = d.get('default_dtype', None)
-    
-    if not isinstance(dtypes,dict):
-        d['dtypes'] = dtypes = OD(dtypes)
-    
-    for k,v in dtypes.items():
-        if not _isinstructions(v):
-            dd = {'_type_': _map(v, pd_dtype=for_pandas)}
-            normalize_element(dd, default=default_dtype)
-        else: 
-            dd = v #normalize_element(v) #don't use default=v, inf recursion
-        
-        if for_pandas:
-            if isinstance(dd, Element):
-                dd = dd.to_dict()
-            _type_ = dd.get('_type_')
-            _type_mapped = _map(_type_, pd_dtype=True)
-            if is_null(_type_) or not isinstance(_type_mapped, (type, str)):
-                raise BadInstruction('Pandas dtype _type_ is invalid: /k: v/: {}: {} || type(v): {}'.format(k, v, type(v)))
-            dtypes[k] = _type_mapped
-        
-        if for_dict:
-            items.append([k, dd])
-    
-    if for_dict and is_null(d.get('items',nan)):
-        d['items'] = items
-
-
-def _normalize_opt_req(d):
-    # all keys that aren't in required (if given) are optional
-    # use 'required' if nearly all keys are optional
-    aliases = {
-        'optional': ['opt','optional','keys_optional'],
-        'required': ['req','required','keys_required'],
-    }
-    for key, aliases in aliases.items():
-        final = nan
-        for alias in aliases:
-            value = d.pop(alias, nan)
-            if is_null(value):
-                pass
-            elif not isinstance(value, MAP['listlike']+(dict,)):
-                raise BadInstruction('Wrong type for "{}": {}'.format(alias, type(value)))
-            elif final is not nan:
-                raise BadInstruction('Got multiple values for {}'.format(key))
-            else:
-                final = value
-        if is_not_null(final):
-            d[key] = final
-
-
-def _normalize_vfy(d):
-    _vfy_ = d.get('_vfy_', nan)
-    if is_null(_vfy_):
-        d.pop('_vfy_', -1)
-    elif not hasattr(_vfy_, '__call__'):
-        raise BadInstruction('_vfy_ must be callable, d: {}'.format(d))
-
-
-#-------------------------------------
-#type - error/warn/ignore/fix/fix+
-#value - error/warn/ignore/fix/fix+
-#//use-this for (list-e, dict-e):
-#missing - error/warn/ignore/fix/fix+
-#extra - error/warn/ignore/fix/fix+
-
-#//explanation: 
-#fix - replace (existing), add (missing) with newly initiated element, if its _call_ is not None or value is specified, otherwise raise error;
-#    - delete (extra element)
-#fix- - fix and DON'T warn
-
-#///too-complicated:
-#list_e - {'missing': error/warn/ignore/fix/fix+,
-#           'extra': error/warn/ignore/fix/fix+,
-#           'value': error/warn/ignore/fix/fix+}
-#dict_e - {'missing': error/warn/ignore/fix/fix+,
-#           'extra': error/warn/ignore/fix/fix+,
-#           'value': error/warn/ignore/fix/fix+}
-
-#copy:
-# 'fix_mode' - the object (x) is copied only if any of the handler modes is set to 'fix'/'fix-'
-# True - obj is always copied
-# False - obj is modified inplace, if mode == 'fix/fix-'
-#         however some defective objects are still "copied" in these cases:
-#             - type mismatch between the obj and norm
-#             - the obj is immutable
-#             - copying it/making new one is considerably faster than modifying inplace (eg adding dataframe missing columns one by one)
-#         therefore user should always overwrite x = verify_data(x), and still update all the references
-
-
-_MODES = ('error','warn','ignore','fix','fix-')
-_ERROR_MODES = ('error',)
-_FIX_MODES = ('fix','fix-')
-_WARN_MODES = ('warn','fix')
-
-_HANDLER_KEYS = ('type','value','key','index','general')
-_H_OBJ_KEYS = ('type','value','general')
-_H_CONTAINER_KEYS = ('key','index')
-_H_CONTAINER_OPTIONS = ('missing','extra')
-
-
-def verify_data(x, norm, mode='error', copy=False, **kw):
-    if copy:
-        x = _copy(x)
-    copy = False
-    
-    if not _isnorm(norm):
-        norm = normalize_element(norm)
-        init_data(norm, copy=False)
-    
-    if isinstance(norm, Element):
-        norm = norm.to_dict()
-    
-    kw.update({'mode': mode})#, 'copy': copy})
-    norm_extra = kw.get('norm_extra', nan)
-    trace = kw.get('trace',[])
-    
-    _verify_input_args(kw)
-    handler = kw['handler']
-    #copy = kw['copy']
-
-    x_ver = x
-    
-    if is_not_null(norm_extra):
-        try: 
-            verify_data(x_ver, norm_extra, 'error', trace=trace)
-            #if _isinstructions(kw['norm_extra']): verify_data(x_ver,norm_extra,**kw)
-            #else: verify_data(x_ver,normalize_element({},default=norm_extra),**kw)
-        except Exception: 
-            pass
-        else: 
-            return x_ver #passed[:] = True
-        
-    
-    _defval_ = norm.get('_defval_', nan)
-    sub_allowed = norm.get('sub', norm.get('sub_allowed')) is not False
-    
-    if is_not_null(_defval_): 
-        if _verify_defval(x_ver, _defval_, sub_allowed=sub_allowed):
-            return x_ver
-    
-    
-    _multi_ = norm.get('_multi_', nan)
-    
-    if is_not_null(_multi_) and len(_multi_):
-        return _verify_multi(x_ver, _multi_, mode, trace, handler, copy)
-    
-    
-    #---------------------------------------------------------------
-    #---------------------------------------------------------------
-    _type = type(x)
-    t_name = _type.__name__
-    len_trace = len(trace)
-    trace2 = trace + ['({}){}'.format(len_trace, t_name)]
-    
-    if not len_trace and copy:
-        x_ver = init_data(x, copy=True) #done many times if _multi_ specified
-    else:
-        x_ver = x
-    
-    passed = pd.Series(True, ['type','value','range','vfy'])
-    
-    
-    #-type-
-    normtype = norm.get('_type_', nan)
-    
-    if is_not_null(normtype):
-        r = _verify_type(_type, normtype, sub_allowed)
-        if r is not True: 
-            _handle_error(handler, 'type', [trace2, t_name, r])
-            passed.type = False
-    
-    
-    #-value-
-    has_value = '_value_' in norm
-    _multival_ = norm.get('_multival_', nan)
-    
-    if has_value:
-        _value_ = norm.get('_value_')
-        passed.value = compare(x_ver, _value_, type_op='ignore')
-        if not passed.value:
-            _handle_error(handler, 'value', [trace2, x_ver, _value_])
-    
-    elif is_not_null(_multival_):
-        passed.value = any(compare(x_ver, val, type_op='ignore') for val in _multival_)
-        if not passed.value:
-            _handle_error(handler, 'value', [trace2, x_ver, _multival_])
-    
-    else:
-        try: iter(x_ver)
-        except TypeError: pass
-        else: 
-            x_ver = _verify_elements(x_ver, norm, mode, trace2, handler, copy)
-    
-    
-    #-range-
-    range = norm.get('range')
-    if isinstance(x_ver, (int, float)) and is_not_null(range) and isinstance(range, str):
-        passed.range = _verify_in_range(x_ver, norm)
-        if not passed.range:
-            _handle_error(handler, 'value', [trace2, x_ver, 'in range: {}'.format(range)])
-    
-    
-    _vfy_ = norm.get('_vfy_')
-    if is_not_null(_vfy_) and passed.all():
-        try: _vfy_(x_ver)
-        except Exception as e:
-            passed.vfy = False
-            e_type, e_args = _parse_user_error(e, trace2, x_ver)
-            _handle_error(handler, e_type, e_args)
-    
-    
-    if not passed.all():
-        x_ver = init_data(norm)
-    
-    
-    return x_ver
-
-
-def _verify_defval(x, _defval_, **kw):
-    _type = type(x)
-    try:
-        _type1 = _defval_['_type_']
-    except Exception as e:
-        print(x, _defval_, kw)
-        raise e
-    _type1a = EQUALS.get(_type1) if not isinstance(_type1,tuple) else tuple((EQUALS.get(t2) for t2 in _type1))
-    
-    correct_types = _flatten_types(_type1, _type1a)
-    sub_allowed = _defval_.get('sub', _defval_.get('sub_allowed'))
-    defval_sub_allowed = False if sub_allowed is False else kw.get('sub_allowed',True)
-    
-    r = _verify_type(_type, correct_types, sub_allowed=defval_sub_allowed)
-    
-    if r is not True: pass
-    elif not compare(x, init_data(_defval_, copy=False), type_op='ignore'): pass
-    #print('Compare UNSUCCESSFUL! {} {}'.format(x,_defval_)
-    else: return True
-    
-    return False
-
-
-def _verify_multi(x, _multi_, mode, trace, handler, copy=False):
-    exceptions = []
-    passed = False
-    x_ver = _null = object()
-    
-    for norm in _multi_:
-        try:
-            x_ver = verify_data(x, norm, 'error', trace=trace)
-            passed = True
-        except VeriError as e:
-            exceptions.append(e)
-        else:break
-    
-    if not passed:
-        dx = _handle_error(handler, exceptions) #may raise (if deepest lvl error's mode in handler is 'error')
-        is_fix = dx['is_fix']
-        
-        if is_fix: 
-            most_similar_norm = _multi_[dx['i']] #i is the index of the first deepest level error
-            x_ver = verify_data(x, most_similar_norm, mode, copy, trace=trace, handler=handler)
- 
-        #A drawback of singling out -> _multi: [{'_type_:xr}, {'_type_':x}] only shows the first e msg
-        #raise VeriError('Verification failed. The following exceptions occurred: {}'.format(exceptions))
-    
-    if x_ver is _null:
-        x_ver = x if not copy else _copy(x)
-    
-    return x_ver
-
-
-def _verify_in_range(x, norm):
-    range = norm['range']
-    limit0, limit1 = norm['_range']
-    
-    if limit0 is not None:
-        result0 = limit0 <= x if range[0]=='[' else limit0 < x
-        if not result0:
-            return False
-    
-    if limit1 is not None: 
-        result1 = x <= limit1 if range[-1]==']' else x < limit1
-        if not result1:
-            return False
-    
-    return True
-
-#-------------------------------------------------------------
-    
-def _verify_elements(x, norm, mode, trace, handler, copy=False):
-    pdlike = (pd.Series, pd.DataFrame)
-    _check_size(x, norm, trace, handler)
-
-    if isinstance(x, dict):
-        x_ver = _verify_dict(x, norm, mode, trace, handler, copy)
-
-    elif isinstance(x, pdlike):
-        x_ver= _verify_pandaslike(x, norm, mode, trace, handler, copy) 
-            
-    else: #if isinstance(x,(list,tuple,set)) or is_iterable:
-        x_ver = _verify_listlike(x, norm, mode, trace, handler, copy)
-
-                          
-    return x_ver
-
-
-def _verify_dict(x, norm, mode, trace, handler, copy=False):
-    fix_vals = handler['type'] in _FIX_MODES or handler['value'] in _FIX_MODES
-    
-    unit = norm.get('unit',nan)
-    extra_allowed = norm.get('extra_allowed')
-    keys_opt = norm.get('optional',[])
-    keys_req = norm.get('required',nan)
-    
-    nitems = norm.get('items')
-    
-    if nitems:
-        nkeys = [itm[0] for itm in nitems]
-        me = _verify_keys(x.keys(), nkeys, trace, handler, keys_opt, keys_req, extra_allowed)
-        
-        if handler['key']['missing'] in _FIX_MODES and len(me['missing_all']):
-            #messes up order if OD
-            n_inited = init_data(norm,copy=False)
-            #if len(missing): print(trace,'missing:',missing)
-            x.update({_copy(k):_copy(v) for k,v in n_inited.items() if k in me['missing_all']})
-            
-        for nk,nv in nitems:
-            if nk in me['missing_all']:continue
-            trace2 = trace[:-1] + [''.join(trace[-1:]) + '({})(key){}'.format(len(trace),nk)]
-            xv = verify_data(x[nk], nv, mode, trace=trace2, handler=handler)
-            if fix_vals: x[nk] = xv
-        
-        if handler['key']['extra'] in _FIX_MODES and len(me['extra']):
-            for ke in me['extra']:
-                x.pop(ke)
-
-    if is_not_null(unit):
-        for k,v in x.items():
-            trace2 = trace[:-1] + [''.join(trace[-1:]) + '({})(key){}'.format(len(trace),k)]
-            xv = verify_data(v, unit, mode, trace=trace2, handler=handler)
-            if fix_vals: x[k] = xv
-             
-    return x
-
-
-def _verify_pandaslike(x, norm, mode, trace, handler, copy=False):
-    unit = norm.get('unit',nan)
-    extra_allowed = norm.get('extra_allowed')
-    keys_opt = norm.get('optional',[])
-    keys_req = norm.get('required',nan)
-    
-    is_series = isinstance(x,pd.Series)
-    is_df = isinstance(x,pd.DataFrame)
-    
-    ndtype0 = norm.get('dtype',nan)
-    ndtypes = norm.get('dtypes',nan)
-    #dtypes = x.dtypes
-    inplace = not(copy)
-    
-    wrong_dtypes = []
-    dtypes = x.dtypes.iteritems() if is_df else [(x.name,x.dtype)]
-    
-    for c,itm in dtypes:
-        dtype = _map(itm.name, pd_dtype=True)
-        if is_not_null(ndtype0):
-            ndtype = ndtype0 
-        elif is_not_null(ndtypes) and c in ndtypes:
-            ndtype = ndtypes[c]
-        else: continue
-        
-        #both may be strings (datetime64[ns])
-        #however. int may be float
-        if dtype != ndtype and dtype is not PD_EQUALS.get(ndtype):
-            wrong_dtypes.append({c:(dtype,ndtype)})
-     
-    nr_wrong = len(wrong_dtypes)    
-            
-    if nr_wrong:
-        trace2 = trace + ['({})(dtypes)'.format(len(trace))]
-        _handle_error(handler, 'type', [trace2, wrong_dtypes])
-            
-    if nr_wrong and handler['type'] in _FIX_MODES:
-        for c, tpl in wrong_dtypes:
-            dtype,ndtype = tpl
-            try:
-                if is_df: x[c] = x[c].astype(ndtype)
-                else: x = x.astype(ndtype)
-            except Exception as e:
-                logging.exception(e)
-            
-            
-    ncols = norm.get('columns')
-    nindex = norm.get('index')
-    
-    _keys = ('missing','extra','missing_all','extra_all')
-    me_cols = {_k: [] for _k in _keys}
-    me_ind = {_k: [] for _k in _keys}
-    
-    if isinstance(keys_opt,dict):
-        index_opt = keys_opt.get('index')
-        cols_opt = keys_opt.get('columns')
-    else: index_opt = cols_opt = []
-    
-    if isinstance(keys_req,dict):
-        index_req = keys_req.get('index')
-        cols_req = keys_req.get('columns')
-    else: index_req = cols_req = nan
-    
-    if isinstance(extra_allowed,dict):
-        ea_index = extra_allowed.get('index')
-        ea_cols = extra_allowed.get('columns')
-    else: ea_index = ea_cols = extra_allowed
-    
-    if is_df and ncols is not None:
-        me_cols = _verify_keys(x.columns, ncols, trace, handler, cols_opt, cols_req, ea_cols)
-        
-    if nindex is not None:
-        me_ind = _verify_keys(x.index, nindex, trace, handler, index_opt, index_req, ea_index)
-    
-    if handler['key']['missing'] not in _FIX_MODES: pass
-    elif len(me_ind['missing']) or len(me_cols['missing']):
-        x_new = init_data(norm)
-        if not inplace: #much faster
-            if is_series: x_new.loc[x.index] = x
-            else: x_new.loc[x.index,x.columns] = x  #(this doesn't link the old x's values with x_new)
-            x = x_new
-    
-        else:
-            for c in me_cols['missing']:
-                pos = next((j for j in ncols if j == c),x.shape[1])
-                x.insert(pos, c, x_new[c])
-                
-            if is_df:
-                for i in me_ind['missing']:
-                    pos = next((j for j in nindex if j == i),x.shape[0])
-                    x.insert(pos, i, x_new.loc[i,:],axis=1)
-            else:
-                for i in me_ind['missing']:
-                    x[i] = x_new[i]
-
-        
-    if handler['key']['extra'] in _FIX_MODES:
-        if len(me_ind['extra']): 
-            if inplace: x.drop(me_ind['extra'], inplace=True)
-            else: x = x.drop(me_ind['extra'])
-        if len(me_cols['extra']):
-            if inplace: x.drop(me_cols['extra'], axis=1, inplace=True)
-            else: x = x.drop(me_cols['extra'], axis=1)
-          
-    return x
-            
-     
-             
-def _verify_listlike(x, norm, mode, trace, handler, copy=False):
-    if isinstance(x, set):
-        new = _verify_set_elements_by_nvalue(x, norm, mode, trace, handler)
-    else:
-        new = _verify_list_elements_by_nvalue(x, norm, mode, trace, handler)
-    
-    unit = norm.get('unit', nan)
-                  
-    if is_not_null(unit):
-        new = [verify_data(v, unit, mode, trace=trace, norm_extra=NORM_EXTRA, handler=handler)
-                for v in new]
-            
-    #if only unit is given, and e.g `unit = {'_type_': dt, '_call_': None}`, `mode = 'fill'` doesn't replace the wrong values with None
-    #(mode 'fill' does and will only work for *missing* data, with either _dict_ attr present, or listlike with endings capped)
-    
-    if is_not_null(new): #and any(m in _FIX_MODES for m in handler.values()):
-        #deepcopy norm_new?
-        norm_new = {k: norm[k] for k in norm if k not in ('_copy_',)}
-        norm_new.update({'values': new}) #,'_value_':None})
-        x = init_data(norm_new)
-    
-    return x
-
-
-def _verify_set_elements_by_nvalue(x, norm, mode, trace, handler):
-    extra_allowed = norm.get('extra_allowed')
-    nvalue = norm.get('value', norm.get('values', norm.get('v', nan)))
-    if is_null(nvalue):
-        return x
-    
-    missing = set(_ for _ in nvalue if _ not in x)
-   
-    if not missing: pass
-    elif handler['index']['missing'] in _FIX_MODES:
-        x.update(set(_copy(_) for _ in missing))
-    else:
-        _handle_error(handler, 'value', [trace, nan, 'missing:{}'.format(missing)])
-    
-    if not extra_allowed:
-        extra = set(_ for _ in x if _ not in nvalue)
-        if not extra: pass
-        elif handler['index']['extra'] in _FIX_MODES:
-            for _ in extra:
-                x.pop(_)
-        else:
-            _handle_error(handler, 'value', [trace, 'extra:{}'.format(extra)])
-            
-    return x
-
-
-def _verify_list_elements_by_nvalue(x, norm, mode, trace, handler):
-    extra_allowed = norm.get('extra_allowed')
-    nvalue = norm.get('value', norm.get('values', norm.get('v', nan)))
-    if is_null(nvalue):
-        return x
-    
-    len_x, len_nv = len(x), len(nvalue)
-    _min_len = min(len_x,len_nv)
-    norm_extra = NORM_EXTRA #?? Should this be deprecated?
-    #if sizes differ then zip will only iterate to the lowest size
-    new = x[:_min_len]
-    
-    if len_x < len_nv:
-        if handler['index']['missing'] in _FIX_MODES:
-            x_new = init_data(norm, copy=False)
-            new += _copy(x_new[len_x:])
-        else:
-            _handle_error(handler, 'value', [trace, nan, 'missing:{}'.format(nvalue[len_x:])])
-    
-    if len_x > len_nv and not extra_allowed:
-        if handler['index']['extra'] not in _FIX_MODES:
-            _handle_error(handler, 'value', [trace, 'extra:{}'.format(x[len_nv:])])
-            new += x[len_nv:]
-            
-    new = [verify_data(v, nv, mode, trace=trace, handler=handler, norm_extra=norm_extra)
-           for v,nv in zip(new[:_min_len],nvalue)] + new[_min_len:]
-    
-    return new
-
-
-#-----------------------------------------------------------------------
-
-def _verify_type(_type, correct_types, sub_allowed=True, **kw):
-    ctps = correct_types
-    ctps2 = EQUALS.get(ctps) if not isinstance(ctps,tuple) else tuple((EQUALS.get(t1) for t1 in ctps))
-    #Note that due to normalisation norm['_type'] is always hashable (is either type or tuple or types)
-    
-    correct_types = _flatten_types(ctps, ctps2)
-    #as_dict = kw.get('as_dict')
-    
-    if sub_allowed and not issubclass(_type, correct_types): pass
-    elif not sub_allowed and _type not in correct_types: pass
-    else: return True
-    
-    return correct_types
-
-
-def _get_missing_extra(x, norm):
-    missing = tuple(filter(lambda nk: nk not in x, norm))
-    extra = tuple(filter(lambda k: k not in norm, x))
-    
-    return {'missing': missing, 'extra': extra}
-
-
-def _verify_keys(x, norm, trace, handler, optional=[], required=None, extra_allowed=False):
-    me = _get_missing_extra(x,norm)
-    extra = tuple(filter(lambda k: k not in optional, me['extra'])) if not extra_allowed else tuple()
-    missing = tuple(filter(lambda k: k not in optional, me['missing']))
-    if is_not_null(required):
-        missing = tuple(filter(lambda k: k in required, missing))
-    
-    len_missing,len_extra = len(missing),len(extra)
-    if not len_missing + len_extra:
-        return {'missing': missing, 'extra': extra, 'missing_all': me['missing'], 'extra_all': me['extra']}
-    
-        
-    mp = missing if len_missing else nan
-    ep = extra if len_extra else nan
-    
-    trace2 = trace + ['({})'.format(len(trace))]
-    _handle_error(handler, 'key', [trace2, ep, mp])
-        
-    return {'missing': missing, 'extra': extra, 'missing_all': me['missing'], 'extra_all': me['extra']}
-
-
-def _check_size(x, norm, trace, handler):
-    size = norm.get('size')
-    if is_null(size):
-        return True
-    
-    len_x = len(x)
-    all_correct = True
-    
-    for arg,op in [('min',lambda y: len_x>=y),
-                   ('max',lambda y:len_x<=y),
-                   ('exact',lambda y: len_x==y)]:
-        limit = size.get(arg)
-        if is_null(limit): continue
-        satisfied = op(limit)
-        all_correct = min(all_correct, satisfied)
-        if not satisfied:
-            _handle_error(handler, 'index', [trace, len_x, '{}:{}'.format(arg,limit)])
-            
-    return all_correct
-
-
-def _check_size2(x, norm, trace, handler):
-    size = norm.get('size',nan)
-    if not is_not_null(size):
-        return True
-    
-    size = norm.get('size')
-    incl = size.get('include',nan)
-    excl = size.get('exclude',nan)
-    len_x = len(x)
-    is_correct = False
-    
-    if is_not_null(excl) and len_x in excl:
-        _handle_error(handler, 'index', [trace,'({}, excl:{})'.format(len_x, excl)])
-         
-    elif is_not_null(incl) and len_x not in incl:
-        _handle_error(handler, 'index', [trace,'({}, incl:{})'.format(len_x, excl)])
-            
-    else: is_correct = True
-            
-            
-    return is_correct
-    
-
-#-------------------------------------------------------------------------------------------------
-
-def _flatten_types(_types, _equals=None):
-    try: _types = tuple(flatten(_types))
-    except TypeError: _types = (_types,)
-    
-    try: _equals = tuple(flatten(_equals))
-    except TypeError: _equals = (_equals,)
-    
-    f = lambda x: x is not None
-    
-    return tuple(unique(filter(f, _types + _equals)))
-
-
-def _verify_is_type(x):
-    if not type(x) is type:
-        raise BadInstruction('Is not type: {}'.format(x))
-    
-    return x
-
-
-def _verify_input_args(kw):
-    handler = kw.get('handler',{})
-    if _isnorm(handler): return kw
-    elif not isinstance(handler,dict):
-        raise TypeError('Handler must be dict, instead got: {}'.format(type(handler).__name__))
-    
-    mode = kw['mode']
-    if kw['mode'] not in _MODES:
-        raise ValueError('Wrong mode: {}'.format(mode))
-    
-    fix_any = mode in _FIX_MODES
-    
-    #--else--:
-    
-    for k in _H_OBJ_KEYS:
-        hx_mode = handler.get(k, kw.get(k,mode))
-        if hx_mode in _FIX_MODES:
-            fix_any = True
-        elif hx_mode not in _MODES:
-            raise ValueError('Wrong "{}" mode: {}'.format(k, hx_mode))
-        handler[k] = hx_mode
-    
-    #{'key': {'extra': _mode, 'missing': _mode2}, 'index': ...} 
-    by_mode = {c: {x: mode for x in _H_CONTAINER_OPTIONS} for c in _H_CONTAINER_KEYS}
-    by_option = {c: {x: kw.get(x) for x in _H_CONTAINER_OPTIONS} for c in _H_CONTAINER_KEYS}
-    by_type = {c: {x: kw.get(c) for x in _H_CONTAINER_OPTIONS} for c in _H_CONTAINER_KEYS}
-    by_handler = {c: {x: handler.get(c, {}).get(x) for x in _H_CONTAINER_OPTIONS} for c in _H_CONTAINER_KEYS}
-    
-    hierarchy = {None: {'doms': 'all'}} #do not overwrite with None
-    for x in (by_mode, by_option, by_type, by_handler):
-        deep_update(handler, x, False, hierarchy)
-
-    
-    for c in _H_CONTAINER_KEYS:
-        for x in _H_CONTAINER_OPTIONS:
-            cx_mode = handler[c][x]
-            if cx_mode in _FIX_MODES:
-                fix_any = True
-            elif cx_mode not in _MODES:
-                raise ValueError('Wrong "{}" mode: {}; kwargs: {}'.format(c, cx_mode, kw))
-            
-    """for k in _H_CONTAINER_KEYS:
-        hx_mode = handler.get(k) #, kw.get(k,mode)
-        if hx_mode is None:
-        if isinstance(hx_mode,str):
-            if hx_mode in _MODES:
-                if hx_mode in _FIX_MODES:
-                    fix_any = True
-                handler[k] = hx_mode = dict.fromkeys(_H_CONTAINER_OPTIONS, hx_mode)
-            else:
-                raise ValueError('Wrong "{}" mode: {}'.format(k, hx_mode))
-        
-        elif not isinstance(hx_mode,dict):
-            raise TypeError('Wrong type for "{}" mode: {}'.format(k, type(hx_mode).__name__))
-        
-        d = hx_mode
-        for k2 in _H_CONTAINER_OPTIONS:
-            hox_mode = d.get(k2, handler.get(k2, kw.get(k2,mode)))
-            if hox_mode in _FIX_MODES:
-                fix_any = True
-            elif hox_mode not in _MODES:
-                raise ValueError('Wrong "{}":{} mode: {}'.format(k, k2, hox_mode))
-            d[k2] = hox_mode
-            
-        handler[k] = d"""
-        
-        
-    handler['_isnorm_'] = True
-    kw['handler'] = handler
-    
-    
-    """copy = kw['copy']
-    if type(copy) is bool: pass
-    elif isinstance(copy,str): pass
-    else: raise TypeError('Wrong type for "copy" argument: {}'.format(type(copy)))
-    
-    if copy == 'fix_mode':
-        if fix_any: copy = True
-        else: copy = False
-        
-    kw['copy'] = copy"""
-        
-        
-    for k in list(kw.keys()):
-        if k not in ('handler','mode','copy'):
-            del kw[k]
-            
-
-
-def _single_out(errors):
-    #higher is more specific
-    def _get_error_rank(e):
-        return _EXC_ORD.index(type(e))
-    
-    def _update(e, rank, lvl, i):
-        e_inf.update({'errors': [e], 'rank': rank, 'lvl': lvl, 'i': i+1})
-    
-    _errors = errors
-    e_inf = {'errors': [_errors[0]],
-             'rank': _get_error_rank(errors[0]),
-             'lvl': errors[0].level,
-             'i': 0}
-    
-    for i,e in enumerate(errors[1:]):
-        rank = _get_error_rank(e)
-        lvl = e.level #_get_trace_lvl(e)
-        
-        if lvl > e_inf['lvl']:
-            _update(e, rank, lvl, i)
-        
-        elif lvl == e_inf['lvl']:
-            if rank > e_inf['rank']:
-                _update(e, rank, lvl, i)
-            elif rank == e_inf['rank']: 
-                e_inf['errors'].append(e)
-
-
-    errors = e_inf['errors']
-    
-    if len(errors) == 1:
-        return {'e': errors[0], 'i': e_inf['i']}
-    
-    e_args = []
-    msgs = []
-    for i,e in enumerate(errors):
-        #if i > 0: e.args[0] = " ".join(e.args[0].split(" ")[1:])
-        #the first arg begins with trace, which'll be identical for same lvl same type errors
-
-        #e_args.extend(e.args)
-        e_args = e.args # this includes trace, got, expected, custom_msg, and the *args
-        msgs.append(e.msg)
-    
-    new_e = errors[0].__class__(*e_args) # use the info of the last error
-    new_e.msg = " || ".join(msgs)
-    
-    return {'e': new_e, 'i': e_inf['i']}
-    
-
-"""def _get_trace_lvl(e):
-    msg = e.args[0]
-    trace = msg.split(" ")[0]
-    
-    lvl = 0
-    
-    for i,c in enumerate(trace):
-        if c!= "(": continue
-        i2 = next(((i+1)+j for j,c2 in enumerate(trace[i+1:]) if not c2.isdigit()),-1)
-        if i2 in (-1,i+1) or trace[i2] != ")": continue
-        
-        lvl2 = int(trace[i+1:i2])
-        if lvl2 != lvl + 1: continue
-        
-        lvl = lvl2
-        
-    return lvl"""
-
-
-def _handle_error(handler, type, args=[], kw={}):
-    e, i = (None, 0)
-    
-    if isinstance(type,VeriError): 
-        e = type
-    elif isinstance(type,(list,tuple)):
-        if len(type) > 1:
-            d = _single_out(type)
-            e,i = d['e'],d['i']
-        else: e = type[0]
-        
-    if e is not None: 
-        type = e.type
-    
-    mode = handler[type]
-    ms = None
-    
-    if not isinstance(mode,dict):
-        ms = _mode_specs(mode)
-    
-        if not (ms['is_error'] or ms['is_warn']):
-            return {'i': i, 'is_fix': ms['is_fix']}
-    
-
-    if e is None:
-        eclass = _EXCEPTIONS[type]
-        e = eclass(*args,**kw)
-        
-    if ms is None:
-        ms = _mode_specs_from_error(e, handler)
-        
-    
-    if ms['is_error']:
-        raise e
-    elif ms['is_warn']:
-        warnings.warn(str(e))
-    
-    return {'i': i, 'is_fix': ms['is_fix']}
-    
-
-
-def _mode_specs(mode):
-    if mode is None:
-        return dict.fromkeys(('is_error','is_fix','is_warn'), False)
-        
-    is_error = mode in _ERROR_MODES
-    is_warn = False if is_error else mode in _WARN_MODES
-    is_fix = False if is_error else mode in _FIX_MODES
-    
-    return {'is_error': is_error, 'is_fix': is_fix, 'is_warn': is_warn}
-
-
-def _mode_specs_from_error(e,handler):
-    is_faulty = e.is_faulty()
-    x = handler[e.type]
-    
-    if is_faulty is True:
-        return _mode_specs(x)
-    elif is_faulty is False:
-        return _mode_specs(None)
-    
-    #-else is_faulty is dict
-    
-    specs = _mode_specs(None)
-    
-    for subset,f_val in is_faulty.items():
-        if not f_val: continue
-        
-        e_mode = x[subset]
-        new_specs = _mode_specs(e_mode)
-        specs.update({k:v for k,v in new_specs.items() if v})
-        
-        
-    return specs
-
-
-def _parse_user_error(e, trace, got=nan, expected=nan, custom_msg=nan):
-    args = [trace, got, expected, custom_msg]
-    if type(e) in _EXC_MAP.values():
-        e_type = next(x for x,y in _EXC_MAP.items() if type(e)==y).type
-        args[3] = nan if not e.args else (e.args[0] if len(e.args)==1 else e.args)
-        return e_type, args
-    elif isinstance(e, VeriError):
-        args[0] = list(trace) + list(e.trace)
-        if e.got is not nan:
-            args[1] = e.got
-        if e.expected is not nan:
-            args[2] = e.expected
-        if e.custom_msg is not nan:
-            args[3] = e.custom_msg
-        return e.type, args
-    else:
-        args[3] = e
-        return 'general', args
-
-
-def convert_exception(e):
-    t = _EXC_MAP.get(type(e))
-    if not t:
-        return e
-    
-    return t(e.msg)
-
-
-
-#--------------------------------------
-
-def fill_missing(x, norm, warn=True):
-    mode = 'fix' if warn else 'fix-'
-    return verify_data(x, norm, mode=mode)
-
-#......................................
-
-def _resolve(x, as_type=False):
-    if _isinstructions(x):
-        return x
-    if as_type:
-        e = None
-        try: 
-            d = {'_type_': x}
-            _normalize_type(d)
-            if '_type_' in d:
-                return d
-            e = BadInstruction('Does not resolve to type: {}'.format(x))
-        except BadInstruction as exc:
-            e = exc
-        if e and as_type!='try':
-            raise e
-    return {'_value_': x}
-
-
-class Element:
-    __aliases = {
-        'type': ['_type_', 'type'],
-        'value': ['_value_', 'value'],
-        'multival': ['_multival_', 'multival'],
-        'defval': ['_defval_', 'defval'],
-        'unit': ['unit'],
-        'dtypes': ['dtypes'],
-        'default_dtype': ['default_dtype'],
-        'call': ['_call_', 'call'],
-        'keys': ['keys'],
-        'values': ['values', 'v'],
-        'items': ['items'],
-        'multi': ['_multi_','multi'],
-        'vfy': ['_vfy_', 'vfy'],
-        'isnorm': ['_isnorm_','isnorm'],
-    }
-    
-    def __init__(self, *type, **kw):
-        self.verify_params(type, kw)
-        if len(type):
-            self.type = type[0] if len(type) == 1 else type
-        
-        self.update(kw)
-    
-    
-    def __call__(self, copy=True):
-        return init_data(self, copy=copy)
-    
-    
-    def verify(self, x, mode='error', copy=False, **kw):
-        return verify_data(x, self, mode, copy, **kw)
-    
-    
-    def to_dict(self, **kw):
-        if hasattr(self, '__dict') and not kw:
-            return self.__dict
-        d = {}
-        #copy_attrs = ['unit','dtypes']
-        
-        for attr, aliases in self._Element__aliases.items():
-            alias = aliases[0]
-            if hasattr(self, attr):
-                value = getattr(self, attr)
-                #if attr in copy_attrs:
-                #    value = value.copy()
-                d[alias] = value
-        
-        d.update(self.__kw)
-        self.__dict = d
-        
-        if kw:
-            d = dict(d, **kw)
-        
-        return d
-    
-    
-    def update(self, d, normalize=True):
-        resolve_attrs = ['unit']
-        resolve_elements = ['dtypes','multi']
-        found = []
-        
-        for attr, aliases in self._Element__aliases.items():
-            for alias in aliases:
-                if alias in d:
-                    value = d[alias]
-                    if attr in resolve_attrs:
-                        value = _resolve(value)
-                    if attr in resolve_elements:
-                        if isinstance(value, dict):
-                            value = {k: _resolve(v, 'try') for k,v in value.items()}
-                        else:
-                            value = [_resolve(v) for v in value]
-                    setattr(self, attr, value)
-                    found.append(alias)
-        
-        self.__kw = {k: v for k,v in d.items() if k not in found}
-        
-        if hasattr(self, '__dict'):
-            del self.__dict
-        
-        if normalize:
-            if hasattr(self, 'isnorm'):
-                del self.isnorm
-            normalize_element(self)
-        else:
-            self.to_dict()
-    
-    
-    def get(self, key, *default):
-        return self.__dict.get(key, *default)
-    
-    
-    def __contains__(self, key):
-        return key in self.__dict
-    
-    
-    def __len__(self):
-        ignore = {'_copy_','_isnorm_'}
-        return sum(1 for x in self.__dict if x not in ignore)
-    
-    
-    @classmethod
-    def verify_params(cls, type, kw):
-        must_contain_attr = '_{}__must_contain'.format(cls.__name__)
-        if hasattr(cls, must_contain_attr):
-            must_contain = getattr(cls, must_contain_attr)
-            for attr in must_contain:
-                aliases = cls._Element__aliases[attr]
-                if not any(x in kw for x in aliases):
-                    raise BadInstruction('Does not contain: {}'.format(attr))
-
-
-class Container(Element):
-    
-    def __getitem__(self, key):
-        if not isinstance(key, tuple):
-            key = (key,)
-        
-        d = self.to_dict()
-        unit = d.get('unit', {})
-        
-        if len(key) == 1:
-            unit.update(_resolve(key[0], 'try'))
-        elif len(key) > 1:
-            resolved = [_resolve(k, 'try') for k in key]
-            types_only, values_only, other = [], [], []
-            for x in resolved:
-                if len(x) == 1 and '_type_' in x:
-                    if isinstance(x.get('_type_'), tuple):
-                        types_only += list(x.get('_type_'))
-                    else:
-                        types_only.append(x.get('_type_'))
-                elif len(x) == 1 and '_value_' in x:
-                    values_only.append(x.get('_value_'))
-                elif len(x) == 1 and '_multival_' in x:
-                    values_only += list(x.get('_multival_'))
-                else:
-                    other.append(x)
-            
-            _type = {'_type_': tuple(types_only) if len(types_only) > 1 else types_only[0]} if len(types_only) else {}
-            _value = ({'_multival_': values_only} if len(values_only)> 1 else {'_value_': values_only[0]}) if values_only else {}
-            if _type and (not _value and not other):
-                unit.update(_type)
-            elif _value and (not _type and not other):
-                unit.update(_value)
-            else:
-                multi = []
-                if _type:
-                    multi.append(_type)
-                if _value:
-                    multi.append(_value)
-                if other:
-                    multi += other
-                unit['_multi_'] = multi
-        
-        if 'unit' in d or unit:
-            d['unit'] = unit
-        
-        return Container(**d)
-    
-    
-    def __iter__(self):
-        raise TypeError("'Container' object is not iterable.")
-
-
-class Multi(Element):
-    def __init__(self, *elements, **kw):
-        if not elements:
-            raise BadInstruction('No elements provided')
-        if 'multi' not in 'kw':
-            kw['multi'] = elements
-        super().__init__(**kw)
-
-
-class Type(Element):
-    __must_contain = ['type']
-    
-    def __init__(self, *type, **kw):
-        if not type:
-            raise BadInstruction('type not provided')
-        if 'type' not in kw:
-            kw['type'] = type
-        super().__init__(**kw)
-
-
-class Value(Element):
-    __must_contain = ['value']
-    
-    def __init__(self, value, **kw):
-        if 'value' not in kw:
-            kw['value'] = value
-        super().__init__(**kw)
-
-
-class MultiVal(Element):
-    __must_contain = ['multival']
-    
-    def __init__(self, *values, **kw):
-        if 'multival' not in kw:
-            kw['multival'] = list(values)
-        super().__init__(**kw)
-
-
-class Dtyct(Container):
-    __must_contain = ['dtypes']
-    
-    def __init__(self, dtypes, **kw):
-        if 'dtypes' not in kw:
-            kw['dtypes'] = dtypes
-        super().__init__(dict, **kw)
-    
-    @classmethod
-    def from_dtypes(cls, *kw, **dtypes):
-        kw = kw[0] if kw else {}
-        return cls(dtypes, **kw)
-
-
-class IntRange(Element):
-    def __init__(self, range, **kw):
-        if 'range' not in kw:
-            kw['range'] = range
-        super().__init__(int, **kw)
-
-
-class FloatRange(Element):
-    def __init__(self, range, **kw):
-        if 'range' not in kw:
-            kw['range'] = range
-        super().__init__(float, **kw)
-
-
-Str = Element(str)
-Int = Element(int)
-Float = Element(float)
-Bool = Element(bool)
-Null = Element(type(None))
-List = Container(list)
-Dict = Container(dict)
-NullDict = Container(dict, unit={'_defval_': None}, default_dtype=None)
-Set = Container(set)
-
-
-__all__ = ['Str','Int','Float','Bool','Null','List','Dict','Dtyct','NullDict',
-           'Set','Multi','Type','Value','MultiVal','Element','Container',
-           'IntRange','FloatRange','normalize_element','normalize','init_data',
-           'verify_data','convert_exception','fill_missing']
+from collections import OrderedDict as OD
+import pandas as pd
+import numpy as np
+import datetime as dt
+from dateutil.parser import parse as parsedate
+import traceback
+import warnings
+import logging
+
+from fons.errors import (BadInstruction, VeriError, VeriTypeError, 
+                         VeriValueError, VeriKeyError, VeriIndexError)
+
+from fons.dict_ops import deep_update
+from fons.iter import (flatten, unique)
+from fons.pyops import (compare, copy as _copy)
+from fons.nan import (nan, Implemented) 
+
+#is_given: nan is NOT implemented
+is_given = Implemented()
+#is_not_null : nan, None and '_nan_' are NOT implemented
+is_not_null = Implemented([None,'_nan_'])
+is_null = lambda x: not is_not_null(x)
+
+
+_EXCEPTIONS = {'type': VeriTypeError,
+               'value': VeriValueError,
+               'key': VeriKeyError,
+               'index': VeriIndexError,
+               'general': VeriError,}
+
+_EXC_MAP = {VeriTypeError: TypeError,
+            VeriValueError: ValueError,
+            VeriKeyError: KeyError,
+            VeriIndexError: IndexError,}
+
+
+_EXC_ORD = [VeriError, VeriTypeError, VeriValueError, VeriKeyError, VeriIndexError]
+
+
+mappings  =  [[['pd.DataFrame','pandas.DataFrame','pandas.core.frame.DataFrame'],pd.DataFrame],
+              [['pd.Series','pandas.Series','pandas.core.series.Series'],pd.Series],
+              [['list'],list],
+              [['tuple'],tuple],
+              [['dict','dictionary'],dict],
+              [['OrderedDict'],OD],
+              [['set'],set],
+              [['string','str'],str],
+              [['int','int8','int16','int32','int64','integer'],int],
+              [['float','float16','float32','float64'],float],
+              [['np.ndarray','numpy.ndarray'],np.array],
+              [['np.ndarray','numpy.ndarray'],np.array],
+              [['dt.date','datetime.date','date'],dt.date],
+              [['dt','dt.datetime','datetime.datetime','datetime','datetime64[ns]'],dt.datetime],
+              [['td','dt.timedelta','datetime.timedelta','timedelta','timedelta64[ns]'],dt.timedelta],
+              [['object'],str],
+              [['type'],type],
+              [['listlike'],(list,tuple,np.ndarray,pd.Index)],
+              [['dictlike'],(dict,OD)]]
+
+
+MAP = {}
+for strnames,func in mappings:
+    MAP.update(dict.fromkeys(strnames, func))
+    MAP.update({func: func})
+    
+    
+EQUALS = {np.datetime64: pd.Timestamp,
+          dt.datetime: pd.Timestamp,
+          np.timedelta64: pd.Timedelta,
+          dt.timedelta: pd.Timedelta,
+          int: np.int32,
+          #type(None): pd._libs.tslib.NaTType,
+          float: (np.float64, int, np.int32),}
+
+#For checking random objs agains pandas objs
+PD_EQUALS = {np.datetime64: pd.Timestamp,
+             dt.datetime: pd.Timestamp,
+             np.timedelta64: pd.Timedelta,
+             dt.timedelta: pd.Timedelta,
+             int: float}
+
+"""for k,v in list(EQUALS.items()):
+    EQUALS[v] = k"""
+    
+PD_STRING = {dt.datetime: 'datetime64[ns]',
+             np.datetime64: 'datetime64[ns]',
+             pd.Timestamp: 'datetime64[ns]',
+             dt.timedelta: 'timedelta64[ns]',
+             np.timedelta64: 'timedelta64[ns]',
+             pd.Timedelta: 'timedelta64[ns]',}
+
+
+
+TYPES = ('type','function','module')
+_TYPES = tuple([cls for cls in object.__subclasses__() if cls.__name__ in TYPES])
+
+DEFAULT_ARGUMENTS = {dt.date: [(0,0,0),{}],
+                     dt.datetime: [(0,0,0),{}],
+                     dt.timedelta: [(0,),{}]}
+
+DO_NOT_CALL_BY_DEFAULT = (dt.date, dt.datetime, dt.timedelta)
+
+#may contain dicts of instructions; later are packed into list([inited])/tuple([inited])
+#if e.g np.ndarray is preferred, must use {'_type_': np.ndarray, '_call_': np.asarray, 'value'/'_value_': [..instructions..], _kw={'dtype': x}} instead
+HANDLEABLES = (list, tuple, set) #?? does `set` belong here?
+
+IMMUTABLES = (int, float, str, bool, tuple, type(None))
+CONTAINERS = (dict, list, tuple, set, pd.Series, pd.DataFrame, pd.Index, np.ndarray)
+COPY_METHOD = (pd.DataFrame, pd.Series, pd.DatetimeIndex, pd.Index, np.ndarray)
+
+
+RESERVED = ('_type_', '_call_', '_value_', '_multival_', '_defval_', '_copy_', '_isnorm_', '_multi_', '_vfy_')
+NORM_EXTRA = {'_type_':str,
+              '_value_': '_keep_'}
+
+
+def _map(item, *default, **kw):
+    if not isinstance(item, str):
+        if kw.get('pd_dtype'):
+            return _map_pd_dtype(item)
+        return item
+    
+    obj = None
+    
+    if item in MAP:
+        obj = MAP[item]
+    elif __name__ == '__main__':
+        obj = getattr(__builtins__, item, None)
+    else:
+        obj = __builtins__.get(item, None)
+    
+    obj_t = (obj,) if not isinstance(obj, tuple) else obj
+    
+    if any(x is None or type(x).__name__ not in TYPES for x in obj_t):
+        if not len(default):
+            raise BadInstruction('Item {} not known.'.format(item))
+        else:
+            return default[0]
+    
+    if kw.get('pd_dtype'):
+        obj = _map_pd_dtype(obj)
+    
+    #if isinstance(obj,str) and obj != 'datetime64[ns]': raise OSError(obj)
+    
+    return obj
+
+
+def _map_pd_dtype(obj):
+    try:
+        obj = PD_STRING.get(obj, obj)
+    except TypeError:
+        pass
+    return obj
+
+
+def _isinstructions(x):
+    if isinstance(x, Element):
+        return True
+    elif not isinstance(x, dict):
+        return False
+    elif not any(k in RESERVED for k in x.keys()):
+        return False
+    
+    return True 
+
+
+def _isnorm(x):
+    if isinstance(x, dict):
+        return bool(x.get('_isnorm_'))
+    elif isinstance(x, Element):
+        return bool(getattr(x, 'isnorm', False))
+    
+    return False
+
+#---------------------
+
+def normalize(data):
+    init_data(data)
+    normalized = normalize_element(data)
+    
+    return normalized
+
+
+def fill(x, norm, **kw):
+    return verify_data(x,norm,mode='fill',**kw)
+
+#----------------------------------------
+
+def init_data(x, copy=True):
+    obj = None
+    _type = type(x)
+    _name = _type.__name__
+    
+    if issubclass(_type, Element):
+        x = x.to_dict()
+        _type = dict
+    
+    if issubclass(_type, dict):
+        obj = _init_from_dict(x)
+        if copy: obj = _copy(obj)
+    
+    elif _type not in HANDLEABLES:
+        if copy: obj = _copy(x)
+        else: obj = x
+
+    else:
+        #isinstr = any(_isintruction(y) for y in x)
+        #may still contain instructions at a sub-level
+        alist = [init_data(y, copy=copy) for y in x]
+      
+        try:
+            call = _map(_name)
+            obj = call(alist)
+                
+        except ValueError:
+            obj = alist
+            
+        except Exception:
+            traceback.print_exc()
+            obj = alist
+        
+    return obj
+
+
+
+def _init_from_dict(D, copy=True):
+    add_to = {}
+    if _isinstructions(D):
+        return _init_instructions(D, copy=copy)
+    
+    #initiating its values (plus making copy of the dict)
+    for n,v in D.items():
+        obj = init_data(v, copy=copy)
+        add_to[n] = obj
+        #keys are always? immutable, no need to copy
+    
+    return add_to 
+
+
+
+def _init_instructions(D, copy=True):
+    normalize_element(D)
+    
+    if '_copy_' in D:
+        if copy:
+            return _copy(D['_copy_'])
+        else:
+            return D['_copy_']
+    
+    _type_ = D.get('_type_')
+    
+    if isinstance(_type_, tuple):
+        _type0_ = _type_[0]
+    else:
+        _type0_ = _type_
+    
+    
+    if '_defval_' in D:
+        return init_data(D['_defval_'], copy=copy)
+    
+    elif '_multi_' in D:
+        return init_data(D['_multi_'][0], copy=copy)
+    
+    elif _type0_ in _TYPES:
+        #return _map(D.get('_value_'))
+        return D.get('_value_')
+    
+    elif '_value_' in D:
+        D['_copy_'] = _copy(D['_value_'])
+        return _init_instructions(D, copy=copy)
+    
+    elif '_multival_' in D:
+        D['_copy_'] = _copy(D['_multival_'][0])
+        return _init_instructions(D, copy=copy)
+    
+    
+    return _init_by_call(_type0_, D, copy=copy)
+    
+
+
+def _init_by_call(_type_, D, copy=True):
+    
+    _call0_ = D.get('_call_',nan)
+
+    if is_given(_call0_):
+        if is_null(_call0_):
+            return nan
+            #raise BadInstruction('Wrong _call_: {}'.format(_call0_))
+    elif is_null(_type_):
+        #return nan
+        raise BadInstruction('_type_ is null')
+    
+
+    #_value_ is used for not using _call_() or _type_() 
+    
+    args,kw,_call2_ = [],{},_type_
+    
+    """if is_null(D.get('args')) and is_null(D.get('kwargs')) and \
+            _type_ in DO_NOT_CALL_BY_DEFAULT:
+        return nan"""
+        
+    
+    if isinstance(D.get('args'),(list,tuple)):
+        args = init_data(D['args'])
+    
+    if isinstance(D.get('kwargs'),dict):
+        kw = init_data(D['kwargs'])
+    
+
+    if is_given(_type_) and (not len(args) or not len(kw)): #??
+        args2,kw2,_call2_ = _known_types(_type_, D, copy=copy)
+        if not len(args):
+            args = args2
+        kw2.update(kw)
+        kw = kw2
+
+
+    if is_given(_call0_): 
+        _call_ = _call0_
+    else: 
+        _call_ = _call2_
+            
+    #print(_type.__name__,'args:',args,'kw:',kw)
+    obj = _call_(*args,**kw)
+    
+    
+    D['_copy_'] = _copy(obj)
+
+    return obj
+
+
+
+def _known_types(_type_, D, copy=True):
+    
+    #vname = vtype.__name__
+    args = []
+    kw = {}
+    call = _type_
+    
+    
+    if issubclass(_type_, (pd.Series, pd.DataFrame)):
+        data = init_data(D.get('data'),copy=False)
+        index = init_data(D.get('index'),copy=False)
+        dtype = MAP.get(D.get('dtype'))
+        
+        name = init_data(D.get('name'),copy=False)
+        columns = init_data(D.get('columns'),copy=False)
+        dtypes = D.get('dtypes')
+        
+        if _type_ is pd.DataFrame:
+            if dtypes:
+                if not isinstance(data,dict):
+                    data = OD([[c,pd.Series(data, index=index, dtype=_map(d,None,pd_dtype=True))] for c,d in D['dtypes'].items()])
+                else:
+                    data = OD([[c,pd.Series(data.get(c), index=index, dtype=_map(d,None,pd_dtype=True))] for c,d in D['dtypes'].items()])
+            
+                if not columns:
+                    D['columns'] = list(dtypes.keys())
+            
+            kw.update({'data':data,'index':index,'columns':columns,'dtype':dtype})
+        
+        else:
+            kw.update({'data':data,'index':index,'name':name,'dtype':dtype})
+    
+    
+    elif issubclass(_type_, dict):
+        new_d = {}
+        items = []
+        
+        if is_not_null(D.get('items', nan)):
+            items = D['items']
+            if isinstance(items,dict):
+                items = list(items.items())
+        
+        elif is_not_null(D.get('keys', nan)):
+            keys = D['keys']
+            if 'values' in D:
+                values = D['values']
+            elif 'value' in D or 'v' in D:
+                values = [D.get('value',D.get('v'))] * len(keys)
+            else:
+                values = [D.get('unit')] * len(keys)
+            
+            items = list(zip(keys,values))
+        
+        new_d = init_data(items, copy=copy)
+        args.append(new_d)
+        
+        if True:
+            D['keys'] = [itm[0] for itm in new_d]
+            #For being able to verify_data later (itm[1] -> {'_type_':type(itm[1]),_value_: itm[1])}
+            items = [[itm[0],normalize_element(itm[1])] for itm in items]
+            D['items'] = items #the instr dicts in items have been normalized due to init_data(items)
+            init_data(D.get('unit'), copy=False) #??
+    
+    
+    elif issubclass(_type_, dt.datetime):
+        value = D.get('value', D.get('v'))
+        
+        if isinstance(value,str):
+            args.append(value)
+            
+            if D.get('format'):
+                call = dt.datetime.strptime
+                args.append(D['format'])
+            else:
+                call = parsedate
+        
+        elif isinstance(value, dt.datetime):
+            args.extend([value.year, value.month, value.day, value.hour,
+                         value.minute, value.second, value.microsecond])
+        
+        elif isinstance(value,(list,tuple)):
+            args.extend(value)
+        
+        elif isinstance(value,(int,float)):
+            call = dt.datetime.utcfromtimestamp
+            args.append(value/1000)
+        
+        else:
+            raise BadInstruction(_type_, D, value)
+    
+    
+    elif issubclass(_type_, dt.timedelta):
+        value = D.get('value', D.get('v'))
+        
+        if isinstance(value,(list,tuple)):
+            args.extend(value)
+            
+        elif isinstance(value,(int,float)):
+            #microseconds
+            args.extend([0,0,value*1000])
+            
+        else:
+            raise BadInstruction(_type_, D, value)  
+    
+    
+    elif issubclass(_type_, (list,tuple,set)):
+        value = D.get('value', D.get('values', D.get('v', nan)))
+        _range = D.get('range', nan)
+        size = D.get('size', nan)
+        
+        if is_not_null(value):
+            args.append(init_data(value, copy=copy))
+            """if is_null(size):
+                D['size'] = {'==': (len(value),)}"""
+        
+        elif is_not_null(_range) and not isinstance(_range, str):
+            arange = list(range(*_range)) #np.arange(*range)
+            args.append(arange)
+            """if not is_not_null(size):
+                D['size'] = {'==': (len(arange),)}"""
+            
+            if not is_given(value):
+                D['value'] = arange
+            
+            init_data(D.get('unit'), copy=False) #??
+    
+    
+    elif issubclass(_type_, (str,int,float)):
+        value = D.get('value', D.get('v'))
+        if is_not_null(value):
+            args.append(init_data(value))
+            D['_value_'] = args[-1]
+            #del D['value']
+        elif issubclass(_type_, (int, float)) and isinstance(D.get('range'), str):
+            limit0, limit1 = D['_range']
+            if None not in D['_range']:
+                args.append((limit0 + limit1) / 2)
+            elif limit0 is not None:
+                args.append(limit0)
+            elif limit1 is not None:
+                args.append(limit1)
+    
+    else: 
+        pass #args.append(init_data(_type_))
+    
+    #print('args_now:',args)    
+    
+    return args, kw, call
+
+
+
+#--------------------------------------------
+
+def normalize_element(x, default=nan):
+    if _isnorm(x): return x
+    
+    #the corresponding keys' values are treated as literal (if they are present in the x):
+    # _defval_, _value_, value, unit, 
+    #_call_  :: return _value_/_multival,_defval_ if those present; 
+    #            otherwise if _call_ in (None, _nan_ ): return None, else _call_(args), 
+    #                and if not given _call_ = _type_. or return None if not is_not_null(_type_)
+    
+    x_initial = x
+    is_element = isinstance(x, Element)
+    if is_element:
+        x = x.to_dict()
+    
+    if _isinstructions(x):
+        d = x
+        _normalize_type(d)
+    else:
+        d = {'_type_': type(x),
+             '_value_': x}
+        
+    _normalize_defval(d, default)
+    
+    _normalize_multi(d)
+    
+    _normalize_value(d)
+
+    _normalize_call(d)
+        
+    _normalize_size(d)
+    _normalize_range(d)
+    
+    _normalize_unit(d)
+    
+    _normalize_dtypes(d)
+    _normalize_opt_req(d)
+    
+    _normalize_vfy(d)
+    
+    _type_ = d.get('_type_',nan)
+    if is_given(_type_):
+        if isinstance(_type_, tuple):
+            _type_ = _type_[0]
+        
+        if not issubclass(_type_, (dt.datetime, dt.timedelta)):
+            _known_types(_type_, d, copy=False)
+    
+    d['_isnorm_'] = True
+    
+    if is_element:
+        x_initial.update(d, normalize=False)
+        return x_initial
+    
+    return d
+
+
+def _normalize_type(d):
+    _type_ = d.get('_type_')
+        
+    if is_null(_type_):
+        d.pop('_type_',-1)
+        return
+            
+    if isinstance(_type_, MAP['listlike']):
+        _type_ = tuple((_map(t) for t in _type_))
+    else:
+        _type_ = _map(_type_)
+    
+    if isinstance(_type_, tuple):
+        for t in _type_:
+            _verify_is_type(t)
+    else:
+        _verify_is_type(_type_)
+    
+    d['_type_'] = _type_
+
+
+def _normalize_defval(d, default):
+    if default is not nan:
+        d['_defval_'] = normalize_element(default)
+    elif '_defval_' in d:
+        d['_defval_'] = normalize_element(d['_defval_'])
+
+
+def _normalize_multi(d):
+    _multi_ = d.get('_multi_',nan)
+    if is_null(_multi_): 
+        d.pop('_multi_', -1)
+    elif isinstance(_multi_, MAP['listlike']):
+        if len(_multi_):
+            _multi_ = list(_multi_)
+            for i,d2 in enumerate(_multi_):
+                _multi_[i] = normalize_element(d2)
+                init_data(_multi_[i], copy=False)
+        else:
+            del d['_multi_']
+    else:
+        raise BadInstruction('Defective "_multi_": {}'.format(_multi_))
+
+
+def _normalize_value(d):
+    if _isinstructions(d.get('_value_')):
+        d['_value_'] = init_data(d['_value_'], copy=False)
+    
+    has_type_key = '_type_' in d
+    _type_ = d.get('_type_')
+    
+    add_types = []
+    sub_allowed = d.get('sub', d.get('sub_allowed')) is not False
+    
+    #Value can be anything but fons.nan.nan
+    if '_value_' in d and not is_given(d['_value_']):
+        d.pop('_value_',-1)
+    
+    _value_ = d.get('_value_')
+    
+    if '_value_' in d:
+        if is_not_null(_value_) and has_type_key:
+            d['_value_'] = _map_value_if_str(_type_, _value_)
+            
+        add_types.append(type(d['_value_']))
+        
+        
+    _multival_ = d.get('_multival_',nan)
+    if is_null(_multival_):
+        d.pop('_multival_',-1)
+    elif isinstance(_multival_, MAP['listlike']):
+        if len(_multival_):
+            inited = [init_data(v, copy=False) for v in _multival_]
+            multival = [_map_value_if_str(_type_, v) 
+                            if has_type_key and is_not_null(v) else 
+                        v for v in inited]
+            add_types += [type(x) for x in multival]
+            if '_value_' in d:
+                multival.insert(d['_value_'], 0)
+                del d['_value_']
+            d['_multival_'] = multival
+        else:
+            del d['_multival_']
+    else:
+        raise BadInstruction('Defective "_multival_": {}'.format(_multival_))
+    
+    
+    if add_types:
+        types = ((_type_,) if not isinstance(_type_, tuple) else _type_)  if has_type_key else ()
+        for x in add_types:
+            if not types : pass
+            elif sub_allowed and not issubclass(x, types): pass
+            elif not sub_allowed and x not in types: pass
+            else: continue
+            types += (x,)
+        
+        if types:
+            d['_type_'] = types if len(types) > 1 else types[0]
+
+
+def _map_value_if_str(_type_, _value_):
+    if is_null(_type_):
+        return _value_
+    #to map e.g {'_type_: type, '_value_': 'list'} to {'_value_': list} 
+    # for (normalized) init and compare purposes
+    t_types = _type_ if isinstance(_type_,tuple) else (_type_,)
+    if isinstance(_value_, str) and not any(issubclass(t,str) for t in t_types):
+        return _map(_value_)
+    else:
+        return _value_
+
+
+def _normalize_call(d):
+    if '_call_' not in d: pass
+    elif is_not_null(d['_call_']): #??
+        d['_call_'] = _map(d['_call_'])
+
+
+def _normalize_size(d):
+    size = _size = d.get('size', nan)
+    if is_null(size):
+        d.pop('size', -1)
+    elif not isinstance(size, (int, dict, str)):
+        raise BadInstruction('"size" must be int/dict/str; got: {}'.format(type(size)))
+    elif isinstance(size, int):
+        d['size'] = {'exact': size}
+    elif isinstance(size, str):
+        _range = _parse_str_range(size, num_type=int)
+        _min = max(0, _range[0] if size.startswith('[') else _range[0]+1) if _range[0] is not None else None
+        _max = max(0, _range[1] if size.endswith(']') else _range[1]-1) if _range[1] is not None else None
+        d['size'] = {'min': _min, 'max': _max}
+    
+    size = d.get('size', nan)
+    if is_not_null(size):
+        for k in ('min','max','exact'):
+            value = size.get(k)
+            if is_null(value):
+                size.pop(k, -1)
+            elif not isinstance(value, int):
+                raise BadInstruction('"size" keyword "{}" must be of type <int>; got: {}; size: {}'.format(k, type(value), _size))
+            elif value < 0:
+                raise BadInstruction('"size" keyword "{}" must be >= 0; got: {}; size: {}'.format(k, value, _size))
+        _min, _max, _exact = size.get('min'), size.get('max'), size.get('exact')
+        if _min is not None and _max is not None and _min > _max:
+            raise BadInstruction('"size" keyword "min" < "max" is not satisfied; size: {}'.format(_size))
+        if _min is not None and _exact is not None:
+            raise BadInstruction('"size" must not have both "min" and "exact" keywords; size: {}'.format(_size))
+        if _max is not None and _exact is not None:
+            raise BadInstruction('"size" must not have both "max" and "exact" keywords; size: {}'.format(_size))
+
+
+def _parse_number(x, num_type=float):
+    if not x or x=='null':
+        return None
+    try: 
+        return num_type(x)
+    except ValueError:
+        return '?'
+
+
+def _parse_str_range(range, num_type=float):
+    first, middle, last = range[:1], range[1:-1], range[-1:]
+    _range = tuple(_parse_number(x.strip(), num_type) for x in middle.split(','))
+    correct = '?' not in _range
+    all_num = all(isinstance(x, num_type) for x in _range)
+    if not range or first not in '[(' or last not in '])' or len(_range)!=2 or not correct \
+            or all_num and _range[0]>_range[1]:
+        raise BadInstruction('Not understood {} range: {}'.format(num_type.__name__, range))
+    return _range
+
+
+def _normalize_range(d):
+    range = d.get('range',nan)
+    if is_null(range):
+        d.pop('range',-1)
+    # range for verifying int/float
+    elif isinstance(range,str):
+        d['_range'] = _parse_str_range(range)
+    # range for list/tuple/set initiation
+    elif isinstance(range,int):
+        d['range'] = (0,range)
+    elif not isinstance(range, MAP['listlike']):
+        raise BadInstruction('Wrong type for "range": {}'.format(type(range)))
+    elif len(range) != 2:
+        raise BadInstruction('Wrong size for "range": {}'.format(len(range)))
+    elif not isinstance(range[0],int) or not isinstance(range[1],int):
+        raise BadInstruction('"range" contains non-int type: {}'.format([type(y) for y in range]))
+
+
+def _normalize_unit(d):
+    if 'unit' in d:
+        d['unit'] = normalize_element(d['unit'])
+        init_data(d['unit'], copy=False)
+
+
+def _normalize_dtypes(d):
+    dtypes = d.get('dtypes', nan)
+    if is_null(dtypes):
+        if 'dtypes' in d:
+            del d['dtypes']
+        return
+    if is_null(d.get('_type_', nan)):
+        raise BadInstruction('_type_ must be given if "dtypes" is defined; d: {}'.format(d))
+    _type = _map(d['_type_'])
+    if not isinstance(_type, tuple):
+        _type = (_type,)
+    for_dict = any(issubclass(x, dict) for x in _type)
+    for_pandas = any(issubclass(x, (pd.Series, pd.DataFrame)) for x in _type)
+    items = []
+    default_dtype = d.get('default_dtype', None)
+    
+    if not isinstance(dtypes,dict):
+        d['dtypes'] = dtypes = OD(dtypes)
+    
+    for k,v in dtypes.items():
+        if not _isinstructions(v):
+            dd = {'_type_': _map(v, pd_dtype=for_pandas)}
+            normalize_element(dd, default=default_dtype)
+        else: 
+            dd = v #normalize_element(v) #don't use default=v, inf recursion
+        
+        if for_pandas:
+            if isinstance(dd, Element):
+                dd = dd.to_dict()
+            _type_ = dd.get('_type_')
+            _type_mapped = _map(_type_, pd_dtype=True)
+            if is_null(_type_) or not isinstance(_type_mapped, (type, str)):
+                raise BadInstruction('Pandas dtype _type_ is invalid: /k: v/: {}: {} || type(v): {}'.format(k, v, type(v)))
+            dtypes[k] = _type_mapped
+        
+        if for_dict:
+            items.append([k, dd])
+    
+    if for_dict and is_null(d.get('items',nan)):
+        d['items'] = items
+
+
+def _normalize_opt_req(d):
+    # all keys that aren't in required (if given) are optional
+    # use 'required' if nearly all keys are optional
+    aliases = {
+        'optional': ['opt','optional','keys_optional'],
+        'required': ['req','required','keys_required'],
+    }
+    for key, aliases in aliases.items():
+        final = nan
+        for alias in aliases:
+            value = d.pop(alias, nan)
+            if is_null(value):
+                pass
+            elif not isinstance(value, MAP['listlike']+(dict,)):
+                raise BadInstruction('Wrong type for "{}": {}'.format(alias, type(value)))
+            elif final is not nan:
+                raise BadInstruction('Got multiple values for {}'.format(key))
+            else:
+                final = value
+        if is_not_null(final):
+            d[key] = final
+
+
+def _normalize_vfy(d):
+    _vfy_ = d.get('_vfy_', nan)
+    if is_null(_vfy_):
+        d.pop('_vfy_', -1)
+    elif not hasattr(_vfy_, '__call__'):
+        raise BadInstruction('_vfy_ must be callable, d: {}'.format(d))
+
+
+#-------------------------------------
+#type - error/warn/ignore/fix/fix+
+#value - error/warn/ignore/fix/fix+
+#//use-this for (list-e, dict-e):
+#missing - error/warn/ignore/fix/fix+
+#extra - error/warn/ignore/fix/fix+
+
+#//explanation: 
+#fix - replace (existing), add (missing) with newly initiated element, if its _call_ is not None or value is specified, otherwise raise error;
+#    - delete (extra element)
+#fix- - fix and DON'T warn
+
+#///too-complicated:
+#list_e - {'missing': error/warn/ignore/fix/fix+,
+#           'extra': error/warn/ignore/fix/fix+,
+#           'value': error/warn/ignore/fix/fix+}
+#dict_e - {'missing': error/warn/ignore/fix/fix+,
+#           'extra': error/warn/ignore/fix/fix+,
+#           'value': error/warn/ignore/fix/fix+}
+
+#copy:
+# 'fix_mode' - the object (x) is copied only if any of the handler modes is set to 'fix'/'fix-'
+# True - obj is always copied
+# False - obj is modified inplace, if mode == 'fix/fix-'
+#         however some defective objects are still "copied" in these cases:
+#             - type mismatch between the obj and norm
+#             - the obj is immutable
+#             - copying it/making new one is considerably faster than modifying inplace (eg adding dataframe missing columns one by one)
+#         therefore user should always overwrite x = verify_data(x), and still update all the references
+
+
+_MODES = ('error','warn','ignore','fix','fix-')
+_ERROR_MODES = ('error',)
+_FIX_MODES = ('fix','fix-')
+_WARN_MODES = ('warn','fix')
+
+_HANDLER_KEYS = ('type','value','key','index','general')
+_H_OBJ_KEYS = ('type','value','general')
+_H_CONTAINER_KEYS = ('key','index')
+_H_CONTAINER_OPTIONS = ('missing','extra')
+
+
+def verify_data(x, norm, mode='error', copy=False, **kw):
+    if copy:
+        x = _copy(x)
+    copy = False
+    
+    if not _isnorm(norm):
+        norm = normalize_element(norm)
+        init_data(norm, copy=False)
+    
+    if isinstance(norm, Element):
+        norm = norm.to_dict()
+    
+    kw.update({'mode': mode})#, 'copy': copy})
+    norm_extra = kw.get('norm_extra', nan)
+    trace = kw.get('trace',[])
+    
+    _verify_input_args(kw)
+    handler = kw['handler']
+    #copy = kw['copy']
+
+    x_ver = x
+    
+    if is_not_null(norm_extra):
+        try: 
+            verify_data(x_ver, norm_extra, 'error', trace=trace)
+            #if _isinstructions(kw['norm_extra']): verify_data(x_ver,norm_extra,**kw)
+            #else: verify_data(x_ver,normalize_element({},default=norm_extra),**kw)
+        except Exception: 
+            pass
+        else: 
+            return x_ver #passed[:] = True
+        
+    
+    _defval_ = norm.get('_defval_', nan)
+    sub_allowed = norm.get('sub', norm.get('sub_allowed')) is not False
+    
+    if is_not_null(_defval_): 
+        if _verify_defval(x_ver, _defval_, sub_allowed=sub_allowed):
+            return x_ver
+    
+    
+    _multi_ = norm.get('_multi_', nan)
+    
+    if is_not_null(_multi_) and len(_multi_):
+        return _verify_multi(x_ver, _multi_, mode, trace, handler, copy)
+    
+    
+    #---------------------------------------------------------------
+    #---------------------------------------------------------------
+    _type = type(x)
+    t_name = _type.__name__
+    len_trace = len(trace)
+    trace2 = trace + ['({}){}'.format(len_trace, t_name)]
+    
+    if not len_trace and copy:
+        x_ver = init_data(x, copy=True) #done many times if _multi_ specified
+    else:
+        x_ver = x
+    
+    passed = pd.Series(True, ['type','value','range','vfy'])
+    
+    
+    #-type-
+    normtype = norm.get('_type_', nan)
+    
+    if is_not_null(normtype):
+        r = _verify_type(_type, normtype, sub_allowed)
+        if r is not True: 
+            _handle_error(handler, 'type', [trace2, t_name, r])
+            passed.type = False
+    
+    
+    #-value-
+    has_value = '_value_' in norm
+    _multival_ = norm.get('_multival_', nan)
+    
+    if has_value:
+        _value_ = norm.get('_value_')
+        passed.value = compare(x_ver, _value_, type_op='ignore')
+        if not passed.value:
+            _handle_error(handler, 'value', [trace2, x_ver, _value_])
+    
+    elif is_not_null(_multival_):
+        passed.value = any(compare(x_ver, val, type_op='ignore') for val in _multival_)
+        if not passed.value:
+            _handle_error(handler, 'value', [trace2, x_ver, _multival_])
+    
+    else:
+        try: iter(x_ver)
+        except TypeError: pass
+        else: 
+            x_ver = _verify_elements(x_ver, norm, mode, trace2, handler, copy)
+    
+    
+    #-range-
+    range = norm.get('range')
+    if isinstance(x_ver, (int, float)) and is_not_null(range) and isinstance(range, str):
+        passed.range = _verify_in_range(x_ver, norm)
+        if not passed.range:
+            _handle_error(handler, 'value', [trace2, x_ver, 'in range: {}'.format(range)])
+    
+    
+    _vfy_ = norm.get('_vfy_')
+    if is_not_null(_vfy_) and passed.all():
+        try: _vfy_(x_ver)
+        except Exception as e:
+            passed.vfy = False
+            e_type, e_args = _parse_user_error(e, trace2, x_ver)
+            _handle_error(handler, e_type, e_args)
+    
+    
+    if not passed.all():
+        x_ver = init_data(norm)
+    
+    
+    return x_ver
+
+
+def _verify_defval(x, _defval_, **kw):
+    _type = type(x)
+    try:
+        _type1 = _defval_['_type_']
+    except Exception as e:
+        print(x, _defval_, kw)
+        raise e
+    _type1a = EQUALS.get(_type1) if not isinstance(_type1,tuple) else tuple((EQUALS.get(t2) for t2 in _type1))
+    
+    correct_types = _flatten_types(_type1, _type1a)
+    sub_allowed = _defval_.get('sub', _defval_.get('sub_allowed'))
+    defval_sub_allowed = False if sub_allowed is False else kw.get('sub_allowed',True)
+    
+    r = _verify_type(_type, correct_types, sub_allowed=defval_sub_allowed)
+    
+    if r is not True: pass
+    elif not compare(x, init_data(_defval_, copy=False), type_op='ignore'): pass
+    #print('Compare UNSUCCESSFUL! {} {}'.format(x,_defval_)
+    else: return True
+    
+    return False
+
+
+def _verify_multi(x, _multi_, mode, trace, handler, copy=False):
+    exceptions = []
+    passed = False
+    x_ver = _null = object()
+    
+    for norm in _multi_:
+        try:
+            x_ver = verify_data(x, norm, 'error', trace=trace)
+            passed = True
+        except VeriError as e:
+            exceptions.append(e)
+        else:break
+    
+    if not passed:
+        dx = _handle_error(handler, exceptions) #may raise (if deepest lvl error's mode in handler is 'error')
+        is_fix = dx['is_fix']
+        
+        if is_fix: 
+            most_similar_norm = _multi_[dx['i']] #i is the index of the first deepest level error
+            x_ver = verify_data(x, most_similar_norm, mode, copy, trace=trace, handler=handler)
+ 
+        #A drawback of singling out -> _multi: [{'_type_:xr}, {'_type_':x}] only shows the first e msg
+        #raise VeriError('Verification failed. The following exceptions occurred: {}'.format(exceptions))
+    
+    if x_ver is _null:
+        x_ver = x if not copy else _copy(x)
+    
+    return x_ver
+
+
+def _verify_in_range(x, norm):
+    range = norm['range']
+    limit0, limit1 = norm['_range']
+    
+    if limit0 is not None:
+        result0 = limit0 <= x if range[0]=='[' else limit0 < x
+        if not result0:
+            return False
+    
+    if limit1 is not None: 
+        result1 = x <= limit1 if range[-1]==']' else x < limit1
+        if not result1:
+            return False
+    
+    return True
+
+#-------------------------------------------------------------
+    
+def _verify_elements(x, norm, mode, trace, handler, copy=False):
+    pdlike = (pd.Series, pd.DataFrame)
+    _check_size(x, norm, trace, handler)
+
+    if isinstance(x, dict):
+        x_ver = _verify_dict(x, norm, mode, trace, handler, copy)
+
+    elif isinstance(x, pdlike):
+        x_ver= _verify_pandaslike(x, norm, mode, trace, handler, copy) 
+            
+    else: #if isinstance(x,(list,tuple,set)) or is_iterable:
+        x_ver = _verify_listlike(x, norm, mode, trace, handler, copy)
+
+                          
+    return x_ver
+
+
+def _verify_dict(x, norm, mode, trace, handler, copy=False):
+    fix_vals = handler['type'] in _FIX_MODES or handler['value'] in _FIX_MODES
+    
+    unit = norm.get('unit',nan)
+    extra_allowed = norm.get('extra_allowed')
+    keys_opt = norm.get('optional',[])
+    keys_req = norm.get('required',nan)
+    
+    nitems = norm.get('items')
+    
+    if nitems:
+        nkeys = [itm[0] for itm in nitems]
+        me = _verify_keys(x.keys(), nkeys, trace, handler, keys_opt, keys_req, extra_allowed)
+        
+        if handler['key']['missing'] in _FIX_MODES and len(me['missing_all']):
+            #messes up order if OD
+            n_inited = init_data(norm,copy=False)
+            #if len(missing): print(trace,'missing:',missing)
+            x.update({_copy(k):_copy(v) for k,v in n_inited.items() if k in me['missing_all']})
+            
+        for nk,nv in nitems:
+            if nk in me['missing_all']:continue
+            trace2 = trace[:-1] + [''.join(trace[-1:]) + '({})(key){}'.format(len(trace),nk)]
+            xv = verify_data(x[nk], nv, mode, trace=trace2, handler=handler)
+            if fix_vals: x[nk] = xv
+        
+        if handler['key']['extra'] in _FIX_MODES and len(me['extra']):
+            for ke in me['extra']:
+                x.pop(ke)
+
+    if is_not_null(unit):
+        for k,v in x.items():
+            trace2 = trace[:-1] + [''.join(trace[-1:]) + '({})(key){}'.format(len(trace),k)]
+            xv = verify_data(v, unit, mode, trace=trace2, handler=handler)
+            if fix_vals: x[k] = xv
+             
+    return x
+
+
+def _verify_pandaslike(x, norm, mode, trace, handler, copy=False):
+    unit = norm.get('unit',nan)
+    extra_allowed = norm.get('extra_allowed')
+    keys_opt = norm.get('optional',[])
+    keys_req = norm.get('required',nan)
+    
+    is_series = isinstance(x,pd.Series)
+    is_df = isinstance(x,pd.DataFrame)
+    
+    ndtype0 = norm.get('dtype',nan)
+    ndtypes = norm.get('dtypes',nan)
+    #dtypes = x.dtypes
+    inplace = not(copy)
+    
+    wrong_dtypes = []
+    dtypes = x.dtypes.iteritems() if is_df else [(x.name,x.dtype)]
+    
+    for c,itm in dtypes:
+        dtype = _map(itm.name, pd_dtype=True)
+        if is_not_null(ndtype0):
+            ndtype = ndtype0 
+        elif is_not_null(ndtypes) and c in ndtypes:
+            ndtype = ndtypes[c]
+        else: continue
+        
+        #both may be strings (datetime64[ns])
+        #however. int may be float
+        if dtype != ndtype and dtype is not PD_EQUALS.get(ndtype):
+            wrong_dtypes.append({c:(dtype,ndtype)})
+     
+    nr_wrong = len(wrong_dtypes)    
+            
+    if nr_wrong:
+        trace2 = trace + ['({})(dtypes)'.format(len(trace))]
+        _handle_error(handler, 'type', [trace2, wrong_dtypes])
+            
+    if nr_wrong and handler['type'] in _FIX_MODES:
+        for c, tpl in wrong_dtypes:
+            dtype,ndtype = tpl
+            try:
+                if is_df: x[c] = x[c].astype(ndtype)
+                else: x = x.astype(ndtype)
+            except Exception as e:
+                logging.exception(e)
+            
+            
+    ncols = norm.get('columns')
+    nindex = norm.get('index')
+    
+    _keys = ('missing','extra','missing_all','extra_all')
+    me_cols = {_k: [] for _k in _keys}
+    me_ind = {_k: [] for _k in _keys}
+    
+    if isinstance(keys_opt,dict):
+        index_opt = keys_opt.get('index')
+        cols_opt = keys_opt.get('columns')
+    else: index_opt = cols_opt = []
+    
+    if isinstance(keys_req,dict):
+        index_req = keys_req.get('index')
+        cols_req = keys_req.get('columns')
+    else: index_req = cols_req = nan
+    
+    if isinstance(extra_allowed,dict):
+        ea_index = extra_allowed.get('index')
+        ea_cols = extra_allowed.get('columns')
+    else: ea_index = ea_cols = extra_allowed
+    
+    if is_df and ncols is not None:
+        me_cols = _verify_keys(x.columns, ncols, trace, handler, cols_opt, cols_req, ea_cols)
+        
+    if nindex is not None:
+        me_ind = _verify_keys(x.index, nindex, trace, handler, index_opt, index_req, ea_index)
+    
+    if handler['key']['missing'] not in _FIX_MODES: pass
+    elif len(me_ind['missing']) or len(me_cols['missing']):
+        x_new = init_data(norm)
+        if not inplace: #much faster
+            if is_series: x_new.loc[x.index] = x
+            else: x_new.loc[x.index,x.columns] = x  #(this doesn't link the old x's values with x_new)
+            x = x_new
+    
+        else:
+            for c in me_cols['missing']:
+                pos = next((j for j in ncols if j == c),x.shape[1])
+                x.insert(pos, c, x_new[c])
+                
+            if is_df:
+                for i in me_ind['missing']:
+                    pos = next((j for j in nindex if j == i),x.shape[0])
+                    x.insert(pos, i, x_new.loc[i,:],axis=1)
+            else:
+                for i in me_ind['missing']:
+                    x[i] = x_new[i]
+
+        
+    if handler['key']['extra'] in _FIX_MODES:
+        if len(me_ind['extra']): 
+            if inplace: x.drop(me_ind['extra'], inplace=True)
+            else: x = x.drop(me_ind['extra'])
+        if len(me_cols['extra']):
+            if inplace: x.drop(me_cols['extra'], axis=1, inplace=True)
+            else: x = x.drop(me_cols['extra'], axis=1)
+          
+    return x
+            
+     
+             
+def _verify_listlike(x, norm, mode, trace, handler, copy=False):
+    if isinstance(x, set):
+        new = _verify_set_elements_by_nvalue(x, norm, mode, trace, handler)
+    else:
+        new = _verify_list_elements_by_nvalue(x, norm, mode, trace, handler)
+    
+    unit = norm.get('unit', nan)
+                  
+    if is_not_null(unit):
+        new = [verify_data(v, unit, mode, trace=trace, norm_extra=NORM_EXTRA, handler=handler)
+                for v in new]
+            
+    #if only unit is given, and e.g `unit = {'_type_': dt, '_call_': None}`, `mode = 'fill'` doesn't replace the wrong values with None
+    #(mode 'fill' does and will only work for *missing* data, with either _dict_ attr present, or listlike with endings capped)
+    
+    if is_not_null(new): #and any(m in _FIX_MODES for m in handler.values()):
+        #deepcopy norm_new?
+        norm_new = {k: norm[k] for k in norm if k not in ('_copy_',)}
+        norm_new.update({'values': new}) #,'_value_':None})
+        x = init_data(norm_new)
+    
+    return x
+
+
+def _verify_set_elements_by_nvalue(x, norm, mode, trace, handler):
+    extra_allowed = norm.get('extra_allowed')
+    nvalue = norm.get('value', norm.get('values', norm.get('v', nan)))
+    if is_null(nvalue):
+        return x
+    
+    missing = set(_ for _ in nvalue if _ not in x)
+   
+    if not missing: pass
+    elif handler['index']['missing'] in _FIX_MODES:
+        x.update(set(_copy(_) for _ in missing))
+    else:
+        _handle_error(handler, 'value', [trace, nan, 'missing:{}'.format(missing)])
+    
+    if not extra_allowed:
+        extra = set(_ for _ in x if _ not in nvalue)
+        if not extra: pass
+        elif handler['index']['extra'] in _FIX_MODES:
+            for _ in extra:
+                x.pop(_)
+        else:
+            _handle_error(handler, 'value', [trace, 'extra:{}'.format(extra)])
+            
+    return x
+
+
+def _verify_list_elements_by_nvalue(x, norm, mode, trace, handler):
+    extra_allowed = norm.get('extra_allowed')
+    nvalue = norm.get('value', norm.get('values', norm.get('v', nan)))
+    if is_null(nvalue):
+        return x
+    
+    len_x, len_nv = len(x), len(nvalue)
+    _min_len = min(len_x,len_nv)
+    norm_extra = NORM_EXTRA #?? Should this be deprecated?
+    #if sizes differ then zip will only iterate to the lowest size
+    new = x[:_min_len]
+    
+    if len_x < len_nv:
+        if handler['index']['missing'] in _FIX_MODES:
+            x_new = init_data(norm, copy=False)
+            new += _copy(x_new[len_x:])
+        else:
+            _handle_error(handler, 'value', [trace, nan, 'missing:{}'.format(nvalue[len_x:])])
+    
+    if len_x > len_nv and not extra_allowed:
+        if handler['index']['extra'] not in _FIX_MODES:
+            _handle_error(handler, 'value', [trace, 'extra:{}'.format(x[len_nv:])])
+            new += x[len_nv:]
+            
+    new = [verify_data(v, nv, mode, trace=trace, handler=handler, norm_extra=norm_extra)
+           for v,nv in zip(new[:_min_len],nvalue)] + new[_min_len:]
+    
+    return new
+
+
+#-----------------------------------------------------------------------
+
+def _verify_type(_type, correct_types, sub_allowed=True, **kw):
+    ctps = correct_types
+    ctps2 = EQUALS.get(ctps) if not isinstance(ctps,tuple) else tuple((EQUALS.get(t1) for t1 in ctps))
+    #Note that due to normalisation norm['_type'] is always hashable (is either type or tuple or types)
+    
+    correct_types = _flatten_types(ctps, ctps2)
+    #as_dict = kw.get('as_dict')
+    
+    if sub_allowed and not issubclass(_type, correct_types): pass
+    elif not sub_allowed and _type not in correct_types: pass
+    else: return True
+    
+    return correct_types
+
+
+def _get_missing_extra(x, norm):
+    missing = tuple(filter(lambda nk: nk not in x, norm))
+    extra = tuple(filter(lambda k: k not in norm, x))
+    
+    return {'missing': missing, 'extra': extra}
+
+
+def _verify_keys(x, norm, trace, handler, optional=[], required=None, extra_allowed=False):
+    me = _get_missing_extra(x,norm)
+    extra = tuple(filter(lambda k: k not in optional, me['extra'])) if not extra_allowed else tuple()
+    missing = tuple(filter(lambda k: k not in optional, me['missing']))
+    if is_not_null(required):
+        missing = tuple(filter(lambda k: k in required, missing))
+    
+    len_missing,len_extra = len(missing),len(extra)
+    if not len_missing + len_extra:
+        return {'missing': missing, 'extra': extra, 'missing_all': me['missing'], 'extra_all': me['extra']}
+    
+        
+    mp = missing if len_missing else nan
+    ep = extra if len_extra else nan
+    
+    trace2 = trace + ['({})'.format(len(trace))]
+    _handle_error(handler, 'key', [trace2, ep, mp])
+        
+    return {'missing': missing, 'extra': extra, 'missing_all': me['missing'], 'extra_all': me['extra']}
+
+
+def _check_size(x, norm, trace, handler):
+    size = norm.get('size')
+    if is_null(size):
+        return True
+    
+    len_x = len(x)
+    all_correct = True
+    
+    for arg,op in [('min',lambda y: len_x>=y),
+                   ('max',lambda y:len_x<=y),
+                   ('exact',lambda y: len_x==y)]:
+        limit = size.get(arg)
+        if is_null(limit): continue
+        satisfied = op(limit)
+        all_correct = min(all_correct, satisfied)
+        if not satisfied:
+            _handle_error(handler, 'index', [trace, len_x, '{}:{}'.format(arg,limit)])
+            
+    return all_correct
+
+
+def _check_size2(x, norm, trace, handler):
+    size = norm.get('size',nan)
+    if not is_not_null(size):
+        return True
+    
+    size = norm.get('size')
+    incl = size.get('include',nan)
+    excl = size.get('exclude',nan)
+    len_x = len(x)
+    is_correct = False
+    
+    if is_not_null(excl) and len_x in excl:
+        _handle_error(handler, 'index', [trace,'({}, excl:{})'.format(len_x, excl)])
+         
+    elif is_not_null(incl) and len_x not in incl:
+        _handle_error(handler, 'index', [trace,'({}, incl:{})'.format(len_x, excl)])
+            
+    else: is_correct = True
+            
+            
+    return is_correct
+    
+
+#-------------------------------------------------------------------------------------------------
+
+def _flatten_types(_types, _equals=None):
+    try: _types = tuple(flatten(_types))
+    except TypeError: _types = (_types,)
+    
+    try: _equals = tuple(flatten(_equals))
+    except TypeError: _equals = (_equals,)
+    
+    f = lambda x: x is not None
+    
+    return tuple(unique(filter(f, _types + _equals)))
+
+
+def _verify_is_type(x):
+    if not type(x) is type:
+        raise BadInstruction('Is not type: {}'.format(x))
+    
+    return x
+
+
+def _verify_input_args(kw):
+    handler = kw.get('handler',{})
+    if _isnorm(handler): return kw
+    elif not isinstance(handler,dict):
+        raise TypeError('Handler must be dict, instead got: {}'.format(type(handler).__name__))
+    
+    mode = kw['mode']
+    if kw['mode'] not in _MODES:
+        raise ValueError('Wrong mode: {}'.format(mode))
+    
+    fix_any = mode in _FIX_MODES
+    
+    #--else--:
+    
+    for k in _H_OBJ_KEYS:
+        hx_mode = handler.get(k, kw.get(k,mode))
+        if hx_mode in _FIX_MODES:
+            fix_any = True
+        elif hx_mode not in _MODES:
+            raise ValueError('Wrong "{}" mode: {}'.format(k, hx_mode))
+        handler[k] = hx_mode
+    
+    #{'key': {'extra': _mode, 'missing': _mode2}, 'index': ...} 
+    by_mode = {c: {x: mode for x in _H_CONTAINER_OPTIONS} for c in _H_CONTAINER_KEYS}
+    by_option = {c: {x: kw.get(x) for x in _H_CONTAINER_OPTIONS} for c in _H_CONTAINER_KEYS}
+    by_type = {c: {x: kw.get(c) for x in _H_CONTAINER_OPTIONS} for c in _H_CONTAINER_KEYS}
+    by_handler = {c: {x: handler.get(c, {}).get(x) for x in _H_CONTAINER_OPTIONS} for c in _H_CONTAINER_KEYS}
+    
+    hierarchy = {None: {'doms': 'all'}} #do not overwrite with None
+    for x in (by_mode, by_option, by_type, by_handler):
+        deep_update(handler, x, False, hierarchy)
+
+    
+    for c in _H_CONTAINER_KEYS:
+        for x in _H_CONTAINER_OPTIONS:
+            cx_mode = handler[c][x]
+            if cx_mode in _FIX_MODES:
+                fix_any = True
+            elif cx_mode not in _MODES:
+                raise ValueError('Wrong "{}" mode: {}; kwargs: {}'.format(c, cx_mode, kw))
+            
+    """for k in _H_CONTAINER_KEYS:
+        hx_mode = handler.get(k) #, kw.get(k,mode)
+        if hx_mode is None:
+        if isinstance(hx_mode,str):
+            if hx_mode in _MODES:
+                if hx_mode in _FIX_MODES:
+                    fix_any = True
+                handler[k] = hx_mode = dict.fromkeys(_H_CONTAINER_OPTIONS, hx_mode)
+            else:
+                raise ValueError('Wrong "{}" mode: {}'.format(k, hx_mode))
+        
+        elif not isinstance(hx_mode,dict):
+            raise TypeError('Wrong type for "{}" mode: {}'.format(k, type(hx_mode).__name__))
+        
+        d = hx_mode
+        for k2 in _H_CONTAINER_OPTIONS:
+            hox_mode = d.get(k2, handler.get(k2, kw.get(k2,mode)))
+            if hox_mode in _FIX_MODES:
+                fix_any = True
+            elif hox_mode not in _MODES:
+                raise ValueError('Wrong "{}":{} mode: {}'.format(k, k2, hox_mode))
+            d[k2] = hox_mode
+            
+        handler[k] = d"""
+        
+        
+    handler['_isnorm_'] = True
+    kw['handler'] = handler
+    
+    
+    """copy = kw['copy']
+    if type(copy) is bool: pass
+    elif isinstance(copy,str): pass
+    else: raise TypeError('Wrong type for "copy" argument: {}'.format(type(copy)))
+    
+    if copy == 'fix_mode':
+        if fix_any: copy = True
+        else: copy = False
+        
+    kw['copy'] = copy"""
+        
+        
+    for k in list(kw.keys()):
+        if k not in ('handler','mode','copy'):
+            del kw[k]
+            
+
+
+def _single_out(errors):
+    #higher is more specific
+    def _get_error_rank(e):
+        return _EXC_ORD.index(type(e))
+    
+    def _update(e, rank, lvl, i):
+        e_inf.update({'errors': [e], 'rank': rank, 'lvl': lvl, 'i': i+1})
+    
+    _errors = errors
+    e_inf = {'errors': [_errors[0]],
+             'rank': _get_error_rank(errors[0]),
+             'lvl': errors[0].level,
+             'i': 0}
+    
+    for i,e in enumerate(errors[1:]):
+        rank = _get_error_rank(e)
+        lvl = e.level #_get_trace_lvl(e)
+        
+        if lvl > e_inf['lvl']:
+            _update(e, rank, lvl, i)
+        
+        elif lvl == e_inf['lvl']:
+            if rank > e_inf['rank']:
+                _update(e, rank, lvl, i)
+            elif rank == e_inf['rank']: 
+                e_inf['errors'].append(e)
+
+
+    errors = e_inf['errors']
+    
+    if len(errors) == 1:
+        return {'e': errors[0], 'i': e_inf['i']}
+    
+    e_args = []
+    msgs = []
+    for i,e in enumerate(errors):
+        #if i > 0: e.args[0] = " ".join(e.args[0].split(" ")[1:])
+        #the first arg begins with trace, which'll be identical for same lvl same type errors
+
+        #e_args.extend(e.args)
+        e_args = e.args # this includes trace, got, expected, custom_msg, and the *args
+        msgs.append(e.msg)
+    
+    new_e = errors[0].__class__(*e_args) # use the info of the last error
+    new_e.msg = " || ".join(msgs)
+    
+    return {'e': new_e, 'i': e_inf['i']}
+    
+
+"""def _get_trace_lvl(e):
+    msg = e.args[0]
+    trace = msg.split(" ")[0]
+    
+    lvl = 0
+    
+    for i,c in enumerate(trace):
+        if c!= "(": continue
+        i2 = next(((i+1)+j for j,c2 in enumerate(trace[i+1:]) if not c2.isdigit()),-1)
+        if i2 in (-1,i+1) or trace[i2] != ")": continue
+        
+        lvl2 = int(trace[i+1:i2])
+        if lvl2 != lvl + 1: continue
+        
+        lvl = lvl2
+        
+    return lvl"""
+
+
+def _handle_error(handler, type, args=[], kw={}):
+    e, i = (None, 0)
+    
+    if isinstance(type,VeriError): 
+        e = type
+    elif isinstance(type,(list,tuple)):
+        if len(type) > 1:
+            d = _single_out(type)
+            e,i = d['e'],d['i']
+        else: e = type[0]
+        
+    if e is not None: 
+        type = e.type
+    
+    mode = handler[type]
+    ms = None
+    
+    if not isinstance(mode,dict):
+        ms = _mode_specs(mode)
+    
+        if not (ms['is_error'] or ms['is_warn']):
+            return {'i': i, 'is_fix': ms['is_fix']}
+    
+
+    if e is None:
+        eclass = _EXCEPTIONS[type]
+        e = eclass(*args,**kw)
+        
+    if ms is None:
+        ms = _mode_specs_from_error(e, handler)
+        
+    
+    if ms['is_error']:
+        raise e
+    elif ms['is_warn']:
+        warnings.warn(str(e))
+    
+    return {'i': i, 'is_fix': ms['is_fix']}
+    
+
+
+def _mode_specs(mode):
+    if mode is None:
+        return dict.fromkeys(('is_error','is_fix','is_warn'), False)
+        
+    is_error = mode in _ERROR_MODES
+    is_warn = False if is_error else mode in _WARN_MODES
+    is_fix = False if is_error else mode in _FIX_MODES
+    
+    return {'is_error': is_error, 'is_fix': is_fix, 'is_warn': is_warn}
+
+
+def _mode_specs_from_error(e,handler):
+    is_faulty = e.is_faulty()
+    x = handler[e.type]
+    
+    if is_faulty is True:
+        return _mode_specs(x)
+    elif is_faulty is False:
+        return _mode_specs(None)
+    
+    #-else is_faulty is dict
+    
+    specs = _mode_specs(None)
+    
+    for subset,f_val in is_faulty.items():
+        if not f_val: continue
+        
+        e_mode = x[subset]
+        new_specs = _mode_specs(e_mode)
+        specs.update({k:v for k,v in new_specs.items() if v})
+        
+        
+    return specs
+
+
+def _parse_user_error(e, trace, got=nan, expected=nan, custom_msg=nan):
+    args = [trace, got, expected, custom_msg]
+    if type(e) in _EXC_MAP.values():
+        e_type = next(x for x,y in _EXC_MAP.items() if type(e)==y).type
+        args[3] = nan if not e.args else (e.args[0] if len(e.args)==1 else e.args)
+        return e_type, args
+    elif isinstance(e, VeriError):
+        args[0] = list(trace) + list(e.trace)
+        if e.got is not nan:
+            args[1] = e.got
+        if e.expected is not nan:
+            args[2] = e.expected
+        if e.custom_msg is not nan:
+            args[3] = e.custom_msg
+        return e.type, args
+    else:
+        args[3] = e
+        return 'general', args
+
+
+def convert_exception(e):
+    t = _EXC_MAP.get(type(e))
+    if not t:
+        return e
+    
+    return t(e.msg)
+
+
+
+#--------------------------------------
+
+def fill_missing(x, norm, warn=True):
+    mode = 'fix' if warn else 'fix-'
+    return verify_data(x, norm, mode=mode)
+
+#......................................
+
+def _resolve(x, as_type=False):
+    if _isinstructions(x):
+        return x
+    if as_type:
+        e = None
+        try: 
+            d = {'_type_': x}
+            _normalize_type(d)
+            if '_type_' in d:
+                return d
+            e = BadInstruction('Does not resolve to type: {}'.format(x))
+        except BadInstruction as exc:
+            e = exc
+        if e and as_type!='try':
+            raise e
+    return {'_value_': x}
+
+
+class Element:
+    __aliases = {
+        'type': ['_type_', 'type'],
+        'value': ['_value_', 'value'],
+        'multival': ['_multival_', 'multival'],
+        'defval': ['_defval_', 'defval'],
+        'unit': ['unit'],
+        'dtypes': ['dtypes'],
+        'default_dtype': ['default_dtype'],
+        'call': ['_call_', 'call'],
+        'keys': ['keys'],
+        'values': ['values', 'v'],
+        'items': ['items'],
+        'multi': ['_multi_','multi'],
+        'vfy': ['_vfy_', 'vfy'],
+        'isnorm': ['_isnorm_','isnorm'],
+    }
+    
+    def __init__(self, *type, **kw):
+        self.verify_params(type, kw)
+        if len(type):
+            self.type = type[0] if len(type) == 1 else type
+        
+        self.update(kw)
+    
+    
+    def __call__(self, copy=True):
+        return init_data(self, copy=copy)
+    
+    
+    def verify(self, x, mode='error', copy=False, **kw):
+        return verify_data(x, self, mode, copy, **kw)
+    
+    
+    def to_dict(self, **kw):
+        if hasattr(self, '__dict') and not kw:
+            return self.__dict
+        d = {}
+        #copy_attrs = ['unit','dtypes']
+        
+        for attr, aliases in self._Element__aliases.items():
+            alias = aliases[0]
+            if hasattr(self, attr):
+                value = getattr(self, attr)
+                #if attr in copy_attrs:
+                #    value = value.copy()
+                d[alias] = value
+        
+        d.update(self.__kw)
+        self.__dict = d
+        
+        if kw:
+            d = dict(d, **kw)
+        
+        return d
+    
+    
+    def update(self, d, normalize=True):
+        resolve_attrs = ['unit']
+        resolve_elements = ['dtypes','multi']
+        found = []
+        
+        for attr, aliases in self._Element__aliases.items():
+            for alias in aliases:
+                if alias in d:
+                    value = d[alias]
+                    if attr in resolve_attrs:
+                        value = _resolve(value)
+                    if attr in resolve_elements:
+                        if isinstance(value, dict):
+                            value = {k: _resolve(v, 'try') for k,v in value.items()}
+                        else:
+                            value = [_resolve(v) for v in value]
+                    setattr(self, attr, value)
+                    found.append(alias)
+        
+        self.__kw = {k: v for k,v in d.items() if k not in found}
+        
+        if hasattr(self, '__dict'):
+            del self.__dict
+        
+        if normalize:
+            if hasattr(self, 'isnorm'):
+                del self.isnorm
+            normalize_element(self)
+        else:
+            self.to_dict()
+    
+    
+    def get(self, key, *default):
+        return self.__dict.get(key, *default)
+    
+    
+    def __contains__(self, key):
+        return key in self.__dict
+    
+    
+    def __len__(self):
+        ignore = {'_copy_','_isnorm_'}
+        return sum(1 for x in self.__dict if x not in ignore)
+    
+    
+    @classmethod
+    def verify_params(cls, type, kw):
+        must_contain_attr = '_{}__must_contain'.format(cls.__name__)
+        if hasattr(cls, must_contain_attr):
+            must_contain = getattr(cls, must_contain_attr)
+            for attr in must_contain:
+                aliases = cls._Element__aliases[attr]
+                if not any(x in kw for x in aliases):
+                    raise BadInstruction('Does not contain: {}'.format(attr))
+
+
+class Container(Element):
+    
+    def __getitem__(self, key):
+        if not isinstance(key, tuple):
+            key = (key,)
+        
+        d = self.to_dict()
+        unit = d.get('unit', {})
+        
+        if len(key) == 1:
+            unit.update(_resolve(key[0], 'try'))
+        elif len(key) > 1:
+            resolved = [_resolve(k, 'try') for k in key]
+            types_only, values_only, other = [], [], []
+            for x in resolved:
+                if len(x) == 1 and '_type_' in x:
+                    if isinstance(x.get('_type_'), tuple):
+                        types_only += list(x.get('_type_'))
+                    else:
+                        types_only.append(x.get('_type_'))
+                elif len(x) == 1 and '_value_' in x:
+                    values_only.append(x.get('_value_'))
+                elif len(x) == 1 and '_multival_' in x:
+                    values_only += list(x.get('_multival_'))
+                else:
+                    other.append(x)
+            
+            _type = {'_type_': tuple(types_only) if len(types_only) > 1 else types_only[0]} if len(types_only) else {}
+            _value = ({'_multival_': values_only} if len(values_only)> 1 else {'_value_': values_only[0]}) if values_only else {}
+            if _type and (not _value and not other):
+                unit.update(_type)
+            elif _value and (not _type and not other):
+                unit.update(_value)
+            else:
+                multi = []
+                if _type:
+                    multi.append(_type)
+                if _value:
+                    multi.append(_value)
+                if other:
+                    multi += other
+                unit['_multi_'] = multi
+        
+        if 'unit' in d or unit:
+            d['unit'] = unit
+        
+        return Container(**d)
+    
+    
+    def __iter__(self):
+        raise TypeError("'Container' object is not iterable.")
+
+
+class Multi(Element):
+    def __init__(self, *elements, **kw):
+        if not elements:
+            raise BadInstruction('No elements provided')
+        if 'multi' not in 'kw':
+            kw['multi'] = elements
+        super().__init__(**kw)
+
+
+class Type(Element):
+    __must_contain = ['type']
+    
+    def __init__(self, *type, **kw):
+        if not type:
+            raise BadInstruction('type not provided')
+        if 'type' not in kw:
+            kw['type'] = type
+        super().__init__(**kw)
+
+
+class Value(Element):
+    __must_contain = ['value']
+    
+    def __init__(self, value, **kw):
+        if 'value' not in kw:
+            kw['value'] = value
+        super().__init__(**kw)
+
+
+class MultiVal(Element):
+    __must_contain = ['multival']
+    
+    def __init__(self, *values, **kw):
+        if 'multival' not in kw:
+            kw['multival'] = list(values)
+        super().__init__(**kw)
+
+
+class Dtyct(Container):
+    __must_contain = ['dtypes']
+    
+    def __init__(self, dtypes, **kw):
+        if 'dtypes' not in kw:
+            kw['dtypes'] = dtypes
+        super().__init__(dict, **kw)
+    
+    @classmethod
+    def from_dtypes(cls, *kw, **dtypes):
+        kw = kw[0] if kw else {}
+        return cls(dtypes, **kw)
+
+
+class IntRange(Element):
+    def __init__(self, range, **kw):
+        if 'range' not in kw:
+            kw['range'] = range
+        super().__init__(int, **kw)
+
+
+class FloatRange(Element):
+    def __init__(self, range, **kw):
+        if 'range' not in kw:
+            kw['range'] = range
+        super().__init__(float, **kw)
+
+
+Str = Element(str)
+Int = Element(int)
+Float = Element(float)
+Bool = Element(bool)
+Null = Element(type(None))
+List = Container(list)
+Dict = Container(dict)
+NullDict = Container(dict, unit={'_defval_': None}, default_dtype=None)
+Set = Container(set)
+
+
+__all__ = ['Str','Int','Float','Bool','Null','List','Dict','Dtyct','NullDict',
+           'Set','Multi','Type','Value','MultiVal','Element','Container',
+           'IntRange','FloatRange','normalize_element','normalize','init_data',
+           'verify_data','convert_exception','fill_missing']
```

### Comparing `fons-0.3.1/fons/__init__.py` & `fons-0.4.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-__version__ = '0.3.1'
-__author__ = 'binares'
-
-'''
-    Python library for various purposes.
-    
-    `fons` - latin for "source"
-    
-    Some useful functions and classes:
-        * aio.call_via_loop_afut - call a (async)function via (another) loop (possibly running in a different thread),
-                                    returns async future with pending result/exception thrown of the function
-        
-        * argv.parse_argv - for parsing input sys.argv into dict values and list values, modifying them, and de-parsing
-        
-        * func.(async_)limitcalls - a decorator for setting rate limit to (async) function/method
-                                    @limitcalls(1, 5, action='sleep')
-                                    def f(): pass     -> f can only be called once per every 5 seconds, sleeps until that delay is reached
-        
-        * io.update_settings - load dict from settings file, supporting multiple configs in the same or different files
-        
-        * iter.flatten - "flatten" a nested list (iterator): list(flatten([2,{3:4},[5,6,(7,)],'89'])) -> [2,{3:4},5,6,7,'89']
-                          (by default includes only "known" iterators; doesn't include: dicts, strings, namedtuples, custom defined classes)
-                            
-        * iter.fliter - "flatten" any iterable: list(fliter([2,{3:4},[5,6,(7,)],'89'])) -> [2,3,4,5,6,7,'8','9']
-        
-        * iter.unique - keep each value of iterator only once: list(unique([2,3,2])) -> [2,3]
-        
-        * sched.(Async)Ticker.loop - repeatedly execute a (async)function with a set interval (supports pandas offsets, e.g. '1B')
-        
-        * time.dt_round - round datetime: dt_round(datetime.datetime(2016,3,1,2), 'D') -> datetime.datetime(2016,3,1)
-        
-        * verify.verify_data - assert the correctness of input data (useful for avoiding accidental user config mistypes)
-'''
+# fons
+
+Python library for various purposes.
+    
+`fons` - latin for "source"
+
+Some useful functions and classes:
+
+    * aio.call_via_loop_afut - call a (async)function via (another) loop (possibly running in a different thread),
+                                returns async future with pending result/exception thrown of the function
+
+    * argv.parse_argv - for parsing input sys.argv into dict values and list values, modifying them, and de-parsing
+
+    * func.(async_)limitcalls - a decorator for setting rate limit to (async) function/method
+                                @limitcalls(1, 5, action='sleep')
+                                def f(): pass     -> f can only be called once per every 5 seconds, sleeps until that delay is reached
+
+    * io.update_settings - load dict from settings file, supporting multiple configs in the same or different files
+
+    * iter.flatten - "flatten" a nested list (iterator): list(flatten([2,{3:4},[5,6,(7,)],'89'])) -> [2,{3:4},5,6,7,'89']
+                      (by default includes only "known" iterators; doesn't include: dicts, strings, namedtuples, custom defined classes)
+
+    * iter.fliter - "flatten" any iterable: list(fliter([2,{3:4},[5,6,(7,)],'89'])) -> [2,3,4,5,6,7,'8','9']
+
+    * iter.unique - keep each value of iterator only once: list(unique([2,3,2])) -> [2,3]
+
+    * sched.(Async)Ticker.loop - repeatedly execute a (async)function with a set interval (supports pandas offsets, e.g. '1B')
+
+    * time.dt_round - round datetime: dt_round(datetime.datetime(2016,3,1,2), 'D') -> datetime.datetime(2016,3,1)
+
+    * verify.verify_data - assert the correctness of input data (useful for avoiding accidental user config mistypes)
+
```

### Comparing `fons-0.3.1/fons.egg-info/PKG-INFO` & `fons-0.4.0/fons/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,33 @@
-Metadata-Version: 2.1
-Name: fons
-Version: 0.3.1
-Summary: A broad range of python tools. Some uses: round datetimes, verify input data, execute functions by schedule, parse argv
-Home-page: https://github.com/binares/fons
-Author: binares
-Author-email: binares@protonmail.com
-License: MIT
-Description: # fons
-        
-        Python library for various purposes.
-            
-        `fons` - latin for "source"
-        
-        Some useful functions and classes:
-        
-            * aio.call_via_loop_afut - call a (async)function via (another) loop (possibly running in a different thread),
-                                        returns async future with pending result/exception thrown of the function
-        
-            * argv.parse_argv - for parsing input sys.argv into dict values and list values, modifying them, and de-parsing
-        
-            * func.(async_)limitcalls - a decorator for setting rate limit to (async) function/method
-                                        @limitcalls(1, 5, action='sleep')
-                                        def f(): pass     -> f can only be called once per every 5 seconds, sleeps until that delay is reached
-        
-            * io.update_settings - load dict from settings file, supporting multiple configs in the same or different files
-        
-            * iter.flatten - "flatten" a nested list (iterator): list(flatten([2,{3:4},[5,6,(7,)],'89'])) -> [2,{3:4},5,6,7,'89']
-                              (by default includes only "known" iterators; doesn't include: dicts, strings, namedtuples, custom defined classes)
-        
-            * iter.fliter - "flatten" any iterable: list(fliter([2,{3:4},[5,6,(7,)],'89'])) -> [2,3,4,5,6,7,'8','9']
-        
-            * iter.unique - keep each value of iterator only once: list(unique([2,3,2])) -> [2,3]
-        
-            * sched.(Async)Ticker.loop - repeatedly execute a (async)function with a set interval (supports pandas offsets, e.g. '1B')
-        
-            * time.dt_round - round datetime: dt_round(datetime.datetime(2016,3,1,2), 'D') -> datetime.datetime(2016,3,1)
-        
-            * verify.verify_data - assert the correctness of input data (useful for avoiding accidental user config mistypes)
-        
-        
-Platform: UNKNOWN
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
+__version__ = "0.4.0"
+__author__ = "binares"
+
+"""
+    Python library for various purposes.
+    
+    `fons` - latin for "source"
+    
+    Some useful functions and classes:
+        * aio.call_via_loop_afut - call a (async)function via (another) loop (possibly running in a different thread),
+                                    returns async future with pending result/exception thrown of the function
+        
+        * argv.parse_argv - for parsing input sys.argv into dict values and list values, modifying them, and de-parsing
+        
+        * func.(async_)limitcalls - a decorator for setting rate limit to (async) function/method
+                                    @limitcalls(1, 5, action='sleep')
+                                    def f(): pass     -> f can only be called once per every 5 seconds, sleeps until that delay is reached
+        
+        * io.update_settings - load dict from settings file, supporting multiple configs in the same or different files
+        
+        * iter.flatten - "flatten" a nested list (iterator): list(flatten([2,{3:4},[5,6,(7,)],'89'])) -> [2,{3:4},5,6,7,'89']
+                          (by default includes only "known" iterators; doesn't include: dicts, strings, namedtuples, custom defined classes)
+                            
+        * iter.fliter - "flatten" any iterable: list(fliter([2,{3:4},[5,6,(7,)],'89'])) -> [2,3,4,5,6,7,'8','9']
+        
+        * iter.unique - keep each value of iterator only once: list(unique([2,3,2])) -> [2,3]
+        
+        * sched.(Async)Ticker.loop - repeatedly execute a (async)function with a set interval (supports pandas offsets, e.g. '1B')
+        
+        * time.dt_round - round datetime: dt_round(datetime.datetime(2016,3,1,2), 'D') -> datetime.datetime(2016,3,1)
+        
+        * verify.verify_data - assert the correctness of input data (useful for avoiding accidental user config mistypes)
+"""
```

### Comparing `fons-0.3.1/fons.egg-info/SOURCES.txt` & `fons-0.4.0/fons.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+MANIFEST.in
 README.md
+requirements.txt
 setup.py
 fons/__init__.py
 fons/aio.py
 fons/all.py
 fons/argv.py
 fons/crypto.py
 fons/debug.py
@@ -12,14 +14,17 @@
 fons/fsync.py
 fons/func.py
 fons/gui.py
 fons/host.py
 fons/io.py
 fons/iter.py
 fons/log.py
+fons/log311.py
+fons/log35.py
+fons/log38.py
 fons/nan.py
 fons/os.py
 fons/processes.py
 fons/py.py
 fons/pyops.py
 fons/reg.py
 fons/sched.py
@@ -45,14 +50,15 @@
 fons/net/urlstr.py
 test/test_aio.py
 test/test_crypto.py
 test/test_event.py
 test/test_func.py
 test/test_io.py
 test/test_iter.py
+test/test_log.py
 test/test_pyops.py
 test/test_sched.py
 test/test_threads.py
 test/test_time.py
 test/test_url.py
 test/test_verify.py
 test/test_verify_old.py
```

### Comparing `fons-0.3.1/PKG-INFO` & `fons-0.4.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,51 @@
-Metadata-Version: 2.1
-Name: fons
-Version: 0.3.1
-Summary: A broad range of python tools. Some uses: round datetimes, verify input data, execute functions by schedule, parse argv
-Home-page: https://github.com/binares/fons
-Author: binares
-Author-email: binares@protonmail.com
-License: MIT
-Description: # fons
-        
-        Python library for various purposes.
-            
-        `fons` - latin for "source"
-        
-        Some useful functions and classes:
-        
-            * aio.call_via_loop_afut - call a (async)function via (another) loop (possibly running in a different thread),
-                                        returns async future with pending result/exception thrown of the function
-        
-            * argv.parse_argv - for parsing input sys.argv into dict values and list values, modifying them, and de-parsing
-        
-            * func.(async_)limitcalls - a decorator for setting rate limit to (async) function/method
-                                        @limitcalls(1, 5, action='sleep')
-                                        def f(): pass     -> f can only be called once per every 5 seconds, sleeps until that delay is reached
-        
-            * io.update_settings - load dict from settings file, supporting multiple configs in the same or different files
-        
-            * iter.flatten - "flatten" a nested list (iterator): list(flatten([2,{3:4},[5,6,(7,)],'89'])) -> [2,{3:4},5,6,7,'89']
-                              (by default includes only "known" iterators; doesn't include: dicts, strings, namedtuples, custom defined classes)
-        
-            * iter.fliter - "flatten" any iterable: list(fliter([2,{3:4},[5,6,(7,)],'89'])) -> [2,3,4,5,6,7,'8','9']
-        
-            * iter.unique - keep each value of iterator only once: list(unique([2,3,2])) -> [2,3]
-        
-            * sched.(Async)Ticker.loop - repeatedly execute a (async)function with a set interval (supports pandas offsets, e.g. '1B')
-        
-            * time.dt_round - round datetime: dt_round(datetime.datetime(2016,3,1,2), 'D') -> datetime.datetime(2016,3,1)
-        
-            * verify.verify_data - assert the correctness of input data (useful for avoiding accidental user config mistypes)
-        
-        
-Platform: UNKNOWN
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: fons
+Version: 0.4.0
+Summary: A broad range of python tools. Some uses: round datetimes, verify input data, execute functions by schedule, parse argv
+Home-page: https://github.com/binares/fons
+Author: binares
+Author-email: binares@protonmail.com
+License: MIT
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+Requires-Dist: aiohttp>=2.0
+Requires-Dist: aiohttp_socks>=0.2
+Requires-Dist: requests>=2.0
+Requires-Dist: cryptography>=1.8
+Requires-Dist: filelock>=3.0
+Requires-Dist: ntplib>=0.3.3
+Requires-Dist: pandas>=0.21
+Requires-Dist: PyYAML>=3.10
+
+# fons
+
+Python library for various purposes.
+    
+`fons` - latin for "source"
+
+Some useful functions and classes:
+
+    * aio.call_via_loop_afut - call a (async)function via (another) loop (possibly running in a different thread),
+                                returns async future with pending result/exception thrown of the function
+
+    * argv.parse_argv - for parsing input sys.argv into dict values and list values, modifying them, and de-parsing
+
+    * func.(async_)limitcalls - a decorator for setting rate limit to (async) function/method
+                                @limitcalls(1, 5, action='sleep')
+                                def f(): pass     -> f can only be called once per every 5 seconds, sleeps until that delay is reached
+
+    * io.update_settings - load dict from settings file, supporting multiple configs in the same or different files
+
+    * iter.flatten - "flatten" a nested list (iterator): list(flatten([2,{3:4},[5,6,(7,)],'89'])) -> [2,{3:4},5,6,7,'89']
+                      (by default includes only "known" iterators; doesn't include: dicts, strings, namedtuples, custom defined classes)
+
+    * iter.fliter - "flatten" any iterable: list(fliter([2,{3:4},[5,6,(7,)],'89'])) -> [2,3,4,5,6,7,'8','9']
+
+    * iter.unique - keep each value of iterator only once: list(unique([2,3,2])) -> [2,3]
+
+    * sched.(Async)Ticker.loop - repeatedly execute a (async)function with a set interval (supports pandas offsets, e.g. '1B')
+
+    * time.dt_round - round datetime: dt_round(datetime.datetime(2016,3,1,2), 'D') -> datetime.datetime(2016,3,1)
+
+    * verify.verify_data - assert the correctness of input data (useful for avoiding accidental user config mistypes)
+
```

### Comparing `fons-0.3.1/test/test_aio.py` & `fons-0.4.0/test/test_aio.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-import pytest
-import asyncio
-
-from fons.aio import call_via_loop
-
-
-async def asyncfunc(arg,*,kw=1):
-    return arg/kw
-
-
-async def _afunc():
-    await asyncio.sleep(0.01)
-    
-    
-def test_call_via_loop():
-    loop = asyncio.get_event_loop()
-    f = call_via_loop(asyncfunc,(4,),{'kw':2})
-    loop.run_until_complete(_afunc())
-    assert f.result(0.1) == 2
-    
-    f = call_via_loop(asyncfunc,(4,),{'kw':0})
-    loop.run_until_complete(_afunc())
-    with pytest.raises(ZeroDivisionError):
-        assert f.result(0.1)
-
-
-if __name__ == '__main__':
-    test_call_via_loop()
+import pytest
+import asyncio
+
+from fons.aio import call_via_loop
+
+
+async def asyncfunc(arg, *, kw=1):
+    return arg / kw
+
+
+async def _afunc():
+    await asyncio.sleep(0.01)
+
+
+def test_call_via_loop():
+    loop = asyncio.get_event_loop()
+    f = call_via_loop(asyncfunc, (4,), {"kw": 2})
+    loop.run_until_complete(_afunc())
+    assert f.result(0.1) == 2
+
+    f = call_via_loop(asyncfunc, (4,), {"kw": 0})
+    loop.run_until_complete(_afunc())
+    with pytest.raises(ZeroDivisionError):
+        assert f.result(0.1)
+
+
+if __name__ == "__main__":
+    test_call_via_loop()
```

### Comparing `fons-0.3.1/test/test_crypto.py` & `fons-0.4.0/test/test_crypto.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import pytest
 from cryptography.fernet import InvalidToken
 from fons.crypto import password_encrypt, password_decrypt
 
-password = 'k2L0?me!r7Gs'
-typo_password = password[:-1] + 'd'
+password = "k2L0?me!r7Gs"
+typo_password = password[:-1] + "d"
 
 DATA = [
-    '',
-    'a',
-    'This text will be encrypted',
-    'Hello world! #s{}:'.format('\u20ac\u00a3'), #euro pound
+    "",
+    "a",
+    "This text will be encrypted",
+    "Hello world! #s{}:".format("\u20ac\u00a3"),  # euro pound
 ]
 
-@pytest.mark.parametrize('text', DATA)
+
+@pytest.mark.parametrize("text", DATA)
 def test_encrypt_decrypt(text):
-    btext = text.encode('utf-8')
+    btext = text.encode("utf-8")
     encoded = password_encrypt(btext, password)
-    
+
     assert encoded != btext
-    
+
     btext2 = password_decrypt(encoded, password)
-    text2 = btext2.decode('utf-8')
-    
+    text2 = btext2.decode("utf-8")
+
     assert text == text2
-    
+
     with pytest.raises(InvalidToken):
         password_decrypt(encoded, typo_password)
-
```

### Comparing `fons-0.3.1/test/test_func.py` & `fons-0.4.0/test/test_func.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,254 +1,260 @@
-import pytest
-import time
-import fons.func as ffunc
-from fons.func import limitcalls, limitcalls_f, limitcalls_m
-from fons.errors import TerminatedException, WaitException
-
-
-ffunc._LIMITCALLS_WARN_WHEN_SLEEP = True
-ffunc._LIMITCALLS_STORE_GLOBALLY = True
-LH = ffunc._LIMITCALLS_HISTORY
-
-r = 4
-m,p = (3,1)
-s = 0.5
-
-#------------------
-
-@limitcalls_f(m)
-def f_totalcalls():
-    return r
-
-
-@limitcalls_f(m,p)
-def f_periodcalls(self):
-    return r
-
-
-
-def _test_totalcalls(func,*args,**kw):
-    for i in range(m):
-        assert func(*args,**kw) == r
-
-    with pytest.raises(TerminatedException):
-        func(*args,**kw)
-
-
-def _test_periodcalls(func,*args,**kw):
-    for i in range(m):
-        assert func(*args,**kw) == r
-
-    with pytest.raises(WaitException):# as e_info:
-        func(*args,**kw)
-
-
-    time.sleep(p-s)
-    with pytest.raises(WaitException):# as e_info:
-        func(*args,**kw)
-
-    time.sleep(s)
-    assert func(*args,**kw) == r
-
-
-    
-#----------------------
-
-def test_f_totalcalls():
-    _test_totalcalls(f_totalcalls)
-
-
-def test_f_periodcalls():
-    _test_periodcalls(f_periodcalls,None)
-
-
-#-------------------------
-totalcalls_code = "def totalcalls%i(self,b,*args): return r"
-
-def totalcalls0(self,b,*args):
-    return r
-
-for i in range(2,5):
-    #exec(totalcalls_code %i)
-    exec('totalcalls%i = totalcalls0' %i)
-
-
-#plain:
-class A:
-    @limitcalls_m(m)
-    def totalcalls(self,b,*args):
-        return r
-
-    totalcalls2 = limitcalls_m(m)(totalcalls0)
-    totalcalls3 = limitcalls_m(m, f=totalcalls0)
-
-    @classmethod
-    @limitcalls_f(m)
-    def cls_totalcalls(cls,b,*args):
-        return r
-    
-    @staticmethod
-    @limitcalls_f(m)
-    def static_totalcalls(b=None,*args):
-        return r
-
-
-class B(A):
-    pass
-
-a = A()
-a2 = A()
-b = B()
-
-
-
-#induced:
-class C:
-    @limitcalls(m)
-    def totalcalls(self,b,*args):
-        return r
-
-    totalcalls2 = limitcalls(m)(totalcalls0)
-    totalcalls3 = limitcalls(m, f=totalcalls0)
-    
-
-    @classmethod
-    @limitcalls(m)
-    def cls_totalcalls(cls,b,*args):
-        return r
-    
-    @staticmethod
-    @limitcalls(m)
-    def static_totalcalls(b=None,*args):
-        return r
-
-    #-----------
-    #ON PURPOSE:
-    
-    @classmethod
-    @limitcalls(m)
-    def cls_totalcalls_self(self,b,*args):
-        return r
-
-    @staticmethod
-    @limitcalls(m)
-    def static_totalcalls_self(self,b,*args):
-        return r
-
-  
-
-
-class D(C):
-    pass
-
-c,c2,d = C(), C(), D()
-
-
-
-def _test_m_totalcalls(objs, funcname):
-    for obj in objs:
-        func = getattr(obj,funcname)
-        
-        _test_totalcalls(func,1,None)
-    
-
-plain_m = [a,a2,b]
-induced_m = [c,c2,d]
-totalcalls_m_funcs = ['totalcalls','totalcalls2','totalcalls3']
-
-def test_m_totalcalls():
-    for funcname in totalcalls_m_funcs:
-        _test_m_totalcalls(plain_m, funcname)
-    
-def test_m_totalcalls_induced():
-    for funcname in totalcalls_m_funcs:
-        _test_m_totalcalls(induced_m, funcname)
-
-#------
-
-def _test_cs_totalcalls(objs,funcname):
-    _test_totalcalls(getattr(objs[0],funcname), {}, None)
-
-    for cls in objs[1:]:
-        with pytest.raises(TerminatedException):
-            getattr(cls,funcname)({},None)  
-
-
-plain = a,A,B,b,a2
-induced = c,C,D,d,c2
-
-def test_c_totalcalls():
-    _test_cs_totalcalls(plain,'cls_totalcalls')
-
-def test_c_totalcalls_induced():
-    _test_cs_totalcalls(induced,'cls_totalcalls')    
-
-
-def test_s_totalcalls():
-    _test_cs_totalcalls(plain,'static_totalcalls')
-
-def test_s_totalcalls_induced():
-    _test_cs_totalcalls(induced,'static_totalcalls')
-
-
-
-def test_cls_totalcalls_induced_with_self():
-    _test_cs_totalcalls(induced,'cls_totalcalls_self')
-
-def test_s_totalcalls_induced_with_self():
-    with pytest.raises(TypeError):
-        #first param 'self' is dict, not hashable
-        _test_cs_totalcalls(induced,'static_totalcalls_self')
-    
-
-@limitcalls(m)
-def totalcalls_self(self,b,*args):
-    return r
-
-def test_f_totalcalls_induced_with_self():
-    _test_totalcalls(totalcalls_self, {}, 2)
-
-
-#---------------------------------------
-
-l_warn = limitcalls_f(m,action='warn')
-l_log = limitcalls_f(m,action='log', logging_level=50)
-l_sleep = limitcalls_f(m,p,action='sleep', logging_level=50)
-l_null = limitcalls_f(m,action=None)
-
-def test_actions():
-    items = [l_warn, l_log, l_sleep, l_null]
-    for dec in items:
-        f = dec(lambda x: r)
-
-        for i in range(m+1):
-            f(None)
-
-    with pytest.raises(ValueError):
-        limitcalls_f(m,action='sleep', logging_level=50)
-
-
-
-"""nan = '_nan_'
-from collections import OrderedDict as OD
-
-params = [['p',2],
-          ['q', 4],
-          ['t','T'],
-          ['*',nan],
-          ['*args', nan],
-          ['**kw', nan]]
-
-darams = OD(params)
-
-params = [[],
-          ['p'],
-          ['p','q=4'],
-          ['p=2, *args'],
-          ['p=2, *, q=4, **kw'],
-          ['self'],
-          ['self=a'],
-          ['self=None'],
-          ['*self, p=2'],
-          ['**self']]
-
-decorators = ['@limicalls_f(m,p)','@limitcalls_m(m,p)','@limitcalls(m,p)']"""
+import pytest
+import time
+import fons.func as ffunc
+from fons.func import limitcalls, limitcalls_f, limitcalls_m
+from fons.errors import TerminatedException, WaitException
+
+
+ffunc._LIMITCALLS_WARN_WHEN_SLEEP = True
+ffunc._LIMITCALLS_STORE_GLOBALLY = True
+LH = ffunc._LIMITCALLS_HISTORY
+
+r = 4
+m, p = (3, 1)
+s = 0.5
+
+# ------------------
+
+
+@limitcalls_f(m)
+def f_totalcalls():
+    return r
+
+
+@limitcalls_f(m, p)
+def f_periodcalls(self):
+    return r
+
+
+def _test_totalcalls(func, *args, **kw):
+    for i in range(m):
+        assert func(*args, **kw) == r
+
+    with pytest.raises(TerminatedException):
+        func(*args, **kw)
+
+
+def _test_periodcalls(func, *args, **kw):
+    for i in range(m):
+        assert func(*args, **kw) == r
+
+    with pytest.raises(WaitException):  # as e_info:
+        func(*args, **kw)
+
+    time.sleep(p - s)
+    with pytest.raises(WaitException):  # as e_info:
+        func(*args, **kw)
+
+    time.sleep(s)
+    assert func(*args, **kw) == r
+
+
+# ----------------------
+
+
+def test_f_totalcalls():
+    _test_totalcalls(f_totalcalls)
+
+
+def test_f_periodcalls():
+    _test_periodcalls(f_periodcalls, None)
+
+
+# -------------------------
+totalcalls_code = "def totalcalls%i(self,b,*args): return r"
+
+
+def totalcalls0(self, b, *args):
+    return r
+
+
+for i in range(2, 5):
+    # exec(totalcalls_code %i)
+    exec("totalcalls%i = totalcalls0" % i)
+
+
+# plain:
+class A:
+    @limitcalls_m(m)
+    def totalcalls(self, b, *args):
+        return r
+
+    totalcalls2 = limitcalls_m(m)(totalcalls0)
+    totalcalls3 = limitcalls_m(m, f=totalcalls0)
+
+    @classmethod
+    @limitcalls_f(m)
+    def cls_totalcalls(cls, b, *args):
+        return r
+
+    @staticmethod
+    @limitcalls_f(m)
+    def static_totalcalls(b=None, *args):
+        return r
+
+
+class B(A):
+    pass
+
+
+a = A()
+a2 = A()
+b = B()
+
+
+# induced:
+class C:
+    @limitcalls(m)
+    def totalcalls(self, b, *args):
+        return r
+
+    totalcalls2 = limitcalls(m)(totalcalls0)
+    totalcalls3 = limitcalls(m, f=totalcalls0)
+
+    @classmethod
+    @limitcalls(m)
+    def cls_totalcalls(cls, b, *args):
+        return r
+
+    @staticmethod
+    @limitcalls(m)
+    def static_totalcalls(b=None, *args):
+        return r
+
+    # -----------
+    # ON PURPOSE:
+
+    @classmethod
+    @limitcalls(m)
+    def cls_totalcalls_self(self, b, *args):
+        return r
+
+    @staticmethod
+    @limitcalls(m)
+    def static_totalcalls_self(self, b, *args):
+        return r
+
+
+class D(C):
+    pass
+
+
+c, c2, d = C(), C(), D()
+
+
+def _test_m_totalcalls(objs, funcname):
+    for obj in objs:
+        func = getattr(obj, funcname)
+
+        _test_totalcalls(func, 1, None)
+
+
+plain_m = [a, a2, b]
+induced_m = [c, c2, d]
+totalcalls_m_funcs = ["totalcalls", "totalcalls2", "totalcalls3"]
+
+
+def test_m_totalcalls():
+    for funcname in totalcalls_m_funcs:
+        _test_m_totalcalls(plain_m, funcname)
+
+
+def test_m_totalcalls_induced():
+    for funcname in totalcalls_m_funcs:
+        _test_m_totalcalls(induced_m, funcname)
+
+
+# ------
+
+
+def _test_cs_totalcalls(objs, funcname):
+    _test_totalcalls(getattr(objs[0], funcname), {}, None)
+
+    for cls in objs[1:]:
+        with pytest.raises(TerminatedException):
+            getattr(cls, funcname)({}, None)
+
+
+plain = a, A, B, b, a2
+induced = c, C, D, d, c2
+
+
+def test_c_totalcalls():
+    _test_cs_totalcalls(plain, "cls_totalcalls")
+
+
+def test_c_totalcalls_induced():
+    _test_cs_totalcalls(induced, "cls_totalcalls")
+
+
+def test_s_totalcalls():
+    _test_cs_totalcalls(plain, "static_totalcalls")
+
+
+def test_s_totalcalls_induced():
+    _test_cs_totalcalls(induced, "static_totalcalls")
+
+
+def test_cls_totalcalls_induced_with_self():
+    _test_cs_totalcalls(induced, "cls_totalcalls_self")
+
+
+def test_s_totalcalls_induced_with_self():
+    with pytest.raises(TypeError):
+        # first param 'self' is dict, not hashable
+        _test_cs_totalcalls(induced, "static_totalcalls_self")
+
+
+@limitcalls(m)
+def totalcalls_self(self, b, *args):
+    return r
+
+
+def test_f_totalcalls_induced_with_self():
+    _test_totalcalls(totalcalls_self, {}, 2)
+
+
+# ---------------------------------------
+
+l_warn = limitcalls_f(m, action="warn")
+l_log = limitcalls_f(m, action="log", logging_level=50)
+l_sleep = limitcalls_f(m, p, action="sleep", logging_level=50)
+l_null = limitcalls_f(m, action=None)
+
+
+def test_actions():
+    items = [l_warn, l_log, l_sleep, l_null]
+    for dec in items:
+        f = dec(lambda x: r)
+
+        for i in range(m + 1):
+            f(None)
+
+    with pytest.raises(ValueError):
+        limitcalls_f(m, action="sleep", logging_level=50)
+
+
+"""nan = '_nan_'
+from collections import OrderedDict as OD
+
+params = [['p',2],
+          ['q', 4],
+          ['t','T'],
+          ['*',nan],
+          ['*args', nan],
+          ['**kw', nan]]
+
+darams = OD(params)
+
+params = [[],
+          ['p'],
+          ['p','q=4'],
+          ['p=2, *args'],
+          ['p=2, *, q=4, **kw'],
+          ['self'],
+          ['self=a'],
+          ['self=None'],
+          ['*self, p=2'],
+          ['**self']]
+
+decorators = ['@limicalls_f(m,p)','@limitcalls_m(m,p)','@limitcalls(m,p)']"""
```

### Comparing `fons-0.3.1/test/test_io.py` & `fons-0.4.0/test/test_io.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,196 +1,216 @@
-import os
-from shutil import copy2
-import pytest
-import datetime
-dt = datetime.datetime
-
-import fons.io as io
-
-fdir = os.path.dirname(__file__)
-PARAMS_PATH = os.path.join(fdir, 'test_io_read_params.txt')
-PARAMS_SAVE_PATH = os.path.join(fdir, 'test_io_read_params_out.txt')
-_SETTINGS_PATH = os.path.join(fdir, 'test_io_update_settings.yaml')
-SETTINGS_PATH = os.path.join(fdir, 'test_io_update_settings_COPY.yaml')
-_SETTINGS_TEST3_PATH = os.path.join(fdir, 'test_io_update_settings_TEST3.yaml')
-SETTINGS_TEST3_PATH = os.path.join(fdir, 'test_io_update_settings_TEST3_COPY.yaml')
-SETTINGS_NO_INDENT_PATH = os.path.join(fdir, 'test_io_update_settings_no_indent.yaml')
-
-#Copy the files, for eGit purposes 
-#(if we don't copy and just overwrite the original, it thinks they've been updated)
-copy2(_SETTINGS_PATH, SETTINGS_PATH)
-copy2(_SETTINGS_TEST3_PATH, SETTINGS_TEST3_PATH)
-
-p_expected = {
-    'token': "jrhyyiycfev:j4vjxh7p06wsf1061wukwvjs3hnhm8",
-    'contacts': {"self": 8711851293646172144751, "rndm": 234},
-    'atpl': [False, True, True, False],
-    2: ["sth", "other"],
-    '2': ["sth", "other2"],
-    None: ["sth", "other"],
-    'end': "//",
-    '<>': 2.4,
-    'NEW_PARAM': ["a", "list"],
-    'NEW_PARAM2': {"its k": "its v"},
-    '613524184:xxpOiJ683r6iNvbCtgA2J4QD817FSTnfP': {"its k": "its v"},
-}
-
-def test_read_params():
-    p = io.read_params(PARAMS_PATH)
-    
-    for k,v_expected in p_expected.items():
-        assert p[k] == v_expected
-    
-
-def test_read_params_with_keys():
-    p = io.read_params(PARAMS_PATH, ['token'])
-    
-    assert isinstance(p, dict) and len(p) == 1
-    assert p['token'] == p_expected['token']
-    
-
-def test_read_params_raises_KeyError():
-    with pytest.raises(KeyError):
-        io.read_params(PARAMS_PATH, ['notPresentKey'])
-
-
-def test_save_params():
-    now = dt.utcnow().isoformat()
-    
-    io.save_params(PARAMS_SAVE_PATH, {'newKey': now}, read_path=PARAMS_PATH)
-    
-    p = io.read_params(PARAMS_SAVE_PATH)
-    
-    assert p['newKey'] == now
-    
-    for k,v_expected in p_expected.items():
-        assert p[k] == v_expected
-    
-    os.remove(PARAMS_SAVE_PATH)
-        
-
-#---------------------------
-
-_ijh = {'_type_': dict,
-        'dtypes': {'k': {'_type_':dict,
-                         'dtypes':{'l': str,
-                                   'm': str}}}}
-verify = {
-    '_type_': dict,
-    #'default_dtype': None
-    'dtypes': {
-        'abc': str,
-        'edf': bool,
-        'ijh': _ijh,
-        'opq': int}}
-
-
-def D():
-    return {'abc': 'not_defined_yet'}
-
-def _drop_meta(d):
-    return {k: v for k,v in d.items() if k != '__meta__'}
-
-def _get(config=None, verify=verify, deep=None, force_update=None):
-    return [config, verify, deep, force_update]
-
-#init verify deep force_update
-_default = [True, verify, True, False]
-
-
-expected_dicts = [
-    {'abc': 'abcvalue', 'edf': True, 'ijh': {"k": {"l": None}}, 'opq': 1}, #0
-    {'abc': 'test_abcvalue', 'edf': False, 'ijh': {"k": {"l": "lV", "m": "mV"}}, 'opq': 1}, #1 
-    {'abc': None, 'opq': 2}, #2
-    {'abc': 'test3_abcvalue', 'ijh': {'k': {'m': 't3mV'}}}, #3
-    {'abc': 'test3_abcvalue', 'ijh': {'k': {'m': 't3mV'}}}, #4
-]
-
-_inp = [
-    [D(), 'default']    + _default,
-    [D(), 'TEST'] + _default,
-    [D(), 'TEST2'] + _default,
-    [D(), 'TEST3'] + [True, verify, False, False], #deep=False
-    [D(), None] + [True, verify, False, False], #deep=False __config__ == TEST3
-]
-
-inp = [x[:1] + [expected_dicts[i]] + x[1:] for i,x in enumerate(_inp)]
-
-
-@pytest.mark.parametrize("d,expected,config,init,verify,deep,force_update", inp)
-def test_update_settings(d, expected, config, init, verify, deep, force_update):
-    
-    io.update_settings(SETTINGS_PATH, d, config=config, init=init,
-                       verify=verify, deep=deep, force_update=force_update)
-    
-    assert _drop_meta(d) == expected
-    
-
-def test_update_settings_no_indent():
-    d = {}
-    io.update_settings(SETTINGS_NO_INDENT_PATH, d, config='TEST',
-                       init=True, verify=verify, deep=True)
-    assert d['__meta__']['default'] == None
-    assert d['__meta__']['config'] == 'TEST'
-    assert d['__meta__']['exclude'] == ['TEST','TEST2','TEST3']
-    
-    assert _drop_meta(d) == expected_dicts[1]
-    
-
-def test_update_settings_modified_time():
-    
-    def _update(d, force_update=False):
-        io.update_settings(SETTINGS_PATH, d, config='TEST3', init=True,
-                           verify=verify, deep=False, force_update=force_update)
-        
-    def _modify_file(path):
-        temp_path = os.path.join(os.path.dirname(path), 'io_temp')
-        with open(path) as f:
-            with open(temp_path,'w') as f2:
-                f2.write(f.read())
-        os.remove(path)
-        os.rename(temp_path, path)
-        
-    def _keep_only_meta(d):
-        for k in list(d.keys()):
-            if k != '__meta__':
-                del d[k]
-        #to force it to update the values
-        if '__meta__' in d:
-            d['__meta__']['last_input'] = {}
-            d['__meta__']['last_input_meta'] = {}
-                
-    _get_dict = lambda d: dict(__meta__=d['__meta__'])
-    
-    def _verify(d, path):
-        #add "modified" times to create (if not already added)
-        _keep_only_meta(d)
-        _update(d)
-        _keep_only_meta(d)
-        
-        #will not update the dict as the file hasn't been modified in the meanwhile
-        _update(d)
-        
-        #values weren't updated
-        assert list(d.keys()) == ['__meta__']
-        
-        #force update
-        _update(d, True)
-        
-        #keys were added
-        assert len(d) > 1
-        
-        #modify the file
-        _modify_file(path)
-        
-        _keep_only_meta(d)
-        
-        #should update
-        _update(d)
-        
-        #keys were added
-        assert len(d) > 1
-    
-    d = {}
-    
-    _verify(d, SETTINGS_PATH)
-    _verify(d, SETTINGS_TEST3_PATH)
+import os
+from shutil import copy2
+import pytest
+import datetime
+
+dt = datetime.datetime
+
+import fons.io as io
+
+fdir = os.path.dirname(__file__)
+PARAMS_PATH = os.path.join(fdir, "test_io_read_params.txt")
+PARAMS_SAVE_PATH = os.path.join(fdir, "test_io_read_params_out.txt")
+_SETTINGS_PATH = os.path.join(fdir, "test_io_update_settings.yaml")
+SETTINGS_PATH = os.path.join(fdir, "test_io_update_settings_COPY.yaml")
+_SETTINGS_TEST3_PATH = os.path.join(fdir, "test_io_update_settings_TEST3.yaml")
+SETTINGS_TEST3_PATH = os.path.join(fdir, "test_io_update_settings_TEST3_COPY.yaml")
+SETTINGS_NO_INDENT_PATH = os.path.join(fdir, "test_io_update_settings_no_indent.yaml")
+
+# Copy the files, for eGit purposes
+# (if we don't copy and just overwrite the original, it thinks they've been updated)
+copy2(_SETTINGS_PATH, SETTINGS_PATH)
+copy2(_SETTINGS_TEST3_PATH, SETTINGS_TEST3_PATH)
+
+p_expected = {
+    "token": "jrhyyiycfev:j4vjxh7p06wsf1061wukwvjs3hnhm8",
+    "contacts": {"self": 8711851293646172144751, "rndm": 234},
+    "atpl": [False, True, True, False],
+    2: ["sth", "other"],
+    "2": ["sth", "other2"],
+    None: ["sth", "other"],
+    "end": "//",
+    "<>": 2.4,
+    "NEW_PARAM": ["a", "list"],
+    "NEW_PARAM2": {"its k": "its v"},
+    "613524184:xxpOiJ683r6iNvbCtgA2J4QD817FSTnfP": {"its k": "its v"},
+}
+
+
+def test_read_params():
+    p = io.read_params(PARAMS_PATH)
+
+    for k, v_expected in p_expected.items():
+        assert p[k] == v_expected
+
+
+def test_read_params_with_keys():
+    p = io.read_params(PARAMS_PATH, ["token"])
+
+    assert isinstance(p, dict) and len(p) == 1
+    assert p["token"] == p_expected["token"]
+
+
+def test_read_params_raises_KeyError():
+    with pytest.raises(KeyError):
+        io.read_params(PARAMS_PATH, ["notPresentKey"])
+
+
+def test_save_params():
+    now = dt.utcnow().isoformat()
+
+    io.save_params(PARAMS_SAVE_PATH, {"newKey": now}, read_path=PARAMS_PATH)
+
+    p = io.read_params(PARAMS_SAVE_PATH)
+
+    assert p["newKey"] == now
+
+    for k, v_expected in p_expected.items():
+        assert p[k] == v_expected
+
+    os.remove(PARAMS_SAVE_PATH)
+
+
+# ---------------------------
+
+_ijh = {
+    "_type_": dict,
+    "dtypes": {"k": {"_type_": dict, "dtypes": {"l": str, "m": str}}},
+}
+verify = {
+    "_type_": dict,
+    #'default_dtype': None
+    "dtypes": {"abc": str, "edf": bool, "ijh": _ijh, "opq": int},
+}
+
+
+def D():
+    return {"abc": "not_defined_yet"}
+
+
+def _drop_meta(d):
+    return {k: v for k, v in d.items() if k != "__meta__"}
+
+
+def _get(config=None, verify=verify, deep=None, force_update=None):
+    return [config, verify, deep, force_update]
+
+
+# init verify deep force_update
+_default = [True, verify, True, False]
+
+
+expected_dicts = [
+    {"abc": "abcvalue", "edf": True, "ijh": {"k": {"l": None}}, "opq": 1},  # 0
+    {
+        "abc": "test_abcvalue",
+        "edf": False,
+        "ijh": {"k": {"l": "lV", "m": "mV"}},
+        "opq": 1,
+    },  # 1
+    {"abc": None, "opq": 2},  # 2
+    {"abc": "test3_abcvalue", "ijh": {"k": {"m": "t3mV"}}},  # 3
+    {"abc": "test3_abcvalue", "ijh": {"k": {"m": "t3mV"}}},  # 4
+]
+
+_inp = [
+    [D(), "default"] + _default,
+    [D(), "TEST"] + _default,
+    [D(), "TEST2"] + _default,
+    [D(), "TEST3"] + [True, verify, False, False],  # deep=False
+    [D(), None] + [True, verify, False, False],  # deep=False __config__ == TEST3
+]
+
+inp = [x[:1] + [expected_dicts[i]] + x[1:] for i, x in enumerate(_inp)]
+
+
+@pytest.mark.parametrize("d,expected,config,init,verify,deep,force_update", inp)
+def test_update_settings(d, expected, config, init, verify, deep, force_update):
+    io.update_settings(
+        SETTINGS_PATH,
+        d,
+        config=config,
+        init=init,
+        verify=verify,
+        deep=deep,
+        force_update=force_update,
+    )
+
+    assert _drop_meta(d) == expected
+
+
+def test_update_settings_no_indent():
+    d = {}
+    io.update_settings(
+        SETTINGS_NO_INDENT_PATH, d, config="TEST", init=True, verify=verify, deep=True
+    )
+    assert d["__meta__"]["default"] == None
+    assert d["__meta__"]["config"] == "TEST"
+    assert d["__meta__"]["exclude"] == ["TEST", "TEST2", "TEST3"]
+
+    assert _drop_meta(d) == expected_dicts[1]
+
+
+def test_update_settings_modified_time():
+    def _update(d, force_update=False):
+        io.update_settings(
+            SETTINGS_PATH,
+            d,
+            config="TEST3",
+            init=True,
+            verify=verify,
+            deep=False,
+            force_update=force_update,
+        )
+
+    def _modify_file(path):
+        temp_path = os.path.join(os.path.dirname(path), "io_temp")
+        with open(path) as f:
+            with open(temp_path, "w") as f2:
+                f2.write(f.read())
+        os.remove(path)
+        os.rename(temp_path, path)
+
+    def _keep_only_meta(d):
+        for k in list(d.keys()):
+            if k != "__meta__":
+                del d[k]
+        # to force it to update the values
+        if "__meta__" in d:
+            d["__meta__"]["last_input"] = {}
+            d["__meta__"]["last_input_meta"] = {}
+
+    _get_dict = lambda d: dict(__meta__=d["__meta__"])
+
+    def _verify(d, path):
+        # add "modified" times to create (if not already added)
+        _keep_only_meta(d)
+        _update(d)
+        _keep_only_meta(d)
+
+        # will not update the dict as the file hasn't been modified in the meanwhile
+        _update(d)
+
+        # values weren't updated
+        assert list(d.keys()) == ["__meta__"]
+
+        # force update
+        _update(d, True)
+
+        # keys were added
+        assert len(d) > 1
+
+        # modify the file
+        _modify_file(path)
+
+        _keep_only_meta(d)
+
+        # should update
+        _update(d)
+
+        # keys were added
+        assert len(d) > 1
+
+    d = {}
+
+    _verify(d, SETTINGS_PATH)
+    _verify(d, SETTINGS_TEST3_PATH)
```

### Comparing `fons-0.3.1/test/test_sched.py` & `fons-0.4.0/test/test_sched.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,345 +1,456 @@
-import pytest
-import warnings
-from queue import Queue
-import asyncio
-import datetime
-dt = datetime.datetime
-td = datetime.timedelta
-import time
-import logging
-logging.basicConfig(level=10)
-
-from fons.sched import (Ticker, AsyncTicker, TickManager, AsyncTickManager, Routine,
-                        WaitException, QuitException, TerminatedException, 
-                        AllTerminated)
-import fons.time as fontime
-
-
-#tfunc = lambda x: 2
-
-
-def to_us(adt):
-    us = adt.microsecond
-    if us <= 0:
-        return us
-    
-    while us < 100000:
-        us *= 10
-        
-    return us
-
-#........................
-gl_counter = 0
-nr = 15
-
-def tfunc(a,b,*,n=4):
-    global gl_counter
-    gl_counter += 1
-    
-    #time.sleep(0.0001)
-    if not(gl_counter % nr):
-        print('gl counter: {}, raising QuitException'.format(gl_counter))
-        raise QuitException
-    
-    return a+b+n
-
-args = (1,2)
-kw = {'n':4}
-
-
-
-factor = 1
-I = 0.01 * factor
-D = 0.01
-
-
-iu_counter = 1
-
-def IU():
-    global iu_counter
-    new_i =  I + 0.003*factor*(iu_counter%20)
-    iu_counter += 1
-    
-    return new_i
-
-
-
-def test_ticker():
-    t = Ticker(tfunc,interval=I,sync=None,args=args,kw=kw,lock=0.2,keep=nr)
-    IU2 = Ticker(IU,interval=I)
-    t3 = Ticker(tfunc,interval=IU,sync=None,lock='next',args=args,kw=kw,keep=nr)
-    
-    t4 = Ticker(tfunc,interval=I,sync=td(0,1),delay=D,lock='next',args=args,kw=kw,keep=nr)
-    t5 = Ticker(tfunc,interval=I,sync='first',delay=D,args=args,kw=kw,keep=nr)
-    t6 = Ticker(tfunc,interval=IU,sync='first',delay=D,args=args,kw=kw,keep=nr,name='TickerX6')
-    
-
-    for x in (t,t3,t4,t5,t6):
-        
-        for i in range(nr):
-            try: x.tick()
-            except WaitException as e:
-                logging.info('{}, {}, sleeping {}'.format(x._name,i,e.wait_time))
-                #warnings.warn('{},{}, sleeping {}'.format(x._name,i,e.wait_time))
-                time.sleep(e.wait_time)
-                x.tick()
-            finally:
-                if i == nr-1 and x in (t3,t4,t5,t6):
-                    entries = list(x.entries)[::-1]
-                    records = list(x.records)[::-1]
-                    secs = ['{}.{}'.format(y.second,int(to_us(y)/1000)) for y in entries]
-                    difs = [round((y-entries[i])/td(seconds=1),int(4/factor)) for i,y in enumerate(entries[1:])]
-                    #difs2 = [round((y[1]-y[0])/td(seconds=1),6) for y in records]
-                    logging.debug('{}\ndifs: {}\n'.format(x._name, difs)) #,difs2))
-              
-
-    for x in (t,t3,t4,t5,t6):
-        assert x._closed
-        with pytest.raises(TerminatedException):
-            x.tick()
-                    
-                
-                
-def test_ticker_thread():
-    q = Queue()
-    callback = lambda x: q.put(x['result'])
-    t = Ticker(lambda: 2 ,interval=0, callback=callback, name='ThreadTicker')
-    t.start_thread()
-    
-    a = q.get(timeout=0.2)
-    assert a == 2
-    
-    t.close()
-    assert t._closed
-    with pytest.raises(TerminatedException):
-        t.tick()
-        
-
-
-def test_synced():
-    at = Ticker(interval='1T',sync='1T')
-    synced = at._synced(dt(2018,8,4,2,5,15,1))
-    assert synced == dt(2018,8,4,2,5)
-    
-    at.tick()
-    assert at.entries[0] == fontime.dt_round(dt.utcnow(),'1T')
-    assert int(at.get_time_remaining()) == 60 - dt.utcnow().second - 1
-        
-#------------------------------------------
-
-async def async_ticker():
-    global gl_counter,iu_counter
-    gl_counter = 0
-    iu_counter = 1
-    
-    global nr
-    nr = 3
-    
-    t = AsyncTicker(tfunc,interval=I,sync=None,args=args,kw=kw,lock=0.2,keep=nr)
-    IU2 = AsyncTicker(IU,interval=I)
-    t3 = AsyncTicker(tfunc,interval=IU,sync=None,lock='next',args=args,kw=kw,keep=nr)
-    
-    t4 = AsyncTicker(tfunc,interval=I,sync=td(0,1),delay=D,lock='next',args=args,kw=kw,keep=nr)
-    t5 = AsyncTicker(tfunc,interval=I,sync='first',delay=D,args=args,kw=kw,keep=nr)
-    t6 = AsyncTicker(tfunc,interval=IU,sync='first',delay=D,args=args,kw=kw,keep=nr,name='TickerX6')
-    
-    
-    for x in (t,t3,t4,t5,t6):
-        
-        for i in range(nr):
-            try: await x.tick()
-            except WaitException as e:
-                logging.info('{}, {}, sleeping {}'.format(x._name,i,e.wait_time))
-                #warnings.warn('{},{}, sleeping {}'.format(x._name,i,e.wait_time))
-                await asyncio.sleep(e.wait_time)
-                await x.tick()
-            finally:
-                if i == nr-1 and x in (t3,t4,t5,t6):
-                    entries = list(x.entries)[::-1]
-                    records = list(x.records)[::-1]
-                    secs = ['{}.{}'.format(y.second,int(to_us(y)/1000)) for y in entries]
-                    difs = [round((y-entries[i])/td(seconds=1),int(4/factor)) for i,y in enumerate(entries[1:])]
-                    #difs2 = [round((y[1]-y[0])/td(seconds=1),6) for y in records]
-                    logging.debug('{}\ndifs: {}\n'.format(x._name, difs)) #,difs2))
-    
-    
-    for x in (t,t3,t4,t5,t6):
-        with pytest.raises(TerminatedException):
-            print('verifying error')
-            await x.tick()
-            print('THIS SHOULD NOT BE PRINTED')
-
-    print('Async all passed')
-    
-    
-loop = asyncio.get_event_loop()
-      
-def test_async_ticker():
-    loop.run_until_complete(asyncio.gather(*[async_ticker()], return_exceptions=False))
-
-    
-#------------------------------------------
-def test_tick_manager():
-    global gl_counter,iu_counter
-    gl_counter = 0
-    iu_counter = 1
-    
-    t = Ticker(tfunc,interval=I,sync=None,args=args,kw=kw,lock=0.2,keep=nr)
-    t2 = Ticker(tfunc,interval=I,sync=None,args=args,kw=kw,lock=0.2,keep=nr)
-    
-    tm = TickManager([t,t2])
-    tm.tick(errors='sleep')
-    tm.tick(errors='sleep')
-    
-    t.close()
-    tm.tick(errors='sleep')
-    
-    t2.close()
-    
-    with pytest.raises(AllTerminated):
-        tm.tick()
-
-
-#------------------------------------------
-
-async def async_tick_manager():
-    global gl_counter,iu_counter
-    gl_counter = 0
-    iu_counter = 1
-    
-    cb = lambda x: print('{} completed at {}'.format(x['ticker']._name,dt.utcnow()))
-    e1 = asyncio.Event()
-    e2 = asyncio.Event()
-    
-    def cb2(e):
-        def cb2_wapped(x):
-            print('{} completed at {}'.format(x['ticker']._name,dt.utcnow()))
-            e.set()
-        return cb2_wapped
-        
-        
-    t1 = AsyncTicker(tfunc,interval=I,sync=None,args=args,kw=kw,lock=0.2,keep=nr,callback=cb2(e1))
-    t2 = AsyncTicker(tfunc,interval=I,sync=None,args=args,kw=kw,lock=0.2,keep=nr,callback=cb2(e2))
-    tm = AsyncTickManager([t1,t2], loop=loop, allterminated='raise', callback=cb)
-    
-    await tm.tick()
-    await tm.tick()
-    
-    print('waiting till e1 set')
-    await e1.wait()
-    print('wait complete')
-    
-    await t1.close()
-    print('t1 closed x1')
-    e2.clear()
-    
-    await tm.tick()
-    
-    print('waiting till e2 set')
-    await e2.wait()
-    print('wait complete')
-
-    await t2.close()
-    print('t2 closed')
-    
-    with pytest.raises(AllTerminated):
-        await tm.tick()
-    print('tm .tick() raised Allterminated')
-     
-    await tm.close()
-    print('tm._closed: {}'.format(tm._closed))
-    with pytest.raises(TerminatedException):
-        await tm.tick()
-    print('tm .tick() raised TerminatedException')
-
-
-def test_async_tick_manager():
-    loop.run_until_complete(asyncio.gather(*[async_tick_manager()], return_exceptions=False))
-
-
-
-
-async def async_tick_manager_loop():
-    global gl_counter,iu_counter
-    gl_counter = 0
-    iu_counter = 1
-    
-    cb = lambda x: print('{} ticked at {}'.format(x['ticker']._name,dt.utcnow()))
-    e1 = asyncio.Event()
-    e2 = asyncio.Event()
-    e3 = asyncio.Event()
-    
-    def cb2(e):
-        def cb2_wapped(x):
-            print('{} ticked at {}'.format(x['ticker']._name,dt.utcnow()))
-            e.set()
-        return cb2_wapped
-        
-        
-    t1 = AsyncTicker(tfunc,interval=I,sync=None,args=args,kw=kw,lock=0.2,keep=nr,callback=cb2(e1),name='AT-1 of AsyncTickManagerMAIN')
-    t2 = AsyncTicker(tfunc,interval=I,sync=None,args=args,kw=kw,lock=0.2,keep=nr,callback=cb2(e2),name='AT-2 of AsyncTickManagerMAIN')
-    tm = AsyncTickManager([t1,t2], loop=loop, allterminated='raise', callback=cb,name='AsyncTickManagerMAIN')
-    
-    #assert e1.is_set()
-    #assert e2.is_set()
-    
-    #tickers are automatically terminated at loop #nr
-    with pytest.raises(AllTerminated):
-        await tm.loop()
-    
-
-             
-def test_async_tick_manager_loop():
-    loop.run_until_complete(asyncio.gather(*[async_tick_manager_loop()], return_exceptions=False))
-
-
-def test_routine():
-    async def rout_func(d={'i':0},break_at=2):
-        d['i'] += 1
-        if d['i'] == break_at:
-            raise QuitException
- 
-    sched = {
-        'r1': {'target': rout_func, 'kwargs': {'d':{'i':0}}, 'interval':0.01},
-        'r2': {'target': rout_func, 'kwargs': {'d':{'i':0},'break_at':4}},
-    }
-    rout = Routine(sched,tickmgr={'allterminated':'close'})
-    loop.run_until_complete(asyncio.gather(*[rout.start()], return_exceptions=False))
-    assert sched['r1']['kwargs']['d']['i'] == 2
-    assert sched['r2']['kwargs']['d']['i'] == 4
-    assert rout.get_event('r1').is_set()
-    assert rout.get_event('r2').is_set()
-    
-#def test_asynctickmgr_with_nonasynctickers():
-    
-    
-"""
-r2 = 'new_return'
-
-intervals = [td(seconds=0.1),0.1]
-exp_intervals = [intervals[0]] *2
-
-as_delay = [True,False,None,'e']
-
-delay = [td(seconds=0.05),0.05,None,dt(2000,1,1)]
-exp_delay = [delay[0]]*2 + [None,None]
-
-
-@pytest.mark.parametrized("interval","as_delay","delay","sync","exp")
-def test_basics(interval,as_delay,delay,sync,exp):
-    t = Ticker(tfunc,interval,as_delay,delay,sync=sync)
-    
-    assert t._ui['delay'] == exp['delay']
-    assert t._ui['as_delay'] == exp['as_delay']
-    
-    now = dt.utcnow()
-    t.tick()
-    
-    assert t._ui["interval"] == fontime.freq_to_offset(exp["interval"])
-    assert t.interval.delta = exp["interval"]
-    assert t.get_last() > now
-    assert t.get_actual_last() > now
-    assert t.sync == exp["sync"]
-    
-    
-def test_"""
+import pytest
+import warnings
+from queue import Queue
+import asyncio
+import datetime
+
+dt = datetime.datetime
+td = datetime.timedelta
+import time
+import logging
+
+from fons.log import quick_logging
+
+logging.basicConfig(level=10)
+# quick_logging(3, True)
+
+from fons.sched import (
+    Ticker,
+    AsyncTicker,
+    TickManager,
+    AsyncTickManager,
+    Routine,
+    WaitException,
+    QuitException,
+    TerminatedException,
+    AllTerminated,
+)
+import fons.time as fontime
+
+
+# tfunc = lambda x: 2
+
+
+def to_us(adt):
+    us = adt.microsecond
+    if us <= 0:
+        return us
+
+    while us < 100000:
+        us *= 10
+
+    return us
+
+
+# ........................
+gl_counter = 0
+nr = 15
+
+
+def tfunc(a, b, *, n=4):
+    global gl_counter
+    gl_counter += 1
+
+    # time.sleep(0.0001)
+    if not (gl_counter % nr):
+        print("gl counter: {}, raising QuitException".format(gl_counter))
+        raise QuitException
+
+    return a + b + n
+
+
+args = (1, 2)
+kw = {"n": 4}
+
+
+factor = 1
+I = 0.01 * factor
+D = 0.01
+
+
+iu_counter = 1
+
+
+def IU():
+    global iu_counter
+    new_i = I + 0.003 * factor * (iu_counter % 20)
+    iu_counter += 1
+
+    return new_i
+
+
+def test_ticker():
+    t = Ticker(tfunc, interval=I, sync=None, args=args, kw=kw, lock=0.2, keep=nr)
+    IU2 = Ticker(IU, interval=I)
+    t3 = Ticker(tfunc, interval=IU, sync=None, lock="next", args=args, kw=kw, keep=nr)
+
+    t4 = Ticker(
+        tfunc,
+        interval=I,
+        sync=td(0, 1),
+        delay=D,
+        lock="next",
+        args=args,
+        kw=kw,
+        keep=nr,
+    )
+    t5 = Ticker(tfunc, interval=I, sync="first", delay=D, args=args, kw=kw, keep=nr)
+    t6 = Ticker(
+        tfunc,
+        interval=IU,
+        sync="first",
+        delay=D,
+        args=args,
+        kw=kw,
+        keep=nr,
+        name="TickerX6",
+    )
+
+    for x in (t, t3, t4, t5, t6):
+        for i in range(nr):
+            try:
+                x.tick()
+            except WaitException as e:
+                logging.info("{}, {}, sleeping {}".format(x._name, i, e.wait_time))
+                # warnings.warn('{},{}, sleeping {}'.format(x._name,i,e.wait_time))
+                time.sleep(e.wait_time)
+                x.tick()
+            finally:
+                if i == nr - 1 and x in (t3, t4, t5, t6):
+                    entries = list(x.entries)[::-1]
+                    records = list(x.records)[::-1]
+                    secs = [
+                        "{}.{}".format(y.second, int(to_us(y) / 1000)) for y in entries
+                    ]
+                    difs = [
+                        round((y - entries[i]) / td(seconds=1), int(4 / factor))
+                        for i, y in enumerate(entries[1:])
+                    ]
+                    # difs2 = [round((y[1]-y[0])/td(seconds=1),6) for y in records]
+                    logging.debug("{}\ndifs: {}\n".format(x._name, difs))  # ,difs2))
+
+    for x in (t, t3, t4, t5, t6):
+        assert x._closed
+        with pytest.raises(TerminatedException):
+            x.tick()
+
+
+def test_ticker_thread():
+    q = Queue()
+    callback = lambda x: q.put(x["result"])
+    t = Ticker(lambda: 2, interval=0, callback=callback, name="ThreadTicker")
+    t.start_thread()
+
+    a = q.get(timeout=0.2)
+    assert a == 2
+
+    t.close()
+    assert t._closed
+    with pytest.raises(TerminatedException):
+        t.tick()
+
+
+def test_synced():
+    at = Ticker(interval="1T", sync="1T")
+    synced = at._synced(dt(2018, 8, 4, 2, 5, 15, 1))
+    assert synced == dt(2018, 8, 4, 2, 5)
+
+    at.tick()
+    assert at.entries[0] == fontime.dt_round(dt.utcnow(), "1T")
+    assert int(at.get_time_remaining()) == 60 - dt.utcnow().second - 1
+
+
+# ------------------------------------------
+
+
+async def async_ticker():
+    global gl_counter, iu_counter
+    gl_counter = 0
+    iu_counter = 1
+
+    global nr
+    nr = 3
+
+    t = AsyncTicker(tfunc, interval=I, sync=None, args=args, kw=kw, lock=0.2, keep=nr)
+    IU2 = AsyncTicker(IU, interval=I)
+    t3 = AsyncTicker(
+        tfunc, interval=IU, sync=None, lock="next", args=args, kw=kw, keep=nr
+    )
+
+    t4 = AsyncTicker(
+        tfunc,
+        interval=I,
+        sync=td(0, 1),
+        delay=D,
+        lock="next",
+        args=args,
+        kw=kw,
+        keep=nr,
+    )
+    t5 = AsyncTicker(
+        tfunc, interval=I, sync="first", delay=D, args=args, kw=kw, keep=nr
+    )
+    t6 = AsyncTicker(
+        tfunc,
+        interval=IU,
+        sync="first",
+        delay=D,
+        args=args,
+        kw=kw,
+        keep=nr,
+        name="TickerX6",
+    )
+
+    for x in (t, t3, t4, t5, t6):
+        for i in range(nr):
+            try:
+                await x.tick()
+            except WaitException as e:
+                logging.info("{}, {}, sleeping {}".format(x._name, i, e.wait_time))
+                # warnings.warn('{},{}, sleeping {}'.format(x._name,i,e.wait_time))
+                await asyncio.sleep(e.wait_time)
+                await x.tick()
+            finally:
+                if i == nr - 1 and x in (t3, t4, t5, t6):
+                    entries = list(x.entries)[::-1]
+                    records = list(x.records)[::-1]
+                    secs = [
+                        "{}.{}".format(y.second, int(to_us(y) / 1000)) for y in entries
+                    ]
+                    difs = [
+                        round((y - entries[i]) / td(seconds=1), int(4 / factor))
+                        for i, y in enumerate(entries[1:])
+                    ]
+                    # difs2 = [round((y[1]-y[0])/td(seconds=1),6) for y in records]
+                    logging.debug("{}\ndifs: {}\n".format(x._name, difs))  # ,difs2))
+
+    for x in (t, t3, t4, t5, t6):
+        with pytest.raises(TerminatedException):
+            print("verifying error")
+            await x.tick()
+            print("THIS SHOULD NOT BE PRINTED")
+
+    print("Async all passed")
+
+
+loop = asyncio.get_event_loop()
+
+
+def test_async_ticker():
+    loop.run_until_complete(asyncio.gather(*[async_ticker()], return_exceptions=False))
+
+
+# ------------------------------------------
+def test_tick_manager():
+    global gl_counter, iu_counter
+    gl_counter = 0
+    iu_counter = 1
+
+    t = Ticker(tfunc, interval=I, sync=None, args=args, kw=kw, lock=0.2, keep=nr)
+    t2 = Ticker(tfunc, interval=I, sync=None, args=args, kw=kw, lock=0.2, keep=nr)
+
+    tm = TickManager([t, t2])
+    tm.tick(errors="sleep")
+    tm.tick(errors="sleep")
+
+    t.close()
+    tm.tick(errors="sleep")
+
+    t2.close()
+
+    with pytest.raises(AllTerminated):
+        tm.tick()
+
+
+# ------------------------------------------
+
+
+async def async_tick_manager():
+    global gl_counter, iu_counter
+    gl_counter = 0
+    iu_counter = 1
+
+    cb = lambda x: print("{} completed at {}".format(x["ticker"]._name, dt.utcnow()))
+    e1 = asyncio.Event()
+    e2 = asyncio.Event()
+
+    def cb2(e):
+        def cb2_wapped(x):
+            print("{} completed at {}".format(x["ticker"]._name, dt.utcnow()))
+            e.set()
+
+        return cb2_wapped
+
+    t1 = AsyncTicker(
+        tfunc,
+        interval=I,
+        sync=None,
+        args=args,
+        kw=kw,
+        lock=0.2,
+        keep=nr,
+        callback=cb2(e1),
+    )
+    t2 = AsyncTicker(
+        tfunc,
+        interval=I,
+        sync=None,
+        args=args,
+        kw=kw,
+        lock=0.2,
+        keep=nr,
+        callback=cb2(e2),
+    )
+    tm = AsyncTickManager([t1, t2], loop=loop, allterminated="raise", callback=cb)
+
+    await tm.tick()
+    await tm.tick()
+
+    print("waiting till e1 set")
+    await e1.wait()
+    print("wait complete")
+
+    await t1.close()
+    print("t1 closed x1")
+    e2.clear()
+
+    await tm.tick()
+
+    print("waiting till e2 set")
+    await e2.wait()
+    print("wait complete")
+
+    await t2.close()
+    print("t2 closed")
+
+    with pytest.raises(AllTerminated):
+        await tm.tick()
+    print("tm .tick() raised Allterminated")
+
+    await tm.close()
+    print("tm._closed: {}".format(tm._closed))
+    with pytest.raises(TerminatedException):
+        await tm.tick()
+    print("tm .tick() raised TerminatedException")
+
+
+def test_async_tick_manager():
+    loop.run_until_complete(
+        asyncio.gather(*[async_tick_manager()], return_exceptions=False)
+    )
+
+
+async def async_tick_manager_loop():
+    global gl_counter, iu_counter
+    gl_counter = 0
+    iu_counter = 1
+
+    cb = lambda x: print("{} ticked at {}".format(x["ticker"]._name, dt.utcnow()))
+    e1 = asyncio.Event()
+    e2 = asyncio.Event()
+    e3 = asyncio.Event()
+
+    def cb2(e):
+        def cb2_wapped(x):
+            print("{} ticked at {}".format(x["ticker"]._name, dt.utcnow()))
+            e.set()
+
+        return cb2_wapped
+
+    t1 = AsyncTicker(
+        tfunc,
+        interval=I,
+        sync=None,
+        args=args,
+        kw=kw,
+        lock=0.2,
+        keep=nr,
+        callback=cb2(e1),
+        name="AT-1 of AsyncTickManagerMAIN",
+    )
+    t2 = AsyncTicker(
+        tfunc,
+        interval=I,
+        sync=None,
+        args=args,
+        kw=kw,
+        lock=0.2,
+        keep=nr,
+        callback=cb2(e2),
+        name="AT-2 of AsyncTickManagerMAIN",
+    )
+    tm = AsyncTickManager(
+        [t1, t2],
+        loop=loop,
+        allterminated="raise",
+        callback=cb,
+        name="AsyncTickManagerMAIN",
+    )
+
+    # assert e1.is_set()
+    # assert e2.is_set()
+
+    # tickers are automatically terminated at loop #nr
+    with pytest.raises(AllTerminated):
+        await tm.loop()
+
+
+def test_async_tick_manager_loop():
+    loop.run_until_complete(
+        asyncio.gather(*[async_tick_manager_loop()], return_exceptions=False)
+    )
+
+
+def test_routine():
+    async def rout_func(d={"i": 0}, break_at=2):
+        print(d)
+        d["i"] += 1
+        if d["i"] == break_at:
+            print("breaking")
+            raise QuitException
+
+    sched = {
+        "r1": {"target": rout_func, "kwargs": {"d": {"i": 0}}, "interval": 0.01},
+        "r2": {"target": rout_func, "kwargs": {"d": {"i": 0}, "break_at": 4}},
+    }
+    rout = Routine(sched, tickmgr={"allterminated": "close"})
+    loop.run_until_complete(asyncio.gather(*[rout.start()], return_exceptions=False))
+    assert sched["r1"]["kwargs"]["d"]["i"] == 2
+    assert sched["r2"]["kwargs"]["d"]["i"] == 4
+    assert rout.get_event("r1").is_set()
+    assert rout.get_event("r2").is_set()
+
+
+# def test_asynctickmgr_with_nonasynctickers():
+
+
+"""
+r2 = 'new_return'
+
+intervals = [td(seconds=0.1),0.1]
+exp_intervals = [intervals[0]] *2
+
+as_delay = [True,False,None,'e']
+
+delay = [td(seconds=0.05),0.05,None,dt(2000,1,1)]
+exp_delay = [delay[0]]*2 + [None,None]
+
+
+@pytest.mark.parametrized("interval","as_delay","delay","sync","exp")
+def test_basics(interval,as_delay,delay,sync,exp):
+    t = Ticker(tfunc,interval,as_delay,delay,sync=sync)
+    
+    assert t._ui['delay'] == exp['delay']
+    assert t._ui['as_delay'] == exp['as_delay']
+    
+    now = dt.utcnow()
+    t.tick()
+    
+    assert t._ui["interval"] == fontime.freq_to_offset(exp["interval"])
+    assert t.interval.delta = exp["interval"]
+    assert t.get_last() > now
+    assert t.get_actual_last() > now
+    assert t.sync == exp["sync"]
+    
+    
+def test_"""
```

### Comparing `fons-0.3.1/test/test_threads.py` & `fons-0.4.0/test/test_threads.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,28 @@
-import datetime
-dt = datetime.datetime
-td = datetime.timedelta
-
-from fons.threads import EliThread
-
-
-def raise_RuntimeError(counter=None):
-    if counter:
-        counter['i'] += 1
-    raise RuntimeError
-    
-    
-def test_EliThread_keepalive():
-    counter = {'i':0}
-    t = EliThread(target=raise_RuntimeError,args=(counter,),keepalive={'pause':0.01,'attempts':4},name='RuntimeRaisingEliThread')
-    started = dt.utcnow()
-    t.start()
-    t.join(0.08)
-    assert counter['i'] == 4
-    assert dt.utcnow() - started > td(seconds=0.04)
-    assert not t.is_alive()
+import datetime
+
+dt = datetime.datetime
+td = datetime.timedelta
+
+from fons.threads import EliThread
+
+
+def raise_RuntimeError(counter=None):
+    if counter:
+        counter["i"] += 1
+    raise RuntimeError
+
+
+def test_EliThread_keepalive():
+    counter = {"i": 0}
+    t = EliThread(
+        target=raise_RuntimeError,
+        args=(counter,),
+        keepalive={"pause": 0.01, "attempts": 4},
+        name="RuntimeRaisingEliThread",
+    )
+    started = dt.utcnow()
+    t.start()
+    t.join(0.08)
+    assert counter["i"] == 4
+    assert dt.utcnow() - started > td(seconds=0.04)
+    assert not t.is_alive()
```

### Comparing `fons-0.3.1/test/test_url.py` & `fons-0.4.0/test/test_url.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,70 @@
 from fons.net.url import expand_url, expand, strip_params, find_urls, expand_in_text
 
 
 def _test_expand_url():
-    url = 'https://t.co/L0t4lQ3hT7'
-    expected_seen = ['https://t.co/L0t4lQ3hT7', 'http://wef.ch/2yg5TRT', 'https://www.weforum.org/agenda/2017/09/dubai-has-successfully-tested-the-first-flying-taxi?utm_content=buffer98989&utm_medium=social&utm_source=twitter.com&utm_campaign=buffer']
+    url = "https://t.co/L0t4lQ3hT7"
+    expected_seen = [
+        "https://t.co/L0t4lQ3hT7",
+        "http://wef.ch/2yg5TRT",
+        "https://www.weforum.org/agenda/2017/09/dubai-has-successfully-tested-the-first-flying-taxi?utm_content=buffer98989&utm_medium=social&utm_source=twitter.com&utm_campaign=buffer",
+    ]
     seen = []
-    
-    assert expand_url(url,seen=seen) == expected_seen[-1]
+
+    assert expand_url(url, seen=seen) == expected_seen[-1]
     assert seen == expected_seen
-    
-    
+
+
 def _test_expand(nr=10):
-    urls = ['https://bit.ly/2rwwupw','https://bit.ly/2I6HWDu',
-            'https://t.co/ydBPKn4wO0','http://t.co/hAplNMmSTg',
-            'http://f-st.co/THHI6hC',
-            ]*nr
-    
-    expected = [x.lower() for x in
-                ('https://www.youtube.com/watch?v=Lvf8koqX_yE&feature=youtu.be', 
-                'https://www.youtube.com/watch?v=UrCs-GuAQDY&feature=youtu.be', 
-                'https://www.coindesk.com/bitcoin-lightning-payments-slowly-becoming-less-reckless/', 
-                'http://www.wtatennis.com/players/player/314320/title/simona-halep', 
-                'https://www.fastcodesign.com/3016456/this-note-taking-system-turns-you-into-an-efficiency-expert?utm_source=facebook'
-                )*nr ]
-    
+    urls = [
+        "https://bit.ly/2rwwupw",
+        "https://bit.ly/2I6HWDu",
+        "https://t.co/ydBPKn4wO0",
+        "http://t.co/hAplNMmSTg",
+        "http://f-st.co/THHI6hC",
+    ] * nr
+
+    expected = [
+        x.lower()
+        for x in (
+            "https://www.youtube.com/watch?v=Lvf8koqX_yE&feature=youtu.be",
+            "https://www.youtube.com/watch?v=UrCs-GuAQDY&feature=youtu.be",
+            "https://www.coindesk.com/bitcoin-lightning-payments-slowly-becoming-less-reckless/",
+            "http://www.wtatennis.com/players/player/314320/title/simona-halep",
+            "https://www.fastcodesign.com/3016456/this-note-taking-system-turns-you-into-an-efficiency-expert?utm_source=facebook",
+        )
+        * nr
+    ]
+
     expanded = [x.lower() if x is not None else x for x in expand(urls)]
-    
+
     assert expanded == expected
 
 
 def test_find_urls():
-    urls = ['https://t.co/ydBPKn4wO0','https://bit.ly/2I6HWDu','www.google.com?search=sth&p2=null','http://www.yahoo.com']
+    urls = [
+        "https://t.co/ydBPKn4wO0",
+        "https://bit.ly/2I6HWDu",
+        "www.google.com?search=sth&p2=null",
+        "http://www.yahoo.com",
+    ]
     temp = "Hello to you, {0}, this here:{1}.\n{2}\r{3}. end"
     text = temp.format(*urls)
-    expected = [[text.find(x),text.find(x)+len(x),x] for x in urls]
+    expected = [[text.find(x), text.find(x) + len(x), x] for x in urls]
     found = find_urls(text)
     assert [list(x) for x in found] == expected
-    
-    
+
+
 def _test_expand_urls_in_text():
-    text = "Hello to you, https://t.co/ydBPKn4wO0 , this here:https://bit.ly/2I6HWDu. end"
+    text = (
+        "Hello to you, https://t.co/ydBPKn4wO0 , this here:https://bit.ly/2I6HWDu. end"
+    )
     expanded = expand_in_text(text)
-    expected = "Hello to you, https://www.coindesk.com/bitcoin-lightning-payments-slowly-becoming-less-reckless/, this here:https://www.youtube.com/watch?v=UrCs-GuAQDY&feature=youtu.be. end" 
+    expected = "Hello to you, https://www.coindesk.com/bitcoin-lightning-payments-slowly-becoming-less-reckless/, this here:https://www.youtube.com/watch?v=UrCs-GuAQDY&feature=youtu.be. end"
     assert expanded == expected
-    
-    
+
+
 def test_strip_params():
-    url = 'https://www.weforum.org/agenda/2017/09/dubai-has-successfully-tested-the-first-flying-taxi?utm_content=buffer98989&utm_medium=social&utm_source=twitter.com&utm_campaign=buffer'
-    expected = 'https://www.weforum.org/agenda/2017/09/dubai-has-successfully-tested-the-first-flying-taxi?utm_content=buffer98989&utm_campaign=buffer'
-    
-    assert strip_params(url,['utm_source','utm_medium']) == expected
+    url = "https://www.weforum.org/agenda/2017/09/dubai-has-successfully-tested-the-first-flying-taxi?utm_content=buffer98989&utm_medium=social&utm_source=twitter.com&utm_campaign=buffer"
+    expected = "https://www.weforum.org/agenda/2017/09/dubai-has-successfully-tested-the-first-flying-taxi?utm_content=buffer98989&utm_campaign=buffer"
+
+    assert strip_params(url, ["utm_source", "utm_medium"]) == expected
```

