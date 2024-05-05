# Comparing `tmp/coh2_live_stats-1.2.2.tar.gz` & `tmp/coh2_live_stats-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coh2_live_stats-1.2.2.tar", last modified: Sun May  5 01:54:00 2024, max compression
+gzip compressed data, was "coh2_live_stats-1.2.3.tar", last modified: Sun May  5 02:03:40 2024, max compression
```

## Comparing `coh2_live_stats-1.2.2.tar` & `coh2_live_stats-1.2.3.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 01:54:00.219108 coh2_live_stats-1.2.2/
-drwxrwxrwx   0        0        0        0 2024-05-05 01:54:00.076976 coh2_live_stats-1.2.2/.github/
-drwxrwxrwx   0        0        0        0 2024-05-05 01:54:00.089977 coh2_live_stats-1.2.2/.github/workflows/
--rw-rw-rw-   0        0        0     2869 2024-05-04 20:48:37.000000 coh2_live_stats-1.2.2/.github/workflows/ci.yml
--rw-rw-rw-   0        0        0      989 2024-05-04 22:37:31.000000 coh2_live_stats-1.2.2/.github/workflows/publish.yml
--rw-rw-rw-   0        0        0      250 2024-05-04 20:48:37.000000 coh2_live_stats-1.2.2/.gitignore
--rw-rw-rw-   0        0        0      378 2024-04-25 10:43:22.000000 coh2_live_stats-1.2.2/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0    35821 2024-02-16 20:40:58.000000 coh2_live_stats-1.2.2/COPYING
--rw-rw-rw-   0        0        0    83824 2024-05-05 01:54:00.218109 coh2_live_stats-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0    40738 2024-05-05 01:46:36.000000 coh2_live_stats-1.2.2/README.md
--rw-rw-rw-   0        0        0      127 2024-04-08 09:48:24.000000 coh2_live_stats-1.2.2/invoke.yml
--rw-rw-rw-   0        0        0     4885 2024-05-04 23:11:47.000000 coh2_live_stats-1.2.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-05 01:54:00.096990 coh2_live_stats-1.2.2/scripts/
--rw-rw-rw-   0        0        0      761 2024-05-04 20:48:37.000000 coh2_live_stats-1.2.2/scripts/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 01:54:00.099987 coh2_live_stats-1.2.2/scripts/github_actions/
--rw-rw-rw-   0        0        0      772 2024-05-04 20:48:37.000000 coh2_live_stats-1.2.2/scripts/github_actions/__init__.py
--rw-rw-rw-   0        0        0     1382 2024-05-04 20:48:37.000000 coh2_live_stats-1.2.2/scripts/github_actions/activate.py
--rw-rw-rw-   0        0        0     1351 2024-05-04 20:48:37.000000 coh2_live_stats-1.2.2/scripts/github_actions/mock_logfile.py
--rw-rw-rw-   0        0        0     5901 2024-05-04 20:48:37.000000 coh2_live_stats-1.2.2/scripts/pyinstaller_setup.py
--rw-rw-rw-   0        0        0    20438 2024-05-05 01:37:08.000000 coh2_live_stats-1.2.2/scripts/readme_generator.py
--rw-rw-rw-   0        0        0     2862 2024-05-04 20:48:37.000000 coh2_live_stats-1.2.2/scripts/script_util.py
--rw-rw-rw-   0        0        0     3775 2024-05-04 20:48:37.000000 coh2_live_stats-1.2.2/scripts/settings_generator.py
--rw-rw-rw-   0        0        0       42 2024-05-05 01:54:00.220111 coh2_live_stats-1.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-05 01:54:00.078977 coh2_live_stats-1.2.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-05 01:54:00.126182 coh2_live_stats-1.2.2/src/coh2_live_stats/
--rw-rw-rw-   0        0        0      758 2024-04-25 08:51:26.000000 coh2_live_stats-1.2.2/src/coh2_live_stats/__init__.py
--rw-rw-rw-   0        0        0    10336 2024-05-04 20:48:37.000000 coh2_live_stats-1.2.2/src/coh2_live_stats/__main__.py
--rw-rw-rw-   0        0        0     6753 2024-05-05 01:53:52.000000 coh2_live_stats-1.2.2/src/coh2_live_stats/_coh2livestats.toml
--rw-rw-rw-   0        0        0     1197 2024-04-13 19:30:05.000000 coh2_live_stats-1.2.2/src/coh2_live_stats/_logging.toml
--rw-rw-rw-   0        0        0    10736 2024-05-04 20:48:37.000000 coh2_live_stats-1.2.2/src/coh2_live_stats/coh2api.py
-drwxrwxrwx   0        0        0        0 2024-05-05 01:54:00.173221 coh2_live_stats-1.2.2/src/coh2_live_stats/data/
--rw-rw-rw-   0        0        0      787 2024-04-15 17:58:04.000000 coh2_live_stats-1.2.2/src/coh2_live_stats/data/__init__.py
--rw-rw-rw-   0        0        0     1775 2024-04-25 11:33:29.000000 coh2_live_stats-1.2.2/src/coh2_live_stats/data/color.py
--rw-rw-rw-   0        0        0     7112 2024-04-16 03:38:58.000000 coh2_live_stats-1.2.2/src/coh2_live_stats/data/countries.py
--rw-rw-rw-   0        0        0     4003 2024-04-22 03:42:09.000000 coh2_live_stats-1.2.2/src/coh2_live_stats/data/faction.py
--rw-rw-rw-   0        0        0     6703 2024-04-25 10:32:48.000000 coh2_live_stats-1.2.2/src/coh2_live_stats/data/match.py
--rw-rw-rw-   0        0        0     6083 2024-05-01 04:55:24.000000 coh2_live_stats-1.2.2/src/coh2_live_stats/data/player.py
--rw-rw-rw-   0        0        0     1755 2024-04-20 11:18:33.000000 coh2_live_stats-1.2.2/src/coh2_live_stats/data/team.py
--rw-rw-rw-   0        0        0     8117 2024-05-04 20:48:37.000000 coh2_live_stats-1.2.2/src/coh2_live_stats/logging_conf.py
--rw-rw-rw-   0        0        0    16104 2024-05-04 20:48:37.000000 coh2_live_stats-1.2.2/src/coh2_live_stats/output.py
--rw-rw-rw-   0        0        0        0 2024-04-14 11:11:19.000000 coh2_live_stats-1.2.2/src/coh2_live_stats/py.typed
-drwxrwxrwx   0        0        0        0 2024-05-05 01:54:00.200705 coh2_live_stats-1.2.2/src/coh2_live_stats/res/
--rw-rw-rw-   0        0        0  8231670 2024-02-19 03:47:36.000000 coh2_live_stats-1.2.2/src/coh2_live_stats/res/coh2_live_stats.ico
--rw-rw-rw-   0        0        0   806942 2024-02-19 03:49:04.000000 coh2_live_stats-1.2.2/src/coh2_live_stats/res/coh2_live_stats.xcf
--rw-rw-rw-   0        0        0    24366 2024-05-05 01:40:24.000000 coh2_live_stats-1.2.2/src/coh2_live_stats/res/example_0.svg
--rw-rw-rw-   0        0        0      963 2024-05-05 01:40:24.000000 coh2_live_stats-1.2.2/src/coh2_live_stats/res/example_1.svg
--rw-rw-rw-   0        0        0    25637 2024-05-05 01:40:24.000000 coh2_live_stats-1.2.2/src/coh2_live_stats/res/example_default.svg
--rw-rw-rw-   0        0        0   806504 2024-03-02 02:13:46.000000 coh2_live_stats-1.2.2/src/coh2_live_stats/res/horn.wav
--rw-rw-rw-   0        0        0  1267392 2024-03-02 02:13:55.000000 coh2_live_stats-1.2.2/src/coh2_live_stats/res/horn_epic.wav
--rw-rw-rw-   0        0        0  1175232 2024-03-02 02:13:42.000000 coh2_live_stats-1.2.2/src/coh2_live_stats/res/horn_subtle.wav
--rw-rw-rw-   0        0        0    12953 2024-05-04 20:48:37.000000 coh2_live_stats-1.2.2/src/coh2_live_stats/settings.py
--rw-rw-rw-   0        0        0     2465 2024-05-04 20:48:37.000000 coh2_live_stats-1.2.2/src/coh2_live_stats/util.py
--rw-rw-rw-   0        0        0      427 2024-05-05 01:53:59.000000 coh2_live_stats-1.2.2/src/coh2_live_stats/version.py
-drwxrwxrwx   0        0        0        0 2024-05-05 01:54:00.213659 coh2_live_stats-1.2.2/src/coh2_live_stats.egg-info/
--rw-rw-rw-   0        0        0    83824 2024-05-05 01:53:59.000000 coh2_live_stats-1.2.2/src/coh2_live_stats.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1725 2024-05-05 01:54:00.000000 coh2_live_stats-1.2.2/src/coh2_live_stats.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 01:53:59.000000 coh2_live_stats-1.2.2/src/coh2_live_stats.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-05-05 01:53:59.000000 coh2_live_stats-1.2.2/src/coh2_live_stats.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      276 2024-05-05 01:53:59.000000 coh2_live_stats-1.2.2/src/coh2_live_stats.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-05 01:53:59.000000 coh2_live_stats-1.2.2/src/coh2_live_stats.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8056 2024-05-05 01:53:01.000000 coh2_live_stats-1.2.2/tasks.py
-drwxrwxrwx   0        0        0        0 2024-05-05 01:54:00.212670 coh2_live_stats-1.2.2/tests/
--rw-rw-rw-   0        0        0      758 2024-04-15 18:02:00.000000 coh2_live_stats-1.2.2/tests/__init__.py
--rw-rw-rw-   0        0        0     3958 2024-04-27 03:22:15.000000 coh2_live_stats-1.2.2/tests/conftest.py
--rw-rw-rw-   0        0        0      528 2024-04-22 03:42:09.000000 coh2_live_stats-1.2.2/tests/ruff.toml
--rw-rw-rw-   0        0        0    31853 2024-05-01 02:32:07.000000 coh2_live_stats-1.2.2/tests/test_api.py
--rw-rw-rw-   0        0        0     4479 2024-05-04 20:48:37.000000 coh2_live_stats-1.2.2/tests/test_logfile_parsing.py
--rw-rw-rw-   0        0        0    10246 2024-05-01 21:31:21.000000 coh2_live_stats-1.2.2/tests/test_output.py
--rw-rw-rw-   0        0        0     3558 2024-04-24 05:22:19.000000 coh2_live_stats-1.2.2/tests/test_settings.py
--rw-rw-rw-   0        0        0     2060 2024-05-04 01:05:47.000000 coh2_live_stats-1.2.2/tests/test_util.py
+drwxrwxrwx   0        0        0        0 2024-05-05 02:03:40.855939 coh2_live_stats-1.2.3/
+drwxrwxrwx   0        0        0        0 2024-05-05 02:03:40.732487 coh2_live_stats-1.2.3/.github/
+drwxrwxrwx   0        0        0        0 2024-05-05 02:03:40.745487 coh2_live_stats-1.2.3/.github/workflows/
+-rw-rw-rw-   0        0        0     2869 2024-05-04 20:48:37.000000 coh2_live_stats-1.2.3/.github/workflows/ci.yml
+-rw-rw-rw-   0        0        0      989 2024-05-04 22:37:31.000000 coh2_live_stats-1.2.3/.github/workflows/publish.yml
+-rw-rw-rw-   0        0        0      250 2024-05-04 20:48:37.000000 coh2_live_stats-1.2.3/.gitignore
+-rw-rw-rw-   0        0        0      378 2024-04-25 10:43:22.000000 coh2_live_stats-1.2.3/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0    35821 2024-02-16 20:40:58.000000 coh2_live_stats-1.2.3/COPYING
+-rw-rw-rw-   0        0        0    83813 2024-05-05 02:03:40.854939 coh2_live_stats-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0    40727 2024-05-05 02:02:00.000000 coh2_live_stats-1.2.3/README.md
+-rw-rw-rw-   0        0        0      127 2024-04-08 09:48:24.000000 coh2_live_stats-1.2.3/invoke.yml
+-rw-rw-rw-   0        0        0     4885 2024-05-04 23:11:47.000000 coh2_live_stats-1.2.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-05 02:03:40.750492 coh2_live_stats-1.2.3/scripts/
+-rw-rw-rw-   0        0        0      761 2024-05-04 20:48:37.000000 coh2_live_stats-1.2.3/scripts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 02:03:40.753500 coh2_live_stats-1.2.3/scripts/github_actions/
+-rw-rw-rw-   0        0        0      772 2024-05-04 20:48:37.000000 coh2_live_stats-1.2.3/scripts/github_actions/__init__.py
+-rw-rw-rw-   0        0        0     1382 2024-05-04 20:48:37.000000 coh2_live_stats-1.2.3/scripts/github_actions/activate.py
+-rw-rw-rw-   0        0        0     1351 2024-05-04 20:48:37.000000 coh2_live_stats-1.2.3/scripts/github_actions/mock_logfile.py
+-rw-rw-rw-   0        0        0     5901 2024-05-04 20:48:37.000000 coh2_live_stats-1.2.3/scripts/pyinstaller_setup.py
+-rw-rw-rw-   0        0        0    20436 2024-05-05 01:59:58.000000 coh2_live_stats-1.2.3/scripts/readme_generator.py
+-rw-rw-rw-   0        0        0     2862 2024-05-04 20:48:37.000000 coh2_live_stats-1.2.3/scripts/script_util.py
+-rw-rw-rw-   0        0        0     3775 2024-05-04 20:48:37.000000 coh2_live_stats-1.2.3/scripts/settings_generator.py
+-rw-rw-rw-   0        0        0       42 2024-05-05 02:03:40.856927 coh2_live_stats-1.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-05 02:03:40.734489 coh2_live_stats-1.2.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-05 02:03:40.778103 coh2_live_stats-1.2.3/src/coh2_live_stats/
+-rw-rw-rw-   0        0        0      758 2024-04-25 08:51:26.000000 coh2_live_stats-1.2.3/src/coh2_live_stats/__init__.py
+-rw-rw-rw-   0        0        0    10336 2024-05-04 20:48:37.000000 coh2_live_stats-1.2.3/src/coh2_live_stats/__main__.py
+-rw-rw-rw-   0        0        0     6753 2024-05-05 02:03:33.000000 coh2_live_stats-1.2.3/src/coh2_live_stats/_coh2livestats.toml
+-rw-rw-rw-   0        0        0     1197 2024-04-13 19:30:05.000000 coh2_live_stats-1.2.3/src/coh2_live_stats/_logging.toml
+-rw-rw-rw-   0        0        0    10736 2024-05-04 20:48:37.000000 coh2_live_stats-1.2.3/src/coh2_live_stats/coh2api.py
+drwxrwxrwx   0        0        0        0 2024-05-05 02:03:40.815052 coh2_live_stats-1.2.3/src/coh2_live_stats/data/
+-rw-rw-rw-   0        0        0      787 2024-04-15 17:58:04.000000 coh2_live_stats-1.2.3/src/coh2_live_stats/data/__init__.py
+-rw-rw-rw-   0        0        0     1775 2024-04-25 11:33:29.000000 coh2_live_stats-1.2.3/src/coh2_live_stats/data/color.py
+-rw-rw-rw-   0        0        0     7112 2024-04-16 03:38:58.000000 coh2_live_stats-1.2.3/src/coh2_live_stats/data/countries.py
+-rw-rw-rw-   0        0        0     4003 2024-04-22 03:42:09.000000 coh2_live_stats-1.2.3/src/coh2_live_stats/data/faction.py
+-rw-rw-rw-   0        0        0     6703 2024-04-25 10:32:48.000000 coh2_live_stats-1.2.3/src/coh2_live_stats/data/match.py
+-rw-rw-rw-   0        0        0     6083 2024-05-01 04:55:24.000000 coh2_live_stats-1.2.3/src/coh2_live_stats/data/player.py
+-rw-rw-rw-   0        0        0     1755 2024-04-20 11:18:33.000000 coh2_live_stats-1.2.3/src/coh2_live_stats/data/team.py
+-rw-rw-rw-   0        0        0     8117 2024-05-04 20:48:37.000000 coh2_live_stats-1.2.3/src/coh2_live_stats/logging_conf.py
+-rw-rw-rw-   0        0        0    16104 2024-05-04 20:48:37.000000 coh2_live_stats-1.2.3/src/coh2_live_stats/output.py
+-rw-rw-rw-   0        0        0        0 2024-04-14 11:11:19.000000 coh2_live_stats-1.2.3/src/coh2_live_stats/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-05 02:03:40.839940 coh2_live_stats-1.2.3/src/coh2_live_stats/res/
+-rw-rw-rw-   0        0        0  8231670 2024-02-19 03:47:36.000000 coh2_live_stats-1.2.3/src/coh2_live_stats/res/coh2_live_stats.ico
+-rw-rw-rw-   0        0        0   806942 2024-02-19 03:49:04.000000 coh2_live_stats-1.2.3/src/coh2_live_stats/res/coh2_live_stats.xcf
+-rw-rw-rw-   0        0        0    24366 2024-05-05 01:40:24.000000 coh2_live_stats-1.2.3/src/coh2_live_stats/res/example_0.svg
+-rw-rw-rw-   0        0        0      963 2024-05-05 01:40:24.000000 coh2_live_stats-1.2.3/src/coh2_live_stats/res/example_1.svg
+-rw-rw-rw-   0        0        0    25637 2024-05-05 01:40:24.000000 coh2_live_stats-1.2.3/src/coh2_live_stats/res/example_default.svg
+-rw-rw-rw-   0        0        0   806504 2024-03-02 02:13:46.000000 coh2_live_stats-1.2.3/src/coh2_live_stats/res/horn.wav
+-rw-rw-rw-   0        0        0  1267392 2024-03-02 02:13:55.000000 coh2_live_stats-1.2.3/src/coh2_live_stats/res/horn_epic.wav
+-rw-rw-rw-   0        0        0  1175232 2024-03-02 02:13:42.000000 coh2_live_stats-1.2.3/src/coh2_live_stats/res/horn_subtle.wav
+-rw-rw-rw-   0        0        0    12953 2024-05-04 20:48:37.000000 coh2_live_stats-1.2.3/src/coh2_live_stats/settings.py
+-rw-rw-rw-   0        0        0     2465 2024-05-04 20:48:37.000000 coh2_live_stats-1.2.3/src/coh2_live_stats/util.py
+-rw-rw-rw-   0        0        0      427 2024-05-05 02:03:40.000000 coh2_live_stats-1.2.3/src/coh2_live_stats/version.py
+drwxrwxrwx   0        0        0        0 2024-05-05 02:03:40.851928 coh2_live_stats-1.2.3/src/coh2_live_stats.egg-info/
+-rw-rw-rw-   0        0        0    83813 2024-05-05 02:03:40.000000 coh2_live_stats-1.2.3/src/coh2_live_stats.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1725 2024-05-05 02:03:40.000000 coh2_live_stats-1.2.3/src/coh2_live_stats.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 02:03:40.000000 coh2_live_stats-1.2.3/src/coh2_live_stats.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-05-05 02:03:40.000000 coh2_live_stats-1.2.3/src/coh2_live_stats.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      276 2024-05-05 02:03:40.000000 coh2_live_stats-1.2.3/src/coh2_live_stats.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-05 02:03:40.000000 coh2_live_stats-1.2.3/src/coh2_live_stats.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8056 2024-05-05 01:53:01.000000 coh2_live_stats-1.2.3/tasks.py
+drwxrwxrwx   0        0        0        0 2024-05-05 02:03:40.850928 coh2_live_stats-1.2.3/tests/
+-rw-rw-rw-   0        0        0      758 2024-04-15 18:02:00.000000 coh2_live_stats-1.2.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     3958 2024-04-27 03:22:15.000000 coh2_live_stats-1.2.3/tests/conftest.py
+-rw-rw-rw-   0        0        0      528 2024-04-22 03:42:09.000000 coh2_live_stats-1.2.3/tests/ruff.toml
+-rw-rw-rw-   0        0        0    31853 2024-05-01 02:32:07.000000 coh2_live_stats-1.2.3/tests/test_api.py
+-rw-rw-rw-   0        0        0     4479 2024-05-04 20:48:37.000000 coh2_live_stats-1.2.3/tests/test_logfile_parsing.py
+-rw-rw-rw-   0        0        0    10246 2024-05-01 21:31:21.000000 coh2_live_stats-1.2.3/tests/test_output.py
+-rw-rw-rw-   0        0        0     3558 2024-04-24 05:22:19.000000 coh2_live_stats-1.2.3/tests/test_settings.py
+-rw-rw-rw-   0        0        0     2060 2024-05-04 01:05:47.000000 coh2_live_stats-1.2.3/tests/test_util.py
```

### Comparing `coh2_live_stats-1.2.2/.github/workflows/ci.yml` & `coh2_live_stats-1.2.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/.github/workflows/publish.yml` & `coh2_live_stats-1.2.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/COPYING` & `coh2_live_stats-1.2.3/COPYING`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/PKG-INFO` & `coh2_live_stats-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coh2_live_stats
-Version: 1.2.2
+Version: 1.2.3
 Summary: Show player and team stats of a currently played, replayed or last played Company of Heroes 2 match.
 Author-email: Andreas Becker <brofi.archlinux@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -709,15 +709,15 @@
 Requires-Dist: pyinstaller>=6.6.0; extra == "build"
 Requires-Dist: pytest>=8.1.1; extra == "build"
 Requires-Dist: pytest-asyncio>=0.23.6; extra == "build"
 Requires-Dist: respx>=0.21.1; extra == "build"
 Requires-Dist: tomlkit>=0.12.4; extra == "build"
 Requires-Dist: twine>=5.0.0; extra == "build"
 
-# <img src="https://raw.githubusercontent.com/brofi/coh2-live-stats/master/src/coh2_live_stats/res/coh2_live_stats.ico" alt="Icon" width="64" align="center"/> CoH2 Live Stats
+# <img src="https://raw.githubusercontent.com/brofi/coh2-live-stats/master/src/coh2_live_stats/res/coh2_live_stats.ico" width="64" align="center"/> CoH2 Live Stats
 
 [![CI branch master](https://github.com/brofi/coh2-live-stats/actions/workflows/ci.yml/badge.svg)](https://github.com/brofi/coh2-live-stats/actions/workflows/ci.yml)
 [![pypi](https://img.shields.io/pypi/v/coh2-live-stats)](https://pypi.org/project/coh2-live-stats/)
 [![versions](https://img.shields.io/pypi/pyversions/coh2-live-stats)](https://github.com/brofi/coh2-live-stats)
 [![license](https://img.shields.io/github/license/brofi/coh2-live-stats)](https://github.com/brofi/coh2-live-stats/blob/master/COPYING)
```

### Comparing `coh2_live_stats-1.2.2/README.md` & `coh2_live_stats-1.2.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# <img src="https://raw.githubusercontent.com/brofi/coh2-live-stats/master/src/coh2_live_stats/res/coh2_live_stats.ico" alt="Icon" width="64" align="center"/> CoH2 Live Stats
+# <img src="https://raw.githubusercontent.com/brofi/coh2-live-stats/master/src/coh2_live_stats/res/coh2_live_stats.ico" width="64" align="center"/> CoH2 Live Stats
 
 [![CI branch master](https://github.com/brofi/coh2-live-stats/actions/workflows/ci.yml/badge.svg)](https://github.com/brofi/coh2-live-stats/actions/workflows/ci.yml)
 [![pypi](https://img.shields.io/pypi/v/coh2-live-stats)](https://pypi.org/project/coh2-live-stats/)
 [![versions](https://img.shields.io/pypi/pyversions/coh2-live-stats)](https://github.com/brofi/coh2-live-stats)
 [![license](https://img.shields.io/github/license/brofi/coh2-live-stats)](https://github.com/brofi/coh2-live-stats/blob/master/COPYING)
```

### Comparing `coh2_live_stats-1.2.2/pyproject.toml` & `coh2_live_stats-1.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/scripts/__init__.py` & `coh2_live_stats-1.2.3/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/scripts/github_actions/__init__.py` & `coh2_live_stats-1.2.3/scripts/github_actions/__init__.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/scripts/github_actions/activate.py` & `coh2_live_stats-1.2.3/scripts/github_actions/activate.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/scripts/github_actions/mock_logfile.py` & `coh2_live_stats-1.2.3/scripts/github_actions/mock_logfile.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/scripts/pyinstaller_setup.py` & `coh2_live_stats-1.2.3/scripts/pyinstaller_setup.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/scripts/readme_generator.py` & `coh2_live_stats-1.2.3/scripts/readme_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -598,16 +598,16 @@
             '\n#### Description\n\n'
             f'{example[0]}\n'
             '\n#### TOML configuration\n\n'
             '```toml\n'
             f'{'\n'.join(example[1])}\n'
             '```\n'
             '\n#### Resulting output\n\n'
-            f'![Example output]('
-            f'https://raw.githubusercontent.com/brofi/coh2-live-stats/master/'
+            '![Example output]('
+            'https://raw.githubusercontent.com/brofi/coh2-live-stats/master/'
             f'src/coh2_live_stats/res/example_{i}.svg)\n'
         )
     return md
 
 
 def _appendix_section() -> list[str]:
     return [
```

### Comparing `coh2_live_stats-1.2.2/scripts/script_util.py` & `coh2_live_stats-1.2.3/scripts/script_util.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/scripts/settings_generator.py` & `coh2_live_stats-1.2.3/scripts/settings_generator.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/src/coh2_live_stats/__init__.py` & `coh2_live_stats-1.2.3/src/coh2_live_stats/__init__.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/src/coh2_live_stats/__main__.py` & `coh2_live_stats-1.2.3/src/coh2_live_stats/__main__.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/src/coh2_live_stats/_coh2livestats.toml` & `coh2_live_stats-1.2.3/src/coh2_live_stats/_coh2livestats.toml`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/src/coh2_live_stats/_logging.toml` & `coh2_live_stats-1.2.3/src/coh2_live_stats/_logging.toml`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/src/coh2_live_stats/coh2api.py` & `coh2_live_stats-1.2.3/src/coh2_live_stats/coh2api.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/src/coh2_live_stats/data/__init__.py` & `coh2_live_stats-1.2.3/src/coh2_live_stats/data/__init__.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/src/coh2_live_stats/data/color.py` & `coh2_live_stats-1.2.3/src/coh2_live_stats/data/color.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/src/coh2_live_stats/data/countries.py` & `coh2_live_stats-1.2.3/src/coh2_live_stats/data/countries.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/src/coh2_live_stats/data/faction.py` & `coh2_live_stats-1.2.3/src/coh2_live_stats/data/faction.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/src/coh2_live_stats/data/match.py` & `coh2_live_stats-1.2.3/src/coh2_live_stats/data/match.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/src/coh2_live_stats/data/player.py` & `coh2_live_stats-1.2.3/src/coh2_live_stats/data/player.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/src/coh2_live_stats/data/team.py` & `coh2_live_stats-1.2.3/src/coh2_live_stats/data/team.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/src/coh2_live_stats/logging_conf.py` & `coh2_live_stats-1.2.3/src/coh2_live_stats/logging_conf.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/src/coh2_live_stats/output.py` & `coh2_live_stats-1.2.3/src/coh2_live_stats/output.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/src/coh2_live_stats/res/coh2_live_stats.ico` & `coh2_live_stats-1.2.3/src/coh2_live_stats/res/coh2_live_stats.ico`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/src/coh2_live_stats/res/coh2_live_stats.xcf` & `coh2_live_stats-1.2.3/src/coh2_live_stats/res/coh2_live_stats.xcf`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/src/coh2_live_stats/res/example_0.svg` & `coh2_live_stats-1.2.3/src/coh2_live_stats/res/example_0.svg`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/src/coh2_live_stats/res/example_1.svg` & `coh2_live_stats-1.2.3/src/coh2_live_stats/res/example_1.svg`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/src/coh2_live_stats/res/example_default.svg` & `coh2_live_stats-1.2.3/src/coh2_live_stats/res/example_default.svg`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/src/coh2_live_stats/res/horn.wav` & `coh2_live_stats-1.2.3/src/coh2_live_stats/res/horn.wav`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/src/coh2_live_stats/res/horn_epic.wav` & `coh2_live_stats-1.2.3/src/coh2_live_stats/res/horn_epic.wav`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/src/coh2_live_stats/res/horn_subtle.wav` & `coh2_live_stats-1.2.3/src/coh2_live_stats/res/horn_subtle.wav`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/src/coh2_live_stats/settings.py` & `coh2_live_stats-1.2.3/src/coh2_live_stats/settings.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/src/coh2_live_stats/util.py` & `coh2_live_stats-1.2.3/src/coh2_live_stats/util.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/src/coh2_live_stats.egg-info/PKG-INFO` & `coh2_live_stats-1.2.3/src/coh2_live_stats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coh2_live_stats
-Version: 1.2.2
+Version: 1.2.3
 Summary: Show player and team stats of a currently played, replayed or last played Company of Heroes 2 match.
 Author-email: Andreas Becker <brofi.archlinux@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -709,15 +709,15 @@
 Requires-Dist: pyinstaller>=6.6.0; extra == "build"
 Requires-Dist: pytest>=8.1.1; extra == "build"
 Requires-Dist: pytest-asyncio>=0.23.6; extra == "build"
 Requires-Dist: respx>=0.21.1; extra == "build"
 Requires-Dist: tomlkit>=0.12.4; extra == "build"
 Requires-Dist: twine>=5.0.0; extra == "build"
 
-# <img src="https://raw.githubusercontent.com/brofi/coh2-live-stats/master/src/coh2_live_stats/res/coh2_live_stats.ico" alt="Icon" width="64" align="center"/> CoH2 Live Stats
+# <img src="https://raw.githubusercontent.com/brofi/coh2-live-stats/master/src/coh2_live_stats/res/coh2_live_stats.ico" width="64" align="center"/> CoH2 Live Stats
 
 [![CI branch master](https://github.com/brofi/coh2-live-stats/actions/workflows/ci.yml/badge.svg)](https://github.com/brofi/coh2-live-stats/actions/workflows/ci.yml)
 [![pypi](https://img.shields.io/pypi/v/coh2-live-stats)](https://pypi.org/project/coh2-live-stats/)
 [![versions](https://img.shields.io/pypi/pyversions/coh2-live-stats)](https://github.com/brofi/coh2-live-stats)
 [![license](https://img.shields.io/github/license/brofi/coh2-live-stats)](https://github.com/brofi/coh2-live-stats/blob/master/COPYING)
```

### Comparing `coh2_live_stats-1.2.2/src/coh2_live_stats.egg-info/SOURCES.txt` & `coh2_live_stats-1.2.3/src/coh2_live_stats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/tasks.py` & `coh2_live_stats-1.2.3/tasks.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/tests/__init__.py` & `coh2_live_stats-1.2.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/tests/conftest.py` & `coh2_live_stats-1.2.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/tests/ruff.toml` & `coh2_live_stats-1.2.3/tests/ruff.toml`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/tests/test_api.py` & `coh2_live_stats-1.2.3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/tests/test_logfile_parsing.py` & `coh2_live_stats-1.2.3/tests/test_logfile_parsing.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/tests/test_output.py` & `coh2_live_stats-1.2.3/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/tests/test_settings.py` & `coh2_live_stats-1.2.3/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `coh2_live_stats-1.2.2/tests/test_util.py` & `coh2_live_stats-1.2.3/tests/test_util.py`

 * *Files identical despite different names*

