# Comparing `tmp/retriever_search-0.1.0.tar.gz` & `tmp/retriever_search-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retriever_search-0.1.0.tar", last modified: Tue Apr 30 17:19:15 2024, max compression
+gzip compressed data, was "retriever_search-0.2.0.tar", last modified: Sun May  5 16:23:08 2024, max compression
```

## Comparing `retriever_search-0.1.0.tar` & `retriever_search-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-30 17:19:15.379568 retriever_search-0.1.0/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1062 2024-04-23 05:51:14.000000 retriever_search-0.1.0/LICENSE
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1990 2024-04-30 17:19:15.378882 retriever_search-0.1.0/PKG-INFO
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1355 2024-04-30 05:46:26.000000 retriever_search-0.1.0/README.md
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-30 17:19:15.376067 retriever_search-0.1.0/retriever_search/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     6508 2024-04-30 16:55:53.000000 retriever_search-0.1.0/retriever_search/DocumentIngestion.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1922 2024-04-24 08:53:52.000000 retriever_search-0.1.0/retriever_search/QueryPipeline.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)       85 2024-04-30 17:18:46.000000 retriever_search-0.1.0/retriever_search/__init__.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     3617 2024-04-24 08:53:52.000000 retriever_search-0.1.0/retriever_search/frontend_app.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1509 2024-04-30 05:38:18.000000 retriever_search-0.1.0/retriever_search/search_app.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     3458 2024-04-30 17:09:10.000000 retriever_search-0.1.0/retriever_search/search_server.py
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-30 17:19:15.378047 retriever_search-0.1.0/retriever_search.egg-info/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1990 2024-04-30 17:19:15.000000 retriever_search-0.1.0/retriever_search.egg-info/PKG-INFO
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      424 2024-04-30 17:19:15.000000 retriever_search-0.1.0/retriever_search.egg-info/SOURCES.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)        1 2024-04-30 17:19:15.000000 retriever_search-0.1.0/retriever_search.egg-info/dependency_links.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      191 2024-04-30 17:19:15.000000 retriever_search-0.1.0/retriever_search.egg-info/requires.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)       17 2024-04-30 17:19:15.000000 retriever_search-0.1.0/retriever_search.egg-info/top_level.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)       38 2024-04-30 17:19:15.379670 retriever_search-0.1.0/setup.cfg
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      834 2024-04-30 04:41:43.000000 retriever_search-0.1.0/setup.py
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-05 16:23:08.797545 retriever_search-0.2.0/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1062 2024-04-23 05:51:14.000000 retriever_search-0.2.0/LICENSE
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     2293 2024-05-05 16:23:08.796574 retriever_search-0.2.0/PKG-INFO
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1512 2024-05-02 20:10:32.000000 retriever_search-0.2.0/README.md
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-05 16:23:08.783742 retriever_search-0.2.0/retriever_search/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     6508 2024-04-30 16:55:53.000000 retriever_search-0.2.0/retriever_search/DocumentIngestion.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1922 2024-04-24 08:53:52.000000 retriever_search-0.2.0/retriever_search/QueryPipeline.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      259 2024-05-02 18:52:21.000000 retriever_search-0.2.0/retriever_search/Utils.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)       85 2024-05-05 16:22:58.000000 retriever_search-0.2.0/retriever_search/__init__.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     9558 2024-05-02 18:56:07.000000 retriever_search-0.2.0/retriever_search/callbacks.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     3597 2024-05-02 19:19:42.000000 retriever_search-0.2.0/retriever_search/frontend_app.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     2615 2024-05-02 18:56:07.000000 retriever_search-0.2.0/retriever_search/layout.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1597 2024-05-02 18:49:21.000000 retriever_search-0.2.0/retriever_search/search_app.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     3458 2024-04-30 17:09:10.000000 retriever_search-0.2.0/retriever_search/search_server.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      935 2024-05-02 19:58:24.000000 retriever_search-0.2.0/retriever_search/viz_server.py
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-05 16:23:08.795175 retriever_search-0.2.0/retriever_search.egg-info/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     2293 2024-05-05 16:23:08.000000 retriever_search-0.2.0/retriever_search.egg-info/PKG-INFO
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      538 2024-05-05 16:23:08.000000 retriever_search-0.2.0/retriever_search.egg-info/SOURCES.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)        1 2024-05-05 16:23:08.000000 retriever_search-0.2.0/retriever_search.egg-info/dependency_links.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      262 2024-05-05 16:23:08.000000 retriever_search-0.2.0/retriever_search.egg-info/requires.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)       17 2024-05-05 16:23:08.000000 retriever_search-0.2.0/retriever_search.egg-info/top_level.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)       38 2024-05-05 16:23:08.797803 retriever_search-0.2.0/setup.cfg
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      961 2024-05-02 20:12:06.000000 retriever_search-0.2.0/setup.py
```

### Comparing `retriever_search-0.1.0/LICENSE` & `retriever_search-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `retriever_search-0.1.0/PKG-INFO` & `retriever_search-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 Metadata-Version: 2.1
 Name: retriever_search
-Version: 0.1.0
+Version: 0.2.0
 Summary: Local retriever search for your use
 Home-page: https://github.com/GovML/retriever.git
 Author: Sidharth Kathpal
 Author-email: kathpal.sid@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: haystack-ai==2.0.0
 Requires-Dist: pymupdf==1.22.5
 Requires-Dist: sentence-transformers==2.5.1
 Requires-Dist: umap==0.1.1
 Requires-Dist: umap-learn==0.5.5
 Requires-Dist: qdrant-haystack==3.0.0
-Requires-Dist: Flask==3.0.2
+Requires-Dist: Flask==2.2.5
 Requires-Dist: pandas==2.2.1
 Requires-Dist: torch==2.2.1
 Requires-Dist: accelerate==0.27.2
 Requires-Dist: gradio==4.21.0
+Requires-Dist: dash==2.15.0
+Requires-Dist: plotly==5.10.0
+Requires-Dist: wordcloud==1.9.2
+Requires-Dist: pyLDAvis==3.4.1
+Requires-Dist: nltk==3.7
 
 <div align="center">
 
 # Retriever
 
 ### To setup your own local search you can now use this repo.
 
@@ -59,11 +64,21 @@
 ```bash
 >>> from retriever_search import search_server
 >>> from retriever_search import frontend_app as fp
 >>> fp.run_frontend()
 >>> search_server.run_search_server('path_to_folder', 'save_json_path', device='cpu')
 ```
 
+## Vizualisation run
+
+Currently run from the git repo
+
+```bash
+$ cd retriever
+>>> from retriever_search import viz_server as vs
+>>> vs.run_viz_server()
+```
+
 ## Where to access the frontend 
 
 Access via the following URL - http://127.0.0.1:7860 
 This URL would work for your local setup only
```

### Comparing `retriever_search-0.1.0/README.md` & `retriever_search-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -38,11 +38,21 @@
 ```bash
 >>> from retriever_search import search_server
 >>> from retriever_search import frontend_app as fp
 >>> fp.run_frontend()
 >>> search_server.run_search_server('path_to_folder', 'save_json_path', device='cpu')
 ```
 
+## Vizualisation run
+
+Currently run from the git repo
+
+```bash
+$ cd retriever
+>>> from retriever_search import viz_server as vs
+>>> vs.run_viz_server()
+```
+
 ## Where to access the frontend 
 
 Access via the following URL - http://127.0.0.1:7860 
 This URL would work for your local setup only
```

### Comparing `retriever_search-0.1.0/retriever_search/DocumentIngestion.py` & `retriever_search-0.2.0/retriever_search/DocumentIngestion.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.1.0/retriever_search/QueryPipeline.py` & `retriever_search-0.2.0/retriever_search/QueryPipeline.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.1.0/retriever_search/frontend_app.py` & `retriever_search-0.2.0/retriever_search/frontend_app.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,9 +82,9 @@
                     html = ("<iframe id=\"iframeid\" src=" + src_val + "\ width=1200 height=2000>")
                     out1 = gr.HTML(html)
 
 
         demo.launch(share=True) 
 
 def run_frontend():
-    gradio_obj = gradio_app("http://127.0.0.1:5000", "https://divine-mildly-emu.ngrok-free.app/")
+    gradio_obj = gradio_app("http://127.0.0.1:5000", "http://127.0.0.1:8055")
     gradio_obj.gradio_launch()
```

### Comparing `retriever_search-0.1.0/retriever_search/search_app.py` & `retriever_search-0.2.0/retriever_search/search_app.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,36 +2,37 @@
 import os
 from retriever_search.DocumentIngestion import DocumentIngestion
 from retriever_search.QueryPipeline import QueryPipeline
 from haystack_integrations.document_stores.qdrant import QdrantDocumentStore
 
 
 class search_app:
-    def __init__(self, inputDirectory, json_save_path, embedding_2d = "red_emb_1K.npy", device = 'cpu'):
+    def __init__(self, inputDirectory, json_save_path, embedding_2d = "red_emb_1K.npy", device = 'cpu', model = 'sentence-transformers/allenai-specter'):
         self.embedding_2d = embedding_2d
         self.json_path = json_save_path
         self.inputDirectory = inputDirectory
         self.device = device
+        self.model = model
 
     def new_search_run(self):
         #model = 'sentence-transformers/all-mpnet-base-v2'
-        model = 'sentence-transformers/allenai-specter'
+        #model = 'sentence-transformers/allenai-specter'
         #model = 'Dagar/t5-small-science-papers'
         if os.path.exists(self.json_path):
             ingestion = DocumentIngestion(self.json_path, model = None, device=self.device)
         else:
-            ingestion = DocumentIngestion(self.inputDirectory, model = model, device=self.device)
+            ingestion = DocumentIngestion(self.inputDirectory, model = self.model, device=self.device)
             ingestion.to_json(self.json_path)
 
         document_store = document_store = QdrantDocumentStore(
             ":memory:",
             embedding_dim=768,  # the embedding_dim should match that of the embedding model
         )
 
         document_store.write_documents(ingestion.documents)
 
         pipe = QueryPipeline(document_store, 
                             type = 'Search', 
-                            ann_model=model, 
+                            ann_model=self.model, 
                             ranker_model="cross-encoder/ms-marco-MiniLM-L-12-v2"
                             )
-        return pipe
+        return pipe
```

### Comparing `retriever_search-0.1.0/retriever_search/search_server.py` & `retriever_search-0.2.0/retriever_search/search_server.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.1.0/retriever_search.egg-info/PKG-INFO` & `retriever_search-0.2.0/retriever_search.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 Metadata-Version: 2.1
 Name: retriever_search
-Version: 0.1.0
+Version: 0.2.0
 Summary: Local retriever search for your use
 Home-page: https://github.com/GovML/retriever.git
 Author: Sidharth Kathpal
 Author-email: kathpal.sid@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: haystack-ai==2.0.0
 Requires-Dist: pymupdf==1.22.5
 Requires-Dist: sentence-transformers==2.5.1
 Requires-Dist: umap==0.1.1
 Requires-Dist: umap-learn==0.5.5
 Requires-Dist: qdrant-haystack==3.0.0
-Requires-Dist: Flask==3.0.2
+Requires-Dist: Flask==2.2.5
 Requires-Dist: pandas==2.2.1
 Requires-Dist: torch==2.2.1
 Requires-Dist: accelerate==0.27.2
 Requires-Dist: gradio==4.21.0
+Requires-Dist: dash==2.15.0
+Requires-Dist: plotly==5.10.0
+Requires-Dist: wordcloud==1.9.2
+Requires-Dist: pyLDAvis==3.4.1
+Requires-Dist: nltk==3.7
 
 <div align="center">
 
 # Retriever
 
 ### To setup your own local search you can now use this repo.
 
@@ -59,11 +64,21 @@
 ```bash
 >>> from retriever_search import search_server
 >>> from retriever_search import frontend_app as fp
 >>> fp.run_frontend()
 >>> search_server.run_search_server('path_to_folder', 'save_json_path', device='cpu')
 ```
 
+## Vizualisation run
+
+Currently run from the git repo
+
+```bash
+$ cd retriever
+>>> from retriever_search import viz_server as vs
+>>> vs.run_viz_server()
+```
+
 ## Where to access the frontend 
 
 Access via the following URL - http://127.0.0.1:7860 
 This URL would work for your local setup only
```

### Comparing `retriever_search-0.1.0/setup.py` & `retriever_search-0.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,15 +16,20 @@
     install_requires=[
         'haystack-ai==2.0.0',
         'pymupdf==1.22.5',
         'sentence-transformers==2.5.1',
         'umap==0.1.1',
         'umap-learn==0.5.5',
         'qdrant-haystack==3.0.0',
-        'Flask==3.0.2',
+        'Flask==2.2.5',
         'pandas==2.2.1',
         'torch==2.2.1',
         'accelerate==0.27.2',
-        'gradio==4.21.0'
+        'gradio==4.21.0',
+        'dash==2.15.0',
+        'plotly==5.10.0',
+        'wordcloud==1.9.2',
+        'pyLDAvis==3.4.1',
+        'nltk==3.7',
     ],
     packages=find_packages(),
 )
```

