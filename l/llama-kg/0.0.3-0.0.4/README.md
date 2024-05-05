# Comparing `tmp/llama-kg-0.0.3.tar.gz` & `tmp/llama-kg-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama-kg-0.0.3.tar", last modified: Sun May  5 15:42:14 2024, max compression
+gzip compressed data, was "llama-kg-0.0.4.tar", last modified: Sun May  5 15:56:28 2024, max compression
```

## Comparing `llama-kg-0.0.3.tar` & `llama-kg-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 15:42:14.982013 llama-kg-0.0.3/
--rw-rw-rw-   0        0        0    11558 2024-05-03 23:35:30.000000 llama-kg-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      189 2024-05-05 15:42:14.965889 llama-kg-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       56 2024-05-03 23:35:30.000000 llama-kg-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 15:42:14.834112 llama-kg-0.0.3/llama_kg/
--rw-rw-rw-   0        0        0        0 2024-04-26 14:13:49.000000 llama-kg-0.0.3/llama_kg/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:42:14.873660 llama-kg-0.0.3/llama_kg/index/
--rw-rw-rw-   0        0        0        0 2024-04-26 14:13:49.000000 llama-kg-0.0.3/llama_kg/index/__init__.py
--rw-rw-rw-   0        0        0     4734 2024-04-26 17:24:28.000000 llama-kg-0.0.3/llama_kg/index/base.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:42:14.933555 llama-kg-0.0.3/llama_kg/llm_predictor/
--rw-rw-rw-   0        0        0     1339 2024-05-05 15:40:51.000000 llama-kg-0.0.3/llama_kg/llm_predictor/KronLLMPredictor.py
--rw-rw-rw-   0        0        0     1312 2024-05-05 15:25:56.000000 llama-kg-0.0.3/llama_kg/llm_predictor/KronLangChainLLM.py
--rw-rw-rw-   0        0        0     1994 2024-05-05 15:41:50.000000 llama-kg-0.0.3/llama_kg/llm_predictor/KronOpenAILLM.py
--rw-rw-rw-   0        0        0        0 2024-04-26 14:13:49.000000 llama-kg-0.0.3/llama_kg/llm_predictor/__init__.py
--rw-rw-rw-   0        0        0     2939 2024-04-20 15:13:03.000000 llama-kg-0.0.3/llama_kg/llm_predictor/openai_utils.py
--rw-rw-rw-   0        0        0      529 2024-05-05 15:41:18.000000 llama-kg-0.0.3/llama_kg/llm_predictor/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:42:14.964925 llama-kg-0.0.3/llama_kg/readers/
--rw-rw-rw-   0        0        0     5695 2024-04-26 15:11:47.000000 llama-kg-0.0.3/llama_kg/readers/S3ListReader.py
--rw-rw-rw-   0        0        0     6137 2024-04-26 15:11:12.000000 llama-kg-0.0.3/llama_kg/readers/S3Reader.py
--rw-rw-rw-   0        0        0        0 2024-04-26 14:13:49.000000 llama-kg-0.0.3/llama_kg/readers/__init__.py
--rw-rw-rw-   0        0        0      361 2024-05-05 15:41:41.000000 llama-kg-0.0.3/llama_kg/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:42:14.867476 llama-kg-0.0.3/llama_kg.egg-info/
--rw-rw-rw-   0        0        0      189 2024-05-05 15:42:14.000000 llama-kg-0.0.3/llama_kg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      557 2024-05-05 15:42:14.000000 llama-kg-0.0.3/llama_kg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 15:42:14.000000 llama-kg-0.0.3/llama_kg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-05 15:42:14.000000 llama-kg-0.0.3/llama_kg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-05 15:42:14.982013 llama-kg-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-05 15:56:28.898324 llama-kg-0.0.4/
+-rw-rw-rw-   0        0        0    11558 2024-05-03 23:35:30.000000 llama-kg-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      189 2024-05-05 15:56:28.881482 llama-kg-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       56 2024-05-03 23:35:30.000000 llama-kg-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 15:56:28.760098 llama-kg-0.0.4/llama_kg/
+-rw-rw-rw-   0        0        0        0 2024-04-26 14:13:49.000000 llama-kg-0.0.4/llama_kg/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:56:28.794501 llama-kg-0.0.4/llama_kg/index/
+-rw-rw-rw-   0        0        0        0 2024-04-26 14:13:49.000000 llama-kg-0.0.4/llama_kg/index/__init__.py
+-rw-rw-rw-   0        0        0     4734 2024-04-26 17:24:28.000000 llama-kg-0.0.4/llama_kg/index/base.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:56:28.850375 llama-kg-0.0.4/llama_kg/llm_predictor/
+-rw-rw-rw-   0        0        0     1339 2024-05-05 15:40:51.000000 llama-kg-0.0.4/llama_kg/llm_predictor/KronLLMPredictor.py
+-rw-rw-rw-   0        0        0     1335 2024-05-05 15:54:55.000000 llama-kg-0.0.4/llama_kg/llm_predictor/KronLangChainLLM.py
+-rw-rw-rw-   0        0        0     2017 2024-05-05 15:54:00.000000 llama-kg-0.0.4/llama_kg/llm_predictor/KronOpenAILLM.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 14:13:49.000000 llama-kg-0.0.4/llama_kg/llm_predictor/__init__.py
+-rw-rw-rw-   0        0        0     2939 2024-04-20 15:13:03.000000 llama-kg-0.0.4/llama_kg/llm_predictor/openai_utils.py
+-rw-rw-rw-   0        0        0      529 2024-05-05 15:41:18.000000 llama-kg-0.0.4/llama_kg/llm_predictor/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:56:28.879483 llama-kg-0.0.4/llama_kg/readers/
+-rw-rw-rw-   0        0        0     5695 2024-04-26 15:11:47.000000 llama-kg-0.0.4/llama_kg/readers/S3ListReader.py
+-rw-rw-rw-   0        0        0     6137 2024-04-26 15:11:12.000000 llama-kg-0.0.4/llama_kg/readers/S3Reader.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 14:13:49.000000 llama-kg-0.0.4/llama_kg/readers/__init__.py
+-rw-rw-rw-   0        0        0      361 2024-05-05 15:56:16.000000 llama-kg-0.0.4/llama_kg/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:56:28.789962 llama-kg-0.0.4/llama_kg.egg-info/
+-rw-rw-rw-   0        0        0      189 2024-05-05 15:56:28.000000 llama-kg-0.0.4/llama_kg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      557 2024-05-05 15:56:28.000000 llama-kg-0.0.4/llama_kg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 15:56:28.000000 llama-kg-0.0.4/llama_kg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-05 15:56:28.000000 llama-kg-0.0.4/llama_kg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-05 15:56:28.899324 llama-kg-0.0.4/setup.cfg
```

### Comparing `llama-kg-0.0.3/LICENSE` & `llama-kg-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `llama-kg-0.0.3/llama_kg/index/base.py` & `llama-kg-0.0.4/llama_kg/index/base.py`

 * *Files identical despite different names*

### Comparing `llama-kg-0.0.3/llama_kg/llm_predictor/KronLLMPredictor.py` & `llama-kg-0.0.4/llama_kg/llm_predictor/KronLLMPredictor.py`

 * *Files identical despite different names*

### Comparing `llama-kg-0.0.3/llama_kg/llm_predictor/KronLangChainLLM.py` & `llama-kg-0.0.4/llama_kg/llm_predictor/KronLangChainLLM.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from llama_index.core.bridge.langchain import BaseLanguageModel, BaseChatModel
 from llama_index.llms.langchain import LangChainLLM
 from llama_index.core.bridge.langchain import OpenAI, ChatOpenAI
 
 from llama_index.core.llms import LLMMetadata
 
-from openai_utils import kron_openai_modelname_to_contextsize
+from llama_kg.llm_predictor.openai_utils import kron_openai_modelname_to_contextsize
 
 def is_chat_model(llm: BaseLanguageModel) -> bool:
     return isinstance(llm, BaseChatModel)
 
 class KronLangChainLLM(LangChainLLM):
     """Adapter for a LangChain LLM."""
```

### Comparing `llama-kg-0.0.3/llama_kg/llm_predictor/KronOpenAILLM.py` & `llama-kg-0.0.4/llama_kg/llm_predictor/KronOpenAILLM.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     is_chat_model,
     is_function_calling_model,
     openai_modelname_to_contextsize,
     resolve_openai_credentials,
     to_openai_message_dicts,
 )
 
-from openai_utils import kron_openai_modelname_to_contextsize
+from llama_kg.llm_predictor.openai_utils import kron_openai_modelname_to_contextsize
 
 class KronOpenAI(OpenAI):
 
     @property
     def metadata(self) -> LLMMetadata:
         return LLMMetadata(
             context_window=kron_openai_modelname_to_contextsize(self.model),
```

### Comparing `llama-kg-0.0.3/llama_kg/llm_predictor/openai_utils.py` & `llama-kg-0.0.4/llama_kg/llm_predictor/openai_utils.py`

 * *Files identical despite different names*

### Comparing `llama-kg-0.0.3/llama_kg/llm_predictor/utils.py` & `llama-kg-0.0.4/llama_kg/llm_predictor/utils.py`

 * *Files identical despite different names*

### Comparing `llama-kg-0.0.3/llama_kg/readers/S3ListReader.py` & `llama-kg-0.0.4/llama_kg/readers/S3ListReader.py`

 * *Files identical despite different names*

### Comparing `llama-kg-0.0.3/llama_kg/readers/S3Reader.py` & `llama-kg-0.0.4/llama_kg/readers/S3Reader.py`

 * *Files identical despite different names*

### Comparing `llama-kg-0.0.3/llama_kg.egg-info/SOURCES.txt` & `llama-kg-0.0.4/llama_kg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

