# Comparing `tmp/fastosc-0.0.2.tar.gz` & `tmp/fastosc-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/sahlen/repositories/oslo1989/fastosc/dist/.tmp-kd_1fa88/fastosc-0.0.2.tar", last modified: Sun May  5 14:24:01 2024, max compression
+gzip compressed data, was "/Users/sahlen/repositories/oslo1989/fastosc/dist/.tmp-3wowlisi/fastosc-0.0.3.tar", last modified: Sun May  5 19:25:48 2024, max compression
```

## Comparing `fastosc-0.0.2.tar` & `fastosc-0.0.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 fastosc-0.0.2/
--rw-r--r--   0 sahlen     (501) staff       (20)      611 2024-05-05 14:24:01.000000 fastosc-0.0.2/PKG-INFO
--rw-r--r--   0 sahlen     (501) staff       (20)      280 2024-05-05 12:26:24.000000 fastosc-0.0.2/README.md
--rw-r--r--   0 sahlen     (501) staff       (20)      930 2024-05-05 14:14:28.000000 fastosc-0.0.2/pyproject.toml
--rw-r--r--   0 sahlen     (501) staff       (20)       38 2024-05-05 14:24:01.000000 fastosc-0.0.2/setup.cfg
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 fastosc-0.0.2/src/
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 fastosc-0.0.2/src/fastosc/
--rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-01-13 16:36:43.000000 fastosc-0.0.2/src/fastosc/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 fastosc-0.0.2/src/fastosc/dispatcher/
--rw-r--r--   0 sahlen     (501) staff       (20)     5937 2024-01-20 18:59:40.000000 fastosc-0.0.2/src/fastosc/dispatcher/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)      250 2024-01-20 18:33:22.000000 fastosc-0.0.2/src/fastosc/dispatcher/handler.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 fastosc-0.0.2/src/fastosc/docs/
--rw-r--r--   0 sahlen     (501) staff       (20)      313 2024-01-20 18:35:02.000000 fastosc-0.0.2/src/fastosc/docs/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 fastosc-0.0.2/src/fastosc/message/
--rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-01-13 21:23:05.000000 fastosc-0.0.2/src/fastosc/message/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9145 2024-01-20 16:18:06.000000 fastosc-0.0.2/src/fastosc/message/arg_value.py
--rw-r--r--   0 sahlen     (501) staff       (20)      457 2024-01-20 16:19:12.000000 fastosc-0.0.2/src/fastosc/message/convert.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3767 2024-01-19 08:45:29.000000 fastosc-0.0.2/src/fastosc/message/osc_bundle.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1960 2024-01-19 08:45:18.000000 fastosc-0.0.2/src/fastosc/message/osc_bundle_builder.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4587 2024-01-19 08:44:11.000000 fastosc-0.0.2/src/fastosc/message/osc_message.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7152 2024-01-20 19:54:40.000000 fastosc-0.0.2/src/fastosc/message/osc_message_builder.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 fastosc-0.0.2/src/fastosc/message/parsing/
--rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-01-08 21:16:09.000000 fastosc-0.0.2/src/fastosc/message/parsing/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1845 2024-01-13 21:33:36.000000 fastosc-0.0.2/src/fastosc/message/parsing/ntp.py
--rw-r--r--   0 sahlen     (501) staff       (20)    15342 2024-01-19 07:40:48.000000 fastosc-0.0.2/src/fastosc/message/parsing/osc_types.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 fastosc-0.0.2/src/fastosc/router/
--rw-r--r--   0 sahlen     (501) staff       (20)    11175 2024-01-20 19:00:31.000000 fastosc-0.0.2/src/fastosc/router/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 fastosc-0.0.2/src/fastosc/server/
--rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-01-19 10:51:55.000000 fastosc-0.0.2/src/fastosc/server/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)      442 2024-01-20 10:37:22.000000 fastosc-0.0.2/src/fastosc/server/dispatcher_server.py
--rw-r--r--   0 sahlen     (501) staff       (20)      960 2024-01-20 10:37:22.000000 fastosc-0.0.2/src/fastosc/server/server_base.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 fastosc-0.0.2/src/fastosc/server/udp/
--rw-r--r--   0 sahlen     (501) staff       (20)     2645 2024-01-19 13:17:58.000000 fastosc-0.0.2/src/fastosc/server/udp/udp_pull_server.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1447 2024-01-19 14:04:48.000000 fastosc-0.0.2/src/fastosc/server/udp/udp_server_base.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 fastosc-0.0.2/src/fastosc.egg-info/
--rw-r--r--   0 sahlen     (501) staff       (20)      611 2024-05-05 14:24:01.000000 fastosc-0.0.2/src/fastosc.egg-info/PKG-INFO
--rw-r--r--   0 sahlen     (501) staff       (20)      872 2024-05-05 14:24:01.000000 fastosc-0.0.2/src/fastosc.egg-info/SOURCES.txt
--rw-r--r--   0 sahlen     (501) staff       (20)        1 2024-05-05 14:24:01.000000 fastosc-0.0.2/src/fastosc.egg-info/dependency_links.txt
--rw-r--r--   0 sahlen     (501) staff       (20)        8 2024-05-05 14:24:01.000000 fastosc-0.0.2/src/fastosc.egg-info/top_level.txt
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:48.000000 fastosc-0.0.3/
+-rw-r--r--   0 sahlen     (501) staff       (20)      611 2024-05-05 19:25:48.000000 fastosc-0.0.3/PKG-INFO
+-rw-r--r--   0 sahlen     (501) staff       (20)      280 2024-05-05 12:26:24.000000 fastosc-0.0.3/README.md
+-rw-r--r--   0 sahlen     (501) staff       (20)      978 2024-05-05 19:25:25.000000 fastosc-0.0.3/pyproject.toml
+-rw-r--r--   0 sahlen     (501) staff       (20)       38 2024-05-05 19:25:48.000000 fastosc-0.0.3/setup.cfg
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:48.000000 fastosc-0.0.3/src/
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:48.000000 fastosc-0.0.3/src/fastosc/
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-01-13 16:36:43.000000 fastosc-0.0.3/src/fastosc/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:48.000000 fastosc-0.0.3/src/fastosc/dispatcher/
+-rw-r--r--   0 sahlen     (501) staff       (20)     5984 2024-05-05 18:52:23.000000 fastosc-0.0.3/src/fastosc/dispatcher/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      250 2024-01-20 18:33:22.000000 fastosc-0.0.3/src/fastosc/dispatcher/handler.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:48.000000 fastosc-0.0.3/src/fastosc/docs/
+-rw-r--r--   0 sahlen     (501) staff       (20)      313 2024-01-20 18:35:02.000000 fastosc-0.0.3/src/fastosc/docs/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:48.000000 fastosc-0.0.3/src/fastosc/message/
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-01-13 21:23:05.000000 fastosc-0.0.3/src/fastosc/message/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9145 2024-01-20 16:18:06.000000 fastosc-0.0.3/src/fastosc/message/arg_value.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      457 2024-01-20 16:19:12.000000 fastosc-0.0.3/src/fastosc/message/convert.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3789 2024-05-05 18:52:23.000000 fastosc-0.0.3/src/fastosc/message/osc_bundle.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1979 2024-05-05 18:51:01.000000 fastosc-0.0.3/src/fastosc/message/osc_bundle_builder.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4812 2024-05-05 18:54:34.000000 fastosc-0.0.3/src/fastosc/message/osc_message.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     7201 2024-05-05 18:52:23.000000 fastosc-0.0.3/src/fastosc/message/osc_message_builder.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:48.000000 fastosc-0.0.3/src/fastosc/message/parsing/
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-01-08 21:16:09.000000 fastosc-0.0.3/src/fastosc/message/parsing/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1871 2024-05-05 18:49:06.000000 fastosc-0.0.3/src/fastosc/message/parsing/ntp.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    15417 2024-05-05 18:52:23.000000 fastosc-0.0.3/src/fastosc/message/parsing/osc_types.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:48.000000 fastosc-0.0.3/src/fastosc/router/
+-rw-r--r--   0 sahlen     (501) staff       (20)    11251 2024-05-05 18:52:23.000000 fastosc-0.0.3/src/fastosc/router/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:48.000000 fastosc-0.0.3/src/fastosc/server/
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-01-19 10:51:55.000000 fastosc-0.0.3/src/fastosc/server/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      450 2024-05-05 18:27:52.000000 fastosc-0.0.3/src/fastosc/server/dispatcher_server.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      964 2024-05-05 18:27:52.000000 fastosc-0.0.3/src/fastosc/server/server_base.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:48.000000 fastosc-0.0.3/src/fastosc/server/udp/
+-rw-r--r--   0 sahlen     (501) staff       (20)     2657 2024-05-05 18:55:35.000000 fastosc-0.0.3/src/fastosc/server/udp/udp_pull_server.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1447 2024-01-19 14:04:48.000000 fastosc-0.0.3/src/fastosc/server/udp/udp_server_base.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:48.000000 fastosc-0.0.3/src/fastosc.egg-info/
+-rw-r--r--   0 sahlen     (501) staff       (20)      611 2024-05-05 19:25:48.000000 fastosc-0.0.3/src/fastosc.egg-info/PKG-INFO
+-rw-r--r--   0 sahlen     (501) staff       (20)      872 2024-05-05 19:25:48.000000 fastosc-0.0.3/src/fastosc.egg-info/SOURCES.txt
+-rw-r--r--   0 sahlen     (501) staff       (20)        1 2024-05-05 19:25:48.000000 fastosc-0.0.3/src/fastosc.egg-info/dependency_links.txt
+-rw-r--r--   0 sahlen     (501) staff       (20)        8 2024-05-05 19:25:48.000000 fastosc-0.0.3/src/fastosc.egg-info/top_level.txt
```

### Comparing `fastosc-0.0.2/PKG-INFO` & `fastosc-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastosc
-Version: 0.0.2
+Version: 0.0.3
 Summary: Modern Python Library for OSC, using best practices such as typing, linting/formatting - inspired by FastAPI
 Author-email: Martin Sahlen <martin8900@gmail.com>
 Project-URL: Homepage, https://github.com/oslo1989/fastosc
 Project-URL: Issues, https://github.com/oslo1989/fastosc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fastosc-0.0.2/pyproject.toml` & `fastosc-0.0.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools"]
+requires = ["setuptools ~=68.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastosc"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     {name = "Martin Sahlen", email = "martin8900@gmail.com"}
 ]
 description = "Modern Python Library for OSC, using best practices such as typing, linting/formatting - inspired by FastAPI"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -19,12 +19,13 @@
 ]
 
 [project.urls]
 Homepage = "https://github.com/oslo1989/fastosc"
 Issues = "https://github.com/oslo1989/fastosc/issues"
 
 [tool.ruff]
-select = ["E", "F", "B", "W", "I" ,"UP", "ANN", "BLE", "FBT", "A", "COM", "C4", "DTZ", "PIE", "Q", "RET", "SIM", "PL", "RUF"]
-extend-select = ["I"]
-fixable = ["ALL"]
+lint.select = ["E", "F", "B", "W", "I" ,"UP", "ANN", "BLE", "FBT", "A", "COM", "C4", "DTZ", "PIE", "Q", "RET", "SIM", "PL", "RUF"]
+lint.extend-select = ["I"]
+lint.fixable = ["ALL"]
 line-length = 120
-target-version = "py37"
+lint.ignore = ["ANN101"]
+target-version = "py37"
```

### Comparing `fastosc-0.0.2/src/fastosc/dispatcher/__init__.py` & `fastosc-0.0.3/src/fastosc/dispatcher/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from fastosc.message.osc_message import OscMessage
 from fastosc.server.server_base import OSCServerBase
 
 MAX_LINE_LENGTH = 45
 
 
 class Dispatcher:
-    def __init__(self, *, logger: logging.Logger, base_address: str = ""):
+    def __init__(self, *, logger: logging.Logger, base_address: str = "") -> None:
         self._server: OSCServerBase | None = None
         self._callbacks: dict[str, Callable[[list[ArgValue], tuple[str, int]], list[ArgValue]]] = {}
         self._logger = logger
         if not base_address.startswith("/"):
             base_address = f"/{base_address}"
         self._base_address = base_address
         self._handler_docs: list[HandlerDescription] = []
@@ -82,15 +82,20 @@
         """
         Remove all existing OSC handlers.
         """
 
         self._callbacks = {}
 
     def send(
-        self, *, address: str, remote_addr: tuple[str, int], params: list[ArgValue], include_base_address: bool = False
+        self,
+        *,
+        address: str,
+        remote_addr: tuple[str, int],
+        params: list[ArgValue],
+        include_base_address: bool = False,
     ) -> None:
         if self._server:
             if include_base_address:
                 address = f"{self._base_address}{address}"
             self._server.send(address=address, params=params, remote_addr=remote_addr)
         else:
             self._logger.error(f"Trying to send OSC message to remote address {remote_addr}, but not server is set up")
@@ -121,15 +126,15 @@
                         # be listened for (e.g. can_be_armed, is_foldable)
                         # --------------------------------------------------------------------------------
                         continue
                     if rv is not None:
                         assert isinstance(rv, list)
                         self.send(address=callback_address, params=rv, remote_addr=remote_addr)
         else:
-            self._logger.error("Unknown OSC address: %s" % message.address)
+            self._logger.error(f"Unknown OSC address: {message.address}")
             # todo: return the error to the socket that sent it
 
     def process_bundle(self, *, bundle: OscBundle, remote_addr: tuple[str, int]) -> None:
         for i in bundle:
             if OscBundle.dgram_is_bundle(i.dgram):
                 self.process_bundle(bundle=i, remote_addr=remote_addr)
             else:
```

### Comparing `fastosc-0.0.2/src/fastosc/message/arg_value.py` & `fastosc-0.0.3/src/fastosc/message/arg_value.py`

 * *Files identical despite different names*

### Comparing `fastosc-0.0.2/src/fastosc/message/osc_bundle.py` & `fastosc-0.0.3/src/fastosc/message/osc_bundle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# ruff: noqa: B904,ANN401
 from __future__ import annotations
 
 import logging
 from typing import Any, Iterator
 
 from fastosc.message import osc_message
 from fastosc.message.parsing import osc_types
@@ -30,15 +31,15 @@
         """
         # Interesting stuff starts after the initial b"#bundle\x00".
         self._dgram = dgram
         index = len(_BUNDLE_PREFIX)
         try:
             self._timestamp, index = osc_types.get_date(self._dgram, index)
         except osc_types.ParseError as pe:
-            raise ParseError("Could not get the date from the datagram: %s" % pe)
+            raise ParseError(f"Could not get the date from the datagram: {pe}")
         # Get the contents as a list of OscBundle and OscMessage.
         self._contents = self._parse_contents(index)
 
     def _parse_contents(self, index: int) -> list[OscBundle | osc_message.OscMessage]:
         contents = []  # type: list[OscBundle | osc_message.OscMessage]
 
         try:
@@ -55,17 +56,17 @@
                 index += content_size
                 # Parse the content into an OSC message or bundle.
                 if OscBundle.dgram_is_bundle(content_dgram):
                     contents.append(OscBundle(content_dgram))
                 elif osc_message.OscMessage.dgram_is_message(content_dgram):
                     contents.append(osc_message.OscMessage(content_dgram))
                 else:
-                    logging.warning("Could not identify content type of dgram %r" % content_dgram)
+                    logging.warning(f"Could not identify content type of dgram {content_dgram!r}")
         except (osc_types.ParseError, osc_message.ParseError, IndexError) as e:
-            raise ParseError("Could not parse a content datagram: %s" % e)
+            raise ParseError(f"Could not parse a content datagram: {e}")
 
         return contents
 
     @staticmethod
     def dgram_is_bundle(dgram: bytes) -> bool:
         """Returns whether this datagram starts like an OSC bundle."""
         return dgram.startswith(_BUNDLE_PREFIX)
```

### Comparing `fastosc-0.0.2/src/fastosc/message/osc_bundle_builder.py` & `fastosc-0.0.3/src/fastosc/message/osc_bundle_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Build OSC bundles for client applications."""
+# ruff: noqa: B904
 
 from __future__ import annotations
 
 from fastosc.message import osc_bundle, osc_message
 from fastosc.message.parsing import osc_types
 
 # Shortcut to specify an immediate execution of messages in the bundle.
```

### Comparing `fastosc-0.0.2/src/fastosc/message/osc_message.py` & `fastosc-0.0.3/src/fastosc/message/osc_message.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Representation of an OSC message in a pythonesque way."""
+# ruff: noqa: B904,PLR0912,PLR0915,PLR2004
+
 from __future__ import annotations
 
 import logging
-from typing import Any, Iterator
+from typing import Iterator
 
 from fastosc.message.arg_value import ArgValue
 from fastosc.message.parsing import osc_types
 
 
 class ParseError(Exception):
     """Base exception raised when a datagram parsing error occurs."""
@@ -36,39 +38,39 @@
             if type_tag.startswith(","):
                 type_tag = type_tag[1:]
 
             params: list[ArgValue] = []
             param_stack = [params]
             # Parse each parameter given its type.
             for param in type_tag:
-                val = NotImplemented  # type: Any
+                val = NotImplemented  # Any
                 if param == "i":  # Integer.
-                    val, index = osc_types.get_int(self._dgram, index)
+                    val, index = osc_types.get_int(self._dgram, index)  # type: ignore
                 elif param == "h":  # Int64.
-                    val, index = osc_types.get_int64(self._dgram, index)
+                    val, index = osc_types.get_int64(self._dgram, index)  # type: ignore
                 elif param == "f":  # Float.
-                    val, index = osc_types.get_float(self._dgram, index)
+                    val, index = osc_types.get_float(self._dgram, index)  # type: ignore
                 elif param == "d":  # Double.
-                    val, index = osc_types.get_double(self._dgram, index)
+                    val, index = osc_types.get_double(self._dgram, index)  # type: ignore
                 elif param == "s":  # String.
-                    val, index = osc_types.get_string(self._dgram, index)
+                    val, index = osc_types.get_string(self._dgram, index)  # type: ignore
                 elif param == "b":  # Blob.
-                    val, index = osc_types.get_blob(self._dgram, index)
+                    val, index = osc_types.get_blob(self._dgram, index)  # type: ignore
                 elif param == "r":  # RGBA.
-                    val, index = osc_types.get_rgba(self._dgram, index)
+                    val, index = osc_types.get_rgba(self._dgram, index)  # type: ignore
                 elif param == "m":  # MIDI.
-                    val, index = osc_types.get_midi(self._dgram, index)
+                    val, index = osc_types.get_midi(self._dgram, index)  # type: ignore
                 elif param == "t":  # osc time tag:
-                    val, index = osc_types.get_timetag(self._dgram, index)
+                    val, index = osc_types.get_timetag(self._dgram, index)  # type: ignore
                 elif param == "T":  # True.
-                    val = True
+                    val = True  # type: ignore
                 elif param == "F":  # False.
-                    val = False
+                    val = False  # type: ignore
                 elif param == "N":  # Nil.
-                    val = None
+                    val = None  # type: ignore
                 elif param == "[":  # Array start.
                     array: list[ArgValue] = []
                     param_stack[-1].append(array)
                     param_stack.append(array)
                 elif param == "]":  # Array stop.
                     if len(param_stack) < 2:
                         raise ParseError(f"Unexpected closing bracket in type tag: {type_tag}")
```

### Comparing `fastosc-0.0.2/src/fastosc/message/osc_message_builder.py` & `fastosc-0.0.3/src/fastosc/message/osc_message_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """Build OSC messages for client applications."""
+
+# ruff: noqa: PLR2004
 from __future__ import annotations
 
 from datetime import datetime
 from typing import Any
 
 from fastosc.message import osc_message
 from fastosc.message.arg_value import (
@@ -22,14 +24,16 @@
     ARG_TYPE_TRUE,
     SUPPORTED_ARG_TYPES,
     ArgValue,
 )
 
 from .parsing import osc_types
 
+# ruff: noqa: PLR0912,B904
+
 
 class BuildError(Exception):
     """Error raised when an incomplete message is trying to be built."""
 
 
 class OscMessageBuilder:
     """Builds arbitrary OscMessage instances."""
@@ -57,15 +61,15 @@
     def args(self) -> list[tuple[str, ArgValue]]:
         """Returns the (type, value) arguments list of this message."""
         return self._args
 
     def _valid_type(self, arg_type: str) -> bool:
         if arg_type in SUPPORTED_ARG_TYPES:
             return True
-        elif isinstance(arg_type, (list, tuple)):
+        if isinstance(arg_type, (list, tuple)):
             return all(self._valid_type(sub_type) for sub_type in arg_type)
         return False
 
     def add_arg(self, arg_value: ArgValue, arg_type: str | None = None) -> None:
         """Add a typed argument to this message.
 
         Args:
```

### Comparing `fastosc-0.0.2/src/fastosc/message/parsing/ntp.py` & `fastosc-0.0.3/src/fastosc/message/parsing/ntp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Parsing and conversion of NTP dates contained in datagrams."""
+# ruff: noqa: BLE001,B904
 
 import datetime
 import struct
 import time
 from typing import NamedTuple
 
 # 63 zero bits followed by a one in the least signifigant bit is a special
```

### Comparing `fastosc-0.0.2/src/fastosc/message/parsing/osc_types.py` & `fastosc-0.0.3/src/fastosc/message/parsing/osc_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """Functions to get OSC types from datagrams and vice versa"""
+
+# ruff: noqa: FBT001,FBT002,B904
 from __future__ import annotations
 
 import math
 import struct
 from datetime import datetime, timedelta
 from typing import Tuple, cast
 
@@ -84,17 +86,17 @@
         # Python slices do not raise an IndexError past the last index,
         # do it ourselves.
         if offset > len(dgram[start_index:]):
             raise ParseError("Datagram is too short")
         data_str = dgram[start_index : start_index + offset]
         return data_str.replace(b"\x00", b"").decode("utf-8"), start_index + offset
     except IndexError as ie:
-        raise ParseError("Could not parse datagram %s" % ie)
+        raise ParseError(f"Could not parse datagram {ie}")
     except TypeError as te:
-        raise ParseError("Could not parse datagram %s" % te)
+        raise ParseError(f"Could not parse datagram {te}")
 
 
 def write_int(val: int) -> bytes:
     """Returns the datagram for the given integer parameter value
 
     Raises:
       - BuildError if the int could not be converted.
@@ -119,15 +121,15 @@
       ParseError if the datagram could not be parsed.
     """
     try:
         if len(dgram[start_index:]) < _INT_DGRAM_LEN:
             raise ParseError("Datagram is too short")
         return (struct.unpack(">i", dgram[start_index : start_index + _INT_DGRAM_LEN])[0], start_index + _INT_DGRAM_LEN)
     except (struct.error, TypeError) as e:
-        raise ParseError("Could not parse datagram %s" % e)
+        raise ParseError(f"Could not parse datagram {e}")
 
 
 def write_int64(val: int) -> bytes:
     """Returns the datagram for the given 64-bit big-endian signed parameter value
 
     Raises:
       - BuildError if the int64 could not be converted.
@@ -155,15 +157,15 @@
         if len(dgram[start_index:]) < _INT64_DGRAM_LEN:
             raise ParseError("Datagram is too short")
         return (
             struct.unpack(">q", dgram[start_index : start_index + _INT64_DGRAM_LEN])[0],
             start_index + _INT64_DGRAM_LEN,
         )
     except (struct.error, TypeError) as e:
-        raise ParseError("Could not parse datagram %s" % e)
+        raise ParseError(f"Could not parse datagram {e}")
 
 
 def get_uint64(dgram: bytes, start_index: int) -> tuple[int, int]:
     """Get a 64-bit big-endian unsigned integer from the datagram.
 
     Args:
       dgram: A datagram packet.
@@ -179,24 +181,23 @@
         if len(dgram[start_index:]) < _UINT64_DGRAM_LEN:
             raise ParseError("Datagram is too short")
         return (
             struct.unpack(">Q", dgram[start_index : start_index + _UINT64_DGRAM_LEN])[0],
             start_index + _UINT64_DGRAM_LEN,
         )
     except (struct.error, TypeError) as e:
-        raise ParseError("Could not parse datagram %s" % e)
+        raise ParseError(f"Could not parse datagram {e}")
 
 
 def write_timetag(ts: float | datetime) -> bytes:
     # do conversion
     if isinstance(ts, datetime):
         ts = ts.timestamp()
     if ts > 0:
         fract, secs = math.modf(ts)
-        secs = secs
         binary = struct.pack(">LL", secs, fract)
     else:
         binary = struct.pack(">LL", 0, 1)
 
     return binary
 
 
@@ -221,20 +222,23 @@
         timetag, _ = get_uint64(dgram, start_index)
         seconds, fraction = ntp.parse_timestamp(timetag)
 
         hours, seconds = seconds // 3600, seconds % 3600
         minutes, seconds = seconds // 60, seconds % 60
 
         utc = datetime.combine(ntp._NTP_EPOCH, datetime.min.time()) + timedelta(
-            hours=hours, minutes=minutes, seconds=seconds, microseconds=fraction
+            hours=hours,
+            minutes=minutes,
+            seconds=seconds,
+            microseconds=fraction,
         )
 
         return (utc, fraction), start_index + _TIMETAG_DGRAM_LEN
     except (struct.error, TypeError) as e:
-        raise ParseError("Could not parse datagram %s" % e)
+        raise ParseError(f"Could not parse datagram {e}")
 
 
 def write_float(val: float) -> bytes:
     """Returns the datagram for the given float parameter value
 
     Raises:
       - BuildError if the float could not be converted.
@@ -265,15 +269,15 @@
             # account for that.
             dgram = dgram + b"\x00" * (_FLOAT_DGRAM_LEN - len(dgram[start_index:]))
         return (
             struct.unpack(">f", dgram[start_index : start_index + _FLOAT_DGRAM_LEN])[0],
             start_index + _FLOAT_DGRAM_LEN,
         )
     except (struct.error, TypeError) as e:
-        raise ParseError("Could not parse datagram %s" % e)
+        raise ParseError(f"Could not parse datagram {e}")
 
 
 def write_double(val: float) -> bytes:
     """Returns the datagram for the given double parameter value
 
     Raises:
       - BuildError if the double could not be converted.
@@ -415,27 +419,30 @@
       ParseError if the datagram could not be parsed.
     """
     try:
         if len(dgram[start_index:]) < _INT_DGRAM_LEN:
             raise ParseError("Datagram is too short")
         return (struct.unpack(">I", dgram[start_index : start_index + _INT_DGRAM_LEN])[0], start_index + _INT_DGRAM_LEN)
     except (struct.error, TypeError) as e:
-        raise ParseError("Could not parse datagram %s" % e)
+        raise ParseError(f"Could not parse datagram {e}")
+
+
+MIDI_PACKET_LENGTH = 4
 
 
 def write_midi(val: MidiPacket) -> bytes:
     """Returns the datagram for the given MIDI message parameter value
 
        A valid MIDI message: (port id, status byte, data1, data2).
 
     Raises:
       - BuildError if the MIDI message could not be converted.
 
     """
-    if len(val) != 4:
+    if len(val) != MIDI_PACKET_LENGTH:
         raise BuildError("MIDI message length is invalid")
     try:
         value = sum((value & 0xFF) << 8 * (3 - pos) for pos, value in enumerate(val))
         return struct.pack(">I", value)
     except struct.error as e:
         raise BuildError(f"Wrong argument value passed: {e}")
 
@@ -456,8 +463,8 @@
     try:
         if len(dgram[start_index:]) < _INT_DGRAM_LEN:
             raise ParseError("Datagram is too short")
         val = struct.unpack(">I", dgram[start_index : start_index + _INT_DGRAM_LEN])[0]
         midi_msg = cast(MidiPacket, tuple((val & 0xFF << 8 * i) >> 8 * i for i in range(3, -1, -1)))
         return (midi_msg, start_index + _INT_DGRAM_LEN)
     except (struct.error, TypeError) as e:
-        raise ParseError("Could not parse datagram %s" % e)
+        raise ParseError(f"Could not parse datagram {e}")
```

### Comparing `fastosc-0.0.2/src/fastosc/router/__init__.py` & `fastosc-0.0.3/src/fastosc/router/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# ruff: noqa: FBT001,FBT002
 from __future__ import annotations
 
 import inspect
 import logging
 from typing import Any, Callable
 
 from fastosc.dispatcher import Dispatcher
@@ -52,30 +53,30 @@
 
         arg_count = f.__code__.co_argcount - 1
 
         shape_len = len(shape) - 1
 
         if shape_len < arg_count:
             raise InvalidParameterValueException(
-                f"too many arguments, expected {shape_len} " f"arguments but signature has {arg_count}."
+                f"too many arguments, expected {shape_len} " f"arguments but signature has {arg_count}.",
             )
-        elif shape_len > arg_count:
+        if shape_len > arg_count:
             raise InvalidParameterValueException(
-                f"too few arguments, expected {shape_len} " f"arguments but signature has {arg_count}."
+                f"too few arguments, expected {shape_len} " f"arguments but signature has {arg_count}.",
             )
 
         # do we do someting with remote_addres?
         # maybe include it if part of parameters? remote_addr param - inject as final param if needed
         def new_f(self: OSCRouter, original_args: list[ArgValue], remote_address: tuple[str, int]) -> list[ArgValue]:
             for a, t in zip(original_args, shape[1:] if len(shape) > 1 else []):
                 q = "'" if isinstance(a, str) else ""
                 if not isinstance(a, t):
                     raise InvalidParameterValueException(
                         f"arg {q}{a}{q} of type <{type(a).__name__}> "  # type: ignore[str-bytes-safe]
-                        f"does not match <{t.__name__}>"
+                        f"does not match <{t.__name__}>",
                     )
             args = original_args
             if include_remote_addr:
                 args = [*original_args, remote_address]  # type: ignore[list-item]
             if include_original_message:
                 args = [*args, original_args]  # type: ignore[list-item]
             return _format_response(f(self, *args))
@@ -83,15 +84,18 @@
         if listen:
             new_f.listen = True  # type: ignore[attr-defined]
         new_f.osc_handler = True  # type: ignore[attr-defined]
         new_f.address = f"/{prefix_}{address}"  # type: ignore[attr-defined]
         new_f.raw_address = address  # type: ignore[attr-defined]
         new_f.__name__ = f.__name__  # type: ignore[attr-defined]
         new_f.handler_info = HandlerInfo(  # type: ignore[attr-defined]
-            shape=orignal_shape, signature=sign, doc=inspect.getdoc(f), function_name=f.__name__
+            shape=orignal_shape,
+            signature=sign,
+            doc=inspect.getdoc(f),
+            function_name=f.__name__,
         )
         return new_f
 
     return check_accepts
 
 
 def osc_get(
@@ -161,15 +165,18 @@
         # here, we can just look up the result from the saved listener method and invoke it?
         # self.listeners[x] = _add_listener()
         # if self._listeners.get(x)]:
         #   self._listeners()
         pass
 
     def _setup_listener(
-        self, h: Callable[[list[ArgValue], tuple[str, int]], list[ArgValue]], start: bool = False, stop: bool = False
+        self,
+        h: Callable[[list[ArgValue], tuple[str, int]], list[ArgValue]],
+        start: bool = False,
+        stop: bool = False,
     ) -> tuple[str, Callable[[list[ArgValue], tuple[str, int]], list[ArgValue]]]:
         if not start and not stop:
             raise InvalidParameterValueException("Need to set either stop or start for listener")
         prefix = "/start_listen" if start else "/stop_listen"
         address: str = h.address  # type: ignore[attr-defined]
         raw_address: str = h.raw_address  # type: ignore[attr-defined]
 
@@ -192,20 +199,19 @@
                         self._listeners[key] = added_listener
                         logging.info(f"listener added for {address} and args {args} for client@{remote_address}")
                     else:
                         logging.info(f"start listen called for {address} and args {args}, but no listener was added.")
                 else:
                     logging.info(
                         f"listener already existing for {address} and args {args} for client@{remote_address}, "
-                        f"will not add unless sending a specific callback query param trailing (|Nil|QueryId"
+                        f"will not add unless sending a specific callback query param trailing (|Nil|QueryId",
                     )
-            elif stop:
-                if key in self._listeners:
-                    self._listeners[key]()
-                    logging.info(f"listener stopped for {address} and args {args} for client@{remote_address}")
+            elif stop and key in self._listeners:
+                self._listeners[key]()
+                logging.info(f"listener stopped for {address} and args {args} for client@{remote_address}")
 
             # this will also send a message on every start / stop request
             self._dispatcher.send(
                 address=f"{self._namespace}{address}",
                 remote_addr=remote_address,
                 params=h(args, remote_address),
                 include_base_address=True,
@@ -242,15 +248,15 @@
     def clear_listeners(self) -> None:
         pass
         # for listener in self._listeners:
         # call listener()
         #     if self._song.tempo_has_listener(listener):
         #         self._song.remove_tempo_listener(listener)
 
-    def __init__(self, *, dispatcher: Dispatcher, namespace: str):
+    def __init__(self, *, dispatcher: Dispatcher, namespace: str) -> None:
         self._dispatcher = dispatcher
         if not namespace.startswith("/"):
             namespace = f"/{namespace}"
         self._namespace = namespace
         self._logger = self._dispatcher._logger
         self._listeners = {}
         self._routers = []
```

### Comparing `fastosc-0.0.2/src/fastosc/server/server_base.py` & `fastosc-0.0.3/src/fastosc/server/server_base.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 
 from fastosc.message.arg_value import ArgValue
 from fastosc.message.convert import convert_message
 from fastosc.message.osc_message_builder import BuildError
 
 
 class OSCServerBase(ABC):
-    def __init__(self, logger: logging.Logger, local_addr: tuple[str, int]):
+    def __init__(self, logger: logging.Logger, local_addr: tuple[str, int]) -> None:
         self._logger = logger
         self._local_addr = local_addr
         self._logger.info("Starting OSC server (local %s)", str(self._local_addr))
 
     @abstractmethod
     def _send_bytes(self, data: bytes, remote_addr: tuple[str, int]) -> None:
         pass
 
     def send(self, *, address: str, params: list[ArgValue], remote_addr: tuple[str, int]) -> None:
         try:
             self._send_bytes(data=convert_message(address=address, params=params), remote_addr=remote_addr)
         except BuildError:
-            self._logger.error("OSC build error: %s" % (traceback.format_exc()))
+            self._logger.error(f"OSC build error: {traceback.format_exc()}")
```

### Comparing `fastosc-0.0.2/src/fastosc/server/udp/udp_pull_server.py` & `fastosc-0.0.3/src/fastosc/server/udp/udp_pull_server.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     This is more efficient in certain environments such as Ableton live embedded python which
     does not support multithreading well (i.e it gives latencies in 100+ms and cannot handle high rates of inbound
     messages without spiking latency.
     """
 
     def __init__(self, *, dispatcher: Dispatcher, logger: logging.Logger, local_addr: tuple[str, int]) -> None:
         super().__init__(logger=logger, dispatcher=dispatcher, local_addr=local_addr)
-        self._socket.setblocking(False)
+        self._socket.setblocking(False)  # noqa: FBT003
 
     def process(self) -> None:
         """
         Synchronously process all data queued on the OSC socket.
         """
         try:
             while True:
@@ -30,29 +30,29 @@
                 self._parse_datagram(data=data, remote_addr=remote_addr)
 
         except OSError as e:
             if e.errno == errno.ECONNRESET:
                 # --------------------------------------------------------------------------------
                 # This benign error seems to occur on startup on Windows
                 # --------------------------------------------------------------------------------
-                self._logger.warning("Non-fatal socket error: %s" % (traceback.format_exc()))
+                self._logger.warning(f"Non-fatal socket error: {traceback.format_exc()}")
             elif e.errno in (errno.EAGAIN, errno.EWOULDBLOCK):
                 # --------------------------------------------------------------------------------
                 # Another benign networking error, throw when no data is received
                 # on a call to recvfrom() on a non-blocking socket
                 # --------------------------------------------------------------------------------
                 pass
             else:
                 # --------------------------------------------------------------------------------
                 # Something more serious has happened
                 # --------------------------------------------------------------------------------
-                self._logger.error("Socket error: %s" % (traceback.format_exc()))
+                self._logger.error(f"Socket error: {traceback.format_exc()}")
 
-        except Exception as e:
-            self._logger.error("Error handling OSC message: %s" % e)
-            self._logger.warning("%s" % traceback.format_exc())
+        except Exception as e:  # noqa
+            self._logger.error(f"Error handling OSC message: {e}")
+            self._logger.warning(f"{traceback.format_exc()}")
 
     def shutdown(self) -> None:
         """
         Shutdown the server network sockets.
         """
         self._socket.close()
```

### Comparing `fastosc-0.0.2/src/fastosc/server/udp/udp_server_base.py` & `fastosc-0.0.3/src/fastosc/server/udp/udp_server_base.py`

 * *Files identical despite different names*

### Comparing `fastosc-0.0.2/src/fastosc.egg-info/PKG-INFO` & `fastosc-0.0.3/src/fastosc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastosc
-Version: 0.0.2
+Version: 0.0.3
 Summary: Modern Python Library for OSC, using best practices such as typing, linting/formatting - inspired by FastAPI
 Author-email: Martin Sahlen <martin8900@gmail.com>
 Project-URL: Homepage, https://github.com/oslo1989/fastosc
 Project-URL: Issues, https://github.com/oslo1989/fastosc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fastosc-0.0.2/src/fastosc.egg-info/SOURCES.txt` & `fastosc-0.0.3/src/fastosc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

