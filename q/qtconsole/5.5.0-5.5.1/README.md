# Comparing `tmp/qtconsole-5.5.0.tar.gz` & `tmp/qtconsole-5.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtconsole-5.5.0.tar", last modified: Mon Nov  6 02:38:54 2023, max compression
+gzip compressed data, was "qtconsole-5.5.1.tar", last modified: Wed Nov 15 22:57:05 2023, max compression
```

## Comparing `qtconsole-5.5.0.tar` & `qtconsole-5.5.1.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-11-06 02:38:54.009891 qtconsole-5.5.0/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       44 2020-10-24 15:40:21.000000 qtconsole-5.5.0/.coveragerc
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-11-06 02:38:53.981890 qtconsole-5.5.0/.github/
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-11-06 02:38:53.985890 qtconsole-5.5.0/.github/workflows/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2621 2023-10-19 15:09:05.000000 qtconsole-5.5.0/.github/workflows/linux-tests.yml
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1347 2023-10-19 15:09:05.000000 qtconsole-5.5.0/.github/workflows/macos-tests.yml
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1361 2023-10-19 15:09:05.000000 qtconsole-5.5.0/.github/workflows/windows-tests.yml
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      350 2023-05-05 17:34:26.000000 qtconsole-5.5.0/.gitignore
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    10807 2015-12-20 14:40:14.000000 qtconsole-5.5.0/.mailmap
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      624 2022-03-27 18:25:58.000000 qtconsole-5.5.0/CONTRIBUTING.md
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1528 2020-10-24 15:40:21.000000 qtconsole-5.5.0/LICENSE
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      371 2020-10-24 15:40:21.000000 qtconsole-5.5.0/MANIFEST.in
--rw-r--r--   0 carlos    (1000) carlos    (1000)     5056 2023-11-06 02:38:54.009891 qtconsole-5.5.0/PKG-INFO
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3661 2023-09-01 14:50:38.000000 qtconsole-5.5.0/README.md
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      678 2020-10-24 15:40:21.000000 qtconsole-5.5.0/RELEASE.md
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-11-06 02:38:53.985890 qtconsole-5.5.0/docs/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     7886 2015-12-20 14:40:14.000000 qtconsole-5.5.0/docs/Makefile
--rwxrwxr-x   0 carlos    (1000) carlos    (1000)     1007 2020-10-24 15:40:21.000000 qtconsole-5.5.0/docs/autogen_config.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      161 2022-03-27 18:25:58.000000 qtconsole-5.5.0/docs/environment.yml
--rwxrwxr-x   0 carlos    (1000) carlos    (1000)     4166 2021-03-17 01:07:09.000000 qtconsole-5.5.0/docs/gh-pages.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-11-06 02:38:53.989890 qtconsole-5.5.0/docs/source/
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-11-06 02:38:53.989890 qtconsole-5.5.0/docs/source/_images/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)   153249 2015-12-20 14:40:14.000000 qtconsole-5.5.0/docs/source/_images/qtconsole.png
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    11830 2023-11-06 00:27:55.000000 qtconsole-5.5.0/docs/source/changelog.rst
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    10284 2021-03-17 01:07:09.000000 qtconsole-5.5.0/docs/source/conf.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-11-06 02:38:53.989890 qtconsole-5.5.0/docs/source/figs/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    53726 2015-12-20 14:40:14.000000 qtconsole-5.5.0/docs/source/figs/besselj.png
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    61184 2015-12-20 14:40:14.000000 qtconsole-5.5.0/docs/source/figs/colors_dark.png
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    44935 2015-12-20 14:40:14.000000 qtconsole-5.5.0/docs/source/figs/jn.html
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    29224 2015-12-20 14:40:14.000000 qtconsole-5.5.0/docs/source/figs/jn.xhtml
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    18580 2020-10-24 15:40:21.000000 qtconsole-5.5.0/docs/source/index.rst
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1184 2023-09-01 14:50:38.000000 qtconsole-5.5.0/docs/source/installation.rst
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-11-06 02:38:53.989890 qtconsole-5.5.0/examples/
--rwxrwxr-x   0 carlos    (1000) carlos    (1000)     1580 2020-10-24 15:40:21.000000 qtconsole-5.5.0/examples/embed_qtconsole.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1057 2020-10-24 15:40:21.000000 qtconsole-5.5.0/examples/inprocess_qtconsole.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      421 2020-10-24 15:40:21.000000 qtconsole-5.5.0/examples/jupyter-qtconsole.desktop
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-11-06 02:38:53.997890 qtconsole-5.5.0/qtconsole/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       48 2015-12-20 14:40:14.000000 qtconsole-5.5.0/qtconsole/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       82 2015-12-20 14:40:14.000000 qtconsole-5.5.0/qtconsole/__main__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       72 2023-11-06 02:36:11.000000 qtconsole-5.5.0/qtconsole/_version.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    14185 2021-11-14 18:48:23.000000 qtconsole-5.5.0/qtconsole/ansi_code_processor.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     6295 2021-11-14 18:48:23.000000 qtconsole-5.5.0/qtconsole/base_frontend_mixin.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3733 2021-03-17 01:07:09.000000 qtconsole-5.5.0/qtconsole/bracket_matcher.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    10683 2022-03-27 18:25:58.000000 qtconsole-5.5.0/qtconsole/call_tip_widget.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1971 2023-03-30 15:34:17.000000 qtconsole-5.5.0/qtconsole/client.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     8848 2023-10-19 14:46:51.000000 qtconsole-5.5.0/qtconsole/comms.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    12909 2023-10-19 14:46:51.000000 qtconsole-5.5.0/qtconsole/completion_html.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2234 2023-10-19 14:46:51.000000 qtconsole-5.5.0/qtconsole/completion_plain.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     8151 2022-10-29 16:58:15.000000 qtconsole-5.5.0/qtconsole/completion_widget.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)   104735 2023-11-06 00:26:20.000000 qtconsole-5.5.0/qtconsole/console_widget.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    34873 2023-10-19 14:46:51.000000 qtconsole-5.5.0/qtconsole/frontend_widget.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     9947 2021-03-17 01:07:09.000000 qtconsole-5.5.0/qtconsole/history_console_widget.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2874 2023-05-05 17:34:26.000000 qtconsole-5.5.0/qtconsole/inprocess.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      169 2020-10-24 15:40:21.000000 qtconsole-5.5.0/qtconsole/ipython_widget.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    24994 2023-11-05 23:26:17.000000 qtconsole-5.5.0/qtconsole/jupyter_widget.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1813 2021-03-17 01:07:09.000000 qtconsole-5.5.0/qtconsole/kernel_mixins.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3793 2021-03-17 01:07:09.000000 qtconsole-5.5.0/qtconsole/kill_ring.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    38402 2022-05-29 16:43:26.000000 qtconsole-5.5.0/qtconsole/mainwindow.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2602 2023-03-28 21:52:03.000000 qtconsole-5.5.0/qtconsole/manager.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     9119 2021-05-02 17:44:56.000000 qtconsole-5.5.0/qtconsole/pygments_highlighter.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      540 2021-03-17 01:07:09.000000 qtconsole-5.5.0/qtconsole/qstringhelpers.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    17229 2023-03-11 20:35:38.000000 qtconsole-5.5.0/qtconsole/qtconsoleapp.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-11-06 02:38:53.985890 qtconsole-5.5.0/qtconsole/resources/
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-11-06 02:38:54.005890 qtconsole-5.5.0/qtconsole/resources/icon/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    26397 2015-12-20 14:40:14.000000 qtconsole-5.5.0/qtconsole/resources/icon/JupyterConsole.svg
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      184 2020-10-24 15:40:21.000000 qtconsole-5.5.0/qtconsole/rich_ipython_widget.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    18478 2023-10-19 14:46:51.000000 qtconsole-5.5.0/qtconsole/rich_jupyter_widget.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     8638 2021-03-17 01:07:09.000000 qtconsole-5.5.0/qtconsole/rich_text.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3801 2020-10-24 15:40:21.000000 qtconsole-5.5.0/qtconsole/styles.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2394 2021-03-17 01:07:09.000000 qtconsole-5.5.0/qtconsole/svg.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-11-06 02:38:54.009891 qtconsole-5.5.0/qtconsole/tests/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      132 2020-10-24 15:40:22.000000 qtconsole-5.5.0/qtconsole/tests/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    26302 2023-03-28 21:52:03.000000 qtconsole-5.5.0/qtconsole/tests/test_00_console_widget.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     7430 2021-11-14 18:48:23.000000 qtconsole-5.5.0/qtconsole/tests/test_ansi_code_processor.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1003 2020-10-24 15:40:22.000000 qtconsole-5.5.0/qtconsole/tests/test_app.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     5400 2021-05-02 17:44:56.000000 qtconsole-5.5.0/qtconsole/tests/test_comms.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3343 2021-03-17 01:07:09.000000 qtconsole-5.5.0/qtconsole/tests/test_completion_widget.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3219 2020-10-24 15:40:22.000000 qtconsole-5.5.0/qtconsole/tests/test_frontend_widget.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      976 2023-05-05 17:34:26.000000 qtconsole-5.5.0/qtconsole/tests/test_inprocess_kernel.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4976 2023-03-07 00:10:49.000000 qtconsole-5.5.0/qtconsole/tests/test_jupyter_widget.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2278 2020-10-24 15:40:22.000000 qtconsole-5.5.0/qtconsole/tests/test_kill_ring.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      519 2020-10-24 15:40:22.000000 qtconsole-5.5.0/qtconsole/tests/test_styles.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     8349 2020-10-24 15:40:22.000000 qtconsole-5.5.0/qtconsole/usage.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     8363 2023-10-19 14:46:51.000000 qtconsole-5.5.0/qtconsole/util.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-11-06 02:38:54.005890 qtconsole-5.5.0/qtconsole.egg-info/
--rw-r--r--   0 carlos    (1000) carlos    (1000)     5056 2023-11-06 02:38:53.000000 qtconsole-5.5.0/qtconsole.egg-info/PKG-INFO
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2140 2023-11-06 02:38:53.000000 qtconsole-5.5.0/qtconsole.egg-info/SOURCES.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-11-06 02:38:53.000000 qtconsole-5.5.0/qtconsole.egg-info/dependency_links.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       62 2023-11-06 02:38:53.000000 qtconsole-5.5.0/qtconsole.egg-info/entry_points.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      166 2023-11-06 02:38:53.000000 qtconsole-5.5.0/qtconsole.egg-info/requires.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       10 2023-11-06 02:38:53.000000 qtconsole-5.5.0/qtconsole.egg-info/top_level.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       88 2020-10-24 15:40:22.000000 qtconsole-5.5.0/readthedocs.yml
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-11-06 02:38:54.009891 qtconsole-5.5.0/requirements/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      233 2023-10-19 14:46:51.000000 qtconsole-5.5.0/requirements/environment.yml
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       38 2023-11-06 02:38:54.009891 qtconsole-5.5.0/setup.cfg
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3306 2023-10-19 15:09:05.000000 qtconsole-5.5.0/setup.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-11-15 22:57:05.745229 qtconsole-5.5.1/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       44 2020-10-24 15:40:21.000000 qtconsole-5.5.1/.coveragerc
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-11-15 22:57:05.733228 qtconsole-5.5.1/.github/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-11-15 22:57:05.733228 qtconsole-5.5.1/.github/workflows/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2621 2023-10-19 15:09:05.000000 qtconsole-5.5.1/.github/workflows/linux-tests.yml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1347 2023-10-19 15:09:05.000000 qtconsole-5.5.1/.github/workflows/macos-tests.yml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1361 2023-10-19 15:09:05.000000 qtconsole-5.5.1/.github/workflows/windows-tests.yml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      350 2023-05-05 17:34:26.000000 qtconsole-5.5.1/.gitignore
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    10807 2015-12-20 14:40:14.000000 qtconsole-5.5.1/.mailmap
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      624 2022-03-27 18:25:58.000000 qtconsole-5.5.1/CONTRIBUTING.md
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1528 2020-10-24 15:40:21.000000 qtconsole-5.5.1/LICENSE
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      371 2020-10-24 15:40:21.000000 qtconsole-5.5.1/MANIFEST.in
+-rw-r--r--   0 carlos    (1000) carlos    (1000)     5056 2023-11-15 22:57:05.745229 qtconsole-5.5.1/PKG-INFO
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3661 2023-09-01 14:50:38.000000 qtconsole-5.5.1/README.md
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      678 2020-10-24 15:40:21.000000 qtconsole-5.5.1/RELEASE.md
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-11-15 22:57:05.737228 qtconsole-5.5.1/docs/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     7886 2015-12-20 14:40:14.000000 qtconsole-5.5.1/docs/Makefile
+-rwxrwxr-x   0 carlos    (1000) carlos    (1000)     1007 2020-10-24 15:40:21.000000 qtconsole-5.5.1/docs/autogen_config.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      161 2022-03-27 18:25:58.000000 qtconsole-5.5.1/docs/environment.yml
+-rwxrwxr-x   0 carlos    (1000) carlos    (1000)     4166 2021-03-17 01:07:09.000000 qtconsole-5.5.1/docs/gh-pages.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-11-15 22:57:05.737228 qtconsole-5.5.1/docs/source/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-11-15 22:57:05.737228 qtconsole-5.5.1/docs/source/_images/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)   153249 2015-12-20 14:40:14.000000 qtconsole-5.5.1/docs/source/_images/qtconsole.png
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    11964 2023-11-15 22:54:15.000000 qtconsole-5.5.1/docs/source/changelog.rst
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    10284 2021-03-17 01:07:09.000000 qtconsole-5.5.1/docs/source/conf.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-11-15 22:57:05.737228 qtconsole-5.5.1/docs/source/figs/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    53726 2015-12-20 14:40:14.000000 qtconsole-5.5.1/docs/source/figs/besselj.png
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    61184 2015-12-20 14:40:14.000000 qtconsole-5.5.1/docs/source/figs/colors_dark.png
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    44935 2015-12-20 14:40:14.000000 qtconsole-5.5.1/docs/source/figs/jn.html
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    29224 2015-12-20 14:40:14.000000 qtconsole-5.5.1/docs/source/figs/jn.xhtml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    18580 2020-10-24 15:40:21.000000 qtconsole-5.5.1/docs/source/index.rst
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1184 2023-09-01 14:50:38.000000 qtconsole-5.5.1/docs/source/installation.rst
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-11-15 22:57:05.737228 qtconsole-5.5.1/examples/
+-rwxrwxr-x   0 carlos    (1000) carlos    (1000)     1580 2020-10-24 15:40:21.000000 qtconsole-5.5.1/examples/embed_qtconsole.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1057 2020-10-24 15:40:21.000000 qtconsole-5.5.1/examples/inprocess_qtconsole.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      421 2020-10-24 15:40:21.000000 qtconsole-5.5.1/examples/jupyter-qtconsole.desktop
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-11-15 22:57:05.741228 qtconsole-5.5.1/qtconsole/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       48 2015-12-20 14:40:14.000000 qtconsole-5.5.1/qtconsole/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       82 2015-12-20 14:40:14.000000 qtconsole-5.5.1/qtconsole/__main__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       72 2023-11-15 22:55:30.000000 qtconsole-5.5.1/qtconsole/_version.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    14185 2021-11-14 18:48:23.000000 qtconsole-5.5.1/qtconsole/ansi_code_processor.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     6295 2021-11-14 18:48:23.000000 qtconsole-5.5.1/qtconsole/base_frontend_mixin.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3733 2021-03-17 01:07:09.000000 qtconsole-5.5.1/qtconsole/bracket_matcher.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    10683 2022-03-27 18:25:58.000000 qtconsole-5.5.1/qtconsole/call_tip_widget.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1971 2023-03-30 15:34:17.000000 qtconsole-5.5.1/qtconsole/client.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     8848 2023-10-19 14:46:51.000000 qtconsole-5.5.1/qtconsole/comms.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    12909 2023-10-19 14:46:51.000000 qtconsole-5.5.1/qtconsole/completion_html.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2234 2023-10-19 14:46:51.000000 qtconsole-5.5.1/qtconsole/completion_plain.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     8151 2022-10-29 16:58:15.000000 qtconsole-5.5.1/qtconsole/completion_widget.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)   104735 2023-11-06 00:26:20.000000 qtconsole-5.5.1/qtconsole/console_widget.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    34873 2023-10-19 14:46:51.000000 qtconsole-5.5.1/qtconsole/frontend_widget.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     9947 2021-03-17 01:07:09.000000 qtconsole-5.5.1/qtconsole/history_console_widget.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2874 2023-05-05 17:34:26.000000 qtconsole-5.5.1/qtconsole/inprocess.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      169 2020-10-24 15:40:21.000000 qtconsole-5.5.1/qtconsole/ipython_widget.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    24994 2023-11-05 23:26:17.000000 qtconsole-5.5.1/qtconsole/jupyter_widget.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1813 2021-03-17 01:07:09.000000 qtconsole-5.5.1/qtconsole/kernel_mixins.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3793 2021-03-17 01:07:09.000000 qtconsole-5.5.1/qtconsole/kill_ring.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    38402 2022-05-29 16:43:26.000000 qtconsole-5.5.1/qtconsole/mainwindow.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2602 2023-03-28 21:52:03.000000 qtconsole-5.5.1/qtconsole/manager.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     9119 2021-05-02 17:44:56.000000 qtconsole-5.5.1/qtconsole/pygments_highlighter.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      540 2021-03-17 01:07:09.000000 qtconsole-5.5.1/qtconsole/qstringhelpers.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    17229 2023-03-11 20:35:38.000000 qtconsole-5.5.1/qtconsole/qtconsoleapp.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-11-15 22:57:05.733228 qtconsole-5.5.1/qtconsole/resources/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-11-15 22:57:05.741228 qtconsole-5.5.1/qtconsole/resources/icon/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    26397 2015-12-20 14:40:14.000000 qtconsole-5.5.1/qtconsole/resources/icon/JupyterConsole.svg
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      184 2020-10-24 15:40:21.000000 qtconsole-5.5.1/qtconsole/rich_ipython_widget.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    18478 2023-10-19 14:46:51.000000 qtconsole-5.5.1/qtconsole/rich_jupyter_widget.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     8638 2021-03-17 01:07:09.000000 qtconsole-5.5.1/qtconsole/rich_text.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3801 2020-10-24 15:40:21.000000 qtconsole-5.5.1/qtconsole/styles.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2394 2021-03-17 01:07:09.000000 qtconsole-5.5.1/qtconsole/svg.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-11-15 22:57:05.745229 qtconsole-5.5.1/qtconsole/tests/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      132 2020-10-24 15:40:22.000000 qtconsole-5.5.1/qtconsole/tests/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    26302 2023-03-28 21:52:03.000000 qtconsole-5.5.1/qtconsole/tests/test_00_console_widget.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     7430 2021-11-14 18:48:23.000000 qtconsole-5.5.1/qtconsole/tests/test_ansi_code_processor.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1003 2020-10-24 15:40:22.000000 qtconsole-5.5.1/qtconsole/tests/test_app.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     5400 2021-05-02 17:44:56.000000 qtconsole-5.5.1/qtconsole/tests/test_comms.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3343 2021-03-17 01:07:09.000000 qtconsole-5.5.1/qtconsole/tests/test_completion_widget.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3219 2020-10-24 15:40:22.000000 qtconsole-5.5.1/qtconsole/tests/test_frontend_widget.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      976 2023-05-05 17:34:26.000000 qtconsole-5.5.1/qtconsole/tests/test_inprocess_kernel.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4976 2023-03-07 00:10:49.000000 qtconsole-5.5.1/qtconsole/tests/test_jupyter_widget.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2278 2020-10-24 15:40:22.000000 qtconsole-5.5.1/qtconsole/tests/test_kill_ring.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      519 2020-10-24 15:40:22.000000 qtconsole-5.5.1/qtconsole/tests/test_styles.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     8349 2020-10-24 15:40:22.000000 qtconsole-5.5.1/qtconsole/usage.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     8354 2023-11-15 22:45:47.000000 qtconsole-5.5.1/qtconsole/util.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-11-15 22:57:05.741228 qtconsole-5.5.1/qtconsole.egg-info/
+-rw-r--r--   0 carlos    (1000) carlos    (1000)     5056 2023-11-15 22:57:05.000000 qtconsole-5.5.1/qtconsole.egg-info/PKG-INFO
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2140 2023-11-15 22:57:05.000000 qtconsole-5.5.1/qtconsole.egg-info/SOURCES.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-11-15 22:57:05.000000 qtconsole-5.5.1/qtconsole.egg-info/dependency_links.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       62 2023-11-15 22:57:05.000000 qtconsole-5.5.1/qtconsole.egg-info/entry_points.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      166 2023-11-15 22:57:05.000000 qtconsole-5.5.1/qtconsole.egg-info/requires.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       10 2023-11-15 22:57:05.000000 qtconsole-5.5.1/qtconsole.egg-info/top_level.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       88 2020-10-24 15:40:22.000000 qtconsole-5.5.1/readthedocs.yml
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-11-15 22:57:05.745229 qtconsole-5.5.1/requirements/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      233 2023-10-19 14:46:51.000000 qtconsole-5.5.1/requirements/environment.yml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       38 2023-11-15 22:57:05.745229 qtconsole-5.5.1/setup.cfg
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3306 2023-10-19 15:09:05.000000 qtconsole-5.5.1/setup.py
```

### Comparing `qtconsole-5.5.0/.github/workflows/linux-tests.yml` & `qtconsole-5.5.1/.github/workflows/linux-tests.yml`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/.github/workflows/macos-tests.yml` & `qtconsole-5.5.1/.github/workflows/macos-tests.yml`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/.github/workflows/windows-tests.yml` & `qtconsole-5.5.1/.github/workflows/windows-tests.yml`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/.mailmap` & `qtconsole-5.5.1/.mailmap`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/CONTRIBUTING.md` & `qtconsole-5.5.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/LICENSE` & `qtconsole-5.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/PKG-INFO` & `qtconsole-5.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtconsole
-Version: 5.5.0
+Version: 5.5.1
 Summary: Jupyter Qt console
 Home-page: http://jupyter.org
 Author: Jupyter Development Team
 Author-email: jupyter@googlegroups.com
 Maintainer: Spyder Development Team
 License: BSD
 Keywords: Interactive,Interpreter,Shell
```

### Comparing `qtconsole-5.5.0/README.md` & `qtconsole-5.5.1/README.md`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/RELEASE.md` & `qtconsole-5.5.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/docs/Makefile` & `qtconsole-5.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/docs/autogen_config.py` & `qtconsole-5.5.1/docs/autogen_config.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/docs/gh-pages.py` & `qtconsole-5.5.1/docs/gh-pages.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/docs/source/_images/qtconsole.png` & `qtconsole-5.5.1/docs/source/_images/qtconsole.png`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/docs/source/changelog.rst` & `qtconsole-5.5.1/docs/source/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 =============================
 
 .. _5.5:
 
 5.5
 ~~~
 
+5.5.1
+-----
+
+`5.5.1 on GitHub <https://github.com/jupyter/qtconsole/milestones/5.5.1>`__
+
+* Fix error when getting code completions.
+
 5.5.0
 -----
 
 `5.5.0 on GitHub <https://github.com/jupyter/qtconsole/milestones/5.5.0>`__
 
 Changes
 +++++++
```

### Comparing `qtconsole-5.5.0/docs/source/conf.py` & `qtconsole-5.5.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/docs/source/figs/besselj.png` & `qtconsole-5.5.1/docs/source/figs/besselj.png`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/docs/source/figs/colors_dark.png` & `qtconsole-5.5.1/docs/source/figs/colors_dark.png`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/docs/source/figs/jn.html` & `qtconsole-5.5.1/docs/source/figs/jn.html`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/docs/source/figs/jn.xhtml` & `qtconsole-5.5.1/docs/source/figs/jn.xhtml`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/docs/source/index.rst` & `qtconsole-5.5.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/docs/source/installation.rst` & `qtconsole-5.5.1/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/examples/embed_qtconsole.py` & `qtconsole-5.5.1/examples/embed_qtconsole.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/examples/inprocess_qtconsole.py` & `qtconsole-5.5.1/examples/inprocess_qtconsole.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/ansi_code_processor.py` & `qtconsole-5.5.1/qtconsole/ansi_code_processor.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/base_frontend_mixin.py` & `qtconsole-5.5.1/qtconsole/base_frontend_mixin.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/bracket_matcher.py` & `qtconsole-5.5.1/qtconsole/bracket_matcher.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/call_tip_widget.py` & `qtconsole-5.5.1/qtconsole/call_tip_widget.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/client.py` & `qtconsole-5.5.1/qtconsole/client.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/comms.py` & `qtconsole-5.5.1/qtconsole/comms.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/completion_html.py` & `qtconsole-5.5.1/qtconsole/completion_html.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/completion_plain.py` & `qtconsole-5.5.1/qtconsole/completion_plain.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/completion_widget.py` & `qtconsole-5.5.1/qtconsole/completion_widget.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/console_widget.py` & `qtconsole-5.5.1/qtconsole/console_widget.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/frontend_widget.py` & `qtconsole-5.5.1/qtconsole/frontend_widget.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/history_console_widget.py` & `qtconsole-5.5.1/qtconsole/history_console_widget.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/inprocess.py` & `qtconsole-5.5.1/qtconsole/inprocess.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/jupyter_widget.py` & `qtconsole-5.5.1/qtconsole/jupyter_widget.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/kernel_mixins.py` & `qtconsole-5.5.1/qtconsole/kernel_mixins.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/kill_ring.py` & `qtconsole-5.5.1/qtconsole/kill_ring.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/mainwindow.py` & `qtconsole-5.5.1/qtconsole/mainwindow.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/manager.py` & `qtconsole-5.5.1/qtconsole/manager.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/pygments_highlighter.py` & `qtconsole-5.5.1/qtconsole/pygments_highlighter.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/qstringhelpers.py` & `qtconsole-5.5.1/qtconsole/qstringhelpers.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/qtconsoleapp.py` & `qtconsole-5.5.1/qtconsole/qtconsoleapp.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/resources/icon/JupyterConsole.svg` & `qtconsole-5.5.1/qtconsole/resources/icon/JupyterConsole.svg`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/rich_jupyter_widget.py` & `qtconsole-5.5.1/qtconsole/rich_jupyter_widget.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/rich_text.py` & `qtconsole-5.5.1/qtconsole/rich_text.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/styles.py` & `qtconsole-5.5.1/qtconsole/styles.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/svg.py` & `qtconsole-5.5.1/qtconsole/svg.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/tests/test_00_console_widget.py` & `qtconsole-5.5.1/qtconsole/tests/test_00_console_widget.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/tests/test_ansi_code_processor.py` & `qtconsole-5.5.1/qtconsole/tests/test_ansi_code_processor.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/tests/test_app.py` & `qtconsole-5.5.1/qtconsole/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/tests/test_comms.py` & `qtconsole-5.5.1/qtconsole/tests/test_comms.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/tests/test_completion_widget.py` & `qtconsole-5.5.1/qtconsole/tests/test_completion_widget.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/tests/test_frontend_widget.py` & `qtconsole-5.5.1/qtconsole/tests/test_frontend_widget.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/tests/test_inprocess_kernel.py` & `qtconsole-5.5.1/qtconsole/tests/test_inprocess_kernel.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/tests/test_jupyter_widget.py` & `qtconsole-5.5.1/qtconsole/tests/test_jupyter_widget.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/tests/test_kill_ring.py` & `qtconsole-5.5.1/qtconsole/tests/test_kill_ring.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/tests/test_styles.py` & `qtconsole-5.5.1/qtconsole/tests/test_styles.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/usage.py` & `qtconsole-5.5.1/qtconsole/usage.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/qtconsole/util.py` & `qtconsole-5.5.1/qtconsole/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
     """return list item number, or default if don't exist"""
     if i >= len(mylist):
         return default
     else:
         return mylist[i]
 
 
-def compute_item_matrix(items, empty=None, *, separator_size=2, displaywith=80):
+def compute_item_matrix(items, empty=None, *, separator_size=2, displaywidth=80):
     """Returns a nested list, and info to columnize items
 
     Parameters
     ----------
     items
         list of strings to columnize
     empty : (default None)
@@ -200,28 +200,26 @@
             [_get_or_default(items, c * nrow + i, default=empty) for c in range(ncol)]
             for i in range(nrow)
         ],
         info,
     )
 
 
-def columnize(items):
+def columnize(items, separator="  ", displaywidth=80):
     """Transform a list of strings into a single string with columns.
 
     Parameters
     ----------
     items : sequence of strings
         The strings to process.
 
     Returns
     -------
     The formatted string.
     """
-    separator = "  "
-    displaywidth = 80
     if not items:
         return "\n"
     matrix, info = compute_item_matrix(
         items, separator_size=len(separator), displaywidth=displaywidth
     )
     fmatrix = [filter(None, x) for x in matrix]
     sjoin = lambda x: separator.join(
```

### Comparing `qtconsole-5.5.0/qtconsole.egg-info/PKG-INFO` & `qtconsole-5.5.1/qtconsole.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtconsole
-Version: 5.5.0
+Version: 5.5.1
 Summary: Jupyter Qt console
 Home-page: http://jupyter.org
 Author: Jupyter Development Team
 Author-email: jupyter@googlegroups.com
 Maintainer: Spyder Development Team
 License: BSD
 Keywords: Interactive,Interpreter,Shell
```

### Comparing `qtconsole-5.5.0/qtconsole.egg-info/SOURCES.txt` & `qtconsole-5.5.1/qtconsole.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qtconsole-5.5.0/setup.py` & `qtconsole-5.5.1/setup.py`

 * *Files identical despite different names*

