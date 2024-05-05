# Comparing `tmp/ragrank-0.0.6.tar.gz` & `tmp/ragrank-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragrank-0.0.6.tar", max compression
+gzip compressed data, was "ragrank-0.0.7.tar", max compression
```

## Comparing `ragrank-0.0.6.tar` & `ragrank-0.0.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0    11345 2024-03-24 21:47:02.132994 ragrank-0.0.6/LICENSE
--rw-r--r--   0        0        0     3850 2024-03-24 21:47:02.132994 ragrank-0.0.6/README.md
--rw-r--r--   0        0        0     2482 2024-03-24 21:47:02.140994 ragrank-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      292 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/__init__.py
--rw-r--r--   0        0        0     2488 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/_trace.py
--rw-r--r--   0        0        0       27 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/_version.py
--rw-r--r--   0        0        0       34 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/bridge/__init__.py
--rw-r--r--   0        0        0      348 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/bridge/pydantic.py
--rw-r--r--   0        0        0      506 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/constants.py
--rw-r--r--   0        0        0      364 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/dataset/__init__.py
--rw-r--r--   0        0        0     6078 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/dataset/base.py
--rw-r--r--   0        0        0     5453 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/dataset/reader.py
--rw-r--r--   0        0        0      179 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/evaluation/__init__.py
--rw-r--r--   0        0        0     2987 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/evaluation/base.py
--rw-r--r--   0        0        0     3811 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/evaluation/outputs.py
--rw-r--r--   0        0        0      617 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/exceptions.py
--rw-r--r--   0        0        0       34 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/integrations/__init__.py
--rw-r--r--   0        0        0      170 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/integrations/langchain/__init__.py
--rw-r--r--   0        0        0     3813 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/integrations/langchain/langchain_llm_wrapper.py
--rw-r--r--   0        0        0      177 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/integrations/llama_index/__init__.py
--rw-r--r--   0        0        0     2870 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/integrations/llama_index/llamaindex_llm_wrapper.py
--rw-r--r--   0        0        0      124 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/integrations/openai/__init__.py
--rw-r--r--   0        0        0     2772 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/integrations/openai/openai_llm.py
--rw-r--r--   0        0        0      215 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/llm/__init__.py
--rw-r--r--   0        0        0     5090 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/llm/base.py
--rw-r--r--   0        0        0      796 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/metric/__init__.py
--rw-r--r--   0        0        0       48 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/metric/_context_related/__init__.py
--rw-r--r--   0        0        0     3213 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/metric/_context_related/relevancy.py
--rw-r--r--   0        0        0     3245 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/metric/_context_related/utilization.py
--rw-r--r--   0        0        0        0 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/metric/_custom/__init__.py
--rw-r--r--   0        0        0     6103 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/metric/_custom/instruct.py
--rw-r--r--   0        0        0     3553 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/metric/_custom/metric.py
--rw-r--r--   0        0        0       49 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/metric/_response_related/__init__.py
--rw-r--r--   0        0        0     3439 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/metric/_response_related/conciseness.py
--rw-r--r--   0        0        0     3357 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/metric/_response_related/relevancy.py
--rw-r--r--   0        0        0     3255 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/metric/base.py
--rw-r--r--   0        0        0      100 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/prompt/__init__.py
--rw-r--r--   0        0        0     9802 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/prompt/_prompts.py
--rw-r--r--   0        0        0     3510 2024-03-24 21:47:02.140994 ragrank-0.0.6/src/ragrank/prompt/base.py
--rw-r--r--   0        0        0       23 2024-03-24 21:47:02.144994 ragrank-0.0.6/src/ragrank/utils/__init__.py
--rw-r--r--   0        0        0     1319 2024-03-24 21:47:02.144994 ragrank-0.0.6/src/ragrank/utils/common.py
--rw-r--r--   0        0        0      261 2024-03-24 21:47:02.144994 ragrank-0.0.6/src/ragrank/utils/llm.py
--rw-r--r--   0        0        0     4895 1970-01-01 00:00:00.000000 ragrank-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11345 2024-05-05 14:07:09.849640 ragrank-0.0.7/LICENSE
+-rw-r--r--   0        0        0     3847 2024-05-05 14:07:09.849640 ragrank-0.0.7/README.md
+-rw-r--r--   0        0        0     2501 2024-05-05 14:07:09.857640 ragrank-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      292 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/__init__.py
+-rw-r--r--   0        0        0     2488 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/_trace.py
+-rw-r--r--   0        0        0       27 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/_version.py
+-rw-r--r--   0        0        0       34 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/bridge/__init__.py
+-rw-r--r--   0        0        0      348 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/bridge/pydantic.py
+-rw-r--r--   0        0        0      512 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/constants.py
+-rw-r--r--   0        0        0      364 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/dataset/__init__.py
+-rw-r--r--   0        0        0     6078 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/dataset/base.py
+-rw-r--r--   0        0        0     5453 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/dataset/reader.py
+-rw-r--r--   0        0        0      179 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/evaluation/__init__.py
+-rw-r--r--   0        0        0     2987 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/evaluation/base.py
+-rw-r--r--   0        0        0     3811 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/evaluation/outputs.py
+-rw-r--r--   0        0        0      617 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/exceptions.py
+-rw-r--r--   0        0        0       34 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/integrations/__init__.py
+-rw-r--r--   0        0        0      170 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/integrations/langchain/__init__.py
+-rw-r--r--   0        0        0     3813 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/integrations/langchain/langchain_llm_wrapper.py
+-rw-r--r--   0        0        0      177 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/integrations/llama_index/__init__.py
+-rw-r--r--   0        0        0     2870 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/integrations/llama_index/llamaindex_llm_wrapper.py
+-rw-r--r--   0        0        0      124 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/integrations/openai/__init__.py
+-rw-r--r--   0        0        0     2772 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/integrations/openai/openai_llm.py
+-rw-r--r--   0        0        0      215 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/llm/__init__.py
+-rw-r--r--   0        0        0     5090 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/llm/base.py
+-rw-r--r--   0        0        0      796 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/metric/__init__.py
+-rw-r--r--   0        0        0       48 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/metric/_context_related/__init__.py
+-rw-r--r--   0        0        0     3213 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/metric/_context_related/relevancy.py
+-rw-r--r--   0        0        0     3245 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/metric/_context_related/utilization.py
+-rw-r--r--   0        0        0        0 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/metric/_custom/__init__.py
+-rw-r--r--   0        0        0     6103 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/metric/_custom/instruct.py
+-rw-r--r--   0        0        0     3553 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/metric/_custom/metric.py
+-rw-r--r--   0        0        0       49 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/metric/_response_related/__init__.py
+-rw-r--r--   0        0        0     3439 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/metric/_response_related/conciseness.py
+-rw-r--r--   0        0        0     3357 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/metric/_response_related/relevancy.py
+-rw-r--r--   0        0        0     3255 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/metric/base.py
+-rw-r--r--   0        0        0      100 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/prompt/__init__.py
+-rw-r--r--   0        0        0     9802 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/prompt/_prompts.py
+-rw-r--r--   0        0        0     3510 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/prompt/base.py
+-rw-r--r--   0        0        0       23 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/utils/__init__.py
+-rw-r--r--   0        0        0     1319 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/utils/common.py
+-rw-r--r--   0        0        0      261 2024-05-05 14:07:09.857640 ragrank-0.0.7/src/ragrank/utils/llm.py
+-rw-r--r--   0        0        0     4932 1970-01-01 00:00:00.000000 ragrank-0.0.7/PKG-INFO
```

### Comparing `ragrank-0.0.6/LICENSE` & `ragrank-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ragrank-0.0.6/README.md` & `ragrank-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 </p>
 
 <h4 align="center">
     <p>
         <a href="https://ragrank.readthedocs.io/latest/">Documentation</a> |
         <a href="https://api-ragrank.readthedocs.io/">API reference</a> |
         <a href="https://ragrank.readthedocs.io/latest/get_started/basic_evaluation.html">Quickstart</a> |
-        <a href="https://discord.gg/yaFRx6ja">Join the Community</a>
+        <a href="https://discord.gg/KzfVpds3">Join the Community</a>
     <p>
 </h4>
 
 Welcome to Ragrank! This toolkit is designed to assist you in evaluating the performance of your Retrieval-Augmented Generation (RAG) applications. You will get proper metrics for evaluate RAG model. The product is still in `beta` stage.
 
 ## 🔥 Installation
 
@@ -65,19 +65,19 @@
 from ragrank.dataset import from_dict
 from ragrank.metric import response_relevancy
 
 # Define your dataset
 data = from_dict({
     "question": "What is the capital of France?",
     "context": ["France is famous for its iconic landmarks such as the Eiffel Tower and its rich culinary tradition."],
-    "answer": "The capital of France is Paris.",
+    "response": "The capital of France is Paris.",
 })
 
 # Evaluate the response relevance metric
-result = evaluate(data=data, metrics=[response_relevancy])
+result = evaluate(data, metrics=[response_relevancy])
 
 # Display the evaluation results
 result.to_dataframe()
 ```
 
 For more information on how to use Ragrank and its various features, please refer to the [documentation](https://ragrank.readthedocs.io/). 📚
```

#### html2text {}

```diff
@@ -12,20 +12,20 @@
 own custom model, refer [docs](https://ragrank.readthedocs.io/)): ```bash
 export OPENAI_API_KEY="..." ``` Here's a quick example of how you can use
 Ragrank to evaluate the relevance of generated responses: ```python from
 ragrank import evaluate from ragrank.dataset import from_dict from
 ragrank.metric import response_relevancy # Define your dataset data = from_dict
 ({ "question": "What is the capital of France?", "context": ["France is famous
 for its iconic landmarks such as the Eiffel Tower and its rich culinary
-tradition."], "answer": "The capital of France is Paris.", }) # Evaluate the
-response relevance metric result = evaluate(data=data, metrics=
-[response_relevancy]) # Display the evaluation results result.to_dataframe()
-``` For more information on how to use Ragrank and its various features, please
-refer to the [documentation](https://ragrank.readthedocs.io/). ð ## License
-This project is licensed under the [Apache License](https://github.com/Auto-
-Playground/Ragrank/blob/main/LICENSE). Feel free to use and modify it according
-to your needs. ## Feedback and Support If you encounter any issues, have
-questions, or would like to provide feedback, please don't hesitate to open an
-issue on the GitHub repository. Your contributions and suggestions are highly
-appreciated! Join our community on Discord to connect with other users, ask
-questions, and share your experiences with Ragrank. We're here to help you make
-the most out of your NLP projects! ð¬ > Happy evaluating! ð
+tradition."], "response": "The capital of France is Paris.", }) # Evaluate the
+response relevance metric result = evaluate(data, metrics=[response_relevancy])
+# Display the evaluation results result.to_dataframe() ``` For more information
+on how to use Ragrank and its various features, please refer to the
+[documentation](https://ragrank.readthedocs.io/). ð ## License This project
+is licensed under the [Apache License](https://github.com/Auto-Playground/
+Ragrank/blob/main/LICENSE). Feel free to use and modify it according to your
+needs. ## Feedback and Support If you encounter any issues, have questions, or
+would like to provide feedback, please don't hesitate to open an issue on the
+GitHub repository. Your contributions and suggestions are highly appreciated!
+Join our community on Discord to connect with other users, ask questions, and
+share your experiences with Ragrank. We're here to help you make the most out
+of your NLP projects! ð¬ > Happy evaluating! ð
```

### Comparing `ragrank-0.0.6/pyproject.toml` & `ragrank-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ragrank"
-version = "0.0.6"
+version = "0.0.7"
 description = "An evaluation library for RAG models"
 authors = ["Izam Mohammed <izamdeveloper1@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/Auto-Playground/ragrank"
 packages = [
     { include = "ragrank", from = "src" },
@@ -20,14 +20,15 @@
 urllib3 = "^2.2.1"
 requests-toolbelt = "^1.0.0"
 requests = "^2.28.2, !=2.30.0"
 pydantic = "^2.6.3"
 pandas = "^2.2.1"
 tqdm = "^4.66.2"
 datasets = "^2.18.0"
+openai = "^1.14.2"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^7.2.6"
 furo = "^2024.1.29"
```

### Comparing `ragrank-0.0.6/src/ragrank/_trace.py` & `ragrank-0.0.7/src/ragrank/_trace.py`

 * *Files identical despite different names*

### Comparing `ragrank-0.0.6/src/ragrank/dataset/base.py` & `ragrank-0.0.7/src/ragrank/dataset/base.py`

 * *Files identical despite different names*

### Comparing `ragrank-0.0.6/src/ragrank/dataset/reader.py` & `ragrank-0.0.7/src/ragrank/dataset/reader.py`

 * *Files identical despite different names*

### Comparing `ragrank-0.0.6/src/ragrank/evaluation/base.py` & `ragrank-0.0.7/src/ragrank/evaluation/base.py`

 * *Files identical despite different names*

### Comparing `ragrank-0.0.6/src/ragrank/evaluation/outputs.py` & `ragrank-0.0.7/src/ragrank/evaluation/outputs.py`

 * *Files identical despite different names*

### Comparing `ragrank-0.0.6/src/ragrank/exceptions.py` & `ragrank-0.0.7/src/ragrank/exceptions.py`

 * *Files identical despite different names*

### Comparing `ragrank-0.0.6/src/ragrank/integrations/langchain/langchain_llm_wrapper.py` & `ragrank-0.0.7/src/ragrank/integrations/langchain/langchain_llm_wrapper.py`

 * *Files identical despite different names*

### Comparing `ragrank-0.0.6/src/ragrank/integrations/llama_index/llamaindex_llm_wrapper.py` & `ragrank-0.0.7/src/ragrank/integrations/llama_index/llamaindex_llm_wrapper.py`

 * *Files identical despite different names*

### Comparing `ragrank-0.0.6/src/ragrank/integrations/openai/openai_llm.py` & `ragrank-0.0.7/src/ragrank/integrations/openai/openai_llm.py`

 * *Files identical despite different names*

### Comparing `ragrank-0.0.6/src/ragrank/llm/base.py` & `ragrank-0.0.7/src/ragrank/llm/base.py`

 * *Files identical despite different names*

### Comparing `ragrank-0.0.6/src/ragrank/metric/__init__.py` & `ragrank-0.0.7/src/ragrank/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `ragrank-0.0.6/src/ragrank/metric/_context_related/relevancy.py` & `ragrank-0.0.7/src/ragrank/metric/_context_related/relevancy.py`

 * *Files identical despite different names*

### Comparing `ragrank-0.0.6/src/ragrank/metric/_context_related/utilization.py` & `ragrank-0.0.7/src/ragrank/metric/_context_related/utilization.py`

 * *Files identical despite different names*

### Comparing `ragrank-0.0.6/src/ragrank/metric/_custom/instruct.py` & `ragrank-0.0.7/src/ragrank/metric/_custom/instruct.py`

 * *Files identical despite different names*

### Comparing `ragrank-0.0.6/src/ragrank/metric/_custom/metric.py` & `ragrank-0.0.7/src/ragrank/metric/_custom/metric.py`

 * *Files identical despite different names*

### Comparing `ragrank-0.0.6/src/ragrank/metric/_response_related/conciseness.py` & `ragrank-0.0.7/src/ragrank/metric/_response_related/conciseness.py`

 * *Files identical despite different names*

### Comparing `ragrank-0.0.6/src/ragrank/metric/_response_related/relevancy.py` & `ragrank-0.0.7/src/ragrank/metric/_response_related/relevancy.py`

 * *Files identical despite different names*

### Comparing `ragrank-0.0.6/src/ragrank/metric/base.py` & `ragrank-0.0.7/src/ragrank/metric/base.py`

 * *Files identical despite different names*

### Comparing `ragrank-0.0.6/src/ragrank/prompt/_prompts.py` & `ragrank-0.0.7/src/ragrank/prompt/_prompts.py`

 * *Files identical despite different names*

### Comparing `ragrank-0.0.6/src/ragrank/prompt/base.py` & `ragrank-0.0.7/src/ragrank/prompt/base.py`

 * *Files identical despite different names*

### Comparing `ragrank-0.0.6/src/ragrank/utils/common.py` & `ragrank-0.0.7/src/ragrank/utils/common.py`

 * *Files identical despite different names*

### Comparing `ragrank-0.0.6/PKG-INFO` & `ragrank-0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: ragrank
-Version: 0.0.6
+Version: 0.0.7
 Summary: An evaluation library for RAG models
 Home-page: https://github.com/Auto-Playground/ragrank
 License: Apache-2.0
 Keywords: rag,evaluation,llmops
 Author: Izam Mohammed
 Author-email: izamdeveloper1@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: datasets (>=2.18.0,<3.0.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: openai (>=1.14.2,<2.0.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Requires-Dist: pathlib (>=1.0.1,<2.0.0)
 Requires-Dist: pydantic (>=2.6.3,<3.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0,!=2.30.0)
 Requires-Dist: requests-toolbelt (>=1.0.0,<2.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Requires-Dist: urllib3 (>=2.2.1,<3.0.0)
@@ -53,15 +54,15 @@
 </p>
 
 <h4 align="center">
     <p>
         <a href="https://ragrank.readthedocs.io/latest/">Documentation</a> |
         <a href="https://api-ragrank.readthedocs.io/">API reference</a> |
         <a href="https://ragrank.readthedocs.io/latest/get_started/basic_evaluation.html">Quickstart</a> |
-        <a href="https://discord.gg/yaFRx6ja">Join the Community</a>
+        <a href="https://discord.gg/KzfVpds3">Join the Community</a>
     <p>
 </h4>
 
 Welcome to Ragrank! This toolkit is designed to assist you in evaluating the performance of your Retrieval-Augmented Generation (RAG) applications. You will get proper metrics for evaluate RAG model. The product is still in `beta` stage.
 
 ## 🔥 Installation
 
@@ -92,19 +93,19 @@
 from ragrank.dataset import from_dict
 from ragrank.metric import response_relevancy
 
 # Define your dataset
 data = from_dict({
     "question": "What is the capital of France?",
     "context": ["France is famous for its iconic landmarks such as the Eiffel Tower and its rich culinary tradition."],
-    "answer": "The capital of France is Paris.",
+    "response": "The capital of France is Paris.",
 })
 
 # Evaluate the response relevance metric
-result = evaluate(data=data, metrics=[response_relevancy])
+result = evaluate(data, metrics=[response_relevancy])
 
 # Display the evaluation results
 result.to_dataframe()
 ```
 
 For more information on how to use Ragrank and its various features, please refer to the [documentation](https://ragrank.readthedocs.io/). 📚
```

#### html2text {}

```diff
@@ -1,21 +1,22 @@
-Metadata-Version: 2.1 Name: ragrank Version: 0.0.6 Summary: An evaluation
+Metadata-Version: 2.1 Name: ragrank Version: 0.0.7 Summary: An evaluation
 library for RAG models Home-page: https://github.com/Auto-Playground/ragrank
 License: Apache-2.0 Keywords: rag,evaluation,llmops Author: Izam Mohammed
 Author-email: izamdeveloper1@gmail.com Requires-Python: >=3.9,<4.0 Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: datasets (>=2.18.0,<3.0.0) Requires-
-Dist: numpy (>=1.26.4,<2.0.0) Requires-Dist: pandas (>=2.2.1,<3.0.0) Requires-
-Dist: pathlib (>=1.0.1,<2.0.0) Requires-Dist: pydantic (>=2.6.3,<3.0.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0,!=2.30.0) Requires-Dist: requests-
-toolbelt (>=1.0.0,<2.0.0) Requires-Dist: tqdm (>=4.66.2,<5.0.0) Requires-Dist:
-urllib3 (>=2.2.1,<3.0.0) Project-URL: Repository, https://github.com/Auto-
-Playground/ragrank Description-Content-Type: text/markdown
+Dist: numpy (>=1.26.4,<2.0.0) Requires-Dist: openai (>=1.14.2,<2.0.0) Requires-
+Dist: pandas (>=2.2.1,<3.0.0) Requires-Dist: pathlib (>=1.0.1,<2.0.0) Requires-
+Dist: pydantic (>=2.6.3,<3.0.0) Requires-Dist: requests
+(>=2.28.2,<3.0.0,!=2.30.0) Requires-Dist: requests-toolbelt (>=1.0.0,<2.0.0)
+Requires-Dist: tqdm (>=4.66.2,<5.0.0) Requires-Dist: urllib3 (>=2.2.1,<3.0.0)
+Project-URL: Repository, https://github.com/Auto-Playground/ragrank
+Description-Content-Type: text/markdown
                                 [Hashnode logo]
                     [GitHub]_[_B_u_i_l_d_]_[_G_i_t_H_u_b_]_[_G_i_t_H_u_b_]_[_G_i_t_H_u_b_]
     ****** _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn || _AA_PP_II_ _rr_ee_ff_ee_rr_ee_nn_cc_ee || _QQ_uu_ii_cc_kk_ss_tt_aa_rr_tt || _JJ_oo_ii_nn_ _tt_hh_ee_ _CC_oo_mm_mm_uu_nn_ii_tt_yy ******
 Welcome to Ragrank! This toolkit is designed to assist you in evaluating the
 performance of your Retrieval-Augmented Generation (RAG) applications. You will
 get proper metrics for evaluate RAG model. The product is still in `beta`
 stage. ## ð¥ Installation Ragrank is available as a PyPi package. To install
@@ -26,20 +27,20 @@
 own custom model, refer [docs](https://ragrank.readthedocs.io/)): ```bash
 export OPENAI_API_KEY="..." ``` Here's a quick example of how you can use
 Ragrank to evaluate the relevance of generated responses: ```python from
 ragrank import evaluate from ragrank.dataset import from_dict from
 ragrank.metric import response_relevancy # Define your dataset data = from_dict
 ({ "question": "What is the capital of France?", "context": ["France is famous
 for its iconic landmarks such as the Eiffel Tower and its rich culinary
-tradition."], "answer": "The capital of France is Paris.", }) # Evaluate the
-response relevance metric result = evaluate(data=data, metrics=
-[response_relevancy]) # Display the evaluation results result.to_dataframe()
-``` For more information on how to use Ragrank and its various features, please
-refer to the [documentation](https://ragrank.readthedocs.io/). ð ## License
-This project is licensed under the [Apache License](https://github.com/Auto-
-Playground/Ragrank/blob/main/LICENSE). Feel free to use and modify it according
-to your needs. ## Feedback and Support If you encounter any issues, have
-questions, or would like to provide feedback, please don't hesitate to open an
-issue on the GitHub repository. Your contributions and suggestions are highly
-appreciated! Join our community on Discord to connect with other users, ask
-questions, and share your experiences with Ragrank. We're here to help you make
-the most out of your NLP projects! ð¬ > Happy evaluating! ð
+tradition."], "response": "The capital of France is Paris.", }) # Evaluate the
+response relevance metric result = evaluate(data, metrics=[response_relevancy])
+# Display the evaluation results result.to_dataframe() ``` For more information
+on how to use Ragrank and its various features, please refer to the
+[documentation](https://ragrank.readthedocs.io/). ð ## License This project
+is licensed under the [Apache License](https://github.com/Auto-Playground/
+Ragrank/blob/main/LICENSE). Feel free to use and modify it according to your
+needs. ## Feedback and Support If you encounter any issues, have questions, or
+would like to provide feedback, please don't hesitate to open an issue on the
+GitHub repository. Your contributions and suggestions are highly appreciated!
+Join our community on Discord to connect with other users, ask questions, and
+share your experiences with Ragrank. We're here to help you make the most out
+of your NLP projects! ð¬ > Happy evaluating! ð
```

