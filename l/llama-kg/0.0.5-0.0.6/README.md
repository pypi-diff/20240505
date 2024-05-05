# Comparing `tmp/llama-kg-0.0.5.tar.gz` & `tmp/llama-kg-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama-kg-0.0.5.tar", last modified: Sun May  5 16:04:09 2024, max compression
+gzip compressed data, was "llama-kg-0.0.6.tar", last modified: Sun May  5 16:07:29 2024, max compression
```

## Comparing `llama-kg-0.0.5.tar` & `llama-kg-0.0.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 16:04:09.187227 llama-kg-0.0.5/
--rw-rw-rw-   0        0        0    11558 2024-05-03 23:35:30.000000 llama-kg-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      189 2024-05-05 16:04:09.169500 llama-kg-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       56 2024-05-03 23:35:30.000000 llama-kg-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 16:04:09.038173 llama-kg-0.0.5/llama_kg/
--rw-rw-rw-   0        0        0        0 2024-04-26 14:13:49.000000 llama-kg-0.0.5/llama_kg/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 16:04:09.072045 llama-kg-0.0.5/llama_kg/index/
--rw-rw-rw-   0        0        0        0 2024-04-26 14:13:49.000000 llama-kg-0.0.5/llama_kg/index/__init__.py
--rw-rw-rw-   0        0        0     4734 2024-04-26 17:24:28.000000 llama-kg-0.0.5/llama_kg/index/base.py
-drwxrwxrwx   0        0        0        0 2024-05-05 16:04:09.134920 llama-kg-0.0.5/llama_kg/llm_predictor/
--rw-rw-rw-   0        0        0     1362 2024-05-05 16:01:21.000000 llama-kg-0.0.5/llama_kg/llm_predictor/KronLLMPredictor.py
--rw-rw-rw-   0        0        0     1335 2024-05-05 15:54:55.000000 llama-kg-0.0.5/llama_kg/llm_predictor/KronLangChainLLM.py
--rw-rw-rw-   0        0        0     2017 2024-05-05 15:54:00.000000 llama-kg-0.0.5/llama_kg/llm_predictor/KronOpenAILLM.py
--rw-rw-rw-   0        0        0        0 2024-04-26 14:13:49.000000 llama-kg-0.0.5/llama_kg/llm_predictor/__init__.py
--rw-rw-rw-   0        0        0     2939 2024-04-20 15:13:03.000000 llama-kg-0.0.5/llama_kg/llm_predictor/openai_utils.py
--rw-rw-rw-   0        0        0      529 2024-05-05 15:41:18.000000 llama-kg-0.0.5/llama_kg/llm_predictor/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-05 16:04:09.166967 llama-kg-0.0.5/llama_kg/readers/
--rw-rw-rw-   0        0        0     5695 2024-04-26 15:11:47.000000 llama-kg-0.0.5/llama_kg/readers/S3ListReader.py
--rw-rw-rw-   0        0        0     6137 2024-04-26 15:11:12.000000 llama-kg-0.0.5/llama_kg/readers/S3Reader.py
--rw-rw-rw-   0        0        0        0 2024-04-26 14:13:49.000000 llama-kg-0.0.5/llama_kg/readers/__init__.py
--rw-rw-rw-   0        0        0      361 2024-05-05 16:03:31.000000 llama-kg-0.0.5/llama_kg/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 16:04:09.067526 llama-kg-0.0.5/llama_kg.egg-info/
--rw-rw-rw-   0        0        0      189 2024-05-05 16:04:08.000000 llama-kg-0.0.5/llama_kg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      557 2024-05-05 16:04:08.000000 llama-kg-0.0.5/llama_kg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 16:04:08.000000 llama-kg-0.0.5/llama_kg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-05 16:04:08.000000 llama-kg-0.0.5/llama_kg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-05 16:04:09.187227 llama-kg-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-05 16:07:29.479343 llama-kg-0.0.6/
+-rw-rw-rw-   0        0        0    11558 2024-05-03 23:35:30.000000 llama-kg-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      189 2024-05-05 16:07:29.463700 llama-kg-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       56 2024-05-03 23:35:30.000000 llama-kg-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 16:07:29.328247 llama-kg-0.0.6/llama_kg/
+-rw-rw-rw-   0        0        0        0 2024-04-26 14:13:49.000000 llama-kg-0.0.6/llama_kg/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 16:07:29.371953 llama-kg-0.0.6/llama_kg/index/
+-rw-rw-rw-   0        0        0        0 2024-04-26 14:13:49.000000 llama-kg-0.0.6/llama_kg/index/__init__.py
+-rw-rw-rw-   0        0        0     4734 2024-04-26 17:24:28.000000 llama-kg-0.0.6/llama_kg/index/base.py
+drwxrwxrwx   0        0        0        0 2024-05-05 16:07:29.431152 llama-kg-0.0.6/llama_kg/llm_predictor/
+-rw-rw-rw-   0        0        0     1362 2024-05-05 16:01:21.000000 llama-kg-0.0.6/llama_kg/llm_predictor/KronLLMPredictor.py
+-rw-rw-rw-   0        0        0     1335 2024-05-05 15:54:55.000000 llama-kg-0.0.6/llama_kg/llm_predictor/KronLangChainLLM.py
+-rw-rw-rw-   0        0        0     2017 2024-05-05 15:54:00.000000 llama-kg-0.0.6/llama_kg/llm_predictor/KronOpenAILLM.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 14:13:49.000000 llama-kg-0.0.6/llama_kg/llm_predictor/__init__.py
+-rw-rw-rw-   0        0        0     2939 2024-04-20 15:13:03.000000 llama-kg-0.0.6/llama_kg/llm_predictor/openai_utils.py
+-rw-rw-rw-   0        0        0      552 2024-05-05 16:06:45.000000 llama-kg-0.0.6/llama_kg/llm_predictor/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-05 16:07:29.461664 llama-kg-0.0.6/llama_kg/readers/
+-rw-rw-rw-   0        0        0     5695 2024-04-26 15:11:47.000000 llama-kg-0.0.6/llama_kg/readers/S3ListReader.py
+-rw-rw-rw-   0        0        0     6137 2024-04-26 15:11:12.000000 llama-kg-0.0.6/llama_kg/readers/S3Reader.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 14:13:49.000000 llama-kg-0.0.6/llama_kg/readers/__init__.py
+-rw-rw-rw-   0        0        0      361 2024-05-05 16:07:24.000000 llama-kg-0.0.6/llama_kg/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 16:07:29.364949 llama-kg-0.0.6/llama_kg.egg-info/
+-rw-rw-rw-   0        0        0      189 2024-05-05 16:07:29.000000 llama-kg-0.0.6/llama_kg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      557 2024-05-05 16:07:29.000000 llama-kg-0.0.6/llama_kg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 16:07:29.000000 llama-kg-0.0.6/llama_kg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-05 16:07:29.000000 llama-kg-0.0.6/llama_kg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-05 16:07:29.480344 llama-kg-0.0.6/setup.cfg
```

### Comparing `llama-kg-0.0.5/LICENSE` & `llama-kg-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `llama-kg-0.0.5/llama_kg/index/base.py` & `llama-kg-0.0.6/llama_kg/index/base.py`

 * *Files identical despite different names*

### Comparing `llama-kg-0.0.5/llama_kg/llm_predictor/KronLLMPredictor.py` & `llama-kg-0.0.6/llama_kg/llm_predictor/KronLLMPredictor.py`

 * *Files identical despite different names*

### Comparing `llama-kg-0.0.5/llama_kg/llm_predictor/KronLangChainLLM.py` & `llama-kg-0.0.6/llama_kg/llm_predictor/KronLangChainLLM.py`

 * *Files identical despite different names*

### Comparing `llama-kg-0.0.5/llama_kg/llm_predictor/KronOpenAILLM.py` & `llama-kg-0.0.6/llama_kg/llm_predictor/KronOpenAILLM.py`

 * *Files identical despite different names*

### Comparing `llama-kg-0.0.5/llama_kg/llm_predictor/openai_utils.py` & `llama-kg-0.0.6/llama_kg/llm_predictor/openai_utils.py`

 * *Files identical despite different names*

### Comparing `llama-kg-0.0.5/llama_kg/llm_predictor/utils.py` & `llama-kg-0.0.6/llama_kg/llm_predictor/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional, Union
 from llama_index.core.llms.llm import LLM
 from langchain.base_language import BaseLanguageModel
 
-from KronLangChainLLM import KronLangChainLLM
+from llama_kg.llm_predictor.KronLangChainLLM import KronLangChainLLM
 from llama_index.llms.openai import OpenAI
 
 from llama_index.core.llms.utils import LLMType
 
 
 def kron_resolve_llm(llm: Optional[LLMType] = None) -> LLM:
     if isinstance(llm, BaseLanguageModel):
```

### Comparing `llama-kg-0.0.5/llama_kg/readers/S3ListReader.py` & `llama-kg-0.0.6/llama_kg/readers/S3ListReader.py`

 * *Files identical despite different names*

### Comparing `llama-kg-0.0.5/llama_kg/readers/S3Reader.py` & `llama-kg-0.0.6/llama_kg/readers/S3Reader.py`

 * *Files identical despite different names*

### Comparing `llama-kg-0.0.5/llama_kg.egg-info/SOURCES.txt` & `llama-kg-0.0.6/llama_kg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

