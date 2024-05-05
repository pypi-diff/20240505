# Comparing `tmp/err_aprs_backend-0.3.0.tar.gz` & `tmp/err_aprs_backend-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "err_aprs_backend-0.3.0.tar", max compression
+gzip compressed data, was "err_aprs_backend-0.4.0.tar", max compression
```

## Comparing `err_aprs_backend-0.3.0.tar` & `err_aprs_backend-0.4.0.tar`

### file list

```diff
@@ -1,25 +1,30 @@
--rw-r--r--   0        0        0     1063 2024-04-28 05:59:29.858011 err_aprs_backend-0.3.0/LICENSE
--rw-r--r--   0        0        0     4600 2024-04-28 05:59:29.858011 err_aprs_backend-0.3.0/README.md
--rw-r--r--   0        0        0      105 2024-04-28 05:59:29.858011 err_aprs_backend-0.3.0/aprs_backend/__init__.py
--rw-r--r--   0        0        0       81 2024-04-28 05:59:29.858011 err_aprs_backend-0.3.0/aprs_backend/aprs.plug
--rw-r--r--   0        0        0    17599 2024-04-28 05:59:29.858011 err_aprs_backend-0.3.0/aprs_backend/aprs.py
--rw-r--r--   0        0        0      212 2024-04-28 05:59:29.858011 err_aprs_backend-0.3.0/aprs_backend/clients/__init__.py
--rw-r--r--   0        0        0     2719 2024-04-28 05:59:29.858011 err_aprs_backend-0.3.0/aprs_backend/clients/aprs_registry.py
--rw-r--r--   0        0        0     5374 2024-04-28 05:59:29.858011 err_aprs_backend-0.3.0/aprs_backend/clients/aprsis.py
--rw-r--r--   0        0        0       82 2024-04-28 05:59:29.858011 err_aprs_backend-0.3.0/aprs_backend/clients/kiss.py
--rw-r--r--   0        0        0       48 2024-04-28 05:59:29.858011 err_aprs_backend-0.3.0/aprs_backend/exceptions/__init__.py
--rw-r--r--   0        0        0      153 2024-04-28 05:59:29.862011 err_aprs_backend-0.3.0/aprs_backend/exceptions/client/__init__.py
--rw-r--r--   0        0        0      311 2024-04-28 05:59:29.862011 err_aprs_backend-0.3.0/aprs_backend/exceptions/client/aprsis.py
--rw-r--r--   0        0        0      113 2024-04-28 05:59:29.862011 err_aprs_backend-0.3.0/aprs_backend/exceptions/packets/__init__.py
--rw-r--r--   0        0        0      112 2024-04-28 05:59:29.862011 err_aprs_backend-0.3.0/aprs_backend/exceptions/packets/parser.py
--rw-r--r--   0        0        0      744 2024-04-28 05:59:29.862011 err_aprs_backend-0.3.0/aprs_backend/message.py
--rw-r--r--   0        0        0     5372 2024-04-28 05:59:29.862011 err_aprs_backend-0.3.0/aprs_backend/packets/__init__.py
--rw-r--r--   0        0        0     9997 2024-04-28 05:59:29.862011 err_aprs_backend-0.3.0/aprs_backend/packets/parser.py
--rw-r--r--   0        0        0     1038 2024-04-28 05:59:29.862011 err_aprs_backend-0.3.0/aprs_backend/person.py
--rw-r--r--   0        0        0       83 2024-04-28 05:59:29.862011 err_aprs_backend-0.3.0/aprs_backend/room.py
--rw-r--r--   0        0        0      495 2024-04-28 05:59:29.862011 err_aprs_backend-0.3.0/aprs_backend/utils/__init__.py
--rw-r--r--   0        0        0      975 2024-04-28 05:59:29.862011 err_aprs_backend-0.3.0/aprs_backend/utils/counter.py
--rw-r--r--   0        0        0       26 2024-04-28 05:59:29.862011 err_aprs_backend-0.3.0/aprs_backend/utils/version.py
--rw-r--r--   0        0        0       22 2024-04-28 05:59:29.862011 err_aprs_backend-0.3.0/aprs_backend/version.py
--rw-r--r--   0        0        0     1412 2024-04-28 05:59:29.862011 err_aprs_backend-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5272 1970-01-01 00:00:00.000000 err_aprs_backend-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-05 15:58:45.130718 err_aprs_backend-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4600 2024-05-05 15:58:45.130718 err_aprs_backend-0.4.0/README.md
+-rw-r--r--   0        0        0      105 2024-05-05 15:58:45.130718 err_aprs_backend-0.4.0/aprs_backend/__init__.py
+-rw-r--r--   0        0        0       81 2024-05-05 15:58:45.130718 err_aprs_backend-0.4.0/aprs_backend/aprs.plug
+-rw-r--r--   0        0        0    20931 2024-05-05 15:58:45.130718 err_aprs_backend-0.4.0/aprs_backend/aprs.py
+-rw-r--r--   0        0        0      212 2024-05-05 15:58:45.130718 err_aprs_backend-0.4.0/aprs_backend/clients/__init__.py
+-rw-r--r--   0        0        0      959 2024-05-05 15:58:45.130718 err_aprs_backend-0.4.0/aprs_backend/clients/_base.py
+-rw-r--r--   0        0        0     2174 2024-05-05 15:58:45.130718 err_aprs_backend-0.4.0/aprs_backend/clients/aprs_registry.py
+-rw-r--r--   0        0        0     6945 2024-05-05 15:58:45.130718 err_aprs_backend-0.4.0/aprs_backend/clients/aprsis.py
+-rw-r--r--   0        0        0     1560 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/clients/beacon.py
+-rw-r--r--   0        0        0       82 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/clients/kiss.py
+-rw-r--r--   0        0        0      562 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/exceptions/__init__.py
+-rw-r--r--   0        0        0       48 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/exceptions/base.py
+-rw-r--r--   0        0        0      158 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/exceptions/client/__init__.py
+-rw-r--r--   0        0        0      396 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/exceptions/client/aprsis.py
+-rw-r--r--   0        0        0      118 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/exceptions/packets/__init__.py
+-rw-r--r--   0        0        0      112 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/exceptions/packets/parser.py
+-rw-r--r--   0        0        0      117 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/exceptions/processor.py
+-rw-r--r--   0        0        0      744 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/message.py
+-rw-r--r--   0        0        0     9038 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/packets/__init__.py
+-rw-r--r--   0        0        0    10116 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/packets/parser.py
+-rw-r--r--   0        0        0     1038 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/person.py
+-rw-r--r--   0        0        0       83 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/room.py
+-rw-r--r--   0        0        0      495 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/utils/__init__.py
+-rw-r--r--   0        0        0      975 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/utils/counter.py
+-rw-r--r--   0        0        0      118 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/utils/datetime.py
+-rw-r--r--   0        0        0      565 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/utils/position.py
+-rw-r--r--   0        0        0       22 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/aprs_backend/version.py
+-rw-r--r--   0        0        0     1412 2024-05-05 15:58:45.134718 err_aprs_backend-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5272 1970-01-01 00:00:00.000000 err_aprs_backend-0.4.0/PKG-INFO
```

### Comparing `err_aprs_backend-0.3.0/LICENSE` & `err_aprs_backend-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.3.0/README.md` & `err_aprs_backend-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.3.0/aprs_backend/aprs.py` & `err_aprs_backend-0.4.0/aprs_backend/aprs.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,80 +4,85 @@
 from aprs_backend.clients import APRSISClient
 from aprs_backend.person import APRSPerson
 from aprs_backend.room import APRSRoom
 from aprs_backend.version import __version__ as ERR_APRS_VERSION
 from errbot.backends.base import Message
 from errbot.backends.base import ONLINE
 from errbot.core import ErrBot
-from aprs_backend.exceptions.client.aprsis import APRSISConnnectError
-from aprs_backend.exceptions.packets.parser import PacketParseError
-from aprs_backend.exceptions import APRSBackendException
+from aprs_backend.exceptions import ProcessorError, PacketParseError, APRSISConnnectError
 from aprs_backend.packets.parser import parse, hash_packet
 from expiringdict import ExpiringDict
 from functools import cached_property
-from aprs_backend.packets import AckPacket, RejectPacket, MessagePacket
+from aprs_backend.packets import AckPacket, RejectPacket, MessagePacket, BeaconPacket
 from aprs_backend.utils.counter import MessageCounter
 from random import randint
 from datetime import datetime
 from better_profanity import profanity
 from aprs_backend.clients.aprs_registry import APRSRegistryClient, RegistryAppConfig
 import logging
 import asyncio
 from errbot.version import VERSION as ERR_VERSION
-
+from aprs_backend.clients.beacon import BeaconConfig, BeaconClient
 
 log = logging.getLogger(__name__)
 
 for handler in log.handlers:
     handler.setFormatter(
         logging.Formatter("%(filename)s: " "%(levelname)s: " "%(funcName)s(): " "%(lineno)d:\t" "%(message)s")
     )
 
 
-class ProcessorError(APRSBackendException):
-    pass
-
-
 class APRSBackend(ErrBot):
     def __init__(self, config):
         log.debug("Initied")
 
         self._errbot_config = config
+        self._multiline = False
+
         aprs_config = {"host": "rotate.aprs.net", "port": 14580}
         aprs_config.update(config.BOT_IDENTITY)
+        aprs_config["aprs_app_name"] = "ErrbotAPRS"
+        aprs_config["app_version"] = f"{ERR_APRS_VERSION}:{ERR_VERSION}"
 
         self._sender_config = {}
 
         if "callsign" not in aprs_config:
             log.fatal("No callsign in bot identity")
             sys.exit(1)
         if "password" not in aprs_config:
             log.fatal("No password in bot identity")
             sys.exit(1)
 
-        self.callsign = aprs_config["callsign"]
-        self.from_call = getattr(self._errbot_config, "APRS_FROM_CALLSIGN", self.callsign)
-        self.listened_callsigns = getattr(self._errbot_config, "APRS_LISTENED_CALLSIGNS", ())
+        self.listening_callsigns = [aprs_config["callsign"]]
+
+        self.callsign = self._get_from_config("APRS_BOT_CALLSIGN", aprs_config["callsign"])
         self.bot_identifier = APRSPerson(self.callsign)
-        self._multiline = False
+        if self.callsign != aprs_config["callsign"]:
+            # bot is using a different callsign from the signin, add it to the filter
+            aprs_config["aprs_filter"] = f"g/{aprs_config['callsign']}/{self.callsign}"
+            self.listening_callsigns.append(self.callsign)
         self._client = APRSISClient(**aprs_config, logger=log)
-        self._send_queue = asyncio.Queue(maxsize=int(getattr(self._errbot_config, "APRS_SEND_MAX_QUEUE", "2048")))
-        self.help_text = getattr(self._errbot_config, "APRS_HELP_TEXT", "APRSBot,Errbot & err-aprs-backend")
+        self._send_queue: asyncio.Queue[MessagePacket] = asyncio.Queue(
+            maxsize=int(self._get_from_config("APRS_SEND_MAX_QUEUE", "2048"))
+        )
+        self.help_text = self._get_from_config(
+            "APRS_HELP_TEXT", f"Errbot {ERR_VERSION} & err-aprs-backend {ERR_APRS_VERSION} by {aprs_config['callsign']}"
+        )
 
         self._message_counter = MessageCounter(initial_value=randint(1, 20))  # nosec not used cryptographically
         self._max_dropped_packets = int(self._get_from_config("APRS_MAX_DROPPED_PACKETS", "25"))
         self._max_cached_packets = int(self._get_from_config("APRS_MAX_CACHED_PACKETS", "2048"))
         self._message_max_retry = int(self._get_from_config("APRS_MESSAGE_MAX_RETRIES", "7"))
         self._message_retry_wait = int(self._get_from_config("APRS_MESSAGE_RETRY_WAIT", "90"))
 
         # strip newlines out of plugin responses before sending to aprs, probably best to leave it true, nothing in aprs will handle
         # a stray newline
         self._strip_newlines = str(self._get_from_config("APRS_STRIP_NEWLINES", "true")).lower() == "true"
 
-        # try to strip out "foul" language the FCC would not like. It is possible/probably an errbot bot response could
+        # try to strip out "foul" language the FCC would not like. It is possible/probable an errbot bot response could
         # go out over the airwaves. This is configurable, but probably should remain on.
         self._language_filter = str(self._get_from_config("APRS_LANGUAGE_FILTER", "true")).lower() == "true"
         if self._language_filter:
             profanity.load_censor_words(self._get_from_config("APRS_LANGUAGE_FILTER_EXTRA_WORDS", []))
 
         self._max_age_cached_packets_seconds = int(self._get_from_config("APRS_MAX_AGE_CACHED_PACETS_SECONDS", "3600"))
         self._packet_cache = ExpiringDict(
@@ -90,15 +95,15 @@
         self._waiting_ack_lock = asyncio.Lock()
 
         self.registry_enabled = self._get_from_config("APRS_REGISTRY_ENABLED", "false").lower() == "true"
         if self.registry_enabled:
             self.registry_app_config = RegistryAppConfig(
                 description=self._get_from_config("APRS_REGISTRY_DESCRIPTION", "err-aprs-backend powered bot"),
                 website=self._get_from_config("APRS_REGISTRY_WEBSITE", ""),
-                listening_callsigns=[self.from_call] + [call for call in self.listened_callsigns],
+                listening_callsigns=self.listening_callsigns,
                 software=self._get_from_config(
                     "APRS_REGISTRY_SOFTWARE", f"err-aprs-backend {ERR_APRS_VERSION} errbot {ERR_VERSION}"
                 ),
             )
             if (registry_software := self._get_from_config("APRS_REGISTRY_SOFTWARE", None)) is not None:
                 self.registry_app_config.software = registry_software
             self.registry_client = APRSRegistryClient(
@@ -106,19 +111,56 @@
                 log=log,
                 frequency_seconds=int(self._get_from_config("APRS_REGISTRY_FREQUENCY_SECONDS", "3600")),
                 app_config=self.registry_app_config,
             )
         else:
             self.registry_client = None
 
+        self.beacon_config = self._get_beacon_config()
+        if self.beacon_config:
+            self.beacon_client = BeaconClient(
+                beacon_config=self.beacon_config,
+                send_queue=self._send_queue,
+                log=log,
+                frequency_seconds=int(self._get_from_config("APRS_BEACON_INTERVAL_SECONDS", "1200")),
+            )
+        else:
+            self.beacon_client = None
         super().__init__(config)
 
     def _get_from_config(self, key: str, default: any = None) -> any:
         return getattr(self._errbot_config, key, default)
 
+    def _get_beacon_config(self) -> BeaconConfig | None:
+        if self._get_from_config("APRS_BEACON_ENABLE", "false") == "true":
+            return None
+        beacon_config = {}
+        beacon_config["latitude"] = self._get_from_config("APRS_BEACON_LATITUDE", None)
+        beacon_config["longitude"] = self._get_from_config("APRS_BEACON_LONGITUDE", None)
+        beacon_config["symbol"] = self._get_from_config("APRS_BEACON_SYMBOL", None)
+        beacon_config["symbol_table"] = self._get_from_config("APRS_BEACON_SYMBOL_TABLE", None)
+        log.debug("Beacon Config %s", beacon_config)
+        for key, value in beacon_config.items():
+            if value is None:
+                log.error(f"Beacon enabled but APRS_BEACON_{key.upper()} not set. Disabling Beacon.")
+                return None
+
+        for key in ["latitude", "longitude"]:
+            try:
+                beacon_config[key] = float(beacon_config[key])
+            except ValueError:
+                log.error("%s is not a valid float in config. Disabling beacon", key)
+                return None
+
+        for key in ["altitude", "comment"]:
+            if (value := self._get_from_config(f"APRS_BEACON_{key.upper()}", None)) is not None:
+                beacon_config[key] = value
+
+        return BeaconConfig(**beacon_config, from_call=self.callsign)
+
     def build_reply(self, msg: Message, text: str, private: bool = False, threaded: bool = False) -> Message:
         log.debug(msg)
         reply = Message(
             body=text,
             to=msg.frm,
             frm=self.bot_identifier,
             extras={
@@ -169,44 +211,56 @@
 
                 # check max retries first, its cheaper than a timedelta
                 if this_packet.last_send_attempt > self._message_max_retry:
                     log.debug("Packet %s over max retries, dropping %s", key, this_packet.json)
                     await self.__drop_message_from_waiting(key)
                     continue
 
-                # if this packet has not been sent in self._message_retry_wait seconds, resent it
-                # it hasn't been ack'd yet
+                # if this packet has not been sent in self._message_retry_wait seconds, resend it
+                # because it hasn't been ack'd yet
                 if (datetime.now() - this_packet.last_send_time).total_seconds() > self._message_retry_wait:
                     log.debug("Message %s needs to be re-sent %s", key, this_packet.json)
                     self.send_message(APRSMessage.from_message_packet(this_packet))
                 # release the loop for a bit
-                await asyncio.sleep(0.01)
+                await asyncio.sleep(0.001)
             # release the loop for a bit longer after we've gone through all keys
-            await asyncio.sleep(0.1)
+            await asyncio.sleep(5)
 
     async def send_worker(self) -> None:
         """Processes self._send_queue to send messages to APRS"""
         log.debug("send_worker started")
         while True:
             try:
-                packet = self._send_queue.get_nowait()
+                packet: MessagePacket | BeaconPacket = self._send_queue.get_nowait()
             except asyncio.QueueEmpty:
                 packet = None
             if packet is not None:
                 log.debug("send_worker got Packet %s", packet.json)
                 await packet.prepare(self._message_counter)
                 packet.update_timestamp()
-                await self._client._send(packet.raw)
-                packet.last_send_time = datetime.now()
-                packet.last_send_attempt += 1
-                async with self._waiting_ack_lock:
-                    self._waiting_ack[hash_packet(packet)] = packet
+                result = await self._client._send(packet.raw)
+                if result:
+                    # send was a success
+                    # if this is a message, add it to _waiting_ack
+                    if isinstance(packet, MessagePacket):
+                        packet.last_send_time = datetime.now()
+                        packet.last_send_attempt += 1
+                        async with self._waiting_ack_lock:
+                            self._waiting_ack[f"{packet.to}-{packet.msgNo}"] = packet
+                else:
+                    # sending failed
+                    log.info("Packet sending failed, waiting 1 second then requeing packet %s", packet)
+                    for _ in range(10):
+                        # microsleeps to let this be more cancellable
+                        await asyncio.sleep(0.1)
+                    await self._send_queue.put(packet)
+
                 self._send_queue.task_done()
             # release the loop for a bit
-            await asyncio.sleep(0.01)
+            await asyncio.sleep(0.001)
 
     async def receive_worker(self) -> bool:
         """_summary_"""
         log.debug("Receive worker started")
         try:
             await self._client.connect()
         except APRSISConnnectError as exc:
@@ -217,29 +271,30 @@
         try:
             while True:
                 packet_str = await self._client.get_packet()
                 # check if this is just a status keepalive from the aprs server
                 # or connetion replies info.
                 # They all startwith "# "
                 if packet_str.startswith("# "):
-                    log.debug("Status message from aprs server: %s", packet_str)
+                    log.debug("Status message from aprs server: %s", packet_str.rstrip("\r\n"))
                     continue
                 try:
                     parsed_packet = parse(packet_str)
-                    # release the loop for a bit
-                    await asyncio.sleep(0.01)
+                    # release the loop for a tiny bit
+                    await asyncio.sleep(0.001)
                     if parsed_packet is not None:
-                        if parsed_packet.to == self.callsign or parsed_packet.to in self.listened_callsigns:
+                        # filtering should handle this, but belt and syspenders
+                        if parsed_packet.to in self.listening_callsigns:
                             await self.process_packet(parsed_packet)
                         else:
                             log.info(
-                                "Packet was not addressed to bot or listened callsigns, not processing %s", packet_str
+                                "Packet was not addressed to the bot, not processing %s", packet_str.rstrip("\r\n")
                             )
                     else:
-                        log.info("This packet parsed to be None: %s", packet_str)
+                        log.info("This packet parsed to be None: %s", packet_str.rstrip("\r\n"))
                 except PacketParseError as exc:
                     log.error(
                         "Dropping packet %s due to Parsing error: %s. Total Dropped Packets: %s",
                         packet_str,
                         exc,
                         self._dropped_packets,
                     )
@@ -264,14 +319,16 @@
     async def async_serve_once(self) -> bool:
         receive_task = asyncio.create_task(self.receive_worker())
 
         worker_tasks = [asyncio.create_task(self.send_worker()), asyncio.create_task(self.retry_worker())]
         # if reporting to the aprs service registry is enabled, start a task for it
         if self.registry_client is not None:
             worker_tasks.append(asyncio.create_task(self.registry_client()))
+        if self.beacon_client is not None:
+            worker_tasks.append(asyncio.create_task(self.beacon_client()))
         result = await asyncio.gather(receive_task, return_exceptions=True)
         await self._send_queue.join()
         for task in worker_tasks:
             task.cancel()
         return result
 
     def serve_once(self) -> bool:
@@ -304,27 +361,27 @@
         last_send_attempt = 0
         if "packet" in msg.extras:
             msgNo = getattr(msg.extras["packet"], "msgNo", None)
             last_send_attempt = getattr(msg.extras["packet"], "last_send_attempt", 0)
         if msgNo is None:
             msgNo = self._message_counter.get_value_sync()
         msg_packet = MessagePacket(
-            from_call=self.from_call,
+            from_call=msg.frm.callsign,
             to_call=msg.to.callsign,
             addresse=msg.to.callsign,
             message_text=msg_text,
             msgNo=msgNo,
             last_send_attempt=last_send_attempt,
         )
         msg_packet._build_raw()
         try:
             self._send_queue.put_nowait(msg_packet)
             log.debug("Packet %s put in send queue", msg_packet.json)
         except asyncio.QueueFull:
-            log.error("Send queue is full, can't send msg %s", msg)
+            log.error("Send queue is full, can't send packet %s", msg_packet.json)
             self._dropped_packets += 1
 
     @property
     def mode(self) -> str:
         return "aprs"
 
     @cached_property
@@ -344,35 +401,40 @@
     async def process_packet(self, packet: AckPacket | RejectPacket | MessagePacket) -> None:
         log.debug("Processing packet %s", packet.json)
         if isinstance(packet, MessagePacket):
             await self._process_message(packet)
         elif isinstance(packet, AckPacket) or isinstance(packet, RejectPacket):
             await self._process_ack_rej(packet)
 
-    async def _process_ack_rej(self, packet: dict[str, str | bool]) -> None:
+    async def _process_ack_rej(self, packet: AckPacket | RejectPacket) -> None:
         """
         Process an ack or reject packet by checking if its in the messages
         waiting for an ack and if so, remove it the message
         """
         # Remove this message from our sent messages that are waiting for acks
-        await self.__drop_message_from_waiting(hash_packet(packet))
+        log.debug(
+            "Processing ACK/REJ packet for msgno %s from %s to %s", packet.msgNo, packet.from_call, packet.addresse
+        )
+        await self.__drop_message_from_waiting(f"{packet.from_call}-{packet.msgNo}")
 
     async def __drop_message_from_waiting(self, message_hash: str) -> None:
         """Gets the waiting_ack_lock and deletes a message from _waiting_ack if it exists"""
+        log.debug("Dropping message hash %s", message_hash)
         async with self._waiting_ack_lock:
-            try:
-                self._waiting_ack.pop(message_hash)
-            except KeyError:
-                pass
+            packet = self._waiting_ack.pop(message_hash)
+        if packet is None:
+            log.error("Tried to drop hash %s and it didn't exist in waiting ack", message_hash)
+        else:
+            log.debug("Dropped Packet from waiting_ack: %s", packet)
 
     def handle_help(self, msg: APRSMessage) -> None:
         """Returns simplified help text for the APRS backend"""
         help_msg = APRSMessage(body=self.help_text, extras=msg.extras)
         help_msg.to = msg.frm
-        help_msg.frm = APRSPerson(callsign=self.from_call)
+        help_msg.frm = self.bot_identifier
         self.send_message(help_msg)
 
     async def _process_message(self, packet: MessagePacket) -> None:
         """
         Check if this message is a dupe of one the bot is already processing
         (waiting for an ack), and dispatch it to plugins
         """
@@ -382,20 +444,21 @@
         this_packet_hash = hash_packet(packet)
         async with self._packet_cache_lock:
             if self._packet_cache.get(this_packet_hash, None) is not None:
                 log.info("Duplicate packet %s. Skipping processing", packet.json)
                 return
             self._packet_cache[this_packet_hash] = packet
         msg = APRSMessage.from_message_packet(packet)
-        if msg.body.lower().strip(" ").strip("\n").strip("\r") == "help":
+        msg.body = msg.body.strip("\n").strip("\r")
+        if msg.body.lower().strip(" ") == "help":
             return self.handle_help(msg)
         return self.callback_message(msg)
 
     async def _ack_message(self, packet: MessagePacket) -> None:
         log.debug("Sending ack for packet %s", packet.json)
         this_ack = AckPacket(
-            from_call=self.from_call, to_call=packet.from_call, addresse=packet.from_call, msgNo=packet.msgNo
+            from_call=packet.to, to_call=packet.from_call, addresse=packet.from_call, msgNo=packet.msgNo
         )
         await this_ack.prepare(self._message_counter)
         this_ack.update_timestamp()
         await self._client._send(this_ack.raw)
         return
```

### Comparing `err_aprs_backend-0.3.0/aprs_backend/clients/aprs_registry.py` & `err_aprs_backend-0.4.0/aprs_backend/clients/aprs_registry.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dataclasses import dataclass
 import httpx
 from functools import cached_property
-import asyncio
+from aprs_backend.clients._base import ClientBase
+from logging import Logger
 
 
 @dataclass
 class RegistryAppConfig:
     description: str
     listening_callsigns: list[str]
     website: str = ""
@@ -20,50 +21,41 @@
                 "service_website": self.website,
                 "software": self.software,
             }
             for this_call in self.listening_callsigns
         ]
 
 
-class APRSRegistryClient:
-    def __init__(self, registry_url: str, app_config: RegistryAppConfig, log, frequency_seconds: int = 3600) -> None:
+class APRSRegistryClient(ClientBase):
+    def __init__(
+        self, registry_url: str, app_config: RegistryAppConfig, log: Logger, frequency_seconds: int = 3600
+    ) -> None:
         self.registry_url = registry_url
-        self.log = log
-        self.frequency_seconds = frequency_seconds
         self.app_config = app_config
+        super().__init__(log=log, frequency_seconds=frequency_seconds)
 
-    async def __call__(self) -> None:
+    async def __process__(self) -> None:
         """Posts to the aprs registry url for each listening callsign for the bot
-        Run as an asyncio task
+        Run as an asyncio task in __call__
         """
-        self.log.debug("Staring APRS Registry Client")
-        try:
-            while True:
-                async with httpx.AsyncClient() as client:
-                    for post_json in self.app_config.post_jsons:
-                        self.log.debug("Posting %s to %s", post_json, self.registry_url)
-                        try:
-                            response = await client.post(self.registry_url, json=post_json)
-                            self.log.debug(response)
-                            response.raise_for_status()
-                        except httpx.RequestError as exc:
-                            self.log.error(
-                                "Request Error while posting %s to %s. Error: %s, response: %s",
-                                post_json,
-                                self.registry_url,
-                                exc,
-                                response,
-                            )
-                        except httpx.HTTPStatusError as exc:
-                            self.log.error(
-                                "Error while posting %s to %s. Error: %s, response: %s",
-                                post_json,
-                                self.registry_url,
-                                exc,
-                                response,
-                            )
-                # instead of sleeping in one big chunk, sleep in smaller chunks for easier cacnellation
-                for i in range(self.frequency_seconds * 10):
-                    await asyncio.sleep(0.1)
-        except asyncio.CancelledError:
-            self.log.info("APRS client cancelled, stopping")
-            return
+        async with httpx.AsyncClient() as client:
+            for post_json in self.app_config.post_jsons:
+                self.log.debug("Posting %s to %s", post_json, self.registry_url)
+                try:
+                    response = await client.post(self.registry_url, json=post_json)
+                    self.log.debug(response)
+                    response.raise_for_status()
+                except httpx.RequestError as exc:
+                    self.log.error(
+                        "Request Error while posting %s to %s. Error: %s",
+                        post_json,
+                        self.registry_url,
+                        exc,
+                    )
+                except httpx.HTTPStatusError as exc:
+                    self.log.error(
+                        "Error while posting %s to %s. Error: %s, response: %s",
+                        post_json,
+                        self.registry_url,
+                        exc,
+                        response,
+                    )
```

### Comparing `err_aprs_backend-0.3.0/aprs_backend/clients/aprsis.py` & `err_aprs_backend-0.4.0/aprs_backend/clients/aprsis.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 import asyncio
 from functools import cached_property
 import time
-from aprs_backend.exceptions.client.aprsis import (
+from aprs_backend.exceptions import (
     APRSISClientError,
     APRSISConnnectError,
+    APRSISLoginError,
     APRSISPacketError,
     APRSISDeadConnectionError,
     APRSISPacketDecodeError,
 )
 
 
 class APRSISClient:
@@ -29,41 +30,77 @@
         self.aprs_host = host
         self.aprs_port = port
         self.aprs_filter = aprs_filter
         self._aprs_app_name = aprs_app_name
         self._app_version = app_version
         self._keepalive_seconds = keepalive_seconds
 
-        if self.aprs_filter.lower() == "default":
-            self.aprs_filter = f"g/{self.callsign}"
-
         self._log = logger if logger is not None else logging.getLogger(__name__)
 
         self.connected = False
         self.__connect_count = 0
         self.__packet_count = 0
         self._writer = None
         self._reader = None
         self._keepalive_last_sent = 0
         self._last_successful_connect = 0
 
     @cached_property
     def _aprs_login(self) -> bytes:
-        return f"user {self.callsign} pass {self.password} vers {self._aprs_app_name} {self._app_version} filter {self.aprs_filter}\n"
+        base_str = f"user {self.callsign} pass {self.password} vers {self._aprs_app_name} {self._app_version}"
+        if self.aprs_filter.lower() != "default":
+            base_str = base_str + f" filter {self.aprs_filter}\r\n"
+        return base_str
+
+    async def _send_login(self):
+        """
+        Sends login string to server
+        """
+
+        self._log.info("Sending login information")
+        try:
+            await self._send(self._aprs_login)
+            aprs_version = await self._reader.readline()
+            aprs_version = aprs_version.decode("latin-1").rstrip()
+            aprs_login_test = await self._reader.readline()
+            aprs_login_test = aprs_login_test.decode("latin-1").rstrip()
+            self._log.debug("APRS server version Response %s", aprs_version)
+            _, _, callsign, status, _, server = aprs_login_test.split(" ", 5)
+            status = status.replace(",", "").lower()
+
+            if callsign == "":
+                raise APRSISLoginError("Server responded with empty callsign???")
+            if callsign != self.callsign:
+                raise APRSISLoginError("Server responsed with: %s" % aprs_login_test)
+            if status != "verified" and self.password != "-1":  # nosec not a hardcoded password
+                raise APRSISLoginError("Password is incorrect")
+
+            if self.password == "-1":  # nosec not a hardcoded password
+                self._log.info("Login successful (receive only)")
+            else:
+                self._log.info("Login successful")
+        except APRSISLoginError as e:
+            self._log.error(str(e))
+            await self.disconnect()
+            raise
+        except Exception as exc:
+            await self.disconnect()
+            self._log.error("Failed to login %s", str(exc))
+            raise APRSISLoginError("Failed to login") from exc
 
     @cached_property
     def _keepalive_packet(self) -> bytes:
         return b"#keepalive\n"
 
     async def connect(self) -> None:
         self.__connect_count += 1
         try:
             self._reader, self._writer = await asyncio.open_connection(self.aprs_host, self.aprs_port)
             # login to aprsis
-            await self._send(self._aprs_login)
+            await self._send_login()
             self._last_successful_connect = time.perf_counter()
             self._log.info(
                 "Connected to %s/%s:%s as %s with filter %s",
                 self.aprs_host,
                 self._get_sock_peer_ip(self._writer),
                 self.aprs_port,
                 self.callsign,
@@ -74,33 +111,33 @@
             self._log.error("Error while connecting: %s", exc)
             self.connected = False
             raise APRSISConnnectError from exc
 
     async def disconnect(self):
         self._log.info("Disconnecting from aprsis")
         self._writer.close()
-        self._reader.close()
         await self._writer.wait_closed()
-        await self._reader.wait_closed()
         self._writer = None
         self._reader = None
         self.connected = False
         self._log.info("Disconnected")
 
-    async def _send(self, packet: str, encoding: str = "utf-8") -> None:
+    async def _send(self, packet: str, encoding: str = "utf-8") -> bool:
         self._log.debug("Sending '%s'", packet)
         packet = packet.rstrip("\r\n") + "\r\n"
         if packet is None:
             self._log.error("Packet is None - %s - Dropping", packet)
-            return
+            return False
         if self._writer is not None:
             self._writer.write(packet.encode(encoding))
             await self._writer.drain()
+            return True
         else:
-            self._log.error("Disconnected, unable to send packet %s, dropped", packet)
+            # disconnected, not able to send packet yet
+            return False
 
     async def _send_keepalive(self) -> bool:
         """
         Send KeepAlive packet if necessary. _writer must be connected.
         :return Whether or not one was sent.
         """
         now = time.perf_counter()
```

### Comparing `err_aprs_backend-0.3.0/aprs_backend/message.py` & `err_aprs_backend-0.4.0/aprs_backend/message.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.3.0/aprs_backend/packets/parser.py` & `err_aprs_backend-0.4.0/aprs_backend/packets/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,8 +246,11 @@
         case _:
             packet_type = "UNKNOWN"
     return packet_type
 
 
 @lru_cache(maxsize=128)
 def hash_packet(packet: AckPacket | MessagePacket | RejectPacket) -> str:
-    return sha256(f"{packet.to}-{packet.msgNo}-{packet.from_call}".encode()).hexdigest()
+    involved_stations = [packet.to, packet.addresse]
+    # alphabetize them for norming
+    involved_stations.sort()
+    return sha256((",".join(involved_stations) + f"-{packet.msgNo}").encode()).hexdigest()
```

### Comparing `err_aprs_backend-0.3.0/aprs_backend/person.py` & `err_aprs_backend-0.4.0/aprs_backend/person.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.3.0/aprs_backend/utils/counter.py` & `err_aprs_backend-0.4.0/aprs_backend/utils/counter.py`

 * *Files identical despite different names*

### Comparing `err_aprs_backend-0.3.0/pyproject.toml` & `err_aprs_backend-0.4.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "err-aprs-backend"
-version = "0.3.0"
+version = "0.4.0"
 description = "Errbot APRS backend plugin"
 authors = ["Andrew Herrington <andrew.the.techie@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "aprs_backend"}]
 include = ["*.plug"]
```

### Comparing `err_aprs_backend-0.3.0/PKG-INFO` & `err_aprs_backend-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: err-aprs-backend
-Version: 0.3.0
+Version: 0.4.0
 Summary: Errbot APRS backend plugin
 License: MIT
 Author: Andrew Herrington
 Author-email: andrew.the.techie@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

