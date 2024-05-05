# Comparing `tmp/PKDevTools-0.13.20240501.109.tar.gz` & `tmp/PKDevTools-0.13.20240505.110.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKDevTools-0.13.20240501.109.tar", last modified: Wed May  1 19:03:13 2024, max compression
+gzip compressed data, was "PKDevTools-0.13.20240505.110.tar", last modified: Sun May  5 06:13:58 2024, max compression
```

## Comparing `PKDevTools-0.13.20240501.109.tar` & `PKDevTools-0.13.20240505.110.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 19:03:13.428426 PKDevTools-0.13.20240501.109/
--rw-rw-rw-   0        0        0     1086 2024-05-01 19:02:02.000000 PKDevTools-0.13.20240501.109/LICENSE
-drwxrwxrwx   0        0        0        0 2024-05-01 19:03:13.412803 PKDevTools-0.13.20240501.109/PKDevTools/
--rw-rw-rw-   0        0        0     1176 2024-05-01 19:02:02.000000 PKDevTools-0.13.20240501.109/PKDevTools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 19:03:13.428426 PKDevTools-0.13.20240501.109/PKDevTools/classes/
--rw-rw-rw-   0        0        0     3402 2024-05-01 19:02:02.000000 PKDevTools-0.13.20240501.109/PKDevTools/classes/Archiver.py
--rw-rw-rw-   0        0        0     5178 2024-05-01 19:02:02.000000 PKDevTools-0.13.20240501.109/PKDevTools/classes/ColorText.py
--rw-rw-rw-   0        0        0     3599 2024-05-01 19:02:02.000000 PKDevTools-0.13.20240501.109/PKDevTools/classes/Committer.py
--rw-rw-rw-   0        0        0     6380 2024-05-01 19:02:02.000000 PKDevTools-0.13.20240501.109/PKDevTools/classes/CookieHelper.py
--rw-rw-rw-   0        0        0     8879 2024-05-01 19:02:02.000000 PKDevTools-0.13.20240501.109/PKDevTools/classes/Fetcher.py
--rw-rw-rw-   0        0        0    11963 2024-05-01 19:02:02.000000 PKDevTools-0.13.20240501.109/PKDevTools/classes/MenuOptions.py
--rw-rw-rw-   0        0        0     2534 2024-05-01 19:02:02.000000 PKDevTools-0.13.20240501.109/PKDevTools/classes/OutputControls.py
--rw-rw-rw-   0        0        0    14378 2024-05-01 19:02:02.000000 PKDevTools-0.13.20240501.109/PKDevTools/classes/PKDateUtilities.py
--rw-rw-rw-   0        0        0     2988 2024-05-01 19:02:02.000000 PKDevTools-0.13.20240501.109/PKDevTools/classes/PKGitFolderDownloader.py
--rw-rw-rw-   0        0        0     5081 2024-05-01 19:02:02.000000 PKDevTools-0.13.20240501.109/PKDevTools/classes/PKJoinableQueue.py
--rw-rw-rw-   0        0        0    10828 2024-05-01 19:02:02.000000 PKDevTools-0.13.20240501.109/PKDevTools/classes/PKMultiProcessorClient.py
--rw-rw-rw-   0        0        0    14334 2024-05-01 19:02:02.000000 PKDevTools-0.13.20240501.109/PKDevTools/classes/PKPickler.py
--rw-rw-rw-   0        0        0     3433 2024-05-01 19:02:02.000000 PKDevTools-0.13.20240501.109/PKDevTools/classes/PKTimer.py
--rw-rw-rw-   0        0        0     4548 2024-05-01 19:02:02.000000 PKDevTools-0.13.20240501.109/PKDevTools/classes/Singleton.py
--rw-rw-rw-   0        0        0     2004 2024-05-01 19:02:02.000000 PKDevTools-0.13.20240501.109/PKDevTools/classes/SuppressOutput.py
--rw-rw-rw-   0        0        0    11301 2024-05-01 19:02:02.000000 PKDevTools-0.13.20240501.109/PKDevTools/classes/Telegram.py
--rw-rw-rw-   0        0        0    24543 2024-05-01 19:02:02.000000 PKDevTools-0.13.20240501.109/PKDevTools/classes/Utils.py
--rw-rw-rw-   0        0        0     9984 2024-05-01 19:02:02.000000 PKDevTools-0.13.20240501.109/PKDevTools/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-01 19:03:08.000000 PKDevTools-0.13.20240501.109/PKDevTools/classes/__init__.py
--rw-rw-rw-   0        0        0     3738 2024-05-01 19:02:02.000000 PKDevTools-0.13.20240501.109/PKDevTools/classes/githubutilities.py
--rw-rw-rw-   0        0        0    16136 2024-05-01 19:02:02.000000 PKDevTools-0.13.20240501.109/PKDevTools/classes/log.py
--rw-rw-rw-   0        0        0     7430 2024-05-01 19:02:02.000000 PKDevTools-0.13.20240501.109/PKDevTools/classes/multiprocessing_logging.py
--rw-rw-rw-   0        0        0     2864 2024-05-01 19:02:02.000000 PKDevTools-0.13.20240501.109/PKDevTools/classes/squash.py
--rw-rw-rw-   0        0        0     4846 2024-05-01 19:02:02.000000 PKDevTools-0.13.20240501.109/PKDevTools/classes/updater.py
-drwxrwxrwx   0        0        0        0 2024-05-01 19:03:13.428426 PKDevTools-0.13.20240501.109/PKDevTools.egg-info/
--rw-rw-rw-   0        0        0     5204 2024-05-01 19:03:13.000000 PKDevTools-0.13.20240501.109/PKDevTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1122 2024-05-01 19:03:13.000000 PKDevTools-0.13.20240501.109/PKDevTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 19:03:13.000000 PKDevTools-0.13.20240501.109/PKDevTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      363 2024-05-01 19:03:13.000000 PKDevTools-0.13.20240501.109/PKDevTools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-01 19:03:06.000000 PKDevTools-0.13.20240501.109/PKDevTools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      176 2024-05-01 19:03:13.000000 PKDevTools-0.13.20240501.109/PKDevTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-01 19:03:13.000000 PKDevTools-0.13.20240501.109/PKDevTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5204 2024-05-01 19:03:13.428426 PKDevTools-0.13.20240501.109/PKG-INFO
--rw-rw-rw-   0        0        0     4290 2024-05-01 19:02:02.000000 PKDevTools-0.13.20240501.109/README.md
--rw-rw-rw-   0        0        0       86 2024-05-01 19:03:13.428426 PKDevTools-0.13.20240501.109/setup.cfg
--rw-rw-rw-   0        0        0     4341 2024-05-01 19:02:02.000000 PKDevTools-0.13.20240501.109/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 06:13:58.337943 PKDevTools-0.13.20240505.110/
+-rw-rw-rw-   0        0        0     1086 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-05 06:13:58.322325 PKDevTools-0.13.20240505.110/PKDevTools/
+-rw-rw-rw-   0        0        0     1176 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 06:13:58.337943 PKDevTools-0.13.20240505.110/PKDevTools/classes/
+-rw-rw-rw-   0        0        0     3402 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/Archiver.py
+-rw-rw-rw-   0        0        0     5178 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/ColorText.py
+-rw-rw-rw-   0        0        0     3599 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/Committer.py
+-rw-rw-rw-   0        0        0     6376 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/CookieHelper.py
+-rw-rw-rw-   0        0        0     8879 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    11963 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0     2534 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/OutputControls.py
+-rw-rw-rw-   0        0        0    14378 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/PKDateUtilities.py
+-rw-rw-rw-   0        0        0     2988 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/PKGitFolderDownloader.py
+-rw-rw-rw-   0        0        0     5081 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/PKJoinableQueue.py
+-rw-rw-rw-   0        0        0    10828 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/PKMultiProcessorClient.py
+-rw-rw-rw-   0        0        0    14334 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/PKPickler.py
+-rw-rw-rw-   0        0        0     3433 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/PKTimer.py
+-rw-rw-rw-   0        0        0     4548 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/Singleton.py
+-rw-rw-rw-   0        0        0     2004 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/SuppressOutput.py
+-rw-rw-rw-   0        0        0    11301 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/Telegram.py
+-rw-rw-rw-   0        0        0    24543 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/Utils.py
+-rw-rw-rw-   0        0        0     9984 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-05 06:13:51.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/__init__.py
+-rw-rw-rw-   0        0        0     3738 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/githubutilities.py
+-rw-rw-rw-   0        0        0    16136 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/log.py
+-rw-rw-rw-   0        0        0     7430 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/multiprocessing_logging.py
+-rw-rw-rw-   0        0        0     2864 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/squash.py
+-rw-rw-rw-   0        0        0     4846 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/updater.py
+drwxrwxrwx   0        0        0        0 2024-05-05 06:13:58.322325 PKDevTools-0.13.20240505.110/PKDevTools.egg-info/
+-rw-rw-rw-   0        0        0     5204 2024-05-05 06:13:58.000000 PKDevTools-0.13.20240505.110/PKDevTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1122 2024-05-05 06:13:58.000000 PKDevTools-0.13.20240505.110/PKDevTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 06:13:58.000000 PKDevTools-0.13.20240505.110/PKDevTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      363 2024-05-05 06:13:58.000000 PKDevTools-0.13.20240505.110/PKDevTools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-05 06:13:49.000000 PKDevTools-0.13.20240505.110/PKDevTools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      176 2024-05-05 06:13:58.000000 PKDevTools-0.13.20240505.110/PKDevTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-05 06:13:58.000000 PKDevTools-0.13.20240505.110/PKDevTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5204 2024-05-05 06:13:58.337943 PKDevTools-0.13.20240505.110/PKG-INFO
+-rw-rw-rw-   0        0        0     4290 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-05 06:13:58.337943 PKDevTools-0.13.20240505.110/setup.cfg
+-rw-rw-rw-   0        0        0     4341 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/setup.py
```

### Comparing `PKDevTools-0.13.20240501.109/LICENSE` & `PKDevTools-0.13.20240505.110/LICENSE`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240501.109/PKDevTools/__init__.py` & `PKDevTools-0.13.20240505.110/PKDevTools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240501.109/PKDevTools/classes/Archiver.py` & `PKDevTools-0.13.20240505.110/PKDevTools/classes/Archiver.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240501.109/PKDevTools/classes/ColorText.py` & `PKDevTools-0.13.20240505.110/PKDevTools/classes/ColorText.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240501.109/PKDevTools/classes/Committer.py` & `PKDevTools-0.13.20240505.110/PKDevTools/classes/Committer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240501.109/PKDevTools/classes/CookieHelper.py` & `PKDevTools-0.13.20240505.110/PKDevTools/classes/CookieHelper.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         - ``ConnectionError`` if request failed for any reason.
 
     :param download_folder: A folder/dir to save downloaded files and cookie files
     :type download_folder: pathlib.Path or str
     :raise ValueError: if ``download_folder`` is not a folder/dir
     '''
 
-    def __init__(self, download_folder: Union[str, Path], baseCookieUrl='https://www.nseindia.com/option-chain', cookieStoreName='nse', baseHtmlUrl = 'https://www.nseindia.com/option-chain', htmlStoreName='nse'):
+    def __init__(self, download_folder: Union[str, Path], baseCookieUrl='https://www.nseindia.com/option-chain', cookieStoreName='n', baseHtmlUrl = 'https://www.nseindia.com/option-chain', htmlStoreName='n'):
         '''Initialise NSE'''
 
         uAgent = 'Mozilla/5.0 (Windows NT 10.0; rv:109.0) Gecko/20100101 Firefox/118.0'
 
         self.default_headers = {
             'User-Agent': uAgent,
             'Accept': '*/*',
```

### Comparing `PKDevTools-0.13.20240501.109/PKDevTools/classes/Fetcher.py` & `PKDevTools-0.13.20240505.110/PKDevTools/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240501.109/PKDevTools/classes/MenuOptions.py` & `PKDevTools-0.13.20240505.110/PKDevTools/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240501.109/PKDevTools/classes/OutputControls.py` & `PKDevTools-0.13.20240505.110/PKDevTools/classes/OutputControls.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240501.109/PKDevTools/classes/PKDateUtilities.py` & `PKDevTools-0.13.20240505.110/PKDevTools/classes/PKDateUtilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240501.109/PKDevTools/classes/PKGitFolderDownloader.py` & `PKDevTools-0.13.20240505.110/PKDevTools/classes/PKGitFolderDownloader.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240501.109/PKDevTools/classes/PKJoinableQueue.py` & `PKDevTools-0.13.20240505.110/PKDevTools/classes/PKJoinableQueue.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240501.109/PKDevTools/classes/PKMultiProcessorClient.py` & `PKDevTools-0.13.20240505.110/PKDevTools/classes/PKMultiProcessorClient.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240501.109/PKDevTools/classes/PKPickler.py` & `PKDevTools-0.13.20240505.110/PKDevTools/classes/PKPickler.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240501.109/PKDevTools/classes/PKTimer.py` & `PKDevTools-0.13.20240505.110/PKDevTools/classes/PKTimer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240501.109/PKDevTools/classes/Singleton.py` & `PKDevTools-0.13.20240505.110/PKDevTools/classes/Singleton.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240501.109/PKDevTools/classes/SuppressOutput.py` & `PKDevTools-0.13.20240505.110/PKDevTools/classes/SuppressOutput.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240501.109/PKDevTools/classes/Telegram.py` & `PKDevTools-0.13.20240505.110/PKDevTools/classes/Telegram.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240501.109/PKDevTools/classes/Utils.py` & `PKDevTools-0.13.20240505.110/PKDevTools/classes/Utils.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240501.109/PKDevTools/classes/WorkflowManager.py` & `PKDevTools-0.13.20240505.110/PKDevTools/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240501.109/PKDevTools/classes/githubutilities.py` & `PKDevTools-0.13.20240505.110/PKDevTools/classes/githubutilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240501.109/PKDevTools/classes/log.py` & `PKDevTools-0.13.20240505.110/PKDevTools/classes/log.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240501.109/PKDevTools/classes/multiprocessing_logging.py` & `PKDevTools-0.13.20240505.110/PKDevTools/classes/multiprocessing_logging.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240501.109/PKDevTools/classes/squash.py` & `PKDevTools-0.13.20240505.110/PKDevTools/classes/squash.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240501.109/PKDevTools/classes/updater.py` & `PKDevTools-0.13.20240505.110/PKDevTools/classes/updater.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240501.109/PKDevTools.egg-info/PKG-INFO` & `PKDevTools-0.13.20240505.110/PKDevTools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240501.109
+Version: 0.13.20240505.110
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240501.109.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240505.110.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240501.109/PKDevTools.egg-info/SOURCES.txt` & `PKDevTools-0.13.20240505.110/PKDevTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240501.109/PKG-INFO` & `PKDevTools-0.13.20240505.110/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240501.109
+Version: 0.13.20240505.110
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240501.109.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240505.110.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240501.109/README.md` & `PKDevTools-0.13.20240505.110/README.md`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240501.109/setup.py` & `PKDevTools-0.13.20240505.110/setup.py`

 * *Files identical despite different names*
