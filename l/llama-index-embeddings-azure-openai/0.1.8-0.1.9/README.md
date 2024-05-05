# Comparing `tmp/llama_index_embeddings_azure_openai-0.1.8.tar.gz` & `tmp/llama_index_embeddings_azure_openai-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_embeddings_azure_openai-0.1.8.tar", max compression
+gzip compressed data, was "llama_index_embeddings_azure_openai-0.1.9.tar", max compression
```

## Comparing `llama_index_embeddings_azure_openai-0.1.8.tar` & `llama_index_embeddings_azure_openai-0.1.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       50 2024-04-26 03:45:06.056108 llama_index_embeddings_azure_openai-0.1.8/README.md
--rw-r--r--   0        0        0      193 2024-04-26 03:45:06.056108 llama_index_embeddings_azure_openai-0.1.8/llama_index/embeddings/azure_openai/__init__.py
--rw-r--r--   0        0        0     4792 2024-04-26 03:45:06.056108 llama_index_embeddings_azure_openai-0.1.8/llama_index/embeddings/azure_openai/base.py
--rw-r--r--   0        0        0     1560 2024-04-26 03:45:06.056108 llama_index_embeddings_azure_openai-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      752 1970-01-01 00:00:00.000000 llama_index_embeddings_azure_openai-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       50 2024-05-05 13:46:03.946164 llama_index_embeddings_azure_openai-0.1.9/README.md
+-rw-r--r--   0        0        0      193 2024-05-05 13:46:03.946164 llama_index_embeddings_azure_openai-0.1.9/llama_index/embeddings/azure_openai/__init__.py
+-rw-r--r--   0        0        0     4887 2024-05-05 13:46:03.946164 llama_index_embeddings_azure_openai-0.1.9/llama_index/embeddings/azure_openai/base.py
+-rw-r--r--   0        0        0     1560 2024-05-05 13:46:03.946164 llama_index_embeddings_azure_openai-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      752 1970-01-01 00:00:00.000000 llama_index_embeddings_azure_openai-0.1.9/PKG-INFO
```

### Comparing `llama_index_embeddings_azure_openai-0.1.8/llama_index/embeddings/azure_openai/base.py` & `llama_index_embeddings_azure_openai-0.1.9/llama_index/embeddings/azure_openai/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,28 +42,30 @@
         embed_batch_size: int = DEFAULT_EMBED_BATCH_SIZE,
         additional_kwargs: Optional[Dict[str, Any]] = None,
         api_key: Optional[str] = None,
         api_version: Optional[str] = None,
         # azure specific
         azure_endpoint: Optional[str] = None,
         azure_deployment: Optional[str] = None,
-        azure_ad_token_provider: AzureADTokenProvider = None,
+        azure_ad_token_provider: Optional[AzureADTokenProvider] = None,
         deployment_name: Optional[str] = None,
         max_retries: int = 10,
         reuse_client: bool = True,
         callback_manager: Optional[CallbackManager] = None,
         num_workers: Optional[int] = None,
         # custom httpx client
         http_client: Optional[httpx.Client] = None,
         **kwargs: Any,
     ):
         azure_endpoint = get_from_param_or_env(
             "azure_endpoint", azure_endpoint, "AZURE_OPENAI_ENDPOINT", ""
         )
 
+        api_key = get_from_param_or_env("api_key", api_key, "AZURE_OPENAI_API_KEY")
+
         azure_deployment = resolve_from_aliases(
             azure_deployment,
             deployment_name,
         )
 
         super().__init__(
             mode=mode,
```

### Comparing `llama_index_embeddings_azure_openai-0.1.8/pyproject.toml` & `llama_index_embeddings_azure_openai-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index embeddings azure openai integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-embeddings-azure-openai"
 readme = "README.md"
-version = "0.1.8"
+version = "0.1.9"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.11.post1"
 llama-index-llms-azure-openai = "^0.1.3"
 llama-index-embeddings-openai = "^0.1.3"
```

### Comparing `llama_index_embeddings_azure_openai-0.1.8/PKG-INFO` & `llama_index_embeddings_azure_openai-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-embeddings-azure-openai
-Version: 0.1.8
+Version: 0.1.9
 Summary: llama-index embeddings azure openai integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

