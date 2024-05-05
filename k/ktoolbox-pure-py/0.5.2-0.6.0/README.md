# Comparing `tmp/ktoolbox_pure_py-0.5.2.tar.gz` & `tmp/ktoolbox_pure_py-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ktoolbox_pure_py-0.5.2.tar", max compression
+gzip compressed data, was "ktoolbox_pure_py-0.6.0.tar", max compression
```

## Comparing `ktoolbox_pure_py-0.5.2.tar` & `ktoolbox_pure_py-0.6.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1533 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/LICENSE
--rw-r--r--   0        0        0     5054 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/README.md
--rw-r--r--   0        0        0      166 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/__init__.py
--rw-r--r--   0        0        0      475 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/__main__.py
--rw-r--r--   0        0        0      949 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/_enum.py
--rw-r--r--   0        0        0      103 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/action/__init__.py
--rw-r--r--   0        0        0      192 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/action/base.py
--rw-r--r--   0        0        0     1187 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/action/fetch.py
--rw-r--r--   0        0        0     6803 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/action/job.py
--rw-r--r--   0        0        0     3233 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/action/search.py
--rw-r--r--   0        0        0     3079 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/action/utils.py
--rw-r--r--   0        0        0      172 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/api/__init__.py
--rw-r--r--   0        0        0     4163 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/api/base.py
--rw-r--r--   0        0        0       31 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/api/misc/__init__.py
--rw-r--r--   0        0        0      480 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/api/misc/get_app_version.py
--rw-r--r--   0        0        0       71 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/api/model/__init__.py
--rw-r--r--   0        0        0      405 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/api/model/announcement.py
--rw-r--r--   0        0        0      581 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/api/model/creator.py
--rw-r--r--   0        0        0      831 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/api/model/post.py
--rw-r--r--   0        0        0      116 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/api/posts/__init__.py
--rw-r--r--   0        0        0      789 2024-04-15 15:56:50.454143 ktoolbox_pure_py-0.5.2/ktoolbox/api/posts/get_announcement.py
--rw-r--r--   0        0        0      997 2024-04-15 15:56:50.454143 ktoolbox_pure_py-0.5.2/ktoolbox/api/posts/get_creator_post.py
--rw-r--r--   0        0        0      629 2024-04-15 15:56:50.454143 ktoolbox_pure_py-0.5.2/ktoolbox/api/posts/get_creators.py
--rw-r--r--   0        0        0      761 2024-04-15 15:56:50.454143 ktoolbox_pure_py-0.5.2/ktoolbox/api/posts/get_post.py
--rw-r--r--   0        0        0      836 2024-04-15 15:56:50.454143 ktoolbox_pure_py-0.5.2/ktoolbox/api/utils.py
--rw-r--r--   0        0        0    10238 2024-04-15 15:56:50.454143 ktoolbox_pure_py-0.5.2/ktoolbox/cli.py
--rw-r--r--   0        0        0     7572 2024-04-15 15:56:50.454143 ktoolbox_pure_py-0.5.2/ktoolbox/configuration.py
--rw-r--r--   0        0        0       67 2024-04-15 15:56:50.454143 ktoolbox_pure_py-0.5.2/ktoolbox/downloader/__init__.py
--rw-r--r--   0        0        0      200 2024-04-15 15:56:50.454143 ktoolbox_pure_py-0.5.2/ktoolbox/downloader/base.py
--rw-r--r--   0        0        0     9705 2024-04-15 15:56:50.454143 ktoolbox_pure_py-0.5.2/ktoolbox/downloader/downloader.py
--rw-r--r--   0        0        0     2913 2024-04-15 15:56:50.454143 ktoolbox_pure_py-0.5.2/ktoolbox/downloader/utils.py
--rw-r--r--   0        0        0       43 2024-04-15 15:56:50.454143 ktoolbox_pure_py-0.5.2/ktoolbox/job/__init__.py
--rw-r--r--   0        0        0     1656 2024-04-15 15:56:50.454143 ktoolbox_pure_py-0.5.2/ktoolbox/job/model.py
--rw-r--r--   0        0        0     6817 2024-04-15 15:56:50.454143 ktoolbox_pure_py-0.5.2/ktoolbox/job/runner.py
--rw-r--r--   0        0        0      882 2024-04-15 15:56:50.454143 ktoolbox_pure_py-0.5.2/ktoolbox/model.py
--rw-r--r--   0        0        0     3701 2024-04-15 15:56:50.454143 ktoolbox_pure_py-0.5.2/ktoolbox/utils.py
--rw-r--r--   0        0        0     1978 2024-04-15 15:56:50.454143 ktoolbox_pure_py-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     6408 1970-01-01 00:00:00.000000 ktoolbox_pure_py-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1533 2024-05-05 12:48:39.634145 ktoolbox_pure_py-0.6.0/LICENSE
+-rw-r--r--   0        0        0     5054 2024-05-05 12:48:39.634145 ktoolbox_pure_py-0.6.0/README.md
+-rw-r--r--   0        0        0      166 2024-05-05 12:48:39.634145 ktoolbox_pure_py-0.6.0/ktoolbox/__init__.py
+-rw-r--r--   0        0        0      475 2024-05-05 12:48:39.634145 ktoolbox_pure_py-0.6.0/ktoolbox/__main__.py
+-rw-r--r--   0        0        0      949 2024-05-05 12:48:39.634145 ktoolbox_pure_py-0.6.0/ktoolbox/_enum.py
+-rw-r--r--   0        0        0      103 2024-05-05 12:48:39.634145 ktoolbox_pure_py-0.6.0/ktoolbox/action/__init__.py
+-rw-r--r--   0        0        0      192 2024-05-05 12:48:39.634145 ktoolbox_pure_py-0.6.0/ktoolbox/action/base.py
+-rw-r--r--   0        0        0     1187 2024-05-05 12:48:39.634145 ktoolbox_pure_py-0.6.0/ktoolbox/action/fetch.py
+-rw-r--r--   0        0        0     7429 2024-05-05 12:48:39.634145 ktoolbox_pure_py-0.6.0/ktoolbox/action/job.py
+-rw-r--r--   0        0        0     3233 2024-05-05 12:48:39.634145 ktoolbox_pure_py-0.6.0/ktoolbox/action/search.py
+-rw-r--r--   0        0        0     3079 2024-05-05 12:48:39.634145 ktoolbox_pure_py-0.6.0/ktoolbox/action/utils.py
+-rw-r--r--   0        0        0      172 2024-05-05 12:48:39.634145 ktoolbox_pure_py-0.6.0/ktoolbox/api/__init__.py
+-rw-r--r--   0        0        0     4163 2024-05-05 12:48:39.634145 ktoolbox_pure_py-0.6.0/ktoolbox/api/base.py
+-rw-r--r--   0        0        0       31 2024-05-05 12:48:39.634145 ktoolbox_pure_py-0.6.0/ktoolbox/api/misc/__init__.py
+-rw-r--r--   0        0        0      480 2024-05-05 12:48:39.634145 ktoolbox_pure_py-0.6.0/ktoolbox/api/misc/get_app_version.py
+-rw-r--r--   0        0        0       71 2024-05-05 12:48:39.634145 ktoolbox_pure_py-0.6.0/ktoolbox/api/model/__init__.py
+-rw-r--r--   0        0        0      405 2024-05-05 12:48:39.634145 ktoolbox_pure_py-0.6.0/ktoolbox/api/model/announcement.py
+-rw-r--r--   0        0        0      581 2024-05-05 12:48:39.634145 ktoolbox_pure_py-0.6.0/ktoolbox/api/model/creator.py
+-rw-r--r--   0        0        0      831 2024-05-05 12:48:39.634145 ktoolbox_pure_py-0.6.0/ktoolbox/api/model/post.py
+-rw-r--r--   0        0        0      116 2024-05-05 12:48:39.634145 ktoolbox_pure_py-0.6.0/ktoolbox/api/posts/__init__.py
+-rw-r--r--   0        0        0      789 2024-05-05 12:48:39.638145 ktoolbox_pure_py-0.6.0/ktoolbox/api/posts/get_announcement.py
+-rw-r--r--   0        0        0      997 2024-05-05 12:48:39.638145 ktoolbox_pure_py-0.6.0/ktoolbox/api/posts/get_creator_post.py
+-rw-r--r--   0        0        0      629 2024-05-05 12:48:39.638145 ktoolbox_pure_py-0.6.0/ktoolbox/api/posts/get_creators.py
+-rw-r--r--   0        0        0      761 2024-05-05 12:48:39.638145 ktoolbox_pure_py-0.6.0/ktoolbox/api/posts/get_post.py
+-rw-r--r--   0        0        0      836 2024-05-05 12:48:39.638145 ktoolbox_pure_py-0.6.0/ktoolbox/api/utils.py
+-rw-r--r--   0        0        0    10070 2024-05-05 12:48:39.638145 ktoolbox_pure_py-0.6.0/ktoolbox/cli.py
+-rw-r--r--   0        0        0     7999 2024-05-05 12:48:39.638145 ktoolbox_pure_py-0.6.0/ktoolbox/configuration.py
+-rw-r--r--   0        0        0       67 2024-05-05 12:48:39.638145 ktoolbox_pure_py-0.6.0/ktoolbox/downloader/__init__.py
+-rw-r--r--   0        0        0      200 2024-05-05 12:48:39.638145 ktoolbox_pure_py-0.6.0/ktoolbox/downloader/base.py
+-rw-r--r--   0        0        0     9705 2024-05-05 12:48:39.638145 ktoolbox_pure_py-0.6.0/ktoolbox/downloader/downloader.py
+-rw-r--r--   0        0        0     2913 2024-05-05 12:48:39.638145 ktoolbox_pure_py-0.6.0/ktoolbox/downloader/utils.py
+-rw-r--r--   0        0        0       43 2024-05-05 12:48:39.638145 ktoolbox_pure_py-0.6.0/ktoolbox/job/__init__.py
+-rw-r--r--   0        0        0     1656 2024-05-05 12:48:39.638145 ktoolbox_pure_py-0.6.0/ktoolbox/job/model.py
+-rw-r--r--   0        0        0     6817 2024-05-05 12:48:39.638145 ktoolbox_pure_py-0.6.0/ktoolbox/job/runner.py
+-rw-r--r--   0        0        0      882 2024-05-05 12:48:39.638145 ktoolbox_pure_py-0.6.0/ktoolbox/model.py
+-rw-r--r--   0        0        0     3701 2024-05-05 12:48:39.638145 ktoolbox_pure_py-0.6.0/ktoolbox/utils.py
+-rw-r--r--   0        0        0     1978 2024-05-05 12:48:39.638145 ktoolbox_pure_py-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6408 1970-01-01 00:00:00.000000 ktoolbox_pure_py-0.6.0/PKG-INFO
```

### Comparing `ktoolbox_pure_py-0.5.2/LICENSE` & `ktoolbox_pure_py-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.2/README.md` & `ktoolbox_pure_py-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.2/ktoolbox/_enum.py` & `ktoolbox_pure_py-0.6.0/ktoolbox/_enum.py`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.2/ktoolbox/action/fetch.py` & `ktoolbox_pure_py-0.6.0/ktoolbox/action/fetch.py`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.2/ktoolbox/action/job.py` & `ktoolbox_pure_py-0.6.0/ktoolbox/action/job.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from datetime import datetime
+from fnmatch import fnmatch
 from itertools import count
 from pathlib import Path
 from typing import List, Union, Optional
 from urllib.parse import urlparse
 
 import aiofiles
 from loguru import logger
@@ -44,43 +45,65 @@
         attachments_path.mkdir(exist_ok=True)
         content_path = post_path / post_structure.content_filepath  # content
         content_path.parent.mkdir(exist_ok=True)
     else:
         attachments_path = post_path
         content_path = None
 
-    # Create jobs
+    # Filter and create jobs for ``Post.attachment``
     jobs: List[Job] = []
-    for i, attachment in enumerate(post.attachments or []):  # type: int, Attachment
+    for i, attachment in enumerate(post.attachments):  # type: int, Attachment
         if not attachment.path:
             continue
-        if is_valid_filename(attachment.name):
-            alt_filename = f"{i + 1}{Path(attachment.name).suffix}" if config.job.sequential_filename \
-                else attachment.name
-        else:
-            attachment_path_without_params = urlparse(attachment.path).path
-            alt_filename = f"{i + 1}{Path(attachment_path_without_params).suffix}" if config.job.sequential_filename \
-                else None
-        jobs.append(
-            Job(
-                path=attachments_path,
-                alt_filename=alt_filename,
-                server_path=attachment.path,
-                type=PostFileTypeEnum.Attachment
-            )
+        file_path_obj = Path(attachment.name) if is_valid_filename(attachment.name) else Path(
+            urlparse(attachment.path).path
         )
-    if post.file and post.file.path:  # file
-        jobs.append(
-            Job(
-                path=post_path,
-                alt_filename=f"{post.id}_{post.file.name}",
-                server_path=post.file.path,
-                type=PostFileTypeEnum.File
+        if (not config.job.allow_list or any(
+                map(
+                    lambda x: fnmatch(file_path_obj.name, x),
+                    config.job.allow_list
+                )
+        )) and not any(
+            map(
+                lambda x: fnmatch(file_path_obj.name, x),
+                config.job.block_list
+            )
+        ):
+            alt_filename = f"{i + 1}{file_path_obj.suffix}" if config.job.sequential_filename else file_path_obj.name
+            jobs.append(
+                Job(
+                    path=attachments_path,
+                    alt_filename=alt_filename,
+                    server_path=attachment.path,
+                    type=PostFileTypeEnum.Attachment
+                )
+            )
+
+    # Filter and create jobs for ``Post.file``
+    if post.file and post.file.path:
+        post_file_name = post.file.name or Path(post.file.path).name
+        if (not config.job.allow_list or any(
+                map(
+                    lambda x: fnmatch(post_file_name, x),
+                    config.job.allow_list
+                )
+        )) and not any(
+            map(
+                lambda x: fnmatch(post_file_name, x),
+                config.job.block_list
+            )
+        ):
+            jobs.append(
+                Job(
+                    path=post_path,
+                    alt_filename=f"{post.id}_{post_file_name}",
+                    server_path=post.file.path,
+                    type=PostFileTypeEnum.File
+                )
             )
-        )
 
     # Write content file
     if content_path and post.content:
         async with aiofiles.open(content_path, "w", encoding=config.downloader.encoding) as f:
             await f.write(post.content)
     if dump_post_data:
         async with aiofiles.open(str(post_path / DataStorageNameEnum.PostData.value), "w", encoding="utf-8") as f:
@@ -95,31 +118,31 @@
         service: str,
         creator_id: str,
         path: Path,
         *,
         all_pages: bool = False,
         offset: int = 0,
         length: Optional[int] = 50,
-        save_creator_indices: bool = True,
+        save_creator_indices: bool = False,
         mix_posts: bool = None,
         start_time: Optional[datetime],
         end_time: Optional[datetime]
 ) -> ActionRet[List[Job]]:
     """
     Create a list of download job from a creator
 
     :param service: The service where the post is located
     :param creator_id: The ID of the creator
     :param path: The path for downloading posts, which needs to be sanitized
     :param all_pages: Fetch all posts, ``offset`` and ``length`` will be ignored if enabled
     :param offset: Result offset (or start offset)
     :param length: The number of posts to fetch
-    :param save_creator_indices: Record ``CreatorIndices`` data for update posts from current creator directory
+    :param save_creator_indices: Record ``CreatorIndices`` data.
     :param mix_posts: Save all files from different posts at same path, \
-     ``update_from``, ``save_creator_indices`` will be ignored if enabled
+     ``save_creator_indices`` will be ignored if enabled
     :param start_time: Start time of the time range
     :param end_time: End time of the time range
     """
     mix_posts = config.job.mix_posts if mix_posts is None else mix_posts
 
     # Get posts
     logger.info(f"Start fetching posts from creator {creator_id}")
@@ -148,15 +171,15 @@
     # Filter posts by publish time
     if start_time or end_time:
         post_list = list(filter_posts_by_date(post_list, start_time, end_time))
     logger.info(f"Get {len(post_list)} posts, start creating jobs")
 
     # Filter posts and generate ``CreatorIndices``
     if not mix_posts:
-        if save_creator_indices:  # It's unnecessary to create indices again when ``update_from`` was provided
+        if save_creator_indices:
             indices = CreatorIndices(
                 creator_id=creator_id,
                 service=service,
                 posts={post.id: post for post in post_list},
                 posts_path={post.id: path / sanitize_filename(post.title) for post in post_list}
             )
             async with aiofiles.open(
```

### Comparing `ktoolbox_pure_py-0.5.2/ktoolbox/action/search.py` & `ktoolbox_pure_py-0.6.0/ktoolbox/action/search.py`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.2/ktoolbox/action/utils.py` & `ktoolbox_pure_py-0.6.0/ktoolbox/action/utils.py`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.2/ktoolbox/api/base.py` & `ktoolbox_pure_py-0.6.0/ktoolbox/api/base.py`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.2/ktoolbox/api/model/creator.py` & `ktoolbox_pure_py-0.6.0/ktoolbox/api/model/creator.py`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.2/ktoolbox/api/model/post.py` & `ktoolbox_pure_py-0.6.0/ktoolbox/api/model/post.py`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.2/ktoolbox/api/posts/get_announcement.py` & `ktoolbox_pure_py-0.6.0/ktoolbox/api/posts/get_announcement.py`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.2/ktoolbox/api/posts/get_creator_post.py` & `ktoolbox_pure_py-0.6.0/ktoolbox/api/posts/get_creator_post.py`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.2/ktoolbox/api/posts/get_creators.py` & `ktoolbox_pure_py-0.6.0/ktoolbox/api/posts/get_creators.py`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.2/ktoolbox/api/posts/get_post.py` & `ktoolbox_pure_py-0.6.0/ktoolbox/api/posts/get_post.py`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.2/ktoolbox/api/utils.py` & `ktoolbox_pure_py-0.6.0/ktoolbox/api/utils.py`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.2/ktoolbox/cli.py` & `ktoolbox_pure_py-0.6.0/ktoolbox/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -213,37 +213,36 @@
     @staticmethod
     async def sync_creator(
             url: str = None,
             service: str = None,
             creator_id: str = None,
             path: Union[Path, str] = Path("."),
             *,
-            save_creator_indices: bool = True,
+            save_creator_indices: bool = False,
             mix_posts: bool = None,
             start_time: str = None,
             end_time: str = None,
             offset: int = 0,
             length: int = None
     ):
         """
         Sync posts from a creator
 
         You can update the directory anytime after download finished, \
         such as to update after creator published new posts.
 
-        * If ``update_from`` was provided, the file should be located **inside the creator directory**.
         * ``start_time`` & ``end_time`` example: ``2023-12-7``, ``2023-12-07``
 
         :param url: The post URL
         :param service: The service where the post is located
         :param creator_id: The ID of the creator
         :param path: Download path, default is current directory
-        :param save_creator_indices: Record ``CreatorIndices`` data for update posts from current creator directory
+        :param save_creator_indices: Record ``CreatorIndices`` data
         :param mix_posts: Save all_pages files from different posts at same path, \
-            ``update_from``, ``save_creator_indices`` will be ignored if enabled
+            ``save_creator_indices`` will be ignored if enabled
         :param start_time: Start time of the published time range for posts downloading. \
             Set to ``0`` if ``None`` was given. \
             Time format: ``%Y-%m-%d``
         :param end_time: End time of the published time range for posts downloading. \
             Set to latest time (infinity) if ``None`` was given. \
             Time format: ``%Y-%m-%d``
         :param offset: Result offset (or start offset)
```

### Comparing `ktoolbox_pure_py-0.5.2/ktoolbox/configuration.py` & `ktoolbox_pure_py-0.6.0/ktoolbox/configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import datetime
+import json
 import logging
 import os
 import tempfile
 import warnings
 from pathlib import Path
-from typing import Literal, Union, Optional, Any
+from typing import Literal, Union, Optional, Any, Set
 
 from loguru import logger
 from pydantic import BaseModel, BaseSettings, validator
 
 __all__ = [
     "config",
     "APIConfiguration",
@@ -100,15 +101,15 @@
     Post path structure model
 
     - Default:
     ```
     ..
     ├─ content.txt
     ├─ <Post file>
-    ├─ <Post data (post.ktoolbox.json)>
+    ├─ <Post data (post.json)>
     └─ attachments
        ├─ 1.png
        └─ 2.png
     ```
 
     :ivar attachments: Sub path of attachment directory
     :ivar content_filepath: Sub path of post content HTML file
@@ -138,34 +139,42 @@
     :ivar post_dirname_format: Customize the post directory name format, you can use some of the \
     [properties](/configuration/reference/#ktoolbox.configuration.JobConfiguration) in ``Post``. \
     e.g. ``[{published}]{id}`` > ``[2024-1-1]123123``, ``{user}_{published}_{title}`` > ``234234_2024-1-1_HelloWorld``
     :ivar post_structure: Post path structure
     :ivar mix_posts: Save all files from different posts at same path in creator directory. \
     It would not create any post directory, and ``CreatorIndices`` would not been recorded.
     :ivar sequential_filename: Rename attachments in numerical order, e.g. ``1.png``, ``2.png``, ...
+    :ivar allow_list: Download files which match these patterns (Unix shell-style), e.g. ``["*.png"]``
+    :ivar block_list: Not to download files which match these patterns (Unix shell-style), e.g. ``["*.psd","*.zip"]``
     """
     count: int = 4
     post_id_as_path: bool = False
     post_dirname_format: str = "{title}"
     post_structure: PostStructureConfiguration = PostStructureConfiguration()
     mix_posts: bool = False
     sequential_filename: bool = False
+    allow_list: Set[str] = set()
+    block_list: Set[str] = set()
 
     # job_list_filepath: Optional[Path] = None
     # """Filepath for job list data saving, ``None`` for disable job list saving"""
 
     @validator("post_id_as_path")
     def post_id_as_path_validator(cls, v):
         if v != cls.__fields__["post_id_as_path"].default:
             warnings.warn(
                 "`JobConfiguration.post_id_as_path` is deprecated and is scheduled for removal in further version. "
                 "Use `JobConfiguration.post_dirname_format` instead",
                 FutureWarning
             )
 
+    @validator("allow_list", "block_list", pre=True)
+    def allow_block_list_validator(cls, v):
+        return set(json.loads(v))
+
 
 class LoggerConfiguration(BaseModel):
     """
     Logger configuration
 
     :ivar path: Path to save logs, ``None`` for disable log file output
     :ivar level: Log filter level
```

### Comparing `ktoolbox_pure_py-0.5.2/ktoolbox/downloader/downloader.py` & `ktoolbox_pure_py-0.6.0/ktoolbox/downloader/downloader.py`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.2/ktoolbox/downloader/utils.py` & `ktoolbox_pure_py-0.6.0/ktoolbox/downloader/utils.py`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.2/ktoolbox/job/model.py` & `ktoolbox_pure_py-0.6.0/ktoolbox/job/model.py`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.2/ktoolbox/job/runner.py` & `ktoolbox_pure_py-0.6.0/ktoolbox/job/runner.py`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.2/ktoolbox/model.py` & `ktoolbox_pure_py-0.6.0/ktoolbox/model.py`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.2/ktoolbox/utils.py` & `ktoolbox_pure_py-0.6.0/ktoolbox/utils.py`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.2/pyproject.toml` & `ktoolbox_pure_py-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ktoolbox-pure-py"
-version = "0.5.2"
+version = "0.6.0"
 description = "A useful CLI tool for downloading posts in Kemono.party / .su (Pure Python version)"
 authors = ["Ljzd-PRO <ljzd@office.ljzd-pro.asia>"]
 readme = "README.md"
 homepage = "https://ktoolbox.readthedocs.io/"
 repository = "https://github.com/Ljzd-PRO/KToolBox"
 documentation = "https://ktoolbox.readthedocs.io/"
 
@@ -36,15 +36,15 @@
 aiofiles = "^23.2.1"
 pathvalidate = "^3.2.0"
 
 [tool.poetry.group.uvloop.dependencies]
 uvloop = "^0.19.0"
 
 [tool.poetry.group.pyinstaller.dependencies]
-pyinstaller = "==6.5.0"
+pyinstaller = "==6.6.0"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.5.3"
 mkdocs-static-i18n = "^1.2.0"
 mkdocs-material = "^9.4.14"
 mkdocstrings = {version="^0.24.0", extras=["python"]}
 mike = "^2.0.0"
```

### Comparing `ktoolbox_pure_py-0.5.2/PKG-INFO` & `ktoolbox_pure_py-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ktoolbox-pure-py
-Version: 0.5.2
+Version: 0.6.0
 Summary: A useful CLI tool for downloading posts in Kemono.party / .su (Pure Python version)
 Home-page: https://ktoolbox.readthedocs.io/
 Keywords: kemono,kemono.party,cli-app,downloader,os-independent
 Author: Ljzd-PRO
 Author-email: ljzd@office.ljzd-pro.asia
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ktoolbox-pure-py Version: 0.5.2 Summary: A useful
+Metadata-Version: 2.1 Name: ktoolbox-pure-py Version: 0.6.0 Summary: A useful
 CLI tool for downloading posts in Kemono.party / .su (Pure Python version)
 Home-page: https://ktoolbox.readthedocs.io/ Keywords: kemono,kemono.party,cli-
 app,downloader,os-independent Author: Ljzd-PRO Author-email: ljzd@office.ljzd-
 pro.asia Requires-Python: >=3.8,<3.12 Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

