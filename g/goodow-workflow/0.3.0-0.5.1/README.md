# Comparing `tmp/goodow-workflow-0.3.0.tar.gz` & `tmp/goodow_workflow-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goodow-workflow-0.3.0.tar", last modified: Mon Dec  6 07:06:31 2021, max compression
+gzip compressed data, was "goodow_workflow-0.5.1.tar", max compression
```

## Comparing `goodow-workflow-0.3.0.tar` & `goodow_workflow-0.5.1.tar`

### file list

```diff
@@ -1,13 +1,5 @@
-drwxr-xr-x   0 larry      (501) staff       (20)        0 2021-12-06 07:06:31.109861 goodow-workflow-0.3.0/
--rw-r--r--   0 larry      (501) staff       (20)      140 2021-12-06 07:06:31.109396 goodow-workflow-0.3.0/PKG-INFO
-drwxr-xr-x   0 larry      (501) staff       (20)        0 2021-12-06 07:06:31.107211 goodow-workflow-0.3.0/goodow/
--rw-r--r--   0 larry      (501) staff       (20)        0 2021-12-06 07:06:22.000000 goodow-workflow-0.3.0/goodow/__init__.py
-drwxr-xr-x   0 larry      (501) staff       (20)        0 2021-12-06 07:06:31.108941 goodow-workflow-0.3.0/goodow_workflow.egg-info/
--rw-r--r--   0 larry      (501) staff       (20)      140 2021-12-06 07:06:31.000000 goodow-workflow-0.3.0/goodow_workflow.egg-info/PKG-INFO
--rw-r--r--   0 larry      (501) staff       (20)      236 2021-12-06 07:06:31.000000 goodow-workflow-0.3.0/goodow_workflow.egg-info/SOURCES.txt
--rw-r--r--   0 larry      (501) staff       (20)        1 2021-12-06 07:06:31.000000 goodow-workflow-0.3.0/goodow_workflow.egg-info/dependency_links.txt
--rw-r--r--   0 larry      (501) staff       (20)       48 2021-12-06 07:06:31.000000 goodow-workflow-0.3.0/goodow_workflow.egg-info/requires.txt
--rw-r--r--   0 larry      (501) staff       (20)        7 2021-12-06 07:06:31.000000 goodow-workflow-0.3.0/goodow_workflow.egg-info/top_level.txt
--rw-r--r--   0 larry      (501) staff       (20)       89 2021-12-06 06:59:17.000000 goodow-workflow-0.3.0/pyproject.toml
--rw-r--r--   0 larry      (501) staff       (20)       38 2021-12-06 07:06:31.109998 goodow-workflow-0.3.0/setup.cfg
--rw-r--r--   0 larry      (501) staff       (20)      209 2021-12-06 07:04:28.000000 goodow-workflow-0.3.0/setup.py
+-rw-r--r--   0        0        0     1994 2024-05-05 13:01:06.513674 goodow_workflow-0.5.1/goodow/workflow/github/send_alert.py
+-rw-r--r--   0        0        0     1559 2024-05-05 13:01:06.513674 goodow_workflow-0.5.1/goodow/workflow/observability/logger.py
+-rw-r--r--   0        0        0       81 2024-05-05 13:01:06.513674 goodow_workflow-0.5.1/goodow/workflow/observability/util.py
+-rw-r--r--   0        0        0      722 2024-05-05 13:01:20.769851 goodow_workflow-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 goodow_workflow-0.5.1/PKG-INFO
```

