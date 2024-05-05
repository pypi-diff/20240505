# Comparing `tmp/blissoda-0.3.1.tar.gz` & `tmp/blissoda-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blissoda-0.3.1.tar", last modified: Wed Mar 13 16:24:19 2024, max compression
+gzip compressed data, was "blissoda-0.4.0.tar", last modified: Sun May  5 14:56:54 2024, max compression
```

## Comparing `blissoda-0.3.1.tar` & `blissoda-0.4.0.tar`

### file list

```diff
@@ -1,147 +1,155 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:24:19.409190 blissoda-0.3.1/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2024-03-13 14:03:14.000000 blissoda-0.3.1/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     6390 2024-03-13 16:24:19.409190 blissoda-0.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1112 2024-03-13 14:03:14.000000 blissoda-0.3.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-03-13 14:03:14.000000 blissoda-0.3.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1714 2024-03-13 16:24:19.409190 blissoda-0.3.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2024-03-13 14:03:14.000000 blissoda-0.3.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:24:19.377190 blissoda-0.3.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:24:19.381190 blissoda-0.3.1/src/blissoda/
--rw-rw-rw-   0 root         (0) root         (0)      771 2024-03-13 16:09:30.000000 blissoda-0.3.1/src/blissoda/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:24:19.385190 blissoda-0.3.1/src/blissoda/app/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 16:24:13.000000 blissoda-0.3.1/src/blissoda/app/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1531 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/app/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     1303 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/app/cli_log_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:24:19.385190 blissoda-0.3.1/src/blissoda/app/workflow_server/
--rw-rw-rw-   0 root         (0) root         (0)     1695 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/app/workflow_server/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1028 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/app/workflow_server/subscriberv0.py
--rw-rw-rw-   0 root         (0) root         (0)     1106 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/app/workflow_server/subscriberv1.py
--rw-rw-rw-   0 root         (0) root         (0)     1112 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/app/workflow_server/subscribervid31.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:24:19.385190 blissoda-0.3.1/src/blissoda/bm02/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 16:24:13.000000 blissoda-0.3.1/src/blissoda/bm02/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1575 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/bm02/xrpd_processor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:24:19.385190 blissoda-0.3.1/src/blissoda/bm23/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 16:24:13.000000 blissoda-0.3.1/src/blissoda/bm23/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      916 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/bm23/exafs_plotter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:24:19.385190 blissoda-0.3.1/src/blissoda/demo/
--rw-rw-rw-   0 root         (0) root         (0)      154 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/demo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/demo/calib.py
--rw-rw-rw-   0 root         (0) root         (0)     1651 2024-03-13 15:29:18.000000 blissoda-0.3.1/src/blissoda/demo/exafs.py
--rw-rw-rw-   0 root         (0) root         (0)     3251 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/demo/example.py
--rw-rw-rw-   0 root         (0) root         (0)     3365 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/demo/id11.py
--rw-rw-rw-   0 root         (0) root         (0)      572 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/demo/id14.py
--rw-rw-rw-   0 root         (0) root         (0)     3453 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/demo/id22.py
--rw-rw-rw-   0 root         (0) root         (0)     5951 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/demo/streamline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:24:19.389190 blissoda-0.3.1/src/blissoda/demo/user_scripts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 16:24:13.000000 blissoda-0.3.1/src/blissoda/demo/user_scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3233 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/demo/user_scripts/all.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/demo/user_scripts/exafs.py
--rw-rw-rw-   0 root         (0) root         (0)      790 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/demo/user_scripts/id11.py
--rw-rw-rw-   0 root         (0) root         (0)      321 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/demo/user_scripts/id14.py
--rw-rw-rw-   0 root         (0) root         (0)      616 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/demo/user_scripts/id22.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/demo/user_scripts/streamline.py
--rw-rw-rw-   0 root         (0) root         (0)      710 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/demo/user_scripts/xrpd.py
--rw-rw-rw-   0 root         (0) root         (0)     2941 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/demo/xrpd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:24:19.389190 blissoda-0.3.1/src/blissoda/exafs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 16:24:13.000000 blissoda-0.3.1/src/blissoda/exafs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      535 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/exafs/plots.py
--rw-rw-rw-   0 root         (0) root         (0)    12719 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/exafs/plotter.py
--rw-rw-rw-   0 root         (0) root         (0)     9917 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/exafs/widgets.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:24:19.389190 blissoda-0.3.1/src/blissoda/flint/
--rw-rw-rw-   0 root         (0) root         (0)     1590 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/flint/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:24:19.389190 blissoda-0.3.1/src/blissoda/id09/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 16:24:13.000000 blissoda-0.3.1/src/blissoda/id09/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3369 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/id09/xrpd_processor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:24:19.389190 blissoda-0.3.1/src/blissoda/id11/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 16:24:13.000000 blissoda-0.3.1/src/blissoda/id11/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5774 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/id11/xrpd_processor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:24:19.389190 blissoda-0.3.1/src/blissoda/id14/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 16:24:13.000000 blissoda-0.3.1/src/blissoda/id14/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3668 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/id14/converter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:24:19.389190 blissoda-0.3.1/src/blissoda/id22/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 16:24:13.000000 blissoda-0.3.1/src/blissoda/id22/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    32606 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/id22/stscan_processor.py
--rw-rw-rw-   0 root         (0) root         (0)     5056 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/id22/xrpd_processor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:24:19.389190 blissoda-0.3.1/src/blissoda/id24/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 16:24:13.000000 blissoda-0.3.1/src/blissoda/id24/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      827 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/id24/exafs_plotter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:24:19.389190 blissoda-0.3.1/src/blissoda/id31/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 16:24:13.000000 blissoda-0.3.1/src/blissoda/id31/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6220 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/id31/optimize_exposure.py
--rw-rw-rw-   0 root         (0) root         (0)     4661 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/id31/streamline_scanner.py
--rw-rw-rw-   0 root         (0) root         (0)     3331 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/id31/xrpd_processor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:24:19.393190 blissoda-0.3.1/src/blissoda/persistent/
--rw-rw-rw-   0 root         (0) root         (0)       93 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/persistent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:24:19.393190 blissoda-0.3.1/src/blissoda/persistent/ndarray/
--rw-rw-rw-   0 root         (0) root         (0)      535 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/persistent/ndarray/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2074 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/persistent/ndarray/ndarrayv0.py
--rw-rw-rw-   0 root         (0) root         (0)     1612 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/persistent/ndarray/ndarrayv1.py
--rw-rw-rw-   0 root         (0) root         (0)     1410 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/persistent/ordereddict.py
--rw-rw-rw-   0 root         (0) root         (0)     7605 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/persistent/parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:24:19.393190 blissoda-0.3.1/src/blissoda/resources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 16:24:13.000000 blissoda-0.3.1/src/blissoda/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:24:19.393190 blissoda-0.3.1/src/blissoda/resources/demo/
--rw-rw-rw-   0 root         (0) root         (0)       70 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/resources/demo/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    47387 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/resources/demo/background.xy
--rw-rw-rw-   0 root         (0) root         (0)      276 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/resources/demo/pdf_config.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:24:19.393190 blissoda-0.3.1/src/blissoda/resources/exafs/
--rw-rw-rw-   0 root         (0) root         (0)       70 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/resources/exafs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4653 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/resources/exafs/exafs.ows
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:24:19.393190 blissoda-0.3.1/src/blissoda/resources/id11/
--rw-rw-rw-   0 root         (0) root         (0)       70 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/resources/id11/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1519 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/resources/id11/integrate_scan_with_saving.json
--rw-rw-rw-   0 root         (0) root         (0)     3066 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/resources/id11/integrate_scan_with_saving_pdf.json
--rw-rw-rw-   0 root         (0) root         (0)     1551 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/resources/id11/integrate_scan_without_saving.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:24:19.393190 blissoda-0.3.1/src/blissoda/resources/id22/
--rw-rw-rw-   0 root         (0) root         (0)     6390 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/resources/id22/Sum_then_integrate_with_saving.json
--rw-rw-rw-   0 root         (0) root         (0)       70 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/resources/id22/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:24:19.393190 blissoda-0.3.1/src/blissoda/resources/streamline/
--rw-rw-rw-   0 root         (0) root         (0)       70 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/resources/streamline/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3612 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/resources/streamline/reprocess.py
--rw-rw-rw-   0 root         (0) root         (0)     7835 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/resources/streamline/streamline_with_calib.json
--rw-rw-rw-   0 root         (0) root         (0)     5685 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/resources/streamline/streamline_without_calib.json
--rw-rw-rw-   0 root         (0) root         (0)     3758 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/resources/streamline/time_record.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:24:19.397190 blissoda-0.3.1/src/blissoda/resources/xrpd/
--rw-rw-rw-   0 root         (0) root         (0)       70 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/resources/xrpd/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1519 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/resources/xrpd/integrate_scan_with_saving.json
--rw-rw-rw-   0 root         (0) root         (0)     1551 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/resources/xrpd/integrate_scan_without_saving.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:24:19.397190 blissoda-0.3.1/src/blissoda/seslab/
--rw-rw-rw-   0 root         (0) root         (0)       30 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/seslab/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      942 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/seslab/streamline_scanner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:24:19.397190 blissoda-0.3.1/src/blissoda/streamline/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 16:24:13.000000 blissoda-0.3.1/src/blissoda/streamline/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21248 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/streamline/scanner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:24:19.397190 blissoda-0.3.1/src/blissoda/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 16:24:13.000000 blissoda-0.3.1/src/blissoda/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3566 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:24:19.397190 blissoda-0.3.1/src/blissoda/tests/mock_id31/
--rw-rw-rw-   0 root         (0) root         (0)      957 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/tests/mock_id31/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      487 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/tests/mock_id31/attenuator.py
--rw-rw-rw-   0 root         (0) root         (0)     3559 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/tests/mock_id31/controllers.py
--rw-rw-rw-   0 root         (0) root         (0)      157 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/tests/mock_id31/image_utils.py
--rw-rw-rw-   0 root         (0) root         (0)       65 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/tests/mock_id31/lima_image.py
--rw-rw-rw-   0 root         (0) root         (0)      426 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/tests/mock_id31/setup_globals.py
--rw-rw-rw-   0 root         (0) root         (0)     2775 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/tests/mock_id31/simulate.py
--rw-rw-rw-   0 root         (0) root         (0)    13550 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/tests/test_id22.py
--rw-rw-rw-   0 root         (0) root         (0)     1862 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/tests/test_id31.py
--rw-rw-rw-   0 root         (0) root         (0)     3943 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/tests/test_persistent.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:24:19.397190 blissoda-0.3.1/src/blissoda/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 16:24:13.000000 blissoda-0.3.1/src/blissoda/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1955 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/utils/directories.py
--rw-rw-rw-   0 root         (0) root         (0)     1075 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/utils/pyfai.py
--rw-rw-rw-   0 root         (0) root         (0)     1235 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/utils/trigger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:24:19.401190 blissoda-0.3.1/src/blissoda/xrpd/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 16:24:13.000000 blissoda-0.3.1/src/blissoda/xrpd/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4573 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/xrpd/data.py
--rw-rw-rw-   0 root         (0) root         (0)      884 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/xrpd/plots.py
--rw-rw-rw-   0 root         (0) root         (0)     7078 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/xrpd/plotter.py
--rw-rw-rw-   0 root         (0) root         (0)    20265 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/xrpd/processor.py
--rw-rw-rw-   0 root         (0) root         (0)     2765 2024-03-13 14:03:14.000000 blissoda-0.3.1/src/blissoda/xrpd/widgets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:24:19.401190 blissoda-0.3.1/src/blissoda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6390 2024-03-13 16:24:19.000000 blissoda-0.3.1/src/blissoda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4124 2024-03-13 16:24:19.000000 blissoda-0.3.1/src/blissoda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-13 16:24:19.000000 blissoda-0.3.1/src/blissoda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2024-03-13 16:24:19.000000 blissoda-0.3.1/src/blissoda.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      908 2024-03-13 16:24:19.000000 blissoda-0.3.1/src/blissoda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-03-13 16:24:19.000000 blissoda-0.3.1/src/blissoda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.109564 blissoda-0.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2024-05-05 10:00:40.000000 blissoda-0.4.0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     6835 2024-05-05 14:56:54.109564 blissoda-0.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2024-05-05 10:00:40.000000 blissoda-0.4.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-05-05 10:00:40.000000 blissoda-0.4.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1781 2024-05-05 14:56:54.109564 blissoda-0.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2024-05-05 10:00:40.000000 blissoda-0.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.077564 blissoda-0.4.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.081564 blissoda-0.4.0/src/blissoda/
+-rw-rw-rw-   0 root         (0) root         (0)      771 2024-05-05 14:52:05.000000 blissoda-0.4.0/src/blissoda/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.081564 blissoda-0.4.0/src/blissoda/app/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:56:48.000000 blissoda-0.4.0/src/blissoda/app/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1531 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/app/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/app/cli_log_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.081564 blissoda-0.4.0/src/blissoda/app/workflow_server/
+-rw-rw-rw-   0 root         (0) root         (0)     1695 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/app/workflow_server/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1028 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/app/workflow_server/subscriberv0.py
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/app/workflow_server/subscriberv1.py
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/app/workflow_server/subscribervid31.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.081564 blissoda-0.4.0/src/blissoda/bm02/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:56:48.000000 blissoda-0.4.0/src/blissoda/bm02/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1575 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/bm02/xrpd_processor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.081564 blissoda-0.4.0/src/blissoda/bm23/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:56:48.000000 blissoda-0.4.0/src/blissoda/bm23/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1327 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/bm23/exafs_plotter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.081564 blissoda-0.4.0/src/blissoda/demo/
+-rw-rw-rw-   0 root         (0) root         (0)      266 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/demo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/demo/calib.py
+-rw-rw-rw-   0 root         (0) root         (0)     1742 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/demo/exafs.py
+-rw-rw-rw-   0 root         (0) root         (0)     3251 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/demo/example.py
+-rw-rw-rw-   0 root         (0) root         (0)     3365 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/demo/id11.py
+-rw-rw-rw-   0 root         (0) root         (0)     1249 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/demo/id12.py
+-rw-rw-rw-   0 root         (0) root         (0)      534 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/demo/id14.py
+-rw-rw-rw-   0 root         (0) root         (0)     3629 2024-05-05 14:52:05.000000 blissoda-0.4.0/src/blissoda/demo/id22.py
+-rw-rw-rw-   0 root         (0) root         (0)     8312 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/demo/streamline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.085564 blissoda-0.4.0/src/blissoda/demo/user_scripts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:56:48.000000 blissoda-0.4.0/src/blissoda/demo/user_scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3712 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/demo/user_scripts/all.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/demo/user_scripts/exafs.py
+-rw-rw-rw-   0 root         (0) root         (0)      790 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/demo/user_scripts/id11.py
+-rw-rw-rw-   0 root         (0) root         (0)      436 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/demo/user_scripts/id12.py
+-rw-rw-rw-   0 root         (0) root         (0)      321 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/demo/user_scripts/id14.py
+-rw-rw-rw-   0 root         (0) root         (0)      616 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/demo/user_scripts/id22.py
+-rw-rw-rw-   0 root         (0) root         (0)      529 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/demo/user_scripts/streamline.py
+-rw-rw-rw-   0 root         (0) root         (0)      710 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/demo/user_scripts/xrpd.py
+-rw-rw-rw-   0 root         (0) root         (0)     2941 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/demo/xrpd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.085564 blissoda-0.4.0/src/blissoda/exafs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:56:48.000000 blissoda-0.4.0/src/blissoda/exafs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      535 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/exafs/plots.py
+-rw-rw-rw-   0 root         (0) root         (0)    12940 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/exafs/plotter.py
+-rw-rw-rw-   0 root         (0) root         (0)     9917 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/exafs/widgets.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.085564 blissoda-0.4.0/src/blissoda/flint/
+-rw-rw-rw-   0 root         (0) root         (0)     1590 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/flint/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.085564 blissoda-0.4.0/src/blissoda/id09/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:56:48.000000 blissoda-0.4.0/src/blissoda/id09/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3369 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/id09/xrpd_processor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.085564 blissoda-0.4.0/src/blissoda/id11/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:56:48.000000 blissoda-0.4.0/src/blissoda/id11/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5774 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/id11/xrpd_processor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.085564 blissoda-0.4.0/src/blissoda/id12/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:56:48.000000 blissoda-0.4.0/src/blissoda/id12/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4624 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/id12/converter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.085564 blissoda-0.4.0/src/blissoda/id14/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:56:48.000000 blissoda-0.4.0/src/blissoda/id14/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4006 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/id14/converter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.085564 blissoda-0.4.0/src/blissoda/id22/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:56:48.000000 blissoda-0.4.0/src/blissoda/id22/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    32576 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/id22/stscan_processor.py
+-rw-rw-rw-   0 root         (0) root         (0)     5093 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/id22/xrpd_processor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.085564 blissoda-0.4.0/src/blissoda/id24/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:56:48.000000 blissoda-0.4.0/src/blissoda/id24/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      866 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/id24/exafs_plotter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.085564 blissoda-0.4.0/src/blissoda/id31/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:56:48.000000 blissoda-0.4.0/src/blissoda/id31/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11177 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/id31/optimize_exposure.py
+-rw-rw-rw-   0 root         (0) root         (0)     8944 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/id31/streamline_scanner.py
+-rw-rw-rw-   0 root         (0) root         (0)     3331 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/id31/xrpd_processor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.085564 blissoda-0.4.0/src/blissoda/persistent/
+-rw-rw-rw-   0 root         (0) root         (0)       93 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/persistent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.085564 blissoda-0.4.0/src/blissoda/persistent/ndarray/
+-rw-rw-rw-   0 root         (0) root         (0)      535 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/persistent/ndarray/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2074 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/persistent/ndarray/ndarrayv0.py
+-rw-rw-rw-   0 root         (0) root         (0)     1612 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/persistent/ndarray/ndarrayv1.py
+-rw-rw-rw-   0 root         (0) root         (0)     1410 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/persistent/ordereddict.py
+-rw-rw-rw-   0 root         (0) root         (0)     7605 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/persistent/parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.085564 blissoda-0.4.0/src/blissoda/resources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:56:48.000000 blissoda-0.4.0/src/blissoda/resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.089564 blissoda-0.4.0/src/blissoda/resources/demo/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/demo/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    47387 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/demo/background.xy
+-rw-rw-rw-   0 root         (0) root         (0)      276 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/demo/pdf_config.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.089564 blissoda-0.4.0/src/blissoda/resources/exafs/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/exafs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4653 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/exafs/exafs.ows
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.089564 blissoda-0.4.0/src/blissoda/resources/id11/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/id11/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1519 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/id11/integrate_scan_with_saving.json
+-rw-rw-rw-   0 root         (0) root         (0)     3066 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/id11/integrate_scan_with_saving_pdf.json
+-rw-rw-rw-   0 root         (0) root         (0)     1551 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/id11/integrate_scan_without_saving.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.089564 blissoda-0.4.0/src/blissoda/resources/id12/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/id12/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      293 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/id12/convert.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.093564 blissoda-0.4.0/src/blissoda/resources/id22/
+-rw-rw-rw-   0 root         (0) root         (0)     6390 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/id22/Sum_then_integrate_with_saving.json
+-rw-rw-rw-   0 root         (0) root         (0)       70 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/id22/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.093564 blissoda-0.4.0/src/blissoda/resources/streamline/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/streamline/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3612 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/streamline/reprocess.py
+-rw-rw-rw-   0 root         (0) root         (0)     7835 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/streamline/streamline_with_calib.json
+-rw-rw-rw-   0 root         (0) root         (0)     5685 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/streamline/streamline_without_calib.json
+-rw-rw-rw-   0 root         (0) root         (0)     3758 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/streamline/time_record.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.093564 blissoda-0.4.0/src/blissoda/resources/xrpd/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/xrpd/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1519 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/xrpd/integrate_scan_with_saving.json
+-rw-rw-rw-   0 root         (0) root         (0)     1551 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/xrpd/integrate_scan_without_saving.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.097564 blissoda-0.4.0/src/blissoda/seslab/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/seslab/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      967 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/seslab/streamline_scanner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.097564 blissoda-0.4.0/src/blissoda/streamline/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:56:48.000000 blissoda-0.4.0/src/blissoda/streamline/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25258 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/streamline/scanner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.097564 blissoda-0.4.0/src/blissoda/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:56:48.000000 blissoda-0.4.0/src/blissoda/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3566 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.097564 blissoda-0.4.0/src/blissoda/tests/mock_id31/
+-rw-rw-rw-   0 root         (0) root         (0)      957 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/tests/mock_id31/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      487 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/tests/mock_id31/attenuator.py
+-rw-rw-rw-   0 root         (0) root         (0)     3559 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/tests/mock_id31/controllers.py
+-rw-rw-rw-   0 root         (0) root         (0)      157 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/tests/mock_id31/image_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)       65 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/tests/mock_id31/lima_image.py
+-rw-rw-rw-   0 root         (0) root         (0)      509 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/tests/mock_id31/setup_globals.py
+-rw-rw-rw-   0 root         (0) root         (0)     2775 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/tests/mock_id31/simulate.py
+-rw-rw-rw-   0 root         (0) root         (0)    13550 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/tests/test_id22.py
+-rw-rw-rw-   0 root         (0) root         (0)     1882 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/tests/test_id31.py
+-rw-rw-rw-   0 root         (0) root         (0)     3943 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/tests/test_persistent.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.097564 blissoda-0.4.0/src/blissoda/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:56:48.000000 blissoda-0.4.0/src/blissoda/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1955 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/utils/directories.py
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/utils/pyfai.py
+-rw-rw-rw-   0 root         (0) root         (0)     1235 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/utils/trigger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.097564 blissoda-0.4.0/src/blissoda/xrpd/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:56:48.000000 blissoda-0.4.0/src/blissoda/xrpd/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4573 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/xrpd/data.py
+-rw-rw-rw-   0 root         (0) root         (0)      884 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/xrpd/plots.py
+-rw-rw-rw-   0 root         (0) root         (0)     7078 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/xrpd/plotter.py
+-rw-rw-rw-   0 root         (0) root         (0)    20265 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/xrpd/processor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2765 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/xrpd/widgets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.097564 blissoda-0.4.0/src/blissoda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6835 2024-05-05 14:56:54.000000 blissoda-0.4.0/src/blissoda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4331 2024-05-05 14:56:54.000000 blissoda-0.4.0/src/blissoda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 14:56:54.000000 blissoda-0.4.0/src/blissoda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2024-05-05 14:56:54.000000 blissoda-0.4.0/src/blissoda.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     1028 2024-05-05 14:56:54.000000 blissoda-0.4.0/src/blissoda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-05 14:56:54.000000 blissoda-0.4.0/src/blissoda.egg-info/top_level.txt
```

### Comparing `blissoda-0.3.1/LICENSE.md` & `blissoda-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/PKG-INFO` & `blissoda-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blissoda
-Version: 0.3.1
+Version: 0.4.0
 Summary: Utilities for ewoks developers
 Home-page: https://gitlab.esrf.fr/bliss/blissoda/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/bliss/blissoda/
 Project-URL: Documentation, https://blissoda.readthedocs.io/
@@ -17,43 +17,52 @@
 License-File: LICENSE.md
 Provides-Extra: client
 Requires-Dist: blissdata>=0.2.5; extra == "client"
 Requires-Dist: ewoksjob; extra == "client"
 Provides-Extra: server
 Requires-Dist: blissdata>=0.2.5; extra == "server"
 Requires-Dist: ewoksjob; extra == "server"
-Provides-Extra: id22
-Requires-Dist: blissdata>=0.2.5; extra == "id22"
-Requires-Dist: ewoksjob; extra == "id22"
-Provides-Extra: id09
-Requires-Dist: blissdata>=0.2.5; extra == "id09"
-Requires-Dist: ewoksjob; extra == "id09"
-Provides-Extra: id31
-Requires-Dist: blissdata>=0.2.5; extra == "id31"
-Requires-Dist: ewoksjob; extra == "id31"
+Provides-Extra: id01
+Requires-Dist: blissdata>=0.2.5; extra == "id01"
+Requires-Dist: ewoksjob; extra == "id01"
 Provides-Extra: bm02
 Requires-Dist: blissdata>=0.2.5; extra == "bm02"
 Requires-Dist: ewoksjob; extra == "bm02"
+Provides-Extra: id09
+Requires-Dist: blissdata>=0.2.5; extra == "id09"
+Requires-Dist: ewoksjob; extra == "id09"
 Provides-Extra: id11
 Requires-Dist: blissdata>=0.2.5; extra == "id11"
 Requires-Dist: ewoksjob; extra == "id11"
+Provides-Extra: id12
+Requires-Dist: blissdata>=0.2.5; extra == "id12"
+Requires-Dist: ewoksjob; extra == "id12"
+Provides-Extra: id13
+Requires-Dist: blissdata>=0.2.5; extra == "id13"
+Requires-Dist: ewoksjob; extra == "id13"
 Provides-Extra: id14
 Requires-Dist: blissdata>=0.2.5; extra == "id14"
 Requires-Dist: ewoksjob; extra == "id14"
-Provides-Extra: streamline
-Requires-Dist: blissdata>=0.2.5; extra == "streamline"
-Requires-Dist: ewoksjob; extra == "streamline"
+Provides-Extra: id22
+Requires-Dist: blissdata>=0.2.5; extra == "id22"
+Requires-Dist: ewoksjob; extra == "id22"
 Provides-Extra: bm23
 Requires-Dist: blissdata>=0.2.5; extra == "bm23"
 Requires-Dist: ewoksjob; extra == "bm23"
 Requires-Dist: silx>=1.1.0; extra == "bm23"
 Provides-Extra: id24
 Requires-Dist: blissdata>=0.2.5; extra == "id24"
 Requires-Dist: ewoksjob; extra == "id24"
 Requires-Dist: silx>=1.1.0; extra == "id24"
+Provides-Extra: id31
+Requires-Dist: blissdata>=0.2.5; extra == "id31"
+Requires-Dist: ewoksjob; extra == "id31"
+Provides-Extra: streamline
+Requires-Dist: blissdata>=0.2.5; extra == "streamline"
+Requires-Dist: ewoksjob; extra == "streamline"
 Provides-Extra: democlient
 Requires-Dist: blissdata>=0.2.5; extra == "democlient"
 Requires-Dist: ewoksjob; extra == "democlient"
 Provides-Extra: demoworker
 Requires-Dist: blissdata>=0.2.5; extra == "demoworker"
 Requires-Dist: ewoksjob; extra == "demoworker"
 Requires-Dist: ewoksjob[blissworker]>=0.2.1; extra == "demoworker"
@@ -61,14 +70,15 @@
 Requires-Dist: est[full]; extra == "demoworker"
 Requires-Dist: orange3; extra == "demoworker"
 Provides-Extra: test
 Requires-Dist: pytest>=7; extra == "test"
 Requires-Dist: mock; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 Requires-Dist: pytest-redis; extra == "test"
+Requires-Dist: scipy; extra == "test"
 Requires-Dist: blissdata>=0.2.5; extra == "test"
 Requires-Dist: ewoksjob; extra == "test"
 Requires-Dist: blissdata>=0.2.5; extra == "test"
 Requires-Dist: ewoksjob; extra == "test"
 Requires-Dist: blissdata>=0.2.5; extra == "test"
 Requires-Dist: ewoksjob; extra == "test"
 Requires-Dist: blissdata>=0.2.5; extra == "test"
@@ -81,14 +91,15 @@
 Requires-Dist: ewoksjob; extra == "test"
 Requires-Dist: silx>=1.1.0; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pytest>=7; extra == "dev"
 Requires-Dist: mock; extra == "dev"
 Requires-Dist: pytest-mock; extra == "dev"
 Requires-Dist: pytest-redis; extra == "dev"
+Requires-Dist: scipy; extra == "dev"
 Requires-Dist: blissdata>=0.2.5; extra == "dev"
 Requires-Dist: ewoksjob; extra == "dev"
 Requires-Dist: blissdata>=0.2.5; extra == "dev"
 Requires-Dist: ewoksjob; extra == "dev"
 Requires-Dist: blissdata>=0.2.5; extra == "dev"
 Requires-Dist: ewoksjob; extra == "dev"
 Requires-Dist: blissdata>=0.2.5; extra == "dev"
@@ -103,14 +114,15 @@
 Requires-Dist: black>=22; extra == "dev"
 Requires-Dist: flake8>=4; extra == "dev"
 Provides-Extra: doc
 Requires-Dist: pytest>=7; extra == "doc"
 Requires-Dist: mock; extra == "doc"
 Requires-Dist: pytest-mock; extra == "doc"
 Requires-Dist: pytest-redis; extra == "doc"
+Requires-Dist: scipy; extra == "doc"
 Requires-Dist: blissdata>=0.2.5; extra == "doc"
 Requires-Dist: ewoksjob; extra == "doc"
 Requires-Dist: blissdata>=0.2.5; extra == "doc"
 Requires-Dist: ewoksjob; extra == "doc"
 Requires-Dist: blissdata>=0.2.5; extra == "doc"
 Requires-Dist: ewoksjob; extra == "doc"
 Requires-Dist: blissdata>=0.2.5; extra == "doc"
```

### Comparing `blissoda-0.3.1/README.md` & `blissoda-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/setup.cfg` & `blissoda-0.4.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -36,47 +36,54 @@
 [options.extras_require]
 client = 
 	blissdata >=0.2.5
 	ewoksjob
 server = 
 	blissdata >=0.2.5
 	ewoksjob
-id22 = 
+id01 = 
+	%(client)s
+bm02 = 
 	%(client)s
 id09 = 
 	%(client)s
-id31 = 
+id11 = 
 	%(client)s
-bm02 = 
+id12 = 
 	%(client)s
-id11 = 
+id13 = 
 	%(client)s
 id14 = 
 	%(client)s
-streamline = 
+id22 = 
 	%(client)s
 bm23 = 
 	%(client)s
 	silx >=1.1.0
 id24 = 
 	%(client)s
 	silx >=1.1.0
+id31 = 
+	%(client)s
+streamline = 
+	%(client)s
 democlient = 
 	%(client)s
 demoworker = 
 	%(server)s
 	ewoksjob[blissworker] >=0.2.1
 	ewoksxrpd >=0.3
 	est[full]
 	orange3
 test = 
 	pytest >=7
 	mock
 	pytest-mock
 	pytest-redis
+	scipy
 	%(client)s
 	%(server)s
 	%(id22)s
 	%(id11)s
 	%(id31)s
 	%(streamline)s
 	%(bm23)s
```

### Comparing `blissoda-0.3.1/src/blissoda/__init__.py` & `blissoda-0.4.0/src/blissoda/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.3.1"
+__version__ = "0.4.0"
 
 try:
     from gevent.monkey import is_anything_patched
     from gevent.monkey import is_module_patched
 except ImportError:
     pass
 else:
```

### Comparing `blissoda-0.3.1/src/blissoda/app/__main__.py` & `blissoda-0.4.0/src/blissoda/app/__main__.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/app/cli_log_utils.py` & `blissoda-0.4.0/src/blissoda/app/cli_log_utils.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/app/workflow_server/__init__.py` & `blissoda-0.4.0/src/blissoda/app/workflow_server/__init__.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/app/workflow_server/subscriberv0.py` & `blissoda-0.4.0/src/blissoda/app/workflow_server/subscriberv0.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/app/workflow_server/subscriberv1.py` & `blissoda-0.4.0/src/blissoda/app/workflow_server/subscriberv1.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/app/workflow_server/subscribervid31.py` & `blissoda-0.4.0/src/blissoda/app/workflow_server/subscribervid31.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/bm02/xrpd_processor.py` & `blissoda-0.4.0/src/blissoda/bm02/xrpd_processor.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/bm23/exafs_plotter.py` & `blissoda-0.4.0/src/blissoda/bm23/exafs_plotter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+from typing import Optional
+
 from ..exafs.plotter import ExafsPlotter
 
 
 class Bm23ExafsPlotter(ExafsPlotter):
     def __init__(self, **defaults) -> None:
         defaults.setdefault("workflow", "/users/opd23/ewoks/online.ows")
-        defaults.setdefault("_scan_type", "cont")
+        defaults.setdefault("_scan_type", "trigscan")
         counters = defaults.setdefault("_counters", dict())
         counters.setdefault(
             "cont",
             {
                 "mu_name": "mu_trans",
                 "energy_name": "energy_cenc",
                 "energy_unit": "keV",
@@ -18,14 +20,24 @@
             "step",
             {
                 "mu_name": "mu_trans",
                 "energy_name": "eneenc",
                 "energy_unit": "keV",
             },
         )
+        counters.setdefault(
+            "trigscan",
+            {
+                "mu_name": "mu_trans",
+                "energy_name": "energy_enc",
+                "energy_unit": "keV",
+            },
+        )
         super().__init__(**defaults)
 
-    def _scan_type_from_scan(self, scan) -> str:
-        if "exafs_step" in scan.name:
+    def _scan_type_from_scan(self, scan) -> Optional[str]:
+        if "exafs_step" in getattr(scan, "name", None):
             return "step"
-        else:
+        elif "exafs_cont" in getattr(scan, "name", None):
             return "cont"
+        elif "trigscan" in getattr(scan, "_scan_name", None):
+            return "trigscan"
```

### Comparing `blissoda-0.3.1/src/blissoda/demo/exafs.py` & `blissoda-0.4.0/src/blissoda/demo/exafs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import os
+from typing import Optional
 
 try:
-    from pint import UnitRegistry
     from bliss import setup_globals
+    from bliss.physics import units
 except ImportError:
-    ureg = None
+    units = None
     setup_globals = None
-else:
-    ureg = UnitRegistry()
 
 from ..exafs.plotter import ExafsPlotter
 from ..resources.exafs import RESOURCE_ROOT
 
 
 class DemoExafsPlotter(ExafsPlotter):
     def __init__(self, **defaults) -> None:
@@ -25,31 +24,33 @@
                 "mu_name": "mu",
                 "energy_name": "energy",
                 "energy_unit": energy_unit,
             },
         )
         super().__init__(**defaults)
 
-    def _scan_type_from_scan(self, scan) -> str:
+    def _scan_type_from_scan(self, scan) -> Optional[str]:
         return "any"
 
     def run(self, expo=0.003):
-        e0 = 8800
-        e1 = 9600
-        step_size = 0.5
+        e0 = 8800  # eV
+        e1 = 9600  # eV
+        step_size = 0.5  # eV
         intervals = int((e1 - e0) / step_size) - 1
 
         from_unit = "eV"
         to_unit = self.counters["energy_unit"]
 
-        if ureg:
-            e0 = (e0 * ureg(from_unit)).to(to_unit).magnitude
-            e1 = (e1 * ureg(from_unit)).to(to_unit).magnitude
+        if units:
+            e0 = (e0 * units.ur(from_unit)).to(to_unit).magnitude
+            e1 = (e1 * units.ur(from_unit)).to(to_unit).magnitude
         else:
-            assert from_unit == to_unit, "counters energy unit is wrong"
+            assert (
+                from_unit == to_unit
+            ), f"counters energy unit is '{to_unit}' instead of 'eV'"
 
         scan = setup_globals.ascan(
             setup_globals.energy, e0, e1, intervals, expo, setup_globals.mu, run=False
         )
         super().run(scan)
```

### Comparing `blissoda-0.3.1/src/blissoda/demo/example.py` & `blissoda-0.4.0/src/blissoda/demo/example.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/demo/id11.py` & `blissoda-0.4.0/src/blissoda/demo/id11.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/demo/id14.py` & `blissoda-0.4.0/src/blissoda/demo/id14.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from pprint import pprint
-from typing import Optional
 
 try:
     from bliss import setup_globals
 except ImportError:
     setup_globals = None
 
 from ..id14.converter import Id14Hdf5ToSpecConverter
 
 
 class DemoId14Hdf5ToSpecConverter(Id14Hdf5ToSpecConverter):
-    def on_new_scan_metadata(self, scan) -> Optional[dict]:
+    def on_new_scan_metadata(self, scan) -> None:
         kwargs = self.get_submit_arguments(scan)
         print("Workflow", self.workflow)
         print(" -> arguments")
         pprint(kwargs)
 
 
 if setup_globals is None:
```

### Comparing `blissoda-0.3.1/src/blissoda/demo/id22.py` & `blissoda-0.4.0/src/blissoda/demo/id22.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,22 +15,31 @@
 from .calib import DEFAULT_CALIB
 from ..id22.stscan_processor import StScanProcessor
 from ..id22.xrpd_processor import Id22XrpdProcessor
 from ..utils import directories
 
 
 class DemoStScanProcessor(StScanProcessor):
-    def __init__(self) -> None:
+    def __init__(self, **defaults) -> None:
         root_dir = directories.get_processed_dir(current_session.scan_saving.filename)
         root_dir = os.path.join(root_dir, "accessible", "id22", "config")
-        super().__init__(
-            _convert_workflow=os.path.join(root_dir, "convert.json"),
-            _rebinsum_workflow=os.path.join(root_dir, "rebinsum.json"),
-            _extract_workflow=os.path.join(root_dir, "extract.json"),
+
+        defaults.setdefault(
+            "_convert_workflow",
+            os.path.join(root_dir, "convert.json"),
+        )
+        defaults.setdefault(
+            "_rebinsum_workflow",
+            os.path.join(root_dir, "rebinsum.json"),
+        )
+        defaults.setdefault(
+            "_extract_workflow",
+            os.path.join(root_dir, "extract.json"),
         )
+        super().__init__(**defaults)
 
     def _submit_job(self, workflow, inputs, convert_destination, **kw):
         print("\nSubmit workfow")
         print(workflow)
         print("Inputs:")
         pprint(inputs)
         print("Save for provenance:")
```

### Comparing `blissoda-0.3.1/src/blissoda/demo/user_scripts/all.py` & `blissoda-0.4.0/src/blissoda/demo/user_scripts/all.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,59 +4,67 @@
 
 from blissoda.bm23.exafs_plotter import Bm23ExafsPlotter
 from blissoda.bm02.xrpd_processor import Bm02XrpdProcessor
 from blissoda.id11.xrpd_processor import Id11XrpdProcessor
 from blissoda.id22.xrpd_processor import Id22XrpdProcessor
 from blissoda.id31.xrpd_processor import Id31XrpdProcessor
 from blissoda.id14.converter import Id14Hdf5ToSpecConverter
+from blissoda.id12.converter import Id12Hdf5ToAsciiConverter
 from blissoda.id31.streamline_scanner import Id31StreamlineScanner
 
 from blissoda.demo.exafs import exafs_plotter
 from blissoda.demo.xrpd import xrpd_processor
 from blissoda.demo.id22 import stscan_processor
 from blissoda.demo.id22 import id22_xrpd_processor
 from blissoda.demo.id11 import id11_xrpd_processor
 from blissoda.demo.id14 import id14_converter
+from blissoda.demo.id12 import id12_converter
 from blissoda.demo.streamline import streamline_scanner
 
 from blissoda.demo.user_scripts.exafs import exafs_demo
 from blissoda.demo.user_scripts.id22 import id22_stscan_demo
 from blissoda.demo.user_scripts.id22 import id22_xrpd_demo
 from blissoda.demo.user_scripts.streamline import streamline_demo
 from blissoda.demo.user_scripts.xrpd import xrpd_demo
 from blissoda.demo.user_scripts.id11 import id11_pdf_demo  # noqa F401
 from blissoda.demo.user_scripts.id14 import id14_demo
+from blissoda.demo.user_scripts.id12 import id12_demo
 
 try:
     from bliss import setup_globals
 except ImportError:
     setup_globals = None
 
 
 def all_print():
     _print_objects(exafs_plotter)
     _print_objects(xrpd_processor)
     _print_objects(id11_xrpd_processor)
     _print_objects(id22_xrpd_processor)
     _print_objects(id14_converter)
+    _print_objects(id12_converter)
     _print_objects(stscan_processor)
     _print_objects(streamline_scanner)
 
     _print_objects(XrpdProcessor())
     _print_objects(ExafsPlotter())
     _print_objects(StreamlineScanner())
     _print_objects(Bm23ExafsPlotter())
     _print_objects(Bm02XrpdProcessor())
     _print_objects(Id11XrpdProcessor())
     _print_objects(Id22XrpdProcessor())
     _print_objects(Id31XrpdProcessor())
     _print_objects(Id14Hdf5ToSpecConverter())
+    _print_objects(Id12Hdf5ToAsciiConverter())
 
     _print_objects(Id31StreamlineScanner())
 
+    print()
+    print("SUCCESS: all objects can be printed")
+
 
 def all_demo():
     print()
     print("===================")
     setup_globals.newcollection("exafs_collection")
     exafs_demo()
 
@@ -89,15 +97,23 @@
     print()
     print("===================")
     setup_globals.newcollection("id14_collection")
     id14_demo()
 
     print()
     print("===================")
+    setup_globals.newcollection("id12_collection")
+    id12_demo()
+
+    print()
+    print("===================")
     setup_globals.newcollection("done_collection")
 
+    print()
+    print("SUCCESS: all demos can be executed")
+
 
 def _print_objects(obj):
     print()
     print("===================")
     print(obj._parameters.name)
     print(obj.__info__())
```

### Comparing `blissoda-0.3.1/src/blissoda/demo/user_scripts/id11.py` & `blissoda-0.4.0/src/blissoda/demo/user_scripts/id11.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/demo/user_scripts/id22.py` & `blissoda-0.4.0/src/blissoda/demo/user_scripts/id22.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/demo/user_scripts/streamline.py` & `blissoda-0.4.0/src/blissoda/demo/user_scripts/streamline.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from blissoda.demo.streamline import streamline_sc
 from blissoda.demo.streamline import streamline_scanner
 
 
-def streamline_demo(with_calibration=False):
+def streamline_demo(with_autocalibration=False):
     # Nothing loaded and 2 holders in the tray:
     streamline_scanner.eject()
     streamline_sc.fill_tray(2)
 
     # Initialize workflow with or without calibration
-    streamline_scanner.init_workflow(with_calibration=with_calibration)
-    if with_calibration:
+    streamline_scanner.init_workflow(with_autocalibration=with_autocalibration)
+    if with_autocalibration:
         streamline_scanner.calib(0.1)
 
     # Measure all holders
     streamline_scanner.run(0.1)
```

### Comparing `blissoda-0.3.1/src/blissoda/demo/user_scripts/xrpd.py` & `blissoda-0.4.0/src/blissoda/demo/user_scripts/xrpd.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/demo/xrpd.py` & `blissoda-0.4.0/src/blissoda/demo/xrpd.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/exafs/plots.py` & `blissoda-0.4.0/src/blissoda/exafs/plots.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/exafs/plotter.py` & `blissoda-0.4.0/src/blissoda/exafs/plotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,24 +99,28 @@
     def energy_unit(self) -> Optional[str]:
         return self.counters.get("energy_unit")
 
     @energy_unit.setter
     def energy_unit(self, value):
         self.counters["energy_unit"] = value
 
-    def _scan_type_from_scan(self, scan) -> str:
+    def _scan_type_from_scan(self, scan) -> Optional[str]:
         raise NotImplementedError
 
     def run(self, scan, filename=None, **kw):
         if not self.enabled:
             scan.run()
             return
 
         self.scan_type = self._scan_type_from_scan(scan)
 
+        if not self.scan_type:
+            scan.run()
+            return
+
         if filename is None:
             try:
                 filename = scan.writer.get_filename()
             except AttributeError:
                 # bliss < 1.0.0
                 filename = scan.writer.filename
         if os.path.exists(filename):
@@ -138,21 +142,25 @@
             scan.run(**kw)
         finally:
             try:
                 try:
                     if not update_loop:
                         update_loop.get()
                     update_loop.kill()
-                    self._submit_and_plot(scan_id)
+                    gevent.spawn(self._last_submit_and_plot, scan_id)
                 finally:
                     self._removed_failed_processing()
                     self._purge_plots()
             except Exception:
                 logger.warning("Post-scan update failed", exc_info=True)
 
+    def _last_submit_and_plot(self, *args, **kw):
+        gevent.sleep(1)
+        self._submit_and_plot(*args, **kw)
+
     def clear(self):
         """Remove all scan curves in all plots"""
         self._get_plot().clear()
 
     def refresh(self):
         """Refresh all plots with the current processed data"""
         for scan_id in self._scans:
```

### Comparing `blissoda-0.3.1/src/blissoda/exafs/widgets.py` & `blissoda-0.4.0/src/blissoda/exafs/widgets.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/flint/__init__.py` & `blissoda-0.4.0/src/blissoda/flint/__init__.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/id09/xrpd_processor.py` & `blissoda-0.4.0/src/blissoda/id09/xrpd_processor.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/id11/xrpd_processor.py` & `blissoda-0.4.0/src/blissoda/id11/xrpd_processor.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/id14/converter.py` & `blissoda-0.4.0/src/blissoda/id14/converter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """User API for HDF5 conversion on the Bliss repl"""
 
 import os
-from typing import Optional, List, Dict
+from typing import List, Dict
 
 from ewoksjob.client import submit
 
 try:
     from bliss import current_session
 except ImportError:
     current_session = None
@@ -52,15 +52,15 @@
     def _sync_scan_metadata(self) -> None:
         if self._enabled:
             workflows_category = trigger.register_workflow_category()
             workflows_category.set("processing", self.on_new_scan_metadata)
         else:
             trigger.unregister_workflow_category()
 
-    def on_new_scan_metadata(self, scan) -> Optional[dict]:
+    def on_new_scan_metadata(self, scan) -> None:
         if not self.scan_requires_processing(scan):
             return
         kwargs = self.get_submit_arguments(scan)
         _ = submit(args=(self.workflow,), kwargs=kwargs, queue=self.worker)
 
     def scan_requires_processing(self, scan) -> bool:
         # TODO: select scan that needs processing
@@ -75,14 +75,18 @@
     def get_inputs(self, scan) -> List[dict]:
         task_identifier = "Hdf5ToSpec"
 
         filename = self.get_filename(scan)
         output_filename = self.workflow_destination(scan)
         scan_nb = scan.scan_info.get("scan_nb")
 
+        # Scan metadata published in id14.McaAcq.McaAcq.save
+        calibration = scan.scan_info["instrument"]["calibration"]
+        mca_calibration = calibration["a"], calibration["b"], 0
+
         return [
             {
                 "task_identifier": task_identifier,
                 "name": "filename",
                 "value": filename,
             },
             {
@@ -91,14 +95,19 @@
                 "value": output_filename,
             },
             {
                 "task_identifier": task_identifier,
                 "name": "scan_numbers",
                 "value": [scan_nb],
             },
+            {
+                "task_identifier": task_identifier,
+                "name": "mca_calibration",
+                "value": mca_calibration,
+            },
         ]
 
     def get_filename(self, scan) -> str:
         filename = scan.scan_info.get("filename")
         if filename:
             return filename
         return current_session.scan_saving.filename
```

### Comparing `blissoda-0.3.1/src/blissoda/id22/stscan_processor.py` & `blissoda-0.4.0/src/blissoda/id22/stscan_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -817,16 +817,16 @@
             {"name": "delta2theta", "value": 0.003},
             {"name": "startp", "value": 31},
             {"name": "device", "value": 0},
             {
                 "name": "outdirs",
                 "value": {
                     "primary": "opid22@diffract22new:/users/opid22/data1/",
-                    # "secondary": "opid22@diffract22bliss:/users/opid22/data1/",
-                    "backup": "opid22@diffract22bliss:/data/id22/backup/data22/",
+                    # "secondary": "opid22@lid22bliss:/users/opid22/data1/",
+                    "backup": "opid22@lid22bliss:/data/id22/backup/data22/",
                 },
             },
             {"name": "retry_timeout", "value": 30},
         ]
 
     def _add_convertrebin_inputs(self, inputs: list, primary_outdir: str):
         if self.convert_include_proposal_outdir:
@@ -837,16 +837,16 @@
     def _add_convertrebin_default_inputs(self, workflow: dict):
         node_attrs = self._get_node_attrs(workflow, "convert")
         node_attrs["default_inputs"] = [
             {
                 "name": "outdirs",
                 "value": {
                     "primary": "opid22@diffract22new:/users/opid22/data1/",
-                    # "secondary": "opid22@diffract22bliss:/users/opid22/data1/",
-                    "backup": "opid22@diffract22bliss:/data/id22/backup/data22/",
+                    # "secondary": "opid22@lid22bliss:/users/opid22/data1/",
+                    "backup": "opid22@lid22bliss:/data/id22/backup/data22/",
                 },
             },
             {"name": "retry_timeout", "value": 30},
             {"name": "ascii_extension", "value": ".adv"},
         ]
 
     def _add_sum_inputs(self, inputs: list, primary_outdir: str):
@@ -881,16 +881,16 @@
     def _add_convert_default_inputs(self, workflow: dict):
         node_attrs = self._get_node_attrs(workflow, "convert")
         node_attrs["default_inputs"] = [
             {
                 "name": "outdirs",
                 "value": {
                     "primary": "opid22@diffract22new:/users/opid22/data1/",
-                    # "secondary": "opid22@diffract22bliss:/users/opid22/data1/",
-                    "backup": "opid22@diffract22bliss:/data/id22/backup/data22/",
+                    # "secondary": "opid22@lid22bliss:/users/opid22/data1/",
+                    "backup": "opid22@lid22bliss:/data/id22/backup/data22/",
                 },
             },
             {"name": "retry_timeout", "value": 30},
         ]
 
     def _add_extract_inputs(self, inputs: list, outprefix: str, primary_outdir: str):
         if self.extract_include_proposal_outdir:
```

### Comparing `blissoda-0.3.1/src/blissoda/id22/xrpd_processor.py` & `blissoda-0.4.0/src/blissoda/id22/xrpd_processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,15 +55,14 @@
         return inputs
 
     def get_sum_inputs(self, scan, lima_name: str):
         task_identifier = "SumBlissScanImages"
 
         filename = self.get_filename(scan)
         scan_nb = scan.scan_info.get("scan_nb")
-        tscan_info = scan.scan_info["tscan_info"]
 
         inputs = [
             {
                 "task_identifier": task_identifier,
                 "name": "filename",
                 "value": filename,
             },
@@ -78,25 +77,28 @@
                 "value": scan_nb,
             },
             {
                 "task_identifier": task_identifier,
                 "name": "detector_name",
                 "value": lima_name,
             },
-            {
-                "task_identifier": task_identifier,
-                "name": "skip_dark",
-                "value": tscan_info["save_background"],
-            },
-            {
-                "task_identifier": task_identifier,
-                "name": "background_step",
-                "value": tscan_info["background_step"],
-            },
         ]
+
+        tscan_info = scan.scan_info.get("tscan_info")
+        if tscan_info:
+            background_step = tscan_info.get("background_step")
+            if background_step is not None:
+                inputs.append(
+                    {
+                        "task_identifier": task_identifier,
+                        "name": "background_step",
+                        "value": background_step,
+                    }
+                )
+
         if self.data_from_memory:
             scan_memory_url = f"{scan.root_node.db_name}:{scan._node_name}"
             inputs.append(
                 {
                     "task_identifier": task_identifier,
                     "name": "scan_memory_url",
                     "value": scan_memory_url,
```

### Comparing `blissoda-0.3.1/src/blissoda/id24/exafs_plotter.py` & `blissoda-0.4.0/src/blissoda/id24/exafs_plotter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional
+
 try:
     from bliss import setup_globals
 except ImportError:
     setup_globals = None
 
 from ..exafs.plotter import ExafsPlotter
 
@@ -17,12 +19,12 @@
                 "mu_name": "mu_trans",
                 "energy_name": "energy_enc",
                 "energy_unit": "keV",
             },
         )
         super().__init__(**defaults)
 
-    def _scan_type_from_scan(self, scan) -> str:
+    def _scan_type_from_scan(self, scan) -> Optional[str]:
         return "escan"
 
     def run(self, scan, **kw):
         super().run(scan, filename=setup_globals.SCAN_SAVING.filename, **kw)
```

### Comparing `blissoda-0.3.1/src/blissoda/id31/xrpd_processor.py` & `blissoda-0.4.0/src/blissoda/id31/xrpd_processor.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/persistent/ndarray/__init__.py` & `blissoda-0.4.0/src/blissoda/persistent/ndarray/__init__.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/persistent/ndarray/ndarrayv0.py` & `blissoda-0.4.0/src/blissoda/persistent/ndarray/ndarrayv0.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/persistent/ndarray/ndarrayv1.py` & `blissoda-0.4.0/src/blissoda/persistent/ndarray/ndarrayv1.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/persistent/ordereddict.py` & `blissoda-0.4.0/src/blissoda/persistent/ordereddict.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/persistent/parameters.py` & `blissoda-0.4.0/src/blissoda/persistent/parameters.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/resources/demo/background.xy` & `blissoda-0.4.0/src/blissoda/resources/demo/background.xy`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/resources/exafs/exafs.ows` & `blissoda-0.4.0/src/blissoda/resources/exafs/exafs.ows`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/resources/id11/integrate_scan_with_saving.json` & `blissoda-0.4.0/src/blissoda/resources/id11/integrate_scan_with_saving.json`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/resources/id11/integrate_scan_with_saving_pdf.json` & `blissoda-0.4.0/src/blissoda/resources/id11/integrate_scan_with_saving_pdf.json`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/resources/id11/integrate_scan_without_saving.json` & `blissoda-0.4.0/src/blissoda/resources/id11/integrate_scan_without_saving.json`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/resources/id22/Sum_then_integrate_with_saving.json` & `blissoda-0.4.0/src/blissoda/resources/id22/Sum_then_integrate_with_saving.json`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/resources/streamline/reprocess.py` & `blissoda-0.4.0/src/blissoda/resources/streamline/reprocess.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/resources/streamline/streamline_with_calib.json` & `blissoda-0.4.0/src/blissoda/resources/streamline/streamline_with_calib.json`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/resources/streamline/streamline_without_calib.json` & `blissoda-0.4.0/src/blissoda/resources/streamline/streamline_without_calib.json`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/resources/streamline/time_record.py` & `blissoda-0.4.0/src/blissoda/resources/streamline/time_record.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/resources/xrpd/integrate_scan_with_saving.json` & `blissoda-0.4.0/src/blissoda/resources/xrpd/integrate_scan_with_saving.json`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/resources/xrpd/integrate_scan_without_saving.json` & `blissoda-0.4.0/src/blissoda/resources/xrpd/integrate_scan_without_saving.json`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/seslab/streamline_scanner.py` & `blissoda-0.4.0/src/blissoda/seslab/streamline_scanner.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 class StreamlineSesScanner(StreamlineScanner):
     def __init__(self, **defaults):
         defaults.setdefault("sample_changer_name", "streamline_sc")
         super().__init__(**defaults)
 
-    def measure_sample(self, *args, **kwargs):
+    def measure_sample(self, *args, has_qrcode: bool = True, **kwargs):
         return None
 
     def _get_calibration(self):
         return {"non_empty": None}
 
     def _newsample(self, sample_name: str):
         print("NEW SAMPLE:", sample_name)
```

### Comparing `blissoda-0.3.1/src/blissoda/streamline/scanner.py` & `blissoda-0.4.0/src/blissoda/streamline/scanner.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 """
 
 import os
 import re
 import shutil
 from numbers import Number
 from contextlib import contextmanager
-from typing import Optional, NamedTuple, Tuple, Dict
+from typing import Optional, NamedTuple, Tuple, Dict, Generator
+
 import numpy
 
 try:
     from bliss import current_session
     from bliss import setup_globals
     from bliss.common.logtools import elog_print
 except ImportError:
@@ -48,28 +49,35 @@
 class StreamlineScanner(
     WithPersistentParameters,
     parameters=[
         ParameterInfo("workflow", category="data processing"),
         ParameterInfo("sample_changer_name", category="names"),
         ParameterInfo("detector_name", category="names"),
         ParameterInfo("energy_name", category="names"),
-        ParameterInfo("calibrations", category="calibration"),
+        ParameterInfo("calibration_scans", category="calibration"),
         ParameterInfo("calibration_motor", category="calibration"),
         ParameterInfo("image_slice", category="PyFai"),
         ParameterInfo("integration_options", category="PyFai"),
         ParameterInfo("pyfai_config", category="PyFai"),
         ParameterInfo("calibrant", category="calibration"),
         ParameterInfo("trigger_workflows", category="data processing"),
         ParameterInfo("vibration_speed_during_scan", category="sample changer"),
+        ParameterInfo("verify_qrcode", category="robust vs. speed"),
+        ParameterInfo("autotune_qrreader_per", category="robust vs. speed"),
+        ParameterInfo("dryrun", category="testing"),
+        ParameterInfo("calib_ring_detector_name", category="calibration"),
     ],
 ):
     def __init__(self, **defaults) -> None:
         defaults.setdefault("image_slice", 0)
         defaults.setdefault("trigger_workflows", True)
         defaults.setdefault("vibration_speed_during_scan", 40)
+        defaults.setdefault("dryrun", False)
+        defaults.setdefault("verify_qrcode", False)
+        defaults.setdefault("autotune_qrreader_per", "baguette")
         super().__init__(**defaults)
 
     def _info_categories(self) -> Dict[str, dict]:
         categories = super()._info_categories()
         try:
             sample_changer = self.sample_changer
         except (AttributeError, KeyError):
@@ -84,16 +92,29 @@
         }
         if self.workflow_has_calib:
             categories["status"]["calibration"] = self._get_calibration().get("image")
         if self.workflow_has_flatfield:
             categories["status"]["flat-field"] = "ON"
         return categories
 
-    def measure_sample(self, *args, **kwargs):
-        return setup_globals.sct(*args, **kwargs)
+    @property
+    def autotune_qrreader_per(self) -> Optional[str]:
+        return self._get_parameter("autotune_qrreader_per")
+
+    @autotune_qrreader_per.setter
+    def autotune_qrreader_per(self, value: Optional[str]):
+        if value not in (None, "sample", "baguette"):
+            raise ValueError("Allowed values are 'sample', 'baguette' or None")
+        self._set_parameter("autotune_qrreader_per", value)
+
+    def measure_sample(self, *args, has_qrcode: bool = True, **kwargs):
+        if self.dryrun:
+            print("Dry-run: skip measurement")
+        else:
+            return setup_globals.sct(*args, **kwargs)
 
     @property
     def sample_changer(self):
         self._raise_when_missing("sample_changer_name")
         return current_session.env_dict[self.sample_changer_name]
 
     def eject(self):
@@ -103,26 +124,33 @@
             "\n\nNumber of remaining sample holders:",
             self.sample_changer.number_of_remaining_baguettes,
         )
 
     def load(self):
         self.sample_changer.translation.on()
         self.sample_changer.load_baguette_with_homing()
+        if self.autotune_qrreader_per == "baguette":
+            self.tune_qrreader_for_baguette()
 
     def run(
         self,
         *scan_args,
         nholders: Optional[int] = None,
         use_qr_code: bool = True,
         current_holder: bool = False,
         sample_indices: Optional[Tuple[int]] = None,
         **scan_kwargs,
     ):
         if self.workflow_has_calib and not self._get_calibration():
             raise RuntimeError("measure a calibration standard first")
+        if self.trigger_workflows:
+            if not self.workflow:
+                raise RuntimeError("initialize a workflow first")
+            if self.pyfai_config and not os.path.exists(self.pyfai_config):
+                raise RuntimeError("the pyFAI configuration file no longer exists")
 
         with self.run_context():
             if current_holder:
                 self.load()
                 self._run_holder(
                     scan_args,
                     scan_kwargs,
@@ -159,39 +187,53 @@
         use_qr_code: bool = True,
         sample_indices: Optional[Tuple[int]] = None,
     ):
         if use_qr_code:
             itfunc = self.sample_changer.iterate_samples
         else:
             itfunc = self.sample_changer.iterate_samples_without_qr
-        for qrcode in itfunc(sample_indices=sample_indices):
+
+        print("")
+        print("========== RUN HOLDER ==========")
+        for qrcode in itfunc(
+            sample_indices=sample_indices,
+            autoTuningAllowed=self.autotune_qrreader_per == "sample",
+        ):
+            print()
             self._process_sample(qrcode, scan_args, scan_kwargs)
+        print("================================")
 
     def calib(
         self,
         *scan_args,
         sample_index: Optional[int] = None,
         use_qr_code: bool = True,
         **scan_kwargs,
     ):
         if sample_index is None:
             raise ValueError("argument 'sample_index' not provided")
         with self.run_context():
-            if use_qr_code:
-                qrcode = self.sample_changer.select_sample(sample_index)
-            else:
-                qrcode = self.sample_changer.select_sample_without_qr(sample_index)
+            qrcode = self._select_sample(sample_index, use_qr_code=use_qr_code)
             self._process_sample(qrcode, scan_args, scan_kwargs, is_calibration=True)
 
-    def select_sample(self, sample_index: int):
+    def select_sample(self, sample_index: int, use_qr_code: bool = True) -> str:
         self.sample_changer.translation.on()
-        return self.sample_changer.select_sample(sample_index)
+        return self._select_sample(sample_index, use_qr_code=use_qr_code)
 
-    def init_workflow(self, with_calibration: bool = False):
-        if with_calibration:
+    def _select_sample(self, sample_index: int, use_qr_code: bool = True) -> str:
+        if use_qr_code:
+            select_sample = self.sample_changer.select_sample
+        else:
+            select_sample = self.sample_changer.select_sample_without_qr
+        return select_sample(
+            sample_index, autoTuningAllowed=self.autotune_qrreader_per == "sample"
+        )
+
+    def init_workflow(self, with_autocalibration: bool = False):
+        if with_autocalibration:
             basename = "streamline_with_calib"
         else:
             basename = "streamline_without_calib"
         filename = f"{basename}.json"
 
         dirname = self._get_workflows_dirname(current_session.scan_saving.filename)
         destination = os.path.join(dirname, filename)
@@ -216,17 +258,17 @@
             print("Cannot use as calibration because no data was collected")
             return
         info = {
             "image": self._get_image_url(scan_info),
             "gallery_directory": self._get_gallery_directory(scan_info.filename),
         }
         position = self._get_calibration_position()
-        if self.calibrations is None:
-            self.calibrations = dict()
-        self.calibrations[position] = info
+        if self.calibration_scans is None:
+            self.calibration_scans = dict()
+        self.calibration_scans[position] = info
 
     def _trigger_processing(self, scan_info: ScanInfo, processed_metadata: dict):
         if not scan_info.filename:
             print("Cannot trigger workflow because no data was collected")
             return
         args, kwargs = self._job_arguments(scan_info, processed_metadata)
         submit(args=args, kwargs=kwargs)
@@ -245,53 +287,92 @@
     def _process_sample(
         self,
         qrcode: str,
         scan_args: tuple,
         scan_kwargs: dict,
         is_calibration: bool = False,
     ):
-        qrcode2 = self.sample_changer.qr_read()
-        if qrcode2 != qrcode and qrcode2 != "ERROR":
+        try:
+            with self._verify_qrcode(qrcode) as qrcode:
+                has_qrcode = qrcode != self._qrcode_error
+                self._newsample(qrcode)
+
+                self._set_scan_metadata(scan_args, scan_kwargs)
+                self._set_raw_dataset_metadata(scan_args, scan_kwargs)
+
+                scan = self.measure_sample(
+                    *scan_args, has_qrcode=has_qrcode, **scan_kwargs
+                )
+
+                scan_info = self._get_scan_info(scan)
+                if is_calibration:
+                    self._set_calibration_scan(scan_info)
+
+                if self.trigger_workflows:
+                    processed_metadata = self._get_processed_dataset_metadata(scan_args)
+                    if self.dryrun:
+                        print("Dry-run: skip workflow triggering")
+                    else:
+                        self._trigger_processing(scan_info, processed_metadata)
+
+                if is_calibration:
+                    elog_print(
+                        f"Streamline calibrant {self.calibrant}: {current_session.scan_saving.filename}"
+                    )
+        finally:
+            setup_globals.enddataset()
+
+    def qr_read(self) -> str:
+        return self.sample_changer.qr_read(
+            autoTuningAllowed=self.autotune_qrreader_per == "sample"
+        )
+
+    @property
+    def _qrcode_error(self) -> str:
+        return self.sample_changer.qrreader.QRCODE_NOT_READABLE
+
+    def tune_qrreader(self, force=False) -> str:
+        self.sample_changer.tune_qrreader(force=force)
+
+    def tune_qrreader_for_baguette(self) -> None:
+        for _ in self.sample_changer.iterate_samples_without_qr():
+            qrcode = self.tune_qrreader()
+            if qrcode != self._qrcode_error:
+                break
+        else:
+            print("QR-reader tuning failed when loading the baguette")
+
+    @contextmanager
+    def _verify_qrcode(self, qrcode: str) -> Generator[str, None, None]:
+        """Check the QR-code before (yields the new code when it changed)
+        and check the QR-code after (raises and exception when it changed)"""
+        if not self.verify_qrcode:
+            yield qrcode
+            return
+
+        qrcode_now = self.qr_read()
+        if qrcode_now != qrcode and qrcode_now != self._qrcode_error:
             print(
-                f"Reading the QR-code twice gives first '{qrcode}' and then '{qrcode2}'"
+                f"Reading the QR-code twice gives first '{qrcode}' and then '{qrcode_now}'"
             )
-            qrcode = qrcode2
-        self._newsample(qrcode)
+            qrcode = qrcode_now
         try:
-            self._set_scan_metadata(scan_args, scan_kwargs)
-            self._set_raw_dataset_metadata(scan_args, scan_kwargs)
-            scan = self.measure_sample(*scan_args, **scan_kwargs)
-            scan_info = self._get_scan_info(scan)
-            if is_calibration:
-                self._set_calibration_scan(scan_info)
-            if self.trigger_workflows:
-                processed_metadata = self._get_processed_dataset_metadata(scan_args)
-                self._trigger_processing(scan_info, processed_metadata)
-            if is_calibration:
-                elog_print(
-                    f"Streamline calibrant {self.calibrant}: {current_session.scan_saving.filename}"
-                )
+            yield qrcode
         finally:
-            try:
-                qrcode2 = self.sample_changer.qr_read()
-                if qrcode2 != qrcode and qrcode2 != "ERROR":
-                    if qrcode == "ERROR":
-                        msg = f"The sample name of dataset '{current_session.scan_saving.filename}' is '{qrcode2}' (read at the end of the dataset)"
-                        elog_print(msg)
-                    else:
-                        msg = f"The sample name of dataset '{current_session.scan_saving.filename}' might be '{qrcode2}' (read at the end of the dataset)"
-                        elog_print(msg)
-                        raise RuntimeError(msg)
-            finally:
-                setup_globals.enddataset()
-
-    def _newsample(self, qrcode: str):
-        qrcode = re.sub(r"\s+", "_", qrcode)
-        if qrcode == "ERROR":
-            qrcode = "UNKNOWN"
+            qrcode_now = self.qr_read()
+            if qrcode_now != qrcode and qrcode_now != self._qrcode_error:
+                if qrcode == self._qrcode_error:
+                    msg = f"The sample name of dataset '{current_session.scan_saving.filename}' is '{qrcode_now}' (read at the end of the dataset)"
+                    elog_print(msg)
+                else:
+                    msg = f"The sample name of dataset '{current_session.scan_saving.filename}' might be '{qrcode_now}' (read at the end of the dataset)"
+                    elog_print(msg)
+                    raise RuntimeError(msg)
+
+    def _newsample(self, qrcode: str) -> None:
         setup_globals.newsample(qrcode)
         setup_globals.newdataset()
 
     def _set_raw_dataset_metadata(self, scan_args: tuple, scan_kwargs: dict) -> None:
         for k, v in self._get_raw_dataset_metadata(scan_args).items():
             current_session.scan_saving.dataset[k] = v
 
@@ -325,24 +406,24 @@
         return metadata
 
     def _get_calibration_position(self) -> Optional[Number]:
         if self.calibration_motor:
             return getattr(setup_globals, self.calibration_motor).position
 
     def _get_calibration(self) -> dict:
-        calibrations = self.calibrations
-        if not calibrations:
+        calibration_scans = self.calibration_scans
+        if not calibration_scans:
             return dict()
         position = self._get_calibration_position()
         if position is not None:
-            positions = [p for p in calibrations if p is not None]
+            positions = [p for p in calibration_scans if p is not None]
             if positions:
                 idx = (numpy.abs(numpy.array(positions) - position)).argmin()
                 position = positions[idx]
-        return calibrations.get(position, dict())
+        return calibration_scans.get(position, dict())
 
     def _get_scan_info(self, scan) -> ScanInfo:
         if scan is None:
             return ScanInfo(filename="", scan_nb=0)
         if isinstance(scan, ScanInfo):
             return scan
         filename = scan.scan_info.get("filename")
@@ -374,28 +455,34 @@
         return os.path.join(
             self._get_output_dir(dataset_filename), os.path.splitext(filename)[0]
         )
 
     def _get_gallery_dirname(self, dataset_filename: str) -> str:
         return os.path.join(self._get_output_dirname(dataset_filename), "gallery")
 
-    def _get_output_filename(self, dataset_filename: str) -> str:
+    def _get_hdf5_output_filename(self, dataset_filename: str) -> str:
         return os.path.join(
             self._get_output_dirname(dataset_filename),
             os.path.basename(dataset_filename),
         )
 
+    def _get_ascii_output_filename(self, dataset_filename: str, unit: str) -> str:
+        basename, _ = os.path.splitext(os.path.basename(dataset_filename))
+        return os.path.join(
+            self._get_output_dirname(dataset_filename), f"{basename}_{unit}.xye"
+        )
+
     def _get_gallery_directory(self, dataset_filename: str) -> str:
         return self._get_gallery_dirname(dataset_filename)
 
     def _get_workflow_save_filename(self, dataset_filename: str) -> str:
         basename = os.path.basename(self.workflow)
         return os.path.join(
             self._get_output_dirname(dataset_filename),
-            os.path.splitext(basename)[0] + ".json",
+            basename,
         )
 
     def _get_workflow_upload_parameters(
         self, dataset_filename: str, processed_metadata: dict
     ) -> Optional[dict]:
         raw = os.path.dirname(dataset_filename)
         dataset = "integrate"
@@ -412,15 +499,15 @@
             "metadata": processed_metadata,
         }
 
     def _job_arguments(self, scan_info: ScanInfo, processed_metadata: dict):
         """Arguments for the workflow execution"""
         self._raise_when_missing("workflow")
         if self.workflow_has_calib:
-            self._raise_when_missing("calibrations", "calibrant")
+            self._raise_when_missing("calibration_scans", "calibrant")
 
         inputs = list()
 
         integrate_image_url = self._get_image_url(scan_info)
 
         # Configuration
         if self.integration_options:
@@ -467,23 +554,28 @@
                 },
                 {
                     "task_identifier": "CalibrateSingle",
                     "name": "robust",
                     "value": False,
                 },
                 {
+                    "task_identifier": "CalibrateSingle",
+                    "name": "ring_detector",
+                    "value": self.calib_ring_detector_name,
+                },
+                {
                     "task_identifier": "DiagnoseCalibrateSingleResults",
                     "name": "image",
                     "value": calibration["image"],
                 },
                 {
                     "task_identifier": "DiagnoseCalibrateSingleResults",
                     "name": "filename",
                     "value": os.path.join(
-                        calibration["gallery_directory"], "ring_detection.svg"
+                        calibration["gallery_directory"], "ring_detection.png"
                     ),
                 },
             ]
 
             if calibration["image"] == integrate_image_url and self.calibrant:
                 inputs += [
                     {
@@ -504,58 +596,64 @@
                 "task_identifier": "Integrate1D",
                 "name": "maximum_persistent_workers",
                 "value": 2,  # Q and 2theta
             },
             {
                 "task_identifier": "SaveNexusPattern1D",
                 "name": "url",
-                "value": self._get_output_filename(scan_info.filename),
+                "value": self._get_hdf5_output_filename(scan_info.filename),
             },
             {
                 "task_identifier": "SaveNexusPattern1D",
                 "name": "bliss_scan_url",
                 "value": scan_info.url,
             },
         ]
 
         # Different outputs depending on the unit
         detector_name = self.detector_name
         for unit in ("q", "2th"):
             inputs += [
                 {
                     "task_identifier": "SaveNexusPattern1D",
-                    "label": f"save_{unit}",
+                    "label": f"save_{unit}_hdf5",
                     "name": "nxprocess_name",
                     "value": f"{detector_name}_integrate_{unit}",
                 },
                 {
                     "task_identifier": "SaveNexusPattern1D",
-                    "label": f"save_{unit}",
+                    "label": f"save_{unit}_hdf5",
                     "name": "nxmeasurement_name",
                     "value": f"{detector_name}_integrated_{unit}",
                 },
                 {
                     "task_identifier": "SaveNexusPattern1D",
-                    "label": f"save_{unit}",
+                    "label": f"save_{unit}_hdf5",
                     "name": "metadata",
                     "value": {
                         f"{detector_name}_integrate_{unit}": {
                             "configuration": {"workflow": self.workflow}
                         }
                     },
                 },
+                {
+                    "task_identifier": "SaveAsciiPattern1D",
+                    "label": f"save_{unit}_ascii",
+                    "name": "filename",
+                    "value": self._get_ascii_output_filename(scan_info.filename, unit),
+                },
             ]
 
         inputs += [
             {
                 "task_identifier": "DiagnoseIntegrate1D",
                 "name": "filename",
                 "value": os.path.join(
                     self._get_gallery_directory(scan_info.filename),
-                    "integrate.svg",
+                    "integrate.png",
                 ),
             },
         ]
 
         # Job arguments
         args = (self.workflow,)
         convert_destination = self._get_workflow_save_filename(scan_info.filename)
```

### Comparing `blissoda-0.3.1/src/blissoda/tests/conftest.py` & `blissoda-0.4.0/src/blissoda/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/tests/mock_id31/__init__.py` & `blissoda-0.4.0/src/blissoda/tests/mock_id31/__init__.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/tests/mock_id31/controllers.py` & `blissoda-0.4.0/src/blissoda/tests/mock_id31/controllers.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/tests/mock_id31/simulate.py` & `blissoda-0.4.0/src/blissoda/tests/mock_id31/simulate.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/tests/test_id22.py` & `blissoda-0.4.0/src/blissoda/tests/test_id22.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/tests/test_id31.py` & `blissoda-0.4.0/src/blissoda/tests/test_id31.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy
 import pytest
 
 from .mock_id31 import mock_id31
 from .mock_id31 import setup_globals
-from ..id31.optimize_exposure import optimize_exposure
+from ..id31 import optimize_exposure
 
 
 @pytest.fixture
 def current_session_mock():
     with mock_id31():
         yield
 
@@ -50,17 +50,17 @@
         sublist = list()
         lst.append(sublist)
         flux = numpy.linspace(1e4, 1e6, 10)
         for fl in flux:
             setup_globals.source.rate = fl
             setup_globals.att(0)
             assert setup_globals.p3.rate == fl
-            expo_time = optimize_exposure(
+            condition = optimize_exposure.optimize_exposure_condition(
                 setup_globals.p3,
                 default_att_position=default_att_position,
                 desired_counts=1e5,
             )
-            setup_globals.ct(expo_time, setup_globals.p3)
+            setup_globals.ct(condition.expo_time, setup_globals.p3)
             sublist.append(setup_globals.atten.bits)
 
     for sublist in lst:
         assert sublist == lst[0]
```

### Comparing `blissoda-0.3.1/src/blissoda/tests/test_persistent.py` & `blissoda-0.4.0/src/blissoda/tests/test_persistent.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/utils/directories.py` & `blissoda-0.4.0/src/blissoda/utils/directories.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/utils/pyfai.py` & `blissoda-0.4.0/src/blissoda/utils/pyfai.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/utils/trigger.py` & `blissoda-0.4.0/src/blissoda/utils/trigger.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/xrpd/data.py` & `blissoda-0.4.0/src/blissoda/xrpd/data.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/xrpd/plots.py` & `blissoda-0.4.0/src/blissoda/xrpd/plots.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/xrpd/plotter.py` & `blissoda-0.4.0/src/blissoda/xrpd/plotter.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/xrpd/processor.py` & `blissoda-0.4.0/src/blissoda/xrpd/processor.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda/xrpd/widgets.py` & `blissoda-0.4.0/src/blissoda/xrpd/widgets.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.3.1/src/blissoda.egg-info/PKG-INFO` & `blissoda-0.4.0/src/blissoda.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blissoda
-Version: 0.3.1
+Version: 0.4.0
 Summary: Utilities for ewoks developers
 Home-page: https://gitlab.esrf.fr/bliss/blissoda/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/bliss/blissoda/
 Project-URL: Documentation, https://blissoda.readthedocs.io/
@@ -17,43 +17,52 @@
 License-File: LICENSE.md
 Provides-Extra: client
 Requires-Dist: blissdata>=0.2.5; extra == "client"
 Requires-Dist: ewoksjob; extra == "client"
 Provides-Extra: server
 Requires-Dist: blissdata>=0.2.5; extra == "server"
 Requires-Dist: ewoksjob; extra == "server"
-Provides-Extra: id22
-Requires-Dist: blissdata>=0.2.5; extra == "id22"
-Requires-Dist: ewoksjob; extra == "id22"
-Provides-Extra: id09
-Requires-Dist: blissdata>=0.2.5; extra == "id09"
-Requires-Dist: ewoksjob; extra == "id09"
-Provides-Extra: id31
-Requires-Dist: blissdata>=0.2.5; extra == "id31"
-Requires-Dist: ewoksjob; extra == "id31"
+Provides-Extra: id01
+Requires-Dist: blissdata>=0.2.5; extra == "id01"
+Requires-Dist: ewoksjob; extra == "id01"
 Provides-Extra: bm02
 Requires-Dist: blissdata>=0.2.5; extra == "bm02"
 Requires-Dist: ewoksjob; extra == "bm02"
+Provides-Extra: id09
+Requires-Dist: blissdata>=0.2.5; extra == "id09"
+Requires-Dist: ewoksjob; extra == "id09"
 Provides-Extra: id11
 Requires-Dist: blissdata>=0.2.5; extra == "id11"
 Requires-Dist: ewoksjob; extra == "id11"
+Provides-Extra: id12
+Requires-Dist: blissdata>=0.2.5; extra == "id12"
+Requires-Dist: ewoksjob; extra == "id12"
+Provides-Extra: id13
+Requires-Dist: blissdata>=0.2.5; extra == "id13"
+Requires-Dist: ewoksjob; extra == "id13"
 Provides-Extra: id14
 Requires-Dist: blissdata>=0.2.5; extra == "id14"
 Requires-Dist: ewoksjob; extra == "id14"
-Provides-Extra: streamline
-Requires-Dist: blissdata>=0.2.5; extra == "streamline"
-Requires-Dist: ewoksjob; extra == "streamline"
+Provides-Extra: id22
+Requires-Dist: blissdata>=0.2.5; extra == "id22"
+Requires-Dist: ewoksjob; extra == "id22"
 Provides-Extra: bm23
 Requires-Dist: blissdata>=0.2.5; extra == "bm23"
 Requires-Dist: ewoksjob; extra == "bm23"
 Requires-Dist: silx>=1.1.0; extra == "bm23"
 Provides-Extra: id24
 Requires-Dist: blissdata>=0.2.5; extra == "id24"
 Requires-Dist: ewoksjob; extra == "id24"
 Requires-Dist: silx>=1.1.0; extra == "id24"
+Provides-Extra: id31
+Requires-Dist: blissdata>=0.2.5; extra == "id31"
+Requires-Dist: ewoksjob; extra == "id31"
+Provides-Extra: streamline
+Requires-Dist: blissdata>=0.2.5; extra == "streamline"
+Requires-Dist: ewoksjob; extra == "streamline"
 Provides-Extra: democlient
 Requires-Dist: blissdata>=0.2.5; extra == "democlient"
 Requires-Dist: ewoksjob; extra == "democlient"
 Provides-Extra: demoworker
 Requires-Dist: blissdata>=0.2.5; extra == "demoworker"
 Requires-Dist: ewoksjob; extra == "demoworker"
 Requires-Dist: ewoksjob[blissworker]>=0.2.1; extra == "demoworker"
@@ -61,14 +70,15 @@
 Requires-Dist: est[full]; extra == "demoworker"
 Requires-Dist: orange3; extra == "demoworker"
 Provides-Extra: test
 Requires-Dist: pytest>=7; extra == "test"
 Requires-Dist: mock; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 Requires-Dist: pytest-redis; extra == "test"
+Requires-Dist: scipy; extra == "test"
 Requires-Dist: blissdata>=0.2.5; extra == "test"
 Requires-Dist: ewoksjob; extra == "test"
 Requires-Dist: blissdata>=0.2.5; extra == "test"
 Requires-Dist: ewoksjob; extra == "test"
 Requires-Dist: blissdata>=0.2.5; extra == "test"
 Requires-Dist: ewoksjob; extra == "test"
 Requires-Dist: blissdata>=0.2.5; extra == "test"
@@ -81,14 +91,15 @@
 Requires-Dist: ewoksjob; extra == "test"
 Requires-Dist: silx>=1.1.0; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pytest>=7; extra == "dev"
 Requires-Dist: mock; extra == "dev"
 Requires-Dist: pytest-mock; extra == "dev"
 Requires-Dist: pytest-redis; extra == "dev"
+Requires-Dist: scipy; extra == "dev"
 Requires-Dist: blissdata>=0.2.5; extra == "dev"
 Requires-Dist: ewoksjob; extra == "dev"
 Requires-Dist: blissdata>=0.2.5; extra == "dev"
 Requires-Dist: ewoksjob; extra == "dev"
 Requires-Dist: blissdata>=0.2.5; extra == "dev"
 Requires-Dist: ewoksjob; extra == "dev"
 Requires-Dist: blissdata>=0.2.5; extra == "dev"
@@ -103,14 +114,15 @@
 Requires-Dist: black>=22; extra == "dev"
 Requires-Dist: flake8>=4; extra == "dev"
 Provides-Extra: doc
 Requires-Dist: pytest>=7; extra == "doc"
 Requires-Dist: mock; extra == "doc"
 Requires-Dist: pytest-mock; extra == "doc"
 Requires-Dist: pytest-redis; extra == "doc"
+Requires-Dist: scipy; extra == "doc"
 Requires-Dist: blissdata>=0.2.5; extra == "doc"
 Requires-Dist: ewoksjob; extra == "doc"
 Requires-Dist: blissdata>=0.2.5; extra == "doc"
 Requires-Dist: ewoksjob; extra == "doc"
 Requires-Dist: blissdata>=0.2.5; extra == "doc"
 Requires-Dist: ewoksjob; extra == "doc"
 Requires-Dist: blissdata>=0.2.5; extra == "doc"
```

### Comparing `blissoda-0.3.1/src/blissoda.egg-info/SOURCES.txt` & `blissoda-0.4.0/src/blissoda.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,35 +23,39 @@
 src/blissoda/bm23/__init__.py
 src/blissoda/bm23/exafs_plotter.py
 src/blissoda/demo/__init__.py
 src/blissoda/demo/calib.py
 src/blissoda/demo/exafs.py
 src/blissoda/demo/example.py
 src/blissoda/demo/id11.py
+src/blissoda/demo/id12.py
 src/blissoda/demo/id14.py
 src/blissoda/demo/id22.py
 src/blissoda/demo/streamline.py
 src/blissoda/demo/xrpd.py
 src/blissoda/demo/user_scripts/__init__.py
 src/blissoda/demo/user_scripts/all.py
 src/blissoda/demo/user_scripts/exafs.py
 src/blissoda/demo/user_scripts/id11.py
+src/blissoda/demo/user_scripts/id12.py
 src/blissoda/demo/user_scripts/id14.py
 src/blissoda/demo/user_scripts/id22.py
 src/blissoda/demo/user_scripts/streamline.py
 src/blissoda/demo/user_scripts/xrpd.py
 src/blissoda/exafs/__init__.py
 src/blissoda/exafs/plots.py
 src/blissoda/exafs/plotter.py
 src/blissoda/exafs/widgets.py
 src/blissoda/flint/__init__.py
 src/blissoda/id09/__init__.py
 src/blissoda/id09/xrpd_processor.py
 src/blissoda/id11/__init__.py
 src/blissoda/id11/xrpd_processor.py
+src/blissoda/id12/__init__.py
+src/blissoda/id12/converter.py
 src/blissoda/id14/__init__.py
 src/blissoda/id14/converter.py
 src/blissoda/id22/__init__.py
 src/blissoda/id22/stscan_processor.py
 src/blissoda/id22/xrpd_processor.py
 src/blissoda/id24/__init__.py
 src/blissoda/id24/exafs_plotter.py
@@ -71,14 +75,16 @@
 src/blissoda/resources/demo/pdf_config.cfg
 src/blissoda/resources/exafs/__init__.py
 src/blissoda/resources/exafs/exafs.ows
 src/blissoda/resources/id11/__init__.py
 src/blissoda/resources/id11/integrate_scan_with_saving.json
 src/blissoda/resources/id11/integrate_scan_with_saving_pdf.json
 src/blissoda/resources/id11/integrate_scan_without_saving.json
+src/blissoda/resources/id12/__init__.py
+src/blissoda/resources/id12/convert.json
 src/blissoda/resources/id22/Sum_then_integrate_with_saving.json
 src/blissoda/resources/id22/__init__.py
 src/blissoda/resources/streamline/__init__.py
 src/blissoda/resources/streamline/reprocess.py
 src/blissoda/resources/streamline/streamline_with_calib.json
 src/blissoda/resources/streamline/streamline_without_calib.json
 src/blissoda/resources/streamline/time_record.py
```

### Comparing `blissoda-0.3.1/src/blissoda.egg-info/requires.txt` & `blissoda-0.4.0/src/blissoda.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -25,41 +25,55 @@
 orange3
 
 [dev]
 pytest>=7
 mock
 pytest-mock
 pytest-redis
+scipy
 blissdata>=0.2.5
 ewoksjob
 silx>=1.1.0
 black>=22
 flake8>=4
 
 [doc]
 pytest>=7
 mock
 pytest-mock
 pytest-redis
+scipy
 blissdata>=0.2.5
 ewoksjob
 silx>=1.1.0
 sphinx>=4.5
 sphinx-autodoc-typehints>=1.16
 sphinx_design
 pydata_sphinx_theme<0.15
 
+[id01]
+blissdata>=0.2.5
+ewoksjob
+
 [id09]
 blissdata>=0.2.5
 ewoksjob
 
 [id11]
 blissdata>=0.2.5
 ewoksjob
 
+[id12]
+blissdata>=0.2.5
+ewoksjob
+
+[id13]
+blissdata>=0.2.5
+ewoksjob
+
 [id14]
 blissdata>=0.2.5
 ewoksjob
 
 [id22]
 blissdata>=0.2.5
 ewoksjob
@@ -82,10 +96,11 @@
 ewoksjob
 
 [test]
 pytest>=7
 mock
 pytest-mock
 pytest-redis
+scipy
 blissdata>=0.2.5
 ewoksjob
 silx>=1.1.0
```

