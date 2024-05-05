# Comparing `tmp/torch_snippets-0.528.tar.gz` & `tmp/torch_snippets-0.530.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_snippets-0.528.tar", last modified: Tue Mar 19 09:25:37 2024, max compression
+gzip compressed data, was "torch_snippets-0.530.tar", last modified: Sun May  5 12:48:50 2024, max compression
```

## Comparing `torch_snippets-0.528.tar` & `torch_snippets-0.530.tar`

### file list

```diff
@@ -1,53 +1,55 @@
-drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2024-03-19 09:25:37.577382 torch_snippets-0.528/
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    11357 2021-12-31 15:06:08.000000 torch_snippets-0.528/LICENSE
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1062 2023-01-17 16:58:23.000000 torch_snippets-0.528/LICENSE.txt
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      111 2021-12-31 15:06:08.000000 torch_snippets-0.528/MANIFEST.in
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5691 2024-03-19 09:25:37.577677 torch_snippets-0.528/PKG-INFO
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4999 2023-01-17 16:58:23.000000 torch_snippets-0.528/README.md
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      871 2024-03-19 09:25:02.000000 torch_snippets-0.528/settings.ini
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       79 2024-03-19 09:25:37.582060 torch_snippets-0.528/setup.cfg
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2001 2024-01-08 09:24:32.000000 torch_snippets-0.528/setup.py
-drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2024-03-19 09:25:37.561668 torch_snippets-0.528/torch_snippets/
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      401 2024-03-19 09:25:33.000000 torch_snippets-0.528/torch_snippets/__init__.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    56479 2024-03-19 09:25:34.000000 torch_snippets-0.528/torch_snippets/_modidx.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4482 2023-01-17 16:58:25.000000 torch_snippets-0.528/torch_snippets/_nbdev.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6211 2024-03-19 09:25:33.000000 torch_snippets-0.528/torch_snippets/adapters.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    12173 2024-03-19 09:25:33.000000 torch_snippets-0.528/torch_snippets/bb_utils.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1436 2024-03-19 09:25:33.000000 torch_snippets-0.528/torch_snippets/bokeh_loader.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1672 2024-03-19 09:25:33.000000 torch_snippets-0.528/torch_snippets/charts.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1866 2023-12-28 06:40:32.000000 torch_snippets-0.528/torch_snippets/dates.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1206 2024-03-19 09:25:33.000000 torch_snippets-0.528/torch_snippets/decorators.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       73 2022-05-07 11:30:59.000000 torch_snippets-0.528/torch_snippets/fastcores.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    11427 2023-11-28 11:52:35.000000 torch_snippets-0.528/torch_snippets/icecream.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4126 2024-03-19 09:25:33.000000 torch_snippets-0.528/torch_snippets/imgaug_loader.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     3429 2024-03-19 09:25:33.000000 torch_snippets-0.528/torch_snippets/inspector.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     8386 2024-03-19 09:25:33.000000 torch_snippets-0.528/torch_snippets/interactive_show.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5727 2024-03-19 09:25:33.000000 torch_snippets-0.528/torch_snippets/ipython.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      597 2024-03-19 09:25:33.000000 torch_snippets-0.528/torch_snippets/load_defaults.py
--rwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    23308 2024-03-02 16:16:09.000000 torch_snippets-0.528/torch_snippets/loader.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     8498 2024-03-19 09:25:33.000000 torch_snippets-0.528/torch_snippets/logger.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    14432 2024-03-19 09:25:33.000000 torch_snippets-0.528/torch_snippets/markup.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    17078 2024-03-19 09:25:18.000000 torch_snippets-0.528/torch_snippets/markup2.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2054 2024-03-19 09:25:33.000000 torch_snippets-0.528/torch_snippets/misc.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    11021 2024-03-19 09:25:33.000000 torch_snippets-0.528/torch_snippets/paths.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1465 2024-03-19 09:25:33.000000 torch_snippets-0.528/torch_snippets/pdf_loader.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      822 2024-03-19 09:25:33.000000 torch_snippets-0.528/torch_snippets/registry.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6144 2024-03-19 09:25:33.000000 torch_snippets-0.528/torch_snippets/sklegos.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    14237 2024-01-09 02:35:49.000000 torch_snippets-0.528/torch_snippets/text_utils.py
-drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2024-03-19 09:25:37.570927 torch_snippets-0.528/torch_snippets/thinc_parser/
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2024-03-19 09:25:33.000000 torch_snippets-0.528/torch_snippets/thinc_parser/__init__.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1082 2022-10-16 17:20:20.000000 torch_snippets-0.528/torch_snippets/thinc_parser/parser.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    31250 2024-02-29 09:58:55.000000 torch_snippets-0.528/torch_snippets/torch_loader.py
-drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2024-03-19 09:25:37.576422 torch_snippets-0.528/torch_snippets/trainer/
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       23 2024-03-19 09:25:33.000000 torch_snippets-0.528/torch_snippets/trainer/__init__.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6882 2024-03-19 09:25:33.000000 torch_snippets-0.528/torch_snippets/trainer/capsule.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1614 2024-03-19 09:25:33.000000 torch_snippets-0.528/torch_snippets/trainer/config.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5801 2024-02-15 11:49:25.000000 torch_snippets-0.528/torch_snippets/trainer/hooks.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2137 2024-02-14 10:01:57.000000 torch_snippets-0.528/torch_snippets/video.py
-drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2024-03-19 09:25:37.569315 torch_snippets-0.528/torch_snippets.egg-info/
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5691 2024-03-19 09:25:37.000000 torch_snippets-0.528/torch_snippets.egg-info/PKG-INFO
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1274 2024-03-19 09:25:37.000000 torch_snippets-0.528/torch_snippets.egg-info/SOURCES.txt
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        1 2024-03-19 09:25:37.000000 torch_snippets-0.528/torch_snippets.egg-info/dependency_links.txt
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-01-17 16:58:23.000000 torch_snippets-0.528/torch_snippets.egg-info/not-zip-safe
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      281 2024-03-19 09:25:37.000000 torch_snippets-0.528/torch_snippets.egg-info/requires.txt
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       15 2024-03-19 09:25:37.000000 torch_snippets-0.528/torch_snippets.egg-info/top_level.txt
+drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2024-05-05 12:48:50.756183 torch_snippets-0.530/
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    11357 2021-12-31 15:06:08.000000 torch_snippets-0.530/LICENSE
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1062 2023-01-17 16:58:23.000000 torch_snippets-0.530/LICENSE.txt
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      111 2021-12-31 15:06:08.000000 torch_snippets-0.530/MANIFEST.in
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5711 2024-05-05 12:48:50.756642 torch_snippets-0.530/PKG-INFO
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4999 2023-01-17 16:58:23.000000 torch_snippets-0.530/README.md
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      871 2024-04-25 12:13:34.000000 torch_snippets-0.530/settings.ini
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       79 2024-05-05 12:48:50.758336 torch_snippets-0.530/setup.cfg
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2001 2024-01-08 09:24:32.000000 torch_snippets-0.530/setup.py
+drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2024-05-05 12:48:50.740661 torch_snippets-0.530/torch_snippets/
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      401 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/__init__.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    57057 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/_modidx.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4482 2023-01-17 16:58:25.000000 torch_snippets-0.530/torch_snippets/_nbdev.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     8846 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/adapters.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    17079 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/bb_utils.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2026 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/bokeh_loader.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    19042 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/charts.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1866 2023-12-28 06:40:32.000000 torch_snippets-0.530/torch_snippets/dates.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2056 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/decorators.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       73 2022-05-07 11:30:59.000000 torch_snippets-0.530/torch_snippets/fastcores.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    11427 2023-11-28 11:52:35.000000 torch_snippets-0.530/torch_snippets/icecream.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     8479 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/imgaug_loader.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     3429 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/inspector.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     8386 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/interactive_show.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5727 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/ipython.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      597 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/load_defaults.py
+-rwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    23434 2024-05-05 12:47:54.000000 torch_snippets-0.530/torch_snippets/loader.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     8480 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/logger.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    14432 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/markup.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    17441 2024-05-05 12:47:53.000000 torch_snippets-0.530/torch_snippets/markup2.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2054 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/misc.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    11039 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/paths.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1465 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/pdf_loader.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      822 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/registry.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     3234 2024-05-05 12:47:53.000000 torch_snippets-0.530/torch_snippets/scp.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6144 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/sklegos.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    14202 2024-03-28 08:34:42.000000 torch_snippets-0.530/torch_snippets/text_utils.py
+drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2024-05-05 12:48:50.750918 torch_snippets-0.530/torch_snippets/thinc_parser/
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/thinc_parser/__init__.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1082 2022-10-16 17:20:20.000000 torch_snippets-0.530/torch_snippets/thinc_parser/parser.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    31250 2024-02-29 09:58:55.000000 torch_snippets-0.530/torch_snippets/torch_loader.py
+drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2024-05-05 12:48:50.754964 torch_snippets-0.530/torch_snippets/trainer/
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       23 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/trainer/__init__.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6882 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/trainer/capsule.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2432 2024-05-05 12:48:47.000000 torch_snippets-0.530/torch_snippets/trainer/config.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5801 2024-04-24 06:16:19.000000 torch_snippets-0.530/torch_snippets/trainer/hooks.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2137 2024-02-14 10:01:57.000000 torch_snippets-0.530/torch_snippets/video.py
+drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2024-05-05 12:48:50.749344 torch_snippets-0.530/torch_snippets.egg-info/
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5711 2024-05-05 12:48:50.000000 torch_snippets-0.530/torch_snippets.egg-info/PKG-INFO
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1337 2024-05-05 12:48:50.000000 torch_snippets-0.530/torch_snippets.egg-info/SOURCES.txt
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        1 2024-05-05 12:48:50.000000 torch_snippets-0.530/torch_snippets.egg-info/dependency_links.txt
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       20 2024-05-05 12:48:50.000000 torch_snippets-0.530/torch_snippets.egg-info/entry_points.txt
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-01-17 16:58:23.000000 torch_snippets-0.530/torch_snippets.egg-info/not-zip-safe
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      281 2024-05-05 12:48:50.000000 torch_snippets-0.530/torch_snippets.egg-info/requires.txt
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       15 2024-05-05 12:48:50.000000 torch_snippets-0.530/torch_snippets.egg-info/top_level.txt
```

### Comparing `torch_snippets-0.528/LICENSE` & `torch_snippets-0.530/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.528/LICENSE.txt` & `torch_snippets-0.530/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.528/PKG-INFO` & `torch_snippets-0.530/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: torch_snippets
-Version: 0.528
+Version: 0.530
 Summary: One line functions for common tasks
 Home-page: https://github.com/sizhky/torch_snippets/tree/master/
 Author: Yeshwanth Reddy
 Author-email: 1992chinna@gmail.com
 License: Apache Software License 2.0
 Keywords: snippets,torch
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7
@@ -327,7 +328,9 @@
      'with_cast',
      'wrap_class',
      'write',
      'writelines',
      'xywh2xyXY',
      'zip_cycle',
      'zip_files']
+
+
```

### Comparing `torch_snippets-0.528/README.md` & `torch_snippets-0.530/README.md`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.528/settings.ini` & `torch_snippets-0.530/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 user = sizhky
 description = One line functions for common tasks
 keywords = snippets, torch
 author = Yeshwanth Reddy
 author_email = 1992chinna@gmail.com
 copyright = sizhky
 branch = master
-version = 0.528
+version = 0.530
 min_python = 3.7
 audience = Developers
 language = English
 custom_sidebar = False
 license = apache2
 status = 2
 requirements = fastcore matplotlib Pillow altair dill ipython loguru numpy pandas tqdm rich PyYAML catalogue confection pydantic typing srsly typing_extensions wasabi jsonlines imgaug>=0.4.0 xmltodict fuzzywuzzy scikit-learn nltk python-Levenshtein pre-commit pymupdf nbconvert nbformat icecream
```

### Comparing `torch_snippets-0.528/setup.py` & `torch_snippets-0.530/setup.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.528/torch_snippets/_modidx.py` & `torch_snippets-0.530/torch_snippets/_modidx.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,16 +82,20 @@
                                                                                   'torch_snippets/bb_utils.py'),
                                          'torch_snippets.bb_utils.to_relative': ( 'bounding_boxes.html#to_relative',
                                                                                   'torch_snippets/bb_utils.py')},
             'torch_snippets.bokeh_loader': { 'torch_snippets.bokeh_loader.get_bplot': ( 'bokeh_plotting.html#get_bplot',
                                                                                         'torch_snippets/bokeh_loader.py'),
                                              'torch_snippets.bokeh_loader.parse_sz': ( 'bokeh_plotting.html#parse_sz',
                                                                                        'torch_snippets/bokeh_loader.py')},
-            'torch_snippets.charts': { 'torch_snippets.charts.confusion_matrix': ( 'charts.html#confusion_matrix',
-                                                                                   'torch_snippets/charts.py')},
+            'torch_snippets.charts': { 'torch_snippets.charts.UpSetAltair': ('charts.html#upsetaltair', 'torch_snippets/charts.py'),
+                                       'torch_snippets.charts.confusion_matrix': ( 'charts.html#confusion_matrix',
+                                                                                   'torch_snippets/charts.py'),
+                                       'torch_snippets.charts.spider': ('charts.html#spider', 'torch_snippets/charts.py'),
+                                       'torch_snippets.charts.upsetaltair_top_level_configuration': ( 'charts.html#upsetaltair_top_level_configuration',
+                                                                                                      'torch_snippets/charts.py')},
             'torch_snippets.dates': {},
             'torch_snippets.decorators': { 'torch_snippets.decorators.check_kwargs_not_none': ( 'decorators.html#check_kwargs_not_none',
                                                                                                 'torch_snippets/decorators.py'),
                                            'torch_snippets.decorators.io': ('decorators.html#io', 'torch_snippets/decorators.py'),
                                            'torch_snippets.decorators.timeit': ('decorators.html#timeit', 'torch_snippets/decorators.py')},
             'torch_snippets.fastcores': {},
             'torch_snippets.icecream': {},
@@ -332,14 +336,15 @@
                                            'torch_snippets.pdf_loader.PDF.show': ('pdf.html#pdf.show', 'torch_snippets/pdf_loader.py')},
             'torch_snippets.registry': { 'torch_snippets.registry.parse': ('registry.html#parse', 'torch_snippets/registry.py'),
                                          'torch_snippets.registry.parse_and_resolve': ( 'registry.html#parse_and_resolve',
                                                                                         'torch_snippets/registry.py'),
                                          'torch_snippets.registry.parse_string': ( 'registry.html#parse_string',
                                                                                    'torch_snippets/registry.py'),
                                          'torch_snippets.registry.tryeval': ('registry.html#tryeval', 'torch_snippets/registry.py')},
+            'torch_snippets.scp': {},
             'torch_snippets.sklegos': { 'torch_snippets.sklegos.Cat2Num': ('sklegos.html#cat2num', 'torch_snippets/sklegos.py'),
                                         'torch_snippets.sklegos.Cat2Num.__init__': ( 'sklegos.html#cat2num.__init__',
                                                                                      'torch_snippets/sklegos.py'),
                                         'torch_snippets.sklegos.Cat2Num.fit': ('sklegos.html#cat2num.fit', 'torch_snippets/sklegos.py'),
                                         'torch_snippets.sklegos.Cat2Num.fit_transform': ( 'sklegos.html#cat2num.fit_transform',
                                                                                           'torch_snippets/sklegos.py'),
                                         'torch_snippets.sklegos.Cat2Num.transform': ( 'sklegos.html#cat2num.transform',
```

### Comparing `torch_snippets-0.528/torch_snippets/_nbdev.py` & `torch_snippets-0.530/torch_snippets/_nbdev.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.528/torch_snippets/adapters.py` & `torch_snippets-0.530/torch_snippets/adapters.py`

 * *Files 27% similar despite different names*

```diff
@@ -15,14 +15,22 @@
     """Convert a numpy image to base64 string"""
     img_str = cv2.imencode(".jpg", image)[1].tobytes()
     img_b64 = base64.b64encode(img_str).decode("utf-8")
     return img_b64
 
 
 def b64_2_np(input: str) -> np.ndarray:
+    """Converts a base64 encoded image to a NumPy array.
+
+    Args:
+        input (str): The base64 encoded image.
+
+    Returns:
+        np.ndarray: The NumPy array representation of the image in RGB format.
+    """
     input = bytes(input, "utf-8")
     input = base64.b64decode(input)
     img_nparr = np.frombuffer(input, np.uint8)
     img_cv2 = cv2.imdecode(img_nparr, cv2.IMREAD_COLOR)
     img_rgb = cv2.cvtColor(img_cv2, cv2.COLOR_BGR2RGB)
     return img_rgb
 
@@ -56,14 +64,25 @@
         output = f.read()
     return output
 
 # %% ../nbs/adapters.ipynb 4
 def _process(
     df: pd.DataFrame, label_column="readable_label", default_label="Background"
 ):
+    """
+    Process the given DataFrame and convert it into a list of records.
+
+    Args:
+        df (pd.DataFrame): The input DataFrame to be processed.
+        label_column (str, optional): The column name for the label. Defaults to "readable_label".
+        default_label (str, optional): The default label value. Defaults to "Background".
+
+    Returns:
+        list: A list of records, where each record is a dictionary representing a row in the DataFrame.
+    """
     df["@xbr"] = df["X"]
     df["@xtl"] = df["x"]
     df["@ybr"] = df["Y"]
     df["@ytl"] = df["y"]
     df["@label"] = df[label_column] if label_column in df.columns else default_label
     df["@occluded"] = "0"
     df["@source"] = "manual"
@@ -105,14 +124,30 @@
     xml_output_file,
     items=None,
     parquet=False,
     relative_df=True,
     default_label="Background",
     extension="jpg",
 ):
+    """
+    Convert CSV annotations to CVAT XML format.
+
+    Args:
+        images_folder (str): Path to the folder containing the images.
+        csvs_folder (str): Path to the folder containing the CSV annotations.
+        xml_output_file (str): Path to the output XML file.
+        items (list, optional): List of items to process. If None, all items will be processed. Defaults to None.
+        parquet (bool, optional): Whether the annotations are stored in Parquet format. Defaults to False.
+        relative_df (bool, optional): Whether the bounding box coordinates in the CSV are relative to the image size. Defaults to True.
+        default_label (str, optional): Default label for the bounding boxes. Defaults to "Background".
+        extension (str, optional): Image file extension. Defaults to "jpg".
+
+    Returns:
+        None
+    """
     images_folder, csvs_folder = [P(_) for _ in [images_folder, csvs_folder]]
     data = AttrDict({"annotations": {"image": []}})
     if items is None:
         items = common(stems(images_folder), stems(csvs_folder))
 
     items = sorted(items)
 
@@ -131,27 +166,47 @@
         _ia["@name"] = f"{item}.jpg"
         _ia["box"] = _process(df, default_label=default_label)
         data.annotations.image.append(_ia)
     write_xml(data, xml_output_file)
 
 
 def _get_attribute_columns(column):
+    """
+    Get attribute columns from a given column.
+
+    Args:
+        column (pandas.Series): The input column.
+
+    Returns:
+        set: A set of attribute columns extracted from the input column.
+    """
+
     def _get_columns_from_row(item):
         if item != item:
             return []
         if isinstance(item, dict):
             return [item["@name"]]
         else:
             return [_item["@name"] for _item in item]
 
     output = set(flatten(column.map(_get_columns_from_row)))
     return output
 
 
 def _get_attribute_data(item, column_name):
+    """
+    Retrieves the attribute data for a given item and column name.
+
+    Parameters:
+    - item: The item to retrieve the attribute data from.
+    - column_name: The name of the column to retrieve the attribute data for.
+
+    Returns:
+    - The attribute data for the given item and column name, or np.nan if not found.
+    """
     if item != item:
         return item
     if isinstance(item, dict):
         if item["@name"] == column_name:
             return item.get("#text", np.nan)
         else:
             return np.nan
@@ -160,14 +215,23 @@
         if item:
             return item[0].get("#text", np.nan)
         else:
             return np.nan
 
 
 def _cvat_ann_2_csv(ann):
+    """
+    Convert CVAT annotation to a pandas DataFrame in CSV format.
+
+    Args:
+        ann (dict): CVAT annotation dictionary.
+
+    Returns:
+        pandas.DataFrame: DataFrame containing the converted annotation data in CSV format.
+    """
     if "box" not in ann:
         return pd.DataFrame()
     if isinstance(ann.box, AttrDict):
         rows = [a.to_dict() for a in [ann.box]]
     else:
         rows = [a.to_dict() for a in ann.box]
     df = pd.DataFrame(rows)
@@ -193,16 +257,29 @@
         for column in new_columns:
             df[column] = df["attribute"].map(lambda x: _get_attribute_data(x, column))
         df.drop(["attribute"], axis=1, inplace=True)
     return df
 
 
 def cvat_2_csvs(xmlfile, csvs_folder):
+    """
+    Convert CVAT XML annotations to CSV files.
+
+    Args:
+        xmlfile (str): Path to the CVAT XML file.
+        csvs_folder (str): Path to the folder where the CSV files will be saved.
+
+    Returns:
+        None
+    """
     data = read_xml(xmlfile)
-    for item in data.annotations.image:
+    items = data.annotations.image
+    if not isinstance(items, list):
+        items = [items]
+    for item in items:
         try:
             df = _cvat_ann_2_csv(item)
             save_at = f'{csvs_folder}/{stem(item["@name"])}.csv'
             makedir(parent(save_at))
             df.to_csv(save_at, index=False)
         except Exception as e:
             Warn(f'{e} @ {item["@name"]}')
```

### Comparing `torch_snippets-0.528/torch_snippets/bb_utils.py` & `torch_snippets-0.530/torch_snippets/bb_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -147,72 +147,147 @@
                 ]
                 return pd.DataFrame(output, columns="ix,bb,dist".split(","))
             raise NotImplementedError("")
         return sorted(other_bbs, key=lambda obj: self.l2(obj[1]))
 
 # %% ../nbs/bounding_boxes.ipynb 8
 def df2bbs(df):
+    """
+    Convert a DataFrame to bounding boxes.
+
+    Parameters:
+    df (pd.DataFrame): The DataFrame to convert.
+
+    Returns:
+    list: A list of bounding boxes.
+    """
     if "bb" in df.columns:
         try:
             return bbfy(df["bb"].values.tolist())
         except:
             return bbfy(df["bb"].map(lambda x: eval(x)).values.tolist())
     return [BB(bb) for bb in df[list("xyXY")].values.tolist()]
 
 
 def bbs2df(bbs):
+    """
+    Convert bounding boxes to a DataFrame.
+
+    Parameters:
+    bbs (list): The bounding boxes to convert.
+
+    Returns:
+    pd.DataFrame: A DataFrame representing the bounding boxes.
+    """
     bbs = [list(bb) for bb in bbs]
     return pd.DataFrame(bbs, columns=["x", "y", "X", "Y"])
 
 
 def bbfy(bbs):
+    """
+    Convert bounding boxes to BB objects.
+
+    Parameters:
+    bbs (list): The bounding boxes to convert.
+
+    Returns:
+    list: A list of BB objects.
+    """
     return [BB(bb) for bb in bbs]
 
 
 def jitter(bbs, noise):
+    """
+    Add noise to bounding boxes. Useful when you have a lot of overlapping boxes.
+
+    Parameters:
+    bbs (list): The bounding boxes to add noise to.
+    noise (float): The amount of noise to add.
+
+    Returns:
+    list: A list of bounding boxes with added noise.
+    """
     return [BB(bb).jitter(noise) for bb in bbs]
 
 
 def compute_eps(eps):
+    """
+    Compute epsilon values for bounding box manipulation.
+
+    Parameters:
+    eps (float or tuple): The epsilon value(s) to compute.
+
+    Returns:
+    tuple: A tuple of epsilon values.
+    """
     if isinstance(eps, tuple):
         if len(eps) == 4:
             epsx, epsy, epsX, epsY = eps
         else:
             epsx, epsy = eps
             epsx, epsy, epsX, epsY = epsx / 2, epsy / 2, epsx / 2, epsy / 2
     else:
         epsx, epsy, epsX, epsY = eps / 2, eps / 2, eps / 2, eps / 2
     return epsx, epsy, epsX, epsY
 
 
 def enlarge_bbs(bbs, eps=0.2):
-    "enlarge all `bbs` by `eps` fraction (i.e., eps*100 percent)"
+    """
+    Enlarge bounding boxes by a certain fraction.
+
+    Parameters:
+    bbs (list): The bounding boxes to enlarge.
+    eps (float, optional): The fraction to enlarge by. Defaults to 0.2.
+
+    Returns:
+    list: A list of enlarged bounding boxes.
+    """
     bbs = bbfy(bbs)
     epsx, epsy, epsX, epsY = compute_eps(eps)
     bbs = bbfy(bbs)
     shs = [(bb.h, bb.w) for bb in bbs]
     return [
         BB(x - (w * epsx), y - (h * epsy), X + (w * epsX), Y + (h * epsY))
         for (x, y, X, Y), (h, w) in zip(bbs, shs)
     ]
 
 
 def shrink_bbs(bbs, eps=0.2):
-    "shrink all `bbs` by `eps` fraction (i.e., eps*100 percent)"
+    """
+    Shrink bounding boxes by a certain fraction.
+
+    Parameters:
+    bbs (list): The bounding boxes to shrink.
+    eps (float, optional): The fraction to shrink by. Defaults to 0.2.
+
+    Returns:
+    list: A list of shrunk bounding boxes.
+    """
     bbs = bbfy(bbs)
     epsx, epsy, epsX, epsY = compute_eps(eps)
     bbs = bbfy(bbs)
     shs = [(bb.h, bb.w) for bb in bbs]
     return [
         BB(x + (w * epsx), y + (h * epsy), X - (w * epsX), Y - (h * epsY))
         for (x, y, X, Y), (h, w) in zip(bbs, shs)
     ]
 
 # %% ../nbs/bounding_boxes.ipynb 9
 def iou(bboxes1, bboxes2):
+    """
+    Calculates the Intersection over Union (IoU) between two sets of bounding boxes.
+
+    Args:
+        bboxes1 (list or numpy array): The first set of bounding boxes in the format [x, y, X, Y].
+        bboxes2 (list or numpy array): The second set of bounding boxes in the format [x, y, X, Y].
+
+    Returns:
+        numpy array: The IoU between each pair of bounding boxes.
+
+    """
     bboxes1 = np.array(bboxes1)
     bboxes2 = np.array(bboxes2)
     x11, y11, x12, y12 = np.split(bboxes1, 4, axis=1)
     x21, y21, x22, y22 = np.split(bboxes2, 4, axis=1)
     xA = np.maximum(x11, np.transpose(x21))
     yA = np.maximum(y11, np.transpose(y21))
     xB = np.minimum(x12, np.transpose(x22))
@@ -221,14 +296,25 @@
     boxAArea = (x12 - x11) * (y12 - y11)
     boxBArea = (x22 - x21) * (y22 - y21)
     iou = interArea / (boxAArea + np.transpose(boxBArea) - interArea)
     return iou
 
 
 def compute_distance_matrix(bboxes1, bboxes2):
+    """
+    Compute the distance matrix between two sets of bounding boxes.
+
+    Parameters:
+    - bboxes1 (list): List of bounding boxes in the format [x, y, X, Y].
+    - bboxes2 (list): List of bounding boxes in the format [x, y, X, Y].
+
+    Returns:
+    - distance_matrix (ndarray): 2D array containing the Euclidean distances between all pairs of bounding boxes.
+    """
+
     # Convert the bounding box lists to NumPy arrays
     bboxes1 = np.array(bboxes1)
     bboxes2 = np.array(bboxes2)
 
     # Extract the x, y coordinates of the bounding boxes
     xy1 = bboxes1[:, :2]
     xy2 = bboxes2[:, :2]
@@ -239,25 +325,46 @@
     # Take the square root to get the Euclidean distances
     distance_matrix = np.sqrt(distance_matrix)
 
     return distance_matrix
 
 
 def compute_distances(df1, df2, shrink_factors=(1, 1)):
-    """Return euclidean distance mxn matrix for all boxes from df1 with all boxes from df2"""
+    """
+    Compute the Euclidean distance matrix between bounding boxes in df1 and df2.
+
+    Parameters:
+    - df1 (DataFrame): The first DataFrame containing bounding boxes.
+    - df2 (DataFrame): The second DataFrame containing bounding boxes.
+    - shrink_factors (tuple, optional): The shrink factors to apply to the bounding boxes. Default is (1, 1).
+
+    Returns:
+    - distances (ndarray): The Euclidean distance matrix between the bounding boxes in df1 and df2.
+    """
     sx, sy = shrink_factors
     bbs1 = np.array(df2bbs(df1)) / np.array([sx, sy, sx, sy])
     bbs2 = np.array(df2bbs(df2)) / np.array([sx, sy, sx, sy])
 
     distances = compute_distance_matrix(bbs1, bbs2)
     return distances
 
 # %% ../nbs/bounding_boxes.ipynb 10
 def split_bb_to_xyXY(df):
-    "convert bb column to separate x,y,X,Y columns"
+    """
+    Convert the 'bb' column in the DataFrame to separate 'x', 'y', 'X', 'Y' columns.
+
+    Args:
+        df (pd.DataFrame): The DataFrame containing the bounding box information.
+
+    Returns:
+        pd.DataFrame: The DataFrame with separate 'x', 'y', 'X', 'Y' columns.
+
+    Raises:
+        AssertionError: If the input is not a DataFrame or if the 'bb' column is missing.
+    """
     df = df.copy()
     assert isinstance(df, pd.DataFrame)
     if all([item in df.columns for item in "xyXY"]):
         return df
     assert "bb" in df.columns, "Expecting the df's bounding boxes to be in `bb` column"
     try:
         df["bb"] = df["bb"].map(eval)
@@ -268,35 +375,77 @@
     df["X"] = df["bb"].map(lambda x: x[2])
     df["Y"] = df["bb"].map(lambda x: x[3])
     df.drop(["bb"], axis=1, inplace=True)
     return df
 
 
 def combine_xyXY_to_bb(df):
-    "combine `x,y,X,Y` to `bb` column"
+    """
+    Combine `x`, `y`, `X`, `Y` columns into a single `bb` column.
+
+    Args:
+        df (pandas.DataFrame): The input DataFrame containing `x`, `y`, `X`, `Y` columns.
+
+    Returns:
+        pandas.DataFrame: The modified DataFrame with the `bb` column.
+
+    Raises:
+        AssertionError: If any of the columns `x`, `y`, `X`, `Y` are missing in the DataFrame.
+    """
     df = df.copy()
     assert all(
         [item in df.columns for item in "xyXY"]
     ), "All the columns `x`, `y`, `X`, `Y` should be in df"
     df["bb"] = df[[*"xyXY"]].values.tolist()
     df.drop([*"xyXY"], inplace=True, axis=1)
     return df
 
 
 def is_absolute(df):
+    """
+    Check if the bounding boxes in the given DataFrame are absolute.
+
+    Args:
+        df (pandas.DataFrame): The DataFrame containing bounding box coordinates.
+
+    Returns:
+        bool: True if the maximum value of the bounding box coordinates is greater than 1.1, False otherwise.
+    """
     bbs = df2bbs(df)
     bbs = np.array(bbs)
     return bbs.max() > 1.1
 
 
 def is_relative(df):
+    """
+    Check if the bounding box coordinates in the DataFrame are relative.
+
+    Args:
+        df (pandas.DataFrame): The DataFrame containing bounding box coordinates.
+
+    Returns:
+        bool: True if the bounding box coordinates are relative, False otherwise.
+    """
     return not is_absolute(df)
 
 
 def to_relative(df, height, width, force=False):
+    """
+    Converts bounding box coordinates in a DataFrame to relative coordinates.
+
+    Args:
+        df (pandas.DataFrame): The DataFrame containing bounding box coordinates.
+        height (int): The height of the image.
+        width (int): The width of the image.
+        force (bool, optional): If True, forces conversion even if the coordinates are already relative.
+                                Defaults to False.
+
+    Returns:
+        pandas.DataFrame: The DataFrame with bounding box coordinates converted to relative coordinates.
+    """
     if not force and is_relative(df):
         return df
     df = df.copy()
     if "x" not in df.columns and "bb" in df.columns:
         _recombine = True
         df = split_bb_to_xyXY(df)
     else:
@@ -307,14 +456,26 @@
     df["Y"] = df["Y"] / height
     if _recombine:
         df = combine_xyXY_to_bb(df)
     return df
 
 
 def to_absolute(df, height, width, force=False):
+    """
+    Converts bounding box coordinates from relative to absolute values.
+
+    Args:
+        df (pandas.DataFrame): The DataFrame containing the bounding box coordinates.
+        height (int): The height of the image.
+        width (int): The width of the image.
+        force (bool, optional): If True, forces the conversion even if the coordinates are already in absolute values. Defaults to False.
+
+    Returns:
+        pandas.DataFrame: The DataFrame with the bounding box coordinates converted to absolute values.
+    """
     if not force and is_absolute(df):
         return df
     df = df.copy()
     if "x" not in df.columns and "bb" in df.columns:
         _recombine = True
         df = split_bb_to_xyXY(df)
     else:
```

### Comparing `torch_snippets-0.528/torch_snippets/dates.py` & `torch_snippets-0.530/torch_snippets/dates.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.528/torch_snippets/icecream.py` & `torch_snippets-0.530/torch_snippets/icecream.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.528/torch_snippets/inspector.py` & `torch_snippets-0.530/torch_snippets/inspector.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.528/torch_snippets/interactive_show.py` & `torch_snippets-0.530/torch_snippets/interactive_show.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.528/torch_snippets/ipython.py` & `torch_snippets-0.530/torch_snippets/ipython.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.528/torch_snippets/load_defaults.py` & `torch_snippets-0.530/torch_snippets/load_defaults.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.528/torch_snippets/loader.py` & `torch_snippets-0.530/torch_snippets/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
     "split",
 ]
 
 
 import os
 import re
 import sys
+from builtins import print
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 import PIL
 import tqdm
 from fastcore.all import L, delegates, patch_to
@@ -361,21 +362,26 @@
     **kwargs,
 ):
     "show an image"
 
     try:
         if isinstance(img, (str, Path)):
             img = read(str(img), 1)
-        if isinstance(img, torch.Tensor):
-            img = img.cpu().detach().numpy().copy()
+        try:
+            import torch
+
+            if isinstance(img, torch.Tensor):
+                img = img.cpu().detach().numpy().copy()
+        except ModuleNotFoundError:
+            pass
         if isinstance(img, PIL.Image.Image):
             img = np.array(img)
-
     except Exception as e:
-        print(e)
+        Warn(e)
+
     if isinstance(img, pd.DataFrame):
         df = img
         html_str = ""
         html_str += '<th style="text-align:center"><td style="vertical-align:top">'
         if title is not None:
             html_str += f'<h4 style="text-align: center;">{title}</h4>'
         max_rows = kwargs.pop("max_rows", 30)
```

### Comparing `torch_snippets-0.528/torch_snippets/logger.py` & `torch_snippets-0.530/torch_snippets/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/logging.ipynb.
 
 # %% auto 0
-__all__ = ['console', 'print', 'reset_logger_width', 'logger', 'Debug', 'Info', 'Warn', 'Excep', 'warn_mode', 'info_mode',
-           'debug_mode', 'excep_mode', 'in_warn_mode', 'in_info_mode', 'in_debug_mode', 'in_excep_mode', 'frames',
-           'get_console', 'reset_logger', 'enter_exit', 'get_logger_level', 'logger_mode', 'in_logger_mode',
-           'notify_waiting']
+__all__ = ['console', 'reset_logger_width', 'logger', 'Debug', 'Info', 'Warn', 'Excep', 'warn_mode', 'info_mode', 'debug_mode',
+           'excep_mode', 'in_warn_mode', 'in_info_mode', 'in_debug_mode', 'in_excep_mode', 'frames', 'get_console',
+           'reset_logger', 'enter_exit', 'get_logger_level', 'logger_mode', 'in_logger_mode', 'notify_waiting']
 
 # %% ../nbs/logging.ipynb 4
 from rich.console import Console
 from rich.theme import Theme
 from loguru import logger
 from datetime import datetime
 from fastcore.basics import patch_to, ifnone
@@ -36,15 +35,15 @@
                 "logging.level.exception": "bold red",
             }
         ),
     )
 
 
 console = get_console()
-print = console.print
+# print = console.print
 
 # %% ../nbs/logging.ipynb 8
 @patch_to(RichHandler)
 def render(
     self,
     *,
     record,
```

### Comparing `torch_snippets-0.528/torch_snippets/markup.py` & `torch_snippets-0.530/torch_snippets/markup.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.528/torch_snippets/markup2.py` & `torch_snippets-0.530/torch_snippets/markup2.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     "write_xml",
 ]
 
 import hashlib
 
 # %% ../nbs/markups.ipynb 2
 import json
+import os
 from collections.abc import Mapping
 from json import JSONEncoder
 from typing import Union
 
 import jsonlines
 import xmltodict
 import yaml
@@ -278,33 +279,46 @@
             elif isinstance(self[k], (L, tuple, list, set, frozenset)):
                 for i, item in enumerate(self[k]):
                     if isinstance(item, AttrDict):
                         addresses.extend(item.find_address(key, f"{new_path}.{i}"))
         return addresses
 
     def summary(self, current_path="", depth=0, sep="  ", max_items=10):
+        max_items = os.environ.get("AD_MAX_ITEMS", max_items)
+
         def format_path(path, key):
             return f"{path}.{key}" if path else key
 
         def format_item(key, item, path, depth, sep):
             import numpy as np
             import pandas as pd
-            import torch
+
+            try:
+                import torch
+            except ModuleNotFoundError:
+
+                class Torch:
+                    Tensor = type(None)
+
+                torch = Torch()
 
             if isinstance(item, (pd.DataFrame,)):
                 return f"{sep * depth}{key} - {type(item).__name__} - shape {item.shape} - columns {item.columns} - {hash_pandas_dataframe(item)}\n"
             if isinstance(item, AttrDict) or hasattr(item, "keys"):
                 item = AttrDict(**item)
                 return f"{sep*depth}{key}\n" + item.summary(path, depth + 1, sep)
             elif isinstance(item, (list, tuple, set, frozenset, L)):
                 return summarize_collection(key, item, path, depth + 1, sep)
             elif isinstance(item, (torch.Tensor, np.ndarray)):
+                is_np = False
                 if isinstance(item, np.ndarray):
+                    is_np = True
                     item = torch.tensor(item)
-                return f"{sep * depth}{key} - {item} - {hash_tensor(item)}\n"
+                is_np = "🔦" if not is_np else "np."
+                return f"{sep * depth}{key} - {is_np}{item} - {hash_tensor(item)}\n"
 
             else:
                 if isinstance(item, (int, float, complex, str)):
                     is_multiline = False
                     if isinstance(item, str):
                         is_multiline = "\n" in item
                         _sep = (
```

### Comparing `torch_snippets-0.528/torch_snippets/misc.py` & `torch_snippets-0.530/torch_snippets/misc.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.528/torch_snippets/paths.py` & `torch_snippets-0.530/torch_snippets/paths.py`

 * *Files 4% similar despite different names*

```diff
@@ -309,28 +309,28 @@
             info.append(f"{thing} - {thing.size()}")
     return "\n".join(info)
 
 
 print_folder_summary = lambda x: print(folder_summary(x))
 
 
-def tree(folder_path, *additional_flags):
-    import subprocess
+def tree(directory):
     from builtins import print
 
+    # Construct the shell command
+    shell_command = f"tree \"{directory}\" --filelimit=20 | sed 's/├/ /g; s/└/ /g; s/|/ /g; s/`/ /g; s/-/─/g; s/│/ /g; s/+/ /g'"
+    # Execute the shell command
     try:
-        # Construct the command by combining "tree" with the folder path and additional flags
-        command = ["tree", folder_path]
-        command.extend(additional_flags)
-
-        # Run the command and capture the output
-        result = subprocess.check_output(command, universal_newlines=True)
-        return print(result)
+        result = subprocess.run(
+            shell_command, shell=True, capture_output=True, text=True
+        )
+        # Print the output
+        print(result.stdout)
     except subprocess.CalledProcessError as e:
-        return f"Error: {e}"
+        print(f"Error executing command: {e}")
 
 # %% ../nbs/paths.ipynb 26
 def readlines(fpath, silent=False, encoding=None):
     with open(fpath, "r", encoding=encoding) as f:
         lines = f.read().split("\n")
         lines = [l.strip() for l in lines if l.strip() != ""]
         if not silent:
```

### Comparing `torch_snippets-0.528/torch_snippets/pdf_loader.py` & `torch_snippets-0.530/torch_snippets/pdf_loader.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.528/torch_snippets/registry.py` & `torch_snippets-0.530/torch_snippets/registry.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.528/torch_snippets/sklegos.py` & `torch_snippets-0.530/torch_snippets/sklegos.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.528/torch_snippets/text_utils.py` & `torch_snippets-0.530/torch_snippets/text_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,20 @@
     "find_substring",
     "get_line_data_from_word_data",
     "edit_distance_path",
     "group_blocks",
 ]
 import string
 
-import pandas as pd, numpy as np
+
+import matplotlib.pyplot as plt
+import numpy as np
+import pandas as pd
 from fuzzywuzzy import fuzz
 from sklearn.cluster import dbscan
-from statistics import mean
-import matplotlib.pyplot as plt
 
 from torch_snippets import *
 
 
 def textify(dataframe: pd.DataFrame, im=None, separator_size: int = 20):
     """Create text out of a dataframe returned by im2df"""
     assert isinstance(dataframe, pd.DataFrame)
@@ -169,15 +170,15 @@
     line__ = {}
     lctr = 0
     for line_ in df_.index:
         line__[line_] = lctr
         lctr += 1
     line__[-1] = -1
     # Created a dictionary to check if the numbering goes wrong
-    df["line"] = df.line_.map(lambda x: line__[x])
+    df["line"] = df.line_.map(lambda x: float(line__[x]))
     df_.index = df_.index.map(lambda x: line__[x])
     # Mapped the row numbers with the dictionary numbers
     for row in range(len(df)):
         if df.loc[row, "line_"] != -1:
             continue
         tmp = df_[df_["Y"] < df.loc[row, "Y"]]
         if tmp.index.max() is np.nan:
@@ -341,15 +342,14 @@
         else:
             ix = max(ixs, key=lambda x: lengths[x])
             ix = min(ixs)
             return ix, matches[ix]
 
 
 from difflib import SequenceMatcher as SM
-from nltk.util import ngrams
 
 
 def fuzzyfind(needle, hay):
     needle_length = len(needle.split())
     max_sim_val = 0
     max_sim_string = ""
 
@@ -368,18 +368,18 @@
 
 
 def get_line_data_from_word_data(df, line_gap=10, block_gap=10):
     df = find_lines(df, eps=line_gap)
     df = find_blocks(df, eps=block_gap)
     df = df.groupby("line_block").agg(
         {
-            "x": min,
-            "y": min,
-            "X": max,
-            "Y": max,
+            "x": "min",
+            "y": "min",
+            "X": "max",
+            "Y": "max",
             "text": lambda x: " ".join(x),
             **{c: lambda x: list(x) for c in df.columns if c not in [*"xyXY", "text"]},
         }
     )
     return df
```

### Comparing `torch_snippets-0.528/torch_snippets/thinc_parser/parser.py` & `torch_snippets-0.530/torch_snippets/thinc_parser/parser.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.528/torch_snippets/torch_loader.py` & `torch_snippets-0.530/torch_snippets/torch_loader.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.528/torch_snippets/trainer/capsule.py` & `torch_snippets-0.530/torch_snippets/trainer/capsule.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.528/torch_snippets/trainer/config.py` & `torch_snippets-0.530/torch_snippets/trainer/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,36 @@
 # %% ../../nbs/config.ipynb 1
 from ..registry import parse
 from .. import store_attr, ifnone
 import inspect as inspect_builtin
 
 # %% ../../nbs/config.ipynb 2
 class DeepLearningConfig:
+    """
+    A configuration class for deep learning models.
+
+    This class provides methods to access and manipulate configuration settings.
+
+    Attributes:
+        input_variables (list): List of input variables defined in the class constructor.
+
+    Methods:
+        keys(): Returns the list of input variables.
+        __getitem__(key): Returns the value of the specified key.
+        __contains__(key): Checks if the specified key is present in the input variables.
+        from_ini_file(filepath, config_root=None): Creates an instance of the class from an INI file.
+        __repr__(): Returns a string representation of the class.
+
+    Example usage:
+        config = DeepLearningConfig()
+        config.from_ini_file('config.ini')
+        print(config.keys())
+        print(config['learning_rate'])
+    """
+
     def keys(self):
         if not hasattr(self, "input_variables"):
             self.input_variables = inspect_builtin.signature(
                 self.__init__
             ).parameters.keys()
         return self.input_variables
```

### Comparing `torch_snippets-0.528/torch_snippets/trainer/hooks.py` & `torch_snippets-0.530/torch_snippets/trainer/hooks.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.528/torch_snippets/video.py` & `torch_snippets-0.530/torch_snippets/video.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.528/torch_snippets.egg-info/PKG-INFO` & `torch_snippets-0.530/torch_snippets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: torch-snippets
-Version: 0.528
+Version: 0.530
 Summary: One line functions for common tasks
 Home-page: https://github.com/sizhky/torch_snippets/tree/master/
 Author: Yeshwanth Reddy
 Author-email: 1992chinna@gmail.com
 License: Apache Software License 2.0
 Keywords: snippets,torch
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7
@@ -327,7 +328,9 @@
      'with_cast',
      'wrap_class',
      'write',
      'writelines',
      'xywh2xyXY',
      'zip_cycle',
      'zip_files']
+
+
```

### Comparing `torch_snippets-0.528/torch_snippets.egg-info/SOURCES.txt` & `torch_snippets-0.530/torch_snippets.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -25,21 +25,23 @@
 torch_snippets/logger.py
 torch_snippets/markup.py
 torch_snippets/markup2.py
 torch_snippets/misc.py
 torch_snippets/paths.py
 torch_snippets/pdf_loader.py
 torch_snippets/registry.py
+torch_snippets/scp.py
 torch_snippets/sklegos.py
 torch_snippets/text_utils.py
 torch_snippets/torch_loader.py
 torch_snippets/video.py
 torch_snippets.egg-info/PKG-INFO
 torch_snippets.egg-info/SOURCES.txt
 torch_snippets.egg-info/dependency_links.txt
+torch_snippets.egg-info/entry_points.txt
 torch_snippets.egg-info/not-zip-safe
 torch_snippets.egg-info/requires.txt
 torch_snippets.egg-info/top_level.txt
 torch_snippets/thinc_parser/__init__.py
 torch_snippets/thinc_parser/parser.py
 torch_snippets/trainer/__init__.py
 torch_snippets/trainer/capsule.py
```

