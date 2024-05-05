# Comparing `tmp/cyantities-0.0.3.tar.gz` & `tmp/cyantities-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyantities-0.0.3.tar", last modified: Wed Apr 24 19:28:17 2024, max compression
+gzip compressed data, was "cyantities-0.1.0.tar", last modified: Sun May  5 12:49:14 2024, max compression
```

## Comparing `cyantities-0.0.3.tar` & `cyantities-0.1.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2024-04-24 19:28:17.708221 cyantities-0.0.3/
-drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2024-04-24 19:28:17.708221 cyantities-0.0.3/Cyantities.egg-info/
--rw-r--r--   0 phd       (1000) phd       (1000)    25031 2024-04-24 19:28:17.000000 cyantities-0.0.3/Cyantities.egg-info/PKG-INFO
--rw-r--r--   0 phd       (1000) phd       (1000)      972 2024-04-24 19:28:17.000000 cyantities-0.0.3/Cyantities.egg-info/SOURCES.txt
--rw-r--r--   0 phd       (1000) phd       (1000)        1 2024-04-24 19:28:17.000000 cyantities-0.0.3/Cyantities.egg-info/dependency_links.txt
--rw-r--r--   0 phd       (1000) phd       (1000)      144 2024-04-24 19:28:17.000000 cyantities-0.0.3/Cyantities.egg-info/entry_points.txt
--rw-r--r--   0 phd       (1000) phd       (1000)       20 2024-04-24 19:28:17.000000 cyantities-0.0.3/Cyantities.egg-info/requires.txt
--rw-r--r--   0 phd       (1000) phd       (1000)       11 2024-04-24 19:28:17.000000 cyantities-0.0.3/Cyantities.egg-info/top_level.txt
--rw-r--r--   0 phd       (1000) phd       (1000)    13827 2024-02-27 16:11:04.000000 cyantities-0.0.3/LICENSE
--rw-r--r--   0 phd       (1000) phd       (1000)      494 2024-04-24 19:02:45.000000 cyantities-0.0.3/MANIFEST.in
--rw-r--r--   0 phd       (1000) phd       (1000)    25031 2024-04-24 19:28:17.708221 cyantities-0.0.3/PKG-INFO
--rw-r--r--   0 phd       (1000) phd       (1000)     8011 2024-04-24 19:21:18.000000 cyantities-0.0.3/README.md
-drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2024-04-24 19:28:17.708221 cyantities-0.0.3/cyantities/
--rw-r--r--   0 phd       (1000) phd       (1000)      838 2024-02-27 16:11:04.000000 cyantities-0.0.3/cyantities/__init__.py
-drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2024-04-24 19:28:17.708221 cyantities-0.0.3/cyantities/_cpp/
--rw-r--r--   0 phd       (1000) phd       (1000)       60 2024-04-07 06:46:30.000000 cyantities-0.0.3/cyantities/_cpp/__init__.py
-drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2024-04-24 19:28:17.708221 cyantities-0.0.3/cyantities/_cpp/cyantities/
--rw-r--r--   0 phd       (1000) phd       (1000)       60 2024-04-07 06:46:25.000000 cyantities-0.0.3/cyantities/_cpp/cyantities/__init__.py
--rw-r--r--   0 phd       (1000) phd       (1000)     8338 2024-04-23 21:08:21.000000 cyantities-0.0.3/cyantities/_cpp/cyantities/boost.hpp
--rw-r--r--   0 phd       (1000) phd       (1000)     5096 2024-04-07 12:21:46.000000 cyantities-0.0.3/cyantities/_cpp/cyantities/quantitywrap.hpp
--rw-r--r--   0 phd       (1000) phd       (1000)     2576 2024-04-23 21:06:46.000000 cyantities-0.0.3/cyantities/_cpp/cyantities/unit.hpp
-drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2024-04-24 19:28:17.708221 cyantities-0.0.3/cyantities/_cpp/src/
--rw-r--r--   0 phd       (1000) phd       (1000)     2130 2024-04-07 12:11:18.000000 cyantities-0.0.3/cyantities/_cpp/src/quantitywrap.cpp
--rw-r--r--   0 phd       (1000) phd       (1000)     4526 2024-03-03 23:03:48.000000 cyantities-0.0.3/cyantities/_cpp/src/unit.cpp
--rw-r--r--   0 phd       (1000) phd       (1000)      863 2024-02-27 16:19:07.000000 cyantities-0.0.3/cyantities/errors.py
--rw-r--r--   0 phd       (1000) phd       (1000)     1678 2024-04-06 20:09:43.000000 cyantities-0.0.3/cyantities/quantity.pxd
--rw-r--r--   0 phd       (1000) phd       (1000)    17932 2024-04-07 13:35:33.000000 cyantities-0.0.3/cyantities/quantity.pyx
-drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2024-04-24 19:28:17.708221 cyantities-0.0.3/cyantities/scripts/
--rw-r--r--   0 phd       (1000) phd       (1000)      855 2024-04-07 09:26:54.000000 cyantities-0.0.3/cyantities/scripts/__init__.py
--rw-r--r--   0 phd       (1000) phd       (1000)     1079 2024-04-07 08:08:51.000000 cyantities-0.0.3/cyantities/scripts/include.py
--rw-r--r--   0 phd       (1000) phd       (1000)     1098 2024-04-07 09:25:42.000000 cyantities-0.0.3/cyantities/scripts/link.py
--rw-r--r--   0 phd       (1000) phd       (1000)     2773 2024-04-23 21:23:36.000000 cyantities-0.0.3/cyantities/unit.pxd
--rw-r--r--   0 phd       (1000) phd       (1000)    21230 2024-04-23 21:25:30.000000 cyantities-0.0.3/cyantities/unit.pyx
-drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2024-04-24 19:28:17.704887 cyantities-0.0.3/examples/
-drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2024-04-24 19:28:17.708221 cyantities-0.0.3/examples/parabola/
--rw-r--r--   0 phd       (1000) phd       (1000)     1375 2024-04-07 11:08:46.000000 cyantities-0.0.3/examples/parabola/build.py
--rw-r--r--   0 phd       (1000) phd       (1000)     1040 2024-04-07 11:18:18.000000 cyantities-0.0.3/examples/parabola/meson.build
--rw-r--r--   0 phd       (1000) phd       (1000)     8484 2024-04-07 15:06:32.000000 cyantities-0.0.3/examples/parabola/parasolve.cpp
--rw-r--r--   0 phd       (1000) phd       (1000)     1720 2024-04-06 20:23:46.000000 cyantities-0.0.3/examples/parabola/parasolve.hpp
--rw-r--r--   0 phd       (1000) phd       (1000)     2994 2024-04-07 11:46:10.000000 cyantities-0.0.3/examples/parabola/parasolve.pyx
--rw-r--r--   0 phd       (1000) phd       (1000)     1700 2024-04-07 15:07:41.000000 cyantities-0.0.3/examples/parabola/run.py
-drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2024-04-24 19:28:17.704887 cyantities-0.0.3/examples/parabola/subprojects/
-drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2024-04-24 19:28:17.708221 cyantities-0.0.3/examples/parabola/subprojects/cyantities/
--rw-r--r--   0 phd       (1000) phd       (1000)     2628 2024-04-07 13:48:33.000000 cyantities-0.0.3/examples/parabola/subprojects/cyantities/meson.build
--rw-r--r--   0 phd       (1000) phd       (1000)     1604 2024-04-24 19:12:12.000000 cyantities-0.0.3/meson.build
--rw-r--r--   0 phd       (1000) phd       (1000)     1363 2024-04-24 19:08:29.000000 cyantities-0.0.3/pyproject.toml
--rw-r--r--   0 phd       (1000) phd       (1000)       38 2024-04-24 19:28:17.708221 cyantities-0.0.3/setup.cfg
--rw-r--r--   0 phd       (1000) phd       (1000)     1549 2024-04-07 09:26:17.000000 cyantities-0.0.3/setup.py
+drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2024-05-05 12:49:14.211716 cyantities-0.1.0/
+drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2024-05-05 12:49:14.211716 cyantities-0.1.0/Cyantities.egg-info/
+-rw-r--r--   0 phd       (1000) phd       (1000)    25677 2024-05-05 12:49:14.000000 cyantities-0.1.0/Cyantities.egg-info/PKG-INFO
+-rw-r--r--   0 phd       (1000) phd       (1000)      972 2024-05-05 12:49:14.000000 cyantities-0.1.0/Cyantities.egg-info/SOURCES.txt
+-rw-r--r--   0 phd       (1000) phd       (1000)        1 2024-05-05 12:49:14.000000 cyantities-0.1.0/Cyantities.egg-info/dependency_links.txt
+-rw-r--r--   0 phd       (1000) phd       (1000)      144 2024-05-05 12:49:14.000000 cyantities-0.1.0/Cyantities.egg-info/entry_points.txt
+-rw-r--r--   0 phd       (1000) phd       (1000)       20 2024-05-05 12:49:14.000000 cyantities-0.1.0/Cyantities.egg-info/requires.txt
+-rw-r--r--   0 phd       (1000) phd       (1000)       11 2024-05-05 12:49:14.000000 cyantities-0.1.0/Cyantities.egg-info/top_level.txt
+-rw-r--r--   0 phd       (1000) phd       (1000)    13827 2024-02-27 16:11:04.000000 cyantities-0.1.0/LICENSE
+-rw-r--r--   0 phd       (1000) phd       (1000)      494 2024-04-24 19:02:45.000000 cyantities-0.1.0/MANIFEST.in
+-rw-r--r--   0 phd       (1000) phd       (1000)    25677 2024-05-05 12:49:14.211716 cyantities-0.1.0/PKG-INFO
+-rw-r--r--   0 phd       (1000) phd       (1000)     8656 2024-05-05 12:40:02.000000 cyantities-0.1.0/README.md
+drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2024-05-05 12:49:14.208382 cyantities-0.1.0/cyantities/
+-rw-r--r--   0 phd       (1000) phd       (1000)      838 2024-02-27 16:11:04.000000 cyantities-0.1.0/cyantities/__init__.py
+drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2024-05-05 12:49:14.208382 cyantities-0.1.0/cyantities/_cpp/
+-rw-r--r--   0 phd       (1000) phd       (1000)       60 2024-04-07 06:46:30.000000 cyantities-0.1.0/cyantities/_cpp/__init__.py
+drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2024-05-05 12:49:14.211716 cyantities-0.1.0/cyantities/_cpp/cyantities/
+-rw-r--r--   0 phd       (1000) phd       (1000)       60 2024-04-07 06:46:25.000000 cyantities-0.1.0/cyantities/_cpp/cyantities/__init__.py
+-rw-r--r--   0 phd       (1000) phd       (1000)     8338 2024-04-23 21:08:21.000000 cyantities-0.1.0/cyantities/_cpp/cyantities/boost.hpp
+-rw-r--r--   0 phd       (1000) phd       (1000)    18157 2024-05-04 20:57:12.000000 cyantities-0.1.0/cyantities/_cpp/cyantities/quantitywrap.hpp
+-rw-r--r--   0 phd       (1000) phd       (1000)     2576 2024-04-23 21:06:46.000000 cyantities-0.1.0/cyantities/_cpp/cyantities/unit.hpp
+drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2024-05-05 12:49:14.211716 cyantities-0.1.0/cyantities/_cpp/src/
+-rw-r--r--   0 phd       (1000) phd       (1000)     2130 2024-04-07 12:11:18.000000 cyantities-0.1.0/cyantities/_cpp/src/quantitywrap.cpp
+-rw-r--r--   0 phd       (1000) phd       (1000)     4526 2024-03-03 23:03:48.000000 cyantities-0.1.0/cyantities/_cpp/src/unit.cpp
+-rw-r--r--   0 phd       (1000) phd       (1000)      863 2024-02-27 16:19:07.000000 cyantities-0.1.0/cyantities/errors.py
+-rw-r--r--   0 phd       (1000) phd       (1000)     1755 2024-04-29 09:14:33.000000 cyantities-0.1.0/cyantities/quantity.pxd
+-rw-r--r--   0 phd       (1000) phd       (1000)    19165 2024-05-05 11:27:53.000000 cyantities-0.1.0/cyantities/quantity.pyx
+drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2024-05-05 12:49:14.211716 cyantities-0.1.0/cyantities/scripts/
+-rw-r--r--   0 phd       (1000) phd       (1000)      855 2024-04-07 09:26:54.000000 cyantities-0.1.0/cyantities/scripts/__init__.py
+-rw-r--r--   0 phd       (1000) phd       (1000)     1079 2024-04-07 08:08:51.000000 cyantities-0.1.0/cyantities/scripts/include.py
+-rw-r--r--   0 phd       (1000) phd       (1000)     1098 2024-04-07 09:25:42.000000 cyantities-0.1.0/cyantities/scripts/link.py
+-rw-r--r--   0 phd       (1000) phd       (1000)     2773 2024-04-23 21:23:36.000000 cyantities-0.1.0/cyantities/unit.pxd
+-rw-r--r--   0 phd       (1000) phd       (1000)    21230 2024-04-23 21:25:30.000000 cyantities-0.1.0/cyantities/unit.pyx
+drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2024-05-05 12:49:14.208382 cyantities-0.1.0/examples/
+drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2024-05-05 12:49:14.211716 cyantities-0.1.0/examples/parabola/
+-rw-r--r--   0 phd       (1000) phd       (1000)     1375 2024-04-07 11:08:46.000000 cyantities-0.1.0/examples/parabola/build.py
+-rw-r--r--   0 phd       (1000) phd       (1000)     1040 2024-04-07 11:18:18.000000 cyantities-0.1.0/examples/parabola/meson.build
+-rw-r--r--   0 phd       (1000) phd       (1000)     8504 2024-05-04 18:32:02.000000 cyantities-0.1.0/examples/parabola/parasolve.cpp
+-rw-r--r--   0 phd       (1000) phd       (1000)     1720 2024-04-06 20:23:46.000000 cyantities-0.1.0/examples/parabola/parasolve.hpp
+-rw-r--r--   0 phd       (1000) phd       (1000)     2994 2024-04-07 11:46:10.000000 cyantities-0.1.0/examples/parabola/parasolve.pyx
+-rw-r--r--   0 phd       (1000) phd       (1000)     1700 2024-04-07 15:07:41.000000 cyantities-0.1.0/examples/parabola/run.py
+drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2024-05-05 12:49:14.208382 cyantities-0.1.0/examples/parabola/subprojects/
+drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2024-05-05 12:49:14.211716 cyantities-0.1.0/examples/parabola/subprojects/cyantities/
+-rw-r--r--   0 phd       (1000) phd       (1000)     2628 2024-04-07 13:48:33.000000 cyantities-0.1.0/examples/parabola/subprojects/cyantities/meson.build
+-rw-r--r--   0 phd       (1000) phd       (1000)     1604 2024-05-05 12:31:04.000000 cyantities-0.1.0/meson.build
+-rw-r--r--   0 phd       (1000) phd       (1000)     1364 2024-05-05 12:30:31.000000 cyantities-0.1.0/pyproject.toml
+-rw-r--r--   0 phd       (1000) phd       (1000)       38 2024-05-05 12:49:14.211716 cyantities-0.1.0/setup.cfg
+-rw-r--r--   0 phd       (1000) phd       (1000)     1549 2024-04-07 09:26:17.000000 cyantities-0.1.0/setup.py
```

### Comparing `cyantities-0.0.3/Cyantities.egg-info/PKG-INFO` & `cyantities-0.1.0/Cyantities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Cyantities
-Version: 0.0.3
+Version: 0.1.0
 Summary: Physical quantities with units.
 Author-email: "Malte J. Ziebarth" <mjz.science@fmvkb.de>
 License:                       EUROPEAN UNION PUBLIC LICENCE v. 1.2
                               EUPL © the European Union 2007, 2016
         
         This European Union Public Licence (the ‘EUPL’) applies to the Work (as defined
         below) which is provided under the terms of this Licence. Any use of the Work,
@@ -290,15 +290,15 @@
         
         All other changes or additions to this Appendix require the production of a new
         EUPL version.
         
 Project-URL: Homepage, https://github.com/mjziebarth/Cyantities
 Project-URL: Bug Tracker, https://github.com/mjziebarth/Cyantities/issues
 Project-URL: Documentation, https://github.com/mjziebarth/Cyantities
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: C++
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
@@ -413,15 +413,17 @@
 dimensional correctness of the data passed from the Python level. Once this is done,
 the numerical data can similarly be transformed from the Python objects to the
 Boost.Units-powered C++ library.
 
 The interaction of Cyantities with Boost.Units is best explained through an
 example. See the example of a ball throw with gravity and friction in
 [examples/parabola](examples/parabola/) for a blueprint of how to use
-Cyantities with Boost.Units.
+Cyantities with Boost.Units, and the example of gravitational force on different
+masses in [examples/gravity](examples/gravity/) for different methods to iterate
+vector-valued quantities in C++.
 
 
 ## Python Known Units
 The following basic units are currently implemented in Cyantities and can be used
 to compose units based on the [coherent SI](#coherent-si-rule) or the [nominator-denominator](#nominator-denominator-rule) rule:
 
 | Python string | Unit          | Comment            |
@@ -476,14 +478,24 @@
 ## License
 This software is licensed under the European Public License (EUPL) version 1.2 or later.
 
 ## Changelog
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+### [0.1.0] - 2024-05-05
+#### Added
+- Add `zeros_like` generator function for `Quantity` (Cython only)
+- Add the `iter()` and `const_iter()` templated methods to C++
+  `QuantityWrapper` class, allowing for the use of range-based for loops and
+  range adaptor closures (`|`-operator syntax) in compile-time provided units.
+- Add the `gravity` example that showcases different methods to iterate
+  vector-valued quantities in C++.
+- Add benchmark for different iteration methods.
+
 ### [0.0.3] - 2024-04-24
 #### Changed
 - Fixed the installation requirements and source distribution manifest.
 - Add version coherence test script.
 
 ### [0.0.2] - 2024-04-23
 #### Changed
```

### Comparing `cyantities-0.0.3/Cyantities.egg-info/SOURCES.txt` & `cyantities-0.1.0/Cyantities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyantities-0.0.3/LICENSE` & `cyantities-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cyantities-0.0.3/PKG-INFO` & `cyantities-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Cyantities
-Version: 0.0.3
+Version: 0.1.0
 Summary: Physical quantities with units.
 Author-email: "Malte J. Ziebarth" <mjz.science@fmvkb.de>
 License:                       EUROPEAN UNION PUBLIC LICENCE v. 1.2
                               EUPL © the European Union 2007, 2016
         
         This European Union Public Licence (the ‘EUPL’) applies to the Work (as defined
         below) which is provided under the terms of this Licence. Any use of the Work,
@@ -290,15 +290,15 @@
         
         All other changes or additions to this Appendix require the production of a new
         EUPL version.
         
 Project-URL: Homepage, https://github.com/mjziebarth/Cyantities
 Project-URL: Bug Tracker, https://github.com/mjziebarth/Cyantities/issues
 Project-URL: Documentation, https://github.com/mjziebarth/Cyantities
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: C++
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
@@ -413,15 +413,17 @@
 dimensional correctness of the data passed from the Python level. Once this is done,
 the numerical data can similarly be transformed from the Python objects to the
 Boost.Units-powered C++ library.
 
 The interaction of Cyantities with Boost.Units is best explained through an
 example. See the example of a ball throw with gravity and friction in
 [examples/parabola](examples/parabola/) for a blueprint of how to use
-Cyantities with Boost.Units.
+Cyantities with Boost.Units, and the example of gravitational force on different
+masses in [examples/gravity](examples/gravity/) for different methods to iterate
+vector-valued quantities in C++.
 
 
 ## Python Known Units
 The following basic units are currently implemented in Cyantities and can be used
 to compose units based on the [coherent SI](#coherent-si-rule) or the [nominator-denominator](#nominator-denominator-rule) rule:
 
 | Python string | Unit          | Comment            |
@@ -476,14 +478,24 @@
 ## License
 This software is licensed under the European Public License (EUPL) version 1.2 or later.
 
 ## Changelog
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+### [0.1.0] - 2024-05-05
+#### Added
+- Add `zeros_like` generator function for `Quantity` (Cython only)
+- Add the `iter()` and `const_iter()` templated methods to C++
+  `QuantityWrapper` class, allowing for the use of range-based for loops and
+  range adaptor closures (`|`-operator syntax) in compile-time provided units.
+- Add the `gravity` example that showcases different methods to iterate
+  vector-valued quantities in C++.
+- Add benchmark for different iteration methods.
+
 ### [0.0.3] - 2024-04-24
 #### Changed
 - Fixed the installation requirements and source distribution manifest.
 - Add version coherence test script.
 
 ### [0.0.2] - 2024-04-23
 #### Changed
```

### Comparing `cyantities-0.0.3/README.md` & `cyantities-0.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -103,15 +103,17 @@
 dimensional correctness of the data passed from the Python level. Once this is done,
 the numerical data can similarly be transformed from the Python objects to the
 Boost.Units-powered C++ library.
 
 The interaction of Cyantities with Boost.Units is best explained through an
 example. See the example of a ball throw with gravity and friction in
 [examples/parabola](examples/parabola/) for a blueprint of how to use
-Cyantities with Boost.Units.
+Cyantities with Boost.Units, and the example of gravitational force on different
+masses in [examples/gravity](examples/gravity/) for different methods to iterate
+vector-valued quantities in C++.
 
 
 ## Python Known Units
 The following basic units are currently implemented in Cyantities and can be used
 to compose units based on the [coherent SI](#coherent-si-rule) or the [nominator-denominator](#nominator-denominator-rule) rule:
 
 | Python string | Unit          | Comment            |
@@ -166,14 +168,24 @@
 ## License
 This software is licensed under the European Public License (EUPL) version 1.2 or later.
 
 ## Changelog
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+### [0.1.0] - 2024-05-05
+#### Added
+- Add `zeros_like` generator function for `Quantity` (Cython only)
+- Add the `iter()` and `const_iter()` templated methods to C++
+  `QuantityWrapper` class, allowing for the use of range-based for loops and
+  range adaptor closures (`|`-operator syntax) in compile-time provided units.
+- Add the `gravity` example that showcases different methods to iterate
+  vector-valued quantities in C++.
+- Add benchmark for different iteration methods.
+
 ### [0.0.3] - 2024-04-24
 #### Changed
 - Fixed the installation requirements and source distribution manifest.
 - Add version coherence test script.
 
 ### [0.0.2] - 2024-04-23
 #### Changed
```

### Comparing `cyantities-0.0.3/cyantities/__init__.py` & `cyantities-0.1.0/cyantities/__init__.py`

 * *Files identical despite different names*

### Comparing `cyantities-0.0.3/cyantities/_cpp/cyantities/boost.hpp` & `cyantities-0.1.0/cyantities/_cpp/cyantities/boost.hpp`

 * *Files identical despite different names*

### Comparing `cyantities-0.0.3/cyantities/_cpp/cyantities/unit.hpp` & `cyantities-0.1.0/cyantities/_cpp/cyantities/unit.hpp`

 * *Files identical despite different names*

### Comparing `cyantities-0.0.3/cyantities/_cpp/src/quantitywrap.cpp` & `cyantities-0.1.0/cyantities/_cpp/src/quantitywrap.cpp`

 * *Files identical despite different names*

### Comparing `cyantities-0.0.3/cyantities/_cpp/src/unit.cpp` & `cyantities-0.1.0/cyantities/_cpp/src/unit.cpp`

 * *Files identical despite different names*

### Comparing `cyantities-0.0.3/cyantities/errors.py` & `cyantities-0.1.0/cyantities/errors.py`

 * *Files identical despite different names*

### Comparing `cyantities-0.0.3/cyantities/quantity.pxd` & `cyantities-0.1.0/cyantities/quantity.pxd`

 * *Files 4% similar despite different names*

```diff
@@ -43,8 +43,11 @@
     cdef object _val_object
     cdef CppUnit _unit
     cdef dict __dict__
 
     cdef _cyinit(self, bool is_scalar, double val, object val_object,
                  CppUnit unit)
 
-    cdef QuantityWrapper wrapper(self) nogil
+    cdef QuantityWrapper wrapper(self) nogil
+
+    @staticmethod
+    cdef Quantity zeros_like(Quantity other, object unit)
```

### Comparing `cyantities-0.0.3/cyantities/quantity.pyx` & `cyantities-0.1.0/cyantities/quantity.pyx`

 * *Files 5% similar despite different names*

```diff
@@ -245,57 +245,66 @@
     A physical quantity: a single or array of real numbers with an associated
     physical unit.
     """
     __dict__: dict
 
     def __init__(self, value, unit, bool copy=True):
         #
-        # First assign the values:
-        #
+        # First determine the values (scalar / ndarray)
+        # and setup all corresponding members for a call
+        # to _cyinit
+        #
+        cdef double d_value
+        cdef bool is_scalar
+        cdef object val_object
         if isinstance(value, float):
-            self._is_scalar = True
-            self._val = value
+            is_scalar = True
+            d_value = value
+            val_object = None
         elif isinstance(value, np.ndarray):
-            self._is_scalar = False
+            is_scalar = False
+            d_value = dummy_double[0]
             if copy:
-                self._val_ndarray = value.copy()
-                self._val_ndarray.flags['WRITEABLE'] = False
+                val_object = value.copy()
+                val_object.flags['WRITEABLE'] = False
             else:
-                self._val_ndarray = value
+                val_object = value
         else:
             raise TypeError("'value' has to be either a float or a NumPy array.")
 
         #
         # Then the unit:
         #
         cdef Unit unit_Unit
+        cdef CppUnit cpp_unit
         if isinstance(unit, Unit):
             unit_Unit = unit
-            self._unit = unit_Unit._unit
+            cpp_unit = unit_Unit._unit
         elif isinstance(unit, str):
-            self._unit = parse_unit(unit)
+            cpp_unit = parse_unit(unit)
 
         else:
             raise TypeError("'unit' has to be either a string or a Unit.")
 
-        # Set initialized:
-        self._initialized = True
+        self._cyinit(is_scalar, d_value, val_object, cpp_unit)
 
 
     cdef _cyinit(self, bool is_scalar, double val, object val_object,
                  CppUnit unit):
         if self._initialized:
             raise RuntimeError("Trying to initialize a second time.")
         self._is_scalar = is_scalar
         self._val = val
         cdef ndarray[dtype=float64_t] val_array
         if isinstance(val_object, np.ndarray):
             val_array = val_object.astype(np.float64, copy=False)
             self._val_ndarray = val_array
             self._val_object = val_array
+        else:
+            self._val_object = None
         self._unit = unit
 
         # Add, if dimensionless, the __array__ routine:
         if unit.dimensionless():
             self.__array__ = self._array
 
         self._initialized = True
@@ -516,38 +525,33 @@
             if self._is_scalar:
                 return float(self._val) == other
             return self._val_ndarray == other
 
         # Now compare quantities:
         cdef Quantity oq = other
         if not self._unit.same_dimension(oq._unit):
-            print("not same dimension.")
             return False
 
         # Check whether there's a scale difference:
         cdef CppUnit div_unit = self._unit / oq._unit
         cdef double scale = div_unit.total_scale()
         if scale == 1.0:
             # No scale difference. Make the two possible
             # comparisons:
             if self._is_scalar and oq._is_scalar:
-                print("scalars not equal.")
                 return self._val == oq._val
             elif not self._is_scalar and not oq._is_scalar:
-                print("arrays not equal.")
                 return self._val_ndarray == oq._val_ndarray
             return False
 
         # Have scale difference. Make the two possible
         # comparisons:
         if self._is_scalar and oq._is_scalar:
-            print("scalars not equal.")
             return self._val == scale*oq._val
         elif not self._is_scalar and not oq._is_scalar:
-            print("arrays not equal.")
             return self._val_ndarray == scale * oq._val_ndarray
         return False
 
 
     def unit(self) -> Unit:
         return generate_from_cpp(self._unit)
 
@@ -558,8 +562,45 @@
         """
         if self._is_scalar:
             return QuantityWrapper(self._val, self._unit)
         else:
             return QuantityWrapper(
                 <double*>self._val_ndarray.data,
                 self._val_ndarray.size,
-                self._unit)
+                self._unit)
+
+
+    @staticmethod
+    cdef Quantity zeros_like(Quantity other, object unit):
+        """
+        Returns a zero-value quantity with shape like another,
+        potentially with a different unit.
+        """
+        # First check the unit:
+        cdef Unit src_unit
+        cdef CppUnit dest_unit
+        if unit is None:
+            dest_unit = other._unit
+        elif isinstance(unit, str):
+            dest_unit = parse_unit(unit)
+        elif isinstance(unit, Unit):
+            src_unit = unit
+            dest_unit = src_unit._unit
+        else:
+            raise TypeError("'unit' must be a Unit instance, unit-specifying "
+                "string, or None."
+            )
+
+        # Now determine the shape of the target quantity:
+        cdef Quantity res = Quantity.__new__(Quantity)
+        if other._is_scalar:
+            res._cyinit(True, 0.0, None, dest_unit)
+
+        else:
+            # Generate a NumPy array with shape equal to the other
+            # quantity:
+            res._cyinit(False, dummy_double[0],
+                np.zeros_like(other._val_object),
+                dest_unit
+            )
+
+        return res
```

### Comparing `cyantities-0.0.3/cyantities/scripts/__init__.py` & `cyantities-0.1.0/cyantities/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `cyantities-0.0.3/cyantities/scripts/include.py` & `cyantities-0.1.0/cyantities/scripts/include.py`

 * *Files identical despite different names*

### Comparing `cyantities-0.0.3/cyantities/scripts/link.py` & `cyantities-0.1.0/cyantities/scripts/link.py`

 * *Files identical despite different names*

### Comparing `cyantities-0.0.3/cyantities/unit.pxd` & `cyantities-0.1.0/cyantities/unit.pxd`

 * *Files identical despite different names*

### Comparing `cyantities-0.0.3/cyantities/unit.pyx` & `cyantities-0.1.0/cyantities/unit.pyx`

 * *Files identical despite different names*

### Comparing `cyantities-0.0.3/examples/parabola/build.py` & `cyantities-0.1.0/examples/parabola/build.py`

 * *Files identical despite different names*

### Comparing `cyantities-0.0.3/examples/parabola/meson.build` & `cyantities-0.1.0/examples/parabola/meson.build`

 * *Files identical despite different names*

### Comparing `cyantities-0.0.3/examples/parabola/parasolve.cpp` & `cyantities-0.1.0/examples/parabola/parasolve.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,16 @@
  * limitations under the Licence.
  */
 
 
 #include <parasolve.hpp>
 #include <cyantities/boost.hpp>
 
+#include <numbers>
+
 #include <boost/units/quantity.hpp>
 #include <boost/units/systems/si/mass.hpp>
 #include <boost/units/systems/si/length.hpp>
 #include <boost/units/systems/si/area.hpp>
 #include <boost/units/systems/si/mass_density.hpp>
 #include <boost/units/systems/si/velocity.hpp>
 #include <boost/units/systems/si/acceleration.hpp>
```

### Comparing `cyantities-0.0.3/examples/parabola/parasolve.hpp` & `cyantities-0.1.0/examples/parabola/parasolve.hpp`

 * *Files identical despite different names*

### Comparing `cyantities-0.0.3/examples/parabola/parasolve.pyx` & `cyantities-0.1.0/examples/parabola/parasolve.pyx`

 * *Files identical despite different names*

### Comparing `cyantities-0.0.3/examples/parabola/run.py` & `cyantities-0.1.0/examples/parabola/run.py`

 * *Files identical despite different names*

### Comparing `cyantities-0.0.3/examples/parabola/subprojects/cyantities/meson.build` & `cyantities-0.1.0/examples/parabola/subprojects/cyantities/meson.build`

 * *Files identical despite different names*

### Comparing `cyantities-0.0.3/meson.build` & `cyantities-0.1.0/meson.build`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 project('cyantities', 'cpp', 'cython',
-        version : '0.0.3', default_options : ['optimization=3'])
+        version : '0.1.0', default_options : ['optimization=3'])
 
 
 #
 # Include directory:
 #
 incdir = include_directories('cyantities/_cpp/')
```

### Comparing `cyantities-0.0.3/pyproject.toml` & `cyantities-0.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["setuptools>=61", "wheel", "cython", "mebuex>=1.3.0", "numpy>=1.26"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Cyantities"
-version = "0.0.3"
+version = "0.1.0"
 authors = [
     {name = "Malte J. Ziebarth", email = "mjz.science@fmvkb.de"},
 ]
 description = """\
    Physical quantities with units."""
 dependencies = [
     "numpy",
     "cython",
     "mebuex"
 ]
 classifiers = [
-    "Development Status :: 1 - Planning",
+    "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: 3",
     "Programming Language :: Cython",
     "Programming Language :: C++",
     """License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)""",
     "Intended Audience :: Science/Research",
     "Natural Language :: English",
     "Operating System :: POSIX :: Linux"
```

### Comparing `cyantities-0.0.3/setup.py` & `cyantities-0.1.0/setup.py`

 * *Files identical despite different names*

