# Comparing `tmp/moulti-1.7.0.tar.gz` & `tmp/moulti-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moulti-1.7.0.tar", last modified: Sun Apr 28 13:17:18 2024, max compression
+gzip compressed data, was "moulti-1.8.0.tar", last modified: Sun May  5 16:13:18 2024, max compression
```

## Comparing `moulti-1.7.0.tar` & `moulti-1.8.0.tar`

### file list

```diff
@@ -1,62 +1,67 @@
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-28 13:17:18.692666 moulti-1.7.0/
--rw-r--r--   0 xavier    (1000) xavier    (1000)     1066 2024-02-16 15:24:09.000000 moulti-1.7.0/LICENSE
--rw-r--r--   0 xavier    (1000) xavier    (1000)     4347 2024-04-28 13:17:18.692666 moulti-1.7.0/PKG-INFO
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     3358 2024-04-20 17:36:22.000000 moulti-1.7.0/README.md
--rw-r--r--   0 xavier    (1000) xavier    (1000)      627 2024-03-01 22:04:07.000000 moulti-1.7.0/pyproject.toml
--rw-rw-r--   0 xavier    (1000) xavier    (1000)       38 2024-04-28 13:17:18.692666 moulti-1.7.0/setup.cfg
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1605 2024-04-28 13:14:18.000000 moulti-1.7.0/setup.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-28 13:17:18.688666 moulti-1.7.0/src/
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-28 13:17:18.688666 moulti-1.7.0/src/moulti/
--rw-r--r--   0 xavier    (1000) xavier    (1000)       76 2024-04-28 13:14:28.000000 moulti-1.7.0/src/moulti/__init__.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)       29 2024-02-26 18:39:57.000000 moulti-1.7.0/src/moulti/__main__.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     7781 2024-03-10 14:34:42.000000 moulti-1.7.0/src/moulti/ansi.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    25720 2024-04-28 13:13:58.000000 moulti-1.7.0/src/moulti/app.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     2841 2024-04-20 13:43:17.000000 moulti-1.7.0/src/moulti/askpass.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     7826 2024-04-24 21:40:25.000000 moulti-1.7.0/src/moulti/cli.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1213 2024-04-18 01:55:09.000000 moulti-1.7.0/src/moulti/helpers.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)      820 2024-03-08 01:07:28.000000 moulti-1.7.0/src/moulti/precli.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    11647 2024-03-31 10:37:10.000000 moulti-1.7.0/src/moulti/protocol.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-28 13:17:18.692666 moulti-1.7.0/src/moulti/widgets/
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      177 2024-04-23 20:39:30.000000 moulti-1.7.0/src/moulti/widgets/__init__.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-28 13:17:18.692666 moulti-1.7.0/src/moulti/widgets/abstractquestion/
--rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-15 22:08:32.000000 moulti-1.7.0/src/moulti/widgets/abstractquestion/__init__.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)      609 2024-04-23 18:32:39.000000 moulti-1.7.0/src/moulti/widgets/abstractquestion/cli.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     2794 2024-04-23 17:32:01.000000 moulti-1.7.0/src/moulti/widgets/abstractquestion/tui.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-28 13:17:18.692666 moulti-1.7.0/src/moulti/widgets/abstractstep/
--rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-15 22:08:39.000000 moulti-1.7.0/src/moulti/widgets/abstractstep/__init__.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      699 2024-04-23 18:32:38.000000 moulti-1.7.0/src/moulti/widgets/abstractstep/cli.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     4594 2024-04-23 21:17:23.000000 moulti-1.7.0/src/moulti/widgets/abstractstep/tui.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-28 13:17:18.692666 moulti-1.7.0/src/moulti/widgets/buttonquestion/
--rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-16 17:31:52.000000 moulti-1.7.0/src/moulti/widgets/buttonquestion/__init__.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     2347 2024-02-17 01:04:31.000000 moulti-1.7.0/src/moulti/widgets/buttonquestion/cli.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     6868 2024-03-17 03:27:04.000000 moulti-1.7.0/src/moulti/widgets/buttonquestion/tui.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)      408 2024-02-16 19:52:22.000000 moulti-1.7.0/src/moulti/widgets/cli.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-28 13:17:18.692666 moulti-1.7.0/src/moulti/widgets/collapsiblestep/
--rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-04-23 17:16:59.000000 moulti-1.7.0/src/moulti/widgets/collapsiblestep/__init__.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      749 2024-04-23 18:32:37.000000 moulti-1.7.0/src/moulti/widgets/collapsiblestep/cli.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     2805 2024-04-24 21:39:15.000000 moulti-1.7.0/src/moulti/widgets/collapsiblestep/tui.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-28 13:17:18.692666 moulti-1.7.0/src/moulti/widgets/divider/
--rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-04-23 20:39:30.000000 moulti-1.7.0/src/moulti/widgets/divider/__init__.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     1614 2024-04-23 20:39:30.000000 moulti-1.7.0/src/moulti/widgets/divider/cli.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      813 2024-04-24 21:40:25.000000 moulti-1.7.0/src/moulti/widgets/divider/tui.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-28 13:17:18.692666 moulti-1.7.0/src/moulti/widgets/inputquestion/
--rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-16 17:31:52.000000 moulti-1.7.0/src/moulti/widgets/inputquestion/__init__.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     2897 2024-02-17 01:06:38.000000 moulti-1.7.0/src/moulti/widgets/inputquestion/cli.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     2197 2024-04-23 21:17:23.000000 moulti-1.7.0/src/moulti/widgets/inputquestion/tui.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     4431 2024-03-10 13:06:07.000000 moulti-1.7.0/src/moulti/widgets/moulticonsole.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     3865 2024-03-09 04:48:36.000000 moulti-1.7.0/src/moulti/widgets/moultilog.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     2288 2024-02-21 01:21:22.000000 moulti-1.7.0/src/moulti/widgets/quitdialog.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-28 13:17:18.692666 moulti-1.7.0/src/moulti/widgets/step/
--rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-16 17:31:46.000000 moulti-1.7.0/src/moulti/widgets/step/__init__.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     4550 2024-04-23 20:13:13.000000 moulti-1.7.0/src/moulti/widgets/step/cli.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     7353 2024-04-28 00:47:55.000000 moulti-1.7.0/src/moulti/widgets/step/tui.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     2854 2024-04-18 01:55:09.000000 moulti-1.7.0/src/moulti/widgets/stepcontainer.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     1786 2024-02-21 22:35:11.000000 moulti-1.7.0/src/moulti/widgets/tui.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)      356 2024-04-10 22:30:03.000000 moulti-1.7.0/src/moulti/widgets/vertscroll.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-28 13:17:18.692666 moulti-1.7.0/src/moulti.egg-info/
--rw-r--r--   0 xavier    (1000) xavier    (1000)     4347 2024-04-28 13:17:18.000000 moulti-1.7.0/src/moulti.egg-info/PKG-INFO
--rw-r--r--   0 xavier    (1000) xavier    (1000)     1534 2024-04-28 13:17:18.000000 moulti-1.7.0/src/moulti.egg-info/SOURCES.txt
--rw-r--r--   0 xavier    (1000) xavier    (1000)        1 2024-04-28 13:17:18.000000 moulti-1.7.0/src/moulti.egg-info/dependency_links.txt
--rw-r--r--   0 xavier    (1000) xavier    (1000)       83 2024-04-28 13:17:18.000000 moulti-1.7.0/src/moulti.egg-info/entry_points.txt
--rw-r--r--   0 xavier    (1000) xavier    (1000)       36 2024-04-28 13:17:18.000000 moulti-1.7.0/src/moulti.egg-info/requires.txt
--rw-r--r--   0 xavier    (1000) xavier    (1000)        7 2024-04-28 13:17:18.000000 moulti-1.7.0/src/moulti.egg-info/top_level.txt
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-05 16:13:18.109601 moulti-1.8.0/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     1066 2024-02-16 15:24:09.000000 moulti-1.8.0/LICENSE
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     4894 2024-05-05 16:13:18.109601 moulti-1.8.0/PKG-INFO
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     3869 2024-05-05 16:06:31.000000 moulti-1.8.0/README.md
+-rw-r--r--   0 xavier    (1000) xavier    (1000)      627 2024-03-01 22:04:07.000000 moulti-1.8.0/pyproject.toml
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)       38 2024-05-05 16:13:18.109601 moulti-1.8.0/setup.cfg
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1655 2024-05-05 16:10:38.000000 moulti-1.8.0/setup.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-05 16:13:18.101601 moulti-1.8.0/src/
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-05 16:13:18.105601 moulti-1.8.0/src/moulti/
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)       76 2024-05-05 16:10:41.000000 moulti-1.8.0/src/moulti/__init__.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)       29 2024-02-26 18:39:57.000000 moulti-1.8.0/src/moulti/__main__.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     7781 2024-03-10 14:34:42.000000 moulti-1.8.0/src/moulti/ansi.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-05 16:13:18.105601 moulti-1.8.0/src/moulti/ansible/
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)        0 2024-04-28 14:10:17.000000 moulti-1.8.0/src/moulti/ansible/__init__.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     7153 2024-05-01 20:47:59.000000 moulti-1.8.0/src/moulti/ansible/moulti.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    26354 2024-05-03 01:53:49.000000 moulti-1.8.0/src/moulti/app.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     2841 2024-04-20 13:43:17.000000 moulti-1.8.0/src/moulti/askpass.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     7235 2024-05-04 21:16:30.000000 moulti-1.8.0/src/moulti/cli.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     3856 2024-05-04 21:51:51.000000 moulti-1.8.0/src/moulti/diff.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1213 2024-04-18 01:55:09.000000 moulti-1.8.0/src/moulti/helpers.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1798 2024-05-02 17:34:34.000000 moulti-1.8.0/src/moulti/pipeline.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)      820 2024-03-08 01:07:28.000000 moulti-1.8.0/src/moulti/precli.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    11647 2024-03-31 10:37:10.000000 moulti-1.8.0/src/moulti/protocol.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-05 16:13:18.105601 moulti-1.8.0/src/moulti/widgets/
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      177 2024-04-23 20:39:30.000000 moulti-1.8.0/src/moulti/widgets/__init__.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-05 16:13:18.105601 moulti-1.8.0/src/moulti/widgets/abstractquestion/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-15 22:08:32.000000 moulti-1.8.0/src/moulti/widgets/abstractquestion/__init__.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)      609 2024-04-23 18:32:39.000000 moulti-1.8.0/src/moulti/widgets/abstractquestion/cli.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     2794 2024-04-23 17:32:01.000000 moulti-1.8.0/src/moulti/widgets/abstractquestion/tui.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-05 16:13:18.109601 moulti-1.8.0/src/moulti/widgets/abstractstep/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-15 22:08:39.000000 moulti-1.8.0/src/moulti/widgets/abstractstep/__init__.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      699 2024-04-23 18:32:38.000000 moulti-1.8.0/src/moulti/widgets/abstractstep/cli.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     4594 2024-04-23 21:17:23.000000 moulti-1.8.0/src/moulti/widgets/abstractstep/tui.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-05 16:13:18.109601 moulti-1.8.0/src/moulti/widgets/buttonquestion/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-16 17:31:52.000000 moulti-1.8.0/src/moulti/widgets/buttonquestion/__init__.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     2347 2024-02-17 01:04:31.000000 moulti-1.8.0/src/moulti/widgets/buttonquestion/cli.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     6868 2024-03-17 03:27:04.000000 moulti-1.8.0/src/moulti/widgets/buttonquestion/tui.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)      408 2024-02-16 19:52:22.000000 moulti-1.8.0/src/moulti/widgets/cli.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-05 16:13:18.109601 moulti-1.8.0/src/moulti/widgets/collapsiblestep/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-04-23 17:16:59.000000 moulti-1.8.0/src/moulti/widgets/collapsiblestep/__init__.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      749 2024-04-23 18:32:37.000000 moulti-1.8.0/src/moulti/widgets/collapsiblestep/cli.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     2805 2024-04-24 21:39:15.000000 moulti-1.8.0/src/moulti/widgets/collapsiblestep/tui.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-05 16:13:18.109601 moulti-1.8.0/src/moulti/widgets/divider/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-04-23 20:39:30.000000 moulti-1.8.0/src/moulti/widgets/divider/__init__.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     1614 2024-04-23 20:39:30.000000 moulti-1.8.0/src/moulti/widgets/divider/cli.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      813 2024-04-24 21:40:25.000000 moulti-1.8.0/src/moulti/widgets/divider/tui.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-05 16:13:18.109601 moulti-1.8.0/src/moulti/widgets/inputquestion/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-16 17:31:52.000000 moulti-1.8.0/src/moulti/widgets/inputquestion/__init__.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     2897 2024-02-17 01:06:38.000000 moulti-1.8.0/src/moulti/widgets/inputquestion/cli.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     2197 2024-04-23 21:17:23.000000 moulti-1.8.0/src/moulti/widgets/inputquestion/tui.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     4431 2024-03-10 13:06:07.000000 moulti-1.8.0/src/moulti/widgets/moulticonsole.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     3865 2024-03-09 04:48:36.000000 moulti-1.8.0/src/moulti/widgets/moultilog.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     2288 2024-02-21 01:21:22.000000 moulti-1.8.0/src/moulti/widgets/quitdialog.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-05 16:13:18.109601 moulti-1.8.0/src/moulti/widgets/step/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-16 17:31:46.000000 moulti-1.8.0/src/moulti/widgets/step/__init__.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     4550 2024-04-23 20:13:13.000000 moulti-1.8.0/src/moulti/widgets/step/cli.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     7353 2024-04-28 00:47:55.000000 moulti-1.8.0/src/moulti/widgets/step/tui.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     2854 2024-04-18 01:55:09.000000 moulti-1.8.0/src/moulti/widgets/stepcontainer.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     1786 2024-02-21 22:35:11.000000 moulti-1.8.0/src/moulti/widgets/tui.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)      356 2024-04-10 22:30:03.000000 moulti-1.8.0/src/moulti/widgets/vertscroll.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-05 16:13:18.109601 moulti-1.8.0/src/moulti.egg-info/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     4894 2024-05-05 16:13:18.000000 moulti-1.8.0/src/moulti.egg-info/PKG-INFO
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     1636 2024-05-05 16:13:18.000000 moulti-1.8.0/src/moulti.egg-info/SOURCES.txt
+-rw-r--r--   0 xavier    (1000) xavier    (1000)        1 2024-05-05 16:13:18.000000 moulti-1.8.0/src/moulti.egg-info/dependency_links.txt
+-rw-r--r--   0 xavier    (1000) xavier    (1000)       83 2024-05-05 16:13:18.000000 moulti-1.8.0/src/moulti.egg-info/entry_points.txt
+-rw-r--r--   0 xavier    (1000) xavier    (1000)       44 2024-05-05 16:13:18.000000 moulti-1.8.0/src/moulti.egg-info/requires.txt
+-rw-r--r--   0 xavier    (1000) xavier    (1000)        7 2024-05-05 16:13:18.000000 moulti-1.8.0/src/moulti.egg-info/top_level.txt
```

### Comparing `moulti-1.7.0/LICENSE` & `moulti-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `moulti-1.7.0/PKG-INFO` & `moulti-1.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,54 @@
 Metadata-Version: 2.1
 Name: moulti
-Version: 1.7.0
+Version: 1.8.0
 Summary: Moulti is a CLI-driven Terminal User Interface (TUI) that enables you to assign the numerous lines emitted by your scripts to visual, collapsible blocks called steps.
 Home-page: https://github.com/xavierog/moulti
 Author: Xavier G.
 Author-email: xavier.moulti@kindwolf.org
 License: MIT
-Keywords: cli,tui,curses,terminal,multiplex,script,output,steps,textual,collapsible
+Keywords: cli,tui,curses,terminal,multiplex,script,output,steps,textual,collapsible,ansible,diff
 Classifier: Environment :: Console :: Curses
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: System :: Logging
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: textual>=0.53
 Requires-Dist: pyperclip
 Requires-Dist: argcomplete
+Requires-Dist: unidiff
 
 # MOULTI
 
 Moulti changes the way your shell scripts (bash, zsh, etc.) display their output in your terminal.
 Moulti enables you to assign the numerous lines emitted by your scripts to "steps", i.e. visual, collapsible blocks featuring their own title and color.
 
 Here is how [upgrading a Debian system](examples/upgrade-system.bash) looks like with Moulti:
 
 ![Moulti demo: Debian upgrade (Animated PNG)](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-demo-debian-upgrade.png?20240218)
 
 Interested? [Run this demo in a container using docker or podman](https://hub.docker.com/r/xavierong/moulti-demo)
 
-Moulti is a tool meant for people who write and execute shell scripts.
+Not convinced yet? What if the output of your Ansible playbooks looked like this?
+
+![Moulti: Ansible playbook output](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-ansible.png?20240505)
+
+Moulti is a tool meant for people who write and execute shell scripts and/or Ansible playbooks.
 Specifically, if you find yourself scrolling up your terminal to ensure everything went fine while your script is still running, then Moulti is made for you.
 
+By the way, Moulti can also display unified diff files:
+
+![Moulti: unified diff output](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-diff.png?20240505)
+
 ## How?
 
 Synopsis:
 
 1. Start a Moulti instance: `moulti init`
 2. Add a step: `moulti step add step_name --title='some clever title here'`
 3. Fill it: `whatever_your_script_does | moulti pass step_name`
@@ -55,14 +64,15 @@
 
 ![Moulti button question](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-button-question.png?20240218)
 
 Moulti also features:
 - a **progress bar**: [documentation](Documentation.md#progress-bar)
 - programmatic scrolling: [documentation](Documentation.md#programmatically-scrolling-through-steps)
 - an askpass helper named `moulti-askpass`: [documentation](Documentation.md#moulti-run-dealing-with-ssh)
+- support for [Ansible playbooks](Documentation.md#moulti-run-dealing-with-ansible) and [unified diff](Documentation.md#moulti-diff)
 
 When it comes to look and feel, Moulti can be customised:
 
 - through `moulti set`: define whether Moulti steps flow up or down: [documentation](Documentation.md#multiple-ways-to-display-steps)
 - through [Textual CSS (TCSS)](https://textual.textualize.io/guide/CSS/): [documentation](Documentation.md#how-to-define-my-own-step-classes-)
 - through ANSI themes: [documentation](Documentation.md#appearance-look-and-feel)
```

### Comparing `moulti-1.7.0/README.md` & `moulti-1.8.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -5,17 +5,25 @@
 
 Here is how [upgrading a Debian system](examples/upgrade-system.bash) looks like with Moulti:
 
 ![Moulti demo: Debian upgrade (Animated PNG)](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-demo-debian-upgrade.png?20240218)
 
 Interested? [Run this demo in a container using docker or podman](https://hub.docker.com/r/xavierong/moulti-demo)
 
-Moulti is a tool meant for people who write and execute shell scripts.
+Not convinced yet? What if the output of your Ansible playbooks looked like this?
+
+![Moulti: Ansible playbook output](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-ansible.png?20240505)
+
+Moulti is a tool meant for people who write and execute shell scripts and/or Ansible playbooks.
 Specifically, if you find yourself scrolling up your terminal to ensure everything went fine while your script is still running, then Moulti is made for you.
 
+By the way, Moulti can also display unified diff files:
+
+![Moulti: unified diff output](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-diff.png?20240505)
+
 ## How?
 
 Synopsis:
 
 1. Start a Moulti instance: `moulti init`
 2. Add a step: `moulti step add step_name --title='some clever title here'`
 3. Fill it: `whatever_your_script_does | moulti pass step_name`
@@ -31,14 +39,15 @@
 
 ![Moulti button question](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-button-question.png?20240218)
 
 Moulti also features:
 - a **progress bar**: [documentation](Documentation.md#progress-bar)
 - programmatic scrolling: [documentation](Documentation.md#programmatically-scrolling-through-steps)
 - an askpass helper named `moulti-askpass`: [documentation](Documentation.md#moulti-run-dealing-with-ssh)
+- support for [Ansible playbooks](Documentation.md#moulti-run-dealing-with-ansible) and [unified diff](Documentation.md#moulti-diff)
 
 When it comes to look and feel, Moulti can be customised:
 
 - through `moulti set`: define whether Moulti steps flow up or down: [documentation](Documentation.md#multiple-ways-to-display-steps)
 - through [Textual CSS (TCSS)](https://textual.textualize.io/guide/CSS/): [documentation](Documentation.md#how-to-define-my-own-step-classes-)
 - through ANSI themes: [documentation](Documentation.md#appearance-look-and-feel)
```

### Comparing `moulti-1.7.0/pyproject.toml` & `moulti-1.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `moulti-1.7.0/setup.py` & `moulti-1.8.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,24 @@
 short_description += 'lines emitted by your scripts to visual, collapsible blocks called steps.'
 
 with open('README.md', 'r') as readme:
 	long_description = readme.read()
 
 setup(
 	name='moulti',
-	version='1.7.0',
+	version='1.8.0',
 	description=short_description,
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	author='Xavier G.',
 	author_email='xavier.moulti@kindwolf.org',
 	url='https://github.com/xavierog/moulti',
 	packages=[
 		'moulti',
+		'moulti.ansible',
 		'moulti.widgets',
 		'moulti.widgets.abstractstep',
 		'moulti.widgets.divider',
 		'moulti.widgets.collapsiblestep',
 		'moulti.widgets.step',
 		'moulti.widgets.abstractquestion',
 		'moulti.widgets.buttonquestion',
@@ -36,17 +37,17 @@
 		'Operating System :: POSIX :: Linux',
 		'Operating System :: MacOS :: MacOS X',
 		'Programming Language :: Python :: 3 :: Only',
 		'Topic :: System :: Logging',
 		'Topic :: Utilities',
 	],
 	license='MIT',
-	keywords=['cli', 'tui', 'curses', 'terminal', 'multiplex', 'script', 'output', 'steps', 'textual', 'collapsible'],
+	keywords=['cli', 'tui', 'curses', 'terminal', 'multiplex', 'script', 'output', 'steps', 'textual', 'collapsible', 'ansible', 'diff'],
 	package_dir={'': 'src'},
-	install_requires=['textual>=0.53', 'pyperclip', 'argcomplete'],
+	install_requires=['textual>=0.53', 'pyperclip', 'argcomplete', 'unidiff'],
 	entry_points={
 		'console_scripts': [
 			'moulti = moulti.precli:main',
 			'moulti-askpass = moulti.askpass:main',
 		]
 	},
 )
```

### Comparing `moulti-1.7.0/src/moulti/ansi.py` & `moulti-1.8.0/src/moulti/ansi.py`

 * *Files identical despite different names*

### Comparing `moulti-1.7.0/src/moulti/app.py` & `moulti-1.8.0/src/moulti/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,17 +39,21 @@
 def timestamp() -> str:
 	timestamp_ns = time_ns()
 	timestamp_s = timestamp_ns//10**9
 	ns = timestamp_ns - timestamp_s * 10**9
 	ms = ns // 10**6
 	timestr = strftime('%FT%T', localtime(timestamp_s))
 	timestr = f'{timestr}.{ms:03d} '
+
 	return timestr
 
-def run_environment(_command: list[str], copy: bool = True) -> dict[str, str]:
+def is_ansible(command: list[str]) -> bool:
+	return bool(len(command)) and 'ansible' in command[0]
+
+def run_environment(command: list[str], copy: bool = True) -> dict[str, str]:
 	"""
 	Return environment variables set by "Moulti run <command>".
 	"""
 	environment = os.environ.copy() if copy else {}
 
 	environment['MOULTI_RUN'] = 'moulti'
 	environment['MOULTI_SOCKET_PATH'] = PRINTABLE_MOULTI_SOCKET
@@ -60,14 +64,23 @@
 		environment['SSH_ASKPASS_REQUIRE'] = 'force'
 
 	if 'SUDO_ASKPASS' not in os.environ:
 		# sudo requires an absolute path:
 		if moulti_askpass_abspath := which('moulti-askpass'):
 			environment['SUDO_ASKPASS'] = moulti_askpass_abspath
 
+	if (ansible_policy := os.environ.get('MOULTI_ANSIBLE', 'default')) != 'no':
+		if ansible_policy == 'force' or (is_ansible(command) and 'ANSIBLE_STDOUT_CALLBACK' not in os.environ):
+			from . import ansible # pylint: disable=import-outside-toplevel
+			if ansible_callback_paths := os.environ.get('ANSIBLE_CALLBACK_PLUGINS', ''):
+				ansible_callback_paths += ':'
+			ansible_callback_paths += ansible.__path__[0]
+			environment['ANSIBLE_CALLBACK_PLUGINS'] = ansible_callback_paths
+			environment['ANSIBLE_STDOUT_CALLBACK'] = 'moulti'
+
 	return environment
 
 class MoultiMessageException(Exception):
 	pass
 
 class Moulti(App):
 	"""
```

### Comparing `moulti-1.7.0/src/moulti/askpass.py` & `moulti-1.8.0/src/moulti/askpass.py`

 * *Files identical despite different names*

### Comparing `moulti-1.7.0/src/moulti/cli.py` & `moulti-1.8.0/src/moulti/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # ruff: noqa: E501 Line too long
 import os
 import sys
 import json
 from argparse import ArgumentParser, BooleanOptionalAction, _SubParsersAction
 from pathlib import Path
-from typing import Any, Generator
+from typing import Generator
 import argcomplete
 from . import __version__ as moulti_version
+from .diff import diff_parse, diff_run
 from .helpers import pint, float_str, send_to_moulti_and_handle_reply
+from .pipeline import pipeline
 from .protocol import send_to_moulti, PRINTABLE_MOULTI_SOCKET
-from .protocol import moulti_connect, send_json_message, recv_json_message
 from .widgets.cli import add_cli_arguments
 
 def init(args: dict) -> None:
 	"""Start a new Moulti instance."""
 
 	# Handle --print-env:
 	if args.pop('print_env', False):
@@ -50,65 +51,31 @@
 				break
 			time.sleep(delay / 1000.0)
 	sys.exit(0 if connected else 1)
 
 def saved_files(directory: Path) -> Generator:
 	"""
 	Iterate over a directory supposedly generated by Moulti's "Save" feature.
-	Yield triplets:
-	- step id (None for instance properties)
-	- Moulti message to send
-	- file descriptor (int) to the related log file (None for questions)
+	Yield pipeline()-compatible triplets.
 	"""
 	json_ext = '.properties.json'
 	for json_file in sorted(directory.glob('*' + json_ext)):
 		if not json_file.is_file():
 			continue
 		with json_file.open(encoding='utf-8', errors='surrogateescape') as json_file_desc:
 			data = json.load(json_file_desc)
 			log_file = json_file.with_name(json_file.name[:-len(json_ext)] + '.contents.log')
 			fileno = os.open(str(log_file), os.O_RDONLY) if log_file.is_file() else None
 			yield data.get('id'), data, fileno
 
 def load(args: dict, read_size: int = 1024**2) -> None:
 	"""
 	Load the contents of a directory supposedly generated by Moulti's "Save" feature and push it to a Moulti instance.
-	Note: so far, this is the only function in Moulti that pipelines messages and replies. Therefore, it is also the
-	only function that actually leverages message ids.
 	"""
-	errors = 0
-	sent_messages: dict[str, bool] = {}
-	def send_message(*args: Any) -> None:
-		msg_id = send_json_message(*args)
-		sent_messages[msg_id] = False
-	filenos = []
-	with moulti_connect() as moulti_socket:
-		for step_id, data, fileno in saved_files(args['saved_directory']):
-			# Send all messages using protocol pipelining:
-			try:
-				# Properties, typically a command that creates and configures a step:
-				send_message(moulti_socket, data)
-				# Contents:
-				if fileno is not None:
-					filenos.append(fileno)
-					pass_msg = {'command': 'pass', 'id': step_id, 'read_size': read_size}
-					send_message(moulti_socket, pass_msg, [fileno])
-			except Exception as exc:
-				errors += 1
-				print(f'Error with {step_id}/{data}/{fileno}: {exc}')
-		# Receive replies to all sent messages:
-		while not all(sent_messages.values()):
-			reply, _ = recv_json_message(moulti_socket, 0)
-			if 'msgid' in reply and reply['msgid'] in sent_messages:
-				sent_messages[reply['msgid']] = True
-				if reply.get('done') is not True:
-					errors += 1
-					print(f'Error: {reply.get("error")}')
-		for fileno in filenos:
-			os.close(fileno)
+	errors = pipeline(saved_files(args['saved_directory']), read_size)
 	sys.exit(errors)
 
 def add_main_commands(subparsers: _SubParsersAction) -> None:
 	# moulti init
 	init_parser = subparsers.add_parser('init', help='Start a new Moulti instance.')
 	init_parser.set_defaults(func=init)
 
@@ -137,14 +104,25 @@
 
 	# moulti load
 	load_parser = subparsers.add_parser('load', help='Load a saved directory into Moulti')
 	load_parser.set_defaults(func=load, command='load')
 	arg = load_parser.add_argument('saved_directory', type=Path, help='path to a directory generated by Moulti\'s "Save" feature')
 	arg.completer = argcomplete.completers.DirectoriesCompleter()
 
+	# moulti diff parse/run
+	diff_parser = subparsers.add_parser('diff', help='Load unified diff data into Moulti')
+	diff_subparsers = diff_parser.add_subparsers(required=True)
+	diff_parse_parser = diff_subparsers.add_parser('parse', help='Load unified diff data into Moulti from a file')
+	diff_parse_parser.set_defaults(func=diff_parse)
+	arg = diff_parse_parser.add_argument('diff_filepath', type=Path, help='path to a unified diff file')
+	arg.completer = argcomplete.completers.FilesCompleter()
+	diff_run_parser = diff_subparsers.add_parser('run', help='Load unified diff data into Moulti from a command')
+	diff_run_parser.set_defaults(func=diff_run)
+	diff_run_parser.add_argument('command', type=str, nargs='+', help='command to run along with its arguments')
+
 	# moulti scroll
 	scroll_parser = subparsers.add_parser('scroll', help='Scroll to make a specific step visible')
 	scroll_parser.set_defaults(func=send_to_moulti_and_handle_reply, command='scroll')
 	scroll_parser.add_argument('id', type=str, help='step identifier')
 	scroll_parser.add_argument('offset', type=int, nargs='?', default=None, help='-1: last line, 0: first line, 1: second line, etc.')
 
 def build_arg_parser() -> ArgumentParser:
```

### Comparing `moulti-1.7.0/src/moulti/helpers.py` & `moulti-1.8.0/src/moulti/helpers.py`

 * *Files identical despite different names*

### Comparing `moulti-1.7.0/src/moulti/precli.py` & `moulti-1.8.0/src/moulti/precli.py`

 * *Files identical despite different names*

### Comparing `moulti-1.7.0/src/moulti/protocol.py` & `moulti-1.8.0/src/moulti/protocol.py`

 * *Files identical despite different names*

### Comparing `moulti-1.7.0/src/moulti/widgets/abstractquestion/cli.py` & `moulti-1.8.0/src/moulti/widgets/abstractquestion/cli.py`

 * *Files identical despite different names*

### Comparing `moulti-1.7.0/src/moulti/widgets/abstractquestion/tui.py` & `moulti-1.8.0/src/moulti/widgets/abstractquestion/tui.py`

 * *Files identical despite different names*

### Comparing `moulti-1.7.0/src/moulti/widgets/abstractstep/cli.py` & `moulti-1.8.0/src/moulti/widgets/abstractstep/cli.py`

 * *Files identical despite different names*

### Comparing `moulti-1.7.0/src/moulti/widgets/abstractstep/tui.py` & `moulti-1.8.0/src/moulti/widgets/abstractstep/tui.py`

 * *Files identical despite different names*

### Comparing `moulti-1.7.0/src/moulti/widgets/buttonquestion/cli.py` & `moulti-1.8.0/src/moulti/widgets/buttonquestion/cli.py`

 * *Files identical despite different names*

### Comparing `moulti-1.7.0/src/moulti/widgets/buttonquestion/tui.py` & `moulti-1.8.0/src/moulti/widgets/buttonquestion/tui.py`

 * *Files identical despite different names*

### Comparing `moulti-1.7.0/src/moulti/widgets/collapsiblestep/cli.py` & `moulti-1.8.0/src/moulti/widgets/collapsiblestep/cli.py`

 * *Files identical despite different names*

### Comparing `moulti-1.7.0/src/moulti/widgets/collapsiblestep/tui.py` & `moulti-1.8.0/src/moulti/widgets/collapsiblestep/tui.py`

 * *Files identical despite different names*

### Comparing `moulti-1.7.0/src/moulti/widgets/divider/cli.py` & `moulti-1.8.0/src/moulti/widgets/divider/cli.py`

 * *Files identical despite different names*

### Comparing `moulti-1.7.0/src/moulti/widgets/divider/tui.py` & `moulti-1.8.0/src/moulti/widgets/divider/tui.py`

 * *Files identical despite different names*

### Comparing `moulti-1.7.0/src/moulti/widgets/inputquestion/cli.py` & `moulti-1.8.0/src/moulti/widgets/inputquestion/cli.py`

 * *Files identical despite different names*

### Comparing `moulti-1.7.0/src/moulti/widgets/inputquestion/tui.py` & `moulti-1.8.0/src/moulti/widgets/inputquestion/tui.py`

 * *Files identical despite different names*

### Comparing `moulti-1.7.0/src/moulti/widgets/moulticonsole.py` & `moulti-1.8.0/src/moulti/widgets/moulticonsole.py`

 * *Files identical despite different names*

### Comparing `moulti-1.7.0/src/moulti/widgets/moultilog.py` & `moulti-1.8.0/src/moulti/widgets/moultilog.py`

 * *Files identical despite different names*

### Comparing `moulti-1.7.0/src/moulti/widgets/quitdialog.py` & `moulti-1.8.0/src/moulti/widgets/quitdialog.py`

 * *Files identical despite different names*

### Comparing `moulti-1.7.0/src/moulti/widgets/step/cli.py` & `moulti-1.8.0/src/moulti/widgets/step/cli.py`

 * *Files identical despite different names*

### Comparing `moulti-1.7.0/src/moulti/widgets/step/tui.py` & `moulti-1.8.0/src/moulti/widgets/step/tui.py`

 * *Files identical despite different names*

### Comparing `moulti-1.7.0/src/moulti/widgets/stepcontainer.py` & `moulti-1.8.0/src/moulti/widgets/stepcontainer.py`

 * *Files identical despite different names*

### Comparing `moulti-1.7.0/src/moulti/widgets/tui.py` & `moulti-1.8.0/src/moulti/widgets/tui.py`

 * *Files identical despite different names*

### Comparing `moulti-1.7.0/src/moulti.egg-info/PKG-INFO` & `moulti-1.8.0/src/moulti.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,54 @@
 Metadata-Version: 2.1
 Name: moulti
-Version: 1.7.0
+Version: 1.8.0
 Summary: Moulti is a CLI-driven Terminal User Interface (TUI) that enables you to assign the numerous lines emitted by your scripts to visual, collapsible blocks called steps.
 Home-page: https://github.com/xavierog/moulti
 Author: Xavier G.
 Author-email: xavier.moulti@kindwolf.org
 License: MIT
-Keywords: cli,tui,curses,terminal,multiplex,script,output,steps,textual,collapsible
+Keywords: cli,tui,curses,terminal,multiplex,script,output,steps,textual,collapsible,ansible,diff
 Classifier: Environment :: Console :: Curses
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: System :: Logging
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: textual>=0.53
 Requires-Dist: pyperclip
 Requires-Dist: argcomplete
+Requires-Dist: unidiff
 
 # MOULTI
 
 Moulti changes the way your shell scripts (bash, zsh, etc.) display their output in your terminal.
 Moulti enables you to assign the numerous lines emitted by your scripts to "steps", i.e. visual, collapsible blocks featuring their own title and color.
 
 Here is how [upgrading a Debian system](examples/upgrade-system.bash) looks like with Moulti:
 
 ![Moulti demo: Debian upgrade (Animated PNG)](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-demo-debian-upgrade.png?20240218)
 
 Interested? [Run this demo in a container using docker or podman](https://hub.docker.com/r/xavierong/moulti-demo)
 
-Moulti is a tool meant for people who write and execute shell scripts.
+Not convinced yet? What if the output of your Ansible playbooks looked like this?
+
+![Moulti: Ansible playbook output](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-ansible.png?20240505)
+
+Moulti is a tool meant for people who write and execute shell scripts and/or Ansible playbooks.
 Specifically, if you find yourself scrolling up your terminal to ensure everything went fine while your script is still running, then Moulti is made for you.
 
+By the way, Moulti can also display unified diff files:
+
+![Moulti: unified diff output](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-diff.png?20240505)
+
 ## How?
 
 Synopsis:
 
 1. Start a Moulti instance: `moulti init`
 2. Add a step: `moulti step add step_name --title='some clever title here'`
 3. Fill it: `whatever_your_script_does | moulti pass step_name`
@@ -55,14 +64,15 @@
 
 ![Moulti button question](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-button-question.png?20240218)
 
 Moulti also features:
 - a **progress bar**: [documentation](Documentation.md#progress-bar)
 - programmatic scrolling: [documentation](Documentation.md#programmatically-scrolling-through-steps)
 - an askpass helper named `moulti-askpass`: [documentation](Documentation.md#moulti-run-dealing-with-ssh)
+- support for [Ansible playbooks](Documentation.md#moulti-run-dealing-with-ansible) and [unified diff](Documentation.md#moulti-diff)
 
 When it comes to look and feel, Moulti can be customised:
 
 - through `moulti set`: define whether Moulti steps flow up or down: [documentation](Documentation.md#multiple-ways-to-display-steps)
 - through [Textual CSS (TCSS)](https://textual.textualize.io/guide/CSS/): [documentation](Documentation.md#how-to-define-my-own-step-classes-)
 - through ANSI themes: [documentation](Documentation.md#appearance-look-and-feel)
```

### Comparing `moulti-1.7.0/src/moulti.egg-info/SOURCES.txt` & `moulti-1.8.0/src/moulti.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,23 +4,27 @@
 setup.py
 src/moulti/__init__.py
 src/moulti/__main__.py
 src/moulti/ansi.py
 src/moulti/app.py
 src/moulti/askpass.py
 src/moulti/cli.py
+src/moulti/diff.py
 src/moulti/helpers.py
+src/moulti/pipeline.py
 src/moulti/precli.py
 src/moulti/protocol.py
 src/moulti.egg-info/PKG-INFO
 src/moulti.egg-info/SOURCES.txt
 src/moulti.egg-info/dependency_links.txt
 src/moulti.egg-info/entry_points.txt
 src/moulti.egg-info/requires.txt
 src/moulti.egg-info/top_level.txt
+src/moulti/ansible/__init__.py
+src/moulti/ansible/moulti.py
 src/moulti/widgets/__init__.py
 src/moulti/widgets/cli.py
 src/moulti/widgets/moulticonsole.py
 src/moulti/widgets/moultilog.py
 src/moulti/widgets/quitdialog.py
 src/moulti/widgets/stepcontainer.py
 src/moulti/widgets/tui.py
```

