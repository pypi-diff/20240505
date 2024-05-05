# Comparing `tmp/coh2_live_stats-1.2.0.tar.gz` & `tmp/coh2_live_stats-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coh2_live_stats-1.2.0.tar", last modified: Sat May  4 22:56:28 2024, max compression
+gzip compressed data, was "coh2_live_stats-1.2.1.tar", last modified: Sun May  5 01:11:39 2024, max compression
```

## Comparing `coh2_live_stats-1.2.0.tar` & `coh2_live_stats-1.2.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:56:28.788541 coh2_live_stats-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:56:28.756541 coh2_live_stats-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:56:28.760541 coh2_live_stats-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)    81699 2024-05-04 22:56:28.788541 coh2_live_stats-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    39436 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/invoke.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:56:28.760541 coh2_live_stats-1.2.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:56:28.764541 coh2_live_stats-1.2.0/scripts/github_actions/
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/scripts/github_actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/scripts/github_actions/activate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/scripts/github_actions/mock_logfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/scripts/pyinstaller_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    19671 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/scripts/readme_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/scripts/script_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/scripts/settings_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 22:56:28.788541 coh2_live_stats-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:56:28.760541 coh2_live_stats-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:56:28.764541 coh2_live_stats-1.2.0/src/coh2_live_stats/
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/src/coh2_live_stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10042 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/src/coh2_live_stats/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/src/coh2_live_stats/_logging.toml
--rw-r--r--   0 runner    (1001) docker     (127)    10427 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/src/coh2_live_stats/coh2api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:56:28.768541 coh2_live_stats-1.2.0/src/coh2_live_stats/data/
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/src/coh2_live_stats/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/src/coh2_live_stats/data/color.py
--rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/src/coh2_live_stats/data/countries.py
--rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/src/coh2_live_stats/data/faction.py
--rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/src/coh2_live_stats/data/match.py
--rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/src/coh2_live_stats/data/player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/src/coh2_live_stats/data/team.py
--rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/src/coh2_live_stats/logging_conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    15671 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/src/coh2_live_stats/output.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/src/coh2_live_stats/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:56:28.780541 coh2_live_stats-1.2.0/src/coh2_live_stats/res/
--rw-r--r--   0 runner    (1001) docker     (127)  8231670 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/src/coh2_live_stats/res/coh2_live_stats.ico
--rw-r--r--   0 runner    (1001) docker     (127)   806942 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/src/coh2_live_stats/res/coh2_live_stats.xcf
--rw-r--r--   0 runner    (1001) docker     (127)    24348 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/src/coh2_live_stats/res/example_0.svg
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/src/coh2_live_stats/res/example_1.svg
--rw-r--r--   0 runner    (1001) docker     (127)    25617 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/src/coh2_live_stats/res/example_default.svg
--rw-r--r--   0 runner    (1001) docker     (127)   806504 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/src/coh2_live_stats/res/horn.wav
--rw-r--r--   0 runner    (1001) docker     (127)  1267392 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/src/coh2_live_stats/res/horn_epic.wav
--rw-r--r--   0 runner    (1001) docker     (127)  1175232 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/src/coh2_live_stats/res/horn_subtle.wav
--rw-r--r--   0 runner    (1001) docker     (127)    12578 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/src/coh2_live_stats/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/src/coh2_live_stats/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-04 22:56:28.000000 coh2_live_stats-1.2.0/src/coh2_live_stats/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:56:28.784541 coh2_live_stats-1.2.0/src/coh2_live_stats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    81699 2024-05-04 22:56:28.000000 coh2_live_stats-1.2.0/src/coh2_live_stats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-04 22:56:28.000000 coh2_live_stats-1.2.0/src/coh2_live_stats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 22:56:28.000000 coh2_live_stats-1.2.0/src/coh2_live_stats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-04 22:56:28.000000 coh2_live_stats-1.2.0/src/coh2_live_stats.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-04 22:56:28.000000 coh2_live_stats-1.2.0/src/coh2_live_stats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-04 22:56:28.000000 coh2_live_stats-1.2.0/src/coh2_live_stats.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7795 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:56:28.784541 coh2_live_stats-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/tests/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)    30970 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/tests/test_logfile_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/tests/test_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-04 22:56:16.000000 coh2_live_stats-1.2.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 01:11:39.697153 coh2_live_stats-1.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 01:11:39.669153 coh2_live_stats-1.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 01:11:39.673153 coh2_live_stats-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)    82305 2024-05-05 01:11:39.697153 coh2_live_stats-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    39934 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/invoke.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 01:11:39.673153 coh2_live_stats-1.2.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 01:11:39.673153 coh2_live_stats-1.2.1/scripts/github_actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/scripts/github_actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/scripts/github_actions/activate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/scripts/github_actions/mock_logfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/scripts/pyinstaller_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19671 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/scripts/readme_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/scripts/script_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/scripts/settings_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 01:11:39.697153 coh2_live_stats-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 01:11:39.669153 coh2_live_stats-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 01:11:39.673153 coh2_live_stats-1.2.1/src/coh2_live_stats/
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/src/coh2_live_stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10042 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/src/coh2_live_stats/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/src/coh2_live_stats/_logging.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    10427 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/src/coh2_live_stats/coh2api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 01:11:39.677153 coh2_live_stats-1.2.1/src/coh2_live_stats/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/src/coh2_live_stats/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/src/coh2_live_stats/data/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/src/coh2_live_stats/data/countries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/src/coh2_live_stats/data/faction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/src/coh2_live_stats/data/match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/src/coh2_live_stats/data/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/src/coh2_live_stats/data/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/src/coh2_live_stats/logging_conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15671 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/src/coh2_live_stats/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/src/coh2_live_stats/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 01:11:39.693153 coh2_live_stats-1.2.1/src/coh2_live_stats/res/
+-rw-r--r--   0 runner    (1001) docker     (127)  8231670 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/src/coh2_live_stats/res/coh2_live_stats.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   806942 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/src/coh2_live_stats/res/coh2_live_stats.xcf
+-rw-r--r--   0 runner    (1001) docker     (127)    24348 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/src/coh2_live_stats/res/example_0.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/src/coh2_live_stats/res/example_1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    25617 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/src/coh2_live_stats/res/example_default.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   806504 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/src/coh2_live_stats/res/horn.wav
+-rw-r--r--   0 runner    (1001) docker     (127)  1267392 2024-05-05 01:11:22.000000 coh2_live_stats-1.2.1/src/coh2_live_stats/res/horn_epic.wav
+-rw-r--r--   0 runner    (1001) docker     (127)  1175232 2024-05-05 01:11:23.000000 coh2_live_stats-1.2.1/src/coh2_live_stats/res/horn_subtle.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    12578 2024-05-05 01:11:23.000000 coh2_live_stats-1.2.1/src/coh2_live_stats/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-05 01:11:23.000000 coh2_live_stats-1.2.1/src/coh2_live_stats/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-05 01:11:39.000000 coh2_live_stats-1.2.1/src/coh2_live_stats/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 01:11:39.693153 coh2_live_stats-1.2.1/src/coh2_live_stats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    82305 2024-05-05 01:11:39.000000 coh2_live_stats-1.2.1/src/coh2_live_stats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-05 01:11:39.000000 coh2_live_stats-1.2.1/src/coh2_live_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 01:11:39.000000 coh2_live_stats-1.2.1/src/coh2_live_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-05 01:11:39.000000 coh2_live_stats-1.2.1/src/coh2_live_stats.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-05 01:11:39.000000 coh2_live_stats-1.2.1/src/coh2_live_stats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-05 01:11:39.000000 coh2_live_stats-1.2.1/src/coh2_live_stats.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7795 2024-05-05 01:11:23.000000 coh2_live_stats-1.2.1/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 01:11:39.693153 coh2_live_stats-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-05 01:11:23.000000 coh2_live_stats-1.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-05-05 01:11:23.000000 coh2_live_stats-1.2.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-05 01:11:23.000000 coh2_live_stats-1.2.1/tests/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    30970 2024-05-05 01:11:23.000000 coh2_live_stats-1.2.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-05-05 01:11:23.000000 coh2_live_stats-1.2.1/tests/test_logfile_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-05-05 01:11:23.000000 coh2_live_stats-1.2.1/tests/test_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-05 01:11:23.000000 coh2_live_stats-1.2.1/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-05 01:11:23.000000 coh2_live_stats-1.2.1/tests/test_util.py
```

### Comparing `coh2_live_stats-1.2.0/.github/workflows/ci.yml` & `coh2_live_stats-1.2.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/.github/workflows/publish.yml` & `coh2_live_stats-1.2.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/COPYING` & `coh2_live_stats-1.2.1/COPYING`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/PKG-INFO` & `coh2_live_stats-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coh2_live_stats
-Version: 1.2.0
+Version: 1.2.1
 Summary: Show player and team stats of a currently played, replayed or last played Company of Heroes 2 match.
 Author-email: Andreas Becker <brofi.archlinux@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -682,14 +682,16 @@
 Project-URL: Issues, https://github.com/brofi/coh2-live-stats/issues
 Project-URL: Source, https://github.com/brofi/coh2-live-stats
 Keywords: CoH2,Company of Heroes 2
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only 
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Games/Entertainment :: Real Time Strategy
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: COPYING
 Requires-Dist: colorama>=0.4.6
@@ -710,14 +712,18 @@
 Requires-Dist: respx>=0.21.1; extra == "build"
 Requires-Dist: tomlkit>=0.12.4; extra == "build"
 Requires-Dist: twine>=5.0.0; extra == "build"
 
 # <img src="src/coh2_live_stats/res/coh2_live_stats.ico" alt="Icon" width="64" align="center"/> CoH2 Live Stats
 
 [![CI branch master](https://github.com/brofi/coh2-live-stats/actions/workflows/ci.yml/badge.svg)](https://github.com/brofi/coh2-live-stats/actions/workflows/ci.yml)
+[![pypi](https://img.shields.io/pypi/v/coh2-live-stats)](https://pypi.org/project/coh2-live-stats/)
+[![versions](https://img.shields.io/pypi/pyversions/coh2-live-stats)](https://github.com/brofi/coh2-live-stats)
+[![license](https://img.shields.io/github/license/brofi/coh2-live-stats)](https://github.com/brofi/coh2-live-stats/blob/master/COPYING)
+
 
 [//]: # (<mark_description>)
 
 Show player and team stats of a currently played, replayed or last played Company of Heroes 2 match.
 
 [//]: # (</mark_description>)
 
@@ -728,19 +734,23 @@
 with [gruvbox](https://github.com/morhetz/gruvbox) colors
 and [Inconsolata](https://github.com/googlefonts/Inconsolata) font.
 
 ## Installation
 
 You can either run _CoH2 Live Stats_ as a standalone bundled application or install and run it with Python.
 
-### Run Bundle [Recommended]
+### Run Bundle [Windows Recommended]
 
 1. [Download](https://github.com/brofi/coh2-live-stats/releases) latest release of _CoH2LiveStats-bundle-[version].zip_
 2. Unzip and run _CoH2LiveStats.exe_
 
+### Install from PyPI [Linux Recommended]
+1. Run `pip install coh2-live-stats`
+2. Run `python -m coh2_live_stats` or simply `coh2livestats`
+
 
 ### Install from source
 
 1. Get source code
    * [Download](https://github.com/brofi/coh2-live-stats/archive/refs/heads/master.zip) source files and unzip
    * **_or_** download and install [Git](https://git-scm.com/download/win) and run `git clone https://github.com/brofi/coh2-live-stats.git`
 2. Download and install [Python](https://www.python.org/downloads/windows/) >= 3.12
```

### Comparing `coh2_live_stats-1.2.0/README.md` & `coh2_live_stats-1.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # <img src="src/coh2_live_stats/res/coh2_live_stats.ico" alt="Icon" width="64" align="center"/> CoH2 Live Stats
 
 [![CI branch master](https://github.com/brofi/coh2-live-stats/actions/workflows/ci.yml/badge.svg)](https://github.com/brofi/coh2-live-stats/actions/workflows/ci.yml)
+[![pypi](https://img.shields.io/pypi/v/coh2-live-stats)](https://pypi.org/project/coh2-live-stats/)
+[![versions](https://img.shields.io/pypi/pyversions/coh2-live-stats)](https://github.com/brofi/coh2-live-stats)
+[![license](https://img.shields.io/github/license/brofi/coh2-live-stats)](https://github.com/brofi/coh2-live-stats/blob/master/COPYING)
+
 
 [//]: # (<mark_description>)
 
 Show player and team stats of a currently played, replayed or last played Company of Heroes 2 match.
 
 [//]: # (</mark_description>)
 
@@ -15,19 +19,23 @@
 with [gruvbox](https://github.com/morhetz/gruvbox) colors
 and [Inconsolata](https://github.com/googlefonts/Inconsolata) font.
 
 ## Installation
 
 You can either run _CoH2 Live Stats_ as a standalone bundled application or install and run it with Python.
 
-### Run Bundle [Recommended]
+### Run Bundle [Windows Recommended]
 
 1. [Download](https://github.com/brofi/coh2-live-stats/releases) latest release of _CoH2LiveStats-bundle-[version].zip_
 2. Unzip and run _CoH2LiveStats.exe_
 
+### Install from PyPI [Linux Recommended]
+1. Run `pip install coh2-live-stats`
+2. Run `python -m coh2_live_stats` or simply `coh2livestats`
+
 
 ### Install from source
 
 1. Get source code
    * [Download](https://github.com/brofi/coh2-live-stats/archive/refs/heads/master.zip) source files and unzip
    * **_or_** download and install [Git](https://git-scm.com/download/win) and run `git clone https://github.com/brofi/coh2-live-stats.git`
 2. Download and install [Python](https://www.python.org/downloads/windows/) >= 3.12
```

### Comparing `coh2_live_stats-1.2.0/pyproject.toml` & `coh2_live_stats-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 license = { file = "COPYING" }
 keywords = ["CoH2", "Company of Heroes 2"]
 classifiers = [
     "Environment :: Console",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3 :: Only ",
+    "Programming Language :: Python :: 3.12",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
     "Topic :: Games/Entertainment :: Real Time Strategy"
 ]
 [project.urls]
 Homepage = 'https://github.com/brofi/coh2-live-stats'
 Documentation = 'https://github.com/brofi/coh2-live-stats'
```

### Comparing `coh2_live_stats-1.2.0/scripts/__init__.py` & `coh2_live_stats-1.2.1/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/scripts/github_actions/__init__.py` & `coh2_live_stats-1.2.1/scripts/github_actions/__init__.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/scripts/github_actions/activate.py` & `coh2_live_stats-1.2.1/scripts/github_actions/activate.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/scripts/github_actions/mock_logfile.py` & `coh2_live_stats-1.2.1/scripts/github_actions/mock_logfile.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/scripts/pyinstaller_setup.py` & `coh2_live_stats-1.2.1/scripts/pyinstaller_setup.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/scripts/readme_generator.py` & `coh2_live_stats-1.2.1/scripts/readme_generator.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/scripts/script_util.py` & `coh2_live_stats-1.2.1/scripts/script_util.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/scripts/settings_generator.py` & `coh2_live_stats-1.2.1/scripts/settings_generator.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/src/coh2_live_stats/__init__.py` & `coh2_live_stats-1.2.1/src/coh2_live_stats/__init__.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/src/coh2_live_stats/__main__.py` & `coh2_live_stats-1.2.1/src/coh2_live_stats/__main__.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/src/coh2_live_stats/_logging.toml` & `coh2_live_stats-1.2.1/src/coh2_live_stats/_logging.toml`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/src/coh2_live_stats/coh2api.py` & `coh2_live_stats-1.2.1/src/coh2_live_stats/coh2api.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/src/coh2_live_stats/data/__init__.py` & `coh2_live_stats-1.2.1/src/coh2_live_stats/data/__init__.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/src/coh2_live_stats/data/color.py` & `coh2_live_stats-1.2.1/src/coh2_live_stats/data/color.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/src/coh2_live_stats/data/countries.py` & `coh2_live_stats-1.2.1/src/coh2_live_stats/data/countries.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/src/coh2_live_stats/data/faction.py` & `coh2_live_stats-1.2.1/src/coh2_live_stats/data/faction.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/src/coh2_live_stats/data/match.py` & `coh2_live_stats-1.2.1/src/coh2_live_stats/data/match.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/src/coh2_live_stats/data/player.py` & `coh2_live_stats-1.2.1/src/coh2_live_stats/data/player.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/src/coh2_live_stats/data/team.py` & `coh2_live_stats-1.2.1/src/coh2_live_stats/data/team.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/src/coh2_live_stats/logging_conf.py` & `coh2_live_stats-1.2.1/src/coh2_live_stats/logging_conf.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/src/coh2_live_stats/output.py` & `coh2_live_stats-1.2.1/src/coh2_live_stats/output.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/src/coh2_live_stats/res/coh2_live_stats.ico` & `coh2_live_stats-1.2.1/src/coh2_live_stats/res/coh2_live_stats.ico`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/src/coh2_live_stats/res/coh2_live_stats.xcf` & `coh2_live_stats-1.2.1/src/coh2_live_stats/res/coh2_live_stats.xcf`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/src/coh2_live_stats/res/example_0.svg` & `coh2_live_stats-1.2.1/src/coh2_live_stats/res/example_0.svg`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/src/coh2_live_stats/res/example_1.svg` & `coh2_live_stats-1.2.1/src/coh2_live_stats/res/example_1.svg`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/src/coh2_live_stats/res/example_default.svg` & `coh2_live_stats-1.2.1/src/coh2_live_stats/res/example_default.svg`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/src/coh2_live_stats/res/horn.wav` & `coh2_live_stats-1.2.1/src/coh2_live_stats/res/horn.wav`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/src/coh2_live_stats/res/horn_epic.wav` & `coh2_live_stats-1.2.1/src/coh2_live_stats/res/horn_epic.wav`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/src/coh2_live_stats/res/horn_subtle.wav` & `coh2_live_stats-1.2.1/src/coh2_live_stats/res/horn_subtle.wav`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/src/coh2_live_stats/settings.py` & `coh2_live_stats-1.2.1/src/coh2_live_stats/settings.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/src/coh2_live_stats/util.py` & `coh2_live_stats-1.2.1/src/coh2_live_stats/util.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/src/coh2_live_stats.egg-info/PKG-INFO` & `coh2_live_stats-1.2.1/src/coh2_live_stats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coh2_live_stats
-Version: 1.2.0
+Version: 1.2.1
 Summary: Show player and team stats of a currently played, replayed or last played Company of Heroes 2 match.
 Author-email: Andreas Becker <brofi.archlinux@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -682,14 +682,16 @@
 Project-URL: Issues, https://github.com/brofi/coh2-live-stats/issues
 Project-URL: Source, https://github.com/brofi/coh2-live-stats
 Keywords: CoH2,Company of Heroes 2
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only 
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Games/Entertainment :: Real Time Strategy
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: COPYING
 Requires-Dist: colorama>=0.4.6
@@ -710,14 +712,18 @@
 Requires-Dist: respx>=0.21.1; extra == "build"
 Requires-Dist: tomlkit>=0.12.4; extra == "build"
 Requires-Dist: twine>=5.0.0; extra == "build"
 
 # <img src="src/coh2_live_stats/res/coh2_live_stats.ico" alt="Icon" width="64" align="center"/> CoH2 Live Stats
 
 [![CI branch master](https://github.com/brofi/coh2-live-stats/actions/workflows/ci.yml/badge.svg)](https://github.com/brofi/coh2-live-stats/actions/workflows/ci.yml)
+[![pypi](https://img.shields.io/pypi/v/coh2-live-stats)](https://pypi.org/project/coh2-live-stats/)
+[![versions](https://img.shields.io/pypi/pyversions/coh2-live-stats)](https://github.com/brofi/coh2-live-stats)
+[![license](https://img.shields.io/github/license/brofi/coh2-live-stats)](https://github.com/brofi/coh2-live-stats/blob/master/COPYING)
+
 
 [//]: # (<mark_description>)
 
 Show player and team stats of a currently played, replayed or last played Company of Heroes 2 match.
 
 [//]: # (</mark_description>)
 
@@ -728,19 +734,23 @@
 with [gruvbox](https://github.com/morhetz/gruvbox) colors
 and [Inconsolata](https://github.com/googlefonts/Inconsolata) font.
 
 ## Installation
 
 You can either run _CoH2 Live Stats_ as a standalone bundled application or install and run it with Python.
 
-### Run Bundle [Recommended]
+### Run Bundle [Windows Recommended]
 
 1. [Download](https://github.com/brofi/coh2-live-stats/releases) latest release of _CoH2LiveStats-bundle-[version].zip_
 2. Unzip and run _CoH2LiveStats.exe_
 
+### Install from PyPI [Linux Recommended]
+1. Run `pip install coh2-live-stats`
+2. Run `python -m coh2_live_stats` or simply `coh2livestats`
+
 
 ### Install from source
 
 1. Get source code
    * [Download](https://github.com/brofi/coh2-live-stats/archive/refs/heads/master.zip) source files and unzip
    * **_or_** download and install [Git](https://git-scm.com/download/win) and run `git clone https://github.com/brofi/coh2-live-stats.git`
 2. Download and install [Python](https://www.python.org/downloads/windows/) >= 3.12
```

### Comparing `coh2_live_stats-1.2.0/src/coh2_live_stats.egg-info/SOURCES.txt` & `coh2_live_stats-1.2.1/src/coh2_live_stats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/tasks.py` & `coh2_live_stats-1.2.1/tasks.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/tests/__init__.py` & `coh2_live_stats-1.2.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/tests/conftest.py` & `coh2_live_stats-1.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/tests/test_api.py` & `coh2_live_stats-1.2.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/tests/test_logfile_parsing.py` & `coh2_live_stats-1.2.1/tests/test_logfile_parsing.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/tests/test_output.py` & `coh2_live_stats-1.2.1/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/tests/test_settings.py` & `coh2_live_stats-1.2.1/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.0/tests/test_util.py` & `coh2_live_stats-1.2.1/tests/test_util.py`

 * *Files identical despite different names*

