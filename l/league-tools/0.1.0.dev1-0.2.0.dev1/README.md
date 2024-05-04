# Comparing `tmp/league_tools-0.1.0.dev1.tar.gz` & `tmp/league_tools-0.2.0.dev1.tar.gz`

## Comparing `league_tools-0.1.0.dev1.tar` & `league_tools-0.2.0.dev1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    17209 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/1.json
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/requirements-dev.lock
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/requirements.lock
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/requirements.txt
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/__init__.py
--rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/base.py
--rw-r--r--   0        0        0    12734 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/index.py
--rw-r--r--   0        0        0     6162 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/formats/BIN.py
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/formats/BNK.py
--rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/formats/WAD.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/formats/WPK.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/formats/__init__.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/formats/section/BKHD.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/formats/section/DATA.py
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/formats/section/DIDX.py
--rw-r--r--   0        0        0    15754 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/formats/section/HIRC.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/formats/section/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/tools/__init__.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/tools/Binary/__init__.py
--rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/tools/Binary/reader.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/utils/__init__.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/utils/type_hints.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/LICENSE
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/README.md
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/pyproject.toml
--rw-r--r--   0        0        0    44987 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0    17209 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/1.json
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/requirements-dev.lock
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/requirements.lock
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/requirements.txt
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/__init__.py
+-rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/base.py
+-rw-r--r--   0        0        0    12808 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/index.py
+-rw-r--r--   0        0        0     6162 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/formats/BIN.py
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/formats/BNK.py
+-rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/formats/WAD.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/formats/WPK.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/formats/__init__.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/formats/section/BKHD.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/formats/section/DATA.py
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/formats/section/DIDX.py
+-rw-r--r--   0        0        0    15754 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/formats/section/HIRC.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/formats/section/__init__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/tools/__init__.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/tools/Binary/__init__.py
+-rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/tools/Binary/reader.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/utils/__init__.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/league_tools/utils/type_hints.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/LICENSE
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/README.md
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0    44987 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev1/PKG-INFO
```

### Comparing `league_tools-0.1.0.dev1/1.json` & `league_tools-0.2.0.dev1/1.json`

 * *Files identical despite different names*

### Comparing `league_tools-0.1.0.dev1/league_tools/base.py` & `league_tools-0.2.0.dev1/league_tools/base.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.1.0.dev1/league_tools/index.py` & `league_tools-0.2.0.dev1/league_tools/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # -*- coding: utf-8 -*-
 # @Author  : Virace
 # @Email   : Virace@aliyun.com
 # @Site    : x-item.com
 # @Software: PyCharm
 # @Create  : 2021/2/27 18:28
-# @Update  : 2024/5/5 2:43
+# @Update  : 2024/5/5 5:35
 # @Detail  : 
 
 # References : http://wiki.xentax.com/index.php/Wwise_SoundBank_(*.bnk)#HIRC_section
 
 import logging
 from collections import OrderedDict, defaultdict
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from pathlib import Path
-from typing import List, Optional, Union
+from typing import List, Optional, Union, get_args
 
 from loguru import logger
 
 from league_tools.base import WemFile
 from league_tools.formats.BIN import BIN, StringHash
 from league_tools.formats.BNK import BNK, HIRC
 from league_tools.formats.WPK import WPK
@@ -165,15 +165,15 @@
     提供音频文件, 返回文件列表
     :param audio_file: 音频文件(bnk、wpk)
     :param get_data: 是否获取音频文件数据
     :param hash_table: 哈希表
     :return:
     """
 
-    if isinstance(audio_file, StrPath):
+    if isinstance(audio_file, str) or hasattr(audio_file, "__fspath__"):
         audio_ext = Path(audio_file).suffix
     elif isinstance(audio_file, bytes):
         br = BinaryReader(audio_file)
         head = br.customize('<4s')
         audio_ext = '.wpk' if head == b'r3d2' else '.bnk'
     else:
         return []
@@ -209,15 +209,15 @@
 def get_event_hashtable(bin_file: Union[StrPath, List[StringHash]], event_file):
     """
     根据皮肤bin文件以及音频事件, 提取事件哈希表
     :param bin_file: bin文件
     :param event_file: bnk event文件
     :return:
     """
-    if isinstance(bin_file, StrPath):
+    if isinstance(bin_file, str) or hasattr(bin_file, "__fspath__"):
         b1 = BIN(bin_file)
         # 获取事件哈希表
         read_strings = b1.hash_tables.copy()
     else:
         read_strings = bin_file.copy()
     # 解析事件文件
     event = BNK(event_file)
```

### Comparing `league_tools-0.1.0.dev1/league_tools/formats/BIN.py` & `league_tools-0.2.0.dev1/league_tools/formats/BIN.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.1.0.dev1/league_tools/formats/BNK.py` & `league_tools-0.2.0.dev1/league_tools/formats/BNK.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.1.0.dev1/league_tools/formats/WAD.py` & `league_tools-0.2.0.dev1/league_tools/formats/WAD.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.1.0.dev1/league_tools/formats/WPK.py` & `league_tools-0.2.0.dev1/league_tools/formats/WPK.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.1.0.dev1/league_tools/formats/section/BKHD.py` & `league_tools-0.2.0.dev1/league_tools/formats/section/BKHD.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.1.0.dev1/league_tools/formats/section/DATA.py` & `league_tools-0.2.0.dev1/league_tools/formats/section/DATA.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.1.0.dev1/league_tools/formats/section/DIDX.py` & `league_tools-0.2.0.dev1/league_tools/formats/section/DIDX.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.1.0.dev1/league_tools/formats/section/HIRC.py` & `league_tools-0.2.0.dev1/league_tools/formats/section/HIRC.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.1.0.dev1/league_tools/tools/Binary/reader.py` & `league_tools-0.2.0.dev1/league_tools/tools/Binary/reader.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.1.0.dev1/.gitignore` & `league_tools-0.2.0.dev1/.gitignore`

 * *Files identical despite different names*

### Comparing `league_tools-0.1.0.dev1/LICENSE` & `league_tools-0.2.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `league_tools-0.1.0.dev1/README.md` & `league_tools-0.2.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `league_tools-0.1.0.dev1/pyproject.toml` & `league_tools-0.2.0.dev1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "league-tools"
-version = "0.1.0dev1"
+version = "0.2.0dev1"
 description = "WAD、BIN、BNK、WPK文件简单处理"
 authors = [{ name = "Virace", email = "Virace@aliyun.com" }]
 keywords = ["league", "wad", "bnk"]
 dependencies = [
     "xxhash>=3.4.1",
     "loguru>=0.7.2",
     "zstd>=1.5.5.1",
```

### Comparing `league_tools-0.1.0.dev1/PKG-INFO` & `league_tools-0.2.0.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: league-tools
-Version: 0.1.0.dev1
+Version: 0.2.0.dev1
 Summary: WAD、BIN、BNK、WPK文件简单处理
 Project-URL: homepage, https://github.com/Virace/py-bnk-extract
 Project-URL: repository, https://github.com/Virace/py-bnk-extract
 Project-URL: Bug Tracker, https://github.com/Virace/py-bnk-extract/issues
 Author-email: Virace <Virace@aliyun.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

