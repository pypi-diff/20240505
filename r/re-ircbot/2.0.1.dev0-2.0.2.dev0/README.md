# Comparing `tmp/re_ircbot-2.0.1.dev0.tar.gz` & `tmp/re_ircbot-2.0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "re_ircbot-2.0.1.dev0.tar", last modified: Sat May  4 22:47:52 2024, max compression
+gzip compressed data, was "re_ircbot-2.0.2.dev0.tar", last modified: Sat May  4 23:20:17 2024, max compression
```

## Comparing `re_ircbot-2.0.1.dev0.tar` & `re_ircbot-2.0.2.dev0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-04 22:47:52.168262 re_ircbot-2.0.1.dev0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1072 2024-05-04 22:47:44.000000 re_ircbot-2.0.1.dev0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14058 2024-05-04 22:47:52.168262 re_ircbot-2.0.1.dev0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13331 2024-05-04 22:47:44.000000 re_ircbot-2.0.1.dev0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-04 22:47:52.164262 re_ircbot-2.0.1.dev0/ircbot/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      125 2024-05-04 22:47:44.000000 re_ircbot-2.0.1.dev0/ircbot/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    53399 2024-05-04 22:47:44.000000 re_ircbot-2.0.1.dev0/ircbot/client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5384 2024-05-04 22:47:44.000000 re_ircbot-2.0.1.dev0/ircbot/dcc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17946 2024-05-04 22:47:44.000000 re_ircbot-2.0.1.dev0/ircbot/hooks.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3027 2024-05-04 22:47:44.000000 re_ircbot-2.0.1.dev0/ircbot/message.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1972 2024-05-04 22:47:44.000000 re_ircbot-2.0.1.dev0/ircbot/shortest_prefix.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11380 2024-05-04 22:47:44.000000 re_ircbot-2.0.1.dev0/ircbot/sqlitedb.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1426 2024-05-04 22:47:44.000000 re_ircbot-2.0.1.dev0/ircbot/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-04 22:47:52.168262 re_ircbot-2.0.1.dev0/re_ircbot.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14058 2024-05-04 22:47:52.000000 re_ircbot-2.0.1.dev0/re_ircbot.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      335 2024-05-04 22:47:52.000000 re_ircbot-2.0.1.dev0/re_ircbot.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-04 22:47:52.000000 re_ircbot-2.0.1.dev0/re_ircbot.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       18 2024-05-04 22:47:52.000000 re_ircbot-2.0.1.dev0/re_ircbot.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-05-04 22:47:52.000000 re_ircbot-2.0.1.dev0/re_ircbot.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-04 22:47:52.168262 re_ircbot-2.0.1.dev0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1869 2024-05-04 22:47:44.000000 re_ircbot-2.0.1.dev0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-04 23:20:17.808748 re_ircbot-2.0.2.dev0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1072 2024-05-04 23:20:09.000000 re_ircbot-2.0.2.dev0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14099 2024-05-04 23:20:17.808748 re_ircbot-2.0.2.dev0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13331 2024-05-04 23:20:09.000000 re_ircbot-2.0.2.dev0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-04 23:20:17.804748 re_ircbot-2.0.2.dev0/ircbot/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      125 2024-05-04 23:20:09.000000 re_ircbot-2.0.2.dev0/ircbot/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    53399 2024-05-04 23:20:09.000000 re_ircbot-2.0.2.dev0/ircbot/client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5384 2024-05-04 23:20:09.000000 re_ircbot-2.0.2.dev0/ircbot/dcc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17833 2024-05-04 23:20:09.000000 re_ircbot-2.0.2.dev0/ircbot/hooks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3039 2024-05-04 23:20:09.000000 re_ircbot-2.0.2.dev0/ircbot/message.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1972 2024-05-04 23:20:09.000000 re_ircbot-2.0.2.dev0/ircbot/shortest_prefix.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11380 2024-05-04 23:20:09.000000 re_ircbot-2.0.2.dev0/ircbot/sqlitedb.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1426 2024-05-04 23:20:09.000000 re_ircbot-2.0.2.dev0/ircbot/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-04 23:20:17.808748 re_ircbot-2.0.2.dev0/re_ircbot.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14099 2024-05-04 23:20:17.000000 re_ircbot-2.0.2.dev0/re_ircbot.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      335 2024-05-04 23:20:17.000000 re_ircbot-2.0.2.dev0/re_ircbot.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-04 23:20:17.000000 re_ircbot-2.0.2.dev0/re_ircbot.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2024-05-04 23:20:17.000000 re_ircbot-2.0.2.dev0/re_ircbot.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-05-04 23:20:17.000000 re_ircbot-2.0.2.dev0/re_ircbot.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-04 23:20:17.808748 re_ircbot-2.0.2.dev0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1869 2024-05-04 23:20:09.000000 re_ircbot-2.0.2.dev0/setup.py
```

### Comparing `re_ircbot-2.0.1.dev0/LICENSE` & `re_ircbot-2.0.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.1.dev0/PKG-INFO` & `re_ircbot-2.0.2.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re-ircbot
-Version: 2.0.1.dev0
+Version: 2.0.2.dev0
 Summary: A simple async irc bot framework with regex command definitions and data permanency
 Home-page: https://github.com/matheusfillipe/ircbot
 Author: Matheus Fillipe
 Author-email: mattf@tilde.club
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Internet
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cachetools==5.3.0
+Requires-Dist: typing_extensions==4.11.0
 
 [![Pypi](https://badge.fury.io/py/re-ircbot.svg)](https://pypi.org/project/re-ircbot/)
 [![Chat with me on irc](https://img.shields.io/badge/-IRC-gray?logo=gitter)](https://mangle.ga/irc)
 
 # re-ircbot, a simple irc bot library
 
 This is a simple irc bot library that uses trio for async callback processing and allows you to
```

### Comparing `re_ircbot-2.0.1.dev0/README.md` & `re_ircbot-2.0.2.dev0/README.md`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.1.dev0/ircbot/client.py` & `re_ircbot-2.0.2.dev0/ircbot/client.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.1.dev0/ircbot/dcc.py` & `re_ircbot-2.0.2.dev0/ircbot/dcc.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.1.dev0/ircbot/hooks.py` & `re_ircbot-2.0.2.dev0/ircbot/hooks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # TODO: Use self typehints instead of class
-from __future__ import annotations
-
 import importlib.util
 import inspect
 import logging
 import os
 import re
 from collections.abc import Callable
 from functools import wraps
 from typing import Awaitable, Literal, TypeAlias, get_args
 
+from typing_extensions import Self
+
 from ircbot.message import Message, Sendable
 from ircbot.shortest_prefix import find_shortest_prefix
 from ircbot.utils import log
 
 
 def md5_file(file):
     import hashlib
@@ -32,18 +32,19 @@
         + opt_close * len(org[len(pref) :])
     )
 
 
 Actions = Literal["privmsg", "ping", "names", "channel", "join", "quit", "part", "dccsend"]
 
 Regex: TypeAlias = str | re.Pattern
-RegexCallback = Callable[[re.Match], Sendable | Awaitable[Sendable | None]]
-RegexWithMessageCallback = Callable[[re.Match, Message], Sendable | Awaitable[Sendable | None]]
-UrlCallback = Callable[[str], Sendable | Awaitable[Sendable | None]]
-ArgCommandCallback = Callable[[re.Match, Message], Sendable | Awaitable[Sendable | None]]
+HookReturn = Sendable | Awaitable[Sendable | None] | None
+RegexCallback = Callable[[re.Match], HookReturn]
+RegexWithMessageCallback = Callable[[re.Match, Message], HookReturn]
+UrlCallback = Callable[[str], HookReturn]
+ArgCommandCallback = Callable[[re.Match, Message], HookReturn]
 
 
 class HookHandler:
     """Defines the behavior of the bot"""
 
     parse_order = False
 
@@ -176,15 +177,15 @@
         return self.regex_cmd_with_messsage(
             f"^{self.command_prefix}{cmd}{f'(?: +({non_space}+))?'*self._command_max_arguments} *$",
             acccept_pms,
             pass_data,
             **kwargs,
         )
 
-    def set_simplify_commands(self, simplify: bool) -> HookHandler:
+    def set_simplify_commands(self, simplify: bool) -> Self:
         self.simplify_arg_commands = simplify
         return self
 
     def arg_command(
         self,
         command: str,
         help: str = "",
@@ -228,48 +229,48 @@
     help_msg_header: list[str] = []
     help_msg: dict[str, str] = {}
     help_msg_bottom: list[str] = []
     commands_help = {}
     help_menu_separator: str = "\n"
     help_on_private: bool = False
 
-    def set_help_menu_separator(self, sep: str) -> HookHandler:
+    def set_help_menu_separator(self, sep: str) -> Self:
         """Sets the separator string between the help commands. If can contain a
         '\n'.
 
         :param sep: separator
         :type sep: str
         """
         self.help_menu_separator = sep
         return self
 
-    def set_help_on_private(self, is_private: bool) -> HookHandler:
+    def set_help_on_private(self, is_private: bool) -> Self:
         """Defines if the help messages should be sent as private messages. This is
         useful to avoide flooding if the bots has many commands.
 
         :param is_private: if true they will be private (default False: display on the current channel)
         """
         self.help_on_private = is_private
         return self
 
-    def set_help_header(self, txt: str) -> HookHandler:
+    def set_help_header(self, txt: str) -> Self:
         """Adds some text to the help message before the command descriptions.
 
         :param txt: Text to display before command descriptions
         :type txt: str
         """
         if isinstance(txt, str):
             self.help_msg_header = [txt]
         elif isinstance(txt, list):
             self.help_msg_header = txt
         else:
             raise BaseException("You must pass wither a list of strings or a string")
         return self
 
-    def set_help_bottom(self, txt: str) -> HookHandler:
+    def set_help_bottom(self, txt: str) -> Self:
         """Adds some text to the help message after the command descriptions.
 
         :param txt: Text to display after command descriptions
         :type txt: str
         """
         if isinstance(txt, str):
             self.help_msg_bottom = [txt]
@@ -371,39 +372,39 @@
                             self.help_menu_separator.join(self.help_msg_header)
                             + self.help_menu_separator.join(self.help_msg.values())
                             + self.help_menu_separator.join(self.help_msg_bottom)
                         )
 
             self.re_command(_reg_word("help", _commands["help"]))(help_menu)
 
-    def set_prefix(self, prefix) -> HookHandler:
+    def set_prefix(self, prefix) -> Self:
         """setPrefix. Sets the prefix for arg commands.
 
         :param prefix: str prefix for commands
         """
         self.command_prefix = prefix
         return self
 
-    def set_single_match(self, _single_match: bool) -> HookHandler:
+    def set_single_match(self, _single_match: bool) -> Self:
         """Defines if there will be only one command handler called. If false all regex and arg_commands will be matched against the user input.
         :param singleMatch: If true there will be only one match per command. Defaults to False (all matches will be called)
         :type singleMatch: bool
         """
         self.single_match = _single_match
         return self
 
-    def set_parser_order(self, top_bottom: bool = True) -> HookHandler:
+    def set_parser_order(self, top_bottom: bool = True) -> Self:
         """setParseOrder.
 
         :param top_bottom: bool -> if True then first defined regex expressions will overwrite last ones. Default is False
         """
         self.parse_order = top_bottom
         return self
 
-    def set_max_arguments(self, n: int) -> HookHandler:
+    def set_max_arguments(self, n: int) -> Self:
         """setMaxArguments.
 
         :param n: number of arguments for callbacks in arg_command decorator
         """
         self._command_max_arguments = n
         return self
```

### Comparing `re_ircbot-2.0.1.dev0/ircbot/message.py` & `re_ircbot-2.0.2.dev0/ircbot/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,8 +100,8 @@
         """__init__.
 
         :param message: Message to send. You can use a message object if you want to change channel or make it a pm.  :param func: Function to call passing the received full message string that the user will reply with. This is useful for building dialogs. This function must either return None, a message to send back (str or IrcBot.Message) or another ReplyIntent. It must receive one argument."""
         self.func = func
         self.message = message
 
 
-Sendable: TypeAlias = str | Message | Color | list[str | Message | Color] | ReplyIntent
+Sendable: TypeAlias = str | Message | Color | list[str] | list[Message] | list[Color] | ReplyIntent
```

### Comparing `re_ircbot-2.0.1.dev0/ircbot/shortest_prefix.py` & `re_ircbot-2.0.2.dev0/ircbot/shortest_prefix.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.1.dev0/ircbot/sqlitedb.py` & `re_ircbot-2.0.2.dev0/ircbot/sqlitedb.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.1.dev0/ircbot/utils.py` & `re_ircbot-2.0.2.dev0/ircbot/utils.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.1.dev0/re_ircbot.egg-info/PKG-INFO` & `re_ircbot-2.0.2.dev0/re_ircbot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re-ircbot
-Version: 2.0.1.dev0
+Version: 2.0.2.dev0
 Summary: A simple async irc bot framework with regex command definitions and data permanency
 Home-page: https://github.com/matheusfillipe/ircbot
 Author: Matheus Fillipe
 Author-email: mattf@tilde.club
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Internet
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cachetools==5.3.0
+Requires-Dist: typing_extensions==4.11.0
 
 [![Pypi](https://badge.fury.io/py/re-ircbot.svg)](https://pypi.org/project/re-ircbot/)
 [![Chat with me on irc](https://img.shields.io/badge/-IRC-gray?logo=gitter)](https://mangle.ga/irc)
 
 # re-ircbot, a simple irc bot library
 
 This is a simple irc bot library that uses trio for async callback processing and allows you to
```

### Comparing `re_ircbot-2.0.1.dev0/setup.py` & `re_ircbot-2.0.2.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 import subprocess
 
 import setuptools
 
-VERSION = "2.0.1-dev"
+VERSION = "2.0.2-dev"
 BRANCH = "v2"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 def requirements():
```

