# Comparing `tmp/clickplc-0.8.2.tar.gz` & `tmp/clickplc-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickplc-0.8.2.tar", last modified: Fri Dec  8 18:23:52 2023, max compression
+gzip compressed data, was "clickplc-0.8.3.tar", last modified: Sun May  5 17:02:04 2024, max compression
```

## Comparing `clickplc-0.8.2.tar` & `clickplc-0.8.3.tar`

### file list

```diff
@@ -1,25 +1,19 @@
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-12-08 18:23:52.188697 clickplc-0.8.2/
--rw-r--r--   0 a.ruddick   (502) staff       (20)       69 2023-04-25 18:38:49.000000 clickplc-0.8.2/.gitignore
--rw-r--r--   0 a.ruddick   (502) staff       (20)    18026 2023-04-10 23:33:43.000000 clickplc-0.8.2/LICENSE
--rw-r--r--   0 a.ruddick   (502) staff       (20)       16 2023-02-06 20:30:11.000000 clickplc-0.8.2/MANIFEST.in
--rw-r--r--   0 a.ruddick   (502) staff       (20)     4088 2023-12-08 18:23:52.188621 clickplc-0.8.2/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2751 2023-06-28 18:39:31.000000 clickplc-0.8.2/README.md
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-12-08 18:23:52.185593 clickplc-0.8.2/clickplc/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1354 2022-11-17 00:56:19.000000 clickplc-0.8.2/clickplc/__init__.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)    23285 2023-08-30 15:47:42.000000 clickplc-0.8.2/clickplc/driver.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3065 2023-06-05 21:17:10.000000 clickplc-0.8.2/clickplc/mock.py
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-12-08 18:23:52.187223 clickplc-0.8.2/clickplc/tests/
--rw-r--r--   0 a.ruddick   (502) staff       (20)        0 2023-04-25 18:45:31.000000 clickplc-0.8.2/clickplc/tests/__init__.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)      190 2023-04-25 18:45:31.000000 clickplc-0.8.2/clickplc/tests/bad_tags.csv
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2306 2023-04-25 18:45:31.000000 clickplc-0.8.2/clickplc/tests/plc_tags.csv
--rw-r--r--   0 a.ruddick   (502) staff       (20)    10508 2023-04-25 18:45:31.000000 clickplc-0.8.2/clickplc/tests/test_driver.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     5510 2023-09-12 22:53:43.000000 clickplc-0.8.2/clickplc/util.py
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-12-08 18:23:52.186449 clickplc-0.8.2/clickplc.egg-info/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     4088 2023-12-08 18:23:52.000000 clickplc-0.8.2/clickplc.egg-info/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)      440 2023-12-08 18:23:52.000000 clickplc-0.8.2/clickplc.egg-info/SOURCES.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-12-08 18:23:52.000000 clickplc-0.8.2/clickplc.egg-info/dependency_links.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)       51 2023-12-08 18:23:52.000000 clickplc-0.8.2/clickplc.egg-info/entry_points.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      205 2023-12-08 18:23:52.000000 clickplc-0.8.2/clickplc.egg-info/requires.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        9 2023-12-08 18:23:52.000000 clickplc-0.8.2/clickplc.egg-info/top_level.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      161 2023-12-08 18:23:52.188928 clickplc-0.8.2/setup.cfg
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1685 2023-12-08 18:23:25.000000 clickplc-0.8.2/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-05 17:02:04.151769 clickplc-0.8.3/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    18026 2024-05-03 04:39:47.000000 clickplc-0.8.3/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)       16 2024-05-03 04:39:47.000000 clickplc-0.8.3/MANIFEST.in
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3713 2024-05-05 17:02:04.151769 clickplc-0.8.3/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2751 2024-05-03 04:39:47.000000 clickplc-0.8.3/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-05 17:02:04.151769 clickplc-0.8.3/clickplc/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1354 2024-05-03 04:39:47.000000 clickplc-0.8.3/clickplc/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    23301 2024-05-03 04:45:35.000000 clickplc-0.8.3/clickplc/driver.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3065 2024-05-03 04:39:47.000000 clickplc-0.8.3/clickplc/mock.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5510 2024-05-03 04:39:47.000000 clickplc-0.8.3/clickplc/util.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-05-05 17:02:04.151769 clickplc-0.8.3/clickplc.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3713 2024-05-05 17:02:04.000000 clickplc-0.8.3/clickplc.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      316 2024-05-05 17:02:04.000000 clickplc-0.8.3/clickplc.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2024-05-05 17:02:04.000000 clickplc-0.8.3/clickplc.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       52 2024-05-05 17:02:04.000000 clickplc-0.8.3/clickplc.egg-info/entry_points.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      206 2024-05-05 17:02:04.000000 clickplc-0.8.3/clickplc.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        9 2024-05-05 17:02:04.000000 clickplc-0.8.3/clickplc.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      161 2024-05-05 17:02:04.151769 clickplc-0.8.3/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1684 2024-05-05 16:58:24.000000 clickplc-0.8.3/setup.py
```

### Comparing `clickplc-0.8.2/LICENSE` & `clickplc-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clickplc-0.8.2/PKG-INFO` & `clickplc-0.8.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,32 @@
 Metadata-Version: 2.1
 Name: clickplc
-Version: 0.8.2
+Version: 0.8.3
 Summary: Python driver for Koyo Ethernet ClickPLCs.
 Home-page: https://github.com/numat/clickplc/
 Author: Patrick Fuller
 Author-email: pat@numat-tech.com
 Maintainer: Alex Ruddick
-Maintainer-email: alex@numat-tech.com
+Maintainer-email: alex@ruddick.tech
 License: GPLv2
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pymodbus>=2.4.0; python_version == "3.8"
-Requires-Dist: pymodbus>=2.4.0; python_version == "3.9"
-Requires-Dist: pymodbus<3.7.0,>=3.0.2; python_version >= "3.10"
 Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: pytest-cov; extra == "test"
-Requires-Dist: pytest-asyncio; extra == "test"
-Requires-Dist: mypy==1.7.1; extra == "test"
-Requires-Dist: ruff==0.1.7; extra == "test"
+License-File: LICENSE
 
 clickplc
 ========
 
 Python ≥3.8 driver and command-line tool for [Koyo Ethernet ClickPLCs](https://www.automationdirect.com/adc/Overview/Catalog/Programmable_Controllers/CLICK_Series_PLCs_(Stackable_Micro_Brick)).
 
 <p align="center">
@@ -123,7 +116,9 @@
     print(await plc.get())  # Get all named variables in tags file
 ```
 
 Additionally, the tags file can be used with the commandline tool to provide more informative output:
 ```
 $ clickplc the-plc-ip-address tags-filepath
 ```
+
+
```

### Comparing `clickplc-0.8.2/README.md` & `clickplc-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `clickplc-0.8.2/clickplc/__init__.py` & `clickplc-0.8.3/clickplc/__init__.py`

 * *Files identical despite different names*

### Comparing `clickplc-0.8.2/clickplc/driver.py` & `clickplc-0.8.3/clickplc/driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,15 +351,15 @@
         1-indexed notation). Each CTD entry takes 32 bits, which is 2 16bit registers.
         """
         if start < 1 or start > 250:
             raise ValueError('CTD must be in [1, 250]')
         if end is not None and (end < 1 or end > 250):
             raise ValueError('CTD end must be in [1, 250]')
 
-        address = 49152 + start - 1
+        address = 49152 + 2 * (start - 1)  # 32-bit
         count = 1 if end is None else (end - start + 1)
         registers = await self.read_registers(address, count * 2)
         bigendian = Endian.BIG if self.pymodbus35plus else Endian.Big  # type:ignore[attr-defined]
         lilendian = Endian.LITTLE if self.pymodbus35plus else Endian.Little  # type:ignore
         decoder = BinaryPayloadDecoder.fromRegisters(registers,
                                                      byteorder=bigendian,
                                                      wordorder=lilendian)
```

### Comparing `clickplc-0.8.2/clickplc/mock.py` & `clickplc-0.8.3/clickplc/mock.py`

 * *Files identical despite different names*

### Comparing `clickplc-0.8.2/clickplc/util.py` & `clickplc-0.8.3/clickplc/util.py`

 * *Files identical despite different names*

### Comparing `clickplc-0.8.2/clickplc.egg-info/PKG-INFO` & `clickplc-0.8.3/clickplc.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,32 @@
 Metadata-Version: 2.1
 Name: clickplc
-Version: 0.8.2
+Version: 0.8.3
 Summary: Python driver for Koyo Ethernet ClickPLCs.
 Home-page: https://github.com/numat/clickplc/
 Author: Patrick Fuller
 Author-email: pat@numat-tech.com
 Maintainer: Alex Ruddick
-Maintainer-email: alex@numat-tech.com
+Maintainer-email: alex@ruddick.tech
 License: GPLv2
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pymodbus>=2.4.0; python_version == "3.8"
-Requires-Dist: pymodbus>=2.4.0; python_version == "3.9"
-Requires-Dist: pymodbus<3.7.0,>=3.0.2; python_version >= "3.10"
 Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: pytest-cov; extra == "test"
-Requires-Dist: pytest-asyncio; extra == "test"
-Requires-Dist: mypy==1.7.1; extra == "test"
-Requires-Dist: ruff==0.1.7; extra == "test"
+License-File: LICENSE
 
 clickplc
 ========
 
 Python ≥3.8 driver and command-line tool for [Koyo Ethernet ClickPLCs](https://www.automationdirect.com/adc/Overview/Catalog/Programmable_Controllers/CLICK_Series_PLCs_(Stackable_Micro_Brick)).
 
 <p align="center">
@@ -123,7 +116,9 @@
     print(await plc.get())  # Get all named variables in tags file
 ```
 
 Additionally, the tags file can be used with the commandline tool to provide more informative output:
 ```
 $ clickplc the-plc-ip-address tags-filepath
 ```
+
+
```

### Comparing `clickplc-0.8.2/setup.py` & `clickplc-0.8.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,39 +3,39 @@
 from setuptools import setup
 
 with open('README.md') as in_file:
     long_description = in_file.read()
 
 setup(
     name='clickplc',
-    version='0.8.2',
+    version='0.8.3',
     description="Python driver for Koyo Ethernet ClickPLCs.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/numat/clickplc/',
     author='Patrick Fuller',
     author_email='pat@numat-tech.com',
     maintainer='Alex Ruddick',
-    maintainer_email='alex@numat-tech.com',
+    maintainer_email='alex@ruddick.tech',
     packages=['clickplc'],
     entry_points={
         'console_scripts': [('clickplc = clickplc:command_line')]
     },
     install_requires=[
         'pymodbus>=2.4.0; python_version == "3.8"',
         'pymodbus>=2.4.0; python_version == "3.9"',
         'pymodbus>=3.0.2,<3.7.0; python_version >= "3.10"',
     ],
     extras_require={
         'test': [
             'pytest',
             'pytest-cov',
             'pytest-asyncio',
-            'mypy==1.7.1',
-            'ruff==0.1.7',
+            'mypy==1.10.0',
+            'ruff==0.4.2',
         ],
     },
     license='GPLv2',
     classifiers=[
         'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
         'Development Status :: 4 - Beta',
         'Natural Language :: English',
```

