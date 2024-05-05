# Comparing `tmp/super_rubik_cube-1.0.2.tar.gz` & `tmp/super_rubik_cube-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "super_rubik_cube-1.0.2.tar", last modified: Sat May  4 16:47:59 2024, max compression
+gzip compressed data, was "super_rubik_cube-1.0.3.tar", last modified: Sat May  4 17:51:59 2024, max compression
```

## Comparing `super_rubik_cube-1.0.2.tar` & `super_rubik_cube-1.0.3.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 16:47:59.628768 super_rubik_cube-1.0.2/
--rw-rw-rw-   0        0        0    35816 2024-05-03 20:00:15.000000 super_rubik_cube-1.0.2/LICENSE
--rw-rw-rw-   0        0        0    20792 2024-05-04 16:47:59.627725 super_rubik_cube-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    20379 2024-05-04 16:27:14.000000 super_rubik_cube-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-04 16:47:59.628768 super_rubik_cube-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      772 2024-05-04 16:47:53.000000 super_rubik_cube-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-04 16:47:59.626725 super_rubik_cube-1.0.2/super_rubik_cube.egg-info/
--rw-rw-rw-   0        0        0    20792 2024-05-04 16:47:59.000000 super_rubik_cube-1.0.2/super_rubik_cube.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2057 2024-05-04 16:47:59.000000 super_rubik_cube-1.0.2/super_rubik_cube.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 16:47:59.000000 super_rubik_cube-1.0.2/super_rubik_cube.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-04 16:47:59.000000 super_rubik_cube-1.0.2/super_rubik_cube.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-04 16:47:59.591132 super_rubik_cube-1.0.2/supercube/
--rw-rw-rw-   0        0        0  3674160 2024-05-03 18:33:03.000000 super_rubik_cube-1.0.2/supercube/.cornerprun
--rw-rw-rw-   0        0        0    90720 2024-05-03 18:32:54.000000 super_rubik_cube-1.0.2/supercube/.move_cornperm
--rw-rw-rw-   0        0        0      297 2024-05-03 15:53:19.000000 super_rubik_cube-1.0.2/supercube/NCube.py
--rw-rw-rw-   0        0        0     1215 2024-05-03 17:20:04.000000 super_rubik_cube-1.0.2/supercube/PocketCube.py
--rw-rw-rw-   0        0        0     1207 2024-05-03 17:17:11.000000 super_rubik_cube-1.0.2/supercube/RubiksCube.py
--rw-rw-rw-   0        0        0       96 2024-05-03 15:43:15.000000 super_rubik_cube-1.0.2/supercube/__init__.py
--rw-rw-rw-   0        0        0    31193 2024-04-14 21:26:56.000000 super_rubik_cube-1.0.2/supercube/cube.py
-drwxrwxrwx   0        0        0        0 2024-05-04 16:47:59.593132 super_rubik_cube-1.0.2/supercube/kociemba/
--rw-rw-rw-   0        0        0     1462 2024-05-03 17:19:32.000000 super_rubik_cube-1.0.2/supercube/kociemba/__init__.py
--rw-rw-rw-   0        0        0     1119 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/build_ckociemba.py
--rw-rw-rw-   0        0        0      413 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/command_line.py
-drwxrwxrwx   0        0        0        0 2024-05-04 16:47:59.597659 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/
--rw-rw-rw-   0        0        0        0 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/__init__.py
--rw-rw-rw-   0        0        0      412 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/color.py
--rw-rw-rw-   0        0        0    19234 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/coordcube.py
--rw-rw-rw-   0        0        0      529 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/corner.py
--rw-rw-rw-   0        0        0    20176 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/cubiecube.py
--rw-rw-rw-   0        0        0      598 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/edge.py
--rw-rw-rw-   0        0        0     4060 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/facecube.py
--rw-rw-rw-   0        0        0     3178 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/facelet.py
-drwxrwxrwx   0        0        0        0 2024-05-04 16:47:59.618216 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/
--rw-rw-rw-   0        0        0  1844165 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/FRtoBR_Move.pkl
--rw-rw-rw-   0        0        0   729671 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/MergeURtoULandUBtoDF.pkl
--rw-rw-rw-   0        0        0  3524721 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/Slice_Flip_Prun.pkl
--rw-rw-rw-   0        0        0  3758442 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/Slice_Twist_Prun.pkl
--rw-rw-rw-   0        0        0  3381387 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/Slice_URFtoDLF_Parity_Prun.pkl
--rw-rw-rw-   0        0        0  3375661 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/Slice_URtoDF_Parity_Prun.pkl
--rw-rw-rw-   0        0        0   182203 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/UBtoDF_Move.pkl
--rw-rw-rw-   0        0        0  3276605 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/URFtoDLF_Move.pkl
--rw-rw-rw-   0        0        0  3483565 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/URtoDF_Move.pkl
--rw-rw-rw-   0        0        0   182203 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/URtoUL_Move.pkl
--rw-rw-rw-   0        0        0   294315 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/flipMove.pkl
--rw-rw-rw-   0        0        0   315721 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/twistMove.pkl
--rw-rw-rw-   0        0        0    13523 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/search.py
--rw-rw-rw-   0        0        0     2485 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-04 16:47:59.626725 super_rubik_cube-1.0.2/supercube/kociemba_2x2/
--rw-rw-rw-   0        0        0        0 2024-04-02 12:07:35.000000 super_rubik_cube-1.0.2/supercube/kociemba_2x2/__init__.py
--rw-rw-rw-   0        0        0     7752 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.2/supercube/kociemba_2x2/client_gui.py
--rw-rw-rw-   0        0        0     1150 2024-05-03 17:23:20.000000 super_rubik_cube-1.0.2/supercube/kociemba_2x2/coord.py
--rw-rw-rw-   0        0        0     7188 2024-05-03 17:22:29.000000 super_rubik_cube-1.0.2/supercube/kociemba_2x2/cubie.py
--rw-rw-rw-   0        0        0     1122 2024-05-03 17:21:59.000000 super_rubik_cube-1.0.2/supercube/kociemba_2x2/defs.py
--rw-rw-rw-   0        0        0     2021 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.2/supercube/kociemba_2x2/enums.py
--rw-rw-rw-   0        0        0     2980 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.2/supercube/kociemba_2x2/example.py
--rw-rw-rw-   0        0        0     4874 2024-05-03 17:21:50.000000 super_rubik_cube-1.0.2/supercube/kociemba_2x2/face.py
--rw-rw-rw-   0        0        0      493 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.2/supercube/kociemba_2x2/misc.py
--rw-rw-rw-   0        0        0     2157 2024-05-04 16:45:18.000000 super_rubik_cube-1.0.2/supercube/kociemba_2x2/moves.py
--rw-rw-rw-   0        0        0     1918 2024-05-04 16:45:26.000000 super_rubik_cube-1.0.2/supercube/kociemba_2x2/pruning.py
--rw-rw-rw-   0        0        0     2598 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.2/supercube/kociemba_2x2/sockets.py
--rw-rw-rw-   0        0        0     2758 2024-05-03 17:21:32.000000 super_rubik_cube-1.0.2/supercube/kociemba_2x2/solver.py
--rw-rw-rw-   0        0        0      412 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.2/supercube/kociemba_2x2/start_server.py
+drwxrwxrwx   0        0        0        0 2024-05-04 17:51:59.006789 super_rubik_cube-1.0.3/
+-rw-rw-rw-   0        0        0    35816 2024-05-03 20:00:15.000000 super_rubik_cube-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0    22858 2024-05-04 17:51:59.006789 super_rubik_cube-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    22367 2024-05-04 17:51:41.000000 super_rubik_cube-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-04 17:51:59.007790 super_rubik_cube-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      904 2024-05-04 17:45:35.000000 super_rubik_cube-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 17:51:59.005782 super_rubik_cube-1.0.3/super_rubik_cube.egg-info/
+-rw-rw-rw-   0        0        0    22858 2024-05-04 17:51:58.000000 super_rubik_cube-1.0.3/super_rubik_cube.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2057 2024-05-04 17:51:58.000000 super_rubik_cube-1.0.3/super_rubik_cube.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 17:51:58.000000 super_rubik_cube-1.0.3/super_rubik_cube.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-04 17:51:58.000000 super_rubik_cube-1.0.3/super_rubik_cube.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 17:51:58.966106 super_rubik_cube-1.0.3/supercube/
+-rw-rw-rw-   0        0        0  3674160 2024-05-03 18:33:03.000000 super_rubik_cube-1.0.3/supercube/.cornerprun
+-rw-rw-rw-   0        0        0    90720 2024-05-03 18:32:54.000000 super_rubik_cube-1.0.3/supercube/.move_cornperm
+-rw-rw-rw-   0        0        0      297 2024-05-03 15:53:19.000000 super_rubik_cube-1.0.3/supercube/NCube.py
+-rw-rw-rw-   0        0        0     1215 2024-05-03 17:20:04.000000 super_rubik_cube-1.0.3/supercube/PocketCube.py
+-rw-rw-rw-   0        0        0     1207 2024-05-03 17:17:11.000000 super_rubik_cube-1.0.3/supercube/RubiksCube.py
+-rw-rw-rw-   0        0        0       96 2024-05-03 15:43:15.000000 super_rubik_cube-1.0.3/supercube/__init__.py
+-rw-rw-rw-   0        0        0    31193 2024-04-14 21:26:56.000000 super_rubik_cube-1.0.3/supercube/cube.py
+drwxrwxrwx   0        0        0        0 2024-05-04 17:51:58.968105 super_rubik_cube-1.0.3/supercube/kociemba/
+-rw-rw-rw-   0        0        0     1462 2024-05-03 17:19:32.000000 super_rubik_cube-1.0.3/supercube/kociemba/__init__.py
+-rw-rw-rw-   0        0        0     1119 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.3/supercube/kociemba/build_ckociemba.py
+-rw-rw-rw-   0        0        0      413 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.3/supercube/kociemba/command_line.py
+drwxrwxrwx   0        0        0        0 2024-05-04 17:51:58.975161 super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/
+-rw-rw-rw-   0        0        0        0 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/__init__.py
+-rw-rw-rw-   0        0        0      412 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/color.py
+-rw-rw-rw-   0        0        0    19234 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/coordcube.py
+-rw-rw-rw-   0        0        0      529 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/corner.py
+-rw-rw-rw-   0        0        0    20176 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/cubiecube.py
+-rw-rw-rw-   0        0        0      598 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/edge.py
+-rw-rw-rw-   0        0        0     4060 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/facecube.py
+-rw-rw-rw-   0        0        0     3178 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/facelet.py
+drwxrwxrwx   0        0        0        0 2024-05-04 17:51:58.995739 super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/prunetables/
+-rw-rw-rw-   0        0        0  1844165 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/prunetables/FRtoBR_Move.pkl
+-rw-rw-rw-   0        0        0   729671 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/prunetables/MergeURtoULandUBtoDF.pkl
+-rw-rw-rw-   0        0        0  3524721 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/prunetables/Slice_Flip_Prun.pkl
+-rw-rw-rw-   0        0        0  3758442 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/prunetables/Slice_Twist_Prun.pkl
+-rw-rw-rw-   0        0        0  3381387 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/prunetables/Slice_URFtoDLF_Parity_Prun.pkl
+-rw-rw-rw-   0        0        0  3375661 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/prunetables/Slice_URtoDF_Parity_Prun.pkl
+-rw-rw-rw-   0        0        0   182203 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/prunetables/UBtoDF_Move.pkl
+-rw-rw-rw-   0        0        0  3276605 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/prunetables/URFtoDLF_Move.pkl
+-rw-rw-rw-   0        0        0  3483565 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/prunetables/URtoDF_Move.pkl
+-rw-rw-rw-   0        0        0   182203 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/prunetables/URtoUL_Move.pkl
+-rw-rw-rw-   0        0        0   294315 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/prunetables/flipMove.pkl
+-rw-rw-rw-   0        0        0   315721 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/prunetables/twistMove.pkl
+-rw-rw-rw-   0        0        0    13523 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/search.py
+-rw-rw-rw-   0        0        0     2485 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-04 17:51:59.005253 super_rubik_cube-1.0.3/supercube/kociemba_2x2/
+-rw-rw-rw-   0        0        0        0 2024-04-02 12:07:35.000000 super_rubik_cube-1.0.3/supercube/kociemba_2x2/__init__.py
+-rw-rw-rw-   0        0        0     7752 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.3/supercube/kociemba_2x2/client_gui.py
+-rw-rw-rw-   0        0        0     1150 2024-05-03 17:23:20.000000 super_rubik_cube-1.0.3/supercube/kociemba_2x2/coord.py
+-rw-rw-rw-   0        0        0     7188 2024-05-03 17:22:29.000000 super_rubik_cube-1.0.3/supercube/kociemba_2x2/cubie.py
+-rw-rw-rw-   0        0        0     1122 2024-05-03 17:21:59.000000 super_rubik_cube-1.0.3/supercube/kociemba_2x2/defs.py
+-rw-rw-rw-   0        0        0     2021 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.3/supercube/kociemba_2x2/enums.py
+-rw-rw-rw-   0        0        0     2980 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.3/supercube/kociemba_2x2/example.py
+-rw-rw-rw-   0        0        0     4874 2024-05-03 17:21:50.000000 super_rubik_cube-1.0.3/supercube/kociemba_2x2/face.py
+-rw-rw-rw-   0        0        0      493 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.3/supercube/kociemba_2x2/misc.py
+-rw-rw-rw-   0        0        0     2157 2024-05-04 16:45:18.000000 super_rubik_cube-1.0.3/supercube/kociemba_2x2/moves.py
+-rw-rw-rw-   0        0        0     1918 2024-05-04 16:45:26.000000 super_rubik_cube-1.0.3/supercube/kociemba_2x2/pruning.py
+-rw-rw-rw-   0        0        0     2598 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.3/supercube/kociemba_2x2/sockets.py
+-rw-rw-rw-   0        0        0     2758 2024-05-03 17:21:32.000000 super_rubik_cube-1.0.3/supercube/kociemba_2x2/solver.py
+-rw-rw-rw-   0        0        0      412 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.3/supercube/kociemba_2x2/start_server.py
```

### Comparing `super_rubik_cube-1.0.2/LICENSE` & `super_rubik_cube-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/PKG-INFO` & `super_rubik_cube-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 Metadata-Version: 2.1
 Name: super-rubik-cube
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library for simulating rubik's cubes of different sizes (N x N), and for solving 2 x 2 and 3 x 3 cubes with kociemba algorithm.
 Author: Ilmi28
 Author-email: <ilmialiev28@gmail.com>
+License: GPL-3.0
+Project-URL: Homepage, https://github.com/Ilmi28/SuperCube
 Keywords: python,rubik,cube,solve,3x3,2x2,rubik's cube,pocket cube,NxN,kociemba,supercube
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Description
 Library for Rubik's Cube manipulation. Creator and customizer for cubes of any size, and solver for 2x2 and 3x3 cubes (Herbert Kociemba's algorithms)
 
+# Installation
+
+```
+pip install super-rubik-cube
+```
+
 # Usage
-> Note: 2D number cube grid looks a bit weird in output examples, but in console everything looks fine.
+> Note: 2D number cube grid may look a bit weird in output examples, but in console everything looks fine.
 ## Creating instance of cube
 You can create Rubik's cube, Pocket cube and NxN cube, where N means positive number.
 ```
 import supercube
 
 rubiks_cube = supercube.RubiksCube() # creates 3X3 cube
 pocket_cube = supercube.PocketCube() # creates 2x2 cube
@@ -228,14 +236,15 @@
                                     └───────────────────────────────────┘
 ```
 ## Scrambling
 You can scramble cube by using method `scramble(number_of_moves=30)`(default value is 30)
 ```
 print(rubiks_cube.scramble())
 rubiks_cube.show()
+rubiks_cube.show(colors=True)
 ```
 Output:
 ```
 B' F' D' B2 F' R' F' L B2 B2 U F D' D2 F' U2 F' R R U' B U L D2 U2 R' U' D D2 F2 
              ┌────────────┐
              │ 36  51  21 │
              │ 26   5  44 │
@@ -245,19 +254,31 @@
 │ 42  14   8 │ 20  23  49 │ 17  32  38 │  2  41  13 │ 
 │ 18  15  16 │ 52  24  48 │ 27   4   3 │ 37   6  46 │ 
 └────────────┼────────────┼────────────┴────────────┘
              │ 45  31  34 │
              │ 22  50  11 │
              │ 25  29  30 │
              └────────────┘
+⬛⬛⬛ 🟥🟨🟩
+⬛⬛⬛ 🟩🟪🟦
+⬛⬛⬛ 🟧🟥🟩
+
+🟦🟨🟪 🟦🟦🟪 🟧🟨🟥 🟪🟥🟨 
+🟦🟧🟪 🟩🟩🟨 🟧🟥🟦 🟪🟦🟧 
+🟧🟧🟧 🟨🟩🟨 🟩🟪🟪 🟦🟪🟨 
+
+⬛⬛⬛ 🟦🟥🟥
+⬛⬛⬛ 🟩🟨🟧
+⬛⬛⬛ 🟩🟥🟥
 ```
 You can also scramble big cubes 
 ```
 print(n_cube.scramble())
 n_cube.show()
+n_cube.show(colors=True)
 ```
 Output:
 ```
 U' 2Bw 2Rw2 3Uw 3L 2B2 3Dw2 2B 2Bw' 2L 3Fw' D2 2Rw 3R 2Rw' 2Bw 2R 3Rw' 2Fw' 3Fw 3B2 L2 2F' 3R2 R' 3Uw2 2Bw 3F' B' B 
                                     ┌───────────────────────────────────┐
                                     │ 294  134  292   71  113    6  197 │
                                     │ 289  205   59   11   87  254  161 │
@@ -279,14 +300,37 @@
                                     │  44  135   79   72   38   58   85 │
                                     │ 103  283  115   81  278  216   78 │
                                     │  22  268  122  270  228  121  175 │
                                     │  96  167   31   18   33  279   94 │
                                     │  51  107  159  272  265  258  251 │
                                     │  99  155   45  273  266  259  252 │
                                     └───────────────────────────────────┘
+⬛⬛⬛⬛⬛⬛⬛ 🟨🟩🟨🟧🟩🟪🟦
+⬛⬛⬛⬛⬛⬛⬛ 🟨🟦🟧🟪🟧🟨🟥
+⬛⬛⬛⬛⬛⬛⬛ 🟧🟥🟦🟪🟧🟩🟩
+⬛⬛⬛⬛⬛⬛⬛ 🟪🟥🟨🟪🟦🟩🟨
+⬛⬛⬛⬛⬛⬛⬛ 🟨🟩🟨🟥🟦🟨🟦
+⬛⬛⬛⬛⬛⬛⬛ 🟥🟧🟦🟪🟪🟪🟨
+⬛⬛⬛⬛⬛⬛⬛ 🟧🟩🟧🟪🟦🟪🟥
+
+🟥🟦🟪🟩🟩🟨🟨 🟩🟪🟩🟦🟧🟦🟪 🟩🟧🟥🟧🟥🟦🟪 🟥🟦🟧🟦🟦🟧🟦 
+🟩🟦🟧🟧🟩🟨🟨 🟧🟪🟪🟧🟧🟧🟨 🟦🟦🟧🟥🟩🟨🟨 🟩🟪🟩🟩🟥🟥🟥 
+🟩🟦🟥🟧🟩🟩🟧 🟪🟩🟦🟪🟧🟦🟪 🟦🟧🟥🟥🟧🟨🟦 🟪🟧🟨🟦🟥🟥🟥 
+🟨🟦🟨🟧🟧🟨🟪 🟥🟥🟥🟩🟧🟦🟩 🟧🟧🟦🟥🟨🟥🟨 🟩🟪🟩🟦🟩🟦🟦 
+🟦🟦🟥🟩🟦🟩🟥 🟪🟪🟪🟪🟨🟦🟥 🟦🟦🟩🟥🟪🟥🟨 🟩🟪🟩🟨🟧🟪🟨 
+🟪🟥🟨🟩🟥🟩🟩 🟧🟪🟪🟪🟨🟧🟧 🟦🟩🟪🟨🟥🟥🟥 🟦🟥🟦🟦🟨🟦🟥 
+🟪🟪🟨🟧🟪🟩🟧 🟦🟪🟪🟩🟥🟪🟨 🟦🟦🟦🟦🟨🟩🟩 🟥🟥🟥🟥🟩🟩🟧 
+
+⬛⬛⬛⬛⬛⬛⬛ 🟪🟥🟥🟥🟨🟧🟧
+⬛⬛⬛⬛⬛⬛⬛ 🟪🟩🟧🟧🟪🟧🟧
+⬛⬛⬛⬛⬛⬛⬛ 🟩🟨🟩🟧🟨🟦🟧
+⬛⬛⬛⬛⬛⬛⬛ 🟪🟨🟩🟨🟦🟩🟥
+⬛⬛⬛⬛⬛⬛⬛ 🟧🟥🟪🟪🟪🟨🟧
+⬛⬛⬛⬛⬛⬛⬛ 🟧🟩🟥🟨🟨🟨🟨
+⬛⬛⬛⬛⬛⬛⬛ 🟩🟥🟪🟨🟨🟨🟨
 ```
 
 # Solving
 Only Rubik's cube and Pocket cube can be solved. Cubes are solved with Herbert Kociemba's algorithm.
 ```
 print(rubiks_cube.scramble())
 rubiks_cube.show()
```

### Comparing `super_rubik_cube-1.0.2/README.md` & `super_rubik_cube-1.0.3/super_rubik_cube.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,30 @@
+Metadata-Version: 2.1
+Name: super-rubik-cube
+Version: 1.0.3
+Summary: Library for simulating rubik's cubes of different sizes (N x N), and for solving 2 x 2 and 3 x 3 cubes with kociemba algorithm.
+Author: Ilmi28
+Author-email: <ilmialiev28@gmail.com>
+License: GPL-3.0
+Project-URL: Homepage, https://github.com/Ilmi28/SuperCube
+Keywords: python,rubik,cube,solve,3x3,2x2,rubik's cube,pocket cube,NxN,kociemba,supercube
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Description
 Library for Rubik's Cube manipulation. Creator and customizer for cubes of any size, and solver for 2x2 and 3x3 cubes (Herbert Kociemba's algorithms)
 
+# Installation
+
+```
+pip install super-rubik-cube
+```
+
 # Usage
-> Note: 2D number cube grid looks a bit weird in output examples, but in console everything looks fine.
+> Note: 2D number cube grid may look a bit weird in output examples, but in console everything looks fine.
 ## Creating instance of cube
 You can create Rubik's cube, Pocket cube and NxN cube, where N means positive number.
 ```
 import supercube
 
 rubiks_cube = supercube.RubiksCube() # creates 3X3 cube
 pocket_cube = supercube.PocketCube() # creates 2x2 cube
@@ -218,14 +236,15 @@
                                     └───────────────────────────────────┘
 ```
 ## Scrambling
 You can scramble cube by using method `scramble(number_of_moves=30)`(default value is 30)
 ```
 print(rubiks_cube.scramble())
 rubiks_cube.show()
+rubiks_cube.show(colors=True)
 ```
 Output:
 ```
 B' F' D' B2 F' R' F' L B2 B2 U F D' D2 F' U2 F' R R U' B U L D2 U2 R' U' D D2 F2 
              ┌────────────┐
              │ 36  51  21 │
              │ 26   5  44 │
@@ -235,19 +254,31 @@
 │ 42  14   8 │ 20  23  49 │ 17  32  38 │  2  41  13 │ 
 │ 18  15  16 │ 52  24  48 │ 27   4   3 │ 37   6  46 │ 
 └────────────┼────────────┼────────────┴────────────┘
              │ 45  31  34 │
              │ 22  50  11 │
              │ 25  29  30 │
              └────────────┘
+⬛⬛⬛ 🟥🟨🟩
+⬛⬛⬛ 🟩🟪🟦
+⬛⬛⬛ 🟧🟥🟩
+
+🟦🟨🟪 🟦🟦🟪 🟧🟨🟥 🟪🟥🟨 
+🟦🟧🟪 🟩🟩🟨 🟧🟥🟦 🟪🟦🟧 
+🟧🟧🟧 🟨🟩🟨 🟩🟪🟪 🟦🟪🟨 
+
+⬛⬛⬛ 🟦🟥🟥
+⬛⬛⬛ 🟩🟨🟧
+⬛⬛⬛ 🟩🟥🟥
 ```
 You can also scramble big cubes 
 ```
 print(n_cube.scramble())
 n_cube.show()
+n_cube.show(colors=True)
 ```
 Output:
 ```
 U' 2Bw 2Rw2 3Uw 3L 2B2 3Dw2 2B 2Bw' 2L 3Fw' D2 2Rw 3R 2Rw' 2Bw 2R 3Rw' 2Fw' 3Fw 3B2 L2 2F' 3R2 R' 3Uw2 2Bw 3F' B' B 
                                     ┌───────────────────────────────────┐
                                     │ 294  134  292   71  113    6  197 │
                                     │ 289  205   59   11   87  254  161 │
@@ -269,14 +300,37 @@
                                     │  44  135   79   72   38   58   85 │
                                     │ 103  283  115   81  278  216   78 │
                                     │  22  268  122  270  228  121  175 │
                                     │  96  167   31   18   33  279   94 │
                                     │  51  107  159  272  265  258  251 │
                                     │  99  155   45  273  266  259  252 │
                                     └───────────────────────────────────┘
+⬛⬛⬛⬛⬛⬛⬛ 🟨🟩🟨🟧🟩🟪🟦
+⬛⬛⬛⬛⬛⬛⬛ 🟨🟦🟧🟪🟧🟨🟥
+⬛⬛⬛⬛⬛⬛⬛ 🟧🟥🟦🟪🟧🟩🟩
+⬛⬛⬛⬛⬛⬛⬛ 🟪🟥🟨🟪🟦🟩🟨
+⬛⬛⬛⬛⬛⬛⬛ 🟨🟩🟨🟥🟦🟨🟦
+⬛⬛⬛⬛⬛⬛⬛ 🟥🟧🟦🟪🟪🟪🟨
+⬛⬛⬛⬛⬛⬛⬛ 🟧🟩🟧🟪🟦🟪🟥
+
+🟥🟦🟪🟩🟩🟨🟨 🟩🟪🟩🟦🟧🟦🟪 🟩🟧🟥🟧🟥🟦🟪 🟥🟦🟧🟦🟦🟧🟦 
+🟩🟦🟧🟧🟩🟨🟨 🟧🟪🟪🟧🟧🟧🟨 🟦🟦🟧🟥🟩🟨🟨 🟩🟪🟩🟩🟥🟥🟥 
+🟩🟦🟥🟧🟩🟩🟧 🟪🟩🟦🟪🟧🟦🟪 🟦🟧🟥🟥🟧🟨🟦 🟪🟧🟨🟦🟥🟥🟥 
+🟨🟦🟨🟧🟧🟨🟪 🟥🟥🟥🟩🟧🟦🟩 🟧🟧🟦🟥🟨🟥🟨 🟩🟪🟩🟦🟩🟦🟦 
+🟦🟦🟥🟩🟦🟩🟥 🟪🟪🟪🟪🟨🟦🟥 🟦🟦🟩🟥🟪🟥🟨 🟩🟪🟩🟨🟧🟪🟨 
+🟪🟥🟨🟩🟥🟩🟩 🟧🟪🟪🟪🟨🟧🟧 🟦🟩🟪🟨🟥🟥🟥 🟦🟥🟦🟦🟨🟦🟥 
+🟪🟪🟨🟧🟪🟩🟧 🟦🟪🟪🟩🟥🟪🟨 🟦🟦🟦🟦🟨🟩🟩 🟥🟥🟥🟥🟩🟩🟧 
+
+⬛⬛⬛⬛⬛⬛⬛ 🟪🟥🟥🟥🟨🟧🟧
+⬛⬛⬛⬛⬛⬛⬛ 🟪🟩🟧🟧🟪🟧🟧
+⬛⬛⬛⬛⬛⬛⬛ 🟩🟨🟩🟧🟨🟦🟧
+⬛⬛⬛⬛⬛⬛⬛ 🟪🟨🟩🟨🟦🟩🟥
+⬛⬛⬛⬛⬛⬛⬛ 🟧🟥🟪🟪🟪🟨🟧
+⬛⬛⬛⬛⬛⬛⬛ 🟧🟩🟥🟨🟨🟨🟨
+⬛⬛⬛⬛⬛⬛⬛ 🟩🟥🟪🟨🟨🟨🟨
 ```
 
 # Solving
 Only Rubik's cube and Pocket cube can be solved. Cubes are solved with Herbert Kociemba's algorithm.
 ```
 print(rubiks_cube.scramble())
 rubiks_cube.show()
```

### Comparing `super_rubik_cube-1.0.2/setup.py` & `super_rubik_cube-1.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 from setuptools import setup, find_packages
 
 DESCRIPTION="Library for simulating rubik's cubes of different sizes (N x N), and for solving 2 x 2 and 3 x 3 cubes with kociemba algorithm."
 LONG_DESCRIPTION = open("README.md", encoding="utf8").read()
+project_urls = {
+    "Homepage": "https://github.com/Ilmi28/SuperCube"
+}
 
 
 setup(
     name="super-rubik-cube",
-    version="1.0.2",
+    version="1.0.3",
     author="Ilmi28",
     author_email="<ilmialiev28@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     package_data={'supercube': ['.cornerprun', '.move_cornperm', 'kociemba/pykociemba/prunetables/*']},
     packages=find_packages(),
-    keywords=['python', 'rubik', 'cube', 'solve', '3x3', '2x2', "rubik's cube", 'pocket cube', 'NxN', 'kociemba', 'supercube']
+    keywords=['python', 'rubik', 'cube', 'solve', '3x3', '2x2', "rubik's cube", 'pocket cube', 'NxN', 'kociemba', 'supercube'],
+    project_urls=project_urls,
+    license='GPL-3.0'
 )
```

### Comparing `super_rubik_cube-1.0.2/super_rubik_cube.egg-info/PKG-INFO` & `super_rubik_cube-1.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,18 @@
-Metadata-Version: 2.1
-Name: super-rubik-cube
-Version: 1.0.2
-Summary: Library for simulating rubik's cubes of different sizes (N x N), and for solving 2 x 2 and 3 x 3 cubes with kociemba algorithm.
-Author: Ilmi28
-Author-email: <ilmialiev28@gmail.com>
-Keywords: python,rubik,cube,solve,3x3,2x2,rubik's cube,pocket cube,NxN,kociemba,supercube
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Description
 Library for Rubik's Cube manipulation. Creator and customizer for cubes of any size, and solver for 2x2 and 3x3 cubes (Herbert Kociemba's algorithms)
 
+# Installation
+
+```
+pip install super-rubik-cube
+```
+
 # Usage
-> Note: 2D number cube grid looks a bit weird in output examples, but in console everything looks fine.
+> Note: 2D number cube grid may look a bit weird in output examples, but in console everything looks fine.
 ## Creating instance of cube
 You can create Rubik's cube, Pocket cube and NxN cube, where N means positive number.
 ```
 import supercube
 
 rubiks_cube = supercube.RubiksCube() # creates 3X3 cube
 pocket_cube = supercube.PocketCube() # creates 2x2 cube
@@ -228,14 +224,15 @@
                                     └───────────────────────────────────┘
 ```
 ## Scrambling
 You can scramble cube by using method `scramble(number_of_moves=30)`(default value is 30)
 ```
 print(rubiks_cube.scramble())
 rubiks_cube.show()
+rubiks_cube.show(colors=True)
 ```
 Output:
 ```
 B' F' D' B2 F' R' F' L B2 B2 U F D' D2 F' U2 F' R R U' B U L D2 U2 R' U' D D2 F2 
              ┌────────────┐
              │ 36  51  21 │
              │ 26   5  44 │
@@ -245,19 +242,31 @@
 │ 42  14   8 │ 20  23  49 │ 17  32  38 │  2  41  13 │ 
 │ 18  15  16 │ 52  24  48 │ 27   4   3 │ 37   6  46 │ 
 └────────────┼────────────┼────────────┴────────────┘
              │ 45  31  34 │
              │ 22  50  11 │
              │ 25  29  30 │
              └────────────┘
+⬛⬛⬛ 🟥🟨🟩
+⬛⬛⬛ 🟩🟪🟦
+⬛⬛⬛ 🟧🟥🟩
+
+🟦🟨🟪 🟦🟦🟪 🟧🟨🟥 🟪🟥🟨 
+🟦🟧🟪 🟩🟩🟨 🟧🟥🟦 🟪🟦🟧 
+🟧🟧🟧 🟨🟩🟨 🟩🟪🟪 🟦🟪🟨 
+
+⬛⬛⬛ 🟦🟥🟥
+⬛⬛⬛ 🟩🟨🟧
+⬛⬛⬛ 🟩🟥🟥
 ```
 You can also scramble big cubes 
 ```
 print(n_cube.scramble())
 n_cube.show()
+n_cube.show(colors=True)
 ```
 Output:
 ```
 U' 2Bw 2Rw2 3Uw 3L 2B2 3Dw2 2B 2Bw' 2L 3Fw' D2 2Rw 3R 2Rw' 2Bw 2R 3Rw' 2Fw' 3Fw 3B2 L2 2F' 3R2 R' 3Uw2 2Bw 3F' B' B 
                                     ┌───────────────────────────────────┐
                                     │ 294  134  292   71  113    6  197 │
                                     │ 289  205   59   11   87  254  161 │
@@ -279,14 +288,37 @@
                                     │  44  135   79   72   38   58   85 │
                                     │ 103  283  115   81  278  216   78 │
                                     │  22  268  122  270  228  121  175 │
                                     │  96  167   31   18   33  279   94 │
                                     │  51  107  159  272  265  258  251 │
                                     │  99  155   45  273  266  259  252 │
                                     └───────────────────────────────────┘
+⬛⬛⬛⬛⬛⬛⬛ 🟨🟩🟨🟧🟩🟪🟦
+⬛⬛⬛⬛⬛⬛⬛ 🟨🟦🟧🟪🟧🟨🟥
+⬛⬛⬛⬛⬛⬛⬛ 🟧🟥🟦🟪🟧🟩🟩
+⬛⬛⬛⬛⬛⬛⬛ 🟪🟥🟨🟪🟦🟩🟨
+⬛⬛⬛⬛⬛⬛⬛ 🟨🟩🟨🟥🟦🟨🟦
+⬛⬛⬛⬛⬛⬛⬛ 🟥🟧🟦🟪🟪🟪🟨
+⬛⬛⬛⬛⬛⬛⬛ 🟧🟩🟧🟪🟦🟪🟥
+
+🟥🟦🟪🟩🟩🟨🟨 🟩🟪🟩🟦🟧🟦🟪 🟩🟧🟥🟧🟥🟦🟪 🟥🟦🟧🟦🟦🟧🟦 
+🟩🟦🟧🟧🟩🟨🟨 🟧🟪🟪🟧🟧🟧🟨 🟦🟦🟧🟥🟩🟨🟨 🟩🟪🟩🟩🟥🟥🟥 
+🟩🟦🟥🟧🟩🟩🟧 🟪🟩🟦🟪🟧🟦🟪 🟦🟧🟥🟥🟧🟨🟦 🟪🟧🟨🟦🟥🟥🟥 
+🟨🟦🟨🟧🟧🟨🟪 🟥🟥🟥🟩🟧🟦🟩 🟧🟧🟦🟥🟨🟥🟨 🟩🟪🟩🟦🟩🟦🟦 
+🟦🟦🟥🟩🟦🟩🟥 🟪🟪🟪🟪🟨🟦🟥 🟦🟦🟩🟥🟪🟥🟨 🟩🟪🟩🟨🟧🟪🟨 
+🟪🟥🟨🟩🟥🟩🟩 🟧🟪🟪🟪🟨🟧🟧 🟦🟩🟪🟨🟥🟥🟥 🟦🟥🟦🟦🟨🟦🟥 
+🟪🟪🟨🟧🟪🟩🟧 🟦🟪🟪🟩🟥🟪🟨 🟦🟦🟦🟦🟨🟩🟩 🟥🟥🟥🟥🟩🟩🟧 
+
+⬛⬛⬛⬛⬛⬛⬛ 🟪🟥🟥🟥🟨🟧🟧
+⬛⬛⬛⬛⬛⬛⬛ 🟪🟩🟧🟧🟪🟧🟧
+⬛⬛⬛⬛⬛⬛⬛ 🟩🟨🟩🟧🟨🟦🟧
+⬛⬛⬛⬛⬛⬛⬛ 🟪🟨🟩🟨🟦🟩🟥
+⬛⬛⬛⬛⬛⬛⬛ 🟧🟥🟪🟪🟪🟨🟧
+⬛⬛⬛⬛⬛⬛⬛ 🟧🟩🟥🟨🟨🟨🟨
+⬛⬛⬛⬛⬛⬛⬛ 🟩🟥🟪🟨🟨🟨🟨
 ```
 
 # Solving
 Only Rubik's cube and Pocket cube can be solved. Cubes are solved with Herbert Kociemba's algorithm.
 ```
 print(rubiks_cube.scramble())
 rubiks_cube.show()
```

### Comparing `super_rubik_cube-1.0.2/super_rubik_cube.egg-info/SOURCES.txt` & `super_rubik_cube-1.0.3/super_rubik_cube.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/.cornerprun` & `super_rubik_cube-1.0.3/supercube/.cornerprun`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/.move_cornperm` & `super_rubik_cube-1.0.3/supercube/.move_cornperm`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/PocketCube.py` & `super_rubik_cube-1.0.3/supercube/PocketCube.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/RubiksCube.py` & `super_rubik_cube-1.0.3/supercube/RubiksCube.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/cube.py` & `super_rubik_cube-1.0.3/supercube/cube.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/kociemba/__init__.py` & `super_rubik_cube-1.0.3/supercube/kociemba/__init__.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/kociemba/build_ckociemba.py` & `super_rubik_cube-1.0.3/supercube/kociemba/build_ckociemba.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/coordcube.py` & `super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/coordcube.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/corner.py` & `super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/corner.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/cubiecube.py` & `super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/cubiecube.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/edge.py` & `super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/edge.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/facecube.py` & `super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/facecube.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/facelet.py` & `super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/facelet.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/FRtoBR_Move.pkl` & `super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/prunetables/FRtoBR_Move.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/MergeURtoULandUBtoDF.pkl` & `super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/prunetables/MergeURtoULandUBtoDF.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/Slice_Flip_Prun.pkl` & `super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/prunetables/Slice_Flip_Prun.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/Slice_Twist_Prun.pkl` & `super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/prunetables/Slice_Twist_Prun.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/Slice_URFtoDLF_Parity_Prun.pkl` & `super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/prunetables/Slice_URFtoDLF_Parity_Prun.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/Slice_URtoDF_Parity_Prun.pkl` & `super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/prunetables/Slice_URtoDF_Parity_Prun.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/UBtoDF_Move.pkl` & `super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/prunetables/UBtoDF_Move.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/URFtoDLF_Move.pkl` & `super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/prunetables/URFtoDLF_Move.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/URtoDF_Move.pkl` & `super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/prunetables/URtoDF_Move.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/URtoUL_Move.pkl` & `super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/prunetables/URtoUL_Move.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/flipMove.pkl` & `super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/prunetables/flipMove.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/twistMove.pkl` & `super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/prunetables/twistMove.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/search.py` & `super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/search.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/tools.py` & `super_rubik_cube-1.0.3/supercube/kociemba/pykociemba/tools.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/kociemba_2x2/client_gui.py` & `super_rubik_cube-1.0.3/supercube/kociemba_2x2/client_gui.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/kociemba_2x2/coord.py` & `super_rubik_cube-1.0.3/supercube/kociemba_2x2/coord.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/kociemba_2x2/cubie.py` & `super_rubik_cube-1.0.3/supercube/kociemba_2x2/cubie.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/kociemba_2x2/defs.py` & `super_rubik_cube-1.0.3/supercube/kociemba_2x2/defs.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/kociemba_2x2/enums.py` & `super_rubik_cube-1.0.3/supercube/kociemba_2x2/enums.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/kociemba_2x2/example.py` & `super_rubik_cube-1.0.3/supercube/kociemba_2x2/example.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/kociemba_2x2/face.py` & `super_rubik_cube-1.0.3/supercube/kociemba_2x2/face.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/kociemba_2x2/moves.py` & `super_rubik_cube-1.0.3/supercube/kociemba_2x2/moves.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/kociemba_2x2/pruning.py` & `super_rubik_cube-1.0.3/supercube/kociemba_2x2/pruning.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/kociemba_2x2/sockets.py` & `super_rubik_cube-1.0.3/supercube/kociemba_2x2/sockets.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.2/supercube/kociemba_2x2/solver.py` & `super_rubik_cube-1.0.3/supercube/kociemba_2x2/solver.py`

 * *Files identical despite different names*

