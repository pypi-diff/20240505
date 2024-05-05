# Comparing `tmp/gpt_batch-0.1.3.tar.gz` & `tmp/gpt_batch-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_batch-0.1.3.tar", last modified: Sun May  5 16:25:11 2024, max compression
+gzip compressed data, was "gpt_batch-0.1.5.tar", last modified: Sun May  5 18:31:20 2024, max compression
```

## Comparing `gpt_batch-0.1.3.tar` & `gpt_batch-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:25:11.066332 gpt_batch-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-05 16:25:11.066332 gpt_batch-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-05 16:25:02.000000 gpt_batch-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:25:11.066332 gpt_batch-0.1.3/gpt_batch/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-05 16:25:02.000000 gpt_batch-0.1.3/gpt_batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-05-05 16:25:02.000000 gpt_batch-0.1.3/gpt_batch/batcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:25:11.066332 gpt_batch-0.1.3/gpt_batch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-05 16:25:10.000000 gpt_batch-0.1.3/gpt_batch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-05 16:25:11.000000 gpt_batch-0.1.3/gpt_batch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 16:25:10.000000 gpt_batch-0.1.3/gpt_batch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-05 16:25:10.000000 gpt_batch-0.1.3/gpt_batch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-05 16:25:10.000000 gpt_batch-0.1.3/gpt_batch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 16:25:11.066332 gpt_batch-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-05 16:25:02.000000 gpt_batch-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:25:11.066332 gpt_batch-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 16:25:02.000000 gpt_batch-0.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-05 16:25:02.000000 gpt_batch-0.1.3/tests/test_batcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:31:20.449804 gpt_batch-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-05 18:31:20.449804 gpt_batch-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-05 18:31:10.000000 gpt_batch-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:31:20.449804 gpt_batch-0.1.5/gpt_batch/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-05 18:31:10.000000 gpt_batch-0.1.5/gpt_batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-05-05 18:31:10.000000 gpt_batch-0.1.5/gpt_batch/batcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:31:20.449804 gpt_batch-0.1.5/gpt_batch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-05 18:31:20.000000 gpt_batch-0.1.5/gpt_batch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-05 18:31:20.000000 gpt_batch-0.1.5/gpt_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 18:31:20.000000 gpt_batch-0.1.5/gpt_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-05 18:31:20.000000 gpt_batch-0.1.5/gpt_batch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-05 18:31:20.000000 gpt_batch-0.1.5/gpt_batch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 18:31:20.449804 gpt_batch-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-05 18:31:10.000000 gpt_batch-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:31:20.449804 gpt_batch-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 18:31:10.000000 gpt_batch-0.1.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-05 18:31:10.000000 gpt_batch-0.1.5/tests/test_batcher.py
```

### Comparing `gpt_batch-0.1.3/PKG-INFO` & `gpt_batch-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt_batch
-Version: 0.1.3
+Version: 0.1.5
 Summary: A package for batch processing with OpenAI API.
 Home-page: https://github.com/fengsxy/gpt_batch
 Author: Ted Yu
 Author-email: liddlerain@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `gpt_batch-0.1.3/README.md` & `gpt_batch-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `gpt_batch-0.1.3/gpt_batch/batcher.py` & `gpt_batch-0.1.5/gpt_batch/batcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,30 +53,34 @@
         )
         return (index, completion.choices[0].message.content)
 
     def process_attitude(self, message_list):
         new_list = []
         num_workers = self.num_workers
         timeout_duration = self.timeout_duration
-        retry_attempts=2
-
+        retry_attempts = 2
+    
         executor = ThreadPoolExecutor(max_workers=num_workers)
         message_chunks = list(self.chunk_list(message_list, num_workers))
-        for chunk in tqdm(message_chunks, desc="Processing messages"):
-            future_to_message =  {executor.submit(self.get_attitude, message): message for message in chunk}
-            for _ in range(retry_attempts):
-                done, not_done = wait(future_to_message.keys(), timeout=timeout_duration)
-                for future in not_done:
-                    future.cancel()
-                new_list.extend(future.result() for future in done if future.done())
-                if len(not_done) == 0:
-                    break
-                future_to_message = {executor.submit(self.get_attitude, future_to_message[future]): future_to_message[future] for future in not_done}
-        executor.shutdown(wait=False)
-        return new_list
+        try:
+            for chunk in tqdm(message_chunks, desc="Processing messages"):
+                future_to_message = {executor.submit(self.get_attitude, message): message for message in chunk}
+                for _ in range(retry_attempts):
+                    done, not_done = wait(future_to_message.keys(), timeout=timeout_duration)
+                    for future in not_done:
+                        future.cancel()
+                    new_list.extend(future.result() for future in done if future.done())
+                    if len(not_done) == 0:
+                        break
+                    future_to_message = {executor.submit(self.get_attitude, future_to_message[future]): future for future in not_done}
+        except Exception as e:
+            print(f"Error occurred: {e}")
+        finally:
+            executor.shutdown(wait=False)
+            return new_list
 
     def complete_attitude_list(self,attitude_list, max_length):
         completed_list = []
         current_index = 0
         for item in attitude_list:
             index, value = item
             # Fill in missing indices
```

### Comparing `gpt_batch-0.1.3/gpt_batch.egg-info/PKG-INFO` & `gpt_batch-0.1.5/gpt_batch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-batch
-Version: 0.1.3
+Version: 0.1.5
 Summary: A package for batch processing with OpenAI API.
 Home-page: https://github.com/fengsxy/gpt_batch
 Author: Ted Yu
 Author-email: liddlerain@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `gpt_batch-0.1.3/tests/test_batcher.py` & `gpt_batch-0.1.5/tests/test_batcher.py`

 * *Files identical despite different names*

