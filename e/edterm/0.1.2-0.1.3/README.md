# Comparing `tmp/edterm-0.1.2.tar.gz` & `tmp/edterm-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edterm-0.1.2.tar", last modified: Sat May  4 23:44:34 2024, max compression
+gzip compressed data, was "edterm-0.1.3.tar", last modified: Sun May  5 00:50:46 2024, max compression
```

## Comparing `edterm-0.1.2.tar` & `edterm-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mpalermo  (1000) mpalermo  (1000)        0 2024-05-04 23:44:34.896206 edterm-0.1.2/
--rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)    11558 2024-05-04 21:25:08.000000 edterm-0.1.2/LICENSE
--rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)     3419 2024-05-04 23:44:34.896206 edterm-0.1.2/PKG-INFO
--rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)     2696 2024-05-04 23:41:32.000000 edterm-0.1.2/README.md
-drwxr-xr-x   0 mpalermo  (1000) mpalermo  (1000)        0 2024-05-04 23:44:34.896206 edterm-0.1.2/edterm/
--rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)        0 2024-05-04 21:27:52.000000 edterm-0.1.2/edterm/__init__.py
--rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)      265 2024-05-04 21:34:41.000000 edterm-0.1.2/edterm/data_reader.py
--rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)     7881 2024-05-04 21:42:53.000000 edterm-0.1.2/edterm/edterm.py
-drwxr-xr-x   0 mpalermo  (1000) mpalermo  (1000)        0 2024-05-04 23:44:34.896206 edterm-0.1.2/edterm.egg-info/
--rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)     3419 2024-05-04 23:44:34.000000 edterm-0.1.2/edterm.egg-info/PKG-INFO
--rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)      266 2024-05-04 23:44:34.000000 edterm-0.1.2/edterm.egg-info/SOURCES.txt
--rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)        1 2024-05-04 23:44:34.000000 edterm-0.1.2/edterm.egg-info/dependency_links.txt
--rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)       46 2024-05-04 23:44:34.000000 edterm-0.1.2/edterm.egg-info/entry_points.txt
--rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)       22 2024-05-04 23:44:34.000000 edterm-0.1.2/edterm.egg-info/requires.txt
--rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)        7 2024-05-04 23:44:34.000000 edterm-0.1.2/edterm.egg-info/top_level.txt
--rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)       38 2024-05-04 23:44:34.896206 edterm-0.1.2/setup.cfg
--rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)     1128 2024-05-04 23:44:06.000000 edterm-0.1.2/setup.py
+drwxr-xr-x   0 mpalermo  (1000) mpalermo  (1000)        0 2024-05-05 00:50:46.835874 edterm-0.1.3/
+-rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)    11558 2024-05-04 21:25:08.000000 edterm-0.1.3/LICENSE
+-rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)     3419 2024-05-05 00:50:46.835874 edterm-0.1.3/PKG-INFO
+-rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)     2696 2024-05-04 23:41:32.000000 edterm-0.1.3/README.md
+drwxr-xr-x   0 mpalermo  (1000) mpalermo  (1000)        0 2024-05-05 00:50:46.835874 edterm-0.1.3/edterm/
+-rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)        0 2024-05-04 21:27:52.000000 edterm-0.1.3/edterm/__init__.py
+-rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)      265 2024-05-04 21:34:41.000000 edterm-0.1.3/edterm/data_reader.py
+-rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)     8247 2024-05-05 00:42:13.000000 edterm-0.1.3/edterm/edterm.py
+drwxr-xr-x   0 mpalermo  (1000) mpalermo  (1000)        0 2024-05-05 00:50:46.835874 edterm-0.1.3/edterm.egg-info/
+-rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)     3419 2024-05-05 00:50:46.000000 edterm-0.1.3/edterm.egg-info/PKG-INFO
+-rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)      266 2024-05-05 00:50:46.000000 edterm-0.1.3/edterm.egg-info/SOURCES.txt
+-rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)        1 2024-05-05 00:50:46.000000 edterm-0.1.3/edterm.egg-info/dependency_links.txt
+-rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)       46 2024-05-05 00:50:46.000000 edterm-0.1.3/edterm.egg-info/entry_points.txt
+-rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)       22 2024-05-05 00:50:46.000000 edterm-0.1.3/edterm.egg-info/requires.txt
+-rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)        7 2024-05-05 00:50:46.000000 edterm-0.1.3/edterm.egg-info/top_level.txt
+-rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)       38 2024-05-05 00:50:46.835874 edterm-0.1.3/setup.cfg
+-rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)     1128 2024-05-05 00:44:27.000000 edterm-0.1.3/setup.py
```

### Comparing `edterm-0.1.2/LICENSE` & `edterm-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `edterm-0.1.2/PKG-INFO` & `edterm-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edterm
-Version: 0.1.2
+Version: 0.1.3
 Summary: A terminal-based GROMACS EDR data plotting tool
 Home-page: https://github.com/mattiafelice-palermo/edterm
 Author: Mattia Felice Palermo
 Author-email: mattiafelice.palermo@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Visualization
```

### Comparing `edterm-0.1.2/README.md` & `edterm-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `edterm-0.1.2/edterm/edterm.py` & `edterm-0.1.3/edterm/edterm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,23 @@
+import os
 import argparse
 import curses
 import pandas as pd
 from .data_reader import load_data
 import time
 import plotext
 import logging
 
+def setup_environment():
+    # Check and set environment variables for locale settings
+    if os.environ.get('LANG', '') != 'en_US.UTF-8':
+        os.environ['LANG'] = 'en_US.UTF-8'
+    if os.environ.get('LC_ALL', '') != 'en_US.UTF-8':
+        os.environ['LC_ALL'] = 'en_US.UTF-8'
+
 def setup_logger():
     # Create a custom logger
     logger = logging.getLogger(__name__)
 
     # Set the log level
     logger.setLevel(logging.DEBUG)
 
@@ -86,14 +94,15 @@
 
     # Build the plot as a string
     plot_str = plotext.build()
     return plot_str.split('\n')
 
 
 def edterm_main(stdscr, args):
+    setup_environment()  # Ensure environment variables are correctly set
     logger = setup_logger()
     curses.curs_set(0)
     setup_colors()
     stdscr.nodelay(1)
     stdscr.clear()
 
     df = load_data(args.file)
```

### Comparing `edterm-0.1.2/edterm.egg-info/PKG-INFO` & `edterm-0.1.3/edterm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edterm
-Version: 0.1.2
+Version: 0.1.3
 Summary: A terminal-based GROMACS EDR data plotting tool
 Home-page: https://github.com/mattiafelice-palermo/edterm
 Author: Mattia Felice Palermo
 Author-email: mattiafelice.palermo@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Visualization
```

### Comparing `edterm-0.1.2/setup.py` & `edterm-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='edterm',
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(),
     description='A terminal-based GROMACS EDR data plotting tool',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Mattia Felice Palermo',
     author_email='mattiafelice.palermo@gmail.com',
     url='https://github.com/mattiafelice-palermo/edterm',
```

