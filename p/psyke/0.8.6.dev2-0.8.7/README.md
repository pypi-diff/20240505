# Comparing `tmp/psyke-0.8.6.dev2.tar.gz` & `tmp/psyke-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psyke-0.8.6.dev2.tar", last modified: Sat May  4 00:09:03 2024, max compression
+gzip compressed data, was "psyke-0.8.7.tar", last modified: Sat May  4 16:36:36 2024, max compression
```

## Comparing `psyke-0.8.6.dev2.tar` & `psyke-0.8.7.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.176646 psyke-0.8.6.dev2/
--rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-05-04 00:09:03.176646 psyke-0.8.6.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-04 00:09:03.000000 psyke-0.8.6.dev2/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.164646 psyke-0.8.6.dev2/psyke/
--rw-r--r--   0 runner    (1001) docker     (127)    18545 2024-05-04 00:09:00.000000 psyke-0.8.6.dev2/psyke/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.168646 psyke-0.8.6.dev2/psyke/clustering/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/clustering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.168646 psyke-0.8.6.dev2/psyke/clustering/cream/
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/clustering/cream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.168646 psyke-0.8.6.dev2/psyke/clustering/exact/
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/clustering/exact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/clustering/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.168646 psyke-0.8.6.dev2/psyke/extraction/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.168646 psyke-0.8.6.dev2/psyke/extraction/cart/
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/cart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/cart/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.168646 psyke-0.8.6.dev2/psyke/extraction/hypercubic/
--rw-r--r--   0 runner    (1001) docker     (127)    10620 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/hypercubic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.168646 psyke-0.8.6.dev2/psyke/extraction/hypercubic/cosmik/
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/hypercubic/cosmik/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.168646 psyke-0.8.6.dev2/psyke/extraction/hypercubic/creepy/
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/hypercubic/creepy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.168646 psyke-0.8.6.dev2/psyke/extraction/hypercubic/divine/
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/hypercubic/divine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.168646 psyke-0.8.6.dev2/psyke/extraction/hypercubic/gridex/
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/hypercubic/gridex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.168646 psyke-0.8.6.dev2/psyke/extraction/hypercubic/gridrex/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/hypercubic/gridrex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.168646 psyke-0.8.6.dev2/psyke/extraction/hypercubic/hex/
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/hypercubic/hex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25697 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/hypercubic/hypercube.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.168646 psyke-0.8.6.dev2/psyke/extraction/hypercubic/iter/
--rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/hypercubic/iter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/hypercubic/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/hypercubic/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.168646 psyke-0.8.6.dev2/psyke/extraction/real/
--rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/real/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/real/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.172646 psyke-0.8.6.dev2/psyke/extraction/trepan/
--rw-r--r--   0 runner    (1001) docker     (127)     6583 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/trepan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/trepan/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/hypercubepredictor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.172646 psyke-0.8.6.dev2/psyke/schema/
--rw-r--r--   0 runner    (1001) docker     (127)    17444 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.172646 psyke-0.8.6.dev2/psyke/tuning/
--rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/tuning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.172646 psyke-0.8.6.dev2/psyke/tuning/crash/
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/tuning/crash/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.172646 psyke-0.8.6.dev2/psyke/tuning/orchid/
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/tuning/orchid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.172646 psyke-0.8.6.dev2/psyke/tuning/pedro/
--rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/tuning/pedro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.172646 psyke-0.8.6.dev2/psyke/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/utils/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    12419 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/utils/logic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/utils/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/utils/sorted.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.176646 psyke-0.8.6.dev2/psyke.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-05-04 00:09:03.000000 psyke-0.8.6.dev2/psyke.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-04 00:09:03.000000 psyke-0.8.6.dev2/psyke.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 00:09:03.000000 psyke-0.8.6.dev2/psyke.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 00:09:02.000000 psyke-0.8.6.dev2/psyke.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-04 00:09:03.000000 psyke-0.8.6.dev2/psyke.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 00:09:03.000000 psyke-0.8.6.dev2/psyke.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 00:09:03.176646 psyke-0.8.6.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.164646 psyke-0.8.6.dev2/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.172646 psyke-0.8.6.dev2/test/psyke/
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.172646 psyke-0.8.6.dev2/test/psyke/clustering/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/clustering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.172646 psyke-0.8.6.dev2/test/psyke/extraction/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/extraction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.172646 psyke-0.8.6.dev2/test/psyke/extraction/cart/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/extraction/cart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/extraction/cart/test_cart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/extraction/cart/test_simplified_cart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.172646 psyke-0.8.6.dev2/test/psyke/extraction/hypercubic/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/extraction/hypercubic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.172646 psyke-0.8.6.dev2/test/psyke/extraction/hypercubic/gridex/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/extraction/hypercubic/gridex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/extraction/hypercubic/gridex/test_gridex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.176646 psyke-0.8.6.dev2/test/psyke/extraction/hypercubic/iter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/extraction/hypercubic/iter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/extraction/hypercubic/iter/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)    14255 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/extraction/hypercubic/test_hypercube.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.176646 psyke-0.8.6.dev2/test/psyke/extraction/real/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/extraction/real/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/extraction/real/test_real.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/extraction/real/test_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.176646 psyke-0.8.6.dev2/test/psyke/extraction/trepan/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/extraction/trepan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/extraction/trepan/test_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/extraction/trepan/test_split.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/extraction/trepan/test_trepan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.176646 psyke-0.8.6.dev2/test/psyke/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/utils/test_prune.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/utils/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/utils/test_simplify_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.176646 psyke-0.8.6.dev2/test/resources/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-04 00:07:23.000000 psyke-0.8.6.dev2/test/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.176646 psyke-0.8.6.dev2/test/resources/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-04 00:07:23.000000 psyke-0.8.6.dev2/test/resources/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.176646 psyke-0.8.6.dev2/test/resources/predictors/
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-04 00:07:23.000000 psyke-0.8.6.dev2/test/resources/predictors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.176646 psyke-0.8.6.dev2/test/resources/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-04 00:07:23.000000 psyke-0.8.6.dev2/test/resources/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.852476 psyke-0.8.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-05-04 16:35:22.000000 psyke-0.8.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-04 16:35:22.000000 psyke-0.8.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8096 2024-05-04 16:36:36.852476 psyke-0.8.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-05-04 16:35:22.000000 psyke-0.8.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-04 16:36:36.000000 psyke-0.8.7/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.840476 psyke-0.8.7/psyke/
+-rw-r--r--   0 runner    (1001) docker     (127)    18601 2024-05-04 16:36:34.000000 psyke-0.8.7/psyke/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.844477 psyke-0.8.7/psyke/clustering/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-04 16:35:22.000000 psyke-0.8.7/psyke/clustering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.844477 psyke-0.8.7/psyke/clustering/cream/
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-04 16:35:22.000000 psyke-0.8.7/psyke/clustering/cream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.844477 psyke-0.8.7/psyke/clustering/exact/
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-04 16:35:22.000000 psyke-0.8.7/psyke/clustering/exact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-04 16:35:22.000000 psyke-0.8.7/psyke/clustering/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.844477 psyke-0.8.7/psyke/extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-04 16:35:22.000000 psyke-0.8.7/psyke/extraction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.844477 psyke-0.8.7/psyke/extraction/cart/
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-04 16:35:22.000000 psyke-0.8.7/psyke/extraction/cart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-04 16:35:22.000000 psyke-0.8.7/psyke/extraction/cart/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.844477 psyke-0.8.7/psyke/extraction/hypercubic/
+-rw-r--r--   0 runner    (1001) docker     (127)    10620 2024-05-04 16:35:22.000000 psyke-0.8.7/psyke/extraction/hypercubic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.844477 psyke-0.8.7/psyke/extraction/hypercubic/cosmik/
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-04 16:35:22.000000 psyke-0.8.7/psyke/extraction/hypercubic/cosmik/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.844477 psyke-0.8.7/psyke/extraction/hypercubic/creepy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-04 16:35:22.000000 psyke-0.8.7/psyke/extraction/hypercubic/creepy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.844477 psyke-0.8.7/psyke/extraction/hypercubic/divine/
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-05-04 16:35:22.000000 psyke-0.8.7/psyke/extraction/hypercubic/divine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.844477 psyke-0.8.7/psyke/extraction/hypercubic/gridex/
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-04 16:35:22.000000 psyke-0.8.7/psyke/extraction/hypercubic/gridex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.844477 psyke-0.8.7/psyke/extraction/hypercubic/gridrex/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-04 16:35:22.000000 psyke-0.8.7/psyke/extraction/hypercubic/gridrex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.844477 psyke-0.8.7/psyke/extraction/hypercubic/hex/
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-04 16:35:22.000000 psyke-0.8.7/psyke/extraction/hypercubic/hex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25697 2024-05-04 16:35:22.000000 psyke-0.8.7/psyke/extraction/hypercubic/hypercube.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.844477 psyke-0.8.7/psyke/extraction/hypercubic/iter/
+-rw-r--r--   0 runner    (1001) docker     (127)    10054 2024-05-04 16:35:22.000000 psyke-0.8.7/psyke/extraction/hypercubic/iter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-04 16:35:22.000000 psyke-0.8.7/psyke/extraction/hypercubic/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-04 16:35:22.000000 psyke-0.8.7/psyke/extraction/hypercubic/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.844477 psyke-0.8.7/psyke/extraction/real/
+-rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-05-04 16:35:22.000000 psyke-0.8.7/psyke/extraction/real/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-04 16:35:22.000000 psyke-0.8.7/psyke/extraction/real/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.848477 psyke-0.8.7/psyke/extraction/trepan/
+-rw-r--r--   0 runner    (1001) docker     (127)     6583 2024-05-04 16:35:22.000000 psyke-0.8.7/psyke/extraction/trepan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-04 16:35:22.000000 psyke-0.8.7/psyke/extraction/trepan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-05-04 16:35:22.000000 psyke-0.8.7/psyke/hypercubepredictor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.848477 psyke-0.8.7/psyke/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)    25929 2024-05-04 16:35:22.000000 psyke-0.8.7/psyke/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.848477 psyke-0.8.7/psyke/tuning/
+-rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-05-04 16:35:22.000000 psyke-0.8.7/psyke/tuning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.848477 psyke-0.8.7/psyke/tuning/crash/
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-04 16:35:22.000000 psyke-0.8.7/psyke/tuning/crash/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.848477 psyke-0.8.7/psyke/tuning/orchid/
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-05-04 16:35:22.000000 psyke-0.8.7/psyke/tuning/orchid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.848477 psyke-0.8.7/psyke/tuning/pedro/
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-05-04 16:35:22.000000 psyke-0.8.7/psyke/tuning/pedro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.848477 psyke-0.8.7/psyke/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-04 16:35:22.000000 psyke-0.8.7/psyke/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-05-04 16:35:22.000000 psyke-0.8.7/psyke/utils/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12419 2024-05-04 16:35:22.000000 psyke-0.8.7/psyke/utils/logic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-04 16:35:22.000000 psyke-0.8.7/psyke/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-05-04 16:35:22.000000 psyke-0.8.7/psyke/utils/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-04 16:35:22.000000 psyke-0.8.7/psyke/utils/sorted.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.852476 psyke-0.8.7/psyke.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8096 2024-05-04 16:36:36.000000 psyke-0.8.7/psyke.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-04 16:36:36.000000 psyke-0.8.7/psyke.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 16:36:36.000000 psyke-0.8.7/psyke.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 16:36:36.000000 psyke-0.8.7/psyke.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-04 16:36:36.000000 psyke-0.8.7/psyke.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 16:36:36.000000 psyke-0.8.7/psyke.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-04 16:35:22.000000 psyke-0.8.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 16:36:36.852476 psyke-0.8.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-05-04 16:35:22.000000 psyke-0.8.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.840476 psyke-0.8.7/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.848477 psyke-0.8.7/test/psyke/
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-05-04 16:35:22.000000 psyke-0.8.7/test/psyke/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.848477 psyke-0.8.7/test/psyke/clustering/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 16:35:22.000000 psyke-0.8.7/test/psyke/clustering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.848477 psyke-0.8.7/test/psyke/extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 16:35:22.000000 psyke-0.8.7/test/psyke/extraction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.848477 psyke-0.8.7/test/psyke/extraction/cart/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 16:35:22.000000 psyke-0.8.7/test/psyke/extraction/cart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-04 16:35:22.000000 psyke-0.8.7/test/psyke/extraction/cart/test_cart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-04 16:35:22.000000 psyke-0.8.7/test/psyke/extraction/cart/test_simplified_cart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.848477 psyke-0.8.7/test/psyke/extraction/hypercubic/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 16:35:22.000000 psyke-0.8.7/test/psyke/extraction/hypercubic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.848477 psyke-0.8.7/test/psyke/extraction/hypercubic/gridex/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 16:35:22.000000 psyke-0.8.7/test/psyke/extraction/hypercubic/gridex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-04 16:35:22.000000 psyke-0.8.7/test/psyke/extraction/hypercubic/gridex/test_gridex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.848477 psyke-0.8.7/test/psyke/extraction/hypercubic/iter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 16:35:22.000000 psyke-0.8.7/test/psyke/extraction/hypercubic/iter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-04 16:35:22.000000 psyke-0.8.7/test/psyke/extraction/hypercubic/iter/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14255 2024-05-04 16:35:22.000000 psyke-0.8.7/test/psyke/extraction/hypercubic/test_hypercube.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.852476 psyke-0.8.7/test/psyke/extraction/real/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 16:35:22.000000 psyke-0.8.7/test/psyke/extraction/real/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-04 16:35:22.000000 psyke-0.8.7/test/psyke/extraction/real/test_real.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-04 16:35:22.000000 psyke-0.8.7/test/psyke/extraction/real/test_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.852476 psyke-0.8.7/test/psyke/extraction/trepan/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 16:35:22.000000 psyke-0.8.7/test/psyke/extraction/trepan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-04 16:35:22.000000 psyke-0.8.7/test/psyke/extraction/trepan/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-04 16:35:22.000000 psyke-0.8.7/test/psyke/extraction/trepan/test_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-04 16:35:22.000000 psyke-0.8.7/test/psyke/extraction/trepan/test_trepan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.852476 psyke-0.8.7/test/psyke/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 16:35:22.000000 psyke-0.8.7/test/psyke/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-04 16:35:22.000000 psyke-0.8.7/test/psyke/utils/test_prune.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-04 16:35:22.000000 psyke-0.8.7/test/psyke/utils/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-04 16:35:22.000000 psyke-0.8.7/test/psyke/utils/test_simplify_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.852476 psyke-0.8.7/test/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-04 16:35:23.000000 psyke-0.8.7/test/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.852476 psyke-0.8.7/test/resources/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-04 16:35:23.000000 psyke-0.8.7/test/resources/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.852476 psyke-0.8.7/test/resources/predictors/
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-04 16:35:23.000000 psyke-0.8.7/test/resources/predictors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:36:36.852476 psyke-0.8.7/test/resources/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-04 16:35:24.000000 psyke-0.8.7/test/resources/tests/__init__.py
```

### Comparing `psyke-0.8.6.dev2/LICENSE` & `psyke-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/PKG-INFO` & `psyke-0.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psyke
-Version: 0.8.6.dev2
+Version: 0.8.7
 Summary: Python-based implementation of PSyKE, i.e. a Platform for Symbolic Knowledge Extraction
 Home-page: https://github.com/psykei/psyke-python
 Author: Matteo Magnini
 Author-email: matteo.magnini@unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/psykei/psyke-python/issues
 Project-URL: Source, https://github.com/psykei/psyke-python
```

### Comparing `psyke-0.8.6.dev2/README.md` & `psyke-0.8.7/README.md`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/psyke/__init__.py` & `psyke-0.8.7/psyke/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -285,22 +285,23 @@
         """
         from psyke.extraction.hypercubic.cosmik import COSMiK
         return COSMiK(predictor, max_components=max_components, k=k, patience=patience, close_to_center=close_to_center,
                       output=output, discretization=discretization, normalization=normalization, seed=seed)
 
     @staticmethod
     def iter(predictor, min_update: float = 0.1, n_points: int = 1, max_iterations: int = 600, min_examples: int = 250,
-             threshold: float = 0.1, fill_gaps: bool = True, normalization: dict[str, tuple[float, float]] = None,
-             output=None, seed: int = get_default_random_seed()) -> Extractor:
+             threshold: float = 0.1, fill_gaps: bool = True, ignore_dimensions=None,
+             normalization: dict[str, tuple[float, float]] = None, output=None,
+             seed: int = get_default_random_seed()) -> Extractor:
         """
         Creates a new ITER extractor.
         """
         from psyke.extraction.hypercubic.iter import ITER
         return ITER(predictor, min_update, n_points, max_iterations, min_examples, threshold, fill_gaps,
-                    normalization, output, seed)
+                    ignore_dimensions, normalization, output, seed)
 
     @staticmethod
     def gridex(predictor, grid, min_examples: int = 250, threshold: float = 0.1, output: Target = Target.CONSTANT,
                discretization=None, normalization: dict[str, tuple[float, float]] = None,
                seed: int = get_default_random_seed()) -> Extractor:
         """
         Creates a new GridEx extractor.
```

### Comparing `psyke-0.8.6.dev2/psyke/clustering/__init__.py` & `psyke-0.8.7/psyke/clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/psyke/clustering/cream/__init__.py` & `psyke-0.8.7/psyke/clustering/cream/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/psyke/clustering/exact/__init__.py` & `psyke-0.8.7/psyke/clustering/exact/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/psyke/clustering/utils.py` & `psyke-0.8.7/psyke/clustering/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/psyke/extraction/__init__.py` & `psyke-0.8.7/psyke/extraction/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/psyke/extraction/cart/__init__.py` & `psyke-0.8.7/psyke/extraction/cart/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/psyke/extraction/cart/predictor.py` & `psyke-0.8.7/psyke/extraction/cart/predictor.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/psyke/extraction/hypercubic/__init__.py` & `psyke-0.8.7/psyke/extraction/hypercubic/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/psyke/extraction/hypercubic/cosmik/__init__.py` & `psyke-0.8.7/psyke/extraction/hypercubic/cosmik/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/psyke/extraction/hypercubic/creepy/__init__.py` & `psyke-0.8.7/psyke/extraction/hypercubic/creepy/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/psyke/extraction/hypercubic/divine/__init__.py` & `psyke-0.8.7/psyke/extraction/hypercubic/divine/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/psyke/extraction/hypercubic/gridex/__init__.py` & `psyke-0.8.7/psyke/extraction/hypercubic/gridex/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/psyke/extraction/hypercubic/gridrex/__init__.py` & `psyke-0.8.7/psyke/extraction/hypercubic/gridrex/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/psyke/extraction/hypercubic/hex/__init__.py` & `psyke-0.8.7/psyke/extraction/hypercubic/hex/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/psyke/extraction/hypercubic/hypercube.py` & `psyke-0.8.7/psyke/extraction/hypercubic/hypercube.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/psyke/extraction/hypercubic/iter/__init__.py` & `psyke-0.8.7/psyke/extraction/hypercubic/iter/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,28 +12,30 @@
 
 class ITER(HyperCubeExtractor):
     """
     Explanator implementing ITER algorithm, doi:10.1007/11823728_26.
     """
 
     def __init__(self, predictor, min_update, n_points, max_iterations, min_examples, threshold, fill_gaps,
-                 normalization, output: Target = Target.CONSTANT, seed=get_default_random_seed()):
-        super().__init__(predictor, output, normalization)
+                 ignore_dimensions: Iterable, normalization, output: Target = Target.CONSTANT,
+                 seed=get_default_random_seed()):
+        super().__init__(predictor, output, normalization=normalization)
         if output is Target.REGRESSION:
             raise NotImplementedError
         self.predictor = predictor
         self.min_update = min_update
         self.n_points = n_points
         self.max_iterations = max_iterations
         self.min_examples = min_examples
         self.threshold = threshold
         self.fill_gaps = fill_gaps
         self._output = Target.CLASSIFICATION if isinstance(predictor, ClassifierMixin) else \
             output if output is not None else Target.CONSTANT
         self.seed = seed
+        self.ignore_dimensions = ignore_dimensions if ignore_dimensions is not None else []
 
     def _best_cube(self, dataframe: pd.DataFrame, cube: GenericCube, cubes: Iterable[Expansion]) -> Expansion | None:
         expansions = []
         for limit in cubes:
             count = limit.cube.count(dataframe)
             dataframe = pd.concat([dataframe, limit.cube.create_samples(self.min_examples - count)])
             limit.cube.update(dataframe, self.predictor)
@@ -70,14 +72,16 @@
         else:
             cube.add_limit(feature, direction)
 
     def _create_temp_cubes(self, cube: GenericCube, min_updates: Iterable[MinUpdate],
                            hypercubes: Iterable[GenericCube]) -> Iterable[Expansion]:
         tmp_cubes = []
         for feature in self._surrounding.dimensions.keys():
+            if feature in self.ignore_dimensions:
+                continue
             limit = cube.check_limits(feature)
             if limit == '*':
                 continue
             for x in {'-', '+'} - {limit}:
                 tmp_cubes += self._create_temp_cube(cube, min_updates, hypercubes, feature, x)
         return tmp_cubes
 
@@ -128,14 +132,16 @@
         return min_updates
 
     def _init_hypercubes(self, dataframe: pd.DataFrame, min_updates: Iterable[MinUpdate]):
         while True:
             hypercubes = self._generate_starting_points(dataframe)
             for hypercube in hypercubes:
                 hypercube.expand_all(min_updates, self._surrounding)
+                for d in self.ignore_dimensions:
+                    hypercube[d] = self._surrounding[d]
             self.n_points = self.n_points - 1
             if not HyperCube.check_overlap(hypercubes, hypercubes):
                 break
         self._hypercubes = hypercubes
 
     def _iterate(self, dataframe: pd.DataFrame, hypercubes: Iterable[GenericCube], min_updates: Iterable[MinUpdate],
                  left_iteration: int) -> int:
```

### Comparing `psyke-0.8.6.dev2/psyke/extraction/hypercubic/strategy.py` & `psyke-0.8.7/psyke/extraction/hypercubic/strategy.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/psyke/extraction/hypercubic/utils.py` & `psyke-0.8.7/psyke/extraction/hypercubic/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/psyke/extraction/real/__init__.py` & `psyke-0.8.7/psyke/extraction/real/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/psyke/extraction/real/utils.py` & `psyke-0.8.7/psyke/extraction/real/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/psyke/extraction/trepan/__init__.py` & `psyke-0.8.7/psyke/extraction/trepan/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/psyke/extraction/trepan/utils.py` & `psyke-0.8.7/psyke/extraction/trepan/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/psyke/hypercubepredictor.py` & `psyke-0.8.7/psyke/hypercubepredictor.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/psyke/tuning/__init__.py` & `psyke-0.8.7/psyke/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/psyke/tuning/crash/__init__.py` & `psyke-0.8.7/psyke/tuning/crash/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/psyke/tuning/orchid/__init__.py` & `psyke-0.8.7/psyke/tuning/orchid/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/psyke/tuning/pedro/__init__.py` & `psyke-0.8.7/psyke/tuning/pedro/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -94,22 +94,23 @@
     def __contains(self, strategies, strategy):
         for s in strategies:
             if strategy.equals(s, self.dataframe.columns[:-1]):
                 return True
         return False
 
     def search(self):
+        max_partitions = 200
         base_partitions = FixedStrategy(2).partition_number(self.dataframe.columns[:-1]) * 3
-        if base_partitions <= 50:
+        if base_partitions <= max_partitions:
             strategies = [FixedStrategy(2)]
-            if FixedStrategy(3).partition_number(self.dataframe.columns[:-1]) <= base_partitions:
+            if FixedStrategy(3).partition_number(self.dataframe.columns[:-1]) <= max_partitions:
                 strategies.append(FixedStrategy(3))
         else:
             strategies = []
-            base_partitions = 50
+            base_partitions = max_partitions
 
         for n in [2, 3, 5, 10]:
             for th in [0.99, 0.75, 0.67, 0.5, 0.3]:
                 strategy = AdaptiveStrategy(self.ranked, [(th, n)])
                 if strategy.partition_number(self.dataframe.columns[:-1]) < base_partitions and \
                         not self.__contains(strategies, strategy):
                     strategies.append(strategy)
```

### Comparing `psyke-0.8.6.dev2/psyke/utils/__init__.py` & `psyke-0.8.7/psyke/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/psyke/utils/dataframe.py` & `psyke-0.8.7/psyke/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/psyke/utils/logic.py` & `psyke-0.8.7/psyke/utils/logic.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/psyke/utils/metrics.py` & `psyke-0.8.7/psyke/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/psyke/utils/plot.py` & `psyke-0.8.7/psyke/utils/plot.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/psyke/utils/sorted.py` & `psyke-0.8.7/psyke/utils/sorted.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/psyke.egg-info/PKG-INFO` & `psyke-0.8.7/psyke.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psyke
-Version: 0.8.6.dev2
+Version: 0.8.7
 Summary: Python-based implementation of PSyKE, i.e. a Platform for Symbolic Knowledge Extraction
 Home-page: https://github.com/psykei/psyke-python
 Author: Matteo Magnini
 Author-email: matteo.magnini@unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/psykei/psyke-python/issues
 Project-URL: Source, https://github.com/psykei/psyke-python
```

### Comparing `psyke-0.8.6.dev2/psyke.egg-info/SOURCES.txt` & `psyke-0.8.7/psyke.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/setup.py` & `psyke-0.8.7/setup.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/test/psyke/__init__.py` & `psyke-0.8.7/test/psyke/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/test/psyke/extraction/cart/test_cart.py` & `psyke-0.8.7/test/psyke/extraction/cart/test_cart.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/test/psyke/extraction/cart/test_simplified_cart.py` & `psyke-0.8.7/test/psyke/extraction/cart/test_simplified_cart.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/test/psyke/extraction/hypercubic/gridex/test_gridex.py` & `psyke-0.8.7/test/psyke/extraction/hypercubic/gridex/test_gridex.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/test/psyke/extraction/hypercubic/iter/test_iter.py` & `psyke-0.8.7/test/psyke/extraction/hypercubic/iter/test_iter.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/test/psyke/extraction/hypercubic/test_hypercube.py` & `psyke-0.8.7/test/psyke/extraction/hypercubic/test_hypercube.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/test/psyke/extraction/real/test_real.py` & `psyke-0.8.7/test/psyke/extraction/real/test_real.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/test/psyke/extraction/real/test_rule.py` & `psyke-0.8.7/test/psyke/extraction/real/test_rule.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/test/psyke/extraction/trepan/test_node.py` & `psyke-0.8.7/test/psyke/extraction/trepan/test_node.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/test/psyke/extraction/trepan/test_split.py` & `psyke-0.8.7/test/psyke/extraction/trepan/test_split.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/test/psyke/extraction/trepan/test_trepan.py` & `psyke-0.8.7/test/psyke/extraction/trepan/test_trepan.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/test/psyke/utils/test_prune.py` & `psyke-0.8.7/test/psyke/utils/test_prune.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/test/psyke/utils/test_simplify.py` & `psyke-0.8.7/test/psyke/utils/test_simplify.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/test/psyke/utils/test_simplify_formatter.py` & `psyke-0.8.7/test/psyke/utils/test_simplify_formatter.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.6.dev2/test/resources/tests/__init__.py` & `psyke-0.8.7/test/resources/tests/__init__.py`

 * *Files identical despite different names*

