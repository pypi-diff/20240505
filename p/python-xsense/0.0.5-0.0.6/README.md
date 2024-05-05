# Comparing `tmp/python-xsense-0.0.5.tar.gz` & `tmp/python-xsense-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-xsense-0.0.5.tar", last modified: Fri Apr 26 20:22:32 2024, max compression
+gzip compressed data, was "python-xsense-0.0.6.tar", last modified: Sun May  5 17:49:45 2024, max compression
```

## Comparing `python-xsense-0.0.5.tar` & `python-xsense-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2024-04-26 20:22:32.158665 python-xsense-0.0.5/
--rw-r--r--   0 theo       (501) staff       (20)     1859 2024-04-26 20:22:32.157964 python-xsense-0.0.5/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)     1226 2024-04-18 18:45:42.000000 python-xsense-0.0.5/README.rst
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2024-04-26 20:22:32.157256 python-xsense-0.0.5/python_xsense.egg-info/
--rw-r--r--   0 theo       (501) staff       (20)     1859 2024-04-26 20:22:31.000000 python-xsense-0.0.5/python_xsense.egg-info/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)      421 2024-04-26 20:22:31.000000 python-xsense-0.0.5/python_xsense.egg-info/SOURCES.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2024-04-26 20:22:31.000000 python-xsense-0.0.5/python_xsense.egg-info/dependency_links.txt
--rw-r--r--   0 theo       (501) staff       (20)       51 2024-04-26 20:22:31.000000 python-xsense-0.0.5/python_xsense.egg-info/requires.txt
--rw-r--r--   0 theo       (501) staff       (20)        7 2024-04-26 20:22:31.000000 python-xsense-0.0.5/python_xsense.egg-info/top_level.txt
--rw-r--r--   0 theo       (501) staff       (20)       38 2024-04-26 20:22:32.158741 python-xsense-0.0.5/setup.cfg
--rw-r--r--   0 theo       (501) staff       (20)      911 2024-04-26 20:21:56.000000 python-xsense-0.0.5/setup.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2024-04-26 20:22:32.156345 python-xsense-0.0.5/xsense/
--rw-r--r--   0 theo       (501) staff       (20)      147 2024-02-20 08:37:03.000000 python-xsense-0.0.5/xsense/__init__.py
--rw-r--r--   0 theo       (501) staff       (20)     5906 2024-04-26 20:21:49.000000 python-xsense-0.0.5/xsense/async_xsense.py
--rw-r--r--   0 theo       (501) staff       (20)     3745 2024-04-18 16:47:49.000000 python-xsense-0.0.5/xsense/aws_signer.py
--rw-r--r--   0 theo       (501) staff       (20)     6437 2024-04-26 20:21:49.000000 python-xsense-0.0.5/xsense/base.py
--rw-r--r--   0 theo       (501) staff       (20)      387 2024-04-25 20:57:22.000000 python-xsense-0.0.5/xsense/device.py
--rw-r--r--   0 theo       (501) staff       (20)      546 2024-04-26 20:21:49.000000 python-xsense-0.0.5/xsense/entity.py
--rw-r--r--   0 theo       (501) staff       (20)      169 2024-04-26 20:21:49.000000 python-xsense-0.0.5/xsense/exceptions.py
--rw-r--r--   0 theo       (501) staff       (20)     1019 2024-04-14 14:39:29.000000 python-xsense-0.0.5/xsense/house.py
--rw-r--r--   0 theo       (501) staff       (20)     1016 2024-04-26 20:21:49.000000 python-xsense-0.0.5/xsense/mapping.py
--rw-r--r--   0 theo       (501) staff       (20)     1198 2024-04-14 16:07:00.000000 python-xsense-0.0.5/xsense/station.py
--rw-r--r--   0 theo       (501) staff       (20)     1411 2024-04-14 18:51:33.000000 python-xsense-0.0.5/xsense/utils.py
--rw-r--r--   0 theo       (501) staff       (20)     5023 2024-04-26 20:21:49.000000 python-xsense-0.0.5/xsense/xsense.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2024-05-05 17:49:45.933220 python-xsense-0.0.6/
+-rw-r--r--   0 theo       (501) staff       (20)     1859 2024-05-05 17:49:45.932017 python-xsense-0.0.6/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)     1226 2024-04-18 18:45:42.000000 python-xsense-0.0.6/README.rst
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2024-05-05 17:49:45.930617 python-xsense-0.0.6/python_xsense.egg-info/
+-rw-r--r--   0 theo       (501) staff       (20)     1859 2024-05-05 17:49:45.000000 python-xsense-0.0.6/python_xsense.egg-info/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)      421 2024-05-05 17:49:45.000000 python-xsense-0.0.6/python_xsense.egg-info/SOURCES.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2024-05-05 17:49:45.000000 python-xsense-0.0.6/python_xsense.egg-info/dependency_links.txt
+-rw-r--r--   0 theo       (501) staff       (20)       51 2024-05-05 17:49:45.000000 python-xsense-0.0.6/python_xsense.egg-info/requires.txt
+-rw-r--r--   0 theo       (501) staff       (20)        7 2024-05-05 17:49:45.000000 python-xsense-0.0.6/python_xsense.egg-info/top_level.txt
+-rw-r--r--   0 theo       (501) staff       (20)       38 2024-05-05 17:49:45.933372 python-xsense-0.0.6/setup.cfg
+-rw-r--r--   0 theo       (501) staff       (20)      911 2024-05-05 17:49:13.000000 python-xsense-0.0.6/setup.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2024-05-05 17:49:45.928593 python-xsense-0.0.6/xsense/
+-rw-r--r--   0 theo       (501) staff       (20)      147 2024-02-20 08:37:03.000000 python-xsense-0.0.6/xsense/__init__.py
+-rw-r--r--   0 theo       (501) staff       (20)     7084 2024-05-05 17:49:04.000000 python-xsense-0.0.6/xsense/async_xsense.py
+-rw-r--r--   0 theo       (501) staff       (20)     3745 2024-05-05 17:48:22.000000 python-xsense-0.0.6/xsense/aws_signer.py
+-rw-r--r--   0 theo       (501) staff       (20)     7201 2024-05-05 17:49:04.000000 python-xsense-0.0.6/xsense/base.py
+-rw-r--r--   0 theo       (501) staff       (20)      387 2024-05-05 17:46:03.000000 python-xsense-0.0.6/xsense/device.py
+-rw-r--r--   0 theo       (501) staff       (20)      801 2024-05-05 17:49:04.000000 python-xsense-0.0.6/xsense/entity.py
+-rw-r--r--   0 theo       (501) staff       (20)      214 2024-05-05 17:49:04.000000 python-xsense-0.0.6/xsense/exceptions.py
+-rw-r--r--   0 theo       (501) staff       (20)     1163 2024-05-05 17:49:04.000000 python-xsense-0.0.6/xsense/house.py
+-rw-r--r--   0 theo       (501) staff       (20)     1114 2024-05-05 17:49:04.000000 python-xsense-0.0.6/xsense/mapping.py
+-rw-r--r--   0 theo       (501) staff       (20)     1204 2024-05-05 17:49:04.000000 python-xsense-0.0.6/xsense/station.py
+-rw-r--r--   0 theo       (501) staff       (20)     1411 2024-05-05 17:46:39.000000 python-xsense-0.0.6/xsense/utils.py
+-rw-r--r--   0 theo       (501) staff       (20)     5972 2024-05-05 17:49:04.000000 python-xsense-0.0.6/xsense/xsense.py
```

### Comparing `python-xsense-0.0.5/PKG-INFO` & `python-xsense-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-xsense
-Version: 0.0.5
+Version: 0.0.6
 Summary: XSense Python Module
 Home-page: https://github.com/theosnel/python-xsense
 Author: Theo Snelleman
 Author-email: <python@theo.snelleman.net>
 License: MIT
 Keywords: python,xsense
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `python-xsense-0.0.5/README.rst` & `python-xsense-0.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `python-xsense-0.0.5/python_xsense.egg-info/PKG-INFO` & `python-xsense-0.0.6/python_xsense.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-xsense
-Version: 0.0.5
+Version: 0.0.6
 Summary: XSense Python Module
 Home-page: https://github.com/theosnel/python-xsense
 Author: Theo Snelleman
 Author-email: <python@theo.snelleman.net>
 License: MIT
 Keywords: python,xsense
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `python-xsense-0.0.5/setup.py` & `python-xsense-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'XSense Python Module'
 
 with open('README.rst', 'r') as fd:
     LONG_DESCRIPTION = fd.read()
 
 setup(
     name='python-xsense',
```

### Comparing `python-xsense-0.0.5/xsense/async_xsense.py` & `python-xsense-0.0.6/xsense/async_xsense.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from datetime import datetime
 import json
 
 import aiohttp
 
 from xsense.aws_signer import AWSSigner
 from xsense.base import XSenseBase
-from xsense.exceptions import SessionExpired, APIFailure
+from xsense.exceptions import SessionExpired, APIFailure, NotFoundError
 from xsense.house import House
 from xsense.station import Station
 
 
 class AsyncXSense(XSenseBase):
     async def api_call(self, code, unauth=False, **kwargs):
         data = {
@@ -55,14 +55,28 @@
                     if errCode in ('10000008', '10000020'):
                         raise SessionExpired(data.get('reMsg'))
                     raise APIFailure(
                         f"Request for code {code} failed with error {errCode}/{data['reCode']} {data.get('reMsg')}"
                     )
                 return data['reData']
 
+    async def get_house(self, house: House, page: str):
+        if self._aws_token_expiring():
+            await self.load_aws()
+
+        url, headers = self._house_request(house, page)
+
+        async with aiohttp.ClientSession() as session:
+            async with session.get(
+                url,
+                headers=headers
+            ) as response:
+                self._lastres = response
+                return await response.json()
+
     async def get_thing(self, station: Station, page: str):
         if self._aws_token_expiring():
             await self.load_aws()
 
         url, headers = self._thing_request(station, page)
 
         async with aiohttp.ClientSession() as session:
@@ -110,16 +124,17 @@
                 i['mqttServer']
             )
             result[i['houseId']] = h
 
             if rooms := await self.get_rooms(h.house_id):
                 h.set_rooms(rooms)
 
-            if station := await self.get_stations(h.house_id):
-                h.set_stations(station)
+            if stations := await self.get_stations(h.house_id):
+                h.set_stations(stations)
+
         self.houses = result
 
     async def get_client_info(self):
         data = await self.api_call("101001", unauth=True)
         self.clientid = data['clientId']
         self.clientsecret = self._decode_secret(data['clientSecret'])
         self.region = data['cgtRegion']
@@ -148,22 +163,41 @@
     async def get_stations(self, houseId: str):
         params = {
             'houseId': houseId,
             'utctimestamp': "0"
         }
         return await self.api_call("103007", **params)
 
+    async def get_house_state(self, house: House):
+        res = await self.get_house(house, 'mainpage')
+        if self._lastres.status == 404:
+            raise NotFoundError(await self._lastres.text)
+
+        if 'reported' in res.get('state', {}):
+            self._parse_get_house_state(house, res['state']['reported'])
+        else:
+            text = await self._lastres.text()
+            raise APIFailure(f'Unable to retrieve house data: {self._lastres.status}/{text}')
+
     async def get_station_state(self, station: Station):
-        res = await self.get_thing(station, f'2nd_info_{station.sn}')
+        if station.type == 'SBS50':
+            res = await self.get_thing(station, f'2nd_info_{station.sn}')
+        else:
+            res = await self.get_thing(station, f'info_{station.sn}')
 
         if 'reported' in res.get('state', {}):
             station.set_data(res['state']['reported'])
         else:
-            raise APIFailure(f'Unable to retrieve station data: {self._lastres.status}/{self._lastres.text()}')
+            text = await self._lastres.text()
+            raise APIFailure(f'Unable to retrieve station data: {self._lastres.status}/{text}')
 
     async def get_state(self, station: Station):
+        if not station.devices:
+            return
+
         res = await self.get_thing(station, '2nd_mainpage')
 
         if 'reported' in res.get('state', {}):
             self._parse_get_state(station, res['state']['reported'])
         else:
-            raise APIFailure(f'Unable to retrieve station data: {self._lastres.status}/{self._lastres.text()}')
+            text = await self._lastres.text()
+            raise APIFailure(f'Unable to retrieve station data: {self._lastres.status}/{text}')
```

### Comparing `python-xsense-0.0.5/xsense/aws_signer.py` & `python-xsense-0.0.6/xsense/aws_signer.py`

 * *Files identical despite different names*

### Comparing `python-xsense-0.0.5/xsense/base.py` & `python-xsense-0.0.6/xsense/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -155,23 +155,40 @@
         headers = {
             'x-amz-date': amz_date,
             'x-amz-target': 'AWSCognitoIdentityProviderService.InitiateAuth',
             'content-type': 'application/x-amz-json-1.1'
         }
         return url, data, headers
 
+    def _house_request(self, house: House, page: str):
+        headers = {
+            'Content-Type': 'application/x-amz-json-1.0',
+            'User-Agent': 'aws-sdk-iOS/2.26.5 iOS/17.3 nl_NL',
+            'X-Amz-Security-Token': self.aws_session_token
+        }
+
+        host = f'{house.mqtt_region}.x-sense-iot.com'
+        uri = f'/things/{house.house_id}/shadow?name={page}'
+
+        url = f'https://{host}{uri}'
+
+        signed = self.signer.sign_headers('GET', url, house.mqtt_region, headers, None)
+        headers |= signed
+
+        return url, headers
+
     def _thing_request(self, station: Station, page: str):
         headers = {
             'Content-Type': 'application/x-amz-json-1.0',
             'User-Agent': 'aws-sdk-iOS/2.26.5 iOS/17.3 nl_NL',
             'X-Amz-Security-Token': self.aws_session_token
         }
 
         host = f'{station.house.mqtt_region}.x-sense-iot.com'
-        uri = f'/things/SBS50{station.sn}/shadow?name={page}'
+        uri = f'/things/{station.type}{station.sn}/shadow?name={page}'
 
         url = f'https://{host}{uri}'
 
         signed = self.signer.sign_headers('GET', url, station.house.mqtt_region, headers, None)
         headers |= signed
 
         return url, headers
@@ -188,7 +205,12 @@
 
     def _parse_get_state(self, station: Station, data: Dict):
         if 'wifiRSSI' in data:
             station.data['wifiRSSI'] = data['wifiRSSI']
         for sn, i in data['devs'].items():
             dev = station.get_device_by_sn(sn)
             dev.set_data(i)
+
+    def _parse_get_house_state(self, house: House, data: Dict):
+        for sn, i in data.items():
+            if station := house.get_station_by_sn(sn):
+                station.set_data(i)
```

### Comparing `python-xsense-0.0.5/xsense/entity.py` & `python-xsense-0.0.6/xsense/entity.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,13 +13,19 @@
         self.room_id = kwargs.get('roomId')
         self._data = {}
 
     def set_data(self, values: dict):
         data = values.copy()
         if 'online' in values:
             self.online = values.pop('online') != '0'
+        if values.get('onlineTime'):
+            self.online = True
         data |= data.pop('status', {})
+        # sofware versions are reported differently per device
+        if 'swMain' in data:
+            data['wifi_sw'] = data.get('sw')
+            data['sw'] = data.pop('swMain', None)
         self._data.update(map_values(self.type, data))
 
     @property
     def data(self):
         return self._data
```

### Comparing `python-xsense-0.0.5/xsense/house.py` & `python-xsense-0.0.6/xsense/house.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import List, Dict
 
 from xsense.station import Station
 
 
 class House:
-    rooms = Dict[str, Dict[str, str]]
-    room_order = List[str]
+    rooms: Dict[str, Dict[str, str]] = None
+    room_order: List[str] = None
 
-    stations = List[Dict[str, str]]
-    station_order = List[str]
+    stations: Dict[str, Station] = None
+    station_order: List[str] = None
 
     def __init__(
             self,
             house_id: str,
             name: str,
             region: str,
             mqtt_region: str,
@@ -38,7 +38,10 @@
                 **i
             )
             s.set_devices(i)
 
             stations[i['stationId']] = s
 
         self.stations = stations
+
+    def get_station_by_sn(self, sn: str):
+        return next((i for _, i in self.stations.items() if i.sn == sn), None)
```

### Comparing `python-xsense-0.0.5/xsense/mapping.py` & `python-xsense-0.0.6/xsense/mapping.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import typing
 
 property_mapper = {
+    '*': {
+        'wifiRssi': 'wifiRSSI'
+    },
     'STH51': {
         'a': 'alarmStatus',
         'b': 'temperature',
         'c': 'humidity',
         'd': 'temperatureUnit',
         'e': 'temperatureRange',
         'f': 'humidityRange',
@@ -31,12 +34,13 @@
 
 def map_type(k: str, value: typing.Any):
     return type_mapping[k](value) if k in type_mapping else value
 
 
 def map_values(device_type: str, data: typing.Dict):
     mapping = property_mapper[device_type] if device_type in property_mapper else {}
+    mapping.update(property_mapper.get('*', {}))
 
     return {
         mapping.get(k, k): map_type(mapping.get(k, k), v)
         for k, v in data.items()
     }
```

### Comparing `python-xsense-0.0.5/xsense/station.py` & `python-xsense-0.0.6/xsense/station.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     ):
         super().__init__(**kwargs)
         self.house = parent
         self.safe_mode = kwargs.get('safeMode')
         self.entity_id = kwargs.get('stationId')
         self.name = kwargs.get('stationName')
         self.sn = kwargs.get('stationSn')
-        self.online = kwargs.get('onLine')
+        self.online = kwargs.get('onLine', True)
         self.type = kwargs.get('category')
 
     def set_devices(self, data):
         self.device_order = data.get('deviceSort')
         result = {}
         result_sn = {}
         for i in data.get('devices'):
```

### Comparing `python-xsense-0.0.5/xsense/utils.py` & `python-xsense-0.0.6/xsense/utils.py`

 * *Files identical despite different names*

### Comparing `python-xsense-0.0.5/xsense/xsense.py` & `python-xsense-0.0.6/xsense/xsense.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import datetime, timedelta
 
 import requests
 
 from xsense.aws_signer import AWSSigner
 from xsense.base import XSenseBase
-from xsense.exceptions import APIFailure, SessionExpired
+from xsense.exceptions import APIFailure, SessionExpired, NotFoundError
 from xsense.house import House
 from xsense.station import Station
 
 
 class XSense(XSenseBase):
     def api_call(self, code, unauth=False, **kwargs):
         data = {
@@ -50,21 +50,31 @@
             errCode = data.get('errCode', 0)
             if errCode in ('10000008', '10000020'):
                 raise SessionExpired(data.get('reMsg'))
             raise APIFailure(f"Request for code {code} failed with error {errCode}/{data['reCode']} {data.get('reMsg')}")
 
         return data['reData']
 
+    def get_house(self, house: House, page: str):
+        if self._aws_token_expiring():
+            self.load_aws()
+
+        url, headers = self._house_request(house, page)
+        res = requests.get(url, headers=headers)
+        self._lastres = res
+        return res.json()
+
     def get_thing(self, station: Station, page: str):
         if self._aws_token_expiring():
             self.load_aws()
 
         url, headers = self._thing_request(station, page)
-
-        return requests.get(url, headers=headers).json()
+        res = requests.get(url, headers=headers)
+        self._lastres = res
+        return res.json()
 
     def login(self, username, password):
         self.sync_login(username, password)
         self.load_aws()
 
     def refresh(self):
         url, data, headers = self._refresh_request()
@@ -138,22 +148,38 @@
     def get_stations(self, houseId: str):
         params = {
             'houseId': houseId,
             'utctimestamp': "0"
         }
         return self.api_call("103007", **params)
 
+    def get_house_state(self, house: House):
+        res = self.get_house(house, 'mainpage')
+        if self._lastres.status_code == 404:
+            raise NotFoundError(self._lastres.text)
+
+        if 'reported' in res.get('state', {}):
+            self._parse_get_house_state(house, res['state']['reported'])
+        else:
+            raise APIFailure(f'Unable to retrieve station data: {self._lastres.status_code}/{self._lastres.text}')
+
     def get_station_state(self, station: Station):
-        res = self.get_thing(station, f'2nd_info_{station.sn}')
+        if station.type == 'SBS50':
+            res = self.get_thing(station, f'2nd_info_{station.sn}')
+        else:
+            res = self.get_thing(station, f'info_{station.sn}')
 
         if 'reported' in res.get('state', {}):
             station.set_data(res['state']['reported'])
         else:
             raise APIFailure(f'Unable to retrieve station data: {self._lastres.status_code}/{self._lastres.text}')
 
     def get_state(self, station: Station):
+        if not station.devices:
+            return
+
         res = self.get_thing(station, '2nd_mainpage')
 
         if 'reported' in res.get('state', {}):
             self._parse_get_state(station, res['state']['reported'])
         else:
             raise APIFailure(f'Unable to retrieve station data: {self._lastres.status_code}/{self._lastres.text}')
```

