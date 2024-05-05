# Comparing `tmp/wxhook-0.0.1.tar.gz` & `tmp/wxhook-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wxhook-0.0.1.tar", last modified: Sat May  4 14:04:41 2024, max compression
+gzip compressed data, was "wxhook-0.0.2.tar", last modified: Sun May  5 02:59:56 2024, max compression
```

## Comparing `wxhook-0.0.1.tar` & `wxhook-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 14:04:41.307914 wxhook-0.0.1/
--rw-rw-rw-   0        0        0     1077 2024-05-02 11:25:01.000000 wxhook-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       51 2024-05-04 13:53:50.000000 wxhook-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     7193 2024-05-04 14:04:41.306925 wxhook-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6449 2024-05-04 14:04:05.000000 wxhook-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-04 14:04:41.307914 wxhook-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     3928 2024-05-04 13:12:46.000000 wxhook-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-04 14:04:41.291527 wxhook-0.0.1/wxhook/
--rw-rw-rw-   0        0        0       44 2024-05-03 14:24:48.000000 wxhook-0.0.1/wxhook/__init__.py
--rw-rw-rw-   0        0        0    16000 2024-05-04 13:29:41.000000 wxhook-0.0.1/wxhook/core.py
--rw-rw-rw-   0        0        0      630 2024-05-03 14:07:48.000000 wxhook-0.0.1/wxhook/events.py
--rw-rw-rw-   0        0        0      273 2024-05-04 13:12:46.000000 wxhook-0.0.1/wxhook/logger.py
--rw-rw-rw-   0        0        0     3826 2024-05-04 13:09:16.000000 wxhook-0.0.1/wxhook/model.py
-drwxrwxrwx   0        0        0        0 2024-05-04 14:04:41.303915 wxhook-0.0.1/wxhook/tools/
--rwxrwxrwx   0        0        0   270336 2024-05-01 02:42:10.000000 wxhook-0.0.1/wxhook/tools/faker.exe
--rwxrwxrwx   0        0        0   911872 2024-05-02 10:39:06.000000 wxhook-0.0.1/wxhook/tools/start-wechat.exe
--rw-rw-rw-   0        0        0   592384 2024-04-30 08:39:12.000000 wxhook-0.0.1/wxhook/tools/wxhook.dll
--rw-rw-rw-   0        0        0     3304 2024-05-04 13:12:46.000000 wxhook-0.0.1/wxhook/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-04 14:04:41.305914 wxhook-0.0.1/wxhook.egg-info/
--rw-rw-rw-   0        0        0     7193 2024-05-04 14:04:41.000000 wxhook-0.0.1/wxhook.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2024-05-04 14:04:41.000000 wxhook-0.0.1/wxhook.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 14:04:41.000000 wxhook-0.0.1/wxhook.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-04 14:04:41.000000 wxhook-0.0.1/wxhook.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-04 14:04:41.000000 wxhook-0.0.1/wxhook.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-05 02:59:56.320611 wxhook-0.0.2/
+-rw-rw-rw-   0        0        0     1077 2024-05-02 11:25:01.000000 wxhook-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       51 2024-05-04 13:53:50.000000 wxhook-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     7199 2024-05-05 02:59:56.319610 wxhook-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6455 2024-05-05 02:40:41.000000 wxhook-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-05 02:59:56.320611 wxhook-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     3928 2024-05-05 02:59:54.000000 wxhook-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 02:59:56.304133 wxhook-0.0.2/wxhook/
+-rw-rw-rw-   0        0        0       44 2024-05-05 02:59:54.000000 wxhook-0.0.2/wxhook/__init__.py
+-rw-rw-rw-   0        0        0    16091 2024-05-05 02:58:29.000000 wxhook-0.0.2/wxhook/core.py
+-rw-rw-rw-   0        0        0      630 2024-05-03 14:07:48.000000 wxhook-0.0.2/wxhook/events.py
+-rw-rw-rw-   0        0        0      273 2024-05-04 13:12:46.000000 wxhook-0.0.2/wxhook/logger.py
+-rw-rw-rw-   0        0        0     3826 2024-05-04 13:09:16.000000 wxhook-0.0.2/wxhook/model.py
+drwxrwxrwx   0        0        0        0 2024-05-05 02:59:56.317609 wxhook-0.0.2/wxhook/tools/
+-rw-rw-rw-   0        0        0       22 2024-05-05 02:55:57.000000 wxhook-0.0.2/wxhook/tools/config.ini
+-rwxrwxrwx   0        0        0   270336 2024-05-01 02:42:10.000000 wxhook-0.0.2/wxhook/tools/faker.exe
+-rwxrwxrwx   0        0        0   911872 2024-05-02 10:39:06.000000 wxhook-0.0.2/wxhook/tools/start-wechat.exe
+-rw-rw-rw-   0        0        0   592384 2024-04-30 08:39:12.000000 wxhook-0.0.2/wxhook/tools/wxhook.dll
+-rw-rw-rw-   0        0        0      103 2024-05-05 02:55:57.000000 wxhook-0.0.2/wxhook/tools/wxhook.json
+-rw-rw-rw-   0        0        0     3304 2024-05-04 13:12:46.000000 wxhook-0.0.2/wxhook/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-05 02:59:56.318609 wxhook-0.0.2/wxhook.egg-info/
+-rw-rw-rw-   0        0        0     7199 2024-05-05 02:59:56.000000 wxhook-0.0.2/wxhook.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-05-05 02:59:56.000000 wxhook-0.0.2/wxhook.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 02:59:56.000000 wxhook-0.0.2/wxhook.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-05 02:59:56.000000 wxhook-0.0.2/wxhook.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-05 02:59:56.000000 wxhook-0.0.2/wxhook.egg-info/top_level.txt
```

### Comparing `wxhook-0.0.1/LICENSE` & `wxhook-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.1/PKG-INFO` & `wxhook-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxhook
-Version: 0.0.1
+Version: 0.0.2
 Summary: wechat robot framework.
 Home-page: https://github.com/miloira/wxhook
 Author: Msky
 Author-email: 690126048@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -22,15 +22,15 @@
 Requires-Dist: xmltodict
 
 
 # WxHook
 
 ## 简介
 
-WxHook是一个基于dll注入实现的python微信机器人框架，支持多种接口、高扩展性、多线程事件高并发，让你轻松应对海量消息，为你的需求实现提供便捷灵活的支持。
+WxHook是一个基于dll注入实现的python微信机器人框架，支持多种接口、高扩展性、多线程消息处理，让你轻松应对海量消息，为你的需求实现提供便捷灵活的支持。
 
 支持的接口
 1. hook同步消息
 2. 取消hook同步消息
 3. hook日志
 4. 取消hook日志
 5. 检查登录状态
@@ -79,15 +79,15 @@
 ```
 
 ## 使用示例
 
 消息事件处理例子
 ```python
 # import os
-# os.environ["PYWX_LOG_LEVEL"] = "INFO" # 修改日志输出级别
+# os.environ["WXHOOK_LOG_LEVEL"] = "INFO" # 修改日志输出级别
 import time
 
 from wxhook import Bot
 from wxhook import events
 from wxhook.model import Event
 
 
@@ -111,15 +111,15 @@
 )
 
 
 # 消息回调地址
 # bot.set_webhook_url("http://127.0.0.1:8000")
 
 @bot.handle(events.TEXT_MESSAGE, once=True)
-def on_message(bot: Bot, event):
+def on_message(bot: Bot, event: Event):
     bot.send_text("filehelper", "这条消息只会发送一次哦")
 
 
 @bot.handle(events.TEXT_MESSAGE)
 def on_message(bot: Bot, event: Event):
     if event.fromUser != bot.info.wxid:
         bot.send_text(event.fromUser, event.content)
@@ -212,8 +212,8 @@
             bot.collect_image(sender, os.path.abspath("test.png"))
         elif content.find("ocr") != -1:
             print(bot.ocr(os.path.abspath("test.png")))
 
 bot.run()
 ```
 
-QQ交流群:625920215
+QQ交流群:625920216
```

### Comparing `wxhook-0.0.1/README.md` & `wxhook-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # WxHook
 
 ## 简介
 
-WxHook是一个基于dll注入实现的python微信机器人框架，支持多种接口、高扩展性、多线程事件高并发，让你轻松应对海量消息，为你的需求实现提供便捷灵活的支持。
+WxHook是一个基于dll注入实现的python微信机器人框架，支持多种接口、高扩展性、多线程消息处理，让你轻松应对海量消息，为你的需求实现提供便捷灵活的支持。
 
 支持的接口
 1. hook同步消息
 2. 取消hook同步消息
 3. hook日志
 4. 取消hook日志
 5. 检查登录状态
@@ -55,15 +55,15 @@
 ```
 
 ## 使用示例
 
 消息事件处理例子
 ```python
 # import os
-# os.environ["PYWX_LOG_LEVEL"] = "INFO" # 修改日志输出级别
+# os.environ["WXHOOK_LOG_LEVEL"] = "INFO" # 修改日志输出级别
 import time
 
 from wxhook import Bot
 from wxhook import events
 from wxhook.model import Event
 
 
@@ -87,15 +87,15 @@
 )
 
 
 # 消息回调地址
 # bot.set_webhook_url("http://127.0.0.1:8000")
 
 @bot.handle(events.TEXT_MESSAGE, once=True)
-def on_message(bot: Bot, event):
+def on_message(bot: Bot, event: Event):
     bot.send_text("filehelper", "这条消息只会发送一次哦")
 
 
 @bot.handle(events.TEXT_MESSAGE)
 def on_message(bot: Bot, event: Event):
     if event.fromUser != bot.info.wxid:
         bot.send_text(event.fromUser, event.content)
@@ -188,8 +188,8 @@
             bot.collect_image(sender, os.path.abspath("test.png"))
         elif content.find("ocr") != -1:
             print(bot.ocr(os.path.abspath("test.png")))
 
 bot.run()
 ```
 
-QQ交流群:625920215
+QQ交流群:625920216
```

### Comparing `wxhook-0.0.1/setup.py` & `wxhook-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'wxhook'
 DESCRIPTION = 'wechat robot framework.'
 URL = 'https://github.com/miloira/wxhook'
 EMAIL = '690126048@qq.com'
 AUTHOR = 'Msky'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'loguru',
     'psutil',
     'pyee',
     'requests',
```

### Comparing `wxhook-0.0.1/wxhook/core.py` & `wxhook-0.0.2/wxhook/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import json
 import typing
-
-import psutil
-import pyee
 import traceback
 import socketserver
+from functools import lru_cache
 
+import psutil
+import pyee
 import requests
 
 from .events import ALL_MESSAGE, SYSTEM_MESSAGE
 from .logger import logger
 from .model import RawData, Event, Account, Contact, ContactDetail, Room, RoomMembers, Table, DB, Response
 from .utils import WeChatManager, start_wechat_with_inject, fake_wechat_version, parse_event
 
@@ -58,16 +58,16 @@
         self.on_stop = on_stop
         self.faked_version = faked_version
         self.event_emitter = pyee.EventEmitter()
         self.wechat_manager = WeChatManager()
         self.remote_port, self.server_port = self.wechat_manager.get_port()
         self.BASE_URL = f"http://{self.remote_host}:{self.remote_port}"
         self.webhook_url = None
-        self.info = None
         self.DATA_SAVE_PATH = None
+        self.WXHELPER_PATH = None
         self.FILE_SAVE_PATH = None
         self.IMAGE_SAVE_PATH = None
         self.VIDEO_SAVE_PATH = None
 
         code, output = start_wechat_with_inject(self.remote_port)
         if code == 1:
             raise Exception(output)
@@ -89,20 +89,19 @@
     @staticmethod
     def call_hook_func(func: typing.Callable, *args, **kwargs) -> typing.Any:
         if callable(func):
             return func(*args, **kwargs)
 
     def init_bot(self, bot: "Bot", event: Event) -> None:
         if event.content["sysmsg"]["@type"] == "SafeModuleCfg":
-            bot.info = bot.get_self_info()
             self.DATA_SAVE_PATH = bot.info.dataSavePath
-            self.FILE_SAVE_PATH = os.path.join(self.DATA_SAVE_PATH, "wxhelper/file")
-            self.IMAGE_SAVE_PATH = os.path.join(self.DATA_SAVE_PATH, "wxhelper/image")
-            self.VIDEO_SAVE_PATH = os.path.join(self.DATA_SAVE_PATH, "wxhelper/video")
-            logger.info(bot.info)
+            self.WXHELPER_PATH = os.path.join(self.DATA_SAVE_PATH, "wxhelper")
+            self.FILE_SAVE_PATH = os.path.join(self.WXHELPER_PATH, "file")
+            self.IMAGE_SAVE_PATH = os.path.join(self.WXHELPER_PATH, "image")
+            self.VIDEO_SAVE_PATH = os.path.join(self.WXHELPER_PATH, "video")
             self.call_hook_func(self.on_login, bot)
 
     def set_webhook_url(self, webhook_url: str) -> None:
         self.webhook_url = webhook_url
 
     def webhook(self, event: dict) -> None:
         if self.webhook_url is not None:
@@ -111,20 +110,20 @@
             except Exception:
                 pass
 
     def call_api(self, api: str, *args, **kwargs) -> dict:
         return requests.request("POST", self.BASE_URL + api, *args, **kwargs).json()
 
     def hook_sync_msg(
-            self,
-            ip: str,
-            port: int,
-            enable_http: int = 0,
-            url: str = "http://127.0.0.1:8000",
-            timeout: int = 30
+        self,
+        ip: str,
+        port: int,
+        enable_http: int = 0,
+        url: str = "http://127.0.0.1:8000",
+        timeout: int = 30
     ) -> Response:
         """hook同步消息"""
         data = {
             "port": port,
             "ip": ip,
             "enableHttp": enable_http,
             "url": url,
@@ -144,14 +143,15 @@
         """取消hook日志"""
         return Response(**self.call_api("/api/unhookLog"))
 
     def check_login(self) -> Response:
         """检查登录状态"""
         return Response(**self.call_api("/api/checkLogin"))
 
+    @lru_cache
     def get_self_info(self) -> Account:
         """获取用户信息"""
         return Account(**self.call_api("/api/userInfo")["data"])
 
     def send_text(self, wxid: str, msg: str) -> Response:
         """发送文本消息"""
         data = {
@@ -230,15 +230,15 @@
         return [Contact(**item) for item in self.call_api("/api/getContactList")["data"]]
 
     def get_contact(self, wxid: str) -> ContactDetail:
         """获取联系人详情"""
         data = {
             "wxid": wxid
         }
-        return ContactDetail(self.call_api("/api/getContactProfile", json=data)["data"])
+        return ContactDetail(**self.call_api("/api/getContactProfile", json=data)["data"])
 
     def create_room(self, member_ids: list[str]) -> Response:
         """创建群聊"""
         data = {
             "memberIds": ",".join(member_ids)
         }
         return Response(**self.call_api("/api/createChatRoom", json=data))
@@ -419,14 +419,18 @@
         }
         return Response(**self.call_api("/api/execSql", json=data))
 
     def test(self) -> Response:
         """测试"""
         return Response(**self.call_api("/api/test"))
 
+    @property
+    def info(self) -> Account:
+        return self.get_self_info()
+
     def on_event(self, raw_data: bytes):
         try:
             data = json.loads(raw_data)
             event = Event(**parse_event(data), rawData=RawData(raw_data))
             logger.debug(event)
             self.call_hook_func(self.on_before_message, self, event)
             self.event_emitter.emit(str(ALL_MESSAGE), self, event)
```

### Comparing `wxhook-0.0.1/wxhook/events.py` & `wxhook-0.0.2/wxhook/events.py`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.1/wxhook/model.py` & `wxhook-0.0.2/wxhook/model.py`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.1/wxhook/tools/faker.exe` & `wxhook-0.0.2/wxhook/tools/faker.exe`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.1/wxhook/tools/start-wechat.exe` & `wxhook-0.0.2/wxhook/tools/start-wechat.exe`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.1/wxhook/tools/wxhook.dll` & `wxhook-0.0.2/wxhook/tools/wxhook.dll`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.1/wxhook/utils.py` & `wxhook-0.0.2/wxhook/utils.py`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.1/wxhook.egg-info/PKG-INFO` & `wxhook-0.0.2/wxhook.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxhook
-Version: 0.0.1
+Version: 0.0.2
 Summary: wechat robot framework.
 Home-page: https://github.com/miloira/wxhook
 Author: Msky
 Author-email: 690126048@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -22,15 +22,15 @@
 Requires-Dist: xmltodict
 
 
 # WxHook
 
 ## 简介
 
-WxHook是一个基于dll注入实现的python微信机器人框架，支持多种接口、高扩展性、多线程事件高并发，让你轻松应对海量消息，为你的需求实现提供便捷灵活的支持。
+WxHook是一个基于dll注入实现的python微信机器人框架，支持多种接口、高扩展性、多线程消息处理，让你轻松应对海量消息，为你的需求实现提供便捷灵活的支持。
 
 支持的接口
 1. hook同步消息
 2. 取消hook同步消息
 3. hook日志
 4. 取消hook日志
 5. 检查登录状态
@@ -79,15 +79,15 @@
 ```
 
 ## 使用示例
 
 消息事件处理例子
 ```python
 # import os
-# os.environ["PYWX_LOG_LEVEL"] = "INFO" # 修改日志输出级别
+# os.environ["WXHOOK_LOG_LEVEL"] = "INFO" # 修改日志输出级别
 import time
 
 from wxhook import Bot
 from wxhook import events
 from wxhook.model import Event
 
 
@@ -111,15 +111,15 @@
 )
 
 
 # 消息回调地址
 # bot.set_webhook_url("http://127.0.0.1:8000")
 
 @bot.handle(events.TEXT_MESSAGE, once=True)
-def on_message(bot: Bot, event):
+def on_message(bot: Bot, event: Event):
     bot.send_text("filehelper", "这条消息只会发送一次哦")
 
 
 @bot.handle(events.TEXT_MESSAGE)
 def on_message(bot: Bot, event: Event):
     if event.fromUser != bot.info.wxid:
         bot.send_text(event.fromUser, event.content)
@@ -212,8 +212,8 @@
             bot.collect_image(sender, os.path.abspath("test.png"))
         elif content.find("ocr") != -1:
             print(bot.ocr(os.path.abspath("test.png")))
 
 bot.run()
 ```
 
-QQ交流群:625920215
+QQ交流群:625920216
```

