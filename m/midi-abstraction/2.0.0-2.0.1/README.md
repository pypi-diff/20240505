# Comparing `tmp/midi-abstraction-2.0.0.tar.gz` & `tmp/midi-abstraction-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midi-abstraction-2.0.0.tar", last modified: Sat May  4 06:27:35 2024, max compression
+gzip compressed data, was "midi-abstraction-2.0.1.tar", last modified: Sat May  4 16:47:40 2024, max compression
```

## Comparing `midi-abstraction-2.0.0.tar` & `midi-abstraction-2.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 cyberrumor  (1000) wheel      (998)        0 2024-05-04 06:27:35.254342 midi-abstraction-2.0.0/
--rw-r--r--   0 cyberrumor  (1000) wheel      (998)    35149 2024-04-30 01:45:13.000000 midi-abstraction-2.0.0/LICENSE
--rw-r--r--   0 cyberrumor  (1000) wheel      (998)     1781 2024-05-04 06:27:35.254342 midi-abstraction-2.0.0/PKG-INFO
--rwxr-xr-x   0 cyberrumor  (1000) wheel      (998)     1270 2024-05-04 05:46:43.000000 midi-abstraction-2.0.0/README.md
-drwxr-xr-x   0 cyberrumor  (1000) wheel      (998)        0 2024-05-04 06:27:35.251008 midi-abstraction-2.0.0/midi_abstraction/
--rwxr-xr-x   0 cyberrumor  (1000) wheel      (998)       32 2024-05-04 00:54:44.000000 midi-abstraction-2.0.0/midi_abstraction/__init__.py
--rwxr-xr-x   0 cyberrumor  (1000) wheel      (998)    15131 2024-05-04 05:17:50.000000 midi-abstraction-2.0.0/midi_abstraction/midi_abstraction.py
-drwxr-xr-x   0 cyberrumor  (1000) wheel      (998)        0 2024-05-04 06:27:35.254342 midi-abstraction-2.0.0/midi_abstraction.egg-info/
--rw-r--r--   0 cyberrumor  (1000) wheel      (998)     1781 2024-05-04 06:27:35.000000 midi-abstraction-2.0.0/midi_abstraction.egg-info/PKG-INFO
--rw-r--r--   0 cyberrumor  (1000) wheel      (998)      252 2024-05-04 06:27:35.000000 midi-abstraction-2.0.0/midi_abstraction.egg-info/SOURCES.txt
--rw-r--r--   0 cyberrumor  (1000) wheel      (998)        1 2024-05-04 06:27:35.000000 midi-abstraction-2.0.0/midi_abstraction.egg-info/dependency_links.txt
--rw-r--r--   0 cyberrumor  (1000) wheel      (998)       17 2024-05-04 06:27:35.000000 midi-abstraction-2.0.0/midi_abstraction.egg-info/top_level.txt
--rw-r--r--   0 cyberrumor  (1000) wheel      (998)       38 2024-05-04 06:27:35.254342 midi-abstraction-2.0.0/setup.cfg
--rwxr-xr-x   0 cyberrumor  (1000) wheel      (998)      787 2024-05-04 06:25:01.000000 midi-abstraction-2.0.0/setup.py
+drwxr-xr-x   0 cyberrumor  (1000) wheel      (998)        0 2024-05-04 16:47:40.635230 midi-abstraction-2.0.1/
+-rw-r--r--   0 cyberrumor  (1000) wheel      (998)    35149 2024-04-30 01:45:13.000000 midi-abstraction-2.0.1/LICENSE
+-rw-r--r--   0 cyberrumor  (1000) wheel      (998)     1781 2024-05-04 16:47:40.635230 midi-abstraction-2.0.1/PKG-INFO
+-rwxr-xr-x   0 cyberrumor  (1000) wheel      (998)     1270 2024-05-04 05:46:43.000000 midi-abstraction-2.0.1/README.md
+drwxr-xr-x   0 cyberrumor  (1000) wheel      (998)        0 2024-05-04 16:47:40.635230 midi-abstraction-2.0.1/midi_abstraction/
+-rwxr-xr-x   0 cyberrumor  (1000) wheel      (998)       32 2024-05-04 00:54:44.000000 midi-abstraction-2.0.1/midi_abstraction/__init__.py
+-rwxr-xr-x   0 cyberrumor  (1000) wheel      (998)    15112 2024-05-04 16:40:52.000000 midi-abstraction-2.0.1/midi_abstraction/midi_abstraction.py
+drwxr-xr-x   0 cyberrumor  (1000) wheel      (998)        0 2024-05-04 16:47:40.635230 midi-abstraction-2.0.1/midi_abstraction.egg-info/
+-rw-r--r--   0 cyberrumor  (1000) wheel      (998)     1781 2024-05-04 16:47:40.000000 midi-abstraction-2.0.1/midi_abstraction.egg-info/PKG-INFO
+-rw-r--r--   0 cyberrumor  (1000) wheel      (998)      252 2024-05-04 16:47:40.000000 midi-abstraction-2.0.1/midi_abstraction.egg-info/SOURCES.txt
+-rw-r--r--   0 cyberrumor  (1000) wheel      (998)        1 2024-05-04 16:47:40.000000 midi-abstraction-2.0.1/midi_abstraction.egg-info/dependency_links.txt
+-rw-r--r--   0 cyberrumor  (1000) wheel      (998)       17 2024-05-04 16:47:40.000000 midi-abstraction-2.0.1/midi_abstraction.egg-info/top_level.txt
+-rw-r--r--   0 cyberrumor  (1000) wheel      (998)       38 2024-05-04 16:47:40.635230 midi-abstraction-2.0.1/setup.cfg
+-rwxr-xr-x   0 cyberrumor  (1000) wheel      (998)      787 2024-05-04 16:42:21.000000 midi-abstraction-2.0.1/setup.py
```

### Comparing `midi-abstraction-2.0.0/LICENSE` & `midi-abstraction-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `midi-abstraction-2.0.0/PKG-INFO` & `midi-abstraction-2.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midi-abstraction
-Version: 2.0.0
+Version: 2.0.1
 Summary: Abstract MIDI pitches into keys, chords, modes, scales, and notes.
 Home-page: https://github.com/cyberrumor/midi-abstraction
 Author: Marco Silva
 Author-email: cyberrumor@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `midi-abstraction-2.0.0/README.md` & `midi-abstraction-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `midi-abstraction-2.0.0/midi_abstraction/midi_abstraction.py` & `midi-abstraction-2.0.1/midi_abstraction/midi_abstraction.py`

 * *Files 0% similar despite different names*

```diff
@@ -426,15 +426,15 @@
                 break
 
         results = []
         for i, step in enumerate(self.steps):
             if degree >= len(SCALE):
                 degree -= 12
 
-            results.append({n.value for n in SCALE[degree]})
+            results.append(SCALE[degree])
 
             degree += step
 
         return results
 
 
 IONIAN = Key(
```

### Comparing `midi-abstraction-2.0.0/midi_abstraction.egg-info/PKG-INFO` & `midi-abstraction-2.0.1/midi_abstraction.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midi-abstraction
-Version: 2.0.0
+Version: 2.0.1
 Summary: Abstract MIDI pitches into keys, chords, modes, scales, and notes.
 Home-page: https://github.com/cyberrumor/midi-abstraction
 Author: Marco Silva
 Author-email: cyberrumor@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `midi-abstraction-2.0.0/setup.py` & `midi-abstraction-2.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding = 'utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = 'midi-abstraction',
-    version = '2.0.0',
+    version = '2.0.1',
     author = 'Marco Silva',
     author_email = 'cyberrumor@gmail.com',
     description = 'Abstract MIDI pitches into keys, chords, modes, scales, and notes.',
     long_description_content_type = 'text/markdown',
     long_description = long_description,
     url = 'https://github.com/cyberrumor/midi-abstraction',
     packages = ['midi_abstraction'],
```

