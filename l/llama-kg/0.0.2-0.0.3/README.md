# Comparing `tmp/llama-kg-0.0.2.tar.gz` & `tmp/llama-kg-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama-kg-0.0.2.tar", last modified: Sun May  5 15:31:41 2024, max compression
+gzip compressed data, was "llama-kg-0.0.3.tar", last modified: Sun May  5 15:42:14 2024, max compression
```

## Comparing `llama-kg-0.0.2.tar` & `llama-kg-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 15:31:41.411897 llama-kg-0.0.2/
--rw-rw-rw-   0        0        0    11558 2024-05-03 23:35:30.000000 llama-kg-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      189 2024-05-05 15:31:41.394540 llama-kg-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       56 2024-05-03 23:35:30.000000 llama-kg-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 15:31:41.271161 llama-kg-0.0.2/llama_kg/
--rw-rw-rw-   0        0        0        0 2024-04-26 14:13:49.000000 llama-kg-0.0.2/llama_kg/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:31:41.306282 llama-kg-0.0.2/llama_kg/index/
--rw-rw-rw-   0        0        0        0 2024-04-26 14:13:49.000000 llama-kg-0.0.2/llama_kg/index/__init__.py
--rw-rw-rw-   0        0        0     4734 2024-04-26 17:24:28.000000 llama-kg-0.0.2/llama_kg/index/base.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:31:41.337654 llama-kg-0.0.2/llama_kg/llm_predictor/
--rw-rw-rw-   0        0        0     1358 2024-04-20 15:13:03.000000 llama-kg-0.0.2/llama_kg/llm_predictor/KronLLMPredictor.py
--rw-rw-rw-   0        0        0     2013 2024-04-20 15:13:03.000000 llama-kg-0.0.2/llama_kg/llm_predictor/KronOpenAILLM.py
--rw-rw-rw-   0        0        0        0 2024-04-26 14:13:49.000000 llama-kg-0.0.2/llama_kg/llm_predictor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:31:41.369781 llama-kg-0.0.2/llama_kg/llm_predictor/llm_predictor/
--rw-rw-rw-   0        0        0     1312 2024-05-05 15:25:56.000000 llama-kg-0.0.2/llama_kg/llm_predictor/llm_predictor/KronLangChainLLM.py
--rw-rw-rw-   0        0        0        0 2024-04-20 15:13:03.000000 llama-kg-0.0.2/llama_kg/llm_predictor/llm_predictor/__init__.py
--rw-rw-rw-   0        0        0     2939 2024-04-20 15:13:03.000000 llama-kg-0.0.2/llama_kg/llm_predictor/llm_predictor/openai_utils.py
--rw-rw-rw-   0        0        0      548 2024-04-20 15:13:03.000000 llama-kg-0.0.2/llama_kg/llm_predictor/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:31:41.392533 llama-kg-0.0.2/llama_kg/readers/
--rw-rw-rw-   0        0        0     5695 2024-04-26 15:11:47.000000 llama-kg-0.0.2/llama_kg/readers/S3ListReader.py
--rw-rw-rw-   0        0        0     6137 2024-04-26 15:11:12.000000 llama-kg-0.0.2/llama_kg/readers/S3Reader.py
--rw-rw-rw-   0        0        0        0 2024-04-26 14:13:49.000000 llama-kg-0.0.2/llama_kg/readers/__init__.py
--rw-rw-rw-   0        0        0      361 2024-05-05 15:31:36.000000 llama-kg-0.0.2/llama_kg/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:31:41.299750 llama-kg-0.0.2/llama_kg.egg-info/
--rw-rw-rw-   0        0        0      189 2024-05-05 15:31:41.000000 llama-kg-0.0.2/llama_kg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      634 2024-05-05 15:31:41.000000 llama-kg-0.0.2/llama_kg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 15:31:41.000000 llama-kg-0.0.2/llama_kg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-05 15:31:41.000000 llama-kg-0.0.2/llama_kg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-05 15:31:41.411897 llama-kg-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-05 15:42:14.982013 llama-kg-0.0.3/
+-rw-rw-rw-   0        0        0    11558 2024-05-03 23:35:30.000000 llama-kg-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      189 2024-05-05 15:42:14.965889 llama-kg-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       56 2024-05-03 23:35:30.000000 llama-kg-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 15:42:14.834112 llama-kg-0.0.3/llama_kg/
+-rw-rw-rw-   0        0        0        0 2024-04-26 14:13:49.000000 llama-kg-0.0.3/llama_kg/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:42:14.873660 llama-kg-0.0.3/llama_kg/index/
+-rw-rw-rw-   0        0        0        0 2024-04-26 14:13:49.000000 llama-kg-0.0.3/llama_kg/index/__init__.py
+-rw-rw-rw-   0        0        0     4734 2024-04-26 17:24:28.000000 llama-kg-0.0.3/llama_kg/index/base.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:42:14.933555 llama-kg-0.0.3/llama_kg/llm_predictor/
+-rw-rw-rw-   0        0        0     1339 2024-05-05 15:40:51.000000 llama-kg-0.0.3/llama_kg/llm_predictor/KronLLMPredictor.py
+-rw-rw-rw-   0        0        0     1312 2024-05-05 15:25:56.000000 llama-kg-0.0.3/llama_kg/llm_predictor/KronLangChainLLM.py
+-rw-rw-rw-   0        0        0     1994 2024-05-05 15:41:50.000000 llama-kg-0.0.3/llama_kg/llm_predictor/KronOpenAILLM.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 14:13:49.000000 llama-kg-0.0.3/llama_kg/llm_predictor/__init__.py
+-rw-rw-rw-   0        0        0     2939 2024-04-20 15:13:03.000000 llama-kg-0.0.3/llama_kg/llm_predictor/openai_utils.py
+-rw-rw-rw-   0        0        0      529 2024-05-05 15:41:18.000000 llama-kg-0.0.3/llama_kg/llm_predictor/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:42:14.964925 llama-kg-0.0.3/llama_kg/readers/
+-rw-rw-rw-   0        0        0     5695 2024-04-26 15:11:47.000000 llama-kg-0.0.3/llama_kg/readers/S3ListReader.py
+-rw-rw-rw-   0        0        0     6137 2024-04-26 15:11:12.000000 llama-kg-0.0.3/llama_kg/readers/S3Reader.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 14:13:49.000000 llama-kg-0.0.3/llama_kg/readers/__init__.py
+-rw-rw-rw-   0        0        0      361 2024-05-05 15:41:41.000000 llama-kg-0.0.3/llama_kg/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:42:14.867476 llama-kg-0.0.3/llama_kg.egg-info/
+-rw-rw-rw-   0        0        0      189 2024-05-05 15:42:14.000000 llama-kg-0.0.3/llama_kg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      557 2024-05-05 15:42:14.000000 llama-kg-0.0.3/llama_kg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 15:42:14.000000 llama-kg-0.0.3/llama_kg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-05 15:42:14.000000 llama-kg-0.0.3/llama_kg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-05 15:42:14.982013 llama-kg-0.0.3/setup.cfg
```

### Comparing `llama-kg-0.0.2/LICENSE` & `llama-kg-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llama-kg-0.0.2/llama_kg/index/base.py` & `llama-kg-0.0.3/llama_kg/index/base.py`

 * *Files identical despite different names*

### Comparing `llama-kg-0.0.2/llama_kg/llm_predictor/KronLLMPredictor.py` & `llama-kg-0.0.3/llama_kg/llm_predictor/KronLLMPredictor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 from typing import Any, Generator, Optional, Protocol, Tuple, runtime_checkable
 
 from llama_index.core.service_context_elements.llm_predictor import  LLMPredictor
 from llama_index.core.llms.utils import LLMType
 from llama_index.core.callbacks.base import CallbackManager
 
-from kron.llm_predictor.utils import kron_resolve_llm
+from utils import kron_resolve_llm
 
 class KronLLMPredictor(LLMPredictor):
     """LLM predictor class.
 
     Wrapper around an LLMChain from Langchain.
 
     Args:
```

### Comparing `llama-kg-0.0.2/llama_kg/llm_predictor/KronOpenAILLM.py` & `llama-kg-0.0.3/llama_kg/llm_predictor/KronOpenAILLM.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     is_chat_model,
     is_function_calling_model,
     openai_modelname_to_contextsize,
     resolve_openai_credentials,
     to_openai_message_dicts,
 )
 
-from kron.llm_predictor.openai_utils import kron_openai_modelname_to_contextsize
+from openai_utils import kron_openai_modelname_to_contextsize
 
 class KronOpenAI(OpenAI):
 
     @property
     def metadata(self) -> LLMMetadata:
         return LLMMetadata(
             context_window=kron_openai_modelname_to_contextsize(self.model),
```

### Comparing `llama-kg-0.0.2/llama_kg/llm_predictor/llm_predictor/KronLangChainLLM.py` & `llama-kg-0.0.3/llama_kg/llm_predictor/KronLangChainLLM.py`

 * *Files identical despite different names*

### Comparing `llama-kg-0.0.2/llama_kg/llm_predictor/llm_predictor/openai_utils.py` & `llama-kg-0.0.3/llama_kg/llm_predictor/openai_utils.py`

 * *Files identical despite different names*

### Comparing `llama-kg-0.0.2/llama_kg/llm_predictor/utils.py` & `llama-kg-0.0.3/llama_kg/llm_predictor/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional, Union
 from llama_index.core.llms.llm import LLM
 from langchain.base_language import BaseLanguageModel
 
-from kron.llm_predictor.KronLangChainLLM import KronLangChainLLM
+from KronLangChainLLM import KronLangChainLLM
 from llama_index.llms.openai import OpenAI
 
 from llama_index.core.llms.utils import LLMType
 
 
 def kron_resolve_llm(llm: Optional[LLMType] = None) -> LLM:
     if isinstance(llm, BaseLanguageModel):
```

### Comparing `llama-kg-0.0.2/llama_kg/readers/S3ListReader.py` & `llama-kg-0.0.3/llama_kg/readers/S3ListReader.py`

 * *Files identical despite different names*

### Comparing `llama-kg-0.0.2/llama_kg/readers/S3Reader.py` & `llama-kg-0.0.3/llama_kg/readers/S3Reader.py`

 * *Files identical despite different names*

### Comparing `llama-kg-0.0.2/llama_kg.egg-info/SOURCES.txt` & `llama-kg-0.0.3/llama_kg.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 llama_kg.egg-info/PKG-INFO
 llama_kg.egg-info/SOURCES.txt
 llama_kg.egg-info/dependency_links.txt
 llama_kg.egg-info/top_level.txt
 llama_kg/index/__init__.py
 llama_kg/index/base.py
 llama_kg/llm_predictor/KronLLMPredictor.py
+llama_kg/llm_predictor/KronLangChainLLM.py
 llama_kg/llm_predictor/KronOpenAILLM.py
 llama_kg/llm_predictor/__init__.py
+llama_kg/llm_predictor/openai_utils.py
 llama_kg/llm_predictor/utils.py
-llama_kg/llm_predictor/llm_predictor/KronLangChainLLM.py
-llama_kg/llm_predictor/llm_predictor/__init__.py
-llama_kg/llm_predictor/llm_predictor/openai_utils.py
 llama_kg/readers/S3ListReader.py
 llama_kg/readers/S3Reader.py
 llama_kg/readers/__init__.py
```

