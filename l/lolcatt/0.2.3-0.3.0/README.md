# Comparing `tmp/lolcatt-0.2.3.tar.gz` & `tmp/lolcatt-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lolcatt-0.2.3.tar", last modified: Sun Jul 16 12:48:18 2023, max compression
+gzip compressed data, was "lolcatt-0.3.0.tar", last modified: Sun May  5 20:43:17 2024, max compression
```

## Comparing `lolcatt-0.2.3.tar` & `lolcatt-0.3.0.tar`

### file list

```diff
@@ -1,66 +1,54 @@
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 12:48:18.288195 lolcatt-0.2.3/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1074 2023-06-30 16:54:52.000000 lolcatt-0.2.3/LICENSE
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      239 2023-06-30 20:26:17.000000 lolcatt-0.2.3/MANIFEST.in
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4187 2023-07-16 12:48:18.288195 lolcatt-0.2.3/PKG-INFO
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     3508 2023-07-16 12:36:17.000000 lolcatt-0.2.3/README.rst
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 12:48:18.288195 lolcatt-0.2.3/docs/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      608 2023-06-30 16:54:52.000000 lolcatt-0.2.3/docs/Makefile
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 12:48:18.284195 lolcatt-0.2.3/docs/_build/
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 12:48:18.284195 lolcatt-0.2.3/docs/_build/html/
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 12:48:18.288195 lolcatt-0.2.3/docs/_build/html/_static/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    14813 2023-07-16 12:36:26.000000 lolcatt-0.2.3/docs/_build/html/_static/basic.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       84 2023-06-30 16:54:52.000000 lolcatt-0.2.3/docs/_build/html/_static/custom.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      286 2023-05-12 22:36:26.000000 lolcatt-0.2.3/docs/_build/html/_static/file.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       90 2023-05-12 22:36:26.000000 lolcatt-0.2.3/docs/_build/html/_static/minus.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4208 2023-07-16 12:36:26.000000 lolcatt-0.2.3/docs/_build/html/_static/nature.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       90 2023-05-12 22:36:26.000000 lolcatt-0.2.3/docs/_build/html/_static/plus.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4956 2023-07-16 12:36:26.000000 lolcatt-0.2.3/docs/_build/html/_static/pygments.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    26168 2023-07-16 00:40:56.000000 lolcatt-0.2.3/docs/_build/html/_static/screenshot.png
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 12:48:18.288195 lolcatt-0.2.3/docs/_static/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       84 2023-06-30 16:54:52.000000 lolcatt-0.2.3/docs/_static/custom.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    26168 2023-07-16 00:40:56.000000 lolcatt-0.2.3/docs/_static/screenshot.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4983 2023-06-30 21:18:35.000000 lolcatt-0.2.3/docs/conf.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      264 2023-06-30 16:54:52.000000 lolcatt-0.2.3/docs/index.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1138 2023-06-30 16:54:52.000000 lolcatt-0.2.3/docs/installation.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      346 2023-07-07 17:09:03.000000 lolcatt-0.2.3/docs/lolcatt.casting.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      517 2023-07-16 12:36:23.000000 lolcatt-0.2.3/docs/lolcatt.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1232 2023-07-07 17:09:03.000000 lolcatt-0.2.3/docs/lolcatt.ui.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      331 2023-07-07 17:09:03.000000 lolcatt-0.2.3/docs/lolcatt.utils.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      805 2023-06-30 16:54:52.000000 lolcatt-0.2.3/docs/make.bat
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       58 2023-07-16 12:36:23.000000 lolcatt-0.2.3/docs/modules.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       27 2023-06-30 16:54:52.000000 lolcatt-0.2.3/docs/readme.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       69 2023-06-30 16:54:52.000000 lolcatt-0.2.3/docs/usage.rst
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 12:48:18.288195 lolcatt-0.2.3/lolcatt/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       41 2023-07-16 00:01:30.000000 lolcatt-0.2.3/lolcatt/.githash
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      125 2023-07-16 12:39:51.000000 lolcatt-0.2.3/lolcatt/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1378 2023-07-16 01:35:15.000000 lolcatt-0.2.3/lolcatt/app.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 12:48:18.288195 lolcatt-0.2.3/lolcatt/casting/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-03 23:40:52.000000 lolcatt-0.2.3/lolcatt/casting/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    10010 2023-07-16 12:11:43.000000 lolcatt-0.2.3/lolcatt/casting/caster.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1336 2023-07-16 00:40:56.000000 lolcatt-0.2.3/lolcatt/casting/youtube_playlist_handler.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1801 2023-07-16 12:19:23.000000 lolcatt-0.2.3/lolcatt/cli.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 12:48:18.288195 lolcatt-0.2.3/lolcatt/ui/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-03 23:40:52.000000 lolcatt-0.2.3/lolcatt/ui/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1579 2023-07-16 01:35:15.000000 lolcatt-0.2.3/lolcatt/ui/lolcatt.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4860 2023-07-16 00:40:56.000000 lolcatt-0.2.3/lolcatt/ui/lolcatt_controls.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1265 2023-07-07 17:09:03.000000 lolcatt-0.2.3/lolcatt/ui/lolcatt_device_info.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1561 2023-07-16 00:40:53.000000 lolcatt-0.2.3/lolcatt/ui/lolcatt_playback_info.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     3068 2023-07-16 12:16:20.000000 lolcatt-0.2.3/lolcatt/ui/lolcatt_progress.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     2917 2023-07-16 12:16:38.000000 lolcatt-0.2.3/lolcatt/ui/lolcatt_url_input.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 12:48:18.288195 lolcatt-0.2.3/lolcatt/utils/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-07 17:09:03.000000 lolcatt-0.2.3/lolcatt/utils/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     2422 2023-07-16 10:50:45.000000 lolcatt-0.2.3/lolcatt/utils/utils.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 12:48:18.288195 lolcatt-0.2.3/lolcatt.egg-info/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4187 2023-07-16 12:48:18.000000 lolcatt-0.2.3/lolcatt.egg-info/PKG-INFO
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1297 2023-07-16 12:48:18.000000 lolcatt-0.2.3/lolcatt.egg-info/SOURCES.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        1 2023-07-16 12:48:18.000000 lolcatt-0.2.3/lolcatt.egg-info/dependency_links.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       45 2023-07-16 12:48:18.000000 lolcatt-0.2.3/lolcatt.egg-info/entry_points.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        1 2023-07-16 12:48:18.000000 lolcatt-0.2.3/lolcatt.egg-info/not-zip-safe
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       52 2023-07-16 12:48:18.000000 lolcatt-0.2.3/lolcatt.egg-info/requires.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        8 2023-07-16 12:48:18.000000 lolcatt-0.2.3/lolcatt.egg-info/top_level.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      558 2023-07-16 12:39:51.000000 lolcatt-0.2.3/pyproject.toml
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      354 2023-07-16 12:48:18.292195 lolcatt-0.2.3/setup.cfg
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1556 2023-07-16 12:39:51.000000 lolcatt-0.2.3/setup.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-16 12:48:18.288195 lolcatt-0.2.3/tests/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       37 2023-06-30 16:54:52.000000 lolcatt-0.2.3/tests/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      211 2023-07-15 16:19:10.000000 lolcatt-0.2.3/tests/test_lolcatt.py
+drwxrwxr-x   0 lueftinger  (1000) lueftinger  (1000)        0 2024-05-05 20:43:17.610986 lolcatt-0.3.0/
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)     1074 2024-02-16 09:11:52.000000 lolcatt-0.3.0/LICENSE
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)      239 2024-02-16 09:11:52.000000 lolcatt-0.3.0/MANIFEST.in
+-rw-r--r--   0 lueftinger  (1000) lueftinger  (1000)     4312 2024-05-05 20:43:17.610986 lolcatt-0.3.0/PKG-INFO
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)     3504 2024-02-16 09:11:52.000000 lolcatt-0.3.0/README.rst
+drwxrwxr-x   0 lueftinger  (1000) lueftinger  (1000)        0 2024-05-05 20:43:17.610986 lolcatt-0.3.0/docs/
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)      608 2024-02-16 09:11:52.000000 lolcatt-0.3.0/docs/Makefile
+drwxrwxr-x   0 lueftinger  (1000) lueftinger  (1000)        0 2024-05-05 20:43:17.610986 lolcatt-0.3.0/docs/_static/
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)       84 2024-02-16 09:11:52.000000 lolcatt-0.3.0/docs/_static/custom.css
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)    26168 2024-02-16 09:11:52.000000 lolcatt-0.3.0/docs/_static/screenshot.png
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)     4983 2024-02-16 09:15:01.000000 lolcatt-0.3.0/docs/conf.py
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)      264 2024-02-16 09:11:52.000000 lolcatt-0.3.0/docs/index.rst
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)     1138 2024-02-16 09:11:52.000000 lolcatt-0.3.0/docs/installation.rst
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)      346 2024-02-16 09:11:52.000000 lolcatt-0.3.0/docs/lolcatt.casting.rst
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)      517 2024-02-16 09:11:52.000000 lolcatt-0.3.0/docs/lolcatt.rst
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)     1232 2024-02-16 09:11:52.000000 lolcatt-0.3.0/docs/lolcatt.ui.rst
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)      331 2024-02-16 09:11:52.000000 lolcatt-0.3.0/docs/lolcatt.utils.rst
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)      805 2024-02-16 09:11:52.000000 lolcatt-0.3.0/docs/make.bat
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)       58 2024-02-16 09:11:52.000000 lolcatt-0.3.0/docs/modules.rst
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)       27 2024-02-16 09:11:52.000000 lolcatt-0.3.0/docs/readme.rst
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)       69 2024-02-16 09:11:52.000000 lolcatt-0.3.0/docs/usage.rst
+drwxrwxr-x   0 lueftinger  (1000) lueftinger  (1000)        0 2024-05-05 20:43:17.610986 lolcatt-0.3.0/lolcatt/
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)      125 2024-05-05 20:42:54.000000 lolcatt-0.3.0/lolcatt/__init__.py
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)     1378 2024-02-16 09:15:01.000000 lolcatt-0.3.0/lolcatt/app.py
+drwxrwxr-x   0 lueftinger  (1000) lueftinger  (1000)        0 2024-05-05 20:43:17.610986 lolcatt-0.3.0/lolcatt/casting/
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)        0 2024-02-16 09:11:52.000000 lolcatt-0.3.0/lolcatt/casting/__init__.py
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)    10035 2024-02-16 09:15:01.000000 lolcatt-0.3.0/lolcatt/casting/caster.py
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)     1336 2024-02-16 09:15:01.000000 lolcatt-0.3.0/lolcatt/casting/youtube_playlist_handler.py
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)     1828 2024-05-05 20:42:54.000000 lolcatt-0.3.0/lolcatt/cli.py
+drwxrwxr-x   0 lueftinger  (1000) lueftinger  (1000)        0 2024-05-05 20:43:17.610986 lolcatt-0.3.0/lolcatt/ui/
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)        0 2024-02-16 09:11:52.000000 lolcatt-0.3.0/lolcatt/ui/__init__.py
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)     1579 2024-02-16 09:11:52.000000 lolcatt-0.3.0/lolcatt/ui/lolcatt.css
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)     4860 2024-02-16 09:15:01.000000 lolcatt-0.3.0/lolcatt/ui/lolcatt_controls.py
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)     1265 2024-02-16 09:15:01.000000 lolcatt-0.3.0/lolcatt/ui/lolcatt_device_info.py
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)     1640 2024-02-16 09:15:01.000000 lolcatt-0.3.0/lolcatt/ui/lolcatt_playback_info.py
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)     3068 2024-02-16 09:15:01.000000 lolcatt-0.3.0/lolcatt/ui/lolcatt_progress.py
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)     3016 2024-02-16 09:15:01.000000 lolcatt-0.3.0/lolcatt/ui/lolcatt_url_input.py
+drwxrwxr-x   0 lueftinger  (1000) lueftinger  (1000)        0 2024-05-05 20:43:17.610986 lolcatt-0.3.0/lolcatt/utils/
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)        0 2024-02-16 09:11:52.000000 lolcatt-0.3.0/lolcatt/utils/__init__.py
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)     2422 2024-02-16 09:15:01.000000 lolcatt-0.3.0/lolcatt/utils/utils.py
+drwxrwxr-x   0 lueftinger  (1000) lueftinger  (1000)        0 2024-05-05 20:43:17.610986 lolcatt-0.3.0/lolcatt.egg-info/
+-rw-r--r--   0 lueftinger  (1000) lueftinger  (1000)     4312 2024-05-05 20:43:17.000000 lolcatt-0.3.0/lolcatt.egg-info/PKG-INFO
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)      982 2024-05-05 20:43:17.000000 lolcatt-0.3.0/lolcatt.egg-info/SOURCES.txt
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)        1 2024-05-05 20:43:17.000000 lolcatt-0.3.0/lolcatt.egg-info/dependency_links.txt
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)       45 2024-05-05 20:43:17.000000 lolcatt-0.3.0/lolcatt.egg-info/entry_points.txt
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)        1 2024-05-05 20:28:54.000000 lolcatt-0.3.0/lolcatt.egg-info/not-zip-safe
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)       54 2024-05-05 20:43:17.000000 lolcatt-0.3.0/lolcatt.egg-info/requires.txt
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)        8 2024-05-05 20:43:17.000000 lolcatt-0.3.0/lolcatt.egg-info/top_level.txt
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)      559 2024-05-05 20:42:54.000000 lolcatt-0.3.0/pyproject.toml
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)       38 2024-05-05 20:43:17.610986 lolcatt-0.3.0/setup.cfg
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)     1556 2024-05-05 20:42:54.000000 lolcatt-0.3.0/setup.py
+drwxrwxr-x   0 lueftinger  (1000) lueftinger  (1000)        0 2024-05-05 20:43:17.610986 lolcatt-0.3.0/tests/
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)       37 2024-02-16 09:11:52.000000 lolcatt-0.3.0/tests/__init__.py
+-rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)      211 2024-02-16 09:11:52.000000 lolcatt-0.3.0/tests/test_lolcatt.py
```

### Comparing `lolcatt-0.2.3/LICENSE` & `lolcatt-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.3/PKG-INFO` & `lolcatt-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lolcatt
-Version: 0.2.3
+Version: 0.3.0
 Summary: A TUI wrapper around `catt`.
 Home-page: https://github.com/LokiLuciferase/lolcatt
 Author: Lukas Lüftinger
 Author-email: lukas.lueftinger@outlook.com
 License: MIT license
 Keywords: lolcatt
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,14 +13,19 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 License-File: LICENSE
+Requires-Dist: toml
+Requires-Dist: click>=8
+Requires-Dist: yt-dlp>=2024.04.09
+Requires-Dist: textual>=0.30.0
+Requires-Dist: catt
 
 =======
 lolcatt
 =======
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
@@ -65,15 +70,15 @@
 Quckstart
 ----------
 
 At first we need to determine the name of the chromecast device we want to cast to. To do so, run ``lolcatt --scan``.
 To start the UI, run ``lolcatt -d '<device name or alias>'`` (or simply ``lolcatt`` if a default device is set).
 A default device and device aliases can be set in the ``catt`` configuration file (per default under ``~/.config/catt/config.cfg``), see catt_'s documentation for more information.
 
-To cast, paste either a URL or a path to a local file into the input field and press enter. To prepend a URL or path to the playback queue instead of playing immediately, hit Ctrl+s instead of enter. To seek, tap the progress bar.
+To cast, paste either a URL or a path to a local file into the input field and press enter. To add a URL or path to the playback queue instead of playing immediately, hit Ctrl+s instead of enter. To seek, tap the progress bar.
 
 For URLs, all websites supported by yt-dlp_ (which handles media download under the hood) are supported. Find a list of supported websites here_. For local media, most common video and image formats are supported.
 
 Youtube playlists are supported, and each contained video will be added to the playback queue. By specifying a cookie file in the config (per default under ``~/.config/lolcatt/config.toml``), you can also access private YouTube playlists such as "Watch Later" (https://www.youtube.com/playlist?list=WL), and ensure played YouTube videos are marked as watched.
 
 
 Troubleshooting
```

### Comparing `lolcatt-0.2.3/README.rst` & `lolcatt-0.3.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 Quckstart
 ----------
 
 At first we need to determine the name of the chromecast device we want to cast to. To do so, run ``lolcatt --scan``.
 To start the UI, run ``lolcatt -d '<device name or alias>'`` (or simply ``lolcatt`` if a default device is set).
 A default device and device aliases can be set in the ``catt`` configuration file (per default under ``~/.config/catt/config.cfg``), see catt_'s documentation for more information.
 
-To cast, paste either a URL or a path to a local file into the input field and press enter. To prepend a URL or path to the playback queue instead of playing immediately, hit Ctrl+s instead of enter. To seek, tap the progress bar.
+To cast, paste either a URL or a path to a local file into the input field and press enter. To add a URL or path to the playback queue instead of playing immediately, hit Ctrl+s instead of enter. To seek, tap the progress bar.
 
 For URLs, all websites supported by yt-dlp_ (which handles media download under the hood) are supported. Find a list of supported websites here_. For local media, most common video and image formats are supported.
 
 Youtube playlists are supported, and each contained video will be added to the playback queue. By specifying a cookie file in the config (per default under ``~/.config/lolcatt/config.toml``), you can also access private YouTube playlists such as "Watch Later" (https://www.youtube.com/playlist?list=WL), and ensure played YouTube videos are marked as watched.
 
 
 Troubleshooting
```

### Comparing `lolcatt-0.2.3/docs/Makefile` & `lolcatt-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.3/docs/_build/html/_static/screenshot.png` & `lolcatt-0.3.0/docs/_static/screenshot.png`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.3/docs/conf.py` & `lolcatt-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.3/docs/installation.rst` & `lolcatt-0.3.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.3/docs/lolcatt.rst` & `lolcatt-0.3.0/docs/lolcatt.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.3/docs/lolcatt.ui.rst` & `lolcatt-0.3.0/docs/lolcatt.ui.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.3/docs/make.bat` & `lolcatt-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.3/lolcatt/app.py` & `lolcatt-0.3.0/lolcatt/app.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.3/lolcatt/casting/caster.py` & `lolcatt-0.3.0/lolcatt/casting/caster.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 @dataclass
 class CastState:
     """Dataclass for cast state, encapsulating info dictionaries of a catt controller."""
 
     cast_info: dict
     info: dict
     is_loading: bool = False
-    media_loaded: bool = False
+    loading_failed: bool = False
     queue_len: int = 0
 
 
 class Caster:
     """
     Class encapsulating the catt.api.CattDevice.
 
@@ -52,15 +52,15 @@
         self._current_item = None
         self._played_queue = []
         self._available_devices = None
         self._catt_call = None
         self._catt_config = get_config_as_dict()
         self._loading_started = time.time()
         self._is_loading_cast = True
-        self._media_loaded = False
+        self._media_loading_failed = False
         self._loading_timeout = 8
         self._update_interval = update_interval
         self._autoplay = autoplay
         self._state_last_updated = time.time()
         self.change_device(name_or_alias)
 
     def _build_cast_args(self) -> List[str]:
@@ -264,38 +264,37 @@
         if time.time() - self._state_last_updated > self._update_interval:
             self._device.controller._update_status()
             self._state_last_updated = time.time()
 
         if self._is_loading_cast and time.time() - self._loading_started > self._loading_timeout:
             self._loading_started = None
             self._is_loading_cast = False
+            self._media_loading_failed = True
 
         if self._device.controller.cast_info.get('player_state') in [
             'PLAYING',
             'BUFFERING',
             'PAUSED',
         ]:
             self._loading_started = None
             self._is_loading_cast = False
-            self._media_loaded = True
-        else:
-            self._media_loaded = False
 
     def get_cast_state(self) -> CastState:
         """
         Returns a CastState object encapsulating the info dictionaries of the currently active
         CattDevice.
 
         :return: A CastState object
         """
         self._tick()
         if self._device is None:
-            cs = CastState({}, {}, False, False)
+            cs = CastState({}, {}, False, False, 0)
         else:
             cs = CastState(
                 self._device.controller.cast_info,
                 self._device.controller.info,
                 is_loading=self._is_loading_cast,
-                media_loaded=self._media_loaded,
+                loading_failed=self._media_loading_failed,
                 queue_len=len(self._queue),
             )
+            self._media_loading_failed = False
         return cs
```

### Comparing `lolcatt-0.2.3/lolcatt/casting/youtube_playlist_handler.py` & `lolcatt-0.3.0/lolcatt/casting/youtube_playlist_handler.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.3/lolcatt/cli.py` & `lolcatt-0.3.0/lolcatt/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 @click.command(
     'lolcatt',
     context_settings=dict(help_option_names=['-h', '--help']),
 )
 @click.version_option(__version__, '-v', '--version', prog_name='lolcatt')
 @click.argument(
     'url_or_path',
-    nargs=1,
+    nargs=-1,
     default=None,
     required=False,
 )
 @click.option(
     '-d',
     '--device',
     default='default',
@@ -53,14 +53,15 @@
 
     if url_or_path is None and scan:
         do_scan()
         return
 
     lolcatt = LolCatt(device_name=device, config=config)
     if url_or_path is not None:
-        lolcatt.caster.enqueue(url_or_path)
+        for up in url_or_path:
+            lolcatt.caster.enqueue(up)
         lolcatt.caster.cast_next()
     lolcatt.run()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `lolcatt-0.2.3/lolcatt/ui/lolcatt.css` & `lolcatt-0.3.0/lolcatt/ui/lolcatt.css`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.3/lolcatt/ui/lolcatt_controls.py` & `lolcatt-0.3.0/lolcatt/ui/lolcatt_controls.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.3/lolcatt/ui/lolcatt_device_info.py` & `lolcatt-0.3.0/lolcatt/ui/lolcatt_device_info.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.3/lolcatt/ui/lolcatt_playback_info.py` & `lolcatt-0.3.0/lolcatt/ui/lolcatt_playback_info.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,24 +11,27 @@
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.label = Label('', id='title')
         self._marquee_gen = None
 
     def _get_playback_info(self) -> str:
-        playing = self.app.caster.get_cast_state().cast_info.get('title')
-        display_name = self.app.caster.get_cast_state().info.get('display_name')
-        is_loading = self.app.caster.get_cast_state().is_loading
+        state = self.app.caster.get_cast_state()
+        playing = state.cast_info.get('title')
+        display_name = state.info.get('display_name')
 
         if playing is not None:
             return f'Playing: "{playing}"'
         elif display_name is not None and display_name != 'Backdrop':
             return f'Displaying: "{display_name}"'
-        elif is_loading:
+        elif state.is_loading:
             return 'Loading...'
+        elif state.loading_failed:
+            self.app.notify('Loading failed.', severity='warning')
+            return 'Nothing is playing.'
         else:
             return 'Nothing is playing.'
 
     def _update_label(self):
         self.label_str = self._get_playback_info() + ' '
         self.label.update(next(self._marquee_gen))
```

### Comparing `lolcatt-0.2.3/lolcatt/ui/lolcatt_progress.py` & `lolcatt-0.3.0/lolcatt/ui/lolcatt_progress.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.3/lolcatt/ui/lolcatt_url_input.py` & `lolcatt-0.3.0/lolcatt/ui/lolcatt_url_input.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     ]
 
     async def action_enqueue(self) -> None:
         """Handle an enqueue action.
 
         Normally triggered by the user pressing Ctrl+s. This will also run any validators.
         """
-        print('enqueue')
         validation_result = self.validate(self.value)
         self.post_message(self.Enqueued(self, self.value, validation_result))
 
 
 class LolCattUrlInput(Static):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -52,22 +51,24 @@
     def cast_url(self):
         if self._input.value == '':
             return
         if self._input.value:
             self.app.caster.enqueue(self._input.value, front=True)
             self._input.value = ''
             self.app.caster.cast_next()
+            self.notify('Playing...', severity='information')
 
     @on(InputField.Enqueued, '#url_input')
     def enqueue_url(self):
         if self._input.value == '':
             return
         if self._input.value:
-            self.app.caster.enqueue(self._input.value, front=True)
+            self.app.caster.enqueue(self._input.value, front=False)
             self._input.value = ''
+            self.notify('Enqueued.', severity='information')
 
     def compose(self):
         yield Container(self._input, id='url_input_container')
 
     def on_key(self, event: Key):
         if event.key == 'escape':
             self.app.remote_screen.focus_next()
```

### Comparing `lolcatt-0.2.3/lolcatt/utils/utils.py` & `lolcatt-0.3.0/lolcatt/utils/utils.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.2.3/lolcatt.egg-info/PKG-INFO` & `lolcatt-0.3.0/lolcatt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lolcatt
-Version: 0.2.3
+Version: 0.3.0
 Summary: A TUI wrapper around `catt`.
 Home-page: https://github.com/LokiLuciferase/lolcatt
 Author: Lukas Lüftinger
 Author-email: lukas.lueftinger@outlook.com
 License: MIT license
 Keywords: lolcatt
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,14 +13,19 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 License-File: LICENSE
+Requires-Dist: toml
+Requires-Dist: click>=8
+Requires-Dist: yt-dlp>=2024.04.09
+Requires-Dist: textual>=0.30.0
+Requires-Dist: catt
 
 =======
 lolcatt
 =======
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
@@ -65,15 +70,15 @@
 Quckstart
 ----------
 
 At first we need to determine the name of the chromecast device we want to cast to. To do so, run ``lolcatt --scan``.
 To start the UI, run ``lolcatt -d '<device name or alias>'`` (or simply ``lolcatt`` if a default device is set).
 A default device and device aliases can be set in the ``catt`` configuration file (per default under ``~/.config/catt/config.cfg``), see catt_'s documentation for more information.
 
-To cast, paste either a URL or a path to a local file into the input field and press enter. To prepend a URL or path to the playback queue instead of playing immediately, hit Ctrl+s instead of enter. To seek, tap the progress bar.
+To cast, paste either a URL or a path to a local file into the input field and press enter. To add a URL or path to the playback queue instead of playing immediately, hit Ctrl+s instead of enter. To seek, tap the progress bar.
 
 For URLs, all websites supported by yt-dlp_ (which handles media download under the hood) are supported. Find a list of supported websites here_. For local media, most common video and image formats are supported.
 
 Youtube playlists are supported, and each contained video will be added to the playback queue. By specifying a cookie file in the config (per default under ``~/.config/lolcatt/config.toml``), you can also access private YouTube playlists such as "Watch Later" (https://www.youtube.com/playlist?list=WL), and ensure played YouTube videos are marked as watched.
 
 
 Troubleshooting
```

### Comparing `lolcatt-0.2.3/pyproject.toml` & `lolcatt-0.3.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -15,20 +15,20 @@
   | buck-out
   | build
   | dist
 )/
 '''
 
 [tool.bumpver]
-current_version = "0.2.3"
+current_version = "0.3.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
-push = true
+push = false
 
 [tool.bumpver.file_patterns]
 "setup.py" = [
     "{version}",
 ]
 "lolcatt/__init__.py" = [
     "__version__ = '{version}'",
```

### Comparing `lolcatt-0.2.3/setup.py` & `lolcatt-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     include_package_data=True,
     keywords='lolcatt',
     name='lolcatt',
     packages=find_packages(include=['lolcatt', 'lolcatt.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/LokiLuciferase/lolcatt',
-    version='0.2.3',
+    version='0.3.0',
     zip_safe=False,
 )
```

