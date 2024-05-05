# Comparing `tmp/taskgen_ai-1.3.2.tar.gz` & `tmp/taskgen_ai-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskgen_ai-1.3.2.tar", last modified: Mon Apr 22 03:28:31 2024, max compression
+gzip compressed data, was "taskgen_ai-1.4.0.tar", last modified: Sun May  5 03:58:00 2024, max compression
```

## Comparing `taskgen_ai-1.3.2.tar` & `taskgen_ai-1.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-04-22 03:28:31.022642 taskgen_ai-1.3.2/
--rw-rw-r--   0 tanchongmin   (501) staff       (20)     1073 2024-02-26 00:45:10.000000 taskgen_ai-1.3.2/LICENSE
--rw-r--r--   0 tanchongmin   (501) staff       (20)    21112 2024-04-22 03:28:31.021906 taskgen_ai-1.3.2/PKG-INFO
--rw-rw-r--   0 tanchongmin   (501) staff       (20)    20503 2024-04-22 02:38:29.000000 taskgen_ai-1.3.2/README.md
--rw-rw-r--   0 tanchongmin   (501) staff       (20)      664 2024-04-22 02:38:21.000000 taskgen_ai-1.3.2/pyproject.toml
--rw-r--r--   0 tanchongmin   (501) staff       (20)       38 2024-04-22 03:28:31.022803 taskgen_ai-1.3.2/setup.cfg
--rw-rw-r--   0 tanchongmin   (501) staff       (20)      202 2024-04-22 02:38:59.000000 taskgen_ai-1.3.2/setup.py
-drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-04-22 03:28:31.017894 taskgen_ai-1.3.2/taskgen/
--rw-rw-r--   0 tanchongmin   (501) staff       (20)      170 2024-03-14 09:43:26.000000 taskgen_ai-1.3.2/taskgen/__init__.py
--rw-r--r--   0 tanchongmin   (501) staff       (20)    33533 2024-04-22 02:45:45.000000 taskgen_ai-1.3.2/taskgen/agent.py
--rw-r--r--   0 tanchongmin   (501) staff       (20)    36879 2024-04-22 03:04:08.000000 taskgen_ai-1.3.2/taskgen/base.py
-drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-04-22 03:28:31.021254 taskgen_ai-1.3.2/taskgen_ai.egg-info/
--rw-r--r--   0 tanchongmin   (501) staff       (20)    21112 2024-04-22 03:28:31.000000 taskgen_ai-1.3.2/taskgen_ai.egg-info/PKG-INFO
--rw-r--r--   0 tanchongmin   (501) staff       (20)      263 2024-04-22 03:28:31.000000 taskgen_ai-1.3.2/taskgen_ai.egg-info/SOURCES.txt
--rw-r--r--   0 tanchongmin   (501) staff       (20)        1 2024-04-22 03:28:31.000000 taskgen_ai-1.3.2/taskgen_ai.egg-info/dependency_links.txt
--rw-r--r--   0 tanchongmin   (501) staff       (20)       26 2024-04-22 03:28:31.000000 taskgen_ai-1.3.2/taskgen_ai.egg-info/requires.txt
--rw-r--r--   0 tanchongmin   (501) staff       (20)        8 2024-04-22 03:28:31.000000 taskgen_ai-1.3.2/taskgen_ai.egg-info/top_level.txt
+drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-05-05 03:58:00.177910 taskgen_ai-1.4.0/
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)     1073 2024-02-26 00:45:10.000000 taskgen_ai-1.4.0/LICENSE
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    21112 2024-05-05 03:58:00.177183 taskgen_ai-1.4.0/PKG-INFO
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)    20503 2024-05-05 03:56:28.000000 taskgen_ai-1.4.0/README.md
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)      664 2024-05-05 03:55:46.000000 taskgen_ai-1.4.0/pyproject.toml
+-rw-r--r--   0 tanchongmin   (501) staff       (20)       38 2024-05-05 03:58:00.178118 taskgen_ai-1.4.0/setup.cfg
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)      202 2024-05-05 03:56:40.000000 taskgen_ai-1.4.0/setup.py
+drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-05-05 03:58:00.172915 taskgen_ai-1.4.0/taskgen/
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)      170 2024-03-14 09:43:26.000000 taskgen_ai-1.4.0/taskgen/__init__.py
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    33494 2024-05-05 03:45:48.000000 taskgen_ai-1.4.0/taskgen/agent.py
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    36833 2024-05-05 03:45:51.000000 taskgen_ai-1.4.0/taskgen/base.py
+drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-05-05 03:58:00.176609 taskgen_ai-1.4.0/taskgen_ai.egg-info/
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    21112 2024-05-05 03:58:00.000000 taskgen_ai-1.4.0/taskgen_ai.egg-info/PKG-INFO
+-rw-r--r--   0 tanchongmin   (501) staff       (20)      263 2024-05-05 03:58:00.000000 taskgen_ai-1.4.0/taskgen_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 tanchongmin   (501) staff       (20)        1 2024-05-05 03:58:00.000000 taskgen_ai-1.4.0/taskgen_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 tanchongmin   (501) staff       (20)       26 2024-05-05 03:58:00.000000 taskgen_ai-1.4.0/taskgen_ai.egg-info/requires.txt
+-rw-r--r--   0 tanchongmin   (501) staff       (20)        8 2024-05-05 03:58:00.000000 taskgen_ai-1.4.0/taskgen_ai.egg-info/top_level.txt
```

### Comparing `taskgen_ai-1.3.2/LICENSE` & `taskgen_ai-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskgen_ai-1.3.2/PKG-INFO` & `taskgen_ai-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: taskgen-ai
-Version: 1.3.2
+Version: 1.4.0
 Summary: A Task-based agentic framework building on StrictJSON outputs by LLM agents
 Author-email: John Tan Chong Min <tanchongmin@gmail.com>
 Project-URL: Homepage, https://github.com/simbianai/taskgen
 Project-URL: Issues, https://github.com/simbianai/taskgen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1.3.6
 Requires-Dist: dill>=0.3.7
 
-# TaskGen v1.3.2
+# TaskGen v1.4.0
 ### A Task-based agentic framework building on StrictJSON outputs by LLM agents
 - Related Repositories: StrictJSON (https://github.com/tanchongmin/strictjson)
 - Video (Part 1): https://www.youtube.com/watch?v=O_XyTT7QGH4
 - Video (Part 2): https://www.youtube.com/watch?v=OWk7moRfTPE
 
 ### Creator's Preamble
 Happy to share that the task-based agentic framework I have been working on - TaskGen - is largely complete!
```

### Comparing `taskgen_ai-1.3.2/README.md` & `taskgen_ai-1.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# TaskGen v1.3.2
+# TaskGen v1.4.0
 ### A Task-based agentic framework building on StrictJSON outputs by LLM agents
 - Related Repositories: StrictJSON (https://github.com/tanchongmin/strictjson)
 - Video (Part 1): https://www.youtube.com/watch?v=O_XyTT7QGH4
 - Video (Part 2): https://www.youtube.com/watch?v=OWk7moRfTPE
 
 ### Creator's Preamble
 Happy to share that the task-based agentic framework I have been working on - TaskGen - is largely complete!
```

### Comparing `taskgen_ai-1.3.2/pyproject.toml` & `taskgen_ai-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "taskgen-ai"
-version = "1.3.2"
+version = "1.4.0"
 authors = [
   { name="John Tan Chong Min", email="tanchongmin@gmail.com" },
 ]
 description = "A Task-based agentic framework building on StrictJSON outputs by LLM agents"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `taskgen_ai-1.3.2/taskgen/agent.py` & `taskgen_ai-1.4.0/taskgen/agent.py`

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

### Comparing `taskgen_ai-1.3.2/taskgen/base.py` & `taskgen_ai-1.4.0/taskgen/base.py`

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

### Comparing `taskgen_ai-1.3.2/taskgen_ai.egg-info/PKG-INFO` & `taskgen_ai-1.4.0/taskgen_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: taskgen-ai
-Version: 1.3.2
+Version: 1.4.0
 Summary: A Task-based agentic framework building on StrictJSON outputs by LLM agents
 Author-email: John Tan Chong Min <tanchongmin@gmail.com>
 Project-URL: Homepage, https://github.com/simbianai/taskgen
 Project-URL: Issues, https://github.com/simbianai/taskgen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1.3.6
 Requires-Dist: dill>=0.3.7
 
-# TaskGen v1.3.2
+# TaskGen v1.4.0
 ### A Task-based agentic framework building on StrictJSON outputs by LLM agents
 - Related Repositories: StrictJSON (https://github.com/tanchongmin/strictjson)
 - Video (Part 1): https://www.youtube.com/watch?v=O_XyTT7QGH4
 - Video (Part 2): https://www.youtube.com/watch?v=OWk7moRfTPE
 
 ### Creator's Preamble
 Happy to share that the task-based agentic framework I have been working on - TaskGen - is largely complete!
```

