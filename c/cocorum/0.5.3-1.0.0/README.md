# Comparing `tmp/cocorum-0.5.3.tar.gz` & `tmp/cocorum-1.0.0.tar.gz`

## Comparing `cocorum-0.5.3.tar` & `cocorum-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0   343002 2020-02-02 00:00:00.000000 cocorum-0.5.3/cocorum_icon.png
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cocorum-0.5.3/requirements.txt
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 cocorum-0.5.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    20037 2020-02-02 00:00:00.000000 cocorum-0.5.3/src/cocorum/__init__.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 cocorum-0.5.3/src/cocorum/localvars.py
--rw-r--r--   0        0        0    14502 2020-02-02 00:00:00.000000 cocorum-0.5.3/src/cocorum/ssechat.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 cocorum-0.5.3/src/cocorum/utils.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 cocorum-0.5.3/LICENSE.txt
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 cocorum-0.5.3/README.md
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 cocorum-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 cocorum-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0   343002 2020-02-02 00:00:00.000000 cocorum-1.0.0/cocorum_icon.png
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cocorum-1.0.0/requirements.txt
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 cocorum-1.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    20037 2020-02-02 00:00:00.000000 cocorum-1.0.0/src/cocorum/__init__.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 cocorum-1.0.0/src/cocorum/localvars.py
+-rw-r--r--   0        0        0    14486 2020-02-02 00:00:00.000000 cocorum-1.0.0/src/cocorum/ssechat.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 cocorum-1.0.0/src/cocorum/utils.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 cocorum-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 cocorum-1.0.0/README.md
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 cocorum-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 cocorum-1.0.0/PKG-INFO
```

### Comparing `cocorum-0.5.3/cocorum_icon.png` & `cocorum-1.0.0/cocorum_icon.png`

 * *Files identical despite different names*

### Comparing `cocorum-0.5.3/.github/workflows/python-publish.yml` & `cocorum-1.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cocorum-0.5.3/src/cocorum/__init__.py` & `cocorum-1.0.0/src/cocorum/__init__.py`

 * *Files identical despite different names*

### Comparing `cocorum-0.5.3/src/cocorum/localvars.py` & `cocorum-1.0.0/src/cocorum/localvars.py`

 * *Files identical despite different names*

### Comparing `cocorum-0.5.3/src/cocorum/ssechat.py` & `cocorum-1.0.0/src/cocorum/ssechat.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,20 +6,17 @@
 Example usage:
 ```
 from cocorum import ssechat
 
 chat = ssechat.SSEChat(stream_id = STREAM_ID) #Stream ID can be base 10 or 36
 chat.clear_mailbox() #Erase messages that were still visible before we connected
 
-msg = True
-while msg:
-    msg = chat.next_chat_message() #Hangs until a new message arrives
+while True:
+    msg = chat.get_message() #Hangs until a new message arrives
     print(msg.user.username, ":", msg)
-
-print("Chat has closed.")
 ```
 S.D.G."""
 
 import json #For parsing SSE message data
 import requests
 import sseclient
 from .localvars import *
@@ -313,14 +310,15 @@
             return
 
         message = next(self.client, None)
         if not message:
             self.chat_running = False #Chat has been closed
             return
         if not message.data: #Blank SSE event
+            print("Blank SSE event:", message)
             #Self recursion should work so long as we don't get dozens of blank events in a row
             return self.next_jsondata()
 
         return json.loads(message.data)
 
     def parse_init_data(self, jsondata):
         """Extract initial chat data from the SSE init message JSON"""
@@ -377,16 +375,15 @@
         self.badges = {badge_slug : SSEChatUserBadge(badge_slug, jsondata["data"]["config"]["badges"][badge_slug], self) for badge_slug in jsondata["data"]["config"]["badges"].keys()}
 
     @property
     def stream_id_b10(self):
         """The chat ID in user"""
         return utils.stream_id_36_to_10(self.stream_id)
 
-    @property
-    def next_chat_message(self):
+    def get_message(self):
         """Return the next chat message (parsing any additional data), waits for it to come in, returns None if chat closed"""
         if not self.__mailbox: #We don't already have messages
             #JSON data is coming in, but it isn't of messages type'
             while (jsondata := self.next_jsondata()) and jsondata["type"] != "messages":
 
                 #Messages were deleted
                 if jsondata["type"] in ("delete_messages", "delete_non_rant_messages"):
```

### Comparing `cocorum-0.5.3/src/cocorum/utils.py` & `cocorum-1.0.0/src/cocorum/utils.py`

 * *Files identical despite different names*

### Comparing `cocorum-0.5.3/LICENSE.txt` & `cocorum-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cocorum-0.5.3/README.md` & `cocorum-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,20 +37,17 @@
 
 ```
 from cocorum import ssechat
 
 chat = ssechat.SSEChat(stream_id = STREAM_ID) #Stream ID can be base 10 or 36
 chat.clear_mailbox() #Erase messages that were still visible before we connected
 
-msg = True
-while msg:
-    msg = chat.next_chat_message() #Hangs until a new message arrives
+while True:
+    msg = chat.get_message() #Hangs until a new message arrives
     print(msg.user.username, ":", msg)
-
-print("Chat has closed.")
 ```
 
 ## Conclusion
 Hope this helps!
 
 I, Wilbur Jaywright, and my brand, Marswide BGL, have no official association with Rumble Corp. beyond that of a normal user and/or channel on the Rumble Video platform. This wrapper is not officially endorsed by Rumble Corp. or its subsidiaries.
```

### Comparing `cocorum-0.5.3/pyproject.toml` & `cocorum-1.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cocorum"
-version = "0.5.3"
+version = "1.0.0"
 keywords = ["rumble", "api", "wrapper", "livestream"]
 authors = [
   { name="Wilbur Jaywright", email="zargulthewizard@outlook.com" },
 ]
 description = "An unofficial Python wrapper for the Rumble Live Stream API v1.0 (beta)"
 readme = "README.md"
 requires-python = ">=3.8"
@@ -16,14 +16,14 @@
   "requests",
   "sseclient", #Only for the Rumble chat SSE stream
   ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Operating System :: OS Independent",
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
 ]
 
 [project.urls]
 Homepage = "https://github.com/thelabcat/rumble-api-wrapper-py"
 Issues = "https://github.com/thelabcat/rumble-api-wrapper-py/issues"
 "Rumble Live Stream API docs" = "https://rumblefaq.groovehq.com/help/how-to-use-rumble-s-live-stream-api"
```

### Comparing `cocorum-0.5.3/PKG-INFO` & `cocorum-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.3
 Name: cocorum
-Version: 0.5.3
+Version: 1.0.0
 Summary: An unofficial Python wrapper for the Rumble Live Stream API v1.0 (beta)
 Project-URL: Homepage, https://github.com/thelabcat/rumble-api-wrapper-py
 Project-URL: Issues, https://github.com/thelabcat/rumble-api-wrapper-py/issues
 Project-URL: Rumble Live Stream API docs, https://rumblefaq.groovehq.com/help/how-to-use-rumble-s-live-stream-api
 Author-email: Wilbur Jaywright <zargulthewizard@outlook.com>
 License-File: LICENSE.txt
 Keywords: api,livestream,rumble,wrapper
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: requests
 Requires-Dist: sseclient
 Description-Content-Type: text/markdown
@@ -56,20 +56,17 @@
 
 ```
 from cocorum import ssechat
 
 chat = ssechat.SSEChat(stream_id = STREAM_ID) #Stream ID can be base 10 or 36
 chat.clear_mailbox() #Erase messages that were still visible before we connected
 
-msg = True
-while msg:
-    msg = chat.next_chat_message() #Hangs until a new message arrives
+while True:
+    msg = chat.get_message() #Hangs until a new message arrives
     print(msg.user.username, ":", msg)
-
-print("Chat has closed.")
 ```
 
 ## Conclusion
 Hope this helps!
 
 I, Wilbur Jaywright, and my brand, Marswide BGL, have no official association with Rumble Corp. beyond that of a normal user and/or channel on the Rumble Video platform. This wrapper is not officially endorsed by Rumble Corp. or its subsidiaries.
```

