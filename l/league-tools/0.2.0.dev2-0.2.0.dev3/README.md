# Comparing `tmp/league_tools-0.2.0.dev2.tar.gz` & `tmp/league_tools-0.2.0.dev3.tar.gz`

## Comparing `league_tools-0.2.0.dev2.tar` & `league_tools-0.2.0.dev3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    17209 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/1.json
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/requirements-dev.lock
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/requirements.lock
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/requirements.txt
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/__init__.py
--rw-r--r--   0        0        0     3764 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/base.py
--rw-r--r--   0        0        0    12808 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/index.py
--rw-r--r--   0        0        0     6162 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/formats/BIN.py
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/formats/BNK.py
--rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/formats/WAD.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/formats/WPK.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/formats/__init__.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/formats/section/BKHD.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/formats/section/DATA.py
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/formats/section/DIDX.py
--rw-r--r--   0        0        0    15754 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/formats/section/HIRC.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/formats/section/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/tools/__init__.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/tools/Binary/__init__.py
--rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/tools/Binary/reader.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/utils/__init__.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/league_tools/utils/type_hints.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/LICENSE
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/README.md
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/pyproject.toml
--rw-r--r--   0        0        0    44987 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev2/PKG-INFO
+-rw-r--r--   0        0        0    17209 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev3/1.json
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev3/requirements-dev.lock
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev3/requirements.lock
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev3/requirements.txt
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev3/league_tools/__init__.py
+-rw-r--r--   0        0        0     3764 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev3/league_tools/base.py
+-rw-r--r--   0        0        0    12781 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev3/league_tools/index.py
+-rw-r--r--   0        0        0     6162 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev3/league_tools/formats/BIN.py
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev3/league_tools/formats/BNK.py
+-rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev3/league_tools/formats/WAD.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev3/league_tools/formats/WPK.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev3/league_tools/formats/__init__.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev3/league_tools/formats/section/BKHD.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev3/league_tools/formats/section/DATA.py
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev3/league_tools/formats/section/DIDX.py
+-rw-r--r--   0        0        0    15754 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev3/league_tools/formats/section/HIRC.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev3/league_tools/formats/section/__init__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev3/league_tools/tools/__init__.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev3/league_tools/tools/Binary/__init__.py
+-rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev3/league_tools/tools/Binary/reader.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev3/league_tools/utils/__init__.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev3/league_tools/utils/type_hints.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev3/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev3/LICENSE
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev3/README.md
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev3/pyproject.toml
+-rw-r--r--   0        0        0    44987 2020-02-02 00:00:00.000000 league_tools-0.2.0.dev3/PKG-INFO
```

### Comparing `league_tools-0.2.0.dev2/1.json` & `league_tools-0.2.0.dev3/1.json`

 * *Files identical despite different names*

### Comparing `league_tools-0.2.0.dev2/league_tools/base.py` & `league_tools-0.2.0.dev3/league_tools/base.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.2.0.dev2/league_tools/index.py` & `league_tools-0.2.0.dev3/league_tools/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # -*- coding: utf-8 -*-
 # @Author  : Virace
 # @Email   : Virace@aliyun.com
 # @Site    : x-item.com
 # @Software: PyCharm
 # @Create  : 2021/2/27 18:28
-# @Update  : 2024/5/5 5:35
+# @Update  : 2024/5/5 23:26
 # @Detail  : 
 
 # References : http://wiki.xentax.com/index.php/Wwise_SoundBank_(*.bnk)#HIRC_section
 
-import logging
 from collections import OrderedDict, defaultdict
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from pathlib import Path
-from typing import List, Optional, Union, get_args
+from typing import List, Optional, Union
 
 from loguru import logger
 
 from league_tools.base import WemFile
 from league_tools.formats.BIN import BIN, StringHash
 from league_tools.formats.BNK import BNK, HIRC
 from league_tools.formats.WPK import WPK
@@ -321,15 +320,15 @@
     no_event = list(set(file_ids).difference(set(event_ids)))
     no_event_files = [file for file in audio_files if file.id in no_event]
 
     for file in no_event_files:
         name = file.filename or f'{file.id}.wem'
         if ext:
             name = Path(name).stem + '.' + ext
-        logging.debug(f'No Event, File: {file.id}')
+        logger.debug(f'No Event, File: {file.id}')
         file.save_file(Path(out_dir).joinpath(name), wem, vgmstream_cli=vgmstream_cli)
 
     # 去重
     temp = {}
     for eh in event_hashes:
         for file in audio_files:
             if eh.hash == file.id:
@@ -338,15 +337,15 @@
                     name = f'{Path(name).stem}.{ext}'
 
                 _dir = Path(out_dir).joinpath(eh.string)
                 _dir.mkdir(parents=True, exist_ok=True)
 
                 if file.id not in temp:
                     temp.update({file.id: _dir.joinpath(name)})
-                    logging.debug(f'Event: {eh.string}, File: {name}')
+                    logger.debug(f'Event: {eh.string}, File: {name}')
                     file.save_file(_dir.joinpath(name), wem, vgmstream_cli=vgmstream_cli)
 
                 else:
                     # 创建链接
                     try:
                         temp[file.id].symlink_to(_dir.joinpath(name))
                     except FileExistsError:
```

### Comparing `league_tools-0.2.0.dev2/league_tools/formats/BIN.py` & `league_tools-0.2.0.dev3/league_tools/formats/BIN.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.2.0.dev2/league_tools/formats/BNK.py` & `league_tools-0.2.0.dev3/league_tools/formats/BNK.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.2.0.dev2/league_tools/formats/WAD.py` & `league_tools-0.2.0.dev3/league_tools/formats/WAD.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.2.0.dev2/league_tools/formats/WPK.py` & `league_tools-0.2.0.dev3/league_tools/formats/WPK.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.2.0.dev2/league_tools/formats/section/BKHD.py` & `league_tools-0.2.0.dev3/league_tools/formats/section/BKHD.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.2.0.dev2/league_tools/formats/section/DATA.py` & `league_tools-0.2.0.dev3/league_tools/formats/section/DATA.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.2.0.dev2/league_tools/formats/section/DIDX.py` & `league_tools-0.2.0.dev3/league_tools/formats/section/DIDX.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.2.0.dev2/league_tools/formats/section/HIRC.py` & `league_tools-0.2.0.dev3/league_tools/formats/section/HIRC.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.2.0.dev2/league_tools/tools/Binary/reader.py` & `league_tools-0.2.0.dev3/league_tools/tools/Binary/reader.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.2.0.dev2/.gitignore` & `league_tools-0.2.0.dev3/.gitignore`

 * *Files identical despite different names*

### Comparing `league_tools-0.2.0.dev2/LICENSE` & `league_tools-0.2.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `league_tools-0.2.0.dev2/README.md` & `league_tools-0.2.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `league_tools-0.2.0.dev2/pyproject.toml` & `league_tools-0.2.0.dev3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "league-tools"
-version = "0.2.0dev2"
+version = "0.2.0dev3"
 description = "WAD、BIN、BNK、WPK文件简单处理"
 authors = [{ name = "Virace", email = "Virace@aliyun.com" }]
 keywords = ["league", "wad", "bnk"]
 dependencies = [
     "xxhash>=3.4.1",
     "loguru>=0.7.2",
     "zstd>=1.5.5.1",
```

### Comparing `league_tools-0.2.0.dev2/PKG-INFO` & `league_tools-0.2.0.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: league-tools
-Version: 0.2.0.dev2
+Version: 0.2.0.dev3
 Summary: WAD、BIN、BNK、WPK文件简单处理
 Project-URL: homepage, https://github.com/Virace/py-bnk-extract
 Project-URL: repository, https://github.com/Virace/py-bnk-extract
 Project-URL: Bug Tracker, https://github.com/Virace/py-bnk-extract/issues
 Author-email: Virace <Virace@aliyun.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

