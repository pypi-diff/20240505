# Comparing `tmp/reskyblock-0.2.3.tar.gz` & `tmp/reskyblock-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reskyblock-0.2.3.tar", last modified: Fri Apr 12 01:58:45 2024, max compression
+gzip compressed data, was "reskyblock-0.2.4.tar", last modified: Sun May  5 03:41:07 2024, max compression
```

## Comparing `reskyblock-0.2.3.tar` & `reskyblock-0.2.4.tar`

### file list

```diff
@@ -1,28 +1,30 @@
--rw-r--r--   0        0        0       13 2024-04-12 01:58:24.860889 reskyblock-0.2.3/README.md
--rw-r--r--   0        0        0     2689 2024-04-12 01:58:45.760933 reskyblock-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      282 2024-04-12 01:58:24.860889 reskyblock-0.2.3/src/reskyblock/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 01:58:24.860889 reskyblock-0.2.3/src/reskyblock/__main__.py
--rw-r--r--   0        0        0     4458 2024-04-12 01:58:24.860889 reskyblock-0.2.3/src/reskyblock/client.py
--rw-r--r--   0        0        0      212 2024-04-12 01:58:24.860889 reskyblock-0.2.3/src/reskyblock/http/__init__.py
--rw-r--r--   0        0        0     2129 2024-04-12 01:58:24.860889 reskyblock-0.2.3/src/reskyblock/http/http_adapter.py
--rw-r--r--   0        0        0      331 2024-04-12 01:58:24.860889 reskyblock-0.2.3/src/reskyblock/models/__init__.py
--rw-r--r--   0        0        0     1259 2024-04-12 01:58:24.860889 reskyblock-0.2.3/src/reskyblock/models/auctions.py
--rw-r--r--   0        0        0      625 2024-04-12 01:58:24.860889 reskyblock-0.2.3/src/reskyblock/models/auctions_ended.py
--rw-r--r--   0        0        0      716 2024-04-12 01:58:24.860889 reskyblock-0.2.3/src/reskyblock/models/bazaar.py
--rw-r--r--   0        0        0       73 2024-04-12 01:58:24.860889 reskyblock-0.2.3/src/reskyblock/nbt/__init__.py
--rw-r--r--   0        0        0     2541 2024-04-12 01:58:24.860889 reskyblock-0.2.3/src/reskyblock/nbt/decoder.py
--rw-r--r--   0        0        0        0 2024-04-12 01:58:24.860889 reskyblock-0.2.3/src/reskyblock/py.typed
--rw-r--r--   0        0        0      131 2024-04-12 01:58:24.860889 reskyblock-0.2.3/src/reskyblock/serialization/__init__.py
--rw-r--r--   0        0        0      992 2024-04-12 01:58:24.860889 reskyblock-0.2.3/src/reskyblock/serialization/json.py
--rw-r--r--   0        0        0      574 2024-04-12 01:58:24.860889 reskyblock-0.2.3/src/reskyblock/urls.py
--rw-r--r--   0        0        0        0 2024-04-12 01:58:24.860889 reskyblock-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0  2018239 2024-04-12 01:58:24.872889 reskyblock-0.2.3/tests/data/auctions.json
--rw-r--r--   0        0        0  2039142 2024-04-12 01:58:24.884889 reskyblock-0.2.3/tests/data/auctions2.json
--rw-r--r--   0        0        0   315276 2024-04-12 01:58:24.884889 reskyblock-0.2.3/tests/data/auctions_ended.json
--rw-r--r--   0        0        0  2264250 2024-04-12 01:58:24.892889 reskyblock-0.2.3/tests/data/bazaar.json
--rw-r--r--   0        0        0    89195 2024-04-12 01:58:24.892889 reskyblock-0.2.3/tests/data/item_bytes.txt
--rw-r--r--   0        0        0     3204 2024-04-12 01:58:24.892889 reskyblock-0.2.3/tests/test_client.py
--rw-r--r--   0        0        0      692 2024-04-12 01:58:24.892889 reskyblock-0.2.3/tests/test_httpx_client.py
--rw-r--r--   0        0        0     6279 2024-04-12 01:58:24.892889 reskyblock-0.2.3/tests/test_nbt.py
--rw-r--r--   0        0        0      819 2024-04-12 01:58:24.892889 reskyblock-0.2.3/tests/test_urls.py
--rw-r--r--   0        0        0      358 1970-01-01 00:00:00.000000 reskyblock-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-05 03:40:49.117972 reskyblock-0.2.4/LICENSE
+-rw-r--r--   0        0        0       13 2024-05-05 03:40:49.117972 reskyblock-0.2.4/README.md
+-rw-r--r--   0        0        0     2689 2024-05-05 03:41:07.022198 reskyblock-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      441 2024-05-05 03:40:49.117972 reskyblock-0.2.4/src/reskyblock/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 03:40:49.117972 reskyblock-0.2.4/src/reskyblock/__main__.py
+-rw-r--r--   0        0        0     9808 2024-05-05 03:40:49.117972 reskyblock-0.2.4/src/reskyblock/client.py
+-rw-r--r--   0        0        0      212 2024-05-05 03:40:49.117972 reskyblock-0.2.4/src/reskyblock/http/__init__.py
+-rw-r--r--   0        0        0     2130 2024-05-05 03:40:49.117972 reskyblock-0.2.4/src/reskyblock/http/http_adapter.py
+-rw-r--r--   0        0        0      387 2024-05-05 03:40:49.117972 reskyblock-0.2.4/src/reskyblock/models/__init__.py
+-rw-r--r--   0        0        0     1353 2024-05-05 03:40:49.117972 reskyblock-0.2.4/src/reskyblock/models/auctions.py
+-rw-r--r--   0        0        0      666 2024-05-05 03:40:49.117972 reskyblock-0.2.4/src/reskyblock/models/auctions_ended.py
+-rw-r--r--   0        0        0      716 2024-05-05 03:40:49.117972 reskyblock-0.2.4/src/reskyblock/models/bazaar.py
+-rw-r--r--   0        0        0       73 2024-05-05 03:40:49.117972 reskyblock-0.2.4/src/reskyblock/nbt/__init__.py
+-rw-r--r--   0        0        0     3357 2024-05-05 03:40:49.117972 reskyblock-0.2.4/src/reskyblock/nbt/decoder.py
+-rw-r--r--   0        0        0        0 2024-05-05 03:40:49.117972 reskyblock-0.2.4/src/reskyblock/py.typed
+-rw-r--r--   0        0        0      131 2024-05-05 03:40:49.117972 reskyblock-0.2.4/src/reskyblock/serialization/__init__.py
+-rw-r--r--   0        0        0      992 2024-05-05 03:40:49.117972 reskyblock-0.2.4/src/reskyblock/serialization/json.py
+-rw-r--r--   0        0        0      575 2024-05-05 03:40:49.117972 reskyblock-0.2.4/src/reskyblock/urls.py
+-rw-r--r--   0        0        0        0 2024-05-05 03:40:49.117972 reskyblock-0.2.4/tests/__init__.py
+-rw-r--r--   0        0        0  2018239 2024-05-05 03:40:49.129973 reskyblock-0.2.4/tests/data/auctions.json
+-rw-r--r--   0        0        0  2039142 2024-05-05 03:40:49.141973 reskyblock-0.2.4/tests/data/auctions2.json
+-rw-r--r--   0        0        0   315276 2024-05-05 03:40:49.141973 reskyblock-0.2.4/tests/data/auctions_ended.json
+-rw-r--r--   0        0        0  2264250 2024-05-05 03:40:49.149973 reskyblock-0.2.4/tests/data/bazaar.json
+-rw-r--r--   0        0        0    89195 2024-05-05 03:40:49.149973 reskyblock-0.2.4/tests/data/item_bytes.txt
+-rw-r--r--   0        0        0     3204 2024-05-05 03:40:49.149973 reskyblock-0.2.4/tests/test_client.py
+-rw-r--r--   0        0        0      692 2024-05-05 03:40:49.149973 reskyblock-0.2.4/tests/test_httpx_client.py
+-rw-r--r--   0        0        0     1992 2024-05-05 03:40:49.149973 reskyblock-0.2.4/tests/test_mock_client.py
+-rw-r--r--   0        0        0     8497 2024-05-05 03:40:49.149973 reskyblock-0.2.4/tests/test_nbt.py
+-rw-r--r--   0        0        0      819 2024-05-05 03:40:49.149973 reskyblock-0.2.4/tests/test_urls.py
+-rw-r--r--   0        0        0      358 1970-01-01 00:00:00.000000 reskyblock-0.2.4/PKG-INFO
```

### Comparing `reskyblock-0.2.3/pyproject.toml` & `reskyblock-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "reskyblock"
-version = "0.2.3"
+version = "0.2.4"
 description = "Python API wrapper for Hypixel SkyBlock"
 authors = [
     { name = "ch-iv", email = "alicesummer38@gmail.com" },
 ]
 dependencies = [
     "pyright>=1.1.350",
     "httpx>=0.26.0",
```

### Comparing `reskyblock-0.2.3/src/reskyblock/http/http_adapter.py` & `reskyblock-0.2.4/src/reskyblock/http/http_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """This module provides all needed functionality for dealing with http requests"""
+
 from abc import ABC, abstractmethod
 
 import httpx
 
 __all__ = ("AbstractHTTPClient", "HTTPXClient", "HTTPXAsyncClient", "AbstractAsyncHTTPClient")
```

### Comparing `reskyblock-0.2.3/src/reskyblock/models/auctions.py` & `reskyblock-0.2.4/src/reskyblock/models/auctions.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,19 +46,21 @@
     uuid: str
     auctioneer: str
     profile_id: str
     decoded_nbt: DecodedNBT | None = None
     command: str | None = None
 
     def __post_init__(self) -> None:
-        self.decoded_nbt = DecodedNBT(raw_data=self.item_bytes)
+        if self.decoded_nbt is None:
+            self.decoded_nbt = DecodedNBT(raw_data=self.item_bytes)
 
-        self.command = (
-            f"/viewauction {self.uuid[:9]}-"
-            f"{self.uuid[9:13]}-{self.uuid[13:17]}-"
-            f"{self.uuid[17:21]}-{self.uuid[21:]}"
-        )
+        if self.command is None:
+            self.command = (
+                f"/viewauction {self.uuid[:9]}-"
+                f"{self.uuid[9:13]}-{self.uuid[13:17]}-"
+                f"{self.uuid[17:21]}-{self.uuid[21:]}"
+            )
 
 
 class AllAuctions(msgspec.Struct):
     last_updated: int
     auctions: list[Auction]
```

### Comparing `reskyblock-0.2.3/src/reskyblock/models/auctions_ended.py` & `reskyblock-0.2.4/src/reskyblock/models/auctions_ended.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     timestamp: int
     price: int
     bin: bool
     item_bytes: str
     decoded_nbt: DecodedNBT | None = None
 
     def __post_init__(self) -> None:
-        self.decoded_nbt = DecodedNBT(raw_data=self.item_bytes)
+        if self.decoded_nbt is None:
+            self.decoded_nbt = DecodedNBT(raw_data=self.item_bytes)
 
 
 class AuctionsEnded(msgspec.Struct, rename="camel"):
     success: bool
     last_updated: int
     auctions: list[EndedAuction]
```

### Comparing `reskyblock-0.2.3/src/reskyblock/models/bazaar.py` & `reskyblock-0.2.4/src/reskyblock/models/bazaar.py`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.3/src/reskyblock/serialization/json.py` & `reskyblock-0.2.4/src/reskyblock/serialization/json.py`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.3/src/reskyblock/urls.py` & `reskyblock-0.2.4/src/reskyblock/urls.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """URLs for the SkyBlock API"""
+
 import random
 
 _AUCTIONS_URL = "https://api.hypixel.net/v2/skyblock/auctions"
 _AUCTIONS_ENDED_URL = "https://api.hypixel.net/v2/skyblock/auctions_ended"
 _BAZAAR_URL = "https://api.hypixel.net/v2/skyblock/bazaar"
```

### Comparing `reskyblock-0.2.3/tests/data/auctions.json` & `reskyblock-0.2.4/tests/data/auctions.json`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.3/tests/data/auctions2.json` & `reskyblock-0.2.4/tests/data/auctions2.json`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.3/tests/data/auctions_ended.json` & `reskyblock-0.2.4/tests/data/auctions_ended.json`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.3/tests/data/bazaar.json` & `reskyblock-0.2.4/tests/data/bazaar.json`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.3/tests/data/item_bytes.txt` & `reskyblock-0.2.4/tests/data/item_bytes.txt`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.3/tests/test_client.py` & `reskyblock-0.2.4/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.3/tests/test_httpx_client.py` & `reskyblock-0.2.4/tests/test_httpx_client.py`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.3/tests/test_nbt.py` & `reskyblock-0.2.4/tests/test_nbt.py`

 * *Files 27% similar despite different names*

```diff
@@ -72,11 +72,74 @@
     assert did.dungeon_stars == 9
     assert did.scrolls == [
         "WITHER_SHIELD_SCROLL",
         "SHADOW_WARP_SCROLL",
         "IMPLOSION_SCROLL",
     ]
 
+    assert did.dict() == {
+        "Count": 1,
+        "Damage": 0,
+        "id": 267,
+        "tag": {
+            "ExtraAttributes": {
+                "ability_scroll": None,
+                "art_of_war_count": 1,
+                "champion_combat_xp": 72582071.63017021,
+                "enchantments": {
+                    "champion": 10,
+                    "cleave": 6,
+                    "critical": 6,
+                    "cubism": 5,
+                    "dragon_hunter": 1,
+                    "ender_slayer": 7,
+                    "execute": 5,
+                    "experience": 4,
+                    "fire_aspect": 3,
+                    "first_strike": 4,
+                    "giant_killer": 6,
+                    "impaling": 3,
+                    "lethality": 6,
+                    "looting": 4,
+                    "luck": 6,
+                    "scavenger": 4,
+                    "smite": 7,
+                    "smoldering": 2,
+                    "syphon": 4,
+                    "thunderlord": 7,
+                    "ultimate_wise": 5,
+                    "vampirism": 6,
+                    "venomous": 5,
+                },
+                "gems": {
+                    "COMBAT_0": "FINE",
+                    "COMBAT_0_gem": "SAPPHIRE",
+                    "DEFENSIVE_0": {"quality": "PERFECT", "uuid": "84c26564-2981-431f-9051-273668a0af50"},
+                    "DEFENSIVE_0_gem": "AMETHYST",
+                    "SAPPHIRE_0": "FINE",
+                    "unlocked_slots": None,
+                },
+                "hot_potato_count": 15,
+                "id": "HYPERION",
+                "modifier": "heroic",
+                "rarity_upgrades": 1,
+                "stats_book": 177662,
+                "timestamp": 1657706160000,
+                "upgrade_level": 9,
+                "uuid": "21616c2d-6a14-4690-9b52-8d1857ed30cb",
+            },
+            "HideFlags": 254,
+            "Unbreakable": 1,
+            "display": {"Lore": None, "Name": "§dHeroic Hyperion §6✪§6✪§6✪§6✪§6✪§c➍"},
+            "ench": None,
+        },
+    }
+
 
 @pytest.mark.parametrize("raw_data", _BULK_NBTS)
 def test_bulk_nbts(raw_data: str) -> None:
     DecodedNBT(raw_data)
+
+
+@pytest.mark.parametrize("raw_data", _BULK_NBTS)
+def test_bulk_nbts_dicts(raw_data: str) -> None:
+    DecodedNBT(raw_data).dict()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `reskyblock-0.2.3/tests/test_urls.py` & `reskyblock-0.2.4/tests/test_urls.py`

 * *Files identical despite different names*

