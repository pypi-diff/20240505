# Comparing `tmp/enconnect-0.3.0.tar.gz` & `tmp/enconnect-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enconnect-0.3.0.tar", last modified: Mon Apr 29 04:53:00 2024, max compression
+gzip compressed data, was "enconnect-0.4.0.tar", last modified: Sun May  5 05:18:47 2024, max compression
```

## Comparing `enconnect-0.3.0.tar` & `enconnect-0.4.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-29 04:53:00.083427 enconnect-0.3.0/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1071 2024-04-08 22:20:24.000000 enconnect-0.3.0/LICENSE
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       33 2024-04-08 22:21:35.000000 enconnect-0.3.0/MANIFEST.in
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2774 2024-04-29 04:53:00.083427 enconnect-0.3.0/PKG-INFO
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2363 2024-04-14 13:59:58.000000 enconnect-0.3.0/README.md
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-29 04:53:00.082427 enconnect-0.3.0/enconnect/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      525 2024-04-08 22:22:18.000000 enconnect-0.3.0/enconnect/__init__.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-29 04:53:00.082427 enconnect-0.3.0/enconnect/instagram/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      405 2024-04-13 00:00:49.000000 enconnect-0.3.0/enconnect/instagram/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6100 2024-04-29 04:47:32.000000 enconnect-0.3.0/enconnect/instagram/instagram.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      982 2024-04-12 05:18:12.000000 enconnect-0.3.0/enconnect/instagram/params.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-29 04:53:00.082427 enconnect-0.3.0/enconnect/instagram/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-12 04:42:12.000000 enconnect-0.3.0/enconnect/instagram/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3160 2024-04-29 04:47:32.000000 enconnect-0.3.0/enconnect/instagram/test/test_instagram.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-29 04:53:00.082427 enconnect-0.3.0/enconnect/philipshue/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      330 2024-04-14 11:22:18.000000 enconnect-0.3.0/enconnect/philipshue/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2254 2024-04-14 11:29:01.000000 enconnect-0.3.0/enconnect/philipshue/bridge.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      955 2024-04-14 11:21:24.000000 enconnect-0.3.0/enconnect/philipshue/params.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-29 04:53:00.082427 enconnect-0.3.0/enconnect/philipshue/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-14 11:30:44.000000 enconnect-0.3.0/enconnect/philipshue/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1773 2024-04-15 09:01:50.000000 enconnect-0.3.0/enconnect/philipshue/test/test_bridge.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-08 22:21:56.000000 enconnect-0.3.0/enconnect/py.typed
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-29 04:53:00.082427 enconnect-0.3.0/enconnect/reddit/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      385 2024-04-13 11:18:53.000000 enconnect-0.3.0/enconnect/reddit/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      954 2024-04-25 02:11:28.000000 enconnect-0.3.0/enconnect/reddit/params.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     7184 2024-04-29 04:47:32.000000 enconnect-0.3.0/enconnect/reddit/reddit.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-29 04:53:00.083427 enconnect-0.3.0/enconnect/reddit/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-13 07:05:56.000000 enconnect-0.3.0/enconnect/reddit/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3117 2024-04-29 04:47:32.000000 enconnect-0.3.0/enconnect/reddit/test/test_reddit.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-29 04:53:00.083427 enconnect-0.3.0/enconnect/ubiquiti/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      330 2024-04-14 11:22:46.000000 enconnect-0.3.0/enconnect/ubiquiti/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1127 2024-04-14 11:21:29.000000 enconnect-0.3.0/enconnect/ubiquiti/params.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4320 2024-04-25 02:26:38.000000 enconnect-0.3.0/enconnect/ubiquiti/router.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-29 04:53:00.083427 enconnect-0.3.0/enconnect/ubiquiti/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-14 11:30:52.000000 enconnect-0.3.0/enconnect/ubiquiti/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2199 2024-04-15 09:01:50.000000 enconnect-0.3.0/enconnect/ubiquiti/test/test_router.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-29 04:53:00.083427 enconnect-0.3.0/enconnect/utils/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      283 2024-04-29 00:13:14.000000 enconnect-0.3.0/enconnect/utils/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6507 2024-04-29 04:47:32.000000 enconnect-0.3.0/enconnect/utils/http.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-29 04:53:00.083427 enconnect-0.3.0/enconnect/utils/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-29 00:13:14.000000 enconnect-0.3.0/enconnect/utils/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2862 2024-04-29 00:13:14.000000 enconnect-0.3.0/enconnect/utils/test/test_http.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        6 2024-04-29 04:48:48.000000 enconnect-0.3.0/enconnect/version.txt
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-29 04:53:00.083427 enconnect-0.3.0/enconnect/youtube/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      391 2024-04-12 07:52:09.000000 enconnect-0.3.0/enconnect/youtube/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      979 2024-04-12 06:47:27.000000 enconnect-0.3.0/enconnect/youtube/params.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-29 04:53:00.083427 enconnect-0.3.0/enconnect/youtube/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-12 07:23:02.000000 enconnect-0.3.0/enconnect/youtube/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3212 2024-04-29 04:47:32.000000 enconnect-0.3.0/enconnect/youtube/test/test_youtube.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     7648 2024-04-29 04:47:32.000000 enconnect-0.3.0/enconnect/youtube/youtube.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-29 04:53:00.083427 enconnect-0.3.0/enconnect.egg-info/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2774 2024-04-29 04:53:00.000000 enconnect-0.3.0/enconnect.egg-info/PKG-INFO
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1245 2024-04-29 04:53:00.000000 enconnect-0.3.0/enconnect.egg-info/SOURCES.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        1 2024-04-29 04:53:00.000000 enconnect-0.3.0/enconnect.egg-info/dependency_links.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       24 2024-04-29 04:53:00.000000 enconnect-0.3.0/enconnect.egg-info/requires.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       10 2024-04-29 04:53:00.000000 enconnect-0.3.0/enconnect.egg-info/top_level.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      529 2024-04-08 22:22:47.000000 enconnect-0.3.0/pyproject.toml
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       24 2024-04-29 00:13:14.000000 enconnect-0.3.0/reqs-install.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      305 2024-04-29 04:53:00.084427 enconnect-0.3.0/setup.cfg
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-05 05:18:47.162314 enconnect-0.4.0/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1071 2024-04-08 22:20:24.000000 enconnect-0.4.0/LICENSE
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       33 2024-04-08 22:21:35.000000 enconnect-0.4.0/MANIFEST.in
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2828 2024-05-05 05:18:47.162314 enconnect-0.4.0/PKG-INFO
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2417 2024-05-05 05:12:09.000000 enconnect-0.4.0/README.md
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-05 05:18:47.160314 enconnect-0.4.0/enconnect/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      525 2024-04-08 22:22:18.000000 enconnect-0.4.0/enconnect/__init__.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-05 05:18:47.161314 enconnect-0.4.0/enconnect/instagram/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      405 2024-04-13 00:00:49.000000 enconnect-0.4.0/enconnect/instagram/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6092 2024-05-05 05:10:19.000000 enconnect-0.4.0/enconnect/instagram/instagram.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      881 2024-05-05 05:10:19.000000 enconnect-0.4.0/enconnect/instagram/params.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-05 05:18:47.161314 enconnect-0.4.0/enconnect/instagram/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-12 04:42:12.000000 enconnect-0.4.0/enconnect/instagram/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3314 2024-05-05 05:10:19.000000 enconnect-0.4.0/enconnect/instagram/test/test_instagram.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-05 05:18:47.161314 enconnect-0.4.0/enconnect/philipshue/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      330 2024-04-14 11:22:18.000000 enconnect-0.4.0/enconnect/philipshue/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2254 2024-04-14 11:29:01.000000 enconnect-0.4.0/enconnect/philipshue/bridge.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      955 2024-04-14 11:21:24.000000 enconnect-0.4.0/enconnect/philipshue/params.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-05 05:18:47.161314 enconnect-0.4.0/enconnect/philipshue/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-14 11:30:44.000000 enconnect-0.4.0/enconnect/philipshue/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1773 2024-04-15 09:01:50.000000 enconnect-0.4.0/enconnect/philipshue/test/test_bridge.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-08 22:21:56.000000 enconnect-0.4.0/enconnect/py.typed
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-05 05:18:47.161314 enconnect-0.4.0/enconnect/reddit/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      385 2024-04-13 11:18:53.000000 enconnect-0.4.0/enconnect/reddit/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1197 2024-05-05 04:49:10.000000 enconnect-0.4.0/enconnect/reddit/params.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)    11372 2024-05-05 05:10:19.000000 enconnect-0.4.0/enconnect/reddit/reddit.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-05 05:18:47.161314 enconnect-0.4.0/enconnect/reddit/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-13 07:05:56.000000 enconnect-0.4.0/enconnect/reddit/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4478 2024-05-05 05:10:19.000000 enconnect-0.4.0/enconnect/reddit/test/test_reddit.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-05 05:18:47.161314 enconnect-0.4.0/enconnect/ubiquiti/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      330 2024-04-14 11:22:46.000000 enconnect-0.4.0/enconnect/ubiquiti/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1127 2024-04-14 11:21:29.000000 enconnect-0.4.0/enconnect/ubiquiti/params.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4376 2024-05-05 05:10:19.000000 enconnect-0.4.0/enconnect/ubiquiti/router.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-05 05:18:47.162314 enconnect-0.4.0/enconnect/ubiquiti/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-14 11:30:52.000000 enconnect-0.4.0/enconnect/ubiquiti/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2199 2024-04-15 09:01:50.000000 enconnect-0.4.0/enconnect/ubiquiti/test/test_router.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-05 05:18:47.162314 enconnect-0.4.0/enconnect/utils/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      283 2024-04-29 00:13:14.000000 enconnect-0.4.0/enconnect/utils/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     8682 2024-05-05 04:49:10.000000 enconnect-0.4.0/enconnect/utils/http.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-05 05:18:47.162314 enconnect-0.4.0/enconnect/utils/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-29 00:13:14.000000 enconnect-0.4.0/enconnect/utils/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2996 2024-05-05 04:49:10.000000 enconnect-0.4.0/enconnect/utils/test/test_http.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        6 2024-05-05 05:13:11.000000 enconnect-0.4.0/enconnect/version.txt
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-05 05:18:47.162314 enconnect-0.4.0/enconnect/youtube/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      391 2024-04-12 07:52:09.000000 enconnect-0.4.0/enconnect/youtube/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      879 2024-05-05 05:10:19.000000 enconnect-0.4.0/enconnect/youtube/params.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-05 05:18:47.162314 enconnect-0.4.0/enconnect/youtube/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-12 07:23:02.000000 enconnect-0.4.0/enconnect/youtube/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3446 2024-05-05 05:10:19.000000 enconnect-0.4.0/enconnect/youtube/test/test_youtube.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     7638 2024-05-05 05:10:19.000000 enconnect-0.4.0/enconnect/youtube/youtube.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-05 05:18:47.162314 enconnect-0.4.0/enconnect.egg-info/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2828 2024-05-05 05:18:47.000000 enconnect-0.4.0/enconnect.egg-info/PKG-INFO
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1245 2024-05-05 05:18:47.000000 enconnect-0.4.0/enconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        1 2024-05-05 05:18:47.000000 enconnect-0.4.0/enconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       24 2024-05-05 05:18:47.000000 enconnect-0.4.0/enconnect.egg-info/requires.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       10 2024-05-05 05:18:47.000000 enconnect-0.4.0/enconnect.egg-info/top_level.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      529 2024-04-08 22:22:47.000000 enconnect-0.4.0/pyproject.toml
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       24 2024-04-29 00:13:14.000000 enconnect-0.4.0/reqs-install.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      339 2024-05-05 05:18:47.162314 enconnect-0.4.0/setup.cfg
```

### Comparing `enconnect-0.3.0/LICENSE` & `enconnect-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `enconnect-0.3.0/PKG-INFO` & `enconnect-0.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enconnect
-Version: 0.3.0
+Version: 0.4.0
 Summary: Enasis Network Remote Connect
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -66,14 +66,18 @@
 And finally run the various tests to validate the code and produce coverage
 information found in the `htmlcov` folder in the root of the project.
 ```
 make -s pytest
 ```
 
 ## Build and upload to PyPi
+Rebuild the environment.
+```
+make -s check-revenv
+```
 Build the package.
 ```
 make -s pypackage
 ```
 Upload to the test PyPi.
 ```
 make -s pypi-upload-test
```

### Comparing `enconnect-0.3.0/README.md` & `enconnect-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,18 @@
 And finally run the various tests to validate the code and produce coverage
 information found in the `htmlcov` folder in the root of the project.
 ```
 make -s pytest
 ```
 
 ## Build and upload to PyPi
+Rebuild the environment.
+```
+make -s check-revenv
+```
 Build the package.
 ```
 make -s pypackage
 ```
 Upload to the test PyPi.
 ```
 make -s pypi-upload-test
```

### Comparing `enconnect-0.3.0/enconnect/__init__.py` & `enconnect-0.4.0/enconnect/__init__.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.3.0/enconnect/instagram/instagram.py` & `enconnect-0.4.0/enconnect/instagram/instagram.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,19 +155,19 @@
         :param path: Path for the location to upstream endpoint.
         :param params: Optional parameters included in request.
         :returns: Response for upstream request to the server.
         """
 
         params = dict(params or {})
 
-        server = self.params.server
-        token = self.params.token
+        server = 'graph.instagram.com'
         client = self.client
 
-        params['access_token'] = token
+        params['access_token'] = (
+            self.params.token)
 
         location = (
             f'https://{server}/{path}')
 
         request = client.request_block
 
         return request(
@@ -189,19 +189,19 @@
         :param path: Path for the location to upstream endpoint.
         :param params: Optional parameters included in request.
         :returns: Response for upstream request to the server.
         """
 
         params = dict(params or {})
 
-        server = self.params.server
-        token = self.params.token
+        server = 'graph.instagram.com'
         client = self.client
 
-        params['access_token'] = token
+        params['access_token'] = (
+            self.params.token)
 
         location = (
             f'https://{server}/{path}')
 
         request = client.request_async
 
         return await request(
```

### Comparing `enconnect-0.3.0/enconnect/instagram/params.py` & `enconnect-0.4.0/enconnect/reddit/params.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,27 +9,33 @@
 
 from typing import Optional
 
 from pydantic import BaseModel
 
 
 
-class InstagramParams(BaseModel, extra='forbid'):
+class RedditParams(BaseModel, extra='forbid'):
     """
     Process and validate the class configuration parameters.
 
-    :param server: Host or IP address for server connection.
     :param timeout: Timeout when waiting for server response.
-    :param token: Token used when authenticating to server.
+    :param username: Username for authenticating with server.
+    :param password: Password for authenticating with server.
+    :param client: Token used when authenticating to server.
+    :param secret: Token used when authenticating to server.
+    :param useragent: Reddit has specifics about this value.
     :param ssl_verify: Require valid certificate from server.
     :param ssl_capem: Optional path to certificate authority.
     :param data: Keyword arguments passed to Pydantic model.
         Parameter is picked up by autodoc, please ignore.
     """
 
-    server: str = 'graph.instagram.com'
     timeout: int = 30
 
-    token: str
+    username: str
+    password: str
+    client: str
+    secret: str
+    useragent: str
 
     ssl_verify: bool = True
     ssl_capem: Optional[str] = None
```

### Comparing `enconnect-0.3.0/enconnect/instagram/test/test_instagram.py` & `enconnect-0.4.0/enconnect/instagram/test/test_instagram.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,14 +26,18 @@
 
 from . import SAMPLES
 from ..instagram import Instagram
 from ..params import InstagramParams
 
 
 
+_REQGET = Request('get', SEMPTY)
+
+
+
 @fixture
 def social() -> Instagram:
     """
     Construct the instance for use in the downstream tests.
 
     :returns: Newly constructed instance of related class.
     """
@@ -72,29 +76,38 @@
         'instagram.Instagram object',
         social)
 
 
     assert social.params is not None
 
 
+
+def test_Instagram_block(
+    social: Instagram,
+) -> None:
+    """
+    Perform various tests associated with relevant routines.
+
+    :param social: Class instance for connecting to service.
+    """
+
+
     patched = patch(
         'httpx.Client.request')
 
     with patched as mocker:
 
         source = read_text(
             f'{SAMPLES}/source.json')
 
-        request = Request('get', SEMPTY)
-
         mocker.side_effect = [
             Response(
                 status_code=200,
                 content=source,
-                request=request)]
+                request=_REQGET)]
 
         media = social.latest_block()
 
 
     sample_path = (
         f'{SAMPLES}/dumped.json')
 
@@ -128,21 +141,19 @@
         new_callable=AsyncMock)
 
     with patched as mocker:
 
         source = read_text(
             f'{SAMPLES}/source.json')
 
-        request = Request('get', SEMPTY)
-
         mocker.side_effect = [
             Response(
                 status_code=200,
                 content=source,
-                request=request)]
+                request=_REQGET)]
 
         waited = social.latest_async()
 
         media = await waited
 
 
     sample_path = (
```

### Comparing `enconnect-0.3.0/enconnect/philipshue/bridge.py` & `enconnect-0.4.0/enconnect/philipshue/bridge.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.3.0/enconnect/philipshue/params.py` & `enconnect-0.4.0/enconnect/philipshue/params.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.3.0/enconnect/philipshue/test/test_bridge.py` & `enconnect-0.4.0/enconnect/philipshue/test/test_bridge.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.3.0/enconnect/reddit/params.py` & `enconnect-0.4.0/enconnect/youtube/params.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 
 from typing import Optional
 
 from pydantic import BaseModel
 
 
 
-class RedditParams(BaseModel, extra='forbid'):
+class YouTubeParams(BaseModel, extra='forbid'):
     """
     Process and validate the class configuration parameters.
 
-    :param server: Host or IP address for server connection.
     :param timeout: Timeout when waiting for server response.
     :param token: Token used when authenticating to server.
     :param ssl_verify: Require valid certificate from server.
     :param ssl_capem: Optional path to certificate authority.
     :param data: Keyword arguments passed to Pydantic model.
         Parameter is picked up by autodoc, please ignore.
     """
 
-    server: str = 'reddit.com'
     timeout: int = 30
 
+    token: str
+
     ssl_verify: bool = True
     ssl_capem: Optional[str] = None
```

### Comparing `enconnect-0.3.0/enconnect/reddit/reddit.py` & `enconnect-0.4.0/enconnect/youtube/youtube.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,137 +7,142 @@
 
 
 
 from typing import Any
 from typing import Literal
 from typing import Optional
 from typing import TYPE_CHECKING
-
-from encommon.types import getate
+from typing import get_args
 
 from httpx import Response
 
 from pydantic import BaseModel
 
 from ..utils import HTTPClient
 
 if TYPE_CHECKING:
-    from .params import RedditParams
+    from .params import YouTubeParams
+
+
+
+RESULT_KINDS = Literal[
+    'channel',
+    'playlist',
+    'video']
 
+_RESULT_KINDS = [
+    f'youtube#{x}' for x in
+    get_args(RESULT_KINDS)]
 
 
-LISTING_VALUE = {
-    'created_utc': 'created',
-    'ups': 'vote_ups',
-    'downs': 'vote_downs',
-    'url_overridden_by_dest': 'url_dest',
-    'media_metadata': 'medias'}
 
+RESULT_VALUE = {
+    'channelId': 'channel',
+    'channelTitle': 'channel_title',
+    'description': 'about',
+    'publishedAt': 'published',
+    'thumbnails': 'thumbnail',
+    'title': 'title'}
 
+RESULT_BASIC = {
+    'channelId': 'channel',
+    'kind': 'kind',
+    'playlistId': 'playlist',
+    'videoId': 'video'}
 
-class RedditListing(BaseModel, extra='ignore'):
+
+
+class YouTubeResult(BaseModel, extra='ignore'):
     """
     Contains information returned from the upstream response.
 
     .. note::
        Fields are not completely documented for this model.
 
     :param data: Keyword arguments passed to Pydantic model.
         Parameter is picked up by autodoc, please ignore.
     """
 
-    name: str
-    id: str
-    created: int
-    title: str
-    selftext: Optional[str] = None
-    author: str
-
-    url: str
-    permalink: str
-    thumbnail: str
-    url_dest: Optional[str] = None
-    domain: str
-
-    medias: Optional[list[str]] = None
+    kind: RESULT_KINDS
 
-    pinned: bool
-    edited: bool | float
-    stickied: bool
-    archived: bool
+    channel: Optional[str] = None
+    playlist: Optional[str] = None
+    video: Optional[str] = None
 
-    vote_downs: int
-    vote_ups: int
-
-    score: int
+    title: str
+    about: Optional[str] = None
+    channel_title: Optional[str] = None
+    thumbnail: str
+    published: str
 
 
     def __init__(
         self,
         **data: Any,
     ) -> None:
         """
         Initialize instance for class using provided parameters.
         """
 
-        items = LISTING_VALUE.items()
+
+        basic = data.get('id', {})
+
+        items = RESULT_BASIC.items()
 
         for old, new in items:
 
-            value = data.get(old)
+            value = basic.get(old)
 
             if value is None:
                 continue
 
             data[new] = value
 
 
-        data = {
-            k: v for k, v in
-            data.items()
-            if v not in ['', None]}
-
+        match = data.get('snippet', {})
 
-        if data.get('medias'):
+        items = RESULT_VALUE.items()
 
-            images: list[str] = []
+        for old, new in items:
 
-            items = data['medias'].items()
+            value = match.get(old)
 
-            for _, media in items:
+            if value is None:
+                continue  # NOCVR
 
-                assert isinstance(media, dict)
+            data[new] = value
 
-                image = getate(media, 's/u')
 
-                assert isinstance(image, str)
+        if 'thumbnail' in data:
+            data['thumbnail'] = (
+                data['thumbnail']
+                ['high']['url'])
 
-                images.append(image)
 
-            data['medias'] = images
+        data['kind'] = data['kind'][8:]
 
 
         super().__init__(**data)
 
 
 
-class Reddit:
+class YouTube:
     """
     Interact with the cloud service API with various methods.
 
     :param params: Parameters for instantiating the instance.
     """
 
-    __params: 'RedditParams'
+    __params: 'YouTubeParams'
     __client: HTTPClient
 
 
     def __init__(
         self,
-        params: 'RedditParams',
+        params: 'YouTubeParams',
     ) -> None:
         """
         Initialize instance for class using provided parameters.
         """
 
         self.__params = params
 
@@ -148,15 +153,15 @@
 
         self.__client = client
 
 
     @property
     def params(
         self,
-    ) -> 'RedditParams':
+    ) -> 'YouTubeParams':
         """
         Return the Pydantic model containing the configuration.
 
         :returns: Pydantic model containing the configuration.
         """
 
         return self.__params
@@ -188,19 +193,23 @@
         :param path: Path for the location to upstream endpoint.
         :param params: Optional parameters included in request.
         :returns: Response for upstream request to the server.
         """
 
         params = dict(params or {})
 
-        server = self.params.server
+        server = 'www.googleapis.com'
         client = self.client
 
+        params['key'] = (
+            self.params.token)
+
         location = (
-            f'https://{server}/{path}')
+            f'https://{server}/'
+            f'youtube/v3/{path}')
 
         request = client.request_block
 
         return request(
             method=method,
             location=location,
             params=params)
@@ -219,108 +228,124 @@
         :param path: Path for the location to upstream endpoint.
         :param params: Optional parameters included in request.
         :returns: Response for upstream request to the server.
         """
 
         params = dict(params or {})
 
-        server = self.params.server
+        server = 'www.googleapis.com'
         client = self.client
 
+        params['key'] = (
+            self.params.token)
+
         location = (
-            f'https://{server}/{path}')
+            f'https://{server}/'
+            f'youtube/v3/{path}')
 
         request = client.request_async
 
         return await request(
             method=method,
             location=location,
             params=params)
 
 
-    def latest(
+    def search(
         # NOCVR
         self,
-        subred: str,
         params: Optional[dict[str, Any]] = None,
-    ) -> list[RedditListing]:
+    ) -> list[YouTubeResult]:
         """
-        Return the new items within the provided subreddit path.
+        Return the results from the provided search parameters.
 
-        :param subred: Path to subreddit containing the content.
         :param params: Optional parameters included in request.
-        :returns: New items within the provided subreddit path.
+        :returns: Results from the provided search parameters.
         """
 
-        return self.latest_block(subred, params)
+        return self.search_block(params)
 
 
-    def latest_block(
+    def search_block(
         self,
-        subred: str,
         params: Optional[dict[str, Any]] = None,
-    ) -> list[RedditListing]:
+    ) -> list[YouTubeResult]:
         """
-        Return the new items within the provided subreddit path.
+        Return the results from the provided search parameters.
 
-        :param subred: Path to subreddit containing the content.
         :param params: Optional parameters included in request.
-        :returns: New items within the provided subreddit path.
+        :returns: Results from the provided search parameters.
         """
 
         params = dict(params or {})
 
 
+        if 'maxResults' not in params:
+            params['maxResults'] = 50
+
+        if 'order' not in params:
+            params['order'] = 'date'
+
+        if 'part' not in params:
+            params['part'] = 'snippet,id'
+
+
         request = self.request_block
 
         response = request(
-            'get', f'r/{subred}/new.json')
+            'get', 'search', params)
 
         response.raise_for_status()
 
         fetched = response.json()
 
         assert isinstance(fetched, dict)
 
 
-        source = fetched['data']
-        children = source['children']
-
         return [
-            RedditListing(**x['data'])
-            for x in children]
+            YouTubeResult(**x)
+            for x in fetched['items']
+            if x['id']['kind']
+            in _RESULT_KINDS]
 
 
-    async def latest_async(
+    async def search_async(
         self,
-        subred: str,
         params: Optional[dict[str, Any]] = None,
-    ) -> list[RedditListing]:
+    ) -> list[YouTubeResult]:
         """
-        Return the new items within the provided subreddit path.
+        Return the results from the provided search parameters.
 
-        :param subred: Path to subreddit containing the content.
         :param params: Optional parameters included in request.
-        :returns: New items within the provided subreddit path.
+        :returns: Results from the provided search parameters.
         """
 
         params = dict(params or {})
 
 
+        if 'maxResults' not in params:
+            params['maxResults'] = 50
+
+        if 'order' not in params:
+            params['order'] = 'date'
+
+        if 'part' not in params:
+            params['part'] = 'snippet,id'
+
+
         request = self.request_async
 
         response = await request(
-            'get', f'r/{subred}/new.json')
+            'get', 'search', params)
 
         response.raise_for_status()
 
         fetched = response.json()
 
         assert isinstance(fetched, dict)
 
 
-        source = fetched['data']
-        children = source['children']
-
         return [
-            RedditListing(**x['data'])
-            for x in children]
+            YouTubeResult(**x)
+            for x in fetched['items']
+            if x['id']['kind']
+            in _RESULT_KINDS]
```

### Comparing `enconnect-0.3.0/enconnect/reddit/test/test_reddit.py` & `enconnect-0.4.0/enconnect/youtube/test/test_youtube.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,103 +21,121 @@
 from httpx import Request
 from httpx import Response
 
 from pytest import fixture
 from pytest import mark
 
 from . import SAMPLES
-from ..params import RedditParams
-from ..reddit import Reddit
+from ..params import YouTubeParams
+from ..youtube import YouTube
+
+
+
+_REQGET = Request('get', SEMPTY)
 
 
 
 @fixture
-def social() -> Reddit:
+def social() -> YouTube:
     """
     Construct the instance for use in the downstream tests.
 
     :returns: Newly constructed instance of related class.
     """
 
-    params = RedditParams()
+    params = YouTubeParams(
+        token='mocked')
 
-    return Reddit(params)
+    return YouTube(params)
 
 
 
-def test_Reddit(
-    social: Reddit,
+def test_YouTube(
+    social: YouTube,
 ) -> None:
     """
     Perform various tests associated with relevant routines.
 
     :param social: Class instance for connecting to service.
     """
 
 
     attrs = list(social.__dict__)
 
     assert attrs == [
-        '_Reddit__params',
-        '_Reddit__client']
+        '_YouTube__params',
+        '_YouTube__client']
 
 
     assert inrepr(
-        'reddit.Reddit object',
+        'youtube.YouTube object',
         social)
 
     assert hash(social) > 0
 
     assert instr(
-        'reddit.Reddit object',
+        'youtube.YouTube object',
         social)
 
 
     assert social.params is not None
 
 
+
+def test_YouTube_block(
+    social: YouTube,
+) -> None:
+    """
+    Perform various tests associated with relevant routines.
+
+    :param social: Class instance for connecting to service.
+    """
+
+
     patched = patch(
         'httpx.Client.request')
 
     with patched as mocker:
 
         source = read_text(
             f'{SAMPLES}/source.json')
 
-        request = Request('get', SEMPTY)
-
         mocker.side_effect = [
             Response(
                 status_code=200,
                 content=source,
-                request=request)]
+                request=_REQGET)]
+
+        payload = {'channelId': 'mocked'}
 
-        listing = social.latest_block('mocked')
+        results = (
+            social
+            .search_block(payload))
 
 
     sample_path = (
         f'{SAMPLES}/dumped.json')
 
     sample = load_sample(
         sample_path,
         [x.model_dump()
-         for x in listing],
+         for x in results],
         update=ENPYRWS)
 
     expect = prep_sample([
         x.model_dump()
-        for x in listing])
+        for x in results])
 
     assert sample == expect
 
 
 
 @mark.asyncio
-async def test_Reddit_async(
-    social: Reddit,
+async def test_YouTube_async(
+    social: YouTube,
 ) -> None:
     """
     Perform various tests associated with relevant routines.
 
     :param social: Class instance for connecting to service.
     """
 
@@ -127,34 +145,36 @@
         new_callable=AsyncMock)
 
     with patched as mocker:
 
         source = read_text(
             f'{SAMPLES}/source.json')
 
-        request = Request('get', SEMPTY)
-
         mocker.side_effect = [
             Response(
                 status_code=200,
                 content=source,
-                request=request)]
+                request=_REQGET)]
+
+        payload = {'channelId': 'mocked'}
 
-        waited = social.latest_async('mocked')
+        waited = (
+            social
+            .search_async(payload))
 
-        listing = await waited
+        results = await waited
 
 
     sample_path = (
         f'{SAMPLES}/dumped.json')
 
     sample = load_sample(
         sample_path,
         [x.model_dump()
-         for x in listing],
+         for x in results],
         update=ENPYRWS)
 
     expect = prep_sample([
         x.model_dump()
-        for x in listing])
+        for x in results])
 
     assert sample == expect
```

### Comparing `enconnect-0.3.0/enconnect/ubiquiti/params.py` & `enconnect-0.4.0/enconnect/ubiquiti/params.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.3.0/enconnect/ubiquiti/router.py` & `enconnect-0.4.0/enconnect/ubiquiti/router.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,18 +74,20 @@
         """
         Establish new session obtaining cookie for authorization.
 
         :returns: Response for upstream request to the server.
         """
 
         params = self.params
+        username = params.username
+        password = params.password
 
         payload = {
-            'username': params.username,
-            'password': params.password}
+            'username': username,
+            'password': password}
 
         response = self.request(
             method='post',
             path='api/auth/login',
             json=payload)
 
         response.raise_for_status()
```

### Comparing `enconnect-0.3.0/enconnect/ubiquiti/test/test_router.py` & `enconnect-0.4.0/enconnect/ubiquiti/test/test_router.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.3.0/enconnect/utils/http.py` & `enconnect-0.4.0/enconnect/utils/http.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 This file is part of Enasis Network software eco-system. Distribution
 is permitted, for more information consult the project license file.
 """
 
 
 
 import asyncio
+from copy import deepcopy
 from time import sleep
 from typing import Any
 from typing import Literal
 from typing import Optional
 
 from httpx import AsyncClient
 from httpx import Client as BlockClient
@@ -19,73 +20,94 @@
 from httpx._types import VerifyTypes
 
 
 
 _METHODS = Literal[
     'delete',
     'get',
+    'post',
     'patch',
     'put']
 
+_HTTPAUTH = tuple[str, str]
+
+_HEADERS = dict[str, str]
+
+_PAYLOAD = dict[str, Any]
+
 
 
 class HTTPClient:
     """
     Interact with the upstream server in blocking or async.
 
     :param timeout: Timeout when waiting for server response.
+    :param headers: Optional headers to include in requests.
     :param verify: Require valid certificate from the server.
     :param capem: Optional path to the certificate authority.
+    :param httpauth: Optional information for authentication.
     :param retry: How many attempts are made with the server.
     :param backoff: Backoff backoff if encountered retries.
     :param states: Which states will be retried with backoff.
     """
 
     __timeout: int
+    __headers: Optional[_HEADERS]
     __verify: VerifyTypes
     __capem: Optional[str]
+    __httpauth: Optional[_HTTPAUTH]
     __retry: int
     __backoff: float
     __states: set[int]
 
     __client_block: BlockClient
     __client_async: AsyncClient
 
 
     def __init__(  # noqa: CFQ002
         self,
         timeout: int = 30,
+        headers: Optional[_HEADERS] = None,
         verify: VerifyTypes = True,
         capem: Optional[str] = None,
+        httpauth: Optional[_HTTPAUTH] = None,
         retry: int = 3,
         backoff: float = 3.0,
         states: set[int] = {429},
     ) -> None:
         """
         Initialize instance for class using provided parameters.
         """
 
         timeout = int(timeout)
+        headers = deepcopy(headers)
+        httpauth = deepcopy(httpauth)
         retry = int(retry)
         backoff = float(backoff)
         states = set(states)
 
         client_block = BlockClient(
             timeout=timeout,
+            headers=headers or None,
+            auth=httpauth or None,
             verify=capem or verify,
             follow_redirects=True)
 
         client_async = AsyncClient(
             timeout=timeout,
+            headers=headers or None,
+            auth=httpauth or None,
             verify=capem or verify,
             follow_redirects=True)
 
         self.__timeout = timeout
+        self.__headers = headers
         self.__verify = verify
         self.__capem = capem
+        self.__httpauth = httpauth
         self.__retry = retry
         self.__backoff = backoff
         self.__states = states
 
         self.__client_block = client_block
         self.__client_async = client_async
 
@@ -100,14 +122,40 @@
         :returns: Value for the attribute from class instance.
         """
 
         return self.__timeout
 
 
     @property
+    def httpauth(
+        self,
+    ) -> Optional[_HTTPAUTH]:
+        """
+        Return the value for the attribute from class instance.
+
+        :returns: Value for the attribute from class instance.
+        """
+
+        return deepcopy(self.__httpauth)
+
+
+    @property
+    def headers(
+        self,
+    ) -> Optional[_HEADERS]:
+        """
+        Return the value for the attribute from class instance.
+
+        :returns: Value for the attribute from class instance.
+        """
+
+        return deepcopy(self.__headers)
+
+
+    @property
     def verify(
         self,
     ) -> VerifyTypes:
         """
         Return the value for the attribute from class instance.
 
         :returns: Value for the attribute from class instance.
@@ -190,28 +238,35 @@
 
         :returns: Value for the attribute from class instance.
         """
 
         return self.__client_async
 
 
-    def request_block(
+    def request_block(  # noqa: CFQ002
         self,
         method: _METHODS,
         location: str,
-        params: Optional[dict[str, Any]] = None,
-        json: Optional[dict[str, Any]] = None,
+        params: Optional[_PAYLOAD] = None,
+        json: Optional[_PAYLOAD] = None,
+        *,
+        data: Optional[_PAYLOAD] = None,
+        headers: Optional[_HEADERS] = None,
+        httpauth: Optional[_HTTPAUTH] = None,
     ) -> Response:
         """
         Return the response for upstream request to the server.
 
         :param method: Method for operation with the API server.
         :param location: Location with path for server request.
         :param params: Optional parameters included in request.
         :param json: Optional JSON payload included in request.
+        :param data: Optional dict payload included in request.
+        :param headers: Optional headers to include in requests.
+        :param httpauth: Optional information for authentication.
         :returns: Response for upstream request to the server.
         """
 
         retry = self.retry
         backoff = self.backoff
         states = self.states
 
@@ -219,41 +274,51 @@
         request = client.request
 
         for count in range(retry):
 
             response = request(
                 method=method,
                 url=location,
-                params=params,
-                json=json)
+                headers=headers or None,
+                params=params or None,
+                data=data or None,
+                json=json or None,
+                auth=httpauth or None)
 
             status = response.status_code
 
             if status not in states:
                 break
 
             sleep(backoff)
 
         return response
 
 
-    async def request_async(
+    async def request_async(  # noqa: CFQ002
         self,
         method: _METHODS,
         location: str,
-        params: Optional[dict[str, Any]] = None,
-        json: Optional[dict[str, Any]] = None,
+        params: Optional[_PAYLOAD] = None,
+        json: Optional[_PAYLOAD] = None,
+        *,
+        data: Optional[_PAYLOAD] = None,
+        headers: Optional[_HEADERS] = None,
+        httpauth: Optional[_HTTPAUTH] = None,
     ) -> Response:
         """
         Return the response for upstream request to the server.
 
         :param method: Method for operation with the API server.
         :param location: Location with path for server request.
         :param params: Optional parameters included in request.
         :param json: Optional JSON payload included in request.
+        :param data: Optional dict payload included in request.
+        :param headers: Optional headers to include in requests.
+        :param httpauth: Optional information for authentication.
         :returns: Response for upstream request to the server.
         """
 
         retry = self.retry
         backoff = self.backoff
         states = self.states
 
@@ -261,16 +326,19 @@
         request = client.request
 
         for count in range(retry):
 
             response = await request(
                 method=method,
                 url=location,
-                params=params,
-                json=json)
+                headers=headers or None,
+                params=params or None,
+                data=data or None,
+                json=json or None,
+                auth=httpauth or None)
 
             status = response.status_code
 
             if status not in states:
                 break
 
             await asyncio.sleep(backoff)
```

### Comparing `enconnect-0.3.0/enconnect/utils/test/test_http.py` & `enconnect-0.4.0/enconnect/utils/test/test_http.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,18 @@
     """
 
 
     attrs = list(httpx.__dict__)
 
     assert attrs == [
         '_HTTPClient__timeout',
+        '_HTTPClient__headers',
         '_HTTPClient__verify',
         '_HTTPClient__capem',
+        '_HTTPClient__httpauth',
         '_HTTPClient__retry',
         '_HTTPClient__backoff',
         '_HTTPClient__states',
         '_HTTPClient__client_block',
         '_HTTPClient__client_async']
 
 
@@ -66,18 +68,22 @@
     assert instr(
         'http.HTTPClient object',
         httpx)
 
 
     assert httpx.timeout == 30
 
+    assert httpx.headers is None
+
     assert httpx.verify is True
 
     assert httpx.capem is None
 
+    assert httpx.httpauth is None
+
     assert httpx.retry == 3
 
     assert httpx.backoff == 3.0
 
     assert httpx.states == {429}
 
     assert httpx.client_block is not None
```

### Comparing `enconnect-0.3.0/enconnect/youtube/params.py` & `enconnect-0.4.0/enconnect/instagram/params.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,27 +9,25 @@
 
 from typing import Optional
 
 from pydantic import BaseModel
 
 
 
-class YouTubeParams(BaseModel, extra='forbid'):
+class InstagramParams(BaseModel, extra='forbid'):
     """
     Process and validate the class configuration parameters.
 
-    :param server: Host or IP address for server connection.
     :param timeout: Timeout when waiting for server response.
     :param token: Token used when authenticating to server.
     :param ssl_verify: Require valid certificate from server.
     :param ssl_capem: Optional path to certificate authority.
     :param data: Keyword arguments passed to Pydantic model.
         Parameter is picked up by autodoc, please ignore.
     """
 
-    server: str = 'www.googleapis.com'
     timeout: int = 30
 
     token: str
 
     ssl_verify: bool = True
     ssl_capem: Optional[str] = None
```

### Comparing `enconnect-0.3.0/enconnect/youtube/youtube.py` & `enconnect-0.4.0/enconnect/reddit/reddit.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,165 +3,167 @@
 
 This file is part of Enasis Network software eco-system. Distribution
 is permitted, for more information consult the project license file.
 """
 
 
 
+import asyncio
 from typing import Any
 from typing import Literal
 from typing import Optional
 from typing import TYPE_CHECKING
-from typing import get_args
+
+from encommon.types import getate
 
 from httpx import Response
 
 from pydantic import BaseModel
 
 from ..utils import HTTPClient
+from ..utils.http import _HTTPAUTH
+from ..utils.http import _PAYLOAD
 
 if TYPE_CHECKING:
-    from .params import YouTubeParams
-
-
-
-RESULT_KINDS = Literal[
-    'channel',
-    'playlist',
-    'video']
+    from .params import RedditParams
 
-_RESULT_KINDS = [
-    f'youtube#{x}' for x in
-    get_args(RESULT_KINDS)]
 
 
+LISTING_VALUE = {
+    'created_utc': 'created',
+    'ups': 'vote_ups',
+    'downs': 'vote_downs',
+    'url_overridden_by_dest': 'url_dest',
+    'media_metadata': 'medias'}
 
-RESULT_VALUE = {
-    'channelId': 'channel',
-    'channelTitle': 'channel_title',
-    'description': 'about',
-    'publishedAt': 'published',
-    'thumbnails': 'thumbnail',
-    'title': 'title'}
 
-RESULT_BASIC = {
-    'channelId': 'channel',
-    'kind': 'kind',
-    'playlistId': 'playlist',
-    'videoId': 'video'}
 
-
-
-class YouTubeResult(BaseModel, extra='ignore'):
+class RedditListing(BaseModel, extra='ignore'):
     """
     Contains information returned from the upstream response.
 
     .. note::
        Fields are not completely documented for this model.
 
     :param data: Keyword arguments passed to Pydantic model.
         Parameter is picked up by autodoc, please ignore.
     """
 
-    kind: RESULT_KINDS
-
-    channel: Optional[str] = None
-    playlist: Optional[str] = None
-    video: Optional[str] = None
-
+    name: str
+    id: str
+    created: int
     title: str
-    about: Optional[str] = None
-    channel_title: Optional[str] = None
+    selftext: Optional[str] = None
+    author: str
+
+    url: str
+    permalink: str
     thumbnail: str
-    published: str
+    url_dest: Optional[str] = None
+    domain: str
+
+    medias: Optional[list[str]] = None
+
+    pinned: bool
+    edited: bool | float
+    stickied: bool
+    archived: bool
+
+    vote_downs: int
+    vote_ups: int
+
+    score: int
 
 
     def __init__(
         self,
         **data: Any,
     ) -> None:
         """
         Initialize instance for class using provided parameters.
         """
 
-
-        basic = data.get('id', {})
-
-        items = RESULT_BASIC.items()
+        items = LISTING_VALUE.items()
 
         for old, new in items:
 
-            value = basic.get(old)
+            value = data.get(old)
 
             if value is None:
                 continue
 
             data[new] = value
 
 
-        match = data.get('snippet', {})
+        data = {
+            k: v for k, v in
+            data.items()
+            if v not in ['', None]}
 
-        items = RESULT_VALUE.items()
 
-        for old, new in items:
+        if data.get('medias'):
 
-            value = match.get(old)
+            images: list[str] = []
 
-            if value is None:
-                continue  # NOCVR
+            items = data['medias'].items()
 
-            data[new] = value
+            for _, media in items:
 
+                assert isinstance(media, dict)
 
-        if 'thumbnail' in data:
-            data['thumbnail'] = (
-                data['thumbnail']
-                ['high']['url'])
+                image = getate(media, 's/u')
 
+                assert isinstance(image, str)
 
-        data['kind'] = data['kind'][8:]
+                images.append(image)
+
+            data['medias'] = images
 
 
         super().__init__(**data)
 
 
 
-class YouTube:
+class Reddit:
     """
     Interact with the cloud service API with various methods.
 
     :param params: Parameters for instantiating the instance.
     """
 
-    __params: 'YouTubeParams'
+    __params: 'RedditParams'
     __client: HTTPClient
 
+    __token: Optional[str]
+
 
     def __init__(
         self,
-        params: 'YouTubeParams',
+        params: 'RedditParams',
     ) -> None:
         """
         Initialize instance for class using provided parameters.
         """
 
         self.__params = params
 
         client = HTTPClient(
             timeout=params.timeout,
             verify=params.ssl_verify,
             capem=params.ssl_capem)
 
         self.__client = client
 
+        self.__token = None
+
 
     @property
     def params(
         self,
-    ) -> 'YouTubeParams':
+    ) -> 'RedditParams':
         """
         Return the Pydantic model containing the configuration.
 
         :returns: Pydantic model containing the configuration.
         """
 
         return self.__params
@@ -176,176 +178,330 @@
 
         :returns: Value for the attribute from class instance.
         """
 
         return self.__client
 
 
+    @property
+    def token(
+        self,
+    ) -> Optional[str]:
+        """
+        Return the value for the attribute from class instance.
+
+        :returns: Value for the attribute from class instance.
+        """
+
+        return self.__token
+
+
+    def request_token_block(
+        self,
+    ) -> str:
+        """
+        Establish new session obtaining token for authorization.
+
+        :returns: Access token used with authenticated requests.
+        """
+
+        if self.__token is not None:
+            return self.__token
+
+        params = self.params
+        username = params.username
+        password = params.password
+        client = params.client
+        secret = params.secret
+
+        request = self.request_block
+
+        payload = {
+            'grant_type': 'password',
+            'username': username,
+            'password': password}
+
+        response = request(
+            method='post',
+            path='api/v1/access_token',
+            data=payload,
+            httpauth=(client, secret))
+
+        response.raise_for_status()
+
+        fetched = response.json()
+
+        assert isinstance(fetched, dict)
+
+        self.__token = (
+            fetched['access_token'])
+
+        return self.__token
+
+
+    async def request_token_async(
+        self,
+    ) -> str:
+        """
+        Establish new session obtaining token for authorization.
+
+        :returns: Access token used with authenticated requests.
+        """
+
+        if self.__token is not None:
+            await asyncio.sleep(0)
+            return self.__token
+
+        params = self.params
+        username = params.username
+        password = params.password
+        client = params.client
+        secret = params.secret
+
+        request = self.request_async
+
+        payload = {
+            'grant_type': 'password',
+            'username': username,
+            'password': password}
+
+        response = await request(
+            method='post',
+            path='api/v1/access_token',
+            data=payload,
+            httpauth=(client, secret))
+
+        response.raise_for_status()
+
+        fetched = response.json()
+
+        assert isinstance(fetched, dict)
+
+        self.__token = (
+            fetched['access_token'])
+
+        return self.__token
+
+
     def request_block(
         self,
-        method: Literal['get'],
+        method: Literal['get', 'post'],
         path: str,
         params: Optional[dict[str, Any]] = None,
+        data: Optional[_PAYLOAD] = None,
+        *,
+        httpauth: Optional[_HTTPAUTH] = None,
     ) -> Response:
         """
         Return the response for upstream request to the server.
 
         :param method: Method for operation with the API server.
         :param path: Path for the location to upstream endpoint.
         :param params: Optional parameters included in request.
+        :param data: Optional dict payload included in request.
+        :param httpauth: Optional information for authentication.
         :returns: Response for upstream request to the server.
         """
 
-        params = dict(params or {})
-
-        server = self.params.server
-        token = self.params.token
+        server = 'www.reddit.com'
         client = self.client
 
-        params['key'] = token
+        request = client.request_block
 
-        location = (
-            f'https://{server}/'
-            f'youtube/v3/{path}')
 
-        request = client.request_block
+        token = self.__token
+        token_key = 'Authorization'
+
+        useragent = self.params.useragent
+
+        headers = {
+            'User-Agent': useragent}
+
+        if token is not None:
+            headers[token_key] = token
+            server = 'oauth.reddit.com'
+
+
+        location = (
+            f'https://{server}/{path}')
 
         return request(
             method=method,
             location=location,
-            params=params)
+            params=params,
+            data=data,
+            headers=headers,
+            httpauth=httpauth)
 
 
     async def request_async(
         self,
-        method: Literal['get'],
+        method: Literal['get', 'post'],
         path: str,
         params: Optional[dict[str, Any]] = None,
+        data: Optional[_PAYLOAD] = None,
+        *,
+        httpauth: Optional[_HTTPAUTH] = None,
     ) -> Response:
         """
         Return the response for upstream request to the server.
 
         :param method: Method for operation with the API server.
         :param path: Path for the location to upstream endpoint.
         :param params: Optional parameters included in request.
+        :param data: Optional dict payload included in request.
+        :param httpauth: Optional information for authentication.
         :returns: Response for upstream request to the server.
         """
 
-        params = dict(params or {})
-
-        server = self.params.server
-        token = self.params.token
+        server = 'www.reddit.com'
         client = self.client
 
-        params['key'] = token
+        request = client.request_async
 
-        location = (
-            f'https://{server}/'
-            f'youtube/v3/{path}')
 
-        request = client.request_async
+        token = self.__token
+        token_key = 'Authorization'
+
+        useragent = self.params.useragent
+
+        headers = {
+            'User-Agent': useragent}
+
+        if token is not None:
+            headers[token_key] = token
+            server = 'oauth.reddit.com'
+
+
+        location = (
+            f'https://{server}/{path}')
 
         return await request(
             method=method,
             location=location,
-            params=params)
+            params=params,
+            data=data,
+            headers=headers,
+            httpauth=httpauth)
 
 
-    def search(
+    def latest(
         # NOCVR
         self,
+        subred: str,
         params: Optional[dict[str, Any]] = None,
-    ) -> list[YouTubeResult]:
+    ) -> list[RedditListing]:
         """
-        Return the results from the provided search parameters.
+        Return the new items within the provided subreddit path.
 
+        :param subred: Path to subreddit containing the content.
         :param params: Optional parameters included in request.
-        :returns: Results from the provided search parameters.
+        :returns: New items within the provided subreddit path.
         """
 
-        return self.search_block(params)
+        return self.latest_block(subred, params)
 
 
-    def search_block(
+    def latest_block(
         self,
+        subred: str,
         params: Optional[dict[str, Any]] = None,
-    ) -> list[YouTubeResult]:
+    ) -> list[RedditListing]:
         """
-        Return the results from the provided search parameters.
+        Return the new items within the provided subreddit path.
 
+        :param subred: Path to subreddit containing the content.
         :param params: Optional parameters included in request.
-        :returns: Results from the provided search parameters.
+        :returns: New items within the provided subreddit path.
         """
 
         params = dict(params or {})
 
+        request = self.request_block
 
-        if 'maxResults' not in params:
-            params['maxResults'] = 50
+        if self.__token is None:
+            self.request_token_block()
 
-        if 'order' not in params:
-            params['order'] = 'date'
 
-        if 'part' not in params:
-            params['part'] = 'snippet,id'
+        def _request() -> Response:
 
+            return request(
+                method='get',
+                path=f'r/{subred}/new.json')
 
-        request = self.request_block
 
-        response = request(
-            'get', 'search', params)
+        response = _request()
+
+        if response.status_code == 401:
+
+            self.__token = None
+
+            self.request_token_block()
+
+            response = _request()
 
         response.raise_for_status()
 
         fetched = response.json()
 
         assert isinstance(fetched, dict)
 
 
+        source = fetched['data']
+        children = source['children']
+
         return [
-            YouTubeResult(**x)
-            for x in fetched['items']
-            if x['id']['kind']
-            in _RESULT_KINDS]
+            RedditListing(**x['data'])
+            for x in children]
 
 
-    async def search_async(
+    async def latest_async(
         self,
+        subred: str,
         params: Optional[dict[str, Any]] = None,
-    ) -> list[YouTubeResult]:
+    ) -> list[RedditListing]:
         """
-        Return the results from the provided search parameters.
+        Return the new items within the provided subreddit path.
 
+        :param subred: Path to subreddit containing the content.
         :param params: Optional parameters included in request.
-        :returns: Results from the provided search parameters.
+        :returns: New items within the provided subreddit path.
         """
 
         params = dict(params or {})
 
+        request = self.request_async
 
-        if 'maxResults' not in params:
-            params['maxResults'] = 50
+        if self.__token is None:
+            await self.request_token_async()
 
-        if 'order' not in params:
-            params['order'] = 'date'
 
-        if 'part' not in params:
-            params['part'] = 'snippet,id'
+        async def _request() -> Response:
 
+            return await request(
+                method='get',
+                path=f'r/{subred}/new.json')
 
-        request = self.request_async
 
-        response = await request(
-            'get', 'search', params)
+        response = await _request()
+
+        if response.status_code == 401:
+
+            self.__token = None
+
+            await self.request_token_async()
+
+            response = await _request()
 
         response.raise_for_status()
 
         fetched = response.json()
 
         assert isinstance(fetched, dict)
 
 
+        source = fetched['data']
+        children = source['children']
+
         return [
-            YouTubeResult(**x)
-            for x in fetched['items']
-            if x['id']['kind']
-            in _RESULT_KINDS]
+            RedditListing(**x['data'])
+            for x in children]
```

### Comparing `enconnect-0.3.0/enconnect.egg-info/PKG-INFO` & `enconnect-0.4.0/enconnect.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enconnect
-Version: 0.3.0
+Version: 0.4.0
 Summary: Enasis Network Remote Connect
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -66,14 +66,18 @@
 And finally run the various tests to validate the code and produce coverage
 information found in the `htmlcov` folder in the root of the project.
 ```
 make -s pytest
 ```
 
 ## Build and upload to PyPi
+Rebuild the environment.
+```
+make -s check-revenv
+```
 Build the package.
 ```
 make -s pypackage
 ```
 Upload to the test PyPi.
 ```
 make -s pypi-upload-test
```

### Comparing `enconnect-0.3.0/enconnect.egg-info/SOURCES.txt` & `enconnect-0.4.0/enconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enconnect-0.3.0/pyproject.toml` & `enconnect-0.4.0/pyproject.toml`

 * *Files identical despite different names*

