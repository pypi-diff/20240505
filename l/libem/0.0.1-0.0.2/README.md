# Comparing `tmp/libem-0.0.1.tar.gz` & `tmp/libem-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libem-0.0.1.tar", last modified: Fri May  3 09:46:18 2024, max compression
+gzip compressed data, was "libem-0.0.2.tar", last modified: Sun May  5 04:07:37 2024, max compression
```

## Comparing `libem-0.0.1.tar` & `libem-0.0.2.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-03 09:46:18.852364 libem-0.0.1/
--rw-r--r--   0 silv       (501) staff       (20)    11357 2024-05-01 02:16:29.000000 libem-0.0.1/LICENSE
--rw-r--r--   0 silv       (501) staff       (20)      272 2024-05-03 09:46:18.852248 libem-0.0.1/PKG-INFO
--rw-r--r--   0 silv       (501) staff       (20)      212 2024-05-03 05:42:27.000000 libem-0.0.1/README.md
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-03 09:46:18.848492 libem-0.0.1/benchmark/
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-01 02:59:47.000000 libem-0.0.1/benchmark/__init__.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-03 09:46:18.848562 libem-0.0.1/eval/
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-02 20:23:30.000000 libem-0.0.1/eval/__init__.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-03 09:46:18.849524 libem-0.0.1/libem/
--rw-r--r--   0 silv       (501) staff       (20)      350 2024-05-03 08:56:58.000000 libem-0.0.1/libem/__init__.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-03 09:46:18.850879 libem-0.0.1/libem/browse/
--rw-r--r--   0 silv       (501) staff       (20)      104 2024-05-03 09:12:55.000000 libem-0.0.1/libem/browse/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     1542 2024-05-03 09:32:13.000000 libem-0.0.1/libem/browse/function.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-03 06:17:55.000000 libem-0.0.1/libem/browse/parameter.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-02 20:20:44.000000 libem-0.0.1/libem/browse/prompt.py
--rw-r--r--   0 silv       (501) staff       (20)      364 2024-05-03 08:56:38.000000 libem-0.0.1/libem/constant.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-03 09:46:18.851259 libem-0.0.1/libem/core/
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-03 06:45:38.000000 libem-0.0.1/libem/core/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     2357 2024-05-03 09:44:29.000000 libem-0.0.1/libem/core/model.py
--rw-r--r--   0 silv       (501) staff       (20)      240 2024-05-03 06:53:59.000000 libem-0.0.1/libem/core/struct.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-03 09:46:18.851797 libem-0.0.1/libem/match/
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-02 20:10:31.000000 libem-0.0.1/libem/match/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)      352 2024-05-03 09:41:15.000000 libem-0.0.1/libem/match/function.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-03 06:17:55.000000 libem-0.0.1/libem/match/parameter.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-02 20:20:44.000000 libem-0.0.1/libem/match/prompt.py
--rw-r--r--   0 silv       (501) staff       (20)      141 2024-05-03 06:50:11.000000 libem-0.0.1/libem/parameter.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-03 09:46:18.852069 libem-0.0.1/libem/prepare/
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-02 20:13:20.000000 libem-0.0.1/libem/prepare/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-02 19:12:22.000000 libem-0.0.1/libem/prepare/function.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-03 06:17:55.000000 libem-0.0.1/libem/prepare/parameter.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-02 20:20:44.000000 libem-0.0.1/libem/prepare/prompt.py
--rw-r--r--   0 silv       (501) staff       (20)      235 2024-05-02 20:19:34.000000 libem-0.0.1/libem/prompt.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-03 09:46:18.850299 libem-0.0.1/libem.egg-info/
--rw-r--r--   0 silv       (501) staff       (20)      272 2024-05-03 09:46:18.000000 libem-0.0.1/libem.egg-info/PKG-INFO
--rw-r--r--   0 silv       (501) staff       (20)      659 2024-05-03 09:46:18.000000 libem-0.0.1/libem.egg-info/SOURCES.txt
--rw-r--r--   0 silv       (501) staff       (20)        1 2024-05-03 09:46:18.000000 libem-0.0.1/libem.egg-info/dependency_links.txt
--rw-r--r--   0 silv       (501) staff       (20)      110 2024-05-03 09:46:18.000000 libem-0.0.1/libem.egg-info/requires.txt
--rw-r--r--   0 silv       (501) staff       (20)       27 2024-05-03 09:46:18.000000 libem-0.0.1/libem.egg-info/top_level.txt
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-03 09:46:18.852136 libem-0.0.1/serve/
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-01 03:03:29.000000 libem-0.0.1/serve/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)       38 2024-05-03 09:46:18.852395 libem-0.0.1/setup.cfg
--rw-r--r--   0 silv       (501) staff       (20)      421 2024-05-03 09:45:46.000000 libem-0.0.1/setup.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-05 04:07:37.984113 libem-0.0.2/
+-rw-r--r--   0 silv       (501) staff       (20)    11357 2024-05-01 02:16:29.000000 libem-0.0.2/LICENSE
+-rw-r--r--   0 silv       (501) staff       (20)      272 2024-05-05 04:07:37.983976 libem-0.0.2/PKG-INFO
+-rw-r--r--   0 silv       (501) staff       (20)      289 2024-05-03 17:08:11.000000 libem-0.0.2/README.md
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-05 04:07:37.981315 libem-0.0.2/benchmark/
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-01 02:59:47.000000 libem-0.0.2/benchmark/__init__.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-05 04:07:37.981385 libem-0.0.2/eval/
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-02 20:23:30.000000 libem-0.0.2/eval/__init__.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-05 04:07:37.981788 libem-0.0.2/libem/
+-rw-r--r--   0 silv       (501) staff       (20)      810 2024-05-05 01:22:28.000000 libem-0.0.2/libem/__init__.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-05 04:07:37.982649 libem-0.0.2/libem/browse/
+-rw-r--r--   0 silv       (501) staff       (20)       92 2024-05-05 00:16:54.000000 libem-0.0.2/libem/browse/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     1542 2024-05-03 17:04:24.000000 libem-0.0.2/libem/browse/function.py
+-rw-r--r--   0 silv       (501) staff       (20)       85 2024-05-05 01:29:22.000000 libem-0.0.2/libem/browse/parameter.py
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-02 20:20:44.000000 libem-0.0.2/libem/browse/prompt.py
+-rw-r--r--   0 silv       (501) staff       (20)      364 2024-05-03 17:03:58.000000 libem-0.0.2/libem/constant.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-05 04:07:37.982899 libem-0.0.2/libem/core/
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-03 06:45:38.000000 libem-0.0.2/libem/core/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     2519 2024-05-05 01:15:38.000000 libem-0.0.2/libem/core/model.py
+-rw-r--r--   0 silv       (501) staff       (20)      809 2024-05-05 00:31:17.000000 libem-0.0.2/libem/core/struct.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-05 04:07:37.983351 libem-0.0.2/libem/match/
+-rw-r--r--   0 silv       (501) staff       (20)       90 2024-05-05 00:16:44.000000 libem-0.0.2/libem/match/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     1199 2024-05-05 01:33:02.000000 libem-0.0.2/libem/match/function.py
+-rw-r--r--   0 silv       (501) staff       (20)       85 2024-05-05 01:29:02.000000 libem-0.0.2/libem/match/parameter.py
+-rw-r--r--   0 silv       (501) staff       (20)      374 2024-05-05 01:35:11.000000 libem-0.0.2/libem/match/prompt.py
+-rw-r--r--   0 silv       (501) staff       (20)      216 2024-05-04 23:40:49.000000 libem-0.0.2/libem/parameter.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-05 04:07:37.983644 libem-0.0.2/libem/prepare/
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-02 20:13:20.000000 libem-0.0.2/libem/prepare/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-02 19:12:22.000000 libem-0.0.2/libem/prepare/function.py
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-03 06:17:55.000000 libem-0.0.2/libem/prepare/parameter.py
+-rw-r--r--   0 silv       (501) staff       (20)       38 2024-05-05 00:06:37.000000 libem-0.0.2/libem/prepare/prompt.py
+-rw-r--r--   0 silv       (501) staff       (20)      185 2024-05-05 01:22:34.000000 libem-0.0.2/libem/prompt.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-05 04:07:37.982275 libem-0.0.2/libem.egg-info/
+-rw-r--r--   0 silv       (501) staff       (20)      272 2024-05-05 04:07:37.000000 libem-0.0.2/libem.egg-info/PKG-INFO
+-rw-r--r--   0 silv       (501) staff       (20)      672 2024-05-05 04:07:37.000000 libem-0.0.2/libem.egg-info/SOURCES.txt
+-rw-r--r--   0 silv       (501) staff       (20)        1 2024-05-05 04:07:37.000000 libem-0.0.2/libem.egg-info/dependency_links.txt
+-rw-r--r--   0 silv       (501) staff       (20)      126 2024-05-05 04:07:37.000000 libem-0.0.2/libem.egg-info/requires.txt
+-rw-r--r--   0 silv       (501) staff       (20)       27 2024-05-05 04:07:37.000000 libem-0.0.2/libem.egg-info/top_level.txt
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-05 04:07:37.983826 libem-0.0.2/serve/
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-04 23:17:56.000000 libem-0.0.2/serve/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)      578 2024-05-04 23:21:19.000000 libem-0.0.2/serve/run.py
+-rw-r--r--   0 silv       (501) staff       (20)       38 2024-05-05 04:07:37.984150 libem-0.0.2/setup.cfg
+-rw-r--r--   0 silv       (501) staff       (20)      421 2024-05-05 04:07:35.000000 libem-0.0.2/setup.py
```

### Comparing `libem-0.0.1/LICENSE` & `libem-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `libem-0.0.1/libem/browse/function.py` & `libem-0.0.2/libem/browse/function.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 
 
 """ Google search function """
 
 # Set up environment variables for Google API if they are not already set
 os.environ.setdefault(
     "GOOGLE_CSE_ID",
-    libem.LIBEM_CONFIG.get("google_cse_id", "")
+    libem.LIBEM_CONFIG.get("GOOGLE_CSE_ID", "")
 )
 os.environ.setdefault(
     "GOOGLE_API_KEY",
-    libem.LIBEM_CONFIG.get("google_api_key", "")
+    libem.LIBEM_CONFIG.get("GOOGLE_API_KEY", "")
 )
 
 
 def google(entity):
     # Ensure required environment variables are set
     if not os.environ.get("GOOGLE_CSE_ID") or not os.environ.get("GOOGLE_API_KEY"):
         raise EnvironmentError(f"GOOGLE_CSE_ID or GOOGLE_API_KEY is not set. "
```

### Comparing `libem-0.0.1/libem/core/model.py` & `libem-0.0.2/libem/core/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 from openai import OpenAI
 
 import libem
 
 """ OpenAI calls """
 os.environ.setdefault(
     "OPENAI_API_KEY",
-    libem.LIBEM_CONFIG.get("openai_api_key", "")
+    libem.LIBEM_CONFIG.get("OPENAI_API_KEY", "")
 )
 
 
 # LLM call with multiple rounds of tool use
-def run(prompt: str, model: str, tools: list[types.ModuleType],
-        max_model_call: int = 3) -> str:
+def call(prompt: str, tools: list[types.ModuleType],
+         model: str, temperature: float = 0,
+         max_model_call: int = 3) -> str:
     if not os.environ.get("OPENAI_API_KEY"):
         raise EnvironmentError(f"OPENAI_API_KEY is not set. "
                                f"Check your environment or {libem.LIBEM_CONFIG_FILE}.")
     client = OpenAI()
 
     # Get the functions from the tools
     available_functions = {
@@ -31,26 +32,28 @@
     # Call the model
     messages = [{"role": "user", "content": prompt}]
     response = client.chat.completions.create(
         model=model,
         messages=messages,
         tools=tools,
         tool_choice="auto",
+        temperature=temperature,
     )
     response_message = response.choices[0].message
     tool_calls = response_message.tool_calls
 
     # Call the tools
     num_model_call = 1
     while tool_calls and num_model_call < max_model_call:
         messages.append(response_message)
         for tool_call in tool_calls:
             function_name = tool_call.function.name
             function_to_call = available_functions[function_name]
             function_args = json.loads(tool_call.function.arguments)
+            print(f"Tool: {function_name} - running ..")
             function_response = function_to_call(**function_args)
             messages.append(
                 {
                     "tool_call_id": tool_call.id,
                     "role": "tool",
                     "name": function_name,
                     "content": function_response,
@@ -60,14 +63,15 @@
 
         # Call the model again with the tool outcomes
         response = client.chat.completions.create(
             model=model,
             messages=messages,
             tools=tools,
             tool_choice="auto",
+            temperature=temperature,
         )
         response_message = response.choices[0].message
         tool_calls = response_message.tool_calls
         num_model_call += 1
 
     if num_model_call == max_model_call:
         raise Warning(f"Max call reached: {messages}\n{response_message}")
```

### Comparing `libem-0.0.1/libem.egg-info/SOURCES.txt` & `libem-0.0.2/libem.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -23,8 +23,9 @@
 libem/match/function.py
 libem/match/parameter.py
 libem/match/prompt.py
 libem/prepare/__init__.py
 libem/prepare/function.py
 libem/prepare/parameter.py
 libem/prepare/prompt.py
-serve/__init__.py
+serve/__init__.py
+serve/run.py
```

