# Comparing `tmp/thebeans-0.0.8.tar.gz` & `tmp/thebeans-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thebeans-0.0.8.tar", last modified: Fri Apr 26 15:55:38 2024, max compression
+gzip compressed data, was "thebeans-0.1.0.tar", last modified: Sun May  5 17:06:32 2024, max compression
```

## Comparing `thebeans-0.0.8.tar` & `thebeans-0.1.0.tar`

### file list

```diff
@@ -1,74 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:38.950176 thebeans-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-26 15:55:28.000000 thebeans-0.0.8/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:38.938176 thebeans-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:38.938176 thebeans-0.0.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-26 15:55:28.000000 thebeans-0.0.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-26 15:55:28.000000 thebeans-0.0.8/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-26 15:55:28.000000 thebeans-0.0.8/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:38.942176 thebeans-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-26 15:55:28.000000 thebeans-0.0.8/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-26 15:55:28.000000 thebeans-0.0.8/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-26 15:55:28.000000 thebeans-0.0.8/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-26 15:55:28.000000 thebeans-0.0.8/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-26 15:55:28.000000 thebeans-0.0.8/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-26 15:55:28.000000 thebeans-0.0.8/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-26 15:55:28.000000 thebeans-0.0.8/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-26 15:55:28.000000 thebeans-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:55:28.000000 thebeans-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-26 15:55:28.000000 thebeans-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-26 15:55:38.950176 thebeans-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-26 15:55:28.000000 thebeans-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:38.950176 thebeans-0.0.8/TheBeans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-26 15:55:38.000000 thebeans-0.0.8/TheBeans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-26 15:55:38.000000 thebeans-0.0.8/TheBeans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:55:38.000000 thebeans-0.0.8/TheBeans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-26 15:55:38.000000 thebeans-0.0.8/TheBeans.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-26 15:55:38.000000 thebeans-0.0.8/TheBeans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 15:55:38.000000 thebeans-0.0.8/TheBeans.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:38.942176 thebeans-0.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/CSVtoDF.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:38.942176 thebeans-0.0.8/docs/Labs/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/Labs/_cats_.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/Labs/_dogs_.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/Labs/broken_dogs_.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/Labs/guestbook.txt
--rw-r--r--   0 runner    (1001) docker     (127)    33576 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/Labs/lab4.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    42912 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/Labs/lab5.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/Labs/learning_python.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/Labs/name.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/Labs/reasons.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:38.946176 thebeans-0.0.8/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    12416 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/examples/ExampleBeans.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/examples/Lab9_Toolbar.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/examples/StudyArea.geojson
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/examples/csv.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   117900 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/examples/europe_110.geo.json
--rw-r--r--   0 runner    (1001) docker     (127)     7330 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/examples/folium.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/examples/quickstart.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/examples/raster.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   207731 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/examples/us_regions.geojson
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/examples/vector.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:38.946176 thebeans-0.0.8/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/thebeans.md
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-26 15:55:28.000000 thebeans-0.0.8/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-26 15:55:28.000000 thebeans-0.0.8/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-26 15:55:28.000000 thebeans-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-26 15:55:28.000000 thebeans-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-26 15:55:28.000000 thebeans-0.0.8/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:55:38.950176 thebeans-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:38.946176 thebeans-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:55:28.000000 thebeans-0.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-26 15:55:28.000000 thebeans-0.0.8/tests/test_thebeans.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:38.946176 thebeans-0.0.8/thebeans/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-26 15:55:28.000000 thebeans-0.0.8/thebeans/CSVtoDF.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-26 15:55:28.000000 thebeans-0.0.8/thebeans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-26 15:55:28.000000 thebeans-0.0.8/thebeans/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-26 15:55:28.000000 thebeans-0.0.8/thebeans/foliummap.py
--rw-r--r--   0 runner    (1001) docker     (127)    14476 2024-04-26 15:55:28.000000 thebeans-0.0.8/thebeans/thebeans.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:06:32.316897 thebeans-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-05 17:06:17.000000 thebeans-0.1.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:06:32.304896 thebeans-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:06:32.308896 thebeans-0.1.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-05 17:06:17.000000 thebeans-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-05 17:06:17.000000 thebeans-0.1.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-05 17:06:17.000000 thebeans-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:06:32.308896 thebeans-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-05 17:06:17.000000 thebeans-0.1.0/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-05 17:06:17.000000 thebeans-0.1.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-05 17:06:17.000000 thebeans-0.1.0/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-05 17:06:17.000000 thebeans-0.1.0/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-05 17:06:17.000000 thebeans-0.1.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-05 17:06:17.000000 thebeans-0.1.0/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-05 17:06:17.000000 thebeans-0.1.0/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-05 17:06:17.000000 thebeans-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 17:06:17.000000 thebeans-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-05 17:06:17.000000 thebeans-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-05 17:06:32.316897 thebeans-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-05 17:06:17.000000 thebeans-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:06:32.316897 thebeans-0.1.0/TheBeans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-05 17:06:32.000000 thebeans-0.1.0/TheBeans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-05 17:06:32.000000 thebeans-0.1.0/TheBeans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 17:06:32.000000 thebeans-0.1.0/TheBeans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-05 17:06:32.000000 thebeans-0.1.0/TheBeans.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-05 17:06:32.000000 thebeans-0.1.0/TheBeans.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-05 17:06:32.000000 thebeans-0.1.0/TheBeans.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:06:32.312897 thebeans-0.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-05 17:06:17.000000 thebeans-0.1.0/docs/CSVtoDF.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:06:32.312897 thebeans-0.1.0/docs/Labs/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 17:06:17.000000 thebeans-0.1.0/docs/Labs/_cats_.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-05 17:06:17.000000 thebeans-0.1.0/docs/Labs/_dogs_.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-05 17:06:17.000000 thebeans-0.1.0/docs/Labs/broken_dogs_.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-05 17:06:17.000000 thebeans-0.1.0/docs/Labs/guestbook.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    33576 2024-05-05 17:06:17.000000 thebeans-0.1.0/docs/Labs/lab4.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    42912 2024-05-05 17:06:17.000000 thebeans-0.1.0/docs/Labs/lab5.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-05 17:06:17.000000 thebeans-0.1.0/docs/Labs/learning_python.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-05 17:06:17.000000 thebeans-0.1.0/docs/Labs/name.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-05 17:06:17.000000 thebeans-0.1.0/docs/Labs/reasons.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-05 17:06:17.000000 thebeans-0.1.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-05 17:06:17.000000 thebeans-0.1.0/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-05 17:06:17.000000 thebeans-0.1.0/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:06:32.316897 thebeans-0.1.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    12416 2024-05-05 17:06:17.000000 thebeans-0.1.0/docs/examples/ExampleBeans.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    30998 2024-05-05 17:06:17.000000 thebeans-0.1.0/docs/examples/Lab9_Toolbar.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-05 17:06:17.000000 thebeans-0.1.0/docs/examples/StudyArea.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-05 17:06:17.000000 thebeans-0.1.0/docs/examples/StudyBox.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-05 17:06:17.000000 thebeans-0.1.0/docs/examples/csv.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   117900 2024-05-05 17:06:17.000000 thebeans-0.1.0/docs/examples/europe_110.geo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7330 2024-05-05 17:06:17.000000 thebeans-0.1.0/docs/examples/folium.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-05-05 17:06:17.000000 thebeans-0.1.0/docs/examples/pysheds.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11977 2024-05-05 17:06:17.000000 thebeans-0.1.0/docs/examples/quickstart.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-05 17:06:17.000000 thebeans-0.1.0/docs/examples/raster.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   207731 2024-05-05 17:06:17.000000 thebeans-0.1.0/docs/examples/us_regions.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-05 17:06:17.000000 thebeans-0.1.0/docs/examples/vector.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-05 17:06:17.000000 thebeans-0.1.0/docs/examples/whitebox.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-05 17:06:17.000000 thebeans-0.1.0/docs/faq.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:06:32.316897 thebeans-0.1.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   248956 2024-05-05 17:06:17.000000 thebeans-0.1.0/docs/images/TheBeans.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-05 17:06:17.000000 thebeans-0.1.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-05 17:06:17.000000 thebeans-0.1.0/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:06:32.316897 thebeans-0.1.0/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-05 17:06:17.000000 thebeans-0.1.0/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-05 17:06:17.000000 thebeans-0.1.0/docs/thebeans.md
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-05 17:06:17.000000 thebeans-0.1.0/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-05 17:06:17.000000 thebeans-0.1.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-05 17:06:17.000000 thebeans-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-05 17:06:17.000000 thebeans-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-05 17:06:17.000000 thebeans-0.1.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 17:06:32.316897 thebeans-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:06:32.316897 thebeans-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 17:06:17.000000 thebeans-0.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-05 17:06:17.000000 thebeans-0.1.0/tests/test_thebeans.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:06:32.316897 thebeans-0.1.0/thebeans/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-05 17:06:17.000000 thebeans-0.1.0/thebeans/CSVtoDF.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-05 17:06:17.000000 thebeans-0.1.0/thebeans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-05 17:06:17.000000 thebeans-0.1.0/thebeans/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-05 17:06:17.000000 thebeans-0.1.0/thebeans/foliummap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23788 2024-05-05 17:06:17.000000 thebeans-0.1.0/thebeans/thebeans.py
```

### Comparing `thebeans-0.0.8/.github/workflows/docs-build.yml` & `thebeans-0.1.0/.github/workflows/docs-build.yml`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                   gdalinfo --version
             - name: Install dependencies
               run: |
                   pip install --no-cache-dir Cython
                   pip install -r requirements.txt -r requirements_dev.txt
                   pip install .
             - name: Discover typos with codespell
-              run: codespell --skip="*.csv,*.geojson,*.json,*.js,*.html,*cff,*.pdf,./.git,*.txt" --ignore-words-list="aci,acount,hist"
+              run: codespell --skip="*pysheds.ipynb,*.csv,*.geojson,*.json,*.js,*.html,*cff,*.pdf,./.git,*.txt" --ignore-words-list="aci,acount,hist"
             - name: PKG-TEST
               run: |
                   python -m unittest discover tests/
             - name: Build docs
               run: |
                   mkdocs build
             # - name: Deploy to Netlify
```

### Comparing `thebeans-0.0.8/.github/workflows/docs.yml` & `thebeans-0.1.0/.github/workflows/docs.yml`

 * *Files 16% similar despite different names*

```diff
@@ -16,13 +16,13 @@
               run: |
                   python -m pip install --upgrade pip
                   pip install --user --no-cache-dir Cython
                   pip install --user -r requirements.txt -r requirements_dev.txt
                   pip install .
             - name: Discover typos with codespell
               run: |
-                  codespell --skip="*.csv,*.geojson,*.json,*.js,*.html,*cff,./.git" --ignore-words-list="aci,hist"
+                  codespell --skip="*pysheds.ipynb,*.csv,*.geojson,*.json,*.js,*.html,*cff,./.git" --ignore-words-list="aci,hist"
             - name: PKG-TEST
               run: |
                   python -m unittest discover tests/
             - run: mkdocs gh-deploy --force
```

### Comparing `thebeans-0.0.8/.github/workflows/installation.yml` & `thebeans-0.1.0/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `thebeans-0.0.8/.github/workflows/macos.yml` & `thebeans-0.1.0/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `thebeans-0.0.8/.github/workflows/pypi.yml` & `thebeans-0.1.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `thebeans-0.0.8/.github/workflows/ubuntu.yml` & `thebeans-0.1.0/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `thebeans-0.0.8/.github/workflows/windows.yml` & `thebeans-0.1.0/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `thebeans-0.0.8/.gitignore` & `thebeans-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `thebeans-0.0.8/TheBeans.egg-info/SOURCES.txt` & `thebeans-0.1.0/TheBeans.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -40,21 +40,25 @@
 docs/Labs/lab5.ipynb
 docs/Labs/learning_python.txt
 docs/Labs/name.txt
 docs/Labs/reasons.txt
 docs/examples/ExampleBeans.ipynb
 docs/examples/Lab9_Toolbar.ipynb
 docs/examples/StudyArea.geojson
+docs/examples/StudyBox.geojson
 docs/examples/csv.ipynb
 docs/examples/europe_110.geo.json
 docs/examples/folium.ipynb
+docs/examples/pysheds.ipynb
 docs/examples/quickstart.ipynb
 docs/examples/raster.ipynb
 docs/examples/us_regions.geojson
 docs/examples/vector.ipynb
+docs/examples/whitebox.ipynb
+docs/images/TheBeans.jpg
 docs/overrides/main.html
 tests/__init__.py
 tests/test_thebeans.py
 thebeans/CSVtoDF.py
 thebeans/__init__.py
 thebeans/common.py
 thebeans/foliummap.py
```

### Comparing `thebeans-0.0.8/docs/Labs/lab4.ipynb` & `thebeans-0.1.0/docs/Labs/lab4.ipynb`

 * *Files identical despite different names*

### Comparing `thebeans-0.0.8/docs/Labs/lab5.ipynb` & `thebeans-0.1.0/docs/Labs/lab5.ipynb`

 * *Files identical despite different names*

### Comparing `thebeans-0.0.8/docs/contributing.md` & `thebeans-0.1.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `thebeans-0.0.8/docs/examples/ExampleBeans.ipynb` & `thebeans-0.1.0/docs/examples/ExampleBeans.ipynb`

 * *Files identical despite different names*

### Comparing `thebeans-0.0.8/docs/examples/StudyArea.geojson` & `thebeans-0.1.0/docs/examples/StudyArea.geojson`

 * *Files identical despite different names*

### Comparing `thebeans-0.0.8/docs/examples/csv.ipynb` & `thebeans-0.1.0/docs/examples/csv.ipynb`

 * *Files identical despite different names*

### Comparing `thebeans-0.0.8/docs/examples/europe_110.geo.json` & `thebeans-0.1.0/docs/examples/europe_110.geo.json`

 * *Files identical despite different names*

### Comparing `thebeans-0.0.8/docs/examples/folium.ipynb` & `thebeans-0.1.0/docs/examples/folium.ipynb`

 * *Files identical despite different names*

### Comparing `thebeans-0.0.8/docs/examples/raster.ipynb` & `thebeans-0.1.0/docs/examples/raster.ipynb`

 * *Files identical despite different names*

### Comparing `thebeans-0.0.8/docs/examples/us_regions.geojson` & `thebeans-0.1.0/docs/examples/us_regions.geojson`

 * *Files identical despite different names*

### Comparing `thebeans-0.0.8/docs/examples/vector.ipynb` & `thebeans-0.1.0/docs/examples/vector.ipynb`

 * *Files identical despite different names*

### Comparing `thebeans-0.0.8/docs/installation.md` & `thebeans-0.1.0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `thebeans-0.0.8/mkdocs.yml` & `thebeans-0.1.0/mkdocs.yml`

 * *Files 11% similar despite different names*

```diff
@@ -39,18 +39,18 @@
     - git-revision-date-localized:
           enable_creation_date: true
           type: timeago
     # - pdf-export
     - mkdocs-jupyter:
           include_source: True
           ignore_h1_titles: True
-          execute: False
+          execute: false
           allow_errors: false
           ignore: ["conf.py"]
-          execute_ignore: ["*ignore.ipynb"]
+          execute_ignore: ["examples/pysheds.ipynb", "examples/folium.ipynb"]
           
 markdown_extensions:
     - admonition
     - abbr
     - attr_list
     - def_list
     - footnotes
@@ -72,20 +72,17 @@
     - Installation: installation.md
     - Usage: usage.md
     - Contributing: contributing.md
     - FAQ: faq.md
     - Changelog: changelog.md
     - Report Issues: https://github.com/phillipslucas/TheBeans/issues
     - Examples:
-        - examples/ExampleBeans.ipynb
         - examples/csv.ipynb
-        - examples/vector.ipynb
-        - examples/raster.ipynb
-        - examples/Lab9_Toolbar.ipynb
+        - examples/folium.ipynb
+        - examples/pysheds.ipynb
+        - examples/quickstart.ipynb
+
     - API Reference:
           - thebeans module: thebeans.md
           - common module: common.md
           - CSVtoDF module: CSVtoDF.md
-    - Labs:
-        - Labs/lab4.ipynb
-        - Labs/lab5.ipynb
```

### Comparing `thebeans-0.0.8/pyproject.toml` & `thebeans-0.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "TheBeans"
-version = "0.0.8"
+version = "0.1.0"
 dynamic = [
     "dependencies",
 ]
 description = "Python package with the beans."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.0.8"
+current_version = "0.1.0"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

### Comparing `thebeans-0.0.8/thebeans/foliummap.py` & `thebeans-0.1.0/thebeans/foliummap.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import folium
+import streamlit_folium
 from ipyleaflet import basemaps
 
 class Map(folium.Map):
     def __init__(self, center = [20,0], zoom = 2, **kwargs):
         super().__init__(location=center, zoom_start = zoom, **kwargs)
 
 
@@ -87,9 +88,30 @@
     def add_layer_control(self):
         """
         Adds a layer control to the map.
 
         Returns:
             None
         """
+    def add_raster(self, data, name="raster", zoom_to_layer=True, **kwargs):
+        """Adds a raster layer to the map.
+
+        Args:
+            data (str): The path to the raster file.
+            name (str, optional): The name of the layer. Defaults to "raster".
+        """
+        import localtileserver
+        
+        try:
+            from localtileserver import TileClient, get_folium_tile_layer
+        except ImportError:
+            raise ImportError("Please install the localtileserver package.")
+
+        client = TileClient(data)
+        layer = get_folium_tile_layer(client, name=name, **kwargs)
+        self.add(layer)
+
+        if zoom_to_layer:
+            self.center = client.center()
+            self.zoom = client.default_zoom
 
         folium.LayerControl().add_to(self)
```

