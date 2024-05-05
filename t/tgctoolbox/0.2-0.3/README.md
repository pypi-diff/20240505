# Comparing `tmp/tgctoolbox-0.2.tar.gz` & `tmp/tgctoolbox-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgctoolbox-0.2.tar", max compression
+gzip compressed data, was "tgctoolbox-0.3.tar", max compression
```

## Comparing `tgctoolbox-0.2.tar` & `tgctoolbox-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      541 2024-05-05 11:52:14.312645 tgctoolbox-0.2/pyproject.toml
--rw-r--r--   0        0        0     1883 2024-05-05 11:34:10.191732 tgctoolbox-0.2/tgctoolbox/__init__.py
--rw-r--r--   0        0        0     2965 2024-04-14 10:00:56.065124 tgctoolbox-0.2/tgctoolbox/downloaders.py
--rw-r--r--   0        0        0     6398 2024-04-14 10:04:12.366063 tgctoolbox-0.2/tgctoolbox/ffmpeg.py
--rw-r--r--   0        0        0     3699 2024-04-04 14:07:33.674769 tgctoolbox-0.2/tgctoolbox/logger.py
--rw-r--r--   0        0        0      125 2024-04-04 14:07:33.502903 tgctoolbox-0.2/tgctoolbox/meta.py
--rw-r--r--   0        0        0     3532 2024-04-14 10:04:35.139755 tgctoolbox-0.2/tgctoolbox/operations.py
--rw-r--r--   0        0        0     2536 2024-04-14 10:05:13.288749 tgctoolbox-0.2/tgctoolbox/recorder.py
--rw-r--r--   0        0        0     7717 2024-05-05 11:42:16.815394 tgctoolbox-0.2/tgctoolbox/settings.py
--rw-r--r--   0        0        0     4338 2024-05-04 17:49:00.284883 tgctoolbox-0.2/tgctoolbox/sound.py
--rw-r--r--   0        0        0     2541 2024-04-14 10:05:55.801603 tgctoolbox-0.2/tgctoolbox/timing.py
--rw-r--r--   0        0        0     1787 2024-04-14 10:06:14.232604 tgctoolbox-0.2/tgctoolbox/vosk.py
--rw-r--r--   0        0        0     3415 2024-04-14 10:06:32.142449 tgctoolbox-0.2/tgctoolbox/wait_run.py
--rw-r--r--   0        0        0     2740 2024-04-13 22:34:12.249076 tgctoolbox-0.2/tgctoolbox/wrapper.py
--rw-r--r--   0        0        0      584 1970-01-01 00:00:00.000000 tgctoolbox-0.2/PKG-INFO
+-rw-r--r--   0        0        0      543 2024-05-05 11:57:18.837770 tgctoolbox-0.3/pyproject.toml
+-rw-r--r--   0        0        0     1883 2024-05-05 11:34:10.191732 tgctoolbox-0.3/tgctoolbox/__init__.py
+-rw-r--r--   0        0        0     2965 2024-04-14 10:00:56.065124 tgctoolbox-0.3/tgctoolbox/downloaders.py
+-rw-r--r--   0        0        0     6398 2024-04-14 10:04:12.366063 tgctoolbox-0.3/tgctoolbox/ffmpeg.py
+-rw-r--r--   0        0        0     3699 2024-04-04 14:07:33.674769 tgctoolbox-0.3/tgctoolbox/logger.py
+-rw-r--r--   0        0        0      125 2024-04-04 14:07:33.502903 tgctoolbox-0.3/tgctoolbox/meta.py
+-rw-r--r--   0        0        0     3532 2024-04-14 10:04:35.139755 tgctoolbox-0.3/tgctoolbox/operations.py
+-rw-r--r--   0        0        0     2536 2024-04-14 10:05:13.288749 tgctoolbox-0.3/tgctoolbox/recorder.py
+-rw-r--r--   0        0        0     7717 2024-05-05 11:42:16.815394 tgctoolbox-0.3/tgctoolbox/settings.py
+-rw-r--r--   0        0        0     4338 2024-05-04 17:49:00.284883 tgctoolbox-0.3/tgctoolbox/sound.py
+-rw-r--r--   0        0        0     2541 2024-04-14 10:05:55.801603 tgctoolbox-0.3/tgctoolbox/timing.py
+-rw-r--r--   0        0        0     1787 2024-04-14 10:06:14.232604 tgctoolbox-0.3/tgctoolbox/vosk.py
+-rw-r--r--   0        0        0     3415 2024-04-14 10:06:32.142449 tgctoolbox-0.3/tgctoolbox/wait_run.py
+-rw-r--r--   0        0        0     2740 2024-04-13 22:34:12.249076 tgctoolbox-0.3/tgctoolbox/wrapper.py
+-rw-r--r--   0        0        0      635 1970-01-01 00:00:00.000000 tgctoolbox-0.3/PKG-INFO
```

### Comparing `tgctoolbox-0.2/pyproject.toml` & `tgctoolbox-0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "tgctoolbox"
-version = "0.2"
+version = "0.3"
 description = "Comprehensive toolbox with all of the utils and tools used in various TGC projects."
 authors = ["Jakub Muszyński <jakub.m.muszynski@gmail.com>"]
 
 [tool.poetry.dependencies]
-python = "^3.12"
+python = "^3.11"
 pytube = "*"
 moviepy = "*"
 tqdm = "*"
 requests = "*"
 vosk = "*"
 websocket = "*"
 starlette = "*"
 colorama = "*"
-pyyaml = "^6.0.1"
+pyyaml = "^6.0.1"
 
 [tool.poetry.extras]
 audio = ["pyaudio"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `tgctoolbox-0.2/tgctoolbox/__init__.py` & `tgctoolbox-0.3/tgctoolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `tgctoolbox-0.2/tgctoolbox/downloaders.py` & `tgctoolbox-0.3/tgctoolbox/downloaders.py`

 * *Files identical despite different names*

### Comparing `tgctoolbox-0.2/tgctoolbox/ffmpeg.py` & `tgctoolbox-0.3/tgctoolbox/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `tgctoolbox-0.2/tgctoolbox/logger.py` & `tgctoolbox-0.3/tgctoolbox/logger.py`

 * *Files identical despite different names*

### Comparing `tgctoolbox-0.2/tgctoolbox/operations.py` & `tgctoolbox-0.3/tgctoolbox/operations.py`

 * *Files identical despite different names*

### Comparing `tgctoolbox-0.2/tgctoolbox/recorder.py` & `tgctoolbox-0.3/tgctoolbox/recorder.py`

 * *Files identical despite different names*

### Comparing `tgctoolbox-0.2/tgctoolbox/settings.py` & `tgctoolbox-0.3/tgctoolbox/settings.py`

 * *Files identical despite different names*

### Comparing `tgctoolbox-0.2/tgctoolbox/sound.py` & `tgctoolbox-0.3/tgctoolbox/sound.py`

 * *Files identical despite different names*

### Comparing `tgctoolbox-0.2/tgctoolbox/timing.py` & `tgctoolbox-0.3/tgctoolbox/timing.py`

 * *Files identical despite different names*

### Comparing `tgctoolbox-0.2/tgctoolbox/vosk.py` & `tgctoolbox-0.3/tgctoolbox/vosk.py`

 * *Files identical despite different names*

### Comparing `tgctoolbox-0.2/tgctoolbox/wait_run.py` & `tgctoolbox-0.3/tgctoolbox/wait_run.py`

 * *Files identical despite different names*

### Comparing `tgctoolbox-0.2/tgctoolbox/wrapper.py` & `tgctoolbox-0.3/tgctoolbox/wrapper.py`

 * *Files identical despite different names*

### Comparing `tgctoolbox-0.2/PKG-INFO` & `tgctoolbox-0.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: tgctoolbox
-Version: 0.2
+Version: 0.3
 Summary: Comprehensive toolbox with all of the utils and tools used in various TGC projects.
 Author: Jakub Muszyński
 Author-email: jakub.m.muszynski@gmail.com
-Requires-Python: >=3.12,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: audio
 Requires-Dist: colorama
 Requires-Dist: moviepy
 Requires-Dist: pytube
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests
```

