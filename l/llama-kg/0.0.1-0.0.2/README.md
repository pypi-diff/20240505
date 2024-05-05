# Comparing `tmp/llama-kg-0.0.1.tar.gz` & `tmp/llama-kg-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama-kg-0.0.1.tar", last modified: Fri May  3 23:48:37 2024, max compression
+gzip compressed data, was "llama-kg-0.0.2.tar", last modified: Sun May  5 15:31:41 2024, max compression
```

## Comparing `llama-kg-0.0.1.tar` & `llama-kg-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 23:48:37.344758 llama-kg-0.0.1/
--rw-rw-rw-   0        0        0    11558 2024-05-03 23:35:30.000000 llama-kg-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      189 2024-05-03 23:48:37.330675 llama-kg-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       56 2024-05-03 23:35:30.000000 llama-kg-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 23:48:37.146414 llama-kg-0.0.1/llama_kg/
--rw-rw-rw-   0        0        0        0 2024-04-26 14:13:49.000000 llama-kg-0.0.1/llama_kg/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 23:48:37.175327 llama-kg-0.0.1/llama_kg/index/
--rw-rw-rw-   0        0        0        0 2024-04-26 14:13:49.000000 llama-kg-0.0.1/llama_kg/index/__init__.py
--rw-rw-rw-   0        0        0     4734 2024-04-26 17:24:28.000000 llama-kg-0.0.1/llama_kg/index/base.py
-drwxrwxrwx   0        0        0        0 2024-05-03 23:48:37.233749 llama-kg-0.0.1/llama_kg/llm_predictor/
--rw-rw-rw-   0        0        0     1358 2024-04-20 15:13:03.000000 llama-kg-0.0.1/llama_kg/llm_predictor/KronLLMPredictor.py
--rw-rw-rw-   0        0        0     2013 2024-04-20 15:13:03.000000 llama-kg-0.0.1/llama_kg/llm_predictor/KronOpenAILLM.py
--rw-rw-rw-   0        0        0        0 2024-04-26 14:13:49.000000 llama-kg-0.0.1/llama_kg/llm_predictor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 23:48:37.295536 llama-kg-0.0.1/llama_kg/llm_predictor/llm_predictor/
--rw-rw-rw-   0        0        0     1331 2024-04-20 15:13:03.000000 llama-kg-0.0.1/llama_kg/llm_predictor/llm_predictor/KronLangChainLLM.py
--rw-rw-rw-   0        0        0        0 2024-04-20 15:13:03.000000 llama-kg-0.0.1/llama_kg/llm_predictor/llm_predictor/__init__.py
--rw-rw-rw-   0        0        0     2939 2024-04-20 15:13:03.000000 llama-kg-0.0.1/llama_kg/llm_predictor/llm_predictor/openai_utils.py
--rw-rw-rw-   0        0        0      548 2024-04-20 15:13:03.000000 llama-kg-0.0.1/llama_kg/llm_predictor/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-03 23:48:37.327198 llama-kg-0.0.1/llama_kg/readers/
--rw-rw-rw-   0        0        0     5695 2024-04-26 15:11:47.000000 llama-kg-0.0.1/llama_kg/readers/S3ListReader.py
--rw-rw-rw-   0        0        0     6137 2024-04-26 15:11:12.000000 llama-kg-0.0.1/llama_kg/readers/S3Reader.py
--rw-rw-rw-   0        0        0        0 2024-04-26 14:13:49.000000 llama-kg-0.0.1/llama_kg/readers/__init__.py
--rw-rw-rw-   0        0        0      361 2024-04-26 14:23:36.000000 llama-kg-0.0.1/llama_kg/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-03 23:48:37.169715 llama-kg-0.0.1/llama_kg.egg-info/
--rw-rw-rw-   0        0        0      189 2024-05-03 23:48:36.000000 llama-kg-0.0.1/llama_kg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      634 2024-05-03 23:48:36.000000 llama-kg-0.0.1/llama_kg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 23:48:36.000000 llama-kg-0.0.1/llama_kg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-03 23:48:36.000000 llama-kg-0.0.1/llama_kg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 23:48:37.345275 llama-kg-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-05 15:31:41.411897 llama-kg-0.0.2/
+-rw-rw-rw-   0        0        0    11558 2024-05-03 23:35:30.000000 llama-kg-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      189 2024-05-05 15:31:41.394540 llama-kg-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       56 2024-05-03 23:35:30.000000 llama-kg-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 15:31:41.271161 llama-kg-0.0.2/llama_kg/
+-rw-rw-rw-   0        0        0        0 2024-04-26 14:13:49.000000 llama-kg-0.0.2/llama_kg/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:31:41.306282 llama-kg-0.0.2/llama_kg/index/
+-rw-rw-rw-   0        0        0        0 2024-04-26 14:13:49.000000 llama-kg-0.0.2/llama_kg/index/__init__.py
+-rw-rw-rw-   0        0        0     4734 2024-04-26 17:24:28.000000 llama-kg-0.0.2/llama_kg/index/base.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:31:41.337654 llama-kg-0.0.2/llama_kg/llm_predictor/
+-rw-rw-rw-   0        0        0     1358 2024-04-20 15:13:03.000000 llama-kg-0.0.2/llama_kg/llm_predictor/KronLLMPredictor.py
+-rw-rw-rw-   0        0        0     2013 2024-04-20 15:13:03.000000 llama-kg-0.0.2/llama_kg/llm_predictor/KronOpenAILLM.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 14:13:49.000000 llama-kg-0.0.2/llama_kg/llm_predictor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:31:41.369781 llama-kg-0.0.2/llama_kg/llm_predictor/llm_predictor/
+-rw-rw-rw-   0        0        0     1312 2024-05-05 15:25:56.000000 llama-kg-0.0.2/llama_kg/llm_predictor/llm_predictor/KronLangChainLLM.py
+-rw-rw-rw-   0        0        0        0 2024-04-20 15:13:03.000000 llama-kg-0.0.2/llama_kg/llm_predictor/llm_predictor/__init__.py
+-rw-rw-rw-   0        0        0     2939 2024-04-20 15:13:03.000000 llama-kg-0.0.2/llama_kg/llm_predictor/llm_predictor/openai_utils.py
+-rw-rw-rw-   0        0        0      548 2024-04-20 15:13:03.000000 llama-kg-0.0.2/llama_kg/llm_predictor/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:31:41.392533 llama-kg-0.0.2/llama_kg/readers/
+-rw-rw-rw-   0        0        0     5695 2024-04-26 15:11:47.000000 llama-kg-0.0.2/llama_kg/readers/S3ListReader.py
+-rw-rw-rw-   0        0        0     6137 2024-04-26 15:11:12.000000 llama-kg-0.0.2/llama_kg/readers/S3Reader.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 14:13:49.000000 llama-kg-0.0.2/llama_kg/readers/__init__.py
+-rw-rw-rw-   0        0        0      361 2024-05-05 15:31:36.000000 llama-kg-0.0.2/llama_kg/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:31:41.299750 llama-kg-0.0.2/llama_kg.egg-info/
+-rw-rw-rw-   0        0        0      189 2024-05-05 15:31:41.000000 llama-kg-0.0.2/llama_kg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      634 2024-05-05 15:31:41.000000 llama-kg-0.0.2/llama_kg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 15:31:41.000000 llama-kg-0.0.2/llama_kg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-05 15:31:41.000000 llama-kg-0.0.2/llama_kg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-05 15:31:41.411897 llama-kg-0.0.2/setup.cfg
```

### Comparing `llama-kg-0.0.1/LICENSE` & `llama-kg-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llama-kg-0.0.1/llama_kg/index/base.py` & `llama-kg-0.0.2/llama_kg/index/base.py`

 * *Files identical despite different names*

### Comparing `llama-kg-0.0.1/llama_kg/llm_predictor/KronLLMPredictor.py` & `llama-kg-0.0.2/llama_kg/llm_predictor/KronLLMPredictor.py`

 * *Files identical despite different names*

### Comparing `llama-kg-0.0.1/llama_kg/llm_predictor/KronOpenAILLM.py` & `llama-kg-0.0.2/llama_kg/llm_predictor/KronOpenAILLM.py`

 * *Files identical despite different names*

### Comparing `llama-kg-0.0.1/llama_kg/llm_predictor/llm_predictor/KronLangChainLLM.py` & `llama-kg-0.0.2/llama_kg/llm_predictor/llm_predictor/KronLangChainLLM.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from llama_index.core.bridge.langchain import BaseLanguageModel, BaseChatModel
 from llama_index.llms.langchain import LangChainLLM
 from llama_index.core.bridge.langchain import OpenAI, ChatOpenAI
 
 from llama_index.core.llms import LLMMetadata
 
-from kron.llm_predictor.openai_utils import kron_openai_modelname_to_contextsize
+from openai_utils import kron_openai_modelname_to_contextsize
 
 def is_chat_model(llm: BaseLanguageModel) -> bool:
     return isinstance(llm, BaseChatModel)
 
 class KronLangChainLLM(LangChainLLM):
     """Adapter for a LangChain LLM."""
```

### Comparing `llama-kg-0.0.1/llama_kg/llm_predictor/llm_predictor/openai_utils.py` & `llama-kg-0.0.2/llama_kg/llm_predictor/llm_predictor/openai_utils.py`

 * *Files identical despite different names*

### Comparing `llama-kg-0.0.1/llama_kg/llm_predictor/utils.py` & `llama-kg-0.0.2/llama_kg/llm_predictor/utils.py`

 * *Files identical despite different names*

### Comparing `llama-kg-0.0.1/llama_kg/readers/S3ListReader.py` & `llama-kg-0.0.2/llama_kg/readers/S3ListReader.py`

 * *Files identical despite different names*

### Comparing `llama-kg-0.0.1/llama_kg/readers/S3Reader.py` & `llama-kg-0.0.2/llama_kg/readers/S3Reader.py`

 * *Files identical despite different names*

### Comparing `llama-kg-0.0.1/llama_kg.egg-info/SOURCES.txt` & `llama-kg-0.0.2/llama_kg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

