# Comparing `tmp/nonebot_adapter_feishu-2.6.0.tar.gz` & `tmp/nonebot_adapter_feishu-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_feishu-2.6.0.tar", max compression
+gzip compressed data, was "nonebot_adapter_feishu-2.6.1.tar", max compression
```

## Comparing `nonebot_adapter_feishu-2.6.0.tar` & `nonebot_adapter_feishu-2.6.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1064 2024-04-26 02:38:59.055566 nonebot_adapter_feishu-2.6.0/LICENSE
--rw-r--r--   0        0        0     2459 2024-04-26 02:38:59.055566 nonebot_adapter_feishu-2.6.0/README.md
--rw-r--r--   0        0        0      863 2024-04-26 02:38:59.055566 nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/__init__.py
--rw-r--r--   0        0        0    11669 2024-04-26 02:38:59.055566 nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/adapter.py
--rw-r--r--   0        0        0    10926 2024-04-26 02:38:59.055566 nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/bot.py
--rw-r--r--   0        0        0     1360 2024-04-26 02:38:59.055566 nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/config.py
--rw-r--r--   0        0        0    12013 2024-04-26 02:38:59.055566 nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/event.py
--rw-r--r--   0        0        0     1348 2024-04-26 02:38:59.055566 nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/exception.py
--rw-r--r--   0        0        0    16543 2024-04-26 02:38:59.059566 nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/message.py
--rw-r--r--   0        0        0       69 2024-04-26 02:38:59.059566 nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/models/__init__.py
--rw-r--r--   0        0        0      700 2024-04-26 02:38:59.059566 nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/models/api.py
--rw-r--r--   0        0        0    12848 2024-04-26 02:38:59.059566 nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/models/common.py
--rw-r--r--   0        0        0      911 2024-04-26 02:38:59.059566 nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/utils.py
--rw-r--r--   0        0        0     2387 2024-04-26 02:38:59.059566 nonebot_adapter_feishu-2.6.0/pyproject.toml
--rw-r--r--   0        0        0     3551 1970-01-01 00:00:00.000000 nonebot_adapter_feishu-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-05 02:58:16.315892 nonebot_adapter_feishu-2.6.1/LICENSE
+-rw-r--r--   0        0        0     2459 2024-05-05 02:58:16.315892 nonebot_adapter_feishu-2.6.1/README.md
+-rw-r--r--   0        0        0      863 2024-05-05 02:58:16.315892 nonebot_adapter_feishu-2.6.1/nonebot/adapters/feishu/__init__.py
+-rw-r--r--   0        0        0    11727 2024-05-05 02:58:16.315892 nonebot_adapter_feishu-2.6.1/nonebot/adapters/feishu/adapter.py
+-rw-r--r--   0        0        0    11790 2024-05-05 02:58:16.315892 nonebot_adapter_feishu-2.6.1/nonebot/adapters/feishu/bot.py
+-rw-r--r--   0        0        0     1360 2024-05-05 02:58:16.315892 nonebot_adapter_feishu-2.6.1/nonebot/adapters/feishu/config.py
+-rw-r--r--   0        0        0    12013 2024-05-05 02:58:16.315892 nonebot_adapter_feishu-2.6.1/nonebot/adapters/feishu/event.py
+-rw-r--r--   0        0        0     1348 2024-05-05 02:58:16.315892 nonebot_adapter_feishu-2.6.1/nonebot/adapters/feishu/exception.py
+-rw-r--r--   0        0        0    16746 2024-05-05 02:58:16.315892 nonebot_adapter_feishu-2.6.1/nonebot/adapters/feishu/message.py
+-rw-r--r--   0        0        0       69 2024-05-05 02:58:16.315892 nonebot_adapter_feishu-2.6.1/nonebot/adapters/feishu/models/__init__.py
+-rw-r--r--   0        0        0      700 2024-05-05 02:58:16.315892 nonebot_adapter_feishu-2.6.1/nonebot/adapters/feishu/models/api.py
+-rw-r--r--   0        0        0    12848 2024-05-05 02:58:16.315892 nonebot_adapter_feishu-2.6.1/nonebot/adapters/feishu/models/common.py
+-rw-r--r--   0        0        0     1326 2024-05-05 02:58:16.315892 nonebot_adapter_feishu-2.6.1/nonebot/adapters/feishu/utils.py
+-rw-r--r--   0        0        0     2387 2024-05-05 02:58:16.319892 nonebot_adapter_feishu-2.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3551 1970-01-01 00:00:00.000000 nonebot_adapter_feishu-2.6.1/PKG-INFO
```

### Comparing `nonebot_adapter_feishu-2.6.0/LICENSE` & `nonebot_adapter_feishu-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_feishu-2.6.0/README.md` & `nonebot_adapter_feishu-2.6.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/__init__.py` & `nonebot_adapter_feishu-2.6.1/nonebot/adapters/feishu/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/adapter.py` & `nonebot_adapter_feishu-2.6.1/nonebot/adapters/feishu/adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,16 @@
                     result = json.loads(response.content)
                     return result
                 else:
                     return response.content
 
             raise NetworkError(
                 f"HTTP request received unexpected "
-                f"status code: {response.status_code}"
+                f"status code: {response.status_code}, "
+                f"response content: {response.content}"
             )
 
         except FeishuAdapterException:
             raise
 
         except Exception as e:
             raise NetworkError("HTTP request failed") from e
```

### Comparing `nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/bot.py` & `nonebot_adapter_feishu-2.6.1/nonebot/adapters/feishu/bot.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import re
+from io import BytesIO
+from pathlib import Path
 from typing_extensions import override
 from typing import TYPE_CHECKING, Any, Union, Literal, Callable, Optional
 
 from nonebot.message import handle_event
 from nonebot.compat import type_validate_python
 
 from nonebot.adapters import Bot as BaseBot
 
-from .utils import log
+from .utils import f2b, log
 from .config import BotConfig
 from .models import BotInfo, ReplyResponse
 from .message import At, Message, MessageSegment
 from .event import Event, MessageEvent, GroupMessageEvent, PrivateMessageEvent
 
 if TYPE_CHECKING:
     from .adapter import Adapter
@@ -318,14 +320,44 @@
             json={
                 "receive_id": receive_id,
                 "content": content,
                 "msg_type": msg_type,
             },
         )
 
+    async def get_file(self, file_key: str):
+        response = await self.call_api(
+            f"im/v1/files/{file_key}", method="GET", _return_response=True
+        )
+
+        return response.content
+
+    async def post_file(
+        self,
+        file_type: Literal["opus", "mp4", "pdf", "doc", "xls", "ppt", "stream"],
+        file_name: str,
+        file: Union[str, bytes, BytesIO, Path],
+        duration: Optional[int] = None,
+    ):
+        data: dict[str, Union[str, int]] = {
+            "file_type": file_type,
+            "file_name": file_name,
+        }
+
+        files = {"file": f2b(file)}
+
+        if duration:
+            data["duration"] = duration
+
+        response = await self.call_api(
+            "im/v1/files", method="POST", data=data, files=files
+        )
+
+        return response
+
     @override
     async def send(
         self,
         event: Event,
         message: Union[str, Message, MessageSegment],
         **kwargs: Any,
     ) -> Any:
```

### Comparing `nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/config.py` & `nonebot_adapter_feishu-2.6.1/nonebot/adapters/feishu/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/event.py` & `nonebot_adapter_feishu-2.6.1/nonebot/adapters/feishu/event.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/exception.py` & `nonebot_adapter_feishu-2.6.1/nonebot/adapters/feishu/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/message.py` & `nonebot_adapter_feishu-2.6.1/nonebot/adapters/feishu/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,16 +86,19 @@
     @staticmethod
     def interactive_template(
         template_id: str, template_variable: dict[str, Any]
     ) -> "InteractiveTemplate":
         return InteractiveTemplate(
             "interactive",
             {
-                "template_id": template_id,
-                "template_variable": template_variable,
+                "type": "template",
+                "data": {
+                    "template_id": template_id,
+                    "template_variable": template_variable,
+                },
             },
         )
 
     @staticmethod
     def todo(task_id: str, summary: "_PostData", due_time: str):
         return Todo(
             "todo", {"task_id": task_id, "summary": summary, "due_time": due_time}
@@ -242,19 +245,24 @@
         data: _InteractiveData
 
     @override
     def __str__(self) -> str:
         return f"[interactive:{self.data!r}]"
 
 
-class _InteractiveTemplateData(TypedDict):
+class _InteractiveTemplateDetail(TypedDict):
     template_id: str
     template_variable: dict[str, Any]
 
 
+class _InteractiveTemplateData(TypedDict):
+    type: Literal["template"]
+    data: _InteractiveTemplateDetail
+
+
 @dataclass
 class InteractiveTemplate(MessageSegment):
     if TYPE_CHECKING:
         data: _InteractiveTemplateData
 
     @override
     def __str__(self) -> str:
```

### Comparing `nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/models/api.py` & `nonebot_adapter_feishu-2.6.1/nonebot/adapters/feishu/models/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/models/common.py` & `nonebot_adapter_feishu-2.6.1/nonebot/adapters/feishu/models/common.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_feishu-2.6.0/pyproject.toml` & `nonebot_adapter_feishu-2.6.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-feishu"
-version = "2.6.0"
+version = "2.6.1"
 description = "feishu(larksuite) adapter for nonebot2"
 authors = ["StarHeartHunt <starheart233@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://feishu.adapters.nonebot.dev/"
 repository = "https://github.com/nonebot/adapter-feishu"
 documentation = "https://feishu.adapters.nonebot.dev/"
```

### Comparing `nonebot_adapter_feishu-2.6.0/PKG-INFO` & `nonebot_adapter_feishu-2.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-feishu
-Version: 2.6.0
+Version: 2.6.1
 Summary: feishu(larksuite) adapter for nonebot2
 Home-page: https://feishu.adapters.nonebot.dev/
 License: MIT
 Keywords: bot,feishu,larksuite
 Author: StarHeartHunt
 Author-email: starheart233@gmail.com
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-adapter-feishu Version: 2.6.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-adapter-feishu Version: 2.6.1 Summary:
 feishu(larksuite) adapter for nonebot2 Home-page: https://
 feishu.adapters.nonebot.dev/ License: MIT Keywords: bot,feishu,larksuite
 Author: StarHeartHunt Author-email: starheart233@gmail.com Requires-Python:
 >=3.9,<4.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
 Framework :: Robot Framework Classifier: Framework :: Robot Framework ::
 Library Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```

