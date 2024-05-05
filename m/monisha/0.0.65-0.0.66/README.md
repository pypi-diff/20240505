# Comparing `tmp/monisha-0.0.65.tar.gz` & `tmp/monisha-0.0.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monisha-0.0.65.tar", last modified: Fri May  3 12:19:06 2024, max compression
+gzip compressed data, was "monisha-0.0.66.tar", last modified: Sun May  5 06:11:07 2024, max compression
```

## Comparing `monisha-0.0.65.tar` & `monisha-0.0.66.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:19:06.250053 monisha-0.0.65/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-03 12:19:02.000000 monisha-0.0.65/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:19:06.242053 monisha-0.0.65/Monisha/
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:19:06.246053 monisha-0.0.65/Monisha/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function01.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function02.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function03.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function04.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function05.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function06.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function07.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function08.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function09.py
--rw-r--r--   0 runner    (1001) docker     (127)    60666 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function10.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function11.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function12.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function13.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function14.py
--rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function15.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function16.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function17.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function18.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function19.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:19:06.250053 monisha-0.0.65/Monisha/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/scripts/en.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/scripts/eo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/scripts/es.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-03 12:19:06.250053 monisha-0.0.65/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-03 12:19:02.000000 monisha-0.0.65/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:19:06.250053 monisha-0.0.65/monisha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-03 12:19:06.000000 monisha-0.0.65/monisha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-03 12:19:06.000000 monisha-0.0.65/monisha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 12:19:06.000000 monisha-0.0.65/monisha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-03 12:19:06.000000 monisha-0.0.65/monisha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-03 12:19:06.000000 monisha-0.0.65/monisha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 12:19:06.250053 monisha-0.0.65/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-03 12:19:02.000000 monisha-0.0.65/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:11:07.303020 monisha-0.0.66/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-05 06:11:02.000000 monisha-0.0.66/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:11:07.299020 monisha-0.0.66/Monisha/
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:11:07.303020 monisha-0.0.66/Monisha/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function02.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function04.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function06.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function07.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function08.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function09.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60666 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function13.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function14.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function15.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function17.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function18.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function19.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function20.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:11:07.303020 monisha-0.0.66/Monisha/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/scripts/en.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/scripts/eo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/scripts/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/scripts/eu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-05 06:11:07.303020 monisha-0.0.66/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-05 06:11:02.000000 monisha-0.0.66/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:11:07.303020 monisha-0.0.66/monisha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-05 06:11:07.000000 monisha-0.0.66/monisha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-05 06:11:07.000000 monisha-0.0.66/monisha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 06:11:07.000000 monisha-0.0.66/monisha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-05 06:11:07.000000 monisha-0.0.66/monisha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-05 06:11:07.000000 monisha-0.0.66/monisha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 06:11:07.303020 monisha-0.0.66/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-05 06:11:02.000000 monisha-0.0.66/setup.py
```

### Comparing `monisha-0.0.65/LICENSE` & `monisha-0.0.66/LICENSE`

 * *Files identical despite different names*

### Comparing `monisha-0.0.65/Monisha/__init__.py` & `monisha-0.0.66/Monisha/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 appname = "monisha"
-version = "0.0.65"
+version = "0.0.66"
 
 install = ["hachoir"]
 
 DATA01 = "clintonabrahamc@gmail.com"
 DATA02 = ['Natural Language :: English',
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
```

### Comparing `monisha-0.0.65/Monisha/functions/__init__.py` & `monisha-0.0.66/Monisha/functions/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from .function06 import Skeys, Uname
 from .function07 import Cmd, Wosd
 from .function18 import Metadatas
 from .function15 import Location
 from .function17 import Filename
 from .function09 import Storage
 from .function16 import FMagic
+from .function20 import Money
 from .function10 import Fonts
 from .function19 import views
 from .function11 import con2s
 from .function12 import YKeys
 from .function05 import Doxo
 from .function13 import Guid
 from .function08 import Num
```

### Comparing `monisha-0.0.65/Monisha/functions/function01.py` & `monisha-0.0.66/Monisha/functions/function01.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+import time
 from ..scripts import Scripted
 #=========================================================================
 
 def timend(tsize, dsize, speed):
     moonuo = round((tsize - dsize) / speed)
     return moonuo
 
 #=========================================================================
 
-def uptime(timetaken):
+def uptime(incoming):
+    timetaken = time.time() - incoming
     hours, hourz = divmod(timetaken, 3600)
     minutes, seconds = divmod(hourz, 60)
     return round(hours), round(minutes), round(seconds)
 
 #=========================================================================
 
 def Timemod(moonos: int) -> str:
```

### Comparing `monisha-0.0.65/Monisha/functions/function02.py` & `monisha-0.0.66/Monisha/functions/function02.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.65/Monisha/functions/function03.py` & `monisha-0.0.66/Monisha/functions/function03.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.65/Monisha/functions/function04.py` & `monisha-0.0.66/Monisha/functions/function04.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.65/Monisha/functions/function06.py` & `monisha-0.0.66/Monisha/functions/function06.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.65/Monisha/functions/function07.py` & `monisha-0.0.66/Monisha/functions/function07.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.65/Monisha/functions/function10.py` & `monisha-0.0.66/Monisha/functions/function10.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.65/Monisha/functions/function14.py` & `monisha-0.0.66/Monisha/functions/function14.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.65/Monisha/functions/function15.py` & `monisha-0.0.66/Monisha/functions/function15.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.65/Monisha/functions/function16.py` & `monisha-0.0.66/Monisha/functions/function16.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.65/Monisha/functions/function17.py` & `monisha-0.0.66/Monisha/functions/function17.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.65/Monisha/functions/function18.py` & `monisha-0.0.66/Monisha/functions/function18.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.65/Monisha/functions/function19.py` & `monisha-0.0.66/Monisha/functions/function19.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.65/Monisha/scripts/es.py` & `monisha-0.0.66/Monisha/scripts/es.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.65/PKG-INFO` & `monisha-0.0.66/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.65
+Version: 0.0.66
 Summary: ㅤ
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.65 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: monisha Version: 0.0.66 Summary: ã¤ Home-page:
 https://github.com/Clinton-Abraham Author: Clinton-Abraham Author-email:
 clintonabrahamc@gmail.com License: MIT Keywords: python,clinton,abraham
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
```

### Comparing `monisha-0.0.65/monisha.egg-info/PKG-INFO` & `monisha-0.0.66/monisha.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.65
+Version: 0.0.66
 Summary: ㅤ
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.65 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: monisha Version: 0.0.66 Summary: ã¤ Home-page:
 https://github.com/Clinton-Abraham Author: Clinton-Abraham Author-email:
 clintonabrahamc@gmail.com License: MIT Keywords: python,clinton,abraham
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
```

### Comparing `monisha-0.0.65/monisha.egg-info/SOURCES.txt` & `monisha-0.0.66/monisha.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -18,16 +18,18 @@
 Monisha/functions/function13.py
 Monisha/functions/function14.py
 Monisha/functions/function15.py
 Monisha/functions/function16.py
 Monisha/functions/function17.py
 Monisha/functions/function18.py
 Monisha/functions/function19.py
+Monisha/functions/function20.py
 Monisha/scripts/__init__.py
 Monisha/scripts/en.py
 Monisha/scripts/eo.py
 Monisha/scripts/es.py
+Monisha/scripts/eu.py
 monisha.egg-info/PKG-INFO
 monisha.egg-info/SOURCES.txt
 monisha.egg-info/dependency_links.txt
 monisha.egg-info/requires.txt
 monisha.egg-info/top_level.txt
```

### Comparing `monisha-0.0.65/setup.py` & `monisha-0.0.66/setup.py`

 * *Files identical despite different names*

