# Comparing `tmp/gbulb-0.6.3.tar.gz` & `tmp/gbulb-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gbulb-0.6.3.tar", last modified: Sun Feb 20 01:48:37 2022, max compression
+gzip compressed data, was "gbulb-0.6.4.tar", last modified: Tue Feb  7 02:32:40 2023, max compression
```

## Comparing `gbulb-0.6.3.tar` & `gbulb-0.6.4.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-20 01:48:37.977825 gbulb-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-02-20 01:47:09.000000 gbulb-0.6.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3196 2022-02-20 01:47:09.000000 gbulb-0.6.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-02-20 01:47:09.000000 gbulb-0.6.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)      587 2022-02-20 01:47:09.000000 gbulb-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-02-20 01:47:09.000000 gbulb-0.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6385 2022-02-20 01:48:37.977825 gbulb-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5121 2022-02-20 01:47:09.000000 gbulb-0.6.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-20 01:48:37.973824 gbulb-0.6.3/changes/
--rw-r--r--   0 runner    (1001) docker     (121)     1210 2022-02-20 01:47:09.000000 gbulb-0.6.3/changes/template.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-20 01:48:37.973824 gbulb-0.6.3/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      663 2022-02-20 01:47:09.000000 gbulb-0.6.3/examples/gtk.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2139 2022-02-20 01:47:09.000000 gbulb-0.6.3/examples/test-gtk.py
--rw-r--r--   0 runner    (1001) docker     (121)      845 2022-02-20 01:47:09.000000 gbulb-0.6.3/examples/wait_signal.py
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-02-20 01:47:09.000000 gbulb-0.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1760 2022-02-20 01:48:37.977825 gbulb-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-02-20 01:47:09.000000 gbulb-0.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-20 01:48:37.973824 gbulb-0.6.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-20 01:48:37.973824 gbulb-0.6.3/src/gbulb/
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-02-20 01:47:09.000000 gbulb-0.6.3/src/gbulb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    32540 2022-02-20 01:47:09.000000 gbulb-0.6.3/src/gbulb/glib_events.py
--rw-r--r--   0 runner    (1001) docker     (121)     1892 2022-02-20 01:47:09.000000 gbulb-0.6.3/src/gbulb/gtk.py
--rw-r--r--   0 runner    (1001) docker     (121)    13196 2022-02-20 01:47:09.000000 gbulb-0.6.3/src/gbulb/transports.py
--rw-r--r--   0 runner    (1001) docker     (121)     1868 2022-02-20 01:47:09.000000 gbulb-0.6.3/src/gbulb/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-20 01:48:37.973824 gbulb-0.6.3/src/gbulb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6385 2022-02-20 01:48:37.000000 gbulb-0.6.3/src/gbulb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      684 2022-02-20 01:48:37.000000 gbulb-0.6.3/src/gbulb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-20 01:48:37.000000 gbulb-0.6.3/src/gbulb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-20 01:47:24.000000 gbulb-0.6.3/src/gbulb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-02-20 01:48:37.000000 gbulb-0.6.3/src/gbulb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-02-20 01:48:37.000000 gbulb-0.6.3/src/gbulb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-20 01:48:37.977825 gbulb-0.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      983 2022-02-20 01:47:09.000000 gbulb-0.6.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-20 01:48:37.977825 gbulb-0.6.3/tests/docker-images/
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-02-20 01:47:09.000000 gbulb-0.6.3/tests/docker-images/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-02-20 01:47:09.000000 gbulb-0.6.3/tests/docker-images/base.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)     1145 2022-02-20 01:47:09.000000 gbulb-0.6.3/tests/docker-images/python.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)    15072 2022-02-20 01:47:09.000000 gbulb-0.6.3/tests/test_glib_events.py
--rw-r--r--   0 runner    (1001) docker     (121)     1428 2022-02-20 01:47:09.000000 gbulb-0.6.3/tests/test_gtk.py
--rw-r--r--   0 runner    (1001) docker     (121)     2963 2022-02-20 01:47:09.000000 gbulb-0.6.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-02-20 01:47:09.000000 gbulb-0.6.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 02:32:40.109005 gbulb-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-02-07 02:31:45.000000 gbulb-0.6.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-02-07 02:31:45.000000 gbulb-0.6.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-02-07 02:31:45.000000 gbulb-0.6.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-02-07 02:31:45.000000 gbulb-0.6.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-02-07 02:31:45.000000 gbulb-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-02-07 02:31:45.000000 gbulb-0.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-02-07 02:32:40.109005 gbulb-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-02-07 02:31:45.000000 gbulb-0.6.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 02:32:40.097005 gbulb-0.6.4/changes/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-02-07 02:31:45.000000 gbulb-0.6.4/changes/template.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 02:32:40.101005 gbulb-0.6.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-02-07 02:31:45.000000 gbulb-0.6.4/examples/gtk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2140 2023-02-07 02:31:45.000000 gbulb-0.6.4/examples/test-gtk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-02-07 02:31:45.000000 gbulb-0.6.4/examples/wait_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-02-07 02:31:45.000000 gbulb-0.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-02-07 02:32:40.109005 gbulb-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-07 02:31:45.000000 gbulb-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 02:32:40.089005 gbulb-0.6.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 02:32:40.101005 gbulb-0.6.4/src/gbulb/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-02-07 02:31:45.000000 gbulb-0.6.4/src/gbulb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32922 2023-02-07 02:31:45.000000 gbulb-0.6.4/src/gbulb/glib_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-02-07 02:31:45.000000 gbulb-0.6.4/src/gbulb/gtk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13158 2023-02-07 02:31:45.000000 gbulb-0.6.4/src/gbulb/transports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-02-07 02:31:45.000000 gbulb-0.6.4/src/gbulb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 02:32:40.105005 gbulb-0.6.4/src/gbulb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-02-07 02:32:40.000000 gbulb-0.6.4/src/gbulb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-02-07 02:32:40.000000 gbulb-0.6.4/src/gbulb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 02:32:40.000000 gbulb-0.6.4/src/gbulb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 02:32:31.000000 gbulb-0.6.4/src/gbulb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-07 02:32:40.000000 gbulb-0.6.4/src/gbulb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-07 02:32:40.000000 gbulb-0.6.4/src/gbulb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 02:32:40.105005 gbulb-0.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-02-07 02:31:45.000000 gbulb-0.6.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 02:32:40.109005 gbulb-0.6.4/tests/docker-images/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-02-07 02:31:45.000000 gbulb-0.6.4/tests/docker-images/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-02-07 02:31:45.000000 gbulb-0.6.4/tests/docker-images/base.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-02-07 02:31:45.000000 gbulb-0.6.4/tests/docker-images/python.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    15071 2023-02-07 02:31:45.000000 gbulb-0.6.4/tests/test_glib_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-02-07 02:31:45.000000 gbulb-0.6.4/tests/test_gtk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-02-07 02:31:45.000000 gbulb-0.6.4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-02-07 02:31:45.000000 gbulb-0.6.4/tox.ini
```

### Comparing `gbulb-0.6.3/CHANGELOG.rst` & `gbulb-0.6.4/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,69 @@
 Change Log
 ==========
 
 .. towncrier release notes start
 
+0.6.4 (2023-02-07)
+------------------
+
+Features
+--------
+
+* Support for Python 3.11 was added. (`#61
+  <https://github.com/beeware/gbulb/issues/61`__`)
+* Initial support for Python 3.12 was added. (`#69
+  <https://github.com/beeware/gbulb/issues/69`__`)
+
+
+Bugfixes
+--------
+
+* The GTK event loop no longer forces the use of the default GLib main context
+  on every instance. (`#59 <https://github.com/beeware/gbulb/issues/59`__`)
+
+
+Misc
+----
+
+* #62, #64
+
+
 0.6.3 (2022-02-20)
 ------------------
 
 Bugfixes
 ^^^^^^^^
 
-* Corrected the import of ``InvalidStateError`` to fix an error seen on Python 3.8+. (`#56 <https://github.com/beeware/gbulb/issues/56>`__)
+* Corrected the import of ``InvalidStateError`` to fix an error seen on Python
+  3.8+. (`#56 <https://github.com/beeware/gbulb/issues/56>`__)
 
-* Reverted the fix from #47; that change led to file descriptor leaks. (`#52 <https://github.com/beeware/gbulb/issues/52>`_)
+* Reverted the fix from #47; that change led to file descriptor leaks. (`#52
+  <https://github.com/beeware/gbulb/issues/52>`__)
 
 
 0.6.2 (2021-10-24)
 ------------------
 
 Features
 ^^^^^^^^
 
-* Added support for Python 3.10. (`#50 <https://github.com/beeware/gbulb/issues/50>`_)
+* Added support for Python 3.10. (`#50
+  <https://github.com/beeware/gbulb/issues/50>`__)
 
 Bugfixes
 ^^^^^^^^
 
-* Corrects a problem where a socket isn't forgotten and causes 100% CPU load. (`#47 <https://github.com/beeware/gbulb/issues/47>`_)
+* Corrects a problem where a socket isn't forgotten and causes 100% CPU load.
+  (`#47 <https://github.com/beeware/gbulb/issues/47>`__)
 
 Improved Documentation
 ^^^^^^^^^^^^^^^^^^^^^^
 
-* (`#49 <https://github.com/beeware/gbulb/issues/49>`_)
+* #49
 
 
 0.6.1 (2018-08-09)
 ------------------
 
 Bug fixes
 ^^^^^^^^^
```

### Comparing `gbulb-0.6.3/LICENSE` & `gbulb-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gbulb-0.6.3/PKG-INFO` & `gbulb-0.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbulb
-Version: 0.6.3
+Version: 0.6.4
 Summary: GLib event loop for tulip (PEP 3156)
 Home-page: https://github.com/beeware/gbulb
 Author: Russell Keith-Magee
 Author-email: russell@keith-magee.com
 Maintainer: Russell Keith-Magee
 Maintainer-email: russell@keith-magee.com
 License: Apache 2.0
@@ -15,21 +15,22 @@
 Keywords: gtk,glib,gnome,asyncio,tulip
 Platform: linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE
 
 gbulb
 =====
 
 .. image:: https://img.shields.io/pypi/pyversions/gbulb.svg
@@ -41,18 +42,18 @@
    :alt: PyPI Version
 
 .. image:: https://img.shields.io/pypi/status/gbulb.svg
    :target: https://pypi.python.org/pypi/gbulb
    :alt: Maturity
 
 .. image:: https://img.shields.io/pypi/l/gbulb.svg
-   :target: https://github.com/beeware/gbulb/blob/master/LICENSE
+   :target: https://github.com/beeware/gbulb/blob/main/LICENSE
    :alt: BSD License
 
-.. image:: https://github.com/beeware/gbulb/workflows/CI/badge.svg?branch=master
+.. image:: https://github.com/beeware/gbulb/workflows/CI/badge.svg?branch=main
    :target: https://github.com/beeware/gbulb/actions
    :alt: Build Status
 
 .. image:: https://img.shields.io/discord/836455665257021440?label=Discord%20Chat&logo=discord&style=plastic
    :target: https://beeware.org/bee/chat/
    :alt: Discord server
 
@@ -63,15 +64,15 @@
 
 As much as possible, except where noted below, it mimics asyncio's interface.
 If you notice any differences, please report them.
 
 Requirements
 ------------
 
-- python 3.6+
+- python 3.7+
 - pygobject
 - glib
 - gtk+3 (optional)
 
 Usage
 -----
 
@@ -157,15 +158,15 @@
 ``GtkEventLoop`` will allow you to call ``run()`` recursively. You should also keep
 in mind that enclosed loops may be started at any time by third-party code
 calling GLib's primitives.
 
 Community
 ---------
 
-gblub is part of the `BeeWare suite`_. You can talk to the community through:
+gbulb is part of the `BeeWare suite`_. You can talk to the community through:
 
 * `@pybeeware on Twitter <https://twitter.com/pybeeware>`__
 
 * `Discord <https://beeware.org/bee/chat/>`__
 
 * The gbulb `Github Discussions forum <https://github.com/beeware/gbulb/discussions>`__
 
@@ -179,9 +180,7 @@
 want to contribute code, please `fork the code`_ and `submit a pull request`_.
 
 .. _BeeWare suite: http://beeware.org
 .. _BeeWare Community Code of Conduct: http://beeware.org/community/behavior/
 .. _log them on Github: https://github.com/beeware/gbulb/issues
 .. _fork the code: https://github.com/beeware/gbulb
 .. _submit a pull request: https://github.com/beeware/gbulb/pulls
-
-
```

### Comparing `gbulb-0.6.3/README.rst` & `gbulb-0.6.4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,18 @@
    :alt: PyPI Version
 
 .. image:: https://img.shields.io/pypi/status/gbulb.svg
    :target: https://pypi.python.org/pypi/gbulb
    :alt: Maturity
 
 .. image:: https://img.shields.io/pypi/l/gbulb.svg
-   :target: https://github.com/beeware/gbulb/blob/master/LICENSE
+   :target: https://github.com/beeware/gbulb/blob/main/LICENSE
    :alt: BSD License
 
-.. image:: https://github.com/beeware/gbulb/workflows/CI/badge.svg?branch=master
+.. image:: https://github.com/beeware/gbulb/workflows/CI/badge.svg?branch=main
    :target: https://github.com/beeware/gbulb/actions
    :alt: Build Status
 
 .. image:: https://img.shields.io/discord/836455665257021440?label=Discord%20Chat&logo=discord&style=plastic
    :target: https://beeware.org/bee/chat/
    :alt: Discord server
 
@@ -32,15 +32,15 @@
 
 As much as possible, except where noted below, it mimics asyncio's interface.
 If you notice any differences, please report them.
 
 Requirements
 ------------
 
-- python 3.6+
+- python 3.7+
 - pygobject
 - glib
 - gtk+3 (optional)
 
 Usage
 -----
 
@@ -126,15 +126,15 @@
 ``GtkEventLoop`` will allow you to call ``run()`` recursively. You should also keep
 in mind that enclosed loops may be started at any time by third-party code
 calling GLib's primitives.
 
 Community
 ---------
 
-gblub is part of the `BeeWare suite`_. You can talk to the community through:
+gbulb is part of the `BeeWare suite`_. You can talk to the community through:
 
 * `@pybeeware on Twitter <https://twitter.com/pybeeware>`__
 
 * `Discord <https://beeware.org/bee/chat/>`__
 
 * The gbulb `Github Discussions forum <https://github.com/beeware/gbulb/discussions>`__
```

### Comparing `gbulb-0.6.3/examples/test-gtk.py` & `gbulb-0.6.4/examples/test-gtk.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/env python3
-from gi.repository import Gtk
 import asyncio
+
+from gi.repository import Gtk
+
 import gbulb
 import gbulb.gtk
 
 
 class ProgressBarWindow(Gtk.Window):
-
     def __init__(self):
         Gtk.Window.__init__(self, title="ProgressBar Demo")
         self.set_border_width(10)
 
         vbox = Gtk.VBox()
         self.add(vbox)
```

### Comparing `gbulb-0.6.3/examples/wait_signal.py` & `gbulb-0.6.4/examples/wait_signal.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 import asyncio
 
-import gbulb
-
 from gi.repository import Gtk
 
+import gbulb
+
 
 @asyncio.coroutine
 def counter(label):
     i = 0
     while True:
         label.set_text(str(i))
         yield from asyncio.sleep(1)
         i += 1
 
 
 @asyncio.coroutine
 def text_watcher(label):
     while True:
-        yield from gbulb.wait_signal(label, 'changed')
-        print('label changed', label.get_text())
+        yield from gbulb.wait_signal(label, "changed")
+        print("label changed", label.get_text())
 
 
 def main():
     gbulb.install(gtk=True)
     loop = gbulb.get_event_loop()
 
     display = Gtk.Entry()
     vbox = Gtk.VBox()
 
     vbox.pack_start(display, True, True, 0)
 
-    win = Gtk.Window(title='Counter window')
-    win.connect('delete-event', lambda *args: loop.stop())
+    win = Gtk.Window(title="Counter window")
+    win.connect("delete-event", lambda *args: loop.stop())
     win.add(vbox)
 
     win.show_all()
 
     asyncio.ensure_future(text_watcher(display))
     asyncio.ensure_future(counter(display))
     loop.run_forever()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `gbulb-0.6.3/setup.cfg` & `gbulb-0.6.4/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -13,19 +13,20 @@
 maintainer_email = russell@keith-magee.com
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Developers
 	License :: OSI Approved :: Apache Software License
 	Operating System :: POSIX
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Software Development :: Libraries :: Python Modules
 license = Apache 2.0
 license_file = LICENSE
 description = GLib event loop for tulip (PEP 3156)
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 keywords = 
@@ -35,50 +36,30 @@
 	asyncio
 	tulip
 platforms = linux
 
 [options]
 zip_safe = False
 packages = find:
-python_requires = >= 3.6
+python_requires = >= 3.7
 include_package_data = True
 package_dir = 
 	= src
 install_requires = 
 	pygobject>=3.14.0
 
 [options.packages.find]
 where = src
 
-[aliases]
-test = pytest
-
-[bdist_wheel]
-universal = 1
-
-[flake8]
-exclude = \
-	venv*/*,\
-	local/*,\
-	docs/*,\
-	build/*,\
-	.eggs/*,\
-	.tox/*
-max-complexity = 10
-max-line-length = 119
-ignore = E121,E123,E126,E226,E24,E704,W503,W504,C901
-
-[isort]
-skip_glob = 
-	docs/conf.py
-	venv*
-	local
-multi_line_output = 3
-
 [tool:pytest]
 testpaths = tests
 norecursedirs = 
 
+[flake8]
+max-complexity = 25
+max-line-length = 119
+ignore = E203,E266,E501,W503
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `gbulb-0.6.3/src/gbulb/glib_events.py` & `gbulb-0.6.4/src/gbulb/glib_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,37 @@
-"""PEP 3156 event loop based on GLib"""
+"""PEP 3156 event loop based on GLib."""
 
 import asyncio
 import os
 import signal
 import socket
 import sys
 import threading
 import weakref
-from asyncio import constants, events, sslproto, tasks, CancelledError
+from asyncio import CancelledError, constants, events, sslproto, tasks
 
 try:
-    from gi.repository import GLib, Gio
+    from gi.repository import Gio, GLib
 except ImportError:  # pragma: no cover
     GLib = None
     Gio = None
 
 
 from . import transports
 
-
 if hasattr(os, "set_blocking"):
 
     def _set_nonblocking(fd):
         os.set_blocking(fd, False)
 
-
 elif sys.platform == "win32":
 
     def _set_nonblocking(fd):
         pass
 
-
 else:
     import fcntl
 
     def _set_nonblocking(fd):
         flags = fcntl.fcntl(fd, fcntl.F_GETFL)
         flags = flags | os.O_NONBLOCK
         fcntl.fcntl(fd, fcntl.F_SETFL, flags)
@@ -46,38 +43,39 @@
 # The Windows `asyncio` implementation doesn't actually use this, but
 # `glib` abstracts so nicely over this that we can use it on any platform
 if sys.platform == "win32":
 
     class AbstractChildWatcher:
         pass
 
-
 else:
     from asyncio.unix_events import AbstractChildWatcher
 
 
 class GLibChildWatcher(AbstractChildWatcher):
     def __init__(self):
         self._sources = {}
         self._handles = {}
 
     # On windows on has to open a process handle for the given PID number
     # before it's possible to use GLib's `child_watch_add` on it
     if sys.platform == "win32":
+
         def _create_handle_for_pid(self, pid):
             import _winapi
 
             return _winapi.OpenProcess(0x00100400, 0, pid)
 
         def _close_process_handle(self, handle):
             import _winapi
 
             _winapi.CloseHandle(handle)
 
     else:
+
         def _create_handle_for_pid(self, pid):
             return pid
 
         def _close_process_handle(self, pid):
             return None
 
     def attach_loop(self, loop):
@@ -181,25 +179,24 @@
     class GLibBaseEventLoopPlatformExt:
         def __init__(self):
             pass
 
         def close(self):
             pass
 
-
 else:
     from asyncio import unix_events
 
     class GLibBaseEventLoopPlatformExt(unix_events.SelectorEventLoop):
-        """
-        Semi-hack that allows us to leverage the existing implementation of Unix domain sockets
-        without having to actually implement a selector based event loop.
+        """Semi-hack that allows us to leverage the existing implementation of
+        Unix domain sockets without having to actually implement a selector
+        based event loop.
 
-        Note that both `__init__` and `close` DO NOT and SHOULD NOT ever call their parent
-        implementation!
+        Note that both `__init__` and `close` DO NOT and SHOULD NOT ever
+        call their parent implementation!
         """
 
         def __init__(self):
             self._sighandlers = {}
 
         def close(self):
             for sig in list(self._sighandlers):
@@ -229,24 +226,27 @@
                 self._sighandlers.pop(sig).cancel()
                 return True
             except KeyError:
                 return False
 
 
 class _BaseEventLoop(asyncio.BaseEventLoop):
-    """
-    Extra inheritance step that needs to be inserted so that we only ever indirectly inherit from
-    `asyncio.BaseEventLoop`. This is necessary as the Unix implementation will also indirectly
+    """Extra inheritance step that needs to be inserted so that we only ever
+    indirectly inherit from `asyncio.BaseEventLoop`.
+
+    This is necessary as the Unix implementation will also indirectly
     inherit from that class (thereby creating diamond inheritance).
-    Python permits and fully supports diamond inheritance so this is not a problem. However it
-    is, on the other hand, not permitted to inherit from a class both directly *and* indirectly –
-    hence we add this intermediate class to make sure that can never happen (see
-    https://stackoverflow.com/q/29214888 for a minimal example a forbidden inheritance tree) and
-    https://www.python.org/download/releases/2.3/mro/ for some extensive documentation of the
-    allowed inheritance structures in python.
+    Python permits and fully supports diamond inheritance so this is not
+    a problem. However it is, on the other hand, not permitted to
+    inherit from a class both directly *and* indirectly – hence we add
+    this intermediate class to make sure that can never happen (see
+    https://stackoverflow.com/q/29214888 for a minimal example a
+    forbidden inheritance tree) and
+    https://www.python.org/download/releases/2.3/mro/ for some extensive
+    documentation of the allowed inheritance structures in python.
     """
 
 
 class GLibBaseEventLoop(_BaseEventLoop, GLibBaseEventLoopPlatformExt):
     def __init__(self, context=None):
         self._handlers = set()
 
@@ -312,40 +312,44 @@
         sslcontext,
         waiter=None,
         *,
         server_side=False,
         server_hostname=None,
         extra=None,
         server=None,
-        ssl_handshake_timeout=None
+        ssl_handshake_timeout=None,
+        ssl_shutdown_timeout=None,
     ):
         """Create SSL transport."""
         # sslproto._is_sslproto_available was removed from asyncio, starting from Python 3.7.
         if (
             hasattr(sslproto, "_is_sslproto_available")
             and not sslproto._is_sslproto_available()
         ):
             raise NotImplementedError(
                 "Proactor event loop requires Python 3.5"
                 " or newer (ssl.MemoryBIO) to support "
                 "SSL"
             )
-        # Support for the ssl_handshake_timeout keyword argument was added in Python 3.7.
         extra_protocol_kwargs = {}
+        # Support for the ssl_handshake_timeout keyword argument was added in Python 3.7.
         if sys.version_info[:2] >= (3, 7):
             extra_protocol_kwargs["ssl_handshake_timeout"] = ssl_handshake_timeout
+        # Support for the ssl_shutdown_timeout keyword argument was added in Python 3.11.
+        if sys.version_info[:2] >= (3, 11):
+            extra_protocol_kwargs["ssl_shutdown_timeout"] = ssl_shutdown_timeout
 
         ssl_protocol = sslproto.SSLProtocol(
             self,
             protocol,
             sslcontext,
             waiter,
             server_side,
             server_hostname,
-            **extra_protocol_kwargs
+            **extra_protocol_kwargs,
         )
         transports.SocketTransport(
             self, rawsock, ssl_protocol, extra=extra, server=server
         )
         return ssl_protocol._app_transport
 
     def _make_datagram_transport(
@@ -372,15 +376,15 @@
         args,
         shell,
         stdin,
         stdout,
         stderr,
         bufsize,
         extra=None,
-        **kwargs
+        **kwargs,
     ):
         """Create subprocess transport."""
         with events.get_child_watcher() as watcher:
             waiter = asyncio.Future(loop=self)
             transport = transports.SubprocessTransport(
                 self,
                 protocol,
@@ -388,15 +392,15 @@
                 shell,
                 stdin,
                 stdout,
                 stderr,
                 bufsize,
                 waiter=waiter,
                 extra=extra,
-                **kwargs
+                **kwargs,
             )
 
             watcher.add_child_handler(
                 transport.get_pid(), self._child_watcher_callback, transport
             )
             try:
                 await waiter
@@ -425,31 +429,33 @@
         self,
         protocol_factory,
         sock,
         sslcontext=None,
         server=None,
         backlog=100,
         ssl_handshake_timeout=getattr(constants, "SSL_HANDSHAKE_TIMEOUT", 60.0),
+        ssl_shutdown_timeout=getattr(constants, "SSL_SHUTDOWN_TIMEOUT", 60.0),
     ):
         self._transports[sock.fileno()] = server
 
         def server_loop(f=None):
             try:
                 if f is not None:
                     (conn, addr) = f.result()
                     protocol = protocol_factory()
                     if sslcontext is not None:
-                        # FIXME: add ssl_handshake_timeout to this call once 3.7 support is merged in.
                         self._make_ssl_transport(
                             conn,
                             protocol,
                             sslcontext,
                             server_side=True,
                             extra={"peername": addr},
                             server=server,
+                            ssl_handshake_timeout=ssl_handshake_timeout,
+                            ssl_shutdown_timeout=ssl_shutdown_timeout,
                         )
                     else:
                         self._make_socket_transport(
                             conn, protocol, extra={"peername": addr}, server=server
                         )
                 if self.is_closed():
                     return
@@ -478,20 +484,22 @@
         sock.close()
 
     def _check_not_coroutine(self, callback, name):
         """Check whether the given callback is a coroutine or not."""
         from asyncio import coroutines
 
         if coroutines.iscoroutine(callback) or coroutines.iscoroutinefunction(callback):
-            raise TypeError("coroutines cannot be used with {}()".format(name))
+            raise TypeError(f"coroutines cannot be used with {name}()")
 
     def _ensure_fd_no_transport(self, fd):
         """Ensure that the given file descriptor is NOT used by any transport.
 
-        Adding another reader to a fd that is already being waited for causes a hang on Windows."""
+        Adding another reader to a fd that is already being waited for
+        causes a hang on Windows.
+        """
         try:
             transport = self._transports[fd]
         except KeyError:
             pass
         else:
             if not hasattr(transport, "is_closing") or not transport.is_closing():
                 raise RuntimeError(
@@ -526,15 +534,16 @@
 
             self._channels[sock_id] = channel
         return channel
 
     def _channel_from_fileobj(self, fileobj):
         """Create GLib IOChannel for the given file object.
 
-        On windows this will only work for files and pipes returned GLib's C library.
+        On windows this will only work for files and pipes returned
+        GLib's C library.
         """
         fd = self._fileobj_to_fd(fileobj)
 
         # pipes have been shown to be blocking here, so we'll do someone
         # else's job for them.
         _set_nonblocking(fd)
 
@@ -552,22 +561,22 @@
         """Obtain the raw file descriptor number for the given file object."""
         if isinstance(fileobj, int):
             fd = fileobj
         else:
             try:
                 fd = int(fileobj.fileno())
             except (AttributeError, TypeError, ValueError):
-                raise ValueError("Invalid file object: {!r}".format(fileobj))
+                raise ValueError(f"Invalid file object: {fileobj!r}")
         if fd < 0:
-            raise ValueError("Invalid file descriptor: {}".format(fd))
+            raise ValueError(f"Invalid file descriptor: {fd}")
         return fd
 
     def _delayed(self, source, callback=None, *args):
-        """Create a future that will complete after the given GLib Source object has become ready
-        and the data it tracks has been processed."""
+        """Create a future that will complete after the given GLib Source
+        object has become ready and the data it tracks has been processed."""
         future = None
 
         def handle_ready(*args):
             try:
                 if callback:
                     (done, result) = callback(*args)
                 else:
@@ -586,22 +595,21 @@
         future = asyncio.Future(loop=self)
         future.handle = GLibHandle(
             loop=self, source=source, repeat=True, callback=handle_ready, args=args
         )
         return future
 
     def _socket_handle_errors(self, sock):
-        """Raise exceptions for error states (SOL_ERROR) on the given socket object."""
+        """Raise exceptions for error states (SOL_ERROR) on the given socket
+        object."""
         errno = sock.getsockopt(socket.SOL_SOCKET, socket.SO_ERROR)
         if errno != 0:
             if sys.platform == "win32":
-                msg = socket.errorTab.get(errno, "Error {0}".format(errno))
-                raise OSError(
-                    errno, "[WinError {0}] {1}".format(errno, msg), None, errno
-                )
+                msg = socket.errorTab.get(errno, f"Error {errno}")
+                raise OSError(errno, f"[WinError {errno}] {msg}", None, errno)
             else:
                 raise OSError(errno, os.strerror(errno))
 
     ###############################
     # Low-level socket operations #
     ###############################
     def sock_connect(self, sock, address):
@@ -627,15 +635,15 @@
 
         def sock_connection_received(sock):
             return (True, sock.accept())
 
         async def accept_coro(future, conn):
             # Coroutine closing the accept socket if the future is cancelled
             try:
-                return (await future)
+                return await future
             except CancelledError:
                 sock.close()
                 raise
 
         future = self._delayed(source, sock_connection_received, sock)
         return self.create_task(accept_coro(future, sock))
 
@@ -672,14 +680,15 @@
         return self._channel_write(channel, buf, write_func)
 
     #####################################
     # Low-level GLib.Channel operations #
     #####################################
     def _channel_read(self, channel, nbytes, read_func=None):
         if read_func is None:
+
             def read_func(channel, nbytes):
                 return channel.read(nbytes)
 
         source = GLib.io_create_watch(channel, GLib.IO_IN | GLib.IO_HUP)
 
         def channel_readable(read_func, channel, nbytes):
             return (True, read_func(channel, nbytes))
@@ -924,23 +933,25 @@
 
     def set_argv(self, argv):
         """Sets argv to be passed to Gio.Application.run()"""
         self._argv = argv
 
 
 class GLibEventLoopPolicy(events.AbstractEventLoopPolicy):
-    """Default GLib event loop policy
+    """Default GLib event loop policy.
 
-    In this policy, each thread has its own event loop.  However, we only
-    automatically create an event loop by default for the main thread; other
-    threads by default have no event loop.
+    In this policy, each thread has its own event loop.  However, we
+    only automatically create an event loop by default for the main
+    thread; other threads by default have no event loop.
     """
 
+    EventLoopCls = GLibEventLoop
+
     # TODO add a parameter to synchronise with GLib's thread default contexts
-    #   (g_main_context_push_thread_default())
+    # (i.e., g_main_context_push_thread_default())
     def __init__(self, application=None):
         self._default_loop = None
         self._application = application
         self._watcher_lock = threading.Lock()
 
         self._watcher = None
         self._policy = asyncio.DefaultEventLoopPolicy()
@@ -954,41 +965,42 @@
                 if self._watcher is None:
                     self._watcher = GLibChildWatcher()
         return self._watcher
 
     def set_child_watcher(self, watcher):
         """Set a child watcher.
 
-        Must be an an instance of GLibChildWatcher, as it ties in with GLib
-        appropriately.
+        Must be an an instance of GLibChildWatcher, as it ties in with
+        GLib appropriately.
         """
 
         if watcher is not None and not isinstance(watcher, GLibChildWatcher):
             raise TypeError("Only GLibChildWatcher is supported!")
 
         with self._watcher_lock:
             self._watcher = watcher
 
     def new_event_loop(self):
         """Create a new event loop and return it."""
-        if not self._default_loop and isinstance(
-            threading.current_thread(), threading._MainThread
+        if (
+            not self._default_loop
+            and threading.main_thread().ident == threading.get_ident()
         ):
             loop = self.get_default_loop()
         else:
-            loop = GLibEventLoop()
+            loop = self.EventLoopCls()
         loop._policy = self
 
         return loop
 
     def get_default_loop(self):
         """Get the default event loop."""
         if not self._default_loop:
             self._default_loop = self._new_default_loop()
         return self._default_loop
 
     def _new_default_loop(self):
-        loop = GLibEventLoop(
+        loop = self.EventLoopCls(
             context=GLib.main_context_default(), application=self._application
         )
         loop._policy = self
         return loop
```

### Comparing `gbulb-0.6.3/src/gbulb/transports.py` & `gbulb-0.6.4/src/gbulb/transports.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import collections
 import socket
 import subprocess
-from asyncio import base_subprocess, transports, CancelledError, InvalidStateError
+from asyncio import CancelledError, InvalidStateError, base_subprocess, transports
 
 
 class BaseTransport(transports.BaseTransport):
     def __init__(self, loop, sock, protocol, waiter=None, extra=None, server=None):
         if hasattr(self, "_sock"):
             return  # The joys of multiple inheritance
 
@@ -366,17 +366,15 @@
                 "not {!r}".format(type(data).__name__)
             )
 
         if not data or self.is_closing():
             return
 
         if self._address and addr not in (None, self._address):
-            raise ValueError(
-                "Invalid address: must be None or {0}".format(self._address)
-            )
+            raise ValueError(f"Invalid address: must be None or {self._address}")
 
         # Do not copy the data yet, as we might be able to send it synchronously
         super().write((data, addr))
 
     sendto = write
 
 
@@ -417,9 +415,9 @@
         self._proc = subprocess.Popen(
             args,
             shell=shell,
             stdin=stdin,
             stdout=stdout,
             stderr=stderr,
             bufsize=bufsize,
-            **kwargs
+            **kwargs,
         )
```

### Comparing `gbulb-0.6.3/src/gbulb/utils.py` & `gbulb-0.6.4/src/gbulb/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 import weakref
 
-__all__ = ["install", "get_event_loop", "wait_signal"]
+__all__ = ["install", "get_event_loop", "new_event_loop", "wait_signal"]
 
 
 def install(gtk=False):
     """Set the default event loop policy.
 
     Call this as early as possible to ensure everything has a reference to the
     correct event loop.
@@ -37,14 +37,19 @@
 
 
 def get_event_loop():
     """Alias to asyncio.get_event_loop()."""
     return asyncio.get_event_loop()
 
 
+def new_event_loop():
+    """Alias to asyncio.new_event_loop()."""
+    return asyncio.new_event_loop()
+
+
 class wait_signal(asyncio.Future):
     """A future for waiting for a given signal to occur."""
 
     def __init__(self, obj, name, *, loop=None):
         super().__init__(loop=loop)
         self._obj = weakref.ref(obj, lambda s: self.cancel())
         self._hnd = obj.connect(name, self._signal_callback)
```

### Comparing `gbulb-0.6.3/src/gbulb.egg-info/PKG-INFO` & `gbulb-0.6.4/src/gbulb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbulb
-Version: 0.6.3
+Version: 0.6.4
 Summary: GLib event loop for tulip (PEP 3156)
 Home-page: https://github.com/beeware/gbulb
 Author: Russell Keith-Magee
 Author-email: russell@keith-magee.com
 Maintainer: Russell Keith-Magee
 Maintainer-email: russell@keith-magee.com
 License: Apache 2.0
@@ -15,21 +15,22 @@
 Keywords: gtk,glib,gnome,asyncio,tulip
 Platform: linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE
 
 gbulb
 =====
 
 .. image:: https://img.shields.io/pypi/pyversions/gbulb.svg
@@ -41,18 +42,18 @@
    :alt: PyPI Version
 
 .. image:: https://img.shields.io/pypi/status/gbulb.svg
    :target: https://pypi.python.org/pypi/gbulb
    :alt: Maturity
 
 .. image:: https://img.shields.io/pypi/l/gbulb.svg
-   :target: https://github.com/beeware/gbulb/blob/master/LICENSE
+   :target: https://github.com/beeware/gbulb/blob/main/LICENSE
    :alt: BSD License
 
-.. image:: https://github.com/beeware/gbulb/workflows/CI/badge.svg?branch=master
+.. image:: https://github.com/beeware/gbulb/workflows/CI/badge.svg?branch=main
    :target: https://github.com/beeware/gbulb/actions
    :alt: Build Status
 
 .. image:: https://img.shields.io/discord/836455665257021440?label=Discord%20Chat&logo=discord&style=plastic
    :target: https://beeware.org/bee/chat/
    :alt: Discord server
 
@@ -63,15 +64,15 @@
 
 As much as possible, except where noted below, it mimics asyncio's interface.
 If you notice any differences, please report them.
 
 Requirements
 ------------
 
-- python 3.6+
+- python 3.7+
 - pygobject
 - glib
 - gtk+3 (optional)
 
 Usage
 -----
 
@@ -157,15 +158,15 @@
 ``GtkEventLoop`` will allow you to call ``run()`` recursively. You should also keep
 in mind that enclosed loops may be started at any time by third-party code
 calling GLib's primitives.
 
 Community
 ---------
 
-gblub is part of the `BeeWare suite`_. You can talk to the community through:
+gbulb is part of the `BeeWare suite`_. You can talk to the community through:
 
 * `@pybeeware on Twitter <https://twitter.com/pybeeware>`__
 
 * `Discord <https://beeware.org/bee/chat/>`__
 
 * The gbulb `Github Discussions forum <https://github.com/beeware/gbulb/discussions>`__
 
@@ -179,9 +180,7 @@
 want to contribute code, please `fork the code`_ and `submit a pull request`_.
 
 .. _BeeWare suite: http://beeware.org
 .. _BeeWare Community Code of Conduct: http://beeware.org/community/behavior/
 .. _log them on Github: https://github.com/beeware/gbulb/issues
 .. _fork the code: https://github.com/beeware/gbulb
 .. _submit a pull request: https://github.com/beeware/gbulb/pulls
-
-
```

### Comparing `gbulb-0.6.3/src/gbulb.egg-info/SOURCES.txt` & `gbulb-0.6.4/src/gbulb.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+.pre-commit-config.yaml
 AUTHORS.rst
 CHANGELOG.rst
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
```

### Comparing `gbulb-0.6.3/tests/conftest.py` & `gbulb-0.6.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gbulb-0.6.3/tests/docker-images/python.Dockerfile` & `gbulb-0.6.4/tests/docker-images/python.Dockerfile`

 * *Files identical despite different names*

### Comparing `gbulb-0.6.3/tests/test_glib_events.py` & `gbulb-0.6.4/tests/test_glib_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import asyncio
 import sys
+from unittest import mock, skipIf
 
 import pytest
-
-from unittest import mock, skipIf
 from gi.repository import Gio, GLib
 
 is_windows = sys.platform == "win32"
 
 
 class TestGLibEventLoopPolicy:
     def test_set_child_watcher(self, glib_policy):
@@ -107,23 +106,23 @@
     @skipIf(is_windows, "Unix signal handlers are not supported on Windows")
     def test_remove_signal_handler_unhandled(self, glib_loop):
         import signal
 
         assert not glib_loop.remove_signal_handler(signal.SIGHUP)
 
     @skipIf(is_windows, "Unix signal handlers are not supported on Windows")
-    @pytest.mark.filterwarnings('ignore:g_unix_signal_source_new')
+    @pytest.mark.filterwarnings("ignore:g_unix_signal_source_new")
     def test_remove_signal_handler_sigkill(self, glib_loop):
         import signal
 
         with pytest.raises(RuntimeError):
             glib_loop.add_signal_handler(signal.SIGKILL, None)
 
     @skipIf(is_windows, "Unix signal handlers are not supported on Windows")
-    @pytest.mark.filterwarnings('ignore:g_unix_signal_source_new')
+    @pytest.mark.filterwarnings("ignore:g_unix_signal_source_new")
     def test_remove_signal_handler_sigill(self, glib_loop):
         import signal
 
         with pytest.raises(ValueError):
             glib_loop.add_signal_handler(signal.SIGILL, None)
 
     def test_run_until_complete_early_stop(self, glib_loop):
```

### Comparing `gbulb-0.6.3/tests/test_gtk.py` & `gbulb-0.6.4/tests/test_gtk.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pytest
 
 try:
     import gi
-    gi.require_version('Gtk', '3.0')
+
+    gi.require_version("Gtk", "3.0")
 
     from gi.repository import Gtk
 except ImportError:  # pragma: no cover
     Gtk = None
 
 
 @pytest.mark.skipif(not Gtk, reason="Gtk is not available")
@@ -35,19 +36,19 @@
         def inner():
             nonlocal loop_count
             i = loop_count
             print("starting loop", loop_count)
             loop_count += 1
 
             if loop_count == 10:
-                print("loop {} stopped".format(i))
+                print(f"loop {i} stopped")
                 gtk_loop.stop()
             else:
                 gtk_loop.call_soon(inner)
                 gtk_loop.run()
-                print("loop {} stopped".format(i))
+                print(f"loop {i} stopped")
                 gtk_loop.stop()
 
         gtk_loop.call_soon(inner)
         gtk_loop.run_forever()
 
         assert loop_count == 10
```

### Comparing `gbulb-0.6.3/tests/test_utils.py` & `gbulb-0.6.4/tests/test_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,17 +9,18 @@
         (False, False),
         (False, True),
         (True, False),
         (True, True),
     ],
 )
 def test_install(gtk, gtk_available):
-    from gbulb import install
     import sys
 
+    from gbulb import install
+
     called = False
 
     def set_event_loop_policy(pol):
         nonlocal called
         called = True
         cls_name = pol.__class__.__name__
         if gtk:
@@ -44,22 +45,32 @@
             else:
                 assert not import_error
                 assert called
 
 
 def test_get_event_loop():
     import asyncio
+
     import gbulb
 
-    assert asyncio.get_event_loop() is gbulb.get_event_loop()
+    try:
+        loop = gbulb.new_event_loop()
+        asyncio.set_event_loop(loop)
+
+        assert asyncio.get_event_loop() is gbulb.get_event_loop()
+
+    finally:
+        loop.close()
 
 
 def test_wait_signal(glib_loop):
     import asyncio
+
     from gi.repository import GObject
+
     from gbulb import wait_signal
 
     class TestObject(GObject.GObject):
         __gsignals__ = {
             "foo": (GObject.SignalFlags.RUN_LAST, None, (str,)),
         }
 
@@ -74,23 +85,31 @@
     async def waiter():
         nonlocal called
         r = await wait_signal(t, "foo")
         assert r == (t, "frozen brains tell no tales")
         called = True
 
     glib_loop.run_until_complete(
-        asyncio.wait([waiter(), emitter()], timeout=1)
+        asyncio.wait(
+            [
+                glib_loop.create_task(waiter()),
+                glib_loop.create_task(emitter()),
+            ],
+            timeout=1,
+        )
     )
 
     assert called
 
 
 def test_wait_signal_cancel(glib_loop):
     import asyncio
+
     from gi.repository import GObject
+
     from gbulb import wait_signal
 
     class TestObject(GObject.GObject):
         __gsignals__ = {
             "foo": (GObject.SignalFlags.RUN_LAST, None, (str,)),
         }
 
@@ -115,15 +134,21 @@
             called = True
 
         r.cancel()
         assert r.cancelled()
         cancelled = True
 
     glib_loop.run_until_complete(
-        asyncio.wait([waiter(), emitter()], timeout=1)
+        asyncio.wait(
+            [
+                glib_loop.create_task(waiter()),
+                glib_loop.create_task(emitter()),
+            ],
+            timeout=1,
+        )
     )
 
     assert cancelled
     assert called
 
 
 def test_wait_signal_cancel_state():
```

### Comparing `gbulb-0.6.3/tox.ini` & `gbulb-0.6.4/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Tox (http://tox.testrun.org/) is a tool for running tests
 # in multiple virtualenvs. This configuration file will run the
 # test suite on all supported python versions. To use it, "pip install tox"
 # and then run "tox" from this directory.
 
 [tox]
-envlist = flake8,towncrier-check,docs,package,py{36,37,38,39,310},pypy3
+envlist = flake8,towncrier-check,docs,package,py{37,38,39,310,311,312},pypy3
 skip_missing_interpreters = true
 
 [testenv]
 setenv = PYTHONPATH = {toxinidir}/src
 deps =
     pytest
     pytest-tldr
@@ -24,30 +24,31 @@
 commands = flake8 {posargs}
 
 [testenv:towncrier-check]
 skip_install = True
 deps =
     {[testenv:towncrier]deps}
 commands =
-    python -m towncrier.check
+    python -m towncrier.check --compare-with origin/main
 
 [testenv:towncrier]
 skip_install = True
 deps =
-    towncrier == 21.9.0
+    towncrier ~= 22.8
 commands =
     towncrier build {posargs}
 
 [testenv:docs]
 deps =
     -r{toxinidir}/docs/requirements_docs.txt
 commands =
     python setup.py build_sphinx -W
 
 [testenv:package]
+skip_install = True
 deps =
     check_manifest
     wheel
     twine
 commands =
     check-manifest -v
     python setup.py sdist bdist_wheel
```

