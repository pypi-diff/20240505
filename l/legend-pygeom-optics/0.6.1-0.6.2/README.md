# Comparing `tmp/legend_pygeom_optics-0.6.1.tar.gz` & `tmp/legend_pygeom_optics-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "legend_pygeom_optics-0.6.1.tar", last modified: Wed Feb  7 14:05:26 2024, max compression
+gzip compressed data, was "legend_pygeom_optics-0.6.2.tar", last modified: Sun May  5 12:46:21 2024, max compression
```

## Comparing `legend_pygeom_optics-0.6.1.tar` & `legend_pygeom_optics-0.6.2.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:05:26.764421 legend_pygeom_optics-0.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:05:26.756421 legend_pygeom_optics-0.6.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:05:26.756421 legend_pygeom_optics-0.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/.github/workflows/distribution.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    44217 2024-02-07 14:05:26.764421 legend_pygeom_optics-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:05:26.756421 legend_pygeom_optics-0.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:05:26.756421 legend_pygeom_optics-0.6.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/docs/source/.py_api_exclude
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:05:26.756421 legend_pygeom_optics-0.6.1/docs/source/exts/
--rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/docs/source/exts/optics_plot_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 14:05:26.764421 legend_pygeom_optics-0.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:05:26.752421 legend_pygeom_optics-0.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:05:26.764421 legend_pygeom_optics-0.6.1/src/legend_pygeom_optics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44217 2024-02-07 14:05:26.000000 legend_pygeom_optics-0.6.1/src/legend_pygeom_optics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-02-07 14:05:26.000000 legend_pygeom_optics-0.6.1/src/legend_pygeom_optics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 14:05:26.000000 legend_pygeom_optics-0.6.1/src/legend_pygeom_optics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 14:05:26.000000 legend_pygeom_optics-0.6.1/src/legend_pygeom_optics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-02-07 14:05:26.000000 legend_pygeom_optics-0.6.1/src/legend_pygeom_optics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-07 14:05:26.000000 legend_pygeom_optics-0.6.1/src/legend_pygeom_optics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:05:26.760421 legend_pygeom_optics-0.6.1/src/legendoptics/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/src/legendoptics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-07 14:05:26.000000 legend_pygeom_optics-0.6.1/src/legendoptics/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/src/legendoptics/copper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:05:26.764421 legend_pygeom_optics-0.6.1/src/legendoptics/data/
--rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/src/legendoptics/data/cu_reflectivity.dat
--rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/src/legendoptics/data/ge_reflectivity.dat
--rw-r--r--   0 runner    (1001) docker     (127)    38826 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/src/legendoptics/data/lar_emission_heindl2010.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/src/legendoptics/data/nylon_absorption.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/src/legendoptics/data/pen_abslength.dat
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/src/legendoptics/data/pen_wlscomponent.dat
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/src/legendoptics/data/psfibers_wlsabslength.dat
--rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/src/legendoptics/data/psfibers_wlscomponent.dat
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/src/legendoptics/data/si_rindex_imag.dat
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/src/legendoptics/data/si_rindex_real.dat
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/src/legendoptics/data/tetratex_reflectivity.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/src/legendoptics/data/tpb_polystyrene_wlscomponent.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/src/legendoptics/data/tpb_vm2000_wlscomponent.dat
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/src/legendoptics/data/tpb_wlsabslength.dat
--rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/src/legendoptics/fibers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/src/legendoptics/germanium.py
--rw-r--r--   0 runner    (1001) docker     (127)    15906 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/src/legendoptics/lar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/src/legendoptics/nylon.py
--rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/src/legendoptics/pen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/src/legendoptics/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/src/legendoptics/pyg4utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/src/legendoptics/silicon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/src/legendoptics/tetratex.py
--rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/src/legendoptics/tpb.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/src/legendoptics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:05:26.764421 legend_pygeom_optics-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/tests/test_data_file_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/tests/test_lar.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-02-07 14:05:05.000000 legend_pygeom_optics-0.6.1/tests/test_pyg4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:21.970514 legend_pygeom_optics-0.6.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:21.962514 legend_pygeom_optics-0.6.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:21.962514 legend_pygeom_optics-0.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/.github/workflows/distribution.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    44217 2024-05-05 12:46:21.970514 legend_pygeom_optics-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:21.962514 legend_pygeom_optics-0.6.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:21.962514 legend_pygeom_optics-0.6.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/docs/source/.py_api_exclude
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:21.962514 legend_pygeom_optics-0.6.2/docs/source/exts/
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/docs/source/exts/optics_plot_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 12:46:21.970514 legend_pygeom_optics-0.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:21.958514 legend_pygeom_optics-0.6.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:21.970514 legend_pygeom_optics-0.6.2/src/legend_pygeom_optics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44217 2024-05-05 12:46:21.000000 legend_pygeom_optics-0.6.2/src/legend_pygeom_optics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-05 12:46:21.000000 legend_pygeom_optics-0.6.2/src/legend_pygeom_optics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 12:46:21.000000 legend_pygeom_optics-0.6.2/src/legend_pygeom_optics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 12:46:21.000000 legend_pygeom_optics-0.6.2/src/legend_pygeom_optics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-05 12:46:21.000000 legend_pygeom_optics-0.6.2/src/legend_pygeom_optics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-05 12:46:21.000000 legend_pygeom_optics-0.6.2/src/legend_pygeom_optics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:21.966514 legend_pygeom_optics-0.6.2/src/legendoptics/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/src/legendoptics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-05 12:46:21.000000 legend_pygeom_optics-0.6.2/src/legendoptics/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/src/legendoptics/copper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:21.970514 legend_pygeom_optics-0.6.2/src/legendoptics/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/src/legendoptics/data/cu_reflectivity.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/src/legendoptics/data/ge_reflectivity.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    38826 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/src/legendoptics/data/lar_emission_heindl2010.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/src/legendoptics/data/nylon_absorption.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/src/legendoptics/data/pen_abslength.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/src/legendoptics/data/pen_wlscomponent.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/src/legendoptics/data/psfibers_wlsabslength.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/src/legendoptics/data/psfibers_wlscomponent.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/src/legendoptics/data/si_rindex_imag.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/src/legendoptics/data/si_rindex_real.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/src/legendoptics/data/tetratex_reflectivity.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/src/legendoptics/data/tpb_polystyrene_wlscomponent.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/src/legendoptics/data/tpb_vm2000_wlscomponent.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/src/legendoptics/data/tpb_wlsabslength.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/src/legendoptics/fibers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/src/legendoptics/germanium.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15906 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/src/legendoptics/lar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/src/legendoptics/nylon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/src/legendoptics/pen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/src/legendoptics/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/src/legendoptics/pyg4utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/src/legendoptics/silicon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/src/legendoptics/tetratex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/src/legendoptics/tpb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/src/legendoptics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:21.970514 legend_pygeom_optics-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/tests/test_data_file_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/tests/test_lar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-05 12:46:18.000000 legend_pygeom_optics-0.6.2/tests/test_pyg4.py
```

### Comparing `legend_pygeom_optics-0.6.1/.github/workflows/distribution.yml` & `legend_pygeom_optics-0.6.2/.github/workflows/distribution.yml`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/.github/workflows/main.yml` & `legend_pygeom_optics-0.6.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/.gitignore` & `legend_pygeom_optics-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/.pre-commit-config.yaml` & `legend_pygeom_optics-0.6.2/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -38,36 +38,36 @@
     rev: "v4.0.0-alpha.8"
     hooks:
       - id: prettier
         types_or: [yaml, markdown, json]
         args: [--prose-wrap=always]
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.2.1"
+    rev: "v0.3.4"
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
       - id: ruff-format
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: "v1.8.0"
+    rev: "v1.9.0"
     hooks:
       - id: mypy
         files: src|tests
         stages: [manual]
         additional_dependencies:
           - pytest
 
   - repo: https://github.com/codespell-project/codespell
     rev: "v2.2.6"
     hooks:
       - id: codespell
 
   - repo: https://github.com/shellcheck-py/shellcheck-py
-    rev: "v0.9.0.6"
+    rev: "v0.10.0.1"
     hooks:
       - id: shellcheck
 
   - repo: local
     hooks:
       - id: disallow-caps
         name: Disallow improper capitalization
@@ -77,12 +77,12 @@
 
   - repo: https://github.com/abravalheri/validate-pyproject
     rev: v0.16
     hooks:
       - id: validate-pyproject
 
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.28.0
+    rev: 0.28.1
     hooks:
       - id: check-dependabot
       - id: check-github-workflows
       - id: check-readthedocs
```

### Comparing `legend_pygeom_optics-0.6.1/LICENSE` & `legend_pygeom_optics-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/PKG-INFO` & `legend_pygeom_optics-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: legend_pygeom_optics
-Version: 0.6.1
+Version: 0.6.2
 Summary: Optical properties of the LEGEND experiment
 Author-email: Luigi Pertoldi <gipert@pm.me>, Manuel Huber <info@manuelhu.de>
 Maintainer: The LEGEND Collaboration
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `legend_pygeom_optics-0.6.1/README.md` & `legend_pygeom_optics-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/docs/source/conf.py` & `legend_pygeom_optics-0.6.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/docs/source/exts/optics_plot_extension.py` & `legend_pygeom_optics-0.6.2/docs/source/exts/optics_plot_extension.py`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/docs/source/index.rst` & `legend_pygeom_optics-0.6.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/pyproject.toml` & `legend_pygeom_optics-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/src/legend_pygeom_optics.egg-info/PKG-INFO` & `legend_pygeom_optics-0.6.2/src/legend_pygeom_optics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: legend_pygeom_optics
-Version: 0.6.1
+Version: 0.6.2
 Summary: Optical properties of the LEGEND experiment
 Author-email: Luigi Pertoldi <gipert@pm.me>, Manuel Huber <info@manuelhu.de>
 Maintainer: The LEGEND Collaboration
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `legend_pygeom_optics-0.6.1/src/legend_pygeom_optics.egg-info/SOURCES.txt` & `legend_pygeom_optics-0.6.2/src/legend_pygeom_optics.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yaml
+CITATION.cff
 LICENSE
 README.md
 codecov.yml
 pyproject.toml
 .github/dependabot.yml
 .github/workflows/distribution.yml
 .github/workflows/main.yml
```

### Comparing `legend_pygeom_optics-0.6.1/src/legendoptics/copper.py` & `legend_pygeom_optics-0.6.2/src/legendoptics/copper.py`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/src/legendoptics/data/cu_reflectivity.dat` & `legend_pygeom_optics-0.6.2/src/legendoptics/data/cu_reflectivity.dat`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/src/legendoptics/data/ge_reflectivity.dat` & `legend_pygeom_optics-0.6.2/src/legendoptics/data/ge_reflectivity.dat`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/src/legendoptics/data/lar_emission_heindl2010.dat` & `legend_pygeom_optics-0.6.2/src/legendoptics/data/lar_emission_heindl2010.dat`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/src/legendoptics/data/nylon_absorption.dat` & `legend_pygeom_optics-0.6.2/src/legendoptics/data/nylon_absorption.dat`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/src/legendoptics/data/pen_abslength.dat` & `legend_pygeom_optics-0.6.2/src/legendoptics/data/pen_abslength.dat`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/src/legendoptics/data/pen_wlscomponent.dat` & `legend_pygeom_optics-0.6.2/src/legendoptics/data/pen_wlscomponent.dat`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/src/legendoptics/data/psfibers_wlsabslength.dat` & `legend_pygeom_optics-0.6.2/src/legendoptics/data/psfibers_wlsabslength.dat`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/src/legendoptics/data/psfibers_wlscomponent.dat` & `legend_pygeom_optics-0.6.2/src/legendoptics/data/psfibers_wlscomponent.dat`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/src/legendoptics/data/si_rindex_imag.dat` & `legend_pygeom_optics-0.6.2/src/legendoptics/data/si_rindex_imag.dat`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/src/legendoptics/data/si_rindex_real.dat` & `legend_pygeom_optics-0.6.2/src/legendoptics/data/si_rindex_real.dat`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/src/legendoptics/data/tpb_polystyrene_wlscomponent.dat` & `legend_pygeom_optics-0.6.2/src/legendoptics/data/tpb_polystyrene_wlscomponent.dat`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/src/legendoptics/data/tpb_vm2000_wlscomponent.dat` & `legend_pygeom_optics-0.6.2/src/legendoptics/data/tpb_vm2000_wlscomponent.dat`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/src/legendoptics/data/tpb_wlsabslength.dat` & `legend_pygeom_optics-0.6.2/src/legendoptics/data/tpb_wlsabslength.dat`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/src/legendoptics/fibers.py` & `legend_pygeom_optics-0.6.2/src/legendoptics/fibers.py`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/src/legendoptics/germanium.py` & `legend_pygeom_optics-0.6.2/src/legendoptics/germanium.py`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/src/legendoptics/lar.py` & `legend_pygeom_optics-0.6.2/src/legendoptics/lar.py`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/src/legendoptics/nylon.py` & `legend_pygeom_optics-0.6.2/src/legendoptics/nylon.py`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/src/legendoptics/pen.py` & `legend_pygeom_optics-0.6.2/src/legendoptics/pen.py`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/src/legendoptics/plot.py` & `legend_pygeom_optics-0.6.2/src/legendoptics/plot.py`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/src/legendoptics/pyg4utils.py` & `legend_pygeom_optics-0.6.2/src/legendoptics/pyg4utils.py`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/src/legendoptics/silicon.py` & `legend_pygeom_optics-0.6.2/src/legendoptics/silicon.py`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/src/legendoptics/tetratex.py` & `legend_pygeom_optics-0.6.2/src/legendoptics/tetratex.py`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/src/legendoptics/tpb.py` & `legend_pygeom_optics-0.6.2/src/legendoptics/tpb.py`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/src/legendoptics/utils.py` & `legend_pygeom_optics-0.6.2/src/legendoptics/utils.py`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/tests/test_import.py` & `legend_pygeom_optics-0.6.2/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/tests/test_plot.py` & `legend_pygeom_optics-0.6.2/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `legend_pygeom_optics-0.6.1/tests/test_pyg4.py` & `legend_pygeom_optics-0.6.2/tests/test_pyg4.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test the attaching of all properties to Geant4 materials."""
+
 from __future__ import annotations
 
 import pint
 import pyg4ometry.geant4 as g4
 
 u = pint.get_application_registry()
```

