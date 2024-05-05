# Comparing `tmp/eurelis_langchain_solr_vectorstore-0.0.1.tar.gz` & `tmp/eurelis_langchain_solr_vectorstore-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eurelis_langchain_solr_vectorstore-0.0.1.tar", last modified: Sun Oct 29 16:57:41 2023, max compression
+gzip compressed data, was "eurelis_langchain_solr_vectorstore-0.0.2.tar", last modified: Sun May  5 08:59:19 2024, max compression
```

## Comparing `eurelis_langchain_solr_vectorstore-0.0.1.tar` & `eurelis_langchain_solr_vectorstore-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-10-29 16:57:41.213404 eurelis_langchain_solr_vectorstore-0.0.1/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     1064 2023-10-29 16:18:57.000000 eurelis_langchain_solr_vectorstore-0.0.1/LICENSE
--rw-r--r--   0 vincentlambert   (501) staff       (20)     2953 2023-10-29 16:57:41.212668 eurelis_langchain_solr_vectorstore-0.0.1/PKG-INFO
--rw-r--r--   0 vincentlambert   (501) staff       (20)     2301 2023-10-29 16:14:22.000000 eurelis_langchain_solr_vectorstore-0.0.1/README.md
--rw-r--r--   0 vincentlambert   (501) staff       (20)      791 2023-10-29 16:50:13.000000 eurelis_langchain_solr_vectorstore-0.0.1/pyproject.toml
--rw-r--r--   0 vincentlambert   (501) staff       (20)       38 2023-10-29 16:57:41.213591 eurelis_langchain_solr_vectorstore-0.0.1/setup.cfg
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-10-29 16:57:41.200301 eurelis_langchain_solr_vectorstore-0.0.1/src/
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-10-29 16:57:41.207678 eurelis_langchain_solr_vectorstore-0.0.1/src/eurelis_langchain_solr_vectorstore/
--rw-r--r--   0 vincentlambert   (501) staff       (20)    16085 2023-10-29 16:14:22.000000 eurelis_langchain_solr_vectorstore-0.0.1/src/eurelis_langchain_solr_vectorstore/__init__.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)     9362 2023-10-29 16:14:22.000000 eurelis_langchain_solr_vectorstore-0.0.1/src/eurelis_langchain_solr_vectorstore/solr_core.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)     5079 2023-10-29 16:14:22.000000 eurelis_langchain_solr_vectorstore-0.0.1/src/eurelis_langchain_solr_vectorstore/types.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2023-10-29 16:57:41.211832 eurelis_langchain_solr_vectorstore-0.0.1/src/eurelis_langchain_solr_vectorstore.egg-info/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     2953 2023-10-29 16:57:41.000000 eurelis_langchain_solr_vectorstore-0.0.1/src/eurelis_langchain_solr_vectorstore.egg-info/PKG-INFO
--rw-r--r--   0 vincentlambert   (501) staff       (20)      431 2023-10-29 16:57:41.000000 eurelis_langchain_solr_vectorstore-0.0.1/src/eurelis_langchain_solr_vectorstore.egg-info/SOURCES.txt
--rw-r--r--   0 vincentlambert   (501) staff       (20)        1 2023-10-29 16:57:41.000000 eurelis_langchain_solr_vectorstore-0.0.1/src/eurelis_langchain_solr_vectorstore.egg-info/dependency_links.txt
--rw-r--r--   0 vincentlambert   (501) staff       (20)       35 2023-10-29 16:57:41.000000 eurelis_langchain_solr_vectorstore-0.0.1/src/eurelis_langchain_solr_vectorstore.egg-info/top_level.txt
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-05 08:59:19.977434 eurelis_langchain_solr_vectorstore-0.0.2/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     1064 2023-10-29 17:22:12.000000 eurelis_langchain_solr_vectorstore-0.0.2/LICENSE
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     3403 2024-05-05 08:59:19.976963 eurelis_langchain_solr_vectorstore-0.0.2/PKG-INFO
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     2752 2024-05-05 08:53:51.000000 eurelis_langchain_solr_vectorstore-0.0.2/README.md
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      791 2024-05-05 08:53:51.000000 eurelis_langchain_solr_vectorstore-0.0.2/pyproject.toml
+-rw-r--r--   0 vincentlambert   (501) staff       (20)       38 2024-05-05 08:59:19.977611 eurelis_langchain_solr_vectorstore-0.0.2/setup.cfg
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-05 08:59:19.967993 eurelis_langchain_solr_vectorstore-0.0.2/src/
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-05 08:59:19.973131 eurelis_langchain_solr_vectorstore-0.0.2/src/eurelis_langchain_solr_vectorstore/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)    16382 2024-05-05 08:53:51.000000 eurelis_langchain_solr_vectorstore-0.0.2/src/eurelis_langchain_solr_vectorstore/__init__.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     9877 2024-05-05 08:53:51.000000 eurelis_langchain_solr_vectorstore-0.0.2/src/eurelis_langchain_solr_vectorstore/solr_core.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     5079 2023-10-29 17:22:12.000000 eurelis_langchain_solr_vectorstore-0.0.2/src/eurelis_langchain_solr_vectorstore/types.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-05 08:59:19.976499 eurelis_langchain_solr_vectorstore-0.0.2/src/eurelis_langchain_solr_vectorstore.egg-info/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     3403 2024-05-05 08:59:19.000000 eurelis_langchain_solr_vectorstore-0.0.2/src/eurelis_langchain_solr_vectorstore.egg-info/PKG-INFO
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      431 2024-05-05 08:59:19.000000 eurelis_langchain_solr_vectorstore-0.0.2/src/eurelis_langchain_solr_vectorstore.egg-info/SOURCES.txt
+-rw-r--r--   0 vincentlambert   (501) staff       (20)        1 2024-05-05 08:59:19.000000 eurelis_langchain_solr_vectorstore-0.0.2/src/eurelis_langchain_solr_vectorstore.egg-info/dependency_links.txt
+-rw-r--r--   0 vincentlambert   (501) staff       (20)       35 2024-05-05 08:59:19.000000 eurelis_langchain_solr_vectorstore-0.0.2/src/eurelis_langchain_solr_vectorstore.egg-info/top_level.txt
```

### Comparing `eurelis_langchain_solr_vectorstore-0.0.1/LICENSE` & `eurelis_langchain_solr_vectorstore-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eurelis_langchain_solr_vectorstore-0.0.1/PKG-INFO` & `eurelis_langchain_solr_vectorstore-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,80 +1,94 @@
 Metadata-Version: 2.1
 Name: eurelis_langchain_solr_vectorstore
-Version: 0.0.1
+Version: 0.0.2
 Summary: Library that provide a Solr based vector store for Langchain
-Author-email: Jérôme DIAZ <j.diaz@eurelis.com>, Vincent Lambert <v.lambert@eurelis.com>
+Author-email: Jérôme DIAZ <j.diaz@eurelis.com>, Vincent LAMBERT <v.lambert@eurelis.com>
 Project-URL: Homepage, https://github.com/Eurelis/Eurelis-Langchain-SolR-VectorStore
 Project-URL: Bug Tracker, https://github.com/Eurelis/Eurelis-Langchain-SolR-VectorStore/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Eurelis-Langchain-SolR-VectorStore
 
+![Python : 11](https://img.shields.io/badge/Python-=3.11-green)
+![Code style : black](https://img.shields.io/badge/Code_style-black-black)
+![Linting : pylint](https://img.shields.io/badge/Linting-pylint-yellowgreen)
+
 This library allows to use a Solr based vector store with the python version of [LangChain](https://www.langchain.com)
 
 ## Usage
+
 This library assume you already have a running Solr instance with a configured dense vector field
 
 ```xml
-    <fieldType name="knn_vector" class="solr.DenseVectorField" vectorDimension="768" similarityFunction="euclidean"/>
-    <field name="vector" type="knn_vector" indexed="true" stored="true"/>
+<fieldType name="knn_vector" class="solr.DenseVectorField" vectorDimension="768" similarityFunction="euclidean"/>
+<field name="vector" type="knn_vector" indexed="true" stored="true"/>
 ```
 
 Be sure to set a vectorDimension value corresponding to what yor embeddings model provide.
 
-```
+```python
 from langchain.embeddings import HuggingFaceEmbeddings
 from eurelis_langchain_solr_vectorstore import Solr
 
 embeddings = HuggingFaceEmbeddings()  # you are free to use any embeddings method allowed by langchain
 
 vector_store = Solr(embeddings)  # with default core configuration
 ```
 
 You can also specify data about the solr instance and core to use:
 
 ```python
 vector_store = Solr(embeddings, core_kwargs={
-        'page_content_field': 'text_t',  # field containing the text content
-        'vector_field': 'vector',        # field containing the embeddings of the text content
-        'core_name': 'langchain',        # core name
-        'url_base': 'http://localhost:8983/solr' # base url to access solr
-    })  # with custom default core configuration
+    'page_content_field': 'text_t',  # field containing the text content
+    'vector_field': 'vector',        # field containing the embeddings of the text content
+    'core_name': 'langchain',        # core name
+    'url_base': 'http://localhost:8983/solr', # base url to access solr
+    'query_handler': 'select', # handler to use to query solr
+    'update_handler': 'update' # update handler for solr
+})  # with custom default core configuration
 ```
 
 In the code above you have both the allowed core arguments and the default value.
 
-
 ### Metadata
+
 The Solr based vector store also supports storing and filtering on metadata.
 
 Metadata are mapped into Solr using the following convention: metadata_*{key}*_*{type}* with 
 key being the original metadata key, and type is automatically inferred as:
+
 - *i* for integer fields
 - *d* for float fields
 - *s* for string fields
 - *b* for boolean fields
 
 The *vector_search* method take an optional *where* param expecting a dict:
+
 - dict item key: base name of a metadata field
 - dict item value: value expected in the metadata field
 
 Example using the vector store as a retriever:
 
 ```python
-retriever = solr.as_retriever(search_kwargs: {'language': 'en', year: 2000})
+retriever = vector_store.as_retriever()
 ```
 
+Example adding filter instructions to the retriever
+```python
+retriever = vector_store.as_retriever(search_kwargs={'filter': {'language': 'en', 'year': 2000}})
+```
 
 ## Docker
 
 A docker compose file is present in the etc/docker folder, use it with
-```
+
+```bash
 docker compose up -d
 ```
 
-to launch a solr instance with a core named *langchain* and a 'vector' field with 768 dimensions.
+To launch a solr instance with a core named *langchain* and a 'vector' field with 768 dimensions.
```

### Comparing `eurelis_langchain_solr_vectorstore-0.0.1/pyproject.toml` & `eurelis_langchain_solr_vectorstore-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "eurelis_langchain_solr_vectorstore"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Jérôme DIAZ", email="j.diaz@eurelis.com" },
-  { name="Vincent Lambert", email="v.lambert@eurelis.com" }
+  { name="Vincent LAMBERT", email="v.lambert@eurelis.com" }
 ]
 description = "Library that provide a Solr based vector store for Langchain"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `eurelis_langchain_solr_vectorstore-0.0.1/src/eurelis_langchain_solr_vectorstore/__init__.py` & `eurelis_langchain_solr_vectorstore-0.0.2/src/eurelis_langchain_solr_vectorstore/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,21 @@
 from __future__ import annotations
 
 import logging
 import uuid
-from typing import (
-    Any,
-    Callable,
-    Dict,
-    Iterable,
-    List,
-    Optional,
-    Tuple,
-    Type
-)
+from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Type
 
 import numpy as np
 
 from langchain.docstore.document import Document
 from langchain.schema.embeddings import Embeddings
 from langchain.schema.vectorstore import VectorStore
 from langchain.vectorstores.utils import maximal_marginal_relevance
 
-from .types import _results_to_docs, _results_to_docs_and_scores
+from .types import _results_to_docs, _results_to_docs_and_scores, Metadata
 from .solr_core import SolrCore
 
 logger = logging.getLogger()
 DEFAULT_K = 4  # Number of Documents to return.
 
 
 class Solr(VectorStore):
@@ -40,33 +31,35 @@
         vectorstore = Solr(
             embeddings,
             core_kwargs={
                 'page_content_field': 'text_t', # name of the solr to store the page content in
                 'vector_field: 'vector', # name of the solr field to store the vector in
                 'core_name': 'langchain', # name of the solr core
                 'url_base': 'http://localhost:8983/solr' # base url to access solr
+                'query_handler': 'select' # select handler to query solr
+                'update_handler': 'update' # update handler to query solr
             }
         )
     Args:
-        embeddings:Embeddings instance,
+        embedding_function: Embeddings instance,
         core_kwargs: arguments to construct the solr core handler
     """
 
     def __init__(
         self,
         embedding_function: Embeddings,
         core_kwargs: Optional[Dict] = None,
     ) -> None:
         """Initialize with a Solr client."""
 
         self._embedding_function = embedding_function
 
         core_kwargs = core_kwargs if core_kwargs else {}
 
-        self._core = SolrCore(**core_kwargs) # ToDO configuration
+        self._core = SolrCore(**core_kwargs)
 
     @property
     def embeddings(self) -> Optional[Embeddings]:
         return self._embedding_function
 
     def add_texts(
         self,
@@ -102,15 +95,15 @@
             non_empty_ids = []
             for idx, m in enumerate(metadatas):
                 if m:
                     non_empty_ids.append(idx)
                 else:
                     empty_ids.append(idx)
             if non_empty_ids:
-                metadatas = [metadatas[idx] for idx in non_empty_ids]
+                metadatas: List[Metadata] = [metadatas[idx] for idx in non_empty_ids]
                 texts_with_metadatas = [texts[idx] for idx in non_empty_ids]
                 embeddings_with_metadatas = (
                     [embeddings[idx] for idx in non_empty_ids] if embeddings else None
                 )
                 ids_with_metadata = [ids[idx] for idx in non_empty_ids]
                 try:
                     self._core.upsert(
@@ -348,26 +341,26 @@
         """Update a document in the collection.
 
         Args:
             ids (List[str]): List of ids of the document to update.
             documents (List[Document]): List of documents to update.
         """
         text = [document.page_content for document in documents]
-        metadata = [document.metadata for document in documents]
+        metadata: List[Metadata] = [document.metadata for document in documents]
         if self._embedding_function is None:
             raise ValueError(
                 "For update, you must specify an embedding function on creation."
             )
         embeddings = self._embedding_function.embed_documents(text)
 
         self._core.upsert(
             ids=ids,
             embeddings=embeddings,
-            documents=text,
             metadatas=metadata,
+            documents=text,
         )
 
     @classmethod
     def from_texts(
         cls: Type[Solr],
         texts: List[str],
         embedding: Optional[Embeddings] = None,
@@ -385,17 +378,20 @@
             embedding (Optional[Embeddings]): Embedding function. Defaults to None.
             metadatas (Optional[List[dict]]): List of metadatas. Defaults to None.
             ids (Optional[List[str]]): List of document IDs. Defaults to None.
 
         Returns:
             Solr: Solr vectorstore.
         """
-        solr = cls(
+        core_kwargs = kwargs.get("core_kwargs")
 
-        )
+        if embedding is None:
+            raise ValueError("Embedding function is required.")
+
+        solr = cls(embedding, core_kwargs)
         solr.add_texts(texts=texts, metadatas=metadatas, ids=ids)
         return solr
 
     @classmethod
     def from_documents(
         cls: Type[Solr],
         documents: List[Document],
```

### Comparing `eurelis_langchain_solr_vectorstore-0.0.1/src/eurelis_langchain_solr_vectorstore/solr_core.py` & `eurelis_langchain_solr_vectorstore-0.0.2/src/eurelis_langchain_solr_vectorstore/solr_core.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 import json
 import logging
-from typing import Optional, List, Tuple
+from typing import Optional, List, Tuple, Mapping, Any
 
 import requests
 from langchain.schema import Document
 
-from .types import OneOrMany, ID, IDs, Embedding, Metadata, validate_ids, maybe_cast_one_to_many, validate_embeddings, \
-    validate_metadatas
+from .types import (
+    OneOrMany,
+    ID,
+    IDs,
+    Embedding,
+    Metadata,
+    validate_ids,
+    maybe_cast_one_to_many,
+    validate_embeddings,
+    validate_metadatas,
+)
 
 
 logger = logging.getLogger()
 
 
 class SolrCore:
     """
@@ -21,122 +30,140 @@
     _METADATA_FIELD_PREFIX_LENGTH = len(_METADATA_FIELD_PREFIX)
 
     def __init__(self, **kwargs):
         self._page_content_field = kwargs.get("page_content_field", "text_t")
         self._vector_field = kwargs.get("vector_field", "vector")
         self._core_name = kwargs.get("core_name", "langchain")
         self._url_base = kwargs.get("url_base", "http://localhost:8983/solr")
+        self._query_handler = kwargs.get("query_handler", "select")
+        self._update_handler = kwargs.get("update_handler", "update")
 
     def get_handler_url(self, handler: str):
         return f"{self._url_base}/{self._core_name}/{handler}"
 
     @staticmethod
-    def metadata_to_solr_fields(metadata: dict) -> dict:
-        solr_dict = dict()
+    def metadata_to_solr_fields(
+        metadata: Mapping[str, str | int | float | bool]
+    ) -> dict:
+        solr_dict = {}
         for key, value in metadata.items():
             try:
                 field_name = SolrCore.field_name_for_metadata_key(key, type(value))
                 solr_dict[field_name] = value
             except ValueError as e:
                 continue
 
         return solr_dict
 
     @staticmethod
     def field_name_for_metadata_key(metadata_key: str, type_: type) -> str:
-        negative_field = metadata_key[0] == '-'  # case of empty field search
+        negative_field = metadata_key[0] == "-"  # case of empty field search
         if negative_field:
             metadata_key = metadata_key[1:]
 
         base_name = f"{SolrCore._METADATA_FIELD_PREFIX}{metadata_key}_"
         if type_ is str:
             base_name += "s"
         elif type_ is int:
             base_name += "i"
         elif type_ is float:
             base_name += "d"
         elif type_ is bool:
             base_name += "b"
         else:
-            raise ValueError(f"Invalid type {type_} given, only str, int, boolean and float supported")
+            raise ValueError(
+                f"Invalid type {type_} given, only str, int, boolean and float supported"
+            )
 
         if negative_field:
             return f"-{base_name}"
 
         return base_name
 
     @staticmethod
     def metadata_key_for_field_name(field_name: str) -> Optional[str]:
         if not field_name.startswith(SolrCore._METADATA_FIELD_PREFIX):
             return None
-        work_name = field_name[SolrCore._METADATA_FIELD_PREFIX_LENGTH:]  # remove prefix
+        work_name = field_name[
+            SolrCore._METADATA_FIELD_PREFIX_LENGTH :
+        ]  # remove prefix
 
         underscore_position = work_name.rfind("_")
         underscore_relative_position = len(work_name) - underscore_position
 
         if underscore_relative_position >= 3:
-            raise ValueError(f"Unsupported solr metadata field suffix in field {field_name}")
+            raise ValueError(
+                f"Unsupported solr metadata field suffix in field {field_name}"
+            )
 
         # TODO: do we need to check suffix consistency here?
         return work_name[:underscore_position]
 
-    def vector_search(self, vector: List[float], n_results: int = 4, where: Optional[dict[str, str]] = None) -> list:
-        url = self.get_handler_url("select")
+    def vector_search(
+        self,
+        vector: List[float],
+        n_results: int = 4,
+        where: Optional[dict[str, str]] = None,
+    ) -> Mapping[str, list[Any]]:
+        url = self.get_handler_url(self._query_handler)
 
         query_params = {
-            'q': '{!knn f=' + self._vector_field + ' topK=' + str(n_results) + '}' + str(vector),
-            'fl': '*, score',
-            'output': 'json'
+            "q": "{!knn f="
+            + self._vector_field
+            + " topK="
+            + str(n_results)
+            + "}"
+            + str(vector),
+            "fl": "*, score",
+            "output": "json",
         }
 
         if where:
             fq_values = []
             for field, value in where.items():
                 field_name = SolrCore.field_name_for_metadata_key(field, type(value))
                 if not field_name:
                     continue
                 fq_values.append(f"{field_name}:{value}")
 
-            query_params['fq'] = " AND ".join(fq_values)
+            query_params["fq"] = " AND ".join(fq_values)
 
-        params = {
-            'params': query_params
-        }
+        params = {"params": query_params}
 
         logging.debug(f"Solr search using params {json.dumps(query_params)}")
 
         x = requests.post(url, json=params)
 
         data_json = json.loads(x.text)
 
         results_documents = []
         results_metadatas = []
         results_distances = []
         results_embeddings = []
 
-        for doc in data_json['response']['docs']:
+        for doc in data_json["response"]["docs"]:
             page_content = doc.get(self._page_content_field)
             results_documents.append(page_content)
 
             metadata = {}
             for solr_field, value in doc.items():
                 metadata_key = SolrCore.metadata_key_for_field_name(solr_field)
                 if not metadata_key or not isinstance(value, (str, int, float, bool)):
                     continue
                 metadata[metadata_key] = value
 
             results_metadatas.append(metadata)
-            results_distances.append(doc.get('score', 0))
+            results_distances.append(doc.get("score", 0))
             results_embeddings.append(doc.get(self._vector_field))
 
         results = {
-            'documents': [results_documents],
-            'metadatas': [results_metadatas],
-            'distances': [results_distances],
-            'embeddings': [results_embeddings]
+            "documents": [results_documents],
+            "metadatas": [results_metadatas],
+            "distances": [results_distances],
+            "embeddings": [results_embeddings],
         }
 
         return results
 
     def _validate_embedding_set(
         self,
         ids: OneOrMany[ID],
@@ -200,15 +227,15 @@
         return ids, embeddings, metadatas, documents  # type: ignore
 
     def upsert(
         self,
         ids: OneOrMany[ID],
         embeddings: Optional[OneOrMany[Embedding]] = None,
         metadatas: Optional[OneOrMany[Metadata]] = None,
-        documents: Optional[OneOrMany[Document]] = None,
+        documents: Optional[OneOrMany[str]] = None,
     ) -> None:
         """Update the embeddings, metadatas or documents for provided ids, or create them if they don't exist.
 
         Args:
             ids: The ids of the embeddings to update
             embeddings: The embeddings to add. If None, embeddings will be computed based on the documents using the embedding_function set for the Collection. Optional.
             metadatas:  The metadata to associate with the embeddings. When querying, you can filter on this metadata. Optional.
@@ -219,41 +246,45 @@
         """
 
         ids, embeddings, metadatas, documents = self._validate_embedding_set(
             ids, embeddings, metadatas, documents
         )
 
         solr_docs = []
-        for doc_id, embedding, metadata, document in zip(ids, embeddings, metadatas, documents):
+        for doc_id, embedding, metadata, document in zip(
+            ids, embeddings, metadatas, documents
+        ):
             solr_doc = {
-                'id': doc_id,
+                "id": doc_id,
                 self._vector_field: embedding,
                 self._page_content_field: document,
-                **SolrCore.metadata_to_solr_fields(metadata)
+                **SolrCore.metadata_to_solr_fields(metadata),
             }
 
             solr_docs.append(solr_doc)
 
-        call_url = self.get_handler_url("update/json?commit=true")
+        call_url = self.get_handler_url(f"{self._update_handler}/json?commit=true")
 
         response = requests.post(call_url, json=solr_docs)
         logging.debug(f"Solr update response {response.text}")
 
     def delete(self, ids: OneOrMany[ID]) -> bool:
         ids_to_delete = maybe_cast_one_to_many(ids)
-        json_body = {
-            'delete': ids_to_delete
-        }
-        response = requests.post(self.get_handler_url("update?commit=true"), json=json_body)
+        json_body = {"delete": ids_to_delete}
+        response = requests.post(
+            self.get_handler_url(f"{self._update_handler}?commit=true"), json=json_body
+        )
 
         logging.debug(f"Solr delete response {response.text}")
 
         return response.status_code == 200
 
     def empty(self) -> bool:
-        json_body = {"delete": {"query":"*:*"}}
+        json_body = {"delete": {"query": "*:*"}}
 
-        response = requests.post(self.get_handler_url("update?commit=true"), json=json_body)
+        response = requests.post(
+            self.get_handler_url(f"{self._update_handler}?commit=true"), json=json_body
+        )
 
         logging.debug(f"Solr delete all response {response.text}")
 
         return response.status_code == 200
```

### Comparing `eurelis_langchain_solr_vectorstore-0.0.1/src/eurelis_langchain_solr_vectorstore/types.py` & `eurelis_langchain_solr_vectorstore-0.0.2/src/eurelis_langchain_solr_vectorstore/types.py`

 * *Files identical despite different names*

### Comparing `eurelis_langchain_solr_vectorstore-0.0.1/src/eurelis_langchain_solr_vectorstore.egg-info/PKG-INFO` & `eurelis_langchain_solr_vectorstore-0.0.2/src/eurelis_langchain_solr_vectorstore.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,80 +1,94 @@
 Metadata-Version: 2.1
-Name: eurelis-langchain-solr-vectorstore
-Version: 0.0.1
+Name: eurelis_langchain_solr_vectorstore
+Version: 0.0.2
 Summary: Library that provide a Solr based vector store for Langchain
-Author-email: Jérôme DIAZ <j.diaz@eurelis.com>, Vincent Lambert <v.lambert@eurelis.com>
+Author-email: Jérôme DIAZ <j.diaz@eurelis.com>, Vincent LAMBERT <v.lambert@eurelis.com>
 Project-URL: Homepage, https://github.com/Eurelis/Eurelis-Langchain-SolR-VectorStore
 Project-URL: Bug Tracker, https://github.com/Eurelis/Eurelis-Langchain-SolR-VectorStore/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Eurelis-Langchain-SolR-VectorStore
 
+![Python : 11](https://img.shields.io/badge/Python-=3.11-green)
+![Code style : black](https://img.shields.io/badge/Code_style-black-black)
+![Linting : pylint](https://img.shields.io/badge/Linting-pylint-yellowgreen)
+
 This library allows to use a Solr based vector store with the python version of [LangChain](https://www.langchain.com)
 
 ## Usage
+
 This library assume you already have a running Solr instance with a configured dense vector field
 
 ```xml
-    <fieldType name="knn_vector" class="solr.DenseVectorField" vectorDimension="768" similarityFunction="euclidean"/>
-    <field name="vector" type="knn_vector" indexed="true" stored="true"/>
+<fieldType name="knn_vector" class="solr.DenseVectorField" vectorDimension="768" similarityFunction="euclidean"/>
+<field name="vector" type="knn_vector" indexed="true" stored="true"/>
 ```
 
 Be sure to set a vectorDimension value corresponding to what yor embeddings model provide.
 
-```
+```python
 from langchain.embeddings import HuggingFaceEmbeddings
 from eurelis_langchain_solr_vectorstore import Solr
 
 embeddings = HuggingFaceEmbeddings()  # you are free to use any embeddings method allowed by langchain
 
 vector_store = Solr(embeddings)  # with default core configuration
 ```
 
 You can also specify data about the solr instance and core to use:
 
 ```python
 vector_store = Solr(embeddings, core_kwargs={
-        'page_content_field': 'text_t',  # field containing the text content
-        'vector_field': 'vector',        # field containing the embeddings of the text content
-        'core_name': 'langchain',        # core name
-        'url_base': 'http://localhost:8983/solr' # base url to access solr
-    })  # with custom default core configuration
+    'page_content_field': 'text_t',  # field containing the text content
+    'vector_field': 'vector',        # field containing the embeddings of the text content
+    'core_name': 'langchain',        # core name
+    'url_base': 'http://localhost:8983/solr', # base url to access solr
+    'query_handler': 'select', # handler to use to query solr
+    'update_handler': 'update' # update handler for solr
+})  # with custom default core configuration
 ```
 
 In the code above you have both the allowed core arguments and the default value.
 
-
 ### Metadata
+
 The Solr based vector store also supports storing and filtering on metadata.
 
 Metadata are mapped into Solr using the following convention: metadata_*{key}*_*{type}* with 
 key being the original metadata key, and type is automatically inferred as:
+
 - *i* for integer fields
 - *d* for float fields
 - *s* for string fields
 - *b* for boolean fields
 
 The *vector_search* method take an optional *where* param expecting a dict:
+
 - dict item key: base name of a metadata field
 - dict item value: value expected in the metadata field
 
 Example using the vector store as a retriever:
 
 ```python
-retriever = solr.as_retriever(search_kwargs: {'language': 'en', year: 2000})
+retriever = vector_store.as_retriever()
 ```
 
+Example adding filter instructions to the retriever
+```python
+retriever = vector_store.as_retriever(search_kwargs={'filter': {'language': 'en', 'year': 2000}})
+```
 
 ## Docker
 
 A docker compose file is present in the etc/docker folder, use it with
-```
+
+```bash
 docker compose up -d
 ```
 
-to launch a solr instance with a core named *langchain* and a 'vector' field with 768 dimensions.
+To launch a solr instance with a core named *langchain* and a 'vector' field with 768 dimensions.
```

