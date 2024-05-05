# Comparing `tmp/fixraidenboss2-3.7.0.tar.gz` & `tmp/fixraidenboss2-3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixraidenboss2-3.7.0.tar", last modified: Sat May  4 20:32:33 2024, max compression
+gzip compressed data, was "fixraidenboss2-3.7.1.tar", last modified: Sun May  5 12:22:38 2024, max compression
```

## Comparing `fixraidenboss2-3.7.0.tar` & `fixraidenboss2-3.7.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:32:33.104026 fixraidenboss2-3.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-04 20:32:29.000000 fixraidenboss2-3.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16284 2024-05-04 20:32:33.104026 fixraidenboss2-3.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15682 2024-05-04 20:32:29.000000 fixraidenboss2-3.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-04 20:32:29.000000 fixraidenboss2-3.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 20:32:33.104026 fixraidenboss2-3.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:32:33.100026 fixraidenboss2-3.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:32:33.100026 fixraidenboss2-3.7.0/src/FixRaidenBoss2/
--rw-r--r--   0 runner    (1001) docker     (127)   177578 2024-05-04 20:32:29.000000 fixraidenboss2-3.7.0/src/FixRaidenBoss2/FixRaidenBoss2.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-04 20:32:29.000000 fixraidenboss2-3.7.0/src/FixRaidenBoss2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-04 20:32:29.000000 fixraidenboss2-3.7.0/src/FixRaidenBoss2/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:32:33.104026 fixraidenboss2-3.7.0/src/FixRaidenBoss2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16284 2024-05-04 20:32:33.000000 fixraidenboss2-3.7.0/src/FixRaidenBoss2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-04 20:32:33.000000 fixraidenboss2-3.7.0/src/FixRaidenBoss2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 20:32:33.000000 fixraidenboss2-3.7.0/src/FixRaidenBoss2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-04 20:32:33.000000 fixraidenboss2-3.7.0/src/FixRaidenBoss2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:22:38.294975 fixraidenboss2-3.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-05 12:22:29.000000 fixraidenboss2-3.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16284 2024-05-05 12:22:38.294975 fixraidenboss2-3.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15682 2024-05-05 12:22:29.000000 fixraidenboss2-3.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-05 12:22:29.000000 fixraidenboss2-3.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 12:22:38.294975 fixraidenboss2-3.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:22:38.294975 fixraidenboss2-3.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:22:38.294975 fixraidenboss2-3.7.1/src/FixRaidenBoss2/
+-rw-r--r--   0 runner    (1001) docker     (127)   179600 2024-05-05 12:22:29.000000 fixraidenboss2-3.7.1/src/FixRaidenBoss2/FixRaidenBoss2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-05 12:22:29.000000 fixraidenboss2-3.7.1/src/FixRaidenBoss2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-05 12:22:29.000000 fixraidenboss2-3.7.1/src/FixRaidenBoss2/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:22:38.294975 fixraidenboss2-3.7.1/src/FixRaidenBoss2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16284 2024-05-05 12:22:38.000000 fixraidenboss2-3.7.1/src/FixRaidenBoss2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-05 12:22:38.000000 fixraidenboss2-3.7.1/src/FixRaidenBoss2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 12:22:38.000000 fixraidenboss2-3.7.1/src/FixRaidenBoss2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-05 12:22:38.000000 fixraidenboss2-3.7.1/src/FixRaidenBoss2.egg-info/top_level.txt
```

### Comparing `fixraidenboss2-3.7.0/LICENSE` & `fixraidenboss2-3.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fixraidenboss2-3.7.0/PKG-INFO` & `fixraidenboss2-3.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FixRaidenBoss2
-Version: 3.7.0
+Version: 3.7.1
 Summary: A script to fix Raiden Shogun Boss Phase 1 for all types of mods
 Author-email: nhok0169 <qqqqaaaapppp0000@gmail.com>, Albert Gold <AlexXianZhenYuAu@gmail.com>
 Project-URL: Homepage, https://github.com/nhok0169/Fix-Raiden-Boss
 Project-URL: Documentation, https://fix-raiden-boss.readthedocs.io/en/latest
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: FixRaidenBoss2 Version: 3.7.0 Summary: A script to
+Metadata-Version: 2.1 Name: FixRaidenBoss2 Version: 3.7.1 Summary: A script to
 fix Raiden Shogun Boss Phase 1 for all types of mods Author-email: nhok0169
 gmail.com>, Albert Gold
 gmail.com> Project-URL: Homepage, https://github.com/nhok0169/Fix-Raiden-Boss
 Project-URL: Documentation, https://fix-raiden-boss.readthedocs.io/en/latest
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
```

### Comparing `fixraidenboss2-3.7.0/README.md` & `fixraidenboss2-3.7.1/README.md`

 * *Files identical despite different names*

### Comparing `fixraidenboss2-3.7.0/pyproject.toml` & `fixraidenboss2-3.7.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "FixRaidenBoss2"
-version = "3.7.0"
+version = "3.7.1"
 authors = [
   {name="nhok0169", email="qqqqaaaapppp0000@gmail.com"},
   {name="Albert Gold", email="AlexXianZhenYuAu@gmail.com"}
 ]
 description = "A script to fix Raiden Shogun Boss Phase 1 for all types of mods"
 readme = "README.md"
 classifiers = [
```

### Comparing `fixraidenboss2-3.7.0/src/FixRaidenBoss2/FixRaidenBoss2.py` & `fixraidenboss2-3.7.1/src/FixRaidenBoss2/FixRaidenBoss2.py`

 * *Files 1% similar despite different names*

```diff
@@ -982,14 +982,21 @@
         The text to be logged into a .txt file
 
         :getter: Returns such a prefix
         :type: :class:`str`
         """
         return self._loggedTxt
 
+    def clear(self):
+        """
+        Clears out any saved text from the logger
+        """
+
+        self._loggedTxt = ""
+
     def _setDefaultHeadingAtts(self):
         """
         Sets the default attributes for printing out a header line
         """
 
         self._headingTxtLen = 0
         self._headingSideLen = self.DefaultHeadingSideLen
@@ -4044,16 +4051,15 @@
             if (remapBlendsRemoved):
                 self.print("space")
 
             if (iniHasErrors):
                 continue
 
             # remove the fix from the .ini files
-            if (iniFullPath is not None and iniFullPath not in fixedInis and iniFullPath not in inisSkipped and 
-                ini.isModIni and (not self._types or ini.type in self._types)):
+            if (iniFullPath is not None and iniFullPath not in fixedInis and iniFullPath not in inisSkipped and ini.isModIni):
                 try:
                     ini.removeFix(keepBackups = keepBackups, fixOnly = fixOnly)
                 except Exception as e:
                     inisSkipped[iniFullPath] = e
                     iniHasErrors = True
                     self.print("handleException", e)
                     continue
@@ -4149,15 +4155,15 @@
             with open(fixedBlendFile, "wb") as f:
                 f.write(result)
 
             return fixedBlendFile
 
         return result
     
-    def correctBlend(self, fixedRemapBlends: Dict[str, RemapBlendModel], skippedBlends: Dict[str, Exception]) -> List[Union[Set[str], Dict[str, Exception]]]:
+    def correctBlend(self, fixedRemapBlends: Dict[str, RemapBlendModel], skippedBlends: Dict[str, Exception], fixOnly: bool = False) -> List[Union[Set[str], Dict[str, Exception]]]:
         """
         Fixes all the Blend.buf files reference by the mod
 
         Requires all the .ini files in the mod to have ran their :meth:`IniFile.parse` function
 
         Parameters
         ----------
@@ -4168,14 +4174,19 @@
             to the fixed RemapBlend.buf file
 
         skippedBlends: Dict[:class:`str`, :class:`Exception`]
             All of the RemapBlend.buf files that have already been skipped due to some error when trying to fix them :raw-html:`<br />` :raw-html:`<br />`
 
             The keys are the absolute filepath to the RemapBlend.buf file that was attempted to be fixed and the values are the exception encountered
 
+        fixOnly: :class:`bool`
+            Whether to not correct some Blend.buf file if its corresponding RemapBlend.buf already exists :raw-html:`<br />` :raw-html:`<br />`
+
+            **Default**: ``True``
+
         Returns
         -------
         [Set[:class:`str`], Dict[:class:`str`, :class:`Exception`]]
             #. The absolute file paths of the RemapBlend.buf files that were fixed
             #. The exceptions encountered when trying to fix some RemapBlend.buf files :raw-html:`<br />` :raw-html:`<br />`
 
             The keys are absolute filepath to the RemapBlend.buf file and the values are the exception encountered
@@ -4231,15 +4242,21 @@
                             targetFullPath = origFullPath
 
                         self.print("log", f"Blend file has already previously encountered an error at {targetFullPath}")
                         continue
 
                     if (blendFixed or modType is None):
                         continue
+
+                    # check if the fixed RemapBlend.buf file already exists and we only want to fix mods without removing their previous fixes
+                    if (fixOnly and os.path.isfile(fixedFullPath)):
+                        self.print("log", f"Blend file was previously fixed at {fixedFullPath}")
+                        continue
                     
+                    # fix the blend
                     correctedBlendPath = None
                     try:
                         correctedBlendPath = self.blendCorrection(origFullPath, modType, fixedBlendFile = fixedFullPath)
                     except Exception as e:
                         currentBlendsSkipped[fixedFullPath] = e
                         skippedBlends[fixedFullPath] = e
                         self.print("handleException", e)
@@ -4330,17 +4347,14 @@
     handleExceptions: :class:`bool`
         When an exception is caught, whether to silently stop running the fix :raw-html:`<br />` :raw-html:`<br />`
 
         **Default**: ``False``
 
     Attributes
     ----------
-    log: Optional[:class:`str`]
-        The folder location to log the run of the fix into a seperate text file
-
     _loggerBasePrefix: :class:`str`
         The prefix string for the logger used when the fix returns back to the original directory that it started to run
 
     logger: :class:`Logger`
         The logger used to pretty print messages
 
     _path: :class:`str`
@@ -4405,14 +4419,21 @@
     inisSkipped: Dict[:class:`str`, :class:`Exception`]
         The .ini files that got skipped :raw-html:`<br />` :raw-html:`<br />`
 
         The keys are the absolute file paths to the .ini files and the values are exceptions that caused the .ini file to be skipped
 
     removedRemapBlends: Set[:class:`str`]
         Previous RemapBlend.buf files that are removed
+
+    undoedInis: Set[:class:`str`]
+        .ini files that got cleared out of any traces of previous fixes
+
+        .. note::
+            These .ini files may or may not have been previously fixed. A path to some .ini file in this attribute **DOES NOT** imply
+            that the .ini file previously had a fix
     """
 
     def __init__(self, path: Optional[str] = None, keepBackups: bool = True, fixOnly: bool = False, undoOnly: bool = False, 
                  readAllInis: bool = False, types: Optional[str] = None, defaultType: Optional[str] = None, log: Optional[str] = None, verbose: bool = True, handleExceptions: bool = False):
         self.log = log
         self._loggerBasePrefix = ""
         self.logger = Logger(logTxt = log, verbose = verbose)
@@ -4433,20 +4454,20 @@
         self.skippedMods: Dict[str, Exception] = {}
         self.blendsFixed: Set[str] = set()
         self.skippedBlendsByMods: DefaultDict[str, Dict[str, Exception]] = defaultdict(lambda: {})
         self.skippedBlends: Dict[str, Exception] = {}
         self.inisFixed = set()
         self.inisSkipped: Dict[str, Exception] = {}
         self.removedRemapBlends: Set[str] = set()
+        self.undoedInis: Set[str] = set()
         self._visitedRemapBlendsAtRemoval: Set[str] = set()
 
         self._setupModPath()
         self._setupModTypes()
         self._setupDefaultModType()
-        self._setupLogPath()
 
         if (self.__errorsBeforeFix is None):
             self._printModsToFix()
 
     @property
     def pathIsCwd(self):
         """
@@ -4472,28 +4493,54 @@
     
     @path.setter
     def path(self, newPath: Optional[str]):
         self._path = newPath
         self._setupModPath()
         self.clear()
 
-    def clear(self):
+    @property
+    def log(self) -> str:
+        """
+        The folder location to log the run of the fix into a seperate text file
+
+        :getter: Returns the file path to the log
+        :setter: Sets the path for the log
+        :type: :class:`str`
+        """
+
+        return self._log
+    
+    @log.setter
+    def log(self, newLog: Optional[str]):
+        self._log = newLog
+        self._setupLogPath()
+
+    def clear(self, clearLog: bool = True):
         """
         Clears up all the saved data
+
+        Paramters
+        ---------
+        clearLog: :class:`bool`
+            Whether to also clear out any saved data in the logger
         """
 
         self.modsFixed = 0
         self.skippedMods = {}
         self.blendsFixed = set()
         self.skippedBlendsByMods = defaultdict(lambda: {})
         self.skippedBlends = {}
         self.inisFixed = set()
         self.inisSkipped = {}
         self.removedRemapBlends = set()
+        self.undoedInis = set()
         self._visitedRemapBlendsAtRemoval = set()
+
+        if (clearLog):
+            self.logger.clear()
     
     def _setupModPath(self):
         """
         Sets the filepath of where the fix will run from
         """
 
         self._pathIsCwd = False
@@ -4507,16 +4554,16 @@
         self._pathIsCwd = (self._path == DefaultPath)
 
     def _setupLogPath(self):
         """
         Sets the folder path for where the log file will be stored
         """
 
-        if (self.log is not None):
-            self.log = FileService.parseOSPath(os.path.join(self.log, LogFile))
+        if (self._log is not None):
+            self._log = FileService.parseOSPath(os.path.join(self._log, LogFile))
 
     def _setupModTypes(self):
         """
         Sets the types of mods that will be fixed
         """
 
         if (isinstance(self.types, set)):
@@ -4623,26 +4670,26 @@
 
         if (iniFullPath in self.inisSkipped):
             self.logger.log(f"the ini file, {fileBaseName}, has alreaedy encountered an error")
             return False
         
         if (iniFullPath in self.inisFixed):
             self.logger.log(f"the ini file, {fileBaseName}, is already fixed")
-            return False
+            return True
 
         # parse the .ini file
         self.logger.log(f"Parsing {fileBaseName}...")
         ini.parse()
         if (ini.isFixed):
             self.logger.log(f"the ini file, {fileBaseName}, is already fixed")
-            return False
+            return True
 
         # fix the blends
         self.logger.log(f"Fixing the {BlendFileType} files for {fileBaseName}...")
-        currentBlendsFixed, currentBlendsSkipped = mod.correctBlend(fixedRemapBlends = fixedRemapBlends, skippedBlends = self.skippedBlends)
+        currentBlendsFixed, currentBlendsSkipped = mod.correctBlend(fixedRemapBlends = fixedRemapBlends, skippedBlends = self.skippedBlends, fixOnly = self.fixOnly)
         self.blendsFixed = self.blendsFixed.union(currentBlendsFixed)
 
         if (currentBlendsSkipped):
             self.skippedBlendsByMods[mod.path] = DictTools.combine(self.skippedBlendsByMods[mod.path], currentBlendsSkipped)
 
         # writing the fixed file
         self.logger.log(f"Making the fixed ini file for {fileBaseName}")
@@ -4682,14 +4729,15 @@
         for ini in mod.inis:
             ini.checkIsMod()
 
         # undo any previous fixes
         if (not self.fixOnly):
             undoedInis, removedRemapBlends = mod.removeFix(self.blendsFixed, self.inisFixed, self._visitedRemapBlendsAtRemoval, self.inisSkipped, keepBackups = self.keepBackups, fixOnly = self.fixOnly)
             self.removedRemapBlends = self.removedRemapBlends.union(removedRemapBlends)
+            self.undoedInis = self.undoedInis.union(undoedInis)
 
         result = False
         firstIniException = None
         inisLen = len(mod.inis)
 
         for i in range(inisLen):
             ini = mod.inis[i]
@@ -4819,62 +4867,73 @@
         fixedBlends = len(self.blendsFixed)
         skippedBlends = len(self.skippedBlends)
         foundBlends = fixedBlends + skippedBlends
         fixedInis = len(self.inisFixed)
         skippedInis = len(self.inisSkipped)
         foundInis = fixedInis + skippedInis
         removedRemapBlends = len(self.removedRemapBlends)
+        undoedInis = len(self.undoedInis)
 
         self.logger.openHeading("Summary", sideLen = 10)
         self.logger.space()
         
         modFixMsg = ""
         blendFixMsg = ""
         iniFixMsg = ""
         removedRemappedMsg = ""
+        undoedInisMsg = ""
         if (not self.undoOnly):
             modFixMsg = f"Out of {foundMods} found mods, fixed {self.modsFixed} mods and skipped {skippedMods} mods"
-            iniFixMsg = f"Out of the {foundInis} {IniFileType}s within the found mods, fixed {fixedInis} {IniFileType}s and skipped {skippedInis} {IniFileType} files"
+            iniFixMsg = f"Out of the {foundInis} {IniFileType}s within the found mods, fixed {fixedInis} {IniFileType}s and skipped {skippedInis} {IniFileType}s"
             blendFixMsg = f"Out of the {foundBlends} {BlendFileType} files within the found mods, fixed {fixedBlends} {BlendFileType} files and skipped {skippedBlends} {BlendFileType} files"
         else:
             modFixMsg = f"Out of {foundMods} found mods, remove fix from {self.modsFixed} mods and skipped {skippedMods} mods"
 
+        if (not self.fixOnly and undoedInis > 0):
+            undoedInisMsg = f"Removed fix from up to {undoedInis} {IniFileType}s"
+
+            if (self.undoOnly):
+                undoedInisMsg += f" and skipped {skippedInis} {IniFileType}s"
+
         if (not self.fixOnly and removedRemapBlends > 0):
             removedRemappedMsg = f"Removed {removedRemapBlends} old {RemapBlendFile} files"
 
 
         self.logger.bulletPoint(modFixMsg)
         if (iniFixMsg):
             self.logger.bulletPoint(iniFixMsg)
 
         if (blendFixMsg):
             self.logger.bulletPoint(blendFixMsg)
 
+        if (undoedInisMsg):
+            self.logger.bulletPoint(undoedInisMsg)
+
         if (removedRemappedMsg):
             self.logger.bulletPoint(removedRemappedMsg)
 
         self.logger.space()
         self.logger.closeHeading()
 
     def createLog(self):
         """
         Creates a log text file that contains all the text printed on the command line
         """
 
-        if (self.log is None):
+        if (self._log is None):
             return
 
         self.logger.includePrefix = False
         self.logger.space()
 
         self.logger.log(f"Creating log file, {LogFile}")
 
         self.logger.includePrefix = True
 
-        with open(self.log, "w", encoding = IniFileEncoding) as f:
+        with open(self._log, "w", encoding = IniFileEncoding) as f:
             f.write(self.logger.loggedTxt)
 
     def createMod(self, path: Optional[str] = None, files: Optional[List[str]] = None) -> Mod:
         """
         Creates a mod
 
         .. note::
```

### Comparing `fixraidenboss2-3.7.0/src/FixRaidenBoss2/__init__.py` & `fixraidenboss2-3.7.1/src/FixRaidenBoss2/__init__.py`

 * *Files identical despite different names*

### Comparing `fixraidenboss2-3.7.0/src/FixRaidenBoss2.egg-info/PKG-INFO` & `fixraidenboss2-3.7.1/src/FixRaidenBoss2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FixRaidenBoss2
-Version: 3.7.0
+Version: 3.7.1
 Summary: A script to fix Raiden Shogun Boss Phase 1 for all types of mods
 Author-email: nhok0169 <qqqqaaaapppp0000@gmail.com>, Albert Gold <AlexXianZhenYuAu@gmail.com>
 Project-URL: Homepage, https://github.com/nhok0169/Fix-Raiden-Boss
 Project-URL: Documentation, https://fix-raiden-boss.readthedocs.io/en/latest
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: FixRaidenBoss2 Version: 3.7.0 Summary: A script to
+Metadata-Version: 2.1 Name: FixRaidenBoss2 Version: 3.7.1 Summary: A script to
 fix Raiden Shogun Boss Phase 1 for all types of mods Author-email: nhok0169
 gmail.com>, Albert Gold
 gmail.com> Project-URL: Homepage, https://github.com/nhok0169/Fix-Raiden-Boss
 Project-URL: Documentation, https://fix-raiden-boss.readthedocs.io/en/latest
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
```

