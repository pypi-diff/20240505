# Comparing `tmp/pymusiclooper-3.4.0.tar.gz` & `tmp/pymusiclooper-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymusiclooper-3.4.0.tar", max compression
+gzip compressed data, was "pymusiclooper-3.4.1.tar", max compression
```

## Comparing `pymusiclooper-3.4.0.tar` & `pymusiclooper-3.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1067 2024-04-25 16:23:19.776152 pymusiclooper-3.4.0/LICENSE
--rw-r--r--   0        0        0     9359 2024-04-25 16:23:19.776152 pymusiclooper-3.4.0/README.md
--rw-r--r--   0        0        0       72 2024-04-25 16:23:19.776152 pymusiclooper-3.4.0/pymusiclooper/__init__.py
--rw-r--r--   0        0        0      212 2024-04-25 16:23:19.776152 pymusiclooper-3.4.0/pymusiclooper/__main__.py
--rw-r--r--   0        0        0    24198 2024-04-25 16:23:19.780153 pymusiclooper-3.4.0/pymusiclooper/analysis.py
--rw-r--r--   0        0        0     3749 2024-04-25 16:23:19.780153 pymusiclooper-3.4.0/pymusiclooper/audio.py
--rw-r--r--   0        0        0    12613 2024-04-25 16:23:19.780153 pymusiclooper-3.4.0/pymusiclooper/cli.py
--rw-r--r--   0        0        0     1953 2024-04-25 16:23:19.780153 pymusiclooper-3.4.0/pymusiclooper/console.py
--rw-r--r--   0        0        0    14568 2024-04-25 16:23:19.780153 pymusiclooper-3.4.0/pymusiclooper/core.py
--rw-r--r--   0        0        0      205 2024-04-25 16:23:19.780153 pymusiclooper-3.4.0/pymusiclooper/exceptions.py
--rw-r--r--   0        0        0    17841 2024-04-25 16:23:19.780153 pymusiclooper-3.4.0/pymusiclooper/handler.py
--rw-r--r--   0        0        0     6108 2024-04-25 16:23:19.780153 pymusiclooper-3.4.0/pymusiclooper/playback.py
--rw-r--r--   0        0        0     1933 2024-04-25 16:23:19.780153 pymusiclooper-3.4.0/pymusiclooper/utils.py
--rw-r--r--   0        0        0     2327 2024-04-25 16:23:19.780153 pymusiclooper-3.4.0/pymusiclooper/youtube.py
--rw-r--r--   0        0        0     1720 2024-04-25 16:23:19.780153 pymusiclooper-3.4.0/pyproject.toml
--rw-r--r--   0        0        0    11020 1970-01-01 00:00:00.000000 pymusiclooper-3.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-05 10:15:22.298101 pymusiclooper-3.4.1/LICENSE
+-rw-r--r--   0        0        0     9359 2024-05-05 10:15:22.298101 pymusiclooper-3.4.1/README.md
+-rw-r--r--   0        0        0       72 2024-05-05 10:15:22.302101 pymusiclooper-3.4.1/pymusiclooper/__init__.py
+-rw-r--r--   0        0        0      212 2024-05-05 10:15:22.302101 pymusiclooper-3.4.1/pymusiclooper/__main__.py
+-rw-r--r--   0        0        0    24264 2024-05-05 10:15:22.302101 pymusiclooper-3.4.1/pymusiclooper/analysis.py
+-rw-r--r--   0        0        0     3749 2024-05-05 10:15:22.302101 pymusiclooper-3.4.1/pymusiclooper/audio.py
+-rw-r--r--   0        0        0    12608 2024-05-05 10:15:22.302101 pymusiclooper-3.4.1/pymusiclooper/cli.py
+-rw-r--r--   0        0        0     1953 2024-05-05 10:15:22.302101 pymusiclooper-3.4.1/pymusiclooper/console.py
+-rw-r--r--   0        0        0    14568 2024-05-05 10:15:22.302101 pymusiclooper-3.4.1/pymusiclooper/core.py
+-rw-r--r--   0        0        0      205 2024-05-05 10:15:22.302101 pymusiclooper-3.4.1/pymusiclooper/exceptions.py
+-rw-r--r--   0        0        0    17841 2024-05-05 10:15:22.302101 pymusiclooper-3.4.1/pymusiclooper/handler.py
+-rw-r--r--   0        0        0     6108 2024-05-05 10:15:22.302101 pymusiclooper-3.4.1/pymusiclooper/playback.py
+-rw-r--r--   0        0        0     1933 2024-05-05 10:15:22.302101 pymusiclooper-3.4.1/pymusiclooper/utils.py
+-rw-r--r--   0        0        0     2327 2024-05-05 10:15:22.302101 pymusiclooper-3.4.1/pymusiclooper/youtube.py
+-rw-r--r--   0        0        0     1516 2024-05-05 10:15:22.302101 pymusiclooper-3.4.1/pyproject.toml
+-rw-r--r--   0        0        0    10958 1970-01-01 00:00:00.000000 pymusiclooper-3.4.1/PKG-INFO
```

### Comparing `pymusiclooper-3.4.0/LICENSE` & `pymusiclooper-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymusiclooper-3.4.0/README.md` & `pymusiclooper-3.4.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 - Export the loop points as metadata tags to a copy of the input audio file(s), for use with game engines, etc.
 - Export a longer, extended version of an audio track by looping it seamlessly to the desired length
 
 ## Pre-requisites
 
 The following software must be installed for `pymusiclooper` to function correctly.
 
-- [Python (64-bit)](https://www.python.org/downloads/) >= 3.8
+- [Python (64-bit)](https://www.python.org/downloads/) >= 3.9
 - [ffmpeg](https://ffmpeg.org/download.html): required for loading audio from youtube (or any stream supported by [yt-dlp](https://github.com/yt-dlp/yt-dlp)) and adds support for loading additional audio formats and codecs such as M4A/AAC, Apple Lossless (ALAC), WMA, ATRAC (.at9), etc. A full list can be found at [ffmpeg's documentation](https://www.ffmpeg.org/general.html#Audio-Codecs). If the aforementioned features are not required, can be skipped.
 
 Supported audio formats *without* ffmpeg include: WAV, FLAC, Ogg/Vorbis, Ogg/Opus, MP3.
 A full list can be found at [libsndfile's supported formats page](https://libsndfile.github.io/libsndfile/formats.html)
 
 ## Installation
```

### Comparing `pymusiclooper-3.4.0/pymusiclooper/analysis.py` & `pymusiclooper-3.4.1/pymusiclooper/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,14 +244,17 @@
 
         pulse = librosa.beat.plp(onset_envelope=onset_env)
         beats_plp = np.flatnonzero(librosa.util.localmax(pulse))
         bpm, beats = librosa.beat.beat_track(onset_envelope=onset_env)
 
         beats = np.union1d(beats, beats_plp)
         beats = np.sort(beats)
+
+        if isinstance(bpm, np.ndarray):
+            bpm = bpm[0]
     except Exception as e:
         raise LoopNotFoundError(f"Beat analysis failed for \"{mlaudio.filename}\". Cannot continue.") from e
 
     return chroma, power_db, bpm, beats
 
 
 @njit
```

### Comparing `pymusiclooper-3.4.0/pymusiclooper/audio.py` & `pymusiclooper-3.4.1/pymusiclooper/audio.py`

 * *Files identical despite different names*

### Comparing `pymusiclooper-3.4.0/pymusiclooper/cli.py` & `pymusiclooper-3.4.1/pymusiclooper/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 import tempfile
 import warnings
 
 import rich_click as click
 from rich.logging import RichHandler
 from rich.progress import Progress, SpinnerColumn, TimeElapsedColumn
 from rich.traceback import install as rich_traceback_handler
-from rich_click.cli import patch as rich_click_patch
+from rich_click.patch import patch as rich_click_patch
 from yt_dlp.utils import YoutubeDLError
 
 rich_click_patch()
 from click_option_group import RequiredMutuallyExclusiveOptionGroup, optgroup
-from click_params import PUBLIC_URL as UrlParamType
+from click_params import URL as UrlParamType
 
 from pymusiclooper import __version__
 from pymusiclooper.console import _COMMAND_GROUPS, _OPTION_GROUPS, rich_console
 from pymusiclooper.core import MusicLooper
 from pymusiclooper.exceptions import AudioLoadError, LoopNotFoundError
 from pymusiclooper.handler import BatchHandler, LoopExportHandler, LoopHandler
 from pymusiclooper.utils import download_audio, get_outputdir, mk_outputdir
```

### Comparing `pymusiclooper-3.4.0/pymusiclooper/console.py` & `pymusiclooper-3.4.1/pymusiclooper/console.py`

 * *Files identical despite different names*

### Comparing `pymusiclooper-3.4.0/pymusiclooper/core.py` & `pymusiclooper-3.4.1/pymusiclooper/core.py`

 * *Files identical despite different names*

### Comparing `pymusiclooper-3.4.0/pymusiclooper/handler.py` & `pymusiclooper-3.4.1/pymusiclooper/handler.py`

 * *Files identical despite different names*

### Comparing `pymusiclooper-3.4.0/pymusiclooper/playback.py` & `pymusiclooper-3.4.1/pymusiclooper/playback.py`

 * *Files identical despite different names*

### Comparing `pymusiclooper-3.4.0/pymusiclooper/utils.py` & `pymusiclooper-3.4.1/pymusiclooper/utils.py`

 * *Files identical despite different names*

### Comparing `pymusiclooper-3.4.0/pymusiclooper/youtube.py` & `pymusiclooper-3.4.1/pymusiclooper/youtube.py`

 * *Files identical despite different names*

### Comparing `pymusiclooper-3.4.0/PKG-INFO` & `pymusiclooper-3.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymusiclooper
-Version: 3.4.0
+Version: 3.4.1
 Summary: Repeat music endlessly and create seamless music loops, with play/export/tagging support.
 Home-page: https://github.com/arkrow/PyMusicLooper
 License: MIT
 Author: arkrow
 Author-email: arkrow@protonmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,24 +17,22 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Requires-Dist: click-option-group (>=0.5.6,<0.6.0)
-Requires-Dist: click-params (>=0.4.1,<0.5.0)
+Requires-Dist: click-params (>=0.5.0,<0.6.0)
 Requires-Dist: lazy-loader (>=0.3)
-Requires-Dist: librosa (>=0.10.1,<0.11.0)
+Requires-Dist: librosa (==0.10.2)
 Requires-Dist: numba (>=0.59.1)
-Requires-Dist: numpy (>=1.25.0)
-Requires-Dist: pytaglib (>=2.0.0)
+Requires-Dist: numpy (>=1.25.0,<2.0.0)
+Requires-Dist: pytaglib (>=3.0.0,<4.0.0)
 Requires-Dist: rich (>=13.4.2)
-Requires-Dist: rich-click (>=1.6.1,<2.0.0)
-Requires-Dist: scipy (<1.13.0)
-Requires-Dist: setuptools (>=67.0.0)
+Requires-Dist: rich-click (>=1.8.0,<2.0.0)
 Requires-Dist: sounddevice (>=0.4.6)
 Requires-Dist: soundfile (>=0.12.1)
 Requires-Dist: yt-dlp (>=2024.4.9)
 Project-URL: Changelog, https://github.com/arkrow/PyMusicLooper/blob/master/CHANGELOG.md
 Project-URL: Repository, https://github.com/arkrow/PyMusicLooper
 Description-Content-Type: text/markdown
 
@@ -57,15 +55,15 @@
 - Export the loop points as metadata tags to a copy of the input audio file(s), for use with game engines, etc.
 - Export a longer, extended version of an audio track by looping it seamlessly to the desired length
 
 ## Pre-requisites
 
 The following software must be installed for `pymusiclooper` to function correctly.
 
-- [Python (64-bit)](https://www.python.org/downloads/) >= 3.8
+- [Python (64-bit)](https://www.python.org/downloads/) >= 3.9
 - [ffmpeg](https://ffmpeg.org/download.html): required for loading audio from youtube (or any stream supported by [yt-dlp](https://github.com/yt-dlp/yt-dlp)) and adds support for loading additional audio formats and codecs such as M4A/AAC, Apple Lossless (ALAC), WMA, ATRAC (.at9), etc. A full list can be found at [ffmpeg's documentation](https://www.ffmpeg.org/general.html#Audio-Codecs). If the aforementioned features are not required, can be skipped.
 
 Supported audio formats *without* ffmpeg include: WAV, FLAC, Ogg/Vorbis, Ogg/Opus, MP3.
 A full list can be found at [libsndfile's supported formats page](https://libsndfile.github.io/libsndfile/formats.html)
 
 ## Installation
```

