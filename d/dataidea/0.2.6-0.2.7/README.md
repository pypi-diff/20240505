# Comparing `tmp/dataidea-0.2.6.tar.gz` & `tmp/dataidea-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataidea-0.2.6.tar", max compression
+gzip compressed data, was "dataidea-0.2.7.tar", last modified: Sun May  5 13:15:15 2024, max compression
```

## Comparing `dataidea-0.2.6.tar` & `dataidea-0.2.7.tar`

### file list

```diff
@@ -1,19 +1,22 @@
--rw-r--r--   0        0        0     7496 2024-04-21 19:53:53.642815 dataidea-0.2.6/README.md
--rw-r--r--   0        0        0      202 2024-04-27 09:53:08.511903 dataidea-0.2.6/dataidea/__init__.py
--rw-r--r--   0        0        0      229 2024-04-19 06:31:05.013813 dataidea-0.2.6/dataidea/datasets/cluster.csv
--rw-r--r--   0        0        0     4645 2024-04-19 06:33:56.213774 dataidea-0.2.6/dataidea/datasets/demo.csv
--rw-r--r--   0        0        0    47391 2024-04-19 06:31:05.017817 dataidea-0.2.6/dataidea/datasets/fpl.csv
--rw-r--r--   0        0        0      370 2024-04-19 06:31:05.021821 dataidea-0.2.6/dataidea/datasets/homeprices.csv
--rw-r--r--   0        0        0     3780 2024-04-27 09:00:34.018881 dataidea-0.2.6/dataidea/datasets/mall.csv
--rw-r--r--   0        0        0  2091239 2024-04-19 06:31:05.025825 dataidea-0.2.6/dataidea/datasets/melbourne.csv
--rw-r--r--   0        0        0      302 2024-04-19 06:31:05.029829 dataidea-0.2.6/dataidea/datasets/music.csv
--rw-r--r--   0        0        0      656 2024-04-19 06:31:05.029829 dataidea-0.2.6/dataidea/datasets/salaries.csv
--rw-r--r--   0        0        0    41983 2024-04-27 09:39:55.284672 dataidea-0.2.6/dataidea/datasets/student-mat.csv
--rw-r--r--   0        0        0    68558 2024-04-27 09:39:44.916354 dataidea-0.2.6/dataidea/datasets/student-por.csv
--rw-r--r--   0        0        0   108285 2024-04-19 06:31:05.029829 dataidea-0.2.6/dataidea/datasets/titanic.csv
--rw-r--r--   0        0        0  1355781 2024-04-19 06:31:05.033833 dataidea-0.2.6/dataidea/datasets/vgsales.csv
--rw-r--r--   0        0        0      217 2024-04-19 06:31:05.033833 dataidea-0.2.6/dataidea/datasets/weather.csv
--rw-r--r--   0        0        0     1030 2024-04-27 09:51:24.344571 dataidea-0.2.6/dataidea/datasets.py
--rw-r--r--   0        0        0      167 2024-04-27 09:39:06.489400 dataidea-0.2.6/dataidea/packages.py
--rw-r--r--   0        0        0      481 2024-04-27 09:44:14.426101 dataidea-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     8295 1970-01-01 00:00:00.000000 dataidea-0.2.6/PKG-INFO
+drwxrwxr-x   0 jumashafara  (1000) jumashafara  (1000)        0 2024-05-05 13:15:15.255330 dataidea-0.2.7/
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)    11337 2024-04-25 15:06:39.000000 dataidea-0.2.7/LICENSE
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)      111 2024-04-25 15:06:39.000000 dataidea-0.2.7/MANIFEST.in
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     2864 2024-05-05 13:15:15.255330 dataidea-0.2.7/PKG-INFO
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     2009 2024-04-30 16:38:32.000000 dataidea-0.2.7/README.md
+drwxrwxr-x   0 jumashafara  (1000) jumashafara  (1000)        0 2024-05-05 13:15:15.255330 dataidea-0.2.7/dataidea/
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)       22 2024-05-05 12:50:45.000000 dataidea-0.2.7/dataidea/__init__.py
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)      417 2024-05-03 14:28:07.000000 dataidea-0.2.7/dataidea/_modidx.py
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)      142 2024-04-25 15:06:39.000000 dataidea-0.2.7/dataidea/core.py
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     1030 2024-04-27 09:51:24.000000 dataidea-0.2.7/dataidea/datasets.py
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)      167 2024-04-27 09:39:06.000000 dataidea-0.2.7/dataidea/packages.py
+drwxrwxr-x   0 jumashafara  (1000) jumashafara  (1000)        0 2024-05-05 13:15:15.255330 dataidea-0.2.7/dataidea.egg-info/
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     2864 2024-05-05 13:15:15.000000 dataidea-0.2.7/dataidea.egg-info/PKG-INFO
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)      376 2024-05-05 13:15:15.000000 dataidea-0.2.7/dataidea.egg-info/SOURCES.txt
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)        1 2024-05-05 13:15:15.000000 dataidea-0.2.7/dataidea.egg-info/dependency_links.txt
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)       59 2024-05-05 13:15:15.000000 dataidea-0.2.7/dataidea.egg-info/entry_points.txt
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)        1 2024-05-05 12:55:26.000000 dataidea-0.2.7/dataidea.egg-info/not-zip-safe
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)        7 2024-05-05 13:15:15.000000 dataidea-0.2.7/dataidea.egg-info/requires.txt
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)        9 2024-05-05 13:15:15.000000 dataidea-0.2.7/dataidea.egg-info/top_level.txt
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     1093 2024-05-05 12:57:47.000000 dataidea-0.2.7/settings.ini
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)       38 2024-05-05 13:15:15.255330 dataidea-0.2.7/setup.cfg
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     2596 2024-04-25 15:06:39.000000 dataidea-0.2.7/setup.py
```

### Comparing `dataidea-0.2.6/dataidea/datasets.py` & `dataidea-0.2.7/dataidea/datasets.py`

 * *Files identical despite different names*

