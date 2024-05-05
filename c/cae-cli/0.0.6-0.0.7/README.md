# Comparing `tmp/cae_cli-0.0.6.tar.gz` & `tmp/cae_cli-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cae_cli-0.0.6.tar", last modified: Sun May  5 19:19:23 2024, max compression
+gzip compressed data, was "cae_cli-0.0.7.tar", last modified: Sun May  5 19:25:12 2024, max compression
```

## Comparing `cae_cli-0.0.6.tar` & `cae_cli-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 19:19:23.841757 cae_cli-0.0.6/
--rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      408 2024-05-05 19:19:23.840752 cae_cli-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 19:19:23.818215 cae_cli-0.0.6/cae/
--rw-rw-rw-   0        0        0     7618 2024-05-05 04:35:29.000000 cae_cli-0.0.6/cae/ArchFlowJavaWeb.py
--rw-rw-rw-   0        0        0       34 2024-05-05 19:15:06.000000 cae_cli-0.0.6/cae/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 19:19:23.839246 cae_cli-0.0.6/cae_cli.egg-info/
--rw-rw-rw-   0        0        0      408 2024-05-05 19:19:23.000000 cae_cli-0.0.6/cae_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2024-05-05 19:19:23.000000 cae_cli-0.0.6/cae_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 19:19:23.000000 cae_cli-0.0.6/cae_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-05 19:19:23.000000 cae_cli-0.0.6/cae_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-05 19:19:23.000000 cae_cli-0.0.6/cae_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-05 19:19:23.841757 cae_cli-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      544 2024-05-05 19:19:09.000000 cae_cli-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 19:25:12.865116 cae_cli-0.0.7/
+-rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      408 2024-05-05 19:25:12.863115 cae_cli-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 19:25:12.850117 cae_cli-0.0.7/cae/
+-rw-rw-rw-   0        0        0     7618 2024-05-05 04:35:29.000000 cae_cli-0.0.7/cae/ArchFlowJavaWeb.py
+-rw-rw-rw-   0        0        0       34 2024-05-05 19:15:06.000000 cae_cli-0.0.7/cae/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 19:25:12.862116 cae_cli-0.0.7/cae_cli.egg-info/
+-rw-rw-rw-   0        0        0      408 2024-05-05 19:25:12.000000 cae_cli-0.0.7/cae_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2024-05-05 19:25:12.000000 cae_cli-0.0.7/cae_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 19:25:12.000000 cae_cli-0.0.7/cae_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-05 19:25:12.000000 cae_cli-0.0.7/cae_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-05 19:25:12.000000 cae_cli-0.0.7/cae_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-05 19:25:12.865116 cae_cli-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      527 2024-05-05 19:25:05.000000 cae_cli-0.0.7/setup.py
```

### Comparing `cae_cli-0.0.6/LICENSE` & `cae_cli-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cae_cli-0.0.6/README.md` & `cae_cli-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `cae_cli-0.0.6/cae/ArchFlowJavaWeb.py` & `cae_cli-0.0.7/cae/ArchFlowJavaWeb.py`

 * *Files identical despite different names*

