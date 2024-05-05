# Comparing `tmp/edterm-0.1.3.tar.gz` & `tmp/edterm-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edterm-0.1.3.tar", last modified: Sun May  5 00:50:46 2024, max compression
+gzip compressed data, was "edterm-0.1.4.tar", last modified: Sun May  5 01:16:05 2024, max compression
```

## Comparing `edterm-0.1.3.tar` & `edterm-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mpalermo  (1000) mpalermo  (1000)        0 2024-05-05 00:50:46.835874 edterm-0.1.3/
--rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)    11558 2024-05-04 21:25:08.000000 edterm-0.1.3/LICENSE
--rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)     3419 2024-05-05 00:50:46.835874 edterm-0.1.3/PKG-INFO
--rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)     2696 2024-05-04 23:41:32.000000 edterm-0.1.3/README.md
-drwxr-xr-x   0 mpalermo  (1000) mpalermo  (1000)        0 2024-05-05 00:50:46.835874 edterm-0.1.3/edterm/
--rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)        0 2024-05-04 21:27:52.000000 edterm-0.1.3/edterm/__init__.py
--rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)      265 2024-05-04 21:34:41.000000 edterm-0.1.3/edterm/data_reader.py
--rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)     8247 2024-05-05 00:42:13.000000 edterm-0.1.3/edterm/edterm.py
-drwxr-xr-x   0 mpalermo  (1000) mpalermo  (1000)        0 2024-05-05 00:50:46.835874 edterm-0.1.3/edterm.egg-info/
--rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)     3419 2024-05-05 00:50:46.000000 edterm-0.1.3/edterm.egg-info/PKG-INFO
--rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)      266 2024-05-05 00:50:46.000000 edterm-0.1.3/edterm.egg-info/SOURCES.txt
--rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)        1 2024-05-05 00:50:46.000000 edterm-0.1.3/edterm.egg-info/dependency_links.txt
--rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)       46 2024-05-05 00:50:46.000000 edterm-0.1.3/edterm.egg-info/entry_points.txt
--rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)       22 2024-05-05 00:50:46.000000 edterm-0.1.3/edterm.egg-info/requires.txt
--rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)        7 2024-05-05 00:50:46.000000 edterm-0.1.3/edterm.egg-info/top_level.txt
--rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)       38 2024-05-05 00:50:46.835874 edterm-0.1.3/setup.cfg
--rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)     1128 2024-05-05 00:44:27.000000 edterm-0.1.3/setup.py
+drwxr-xr-x   0 mpalermo  (1000) mpalermo  (1000)        0 2024-05-05 01:16:05.125741 edterm-0.1.4/
+-rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)    11558 2024-05-04 21:25:08.000000 edterm-0.1.4/LICENSE
+-rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)     3419 2024-05-05 01:16:05.115741 edterm-0.1.4/PKG-INFO
+-rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)     2696 2024-05-04 23:41:32.000000 edterm-0.1.4/README.md
+drwxr-xr-x   0 mpalermo  (1000) mpalermo  (1000)        0 2024-05-05 01:16:05.115741 edterm-0.1.4/edterm/
+-rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)        0 2024-05-04 21:27:52.000000 edterm-0.1.4/edterm/__init__.py
+-rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)      265 2024-05-04 21:34:41.000000 edterm-0.1.4/edterm/data_reader.py
+-rw-------   0 mpalermo  (1000) mpalermo  (1000)     8182 2024-05-05 01:11:32.000000 edterm-0.1.4/edterm/edterm.py
+drwxr-xr-x   0 mpalermo  (1000) mpalermo  (1000)        0 2024-05-05 01:16:05.115741 edterm-0.1.4/edterm.egg-info/
+-rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)     3419 2024-05-05 01:16:05.000000 edterm-0.1.4/edterm.egg-info/PKG-INFO
+-rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)      266 2024-05-05 01:16:05.000000 edterm-0.1.4/edterm.egg-info/SOURCES.txt
+-rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)        1 2024-05-05 01:16:05.000000 edterm-0.1.4/edterm.egg-info/dependency_links.txt
+-rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)       46 2024-05-05 01:16:05.000000 edterm-0.1.4/edterm.egg-info/entry_points.txt
+-rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)       22 2024-05-05 01:16:05.000000 edterm-0.1.4/edterm.egg-info/requires.txt
+-rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)        7 2024-05-05 01:16:05.000000 edterm-0.1.4/edterm.egg-info/top_level.txt
+-rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)       38 2024-05-05 01:16:05.125741 edterm-0.1.4/setup.cfg
+-rw-r--r--   0 mpalermo  (1000) mpalermo  (1000)     1128 2024-05-05 01:09:28.000000 edterm-0.1.4/setup.py
```

### Comparing `edterm-0.1.3/LICENSE` & `edterm-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `edterm-0.1.3/PKG-INFO` & `edterm-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edterm
-Version: 0.1.3
+Version: 0.1.4
 Summary: A terminal-based GROMACS EDR data plotting tool
 Home-page: https://github.com/mattiafelice-palermo/edterm
 Author: Mattia Felice Palermo
 Author-email: mattiafelice.palermo@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Visualization
```

### Comparing `edterm-0.1.3/README.md` & `edterm-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `edterm-0.1.3/edterm/edterm.py` & `edterm-0.1.4/edterm/edterm.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 import os
 import argparse
-import curses
 import pandas as pd
 from .data_reader import load_data
 import time
 import plotext
 import logging
+import locale
 
 def setup_environment():
     # Check and set environment variables for locale settings
     if os.environ.get('LANG', '') != 'en_US.UTF-8':
+        print("hmpg")
         os.environ['LANG'] = 'en_US.UTF-8'
     if os.environ.get('LC_ALL', '') != 'en_US.UTF-8':
         os.environ['LC_ALL'] = 'en_US.UTF-8'
+    # Set locale settings in the locale module
+    locale.setlocale(locale.LC_ALL, 'en_US.UTF-8')
+
+
+setup_environment()
+
+import curses
 
 def setup_logger():
     # Create a custom logger
     logger = logging.getLogger(__name__)
 
     # Set the log level
     logger.setLevel(logging.DEBUG)
@@ -112,19 +120,17 @@
     max_y, max_x = stdscr.getmaxyx()  # Initial size
     menu_width = 20  # Assume menu width to start
     first_draw = True
     last_number_time = time.time()
     input_mode = False
     resize_happened = True
     x_min, x_max = None, None
-    counter = 0
     number_buffer = ""
 
     while True:
-        counter += 1
         if input_mode:
             stdscr.nodelay(0)  # Switch to blocking mode for input
             stdscr.move(max_y-1, 0)
             stdscr.clrtoeol()
             stdscr.addstr(max_y-1, 0, "Provide the desired time window (x_min x_max): ")
             curses.echo()
             input_str = stdscr.getstr(max_y-1, 50).decode('utf-8')
@@ -139,24 +145,21 @@
             curses.noecho()
             input_mode = False
             stdscr.nodelay(1)  # Turn non-blocking mode back on
 
 
         new_max_y, new_max_x = stdscr.getmaxyx()
         if new_max_y != max_y or new_max_x != max_x:
-            logger.info(f"Resize happend! {counter}")
             max_y, max_x = new_max_y, new_max_x
             first_draw = True
             resize_happend = True
             stdscr.clear()  # Clear the screen because the terminal size has changed
             stdscr.refresh()
 
 
-        if not resize_happened: logger.info(f"Resize status {resize_happened}, {counter}")
-
         # Draw static elements only if they need to be redrawn or once
         if first_draw:
             stdscr.addstr(0, 0, "Welcome to the GROMACS Data Plotter Tool")
             stdscr.addstr(1, 0, f"File: {args.file}")
             stdscr.addstr(2, 0, "Press 'q' to quit. Use UP/DOWN arrows or type numbers to select.")
             first_draw = False
 
@@ -176,15 +179,14 @@
             last_index = current_index
             plot_width = max_x - menu_width - 5  # Calculate available width for plot
             plot_height = max_y - 5  # Calculate available height for plot
             plot_lines = plot_ascii(df, columns[current_index], plot_width, plot_height, x_min, x_max)
             plot_row = 4  # Starting row for plot
             stdscr.clrtobot()  # Clear from here to bottom of the screen
             for line in plot_lines:
-                logger.info(len(line))
                 if plot_row < max_y - 1:
                     parse_and_print_ansi(stdscr, plot_row, menu_width + 4, line)
                     plot_row += 1
             resize_happened = False
 
         stdscr.noutrefresh()
         curses.doupdate()
```

### Comparing `edterm-0.1.3/edterm.egg-info/PKG-INFO` & `edterm-0.1.4/edterm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edterm
-Version: 0.1.3
+Version: 0.1.4
 Summary: A terminal-based GROMACS EDR data plotting tool
 Home-page: https://github.com/mattiafelice-palermo/edterm
 Author: Mattia Felice Palermo
 Author-email: mattiafelice.palermo@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Visualization
```

### Comparing `edterm-0.1.3/setup.py` & `edterm-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='edterm',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     description='A terminal-based GROMACS EDR data plotting tool',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Mattia Felice Palermo',
     author_email='mattiafelice.palermo@gmail.com',
     url='https://github.com/mattiafelice-palermo/edterm',
```

