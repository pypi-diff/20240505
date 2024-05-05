# Comparing `tmp/atpbar-1.1.4.tar.gz` & `tmp/atpbar-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atpbar-1.1.4.tar", last modified: Sat May  8 18:51:16 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `atpbar-1.1.4.tar` & `atpbar-2.0.0.tar`

### file list

```diff
@@ -1,56 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-08 18:51:16.621011 atpbar-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1487 2021-05-08 18:51:07.000000 atpbar-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       65 2021-05-08 18:51:07.000000 atpbar-1.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    21194 2021-05-08 18:51:16.621011 atpbar-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    16532 2021-05-08 18:51:07.000000 atpbar-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-08 18:51:16.621011 atpbar-1.1.4/atpbar/
--rw-r--r--   0 runner    (1001) docker     (121)      366 2021-05-08 18:51:07.000000 atpbar-1.1.4/atpbar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2021-05-08 18:51:16.621011 atpbar-1.1.4/atpbar/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     2343 2021-05-08 18:51:07.000000 atpbar-1.1.4/atpbar/funcs.py
--rw-r--r--   0 runner    (1001) docker     (121)     4359 2021-05-08 18:51:07.000000 atpbar-1.1.4/atpbar/machine.py
--rw-r--r--   0 runner    (1001) docker     (121)     3419 2021-05-08 18:51:07.000000 atpbar-1.1.4/atpbar/main.py
--rw-r--r--   0 runner    (1001) docker     (121)      329 2021-05-08 18:51:07.000000 atpbar-1.1.4/atpbar/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2291 2021-05-08 18:51:07.000000 atpbar-1.1.4/atpbar/pickup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-08 18:51:16.617011 atpbar-1.1.4/atpbar/presentation/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-08 18:51:07.000000 atpbar-1.1.4/atpbar/presentation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3779 2021-05-08 18:51:07.000000 atpbar-1.1.4/atpbar/presentation/barjupyter.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2817 2021-05-08 18:51:07.000000 atpbar-1.1.4/atpbar/presentation/bartty.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3071 2021-05-08 18:51:07.000000 atpbar-1.1.4/atpbar/presentation/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      889 2021-05-08 18:51:07.000000 atpbar-1.1.4/atpbar/presentation/create.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-08 18:51:16.617011 atpbar-1.1.4/atpbar/presentation/detect/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-08 18:51:07.000000 atpbar-1.1.4/atpbar/presentation/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      915 2021-05-08 18:51:07.000000 atpbar-1.1.4/atpbar/presentation/detect/jupy.py
--rw-r--r--   0 runner    (1001) docker     (121)      949 2021-05-08 18:51:07.000000 atpbar-1.1.4/atpbar/presentation/detect/spy.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1696 2021-05-08 18:51:07.000000 atpbar-1.1.4/atpbar/presentation/txtprint.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2349 2021-05-08 18:51:07.000000 atpbar-1.1.4/atpbar/report.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2648 2021-05-08 18:51:07.000000 atpbar-1.1.4/atpbar/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-08 18:51:16.617011 atpbar-1.1.4/atpbar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    21194 2021-05-08 18:51:16.000000 atpbar-1.1.4/atpbar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1321 2021-05-08 18:51:16.000000 atpbar-1.1.4/atpbar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-08 18:51:16.000000 atpbar-1.1.4/atpbar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-05-08 18:51:16.000000 atpbar-1.1.4/atpbar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-05-08 18:51:16.000000 atpbar-1.1.4/atpbar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      198 2021-05-08 18:51:16.621011 atpbar-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1277 2021-05-08 18:51:07.000000 atpbar-1.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-08 18:51:16.613011 atpbar-1.1.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-08 18:51:16.617011 atpbar-1.1.4/tests/presentation/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-08 18:51:07.000000 atpbar-1.1.4/tests/presentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-08 18:51:16.617011 atpbar-1.1.4/tests/presentation/detect/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-08 18:51:07.000000 atpbar-1.1.4/tests/presentation/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1789 2021-05-08 18:51:07.000000 atpbar-1.1.4/tests/presentation/detect/test_is_jupyter_notebook.py
--rw-r--r--   0 runner    (1001) docker     (121)     2381 2021-05-08 18:51:07.000000 atpbar-1.1.4/tests/presentation/detect/test_is_spyder_ide.py
--rw-r--r--   0 runner    (1001) docker     (121)      965 2021-05-08 18:51:07.000000 atpbar-1.1.4/tests/presentation/test_ProgressPrint.py
--rw-r--r--   0 runner    (1001) docker     (121)     6096 2021-05-08 18:51:07.000000 atpbar-1.1.4/tests/presentation/test_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2401 2021-05-08 18:51:07.000000 atpbar-1.1.4/tests/presentation/test_create_presentation.py
--rw-r--r--   0 runner    (1001) docker     (121)      298 2021-05-08 18:51:07.000000 atpbar-1.1.4/tests/presentation/test_is_jupyter_notebook.py
--rw-r--r--   0 runner    (1001) docker     (121)     1568 2021-05-08 18:51:07.000000 atpbar-1.1.4/tests/presentation/test_presentation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-08 18:51:16.617011 atpbar-1.1.4/tests/scenarios/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-08 18:51:07.000000 atpbar-1.1.4/tests/scenarios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2461 2021-05-08 18:51:07.000000 atpbar-1.1.4/tests/scenarios/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     3526 2021-05-08 18:51:07.000000 atpbar-1.1.4/tests/scenarios/test_disable.py
--rw-r--r--   0 runner    (1001) docker     (121)     1950 2021-05-08 18:51:07.000000 atpbar-1.1.4/tests/scenarios/test_last_report.py
--rw-r--r--   0 runner    (1001) docker     (121)     4281 2021-05-08 18:51:07.000000 atpbar-1.1.4/tests/scenarios/test_multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1947 2021-05-08 18:51:07.000000 atpbar-1.1.4/tests/scenarios/test_readme_mantichora.py
--rw-r--r--   0 runner    (1001) docker     (121)     5060 2021-05-08 18:51:07.000000 atpbar-1.1.4/tests/scenarios/test_readme_quick_start.py
--rw-r--r--   0 runner    (1001) docker     (121)     5032 2021-05-08 18:51:07.000000 atpbar-1.1.4/tests/scenarios/test_threading.py
--rw-r--r--   0 runner    (1001) docker     (121)    68611 2021-05-08 18:51:07.000000 atpbar-1.1.4/versioneer.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/__about__.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/__init__.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/funcs.py
+-rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/machine.py
+-rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/py.typed
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/stream.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/presentation/__init__.py
+-rwxr-xr-x   0        0        0     3692 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/presentation/barjupyter.py
+-rwxr-xr-x   0        0        0     3470 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/presentation/bartty.py
+-rwxr-xr-x   0        0        0     3140 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/presentation/base.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/presentation/create.py
+-rwxr-xr-x   0        0        0     1689 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/presentation/txtprint.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/presentation/detect/__init__.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/presentation/detect/jupy.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/presentation/detect/spy.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/progressreport/__init__.py
+-rwxr-xr-x   0        0        0     1527 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/progressreport/complement.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/progressreport/pickup.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/progressreport/report.py
+-rwxr-xr-x   0        0        0     2895 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/progressreport/reporter.py
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 atpbar-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 atpbar-2.0.0/LICENSE
+-rw-r--r--   0        0        0    15398 2020-02-02 00:00:00.000000 atpbar-2.0.0/README.md
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 atpbar-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    16356 2020-02-02 00:00:00.000000 atpbar-2.0.0/PKG-INFO
```

### Comparing `atpbar-1.1.4/LICENSE` & `atpbar-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `atpbar-1.1.4/README.md` & `atpbar-2.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,354 +1,354 @@
-[![PyPI version](https://badge.fury.io/py/atpbar.svg)](https://badge.fury.io/py/atpbar) 
-[![Anaconda-Server Badge](https://anaconda.org/conda-forge/atpbar/badges/version.svg)](https://anaconda.org/conda-forge/atpbar) 
-[![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.2567283.svg)](https://doi.org/10.5281/zenodo.2567283) 
-[![Test Status](https://github.com/alphatwirl/atpbar/workflows/Test/badge.svg)](https://github.com/alphatwirl/atpbar/actions?query=workflow%3ATest)
+[![PyPI version](https://badge.fury.io/py/atpbar.svg)](https://badge.fury.io/py/atpbar)
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/atpbar/badges/version.svg)](https://anaconda.org/conda-forge/atpbar)
+[![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.2567283.svg)](https://doi.org/10.5281/zenodo.2567283)
+
+[![Test Status](https://github.com/alphatwirl/atpbar/actions/workflows/unit-test.yml/badge.svg)](https://github.com/alphatwirl/atpbar/actions/workflows/unit-test.yml)
+[![Test Status](https://github.com/alphatwirl/atpbar/actions/workflows/type-check.yml/badge.svg)](https://github.com/alphatwirl/atpbar/actions/workflows/type-check.yml)
 [![codecov](https://codecov.io/gh/alphatwirl/atpbar/branch/master/graph/badge.svg)](https://codecov.io/gh/alphatwirl/atpbar)
 
 # atpbar
 
-_Progress bars_ for threading and multiprocessing tasks on terminal
-and Jupyter Notebook.
+_Progress bars_ for threading and multiprocessing tasks on the terminal and
+Jupyter Notebook.
 
-```
+```plaintext
  100.00% :::::::::::::::::::::::::::::::::::::::: |     7811 /     7811 |:  task 1
  100.00% :::::::::::::::::::::::::::::::::::::::: |    23258 /    23258 |:  task 0
   65.62% ::::::::::::::::::::::::::               |     8018 /    12219 |:  task 4
   60.89% ::::::::::::::::::::::::                 |    31083 /    51048 |:  task 2
   25.03% ::::::::::                               |    23884 /    95421 |:  task 3
 ```
-  
-_atpbar_ can display multiple progress bars simultaneously growing to
-show the progresses of iterations of loops in
+
+_atpbar_ can display multiple progress bars simultaneously growing to show the
+progress of each iteration of loops in
 [threading](https://docs.python.org/3/library/threading.html) or
 [multiprocessing](https://docs.python.org/3/library/multiprocessing.html)
-tasks. _atpbar_ can display progress bars on terminal and [Jupyter
-Notebook](https://jupyter.org/). _atpbar_ can be used with
-[_Mantichora_](https://github.com/alphatwirl/mantichora).
-
-_atpbar_ started its development in 2015 as part of
-[_alphatwirl_](https://github.com/alphatwirl/alphatwirl). _atpbar_
-prevented physicists from terminating their running analysis codes,
-which would take many hours to complete, by showing progress bars
-indicating their codes were actually running. The progress bars have
-saved the physicists countless hours total. _atpbar_ had been the
-sub-package
-[_progressbar_](https://github.com/alphatwirl/alphatwirl/tree/v0.22.0/alphatwirl/progressbar)
-of alphatwirl until it became an independent package, with the name
-_atpbar_, in February 2019.
+tasks. _atpbar_ can display progress bars on the terminal and [Jupyter
+Notebook](https://jupyter.org/).
 
+_atpbar_ started its development in 2015 and was the sub-package
+[_progressbar_](https://github.com/alphatwirl/alphatwirl/tree/v0.22.0/alphatwirl/progressbar)
+of alphatwirl. It became an independent package in 2019.
 
-You can try it on Jupyter Notebook online: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/alphatwirl/notebook-atpbar-001/master?filepath=atpbar.ipynb)
+You can try it on Jupyter Notebook online:
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/alphatwirl/notebook-atpbar-001/master?filepath=atpbar.ipynb)
 
-*****
+---
 
-- [**Requirement**](#requirement)
-- [**Install**](#install)
-- [**User guide**](#user-guide)
-    - [**Quick start**](#quick-start)
-        - [Import libraries](#import-libraries)
-        - [One loop](#one-loop)
-        - [Nested loops](#nested-loops)
-        - [Threading](#threading)
-        - [Multiprocessing](#multiprocessing)
-        - [With Mantichora](#with-mantichora)
-    - [**Features**](#features)
-        - [A `break` and an exception](#a-break-and-an-exception)
-        - [Progress of starting threads and processes with progress bars](#progress-of-starting-threads-and-processes-with-progress-bars)
-        - [On Jupyter Notebook](#on-jupyter-notebook)
-        - [Non TTY device](#non-tty-device)
-        - [How to disable progress bars](#how-to-disable-progress-bars)
-- [**License**](#license)
-- [**Contact**](#contact)
+- [Requirement](#requirement)
+- [Install](#install)
+- [User guide](#user-guide)
+- [Quick start](#quick-start)
+  - [Import libraries](#import-libraries)
+  - [One loop](#one-loop)
+  - [Nested loops](#nested-loops)
+  - [Threading](#threading)
+  - [Multiprocessing](#multiprocessing)
+  - [Multiprocessing.Pool](#multiprocessingpool)
+- [Features](#features)
+  - [A `break` and an exception](#a-break-and-an-exception)
+  - [Progress of starting threads and processes with progress bars](#progress-of-starting-threads-and-processes-with-progress-bars)
+  - [On Jupyter Notebook](#on-jupyter-notebook)
+  - [Non TTY device](#non-tty-device)
+  - [How to disable progress bars](#how-to-disable-progress-bars)
+- [License](#license)
 
-*****
+---
 
 ## Requirement
 
-- Python 3.6, 3.7, or 3.8
+- Python 3.10, 3.11, or 3.12
 
-*****
+---
 
 ## Install
 
-You can install with `conda` from conda-forge:
+You can install with `pip` from [PyPI](https://pypi.org/project/atpbar/):
 
 ```bash
-conda install -c conda-forge atpbar
+pip install -U atpbar
 ```
 
-or with `pip`:
+To install with Jupyter Notebook support, use the following command:
 
 ```bash
-pip install -U atpbar
+pip install -U atpbar[jupyter]
 ```
 
-*****
+---
 
 ## User guide
 
 ### Quick start
 
-I will show here how to use atpbar by simple examples.
+I will show you how to use the atpbar using simple examples.
 
 #### Import libraries
 
 To create simple loops in the examples, we use two python standard
 libraries, [time](https://docs.python.org/3/library/time.html) and
 [random](https://docs.python.org/3/library/random.html). Import the
 two packages as well as `atpbar`.
 
 ```python
 import time, random
 from atpbar import atpbar
 ```
 
-**Note**: import the object `atpbar` from the package `atpbar` rather
-than importing the package `atpbar` itself.
-
 #### One loop
 
-The object `atpbar` is an iterable that can wrap another iterable and
-shows the progress bars for the iterations. (The idea of making the
-interface iterable was inspired by
-[tqdm](https://github.com/tqdm/tqdm).)
-
+The object `atpbar` is an iterable that can wrap another iterable and shows the
+progress bars for the iterations. (The idea of making the interface iterable
+was inspired by [tqdm](https://github.com/tqdm/tqdm).)
 
 ```python
 n = random.randint(1000, 10000)
 for i in atpbar(range(n)):
     time.sleep(0.0001)
 ```
 
-The task in the above code is to sleep for `0.0001` seconds in each
-iteration of the loop. The number of the iterations of the loop is
-randomly selected from between `1000` and `10000`.
+The task in the above code is to sleep for `0.0001` seconds in each iteration
+of the loop. The number of the iterations of the loop is randomly selected from
+between `1000` and `10000`.
 
 A progress bar will be shown by `atpbar`.
 
-```
-  51.25% ::::::::::::::::::::                     |     4132 /     8062 |:  range(0, 8062) 
+```plaintext
+  51.25% ::::::::::::::::::::                     |     4132 /     8062 |:  range(0, 8062)
 ```
 
-In order for `atpbar` to show a progress bar, the wrapped iterable
-needs to have a length. If the length cannot be obtained by `len()`,
-`atpbar` won't show a progress bar.
+In order for `atpbar` to show a progress bar, the wrapped iterable needs to
+have a length. If the length cannot be obtained by `len()`, `atpbar` won't show
+a progress bar.
 
 #### Nested loops
 
-`atpbar` can show progress bars for nested loops as in the following
-example.
+`atpbar` can show progress bars for nested loops as in the following example.
 
 ```python
-for i in atpbar(range(4), name='outer'):
+for i in atpbar(range(4), name='Outer'):
     n = random.randint(1000, 10000)
-    for j in atpbar(range(n), name='inner {}'.format(i)):
+    for j in atpbar(range(n), name='Inner {}'.format(i)):
         time.sleep(0.0001)
 ```
 
 The outer loop iterates 4 times. The inner loop is similar to the loop
 in the previous example---sleeps for `0.0001` seconds. You can
 optionally give the keyword argument `name` to specify the label on
 the progress bar.
 
-```
- 100.00% :::::::::::::::::::::::::::::::::::::::: |     3287 /     3287 |:  inner 0
- 100.00% :::::::::::::::::::::::::::::::::::::::: |     5850 /     5850 |:  inner 1
-  50.00% ::::::::::::::::::::                     |        2 /        4 |:  outer  
-  34.42% :::::::::::::                            |     1559 /     4529 |:  inner 2
+```plaintext
+ 100.00% :::::::::::::::::::::::::::::::::::::::: |     3287 /     3287 |:  Inner 0
+ 100.00% :::::::::::::::::::::::::::::::::::::::: |     5850 /     5850 |:  Inner 1
+  50.00% ::::::::::::::::::::                     |        2 /        4 |:  Outer
+  34.42% :::::::::::::                            |     1559 /     4529 |:  Inner 2
 ```
 
-In the snapshot of the progress bars above, the outer loop is in its
-3rd iteration. The inner loop has completed twice and is running the
-third. The progress bars for the completed tasks move up. The progress
-bars for the active tasks are growing at the bottom.
+In the snapshot of the progress bars above, the outer loop is in its 3rd
+iteration. The inner loop has been completed twice and is running the third.
+The progress bars for the completed tasks move up. The progress bars for the
+active tasks are growing at the bottom.
 
 #### Threading
 
-`atpbar` can show multiple progress bars for loops concurrently
-iterating in different threads.
+`atpbar` can show multiple progress bars for loops concurrently iterating in
+different threads.
 
 The function `run_with_threading()` in the following code shows an
 example.
 
 ```python
 from atpbar import flush
 import threading
 
 def run_with_threading():
-    nthreads = 5
     def task(n, name):
-        for i in atpbar(range(n), name=name):
+        for _ in atpbar(range(n), name=name):
             time.sleep(0.0001)
-    threads = [ ]
-    for i in range(nthreads):
-        name = 'thread {}'.format(i)
-        n = random.randint(5, 100000)
+
+    n_threads = 5
+    threads = []
+
+    for i in range(n_threads):
+        name = 'Thread {}'.format(i)
+        n = random.randint(5, 10000)
         t = threading.Thread(target=task, args=(n, name))
         t.start()
         threads.append(t)
+
     for t in threads:
         t.join()
+
     flush()
 
+
 run_with_threading()
 ```
 
-The task to sleep for `0.0001` seconds is defined as the function
-`task`. The `task` is concurrently run 5 times with `threading`.
-`atpbar` can be used in any threads. Five progress bars growing
-simultaneously will be shown. The function `flush()` returns when the
-progress bars have finished updating.
-
-```
- 100.00% :::::::::::::::::::::::::::::::::::::::: |     8042 /     8042 |:  thread 3 
-  33.30% :::::::::::::                            |    31967 /    95983 |:  thread 0 
-  77.41% ::::::::::::::::::::::::::::::           |    32057 /    41411 |:  thread 1 
-  45.78% ::::::::::::::::::                       |    31816 /    69499 |:  thread 2 
-  39.93% :::::::::::::::                          |    32373 /    81077 |:  thread 4 
+The task to sleep for `0.0001` seconds is defined as the function `task`. The
+`task` is concurrently run five times with `threading`. `atpbar` can be used in
+any thread. Five progress bars growing simultaneously will be shown. The
+function `flush()` returns when the progress bars have finished updating.
+
+```plaintext
+ 100.00% :::::::::::::::::::::::::::::::::::::::: |     8042 /     8042 |:  Thread 3
+  33.30% :::::::::::::                            |    31967 /    95983 |:  Thread 0
+  77.41% ::::::::::::::::::::::::::::::           |    32057 /    41411 |:  Thread 1
+  45.78% ::::::::::::::::::                       |    31816 /    69499 |:  Thread 2
+  39.93% :::::::::::::::                          |    32373 /    81077 |:  Thread 4
 ```
 
 As a task completes, the progress bar for the task moves up. The
 progress bars for active tasks are at the bottom.
 
 #### Multiprocessing
 
 `atpbar` can be used with `multiprocessing`.
 
-The function `run_with_multiprocessing()` in the following code shows
-an example.
+The function `run_with_multiprocessing()` in the following code shows an
+example.
 
 ```python
 import multiprocessing
 multiprocessing.set_start_method('fork', force=True)
 
 from atpbar import register_reporter, find_reporter, flush
 
 def run_with_multiprocessing():
+
     def task(n, name):
-        for i in atpbar(range(n), name=name):
+        for _ in atpbar(range(n), name=name):
             time.sleep(0.0001)
+
     def worker(reporter, task, queue):
         register_reporter(reporter)
         while True:
             args = queue.get()
             if args is None:
                 queue.task_done()
                 break
             task(*args)
             queue.task_done()
-    nprocesses = 4
-    ntasks = 10
+
+    n_processes = 4
+    processes = []
+
     reporter = find_reporter()
     queue = multiprocessing.JoinableQueue()
-    for i in range(nprocesses):
+
+    for i in range(n_processes):
         p = multiprocessing.Process(target=worker, args=(reporter, task, queue))
         p.start()
-    for i in range(ntasks):
-        name = 'task {}'.format(i)
-        n = random.randint(5, 100000)
+        processes.append(p)
+
+    n_tasks = 10
+    for i in range(n_tasks):
+        name = 'Task {}'.format(i)
+        n = random.randint(5, 10000)
         queue.put((n, name))
-    for i in range(nprocesses):
+
+    for i in range(n_processes):
         queue.put(None)
-        queue.join()
+    queue.join()
+
     flush()
 
+
 run_with_multiprocessing()
 ```
 
 It starts four workers in subprocesses with `multiprocessing` and have
 them run ten tasks.
 
 In order to use `atpbar` in a subprocess, the `reporter`, which can be
 found in the main process by the function `find_reporter()`, needs to
 be brought to the subprocess and registered there by the function
 `register_reporter()`.
 
 Simultaneously growing progress bars will be shown.
 
-```
- 100.00% :::::::::::::::::::::::::::::::::::::::: |    44714 /    44714 |:  task 3
- 100.00% :::::::::::::::::::::::::::::::::::::::: |    47951 /    47951 |:  task 2
- 100.00% :::::::::::::::::::::::::::::::::::::::: |    21461 /    21461 |:  task 5
- 100.00% :::::::::::::::::::::::::::::::::::::::: |    73721 /    73721 |:  task 1
- 100.00% :::::::::::::::::::::::::::::::::::::::: |    31976 /    31976 |:  task 4
- 100.00% :::::::::::::::::::::::::::::::::::::::: |    80765 /    80765 |:  task 0
-  58.12% :::::::::::::::::::::::                  |    20133 /    34641 |:  task 6
-  20.47% ::::::::                                 |    16194 /    79126 |:  task 7
-  47.71% :::::::::::::::::::                      |    13072 /    27397 |:  task 8
-  76.09% ::::::::::::::::::::::::::::::           |     9266 /    12177 |:  task 9
-```
+```plaintext
+ 100.00% :::::::::::::::::::::::::::::::::::::::: |    44714 /    44714 |:  Task 3
+ 100.00% :::::::::::::::::::::::::::::::::::::::: |    47951 /    47951 |:  Task 2
+ 100.00% :::::::::::::::::::::::::::::::::::::::: |    21461 /    21461 |:  Task 5
+ 100.00% :::::::::::::::::::::::::::::::::::::::: |    73721 /    73721 |:  Task 1
+ 100.00% :::::::::::::::::::::::::::::::::::::::: |    31976 /    31976 |:  Task 4
+ 100.00% :::::::::::::::::::::::::::::::::::::::: |    80765 /    80765 |:  Task 0
+  58.12% :::::::::::::::::::::::                  |    20133 /    34641 |:  Task 6
+  20.47% ::::::::                                 |    16194 /    79126 |:  Task 7
+  47.71% :::::::::::::::::::                      |    13072 /    27397 |:  Task 8
+  76.09% ::::::::::::::::::::::::::::::           |     9266 /    12177 |:  Task 9
+```
+
+#### Multiprocessing.Pool
+
+To use `atpbar` with
+[`multiprocessing.Pool`](https://docs.python.org/3/library/multiprocessing.html#multiprocessing.pool.Pool),
+use `find_reporter` as the initializer and give the `reporter` as an argument
+to the initializer.
 
-#### With Mantichora
+```python
+def task(n, name):
+    for _ in atpbar(range(n), name=name):
+        time.sleep(0.0001)
 
-[_Mantichora_](https://github.com/alphatwirl/mantichora) provides a
-simple interface to _multiprocessing_.
 
-With Mantichora, `task()` can be concurrently run with multiprocessing
-with as simple code as the following example:
+def run_with_multiprocessing_pool():
 
-```python
-from mantichora import mantichora
+    n_processes = 4
+    reporter = find_reporter()
+    n_tasks = 10
 
-def task(name):
-    n = random.randint(1000, 10000)
-    for i in atpbar(range(n), name=name):
-        time.sleep(0.0001)
+    args = [(random.randint(5, 10000), 'Task {}'.format(i)) for i in range(n_tasks)]
 
-with mantichora() as mcore:
-    mcore.run(task, 'task 1')
-    mcore.run(task, 'task 2')
-    mcore.run(task, 'task 3')
-    mcore.run(task, 'task 4')
-    mcore.run(task, 'task 5')
-    returns = mcore.returns()
-```
+    with multiprocessing.Pool(n_processes, register_reporter, (reporter,)) as pool:
+        pool.starmap(task, args)
 
-`atpbar` can be used in the task function.
+    flush()
 
-```
- 100.00% :::::::::::::::::::::::::::::::::::::::: |     2288 /     2288 |:  task 3
- 100.00% :::::::::::::::::::::::::::::::::::::::: |     3964 /     3964 |:  task 4
- 100.00% :::::::::::::::::::::::::::::::::::::::: |     4207 /     4207 |:  task 2
- 100.00% :::::::::::::::::::::::::::::::::::::::: |     8519 /     8519 |:  task 1
- 100.00% :::::::::::::::::::::::::::::::::::::::: |     6595 /     6595 |:  task 5
+
+run_with_multiprocessing_pool()
 ```
 
-*****
+---
 
 ### Features
 
 #### A `break` and an exception
 
 When the loop ends with a `break` or an exception, the progress bar stops with
 the last complete iteration.
 
 For example, the loop in the following code breaks during the 1235th iteration.
+
 ```python
 for i in atpbar(range(2000)):
     if i == 1234:
         break
     time.sleep(0.0001)
 ```
 
 Since `i` starts with `0`, when `i` is `1234`, the loop is in its 1235th
 iteration. The last complete iteration is 1234. The progress bar stops at 1234.
 
-```
+```plaintext
   61.70% ::::::::::::::::::::::::                 |     1234 /     2000 |:  range(0, 2000)
 ```
 
 As an example of an exception, in the following code, an exception is
 thrown during the 1235th iteration.
+
 ```python
 for i in atpbar(range(2000)):
     if i == 1234:
         raise Exception
     time.sleep(0.0001)
 ```
+
 The progress bar stops at the last complete iteration, 1234.
 
 ```
   61.70% ::::::::::::::::::::::::                 |     1234 /     2000 |:  range(0, 2000)
 Traceback (most recent call last):
   File "<stdin>", line 3, in <module>
 Exception
@@ -364,132 +364,135 @@
 
 def run_with_threading():
     def task(n, name):
         for i in atpbar(range(n), name=name):
             if i == 1234:
                 break
             time.sleep(0.0001)
-    nthreads = 5
-    threads = [ ]
-    for i in range(nthreads):
-        name = 'thread {}'.format(i)
+
+    n_threads = 5
+    threads = []
+
+    for i in range(n_threads):
+        name = 'Thread {}'.format(i)
         n = random.randint(3000, 10000)
         t = threading.Thread(target=task, args=(n, name))
         t.start()
         threads.append(t)
+
     for t in threads:
         t.join()
+
     flush()
 
 run_with_threading()
 ```
 
 All progress bars stop at 1234.
 
 ```
-  18.21% :::::::                                  |     1234 /     6777 |:  thread 0
-  15.08% ::::::                                   |     1234 /     8183 |:  thread 2
-  15.25% ::::::                                   |     1234 /     8092 |:  thread 1
-  39.90% :::::::::::::::                          |     1234 /     3093 |:  thread 4
-  19.67% :::::::                                  |     1234 /     6274 |:  thread 3
+  18.21% :::::::                                  |     1234 /     6777 |:  Thread 0
+  15.08% ::::::                                   |     1234 /     8183 |:  Thread 2
+  15.25% ::::::                                   |     1234 /     8092 |:  Thread 1
+  39.90% :::::::::::::::                          |     1234 /     3093 |:  Thread 4
+  19.67% :::::::                                  |     1234 /     6274 |:  Thread 3
 ```
 
 #### Progress of starting threads and processes with progress bars
 
-`atpbar` can be used for a loop that starts sub-threads or
-sub-processes in which `atpbar` is also used.
+`atpbar` can be used for a loop that starts sub-threads or sub-processes in
+which `atpbar` is also used.
 
 ```python
 from atpbar import flush
 import threading
 
 def run_with_threading():
     def task(n, name):
         for i in atpbar(range(n), name=name):
             time.sleep(0.0001)
-    nthreads = 5
-    threads = [ ]
-    for i in atpbar(range(nthreads)):
-        name = 'thread {}'.format(i)
+
+    n_threads = 5
+    threads = []
+
+    for i in atpbar(range(n_threads)):
+        name = 'Thread {}'.format(i)
         n = random.randint(200, 1000)
         t = threading.Thread(target=task, args=(n, name))
         t.start()
         threads.append(t)
         time.sleep(0.1)
+
     for t in threads:
         t.join()
+
     flush()
 
 run_with_threading()
 ```
 
 ```
- 100.00% :::::::::::::::::::::::::::::::::::::::: |      209 /      209 |:  thread 1
- 100.00% :::::::::::::::::::::::::::::::::::::::: |      699 /      699 |:  thread 0
- 100.00% :::::::::::::::::::::::::::::::::::::::: |      775 /      775 |:  thread 2
- 100.00% :::::::::::::::::::::::::::::::::::::::: |      495 /      495 |:  thread 3
+ 100.00% :::::::::::::::::::::::::::::::::::::::: |      209 /      209 |:  Thread 1
+ 100.00% :::::::::::::::::::::::::::::::::::::::: |      699 /      699 |:  Thread 0
+ 100.00% :::::::::::::::::::::::::::::::::::::::: |      775 /      775 |:  Thread 2
+ 100.00% :::::::::::::::::::::::::::::::::::::::: |      495 /      495 |:  Thread 3
  100.00% :::::::::::::::::::::::::::::::::::::::: |        5 /        5 |:  range(0, 5)
- 100.00% :::::::::::::::::::::::::::::::::::::::: |      647 /      647 |:  thread 4 
+ 100.00% :::::::::::::::::::::::::::::::::::::::: |      647 /      647 |:  Thread 4
 ```
 
-The `atpbar` sensibly works regardless of the order in which multiple
-instances of `atpbar` in multiple threads and multiple processes start
-and end. The progress bars in the example above indicates that the
-loops in four threads have already ended before the loop in the main
-threads ended; the loop in the last thread ended afterwards.
+The `atpbar` sensibly works regardless of the order in which multiple instances
+of `atpbar` in multiple threads and multiple processes start and end. The
+progress bars in the example above indicate that the loops in four threads
+have already ended before the loop in the main threads ended; the loop in the
+last thread ended afterward.
 
-*****
+---
 
 #### On Jupyter Notebook
 
 On Jupyter Notebook, `atpbar` shows progress bars based on
 [widgets](https://ipywidgets.readthedocs.io).
 
 <img src="https://raw.githubusercontent.com/alphatwirl/notebook-atpbar-001/v1.0.1/images/20190304_01_atpbar_jupyter.gif" width="800">
 
 You can try interactively online:
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/alphatwirl/notebook-atpbar-001/master?filepath=atpbar.ipynb)
 
-*****
+---
 
 #### Non TTY device
 
-If neither on Jupyter Notebook or on a TTY device, `atpbar` is not
-able to show progress bars. `atpbar` occasionally prints the status.
+If neither on Jupyter Notebook or on a TTY device, `atpbar` is not able to show
+progress bars. `atpbar` occasionally prints the status.
 
 ```
-03/04 09:17 :     1173 /     7685 ( 15.26%): thread 0 
-03/04 09:17 :     1173 /     6470 ( 18.13%): thread 3 
-03/04 09:17 :     1199 /     1199 (100.00%): thread 4 
-03/04 09:18 :     1756 /     2629 ( 66.79%): thread 2 
-03/04 09:18 :     1757 /     7685 ( 22.86%): thread 0 
-03/04 09:18 :     1757 /     6470 ( 27.16%): thread 3 
-03/04 09:19 :     2342 /     2629 ( 89.08%): thread 2 
+03/04 09:17 :     1173 /     7685 ( 15.26%): Thread 0
+03/04 09:17 :     1173 /     6470 ( 18.13%): Thread 3
+03/04 09:17 :     1199 /     1199 (100.00%): Thread 4
+03/04 09:18 :     1756 /     2629 ( 66.79%): Thread 2
+03/04 09:18 :     1757 /     7685 ( 22.86%): Thread 0
+03/04 09:18 :     1757 /     6470 ( 27.16%): Thread 3
+03/04 09:19 :     2342 /     2629 ( 89.08%): Thread 2
 ```
 
-*****
+---
 
 #### How to disable progress bars
 
 The function `disable()` disables `atpbar`; progress bars will not be shown.
 
 ```python
 from atpbar import disable
 
 disable()
 ```
 
 This function needs to be called before `atpbar` or `find_reporter()` is used,
 typically at the beginning of the program.
 
-*****
+---
 
 ## License
 
 - _atpbar_ is licensed under the BSD license.
 
-*****
-
-## Contact
-
-- <span itemscope itemtype="https://schema.org/Person"><a itemprop="sameAs" content="https://orcid.org/0000-0003-3225-9861" href="https://orcid.org/0000-0003-3225-9861" target="orcid.widget" rel="me noopener noreferrer" style="vertical-align:text-top;"><img src="https://orcid.org/sites/default/files/images/orcid_16x16.png" style="width:1em;margin-right:.5em;" alt="ORCID iD icon"></a></span>Tai Sakuma - tai.sakuma@gmail.com
-
+---
```

### Comparing `atpbar-1.1.4/atpbar/main.py` & `atpbar-2.0.0/atpbar/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-# Tai Sakuma <tai.sakuma@gmail.com>
-import os, uuid
-import logging
-import time
-
 import contextlib
+import logging
+import uuid
+from collections.abc import Iterable, Iterator
+from typing import Generic, Optional, TypeVar
 
 from .funcs import fetch_reporter
+from .progressreport import Report
+
+T = TypeVar('T')
 
-##__________________________________________________________________||
-def atpbar(iterable, name=None, time_track=False):
+
+def atpbar(iterable: Iterable[T], /, name: Optional[str] = None) -> Iterable[T]:
     """returns an instance of `Atpbar`
 
     Parameters
     ----------
     iterable : iterable
         An iterable whose progress of the iterations is to be shown
     name : str
@@ -22,28 +24,28 @@
     -------
     iterable
         An instance of `Atpbar` if successfully instantiated.
         Otherwise, the object received as the parameter `iterable`.
 
     """
     try:
-        len_ = len(iterable)
+        len_ = len(iterable)  # type: ignore
     except TypeError:
         logger = logging.getLogger(__name__)
-        logging.warning('length is unknown: {!r}'.format(iterable))
-        logging.warning('atpbar is turned off')
+        logger.warning("length is unknown: {!r}".format(iterable))
+        logger.warning("atpbar is turned off")
         return iterable
 
     if name is None:
         name = repr(iterable)
 
-    return Atpbar(iterable, name=name, len_=len_, time_track=time_track)
+    return Atpbar(iterable, name=name, len_=len_)
+
 
-##__________________________________________________________________||
-class Atpbar:
+class Atpbar(Generic[T]):
     """Progress bar
 
     An iterable that wraps another iterable and shows the progress
     bars for the iterations. The class is usually instantiated by the
     function `atpbar`.
 
     Parameters
@@ -53,57 +55,53 @@
     name : str
         A label to be shown on the progress bar
     len_ : int
         The length of the iterable
 
     """
 
-    def __init__(self, iterable, name, len_, time_track=False):
+    def __init__(self, iterable: Iterable[T], name: str, len_: int):
         self.iterable = iterable
         self.name = name
         self.len_ = len_
         self.id_ = uuid.uuid4()
-        self.time_track = time_track
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[T]:
         with fetch_reporter() as reporter:
             self.reporter = reporter
             self.loop_complete = False
             self._report_start()
             with report_last(pbar=self):
-                for i, e in enumerate(self. iterable):
+                for i, e in enumerate(self.iterable):
                     yield e
                     self._report_progress(i)
                 else:
                     self.loop_complete = True
 
-    def _report_start(self):
+    def _report_start(self) -> None:
         if self.reporter is None:
             return
         try:
-            report = dict(
-                taskid=self.id_, name=self.name,
-                done=0, total=self.len_)
-            if self.time_track:
-                report['start_time'] = start_time=time.time()
+            report = Report(taskid=self.id_, name=self.name, done=0, total=self.len_)
             self.reporter.report(report)
-        except:
+        except BaseException:
             pass
 
-    def _report_progress(self, i):
+    def _report_progress(self, i: int) -> None:
         if self.reporter is None:
             return
         try:
-            report = dict(taskid=self.id_, done=(i+1))
+            report = Report(taskid=self.id_, done=(i + 1))
             self.reporter.report(report)
-        except:
+        except BaseException:
             pass
 
+
 @contextlib.contextmanager
-def report_last(pbar):
+def report_last(pbar: Atpbar[T]) -> Iterator[None]:
     """send a last report
 
     This function sends the last report of the task when the loop ends
     with `break` or an exception so that the progress bar will be
     updated with the last complete iteration.
 
     """
@@ -111,13 +109,11 @@
         yield
     finally:
         if pbar.loop_complete:
             return
         if pbar.reporter is None:
             return
         try:
-            report = dict(taskid=pbar.id_, first=False, last=True)
+            report = Report(taskid=pbar.id_, first=False, last=True)
             pbar.reporter.report(report)
-        except:
+        except BaseException:
             pass
-
-##__________________________________________________________________||
```

### Comparing `atpbar-1.1.4/atpbar/presentation/bartty.py` & `atpbar-2.0.0/atpbar/presentation/bartty.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,82 +1,112 @@
-# Tai Sakuma <tai.sakuma@gmail.com>
-import os
-import sys
 import shutil
+from typing import TextIO
+from uuid import UUID
 
-from .base import Presentation
+from .base import Presentation, Report
 
-##__________________________________________________________________||
 MINIMUM_TERMINAL_WIDTH = 90
 
-##__________________________________________________________________||
+
 class ProgressBar(Presentation):
-    def __init__(self):
+    stdout_stderr_redrection = True
+
+    def __init__(self) -> None:
         super().__init__()
-        self.lines = [ ]
-        self.interval = 0.1 # [second]
+        self.interval = 0.1  # [second]
         self.width = self._get_width()
 
-    def __repr__(self):
-        return '{}()'.format(
-            self.__class__.__name__
-        )
+        self.active_bars = list[str]()
+        self.just_finised_bars = list[str]()
 
-    def _get_width(self):
+    def __repr__(self) -> str:
+        return "{}()".format(self.__class__.__name__)
+
+    def _get_width(self) -> int:
         try:
             columns = shutil.get_terminal_size().columns
             return max(MINIMUM_TERMINAL_WIDTH, columns - 1)
         except AttributeError:
             return MINIMUM_TERMINAL_WIDTH
 
-    def _present(self):
-        self._delete_previous_lines()
-        self._create_lines()
-        self._print_lines()
-
-    def _delete_previous_lines(self):
-        if len(self.lines) >= 1:
-            sys.stdout.write('\033[2K\033[1G')
-            # '\033[2K' erase the line
-            # '\033[1G' move the cursor to the beginning of the line
-        if len(self.lines) >= 2:
-            sys.stdout.write('\033[A\033[K'*(len(self.lines) - 1))
-            # '\033[A' move the cursor up
-            # '\033[K' clear from cursor to the end of the line
-        self.lines = [ ]
-        self.last = [ ]
-
-    def _create_lines(self):
-        for taskid in self._active_taskids + self._new_taskids:
-            report = self._report_dict[taskid]
-            line = self._create_line(report)
-            self.lines.append(line)
-        for taskid in self._finishing_taskids:
-            report = self._report_dict[taskid]
-            line = self._create_line(report)
-            self.last.append(line)
-
-    def _create_line(self, report):
-        percent = float(report['done'])/report['total'] if report['total'] > 0 else 1
-        bar = (':' * int(percent * 40)).ljust(40, " ")
+    def _present(self) -> None:
+        self._erase_active_bars()
+        self._compose_just_finised_bars()
+        self._compose_active_bars()
+        self._draw_just_finised_bars()
+        self._draw_active_bars()
+
+    def _write(self, s: str, out: TextIO) -> None:
+        if not s:
+            return
+        self._erase_active_bars()
+        out.write(s.rstrip())
+        out.write("\n")
+        out.flush()
+        self._draw_active_bars()
+
+    def _erase_active_bars(self) -> None:
+        nlines = len(self._active_taskids) + len(self._finishing_taskids)
+        # must be the same as len(self.active_bars)
+
+        if nlines == 0:
+            return
+
+        code = "\033[1G" + "\033[A" * (nlines - 1) + "\033[0J"
+        # '\033[1G' move the cursor to the beginning of the line
+        # '\033[A' move the cursor up
+        # '\033[0J' clear from cursor to end of screen
+
+        self.out.write(code)
+        self.out.flush()
+
+    def _compose_just_finised_bars(self) -> None:
+        self.just_finised_bars = [
+            self._compose_bar_from_taskid(i) for i in self._finishing_taskids
+        ]
+
+    def _compose_active_bars(self) -> None:
+        self.active_bars = [
+            self._compose_bar_from_taskid(i)
+            for i in self._active_taskids + self._new_taskids
+        ]
+
+    def _compose_bar_from_taskid(self, taskid: UUID) -> str:
+        report = self._report_dict[taskid]
+        return self._compose_bar_from_report(report)
+
+    def _compose_bar_from_report(self, report: Report) -> str:
+
+        percent = float(report["done"]) / report["total"] if report["total"] > 0 else 1
+        # e.g., 0.7143369818769065
+
+        bar = (":" * int(percent * 40)).ljust(40, " ")
+        # e.g., "::::::::::::::::::::::::::::            "
+
         percent = round(percent * 100, 2)
-        format = ' {percent:6.2f}% {bar:s} | {done:8d} / {total:8d} |:  {name} '
+        # e.g., 71.43
 
-        if "start_time" in report.keys():
-            elapsed_str, remaining_str = self._get_time_track(
-                report["start_time"], percent
-            )
-            format += " | [{:s} / {:s}]".format(elapsed_str, remaining_str)
+        format = " {percent:6.2f}% {bar:s} | {done:8d} / {total:8d} |:  {name} "
 
         ret = format.format(
-            percent=percent, bar=bar,
-            done=report['done'], total=report['total'],
-            name=report['name'])
-        ret = ret[:self.width].ljust(self.width, ' ')
-        return ret
+            percent=percent,
+            bar=bar,
+            done=report["done"],
+            total=report["total"],
+            name=report["name"],
+        )
+        # e.g., "  71.43% ::::::::::::::::::::::::::::             |     3981 /     5573 |:  task name "
+
+        ret = ret[: self.width].ljust(self.width, " ")
+        # e.g., "  71.43% ::::::::::::::::::::::::::::             |     3981 /     5573 |:  task na"
 
-    def _print_lines(self):
-        if len(self.last) > 0: sys.stdout.write("\n".join(self.last) + "\n")
-        sys.stdout.write("\n".join(self.lines))
-        sys.stdout.flush()
+        return ret
 
-##__________________________________________________________________||
+    def _draw_just_finised_bars(self) -> None:
+        if self.just_finised_bars:
+            self.out.write("\n".join(self.just_finised_bars) + "\n")
+            self.out.flush()
+
+    def _draw_active_bars(self) -> None:
+        if self.active_bars:
+            self.out.write("\n".join(self.active_bars))
+            self.out.flush()
```

### Comparing `atpbar-1.1.4/atpbar/presentation/detect/spy.py` & `atpbar-2.0.0/atpbar/presentation/detect/spy.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 import os
 
 try:
-    import spyder
+    import spyder  # type: ignore
 except ImportError:
     spyder = None
 
 try:
     from IPython import get_ipython
 except ImportError:
-    get_ipython = None
+    get_ipython = None  # type: ignore
 
-##__________________________________________________________________||
-def is_spyder_ide():
+
+def is_spyder_ide() -> bool:
     """Tests if on Spyder IDE
 
     Returns
     -------
     bool
         True if on Spyder IDE
 
     """
 
     if spyder is None:
         return False
 
     try:
-        if 'IPKernelApp' not in get_ipython().config:
+        if "IPKernelApp" not in get_ipython().config:
             return False
     except:
         return False
 
-    if 'SPYDER_ARGS' not in os.environ:
+    if "SPYDER_ARGS" not in os.environ:
         return False
 
-    min_n_spy_var = 15 # A possible minimum number of the environmental
-                       # variables that start with "SPY_" on Spyder IDE.
-    n_spy_var =  len([k for k in os.environ.keys() if k.startswith('SPY_')])
+    min_n_spy_var = 15  # A possible minimum number of the environmental
+    # variables that start with "SPY_" on Spyder IDE.
+    n_spy_var = len([k for k in os.environ.keys() if k.startswith("SPY_")])
     if n_spy_var < min_n_spy_var:
         return False
 
     return True
-
-##__________________________________________________________________||
```

### Comparing `atpbar-1.1.4/atpbar/presentation/txtprint.py` & `atpbar-2.0.0/atpbar/presentation/txtprint.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,62 +1,63 @@
-# Tai Sakuma <tai.sakuma@gmail.com>
-import sys, time
+import time
+from uuid import UUID
+
+from .base import Presentation, Report
 
-from .base import Presentation
 
-##__________________________________________________________________||
 class ProgressPrint(Presentation):
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__()
-        self.interval = 60.0 # [second]
-        self.last_time = { } # key: taskid
+        self.interval = 60.0  # [second]
+        self.last_time_map = dict[UUID, float]()
 
-    def __repr__(self):
-        return '{}()'.format(
-            self.__class__.__name__
-        )
+    def __repr__(self) -> str:
+        return "{}()".format(self.__class__.__name__)
 
-    def present(self, report):
+    def present(self, report: Report) -> None:
 
         if not self._register_report(report):
             return
 
-        if not self._need_to_present(report):
+        if not self._need_to_present_(report):
             return
 
-        self._present(report)
+        self._present_(report)
 
-        self.last_time[report['taskid']] = self._time()
-
-    def _present(self, report):
-        time_ = time.strftime('%m/%d %H:%M', time.localtime(time.time()))
-        percent = float(report['done'])/report['total'] if report['total'] > 0 else 1
+        self.last_time_map[report["taskid"]] = self._time()
+    
+    def _present(self) -> None:
+        pass
+
+    def _present_(self, report: Report) -> None:
+        time_ = time.strftime("%m/%d %H:%M", time.localtime(time.time()))
+        percent = float(report["done"]) / report["total"] if report["total"] > 0 else 1
         percent = round(percent * 100, 2)
         line = "{time} : {done:8d} / {total:8d} ({percent:6.2f}%): {name} ".format(
             time=time_,
-            done=report['done'], total=report['total'],
-            percent=percent, name=report['name']
+            done=report["done"],
+            total=report["total"],
+            percent=percent,
+            name=report["name"],
         )
-        line = '{}\n'.format(line)
-        sys.stdout.write(line)
-        sys.stdout.flush()
+        line = "{}\n".format(line)
+        self.out.write(line)
+        self.out.flush()
 
-    def _need_to_present(self, report):
+    def _need_to_present_(self, report: Report) -> bool:
 
-        if report['first']:
+        if report["first"]:
             return True
 
-        if report['last']:
+        if report["last"]:
             return True
 
-        if report['taskid'] not in self.last_time:
+        if report["taskid"] not in self.last_time_map:
             return True
 
-        if self._time() - self.last_time[report['taskid']] > self.interval:
+        if self._time() - self.last_time_map[report["taskid"]] > self.interval:
             return True
 
         return False
 
-    def _time(self):
+    def _time(self) -> float:
         return time.time()
-
-##__________________________________________________________________||
```

### Comparing `atpbar-1.1.4/atpbar/report.py` & `atpbar-2.0.0/atpbar/progressreport/complement.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,51 @@
-# Tai Sakuma <tai.sakuma@gmail.com>
+from uuid import UUID
+
+from .report import Report
+
 
-##__________________________________________________________________||
 class ProgressReportComplementer:
     """Complement progress reports
 
     Complement a progress report with the previous report for the same
     task.
 
     Parameters
     ----------
-    report : dict
-        A progress report, a dict with the following entries. The
-        `taskid` must be always given. The first report for a task
-        must include `done`, `total`, and 'name'. The `first` and
-        `last` will be automatically determined if not given.
-
-        taskid : immutable
-            The unique task ID.
-        done : int, optional
-            The number of the iterations done so far
-        total : int
-            The total iterations to be done
-        name : str
-            A name of the task. It will be use as the label on the
-            progress bars.
-        first : bool
-            `True` if the first report for the task. If not given,
-            automatically determined from `done`; `True` if `done` is
-            0, `False` otherwise
-        last : bool
-            `True` if the last report for the task. If not given,
-            automatically determined from `done` and `total`; `True`
-            if `done` equals `total`, `False` otherwise
+    report : Report
+        A report must always include `taskid`. The first report for a task must
+        include `done`, `total`, and 'name'. The `first` and `last` will be
+        automatically determined if not given.
 
     """
-    def __init__(self):
-        self.previous_reports = { }
-        self.volatile_fileds = ('first', 'last')
 
-    def __call__(self, report):
-        taskid = report['taskid']
+    def __init__(self) -> None:
+        self.previous_reports = dict[UUID, Report]()
+
+    def __call__(self, report: Report) -> None:
+        taskid = report["taskid"]
         if taskid in self.previous_reports:
             self._complement(taskid, report)
         self._first(report)
         self._last(report)
         self._store(taskid, report.copy())
 
-    def _complement(self, taskid, report):
+    def _complement(self, taskid: UUID, report: Report) -> None:
         report_copy = report.copy()
-        report.clear()
+        report.update(Report(taskid=taskid))
         report.update(self.previous_reports[taskid])
         report.update(report_copy)
 
-    def _first(self, report):
-        if 'first' in report:
+    def _first(self, report: Report) -> None:
+        if "first" in report:
             return
-        report['first'] = (report['done'] == 0)
+        report["first"] = report["done"] == 0
 
-    def _last(self, report):
-        if 'last' in report:
+    def _last(self, report: Report) -> None:
+        if "last" in report:
             return
-        report['last'] = (report['done'] >= report['total'])
+        report["last"] = report["done"] >= report["total"]
 
-    def _store(self, taskid, report):
-        for k in self.volatile_fileds:
-            report.pop(k, None)
+    def _store(self, taskid: UUID, report: Report) -> None:
+        report.pop('first', None)
+        report.pop('last', None)
         self.previous_reports[taskid] = report
-
-##__________________________________________________________________||
```

### Comparing `atpbar-1.1.4/atpbar/reporter.py` & `atpbar-2.0.0/atpbar/progressreport/reporter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,21 @@
-# Tai Sakuma <tai.sakuma@gmail.com>
 import time
-from .report import ProgressReportComplementer
+from multiprocessing import Queue
+from typing import TYPE_CHECKING
+from uuid import UUID
+
+from .complement import ProgressReportComplementer
+from .report import Report
+
+if TYPE_CHECKING:
+    from atpbar.stream import StreamQueue
+
+DEFAULT_INTERVAL = 0.1  # [second]
 
-##__________________________________________________________________||
-DEFAULT_INTERVAL = 0.1 # [second]
 
-##__________________________________________________________________||
 class ProgressReporter:
     """A progress reporter
 
     This class sends progress reports. The reports will be picked up
     by the pickup (`ProgressReportPickup`), which uses the reports,
     for example, to update `ProgressBar` on the screen.
 
@@ -34,28 +40,35 @@
     regardless of whether it is given within the interval.
 
     Parameters
     ----------
     queue : multiprocessing.Queue
         The queue through which this class sends progress reports.
     """
-    def __init__(self, queue):
+
+    def __init__(
+        self,
+        queue: 'Queue[Report]',
+        notices_from_sub_processes: 'Queue[bool]',
+        stream_queue: 'StreamQueue',
+    ) -> None:
         self.queue = queue
-        self.interval = DEFAULT_INTERVAL # [second]
-        self.last_time = { } # key: taskid
+        self.interval = DEFAULT_INTERVAL  # [second]
+        self.last_time = dict[UUID, float]()
         self.complete_report = ProgressReportComplementer()
-
-    def __repr__(self):
-        return '{}(queue={!r}, interval={!r})'.format(
-            self.__class__.__name__,
-            self.queue,
-            self.interval
+        self.notices_from_sub_processes = notices_from_sub_processes
+        self.stream_queue = stream_queue
+        self.stream_redirection_enablaed = True
+
+    def __repr__(self) -> str:
+        return "{}(queue={!r}, interval={!r})".format(
+            self.__class__.__name__, self.queue, self.interval
         )
 
-    def report(self, report):
+    def report(self, report: Report) -> None:
         """send ``report`` to a progress monitor
 
         Parameters
         ----------
         report : ProgressReport
             a progress report
 
@@ -64,26 +77,24 @@
         self.complete_report(report)
 
         if not self._need_to_report(report):
             return
 
         self.queue.put(report)
 
-        self.last_time[report['taskid']] = time.time()
+        self.last_time[report["taskid"]] = time.time()
 
-    def _need_to_report(self, report):
+    def _need_to_report(self, report: Report) -> bool:
 
-        if report['first']:
+        if report["first"]:
             return True
 
-        if report['last']:
+        if report["last"]:
             return True
 
-        if report['taskid'] not in self.last_time:
+        if report["taskid"] not in self.last_time:
             return True
 
-        if time.time() - self.last_time[report['taskid']] > self.interval:
+        if time.time() - self.last_time[report["taskid"]] > self.interval:
             return True
 
         return False
-
-##__________________________________________________________________||
```

