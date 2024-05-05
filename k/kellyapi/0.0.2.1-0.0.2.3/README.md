# Comparing `tmp/kellyapi-0.0.2.1.tar.gz` & `tmp/kellyapi-0.0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kellyapi-0.0.2.1.tar", last modified: Mon Apr 29 15:58:15 2024, max compression
+gzip compressed data, was "kellyapi-0.0.2.3.tar", last modified: Sun May  5 16:39:30 2024, max compression
```

## Comparing `kellyapi-0.0.2.1.tar` & `kellyapi-0.0.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:58:15.035273 kellyapi-0.0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-29 15:58:11.000000 kellyapi-0.0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-29 15:58:15.035273 kellyapi-0.0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-29 15:58:11.000000 kellyapi-0.0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:58:15.035273 kellyapi-0.0.2.1/kellyapi/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-29 15:58:11.000000 kellyapi-0.0.2.1/kellyapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-04-29 15:58:11.000000 kellyapi-0.0.2.1/kellyapi/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-29 15:58:11.000000 kellyapi-0.0.2.1/kellyapi/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:58:15.035273 kellyapi-0.0.2.1/kellyapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-29 15:58:15.000000 kellyapi-0.0.2.1/kellyapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-29 15:58:15.000000 kellyapi-0.0.2.1/kellyapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:58:15.000000 kellyapi-0.0.2.1/kellyapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-29 15:58:15.000000 kellyapi-0.0.2.1/kellyapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-29 15:58:15.000000 kellyapi-0.0.2.1/kellyapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 15:58:15.035273 kellyapi-0.0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-29 15:58:11.000000 kellyapi-0.0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:39:30.384714 kellyapi-0.0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-05 16:39:26.000000 kellyapi-0.0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-05-05 16:39:30.384714 kellyapi-0.0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-05 16:39:26.000000 kellyapi-0.0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:39:30.384714 kellyapi-0.0.2.3/kellyapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-05 16:39:26.000000 kellyapi-0.0.2.3/kellyapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-05-05 16:39:26.000000 kellyapi-0.0.2.3/kellyapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-05 16:39:26.000000 kellyapi-0.0.2.3/kellyapi/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:39:30.384714 kellyapi-0.0.2.3/kellyapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-05-05 16:39:30.000000 kellyapi-0.0.2.3/kellyapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-05 16:39:30.000000 kellyapi-0.0.2.3/kellyapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 16:39:30.000000 kellyapi-0.0.2.3/kellyapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-05 16:39:30.000000 kellyapi-0.0.2.3/kellyapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-05 16:39:30.000000 kellyapi-0.0.2.3/kellyapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 16:39:30.384714 kellyapi-0.0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-05 16:39:26.000000 kellyapi-0.0.2.3/setup.py
```

### Comparing `kellyapi-0.0.2.1/LICENSE` & `kellyapi-0.0.2.3/LICENSE`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Damantha Jasinghe
+Copyright (c) 2024 KellyAPI
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `kellyapi-0.0.2.1/PKG-INFO` & `kellyapi-0.0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kellyapi
-Version: 0.0.2.1
+Version: 0.0.2.3
 Summary: A Project Made To Centralize Various APIs 📖 No Authorization Needed :)
 Home-page: https://github.com/NotReallyPrince/Prince-Api
 Author: NotReallyPrince
 Author-email: princebots3011@gmail.com
 License: MIT
 Project-URL: Tracker, https://github.com/NotReallyPrince/Kelly-API/issues
 Project-URL: Community, https://t.me/PrincexUpdates
```

### Comparing `kellyapi-0.0.2.1/README.md` & `kellyapi-0.0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `kellyapi-0.0.2.1/kellyapi/api.py` & `kellyapi-0.0.2.3/kellyapi/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
+import base64
 from io import BytesIO
 from typing import List, Union
 
 import aiohttp
-import base64
 from aiohttp.client_exceptions import ClientConnectorError, ContentTypeError
 from dotmap import DotMap
 
 from .errors import *
 
 
 class KellyAPI:
@@ -29,15 +29,15 @@
 
     async def _fetch(self, route, timeout=60, **params):
         try:
             async with self.session() as client:
                 resp = await client.get(
                     self.api + route,
                     params=params,
-                    headers={"Kelly-API-KEY": self.api_key},
+                    headers={"Authorization": f"Bearer {self.api_key}"},
                     timeout=timeout,
                 )
                 if resp.status in (401, 403):
                     raise InvalidApiKey(
                         "Invalid API key, Get an api key from @KellyAIBot"
                     )
                 if resp.status == 502:
@@ -53,15 +53,15 @@
 
     async def _post_json(self, route, data=None, timeout=60):
         try:
             async with self.session() as client:
                 resp = await client.post(
                     self.api + route,
                     json=data,
-                    headers={"Kelly-API-KEY": self.api_key},
+                    headers={"Kelly-API-KEY": f"Bearer {self.api_key}"},
                     timeout=timeout,
                 )
                 if resp.status in (401, 403):
                     raise InvalidApiKey(
                         "Invalid API key, Get an api key from @KellyAIBot"
                     )
                 if resp.status == 502:
@@ -70,76 +70,116 @@
         except asyncio.TimeoutError:
             raise TimeoutError
         except ContentTypeError:
             raise InvalidContent
         except ClientConnectorError:
             raise ConnectionError
         return self._parse_result(response)
+    
 
     async def sd_models(self):
-        content = await self._fetch("sd-models")
+        content = await self._fetch("sd/models")
         return content
 
     async def sdxl_models(self):
-        content = await self._fetch("sdxl-models")
+        content = await self._fetch("sdxl/models")
         return content
 
     async def generate(
         self,
         prompt: str,
         negative_prompt: str = "canvas frame, cartoon, 3d, ((disfigured)), ((bad art)), ((deformed)),((extra limbs)),((close up)),((b&w)), weird colors, blurry, (((duplicate))), ((morbid)), ((mutilated)), [out of frame], extra fingers, mutated hands, ((poorly drawn hands)), ((poorly drawn face)), (((mutation))), (((deformed))), ((ugly)), blurry, ((bad anatomy)), (((bad proportions))), ((extra limbs)), cloned face, (((disfigured))), out of frame, ugly, extra limbs, (bad anatomy), gross proportions, (malformed limbs), ((missing arms)), ((missing legs)), (((extra arms))), (((extra legs))), mutated hands, (fused fingers), (too many fingers), (((long neck))), Photoshop, video game, ugly, tiling, poorly drawn hands, poorly drawn feet, poorly drawn face, out of frame, mutation, mutated, extra limbs, extra legs, extra arms, disfigured, deformed, cross-eye, body out of frame, blurry, bad art, bad anatomy, nsfw",
         model: str = "PhotoPerfect",
+        width: int = 1024,
+        height: int = 1024,
+    ):
+        kwargs = dict(
+            prompt=prompt,
+            negative_prompt=negative_prompt,
+            model=model,
+            width=width,
+            height=height,
+            responseType="base64data"
+        )
+        content = await self._post_json("image/generate", data=kwargs)
+        image_data = base64.b64decode(content.image)
+        return image_data
+
+    async def img2img(
+        self,
+        prompt: str,
+        image_data: str,
+        negative_prompt: str = "canvas frame, cartoon, 3d, ((disfigured)), ((bad art)), ((deformed)),((extra limbs)),((close up)),((b&w)), weird colors, blurry, (((duplicate))), ((morbid)), ((mutilated)), [out of frame], extra fingers, mutated hands, ((poorly drawn hands)), ((poorly drawn face)), (((mutation))), (((deformed))), ((ugly)), blurry, ((bad anatomy)), (((bad proportions))), ((extra limbs)), cloned face, (((disfigured))), out of frame, ugly, extra limbs, (bad anatomy), gross proportions, (malformed limbs), ((missing arms)), ((missing legs)), (((extra arms))), (((extra legs))), mutated hands, (fused fingers), (too many fingers), (((long neck))), Photoshop, video game, ugly, tiling, poorly drawn hands, poorly drawn feet, poorly drawn face, out of frame, mutation, mutated, extra limbs, extra legs, extra arms, disfigured, deformed, cross-eye, body out of frame, blurry, bad art, bad anatomy, nsfw",
         width: str = 1024,
         height: str = 1024,
     ):
         kwargs = dict(
             prompt=prompt,
             negative_prompt=negative_prompt,
-            model=model,
+            image_data=image_data,
             width=width,
             height=height,
+            responseType="base64data"
         )
-        content = await self._post_json("generate", data=kwargs)
-        image_data =  base64.b64decode(content.image)
+        content = await self._post_json("image/edit", data=kwargs)
+        image_data = base64.b64decode(content.image)
         return image_data
 
+    async def img2text(
+        self,
+        prompt: str,
+        image_data: str,
+    ):
+        kwargs = dict(
+            prompt=prompt,
+            image_data=image_data,
+        )
+        content = await self._post_json("image/description", data=kwargs)
+        return content.content
+
     async def llm_models(self):
-        content = await self._fetch("llm-models")
+        content = await self._fetch("chat/models")
         return content
 
     async def llm(self, prompt: str, model: str = "chatgpt", character: str = "KelyAI"):
-        kwargs = dict(prompt=prompt, model=model, character=character)
-        content = await self._post_json("llm", data=kwargs)
+        kwargs = dict(prompt=prompt, character=character)
+        content = await self._post_json(f"chat/{model}", data=kwargs)
         return content.message
 
     async def upscale(self, image_data: str):
-        kwargs = dict(image_data=image)
-        content = await self._post_json("upscale", data=kwargs)
-        image_data =  base64.b64decode(content.image)
+        kwargs = dict(image_data=image_data, responseType="base64data")
+        content = await self._post_json("image/upscale", data=kwargs)
+        image_data = base64.b64decode(content.image)
         return image_data
 
-    async def rmbg(self, image_data: str):
-        kwargs = dict(image_data=image)
-        content = await self._post_json("rmbg", data=kwargs)
-        image_data =  base64.b64decode(content.image)
+    async def removebg(self, image_data: str):
+        kwargs = dict(image_data=image_data, responseType="base64data")
+        content = await self._post_json("image/removebg", data=kwargs)
+        image_data = base64.b64decode(content.image)
         return image_data
 
     async def voice_models(self):
-        content = await self._fetch("voice-models")
+        content = await self._fetch("voice/models")
         return content
 
     async def text2voice(self, text: str, model: str = "en-US_LisaExpressive"):
-        kwargs = dict(text=text, model=model)
-        content = await self._post_json("text2voice", data=kwargs)
-        image_data =  base64.b64decode(content.voice)
+        kwargs = dict(text=text, model=model, responseType="base64data")
+        content = await self._post_json("voice/generation", data=kwargs)
+        image_data = base64.b64decode(content.voice)
         return image_data
 
     async def voice2text(self, audio: str):
         kwargs = dict(audio=audio)
-        content = await self._post_json("voice2text", data=kwargs)
+        content = await self._post_json("voice/transcribe", data=kwargs)
         return content.result
 
     async def text2write(self, text: str):
-        kwargs = dict(text=text)
-        content = await self._post_json("text2write", data=kwargs)
-        image_data =  base64.b64decode(content.image)
+        kwargs = dict(code=text, responseType="base64data")
+        content = await self._post_json("write/notes", data=kwargs)
+        image_data = base64.b64decode(content.image)
         return image_data
+
+    async def code2image(self, text: str):
+        kwargs = dict(code=text, responseType="base64data")
+        content = await self._post_json("write/code", data=kwargs)
+        image_data = base64.b64decode(content.image)
+        return image_data
```

### Comparing `kellyapi-0.0.2.1/kellyapi/errors.py` & `kellyapi-0.0.2.3/kellyapi/errors.py`

 * *Files identical despite different names*

### Comparing `kellyapi-0.0.2.1/kellyapi.egg-info/PKG-INFO` & `kellyapi-0.0.2.3/kellyapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kellyapi
-Version: 0.0.2.1
+Version: 0.0.2.3
 Summary: A Project Made To Centralize Various APIs 📖 No Authorization Needed :)
 Home-page: https://github.com/NotReallyPrince/Prince-Api
 Author: NotReallyPrince
 Author-email: princebots3011@gmail.com
 License: MIT
 Project-URL: Tracker, https://github.com/NotReallyPrince/Kelly-API/issues
 Project-URL: Community, https://t.me/PrincexUpdates
```

### Comparing `kellyapi-0.0.2.1/setup.py` & `kellyapi-0.0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", encoding="utf8") as readme:
     long_description = readme.read()
 
 setuptools.setup(
     name="kellyapi",
     packages=setuptools.find_packages(),
-    version="0.0.2.1",
+    version="0.0.2.3",
     license="MIT",
     description="A Project Made To Centralize Various APIs 📖 No Authorization Needed :)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="NotReallyPrince",
     author_email="princebots3011@gmail.com",
     url="https://github.com/NotReallyPrince/Prince-Api",
```

