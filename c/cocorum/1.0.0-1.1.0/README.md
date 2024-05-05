# Comparing `tmp/cocorum-1.0.0.tar.gz` & `tmp/cocorum-1.1.0.tar.gz`

## Comparing `cocorum-1.0.0.tar` & `cocorum-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0   343002 2020-02-02 00:00:00.000000 cocorum-1.0.0/cocorum_icon.png
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cocorum-1.0.0/requirements.txt
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 cocorum-1.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    20037 2020-02-02 00:00:00.000000 cocorum-1.0.0/src/cocorum/__init__.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 cocorum-1.0.0/src/cocorum/localvars.py
--rw-r--r--   0        0        0    14486 2020-02-02 00:00:00.000000 cocorum-1.0.0/src/cocorum/ssechat.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 cocorum-1.0.0/src/cocorum/utils.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 cocorum-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 cocorum-1.0.0/README.md
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 cocorum-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 cocorum-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0   343002 2020-02-02 00:00:00.000000 cocorum-1.1.0/cocorum_icon.png
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cocorum-1.1.0/requirements.txt
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 cocorum-1.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    20037 2020-02-02 00:00:00.000000 cocorum-1.1.0/src/cocorum/__init__.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 cocorum-1.1.0/src/cocorum/localvars.py
+-rw-r--r--   0        0        0    14635 2020-02-02 00:00:00.000000 cocorum-1.1.0/src/cocorum/ssechat.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 cocorum-1.1.0/src/cocorum/utils.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 cocorum-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 cocorum-1.1.0/README.md
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 cocorum-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 cocorum-1.1.0/PKG-INFO
```

### Comparing `cocorum-1.0.0/cocorum_icon.png` & `cocorum-1.1.0/cocorum_icon.png`

 * *Files identical despite different names*

### Comparing `cocorum-1.0.0/.github/workflows/python-publish.yml` & `cocorum-1.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cocorum-1.0.0/src/cocorum/__init__.py` & `cocorum-1.1.0/src/cocorum/__init__.py`

 * *Files identical despite different names*

### Comparing `cocorum-1.0.0/src/cocorum/localvars.py` & `cocorum-1.1.0/src/cocorum/localvars.py`

 * *Files identical despite different names*

### Comparing `cocorum-1.0.0/src/cocorum/ssechat.py` & `cocorum-1.1.0/src/cocorum/ssechat.py`

 * *Files 2% similar despite different names*

```diff
@@ -338,15 +338,15 @@
         #subscription TODO
         #rant levels TODO
         self.message_length_max = jsondata["data"]["config"]["message_length_max"]
 
     def update_mailbox(self, jsondata):
         """Parse chat messages from an SSE data JSON"""
         #Add new messages
-        self.__mailbox += [SSEChatMessage(message_json, self) for message_json in jsondata["data"]["messages"]]
+        self.__mailbox += [SSEChatMessage(message_json, self) for message_json in jsondata["data"]["messages"] if message_json["id"] not in self.__mailbox]
 
     def clear_mailbox(self):
         """Delete anything in the mailbox"""
         self.__mailbox = []
 
     def clear_deleted_message_ids(self):
         """Clear and return the list of deleted message IDs"""
@@ -377,29 +377,36 @@
     @property
     def stream_id_b10(self):
         """The chat ID in user"""
         return utils.stream_id_36_to_10(self.stream_id)
 
     def get_message(self):
         """Return the next chat message (parsing any additional data), waits for it to come in, returns None if chat closed"""
-        if not self.__mailbox: #We don't already have messages
-            #JSON data is coming in, but it isn't of messages type'
-            while (jsondata := self.next_jsondata()) and jsondata["type"] != "messages":
-
-                #Messages were deleted
-                if jsondata["type"] in ("delete_messages", "delete_non_rant_messages"):
-                    self.deleted_message_ids += jsondata["data"]["message_ids"]
-
-                #Unimplemented event type
-                else:
-                    print("API sent an unimplemented SSE event type")
-                    print(jsondata)
+        #We don't already have messages
+        while not self.__mailbox:
+            jsondata = self.next_jsondata()
 
-            if not jsondata: #The chat has closed or a blank event
+            #The chat has closed
+            if not jsondata:
                 return
 
-            #Parse messages, users, and channels
-            self.update_mailbox(jsondata)
-            self.update_users(jsondata)
-            self.update_channels(jsondata)
+            #Messages were deleted
+            if jsondata["type"] in ("delete_messages", "delete_non_rant_messages"):
+                self.deleted_message_ids += jsondata["data"]["message_ids"]
+
+            #Re-initialize (could contain new messages)
+            elif jsondata["type"] == "init":
+                self.parse_init_data(jsondata)
+
+            #New messages
+            elif jsondata["type"] == "messages":
+                #Parse messages, users, and channels
+                self.update_mailbox(jsondata)
+                self.update_users(jsondata)
+                self.update_channels(jsondata)
+
+            #Unimplemented event type
+            else:
+                print("API sent an unimplemented SSE event type")
+                print(jsondata)
 
         return self.__mailbox.pop(0) #Return the first message in the mailbox, and then remove it from there
```

### Comparing `cocorum-1.0.0/src/cocorum/utils.py` & `cocorum-1.1.0/src/cocorum/utils.py`

 * *Files identical despite different names*

### Comparing `cocorum-1.0.0/LICENSE.txt` & `cocorum-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cocorum-1.0.0/README.md` & `cocorum-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cocorum-1.0.0/pyproject.toml` & `cocorum-1.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cocorum"
-version = "1.0.0"
+version = "1.1.0"
 keywords = ["rumble", "api", "wrapper", "livestream"]
 authors = [
   { name="Wilbur Jaywright", email="zargulthewizard@outlook.com" },
 ]
 description = "An unofficial Python wrapper for the Rumble Live Stream API v1.0 (beta)"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `cocorum-1.0.0/PKG-INFO` & `cocorum-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cocorum
-Version: 1.0.0
+Version: 1.1.0
 Summary: An unofficial Python wrapper for the Rumble Live Stream API v1.0 (beta)
 Project-URL: Homepage, https://github.com/thelabcat/rumble-api-wrapper-py
 Project-URL: Issues, https://github.com/thelabcat/rumble-api-wrapper-py/issues
 Project-URL: Rumble Live Stream API docs, https://rumblefaq.groovehq.com/help/how-to-use-rumble-s-live-stream-api
 Author-email: Wilbur Jaywright <zargulthewizard@outlook.com>
 License-File: LICENSE.txt
 Keywords: api,livestream,rumble,wrapper
```

