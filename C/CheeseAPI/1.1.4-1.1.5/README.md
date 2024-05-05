# Comparing `tmp/cheeseapi-1.1.4.tar.gz` & `tmp/cheeseapi-1.1.5.tar.gz`

## Comparing `cheeseapi-1.1.4.tar` & `cheeseapi-1.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 cheeseapi-1.1.4/CheeseAPI/__init__.py
--rw-r--r--   0        0        0     7395 2020-02-02 00:00:00.000000 cheeseapi-1.1.4/CheeseAPI/app.py
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 cheeseapi-1.1.4/CheeseAPI/cors.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cheeseapi-1.1.4/CheeseAPI/exception.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 cheeseapi-1.1.4/CheeseAPI/file.py
--rw-r--r--   0        0        0    32435 2020-02-02 00:00:00.000000 cheeseapi-1.1.4/CheeseAPI/handle.py
--rw-r--r--   0        0        0     4493 2020-02-02 00:00:00.000000 cheeseapi-1.1.4/CheeseAPI/protocol.py
--rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 cheeseapi-1.1.4/CheeseAPI/request.py
--rw-r--r--   0        0        0    17621 2020-02-02 00:00:00.000000 cheeseapi-1.1.4/CheeseAPI/response.py
--rw-r--r--   0        0        0    13136 2020-02-02 00:00:00.000000 cheeseapi-1.1.4/CheeseAPI/route.py
--rw-r--r--   0        0        0    10335 2020-02-02 00:00:00.000000 cheeseapi-1.1.4/CheeseAPI/schedule.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cheeseapi-1.1.4/CheeseAPI/server.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 cheeseapi-1.1.4/CheeseAPI/signal.py
--rw-r--r--   0        0        0     8558 2020-02-02 00:00:00.000000 cheeseapi-1.1.4/CheeseAPI/text.py
--rw-r--r--   0        0        0    12835 2020-02-02 00:00:00.000000 cheeseapi-1.1.4/CheeseAPI/validator.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 cheeseapi-1.1.4/CheeseAPI/websocket.py
--rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 cheeseapi-1.1.4/CheeseAPI/workspace.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 cheeseapi-1.1.4/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeseapi-1.1.4/LICENSE
--rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 cheeseapi-1.1.4/README.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cheeseapi-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 cheeseapi-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/CheeseAPI/__init__.py
+-rw-r--r--   0        0        0     7395 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/CheeseAPI/app.py
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/CheeseAPI/cors.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/CheeseAPI/exception.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/CheeseAPI/file.py
+-rw-r--r--   0        0        0    32435 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/CheeseAPI/handle.py
+-rw-r--r--   0        0        0     4493 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/CheeseAPI/protocol.py
+-rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/CheeseAPI/request.py
+-rw-r--r--   0        0        0    17621 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/CheeseAPI/response.py
+-rw-r--r--   0        0        0    13136 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/CheeseAPI/route.py
+-rw-r--r--   0        0        0    10363 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/CheeseAPI/schedule.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/CheeseAPI/server.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/CheeseAPI/signal.py
+-rw-r--r--   0        0        0     8558 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/CheeseAPI/text.py
+-rw-r--r--   0        0        0    12835 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/CheeseAPI/validator.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/CheeseAPI/websocket.py
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/CheeseAPI/workspace.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/LICENSE
+-rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/README.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/PKG-INFO
```

### Comparing `cheeseapi-1.1.4/CheeseAPI/app.py` & `cheeseapi-1.1.5/CheeseAPI/app.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.4/CheeseAPI/cors.py` & `cheeseapi-1.1.5/CheeseAPI/cors.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.4/CheeseAPI/exception.py` & `cheeseapi-1.1.5/CheeseAPI/exception.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.4/CheeseAPI/file.py` & `cheeseapi-1.1.5/CheeseAPI/file.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.4/CheeseAPI/handle.py` & `cheeseapi-1.1.5/CheeseAPI/handle.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.4/CheeseAPI/protocol.py` & `cheeseapi-1.1.5/CheeseAPI/protocol.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.4/CheeseAPI/request.py` & `cheeseapi-1.1.5/CheeseAPI/request.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.4/CheeseAPI/response.py` & `cheeseapi-1.1.5/CheeseAPI/response.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.4/CheeseAPI/route.py` & `cheeseapi-1.1.5/CheeseAPI/route.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.4/CheeseAPI/schedule.py` & `cheeseapi-1.1.5/CheeseAPI/schedule.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,35 +229,35 @@
 
         if not startTimer:
             startTimer = datetime.datetime.now()
 
         if fn:
             self._app._managers_['schedules'][key] = {
                 'timer': timer,
-                'fn': dill.dumps(fn),
+                'fn': dill.dumps(fn, recurse = True),
                 'startTimer': startTimer,
                 'expected_repetition_num': expected_repetition_num,
                 'total_repetition_num': 0,
                 'auto_remove': auto_remove,
                 'active': True
             }
             return
 
-        def decorator(fn):
+        def wrapper(fn):
             self._app._managers_['schedules'][key] = {
                 'timer': timer,
-                'fn': dill.dumps(fn),
+                'fn': dill.dumps(fn, recurse = True),
                 'startTimer': startTimer,
                 'expected_repetition_num': expected_repetition_num,
                 'total_repetition_num': 0,
                 'auto_remove': auto_remove,
                 'active': True
             }
             return fn
-        return decorator
+        return wrapper
 
     @overload
     def remove(self, fn: Callable):
         '''
         通过函数删除计划。
 
         ```python
```

### Comparing `cheeseapi-1.1.4/CheeseAPI/server.py` & `cheeseapi-1.1.5/CheeseAPI/server.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.4/CheeseAPI/signal.py` & `cheeseapi-1.1.5/CheeseAPI/signal.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.4/CheeseAPI/text.py` & `cheeseapi-1.1.5/CheeseAPI/text.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.4/CheeseAPI/validator.py` & `cheeseapi-1.1.5/CheeseAPI/validator.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.4/CheeseAPI/websocket.py` & `cheeseapi-1.1.5/CheeseAPI/websocket.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.4/CheeseAPI/workspace.py` & `cheeseapi-1.1.5/CheeseAPI/workspace.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.4/LICENSE` & `cheeseapi-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.4/README.md` & `cheeseapi-1.1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,16 @@
 ```python
 from CheeseAPI import app, Response
 
 @app.route.get('/')
 async def index(**kwargs):
     return Response('这里是CheeseAPI！')
 
-app.run()
+if __name__ == '__main__':
+    app.run()
 ```
 
 运行`app.py`，可以看到打印了一些服务器的基本信息：
 
 ```
 $ python app.py
 (STARTING) 2024-03-19 14:03:12.405969 > The master process 346 started
```

### Comparing `cheeseapi-1.1.4/pyproject.toml` & `cheeseapi-1.1.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "hatchling" ]
 build-backend = "hatchling.build"
 
 [project]
 name = "CheeseAPI"
-version = "1.1.4"
+version = "1.1.5"
 description = "一款web协程框架。"
 readme = "README.md"
 license-files = { paths = [ "LICENSE" ] }
 authors = [
     { name = "Cheese Unknown", email = "cheese@cheese.ren" }
 ]
 keywords = [ 'API', 'BackEnd' ]
```

### Comparing `cheeseapi-1.1.4/PKG-INFO` & `cheeseapi-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: CheeseAPI
-Version: 1.1.4
+Version: 1.1.5
 Summary: 一款web协程框架。
 Project-URL: Source, https://github.com/CheeseUnknown/CheeseAPI
 Author-email: Cheese Unknown <cheese@cheese.ren>
 License-File: LICENSE
 Keywords: API,BackEnd
 Requires-Dist: cheeselog==1.0.*
 Requires-Dist: cheesesignal==1.1.*
@@ -92,15 +92,16 @@
 ```python
 from CheeseAPI import app, Response
 
 @app.route.get('/')
 async def index(**kwargs):
     return Response('这里是CheeseAPI！')
 
-app.run()
+if __name__ == '__main__':
+    app.run()
 ```
 
 运行`app.py`，可以看到打印了一些服务器的基本信息：
 
 ```
 $ python app.py
 (STARTING) 2024-03-19 14:03:12.405969 > The master process 346 started
```

