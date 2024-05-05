# Comparing `tmp/rag_retrieval-0.2.0.tar.gz` & `tmp/rag_retrieval-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rag_retrieval-0.2.0.tar", last modified: Sat May  4 09:15:10 2024, max compression
+gzip compressed data, was "rag_retrieval-0.2.1.tar", last modified: Sun May  5 06:46:22 2024, max compression
```

## Comparing `rag_retrieval-0.2.0.tar` & `rag_retrieval-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 jcli       (501) staff       (20)        0 2024-05-04 09:15:10.563356 rag_retrieval-0.2.0/
--rw-r--r--   0 jcli       (501) staff       (20)     1055 2024-03-20 15:01:37.000000 rag_retrieval-0.2.0/LICENSE
--rw-r--r--   0 jcli       (501) staff       (20)     7263 2024-05-04 09:15:10.563154 rag_retrieval-0.2.0/PKG-INFO
--rw-r--r--   0 jcli       (501) staff       (20)     4829 2024-03-20 15:01:42.000000 rag_retrieval-0.2.0/README.md
--rw-r--r--   0 jcli       (501) staff       (20)     1419 2024-05-04 09:12:44.000000 rag_retrieval-0.2.0/pyproject.toml
-drwxr-xr-x   0 jcli       (501) staff       (20)        0 2024-05-04 09:15:10.558642 rag_retrieval-0.2.0/rag_retrieval/
--rw-r--r--   0 jcli       (501) staff       (20)       89 2024-05-04 09:11:48.000000 rag_retrieval-0.2.0/rag_retrieval/__init__.py
-drwxr-xr-x   0 jcli       (501) staff       (20)        0 2024-05-04 09:15:10.557857 rag_retrieval-0.2.0/rag_retrieval/infer/
-drwxr-xr-x   0 jcli       (501) staff       (20)        0 2024-05-04 09:15:10.561770 rag_retrieval-0.2.0/rag_retrieval/infer/reranker_models/
--rw-r--r--   0 jcli       (501) staff       (20)      720 2024-05-04 08:58:48.000000 rag_retrieval-0.2.0/rag_retrieval/infer/reranker_models/__init__.py
--rw-r--r--   0 jcli       (501) staff       (20)       28 2024-05-04 08:53:27.000000 rag_retrieval-0.2.0/rag_retrieval/infer/reranker_models/colbert_ranker.py
--rw-r--r--   0 jcli       (501) staff       (20)     8726 2024-05-04 08:53:42.000000 rag_retrieval-0.2.0/rag_retrieval/infer/reranker_models/cross_encoder_ranker.py
--rw-r--r--   0 jcli       (501) staff       (20)    14175 2024-05-04 08:53:50.000000 rag_retrieval-0.2.0/rag_retrieval/infer/reranker_models/llm_rankers.py
--rw-r--r--   0 jcli       (501) staff       (20)      639 2024-04-13 14:51:56.000000 rag_retrieval-0.2.0/rag_retrieval/infer/reranker_models/ranker.py
--rw-r--r--   0 jcli       (501) staff       (20)     1482 2024-04-14 16:12:48.000000 rag_retrieval-0.2.0/rag_retrieval/infer/reranker_models/result.py
--rw-r--r--   0 jcli       (501) staff       (20)     1543 2024-04-14 16:43:02.000000 rag_retrieval-0.2.0/rag_retrieval/infer/reranker_models/utils.py
--rw-r--r--   0 jcli       (501) staff       (20)     2978 2024-05-04 08:53:08.000000 rag_retrieval-0.2.0/rag_retrieval/reranker.py
-drwxr-xr-x   0 jcli       (501) staff       (20)        0 2024-05-04 09:15:10.562602 rag_retrieval-0.2.0/rag_retrieval.egg-info/
--rw-r--r--   0 jcli       (501) staff       (20)     7263 2024-05-04 09:15:10.000000 rag_retrieval-0.2.0/rag_retrieval.egg-info/PKG-INFO
--rw-r--r--   0 jcli       (501) staff       (20)      640 2024-05-04 09:15:10.000000 rag_retrieval-0.2.0/rag_retrieval.egg-info/SOURCES.txt
--rw-r--r--   0 jcli       (501) staff       (20)        1 2024-05-04 09:15:10.000000 rag_retrieval-0.2.0/rag_retrieval.egg-info/dependency_links.txt
--rw-r--r--   0 jcli       (501) staff       (20)      114 2024-05-04 09:15:10.000000 rag_retrieval-0.2.0/rag_retrieval.egg-info/requires.txt
--rw-r--r--   0 jcli       (501) staff       (20)       14 2024-05-04 09:15:10.000000 rag_retrieval-0.2.0/rag_retrieval.egg-info/top_level.txt
--rw-r--r--   0 jcli       (501) staff       (20)       38 2024-05-04 09:15:10.563397 rag_retrieval-0.2.0/setup.cfg
-drwxr-xr-x   0 jcli       (501) staff       (20)        0 2024-05-04 09:15:10.562240 rag_retrieval-0.2.0/tests/
--rw-r--r--   0 jcli       (501) staff       (20)       99 2024-04-17 17:10:16.000000 rag_retrieval-0.2.0/tests/test_predict.py
+drwxr-xr-x   0 jcli       (501) staff       (20)        0 2024-05-05 06:46:22.030043 rag_retrieval-0.2.1/
+-rw-r--r--   0 jcli       (501) staff       (20)     1055 2024-03-20 15:01:37.000000 rag_retrieval-0.2.1/LICENSE
+-rw-r--r--   0 jcli       (501) staff       (20)     9665 2024-05-05 06:46:22.029814 rag_retrieval-0.2.1/PKG-INFO
+-rw-r--r--   0 jcli       (501) staff       (20)     9316 2024-05-05 06:44:45.000000 rag_retrieval-0.2.1/README.md
+drwxr-xr-x   0 jcli       (501) staff       (20)        0 2024-05-05 06:46:22.024401 rag_retrieval-0.2.1/examples/
+-rw-r--r--   0 jcli       (501) staff       (20)     7571 2024-05-05 06:28:52.000000 rag_retrieval-0.2.1/examples/Reranker_Tutorial.md
+-rw-r--r--   0 jcli       (501) staff       (20)     1310 2024-05-05 06:46:18.000000 rag_retrieval-0.2.1/pyproject.toml
+drwxr-xr-x   0 jcli       (501) staff       (20)        0 2024-05-05 06:46:22.024810 rag_retrieval-0.2.1/rag_retrieval/
+-rw-r--r--   0 jcli       (501) staff       (20)       68 2024-05-05 05:28:14.000000 rag_retrieval-0.2.1/rag_retrieval/__init__.py
+drwxr-xr-x   0 jcli       (501) staff       (20)        0 2024-05-05 06:46:22.023722 rag_retrieval-0.2.1/rag_retrieval/infer/
+drwxr-xr-x   0 jcli       (501) staff       (20)        0 2024-05-05 06:46:22.028440 rag_retrieval-0.2.1/rag_retrieval/infer/reranker_models/
+-rw-r--r--   0 jcli       (501) staff       (20)      720 2024-05-04 08:58:48.000000 rag_retrieval-0.2.1/rag_retrieval/infer/reranker_models/__init__.py
+-rw-r--r--   0 jcli       (501) staff       (20)       28 2024-05-04 08:53:27.000000 rag_retrieval-0.2.1/rag_retrieval/infer/reranker_models/colbert_ranker.py
+-rw-r--r--   0 jcli       (501) staff       (20)     8726 2024-05-04 08:53:42.000000 rag_retrieval-0.2.1/rag_retrieval/infer/reranker_models/cross_encoder_ranker.py
+-rw-r--r--   0 jcli       (501) staff       (20)    14175 2024-05-04 08:53:50.000000 rag_retrieval-0.2.1/rag_retrieval/infer/reranker_models/llm_rankers.py
+-rw-r--r--   0 jcli       (501) staff       (20)      639 2024-04-13 14:51:56.000000 rag_retrieval-0.2.1/rag_retrieval/infer/reranker_models/ranker.py
+-rw-r--r--   0 jcli       (501) staff       (20)     1482 2024-04-14 16:12:48.000000 rag_retrieval-0.2.1/rag_retrieval/infer/reranker_models/result.py
+-rw-r--r--   0 jcli       (501) staff       (20)     1543 2024-04-14 16:43:02.000000 rag_retrieval-0.2.1/rag_retrieval/infer/reranker_models/utils.py
+-rw-r--r--   0 jcli       (501) staff       (20)     2978 2024-05-04 08:53:08.000000 rag_retrieval-0.2.1/rag_retrieval/reranker.py
+drwxr-xr-x   0 jcli       (501) staff       (20)        0 2024-05-05 06:46:22.029559 rag_retrieval-0.2.1/rag_retrieval.egg-info/
+-rw-r--r--   0 jcli       (501) staff       (20)     9665 2024-05-05 06:46:22.000000 rag_retrieval-0.2.1/rag_retrieval.egg-info/PKG-INFO
+-rw-r--r--   0 jcli       (501) staff       (20)      712 2024-05-05 06:46:22.000000 rag_retrieval-0.2.1/rag_retrieval.egg-info/SOURCES.txt
+-rw-r--r--   0 jcli       (501) staff       (20)        1 2024-05-05 06:46:22.000000 rag_retrieval-0.2.1/rag_retrieval.egg-info/dependency_links.txt
+-rw-r--r--   0 jcli       (501) staff       (20)       33 2024-05-05 06:46:22.000000 rag_retrieval-0.2.1/rag_retrieval.egg-info/requires.txt
+-rw-r--r--   0 jcli       (501) staff       (20)       14 2024-05-05 06:46:22.000000 rag_retrieval-0.2.1/rag_retrieval.egg-info/top_level.txt
+-rw-r--r--   0 jcli       (501) staff       (20)       38 2024-05-05 06:46:22.030083 rag_retrieval-0.2.1/setup.cfg
+drwxr-xr-x   0 jcli       (501) staff       (20)        0 2024-05-05 06:46:22.029156 rag_retrieval-0.2.1/tests/
+-rw-r--r--   0 jcli       (501) staff       (20)      632 2024-05-04 15:18:00.000000 rag_retrieval-0.2.1/tests/test_cross_encoder_reranker.py
+-rw-r--r--   0 jcli       (501) staff       (20)      806 2024-05-04 15:18:35.000000 rag_retrieval-0.2.1/tests/test_llm_reranker.py
```

### Comparing `rag_retrieval-0.2.0/LICENSE` & `rag_retrieval-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rag_retrieval-0.2.0/pyproject.toml` & `rag_retrieval-0.2.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -9,19 +9,19 @@
     "rag_retrieval.infer.reranker_models",
 ]
 
 [project]
 name = "rag_retrieval" 
 
 
-version = "0.2.0"
+version = "0.2.1"
 
-description = "A unified API for various RAG Retrieval  re-ranking models."
+description = "A unified API for various RAG Retrieval  reranker models."
 
-readme = "README.md"
+readme = "examples/Reranker_Tutorial.md"
 
 requires-python = ">=3.8"
 
 license = {file = "LICENSE"}
 
 keywords = ["reranking", "retrieval", "rag", "nlp"]
 
@@ -44,17 +44,13 @@
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: 3 :: Only",
 ]
 
 dependencies = [
   "pydantic",
   "tqdm",
+  "torch",
+  "transformers"
 ]
 
-[project.optional-dependencies]
-all = ["transformers", "torch", "requests"]
-transformers = ["transformers", "torch",]
-api = ["requests"]
-dev = ["pytest"]
-
 [project.urls]
 "Homepage" = "https://github.com/NLPJCL/RAG-Retrieval"
```

### Comparing `rag_retrieval-0.2.0/rag_retrieval/infer/reranker_models/__init__.py` & `rag_retrieval-0.2.1/rag_retrieval/infer/reranker_models/__init__.py`

 * *Files identical despite different names*

### Comparing `rag_retrieval-0.2.0/rag_retrieval/infer/reranker_models/cross_encoder_ranker.py` & `rag_retrieval-0.2.1/rag_retrieval/infer/reranker_models/cross_encoder_ranker.py`

 * *Files identical despite different names*

### Comparing `rag_retrieval-0.2.0/rag_retrieval/infer/reranker_models/llm_rankers.py` & `rag_retrieval-0.2.1/rag_retrieval/infer/reranker_models/llm_rankers.py`

 * *Files identical despite different names*

### Comparing `rag_retrieval-0.2.0/rag_retrieval/infer/reranker_models/ranker.py` & `rag_retrieval-0.2.1/rag_retrieval/infer/reranker_models/ranker.py`

 * *Files identical despite different names*

### Comparing `rag_retrieval-0.2.0/rag_retrieval/infer/reranker_models/result.py` & `rag_retrieval-0.2.1/rag_retrieval/infer/reranker_models/result.py`

 * *Files identical despite different names*

### Comparing `rag_retrieval-0.2.0/rag_retrieval/infer/reranker_models/utils.py` & `rag_retrieval-0.2.1/rag_retrieval/infer/reranker_models/utils.py`

 * *Files identical despite different names*

### Comparing `rag_retrieval-0.2.0/rag_retrieval/reranker.py` & `rag_retrieval-0.2.1/rag_retrieval/reranker.py`

 * *Files identical despite different names*

### Comparing `rag_retrieval-0.2.0/rag_retrieval.egg-info/SOURCES.txt` & `rag_retrieval-0.2.1/rag_retrieval.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 LICENSE
 README.md
 pyproject.toml
+examples/Reranker_Tutorial.md
 rag_retrieval/__init__.py
 rag_retrieval/reranker.py
 rag_retrieval.egg-info/PKG-INFO
 rag_retrieval.egg-info/SOURCES.txt
 rag_retrieval.egg-info/dependency_links.txt
 rag_retrieval.egg-info/requires.txt
 rag_retrieval.egg-info/top_level.txt
 rag_retrieval/infer/reranker_models/__init__.py
 rag_retrieval/infer/reranker_models/colbert_ranker.py
 rag_retrieval/infer/reranker_models/cross_encoder_ranker.py
 rag_retrieval/infer/reranker_models/llm_rankers.py
 rag_retrieval/infer/reranker_models/ranker.py
 rag_retrieval/infer/reranker_models/result.py
 rag_retrieval/infer/reranker_models/utils.py
-tests/test_predict.py
+tests/test_cross_encoder_reranker.py
+tests/test_llm_reranker.py
```

