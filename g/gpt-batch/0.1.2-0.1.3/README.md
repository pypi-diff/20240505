# Comparing `tmp/gpt_batch-0.1.2.tar.gz` & `tmp/gpt_batch-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_batch-0.1.2.tar", last modified: Sat May  4 16:12:31 2024, max compression
+gzip compressed data, was "gpt_batch-0.1.3.tar", last modified: Sun May  5 16:25:11 2024, max compression
```

## Comparing `gpt_batch-0.1.2.tar` & `gpt_batch-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:12:31.756536 gpt_batch-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-04 16:12:31.756536 gpt_batch-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-04 16:12:22.000000 gpt_batch-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:12:31.756536 gpt_batch-0.1.2/gpt_batch/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-04 16:12:22.000000 gpt_batch-0.1.2/gpt_batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7263 2024-05-04 16:12:22.000000 gpt_batch-0.1.2/gpt_batch/batcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:12:31.756536 gpt_batch-0.1.2/gpt_batch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-04 16:12:31.000000 gpt_batch-0.1.2/gpt_batch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-04 16:12:31.000000 gpt_batch-0.1.2/gpt_batch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 16:12:31.000000 gpt_batch-0.1.2/gpt_batch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-04 16:12:31.000000 gpt_batch-0.1.2/gpt_batch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-04 16:12:31.000000 gpt_batch-0.1.2/gpt_batch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 16:12:31.756536 gpt_batch-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-04 16:12:22.000000 gpt_batch-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:12:31.756536 gpt_batch-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 16:12:22.000000 gpt_batch-0.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-04 16:12:22.000000 gpt_batch-0.1.2/tests/test_batcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:25:11.066332 gpt_batch-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-05 16:25:11.066332 gpt_batch-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-05 16:25:02.000000 gpt_batch-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:25:11.066332 gpt_batch-0.1.3/gpt_batch/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-05 16:25:02.000000 gpt_batch-0.1.3/gpt_batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-05-05 16:25:02.000000 gpt_batch-0.1.3/gpt_batch/batcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:25:11.066332 gpt_batch-0.1.3/gpt_batch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-05 16:25:10.000000 gpt_batch-0.1.3/gpt_batch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-05 16:25:11.000000 gpt_batch-0.1.3/gpt_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 16:25:10.000000 gpt_batch-0.1.3/gpt_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-05 16:25:10.000000 gpt_batch-0.1.3/gpt_batch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-05 16:25:10.000000 gpt_batch-0.1.3/gpt_batch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 16:25:11.066332 gpt_batch-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-05 16:25:02.000000 gpt_batch-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:25:11.066332 gpt_batch-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 16:25:02.000000 gpt_batch-0.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-05 16:25:02.000000 gpt_batch-0.1.3/tests/test_batcher.py
```

### Comparing `gpt_batch-0.1.2/PKG-INFO` & `gpt_batch-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt_batch
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package for batch processing with OpenAI API.
 Home-page: https://github.com/fengsxy/gpt_batch
 Author: Ted Yu
 Author-email: liddlerain@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -17,15 +17,15 @@
 A simple tool to batch process messages using OpenAI's GPT models. `GPTBatcher` allows for efficient handling of multiple requests simultaneously, ensuring quick responses and robust error management.
 
 ## Installation
 
 To get started with `GPTBatcher`, clone this repository to your local machine. Navigate to the repository directory and install the required dependencies (if any) by running:
 
 ```bash
-pip install -r requirements.txt
+pip install gpt_batch
 ```
 
 ## Quick Start
 
 To use `GPTBatcher`, you need to instantiate it with your OpenAI API key and the model name you wish to use. Here's a quick guide:
 
 ### Handling Message Lists
@@ -71,15 +71,8 @@
 - **num_workers** (int): Number of parallel workers for request handling, default is 64.
 - **timeout_duration** (int): Timeout for API responses in seconds, default is 60.
 - **retry_attempts** (int): How many times to retry a failed request, default is 2.
 - **miss_index** (list): Tracks indices of requests that failed to process correctly.
 
 For more detailed documentation on the parameters and methods, refer to the class docstring.
 
-## License
-
-Specify your licensing information here.
-
-```
-
-This README provides clear instructions on how to install and use the `GPTBatcher`, along with detailed explanations of its configuration parameters. Adjust the "License" section as necessary based on your project's licensing terms.
```

### Comparing `gpt_batch-0.1.2/README.md` & `gpt_batch-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 A simple tool to batch process messages using OpenAI's GPT models. `GPTBatcher` allows for efficient handling of multiple requests simultaneously, ensuring quick responses and robust error management.
 
 ## Installation
 
 To get started with `GPTBatcher`, clone this repository to your local machine. Navigate to the repository directory and install the required dependencies (if any) by running:
 
 ```bash
-pip install -r requirements.txt
+pip install gpt_batch
 ```
 
 ## Quick Start
 
 To use `GPTBatcher`, you need to instantiate it with your OpenAI API key and the model name you wish to use. Here's a quick guide:
 
 ### Handling Message Lists
@@ -59,15 +59,7 @@
 - **temperature** (float): Adjusts the creativity of the responses, default is 1.
 - **num_workers** (int): Number of parallel workers for request handling, default is 64.
 - **timeout_duration** (int): Timeout for API responses in seconds, default is 60.
 - **retry_attempts** (int): How many times to retry a failed request, default is 2.
 - **miss_index** (list): Tracks indices of requests that failed to process correctly.
 
 For more detailed documentation on the parameters and methods, refer to the class docstring.
-
-## License
-
-Specify your licensing information here.
-
-```
-
-This README provides clear instructions on how to install and use the `GPTBatcher`, along with detailed explanations of its configuration parameters. Adjust the "License" section as necessary based on your project's licensing terms.
```

### Comparing `gpt_batch-0.1.2/gpt_batch/batcher.py` & `gpt_batch-0.1.3/gpt_batch/batcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             for _ in range(retry_attempts):
                 done, not_done = wait(future_to_message.keys(), timeout=timeout_duration)
                 for future in not_done:
                     future.cancel()
                 new_list.extend(future.result() for future in done if future.done())
                 if len(not_done) == 0:
                     break
-                future_to_message = {executor.submit(self.get_attitude, future_to_message[future]): future_to_message[future] for future, msg in not_done}
+                future_to_message = {executor.submit(self.get_attitude, future_to_message[future]): future_to_message[future] for future in not_done}
         executor.shutdown(wait=False)
         return new_list
 
     def complete_attitude_list(self,attitude_list, max_length):
         completed_list = []
         current_index = 0
         for item in attitude_list:
```

### Comparing `gpt_batch-0.1.2/gpt_batch.egg-info/PKG-INFO` & `gpt_batch-0.1.3/gpt_batch.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-batch
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package for batch processing with OpenAI API.
 Home-page: https://github.com/fengsxy/gpt_batch
 Author: Ted Yu
 Author-email: liddlerain@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -17,15 +17,15 @@
 A simple tool to batch process messages using OpenAI's GPT models. `GPTBatcher` allows for efficient handling of multiple requests simultaneously, ensuring quick responses and robust error management.
 
 ## Installation
 
 To get started with `GPTBatcher`, clone this repository to your local machine. Navigate to the repository directory and install the required dependencies (if any) by running:
 
 ```bash
-pip install -r requirements.txt
+pip install gpt_batch
 ```
 
 ## Quick Start
 
 To use `GPTBatcher`, you need to instantiate it with your OpenAI API key and the model name you wish to use. Here's a quick guide:
 
 ### Handling Message Lists
@@ -71,15 +71,8 @@
 - **num_workers** (int): Number of parallel workers for request handling, default is 64.
 - **timeout_duration** (int): Timeout for API responses in seconds, default is 60.
 - **retry_attempts** (int): How many times to retry a failed request, default is 2.
 - **miss_index** (list): Tracks indices of requests that failed to process correctly.
 
 For more detailed documentation on the parameters and methods, refer to the class docstring.
 
-## License
-
-Specify your licensing information here.
-
-```
-
-This README provides clear instructions on how to install and use the `GPTBatcher`, along with detailed explanations of its configuration parameters. Adjust the "License" section as necessary based on your project's licensing terms.
```

### Comparing `gpt_batch-0.1.2/tests/test_batcher.py` & `gpt_batch-0.1.3/tests/test_batcher.py`

 * *Files identical despite different names*

