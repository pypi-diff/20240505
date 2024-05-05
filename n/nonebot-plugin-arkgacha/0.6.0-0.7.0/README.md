# Comparing `tmp/nonebot_plugin_arkgacha-0.6.0.tar.gz` & `tmp/nonebot_plugin_arkgacha-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_arkgacha-0.6.0.tar", last modified: Sun Mar 10 15:09:56 2024, max compression
+gzip compressed data, was "nonebot_plugin_arkgacha-0.7.0.tar", last modified: Sun May  5 14:24:20 2024, max compression
```

## Comparing `nonebot_plugin_arkgacha-0.6.0.tar` & `nonebot_plugin_arkgacha-0.7.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35182 2024-03-10 14:48:35.842394 nonebot_plugin_arkgacha-0.6.0/LICENSE
--rw-r--r--   0        0        0     2249 2024-03-10 14:48:35.842394 nonebot_plugin_arkgacha-0.6.0/README.md
--rw-r--r--   0        0        0     6501 2024-03-10 15:05:50.328155 nonebot_plugin_arkgacha-0.6.0/nonebot_plugin_arkgacha/__init__.py
--rw-r--r--   0        0        0     2852 2024-03-10 15:06:04.916635 nonebot_plugin_arkgacha-0.6.0/nonebot_plugin_arkgacha/__main__.py
--rw-r--r--   0        0        0      330 2024-03-10 14:48:35.843392 nonebot_plugin_arkgacha-0.6.0/nonebot_plugin_arkgacha/config.py
--rw-r--r--   0        0        0      822 2024-03-10 15:09:56.461570 nonebot_plugin_arkgacha-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2639 1970-01-01 00:00:00.000000 nonebot_plugin_arkgacha-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    35182 2024-03-10 14:48:35.842394 nonebot_plugin_arkgacha-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2315 2024-05-05 14:19:24.403033 nonebot_plugin_arkgacha-0.7.0/README.md
+-rw-r--r--   0        0        0     6940 2024-05-05 14:22:46.366580 nonebot_plugin_arkgacha-0.7.0/nonebot_plugin_arkgacha/__init__.py
+-rw-r--r--   0        0        0     2852 2024-03-10 15:06:04.916635 nonebot_plugin_arkgacha-0.7.0/nonebot_plugin_arkgacha/__main__.py
+-rw-r--r--   0        0        0      371 2024-05-05 14:19:24.420558 nonebot_plugin_arkgacha-0.7.0/nonebot_plugin_arkgacha/config.py
+-rw-r--r--   0        0        0      819 2024-05-05 14:24:20.885898 nonebot_plugin_arkgacha-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2701 1970-01-01 00:00:00.000000 nonebot_plugin_arkgacha-0.7.0/PKG-INFO
```

### Comparing `nonebot_plugin_arkgacha-0.6.0/LICENSE` & `nonebot_plugin_arkgacha-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arkgacha-0.6.0/README.md` & `nonebot_plugin_arkgacha-0.7.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 ## 配置
 
 - ARKGACHA_PROXY: 代理配置，默认为空
 - ARKGACHA_POOL_FILE: 抽卡池文件路径, 不填则使用 [`localstore`](https://github.com/nonebot/plugin-localstore) 保存抽卡池
 - ARKGACHA_MAX: 抽卡最大次数, 默认为 300
 - ARKGACHA_PURE_TEXT: 是否使用纯文本, 默认为 False (十连模拟必须使用图片)
 - ARKGACHA_AUTO_UPDATE: 是否自动更新，默认为 True
+- ARKGACHA_REPLY_SENDER: 是否回复发送者，默认为 False
 
 ## 注意事项
 1. `方舟抽卡` 不需要图片资源, 可在不经过 `nb arkgacha init` 或 `arkkit init` 的情况下使用
 2. `方舟十连` 需要图片资源, 需要先在命令行中执行 `nb arkgacha init` 或 `arkkit init -SIMG` 初始化资源，否则会出现错误
 3. 若配置，每天 16 点将自动更新卡池资源
 4. 如果获取资源时出现网络错误，请检查代理设置，或尝试访问 PRTS
```

#### html2text {}

```diff
@@ -8,15 +8,16 @@
 **å¨ä½¿ç¨è¯¥æä»¶ä¹åï¼éè¦ååå§åèµæº** å½ä»¤è¡è¾å¥ï¼
 ```bash nb arkgacha init ``` æ ```bash arkkit init -SIMG ``` ## éç½® -
 ARKGACHA_PROXY: ä»£çéç½®ï¼é»è®¤ä¸ºç©º - ARKGACHA_POOL_FILE:
 æ½å¡æ± æä»¶è·¯å¾, ä¸å¡«åä½¿ç¨ [`localstore`](https://github.com/
 nonebot/plugin-localstore) ä¿å­æ½å¡æ±  - ARKGACHA_MAX: æ½å¡æå¤§æ¬¡æ°,
 é»è®¤ä¸º 300 - ARKGACHA_PURE_TEXT: æ¯å¦ä½¿ç¨çº¯ææ¬, é»è®¤ä¸º False
 (åè¿æ¨¡æå¿é¡»ä½¿ç¨å¾ç) - ARKGACHA_AUTO_UPDATE:
-æ¯å¦èªå¨æ´æ°ï¼é»è®¤ä¸º True ## æ³¨æäºé¡¹ 1. `æ¹èæ½å¡`
+æ¯å¦èªå¨æ´æ°ï¼é»è®¤ä¸º True - ARKGACHA_REPLY_SENDER:
+æ¯å¦åå¤åéèï¼é»è®¤ä¸º False ## æ³¨æäºé¡¹ 1. `æ¹èæ½å¡`
 ä¸éè¦å¾çèµæº, å¯å¨ä¸ç»è¿ `nb arkgacha init` æ `arkkit init`
 çæåµä¸ä½¿ç¨ 2. `æ¹èåè¿` éè¦å¾çèµæº,
 éè¦åå¨å½ä»¤è¡ä¸­æ§è¡ `nb arkgacha init` æ `arkkit init -SIMG`
 åå§åèµæºï¼å¦åä¼åºç°éè¯¯ 3. è¥éç½®ï¼æ¯å¤© 16
 ç¹å°èªå¨æ´æ°å¡æ± èµæº 4.
 å¦æè·åèµæºæ¶åºç°ç½ç»éè¯¯ï¼è¯·æ£æ¥ä»£çè®¾ç½®ï¼æå°è¯è®¿é®
 PRTS ## ä½¿ç¨æ¹æ³ æä»¤å¦ä¸: > æ¹èæ½å¡ > > æ¹èæ½å¡ 200 > >
```

### Comparing `nonebot_plugin_arkgacha-0.6.0/nonebot_plugin_arkgacha/__init__.py` & `nonebot_plugin_arkgacha-0.7.0/nonebot_plugin_arkgacha/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 from nonebot.adapters import Event
 from nonebot.plugin import PluginMetadata, inherit_supported_adapters
 
 require("nonebot_plugin_alconna")
 require("nonebot_plugin_localstore")
 require("nonebot_plugin_apscheduler")
 
-from nonebot_plugin_alconna import Match, UniMessage, SerializeFailed, on_alconna
+from nonebot_plugin_alconna import Match, UniMessage, SerializeFailed, on_alconna, MsgTarget, SupportScope
 from nonebot_plugin_localstore import get_cache_file, get_data_file
 from nonebot_plugin_apscheduler import scheduler
 
 from .config import Config
 
 driver = get_driver()
 _config = get_plugin_config(Config)
-__version__ = "0.6.0"
+__version__ = "0.7.0"
 __plugin_meta__ = PluginMetadata(
     name="明日方舟抽卡模拟",
     description="明模拟日方舟抽卡功能，支持模拟十连",
     usage="""\
 方舟抽卡 [count = 10]
 方舟十连
 方舟抽卡帮助
@@ -52,15 +52,15 @@
 user_cache_file = get_cache_file("arkgacha", "user.json")
 if not user_cache_file.exists():
     userdata = {}
 else:
     with user_cache_file.open("r", encoding="utf-8") as f:
         userdata = json.load(f)
 
-gacha_regex = on_alconna(
+gacha_cmd = on_alconna(
     Alconna(
         "方舟抽卡", Args["count", int, 10],
         meta=CommandMeta(
             description="文字版抽卡，可以转图片发送",
             usage=f"方舟抽卡 [count = 10], count不会超过{_config.arkgacha_max}",
             example="方舟抽卡 10",
             compact=True
@@ -126,16 +126,16 @@
             except (ActionFailed, NetworkError, SerializeFailed):
                 await update_regex.send(text)
         await update_regex.finish()
     else:
         await update_regex.finish("卡池已是最新")
 
 
-@gacha_regex.handle()
-async def _(event: Event, count: Match[int]):
+@gacha_cmd.handle()
+async def _(event: Event, count: Match[int], target: MsgTarget):
     session = event.get_user_id()
     if session not in userdata:
         user = GachaUser()
         userdata[session] = asdict(user)
     else:
         user = GachaUser(**userdata[session])
     _count = min(max(int(count.result), 1), _config.arkgacha_max)
@@ -156,37 +156,43 @@
         f"六星角色：\n" +
         "\n".join(f"{i} x{get_six[i]}" for i in get_six) +
         "\n五星角色：\n" +
         "\n".join(f"{i} x{get_five[i]}" for i in get_five) +
         "\n四星角色：\n" +
         f"共{four_count}个四星"
     )
+    reply_to = _config.arkgacha_reply_sender
+    if target.scope is SupportScope.qq_api and not target.parent_id:
+        reply_to = False
     if _config.arkgacha_pure_text:
-        await gacha_regex.send(text)
+        await UniMessage.text(text).send(reply_to=reply_to)
     else:
         img = gacha.create_image(user, data, _count, True)
         try:
-            await UniMessage.image(raw=img, mimetype="image/jpeg").send()
+            await UniMessage.image(raw=img, mimetype="image/jpeg").send(reply_to=reply_to)
         except (ActionFailed, NetworkError, SerializeFailed):
-            await gacha_regex.send(text)
+            await UniMessage.text(text).send(reply_to=reply_to)
     userdata[session] = asdict(user)
-    await gacha_regex.finish()
+    await gacha_cmd.finish()
 
 
 @simulate_regex.handle()
-async def _(event: Event):
+async def _(event: Event, target: MsgTarget):
     from arknights_toolkit.gacha.simulate import simulate_image
 
     session = event.get_user_id()
     if session not in userdata:
         user = GachaUser()
         userdata[session] = asdict(user)
     else:
         user = GachaUser(**userdata[session])
     res = gacha.gacha(user, 10)
     img = await simulate_image(res[0], proxy=_config.arkgacha_proxy)
+    reply_to = _config.arkgacha_reply_sender
+    if target.scope is SupportScope.qq_api and not target.parent_id:
+        reply_to = False
     try:
-        await UniMessage.image(raw=img, mimetype="image/jpeg").send()
+        await UniMessage.image(raw=img, mimetype="image/jpeg").send(reply_to=reply_to)
     except (ActionFailed, NetworkError, SerializeFailed):
-        await simulate_regex.send("图片发送失败")
+        await UniMessage.text("图片发送失败").send(reply_to=reply_to)
     userdata[session] = asdict(user)
-    await gacha_regex.finish()
+    await gacha_cmd.finish()
```

### Comparing `nonebot_plugin_arkgacha-0.6.0/nonebot_plugin_arkgacha/__main__.py` & `nonebot_plugin_arkgacha-0.7.0/nonebot_plugin_arkgacha/__main__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arkgacha-0.6.0/pyproject.toml` & `nonebot_plugin_arkgacha-0.7.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [project]
 name = "nonebot-plugin-arkgacha"
-version = "0.6.0"
+version = "0.7.0"
 description = "Plugin for Arknights gacha, support multi platform"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
-    "nonebot2>=2.2.1",
-    "nonebot-plugin-alconna>=0.40.0rc3",
-    "arknights-toolkit>=0.6.4",
+    "nonebot2>=2.3.0",
+    "nonebot-plugin-alconna>=0.45.3",
+    "arknights-toolkit>=0.7.2",
     "nonebot-plugin-localstore>=0.6.0",
     "nonebot-plugin-apscheduler>=0.4.0",
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
 
 [project.entry-points.nb_scripts]
 arkgacha = "nonebot_plugin_arkgacha.__main__:main"
@@ -24,16 +24,16 @@
 [tool.pdm.build]
 includes = [
     "nonebot_plugin_arkgacha",
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "nonebot-adapter-qq>=1.4.2",
-    "nonebot2[httpx,websockets]>=2.2.1",
+    "nonebot-adapter-qq>=1.4.4",
+    "nonebot2[httpx,websockets]>=2.3.0",
 ]
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `nonebot_plugin_arkgacha-0.6.0/PKG-INFO` & `nonebot_plugin_arkgacha-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-arkgacha
-Version: 0.6.0
+Version: 0.7.0
 Summary: Plugin for Arknights gacha, support multi platform
 Author-Email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
-Requires-Python: >=3.8
-Requires-Dist: nonebot2>=2.2.1
-Requires-Dist: nonebot-plugin-alconna>=0.40.0rc3
-Requires-Dist: arknights-toolkit>=0.6.4
+Requires-Python: >=3.9
+Requires-Dist: nonebot2>=2.3.0
+Requires-Dist: nonebot-plugin-alconna>=0.45.3
+Requires-Dist: arknights-toolkit>=0.7.2
 Requires-Dist: nonebot-plugin-localstore>=0.6.0
 Requires-Dist: nonebot-plugin-apscheduler>=0.4.0
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
 </p>
@@ -64,14 +64,15 @@
 ## 配置
 
 - ARKGACHA_PROXY: 代理配置，默认为空
 - ARKGACHA_POOL_FILE: 抽卡池文件路径, 不填则使用 [`localstore`](https://github.com/nonebot/plugin-localstore) 保存抽卡池
 - ARKGACHA_MAX: 抽卡最大次数, 默认为 300
 - ARKGACHA_PURE_TEXT: 是否使用纯文本, 默认为 False (十连模拟必须使用图片)
 - ARKGACHA_AUTO_UPDATE: 是否自动更新，默认为 True
+- ARKGACHA_REPLY_SENDER: 是否回复发送者，默认为 False
 
 ## 注意事项
 1. `方舟抽卡` 不需要图片资源, 可在不经过 `nb arkgacha init` 或 `arkkit init` 的情况下使用
 2. `方舟十连` 需要图片资源, 需要先在命令行中执行 `nb arkgacha init` 或 `arkkit init -SIMG` 初始化资源，否则会出现错误
 3. 若配置，每天 16 点将自动更新卡池资源
 4. 如果获取资源时出现网络错误，请检查代理设置，或尝试访问 PRTS
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-arkgacha Version: 0.6.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-arkgacha Version: 0.7.0 Summary:
 Plugin for Arknights gacha, support multi platform Author-Email: RF-Tar-Railt
-qq.com> License: MIT Requires-Python: >=3.8 Requires-Dist: nonebot2>=2.2.1
-Requires-Dist: nonebot-plugin-alconna>=0.40.0rc3 Requires-Dist: arknights-
-toolkit>=0.6.4 Requires-Dist: nonebot-plugin-localstore>=0.6.0 Requires-Dist:
+qq.com> License: MIT Requires-Python: >=3.9 Requires-Dist: nonebot2>=2.3.0
+Requires-Dist: nonebot-plugin-alconna>=0.45.3 Requires-Dist: arknights-
+toolkit>=0.7.2 Requires-Dist: nonebot-plugin-localstore>=0.6.0 Requires-Dist:
 nonebot-plugin-apscheduler>=0.4.0 Description-Content-Type: text/markdown
                                    _[_n_o_n_e_b_o_t_]
         # NoneBot Plugin Arkgacha _â¨ ææ¥æ¹èæ½å¡æ¨¡æå¨ â¨_
                             _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 è¯¥æä»¶æä¾äºæ¨¡æææ¥æ¹èæ½å¡çåè½ï¼åæ¬æ å¤´å½¢å¼çæ½å¡æ¨¡æä¸æ¨¡æåè¿
 éè¿ä½¿ç¨ [`plugin-alconna`](https://github.com/nonebot/plugin-alconna)
 æä»¶ééå¤å¹³å° ## å®è£ ```bash $ pip install nonebot-plugin-arkgacha
@@ -14,15 +14,16 @@
 **å¨ä½¿ç¨è¯¥æä»¶ä¹åï¼éè¦ååå§åèµæº** å½ä»¤è¡è¾å¥ï¼
 ```bash nb arkgacha init ``` æ ```bash arkkit init -SIMG ``` ## éç½® -
 ARKGACHA_PROXY: ä»£çéç½®ï¼é»è®¤ä¸ºç©º - ARKGACHA_POOL_FILE:
 æ½å¡æ± æä»¶è·¯å¾, ä¸å¡«åä½¿ç¨ [`localstore`](https://github.com/
 nonebot/plugin-localstore) ä¿å­æ½å¡æ±  - ARKGACHA_MAX: æ½å¡æå¤§æ¬¡æ°,
 é»è®¤ä¸º 300 - ARKGACHA_PURE_TEXT: æ¯å¦ä½¿ç¨çº¯ææ¬, é»è®¤ä¸º False
 (åè¿æ¨¡æå¿é¡»ä½¿ç¨å¾ç) - ARKGACHA_AUTO_UPDATE:
-æ¯å¦èªå¨æ´æ°ï¼é»è®¤ä¸º True ## æ³¨æäºé¡¹ 1. `æ¹èæ½å¡`
+æ¯å¦èªå¨æ´æ°ï¼é»è®¤ä¸º True - ARKGACHA_REPLY_SENDER:
+æ¯å¦åå¤åéèï¼é»è®¤ä¸º False ## æ³¨æäºé¡¹ 1. `æ¹èæ½å¡`
 ä¸éè¦å¾çèµæº, å¯å¨ä¸ç»è¿ `nb arkgacha init` æ `arkkit init`
 çæåµä¸ä½¿ç¨ 2. `æ¹èåè¿` éè¦å¾çèµæº,
 éè¦åå¨å½ä»¤è¡ä¸­æ§è¡ `nb arkgacha init` æ `arkkit init -SIMG`
 åå§åèµæºï¼å¦åä¼åºç°éè¯¯ 3. è¥éç½®ï¼æ¯å¤© 16
 ç¹å°èªå¨æ´æ°å¡æ± èµæº 4.
 å¦æè·åèµæºæ¶åºç°ç½ç»éè¯¯ï¼è¯·æ£æ¥ä»£çè®¾ç½®ï¼æå°è¯è®¿é®
 PRTS ## ä½¿ç¨æ¹æ³ æä»¤å¦ä¸: > æ¹èæ½å¡ > > æ¹èæ½å¡ 200 > >
```

