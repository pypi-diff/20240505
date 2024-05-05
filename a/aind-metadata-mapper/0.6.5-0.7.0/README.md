# Comparing `tmp/aind_metadata_mapper-0.6.5.tar.gz` & `tmp/aind_metadata_mapper-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_metadata_mapper-0.6.5.tar", last modified: Wed Apr 24 23:21:47 2024, max compression
+gzip compressed data, was "aind_metadata_mapper-0.7.0.tar", last modified: Sun May  5 21:04:15 2024, max compression
```

## Comparing `aind_metadata_mapper-0.6.5.tar` & `aind_metadata_mapper-0.7.0.tar`

### file list

```diff
@@ -1,120 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.734520 aind_metadata_mapper-0.6.5/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.714519 aind_metadata_mapper-0.6.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.718519 aind_metadata_mapper-0.6.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.722519 aind_metadata_mapper-0.6.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/.github/workflows/test_and_lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-04-24 23:21:47.734520 aind_metadata_mapper-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.722519 aind_metadata_mapper-0.6.5/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.722519 aind_metadata_mapper-0.6.5/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.722519 aind_metadata_mapper-0.6.5/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/doc_template/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.722519 aind_metadata_mapper-0.6.5/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/examples/bergamo_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.722519 aind_metadata_mapper-0.6.5/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/scripts/singularity_build.def
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 23:21:47.734520 aind_metadata_mapper-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.718519 aind_metadata_mapper-0.6.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.722519 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-24 23:21:38.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.722519 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/bergamo/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/bergamo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23421 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/bergamo/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.722519 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/ephys/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/ephys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/ephys/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.726519 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/fib/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/fib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/fib/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/gather_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.726519 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/mesoscope/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/mesoscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/mesoscope/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.726519 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/neuropixels/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/neuropixels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/neuropixels/mvr_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/neuropixels/neuropixels_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/neuropixels/open_ephys_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/neuropixels/sync_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/neuropixels/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.734520 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-04-24 23:21:47.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-24 23:21:47.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 23:21:47.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-24 23:21:47.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-24 23:21:47.000000 aind_metadata_mapper-0.6.5/src/aind_metadata_mapper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.726519 aind_metadata_mapper-0.6.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.718519 aind_metadata_mapper-0.6.5/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.726519 aind_metadata_mapper-0.6.5/tests/resources/bergamo/
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/bergamo/cropped_neuron50_00001.tif
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/bergamo/example_description0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    76696 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/bergamo/example_metadata.txt.gz
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/bergamo/expected_session.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.730519 aind_metadata_mapper-0.6.5/tests/resources/ephys/
--rw-r--r--   0 runner    (1001) docker     (127)    11653 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/ephys/ephys_session.json
--rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/ephys/newscale_main.csv
--rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/ephys/newscale_surface_finding.csv
--rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/ephys/settings_main.xml
--rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/ephys/settings_surface_finding.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.730519 aind_metadata_mapper-0.6.5/tests/resources/fib/
--rw-r--r--   0 runner    (1001) docker     (127)    15663 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/fib/000000_ophys_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/fib/000000_ophys_session.json
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/fib/example_from_teensy.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.730519 aind_metadata_mapper-0.6.5/tests/resources/gather_metadata_job/
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/gather_metadata_job/example_procedures_response.json
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/gather_metadata_job/example_subject_response.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.730519 aind_metadata_mapper-0.6.5/tests/resources/gather_metadata_job/metadata_files/
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/gather_metadata_job/metadata_files/data_description.json
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/gather_metadata_job/metadata_files/procedures.json
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/gather_metadata_job/metadata_files/processing.json
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/gather_metadata_job/metadata_files/subject.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.730519 aind_metadata_mapper-0.6.5/tests/resources/mesoscope/
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/mesoscope/0123456789_Face_20240212T091444.json
--rw-r--r--   0 runner    (1001) docker     (127)    15701 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/mesoscope/example_extract.json
--rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/mesoscope/example_platform.json
--rw-r--r--   0 runner    (1001) docker     (127)    12038 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/mesoscope/expected_session.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.734520 aind_metadata_mapper-0.6.5/tests/resources/neuropixels/
--rw-r--r--   0 runner    (1001) docker     (127)    39424 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/neuropixels/base-missing-probe_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)    40853 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/neuropixels/base_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/neuropixels/mvr.ini
--rw-r--r--   0 runner    (1001) docker     (127)    42611 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/neuropixels/mvr_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)    42283 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/neuropixels/open-ephys-inferred_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)    42266 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/neuropixels/open-ephys_rig.json
--rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/neuropixels/settings.mislabeled-probes-0.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/neuropixels/settings.mislabeled-probes-1.xml
--rw-r--r--   0 runner    (1001) docker     (127)   132751 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/neuropixels/settings.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/neuropixels/sync.yml
--rw-r--r--   0 runner    (1001) docker     (127)    46653 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/resources/neuropixels/sync_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)    13902 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/test_bergamo.py
--rw-r--r--   0 runner    (1001) docker     (127)     9895 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/test_ephys.py
--rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/test_fib.py
--rw-r--r--   0 runner    (1001) docker     (127)    15172 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/test_gather_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/test_legacy_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/test_mesoscope.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:21:47.734520 aind_metadata_mapper-0.6.5/tests/test_neuropixels/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/test_neuropixels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/test_neuropixels/test_mvr_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/test_neuropixels/test_neuropixels_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/test_neuropixels/test_open_ephys_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/test_neuropixels/test_open_ephys_rig_inferrred.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/test_neuropixels/test_sync_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-24 23:21:37.000000 aind_metadata_mapper-0.6.5/tests/test_neuropixels/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.985203 aind_metadata_mapper-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.961203 aind_metadata_mapper-0.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.969203 aind_metadata_mapper-0.7.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.969203 aind_metadata_mapper-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/.github/workflows/test_and_lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-05-05 21:04:15.985203 aind_metadata_mapper-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.969203 aind_metadata_mapper-0.7.0/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.969203 aind_metadata_mapper-0.7.0/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.969203 aind_metadata_mapper-0.7.0/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/doc_template/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.969203 aind_metadata_mapper-0.7.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/examples/bergamo_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.969203 aind_metadata_mapper-0.7.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/scripts/singularity_build.def
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 21:04:15.985203 aind_metadata_mapper-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.965203 aind_metadata_mapper-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.969203 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.969203 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/bergamo/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/bergamo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23421 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/bergamo/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.973203 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/ephys/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/ephys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/ephys/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.973203 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/fib/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/fib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/fib/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12051 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/gather_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.973203 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/mesoscope/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/mesoscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/mesoscope/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.973203 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/neuropixels/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/neuropixels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/neuropixels/mvr_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/neuropixels/neuropixels_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/neuropixels/open_ephys_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/neuropixels/sync_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/neuropixels/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.981203 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-05-05 21:04:15.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-05 21:04:15.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 21:04:15.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-05 21:04:15.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-05 21:04:15.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.973203 aind_metadata_mapper-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.965203 aind_metadata_mapper-0.7.0/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.973203 aind_metadata_mapper-0.7.0/tests/resources/bergamo/
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/bergamo/cropped_neuron50_00001.tif
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/bergamo/example_description0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    76696 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/bergamo/example_metadata.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/bergamo/expected_session.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.977203 aind_metadata_mapper-0.7.0/tests/resources/ephys/
+-rw-r--r--   0 runner    (1001) docker     (127)    11653 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/ephys/ephys_session.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/ephys/newscale_main.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/ephys/newscale_surface_finding.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/ephys/settings_main.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/ephys/settings_surface_finding.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.977203 aind_metadata_mapper-0.7.0/tests/resources/fib/
+-rw-r--r--   0 runner    (1001) docker     (127)    15663 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/fib/000000_ophys_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/fib/000000_ophys_session.json
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/fib/example_from_teensy.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.977203 aind_metadata_mapper-0.7.0/tests/resources/gather_metadata_job/
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/gather_metadata_job/example_funding_multiple_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/gather_metadata_job/example_funding_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/gather_metadata_job/example_procedures_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/gather_metadata_job/example_subject_response.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.977203 aind_metadata_mapper-0.7.0/tests/resources/gather_metadata_job/metadata_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/gather_metadata_job/metadata_files/data_description.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/gather_metadata_job/metadata_files/procedures.json
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/gather_metadata_job/metadata_files/processing.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/gather_metadata_job/metadata_files/subject.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.977203 aind_metadata_mapper-0.7.0/tests/resources/mesoscope/
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/mesoscope/0123456789_Face_20240212T091444.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15701 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/mesoscope/example_extract.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/mesoscope/example_platform.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12038 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/mesoscope/expected_session.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.981203 aind_metadata_mapper-0.7.0/tests/resources/neuropixels/
+-rw-r--r--   0 runner    (1001) docker     (127)    39424 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/neuropixels/base-missing-probe_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)    40853 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/neuropixels/base_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/neuropixels/mvr.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    42611 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/neuropixels/mvr_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)    42283 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/neuropixels/open-ephys-inferred_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)    42266 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/neuropixels/open-ephys_rig.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/neuropixels/settings.mislabeled-probes-0.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/neuropixels/settings.mislabeled-probes-1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   132751 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/neuropixels/settings.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/neuropixels/sync.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    46653 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/neuropixels/sync_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13902 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/test_bergamo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9895 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/test_ephys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/test_fib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17909 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/test_gather_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/test_legacy_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/test_mesoscope.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.981203 aind_metadata_mapper-0.7.0/tests/test_neuropixels/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/test_neuropixels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/test_neuropixels/test_mvr_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/test_neuropixels/test_neuropixels_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/test_neuropixels/test_open_ephys_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/test_neuropixels/test_open_ephys_rig_inferrred.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/test_neuropixels/test_sync_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/test_neuropixels/utils.py
```

### Comparing `aind_metadata_mapper-0.6.5/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_metadata_mapper-0.7.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_metadata_mapper-0.7.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/.github/ISSUE_TEMPLATE/user-story.md` & `aind_metadata_mapper-0.7.0/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/.github/workflows/tag_and_publish.yml` & `aind_metadata_mapper-0.7.0/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/.github/workflows/test_and_lint.yml` & `aind_metadata_mapper-0.7.0/.github/workflows/test_and_lint.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/.gitignore` & `aind_metadata_mapper-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/LICENSE` & `aind_metadata_mapper-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/PKG-INFO` & `aind_metadata_mapper-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-metadata-mapper
-Version: 0.6.5
+Version: 0.7.0
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_metadata_mapper-0.6.5/README.md` & `aind_metadata_mapper-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/doc_template/Makefile` & `aind_metadata_mapper-0.7.0/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/doc_template/make.bat` & `aind_metadata_mapper-0.7.0/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/doc_template/source/_static/dark-logo.svg` & `aind_metadata_mapper-0.7.0/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/doc_template/source/_static/favicon.ico` & `aind_metadata_mapper-0.7.0/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/doc_template/source/_static/light-logo.svg` & `aind_metadata_mapper-0.7.0/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/doc_template/source/conf.py` & `aind_metadata_mapper-0.7.0/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/examples/bergamo_session.py` & `aind_metadata_mapper-0.7.0/examples/bergamo_session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/pyproject.toml` & `aind_metadata_mapper-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/bergamo/session.py` & `aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/bergamo/session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/core.py` & `aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/core.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/ephys/session.py` & `aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/ephys/session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/fib/session.py` & `aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/fib/session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/gather_metadata.py` & `aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/gather_metadata.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """Module to gather metadata from different sources."""
 
 import argparse
 import json
 import sys
 from pathlib import Path
-from typing import List, Optional, Tuple, Type
+from typing import List, Optional, Type
 
 import requests
 from aind_data_schema.base import AindCoreModel
 from aind_data_schema.core.acquisition import Acquisition
 from aind_data_schema.core.data_description import (
     DataDescription,
-    Funding,
     RawDataDescription,
 )
 from aind_data_schema.core.instrument import Instrument
 from aind_data_schema.core.metadata import Metadata
 from aind_data_schema.core.procedures import Procedures
 from aind_data_schema.core.processing import PipelineProcess, Processing
 from aind_data_schema.core.rig import Rig
@@ -28,32 +27,32 @@
 from pydantic_settings import BaseSettings
 
 
 class SubjectSettings(BaseSettings):
     """Fields needed to retrieve subject metadata"""
 
     subject_id: str
-    metadata_service_url: str
+    metadata_service_path: str = "subject"
 
 
 class ProceduresSettings(BaseSettings):
     """Fields needed to retrieve procedures metadata"""
 
     subject_id: str
-    metadata_service_url: str
+    metadata_service_path: str = "procedures"
 
 
-class DataDescriptionSettings(BaseSettings):
+class RawDataDescriptionSettings(BaseSettings):
     """Fields needed to retrieve data description metadata"""
 
     name: str
-    investigators: List[PIDName]
+    project_name: str
     modality: List[Modality.ONE_OF]
-    funding_source: Optional[Tuple] = (Funding(funder=Organization.AI),)
     institution: Optional[Organization.ONE_OF] = Organization.AIND
+    metadata_service_path: str = "funding"
 
 
 class ProcessingSettings(BaseSettings):
     """Fields needed to retrieve processing metadata"""
 
     pipeline_process: PipelineProcess
 
@@ -72,16 +71,17 @@
     acquisition_filepath: Optional[Path] = None
     instrument_filepath: Optional[Path] = None
 
 
 class JobSettings(BaseSettings):
     """Fields needed to gather all metadata"""
 
+    metadata_service_domain: Optional[str] = None
     subject_settings: Optional[SubjectSettings] = None
-    data_description_settings: Optional[DataDescriptionSettings] = None
+    raw_data_description_settings: Optional[RawDataDescriptionSettings] = None
     procedures_settings: Optional[ProceduresSettings] = None
     processing_settings: Optional[ProcessingSettings] = None
     metadata_settings: Optional[MetadataSettings] = None
     directory_to_write_to: Path
 
 
 class GatherMetadataJob:
@@ -95,78 +95,107 @@
         settings : JobSettings
         """
         self.settings = settings
 
     def get_subject(self) -> dict:
         """Get subject metadata"""
         response = requests.get(
-            self.settings.subject_settings.metadata_service_url
-            + f"/subject/{self.settings.subject_settings.subject_id}"
+            self.settings.metadata_service_domain
+            + f"/{self.settings.subject_settings.metadata_service_path}/"
+            + f"{self.settings.subject_settings.subject_id}"
         )
 
         if response.status_code < 300 or response.status_code == 406:
             json_content = response.json()
             return json_content["data"]
         else:
             raise AssertionError(
                 f"Subject metadata is not valid! {response.json()}"
             )
 
     def get_procedures(self) -> dict:
         """Get procedures metadata"""
         response = requests.get(
-            self.settings.procedures_settings.metadata_service_url
-            + f"/procedures/{self.settings.procedures_settings.subject_id}"
+            self.settings.metadata_service_domain
+            + f"/{self.settings.procedures_settings.metadata_service_path}/"
+            + f"{self.settings.procedures_settings.subject_id}"
         )
 
         if response.status_code < 300 or response.status_code == 406:
             json_content = response.json()
             return json_content["data"]
         else:
             raise AssertionError(
                 f"Procedures metadata is not valid! {response.json()}"
             )
 
     def get_raw_data_description(self) -> dict:
         """Get raw data description metadata"""
+
+        def get_funding_info(domain: str, url_path: str, project_name: str):
+            """Utility method to retrieve funding info from metadata service"""
+            response = requests.get("/".join([domain, url_path, project_name]))
+            if response.status_code == 200:
+                funding_info = [response.json().get("data")]
+            elif response.status_code == 300:
+                funding_info = response.json().get("data")
+            else:
+                funding_info = []
+            investigators = set()
+            for f in funding_info:
+                project_fundees = f.get("fundee", "").split(",")
+                pid_names = [
+                    PIDName(name=p.strip()).model_dump_json()
+                    for p in project_fundees
+                ]
+                if project_fundees is not [""]:
+                    investigators.update(pid_names)
+            investigators = [
+                PIDName.model_validate_json(i) for i in investigators
+            ]
+            investigators.sort(key=lambda x: x.name)
+            return funding_info, investigators
+
+        # Returns a dict with platform, subject_id, and acq_datetime
         basic_settings = RawDataDescription.parse_name(
-            name=self.settings.data_description_settings.name
+            name=self.settings.raw_data_description_settings.name
+        )
+        funding_source, investigator_list = get_funding_info(
+            self.settings.metadata_service_domain,
+            self.settings.raw_data_description_settings.metadata_service_path,
+            self.settings.raw_data_description_settings.project_name,
         )
 
         try:
             return json.loads(
                 RawDataDescription(
-                    name=self.settings.data_description_settings.name,
+                    name=self.settings.raw_data_description_settings.name,
                     institution=(
-                        self.settings.data_description_settings.institution
-                    ),
-                    modality=self.settings.data_description_settings.modality,
-                    funding_source=(
-                        self.settings.data_description_settings.funding_source
+                        self.settings.raw_data_description_settings.institution
                     ),
-                    investigators=(
-                        self.settings.data_description_settings.investigators
+                    modality=(
+                        self.settings.raw_data_description_settings.modality
                     ),
+                    funding_source=funding_source,
+                    investigators=investigator_list,
                     **basic_settings,
                 ).model_dump_json()
             )
         except ValidationError:
             return json.loads(
                 RawDataDescription.model_construct(
-                    name=self.settings.data_description_settings.name,
+                    name=self.settings.raw_data_description_settings.name,
                     institution=(
-                        self.settings.data_description_settings.institution
-                    ),
-                    modality=self.settings.data_description_settings.modality,
-                    funding_source=(
-                        self.settings.data_description_settings.funding_source
+                        self.settings.raw_data_description_settings.institution
                     ),
-                    investigators=(
-                        self.settings.data_description_settings.investigators
+                    modality=(
+                        self.settings.raw_data_description_settings.modality
                     ),
+                    funding_source=funding_source,
+                    investigators=investigator_list,
                     **basic_settings,
                 ).model_dump_json()
             )
 
     def get_processing_metadata(self):
         """Get processing metadata"""
 
@@ -272,15 +301,15 @@
                 filename=Subject.default_filename(), contents=contents
             )
         if self.settings.procedures_settings is not None:
             contents = self.get_procedures()
             self._write_json_file(
                 filename=Procedures.default_filename(), contents=contents
             )
-        if self.settings.data_description_settings is not None:
+        if self.settings.raw_data_description_settings is not None:
             contents = self.get_raw_data_description()
             self._write_json_file(
                 filename=DataDescription.default_filename(), contents=contents
             )
         if self.settings.processing_settings is not None:
             contents = self.get_processing_metadata()
             self._write_json_file(
```

### Comparing `aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/mesoscope/session.py` & `aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/mesoscope/session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/neuropixels/mvr_rig.py` & `aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/neuropixels/mvr_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/neuropixels/neuropixels_rig.py` & `aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/neuropixels/neuropixels_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/neuropixels/open_ephys_rig.py` & `aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/neuropixels/open_ephys_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/neuropixels/sync_rig.py` & `aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/neuropixels/sync_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/src/aind_metadata_mapper/neuropixels/utils.py` & `aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/neuropixels/utils.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/src/aind_metadata_mapper.egg-info/PKG-INFO` & `aind_metadata_mapper-0.7.0/src/aind_metadata_mapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-metadata-mapper
-Version: 0.6.5
+Version: 0.7.0
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_metadata_mapper-0.6.5/src/aind_metadata_mapper.egg-info/SOURCES.txt` & `aind_metadata_mapper-0.7.0/src/aind_metadata_mapper.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,16 @@
 tests/resources/ephys/newscale_main.csv
 tests/resources/ephys/newscale_surface_finding.csv
 tests/resources/ephys/settings_main.xml
 tests/resources/ephys/settings_surface_finding.xml
 tests/resources/fib/000000_ophys_rig.json
 tests/resources/fib/000000_ophys_session.json
 tests/resources/fib/example_from_teensy.txt
+tests/resources/gather_metadata_job/example_funding_multiple_response.json
+tests/resources/gather_metadata_job/example_funding_response.json
 tests/resources/gather_metadata_job/example_procedures_response.json
 tests/resources/gather_metadata_job/example_subject_response.json
 tests/resources/gather_metadata_job/metadata_files/data_description.json
 tests/resources/gather_metadata_job/metadata_files/procedures.json
 tests/resources/gather_metadata_job/metadata_files/processing.json
 tests/resources/gather_metadata_job/metadata_files/subject.json
 tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json
```

### Comparing `aind_metadata_mapper-0.6.5/tests/resources/bergamo/cropped_neuron50_00001.tif` & `aind_metadata_mapper-0.7.0/tests/resources/bergamo/cropped_neuron50_00001.tif`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/resources/bergamo/example_description0.txt` & `aind_metadata_mapper-0.7.0/tests/resources/bergamo/example_description0.txt`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/resources/bergamo/example_metadata.txt.gz` & `aind_metadata_mapper-0.7.0/tests/resources/bergamo/example_metadata.txt.gz`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/resources/bergamo/expected_session.json` & `aind_metadata_mapper-0.7.0/tests/resources/bergamo/expected_session.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/resources/ephys/ephys_session.json` & `aind_metadata_mapper-0.7.0/tests/resources/ephys/ephys_session.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/resources/ephys/newscale_main.csv` & `aind_metadata_mapper-0.7.0/tests/resources/ephys/newscale_main.csv`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/resources/ephys/newscale_surface_finding.csv` & `aind_metadata_mapper-0.7.0/tests/resources/ephys/newscale_surface_finding.csv`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/resources/ephys/settings_main.xml` & `aind_metadata_mapper-0.7.0/tests/resources/ephys/settings_main.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/resources/ephys/settings_surface_finding.xml` & `aind_metadata_mapper-0.7.0/tests/resources/ephys/settings_surface_finding.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/resources/fib/000000_ophys_rig.json` & `aind_metadata_mapper-0.7.0/tests/resources/fib/000000_ophys_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/resources/fib/000000_ophys_session.json` & `aind_metadata_mapper-0.7.0/tests/resources/fib/000000_ophys_session.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/resources/gather_metadata_job/example_procedures_response.json` & `aind_metadata_mapper-0.7.0/tests/resources/gather_metadata_job/example_procedures_response.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/resources/gather_metadata_job/example_subject_response.json` & `aind_metadata_mapper-0.7.0/tests/resources/gather_metadata_job/example_subject_response.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/resources/gather_metadata_job/metadata_files/data_description.json` & `aind_metadata_mapper-0.7.0/tests/resources/gather_metadata_job/metadata_files/data_description.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/resources/gather_metadata_job/metadata_files/procedures.json` & `aind_metadata_mapper-0.7.0/tests/resources/gather_metadata_job/metadata_files/procedures.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/resources/gather_metadata_job/metadata_files/processing.json` & `aind_metadata_mapper-0.7.0/tests/resources/gather_metadata_job/metadata_files/processing.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/resources/gather_metadata_job/metadata_files/subject.json` & `aind_metadata_mapper-0.7.0/tests/resources/gather_metadata_job/metadata_files/subject.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json` & `aind_metadata_mapper-0.7.0/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json` & `aind_metadata_mapper-0.7.0/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/resources/mesoscope/0123456789_Face_20240212T091444.json` & `aind_metadata_mapper-0.7.0/tests/resources/mesoscope/0123456789_Face_20240212T091444.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/resources/mesoscope/example_extract.json` & `aind_metadata_mapper-0.7.0/tests/resources/mesoscope/example_extract.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/resources/mesoscope/example_platform.json` & `aind_metadata_mapper-0.7.0/tests/resources/mesoscope/example_platform.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/resources/mesoscope/expected_session.json` & `aind_metadata_mapper-0.7.0/tests/resources/mesoscope/expected_session.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/resources/neuropixels/base-missing-probe_rig.json` & `aind_metadata_mapper-0.7.0/tests/resources/neuropixels/base-missing-probe_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/resources/neuropixels/base_rig.json` & `aind_metadata_mapper-0.7.0/tests/resources/neuropixels/base_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/resources/neuropixels/mvr.ini` & `aind_metadata_mapper-0.7.0/tests/resources/neuropixels/mvr.ini`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/resources/neuropixels/mvr_rig.json` & `aind_metadata_mapper-0.7.0/tests/resources/neuropixels/mvr_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/resources/neuropixels/open-ephys-inferred_rig.json` & `aind_metadata_mapper-0.7.0/tests/resources/neuropixels/open-ephys-inferred_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/resources/neuropixels/open-ephys_rig.json` & `aind_metadata_mapper-0.7.0/tests/resources/neuropixels/open-ephys_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/resources/neuropixels/settings.mislabeled-probes-0.xml` & `aind_metadata_mapper-0.7.0/tests/resources/neuropixels/settings.mislabeled-probes-0.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/resources/neuropixels/settings.mislabeled-probes-1.xml` & `aind_metadata_mapper-0.7.0/tests/resources/neuropixels/settings.mislabeled-probes-1.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/resources/neuropixels/settings.xml` & `aind_metadata_mapper-0.7.0/tests/resources/neuropixels/settings.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/resources/neuropixels/sync.yml` & `aind_metadata_mapper-0.7.0/tests/resources/neuropixels/sync.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/resources/neuropixels/sync_rig.json` & `aind_metadata_mapper-0.7.0/tests/resources/neuropixels/sync_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/test_bergamo.py` & `aind_metadata_mapper-0.7.0/tests/test_bergamo.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/test_ephys.py` & `aind_metadata_mapper-0.7.0/tests/test_ephys.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/test_fib.py` & `aind_metadata_mapper-0.7.0/tests/test_fib.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/test_gather_metadata.py` & `aind_metadata_mapper-0.7.0/tests/test_gather_metadata.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,25 +5,24 @@
 import unittest
 from datetime import datetime, timezone
 from pathlib import Path
 from unittest.mock import MagicMock, mock_open, patch
 
 from aind_data_schema.core.processing import DataProcess, PipelineProcess
 from aind_data_schema.models.modalities import Modality
-from aind_data_schema.models.pid_names import PIDName
 from aind_data_schema.models.process_names import ProcessName
 from requests import Response
 
 from aind_metadata_mapper.gather_metadata import (
-    DataDescriptionSettings,
     GatherMetadataJob,
     JobSettings,
     MetadataSettings,
     ProceduresSettings,
     ProcessingSettings,
+    RawDataDescriptionSettings,
     SubjectSettings,
 )
 
 RESOURCES_DIR = (
     Path(os.path.dirname(os.path.realpath(__file__)))
     / "resources"
     / "gather_metadata_job"
@@ -39,16 +38,24 @@
         """Load json files."""
         with open(RESOURCES_DIR / "example_subject_response.json", "r") as f:
             example_subject_response = json.load(f)
         with open(
             RESOURCES_DIR / "example_procedures_response.json", "r"
         ) as f:
             example_procedures_response = json.load(f)
+        with open(RESOURCES_DIR / "example_funding_response.json", "r") as f:
+            example_funding_response = json.load(f)
+        with open(
+            RESOURCES_DIR / "example_funding_multiple_response.json", "r"
+        ) as f:
+            example_funding_multi_response = json.load(f)
         cls.example_subject_response = example_subject_response
         cls.example_procedures_response = example_procedures_response
+        cls.example_funding_response = example_funding_response
+        cls.example_funding_multi_response = example_funding_multi_response
 
     def test_class_constructor(self):
         """Tests class is constructed properly"""
         job_settings = JobSettings(directory_to_write_to=RESOURCES_DIR)
         metadata_job = GatherMetadataJob(settings=job_settings)
         self.assertIsNotNone(metadata_job)
 
@@ -58,38 +65,39 @@
         mock_response = Response()
         mock_response.status_code = 200
         body = json.dumps(self.example_subject_response)
         mock_response._content = body.encode("utf-8")
         mock_get.return_value = mock_response
 
         job_settings = JobSettings(
+            metadata_service_domain="http://acme.test",
             directory_to_write_to=RESOURCES_DIR,
             subject_settings=SubjectSettings(
                 subject_id="632269",
-                metadata_service_url="http://acme.test",
             ),
         )
         metadata_job = GatherMetadataJob(settings=job_settings)
         contents = metadata_job.get_subject()
         self.assertEqual("632269", contents["subject_id"])
+        mock_get.assert_called_once_with("http://acme.test/subject/632269")
 
     @patch("requests.get")
     def test_get_subject_error(self, mock_get: MagicMock):
         """Tests get_subject when an error is raised"""
         mock_response = Response()
         mock_response.status_code = 500
         body = json.dumps({"message": "Internal Server Error"})
         mock_response._content = body.encode("utf-8")
         mock_get.return_value = mock_response
 
         job_settings = JobSettings(
             directory_to_write_to=RESOURCES_DIR,
+            metadata_service_domain="http://acme.test",
             subject_settings=SubjectSettings(
                 subject_id="632269",
-                metadata_service_url="http://acme.test",
             ),
         )
         metadata_job = GatherMetadataJob(settings=job_settings)
         with self.assertRaises(AssertionError) as e:
             metadata_job.get_subject()
         expected_error_message = (
             "Subject metadata is not valid! "
@@ -104,93 +112,146 @@
         mock_response.status_code = 406
         body = json.dumps(self.example_procedures_response)
         mock_response._content = body.encode("utf-8")
         mock_get.return_value = mock_response
 
         job_settings = JobSettings(
             directory_to_write_to=RESOURCES_DIR,
+            metadata_service_domain="http://acme.test",
             procedures_settings=ProceduresSettings(
                 subject_id="632269",
-                metadata_service_url="http://acme.test",
             ),
         )
         metadata_job = GatherMetadataJob(settings=job_settings)
         contents = metadata_job.get_procedures()
         self.assertEqual("632269", contents["subject_id"])
+        mock_get.assert_called_once_with("http://acme.test/procedures/632269")
 
     @patch("requests.get")
     def test_get_procedures_error(self, mock_get: MagicMock):
         """Tests get_procedures when an error is raised"""
         mock_response = Response()
         mock_response.status_code = 500
         body = json.dumps({"message": "Internal Server Error"})
         mock_response._content = body.encode("utf-8")
         mock_get.return_value = mock_response
 
         job_settings = JobSettings(
             directory_to_write_to=RESOURCES_DIR,
+            metadata_service_domain="http://acme.test",
             procedures_settings=ProceduresSettings(
                 subject_id="632269",
-                metadata_service_url="http://acme.test",
             ),
         )
         metadata_job = GatherMetadataJob(settings=job_settings)
         with self.assertRaises(AssertionError) as e:
             metadata_job.get_procedures()
         expected_error_message = (
             "Procedures metadata is not valid! "
             "{'message': 'Internal Server Error'}"
         )
         self.assertTrue(expected_error_message in str(e.exception))
 
-    def test_get_raw_data_description(self):
+    @patch("requests.get")
+    def test_get_raw_data_description(self, mock_get: MagicMock):
         """Tests get_raw_data_description method with valid model"""
+
+        mock_response = Response()
+        mock_response.status_code = 200
+        body = json.dumps(self.example_funding_response)
+        mock_response._content = body.encode("utf-8")
+        mock_get.return_value = mock_response
+
         job_settings = JobSettings(
             directory_to_write_to=RESOURCES_DIR,
-            data_description_settings=DataDescriptionSettings(
-                investigators=[
-                    PIDName(name="Anna Apple"),
-                    PIDName(name="John Smith"),
-                ],
+            metadata_service_domain="http://acme.test",
+            raw_data_description_settings=RawDataDescriptionSettings(
+                project_name="Ephys Platform",
                 name="ecephys_632269_2023-10-10_10-10-10",
                 modality=[Modality.ECEPHYS, Modality.BEHAVIOR_VIDEOS],
             ),
         )
         metadata_job = GatherMetadataJob(settings=job_settings)
         contents = metadata_job.get_raw_data_description()
+        expected_investigators = ["Anna Apple", "John Smith"]
+        actual_investigators = [i["name"] for i in contents["investigators"]]
+        self.assertEqual(expected_investigators, actual_investigators)
         self.assertEqual("ecephys", contents["platform"]["abbreviation"])
         self.assertEqual("632269", contents["subject_id"])
         self.assertEqual(
             "ecephys_632269_2023-10-10_10-10-10", contents["name"]
         )
+        mock_get.assert_called_once_with(
+            "http://acme.test/funding/Ephys Platform"
+        )
+
+    @patch("requests.get")
+    def test_get_raw_data_description_multi_response(
+        self, mock_get: MagicMock
+    ):
+        """Tests get_raw_data_description method with valid model and multiple
+        items in funding response"""
+
+        mock_response = Response()
+        mock_response.status_code = 300
+        body = json.dumps(self.example_funding_multi_response)
+        mock_response._content = body.encode("utf-8")
+        mock_get.return_value = mock_response
 
-    def test_get_raw_data_description_invalid(self):
-        """Tests get_raw_data_description method with invalid model"""
         job_settings = JobSettings(
             directory_to_write_to=RESOURCES_DIR,
-            data_description_settings=DataDescriptionSettings(
-                investigators=[],
+            metadata_service_domain="http://acme.test",
+            raw_data_description_settings=RawDataDescriptionSettings(
+                project_name="Ephys Platform",
                 name="ecephys_632269_2023-10-10_10-10-10",
                 modality=[Modality.ECEPHYS, Modality.BEHAVIOR_VIDEOS],
             ),
         )
         metadata_job = GatherMetadataJob(settings=job_settings)
-        with self.assertWarns(UserWarning) as w:
-            contents = metadata_job.get_raw_data_description()
+        contents = metadata_job.get_raw_data_description()
+        expected_investigators = ["Anna Apple", "Don Key", "John Smith"]
+        actual_investigators = [i["name"] for i in contents["investigators"]]
+        self.assertEqual(2, len(contents["funding_source"]))
+        self.assertEqual(expected_investigators, actual_investigators)
         self.assertEqual("ecephys", contents["platform"]["abbreviation"])
         self.assertEqual("632269", contents["subject_id"])
         self.assertEqual(
             "ecephys_632269_2023-10-10_10-10-10", contents["name"]
         )
-        expected_warning = (
-            "Pydantic serializer warnings:\n"
-            "  Expected `list[Funding]` but got `tuple` -"
-            " serialized value may not be as expected"
+        mock_get.assert_called_once_with(
+            "http://acme.test/funding/Ephys Platform"
+        )
+
+    @patch("requests.get")
+    def test_get_raw_data_description_invalid(self, mock_get: MagicMock):
+        """Tests get_raw_data_description method with invalid model"""
+        mock_response = Response()
+        mock_response.status_code = 500
+        body = json.dumps({"message": "Internal Server Error"})
+        mock_response._content = body.encode("utf-8")
+        mock_get.return_value = mock_response
+
+        job_settings = JobSettings(
+            directory_to_write_to=RESOURCES_DIR,
+            metadata_service_domain="http://acme.test",
+            raw_data_description_settings=RawDataDescriptionSettings(
+                project_name="foo",
+                name="ecephys_632269_2023-10-10_10-10-10",
+                modality=[Modality.ECEPHYS, Modality.BEHAVIOR_VIDEOS],
+            ),
+        )
+        metadata_job = GatherMetadataJob(settings=job_settings)
+        # with self.assertWarns(UserWarning) as w:
+        contents = metadata_job.get_raw_data_description()
+        self.assertEqual("ecephys", contents["platform"]["abbreviation"])
+        self.assertEqual("632269", contents["subject_id"])
+        self.assertEqual(
+            "ecephys_632269_2023-10-10_10-10-10", contents["name"]
         )
-        self.assertEqual(expected_warning, str(w.warning))
+        self.assertEqual([], contents["investigators"])
 
     def test_get_processing_metadata(self):
         """Tests get_processing_metadata method"""
         data_process = DataProcess(
             name=ProcessName.COMPRESSION,
             software_version="0.0.15",
             start_date_time=datetime(
@@ -338,27 +399,23 @@
         )
         processing_pipeline = PipelineProcess(
             data_processes=[data_process], processor_full_name="Anna Apple"
         )
 
         job_settings = JobSettings(
             directory_to_write_to=RESOURCES_DIR,
+            metadata_service_domain="http://acme.test",
             subject_settings=SubjectSettings(
                 subject_id="632269",
-                metadata_service_url="http://acme.test",
             ),
             procedures_settings=ProceduresSettings(
                 subject_id="632269",
-                metadata_service_url="http://acme.test",
             ),
-            data_description_settings=DataDescriptionSettings(
-                investigators=[
-                    PIDName(name="Anna Apple"),
-                    PIDName(name="John Smith"),
-                ],
+            raw_data_description_settings=RawDataDescriptionSettings(
+                project_name="Ephys Platform",
                 name="ecephys_632269_2023-10-10_10-10-10",
                 modality=[Modality.ECEPHYS, Modality.BEHAVIOR_VIDEOS],
             ),
             processing_settings=ProcessingSettings(
                 pipeline_process=processing_pipeline
             ),
             metadata_settings=MetadataSettings(
```

### Comparing `aind_metadata_mapper-0.6.5/tests/test_legacy_core.py` & `aind_metadata_mapper-0.7.0/tests/test_legacy_core.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/test_mesoscope.py` & `aind_metadata_mapper-0.7.0/tests/test_mesoscope.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/test_neuropixels/test_mvr_rig.py` & `aind_metadata_mapper-0.7.0/tests/test_neuropixels/test_mvr_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/test_neuropixels/test_neuropixels_rig.py` & `aind_metadata_mapper-0.7.0/tests/test_neuropixels/test_neuropixels_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/test_neuropixels/test_open_ephys_rig.py` & `aind_metadata_mapper-0.7.0/tests/test_neuropixels/test_open_ephys_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/test_neuropixels/test_open_ephys_rig_inferrred.py` & `aind_metadata_mapper-0.7.0/tests/test_neuropixels/test_open_ephys_rig_inferrred.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/test_neuropixels/test_sync_rig.py` & `aind_metadata_mapper-0.7.0/tests/test_neuropixels/test_sync_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.6.5/tests/test_neuropixels/utils.py` & `aind_metadata_mapper-0.7.0/tests/test_neuropixels/utils.py`

 * *Files identical despite different names*

