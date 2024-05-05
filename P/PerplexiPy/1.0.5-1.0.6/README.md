# Comparing `tmp/PerplexiPy-1.0.5-py3-none-any.whl.zip` & `tmp/PerplexiPy-1.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 12240 bytes, number of entries: 10
--rw-r--r--  2.0 unx     9253 b- defN 24-Apr-22 04:33 perplexipy/__init__.py
--rw-r--r--  2.0 unx    13193 b- defN 24-May-02 18:08 perplexipy/codex.py
+Zip file size: 12541 bytes, number of entries: 10
+-rw-r--r--  2.0 unx     9853 b- defN 24-May-05 02:03 perplexipy/__init__.py
+-rw-r--r--  2.0 unx    13411 b- defN 24-May-05 02:08 perplexipy/codex.py
 -rw-r--r--  2.0 unx      283 b- defN 24-Mar-01 20:13 perplexipy/errors.py
 -rw-r--r--  2.0 unx      684 b- defN 24-Apr-13 17:06 perplexipy/responses.py
--rw-r--r--  2.0 unx     1514 b- defN 24-May-02 18:12 PerplexiPy-1.0.5.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     6968 b- defN 24-May-02 18:12 PerplexiPy-1.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-02 18:12 PerplexiPy-1.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 24-May-02 18:12 PerplexiPy-1.0.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 24-May-02 18:12 PerplexiPy-1.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      814 b- defN 24-May-02 18:12 PerplexiPy-1.0.5.dist-info/RECORD
-10 files, 32861 bytes uncompressed, 10848 bytes compressed:  67.0%
+-rw-r--r--  2.0 unx     1514 b- defN 24-May-05 02:11 PerplexiPy-1.0.6.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     6968 b- defN 24-May-05 02:11 PerplexiPy-1.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-05 02:11 PerplexiPy-1.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 24-May-05 02:11 PerplexiPy-1.0.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 24-May-05 02:11 PerplexiPy-1.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      814 b- defN 24-May-05 02:11 PerplexiPy-1.0.6.dist-info/RECORD
+10 files, 33679 bytes uncompressed, 11149 bytes compressed:  66.9%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: perplexipy/errors.py
 Comment: 
 
 Filename: perplexipy/responses.py
 Comment: 
 
-Filename: PerplexiPy-1.0.5.dist-info/LICENSE.txt
+Filename: PerplexiPy-1.0.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: PerplexiPy-1.0.5.dist-info/METADATA
+Filename: PerplexiPy-1.0.6.dist-info/METADATA
 Comment: 
 
-Filename: PerplexiPy-1.0.5.dist-info/WHEEL
+Filename: PerplexiPy-1.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: PerplexiPy-1.0.5.dist-info/entry_points.txt
+Filename: PerplexiPy-1.0.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: PerplexiPy-1.0.5.dist-info/top_level.txt
+Filename: PerplexiPy-1.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: PerplexiPy-1.0.5.dist-info/RECORD
+Filename: PerplexiPy-1.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## perplexipy/__init__.py

```diff
@@ -27,27 +27,27 @@
 from perplexipy.responses import Responses
 
 load_dotenv()
 
 import os
 
 
-
+_CLAUDE_MODEL = 'claude-3-haiku'
 """
 `PERPLEXITY_API_KEY` is set to the environment variable of the same name if
 present, otherwise it's set to the empty string `''`.
 """
 PERPLEXITY_API_KEY = os.environ.get('PERPLEXITY_API_KEY', default = '')
 PERPLEXITY_API_PREFIX = 'pplx-'
 PERPLEXITY_API_URL = 'https://api.perplexity.ai'
 """
 The default model is **mistral-7b-instruct** because of it's efficiency and
 performance qualities.  Ref:  https://arxiv.org/abs/2310.06825
 """
-PERPLEXITY_DEFAULT_MODEL = 'mistral-7b-instruct'
+PERPLEXITY_DEFAULT_MODEL = 'llama-3-sonar-small-32k-chat'
 PERPLEXITY_DEFAULT_ROLE = 'user'
 PERPLEXITY_TIMEOUT = 30.0 # seconds
 PERPLEXITY_VALID_ROLES = { 'assistant', 'system', 'user', } # future proofing.
 
 
 """
 Immutable dictionary-like object of a model's capabilities.  Use `_asDict()` if
@@ -57,26 +57,30 @@
 
 
 class PerplexityClient:
     """
     PerplexityClient objects encapsulate all the API functionality.  They can be
     instantiated across multiple contexts, each keeping its own state.
     """
-    def __init__(self, key: str, endpoint:str = PERPLEXITY_API_URL):
+    def __init__(self, key: str, endpoint:str = PERPLEXITY_API_URL, unitTest = False):
         """
         Create a new instance of `perplexipy.PerplexityClient` using the API
         `key` to connect to the corresponding `endpoint`.
 
         Arguments
         ---------
             key
         A valid API key string.  If not present, it defaults to `perplexipy.PERPLEXITY_API_KEY`.
 
             endpoint
-        An string representing a URL to the Perplexity API.
+        A string representing a URL to the Perplexity API.
+
+            unitTest
+        A Boolean to indicate if internal object states need to be modified for
+        unit testing.  Has no effect in regular code.
 
         Returns
         -------
         An instance of `perplexipy.PerplexityClient` if successful.
 
         Attributes:
 
@@ -101,14 +105,15 @@
         self._role = PERPLEXITY_DEFAULT_ROLE
         self._model = PERPLEXITY_DEFAULT_MODEL
         self._client = OpenAI(
             api_key = self._key,
             base_url = self._endpoint,
             timeout = PERPLEXITY_TIMEOUT,
         )
+        self._unitTest = unitTest
 
 
     def query(self, query: str) -> str:
         """
         Send a single message query to the service, receive a single response.
 
         Arguments
@@ -229,15 +234,15 @@
             stream = True,
         )
 
         return Responses(response)
 
 
     @property
-    def models(self):
+    def models(self, unitTest = False):
         """
         Provide a dictionary of the models supported by Perplexity listed in:
 
         https://docs.perplexity.ai/docs/model-cards
 
         Returns
         -------
@@ -248,22 +253,22 @@
         - `parameterCount`
         - `contextLength`
         - `modelType`
         - `availability`
         """
         supportedModels = OrderedDict({
             'codellama-70b-instruct': ModelInfo('70B', 16384, 'chat completion', 'open source',),
-            'llama-3-8b-instruct': ModelInfo('8B', 8192, 'chat completion', 'open source'),
             'llama-3-70b-instruct': ModelInfo('70B', 8192, 'chat completion', 'open source'),
+            'llama-3-8b-instruct': ModelInfo('8B', 8192, 'chat completion', 'open source'),
+            'llama-3-sonar-large-32k-chat': ModelInfo('8x7B', 32768, 'chat completion', 'Perplexity',),
+            'llama-3-sonar-large-32k-online': ModelInfo('8x7B', 32768, 'chat completion', 'Perplexity',),
+            'llama-3-sonar-small-32k-chat': ModelInfo('7B', 32768, 'chat completion', 'Perplexity',),
+            'llama-3-sonar-small-32k-online': ModelInfo('7B', 32768, 'chat completion', 'Perplexity',),
             'mistral-7b-instruct': ModelInfo('7B', 16384, 'chat completion', 'open source',),
             'mixtral-8x7b-instruct': ModelInfo('8x7B', 16384, 'chat completion', 'open source',),
-            'sonar-medium-chat': ModelInfo('8x7B', 16348, 'chat completion', 'Perplexity',),
-            'sonar-medium-online': ModelInfo('8x7B', 12000, 'chat completion', 'Perplexity',),
-            'sonar-small-chat': ModelInfo('7B', 16384, 'chat completion', 'Perplexity',),
-            'sonar-small-online': ModelInfo('7B', 12000, 'chat completion', 'Perplexity',),
         })
 
         return supportedModels
 
 
     @property
     def model(self) -> str:
@@ -292,12 +297,19 @@
         `perplexipy.PerplexityClientError` if the `value` isn't included in the list of
         supported models.
         """
         if not value:
             raise PerplexityClientError('value cannot be None')
 
         models = self.models
-        if value not in models:
-            raise PerplexityClientError('value = %s error; supported models: %s' % (value, ', '.join(models)))
+        if not self._unitTest:
+            if value not in models:
+                raise PerplexityClientError('value = %s error; supported models: %s' % (value, ', '.join(models)))
 
         self._model = value
 
+        # Validate that the model still works, revert otherwise
+        try:
+            self.query('Concise answer: what color is the sky?')
+        except:
+            raise PerplexityClientError('model %s no longer available in underlying API')
+
```

## perplexipy/codex.py

```diff
@@ -242,19 +242,22 @@
 
     return result
 
 
 def _activeModel(modelID: int = 0) -> str:
     if modelID:
         try:
+            modelsList = list(_client.models.keys())
             ref = modelID-1
-            model = list(_client.models.keys())[ref]
+            model = modelsList[ref]
             _client.model = model
         except:
             click.secho('Invalid model ID = %s' % modelID, bg = 'red', fg = 'white')
+            if modelID in range(1, len(modelsList)):
+                click.secho('Model no longer supported by the back-end Perplexity provider', bg = 'bright_yellow', fg = 'black')
     click.secho('Active model: %s\n' % _client.model, fg = 'green', bold = True)
     return _client.model
 
 
 def _REPLHello():
     click.clear()
     printF(HTML('PerplexiPy <b><ansigreen>Codex playground - coding, scripting, and sysops assistant</ansigreen></b>'))
```

## Comparing `PerplexiPy-1.0.5.dist-info/LICENSE.txt` & `PerplexiPy-1.0.6.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `PerplexiPy-1.0.5.dist-info/METADATA` & `PerplexiPy-1.0.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PerplexiPy
-Version: 1.0.5
+Version: 1.0.6
 Summary: PerplexiPy - A robust Perplexity AI API client
 Author-email: CIME Software Ltd <perplexipy@cime.net>
 License: BSD-3
 Project-URL: homepage, https://cime-software.github.io/perplexipy/
 Project-URL: Documentation, https://cime-software.github.io/perplexipy/
 Project-URL: Bug Tracker, https://github.com/CIME-Software/perplexipy/issues
 Project-URL: Source, https://github.com/CIME-Software/perplexipy
@@ -22,15 +22,15 @@
 Requires-Dist: appdirs
 Requires-Dist: click
 Requires-Dist: openai (>=1.12.0)
 Requires-Dist: prompt-toolkit
 Requires-Dist: python-dotenv
 Requires-Dist: pyyaml
 
-% perplexipy(3) Version 1.0.5 | Perplexity AI high level API documentation
+% perplexipy(3) Version 1.0.6 | Perplexity AI high level API documentation
 
 Name
 ====
 
 **PerplexiPy** - Perplexity AI high level library
```

### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: PerplexiPy Version: 1.0.5 Summary: PerplexiPy - A
+Metadata-Version: 2.1 Name: PerplexiPy Version: 1.0.6 Summary: PerplexiPy - A
 robust Perplexity AI API client Author-email: CIME Software Ltd
 cime.net> License: BSD-3 Project-URL: homepage, https://cime-
 software.github.io/perplexipy/ Project-URL: Documentation, https://cime-
 software.github.io/perplexipy/ Project-URL: Bug Tracker, https://github.com/
 CIME-Software/perplexipy/issues Project-URL: Source, https://github.com/CIME-
 Software/perplexipy Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: BSD
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE.txt Requires-Dist: appdirs Requires-Dist: click Requires-Dist: openai
 (>=1.12.0) Requires-Dist: prompt-toolkit Requires-Dist: python-dotenv Requires-
-Dist: pyyaml % perplexipy(3) Version 1.0.5 | Perplexity AI high level API
+Dist: pyyaml % perplexipy(3) Version 1.0.6 | Perplexity AI high level API
 documentation Name ==== **PerplexiPy** - Perplexity AI high level library
 [https://images2.imgbox.com/57/94/AsI1WSfy_o.png]Synopsis ======== ```python
 client = PerplexityClient() \ print(client.query('What is the meaning of 42?')
 \ for result in client.queryStreamable('List of all US presidents'): \ print
 (result) ``` Description =========== **PerplexiPy** is a high-level,
 convenience library for interacting with the Perplexity API from any Python
 3.9+ application. The library aims to simplify interactions with Perplexity
```

## Comparing `PerplexiPy-1.0.5.dist-info/RECORD` & `PerplexiPy-1.0.6.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-perplexipy/__init__.py,sha256=jex9IfNCEyLV3rtpq7L3VEfs75NmHXZki8l6wD-wohA,9253
-perplexipy/codex.py,sha256=-54JQvPd1uP3bk6NS_0UW7BEaWTLR97B4zkMKsWmCOg,13193
+perplexipy/__init__.py,sha256=7E09bh_YwfZHEQhIe6dWTJG28MHh1wl_57GOAa8_ws0,9853
+perplexipy/codex.py,sha256=ZVTXxNkxACxtqkbn3yGd2f-xVx2jhdWWtZBbgQZL2H8,13411
 perplexipy/errors.py,sha256=YM4dVV9q2aLm_ZJdhyCjhejLXdo8mEffx93zlP_7lOs,283
 perplexipy/responses.py,sha256=1OrBpZxGHaVvlE5x9ZtdQhoXP5RbmKOXtHGt6Nm7g2I,684
-PerplexiPy-1.0.5.dist-info/LICENSE.txt,sha256=j9TykfeJa2xvP5Wmggfxaz8pTnedQO9BQX5PbJkh8Yc,1514
-PerplexiPy-1.0.5.dist-info/METADATA,sha256=49S_0LgeHZgVzxPmndB8j_3ra6Ju30DjTZnlQR2C8Jg,6968
-PerplexiPy-1.0.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-PerplexiPy-1.0.5.dist-info/entry_points.txt,sha256=tRB7D5Ao_Rptera8eLiPoF9ecAvHbf5lFSYYaGs9Cfw,49
-PerplexiPy-1.0.5.dist-info/top_level.txt,sha256=JS_DtYqartG2-vkrCiFr0aeoy4Dg6my7DlmUA90wKhA,11
-PerplexiPy-1.0.5.dist-info/RECORD,,
+PerplexiPy-1.0.6.dist-info/LICENSE.txt,sha256=j9TykfeJa2xvP5Wmggfxaz8pTnedQO9BQX5PbJkh8Yc,1514
+PerplexiPy-1.0.6.dist-info/METADATA,sha256=WvRg-ifsD6yTpBZaQCvGuOXWNC-a73B-7Qr_u-1E0f4,6968
+PerplexiPy-1.0.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+PerplexiPy-1.0.6.dist-info/entry_points.txt,sha256=tRB7D5Ao_Rptera8eLiPoF9ecAvHbf5lFSYYaGs9Cfw,49
+PerplexiPy-1.0.6.dist-info/top_level.txt,sha256=JS_DtYqartG2-vkrCiFr0aeoy4Dg6my7DlmUA90wKhA,11
+PerplexiPy-1.0.6.dist-info/RECORD,,
```

