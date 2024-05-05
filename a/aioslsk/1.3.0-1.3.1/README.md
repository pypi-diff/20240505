# Comparing `tmp/aioslsk-1.3.0.tar.gz` & `tmp/aioslsk-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioslsk-1.3.0.tar", max compression
+gzip compressed data, was "aioslsk-1.3.1.tar", max compression
```

## Comparing `aioslsk-1.3.0.tar` & `aioslsk-1.3.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0    35149 2024-04-28 10:31:59.363566 aioslsk-1.3.0/LICENSE
--rw-r--r--   0        0        0     3072 2024-04-28 10:31:59.363566 aioslsk-1.3.0/README.rst
--rw-r--r--   0        0        0     1748 2024-04-28 10:32:13.723706 aioslsk-1.3.0/pyproject.toml
--rw-r--r--   0        0        0       23 2024-04-28 10:32:13.723706 aioslsk-1.3.0/src/aioslsk/__init__.py
--rw-r--r--   0        0        0      872 2024-04-28 10:31:59.363566 aioslsk-1.3.0/src/aioslsk/base_manager.py
--rw-r--r--   0        0        0    13256 2024-04-28 10:31:59.363566 aioslsk-1.3.0/src/aioslsk/client.py
--rw-r--r--   0        0        0    30171 2024-04-28 10:31:59.363566 aioslsk-1.3.0/src/aioslsk/commands.py
--rw-r--r--   0        0        0     1161 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/constants.py
--rw-r--r--   0        0        0    24275 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/distributed.py
--rw-r--r--   0        0        0    14010 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/events.py
--rw-r--r--   0        0        0     2043 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/interest/__init__.py
--rw-r--r--   0        0        0     5333 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/interest/manager.py
--rw-r--r--   0        0        0     3980 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/naming.py
--rw-r--r--   0        0        0        0 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/network/__init__.py
--rw-r--r--   0        0        0    26908 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/network/connection.py
--rw-r--r--   0        0        0    45116 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/network/network.py
--rw-r--r--   0        0        0     2862 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/network/rate_limiter.py
--rw-r--r--   0        0        0     7299 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/network/upnp.py
--rw-r--r--   0        0        0     5627 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/peer.py
--rw-r--r--   0        0        0        0 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/protocol/__init__.py
--rw-r--r--   0        0        0    48230 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/protocol/messages.py
--rw-r--r--   0        0        0     2541 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/protocol/obfuscation.py
--rw-r--r--   0        0        0    17136 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/protocol/primitives.py
--rw-r--r--   0        0        0    17971 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/room/manager.py
--rw-r--r--   0        0        0     1103 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/room/model.py
--rw-r--r--   0        0        0        0 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/search/__init__.py
--rw-r--r--   0        0        0    14624 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/search/manager.py
--rw-r--r--   0        0        0     3012 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/search/model.py
--rw-r--r--   0        0        0     2126 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/server.py
--rw-r--r--   0        0        0      484 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/session.py
--rw-r--r--   0        0        0     4562 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/settings.py
--rw-r--r--   0        0        0        0 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/shares/__init__.py
--rw-r--r--   0        0        0     1428 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/shares/cache.py
--rw-r--r--   0        0        0    30182 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/shares/manager.py
--rw-r--r--   0        0        0     4284 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/shares/model.py
--rw-r--r--   0        0        0     2754 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/shares/utils.py
--rw-r--r--   0        0        0        0 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/transfer/__init__.py
--rw-r--r--   0        0        0     2342 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/transfer/cache.py
--rw-r--r--   0        0        0      338 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/transfer/interface.py
--rw-r--r--   0        0        0    53703 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/transfer/manager.py
--rw-r--r--   0        0        0    12071 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/transfer/model.py
--rw-r--r--   0        0        0    13411 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/transfer/state.py
--rw-r--r--   0        0        0        0 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/user/__init__.py
--rw-r--r--   0        0        0    14601 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/user/manager.py
--rw-r--r--   0        0        0     3440 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/user/model.py
--rw-r--r--   0        0        0     1945 2024-04-28 10:31:59.367566 aioslsk-1.3.0/src/aioslsk/utils.py
--rw-r--r--   0        0        0     4547 1970-01-01 00:00:00.000000 aioslsk-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-05 17:14:27.161138 aioslsk-1.3.1/LICENSE
+-rw-r--r--   0        0        0     3072 2024-05-05 17:14:27.161138 aioslsk-1.3.1/README.rst
+-rw-r--r--   0        0        0     1748 2024-05-05 17:14:37.305100 aioslsk-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0       23 2024-05-05 17:14:37.301100 aioslsk-1.3.1/src/aioslsk/__init__.py
+-rw-r--r--   0        0        0      872 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/base_manager.py
+-rw-r--r--   0        0        0    13509 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/client.py
+-rw-r--r--   0        0        0    30171 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/commands.py
+-rw-r--r--   0        0        0     1161 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/constants.py
+-rw-r--r--   0        0        0    24275 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/distributed.py
+-rw-r--r--   0        0        0    14010 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/events.py
+-rw-r--r--   0        0        0     2043 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/interest/__init__.py
+-rw-r--r--   0        0        0     5333 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/interest/manager.py
+-rw-r--r--   0        0        0     3980 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/naming.py
+-rw-r--r--   0        0        0        0 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/network/__init__.py
+-rw-r--r--   0        0        0    26908 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/network/connection.py
+-rw-r--r--   0        0        0    45116 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/network/network.py
+-rw-r--r--   0        0        0     2862 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/network/rate_limiter.py
+-rw-r--r--   0        0        0     7299 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/network/upnp.py
+-rw-r--r--   0        0        0     5627 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/peer.py
+-rw-r--r--   0        0        0        0 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/protocol/__init__.py
+-rw-r--r--   0        0        0    48230 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/protocol/messages.py
+-rw-r--r--   0        0        0     2541 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/protocol/obfuscation.py
+-rw-r--r--   0        0        0    17136 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/protocol/primitives.py
+-rw-r--r--   0        0        0    17971 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/room/manager.py
+-rw-r--r--   0        0        0     1103 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/room/model.py
+-rw-r--r--   0        0        0        0 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/search/__init__.py
+-rw-r--r--   0        0        0    14624 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/search/manager.py
+-rw-r--r--   0        0        0     3012 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/search/model.py
+-rw-r--r--   0        0        0     2126 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/server.py
+-rw-r--r--   0        0        0      484 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/session.py
+-rw-r--r--   0        0        0     4562 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/settings.py
+-rw-r--r--   0        0        0        0 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/shares/__init__.py
+-rw-r--r--   0        0        0     1561 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/shares/cache.py
+-rw-r--r--   0        0        0    35269 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/shares/manager.py
+-rw-r--r--   0        0        0     4284 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/shares/model.py
+-rw-r--r--   0        0        0     2754 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/shares/utils.py
+-rw-r--r--   0        0        0        0 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/transfer/__init__.py
+-rw-r--r--   0        0        0     2342 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/transfer/cache.py
+-rw-r--r--   0        0        0      338 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/transfer/interface.py
+-rw-r--r--   0        0        0    53704 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/transfer/manager.py
+-rw-r--r--   0        0        0    12071 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/transfer/model.py
+-rw-r--r--   0        0        0    13411 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/transfer/state.py
+-rw-r--r--   0        0        0        0 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/user/__init__.py
+-rw-r--r--   0        0        0    14609 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/user/manager.py
+-rw-r--r--   0        0        0     3440 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/user/model.py
+-rw-r--r--   0        0        0     1945 2024-05-05 17:14:27.165138 aioslsk-1.3.1/src/aioslsk/utils.py
+-rw-r--r--   0        0        0     4547 1970-01-01 00:00:00.000000 aioslsk-1.3.1/PKG-INFO
```

### Comparing `aioslsk-1.3.0/LICENSE` & `aioslsk-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aioslsk-1.3.0/README.rst` & `aioslsk-1.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `aioslsk-1.3.0/pyproject.toml` & `aioslsk-1.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aioslsk"
-version = "v1.3.0"
+version = "v1.3.1"
 description = "Asyncio based SoulSeek client"
 authors = ["JurgenR <1249228+JurgenR@users.noreply.github.com>"]
 repository = "https://github.com/JurgenR/aioslsk/"
 documentation = "https://readthedocs.org/projects/aioslsk/"
 readme = "README.rst"
 license = "GPL-3.0-or-later"
 packages = [{include = "aioslsk", from = "src"}]
```

### Comparing `aioslsk-1.3.0/src/aioslsk/base_manager.py` & `aioslsk-1.3.1/src/aioslsk/base_manager.py`

 * *Files identical despite different names*

### Comparing `aioslsk-1.3.0/src/aioslsk/client.py` & `aioslsk-1.3.1/src/aioslsk/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     ServerReconnectedEvent,
     SessionDestroyedEvent,
     SessionInitializedEvent,
 )
 from .exceptions import AioSlskException, AuthenticationError, InvalidSessionError
 from .interest.manager import InterestManager
 from .shares.cache import SharesCache, SharesNullCache
-from .shares.manager import SharesManager
+from .shares.manager import ExecutorFactory, SharesManager
 from .network.connection import ConnectionState, ServerConnection
 from .network.network import Network
 from .peer import PeerManager
 from .protocol.messages import Login
 from .protocol.primitives import calc_md5
 from .room.manager import RoomManager
 from .search.manager import SearchManager
@@ -49,14 +49,15 @@
     different :class:`aioslsk.base_manager.BaseManager` classes and orchestrates
     the lifecycle of those classes
     """
 
     def __init__(
             self, settings: Settings,
             shares_cache: Optional[SharesCache] = None, transfer_cache: Optional[TransferCache] = None,
+            executor_factory: Optional[ExecutorFactory] = None,
             event_bus: Optional[EventBus] = None):
         self.settings: Settings = settings
 
         self._stop_event: Optional[asyncio.Event] = None
 
         self.ticket_generator = ticket_generator()
         self.events: EventBus = event_bus or EventBus()
@@ -66,15 +67,16 @@
         self.distributed_network: DistributedNetwork = self.create_distributed_network()
 
         self.users: UserManager = self.create_user_manager()
         self.rooms: RoomManager = self.create_room_manager()
         self.interests: InterestManager = self.create_interest_manager()
 
         self.shares: SharesManager = self.create_shares_manager(
-            shares_cache or SharesNullCache()
+            shares_cache or SharesNullCache(),
+            executor_factory=executor_factory
         )
         self.transfers: TransferManager = self.create_transfer_manager(
             transfer_cache or TransferNullCache()
         )
         self.peers: PeerManager = self.create_peer_manager()
         self.searches: SearchManager = self.create_search_manager()
         self.server_manager: ServerManager = self.create_server_manager()
@@ -305,20 +307,24 @@
         return InterestManager(
             self.settings,
             self.events,
             self.users,
             self.network
         )
 
-    def create_shares_manager(self, cache: SharesCache) -> SharesManager:
+    def create_shares_manager(
+            self, cache: SharesCache,
+            executor_factory: Optional[ExecutorFactory] = None) -> SharesManager:
+
         return SharesManager(
             self.settings,
             self.events,
             self.network,
-            cache=cache
+            cache=cache,
+            executor_factory=executor_factory
         )
 
     def create_transfer_manager(self, cache: TransferCache) -> TransferManager:
         return TransferManager(
             self.settings,
             self.events,
             self.users,
```

### Comparing `aioslsk-1.3.0/src/aioslsk/commands.py` & `aioslsk-1.3.1/src/aioslsk/commands.py`

 * *Files identical despite different names*

### Comparing `aioslsk-1.3.0/src/aioslsk/constants.py` & `aioslsk-1.3.1/src/aioslsk/constants.py`

 * *Files identical despite different names*

### Comparing `aioslsk-1.3.0/src/aioslsk/distributed.py` & `aioslsk-1.3.1/src/aioslsk/distributed.py`

 * *Files identical despite different names*

### Comparing `aioslsk-1.3.0/src/aioslsk/events.py` & `aioslsk-1.3.1/src/aioslsk/events.py`

 * *Files identical despite different names*

### Comparing `aioslsk-1.3.0/src/aioslsk/exceptions.py` & `aioslsk-1.3.1/src/aioslsk/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioslsk-1.3.0/src/aioslsk/interest/manager.py` & `aioslsk-1.3.1/src/aioslsk/interest/manager.py`

 * *Files identical despite different names*

### Comparing `aioslsk-1.3.0/src/aioslsk/naming.py` & `aioslsk-1.3.1/src/aioslsk/naming.py`

 * *Files identical despite different names*

### Comparing `aioslsk-1.3.0/src/aioslsk/network/connection.py` & `aioslsk-1.3.1/src/aioslsk/network/connection.py`

 * *Files identical despite different names*

### Comparing `aioslsk-1.3.0/src/aioslsk/network/network.py` & `aioslsk-1.3.1/src/aioslsk/network/network.py`

 * *Files identical despite different names*

### Comparing `aioslsk-1.3.0/src/aioslsk/network/rate_limiter.py` & `aioslsk-1.3.1/src/aioslsk/network/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `aioslsk-1.3.0/src/aioslsk/network/upnp.py` & `aioslsk-1.3.1/src/aioslsk/network/upnp.py`

 * *Files identical despite different names*

### Comparing `aioslsk-1.3.0/src/aioslsk/peer.py` & `aioslsk-1.3.1/src/aioslsk/peer.py`

 * *Files identical despite different names*

### Comparing `aioslsk-1.3.0/src/aioslsk/protocol/messages.py` & `aioslsk-1.3.1/src/aioslsk/protocol/messages.py`

 * *Files identical despite different names*

### Comparing `aioslsk-1.3.0/src/aioslsk/protocol/obfuscation.py` & `aioslsk-1.3.1/src/aioslsk/protocol/obfuscation.py`

 * *Files identical despite different names*

### Comparing `aioslsk-1.3.0/src/aioslsk/protocol/primitives.py` & `aioslsk-1.3.1/src/aioslsk/protocol/primitives.py`

 * *Files identical despite different names*

### Comparing `aioslsk-1.3.0/src/aioslsk/room/manager.py` & `aioslsk-1.3.1/src/aioslsk/room/manager.py`

 * *Files identical despite different names*

### Comparing `aioslsk-1.3.0/src/aioslsk/room/model.py` & `aioslsk-1.3.1/src/aioslsk/room/model.py`

 * *Files identical despite different names*

### Comparing `aioslsk-1.3.0/src/aioslsk/search/manager.py` & `aioslsk-1.3.1/src/aioslsk/search/manager.py`

 * *Files identical despite different names*

### Comparing `aioslsk-1.3.0/src/aioslsk/search/model.py` & `aioslsk-1.3.1/src/aioslsk/search/model.py`

 * *Files identical despite different names*

### Comparing `aioslsk-1.3.0/src/aioslsk/server.py` & `aioslsk-1.3.1/src/aioslsk/server.py`

 * *Files identical despite different names*

### Comparing `aioslsk-1.3.0/src/aioslsk/settings.py` & `aioslsk-1.3.1/src/aioslsk/settings.py`

 * *Files identical despite different names*

### Comparing `aioslsk-1.3.0/src/aioslsk/shares/cache.py` & `aioslsk-1.3.1/src/aioslsk/shares/cache.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,21 +20,23 @@
         return []
 
     def write(self, shared_directories: List[SharedDirectory]):  # pragma: no cover
         pass
 
 
 class SharesShelveCache:
+    """Shares cache that uses the Python built-in `shelve` module"""
     DEFAULT_FILENAME = 'shares_index'
 
-    def __init__(self, data_directory: str):
+    def __init__(self, data_directory: str, filename: str = DEFAULT_FILENAME):
         self.data_directory: str = data_directory
+        self.filename: str = filename
 
     def _get_index_path(self) -> str:
-        return os.path.join(self.data_directory, self.DEFAULT_FILENAME)
+        return os.path.join(self.data_directory, self.filename)
 
     def read(self) -> List[SharedDirectory]:
         with shelve.open(self._get_index_path(), 'c') as db:
             directories: List[SharedDirectory] = db.get('index', list())
             for directory in directories:
                 new_items = set()
                 for item in directory.items:
```

### Comparing `aioslsk-1.3.0/src/aioslsk/shares/manager.py` & `aioslsk-1.3.1/src/aioslsk/shares/manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 from aiofiles import os as asyncos
 import asyncio
+from concurrent.futures import Executor
 from functools import partial
 import logging
 import mutagen
 from mutagen.mp3 import BitrateMode
 import os
 import re
 import sys
 import time
-from typing import Optional, Dict, List, Set, Tuple, Union
+from typing import (
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Set,
+    Tuple,
+    Union,
+)
 import uuid
 from weakref import WeakSet
 
 from ..base_manager import BaseManager
 from .cache import SharesNullCache, SharesCache
 from ..events import (
     EventBus,
@@ -37,14 +46,16 @@
 from ..search.model import SearchQuery
 from ..session import Session
 from ..settings import Settings
 from .utils import convert_items_to_file_data
 
 logger = logging.getLogger(__name__)
 
+ItemAttributes = List[Tuple[int, int]]
+ExecutorFactory = Callable[[], Executor]
 
 _COMPRESSED_FORMATS = [
     'MP3',
     'MP4',
     'ASF',  # WMA
     'OggVorbis'
 ]
@@ -57,14 +68,20 @@
 
 
 def scan_directory(
         shared_directory: SharedDirectory,
         children: Optional[List[SharedDirectory]] = None) -> Set[SharedItem]:
     """Scans the directory for items to share
 
+    Warning: when using ProcessPoolExecutor on this method the returned items
+    will not have the shared directory set in some cases. The shared_directory
+    passed here is a copy and the object will be removed once this function
+    finishes (see https://stackoverflow.com/a/72726998/1419478). In this case
+    you should manually assign it again
+
     :param shared_directory: `SharedDirectory` instance
     :param children: list of `SharedDirectory` instances, the items in this list
         will not be returned and should be scanned individually
     :return: set of `SharedItem` objects found during the scan
     """
     children = children or []
     shared_items = set()
@@ -90,15 +107,15 @@
                 shared_items.add(
                     SharedItem(shared_directory, subdir, filename, modified)
                 )
 
     return shared_items
 
 
-def extract_attributes(filepath: str) -> List[Tuple[int, int]]:
+def extract_attributes(filepath: str) -> ItemAttributes:
     """Attempts to extract attributes from the file at `filepath`. If there was
     an error attempting to extract the attributes this method will log a warning
     and return an empty list of attributes
     """
     attributes = []
     try:
         mutagen_file = mutagen.File(filepath)
@@ -133,24 +150,26 @@
 
 
 class SharesManager(BaseManager):
     _ALIAS_LENGTH = 5
 
     def __init__(
             self, settings: Settings, event_bus: EventBus,
-            network: Network, cache: Optional[SharesCache] = None):
+            network: Network, cache: Optional[SharesCache] = None,
+            executor_factory: Optional[ExecutorFactory] = None):
         self._settings: Settings = settings
         self._event_bus: EventBus = event_bus
         self._network: Network = network
         self._term_map: Dict[str, WeakSet[SharedItem]] = {}
-        self._shared_directories: List[SharedDirectory] = list()
+        self._shared_directories: List[SharedDirectory] = []
         self._session: Optional[Session] = None
 
         self.cache: SharesCache = cache if cache else SharesNullCache()
-        self.executor = None
+        self.executor: Optional[Executor] = None
+        self.executor_factory: Optional[ExecutorFactory] = executor_factory
 
         self.naming_strategies = [
             DefaultNamingStrategy(),
             NumberDuplicateStrategy()
         ]
 
         self.register_listeners()
@@ -195,29 +214,61 @@
 
         # To lowercase
         alias_bytes = bytes([(byte % 26) + 0x61 for byte in alias_bytearr])
         alias_string = alias_bytes.decode('utf8')
 
         return alias_string
 
+    async def start(self):
+        if self.executor_factory:
+            self.executor = self.executor_factory()
+
+    async def stop(self) -> List[asyncio.Task]:
+        if self.executor:
+            self.executor.shutdown()
+            self.executor = None
+
+        return []
+
     async def load_data(self):
         self.read_cache()
         self.load_from_settings()
 
     async def store_data(self):
         self.write_cache()
 
     def load_from_settings(self):
-        """Loads the directories from the settings"""
-        for shared_directory in self._settings.shares.directories:
-            self.add_shared_directory(
-                shared_directory.path,
-                share_mode=shared_directory.share_mode,
-                users=shared_directory.users
-            )
+        """Loads the shared directories from the settings. Existing directories
+        will be updated, non-existing directories added, directories that no
+        longer exist will be removed
+        """
+        new_shared_directories: List[SharedDirectory] = []
+
+        # Add or update directories
+        for directory_entry in self._settings.shares.directories:
+            try:
+                shared_directory = self.get_shared_directory(directory_entry.path)
+            except SharedDirectoryError:
+                shared_directory = self.add_shared_directory(
+                    directory_entry.path,
+                    share_mode=directory_entry.share_mode,
+                    users=directory_entry.users
+                )
+            else:
+                self.update_shared_directory(
+                    shared_directory,
+                    share_mode=directory_entry.share_mode,
+                    users=directory_entry.users or []
+                )
+
+            new_shared_directories.append(shared_directory)
+
+        self._shared_directories = new_shared_directories
+
+        self.rebuild_term_map()
 
     def read_cache(self):
         """Read the directories from the cache"""
         logger.info("reading directories from cache")
         directories = self.cache.read()
         logger.info(f"read {len(directories)} directories from cache")
         self._shared_directories = directories
@@ -254,22 +305,23 @@
         for item in shared_directory.items:
             self._add_item_to_term_map(item)
         logger.debug(f"term map contains {len(self._term_map)} terms")
 
     async def get_shared_item(self, remote_path: str, username: Optional[str] = None) -> SharedItem:
         """Gets a shared item from the cache based on the given file path. If
         the file does not exist in the `shared_items` or the file is present
-        in the cache but does not exist on disk a `FileNotFoundError` is raised
+        in the cache but does not exist on disk a :class:`.FileNotFoundError` is
+        raised
 
         If a `username` is passed this will also check if the file is locked
-        and raise a `FileNotSharedError` if the file is not accessible for that
-        user
+        and raise a :class:`.FileNotSharedError` if the file is not accessible
+        for that user
 
         :param remote_path: the remote_path
-        :param username:
+        :param username: optional username to check if the file is shared or not
         :raise FileNotFoundError: filename was not found in shared_items or was found
             but did not exist on disk
         :raise FileNotSharedError: file is found, but locked for the given
             `username`
         """
         for shared_directory in self._shared_directories:
             try:
@@ -289,51 +341,79 @@
             raise FileNotFoundError(f"file name {remote_path} not found in cache")
 
     def add_shared_directory(
             self, shared_directory: str,
             share_mode: DirectoryShareMode = DirectoryShareMode.EVERYONE,
             users: Optional[List[str]] = None) -> SharedDirectory:
         """Adds a shared directory. This method will call `generate_alias` and
-        add the directory to the directory map.
+        add the directory to the directory map. This method will not scan the
+        directory, for scanning see the :meth:`scan`, :meth:`scan_directory_files`
+        and :meth:`scan_directory_file_attributes` methods.
 
         :param shared_directory: path of the shared directory
         :param share_mode: the share mode for the directory
         :param users: in case the share mode is `USERS`, a list of users to
             share it with
-        :return: a `SharedDirectory` object
+        :return: a :class:`.SharedDirectory` object
+        :raise SharedDirectoryError: if the directory is already shared
         """
-        # Calc absolute path, generate an alias and store it
+        if self.is_directory_shared(shared_directory):
+            raise SharedDirectoryError(
+                f"directory {shared_directory} is already shared")
+
+        # Generate an absolute path, alias and create the object
         abs_directory = os.path.normpath(os.path.abspath(shared_directory))
         alias = self.generate_alias(abs_directory)
 
-        # Check if we have an existing shared directory, otherwise return it
         directory_object = SharedDirectory(
             shared_directory,
             abs_directory,
             alias,
             share_mode=share_mode,
             users=users or []
         )
-        for shared_dir in self._shared_directories:
-            if shared_dir == directory_object:
-                return shared_dir
 
         # If the new directory is a child of an existing directory, move items
         # to the child directory and remove them from the parent directory
         parents = self._get_parent_directories(directory_object)
         if parents:
             parent = parents[-1]
             children = parent.get_items_for_directory(directory_object)
             directory_object.items |= children
             parent.items -= children
 
         self._shared_directories.append(directory_object)
         return directory_object
 
-    def remove_shared_directory(self, directory: SharedDirectory):
+    def update_shared_directory(
+            self, directory: Union[str, SharedDirectory],
+            share_mode: Optional[DirectoryShareMode] = None,
+            users: Optional[List[str]] = None) -> SharedDirectory:
+        """Updates `share_mode` and `users` values for the given directory
+
+        :param directory: if a string is given this method will attempt to find
+            the shared directory based on the absolute path
+        :return: the updated directory
+        :raise SharedDirectoryError: if the given directory is a string and not
+            in the list of shared directories
+        """
+        if isinstance(directory, str):
+            shared_directory = self.get_shared_directory(directory)
+        else:
+            shared_directory = directory
+
+        if share_mode is not None:
+            shared_directory.share_mode = share_mode
+
+        if users is not None:
+            shared_directory.users = users
+
+        return shared_directory
+
+    def remove_shared_directory(self, directory: Union[str, SharedDirectory]) -> SharedDirectory:
         """Removes the given shared directory. If the directory was a
         subdirectory of another shared directory its items will be moved into
         that directory
 
         Example file structure:
 
         * Music\\
@@ -351,38 +431,71 @@
         * Music\\ : EVERYONE
         * Music\\Artist_One\\ : FRIENDS
 
         And removes the `Music\\Artist_One\\ shared directory the files of that
         directory get returned back to the parent directory. In this case file
         `song_two.mp3` will be shared with EVERYONE again
 
-        :param shared_directory: `SharedDirectory` instance to remove
-        :raise SharedDirectoryError: raised when the passed `shared_directory`
-            was not added to the manager
+        :param shared_directory: :class:`.SharedDirectory` instance to remove
+        :return: the removed directory
+        :raise SharedDirectoryError: raised when the passed `directory` was not
+            added to the manager
         """
-        if directory not in self._shared_directories:
-            raise SharedDirectoryError(
-                "attempted to remove directory which was not added to the manager"
-            )
+        if isinstance(directory, str):
+            shared_directory = self.get_shared_directory(directory)
+        else:
+            if directory not in self._shared_directories:
+                raise SharedDirectoryError(
+                    "attempted to remove directory which was not added to the manager"
+                )
+            else:
+                shared_directory = directory
 
-        self._shared_directories.remove(directory)
+        self._shared_directories.remove(shared_directory)
 
-        parents = self._get_parent_directories(directory)
+        parents = self._get_parent_directories(shared_directory)
         # If the directory has a parent directory, move all items into that
         # directory
         if parents:
             parent = parents[-1]
-            parent.items |= directory.items
+            parent.items |= shared_directory.items
 
         self._cleanup_term_map()
 
+        return shared_directory
+
+    def get_shared_directory(self, directory: str) -> SharedDirectory:
+        """Calculates the absolute path of given `directory` and looks for the
+        matching :class:`SharedDirectory` instance
+
+        :raise SharedDirectoryError: if the directory is not found
+        """
+        abs_path = os.path.normpath(os.path.abspath(directory))
+        for shared_directory in self.shared_directories:
+            if shared_directory.absolute_path == abs_path:
+                return shared_directory
+
+        raise SharedDirectoryError(
+            f"did not find shared directory with path : {directory}")
+
+    def is_directory_shared(self, directory: str) -> bool:
+        """Checks if a directory is already a shared directory by checking the
+        absolute path of that directory
+        """
+        try:
+            self.get_shared_directory(directory)
+        except SharedDirectoryError:
+            return False
+        else:
+            return True
+
     async def scan_directory_files(self, shared_directory: SharedDirectory):
         """Scans the files for the given `shared_directory`
 
-        :param shared_directory: `SharedDirectory` instance to scan
+        :param shared_directory: :class:`.SharedDirectory` instance to scan
         :raise SharedDirectoryError: raised when the passed `shared_directory`
             was not added to the manager
         """
         loop = asyncio.get_running_loop()
 
         if shared_directory not in self._shared_directories:
             raise SharedDirectoryError(
@@ -400,81 +513,98 @@
                 )
             )
         except Exception:
             logger.exception(f"exception scanning directory : {shared_directory!r}")
         else:
             logger.debug(f"scan found {len(shared_items)} files for directory {shared_directory!r}")
 
+            # When using a ProcessPoolExecutor the `shared_directory` property
+            # might be set to None (since objects are cloned instead of passed
+            # by reference). Re-assign it the proper object
+            for item in shared_items:
+                item.shared_directory = shared_directory
+
             # Adds all new items to the directory items
             shared_directory.items |= shared_items
+
             # Remove all items from the cache that weren't in the returned items
-            # set
+            # set. Because the `modified` parameter is part of the hash items
+            # with a changed `modified` parameter will also be removed meaning
+            # their attributes will be reset and these files attributes need
+            # to be rescanned
             shared_directory.items -= (shared_directory.items ^ shared_items)
 
         self._build_term_map(shared_directory)
         self._cleanup_term_map()
 
     async def scan_directory_file_attributes(self, shared_directory: SharedDirectory):
         """Scans the file attributes for files in the given `shared_directory`.
         only files that do not yet have attributes will be scanned
 
         The results of the scan are handled internally and are automatically to
-        the `SharedItem` object for which the scan was performed
+        the :class:`.SharedItem` object for which the scan was performed
 
-        :param shared_directory: `SharedDirectory` instance for which the files
-            need to be scanned
+        :param shared_directory: :class:`.SharedDirectory` instance for which
+            the files need to be scanned
         :return: List of futures for each file that needs to be scanned
         """
-        def extract_item_attributes(item: SharedItem):
-            return item, extract_attributes(item.get_absolute_path())
-
         loop = asyncio.get_running_loop()
 
         # Schedule the items on the executor
-        extract_futures: List[asyncio.Future] = []
+        futures: List[asyncio.Future] = []
         for item in shared_directory.items:
             if item.attributes is None:
                 future = loop.run_in_executor(
                     self.executor,
-                    partial(extract_item_attributes, item)
+                    partial(extract_attributes, item.get_absolute_path())
                 )
-                extract_futures.append(future)
+                future.add_done_callback(
+                    partial(self._extract_attributes_callback, item)
+                )
+                futures.append(future)
 
         logger.debug(
-            f"scheduled {len(extract_futures)} / {len(shared_directory.items)} items "
+            f"scheduled {len(futures)} / {len(shared_directory.items)} items "
             f"for attribute extracting for directory {shared_directory}")
 
-        for future in asyncio.as_completed(extract_futures):
-            try:
-                item, attributes = await future
-            except Exception:
-                logger.warning("exception fetching shared item attributes")
-            else:
-                item.attributes = attributes
+        start = time.perf_counter()
+
+        await asyncio.gather(*futures, return_exceptions=True)
+
+        logger.debug(
+            f"scanned attributes for {len(futures)} items in {time.perf_counter() - start}s")
+
+    def _extract_attributes_callback(self, item: SharedItem, future: asyncio.Future):
+        try:
+            attributes = future.result()
+        except Exception:
+            logger.warning("exception fetching shared item attributes")
+        else:
+            item.attributes = attributes
 
     async def scan(self):
         """Scan the files and their attributes for all directories currently
         defined in the `shared_directories`
 
-        This method will emit a `ScanCompleteEvent` on the event bus and report
-        the shares to the server
+        This method will emit a :class:`.ScanCompleteEvent` on the event bus
+        and report the shares to the server
         """
         start_time = time.perf_counter()
 
         files_tasks = [
             self.scan_directory_files(shared_directory)
             for shared_directory in self._shared_directories
         ]
         await asyncio.gather(*files_tasks, return_exceptions=True)
 
         attribute_futures = [
             self.scan_directory_file_attributes(shared_directory)
             for shared_directory in self._shared_directories
         ]
-        await asyncio.gather(*attribute_futures, return_exceptions=True)
+        await asyncio.gather(*attribute_futures)
 
         logger.info(f"completed scan in {time.perf_counter() - start_time} seconds")
         folder_count, file_count = self.get_stats()
         await self._event_bus.emit(
             ScanCompleteEvent(folder_count, file_count)
         )
 
@@ -627,15 +757,15 @@
             else:
                 public_dirs.append(shared_dir)
 
         return public_dirs, locked_dirs
 
     def create_shares_reply(self, username: str) -> Tuple[List[DirectoryData], List[DirectoryData]]:
         """Creates a complete list of the currently shared items as a reply to
-        a `PeerSharesRequest` messages
+        a :class:`.PeerSharesRequest` messages
 
         :param username: username of the user requesting the shares reply, this
             is used to determine the locked results
         :return: tuple with two lists: public directories and locked directories
         """
         def list_unique_directories(directories: List[SharedDirectory]) -> Dict[Tuple[str, ...], List[SharedItem]]:
             response_dirs: Dict[Tuple[str, ...], List[SharedItem]] = {}
```

### Comparing `aioslsk-1.3.0/src/aioslsk/shares/model.py` & `aioslsk-1.3.1/src/aioslsk/shares/model.py`

 * *Files identical despite different names*

### Comparing `aioslsk-1.3.0/src/aioslsk/shares/utils.py` & `aioslsk-1.3.1/src/aioslsk/shares/utils.py`

 * *Files identical despite different names*

### Comparing `aioslsk-1.3.0/src/aioslsk/transfer/cache.py` & `aioslsk-1.3.1/src/aioslsk/transfer/cache.py`

 * *Files identical despite different names*

### Comparing `aioslsk-1.3.0/src/aioslsk/transfer/manager.py` & `aioslsk-1.3.1/src/aioslsk/transfer/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -435,14 +435,15 @@
         :return: The matching transfer object
         :raise ValueError: If the transfer is not found
         """
         req_transfer = Transfer(username, remote_path, direction)
         for transfer in self._transfers:
             if transfer == req_transfer:
                 return transfer
+
         raise ValueError(
             f"transfer for user {username} and remote_path {remote_path} (direction={direction}) not found")
 
     async def manage_user_tracking(self):
         """Remove or add user tracking based on the list of transfers. This
         method will untrack users for which there are no more unfinished
         transfers and start/keep tracking users for which there are unfinished
```

### Comparing `aioslsk-1.3.0/src/aioslsk/transfer/model.py` & `aioslsk-1.3.1/src/aioslsk/transfer/model.py`

 * *Files identical despite different names*

### Comparing `aioslsk-1.3.0/src/aioslsk/transfer/state.py` & `aioslsk-1.3.1/src/aioslsk/transfer/state.py`

 * *Files identical despite different names*

### Comparing `aioslsk-1.3.0/src/aioslsk/user/manager.py` & `aioslsk-1.3.1/src/aioslsk/user/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,16 +189,16 @@
         for friend in self._settings.users.friends:
             tasks.append(self.track_user(friend, TrackingFlag.FRIEND))
 
         await asyncio.gather(*tasks, return_exceptions=True)
 
     async def untrack_user(self, username: str, flag: TrackingFlag):
         """Removes the given flag from the user and untracks the user (send
-        `RemoveUser` message) in case none of the AddUser tracking flags are
-        set or the removed tracking flag is `TrackingFlag.REQUESTED`.
+        :class:`.RemoveUser` message) in case none of the AddUser tracking flags
+        are set or the removed tracking flag is `TrackingFlag.REQUESTED`.
 
         The user will be removed from the tracked users if there are no flags
         left, if there is still a reference left to the user it will remain
         stored
 
         :param username: user to untrack
         :param flag: tracking flag to remove from the user
```

### Comparing `aioslsk-1.3.0/src/aioslsk/user/model.py` & `aioslsk-1.3.1/src/aioslsk/user/model.py`

 * *Files identical despite different names*

### Comparing `aioslsk-1.3.0/src/aioslsk/utils.py` & `aioslsk-1.3.1/src/aioslsk/utils.py`

 * *Files identical despite different names*

### Comparing `aioslsk-1.3.0/PKG-INFO` & `aioslsk-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioslsk
-Version: 1.3.0
+Version: 1.3.1
 Summary: Asyncio based SoulSeek client
 Home-page: https://github.com/JurgenR/aioslsk/
 License: GPL-3.0-or-later
 Keywords: soulseek,p2p,async
 Author: JurgenR
 Author-email: 1249228+JurgenR@users.noreply.github.com
 Requires-Python: >=3.8,<3.13
```

