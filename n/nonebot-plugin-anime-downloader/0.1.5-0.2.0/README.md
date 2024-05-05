# Comparing `tmp/nonebot_plugin_anime_downloader-0.1.5.tar.gz` & `tmp/nonebot_plugin_anime_downloader-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_anime_downloader-0.1.5.tar", last modified: Fri May  3 14:36:37 2024, max compression
+gzip compressed data, was "nonebot_plugin_anime_downloader-0.2.0.tar", last modified: Sun May  5 05:28:51 2024, max compression
```

## Comparing `nonebot_plugin_anime_downloader-0.1.5.tar` & `nonebot_plugin_anime_downloader-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1062 2024-05-03 14:36:02.688340 nonebot_plugin_anime_downloader-0.1.5/LICENSE
--rw-r--r--   0        0        0     3751 2024-05-03 14:36:02.688340 nonebot_plugin_anime_downloader-0.1.5/README.md
--rw-r--r--   0        0        0    11717 2024-05-03 14:36:02.688340 nonebot_plugin_anime_downloader-0.1.5/nonebot_plugin_anime_downloader/__init__.py
--rw-r--r--   0        0        0     4761 2024-05-03 14:36:02.688340 nonebot_plugin_anime_downloader-0.1.5/nonebot_plugin_anime_downloader/acgrip/__init__.py
--rw-r--r--   0        0        0      654 2024-05-03 14:36:02.688340 nonebot_plugin_anime_downloader-0.1.5/nonebot_plugin_anime_downloader/config.py
--rw-r--r--   0        0        0      698 2024-05-03 14:36:02.688340 nonebot_plugin_anime_downloader-0.1.5/nonebot_plugin_anime_downloader/data_source.py
--rw-r--r--   0        0        0     1609 2024-05-03 14:36:02.688340 nonebot_plugin_anime_downloader-0.1.5/nonebot_plugin_anime_downloader/downloader/__init__.py
--rw-r--r--   0        0        0     1214 2024-05-03 14:36:02.688340 nonebot_plugin_anime_downloader-0.1.5/nonebot_plugin_anime_downloader/downloader/models.py
--rw-r--r--   0        0        0      175 2024-05-03 14:36:02.688340 nonebot_plugin_anime_downloader-0.1.5/nonebot_plugin_anime_downloader/models.py
--rw-r--r--   0        0        0     1441 2024-05-03 14:36:02.688340 nonebot_plugin_anime_downloader-0.1.5/nonebot_plugin_anime_downloader/routes.py
--rw-r--r--   0        0        0      761 2024-05-03 14:36:02.688340 nonebot_plugin_anime_downloader-0.1.5/nonebot_plugin_anime_downloader/tasks.py
--rw-r--r--   0        0        0      316 2024-05-03 14:36:02.688340 nonebot_plugin_anime_downloader-0.1.5/nonebot_plugin_anime_downloader/templates/index.html
--rw-r--r--   0        0        0      897 2024-05-03 14:36:02.688340 nonebot_plugin_anime_downloader-0.1.5/nonebot_plugin_anime_downloader/test.py
--rw-r--r--   0        0        0     2659 2024-05-03 14:36:02.688340 nonebot_plugin_anime_downloader-0.1.5/nonebot_plugin_anime_downloader/utils.py
--rw-r--r--   0        0        0      730 2024-05-03 14:36:37.024333 nonebot_plugin_anime_downloader-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     4400 1970-01-01 00:00:00.000000 nonebot_plugin_anime_downloader-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-05 05:28:21.516542 nonebot_plugin_anime_downloader-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4232 2024-05-05 05:28:21.516542 nonebot_plugin_anime_downloader-0.2.0/README.md
+-rw-r--r--   0        0        0    15250 2024-05-05 05:28:21.516542 nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/__init__.py
+-rw-r--r--   0        0        0     4745 2024-05-05 05:28:21.516542 nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/acgrip/__init__.py
+-rw-r--r--   0        0        0      654 2024-05-05 05:28:21.516542 nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/config.py
+-rw-r--r--   0        0        0      698 2024-05-05 05:28:21.516542 nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/data_source.py
+-rw-r--r--   0        0        0     1609 2024-05-05 05:28:21.516542 nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/downloader/__init__.py
+-rw-r--r--   0        0        0     1214 2024-05-05 05:28:21.516542 nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/downloader/models.py
+-rw-r--r--   0        0        0      175 2024-05-05 05:28:21.516542 nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/models.py
+-rw-r--r--   0        0        0     2860 2024-05-05 05:28:21.516542 nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/routes.py
+-rw-r--r--   0        0        0      761 2024-05-05 05:28:21.516542 nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/tasks.py
+-rw-r--r--   0        0        0      481 2024-05-05 05:28:21.516542 nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/templates/index.html
+-rw-r--r--   0        0        0     3928 2024-05-05 05:28:21.516542 nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/utils.py
+-rw-r--r--   0        0        0      730 2024-05-05 05:28:51.884538 nonebot_plugin_anime_downloader-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4881 1970-01-01 00:00:00.000000 nonebot_plugin_anime_downloader-0.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_anime_downloader-0.1.5/LICENSE` & `nonebot_plugin_anime_downloader-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.5/README.md` & `nonebot_plugin_anime_downloader-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 
 ## 使用
 | 命令 | 别名 | 说明 | 示例 |
 | --- | --- | --- | --- |
 | sub | 订阅 | 通过 Tag 订阅番剧 | `sub Up to 21°C Nijiyon Animation 2 MP4` |
 | unsub | 取消订阅 | 通过 Tag 取消订阅番剧 | `unsub Up to 21°C Nijiyon Animation 2 MP4` |
 | listsub | sublist, 订阅列表 | 查看当前用户/群组的订阅列表 | `sublist` |
+| amnsc | 番剧搜索, 搜索番剧, animesearch | 通过关键词搜索番剧 | `amnsc Nijiyon Animation 2` |
+| amnd | 番剧下载, 下载番剧, animedownload | 通过 资源ID 下载番剧 | `amnd 114514` |
 
 这里的 Tag 就是用来在 ACG.RIP 搜索的关键词，番剧名、分辨率、字幕组等等，只要能在 ACG.RIP 搜索到的都可以
 
 > 记得加上你的命令头哦
 
 ## 效果
 
@@ -34,14 +36,19 @@
 1. Up to 21°C Nijiyon Animation 2 MP4
 
 (过了一段时间)
 
 **bot**: [Up to 21°C] Love Live！虹咲學園 學園偶像同好會 短篇動畫 第二季 / Nijiyon Animation 2 - 04 (ABEMA 1920x1080 AVC AAC MP4) 现在可以观看了！
 [http://example.com/anime/302322](http://example.com/anime/302322)
 
+**user**: `/amnd 302322`
+
+**bot**: [Up to 21°C] Love Live！虹咲學園 學園偶像同好會 短篇動畫 第二季 / Nijiyon Animation 2 - 04 (ABEMA 1920x1080 AVC AAC MP4) 现在可以观看了！
+[http://example.com/anime/302322](http://example.com/anime/302322)
+
 
 ## 安装方法
 <details open>
 <summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
     nb plugin install nonebot-plugin-anime-downloader
```

### Comparing `nonebot_plugin_anime_downloader-0.1.5/nonebot_plugin_anime_downloader/__init__.py` & `nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -21,28 +21,29 @@
 from nonebot_plugin_apscheduler import scheduler
 from nonebot_plugin_alconna import UniMessage, Target
 
 from .config import Config
 from .tasks import TaskManager
 from .routes import VideoManager
 from .downloader import TorrentDownloader
-from .utils import is_tag_match_title, generate_folder_name
 from .data_source import ACGRIPBase, UserBase, VideoBase, ACGRIPData, User, Video
+from .utils import is_tag_match_title, generate_folder_name, extract_tags_from_title
 from .acgrip import (
     make_request,
     extract_data,
+    get_anime_data,
     fetch_torrent_data,
     replace_html_entities,
 )
 
 
 __plugin_meta__ = PluginMetadata(
     name="番剧下载",
     description="基于 qBittorrent Web UI 的番剧下载 NoneBot 插件",
-    usage="/sub 订阅 Tag\n/unsub 取消订阅 Tag\n/listsub 查看订阅列表",
+    usage="/sub 订阅 Tag\n/unsub 取消订阅 Tag\n/listsub 查看订阅列表\n/anmsc 搜索番剧\n/anmd 下载番剧",
     type="application",
     homepage="https://github.com/zhaomaoniu/nonebot-plugin-anime-downloader",
     config=Config,
     supported_adapters=inherit_supported_adapters("nonebot_plugin_alconna"),
 )
 
 
@@ -88,14 +89,39 @@
 VideoBase.metadata.create_all(video_engine)
 
 acgrip_session = sessionmaker(bind=acg_rip_engine)()
 user_session = sessionmaker(bind=user_engine)()
 video_session = sessionmaker(bind=video_engine)()
 
 
+async def check_video_downloaded(title: str, torrent_id: int, user_id: str):
+    logger.info(f"Checking whether {title} is downloaded for {user_id}...")
+    if torrent_id in video_manager.ids:
+        logger.info(f"{title} is downloaded for {user_id}! Sending message...")
+        # send message to user
+        msg = (
+            f"{title} 现在可以观看了！\n"
+            + f"{plugin_config.anime_url}:{nonebot.get_driver().config.port}/anime/{torrent_id}"
+        )
+        chat_type = str(user_id).split("_")[0]
+        id_ = str(user_id).split("_")[-1]
+        target = Target(
+            id=id_,
+            parent_id=id_ if chat_type == "group" else "",
+            channel=chat_type == "group",
+            private=chat_type == "private",
+        )
+        await UniMessage(msg).send(target)
+        logger.info(f"Message sent to {user_id}!")
+
+        scheduler.remove_job(f"{title}_{user_id}")
+    else:
+        logger.info(f"{title} is not downloaded yet for {user_id}.")
+
+
 @scheduler.scheduled_job("interval", seconds=plugin_config.acgrip_interval)
 @nonebot.get_driver().on_startup
 async def fetch_acgrip_data():
     html_content = await make_request(base_url=plugin_config.acgrip_url)
     data = extract_data(replace_html_entities(html_content))
 
     # get new data
@@ -119,65 +145,58 @@
     users = user_session.query(User).all()
     for user in users:
         tags_str = user.tags
         tags_list: List[List[str]] = json.loads(tags_str)
         for tags in tags_list:
             for entry in new_data:
                 if is_tag_match_title(tags, entry["title"]):
+                    # check if the video is already downloaded
+                    if entry["id"] in video_manager.ids:
+                        # send message to user
+                        msg = (
+                            f"{entry['title']} 现在可以观看了！\n"
+                            + f"{plugin_config.anime_url}:{nonebot.get_driver().config.port}/anime/{entry['id']}"
+                        )
+                        chat_type = str(user.id).split("_")[0]
+                        id_ = str(user.id).split("_")[-1]
+                        target = Target(
+                            id=id_,
+                            parent_id=id_ if chat_type == "group" else "",
+                            channel=chat_type == "group",
+                            private=chat_type == "private",
+                        )
+                        await UniMessage(msg).send(target)
+                        continue
+
                     # start download torrent
                     logger.info(f"Downloading {entry['title']} for {user.id}...")
 
                     if str(entry["url"]).startswith("http"):
                         url = f"{entry['url']}.torrent"
                     else:
                         url = f"{plugin_config.acgrip_url}{entry['url']}.torrent"
 
                     torrent_data = await fetch_torrent_data(url)
-                    torrent_info = await torrent_downloader.download_torrent(
-                        torrent_data, generate_folder_name(tags)
-                    )
+                    try:
+                        torrent_info = await torrent_downloader.download_torrent(
+                            torrent_data, generate_folder_name(tags)
+                        )
+                    except Exception:
+                        logger.warning(
+                            f"Failed to download {entry['title']} for {user.id}! Probably due to the same torrent."
+                        )
                     task_manager.add(
                         {
                             "id": user.id,
                             "content": torrent_info,
                             "torrent_id": int(entry["id"]),
                         }
                     )
 
                     # set a scheduler to check if the video is downloaded
-                    async def check_video_downloaded(
-                        title: str, torrent_id: int, user_id: str
-                    ):
-                        logger.info(
-                            f"Checking whether {title} is downloaded for {user_id}..."
-                        )
-                        if torrent_id in video_manager.ids:
-                            logger.info(
-                                f"{title} is downloaded for {user_id}! Sending message..."
-                            )
-                            # send message to user
-                            msg = (
-                                f"{title} 现在可以观看了！\n"
-                                + f"{plugin_config.anime_url}:{nonebot.get_driver().config.port}/anime/{torrent_id}"
-                            )
-                            chat_type = str(user_id).split("_")[0]
-                            id_ = str(user_id).split("_")[-1]
-                            target = Target(
-                                id=id_,
-                                parent_id=id_ if chat_type == "group" else "",
-                                channel=chat_type == "group",
-                                private=chat_type == "private",
-                            )
-                            await UniMessage(msg).send(target)
-                            logger.info(f"Message sent to {user_id}!")
-
-                            scheduler.remove_job(f"{title}_{user_id}")
-                        else:
-                            logger.info(f"{title} is not downloaded yet for {user_id}.")
-
                     scheduler.add_job(
                         check_video_downloaded,
                         "interval",
                         seconds=10,
                         args=(entry["title"], int(entry["id"]), user.id),
                         id=f"{entry['title']}_{user.id}",
                     )
@@ -244,29 +263,35 @@
 async def get_target(event: Event) -> Target:
     return UniMessage.get_target(event)
 
 
 subscribes = on_command("sub", aliases={"订阅"}, priority=5)
 unsubscribes = on_command("unsub", aliases={"取消订阅"}, priority=5)
 list_subscribes = on_command("listsub", aliases={"订阅列表", "sublist"}, priority=5)
+search = on_command(
+    "anmsc", aliases={"番剧搜索", "搜索番剧", "搜番", "animesearch"}, priority=5
+)
+download = on_command(
+    "anmd", aliases={"番剧下载", "下载番剧", "下番", "animedownload"}, priority=5
+)
 
 
 @subscribes.handle()
 async def sub_handle(target: Target = Depends(get_target), arg: Message = CommandArg()):
     if arg.extract_plain_text() == "":
         await subscribes.finish("请提供 Tag！")
 
     args = arg.extract_plain_text().split(" ")
 
     if args == []:
         await subscribes.finish("请提供 Tag！")
 
     # check if the user is already subscribed the same tag
     id_ = f"{'private' if target.private else 'group'}_{target.id}"
-    print(id_, target.id, target.private)
+
     user = user_session.query(User).filter_by(id=id_).first()
     if user is not None:
         tags_str = user.tags
         tags_list: List[List[str]] = json.loads(tags_str)
         for tags in tags_list:
             if tags == args:
                 await subscribes.finish("您已经订阅了这个 Tag！")
@@ -310,7 +335,100 @@
         await list_subscribes.finish("您还没有订阅任何 Tag！")
     tags_str = user.tags
     tags_list: List[List[str]] = json.loads(tags_str)
     msg = "您订阅的 Tag 有：\n"
     for index, tags in enumerate(tags_list):
         msg += f"{index + 1}. {' '.join(tags)}\n"
     await list_subscribes.finish(msg)
+
+
+@search.handle()
+async def search_handle(arg: Message = CommandArg()):
+    if arg.extract_plain_text() == "":
+        await search.finish("请提供搜索关键词！")
+
+    tags = arg.extract_plain_text().split(" ")
+
+    if tags == []:
+        await search.finish("请提供搜索关键词！")
+
+    anime_data = await get_anime_data(tags, plugin_config.acgrip_url)
+
+    if anime_data == []:
+        await search.finish("没有找到相关番剧！")
+
+    msg = ""
+    for entry in anime_data:
+        msg += f"{entry['id']}. {entry['title']}\n"
+
+    await search.send(msg.strip())
+
+    # store the data
+    for entry in anime_data:
+        existing_entry = (
+            acgrip_session.query(ACGRIPData).filter_by(id=entry["id"]).first()
+        )
+        if existing_entry is None:
+            acgrip_session.add(ACGRIPData(**entry))
+
+    acgrip_session.commit()
+
+
+@download.handle()
+async def download_handle(
+    arg: Message = CommandArg(), target: Target = Depends(get_target)
+):
+    if arg.extract_plain_text() == "":
+        await download.finish("请提供资源 ID！")
+
+    args = arg.extract_plain_text().split(" ")
+
+    if len(args) != 1:
+        await download.finish("请提供正确的资源 ID！")
+
+    anime_entry = acgrip_session.query(ACGRIPData).filter_by(id=args[0]).first()
+
+    if anime_entry is None:
+        await download.finish("没有找到相关番剧，请使用搜索功能（/anmsc）获得资源 ID")
+
+    torrent_id = args[0]
+
+    if not torrent_id.isdigit():
+        await download.finish("请提供正确的资源 ID！")
+
+    if int(torrent_id) in video_manager.ids:
+        await download.finish(
+            f"{anime_entry.title} 已存在！\n"
+            + f"{plugin_config.anime_url}:{nonebot.get_driver().config.port}/anime/{torrent_id}"
+        )
+
+    id_ = f"{'private' if target.private else 'group'}_{target.id}"
+
+    tags = extract_tags_from_title(anime_entry.title)
+
+    torrent_data = await fetch_torrent_data(
+        f"{plugin_config.acgrip_url}/t/{torrent_id}.torrent"
+    )
+    try:
+        torrent_info = await torrent_downloader.download_torrent(
+            torrent_data, generate_folder_name(tags)
+        )
+    except Exception:
+        await download.finish("下载失败！请稍后重试。")
+
+    task_manager.add(
+        {
+            "id": id_,
+            "content": torrent_info,
+            "torrent_id": int(torrent_id),
+        }
+    )
+
+    await download.send(f"开始下载 {anime_entry.title}...")
+
+    scheduler.add_job(
+        check_video_downloaded,
+        "interval",
+        seconds=10,
+        args=(anime_entry.title, int(torrent_id), id_),
+        id=f"{anime_entry.title}_{id_}",
+    )
```

### Comparing `nonebot_plugin_anime_downloader-0.1.5/nonebot_plugin_anime_downloader/acgrip/__init__.py` & `nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/acgrip/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     for tag in tags:
         tag.replace(" ", "+")
 
     query = "+".join(tags)
     return query
 
 
-def get_anime_data(tags: List[str]) -> List[Dict[str, str]]:
+async def get_anime_data(tags: List[str], base_url: str) -> List[Dict[str, str]]:
     """Fetches anime data from ACG.RIP.
 
     Args:
       tags: A list of tags to search for.
 
     Returns:
       A list of dictionaries, where each dictionary contains information
@@ -143,15 +143,15 @@
         "title": "[桜都字幕组] ... [简繁内封]",
         "url": "/t/302390",
         "id": "302390",
         "size": "99.8 MB"
       }
     """
     query = convert_tags_to_query(tags)
-    html = make_request(f"?term={query}")
+    html = await make_request(f"?term={query}", base_url)
     html = replace_html_entities(html)
     data = extract_data(html)
     return data
 
 
 async def main() -> None:
     tag = ["北宇治字幕组", "GIRLS BAND CRY", "简体内嵌"]
@@ -161,10 +161,7 @@
     data = extract_data(html)
     print(data)
 
 
 if __name__ == "__main__":
     loop = asyncio.get_event_loop()
     loop.run_until_complete(main())
-
-
-__all__ = ["get_anime_data", "fetch_torrent_data"]
```

### Comparing `nonebot_plugin_anime_downloader-0.1.5/nonebot_plugin_anime_downloader/config.py` & `nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.5/nonebot_plugin_anime_downloader/data_source.py` & `nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.5/nonebot_plugin_anime_downloader/downloader/__init__.py` & `nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.5/nonebot_plugin_anime_downloader/downloader/models.py` & `nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/downloader/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.5/nonebot_plugin_anime_downloader/tasks.py` & `nonebot_plugin_anime_downloader-0.2.0/nonebot_plugin_anime_downloader/tasks.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_anime_downloader-0.1.5/pyproject.toml` & `nonebot_plugin_anime_downloader-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-anime-downloader"
-version = "0.1.5"
+version = "0.2.0"
 description = "✨ 基于 qBittorrent Web UI 的番剧下载 NoneBot 插件 ✨"
 authors = [
     { name = "zhaomaoniu", email = "2667292003@qq.com" },
 ]
 dependencies = [
     "nonebot2>=2.2.1",
     "aiohttp>=3.9.5",
```

### Comparing `nonebot_plugin_anime_downloader-0.1.5/PKG-INFO` & `nonebot_plugin_anime_downloader-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-anime-downloader
-Version: 0.1.5
+Version: 0.2.0
 Summary: ✨ 基于 qBittorrent Web UI 的番剧下载 NoneBot 插件 ✨
 Author-Email: zhaomaoniu <2667292003@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: nonebot2>=2.2.1
 Requires-Dist: aiohttp>=3.9.5
 Requires-Dist: qbittorrent-api>=2024.3.60
@@ -32,14 +32,16 @@
 
 ## 使用
 | 命令 | 别名 | 说明 | 示例 |
 | --- | --- | --- | --- |
 | sub | 订阅 | 通过 Tag 订阅番剧 | `sub Up to 21°C Nijiyon Animation 2 MP4` |
 | unsub | 取消订阅 | 通过 Tag 取消订阅番剧 | `unsub Up to 21°C Nijiyon Animation 2 MP4` |
 | listsub | sublist, 订阅列表 | 查看当前用户/群组的订阅列表 | `sublist` |
+| amnsc | 番剧搜索, 搜索番剧, animesearch | 通过关键词搜索番剧 | `amnsc Nijiyon Animation 2` |
+| amnd | 番剧下载, 下载番剧, animedownload | 通过 资源ID 下载番剧 | `amnd 114514` |
 
 这里的 Tag 就是用来在 ACG.RIP 搜索的关键词，番剧名、分辨率、字幕组等等，只要能在 ACG.RIP 搜索到的都可以
 
 > 记得加上你的命令头哦
 
 ## 效果
 
@@ -53,14 +55,19 @@
 1. Up to 21°C Nijiyon Animation 2 MP4
 
 (过了一段时间)
 
 **bot**: [Up to 21°C] Love Live！虹咲學園 學園偶像同好會 短篇動畫 第二季 / Nijiyon Animation 2 - 04 (ABEMA 1920x1080 AVC AAC MP4) 现在可以观看了！
 [http://example.com/anime/302322](http://example.com/anime/302322)
 
+**user**: `/amnd 302322`
+
+**bot**: [Up to 21°C] Love Live！虹咲學園 學園偶像同好會 短篇動畫 第二季 / Nijiyon Animation 2 - 04 (ABEMA 1920x1080 AVC AAC MP4) 现在可以观看了！
+[http://example.com/anime/302322](http://example.com/anime/302322)
+
 
 ## 安装方法
 <details open>
 <summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
     nb plugin install nonebot-plugin-anime-downloader
```

