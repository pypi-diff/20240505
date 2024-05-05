# Comparing `tmp/revkimi-0.0.1.tar.gz` & `tmp/revkimi-0.0.2.tar.gz`

## Comparing `revkimi-0.0.1.tar` & `revkimi-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 revkimi-0.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 revkimi-0.0.1/revKimi/__init__.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 revkimi-0.0.1/revKimi/config.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 revkimi-0.0.1/revKimi/exceptions.py
--rw-r--r--   0        0        0     5209 2020-02-02 00:00:00.000000 revkimi-0.0.1/revKimi/main.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 revkimi-0.0.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 revkimi-0.0.1/LICENSE
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 revkimi-0.0.1/README.md
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 revkimi-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 revkimi-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0   389069 2020-02-02 00:00:00.000000 revkimi-0.0.2/.github/resources/steps.png
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 revkimi-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 revkimi-0.0.2/revKimi/__init__.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 revkimi-0.0.2/revKimi/config.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 revkimi-0.0.2/revKimi/exceptions.py
+-rw-r--r--   0        0        0     6390 2020-02-02 00:00:00.000000 revkimi-0.0.2/revKimi/main.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 revkimi-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 revkimi-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 revkimi-0.0.2/README.md
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 revkimi-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 revkimi-0.0.2/PKG-INFO
```

### Comparing `revkimi-0.0.1/revKimi/config.py` & `revkimi-0.0.2/revKimi/config.py`

 * *Files identical despite different names*

### Comparing `revkimi-0.0.1/revKimi/main.py` & `revkimi-0.0.2/revKimi/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -33,66 +33,94 @@
         resp = requests.get(
             url=self.api_base + "/auth/token/refresh",
             headers=self.__get_header("refresh_token")
         ).json()
         self.config["access_token"] = resp["access_token"]
         self.config["refresh_token"] = resp["refresh_token"]
 
-    def __check_response(self, response: str):
-        try:
-            response_dict = json.loads(response)
-            if response_dict.get("error_type") == "auth.token.invalid":
-                self.__refresh_token()
-        except Exception as e:
-            return
-
     def __request(
             self,
             method: str,
             url: str,
-            json: dict,
             stream: bool = False,
             **kwargs
     ) -> requests.Response:
         resp = requests.request(
             method=method,
             url=url,
-            json=json,
             stream=stream,
             headers=self.__get_header("access_token"),
             **kwargs
         )
         stat_code = resp.status_code
-        if stat_code != 401:
+        if stat_code == 200:
             return resp
         resp_json = resp.json()
         if resp_json.get("error_type") == "auth.token.invalid":
+            # token过期
             self.__refresh_token()
             return requests.request(
                 method=method,
                 url=url,
-                json=json,
                 stream=stream,
                 headers=self.__get_header("access_token"),
                 **kwargs
             )
+        else:
+            raise UnexpectedResponse(str(resp_json))
 
-    def create_conversation(self, name: str) -> dict:
+    def create_conversation(self, name: str = "未命名会话") -> dict:
         """创建会话"""
         resp = self.__request(
-            method="GET",
+            method="POST",
             url=self.api_base + "/chat",
             json={
                 "name": f"{name}",
                 "is_example": False,
                 "born_from": ""
             }
         ).json()
         return resp
 
+    def delete_conversation(self, conversation_id: str) -> None:
+        """删除会话"""
+        self.__request(
+            method="DELETE",
+            url=self.api_base + f"/chat/{conversation_id}"
+        )
+
+    def get_conversations(self, size: int = 30) -> dict:
+        """获取会话列表
+        :param size: 最多获取条数（默认30）
+        """
+        resp = self.__request(
+            method="POST",
+            url=self.api_base + "/chat/list",
+            json={
+                "kimiplus_id": "",
+                "offset": 0,
+                "size": size
+            }
+        ).json()
+        return resp
+
+    def get_history(self, conversation_id: str, last: int = 50):
+        """获取会话历史
+        :param conversation_id: 会话ID
+        :param last: 历史条数（默认50）
+        """
+        resp = self.__request(
+            method="POST",
+            url=self.api_base + f"/chat/{conversation_id}/segment/scroll",
+            json={
+                "last": last
+            }
+        ).json()
+        return resp
+
     def __stream_ask(
             self,
             prompt: str,
             conversation_id: Optional[str],
             timeout: int = 10,
             use_search: bool = False
     ) -> Generator[dict, None, None]:
@@ -101,15 +129,15 @@
         :param prompt: 提问内容
         :param conversation_id: 会话id（若不填则会新建）
         :param timeout: 超时时间（默认10秒）
         :param use_search: 是否使用搜索
 
         """
         if not conversation_id:
-            conversation_id = self.create_conversation("未命名")["id"]
+            conversation_id = self.create_conversation()["id"]
         resp = self.__request(
             method="POST",
             url=self.api_base + f"/chat/{conversation_id}/completion/stream",
             timeout=timeout,
             stream=True,
             json={
                 "kimiplus_id": "kimi",
@@ -117,22 +145,31 @@
                     "role": "user",
                     "content": prompt
                 }],
                 "refs": [],
                 "use_search": use_search
             }
         )
+        reply_text = ""
         for chunk in resp.iter_lines():
             try:
                 if chunk:
+                    # 非空chunk
                     chunk = chunk.decode("utf-8")
                     if not chunk.endswith("}"):
+                        # 不完整
                         continue
                     chunk_json = json.loads(chunk[6:])
-                    yield chunk_json
+                    if chunk_json.get("event") == "cmpl":
+                        reply_text += chunk_json.get("text")
+                        result = {
+                            "conversation_id": conversation_id,
+                            "text": reply_text
+                        }
+                        yield result
             except Exception as e:
                 pass
 
     def ask(
             self,
             prompt: str,
             conversation_id: Optional[str],
@@ -146,22 +183,19 @@
         :param conversation_id: 会话id（若不填则会新建）
         :param timeout: 超时时间（默认10秒）
         :param use_search: 是否使用搜索
         :param stream: 是否为流式
 
         """
         resp_generator = self.__stream_ask(
-            prompt,
-            conversation_id,
-            timeout,
-            use_search
-        )
+                            prompt,
+                            conversation_id,
+                            timeout,
+                            use_search
+                        )
         if stream:
             return resp_generator
         else:
-            content = ""
+            result = None
             for chunk in resp_generator:
-                if chunk.get("event") == "cmpl":
-                    content += chunk.get("text")
-            return {
-                "text": content
-            }
+                result = chunk
+            return result
```

### Comparing `revkimi-0.0.1/.gitignore` & `revkimi-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `revkimi-0.0.1/LICENSE` & `revkimi-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `revkimi-0.0.1/pyproject.toml` & `revkimi-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "revKimi"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     {name = "old-dream321", email = "hzz123123@outlook.com"}
 ]
 description = "kimi逆向api"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.9"
```

