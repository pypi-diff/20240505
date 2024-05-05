# Comparing `tmp/tgctoolbox-0.1.tar.gz` & `tmp/tgctoolbox-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgctoolbox-0.1.tar", max compression
+gzip compressed data, was "tgctoolbox-0.2.tar", max compression
```

## Comparing `tgctoolbox-0.1.tar` & `tgctoolbox-0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0      522 2024-03-29 00:08:43.778355 tgctoolbox-0.1/pyproject.toml
--rw-r--r--   0        0        0     1465 2024-03-29 00:29:09.875305 tgctoolbox-0.1/tgctoolbox/__init__.py
--rw-r--r--   0        0        0     2789 2024-03-28 23:18:41.616539 tgctoolbox-0.1/tgctoolbox/downloaders.py
--rw-r--r--   0        0        0     5752 2024-03-28 23:18:48.328423 tgctoolbox-0.1/tgctoolbox/ffmpeg.py
--rw-r--r--   0        0        0     3472 2024-03-23 12:35:46.397899 tgctoolbox-0.1/tgctoolbox/logger.py
--rw-r--r--   0        0        0      131 2024-03-25 13:14:03.792489 tgctoolbox-0.1/tgctoolbox/meta.py
--rw-r--r--   0        0        0     3687 2024-03-28 23:18:57.689779 tgctoolbox-0.1/tgctoolbox/operations.py
--rw-r--r--   0        0        0     2658 2024-03-29 00:28:22.705823 tgctoolbox-0.1/tgctoolbox/recorder.py
--rw-r--r--   0        0        0     3472 2024-03-25 13:28:29.971846 tgctoolbox-0.1/tgctoolbox/sound.py
--rw-r--r--   0        0        0     2494 2024-03-28 23:19:16.970214 tgctoolbox-0.1/tgctoolbox/timing.py
--rw-r--r--   0        0        0     1814 2024-03-28 23:19:24.167992 tgctoolbox-0.1/tgctoolbox/vosk.py
--rw-r--r--   0        0        0     3381 2024-03-28 23:19:28.174695 tgctoolbox-0.1/tgctoolbox/wait_run.py
--rw-r--r--   0        0        0     1726 2024-03-28 23:19:31.648944 tgctoolbox-0.1/tgctoolbox/wrapper.py
--rw-r--r--   0        0        0      545 1970-01-01 00:00:00.000000 tgctoolbox-0.1/PKG-INFO
+-rw-r--r--   0        0        0      541 2024-05-05 11:52:14.312645 tgctoolbox-0.2/pyproject.toml
+-rw-r--r--   0        0        0     1883 2024-05-05 11:34:10.191732 tgctoolbox-0.2/tgctoolbox/__init__.py
+-rw-r--r--   0        0        0     2965 2024-04-14 10:00:56.065124 tgctoolbox-0.2/tgctoolbox/downloaders.py
+-rw-r--r--   0        0        0     6398 2024-04-14 10:04:12.366063 tgctoolbox-0.2/tgctoolbox/ffmpeg.py
+-rw-r--r--   0        0        0     3699 2024-04-04 14:07:33.674769 tgctoolbox-0.2/tgctoolbox/logger.py
+-rw-r--r--   0        0        0      125 2024-04-04 14:07:33.502903 tgctoolbox-0.2/tgctoolbox/meta.py
+-rw-r--r--   0        0        0     3532 2024-04-14 10:04:35.139755 tgctoolbox-0.2/tgctoolbox/operations.py
+-rw-r--r--   0        0        0     2536 2024-04-14 10:05:13.288749 tgctoolbox-0.2/tgctoolbox/recorder.py
+-rw-r--r--   0        0        0     7717 2024-05-05 11:42:16.815394 tgctoolbox-0.2/tgctoolbox/settings.py
+-rw-r--r--   0        0        0     4338 2024-05-04 17:49:00.284883 tgctoolbox-0.2/tgctoolbox/sound.py
+-rw-r--r--   0        0        0     2541 2024-04-14 10:05:55.801603 tgctoolbox-0.2/tgctoolbox/timing.py
+-rw-r--r--   0        0        0     1787 2024-04-14 10:06:14.232604 tgctoolbox-0.2/tgctoolbox/vosk.py
+-rw-r--r--   0        0        0     3415 2024-04-14 10:06:32.142449 tgctoolbox-0.2/tgctoolbox/wait_run.py
+-rw-r--r--   0        0        0     2740 2024-04-13 22:34:12.249076 tgctoolbox-0.2/tgctoolbox/wrapper.py
+-rw-r--r--   0        0        0      584 1970-01-01 00:00:00.000000 tgctoolbox-0.2/PKG-INFO
```

### Comparing `tgctoolbox-0.1/pyproject.toml` & `tgctoolbox-0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "tgctoolbox"
-version = "0.1"
+version = "0.2"
 description = "Comprehensive toolbox with all of the utils and tools used in various TGC projects."
 authors = ["Jakub Muszyński <jakub.m.muszynski@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.12"
 pytube = "*"
 moviepy = "*"
 tqdm = "*"
 requests = "*"
 vosk = "*"
 websocket = "*"
 starlette = "*"
 colorama = "*"
+pyyaml = "^6.0.1"
 
 [tool.poetry.extras]
 audio = ["pyaudio"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `tgctoolbox-0.1/tgctoolbox/downloaders.py` & `tgctoolbox-0.2/tgctoolbox/downloaders.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,77 +1,89 @@
-import os
-import requests
-from pathlib import Path
-from zipfile import ZipFile
-from io import BytesIO
-from tgctoolbox import TGCLoggerSetup
-from pytube import YouTube
-from moviepy.editor import AudioFileClip
-from tqdm import tqdm
-
-logger = TGCLoggerSetup(__name__)
-
-def download_vosk_model(model_name, destination_folder):
-    model_url = f"https://alphacephei.com/vosk/models/vosk-model-{model_name}.zip"
-
-    try:
-        # Creating destination folder if it doesn't exist
-        Path(destination_folder).mkdir(parents=True, exist_ok=True)
-
-        logger.info(f"Downloading model '{model_name}' from {model_url}")
-
-        # Downloading the model
-        response = requests.get(model_url)
-        response.raise_for_status()  # Raise an HTTPError if the HTTP request returned an unsuccessful status code
-
-        # Unzipping the model
-        with ZipFile(BytesIO(response.content)) as model_zip:
-            model_zip.extractall(destination_folder)
-        
-        logger.info(f"Model '{model_name}' downloaded and extracted to {destination_folder}")
-    
-    except requests.HTTPError as http_err:
-        logger.error(f"HTTP error occurred: {http_err}", exc_info=True)
-    except Exception as err:
-        print(f"An error occurred: {err}", exc_info=True)
-
-
-def download_file(url, filename):
-    """
-    Download a file from a URL and display a progress bar.
-
-    Args:
-        url (str): The URL of the file to download.
-        filename (str): The name to save the file as.
-    """
-    response = requests.get(url, stream=True)
-
-    if response.status_code == 200:
-        total_size_in_bytes= int(response.headers.get('content-length', 0))
-        progress_bar = tqdm(total=total_size_in_bytes, unit='iB', unit_scale=True)
-
-        with open(filename, 'wb') as file:
-            for chunk in response.iter_content(chunk_size=1024):
-                progress_bar.update(len(chunk))
-                if chunk:
-                    file.write(chunk)
-
-        progress_bar.close()
-
-        if total_size_in_bytes != 0 and progress_bar.n != total_size_in_bytes:
-            print("ERROR, something went wrong")
-    else:
-        print(f"Failed to download file. HTTP response code: {response.status_code}")
-        
-
-def download_video_as_wav(youtube_link, output_filename):
-    # Step 1: Download YouTube video
-    yt = YouTube(youtube_link)
-    video = yt.streams.filter(only_audio=True).first()
-    download_path = video.download()
-    
-    # Step 2: Convert the downloaded file to WAV
-    video_clip = AudioFileClip(download_path)
-    video_clip.write_audiofile(f"{output_filename}.wav")
-    
-    # Optional: Remove the original download (if you want to keep only the WAV file)
-    os.remove(download_path)
+import os
+from io import BytesIO
+from pathlib import Path
+from zipfile import ZipFile
+
+import requests
+from moviepy.editor import AudioFileClip
+from pytube import YouTube
+from tqdm import tqdm
+
+from .logger import setup_custom_logger as TGCLoggerSetup
+
+logger = TGCLoggerSetup(__name__)
+
+
+def download_vosk_model(model_name, destination_folder) -> bool:
+    model_url = f"https://alphacephei.com/vosk/models/vosk-model-{model_name}.zip"
+
+    try:
+        # Creating destination folder if it doesn't exist
+        Path(destination_folder).mkdir(parents=True, exist_ok=True)
+
+        logger.info(f"Downloading model '{model_name}' from {model_url}")
+
+        # Downloading the model
+        response = requests.get(model_url)
+        if response.status_code == 404:  # Model not found
+            logger.error(
+                f"Model '{model_name}' not found. Please check the model name and try again."
+            )
+            return False
+        elif response.status_code != 200:  # Other HTTP error
+            response.raise_for_status()
+
+        # Unzipping the model
+        with ZipFile(BytesIO(response.content)) as model_zip:
+            model_zip.extractall(destination_folder)
+
+        logger.info(
+            f"Model '{model_name}' downloaded and extracted to {destination_folder}"
+        )
+        return True
+
+    except requests.HTTPError as http_err:
+        logger.error(f"HTTP error occurred: {http_err}", exc_info=True)
+    except Exception as err:
+        print(f"An error occurred: {err}", exc_info=True)
+
+
+def download_file(url, filename):
+    """
+    Download a file from a URL and display a progress bar.
+
+    Args:
+        url (str): The URL of the file to download.
+        filename (str): The name to save the file as.
+    """
+    response = requests.get(url, stream=True)
+
+    if response.status_code == 200:
+        total_size_in_bytes = int(response.headers.get("content-length", 0))
+        progress_bar = tqdm(total=total_size_in_bytes, unit="iB", unit_scale=True)
+
+        with open(filename, "wb") as file:
+            for chunk in response.iter_content(chunk_size=1024):
+                progress_bar.update(len(chunk))
+                if chunk:
+                    file.write(chunk)
+
+        progress_bar.close()
+
+        if total_size_in_bytes != 0 and progress_bar.n != total_size_in_bytes:
+            print("ERROR, something went wrong")
+    else:
+        print(f"Failed to download file. HTTP response code: {response.status_code}")
+
+
+def download_video_as_wav(youtube_link, output_filename):
+    # Step 1: Download YouTube video
+    yt = YouTube(youtube_link)
+    video = yt.streams.filter(only_audio=True).first()
+    download_path = video.download()
+
+    # Step 2: Convert the downloaded file to WAV
+    video_clip = AudioFileClip(download_path)
+    video_clip.write_audiofile(f"{output_filename}.wav")
+
+    # Optional: Remove the original download (if you want to keep only the WAV file)
+    os.remove(download_path)
```

### Comparing `tgctoolbox-0.1/tgctoolbox/ffmpeg.py` & `tgctoolbox-0.2/tgctoolbox/ffmpeg.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,127 +1,179 @@
 import subprocess
 import sys
-from tgctoolbox import TGCLoggerSetup
+
+from .logger import setup_custom_logger as TGCLoggerSetup
 
 logger = TGCLoggerSetup(__name__)
 
+
 def is_admin():
     """_summary_: Checks if the current user is an administrator on Windows.
 
     Returns:
         bool: True if the current user is an administrator, False otherwise.
     """
     try:
-        return subprocess.check_call(['net', 'session'], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL) == 0
+        return (
+            subprocess.check_call(
+                ["net", "session"], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL
+            )
+            == 0
+        )
     except:
         return False
 
+
 def run_as_admin():
     """_summary_: Restarts the current script with administrator privileges on Windows.
-    
+
     Raises:
         PermissionError: If the current user is not an administrator.
     """
     logger.info("Requesting administrator privileges...")
-    subprocess.call(['powershell', 'Start-Process', 'python', f"'{sys.argv[0]}'", '-Verb', 'RunAs'])
+    subprocess.call(
+        ["powershell", "Start-Process", "python", f"'{sys.argv[0]}'", "-Verb", "RunAs"]
+    )
     sys.exit()
 
+
 def is_choco_installed():
     """_summary_: Checks if Chocolatey is installed on Windows. Output of the command called to do so is supressed.
 
     Returns:
         bool: True if Chocolatey is installed, False otherwise.
     """
     try:
-        return subprocess.run("choco -v", shell=True, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL).returncode == 0
+        return (
+            subprocess.run(
+                "choco -v",
+                shell=True,
+                stdout=subprocess.DEVNULL,
+                stderr=subprocess.DEVNULL,
+            ).returncode
+            == 0
+        )
     except FileNotFoundError:
         return False
 
+
 def is_ffmpeg_installed():
     """_summary_: Checks if FFmpeg is installed on Windows. Output of the command called to do so is supressed.
 
     Returns:
         bool: True if FFmpeg is installed, False otherwise.
     """
     try:
-        return subprocess.run(["ffmpeg", "-version"], stdout=subprocess.DEVNULL, check=False).returncode == 0
+        return (
+            subprocess.run(
+                ["ffmpeg", "-version"], stdout=subprocess.DEVNULL, check=False
+            ).returncode
+            == 0
+        )
     except FileNotFoundError:
         return False
 
+
 def install_ffmpeg_windows(supress_output=False):
     """_summary_: Installs Chocolatey and FFmpeg on Windows. If the current user is not an administrator, the script will be restarted with administrator privileges.
 
     NOTE: This function is only intended to be called on Windows. Also, supress output only supresses stdout not stderr, for ease of debugging.
-    
+
     Args:
         supress_output (bool, optional): Whether to supress the output of the commands called during installation. Defaults to False.
     """
     stdout = subprocess.DEVNULL if supress_output else None
-    
+
     if not is_choco_installed() or not is_ffmpeg_installed():
         if not is_admin():
             run_as_admin()
 
         if not is_choco_installed():
             logger.info("Installing Chocolatey...")
-            ps_command = 'Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString(\'https://chocolatey.org/install.ps1\'))'
-            subprocess.run(["powershell", "-Command", ps_command], check=True, stdout=stdout)
+            ps_command = "Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))"
+            subprocess.run(
+                ["powershell", "-Command", ps_command], check=True, stdout=stdout
+            )
 
         if not is_ffmpeg_installed():
             logger.info("Installing FFmpeg...")
-            subprocess.run(['choco', 'install', 'ffmpeg'], check=True, stdout=stdout)
-            
+            subprocess.run(["choco", "install", "ffmpeg"], check=True, stdout=stdout)
+
     else:
         logger.info("Chocolatey and FFmpeg are already installed.")
 
+
 def install_ffmpeg_linux(supress_output=False):
     """_summary_: Installs Chocolatey and FFmpeg on Linux. Only tested on Unix containers, not live distro.
 
     NOTE: This function is only intended to be called on Linux. Also, supress output supresses both stdout and stderr.
-    
+
     Args:
         supress_output (bool, optional): Whether to supress the output of the commands called during installation. Defaults to False.
     """
     try:
         stdout = subprocess.DEVNULL if supress_output else None
 
         # Check if FFmpeg is installed
         try:
-            ffmpeg_check = subprocess.run(["ffmpeg", "-version"], stdout=stdout, stderr=stdout, check=False)
+            ffmpeg_check = subprocess.run(
+                ["ffmpeg", "-version"], stdout=stdout, stderr=stdout, check=False
+            )
             if ffmpeg_check.returncode != 0:
                 raise FileNotFoundError("FFmpeg not found")
         except FileNotFoundError:
             logger.info("FFmpeg is not installed, installing now...")
-            subprocess.run(['sudo', 'apt', 'update'], check=True, stdout=stdout, stderr=stdout)
-            subprocess.run(['sudo', 'apt', 'install', '-y', 'ffmpeg'], check=True, stdout=stdout, stderr=stdout)
+            subprocess.run(
+                ["sudo", "apt", "update"], check=True, stdout=stdout, stderr=stdout
+            )
+            subprocess.run(
+                ["sudo", "apt", "install", "-y", "ffmpeg"],
+                check=True,
+                stdout=stdout,
+                stderr=stdout,
+            )
         else:
             logger.info("FFmpeg is already installed.")
     except subprocess.CalledProcessError as e:
-        logger.error(f"Failed to install FFmpeg on Linux. Error: {str(e)}", exc_info=True)
+        logger.error(
+            f"Failed to install FFmpeg on Linux. Error: {str(e)}", exc_info=True
+        )
         sys.exit(1)
 
 
 def install_ffmpeg_macos(supress_output=False):
     """_summary_: Installs Chocolatey and FFmpeg on MacOS. This have not been tested.
-    
+
     WARNING: This function have not been tested. It should theoretically work, but be warned that it might not.s
 
     Args:
         supress_output (bool, optional): _description_. Defaults to False.
     """
     try:
         stdout = subprocess.DEVNULL if supress_output else None
-        
+
         # Check if Homebrew is installed
-        if subprocess.run("brew -v", shell=True, stdout=stdout, check=False).returncode != 0:
+        if (
+            subprocess.run("brew -v", shell=True, stdout=stdout, check=False).returncode
+            != 0
+        ):
             logger.info("Installing Homebrew...")
-            subprocess.run('/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"', check=True, shell=True)
-        
+            subprocess.run(
+                '/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"',
+                check=True,
+                shell=True,
+            )
+
         # Check if FFmpeg is installed
-        if subprocess.run("ffmpeg -version", shell=True, stdout=stdout, check=False).returncode != 0:
+        if (
+            subprocess.run(
+                "ffmpeg -version", shell=True, stdout=stdout, check=False
+            ).returncode
+            != 0
+        ):
             logger.info("Installing FFmpeg...")
-            subprocess.run(['brew', 'install', 'ffmpeg'], check=True)
+            subprocess.run(["brew", "install", "ffmpeg"], check=True)
         else:
             logger.info("FFmpeg is already installed.")
     except subprocess.CalledProcessError:
         logger.error("Failed to install FFmpeg on macOS.", exc_info=True)
         sys.exit(1)
```

### Comparing `tgctoolbox-0.1/tgctoolbox/logger.py` & `tgctoolbox-0.2/tgctoolbox/logger.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,94 +1,121 @@
-import logging
-import inspect
-from typing import Type
-
-class JacobsAmazingLoggerFormatter(logging.Formatter):
-    """Logging Formatter to add colors to the levelname and include function name"""
-
-    grey = "\x1b[38;21m"
-    blue = "\x1b[34m"
-    light_blue = "\x1b[94m"
-    green = "\x1b[32m"
-    yellow = "\x1b[33m"
-    red = "\x1b[31m"
-    reset = "\x1b[0m"
-
-    LEVEL_COLORS = {
-        logging.DEBUG: blue,
-        logging.INFO: green,
-        logging.WARNING: yellow,
-        logging.ERROR: red,
-        logging.CRITICAL: red
-    }
-
-    def format(self, record):
-        # Dynamically find the name of the calling function
-        stack = inspect.stack()
-        func_name = "unknown"
-        for frame in stack:
-            if frame.function not in ["emit", "format"] and 'logging' not in frame.filename:
-                func_name = frame.function
-                break
-        record.func_name = func_name
-
-        # Colorize levelname
-        color = self.LEVEL_COLORS.get(record.levelno, self.grey)
-        record.levelname = color + record.levelname + self.reset
-        
-        if hasattr(record, 'timespec'):
-            record.msg = self.light_blue + "TIMESPEC: " + self.reset + record.msg
-            return super(JacobsAmazingLoggerFormatter, self).format(record)
-        
-        if hasattr(record, 'result'):
-            record.msg = self.light_blue + "RESULT: " + self.reset + record.msg
-            return super(JacobsAmazingLoggerFormatter, self).format(record)
-
-        # Set the format and return the formatted record
-        self._style._fmt = "%(levelname)s: [%(func_name)s] %(asctime)s - %(message)s"
-        return super(JacobsAmazingLoggerFormatter, self).format(record)
-    
-    
-class JacobsAmazingLogger(logging.Logger):
-    def timespec(self, message, *args, **kwargs):
-        # Add a custom attribute to the log record
-        if self.isEnabledFor(logging.INFO):
-            # Create a new record with a custom attribute
-            record = self.makeRecord(self.name, logging.INFO, "(unknown file)", 0, message, args, kwargs, None)
-            record.timespec = True
-            self.handle(record)
-            
-class JacobsAmazingResultsLogger(logging.Logger):
-    def result(self, message, *args, **kwargs):
-        # Add a custom attribute to the log record
-        if self.isEnabledFor(logging.INFO):
-            # Create a new record with a custom attribute
-            record = self.makeRecord(self.name, logging.INFO, "(unknown file)", 0, message, args, kwargs, None)
-            record.result = True
-            self.handle(record)
-
-
-def setup_custom_logger(name: str, level: str = 'INFO', logger = None) -> Type[logging.Logger]:
-    """
-    Set up and return a custom logger with the specified name and level.
-
-    :param name: Name of the logger.
-    :param level: Logging level, e.g., 'INFO', 'DEBUG'.
-    :return: Configured logger instance.
-    """
-    if logger is not None:
-        logger = logger
-    else:
-        logger = logging.getLogger(name)
-    logger.setLevel(level.upper())
-
-    # Create and set handler and formatter
-    handler = logging.StreamHandler()
-    handler.setFormatter(JacobsAmazingLoggerFormatter())
-    logger.addHandler(handler)
-
-    return logger
-
-
-def log_result(message):
-    logger = setup_custom_logger(__name__, level='INFO', logger=JacobsAmazingResultsLogger(__name__))
-    logger.result(message)
+import inspect
+import logging
+from typing import Type
+
+
+class JacobsAmazingLoggerFormatter(logging.Formatter):
+    """Logging Formatter to add colors to the levelname and include function name"""
+
+    grey = "\x1b[38;21m"
+    blue = "\x1b[34m"
+    light_blue = "\x1b[94m"
+    green = "\x1b[32m"
+    yellow = "\x1b[33m"
+    red = "\x1b[31m"
+    reset = "\x1b[0m"
+
+    LEVEL_COLORS = {
+        logging.DEBUG: blue,
+        logging.INFO: green,
+        logging.WARNING: yellow,
+        logging.ERROR: red,
+        logging.CRITICAL: red,
+    }
+
+    def format(self, record):
+        # Dynamically find the name of the calling function
+        stack = inspect.stack()
+        func_name = "unknown"
+        for frame in stack:
+            if (
+                frame.function not in ["emit", "format"]
+                and "logging" not in frame.filename
+            ):
+                func_name = frame.function
+                break
+        record.func_name = func_name
+
+        # Colorize levelname
+        color = self.LEVEL_COLORS.get(record.levelno, self.grey)
+        record.levelname = color + record.levelname + self.reset
+
+        if hasattr(record, "timespec"):
+            record.msg = self.light_blue + "TIMESPEC: " + self.reset + record.msg
+            return super(JacobsAmazingLoggerFormatter, self).format(record)
+
+        if hasattr(record, "result"):
+            record.msg = self.light_blue + "RESULT: " + self.reset + record.msg
+            return super(JacobsAmazingLoggerFormatter, self).format(record)
+
+        # Set the format and return the formatted record
+        self._style._fmt = "%(levelname)s: [%(func_name)s] %(asctime)s - %(message)s"
+        return super(JacobsAmazingLoggerFormatter, self).format(record)
+
+
+class JacobsAmazingLogger(logging.Logger):
+    def timespec(self, message, *args, **kwargs):
+        # Add a custom attribute to the log record
+        if self.isEnabledFor(logging.INFO):
+            # Create a new record with a custom attribute
+            record = self.makeRecord(
+                self.name,
+                logging.INFO,
+                "(unknown file)",
+                0,
+                message,
+                args,
+                kwargs,
+                None,
+            )
+            record.timespec = True
+            self.handle(record)
+
+
+class JacobsAmazingResultsLogger(logging.Logger):
+    def result(self, message, *args, **kwargs):
+        # Add a custom attribute to the log record
+        if self.isEnabledFor(logging.INFO):
+            # Create a new record with a custom attribute
+            record = self.makeRecord(
+                self.name,
+                logging.INFO,
+                "(unknown file)",
+                0,
+                message,
+                args,
+                kwargs,
+                None,
+            )
+            record.result = True
+            self.handle(record)
+
+
+def setup_custom_logger(
+    name: str, level: str = "INFO", logger=None
+) -> Type[logging.Logger]:
+    """
+    Set up and return a custom logger with the specified name and level.
+
+    :param name: Name of the logger.
+    :param level: Logging level, e.g., 'INFO', 'DEBUG'.
+    :return: Configured logger instance.
+    """
+    if logger is not None:
+        logger = logger
+    else:
+        logger = logging.getLogger(name)
+    logger.setLevel(level.upper())
+
+    # Create and set handler and formatter
+    handler = logging.StreamHandler()
+    handler.setFormatter(JacobsAmazingLoggerFormatter())
+    logger.addHandler(handler)
+
+    return logger
+
+
+def log_result(message):
+    logger = setup_custom_logger(
+        __name__, level="INFO", logger=JacobsAmazingResultsLogger(__name__)
+    )
+    logger.result(message)
```

### Comparing `tgctoolbox-0.1/tgctoolbox/operations.py` & `tgctoolbox-0.2/tgctoolbox/operations.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,102 +1,107 @@
-from ast import Dict
-import os
-import glob
-import logging
-from typing import Dict
-import tempfile
-from tgctoolbox import TGCLoggerSetup
-
-logger = TGCLoggerSetup(__name__)
-
-def dir_size_adjust(dir_path: str, 
-                    num_files : int = 10, 
-                    size_limit : int = 100000000, 
-                    logger: logging.Logger = logger):
-    
-    """_summary_: Adjusts the number of files in the directory to 10 by deleting the oldest files.
-
-    Args:
-        file_path (str): Path to the directory.
-        num_files (int, optional): Number of files to keep. Defaults to 10.
-        size_limit (int, optional): Maximum size of the directory in bytes. Defaults to 100000000.
-    """
-    files = glob.glob(os.path.join(dir_path, "*"))
-    try:
-        if len(files) > num_files:
-            files.sort(key=os.path.getmtime)
-            for i in range(len(files) - 10):
-                os.remove(files[i])
-            files = glob.glob(os.path.join(dir_path, "*"))
-            files.sort(key=os.path.getmtime, reverse=True)
-            return True
-        if sum(os.path.getsize(f) for f in files) > size_limit:
-            files.sort(key=os.path.getmtime)
-            while sum(os.path.getsize(f) for f in files) > size_limit:
-                os.remove(files[0])
-                logger.info(f"Removed file {files[0]}")
-                files = glob.glob(os.path.join(dir_path, "*"))
-            files.sort(key=os.path.getmtime, reverse=True)
-            return True
-        else:
-            files.sort(key=os.path.getmtime, reverse=True)
-            return True
-    except FileNotFoundError:
-        logger.error(f"Directory not found: {dir_path}", exc_info=True)
-    except PermissionError:
-        logger.error(f"Permission denied for directory: {dir_path}", exc_info=True)
-    except Exception as e:
-        logger.error("An unexpected error occurred in dir_size_adjust", exc_info=True)
-    return False
-
-def dict_size_adjust(dict : Dict, 
-                     num_items : int = 10, 
-                     logger: logging.Logger = logger):
-    
-    """_summary_: Adjusts the number of items in the dictionary to 10 by deleting the oldest items.
-
-    Args:
-        dict (dict): Dictionary to be adjusted.
-        num_items (int, optional): Number of items to keep. Defaults to 10.
-    """
-    try:
-        keys = list(dict.keys())
-        keys.sort(key=lambda x: dict[x]['timestamp'])
-        if len(dict) > num_items:
-            for i in range(len(dict) - num_items):
-                logger.info(f"Removed task {keys[i]}")
-                del dict[keys[i]]
-            return True
-        else:
-            return True
-    except Exception as e:
-        logger.error(f"An unexpected error occurred in dict_size_adjust: {e}", exc_info=True)
-        return False
-
-def save_temp_file(audio_data: bytes, file_extension: str = 'wav') -> str:
-    """
-    Save the audio data to a temporary file and return the file path.
-
-    Args:
-    audio_data (bytes): The audio data to save.
-    file_extension (str): The file extension for the audio file (default 'wav').
-
-    Returns:
-    str: The path to the temporary audio file.
-    """
-    temp_file, temp_file_path = tempfile.mkstemp(suffix=f'.{file_extension}')
-    with os.fdopen(temp_file, 'wb') as file:
-        file.write(audio_data)
-
-    return temp_file_path
-
-def get_file_extension(file_path: str) -> str:
-    """
-    Get the file extension of a file.
-
-    Args:
-    file_path (str): The path to the file.
-
-    Returns:
-    str: The file extension.
-    """
-    return os.path.splitext(file_path)[1][1:].strip().lower()
+import glob
+import logging
+import os
+import tempfile
+from ast import Dict
+from typing import Dict
+
+from .logger import setup_custom_logger as TGCLoggerSetup
+
+logger = TGCLoggerSetup(__name__)
+
+
+def dir_size_adjust(
+    dir_path: str,
+    num_files: int = 10,
+    size_limit: int = 100000000,
+    logger: logging.Logger = logger,
+):
+    """_summary_: Adjusts the number of files in the directory to 10 by deleting the oldest files.
+
+    Args:
+        file_path (str): Path to the directory.
+        num_files (int, optional): Number of files to keep. Defaults to 10.
+        size_limit (int, optional): Maximum size of the directory in bytes. Defaults to 100000000.
+    """
+    files = glob.glob(os.path.join(dir_path, "*"))
+    try:
+        if len(files) > num_files:
+            files.sort(key=os.path.getmtime)
+            for i in range(len(files) - 10):
+                os.remove(files[i])
+            files = glob.glob(os.path.join(dir_path, "*"))
+            files.sort(key=os.path.getmtime, reverse=True)
+            return True
+        if sum(os.path.getsize(f) for f in files) > size_limit:
+            files.sort(key=os.path.getmtime)
+            while sum(os.path.getsize(f) for f in files) > size_limit:
+                os.remove(files[0])
+                logger.info(f"Removed file {files[0]}")
+                files = glob.glob(os.path.join(dir_path, "*"))
+            files.sort(key=os.path.getmtime, reverse=True)
+            return True
+        else:
+            files.sort(key=os.path.getmtime, reverse=True)
+            return True
+    except FileNotFoundError:
+        logger.error(f"Directory not found: {dir_path}", exc_info=True)
+    except PermissionError:
+        logger.error(f"Permission denied for directory: {dir_path}", exc_info=True)
+    except Exception as e:
+        logger.error("An unexpected error occurred in dir_size_adjust", exc_info=True)
+    return False
+
+
+def dict_size_adjust(dict: Dict, num_items: int = 10, logger: logging.Logger = logger):
+    """_summary_: Adjusts the number of items in the dictionary to 10 by deleting the oldest items.
+
+    Args:
+        dict (dict): Dictionary to be adjusted.
+        num_items (int, optional): Number of items to keep. Defaults to 10.
+    """
+    try:
+        keys = list(dict.keys())
+        keys.sort(key=lambda x: dict[x]["timestamp"])
+        if len(dict) > num_items:
+            for i in range(len(dict) - num_items):
+                logger.info(f"Removed task {keys[i]}")
+                del dict[keys[i]]
+            return True
+        else:
+            return True
+    except Exception as e:
+        logger.error(
+            f"An unexpected error occurred in dict_size_adjust: {e}", exc_info=True
+        )
+        return False
+
+
+def save_temp_file(audio_data: bytes, file_extension: str = "wav") -> str:
+    """
+    Save the audio data to a temporary file and return the file path.
+
+    Args:
+    audio_data (bytes): The audio data to save.
+    file_extension (str): The file extension for the audio file (default 'wav').
+
+    Returns:
+    str: The path to the temporary audio file.
+    """
+    temp_file, temp_file_path = tempfile.mkstemp(suffix=f".{file_extension}")
+    with os.fdopen(temp_file, "wb") as file:
+        file.write(audio_data)
+
+    return temp_file_path
+
+
+def get_file_extension(file_path: str) -> str:
+    """
+    Get the file extension of a file.
+
+    Args:
+    file_path (str): The path to the file.
+
+    Returns:
+    str: The file extension.
+    """
+    return os.path.splitext(file_path)[1][1:].strip().lower()
```

### Comparing `tgctoolbox-0.1/tgctoolbox/recorder.py` & `tgctoolbox-0.2/tgctoolbox/recorder.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 try:
     import pyaudio
+
     PyAudio = pyaudio.PyAudio
 except ImportError:
     PyAudio = None
 import websocket
 import threading
 import time
-from tgctoolbox import TGCLoggerSetup
+from .logger import setup_custom_logger as TGCLoggerSetup
 
 if PyAudio is None:
-        raise ImportError("The 'audio' extras are required to use this feature. "
-                          "Install them with: pip install tgctoolbox[audio]")
+    raise ImportError(
+        "The 'audio' extras are required to use this feature. "
+        "Install them with: pip install tgctoolbox[audio]"
+    )
 
 # Constants for audio recording
 FORMAT = pyaudio.paInt16  # Audio format
-CHANNELS = 1              # Mono audio
-RATE = 16000              # Sampling rate
-CHUNK = 1024              # Frames per buffer
+CHANNELS = 1  # Mono audio
+RATE = 16000  # Sampling rate
+CHUNK = 1024  # Frames per buffer
 
 # WebSocket URL
 ws_url = "ws://localhost:8000/ws/transcribe_aai"
 
 # Initialize PyAudio
 audio = pyaudio.PyAudio()
 
 logger = TGCLoggerSetup("recorder")
 
+
 # WebSocket client
 class WSClient(threading.Thread):
     def __init__(self, url):
         threading.Thread.__init__(self)
-        self.ws = websocket.WebSocketApp(url,
-                                         on_message=self.on_message,
-                                         on_error=self.on_error,
-                                         on_close=self.on_close)
+        self.ws = websocket.WebSocketApp(
+            url,
+            on_message=self.on_message,
+            on_error=self.on_error,
+            on_close=self.on_close,
+        )
         self.ws.on_open = self.on_open
         logger.info(f"WebSocket client initialized: {self.ws.__dict__}")
 
     def run(self):
         self.ws.run_forever()
 
     def send_audio(self, data):
@@ -55,32 +61,34 @@
     def on_close(self, ws, close_status_code, close_reason):
         logger.info("### closed ###")
 
     def on_open(self, ws):
         logger.info("WebSocket opened")
         logger.info("WebSocket opened")
 
+
 def record_audio(ws_client):
-    stream = audio.open(format=FORMAT, channels=CHANNELS,
-                        rate=RATE, input=True,
-                        frames_per_buffer=CHUNK)
+    stream = audio.open(
+        format=FORMAT, channels=CHANNELS, rate=RATE, input=True, frames_per_buffer=CHUNK
+    )
 
     logger.info("Recording...")
 
     try:
         while True:
             data = stream.read(CHUNK)
             ws_client.send_audio(data)
-            
+
     except KeyboardInterrupt:
         logger.warning("Recording stopped by user request. Exiting...")
         stream.stop_stream()
         stream.close()
         audio.terminate()
         ws_client.ws.close()
 
+
 if __name__ == "__main__":
     ws_client = WSClient(ws_url)
     ws_client.start()
 
     time.sleep(1)  # Wait for the WebSocket connection to establish
     record_audio(ws_client)
```

### Comparing `tgctoolbox-0.1/tgctoolbox/timing.py` & `tgctoolbox-0.2/tgctoolbox/timing.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,72 @@
-from starlette.middleware.base import BaseHTTPMiddleware
-import time
-from tgctoolbox import TGCLogger, TGCLoggerSetup
-
-class TimingMiddleware(BaseHTTPMiddleware):
-    """
-    Middleware for measuring and logging the time taken for each request.
-
-    This middleware calculates the duration of each HTTP request and logs it
-    using a custom logger. It's useful for monitoring and performance analysis.
-
-    Attributes:
-        logger (TGCLogger): A logger instance to log timing information.
-
-    Args:
-        app: The Starlette/FastAPI application instance to which this middleware is applied.
-    """
-
-    def __init__(self, app):
-        """
-        Initialize the middleware with the application instance.
-
-        Args:
-            app: The application instance to which this middleware is attached.
-        """
-        super().__init__(app)
-        self.logger = TGCLoggerSetup(__name__, level='DEBUG', logger=TGCLogger(__name__))
-
-    async def dispatch(self, request, call_next):
-        """
-        Process each request, measure its processing time, and log the duration.
-
-        This method is an asynchronous coroutine. It records the start time of a request,
-        awaits its completion, and then logs the time taken to process the request.
-
-        Args:
-            request: The incoming HTTP request.
-            call_next: A callable that proceeds to the next middleware or actual request handler.
-
-        Returns:
-            Response: The HTTP response generated by handling the request.
-        """
-        start_time = time.time()
-        response = await call_next(request)
-        process_time = time.time() - start_time
-        self.logger.timespec(f"Request to {request.url.path} took {process_time:.2f} seconds")
-        return response
-
-
-def log_time(start_time, end_time, message=None):
-    """
-    Log the time duration between two time points with an optional message.
-
-    This function calculates the duration between `start_time` and `end_time`
-    and logs it with an optional message for context.
-
-    Args:
-        start_time (float): The start time in seconds.
-        end_time (float): The end time in seconds.
-        message (str, optional): An optional message to include in the log. Defaults to None.
-    """
-    duration = end_time - start_time
-    logger = TGCLoggerSetup(__name__, level='DEBUG', logger=TGCLogger(__name__))
-    logger.timespec(f"{message}: {duration:.2f} seconds")
+import time
+
+from starlette.middleware.base import BaseHTTPMiddleware
+
+from .logger import JacobsAmazingLogger as TGCLogger
+from .logger import setup_custom_logger as TGCLoggerSetup
+
+
+class TimingMiddleware(BaseHTTPMiddleware):
+    """
+    Middleware for measuring and logging the time taken for each request.
+
+    This middleware calculates the duration of each HTTP request and logs it
+    using a custom logger. It's useful for monitoring and performance analysis.
+
+    Attributes:
+        logger (TGCLogger): A logger instance to log timing information.
+
+    Args:
+        app: The Starlette/FastAPI application instance to which this middleware is applied.
+    """
+
+    def __init__(self, app):
+        """
+        Initialize the middleware with the application instance.
+
+        Args:
+            app: The application instance to which this middleware is attached.
+        """
+        super().__init__(app)
+        self.logger = TGCLoggerSetup(
+            __name__, level="DEBUG", logger=TGCLogger(__name__)
+        )
+
+    async def dispatch(self, request, call_next):
+        """
+        Process each request, measure its processing time, and log the duration.
+
+        This method is an asynchronous coroutine. It records the start time of a request,
+        awaits its completion, and then logs the time taken to process the request.
+
+        Args:
+            request: The incoming HTTP request.
+            call_next: A callable that proceeds to the next middleware or actual request handler.
+
+        Returns:
+            Response: The HTTP response generated by handling the request.
+        """
+        start_time = time.time()
+        response = await call_next(request)
+        process_time = time.time() - start_time
+        self.logger.timespec(
+            f"Request to {request.url.path} took {process_time:.2f} seconds"
+        )
+        return response
+
+
+def log_time(start_time, end_time, message=None):
+    """
+    Log the time duration between two time points with an optional message.
+
+    This function calculates the duration between `start_time` and `end_time`
+    and logs it with an optional message for context.
+
+    Args:
+        start_time (float): The start time in seconds.
+        end_time (float): The end time in seconds.
+        message (str, optional): An optional message to include in the log. Defaults to None.
+    """
+    duration = end_time - start_time
+    logger = TGCLoggerSetup(__name__, level="DEBUG", logger=TGCLogger(__name__))
+    logger.timespec(f"{message}: {duration:.2f} seconds")
```

### Comparing `tgctoolbox-0.1/tgctoolbox/vosk.py` & `tgctoolbox-0.2/tgctoolbox/vosk.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,63 @@
-import vosk
-from vosk import KaldiRecognizer
-import json
-import logging
-from tgctoolbox import TGCLoggerSetup
-
-# Initialize logger
-logger = TGCLoggerSetup("vosk", level="INFO")
-
-def transcribe_vosk(audio_data, kaldi_recognizer: KaldiRecognizer = None, verbose=False, include_partial=False):
-    """
-    Transcribe audio data using the Vosk model.
-    
-    Args:
-        audio_data: The audio data to be transcribed.
-        kaldi_recognizer (KaldiRecognizer): The KaldiRecognizer instance.
-        verbose (bool): Flag to set verbose logging.
-
-    Returns:
-        The transcription result as a string.
-    
-    Raises:
-        ValueError: If Kaldi recognizer is not specified or audio data is invalid.
-    """
-
-    # Check if Kaldi recognizer is specified
-    if kaldi_recognizer is None:
-        logger.error("Kaldi recognizer is not specified.")
-        raise ValueError("Kaldi recognizer is not specified.")
-
-    # Check the validity of audio data
-    if not audio_data:
-        logger.error("Invalid or empty audio data received.")
-        raise ValueError("Invalid or empty audio data.")
-
-    # Set logging level
-    vosk.SetLogLevel(0 if verbose else -1)
-    
-    # Start transcription variable
-    transcription = ''
-    
-    try:
-        # Process audio data and transcribe
-        if kaldi_recognizer.AcceptWaveform(audio_data):
-            result = json.loads(kaldi_recognizer.Result())
-            transcription = result.get('text', '')
-        elif include_partial:
-            partial_result = json.loads(kaldi_recognizer.PartialResult())
-            transcription = partial_result.get('partial', '')
-
-        return transcription
-
-    except Exception as e:
-        logger.error(f"Error during transcription: {e}", exc_info=True)
-        raise e
+import json
+import logging
+
+import vosk
+from vosk import KaldiRecognizer
+
+from .logger import setup_custom_logger as TGCLoggerSetup
+
+# Initialize logger
+logger = TGCLoggerSetup("vosk", level="INFO")
+
+
+def transcribe_vosk(
+    audio_data,
+    kaldi_recognizer: KaldiRecognizer = None,
+    verbose=False,
+    include_partial=False,
+):
+    """
+    Transcribe audio data using the Vosk model.
+
+    Args:
+        audio_data: The audio data to be transcribed.
+        kaldi_recognizer (KaldiRecognizer): The KaldiRecognizer instance.
+        verbose (bool): Flag to set verbose logging.
+
+    Returns:
+        The transcription result as a string.
+
+    Raises:
+        ValueError: If Kaldi recognizer is not specified or audio data is invalid.
+    """
+
+    # Check if Kaldi recognizer is specified
+    if kaldi_recognizer is None:
+        logger.error("Kaldi recognizer is not specified.")
+        raise ValueError("Kaldi recognizer is not specified.")
+
+    # Check the validity of audio data
+    if not audio_data:
+        logger.error("Invalid or empty audio data received.")
+        raise ValueError("Invalid or empty audio data.")
+
+    # Set logging level
+    vosk.SetLogLevel(0 if verbose else -1)
+
+    # Start transcription variable
+    transcription = ""
+
+    try:
+        # Process audio data and transcribe
+        if kaldi_recognizer.AcceptWaveform(audio_data):
+            result = json.loads(kaldi_recognizer.Result())
+            transcription = result.get("text", "")
+        elif include_partial:
+            partial_result = json.loads(kaldi_recognizer.PartialResult())
+            transcription = partial_result.get("partial", "")
+
+        return transcription
+
+    except Exception as e:
+        logger.error(f"Error during transcription: {e}", exc_info=True)
+        raise e
```

### Comparing `tgctoolbox-0.1/PKG-INFO` & `tgctoolbox-0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: tgctoolbox
-Version: 0.1
+Version: 0.2
 Summary: Comprehensive toolbox with all of the utils and tools used in various TGC projects.
 Author: Jakub Muszyński
 Author-email: jakub.m.muszynski@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: audio
 Requires-Dist: colorama
 Requires-Dist: moviepy
 Requires-Dist: pytube
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests
 Requires-Dist: starlette
 Requires-Dist: tqdm
 Requires-Dist: vosk
 Requires-Dist: websocket
```

