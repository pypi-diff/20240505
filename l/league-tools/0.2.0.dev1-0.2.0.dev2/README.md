# Comparing `tmp/league_tools-0.2.0.dev1.tar.gz` & `tmp/league_tools-0.2.0.dev2.tar.gz`

## Comparing `league_tools-0.2.0.dev1.tar` & `league_tools-0.2.0.dev2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    17209 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/1.json
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/requirements-dev.lock
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/requirements.lock
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/requirements.txt
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/__init__.py
--rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/base.py
--rw-r--r--   0        0        0    12808 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/index.py
--rw-r--r--   0        0        0     6162 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/formats/BIN.py
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/formats/BNK.py
--rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/formats/WAD.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/formats/WPK.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/formats/__init__.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/formats/section/BKHD.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/formats/section/DATA.py
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/formats/section/DIDX.py
--rw-r--r--   0        0        0    15754 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/formats/section/HIRC.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/formats/section/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/tools/__init__.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/tools/Binary/__init__.py
--rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/tools/Binary/reader.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/utils/__init__.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/utils/type_hints.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/LICENSE
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/README.md
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/pyproject.toml
--rw-r--r--   0        0        0    44987 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0    17209 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/1.json
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/requirements-dev.lock
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/requirements.lock
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/requirements.txt
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/__init__.py
+-rw-r--r--   0        0        0     3764 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/base.py
+-rw-r--r--   0        0        0    12808 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/index.py
+-rw-r--r--   0        0        0     6162 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/formats/BIN.py
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/formats/BNK.py
+-rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/formats/WAD.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/formats/WPK.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/formats/__init__.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/formats/section/BKHD.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/formats/section/DATA.py
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/formats/section/DIDX.py
+-rw-r--r--   0        0        0    15754 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/formats/section/HIRC.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/formats/section/__init__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/tools/__init__.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/tools/Binary/__init__.py
+-rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/tools/Binary/reader.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/utils/__init__.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/utils/type_hints.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/LICENSE
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/README.md
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/pyproject.toml
+-rw-r--r--   0        0        0    44987 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/PKG-INFO
```

### Comparing `league_tools-0.2.0.dev1/1.json` & `league_tools-0.2.0.dev2/1.json`

 * *Files identical despite different names*

### Comparing `league_tools-0.2.0.dev1/league_tools/base.py` & `league_tools-0.2.0.dev2/league_tools/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # @Author  : Virace
 # @Email   : Virace@aliyun.com
 # @Site    : x-item.com
 # @Software: PyCharm
 # @Create  : 2021/2/27 19:36
-# @Update  : 2024/5/5 2:16
+# @Update  : 2024/5/5 7:07
 # @Detail  : 块 基类
 
 import os
 import subprocess
 from dataclasses import dataclass
 from io import BytesIO
 from pathlib import Path
@@ -118,15 +118,15 @@
                 str(wem_path),
                 '-o',
                 str(path)
             ],
                 stdout=subprocess.DEVNULL,
                 timeout=999999999
             )
-            if not wem:
+            if not wem and wem_path.exists():
                 wem_path.unlink()
         del data
 
     def __iter__(self):
         return [self.id, self.offset, self.length]
 
     def __dict__(self):
```

### Comparing `league_tools-0.2.0.dev1/league_tools/index.py` & `league_tools-0.2.0.dev2/league_tools/index.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.2.0.dev1/league_tools/formats/BIN.py` & `league_tools-0.2.0.dev2/league_tools/formats/BIN.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.2.0.dev1/league_tools/formats/BNK.py` & `league_tools-0.2.0.dev2/league_tools/formats/BNK.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.2.0.dev1/league_tools/formats/WAD.py` & `league_tools-0.2.0.dev2/league_tools/formats/WAD.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.2.0.dev1/league_tools/formats/WPK.py` & `league_tools-0.2.0.dev2/league_tools/formats/WPK.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.2.0.dev1/league_tools/formats/section/BKHD.py` & `league_tools-0.2.0.dev2/league_tools/formats/section/BKHD.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.2.0.dev1/league_tools/formats/section/DATA.py` & `league_tools-0.2.0.dev2/league_tools/formats/section/DATA.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.2.0.dev1/league_tools/formats/section/DIDX.py` & `league_tools-0.2.0.dev2/league_tools/formats/section/DIDX.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.2.0.dev1/league_tools/formats/section/HIRC.py` & `league_tools-0.2.0.dev2/league_tools/formats/section/HIRC.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.2.0.dev1/league_tools/tools/Binary/reader.py` & `league_tools-0.2.0.dev2/league_tools/tools/Binary/reader.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.2.0.dev1/.gitignore` & `league_tools-0.2.0.dev2/.gitignore`

 * *Files identical despite different names*

### Comparing `league_tools-0.2.0.dev1/LICENSE` & `league_tools-0.2.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `league_tools-0.2.0.dev1/README.md` & `league_tools-0.2.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `league_tools-0.2.0.dev1/pyproject.toml` & `league_tools-0.2.0.dev2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "league-tools"
-version = "0.2.0dev1"
+version = "0.2.0dev2"
 description = "WAD、BIN、BNK、WPK文件简单处理"
 authors = [{ name = "Virace", email = "Virace@aliyun.com" }]
 keywords = ["league", "wad", "bnk"]
 dependencies = [
     "xxhash>=3.4.1",
     "loguru>=0.7.2",
     "zstd>=1.5.5.1",
```

### Comparing `league_tools-0.2.0.dev1/PKG-INFO` & `league_tools-0.2.0.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: league-tools
-Version: 0.2.0.dev1
+Version: 0.2.0.dev2
 Summary: WAD、BIN、BNK、WPK文件简单处理
 Project-URL: homepage, https://github.com/Virace/py-bnk-extract
 Project-URL: repository, https://github.com/Virace/py-bnk-extract
 Project-URL: Bug Tracker, https://github.com/Virace/py-bnk-extract/issues
 Author-email: Virace <Virace@aliyun.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

