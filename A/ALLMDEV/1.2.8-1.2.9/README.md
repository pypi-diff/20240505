# Comparing `tmp/ALLMDEV-1.2.8-py3-none-any.whl.zip` & `tmp/ALLMDEV-1.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,23 @@
-Zip file size: 15952 bytes, number of entries: 18
+Zip file size: 20556 bytes, number of entries: 21
 -rw-rw-rw-  2.0 fat       39 b- defN 24-Apr-17 06:01 ALLMDEV/__init__.py
--rw-rw-rw-  2.0 fat     3096 b- defN 24-Apr-27 08:57 ALLMDEV/agent_rag.py
--rw-rw-rw-  2.0 fat     3440 b- defN 24-Apr-27 08:48 ALLMDEV/agent_ragrun.py
--rw-rw-rw-  2.0 fat      757 b- defN 24-Apr-17 06:35 ALLMDEV/cli.py
--rw-rw-rw-  2.0 fat      981 b- defN 24-May-03 13:33 ALLMDEV/cloud.py
--rw-rw-rw-  2.0 fat     1851 b- defN 24-May-03 13:51 ALLMDEV/cloudrag.py
+-rw-rw-rw-  2.0 fat     3706 b- defN 24-May-04 14:17 ALLMDEV/agentapi.py
+-rw-rw-rw-  2.0 fat     3440 b- defN 24-Apr-27 08:48 ALLMDEV/agentchat.py
+-rw-rw-rw-  2.0 fat     4454 b- defN 24-May-04 14:17 ALLMDEV/azureagentapi.py
+-rw-rw-rw-  2.0 fat     3556 b- defN 24-May-05 07:36 ALLMDEV/azureagentchat.py
+-rw-rw-rw-  2.0 fat     1294 b- defN 24-May-05 07:01 ALLMDEV/azurecli.py
+-rw-rw-rw-  2.0 fat      757 b- defN 24-May-04 08:56 ALLMDEV/cli.py
 -rw-rw-rw-  2.0 fat     1945 b- defN 24-Apr-26 04:23 ALLMDEV/fasty.py
--rw-rw-rw-  2.0 fat     2579 b- defN 24-Apr-20 10:27 ALLMDEV/generate.py
--rw-rw-rw-  2.0 fat    10334 b- defN 24-Apr-19 14:10 ALLMDEV/instruct.py
--rw-rw-rw-  2.0 fat     1985 b- defN 24-Apr-25 11:09 ALLMDEV/rag.py
--rw-rw-rw-  2.0 fat     3016 b- defN 24-Apr-25 07:21 ALLMDEV/ragrun.py
--rw-rw-rw-  2.0 fat     3490 b- defN 24-Apr-27 09:53 ALLMDEV/ragserve.py
--rw-rw-rw-  2.0 fat      683 b- defN 24-May-03 07:37 ALLMDEV/test.py
--rw-rw-rw-  2.0 fat     3925 b- defN 24-May-03 14:02 ALLMDEV-1.2.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-03 14:02 ALLMDEV-1.2.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      273 b- defN 24-May-03 14:02 ALLMDEV-1.2.8.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        8 b- defN 24-May-03 14:02 ALLMDEV-1.2.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1360 b- defN 24-May-03 14:02 ALLMDEV-1.2.8.dist-info/RECORD
-18 files, 39854 bytes uncompressed, 13766 bytes compressed:  65.5%
+-rw-rw-rw-  2.0 fat    10334 b- defN 24-May-04 13:49 ALLMDEV/instruct.py
+-rw-rw-rw-  2.0 fat     3096 b- defN 24-Apr-27 08:57 ALLMDEV/newagent.py
+-rw-rw-rw-  2.0 fat     2795 b- defN 24-May-04 14:18 ALLMDEV/serve.py
+-rw-rw-rw-  2.0 fat      683 b- defN 24-May-04 14:32 ALLMDEV/test.py
+-rw-rw-rw-  2.0 fat     3096 b- defN 24-May-05 07:54 ALLMDEV/updateagent.py
+-rw-rw-rw-  2.0 fat     3883 b- defN 24-May-04 14:17 ALLMDEV/vertexagentapi.py
+-rw-rw-rw-  2.0 fat     1851 b- defN 24-May-04 14:57 ALLMDEV/vertexagentchat.py
+-rw-rw-rw-  2.0 fat     1095 b- defN 24-May-04 13:50 ALLMDEV/vertexcli.py
+-rw-rw-rw-  2.0 fat     4588 b- defN 24-May-05 07:57 ALLMDEV-1.2.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-05 07:57 ALLMDEV-1.2.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      522 b- defN 24-May-05 07:57 ALLMDEV-1.2.9.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        8 b- defN 24-May-05 07:57 ALLMDEV-1.2.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1620 b- defN 24-May-05 07:57 ALLMDEV-1.2.9.dist-info/RECORD
+21 files, 52854 bytes uncompressed, 17966 bytes compressed:  66.0%
```

## zipnote {}

```diff
@@ -1,55 +1,64 @@
 Filename: ALLMDEV/__init__.py
 Comment: 
 
-Filename: ALLMDEV/agent_rag.py
+Filename: ALLMDEV/agentapi.py
 Comment: 
 
-Filename: ALLMDEV/agent_ragrun.py
+Filename: ALLMDEV/agentchat.py
 Comment: 
 
-Filename: ALLMDEV/cli.py
+Filename: ALLMDEV/azureagentapi.py
 Comment: 
 
-Filename: ALLMDEV/cloud.py
+Filename: ALLMDEV/azureagentchat.py
 Comment: 
 
-Filename: ALLMDEV/cloudrag.py
+Filename: ALLMDEV/azurecli.py
 Comment: 
 
-Filename: ALLMDEV/fasty.py
+Filename: ALLMDEV/cli.py
 Comment: 
 
-Filename: ALLMDEV/generate.py
+Filename: ALLMDEV/fasty.py
 Comment: 
 
 Filename: ALLMDEV/instruct.py
 Comment: 
 
-Filename: ALLMDEV/rag.py
+Filename: ALLMDEV/newagent.py
 Comment: 
 
-Filename: ALLMDEV/ragrun.py
+Filename: ALLMDEV/serve.py
 Comment: 
 
-Filename: ALLMDEV/ragserve.py
+Filename: ALLMDEV/test.py
 Comment: 
 
-Filename: ALLMDEV/test.py
+Filename: ALLMDEV/updateagent.py
+Comment: 
+
+Filename: ALLMDEV/vertexagentapi.py
+Comment: 
+
+Filename: ALLMDEV/vertexagentchat.py
+Comment: 
+
+Filename: ALLMDEV/vertexcli.py
 Comment: 
 
-Filename: ALLMDEV-1.2.8.dist-info/METADATA
+Filename: ALLMDEV-1.2.9.dist-info/METADATA
 Comment: 
 
-Filename: ALLMDEV-1.2.8.dist-info/WHEEL
+Filename: ALLMDEV-1.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: ALLMDEV-1.2.8.dist-info/entry_points.txt
+Filename: ALLMDEV-1.2.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: ALLMDEV-1.2.8.dist-info/top_level.txt
+Filename: ALLMDEV-1.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: ALLMDEV-1.2.8.dist-info/RECORD
+Filename: ALLMDEV-1.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ALLMDEV/agent_rag.py` & `ALLMDEV/newagent.py`

 * *Files identical despite different names*

## Comparing `ALLMDEV/agent_ragrun.py` & `ALLMDEV/agentchat.py`

 * *Files identical despite different names*

## Comparing `ALLMDEV/cloud.py` & `ALLMDEV/vertexcli.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 
 
 
 def main():
     parser = argparse.ArgumentParser()
     # parser.add_argument("--model", type=str, default="Mistral", help="Name of the model or path to the model file")
     parser.add_argument("--projectid", type=str, default=None, help="Id of your GCP project.")
-    parser.add_argument("--region", type=str, default=0.5, help="Your cloud provider region.")
+    parser.add_argument("--region", type=str, default=None, help="Your cloud provider region.")
+    parser.add_argument("--model", type=str, default='gemini-1.0-pro-002', help="Your cloud model deployed on VertexAI.")
     args = parser.parse_args()
     # Initialize Vertex AI
     vertexai.init(project=args.projectid, location=args.region)
     # Load the model
-    multimodal_model = GenerativeModel(model_name="gemini-1.0-pro-002")
+    multimodal_model = GenerativeModel(model_name=args.model)
 
     infer(multimodal_model)
 
 if __name__=='__main__':
      main()
```

## Comparing `ALLMDEV/cloudrag.py` & `ALLMDEV/vertexagentchat.py`

 * *Files identical despite different names*

## Comparing `ALLMDEV/generate.py` & `ALLMDEV/serve.py`

 * *Files 7% similar despite different names*

```diff
@@ -64,15 +64,16 @@
 
     response_iter = llm.stream_complete(prompt)
     response_text = ''.join(response.delta for response in response_iter)
 
     return jsonify({"response": response_text})
 
 def main():
-        print(f"Inference is working on http://{host}:{port}/v1/chat/completions. You can configure custom host IP and port, and ssl certificate via the apiconfig.txt file available at {config_file_path}")
         if cert_file is not "" and cert_key is not "":
-            app.run(host=host, port=port, debug=False, ssl_context=[cert_file,cert_key])
+            print(f"Inference is working on https://{host}:{port}/v1/chat/completions. You can configure custom host IP and port, and ssl certificate via the apiconfig.txt file available at {config_file_path}")
+            app.run(host=host, port=port, debug=False, ssl_context=(cert_file,cert_key))
         else:
+            print(f"Inference is working on http://{host}:{port}/v1/chat/completions. You can configure custom host IP and port, and ssl certificate via the apiconfig.txt file available at {config_file_path}")
             app.run(host=host, port=port, debug=False)
 
 if __name__ == "__main__":
     main()
```

## Comparing `ALLMDEV/ragserve.py` & `ALLMDEV/agentapi.py`

 * *Files 7% similar despite different names*

```diff
@@ -83,15 +83,16 @@
 def main():
         global persist_directory
         parser = argparse.ArgumentParser()
         parser.add_argument("--agent", type=str, help="Name of the agent to query.")
         args = parser.parse_args()
         agentname=args.agent
         persist_directory = os.path.join('db', agentname)
-        print(f"Inference is working on http://{host}:{port}/v1/chat/completions. You can configure custom host IP and port, and ssl certificate via the apiconfig.txt file available at {config_file_path}")
         if cert_file is not "" and cert_key is not "":
-            app.run(host=host, port=port, debug=False, ssl_context=[cert_file,cert_key])
+            print(f"Inference is working on https://{host}:{port}/v1/chat/completions. You can configure custom host IP and port, and ssl certificate via the apiconfig.txt file available at {config_file_path}")
+            app.run(host=host, port=port, debug=False, ssl_context=(cert_file,cert_key))
         else:
+            print(f"Inference is working on http://{host}:{port}/v1/chat/completions. You can configure custom host IP and port, and ssl certificate via the apiconfig.txt file available at {config_file_path}")
             app.run(host=host, port=port, debug=False)
 
 if __name__ == "__main__":
     main()
```

## Comparing `ALLMDEV-1.2.8.dist-info/METADATA` & `ALLMDEV-1.2.9.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ALLMDEV
-Version: 1.2.8
+Version: 1.2.9
 Summary: A simple and efficient python library for fast inference of GGUF Large Language Models.
 Author: All Advance AI
 Author-email: allmdev@allaai.com
 Maintainer: Soham Ghadge
 Maintainer-email: soham.ghadge@allaai.com
 Keywords: GGUF,GGUF Large Language Model,GGUF Large Language Models,GGUF Large Language Modeling,GGUF Large Language Modeling Library
 Description-Content-Type: text/markdown
@@ -83,23 +83,40 @@
 After your agents are created you can also initiate agent-specific API server using the allm-agentapi command:
 
 
 ```bash
 allm-agentapi --agent agent name
 ```
 
+You can also add additional documents to your existing agents by using the allm-updateagent command:
+
+```bash
+allm-updateagent --doc "document path" --agent agentname
+```
+
 ##Supported Cloud models.
 
-As of now, ALLM supports the Generative LLMs on VertexAI, including Gemini-1.5 pro and others. You can start local inference of cloud based models using the following command:
+As of now, ALLM supports the Generative LLMs on VertexAI, including Gemini-1.5 pro and AzureOpenAi models. You can start local inference of cloud based models using the following command:
 
 ```bash
-allm-cloud --projectid Id_of_your_GCP_project --region location_of_your_cloud_server
+allm-run-vertex --projectid Id_of_your_GCP_project --region location_of_your_cloud_server
+```
+or
+```bash
+allm-run-azure --key key --version version --endpoint https://{your_endpoint}.openai.azure.com --model model_name
 ```
 
 You can also have a custom agent working with your cloud deployed model using the following command. It is important to note that before this step, agent should be created using the commands in the AGENTS section above.
 
 ```bash
-allm-cloudagent --projectid Id_of_your_GCP_project --region location_of_your_cloud_server --agent agent_name
+allm-agentchat-vertex --projectid Id_of_your_GCP_project --region location_of_your_cloud_server --agent agent_name
+```
+or
+```bash
+allm-run-azure --key key --version version --endpoint https://{your_endpoint}.openai.azure.com --model model_name --agent agentname
 ```
+model_name is an optional parameter in both vertex and azure, if not mentioned, inference will work on gemini-1.0-pro-002 for vertex and gpt-35-turbo for OpenAI by default.
+
+
 ## Supported Model names
 Llama2, llama, llama2_chat, Llama_chat, Mistral, Mistral_instruct
```

