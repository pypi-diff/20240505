# Comparing `tmp/airthings_ble-0.8.0.tar.gz` & `tmp/airthings_ble-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airthings_ble-0.8.0.tar", max compression
+gzip compressed data, was "airthings_ble-0.9.0.tar", max compression
```

## Comparing `airthings_ble-0.8.0.tar` & `airthings_ble-0.9.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1078 2024-05-02 09:40:09.242837 airthings_ble-0.8.0/LICENSE
--rw-r--r--   0        0        0      985 2024-05-02 09:40:09.242837 airthings_ble-0.8.0/README.md
--rw-r--r--   0        0        0      304 2024-05-02 09:40:11.482850 airthings_ble-0.8.0/airthings_ble/__init__.py
--rw-r--r--   0        0        0     2157 2024-05-02 09:40:09.242837 airthings_ble-0.8.0/airthings_ble/const.py
--rw-r--r--   0        0        0     4048 2024-05-02 09:40:09.242837 airthings_ble-0.8.0/airthings_ble/device_type.py
--rw-r--r--   0        0        0    25217 2024-05-02 09:40:09.242837 airthings_ble-0.8.0/airthings_ble/parser.py
--rw-r--r--   0        0        0        0 2024-05-02 09:40:09.242837 airthings_ble-0.8.0/airthings_ble/py.typed
--rw-r--r--   0        0        0     2182 2024-05-02 09:40:11.458850 airthings_ble-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2192 1970-01-01 00:00:00.000000 airthings_ble-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-05-05 18:32:20.466195 airthings_ble-0.9.0/LICENSE
+-rw-r--r--   0        0        0      985 2024-05-05 18:32:20.466195 airthings_ble-0.9.0/README.md
+-rw-r--r--   0        0        0      304 2024-05-05 18:32:21.834212 airthings_ble-0.9.0/airthings_ble/__init__.py
+-rw-r--r--   0        0        0     2165 2024-05-05 18:32:20.466195 airthings_ble-0.9.0/airthings_ble/const.py
+-rw-r--r--   0        0        0     4048 2024-05-05 18:32:20.466195 airthings_ble-0.9.0/airthings_ble/device_type.py
+-rw-r--r--   0        0        0    25525 2024-05-05 18:32:20.466195 airthings_ble-0.9.0/airthings_ble/parser.py
+-rw-r--r--   0        0        0        0 2024-05-05 18:32:20.466195 airthings_ble-0.9.0/airthings_ble/py.typed
+-rw-r--r--   0        0        0     2182 2024-05-05 18:32:21.806212 airthings_ble-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2192 1970-01-01 00:00:00.000000 airthings_ble-0.9.0/PKG-INFO
```

### Comparing `airthings_ble-0.8.0/LICENSE` & `airthings_ble-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `airthings_ble-0.8.0/README.md` & `airthings_ble-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `airthings_ble-0.8.0/airthings_ble/const.py` & `airthings_ble-0.9.0/airthings_ble/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,8 +49,8 @@
 
 CO2_MAX = 65534
 VOC_MAX = 65534
 PERCENTAGE_MAX = 100
 RADON_MAX = 16383
 TEMPERATURE_MAX = 100
 
-MAX_UPDATE_ATTEMPTS = 3
+DEFAULT_MAX_UPDATE_ATTEMPTS = 1
```

### Comparing `airthings_ble-0.8.0/airthings_ble/device_type.py` & `airthings_ble-0.9.0/airthings_ble/device_type.py`

 * *Files identical despite different names*

### Comparing `airthings_ble-0.8.0/airthings_ble/parser.py` & `airthings_ble-0.9.0/airthings_ble/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from async_interrupt import interrupt
 from bleak import BleakClient, BleakError
 from bleak.backends.device import BLEDevice
 from bleak_retry_connector import BleakClientWithServiceCache, establish_connection
 
 from .const import (
-    MAX_UPDATE_ATTEMPTS,
+    DEFAULT_MAX_UPDATE_ATTEMPTS,
     BQ_TO_PCI_MULTIPLIER,
     CHAR_UUID_DATETIME,
     CHAR_UUID_DEVICE_NAME,
     CHAR_UUID_FIRMWARE_REV,
     CHAR_UUID_HARDWARE_REV,
     CHAR_UUID_HUMIDITY,
     CHAR_UUID_ILLUMINANCE_ACCELEROMETER,
@@ -477,18 +477,25 @@
 class AirthingsBluetoothDeviceData:
     """Data for Airthings BLE sensors."""
 
     def __init__(
         self,
         logger: Logger,
         is_metric: bool = True,
+        max_attempts: int = DEFAULT_MAX_UPDATE_ATTEMPTS,
     ) -> None:
+        """Initialize the Airthings BLE sensor data object."""
         self.logger = logger
         self.is_metric = is_metric
         self.device_info = AirthingsDeviceInfo()
+        self.max_attempts = max_attempts
+
+    def set_max_attempts(self, max_attempts: int) -> None:
+        """Set the number of attempts."""
+        self.max_attempts = max_attempts
 
     async def _get_device_characteristics(
         self, client: BleakClient, device: AirthingsDevice
     ) -> None:
         device_info = self.device_info
         device_info.address = client.address
         did_first_sync = device_info.did_first_sync
@@ -644,16 +651,16 @@
         """Handle disconnect from device."""
         self.logger.debug("Disconnected from %s", client.address)
         if not disconnect_future.done():
             disconnect_future.set_result(True)
 
     async def update_device(self, ble_device: BLEDevice) -> AirthingsDevice:
         """Connects to the device through BLE and retrieves relevant data"""
-        for attempt in range(MAX_UPDATE_ATTEMPTS):
-            is_final_attempt = attempt == MAX_UPDATE_ATTEMPTS - 1
+        for attempt in range(self.max_attempts):
+            is_final_attempt = attempt == self.max_attempts - 1
             try:
                 return await self._update_device(ble_device)
             except DisconnectedError:
                 if is_final_attempt:
                     raise
                 self.logger.debug(
                     "Unexpectedly disconnected from %s", ble_device.address
```

### Comparing `airthings_ble-0.8.0/pyproject.toml` & `airthings_ble-0.9.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "airthings-ble"
-version = "0.8.0"
+version = "0.9.0"
 description = "Manage Airthings BLE devices"
 authors = ["Vincent Giorgi", "Ståle Storø Hauknes"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/Airthings/airthings-ble"
 documentation = "https://airthings-ble.readthedocs.io"
 classifiers = [
```

### Comparing `airthings_ble-0.8.0/PKG-INFO` & `airthings_ble-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airthings-ble
-Version: 0.8.0
+Version: 0.9.0
 Summary: Manage Airthings BLE devices
 Home-page: https://github.com/Airthings/airthings-ble
 License: Apache Software License 2.0
 Author: Vincent Giorgi
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

