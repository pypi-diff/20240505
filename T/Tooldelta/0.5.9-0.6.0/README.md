# Comparing `tmp/tooldelta-0.5.9.tar.gz` & `tmp/tooldelta-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tooldelta-0.5.9.tar", max compression
+gzip compressed data, was "tooldelta-0.6.0.tar", max compression
```

## Comparing `tooldelta-0.5.9.tar` & `tooldelta-0.6.0.tar`

### file list

```diff
@@ -1,30 +1,29 @@
--rwxr-xr-x   0        0        0     1497 2024-04-20 14:07:12.823486 tooldelta-0.5.9/LICENSE
--rwxr-xr-x   0        0        0     2504 2024-04-20 14:07:12.823486 tooldelta-0.5.9/README.md
--rwxr-xr-x   0        0        0      973 2024-04-20 14:07:20.891478 tooldelta-0.5.9/pyproject.toml
--rwxr-xr-x   0        0        0      360 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/__init__.py
--rw-r--r--   0        0        0     4979 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/auths.py
--rwxr-xr-x   0        0        0    19961 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/builtins.py
--rwxr-xr-x   0        0        0    12372 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/cfg.py
--rwxr-xr-x   0        0        0    10889 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/color_print.py
--rw-r--r--   0        0        0     1884 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/constants.py
--rw-r--r--   0        0        0     5870 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/fb_conn/fbconn.py
--rwxr-xr-x   0        0        0    30106 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/frame.py
--rwxr-xr-x   0        0        0     4644 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/game_texts.py
--rwxr-xr-x   0        0        0      476 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/get_tool_delta_version.py
--rwxr-xr-x   0        0        0    20525 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/launch_cli.py
--rwxr-xr-x   0        0        0     1534 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/launch_options.py
--rwxr-xr-x   0        0        0     2425 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/logger.py
--rw-r--r--   0        0        0    30151 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/neo_conn.py
--rwxr-xr-x   0        0        0     1292 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/packets.py
--rwxr-xr-x   0        0        0    15769 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/plugin_load/PluginGroup.py
--rwxr-xr-x   0        0        0     3118 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/plugin_load/__init__.py
--rwxr-xr-x   0        0        0     7341 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/plugin_load/classic_plugin/__init__.py
--rwxr-xr-x   0        0        0      450 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/plugin_load/funcs.py
--rwxr-xr-x   0        0        0     9975 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/plugin_load/injected_plugin/__init__.py
--rwxr-xr-x   0        0        0     9146 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/plugin_load/injected_plugin/movent.py
--rwxr-xr-x   0        0        0    16934 2024-04-20 14:07:12.831486 tooldelta-0.5.9/tooldelta/plugin_manager.py
--rwxr-xr-x   0        0        0    16769 2024-04-20 14:07:12.831486 tooldelta-0.5.9/tooldelta/plugin_market.py
--rw-r--r--   0        0        0     1784 2024-04-20 14:07:12.831486 tooldelta-0.5.9/tooldelta/starter.py
--rwxr-xr-x   0        0        0      808 2024-04-20 14:07:12.831486 tooldelta-0.5.9/tooldelta/sys_args.py
--rwxr-xr-x   0        0        0     9071 2024-04-20 14:07:12.831486 tooldelta-0.5.9/tooldelta/urlmethod.py
--rw-r--r--   0        0        0     3743 1970-01-01 00:00:00.000000 tooldelta-0.5.9/PKG-INFO
+-rwxr-xr-x   0        0        0     1497 2024-05-05 15:13:40.927657 tooldelta-0.6.0/LICENSE
+-rwxr-xr-x   0        0        0     2504 2024-05-05 15:13:40.927657 tooldelta-0.6.0/README.md
+-rw-r--r--   0        0        0      891 2024-05-05 15:13:50.547635 tooldelta-0.6.0/pyproject.toml
+-rwxr-xr-x   0        0        0      618 2024-05-05 15:13:40.927657 tooldelta-0.6.0/tooldelta/__init__.py
+-rw-r--r--   0        0        0     4979 2024-05-05 15:13:40.927657 tooldelta-0.6.0/tooldelta/auths.py
+-rwxr-xr-x   0        0        0    12372 2024-05-05 15:13:40.927657 tooldelta-0.6.0/tooldelta/cfg.py
+-rwxr-xr-x   0        0        0    10889 2024-05-05 15:13:40.927657 tooldelta-0.6.0/tooldelta/color_print.py
+-rw-r--r--   0        0        0     1885 2024-05-05 15:13:40.927657 tooldelta-0.6.0/tooldelta/constants.py
+-rwxr-xr-x   0        0        0    34694 2024-05-05 15:13:40.927657 tooldelta-0.6.0/tooldelta/frame.py
+-rwxr-xr-x   0        0        0    13149 2024-05-05 15:13:40.927657 tooldelta-0.6.0/tooldelta/game_texts.py
+-rwxr-xr-x   0        0        0      476 2024-05-05 15:13:40.927657 tooldelta-0.6.0/tooldelta/get_tool_delta_version.py
+-rwxr-xr-x   0        0        0    23741 2024-05-05 15:13:40.927657 tooldelta-0.6.0/tooldelta/launch_cli.py
+-rwxr-xr-x   0        0        0     1832 2024-05-05 15:13:40.931657 tooldelta-0.6.0/tooldelta/launch_options.py
+-rwxr-xr-x   0        0        0     2425 2024-05-05 15:13:40.931657 tooldelta-0.6.0/tooldelta/logger.py
+-rw-r--r--   0        0        0    29752 2024-05-05 15:13:40.931657 tooldelta-0.6.0/tooldelta/neo_conn.py
+-rwxr-xr-x   0        0        0     1295 2024-05-05 15:13:40.931657 tooldelta-0.6.0/tooldelta/packets.py
+-rwxr-xr-x   0        0        0    16965 2024-05-05 15:13:40.931657 tooldelta-0.6.0/tooldelta/plugin_load/PluginGroup.py
+-rwxr-xr-x   0        0        0     3118 2024-05-05 15:13:40.931657 tooldelta-0.6.0/tooldelta/plugin_load/__init__.py
+-rwxr-xr-x   0        0        0     7792 2024-05-05 15:13:40.931657 tooldelta-0.6.0/tooldelta/plugin_load/classic_plugin/__init__.py
+-rwxr-xr-x   0        0        0     9975 2024-05-05 15:13:40.931657 tooldelta-0.6.0/tooldelta/plugin_load/injected_plugin/__init__.py
+-rwxr-xr-x   0        0        0     6318 2024-05-05 15:13:40.931657 tooldelta-0.6.0/tooldelta/plugin_load/injected_plugin/movent.py
+-rw-r--r--   0        0        0     7025 2024-05-05 15:13:40.931657 tooldelta-0.6.0/tooldelta/plugin_load/utils.py
+-rwxr-xr-x   0        0        0    17005 2024-05-05 15:13:40.931657 tooldelta-0.6.0/tooldelta/plugin_manager.py
+-rwxr-xr-x   0        0        0    16754 2024-05-05 15:13:40.931657 tooldelta-0.6.0/tooldelta/plugin_market.py
+-rw-r--r--   0        0        0     1932 2024-05-05 15:13:40.931657 tooldelta-0.6.0/tooldelta/starter.py
+-rwxr-xr-x   0        0        0     1110 2024-05-05 15:13:40.931657 tooldelta-0.6.0/tooldelta/sys_args.py
+-rwxr-xr-x   0        0        0     9215 2024-05-05 15:13:40.931657 tooldelta-0.6.0/tooldelta/urlmethod.py
+-rw-r--r--   0        0        0    20711 2024-05-05 15:13:40.931657 tooldelta-0.6.0/tooldelta/utils.py
+-rw-r--r--   0        0        0     3592 1970-01-01 00:00:00.000000 tooldelta-0.6.0/PKG-INFO
```

### Comparing `tooldelta-0.5.9/LICENSE` & `tooldelta-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.9/README.md` & `tooldelta-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.9/pyproject.toml` & `tooldelta-0.6.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 [tool.poetry]
 name = "Tooldelta"
-version = "0.5.9" # This field is automatically set to the value in the version file
+version = "0.6.0" # This field is automatically set to the value in the version file
 description = "Plugin Loader for NeteaseRentalServer on Panel"
 authors = ["SuperScript-PRC"]
 license = ""
 
 readme = "README.md"
 homepage = "https://github.com/SuperScript-PRC/ToolDelta"
 repository = "https://github.com/SuperScript-PRC/ToolDelta"
 
 # Please don't change this manually, your changes may invalidate other people's package management, use poetry to make changes!
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 psutil = "5.9.8"
 requests = "2.31.0"
-nbt = "1.5.1"
-qrcode = "7.4.2"
-pymysql = "1.1.0"
-websockets = "12.0"
 ujson = "5.9.0"
-rich = "13.7.0"
 colorama = "^0.4.6"
 pillow = "^10.2.0"
 shellescape = "^3.8.1"
 pyspeedtest = "1.2.7"
-tqdm = "4.66.2"
 aiohttp = "^3.9.3"
 python-socketio = "5.11.1"
 flask = "^3.0.2"
 mido = "^1.3.2"
 websocket-client = "^1.7.0"
+fcwslib = "^3.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tooldelta-0.5.9/tooldelta/auths.py` & `tooldelta-0.6.0/tooldelta/auths.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.9/tooldelta/builtins.py` & `tooldelta-0.6.0/tooldelta/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,21 +20,22 @@
 from typing import Any, Callable, Dict, List, Tuple, Optional
 import ctypes
 import threading
 import traceback
 import json as rjson
 import ujson as json
 from .color_print import Print
+from .constants import TOOLDELTA_PLUGIN_DATA_DIR
 
 event_pool = {"tmpjson_save": threading.Event()}
 event_flags_pool = {"tmpjson_save": True}
-threads_list: list["Builtins.createThread"] = []
+threads_list: list["Utils.createThread"] = []
 
 
-class Builtins:
+class Utils:
     """提供了一些实用方法的类"""
     class ThreadExit(SystemExit):
         """线程退出."""
 
     class ClassicThread(threading.Thread):
         """简化ToolDelta子线程创建的threading.Thread的子类."""
 
@@ -57,15 +58,15 @@
             self._thread_id = None
 
         def run(self) -> None:
             """线程运行方法"""
             threads_list.append(self)
             try:
                 self.func(*self.all_args[0], **self.all_args[1])
-            except (Builtins.ThreadExit, SystemExit):
+            except (Utils.ThreadExit, SystemExit):
                 pass
             except Exception:
                 Print.print_err(
                     f"线程 {self.usage or self.func.__name__} 出错:\n" + traceback.format_exc())
             finally:
                 threads_list.remove(self)
 
@@ -115,15 +116,15 @@
             Raises:
                 err: 文件不存在时
             """
             if path in jsonPathTmp:
                 return
             try:
                 with open(path, 'r', encoding='utf-8') as file:
-                    js = Builtins.SimpleJsonDataReader.SafeJsonLoad(file)
+                    js = Utils.SimpleJsonDataReader.SafeJsonLoad(file)
             except FileNotFoundError as err:
                 if not needFileExists:
                     js = None
                 else:
                     raise err from None
             jsonPathTmp[path] = [False, js]
 
@@ -139,21 +140,21 @@
             Returns:
                 bool: 存盘是否成功
             """
             if jsonPathTmp.get(path) is not None:
                 isChanged, dat = jsonPathTmp[path]
                 if isChanged:
                     with open(path, 'w', encoding='utf-8') as file:
-                        Builtins.SimpleJsonDataReader.SafeJsonDump(dat, file)
+                        Utils.SimpleJsonDataReader.SafeJsonDump(dat, file)
                 del jsonPathTmp[path]
                 return True
             return False
 
         @staticmethod
-        def read(path: str) -> list[Any] | dict[Any, Any] | Any:
+        def read(path: str) -> Any:
             """对缓存区的该虚拟路径的文件进行读操作, 返回一个深拷贝的JSON对象
 
             Args:
                 path (str): 文件的虚拟路径
 
             Raises:
                 Exception: json路径未初始化, 不能进行读取和写入操作
@@ -210,31 +211,31 @@
                 timeout (int, optional): 多久没有再进行读取操作时卸载缓存
 
             Returns:
                 Any: 该虚拟路径的JSON
             """
             if path not in jsonUnloadPathTmp and not path in jsonPathTmp:
                 jsonUnloadPathTmp[path] = timeout + int(time.time())
-                Builtins.TMPJson.loadPathJson(path, needFileExists)
-            return Builtins.TMPJson.read(path)
+                Utils.TMPJson.loadPathJson(path, needFileExists)
+            return Utils.TMPJson.read(path)
 
         @staticmethod
         def write_as_tmp(path: str, obj: Any, needFileExists: bool = True, timeout: int = 60) -> None:
             """写入json文件并将其从磁盘加载到缓存区, 以便一段时间内能快速读写.
 
             Args:
                 path (str): 作为文件的磁盘内路径的同时也会作为在缓存区的虚拟路径
                 obj (Any): 任何合法的JSON类型 例如 dict/list/str/bool/int/float
                 needFileExists (bool, optional): 默认为 True, 为 False 时, 若文件路径不存在, 就会自动创建一个文件, 且写入默认值null
                 timeout (int, optional): 多久没有再进行读取操作时卸载缓存
             """
             if path not in jsonUnloadPathTmp and not path in jsonPathTmp:
                 jsonUnloadPathTmp[path] = timeout + int(time.time())
-                Builtins.TMPJson.loadPathJson(path, needFileExists)
-            Builtins.TMPJson.write(path, obj)
+                Utils.TMPJson.loadPathJson(path, needFileExists)
+            Utils.TMPJson.write(path, obj)
 
         @staticmethod
         def cancel_change(path: str) -> None:
             """取消缓存json所做的更改, 非必要情况请勿调用, 你不知道什么时候会自动保存所做更改"""
             jsonPathTmp[path][0] = False
 
         @staticmethod
@@ -284,35 +285,35 @@
 
             Args:
                 plugin_name (str): 插件名
                 file (str): 文件名
                 default (dict, optional): 默认值, 若文件不存在则会写入这个默认值
 
             Raises:
-                Builtins.SimpleJsonDataReader.DataReadError: 读取数据时发生错误
+                Utils.SimpleJsonDataReader.DataReadError: 读取数据时发生错误
                 err: 读取文件路径时发生错误
 
             Returns:
                 dict | list: JSON对象
             """
             if file.endswith(".json"):
                 file = file[:-5]
-            filepath = os.path.join("插件数据文件", plugin_name, f"{file}.json")
-            os.makedirs(os.path.join("插件数据文件", plugin_name), exist_ok=True)
+            filepath = os.path.join(TOOLDELTA_PLUGIN_DATA_DIR, plugin_name, f"{file}.json")
+            os.makedirs(os.path.join(TOOLDELTA_PLUGIN_DATA_DIR, plugin_name), exist_ok=True)
             try:
                 if default is not None and not os.path.isfile(filepath):
                     with open(filepath, "w", encoding="utf-8") as f:
-                        Builtins.SimpleJsonDataReader.SafeJsonDump(default, f)
+                        Utils.SimpleJsonDataReader.SafeJsonDump(default, f)
                     return default
                 with open(filepath, "r", encoding="utf-8") as f:
-                    res = Builtins.SimpleJsonDataReader.SafeJsonLoad(f)
+                    res = Utils.SimpleJsonDataReader.SafeJsonLoad(f)
                 return res
             except rjson.JSONDecodeError as err:
                 # 判断是否有msg.doc.pos属性
-                raise Builtins.SimpleJsonDataReader.DataReadError(
+                raise Utils.SimpleJsonDataReader.DataReadError(
                     err.msg, err.doc, err.pos
                 )
             except Exception as err:
                 Print.print_err(f"读文件路径 {filepath} 发生错误")
                 raise err
 
         @staticmethod
@@ -320,20 +321,20 @@
             """将一个json对象写入插件数据文件夹, 会自动创建文件夹和文件.
 
             Args:
                 plugin_name (str): 插件名
                 file (str): 文件名
                 obj (str | dict[Any, Any] | list[Any]): JSON对象
             """
-            os.makedirs(f"插件数据文件/{plugin_name}", exist_ok=True)
-            with open(f"插件数据文件/{plugin_name}/{file}.json", "w", encoding="utf-8") as f:
-                Builtins.SimpleJsonDataReader.SafeJsonDump(obj, f)
+            os.makedirs(f"{TOOLDELTA_PLUGIN_DATA_DIR}/{plugin_name}", exist_ok=True)
+            with open(f"{TOOLDELTA_PLUGIN_DATA_DIR}/{plugin_name}/{file}.json", "w", encoding="utf-8") as f:
+                Utils.SimpleJsonDataReader.SafeJsonDump(obj, f)
 
     @staticmethod
-    def get_threads_list() -> list["Builtins.createThread"]:
+    def get_threads_list() -> list["Utils.createThread"]:
         "返回使用 createThread 创建的全线程列表."
         return threads_list
 
     @staticmethod
     def SimpleFmt(kw: Dict[str, Any], *args: str) -> str:
         """
         快速将字符串内按照给出的dict的键值对替换掉内容.
@@ -341,15 +342,15 @@
         参数:
             kw: Dict[str, Any], 键值对应替换的内容
             *args: str, 需要被替换的字符串
 
         示例:
             >>> my_color = "red"; my_item = "apple"
             >>> kw = {"[颜色]": my_color, "[物品]": my_item}
-            >>> Builtins.SimpleFmt(kw, "I like [颜色] [物品].")
+            >>> Utils.SimpleFmt(kw, "I like [颜色] [物品].")
             I like red apple.
         """
         __sub = args[0]
         for k, v in kw.items():
             if k in __sub:
                 __sub = __sub.replace(k, str(v))
         return __sub
@@ -359,27 +360,45 @@
         """
         相当于 assert cond, 但是可以自定义引发的异常的类型
         """
         if not cond:
             raise exc
 
     @staticmethod
-    def thread_func(func: Any) -> Any:
+    def thread_func(func_or_name: Callable | str) -> Any:
         """
         在事件方法可能执行较久会造成堵塞时使用, 方便快捷地创建一个新线程, 例如:
 
-        @Builtins.run_as_new_thread
+        @Utils.thread_func
+        def on_inject(self):
+            ...
+        或者:
+        @Utils.thread_func("一个会卡一分钟的线程")
         def on_inject(self):
             ...
         """
-
-        def thread_fun(*args: Tuple, **kwargs: Any) -> None:
-            Builtins.createThread(func, usage="简易线程方法:" +
-                                  func.__name__, args=args, **kwargs)
-
+        if isinstance(func_or_name, str):
+            def _recv_func(func: Callable):
+                def thread_fun(*args: Tuple, **kwargs: Any) -> None:
+                    Utils.createThread(
+                        func,
+                        usage=func_or_name,
+                        args=args,
+                        **kwargs
+                )
+                return thread_fun
+            return _recv_func
+        else:
+            def thread_fun(*args: Tuple, **kwargs: Any) -> None:
+                Utils.createThread(
+                    func_or_name,
+                    usage="简易线程方法:" + func_or_name.__name__,
+                    args=args,
+                    **kwargs
+                )
         return thread_fun
 
     run_as_new_thread = thread_func
     new_thread = thread_func
 
     @staticmethod
     def try_int(arg: Any) -> Optional[int]:
@@ -445,15 +464,15 @@
             func: function, 线程方法
             exc_cb: function, 若玩家已处于一个对话中, 则向方法exc_cb传参并调用它: player(玩家名)
             args: tuple, 线程方法的参数组
             kwargs: dict, 线程方法的关键词参数组
         """
         if kwargs is None:
             kwargs = {}
-        Builtins.createThread(
+        Utils.createThread(
             _dialogue_thread_run, args=(player, func, exc_cb, args, kwargs)
         )
 
     @staticmethod
     def fuzzy_match(lst: List[str], sub: str) -> List[str]:
         """
         模糊匹配列表内的字符串, 可以用在诸如模糊匹配玩家名的用途
@@ -503,40 +522,41 @@
     while 1:
         evt.wait(2)
         secs += 2
         if secs >= 60:
             secs = 0
             for k, (isChanged, dat) in jsonPathTmp.copy().items():
                 if isChanged:
-                    Builtins.SimpleJsonDataReader.SafeJsonDump(dat, k)
+                    Utils.SimpleJsonDataReader.SafeJsonDump(dat, k)
                     jsonPathTmp[k][0] = False
         for k, v in jsonUnloadPathTmp.copy().items():
             if time.time() - v > 0:
-                Builtins.TMPJson.unloadPathJson(k)
+                Utils.TMPJson.unloadPathJson(k)
                 del jsonUnloadPathTmp[k]
         if not event_flags_pool["tmpjson_save"]:
             return
 
 
 def tmpjson_save_thread() -> None:
     """JSON缓存文件定时保存"""
-    Builtins.createThread(_tmpjson_save_thread, usage="JSON缓存文件定时保存")
+    Utils.createThread(_tmpjson_save_thread, usage="JSON缓存文件定时保存")
 
 
 def _dialogue_thread_run(player, func, exc_cb, args, kwargs):
-    if not Builtins.player_in_dialogue(player):
-        Builtins.add_in_dialogue_player(player)
+    "启动专用的玩家会话线程, 可免除当玩家在对话线程时又试图再创建一个对话线程的问题"
+    if not Utils.player_in_dialogue(player):
+        Utils.add_in_dialogue_player(player)
     else:
         if exc_cb is not None:
             exc_cb(player)
         return
     try:
         func(*args, **kwargs)
     except Exception:
         Print.print_err(f"玩家{player}的会话线程 出现问题:")
         Print.print_err(traceback.format_exc())
-    Builtins.remove_in_dialogue_player(player)
+    Utils.remove_in_dialogue_player(player)
 
 
 jsonPathTmp = {}
 in_dialogue_list = []
 jsonUnloadPathTmp = {}
```

### Comparing `tooldelta-0.5.9/tooldelta/cfg.py` & `tooldelta-0.6.0/tooldelta/cfg.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.9/tooldelta/color_print.py` & `tooldelta-0.6.0/tooldelta/color_print.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.9/tooldelta/frame.py` & `tooldelta-0.6.0/tooldelta/frame.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """
+ToolDelta基本框架
+
 整个系统由三个部分组成
     Frame: 负责整个 ToolDelta 的基本框架运行
     GameCtrl: 负责对接游戏
         - Launchers: 负责将不同启动器的游戏接口统一成固定的接口, 供插件在多平台游戏接口运行(FastBuilder External, NeOmega, (TLSP, etc.))
+    PluginGroup: 负责对插件进行统一管理
 """
 
 import os
 import sys
 import time
 import getpass
 import traceback
@@ -17,64 +20,65 @@
 import tooldelta
 from tooldelta import (
     auths,
     constants,
     plugin_market,
 )
 from .constants import PRG_NAME
-from .builtins import Builtins, safe_close
+from .utils import Utils, safe_close
+from .plugin_load.injected_plugin import safe_jump
 from .get_tool_delta_version import get_tool_delta_version
 from .color_print import Print
 from .cfg import Cfg
 from .logger import publicLogger
-from .game_texts import GameTextsLoader
+from .game_texts import GameTextsLoader, GameTextsHandle
 from .urlmethod import if_token, fbtokenFix
 from .sys_args import sys_args_to_dict
 from .launch_cli import (
     FrameNeOmg,
     FrameNeOmgRemote,
     SysStatus,
 )
 
 from .packets import PacketIDS
-from .plugin_load.injected_plugin import (
-    execute_death_message,
-    execute_init,
-    execute_player_join,
-    execute_player_prejoin,
-    execute_player_left,
-    execute_player_message,
-    execute_repeat,
-    safe_jump,
-)
 
 sys_args_dict = sys_args_to_dict(sys.argv)
 VERSION = get_tool_delta_version()
 Config = Cfg()
+
 if TYPE_CHECKING:
     from .plugin_load.PluginGroup import PluginGroup
 
+LAUNCHERS: list[
+    tuple[str, type[FrameNeOmg | FrameNeOmgRemote]]
+] = [
+    ("NeOmega 框架 (NeOmega模式, 租赁服适应性强, 推荐)", FrameNeOmg),
+    (
+        "NeOmega 框架 (NeOmega连接模式, 需要先启动对应的neOmega接入点)",
+        FrameNeOmgRemote,
+    ),
+]
 
 class Frame:
-    """系统框架"""
+    """ToolDelta主框架"""
 
     class FrameBasic:
         """系统基本信息"""
         system_version = VERSION
         max_connect_fb_time = 60
         connect_fb_start_time = time.time()
         data_path = "插件数据文件/"
 
     class SystemVersionException(ImportError):
         """系统版本异常"""
         msg: str
 
     def __init__(self) -> None:
         """初始化"""
-        self.ClassicThread = self.createThread = Builtins.createThread
+        self.createThread = Utils.createThread
         self.sys_data = self.FrameBasic()
         self.serverNumber: int = 0
         self.serverPasswd: str = ""
         self.launchMode: int = 0
         self.consoleMenu = []
         self.on_plugin_err = staticmethod(
             lambda name, _, err: Print.print_err(f"插件 <{name}> 出现问题: \n{err}")
@@ -95,15 +99,15 @@
             self.serverNumber = cfgs["服务器号"]
             self.serverPasswd = cfgs["密码"]
             self.launchMode = cfgs["启动器启动模式(请不要手动更改此项, 改为0可重置)"]
             self.is_mir = cfgs["是否使用github镜像"]
             self.plugin_market_url = cfgs["插件市场源"]
             auth_server = cfgs["验证服务器地址(更换时记得更改fbtoken)"]
             publicLogger.switch_logger(cfgs["是否记录日志"])
-            if self.launchMode != 0 and self.launchMode not in range(1, len(constants.LAUNCHERS) + 1):
+            if self.launchMode != 0 and self.launchMode not in range(1, len(LAUNCHERS) + 1):
                 raise Config.ConfigError("你不该随意修改启动器模式, 现在赶紧把它改回0吧")
         except Config.ConfigError as err:
             # 配置文件有误
             r = self.upgrade_cfg()
             if r:
                 Print.print_war("配置文件未升级, 已自动升级, 请重启 ToolDelta")
             else:
@@ -128,15 +132,14 @@
                     std["密码"] = int(self.serverPasswd)
                     Config.default_cfg("ToolDelta基本配置.json", std, True)
                     Print.print_suc("登录配置设置成功")
                     cfgs = std
                     break
                 except Exception:
                     Print.print_err("输入有误， 租赁服号和密码应当是纯数字")
-
         auth_servers = constants.AUTH_SERVERS
         if auth_server == "":
             Print.print_inf("选择 ToolDelta机器人账号 使用的验证服务器:")
             for i, (auth_server_name, _) in enumerate(auth_servers):
                 Print.print_inf(f" {i + 1} - {auth_server_name}")
             Print.print_inf(
                 "§cNOTE: 使用的机器人账号是在哪里获取的就选择哪一个验证服务器, 不能混用"
@@ -181,43 +184,119 @@
                             Print.print_err("暂无法登录该验证服务器")
                             raise SystemExit
                     with open("fbtoken", "w", encoding="utf-8") as f:
                         f.write(token)
                 except requests.exceptions.RequestException as e:
                     Print.print_err(f"登录失败，原因：{e}\n正在切换至Token登录")
             if_token()
-        launchers = constants.LAUNCHERS
+
         if self.launchMode == 0:
             Print.print_inf("请选择启动器启动模式(之后可在ToolDelta启动配置更改):")
-            for i, (launcher_name, _) in enumerate(launchers):
+            for i, (launcher_name, _) in enumerate(LAUNCHERS):
                 Print.print_inf(f" {i + 1} - {launcher_name}")
             while 1:
                 try:
                     ch = int(input(Print.fmt_info("请选择: ", "§f 输入 ")))
-                    if ch not in range(1, len(launchers) + 1):
+                    if ch not in range(1, len(LAUNCHERS) + 1):
                         raise ValueError
                     cfgs["启动器启动模式(请不要手动更改此项, 改为0可重置)"] = ch
                     break
                 except ValueError:
                     Print.print_err("输入不合法, 或者是不在范围内, 请重新输入")
             Config.default_cfg("ToolDelta基本配置.json", cfgs, True)
         # 修复fbtoken
         fbtokenFix()
         with open("fbtoken", "r", encoding="utf-8") as f:
             fbtoken = f.read()
-        self.launcher = launchers[
+        self.launcher = LAUNCHERS[
             cfgs["启动器启动模式(请不要手动更改此项, 改为0可重置)"] - 1
         ][1](
             self.serverNumber,
             self.serverPasswd,
             fbtoken,
             auth_server,
         )
 
     @staticmethod
+    def change_config():
+        "修改配置文件"
+        try:
+            old_cfg = Config.get_cfg("ToolDelta基本配置.json", constants.LAUNCH_CFG_STD)
+        except FileNotFoundError:
+            Print.clean_print("§c未初始化配置文件, 无法进行修改")
+            return
+        except Config.ConfigError as err:
+            Print.print_err(f"配置文件损坏: {err}")
+            return
+        if (old_cfg['启动器启动模式(请不要手动更改此项, 改为0可重置)'] - 1) not in range(0, 2):
+            Print.print_err(f"配置文件损坏: 启动模式错误: {old_cfg['启动器启动模式(请不要手动更改此项, 改为0可重置)'] - 1}")
+            return
+        while 1:
+            md = (
+                "NeOmega 框架 (NeOmega模式, 租赁服适应性强, 推荐)",
+                "NeOmega 框架 (NeOmega连接模式, 需要先启动对应的neOmega接入点)",
+            )
+            Print.clean_print("§b现有配置项如下:")
+            Print.clean_print(f" 1. 租赁服号: {old_cfg['服务器号']}")
+            Print.clean_print(f" 2. 密码: <已隐藏>")
+            Print.clean_print(f" 3. 启动器启动模式: {md[old_cfg['启动器启动模式(请不要手动更改此项, 改为0可重置)'] - 1]}")
+            Print.clean_print(f" 4. 是否记录日志: {old_cfg['是否记录日志']}")
+            Print.clean_print(f" 5. 验证服务器地址: {old_cfg['验证服务器地址(更换时记得更改fbtoken)']}")
+            Print.clean_print(f"    §a直接回车: 保存并退出")
+            resp = input(Print.clean_fmt("§6输入序号可修改配置项(0~4): ")).strip()
+            if resp == "":
+                Config.default_cfg("ToolDelta基本配置.json", old_cfg, True)
+                Print.clean_print("§a配置已保存!")
+                return
+            match resp:
+                case "1":
+                    n = Utils.try_int(input(Print.clean_fmt("§b请输入租赁服号: ")))
+                    if n is None:
+                        input(Print.clean_fmt("§c不是合法租赁服号, 回车键继续"))
+                        continue
+                    old_cfg["服务器号"] = n
+                    input(Print.clean_fmt(f"§f新的租赁服号: §a{n}§f, 回车键继续"))
+                case "2":
+                    n = getpass.getpass(Print.clean_fmt("§b请输入租赁服密码(自动隐藏): "))
+                    if len(n) != 6:
+                        input(Print.clean_fmt("§c不是合法租赁服六位数密码, 回车键继续"))
+                        continue
+                    n = Utils.try_int(n)
+                    if n is None:
+                        input(Print.clean_fmt("§c不是合法租赁服密码, 回车键继续"))
+                        continue
+                    old_cfg["密码"] = n
+                    input(Print.clean_fmt(f"§f新的租赁服密码: §a******§f, 回车键继续"))
+                case "3":
+                    Print.print_inf("选择启动器启动模式(之后可在ToolDelta启动配置更改):")
+                    for i, (launcher_name, _) in enumerate(LAUNCHERS):
+                        Print.print_inf(f" {i + 1} - {launcher_name}")
+                    while 1:
+                        try:
+                            ch = int(input(Print.clean_fmt("请选择: ")))
+                            if ch not in range(1, len(LAUNCHERS) + 1):
+                                raise ValueError
+                            old_cfg["启动器启动模式(请不要手动更改此项, 改为0可重置)"] = ch
+                            break
+                        except ValueError:
+                            Print.print_err("输入不合法, 或者是不在范围内, 请重新输入")
+                            continue
+                    input(Print.clean_fmt(f"§a已选择启动器启动模式: §f{md[old_cfg['启动器启动模式(请不要手动更改此项, 改为0可重置)'] - 1]}, 回车键继续"))
+                case "4":
+                    old_cfg['是否记录日志'] = [True, False][old_cfg['是否记录日志']]
+                    input(Print.clean_fmt(f"日志记录模式已改为: {['§c关闭', '§a开启'][old_cfg['是否记录日志']]}, 回车键继续"))
+                case "5":
+                    n = input(Print.clean_fmt("§b请输入验证服务器地址: "))
+                    if not n.startswith("http://") and not n.startswith("https://"):
+                        input(Print.clean_fmt("§c不合法URL地址, 回车键继续"))
+                        continue
+                    old_cfg['验证服务器地址(更换时记得更改fbtoken)'] = n
+                    input(Print.clean_fmt(f"§a验证服务器已设置, 回车键继续"))
+
+    @staticmethod
     def upgrade_cfg() -> bool:
         """升级配置文件
 
         Returns:
             bool: 是否升级了配置文件
         """
         old_cfg = Config.get_cfg("ToolDelta基本配置.json", {})
@@ -257,28 +336,20 @@
         Print.print_suc(
             f"成功载入 §f{plugins.normal_plugin_loaded_num}§a 个组合式插件, §f{plugins.injected_plugin_loaded_num}§a 个注入式插件"
         )
 
     @staticmethod
     def basic_operation():
         """初始化文件夹"""
-        if os.path.isdir("插件文件/ToolDelta组合式插件"):
-            os.rename(
-                "插件文件/ToolDelta组合式插件",
-                f"插件文件/{constants.TOOLDELTA_CLASSIC_PLUGIN}",
-            )
         os.makedirs(
             f"插件文件/{constants.TOOLDELTA_CLASSIC_PLUGIN}", exist_ok=True)
         os.makedirs(
             f"插件文件/{constants.TOOLDELTA_INJECTED_PLUGIN}", exist_ok=True)
         os.makedirs("插件配置文件", exist_ok=True)
-        os.makedirs("tooldelta/fb_conn", exist_ok=True)
         os.makedirs("tooldelta/neo_libs", exist_ok=True)
-        os.makedirs("插件数据文件/status", exist_ok=True)
-        os.makedirs("插件数据文件/players", exist_ok=True)
         os.makedirs("插件数据文件/game_texts", exist_ok=True)
 
     def add_console_cmd_trigger(
         self,
         triggers: list[str],
         arg_hint: str | None,
         usage: str,
@@ -322,15 +393,15 @@
                 return
             try:
                 return func(rsp_arg) or 0
             except Exception:
                 Print.print_err(f"控制台指令出错： {traceback.format_exc()}")
                 return 0
 
-        @Builtins.thread_func
+        @Utils.thread_func
         def _execute_mc_command_and_get_callback(cmd: str) -> None:
             """执行Minecraft指令并获取回调结果。
 
             Args:
                 cmd (str): 要执行的Minecraft指令。
 
             Raises:
@@ -342,21 +413,22 @@
                 if isinstance(result, type(None)):
                     raise ValueError("指令执行失败")
                 if (result.OutputMessages[0].Message == "commands.generic.syntax") | (
                     result.OutputMessages[0].Message == "commands.generic.unknown"
                 ):
                     Print.print_err(f'未知的MC指令， 可能是指令格式有误： "{cmd}"')
                 else:
-                    jso = json.dumps(
-                        result.as_dict["OutputMessages"], indent=2, ensure_ascii=False
-                    )
+                    mjon = self.link_game_ctrl.Game_Data_Handle.Handle_Text_Class1(result.as_dict["OutputMessages"])
                     if not result.SuccessCount:
-                        Print.print_war(f"指令执行失败: \n{jso}")
+                        print_str = "指令执行失败: " + " ".join(mjon); Print.print_war(print_str)
+                        Print.print_war(result.as_dict["OutputMessages"])
                     else:
-                        Print.print_suc(f"指令执行成功: \n{jso}")
+                        print_str = "指令执行成功: " + " ".join(mjon); Print.print_suc(print_str)
+                        Print.print_suc(result.as_dict["OutputMessages"])
+
             except IndexError as exec_err:
                 if isinstance(result, type(None)):
                     raise ValueError("指令执行失败") from exec_err
                 if result.SuccessCount:
                     Print.print_suc(
                         f"指令执行成功: \n{json.dumps(result.as_dict['OutputMessages'], indent=2, ensure_ascii=False)}"
                     )
@@ -422,14 +494,16 @@
                     else:
                         for tri in triggers:
                             if rsp.startswith(tri):
                                 res = _try_execute_console_cmd(
                                     func, rsp, 1, tri)
                                 if res == -1:
                                     return
+                if res != 0 and rsp:
+                    self.link_game_ctrl.say_to('@a', f'[§bToolDelta控制台§r] §3{rsp}§r')
 
         self.createThread(_console_cmd_thread, usage="控制台指令")
 
     def system_exit(self) -> None:
         """系统退出"""
         asyncio.run(safe_jump())
         exit_status_code = getattr(self.launcher, "secret_exit_key", "null")
@@ -494,27 +568,29 @@
         """初始化
 
         Args:
             frame (Frame): 继承Frame的对象
         """
         frame.basic_operation()
         self.Game_Data = GameTextsLoader().game_texts_data
+        self.Game_Data_Handle = GameTextsHandle(self.Game_Data)
         self.linked_frame = frame
         self.players_uuid = {}
         self.allplayers = []
         self.bot_name = ""
         self.linked_frame: Frame
         self.pkt_unique_id: int = 0
         self.pkt_cache: list = []
         self.require_listen_packets = {9, 79, 63}
         self.store_uuid_pkt: dict[str, str] | None = None
         self.launcher = self.linked_frame.launcher
         if isinstance(self.launcher, (FrameNeOmgRemote, FrameNeOmg)):
-            self.launcher.packet_handler = lambda pckType, pck: Builtins.createThread(
+            self.launcher.packet_handler = lambda pckType, pck: Utils.createThread(
                 self.packet_handler, (pckType, pck), usage="数据包处理")
+        # 初始化基本函数
         self.sendcmd = self.launcher.sendcmd
         self.sendwscmd = self.launcher.sendwscmd
         self.sendwocmd = self.launcher.sendwocmd
         self.sendPacket = self.launcher.sendPacket
         if isinstance(self.linked_frame.launcher, FrameNeOmg):
             self.requireUUIDPacket = False
         else:
@@ -533,15 +609,15 @@
         """添加监听的数据包
 
         Args:
             pkt (int): 数据包ID
         """
         self.require_listen_packets.add(pkt)
 
-    @Builtins.run_as_new_thread
+    @Utils.run_as_new_thread
     def packet_handler(self, pkt_type: int, pkt: dict) -> None:
         """数据包处理分发任务函数
 
         Args:
             pkt_type (int): 数据包类型
             pkt (dict): 数据包内容
         """
@@ -565,23 +641,25 @@
         res = self.launcher.get_players_and_uuids()
         if res:
             self.allplayers = list(res.keys())
             self.players_uuid.update(res)
         for player in pkt["Entries"]:
             isJoining = bool(player["Skin"]["SkinData"])
             playername = player["Username"]
+            if isJoining and "§" in playername:
+                self.say_to("@a", f"§l§7<§6§o!§r§l§7> §6此玩家名字中含特殊字符, 可能导致插件运行异常!")
+                # 没有VIP名字供测试...
             if isJoining:
                 Print.print_inf(f"§e{playername} 加入了游戏")
                 if playername not in self.allplayers and not res:
                     self.allplayers.append(playername)
                     return
                 plugin_group.execute_player_join(
                     playername, self.linked_frame.on_plugin_err
                 )
-                asyncio.run(execute_player_join(playername))
             else:
                 playername = next(
                     (k for k, v in self.players_uuid.items()
                      if v == player["UUID"]),
                     None,
                 )
                 if playername is None:
@@ -589,15 +667,14 @@
                     continue
                 if playername != "???" and not res:
                     self.allplayers.remove(playername)
                 Print.print_inf(f"§e{playername} 退出了游戏")
                 plugin_group.execute_player_leave(
                     playername, self.linked_frame.on_plugin_err
                 )
-                asyncio.run(execute_player_left(playername))
 
     def process_text_packet(self, pkt: dict, plugin_grp: "PluginGroup") -> None:
         """处理9号数据包的消息
 
         Args:
             pkt (dict): 数据包内容
             plugin_grp (PluginGroup): 插件组对象
@@ -605,64 +682,53 @@
         match pkt["TextType"]:
             case 2:
                 if pkt["Message"] == "§e%multiplayer.player.joined":
                     player = pkt["Parameters"][0]
                     plugin_grp.execute_player_prejoin(
                         player, self.linked_frame.on_plugin_err
                     )
-                    asyncio.run(execute_player_prejoin(player))
-                elif pkt["Message"].startswith("death."):
-                    death_message = self.Game_Data.get(pkt["Message"])
-                    if death_message:
-                        filled_parameters = [
-                            self.Game_Data.get(param.replace("%", ""), param)
-                            for param in pkt["Parameters"]
-                        ]
-                        filled_message = death_message.format(
-                            *filled_parameters)
-                        Print.print_inf(filled_message)
-
-                    if len(pkt["Parameters"]) >= 2:
-                        killer = pkt["Parameters"][1]
-                    else:
-                        killer = None
-                    plugin_grp.execute_player_death(
+                elif not pkt["Message"].startswith("§e%multiplayer.player.joined") and not pkt["Message"].startswith("§e%multiplayer.player.left"):
+                    jon = self.Game_Data_Handle.Handle_Text_Class1(pkt)
+                    Print.print_inf(("§1" + " ".join(jon)))
+                    if pkt["Message"].startswith("death."):
+                        if len(pkt["Parameters"]) >= 2:
+                            killer = pkt["Parameters"][1]
+                        else:
+                            killer = None
+                        plugin_grp.execute_player_death(
                         pkt["Parameters"][0],
                         killer,
                         pkt["Message"],
                         self.linked_frame.on_plugin_err,
                     )
-                    asyncio.run(
-                        execute_death_message(
-                            pkt["Parameters"][0], killer, pkt["Message"]
-                        )
-                    )
             case 1 | 7:
                 player, msg = pkt["SourceName"], pkt["Message"]
                 plugin_grp.execute_player_message(
                     player, msg, self.linked_frame.on_plugin_err
                 )
-                asyncio.run(execute_player_message(player, msg))
-
                 Print.print_inf(f"<{player}> {msg}")
             case 8:
                 player, msg = pkt["SourceName"], pkt["Message"]
                 Print.print_inf(f"{player} 使用say说: {msg.strip(f'[{player}]')}")
                 plugin_grp.execute_player_message(
                     player, msg, self.linked_frame.on_plugin_err
                 )
-                asyncio.run(execute_player_message(player, msg))
             case 9:
                 msg = pkt["Message"]
                 try:
                     msg_text = json.loads(msg)["rawtext"]
+                    if len(msg_text) > 0 and msg_text[0].get("translate") == "***":
+                        Print.print_with_info("(该tellraw内容为敏感词)", "§f 消息 ")
+                        return
                     msg_text = "".join([i["text"] for i in msg_text])
-                    Print.print_inf(msg_text)
+                    Print.print_with_info(msg_text, "§f 消息 ")
                 except Exception:
                     pass
+            case 10:
+                self.Game_Data_Handle.Handle_Text_Class2(pkt)
 
     def Inject(self) -> None:
         """载入游戏时的初始化"""
         res = self.launcher.get_players_and_uuids()
         if res:
             self.allplayers = list(res.keys())
             self.players_uuid.update(res)
@@ -691,17 +757,14 @@
         self.bot_name = self.launcher.get_bot_name()
         if self.bot_name is None:
             self.bot_name = self.allplayers[0]
         self.linked_frame.comsole_cmd_start()
         self.linked_frame.link_plugin_group.execute_init(
             self.linked_frame.on_plugin_err
         )
-        Builtins.createThread(asyncio.run, (execute_repeat(),))
-        Print.print_inf("正在执行初始化注入式函数init任务")
-        asyncio.run(execute_init())
         Print.print_suc("初始化注入式函数init任务执行完毕")
         self.inject_welcome()
 
     def inject_welcome(self) -> None:
         """初始化欢迎信息"""
 
         if isinstance(self.bot_name, str):
```

### Comparing `tooldelta-0.5.9/tooldelta/launch_cli.py` & `tooldelta-0.6.0/tooldelta/launch_cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,19 +7,20 @@
 import random
 import subprocess
 import platform
 from typing import Callable, Optional
 import ujson as json
 import requests
 import tooldelta
+import fcwslib
 
 from tooldelta import constants
 from . import neo_conn
 from .cfg import Cfg
-from .builtins import Builtins
+from .utils import Utils
 from .color_print import Print
 from .sys_args import sys_args_to_dict
 from .packets import Packet_CommandOutput
 from .urlmethod import download_file_singlethreaded, get_free_port
 
 Config = Cfg()
 
@@ -176,14 +177,31 @@
             NotImplementedError: 未实现此方法
 
         Returns:
             bool: 是否为OP
         """
         raise NotImplementedError
 
+    def place_command_block_with_nbt_data(self, block_name:str, block_states:str, 
+                                          position: tuple[int, int, int],
+                                          nbt_data: neo_conn.CommandBlockNBTData):
+        """在 position 放置方块名为 block_name 且方块状态为 block_states 的命令块，
+        同时向该方块写入 nbt_data 所指代的 NBT 数据
+
+        Args:
+            block_name (str): 命令块的方块名，如 chain_command_block
+            block_states (str): 命令块的方块状态，如 朝向南方 的命令方块表示为 ["facing_direction":3]
+            position (tuple[int, int, int]): 命令块应当被放置的位置。三元整数元组从左到右依次对应世界坐标的 X, Y, Z 轴坐标
+            nbt_data (neo_conn.CommandBlockNBTData): 该命令块的原始 NBT 数据
+
+        Raises:
+            NotImplementedError: 未实现此方法
+        """
+        raise NotImplementedError
+
 
 class FrameNeOmg(StandardFrame):
     """使用 NeOmega 框架连接到游戏"""
     launch_type = "NeOmega"
 
     def __init__(self, serverNumber: int, password: str, fbToken: str, auth_server: str) -> None:
         """初始化 NeOmega 框架
@@ -240,19 +258,20 @@
     def start_neomega_proc(self) -> int:
         """启动 NeOmega 进程
 
         Returns:
             int: 端口号
         """
         free_port = get_free_port(24016)
+        sys_machine = platform.uname().machine
         access_point_file = (
-            f"neomega_{platform.uname().system.lower()}_access_point_{self.sys_machine}"
+            f"neomega_{platform.uname().system.lower()}_access_point_{sys_machine}"
         )
         if "TERMUX_VERSION" in os.environ:
-            access_point_file = f"neomega_android_access_point_{self.sys_machine}"
+            access_point_file = f"neomega_android_access_point_{sys_machine}"
         if platform.system() == "Windows":
             access_point_file += ".exe"
         py_file_path = os.path.join(
             os.getcwd(), "tooldelta", "neo_libs", access_point_file
         )
         if platform.uname().system.lower() == "linux":
             os.system("chmod +x " + shlex.quote(py_file_path))
@@ -297,15 +316,15 @@
                 elif f"STATUS CODE: {self.secret_exit_key}" in msg_orig:
                     with Print.lock:
                         Print.print_with_info("§a机器人已退出", "§b NOMG ")
                     continue
                 with Print.lock:
                     Print.print_with_info(msg_orig, "§b NOMG ")
 
-        Builtins.createThread(_msg_show_thread, usage="显示来自NeOmega的信息")
+        Utils.createThread(_msg_show_thread, usage="显示来自NeOmega的信息")
 
     def make_secret_key(self) -> None:
         """生成退出密钥"""
         self.secret_exit_key = hex(random.randint(10000, 99999))
 
     def launch(self) -> SystemExit | Exception | SystemError:
         """启动 NeOmega 进程
@@ -338,14 +357,17 @@
             return SystemExit("正常退出.")
         if self.status == SysStatus.CRASHED_EXIT:
             return Exception("NeOmega 已崩溃")
         return SystemError("未知的退出状态")
 
     def download_libs(self) -> None:
         """根据系统架构和平台下载所需的库。"""
+        if "no-download-libs" in sys_args_to_dict().keys():
+            Print.print_war("将不会进行依赖库的下载和检测更新.")
+            return
         cfgs = Config.get_cfg("ToolDelta基本配置.json", constants.LAUNCH_CFG_STD)
         is_mir: bool = cfgs["是否使用github镜像"]
         if is_mir:
             mirror_src = "https://tdload.tblstudio.cn/" + \
                 "https://raw.githubusercontent.com/ToolDelta/ToolDelta/main/"
             depen_url = "https://tdload.tblstudio.cn/" + \
                 "https://raw.githubusercontent.com/ToolDelta/DependencyLibrary/main/"
@@ -358,23 +380,23 @@
                     f"{mirror_src}require_files.json", timeout=5
                 ).text
             )
         except Exception as err:
             Print.print_err(f"获取依赖库表出现问题: {err}")
             self.update_status(SysStatus.CRASHED_EXIT)
             return
-        self.sys_machine = platform.machine().lower()
-        if self.sys_machine == "x86_64":
-            self.sys_machine = "amd64"
-        elif self.sys_machine == "aarch64":
-            self.sys_machine = "arm64"
+        sys_machine = platform.machine().lower()
+        if sys_machine == "x86_64":
+            sys_machine = "amd64"
+        elif sys_machine == "aarch64":
+            sys_machine = "arm64"
         if "TERMUX_VERSION" in os.environ:
-            sys_info_fmt: str = f"Android:{self.sys_machine.lower()}"
+            sys_info_fmt: str = f"Android:{sys_machine.lower()}"
         else:
-            sys_info_fmt: str = f"{platform.uname().system}:{self.sys_machine.lower()}"
+            sys_info_fmt: str = f"{platform.uname().system}:{sys_machine.lower()}"
         source_dict: list[str] = require_depen[sys_info_fmt]
         commit_remote = requests.get(
             f"{depen_url}commit", timeout=5
         ).text
         commit_file_path = os.path.join(
             os.getcwd(), "tooldelta", "neo_libs", "commit")
         replace_file = False
@@ -527,17 +549,46 @@
 
         Returns:
             bool: 是否为OP
         """
         if self.omega is None:
             raise ValueError("未连接到接入点")
         player_obj = self.omega.get_player_by_name(player)
-        if player_obj is None or player_obj.command_permission_level is None:
+        if player_obj is None or player_obj.op_permissions_level is None:
             raise ValueError("未能获取玩家对象")
-        return player_obj.command_permission_level > 2
+        return player_obj.op_permissions_level > 1
+
+    def place_command_block_with_nbt_data(self, block_name:str, block_states:str,
+                                          position: tuple[int, int, int],
+                                          nbt_data: neo_conn.CommandBlockNBTData):
+        """在 position 放置方块名为 block_name 且方块状态为 block_states 的命令块，
+        同时向该方块写入 nbt_data 所指代的 NBT 数据
+
+        Args:
+            block_name (str): 命令块的方块名，如 chain_command_block
+            block_states (str): 命令块的方块状态，如 朝向南方 的命令方块表示为 ["facing_direction":3]
+            position (tuple[int, int, int]): 命令块应当被放置的位置。三元整数元组从左到右依次对应世界坐标的 X, Y, Z 轴坐标
+            nbt_data (neo_conn.CommandBlockNBTData): 该命令块的原始 NBT 数据
+
+        Raises:
+            NotImplementedError: 未实现此方法
+        """
+        if self.omega is None:
+            raise ValueError("未连接到接入点")
+        self.omega.place_command_block(neo_conn.CommandBlockPlaceOption(
+            X=position[0], Y=position[1], Z=position[2],
+            BlockName=block_name, BockState=block_states,
+            NeedRedStone=(not nbt_data.ConditionalMode),
+            Conditional=nbt_data.ConditionalMode,
+            Command=nbt_data.Command,
+            Name=nbt_data.CustomName,
+            TickDelay=nbt_data.TickDelay,
+            ShouldTrackOutput=nbt_data.TrackOutput,
+            ExecuteOnFirstTick=nbt_data.ExecuteOnFirstTick
+        ))
 
     sendPacketJson = sendPacket
 
 
 class FrameNeOmgRemote(FrameNeOmg):
     """远程启动器框架(使用 NeOmega 框架的Remote连接)
 
@@ -558,14 +609,15 @@
         try:
             openat_port = int(sys_args_to_dict().get(
                 "access-point-port") or "24020")
             if openat_port not in range(65536):
                 raise AssertionError
         except (ValueError, AssertionError):
             Print.print_err("启动参数 -access-point-port 错误: 不是1~65535的整数")
+            raise SystemExit("端口参数错误")
         if openat_port == 0:
             Print.print_war(
                 "未用启动参数指定链接neOmega接入点开放端口, 尝试使用默认端口 24015"
             )
             Print.print_inf("可使用启动参数 -access-point-port 端口 以指定接入点端口.")
             openat_port = 24015
             return SystemExit("未指定端口号")
@@ -585,7 +637,19 @@
         self.exit_event.wait()
         self.update_status(SysStatus.NORMAL_EXIT)
         if self.status == SysStatus.NORMAL_EXIT:
             return SystemExit("正常退出.")
         if self.status == SysStatus.CRASHED_EXIT:
             return Exception("接入点已崩溃")
         return SystemError("未知的退出状态")
+
+class FrameBEConnect(StandardFrame):
+    "WIP: Minecraft Bedrock '/connect' 指令所连接的服务端"
+    def __init__(self, serverNumber: int, password: str, fbToken: str, auth_server_url: str) -> None:
+        super().__init__(serverNumber, password, fbToken, auth_server_url)
+
+    def prepare_apis(self):
+        ...
+
+    async def wait_connect(self):
+        server = fcwslib.server.Server("127.0.0.1", 23000)
+        await server.run_forever()
```

### Comparing `tooldelta-0.5.9/tooldelta/launch_options.py` & `tooldelta-0.6.0/tooldelta/launch_options.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,54 @@
-"启动选项"
+"启动页面"
 import os
 import signal
 import traceback
 from .color_print import Print
 from .starter import start_tool_delta
+from .frame import Frame
 from .plugin_manager import plugin_manager
 from .plugin_market import market
-from .sys_args import sys_args_to_dict
+from .sys_args import sys_args_to_dict, print_help
 
 
 def signal_handler(*_) -> None:
     """排除信号中断"""
     return Print.print_war("ToolDelta 已忽略信号中断")
 
 
 signal.signal(signal.SIGINT, signal_handler)
 
 
 def client_title() -> None:
     "选择启动模式"
     try:
+        if "h" in sys_args_to_dict() or "help" in sys_args_to_dict():
+            print_help()
+            os._exit(0)
         launch_mode = sys_args_to_dict()
         if launch_mode.get("l"):
             if not isinstance(launch_mode["l"], str):
                 raise ValueError("启动模式参数不合法")
             r = launch_mode["l"]
         else:
-            Print.clean_print("§b请选择启动模式(使用启动参数 -l <启动模式> 可以跳过该页面):")
-            Print.clean_print("1 - 启动 ToolDelta")
-            Print.clean_print("2 - 打开 ToolDelta 插件管理器")
-            Print.clean_print("3 - 打开 ToolDelta 插件市场")
+            Print.clean_print("§a请选择启动模式§6(使用启动参数 -l <启动模式> 可以跳过该页面):")
+            Print.clean_print("1 - §b启动 ToolDelta")
+            Print.clean_print("2 - §d打开 ToolDelta 插件管理器")
+            Print.clean_print("3 - §d打开 ToolDelta 插件市场")
+            Print.clean_print("4 - §a修改 ToolDelta 启动配置")
             r = input("请选择:").strip()
         match r:
             case "1":
                 start_tool_delta()
             case "2":
                 plugin_manager.manage_plugins()
             case "3":
                 market.enter_plugin_market()
+            case "4":
+                Frame.change_config()
             case _:
                 Print.clean_print("§c不合法的模式: " + r)
         os._exit(0)
     except EOFError:
         pass
     except Exception:
         Print.print_err("ToolDelta 运行过程中出现问题: " + traceback.format_exc())
```

### Comparing `tooldelta-0.5.9/tooldelta/logger.py` & `tooldelta-0.6.0/tooldelta/logger.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.9/tooldelta/neo_conn.py` & `tooldelta-0.6.0/tooldelta/neo_conn.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import ujson as json
 import os.path
 import traceback
 import threading
 import enum
 from typing import Iterable, Tuple, Optional, Union, Any, Callable, List, Dict
 from threading import Thread
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from tooldelta.color_print import Print
 from tooldelta.packets import Packet_CommandOutput
 
 CInt = ctypes.c_longlong
 CString = ctypes.c_char_p
 CBytes = ctypes.POINTER(ctypes.c_char)
 
@@ -64,16 +64,14 @@
     UserToken: str = ""
     UserName: str = ""
     UserPassword: str = ""
     ServerCode: str = ""
     ServerPassword: str = ""
 
 
-
-
 def StartOmega(address, AccountOptions):
     r = LIB.StartOmega(
         toCString(address), toCString(json.dumps(AccountOptions.__dict__))
     )
     if r is not None:
         raise Exception(toPyString(r))
 
@@ -202,27 +200,20 @@
     WorldDifficulty: Optional[int] = None
     Time: Optional[int] = None
     DayTime: Optional[int] = None
     TimePercent: Optional[float] = None
     GameRules: Optional[Dict[str, Any]] = None
 
 
-
-
-def ConsumeChat() -> "Chat":
-    chatData = json.loads(toPyString(LIB.ConsumeChat()))
-    return Chat(**chatData)
-
-
 class Counter:
     def __init__(self, prefix: str) -> None:
         self.current_i = 0
         self.prefix = prefix
 
-    def __next__(self) -> int:
+    def __next__(self) -> str:
         self.current_i += 1
         return f"{self.prefix}_{self.current_i}"
 
 
 @dataclass
 class ActionPermissionMap:
     ActionPermissionAttackMobs: bool = False
@@ -245,47 +236,35 @@
     AdventureFlagNoClip: bool = False
     AdventureFlagWorldBuilder: bool = False
     AdventureFlagWorldImmutable: bool = False
     AdventureSettingsFlagsNoMvP: bool = False
     AdventureSettingsFlagsNoPvM: bool = False
     AdventureSettingsFlagsShowNameTags: bool = False
 
-
-@dataclass
-class Chat:
-    Name: str = ""
-    Msg: List[str] = ""
-    Type: int = 1
-    RawMsg: str = ""
-    RawName: str = ""
-    RawParameters: Optional[Any] = None
-    Aux: Optional[Any] = None
-
-
 @dataclass
 class CommandOrigin:
     Origin: int = 0
     UUID: str = ""
     RequestID: str = ""
     PlayerUniqueID: int = 0
 
 
 @dataclass
 class OutputMessage:
-    Success: bool = False
-    Message: str = ""
-    Parameters: Optional[List[Any]] = None
+    Success: bool
+    Message: str
+    Parameters: List[Any]
 
 
 @dataclass
 class CommandOutput:
-    CommandOrigin: Optional["CommandOrigin"] = None
-    OutputType: int = 0
-    SuccessCount: int = 0
-    OutputMessages: Optional[List[OutputMessage]] = None
+    CommandOrigin: "CommandOrigin"
+    OutputType: int
+    SuccessCount: int
+    OutputMessages: List[OutputMessage]
     DataSet: Optional[Any] = None
 
     @property
     def as_dict(self):
         return _unpack_command_output(self)
 
 
@@ -308,14 +287,15 @@
         and commandOutputData["OutputMessages"] != ""
     ):
         outputMessagesData = commandOutputData["OutputMessages"]
         for outputMessageData in outputMessagesData:
             outputMessage = OutputMessage(
                 Success=outputMessageData["Success"],
                 Message=outputMessageData["Message"],
+                Parameters=[]
             )
             parameters = []
             if "Parameters" in outputMessageData.keys():
                 parametersData = outputMessageData["Parameters"]
                 for parameterData in parametersData:
                     try:
                         parameters.append(json.loads(parameterData))
@@ -345,14 +325,36 @@
     Name: str = ""
     TickDelay: int = 0
     ShouldTrackOutput: bool = False
     ExecuteOnFirstTick: bool = False
 
 
 @dataclass
+class CommandBlockNBTData:
+    """指代一个命令块的原始 NBT 数据 (ToolDelta 专有实现类)
+    
+    Args
+        Command (str; TAG_String): 命令块所包含的命令，默认为 空字符串
+        CustomName (str; TAG_String): 命令方块的悬浮文本，默认为 空字符串
+        TickDelay (int; TAG_Int): 命令块使用的延迟，默认为 0
+        ExecuteOnFirstTick (bool; TAG_Byte): 是否在该命令块上使用第一个已选项(仅重复型命令块适用)，默认 启用
+        TrackOutput (bool; TAG_Byte): 是否在该命令块上启用命令执行输出，默认 启用
+        ConditionalMode (bool; TAG_Byte): 命令块是否是“有条件的”，默认为 无条件
+        Auto (bool; TAG_Byte): 命令块是否自动运行(无需红石控制)，默认为 自动运行(无需红石控制)
+    """
+    Command: str = ""
+    CustomName: str = ""
+    TickDelay: int = 0
+    ExecuteOnFirstTick: bool = True
+    TrackOutput: bool = True
+    ConditionalMode: bool = False
+    Auto: bool = True
+
+
+@dataclass
 class QueriedPlayerPos:
     dimension: int = 0
     x: float = 0
     y: float = 0.0
     z: float = 0.0
     yRot: float = 0.0
 
@@ -449,28 +451,28 @@
 
     @property
     def entity_runtime_id(self) -> int:
         OmegaAvailable()
         return int(LIB.PlayerEntityRuntimeID(self._c_uuid))
 
     @property
-    def entity_metadata(self) -> any:
+    def entity_metadata(self) -> Any:
         OmegaAvailable()
         return json.loads(toPyString(LIB.PlayerEntityMetadata(self._c_uuid)))
 
     def query(self, conditions: Union[None, str, List[str]] = None) -> CommandOutput:
         query_str = f'querytarget @a[name="{self.name}"'
         if conditions is None:
             query_str += "]"
         elif isinstance(conditions, str):
             query_str += "," + conditions + "]"
         else:
             query_str += "," + ",".join(conditions) + "]"
         ret = self.parent.send_websocket_command_need_response(query_str)
-        return ret
+        return ret # type: ignore
 
     def check_conditions(self, conditions: Union[None, str, List[str]] = None) -> bool:
         return self.query(conditions).SuccessCount > 0
 
     def set_ability_map(
         self, action_permission: ActionPermissionMap, adventure_flag: AdventureFlagsMap
     ):
@@ -494,16 +496,16 @@
     Local = "Local"  # 在内部启动一个单独的 neOmega Core
 
 
 class ThreadOmega:
     def __init__(
         self,
         connect_type: ConnectType,
-        address: str = "tcp://localhost:24016",
-        accountOption: AccountOptions = None,
+        address: str,
+        accountOption: AccountOptions,
     ) -> None:
         self._thread_counter = Counter("thread")
         self._running_threads: Dict[str, Thread] = {}
         if connect_type == ConnectType.Local:
             StartOmega(address, accountOption)
             Print.print_inf(f"Omega 接入点已启动, 在 {address} 开放接口")
         elif connect_type == ConnectType.Remote:
@@ -515,16 +517,15 @@
         self._omega_disconnected_reason = ""
 
         # cmd events
         self._cmd_callback_retriever_counter = Counter("cmd_callback")
         self._omega_cmd_callback_events: Dict[str, Callable] = {}
 
         # packet listeners
-        self._packet_listeners: Dict[str,
-                                     List[Callable[[str, any], None]]] = {}
+        self._packet_listeners: Dict[str, List[Callable[[str, Any], None]]] = {}
 
         # setup actions
         # make LIB listen to all packets and new packets will have eventType="MCPacket"
         LIB.ListenAllPackets()
         mapping = json.loads(toPyString(LIB.GetPacketNameIDMapping()))
         self._packet_name_to_id_mapping: dict[str, int] = mapping
         self._packet_id_to_name_mapping = {}
@@ -538,20 +539,14 @@
 
         # get bot basic info (this info will not change so we need to get it only once)
         self._bot_basic_info = ClientMaintainedBotBasicInfo(
             **json.loads(toPyString(LIB.GetClientMaintainedBotBasicInfo()))
         )
 
         # player hooks
-        self._bind_players: Dict[str, PlayerKit] = {}
-
-        # named command block msg
-        self._name_command_block_msg_listeners: Dict[
-            str, List[Callable[[Chat], None]]
-        ] = {}
 
         # start routine
         self.start_new(self._react)
 
     def start_new(self, func: Callable, args: Iterable[Any] = ()):
         try:
             thread_i = next(self._thread_counter)
@@ -612,24 +607,14 @@
 
             elif eventType == "PlayerInterceptInput":
                 OmitEvent()
 
             elif eventType == "Chat":
                 OmitEvent()
 
-            elif eventType == "NamedCommandBlockMsg":
-                blockName = retriever
-                listeners = self._name_command_block_msg_listeners[blockName]
-                if len(listeners) == 0:
-                    LIB.OmitEvent()
-                else:
-                    chat = ConsumeChat()
-                    for l in listeners:
-                        self.start_new(l, (chat,))
-
     def wait_disconnect(self) -> str:
         """return: disconnect reason"""
         self._omega_disconnected_lock.wait()
         return self._omega_disconnected_reason
 
     @staticmethod
     def _create_lock_and_result_setter():
@@ -724,24 +709,24 @@
         for t in res:
             self._packet_listeners[t].append(callback)
 
     def construct_game_packet_bytes_in_json_as_is(
         self, packet_type: Union[int, str], content: Any
     ) -> tuple[int, bytes]:
         if isinstance(packet_type, str):
-            packet_type = self.get_packet_name_to_id_mapping(packet_type)
-        return packet_type, JsonStrAsIsGamePacketBytes(packet_type, json.dumps(content))
+            packet_type = self.get_packet_name_to_id_mapping(packet_type) # type: ignore
+        return packet_type, JsonStrAsIsGamePacketBytes(packet_type, json.dumps(content)) # type: ignore
 
     def send_game_packet_in_json_as_is(
         self, packet_type: Union[int, str], content: Any
     ):
         if isinstance(packet_type, str):
-            packet_type = self.get_packet_name_to_id_mapping(packet_type)
+            packet_type = self.get_packet_name_to_id_mapping(packet_type) # type: ignore
         OmegaAvailable()
-        SendGamePacket(packet_type, json.dumps(content))
+        SendGamePacket(packet_type, json.dumps(content))  # type: ignore
 
     def get_bot_basic_info(self) -> ClientMaintainedBotBasicInfo:
         return self._bot_basic_info
 
     def get_bot_name(self) -> str:
         return self._bot_basic_info.BotName
 
@@ -763,24 +748,25 @@
         return ClientMaintainedExtendInfo(
             **json.loads(toPyString(LIB.GetClientMaintainedExtendInfo()))
         )
 
     def _get_bind_player(self, uuidStr: str) -> Optional[PlayerKit]:
         if uuidStr is None or uuidStr == "":
             return None
-        if uuidStr in self._bind_players:
-            return self._bind_players[uuidStr]
-        bind_player = PlayerKit(uuidStr, self)
-        self._bind_players[uuidStr] = bind_player
-        return bind_player
+        return PlayerKit(uuidStr, self)
 
     def get_all_online_players(self):
         OmegaAvailable()
         playerUUIDS = json.loads(toPyString(LIB.GetAllOnlinePlayers()))
-        return [self._get_bind_player(uuidStr) for uuidStr in playerUUIDS]
+        ret: List[PlayerKit] = []
+        for uuidStr in playerUUIDS:
+            r = self._get_bind_player(uuidStr)
+            if r:
+                ret.append(r)
+        return ret
 
     def get_player_by_name(self, name: str) -> Optional[PlayerKit]:
         OmegaAvailable()
         playerUUID = toPyString(LIB.GetPlayerByName(toCString(name)))
         return self._get_bind_player(playerUUID)
 
     def get_player_by_uuid(self, uuidStr: str) -> Optional[PlayerKit]:
@@ -789,23 +775,14 @@
         return self._get_bind_player(playerUUID)
 
     def listen_player_change(self, callback: Callable[[PlayerKit, str], None]):
         for player in self.get_all_online_players():
             callback(player, "exist")
         self._player_change_listeners.append(callback)
 
-    def listen_named_command_block(
-        self, command_block_name: str, callback: Callable[[Chat], None]
-    ):
-        if command_block_name not in self._name_command_block_msg_listeners:
-            self._name_command_block_msg_listeners[command_block_name] = []
-        LIB.ListenCommandBlock(toCString(command_block_name))
-        self._name_command_block_msg_listeners[command_block_name].append(
-            callback)
-
     @staticmethod
     def place_command_block(place_option: CommandBlockPlaceOption):
         LIB.PlaceCommandBlock(toCString(json.dumps(place_option.__dict__)))
 
     def __del__(self):
         for t in self._running_threads.values():
             t.join()
@@ -872,15 +849,15 @@
     LIB.ConsumeMCPacket.restype = MCPacketEvent
     LIB.SendWebSocketCommandNeedResponse.argtypes = [CString, CString]
     LIB.SendPlayerCommandNeedResponse.argtypes = [CString, CString]
     LIB.SendWOCommand.argtypes = [CString]
     LIB.SendWebSocketCommandOmitResponse.argtypes = [CString]
     LIB.SendPlayerCommandOmitResponse.argtypes = [CString]
     LIB.FreeMem.argtypes = [ctypes.c_void_p]
-    LIB.ListenAllPackets.argtypes = None
+    LIB.ListenAllPackets.argtypes = []
     LIB.GetPacketNameIDMapping.restype = CString
     LIB.JsonStrAsIsGamePacketBytes.argtypes = [CInt, CString]
     LIB.JsonStrAsIsGamePacketBytes.restype = JsonStrAsIsGamePacketBytes_return
     LIB.SendGamePacket.argtypes = [CInt, CString]
     LIB.SendGamePacket.restype = CString
     LIB.GetClientMaintainedBotBasicInfo.restype = CString
     LIB.GetClientMaintainedExtendInfo.restype = CString
```

### Comparing `tooldelta-0.5.9/tooldelta/packets.py` & `tooldelta-0.6.0/tooldelta/packets.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-"构建数据包方便获取"
+"数据包类构建器"
 
 class PacketIDS:
-    "数据包id"
+    "数据包id常量表"
     Text = 9
     PlayerList = 63
     CommandOutput = 79
 
 
 class SubPacket_CmdOutputMsg:
     """命令输出消息子包构建"""
```

### Comparing `tooldelta-0.5.9/tooldelta/plugin_load/PluginGroup.py` & `tooldelta-0.6.0/tooldelta/plugin_load/PluginGroup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,40 @@
-"插件管理器"
+"插件加载器框架"
 import asyncio
 import traceback
-from typing import TYPE_CHECKING, Any, Callable, Union
+from typing import TYPE_CHECKING, Any, Callable, Union, TypeVar
+
+PLUGIN_CLS_TYPE = TypeVar("PLUGIN_CLS_TYPE")
 
 from ..color_print import Print
 from ..plugin_load.classic_plugin import Plugin
+from ..utils import Utils
+from .injected_plugin import (
+    execute_init,
+    execute_player_prejoin,
+    execute_player_join,
+    execute_player_message,
+    execute_death_message,
+    execute_player_left,
+    execute_repeat
+)
 from ..plugin_load import (
     classic_plugin,
     injected_plugin,
     NON_FUNC,
     NotValidPluginError,
     PluginAPINotFoundError,
     PluginAPIVersionError,
 )
 from ..constants import PRG_NAME
-if TYPE_CHECKING:
-    from ..frame import Frame
+from .utils import set_frame as _set_frame
+from .injected_plugin.movent import set_frame as _set_frame_inj
 
+if TYPE_CHECKING:
+    from ..frame import Frame, GameCtrl
 
 class PluginGroup:
     "插件组"
     plugins: list[list[str | Plugin]] = []
     plugins_funcs: dict[str, list] = {
         "on_def": [],
         "on_inject": [],
@@ -34,23 +48,24 @@
     pluginAPI_added_cache = []
     broadcast_evts_cache = {}
 
     def __init__(self):
         "初始化"
         self._listen_packet_ids = set()
         self._packet_funcs: dict[str, list[Callable]] = {}
-        self.plugins_api: dict[str, Plugin] = {}
         self._broadcast_listeners: dict[str, list[Callable]] = {}
+        self._repeat_funcs = {}
+        self.plugins_api: dict[str, Plugin] = {}
         self.excType = 0
         self.normal_plugin_loaded_num = 0
         self.injected_plugin_loaded_num = 0
         self.loaded_plugins_name = []
         self.linked_frame: Union["Frame" , None] = None
 
-    def add_plugin(self, plugin: type[Plugin]) -> type[Plugin]:
+    def add_plugin(self, plugin: type[PLUGIN_CLS_TYPE]) -> type[PLUGIN_CLS_TYPE]:
         """添加插件
 
         Args:
             plugin (type[Plugin]): 插件主类
 
         Raises:
             NotValidPluginError: 插件主类必须继承Plugin类
@@ -61,32 +76,32 @@
         try:
             if not Plugin.__subclasscheck__(plugin):
                 raise NotValidPluginError(f"插件主类必须继承Plugin类 而不是 {plugin}")
         except TypeError as exc:
             raise NotValidPluginError(
                 f"插件主类必须继承Plugin类 而不是 {plugin.__class__}") from exc
         self.plugin_added_cache["plugin"] = plugin
-        self.test_plugin(plugin)
+        self.test_plugin(plugin) # type: ignore
         return plugin
 
-    def add_plugin_as_api(self, apiName: str) -> Callable[[type[Plugin]], type[Plugin]]:
+    def add_plugin_as_api(self, apiName: str):
         """添加插件作为API
 
         Args:
             apiName (str): API名
 
         Returns:
             Callable[[type[Plugin]], type[Plugin]]: 添加插件作为API
         """
-        def _add_plugin_2_api(api_plugin:  type[Plugin]) -> type[Plugin]:
+        def _add_plugin_2_api(api_plugin: type[PLUGIN_CLS_TYPE]) -> type[PLUGIN_CLS_TYPE]:
             if not Plugin.__subclasscheck__(api_plugin):
                 raise NotValidPluginError("API插件主类必须继承Plugin类")
             self.plugin_added_cache["plugin"] = api_plugin
             self.pluginAPI_added_cache.append(apiName)
-            self.test_plugin(api_plugin)
+            self.test_plugin(api_plugin) # type: ignore
             return api_plugin
 
         return _add_plugin_2_api
 
     def add_packet_listener(self, pktID: int | list[int]) -> Callable[[Callable], Callable]:
         """添加数据包监听器
 
@@ -197,38 +212,44 @@
             raise self.linked_frame.SystemVersionException(
                 f"该组件需要{PRG_NAME}为{'.'.join([str(i) for i in self.linked_frame.sys_data.system_version])}版本"
             )
         elif self.linked_frame is None:
 
             raise ValueError("无法检查ToolDelta系统版本，请确保已经加载了ToolDelta系统组件")
 
-    def get_plugin_api(self, apiName: str, min_version: tuple | None = None) -> Plugin:
+    def get_plugin_api(self, apiName: str, min_version: tuple | None = None, force = True) -> Any:
         """获取插件API
 
         Args:
             apiName (str): 插件API名
             min_version (tuple | None, optional): API最低版本(若不填则默认不检查最低版本)
+            force: 若为False, 则在找不到插件API时不报错而是返回None
 
         Raises:
             PluginAPIVersionError: 插件API版本错误
             PluginAPINotFoundError: 无法找到API插件
 
         Returns:
             Plugin: 插件API
         """
         api = self.plugins_api.get(apiName)
         if api:
             if min_version and api.version < min_version:
                 raise PluginAPIVersionError(apiName, min_version, api.version)
             return api
-        raise PluginAPINotFoundError(f"无法找到API插件：{apiName}")
+        if force:
+            raise PluginAPINotFoundError(f"无法找到API插件：{apiName}")
+        else:
+            return None
 
     def set_frame(self, frame: "Frame") -> None:
-        "设置关联的框架"
+        "设置关联的系统框架"
         self.linked_frame = frame
+        _set_frame(frame)
+        _set_frame_inj(frame)
 
     def read_all_plugins(self) -> None:
         """读取所有插件
 
         Raises:
             SystemExit: 读取插件出现问题
         """
@@ -239,72 +260,71 @@
             self.execute_def(self.linked_frame.on_plugin_err)
             asyncio.run(injected_plugin.load_plugin(self))
         except Exception as err:
             err_str = "\n".join(traceback.format_exc().split("\n")[1:])
             Print.print_err(f"加载插件出现问题: \n{err_str}")
             raise SystemExit from err
 
-    @staticmethod
-    def load_plugin_hot(plugin_name: str, plugin_type: str) -> None:
+    def load_plugin_hot(self, plugin_name: str, plugin_type: str) -> None:
         """热加载插件
 
         Args:
             plugin_name (str): 插件名
             plugin_type (str): 插件类型
         """
         plugin = None
         if plugin_type == "classic":
-            plugin = classic_plugin.load_plugin(plugin_name)
+            plugin = classic_plugin.load_plugin(self, plugin_name)
         elif plugin_type == "injected":
             asyncio.run(injected_plugin.load_plugin_file(plugin_name))
         # 检查是否有on_def成员再执行
         if plugin and hasattr(plugin, "on_def"):
             plugin.on_def() # type: ignore
         Print.print_suc(f"成功热加载插件: {plugin_name}")
 
-    def add_listen_packet_id(self, packetType: int) -> None:
-        """添加数据包监听
+    def _add_listen_packet_id(self, packetType: int) -> None:
+        """添加数据包监听, 仅在系统内部使用
 
         Args:
             packetType (int): 数据包ID
 
         Raises:
             ValueError: 无法添加数据包监听，请确保已经加载了系统组件
         """
         if self.linked_frame is None:
             raise ValueError("无法添加数据包监听，请确保已经加载了系统组件")
         self._listen_packet_ids.add(packetType)
         self.linked_frame.link_game_ctrl.add_listen_pkt(packetType)
 
-    def add_listen_packet_func(self, packetType: int, func: Callable) -> None:
-        """添加数据包监听器
+    def _add_listen_packet_func(self, packetType: int, func: Callable) -> None:
+        """添加数据包监听器, 仅在系统内部使用
 
         Args:
             packetType (int): 数据包ID
             func (Callable): 数据包监听器
         """
         if self._packet_funcs.get(str(packetType)):
             self._packet_funcs[str(packetType)].append(func)
         else:
             self._packet_funcs[str(packetType)] = [func]
 
-    def add_broadcast_evt(self, evt: str, func: Callable) -> None:
-        """添加广播事件监听器
+    def _add_broadcast_evt(self, evt: str, func: Callable) -> None:
+        """添加广播事件监听器, 仅在系统内部使用
 
         Args:
             evt (str): 事件名
             func (Callable): 事件监听器
         """
         if self._broadcast_listeners.get(evt):
             self._broadcast_listeners[evt].append(func)
         else:
             self._broadcast_listeners[evt] = [func]
 
     def execute_def(self, onerr: Callable[[str, Exception, str], None] = NON_FUNC) -> None:
-        """执行插件的初始化方法
+        """执行插件的二次初始化方法
 
         Args:
             onerr (Callable[[str, Exception, str], None], optional): 插件出错时的处理方法. Defaults to NON_FUNC.
 
         Raises:
             SystemExit: 缺少前置
             SystemExit: 前置版本过低
@@ -320,24 +340,26 @@
                     f"插件 {name} 需要该前置组件 {err.name} 版本: {err.m_ver}, 但是现有版本过低: {err.n_ver}"
                 )
                 raise SystemExit from err
             except Exception as err:
                 onerr(name, err, traceback.format_exc())
 
     def execute_init(self, onerr: Callable[[str, Exception, str], None] = NON_FUNC) -> None:
-        """执行插件的初始化方法
+        """执行插件的连接游戏后初始化方法
 
         Args:
             onerr (Callable[[str, Exception, str], None], optional): 插件出错时的处理方法
         """
         for name, func in self.plugins_funcs["on_inject"]:
             try:
                 func()
             except Exception as err:
                 onerr(name, err, traceback.format_exc())
+        asyncio.run(execute_init())
+        Utils.createThread(asyncio.run, (execute_repeat(),))
 
     def execute_player_prejoin(
         self, player, onerr: Callable[[str, Exception, str], None] = NON_FUNC
     ) -> None:
         """执行玩家加入前的方法
 
         Args:
@@ -345,14 +367,15 @@
             onerr (Callable[[str, Exception, str], None], optional): 插件出错时的处理方法
         """
         for name, func in self.plugins_funcs["on_player_prejoin"]:
             try:
                 func(player)
             except Exception as err:
                 onerr(name, err, traceback.format_exc())
+        asyncio.run(execute_player_prejoin(player))
 
     def execute_player_join(
         self, player: str, onerr: Callable[[str, Exception, str], None] = NON_FUNC
     ) -> None:
         """执行玩家加入的方法
 
         Args:
@@ -360,14 +383,15 @@
             onerr (Callable[[str, Exception, str], None], optional): q 插件出错时的处理方法
         """
         for name, func in self.plugins_funcs["on_player_join"]:
             try:
                 func(player)
             except Exception as err:
                 onerr(name, err, traceback.format_exc())
+        asyncio.run(execute_player_join(player))
 
     def execute_player_message(
         self, player: str, msg: str, onerr: Callable[[str, Exception, str], None] = NON_FUNC
     ) -> None:
         """执行玩家消息的方法
 
         Args:
@@ -379,14 +403,15 @@
         if msg.startswith(pat):
             msg = msg.strip(pat)
         for name, func in self.plugins_funcs["on_player_message"]:
             try:
                 func(player, msg)
             except Exception as err:
                 onerr(name, err, traceback.format_exc())
+        asyncio.run(execute_player_message(player, msg))
 
     def execute_player_leave(
         self, player: str, onerr: Callable[[str, Exception, str], None] = NON_FUNC
     ) -> None:
         """执行玩家离开的方法
 
         Args:
@@ -394,14 +419,15 @@
             onerr (Callable[[str, Exception, str], None], optional): 插件出错时的处理方法
         """
         for name, func in self.plugins_funcs["on_player_leave"]:
             try:
                 func(player)
             except Exception as err:
                 onerr(name, err, traceback.format_exc())
+        asyncio.run(execute_player_left(player))
 
     def execute_player_death(
         self,
         player: str,
         killer: str | None,
         msg: str,
         onerr: Callable[[str, Exception, str], None] = NON_FUNC,
@@ -415,14 +441,19 @@
             onerr (Callable[[str, Exception, str], None], optional): 插件出错时的处理方法
         """
         for name, func in self.plugins_funcs["on_player_death"]:
             try:
                 func(player, killer, msg)
             except Exception as err:
                 onerr(name, err, traceback.format_exc())
+        asyncio.run(
+            execute_death_message(
+                player, killer, msg
+            )
+        )
 
     def processPacketFunc(self, pktID: int, pkt: dict) -> bool:
         """处理数据包监听器
 
         Args:
             pktID (int): 数据包ID
             pkt (dict): 数据包
```

### Comparing `tooldelta-0.5.9/tooldelta/plugin_load/__init__.py` & `tooldelta-0.6.0/tooldelta/plugin_load/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.9/tooldelta/plugin_load/classic_plugin/__init__.py` & `tooldelta-0.6.0/tooldelta/plugin_load/classic_plugin/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,81 +1,78 @@
 "ToolDelta类式插件"
 import importlib
 import os
 import sys
 import traceback
+import zipfile
 from typing import TYPE_CHECKING, Callable, Union
 from ...color_print import Print
-from ...builtins import Builtins
+from ...utils import Utils
 from ...cfg import Cfg
-from ...plugin_load.funcs import unzip_plugin
 from ...plugin_load import plugin_is_enabled, NotValidPluginError
 from ...constants import TOOLDELTA_CLASSIC_PLUGIN
 
 if TYPE_CHECKING:
     # 类型注释
     from ...frame import Frame
     from ...plugin_load.PluginGroup import PluginGroup
 
-
 class Plugin:
     "插件信息主类"
     name: str = ""
     version = (0, 0, 1)
     author = "?"
     description = "..."
 
     def __init__(self, frame: "Frame"):
         self.frame = frame
         self.game_ctrl = frame.get_game_control()
 
     @property
     def data_path(self) -> str:
-        "数据路径"
-        return os.path.join("插件数据文件", self.name)
-
-
-plugin_group_cache: list[Union["PluginGroup", None]] = [None]
-
+        "该插件的数据文件夹路径 (调用时直接创建数据文件夹)"
+        path = os.path.join("插件数据文件", self.name)
+        os.makedirs(path, exist_ok=True)
+        return path
 
 def read_plugins(plugin_grp: "PluginGroup") -> None:
     """读取插件
 
     Args:
         plugin_grp (PluginGroup): 插件组
     """
-    plugin_group_cache[0] = plugin_grp
     PLUGIN_PATH = os.path.join("插件文件", TOOLDELTA_CLASSIC_PLUGIN)
     sys.path.append(os.path.join("插件文件", TOOLDELTA_CLASSIC_PLUGIN))
     for plugin_dir in os.listdir(PLUGIN_PATH):
         if not plugin_is_enabled(plugin_dir):
             continue
         if (
             not os.path.isdir(os.path.join(
                 PLUGIN_PATH, plugin_dir.strip(".zip")))
             and os.path.isfile(os.path.join(PLUGIN_PATH, plugin_dir))
             and plugin_dir.endswith(".zip")
         ):
             Print.print_with_info(f"§6正在解压插件{plugin_dir}, 请稍后", "§6 解压 ")
-            unzip_plugin(
+            _unzip_plugin(
                 os.path.join(PLUGIN_PATH, plugin_dir),
                 os.path.join(PLUGIN_PATH, plugin_dir.strip(".zip")),
             )
             Print.print_suc(f"§a成功解压插件{plugin_dir} -> 插件目录")
             plugin_dir = plugin_dir.strip(".zip")
         if os.path.isdir(os.path.join(PLUGIN_PATH, plugin_dir)):
             sys.path.append(os.path.join(PLUGIN_PATH, plugin_dir))
-            load_plugin(plugin_dir)
+            load_plugin(plugin_grp, plugin_dir)
             plugin_grp.loaded_plugins_name.append(plugin_dir)
 
 
-def load_plugin(plugin_dirname: str) -> Union[None, Plugin]:
+def load_plugin(plugin_group: "PluginGroup", plugin_dirname: str) -> Union[None, Plugin]:
     """加载插件
 
     Args:
+        plugin_group (PluginGroup): 插件组类
         plugin_dirname (str): 插件目录名
         hot_load (bool, optional): 是否热加载
 
     Raises:
         ValueError: 插件组未初始化读取
         ValueError: 插件组未绑定框架
         ValueError: 插件主类需要作者名
@@ -84,40 +81,40 @@
         SystemExit: 插件名字不合法
         SystemExit: 插件配置文件报错
         SystemExit: 插件读取数据失败
 
     Returns:
         Union[None, Plugin]: 插件实例
     """
-    plugin_grp = plugin_group_cache[0]
+    plugin_grp = plugin_group
     if isinstance(plugin_grp, type(None)):
         raise ValueError("插件组未初始化读取")
     if isinstance(plugin_grp.linked_frame, type(None)):
         raise ValueError("插件组未绑定框架")
     try:
         if os.path.isfile(
             os.path.join(
                 "插件文件", TOOLDELTA_CLASSIC_PLUGIN, plugin_dirname, "__init__.py"
             )
         ):
             importlib.__import__(plugin_dirname)
         else:
             Print.print_war(f"{plugin_dirname} 文件夹 未发现插件文件, 跳过加载")
             return
-        Builtins.simpleAssert(
+        Utils.simpleAssert(
             plugin_grp.plugin_added_cache["plugin"] is not None,
             NotValidPluginError(
                 "需要调用1次 @plugins.add_plugin 以注册插件主类, 然而没有调用"
             ),
         )
         plugin: type[Plugin] = plugin_grp.plugin_added_cache["plugin"]
         if plugin.name is None:
             raise ValueError(f"插件主类 {plugin.__name__} 需要作者名")
         plugin_ins = plugin(plugin_grp.linked_frame)
-        if isinstance(plugin_ins, type(None)) or plugin_ins.name is "":
+        if isinstance(plugin_ins, type(None)) or plugin_ins.name == "":
             raise ValueError(f"插件主类 {plugin.__name__} 需要作者名")
         plugin_grp.plugins.append([plugin_ins.name, plugin_ins])
         _v0, _v1, _v2 = plugin_ins.version
         for evt_name in (
             "on_def",
             "on_inject",
             "on_player_prejoin",
@@ -135,16 +132,16 @@
         )
         plugin_grp.normal_plugin_loaded_num += 1
         if plugin_grp.plugin_added_cache["packets"] != []:
             for pktType, func in plugin_grp.plugin_added_cache["packets"]:
                 pfunc = getattr(plugin_ins, func.__name__)
                 if pfunc is None:
                     raise NotValidPluginError("数据包监听不能在主插件类以外定义")
-                plugin_grp.add_listen_packet_id(pktType)
-                plugin_grp.add_listen_packet_func(
+                plugin_grp._add_listen_packet_id(pktType)
+                plugin_grp._add_listen_packet_func(
                     pktType, pfunc
                 )
         if plugin_grp.pluginAPI_added_cache is not None:
             for _api in plugin_grp.pluginAPI_added_cache:
                 if isinstance(_api, str):
                     plugin_grp.plugins_api[_api] = plugin_ins
                 else:
@@ -154,30 +151,44 @@
         if plugin_grp.broadcast_evts_cache != {}:
             for evt, funcs in plugin_grp.broadcast_evts_cache.items():
                 for func in funcs:
                     bfunc = getattr(plugin_ins, func.__name__)
                     if bfunc is not None:
                         # 在插件主类以内定义了广播接收器
                         func = bfunc
-                    plugin_grp.add_broadcast_evt(evt, func)
+                    plugin_grp._add_broadcast_evt(evt, func)
         return plugin_ins
     except NotValidPluginError as err:
         Print.print_err(f"插件 {plugin_dirname} 不合法: {err.args[0]}")
         raise SystemExit from err
     except Cfg.ConfigError as err:
         Print.print_err(f"插件 {plugin_dirname} 配置文件报错：{err}")
         Print.print_err("你也可以直接删除配置文件, 重新启动ToolDelta以自动生成配置文件")
         raise SystemExit from err
-    except Builtins.SimpleJsonDataReader.DataReadError as err:
+    except Utils.SimpleJsonDataReader.DataReadError as err:
         Print.print_err(f"插件 {plugin_dirname} 读取数据失败: {err}")
     except plugin_grp.linked_frame.SystemVersionException as err:
         Print.print_err(f"插件 {plugin_dirname} 需要更高版本的ToolDelta加载: {err}")
     except Exception as err:
         Print.print_err(f"加载插件 {plugin_dirname} 出现问题, 报错如下: ")
         Print.print_err("§c" + traceback.format_exc())
         raise SystemExit from err
     finally:
         plugin_grp.plugin_added_cache["plugin"] = None
         plugin_grp.plugin_added_cache["packets"].clear()
         plugin_grp.pluginAPI_added_cache.clear()
         plugin_grp.broadcast_evts_cache.clear()
     return None
+
+def _unzip_plugin(zip_dir: str, exp_dir: str) -> None:
+    """解压插件ZIP包
+
+    Args:
+        zip_dir (str): 压缩文件路径
+        exp_dir (str): 解压目录
+    """
+    try:
+        f = zipfile.ZipFile(zip_dir, "r")
+        f.extractall(exp_dir)
+    except Exception as err:
+        Print.print_err(f"zipfile: 解压失败: {err}")
+        raise EOFError("解压失败") from err
```

### Comparing `tooldelta-0.5.9/tooldelta/plugin_load/injected_plugin/__init__.py` & `tooldelta-0.6.0/tooldelta/plugin_load/injected_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.9/tooldelta/plugin_load/injected_plugin/movent.py` & `tooldelta-0.6.0/tooldelta/plugin_load/injected_plugin/movent.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 "注入式执行函数"
 import time
 from typing import TYPE_CHECKING, Any, Optional
-from tooldelta.color_print import Print
-from tooldelta.packets import Packet_CommandOutput
+from ...color_print import Print
+from ...packets import Packet_CommandOutput
+from ..utils import (
+    getTarget,
+    getPos
+)
+
 if TYPE_CHECKING:
     from tooldelta.frame import Frame, GameCtrl
 
 
 def check_avaliable(sth: "GameCtrl") -> Optional[AttributeError]:
     """
     检查给定的 "GameCtrl" 对象是否可用
@@ -138,40 +143,14 @@
     check_avaliable(game_control)
     if playername not in get_all_player():
         return False
     # 检测框架是否为"Frame"NeOmg
     if movent_frame.launcher.is_op is not None:
         return movent_frame.launcher.is_op(playername)
 
-
-def getTarget(sth: str, timeout: bool | int = 5) -> list:
-    """
-    获取符合目标选择器实体的列表
-
-    参数:
-        sth: 目标选择器
-        timeout: 超时时间，默认为5秒
-    """
-    check_avaliable(game_control)
-    if not sth.startswith("@"):
-        raise ValueError("Minecraft Target Selector is not correct.")
-    result = sendwscmd(f"/testfor {sth}", True, timeout)
-    if result is None:
-        raise ValueError("Failed to get the target.")
-    result = (
-        result
-        .OutputMessages[0]
-        .Parameters
-    )
-    if result:
-        result = result[0]
-        return result.split(", ")
-    raise ValueError("Failed to get the target.")
-
-
 def find_key_from_value(dic: dict, val: Any) -> Optional[Any]:
     """
     从字典中根据值查找对应的键
 
     参数:
         dic: 目标字典
         val: 目标值
@@ -183,76 +162,14 @@
 
 def get_robotname() -> str | None:
     """获取机器人名称。"""
     check_avaliable(game_control)
     return game_control.bot_name
 
 
-def getPos(targetNameToGet: str, timeout: float | int = 5) -> dict:
-    """获取目标玩家的位置信息
-
-    参数:
-        targetNameToGet: 目标玩家的名称
-        timeout: 超时时间（秒）。默认为5秒
-
-    异常:
-        ValueError: 当目标玩家不存在时抛出该异常
-        ValueError: 当获取位置信息失败时抛出该异常
-        AttributeError: 当获取玩家UUID失败时抛出该异常
-    """
-    check_avaliable(game_control)
-    if targetNameToGet not in get_all_player() or targetNameToGet.startswith("@"):
-        raise ValueError(f"Player {targetNameToGet} does not exist.")
-    result = sendwscmd(
-        f'/querytarget @a[name="{targetNameToGet}"]', True, timeout)
-    if isinstance(result, type(None)):
-        raise ValueError("Failed to get the position.")
-    if not result.OutputMessages[0].Success:
-        raise ValueError(
-            f"Failed to get the position: {result.OutputMessages[0]}")
-    parameter = result.OutputMessages[0].Parameters[0]
-    if isinstance(parameter, str):
-        raise ValueError("Failed to get the position.")
-    result = {}
-
-    if game_control.players_uuid is None:
-        raise AttributeError("Failed to get the players_uuid.")
-    targetName = targetNameToGet
-    x = (
-        parameter[0]["position"]["x"]
-        if parameter[0]["position"]["x"] >= 0
-        else parameter[0]["position"]["x"] - 1
-    )
-    y = parameter[0]["position"]["y"] - 1.6200103759765
-    z = (
-        parameter[0]["position"]["z"]
-        if parameter[0]["position"]["z"] >= 0
-        else parameter[0]["position"]["z"] - 1
-    )
-    position = {
-        "x": float(f"{x:.2f}"),
-        "y": float(f"{y:.2f}"),
-        "z": float(f"{z:.2f}"),
-    }
-    dimension = parameter[0]["dimension"]
-    yRot = parameter[0]["yRot"]
-    result[targetName] = {
-        "dimension": dimension,
-        "position": position,
-        "yRot": yRot,
-    }
-    if targetNameToGet == "@a":
-        return result
-    if len(result) != 1:
-        raise ValueError("Failed to get the position.")
-    if targetNameToGet.startswith("@a"):
-        return list(result.values())[0]
-    return result[targetNameToGet]
-
-
 def countdown(delay: int | float, msg: str | None = None) -> None:
     """
     倒计时函数
 
     参数:
         delay: 延迟时间，可以是整数或浮点数
         msg: 倒计时消息，可选参数，默认为"Countdown"
```

### Comparing `tooldelta-0.5.9/tooldelta/plugin_manager.py` & `tooldelta-0.6.0/tooldelta/plugin_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 import os
 import platform
 import shutil
 import shlex
 import time
 from typing import Optional
 import ujson as json
-from .builtins import Builtins
+from .utils import Utils
 from .color_print import Print
 from .plugin_market import market
 from .plugin_load import PluginRegData
 from .constants import (
     TOOLDELTA_PLUGIN_DIR,
     TOOLDELTA_CLASSIC_PLUGIN,
     TOOLDELTA_INJECTED_PLUGIN
 )
 
-JsonIO = Builtins.SimpleJsonDataReader
+JsonIO = Utils.SimpleJsonDataReader
 
 if platform.system().lower() == "windows":
     CLS_CMD = "cls"
 else:
     CLS_CMD = "clear"
 
 
@@ -39,17 +39,17 @@
         "插件管理界面"
         clear_screen()
         np = self.autoRegisterPlugins()
         if np > 0:
             Print.clean_print(f"§a已自动注册{np}个未被注册的插件.")
         while 1:
             plugins = self.list_plugins_list()
-            Print.clean_print("§f输入§bu§f更新本地所有插件, §f输入§cq§f退出")
-            Print.clean_print("§f输入§ds§f同步插件注册表信息(在手动安装插件后使用)")
-            r = input(Print.clean_fmt("§f输入插件关键词进行选择\n(空格可分隔关键词):"))
+            with Print.lock:Print.clean_print("§f输入§bu§f更新本地所有插件, §f输入§cq§f退出")
+            with Print.lock:Print.clean_print("§f输入§ds§f同步插件注册表信息(在手动安装插件后使用)")
+            with Print.lock:r = input(Print.clean_fmt("§f输入插件关键词进行选择\n(空格可分隔关键词):"))
             r1 = r.strip().lower()
             if r1 == "":
                 continue
             elif r1 == "s":
                 self.sync_plugin_datas_to_register()
                 Print.clean_print("§a同步插件注册表数据成功.")
                 time.sleep(2)
@@ -184,15 +184,15 @@
             Print.clean_print("§c没有任何已安装插件匹配得上关键词")
             return None
         if len(res) > 1:
             Print.clean_print("§a☑ §f关键词查找到的插件:")
             for i, plugin in enumerate(res):
                 Print.clean_print(str(i + 1) + ". " +
                                   self.make_plugin_icon(plugin))
-            r = Builtins.try_int(input(Print.clean_fmt("§f请选择序号: ")))
+            r = Utils.try_int(input(Print.clean_fmt("§f请选择序号: ")))
             if r is None or r not in range(1, len(res) + 1):
                 Print.clean_print("§c序号无效, 回车键继续")
                 return None
             return res[r - 1]
         return res[0]
 
     @staticmethod
@@ -336,15 +336,15 @@
                     or os.path.exists(os.path.join("插件文件", f_dirname[p.plugin_type], p.name + "+disabled"))
                 ):
                     res.append(p)
                     r0[p.plugin_type].append(p.name)
         return r0, res
 
     def get_2_compare_plugins_reg(self) -> list[PluginRegData]:
-        """获取用于比较的插件注册信息列表
+        """获取用于比较的插件注册信息列表, 比较已注册与未注册插件
 
         Returns:
             list[PluginRegData]: 插件注册信息列表
         """
         f_plugins: list[PluginRegData] = []
         reg_dict, reg_list = self.get_plugin_reg_name_dict_and_datas()
         for p, k in {
```

### Comparing `tooldelta-0.5.9/tooldelta/plugin_market.py` & `tooldelta-0.6.0/tooldelta/plugin_market.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"插件商店生成与操作"
+"插件市场客户端"
 import os
 import platform
 import shutil
 import tempfile
 import traceback
 import time
 import shlex
 import requests
 import ujson as json
 from tooldelta import urlmethod
-from .builtins import Builtins
+from .utils import Utils
 from .color_print import Print
 from .plugin_load import PluginRegData
 from .cfg import Cfg
 from .constants import (
     PLUGIN_MARKET_SOURCE_OFFICIAL,
     TOOLDELTA_CLASSIC_PLUGIN,
     TOOLDELTA_INJECTED_PLUGIN
@@ -150,15 +150,15 @@
                 if last_operation == "+":
                     now_index += CTXS
                 elif last_operation == "-":
                     now_index -= CTXS
                 elif last_operation == "q":
                     break
                 else:
-                    res = Builtins.try_int(last_operation)
+                    res = Utils.try_int(last_operation)
                     if res:
                         if res in range(1, all_indexes + 1):
                             plugin_data = self.get_plugin_data_from_market(
                                 plugins_list[res - 1][0])
                             ok, pres = self.choice_plugin(plugin_data)
                             if ok:
                                 if in_game:
```

### Comparing `tooldelta-0.5.9/tooldelta/starter.py` & `tooldelta-0.6.0/tooldelta/starter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 """ToolDelta 启动器"""
 import os
 import time
 import traceback
-from .builtins import tmpjson_save_thread
+from .utils import tmpjson_save_thread
 from .urlmethod import check_update
+from .sys_args import sys_args_to_dict
 from .frame import Frame, GameCtrl
 from .color_print import Print
 from .plugin_load.PluginGroup import plugin_group
 from .plugin_load.injected_plugin import movent
 
 frame = Frame()
 
-
 def start_tool_delta() -> None:
     """启动ToolDelta"""
-    plugin_group.set_frame(frame)
     try:
         frame.welcome()
-        check_update()
+        if "no-update-check" not in sys_args_to_dict().keys():
+            check_update()
+        else:
+            Print.print_war("将不会进行自动更新.")
         frame.basic_operation()
         frame.loadConfiguration()
         game_control = GameCtrl(frame)
         frame.set_game_control(game_control)
         frame.set_plugin_group(plugin_group)
-        movent.set_frame(frame)
+        plugin_group.set_frame(frame)
         plugin_group.read_all_plugins()
         frame.plugin_load_finished(plugin_group)
         tmpjson_save_thread()
         frame.launcher.listen_launched(game_control.Inject)
         game_control.set_listen_packets()
         raise frame.launcher.launch()
     except (KeyboardInterrupt, SystemExit, EOFError):
```

### Comparing `tooldelta-0.5.9/tooldelta/urlmethod.py` & `tooldelta-0.6.0/tooldelta/urlmethod.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""自定义使用方法"""
+"""自定义常用URL方法"""
 import os
 import re
 import shutil
 import socket
 import time
 from typing import Union
 from concurrent.futures import ThreadPoolExecutor, as_completed
@@ -245,25 +245,27 @@
             except OSError:
                 Print.print_war(f"端口 {port} 正被占用, 跳过")
     raise ValueError(f"未找到空闲端口({start}~{end})")
 
 
 def check_update() -> None:
     """检查更新"""
-    latest_version: str = requests.get(
-        "https://api.github.com/repos/ToolDelta/ToolDelta/releases/latest", timeout=5).json()["tag_name"]
-    current_version = ".".join(
-        map(str, get_tool_delta_version()[:3]))
-
-    if not latest_version.replace(".", "") <= current_version.replace(".", ""):
-        # Print.print_suc(f"当前为最新版本 -> v{current_version}，无需更新")
-        Print.print_load(
-            f"检测到最新版本 {current_version} -> {latest_version}，请及时更新!"
-        )
-
+    try:
+        latest_version: str = requests.get(
+            "https://api.github.com/repos/ToolDelta/ToolDelta/releases/latest", timeout=5).json()["tag_name"]
+        current_version = ".".join(
+            map(str, get_tool_delta_version()[:3]))
+
+        if not latest_version.replace(".", "") <= current_version.replace(".", ""):
+            # Print.print_suc(f"当前为最新版本 -> v{current_version}，无需更新")
+            Print.print_load(
+                f"检测到最新版本 {current_version} -> {latest_version}，请及时更新!"
+            )
+    except KeyError:
+        Print.print_war("获取最新版本失败，请检查网络连接")
 
 def if_token() -> None:
     """检查路径下是否有fbtoken，没有就提示输入
 
     Raises:
         SystemExit: 未输入fbtoken
     """
```

### Comparing `tooldelta-0.5.9/PKG-INFO` & `tooldelta-0.6.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,32 @@
 Metadata-Version: 2.1
 Name: Tooldelta
-Version: 0.5.9
+Version: 0.6.0
 Summary: Plugin Loader for NeteaseRentalServer on Panel
 Home-page: https://github.com/SuperScript-PRC/ToolDelta
 Author: SuperScript-PRC
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
+Requires-Dist: fcwslib (>=3.0.0,<4.0.0)
 Requires-Dist: flask (>=3.0.2,<4.0.0)
 Requires-Dist: mido (>=1.3.2,<2.0.0)
-Requires-Dist: nbt (==1.5.1)
 Requires-Dist: pillow (>=10.2.0,<11.0.0)
 Requires-Dist: psutil (==5.9.8)
-Requires-Dist: pymysql (==1.1.0)
 Requires-Dist: pyspeedtest (==1.2.7)
 Requires-Dist: python-socketio (==5.11.1)
-Requires-Dist: qrcode (==7.4.2)
 Requires-Dist: requests (==2.31.0)
-Requires-Dist: rich (==13.7.0)
 Requires-Dist: shellescape (>=3.8.1,<4.0.0)
-Requires-Dist: tqdm (==4.66.2)
 Requires-Dist: ujson (==5.9.0)
 Requires-Dist: websocket-client (>=1.7.0,<2.0.0)
-Requires-Dist: websockets (==12.0)
 Project-URL: Repository, https://github.com/SuperScript-PRC/ToolDelta
 Description-Content-Type: text/markdown
 
 <h1 align="center">ToolDelta - Multi Platform Edition</h1>
 <p align="center">
   <a href="https://github.com/ToolDelta/ToolDelta/releases"><img src="https://img.shields.io/github/v/release/ToolDelta/ToolDelta?display_name=tag&sort=semver" alt="Releases"></a>
   <img src="https://img.shields.io/github/stars/ToolDelta/ToolDelta.svg?style=falt" alt="Stars">
```

#### html2text {}

```diff
@@ -1,24 +1,22 @@
-Metadata-Version: 2.1 Name: Tooldelta Version: 0.5.9 Summary: Plugin Loader for
+Metadata-Version: 2.1 Name: Tooldelta Version: 0.6.0 Summary: Plugin Loader for
 NeteaseRentalServer on Panel Home-page: https://github.com/SuperScript-PRC/
 ToolDelta Author: SuperScript-PRC Requires-Python: >=3.9,<3.13 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: aiohttp (>=3.9.3,<4.0.0) Requires-Dist: colorama
-(>=0.4.6,<0.5.0) Requires-Dist: flask (>=3.0.2,<4.0.0) Requires-Dist: mido
-(>=1.3.2,<2.0.0) Requires-Dist: nbt (==1.5.1) Requires-Dist: pillow
-(>=10.2.0,<11.0.0) Requires-Dist: psutil (==5.9.8) Requires-Dist: pymysql
-(==1.1.0) Requires-Dist: pyspeedtest (==1.2.7) Requires-Dist: python-socketio
-(==5.11.1) Requires-Dist: qrcode (==7.4.2) Requires-Dist: requests (==2.31.0)
-Requires-Dist: rich (==13.7.0) Requires-Dist: shellescape (>=3.8.1,<4.0.0)
-Requires-Dist: tqdm (==4.66.2) Requires-Dist: ujson (==5.9.0) Requires-Dist:
-websocket-client (>=1.7.0,<2.0.0) Requires-Dist: websockets (==12.0) Project-
-URL: Repository, https://github.com/SuperScript-PRC/ToolDelta Description-
-Content-Type: text/markdown
+(>=0.4.6,<0.5.0) Requires-Dist: fcwslib (>=3.0.0,<4.0.0) Requires-Dist: flask
+(>=3.0.2,<4.0.0) Requires-Dist: mido (>=1.3.2,<2.0.0) Requires-Dist: pillow
+(>=10.2.0,<11.0.0) Requires-Dist: psutil (==5.9.8) Requires-Dist: pyspeedtest
+(==1.2.7) Requires-Dist: python-socketio (==5.11.1) Requires-Dist: requests
+(==2.31.0) Requires-Dist: shellescape (>=3.8.1,<4.0.0) Requires-Dist: ujson
+(==5.9.0) Requires-Dist: websocket-client (>=1.7.0,<2.0.0) Project-URL:
+Repository, https://github.com/SuperScript-PRC/ToolDelta Description-Content-
+Type: text/markdown
                ************ TToooollDDeellttaa -- MMuullttii PPllaattffoorrmm EEddiittiioonn ************
                                _[_R_e_l_e_a_s_e_s_][Stars]
                        _[_o_p_i_s_s_u_e_s_]_[_c_l_i_s_s_u_e_s_]_[_o_p_p_r_]_[_c_l_p_r_]
                TToooollDDeellttaa æ¯ä¾èµäº PPhhooeenniixxBBuuiillddeerr || NNeeoo OOmmeeggaa
     çå¤åè½æ©å±ç»ä»¶ï¼å¯ä»¥å è½½åç§åæ ·æè¶£çæä»¶ã
   TToooollDDeellttaa å¯ä»¥ä½¿å¾ä½ ç ?ä?¸?­?å??½?ç???ã???æ???ç???ä?¸??ç???ã???å??º?å?²?©?ç???ç?§??è?µ??æ??
                      çç©æ³ååè½æ´å å¤æ ·åã
```

