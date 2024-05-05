# Comparing `tmp/hueble-1.0.0.tar.gz` & `tmp/hueble-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hueble-1.0.0.tar", last modified: Sun May  5 16:41:04 2024, max compression
+gzip compressed data, was "hueble-1.0.1.tar", last modified: Sun May  5 18:05:26 2024, max compression
```

## Comparing `hueble-1.0.0.tar` & `hueble-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 16:41:04.252495 hueble-1.0.0/
-drwxrwxrwx   0        0        0        0 2024-05-05 16:41:04.248499 hueble-1.0.0/HueBLE.egg-info/
--rw-rw-rw-   0        0        0     5125 2024-05-05 16:41:04.000000 hueble-1.0.0/HueBLE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2024-05-05 16:41:04.000000 hueble-1.0.0/HueBLE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 16:41:04.000000 hueble-1.0.0/HueBLE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-05-05 16:41:04.000000 hueble-1.0.0/HueBLE.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-05 16:41:04.000000 hueble-1.0.0/HueBLE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    40554 2024-05-05 15:22:04.000000 hueble-1.0.0/HueBLE.py
--rw-rw-rw-   0        0        0     1091 2024-02-03 18:25:11.000000 hueble-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0     5125 2024-05-05 16:41:04.250494 hueble-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2701 2024-05-05 16:28:47.000000 hueble-1.0.0/README.md
--rw-rw-rw-   0        0        0     1172 2024-05-05 16:39:42.000000 hueble-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-05 16:41:04.253496 hueble-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-05 18:05:26.763859 hueble-1.0.1/
+drwxrwxrwx   0        0        0        0 2024-05-05 18:05:26.760859 hueble-1.0.1/HueBLE.egg-info/
+-rw-rw-rw-   0        0        0     5576 2024-05-05 18:05:26.000000 hueble-1.0.1/HueBLE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2024-05-05 18:05:26.000000 hueble-1.0.1/HueBLE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 18:05:26.000000 hueble-1.0.1/HueBLE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-05-05 18:05:26.000000 hueble-1.0.1/HueBLE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-05 18:05:26.000000 hueble-1.0.1/HueBLE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    40554 2024-05-05 15:22:04.000000 hueble-1.0.1/HueBLE.py
+-rw-rw-rw-   0        0        0     1091 2024-02-03 18:25:11.000000 hueble-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     5576 2024-05-05 18:05:26.762859 hueble-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3152 2024-05-05 17:44:36.000000 hueble-1.0.1/README.md
+-rw-rw-rw-   0        0        0     1172 2024-05-05 17:58:06.000000 hueble-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-05 18:05:26.763859 hueble-1.0.1/setup.cfg
```

### Comparing `hueble-1.0.0/HueBLE.egg-info/PKG-INFO` & `hueble-1.0.1/HueBLE.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HueBLE
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python module for controlling and monitoring Bluetooth Philips Hue bulbs
 Author-email: Harvey Lelliott <harveylelliott@duck.com>
 License: MIT License
         
         Copyright (c) 2024 Harvey Lelliott
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,19 +43,23 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: bleak>=0.19.0
 Requires-Dist: bleak-retry-connector
 
 # HueBLE
 
-![HueBLE logo](/hue_ble.png)
+![HueBLE logo](https://raw.githubusercontent.com/flip-dots/HueBLE/main/hue_ble.png)
 
+[![PyPI Status](https://img.shields.io/pypi/v/HueBLE.svg)](https://pypi.python.org/pypi/HueBLE)
+[![Documentation Status](https://readthedocs.org/projects/hueble/badge/?version=latest)](https://hueble.readthedocs.io/en/latest/?badge=latest)
+[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Python module for controlling Bluetooth Philips Hue lights.
  - 👌 Free software: MIT license
+ - 🍝 Sauce: https://github.com/flip-dots/HueBLE
  - 🖨️ Documentation: https://hueble.readthedocs.io/en/latest/
  - 📦 PIP: https://pypi.org/project/HueBLE/
 
 
 This Python module enables you to control Philips Hue Bluetooth lights directly
 from your computer, without the need for a Hue bridge or ZigBee dongle.
 It leverages the Bleak library to interact with Bluetooth Philips Hue lights.
```

### Comparing `hueble-1.0.0/HueBLE.py` & `hueble-1.0.1/HueBLE.py`

 * *Files identical despite different names*

### Comparing `hueble-1.0.0/LICENSE.txt` & `hueble-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hueble-1.0.0/PKG-INFO` & `hueble-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HueBLE
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python module for controlling and monitoring Bluetooth Philips Hue bulbs
 Author-email: Harvey Lelliott <harveylelliott@duck.com>
 License: MIT License
         
         Copyright (c) 2024 Harvey Lelliott
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,19 +43,23 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: bleak>=0.19.0
 Requires-Dist: bleak-retry-connector
 
 # HueBLE
 
-![HueBLE logo](/hue_ble.png)
+![HueBLE logo](https://raw.githubusercontent.com/flip-dots/HueBLE/main/hue_ble.png)
 
+[![PyPI Status](https://img.shields.io/pypi/v/HueBLE.svg)](https://pypi.python.org/pypi/HueBLE)
+[![Documentation Status](https://readthedocs.org/projects/hueble/badge/?version=latest)](https://hueble.readthedocs.io/en/latest/?badge=latest)
+[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Python module for controlling Bluetooth Philips Hue lights.
  - 👌 Free software: MIT license
+ - 🍝 Sauce: https://github.com/flip-dots/HueBLE
  - 🖨️ Documentation: https://hueble.readthedocs.io/en/latest/
  - 📦 PIP: https://pypi.org/project/HueBLE/
 
 
 This Python module enables you to control Philips Hue Bluetooth lights directly
 from your computer, without the need for a Hue bridge or ZigBee dongle.
 It leverages the Bleak library to interact with Bluetooth Philips Hue lights.
```

### Comparing `hueble-1.0.0/README.md` & `hueble-1.0.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # HueBLE
 
-![HueBLE logo](/hue_ble.png)
+![HueBLE logo](https://raw.githubusercontent.com/flip-dots/HueBLE/main/hue_ble.png)
 
+[![PyPI Status](https://img.shields.io/pypi/v/HueBLE.svg)](https://pypi.python.org/pypi/HueBLE)
+[![Documentation Status](https://readthedocs.org/projects/hueble/badge/?version=latest)](https://hueble.readthedocs.io/en/latest/?badge=latest)
+[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Python module for controlling Bluetooth Philips Hue lights.
  - 👌 Free software: MIT license
+ - 🍝 Sauce: https://github.com/flip-dots/HueBLE
  - 🖨️ Documentation: https://hueble.readthedocs.io/en/latest/
  - 📦 PIP: https://pypi.org/project/HueBLE/
 
 
 This Python module enables you to control Philips Hue Bluetooth lights directly
 from your computer, without the need for a Hue bridge or ZigBee dongle.
 It leverages the Bleak library to interact with Bluetooth Philips Hue lights.
```

### Comparing `hueble-1.0.0/pyproject.toml` & `hueble-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "HueBLE"
-version = "1.0.0"
+version = "1.0.1"
 dependencies = [
   "bleak>=0.19.0",
   "bleak-retry-connector"
 ]
 requires-python = ">=3.10"
 authors = [
   { name="Harvey Lelliott", email="harveylelliott@duck.com" },
```

