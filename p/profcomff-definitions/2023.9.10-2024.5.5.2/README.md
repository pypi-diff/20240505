# Comparing `tmp/profcomff_definitions-2023.9.10.tar.gz` & `tmp/profcomff_definitions-2024.5.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profcomff_definitions-2023.9.10.tar", last modified: Mon Sep 11 09:37:58 2023, max compression
+gzip compressed data, was "profcomff_definitions-2024.5.5.2.tar", last modified: Sat May  4 22:43:20 2024, max compression
```

## Comparing `profcomff_definitions-2023.9.10.tar` & `profcomff_definitions-2024.5.5.2.tar`

### file list

```diff
@@ -1,38 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 09:37:58.535211 profcomff_definitions-2023.9.10/
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2023-09-11 09:37:47.000000 profcomff_definitions-2023.9.10/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6173 2023-09-11 09:37:58.535211 profcomff_definitions-2023.9.10/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2023-09-11 09:37:47.000000 profcomff_definitions-2023.9.10/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 09:37:58.531211 profcomff_definitions-2023.9.10/profcomff_definitions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 09:37:58.531211 profcomff_definitions-2023.9.10/profcomff_definitions/DM/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-09-11 09:37:47.000000 profcomff_definitions-2023.9.10/profcomff_definitions/DM/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 09:37:58.531211 profcomff_definitions-2023.9.10/profcomff_definitions/DWH/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-09-11 09:37:47.000000 profcomff_definitions-2023.9.10/profcomff_definitions/DWH/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 09:37:58.531211 profcomff_definitions-2023.9.10/profcomff_definitions/ODS/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-09-11 09:37:47.000000 profcomff_definitions-2023.9.10/profcomff_definitions/ODS/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 09:37:58.535211 profcomff_definitions-2023.9.10/profcomff_definitions/STG/
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2023-09-11 09:37:47.000000 profcomff_definitions-2023.9.10/profcomff_definitions/STG/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2023-09-11 09:37:47.000000 profcomff_definitions-2023.9.10/profcomff_definitions/STG/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2023-09-11 09:37:47.000000 profcomff_definitions-2023.9.10/profcomff_definitions/STG/marketing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2023-09-11 09:37:47.000000 profcomff_definitions-2023.9.10/profcomff_definitions/STG/pinger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2023-09-11 09:37:47.000000 profcomff_definitions-2023.9.10/profcomff_definitions/STG/print.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2023-09-11 09:37:47.000000 profcomff_definitions-2023.9.10/profcomff_definitions/STG/services.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2023-09-11 09:37:47.000000 profcomff_definitions-2023.9.10/profcomff_definitions/STG/social.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2023-09-11 09:37:47.000000 profcomff_definitions-2023.9.10/profcomff_definitions/STG/timetable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2023-09-11 09:37:47.000000 profcomff_definitions-2023.9.10/profcomff_definitions/STG/union_member.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2023-09-11 09:37:47.000000 profcomff_definitions-2023.9.10/profcomff_definitions/STG/userdata.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2023-09-11 09:37:47.000000 profcomff_definitions-2023.9.10/profcomff_definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2023-09-11 09:37:47.000000 profcomff_definitions-2023.9.10/profcomff_definitions/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 09:37:58.531211 profcomff_definitions-2023.9.10/profcomff_definitions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6173 2023-09-11 09:37:58.000000 profcomff_definitions-2023.9.10/profcomff_definitions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      886 2023-09-11 09:37:58.000000 profcomff_definitions-2023.9.10/profcomff_definitions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-11 09:37:58.000000 profcomff_definitions-2023.9.10/profcomff_definitions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-09-11 09:37:58.000000 profcomff_definitions-2023.9.10/profcomff_definitions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-09-11 09:37:58.000000 profcomff_definitions-2023.9.10/profcomff_definitions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      362 2023-09-11 09:37:47.000000 profcomff_definitions-2023.9.10/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-11 09:37:58.535211 profcomff_definitions-2023.9.10/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      728 2023-09-11 09:37:47.000000 profcomff_definitions-2023.9.10/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 09:37:58.535211 profcomff_definitions-2023.9.10/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-11 09:37:47.000000 profcomff_definitions-2023.9.10/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2023-09-11 09:37:47.000000 profcomff_definitions-2023.9.10/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2023-09-11 09:37:47.000000 profcomff_definitions-2023.9.10/tests/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2023-09-11 09:37:47.000000 profcomff_definitions-2023.9.10/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:43:20.303697 profcomff_definitions-2024.5.5.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:43:20.287697 profcomff_definitions-2024.5.5.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:43:20.291697 profcomff_definitions-2024.5.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/.github/workflows/checks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/.github/workflows/deploy_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     9032 2024-05-04 22:43:20.303697 profcomff_definitions-2024.5.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/alembic.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:43:20.291697 profcomff_definitions-2024.5.5.2/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/migrations/README
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/migrations/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:43:20.291697 profcomff_definitions-2024.5.5.2/migrations/rights/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/migrations/rights/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/migrations/rights/operations_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/migrations/rights/operations_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/migrations/rights/render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8112 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/migrations/rights/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:43:20.295697 profcomff_definitions-2024.5.5.2/migrations/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/migrations/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/migrations/schema/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/migrations/schema/render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/migrations/schema/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/migrations/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:43:20.295697 profcomff_definitions-2024.5.5.2/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/migrations/versions/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/migrations/versions/0a24041f09d1_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/migrations/versions/1e868db5c6ea_physics_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/migrations/versions/4892e78eb989_add_raw_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85873 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/migrations/versions/77d9cf76373d_the_great_megre.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59583 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/migrations/versions/a80b250420e4_schema_integrity_fixes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/migrations/versions/b0d0bbe799db_fix_reciever.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/migrations/versions/d71054079206_fix_tg_chat_int_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/migrations/versions/fa6331fe4c72_rights.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:43:20.295697 profcomff_definitions-2024.5.5.2/profcomff_definitions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:43:20.295697 profcomff_definitions-2024.5.5.2/profcomff_definitions/DM/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/profcomff_definitions/DM/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/profcomff_definitions/DM/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:43:20.299697 profcomff_definitions-2024.5.5.2/profcomff_definitions/DWH/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/profcomff_definitions/DWH/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/profcomff_definitions/DWH/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:43:20.299697 profcomff_definitions-2024.5.5.2/profcomff_definitions/ODS/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/profcomff_definitions/ODS/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/profcomff_definitions/ODS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/profcomff_definitions/ODS/timetable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:43:20.299697 profcomff_definitions-2024.5.5.2/profcomff_definitions/STG/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/profcomff_definitions/STG/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/profcomff_definitions/STG/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/profcomff_definitions/STG/achievement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/profcomff_definitions/STG/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/profcomff_definitions/STG/marketing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/profcomff_definitions/STG/physics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/profcomff_definitions/STG/pinger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/profcomff_definitions/STG/print.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/profcomff_definitions/STG/rasphysmsu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/profcomff_definitions/STG/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/profcomff_definitions/STG/social.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/profcomff_definitions/STG/timetable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/profcomff_definitions/STG/union_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/profcomff_definitions/STG/userdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/profcomff_definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/profcomff_definitions/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:43:20.299697 profcomff_definitions-2024.5.5.2/profcomff_definitions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9032 2024-05-04 22:43:20.000000 profcomff_definitions-2024.5.5.2/profcomff_definitions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-04 22:43:20.000000 profcomff_definitions-2024.5.5.2/profcomff_definitions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 22:43:20.000000 profcomff_definitions-2024.5.5.2/profcomff_definitions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-04 22:43:20.000000 profcomff_definitions-2024.5.5.2/profcomff_definitions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-04 22:43:20.000000 profcomff_definitions-2024.5.5.2/profcomff_definitions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/requirements.dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 22:43:20.303697 profcomff_definitions-2024.5.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:43:20.299697 profcomff_definitions-2024.5.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/tests/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-04 22:43:11.000000 profcomff_definitions-2024.5.5.2/tests/tests.py
```

### Comparing `profcomff_definitions-2023.9.10/LICENSE` & `profcomff_definitions-2024.5.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2023.9.10/PKG-INFO` & `profcomff_definitions-2024.5.5.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: profcomff_definitions
-Version: 2023.9.10
-Summary: Data warehouse definitions and schemas
-Home-page: https://github.com/profcomff/dwh-definitions
-Author: Stanislav Roslavtsev
-Author-email: roslavtzev.stanislaw@yandex.ru
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: SQLAlchemy
-Requires-Dist: psycopg2-binary
-
 # dwh-definitions
 Библиотека, описывающая структуру всех баз данных профкома ФФ. Реализована с помощью разделения всех баз данных в 4 категории - [STG](https://github.com/profcomff/dwh-definitions/blob/main/profcomff_definitions/STG/README.md), [DWH](https://github.com/profcomff/dwh-definitions/blob/main/profcomff_definitions/DWH/README.md), [ODS](https://github.com/profcomff/dwh-definitions/blob/main/profcomff_definitions/ODS/README.md) и [DM](https://github.com/profcomff/dwh-definitions/blob/main/profcomff_definitions/DM/README.md).
 
 ## Функционал
 - Удобное и структурированное хранение данных
 - Разграничение и удобное управление правами доступа
```

### Comparing `profcomff_definitions-2023.9.10/profcomff_definitions/STG/auth.py` & `profcomff_definitions-2024.5.5.2/profcomff_definitions/STG/auth.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,79 +1,88 @@
-import datetime
+from datetime import datetime
 
-from sqlalchemy import Boolean, DateTime, Integer, String
 from sqlalchemy.orm import Mapped, mapped_column
 
 from profcomff_definitions.base import Base
 
 
 class User(Base):
-    id: Mapped[int] = mapped_column(Integer, primary_key=True)
-    is_deleted: Mapped[bool] = mapped_column(Boolean)
-    create_ts: Mapped[datetime.datetime] = mapped_column(DateTime)
-    update_ts: Mapped[datetime.datetime] = mapped_column(DateTime)
+    id: Mapped[int] = mapped_column(primary_key=True)
+    is_deleted: Mapped[bool | None]
+    create_ts: Mapped[datetime | None]
+    update_ts: Mapped[datetime | None]
 
 
 class Group(Base):
-    id: Mapped[int] = mapped_column(Integer, primary_key=True)
-    name: Mapped[str] = mapped_column(String)
-    parent_id: Mapped[int] = mapped_column(Integer)
-    create_ts: Mapped[datetime.datetime] = mapped_column(DateTime)
-    update_ts: Mapped[datetime.datetime] = mapped_column(DateTime)
-    is_deleted: Mapped[bool] = mapped_column(Boolean)
+    id: Mapped[int] = mapped_column(primary_key=True)
+    name: Mapped[str | None]
+    parent_id: Mapped[int | None]
+    create_ts: Mapped[datetime | None]
+    update_ts: Mapped[datetime | None]
+    is_deleted: Mapped[bool | None]
 
 
 class UserGroup(Base):
-    id: Mapped[int] = mapped_column(Integer, primary_key=True)
-    user_id: Mapped[int] = mapped_column(Integer)
-    group_id: Mapped[int] = mapped_column(Integer)
-    is_deleted: Mapped[bool] = mapped_column(Boolean)
+    id: Mapped[int] = mapped_column(primary_key=True)
+    user_id: Mapped[int | None]
+    group_id: Mapped[int | None]
+    is_deleted: Mapped[bool | None]
 
 
 class AuthMethod(Base):
-    id: Mapped[int] = mapped_column(Integer, primary_key=True)
-    user_id: Mapped[int] = mapped_column(Integer)
-    auth_method: Mapped[str] = mapped_column(String)
-    param: Mapped[str] = mapped_column(String)
-    value: Mapped[str] = mapped_column(String)
-    create_ts: Mapped[datetime.datetime] = mapped_column(DateTime)
-    update_ts: Mapped[datetime.datetime] = mapped_column(DateTime)
-    is_deleted: Mapped[bool] = mapped_column(Boolean)
+    id: Mapped[int] = mapped_column(primary_key=True)
+    user_id: Mapped[int | None]
+    auth_method: Mapped[str | None]
+    param: Mapped[str | None]
+    value: Mapped[str | None]
+    create_ts: Mapped[datetime | None]
+    update_ts: Mapped[datetime | None]
+    is_deleted: Mapped[bool | None]
 
 
 class UserSession(Base):
-    id: Mapped[int] = mapped_column(Integer, primary_key=True)
-    session_name: Mapped[str] = mapped_column(String)
-    user_id: Mapped[int] = mapped_column(Integer)
-    expires: Mapped[datetime.datetime] = mapped_column(DateTime)
-    token: Mapped[str] = mapped_column(String)
-    last_activity: Mapped[datetime.datetime] = mapped_column(DateTime)
-    create_ts: Mapped[datetime.datetime] = mapped_column(DateTime)
+    id: Mapped[int] = mapped_column(primary_key=True)
+    session_name: Mapped[str | None]
+    user_id: Mapped[int | None]
+    expires: Mapped[datetime | None]
+    token: Mapped[str | None]
+    last_activity: Mapped[datetime | None]
+    create_ts: Mapped[datetime | None]
 
 
 class Scope(Base):
-    id: Mapped[int] = mapped_column(Integer, primary_key=True)
-    creator_id: Mapped[int] = mapped_column(Integer)
-    name: Mapped[str] = mapped_column(String)
-    comment: Mapped[str] = mapped_column(String)
-    is_deleted: Mapped[bool] = mapped_column(Boolean)
+    id: Mapped[int] = mapped_column(primary_key=True)
+    creator_id: Mapped[int | None]
+    name: Mapped[str | None]
+    comment: Mapped[str | None]
+    is_deleted: Mapped[bool | None]
 
 
 class GroupScope(Base):
-    id: Mapped[int] = mapped_column(Integer, primary_key=True)
-    group_id: Mapped[int] = mapped_column(Integer)
-    scope_id: Mapped[int] = mapped_column(Integer)
-    is_deleted: Mapped[bool] = mapped_column(Boolean)
+    id: Mapped[int] = mapped_column(primary_key=True)
+    group_id: Mapped[int | None]
+    scope_id: Mapped[int | None]
+    is_deleted: Mapped[bool | None]
 
 
 class UserSessionScope(Base):
-    id: Mapped[int] = mapped_column(Integer, primary_key=True)
-    user_session_id: Mapped[int] = mapped_column(Integer)
-    scope_id: Mapped[int] = mapped_column(Integer)
-    is_deleted: Mapped[bool] = mapped_column(Boolean)
+    id: Mapped[int] = mapped_column(primary_key=True)
+    user_session_id: Mapped[int | None]
+    scope_id: Mapped[int | None]
+    is_deleted: Mapped[bool | None]
 
 
 class UserMessageDelay(Base):
-    id: Mapped[int] = mapped_column(Integer, primary_key=True)
-    delay_time: Mapped[datetime.datetime] = mapped_column(DateTime)
-    user_email: Mapped[str] = mapped_column(String)
-    user_ip: Mapped[str] = mapped_column(String)
+    id: Mapped[int] = mapped_column(primary_key=True)
+    delay_time: Mapped[datetime | None]
+    user_email: Mapped[str | None]
+    user_ip: Mapped[str | None]
+
+
+class DynamicOption(Base):
+    id: Mapped[int] = mapped_column(primary_key=True)
+    create_ts: Mapped[datetime | None]
+    value_integer: Mapped[int | None]
+    value_string: Mapped[str | None]
+    value_double: Mapped[float | None]
+    update_ts: Mapped[datetime | None]
+    name: Mapped[str | None]
```

### Comparing `profcomff_definitions-2023.9.10/profcomff_definitions/STG/social.py` & `profcomff_definitions-2024.5.5.2/profcomff_definitions/STG/union_member.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,30 @@
-from datetime import datetime
-
-import sqlalchemy as sa
 from sqlalchemy.orm import Mapped, mapped_column
 
 from profcomff_definitions.base import Base
 
 
-class WebhookStorage(Base):
-    id: Mapped[int] = mapped_column(sa.Integer, primary_key=True)
-    system: Mapped[str] = mapped_column(sa.String)
-    message: Mapped[sa.JSON] = mapped_column(sa.JSON(True))
-
-
-class VkGroups(Base):
-    id: Mapped[int] = mapped_column(sa.Integer, primary_key=True)
-    group_id: Mapped[int] = mapped_column(sa.Integer)
-    confirmation_token: Mapped[str] = mapped_column(sa.String)
-    secret_key: Mapped[str] = mapped_column(sa.String)
-    create_ts: Mapped[datetime] = mapped_column(sa.DateTime)
-    update_ts: Mapped[datetime] = mapped_column(sa.DateTime)
+class UnionMember(Base):
+    id: Mapped[int] = mapped_column(primary_key=True)
+    type_of_learning: Mapped[str | None]
+    rzd_status: Mapped[str | None]
+    academic_level: Mapped[str | None]
+    status: Mapped[str | None]
+    faculty: Mapped[str | None]
+    first_name: Mapped[str | None]
+    last_name: Mapped[str | None]
+    email: Mapped[str | None]
+    date_of_birth: Mapped[str | None]
+    phone_number: Mapped[str | None]
+    image: Mapped[str | None]
+    rzd_datetime: Mapped[str | None]
+    rzd_number: Mapped[str | None]
+    grade_level: Mapped[int | None]
+    has_student_id: Mapped[bool | None]
+    entry_date: Mapped[str | None]
+    status_gain_date: Mapped[str | None]
+    card_id: Mapped[int | None]
+    card_status: Mapped[str | None]
+    card_date: Mapped[str | None]
+    card_number: Mapped[str | None]
+    card_user: Mapped[str | None]
+    card: Mapped[str | None]
```

### Comparing `profcomff_definitions-2023.9.10/profcomff_definitions/base.py` & `profcomff_definitions-2024.5.5.2/profcomff_definitions/base.py`

 * *Files identical despite different names*

### Comparing `profcomff_definitions-2023.9.10/profcomff_definitions.egg-info/SOURCES.txt` & `profcomff_definitions-2024.5.5.2/profcomff_definitions.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,61 @@
+.gitignore
 LICENSE
+Makefile
 README.md
+alembic.ini
 pyproject.toml
-setup.py
+requirements.dev.txt
+requirements.txt
+.github/workflows/checks.yml
+.github/workflows/deploy_and_publish.yml
+migrations/README
+migrations/env.py
+migrations/script.py.mako
+migrations/rights/__init__.py
+migrations/rights/operations_groups.py
+migrations/rights/operations_tables.py
+migrations/rights/render.py
+migrations/rights/schemas.py
+migrations/schema/__init__.py
+migrations/schema/operations.py
+migrations/schema/render.py
+migrations/schema/schemas.py
+migrations/versions/.gitkeep
+migrations/versions/0a24041f09d1_init.py
+migrations/versions/1e868db5c6ea_physics_contacts.py
+migrations/versions/4892e78eb989_add_raw_html.py
+migrations/versions/77d9cf76373d_the_great_megre.py
+migrations/versions/a80b250420e4_schema_integrity_fixes.py
+migrations/versions/b0d0bbe799db_fix_reciever.py
+migrations/versions/d71054079206_fix_tg_chat_int_type.py
+migrations/versions/fa6331fe4c72_rights.py
 profcomff_definitions/__init__.py
 profcomff_definitions/base.py
 profcomff_definitions.egg-info/PKG-INFO
 profcomff_definitions.egg-info/SOURCES.txt
 profcomff_definitions.egg-info/dependency_links.txt
 profcomff_definitions.egg-info/requires.txt
 profcomff_definitions.egg-info/top_level.txt
+profcomff_definitions/DM/README.md
 profcomff_definitions/DM/__init__.py
+profcomff_definitions/DWH/README.md
 profcomff_definitions/DWH/__init__.py
+profcomff_definitions/ODS/README.md
 profcomff_definitions/ODS/__init__.py
+profcomff_definitions/ODS/timetable.py
+profcomff_definitions/STG/README.md
 profcomff_definitions/STG/__init__.py
+profcomff_definitions/STG/achievement.py
 profcomff_definitions/STG/auth.py
 profcomff_definitions/STG/marketing.py
+profcomff_definitions/STG/physics.py
 profcomff_definitions/STG/pinger.py
 profcomff_definitions/STG/print.py
+profcomff_definitions/STG/rasphysmsu.py
 profcomff_definitions/STG/services.py
 profcomff_definitions/STG/social.py
 profcomff_definitions/STG/timetable.py
 profcomff_definitions/STG/union_member.py
 profcomff_definitions/STG/userdata.py
 tests/__init__.py
 tests/conftest.py
```

### Comparing `profcomff_definitions-2023.9.10/tests/conftest.py` & `profcomff_definitions-2024.5.5.2/tests/conftest.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import os
 from pathlib import Path
+from typing import Generator
 
 import pytest
 from alembic import command
 from alembic.config import Config
 from sqlalchemy import create_engine
 from sqlalchemy.engine import Engine
 
 
 REPO_ROOT = Path(os.path.abspath(os.path.dirname(__file__))).parent.resolve()
 
 
 @pytest.fixture(scope='session')
-def migration() -> None:
+def migration() -> Generator[None, None, None]:
     alembic_cfg = Config()
     alembic_cfg.set_main_option('script_location', str(REPO_ROOT / "migrations"))
     alembic_cfg.set_main_option('sqlalchemy.url', "postgresql://postgres:postgres@localhost:5432/postgres")
+    command.upgrade(alembic_cfg, 'head')
     command.revision(alembic_cfg, autogenerate=True, message="tests")
     command.upgrade(alembic_cfg, 'head')
-    yield migration
-    command.downgrade(alembic_cfg, '-1')
+    yield
+    command.downgrade(alembic_cfg, 'head-1')
 
 
 @pytest.fixture()
-def engine() -> Engine:
+def engine() -> Generator[Engine, None, None]:
     engine = create_engine("postgresql://postgres:postgres@localhost:5432/postgres")
     yield engine
```

### Comparing `profcomff_definitions-2023.9.10/tests/tests.py` & `profcomff_definitions-2024.5.5.2/tests/tests.py`

 * *Files identical despite different names*

