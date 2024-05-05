# Comparing `tmp/nocaselist-2.0.0.tar.gz` & `tmp/nocaselist-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nocaselist-2.0.0.tar", last modified: Thu Jun  1 14:28:09 2023, max compression
+gzip compressed data, was "nocaselist-2.0.1.tar", last modified: Sun May  5 08:13:14 2024, max compression
```

## Comparing `nocaselist-2.0.0.tar` & `nocaselist-2.0.1.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-06-01 14:28:09.024378 nocaselist-2.0.0/
--rw-r--r--   0 maiera     (501) staff       (20)      424 2022-08-04 11:04:17.000000 nocaselist-2.0.0/INSTALL.md
--rw-r--r--   0 maiera     (501) staff       (20)    11357 2022-08-04 11:04:17.000000 nocaselist-2.0.0/LICENSE
--rw-r--r--   0 maiera     (501) staff       (20)      263 2023-06-01 14:28:08.000000 nocaselist-2.0.0/MANIFEST.in
--rw-r--r--   0 maiera     (501) staff       (20)     4242 2023-06-01 14:28:09.023658 nocaselist-2.0.0/PKG-INFO
--rw-r--r--   0 maiera     (501) staff       (20)     2976 2023-05-01 07:33:49.000000 nocaselist-2.0.0/README.rst
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-06-01 14:28:09.012162 nocaselist-2.0.0/nocaselist/
--rw-r--r--   0 maiera     (501) staff       (20)      191 2022-08-04 11:04:17.000000 nocaselist-2.0.0/nocaselist/__init__.py
--rw-r--r--   0 maiera     (501) staff       (20)    21704 2023-06-01 05:24:41.000000 nocaselist-2.0.0/nocaselist/_nocaselist.py
--rw-r--r--   0 maiera     (501) staff       (20)      326 2023-06-01 14:25:52.000000 nocaselist-2.0.0/nocaselist/_version.py
--rw-r--r--   0 maiera     (501) staff       (20)        0 2023-06-01 05:24:41.000000 nocaselist-2.0.0/nocaselist/py.typed
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-06-01 14:28:09.015369 nocaselist-2.0.0/nocaselist.egg-info/
--rw-r--r--   0 maiera     (501) staff       (20)     4242 2023-06-01 14:28:08.000000 nocaselist-2.0.0/nocaselist.egg-info/PKG-INFO
--rw-r--r--   0 maiera     (501) staff       (20)      619 2023-06-01 14:28:08.000000 nocaselist-2.0.0/nocaselist.egg-info/SOURCES.txt
--rw-r--r--   0 maiera     (501) staff       (20)        1 2023-06-01 14:28:08.000000 nocaselist-2.0.0/nocaselist.egg-info/dependency_links.txt
--rw-r--r--   0 maiera     (501) staff       (20)      195 2023-06-01 14:28:08.000000 nocaselist-2.0.0/nocaselist.egg-info/requires.txt
--rw-r--r--   0 maiera     (501) staff       (20)       11 2023-06-01 14:28:08.000000 nocaselist-2.0.0/nocaselist.egg-info/top_level.txt
--rw-r--r--   0 maiera     (501) staff       (20)        1 2023-06-01 14:28:08.000000 nocaselist-2.0.0/nocaselist.egg-info/zip-safe
--rw-r--r--   0 maiera     (501) staff       (20)      750 2023-06-01 05:24:41.000000 nocaselist-2.0.0/requirements.txt
--rw-r--r--   0 maiera     (501) staff       (20)       38 2023-06-01 14:28:09.024546 nocaselist-2.0.0/setup.cfg
--rwxr-xr-x   0 maiera     (501) staff       (20)     6647 2023-06-01 05:24:41.000000 nocaselist-2.0.0/setup.py
--rw-r--r--   0 maiera     (501) staff       (20)     1155 2023-06-01 05:24:41.000000 nocaselist-2.0.0/test-requirements.txt
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-06-01 14:28:09.015811 nocaselist-2.0.0/tests/
--rw-r--r--   0 maiera     (501) staff       (20)        0 2020-07-19 13:03:24.000000 nocaselist-2.0.0/tests/__init__.py
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-06-01 14:28:09.016300 nocaselist-2.0.0/tests/installtest/
--rwxr-xr-x   0 maiera     (501) staff       (20)    12821 2022-08-04 11:04:17.000000 nocaselist-2.0.0/tests/installtest/test_install.sh
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-06-01 14:28:09.020290 nocaselist-2.0.0/tests/unittest/
--rw-r--r--   0 maiera     (501) staff       (20)        0 2020-07-19 13:03:24.000000 nocaselist-2.0.0/tests/unittest/__init__.py
--rw-r--r--   0 maiera     (501) staff       (20)    85041 2023-06-01 05:24:41.000000 nocaselist-2.0.0/tests/unittest/test_nocaselist.py
--rw-r--r--   0 maiera     (501) staff       (20)      401 2020-07-19 13:03:24.000000 nocaselist-2.0.0/tests/unittest/test_package.py
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-06-01 14:28:09.022591 nocaselist-2.0.0/tests/utils/
--rw-r--r--   0 maiera     (501) staff       (20)        0 2020-07-21 04:12:03.000000 nocaselist-2.0.0/tests/utils/__init__.py
--rw-r--r--   0 maiera     (501) staff       (20)     3444 2022-08-04 11:04:17.000000 nocaselist-2.0.0/tests/utils/import_installed.py
--rw-r--r--   0 maiera     (501) staff       (20)     7138 2023-06-01 05:24:41.000000 nocaselist-2.0.0/tests/utils/simplified_test_function.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-05-05 08:13:14.020842 nocaselist-2.0.1/
+-rw-r--r--   0 maiera     (501) staff       (20)      182 2024-05-04 16:41:38.000000 nocaselist-2.0.1/AUTHORS.md
+-rw-r--r--   0 maiera     (501) staff       (20)      424 2022-08-04 11:04:17.000000 nocaselist-2.0.1/INSTALL.md
+-rw-r--r--   0 maiera     (501) staff       (20)    11357 2022-08-04 11:04:17.000000 nocaselist-2.0.1/LICENSE
+-rw-r--r--   0 maiera     (501) staff       (20)      262 2024-05-05 08:11:33.000000 nocaselist-2.0.1/MANIFEST.in
+-rw-r--r--   0 maiera     (501) staff       (20)     4404 2024-05-05 08:13:14.020323 nocaselist-2.0.1/PKG-INFO
+-rw-r--r--   0 maiera     (501) staff       (20)     2736 2024-05-05 08:11:22.000000 nocaselist-2.0.1/README.md
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-05-05 08:13:14.008436 nocaselist-2.0.1/nocaselist/
+-rw-r--r--   0 maiera     (501) staff       (20)      226 2024-05-04 16:11:26.000000 nocaselist-2.0.1/nocaselist/__init__.py
+-rw-r--r--   0 maiera     (501) staff       (20)    21739 2024-05-04 16:11:26.000000 nocaselist-2.0.1/nocaselist/_nocaselist.py
+-rw-r--r--   0 maiera     (501) staff       (20)      361 2024-05-04 17:01:48.000000 nocaselist-2.0.1/nocaselist/_version.py
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2023-08-22 06:44:32.000000 nocaselist-2.0.1/nocaselist/py.typed
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-05-05 08:13:14.018389 nocaselist-2.0.1/nocaselist.egg-info/
+-rw-r--r--   0 maiera     (501) staff       (20)     4404 2024-05-05 08:13:13.000000 nocaselist-2.0.1/nocaselist.egg-info/PKG-INFO
+-rw-r--r--   0 maiera     (501) staff       (20)      629 2024-05-05 08:13:13.000000 nocaselist-2.0.1/nocaselist.egg-info/SOURCES.txt
+-rw-r--r--   0 maiera     (501) staff       (20)        1 2024-05-05 08:13:13.000000 nocaselist-2.0.1/nocaselist.egg-info/dependency_links.txt
+-rw-r--r--   0 maiera     (501) staff       (20)      201 2024-05-05 08:13:13.000000 nocaselist-2.0.1/nocaselist.egg-info/requires.txt
+-rw-r--r--   0 maiera     (501) staff       (20)       11 2024-05-05 08:13:13.000000 nocaselist-2.0.1/nocaselist.egg-info/top_level.txt
+-rw-r--r--   0 maiera     (501) staff       (20)        1 2024-05-05 08:13:13.000000 nocaselist-2.0.1/nocaselist.egg-info/zip-safe
+-rw-r--r--   0 maiera     (501) staff       (20)      750 2023-08-22 06:44:32.000000 nocaselist-2.0.1/requirements.txt
+-rw-r--r--   0 maiera     (501) staff       (20)       38 2024-05-05 08:13:14.020978 nocaselist-2.0.1/setup.cfg
+-rwxr-xr-x   0 maiera     (501) staff       (20)     6681 2024-05-04 16:29:08.000000 nocaselist-2.0.1/setup.py
+-rw-r--r--   0 maiera     (501) staff       (20)     1231 2023-08-22 06:48:32.000000 nocaselist-2.0.1/test-requirements.txt
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-05-05 08:13:14.012699 nocaselist-2.0.1/tests/
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2020-07-19 13:03:24.000000 nocaselist-2.0.1/tests/__init__.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-05-05 08:13:14.013127 nocaselist-2.0.1/tests/installtest/
+-rwxr-xr-x   0 maiera     (501) staff       (20)    11906 2024-05-04 16:11:26.000000 nocaselist-2.0.1/tests/installtest/test_install.sh
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-05-05 08:13:14.015957 nocaselist-2.0.1/tests/unittest/
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2020-07-19 13:03:24.000000 nocaselist-2.0.1/tests/unittest/__init__.py
+-rw-r--r--   0 maiera     (501) staff       (20)    85076 2024-05-04 16:11:26.000000 nocaselist-2.0.1/tests/unittest/test_nocaselist.py
+-rw-r--r--   0 maiera     (501) staff       (20)      436 2024-05-04 16:11:26.000000 nocaselist-2.0.1/tests/unittest/test_package.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-05-05 08:13:14.017591 nocaselist-2.0.1/tests/utils/
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2020-07-21 04:12:03.000000 nocaselist-2.0.1/tests/utils/__init__.py
+-rw-r--r--   0 maiera     (501) staff       (20)     3479 2024-05-04 16:11:26.000000 nocaselist-2.0.1/tests/utils/import_installed.py
+-rw-r--r--   0 maiera     (501) staff       (20)     7202 2024-05-04 16:11:26.000000 nocaselist-2.0.1/tests/utils/simplified_test_function.py
```

### Comparing `nocaselist-2.0.0/LICENSE` & `nocaselist-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nocaselist-2.0.0/PKG-INFO` & `nocaselist-2.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nocaselist
-Version: 2.0.0
+Version: 2.0.1
 Summary: A case-insensitive list for Python
 Home-page: https://github.com/pywbem/nocaselist
 Author: Andreas Maier
 Author-email: andreas.r.maier@gmx.de
 Maintainer: Andreas Maier
 Maintainer-email: andreas.r.maier@gmx.de
 License: Apache Software License 2.0
@@ -22,106 +22,88 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
-Provides-Extra: test
 License-File: LICENSE
-
-nocaselist - A case-insensitive list for Python
-===============================================
-
-.. image:: https://badge.fury.io/py/nocaselist.svg
-    :target: https://pypi.python.org/pypi/nocaselist/
-    :alt: Version on Pypi
-
-.. image:: https://github.com/pywbem/nocaselist/workflows/test/badge.svg?branch=master
-    :target: https://github.com/pywbem/nocaselist/actions/
-    :alt: Actions status
-
-.. image:: https://readthedocs.org/projects/nocaselist/badge/?version=latest
-    :target: https://readthedocs.org/projects/nocaselist/builds/
-    :alt: Docs build status (master)
-
-.. image:: https://coveralls.io/repos/github/pywbem/nocaselist/badge.svg?branch=master
-    :target: https://coveralls.io/github/pywbem/nocaselist?branch=master
-    :alt: Test coverage (master)
-
-
-Overview
---------
-
-Class `NocaseList`_ is a case-insensitive list that preserves the lexical case
-of its items.
+License-File: AUTHORS.md
+Requires-Dist: typing-extensions<4.2.0,>=3.10; python_version == "3.6"
+Requires-Dist: typing-extensions>=3.10; python_version >= "3.7"
+Provides-Extra: test
+Requires-Dist: pytest>=7.0.0; extra == "test"
+Requires-Dist: virtualenv>=20.1.0; extra == "test"
+Requires-Dist: six>=1.14.0; extra == "test"
+Requires-Dist: packaging<22.0,>=21.0; extra == "test"
+Requires-Dist: pluggy>=0.13.1; extra == "test"
+
+# nocaselist - A case-insensitive list for Python
+
+[![Version on Pypi](https://img.shields.io/pypi/v/nocaselist.svg)](https://pypi.python.org/pypi/nocaselist/)
+[![Test status (master)](https://github.com/pywbem/nocaselist/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/pywbem/nocaselist/actions/workflows/test.yml?query=branch%3Amaster)
+[![Docs status (master)](https://readthedocs.org/projects/nocaselist/badge/?version=latest)](https://readthedocs.org/projects/nocaselist/builds/)
+[![Test coverage (master)](https://coveralls.io/repos/github/pywbem/nocaselist/badge.svg?branch=master)](https://coveralls.io/github/pywbem/nocaselist?branch=master)
+
+# Overview
+
+Class
+[NocaseList](https://nocaselist.readthedocs.io/en/stable/reference.html#nocaselist.NocaseList)
+is a case-insensitive list that preserves the lexical case of its items.
 
 Example:
 
-.. code-block:: bash
-
     $ python
     >>> from nocaselist import NocaseList
 
     >>> list1 = NocaseList(['Alpha', 'Beta'])
 
     >>> print(list1)  # Any access is case-preserving
     ['Alpha', 'Beta']
 
     >>> 'ALPHA' in list1  # Any lookup or comparison is case-insensitive
     True
 
-The `NocaseList`_ class supports the functionality of the built-in
-`list class of Python 3.8`_ on all Python versions it supports (except for being
-case-insensitive, of course).
-
-.. _list class of Python 3.8: https://docs.python.org/3.8/library/stdtypes.html#list
-.. _NocaseList: https://nocaselist.readthedocs.io/en/stable/reference.html#nocaselist.NocaseList
+The
+[NocaseList](https://nocaselist.readthedocs.io/en/stable/reference.html#nocaselist.NocaseList)
+class supports the functionality of the built-in
+[list class of Python 3.8](https://docs.python.org/3.8/library/stdtypes.html#list)
+on all Python versions it supports (except for being case-insensitive, of
+course).
 
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
 
+# Installation
 
-Installation
-------------
-
-To install the latest released version of the nocaselist package into your
-active Python environment:
-
-.. code-block:: bash
+To install the latest released version of the nocaselist package into
+your active Python environment:
 
     $ pip install nocaselist
 
 The nocaselist package has no prerequisite Python packages.
 
-For more details and alternative ways to install, see `Installation`_.
+For more details and alternative ways to install, see
+[Installation](https://nocaselist.readthedocs.io/en/stable/intro.html#installation).
 
-.. _Installation: https://nocaselist.readthedocs.io/en/stable/intro.html#installation
+# Documentation
 
-Documentation
--------------
+- [Documentation](https://nocaselist.readthedocs.io/en/stable/)
 
-* `Documentation <https://nocaselist.readthedocs.io/en/stable/>`_
+# Change History
 
-Change History
---------------
+- [Change history](https://nocaselist.readthedocs.io/en/stable/changes.html)
 
-* `Change history <https://nocaselist.readthedocs.io/en/stable/changes.html>`_
-
-Contributing
-------------
+# Contributing
 
 For information on how to contribute to the nocaselist project, see
-`Contributing <https://nocaselist.readthedocs.io/en/stable/development.html#contributing>`_.
-
+[Contributing](https://nocaselist.readthedocs.io/en/stable/development.html#contributing).
 
-License
--------
+# License
 
-The nocaselist project is provided under the
-`Apache Software License 2.0 <https://raw.githubusercontent.com/pywbem/nocaselist/master/LICENSE>`_.
+The nocaselist project is provided under the [Apache Software License
+2.0](https://raw.githubusercontent.com/pywbem/nocaselist/master/LICENSE).
```

### Comparing `nocaselist-2.0.0/README.rst` & `nocaselist-2.0.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,96 +1,70 @@
-nocaselist - A case-insensitive list for Python
-===============================================
+# nocaselist - A case-insensitive list for Python
 
-.. image:: https://badge.fury.io/py/nocaselist.svg
-    :target: https://pypi.python.org/pypi/nocaselist/
-    :alt: Version on Pypi
-
-.. image:: https://github.com/pywbem/nocaselist/workflows/test/badge.svg?branch=master
-    :target: https://github.com/pywbem/nocaselist/actions/
-    :alt: Actions status
-
-.. image:: https://readthedocs.org/projects/nocaselist/badge/?version=latest
-    :target: https://readthedocs.org/projects/nocaselist/builds/
-    :alt: Docs build status (master)
-
-.. image:: https://coveralls.io/repos/github/pywbem/nocaselist/badge.svg?branch=master
-    :target: https://coveralls.io/github/pywbem/nocaselist?branch=master
-    :alt: Test coverage (master)
-
-
-Overview
---------
-
-Class `NocaseList`_ is a case-insensitive list that preserves the lexical case
-of its items.
+[![Version on Pypi](https://img.shields.io/pypi/v/nocaselist.svg)](https://pypi.python.org/pypi/nocaselist/)
+[![Test status (master)](https://github.com/pywbem/nocaselist/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/pywbem/nocaselist/actions/workflows/test.yml?query=branch%3Amaster)
+[![Docs status (master)](https://readthedocs.org/projects/nocaselist/badge/?version=latest)](https://readthedocs.org/projects/nocaselist/builds/)
+[![Test coverage (master)](https://coveralls.io/repos/github/pywbem/nocaselist/badge.svg?branch=master)](https://coveralls.io/github/pywbem/nocaselist?branch=master)
+
+# Overview
+
+Class
+[NocaseList](https://nocaselist.readthedocs.io/en/stable/reference.html#nocaselist.NocaseList)
+is a case-insensitive list that preserves the lexical case of its items.
 
 Example:
 
-.. code-block:: bash
-
     $ python
     >>> from nocaselist import NocaseList
 
     >>> list1 = NocaseList(['Alpha', 'Beta'])
 
     >>> print(list1)  # Any access is case-preserving
     ['Alpha', 'Beta']
 
     >>> 'ALPHA' in list1  # Any lookup or comparison is case-insensitive
     True
 
-The `NocaseList`_ class supports the functionality of the built-in
-`list class of Python 3.8`_ on all Python versions it supports (except for being
-case-insensitive, of course).
-
-.. _list class of Python 3.8: https://docs.python.org/3.8/library/stdtypes.html#list
-.. _NocaseList: https://nocaselist.readthedocs.io/en/stable/reference.html#nocaselist.NocaseList
+The
+[NocaseList](https://nocaselist.readthedocs.io/en/stable/reference.html#nocaselist.NocaseList)
+class supports the functionality of the built-in
+[list class of Python 3.8](https://docs.python.org/3.8/library/stdtypes.html#list)
+on all Python versions it supports (except for being case-insensitive, of
+course).
 
 The case-insensitivity is achieved by matching any key values as their
 casefolded values. By default, the casefolding is performed with
-`str.casefold()`_ for unicode string keys and with `bytes.lower()`_ for byte
-string keys.
-The default casefolding can be overridden with a user-defined casefold method.
-
-.. _str.casefold(): https://docs.python.org/3/library/stdtypes.html#str.casefold
-.. _bytes.lower(): https://docs.python.org/3/library/stdtypes.html#bytes.lower
-
+[str.casefold()](https://docs.python.org/3/library/stdtypes.html#str.casefold)
+for unicode string keys and with
+[bytes.lower()](https://docs.python.org/3/library/stdtypes.html#bytes.lower)
+for byte string keys. The default casefolding can be overridden with a
+user-defined casefold method.
 
-Installation
-------------
+# Installation
 
-To install the latest released version of the nocaselist package into your
-active Python environment:
-
-.. code-block:: bash
+To install the latest released version of the nocaselist package into
+your active Python environment:
 
     $ pip install nocaselist
 
 The nocaselist package has no prerequisite Python packages.
 
-For more details and alternative ways to install, see `Installation`_.
-
-.. _Installation: https://nocaselist.readthedocs.io/en/stable/intro.html#installation
+For more details and alternative ways to install, see
+[Installation](https://nocaselist.readthedocs.io/en/stable/intro.html#installation).
 
-Documentation
--------------
+# Documentation
 
-* `Documentation <https://nocaselist.readthedocs.io/en/stable/>`_
+- [Documentation](https://nocaselist.readthedocs.io/en/stable/)
 
-Change History
---------------
+# Change History
 
-* `Change history <https://nocaselist.readthedocs.io/en/stable/changes.html>`_
+- [Change history](https://nocaselist.readthedocs.io/en/stable/changes.html)
 
-Contributing
-------------
+# Contributing
 
 For information on how to contribute to the nocaselist project, see
-`Contributing <https://nocaselist.readthedocs.io/en/stable/development.html#contributing>`_.
-
+[Contributing](https://nocaselist.readthedocs.io/en/stable/development.html#contributing).
 
-License
--------
+# License
 
-The nocaselist project is provided under the
-`Apache Software License 2.0 <https://raw.githubusercontent.com/pywbem/nocaselist/master/LICENSE>`_.
+The nocaselist project is provided under the [Apache Software License
+2.0](https://raw.githubusercontent.com/pywbem/nocaselist/master/LICENSE).
```

### Comparing `nocaselist-2.0.0/nocaselist/_nocaselist.py` & `nocaselist-2.0.1/nocaselist/_nocaselist.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Copyright (C) 2020 Andreas Maier
 """
 This module provides class NocaseList.
 """
 
 import sys
 import os
 from typing import Callable, AnyStr, Optional, Union
```

### Comparing `nocaselist-2.0.0/nocaselist.egg-info/PKG-INFO` & `nocaselist-2.0.1/nocaselist.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nocaselist
-Version: 2.0.0
+Version: 2.0.1
 Summary: A case-insensitive list for Python
 Home-page: https://github.com/pywbem/nocaselist
 Author: Andreas Maier
 Author-email: andreas.r.maier@gmx.de
 Maintainer: Andreas Maier
 Maintainer-email: andreas.r.maier@gmx.de
 License: Apache Software License 2.0
@@ -22,106 +22,88 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
-Provides-Extra: test
 License-File: LICENSE
-
-nocaselist - A case-insensitive list for Python
-===============================================
-
-.. image:: https://badge.fury.io/py/nocaselist.svg
-    :target: https://pypi.python.org/pypi/nocaselist/
-    :alt: Version on Pypi
-
-.. image:: https://github.com/pywbem/nocaselist/workflows/test/badge.svg?branch=master
-    :target: https://github.com/pywbem/nocaselist/actions/
-    :alt: Actions status
-
-.. image:: https://readthedocs.org/projects/nocaselist/badge/?version=latest
-    :target: https://readthedocs.org/projects/nocaselist/builds/
-    :alt: Docs build status (master)
-
-.. image:: https://coveralls.io/repos/github/pywbem/nocaselist/badge.svg?branch=master
-    :target: https://coveralls.io/github/pywbem/nocaselist?branch=master
-    :alt: Test coverage (master)
-
-
-Overview
---------
-
-Class `NocaseList`_ is a case-insensitive list that preserves the lexical case
-of its items.
+License-File: AUTHORS.md
+Requires-Dist: typing-extensions<4.2.0,>=3.10; python_version == "3.6"
+Requires-Dist: typing-extensions>=3.10; python_version >= "3.7"
+Provides-Extra: test
+Requires-Dist: pytest>=7.0.0; extra == "test"
+Requires-Dist: virtualenv>=20.1.0; extra == "test"
+Requires-Dist: six>=1.14.0; extra == "test"
+Requires-Dist: packaging<22.0,>=21.0; extra == "test"
+Requires-Dist: pluggy>=0.13.1; extra == "test"
+
+# nocaselist - A case-insensitive list for Python
+
+[![Version on Pypi](https://img.shields.io/pypi/v/nocaselist.svg)](https://pypi.python.org/pypi/nocaselist/)
+[![Test status (master)](https://github.com/pywbem/nocaselist/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/pywbem/nocaselist/actions/workflows/test.yml?query=branch%3Amaster)
+[![Docs status (master)](https://readthedocs.org/projects/nocaselist/badge/?version=latest)](https://readthedocs.org/projects/nocaselist/builds/)
+[![Test coverage (master)](https://coveralls.io/repos/github/pywbem/nocaselist/badge.svg?branch=master)](https://coveralls.io/github/pywbem/nocaselist?branch=master)
+
+# Overview
+
+Class
+[NocaseList](https://nocaselist.readthedocs.io/en/stable/reference.html#nocaselist.NocaseList)
+is a case-insensitive list that preserves the lexical case of its items.
 
 Example:
 
-.. code-block:: bash
-
     $ python
     >>> from nocaselist import NocaseList
 
     >>> list1 = NocaseList(['Alpha', 'Beta'])
 
     >>> print(list1)  # Any access is case-preserving
     ['Alpha', 'Beta']
 
     >>> 'ALPHA' in list1  # Any lookup or comparison is case-insensitive
     True
 
-The `NocaseList`_ class supports the functionality of the built-in
-`list class of Python 3.8`_ on all Python versions it supports (except for being
-case-insensitive, of course).
-
-.. _list class of Python 3.8: https://docs.python.org/3.8/library/stdtypes.html#list
-.. _NocaseList: https://nocaselist.readthedocs.io/en/stable/reference.html#nocaselist.NocaseList
+The
+[NocaseList](https://nocaselist.readthedocs.io/en/stable/reference.html#nocaselist.NocaseList)
+class supports the functionality of the built-in
+[list class of Python 3.8](https://docs.python.org/3.8/library/stdtypes.html#list)
+on all Python versions it supports (except for being case-insensitive, of
+course).
 
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
 
+# Installation
 
-Installation
-------------
-
-To install the latest released version of the nocaselist package into your
-active Python environment:
-
-.. code-block:: bash
+To install the latest released version of the nocaselist package into
+your active Python environment:
 
     $ pip install nocaselist
 
 The nocaselist package has no prerequisite Python packages.
 
-For more details and alternative ways to install, see `Installation`_.
+For more details and alternative ways to install, see
+[Installation](https://nocaselist.readthedocs.io/en/stable/intro.html#installation).
 
-.. _Installation: https://nocaselist.readthedocs.io/en/stable/intro.html#installation
+# Documentation
 
-Documentation
--------------
+- [Documentation](https://nocaselist.readthedocs.io/en/stable/)
 
-* `Documentation <https://nocaselist.readthedocs.io/en/stable/>`_
+# Change History
 
-Change History
---------------
+- [Change history](https://nocaselist.readthedocs.io/en/stable/changes.html)
 
-* `Change history <https://nocaselist.readthedocs.io/en/stable/changes.html>`_
-
-Contributing
-------------
+# Contributing
 
 For information on how to contribute to the nocaselist project, see
-`Contributing <https://nocaselist.readthedocs.io/en/stable/development.html#contributing>`_.
-
+[Contributing](https://nocaselist.readthedocs.io/en/stable/development.html#contributing).
 
-License
--------
+# License
 
-The nocaselist project is provided under the
-`Apache Software License 2.0 <https://raw.githubusercontent.com/pywbem/nocaselist/master/LICENSE>`_.
+The nocaselist project is provided under the [Apache Software License
+2.0](https://raw.githubusercontent.com/pywbem/nocaselist/master/LICENSE).
```

### Comparing `nocaselist-2.0.0/nocaselist.egg-info/SOURCES.txt` & `nocaselist-2.0.1/nocaselist.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

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
 nocaselist/__init__.py
 nocaselist/_nocaselist.py
 nocaselist/_version.py
 nocaselist/py.typed
```

### Comparing `nocaselist-2.0.0/requirements.txt` & `nocaselist-2.0.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `nocaselist-2.0.0/setup.py` & `nocaselist-2.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python
+# Copyright (C) 2020 Andreas Maier
 """
 Python setup script for the nocaselist project.
 """
 
 import sys
 import os
 import io
@@ -166,15 +167,15 @@
     extras_require={
         "test": test_requirements,
     },
     cmdclass={
         'test': test,
     },
     description="A case-insensitive list for Python",
-    long_description=read_file('README.rst'),
+    long_description=read_file('README.md'),
     long_description_content_type='text/x-rst',
     license="Apache Software License 2.0",
     author="Andreas Maier",
     author_email='andreas.r.maier@gmx.de',
     maintainer="Andreas Maier",
     maintainer_email='andreas.r.maier@gmx.de',
     url='https://github.com/pywbem/nocaselist',
```

### Comparing `nocaselist-2.0.0/test-requirements.txt` & `nocaselist-2.0.1/test-requirements.txt`

 * *Files 22% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 # tox 3.17 requires six>=1.14.0
 six>=1.14.0
 
 
 # Indirect dependencies with special constraints:
 
 # packaging (used by pytest)
-packaging>=17.0
+# safety 2.3.5 started pinning packaging to <22.0 and requires >=21.0
+packaging>=21.0,<22.0
 
 # pluggy (used by pytest, tox)
 # Pluggy 0.12.0 has a bug causing pytest plugins to fail loading on py38
 # pytest 4.3.1 depends on pluggy>=0.7
 # tox 3.21.0 depends on pluggy>=0.12.0
 pluggy>=0.13.1
```

### Comparing `nocaselist-2.0.0/tests/installtest/test_install.sh` & `nocaselist-2.0.1/tests/installtest/test_install.sh`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/bin/bash
+# Copyright (C) 2020 Andreas Maier
 #
 # Test the installation of the package.
 #
 # This script can be run from any directory.
 
 DEBUG="false"
 VERBOSE="true"
@@ -411,67 +412,43 @@
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
 
@@ -495,15 +472,13 @@
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

### Comparing `nocaselist-2.0.0/tests/unittest/test_nocaselist.py` & `nocaselist-2.0.1/tests/unittest/test_nocaselist.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Copyright (C) 2020 Andreas Maier
 """
 Test the NocaseList class.
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `nocaselist-2.0.0/tests/utils/import_installed.py` & `nocaselist-2.0.1/tests/utils/import_installed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Copyright (C) 2020 Andreas Maier
 """
 import_installed - Utility function for testing the installed version of the
 package.
 """
 
 from __future__ import absolute_import, print_function
```

### Comparing `nocaselist-2.0.0/tests/utils/simplified_test_function.py` & `nocaselist-2.0.1/tests/utils/simplified_test_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+# Copyright (C) 2020 Andreas Maier
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
 
 
@@ -144,15 +146,15 @@
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
@@ -166,15 +168,15 @@
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

