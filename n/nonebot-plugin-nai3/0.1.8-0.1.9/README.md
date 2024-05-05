# Comparing `tmp/nonebot_plugin_nai3-0.1.8.tar.gz` & `tmp/nonebot_plugin_nai3-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nai3-0.1.8.tar", max compression
+gzip compressed data, was "nonebot_plugin_nai3-0.1.9.tar", max compression
```

## Comparing `nonebot_plugin_nai3-0.1.8.tar` & `nonebot_plugin_nai3-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1098 2024-04-13 00:11:40.913503 nonebot_plugin_nai3-0.1.8/LICENSE
--rw-r--r--   0        0        0    13202 2024-05-03 14:53:25.721129 nonebot_plugin_nai3-0.1.8/nonebot_plugin_nai3/__init__.py
--rw-r--r--   0        0        0      803 2024-05-02 12:22:13.415920 nonebot_plugin_nai3-0.1.8/nonebot_plugin_nai3/config.py
--rw-r--r--   0        0        0     2440 2024-04-14 23:34:30.728833 nonebot_plugin_nai3-0.1.8/nonebot_plugin_nai3/utils.py
--rw-r--r--   0        0        0     1071 2024-05-03 14:48:40.750023 nonebot_plugin_nai3-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     5363 2024-05-02 12:22:18.486293 nonebot_plugin_nai3-0.1.8/README.md
--rw-r--r--   0        0        0     5959 1970-01-01 00:00:00.000000 nonebot_plugin_nai3-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-13 00:11:40.913503 nonebot_plugin_nai3-0.1.9/LICENSE
+-rw-r--r--   0        0        0    13499 2024-05-03 15:48:43.074462 nonebot_plugin_nai3-0.1.9/nonebot_plugin_nai3/__init__.py
+-rw-r--r--   0        0        0      803 2024-05-02 12:22:13.415920 nonebot_plugin_nai3-0.1.9/nonebot_plugin_nai3/config.py
+-rw-r--r--   0        0        0     2440 2024-04-14 23:34:30.728833 nonebot_plugin_nai3-0.1.9/nonebot_plugin_nai3/utils.py
+-rw-r--r--   0        0        0     1071 2024-05-03 16:03:51.581632 nonebot_plugin_nai3-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     5363 2024-05-02 12:22:18.486293 nonebot_plugin_nai3-0.1.9/README.md
+-rw-r--r--   0        0        0     5959 1970-01-01 00:00:00.000000 nonebot_plugin_nai3-0.1.9/PKG-INFO
```

### Comparing `nonebot_plugin_nai3-0.1.8/LICENSE` & `nonebot_plugin_nai3-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.1.8/nonebot_plugin_nai3/__init__.py` & `nonebot_plugin_nai3-0.1.9/nonebot_plugin_nai3/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import io
 import os
 import random
 import shutil
 import time
 import zipfile
 from argparse import Namespace
+from datetime import date
 from importlib.metadata import version
 from pathlib import Path
 
 import ujson as json
 from httpx import AsyncClient
 from nonebot.adapters.onebot.v11 import (
     GROUP_ADMIN,
@@ -108,18 +109,22 @@
                 await nai3.finish("你在画图黑名单中!", at_sender=True)
     except FileNotFoundError:
         pass
 
     # 更新冷却时间和次数
     now_time = time.time()
     try:
-        cd[gid]["user"][uid]["limit"]
+        cd[gid]
     except KeyError:
         cd[gid] = {"cool_time": now_time - nai3_config.nai3_cooltime_group, "user": {}}
+    try:
+        cd[gid]["user"][uid]
+    except KeyError:
         cd[gid]["user"][uid] = {
+            "date": date.today(),
             "limit": 999 if event.get_user_id() in bot.config.superusers else nai3_config.nai3_limit,
             "cool_time": now_time - nai3_config.nai3_cooltime_user,
         }
 
     # 判断冷却时间并阻断
     if event.get_user_id() not in bot.config.superusers:
         logger.debug(event.get_user_id())
@@ -134,16 +139,19 @@
         if now_time - cd[gid]["user"][uid]["cool_time"] < nai3_config.nai3_cooltime_user:
             await nai3.finish(
                 "个人绘画冷却中, 剩余时间: {} 秒...".format(
                     round(nai3_config.nai3_cooltime_user - now_time + cd[gid]["cool_time"], 3)
                 ),
                 at_sender=True,
             )
-        if cd[gid]["user"][uid]["limit"] <= 0:
+        if (cd[gid]["user"][uid]["limit"] <= 0) and (cd[gid]["user"][uid]["date"] == date.today()):
             await nai3.finish("今天已经没次数了哦~", at_send=True)
+        else:
+            cd[gid]["user"][uid]["date"] == date.today()
+            cd[gid]["user"][uid]["limit"] == nai3_config.nai3_limit
 
     await nai3.send(
         "脑积水已收到绘画指令, 正在生成图片(剩余次数: {})...".format(cd[gid]["user"][uid]["limit"]), at_sender=True
     )
 
     # 组装 json 数据
     json_for_t2i["input"] = format_str(list_to_str(args.prompt))
```

### Comparing `nonebot_plugin_nai3-0.1.8/nonebot_plugin_nai3/config.py` & `nonebot_plugin_nai3-0.1.9/nonebot_plugin_nai3/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.1.8/nonebot_plugin_nai3/utils.py` & `nonebot_plugin_nai3-0.1.9/nonebot_plugin_nai3/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.1.8/pyproject.toml` & `nonebot_plugin_nai3-0.1.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-nai3"
-version = "0.1.8"
+version = "0.1.9"
 description = "通过 NovelAI 生成图片"
 authors = ["zhulinyv <zhulinyv2005@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_nai3"}]
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_plugin_nai3-0.1.8/README.md` & `nonebot_plugin_nai3-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.1.8/PKG-INFO` & `nonebot_plugin_nai3-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nai3
-Version: 0.1.8
+Version: 0.1.9
 Summary: 通过 NovelAI 生成图片
 License: MIT
 Author: zhulinyv
 Author-email: zhulinyv2005@outlook.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-nai3 Version: 0.1.8 Summary: éè¿
+Metadata-Version: 2.1 Name: nonebot-plugin-nai3 Version: 0.1.9 Summary: éè¿
 NovelAI çæå¾ç License: MIT Author: zhulinyv Author-email:
 zhulinyv2005@outlook.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.1,<0.25.0) Requires-Dist: nonebot-adapter-onebot
 (>=2.2.3,<3.0.0) Requires-Dist: nonebot-plugin-smms (>=0.1.0,<0.2.0) Requires-
```

