# Comparing `tmp/glassesValidator-1.2.4.tar.gz` & `tmp/glassesvalidator-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glassesValidator-1.2.4.tar", last modified: Wed Mar 13 16:13:00 2024, max compression
+gzip compressed data, was "glassesvalidator-1.2.5.tar", last modified: Sun May  5 19:33:40 2024, max compression
```

## Comparing `glassesValidator-1.2.4.tar` & `glassesvalidator-1.2.5.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:13:00.648316 glassesValidator-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-13 16:12:53.000000 glassesValidator-1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-13 16:12:53.000000 glassesValidator-1.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    50937 2024-03-13 16:13:00.648316 glassesValidator-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    48586 2024-03-13 16:12:53.000000 glassesValidator-1.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 16:13:00.648316 glassesValidator-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:13:00.632317 glassesValidator-1.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:13:00.636317 glassesValidator-1.2.4/src/glassesValidator/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:13:00.636317 glassesValidator-1.2.4/src/glassesValidator/GUI/
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/GUI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/GUI/_general_imgui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:13:00.640317 glassesValidator-1.2.4/src/glassesValidator/GUI/_impl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/GUI/_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/GUI/_impl/async_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)    15193 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/GUI/_impl/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    12224 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/GUI/_impl/db.py
--rw-r--r--   0 runner    (1001) docker     (127)    23661 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/GUI/_impl/filepicker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/GUI/_impl/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)   125067 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/GUI/_impl/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/GUI/_impl/imagehelper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/GUI/_impl/msgbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     7347 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/GUI/_impl/process_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/GUI/_impl/structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/GUI/_impl/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:13:00.640317 glassesValidator-1.2.4/src/glassesValidator/config/
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/config/markerPositions.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:13:00.640317 glassesValidator-1.2.4/src/glassesValidator/config/poster/
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/config/poster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   218472 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/config/poster/poster.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/config/poster/poster.tex
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/config/targetPositions.csv
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/config/validationSetup.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:13:00.640317 glassesValidator-1.2.4/src/glassesValidator/preprocess/
--rw-r--r--   0 runner    (1001) docker     (127)    15578 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/preprocess/SMI_ETG.py
--rw-r--r--   0 runner    (1001) docker     (127)    14307 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/preprocess/SeeTrue_STONE.py
--rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/preprocess/adhawk_mindlink.py
--rw-r--r--   0 runner    (1001) docker     (127)    25794 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/preprocess/pupilLabs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15117 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/preprocess/tobii_G2.py
--rw-r--r--   0 runner    (1001) docker     (127)    11940 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/preprocess/tobii_G3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:13:00.644317 glassesValidator-1.2.4/src/glassesValidator/process/
--rw-r--r--   0 runner    (1001) docker     (127)    10521 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10441 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/process/_image_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)    12562 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/process/b_codeMarkerInterval.py
--rw-r--r--   0 runner    (1001) docker     (127)     9087 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/process/c_detectMarkers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8095 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/process/d_gazeToPoster.py
--rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/process/e1_computeOffsetsToTargets.py
--rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/process/e2_determineFixationIntervals.py
--rw-r--r--   0 runner    (1001) docker     (127)     7944 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/process/f_calculateDataQuality.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:13:00.644317 glassesValidator-1.2.4/src/glassesValidator/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:13:00.644317 glassesValidator-1.2.4/src/glassesValidator/resources/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    16848 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/resources/fonts/Karla-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   556216 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/resources/fonts/NotoSans-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/resources/fonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1243500 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/resources/fonts/materialdesignicons-webfont.7.0.96.ttf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:13:00.648316 glassesValidator-1.2.4/src/glassesValidator/resources/icons/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/resources/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29894 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/resources/icons/icon.icns
--rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/resources/icons/icon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    11797 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/resources/icons/icon.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:13:00.648316 glassesValidator-1.2.4/src/glassesValidator/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    66697 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12559 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/utils/makeVideo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:13:00.648316 glassesValidator-1.2.4/src/glassesValidator/utils/mp4analyser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/utils/mp4analyser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/utils/mp4analyser/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    60401 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/utils/mp4analyser/iso.py
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/utils/mp4analyser/mpeglookups.py
--rw-r--r--   0 runner    (1001) docker     (127)    29359 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/utils/mp4analyser/non_iso.py
--rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/utils/mp4analyser/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/utils/mp4analyser/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-13 16:12:54.000000 glassesValidator-1.2.4/src/glassesValidator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:13:00.648316 glassesValidator-1.2.4/src/glassesValidator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    50937 2024-03-13 16:13:00.000000 glassesValidator-1.2.4/src/glassesValidator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-03-13 16:13:00.000000 glassesValidator-1.2.4/src/glassesValidator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 16:13:00.000000 glassesValidator-1.2.4/src/glassesValidator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-13 16:13:00.000000 glassesValidator-1.2.4/src/glassesValidator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-03-13 16:13:00.000000 glassesValidator-1.2.4/src/glassesValidator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-13 16:13:00.000000 glassesValidator-1.2.4/src/glassesValidator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:33:40.428053 glassesvalidator-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    51727 2024-05-05 19:33:40.428053 glassesvalidator-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    49376 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 19:33:40.428053 glassesvalidator-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:33:40.408053 glassesvalidator-1.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:33:40.412053 glassesvalidator-1.2.5/src/glassesValidator/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:33:40.416053 glassesvalidator-1.2.5/src/glassesValidator/GUI/
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/GUI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/GUI/_general_imgui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:33:40.416053 glassesvalidator-1.2.5/src/glassesValidator/GUI/_impl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/GUI/_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/GUI/_impl/async_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15193 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/GUI/_impl/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12224 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/GUI/_impl/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23661 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/GUI/_impl/filepicker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/GUI/_impl/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)   125075 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/GUI/_impl/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/GUI/_impl/imagehelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/GUI/_impl/msgbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7347 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/GUI/_impl/process_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/GUI/_impl/structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/GUI/_impl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:33:40.416053 glassesvalidator-1.2.5/src/glassesValidator/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/config/markerPositions.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:33:40.416053 glassesvalidator-1.2.5/src/glassesValidator/config/poster/
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/config/poster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   218472 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/config/poster/poster.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/config/poster/poster.tex
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/config/targetPositions.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/config/validationSetup.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:33:40.420053 glassesvalidator-1.2.5/src/glassesValidator/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)    15578 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/preprocess/SMI_ETG.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13968 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/preprocess/SeeTrue_STONE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/preprocess/adhawk_mindlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25794 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/preprocess/pupilLabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15117 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/preprocess/tobii_G2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11940 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/preprocess/tobii_G3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:33:40.420053 glassesvalidator-1.2.5/src/glassesValidator/process/
+-rw-r--r--   0 runner    (1001) docker     (127)    10521 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10441 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/process/_image_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12562 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/process/b_codeMarkerInterval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9087 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/process/c_detectMarkers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8095 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/process/d_gazeToPoster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/process/e1_computeOffsetsToTargets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/process/e2_determineFixationIntervals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/process/f_calculateDataQuality.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:33:40.420053 glassesvalidator-1.2.5/src/glassesValidator/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:33:40.424053 glassesvalidator-1.2.5/src/glassesValidator/resources/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    16848 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/resources/fonts/Karla-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   556216 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/resources/fonts/NotoSans-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/resources/fonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1243500 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/resources/fonts/materialdesignicons-webfont.7.0.96.ttf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:33:40.424053 glassesvalidator-1.2.5/src/glassesValidator/resources/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/resources/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29894 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/resources/icons/icon.icns
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/resources/icons/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    11797 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/resources/icons/icon.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:33:40.424053 glassesvalidator-1.2.5/src/glassesValidator/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    66690 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12559 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/utils/makeVideo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:33:40.428053 glassesvalidator-1.2.5/src/glassesValidator/utils/mp4analyser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/utils/mp4analyser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/utils/mp4analyser/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60401 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/utils/mp4analyser/iso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/utils/mp4analyser/mpeglookups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29359 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/utils/mp4analyser/non_iso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/utils/mp4analyser/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/utils/mp4analyser/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-05 19:33:36.000000 glassesvalidator-1.2.5/src/glassesValidator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:33:40.428053 glassesvalidator-1.2.5/src/glassesValidator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    51727 2024-05-05 19:33:40.000000 glassesvalidator-1.2.5/src/glassesValidator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-05 19:33:40.000000 glassesvalidator-1.2.5/src/glassesValidator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 19:33:40.000000 glassesvalidator-1.2.5/src/glassesValidator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-05 19:33:40.000000 glassesvalidator-1.2.5/src/glassesValidator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-05 19:33:40.000000 glassesvalidator-1.2.5/src/glassesValidator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-05 19:33:40.000000 glassesvalidator-1.2.5/src/glassesValidator.egg-info/top_level.txt
```

### Comparing `glassesValidator-1.2.4/LICENSE` & `glassesvalidator-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/PKG-INFO` & `glassesvalidator-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glassesValidator
-Version: 1.2.4
+Version: 1.2.5
 Summary: Automatic determination of accuracy of wearable eye tracker recordings.
 Home-page: https://github.com/dcnieho/glassesValidator
 Author: Diederick Niehorster
 Author-email: diederick_c.niehorster@humlab.lu.se
 License: MIT License
         
         Copyright (c) 2022-2023 Diederick Niehorster
@@ -53,23 +53,23 @@
 
 [![Downloads](https://static.pepy.tech/badge/glassesvalidator)](https://pepy.tech/project/glassesvalidator)
 [![Citation Badge](https://img.shields.io/endpoint?url=https%3A%2F%2Fapi.juleskreuer.eu%2Fcitation-badge.php%3Fshield%26doi%3D10.3758%2Fs13428-023-02105-5&color=blue)](https://scholar.google.com/citations?view_op=view_citation&citation_for_view=uRUYoVgAAAAJ:uWQEDVKXjbEC)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/glassesValidator.svg)](https://pypi.org/project/glassesValidator/)
 [![image](https://img.shields.io/pypi/pyversions/glassesValidator.svg)](https://pypi.org/project/glassesValidator/)
 [![DOI](https://zenodo.org/badge/DOI/10.3758/s13428-023-02105-5.svg)](https://doi.org/10.3758/s13428-023-02105-5)
 
-# GlassesValidator v1.2.4
+# GlassesValidator v1.2.5
 Tool for automatic determination of data quality (accuracy and precision) of wearable eye tracker recordings.
 
 If you use this tool or any of the code in this repository, please cite:<br>
 [Niehorster, D.C., Hessels, R.S., Benjamins, J.S., Nyström, M. and Hooge, I.T.C. (2023). GlassesValidator:
 A data quality tool for eye tracking glasses. Behavior Research Methods. doi: 10.3758/s13428-023-02105-5](https://doi.org/10.3758/s13428-023-02105-5)
 
 # How to acquire
-GlassesValidator is available from `https://github.com/dcnieho/glassesValidator`, and supports Python 3.10 and 3.11 on Windows, MacOS and Linux. 
+GlassesValidator is available from `https://github.com/dcnieho/glassesValidator`, and supports Python 3.10 and 3.11 on Windows, MacOS and Linux.
 
 For Windows users who wish to use the glassesValidator GUI, the easiest way to acquire glassesValidator is to [download
 a standalone executable](https://github.com/dcnieho/glassesValidator/releases/latest). The standalone executable is not
 available for MacOS or Linux.
 
 For users on Windows, Mac or Linux who wish to use glassesValidator in their Python code, the easiest way to acquire
 glassesValidator is to install it directly into your Python distribution using the command
@@ -91,16 +91,15 @@
         glassesValidator.GUI.run()
     ```
 
 # Usage
 The glassesValidator validation procedure consists of two parts, 1) a poster and validation procedure that is used during a recording, and 2) Python software
 for offline processing of the recording to estimate data quality measures. The glassesValidator package includes a graphical user interface (GUI)
 that can be used to perform all processing. Below we describe an example workflow using the GUI. Advanced users can however opt to call all the GUI's
-functionality directly from their own Python scripts without making use of the graphical user interface. The interested reader is referred to the glassesValidator
-manual for further details regarding how to use the glassesValidator functionality directly from their own scripts.
+functionality directly from their own Python scripts without making use of the graphical user interface. The interested reader is referred to the [API section below](#api) for further details regarding how to use the glassesValidator functionality directly from their own scripts.
 
 ## Workflow and example data
 Here we first present an example workflow using the GUI. More detailed information about [using the GUI](#the-gui), or [the programming API](#api), are provided
 below.
 
 1. Before recording, the researcher prints [the poster](#the-poster) included with glassesValidator on A2 paper. See the instructions in [the section about the
    poster](#the-poster) for checking if the poster is printed correctly.
@@ -108,22 +107,22 @@
    setting, but we think that a suitable default is to hang the poster such that the top row of fixation targets is at eye height for an average-length participant.
 3. The operator positions the participant in front of the glassesValidator poster. An easy method for positioning the participant is to ask them to stretch their
    arm out straight forward and stand at a distance where their fist touches the poster. The operator then issues the following suggested instructions:
    `Look at the nine fixation targets in reading order for one second each. Start with the top-left (red) target. When looking at the fixation targets, keep your
    head as still as possible, move only your eyes.` These verbal instructions could be accompanied by pointing at the fixation targets in the desired looking order
    to further help the participant to follow the instructions.
 4. To start calculating accuracy and precision, the researcher imports the recordings for which data quality should be determined into a glassesValidator project
-   (after any [preprocessing if required](#required-preprocessing-outside-glassesvalidator), for instance by drag-dropping a folder with recordings onto the
+   (after any [preprocessing if required](#required-preprocessing-outside-glassesvalidator)), for instance by drag-dropping a folder with recordings onto the
    glassesValidator GUI window and selecting the import action.
-5. Once imported, the researcher indicates which episode(s) of each recording contain a validation using a graphical interface included with glassesValidator. When performing this step, a GUI appears for each recording, playing back the scene video with gaze overlaid. To code one or multiple validation intervals, do the following:
-    - The scene video will start playing automatically. You can perform action in the GUI using keypresses (make sure scene video GUI has focus so that the keypresses are received). All actions you can perform are listed by hovering your mouse over the `(?)` icon in the bottom right of the GUI.
+5. Once imported, the researcher indicates which episode(s) of each recording contain a validation using a graphical interface included with glassesValidator. As described in the step-by-step annotation instructions below, a validation interval is a single continuous timespan during which a participants looks at the validation poster, spanning from the start of the look at the first fixation target to the end of the look at the last target. Do not include multiple episodes where the participants looks at the targets on the poster in a single annotated interval (for instance when you do validation twice at different distances, annotate these two validations as two separate episodes) and do not make intervals for looks to each individual validation target (glassesValidator automatically parses the gaze data and assigns looks to individual validation targets). When performing this annotation step, a GUI appears for each recording, playing back the scene video with gaze overlaid. To code one or multiple validation intervals, do the following:
+    - The scene video will start playing automatically. You can perform actions in the GUI using keypresses (make sure scene video GUI has focus so that the keypresses are received). All actions you can perform are listed by hovering your mouse over the `(?)` icon in the bottom right of the GUI.
     - Seek in the video to the start of the validation interval. To skip forward one second in the video, press `L`. For 10 seconds, press `shift+L`. To go one or ten seconds backward in the video, press `H` or `shift+H`.
     - Pause playback, and use the `J` and `K` keys to go forward and backward by one frame to precisely locate where the observer starts fixating the first validation target.
     - Press `F` to mark this frame as the start of a validation interval.
-    - Seek in the video to the end of the validation interval. Pressing `P` restarts playback of the video. Once at the end of the validation interval, pause again and again use `J` and `K` to find the precise frame where the fixation on the last validation target ends.
+    - Seek in the video to the end of the validation interval (where the observer stops looking at the last validation target). Pressing `P` restarts playback of the video. Once at the end of the validation interval, pause again and again use `J` and `K` to find the precise frame where the fixation on the last validation target ends.
     - Press `F` to mark this frame as the end of a validation interval.
     - If you have more validation intervals in the video, then seek further in the video to the next interval(s) and repeat the above actions to mark each.
     - Once done, press `Q` to close the GUI.
 6. The recordings are then further processed automatically, and data quality is determined for validation episodes in the recording.
 7. Finally, once all recordings have been processed, the researcher exports the data quality measures from the recordings in the project into a summary Excel file.
    This summary function can optionally average the data quality values over the fixation targets for each recording.
```

### Comparing `glassesValidator-1.2.4/README.md` & `glassesvalidator-1.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [![Downloads](https://static.pepy.tech/badge/glassesvalidator)](https://pepy.tech/project/glassesvalidator)
 [![Citation Badge](https://img.shields.io/endpoint?url=https%3A%2F%2Fapi.juleskreuer.eu%2Fcitation-badge.php%3Fshield%26doi%3D10.3758%2Fs13428-023-02105-5&color=blue)](https://scholar.google.com/citations?view_op=view_citation&citation_for_view=uRUYoVgAAAAJ:uWQEDVKXjbEC)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/glassesValidator.svg)](https://pypi.org/project/glassesValidator/)
 [![image](https://img.shields.io/pypi/pyversions/glassesValidator.svg)](https://pypi.org/project/glassesValidator/)
 [![DOI](https://zenodo.org/badge/DOI/10.3758/s13428-023-02105-5.svg)](https://doi.org/10.3758/s13428-023-02105-5)
 
-# GlassesValidator v1.2.4
+# GlassesValidator v1.2.5
 Tool for automatic determination of data quality (accuracy and precision) of wearable eye tracker recordings.
 
 If you use this tool or any of the code in this repository, please cite:<br>
 [Niehorster, D.C., Hessels, R.S., Benjamins, J.S., Nyström, M. and Hooge, I.T.C. (2023). GlassesValidator:
 A data quality tool for eye tracking glasses. Behavior Research Methods. doi: 10.3758/s13428-023-02105-5](https://doi.org/10.3758/s13428-023-02105-5)
 
 # How to acquire
-GlassesValidator is available from `https://github.com/dcnieho/glassesValidator`, and supports Python 3.10 and 3.11 on Windows, MacOS and Linux. 
+GlassesValidator is available from `https://github.com/dcnieho/glassesValidator`, and supports Python 3.10 and 3.11 on Windows, MacOS and Linux.
 
 For Windows users who wish to use the glassesValidator GUI, the easiest way to acquire glassesValidator is to [download
 a standalone executable](https://github.com/dcnieho/glassesValidator/releases/latest). The standalone executable is not
 available for MacOS or Linux.
 
 For users on Windows, Mac or Linux who wish to use glassesValidator in their Python code, the easiest way to acquire
 glassesValidator is to install it directly into your Python distribution using the command
@@ -38,16 +38,15 @@
         glassesValidator.GUI.run()
     ```
 
 # Usage
 The glassesValidator validation procedure consists of two parts, 1) a poster and validation procedure that is used during a recording, and 2) Python software
 for offline processing of the recording to estimate data quality measures. The glassesValidator package includes a graphical user interface (GUI)
 that can be used to perform all processing. Below we describe an example workflow using the GUI. Advanced users can however opt to call all the GUI's
-functionality directly from their own Python scripts without making use of the graphical user interface. The interested reader is referred to the glassesValidator
-manual for further details regarding how to use the glassesValidator functionality directly from their own scripts.
+functionality directly from their own Python scripts without making use of the graphical user interface. The interested reader is referred to the [API section below](#api) for further details regarding how to use the glassesValidator functionality directly from their own scripts.
 
 ## Workflow and example data
 Here we first present an example workflow using the GUI. More detailed information about [using the GUI](#the-gui), or [the programming API](#api), are provided
 below.
 
 1. Before recording, the researcher prints [the poster](#the-poster) included with glassesValidator on A2 paper. See the instructions in [the section about the
    poster](#the-poster) for checking if the poster is printed correctly.
@@ -55,22 +54,22 @@
    setting, but we think that a suitable default is to hang the poster such that the top row of fixation targets is at eye height for an average-length participant.
 3. The operator positions the participant in front of the glassesValidator poster. An easy method for positioning the participant is to ask them to stretch their
    arm out straight forward and stand at a distance where their fist touches the poster. The operator then issues the following suggested instructions:
    `Look at the nine fixation targets in reading order for one second each. Start with the top-left (red) target. When looking at the fixation targets, keep your
    head as still as possible, move only your eyes.` These verbal instructions could be accompanied by pointing at the fixation targets in the desired looking order
    to further help the participant to follow the instructions.
 4. To start calculating accuracy and precision, the researcher imports the recordings for which data quality should be determined into a glassesValidator project
-   (after any [preprocessing if required](#required-preprocessing-outside-glassesvalidator), for instance by drag-dropping a folder with recordings onto the
+   (after any [preprocessing if required](#required-preprocessing-outside-glassesvalidator)), for instance by drag-dropping a folder with recordings onto the
    glassesValidator GUI window and selecting the import action.
-5. Once imported, the researcher indicates which episode(s) of each recording contain a validation using a graphical interface included with glassesValidator. When performing this step, a GUI appears for each recording, playing back the scene video with gaze overlaid. To code one or multiple validation intervals, do the following:
-    - The scene video will start playing automatically. You can perform action in the GUI using keypresses (make sure scene video GUI has focus so that the keypresses are received). All actions you can perform are listed by hovering your mouse over the `(?)` icon in the bottom right of the GUI.
+5. Once imported, the researcher indicates which episode(s) of each recording contain a validation using a graphical interface included with glassesValidator. As described in the step-by-step annotation instructions below, a validation interval is a single continuous timespan during which a participants looks at the validation poster, spanning from the start of the look at the first fixation target to the end of the look at the last target. Do not include multiple episodes where the participants looks at the targets on the poster in a single annotated interval (for instance when you do validation twice at different distances, annotate these two validations as two separate episodes) and do not make intervals for looks to each individual validation target (glassesValidator automatically parses the gaze data and assigns looks to individual validation targets). When performing this annotation step, a GUI appears for each recording, playing back the scene video with gaze overlaid. To code one or multiple validation intervals, do the following:
+    - The scene video will start playing automatically. You can perform actions in the GUI using keypresses (make sure scene video GUI has focus so that the keypresses are received). All actions you can perform are listed by hovering your mouse over the `(?)` icon in the bottom right of the GUI.
     - Seek in the video to the start of the validation interval. To skip forward one second in the video, press `L`. For 10 seconds, press `shift+L`. To go one or ten seconds backward in the video, press `H` or `shift+H`.
     - Pause playback, and use the `J` and `K` keys to go forward and backward by one frame to precisely locate where the observer starts fixating the first validation target.
     - Press `F` to mark this frame as the start of a validation interval.
-    - Seek in the video to the end of the validation interval. Pressing `P` restarts playback of the video. Once at the end of the validation interval, pause again and again use `J` and `K` to find the precise frame where the fixation on the last validation target ends.
+    - Seek in the video to the end of the validation interval (where the observer stops looking at the last validation target). Pressing `P` restarts playback of the video. Once at the end of the validation interval, pause again and again use `J` and `K` to find the precise frame where the fixation on the last validation target ends.
     - Press `F` to mark this frame as the end of a validation interval.
     - If you have more validation intervals in the video, then seek further in the video to the next interval(s) and repeat the above actions to mark each.
     - Once done, press `Q` to close the GUI.
 6. The recordings are then further processed automatically, and data quality is determined for validation episodes in the recording.
 7. Finally, once all recordings have been processed, the researcher exports the data quality measures from the recordings in the project into a summary Excel file.
    This summary function can optionally average the data quality values over the fixation targets for each recording.
```

### Comparing `glassesValidator-1.2.4/setup.py` & `glassesvalidator-1.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/GUI/__init__.py` & `glassesvalidator-1.2.5/src/glassesValidator/GUI/__init__.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/GUI/_general_imgui.py` & `glassesvalidator-1.2.5/src/glassesValidator/GUI/_general_imgui.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/GUI/_impl/async_thread.py` & `glassesvalidator-1.2.5/src/glassesValidator/GUI/_impl/async_thread.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/GUI/_impl/callbacks.py` & `glassesvalidator-1.2.5/src/glassesValidator/GUI/_impl/callbacks.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/GUI/_impl/db.py` & `glassesvalidator-1.2.5/src/glassesValidator/GUI/_impl/db.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/GUI/_impl/filepicker.py` & `glassesvalidator-1.2.5/src/glassesValidator/GUI/_impl/filepicker.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/GUI/_impl/globals.py` & `glassesvalidator-1.2.5/src/glassesValidator/GUI/_impl/globals.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/GUI/_impl/gui.py` & `glassesvalidator-1.2.5/src/glassesValidator/GUI/_impl/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -509,18 +509,18 @@
             has_no_job = [not x for x in has_job]
             if any(has_no_job):
                 # before stage 1
                 not_imported_ids = [id for id,q in zip(ids,has_no_job) if q and get_simplified_task_state(self.recordings[id].task)==TaskSimplified.Not_Imported]
                 self.draw_recording_process_button(not_imported_ids, label="󰼛 Import", action=Task.Imported)
                 # after stage 1
                 imported_ids = [id for id,q in zip(ids,has_no_job) if q and get_simplified_task_state(self.recordings[id].task)==TaskSimplified.Imported]
-                self.draw_recording_process_button(imported_ids, label="󰼛 Code validation intervals", action=Task.Coded, should_chain_next=globals.settings.continue_process_after_code)
+                self.draw_recording_process_button(imported_ids, label="󰼛 Code validation interval(s)", action=Task.Coded, should_chain_next=globals.settings.continue_process_after_code)
                 # already coded, recode
                 recoded_ids = [id for id,q in zip(ids,has_no_job) if q and get_simplified_task_state(self.recordings[id].task) in [TaskSimplified.Coded, TaskSimplified.Processed]]
-                self.draw_recording_process_button(recoded_ids, label="󰑐 Edit validation intervals", action=Task.Coded, should_chain_next=globals.settings.continue_process_after_code)
+                self.draw_recording_process_button(recoded_ids, label="󰑐 Edit validation interval(s)", action=Task.Coded, should_chain_next=globals.settings.continue_process_after_code)
                 # after stage 2 / during stage 3
                 coded_ids = [id for id,q in zip(ids,has_no_job) if q and get_simplified_task_state(self.recordings[id].task)==TaskSimplified.Coded]
                 # NB: don't send action, so that callback code figures out where we we left off and continues there, instead of rerunning all steps of this stage (e.g. if error occurred in last step because file was opened and couldn't be written), then we only rerun the failed task and anything after it
                 self.draw_recording_process_button(coded_ids, label="󰼛 Calculate data quality", should_chain_next=True)
                 # already fully done, recompute
                 processed_ids = [id for id,q in zip(ids,has_no_job) if q and get_simplified_task_state(self.recordings[id].task)==TaskSimplified.Processed]
                 self.draw_recording_process_button(processed_ids, label="󰑐 Recalculate data quality", action=Task.Markers_Detected, should_chain_next=True)
@@ -1688,15 +1688,15 @@
                 if video_ids:
                     text.append("󰯜 Export scene video")
                     action.append(lambda: async_thread.run(callbacks.process_recordings(video_ids, task=Task.Make_Video)))
                     hover_text.append("Export scene video with gaze overlay and showing detected fiducial markers.")
                 # already coded, recode
                 recoded_ids = [id for id,q in zip(ids,has_no_job) if q and get_simplified_task_state(globals.recordings[id].task) in [TaskSimplified.Coded, TaskSimplified.Processed]]
                 if recoded_ids:
-                    text.append("󰑐 Edit validation intervals")
+                    text.append("󰑐 Edit validation interval(s)")
                     action.append(lambda: async_thread.run(callbacks.process_recordings(recoded_ids, task=Task.Coded, chain=set.continue_process_after_code)))
                     hover_text.append("Edit validation interval coding for the selected recordings.")
                 # already fully done, recompute or export results
                 processed_ids = [id for id,q in zip(ids,has_no_job) if q and get_simplified_task_state(globals.recordings[id].task)==TaskSimplified.Processed]
                 if processed_ids:
                     text.append("󰑐 Recalculate data quality")
                     action.append(lambda: async_thread.run(callbacks.process_recordings(processed_ids, task=Task.Markers_Detected)))
@@ -1706,15 +1706,15 @@
                 if not_imported_ids:
                     text.append("󰼛 Import")
                     action.append(lambda: async_thread.run(callbacks.process_recordings(not_imported_ids, task=Task.Imported, chain=False)))
                     hover_text.append("Run import job for the selected recordings.")
                 # after stage 1
                 imported_ids = [id for id,q in zip(ids,has_no_job) if q and get_simplified_task_state(globals.recordings[id].task)==TaskSimplified.Imported]
                 if imported_ids:
-                    text.append("󰼛 Code validation intervals")
+                    text.append("󰼛 Code validation interval(s)")
                     action.append(lambda: async_thread.run(callbacks.process_recordings(imported_ids, task=Task.Coded, chain=set.continue_process_after_code)))
                     hover_text.append("Code validation intervals for the selected recordings.")
                 # after stage 2 / during stage 3
                 coded_ids = [id for id,q in zip(ids,has_no_job) if q and get_simplified_task_state(globals.recordings[id].task)==TaskSimplified.Coded]
                 if coded_ids:
                     text.append("󰼛 Calculate data quality")
                     # NB: don't send action, so that callback code figures out where we we left off and continues there, instead of rerunning all steps of this stage (e.g. if error occurred in last step because file was opened and couldn't be written), then we only rerun the failed task and anything after it
```

### Comparing `glassesValidator-1.2.4/src/glassesValidator/GUI/_impl/imagehelper.py` & `glassesvalidator-1.2.5/src/glassesValidator/GUI/_impl/imagehelper.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/GUI/_impl/msgbox.py` & `glassesvalidator-1.2.5/src/glassesValidator/GUI/_impl/msgbox.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,21 +42,21 @@
         if more:
             msg_size_y += imgui.get_text_line_height_with_spacing() + imgui.get_frame_height_with_spacing()
         if icon and (diff := icon_size.y - msg_size_y) > 0:
             imgui.dummy((0, diff / 2 - imgui.style.item_spacing.y))
         imgui.text_unformatted(msg)
         if more:
             imgui.text("")
-            if imgui.tree_node("More info", flags=imgui.TreeNodeFlags_.span_avail_width):
+            if imgui.tree_node_ex("More info", flags=imgui.TreeNodeFlags_.span_avail_width):
                 size = imgui.io.display_size
                 more_size = imgui.calc_text_size(more)
-                _36 = globals.gui.scaled(26) + imgui.style.scrollbar_size
-                width = min(more_size.x + _36, size.x * 0.8 - icon_size.x)
-                height = min(more_size.y + _36, size.y * 0.7 - msg_size_y)
-                imgui.input_text_multiline(f"###more_info_{title}", more,  width=width, height=height, flags=imgui.InputTextFlags_.read_only)
+                _26 = globals.gui.scaled(26) + imgui.style.scrollbar_size
+                width = min(more_size.x + _26, size.x * 0.8 - icon_size.x)
+                height = min(more_size.y + _26, size.y * 0.7 - msg_size_y)
+                imgui.input_text_multiline(f"###more_info_{title}", more,  (width, height), flags=imgui.InputTextFlags_.read_only)
                 imgui.tree_pop()
         imgui.end_group()
         imgui.same_line(spacing=spacing)
         imgui.dummy((0, 0))
     return utils.popup(title, popup_content, buttons, closable=False, outside=False)
```

### Comparing `glassesValidator-1.2.4/src/glassesValidator/GUI/_impl/process_pool.py` & `glassesvalidator-1.2.5/src/glassesValidator/GUI/_impl/process_pool.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/GUI/_impl/structs.py` & `glassesvalidator-1.2.5/src/glassesValidator/GUI/_impl/structs.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/GUI/_impl/utils.py` & `glassesvalidator-1.2.5/src/glassesValidator/GUI/_impl/utils.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/config/__init__.py` & `glassesvalidator-1.2.5/src/glassesValidator/config/__init__.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/config/markerPositions.csv` & `glassesvalidator-1.2.5/src/glassesValidator/config/markerPositions.csv`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/config/poster/__init__.py` & `glassesvalidator-1.2.5/src/glassesValidator/config/poster/__init__.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/config/poster/poster.pdf` & `glassesvalidator-1.2.5/src/glassesValidator/config/poster/poster.pdf`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/config/poster/poster.tex` & `glassesvalidator-1.2.5/src/glassesValidator/config/poster/poster.tex`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/config/validationSetup.txt` & `glassesvalidator-1.2.5/src/glassesValidator/config/validationSetup.txt`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/preprocess/SMI_ETG.py` & `glassesvalidator-1.2.5/src/glassesValidator/preprocess/SMI_ETG.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/preprocess/SeeTrue_STONE.py` & `glassesvalidator-1.2.5/src/glassesValidator/preprocess/SeeTrue_STONE.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,14 +163,15 @@
     # make scene video
     print('  Prepping scene video...')
     # 1. see if there are frames missing, insert black frames if so
     frames = []
     for f in sceneVidDir.glob('*.jpeg'):
         _,fr = f.stem.split('_')
         frames.append(int(fr))
+    frames = sorted(frames)
 
     # 2. see if framenumbers are as expected from the gaze data file
     # get average ifi
     ifi = np.mean(np.diff(frameTimestamps.index))
     # 2.1 remove frame timestamps that are before the first frame for which we have an image
     frameTimestamps=frameTimestamps.drop(frameTimestamps[frameTimestamps.frame_idx < frames[ 0]].index)
     # 2.2 remove frame timestamps that are beyond last frame for which we have an image
@@ -207,22 +208,14 @@
         blackIm = np.zeros((h,w,3), np.uint8)   # black image
         for f in blackFrames:
             # store black frame to file
             cv2.imwrite(str(sceneVidDir / 'frame_{:d}.jpeg'.format(f)),blackIm)
             frames.append(f)
         frames = sorted(frames)
 
-    frameTsDelta = np.diff(frameTimestamps.frame_idx)
-    if np.any(frameTsDelta>1):
-        # frames missing from frametimestamps
-        err
-
-    if len(frames) != frameTimestamps.shape[0]:
-        raise RuntimeError('Number of frames ({}) isn''t equal to number of frame timestamps ({}) and this couldnt be repaired'.format(len(frames),frameTimestamps.shape[0]))
-
     # 3. make into video
     framerate = "{:.4f}".format(1000./ifi)
     cmd_str = ' '.join(['ffmpeg', '-y', '-f', 'image2', '-framerate', framerate, '-start_number', str(frames[0]), '-i', '"'+str(sceneVidDir / 'frame_%d.jpeg')+'"', '"'+str(outputDir / 'worldCamera.mp4')+'"'])
     os.system(cmd_str)
 
     # attempt 2 that should allow correct VFR video files, but doesn't work with current MediaWriter
     # due to what i think is a bug: https://github.com/matham/ffpyplayer/issues/129.
```

### Comparing `glassesValidator-1.2.4/src/glassesValidator/preprocess/__init__.py` & `glassesvalidator-1.2.5/src/glassesValidator/preprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/preprocess/adhawk_mindlink.py` & `glassesvalidator-1.2.5/src/glassesValidator/preprocess/adhawk_mindlink.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/preprocess/pupilLabs.py` & `glassesvalidator-1.2.5/src/glassesValidator/preprocess/pupilLabs.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/preprocess/tobii_G2.py` & `glassesvalidator-1.2.5/src/glassesValidator/preprocess/tobii_G2.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/preprocess/tobii_G3.py` & `glassesvalidator-1.2.5/src/glassesValidator/preprocess/tobii_G3.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/process/__init__.py` & `glassesvalidator-1.2.5/src/glassesValidator/process/__init__.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/process/_image_gui.py` & `glassesvalidator-1.2.5/src/glassesValidator/process/_image_gui.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/process/b_codeMarkerInterval.py` & `glassesvalidator-1.2.5/src/glassesValidator/process/b_codeMarkerInterval.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/process/c_detectMarkers.py` & `glassesvalidator-1.2.5/src/glassesValidator/process/c_detectMarkers.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/process/d_gazeToPoster.py` & `glassesvalidator-1.2.5/src/glassesValidator/process/d_gazeToPoster.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/process/e1_computeOffsetsToTargets.py` & `glassesvalidator-1.2.5/src/glassesValidator/process/e1_computeOffsetsToTargets.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/process/e2_determineFixationIntervals.py` & `glassesvalidator-1.2.5/src/glassesValidator/process/e2_determineFixationIntervals.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/process/f_calculateDataQuality.py` & `glassesvalidator-1.2.5/src/glassesValidator/process/f_calculateDataQuality.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,17 +114,17 @@
                         hasData = False
                         for k in ('acc_x','acc_y','acc','rms_x','rms_y','rms','std_x','std_y','std'):
                             df.loc[(i,e,t),k] = np.nan
                         if include_data_loss:
                             df.loc[(i,e,t),'data_loss'] = np.nan
 
                     if hasData:
-                        df.loc[(i,e,t),'acc_x'] = np.nanmean(data['offset_x'])
-                        df.loc[(i,e,t),'acc_y'] = np.nanmean(data['offset_y'])
-                        df.loc[(i,e,t),'acc'  ] = np.nanmean(np.hypot(data['offset_x'],data['offset_y']))
+                        df.loc[(i,e,t),'acc_x'] = np.nanmedian(data['offset_x'])
+                        df.loc[(i,e,t),'acc_y'] = np.nanmedian(data['offset_y'])
+                        df.loc[(i,e,t),'acc'  ] = np.nanmedian(np.hypot(data['offset_x'],data['offset_y']))
 
                         df.loc[(i,e,t),'rms_x'] = np.sqrt(np.nanmean(np.diff(data['offset_x'])**2))
                         df.loc[(i,e,t),'rms_y'] = np.sqrt(np.nanmean(np.diff(data['offset_y'])**2))
                         df.loc[(i,e,t),'rms'  ] = np.hypot(df.loc[(i,e,t),'rms_x'], df.loc[(i,e,t),'rms_y'])
 
                         df.loc[(i,e,t),'std_x'] = np.nanstd(data['offset_x'],ddof=1)
                         df.loc[(i,e,t),'std_y'] = np.nanstd(data['offset_y'],ddof=1)
```

### Comparing `glassesValidator-1.2.4/src/glassesValidator/resources/fonts/Karla-Regular.ttf` & `glassesvalidator-1.2.5/src/glassesValidator/resources/fonts/Karla-Regular.ttf`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/resources/fonts/NotoSans-Regular.ttf` & `glassesvalidator-1.2.5/src/glassesValidator/resources/fonts/NotoSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/resources/fonts/materialdesignicons-webfont.7.0.96.ttf` & `glassesvalidator-1.2.5/src/glassesValidator/resources/fonts/materialdesignicons-webfont.7.0.96.ttf`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/resources/icons/icon.icns` & `glassesvalidator-1.2.5/src/glassesValidator/resources/icons/icon.icns`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/resources/icons/icon.ico` & `glassesvalidator-1.2.5/src/glassesValidator/resources/icons/icon.ico`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/resources/icons/icon.png` & `glassesvalidator-1.2.5/src/glassesValidator/resources/icons/icon.png`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/utils/__init__.py` & `glassesvalidator-1.2.5/src/glassesValidator/utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
     file = path / _status_file
     if not file.is_file():
         _create_recording_status_file(file)
 
     with open(file, 'r') as f:
         return json.load(f, object_hook=json_reconstitute)
 
-def get_last_finished_step(status: typing.Dict[str,Status]):
+def get_last_finished_step(status: dict[str,Status]):
     last = Task.Not_Imported
     while (next_task:=get_next_task(last)) is not None:
         if status[str(next_task)] != Status.Finished:
             break
         last = next_task
 
     return last
```

### Comparing `glassesValidator-1.2.4/src/glassesValidator/utils/makeVideo.py` & `glassesvalidator-1.2.5/src/glassesValidator/utils/makeVideo.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/utils/mp4analyser/core.py` & `glassesvalidator-1.2.5/src/glassesValidator/utils/mp4analyser/core.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/utils/mp4analyser/iso.py` & `glassesvalidator-1.2.5/src/glassesValidator/utils/mp4analyser/iso.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/utils/mp4analyser/mpeglookups.py` & `glassesvalidator-1.2.5/src/glassesValidator/utils/mp4analyser/mpeglookups.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/utils/mp4analyser/non_iso.py` & `glassesvalidator-1.2.5/src/glassesValidator/utils/mp4analyser/non_iso.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/utils/mp4analyser/summary.py` & `glassesvalidator-1.2.5/src/glassesValidator/utils/mp4analyser/summary.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator/utils/mp4analyser/util.py` & `glassesvalidator-1.2.5/src/glassesValidator/utils/mp4analyser/util.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.2.4/src/glassesValidator.egg-info/PKG-INFO` & `glassesvalidator-1.2.5/src/glassesValidator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glassesValidator
-Version: 1.2.4
+Version: 1.2.5
 Summary: Automatic determination of accuracy of wearable eye tracker recordings.
 Home-page: https://github.com/dcnieho/glassesValidator
 Author: Diederick Niehorster
 Author-email: diederick_c.niehorster@humlab.lu.se
 License: MIT License
         
         Copyright (c) 2022-2023 Diederick Niehorster
@@ -53,23 +53,23 @@
 
 [![Downloads](https://static.pepy.tech/badge/glassesvalidator)](https://pepy.tech/project/glassesvalidator)
 [![Citation Badge](https://img.shields.io/endpoint?url=https%3A%2F%2Fapi.juleskreuer.eu%2Fcitation-badge.php%3Fshield%26doi%3D10.3758%2Fs13428-023-02105-5&color=blue)](https://scholar.google.com/citations?view_op=view_citation&citation_for_view=uRUYoVgAAAAJ:uWQEDVKXjbEC)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/glassesValidator.svg)](https://pypi.org/project/glassesValidator/)
 [![image](https://img.shields.io/pypi/pyversions/glassesValidator.svg)](https://pypi.org/project/glassesValidator/)
 [![DOI](https://zenodo.org/badge/DOI/10.3758/s13428-023-02105-5.svg)](https://doi.org/10.3758/s13428-023-02105-5)
 
-# GlassesValidator v1.2.4
+# GlassesValidator v1.2.5
 Tool for automatic determination of data quality (accuracy and precision) of wearable eye tracker recordings.
 
 If you use this tool or any of the code in this repository, please cite:<br>
 [Niehorster, D.C., Hessels, R.S., Benjamins, J.S., Nyström, M. and Hooge, I.T.C. (2023). GlassesValidator:
 A data quality tool for eye tracking glasses. Behavior Research Methods. doi: 10.3758/s13428-023-02105-5](https://doi.org/10.3758/s13428-023-02105-5)
 
 # How to acquire
-GlassesValidator is available from `https://github.com/dcnieho/glassesValidator`, and supports Python 3.10 and 3.11 on Windows, MacOS and Linux. 
+GlassesValidator is available from `https://github.com/dcnieho/glassesValidator`, and supports Python 3.10 and 3.11 on Windows, MacOS and Linux.
 
 For Windows users who wish to use the glassesValidator GUI, the easiest way to acquire glassesValidator is to [download
 a standalone executable](https://github.com/dcnieho/glassesValidator/releases/latest). The standalone executable is not
 available for MacOS or Linux.
 
 For users on Windows, Mac or Linux who wish to use glassesValidator in their Python code, the easiest way to acquire
 glassesValidator is to install it directly into your Python distribution using the command
@@ -91,16 +91,15 @@
         glassesValidator.GUI.run()
     ```
 
 # Usage
 The glassesValidator validation procedure consists of two parts, 1) a poster and validation procedure that is used during a recording, and 2) Python software
 for offline processing of the recording to estimate data quality measures. The glassesValidator package includes a graphical user interface (GUI)
 that can be used to perform all processing. Below we describe an example workflow using the GUI. Advanced users can however opt to call all the GUI's
-functionality directly from their own Python scripts without making use of the graphical user interface. The interested reader is referred to the glassesValidator
-manual for further details regarding how to use the glassesValidator functionality directly from their own scripts.
+functionality directly from their own Python scripts without making use of the graphical user interface. The interested reader is referred to the [API section below](#api) for further details regarding how to use the glassesValidator functionality directly from their own scripts.
 
 ## Workflow and example data
 Here we first present an example workflow using the GUI. More detailed information about [using the GUI](#the-gui), or [the programming API](#api), are provided
 below.
 
 1. Before recording, the researcher prints [the poster](#the-poster) included with glassesValidator on A2 paper. See the instructions in [the section about the
    poster](#the-poster) for checking if the poster is printed correctly.
@@ -108,22 +107,22 @@
    setting, but we think that a suitable default is to hang the poster such that the top row of fixation targets is at eye height for an average-length participant.
 3. The operator positions the participant in front of the glassesValidator poster. An easy method for positioning the participant is to ask them to stretch their
    arm out straight forward and stand at a distance where their fist touches the poster. The operator then issues the following suggested instructions:
    `Look at the nine fixation targets in reading order for one second each. Start with the top-left (red) target. When looking at the fixation targets, keep your
    head as still as possible, move only your eyes.` These verbal instructions could be accompanied by pointing at the fixation targets in the desired looking order
    to further help the participant to follow the instructions.
 4. To start calculating accuracy and precision, the researcher imports the recordings for which data quality should be determined into a glassesValidator project
-   (after any [preprocessing if required](#required-preprocessing-outside-glassesvalidator), for instance by drag-dropping a folder with recordings onto the
+   (after any [preprocessing if required](#required-preprocessing-outside-glassesvalidator)), for instance by drag-dropping a folder with recordings onto the
    glassesValidator GUI window and selecting the import action.
-5. Once imported, the researcher indicates which episode(s) of each recording contain a validation using a graphical interface included with glassesValidator. When performing this step, a GUI appears for each recording, playing back the scene video with gaze overlaid. To code one or multiple validation intervals, do the following:
-    - The scene video will start playing automatically. You can perform action in the GUI using keypresses (make sure scene video GUI has focus so that the keypresses are received). All actions you can perform are listed by hovering your mouse over the `(?)` icon in the bottom right of the GUI.
+5. Once imported, the researcher indicates which episode(s) of each recording contain a validation using a graphical interface included with glassesValidator. As described in the step-by-step annotation instructions below, a validation interval is a single continuous timespan during which a participants looks at the validation poster, spanning from the start of the look at the first fixation target to the end of the look at the last target. Do not include multiple episodes where the participants looks at the targets on the poster in a single annotated interval (for instance when you do validation twice at different distances, annotate these two validations as two separate episodes) and do not make intervals for looks to each individual validation target (glassesValidator automatically parses the gaze data and assigns looks to individual validation targets). When performing this annotation step, a GUI appears for each recording, playing back the scene video with gaze overlaid. To code one or multiple validation intervals, do the following:
+    - The scene video will start playing automatically. You can perform actions in the GUI using keypresses (make sure scene video GUI has focus so that the keypresses are received). All actions you can perform are listed by hovering your mouse over the `(?)` icon in the bottom right of the GUI.
     - Seek in the video to the start of the validation interval. To skip forward one second in the video, press `L`. For 10 seconds, press `shift+L`. To go one or ten seconds backward in the video, press `H` or `shift+H`.
     - Pause playback, and use the `J` and `K` keys to go forward and backward by one frame to precisely locate where the observer starts fixating the first validation target.
     - Press `F` to mark this frame as the start of a validation interval.
-    - Seek in the video to the end of the validation interval. Pressing `P` restarts playback of the video. Once at the end of the validation interval, pause again and again use `J` and `K` to find the precise frame where the fixation on the last validation target ends.
+    - Seek in the video to the end of the validation interval (where the observer stops looking at the last validation target). Pressing `P` restarts playback of the video. Once at the end of the validation interval, pause again and again use `J` and `K` to find the precise frame where the fixation on the last validation target ends.
     - Press `F` to mark this frame as the end of a validation interval.
     - If you have more validation intervals in the video, then seek further in the video to the next interval(s) and repeat the above actions to mark each.
     - Once done, press `Q` to close the GUI.
 6. The recordings are then further processed automatically, and data quality is determined for validation episodes in the recording.
 7. Finally, once all recordings have been processed, the researcher exports the data quality measures from the recordings in the project into a summary Excel file.
    This summary function can optionally average the data quality values over the fixation targets for each recording.
```

### Comparing `glassesValidator-1.2.4/src/glassesValidator.egg-info/SOURCES.txt` & `glassesvalidator-1.2.5/src/glassesValidator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

