# Comparing `tmp/wsclient-0.3.0.tar.gz` & `tmp/wsclient-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wsclient-0.3.0.tar", last modified: Sun Aug 30 16:37:38 2020, max compression
+gzip compressed data, was "wsclient-0.4.0.tar", last modified: Sun May  5 08:16:48 2024, max compression
```

## Comparing `wsclient-0.3.0.tar` & `wsclient-0.4.0.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxrwxrwx   0        0        0        0 2020-08-30 16:37:38.000000 wsclient-0.3.0/
--rw-rw-rw-   0        0        0      423 2020-08-30 16:37:38.000000 wsclient-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0       78 2020-05-02 01:41:10.000000 wsclient-0.3.0/README.md
--rw-rw-rw-   0        0        0       42 2020-08-30 16:37:38.000000 wsclient-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      717 2020-08-19 04:55:56.000000 wsclient-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2020-08-30 16:37:38.000000 wsclient-0.3.0/signalr_aio_wsclient/
-drwxrwxrwx   0        0        0        0 2020-08-30 16:37:38.000000 wsclient-0.3.0/signalr_aio_wsclient/events/
--rw-rw-rw-   0        0        0      586 2020-01-26 13:03:38.000000 wsclient-0.3.0/signalr_aio_wsclient/events/_events.py
--rw-rw-rw-   0        0        0       32 2020-01-26 13:03:38.000000 wsclient-0.3.0/signalr_aio_wsclient/events/__init__.py
-drwxrwxrwx   0        0        0        0 2020-08-30 16:37:38.000000 wsclient-0.3.0/signalr_aio_wsclient/hubs/
--rw-rw-rw-   0        0        0     1560 2020-01-26 13:03:38.000000 wsclient-0.3.0/signalr_aio_wsclient/hubs/_hub.py
--rw-rw-rw-   0        0        0       23 2020-01-26 13:03:38.000000 wsclient-0.3.0/signalr_aio_wsclient/hubs/__init__.py
-drwxrwxrwx   0        0        0        0 2020-08-30 16:37:38.000000 wsclient-0.3.0/signalr_aio_wsclient/transports/
--rw-rw-rw-   0        0        0       52 2020-01-26 13:03:38.000000 wsclient-0.3.0/signalr_aio_wsclient/transports/_exceptions.py
--rw-rw-rw-   0        0        0     2419 2020-01-26 13:03:38.000000 wsclient-0.3.0/signalr_aio_wsclient/transports/_parameters.py
--rw-rw-rw-   0        0        0      454 2020-01-26 13:03:38.000000 wsclient-0.3.0/signalr_aio_wsclient/transports/_queue_events.py
--rw-rw-rw-   0        0        0     3798 2020-01-26 13:03:38.000000 wsclient-0.3.0/signalr_aio_wsclient/transports/_transport.py
--rw-rw-rw-   0        0        0       33 2020-01-26 13:03:38.000000 wsclient-0.3.0/signalr_aio_wsclient/transports/__init__.py
--rw-rw-rw-   0        0        0     1478 2020-01-26 13:03:38.000000 wsclient-0.3.0/signalr_aio_wsclient/_connection.py
--rw-rw-rw-   0        0        0       35 2020-01-26 13:03:38.000000 wsclient-0.3.0/signalr_aio_wsclient/__init__.py
-drwxrwxrwx   0        0        0        0 2020-08-30 16:37:38.000000 wsclient-0.3.0/test/
--rw-rw-rw-   0        0        0     2019 2020-01-26 13:03:38.000000 wsclient-0.3.0/test/test_extend_attrs.py
-drwxrwxrwx   0        0        0        0 2020-08-30 16:37:38.000000 wsclient-0.3.0/wsclient/
--rw-rw-rw-   0        0        0    22866 2020-08-26 08:38:20.000000 wsclient-0.3.0/wsclient/base.py
--rw-rw-rw-   0        0        0     6783 2020-08-26 08:38:20.000000 wsclient-0.3.0/wsclient/channel.py
--rw-rw-rw-   0        0        0    28432 2020-08-26 08:38:20.000000 wsclient-0.3.0/wsclient/conn.py
--rw-rw-rw-   0        0        0     5613 2020-08-19 04:55:56.000000 wsclient-0.3.0/wsclient/conn_mgr.py
--rw-rw-rw-   0        0        0      218 2020-08-19 04:55:55.000000 wsclient-0.3.0/wsclient/errors.py
--rw-rw-rw-   0        0        0     7712 2020-05-02 01:41:11.000000 wsclient-0.3.0/wsclient/extend_attrs.py
--rw-rw-rw-   0        0        0     2051 2020-05-02 01:41:11.000000 wsclient-0.3.0/wsclient/interpreter.py
--rw-rw-rw-   0        0        0       48 2020-01-26 13:03:38.000000 wsclient-0.3.0/wsclient/merged.py
--rw-rw-rw-   0        0        0    21344 2020-08-19 04:55:56.000000 wsclient-0.3.0/wsclient/sub.py
--rw-rw-rw-   0        0        0    24650 2020-08-30 15:12:09.000000 wsclient-0.3.0/wsclient/transport.py
--rw-rw-rw-   0        0        0     5032 2020-06-16 15:03:48.000000 wsclient-0.3.0/wsclient/url.py
--rw-rw-rw-   0        0        0      621 2020-08-19 04:55:55.000000 wsclient-0.3.0/wsclient/__init__.py
-drwxrwxrwx   0        0        0        0 2020-08-30 16:37:38.000000 wsclient-0.3.0/wsclient.egg-info/
--rw-rw-rw-   0        0        0        1 2020-08-30 16:37:38.000000 wsclient-0.3.0/wsclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      423 2020-08-30 16:37:38.000000 wsclient-0.3.0/wsclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       86 2020-08-30 16:37:38.000000 wsclient-0.3.0/wsclient.egg-info/requires.txt
--rw-rw-rw-   0        0        0      893 2020-08-30 16:37:38.000000 wsclient-0.3.0/wsclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       30 2020-08-30 16:37:38.000000 wsclient-0.3.0/wsclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:16:48.824117 wsclient-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-05 08:16:41.000000 wsclient-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-05 08:16:48.824117 wsclient-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-05 08:16:41.000000 wsclient-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-05 08:16:41.000000 wsclient-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 08:16:48.824117 wsclient-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-05 08:16:41.000000 wsclient-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:16:48.820117 wsclient-0.4.0/signalr_aio_wsclient/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-05 08:16:41.000000 wsclient-0.4.0/signalr_aio_wsclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-05 08:16:41.000000 wsclient-0.4.0/signalr_aio_wsclient/_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:16:48.820117 wsclient-0.4.0/signalr_aio_wsclient/events/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-05 08:16:41.000000 wsclient-0.4.0/signalr_aio_wsclient/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-05 08:16:41.000000 wsclient-0.4.0/signalr_aio_wsclient/events/_events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:16:48.820117 wsclient-0.4.0/signalr_aio_wsclient/hubs/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-05 08:16:41.000000 wsclient-0.4.0/signalr_aio_wsclient/hubs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-05 08:16:41.000000 wsclient-0.4.0/signalr_aio_wsclient/hubs/_hub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:16:48.820117 wsclient-0.4.0/signalr_aio_wsclient/transports/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-05 08:16:41.000000 wsclient-0.4.0/signalr_aio_wsclient/transports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-05 08:16:41.000000 wsclient-0.4.0/signalr_aio_wsclient/transports/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-05 08:16:41.000000 wsclient-0.4.0/signalr_aio_wsclient/transports/_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-05 08:16:41.000000 wsclient-0.4.0/signalr_aio_wsclient/transports/_queue_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-05-05 08:16:41.000000 wsclient-0.4.0/signalr_aio_wsclient/transports/_transport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:16:48.820117 wsclient-0.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-05 08:16:41.000000 wsclient-0.4.0/test/test_extend_attrs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:16:48.824117 wsclient-0.4.0/wsclient/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-05 08:16:41.000000 wsclient-0.4.0/wsclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22266 2024-05-05 08:16:41.000000 wsclient-0.4.0/wsclient/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6751 2024-05-05 08:16:41.000000 wsclient-0.4.0/wsclient/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28005 2024-05-05 08:16:41.000000 wsclient-0.4.0/wsclient/conn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5431 2024-05-05 08:16:41.000000 wsclient-0.4.0/wsclient/conn_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-05 08:16:41.000000 wsclient-0.4.0/wsclient/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7421 2024-05-05 08:16:41.000000 wsclient-0.4.0/wsclient/extend_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-05 08:16:41.000000 wsclient-0.4.0/wsclient/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-05 08:16:41.000000 wsclient-0.4.0/wsclient/merged.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22128 2024-05-05 08:16:41.000000 wsclient-0.4.0/wsclient/sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25454 2024-05-05 08:16:41.000000 wsclient-0.4.0/wsclient/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-05-05 08:16:41.000000 wsclient-0.4.0/wsclient/url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:16:48.824117 wsclient-0.4.0/wsclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-05 08:16:48.000000 wsclient-0.4.0/wsclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-05 08:16:48.000000 wsclient-0.4.0/wsclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 08:16:48.000000 wsclient-0.4.0/wsclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-05 08:16:48.000000 wsclient-0.4.0/wsclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-05 08:16:48.000000 wsclient-0.4.0/wsclient.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `wsclient-0.3.0/signalr_aio_wsclient/events/_events.py` & `wsclient-0.4.0/signalr_aio_wsclient/events/_events.py`

 * *Files identical despite different names*

### Comparing `wsclient-0.3.0/signalr_aio_wsclient/transports/_parameters.py` & `wsclient-0.4.0/signalr_aio_wsclient/transports/_parameters.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,69 +8,77 @@
 from json import dumps
 from urllib.parse import urlparse, urlunparse, urlencode
 import requests
 
 
 class WebSocketParameters:
     def __init__(self, connection):
-        self.protocol_version = '1.5'
+        self.protocol_version = "1.5"
         self.raw_url = self._clean_url(connection.url)
         self.conn_data = self._get_conn_data(connection.hub)
         self.session = connection.session
         self.headers = None
         self.socket_conf = None
         self._negotiate()
         self.socket_url = self._get_socket_url()
 
     @staticmethod
     def _clean_url(url):
-        if url[-1] == '/':
+        if url[-1] == "/":
             return url[:-1]
         else:
             return url
 
     @staticmethod
     def _get_conn_data(hub):
-        conn_data = dumps([{'name': hub}])
+        conn_data = dumps([{"name": hub}])
         return conn_data
 
     @staticmethod
     def _format_url(url, action, query):
-        return '{url}/{action}?{query}'.format(url=url, action=action, query=query)
+        return "{url}/{action}?{query}".format(url=url, action=action, query=query)
 
     def _negotiate(self):
         if self.session is None:
             self.session = requests.Session()
-        query = urlencode({
-            'connectionData': self.conn_data,
-            'clientProtocol': self.protocol_version,
-        })
-        url = self._format_url(self.raw_url, 'negotiate', query)
+        query = urlencode(
+            {
+                "connectionData": self.conn_data,
+                "clientProtocol": self.protocol_version,
+            }
+        )
+        url = self._format_url(self.raw_url, "negotiate", query)
         self.headers = dict(self.session.headers)
         request = self.session.get(url)
-        self.headers['Cookie'] = self._get_cookie_str(request.cookies)
+        self.headers["Cookie"] = self._get_cookie_str(request.cookies)
         self.socket_conf = request.json()
 
     @staticmethod
     def _get_cookie_str(request):
-        return '; '.join([
-            '%s=%s' % (name, value)
-            for name, value in request.items()
-        ])
+        return "; ".join(["%s=%s" % (name, value) for name, value in request.items()])
 
     def _get_socket_url(self):
         ws_url = self._get_ws_url_from()
-        query = urlencode({
-            'transport': 'webSockets',
-            'connectionToken': self.socket_conf['ConnectionToken'],
-            'connectionData': self.conn_data,
-            'clientProtocol': self.socket_conf['ProtocolVersion'],
-        })
+        query = urlencode(
+            {
+                "transport": "webSockets",
+                "connectionToken": self.socket_conf["ConnectionToken"],
+                "connectionData": self.conn_data,
+                "clientProtocol": self.socket_conf["ProtocolVersion"],
+            }
+        )
 
-        return self._format_url(ws_url, 'connect', query)
+        return self._format_url(ws_url, "connect", query)
 
     def _get_ws_url_from(self):
         parsed = urlparse(self.raw_url)
-        scheme = 'wss' if parsed.scheme == 'https' else 'ws'
-        url_data = (scheme, parsed.netloc, parsed.path, parsed.params, parsed.query, parsed.fragment)
+        scheme = "wss" if parsed.scheme == "https" else "ws"
+        url_data = (
+            scheme,
+            parsed.netloc,
+            parsed.path,
+            parsed.params,
+            parsed.query,
+            parsed.fragment,
+        )
 
         return urlunparse(url_data)
```

### Comparing `wsclient-0.3.0/signalr_aio_wsclient/transports/_transport.py` & `wsclient-0.4.0/signalr_aio_wsclient/transports/_transport.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # Stanislav Lazarov
 
 # python compatiblity for <3.6
 try:
     ModuleNotFoundError
 except NameError:
     ModuleNotFoundError = ImportError
+import platform
 
 # -----------------------------------
 # Internal Imports
 from ._exceptions import ConnectionClosed
 from ._parameters import WebSocketParameters
 from ._queue_events import InvokeEvent, CloseEvent
 
@@ -28,14 +29,16 @@
 try:
     import uvloop
 
     asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
 except ModuleNotFoundError:
     pass
 
+_DECLUDE_LOOP = platform.python_version_tuple() >= ("3", "10", "0")
+
 
 class Transport:
     def __init__(self, connection):
         self._connection = connection
         self._ws_params = None
         self._conn_handler = None
         self.ws_loop = None
@@ -63,30 +66,40 @@
 
     def _set_loop_and_queue(self):
         try:
             self.ws_loop = asyncio.get_event_loop()
         except RuntimeError:
             self.ws_loop = asyncio.new_event_loop()
         asyncio.set_event_loop(self.ws_loop)
-        self.invoke_queue = asyncio.Queue(loop=self.ws_loop)
+        _queuekw = {} if _DECLUDE_LOOP else {"loop": self.ws_loop}
+        self.invoke_queue = asyncio.Queue(**_queuekw)
 
     def _connect(self):
-        self._conn_handler = asyncio.ensure_future(self._socket(self.ws_loop), loop=self.ws_loop)
+        self._conn_handler = asyncio.ensure_future(
+            self._socket(self.ws_loop), loop=self.ws_loop
+        )
 
     async def _socket(self, loop):
-        async with websockets.connect(self._ws_params.socket_url, extra_headers=self._ws_params.headers,
-                                      loop=loop) as self.ws:
+        async with websockets.connect(
+            self._ws_params.socket_url, extra_headers=self._ws_params.headers, loop=loop
+        ) as self.ws:
             self._connection.started = True
             await self._master_handler(self.ws)
 
     async def _master_handler(self, ws):
-        consumer_task = asyncio.ensure_future(self._consumer_handler(ws), loop=self.ws_loop)
-        producer_task = asyncio.ensure_future(self._producer_handler(ws), loop=self.ws_loop)
-        done, pending = await asyncio.wait([consumer_task, producer_task],
-                                           loop=self.ws_loop, return_when=asyncio.FIRST_EXCEPTION)
+        consumer_task = asyncio.ensure_future(
+            self._consumer_handler(ws), loop=self.ws_loop
+        )
+        producer_task = asyncio.ensure_future(
+            self._producer_handler(ws), loop=self.ws_loop
+        )
+        done, pending = await asyncio.wait(
+            [consumer_task, producer_task],
+            return_when=asyncio.FIRST_EXCEPTION,
+        )
 
         for task in pending:
             task.cancel()
 
     async def _consumer_handler(self, ws):
         while True:
             message = await ws.recv()
@@ -95,21 +108,21 @@
                 await self._connection.received.fire(**data)
 
     async def _producer_handler(self, ws):
         while True:
             try:
                 event = await self.invoke_queue.get()
                 if event is not None:
-                    if event.type == 'INVOKE':
+                    if event.type == "INVOKE":
                         await ws.send(dumps(event.message))
-                    elif event.type == 'CLOSE':
+                    elif event.type == "CLOSE":
                         await ws.close()
                         while ws.open is True:
                             await asyncio.sleep(0.1)
                         else:
                             self._connection.started = False
                             break
                 else:
                     break
                 self.invoke_queue.task_done()
             except Exception as e:
-                raise e
+                raise e
```

### Comparing `wsclient-0.3.0/signalr_aio_wsclient/_connection.py` & `wsclient-0.4.0/signalr_aio_wsclient/_connection.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from .events import EventHook
 from .hubs import Hub
 from .transports import Transport
 
 
 class Connection(object):
-    protocol_version = '1.5'
+    protocol_version = "1.5"
 
     def __init__(self, url, session=None):
         self.url = url
         self.__hubs = {}
         self.__send_counter = -1
         self.hub = None
         self.session = session
@@ -35,15 +35,16 @@
         self.hub = [hub_name for hub_name in self.__hubs][0]
         self.__transport.start()
 
     def register_hub(self, name):
         if name not in self.__hubs:
             if self.started:
                 raise RuntimeError(
-                    'Cannot create new hub because connection is already started.')
+                    "Cannot create new hub because connection is already started."
+                )
             self.__hubs[name] = Hub(name, self)
             return self.__hubs[name]
 
     def increment_send_counter(self):
         self.__send_counter += 1
         return self.__send_counter
```

### Comparing `wsclient-0.3.0/wsclient/base.py` & `wsclient-0.4.0/wsclient/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,590 +1,604 @@
-from .conn_mgr import ConnectionManager
-from .conn import Response
-from .sub import SubscriptionHandler
-from .merged import Merged
-from .interpreter import Interpreter
-from .channel import ChannelsInfo
-from .errors import WSError
-from .url import URLFactory
-from .extend_attrs import WSMeta
-from .transport import Transport
-
-from fons.aio import call_via_loop_afut
-from fons.dict_ops import deep_update, deep_get
-from fons.errors import TerminatedException
-from fons.event import Event
-from fons.reg import create_name
-import fons.log as _log
-
-import asyncio
-
-logger,logger2,tlogger,tloggers,tlogger0 = _log.get_standard_5(__name__)
-
-_WSCLIENT_NAMES = set()
-_ASC = ''.join(chr(i) for i in range(128))
-_ALNUM_ = ''.join(x for x in _ASC if x.isalnum()) + '_'
-_ALPHA_ = ''.join(x for x in _ASC if x.isalpha()) + '_'
-_ALNUM_DOT_ = _ALNUM_ + '.'
-_quit_command = object()
-
-
-class WSClient(metaclass=WSMeta):
-    auth_defaults = {
-        'apply_to_packs': None, #to which packs (that .encode() returns) the following applies
-                                #if None, then to all of them
-                                # example: [0,2] applies to [*pck0*, pck1 ,*pck2*]
-        'is_required': None, #if False, .sign procedure will not be invoked even if channel's "is_private" is True
-                          #if True, will not be evoked even if "is_private" is False
-        'via_url': False, #if True, authentication will not be evoked (regardless of "required" and "is_private")
-        'takes_input': True, #whether or not .sign takes .encode() output as its first argument
-        'each_time': False, #if True, then .sign procedure will be invoked each time when "is_private" is True
-                            #otherwise only if connection has not been authenticated yet (cnxi.authenticated)
-        'send_separately': False, #if True, the .sign() output is sent separately (followed by the initial message)
-        'set_authenticated': None, #if True, then cnxi.authenticated will be set only after send_separately is performed (in .tp.send)
-                                     # .sign is invoked by one of the listed channels; otherwise always
-    }
-    #Used on .subscribe_to_{x} , raises ValueError when doesn't have
-    # {
-    #    "x": True,
-    #    "y": {"_": False, "yz": True}
-    # }
-    has = {}
-    
-    channel_defaults = {
-        # If channel's url is None, this will be used (may be a function):
-        #  final_url = (url / url()).format(**self.url_compontents)
-        #  (wrapped by .cis.wrap_url(url))
-        'url': '',
-        'connection_profile': None,
-        # Whether or not .tp.send actually sends something to the cnx socket
-        # (as opposed to just connecting)
-        'send': True, # if `url` is undefined ('') then this doesn't count
-        'cnx_params_converter': None,
-        'merge_option': False,
-        'merge_limit': None, #>=2 for merge support
-        'merge_index': None, #by default 1
-        # if False, .remove_subscription raises WSError on that channel
-        'unsub_option': True,
-        # Function that is called in .subscribe_to (-> .sh.add_subscription)
-        # *may* be string (as "m$methodNameHere")
-        # *may* have a first argument for the subscription params (i.e. {'_': channel, ...})
-        'on_creation': None,
-        # Fetch necessary subscription related data shortly after 
-        # subscription becomes active
-        'fetch_data_on_sub': True,
-        # To ensure that the user won't be using out-dated data
-        # after unsubbing (unsub might also occur due to websocket crash)
-        'delete_data_on_unsub': True,
-        # change it to 1 if subscription states are not updated by server
-        'default_subscription_state': 0,
-        # Activate subscription when receives acknowledgement.
-        # Set it to "on_cnx_activation" for the sub to be activated after its cnx is activated
-        'auto_activate': True,
-        # if connection has no subscriptions left, drop it; if left to None then = `not send`
-        'drop_unused_connection': None, 
-    }
-    # If "is_private" is set to True, .sign() is called on the specific output to server
-
-    # {
-    #    "channel": {
-    #        # all listed on channel_defaults +
-    #        "required": [],
-    #        "identifiers": None,
-    #        "is_private": False,
-    # }
-    channels = {}
-    
-    max_total_subscriptions = None
-    max_total_connections = None
-    max_subscriptions_per_connection = None
-    # the interval between pushing (sending) individual subscriptions to the server
-    subscription_push_rate_limit = None
-    
-    connection_defaults = {
-        # change hub_name and hub_methods only if signalr is set to True
-        'signalr': False,
-        'hub_name': None,
-        # it is necessary to list *all* methods to avoid KeyError
-        # during signalr_aio message handling
-        'hub_methods': [],
-        'socketio': False,
-        # only event-messages that are listed here are forwarded to .handle
-        'event_names': [], # if socketio is enabled
-        'connect_timeout': None,
-        'reconnect_try_interval': 30,
-        # if current_time > last_message_recived_timestamp + recv_timeout,
-        # it assumes that the connection has been lost, and force crashes-reconnects
-        # the socket
-        'recv_timeout': None, #seconds
-        # timeout for "send" response (if expected)
-        'waiter_timeout': 5,
-        # function that returns ping message to be sent to the socket
-        # if it is a method of subclass, can be given as 'm$method_name_here'
-        # if 'ping_as_message' == False, this may be left to None
-        'ping': None,
-        # This must be overriden to activate the ping utility
-        'ping_interval': None,
-        # if specified, ping ticker only sends the message if
-        # current_time > last_message_received_timestamp + ping_after
-        'ping_after': None, #in seconds
-        # instead sending as raw bytes (via .ping of connection's socket)
-        # sends the ping as an ordinary message
-        'ping_as_message': False, # if 'dump' then the message is json encoded first
-        # Only applies if 'ping_as_message' == False, force crashes-reconnects
-        # the socket if no pong frame is received within that time
-        'ping_timeout': 5,
-        # accepts received message as first arg, returns either
-        # a) `None` if message was not ping, b) the pong message to be sent back
-        'pong': None,
-        'pong_as_message': True, # if 'dump' then the message is json encoded first
-        'poll_interval': 0.05,
-        # True, False, 'force' (logs and skips the object if it is not unpackable)
-        # ignored if `signalr` or `socketio` is enabled
-        'unpack_json': True, 
-    }
-    connection_profiles = {}
-    
-    url_components = {}
-    
-    # Since socket interpreter may clog due to high CPU usage,
-    # maximum lengths for the queues are set, and if full,
-    # previous items are removed one-by-one to make room for new ones
-    queue_maxsizes = {
-        'event': 100,
-        'received': 0,#1000,
-        'send': 100,
-    }
-    
-    message = {
-        'id': {
-            #numbers are always added, but uppers/lowers can be decluded
-            'config': {
-                'uppers': False,
-                'lowers': True,
-                'length': 14,
-                'type': 'str', #if 'int', return type will be int
-            },
-            #e.g. "id" if response = {"id": x, ...}; may be a function
-            'key':  None,
-        },
-        'error': {
-            # error is present if error_msg=deep_get([r], keyword) is in .exceptions  
-            # may be a function that extracts the msg
-            'key': None,
-            # extracted from response that you feed to the exception
-            'args_keys': [],
-        },
-    }
-    
-    # Code/message: exception class
-    exceptions = {
-        '__default__': WSError,
-    }
-    
-    # WSClient's subsclasses borrow __extend_attrs__ and __deepcopy_on__init__ from their parents,
-    # except the attrs that are prefixed with '-' (and plain '-' will omit all from parents)
-    # Example:
-    # ```
-    # class SubWSClient(WSClient):
-    #    auth_defaults = {'via_url': True}
-    #    connection_defaults = {'ping_interval': 2, 'something': 'some_value}
-    #    __extend_attrs__ = ['new_attr','-auth_defaults]
-    #    __deepcopy_on_init__ = ['new_attr_2']
-    #
-    # >>> SubWSClient.__deepcopy_on_init__ == ['new_attr_2'] + WSClient.__deepcopy_on_init__
-    # True
-    # >>> new_extend_attrs = ['new_attr'] + WSClient.__extend_attrs__
-    # >>> new_extend_attrs.remove('auth_defaults')
-    # >>> SubWSClient.__extend_attrs__ == new_extend_attrs
-    # True
-    # >>> new_connection_defaults = dict(WSClient.connection_defaults, ping_interval=2, something='some_value'}
-    # >>> SubWSClient.connection_defaults == new_connection_defaults
-    # True
-    # >>> SubWSClient.auth_defaults
-    # {'via_url': True}
-
-    # ```
-    # Now all SubWSClients attrs that are listed in its __extend_attrs__ will deep extend
-    # its parents corresponding attrs. And on __init__ all attrs listed in  __deepcopy_on__init
-    # will be deepcopied during SubWSClient.__init__ (and assigned to the resulting object)
-    __extend_attrs__ = [
-        'auth_defaults',
-        'channel_defaults',
-        'channels',
-        'connection_defaults',
-        'connection_profiles',
-        'exceptions',
-        'has',
-        'message',
-        'queue_maxsizes',
-        'url_components',
-    ]
-    __deepcopy_on_init__ = __extend_attrs__[:]
-    
-    # To be initiated during the creation of the class, and in every subclass that has its own __properties__.
-    # :: property_name, attr_name, getter_enabled(<bool>), setter_enabled, deleter_enabled
-    #    (by default all 3 are True)
-    __properties__ = [['channels_info','cis'],
-                      ['connection_manager','cm'],
-                      ['interpreter','ip'],
-                      ['subscription_handler','sh'],
-                      ['transport','tp'],]
-    
-    # Connection.recv and Connection.send run on on its own thread (message handler runs on main thread).
-    # Possibly useful to avoid handler slowing down .recv, which may cause some messages from the server to be missed.
-    #sockets_per_thread = None
-    
-    name_registry = _WSCLIENT_NAMES
-    
-    ChannelsInfo_cls = ChannelsInfo
-    ConnectionManager_cls = ConnectionManager
-    Interpreter_cls = Interpreter
-    SubscriptionHandler_cls = SubscriptionHandler
-    Transport_cls = Transport
-    
-    _verbose = 0 # 1, 2, 3
-    
-    
-    def __init__(self, config={}):
-        config = config.copy()
-        subscriptions = config.pop('subscriptions', None)  
-        
-        for key in config:
-            setattr(self, key, deep_update(getattr(self, key, None), config[key], copy=True))
-        
-        self.name = create_name(getattr(self,'name',None), self.__class__.__name__, self.name_registry)
-
-        if getattr(self,'loop',None) is None:
-            self.loop = asyncio.get_event_loop()
-            
-        self.tp = self.Transport_cls(self)
-        self._loop = self.tp._thread._loop
-        
-        self.cis = self.ChannelsInfo_cls(self)
-        self.sh = self.SubscriptionHandler_cls(self)
-        self.ip = self.Interpreter_cls(self)
-        self.cm = self.ConnectionManager_cls(self)
-        
-        self._closed = False
-        
-        self.reload_urls()
-        
-        if subscriptions is not None:
-            for params in subscriptions:
-                self.subscribe_to(params)
-        
-        #self.start.__doc__ = self.tp.start.__doc__    
-        #self.send.__doc__ = self.tp.send.__doc__
-        
-        
-    def start(self):
-        if self._closed:
-            raise TerminatedException("'{}' is closed".format(self.name))
-        
-        if asyncio.get_event_loop() is self.loop:
-            return asyncio.ensure_future(self.tp.start())
-        else:
-            return call_via_loop_afut(self.tp.start, loop=self.loop)
-    
-    
-    def on_start(self):
-        """
-        Overwrite this method. May be asynchronous.
-        Is executed as the first thing when .start() is awaited on.
-        """
-    
-    
-    def send(self, params, wait=False, id=None, cnx=None, sub=None):
-        return asyncio.ensure_future(self.tp.send(params,wait,id,cnx,sub), loop=self.loop)
-    
-    
-    def transform(self, params):
-        """
-        This is called after .sh.add_subscription(), but before (parallel) cnx_params_converter()
-        (preparing for url creation) and .encode() (sent to websocket).
-        It is also called in .tp.send(), IF plain params are sent (not Subscription / Request)
-        Params can be modified inplace OR returned as a new dict.
-        """
-    
-    
-    def encode(self, request, sub=None):
-        """
-        Overwrite this method
-        :param request: a Request / Subscription object (containing .params)
-        :param sub: if None, this is a non-subscription request. 
-                    Otherwise True for subbing and False for unsubbing.
-        :returns: output               | (non-tuple) 
-                  (output, message_id) | (tuple)
-                  .merge([pck0, pck1, ...]) where `pck` is on of the two above
-        The output will be sent to socket (but before that json encoding will be applied)
-        """
-        raise NotImplementedError
-    
-    
-    def sign(self, out={}):
-        """Authenticates the output received from .encode(). Override for specific use."""
-        return out.copy()
-    
-              
-    def extract_message_id(self, R):
-        """
-        :type R: Response
-        May want to override this method
-        """
-        r = R.data
-        key = self.message['id']['key']
-        if not isinstance(r, dict) or key is None:
-            return None
-        try:
-            if hasattr(key, '__call__'):
-                return key(r)
-            else:
-                return deep_get([r], key)
-        except Exception as e:
-            logger.error('{} - could not extract id: {}. r: {}.'.format(self.name, e, r))
-            return None
-    
-    
-    def extract_errors(self, R):
-        """
-        :type R: Response
-        :returns: list of errors
-        May want to override this method
-        """
-        r = R.data if isinstance(R, Response) else R
-        key = self.message['error']['key']
-        if not isinstance(r, dict) or key is None:
-            return []
-        
-        try:
-            if hasattr(key, '__call__'):
-                msg = key(r)
-            else:
-                msg = deep_get([r], key)
-            
-            e_cls = self.exceptions.get(msg, self.exceptions['__default__'])
-            args = self.create_error_args(r)
-            if not args:
-                args = [msg]
-            
-            errors = [e_cls(*args)]
-        
-        except Exception as e:
-            logger.error('{} - exception occurred while extracting errors: {}. r: {}.' \
-                         .format(self.name, repr(e), r))
-            logger.exception(e)
-            errors = []
-        
-        return errors
-    
-    
-    def create_error_args(self, r):
-        """
-        :returns: arguments for initiating the error
-        May want to override this method
-        """
-        args_keys = self.message['error']['args_keys']
-        if args_keys is None:
-            return []
-        args = []
-        for key in args_keys:
-            if hasattr(key, '__call__'):
-                args.append(key(r))
-            else:
-                args.append(deep_get([r], key))
-        
-        return args
-    
-    
-    def handle(self, R):
-        """:type R: Response
-          Override this for specific socket response handling. 
-          async form is also accepted. Note that if signalr is enabled,
-          R.data = raw_data (dict), not raw_data['M']['A'] (that is sent to its hub handlers)."""
-          
-    
-    def fetch_data(self, subscription, prev_state):
-        """Override this method"""
-        
-        
-    def delete_data(self, subscription, prev_state):
-        """Override this method"""
-    
-    
-    def get_dependencies(self, subscription):
-        """:returns: list of subscriptions (id_tuple, dict, ..) that are pre-required for `subscription`
-        Override this method"""
-        return []
-    
-    
-    @staticmethod
-    def merge(param_arr):
-        if isinstance(param_arr, (str, dict)) or not hasattr(param_arr, '__iter__'):
-            return param_arr
-        return Merged(param_arr)
-    
-    @staticmethod
-    def is_param_merged(x):
-        return isinstance(x, Merged)
-    
-        
-    def broadcast_event(self, event_type, value):
-        """Analogous to cnx.broadcast_event (here puts to user_event_queue)"""
-        self.tp.station.broadcast('event', Event('0', event_type, value))
-    
-    def add_event_queue(self, queue=None, maxsize=None):
-        return self.tp.add_queue('event', None, queue, maxsize)
-    
-    def add_recv_queue(self, queue=None, maxsize=None):
-        return self.tp.add_queue('recv', None, queue, maxsize)
-    
-    def remove_event_queue(self, id_or_queue):
-        return self.tp.remove_queue('event', id_or_queue)
-        
-    def remove_recv_queue(self, id_or_queue):
-        return self.tp.remove_queue('recv', id_or_queue)
-    
-    
-    async def listen(self, channel='event', queue_id=0, timeout=None):
-        """Listen for queue (default is event queue)
-           :param channel: "event" and "recv" channels are being sent to"""
-        #event queue receives ("socket","empty"), ("active",1) and ("active",0) events
-        # ("active" isn't related to cnx-s, but whether or not WSClient has pushed its subscriptions
-        #   and is ready to accept from send queue)
-        await asyncio.wait_for(self.tp.station.get_queue(channel, queue_id).wait(), timeout)
-    
-    
-    def is_running(self):
-        """Set when .start() is awaited on. Cleared when .start() finishes."""
-        return self.tp.station.get_event('running', 0, loop=0).is_set()
-    
-        
-    def is_active(self):
-        """Set after send queue starts firing. Cleared when the firing stops.
-           I.e .is_active()==True means that .send method is currently usable."""
-        return self.tp.station.get_event('active', 0, loop=0).is_set()
-    
-    
-    async def wait_till_active(self, timeout=None):
-        if self._closed:
-            raise TerminatedException('{} is closed'.format(self.name))
-        #self.station._print()
-        #print({'loop': id(self.loop), 'out_loop': id(self.out_loop), 'context': id(asyncio.get_event_loop())})
-        event = self.tp.station.get_event('active', 0)
-        await asyncio.wait_for(event.wait(), timeout)
-        
-    
-    def stop(self):
-        if asyncio.get_event_loop() is self.loop:
-            return asyncio.ensure_future(self.tp.stop())
-        else:
-            return call_via_loop_afut(self.tp.stop, loop=self.loop)
-    
-    def close(self):
-        if self._closed:
-            return
-        self._closed = True
-        self.stop()
-    
-    
-    def reload_urls(self):
-        for ch_values in list(self.channels.values()) + [self.channel_defaults]:
-            if ch_values.get('url') is not None:
-                ch_values['url_factory'] = URLFactory(self, ch_values['url'])
-            cpc = ch_values.get('cnx_params_converter')
-            if isinstance(cpc, str):
-                if cpc.startswith('m$'): cpc = cpc[2:]
-                ch_values['cnx_params_converter'] = getattr(self, cpc)
-    
-    
-    def subscribe_to(self, params):
-        return self.sh.add_subscription(params)
-    
-    def unsubscribe_to(self, x):
-        return self.sh.remove_subscription(x)
-    
-    
-    def _log(self, msg, level='DEBUG', logger=logger, add_name=True):
-        if not isinstance(msg, Exception):
-            if add_name:
-                msg = '{} - {}'.format(self.name, msg)
-            logger.log(_log.level_to_int(level), msg)
-        else:
-            logger.exception(msg)
-    
-    
-    def log(self, msg, level='DEBUG', logger=logger, add_name=True):
-        if self.verbose and self.verbose >= 1:
-            self._log(msg, level, logger, add_name)
-    
-    
-    def log2(self, msg, level='DEBUG', logger=logger, add_name=True):
-        if self.verbose and self.verbose >= 2:
-            self._log(msg, level, logger, add_name)
-    
-    
-    def log3(self, msg, level='DEBUG', logger=logger, add_name=True):
-        if self.verbose and self.verbose >= 3:
-            self._log(msg, level, logger, add_name)
-    
-    
-    @property
-    def subscriptions(self):
-        return self.sh.subscriptions[:]
-    @property
-    def has_got(self):
-        return self.cis.has_got
-    @property
-    def has_merge_option(self):
-        return self.cis.has_merge_option
-    @property
-    def get_merge_limit(self):
-        return self.cis.get_merge_limit
-    @property
-    def has_unsub_option(self):
-        return self.cis.has_unsub_option
-    @property
-    def verify_has(self):
-        return self.cis.verify_has
-    @property
-    def sub_to(self):
-        return self.subscribe_to
-    @property
-    def unsub_to(self):
-        return self.unsubscribe_to
-    @property
-    def is_subscribed_to(self):
-        return self.sh.is_subscribed_to
-    @property
-    def handle_subscription_ack(self):
-        return self.sh.handle_subscription_ack
-    @property
-    def get_subscription(self):
-        return self.sh.get_subscription
-    @property
-    def change_subscription_state(self):
-        return self.sh.change_subscription_state
-    @property
-    def wait_till_subscription_active(self):
-        return self.sh.wait_till_subscription_active
-    @property
-    def get_value(self):
-        return self.cis.get_value
-    #@property
-    #def get_connection(self):
-    #    return self.sh.find_available_connection
-    @property
-    def generate_message_id(self):
-        return self.ip.generate_message_id
-    @property
-    def station(self):
-        return self.tp.station
-    @property
-    def verbose(self):
-        return self._verbose
-    @verbose.setter
-    def verbose(self, value):
-        self._verbose = value
-        if getattr(self, 'cm', None) is not None:
-            for cnx in self.cm.connections.values():
-                cnx.verbose = value
+from .conn_mgr import ConnectionManager
+from .conn import Response
+from .sub import SubscriptionHandler
+from .merged import Merged
+from .interpreter import Interpreter
+from .channel import ChannelsInfo
+from .errors import WSError
+from .url import URLFactory
+from .extend_attrs import WSMeta
+from .transport import Transport
+
+from fons.aio import call_via_loop_afut
+from fons.dict_ops import deep_update, deep_get
+from fons.errors import TerminatedException
+from fons.event import Event
+from fons.reg import create_name
+import fons.log as _log
+
+import asyncio
+
+logger, logger2, tlogger, tloggers, tlogger0 = _log.get_standard_5(__name__)
+
+_WSCLIENT_NAMES = set()
+_ASC = "".join(chr(i) for i in range(128))
+_ALNUM_ = "".join(x for x in _ASC if x.isalnum()) + "_"
+_ALPHA_ = "".join(x for x in _ASC if x.isalpha()) + "_"
+_ALNUM_DOT_ = _ALNUM_ + "."
+_quit_command = object()
+
+
+class WSClient(metaclass=WSMeta):
+    auth_defaults = {
+        "apply_to_packs": None,  # to which packs (that .encode() returns) the following applies
+        # if None, then to all of them
+        # example: [0,2] applies to [*pck0*, pck1 ,*pck2*]
+        "is_required": None,  # if False, .sign procedure will not be invoked even if channel's "is_private" is True
+        # if True, will not be evoked even if "is_private" is False
+        "via_url": False,  # if True, authentication will not be evoked (regardless of "required" and "is_private")
+        "takes_input": True,  # whether or not .sign takes .encode() output as its first argument
+        "each_time": False,  # if True, then .sign procedure will be invoked each time when "is_private" is True
+        # otherwise only if connection has not been authenticated yet (cnxi.authenticated)
+        "send_separately": False,  # if True, the .sign() output is sent separately (followed by the initial message)
+        "set_authenticated": None,  # if True, then cnxi.authenticated will be set only after send_separately is performed (in .tp.send)
+        # .sign is invoked by one of the listed channels; otherwise always
+    }
+    # Used on .subscribe_to_{x} , raises ValueError when doesn't have
+    # {
+    #    "x": True,
+    #    "y": {"_": False, "yz": True}
+    # }
+    has = {}
+
+    channel_defaults = {
+        # If channel's url is None, this will be used (may be a function):
+        #  final_url = (url / url()).format(**self.url_compontents)
+        #  (wrapped by .cis.wrap_url(url))
+        "url": "",
+        "connection_profile": None,
+        # Whether or not .tp.send actually sends something to the cnx socket
+        # (as opposed to just connecting)
+        "send": True,  # if `url` is undefined ('') then this doesn't count
+        "cnx_params_converter": None,
+        "merge_option": False,
+        "merge_limit": None,  # >=2 for merge support
+        "merge_index": None,  # by default 1
+        # if False, .remove_subscription raises WSError on that channel
+        "unsub_option": True,
+        # Function that is called in .subscribe_to (-> .sh.add_subscription)
+        # *may* be string (as "m$methodNameHere")
+        # *may* have a first argument for the subscription params (i.e. {'_': channel, ...})
+        "on_creation": None,
+        # Fetch necessary subscription related data shortly after
+        # subscription becomes active
+        "fetch_data_on_sub": True,
+        # To ensure that the user won't be using out-dated data
+        # after unsubbing (unsub might also occur due to websocket crash)
+        "delete_data_on_unsub": True,
+        # change it to 1 if subscription states are not updated by server
+        "default_subscription_state": 0,
+        # Activate subscription when receives acknowledgement.
+        # Set it to "on_cnx_activation" for the sub to be activated after its cnx is activated
+        "auto_activate": True,
+        # if connection has no subscriptions left, drop it; if left to None then = `not send`
+        "drop_unused_connection": None,
+    }
+    # If "is_private" is set to True, .sign() is called on the specific output to server
+
+    # {
+    #    "channel": {
+    #        # all listed on channel_defaults +
+    #        "required": [],
+    #        "identifiers": None,
+    #        "is_private": False,
+    # }
+    channels = {}
+
+    max_total_subscriptions = None
+    max_total_connections = None
+    max_subscriptions_per_connection = None
+    # the interval between pushing (sending) individual subscriptions to the server
+    subscription_push_rate_limit = None
+
+    connection_defaults = {
+        # change hub_name and hub_methods only if signalr is set to True
+        "signalr": False,
+        "hub_name": None,
+        # it is necessary to list *all* methods to avoid KeyError
+        # during signalr_aio message handling
+        "hub_methods": [],
+        "socketio": False,
+        # only event-messages that are listed here are forwarded to .handle
+        "event_names": [],  # if socketio is enabled
+        "connect_timeout": None,
+        "reconnect_try_interval": 30,  # when connect fails try again after X seconds
+        # if current_time > last_message_recived_timestamp + recv_timeout,
+        # it assumes that the connection has been lost, and force crashes-reconnects
+        # the socket
+        "recv_timeout": None,  # seconds
+        # timeout for "send" response (if expected)
+        "waiter_timeout": 5,
+        # function that returns ping message to be sent to the socket
+        # if it is a method of subclass, can be given as 'm$method_name_here'
+        # if 'ping_as_message' == False, this may be left to None
+        "ping": None,
+        # This must be overriden to activate the ping utility
+        "ping_interval": None,
+        # if specified, ping ticker only sends the message if
+        # current_time > last_message_received_timestamp + ping_after
+        "ping_after": None,  # in seconds
+        # instead sending as raw bytes (via .ping of connection's socket)
+        # sends the ping as an ordinary message
+        "ping_as_message": False,  # if 'dump' then the message is json encoded first
+        # Only applies if 'ping_as_message' == False, force crashes-reconnects
+        # the socket if no pong frame is received within that time
+        "ping_timeout": 5,
+        # accepts received message as first arg, returns either
+        # a) `None` if message was not ping, b) the pong message to be sent back
+        "pong": None,
+        "pong_as_message": True,  # if 'dump' then the message is json encoded first
+        "poll_interval": 0.05,
+        # max number of requests per second / per seconds of interval
+        "rate_limit": None,  # nb_requests or (nb_request, seconds)
+        # logged when rate_limit is hit
+        "throttle_logging_level": 0,  # 0 - 50 ('DEBUG' - 'CRITICAL')
+        # True, False, 'force' (logs and skips the object if it is not unpackable)
+        # ignored if `signalr` or `socketio` is enabled
+        "unpack_json": True,
+    }
+    connection_profiles = {}
+
+    url_components = {}
+
+    # Since socket interpreter may clog due to high CPU usage,
+    # maximum lengths for the queues are set, and if full,
+    # previous items are removed one-by-one to make room for new ones
+    queue_maxsizes = {
+        "event": 100,
+        "received": 0,  # 1000,
+        "send": 100,
+    }
+
+    message = {
+        "id": {
+            # numbers are always added, but uppers/lowers can be decluded
+            "config": {
+                "uppers": False,
+                "lowers": True,
+                "length": 14,
+                "type": "str",  # if 'int', return type will be int
+            },
+            # e.g. "id" if response = {"id": x, ...}; may be a function
+            "key": None,
+        },
+        "error": {
+            # error is present if error_msg=deep_get([r], keyword) is in .exceptions
+            # may be a function that extracts the msg
+            "key": None,
+            # extracted from response that you feed to the exception
+            "args_keys": [],
+        },
+    }
+
+    # Code/message: exception class
+    exceptions = {
+        "__default__": WSError,
+    }
+
+    # WSClient's subsclasses borrow __extend_attrs__ and __deepcopy_on__init__ from their parents,
+    # except the attrs that are prefixed with '-' (and plain '-' will omit all from parents)
+    # Example:
+    # ```
+    # class SubWSClient(WSClient):
+    #    auth_defaults = {'via_url': True}
+    #    connection_defaults = {'ping_interval': 2, 'something': 'some_value}
+    #    __extend_attrs__ = ['new_attr','-auth_defaults]
+    #    __deepcopy_on_init__ = ['new_attr_2']
+    #
+    # >>> SubWSClient.__deepcopy_on_init__ == ['new_attr_2'] + WSClient.__deepcopy_on_init__
+    # True
+    # >>> new_extend_attrs = ['new_attr'] + WSClient.__extend_attrs__
+    # >>> new_extend_attrs.remove('auth_defaults')
+    # >>> SubWSClient.__extend_attrs__ == new_extend_attrs
+    # True
+    # >>> new_connection_defaults = dict(WSClient.connection_defaults, ping_interval=2, something='some_value'}
+    # >>> SubWSClient.connection_defaults == new_connection_defaults
+    # True
+    # >>> SubWSClient.auth_defaults
+    # {'via_url': True}
+
+    # ```
+    # Now all SubWSClients attrs that are listed in its __extend_attrs__ will deep extend
+    # its parents corresponding attrs. And on __init__ all attrs listed in  __deepcopy_on__init
+    # will be deepcopied during SubWSClient.__init__ (and assigned to the resulting object)
+    __extend_attrs__ = [
+        "auth_defaults",
+        "channel_defaults",
+        "channels",
+        "connection_defaults",
+        "connection_profiles",
+        "exceptions",
+        "has",
+        "message",
+        "queue_maxsizes",
+        "url_components",
+    ]
+    __deepcopy_on_init__ = __extend_attrs__[:]
+
+    # To be initiated during the creation of the class, and in every subclass that has its own __properties__.
+    # :: property_name, attr_name, getter_enabled(<bool>), setter_enabled, deleter_enabled
+    #    (by default all 3 are True)
+    __properties__ = [
+        ["channels_info", "cis"],
+        ["connection_manager", "cm"],
+        ["interpreter", "ip"],
+        ["subscription_handler", "sh"],
+        ["transport", "tp"],
+    ]
+
+    # Connection.recv and Connection.send run on on its own thread (message handler runs on main thread).
+    # Possibly useful to avoid handler slowing down .recv, which may cause some messages from the server to be missed.
+    # sockets_per_thread = None
+
+    name_registry = _WSCLIENT_NAMES
+
+    ChannelsInfo_cls = ChannelsInfo
+    ConnectionManager_cls = ConnectionManager
+    Interpreter_cls = Interpreter
+    SubscriptionHandler_cls = SubscriptionHandler
+    Transport_cls = Transport
+
+    _verbose = 0  # 1, 2, 3
+
+    def __init__(self, config={}):
+        config = config.copy()
+        subscriptions = config.pop("subscriptions", None)
+
+        for key in config:
+            setattr(
+                self, key, deep_update(getattr(self, key, None), config[key], copy=True)
+            )
+
+        self.name = create_name(
+            getattr(self, "name", None), self.__class__.__name__, self.name_registry
+        )
+
+        if getattr(self, "loop", None) is None:
+            self.loop = asyncio.get_event_loop()
+
+        self.tp = self.Transport_cls(self)
+        self._loop = self.tp._thread._loop
+
+        self.cis = self.ChannelsInfo_cls(self)
+        self.sh = self.SubscriptionHandler_cls(self)
+        self.ip = self.Interpreter_cls(self)
+        self.cm = self.ConnectionManager_cls(self)
+
+        self._closed = False
+
+        self.reload_urls()
+
+        if subscriptions is not None:
+            for params in subscriptions:
+                self.subscribe_to(params)
+
+        # self.start.__doc__ = self.tp.start.__doc__
+        # self.send.__doc__ = self.tp.send.__doc__
+
+    def start(self):
+        if self._closed:
+            raise TerminatedException("'{}' is closed".format(self.name))
+
+        if asyncio.get_event_loop() is self.loop:
+            return asyncio.ensure_future(self.tp.start())
+        else:
+            return call_via_loop_afut(self.tp.start, loop=self.loop)
+
+    def on_start(self):
+        """
+        Overwrite this method. May be asynchronous.
+        Is executed as the first thing when .start() is awaited on.
+        """
+
+    def send(self, params, wait=False, id=None, cnx=None, sub=None):
+        return asyncio.ensure_future(
+            self.tp.send(params, wait, id, cnx, sub), loop=self.loop
+        )
+
+    def transform(self, params):
+        """
+        This is called after .sh.add_subscription(), but before (parallel) cnx_params_converter()
+        (preparing for url creation) and .encode() (sent to websocket).
+        It is also called in .tp.send(), IF plain params are sent (not Subscription / Request)
+        Params can be modified inplace OR returned as a new dict.
+        """
+
+    def encode(self, request, sub=None):
+        """
+        Overwrite this method
+        :param request: a Request / Subscription object (containing .params)
+        :param sub: if None, this is a non-subscription request.
+                    Otherwise True for subbing and False for unsubbing.
+        :returns: output               | (non-tuple)
+                  (output, message_id) | (tuple)
+                  .merge([pck0, pck1, ...]) where `pck` is on of the two above
+        The output will be sent to socket (but before that json encoding will be applied)
+        """
+        raise NotImplementedError
+
+    def sign(self, out={}):
+        """Authenticates the output received from .encode(). Override for specific use."""
+        return out.copy()
+
+    def extract_message_id(self, R):
+        """
+        :type R: Response
+        May want to override this method
+        """
+        r = R.data
+        key = self.message["id"]["key"]
+        if not isinstance(r, dict) or key is None:
+            return None
+        try:
+            if hasattr(key, "__call__"):
+                return key(r)
+            else:
+                return deep_get([r], key)
+        except Exception as e:
+            logger.error(
+                "{} - could not extract id: {}. r: {}.".format(self.name, e, r)
+            )
+            return None
+
+    def extract_errors(self, R):
+        """
+        :type R: Response
+        :returns: list of errors
+        May want to override this method
+        """
+        r = R.data if isinstance(R, Response) else R
+        key = self.message["error"]["key"]
+        if not isinstance(r, dict) or key is None:
+            return []
+
+        try:
+            if hasattr(key, "__call__"):
+                msg = key(r)
+            else:
+                msg = deep_get([r], key)
+
+            e_cls = self.exceptions.get(msg, self.exceptions["__default__"])
+            args = self.create_error_args(r)
+            if not args:
+                args = [msg]
+
+            errors = [e_cls(*args)]
+
+        except Exception as e:
+            logger.error(
+                "{} - exception occurred while extracting errors: {}. r: {}.".format(
+                    self.name, repr(e), r
+                )
+            )
+            logger.exception(e)
+            errors = []
+
+        return errors
+
+    def create_error_args(self, r):
+        """
+        :returns: arguments for initiating the error
+        May want to override this method
+        """
+        args_keys = self.message["error"]["args_keys"]
+        if args_keys is None:
+            return []
+        args = []
+        for key in args_keys:
+            if hasattr(key, "__call__"):
+                args.append(key(r))
+            else:
+                args.append(deep_get([r], key))
+
+        return args
+
+    def handle(self, R):
+        """:type R: Response
+        Override this for specific socket response handling.
+        async form is also accepted. Note that if signalr is enabled,
+        R.data = raw_data (dict), not raw_data['M']['A'] (that is sent to its hub handlers).
+        """
+
+    def fetch_data(self, subscription, prev_state):
+        """Override this method"""
+
+    def delete_data(self, subscription, prev_state):
+        """Override this method"""
+
+    def get_dependencies(self, subscription):
+        """:returns: list of subscriptions (id_tuple, dict, ..) that are pre-required for `subscription`
+        Override this method"""
+        return []
+
+    @staticmethod
+    def merge(param_arr):
+        if isinstance(param_arr, (str, dict)) or not hasattr(param_arr, "__iter__"):
+            return param_arr
+        return Merged(param_arr)
+
+    @staticmethod
+    def is_param_merged(x):
+        return isinstance(x, Merged)
+
+    def broadcast_event(self, event_type, value):
+        """Analogous to cnx.broadcast_event (here puts to user_event_queue)"""
+        self.tp.station.broadcast("event", Event("0", event_type, value))
+
+    def add_event_queue(self, queue=None, maxsize=None):
+        return self.tp.add_queue("event", None, queue, maxsize)
+
+    def add_recv_queue(self, queue=None, maxsize=None):
+        return self.tp.add_queue("recv", None, queue, maxsize)
+
+    def remove_event_queue(self, id_or_queue):
+        return self.tp.remove_queue("event", id_or_queue)
+
+    def remove_recv_queue(self, id_or_queue):
+        return self.tp.remove_queue("recv", id_or_queue)
+
+    async def listen(self, channel="event", queue_id=0, timeout=None):
+        """Listen for queue (default is event queue)
+        :param channel: "event" and "recv" channels are being sent to"""
+        # event queue receives ("socket","empty"), ("active",1) and ("active",0) events
+        # ("active" isn't related to cnx-s, but whether or not WSClient has pushed its subscriptions
+        #   and is ready to accept from send queue)
+        await asyncio.wait_for(
+            self.tp.station.get_queue(channel, queue_id).wait(), timeout
+        )
+
+    def is_running(self):
+        """Set when .start() is awaited on. Cleared when .start() finishes."""
+        return self.tp.station.get_event("running", 0, loop=0).is_set()
+
+    def is_active(self):
+        """Set after send queue starts firing. Cleared when the firing stops.
+        I.e .is_active()==True means that .send method is currently usable."""
+        return self.tp.station.get_event("active", 0, loop=0).is_set()
+
+    async def wait_till_active(self, timeout=None):
+        if self._closed:
+            raise TerminatedException("{} is closed".format(self.name))
+        # self.station._print()
+        # print({'loop': id(self.loop), 'out_loop': id(self.out_loop), 'context': id(asyncio.get_event_loop())})
+        event = self.tp.station.get_event("active", 0)
+        await asyncio.wait_for(event.wait(), timeout)
+
+    def stop(self):
+        if asyncio.get_event_loop() is self.loop:
+            return asyncio.ensure_future(self.tp.stop())
+        else:
+            return call_via_loop_afut(self.tp.stop, loop=self.loop)
+
+    def close(self):
+        if self._closed:
+            return
+        self._closed = True
+        self.stop()
+
+    def reload_urls(self):
+        for ch_values in list(self.channels.values()) + [self.channel_defaults]:
+            if ch_values.get("url") is not None:
+                ch_values["url_factory"] = URLFactory(self, ch_values["url"])
+            cpc = ch_values.get("cnx_params_converter")
+            if isinstance(cpc, str):
+                if cpc.startswith("m$"):
+                    cpc = cpc[2:]
+                ch_values["cnx_params_converter"] = getattr(self, cpc)
+
+    def subscribe_to(self, params):
+        return self.sh.add_subscription(params)
+
+    def unsubscribe_to(self, x):
+        return self.sh.remove_subscription(x)
+
+    def _log(self, msg, level="DEBUG", logger=logger, add_name=True):
+        if not isinstance(msg, Exception):
+            if add_name:
+                msg = "{} - {}".format(self.name, msg)
+            logger.log(_log.level_to_int(level), msg)
+        else:
+            logger.exception(msg)
+
+    def log(self, msg, level="DEBUG", logger=logger, add_name=True):
+        if self.verbose and self.verbose >= 1:
+            self._log(msg, level, logger, add_name)
+
+    def log2(self, msg, level="DEBUG", logger=logger, add_name=True):
+        if self.verbose and self.verbose >= 2:
+            self._log(msg, level, logger, add_name)
+
+    def log3(self, msg, level="DEBUG", logger=logger, add_name=True):
+        if self.verbose and self.verbose >= 3:
+            self._log(msg, level, logger, add_name)
+
+    @property
+    def subscriptions(self):
+        return self.sh.subscriptions[:]
+
+    @property
+    def has_got(self):
+        return self.cis.has_got
+
+    @property
+    def has_merge_option(self):
+        return self.cis.has_merge_option
+
+    @property
+    def get_merge_limit(self):
+        return self.cis.get_merge_limit
+
+    @property
+    def has_unsub_option(self):
+        return self.cis.has_unsub_option
+
+    @property
+    def verify_has(self):
+        return self.cis.verify_has
+
+    @property
+    def sub_to(self):
+        return self.subscribe_to
+
+    @property
+    def unsub_to(self):
+        return self.unsubscribe_to
+
+    @property
+    def is_subscribed_to(self):
+        return self.sh.is_subscribed_to
+
+    @property
+    def handle_subscription_ack(self):
+        return self.sh.handle_subscription_ack
+
+    @property
+    def get_subscription(self):
+        return self.sh.get_subscription
+
+    @property
+    def change_subscription_state(self):
+        return self.sh.change_subscription_state
+
+    @property
+    def wait_till_subscription_active(self):
+        return self.sh.wait_till_subscription_active
+
+    @property
+    def wait_till_subscriptions_active(self):
+        return self.sh.wait_till_subscriptions_active
+
+    @property
+    def get_value(self):
+        return self.cis.get_value
+
+    # @property
+    # def get_connection(self):
+    #    return self.sh.find_available_connection
+    @property
+    def generate_message_id(self):
+        return self.ip.generate_message_id
+
+    @property
+    def station(self):
+        return self.tp.station
+
+    @property
+    def verbose(self):
+        return self._verbose
+
+    @verbose.setter
+    def verbose(self, value):
+        self._verbose = value
+        if getattr(self, "cm", None) is not None:
+            for cnx in self.cm.connections.values():
+                cnx.verbose = value
```

### Comparing `wsclient-0.3.0/wsclient/conn.py` & `wsclient-0.4.0/wsclient/conn.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,708 +1,784 @@
-import websockets
-import signalr_aio_wsclient as signalr_aio
-import socketio
-import sys
-import json
-import asyncio
-import inspect
-import time
-import datetime
-dt = datetime.datetime
-td = datetime.timedelta
-
-from fons.aio import call_via_loop_afut
-from fons.debug import (safeTry, safeAsyncTry)
-
-from fons.event import (Station, Event, force_put,
-                        empty_queue, create_name)
-from fons.func import (async_limitcalls, get_arg_count)
-from fons.sched import AsyncTicker
-import fons.log as _log
-
-logger,logger2,tlogger,tloggers,tlogger0 = _log.get_standard_5(__name__)
-
-
-_CONNECTION_IDS = set()
-_CONNECTION_NAMES = set()
-_stop_command = object()
-_heartbeat = object()
-
-
-class Connection:
-    def __init__(self, url, handle=None,*, on_activate=None,
-                 signalr=False, hub_name=None, hub_methods=None,
-                 socketio=False, event_names=None,
-                 reconnect_try_interval=None, connect_timeout=None, recv_timeout=None, 
-                 ping_interval=None, ping=None, ping_after=None, ping_timeout=5,
-                 ping_as_message=False, pong=None, pong_as_message=True,
-                 rate_limit=None, poll_interval=None,
-                 queue_maxsizes={}, recv_queue=None, event_queue=None,
-                 id=None, name_prefix=None, loop=None, out_loop=None, throttle_logging_level=0,
-                 extra_headers=None, unpack_json=True, verbose=0):
-        """
-        :param url: str or (coroutine) function that returns str
-        :param handle: (sync) function or list of functions (or None)
-        :param on_activate: (a)sync function or list of functions (or None)
-        :param out_loop: for station events and queues (recv [received] queue, event queue)
-        :param extra_headers: (coroutine) function that returns dict
-        :param unpack_json:
-            True, False, 'force' (logs and skips the object if it it is not unpackable)
-            ignored if  `socketio` or `signalr` is enabled
-                            
-        """
-        if signalr and socketio:
-            raise ValueError('`signalr` and `socketio` can\'t be simultaneously True')
-        if ping_interval is not None and not ping_as_message and (signalr or socketio):
-            which = 'signalr' if signalr else 'socketio'
-            raise ValueError('Cannot send raw ping frames if `{}` is set to True. ' \
-                             'You could enable `ping_as_message` instead.'.format(which))
-        if pong and not pong_as_message and (signalr or socketio):
-            which = 'signalr' if signalr else 'socketio'
-            raise ValueError('Cannot send raw pong frames if `{}` is set to True. ' \
-                             'You could enable `pong_as_message` instead.'.format(which))
-        if isinstance(ping_as_message, str) and ping_as_message!='dump':
-            raise ValueError(ping_as_message)
-        if isinstance(pong_as_message, str) and pong_as_message!='dump':
-            raise ValueError(pong_as_message)
-        self.url = url
-        self.extra_headers = extra_headers
-        self.handle = handle
-        self.on_activate = on_activate
-        self.verbose = verbose
-        #if id is None, returns free connection number (as str)
-        self.id = create_name(id, None, registry=_CONNECTION_IDS)
-        #default_name is used (and int added to that if already taken)
-        default_name = '{}-{}'.format(self.__class__.__name__ if name_prefix is None 
-                                      else name_prefix, self.id)
-        self.name = create_name(None, default_name, _CONNECTION_NAMES, add_int='if_taken')
-        
-        self.socketio = socketio
-        self.signalr = signalr
-        self.hub_name = hub_name
-        self.hub_methods = hub_methods if hub_methods is not None else []
-        self.event_names = event_names if event_names is not None else []
-        self.conn = None
-        self.socket = None
-        self.hub = None
-        self.loop = loop if loop is not None else asyncio.get_event_loop()
-        q = next((x for x in (recv_queue,event_queue) if x is not None), None)
-        if out_loop is None and q is not None:
-            out_loop = q._loop
-        self.out_loop = out_loop if out_loop is not None else self.loop
-        
-        self.connect_timeout = connect_timeout
-        self.recv_timeout = recv_timeout
-        self.reconnect_try_interval = reconnect_try_interval
-        self.poll_interval = poll_interval
-        self.throttle_logging_level = throttle_logging_level
-        self._throttle_original = self._throttle
-        self.rate_limit = rate_limit
-        
-        self.ping_func = ping
-        self.ping_interval = ping_interval
-        self.ping_after = ping_after
-        self.ping_as_message = ping_as_message
-        self.ping_timeout = ping_timeout
-        self.ping_ticker = None
-        self.pong_func = pong
-        self.pong_as_message = pong_as_message
-        
-        self.unpack_json = unpack_json
-        
-        self.station = Station(loops = {-1: self.loop, 
-                                         0: self.out_loop},
-                               name = self.name+'[Station]')
-       
-        station_channels = ['started','active','stopped','_stop_initiated','empty','event','recv']
-        for ch in station_channels:
-            self.station.add_channel(ch)
-        for ch in ['started','active','stopped','_stop_initiated','empty']:
-            self.station.add_event(ch, id=0)
-            
-        def _add_q(ch, q_id, queue):
-            maxsizes = {'event': 100}
-            #only add to out_loop
-            loops = [0] if queue is None else [queue._loop]
-            self.station.add_queue(ch, q_id, queue,
-                                   maxsize = queue_maxsizes.get(ch, maxsizes.get(ch,0)),
-                                   loops = loops)
-            
-        for ch,q in [['recv', recv_queue],
-                     ['event', event_queue]]:
-            if isinstance(q,dict):
-                for i,_q in q.items():
-                    _add_q(ch,i,_q)
-            elif hasattr(q,'__iter__'):
-                for i,_q in enumerate(q):
-                    _add_q(ch,i,_q)
-            else:
-                _add_q(ch,0,q)
-
-        self._queues = {}
-        self.futures = dict.fromkeys(['start', 'stop', 'ping', 'recv_loop', 
-                                      'on_activate', 'signalr_wait'])
-        self.connected_url = None
-        self.connected_ts = None
-        self.last_recv_ts = None
-        self._last_ping_ts = None
-        self._ignore_recv_ts = False
-        self._stopped = False
-    
-    
-    async def _connect(self):
-        suffix = ' (socketio)' if self.socketio else (' (signalr)' if self.signalr else '')
-        self.log("connecting{}".format(suffix))
-        params = {}
-        
-        url = self.url
-        if hasattr(self.url,'__call__'):
-            url = url()
-        if inspect.isawaitable(url):
-            url = await url
-        
-        headers_from_url = {}
-        if isinstance(url, dict):
-            _headers = url.get('extra_headers')
-            if _headers is not None:
-                headers_from_url.update(_headers)
-            url = url['url']
-        url_msg = 'url: {}'.format(url) if url!='' else 'url empty'
-        self.log(url_msg)
-        
-        extra_headers = self.extra_headers
-        if hasattr(extra_headers,'__call__'):
-            extra_headers = extra_headers()
-        if inspect.isawaitable(extra_headers):
-            extra_headers = await extra_headers
-        
-        if extra_headers is None:
-            extra_headers = {}
-        
-        final_headers = dict(extra_headers, **headers_from_url)
-        if final_headers:
-            params['extra_headers'] = final_headers
-        
-        if not url:
-            pass
-        elif self.signalr:
-            await self._connect_signalr(url)
-        elif self.socketio:
-            await self._connect_socketio(url)
-        else:
-            await self._connect_ordinary(url, params)
-        
-        self.log("connection established")
-        self.connected_url = url
-        self.connected_ts = time.time()
-        #self.socket.settimeout(self.timeout)
-    
-    
-    async def _connect_ordinary(self, url, params={}):
-        self.conn = websockets.connect(url, **params)
-        self.socket = await self.conn.__aenter__() # this also execs logging.basicConfig
-        q = self._socket_recv_queue
-        
-        async def recv_loop():
-            while True:
-                try: r = await self.socket.recv()
-                except websockets.ConnectionClosed as e:
-                    force_put(q, e)
-                    break
-                else: force_put(q, r)
-
-        self.futures['recv_loop'] = \
-            asyncio.ensure_future(recv_loop())
-    
-    
-    async def _connect_signalr(self, url):
-        self.conn = signalr_aio.Connection(url, session=None)
-        self.hub = self.conn.register_hub(self.hub_name)
-        #All data received from server is handled by .handle,
-        # hub specific handling is not implemented
-        async def do_nothing(msg):
-            pass
-        for method in self.hub_methods:
-            self.hub.client.on(method, do_nothing)
-        #messages to .recv are forwarded via signal_recv_queue
-        q = self._socket_recv_queue
-        async def put_to_recv_queue(**data):
-            await q.put(data)
-            
-        self.conn.received += put_to_recv_queue
-        self.conn.start()
-        
-        signalr_fut = self.conn._Connection__transport._conn_handler
-        await asyncio.wait([signalr_fut], timeout=0.5)
-        if signalr_fut.done():
-            await signalr_fut # raises exception if occurred
-        
-        async def wait_on_signalr_future():
-            try:
-                await signalr_fut
-            except websockets.ConnectionClosed as e:
-                self.log('signalr socket has crashed')
-                await q.put(e)
-            else:
-                self.log('signalr socket has been closed')
-                await q.put(websockets.ConnectionClosed(-1, 'signalr ws closed'))
-                
-        self.futures['signalr_wait'] = asyncio.ensure_future(wait_on_signalr_future())
-    
-    
-    async def _connect_socketio(self, url):
-        self.conn = sio = socketio.AsyncClient(reconnection=False)
-        #messages to .recv are forwarded via signal_recv_queue
-        q = self._socket_recv_queue
-        connected = asyncio.Event()
-        
-        async def message(data):
-            await q.put(data)
-        
-        for event in self.event_names:
-            sio.on(event)(message)
-        
-        @sio.event
-        async def connect():
-            connected.set()
-        
-        @sio.event
-        async def connect_error(*args):
-            self.log('socketio encountered connect error')
-            await q.put(websockets.ConnectionClosed(-1, 'socketio connect error'))
-        
-        # This isn't executed when user itself evokes sio.disconnect (or here Connection.stop())
-        @sio.event
-        async def disconnect():
-            self.log('socketio connection has crashed')
-            await q.put(websockets.ConnectionClosed(-1, 'socketio ws crashed'))
-        
-        await sio.connect(url, transports='websocket')
-        await connected.wait()
-    
-    
-    async def _activate(self, timeout=None):
-        # Close any previous connection if by chance left open (though it shouldn't happen)
-        await self._exit_conn() 
-        # Renew the queue to ensure that we won't be receiving anything from previous sockets
-        # TODO: set max size to this queue?
-        self._socket_recv_queue = asyncio.Queue(loop=self.loop)
-        self.conn = None
-        fut = asyncio.ensure_future(self._connect())
-        wait_started = time.time()
-        is_exceeded = lambda: timeout is not None and time.time() - wait_started > timeout
-        while not self._stopped and not is_exceeded() and not fut.done():
-            await asyncio.wait([fut], timeout=0.1)
-        to_occurred = is_exceeded()
-        if fut.done():
-            await fut # raise exception if occurred
-        else:
-            fut.cancel()
-            await self._exit_conn()
-            if to_occurred:
-                raise asyncio.TimeoutError('{} - connect timeout occurred'.format(self.name))
-        if self._stopped:
-            return
-        self.station.broadcast('active')
-        self.broadcast_event('socket', 1)
-        if self.on_activate is not None:
-            on_activate = [self.on_activate] if not hasattr(self.on_activate, '__iter__') \
-                             else self.on_activate
-            for i,f in enumerate(on_activate):
-                args = [self] if get_arg_count(f) else []
-                key = 'on_activate{}'.format('_{}'.format(i) if i else '')
-                self.futures[key] = call_via_loop_afut(f, args)
-    
-    
-    async def _safe_activate(self, timeout=None):
-        await safeAsyncTry(self._activate, (timeout,), attempts=True,
-                           pause=self.reconnect_try_interval,
-                           exit_on=self.station.get_event('_stop_initiated',0,loop=-1))
-    
-    
-    def start(self):
-        f = self.futures['start']
-        if f is not None and not f.done():
-            raise RuntimeError('{} is already running.'.format(self.name))
-        self._stopped = False
-        self.futures['start'] = f = \
-            asyncio.ensure_future(self._start(), loop=self.loop)
-        return f
-    
-    
-    async def _start(self):
-        fstop = self.futures['stop']
-        if fstop is not None and not fstop.done():
-            self.log2("waiting till 'stop' fut done")
-            await fstop
-
-        self.station.broadcast_multiple(
-            [{'_': 'started', 'op': 'set'},
-             {'_': 'stopped', 'op': 'clear'},
-             {'_': '_stop_initiated', 'op': 'clear'},]
-        )
-        self.broadcast_event('running', 1)
-        await self._safe_activate(self.connect_timeout)
-        
-        if not self._stopped and self.connected_url:
-            self._start_ping_ticker()
-        
-        self._ignore_recv_ts = True
-        recv = self._get_recv()
-        try:
-            while not self._stopped:
-                try:
-                    #asyncio.wait doesn't cancel the recv task when timeout occurs (.gather does)
-                    done, pending = await asyncio.wait([recv], timeout=self.poll_interval)
-                    if recv.done():
-                        #raises ConnectionClosed if .conn was closed
-                        result = recv.result()
-                        if result is _heartbeat:
-                            continue
-                        elif result is _stop_command:
-                            break
-                        
-                    self._verify_recv_timeout()
-
-                    if not recv.done():
-                        self.station.broadcast('empty', op='set')
-                        self.broadcast_event('socket', 'empty')
-                        continue
-                    
-                    self.last_recv_ts = time.time() 
-                    self._ignore_recv_ts = False
-                    r = self.decode_response(result)
-                    is_ping = await self.pong(r)
-                    self.station.broadcast('empty', op='clear')
-                    self.broadcast_event('socket', 'recv')
-                    if is_ping:
-                        continue
-                    
-                except websockets.ConnectionClosed:
-                    await self._on_websocket_error()
-                except (json.JSONDecodeError, UnicodeDecodeError) as e:
-                    dots = '...' if len(result) > 200 else ''
-                    logger2.error("{} - non json-decodable response: {}{}"\
-                                  .format(self.name, result[:200], dots))
-                    logger.error(result)
-                    logger.exception(e)
-                else:
-                    if self.verbose and self.verbose >= 3:
-                        self.log3('received:\n{}'.format(r))
-                    if self.handle is not None:
-                        handlers = self.handle if hasattr(self.handle, '__iter__') else [self.handle]
-                        for handle in handlers:
-                            handle(r)
-                    response = Response(self.id, 'recv', r)
-                    self.station.broadcast('recv', response)
-                finally:
-                    if recv.done():
-                        recv = self._get_recv()
-        except Exception as e:
-            logger2.error("Error occurred in '{}': {}".format(self.name, repr(e)))
-            logger.exception(e)
-        finally:
-            self.station.broadcast('active', op='clear')
-            self.broadcast_event('socket', 0)
-            #print('Leaving {}'.format(self.name))
-            recv.cancel()
-            for fn in ('recv_loop','signalr_wait'):
-                if self.futures[fn] is not None:
-                    self.futures[fn].cancel()
-            self.stop()
-            await self._exit_conn()
-    
-    
-    def _start_ping_ticker(self):
-        if self.ping_interval is None:
-            return
-        self.ping_ticker = \
-            AsyncTicker(self.ping,
-                        self.ping_interval,
-                        keepalive={'pause':self.ping_interval/3},
-                        loop=self.loop,
-                        logging_level=0,
-                        name='{}-Ping-Ticker'.format(self.name))
-        self.futures['ping'] = asyncio.ensure_future(self.ping_ticker.loop())
-    
-    
-    def decode_response(self, r):
-        """If signalr enabled then r may contain byte strings,
-           override this method to decode them."""
-        if self.signalr:
-            return r
-        elif self.socketio:
-            return r # json.loads(r['data'])
-        elif self.unpack_json == 'force':
-            return json.loads(r)
-        elif self.unpack_json:
-            try:
-                return json.loads(r)
-            except (json.JSONDecodeError, UnicodeDecodeError):
-                return r
-        else:
-            return r
-    
-    
-    def _verify_recv_timeout(self):
-        if self.connected_url and self.recv_timeout is not None and not self._ignore_recv_ts and \
-                self.last_recv_ts is not None and time.time() - self.last_recv_ts > self.recv_timeout:
-            self.log('recv timeout occurred. Reconnecting.', 'ERROR')
-            asyncio.ensure_future(self._exit_conn(self.conn))
-            #To force the current recv to complete itself (if not already done)
-            self._socket_recv_queue.put_nowait(_heartbeat)
-            raise websockets.ConnectionClosed(-2, 'recv timeout occurred')
-    
-    
-    async def _on_websocket_error(self):
-        self._ignore_recv_ts = True
-        if self._stopped: return
-        self.log("websocket has crashed. Reconnecting.", logger=logger2)
-        self.station.broadcast('active', op='clear')
-        self.broadcast_event('socket', 0)
-        await self._safe_activate(self.connect_timeout)
-    
-    
-    def _get_recv(self):
-        #will cause some receptions to be lost, as the task wrapped around _socket.recv()
-        # is cancelled when timeout occurs:
-        #r = await asyncio.wait_for(self._socket.recv(),self.poll_interval)
-        #----
-        async def get_from_queue():
-            r = await self._socket_recv_queue.get()
-            if isinstance(r, websockets.ConnectionClosed):
-                raise r
-            return r
-        return asyncio.ensure_future(get_from_queue())
-    
-    
-    async def recv(self, timeout=None, queue_id=0, strip=True):
-        queue = self.station.get_queue('recv', queue_id)
-        r = asyncio.wait_for(await queue.get(), timeout)
-        if strip: 
-            r = r.data
-        return r
-    
-    
-    def send(self, message, dump=True, log=True):
-        return call_via_loop_afut(self._send, (message, dump, log), loop=self.loop)
-    
-    
-    async def _send(self, message, dump=True, log=True):
-        await self.throttle()
-        await self.wait_till_active(self.connect_timeout)
-        if log:
-            self.log('sending: {}'.format(message))
-        if self.signalr:
-            self.hub.server.invoke(*message)
-        elif self.socketio:
-            await self.conn.emit(*message)
-        else:
-            send_msg = json.dumps(message) if dump else message
-            await self.socket.send(send_msg)
-    
-    
-    async def ping(self):
-        try:
-            last_ts = max(self._last_ping_ts, self.last_recv_ts)
-        except TypeError:
-            last_ts = next((x for x in (self._last_ping_ts, self.last_recv_ts) if x), 0)
-        
-        if self.ping_after is None or time.time() > last_ts + self.ping_after:
-            if self.ping_as_message:
-                message = self.ping_func()
-                self.log2('sending ping: {}'.format(message))
-                # message will be json encoded
-                await self.send(message, dump=(self.ping_as_message=='dump'), log=False)
-            else:
-                args = [self.ping_func()] if self.ping_func is not None else []
-                self.log2('sending ping{}'.format(': '+str(args[0]) if args else ''))
-                # message will be converted into bytes (must be str or bytes)
-                try: await asyncio.wait_for(self.socket.ping(*args), self.ping_timeout)
-                except asyncio.TimeoutError:
-                    await self._socket_recv_queue.put(
-                        websockets.ConnectionClosed(-3, 'Ping timeout occurred'))
-                finally:
-                    self._last_ping_ts = time.time()
-    
-     
-    async def pong(self, r):
-        if not self.pong_func:
-            return
-        message = self.pong_func(r)
-        if message is None:
-            return
-        
-        self.log2('received ping: {}. sending pong: {}'.format(r, message))
-        if self.pong_as_message:
-            await self.send(message, dump=(self.pong_as_message=='dump'), log=False)
-        else:
-            await self.socket.pong(message)
-        
-        return True # pong was successfully sent
-    
-    
-    async def throttle(self):
-        await self._throttle()
-    
-    #This will be wrapped by .rate_limit setter (property)
-    async def _throttle(self):
-        pass
-    
-    
-    def is_running(self):
-        return self.futures['start'] is not None and not self.futures['start'].done() and \
-            self.station.get_event('started',0,loop=0).is_set()
-    
-    
-    def is_active(self):
-        return self.is_running() and self.station.get_event('active',0,loop=0).is_set()
-    
-    
-    def is_connected(self):
-        return self.is_active()
-    
-    
-    async def wait_till_active(self, timeout=None):
-        #self.station._print()
-        #print({'loop': id(self.loop), 'out_loop': id(self.out_loop), 'context': id(asyncio.get_event_loop())})
-        event = self.station.get_event('active',0)
-        await asyncio.wait_for(event.wait(), timeout)
-    
-    @property
-    def wait_till_connected(self):
-        return self.wait_till_active
-    
-    @property
-    def add_receptor(self):
-        return self.station.add
-    @property
-    def remove_receptor(self):
-        return self.station.remove
-    
-    def add_queue(self, id, channel='recv', queue=None, maxsize=0, loop='out'):
-        loops = ([loop] if loop!='out' else self.out_loop) if loop is not None else asyncio.get_event_loop()
-        return self.station.add_queue(channel,id,queue,maxsize,loops)
-    
-    def remove_queue(self, id, channel='recv', loop='out'):
-        loops = ([loop] if loop!='out' else self.out_loop) if loop is not None else asyncio.get_event_loop()
-        return self.station.remove(channel,id,loops)
-
-    def broadcast_event(self, event_type, value):
-        self.station.broadcast('event', ConnectionEvent(self.id, event_type, value))
-    
-    
-    def stop(self):
-        f = self.futures['stop']
-        if f is not None and not f.done():
-            return f
-        self.futures['stop'] = f = \
-            asyncio.ensure_future(self._stop(), loop=self.loop)  
-        return f
-    
-    async def _stop(self):
-        #f = self.futures['stop']
-        #if f is not None and not f.done():
-        #    return
-        self._stopped = True
-        self.station.broadcast('_stop_initiated')
-        if self.conn is None: 
-            return
-        fstart = self.futures['start']
-        fping = self.futures['ping']
-        self.log2('stopping')
-        await self._socket_recv_queue.put(_stop_command)
-        if self.ping_ticker is not None:
-            await self.ping_ticker.close()
-            if not fping.done():
-                self.log2('waiting on "ping" future')
-                await fping
-        self.log2('closing socket')
-        await self._exit_conn()
-        if not fstart.done():
-            self.log2('waiting on "start" future')
-            await fstart
-        self.conn = None
-        self.hub = None
-        self.socket = None
-        empty_queue(self._socket_recv_queue)
-        self.station.broadcast_multiple(
-            [{'_': 'stopped', 'op': 'set'},
-             {'_': 'started', 'op': 'clear'},]
-        )
-        self.broadcast_event('running', 0)
-        self.log('stopped')
-        
-        
-    async def _exit_conn(self, conn=None):
-        conn = conn if conn is not None else self.conn
-        if conn is None:
-            pass
-        elif self.signalr:
-            safeTry(conn.close)
-            #self.hub = None
-        elif self.socketio:
-            await safeAsyncTry(conn.disconnect)
-            # this must be done here as socketio has not callback on user initiated disconnect
-            await self._socket_recv_queue.put(websockets.ConnectionClosed(-1, 'socketio ws closed'))
-        else:
-            if hasattr(conn, 'ws_client'):
-                try: await conn.__aexit__(*sys.exc_info())
-                except Exception as e: logger.exception(e)
-            #self.socket = None
-
-        
-    @property
-    def rate_limit(self):
-        return self._rate_limit
-    
-    @rate_limit.setter
-    def rate_limit(self, value):
-        _value = value
-        if value is None:
-            self._throttle = self._throttle_original
-        else:
-            value = (value, 1) if not hasattr(value,'__iter__') else tuple(value)
-            if len(value) != 2: 
-                raise ValueError(_value)
-            self._throttle = \
-                async_limitcalls(*value, 'sleep', 
-                                 logging_level=self.throttle_logging_level, 
-                                 retain_order=True,
-                                 loop=self.loop, 
-                                 f=self._throttle)
-        self._rate_limit = value
-    
-    
-    def _log(self, msg, level='DEBUG', logger=logger, add_name=True):
-        if not isinstance(msg, Exception):
-            if add_name:
-                msg = '{} - {}'.format(self.name, msg)
-            logger.log(_log.level_to_int(level), msg)
-        else:
-            logger.exception(msg)
-    
-    
-    def log(self, msg, level='DEBUG', logger=logger, add_name=True):
-        if self.verbose and self.verbose >= 1:
-            self._log(msg, level, logger, add_name)
-    
-    
-    def log2(self, msg, level='DEBUG', logger=logger, add_name=True):
-        if self.verbose and self.verbose >= 2:
-            self._log(msg, level, logger, add_name)
-    
-    
-    def log3(self, msg, level='DEBUG', logger=logger, add_name=True):
-        if self.verbose and self.verbose >= 3:
-            self._log(msg, level, logger, add_name)
-    
-    
-    def __str__(self):
-        return self.name
-        
-
-class ConnectionEvent(Event):
-    pass
-
-class Response(Event):
-    pass
+import websockets
+import signalr_aio_wsclient as signalr_aio
+import socketio
+import sys
+import json
+import asyncio
+import inspect
+import time
+import datetime
+
+dt = datetime.datetime
+td = datetime.timedelta
+
+from fons.aio import call_via_loop_afut, FonsQueue
+from fons.debug import safeTry, safeAsyncTry
+
+from fons.event import Station, Event, force_put, empty_queue, create_name
+from fons.func import async_limitcalls, get_arg_count
+from fons.sched import AsyncTicker
+import fons.log as _log
+
+logger, logger2, tlogger, tloggers, tlogger0 = _log.get_standard_5(__name__)
+
+
+_CONNECTION_IDS = set()
+_CONNECTION_NAMES = set()
+_stop_command = object()
+_heartbeat = object()
+
+
+class Connection:
+    def __init__(
+        self,
+        url,
+        handle=None,
+        *,
+        on_activate=None,
+        signalr=False,
+        hub_name=None,
+        hub_methods=None,
+        socketio=False,
+        event_names=None,
+        reconnect_try_interval=None,
+        connect_timeout=None,
+        recv_timeout=None,
+        ping_interval=None,
+        ping=None,
+        ping_after=None,
+        ping_timeout=5,
+        ping_as_message=False,
+        pong=None,
+        pong_as_message=True,
+        rate_limit=None,
+        poll_interval=None,
+        queue_maxsizes={},
+        recv_queue=None,
+        event_queue=None,
+        id=None,
+        name_prefix=None,
+        loop=None,
+        out_loop=None,
+        throttle_logging_level=0,
+        extra_headers=None,
+        unpack_json=True,
+        verbose=0
+    ):
+        """
+        :param url: str or (coroutine) function that returns str
+        :param handle: (sync) function or list of functions (or None)
+        :param on_activate: (a)sync function or list of functions (or None)
+        :param out_loop: for station events and queues (recv [received] queue, event queue)
+        :param extra_headers: (coroutine) function that returns dict
+        :param unpack_json:
+            True, False, 'force' (logs and skips the object if it it is not unpackable)
+            ignored if  `socketio` or `signalr` is enabled
+
+        """
+        if signalr and socketio:
+            raise ValueError("`signalr` and `socketio` can't be simultaneously True")
+        if ping_interval is not None and not ping_as_message and (signalr or socketio):
+            which = "signalr" if signalr else "socketio"
+            raise ValueError(
+                "Cannot send raw ping frames if `{}` is set to True. "
+                "You could enable `ping_as_message` instead.".format(which)
+            )
+        if pong and not pong_as_message and (signalr or socketio):
+            which = "signalr" if signalr else "socketio"
+            raise ValueError(
+                "Cannot send raw pong frames if `{}` is set to True. "
+                "You could enable `pong_as_message` instead.".format(which)
+            )
+        if isinstance(ping_as_message, str) and ping_as_message != "dump":
+            raise ValueError(ping_as_message)
+        if isinstance(pong_as_message, str) and pong_as_message != "dump":
+            raise ValueError(pong_as_message)
+        self.url = url
+        self.extra_headers = extra_headers
+        self.handle = handle
+        self.on_activate = on_activate
+        self.verbose = verbose
+        # if id is None, returns free connection number (as str)
+        self.id = create_name(id, None, registry=_CONNECTION_IDS)
+        # default_name is used (and int added to that if already taken)
+        default_name = "{}-{}".format(
+            self.__class__.__name__ if name_prefix is None else name_prefix, self.id
+        )
+        self.name = create_name(
+            None, default_name, _CONNECTION_NAMES, add_int="if_taken"
+        )
+
+        self.socketio = socketio
+        self.signalr = signalr
+        self.hub_name = hub_name
+        self.hub_methods = hub_methods if hub_methods is not None else []
+        self.event_names = event_names if event_names is not None else []
+        self.conn = None
+        self.socket = None
+        self.hub = None
+        self.loop = loop if loop is not None else asyncio.get_event_loop()
+        q = next((x for x in (recv_queue, event_queue) if x is not None), None)
+        if out_loop is None and q is not None:
+            out_loop = q._loop
+        self.out_loop = out_loop if out_loop is not None else self.loop
+
+        self.connect_timeout = connect_timeout
+        self.recv_timeout = recv_timeout
+        self.reconnect_try_interval = reconnect_try_interval
+        self.poll_interval = poll_interval
+        self.throttle_logging_level = throttle_logging_level
+        self._throttle_original = self._throttle
+        self.rate_limit = rate_limit
+
+        self.ping_func = ping
+        self.ping_interval = ping_interval
+        self.ping_after = ping_after
+        self.ping_as_message = ping_as_message
+        self.ping_timeout = ping_timeout
+        self.ping_ticker = None
+        self.pong_func = pong
+        self.pong_as_message = pong_as_message
+
+        self.unpack_json = unpack_json
+
+        self.station = Station(
+            loops={-1: self.loop, 0: self.out_loop}, name=self.name + "[Station]"
+        )
+
+        station_channels = [
+            "started",
+            "active",
+            "stopped",
+            "_stop_initiated",
+            "empty",
+            "event",
+            "recv",
+        ]
+        for ch in station_channels:
+            self.station.add_channel(ch)
+        for ch in ["started", "active", "stopped", "_stop_initiated", "empty"]:
+            self.station.add_event(ch, id=0)
+
+        def _add_q(ch, q_id, queue):
+            maxsizes = {"event": 100}
+            # only add to out_loop
+            loops = [0] if queue is None else [queue._loop]
+            self.station.add_queue(
+                ch,
+                q_id,
+                queue,
+                maxsize=queue_maxsizes.get(ch, maxsizes.get(ch, 0)),
+                loops=loops,
+            )
+
+        for ch, q in [["recv", recv_queue], ["event", event_queue]]:
+            if isinstance(q, dict):
+                for i, _q in q.items():
+                    _add_q(ch, i, _q)
+            elif hasattr(q, "__iter__"):
+                for i, _q in enumerate(q):
+                    _add_q(ch, i, _q)
+            else:
+                _add_q(ch, 0, q)
+
+        self._queues = {}
+        self.futures = dict.fromkeys(
+            ["start", "stop", "ping", "recv_loop", "on_activate", "signalr_wait"]
+        )
+        self.connected_url = None
+        self.connected_ts = None
+        self.last_recv_ts = None
+        self._last_ping_ts = None
+        self._ignore_recv_ts = False
+        self._stopped = False
+
+    async def _connect(self):
+        suffix = (
+            " (socketio)" if self.socketio else (" (signalr)" if self.signalr else "")
+        )
+        self.log("connecting{}".format(suffix))
+        params = {}
+
+        url = self.url
+        if hasattr(self.url, "__call__"):
+            url = url()
+        if inspect.isawaitable(url):
+            url = await url
+
+        headers_from_url = {}
+        if isinstance(url, dict):
+            _headers = url.get("extra_headers")
+            if _headers is not None:
+                headers_from_url.update(_headers)
+            url = url["url"]
+        url_msg = "url: {}".format(url) if url != "" else "url empty"
+        self.log(url_msg)
+
+        extra_headers = self.extra_headers
+        if hasattr(extra_headers, "__call__"):
+            extra_headers = extra_headers()
+        if inspect.isawaitable(extra_headers):
+            extra_headers = await extra_headers
+
+        if extra_headers is None:
+            extra_headers = {}
+
+        final_headers = dict(extra_headers, **headers_from_url)
+        if final_headers:
+            params["extra_headers"] = final_headers
+
+        if not url:
+            pass
+        elif self.signalr:
+            await self._connect_signalr(url)
+        elif self.socketio:
+            await self._connect_socketio(url)
+        else:
+            await self._connect_ordinary(url, params)
+
+        self.log("connection established")
+        self.connected_url = url
+        self.connected_ts = time.time()
+        # self.socket.settimeout(self.timeout)
+
+    async def _connect_ordinary(self, url, params={}):
+        self.conn = websockets.connect(url, **params)
+        self.socket = (
+            await self.conn.__aenter__()
+        )  # this also execs logging.basicConfig
+        q = self._socket_recv_queue
+
+        async def recv_loop():
+            while True:
+                try:
+                    r = await self.socket.recv()
+                except websockets.ConnectionClosed as e:
+                    force_put(q, e)
+                    break
+                else:
+                    force_put(q, r)
+
+        self.futures["recv_loop"] = asyncio.ensure_future(recv_loop())
+
+    async def _connect_signalr(self, url):
+        self.conn = signalr_aio.Connection(url, session=None)
+        self.hub = self.conn.register_hub(self.hub_name)
+
+        # All data received from server is handled by .handle,
+        # hub specific handling is not implemented
+        async def do_nothing(msg):
+            pass
+
+        for method in self.hub_methods:
+            self.hub.client.on(method, do_nothing)
+        # messages to .recv are forwarded via signal_recv_queue
+        q = self._socket_recv_queue
+
+        async def put_to_recv_queue(**data):
+            await q.put(data)
+
+        self.conn.received += put_to_recv_queue
+        self.conn.start()
+
+        signalr_fut = self.conn._Connection__transport._conn_handler
+        await asyncio.wait([signalr_fut], timeout=0.5)
+        if signalr_fut.done():
+            await signalr_fut  # raises exception if occurred
+
+        async def wait_on_signalr_future():
+            try:
+                await signalr_fut
+            except websockets.ConnectionClosed as e:
+                self.log("signalr socket has crashed")
+                await q.put(e)
+            else:
+                self.log("signalr socket has been closed")
+                await q.put(websockets.ConnectionClosed(-1, "signalr ws closed"))
+
+        self.futures["signalr_wait"] = asyncio.ensure_future(wait_on_signalr_future())
+
+    async def _connect_socketio(self, url):
+        self.conn = sio = socketio.AsyncClient(reconnection=False)
+        # messages to .recv are forwarded via signal_recv_queue
+        q = self._socket_recv_queue
+        connected = asyncio.Event()
+
+        async def message(data):
+            await q.put(data)
+
+        for event in self.event_names:
+            sio.on(event)(message)
+
+        @sio.event
+        async def connect():
+            connected.set()
+
+        @sio.event
+        async def connect_error(*args):
+            self.log("socketio encountered connect error")
+            await q.put(websockets.ConnectionClosed(-1, "socketio connect error"))
+
+        # This isn't executed when user itself evokes sio.disconnect (or here Connection.stop())
+        @sio.event
+        async def disconnect():
+            self.log("socketio connection has crashed")
+            await q.put(websockets.ConnectionClosed(-1, "socketio ws crashed"))
+
+        await sio.connect(url, transports="websocket")
+        await connected.wait()
+
+    async def _activate(self, timeout=None):
+        # Close any previous connection if by chance left open (though it shouldn't happen)
+        await self._exit_conn()
+        # Renew the queue to ensure that we won't be receiving anything from previous sockets
+        # TODO: set max size to this queue?
+        self._socket_recv_queue = FonsQueue(loop=self.loop)
+        self.conn = None
+        fut = asyncio.ensure_future(self._connect())
+        wait_started = time.time()
+        is_exceeded = (
+            lambda: timeout is not None and time.time() - wait_started > timeout
+        )
+        while not self._stopped and not is_exceeded() and not fut.done():
+            await asyncio.wait([fut], timeout=0.1)
+        to_occurred = is_exceeded()
+        if fut.done():
+            await fut  # raise exception if occurred
+        else:
+            fut.cancel()
+            await self._exit_conn()
+            if to_occurred:
+                raise asyncio.TimeoutError(
+                    "{} - connect timeout occurred".format(self.name)
+                )
+        if self._stopped:
+            return
+        self.station.broadcast("active")
+        self.broadcast_event("socket", 1)
+        if self.on_activate is not None:
+            on_activate = (
+                [self.on_activate]
+                if not hasattr(self.on_activate, "__iter__")
+                else self.on_activate
+            )
+            for i, f in enumerate(on_activate):
+                args = [self] if get_arg_count(f) else []
+                key = "on_activate{}".format("_{}".format(i) if i else "")
+                self.futures[key] = call_via_loop_afut(f, args)
+
+    async def _safe_activate(self, timeout=None):
+        await safeAsyncTry(
+            self._activate,
+            (timeout,),
+            attempts=True,
+            pause=self.reconnect_try_interval,
+            exit_on=self.station.get_event("_stop_initiated", 0, loop=-1),
+        )
+
+    def start(self):
+        f = self.futures["start"]
+        if f is not None and not f.done():
+            raise RuntimeError("{} is already running.".format(self.name))
+        self._stopped = False
+        self.futures["start"] = f = asyncio.ensure_future(self._start(), loop=self.loop)
+        return f
+
+    async def _start(self):
+        fstop = self.futures["stop"]
+        if fstop is not None and not fstop.done():
+            self.log2("waiting till 'stop' fut done")
+            await fstop
+
+        self.station.broadcast_multiple(
+            [
+                {"_": "started", "op": "set"},
+                {"_": "stopped", "op": "clear"},
+                {"_": "_stop_initiated", "op": "clear"},
+            ]
+        )
+        self.broadcast_event("running", 1)
+        await self._safe_activate(self.connect_timeout)
+
+        if not self._stopped and self.connected_url:
+            self._start_ping_ticker()
+
+        self._ignore_recv_ts = True
+        recv = self._get_recv()
+        try:
+            while not self._stopped:
+                try:
+                    # asyncio.wait doesn't cancel the recv task when timeout occurs (.gather does)
+                    done, pending = await asyncio.wait(
+                        [recv], timeout=self.poll_interval
+                    )
+                    if recv.done():
+                        # raises ConnectionClosed if .conn was closed
+                        result = recv.result()
+                        if result is _heartbeat:
+                            continue
+                        elif result is _stop_command:
+                            break
+
+                    self._verify_recv_timeout()
+
+                    if not recv.done():
+                        self.station.broadcast("empty", op="set")
+                        self.broadcast_event("socket", "empty")
+                        continue
+
+                    self.last_recv_ts = time.time()
+                    self._ignore_recv_ts = False
+                    r = self.decode_response(result)
+                    is_ping = await self.pong(r)
+                    self.station.broadcast("empty", op="clear")
+                    self.broadcast_event("socket", "recv")
+                    if is_ping:
+                        continue
+
+                except websockets.ConnectionClosed:
+                    await self._on_websocket_error()
+                except (json.JSONDecodeError, UnicodeDecodeError) as e:
+                    dots = "..." if len(result) > 200 else ""
+                    logger2.error(
+                        "{} - non json-decodable response: {}{}".format(
+                            self.name, result[:200], dots
+                        )
+                    )
+                    logger.error(result)
+                    logger.exception(e)
+                else:
+                    if self.verbose and self.verbose >= 3:
+                        self.log3("received:\n{}".format(r))
+                    if self.handle is not None:
+                        handlers = (
+                            self.handle
+                            if hasattr(self.handle, "__iter__")
+                            else [self.handle]
+                        )
+                        for handle in handlers:
+                            handle(r)
+                    response = Response(self.id, "recv", r)
+                    self.station.broadcast("recv", response)
+                finally:
+                    if recv.done():
+                        recv = self._get_recv()
+        except Exception as e:
+            logger2.error("Error occurred in '{}': {}".format(self.name, repr(e)))
+            logger.exception(e)
+        finally:
+            self.station.broadcast("active", op="clear")
+            self.broadcast_event("socket", 0)
+            # print('Leaving {}'.format(self.name))
+            recv.cancel()
+            for fn in ("recv_loop", "signalr_wait"):
+                if self.futures[fn] is not None:
+                    self.futures[fn].cancel()
+            self.stop()
+            await self._exit_conn()
+
+    def _start_ping_ticker(self):
+        if self.ping_interval is None:
+            return
+        self.ping_ticker = AsyncTicker(
+            self.ping,
+            self.ping_interval,
+            keepalive={"pause": self.ping_interval / 3},
+            loop=self.loop,
+            logging_level=0,
+            name="{}-Ping-Ticker".format(self.name),
+        )
+        self.futures["ping"] = asyncio.ensure_future(self.ping_ticker.loop())
+
+    def decode_response(self, r):
+        """If signalr enabled then r may contain byte strings,
+        override this method to decode them."""
+        if self.signalr:
+            return r
+        elif self.socketio:
+            return r  # json.loads(r['data'])
+        elif self.unpack_json == "force":
+            return json.loads(r)
+        elif self.unpack_json:
+            try:
+                return json.loads(r)
+            except (json.JSONDecodeError, UnicodeDecodeError):
+                return r
+        else:
+            return r
+
+    def _verify_recv_timeout(self):
+        if (
+            self.connected_url
+            and self.recv_timeout is not None
+            and not self._ignore_recv_ts
+            and self.last_recv_ts is not None
+            and time.time() - self.last_recv_ts > self.recv_timeout
+        ):
+            self.log("recv timeout occurred. Reconnecting.", "ERROR")
+            asyncio.ensure_future(self._exit_conn(self.conn))
+            # To force the current recv to complete itself (if not already done)
+            self._socket_recv_queue.put_nowait(_heartbeat)
+            raise websockets.ConnectionClosed(-2, "recv timeout occurred")
+
+    async def _on_websocket_error(self):
+        self._ignore_recv_ts = True
+        if self._stopped:
+            return
+        self.log("websocket has crashed. Reconnecting.", logger=logger2)
+        self.station.broadcast("active", op="clear")
+        self.broadcast_event("socket", 0)
+        await self._safe_activate(self.connect_timeout)
+
+    def _get_recv(self):
+        # will cause some receptions to be lost, as the task wrapped around _socket.recv()
+        # is cancelled when timeout occurs:
+        # r = await asyncio.wait_for(self._socket.recv(),self.poll_interval)
+        # ----
+        async def get_from_queue():
+            r = await self._socket_recv_queue.get()
+            if isinstance(r, websockets.ConnectionClosed):
+                raise r
+            return r
+
+        return asyncio.ensure_future(get_from_queue())
+
+    async def recv(self, timeout=None, queue_id=0, strip=True):
+        queue = self.station.get_queue("recv", queue_id)
+        r = asyncio.wait_for(await queue.get(), timeout)
+        if strip:
+            r = r.data
+        return r
+
+    def send(self, message, dump=True, log=True):
+        return call_via_loop_afut(self._send, (message, dump, log), loop=self.loop)
+
+    async def _send(self, message, dump=True, log=True):
+        await self.throttle()
+        await self.wait_till_active(self.connect_timeout)
+        if log:
+            self.log("sending: {}".format(message))
+        if self.signalr:
+            self.hub.server.invoke(*message)
+        elif self.socketio:
+            await self.conn.emit(*message)
+        else:
+            send_msg = json.dumps(message) if dump else message
+            await self.socket.send(send_msg)
+
+    async def ping(self):
+        try:
+            last_ts = max(self._last_ping_ts, self.last_recv_ts)
+        except TypeError:
+            last_ts = next((x for x in (self._last_ping_ts, self.last_recv_ts) if x), 0)
+
+        if self.ping_after is None or time.time() > last_ts + self.ping_after:
+            if self.ping_as_message:
+                message = self.ping_func()
+                self.log2("sending ping: {}".format(message))
+                # message will be json encoded
+                await self.send(
+                    message, dump=(self.ping_as_message == "dump"), log=False
+                )
+            else:
+                args = [self.ping_func()] if self.ping_func is not None else []
+                self.log2("sending ping{}".format(": " + str(args[0]) if args else ""))
+                # message will be converted into bytes (must be str or bytes)
+                try:
+                    await asyncio.wait_for(self.socket.ping(*args), self.ping_timeout)
+                except asyncio.TimeoutError:
+                    await self._socket_recv_queue.put(
+                        websockets.ConnectionClosed(-3, "Ping timeout occurred")
+                    )
+                finally:
+                    self._last_ping_ts = time.time()
+
+    async def pong(self, r):
+        if not self.pong_func:
+            return
+        message = self.pong_func(r)
+        if message is None:
+            return
+
+        self.log2("received ping: {}. sending pong: {}".format(r, message))
+        if self.pong_as_message:
+            await self.send(message, dump=(self.pong_as_message == "dump"), log=False)
+        else:
+            await self.socket.pong(message)
+
+        return True  # pong was successfully sent
+
+    async def throttle(self):
+        await self._throttle()
+
+    # This will be wrapped by .rate_limit setter (property)
+    async def _throttle(self):
+        pass
+
+    def is_running(self):
+        return (
+            self.futures["start"] is not None
+            and not self.futures["start"].done()
+            and self.station.get_event("started", 0, loop=0).is_set()
+        )
+
+    def is_active(self):
+        return (
+            self.is_running() and self.station.get_event("active", 0, loop=0).is_set()
+        )
+
+    def is_connected(self):
+        return self.is_active()
+
+    async def wait_till_active(self, timeout=None):
+        # self.station._print()
+        # print({'loop': id(self.loop), 'out_loop': id(self.out_loop), 'context': id(asyncio.get_event_loop())})
+        event = self.station.get_event("active", 0)
+        await asyncio.wait_for(event.wait(), timeout)
+
+    @property
+    def wait_till_connected(self):
+        return self.wait_till_active
+
+    @property
+    def add_receptor(self):
+        return self.station.add
+
+    @property
+    def remove_receptor(self):
+        return self.station.remove
+
+    def add_queue(self, id, channel="recv", queue=None, maxsize=0, loop="out"):
+        loops = (
+            ([loop] if loop != "out" else self.out_loop)
+            if loop is not None
+            else asyncio.get_event_loop()
+        )
+        return self.station.add_queue(channel, id, queue, maxsize, loops)
+
+    def remove_queue(self, id, channel="recv", loop="out"):
+        loops = (
+            ([loop] if loop != "out" else self.out_loop)
+            if loop is not None
+            else asyncio.get_event_loop()
+        )
+        return self.station.remove(channel, id, loops)
+
+    def broadcast_event(self, event_type, value):
+        self.station.broadcast("event", ConnectionEvent(self.id, event_type, value))
+
+    def stop(self):
+        f = self.futures["stop"]
+        if f is not None and not f.done():
+            return f
+        self.futures["stop"] = f = asyncio.ensure_future(self._stop(), loop=self.loop)
+        return f
+
+    async def _stop(self):
+        # f = self.futures['stop']
+        # if f is not None and not f.done():
+        #    return
+        self._stopped = True
+        self.station.broadcast("_stop_initiated")
+        if self.conn is None:
+            return
+        fstart = self.futures["start"]
+        fping = self.futures["ping"]
+        self.log2("stopping")
+        await self._socket_recv_queue.put(_stop_command)
+        if self.ping_ticker is not None:
+            await self.ping_ticker.close()
+            if not fping.done():
+                self.log2('waiting on "ping" future')
+                await fping
+        self.log2("closing socket")
+        await self._exit_conn()
+        if not fstart.done():
+            self.log2('waiting on "start" future')
+            await fstart
+        self.conn = None
+        self.hub = None
+        self.socket = None
+        empty_queue(self._socket_recv_queue)
+        self.station.broadcast_multiple(
+            [
+                {"_": "stopped", "op": "set"},
+                {"_": "started", "op": "clear"},
+            ]
+        )
+        self.broadcast_event("running", 0)
+        self.log("stopped")
+
+    async def _exit_conn(self, conn=None):
+        conn = conn if conn is not None else self.conn
+        if conn is None:
+            pass
+        elif self.signalr:
+            safeTry(conn.close)
+            # self.hub = None
+        elif self.socketio:
+            await safeAsyncTry(conn.disconnect)
+            # this must be done here as socketio has not callback on user initiated disconnect
+            await self._socket_recv_queue.put(
+                websockets.ConnectionClosed(-1, "socketio ws closed")
+            )
+        else:
+            if hasattr(conn, "ws_client"):
+                try:
+                    await conn.__aexit__(*sys.exc_info())
+                except Exception as e:
+                    logger.exception(e)
+            # self.socket = None
+
+    @property
+    def rate_limit(self):
+        return self._rate_limit
+
+    @rate_limit.setter
+    def rate_limit(self, value):
+        _value = value
+        if value is None:
+            self._throttle = self._throttle_original
+        else:
+            value = (value, 1) if not hasattr(value, "__iter__") else tuple(value)
+            if len(value) != 2:
+                raise ValueError(_value)
+            self._throttle = async_limitcalls(
+                *value,
+                "sleep",
+                logging_level=self.throttle_logging_level,
+                retain_order=True,
+                loop=self.loop,
+                f=self._throttle
+            )
+        self._rate_limit = value
+
+    def _log(self, msg, level="DEBUG", logger=logger, add_name=True):
+        if not isinstance(msg, Exception):
+            if add_name:
+                msg = "{} - {}".format(self.name, msg)
+            logger.log(_log.level_to_int(level), msg)
+        else:
+            logger.exception(msg)
+
+    def log(self, msg, level="DEBUG", logger=logger, add_name=True):
+        if self.verbose and self.verbose >= 1:
+            self._log(msg, level, logger, add_name)
+
+    def log2(self, msg, level="DEBUG", logger=logger, add_name=True):
+        if self.verbose and self.verbose >= 2:
+            self._log(msg, level, logger, add_name)
+
+    def log3(self, msg, level="DEBUG", logger=logger, add_name=True):
+        if self.verbose and self.verbose >= 3:
+            self._log(msg, level, logger, add_name)
+
+    def __str__(self):
+        return self.name
+
+
+class ConnectionEvent(Event):
+    pass
+
+
+class Response(Event):
+    pass
```

### Comparing `wsclient-0.3.0/wsclient/conn_mgr.py` & `wsclient-0.4.0/wsclient/conn_mgr.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,143 +1,164 @@
-from fons.dict_ops import deep_get
-from fons.event import Station
-import fons.log as _log
-
-from .conn import Connection
-from .errors import ConnectionLimitExceeded
-
-logger,logger2,tlogger,tloggers,tlogger0 = _log.get_standard_5(__name__)
-
-# How to integrate both url and socket sub registration?
-# When unsubbing remove it from cnxi's url_factory, which
-# will then later .satisfies(sub), but return e.g. 'through_socket'
-# which will signal to .send() to proceed with the through-socket
-# procedure
-
-class ConnectionManager:
-    def __init__(self, wrapper):
-        """:type wrapper: WSClient"""
-        self.wc = wrapper
-        self.connections = {}
-        self.cnx_infs = {}
-        self.station = Station([{'channel': 'all_active', 'id': 0, 'queue': False}],
-                               loops=[self.wc.loop],
-                               name=self.wc.name+'[CM][Station]')
-    
-    def add_connection(self, config, start=False):
-        cur_len = len(self.connections)
-        if self.wc.max_total_connections is not None and cur_len >= self.wc.max_total_connections:
-            raise ConnectionLimitExceeded('{} - number of connections ({}) has reached its limit ({})'
-                                          .format(self.wc.name, cur_len, self.wc.max_total_connections))
-        cnx = Connection(**config)
-        self.connections[cnx.id] = cnx
-        self.cnx_infs[cnx] = ConnectionInfo(self.wc, cnx)
-        if start:
-            cnx.start()
-        return cnx
-    
-    def remove_connection(self, id, delete=False):
-        cnx = None
-        if not isinstance(id, Connection):
-            try: cnx = self.connections[id]
-            except KeyError: pass
-        else:
-            cnx = id
-        if cnx is not None:
-            cnx.stop()
-            if delete and cnx.id in self.connections:
-                self.wc.log('removing connection <{}>'.format(cnx.id))
-                del self.connections[cnx.id]
-            if delete and cnx in self.cnx_infs:
-                del self.cnx_infs[cnx]
-        return cnx
-    
-    def remove_all(self):
-        for id in list(self.connections.keys()):
-            self.remove_connection(id)
-            
-    def delete_connection(self, cnx):
-        try: del self.connections[cnx.id]
-        except KeyError: pass
-        
-        try: del self.cnx_infs[cnx]
-        except KeyError: pass
-        
-        if cnx.is_running():
-            cnx.stop()
-            
-            
-class ConnectionInfo:
-    def __init__(self, wc, cnx):
-        """:type wc: WSClient
-           :type cnx: Connection"""
-        self.wc = wc
-        self.cnx = cnx
-        self.max_subscriptions = (self.wc.max_subscriptions_per_connection
-                                    if self.wc.max_subscriptions_per_connection is not None else
-                                  100*1000)
-        self.authenticated = False
-        
-    def satisfies(self, params, url_factory=None):
-        """:param url_factory: may provide params specific url_factory
-                               which shall yield True if cnx.url.params == url_factory.params
-                               (useful for reusing old connection for the exact same subscription,
-                                if the url directly provides stream (takes only one sub, enabled by connecting))"""
-        channel = params['_']
-        #send = self.wc.cis.get_value(channel,'send',True)
-        #register_via = self.wc.cis.get_value(channel,'register_via','socket').lower()
-        #methods = register_via.split(' ')
-        #url_satisfied = True
-        #if 'url' in methods:
-        if url_factory is None:
-            url_factory = self.wc.cis.get_value(channel,'url_factory')
-        if self.cnx.url != url_factory:
-            return False
-        auth_satisfied = self.auth_satisfied(channel)
-        if not auth_satisfied:
-            return False
-        return True
-        
-    def auth_satisfied(self, channel):
-        is_private = self.wc.cis.get_value(channel,'is_private')
-        seq = self.auth_seq(channel)
-        auth_required = deep_get(seq,'required',return2=None)
-        if (not is_private and auth_required is None) or \
-                (auth_required is not None and not auth_required):
-            return True
-        via_url = deep_get(seq,'via_url')
-        if via_url: 
-            return True
-        each_time = deep_get(seq,'each_time')
-        if each_time or self.authenticated:
-            return True
-        #One for authentication subscription, the other for current subscription
-        elif self.free_subscription_slots >= 2:
-            return True
-        return False        
-    
-    def is_private(self):
-        pass
-    
-    def auth_seq(self, channel, i=None):
-        auth = self.wc.cis.get_value(channel,'auth',{})
-        defaults = self.wc.auth_defaults
-        if i is None:
-            return [auth, defaults]
-        else:
-            auth_i = auth.get(i, {})
-            defaults_i = defaults.get(i, {})
-            return [auth_i, auth, defaults_i, defaults]
-    
-    def get_auth_value(self, channel, *args, **kw):
-        """Deep get auth value of channel"""
-        return deep_get(self.auth_seq(channel),*args,**kw)
-        
-    @property
-    def connection(self):
-        return self.cnx
-    @property
-    def sub_count(self):
-        return sum(s.cnx is self.cnx for s in self.wc.sh.subscriptions)
-    @property
-    def free_subscription_slots(self):
-        return self.max_subscriptions - self.sub_count
+from fons.dict_ops import deep_get
+from fons.event import Station
+import fons.log as _log
+
+from .conn import Connection
+from .errors import ConnectionLimitExceeded
+
+logger, logger2, tlogger, tloggers, tlogger0 = _log.get_standard_5(__name__)
+
+# How to integrate both url and socket sub registration?
+# When unsubbing remove it from cnxi's url_factory, which
+# will then later .satisfies(sub), but return e.g. 'through_socket'
+# which will signal to .send() to proceed with the through-socket
+# procedure
+
+
+class ConnectionManager:
+    def __init__(self, wrapper):
+        """:type wrapper: WSClient"""
+        self.wc = wrapper
+        self.connections = {}
+        self.cnx_infs = {}
+        self.station = Station(
+            [{"channel": "all_active", "id": 0, "queue": False}],
+            loops=[self.wc.loop],
+            name=self.wc.name + "[CM][Station]",
+        )
+
+    def add_connection(self, config, start=False):
+        cur_len = len(self.connections)
+        if (
+            self.wc.max_total_connections is not None
+            and cur_len >= self.wc.max_total_connections
+        ):
+            raise ConnectionLimitExceeded(
+                "{} - number of connections ({}) has reached its limit ({})".format(
+                    self.wc.name, cur_len, self.wc.max_total_connections
+                )
+            )
+        cnx = Connection(**config)
+        self.connections[cnx.id] = cnx
+        self.cnx_infs[cnx] = ConnectionInfo(self.wc, cnx)
+        if start:
+            cnx.start()
+        return cnx
+
+    def remove_connection(self, id, delete=False):
+        cnx = None
+        if not isinstance(id, Connection):
+            try:
+                cnx = self.connections[id]
+            except KeyError:
+                pass
+        else:
+            cnx = id
+        if cnx is not None:
+            cnx.stop()
+            if delete and cnx.id in self.connections:
+                self.wc.log("removing connection <{}>".format(cnx.id))
+                del self.connections[cnx.id]
+            if delete and cnx in self.cnx_infs:
+                del self.cnx_infs[cnx]
+        return cnx
+
+    def remove_all(self):
+        for id in list(self.connections.keys()):
+            self.remove_connection(id)
+
+    def delete_connection(self, cnx):
+        try:
+            del self.connections[cnx.id]
+        except KeyError:
+            pass
+
+        try:
+            del self.cnx_infs[cnx]
+        except KeyError:
+            pass
+
+        if cnx.is_running():
+            cnx.stop()
+
+
+class ConnectionInfo:
+    def __init__(self, wc, cnx):
+        """:type wc: WSClient
+        :type cnx: Connection"""
+        self.wc = wc
+        self.cnx = cnx
+        self.max_subscriptions = (
+            self.wc.max_subscriptions_per_connection
+            if self.wc.max_subscriptions_per_connection is not None
+            else 100 * 1000
+        )
+        self.authenticated = False
+
+    def satisfies(self, params, url_factory=None):
+        """:param url_factory: may provide params specific url_factory
+        which shall yield True if cnx.url.params == url_factory.params
+        (useful for reusing old connection for the exact same subscription,
+         if the url directly provides stream (takes only one sub, enabled by connecting))
+        """
+        channel = params["_"]
+        # send = self.wc.cis.get_value(channel,'send',True)
+        # register_via = self.wc.cis.get_value(channel,'register_via','socket').lower()
+        # methods = register_via.split(' ')
+        # url_satisfied = True
+        # if 'url' in methods:
+        if url_factory is None:
+            url_factory = self.wc.cis.get_value(channel, "url_factory")
+        if self.cnx.url != url_factory:
+            return False
+        auth_satisfied = self.auth_satisfied(channel)
+        if not auth_satisfied:
+            return False
+        return True
+
+    def auth_satisfied(self, channel):
+        is_private = self.wc.cis.get_value(channel, "is_private")
+        seq = self.auth_seq(channel)
+        auth_required = deep_get(seq, "required", return2=None)
+        if (not is_private and auth_required is None) or (
+            auth_required is not None and not auth_required
+        ):
+            return True
+        via_url = deep_get(seq, "via_url")
+        if via_url:
+            return True
+        each_time = deep_get(seq, "each_time")
+        if each_time or self.authenticated:
+            return True
+        # One for authentication subscription, the other for current subscription
+        elif self.free_subscription_slots >= 2:
+            return True
+        return False
+
+    def is_private(self):
+        pass
+
+    def auth_seq(self, channel, i=None):
+        auth = self.wc.cis.get_value(channel, "auth", {})
+        defaults = self.wc.auth_defaults
+        if i is None:
+            return [auth, defaults]
+        else:
+            auth_i = auth.get(i, {})
+            defaults_i = defaults.get(i, {})
+            return [auth_i, auth, defaults_i, defaults]
+
+    def get_auth_value(self, channel, *args, **kw):
+        """Deep get auth value of channel"""
+        return deep_get(self.auth_seq(channel), *args, **kw)
+
+    @property
+    def connection(self):
+        return self.cnx
+
+    @property
+    def sub_count(self):
+        return sum(s.cnx is self.cnx for s in self.wc.sh.subscriptions)
+
+    @property
+    def free_subscription_slots(self):
+        return self.max_subscriptions - self.sub_count
```

### Comparing `wsclient-0.3.0/wsclient/extend_attrs.py` & `wsclient-0.4.0/wsclient/extend_attrs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,196 +1,207 @@
-from fons.dict_ops import deep_update
-from fons.py import mro as _mro
-
-import copy as _copy
-
-PROPERTY_RECURSION_LIMIT = 2
-
-_ASC = ''.join(chr(i) for i in range(128))
-_ALNUM_ = ''.join(x for x in _ASC if x.isalnum()) + '_'
-_ALPHA_ = ''.join(x for x in _ASC if x.isalpha()) + '_'
-_ALNUM_DOT_ = _ALNUM_ + '.'
-
-
-
-class ExtendAttrs(type):
-    """
-    Deep updates attributes listed in __extend_attrs__, by copying the next attribute found in mro,
-    and then "deep updates" it with the same attr of current class. 
-    IMPORTANT!
-    All these attributes are being deepcopied, i.e. all references to previous attrs 
-    and their (deep) values are lost.
-    """
-    def __new__(cls, name, bases, attrs):
-        mro = _mro(*bases)
-        mro_included = (attrs,) + mro
-        extend_attrs = ExtendAttrs._join(mro_included, '__extend_attrs__')
-        
-        # Extend the attributes listed in 'extend_attrs'
-        for _ in extend_attrs:
-            try: nxt_value = next(getattr(x, _) for x in mro if hasattr(x, _))
-            except StopIteration: continue
-            if _ in attrs:
-                attrs[_] = deep_update(nxt_value, attrs[_], copy=True)
-            else:
-                attrs[_] = _copy.deepcopy(nxt_value)
-        
-        if '__extend_attrs__' in attrs:
-            # Save the original value
-            attrs['_{}__extend_attrs'.format(name)] = attrs['__extend_attrs__']
-            # Overwrite with new value
-            attrs['__extend_attrs__'] = extend_attrs
-        
-        if '__deepcopy_on_init__' in attrs:
-            attrs['_{}__deepcopy_on_init'.format(name)] = attrs['__deepcopy_on_init__']
-            deepcopy_on_init = ExtendAttrs._join(mro_included, '__deepcopy_on_init__')
-            attrs['__deepcopy_on_init__'] = deepcopy_on_init
-        
-        # Override object class' __new__ method so that it would deepcopy the attrs
-        # listed in __deepcopy_on_init__ before calling __init__ of the class
-        is_first = not any(isinstance(x, ExtendAttrs) for x in bases)
-        if is_first:
-            ExtendAttrs.override__new__(mro, attrs)
-        
-        return super(ExtendAttrs, cls).__new__(cls, name, bases, attrs)
-    
-    
-    @staticmethod
-    def _join(bases, name='__extend_attrs__'):
-        """Adds all previous __extend_attrs__ together, and deducts all that start with '-'"""
-        extend_attrs = []
-        
-        for cls in reversed(bases):
-            is_dict = isinstance(cls, dict)
-            _name = name if is_dict else '_{}{}'.format(cls.__name__, name[:-2])
-            cls_ea = cls.get(_name) if is_dict else getattr(cls, _name, None)
-            
-            if cls_ea is None:
-                continue
-            
-            if '-' in cls_ea:
-                extend_attrs = []
-            
-            deduct = [x for x in cls_ea if len(x)>1 and x[0]=='-']
-            add = [x for x in cls_ea if not x.startswith('-')]
-            
-            for attr in deduct:
-                try: extend_attrs.remove(attr[1:])
-                except ValueError: pass
-            
-            for attr in add:
-                if attr not in extend_attrs:
-                    extend_attrs.append(attr)
-                
-        return extend_attrs
-    
-    
-    @staticmethod
-    def override__new__(mro, attrs):
-        if '__new__' in attrs:
-            orig_new = attrs['__new__']
-        elif len(mro):
-            orig_new = mro[0].__new__
-        else:
-            orig_new = object.__new__
-        
-        def __new_with_deepcopy__(cls, *args, **kw):
-            obj = orig_new(cls)
-            ExtendAttrs.deepcopy_attrs(obj)
-            return obj
-
-        attrs['__new__'] = __new_with_deepcopy__
-    
-    
-    @staticmethod
-    def deepcopy_attrs(obj):
-        if not hasattr(obj, '__deepcopy_on_init__'):
-            return
-        for key in obj.__deepcopy_on_init__:
-            if hasattr(obj, key):
-                setattr(obj, key, _copy.deepcopy(getattr(obj, key)))
-
-
-class CreateProperties(type):
-    """Initiates properties listed in __properties__. Also creates sub_to_{x} and unsub_to{x} shortcuts to all
-    methods that match the patterns subscribe_to_{x} / unsubscribe_to_{x}"""
-    def __new__(cls, name, bases, attrs):
-        CreateProperties._init_properties(attrs)
-       
-        return super(CreateProperties, cls).__new__(cls, name, bases, attrs)
-    
-    
-    @staticmethod
-    def _init_properties(attrs):
-        properties = attrs.get('__properties__', [])
-        final_properties = properties[:]
-        
-        #Create properties for methods that start with "(un)subscribe_to"
-        for attr in attrs:
-            for startsWith,replaceWith in zip(['subscribe_to_','unsubscribe_to_'],
-                                              ['sub_to_','unsub_to_']):
-                if attr.startswith(startsWith):
-                    property_name = replaceWith + attr[len(startsWith):]
-                    final_properties.append([property_name,attr,True,False,False])
-                    
-        for item in final_properties:
-            property_name = item[0]
-            attrs[property_name] = CreateProperties._create_property(*item)
-    
-    
-    @staticmethod            
-    def _verify_name(name, set=_ALNUM_):
-        if not all(x in set for x in name):
-            raise ValueError("The property name/value '{}' contains non alnum characters".format(name))
-                             
-        if not all(x[:1] in _ALPHA_ for x in name.split('.')):
-            raise ValueError("The property name/value '{}' starts with non alpha character".format(name))
-    
-    
-    @staticmethod       
-    def _create_property(property_name, attr, GET=True, SET=True, DEL=True):
-        """
-        This MAY be vulnerable to attack, if the x.y.z... leads to another
-        property (that executes code), or to who knows what object.
-        Make sure that the __properties__ are trusted 
-        (which they as pre-assigned class attributes almost certainly should be,
-         unless we are talking about hypothetical dynamic subclassing through an API,
-         or a malevolent github team member in a situation where other members
-         didn't turn attention to __properties__ modification).
-        For that reason the PROPERTY_RECURSION_LIMIT is set to 2."""
-        CreateProperties._verify_name(property_name)
-        #attr can be given as attr_of_self.attr_of_that_attr....
-        CreateProperties._verify_name(attr, _ALNUM_DOT_)
-        
-        attr_seq = attr.split('.')
-        if len(attr_seq) > PROPERTY_RECURSION_LIMIT:
-            raise ValueError('Property "{}" value "{}" > PROPERTY_RECURSION_LIMIT ({})' \
-                             .format(property_name, attr, PROPERTY_RECURSION_LIMIT))
-        last_attr = attr_seq[-1]
-        
-        def _getattr(self, attr_seq=attr_seq):
-            obj = self
-            for x in attr_seq:
-                obj = getattr(obj, x)
-            return obj
-        
-        def _setattr(self, value):
-            pre_last_obj = _getattr(self, attr_seq[:-1])
-            setattr(pre_last_obj, last_attr, value)
-            
-        def _delattr(self):
-            pre_last_obj = _getattr(self, attr_seq[:-1])
-            delattr(pre_last_obj, last_attr)
-            
-        args = [None, None, None]
-        if GET:
-            args[0] = _getattr
-        if SET:
-            args[1] = _setattr
-        if DEL:
-            args[2] = _delattr
-            
-        return property(*args)
-    
-    
-class WSMeta(CreateProperties, ExtendAttrs):
-    pass
+from fons.dict_ops import deep_update
+from fons.py import mro as _mro
+
+import copy as _copy
+
+PROPERTY_RECURSION_LIMIT = 2
+
+_ASC = "".join(chr(i) for i in range(128))
+_ALNUM_ = "".join(x for x in _ASC if x.isalnum()) + "_"
+_ALPHA_ = "".join(x for x in _ASC if x.isalpha()) + "_"
+_ALNUM_DOT_ = _ALNUM_ + "."
+
+
+class ExtendAttrs(type):
+    """
+    Deep updates attributes listed in __extend_attrs__, by copying the next attribute found in mro,
+    and then "deep updates" it with the same attr of current class.
+    IMPORTANT!
+    All these attributes are being deepcopied, i.e. all references to previous attrs
+    and their (deep) values are lost.
+    """
+
+    def __new__(cls, name, bases, attrs):
+        mro = _mro(*bases)
+        mro_included = (attrs,) + mro
+        extend_attrs = ExtendAttrs._join(mro_included, "__extend_attrs__")
+
+        # Extend the attributes listed in 'extend_attrs'
+        for _ in extend_attrs:
+            try:
+                nxt_value = next(getattr(x, _) for x in mro if hasattr(x, _))
+            except StopIteration:
+                continue
+            if _ in attrs:
+                attrs[_] = deep_update(nxt_value, attrs[_], copy=True)
+            else:
+                attrs[_] = _copy.deepcopy(nxt_value)
+
+        if "__extend_attrs__" in attrs:
+            # Save the original value
+            attrs["_{}__extend_attrs".format(name)] = attrs["__extend_attrs__"]
+            # Overwrite with new value
+            attrs["__extend_attrs__"] = extend_attrs
+
+        if "__deepcopy_on_init__" in attrs:
+            attrs["_{}__deepcopy_on_init".format(name)] = attrs["__deepcopy_on_init__"]
+            deepcopy_on_init = ExtendAttrs._join(mro_included, "__deepcopy_on_init__")
+            attrs["__deepcopy_on_init__"] = deepcopy_on_init
+
+        # Override object class' __new__ method so that it would deepcopy the attrs
+        # listed in __deepcopy_on_init__ before calling __init__ of the class
+        is_first = not any(isinstance(x, ExtendAttrs) for x in bases)
+        if is_first:
+            ExtendAttrs.override__new__(mro, attrs)
+
+        return super(ExtendAttrs, cls).__new__(cls, name, bases, attrs)
+
+    @staticmethod
+    def _join(bases, name="__extend_attrs__"):
+        """Adds all previous __extend_attrs__ together, and deducts all that start with '-'"""
+        extend_attrs = []
+
+        for cls in reversed(bases):
+            is_dict = isinstance(cls, dict)
+            _name = name if is_dict else "_{}{}".format(cls.__name__, name[:-2])
+            cls_ea = cls.get(_name) if is_dict else getattr(cls, _name, None)
+
+            if cls_ea is None:
+                continue
+
+            if "-" in cls_ea:
+                extend_attrs = []
+
+            deduct = [x for x in cls_ea if len(x) > 1 and x[0] == "-"]
+            add = [x for x in cls_ea if not x.startswith("-")]
+
+            for attr in deduct:
+                try:
+                    extend_attrs.remove(attr[1:])
+                except ValueError:
+                    pass
+
+            for attr in add:
+                if attr not in extend_attrs:
+                    extend_attrs.append(attr)
+
+        return extend_attrs
+
+    @staticmethod
+    def override__new__(mro, attrs):
+        if "__new__" in attrs:
+            orig_new = attrs["__new__"]
+        elif len(mro):
+            orig_new = mro[0].__new__
+        else:
+            orig_new = object.__new__
+
+        def __new_with_deepcopy__(cls, *args, **kw):
+            obj = orig_new(cls)
+            ExtendAttrs.deepcopy_attrs(obj)
+            return obj
+
+        attrs["__new__"] = __new_with_deepcopy__
+
+    @staticmethod
+    def deepcopy_attrs(obj):
+        if not hasattr(obj, "__deepcopy_on_init__"):
+            return
+        for key in obj.__deepcopy_on_init__:
+            if hasattr(obj, key):
+                setattr(obj, key, _copy.deepcopy(getattr(obj, key)))
+
+
+class CreateProperties(type):
+    """Initiates properties listed in __properties__. Also creates sub_to_{x} and unsub_to{x} shortcuts to all
+    methods that match the patterns subscribe_to_{x} / unsubscribe_to_{x}"""
+
+    def __new__(cls, name, bases, attrs):
+        CreateProperties._init_properties(attrs)
+
+        return super(CreateProperties, cls).__new__(cls, name, bases, attrs)
+
+    @staticmethod
+    def _init_properties(attrs):
+        properties = attrs.get("__properties__", [])
+        final_properties = properties[:]
+
+        # Create properties for methods that start with "(un)subscribe_to"
+        for attr in attrs:
+            for startsWith, replaceWith in zip(
+                ["subscribe_to_", "unsubscribe_to_"], ["sub_to_", "unsub_to_"]
+            ):
+                if attr.startswith(startsWith):
+                    property_name = replaceWith + attr[len(startsWith) :]
+                    final_properties.append([property_name, attr, True, False, False])
+
+        for item in final_properties:
+            property_name = item[0]
+            attrs[property_name] = CreateProperties._create_property(*item)
+
+    @staticmethod
+    def _verify_name(name, set=_ALNUM_):
+        if not all(x in set for x in name):
+            raise ValueError(
+                "The property name/value '{}' contains non alnum characters".format(
+                    name
+                )
+            )
+
+        if not all(x[:1] in _ALPHA_ for x in name.split(".")):
+            raise ValueError(
+                "The property name/value '{}' starts with non alpha character".format(
+                    name
+                )
+            )
+
+    @staticmethod
+    def _create_property(property_name, attr, GET=True, SET=True, DEL=True):
+        """
+        This MAY be vulnerable to attack, if the x.y.z... leads to another
+        property (that executes code), or to who knows what object.
+        Make sure that the __properties__ are trusted
+        (which they as pre-assigned class attributes almost certainly should be,
+         unless we are talking about hypothetical dynamic subclassing through an API,
+         or a malevolent github team member in a situation where other members
+         didn't turn attention to __properties__ modification).
+        For that reason the PROPERTY_RECURSION_LIMIT is set to 2."""
+        CreateProperties._verify_name(property_name)
+        # attr can be given as attr_of_self.attr_of_that_attr....
+        CreateProperties._verify_name(attr, _ALNUM_DOT_)
+
+        attr_seq = attr.split(".")
+        if len(attr_seq) > PROPERTY_RECURSION_LIMIT:
+            raise ValueError(
+                'Property "{}" value "{}" > PROPERTY_RECURSION_LIMIT ({})'.format(
+                    property_name, attr, PROPERTY_RECURSION_LIMIT
+                )
+            )
+        last_attr = attr_seq[-1]
+
+        def _getattr(self, attr_seq=attr_seq):
+            obj = self
+            for x in attr_seq:
+                obj = getattr(obj, x)
+            return obj
+
+        def _setattr(self, value):
+            pre_last_obj = _getattr(self, attr_seq[:-1])
+            setattr(pre_last_obj, last_attr, value)
+
+        def _delattr(self):
+            pre_last_obj = _getattr(self, attr_seq[:-1])
+            delattr(pre_last_obj, last_attr)
+
+        args = [None, None, None]
+        if GET:
+            args[0] = _getattr
+        if SET:
+            args[1] = _setattr
+        if DEL:
+            args[2] = _delattr
+
+        return property(*args)
+
+
+class WSMeta(CreateProperties, ExtendAttrs):
+    pass
```

### Comparing `wsclient-0.3.0/wsclient/interpreter.py` & `wsclient-0.4.0/wsclient/interpreter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,61 @@
-from fons.crypto import nonce as _nonce
-
-class Interpreter:
-    #Generate / decode message ids
-    def __init__(self, wrapper):
-        """:type wrapper: WSClient"""
-        self.wc = wrapper
-    
-    def generate_message_id(self, uid, unsubscribe=False):
-        c = self.wc.message['id']['config']
-        kw = {x:y for x,y in c.items() if x in ('uppers','lowers')}
-        #if not c['numbers']: kw['set'] = 'alpha'
-        as_int = c['type'] in ('int',int)
-        set = 'num' if as_int or not any(kw.values()) else 'alnum'
-        nonce = _nonce(c['length']-5,set,**kw)
-        if uid is None:
-            message_id = nonce + ('90000' if set=='num' else _nonce(5,'alpha',**kw))
-        else:
-            message_id = nonce + ('1' if not unsubscribe else '0') + str(uid)
-        if as_int:
-            message_id = int(message_id)
-        return message_id
-    
-    @staticmethod
-    def decode_message_id(message_id):
-        if message_id is None:
-            return (None,None)
-        is_int = isinstance(message_id,int)
-        str_id = str(message_id) if is_int else message_id
-        if (    len(str_id) < 5
-                or str_id[-5] not in ('0','1')
-                or not all(x.isdigit() for x in str_id[-5:])):
-            return (None,None)
-        uid = str_id[-4:]
-        #1: is subscribed; 0: unsubscribed
-        status = 1 if str_id[-5] == '1' else 0
-        return (uid,status)
-    
-    @staticmethod
-    def extend(d, extra):
-        return dict(d, **{k:v for k,v in extra.items() if k not in d})
-    
-    @staticmethod
-    def comma_separate(items, f=None):
-        if isinstance(items,str): items = [items]
-        if f is not None: items = [f(x) for x in items]
-        return ','.join(items)
-    
-    def interpret_variable(self, var):
-        if isinstance(var, str):
-            if var.startswith('m$'):
-                var = var[2:]
-            elif var.startswith('$'):
-                var = var[1:]
-            var = getattr(self.wc, var)
-        return var
+from fons.crypto import nonce as _nonce
+
+
+class Interpreter:
+    # Generate / decode message ids
+    def __init__(self, wrapper):
+        """:type wrapper: WSClient"""
+        self.wc = wrapper
+
+    def generate_message_id(self, uid, unsubscribe=False):
+        c = self.wc.message["id"]["config"]
+        kw = {x: y for x, y in c.items() if x in ("uppers", "lowers")}
+        # if not c['numbers']: kw['set'] = 'alpha'
+        as_int = c["type"] in ("int", int)
+        set = "num" if as_int or not any(kw.values()) else "alnum"
+        nonce = _nonce(c["length"] - 5, set, **kw)
+        if uid is None:
+            message_id = nonce + ("90000" if set == "num" else _nonce(5, "alpha", **kw))
+        else:
+            message_id = nonce + ("1" if not unsubscribe else "0") + str(uid)
+        if as_int:
+            message_id = int(message_id)
+        return message_id
+
+    @staticmethod
+    def decode_message_id(message_id):
+        if message_id is None:
+            return (None, None)
+        is_int = isinstance(message_id, int)
+        str_id = str(message_id) if is_int else message_id
+        if (
+            len(str_id) < 5
+            or str_id[-5] not in ("0", "1")
+            or not all(x.isdigit() for x in str_id[-5:])
+        ):
+            return (None, None)
+        uid = str_id[-4:]
+        # 1: is subscribed; 0: unsubscribed
+        status = 1 if str_id[-5] == "1" else 0
+        return (uid, status)
+
+    @staticmethod
+    def extend(d, extra):
+        return dict(d, **{k: v for k, v in extra.items() if k not in d})
+
+    @staticmethod
+    def comma_separate(items, f=None):
+        if isinstance(items, str):
+            items = [items]
+        if f is not None:
+            items = [f(x) for x in items]
+        return ",".join(items)
+
+    def interpret_variable(self, var):
+        if isinstance(var, str):
+            if var.startswith("m$"):
+                var = var[2:]
+            elif var.startswith("$"):
+                var = var[1:]
+            var = getattr(self.wc, var)
+        return var
```

### Comparing `wsclient-0.3.0/wsclient/sub.py` & `wsclient-0.4.0/wsclient/sub.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,552 +1,642 @@
-import copy as _copy
-import asyncio
-import functools
-import datetime
-dt = datetime.datetime
-td = datetime.timedelta
-
-import fons.log as _log
-from fons.event import Station
-from fons.func import get_arg_count
-
-from .errors import (SubscriptionError, SubscriptionLimitExceeded)
-from .merged import Merged
-from .transport import Request
-
-
-logger,logger2,tlogger,tloggers,tlogger0 = _log.get_standard_5(__name__)
-
-
-class SubscriptionHandler:
-    def __init__(self, wrapper):
-        """:type wrapper: WSClient"""
-        self.wc = wrapper
-        
-        self.subscriptions = []
-        
-        #all uids are in str form and consist of 4 digits
-        self.uids = dict.fromkeys(['0'*(4-len(str(i)))+str(i) for i in range(1,10000)],False)
-        
-
-    async def push_subscriptions(self, cnx=None):
-        cnx_sfx = 'cnx <{}>'.format(cnx.id) if cnx is not None else 'all'
-        self.wc.log('pushing {} subscriptions'.format(cnx_sfx))
-        mergers = set()
-        pushed = []
-        
-        for s in self.subscriptions:
-            if cnx is not None and s.cnx is not cnx:
-                continue
-            if s.merger is not None:
-                if s.merger in mergers:
-                    continue
-                mergers.add(s.merger)
-                s = s.merger
-            self.wc.log('pushing {} to cnx <{}>'.format(s, s.cnx.id))
-            try:
-                await s.push()
-            except Exception as e:
-                logger2.error('{} - could not push {} to cnx <{}>'.format(self.wc.name, s, s.cnx.id))
-                logger.exception(e)
-            else:
-                pushed.append(s)
-            if self.wc.subscription_push_rate_limit:
-                await asyncio.sleep(self.wc.subscription_push_rate_limit)
-        self.wc.log('{} subscriptions pushed'.format(cnx_sfx))
-        
-        return pushed
-        
-        
-    def add_subscription(self, params, *, dependants=[]):
-        """:param params: dict or id_tuple"""
-        if hasattr(params, '__iter__') and not isinstance(params, dict):
-            params = self.wc.cis.parse_id_tuple(params)
-        else:
-            params = params.copy()
-        output = self.wc.transform(params)
-        if output is not None:
-            params = output
-        channel = params['_']
-        self.wc.cis.verify_has(channel)
-        self.wc.cis.verify_input(params)
-        id_tuple = self.wc.cis.create_id_tuple(params)
-        merge = False
-        
-        if self.wc.cis.has_merge_option(channel):
-            merge_index = self.wc.cis.get_value(channel, 'merge_index', 1)
-            #if merge_index <= 1: raise ValueError(merge_index)
-            if isinstance(id_tuple[merge_index], Merged):
-                merge = True
-        elif any(isinstance(x, Merged) for x in id_tuple): 
-            raise ValueError("{} - channel '{}' doesn't accept merged params; got: {}".format(
-                              self.wc.name, channel, params))
-        
-        count = 1
-        merge_limit = self.wc.cis.get_merge_limit(channel)
-        
-        if merge:
-            params_list = []
-            identifiers = self.wc.cis._fetch_subscription_identifiers(channel)
-            p_name = identifiers[merge_index]
-            count = len(params[p_name])
-            if not len(params[p_name]):
-                raise ValueError("{} - got empty merged param: '{}'".format(self.wc.name, p_name))
-            elif merge_limit is not None and count > merge_limit:
-                raise ValueError("{} - param '{}' count > merge_limit [{} > {}]".format(
-                                  self.wc.name, p_name, count, merge_limit))
-            for p_value in params[p_name]:
-                new = _copy.deepcopy(params)
-                new[p_name] = p_value
-                params_list.append(new)
-        else:
-            params_list = [params]
-        
-        
-        free = self.get_total_free_subscription_slots()
-        not_subbed = []
-    
-        for _params in params_list:
-            if self.is_subscribed_to(_params):
-                _s = self.get_subscription(_params)
-                if not dependants:
-                    _s.independently_called = True
-                self.wc.log2('already subbed to: {}'.format(_s.id_tuple))
-            else:
-                not_subbed.append(_params)
-                
-        count = len(not_subbed)
-        if not count:
-            return None
-            
-        if free is not None and count > free:
-            raise SubscriptionLimitExceeded
-        
-        on_creation = self.wc.cis.get_value(channel, 'on_creation')
-        if isinstance(on_creation, str):
-            on_creation = self.wc.ip.interpret_variable(on_creation)
-        
-        if on_creation is not None:
-            _args = [_copy.deepcopy(params)] if get_arg_count(on_creation) else []
-            on_creation(*_args)
-        
-        merge = count > 1
-        if merge:
-            new_params = _copy.deepcopy(params)
-            new_params[p_name] = self.wc.merge([x[p_name] for x in not_subbed])
-        else:
-            new_params = not_subbed[0]
-        
-        cnx = self.find_available_connection(new_params, create=True, count=count)
-        self.wc.log('{} available cnx <{}>'.format(params, cnx.id))
-        subs = [] 
-        
-        for i,_params in enumerate(not_subbed):
-            s = Subscription(_params, self.wc, cnx, dependants=dependants)
-            self.subscriptions.append(s)
-            subs.append(s)
-        
-        if merge:
-            s = SubscriptionMerger(channel, self.wc, cnx, subs, dependants=dependants)
-        
-        dependencies = self.wc.get_dependencies(s)
-        for dep in dependencies:
-            if not self.is_subscribed_to(dep):
-                self.wc.log('adding provider sub {} for {}'.format(dep, s.id_tuple))
-                self.add_subscription(dep, dependants=[s])
-        
-        if self.wc.tp._thread.isAlive() and self.wc.is_active():
-            return s.push()
-        
-        return True
-    
-    
-    def remove_subscription(self, x):
-        """:param x: dict, id_tuple, uid, Request, Subscription, SubscriptionMerger"""
-        #For removing merged subscription, pass SubscriptionMerger instance
-        if hasattr(x, '__iter__') and not isinstance(x, (dict,str,Request)):
-            x = self.wc.cis.parse_id_tuple(x)
-            
-        if isinstance(x, dict):
-            channel = x['_']
-            self.wc.cis.verify_has(channel)
-            self.wc.cis.verify_input(x)
-        
-        if not self.is_subscribed_to(x):
-            return None
-  
-        s = self.get_subscription(x)
-        
-        if getattr(s,'merger',None) is not None:
-            raise SubscriptionError("{} - '{}' cannot be removed because it has merger attached to it.".format(
-                                    self.wc.name, s.id_tuple))
-        if not self.wc.cis.has_unsub_option(s.channel):
-            raise SubscriptionError("{} - '{}' doesn't support unsubscribing.".format(
-                                    self.wc.name, s.channel))
-        if s.dependants or s.is_merger() and any(_s.dependants for _s in s.subscriptions):
-            raise SubscriptionError("{} - '{}' cannot be removed because it has dependants.".format(
-                                    self.wc.name, s.id_tuple))
-
-        self.release_uid(s.uid)
-        if s.is_merger():
-            self.release_uid(_s.uid for _s in s.subscriptions)
-        self.change_subscription_state(s, 0)
-        s.independently_called = False
-        
-        id_tuples = [s.id_tuple] if not s.is_merger() else [_s.id_tuple for _s in s.subscriptions]
-        for id_tuple in id_tuples:
-            try: s_index = next(_i for _i,_s in enumerate(self.subscriptions) if _s.id_tuple == id_tuple)
-            except StopIteration: continue
-            else: del self.subscriptions[s_index]
-        
-        providers = self.find_provider_subs(s)
-        for p in providers:
-            p.remove_dependant(s)
-        
-        for p in providers:
-            if not p.dependants and not p.independently_called:
-                try:
-                    self.wc.log("removing provider sub {} of {}".format(p.id_tuple, s.id_tuple))
-                    self.remove_subscription(p)
-                except Exception as e:
-                    logger.error("{} - could not remove provider sub {} of {}: {}".format(
-                                 self.wc.name, p.id_tuple, s.id_tuple, repr(e)))
-                    logger.exception(e)
-        
-        if self.wc.is_active():
-            return s.unsub()
-        
-        #If no "send" is deployed on cnx, and cnx would NOT be deleted 
-        # (after *compulsory* stopping in "no send" case, as that is the only way to stop its feed),
-        # re-subscribing on the old cnx could cause delay due to the old's "stop" future not having completed yet
-        #Thus to guarantee the fluency it's better to delete the cnx entirely
-        send = self.wc.cis.get_value(s.channel,'send')
-        #Cnx with param variance probably can't be reused
-        #if s.is_merger() and not any(s.cnx is _s.cnx for _s in self.subscriptions):
-        if s.cnx.url and not send and not any(s.cnx is _s.cnx for _s in self.subscriptions):
-            self.wc.cm.remove_connection(s.cnx, delete=True)
-        
-        return True
-    
-    
-    def get_total_free_subscription_slots(self):
-        if self.wc.max_total_subscriptions is not None:
-            return self.wc.max_total_subscriptions - len(self.subscriptions)
-        return None
-    
-    
-    def find_provider_subs(self, s):
-        return [_s for _s in self.subscriptions if s in _s.dependants]
-    
-    
-    def find_available_connection(self, params, create=False, count=1):
-        channel = params['_']
-        is_sub = self.wc.cis.is_subscription(channel)
-        free_slots = self.get_total_free_subscription_slots()
-        if is_sub and free_slots is not None and count > free_slots:
-            raise SubscriptionError
-        
-        cnx = None
-        cfg = self.wc.cis.fetch_connection_config(channel, params)
-        url_factory = cfg['url']
-        
-        for _cnx,_cnxi in self.wc.cm.cnx_infs.items():
-            if is_sub:
-                free_slots = _cnxi.free_subscription_slots
-                if free_slots is not None and free_slots < count:
-                    continue
-            if _cnxi.satisfies(params, url_factory):
-                cnx = _cnx
-                
-        if cnx is None and create: 
-            cnx = self.create_connection(params, cfg)
-        if cnx is None:
-            raise SubscriptionError
-        
-        return cnx
-    
-    
-    def create_connection(self, params, cfg=None):
-        if cfg is None:
-            channel = params['_']
-            cfg = self.wc.cis.fetch_connection_config(channel, params)
-        cnx = self.wc.cm.add_connection(cfg)
-        return cnx
-        
-        
-    def is_subscribed_to(self, x, active=None):
-        """:param x: dict, id_tuple, uid, Request, Subscription, MergedSubscription"""
-        if isinstance(x, Request):
-            if x.is_merger():
-                return any(self.is_subscribed_to(s, active) for s in x.subscriptions)
-            x = x.id_tuple
-        
-        try: s = self.get_subscription(x)
-        except ValueError:
-            return False
-        if active:
-            return s.is_active()
-        else:
-            return True
-        
-        
-    def handle_subscription_ack(self, message_id):
-        #print(r)
-        uid,status = self.wc.ip.decode_message_id(message_id)
-        if uid is None:
-            return
-        try: s = self.get_subscription(uid)
-        except ValueError: 
-            self.wc.log2("uid doesn't exist: {}".format(uid), 'WARN')
-            return
-        auto_activate = self.wc.cis.get_value(s.channel, 'auto_activate')
-        if status and auto_activate != 'on_cnx_activation' and auto_activate:
-            self.change_subscription_state(uid, 1)
-        elif not status:
-            self.change_subscription_state(uid, 0)
-    
-    
-    def change_subscription_state(self, x, state, cnx_active=False, provider_active=True):
-        """
-        :param cnx_active: if True, positive state can only be assigned if subscription's connection is active
-        :param provider_active: -||- all subscription's provider subs are active
-        """
-        #TODO: force state to 0 if not self.is_running() ?
-        s = self.get_subscription(x)
-        prev_state = s.state
-        if prev_state == state:
-            return
-        
-        if state and cnx_active and (s.cnx is None or not s.cnx.is_active()):
-            return
-        
-        if state and provider_active:
-            providers = self.find_provider_subs(s)
-            if not all(p.state for p in providers):
-                return
-        
-        s.state = state
-        
-        if state != prev_state:
-            self.wc.log(s)
-        
-        def data_ops(s):
-            #Fetch necessary data before enabling subscription
-            if state and self.wc.cis.has_fetch_data_on_sub_requirement(s.channel):
-                self.wc.loop.call_soon_threadsafe(functools.partial(
-                    self.wc.fetch_data, s, prev_state))
-            #To make it absolutely sure that the user won't be
-            # using out-dated data
-            if not state and self.wc.cis.has_delete_data_on_unsub_requirement(s.channel):
-                self.wc.loop.call_soon_threadsafe(functools.partial(
-                    self.wc.delete_data, s, prev_state))
-                
-        subs = [s] if not s.is_merger() else s.subscriptions
-        for _s in subs:
-            data_ops(_s)
-        
-        # Dependent subscription is disabled automatically, but enabling is left to user side. 
-        if not state:
-            for dep in s.dependants:
-                self.change_subscription_state(dep, 0)
-    
-    
-    def create_uid(self, reserve=True):
-        uid = next(x for x,v in self.uids.items() if not v)
-        if reserve:
-            self.uids[uid] = True
-        return uid
-    
-    def release_uid(self, uid):
-        self.uids[uid] = False
-    
-
-    def get_subscription(self, x):
-        """:param x: dict, id_tuple, uid, Request, Subscription, MergedSubscription"""
-        if isinstance(x, Subscription):
-            return x
-        if isinstance(x, Request):
-            x = x.id_tuple
-        id_tuple = self.wc.cis.get_subscription_id_tuple(x)
-        
-        s = next((_s for _s in self.subscriptions if _s.id_tuple == id_tuple), None)
-        if s is None:
-            raise ValueError('No subscription match for {}'.format(x))
-        return s
-        
-    def get_subscription_state(self, x):
-        return self.get_subscription(x).state
-
-    def get_subscription_uid(self, x):
-        return self.get_subscription(x).uid
-    
-    async def wait_till_subscription_active(self, x, timeout=None):
-        s = self.get_subscription(x)
-        await s.wait_till_active(timeout)
-    
-    @property
-    def ip(self):
-        return self.wc.ip
-    
-    
-class Subscription(Request):
-    def __init__(self, params, wrapper, cnx, *, dependants=[]):
-        """:type wrapper: WSClient
-           :type cnx: Connection"""
-        super().__init__(params, wrapper, cnx)
-        
-        self.uid = self.wc.sh.create_uid()
-        self.station = Station( [{'channel': 'active', 'id': 0, 'queue': False, 'loops': [0,-1]},
-                                 {'channel': 'inactive', 'id': 0, 'queue': False, 'loops': [0,-1]}],
-                                loops={-1: self.wc._loop, 
-                                        0: self.wc.loop})
-        self.state = self.wc.cis.get_default_subscription_state(self.channel)
-        self.dependants = []
-        self.independently_called = not dependants # this can also be True if it does have dependants
-        for s in dependants:
-            self.add_dependant(s)
-        
-    def add_merger(self, merger):
-        if self.is_active():
-            raise RuntimeError("{} - {} merger can't be added while sub is active".format(
-                                self.wc.name, self.id_tuple))
-        merger.add(self)
-        
-    def remove_merger(self, merger):
-        merger.remove(self)
-    
-    def add_dependant(self, s):
-        if s not in self.dependants:
-            self.dependants.append(s)
-            return True
-        return None
-    
-    def remove_dependant(self, s):
-        if s in self.dependants:
-            self.dependants.remove(s)
-            return True
-        return None
-    
-    def push(self):
-        if self.merger is not None:
-            return self.merger.push()
-        return asyncio.ensure_future(self.wc.tp.send(self, sub=True))
-        
-    def unsub(self):
-        if self.merger is not None:
-            return self.merger.unsub(self)
-        return asyncio.ensure_future(self.wc.tp.send(self, sub=False))
-        
-    def is_active(self):
-        return bool(self.state) # `active/inactive` events aren't set immediately, use `state` instead
-    
-    def _is_active(self):
-        return self.station.get_event('active', 0, loop=0).is_set()
-    
-    def _is_active2(self):
-        return not self.station.get_event('inactive', 0, loop=0).is_set()
-    
-    async def wait_till_active(self, timeout=None):
-        await asyncio.wait_for(self.station.get_event('active', 0).wait(), timeout)
-    
-    def _set_state(self, value):
-        self._state = value
-        active_op = 'set' if value else 'clear'
-        inactive_op = 'clear' if value else 'set'
-        self.station.broadcast_multiple(
-            [
-                {'_': 'active', 'op': active_op},
-                {'_': 'inactive', 'op': inactive_op},
-            ]
-        )
-
-    @property
-    def state(self):
-        return self._state
-    @state.setter
-    def state(self, value):
-        self._set_state(value)
-
-    @property
-    def sub(self):
-        return self.push
-            
-    def __str__(self):
-        return 'Sub({}, state={})'.format(self.id_tuple, self.state)
-    
-    
-class SubscriptionMerger(Subscription):
-    def __init__(self, channel, wrapper, cnx, subs=[], *, dependants=[]):
-        """:type wrapper: WSClient
-           :type cnx: Connection"""
-        id_tuple_kw = wrapper.cis._fetch_subscription_identifiers(channel)
-        merge_index = wrapper.cis.get_value(channel, 'merge_index')
-        merge_index = 1 if merge_index is None else merge_index
-        
-        params = dict(_ = channel, 
-                      **{k: (None if i+1 != merge_index else Merged())
-                         for i,k in enumerate(id_tuple_kw[1:])}
-                      )
-        
-        self.id_tuple_kw = id_tuple_kw
-        self.merge_index = merge_index
-        self.merge_param = id_tuple_kw[self.merge_index]
-        self.subscriptions = []
-        
-        super().__init__(params, wrapper, cnx, dependants=dependants)
-        
-        for s in subs:
-            self.add(s)
-        
-    def add(self, s):
-        if s.wc is not self.wc:
-            raise ValueError('Subscription has different WSClient attached')
-        elif s.channel != self.channel:
-            raise ValueError('Subscription has different channel attached - {}'.format(s.channel))
-        elif s.cnx != self.cnx:
-            raise ValueError('Subscription has different cnx attached')
-        elif s.merger is not None and s.merger is not self:
-            raise ValueError('Subscription has different merger already attached')
-        s.merger = self
-
-        if s not in self.subscriptions:
-            self.subscriptions.append(s)
-            self.params[self.mp] = Merged(self.params[self.mp] + (s.params[self.mp],))
-            self.params.update({k:v for k,v in s.params.items() if k not in ('_',self.mp)})
-            self.update_id_tuple()
-            return True
-        return None
-            
-    def remove(self, s):
-        if s.merger is not None and s.merger is not self:
-            raise ValueError('Subscription has different merger attached.')
-        s.merger = None
-        try: self.subscriptions.remove(s)
-        except ValueError:
-            return None
-        self.params[self.mp] = Merged(x for x in self.params[self.mp] if x != s.params[self.mp])
-        self.update_id_tuple()
-        return True
-    
-    def add_merger(self, merger):
-        raise NotImplementedError
-    
-    def remove_merger(self, merger):
-        raise NotImplementedError
-    
-    def is_merged(self):
-        return True
-    
-    def is_merger(self):
-        return True
-    
-    def update_id_tuple(self):
-        self.id_tuple = tuple(self.params[k] for k in self.id_tuple_kw)
-    
-    def _set_state(self, value):
-        super()._set_state(value)
-        for s in self.subscriptions:
-            s._set_state(value)
-            
-    @property
-    def mp(self):
-        return self.merge_param
+import copy as _copy
+import asyncio
+import functools
+import time
+import datetime
+
+dt = datetime.datetime
+td = datetime.timedelta
+
+import fons.log as _log
+from fons.event import Station
+from fons.func import get_arg_count
+
+from .errors import SubscriptionError, SubscriptionLimitExceeded
+from .merged import Merged
+from .transport import Request
+
+
+logger, logger2, tlogger, tloggers, tlogger0 = _log.get_standard_5(__name__)
+
+
+class SubscriptionHandler:
+    def __init__(self, wrapper):
+        """:type wrapper: WSClient"""
+        self.wc = wrapper
+
+        self.subscriptions = []
+
+        # all uids are in str form and consist of 4 digits
+        self.uids = dict.fromkeys(
+            ["0" * (4 - len(str(i))) + str(i) for i in range(1, 10000)], False
+        )
+
+    async def push_subscriptions(self, cnx=None):
+        cnx_sfx = "cnx <{}>".format(cnx.id) if cnx is not None else "all"
+        self.wc.log("pushing {} subscriptions".format(cnx_sfx))
+        mergers = set()
+        pushed = []
+
+        for s in self.subscriptions:
+            if cnx is not None and s.cnx is not cnx:
+                continue
+            if s.merger is not None:
+                if s.merger in mergers:
+                    continue
+                mergers.add(s.merger)
+                s = s.merger
+            self.wc.log("pushing {} to cnx <{}>".format(s, s.cnx.id))
+            try:
+                await s.push()
+            except Exception as e:
+                logger2.error(
+                    "{} - could not push {} to cnx <{}>".format(
+                        self.wc.name, s, s.cnx.id
+                    )
+                )
+                logger.exception(e)
+            else:
+                pushed.append(s)
+            if self.wc.subscription_push_rate_limit:
+                await asyncio.sleep(self.wc.subscription_push_rate_limit)
+        self.wc.log("{} subscriptions pushed".format(cnx_sfx))
+
+        return pushed
+
+    def add_subscription(self, params, *, dependants=[]):
+        """:param params: dict or id_tuple"""
+        if hasattr(params, "__iter__") and not isinstance(params, dict):
+            params = self.wc.cis.parse_id_tuple(params)
+        else:
+            params = params.copy()
+        output = self.wc.transform(params)
+        if output is not None:
+            params = output
+        channel = params["_"]
+        self.wc.cis.verify_has(channel)
+        self.wc.cis.verify_input(params)
+        id_tuple = self.wc.cis.create_id_tuple(params)
+        merge = False
+
+        if self.wc.cis.has_merge_option(channel):
+            merge_index = self.wc.cis.get_value(channel, "merge_index", 1)
+            # if merge_index <= 1: raise ValueError(merge_index)
+            if isinstance(id_tuple[merge_index], Merged):
+                merge = True
+        elif any(isinstance(x, Merged) for x in id_tuple):
+            raise ValueError(
+                "{} - channel '{}' doesn't accept merged params; got: {}".format(
+                    self.wc.name, channel, params
+                )
+            )
+
+        count = 1
+        merge_limit = self.wc.cis.get_merge_limit(channel)
+
+        if merge:
+            params_list = []
+            identifiers = self.wc.cis._fetch_subscription_identifiers(channel)
+            p_name = identifiers[merge_index]
+            count = len(params[p_name])
+            if not len(params[p_name]):
+                raise ValueError(
+                    "{} - got empty merged param: '{}'".format(self.wc.name, p_name)
+                )
+            elif merge_limit is not None and count > merge_limit:
+                raise ValueError(
+                    "{} - param '{}' count > merge_limit [{} > {}]".format(
+                        self.wc.name, p_name, count, merge_limit
+                    )
+                )
+            for p_value in params[p_name]:
+                new = _copy.deepcopy(params)
+                new[p_name] = p_value
+                params_list.append(new)
+        else:
+            params_list = [params]
+
+        free = self.get_total_free_subscription_slots()
+        not_subbed = []
+
+        for _params in params_list:
+            if self.is_subscribed_to(_params):
+                _s = self.get_subscription(_params)
+                if not dependants:
+                    _s.independently_called = True
+                self.wc.log2("already subbed to: {}".format(_s.id_tuple))
+            else:
+                not_subbed.append(_params)
+
+        count = len(not_subbed)
+        if not count:
+            return None
+
+        if free is not None and count > free:
+            raise SubscriptionLimitExceeded
+
+        on_creation = self.wc.cis.get_value(channel, "on_creation")
+        if isinstance(on_creation, str):
+            on_creation = self.wc.ip.interpret_variable(on_creation)
+
+        if on_creation is not None:
+            _args = [_copy.deepcopy(params)] if get_arg_count(on_creation) else []
+            on_creation(*_args)
+
+        merge = count > 1
+        if merge:
+            new_params = _copy.deepcopy(params)
+            new_params[p_name] = self.wc.merge([x[p_name] for x in not_subbed])
+        else:
+            new_params = not_subbed[0]
+
+        cnx = self.find_available_connection(new_params, create=True, count=count)
+        self.wc.log("{} available cnx <{}>".format(params, cnx.id))
+        subs = []
+
+        for i, _params in enumerate(not_subbed):
+            s = Subscription(_params, self.wc, cnx, dependants=dependants)
+            self.subscriptions.append(s)
+            subs.append(s)
+
+        if merge:
+            s = SubscriptionMerger(channel, self.wc, cnx, subs, dependants=dependants)
+
+        dependencies = self.wc.get_dependencies(s)
+        for dep in dependencies:
+            if not self.is_subscribed_to(dep):
+                self.wc.log("adding provider sub {} for {}".format(dep, s.id_tuple))
+                self.add_subscription(dep, dependants=[s])
+
+        if self.wc.tp._thread.is_alive() and self.wc.is_active():
+            return s.push()
+
+        return True
+
+    def remove_subscription(self, x):
+        """:param x: dict, id_tuple, uid, Request, Subscription, SubscriptionMerger"""
+        # For removing merged subscription, pass SubscriptionMerger instance
+        if hasattr(x, "__iter__") and not isinstance(x, (dict, str, Request)):
+            x = self.wc.cis.parse_id_tuple(x)
+
+        if isinstance(x, dict):
+            channel = x["_"]
+            self.wc.cis.verify_has(channel)
+            self.wc.cis.verify_input(x)
+
+        if not self.is_subscribed_to(x):
+            return None
+
+        s = self.get_subscription(x)
+
+        if getattr(s, "merger", None) is not None:
+            raise SubscriptionError(
+                "{} - '{}' cannot be removed because it has merger attached to it.".format(
+                    self.wc.name, s.id_tuple
+                )
+            )
+        if not self.wc.cis.has_unsub_option(s.channel):
+            raise SubscriptionError(
+                "{} - '{}' doesn't support unsubscribing.".format(
+                    self.wc.name, s.channel
+                )
+            )
+        if (
+            s.dependants
+            or s.is_merger()
+            and any(_s.dependants for _s in s.subscriptions)
+        ):
+            raise SubscriptionError(
+                "{} - '{}' cannot be removed because it has dependants.".format(
+                    self.wc.name, s.id_tuple
+                )
+            )
+
+        self.release_uid(s.uid)
+        if s.is_merger():
+            self.release_uid(_s.uid for _s in s.subscriptions)
+        self.change_subscription_state(s, 0)
+        s.independently_called = False
+
+        id_tuples = (
+            [s.id_tuple]
+            if not s.is_merger()
+            else [_s.id_tuple for _s in s.subscriptions]
+        )
+        for id_tuple in id_tuples:
+            try:
+                s_index = next(
+                    _i
+                    for _i, _s in enumerate(self.subscriptions)
+                    if _s.id_tuple == id_tuple
+                )
+            except StopIteration:
+                continue
+            else:
+                del self.subscriptions[s_index]
+
+        providers = self.find_provider_subs(s)
+        for p in providers:
+            p.remove_dependant(s)
+
+        for p in providers:
+            if not p.dependants and not p.independently_called:
+                try:
+                    self.wc.log(
+                        "removing provider sub {} of {}".format(p.id_tuple, s.id_tuple)
+                    )
+                    self.remove_subscription(p)
+                except Exception as e:
+                    logger.error(
+                        "{} - could not remove provider sub {} of {}: {}".format(
+                            self.wc.name, p.id_tuple, s.id_tuple, repr(e)
+                        )
+                    )
+                    logger.exception(e)
+
+        if self.wc.is_active():
+            return s.unsub()
+
+        # If no "send" is deployed on cnx, and cnx would NOT be deleted
+        # (after *compulsory* stopping in "no send" case, as that is the only way to stop its feed),
+        # re-subscribing on the old cnx could cause delay due to the old's "stop" future not having completed yet
+        # Thus to guarantee the fluency it's better to delete the cnx entirely
+        send = self.wc.cis.get_value(s.channel, "send")
+        # Cnx with param variance probably can't be reused
+        # if s.is_merger() and not any(s.cnx is _s.cnx for _s in self.subscriptions):
+        if (
+            s.cnx.url
+            and not send
+            and not any(s.cnx is _s.cnx for _s in self.subscriptions)
+        ):
+            self.wc.cm.remove_connection(s.cnx, delete=True)
+
+        return True
+
+    def get_total_free_subscription_slots(self):
+        if self.wc.max_total_subscriptions is not None:
+            return self.wc.max_total_subscriptions - len(self.subscriptions)
+        return None
+
+    def find_provider_subs(self, s):
+        return [_s for _s in self.subscriptions if s in _s.dependants]
+
+    def find_available_connection(self, params, create=False, count=1):
+        channel = params["_"]
+        is_sub = self.wc.cis.is_subscription(channel)
+        free_slots = self.get_total_free_subscription_slots()
+        if is_sub and free_slots is not None and count > free_slots:
+            raise SubscriptionError
+
+        cnx = None
+        cfg = self.wc.cis.fetch_connection_config(channel, params)
+        url_factory = cfg["url"]
+
+        for _cnx, _cnxi in self.wc.cm.cnx_infs.items():
+            if is_sub:
+                free_slots = _cnxi.free_subscription_slots
+                if free_slots is not None and free_slots < count:
+                    continue
+            if _cnxi.satisfies(params, url_factory):
+                cnx = _cnx
+
+        if cnx is None and create:
+            cnx = self.create_connection(params, cfg)
+        if cnx is None:
+            raise SubscriptionError
+
+        return cnx
+
+    def create_connection(self, params, cfg=None):
+        if cfg is None:
+            channel = params["_"]
+            cfg = self.wc.cis.fetch_connection_config(channel, params)
+        cnx = self.wc.cm.add_connection(cfg)
+        return cnx
+
+    def is_subscribed_to(self, x, active=None):
+        """:param x: dict, id_tuple, uid, Request, Subscription, MergedSubscription"""
+        if isinstance(x, Request):
+            if x.is_merger():
+                return any(self.is_subscribed_to(s, active) for s in x.subscriptions)
+            x = x.id_tuple
+
+        try:
+            s = self.get_subscription(x)
+        except ValueError:
+            return False
+        if active:
+            return s.is_active()
+        else:
+            return True
+
+    def handle_subscription_ack(self, message_id):
+        # print(r)
+        uid, status = self.wc.ip.decode_message_id(message_id)
+        if uid is None:
+            return
+        try:
+            s = self.get_subscription(uid)
+        except ValueError:
+            self.wc.log2("uid doesn't exist: {}".format(uid), "WARN")
+            return
+        auto_activate = self.wc.cis.get_value(s.channel, "auto_activate")
+        if status and auto_activate != "on_cnx_activation" and auto_activate:
+            self.change_subscription_state(uid, 1)
+        elif not status:
+            self.change_subscription_state(uid, 0)
+
+    def change_subscription_state(
+        self, x, state, cnx_active=False, provider_active=True
+    ):
+        """
+        :param cnx_active: if True, positive state can only be assigned if subscription's connection is active
+        :param provider_active: -||- all subscription's provider subs are active
+        """
+        # TODO: force state to 0 if not self.is_running() ?
+        s = self.get_subscription(x)
+        prev_state = s.state
+        if prev_state == state:
+            return
+
+        if state and cnx_active and (s.cnx is None or not s.cnx.is_active()):
+            return
+
+        if state and provider_active:
+            providers = self.find_provider_subs(s)
+            if not all(p.state for p in providers):
+                return
+
+        s.state = state
+
+        if state != prev_state:
+            self.wc.log(s)
+
+        def data_ops(s):
+            # Fetch necessary data before enabling subscription
+            if state and self.wc.cis.has_fetch_data_on_sub_requirement(s.channel):
+                self.wc.loop.call_soon_threadsafe(
+                    functools.partial(self.wc.fetch_data, s, prev_state)
+                )
+            # To make it absolutely sure that the user won't be
+            # using out-dated data
+            if not state and self.wc.cis.has_delete_data_on_unsub_requirement(
+                s.channel
+            ):
+                self.wc.loop.call_soon_threadsafe(
+                    functools.partial(self.wc.delete_data, s, prev_state)
+                )
+
+        subs = [s] if not s.is_merger() else s.subscriptions
+        for _s in subs:
+            data_ops(_s)
+
+        # Dependent subscription is disabled automatically, but enabling is left to user side.
+        if not state:
+            for dep in s.dependants:
+                self.change_subscription_state(dep, 0)
+
+    def create_uid(self, reserve=True):
+        uid = next(x for x, v in self.uids.items() if not v)
+        if reserve:
+            self.uids[uid] = True
+        return uid
+
+    def release_uid(self, uid):
+        self.uids[uid] = False
+
+    def get_subscription(self, x):
+        """:param x: dict, id_tuple, uid, Request, Subscription, MergedSubscription"""
+        if isinstance(x, Subscription):
+            return x
+        if isinstance(x, Request):
+            x = x.id_tuple
+        id_tuple = self.wc.cis.get_subscription_id_tuple(x)
+
+        s = next((_s for _s in self.subscriptions if _s.id_tuple == id_tuple), None)
+        if s is None:
+            raise ValueError("No subscription match for {}".format(x))
+        return s
+
+    def get_subscription_state(self, x):
+        return self.get_subscription(x).state
+
+    def get_subscription_uid(self, x):
+        return self.get_subscription(x).uid
+
+    async def wait_till_subscription_active(self, x, timeout=None):
+        s = self.get_subscription(x)
+        await s.wait_till_active(timeout)
+
+    async def wait_till_subscriptions_active(self, subscriptions):
+        """:param subcriptions: [subscription, ...] or {subcription: timeout, ...}"""
+        timeouts_by_sub = subscriptions
+        if not isinstance(subscriptions, dict):
+            timeouts_by_sub = dict.fromkeys(subscriptions, None)
+        timeouts_by_sub = {
+            self.get_subscription(x): timeout for x, timeout in timeouts_by_sub.items()
+        }
+        started = time.time()
+        while True:
+            not_active = [s for s in timeouts_by_sub if not s.state]
+            if not not_active:
+                break
+            elapsed = time.time() - started
+            exceeded = [
+                s
+                for s in not_active
+                if timeouts_by_sub[s] is not None and elapsed > timeouts_by_sub[s]
+            ]
+            if exceeded:
+                raise asyncio.TimeoutError(
+                    "Subcription(s) {} have exceeded their timeout".format(exceeded)
+                )
+            await asyncio.sleep(0.05)
+
+    @property
+    def ip(self):
+        return self.wc.ip
+
+
+class Subscription(Request):
+    def __init__(self, params, wrapper, cnx, *, dependants=[]):
+        """:type wrapper: WSClient
+        :type cnx: Connection"""
+        super().__init__(params, wrapper, cnx)
+
+        self.uid = self.wc.sh.create_uid()
+        self.station = Station(
+            [
+                {"channel": "active", "id": 0, "queue": False, "loops": [0, -1]},
+                {"channel": "inactive", "id": 0, "queue": False, "loops": [0, -1]},
+            ],
+            loops={-1: self.wc._loop, 0: self.wc.loop},
+        )
+        self.state = self.wc.cis.get_default_subscription_state(self.channel)
+        self.dependants = []
+        self.independently_called = (
+            not dependants
+        )  # this can also be True if it does have dependants
+        for s in dependants:
+            self.add_dependant(s)
+
+    def add_merger(self, merger):
+        if self.is_active():
+            raise RuntimeError(
+                "{} - {} merger can't be added while sub is active".format(
+                    self.wc.name, self.id_tuple
+                )
+            )
+        merger.add(self)
+
+    def remove_merger(self, merger):
+        merger.remove(self)
+
+    def add_dependant(self, s):
+        if s not in self.dependants:
+            self.dependants.append(s)
+            return True
+        return None
+
+    def remove_dependant(self, s):
+        if s in self.dependants:
+            self.dependants.remove(s)
+            return True
+        return None
+
+    def push(self):
+        if self.merger is not None:
+            return self.merger.push()
+        return asyncio.ensure_future(self.wc.tp.send(self, sub=True))
+
+    def unsub(self):
+        if self.merger is not None:
+            return self.merger.unsub(self)
+        return asyncio.ensure_future(self.wc.tp.send(self, sub=False))
+
+    def is_active(self):
+        return bool(
+            self.state
+        )  # `active/inactive` events aren't set immediately, use `state` instead
+
+    def _is_active(self):
+        return self.station.get_event("active", 0, loop=0).is_set()
+
+    def _is_active2(self):
+        return not self.station.get_event("inactive", 0, loop=0).is_set()
+
+    async def wait_till_active(self, timeout=None):
+        await asyncio.wait_for(self.station.get_event("active", 0).wait(), timeout)
+
+    def _set_state(self, value):
+        self._state = value
+        active_op = "set" if value else "clear"
+        inactive_op = "clear" if value else "set"
+        self.station.broadcast_multiple(
+            [
+                {"_": "active", "op": active_op},
+                {"_": "inactive", "op": inactive_op},
+            ]
+        )
+
+    @property
+    def state(self):
+        return self._state
+
+    @state.setter
+    def state(self, value):
+        self._set_state(value)
+
+    @property
+    def sub(self):
+        return self.push
+
+    def __str__(self):
+        return "Sub({}, state={})".format(self.id_tuple, self.state)
+
+
+class SubscriptionMerger(Subscription):
+    def __init__(self, channel, wrapper, cnx, subs=[], *, dependants=[]):
+        """:type wrapper: WSClient
+        :type cnx: Connection"""
+        id_tuple_kw = wrapper.cis._fetch_subscription_identifiers(channel)
+        merge_index = wrapper.cis.get_value(channel, "merge_index")
+        merge_index = 1 if merge_index is None else merge_index
+
+        params = dict(
+            _=channel,
+            **{
+                k: (None if i + 1 != merge_index else Merged())
+                for i, k in enumerate(id_tuple_kw[1:])
+            }
+        )
+
+        self.id_tuple_kw = id_tuple_kw
+        self.merge_index = merge_index
+        self.merge_param = id_tuple_kw[self.merge_index]
+        self.subscriptions = []
+
+        super().__init__(params, wrapper, cnx, dependants=dependants)
+
+        for s in subs:
+            self.add(s)
+
+    def add(self, s):
+        if s.wc is not self.wc:
+            raise ValueError("Subscription has different WSClient attached")
+        elif s.channel != self.channel:
+            raise ValueError(
+                "Subscription has different channel attached - {}".format(s.channel)
+            )
+        elif s.cnx != self.cnx:
+            raise ValueError("Subscription has different cnx attached")
+        elif s.merger is not None and s.merger is not self:
+            raise ValueError("Subscription has different merger already attached")
+        s.merger = self
+
+        if s not in self.subscriptions:
+            self.subscriptions.append(s)
+            self.params[self.mp] = Merged(self.params[self.mp] + (s.params[self.mp],))
+            self.params.update(
+                {k: v for k, v in s.params.items() if k not in ("_", self.mp)}
+            )
+            self.update_id_tuple()
+            return True
+        return None
+
+    def remove(self, s):
+        if s.merger is not None and s.merger is not self:
+            raise ValueError("Subscription has different merger attached.")
+        s.merger = None
+        try:
+            self.subscriptions.remove(s)
+        except ValueError:
+            return None
+        self.params[self.mp] = Merged(
+            x for x in self.params[self.mp] if x != s.params[self.mp]
+        )
+        self.update_id_tuple()
+        return True
+
+    def add_merger(self, merger):
+        raise NotImplementedError
+
+    def remove_merger(self, merger):
+        raise NotImplementedError
+
+    def is_merged(self):
+        return True
+
+    def is_merger(self):
+        return True
+
+    def update_id_tuple(self):
+        self.id_tuple = tuple(self.params[k] for k in self.id_tuple_kw)
+
+    def _set_state(self, value):
+        super()._set_state(value)
+        for s in self.subscriptions:
+            s._set_state(value)
+
+    @property
+    def mp(self):
+        return self.merge_param
```

### Comparing `wsclient-0.3.0/wsclient/transport.py` & `wsclient-0.4.0/wsclient/transport.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,578 +1,711 @@
-from fons.aio import call_via_loop
-from fons.debug import (trylog, wrap_trylog)
-from fons.dict_ops import deep_get
-from fons.errors import TerminatedException
-from fons.event import (Station, force_put)
-from fons.threads import EliThread
-import fons.log as _log
-
-import sys
-import asyncio
-import copy as _copy
-import functools
-from collections import defaultdict
-
-from .sub import Merged
-
-logger,logger2,tlogger,tloggers,tlogger0 = _log.get_standard_5(__name__)
-
-# Number of WSClient objects per thread. For infinite set to 0.
-sockets_per_thread = 1
-threads = set()
-_quit_command = object()
-
-
-class Transport:
-    def __init__(self, wrapper):
-        """:type wrapper: WSClient"""
-        self.wc = wrapper
-            
-        # If param `_loop` was given in config, and a thread with such loop already exists,
-        # share that thread
-        _loop = getattr(self.wc,'_loop',None)
-        thread = next((x for x in threads if _loop == x._loop),None)
-        
-        if thread is None:
-            try: thread = min(threads, key=lambda x: x.socket_count)
-            except ValueError:
-                thread = None
-            if thread is not None and sockets_per_thread > 0 and \
-                    thread.socket_count >= sockets_per_thread:
-                thread = None
-        
-        if thread is not None:
-            self._thread = thread
-        else:
-            if _loop is None: 
-                _loop = asyncio.new_event_loop()
-            self._thread = EliThread(target=_loop.run_forever, loop=_loop,
-                                     daemon=True, name='{}Thread'.format(self.wc.name))
-            self._thread.socket_count = 0
-            threads.add(self._thread)
-        
-        self.wc._loop = self._thread._loop
-        
-        #"_" beginning of an attr signifies that _thread._loop is used
-        self._event_queue = asyncio.Queue(0, loop=self.wc._loop)
-        self.recv_queue = asyncio.Queue(0, loop=self.wc.loop)
-        self.send_queue = asyncio.Queue(self.wc.queue_maxsizes.get('send',0), loop=self.wc.loop)
-        self._send_event = asyncio.Event(loop=self.wc._loop)
-        
-        self._event_queue.name = '{}[EQ]'.format(self.wc.name)
-        self.recv_queue.name = '{}[RQ]'.format(self.wc.name)
-        self.send_queue.name = '{}[SQ]'.format(self.wc.name)
-        
-        #These are the two main queues:
-        # event : receives ConnectionEvent from all (active) connections
-        #         can also receive Event when evoking self.wc.broadcast_event(..)
-        #         can be listened on using self.wc.listen()
-        # recv : receives websocket inputs (wrapped with Response) from all (active) connections
-        #        self.wc.handle receives from it
-        #For adding more queues, use self.wc.add_event_queue / self.wc.add_recv_queue
-        #
-        self.user_event_queue = ueq = \
-            asyncio.Queue(self.wc.queue_maxsizes.get('event',100), loop=self.wc.loop)
-        ueq.name = '{}[UEQ]'.format(self.wc.name)
-        ueq.warn = False
-        
-        self.station = \
-            Station([{'channel': 'event', 'id': 0, 'queue': ueq, 'event': False, 'loops': [0]},
-                     {'channel': 'recv', 'id': 0, 'queue': False, 'event': None, 'loops': [0]},
-                     {'channel': 'empty', 'id': 0, 'queue': False, 'event': None, 'loops': [0]},
-                     {'channel': 'running', 'id': 0, 'queue': False, 'event': None, 'loops': [0,-1]},
-                     {'channel': 'stopped', 'id': 0, 'queue': False, 'event': None, 'loops': [0,-1]},
-                     {'channel': 'active', 'id': 0, 'queue': False, 'event': None, 'loops': [0,-1]},
-                     {'channel': 'inactive', 'id': 0, 'queue': False, 'event': None, 'loops': [0,-1]},],
-                    default_queue_size = 100,
-                    loops = {0: self.wc.loop, -1: self.wc._loop},
-                    name = self.wc.name+'[Station]')
-        
-        self.station.broadcast('inactive')
-        self.station.broadcast('stopped')
-        self.waiters = {}
-        self.futures = {}
-    
-    
-    async def start(self):
-        if 'stop' in self.futures:
-            try: await self.futures['stop']
-            except Exception: pass
-        
-        if 'start' in self.futures:
-            return await self.futures['start']
-            
-        self.futures['start'] = asyncio.Future()
-        f1 = f2 = None
-        try:
-            self.wc.log('starting')
-            self.station.broadcast('running')
-            self.station.broadcast('stopped', op='clear')
-    
-            (await self.wc.on_start()) if asyncio.iscoroutinefunction(self.wc.on_start) else self.wc.on_start()
-    
-            _loop = self._thread._loop
-            f1 = call_via_loop(wrap_trylog(self._main), loop=_loop, module='asyncio')
-            f2 = call_via_loop(self.process_events, loop=_loop, module='asyncio')
-            
-            if not self._thread.isAlive():
-                self._thread.start()
-    
-            await self.process_responses()
-            
-            await asyncio.wait([f1,f2])
-            
-        finally:
-            if f1 is not None:
-                f1.cancel()
-            if f2 is not None:
-                f2.cancel()
-            if sys.exc_info()[1] is None:
-                self.futures['start'].set_result(None)
-            else:
-                self.futures['start'].set_exception(sys.exc_info()[1])
-            del self.futures['start']
-            self.station.broadcast('running', op='clear')
-            self.station.broadcast('stopped')
-        
-        
-    async def _main(self):
-        # This runs in self._thread
-        loop = self.wc.loop
-        _loop = asyncio.get_event_loop()
-        
-        # .send() is rooted via .send_queue
-        async def _send(future, params, wait, id, cnx, sub):
-            """:type future: asyncio.Future"""
-            try: r = await self.send(params, wait, id, cnx, sub)
-            except Exception as e:
-                self.wc.log('thread .send() error occurred: {}'.format(repr(e)), 'ERROR')
-                self.wc.log(e)
-                loop.call_soon_threadsafe(
-                    functools.partial(future.set_exception, e))
-            else: 
-                loop.call_soon_threadsafe(
-                    functools.partial(future.set_result, r))
-        
-        # receives updates from the queue, sends them.
-        async def _fire_from_send_queue():
-            while not self.wc._closed:
-                # get from queue via the main loop
-                fut = call_via_loop(self.send_queue.get,
-                                    module='asyncio',
-                                    loop=loop,)
-                item = await fut
-                if item is _quit_command:
-                    break
-                future,params,wait,id,cnx,sub = item
-                asyncio.ensure_future(
-                    _send(future,params,wait,id,cnx,sub))
-        
-        # Start firing right now (allow user initiated sending) before pushing
-        # the subs, as the .wc.handle method (which runs outside of the ._thread)
-        # might need to respond to some of the messages received during the pushing
-        fire = asyncio.ensure_future(_fire_from_send_queue())
-        
-        self.station.broadcast('active')
-        self.station.broadcast('inactive', op='clear')
-        self.wc.broadcast_event('active', 1)
-        
-        try:
-            await call_via_loop(self.wc.wait_till_active, (5,),
-                                loop=self.wc.loop, module='asyncio')
-            await self.wc.wait_till_active(1)
-            # Connections will be started when subscriptions are being pushed
-            # (in .send method). Note that since this here is running in ._thread,
-            # the subscription out messages are NOT sent via the queue.
-            await self.wc.sh.push_subscriptions()
-            await fire
-        finally:
-            fire.cancel()
-            self.station.broadcast('active', op='clear')
-            self.station.broadcast('inactive')
-            self.wc.broadcast_event('active', 0)
-            self.wc.log('stopped')
-        
-    
-    async def process_responses(self):
-        # Process received results from connections. This runs in the main loop (self.loop)
-        self.wc.log2('starting response processing')
-        iscoro = asyncio.iscoroutinefunction(self.wc.handle)
-        recv = None
-        
-        while not self.wc._closed:
-            poll_interval = self.wc.connection_defaults['poll_interval']
-            if recv is None:
-                recv = asyncio.ensure_future(self.recv_queue.get())
-                
-            done,pending = await asyncio.wait([recv], timeout=poll_interval)
-            if not recv.done():
-                self.station.broadcast('empty')
-                self.wc.broadcast_event('socket', 'empty')
-                continue
-            
-            R = recv.result()
-            recv = None
-            if R is _quit_command:
-                break
-            
-            try:
-                if iscoro:
-                    await self.wc.handle(R)
-                else:
-                    self.wc.handle(R)
-            except Exception as e:
-                str_r = str(R.data)
-                dots = '...' if len(str_r) > 200 else ''
-                logger2.error('{} - {} while handling response: {}{}'.format(
-                    self.wc.name, e.__class__.__name__, str_r[:200], dots))
-                logger.error(str_r)
-                logger.exception(e)
-            else:
-                message_id = self.wc.extract_message_id(R)
-                if message_id is not None:
-                    errors = self.wc.extract_errors(R)
-                    error = errors if isinstance(errors, Exception) else \
-                                (errors[0] if len(errors) else None)
-                    ftw = functools.partial(
-                        self.forward_to_waiters, message_id, R, error=error, remove=True, copy=1)
-                    self.wc._loop.call_soon_threadsafe(
-                        functools.partial(trylog, ftw))
-                self.station.broadcast('recv')
-        
-        if recv is not None:
-            recv.cancel()
-    
-    
-    async def process_events(self):
-        # Process events from connections. This runs in self._thread
-        self.wc.log2('starting event processing')
-        activation_count = defaultdict(int)
-        
-        while not self.wc._closed:
-            e = await self._event_queue.get()
-            if e is _quit_command:
-                break
-            
-            try: cnx = self.wc.cm.connections[e.id]
-            except KeyError: continue
-            
-            if e.type == 'socket' and e.data == 0:
-                for s in self.wc.sh.subscriptions:
-                    if s.cnx is cnx:
-                        self.wc.sh.change_subscription_state(s, 0)
-                try: self.wc.cm.cnx_infs[cnx].authenticated = False
-                except KeyError: pass
-                        
-            elif e.type == 'socket' and e.data == 1:
-                # Do not push on first notification,
-                # as during that time *all* subscriptions are being pushed anyway
-                pushed = None
-                if activation_count[cnx]:
-                    pushed = await self.wc.sh.push_subscriptions(cnx)
-                    
-                for s in self.wc.sh.subscriptions:
-                    if s.cnx is cnx:
-                        v = self.wc.cis.get_value(s.channel, 'auto_activate')
-                        if v == 'on_cnx_activation' and (pushed is None or s in pushed):
-                            self.wc.sh.change_subscription_state(s, 1)
-                        
-                activation_count[cnx] += 1
-                
-            elif e.type == 'running' and e.data == 0:
-                activation_count[cnx] = 0
-            
-            
-    async def send(self, params, wait=False, id=None, cnx=None, sub=None):
-        """
-           :type params: dict, Request, Subscription
-           :type cnx: Connection
-           :param params: 
-             must contain '_' key; also accepts Subscription object
-           :param wait: 
-             False : don't wait
-             'default', True->'default', None, of type int/float: timeout to wait
-             'return': doesn't wait, but returns the waiter
-             if signalr/socketio is enabled then id system is probably not implementable (leave wait to False).
-           :param id:
-             custom id to be attached to the waiter. in that case user must forward the response to
-             the waiter manually (e.g. through .handle)
-             if channel sends multiple messages, id may be given as [id0, id1, ..]
-           :param cnx: 
-             may be specified if params is dict, otherwise cnx of given request will be used 
-           :param sub:
-             if subscription, True for subbing, False for unsubbing
-        """
-        if isinstance(params, dict):
-            params = params.copy()
-            output = self.wc.transform(params)
-            if output is not None:
-                params = output
-        
-        if isinstance(params, dict) and cnx is None:
-            cnx = self.wc.sh.find_available_connection(params, create=True)
-            
-        rq = Request(params, self.wc, cnx) if not isinstance(params, Request) else params
-        
-        #Forward to thread
-        if not self._is_in_thread_loop():
-            fut = asyncio.Future()
-            await self.send_queue.put( (fut, rq, wait, id, cnx, sub) )
-            return await fut
-        
-        params = rq.params
-        cnx = rq.cnx
-        channel = rq.channel
-        cnxi = self.wc.cm.cnx_infs[cnx]
-        send = self.wc.cis.get_value(channel ,'send')
-        drop =  self.wc.cis.get_value(channel, 'drop_unused_connection', not send)
-        
-        if not cnx.is_running() and (sub is None or sub):
-            try: cnx.start()
-            except RuntimeError: pass
-            await cnx.wait_till_active(cnx.connect_timeout)
-        elif (sub is not None and not sub) and cnx.url and drop:
-            # Due to param variance difference old connections would not satisfy
-            # the new variance, and would remain unused
-            # if rq.is_merger() and not any(_s.merger is not rq and _s.cnx is cnx
-            #                               for _s in self.wc.sh.subscriptions):
-            if not any(cnx is _s.cnx for _s in self.wc.sh.subscriptions):
-                self.wc.cm.remove_connection(cnx, True)
-            if cnx.is_running():
-                await cnx.stop()
-        
-        wait = 'default' if wait is True else wait
-        add_waiter = wait is not False
-        return_waiter = wait in ('return','return-waiter','return_waiter','return waiter')
-        
-        def _return():
-            if not add_waiter or not return_waiter: 
-                return None
-            else:
-                f = asyncio.Future()
-                f.set_result(None)
-                return f
-        
-        if not cnx.url or not send:
-            return _return()
-        
-        packs = self.wc.encode(rq, sub)
-        # WSClient.encode should return `None` if this specific request is not meant to be sent
-        if packs is None:
-            return _return()
-        
-        if not isinstance(packs, Merged):
-            packs = [packs]
-        single = (len(packs) == 1)
-        
-        is_private = self.wc.cis.get_value(channel,'is_private')
-        auth_seq = cnxi.auth_seq(channel)
-        apply_to_packs = deep_get(auth_seq, 'apply_to_packs')
-        iscoro = asyncio.iscoroutinefunction(self.wc.sign)
-        
-        async def sign(_aInp):
-            if iscoro:
-                return await self.wc.sign(*_aInp)
-            else:
-                return self.wc.sign(*_aInp)
-        
-        
-        async def send_pack(i):
-            pck = packs[i]
-            msg_id = None
-            if isinstance(pck, tuple):
-                out, msg_id = pck
-            else:
-                out = pck
-            if id is not None:
-                try: msg_id = id[i] if not isinstance(id, (str,int)) else id
-                except IndexError: pass
-
-            if add_waiter and msg_id is None:
-                raise RuntimeError('{} - waiter requested but "message_id" was not ' \
-                                   'provided / returned by .encode(config)'.format(self.wc.name))
-            
-            async def do_auth(out):
-                seq = cnxi.auth_seq(channel, i)
-                auth_required = deep_get(seq,'is_required',return2=None)
-                takes_input = deep_get(seq,'takes_input',return2=True)
-                via_url = deep_get(seq,'via_url')
-                each_time = deep_get(seq,'each_time')
-                send_separately = deep_get(seq,'send_separately')
-                set_authenticated = deep_get(seq,'set_authenticated',return2=True)
-                
-                self.wc.log2('do_auth || i: {i} params: {params}, is_private: {is_private} auth_required: {auth_required} '\
-                             'via_url: {via_url} each_time: {each_time} send_separately: {send_separately} '\
-                             'takes_input: {takes_input} set_authenticated: {set_authenticated} cnxi.authenticated: {authenticated}'
-                             .format(i=i, params=params, is_private=is_private, auth_required=auth_required, via_url=via_url,
-                                     each_time=each_time, send_separately=send_separately, takes_input=takes_input,
-                                     set_authenticated=set_authenticated, authenticated=cnxi.authenticated))
-            
-                if (is_private and auth_required is None or auth_required) and not via_url:
-                    _aInp = [out] if takes_input else []
-                    if each_time:
-                        out = await sign(_aInp)
-                    elif not cnxi.authenticated:
-                        _aOut = await sign(_aInp)
-                        if not send_separately: 
-                            out = _aOut
-                        else:
-                            await cnx.send(_aOut)
-                        
-                        if set_authenticated:
-                            cnxi.authenticated = True
-                        
-                return out
-            
-            if apply_to_packs is None or i in apply_to_packs:
-                out = await do_auth(out)
-            
-            await cnx.send(out)
-            
-            waiter = self.add_waiter(msg_id) if add_waiter else None
-            if not add_waiter:
-                return None
-            elif return_waiter:
-                return waiter
-            else:
-                _wait = wait if wait != 'default' else \
-                        self.wc.cis.get_value(channel, 'waiter_timeout', set='cnx')
-                        
-                try: return await self.wait_on_waiter(waiter, _wait)
-                finally: self.remove_waiter(waiter)
-        
-        r = []
-        for i in range(len(packs)):
-            r.append(await send_pack(i))
-        
-        return r[0] if single else r
-    
-    
-    def forward_to_waiters(self, message_id, message, error=None, remove=True, copy=None):
-        try: waiters = self.waiters[message_id]
-        except KeyError: return
-        for i,waiter in enumerate(waiters):
-            if copy is True or isinstance(copy, int) and copy is not False and copy >= i:
-                if error is None:
-                    message = _copy.deepcopy(message)
-                else:
-                    error = _copy.deepcopy(error)
-            try:
-                if error is None:
-                    waiter.set_result(message)
-                else:
-                    waiter.set_exception(error)
-            except asyncio.InvalidStateError:
-                logger.error('{} - "{}"\'s waiter #{} result has already been set'.format(
-                    self.wc.name, message_id, i))
-        if remove:
-            del self.waiters[message_id]
-            
-            
-    def add_waiter(self, message_id):
-        waiter = asyncio.Future()
-        waiter.message_id = message_id
-        try: l = self.waiters[message_id]
-        except KeyError: 
-            l = self.waiters[message_id] = []
-        l.append(waiter)
-        return waiter
-    
-    def remove_waiter(self, waiter):
-        try: self.waiters[waiter.message_id].remove(waiter)
-        except (KeyError,ValueError): return None
-        else: return True
-        finally:
-            if not len(self.waiters.get(waiter.message_id,[None])):
-                del self.waiters[waiter.message_id]
-                      
-    def has_waiter(self, message_id):
-        return message_id in self.waiters and len(self.waiters[message_id])
-    
-    async def wait_on_waiter(self, waiter, timeout='default'):
-        if timeout == 'default':
-            timeout = self.wc.connection_defaults['waiter_timeout']
-        self.wc.log2('waiting on waiter {}, timeout: {}'.format(waiter.message_id, timeout))
-        try: r = await asyncio.wait_for(waiter, timeout)
-        except asyncio.TimeoutError as e:
-            self.wc.log2('timeout occurred on waiter {}'.format(waiter.message_id), 'ERROR')
-            raise e
-        self.wc.log2('{} wait finished'.format(waiter.message_id))
-        return r
-
-
-    def add_queue(self, channel, id=None, queue=None, maxsize=None, loop='out'):
-        loops = ([loop] if loop!='out' else self.loop) if loop is not None else asyncio.get_event_loop()
-        if maxsize is None:
-            maxsize = self.wc.queue_maxsizes.get(channel, 0)
-        # for cnx in self.wc.cm.connections.values():
-        #     cnx.add_queue(channel, id, queue, maxsize, loops)
-        return self.station.add_queue(channel, id, queue, maxsize, loops)
-    
-    def remove_queue(self, channel, queue_or_id, loop='out'):
-        id = queue_or_id if not isinstance(queue_or_id,asyncio.Event) else queue_or_id.id
-        loops = ([loop] if loop!='out' else self.loop) if loop is not None else asyncio.get_event_loop()
-        # for cnx in self.wc.cm.connections.values():
-        #     cnx.remove(channel, id, loops)
-        return self.station.remove(channel, id, loops)
-    
-    
-    def _is_in_thread_loop(self):
-        return asyncio.get_event_loop() is self._thread._loop
-    
-    async def stop(self):
-        if 'stop' in self.futures:
-            return await self.futures['stop']
-        
-        self.futures['stop'] = asyncio.Future()
-        
-        try:
-            self.wc.cm.remove_all()
-            
-            if 'start' in self.futures:
-                for attr in ('recv_queue','send_queue','_event_queue'):
-                    queue = getattr(self,attr)
-                    call_via_loop(force_put, (queue, _quit_command), loop=queue._loop)
-                
-                try: await self.futures['start']
-                except Exception: pass
-        
-        finally:
-            if sys.exc_info()[1] is None:
-                self.futures['stop'].set_result(None)
-            else:
-                self.futures['stop'].set_exception(sys.exc_info()[1])
-            del self.futures['stop']
-        
-
-class Request:
-    def __init__(self, params, wrapper, cnx=None):
-        """:type wrapper: WSClient
-           :type cnx: Connection"""
-        self.wc = wrapper
-        self.cnx = cnx
-        self.params = params.copy()
-        self.id_tuple = self.wc.cis.create_id_tuple(params)
-        self.channel = self.id_tuple[0]
-        self.merger = None
-        
-    def push(self):
-        return asyncio.ensure_future(self.wc.tp.send(self))
-    
-    def is_merged(self):
-        return self.merger is not None
-    
-    def is_merger(self):
-        return False
-    
-    def __eq__(self, other):
-        if not isinstance(other, Request):
-            return False
-        return other.id_tuple == self.id_tuple and other.cnx == self.cnx
-    
-    def __hash__(self):
-        return id(self)
-
-    
-def set_sockets_per_thread(value):
-    global sockets_per_thread
-    sockets_per_thread = value
+from fons.aio import call_via_loop, FonsEvent, FonsQueue
+from fons.debug import trylog, wrap_trylog
+from fons.dict_ops import deep_get
+from fons.errors import TerminatedException
+from fons.event import Station, force_put
+from fons.threads import EliThread
+import fons.log as _log
+
+import sys
+import asyncio
+import copy as _copy
+import functools
+from collections import defaultdict
+
+from .sub import Merged
+
+logger, logger2, tlogger, tloggers, tlogger0 = _log.get_standard_5(__name__)
+
+# Number of WSClient objects per thread. For infinite set to 0.
+sockets_per_thread = 1
+threads = set()
+_quit_command = object()
+
+
+class Transport:
+    def __init__(self, wrapper):
+        """:type wrapper: WSClient"""
+        self.wc = wrapper
+
+        # If param `_loop` was given in config, and a thread with such loop already exists,
+        # share that thread
+        _loop = getattr(self.wc, "_loop", None)
+        thread = next((x for x in threads if _loop == x._loop), None)
+
+        if thread is None:
+            try:
+                thread = min(threads, key=lambda x: x.socket_count)
+            except ValueError:
+                thread = None
+            if (
+                thread is not None
+                and sockets_per_thread > 0
+                and thread.socket_count >= sockets_per_thread
+            ):
+                thread = None
+
+        if thread is not None:
+            self._thread = thread
+        else:
+            if _loop is None:
+                _loop = asyncio.new_event_loop()
+            self._thread = EliThread(
+                target=_loop.run_forever,
+                loop=_loop,
+                daemon=True,
+                name="{}Thread".format(self.wc.name),
+            )
+            self._thread.socket_count = 0
+            threads.add(self._thread)
+
+        self.wc._loop = self._thread._loop
+
+        # "_" beginning of an attr signifies that _thread._loop is used
+        self._event_queue = FonsQueue(0, loop=self.wc._loop)
+        self.recv_queue = FonsQueue(0, loop=self.wc.loop)
+        self.send_queue = FonsQueue(
+            self.wc.queue_maxsizes.get("send", 0), loop=self.wc.loop
+        )
+        self._send_event = FonsEvent(loop=self.wc._loop)
+
+        self._event_queue.name = "{}[EQ]".format(self.wc.name)
+        self.recv_queue.name = "{}[RQ]".format(self.wc.name)
+        self.send_queue.name = "{}[SQ]".format(self.wc.name)
+
+        # These are the two main queues:
+        # event : receives ConnectionEvent from all (active) connections
+        #         can also receive Event when evoking self.wc.broadcast_event(..)
+        #         can be listened on using self.wc.listen()
+        # recv : receives websocket inputs (wrapped with Response) from all (active) connections
+        #        self.wc.handle receives from it
+        # For adding more queues, use self.wc.add_event_queue / self.wc.add_recv_queue
+        #
+        self.user_event_queue = ueq = FonsQueue(
+            self.wc.queue_maxsizes.get("event", 100), loop=self.wc.loop
+        )
+        ueq.name = "{}[UEQ]".format(self.wc.name)
+        ueq.warn = False
+
+        self.station = Station(
+            [
+                {
+                    "channel": "event",
+                    "id": 0,
+                    "queue": ueq,
+                    "event": False,
+                    "loops": [0],
+                },
+                {
+                    "channel": "recv",
+                    "id": 0,
+                    "queue": False,
+                    "event": None,
+                    "loops": [0],
+                },
+                {
+                    "channel": "empty",
+                    "id": 0,
+                    "queue": False,
+                    "event": None,
+                    "loops": [0],
+                },
+                {
+                    "channel": "running",
+                    "id": 0,
+                    "queue": False,
+                    "event": None,
+                    "loops": [0, -1],
+                },
+                {
+                    "channel": "stopped",
+                    "id": 0,
+                    "queue": False,
+                    "event": None,
+                    "loops": [0, -1],
+                },
+                {
+                    "channel": "active",
+                    "id": 0,
+                    "queue": False,
+                    "event": None,
+                    "loops": [0, -1],
+                },
+                {
+                    "channel": "inactive",
+                    "id": 0,
+                    "queue": False,
+                    "event": None,
+                    "loops": [0, -1],
+                },
+            ],
+            default_queue_size=100,
+            loops={0: self.wc.loop, -1: self.wc._loop},
+            name=self.wc.name + "[Station]",
+        )
+
+        self.station.broadcast("inactive")
+        self.station.broadcast("stopped")
+        self.waiters = {}
+        self.futures = {}
+
+    async def start(self):
+        if "stop" in self.futures:
+            try:
+                await self.futures["stop"]
+            except Exception:
+                pass
+
+        if "start" in self.futures:
+            return await self.futures["start"]
+
+        self.futures["start"] = asyncio.Future()
+        f1 = f2 = None
+        try:
+            self.wc.log("starting")
+            self.station.broadcast("running")
+            self.station.broadcast("stopped", op="clear")
+
+            (await self.wc.on_start()) if asyncio.iscoroutinefunction(
+                self.wc.on_start
+            ) else self.wc.on_start()
+
+            _loop = self._thread._loop
+            f1 = call_via_loop(wrap_trylog(self._main), loop=_loop, module="asyncio")
+            f2 = call_via_loop(self.process_events, loop=_loop, module="asyncio")
+
+            if not self._thread.is_alive():
+                self._thread.start()
+
+            await self.process_responses()
+
+            await asyncio.wait([f1, f2])
+
+        finally:
+            if f1 is not None:
+                f1.cancel()
+            if f2 is not None:
+                f2.cancel()
+            if sys.exc_info()[1] is None:
+                self.futures["start"].set_result(None)
+            else:
+                self.futures["start"].set_exception(sys.exc_info()[1])
+            del self.futures["start"]
+            self.station.broadcast("running", op="clear")
+            self.station.broadcast("stopped")
+
+    async def _main(self):
+        # This runs in self._thread
+        loop = self.wc.loop
+        _loop = asyncio.get_event_loop()
+
+        # .send() is rooted via .send_queue
+        async def _send(future, params, wait, id, cnx, sub):
+            """:type future: asyncio.Future"""
+            try:
+                r = await self.send(params, wait, id, cnx, sub)
+            except Exception as e:
+                self.wc.log(
+                    "thread .send() error occurred: {}".format(repr(e)), "ERROR"
+                )
+                self.wc.log(e)
+                loop.call_soon_threadsafe(functools.partial(future.set_exception, e))
+            else:
+                loop.call_soon_threadsafe(functools.partial(future.set_result, r))
+
+        # receives updates from the queue, sends them.
+        async def _fire_from_send_queue():
+            while not self.wc._closed:
+                # get from queue via the main loop
+                fut = call_via_loop(
+                    self.send_queue.get,
+                    module="asyncio",
+                    loop=loop,
+                )
+                item = await fut
+                if item is _quit_command:
+                    break
+                future, params, wait, id, cnx, sub = item
+                asyncio.ensure_future(_send(future, params, wait, id, cnx, sub))
+
+        # Start firing right now (allow user initiated sending) before pushing
+        # the subs, as the .wc.handle method (which runs outside of the ._thread)
+        # might need to respond to some of the messages received during the pushing
+        fire = asyncio.ensure_future(_fire_from_send_queue())
+
+        self.station.broadcast("active")
+        self.station.broadcast("inactive", op="clear")
+        self.wc.broadcast_event("active", 1)
+
+        try:
+            await call_via_loop(
+                self.wc.wait_till_active, (5,), loop=self.wc.loop, module="asyncio"
+            )
+            await self.wc.wait_till_active(1)
+            # Connections will be started when subscriptions are being pushed
+            # (in .send method). Note that since this here is running in ._thread,
+            # the subscription out messages are NOT sent via the queue.
+            await self.wc.sh.push_subscriptions()
+            await fire
+        finally:
+            fire.cancel()
+            self.station.broadcast("active", op="clear")
+            self.station.broadcast("inactive")
+            self.wc.broadcast_event("active", 0)
+            self.wc.log("stopped")
+
+    async def process_responses(self):
+        # Process received results from connections. This runs in the main loop (self.loop)
+        self.wc.log2("starting response processing")
+        iscoro = asyncio.iscoroutinefunction(self.wc.handle)
+        recv = None
+
+        while not self.wc._closed:
+            poll_interval = self.wc.connection_defaults["poll_interval"]
+            if recv is None:
+                recv = asyncio.ensure_future(self.recv_queue.get())
+
+            done, pending = await asyncio.wait([recv], timeout=poll_interval)
+            if not recv.done():
+                self.station.broadcast("empty")
+                self.wc.broadcast_event("socket", "empty")
+                continue
+
+            R = recv.result()
+            recv = None
+            if R is _quit_command:
+                break
+
+            try:
+                if iscoro:
+                    await self.wc.handle(R)
+                else:
+                    self.wc.handle(R)
+            except Exception as e:
+                str_r = str(R.data)
+                dots = "..." if len(str_r) > 200 else ""
+                logger2.error(
+                    "{} - {} while handling response: {}{}".format(
+                        self.wc.name, e.__class__.__name__, str_r[:200], dots
+                    )
+                )
+                logger.error(str_r)
+                logger.exception(e)
+            else:
+                message_id = self.wc.extract_message_id(R)
+                if message_id is not None:
+                    errors = self.wc.extract_errors(R)
+                    error = (
+                        errors
+                        if isinstance(errors, Exception)
+                        else (errors[0] if len(errors) else None)
+                    )
+                    ftw = functools.partial(
+                        self.forward_to_waiters,
+                        message_id,
+                        R,
+                        error=error,
+                        remove=True,
+                        copy=1,
+                    )
+                    self.wc._loop.call_soon_threadsafe(functools.partial(trylog, ftw))
+                self.station.broadcast("recv")
+
+        if recv is not None:
+            recv.cancel()
+
+    async def process_events(self):
+        # Process events from connections. This runs in self._thread
+        self.wc.log2("starting event processing")
+        activation_count = defaultdict(int)
+
+        while not self.wc._closed:
+            e = await self._event_queue.get()
+            if e is _quit_command:
+                break
+
+            try:
+                cnx = self.wc.cm.connections[e.id]
+            except KeyError:
+                continue
+
+            if e.type == "socket" and e.data == 0:
+                for s in self.wc.sh.subscriptions:
+                    if s.cnx is cnx:
+                        self.wc.sh.change_subscription_state(s, 0)
+                try:
+                    self.wc.cm.cnx_infs[cnx].authenticated = False
+                except KeyError:
+                    pass
+
+            elif e.type == "socket" and e.data == 1:
+                # Do not push on first notification,
+                # as during that time *all* subscriptions are being pushed anyway
+                pushed = None
+                if activation_count[cnx]:
+                    pushed = await self.wc.sh.push_subscriptions(cnx)
+
+                for s in self.wc.sh.subscriptions:
+                    if s.cnx is cnx:
+                        v = self.wc.cis.get_value(s.channel, "auto_activate")
+                        if v == "on_cnx_activation" and (pushed is None or s in pushed):
+                            self.wc.sh.change_subscription_state(s, 1)
+
+                activation_count[cnx] += 1
+
+            elif e.type == "running" and e.data == 0:
+                activation_count[cnx] = 0
+
+    async def send(self, params, wait=False, id=None, cnx=None, sub=None):
+        """
+        :type params: dict, Request, Subscription
+        :type cnx: Connection
+        :param params:
+          must contain '_' key; also accepts Subscription object
+        :param wait:
+          False : don't wait
+          'default', True->'default', None, of type int/float: timeout to wait
+          'return': doesn't wait, but returns the waiter
+          if signalr/socketio is enabled then id system is probably not implementable (leave wait to False).
+        :param id:
+          custom id to be attached to the waiter. in that case user must forward the response to
+          the waiter manually (e.g. through .handle)
+          if channel sends multiple messages, id may be given as [id0, id1, ..]
+        :param cnx:
+          may be specified if params is dict, otherwise cnx of given request will be used
+        :param sub:
+          if subscription, True for subbing, False for unsubbing
+        """
+        if isinstance(params, dict):
+            params = params.copy()
+            output = self.wc.transform(params)
+            if output is not None:
+                params = output
+
+        if isinstance(params, dict) and cnx is None:
+            cnx = self.wc.sh.find_available_connection(params, create=True)
+
+        rq = (
+            Request(params, self.wc, cnx) if not isinstance(params, Request) else params
+        )
+
+        # Forward to thread
+        if not self._is_in_thread_loop():
+            fut = asyncio.Future()
+            await self.send_queue.put((fut, rq, wait, id, cnx, sub))
+            return await fut
+
+        params = rq.params
+        cnx = rq.cnx
+        channel = rq.channel
+        cnxi = self.wc.cm.cnx_infs[cnx]
+        send = self.wc.cis.get_value(channel, "send")
+        drop = self.wc.cis.get_value(channel, "drop_unused_connection", not send)
+
+        if not cnx.is_running() and (sub is None or sub):
+            try:
+                cnx.start()
+            except RuntimeError:
+                pass
+            await cnx.wait_till_active(cnx.connect_timeout)
+        elif (sub is not None and not sub) and cnx.url and drop:
+            # Due to param variance difference old connections would not satisfy
+            # the new variance, and would remain unused
+            # if rq.is_merger() and not any(_s.merger is not rq and _s.cnx is cnx
+            #                               for _s in self.wc.sh.subscriptions):
+            if not any(cnx is _s.cnx for _s in self.wc.sh.subscriptions):
+                self.wc.cm.remove_connection(cnx, True)
+            if cnx.is_running():
+                await cnx.stop()
+
+        wait = "default" if wait is True else wait
+        add_waiter = wait is not False
+        return_waiter = wait in (
+            "return",
+            "return-waiter",
+            "return_waiter",
+            "return waiter",
+        )
+
+        def _return():
+            if not add_waiter or not return_waiter:
+                return None
+            else:
+                f = asyncio.Future()
+                f.set_result(None)
+                return f
+
+        if not cnx.url or not send:
+            return _return()
+
+        packs = self.wc.encode(rq, sub)
+        # WSClient.encode should return `None` if this specific request is not meant to be sent
+        if packs is None:
+            return _return()
+
+        if not isinstance(packs, Merged):
+            packs = [packs]
+        single = len(packs) == 1
+
+        is_private = self.wc.cis.get_value(channel, "is_private")
+        auth_seq = cnxi.auth_seq(channel)
+        apply_to_packs = deep_get(auth_seq, "apply_to_packs")
+        iscoro = asyncio.iscoroutinefunction(self.wc.sign)
+
+        async def sign(_aInp):
+            if iscoro:
+                return await self.wc.sign(*_aInp)
+            else:
+                return self.wc.sign(*_aInp)
+
+        async def send_pack(i):
+            pck = packs[i]
+            msg_id = None
+            if isinstance(pck, tuple):
+                out, msg_id = pck
+            else:
+                out = pck
+            if id is not None:
+                try:
+                    msg_id = id[i] if not isinstance(id, (str, int)) else id
+                except IndexError:
+                    pass
+
+            if add_waiter and msg_id is None:
+                raise RuntimeError(
+                    '{} - waiter requested but "message_id" was not '
+                    "provided / returned by .encode(config)".format(self.wc.name)
+                )
+
+            async def do_auth(out):
+                seq = cnxi.auth_seq(channel, i)
+                auth_required = deep_get(seq, "is_required", return2=None)
+                takes_input = deep_get(seq, "takes_input", return2=True)
+                via_url = deep_get(seq, "via_url")
+                each_time = deep_get(seq, "each_time")
+                send_separately = deep_get(seq, "send_separately")
+                set_authenticated = deep_get(seq, "set_authenticated", return2=True)
+
+                self.wc.log2(
+                    "do_auth || i: {i} params: {params}, is_private: {is_private} auth_required: {auth_required} "
+                    "via_url: {via_url} each_time: {each_time} send_separately: {send_separately} "
+                    "takes_input: {takes_input} set_authenticated: {set_authenticated} cnxi.authenticated: {authenticated}".format(
+                        i=i,
+                        params=params,
+                        is_private=is_private,
+                        auth_required=auth_required,
+                        via_url=via_url,
+                        each_time=each_time,
+                        send_separately=send_separately,
+                        takes_input=takes_input,
+                        set_authenticated=set_authenticated,
+                        authenticated=cnxi.authenticated,
+                    )
+                )
+
+                if (
+                    is_private and auth_required is None or auth_required
+                ) and not via_url:
+                    _aInp = [out] if takes_input else []
+                    if each_time:
+                        out = await sign(_aInp)
+                    elif not cnxi.authenticated:
+                        _aOut = await sign(_aInp)
+                        if not send_separately:
+                            out = _aOut
+                        else:
+                            await cnx.send(_aOut)
+
+                        if set_authenticated:
+                            cnxi.authenticated = True
+
+                return out
+
+            if apply_to_packs is None or i in apply_to_packs:
+                out = await do_auth(out)
+
+            await cnx.send(out)
+
+            waiter = self.add_waiter(msg_id) if add_waiter else None
+            if not add_waiter:
+                return None
+            elif return_waiter:
+                return waiter
+            else:
+                _wait = (
+                    wait
+                    if wait != "default"
+                    else self.wc.cis.get_value(channel, "waiter_timeout", set="cnx")
+                )
+
+                try:
+                    return await self.wait_on_waiter(waiter, _wait)
+                finally:
+                    self.remove_waiter(waiter)
+
+        r = []
+        for i in range(len(packs)):
+            r.append(await send_pack(i))
+
+        return r[0] if single else r
+
+    def forward_to_waiters(
+        self, message_id, message, error=None, remove=True, copy=None
+    ):
+        try:
+            waiters = self.waiters[message_id]
+        except KeyError:
+            return
+        for i, waiter in enumerate(waiters):
+            if (
+                copy is True
+                or isinstance(copy, int)
+                and copy is not False
+                and copy >= i
+            ):
+                if error is None:
+                    message = _copy.deepcopy(message)
+                else:
+                    error = _copy.deepcopy(error)
+            try:
+                if error is None:
+                    waiter.set_result(message)
+                else:
+                    waiter.set_exception(error)
+            except asyncio.InvalidStateError:
+                logger.error(
+                    '{} - "{}"\'s waiter #{} result has already been set'.format(
+                        self.wc.name, message_id, i
+                    )
+                )
+        if remove:
+            del self.waiters[message_id]
+
+    def add_waiter(self, message_id):
+        waiter = asyncio.Future()
+        waiter.message_id = message_id
+        try:
+            l = self.waiters[message_id]
+        except KeyError:
+            l = self.waiters[message_id] = []
+        l.append(waiter)
+        return waiter
+
+    def remove_waiter(self, waiter):
+        try:
+            self.waiters[waiter.message_id].remove(waiter)
+        except (KeyError, ValueError):
+            return None
+        else:
+            return True
+        finally:
+            if not len(self.waiters.get(waiter.message_id, [None])):
+                del self.waiters[waiter.message_id]
+
+    def has_waiter(self, message_id):
+        return message_id in self.waiters and len(self.waiters[message_id])
+
+    async def wait_on_waiter(self, waiter, timeout="default"):
+        if timeout == "default":
+            timeout = self.wc.connection_defaults["waiter_timeout"]
+        self.wc.log2(
+            "waiting on waiter {}, timeout: {}".format(waiter.message_id, timeout)
+        )
+        try:
+            r = await asyncio.wait_for(waiter, timeout)
+        except asyncio.TimeoutError as e:
+            self.wc.log2(
+                "timeout occurred on waiter {}".format(waiter.message_id), "ERROR"
+            )
+            raise e
+        self.wc.log2("{} wait finished".format(waiter.message_id))
+        return r
+
+    def add_queue(self, channel, id=None, queue=None, maxsize=None, loop="out"):
+        loops = (
+            ([loop] if loop != "out" else self.loop)
+            if loop is not None
+            else asyncio.get_event_loop()
+        )
+        if maxsize is None:
+            maxsize = self.wc.queue_maxsizes.get(channel, 0)
+        # for cnx in self.wc.cm.connections.values():
+        #     cnx.add_queue(channel, id, queue, maxsize, loops)
+        return self.station.add_queue(channel, id, queue, maxsize, loops)
+
+    def remove_queue(self, channel, queue_or_id, loop="out"):
+        id = (
+            queue_or_id
+            if not isinstance(queue_or_id, asyncio.Event)
+            else queue_or_id.id
+        )
+        loops = (
+            ([loop] if loop != "out" else self.loop)
+            if loop is not None
+            else asyncio.get_event_loop()
+        )
+        # for cnx in self.wc.cm.connections.values():
+        #     cnx.remove(channel, id, loops)
+        return self.station.remove(channel, id, loops)
+
+    def _is_in_thread_loop(self):
+        return asyncio.get_event_loop() is self._thread._loop
+
+    async def stop(self):
+        if "stop" in self.futures:
+            return await self.futures["stop"]
+
+        self.futures["stop"] = asyncio.Future()
+
+        try:
+            self.wc.cm.remove_all()
+
+            if "start" in self.futures:
+                for attr in ("recv_queue", "send_queue", "_event_queue"):
+                    queue = getattr(self, attr)
+                    call_via_loop(force_put, (queue, _quit_command), loop=queue._loop)
+
+                try:
+                    await self.futures["start"]
+                except Exception:
+                    pass
+
+        finally:
+            if sys.exc_info()[1] is None:
+                self.futures["stop"].set_result(None)
+            else:
+                self.futures["stop"].set_exception(sys.exc_info()[1])
+            del self.futures["stop"]
+
+
+class Request:
+    def __init__(self, params, wrapper, cnx=None):
+        """:type wrapper: WSClient
+        :type cnx: Connection"""
+        self.wc = wrapper
+        self.cnx = cnx
+        self.params = params.copy()
+        self.id_tuple = self.wc.cis.create_id_tuple(params)
+        self.channel = self.id_tuple[0]
+        self.merger = None
+
+    def push(self):
+        return asyncio.ensure_future(self.wc.tp.send(self))
+
+    def is_merged(self):
+        return self.merger is not None
+
+    def is_merger(self):
+        return False
+
+    def __eq__(self, other):
+        if not isinstance(other, Request):
+            return False
+        return other.id_tuple == self.id_tuple and other.cnx == self.cnx
+
+    def __hash__(self):
+        return id(self)
+
+
+def set_sockets_per_thread(value):
+    global sockets_per_thread
+    sockets_per_thread = value
```

### Comparing `wsclient-0.3.0/wsclient/url.py` & `wsclient-0.4.0/wsclient/url.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,157 +1,162 @@
-from fons.func import get_arg_count
-import asyncio
-
-
-class URLFactory:
-    def __init__(self, wrapper, url_notation, params=None):
-        """:type wrapper: WSClient
-           :type url_notation: str"""
-        self.wc = wrapper
-        self.notation = url_notation
-        self.params = params
-        
-        self.parts = self.split(url_notation)
-        decoded = [self.decode_part(x) for x in self.parts]
-        self.types = [x[0] for x in decoded]
-        self.names = [x[1] for x in decoded]
-        
-        
-    async def create_url(self, params):
-        """
-        :returns: a dict with `url` and `extra_headers`
-        """
-        if params is None:
-            params = self.params
-        
-        str_parts = []
-        headers = {}
-        
-        for name,type in zip(self.names,self.types):
-            # Each resolved can be either
-            #  - <str> (appended to the url)
-            #  - <dict> (extended to headers)
-            #  - None (ignored)
-            # or a list of those
-            if type == 'plain':
-                resolved = name
-            elif type == 'attribute':
-                resolved = getattr(self.wc, name)
-            elif type in ('variable',):
-                resolved = params[name]
-            elif type == 'component':
-                cmp = self.wc.url_components[name]
-                if hasattr(cmp,'__call__'):
-                    args = [self] if get_arg_count(cmp) else []
-                    cmp = (await cmp(*args)) if asyncio.iscoroutinefunction(cmp) else cmp(*args)
-                resolved = cmp
-            elif type in ('method', 'method:shared'):
-                method = getattr(self.wc, name)
-                args = [self] if get_arg_count(method) else []
-                resolved = (await method(*args)) if asyncio.iscoroutinefunction(method) else method(*args)
-            else:
-                raise ValueError(type)
-            
-            if isinstance(resolved, (str, dict)) or resolved is None:
-                resolved = [resolved]
-            
-            for x in resolved:
-                if x is None:
-                    continue
-                elif isinstance(x, dict):
-                    headers.update(x)
-                else:
-                    str_parts.append(x)
-        
-        url = ''.join(str_parts)
-        
-        config = {
-            'url': url,
-        }
-        if headers:
-            config['extra_headers'] = headers
-        
-        return config
-    
-    @staticmethod
-    def split(url):
-        parts = []
-        while url:
-            i = url.find('<')
-            j = url[i:].find('>')
-            if i == -1 or j == -1:
-                parts.append(url)
-                break
-            j += i
-            preceding = url[:i]
-            if preceding:
-                parts.append(preceding)
-            var = url[i:j+1]
-            if j-i > 1:
-                parts.append(var)
-            url = url[j+1:]
-        return parts
-    
-    @staticmethod
-    def decode_part(x):
-        if not x.startswith('<'):
-            return 'plain', x
-        
-        x = x[1:-1]
-        
-        if x[:1] == '$' or x[:2] == 'c$':
-            return 'component', x[x.find('$')+1:]
-        
-        elif x[:2] == 'a$':
-            return 'attribute', x[2:]
-        
-        elif x[:2] != 'm$':
-            return 'variable', x
-        
-        shared = ':shared' if x.endswith(':shared') else ''
-        if shared:
-            x = x[:-len(':shared')]
-        
-        if x[:2] == 'm$':
-            return 'method{}'.format(shared), x[2:]
-        #else:
-        #    return 'variable{}'.format(shared), x
-        
-        
-    def copy(self, params=None):
-        if params is None:
-            params = self.params
-        return self.__class__(self.wc, self.notation, params)
-    
-    
-    def __eq__(self, other):
-        if not isinstance(other, URLFactory):
-            raise TypeError(type(other))
-        
-        if self.names != other.names or self.types != other.types:
-            return False
-        
-        if None not in (self.params, other.params) and self.params==other.params:
-            return True
-        
-        for obj in (self,other):
-            for name,type in zip(obj.names, obj.types):
-                if type=='method':
-                    return False
-                elif type=='variable':
-                    v1 = self.params.get(name)
-                    v2 = other.params.get(name)
-                    if None in (v1, v2) or v1 != v2:
-                        return False
-                elif type == 'component' and not isinstance(self.wc.url_components[name], str):
-                    return False
-                
-        return True
-    
-    
-    def __call__(self):
-        #Note that it returns coroutine
-        return self.create_url(self.params)
-    
-    
-    def __bool__(self):
-        return bool(self.notation)
+from fons.func import get_arg_count
+import asyncio
+
+
+class URLFactory:
+    def __init__(self, wrapper, url_notation, params=None):
+        """:type wrapper: WSClient
+        :type url_notation: str"""
+        self.wc = wrapper
+        self.notation = url_notation
+        self.params = params
+
+        self.parts = self.split(url_notation)
+        decoded = [self.decode_part(x) for x in self.parts]
+        self.types = [x[0] for x in decoded]
+        self.names = [x[1] for x in decoded]
+
+    async def create_url(self, params):
+        """
+        :returns: a dict with `url` and `extra_headers`
+        """
+        if params is None:
+            params = self.params
+
+        str_parts = []
+        headers = {}
+
+        for name, type in zip(self.names, self.types):
+            # Each resolved can be either
+            #  - <str> (appended to the url)
+            #  - <dict> (extended to headers)
+            #  - None (ignored)
+            # or a list of those
+            if type == "plain":
+                resolved = name
+            elif type == "attribute":
+                resolved = getattr(self.wc, name)
+            elif type in ("variable",):
+                resolved = params[name]
+            elif type == "component":
+                cmp = self.wc.url_components[name]
+                if hasattr(cmp, "__call__"):
+                    args = [self] if get_arg_count(cmp) else []
+                    cmp = (
+                        (await cmp(*args))
+                        if asyncio.iscoroutinefunction(cmp)
+                        else cmp(*args)
+                    )
+                resolved = cmp
+            elif type in ("method", "method:shared"):
+                method = getattr(self.wc, name)
+                args = [self] if get_arg_count(method) else []
+                resolved = (
+                    (await method(*args))
+                    if asyncio.iscoroutinefunction(method)
+                    else method(*args)
+                )
+            else:
+                raise ValueError(type)
+
+            if isinstance(resolved, (str, dict)) or resolved is None:
+                resolved = [resolved]
+
+            for x in resolved:
+                if x is None:
+                    continue
+                elif isinstance(x, dict):
+                    headers.update(x)
+                else:
+                    str_parts.append(x)
+
+        url = "".join(str_parts)
+
+        config = {
+            "url": url,
+        }
+        if headers:
+            config["extra_headers"] = headers
+
+        return config
+
+    @staticmethod
+    def split(url):
+        parts = []
+        while url:
+            i = url.find("<")
+            j = url[i:].find(">")
+            if i == -1 or j == -1:
+                parts.append(url)
+                break
+            j += i
+            preceding = url[:i]
+            if preceding:
+                parts.append(preceding)
+            var = url[i : j + 1]
+            if j - i > 1:
+                parts.append(var)
+            url = url[j + 1 :]
+        return parts
+
+    @staticmethod
+    def decode_part(x):
+        if not x.startswith("<"):
+            return "plain", x
+
+        x = x[1:-1]
+
+        if x[:1] == "$" or x[:2] == "c$":
+            return "component", x[x.find("$") + 1 :]
+
+        elif x[:2] == "a$":
+            return "attribute", x[2:]
+
+        elif x[:2] != "m$":
+            return "variable", x
+
+        shared = ":shared" if x.endswith(":shared") else ""
+        if shared:
+            x = x[: -len(":shared")]
+
+        if x[:2] == "m$":
+            return "method{}".format(shared), x[2:]
+        # else:
+        #    return 'variable{}'.format(shared), x
+
+    def copy(self, params=None):
+        if params is None:
+            params = self.params
+        return self.__class__(self.wc, self.notation, params)
+
+    def __eq__(self, other):
+        if not isinstance(other, URLFactory):
+            raise TypeError(type(other))
+
+        if self.names != other.names or self.types != other.types:
+            return False
+
+        if None not in (self.params, other.params) and self.params == other.params:
+            return True
+
+        for obj in (self, other):
+            for name, type in zip(obj.names, obj.types):
+                if type == "method":
+                    return False
+                elif type == "variable":
+                    v1 = self.params.get(name)
+                    v2 = other.params.get(name)
+                    if None in (v1, v2) or v1 != v2:
+                        return False
+                elif type == "component" and not isinstance(
+                    self.wc.url_components[name], str
+                ):
+                    return False
+
+        return True
+
+    def __call__(self):
+        # Note that it returns coroutine
+        return self.create_url(self.params)
+
+    def __bool__(self):
+        return bool(self.notation)
```

### Comparing `wsclient-0.3.0/wsclient.egg-info/SOURCES.txt` & `wsclient-0.4.0/wsclient.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+MANIFEST.in
 README.md
+requirements.txt
 setup.py
 signalr_aio_wsclient/__init__.py
 signalr_aio_wsclient/_connection.py
 signalr_aio_wsclient/events/__init__.py
 signalr_aio_wsclient/events/_events.py
 signalr_aio_wsclient/hubs/__init__.py
 signalr_aio_wsclient/hubs/_hub.py
```

