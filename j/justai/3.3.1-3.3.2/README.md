# Comparing `tmp/justai-3.3.1.tar.gz` & `tmp/justai-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "justai-3.3.1.tar", last modified: Thu May  2 08:29:32 2024, max compression
+gzip compressed data, was "justai-3.3.2.tar", last modified: Sun May  5 14:42:02 2024, max compression
```

## Comparing `justai-3.3.1.tar` & `justai-3.3.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-02 08:29:32.127888 justai-3.3.1/
--rw-r--r--   0 hp         (501) staff       (20)     1211 2020-11-28 21:10:12.000000 justai-3.3.1/LICENSE
--rw-r--r--   0 hp         (501) staff       (20)      198 2024-02-20 10:20:38.000000 justai-3.3.1/MANIFEST.in
--rw-r--r--   0 hp         (501) staff       (20)     6448 2024-05-02 08:29:32.127579 justai-3.3.1/PKG-INFO
--rw-r--r--   0 hp         (501) staff       (20)     4082 2024-05-02 08:29:29.000000 justai-3.3.1/README.md
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-02 08:29:32.117151 justai-3.3.1/justai/
--rw-r--r--   0 hp         (501) staff       (20)      579 2024-04-01 20:26:06.000000 justai-3.3.1/justai/__init__.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-02 08:29:32.119347 justai-3.3.1/justai/agent/
--rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:05:20.000000 justai-3.3.1/justai/agent/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     5992 2024-03-31 21:07:33.000000 justai-3.3.1/justai/agent/agent.py
--rw-r--r--   0 hp         (501) staff       (20)      997 2024-03-05 16:49:21.000000 justai-3.3.1/justai/agent/message.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-02 08:29:32.120430 justai-3.3.1/justai/interactive/
--rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:06:50.000000 justai-3.3.1/justai/interactive/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     5452 2024-02-07 19:49:01.000000 justai-3.3.1/justai/interactive/commands.py
--rw-r--r--   0 hp         (501) staff       (20)     1320 2024-03-05 16:26:44.000000 justai-3.3.1/justai/interactive/repl.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-02 08:29:32.122134 justai-3.3.1/justai/models/
--rw-r--r--   0 hp         (501) staff       (20)     2987 2024-04-30 15:37:24.000000 justai-3.3.1/justai/models/anthropic_models.py
--rw-r--r--   0 hp         (501) staff       (20)     2465 2024-05-02 08:28:02.000000 justai-3.3.1/justai/models/gguf_models.py
--rw-r--r--   0 hp         (501) staff       (20)      920 2024-04-30 15:42:29.000000 justai-3.3.1/justai/models/model.py
--rw-r--r--   0 hp         (501) staff       (20)      709 2024-03-06 13:20:05.000000 justai-3.3.1/justai/models/modelfactory.py
--rw-r--r--   0 hp         (501) staff       (20)     5907 2024-04-04 20:33:40.000000 justai-3.3.1/justai/models/openai_models.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-02 08:29:32.123830 justai-3.3.1/justai/tools/
--rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:08:21.000000 justai-3.3.1/justai/tools/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     3815 2024-04-02 09:00:24.000000 justai-3.3.1/justai/tools/cache.py
--rw-r--r--   0 hp         (501) staff       (20)      563 2023-08-26 19:32:55.000000 justai-3.3.1/justai/tools/display.py
--rw-r--r--   0 hp         (501) staff       (20)     3479 2024-04-29 12:34:52.000000 justai-3.3.1/justai/tools/log.py
--rw-r--r--   0 hp         (501) staff       (20)      615 2024-02-09 15:06:31.000000 justai-3.3.1/justai/tools/prompts.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-02 08:29:32.126026 justai-3.3.1/justai/translator/
--rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:11:10.000000 justai-3.3.1/justai/translator/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     4052 2024-02-13 10:39:31.000000 justai-3.3.1/justai/translator/languages.py
--rw-r--r--   0 hp         (501) staff       (20)     1759 2024-04-05 09:44:01.000000 justai-3.3.1/justai/translator/prompts.toml
--rw-r--r--   0 hp         (501) staff       (20)    16620 2024-04-29 12:34:32.000000 justai-3.3.1/justai/translator/translator.py
--rw-r--r--   0 hp         (501) staff       (20)     5243 2024-02-16 15:51:36.000000 justai-3.3.1/justai/translator/xliff.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-02 08:29:32.126625 justai-3.3.1/justai.egg-info/
--rw-r--r--   0 hp         (501) staff       (20)     6448 2024-05-02 08:29:32.000000 justai-3.3.1/justai.egg-info/PKG-INFO
--rw-r--r--   0 hp         (501) staff       (20)      785 2024-05-02 08:29:32.000000 justai-3.3.1/justai.egg-info/SOURCES.txt
--rw-r--r--   0 hp         (501) staff       (20)        1 2024-05-02 08:29:32.000000 justai-3.3.1/justai.egg-info/dependency_links.txt
--rw-r--r--   0 hp         (501) staff       (20)      146 2024-05-02 08:29:32.000000 justai-3.3.1/justai.egg-info/requires.txt
--rw-r--r--   0 hp         (501) staff       (20)        7 2024-05-02 08:29:32.000000 justai-3.3.1/justai.egg-info/top_level.txt
--rw-r--r--   0 hp         (501) staff       (20)      894 2024-05-02 08:29:29.000000 justai-3.3.1/pyproject.toml
--rw-r--r--   0 hp         (501) staff       (20)       38 2024-05-02 08:29:32.127961 justai-3.3.1/setup.cfg
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-05 14:42:02.784314 justai-3.3.2/
+-rw-r--r--   0 hp         (501) staff       (20)     1211 2020-11-28 21:10:12.000000 justai-3.3.2/LICENSE
+-rw-r--r--   0 hp         (501) staff       (20)      198 2024-02-20 10:20:38.000000 justai-3.3.2/MANIFEST.in
+-rw-r--r--   0 hp         (501) staff       (20)     6448 2024-05-05 14:42:02.784103 justai-3.3.2/PKG-INFO
+-rw-r--r--   0 hp         (501) staff       (20)     4082 2024-05-05 14:42:01.000000 justai-3.3.2/README.md
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-05 14:42:02.776805 justai-3.3.2/justai/
+-rw-r--r--   0 hp         (501) staff       (20)      579 2024-04-01 20:26:06.000000 justai-3.3.2/justai/__init__.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-05 14:42:02.778114 justai-3.3.2/justai/agent/
+-rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:05:20.000000 justai-3.3.2/justai/agent/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     5992 2024-03-31 21:07:33.000000 justai-3.3.2/justai/agent/agent.py
+-rw-r--r--   0 hp         (501) staff       (20)      997 2024-03-05 16:49:21.000000 justai-3.3.2/justai/agent/message.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-05 14:42:02.779889 justai-3.3.2/justai/interactive/
+-rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:06:50.000000 justai-3.3.2/justai/interactive/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     5452 2024-02-07 19:49:01.000000 justai-3.3.2/justai/interactive/commands.py
+-rw-r--r--   0 hp         (501) staff       (20)     1320 2024-03-05 16:26:44.000000 justai-3.3.2/justai/interactive/repl.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-05 14:42:02.781044 justai-3.3.2/justai/models/
+-rw-r--r--   0 hp         (501) staff       (20)     2987 2024-04-30 15:37:24.000000 justai-3.3.2/justai/models/anthropic_models.py
+-rw-r--r--   0 hp         (501) staff       (20)     2465 2024-05-02 08:28:02.000000 justai-3.3.2/justai/models/gguf_models.py
+-rw-r--r--   0 hp         (501) staff       (20)      920 2024-04-30 15:42:29.000000 justai-3.3.2/justai/models/model.py
+-rw-r--r--   0 hp         (501) staff       (20)      709 2024-03-06 13:20:05.000000 justai-3.3.2/justai/models/modelfactory.py
+-rw-r--r--   0 hp         (501) staff       (20)     5907 2024-04-04 20:33:40.000000 justai-3.3.2/justai/models/openai_models.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-05 14:42:02.782073 justai-3.3.2/justai/tools/
+-rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:08:21.000000 justai-3.3.2/justai/tools/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     3815 2024-04-02 09:00:24.000000 justai-3.3.2/justai/tools/cache.py
+-rw-r--r--   0 hp         (501) staff       (20)      563 2023-08-26 19:32:55.000000 justai-3.3.2/justai/tools/display.py
+-rw-r--r--   0 hp         (501) staff       (20)     3479 2024-04-29 12:34:52.000000 justai-3.3.2/justai/tools/log.py
+-rw-r--r--   0 hp         (501) staff       (20)      615 2024-02-09 15:06:31.000000 justai-3.3.2/justai/tools/prompts.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-05 14:42:02.783286 justai-3.3.2/justai/translator/
+-rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:11:10.000000 justai-3.3.2/justai/translator/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     4052 2024-02-13 10:39:31.000000 justai-3.3.2/justai/translator/languages.py
+-rw-r--r--   0 hp         (501) staff       (20)     1759 2024-04-05 09:44:01.000000 justai-3.3.2/justai/translator/prompts.toml
+-rw-r--r--   0 hp         (501) staff       (20)    16685 2024-05-05 14:41:25.000000 justai-3.3.2/justai/translator/translator.py
+-rw-r--r--   0 hp         (501) staff       (20)     5243 2024-02-16 15:51:36.000000 justai-3.3.2/justai/translator/xliff.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-05 14:42:02.783551 justai-3.3.2/justai.egg-info/
+-rw-r--r--   0 hp         (501) staff       (20)     6448 2024-05-05 14:42:02.000000 justai-3.3.2/justai.egg-info/PKG-INFO
+-rw-r--r--   0 hp         (501) staff       (20)      785 2024-05-05 14:42:02.000000 justai-3.3.2/justai.egg-info/SOURCES.txt
+-rw-r--r--   0 hp         (501) staff       (20)        1 2024-05-05 14:42:02.000000 justai-3.3.2/justai.egg-info/dependency_links.txt
+-rw-r--r--   0 hp         (501) staff       (20)      146 2024-05-05 14:42:02.000000 justai-3.3.2/justai.egg-info/requires.txt
+-rw-r--r--   0 hp         (501) staff       (20)        7 2024-05-05 14:42:02.000000 justai-3.3.2/justai.egg-info/top_level.txt
+-rw-r--r--   0 hp         (501) staff       (20)      894 2024-05-05 14:42:01.000000 justai-3.3.2/pyproject.toml
+-rw-r--r--   0 hp         (501) staff       (20)       38 2024-05-05 14:42:02.784362 justai-3.3.2/setup.cfg
```

### Comparing `justai-3.3.1/LICENSE` & `justai-3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `justai-3.3.1/PKG-INFO` & `justai-3.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: justai
-Version: 3.3.1
+Version: 3.3.2
 Summary: Makes working with OpenAI's GPT API and other LLM's super easy
 Author-email: HP Harmsen <hp@harmsen.nl>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -54,15 +54,15 @@
 Requires-Dist: llama-cpp-python; extra == "llama"
 
 # JustAI
 
 Package to make working with Large Language models in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 3.3.1
+Current version: 3.3.2
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install justai
 ~~~~
 2. Create an OpenAI acccount (for GPT3.5 / 4) [here](https://platform.openai.com/) or an Anthropic account [here](https://console.anthropic.com/)
```

### Comparing `justai-3.3.1/README.md` & `justai-3.3.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # JustAI
 
 Package to make working with Large Language models in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 3.3.1
+Current version: 3.3.2
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install justai
 ~~~~
 2. Create an OpenAI acccount (for GPT3.5 / 4) [here](https://platform.openai.com/) or an Anthropic account [here](https://console.anthropic.com/)
```

### Comparing `justai-3.3.1/justai/__init__.py` & `justai-3.3.2/justai/__init__.py`

 * *Files identical despite different names*

### Comparing `justai-3.3.1/justai/agent/agent.py` & `justai-3.3.2/justai/agent/agent.py`

 * *Files identical despite different names*

### Comparing `justai-3.3.1/justai/agent/message.py` & `justai-3.3.2/justai/agent/message.py`

 * *Files identical despite different names*

### Comparing `justai-3.3.1/justai/interactive/commands.py` & `justai-3.3.2/justai/interactive/commands.py`

 * *Files identical despite different names*

### Comparing `justai-3.3.1/justai/interactive/repl.py` & `justai-3.3.2/justai/interactive/repl.py`

 * *Files identical despite different names*

### Comparing `justai-3.3.1/justai/models/anthropic_models.py` & `justai-3.3.2/justai/models/anthropic_models.py`

 * *Files identical despite different names*

### Comparing `justai-3.3.1/justai/models/gguf_models.py` & `justai-3.3.2/justai/models/gguf_models.py`

 * *Files identical despite different names*

### Comparing `justai-3.3.1/justai/models/model.py` & `justai-3.3.2/justai/models/model.py`

 * *Files identical despite different names*

### Comparing `justai-3.3.1/justai/models/modelfactory.py` & `justai-3.3.2/justai/models/modelfactory.py`

 * *Files identical despite different names*

### Comparing `justai-3.3.1/justai/models/openai_models.py` & `justai-3.3.2/justai/models/openai_models.py`

 * *Files identical despite different names*

### Comparing `justai-3.3.1/justai/tools/cache.py` & `justai-3.3.2/justai/tools/cache.py`

 * *Files identical despite different names*

### Comparing `justai-3.3.1/justai/tools/display.py` & `justai-3.3.2/justai/tools/display.py`

 * *Files identical despite different names*

### Comparing `justai-3.3.1/justai/tools/log.py` & `justai-3.3.2/justai/tools/log.py`

 * *Files identical despite different names*

### Comparing `justai-3.3.1/justai/tools/prompts.py` & `justai-3.3.2/justai/tools/prompts.py`

 * *Files identical despite different names*

### Comparing `justai-3.3.1/justai/translator/languages.py` & `justai-3.3.2/justai/translator/languages.py`

 * *Files identical despite different names*

### Comparing `justai-3.3.1/justai/translator/prompts.toml` & `justai-3.3.2/justai/translator/prompts.toml`

 * *Files identical despite different names*

### Comparing `justai-3.3.1/justai/translator/translator.py` & `justai-3.3.2/justai/translator/translator.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,14 +120,15 @@
 
     def do_translate(self, texts, language: str, options: dict = {}):
         # Options can be:
         # REPLACE_VARIABLES: True | False
         # LOG: True | False
         # STRING_CACHED: True | False
         # CONCATENATED: True | False
+        # PROMPT = 'prompt'  # Om een eigen prompt mee te geven.
 
         # assert all(is_translatable(text) for text in texts), "Not all translatable"  # !! Tijdelijk
         cache = StringCache(language) if options.get(Opt.STRING_CACHED) else {}
         source_list = [text for text in texts if text not in cache]
 
         if source_list:
             variables = []
```

### Comparing `justai-3.3.1/justai/translator/xliff.py` & `justai-3.3.2/justai/translator/xliff.py`

 * *Files identical despite different names*

### Comparing `justai-3.3.1/justai.egg-info/PKG-INFO` & `justai-3.3.2/justai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: justai
-Version: 3.3.1
+Version: 3.3.2
 Summary: Makes working with OpenAI's GPT API and other LLM's super easy
 Author-email: HP Harmsen <hp@harmsen.nl>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -54,15 +54,15 @@
 Requires-Dist: llama-cpp-python; extra == "llama"
 
 # JustAI
 
 Package to make working with Large Language models in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 3.3.1
+Current version: 3.3.2
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install justai
 ~~~~
 2. Create an OpenAI acccount (for GPT3.5 / 4) [here](https://platform.openai.com/) or an Anthropic account [here](https://console.anthropic.com/)
```

### Comparing `justai-3.3.1/justai.egg-info/SOURCES.txt` & `justai-3.3.2/justai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `justai-3.3.1/pyproject.toml` & `justai-3.3.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=69", "wheel>=0.42"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "justai"
-version = "3.3.1"
+version = "3.3.2"
 description = "Makes working with OpenAI's GPT API and other LLM's super easy"
 readme = "README.md"
 authors = [{ name = "HP Harmsen", email = "hp@harmsen.nl" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

