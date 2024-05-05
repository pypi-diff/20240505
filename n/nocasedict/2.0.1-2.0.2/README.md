# Comparing `tmp/nocasedict-2.0.1.tar.gz` & `tmp/nocasedict-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nocasedict-2.0.1.tar", last modified: Mon May  1 07:11:19 2023, max compression
+gzip compressed data, was "nocasedict-2.0.2.tar", last modified: Sun May  5 14:15:36 2024, max compression
```

## Comparing `nocasedict-2.0.1.tar` & `nocasedict-2.0.2.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-05-01 07:11:19.464289 nocasedict-2.0.1/
--rw-r--r--   0 maiera     (501) staff       (20)      424 2023-04-30 18:32:10.000000 nocasedict-2.0.1/INSTALL.md
--rw-r--r--   0 maiera     (501) staff       (20)    26526 2023-04-30 18:32:10.000000 nocasedict-2.0.1/LICENSE
--rw-r--r--   0 maiera     (501) staff       (20)      263 2023-05-01 07:11:18.000000 nocasedict-2.0.1/MANIFEST.in
--rw-r--r--   0 maiera     (501) staff       (20)     5596 2023-05-01 07:11:19.463941 nocasedict-2.0.1/PKG-INFO
--rw-r--r--   0 maiera     (501) staff       (20)     4256 2023-05-01 07:11:07.000000 nocasedict-2.0.1/README.rst
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-05-01 07:11:19.455568 nocasedict-2.0.1/nocasedict/
--rw-r--r--   0 maiera     (501) staff       (20)      294 2023-04-30 18:32:10.000000 nocasedict-2.0.1/nocasedict/__init__.py
--rw-r--r--   0 maiera     (501) staff       (20)     2151 2023-05-01 07:11:07.000000 nocasedict-2.0.1/nocasedict/_hashable.py
--rw-r--r--   0 maiera     (501) staff       (20)     1470 2023-05-01 07:11:07.000000 nocasedict-2.0.1/nocasedict/_keyableby.py
--rw-r--r--   0 maiera     (501) staff       (20)    27740 2023-05-01 07:11:07.000000 nocasedict-2.0.1/nocasedict/_nocasedict.py
--rw-r--r--   0 maiera     (501) staff       (20)     1141 2023-05-01 07:11:07.000000 nocasedict-2.0.1/nocasedict/_utils.py
--rw-r--r--   0 maiera     (501) staff       (20)      326 2023-05-01 07:11:07.000000 nocasedict-2.0.1/nocasedict/_version.py
--rw-r--r--   0 maiera     (501) staff       (20)        0 2023-05-01 07:11:07.000000 nocasedict-2.0.1/nocasedict/py.typed
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-05-01 07:11:19.458410 nocasedict-2.0.1/nocasedict.egg-info/
--rw-r--r--   0 maiera     (501) staff       (20)     5596 2023-05-01 07:11:19.000000 nocasedict-2.0.1/nocasedict.egg-info/PKG-INFO
--rw-r--r--   0 maiera     (501) staff       (20)      754 2023-05-01 07:11:19.000000 nocasedict-2.0.1/nocasedict.egg-info/SOURCES.txt
--rw-r--r--   0 maiera     (501) staff       (20)        1 2023-05-01 07:11:19.000000 nocasedict-2.0.1/nocasedict.egg-info/dependency_links.txt
--rw-r--r--   0 maiera     (501) staff       (20)       84 2023-05-01 07:11:19.000000 nocasedict-2.0.1/nocasedict.egg-info/requires.txt
--rw-r--r--   0 maiera     (501) staff       (20)       11 2023-05-01 07:11:19.000000 nocasedict-2.0.1/nocasedict.egg-info/top_level.txt
--rw-r--r--   0 maiera     (501) staff       (20)        1 2023-05-01 07:11:19.000000 nocasedict-2.0.1/nocasedict.egg-info/zip-safe
--rw-r--r--   0 maiera     (501) staff       (20)      506 2023-05-01 07:11:07.000000 nocasedict-2.0.1/requirements.txt
--rw-r--r--   0 maiera     (501) staff       (20)       38 2023-05-01 07:11:19.464421 nocasedict-2.0.1/setup.cfg
--rwxr-xr-x   0 maiera     (501) staff       (20)     6663 2023-05-01 07:11:07.000000 nocasedict-2.0.1/setup.py
--rw-r--r--   0 maiera     (501) staff       (20)     1070 2023-05-01 07:11:07.000000 nocasedict-2.0.1/test-requirements.txt
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-05-01 07:11:19.458957 nocasedict-2.0.1/tests/
--rw-r--r--   0 maiera     (501) staff       (20)        0 2020-07-21 05:09:05.000000 nocasedict-2.0.1/tests/__init__.py
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-05-01 07:11:19.459352 nocasedict-2.0.1/tests/installtest/
--rwxr-xr-x   0 maiera     (501) staff       (20)    12821 2023-04-30 18:32:10.000000 nocasedict-2.0.1/tests/installtest/test_install.sh
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-05-01 07:11:19.462124 nocasedict-2.0.1/tests/unittest/
--rw-r--r--   0 maiera     (501) staff       (20)        0 2020-07-21 05:09:05.000000 nocasedict-2.0.1/tests/unittest/__init__.py
--rw-r--r--   0 maiera     (501) staff       (20)     9210 2023-05-01 07:11:07.000000 nocasedict-2.0.1/tests/unittest/test_hashable.py
--rw-r--r--   0 maiera     (501) staff       (20)     4067 2023-05-01 07:11:07.000000 nocasedict-2.0.1/tests/unittest/test_keyableby.py
--rwxr-xr-x   0 maiera     (501) staff       (20)    90763 2023-05-01 07:11:07.000000 nocasedict-2.0.1/tests/unittest/test_nocasedict.py
--rw-r--r--   0 maiera     (501) staff       (20)      401 2023-04-30 18:32:10.000000 nocasedict-2.0.1/tests/unittest/test_package.py
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-05-01 07:11:19.463503 nocasedict-2.0.1/tests/utils/
--rw-r--r--   0 maiera     (501) staff       (20)        0 2020-07-21 05:09:05.000000 nocasedict-2.0.1/tests/utils/__init__.py
--rw-r--r--   0 maiera     (501) staff       (20)     3444 2023-04-30 18:32:10.000000 nocasedict-2.0.1/tests/utils/import_installed.py
--rw-r--r--   0 maiera     (501) staff       (20)     7138 2023-05-01 07:11:07.000000 nocasedict-2.0.1/tests/utils/simplified_test_function.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-05-05 14:15:36.869804 nocasedict-2.0.2/
+-rw-r--r--   0 maiera     (501) staff       (20)      424 2024-05-05 13:39:37.000000 nocasedict-2.0.2/AUTHORS.md
+-rw-r--r--   0 maiera     (501) staff       (20)      424 2023-04-30 18:32:10.000000 nocasedict-2.0.2/INSTALL.md
+-rw-r--r--   0 maiera     (501) staff       (20)    26526 2023-04-30 18:32:10.000000 nocasedict-2.0.2/LICENSE
+-rw-r--r--   0 maiera     (501) staff       (20)      262 2024-05-05 14:15:36.000000 nocasedict-2.0.2/MANIFEST.in
+-rw-r--r--   0 maiera     (501) staff       (20)     5511 2024-05-05 14:15:36.868984 nocasedict-2.0.2/PKG-INFO
+-rw-r--r--   0 maiera     (501) staff       (20)     3796 2024-05-05 09:30:25.000000 nocasedict-2.0.2/README.md
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-05-05 14:15:36.849783 nocasedict-2.0.2/nocasedict/
+-rw-r--r--   0 maiera     (501) staff       (20)      294 2023-04-30 18:32:10.000000 nocasedict-2.0.2/nocasedict/__init__.py
+-rw-r--r--   0 maiera     (501) staff       (20)     2151 2023-11-20 16:34:28.000000 nocasedict-2.0.2/nocasedict/_hashable.py
+-rw-r--r--   0 maiera     (501) staff       (20)     1462 2024-05-05 10:32:48.000000 nocasedict-2.0.2/nocasedict/_keyableby.py
+-rw-r--r--   0 maiera     (501) staff       (20)    27652 2024-05-05 10:32:48.000000 nocasedict-2.0.2/nocasedict/_nocasedict.py
+-rw-r--r--   0 maiera     (501) staff       (20)     1141 2023-11-20 16:34:28.000000 nocasedict-2.0.2/nocasedict/_utils.py
+-rw-r--r--   0 maiera     (501) staff       (20)      326 2024-05-05 14:15:00.000000 nocasedict-2.0.2/nocasedict/_version.py
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2023-11-20 16:34:28.000000 nocasedict-2.0.2/nocasedict/py.typed
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-05-05 14:15:36.865383 nocasedict-2.0.2/nocasedict.egg-info/
+-rw-r--r--   0 maiera     (501) staff       (20)     5511 2024-05-05 14:15:36.000000 nocasedict-2.0.2/nocasedict.egg-info/PKG-INFO
+-rw-r--r--   0 maiera     (501) staff       (20)      764 2024-05-05 14:15:36.000000 nocasedict-2.0.2/nocasedict.egg-info/SOURCES.txt
+-rw-r--r--   0 maiera     (501) staff       (20)        1 2024-05-05 14:15:36.000000 nocasedict-2.0.2/nocasedict.egg-info/dependency_links.txt
+-rw-r--r--   0 maiera     (501) staff       (20)      171 2024-05-05 14:15:36.000000 nocasedict-2.0.2/nocasedict.egg-info/requires.txt
+-rw-r--r--   0 maiera     (501) staff       (20)       11 2024-05-05 14:15:36.000000 nocasedict-2.0.2/nocasedict.egg-info/top_level.txt
+-rw-r--r--   0 maiera     (501) staff       (20)        1 2024-05-05 14:15:36.000000 nocasedict-2.0.2/nocasedict.egg-info/zip-safe
+-rw-r--r--   0 maiera     (501) staff       (20)      506 2023-11-20 16:34:28.000000 nocasedict-2.0.2/requirements.txt
+-rw-r--r--   0 maiera     (501) staff       (20)       38 2024-05-05 14:15:36.870088 nocasedict-2.0.2/setup.cfg
+-rwxr-xr-x   0 maiera     (501) staff       (20)     6665 2024-05-05 09:30:25.000000 nocasedict-2.0.2/setup.py
+-rw-r--r--   0 maiera     (501) staff       (20)     1143 2024-05-05 13:33:53.000000 nocasedict-2.0.2/test-requirements.txt
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-05-05 14:15:36.853509 nocasedict-2.0.2/tests/
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2020-07-21 05:09:05.000000 nocasedict-2.0.2/tests/__init__.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-05-05 14:15:36.854096 nocasedict-2.0.2/tests/installtest/
+-rwxr-xr-x   0 maiera     (501) staff       (20)    11871 2023-11-20 16:34:28.000000 nocasedict-2.0.2/tests/installtest/test_install.sh
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-05-05 14:15:36.858998 nocasedict-2.0.2/tests/unittest/
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2020-07-21 05:09:05.000000 nocasedict-2.0.2/tests/unittest/__init__.py
+-rw-r--r--   0 maiera     (501) staff       (20)     9208 2024-05-05 10:32:48.000000 nocasedict-2.0.2/tests/unittest/test_hashable.py
+-rw-r--r--   0 maiera     (501) staff       (20)     4081 2023-11-20 16:34:28.000000 nocasedict-2.0.2/tests/unittest/test_keyableby.py
+-rwxr-xr-x   0 maiera     (501) staff       (20)    90695 2024-05-05 10:32:48.000000 nocasedict-2.0.2/tests/unittest/test_nocasedict.py
+-rw-r--r--   0 maiera     (501) staff       (20)      401 2023-04-30 18:32:10.000000 nocasedict-2.0.2/tests/unittest/test_package.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-05-05 14:15:36.861415 nocasedict-2.0.2/tests/utils/
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2020-07-21 05:09:05.000000 nocasedict-2.0.2/tests/utils/__init__.py
+-rw-r--r--   0 maiera     (501) staff       (20)     3411 2024-05-05 10:32:48.000000 nocasedict-2.0.2/tests/utils/import_installed.py
+-rw-r--r--   0 maiera     (501) staff       (20)     7167 2024-05-05 09:02:08.000000 nocasedict-2.0.2/tests/utils/simplified_test_function.py
```

### Comparing `nocasedict-2.0.1/LICENSE` & `nocasedict-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nocasedict-2.0.1/PKG-INFO` & `nocasedict-2.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nocasedict
-Version: 2.0.1
+Version: 2.0.2
 Summary: A case-insensitive ordered dictionary for Python
 Home-page: https://github.com/pywbem/nocasedict
 Author: Andreas Maier
 Author-email: andreas.r.maier@gmx.de
 Maintainer: Andreas Maier
 Maintainer-email: andreas.r.maier@gmx.de
 License: GNU Lesser General Public License v2 or later (LGPLv2+)
@@ -21,133 +21,109 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
-Provides-Extra: test
+Description-Content-Type: text/markdown
 License-File: LICENSE
-
-nocasedict - A case-insensitive ordered dictionary for Python
-=============================================================
-
-.. image:: https://badge.fury.io/py/nocasedict.svg
-    :target: https://pypi.python.org/pypi/nocasedict/
-    :alt: Version on Pypi
-
-.. image:: https://github.com/pywbem/nocasedict/workflows/test/badge.svg?branch=master
-    :target: https://github.com/pywbem/nocasedict/actions/
-    :alt: Actions status
-
-.. image:: https://readthedocs.org/projects/nocasedict/badge/?version=latest
-    :target: https://readthedocs.org/projects/nocasedict/builds/
-    :alt: Docs build status (master)
-
-.. image:: https://coveralls.io/repos/github/pywbem/nocasedict/badge.svg?branch=master
-    :target: https://coveralls.io/github/pywbem/nocasedict?branch=master
-    :alt: Test coverage (master)
-
-
-Overview
---------
-
-Class `NocaseDict`_ is a case-insensitive ordered dictionary that preserves
-the original lexical case of its keys.
+License-File: AUTHORS.md
+Provides-Extra: test
+Requires-Dist: pytest>=7.0.0; extra == "test"
+Requires-Dist: virtualenv>=20.15.0; python_version <= "3.11" and extra == "test"
+Requires-Dist: virtualenv>=20.23.0; python_version >= "3.12" and extra == "test"
+Requires-Dist: packaging>=17.0; extra == "test"
+Requires-Dist: pluggy>=0.13.1; extra == "test"
+Requires-Dist: six>=1.14.0; extra == "test"
+
+# nocasedict - A case-insensitive ordered dictionary for Python
+
+[![Version on Pypi](https://img.shields.io/pypi/v/nocasedict.svg)](https://pypi.python.org/pypi/nocasedict/)
+[![Test status (master)](https://github.com/pywbem/nocasedict/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/pywbem/nocasedict/actions/workflows/test.yml?query=branch%3Amaster)
+[![Docs status (master)](https://readthedocs.org/projects/nocasedict/badge/?version=latest)](https://readthedocs.org/projects/nocasedict/builds/)
+[![Test coverage (master)](https://coveralls.io/repos/github/pywbem/nocasedict/badge.svg?branch=master)](https://coveralls.io/github/pywbem/nocasedict?branch=master)
+
+# Overview
+
+Class
+[NocaseDict](https://nocasedict.readthedocs.io/en/stable/reference.html#nocasedict.NocaseDict)
+is a case-insensitive ordered dictionary that preserves the original
+lexical case of its keys.
 
 Example:
 
-.. code-block:: bash
-
     $ python
     >>> from nocasedict import NocaseDict
 
     >>> dict1 = NocaseDict({'Alpha': 1, 'Beta': 2})
 
     >>> dict1['ALPHA']  # Lookup by key is case-insensitive
     1
 
     >>> print(dict1)  # Keys are returned with the original lexical case
     NocaseDict({'Alpha': 1, 'Beta': 2})
 
-The `NocaseDict`_ class supports the functionality of the built-in
-`dict class of Python 3.8`_ on all Python versions it supports with
-the following exceptions (and the case-insensitivity of course):
-
-* The ``iter..()``, ``view..()`` and ``has_key()`` methods are only present
-  on Python 2, consistent with the built-in ``dict`` class.
-
-* The ``keys()``, ``values()`` and ``items()`` methods return a list on Python 2
-  and a dictionary view on Python 3, consistent with the built-in ``dict``
-  class.
-
-.. _dict class of Python 3.8: https://docs.python.org/3.8/library/stdtypes.html#dict
+The
+[NocaseDict](https://nocasedict.readthedocs.io/en/stable/reference.html#nocasedict.NocaseDict)
+class supports the functionality of the built-in
+[dict class of Python 3.8](https://docs.python.org/3.8/library/stdtypes.html#dict)
+on all Python versions it supports with the following exceptions (and the
+case-insensitivity of course):
+
+- The `iter..()`, `view..()` and `has_key()` methods are only present
+  on Python 2, consistent with the built-in `dict` class.
+- The `keys()`, `values()` and `items()` methods return a list on
+  Python 2 and a dictionary view on Python 3, consistent with the
+  built-in `dict` class.
 
 The case-insensitivity is achieved by matching any key values as their
 casefolded values. By default, the casefolding is performed with
-`str.casefold()`_ for unicode string keys and with `bytes.lower()`_ for byte
-string keys.
-The default casefolding can be overridden with a user-defined casefold method.
-
-.. _str.casefold(): https://docs.python.org/3/library/stdtypes.html#str.casefold
-.. _bytes.lower(): https://docs.python.org/3/library/stdtypes.html#bytes.lower
+[str.casefold()](https://docs.python.org/3/library/stdtypes.html#str.casefold)
+for unicode string keys and with
+[bytes.lower()](https://docs.python.org/3/library/stdtypes.html#bytes.lower)
+for byte string keys. The default casefolding can be overridden with a
+user-defined casefold method.
 
 Functionality can be added using mixin classes:
 
-* `HashableMixin`_ mixin class: Adds case-insensitive hashability.
-
-* `KeyableByMixin`_ mixin generator function: Adds ability to get the key from
-  an attribute of the value object.
-
-Why yet another case-insensitive dictionary: We found that all previously
-existing case-insensitive dictionary packages on Pypi either had flaws, were
-not well maintained, or did not support the Python versions we needed.
-
-.. _dict of Python 2: https://docs.python.org/2/library/stdtypes.html#dict
-.. _dict of Python 3: https://docs.python.org/3/library/stdtypes.html#dict
-.. _NocaseDict: https://nocasedict.readthedocs.io/en/stable/reference.html#nocasedict.NocaseDict
-.. _HashableMixin: https://nocasedict.readthedocs.io/en/stable/reference.html#nocasedict.HashableMixin
-.. _KeyableByMixin: https://nocasedict.readthedocs.io/en/stable/reference.html#nocasedict.KeyableByMixin
-
-Installation
-------------
+- [HashableMixin](https://nocasedict.readthedocs.io/en/stable/reference.html#nocasedict.HashableMixin)
+  mixin class: Adds case-insensitive hashability.
+- [KeyableByMixin](https://nocasedict.readthedocs.io/en/stable/reference.html#nocasedict.KeyableByMixin)
+  mixin generator function: Adds ability to get the key from an
+  attribute of the value object.
+
+Why yet another case-insensitive dictionary: We found that all
+previously existing case-insensitive dictionary packages on Pypi either
+had flaws, were not well maintained, or did not support the Python
+versions we needed.
 
-To install the latest released version of the nocasedict package into your
-active Python environment:
+# Installation
 
-.. code-block:: bash
+To install the latest released version of the nocasedict package into
+your active Python environment:
 
     $ pip install nocasedict
 
 This will also install any prerequisite Python packages.
 
-For more details and alternative ways to install, see `Installation`_.
+For more details and alternative ways to install, see
+[Installation](https://nocasedict.readthedocs.io/en/stable/intro.html#installation).
 
-.. _Installation: https://nocasedict.readthedocs.io/en/stable/intro.html#installation
+# Documentation
 
+- [Documentation](https://nocasedict.readthedocs.io/en/stable/)
 
-Documentation
--------------
+# Change History
 
-* `Documentation <https://nocasedict.readthedocs.io/en/stable/>`_
+- [Change history](https://nocasedict.readthedocs.io/en/stable/changes.html)
 
-
-Change History
---------------
-
-* `Change history <https://nocasedict.readthedocs.io/en/stable/changes.html>`_
-
-
-Contributing
-------------
+# Contributing
 
 For information on how to contribute to the nocasedict project, see
-`Contributing <https://nocasedict.readthedocs.io/en/stable/development.html#contributing>`_.
-
+[Contributing](https://nocasedict.readthedocs.io/en/stable/development.html#contributing).
 
-License
--------
+# License
 
 The nocasedict project is provided under the
-`GNU Lesser General Public License (LGPL) version 2.1 <https://raw.githubusercontent.com/pywbem/nocasedict/master/LICENSE>`_,
+[GNU Lesser General Public License (LGPL) version 2.1](https://raw.githubusercontent.com/pywbem/nocasedict/master/LICENSE),
 or (at your option) any later version.
```

### Comparing `nocasedict-2.0.1/README.rst` & `nocasedict-2.0.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,122 +1,91 @@
-nocasedict - A case-insensitive ordered dictionary for Python
-=============================================================
+# nocasedict - A case-insensitive ordered dictionary for Python
 
-.. image:: https://badge.fury.io/py/nocasedict.svg
-    :target: https://pypi.python.org/pypi/nocasedict/
-    :alt: Version on Pypi
-
-.. image:: https://github.com/pywbem/nocasedict/workflows/test/badge.svg?branch=master
-    :target: https://github.com/pywbem/nocasedict/actions/
-    :alt: Actions status
-
-.. image:: https://readthedocs.org/projects/nocasedict/badge/?version=latest
-    :target: https://readthedocs.org/projects/nocasedict/builds/
-    :alt: Docs build status (master)
-
-.. image:: https://coveralls.io/repos/github/pywbem/nocasedict/badge.svg?branch=master
-    :target: https://coveralls.io/github/pywbem/nocasedict?branch=master
-    :alt: Test coverage (master)
-
-
-Overview
---------
-
-Class `NocaseDict`_ is a case-insensitive ordered dictionary that preserves
-the original lexical case of its keys.
+[![Version on Pypi](https://img.shields.io/pypi/v/nocasedict.svg)](https://pypi.python.org/pypi/nocasedict/)
+[![Test status (master)](https://github.com/pywbem/nocasedict/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/pywbem/nocasedict/actions/workflows/test.yml?query=branch%3Amaster)
+[![Docs status (master)](https://readthedocs.org/projects/nocasedict/badge/?version=latest)](https://readthedocs.org/projects/nocasedict/builds/)
+[![Test coverage (master)](https://coveralls.io/repos/github/pywbem/nocasedict/badge.svg?branch=master)](https://coveralls.io/github/pywbem/nocasedict?branch=master)
+
+# Overview
+
+Class
+[NocaseDict](https://nocasedict.readthedocs.io/en/stable/reference.html#nocasedict.NocaseDict)
+is a case-insensitive ordered dictionary that preserves the original
+lexical case of its keys.
 
 Example:
 
-.. code-block:: bash
-
     $ python
     >>> from nocasedict import NocaseDict
 
     >>> dict1 = NocaseDict({'Alpha': 1, 'Beta': 2})
 
     >>> dict1['ALPHA']  # Lookup by key is case-insensitive
     1
 
     >>> print(dict1)  # Keys are returned with the original lexical case
     NocaseDict({'Alpha': 1, 'Beta': 2})
 
-The `NocaseDict`_ class supports the functionality of the built-in
-`dict class of Python 3.8`_ on all Python versions it supports with
-the following exceptions (and the case-insensitivity of course):
-
-* The ``iter..()``, ``view..()`` and ``has_key()`` methods are only present
-  on Python 2, consistent with the built-in ``dict`` class.
-
-* The ``keys()``, ``values()`` and ``items()`` methods return a list on Python 2
-  and a dictionary view on Python 3, consistent with the built-in ``dict``
-  class.
-
-.. _dict class of Python 3.8: https://docs.python.org/3.8/library/stdtypes.html#dict
+The
+[NocaseDict](https://nocasedict.readthedocs.io/en/stable/reference.html#nocasedict.NocaseDict)
+class supports the functionality of the built-in
+[dict class of Python 3.8](https://docs.python.org/3.8/library/stdtypes.html#dict)
+on all Python versions it supports with the following exceptions (and the
+case-insensitivity of course):
+
+- The `iter..()`, `view..()` and `has_key()` methods are only present
+  on Python 2, consistent with the built-in `dict` class.
+- The `keys()`, `values()` and `items()` methods return a list on
+  Python 2 and a dictionary view on Python 3, consistent with the
+  built-in `dict` class.
 
 The case-insensitivity is achieved by matching any key values as their
 casefolded values. By default, the casefolding is performed with
-`str.casefold()`_ for unicode string keys and with `bytes.lower()`_ for byte
-string keys.
-The default casefolding can be overridden with a user-defined casefold method.
-
-.. _str.casefold(): https://docs.python.org/3/library/stdtypes.html#str.casefold
-.. _bytes.lower(): https://docs.python.org/3/library/stdtypes.html#bytes.lower
+[str.casefold()](https://docs.python.org/3/library/stdtypes.html#str.casefold)
+for unicode string keys and with
+[bytes.lower()](https://docs.python.org/3/library/stdtypes.html#bytes.lower)
+for byte string keys. The default casefolding can be overridden with a
+user-defined casefold method.
 
 Functionality can be added using mixin classes:
 
-* `HashableMixin`_ mixin class: Adds case-insensitive hashability.
+- [HashableMixin](https://nocasedict.readthedocs.io/en/stable/reference.html#nocasedict.HashableMixin)
+  mixin class: Adds case-insensitive hashability.
+- [KeyableByMixin](https://nocasedict.readthedocs.io/en/stable/reference.html#nocasedict.KeyableByMixin)
+  mixin generator function: Adds ability to get the key from an
+  attribute of the value object.
+
+Why yet another case-insensitive dictionary: We found that all
+previously existing case-insensitive dictionary packages on Pypi either
+had flaws, were not well maintained, or did not support the Python
+versions we needed.
 
-* `KeyableByMixin`_ mixin generator function: Adds ability to get the key from
-  an attribute of the value object.
+# Installation
 
-Why yet another case-insensitive dictionary: We found that all previously
-existing case-insensitive dictionary packages on Pypi either had flaws, were
-not well maintained, or did not support the Python versions we needed.
-
-.. _dict of Python 2: https://docs.python.org/2/library/stdtypes.html#dict
-.. _dict of Python 3: https://docs.python.org/3/library/stdtypes.html#dict
-.. _NocaseDict: https://nocasedict.readthedocs.io/en/stable/reference.html#nocasedict.NocaseDict
-.. _HashableMixin: https://nocasedict.readthedocs.io/en/stable/reference.html#nocasedict.HashableMixin
-.. _KeyableByMixin: https://nocasedict.readthedocs.io/en/stable/reference.html#nocasedict.KeyableByMixin
-
-Installation
-------------
-
-To install the latest released version of the nocasedict package into your
-active Python environment:
-
-.. code-block:: bash
+To install the latest released version of the nocasedict package into
+your active Python environment:
 
     $ pip install nocasedict
 
 This will also install any prerequisite Python packages.
 
-For more details and alternative ways to install, see `Installation`_.
-
-.. _Installation: https://nocasedict.readthedocs.io/en/stable/intro.html#installation
+For more details and alternative ways to install, see
+[Installation](https://nocasedict.readthedocs.io/en/stable/intro.html#installation).
 
+# Documentation
 
-Documentation
--------------
+- [Documentation](https://nocasedict.readthedocs.io/en/stable/)
 
-* `Documentation <https://nocasedict.readthedocs.io/en/stable/>`_
+# Change History
 
+- [Change history](https://nocasedict.readthedocs.io/en/stable/changes.html)
 
-Change History
---------------
-
-* `Change history <https://nocasedict.readthedocs.io/en/stable/changes.html>`_
-
-
-Contributing
-------------
+# Contributing
 
 For information on how to contribute to the nocasedict project, see
-`Contributing <https://nocasedict.readthedocs.io/en/stable/development.html#contributing>`_.
-
+[Contributing](https://nocasedict.readthedocs.io/en/stable/development.html#contributing).
 
-License
--------
+# License
 
 The nocasedict project is provided under the
-`GNU Lesser General Public License (LGPL) version 2.1 <https://raw.githubusercontent.com/pywbem/nocasedict/master/LICENSE>`_,
+[GNU Lesser General Public License (LGPL) version 2.1](https://raw.githubusercontent.com/pywbem/nocasedict/master/LICENSE),
 or (at your option) any later version.
```

### Comparing `nocasedict-2.0.1/nocasedict/_hashable.py` & `nocasedict-2.0.2/nocasedict/_hashable.py`

 * *Files identical despite different names*

### Comparing `nocasedict-2.0.1/nocasedict/_keyableby.py` & `nocasedict-2.0.2/nocasedict/_keyableby.py`

 * *Files 15% similar despite different names*

```diff
@@ -38,9 +38,9 @@
 
         md = MyDict([Obj('A', 1), Obj('B', 2)])
 
         print(md)
         # MyDict({'A': <__main__.Obj object at 0x10bc3d820>,
         #         'B': <__main__.Obj object at 0x10bc89af0>})
     """
-    return type('KeyableByMixin_{}'.format(key_attr),
+    return type(f'KeyableByMixin_{key_attr}',
                 (), {'nocasedict_KeyableByMixin_key_attr': key_attr})
```

### Comparing `nocasedict-2.0.1/nocasedict/_nocasedict.py` & `nocasedict-2.0.2/nocasedict/_nocasedict.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,16 +79,15 @@
     def __contains__(self, x):
         return x in iter(self)
 
     def __reversed__(self):
         return reversed(list(iter(self)))
 
     def __repr__(self):
-        return "{t}({d!r})".format(
-            t=self.__class__.__name__, d=self._dict)
+        return f"{self.__class__.__name__}({self._dict!r})"
 
 
 class dict_keys(_DictView, KeysView):
     # pylint: disable=too-few-public-methods
     """
     Dictionary values view.
     """
@@ -322,15 +321,15 @@
           AttributeError: The key does not have the casefold method.
           KeyError: Key does not exist (case-insensitively).
         """
         k = self._casefolded_key(key)
         try:
             return self._data[k][1]
         except KeyError:
-            key_error = KeyError("Key {0!r} not found".format(key))
+            key_error = KeyError(f"Key {key!r} not found")
             key_error.__cause__ = None  # Suppress 'During handling..'
             raise key_error  # pylint: disable=raise-missing-from
 
     def __setitem__(self, key: Key, value: Any) -> None:
         """
         Update the value of the item with an existing key (looked up
         case-insensitively), or if an item with the key does not exist, add an
@@ -354,15 +353,15 @@
           AttributeError: The key does not have the casefold method.
           KeyError: Key does not exist (case-insensitively).
         """
         k = self._casefolded_key(key)
         try:
             del self._data[k]
         except KeyError:
-            key_error = KeyError("Key {0!r} not found".format(key))
+            key_error = KeyError(f"Key {key!r} not found")
             key_error.__cause__ = None  # Suppress 'During handling..'
             raise key_error  # pylint: disable=raise-missing-from
 
     def __len__(self) -> int:
         """
         Return the number of items in the dictionary.
 
@@ -533,18 +532,17 @@
         debugging.
 
         The order of items is in dictionary iteration order, and the keys are
         in the original lexical case.
 
         Invoked when using e.g.: ``repr(ncd)``
         """
-        items = ["{0!r}: {1!r}".format(key, value)
-                 for key, value in self.items()]
+        items = [f"{key!r}: {value!r}" for key, value in self.items()]
         items_str = ', '.join(items)
-        return "{0.__class__.__name__}({{{1}}})".format(self, items_str)
+        return f"{self.__class__.__name__}({{{items_str}}})"
 
     def update(self, *args, **kwargs) -> None:
         # pylint: disable=arguments-differ,signature-differs
         # Note: The signature in Python 3 is: update(self, other=(), /, **kwds)
         #       Since the / marker cannot be used in Python 2, the *args
         #       approach has the same effect, i.e. to ensure that the
         #       parameter can only be specified as a keyword argument.
```

### Comparing `nocasedict-2.0.1/nocasedict/_utils.py` & `nocasedict-2.0.2/nocasedict/_utils.py`

 * *Files identical despite different names*

### Comparing `nocasedict-2.0.1/nocasedict.egg-info/PKG-INFO` & `nocasedict-2.0.2/nocasedict.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nocasedict
-Version: 2.0.1
+Version: 2.0.2
 Summary: A case-insensitive ordered dictionary for Python
 Home-page: https://github.com/pywbem/nocasedict
 Author: Andreas Maier
 Author-email: andreas.r.maier@gmx.de
 Maintainer: Andreas Maier
 Maintainer-email: andreas.r.maier@gmx.de
 License: GNU Lesser General Public License v2 or later (LGPLv2+)
@@ -21,133 +21,109 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
-Provides-Extra: test
+Description-Content-Type: text/markdown
 License-File: LICENSE
-
-nocasedict - A case-insensitive ordered dictionary for Python
-=============================================================
-
-.. image:: https://badge.fury.io/py/nocasedict.svg
-    :target: https://pypi.python.org/pypi/nocasedict/
-    :alt: Version on Pypi
-
-.. image:: https://github.com/pywbem/nocasedict/workflows/test/badge.svg?branch=master
-    :target: https://github.com/pywbem/nocasedict/actions/
-    :alt: Actions status
-
-.. image:: https://readthedocs.org/projects/nocasedict/badge/?version=latest
-    :target: https://readthedocs.org/projects/nocasedict/builds/
-    :alt: Docs build status (master)
-
-.. image:: https://coveralls.io/repos/github/pywbem/nocasedict/badge.svg?branch=master
-    :target: https://coveralls.io/github/pywbem/nocasedict?branch=master
-    :alt: Test coverage (master)
-
-
-Overview
---------
-
-Class `NocaseDict`_ is a case-insensitive ordered dictionary that preserves
-the original lexical case of its keys.
+License-File: AUTHORS.md
+Provides-Extra: test
+Requires-Dist: pytest>=7.0.0; extra == "test"
+Requires-Dist: virtualenv>=20.15.0; python_version <= "3.11" and extra == "test"
+Requires-Dist: virtualenv>=20.23.0; python_version >= "3.12" and extra == "test"
+Requires-Dist: packaging>=17.0; extra == "test"
+Requires-Dist: pluggy>=0.13.1; extra == "test"
+Requires-Dist: six>=1.14.0; extra == "test"
+
+# nocasedict - A case-insensitive ordered dictionary for Python
+
+[![Version on Pypi](https://img.shields.io/pypi/v/nocasedict.svg)](https://pypi.python.org/pypi/nocasedict/)
+[![Test status (master)](https://github.com/pywbem/nocasedict/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/pywbem/nocasedict/actions/workflows/test.yml?query=branch%3Amaster)
+[![Docs status (master)](https://readthedocs.org/projects/nocasedict/badge/?version=latest)](https://readthedocs.org/projects/nocasedict/builds/)
+[![Test coverage (master)](https://coveralls.io/repos/github/pywbem/nocasedict/badge.svg?branch=master)](https://coveralls.io/github/pywbem/nocasedict?branch=master)
+
+# Overview
+
+Class
+[NocaseDict](https://nocasedict.readthedocs.io/en/stable/reference.html#nocasedict.NocaseDict)
+is a case-insensitive ordered dictionary that preserves the original
+lexical case of its keys.
 
 Example:
 
-.. code-block:: bash
-
     $ python
     >>> from nocasedict import NocaseDict
 
     >>> dict1 = NocaseDict({'Alpha': 1, 'Beta': 2})
 
     >>> dict1['ALPHA']  # Lookup by key is case-insensitive
     1
 
     >>> print(dict1)  # Keys are returned with the original lexical case
     NocaseDict({'Alpha': 1, 'Beta': 2})
 
-The `NocaseDict`_ class supports the functionality of the built-in
-`dict class of Python 3.8`_ on all Python versions it supports with
-the following exceptions (and the case-insensitivity of course):
-
-* The ``iter..()``, ``view..()`` and ``has_key()`` methods are only present
-  on Python 2, consistent with the built-in ``dict`` class.
-
-* The ``keys()``, ``values()`` and ``items()`` methods return a list on Python 2
-  and a dictionary view on Python 3, consistent with the built-in ``dict``
-  class.
-
-.. _dict class of Python 3.8: https://docs.python.org/3.8/library/stdtypes.html#dict
+The
+[NocaseDict](https://nocasedict.readthedocs.io/en/stable/reference.html#nocasedict.NocaseDict)
+class supports the functionality of the built-in
+[dict class of Python 3.8](https://docs.python.org/3.8/library/stdtypes.html#dict)
+on all Python versions it supports with the following exceptions (and the
+case-insensitivity of course):
+
+- The `iter..()`, `view..()` and `has_key()` methods are only present
+  on Python 2, consistent with the built-in `dict` class.
+- The `keys()`, `values()` and `items()` methods return a list on
+  Python 2 and a dictionary view on Python 3, consistent with the
+  built-in `dict` class.
 
 The case-insensitivity is achieved by matching any key values as their
 casefolded values. By default, the casefolding is performed with
-`str.casefold()`_ for unicode string keys and with `bytes.lower()`_ for byte
-string keys.
-The default casefolding can be overridden with a user-defined casefold method.
-
-.. _str.casefold(): https://docs.python.org/3/library/stdtypes.html#str.casefold
-.. _bytes.lower(): https://docs.python.org/3/library/stdtypes.html#bytes.lower
+[str.casefold()](https://docs.python.org/3/library/stdtypes.html#str.casefold)
+for unicode string keys and with
+[bytes.lower()](https://docs.python.org/3/library/stdtypes.html#bytes.lower)
+for byte string keys. The default casefolding can be overridden with a
+user-defined casefold method.
 
 Functionality can be added using mixin classes:
 
-* `HashableMixin`_ mixin class: Adds case-insensitive hashability.
-
-* `KeyableByMixin`_ mixin generator function: Adds ability to get the key from
-  an attribute of the value object.
-
-Why yet another case-insensitive dictionary: We found that all previously
-existing case-insensitive dictionary packages on Pypi either had flaws, were
-not well maintained, or did not support the Python versions we needed.
-
-.. _dict of Python 2: https://docs.python.org/2/library/stdtypes.html#dict
-.. _dict of Python 3: https://docs.python.org/3/library/stdtypes.html#dict
-.. _NocaseDict: https://nocasedict.readthedocs.io/en/stable/reference.html#nocasedict.NocaseDict
-.. _HashableMixin: https://nocasedict.readthedocs.io/en/stable/reference.html#nocasedict.HashableMixin
-.. _KeyableByMixin: https://nocasedict.readthedocs.io/en/stable/reference.html#nocasedict.KeyableByMixin
-
-Installation
-------------
+- [HashableMixin](https://nocasedict.readthedocs.io/en/stable/reference.html#nocasedict.HashableMixin)
+  mixin class: Adds case-insensitive hashability.
+- [KeyableByMixin](https://nocasedict.readthedocs.io/en/stable/reference.html#nocasedict.KeyableByMixin)
+  mixin generator function: Adds ability to get the key from an
+  attribute of the value object.
+
+Why yet another case-insensitive dictionary: We found that all
+previously existing case-insensitive dictionary packages on Pypi either
+had flaws, were not well maintained, or did not support the Python
+versions we needed.
 
-To install the latest released version of the nocasedict package into your
-active Python environment:
+# Installation
 
-.. code-block:: bash
+To install the latest released version of the nocasedict package into
+your active Python environment:
 
     $ pip install nocasedict
 
 This will also install any prerequisite Python packages.
 
-For more details and alternative ways to install, see `Installation`_.
+For more details and alternative ways to install, see
+[Installation](https://nocasedict.readthedocs.io/en/stable/intro.html#installation).
 
-.. _Installation: https://nocasedict.readthedocs.io/en/stable/intro.html#installation
+# Documentation
 
+- [Documentation](https://nocasedict.readthedocs.io/en/stable/)
 
-Documentation
--------------
+# Change History
 
-* `Documentation <https://nocasedict.readthedocs.io/en/stable/>`_
+- [Change history](https://nocasedict.readthedocs.io/en/stable/changes.html)
 
-
-Change History
---------------
-
-* `Change history <https://nocasedict.readthedocs.io/en/stable/changes.html>`_
-
-
-Contributing
-------------
+# Contributing
 
 For information on how to contribute to the nocasedict project, see
-`Contributing <https://nocasedict.readthedocs.io/en/stable/development.html#contributing>`_.
-
+[Contributing](https://nocasedict.readthedocs.io/en/stable/development.html#contributing).
 
-License
--------
+# License
 
 The nocasedict project is provided under the
-`GNU Lesser General Public License (LGPL) version 2.1 <https://raw.githubusercontent.com/pywbem/nocasedict/master/LICENSE>`_,
+[GNU Lesser General Public License (LGPL) version 2.1](https://raw.githubusercontent.com/pywbem/nocasedict/master/LICENSE),
 or (at your option) any later version.
```

### Comparing `nocasedict-2.0.1/nocasedict.egg-info/SOURCES.txt` & `nocasedict-2.0.2/nocasedict.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+AUTHORS.md
 INSTALL.md
 LICENSE
 MANIFEST.in
-README.rst
+README.md
 requirements.txt
 setup.py
 test-requirements.txt
 nocasedict/__init__.py
 nocasedict/_hashable.py
 nocasedict/_keyableby.py
 nocasedict/_nocasedict.py
```

### Comparing `nocasedict-2.0.1/setup.py` & `nocasedict-2.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,16 +166,16 @@
     extras_require={
         "test": test_requirements,
     },
     cmdclass={
         'test': test,
     },
     description="A case-insensitive ordered dictionary for Python",
-    long_description=read_file('README.rst'),
-    long_description_content_type='text/x-rst',
+    long_description=read_file('README.md'),
+    long_description_content_type='text/markdown',
     license="GNU Lesser General Public License v2 or later (LGPLv2+)",
     author="Andreas Maier",
     author_email='andreas.r.maier@gmx.de',
     maintainer="Andreas Maier",
     maintainer_email='andreas.r.maier@gmx.de',
     url='https://github.com/pywbem/nocasedict',
     project_urls={
```

### Comparing `nocasedict-2.0.1/test-requirements.txt` & `nocasedict-2.0.2/test-requirements.txt`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 # pytest 7.0.0 started using type hints
 pytest>=7.0.0
 
 # Install test direct dependencies:
 
 # virtualenv
 # tox 3.21.0 requires virtualenv!=20.0.[0-7],>=16.0.0 and requires py>=3.5
-virtualenv>=20.1.0
+virtualenv>=20.15.0; python_version <= '3.11'
+virtualenv>=20.23.0; python_version >= '3.12'
 
 
 # Indirect dependencies with special constraints:
 
 # packaging (used by pytest)
 packaging>=17.0
```

### Comparing `nocasedict-2.0.1/tests/installtest/test_install.sh` & `nocasedict-2.0.2/tests/installtest/test_install.sh`

 * *Files 4% similar despite different names*

```diff
@@ -411,67 +411,43 @@
 {
   testcase="test1"
   info "Testcase $testcase: Pip install from repo root directory: ${ROOT_DIR}"
   make_virtualenv "$testcase"
 
   call "cd ${ROOT_DIR}; pip install . $PIP_OPTS" "Installing with pip from repo root directory (PACKAGE_LEVEL=$PACKAGE_LEVEL)"
 
-  assert_import_ok "${PACKAGE_NAME}"
-  remove_virtualenv "$testcase"
-  cleanup_egg_file
-}
-
-function test2()
-{
-  testcase="test2"
-  info "Testcase $testcase: setup.py install from repo root directory: ${ROOT_DIR}"
-  make_virtualenv "$testcase"
-
-  call "cd ${ROOT_DIR}; python setup.py install" "Installing with setup.py from repo root directory (latest package levels)"
-
+  pip list
   assert_import_ok "${PACKAGE_NAME}"
   remove_virtualenv "$testcase"
   cleanup_egg_file
 }
 
 function test3()
 {
   testcase="test3"
   info "Testcase $testcase: Pip install from wheel distribution archive: $WHL_DISTFILE"
   make_virtualenv "$testcase"
 
   call "cd ${TMP_TEST_DIR}; pip install $(abspath $WHL_DISTFILE) $PIP_OPTS" "Installing with pip from wheel distribution archive (PACKAGE_LEVEL=$PACKAGE_LEVEL)"
 
+  pip list
   assert_import_ok "${PACKAGE_NAME}"
   remove_virtualenv "$testcase"
   cleanup_egg_file
 }
 
 function test4()
 {
   testcase="test4"
   info "Testcase $testcase: Pip install from source distribution archive: $SRC_DISTFILE"
   make_virtualenv "$testcase"
 
   call "cd ${TMP_TEST_DIR}; pip install $(abspath $SRC_DISTFILE) $PIP_OPTS" "Installing with pip from source distribution archive (PACKAGE_LEVEL=$PACKAGE_LEVEL)"
 
-  assert_import_ok "${PACKAGE_NAME}"
-  remove_virtualenv "$testcase"
-  cleanup_egg_file
-}
-
-function test5()
-{
-  testcase="test5"
-  info "Testcase $testcase: setup.py install from unpacked source distribution archive: $SRC_DISTFILE"
-  make_virtualenv "$testcase"
-  run "tar -x -v -f $SRC_DISTFILE -C $SRC_DISTFILE_UNPACK_DIR" "Unpacking source distribution archive to: $SRC_DISTFILE_UNPACK_DIR"
-
-  call "cd $SRC_DISTFILE_UNPACK_DIR/$SRC_DISTFILE_TOP_DIR; python setup.py install" "Installing with setup.py from unpack directory: $SRC_DISTFILE_UNPACK_DIR/$SRC_DISTFILE_TOP_DIR (latest package levels)"
-
+  pip list
   assert_import_ok "${PACKAGE_NAME}"
   remove_virtualenv "$testcase"
   cleanup_egg_file
 }
 
 #----- main
 
@@ -495,15 +471,13 @@
   error "Cannot find Python command: $PYTHON_CMD"
   exit 1
 fi
 
 prep
 
 test1
-test2
 test3
 test4
-test5
 
 cleanup
 
 info "All testcases succeeded."
```

### Comparing `nocasedict-2.0.1/tests/unittest/test_hashable.py` & `nocasedict-2.0.2/tests/unittest/test_hashable.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 class NonHashable:
     # pylint: disable=too-few-public-methods
     """
     Class that raises TypeError when hashing its objects.
     """
 
     def __hash__(self):
-        raise TypeError("Cannot hash %s" % type(self))
+        raise TypeError(f"Cannot hash {type(self)}")
 
 
 TESTCASES_HASHABLEMIXIN_HASH = [
 
     # Testcases for HashableMixin.__hash__()
 
     # Each list item is a testcase tuple with these items:
```

### Comparing `nocasedict-2.0.1/tests/unittest/test_keyableby.py` & `nocasedict-2.0.2/tests/unittest/test_keyableby.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,8 +129,8 @@
     assert testcase.exp_exc_types is None
 
     assert len(ncd) == len(exp_tuples)
     for exp_key, exp_value in exp_tuples:
         assert exp_key in ncd
         value = ncd[exp_key]
         # pylint: disable=unidiomatic-typecheck
-        assert type(value) == type(exp_value)
+        assert type(value) == type(exp_value)  # noqa: E721
```

### Comparing `nocasedict-2.0.1/tests/unittest/test_nocasedict.py` & `nocasedict-2.0.2/tests/unittest/test_nocasedict.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,18 +54,18 @@
 class NonEquatable:
     # pylint: disable=too-few-public-methods
     """
     Class that raises TypeError when comparing its objects for equality.
     """
 
     def __eq__(self, other):
-        raise TypeError("Cannot compare %s to %s" % (type(self), type(other)))
+        raise TypeError(f"Cannot compare {type(self)} to {type(other)}")
 
     def __ne__(self, other):
-        raise TypeError("Cannot compare %s to %s" % (type(self), type(other)))
+        raise TypeError(f"Cannot compare {type(self)} to {type(other)}")
 
 
 TESTCASES_NOCASEDICT_INIT = [
 
     # Testcases for NocaseDict.__init__() / ncd=NocaseDict()
 
     # Each list item is a testcase tuple with these items:
@@ -309,26 +309,26 @@
 
     # The verification below also uses some NocaseDict features, but that is
     # unavoidable if we want to work through the public interface:
 
     act_items = []
     for key in act_dict:  # Uses NocaseDict iteration
         act_value = act_dict[key]  # Uses NocaseDict getitem
-        assert key in exp_dict, "Unexpected extra key %r" % key
+        assert key in exp_dict, f"Unexpected extra key {key!r}"
         exp_value = exp_dict[key]
-        assert act_value == exp_value, "Unexpected value at key %r" % key
+        assert act_value == exp_value, f"Unexpected value at key {key!r}"
         act_items.append((key, act_value))
 
     exp_items = []
     for key in exp_dict:
         exp_value = exp_dict[key]
         # Next line uses NocaseDict contains:
-        assert key in act_dict, "Unexpected missing key %r" % key
+        assert key in act_dict, f"Unexpected missing key {key!r}"
         act_value = act_dict[key]  # Uses NocaseDict getitem
-        assert act_value == exp_value, "Unexpected value at key %r" % key
+        assert act_value == exp_value, f"Unexpected value at key {key!r}"
         exp_items.append((key, exp_value))
 
     if verify_order:
         assert act_items == exp_items, "Unexpected order of items"
 
 
 TESTCASES_NOCASEDICT_GETITEM = [
@@ -561,15 +561,15 @@
     # The code to be tested
     act_value = obj[key]
 
     # Ensure that exceptions raised in the remainder of this function
     # are not mistaken as expected exceptions
     assert testcase.exp_exc_types is None
 
-    assert act_value == exp_value, "Unexpected value at key %r" % key
+    assert act_value == exp_value, f"Unexpected value at key {key!r}"
 
 
 TESTCASES_NOCASEDICT_SETITEM = [
 
     # Testcases for NocaseDict.__setitem__() / ncd[key]=value
 
     # Each list item is a testcase tuple with these items:
@@ -704,15 +704,15 @@
     assert testcase.exp_exc_types is None
 
     # The verification below also uses some NocaseDict features, but that is
     # unavoidable if we want to work through the public interface:
 
     act_value = obj[key]  # Uses NocaseDIct getitem
 
-    assert act_value == value, "Unexpected value at key %r" % key
+    assert act_value == value, f"Unexpected value at key {key!r}"
 
 
 TESTCASES_NOCASEDICT_DELITEM = [
 
     # Testcases for NocaseDict.__delitem__() / del ncd[key]
 
     # Each list item is a testcase tuple with these items:
@@ -1024,16 +1024,15 @@
     # The code to be tested
     act_result = key in obj
 
     # Ensure that exceptions raised in the remainder of this function
     # are not mistaken as expected exceptions
     assert testcase.exp_exc_types is None
 
-    assert act_result == exp_result, \
-        "Unexpected result at key {k!r}".format(k=key)
+    assert act_result == exp_result, f"Unexpected result at key {key!r}"
 
 
 TESTCASES_NOCASEDICT_FROMKEYS = [
 
     # Testcases for NocaseDict.fromkeys()
 
     # Each list item is a testcase tuple with these items:
@@ -1880,16 +1879,16 @@
     # The code to be tested
     act_value = obj.setdefault(key, default)
 
     # Ensure that exceptions raised in the remainder of this function
     # are not mistaken as expected exceptions
     assert testcase.exp_exc_types is None
 
-    assert act_value == exp_value, "Unexpected value at key %r with " \
-                                   "default %r" % (key, default)
+    assert act_value == exp_value, \
+        f"Unexpected value at key {key!r} with default {default!r}"
 
 
 TESTCASES_NOCASEDICT_ITEMS = [
 
     # Testcases for NocaseDict.keys(), values(), items()
 
     # Each list item is a testcase tuple with these items:
@@ -2118,16 +2117,16 @@
     assert testcase.exp_exc_types is None
 
     if not TEST_AGAINST_DICT:
         assert re.match(r'^NocaseDict\(.*\)$', result)
 
     # Note: This only tests for existence of each item, not for excess items
     # or representing the correct order.
-    for item in obj.items():
-        exp_item_result = "{0!r}: {1!r}".format(*item)
+    for key, value in obj.items():
+        exp_item_result = f"{key!r}: {value!r}"
         assert exp_item_result in result
 
 
 TESTCASES_NOCASEDICT_UPDATE = [
 
     # Testcases for NocaseDict.update()
 
@@ -3050,15 +3049,15 @@
 @simplified_test_function
 def test_NocaseDict_ordering(testcase,
                              obj1, obj2, op, exp_result):
     """
     Test function for NocaseDict.__le__(), __lt__(), __ge__(), __gt__() / ord.
     """
 
-    comp_str = 'obj1 %s obj2' % op
+    comp_str = f'obj1 {op} obj2'
 
     # Double check they are different objects
     assert id(obj1) != id(obj2)
 
     # The code to be tested
     result = eval(comp_str)  # pylint: disable=eval-used
```

### Comparing `nocasedict-2.0.1/tests/utils/import_installed.py` & `nocasedict-2.0.2/tests/utils/import_installed.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,39 +45,39 @@
         dirpath = ''
         try:
             ix = sys.path.index(dirpath)
         except ValueError:
             ix = None
         if ix is not None:
             if test_installed == 'DEBUG':
-                print("Debug: Removing {0} at index {1} from module search "
-                      "path".format(dirpath, ix))
+                print(f"Debug: Removing {dirpath} at index {ix} from module "
+                      "search path")
             del sys.path[ix]
 
         # Move CWD to end. Reason is that when testing with an editable
         # installation, the CWD is needed, but when testing with a non-editable
         # installation, the package should not be found inthe CWD.
         # Note that somehow the CWD gets inserted at the begin of the search
         # path every time, so we need a loop.
         dirpath = os.getcwd()
         while True:
             try:
                 ix = sys.path.index(dirpath)
             except ValueError:
                 if test_installed == 'DEBUG':
-                    print("Debug: Appending {0} to end of module search "
-                          "path".format(dirpath))
+                    print(f"Debug: Appending {dirpath} to end of module "
+                          "search path")
                 sys.path.append(dirpath)
                 break
             if ix == len(sys.path) - 1:
                 # it exists once at the end
                 break
             if test_installed == 'DEBUG':
-                print("Debug: Removing {0} at index {1} from module search "
-                      "path".format(dirpath, ix))
+                print(f"Debug: Removing {dirpath} at index {ix} from module "
+                      "search path")
             del sys.path[ix]
 
     if module_name not in sys.modules:
         module = __import__(module_name, level=0)  # only absolute imports
         if test_installed == 'DEBUG':
             print("Debug: {0} module newly loaded from: {1}".
                   format(module_name, module.__file__))
```

### Comparing `nocasedict-2.0.1/tests/utils/simplified_test_function.py` & `nocasedict-2.0.2/tests/utils/simplified_test_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 simplified_test_function - Pytest extension for simplifying test functions.
 """
 
 from __future__ import absolute_import
 
 import functools
+import warnings
 from collections import namedtuple
 from inspect import Signature, Parameter  # type: ignore
 import pytest
 
 __all__ = ['simplified_test_function']
 
 
@@ -144,15 +145,15 @@
                         pdb.set_trace()
 
                     test_func(testcase, **kwargs)  # not expecting an exception
 
                     ret = None  # Debugging hint
                     assert len(rec_warnings) >= 1
         else:
-            with pytest.warns(None) as rec_warnings:
+            with warnings.catch_warnings(record=True) as rec_warnings:
                 if exp_exc_types:
                     with pytest.raises(exp_exc_types):
                         if condition == 'pdb':
                             # pylint: disable=forgotten-debug-statement
                             pdb.set_trace()
 
                         test_func(testcase, **kwargs)  # expecting an exception
@@ -166,15 +167,15 @@
                     test_func(testcase, **kwargs)  # not expecting an exception
 
                     ret = None  # Debugging hint
 
                     # Verify that no warnings have occurred
                     if exp_warn_types is None and rec_warnings:
                         lines = []
-                        for w in rec_warnings.list:
+                        for w in rec_warnings:
                             tup = (w.filename, w.lineno, w.category.__name__,
                                    str(w.message))
                             line = "{t[0]}:{t[1]}: {t[2]}: {t[3]}".format(t=tup)
                             if line not in lines:
                                 lines.append(line)
                         msg = "Unexpected warnings:\n{}".format(
                             '\n'.join(lines))
```

