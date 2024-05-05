# Comparing `tmp/cybermarket_server-1.0.0.tar.gz` & `tmp/cybermarket_server-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybermarket_server-1.0.0.tar", last modified: Fri May  3 13:18:46 2024, max compression
+gzip compressed data, was "cybermarket_server-1.0.1.tar", last modified: Sun May  5 13:49:51 2024, max compression
```

## Comparing `cybermarket_server-1.0.0.tar` & `cybermarket_server-1.0.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 13:18:46.702857 cybermarket_server-1.0.0/
--rw-rw-rw-   0        0        0   157530 2024-05-03 12:37:30.000000 cybermarket_server-1.0.0/ERD_diagram.png
--rw-rw-rw-   0        0        0     1088 2024-05-03 12:57:38.000000 cybermarket_server-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      226 2024-05-02 23:09:35.000000 cybermarket_server-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3996 2024-05-03 13:18:46.698677 cybermarket_server-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2255 2024-05-03 12:13:57.000000 cybermarket_server-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 13:18:46.698677 cybermarket_server-1.0.0/cybermarket_server.egg-info/
--rw-rw-rw-   0        0        0     3996 2024-05-03 13:18:46.000000 cybermarket_server-1.0.0/cybermarket_server.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      997 2024-05-03 13:18:46.000000 cybermarket_server-1.0.0/cybermarket_server.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 13:18:46.000000 cybermarket_server-1.0.0/cybermarket_server.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-05-03 13:18:46.000000 cybermarket_server-1.0.0/cybermarket_server.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-03 13:18:46.000000 cybermarket_server-1.0.0/cybermarket_server.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-03 13:18:46.662000 cybermarket_server-1.0.0/docs/
--rw-rw-rw-   0        0        0      638 2024-05-01 14:17:13.000000 cybermarket_server-1.0.0/docs/Makefile
--rwxrwxrwx   0        0        0      804 2024-05-01 14:17:13.000000 cybermarket_server-1.0.0/docs/make.bat
-drwxrwxrwx   0        0        0        0 2024-05-03 13:18:46.669044 cybermarket_server-1.0.0/docs/source/
--rw-rw-rw-   0        0        0     2184 2024-05-02 23:44:07.000000 cybermarket_server-1.0.0/docs/source/conf.py
--rw-rw-rw-   0        0        0      485 2024-05-02 09:54:57.000000 cybermarket_server-1.0.0/docs/source/index.rst
--rw-rw-rw-   0        0        0       53 2024-05-02 13:34:04.000000 cybermarket_server-1.0.0/docs/source/modules.rst
--rw-rw-rw-   0        0        0     1180 2024-05-02 13:34:04.000000 cybermarket_server-1.0.0/docs/source/src.cybermarket_server.rst
--rw-rw-rw-   0        0        0      232 2024-05-02 13:34:04.000000 cybermarket_server-1.0.0/docs/source/src.rst
--rw-rw-rw-   0        0        0     3442 2024-05-03 10:02:46.000000 cybermarket_server-1.0.0/dodo.py
-drwxrwxrwx   0        0        0        0 2024-05-03 13:18:46.598754 cybermarket_server-1.0.0/locale/
-drwxrwxrwx   0        0        0        0 2024-05-03 13:18:46.598754 cybermarket_server-1.0.0/locale/ru_RU/
-drwxrwxrwx   0        0        0        0 2024-05-03 13:18:46.670931 cybermarket_server-1.0.0/locale/ru_RU/LC_MESSAGES/
--rw-rw-rw-   0        0        0     8793 2024-05-03 12:47:44.000000 cybermarket_server-1.0.0/locale/ru_RU/LC_MESSAGES/Russian.po
-drwxrwxrwx   0        0        0        0 2024-05-03 13:18:46.598754 cybermarket_server-1.0.0/locale/zh_CN/
-drwxrwxrwx   0        0        0        0 2024-05-03 13:18:46.671773 cybermarket_server-1.0.0/locale/zh_CN/LC_MESSAGES/
--rw-rw-rw-   0        0        0     7304 2024-05-03 12:47:44.000000 cybermarket_server-1.0.0/locale/zh_CN/LC_MESSAGES/Chinese.po
--rw-rw-rw-   0        0        0      810 2024-05-03 13:15:51.000000 cybermarket_server-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-03 13:18:46.702857 cybermarket_server-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      533 2024-05-03 12:55:34.000000 cybermarket_server-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-03 13:18:46.673432 cybermarket_server-1.0.0/src/
--rw-rw-rw-   0        0        0       30 2024-05-01 20:19:51.000000 cybermarket_server-1.0.0/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 13:18:46.686293 cybermarket_server-1.0.0/src/cybermarket_server/
--rw-rw-rw-   0        0        0       30 2024-05-01 20:19:51.000000 cybermarket_server-1.0.0/src/cybermarket_server/__init__.py
--rw-rw-rw-   0        0        0     3164 2024-05-02 22:57:42.000000 cybermarket_server-1.0.0/src/cybermarket_server/__main__.py
--rw-rw-rw-   0        0        0    28952 2024-05-02 22:57:52.000000 cybermarket_server-1.0.0/src/cybermarket_server/cmd_process.py
-drwxrwxrwx   0        0        0        0 2024-05-03 13:18:46.689212 cybermarket_server-1.0.0/src/cybermarket_server/database/
--rw-rw-rw-   0        0        0    32768 2024-05-03 12:47:44.000000 cybermarket_server-1.0.0/src/cybermarket_server/database/cybermarket.db
--rw-rw-rw-   0        0        0     2111 2024-05-02 22:58:01.000000 cybermarket_server-1.0.0/src/cybermarket_server/invitation.py
--rw-rw-rw-   0        0        0      786 2024-05-01 21:12:33.000000 cybermarket_server-1.0.0/src/cybermarket_server/lang.py
-drwxrwxrwx   0        0        0        0 2024-05-03 13:18:46.606969 cybermarket_server-1.0.0/src/cybermarket_server/locale/
-drwxrwxrwx   0        0        0        0 2024-05-03 13:18:46.606007 cybermarket_server-1.0.0/src/cybermarket_server/locale/ru_RU/
-drwxrwxrwx   0        0        0        0 2024-05-03 13:18:46.691234 cybermarket_server-1.0.0/src/cybermarket_server/locale/ru_RU/LC_MESSAGES/
--rw-rw-rw-   0        0        0     5078 2024-05-03 12:40:06.000000 cybermarket_server-1.0.0/src/cybermarket_server/locale/ru_RU/LC_MESSAGES/Russian.mo
-drwxrwxrwx   0        0        0        0 2024-05-03 13:18:46.606969 cybermarket_server-1.0.0/src/cybermarket_server/locale/zh_CN/
-drwxrwxrwx   0        0        0        0 2024-05-03 13:18:46.692251 cybermarket_server-1.0.0/src/cybermarket_server/locale/zh_CN/LC_MESSAGES/
--rw-rw-rw-   0        0        0     3594 2024-05-03 12:40:05.000000 cybermarket_server-1.0.0/src/cybermarket_server/locale/zh_CN/LC_MESSAGES/Chinese.mo
--rw-rw-rw-   0        0        0    17026 2024-05-03 12:59:02.000000 cybermarket_server-1.0.0/src/cybermarket_server/model.py
--rw-rw-rw-   0        0        0     1366 2024-05-02 14:00:38.000000 cybermarket_server-1.0.0/src/cybermarket_server/setting.py
-drwxrwxrwx   0        0        0        0 2024-05-03 13:18:46.696662 cybermarket_server-1.0.0/tests/
--rw-rw-rw-   0        0        0        0 2024-05-01 20:19:43.000000 cybermarket_server-1.0.0/tests/__init__.py
--rw-rw-rw-   0        0        0       52 2024-04-30 11:52:47.000000 cybermarket_server-1.0.0/tests/setting_unittest.py
--rw-rw-rw-   0        0        0    32368 2024-05-02 13:21:42.000000 cybermarket_server-1.0.0/tests/unit_test.py
+drwxrwxrwx   0        0        0        0 2024-05-05 13:49:51.153278 cybermarket_server-1.0.1/
+-rw-rw-rw-   0        0        0   157530 2024-05-03 12:37:30.000000 cybermarket_server-1.0.1/ERD_diagram.png
+-rw-rw-rw-   0        0        0     1088 2024-05-03 12:57:38.000000 cybermarket_server-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      226 2024-05-02 23:09:35.000000 cybermarket_server-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3996 2024-05-05 13:49:51.152104 cybermarket_server-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2255 2024-05-03 12:13:57.000000 cybermarket_server-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 13:49:51.150393 cybermarket_server-1.0.1/cybermarket_server.egg-info/
+-rw-rw-rw-   0        0        0     3996 2024-05-05 13:49:50.000000 cybermarket_server-1.0.1/cybermarket_server.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      997 2024-05-05 13:49:50.000000 cybermarket_server-1.0.1/cybermarket_server.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 13:49:50.000000 cybermarket_server-1.0.1/cybermarket_server.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-05 13:49:50.000000 cybermarket_server-1.0.1/cybermarket_server.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-05 13:49:50.000000 cybermarket_server-1.0.1/cybermarket_server.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-05 13:49:50.847131 cybermarket_server-1.0.1/docs/
+-rw-rw-rw-   0        0        0      638 2024-05-01 14:17:13.000000 cybermarket_server-1.0.1/docs/Makefile
+-rwxrwxrwx   0        0        0      804 2024-05-01 14:17:13.000000 cybermarket_server-1.0.1/docs/make.bat
+drwxrwxrwx   0        0        0        0 2024-05-05 13:49:50.910258 cybermarket_server-1.0.1/docs/source/
+-rw-rw-rw-   0        0        0     2184 2024-05-05 08:43:35.000000 cybermarket_server-1.0.1/docs/source/conf.py
+-rw-rw-rw-   0        0        0      485 2024-05-02 09:54:57.000000 cybermarket_server-1.0.1/docs/source/index.rst
+-rw-rw-rw-   0        0        0       53 2024-05-02 13:34:04.000000 cybermarket_server-1.0.1/docs/source/modules.rst
+-rw-rw-rw-   0        0        0     1180 2024-05-02 13:34:04.000000 cybermarket_server-1.0.1/docs/source/src.cybermarket_server.rst
+-rw-rw-rw-   0        0        0      232 2024-05-02 13:34:04.000000 cybermarket_server-1.0.1/docs/source/src.rst
+-rw-rw-rw-   0        0        0     3442 2024-05-03 10:02:46.000000 cybermarket_server-1.0.1/dodo.py
+drwxrwxrwx   0        0        0        0 2024-05-05 13:49:50.719368 cybermarket_server-1.0.1/locale/
+drwxrwxrwx   0        0        0        0 2024-05-05 13:49:50.717991 cybermarket_server-1.0.1/locale/ru_RU/
+drwxrwxrwx   0        0        0        0 2024-05-05 13:49:50.930279 cybermarket_server-1.0.1/locale/ru_RU/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     8572 2024-05-04 22:12:25.000000 cybermarket_server-1.0.1/locale/ru_RU/LC_MESSAGES/Russian.po
+drwxrwxrwx   0        0        0        0 2024-05-05 13:49:50.720226 cybermarket_server-1.0.1/locale/zh_CN/
+drwxrwxrwx   0        0        0        0 2024-05-05 13:49:50.940543 cybermarket_server-1.0.1/locale/zh_CN/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     7087 2024-05-04 22:12:25.000000 cybermarket_server-1.0.1/locale/zh_CN/LC_MESSAGES/Chinese.po
+-rw-rw-rw-   0        0        0      810 2024-05-05 13:48:59.000000 cybermarket_server-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-05 13:49:51.154242 cybermarket_server-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      533 2024-05-03 12:55:34.000000 cybermarket_server-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 13:49:50.950800 cybermarket_server-1.0.1/src/
+-rw-rw-rw-   0        0        0       30 2024-05-01 20:19:51.000000 cybermarket_server-1.0.1/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 13:49:51.081451 cybermarket_server-1.0.1/src/cybermarket_server/
+-rw-rw-rw-   0        0        0       30 2024-05-01 20:19:51.000000 cybermarket_server-1.0.1/src/cybermarket_server/__init__.py
+-rw-rw-rw-   0        0        0     3164 2024-05-04 15:47:19.000000 cybermarket_server-1.0.1/src/cybermarket_server/__main__.py
+-rw-rw-rw-   0        0        0    28969 2024-05-05 08:34:16.000000 cybermarket_server-1.0.1/src/cybermarket_server/cmd_process.py
+drwxrwxrwx   0        0        0        0 2024-05-05 13:49:51.085661 cybermarket_server-1.0.1/src/cybermarket_server/database/
+-rw-rw-rw-   0        0        0    32768 2024-05-03 12:47:44.000000 cybermarket_server-1.0.1/src/cybermarket_server/database/cybermarket.db
+-rw-rw-rw-   0        0        0     2111 2024-05-02 22:58:01.000000 cybermarket_server-1.0.1/src/cybermarket_server/invitation.py
+-rw-rw-rw-   0        0        0      786 2024-05-01 21:12:33.000000 cybermarket_server-1.0.1/src/cybermarket_server/lang.py
+drwxrwxrwx   0        0        0        0 2024-05-05 13:49:50.725141 cybermarket_server-1.0.1/src/cybermarket_server/locale/
+drwxrwxrwx   0        0        0        0 2024-05-05 13:49:50.724218 cybermarket_server-1.0.1/src/cybermarket_server/locale/ru_RU/
+drwxrwxrwx   0        0        0        0 2024-05-05 13:49:51.094999 cybermarket_server-1.0.1/src/cybermarket_server/locale/ru_RU/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     5078 2024-05-04 22:12:27.000000 cybermarket_server-1.0.1/src/cybermarket_server/locale/ru_RU/LC_MESSAGES/Russian.mo
+drwxrwxrwx   0        0        0        0 2024-05-05 13:49:50.725141 cybermarket_server-1.0.1/src/cybermarket_server/locale/zh_CN/
+drwxrwxrwx   0        0        0        0 2024-05-05 13:49:51.111100 cybermarket_server-1.0.1/src/cybermarket_server/locale/zh_CN/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     3594 2024-05-04 22:12:26.000000 cybermarket_server-1.0.1/src/cybermarket_server/locale/zh_CN/LC_MESSAGES/Chinese.mo
+-rw-rw-rw-   0        0        0    17058 2024-05-05 08:38:58.000000 cybermarket_server-1.0.1/src/cybermarket_server/model.py
+-rw-rw-rw-   0        0        0     1366 2024-05-05 08:27:58.000000 cybermarket_server-1.0.1/src/cybermarket_server/setting.py
+drwxrwxrwx   0        0        0        0 2024-05-05 13:49:51.147443 cybermarket_server-1.0.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-01 20:19:43.000000 cybermarket_server-1.0.1/tests/__init__.py
+-rw-rw-rw-   0        0        0       52 2024-04-30 11:52:47.000000 cybermarket_server-1.0.1/tests/setting_unittest.py
+-rw-rw-rw-   0        0        0    32403 2024-05-05 08:42:04.000000 cybermarket_server-1.0.1/tests/unit_test.py
```

### Comparing `cybermarket_server-1.0.0/ERD_diagram.png` & `cybermarket_server-1.0.1/ERD_diagram.png`

 * *Files identical despite different names*

### Comparing `cybermarket_server-1.0.0/LICENSE` & `cybermarket_server-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cybermarket_server-1.0.0/PKG-INFO` & `cybermarket_server-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybermarket_server
-Version: 1.0.0
+Version: 1.0.1
 Summary: The server of the online network market accepts login, listing, purchase, etc. requests sent by the client.
 Author-email: Hailin Liu <0123liuhailin@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Hailin Liu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `cybermarket_server-1.0.0/README.md` & `cybermarket_server-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cybermarket_server-1.0.0/cybermarket_server.egg-info/PKG-INFO` & `cybermarket_server-1.0.1/cybermarket_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybermarket_server
-Version: 1.0.0
+Version: 1.0.1
 Summary: The server of the online network market accepts login, listing, purchase, etc. requests sent by the client.
 Author-email: Hailin Liu <0123liuhailin@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Hailin Liu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `cybermarket_server-1.0.0/cybermarket_server.egg-info/SOURCES.txt` & `cybermarket_server-1.0.1/cybermarket_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cybermarket_server-1.0.0/docs/Makefile` & `cybermarket_server-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cybermarket_server-1.0.0/docs/make.bat` & `cybermarket_server-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cybermarket_server-1.0.0/docs/source/conf.py` & `cybermarket_server-1.0.1/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'cybermarket-server'
 copyright = '2024, Hailin Liu'
 author = 'Hailin Liu'
 
 # The full version, including alpha/beta/rc tags
-release = '1.0.0'
+release = '1.0.1'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `cybermarket_server-1.0.0/docs/source/src.cybermarket_server.rst` & `cybermarket_server-1.0.1/docs/source/src.cybermarket_server.rst`

 * *Files identical despite different names*

### Comparing `cybermarket_server-1.0.0/dodo.py` & `cybermarket_server-1.0.1/dodo.py`

 * *Files identical despite different names*

### Comparing `cybermarket_server-1.0.0/locale/ru_RU/LC_MESSAGES/Russian.po` & `cybermarket_server-1.0.1/locale/ru_RU/LC_MESSAGES/Russian.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,221 +1,221 @@
-# Russian (Russia) translations for .
-# Copyright (C) 2024 ORGANIZATION
-# This file is distributed under the same license as the  project.
-# FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
-#
-msgid ""
-msgstr ""
-"Project-Id-Version:  1.0.0\n"
-"Report-Msgid-Bugs-To: 0123liuhailin@gmail.com\n"
-"POT-Creation-Date: 2024-05-02 16:18+0300\n"
-"PO-Revision-Date: 2024-04-27 16:07+0300\n"
-"Last-Translator: @lhl4971 <github.com/lhl4971/>\n"
-"Language: ru_RU\n"
-"Language-Team: ru_RU <github.com/pyCybermarket2024>\n"
-"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=utf-8\n"
-"Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
-
-#: src/cybermarket_server/cmd_process.py:27
-msgid "This username is occupied"
-msgstr "Пользовательский логин занят"
-
-#: src/cybermarket_server/cmd_process.py:54
-msgid "Username has been set"
-msgstr "Пользовательский логин установлен"
-
-#: src/cybermarket_server/cmd_process.py:58
-#: src/cybermarket_server/cmd_process.py:83
-#: src/cybermarket_server/cmd_process.py:114
-#: src/cybermarket_server/cmd_process.py:152
-#: src/cybermarket_server/cmd_process.py:177
-#: src/cybermarket_server/cmd_process.py:213
-#: src/cybermarket_server/cmd_process.py:245
-#: src/cybermarket_server/cmd_process.py:273
-#: src/cybermarket_server/cmd_process.py:298
-#: src/cybermarket_server/cmd_process.py:328
-#: src/cybermarket_server/cmd_process.py:410
-#: src/cybermarket_server/cmd_process.py:490
-#: src/cybermarket_server/cmd_process.py:515
-#: src/cybermarket_server/cmd_process.py:540
-#: src/cybermarket_server/cmd_process.py:565
-#: src/cybermarket_server/cmd_process.py:591
-#: src/cybermarket_server/cmd_process.py:622
-#: src/cybermarket_server/cmd_process.py:649
-#: src/cybermarket_server/cmd_process.py:674
-#: src/cybermarket_server/cmd_process.py:708
-#: src/cybermarket_server/cmd_process.py:733
-msgid "You have not logged in or your login has timed out"
-msgstr "Вы не вошли в систему или время входа в систему истекло"
-
-#: src/cybermarket_server/cmd_process.py:79
-#: src/cybermarket_server/cmd_process.py:561
-msgid "Email has been set"
-msgstr "Электронная почта установлена"
-
-#: src/cybermarket_server/cmd_process.py:106
-#: src/cybermarket_server/cmd_process.py:614
-msgid "New password has been set"
-msgstr "Новый пароль установлен"
-
-#: src/cybermarket_server/cmd_process.py:110
-#: src/cybermarket_server/cmd_process.py:148
-msgid "The password of the user is incorrect"
-msgstr "Пароль пользователя неверен"
-
-#: src/cybermarket_server/cmd_process.py:138
-msgid "The user has been logged in, please do not log in again"
-msgstr "Пользователь уже вошел, пожалуйста, не входите снова"
-
-#: src/cybermarket_server/cmd_process.py:144
-msgid "This user is logged in"
-msgstr "Пользователь вошел"
-
-#: src/cybermarket_server/cmd_process.py:173
-#: src/cybermarket_server/cmd_process.py:511
-msgid "You have successfully logged out"
-msgstr "Вы успешно вышли из системы"
-
-#: src/cybermarket_server/cmd_process.py:200
-msgid "The quantity of added products should be a positive integer"
-msgstr "Количество добавленных товаров должно быть положительным целым числом"
-
-#: src/cybermarket_server/cmd_process.py:204
-msgid "The product you are trying to add cannot be found"
-msgstr "Товар, который вы пытаетесь добавить, не найден."
-
-#: src/cybermarket_server/cmd_process.py:209
-msgid "This product has been added to the shopping cart"
-msgstr "Товар добавлен в корзину"
-
-#: src/cybermarket_server/cmd_process.py:236
-msgid "This product is not in your shopping cart"
-msgstr "Этого товара нет в вашей корзине"
-
-#: src/cybermarket_server/cmd_process.py:241
-msgid "This product has been removed from the shopping cart"
-msgstr "Товар был удален из корзины"
-
-#: src/cybermarket_server/cmd_process.py:266
-msgid "Obtained order list"
-msgstr "Список заказов получен"
-
-#: src/cybermarket_server/cmd_process.py:268
-#: src/cybermarket_server/cmd_process.py:354
-#: src/cybermarket_server/cmd_process.py:379
-msgid "storename"
-msgstr "Название магазина"
-
-#: src/cybermarket_server/cmd_process.py:268
-#: src/cybermarket_server/cmd_process.py:379
-msgid "productname"
-msgstr "Название товара"
-
-#: src/cybermarket_server/cmd_process.py:269
-#: src/cybermarket_server/cmd_process.py:380
-msgid "price"
-msgstr "Цена"
-
-#: src/cybermarket_server/cmd_process.py:269
-msgid "quantity"
-msgstr "Количество"
-
-#: src/cybermarket_server/cmd_process.py:294
-msgid "Order price obtained"
-msgstr "Стоимость заказа получена"
-
-#: src/cybermarket_server/cmd_process.py:320
-msgid "Order has been checked out"
-msgstr "Заказ оплачен"
-
-#: src/cybermarket_server/cmd_process.py:354
-#: src/cybermarket_server/cmd_process.py:380
-msgid "description"
-msgstr "Описание"
-
-#: src/cybermarket_server/cmd_process.py:355
-msgid "email"
-msgstr "Электронная почта"
-
-#: src/cybermarket_server/cmd_process.py:377
-msgid "Product list has been obtained"
-msgstr "Список товаров получен"
-
-#: src/cybermarket_server/cmd_process.py:379
-msgid "product_id"
-msgstr "Код товара"
-
-#: src/cybermarket_server/cmd_process.py:380
-msgid "stock"
-msgstr "в наличии"
-
-#: src/cybermarket_server/cmd_process.py:384
-msgid "No store with this name found"
-msgstr "Магазин с таким названием не найден"
-
-#: src/cybermarket_server/cmd_process.py:406
-msgid "Invitation code has been generated"
-msgstr "Пригласительный код создан"
-
-#: src/cybermarket_server/cmd_process.py:435
-msgid "This storename is occupied"
-msgstr "Название магазина занято"
-
-#: src/cybermarket_server/cmd_process.py:450
-msgid ""
-"Your invitation code cannot be verified. This invitation code may be "
-"wrong or has already been used. Please contact other merchants to request"
-" the invitation code."
-msgstr ""
-"Ваш код приглашения не может быть проверен. Этот код приглашения может "
-"быть неверным или уже использовался. Пожалуйста, свяжитесь с другими "
-"продавцами, чтобы запросить код приглашения."
-
-#: src/cybermarket_server/cmd_process.py:476
-msgid "The merchant has been logged in, please do not log in again"
-msgstr "Продавец уже вошел, пожалуйста, не входите снова"
-
-#: src/cybermarket_server/cmd_process.py:482
-msgid "This merchant is logged in"
-msgstr "Продавец вошел в систему"
-
-#: src/cybermarket_server/cmd_process.py:486
-#: src/cybermarket_server/cmd_process.py:618
-msgid "The password of the merchant is incorrect"
-msgstr "Пароль продавца неверен"
-
-#: src/cybermarket_server/cmd_process.py:536
-msgid "Storename has been set"
-msgstr "Название магазина установлено"
-
-#: src/cybermarket_server/cmd_process.py:587
-msgid "Description has been set"
-msgstr "Описание установлено"
-
-#: src/cybermarket_server/cmd_process.py:645
-msgid "This product has been added to the product list"
-msgstr "Продукт добавлен в список продуктов"
-
-#: src/cybermarket_server/cmd_process.py:670
-msgid "This product has been deleted from the product list"
-msgstr "Товар удален из списка товаров"
-
-#: src/cybermarket_server/cmd_process.py:700
-msgid "This product has been restock"
-msgstr "Этот продукт был пополнен"
-
-#: src/cybermarket_server/cmd_process.py:704
-msgid "You are restocking an item that is not from this store"
-msgstr "Вы пополняете товар, которого нет в этом магазине"
-
-#: src/cybermarket_server/cmd_process.py:729
-msgid "Your total profit has been obtained"
-msgstr "Ваша общая прибыль получена"
-
-#: src/cybermarket_server/cmd_process.py:790
-msgid "You are trying to call an undefined method"
-msgstr "Вы пытаетесь вызвать неопределенный метод"
-
+# Russian (Russia) translations for .
+# Copyright (C) 2024 ORGANIZATION
+# This file is distributed under the same license as the  project.
+# FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
+#
+msgid ""
+msgstr ""
+"Project-Id-Version:  1.0.0\n"
+"Report-Msgid-Bugs-To: 0123liuhailin@gmail.com\n"
+"POT-Creation-Date: 2024-05-05 01:12+0300\n"
+"PO-Revision-Date: 2024-04-27 16:07+0300\n"
+"Last-Translator: @lhl4971 <github.com/lhl4971/>\n"
+"Language: ru_RU\n"
+"Language-Team: ru_RU <github.com/pyCybermarket2024>\n"
+"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
+"MIME-Version: 1.0\n"
+"Content-Type: text/plain; charset=utf-8\n"
+"Content-Transfer-Encoding: 8bit\n"
+"Generated-By: Babel 2.11.0\n"
+
+#: src/cybermarket_server/cmd_process.py:27
+msgid "This username is occupied"
+msgstr "Пользовательский логин занят"
+
+#: src/cybermarket_server/cmd_process.py:54
+msgid "Username has been set"
+msgstr "Пользовательский логин установлен"
+
+#: src/cybermarket_server/cmd_process.py:58
+#: src/cybermarket_server/cmd_process.py:83
+#: src/cybermarket_server/cmd_process.py:114
+#: src/cybermarket_server/cmd_process.py:152
+#: src/cybermarket_server/cmd_process.py:177
+#: src/cybermarket_server/cmd_process.py:213
+#: src/cybermarket_server/cmd_process.py:245
+#: src/cybermarket_server/cmd_process.py:273
+#: src/cybermarket_server/cmd_process.py:298
+#: src/cybermarket_server/cmd_process.py:328
+#: src/cybermarket_server/cmd_process.py:410
+#: src/cybermarket_server/cmd_process.py:490
+#: src/cybermarket_server/cmd_process.py:515
+#: src/cybermarket_server/cmd_process.py:540
+#: src/cybermarket_server/cmd_process.py:565
+#: src/cybermarket_server/cmd_process.py:591
+#: src/cybermarket_server/cmd_process.py:622
+#: src/cybermarket_server/cmd_process.py:649
+#: src/cybermarket_server/cmd_process.py:674
+#: src/cybermarket_server/cmd_process.py:708
+#: src/cybermarket_server/cmd_process.py:733
+msgid "You have not logged in or your login has timed out"
+msgstr "Вы не вошли в систему или время входа в систему истекло"
+
+#: src/cybermarket_server/cmd_process.py:79
+#: src/cybermarket_server/cmd_process.py:561
+msgid "Email has been set"
+msgstr "Электронная почта установлена"
+
+#: src/cybermarket_server/cmd_process.py:106
+#: src/cybermarket_server/cmd_process.py:614
+msgid "New password has been set"
+msgstr "Новый пароль установлен"
+
+#: src/cybermarket_server/cmd_process.py:110
+#: src/cybermarket_server/cmd_process.py:148
+msgid "The password of the user is incorrect"
+msgstr "Пароль пользователя неверен"
+
+#: src/cybermarket_server/cmd_process.py:138
+msgid "The user has been logged in, please do not log in again"
+msgstr "Пользователь уже вошел, пожалуйста, не входите снова"
+
+#: src/cybermarket_server/cmd_process.py:144
+msgid "This user is logged in"
+msgstr "Пользователь вошел"
+
+#: src/cybermarket_server/cmd_process.py:173
+#: src/cybermarket_server/cmd_process.py:511
+msgid "You have successfully logged out"
+msgstr "Вы успешно вышли из системы"
+
+#: src/cybermarket_server/cmd_process.py:200
+msgid "The quantity of added products should be a positive integer"
+msgstr "Количество добавленных товаров должно быть положительным целым числом"
+
+#: src/cybermarket_server/cmd_process.py:204
+msgid "The product you are trying to add cannot be found"
+msgstr "Товар, который вы пытаетесь добавить, не найден."
+
+#: src/cybermarket_server/cmd_process.py:209
+msgid "This product has been added to the shopping cart"
+msgstr "Товар добавлен в корзину"
+
+#: src/cybermarket_server/cmd_process.py:236
+msgid "This product is not in your shopping cart"
+msgstr "Этого товара нет в вашей корзине"
+
+#: src/cybermarket_server/cmd_process.py:241
+msgid "This product has been removed from the shopping cart"
+msgstr "Товар был удален из корзины"
+
+#: src/cybermarket_server/cmd_process.py:266
+msgid "Obtained order list"
+msgstr "Список заказов получен"
+
+#: src/cybermarket_server/cmd_process.py:268
+#: src/cybermarket_server/cmd_process.py:354
+#: src/cybermarket_server/cmd_process.py:379
+msgid "storename"
+msgstr "Название магазина"
+
+#: src/cybermarket_server/cmd_process.py:268
+#: src/cybermarket_server/cmd_process.py:379
+msgid "productname"
+msgstr "Название товара"
+
+#: src/cybermarket_server/cmd_process.py:269
+#: src/cybermarket_server/cmd_process.py:380
+msgid "price"
+msgstr "Цена"
+
+#: src/cybermarket_server/cmd_process.py:269
+msgid "quantity"
+msgstr "Количество"
+
+#: src/cybermarket_server/cmd_process.py:294
+msgid "Order price obtained"
+msgstr "Стоимость заказа получена"
+
+#: src/cybermarket_server/cmd_process.py:320
+msgid "Order has been checked out"
+msgstr "Заказ оплачен"
+
+#: src/cybermarket_server/cmd_process.py:354
+#: src/cybermarket_server/cmd_process.py:380
+msgid "description"
+msgstr "Описание"
+
+#: src/cybermarket_server/cmd_process.py:355
+msgid "email"
+msgstr "Электронная почта"
+
+#: src/cybermarket_server/cmd_process.py:377
+msgid "Product list has been obtained"
+msgstr "Список товаров получен"
+
+#: src/cybermarket_server/cmd_process.py:379
+msgid "product_id"
+msgstr "Код товара"
+
+#: src/cybermarket_server/cmd_process.py:380
+msgid "stock"
+msgstr "в наличии"
+
+#: src/cybermarket_server/cmd_process.py:384
+msgid "No store with this name found"
+msgstr "Магазин с таким названием не найден"
+
+#: src/cybermarket_server/cmd_process.py:406
+msgid "Invitation code has been generated"
+msgstr "Пригласительный код создан"
+
+#: src/cybermarket_server/cmd_process.py:435
+msgid "This storename is occupied"
+msgstr "Название магазина занято"
+
+#: src/cybermarket_server/cmd_process.py:450
+msgid ""
+"Your invitation code cannot be verified. This invitation code may be "
+"wrong or has already been used. Please contact other merchants to request"
+" the invitation code."
+msgstr ""
+"Ваш код приглашения не может быть проверен. Этот код приглашения может "
+"быть неверным или уже использовался. Пожалуйста, свяжитесь с другими "
+"продавцами, чтобы запросить код приглашения."
+
+#: src/cybermarket_server/cmd_process.py:476
+msgid "The merchant has been logged in, please do not log in again"
+msgstr "Продавец уже вошел, пожалуйста, не входите снова"
+
+#: src/cybermarket_server/cmd_process.py:482
+msgid "This merchant is logged in"
+msgstr "Продавец вошел в систему"
+
+#: src/cybermarket_server/cmd_process.py:486
+#: src/cybermarket_server/cmd_process.py:618
+msgid "The password of the merchant is incorrect"
+msgstr "Пароль продавца неверен"
+
+#: src/cybermarket_server/cmd_process.py:536
+msgid "Storename has been set"
+msgstr "Название магазина установлено"
+
+#: src/cybermarket_server/cmd_process.py:587
+msgid "Description has been set"
+msgstr "Описание установлено"
+
+#: src/cybermarket_server/cmd_process.py:645
+msgid "This product has been added to the product list"
+msgstr "Продукт добавлен в список продуктов"
+
+#: src/cybermarket_server/cmd_process.py:670
+msgid "This product has been deleted from the product list"
+msgstr "Товар удален из списка товаров"
+
+#: src/cybermarket_server/cmd_process.py:700
+msgid "This product has been restock"
+msgstr "Этот продукт был пополнен"
+
+#: src/cybermarket_server/cmd_process.py:704
+msgid "You are restocking an item that is not from this store"
+msgstr "Вы пополняете товар, которого нет в этом магазине"
+
+#: src/cybermarket_server/cmd_process.py:729
+msgid "Your total profit has been obtained"
+msgstr "Ваша общая прибыль получена"
+
+#: src/cybermarket_server/cmd_process.py:790
+msgid "You are trying to call an undefined method"
+msgstr "Вы пытаетесь вызвать неопределенный метод"
+
```

### Comparing `cybermarket_server-1.0.0/locale/zh_CN/LC_MESSAGES/Chinese.po` & `cybermarket_server-1.0.1/locale/zh_CN/LC_MESSAGES/Chinese.po`

 * *Files 18% similar despite different names*

```diff
@@ -1,217 +1,217 @@
-# Chinese (Simplified, China) translations for .
-# Copyright (C) 2024 ORGANIZATION
-# This file is distributed under the same license as the  project.
-# FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
-#
-msgid ""
-msgstr ""
-"Project-Id-Version:  1.0.0\n"
-"Report-Msgid-Bugs-To: 0123liuhailin@gmail.com\n"
-"POT-Creation-Date: 2024-05-02 16:18+0300\n"
-"PO-Revision-Date: 2024-04-27 15:54+0300\n"
-"Last-Translator: @lhl4971 <github.com/lhl4971/>\n"
-"Language: zh_Hans_CN\n"
-"Language-Team: ru_RU <github.com/pyCybermarket2024>\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=utf-8\n"
-"Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
-
-#: src/cybermarket_server/cmd_process.py:27
-msgid "This username is occupied"
-msgstr "该用户名已被占用"
-
-#: src/cybermarket_server/cmd_process.py:54
-msgid "Username has been set"
-msgstr "用户名已设置"
-
-#: src/cybermarket_server/cmd_process.py:58
-#: src/cybermarket_server/cmd_process.py:83
-#: src/cybermarket_server/cmd_process.py:114
-#: src/cybermarket_server/cmd_process.py:152
-#: src/cybermarket_server/cmd_process.py:177
-#: src/cybermarket_server/cmd_process.py:213
-#: src/cybermarket_server/cmd_process.py:245
-#: src/cybermarket_server/cmd_process.py:273
-#: src/cybermarket_server/cmd_process.py:298
-#: src/cybermarket_server/cmd_process.py:328
-#: src/cybermarket_server/cmd_process.py:410
-#: src/cybermarket_server/cmd_process.py:490
-#: src/cybermarket_server/cmd_process.py:515
-#: src/cybermarket_server/cmd_process.py:540
-#: src/cybermarket_server/cmd_process.py:565
-#: src/cybermarket_server/cmd_process.py:591
-#: src/cybermarket_server/cmd_process.py:622
-#: src/cybermarket_server/cmd_process.py:649
-#: src/cybermarket_server/cmd_process.py:674
-#: src/cybermarket_server/cmd_process.py:708
-#: src/cybermarket_server/cmd_process.py:733
-msgid "You have not logged in or your login has timed out"
-msgstr "您尚未登录或登录超时"
-
-#: src/cybermarket_server/cmd_process.py:79
-#: src/cybermarket_server/cmd_process.py:561
-msgid "Email has been set"
-msgstr "邮箱已设置"
-
-#: src/cybermarket_server/cmd_process.py:106
-#: src/cybermarket_server/cmd_process.py:614
-msgid "New password has been set"
-msgstr "新密码已设置"
-
-#: src/cybermarket_server/cmd_process.py:110
-#: src/cybermarket_server/cmd_process.py:148
-msgid "The password of the user is incorrect"
-msgstr "用户密码不正确"
-
-#: src/cybermarket_server/cmd_process.py:138
-msgid "The user has been logged in, please do not log in again"
-msgstr "该用户已登录，请勿再次登录"
-
-#: src/cybermarket_server/cmd_process.py:144
-msgid "This user is logged in"
-msgstr "用户已登录"
-
-#: src/cybermarket_server/cmd_process.py:173
-#: src/cybermarket_server/cmd_process.py:511
-msgid "You have successfully logged out"
-msgstr "您已成功退出"
-
-#: src/cybermarket_server/cmd_process.py:200
-msgid "The quantity of added products should be a positive integer"
-msgstr "添加的产品数量应为正整数"
-
-#: src/cybermarket_server/cmd_process.py:204
-msgid "The product you are trying to add cannot be found"
-msgstr "找不到您尝试添加的产品"
-
-#: src/cybermarket_server/cmd_process.py:209
-msgid "This product has been added to the shopping cart"
-msgstr "该产品已添加至购物车"
-
-#: src/cybermarket_server/cmd_process.py:236
-msgid "This product is not in your shopping cart"
-msgstr "该产品不在您的购物车中"
-
-#: src/cybermarket_server/cmd_process.py:241
-msgid "This product has been removed from the shopping cart"
-msgstr "该产品已从购物车中删除"
-
-#: src/cybermarket_server/cmd_process.py:266
-msgid "Obtained order list"
-msgstr "已获取订单列表"
-
-#: src/cybermarket_server/cmd_process.py:268
-#: src/cybermarket_server/cmd_process.py:354
-#: src/cybermarket_server/cmd_process.py:379
-msgid "storename"
-msgstr "店铺名称"
-
-#: src/cybermarket_server/cmd_process.py:268
-#: src/cybermarket_server/cmd_process.py:379
-msgid "productname"
-msgstr "产品名称"
-
-#: src/cybermarket_server/cmd_process.py:269
-#: src/cybermarket_server/cmd_process.py:380
-msgid "price"
-msgstr "价格"
-
-#: src/cybermarket_server/cmd_process.py:269
-msgid "quantity"
-msgstr "数量"
-
-#: src/cybermarket_server/cmd_process.py:294
-msgid "Order price obtained"
-msgstr "订单价格已获取"
-
-#: src/cybermarket_server/cmd_process.py:320
-msgid "Order has been checked out"
-msgstr "订单已结账"
-
-#: src/cybermarket_server/cmd_process.py:354
-#: src/cybermarket_server/cmd_process.py:380
-msgid "description"
-msgstr "描述"
-
-#: src/cybermarket_server/cmd_process.py:355
-msgid "email"
-msgstr "电子邮件"
-
-#: src/cybermarket_server/cmd_process.py:377
-msgid "Product list has been obtained"
-msgstr "已获取产品清单"
-
-#: src/cybermarket_server/cmd_process.py:379
-msgid "product_id"
-msgstr "产品编号"
-
-#: src/cybermarket_server/cmd_process.py:380
-msgid "stock"
-msgstr "库存数量"
-
-#: src/cybermarket_server/cmd_process.py:384
-msgid "No store with this name found"
-msgstr "未找到该名称的商店"
-
-#: src/cybermarket_server/cmd_process.py:406
-msgid "Invitation code has been generated"
-msgstr "邀请码已生成"
-
-#: src/cybermarket_server/cmd_process.py:435
-msgid "This storename is occupied"
-msgstr "该店名已被占用"
-
-#: src/cybermarket_server/cmd_process.py:450
-msgid ""
-"Your invitation code cannot be verified. This invitation code may be "
-"wrong or has already been used. Please contact other merchants to request"
-" the invitation code."
-msgstr "无法验证您的邀请码。 该邀请码可能有误或已被使用。 请联系其他商户索取邀请码。"
-
-#: src/cybermarket_server/cmd_process.py:476
-msgid "The merchant has been logged in, please do not log in again"
-msgstr "商户已登录，请勿再次登录"
-
-#: src/cybermarket_server/cmd_process.py:482
-msgid "This merchant is logged in"
-msgstr "该商户已登录"
-
-#: src/cybermarket_server/cmd_process.py:486
-#: src/cybermarket_server/cmd_process.py:618
-msgid "The password of the merchant is incorrect"
-msgstr "商户密码不正确"
-
-#: src/cybermarket_server/cmd_process.py:536
-msgid "Storename has been set"
-msgstr "店铺名称已设定"
-
-#: src/cybermarket_server/cmd_process.py:587
-msgid "Description has been set"
-msgstr "描述已设定"
-
-#: src/cybermarket_server/cmd_process.py:645
-msgid "This product has been added to the product list"
-msgstr "该产品已添加到产品列表中"
-
-#: src/cybermarket_server/cmd_process.py:670
-msgid "This product has been deleted from the product list"
-msgstr "该产品已从产品列表中删除"
-
-#: src/cybermarket_server/cmd_process.py:700
-msgid "This product has been restock"
-msgstr "该产品已补货"
-
-#: src/cybermarket_server/cmd_process.py:704
-msgid "You are restocking an item that is not from this store"
-msgstr "您正在补货的商品不是来自该商店"
-
-#: src/cybermarket_server/cmd_process.py:729
-msgid "Your total profit has been obtained"
-msgstr "您的总利润已获取"
-
-#: src/cybermarket_server/cmd_process.py:790
-msgid "You are trying to call an undefined method"
-msgstr "您正在尝试调用未定义的方法"
-
+# Chinese (Simplified, China) translations for .
+# Copyright (C) 2024 ORGANIZATION
+# This file is distributed under the same license as the  project.
+# FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
+#
+msgid ""
+msgstr ""
+"Project-Id-Version:  1.0.0\n"
+"Report-Msgid-Bugs-To: 0123liuhailin@gmail.com\n"
+"POT-Creation-Date: 2024-05-05 01:12+0300\n"
+"PO-Revision-Date: 2024-04-27 15:54+0300\n"
+"Last-Translator: @lhl4971 <github.com/lhl4971/>\n"
+"Language: zh_Hans_CN\n"
+"Language-Team: ru_RU <github.com/pyCybermarket2024>\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+"MIME-Version: 1.0\n"
+"Content-Type: text/plain; charset=utf-8\n"
+"Content-Transfer-Encoding: 8bit\n"
+"Generated-By: Babel 2.11.0\n"
+
+#: src/cybermarket_server/cmd_process.py:27
+msgid "This username is occupied"
+msgstr "该用户名已被占用"
+
+#: src/cybermarket_server/cmd_process.py:54
+msgid "Username has been set"
+msgstr "用户名已设置"
+
+#: src/cybermarket_server/cmd_process.py:58
+#: src/cybermarket_server/cmd_process.py:83
+#: src/cybermarket_server/cmd_process.py:114
+#: src/cybermarket_server/cmd_process.py:152
+#: src/cybermarket_server/cmd_process.py:177
+#: src/cybermarket_server/cmd_process.py:213
+#: src/cybermarket_server/cmd_process.py:245
+#: src/cybermarket_server/cmd_process.py:273
+#: src/cybermarket_server/cmd_process.py:298
+#: src/cybermarket_server/cmd_process.py:328
+#: src/cybermarket_server/cmd_process.py:410
+#: src/cybermarket_server/cmd_process.py:490
+#: src/cybermarket_server/cmd_process.py:515
+#: src/cybermarket_server/cmd_process.py:540
+#: src/cybermarket_server/cmd_process.py:565
+#: src/cybermarket_server/cmd_process.py:591
+#: src/cybermarket_server/cmd_process.py:622
+#: src/cybermarket_server/cmd_process.py:649
+#: src/cybermarket_server/cmd_process.py:674
+#: src/cybermarket_server/cmd_process.py:708
+#: src/cybermarket_server/cmd_process.py:733
+msgid "You have not logged in or your login has timed out"
+msgstr "您尚未登录或登录超时"
+
+#: src/cybermarket_server/cmd_process.py:79
+#: src/cybermarket_server/cmd_process.py:561
+msgid "Email has been set"
+msgstr "邮箱已设置"
+
+#: src/cybermarket_server/cmd_process.py:106
+#: src/cybermarket_server/cmd_process.py:614
+msgid "New password has been set"
+msgstr "新密码已设置"
+
+#: src/cybermarket_server/cmd_process.py:110
+#: src/cybermarket_server/cmd_process.py:148
+msgid "The password of the user is incorrect"
+msgstr "用户密码不正确"
+
+#: src/cybermarket_server/cmd_process.py:138
+msgid "The user has been logged in, please do not log in again"
+msgstr "该用户已登录，请勿再次登录"
+
+#: src/cybermarket_server/cmd_process.py:144
+msgid "This user is logged in"
+msgstr "用户已登录"
+
+#: src/cybermarket_server/cmd_process.py:173
+#: src/cybermarket_server/cmd_process.py:511
+msgid "You have successfully logged out"
+msgstr "您已成功退出"
+
+#: src/cybermarket_server/cmd_process.py:200
+msgid "The quantity of added products should be a positive integer"
+msgstr "添加的产品数量应为正整数"
+
+#: src/cybermarket_server/cmd_process.py:204
+msgid "The product you are trying to add cannot be found"
+msgstr "找不到您尝试添加的产品"
+
+#: src/cybermarket_server/cmd_process.py:209
+msgid "This product has been added to the shopping cart"
+msgstr "该产品已添加至购物车"
+
+#: src/cybermarket_server/cmd_process.py:236
+msgid "This product is not in your shopping cart"
+msgstr "该产品不在您的购物车中"
+
+#: src/cybermarket_server/cmd_process.py:241
+msgid "This product has been removed from the shopping cart"
+msgstr "该产品已从购物车中删除"
+
+#: src/cybermarket_server/cmd_process.py:266
+msgid "Obtained order list"
+msgstr "已获取订单列表"
+
+#: src/cybermarket_server/cmd_process.py:268
+#: src/cybermarket_server/cmd_process.py:354
+#: src/cybermarket_server/cmd_process.py:379
+msgid "storename"
+msgstr "店铺名称"
+
+#: src/cybermarket_server/cmd_process.py:268
+#: src/cybermarket_server/cmd_process.py:379
+msgid "productname"
+msgstr "产品名称"
+
+#: src/cybermarket_server/cmd_process.py:269
+#: src/cybermarket_server/cmd_process.py:380
+msgid "price"
+msgstr "价格"
+
+#: src/cybermarket_server/cmd_process.py:269
+msgid "quantity"
+msgstr "数量"
+
+#: src/cybermarket_server/cmd_process.py:294
+msgid "Order price obtained"
+msgstr "订单价格已获取"
+
+#: src/cybermarket_server/cmd_process.py:320
+msgid "Order has been checked out"
+msgstr "订单已结账"
+
+#: src/cybermarket_server/cmd_process.py:354
+#: src/cybermarket_server/cmd_process.py:380
+msgid "description"
+msgstr "描述"
+
+#: src/cybermarket_server/cmd_process.py:355
+msgid "email"
+msgstr "电子邮件"
+
+#: src/cybermarket_server/cmd_process.py:377
+msgid "Product list has been obtained"
+msgstr "已获取产品清单"
+
+#: src/cybermarket_server/cmd_process.py:379
+msgid "product_id"
+msgstr "产品编号"
+
+#: src/cybermarket_server/cmd_process.py:380
+msgid "stock"
+msgstr "库存数量"
+
+#: src/cybermarket_server/cmd_process.py:384
+msgid "No store with this name found"
+msgstr "未找到该名称的商店"
+
+#: src/cybermarket_server/cmd_process.py:406
+msgid "Invitation code has been generated"
+msgstr "邀请码已生成"
+
+#: src/cybermarket_server/cmd_process.py:435
+msgid "This storename is occupied"
+msgstr "该店名已被占用"
+
+#: src/cybermarket_server/cmd_process.py:450
+msgid ""
+"Your invitation code cannot be verified. This invitation code may be "
+"wrong or has already been used. Please contact other merchants to request"
+" the invitation code."
+msgstr "无法验证您的邀请码。 该邀请码可能有误或已被使用。 请联系其他商户索取邀请码。"
+
+#: src/cybermarket_server/cmd_process.py:476
+msgid "The merchant has been logged in, please do not log in again"
+msgstr "商户已登录，请勿再次登录"
+
+#: src/cybermarket_server/cmd_process.py:482
+msgid "This merchant is logged in"
+msgstr "该商户已登录"
+
+#: src/cybermarket_server/cmd_process.py:486
+#: src/cybermarket_server/cmd_process.py:618
+msgid "The password of the merchant is incorrect"
+msgstr "商户密码不正确"
+
+#: src/cybermarket_server/cmd_process.py:536
+msgid "Storename has been set"
+msgstr "店铺名称已设定"
+
+#: src/cybermarket_server/cmd_process.py:587
+msgid "Description has been set"
+msgstr "描述已设定"
+
+#: src/cybermarket_server/cmd_process.py:645
+msgid "This product has been added to the product list"
+msgstr "该产品已添加到产品列表中"
+
+#: src/cybermarket_server/cmd_process.py:670
+msgid "This product has been deleted from the product list"
+msgstr "该产品已从产品列表中删除"
+
+#: src/cybermarket_server/cmd_process.py:700
+msgid "This product has been restock"
+msgstr "该产品已补货"
+
+#: src/cybermarket_server/cmd_process.py:704
+msgid "You are restocking an item that is not from this store"
+msgstr "您正在补货的商品不是来自该商店"
+
+#: src/cybermarket_server/cmd_process.py:729
+msgid "Your total profit has been obtained"
+msgstr "您的总利润已获取"
+
+#: src/cybermarket_server/cmd_process.py:790
+msgid "You are trying to call an undefined method"
+msgstr "您正在尝试调用未定义的方法"
+
```

### Comparing `cybermarket_server-1.0.0/pyproject.toml` & `cybermarket_server-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cybermarket_server"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     {name = "Hailin Liu", email = "0123liuhailin@gmail.com"},
 ]
 description = "The server of the online network market accepts login, listing, purchase, etc. requests sent by the client."
 readme = "README.md"
 requires-python = ">=3.11"
 keywords = ["shopping", "online-market"]
```

### Comparing `cybermarket_server-1.0.0/setup.py` & `cybermarket_server-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `cybermarket_server-1.0.0/src/cybermarket_server/__main__.py` & `cybermarket_server-1.0.1/src/cybermarket_server/__main__.py`

 * *Files identical despite different names*

### Comparing `cybermarket_server-1.0.0/src/cybermarket_server/cmd_process.py` & `cybermarket_server-1.0.1/src/cybermarket_server/cmd_process.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,15 +261,15 @@
         item_dataframe (pd.Dataframe): Dataframe of items in the shopping cart
     """
     result = session.query(Client).filter(
         Client.connected_address == connected_address).first()
     if result:
         msg = _("Obtained order list")
         reply = str(request_id) + " 200 OK: " + msg
-        column_labels = [_('storename'), _('productname'),
+        column_labels = [_('storename'), _("product_id"), _('productname'),
                          _('price'), _('quantity')]
         df = pd.DataFrame(result.get_items(), columns=column_labels)
         return [reply, df]
     else:
         msg = _("You have not logged in or your login has timed out")
         reply = str(request_id) + " 401 Unauthorized: " + msg
         return [reply]
```

### Comparing `cybermarket_server-1.0.0/src/cybermarket_server/database/cybermarket.db` & `cybermarket_server-1.0.1/src/cybermarket_server/database/cybermarket.db`

 * *Files identical despite different names*

### Comparing `cybermarket_server-1.0.0/src/cybermarket_server/invitation.py` & `cybermarket_server-1.0.1/src/cybermarket_server/invitation.py`

 * *Files identical despite different names*

### Comparing `cybermarket_server-1.0.0/src/cybermarket_server/lang.py` & `cybermarket_server-1.0.1/src/cybermarket_server/lang.py`

 * *Files identical despite different names*

### Comparing `cybermarket_server-1.0.0/src/cybermarket_server/locale/ru_RU/LC_MESSAGES/Russian.mo` & `cybermarket_server-1.0.1/src/cybermarket_server/locale/ru_RU/LC_MESSAGES/Russian.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  1.0.0\n"
 "Report-Msgid-Bugs-To: 0123liuhailin@gmail.com\n"
-"POT-Creation-Date: 2024-05-03 15:40+0300\n"
+"POT-Creation-Date: 2024-05-05 01:12+0300\n"
 "PO-Revision-Date: 2024-04-27 16:07+0300\n"
 "Last-Translator: @lhl4971 <github.com/lhl4971/>\n"
 "Language: ru_RU\n"
 "Language-Team: ru_RU <github.com/pyCybermarket2024>\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
```

### Comparing `cybermarket_server-1.0.0/src/cybermarket_server/locale/zh_CN/LC_MESSAGES/Chinese.mo` & `cybermarket_server-1.0.1/src/cybermarket_server/locale/zh_CN/LC_MESSAGES/Chinese.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  1.0.0\n"
 "Report-Msgid-Bugs-To: 0123liuhailin@gmail.com\n"
-"POT-Creation-Date: 2024-05-03 15:40+0300\n"
+"POT-Creation-Date: 2024-05-05 01:12+0300\n"
 "PO-Revision-Date: 2024-04-27 15:54+0300\n"
 "Last-Translator: @lhl4971 <github.com/lhl4971/>\n"
 "Language: zh_Hans_CN\n"
 "Language-Team: ru_RU <github.com/pyCybermarket2024>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `cybermarket_server-1.0.0/src/cybermarket_server/model.py` & `cybermarket_server-1.0.1/src/cybermarket_server/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,14 +187,15 @@
 
         Returns:
             list: A list of tuples containing store name, product name, price,
             and quantity of each item.
         """
         result = session.query(
             Merchant.storename,
+            Product.productId,
             Product.productname,
             Product.price,
             Order.quantity
             ).join(
                 Product, Order.product_id == Product.productId
             ).join(
                 Merchant, Product.merchant_id == Merchant.merchantId
@@ -209,15 +210,15 @@
 
         Returns:
             float: The total price of the items.
         """
         sum_price = 0
         item_list = self.get_items()
         for item in item_list:
-            sum_price += item[2]*item[3]
+            sum_price += item[3]*item[4]
         return sum_price
 
     def checkout_item(self):
         """Check out all items in the client's basket, finalizing the order."""
         for item in self.order:
             if item.quantity <= item.product.stock:
                 item.checkout()
```

### Comparing `cybermarket_server-1.0.0/src/cybermarket_server/setting.py` & `cybermarket_server-1.0.1/src/cybermarket_server/setting.py`

 * *Files identical despite different names*

### Comparing `cybermarket_server-1.0.0/tests/unit_test.py` & `cybermarket_server-1.0.1/tests/unit_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         cmd_process.client_create(
             "8000", "127.0.0.1:33000", "liuhailin",
             "0123liuhailin@gmail.com", "123456"
             )
 
     def test_0(self):
         result = cmd_process.client_create(
-            "0", "127.0.0.1:33001", "qangqi",
+            "0", "127.0.0.1:33001", "tangqi",
             "t390697002@gmail.com", "123456"
             )
         expected_result = ["0 201 Created"]
         self.assertEqual(result, expected_result)
 
     def test_1(self):
         result = cmd_process.client_create(
@@ -369,14 +369,15 @@
             "2", "127.0.0.1:33000", 2, 5
         )
         result = cmd_process.client_get_items(
             "3", "127.0.0.1:33000"
         )
         data = {
             'storename': ["Cybermarket", "Cybermarket"],
+            'product_id': [1, 2],
             'productname': ['router', 'switch'],
             'price': [100.0, 200.0],
             'quantity': [5, 5]
         }
         df = pd.DataFrame(data)
         expected_result = [
             "3 200 OK: Obtained order list", df
```

