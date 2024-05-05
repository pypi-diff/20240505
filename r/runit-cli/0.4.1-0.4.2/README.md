# Comparing `tmp/runit_cli-0.4.1.tar.gz` & `tmp/runit_cli-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runit_cli-0.4.1.tar", last modified: Wed May  1 12:06:29 2024, max compression
+gzip compressed data, was "runit_cli-0.4.2.tar", last modified: Sun May  5 10:26:53 2024, max compression
```

## Comparing `runit_cli-0.4.1.tar` & `runit_cli-0.4.2.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:29.227735 runit_cli-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-01 12:06:25.000000 runit_cli-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-01 12:06:29.227735 runit_cli-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-05-01 12:06:25.000000 runit_cli-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:29.219735 runit_cli-0.4.1/runit/
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/Request.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17176 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:29.219735 runit_cli-0.4.1/runit/languages/
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/languages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/languages/javascript.py
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/languages/multi.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/languages/php.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/languages/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/languages/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:29.219735 runit_cli-0.4.1/runit/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9537 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/modules/account.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:29.219735 runit_cli-0.4.1/runit/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/plugins/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:29.219735 runit_cli-0.4.1/runit/plugins/languages/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/plugins/languages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/plugins/languages/javascript.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/plugins/languages/language.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/plugins/languages/php.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/plugins/languages/python.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/plugins/languages/r.py
--rw-r--r--   0 runner    (1001) docker     (127)    16501 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/runit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:29.219735 runit_cli-0.4.1/runit/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/templates/.runitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/templates/404.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:29.223734 runit_cli-0.4.1/runit/templates/javascript/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/templates/javascript/main.js
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/templates/javascript/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:29.223734 runit_cli-0.4.1/runit/templates/multi/
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/templates/multi/application.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/templates/multi/composer.json
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/templates/multi/index.php
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/templates/multi/main.js
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/templates/multi/package.json
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/templates/multi/request.php
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/templates/multi/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:29.223734 runit_cli-0.4.1/runit/templates/php/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/templates/php/composer.json
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/templates/php/index.php
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:29.223734 runit_cli-0.4.1/runit/templates/python/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/templates/python/application.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/templates/python/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/templates/request.php
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/templates/runit.json
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:29.215735 runit_cli-0.4.1/runit/tools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:29.223734 runit_cli-0.4.1/runit/tools/javascript/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/tools/javascript/loader.js
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/tools/javascript/runner.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:29.223734 runit_cli-0.4.1/runit/tools/php/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/tools/php/loader.php
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/tools/php/manager.php
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/tools/php/runner.php
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:29.223734 runit_cli-0.4.1/runit/tools/python/
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/tools/python/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-01 12:06:25.000000 runit_cli-0.4.1/runit/tools/python/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:29.227735 runit_cli-0.4.1/runit_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-01 12:06:29.000000 runit_cli-0.4.1/runit_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-01 12:06:29.000000 runit_cli-0.4.1/runit_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:06:29.000000 runit_cli-0.4.1/runit_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-01 12:06:29.000000 runit_cli-0.4.1/runit_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-01 12:06:29.000000 runit_cli-0.4.1/runit_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 12:06:29.000000 runit_cli-0.4.1/runit_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 12:06:29.227735 runit_cli-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-01 12:06:25.000000 runit_cli-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:29.227735 runit_cli-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-01 12:06:25.000000 runit_cli-0.4.1/tests/test_clone_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-01 12:06:25.000000 runit_cli-0.4.1/tests/test_create_new_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-01 12:06:25.000000 runit_cli-0.4.1/tests/test_create_project_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-05-01 12:06:25.000000 runit_cli-0.4.1/tests/test_generate_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     6487 2024-05-01 12:06:25.000000 runit_cli-0.4.1/tests/test_publish_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-05-01 12:06:25.000000 runit_cli-0.4.1/tests/test_run_project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:26:53.784453 runit_cli-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-05 10:26:47.000000 runit_cli-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-05 10:26:53.784453 runit_cli-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-05-05 10:26:47.000000 runit_cli-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:26:53.776453 runit_cli-0.4.2/runit/
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/Request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17176 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:26:53.776453 runit_cli-0.4.2/runit/languages/
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/languages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/languages/javascript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/languages/multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/languages/php.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/languages/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/languages/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:26:53.776453 runit_cli-0.4.2/runit/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9537 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/modules/account.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:26:53.776453 runit_cli-0.4.2/runit/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/plugins/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:26:53.776453 runit_cli-0.4.2/runit/plugins/languages/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/plugins/languages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/plugins/languages/javascript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/plugins/languages/language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/plugins/languages/php.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/plugins/languages/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/plugins/languages/r.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/runit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:26:53.780453 runit_cli-0.4.2/runit/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/templates/.runitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/templates/404.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:26:53.780453 runit_cli-0.4.2/runit/templates/javascript/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/templates/javascript/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/templates/javascript/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:26:53.780453 runit_cli-0.4.2/runit/templates/multi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/templates/multi/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/templates/multi/composer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/templates/multi/index.php
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/templates/multi/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/templates/multi/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/templates/multi/request.php
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/templates/multi/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:26:53.780453 runit_cli-0.4.2/runit/templates/php/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/templates/php/composer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/templates/php/index.php
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:26:53.780453 runit_cli-0.4.2/runit/templates/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/templates/python/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/templates/python/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/templates/request.php
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/templates/runit.json
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:26:53.772453 runit_cli-0.4.2/runit/tools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:26:53.780453 runit_cli-0.4.2/runit/tools/javascript/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/tools/javascript/loader.js
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/tools/javascript/runner.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:26:53.780453 runit_cli-0.4.2/runit/tools/php/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/tools/php/loader.php
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/tools/php/manager.php
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/tools/php/runner.php
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:26:53.780453 runit_cli-0.4.2/runit/tools/python/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/tools/python/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-05 10:26:47.000000 runit_cli-0.4.2/runit/tools/python/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:26:53.784453 runit_cli-0.4.2/runit_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-05 10:26:53.000000 runit_cli-0.4.2/runit_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-05 10:26:53.000000 runit_cli-0.4.2/runit_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 10:26:53.000000 runit_cli-0.4.2/runit_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-05 10:26:53.000000 runit_cli-0.4.2/runit_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-05 10:26:53.000000 runit_cli-0.4.2/runit_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-05 10:26:53.000000 runit_cli-0.4.2/runit_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 10:26:53.784453 runit_cli-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-05 10:26:47.000000 runit_cli-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:26:53.784453 runit_cli-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-05 10:26:47.000000 runit_cli-0.4.2/tests/test_clone_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-05 10:26:47.000000 runit_cli-0.4.2/tests/test_create_new_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-05 10:26:47.000000 runit_cli-0.4.2/tests/test_create_project_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-05-05 10:26:47.000000 runit_cli-0.4.2/tests/test_generate_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6487 2024-05-05 10:26:47.000000 runit_cli-0.4.2/tests/test_publish_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-05-05 10:26:47.000000 runit_cli-0.4.2/tests/test_run_project.py
```

### Comparing `runit_cli-0.4.1/PKG-INFO` & `runit_cli-0.4.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runit-cli
-Version: 0.4.1
+Version: 0.4.2
 Summary: Develop serverless applications
 Author: Amos Amissah
 Author-email: theonlyamos@gmail.com
 Project-URL: Source, https://github.com/theonlyamos/runit
 Project-URL: Tracker, https://github.com/theonlyamos/runit/issues
 Keywords: python3 runit developer serverless architecture docker
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `runit_cli-0.4.1/README.md` & `runit_cli-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.1/runit/Request.py` & `runit_cli-0.4.2/runit/Request.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.1/runit/cli.py` & `runit_cli-0.4.2/runit/cli.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.1/runit/constants.py` & `runit_cli-0.4.2/runit/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from pathlib import Path
 from dotenv import load_dotenv
 
 load_dotenv()
 
-VERSION = "0.4.1"
+VERSION = "0.4.2"
 CURRENT_PROJECT = ""
 NOT_FOUND_FILE = '404.html'
 DOT_RUNIT_IGNORE = '.runitignore'
 CONFIG_FILE = 'runit.json'
 STARTER_CONFIG_FILE = 'runit.json'
 IS_RUNNING = False
 CURRENT_PROJECT_DIR = Path(os.curdir).resolve()
```

### Comparing `runit_cli-0.4.1/runit/core.py` & `runit_cli-0.4.2/runit/core.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.1/runit/generate.py` & `runit_cli-0.4.2/runit/generate.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.1/runit/languages/__init__.py` & `runit_cli-0.4.2/runit/languages/__init__.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.1/runit/languages/javascript.py` & `runit_cli-0.4.2/runit/languages/javascript.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.1/runit/languages/multi.py` & `runit_cli-0.4.2/runit/languages/multi.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.1/runit/languages/php.py` & `runit_cli-0.4.2/runit/languages/php.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.1/runit/languages/python.py` & `runit_cli-0.4.2/runit/languages/python.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.1/runit/languages/runtime.py` & `runit_cli-0.4.2/runit/languages/runtime.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.1/runit/modules/account.py` & `runit_cli-0.4.2/runit/modules/account.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.1/runit/plugins/base.py` & `runit_cli-0.4.2/runit/plugins/base.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.1/runit/plugins/languages/javascript.py` & `runit_cli-0.4.2/runit/plugins/languages/javascript.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.1/runit/plugins/languages/language.py` & `runit_cli-0.4.2/runit/plugins/languages/language.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.1/runit/plugins/languages/php.py` & `runit_cli-0.4.2/runit/plugins/languages/php.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.1/runit/plugins/languages/python.py` & `runit_cli-0.4.2/runit/plugins/languages/python.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.1/runit/runit.py` & `runit_cli-0.4.2/runit/runit.py`

 * *Files 1% similar despite different names*

```diff
@@ -448,23 +448,23 @@
             logger.info(msg="[-] Deleting old virtual environment...")
             rm_command = "rm -rf" if sys.platform != 'win32' else 'rm -r'
             os.system(f"{rm_command} {os.path.realpath(venv_path)}")
         
         logger.info(msg="[!] Creating virtual environment...")
         os.system("python -m venv venv")
         
-        pip_path = Path(venv_path, 'Scripts', 'pip.exe')
+        pip_path = f"{Path(venv_path, 'bin', 'pip').resolve()}"
         # logger.info(f"--{str(Path(pip_path).resolve())}")
-        if sys.platform != 'win32':
-            pip_path = f"{Path(venv_path, 'bin', 'pip').resolve()}"
+        if sys.platform == 'win32':
+            pip_path = Path(venv_path, 'Scripts', 'pip.exe')
         try:
             logger.info("[!] Installing python packages...")
             # os.system(f"{str(pip_path)} install python-dotenv")
             activate_install_instructions = f"""
-            {str(pip_path)} install python-dotenv -r requirements.txt
+            {str(pip_path)} install -r requirements.txt
             """.strip()
             os.system(activate_install_instructions)
             logger.info("[+] Installed python packages")
         except Exception as e:
             logger.exception(str(e))
             logger.error("[!] Couldn't install packages")
             logger.debug(INSTALL_MODULE_LATER_MESSAGE)
```

### Comparing `runit_cli-0.4.1/runit/templates/404.html` & `runit_cli-0.4.2/runit/templates/404.html`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.1/runit/templates/multi/application.py` & `runit_cli-0.4.2/runit/templates/multi/application.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.1/runit/templates/python/application.py` & `runit_cli-0.4.2/runit/templates/python/application.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.1/runit/tools/php/loader.php` & `runit_cli-0.4.2/runit/tools/php/loader.php`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <?php
 /**
  * Description
  * @authors Amos Amissah (theonlyamos@gmail.com)
  * @date    2022-07-09 15:05:41
  * @version 1.0.0
  */
-require_once __DIR__ . '/manager.php';
-use Runit\Controller\DotEnvEnvironment;
+// require_once __DIR__ . '/manager.php';
+// use Runit\Controller\DotEnvEnvironment;
 
 try {
     if ($argc >= 2) {
         $filename = $argv[1];
         $filepath = dirname($filename);
-        (new DotEnvEnvironment)->load($filepath);
+        // (new DotEnvEnvironment)->load($filepath);
         include_once $filename;
         echo join(',', get_defined_functions()['user']);
     }
 } catch (Exception $error) {
     echo $error->getMessage();
 }
```

### Comparing `runit_cli-0.4.1/runit/tools/php/manager.php` & `runit_cli-0.4.2/runit/tools/php/manager.php`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.1/runit/tools/python/runner.py` & `runit_cli-0.4.2/runit/tools/python/runner.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import os
 import sys
 import inspect
-from dotenv import load_dotenv
 
 args = sys.argv
 functionArguments = None
 
 try:
     if len(args) >= 3:
         filename = args[1]
         functionname = args[2]
         filepath = os.path.split(filename)[0]
-        load_dotenv(os.path.join(filepath, '.env'))
+
         sys.path.append(filepath)
         module = __import__(str(inspect.getmodulename(filename)))
         method = [f[1] for f in inspect.getmembers(module, inspect.isfunction) if f[0] == functionname][0]
 
         if len(args) > 3:
             functionArguments = args[3]
```

### Comparing `runit_cli-0.4.1/runit_cli.egg-info/PKG-INFO` & `runit_cli-0.4.2/runit_cli.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runit-cli
-Version: 0.4.1
+Version: 0.4.2
 Summary: Develop serverless applications
 Author: Amos Amissah
 Author-email: theonlyamos@gmail.com
 Project-URL: Source, https://github.com/theonlyamos/runit
 Project-URL: Tracker, https://github.com/theonlyamos/runit/issues
 Keywords: python3 runit developer serverless architecture docker
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `runit_cli-0.4.1/runit_cli.egg-info/SOURCES.txt` & `runit_cli-0.4.2/runit_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.1/setup.py` & `runit_cli-0.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from importlib.metadata import entry_points
 from setuptools import setup, find_packages
 
-VERSION = '0.4.1'
+VERSION = '0.4.2'
 
 with open('README.md', 'rt') as file:
     LONG_DESCRIPTION = file.read()
 
 setup(
     name='runit-cli',
     version=VERSION,
```

### Comparing `runit_cli-0.4.1/tests/test_clone_project.py` & `runit_cli-0.4.2/tests/test_clone_project.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.1/tests/test_create_new_project.py` & `runit_cli-0.4.2/tests/test_create_new_project.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.1/tests/test_create_project_config.py` & `runit_cli-0.4.2/tests/test_create_project_config.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.1/tests/test_generate_function.py` & `runit_cli-0.4.2/tests/test_generate_function.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.1/tests/test_publish_project.py` & `runit_cli-0.4.2/tests/test_publish_project.py`

 * *Files identical despite different names*

### Comparing `runit_cli-0.4.1/tests/test_run_project.py` & `runit_cli-0.4.2/tests/test_run_project.py`

 * *Files identical despite different names*

