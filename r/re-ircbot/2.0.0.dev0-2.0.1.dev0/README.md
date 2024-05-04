# Comparing `tmp/re_ircbot-2.0.0.dev0.tar.gz` & `tmp/re_ircbot-2.0.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "re_ircbot-2.0.0.dev0.tar", last modified: Sat May  4 15:04:21 2024, max compression
+gzip compressed data, was "re_ircbot-2.0.1.dev0.tar", last modified: Sat May  4 22:47:52 2024, max compression
```

## Comparing `re_ircbot-2.0.0.dev0.tar` & `re_ircbot-2.0.1.dev0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-04 15:04:21.306030 re_ircbot-2.0.0.dev0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1072 2024-05-04 15:04:13.000000 re_ircbot-2.0.0.dev0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14058 2024-05-04 15:04:21.306030 re_ircbot-2.0.0.dev0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13331 2024-05-04 15:04:13.000000 re_ircbot-2.0.0.dev0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-04 15:04:21.306030 re_ircbot-2.0.0.dev0/ircbot/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      125 2024-05-04 15:04:13.000000 re_ircbot-2.0.0.dev0/ircbot/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    54469 2024-05-04 15:04:13.000000 re_ircbot-2.0.0.dev0/ircbot/client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5384 2024-05-04 15:04:13.000000 re_ircbot-2.0.0.dev0/ircbot/dcc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1658 2024-05-04 15:04:13.000000 re_ircbot-2.0.0.dev0/ircbot/message.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1972 2024-05-04 15:04:13.000000 re_ircbot-2.0.0.dev0/ircbot/shortest_prefix.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11380 2024-05-04 15:04:13.000000 re_ircbot-2.0.0.dev0/ircbot/sqlitedb.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16430 2024-05-04 15:04:13.000000 re_ircbot-2.0.0.dev0/ircbot/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-04 15:04:21.306030 re_ircbot-2.0.0.dev0/re_ircbot.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14058 2024-05-04 15:04:21.000000 re_ircbot-2.0.0.dev0/re_ircbot.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      319 2024-05-04 15:04:21.000000 re_ircbot-2.0.0.dev0/re_ircbot.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-04 15:04:21.000000 re_ircbot-2.0.0.dev0/re_ircbot.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       18 2024-05-04 15:04:21.000000 re_ircbot-2.0.0.dev0/re_ircbot.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-05-04 15:04:21.000000 re_ircbot-2.0.0.dev0/re_ircbot.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-04 15:04:21.306030 re_ircbot-2.0.0.dev0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1869 2024-05-04 15:04:13.000000 re_ircbot-2.0.0.dev0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-04 22:47:52.168262 re_ircbot-2.0.1.dev0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1072 2024-05-04 22:47:44.000000 re_ircbot-2.0.1.dev0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14058 2024-05-04 22:47:52.168262 re_ircbot-2.0.1.dev0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13331 2024-05-04 22:47:44.000000 re_ircbot-2.0.1.dev0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-04 22:47:52.164262 re_ircbot-2.0.1.dev0/ircbot/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      125 2024-05-04 22:47:44.000000 re_ircbot-2.0.1.dev0/ircbot/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    53399 2024-05-04 22:47:44.000000 re_ircbot-2.0.1.dev0/ircbot/client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5384 2024-05-04 22:47:44.000000 re_ircbot-2.0.1.dev0/ircbot/dcc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17946 2024-05-04 22:47:44.000000 re_ircbot-2.0.1.dev0/ircbot/hooks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3027 2024-05-04 22:47:44.000000 re_ircbot-2.0.1.dev0/ircbot/message.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1972 2024-05-04 22:47:44.000000 re_ircbot-2.0.1.dev0/ircbot/shortest_prefix.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11380 2024-05-04 22:47:44.000000 re_ircbot-2.0.1.dev0/ircbot/sqlitedb.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1426 2024-05-04 22:47:44.000000 re_ircbot-2.0.1.dev0/ircbot/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-04 22:47:52.168262 re_ircbot-2.0.1.dev0/re_ircbot.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14058 2024-05-04 22:47:52.000000 re_ircbot-2.0.1.dev0/re_ircbot.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      335 2024-05-04 22:47:52.000000 re_ircbot-2.0.1.dev0/re_ircbot.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-04 22:47:52.000000 re_ircbot-2.0.1.dev0/re_ircbot.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       18 2024-05-04 22:47:52.000000 re_ircbot-2.0.1.dev0/re_ircbot.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-05-04 22:47:52.000000 re_ircbot-2.0.1.dev0/re_ircbot.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-04 22:47:52.168262 re_ircbot-2.0.1.dev0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1869 2024-05-04 22:47:44.000000 re_ircbot-2.0.1.dev0/setup.py
```

### Comparing `re_ircbot-2.0.0.dev0/LICENSE` & `re_ircbot-2.0.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.0.dev0/PKG-INFO` & `re_ircbot-2.0.1.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re-ircbot
-Version: 2.0.0.dev0
+Version: 2.0.1.dev0
 Summary: A simple async irc bot framework with regex command definitions and data permanency
 Home-page: https://github.com/matheusfillipe/ircbot
 Author: Matheus Fillipe
 Author-email: mattf@tilde.club
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `re_ircbot-2.0.0.dev0/README.md` & `re_ircbot-2.0.1.dev0/README.md`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.0.dev0/ircbot/client.py` & `re_ircbot-2.0.1.dev0/ircbot/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,99 +18,35 @@
 import random
 import re
 import socket
 from copy import copy, deepcopy
 from functools import partial
 from math import ceil
 from pathlib import Path
-from typing import Awaitable, Callable, TypeAlias
+from typing import Any, Awaitable, Callable
 
 from cachetools import TTLCache
 
-from ircbot import dcc, utils
-from ircbot.message import Message, RawMessage, ReplyIntent
+from ircbot import dcc, hooks
+from ircbot.message import Color, Message, RawMessage, ReplyIntent, Sendable
 from ircbot.sqlitedb import DB
-from ircbot.utils import debug, log, logger
+from ircbot.utils import debug, log, logger, validate_url
 
 Message = Message
 ReplyIntent = ReplyIntent
 RawMessage = RawMessage
 
 BUFFSIZE = 2048
 MAX_MESSAGE_LEN = 410
 
 
 class BotConnectionError(Exception):
     pass
 
 
-class Color(object):
-    """Colorcodes enum."""
-
-    esc = "\003"
-    white = "00"
-    black = "01"
-    navy = "02"
-    green = "03"
-    red = "04"
-    maroon = "05"
-    purple = "06"
-    orange = "07"
-    yellow = "08"
-    light_green = "09"
-    teal = "10"
-    cyan = "11"
-    blue = "12"
-    magenta = "13"
-    gray = "14"
-    light_gray = "15"
-
-    COLORS = [
-        "00",
-        "01",
-        "02",
-        "03",
-        "04",
-        "05",
-        "06",
-        "07",
-        "08",
-        "09",
-        "10",
-        "11",
-        "12",
-        "13",
-        "14",
-        "15",
-    ]
-
-    def __init__(self, text, fg=white, bg=None):
-        if bg is not None:
-            self.text = "{}{},{}{}".format(self.esc, fg, bg, text)
-        else:
-            self.text = "{}{}{}".format(self.esc, fg, text)
-        self.str = self.text + Color.esc
-
-    @classmethod
-    def random(cls):
-        return random.choice(cls.COLORS)
-
-    @classmethod
-    def colors(cls):
-        """Returns the color names."""
-        return [
-            k
-            for k in Color.__dict__
-            if not (k.startswith("_") or k in ["esc", "COLORS", "colors", "getcolors", "random"])
-        ]
-
-    def __str__(self):
-        return self.str
-
-
 class DBOperation(object):
     ADD = 1
     UPDATE = 0
     REMOVE = -1
 
     def __init__(self, data={}, id={}, op=UPDATE):
         self.data = data
@@ -224,17 +160,16 @@
         self.writer.close()
         await self.writer.wait_closed()
 
     def close(self):
         self.writer.close()
 
 
-class IrcBot:
-    AsyncCallback = Callable[["IrcBot"], Awaitable[None]]
-    Sendable: TypeAlias = str | Message | Color | list[str | Message | Color]
+class IrcBot(hooks.HookHandler):
+    AsyncCallback = Callable[[], Awaitable[None]]
 
     nick: str
     password: str
     server_password: str | None
     username: str
     host: str
     port: int
@@ -258,14 +193,15 @@
     ping_delay: int
     is_running_with_callback: bool
     async_callback: AsyncCallback | None
     retry_connecting: bool
     message_queue: asyncio.Queue[str]
     db_operation_queue: asyncio.Queue[PersistentData]
     stream: TCPStream
+    _data: Any
 
     def __init__(
         self,
         host: str,
         port: int = 6667,
         nick: str = "bot",
         channels: list[str] | str | None = None,
@@ -323,15 +259,14 @@
         self.port = port
         self.channels = channels
         self.use_sasl = use_sasl
         self.use_ssl = use_ssl
         self.tables = tables
         self.delay = delay
         self.accept_join_from = accept_join_from
-        self.custom_handlers = utils.custom_handlers
         self.custom_handlers.update(custom_handlers)
         self.strip_messages = strip_messages
         self.dcc_ports = dcc_ports
         self.dcc_host = dcc_host
         self.dcc_announce_host = dcc_announce_host
         self.middleware = []
         self._dcc_busy_ports = {}
@@ -344,39 +279,51 @@
 
         self._awaiting_messages = {}
 
         self.connected = False
         self.server_channels = {}
         self.channel_names = {}
 
-        if utils.arg_commands_with_message:
-            new_commands = deepcopy(utils._defined_command_dict)
-            new_commands.update(utils.arg_commands_with_message)
-            utils.set_commands(new_commands, prefix=utils.command_prefix)
-
         self.message_queue = asyncio.Queue()
         self.db_operation_queue = asyncio.Queue()
         self.replyIntents = {}
 
         self.ping_delay = 30  # seconds
 
         self.is_running_with_callback = False
         self.async_callback = None
         self.retry_connecting = False
 
+    @property
+    def data(self):
+        """Store anything you want in memory here."""
+        return self._data
+
+    @data.setter
+    def data(self, value: Any):
+        self._data = value
+
+    def _install_hooks(self):
+        self.custom_handlers.update(self.custom_handlers)
+        if self.arg_commands_with_message:
+            new_commands = deepcopy(self._defined_command_dict)
+            new_commands.update(self.arg_commands_with_message)
+            self.set_commands(new_commands, prefix=self.command_prefix)
+
     async def hot_reload(self):
         """Reload the handlers."""
-        utils._hot_reload()
-        self.custom_handlers.update(utils.custom_handlers)
-        if utils.arg_commands_with_message:
-            new_commands = deepcopy(utils._defined_command_dict)
-            new_commands.update(utils.arg_commands_with_message)
-            utils.set_commands(new_commands, prefix=utils.command_prefix)
+        self._hot_reload()
+        self.custom_handlers.update(self.custom_handlers)
+        if self.arg_commands_with_message:
+            new_commands = deepcopy(self._defined_command_dict)
+            new_commands.update(self.arg_commands_with_message)
+            self.set_commands(new_commands, prefix=self.command_prefix)
 
-    async def _mainloop(self, async_callback: AsyncCallback):
+    async def _mainloop(self, async_callback: AsyncCallback | None):
+        self._install_hooks()
         self.is_running_with_callback = bool(async_callback)
         self.async_callback = async_callback
         while True:
             try:
                 await self._main_task()
             except (BotConnectionError, socket.gaierror):
                 log(f"Attempting to reconnect in {self.ping_delay / 2}...")
@@ -399,24 +346,24 @@
     async def start_with_callback(self):
         await asyncio.gather(self.connect(), self._wait_and_async_cb_task())
 
     async def _wait_and_async_cb_task(self):
         while not self.connected:
             await asyncio.sleep(1)
         if self.async_callback:
-            await self.async_callback(self)
+            await self.async_callback()
 
     def add_middleware(self, method):
         """Adds a middleware to run before every command.
 
         :param method callable: Async method that will receive the this bot instance and the incoming message object for every command handling event. If this methods doesn't return True, then the callback execution stops.
         """
         self.middleware.append(method)
 
-    def run(self, async_callback: AsyncCallback):
+    def run(self, async_callback: AsyncCallback | None = None):
         """Simply starts the bot.
 
         param: async_callback: async function to be called.
         """
         asyncio.run(self._mainloop(async_callback))
 
     async def sleep(self, time):
@@ -448,14 +395,15 @@
 
     async def connect(self):
         remote_ip = socket.gethostbyname(self.host)
         log("ip of irc server is:", remote_ip)
         if self.use_ssl:
             log("Using SSL connection")
             import ssl
+
             ssl_context = ssl.create_default_context()
             ssl_context.check_hostname = False
             ssl_context.verify_mode = ssl.CERT_NONE
             reader, writer = await asyncio.open_connection(remote_ip, self.port, ssl=ssl_context)
         else:
             reader, writer = await asyncio.open_connection(remote_ip, self.port)
 
@@ -1016,15 +964,15 @@
     # MAIN DATA RECEIVING HANDLER
     async def data_handler(self, data: str):
         nick = self.nick
         host = self.host
         self.connected = True
 
         try:
-            if utils._hot_reload_if_changed():
+            if self._hot_reload_if_changed():
                 await self.hot_reload()
         except Exception as e:
             log(f"Error in hot reload: {str(e)}")
             logger.exception(e)
 
         IRC_P = {
             # DCC
@@ -1315,51 +1263,49 @@
                         _message,
                         _message,
                     )
                     del self.replyIntents[channel][sender_nick]
                     await self.process_result(result, channel, sender_nick, is_private)
                     return
 
-                for i, cmd in enumerate(utils.regex_commands[::-1] if not utils.parse_order else utils.regex_commands):
+                for i, cmd in enumerate(self.regex_commands[::-1] if not self.parse_order else self.regex_commands):
                     if matched:
                         break
                     for reg in cmd:
                         m = re.match(reg, msg)
                         if m:
-                            if cmd in utils.regex_commands:
-                                if is_private and not utils.regex_commands_accept_pm[i]:
+                            if cmd in self.regex_commands:
+                                if is_private and not self.regex_commands_accept_pm[i]:
                                     continue
                                 _message = Message(channel, sender_nick, msg, is_private)
                                 result = await self._call_cb(cmd[reg], _message, m)
                             if result:
                                 await self.process_result(result, channel, sender_nick, is_private)
                                 matched = True
-                            if utils.single_match:
+                            if self.single_match:
                                 matched = True
                                 break
 
-                if matched and utils.single_match:
+                if matched and self.single_match:
                     await self.check_tables()
                     return
 
                 for i, cmd in enumerate(
-                    utils.regex_commands_with_message[::-1]
-                    if not utils.parse_order
-                    else utils.regex_commands_with_message
+                    self.regex_commands_with_message[::-1] if not self.parse_order else self.regex_commands_with_message
                 ):
                     if matched:
                         break
                     for reg in cmd:
                         m = re.match(reg, msg)  # , flags=re.IGNORECASE)
                         if m:
-                            if cmd in utils.regex_commands_with_message:
-                                if is_private and not utils.regex_commands_with_message_accept_pm[i]:
+                            if cmd in self.regex_commands_with_message:
+                                if is_private and not self.regex_commands_with_message_accept_pm[i]:
                                     continue
                                 debug("sending to", sender_nick)
-                                if utils.regex_commands_with_message_pass_data[i]:
+                                if self.regex_commands_with_message_pass_data[i]:
                                     _message = Message(
                                         channel,
                                         sender_nick,
                                         msg,
                                         is_private,
                                         strip=self.strip_messages,
                                     )
@@ -1378,35 +1324,35 @@
                                         strip=self.strip_messages,
                                     )
                                     result = await self._call_cb(cmd[reg], _message, m, _message)
 
                             if result:
                                 await self.process_result(result, channel, sender_nick, is_private)
                                 matched = True
-                            if utils.single_match:
+                            if self.single_match:
                                 matched = True
                                 break
 
-                if matched and utils.single_match:
+                if matched and self.single_match:
                     await self.check_tables()
                     return
 
                 # URL MATCHER
-                if utils.url_commands:
+                if self.url_commands:
                     for word in msg.split(" "):
                         if len(word) < 6:
                             continue
                         result = None
                         word = word.strip()
                         if word[-1] in [" ", "?", ",", ";", ":", "\\"]:
                             word = word[:-1]
-                        if utils.validate_url(word):
+                        if validate_url(word):
                             debug("Checking url: " + str(word))
                             _message = Message(channel, sender_nick, msg, is_private)
-                            result = await self._call_cb(utils.url_commands[-1], _message, word)
+                            result = await self._call_cb(self.url_commands[-1], _message, word)
                         if result:
                             await self.send_message(result, channel)
 
             await self.check_tables()
 
         except Exception as e:
             log("ERROR IN MAINLOOP: ", e)
@@ -1415,15 +1361,15 @@
     async def _call_cb(self, cb, message, *args, **kwargs):
         if message is not None:
             for middleware in self.middleware:
                 resp = await middleware(self, message)
                 if not resp:
                     return
         if inspect.iscoroutinefunction(cb):
-            return await cb(self, *args, **kwargs)
+            return await cb(*args, **kwargs)
         return cb(*args, **kwargs)
 
     def __del__(self):
         try:
             self.stream.close()
         except:
             pass
```

### Comparing `re_ircbot-2.0.0.dev0/ircbot/dcc.py` & `re_ircbot-2.0.1.dev0/ircbot/dcc.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.0.dev0/ircbot/shortest_prefix.py` & `re_ircbot-2.0.1.dev0/ircbot/shortest_prefix.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.0.dev0/ircbot/sqlitedb.py` & `re_ircbot-2.0.1.dev0/ircbot/sqlitedb.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.0.dev0/ircbot/utils.py` & `re_ircbot-2.0.1.dev0/ircbot/hooks.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,534 +1,469 @@
-# TODO make a class instead of this globals crap
+# TODO: Use self typehints instead of class
+from __future__ import annotations
 
-import collections
 import importlib.util
 import inspect
 import logging
 import os
 import re
-import sys
+from collections.abc import Callable
 from functools import wraps
+from typing import Awaitable, Literal, TypeAlias, get_args
 
-has_validators = False
-try:
-    import validators
-
-    has_validators = True
-except:
-    pass
-
-from ircbot.message import Message
+from ircbot.message import Message, Sendable
 from ircbot.shortest_prefix import find_shortest_prefix
-
-logger = None
-
-parse_order = False
-
-# COMMAND DECORATORS
-regex_commands = []
-regex_commands_accept_pm = []
-
-# HOT RELOAD
-hot_reload_env = os.environ.get("IRCBOT_HOT_RELOAD", "False").lower() in ["true", "1", "yes", "on"]
-hot_reload_files = set()
-hot_reload_hash_map = {}
+from ircbot.utils import log
 
 
 def md5_file(file):
     import hashlib
 
     with open(file, "rb") as f:
         return hashlib.md5(f.read()).hexdigest()
 
 
-def _hot_reload_if_changed():
-    """Checks if any of the files in hot_reload_files has changed and if so
-    Only works if hot_reload_env is True.
-
-    :return: True if any file has changed
-    """
-    if hot_reload_env:
-        for module_path in hot_reload_files:
-            new_hash = md5_file(module_path)
-            current_hash = hot_reload_hash_map.get(module_path, None)
-            hot_reload_hash_map[module_path] = new_hash
-            if new_hash != current_hash and current_hash is not None:
-                log(f"Reloading due changes to {module_path}")
-                _hot_reload()
-                return True
-    return False
-
-
-def _add_hot_reload(func):
-    """Adds full path to file of function to hot_reload_files set."""
-    module_path = inspect.getfile(func)
-    hot_reload_files.add(module_path)
-
-
-def regex_cmd(filters, acccept_pms=True, **kwargs):
-    """regex_cmd. The function should take a match object from the re python
-    library. Will not receive private messages, use regex_commands_with_message
-    instead.
-
-    :param filters: Regex expression
-    :param acccept_pms: bool. Should this command work with private messages?.
-    :param kwargs:
-    """
-
-    def wrap_cmd(func):
-        @wraps(func)
-        def wrapped(*a, **bb):
-            return func(*a, **bb)
-
-        _add_hot_reload(func)
-        regex_commands.append({filters: func})
-        regex_commands_accept_pm.append(acccept_pms)
-        return wrapped
-
-    return wrap_cmd
-
-
-regex_commands_with_message = []
-regex_commands_with_message_accept_pm = []
-regex_commands_with_message_pass_data = []
-
-
-def regex_cmd_with_messsage(filters, acccept_pms=True, pass_data=False, **kwargs):
-    """regex_cmd_with_sender. The function should take a match object from the
-    re python library and a IrcBot.Message as a second parameter.
-
-    :param filters: regex filter
-    :param acccept_pms: bool. Should this command work with private messages?.
-    :param pass_data: If true function should accept an extra data argument.
-    :param kwargs:
-    """
-    logging.debug("Creating regex with message: %s", filters)
-
-    def wrap_cmd(func):
-        @wraps(func)
-        def wrapped(*a, **bb):
-            return func(*a, **bb)
-
-        _add_hot_reload(func)
-        regex_commands_with_message.append({filters: func})
-        regex_commands_with_message_accept_pm.append(acccept_pms)
-        regex_commands_with_message_pass_data.append(pass_data)
-        return wrapped
-
-    return wrap_cmd
-
-
-url_commands = []
-
-
-def url_handler(**kwargs):
-    """url_handler. The function should take a string that is the matched url.
-
-    :param kwargs:
-    """
-
-    def wrap_cmd(func):
-        @wraps(func)
-        def wrapped(*a, **bb):
-            return func(*a, **bb)
-
-        _add_hot_reload(func)
-        url_commands.append(func)
-        return wrapped
-
-    return wrap_cmd
-
-
-custom_handlers = {}
-
-
-def custom_handler(action, **kwargs):
-    """custom_handler. Add handlers for other user actions like join, quit,
-    part..
-
-    :param action: str or list of strings with one or more of the possible actions
-        Possible actions and function necessary arguments are:
-        type             kwargs
-        'privmsg' -> {'nick', 'channel', 'text'}
-        'ping' -> {'ping'}
-        'names' -> {'channel', 'names'}
-        'channel' -> {'channel', 'channeldescription'}
-        'join' -> {'nick', 'channel'}
-        'quit' -> {'nick', 'text'}
-        'part' -> {'nick', 'channel'}
-        'dccsend' -> {'nick', 'filename', 'ip', 'port', 'size'}
-    """
-
-    def wrap_cmd(func):
-        @wraps(func)
-        def wrapped(*a, **bb):
-            return func(*a, **bb)
-
-        if isinstance(action, str):
-            custom_handlers[action] = func
-        if isinstance(action, list):
-            for a in action:
-                custom_handlers[a] = func
-        return wrapped
-
-    return wrap_cmd
-
-
-single_match = False
-command_prefix = "!"
-_command_max_arguments = 25
-_NonSpace = r"\S"
-re_command = lambda cmd, acccept_pms=True, pass_data=False, **kwargs: regex_cmd_with_messsage(
-    f"^{command_prefix}{cmd}{f'(?: +({_NonSpace}+))?'*_command_max_arguments} *$",
-    acccept_pms,
-    pass_data,
-    **kwargs,
-)
-
-arg_commands_with_message = {}
-
-simplify_arg_commands = True
-
-
-def set_simplify_commands(simplify):
-    global simplify_arg_commands
-    simplify_arg_commands = simplify
-
-
-def arg_command(
-    command,
-    help="",
-    command_help="",
-    acccept_pms=True,
-    pass_data=False,
-    simplify=None,
-    **kwargs,
-):
-    """Wrapper for setCommands.
-
-    :param command: Command
-    :param acccept_pms: bool. Should this command work with private messages?.
-    param: simplify: Uses shortest prefixes for each command. If True the shortest differentiatable prefixes for the commands will work. Like if there is start and stop, !sta will call start and !sto will call stop. Instead of passing a function  directly you can pass in a dict like:
-    param: help: Message to display on help command.
-    param: command_help: Message to display on help command with this command's name as argument.
-    """
-
-    if simplify is None:
-        simplify = simplify_arg_commands
-
-    def wrap_cmd(func):
-        @wraps(func)
-        def wrapped(*a, **bb):
-            return func(*a, **bb)
-
-        _add_hot_reload(func)
-        arg_commands_with_message[command] = {
-            "function": func,
-            "acccept_pms": acccept_pms,
-            "pass_data": pass_data,
-            "help": help,
-            "command_help": command_help,
-            "simplify": simplify,
-        }
-
-        return wrapped
-
-    return wrap_cmd
-
-
-help_msg_header = []
-help_msg = {}
-help_msg_bottom = []
-commands_help = {}
-help_menu_separator = "\n"
-help_on_private = False
-
-
-def set_help_menu_separator(sep: str):
-    """Sets the separator string between the help commands. If can contain a
-    '\n'.
-
-    :param sep: separator
-    :type sep: str
-    """
-    global help_menu_separator
-    help_menu_separator = sep
-
-
-def set_help_on_private(is_private):
-    """Defines if the help messages should be sent as private messages. This is
-    useful to avoide flooding if the bots has many commands.
-
-    :param is_private: if true they will be private (default False: display on the current channel)
-    """
-    global help_on_private
-    help_on_private = is_private
-
-
-def set_help_header(txt: str):
-    """Adds some text to the help message before the command descriptions.
-
-    :param txt: Text to display before command descriptions
-    :type txt: str
-    """
-    global help_msg_header
-    if isinstance(txt, str):
-        help_msg_header = [txt]
-    elif isinstance(txt, list):
-        help_msg_header = txt
-    else:
-        raise BaseException("You must pass wither a list of strings or a string")
-
-
-def set_help_bottom(txt: str):
-    """Adds some text to the help message after the command descriptions.
-
-    :param txt: Text to display after command descriptions
-    :type txt: str
-    """
-    global help_msg_bottom
-    if isinstance(txt, str):
-        help_msg_bottom = [txt]
-    elif isinstance(txt, list):
-        help_msg_bottom = txt
-    else:
-        raise BaseException("You must pass wither a list of strings or a string")
-
-
 def _reg_word(org, pref):
     opt_open = r"(?:"
     opt_close = r")?"
     return (
         re.escape(pref)
         + opt_open * (len([re.escape(c) for c in org[len(pref) :]]) > 0)
         + opt_open.join([re.escape(c) for c in org[len(pref) :]])
         + opt_close * len(org[len(pref) :])
     )
 
 
-_defined_command_dict = {}
-
+Actions = Literal["privmsg", "ping", "names", "channel", "join", "quit", "part", "dccsend"]
 
-def set_commands(command_dict: dict, simplify=None, prefix="!"):
-    """Defines commands for the bot from existing functions
-    param: command_dict: Takes a dictionary of "command names": function's to call creating the commands for each of them.
-    param: simplify: Uses shortest prefixes for each command. If True the shortest differentiatable prefixes for the commands will work. Like if there is start and stop, !sta will call start and !sto will call stop. Instead of passing a function  directly you can pass in a dict like:
-    {"function": cb, "acccept_pms": True, "pass_data": True, "help": "This command starts the bot", "command_help": "Detailed help for this command in particular"}
-    if needed. The help parameter if passed will define the 'help' command.
-    """
-    global command_prefix, help_msg, commands_help
-    command_prefix = prefix
-
-    if simplify is None:
-        simplify = simplify_arg_commands
-
-    if "help" in command_dict:
-        logging.error("You should not redefine 'help'")
-
-    def not_regex(c):
-        if len(c) < 2:
-            return True
-        if isinstance(command_dict[c], dict) and "simplify" not in command_dict[c]:
-            return not simplify
-        if isinstance(command_dict[c], dict) and "simplify" in command_dict[c]:
-            return not command_dict[c]["simplify"]
-        return False
-
-    _commands = find_shortest_prefix([c for c in command_dict.keys() if not not_regex(c)])
-    min_commands = []
-    exclude_list = [c for c in command_dict.keys() if not_regex(c)]
-    for cmd in command_dict:
-        if cmd in exclude_list:
-            min_commands.append(cmd)
+Regex: TypeAlias = str | re.Pattern
+RegexCallback = Callable[[re.Match], Sendable | Awaitable[Sendable | None]]
+RegexWithMessageCallback = Callable[[re.Match, Message], Sendable | Awaitable[Sendable | None]]
+UrlCallback = Callable[[str], Sendable | Awaitable[Sendable | None]]
+ArgCommandCallback = Callable[[re.Match, Message], Sendable | Awaitable[Sendable | None]]
+
+
+class HookHandler:
+    """Defines the behavior of the bot"""
+
+    parse_order = False
+
+    # COMMAND DECORATORS
+    regex_commands: list[dict[Regex, Callable]] = []
+    regex_commands_accept_pm: list[bool] = []
+
+    regex_commands_with_message: list[dict[Regex, RegexWithMessageCallback]] = []
+    regex_commands_with_message_accept_pm: list[bool] = []
+    regex_commands_with_message_pass_data: list[bool] = []
+
+    url_commands: list[UrlCallback] = []
+
+    custom_handlers: dict[str, Callable] = {}
+
+    arg_commands_with_message = {}
+
+    # HOT RELOAD
+    hot_reload_env = os.environ.get("IRCBOT_HOT_RELOAD", "False").lower() in ["true", "1", "yes", "on"]
+    hot_reload_files = set()
+    hot_reload_hash_map = {}
+
+    def regex_cmd(self, filters: Regex, acccept_pms: bool = True, **kwargs):
+        """regex_cmd. The function should take a match object from the re python
+        library. Will not receive private messages, use regex_commands_with_message
+        instead.
+
+        :param filters: Regex expression
+        :param acccept_pms: bool. Should this command work with private messages?.
+        :param kwargs:
+        """
+
+        def wrap_cmd(func: RegexCallback):
+            @wraps(func)
+            def wrapped(*a, **bb):
+                return func(*a, **bb)
+
+            self._add_hot_reload(func)
+            self.regex_commands.append({filters: func})
+            self.regex_commands_accept_pm.append(acccept_pms)
+            return wrapped
+
+        return wrap_cmd
+
+    def regex_cmd_with_messsage(self, filters: Regex, acccept_pms: bool = True, pass_data: bool = False, **kwargs):
+        """regex_cmd_with_sender. The function should take a match object from the
+        re python library and a IrcBot.Message as a second parameter.
+
+        :param filters: regex filter
+        :param acccept_pms: bool. Should this command work with private messages?.
+        :param pass_data: If true function should accept an extra data argument.
+        :param kwargs:
+        """
+        logging.debug("Creating regex with message: %s", filters)
+
+        def wrap_cmd(func):
+            @wraps(func)
+            def wrapped(*a, **bb):
+                return func(*a, **bb)
+
+            self._add_hot_reload(func)
+            self.regex_commands_with_message.append({filters: func})
+            self.regex_commands_with_message_accept_pm.append(acccept_pms)
+            self.regex_commands_with_message_pass_data.append(pass_data)
+            return wrapped
+
+        return wrap_cmd
+
+    def url_handler(self, **kwargs):
+        """url_handler. The function should take a string that is the matched url.
+
+        :param kwargs:
+        """
+
+        def wrap_cmd(func: UrlCallback):
+            @wraps(func)
+            def wrapped(*a, **bb):
+                return func(*a, **bb)
+
+            self._add_hot_reload(func)
+            self.url_commands.append(func)
+            return wrapped
+
+        return wrap_cmd
+
+    def custom_handler(self, action: Actions | list[Actions], **kwargs):
+        """custom_handler. Add handlers for other user actions like join, quit,
+        part..
+
+        :param action: str or list of strings with one or more of the possible actions
+            Possible actions and function necessary arguments are:
+            type             kwargs
+            'privmsg' -> {'nick', 'channel', 'text'}
+            'ping' -> {'ping'}
+            'names' -> {'channel', 'names'}
+            'channel' -> {'channel', 'channeldescription'}
+            'join' -> {'nick', 'channel'}
+            'quit' -> {'nick', 'text'}
+            'part' -> {'nick', 'channel'}
+            'dccsend' -> {'nick', 'filename', 'ip', 'port', 'size'}
+        """
+
+        def wrap_cmd(func):
+            @wraps(func)
+            def wrapped(*a, **bb):
+                return func(*a, **bb)
+
+            accepted_actions = set(get_args(Actions))
+            if isinstance(action, str):
+                if action not in accepted_actions:
+                    raise ValueError(f"Invalid action {action}")
+                self.custom_handlers[action] = func
+            if isinstance(action, list) or isinstance(action, set):
+                for a in action:
+                    if a not in accepted_actions:
+                        raise ValueError(f"Invalid action {a}")
+                    self.custom_handlers[a] = func
+            return wrapped
+
+        return wrap_cmd
+
+    single_match: bool = False
+    command_prefix: str = "!"
+    _command_max_arguments: int = 25
+
+    simplify_arg_commands: bool = True
+
+    def re_command(self, cmd, acccept_pms=True, pass_data=False, **kwargs):
+        non_space: str = r"\S"
+        return self.regex_cmd_with_messsage(
+            f"^{self.command_prefix}{cmd}{f'(?: +({non_space}+))?'*self._command_max_arguments} *$",
+            acccept_pms,
+            pass_data,
+            **kwargs,
+        )
+
+    def set_simplify_commands(self, simplify: bool) -> HookHandler:
+        self.simplify_arg_commands = simplify
+        return self
+
+    def arg_command(
+        self,
+        command: str,
+        help: str = "",
+        command_help: str = "",
+        acccept_pms: bool = True,
+        pass_data: bool = False,
+        simplify: bool | None = None,
+        **kwargs,
+    ):
+        """Wrapper for setCommands.
+
+        :param command: Command
+        :param acccept_pms: bool. Should this command work with private messages?.
+        param: simplify: Uses shortest prefixes for each command. If True the shortest differentiatable prefixes for the commands will work. Like if there is start and stop, !sta will call start and !sto will call stop. Instead of passing a function  directly you can pass in a dict like:
+        param: help: Message to display on help command.
+        param: command_help: Message to display on help command with this command's name as argument.
+        """
+
+        if simplify is None:
+            simplify = self.simplify_arg_commands
+
+        def wrap_cmd(func: ArgCommandCallback):
+            @wraps(func)
+            def wrapped(*a, **bb):
+                return func(*a, **bb)
+
+            self._add_hot_reload(func)
+            self.arg_commands_with_message[command] = {
+                "function": func,
+                "acccept_pms": acccept_pms,
+                "pass_data": pass_data,
+                "help": help,
+                "command_help": command_help,
+                "simplify": simplify,
+            }
+
+            return wrapped
+
+        return wrap_cmd
+
+    help_msg_header: list[str] = []
+    help_msg: dict[str, str] = {}
+    help_msg_bottom: list[str] = []
+    commands_help = {}
+    help_menu_separator: str = "\n"
+    help_on_private: bool = False
+
+    def set_help_menu_separator(self, sep: str) -> HookHandler:
+        """Sets the separator string between the help commands. If can contain a
+        '\n'.
+
+        :param sep: separator
+        :type sep: str
+        """
+        self.help_menu_separator = sep
+        return self
+
+    def set_help_on_private(self, is_private: bool) -> HookHandler:
+        """Defines if the help messages should be sent as private messages. This is
+        useful to avoide flooding if the bots has many commands.
+
+        :param is_private: if true they will be private (default False: display on the current channel)
+        """
+        self.help_on_private = is_private
+        return self
+
+    def set_help_header(self, txt: str) -> HookHandler:
+        """Adds some text to the help message before the command descriptions.
+
+        :param txt: Text to display before command descriptions
+        :type txt: str
+        """
+        if isinstance(txt, str):
+            self.help_msg_header = [txt]
+        elif isinstance(txt, list):
+            self.help_msg_header = txt
         else:
-            min_commands.append(_commands[cmd])
+            raise BaseException("You must pass wither a list of strings or a string")
+        return self
 
-    regexps = [
-        _reg_word(org, pref) if not not_regex(org) else re.escape(org)
-        for org, pref in zip(command_dict.keys(), min_commands)
-    ]
-
-    for cmd, reg in zip(command_dict.keys(), regexps):
-        cb = command_dict[cmd]
-        # give preference if simplify comes in a dict
-        simp = simplify and not not_regex(cmd)
-        expression = reg if simp else cmd
-        logging.debug("DEFINING %s", expression)
-        logging.debug("simplify? %s", simplify)
-        logging.debug("simp? %s", simp)
-
-        if isinstance(cb, dict):
-            re_command(
-                expression,
-                acccept_pms=True if "acccept_pms" not in cb else cb["acccept_pms"],
-                pass_data=False if "pass_data" not in cb else cb["pass_data"],
-            )(cb["function"])
-            help_msg[cmd] = f"{command_prefix}{cmd}: {cb['help']}" if "help" in cb else ""
-
-            if "command_help" in cb and cb["command_help"]:
-                commands_help[cmd] = cb["command_help"]
-            elif "help" in cb and cb["help"]:
-                commands_help[cmd] = cb["help"]
+    def set_help_bottom(self, txt: str) -> HookHandler:
+        """Adds some text to the help message after the command descriptions.
 
-        elif isinstance(cb, collections.abc.Callable):
-            re_command(expression)(cb)
+        :param txt: Text to display after command descriptions
+        :type txt: str
+        """
+        if isinstance(txt, str):
+            self.help_msg_bottom = [txt]
+        elif isinstance(txt, list):
+            self.help_msg_bottom = txt
         else:
-            logging.error("You passed a wrong data type on setCommands for command: %s", cmd)
-            sys.exit(1)
-
-    _defined_command_dict = command_dict
-    if help_msg or commands_help:
-        _commands = find_shortest_prefix([c for c in command_dict.keys() if not not_regex(c)] + ["help"])
-
-        def help_menu(args, message):
-            channel = message.channel
-            if help_on_private:
-                channel = message.sender_nick
-
-            if args[1] in commands_help:
-                return Message(channel, message=commands_help[args[1]])
-            if help_msg:
-                if "\n" in help_menu_separator:
-                    before = help_menu_separator.split("\n")[0]
-                    after = help_menu_separator.split("\n")[-1]
-                    txt = list(help_msg.values())[0]
-                    return (
-                        help_msg_header
-                        + [Message(channel, message=after + txt + before) for txt in help_msg.values()]
-                        + help_msg_bottom
-                    )
-                else:
-                    return (
-                        help_menu_separator.join(help_msg_header)
-                        + help_menu_separator.join(help_msg.values())
-                        + help_menu_separator.join(help_msg_bottom)
-                    )
-
-        re_command(_reg_word("help", _commands["help"]))(help_menu)
-
-
-def set_prefix(prefix):
-    """setPrefix. Sets the prefix for arg commands.
-
-    :param prefix: str prefix for commands
-    """
-    global command_prefix
-    command_prefix = prefix
-
-
-def set_single_match(singleMatch: bool):
-    """Defines if there will be only one command handler called. If false all regex and arg_commands will be matched against the user input.
-    :param singleMatch: If true there will be only one match per command. Defaults to False (all matches will be called)
-    :type singleMatch: bool
-    """
-    global single_match
-    single_match = singleMatch
-
+            raise BaseException("You must pass wither a list of strings or a string")
+        return self
 
-def set_parser_order(top_bottom: bool = True):
-    """setParseOrder.
+    _defined_command_dict = {}
 
-    :param top_bottom: bool -> if True then first defined regex expressions will overwrite last ones. Default is False
-    """
-    global parse_order
-    parse_order = top_bottom
+    def set_commands(self, command_dict: dict, simplify: bool | None = None, prefix: str = "!"):
+        """Defines commands for the bot from existing functions
+        param: command_dict: Takes a dictionary of "command names": function's to call creating the commands for each of them.
+        param: simplify: Uses shortest prefixes for each command. If True the shortest differentiatable prefixes for the commands will work. Like if there is start and stop, !sta will call start and !sto will call stop. Instead of passing a function  directly you can pass in a dict like:
+        {"function": cb, "acccept_pms": True, "pass_data": True, "help": "This command starts the bot", "command_help": "Detailed help for this command in particular"}
+        if needed. The help parameter if passed will define the 'help' command.
+        """
+        self.command_prefix = prefix
 
+        if simplify is None:
+            simplify = self.simplify_arg_commands
 
-def set_max_arguments(n):
-    """setMaxArguments.
-
-    :param n: number of arguments for callbacks in arg_command decorator
-    """
-    global _command_max_arguments
-    _command_max_arguments = n
-
-
-def set_loglevel(level, logfile=None):
-    """Sets the loggins level of the logging module.
-
-    :param level: int. level, (logging.DEBUG, logging.INFO, etc...)
-    :param logfile: str. Path for file or empty for none.
-    """
-    global logger
-    logging.basicConfig(
-        level=level,
-        filename=logfile,
-        format="%(asctime)s::%(levelname)s -> %(message)s",
-        datefmt="%I:%M:%S %p",
-    )
-    logger = logging.getLogger()
-    logger.setLevel(level)
+        if "help" in command_dict:
+            logging.error("You should not redefine 'help'")
 
+        def not_regex(c):
+            if len(c) < 2:
+                return True
+            if isinstance(command_dict[c], dict) and "simplify" not in command_dict[c]:
+                return not simplify
+            if isinstance(command_dict[c], dict) and "simplify" in command_dict[c]:
+                return not command_dict[c]["simplify"]
+            return False
+
+        _commands = find_shortest_prefix([c for c in command_dict.keys() if not not_regex(c)])
+        min_commands = []
+        exclude_list = [c for c in command_dict.keys() if not_regex(c)]
+        for cmd in command_dict:
+            if cmd in exclude_list:
+                min_commands.append(cmd)
+            else:
+                min_commands.append(_commands[cmd])
 
-set_loglevel(logging.DEBUG)
+        regexps = [
+            _reg_word(org, pref) if not not_regex(org) else re.escape(org)
+            for org, pref in zip(command_dict.keys(), min_commands)
+        ]
+
+        for cmd, reg in zip(command_dict.keys(), regexps):
+            cb = command_dict[cmd]
+            # give preference if simplify comes in a dict
+            simp = simplify and not not_regex(cmd)
+            expression = reg if simp else cmd
+            logging.debug("DEFINING %s", expression)
+            logging.debug("simplify? %s", simplify)
+            logging.debug("simp? %s", simp)
+
+            if isinstance(cb, dict):
+                self.re_command(
+                    expression,
+                    acccept_pms=True if "acccept_pms" not in cb else cb["acccept_pms"],
+                    pass_data=False if "pass_data" not in cb else cb["pass_data"],
+                )(cb["function"])
+                self.help_msg[cmd] = f"{self.command_prefix}{cmd}: {cb['help']}" if "help" in cb else ""
+
+                if "command_help" in cb and cb["command_help"]:
+                    self.commands_help[cmd] = cb["command_help"]
+                elif "help" in cb and cb["help"]:
+                    self.commands_help[cmd] = cb["help"]
 
+            elif isinstance(cb, Callable):
+                self.re_command(expression)(cb)
+            else:
+                raise BaseException(f"Invalid command definition for {cmd}")
 
-def log(*args, level=logging.INFO):
-    msg = " ".join([str(a) for a in list(args)])
-    if type(level) == int:
-        logger.log(level, msg)
-    elif type(level) == str:
-        getattr(logger, level)(msg)
-
-
-def debug(*args, level=logging.DEBUG):
-    msg = " ".join([str(a) for a in list(args)])
-    logger.log(level, msg)
-
-
-def warning(*args, level=logging.WARNING):
-    msg = " ".join([str(a) for a in list(args)])
-    logger.log(level, msg)
-
-
-# Extras
-def validate_url(url):
-    if has_validators:
-        return validators.url(url)
-    else:
-        log("You do not have the validators module installed! run `pip install validators` to use this functionality")
-
-
-def m2list(args):
-    return [args[i] for i in range(1, _command_max_arguments) if args[i]]
-
-
-def _hot_reload():
-    """Reloads all files in hot_reload_files setting regex_commands, regex_commands_with_message, url_commands, custom_handlers"""
-    global regex_commands, regex_commands_accept_pm, regex_commands_with_message, regex_commands_with_message_accept_pm, regex_commands_with_message_pass_data, url_commands, arg_commands_with_message, custom_handlers
-    state = [
-        regex_commands,
-        regex_commands_accept_pm,
-        regex_commands_with_message,
-        regex_commands_with_message_accept_pm,
-        regex_commands_with_message_pass_data,
-        url_commands,
-        arg_commands_with_message,
-        custom_handlers,
-    ]
-    initial_state = []
-    for s in state:
-        initial_state.append(s.copy())
-        s.clear()
-
-    for file in hot_reload_files:
-        # skip current file
-        if file == __file__:
-            continue
-        log(f"Reloading {file}")
-        try:
-            module_name = os.path.basename(file).split(".")[0]
-            spec = importlib.util.spec_from_file_location(module_name, file)
-            if spec is None:
-                log(f"Error reloading {file}: spec is None")
+        self._defined_command_dict = command_dict
+        if self.help_msg or self.commands_help:
+            _commands = find_shortest_prefix([c for c in command_dict.keys() if not not_regex(c)] + ["help"])
+
+            def help_menu(args, message):
+                channel = message.channel
+                if self.help_on_private:
+                    channel = message.sender_nick
+
+                if args[1] in self.commands_help:
+                    return Message(channel, message=self.commands_help[args[1]])
+                if self.help_msg:
+                    if "\n" in self.help_menu_separator:
+                        before = self.help_menu_separator.split("\n")[0]
+                        after = self.help_menu_separator.split("\n")[-1]
+                        return (
+                            self.help_msg_header
+                            + [Message(channel, message=after + txt + before) for txt in self.help_msg.values()]
+                            + self.help_msg_bottom
+                        )
+                    else:
+                        return (
+                            self.help_menu_separator.join(self.help_msg_header)
+                            + self.help_menu_separator.join(self.help_msg.values())
+                            + self.help_menu_separator.join(self.help_msg_bottom)
+                        )
+
+            self.re_command(_reg_word("help", _commands["help"]))(help_menu)
+
+    def set_prefix(self, prefix) -> HookHandler:
+        """setPrefix. Sets the prefix for arg commands.
+
+        :param prefix: str prefix for commands
+        """
+        self.command_prefix = prefix
+        return self
+
+    def set_single_match(self, _single_match: bool) -> HookHandler:
+        """Defines if there will be only one command handler called. If false all regex and arg_commands will be matched against the user input.
+        :param singleMatch: If true there will be only one match per command. Defaults to False (all matches will be called)
+        :type singleMatch: bool
+        """
+        self.single_match = _single_match
+        return self
+
+    def set_parser_order(self, top_bottom: bool = True) -> HookHandler:
+        """setParseOrder.
+
+        :param top_bottom: bool -> if True then first defined regex expressions will overwrite last ones. Default is False
+        """
+        self.parse_order = top_bottom
+        return self
+
+    def set_max_arguments(self, n: int) -> HookHandler:
+        """setMaxArguments.
+
+        :param n: number of arguments for callbacks in arg_command decorator
+        """
+        self._command_max_arguments = n
+        return self
+
+    def _add_hot_reload(self, func):
+        """Adds full path to file of function to hot_reload_files set."""
+        module_path = inspect.getfile(func)
+        self.hot_reload_files.add(module_path)
+
+    def _hot_reload(self):
+        """Reloads all files in hot_reload_files setting regex_commands, regex_commands_with_message, url_commands, custom_handlers"""
+        state = [
+            self.regex_commands,
+            self.regex_commands_accept_pm,
+            self.regex_commands_with_message,
+            self.regex_commands_with_message_accept_pm,
+            self.regex_commands_with_message_pass_data,
+            self.url_commands,
+            self.arg_commands_with_message,
+            self.custom_handlers,
+        ]
+        initial_state = []
+        for s in state:
+            initial_state.append(s.copy())
+            s.clear()
+
+        for file in self.hot_reload_files:
+            # skip current file
+            if file == __file__:
                 continue
-            else:
-                module = importlib.util.module_from_spec(spec)
-                spec.loader.exec_module(module)
+            log(f"Reloading {file}")
+            try:
+                module_name = os.path.basename(file).split(".")[0]
+                spec = importlib.util.spec_from_file_location(module_name, file)
+                if spec is None:
+                    log(f"Error reloading {file}: spec is None")
+                    continue
+                else:
+                    module = importlib.util.module_from_spec(spec)
+                    spec.loader.exec_module(module)
 
-        except Exception as e:
-            log(f"Error reloading {file}: {e}")
-            for i, s in enumerate(state):
-                s.clear()
-                s = initial_state[i]
-            raise e
+            except Exception as e:
+                log(f"Error reloading {file}: {e}")
+                for i, s in enumerate(state):
+                    s.clear()
+                    s = initial_state[i]
+                raise e
+
+    def _hot_reload_if_changed(self):
+        """Checks if any of the files in hot_reload_files has changed and if so
+        Only works if hot_reload_env is True.
+
+        :return: True if any file has changed
+        """
+        if self.hot_reload_env:
+            for module_path in self.hot_reload_files:
+                new_hash = md5_file(module_path)
+                current_hash = self.hot_reload_hash_map.get(module_path, None)
+                self.hot_reload_hash_map[module_path] = new_hash
+                if new_hash != current_hash and current_hash is not None:
+                    log(f"Reloading due changes to {module_path}")
+                    self._hot_reload()
+                    return True
+        return False
```

### Comparing `re_ircbot-2.0.0.dev0/re_ircbot.egg-info/PKG-INFO` & `re_ircbot-2.0.1.dev0/re_ircbot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re-ircbot
-Version: 2.0.0.dev0
+Version: 2.0.1.dev0
 Summary: A simple async irc bot framework with regex command definitions and data permanency
 Home-page: https://github.com/matheusfillipe/ircbot
 Author: Matheus Fillipe
 Author-email: mattf@tilde.club
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `re_ircbot-2.0.0.dev0/setup.py` & `re_ircbot-2.0.1.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 import subprocess
 
 import setuptools
 
-VERSION = "2.0.0-dev"
+VERSION = "2.0.1-dev"
 BRANCH = "v2"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 def requirements():
```

