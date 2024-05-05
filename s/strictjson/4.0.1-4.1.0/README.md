# Comparing `tmp/strictjson-4.0.1.tar.gz` & `tmp/strictjson-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strictjson-4.0.1.tar", last modified: Mon Apr 22 03:29:13 2024, max compression
+gzip compressed data, was "strictjson-4.1.0.tar", last modified: Sun May  5 04:28:15 2024, max compression
```

## Comparing `strictjson-4.0.1.tar` & `strictjson-4.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-04-22 03:29:13.524657 strictjson-4.0.1/
--rw-r--r--   0 tanchongmin   (501) staff       (20)     1073 2024-01-05 08:31:13.000000 strictjson-4.0.1/LICENSE
--rw-r--r--   0 tanchongmin   (501) staff       (20)    15786 2024-04-22 03:29:13.523885 strictjson-4.0.1/PKG-INFO
--rw-r--r--   0 tanchongmin   (501) staff       (20)    15150 2024-04-22 02:39:25.000000 strictjson-4.0.1/README.md
--rw-r--r--   0 tanchongmin   (501) staff       (20)      690 2024-04-22 02:37:17.000000 strictjson-4.0.1/pyproject.toml
--rw-r--r--   0 tanchongmin   (501) staff       (20)       38 2024-04-22 03:29:13.524781 strictjson-4.0.1/setup.cfg
-drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-04-22 03:29:13.520788 strictjson-4.0.1/strictjson/
--rw-rw-r--   0 tanchongmin   (501) staff       (20)      171 2024-02-26 00:45:10.000000 strictjson-4.0.1/strictjson/__init__.py
--rw-r--r--   0 tanchongmin   (501) staff       (20)    33533 2024-04-22 02:45:45.000000 strictjson-4.0.1/strictjson/agent.py
--rw-r--r--   0 tanchongmin   (501) staff       (20)    36879 2024-04-22 03:03:40.000000 strictjson-4.0.1/strictjson/base.py
-drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-04-22 03:29:13.523335 strictjson-4.0.1/strictjson.egg-info/
--rw-r--r--   0 tanchongmin   (501) staff       (20)    15786 2024-04-22 03:29:13.000000 strictjson-4.0.1/strictjson.egg-info/PKG-INFO
--rw-r--r--   0 tanchongmin   (501) staff       (20)      263 2024-04-22 03:29:13.000000 strictjson-4.0.1/strictjson.egg-info/SOURCES.txt
--rw-r--r--   0 tanchongmin   (501) staff       (20)        1 2024-04-22 03:29:13.000000 strictjson-4.0.1/strictjson.egg-info/dependency_links.txt
--rw-r--r--   0 tanchongmin   (501) staff       (20)       26 2024-04-22 03:29:13.000000 strictjson-4.0.1/strictjson.egg-info/requires.txt
--rw-r--r--   0 tanchongmin   (501) staff       (20)       11 2024-04-22 03:29:13.000000 strictjson-4.0.1/strictjson.egg-info/top_level.txt
+drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-05-05 04:28:15.399492 strictjson-4.1.0/
+-rw-r--r--   0 tanchongmin   (501) staff       (20)     1073 2024-01-05 08:31:13.000000 strictjson-4.1.0/LICENSE
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    15930 2024-05-05 04:28:15.398864 strictjson-4.1.0/PKG-INFO
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    15294 2024-05-05 04:13:13.000000 strictjson-4.1.0/README.md
+-rw-r--r--   0 tanchongmin   (501) staff       (20)      690 2024-05-05 04:10:48.000000 strictjson-4.1.0/pyproject.toml
+-rw-r--r--   0 tanchongmin   (501) staff       (20)       38 2024-05-05 04:28:15.399657 strictjson-4.1.0/setup.cfg
+drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-05-05 04:28:15.395494 strictjson-4.1.0/strictjson/
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)      171 2024-02-26 00:45:10.000000 strictjson-4.1.0/strictjson/__init__.py
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    33494 2024-05-05 03:45:48.000000 strictjson-4.1.0/strictjson/agent.py
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    36833 2024-05-05 03:45:51.000000 strictjson-4.1.0/strictjson/base.py
+drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-05-05 04:28:15.398099 strictjson-4.1.0/strictjson.egg-info/
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    15930 2024-05-05 04:28:15.000000 strictjson-4.1.0/strictjson.egg-info/PKG-INFO
+-rw-r--r--   0 tanchongmin   (501) staff       (20)      263 2024-05-05 04:28:15.000000 strictjson-4.1.0/strictjson.egg-info/SOURCES.txt
+-rw-r--r--   0 tanchongmin   (501) staff       (20)        1 2024-05-05 04:28:15.000000 strictjson-4.1.0/strictjson.egg-info/dependency_links.txt
+-rw-r--r--   0 tanchongmin   (501) staff       (20)       26 2024-05-05 04:28:15.000000 strictjson-4.1.0/strictjson.egg-info/requires.txt
+-rw-r--r--   0 tanchongmin   (501) staff       (20)       11 2024-05-05 04:28:15.000000 strictjson-4.1.0/strictjson.egg-info/top_level.txt
```

### Comparing `strictjson-4.0.1/LICENSE` & `strictjson-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `strictjson-4.0.1/PKG-INFO` & `strictjson-4.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: strictjson
-Version: 4.0.1
+Version: 4.1.0
 Summary: A Strict JSON Framework for LLM Outputs, that fixes problems that json.loads() cannot solve
 Author-email: John Tan Chong Min <tanchongmin@gmail.com>
 Project-URL: Homepage, https://github.com/tanchongmin/strictjson
 Project-URL: Issues, https://github.com/tanchongmin/strictjson/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1.3.6
 Requires-Dist: dill>=0.3.7
 
-# Strict JSON v4.0.1
+# Strict JSON v4.1.0
 [UPDATE]: For Agentic Framework, do check out TaskGen (the official Agentic Framework building on StrictJSON). This will make the StrictJSON repo neater and this github will focus on using StrictJSON for LLM Output Parsing
 - https://github.com/simbianai/taskgen
 
 ### A Strict JSON Framework for LLM Outputs, that fixes problems that json.loads() cannot solve
 - Works for JSON outputs with multiple ' or " or { or } or \ or unmatched braces/brackets that may break a json.loads()
 
 ### Base Functionalities (see Tutorial.ipynb)
@@ -27,14 +27,15 @@
 - Easy construction of LLM-based functions using ```Function``` (Note: renamed from `strict_function` to keep in line with naming convention of capitalised class groups. `strict_function` still works for legacy support.)
 - Easy integration with OpenAI JSON Mode by setting `openai_json_mode = True`
 - Exposing of llm variable for `strict_json` and `Function` for easy use of self-defined LLMs
 
 ### Tutorials and Community Support
 - Created: 7 Apr 2023
 - Collaborators welcome
+- Video tutorial (Ask Me Anything): [https://www.youtube.com/watch?v=L4aytve5v1Q](https://www.youtube.com/watch?v=L4aytve5v1Q)
 - Video tutorial: [https://www.youtube.com/watch?v=IjTUKAciTCg](https://www.youtube.com/watch?v=1N-znDTlhNc)
 - Discussion Channel (my discord - John's AI Group): [discord.gg/bzp87AHJy5](discord.gg/bzp87AHJy5)
 
 ## How do I use this? 
 1. Download package via command line ```pip install strictjson```
 2. Set up your OpenAPI API Key. Refer to ```Tutorial.ipynb``` for how to do it for Jupyter Notebooks.
 3. Import the required functions from ```strictjson``` and use them!
@@ -265,15 +266,15 @@
 
 #### Example Input
 ```python
 res = strict_json(system_prompt = 'You are a classifier',
                     user_prompt = 'It is a beautiful and sunny day',
                     output_format = {'Sentiment': ['Type of Sentiment', 
                                                    'Strength of Sentiment, type: Enum[1, 2, 3, 4, 5]'],
-                                    'Adjectives': "Name and Description, type: List[Dict['Name', 'Description']]",
+                                    'Adjectives': "Name and Description as separate keys, type: List[Dict['Name', 'Description']]",
                                     'Words': {
                                         'Number of words': 'Word count', 
                                         'Language': {
                                               'English': 'Whether it is English, type: bool',
                                               'Chinese': 'Whether it is Chinese, type: bool'
                                                   },
                                         'Proper Words': 'Whether the words are proper in the native language, type: bool'
```

### Comparing `strictjson-4.0.1/README.md` & `strictjson-4.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Strict JSON v4.0.1
+# Strict JSON v4.1.0
 [UPDATE]: For Agentic Framework, do check out TaskGen (the official Agentic Framework building on StrictJSON). This will make the StrictJSON repo neater and this github will focus on using StrictJSON for LLM Output Parsing
 - https://github.com/simbianai/taskgen
 
 ### A Strict JSON Framework for LLM Outputs, that fixes problems that json.loads() cannot solve
 - Works for JSON outputs with multiple ' or " or { or } or \ or unmatched braces/brackets that may break a json.loads()
 
 ### Base Functionalities (see Tutorial.ipynb)
@@ -11,14 +11,15 @@
 - Easy construction of LLM-based functions using ```Function``` (Note: renamed from `strict_function` to keep in line with naming convention of capitalised class groups. `strict_function` still works for legacy support.)
 - Easy integration with OpenAI JSON Mode by setting `openai_json_mode = True`
 - Exposing of llm variable for `strict_json` and `Function` for easy use of self-defined LLMs
 
 ### Tutorials and Community Support
 - Created: 7 Apr 2023
 - Collaborators welcome
+- Video tutorial (Ask Me Anything): [https://www.youtube.com/watch?v=L4aytve5v1Q](https://www.youtube.com/watch?v=L4aytve5v1Q)
 - Video tutorial: [https://www.youtube.com/watch?v=IjTUKAciTCg](https://www.youtube.com/watch?v=1N-znDTlhNc)
 - Discussion Channel (my discord - John's AI Group): [discord.gg/bzp87AHJy5](discord.gg/bzp87AHJy5)
 
 ## How do I use this? 
 1. Download package via command line ```pip install strictjson```
 2. Set up your OpenAPI API Key. Refer to ```Tutorial.ipynb``` for how to do it for Jupyter Notebooks.
 3. Import the required functions from ```strictjson``` and use them!
@@ -249,15 +250,15 @@
 
 #### Example Input
 ```python
 res = strict_json(system_prompt = 'You are a classifier',
                     user_prompt = 'It is a beautiful and sunny day',
                     output_format = {'Sentiment': ['Type of Sentiment', 
                                                    'Strength of Sentiment, type: Enum[1, 2, 3, 4, 5]'],
-                                    'Adjectives': "Name and Description, type: List[Dict['Name', 'Description']]",
+                                    'Adjectives': "Name and Description as separate keys, type: List[Dict['Name', 'Description']]",
                                     'Words': {
                                         'Number of words': 'Word count', 
                                         'Language': {
                                               'English': 'Whether it is English, type: bool',
                                               'Chinese': 'Whether it is Chinese, type: bool'
                                                   },
                                         'Proper Words': 'Whether the words are proper in the native language, type: bool'
```

### Comparing `strictjson-4.0.1/pyproject.toml` & `strictjson-4.1.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "strictjson"
-version = "4.0.1"
+version = "4.1.0"
 authors = [
   { name="John Tan Chong Min", email="tanchongmin@gmail.com" },
 ]
 description = "A Strict JSON Framework for LLM Outputs, that fixes problems that json.loads() cannot solve"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `strictjson-4.0.1/strictjson/agent.py` & `strictjson-4.1.0/strictjson/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         ''' Adds a list of memories '''
         if not isinstance(memory_list, list):
             memory_list = list(memory_list)
         self.memory.extend(memory_list)
         
     def remove(self, memory_to_remove):
         ''' Removes a memory '''
-        self.memory.remove(new_memory)
+        self.memory.remove(memory_to_remove)
         
     def reset(self):
         ''' Clears all memory '''
         self.memory = []
         
     def isempty(self) -> bool:
         ''' Returns whether or not the memory is empty '''
@@ -256,18 +256,18 @@
         if task != '':
             filtered_fn_list = self.memory_bank['Function'].retrieve(task)
             # add back compulsory functions (default: use_llm, end_task) if present in function_map
             for name, function in self.function_map.items():
                 if function.is_compulsory:
                     filtered_fn_list.append(function)
                 
-        # add in additional context to the prompt
+        # add in global context to the prompt
         global_context = ''
         if self.get_global_context is not None:
-            global_context = 'Additional Context:' + self.get_global_context(self) + '\n'
+            global_context = 'Global Context:' + self.get_global_context(self) + '\n'
         
         system_prompt = f"You are an agent named {self.agent_name} with the following description: ```{self.agent_description}```\n"
         if provide_function_list:
             system_prompt += f"You have the following Equipped Functions available:\n```{self.list_functions(filtered_fn_list)}```\n"
         system_prompt += global_context
         system_prompt += query
         
@@ -377,18 +377,18 @@
                 # Function is done separately
                 if name == 'Function': continue
                 # Do not need to add to context if the memory item is empty
                 if self.memory_bank[name].isempty(): continue
                 rag_info += f'Related {name}: ```{self.memory_bank[name].retrieve(subtask)}```\n'
 
             res = self.query(query = f'{rag_info}Overall Task:```{self.overall_task}```\nContext:```{self.subtasks_completed}```\nAssigned Subtask: ```{function_params["instruction"]}```\nPerform the Assigned Subtask only - do not just state what has or can be done - actually generate the outcome of Assigned Subtask fully but only within your Agent Capabilities', 
-                            output_format = {"Assigned Subtask Outcome": "Generate a full response to the Assigned Subtask"},
+                            output_format = {"Output": "Generate a full response to the Assigned Subtask"},
                             provide_function_list = False)
             
-            res = res["Assigned Subtask Outcome"]
+            res = res["Output"]
             
             if self.verbose: 
                 print('>', res)
                 print()
             
         elif function_name == "end_task":
             return
@@ -419,15 +419,15 @@
         ''' Based on what the task is and the subtasks completed, we get the next subtask, function and input parameters'''
         
         if task == '':
                 background_info = f"Assigned Task:```{self.task}```\nAssigned Plan: ```{self.overall_plan}```\nPast Subtasks Completed: ```{self.subtasks_completed}```\n"
         else:
             background_info = f"Assigned Task:```{task}```\n"
                 
-        # only add overall plan if there is and not evaluasting for single task
+        # only add overall plan if there is and not evaluating for single task
         if task == '':
             task = ', '.join(self.overall_plan) if self.overall_plan is not None else task
         task = self.task if task == '' else task
             
         # Add in memory to the Agent
         rag_info = ''
         for name in self.memory_bank.keys():
```

### Comparing `strictjson-4.0.1/strictjson/base.py` & `strictjson-4.1.0/strictjson/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -473,15 +473,15 @@
         # start off with no error message
         error_msg = ''
 
         # wrap the values with angle brackets and wrap keys with delimiter to encourage LLM to modify it
         new_output_format = wrap_with_angle_brackets(output_format, delimiter, 1)
         
         output_format_prompt = f'''\nOutput in the following json string format: {new_output_format}
-Update text enclosed in <>. Be concise. Output only the json string without any explanation. You must output valid json with all keys present.'''
+Update text enclosed in <>. Output only a valid json string beginning with {{ and ending with }}'''
 
         for i in range(num_tries):
             my_system_prompt = str(system_prompt) + output_format_prompt + error_msg
             my_user_prompt = str(user_prompt) 
 
             # Use OpenAI to get a response
             res = chat(my_system_prompt, my_user_prompt, **kwargs)
```

### Comparing `strictjson-4.0.1/strictjson.egg-info/PKG-INFO` & `strictjson-4.1.0/strictjson.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: strictjson
-Version: 4.0.1
+Version: 4.1.0
 Summary: A Strict JSON Framework for LLM Outputs, that fixes problems that json.loads() cannot solve
 Author-email: John Tan Chong Min <tanchongmin@gmail.com>
 Project-URL: Homepage, https://github.com/tanchongmin/strictjson
 Project-URL: Issues, https://github.com/tanchongmin/strictjson/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1.3.6
 Requires-Dist: dill>=0.3.7
 
-# Strict JSON v4.0.1
+# Strict JSON v4.1.0
 [UPDATE]: For Agentic Framework, do check out TaskGen (the official Agentic Framework building on StrictJSON). This will make the StrictJSON repo neater and this github will focus on using StrictJSON for LLM Output Parsing
 - https://github.com/simbianai/taskgen
 
 ### A Strict JSON Framework for LLM Outputs, that fixes problems that json.loads() cannot solve
 - Works for JSON outputs with multiple ' or " or { or } or \ or unmatched braces/brackets that may break a json.loads()
 
 ### Base Functionalities (see Tutorial.ipynb)
@@ -27,14 +27,15 @@
 - Easy construction of LLM-based functions using ```Function``` (Note: renamed from `strict_function` to keep in line with naming convention of capitalised class groups. `strict_function` still works for legacy support.)
 - Easy integration with OpenAI JSON Mode by setting `openai_json_mode = True`
 - Exposing of llm variable for `strict_json` and `Function` for easy use of self-defined LLMs
 
 ### Tutorials and Community Support
 - Created: 7 Apr 2023
 - Collaborators welcome
+- Video tutorial (Ask Me Anything): [https://www.youtube.com/watch?v=L4aytve5v1Q](https://www.youtube.com/watch?v=L4aytve5v1Q)
 - Video tutorial: [https://www.youtube.com/watch?v=IjTUKAciTCg](https://www.youtube.com/watch?v=1N-znDTlhNc)
 - Discussion Channel (my discord - John's AI Group): [discord.gg/bzp87AHJy5](discord.gg/bzp87AHJy5)
 
 ## How do I use this? 
 1. Download package via command line ```pip install strictjson```
 2. Set up your OpenAPI API Key. Refer to ```Tutorial.ipynb``` for how to do it for Jupyter Notebooks.
 3. Import the required functions from ```strictjson``` and use them!
@@ -265,15 +266,15 @@
 
 #### Example Input
 ```python
 res = strict_json(system_prompt = 'You are a classifier',
                     user_prompt = 'It is a beautiful and sunny day',
                     output_format = {'Sentiment': ['Type of Sentiment', 
                                                    'Strength of Sentiment, type: Enum[1, 2, 3, 4, 5]'],
-                                    'Adjectives': "Name and Description, type: List[Dict['Name', 'Description']]",
+                                    'Adjectives': "Name and Description as separate keys, type: List[Dict['Name', 'Description']]",
                                     'Words': {
                                         'Number of words': 'Word count', 
                                         'Language': {
                                               'English': 'Whether it is English, type: bool',
                                               'Chinese': 'Whether it is Chinese, type: bool'
                                                   },
                                         'Proper Words': 'Whether the words are proper in the native language, type: bool'
```

