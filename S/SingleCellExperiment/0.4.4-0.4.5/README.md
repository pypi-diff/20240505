# Comparing `tmp/SingleCellExperiment-0.4.4.tar.gz` & `tmp/singlecellexperiment-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SingleCellExperiment-0.4.4.tar", last modified: Wed Feb 14 16:41:52 2024, max compression
+gzip compressed data, was "singlecellexperiment-0.4.5.tar", last modified: Sun May  5 19:44:05 2024, max compression
```

## Comparing `SingleCellExperiment-0.4.4.tar` & `singlecellexperiment-0.4.5.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 16:41:52.847895 SingleCellExperiment-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 16:41:52.831895 SingleCellExperiment-0.4.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 16:41:52.835895 SingleCellExperiment-0.4.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13646 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-02-14 16:41:52.847895 SingleCellExperiment-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 16:41:52.839895 SingleCellExperiment-0.4.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 16:41:52.839895 SingleCellExperiment-0.4.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    10523 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/docs/tutorial.md
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-02-14 16:41:52.851895 SingleCellExperiment-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 16:41:52.831895 SingleCellExperiment-0.4.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 16:41:52.847895 SingleCellExperiment-0.4.4/src/SingleCellExperiment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-02-14 16:41:52.000000 SingleCellExperiment-0.4.4/src/SingleCellExperiment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-02-14 16:41:52.000000 SingleCellExperiment-0.4.4/src/SingleCellExperiment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 16:41:52.000000 SingleCellExperiment-0.4.4/src/SingleCellExperiment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 16:40:48.000000 SingleCellExperiment-0.4.4/src/SingleCellExperiment.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-02-14 16:41:52.000000 SingleCellExperiment-0.4.4/src/SingleCellExperiment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-14 16:41:52.000000 SingleCellExperiment-0.4.4/src/SingleCellExperiment.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 16:41:52.843895 SingleCellExperiment-0.4.4/src/singlecellexperiment/
--rw-r--r--   0 runner    (1001) docker     (127)    45334 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/src/singlecellexperiment/SingleCellExperiment.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/src/singlecellexperiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/src/singlecellexperiment/_combineutils.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/src/singlecellexperiment/_ioutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 16:41:52.843895 SingleCellExperiment-0.4.4/src/singlecellexperiment/io/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/src/singlecellexperiment/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/src/singlecellexperiment/io/h5ad.py
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/src/singlecellexperiment/io/tenx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 16:41:52.843895 SingleCellExperiment-0.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 16:41:52.847895 SingleCellExperiment-0.4.4/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)   311344 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/tests/data/adata.h5ad
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/tests/data/mocks.py
--rw-r--r--   0 runner    (1001) docker     (127)   986863 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/tests/data/tenx.sub.h5
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/tests/test_sce.py
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/tests/test_sce_combine_cols.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/tests/test_sce_combine_rows.py
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/tests/test_sce_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/tests/test_sce_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/tests/test_sce_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-02-14 16:40:38.000000 SingleCellExperiment-0.4.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:44:05.079266 singlecellexperiment-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:44:05.067266 singlecellexperiment-0.4.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:44:05.071266 singlecellexperiment-0.4.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13646 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-05 19:44:05.079266 singlecellexperiment-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:44:05.071266 singlecellexperiment-0.4.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:44:05.071266 singlecellexperiment-0.4.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10523 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/docs/tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-05 19:44:05.079266 singlecellexperiment-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:44:05.067266 singlecellexperiment-0.4.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:44:05.079266 singlecellexperiment-0.4.5/src/SingleCellExperiment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-05 19:44:05.000000 singlecellexperiment-0.4.5/src/SingleCellExperiment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-05 19:44:05.000000 singlecellexperiment-0.4.5/src/SingleCellExperiment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 19:44:05.000000 singlecellexperiment-0.4.5/src/SingleCellExperiment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 19:43:00.000000 singlecellexperiment-0.4.5/src/SingleCellExperiment.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-05 19:44:05.000000 singlecellexperiment-0.4.5/src/SingleCellExperiment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-05 19:44:05.000000 singlecellexperiment-0.4.5/src/SingleCellExperiment.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:44:05.075266 singlecellexperiment-0.4.5/src/singlecellexperiment/
+-rw-r--r--   0 runner    (1001) docker     (127)    45569 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/src/singlecellexperiment/SingleCellExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/src/singlecellexperiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/src/singlecellexperiment/_combineutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/src/singlecellexperiment/_ioutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:44:05.075266 singlecellexperiment-0.4.5/src/singlecellexperiment/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/src/singlecellexperiment/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/src/singlecellexperiment/io/h5ad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/src/singlecellexperiment/io/tenx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:44:05.075266 singlecellexperiment-0.4.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:44:05.075266 singlecellexperiment-0.4.5/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   311344 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/tests/data/adata.h5ad
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/tests/data/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)   986863 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/tests/data/tenx.sub.h5
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/tests/test_sce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/tests/test_sce_combine_cols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/tests/test_sce_combine_rows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/tests/test_sce_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/tests/test_sce_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/tests/test_sce_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-05 19:42:51.000000 singlecellexperiment-0.4.5/tox.ini
```

### Comparing `SingleCellExperiment-0.4.4/.coveragerc` & `singlecellexperiment-0.4.5/.coveragerc`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.4.4/.github/workflows/pypi-publish.yml` & `singlecellexperiment-0.4.5/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.4.4/.github/workflows/pypi-test.yml` & `singlecellexperiment-0.4.5/.github/workflows/pypi-test.yml`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.4.4/.gitignore` & `singlecellexperiment-0.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.4.4/.pre-commit-config.yaml` & `singlecellexperiment-0.4.5/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 exclude: '^docs/conf.py'
 
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.5.0
+  rev: v4.6.0
   hooks:
   - id: trailing-whitespace
   - id: check-added-large-files
   - id: check-ast
   - id: check-json
   - id: check-merge-conflict
   - id: check-xml
@@ -22,22 +22,22 @@
   hooks:
     - id: docformatter
       additional_dependencies: [tomli]
       args: [--in-place, --wrap-descriptions=120, --wrap-summaries=120]
       # --config, ./pyproject.toml
 
 - repo: https://github.com/psf/black
-  rev: 24.1.1
+  rev: 24.4.0
   hooks:
   - id: black
     language_version: python3
 
 - repo: https://github.com/astral-sh/ruff-pre-commit
   # Ruff version.
-  rev: v0.2.1
+  rev: v0.3.7
   hooks:
     - id: ruff
       args: [--fix, --exit-non-zero-on-fix]
 
 ## If like to embrace black styles even in the docs:
 # - repo: https://github.com/asottile/blacken-docs
 #   rev: v1.13.0
```

### Comparing `SingleCellExperiment-0.4.4/CHANGELOG.md` & `singlecellexperiment-0.4.5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.4.4/CONTRIBUTING.md` & `singlecellexperiment-0.4.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.4.4/LICENSE.txt` & `singlecellexperiment-0.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.4.4/PKG-INFO` & `singlecellexperiment-0.4.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SingleCellExperiment
-Version: 0.4.4
+Version: 0.4.5
 Summary: Container class for single-cell experiments
 Home-page: https://github.com/BiocPy/SingleCellExperiment
 Author: jkanche
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/BiocPy/SingleCellExperiment
 Platform: any
@@ -16,22 +16,24 @@
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Requires-Dist: summarizedexperiment<0.5.0,>=0.4.0
 Provides-Extra: optional
 Requires-Dist: anndata; extra == "optional"
 Requires-Dist: h5py; extra == "optional"
 Requires-Dist: mudata; extra == "optional"
 Requires-Dist: delayedarray; extra == "optional"
+Requires-Dist: hdf5array; extra == "optional"
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: anndata; extra == "testing"
 Requires-Dist: h5py; extra == "testing"
 Requires-Dist: mudata; extra == "testing"
 Requires-Dist: delayedarray; extra == "testing"
+Requires-Dist: hdf5array; extra == "testing"
 
 [![Project generated with PyScaffold](https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold)](https://pyscaffold.org/)
 [![PyPI-Server](https://img.shields.io/pypi/v/SingleCellExperiment.svg)](https://pypi.org/project/SingleCellExperiment/)
 ![Unit tests](https://github.com/BiocPy/SingleCellExperiment/actions/workflows/pypi-test.yml/badge.svg)
 
 # SingleCellExperiment
```

### Comparing `SingleCellExperiment-0.4.4/README.md` & `singlecellexperiment-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.4.4/docs/Makefile` & `singlecellexperiment-0.4.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.4.4/docs/changelog.md` & `singlecellexperiment-0.4.5/docs/changelog.md`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.4.4/docs/conf.py` & `singlecellexperiment-0.4.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.4.4/docs/index.md` & `singlecellexperiment-0.4.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.4.4/docs/readme.md` & `singlecellexperiment-0.4.5/docs/readme.md`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.4.4/docs/tutorial.md` & `singlecellexperiment-0.4.5/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.4.4/pyproject.toml` & `singlecellexperiment-0.4.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.4.4/setup.cfg` & `singlecellexperiment-0.4.5/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -33,22 +33,24 @@
 
 [options.extras_require]
 optional = 
 	anndata
 	h5py
 	mudata
 	delayedarray
+	hdf5array
 testing = 
 	setuptools
 	pytest
 	pytest-cov
 	anndata
 	h5py
 	mudata
 	delayedarray
+	hdf5array
 
 [options.entry_points]
 
 [tool:pytest]
 addopts = 
 	--cov singlecellexperiment --cov-report term-missing
 	--verbose
```

### Comparing `SingleCellExperiment-0.4.4/setup.py` & `singlecellexperiment-0.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.4.4/src/SingleCellExperiment.egg-info/PKG-INFO` & `singlecellexperiment-0.4.5/src/SingleCellExperiment.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SingleCellExperiment
-Version: 0.4.4
+Version: 0.4.5
 Summary: Container class for single-cell experiments
 Home-page: https://github.com/BiocPy/SingleCellExperiment
 Author: jkanche
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/BiocPy/SingleCellExperiment
 Platform: any
@@ -16,22 +16,24 @@
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Requires-Dist: summarizedexperiment<0.5.0,>=0.4.0
 Provides-Extra: optional
 Requires-Dist: anndata; extra == "optional"
 Requires-Dist: h5py; extra == "optional"
 Requires-Dist: mudata; extra == "optional"
 Requires-Dist: delayedarray; extra == "optional"
+Requires-Dist: hdf5array; extra == "optional"
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: anndata; extra == "testing"
 Requires-Dist: h5py; extra == "testing"
 Requires-Dist: mudata; extra == "testing"
 Requires-Dist: delayedarray; extra == "testing"
+Requires-Dist: hdf5array; extra == "testing"
 
 [![Project generated with PyScaffold](https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold)](https://pyscaffold.org/)
 [![PyPI-Server](https://img.shields.io/pypi/v/SingleCellExperiment.svg)](https://pypi.org/project/SingleCellExperiment/)
 ![Unit tests](https://github.com/BiocPy/SingleCellExperiment/actions/workflows/pypi-test.yml/badge.svg)
 
 # SingleCellExperiment
```

### Comparing `SingleCellExperiment-0.4.4/src/SingleCellExperiment.egg-info/SOURCES.txt` & `singlecellexperiment-0.4.5/src/SingleCellExperiment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.4.4/src/singlecellexperiment/SingleCellExperiment.py` & `singlecellexperiment-0.4.5/src/singlecellexperiment/SingleCellExperiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1011,33 +1011,36 @@
         """Create a ``SingleCellExperiment`` from :py:class:`~anndata.AnnData`.
 
          Args:
             input:
                 Input data.
 
         Returns:
-            A ``SingleCellExperiment`` object.
+            A ``SingleCellExperiment`` object. If the input contains any data
+            in the ``uns`` attribute, the `metadata` slot of the ``SingleCellExperiment``
+            will contain a key ``uns``.
         """
 
         layers = OrderedDict()
         for asy, mat in input.layers.items():
             layers[asy] = mat.transpose()
 
         if input.X is not None:
             layers["X"] = input.X.transpose()
 
         obsm = _to_normal_dict(input.obsm)
         varp = _to_normal_dict(input.varp)
         obsp = _to_normal_dict(input.obsp)
+        _metadata = {"uns": input.uns} if input.uns is not None else None
 
         return cls(
             assays=layers,
             row_data=biocframe.BiocFrame.from_pandas(input.var),
             column_data=biocframe.BiocFrame.from_pandas(input.obs),
-            metadata=input.uns,
+            metadata=_metadata,
             reduced_dims=obsm,
             row_pairs=varp,
             column_pairs=obsp,
         )
 
     ###############################
     ######>> MuData interop <<#####
```

### Comparing `SingleCellExperiment-0.4.4/src/singlecellexperiment/__init__.py` & `singlecellexperiment-0.4.5/src/singlecellexperiment/__init__.py`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.4.4/src/singlecellexperiment/_combineutils.py` & `singlecellexperiment-0.4.5/src/singlecellexperiment/_combineutils.py`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.4.4/src/singlecellexperiment/io/tenx.py` & `singlecellexperiment-0.4.5/src/singlecellexperiment/io/tenx.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,34 +54,29 @@
             Path to 10x H5 file.
 
     Returns:
         A single-cell experiment object.
     """
 
     import h5py
-    from scipy.sparse import csc_matrix, csr_matrix
+    from hdf5array import Hdf5CompressedSparseMatrix
 
     h5 = h5py.File(path, mode="r")
 
     if "matrix" not in h5.keys():
         raise ValueError(f"H5 file ({path}) is not a 10X V3 format.")
 
     groups = h5["matrix"].keys()
 
     # read the matrix
-    data = h5["matrix"]["data"][:]
-    indices = h5["matrix"]["indices"][:]
-    indptr = h5["matrix"]["indptr"][:]
     shape = tuple(h5["matrix"]["shape"][:])
 
-    counts = None
-    if len(indptr) == shape[1] + 1:
-        counts = csc_matrix((data, indices, indptr), shape=shape)
-    else:
-        counts = csr_matrix((data, indices, indptr), shape=shape)
+    counts = Hdf5CompressedSparseMatrix(
+        path=path, group_name="matrix", by_column=True, shape=shape
+    )
 
     # read features
     features = None
     ignore_list = []
     if "features" in groups:
         features = {}
         for key, val in h5["matrix"]["features"].items():
@@ -102,10 +97,12 @@
 
     barcodes = None
     if "barcodes" in groups:
         barcodes = {}
         barcodes["barcodes"] = [x.decode("ascii") for x in h5["matrix"]["barcodes"]]
         barcodes = BiocFrame(barcodes, number_of_rows=counts.shape[1])
 
+    h5.close()
+
     return SingleCellExperiment(
         assays={"counts": counts}, row_data=features, column_data=barcodes
     )
```

### Comparing `SingleCellExperiment-0.4.4/tests/data/adata.h5ad` & `singlecellexperiment-0.4.5/tests/data/adata.h5ad`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.4.4/tests/data/mocks.py` & `singlecellexperiment-0.4.5/tests/data/mocks.py`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.4.4/tests/data/tenx.sub.h5` & `singlecellexperiment-0.4.5/tests/data/tenx.sub.h5`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.4.4/tests/test_sce.py` & `singlecellexperiment-0.4.5/tests/test_sce.py`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.4.4/tests/test_sce_combine_cols.py` & `singlecellexperiment-0.4.5/tests/test_sce_combine_cols.py`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.4.4/tests/test_sce_combine_rows.py` & `singlecellexperiment-0.4.5/tests/test_sce_combine_rows.py`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.4.4/tests/test_sce_io.py` & `singlecellexperiment-0.4.5/tests/test_sce_io.py`

 * *Files 14% similar despite different names*

```diff
@@ -125,14 +125,22 @@
     adata.var_names = [f"var_{j+1}" for j in range(d)]
 
     tse = singlecellexperiment.SingleCellExperiment.from_anndata(adata)
 
     assert tse is not None
     assert isinstance(tse, SingleCellExperiment)
 
+    # to avoid unknown mapping types;
+    # ran into an issue with anndata.compat._overloaded_dict.OverloadedDict when loading a h5ad
+    adata.uns = {".internal": [f"obs_{i+1}" for i in range(n)]}
+    tse = singlecellexperiment.SingleCellExperiment.from_anndata(adata)
+
+    assert tse is not None
+    assert isinstance(tse, SingleCellExperiment)
+
 
 def test_SCE_to_mudata():
     tse = SingleCellExperiment(
         assays={"counts": counts}, row_data=row_data, column_data=col_data
     )
 
     assert tse is not None
```

### Comparing `SingleCellExperiment-0.4.4/tests/test_sce_methods.py` & `singlecellexperiment-0.4.5/tests/test_sce_methods.py`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.4.4/tests/test_sce_slice.py` & `singlecellexperiment-0.4.5/tests/test_sce_slice.py`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.4.4/tox.ini` & `singlecellexperiment-0.4.5/tox.ini`

 * *Files identical despite different names*

