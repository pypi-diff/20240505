# Comparing `tmp/llama_index_llms_azure_openai-0.1.6.tar.gz` & `tmp/llama_index_llms_azure_openai-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_azure_openai-0.1.6.tar", max compression
+gzip compressed data, was "llama_index_llms_azure_openai-0.1.7.tar", max compression
```

## Comparing `llama_index_llms_azure_openai-0.1.6.tar` & `llama_index_llms_azure_openai-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       44 2024-04-15 18:30:41.291504 llama_index_llms_azure_openai-0.1.6/README.md
--rw-r--r--   0        0        0      177 2024-04-15 18:30:41.291504 llama_index_llms_azure_openai-0.1.6/llama_index/llms/azure_openai/__init__.py
--rw-r--r--   0        0        0     8031 2024-04-15 18:30:41.291504 llama_index_llms_azure_openai-0.1.6/llama_index/llms/azure_openai/base.py
--rw-r--r--   0        0        0     1245 2024-04-15 18:30:41.291504 llama_index_llms_azure_openai-0.1.6/llama_index/llms/azure_openai/utils.py
--rw-r--r--   0        0        0     1590 2024-04-15 18:30:41.291504 llama_index_llms_azure_openai-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 llama_index_llms_azure_openai-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       44 2024-05-05 13:46:03.974164 llama_index_llms_azure_openai-0.1.7/README.md
+-rw-r--r--   0        0        0      177 2024-05-05 13:46:03.974164 llama_index_llms_azure_openai-0.1.7/llama_index/llms/azure_openai/__init__.py
+-rw-r--r--   0        0        0     8395 2024-05-05 13:46:03.974164 llama_index_llms_azure_openai-0.1.7/llama_index/llms/azure_openai/base.py
+-rw-r--r--   0        0        0     1245 2024-05-05 13:46:03.974164 llama_index_llms_azure_openai-0.1.7/llama_index/llms/azure_openai/utils.py
+-rw-r--r--   0        0        0     1590 2024-05-05 13:46:03.974164 llama_index_llms_azure_openai-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 llama_index_llms_azure_openai-0.1.7/PKG-INFO
```

### Comparing `llama_index_llms_azure_openai-0.1.6/llama_index/llms/azure_openai/base.py` & `llama_index_llms_azure_openai-0.1.7/llama_index/llms/azure_openai/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         timeout: float = 60.0,
         reuse_client: bool = True,
         api_key: Optional[str] = None,
         api_version: Optional[str] = None,
         # azure specific
         azure_endpoint: Optional[str] = None,
         azure_deployment: Optional[str] = None,
-        azure_ad_token_provider: AzureADTokenProvider = None,
+        azure_ad_token_provider: Optional[AzureADTokenProvider] = None,
         use_azure_ad: bool = False,
         callback_manager: Optional[CallbackManager] = None,
         # aliases for engine
         deployment_name: Optional[str] = None,
         deployment_id: Optional[str] = None,
         deployment: Optional[str] = None,
         # custom httpx client
@@ -182,14 +182,24 @@
             )
         return self._aclient
 
     def _get_credential_kwargs(self, **kwargs: Any) -> Dict[str, Any]:
         if self.use_azure_ad:
             self._azure_ad_token = refresh_openai_azuread_token(self._azure_ad_token)
             self.api_key = self._azure_ad_token.token
+        else:
+            import os
+
+            self.api_key = self.api_key or os.getenv("AZURE_OPENAI_API_KEY")
+
+        if self.api_key is None:
+            raise ValueError(
+                "You must set an `api_key` parameter. "
+                "Alternatively, you can set the AZURE_OPENAI_API_KEY env var OR set `use_azure_ad=True`."
+            )
 
         return {
             "api_key": self.api_key,
             "max_retries": self.max_retries,
             "timeout": self.timeout,
             "azure_endpoint": self.azure_endpoint,
             "azure_deployment": self.azure_deployment,
```

### Comparing `llama_index_llms_azure_openai-0.1.6/llama_index/llms/azure_openai/utils.py` & `llama_index_llms_azure_openai-0.1.7/llama_index/llms/azure_openai/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_llms_azure_openai-0.1.6/pyproject.toml` & `llama_index_llms_azure_openai-0.1.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms azure openai integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-azure-openai"
 readme = "README.md"
-version = "0.1.6"
+version = "0.1.7"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.11.post1"
 llama-index-llms-openai = "^0.1.1"
 azure-identity = "^1.15.0"
 httpx = "*"
```

### Comparing `llama_index_llms_azure_openai-0.1.6/PKG-INFO` & `llama_index_llms_azure_openai-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-azure-openai
-Version: 0.1.6
+Version: 0.1.7
 Summary: llama-index llms azure openai integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

