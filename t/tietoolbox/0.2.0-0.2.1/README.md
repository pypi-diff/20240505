# Comparing `tmp/tietoolbox-0.2.0.tar.gz` & `tmp/tietoolbox-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tietoolbox-0.2.0.tar", last modified: Fri May  3 08:44:51 2024, max compression
+gzip compressed data, was "tietoolbox-0.2.1.tar", last modified: Sun May  5 07:52:11 2024, max compression
```

## Comparing `tietoolbox-0.2.0.tar` & `tietoolbox-0.2.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 08:44:51.279824 tietoolbox-0.2.0/
--rw-rw-rw-   0        0        0     1585 2024-04-22 06:47:24.000000 tietoolbox-0.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0      119 2024-04-22 06:47:24.000000 tietoolbox-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3352 2024-05-03 08:44:51.169831 tietoolbox-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1880 2024-04-22 06:47:24.000000 tietoolbox-0.2.0/README.md
--rw-rw-rw-   0        0        0        7 2024-05-03 08:34:36.000000 tietoolbox-0.2.0/VERSION
-drwxrwxrwx   0        0        0        0 2024-05-03 08:44:45.938848 tietoolbox-0.2.0/images/
--rw-rw-rw-   0        0        0    45673 2024-04-21 10:48:54.000000 tietoolbox-0.2.0/images/signal-height-diagram.png
--rw-rw-rw-   0        0        0   504466 2024-04-08 16:19:41.000000 tietoolbox-0.2.0/images/snapshot.png
--rw-rw-rw-   0        0        0   509539 2024-04-21 10:48:54.000000 tietoolbox-0.2.0/images/tie-analysis.png
--rw-rw-rw-   0        0        0       42 2024-05-03 08:44:51.282836 tietoolbox-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     2366 2024-05-03 08:34:22.000000 tietoolbox-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-03 08:44:47.380853 tietoolbox-0.2.0/tietoolbox/
--rw-rw-rw-   0        0        0       77 2024-04-21 10:48:54.000000 tietoolbox-0.2.0/tietoolbox/__init__.py
--rw-rw-rw-   0        0        0     4401 2024-04-04 13:01:18.000000 tietoolbox-0.2.0/tietoolbox/commonlogger.py
--rw-rw-rw-   0        0        0     2544 2024-04-04 13:01:18.000000 tietoolbox-0.2.0/tietoolbox/config.py
--rw-rw-rw-   0        0        0      494 2024-03-28 10:14:47.000000 tietoolbox-0.2.0/tietoolbox/debug.py
-drwxrwxrwx   0        0        0        0 2024-05-03 08:44:44.651883 tietoolbox-0.2.0/tietoolbox/esri/
-drwxrwxrwx   0        0        0        0 2024-05-03 08:44:49.715843 tietoolbox-0.2.0/tietoolbox/esri/toolboxes/
--rw-rw-rw-   0        0        0     1463 2024-05-03 07:15:22.000000 tietoolbox-0.2.0/tietoolbox/esri/toolboxes/TIEtoolbox.Analysis.pyt.xml
--rw-rw-rw-   0        0        0     1748 2024-05-03 07:15:22.000000 tietoolbox-0.2.0/tietoolbox/esri/toolboxes/TIEtoolbox.Downloader.pyt.xml
--rw-rw-rw-   0        0        0     1892 2024-05-03 07:15:22.000000 tietoolbox-0.2.0/tietoolbox/esri/toolboxes/TIEtoolbox.Exporter.pyt.xml
--rw-rw-rw-   0        0        0     1808 2024-05-03 07:15:22.000000 tietoolbox-0.2.0/tietoolbox/esri/toolboxes/TIEtoolbox.Viewer.pyt.xml
--rw-rw-rw-   0        0        0    21749 2024-05-03 08:34:36.000000 tietoolbox-0.2.0/tietoolbox/esri/toolboxes/TIEtoolbox.pyt
--rw-rw-rw-   0        0        0   207935 2024-05-03 08:27:56.000000 tietoolbox-0.2.0/tietoolbox/esri/toolboxes/TIEtoolbox.pyt.xml
--rw-rw-rw-   0        0        0    15529 2024-05-03 08:34:36.000000 tietoolbox-0.2.0/tietoolbox/feature_exporter.py
--rw-rw-rw-   0        0        0     5456 2024-04-21 10:48:54.000000 tietoolbox-0.2.0/tietoolbox/runner.py
-drwxrwxrwx   0        0        0        0 2024-05-03 08:44:50.888824 tietoolbox-0.2.0/tietoolbox/scripts/
--rw-rw-rw-   0        0        0        0 2024-04-04 13:01:18.000000 tietoolbox-0.2.0/tietoolbox/scripts/__init__.py
--rw-rw-rw-   0        0        0     3269 2024-04-04 13:01:18.000000 tietoolbox-0.2.0/tietoolbox/scripts/config.py
--rw-rw-rw-   0        0        0    96011 2024-04-04 13:01:18.000000 tietoolbox-0.2.0/tietoolbox/scripts/symbols.tsv
--rw-rw-rw-   0        0        0    16196 2024-05-03 08:34:36.000000 tietoolbox-0.2.0/tietoolbox/scripts/tie_analysis_dask.py
--rw-rw-rw-   0        0        0     5718 2024-04-30 14:55:39.000000 tietoolbox-0.2.0/tietoolbox/scripts/tie_viewer.py
--rw-rw-rw-   0        0        0     3337 2024-04-04 13:01:18.000000 tietoolbox-0.2.0/tietoolbox/scripts/traces_export_utils.py
--rw-rw-rw-   0        0        0     7091 2024-04-04 13:01:18.000000 tietoolbox-0.2.0/tietoolbox/scripts/utils.py
--rw-rw-rw-   0        0        0      126 2024-03-28 10:14:47.000000 tietoolbox-0.2.0/tietoolbox/test.py
--rw-rw-rw-   0        0        0      293 2024-04-04 13:01:18.000000 tietoolbox-0.2.0/tietoolbox/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-03 08:44:51.068836 tietoolbox-0.2.0/tietoolbox.egg-info/
--rw-rw-rw-   0        0        0     3352 2024-05-03 08:44:43.000000 tietoolbox-0.2.0/tietoolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1051 2024-05-03 08:44:44.000000 tietoolbox-0.2.0/tietoolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 08:44:43.000000 tietoolbox-0.2.0/tietoolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      124 2024-05-03 08:44:43.000000 tietoolbox-0.2.0/tietoolbox.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      171 2024-05-03 08:44:43.000000 tietoolbox-0.2.0/tietoolbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-03 08:44:43.000000 tietoolbox-0.2.0/tietoolbox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-05 07:52:11.488106 tietoolbox-0.2.1/
+-rw-rw-rw-   0        0        0     1585 2024-04-22 06:47:24.000000 tietoolbox-0.2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      119 2024-04-22 06:47:24.000000 tietoolbox-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3352 2024-05-05 07:52:11.295095 tietoolbox-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1880 2024-04-22 06:47:24.000000 tietoolbox-0.2.1/README.md
+-rw-rw-rw-   0        0        0        7 2024-05-05 07:48:49.000000 tietoolbox-0.2.1/VERSION
+drwxrwxrwx   0        0        0        0 2024-05-05 07:52:04.416139 tietoolbox-0.2.1/images/
+-rw-rw-rw-   0        0        0    45673 2024-04-21 10:48:54.000000 tietoolbox-0.2.1/images/signal-height-diagram.png
+-rw-rw-rw-   0        0        0   504466 2024-04-08 16:19:41.000000 tietoolbox-0.2.1/images/snapshot.png
+-rw-rw-rw-   0        0        0   509539 2024-04-21 10:48:54.000000 tietoolbox-0.2.1/images/tie-analysis.png
+-rw-rw-rw-   0        0        0       42 2024-05-05 07:52:11.516112 tietoolbox-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     2366 2024-05-03 08:34:22.000000 tietoolbox-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 07:52:06.378120 tietoolbox-0.2.1/tietoolbox/
+-rw-rw-rw-   0        0        0       77 2024-04-21 10:48:54.000000 tietoolbox-0.2.1/tietoolbox/__init__.py
+-rw-rw-rw-   0        0        0     4401 2024-04-04 13:01:18.000000 tietoolbox-0.2.1/tietoolbox/commonlogger.py
+-rw-rw-rw-   0        0        0     2544 2024-04-04 13:01:18.000000 tietoolbox-0.2.1/tietoolbox/config.py
+-rw-rw-rw-   0        0        0      494 2024-03-28 10:14:47.000000 tietoolbox-0.2.1/tietoolbox/debug.py
+drwxrwxrwx   0        0        0        0 2024-05-05 07:52:02.870144 tietoolbox-0.2.1/tietoolbox/esri/
+drwxrwxrwx   0        0        0        0 2024-05-05 07:52:09.061103 tietoolbox-0.2.1/tietoolbox/esri/toolboxes/
+-rw-rw-rw-   0        0        0     1463 2024-05-03 07:15:22.000000 tietoolbox-0.2.1/tietoolbox/esri/toolboxes/TIEtoolbox.Analysis.pyt.xml
+-rw-rw-rw-   0        0        0     1748 2024-05-03 07:15:22.000000 tietoolbox-0.2.1/tietoolbox/esri/toolboxes/TIEtoolbox.Downloader.pyt.xml
+-rw-rw-rw-   0        0        0     1892 2024-05-03 07:15:22.000000 tietoolbox-0.2.1/tietoolbox/esri/toolboxes/TIEtoolbox.Exporter.pyt.xml
+-rw-rw-rw-   0        0        0     1808 2024-05-03 07:15:22.000000 tietoolbox-0.2.1/tietoolbox/esri/toolboxes/TIEtoolbox.Viewer.pyt.xml
+-rw-rw-rw-   0        0        0    21812 2024-05-05 07:48:49.000000 tietoolbox-0.2.1/tietoolbox/esri/toolboxes/TIEtoolbox.pyt
+-rw-rw-rw-   0        0        0   207935 2024-05-03 08:27:56.000000 tietoolbox-0.2.1/tietoolbox/esri/toolboxes/TIEtoolbox.pyt.xml
+-rw-rw-rw-   0        0        0    15529 2024-05-03 08:34:36.000000 tietoolbox-0.2.1/tietoolbox/feature_exporter.py
+-rw-rw-rw-   0        0        0     5456 2024-04-21 10:48:54.000000 tietoolbox-0.2.1/tietoolbox/runner.py
+drwxrwxrwx   0        0        0        0 2024-05-05 07:52:10.786102 tietoolbox-0.2.1/tietoolbox/scripts/
+-rw-rw-rw-   0        0        0        0 2024-04-04 13:01:18.000000 tietoolbox-0.2.1/tietoolbox/scripts/__init__.py
+-rw-rw-rw-   0        0        0     3269 2024-04-04 13:01:18.000000 tietoolbox-0.2.1/tietoolbox/scripts/config.py
+-rw-rw-rw-   0        0        0    96011 2024-04-04 13:01:18.000000 tietoolbox-0.2.1/tietoolbox/scripts/symbols.tsv
+-rw-rw-rw-   0        0        0    16196 2024-05-03 08:34:36.000000 tietoolbox-0.2.1/tietoolbox/scripts/tie_analysis_dask.py
+-rw-rw-rw-   0        0        0     5718 2024-04-30 14:55:39.000000 tietoolbox-0.2.1/tietoolbox/scripts/tie_viewer.py
+-rw-rw-rw-   0        0        0     3337 2024-04-04 13:01:18.000000 tietoolbox-0.2.1/tietoolbox/scripts/traces_export_utils.py
+-rw-rw-rw-   0        0        0     7091 2024-04-04 13:01:18.000000 tietoolbox-0.2.1/tietoolbox/scripts/utils.py
+-rw-rw-rw-   0        0        0      126 2024-03-28 10:14:47.000000 tietoolbox-0.2.1/tietoolbox/test.py
+-rw-rw-rw-   0        0        0      293 2024-04-04 13:01:18.000000 tietoolbox-0.2.1/tietoolbox/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-05 07:52:11.099097 tietoolbox-0.2.1/tietoolbox.egg-info/
+-rw-rw-rw-   0        0        0     3352 2024-05-05 07:52:00.000000 tietoolbox-0.2.1/tietoolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1051 2024-05-05 07:52:02.000000 tietoolbox-0.2.1/tietoolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 07:52:01.000000 tietoolbox-0.2.1/tietoolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      124 2024-05-05 07:52:01.000000 tietoolbox-0.2.1/tietoolbox.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      171 2024-05-05 07:52:01.000000 tietoolbox-0.2.1/tietoolbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-05 07:52:01.000000 tietoolbox-0.2.1/tietoolbox.egg-info/top_level.txt
```

### Comparing `tietoolbox-0.2.0/LICENSE.txt` & `tietoolbox-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tietoolbox-0.2.0/PKG-INFO` & `tietoolbox-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tietoolbox
-Version: 0.2.0
+Version: 0.2.1
 Summary: Basic ESRI ArcMap/ArcGis Pro TIE Toolbox to perform Trace Information Extraction (TIE) Analysis.
 Author: swisstopo
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering :: Image Processing
```

### Comparing `tietoolbox-0.2.0/README.md` & `tietoolbox-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tietoolbox-0.2.0/images/signal-height-diagram.png` & `tietoolbox-0.2.1/images/signal-height-diagram.png`

 * *Files identical despite different names*

### Comparing `tietoolbox-0.2.0/images/snapshot.png` & `tietoolbox-0.2.1/images/snapshot.png`

 * *Files identical despite different names*

### Comparing `tietoolbox-0.2.0/images/tie-analysis.png` & `tietoolbox-0.2.1/images/tie-analysis.png`

 * *Files identical despite different names*

### Comparing `tietoolbox-0.2.0/setup.py` & `tietoolbox-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `tietoolbox-0.2.0/tietoolbox/commonlogger.py` & `tietoolbox-0.2.1/tietoolbox/commonlogger.py`

 * *Files identical despite different names*

### Comparing `tietoolbox-0.2.0/tietoolbox/config.py` & `tietoolbox-0.2.1/tietoolbox/config.py`

 * *Files identical despite different names*

### Comparing `tietoolbox-0.2.0/tietoolbox/esri/toolboxes/TIEtoolbox.Analysis.pyt.xml` & `tietoolbox-0.2.1/tietoolbox/esri/toolboxes/TIEtoolbox.Analysis.pyt.xml`

 * *Files identical despite different names*

### Comparing `tietoolbox-0.2.0/tietoolbox/esri/toolboxes/TIEtoolbox.Downloader.pyt.xml` & `tietoolbox-0.2.1/tietoolbox/esri/toolboxes/TIEtoolbox.Downloader.pyt.xml`

 * *Files identical despite different names*

### Comparing `tietoolbox-0.2.0/tietoolbox/esri/toolboxes/TIEtoolbox.Exporter.pyt.xml` & `tietoolbox-0.2.1/tietoolbox/esri/toolboxes/TIEtoolbox.Exporter.pyt.xml`

 * *Files identical despite different names*

### Comparing `tietoolbox-0.2.0/tietoolbox/esri/toolboxes/TIEtoolbox.Viewer.pyt.xml` & `tietoolbox-0.2.1/tietoolbox/esri/toolboxes/TIEtoolbox.Viewer.pyt.xml`

 * *Files identical despite different names*

### Comparing `tietoolbox-0.2.0/tietoolbox/esri/toolboxes/TIEtoolbox.pyt` & `tietoolbox-0.2.1/tietoolbox/esri/toolboxes/TIEtoolbox.pyt`

 * *Files 1% similar despite different names*

```diff
@@ -45,28 +45,25 @@
     STARTUPINFO,
     STDOUT,
     CalledProcessError,
     Popen,
 )
 from threading import Timer
 
-
 from tietoolbox import commonlogger, feature_exporter, utils, runner as tie_runner
 from tietoolbox.runner import Runner
 
-
 # TODO: disabling
 DEBUG = True
 MAX_LINES = 1000
 
 if DEBUG:
     sys.dont_write_bytecode = True
     imp.reload(tie_runner)
 
-
 # Python2,3
 
 
 class PythonNotFound(Exception):
     pass
 
 
@@ -133,17 +130,18 @@
             sys.exit(2)
 
     def get_path(self, name):
         # H:\code\arcmap-tie-toolbox\toolbox\tietoolbox\esri\toolboxes
         path = os.path.abspath(os.path.join(self.current_dir, "../../.."))
         arcpy.AddMessage(path)
         for root, dirs, files in os.walk(path):
-            arcpy.AddMessage(files)
             if name in files:
-                return os.path.join(root, name)
+                script_path = os.path.join(root, name)
+                arcpy.AddMessage("Found script at {}".format(script_path))
+                return script_path
         return None
 
     @property
     def python_exe(self, exe_name="python.exe"):
         if self._python_exe is not None:
             return self._python_exe
         if six.PY3:
@@ -470,15 +468,15 @@
         cmd = 'cmd "/c activate {} && {}  && deactivate && exit 0"'.format(
             self.conda_env_path, cmd
         )
 
         ret = runner.running(
             cmd,
             callback=arcpy.AddMessage,
-            working_dir=r"H:\code\geocover-examples\tie",
+            working_dir=self.conda_env_path,
             minimized=True,
         )
 
         if ret == 0:
             arcpy.AddMessage("Success")
 
         return
```

### Comparing `tietoolbox-0.2.0/tietoolbox/esri/toolboxes/TIEtoolbox.pyt.xml` & `tietoolbox-0.2.1/tietoolbox/esri/toolboxes/TIEtoolbox.pyt.xml`

 * *Files identical despite different names*

### Comparing `tietoolbox-0.2.0/tietoolbox/feature_exporter.py` & `tietoolbox-0.2.1/tietoolbox/feature_exporter.py`

 * *Files identical despite different names*

### Comparing `tietoolbox-0.2.0/tietoolbox/runner.py` & `tietoolbox-0.2.1/tietoolbox/runner.py`

 * *Files identical despite different names*

### Comparing `tietoolbox-0.2.0/tietoolbox/scripts/config.py` & `tietoolbox-0.2.1/tietoolbox/scripts/config.py`

 * *Files identical despite different names*

### Comparing `tietoolbox-0.2.0/tietoolbox/scripts/symbols.tsv` & `tietoolbox-0.2.1/tietoolbox/scripts/symbols.tsv`

 * *Files identical despite different names*

### Comparing `tietoolbox-0.2.0/tietoolbox/scripts/tie_analysis_dask.py` & `tietoolbox-0.2.1/tietoolbox/scripts/tie_analysis_dask.py`

 * *Files identical despite different names*

### Comparing `tietoolbox-0.2.0/tietoolbox/scripts/tie_viewer.py` & `tietoolbox-0.2.1/tietoolbox/scripts/tie_viewer.py`

 * *Files identical despite different names*

### Comparing `tietoolbox-0.2.0/tietoolbox/scripts/traces_export_utils.py` & `tietoolbox-0.2.1/tietoolbox/scripts/traces_export_utils.py`

 * *Files identical despite different names*

### Comparing `tietoolbox-0.2.0/tietoolbox/scripts/utils.py` & `tietoolbox-0.2.1/tietoolbox/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `tietoolbox-0.2.0/tietoolbox.egg-info/PKG-INFO` & `tietoolbox-0.2.1/tietoolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tietoolbox
-Version: 0.2.0
+Version: 0.2.1
 Summary: Basic ESRI ArcMap/ArcGis Pro TIE Toolbox to perform Trace Information Extraction (TIE) Analysis.
 Author: swisstopo
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering :: Image Processing
```

### Comparing `tietoolbox-0.2.0/tietoolbox.egg-info/SOURCES.txt` & `tietoolbox-0.2.1/tietoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

