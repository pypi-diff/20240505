# Comparing `tmp/skrutable-1.2.0.tar.gz` & `tmp/skrutable-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skrutable-1.2.0.tar", last modified: Sat Jan  7 22:17:17 2023, max compression
+gzip compressed data, was "skrutable-1.2.1.tar", last modified: Sun May  5 02:37:52 2024, max compression
```

## Comparing `skrutable-1.2.0.tar` & `skrutable-1.2.1.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxr-xr-x   0 tylerneill   (503) staff       (20)        0 2023-01-07 22:17:17.178486 skrutable-1.2.0/
--rw-r--r--   0 tylerneill   (503) staff       (20)      165 2023-01-06 04:21:46.000000 skrutable-1.2.0/LICENSE.md
--rw-r--r--   0 tylerneill   (503) staff       (20)       50 2023-01-07 21:30:02.000000 skrutable-1.2.0/MANIFEST.in
--rw-r--r--   0 tylerneill   (503) staff       (20)     1126 2023-01-07 22:17:17.178564 skrutable-1.2.0/PKG-INFO
--rw-r--r--   0 tylerneill   (503) staff       (20)      106 2023-01-07 22:17:17.178797 skrutable-1.2.0/setup.cfg
--rw-r--r--   0 tylerneill   (503) staff       (20)     1015 2023-01-07 21:57:22.000000 skrutable-1.2.0/setup.py
-drwxr-xr-x   0 tylerneill   (503) staff       (20)        0 2023-01-07 22:17:17.171122 skrutable-1.2.0/src/
-drwxr-xr-x   0 tylerneill   (503) staff       (20)        0 2023-01-07 22:17:17.177506 skrutable-1.2.0/src/skrutable/
--rw-r--r--   0 tylerneill   (503) staff       (20)      716 2023-01-07 22:16:24.000000 skrutable-1.2.0/src/skrutable/README.md
--rw-r--r--   0 tylerneill   (503) staff       (20)       21 2023-01-07 22:16:54.000000 skrutable-1.2.0/src/skrutable/__init__.py
--rw-r--r--   0 tylerneill   (503) staff       (20)     1077 2023-01-07 22:16:18.000000 skrutable-1.2.0/src/skrutable/config.json
--rw-r--r--   0 tylerneill   (503) staff       (20)      281 2023-01-07 22:16:18.000000 skrutable-1.2.0/src/skrutable/config.py
--rw-r--r--   0 tylerneill   (503) staff       (20)    16633 2023-01-07 22:16:19.000000 skrutable-1.2.0/src/skrutable/manual.md
--rw-r--r--   0 tylerneill   (503) staff       (20)    26789 2023-01-07 22:16:19.000000 skrutable-1.2.0/src/skrutable/meter_identification.py
--rw-r--r--   0 tylerneill   (503) staff       (20)    12348 2023-01-07 22:16:19.000000 skrutable-1.2.0/src/skrutable/meter_patterns.py
--rw-r--r--   0 tylerneill   (503) staff       (20)     4957 2023-01-07 22:16:19.000000 skrutable-1.2.0/src/skrutable/phonemes.py
--rw-r--r--   0 tylerneill   (503) staff       (20)    10736 2023-01-07 22:16:19.000000 skrutable-1.2.0/src/skrutable/scansion.py
--rw-r--r--   0 tylerneill   (503) staff       (20)     1339 2023-01-07 22:16:19.000000 skrutable-1.2.0/src/skrutable/scheme_detection.py
--rw-r--r--   0 tylerneill   (503) staff       (20)    17766 2023-01-07 22:16:19.000000 skrutable-1.2.0/src/skrutable/scheme_maps.py
--rw-r--r--   0 tylerneill   (503) staff       (20)   212298 2023-01-07 22:16:19.000000 skrutable-1.2.0/src/skrutable/scheme_vectors_mbh.py
--rw-r--r--   0 tylerneill   (503) staff       (20)     2933 2023-01-07 22:16:19.000000 skrutable-1.2.0/src/skrutable/skrutable_one.py
-drwxr-xr-x   0 tylerneill   (503) staff       (20)        0 2023-01-07 22:17:17.178300 skrutable-1.2.0/src/skrutable/splitter/
--rw-r--r--   0 tylerneill   (503) staff       (20)     7878 2023-01-07 22:16:19.000000 skrutable-1.2.0/src/skrutable/splitter/wrapper.py
--rw-r--r--   0 tylerneill   (503) staff       (20)     5532 2023-01-07 22:16:19.000000 skrutable-1.2.0/src/skrutable/transliteration.py
--rw-r--r--   0 tylerneill   (503) staff       (20)     1435 2023-01-07 22:16:19.000000 skrutable-1.2.0/src/skrutable/virAma_avoidance.py
-drwxr-xr-x   0 tylerneill   (503) staff       (20)        0 2023-01-07 22:17:17.178143 skrutable-1.2.0/src/skrutable.egg-info/
--rw-r--r--   0 tylerneill   (503) staff       (20)     1126 2023-01-07 22:17:17.000000 skrutable-1.2.0/src/skrutable.egg-info/PKG-INFO
--rw-r--r--   0 tylerneill   (503) staff       (20)      666 2023-01-07 22:17:17.000000 skrutable-1.2.0/src/skrutable.egg-info/SOURCES.txt
--rw-r--r--   0 tylerneill   (503) staff       (20)        1 2023-01-07 22:17:17.000000 skrutable-1.2.0/src/skrutable.egg-info/dependency_links.txt
--rw-r--r--   0 tylerneill   (503) staff       (20)       10 2023-01-07 22:17:17.000000 skrutable-1.2.0/src/skrutable.egg-info/top_level.txt
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-05 02:37:52.351500 skrutable-1.2.1/
+-rw-r--r--   0 tyler      (501) staff       (20)      165 2024-05-05 02:36:03.000000 skrutable-1.2.1/LICENSE.md
+-rw-r--r--   0 tyler      (501) staff       (20)      409 2024-05-05 02:37:52.351446 skrutable-1.2.1/PKG-INFO
+-rw-r--r--   0 tyler      (501) staff       (20)      716 2024-05-05 02:06:10.000000 skrutable-1.2.1/README.md
+-rw-r--r--   0 tyler      (501) staff       (20)      106 2024-05-05 02:37:52.351694 skrutable-1.2.1/setup.cfg
+-rw-r--r--   0 tyler      (501) staff       (20)      779 2024-05-05 02:36:42.000000 skrutable-1.2.1/setup.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-05 02:37:52.345083 skrutable-1.2.1/src/
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-05 02:37:52.350210 skrutable-1.2.1/src/skrutable/
+-rw-r--r--   0 tyler      (501) staff       (20)     1077 2024-05-05 02:06:10.000000 skrutable-1.2.1/src/skrutable/config.json
+-rw-r--r--   0 tyler      (501) staff       (20)      281 2024-05-05 02:06:10.000000 skrutable-1.2.1/src/skrutable/config.py
+-rw-r--r--   0 tyler      (501) staff       (20)    16697 2024-05-05 02:06:10.000000 skrutable-1.2.1/src/skrutable/manual.md
+-rw-r--r--   0 tyler      (501) staff       (20)    26789 2024-05-05 02:06:10.000000 skrutable-1.2.1/src/skrutable/meter_identification.py
+-rw-r--r--   0 tyler      (501) staff       (20)    12348 2024-05-05 02:06:10.000000 skrutable-1.2.1/src/skrutable/meter_patterns.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4957 2024-05-05 02:06:10.000000 skrutable-1.2.1/src/skrutable/phonemes.py
+-rw-r--r--   0 tyler      (501) staff       (20)    10736 2024-05-05 02:06:10.000000 skrutable-1.2.1/src/skrutable/scansion.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1339 2024-05-05 02:06:10.000000 skrutable-1.2.1/src/skrutable/scheme_detection.py
+-rw-r--r--   0 tyler      (501) staff       (20)    17766 2024-05-05 02:06:10.000000 skrutable-1.2.1/src/skrutable/scheme_maps.py
+-rw-r--r--   0 tyler      (501) staff       (20)   212298 2024-05-05 02:06:10.000000 skrutable-1.2.1/src/skrutable/scheme_vectors_mbh.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2933 2024-05-05 02:06:10.000000 skrutable-1.2.1/src/skrutable/skrutable_one.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-05 02:37:52.350929 skrutable-1.2.1/src/skrutable/splitter/
+-rw-r--r--   0 tyler      (501) staff       (20)     7878 2024-05-05 02:06:10.000000 skrutable-1.2.1/src/skrutable/splitter/wrapper.py
+-rw-r--r--   0 tyler      (501) staff       (20)     5532 2024-05-05 02:06:10.000000 skrutable-1.2.1/src/skrutable/transliteration.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1435 2024-05-05 02:06:10.000000 skrutable-1.2.1/src/skrutable/virAma_avoidance.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-05-05 02:37:52.351241 skrutable-1.2.1/src/skrutable.egg-info/
+-rw-r--r--   0 tyler      (501) staff       (20)      409 2024-05-05 02:37:52.000000 skrutable-1.2.1/src/skrutable.egg-info/PKG-INFO
+-rw-r--r--   0 tyler      (501) staff       (20)      650 2024-05-05 02:37:52.000000 skrutable-1.2.1/src/skrutable.egg-info/SOURCES.txt
+-rw-r--r--   0 tyler      (501) staff       (20)        1 2024-05-05 02:37:52.000000 skrutable-1.2.1/src/skrutable.egg-info/dependency_links.txt
+-rw-r--r--   0 tyler      (501) staff       (20)       15 2024-05-05 02:37:52.000000 skrutable-1.2.1/src/skrutable.egg-info/requires.txt
+-rw-r--r--   0 tyler      (501) staff       (20)       10 2024-05-05 02:37:52.000000 skrutable-1.2.1/src/skrutable.egg-info/top_level.txt
```

### Comparing `skrutable-1.2.0/src/skrutable/README.md` & `skrutable-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `skrutable-1.2.0/src/skrutable/config.json` & `skrutable-1.2.1/src/skrutable/config.json`

 * *Files identical despite different names*

### Comparing `skrutable-1.2.0/src/skrutable/manual.md` & `skrutable-1.2.1/src/skrutable/manual.md`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
 
 # using the code
 
 ## installation
 
 1. Have Python 3 installed (`Homebrew` and Python 3.8+ recommended)
 
-2. Run `pip3 install skrutable`
+2. Run `pip3 install skrutable` ([latest version on PyPi](https://pypi.org/project/skrutable/))
 
 ## objects
 
 From each respective Python module (`transliteration.py`, `scansion.py`, `meter_identification.py`, `splitter.wrapper.py`), import the respective object constructor (`Transliterator`, `Scanner`, `MeterIdentifier`, `Splitter`), instantiate the object, and call its primary methods (`transliterate()`, `scan()`, `identify_meter()`, `split()`). Transliteration and sandhi/compound splitting both return strings, whereas scansion and meter identification return `Scansion.Verse` objects, which themselves contain (among other things) a `meter_label` string attribute and a `summarize()` method that returns a string.
 
 The following are the important function parameters:
```

#### html2text {}

```diff
@@ -119,16 +119,17 @@
 (https://splitter-server-tylergneill.pythonanywhere.com/)), so you'll need a
 working internet connection for this functionality. (A previous, offline
 solution for incorporating the splitter involved requiring the user to set up
 `TensorFlow 1.x` on `Python 3.5` and to bridge different versions of Python
 with inelegant path hacks. Remnants of this still remain in the codebase and
 can be made to work if needed but are totally inactive at present.) # using the
 code ## installation 1. Have Python 3 installed (`Homebrew` and Python 3.8+
-recommended) 2. Run `pip3 install skrutable` ## objects From each respective
-Python module (`transliteration.py`, `scansion.py`, `meter_identification.py`,
+recommended) 2. Run `pip3 install skrutable` ([latest version on PyPi](https://
+pypi.org/project/skrutable/)) ## objects From each respective Python module
+(`transliteration.py`, `scansion.py`, `meter_identification.py`,
 `splitter.wrapper.py`), import the respective object constructor
 (`Transliterator`, `Scanner`, `MeterIdentifier`, `Splitter`), instantiate the
 object, and call its primary methods (`transliterate()`, `scan()`,
 `identify_meter()`, `split()`). Transliteration and sandhi/compound splitting
 both return strings, whereas scansion and meter identification return
 `Scansion.Verse` objects, which themselves contain (among other things) a
 `meter_label` string attribute and a `summarize()` method that returns a
```

### Comparing `skrutable-1.2.0/src/skrutable/meter_identification.py` & `skrutable-1.2.1/src/skrutable/meter_identification.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.2.0/src/skrutable/meter_patterns.py` & `skrutable-1.2.1/src/skrutable/meter_patterns.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.2.0/src/skrutable/phonemes.py` & `skrutable-1.2.1/src/skrutable/phonemes.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.2.0/src/skrutable/scansion.py` & `skrutable-1.2.1/src/skrutable/scansion.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.2.0/src/skrutable/scheme_detection.py` & `skrutable-1.2.1/src/skrutable/scheme_detection.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.2.0/src/skrutable/scheme_maps.py` & `skrutable-1.2.1/src/skrutable/scheme_maps.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.2.0/src/skrutable/scheme_vectors_mbh.py` & `skrutable-1.2.1/src/skrutable/scheme_vectors_mbh.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.2.0/src/skrutable/skrutable_one.py` & `skrutable-1.2.1/src/skrutable/skrutable_one.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.2.0/src/skrutable/splitter/wrapper.py` & `skrutable-1.2.1/src/skrutable/splitter/wrapper.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.2.0/src/skrutable/transliteration.py` & `skrutable-1.2.1/src/skrutable/transliteration.py`

 * *Files identical despite different names*

### Comparing `skrutable-1.2.0/src/skrutable/virAma_avoidance.py` & `skrutable-1.2.1/src/skrutable/virAma_avoidance.py`

 * *Files identical despite different names*

