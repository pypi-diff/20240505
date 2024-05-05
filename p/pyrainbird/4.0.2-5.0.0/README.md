# Comparing `tmp/pyrainbird-4.0.2.tar.gz` & `tmp/pyrainbird-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrainbird-4.0.2.tar", last modified: Sat Feb 17 18:14:39 2024, max compression
+gzip compressed data, was "pyrainbird-5.0.0.tar", last modified: Sun May  5 06:55:39 2024, max compression
```

## Comparing `pyrainbird-4.0.2.tar` & `pyrainbird-5.0.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 18:14:39.490288 pyrainbird-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-17 18:14:30.000000 pyrainbird-4.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-02-17 18:14:39.490288 pyrainbird-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-02-17 18:14:30.000000 pyrainbird-4.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 18:14:39.486288 pyrainbird-4.0.2/pyrainbird/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-17 18:14:30.000000 pyrainbird-4.0.2/pyrainbird/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18927 2024-02-17 18:14:30.000000 pyrainbird-4.0.2/pyrainbird/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-02-17 18:14:30.000000 pyrainbird-4.0.2/pyrainbird/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    21246 2024-02-17 18:14:30.000000 pyrainbird-4.0.2/pyrainbird/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-02-17 18:14:30.000000 pyrainbird-4.0.2/pyrainbird/encryption.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-02-17 18:14:30.000000 pyrainbird-4.0.2/pyrainbird/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-02-17 18:14:30.000000 pyrainbird-4.0.2/pyrainbird/rainbird.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 18:14:39.486288 pyrainbird-4.0.2/pyrainbird/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-02-17 18:14:30.000000 pyrainbird-4.0.2/pyrainbird/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-02-17 18:14:30.000000 pyrainbird-4.0.2/pyrainbird/resources/models.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7268 2024-02-17 18:14:30.000000 pyrainbird-4.0.2/pyrainbird/resources/sipcommands.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-02-17 18:14:30.000000 pyrainbird-4.0.2/pyrainbird/timeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 18:14:39.490288 pyrainbird-4.0.2/pyrainbird.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-02-17 18:14:39.000000 pyrainbird-4.0.2/pyrainbird.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-17 18:14:39.000000 pyrainbird-4.0.2/pyrainbird.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-17 18:14:39.000000 pyrainbird-4.0.2/pyrainbird.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-17 18:14:39.000000 pyrainbird-4.0.2/pyrainbird.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-17 18:14:39.000000 pyrainbird-4.0.2/pyrainbird.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-02-17 18:14:39.490288 pyrainbird-4.0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       80 2024-02-17 18:14:30.000000 pyrainbird-4.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 18:14:39.490288 pyrainbird-4.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    47505 2024-02-17 18:14:30.000000 pyrainbird-4.0.2/tests/test_async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-02-17 18:14:30.000000 pyrainbird-4.0.2/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-02-17 18:14:30.000000 pyrainbird-4.0.2/tests/test_rainbird.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:55:39.508157 pyrainbird-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-05 06:55:35.000000 pyrainbird-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-05 06:55:39.508157 pyrainbird-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-05 06:55:35.000000 pyrainbird-5.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:55:39.504157 pyrainbird-5.0.0/pyrainbird/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-05 06:55:35.000000 pyrainbird-5.0.0/pyrainbird/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18927 2024-05-05 06:55:35.000000 pyrainbird-5.0.0/pyrainbird/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-05 06:55:35.000000 pyrainbird-5.0.0/pyrainbird/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23102 2024-05-05 06:55:35.000000 pyrainbird-5.0.0/pyrainbird/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-05-05 06:55:35.000000 pyrainbird-5.0.0/pyrainbird/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-05 06:55:35.000000 pyrainbird-5.0.0/pyrainbird/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-05-05 06:55:35.000000 pyrainbird-5.0.0/pyrainbird/rainbird.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:55:39.504157 pyrainbird-5.0.0/pyrainbird/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-05 06:55:35.000000 pyrainbird-5.0.0/pyrainbird/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-05 06:55:35.000000 pyrainbird-5.0.0/pyrainbird/resources/models.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7268 2024-05-05 06:55:35.000000 pyrainbird-5.0.0/pyrainbird/resources/sipcommands.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-05 06:55:35.000000 pyrainbird-5.0.0/pyrainbird/timeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:55:39.508157 pyrainbird-5.0.0/pyrainbird.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-05 06:55:39.000000 pyrainbird-5.0.0/pyrainbird.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-05 06:55:39.000000 pyrainbird-5.0.0/pyrainbird.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 06:55:39.000000 pyrainbird-5.0.0/pyrainbird.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-05 06:55:39.000000 pyrainbird-5.0.0/pyrainbird.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-05 06:55:39.000000 pyrainbird-5.0.0/pyrainbird.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-05 06:55:39.508157 pyrainbird-5.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       80 2024-05-05 06:55:35.000000 pyrainbird-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:55:39.508157 pyrainbird-5.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    47508 2024-05-05 06:55:35.000000 pyrainbird-5.0.0/tests/test_async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-05 06:55:35.000000 pyrainbird-5.0.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-05 06:55:35.000000 pyrainbird-5.0.0/tests/test_rainbird.py
```

### Comparing `pyrainbird-4.0.2/LICENSE` & `pyrainbird-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrainbird-4.0.2/PKG-INFO` & `pyrainbird-5.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyrainbird
-Version: 4.0.2
+Version: 5.0.0
 Summary: Rain Bird Controller
 Home-page: https://github.com/allenporter/pyrainbird
 Author: J.J.Barrancos
 Author-email: jordy@fusion-ict.nl
 License: MIT
 Keywords: Rain Bird
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pycryptodome>=3.16.0
 Requires-Dist: requests>=2.22.0
 Requires-Dist: PyYAML>=5.4
-Requires-Dist: pydantic>=1.10.4
+Requires-Dist: mashumaro>=3.12
 Requires-Dist: python-dateutil>=2.8.2
 Requires-Dist: ical>=4.2.9
 Requires-Dist: aiohttp_retry>=2.8.3
 
 Python module for interacting with [WiFi LNK](https://www.rainbird.com/products/module-wi-fi-lnk) module of the Rain Bird Irrigation system. This project has no affiliation with Rain Bird.
 
 This module communicates directly towards the IP Address of the WiFi module. You can start/stop the irrigation, get the currently active zone, and other controller settings. This library currently only has very limited cloud support. Also there are a number of Rain Bird devices with very different command APIs.
```

### Comparing `pyrainbird-4.0.2/README.md` & `pyrainbird-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pyrainbird-4.0.2/pyrainbird/async_client.py` & `pyrainbird-5.0.0/pyrainbird/async_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -242,45 +242,45 @@
             value.month,
             value.year,
         )
 
     async def get_wifi_params(self) -> WifiParams:
         """Return wifi parameters and other settings."""
         result = await self._local_client.request("getWifiParams")
-        return WifiParams.parse_obj(result)
+        return WifiParams.from_dict(result)
 
     async def get_settings(self) -> Settings:
         """Return a combined set of device settings."""
         result = await self._local_client.request("getSettings")
-        return Settings.parse_obj(result)
+        return Settings.from_dict(result)
 
     async def get_weather_adjustment_mask(self) -> WeatherAdjustmentMask:
         """Return the weather adjustment mask, subset of the settings."""
         result = await self._local_client.request("getWeatherAdjustmentMask")
-        return WeatherAdjustmentMask.parse_obj(result)
+        return WeatherAdjustmentMask.from_dict(result)
 
     async def get_zip_code(self) -> ZipCode:
         """Return zip code and location, a subset of the settings."""
         result = await self._local_client.request("getZipCode")
-        return ZipCode.parse_obj(result)
+        return ZipCode.from_dict(result)
 
     async def get_program_info(self) -> ProgramInfo:
         """Return program information, a subset of the settings."""
         result = await self._local_client.request("getProgramInfo")
-        return ProgramInfo.parse_obj(result)
+        return ProgramInfo.from_dict(result)
 
     async def get_network_status(self) -> NetworkStatus:
         """Return the device network status."""
         result = await self._local_client.request("getNetworkStatus")
-        return NetworkStatus.parse_obj(result)
+        return NetworkStatus.from_dict(result)
 
     async def get_server_mode(self) -> ServerMode:
         """Return details about the device server setup."""
         result = await self._local_client.request("getServerMode")
-        return ServerMode.parse_obj(result)
+        return ServerMode.from_dict(result)
 
     async def water_budget(self, budget) -> WaterBudget:
         """Return the water budget."""
         return await self._process_command(
             lambda resp: WaterBudget(resp["programCode"], resp["seasonalAdjust"]),
             "WaterBudgetRequest",
             budget,
@@ -356,15 +356,15 @@
     async def get_schedule_and_settings(self, stick_id: str) -> ScheduleAndSettings:
         """Request the schedule and settings from the cloud."""
         if not self._cloud_client:
             raise ValueError("Cloud client not configured")
         result = await self._cloud_client.request(
             "requestScheduleAndSettings", {"StickId": stick_id}
         )
-        return ScheduleAndSettings.parse_obj(result)
+        return ScheduleAndSettings.from_dict(result)
 
     async def get_weather_and_status(
         self, stick_id: str, country: str, zip_code: str
     ) -> WeatherAndStatus:
         """Request the weather and status of the device.
 
         The results include things like custom station names, program names, etc.
@@ -375,20 +375,20 @@
             "requestWeatherAndStatus",
             {
                 "Country": country,
                 "StickId": stick_id,
                 "ZipCode": zip_code,
             },
         )
-        return WeatherAndStatus.parse_obj(result)
+        return WeatherAndStatus.from_dict(result)
 
     async def get_combined_controller_state(self) -> ControllerState:
         """Return the combined controller state."""
         return await self._process_command(
-            lambda resp: ControllerState.parse_obj(resp),
+            lambda resp: ControllerState.from_dict(resp),
             "CombinedControllerStateRequest",
         )
 
     async def get_controller_firmware_version(self) -> ControllerFirmwareVersion:
         """Return the controller firmware version."""
         return await self._process_command(
             lambda resp: ControllerFirmwareVersion(
@@ -439,15 +439,15 @@
                             ) not in stations.stations.active_set:
                                 continue
                             schedule_data[key].append(entry)
                     elif key == "controllerInfo":
                         schedule_data[key].update(value)
                     else:
                         schedule_data[key].append(value)
-        return Schedule.parse_obj(schedule_data)
+        return Schedule.from_dict(schedule_data)
 
     async def get_schedule_command(self, command_code: str) -> dict[str, Any]:
         """Run the schedule command for the specified raw command code."""
         return await self._process_command(
             lambda resp: resp,
             "RetrieveScheduleRequest",
             command_code,
```

### Comparing `pyrainbird-4.0.2/pyrainbird/const.py` & `pyrainbird-5.0.0/pyrainbird/const.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-4.0.2/pyrainbird/data.py` & `pyrainbird-5.0.0/pyrainbird/data.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 """Data model for rainbird client api."""
 
 import datetime
 import logging
 from collections.abc import Iterable
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from enum import IntEnum
 from typing import Any, Optional
 
 from ical.iter import MergedIterable, SortableItem
 from ical.timespan import Timespan
-try:
-    from pydantic.v1 import BaseModel, Field, root_validator, validator
-except ImportError:
-    from pydantic import BaseModel, Field, root_validator, validator
+from mashumaro import DataClassDictMixin, field_options
+from mashumaro.types import SerializationStrategy
 
 from .const import DayOfWeek, ProgramFrequency
 from .resources import RAINBIRD_MODELS
 from .timeline import ProgramEvent, ProgramTimeline, create_recurrence, ProgramId
 
 _LOGGER = logging.getLogger(__name__)
 
@@ -189,95 +187,98 @@
 
 @dataclass
 class WaterBudget:
     program: int
     adjust: int
 
 
-class WifiParams(BaseModel):
+@dataclass
+class WifiParams(DataClassDictMixin):
     """Wifi parameters for the device."""
 
-    mac_address: Optional[str] = Field(alias="macAddress")
+    mac_address: Optional[str] = field(metadata=field_options(alias="macAddress"))
     """The mac address for the device, also referred to as the stick id."""
 
-    local_ip_address: Optional[str] = Field(alias="localIpAddress")
-    local_netmask: Optional[str] = Field(alias="localNetmask")
-    local_gateway: Optional[str] = Field(alias="localGateway")
+    local_ip_address: Optional[str] = field(metadata=field_options(alias="localIpAddress"))
+    local_netmask: Optional[str] = field(metadata=field_options(alias="localNetmask"))
+    local_gateway: Optional[str] = field(metadata=field_options(alias="localGateway"))
     rssi: Optional[int]
-    wifi_ssid: Optional[str] = Field(alias="wifiSsid")
-    wifi_password: Optional[str] = Field(alias="wifiPassword")
-    wifi_security: Optional[str] = Field(alias="wifiSecurity")
-    ap_timeout_no_lan: Optional[int] = Field(alias="apTimeoutNoLan")
-    ap_timeout_idle: Optional[int] = Field(alias="apTimeoutIdle")
-    ap_security: Optional[str] = Field(alias="apSecurity")
-    sick_version: Optional[str] = Field(alias="stickVersion")
+    wifi_ssid: Optional[str] = field(metadata=field_options(alias="wifiSsid"))
+    wifi_password: Optional[str] = field(metadata=field_options(alias="wifiPassword"))
+    wifi_security: Optional[str] = field(metadata=field_options(alias="wifiSecurity"))
+    ap_timeout_no_lan: Optional[int] = field(metadata=field_options(alias="apTimeoutNoLan"))
+    ap_timeout_idle: Optional[int] = field(metadata=field_options(alias="apTimeoutIdle"))
+    ap_security: Optional[str] = field(metadata=field_options(alias="apSecurity"))
+    sick_version: Optional[str] = field(metadata=field_options(alias="stickVersion"))
 
 
 class SoilType(IntEnum):
     """Soil type."""
 
     NONE = 0
     CLAY = 1
     SAND = 2
     OTHER = 3
 
 
-class ProgramInfo(BaseModel):
+@dataclass
+class ProgramInfo(DataClassDictMixin):
     """Program information for the device.
 
     The values are repeated once for each program.
     """
 
-    soil_types: list[SoilType] = Field(default_factory=list, alias="SoilTypes")
-    flow_rates: list[int] = Field(default_factory=list, alias="FlowRates")
-    flow_units: list[int] = Field(default_factory=list, alias="FlowUnits")
-
-    @root_validator(pre=True)
-    def _soil_type(cls, values: dict[str, Any]):
-        """Validate different ways the SoilTypes parameter is handled."""
+    soil_types: list[SoilType] = field(default_factory=list, metadata=field_options(alias="SoilTypes"))
+    flow_rates: list[int] = field(default_factory=list, metadata=field_options(alias="FlowRates"))
+    flow_units: list[int] = field(default_factory=list, metadata=field_options(alias="FlowUnits"))
+
+    @classmethod
+    def __pre_deserialize__(cls, values: dict[Any, Any]) -> dict[Any, Any]:
         if soil_type := values.get("soilTypes"):
             values["SoilTypes"] = soil_type
         return values
 
 
-class Settings(BaseModel):
+@dataclass
+class Settings(DataClassDictMixin):
     """Settings for the device."""
 
-    num_programs: int = Field(alias="numPrograms")
-    program_opt_out_mask: str = Field(alias="programOptOutMask")
-    global_disable: bool = Field(alias="globalDisable")
+    num_programs: int = field(metadata=field_options(alias="numPrograms"))
+    program_opt_out_mask: str = field(metadata=field_options(alias="programOptOutMask"))
+    global_disable: bool = field(metadata=field_options(alias="globalDisable"))
 
     code: Optional[str]
     """Zip code for the device."""
 
     country: Optional[str]
     """Country location of the device."""
 
     # Program information
-    soil_types: list[SoilType] = Field(default_factory=list, alias="SoilTypes")
-    flow_rates: list[int] = Field(default_factory=list, alias="FlowRates")
-    flow_units: list[int] = Field(default_factory=list, alias="FlowUnits")
-
-    @root_validator(pre=True)
-    def _soil_type(cls, values: dict[str, Any]):
-        """Validate different ways the SoilTypes parameter is handled."""
+    soil_types: list[SoilType] = field(default_factory=list, metadata=field_options(alias="SoilTypes"))
+    flow_rates: list[int] = field(default_factory=list, metadata=field_options(alias="FlowRates"))
+    flow_units: list[int] = field(default_factory=list, metadata=field_options(alias="FlowUnits"))
+
+    @classmethod
+    def __pre_deserialize__(cls, values: dict[Any, Any]) -> dict[Any, Any]:
         if soil_type := values.get("soilTypes"):
             values["SoilTypes"] = soil_type
         return values
 
 
-class WeatherAdjustmentMask(BaseModel):
+@dataclass
+class WeatherAdjustmentMask(DataClassDictMixin):
     """Weather adjustment mask response."""
 
-    num_programs: int = Field(alias="numPrograms")
-    program_opt_out_mask: str = Field(alias="programOptOutMask")
-    global_disable: bool = Field(alias="globalDisable")
+    num_programs: int = field(metadata=field_options(alias="numPrograms"))
+    program_opt_out_mask: str = field(metadata=field_options(alias="programOptOutMask"))
+    global_disable: bool = field(metadata=field_options(alias="globalDisable"))
 
 
-class ZipCode(BaseModel):
+@dataclass
+class ZipCode(DataClassDictMixin):
     """Get the zip code of the device."""
 
     code: Optional[str]
     """Zip code for the device."""
 
     country: Optional[str]
     """Country location of the device."""
@@ -297,188 +298,240 @@
 
     @property
     def settings(self) -> Optional[Settings]:
         """Return device settings."""
         return self._settings
 
     @classmethod
-    def parse_obj(cls, data: dict[str, Any]):
+    def from_dict(cls, data: dict[str, Any]):
         """Parse a ScheduleAndSettings from an API response."""
         status = data.get("status", None)
-        settings = Settings.parse_obj(data["settings"]) if "settings" in data else None
+        settings = Settings.from_dict(data["settings"]) if "settings" in data else None
         return ScheduleAndSettings(status, settings)
 
 
-class Controller(BaseModel):
+@dataclass
+class Controller(DataClassDictMixin):
     """Settings for the controller."""
 
-    available_stations: list[int] = Field(
-        alias="availableStations", default_factory=list
+    available_stations: list[int] = field(
+        metadata=field_options(alias="availableStations"), default_factory=list
     )
-    custom_name: Optional[str] = Field(alias="customName")
-    custom_program_names: dict[str, str] = Field(
-        alias="customProgramNames", default_factory=dict
+    custom_name: Optional[str] = field(metadata=field_options(alias="customName"), default=None)
+    custom_program_names: dict[str, str] = field(
+        metadata=field_options(alias="customProgramNames"), default_factory=dict
     )
-    custom_station_names: dict[str, str] = Field(
-        alias="customStationNames", default_factory=dict
+    custom_station_names: dict[str, str] = field(
+        metadata=field_options(alias="customStationNames"), default_factory=dict
     )
 
 
-class Forecast(BaseModel):
+@dataclass
+class Forecast(DataClassDictMixin):
     """Weather forecast data from the cloud API."""
 
-    date_time: Optional[int] = Field(alias="dateTime")
+    date_time: Optional[int] = field(metadata=field_options(alias="dateTime"))
     icon: Optional[str]
     description: Optional[str]
     high: Optional[int]
     low: Optional[int]
     chance_of_rain: Optional[int]
     precip: Optional[float]
 
 
-class Weather(BaseModel):
+@dataclass
+class Weather(DataClassDictMixin):
     """Weather settings from the cloud API."""
 
     city: Optional[str]
-    forecast: list[Forecast] = Field(default_factory=list)
-    location: Optional[str]
-    time_zone_id: Optional[str] = Field(alias="timeZoneId")
-    time_zone_raw_offset: Optional[str] = Field(alias="timeZoneRawOffset")
+    forecast: list[Forecast] = field(default_factory=list)
+    location: Optional[str] = None
+    time_zone_id: Optional[str] = field(metadata=field_options(alias="timeZoneId"), default=None)
+    time_zone_raw_offset: Optional[str] = field(metadata=field_options(alias="timeZoneRawOffset"), default=None)
 
 
-class WeatherAndStatus(BaseModel):
+@dataclass
+class WeatherAndStatus(DataClassDictMixin):
     """Weather and status from the cloud API."""
 
-    stick_id: Optional[str] = Field(alias="StickId")
-    controller: Optional[Controller] = Field(alias="Controller")
-    forecasted_rain: Optional[dict[str, Any]] = Field(alias="ForecastedRain")
-    weather: Optional[Weather] = Field(alias="Weather")
+    stick_id: Optional[str] = field(metadata=field_options(alias="StickId"))
+    controller: Optional[Controller] = field(metadata=field_options(alias="Controller"))
+    forecasted_rain: Optional[dict[str, Any]] = field(metadata=field_options(alias="ForecastedRain"))
+    weather: Optional[Weather] = field(metadata=field_options(alias="Weather"))
 
 
-class NetworkStatus(BaseModel):
+@dataclass
+class NetworkStatus(DataClassDictMixin):
     """Get the device network status."""
 
-    network_up: bool = Field(alias="networkUp")
-    internet_up: bool = Field(alias="internetUp")
+    network_up: bool = field(metadata=field_options(alias="networkUp"))
+    internet_up: bool = field(metadata=field_options(alias="internetUp"))
 
 
-class ServerMode(BaseModel):
+@dataclass
+class ServerMode(DataClassDictMixin):
     """Details about the device server connection."""
 
-    server_mode: bool = Field(alias="serverMode")
-    check_in_interval: int = Field(alias="checkInInterval")
-    server_url: str = Field(alias="serverUrl")
-    relay_timeout: int = Field(alias="relayTimeout")
-    missed_checkins: int = Field(alias="missedCheckins")
-
+    server_mode: bool = field(metadata=field_options(alias="serverMode"))
+    check_in_interval: int = field(metadata=field_options(alias="checkInInterval"))
+    server_url: str = field(metadata=field_options(alias="serverUrl"))
+    relay_timeout: int = field(metadata=field_options(alias="relayTimeout"))
+    missed_checkins: int = field(metadata=field_options(alias="missedCheckins"))
+
+
+class DeviceTime(SerializationStrategy):
+    """Validate different ways the device time parameter is handled."""
+
+    def serialize(self, value: Any) -> Any:
+        raise ValueError("serialize not implemented")
+
+    def deserialize(self, values: dict[str, Any]) -> datetime.datetime:
+        """Deserialize the device time fields."""
+        for f in {"year", "month", "day", "hour", "minute", "second"}:
+            if f not in values:
+                raise ValueError(f"Missing field '{f}' in values")
+        return datetime.datetime(
+            int(values["year"]),
+            int(values["month"]),
+            int(values["day"]),
+            int(values["hour"]),
+            int(values["minute"]),
+            int(values["second"]),
+        )
 
-class ControllerState(BaseModel):
+@dataclass
+class ControllerState(DataClassDictMixin):
     """Details about the controller state."""
 
-    delay_setting: int = Field(alias="delaySetting")
+    delay_setting: int = field(metadata=field_options(alias="delaySetting"))
     """Number of days that irrigation is paused."""
 
-    sensor_state: int = Field(alias="sensorState")
+    sensor_state: int = field(metadata=field_options(alias="sensorState"))
     """Rain sensor status."""
 
-    irrigation_state: int = Field(alias="irrigationState")
+    irrigation_state: int = field(metadata=field_options(alias="irrigationState"))
     """State of irrigation."""
 
-    seasonal_adjust: int = Field(alias="seasonalAdjust")
-    remaining_runtime: int = Field(alias="remainingRuntime")
+    seasonal_adjust: int = field(metadata=field_options(alias="seasonalAdjust"))
+    remaining_runtime: int = field(metadata=field_options(alias="remainingRuntime"))
 
     # TODO: Likely need to make this a mask w/ States
-    active_station: int = Field(alias="activeStation")
+    active_station: int = field(metadata=field_options(alias="activeStation"))
 
-    device_time: datetime.datetime
+    device_time: datetime.datetime = field(metadata=field_options(serialization_strategy=DeviceTime()))
 
-    @root_validator(pre=True)
-    def _device_time(cls, values: dict[str, Any]):
-        """Validate different ways the SoilTypes parameter is handled."""
-        for field in {"year", "month", "day", "hour", "minute", "second"}:
-            if field not in values:
-                raise ValueError(f"Missing field '{field}' in values")
-        values["device_time"] = datetime.datetime(
-            int(values["year"]),
-            int(values["month"]),
-            int(values["day"]),
-            int(values["hour"]),
-            int(values["minute"]),
-            int(values["second"]),
-        )
-        return values
+    @classmethod
+    def __pre_deserialize__(cls, d: dict[Any, Any]) -> dict[Any, Any]:
+        d["device_time"] = {
+            k: d[k]
+            for k in ("year", "month", "day", "hour", "minute", "second")
+        }
+        return d
 
 
-class ControllerInfo(BaseModel):
+@dataclass
+class ControllerInfo(DataClassDictMixin):
     """Data about the controller settings."""
 
-    station_delay: int = Field(alias="stationDelay", default=0)
-    rain_delay: int = Field(alias="rainDelay", default=0)
-    rain_sensor: bool = Field(alias="rainSensor", default=False)
+    station_delay: int = field(metadata=field_options(alias="stationDelay"), default=0)
+    rain_delay: int = field(metadata=field_options(alias="rainDelay"), default=0)
+    rain_sensor: bool = field(metadata=field_options(alias="rainSensor"), default=False)
 
     @property
     def delay_days(self) -> int:
         """Return the amount of delay before starting the schedule."""
         return max(self.station_delay, self.rain_delay)
 
 
-class ZoneDuration(BaseModel):
+@dataclass
+class ZoneDuration(DataClassDictMixin):
     """Program runtime for a specific zone."""
 
     zone: int
     """Zone the program irrigates."""
 
     duration: datetime.timedelta
     """Runtime of the program in the specified zone."""
 
     @property
     def name(self) -> str:
         return f"Zone {self.zone}"
 
-    @validator("zone", pre=True)
-    def _parse_zone(cls, value: int) -> datetime.timedelta:
-        """Parse the zone value."""
-        return value + 1
-
-    @validator("duration", pre=True)
-    def _parse_duration(cls, value: int) -> datetime.timedelta:
-        """Parse the zone duration values."""
-        return datetime.timedelta(minutes=value)
+    @classmethod
+    def __pre_deserialize__(cls, values: dict[Any, Any]) -> dict[Any, Any]:
+        if duration := values.get("duration"):
+            values["duration"] = duration * 60  #datetime.timedelta(minutes=duration)
+        return values
+
+
+class TimeSerializationStrategy(SerializationStrategy):
+    """Validate different ways the device time parameter is handled."""
+
+    def serialize(self, value: Any) -> Any:
+        raise ValueError("Serialize not implemented")
 
+    def deserialize(self, starts: list[int]) -> list[datetime.time]:
+        """Deserialize the device time fields."""
+        result: list[datetime.time] = []
+        for start in starts:
+            if start == 65535:
+                continue
+            result.append(datetime.time(hour=int(start / 60), minute=start % 60))
+        return result
+
+
+
+
+class DayOfWeekSerializationStrategy(SerializationStrategy):
+    """Validate different ways the device time parameter is handled."""
 
-class Program(BaseModel):
+    def serialize(self, value: Any) -> str:
+        raise ValueError("Serialization not implemented")
+
+    def deserialize(self, mask: int) -> list[DayOfWeek]:
+        """Deserialize the device time fields."""
+        _LOGGER.debug("DayOfWeekSerializationStrategy=%s", mask)
+        result: set[DayOfWeek] = set()
+        for day in range(0, 7):
+            if mask & (1 << day):
+                result.add(DayOfWeek(day))
+        return result
+
+
+@dataclass
+class Program(DataClassDictMixin):
     """Details about a program.
 
     The frequency determines which fields of the program are relevant. A
     CUSTOM program looks at days_of_week. A CYCLIC program looks at period.
     ODD/EVEN are odd/even days of the month.
     """
 
     program: int
     """The program number."""
 
     frequency: ProgramFrequency
     """Determines how often the program runs."""
 
-    days_of_week: set[DayOfWeek] = Field(alias="daysOfWeekMask", default_factory=set)
+    days_of_week: set[DayOfWeek] = field(metadata=field_options(alias="daysOfWeekMask", serialization_strategy=DayOfWeekSerializationStrategy()), default_factory=set)
     """For a CUSTOM program determines the days of the week."""
 
-    period: Optional[int]
+    period: Optional[int] = None
     """For a CYCLIC program determines how often to run."""
 
-    synchro: Optional[int]
+    synchro: Optional[int] = None
     """Days from today before starting the first day of the program."""
 
-    starts: list[datetime.time] = Field(default_factory=list)
+    starts: list[datetime.time] = field(default_factory=list, metadata=field_options(serialization_strategy=TimeSerializationStrategy()))
     """Time of day the program starts."""
 
-    durations: list[ZoneDuration] = Field(default_factory=list)
+    durations: list[ZoneDuration] = field(default_factory=list)
     """Durations for run times for each zone."""
 
-    controller_info: Optional[ControllerInfo] = Field(alias="controllerInfo")
+    controller_info: Optional[ControllerInfo] = field(metadata=field_options(alias="controllerInfo"), default=None)
     """Information about the controller as input into the programs."""
 
     @property
     def name(self) -> str:
         """Name of the program."""
         letter = chr(ord("A") + self.program)
         return f"PGM {letter}"
@@ -540,52 +593,30 @@
         return total
 
     @property
     def delay_days(self) -> int:
         """Return the number of delays programs are delayed."""
         return self.controller_info.delay_days if self.controller_info else 0
 
-    @root_validator(pre=True)
-    def _clear_other_fields(cls, values: dict[str, Any]) -> set[DayOfWeek]:
-        """Clear fields unrelated to the current frequency."""
-        if ProgramFrequency.CUSTOM != values.get("frequency"):
-            if "daysOfWeekMask" in values:
-                del values["daysOfWeekMask"]
-        if ProgramFrequency.CYCLIC != values.get("frequency"):
-            if "period" in values:
-                del values["period"]
-        return values
-
-    @validator("days_of_week", pre=True)
-    def _parse_days_of_week(cls, mask: int) -> set[DayOfWeek]:
-        """Parse the days of week bitmask to a enum set."""
-        result: set[DayOfWeek] = set()
-        for day in range(0, 7):
-            if mask & (1 << day):
-                result.add(DayOfWeek(day))
-        return result
+    def __post_init__(self):
+        if self.frequency != ProgramFrequency.CUSTOM:
+            self.days_of_week = set()
+        if self.frequency != ProgramFrequency.CYCLIC:
+            self.period = None
 
-    @validator("starts", pre=True)
-    def _parse_starts(cls, starts: list[int]) -> set[DayOfWeek]:
-        """Parse the days of week bitmask to a enum set."""
-        result: list[datetime.time] = []
-        for start in starts:
-            if start == 65535:
-                continue
-            result.append(datetime.time(hour=int(start / 60), minute=start % 60))
-        return result
 
 
-class Schedule(BaseModel):
+@dataclass
+class Schedule(DataClassDictMixin):
     """Details about program schedules."""
 
-    controller_info: Optional[ControllerInfo] = Field(alias="controllerInfo")
+    controller_info: Optional[ControllerInfo] = field(metadata=field_options(alias="controllerInfo"))
     """Information about the controller used in the schedule."""
 
-    programs: list[Program] = Field(alias="programInfo")
+    programs: list[Program] = field(metadata=field_options(alias="programInfo"))
     """Details about the currently scheduled programs."""
 
     @property
     def timeline(self) -> ProgramTimeline:
         """Return a timeline of all programs."""
         return self.timeline_tz(datetime.datetime.now().tzinfo)
 
@@ -611,38 +642,30 @@
         return ProgramTimeline(MergedIterable(iters))
 
     @property
     def delay_days(self) -> int:
         """Return the number of delays programs are delayed."""
         return self.controller_info.delay_days if self.controller_info else 0
 
-    @root_validator(pre=True)
-    def _parse_start_info(cls, values: dict[str, Any]):
+    @classmethod
+    def __pre_deserialize__(cls, values: dict[Any, Any]) -> dict[Any, Any]:
         """Parse the input values from the response into a usable format."""
         programs = values.get("programStartInfo", [])
         if not programs:
             return values
-        for program_start_info in values.get("programStartInfo"):
+        for program_start_info in programs:
             program = program_start_info.get("program")
             if program is None:
                 continue
             values["programInfo"][program]["starts"] = program_start_info.get(
                 "startTime", []
             )
             values["programInfo"][program]["controllerInfo"] = values.get(
                 "controllerInfo"
             )
-        return values
-
-    @root_validator(pre=True)
-    def _parse_durations(cls, values: dict[str, Any]):
-        """Parse the input values from the response into a usable format."""
-        programs = values.get("programInfo", [])
-        if not programs:
-            return values
         for program in range(0, len(programs)):
             values["programInfo"][program]["durations"] = []
         for zone_durations in values.get("durations", []):
             zone = zone_durations.get("zone")
             if zone is None:
                 continue
             duration_values = zone_durations.get("durations", [])
@@ -656,13 +679,12 @@
                 continue
             for program in range(0, len(programs)):
                 duration = duration_values[program]
                 if not duration:
                     continue
                 values["programInfo"][program]["durations"].append(
                     {
-                        "zone": zone,
+                        "zone": zone + 1,
                         "duration": duration,
                     }
                 )
-
         return values
```

### Comparing `pyrainbird-4.0.2/pyrainbird/encryption.py` & `pyrainbird-5.0.0/pyrainbird/encryption.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-4.0.2/pyrainbird/rainbird.py` & `pyrainbird-5.0.0/pyrainbird/rainbird.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-4.0.2/pyrainbird/resources/__init__.py` & `pyrainbird-5.0.0/pyrainbird/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-4.0.2/pyrainbird/resources/models.yaml` & `pyrainbird-5.0.0/pyrainbird/resources/models.yaml`

 * *Files identical despite different names*

### Comparing `pyrainbird-4.0.2/pyrainbird/resources/sipcommands.yaml` & `pyrainbird-5.0.0/pyrainbird/resources/sipcommands.yaml`

 * *Files identical despite different names*

### Comparing `pyrainbird-4.0.2/pyrainbird/timeline.py` & `pyrainbird-5.0.0/pyrainbird/timeline.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-4.0.2/pyrainbird.egg-info/PKG-INFO` & `pyrainbird-5.0.0/pyrainbird.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyrainbird
-Version: 4.0.2
+Version: 5.0.0
 Summary: Rain Bird Controller
 Home-page: https://github.com/allenporter/pyrainbird
 Author: J.J.Barrancos
 Author-email: jordy@fusion-ict.nl
 License: MIT
 Keywords: Rain Bird
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pycryptodome>=3.16.0
 Requires-Dist: requests>=2.22.0
 Requires-Dist: PyYAML>=5.4
-Requires-Dist: pydantic>=1.10.4
+Requires-Dist: mashumaro>=3.12
 Requires-Dist: python-dateutil>=2.8.2
 Requires-Dist: ical>=4.2.9
 Requires-Dist: aiohttp_retry>=2.8.3
 
 Python module for interacting with [WiFi LNK](https://www.rainbird.com/products/module-wi-fi-lnk) module of the Rain Bird Irrigation system. This project has no affiliation with Rain Bird.
 
 This module communicates directly towards the IP Address of the WiFi module. You can start/stop the irrigation, get the currently active zone, and other controller settings. This library currently only has very limited cloud support. Also there are a number of Rain Bird devices with very different command APIs.
```

### Comparing `pyrainbird-4.0.2/pyrainbird.egg-info/SOURCES.txt` & `pyrainbird-5.0.0/pyrainbird.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrainbird-4.0.2/setup.cfg` & `pyrainbird-5.0.0/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyrainbird
-version = 4.0.2
+version = 5.0.0
 description = Rain Bird Controller
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/allenporter/pyrainbird
 author = J.J.Barrancos
 author_email = jordy@fusion-ict.nl
 license = MIT
@@ -14,15 +14,15 @@
 [options]
 packages = find:
 python_requires = >=3.10
 install_requires = 
 	pycryptodome>=3.16.0
 	requests>=2.22.0
 	PyYAML>=5.4
-	pydantic>=1.10.4
+	mashumaro>=3.12
 	python-dateutil>=2.8.2
 	ical>=4.2.9
 	aiohttp_retry>=2.8.3
 install_package_data = True
 package_dir = 
 	= .
```

### Comparing `pyrainbird-4.0.2/tests/test_async_client.py` & `pyrainbird-5.0.0/tests/test_async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -447,15 +447,15 @@
             "apSecurity": "unknown",
             "stickVersion": "Rain Bird Stick Rev C/1.63",
         },
         "id": 1234,
     }
     encrypt_response(payload)
     params = await controller.get_wifi_params()
-    assert params.dict() == {
+    assert params.to_dict() == {
         "ap_security": "unknown",
         "ap_timeout_idle": 20,
         "ap_timeout_no_lan": 20,
         "local_gateway": "192.168.1.1",
         "local_ip_address": "192.168.1.10",
         "local_netmask": "255.255.255.0",
         "mac_address": "11:22:33:44:55:66",
```

### Comparing `pyrainbird-4.0.2/tests/test_data.py` & `pyrainbird-5.0.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-4.0.2/tests/test_rainbird.py` & `pyrainbird-5.0.0/tests/test_rainbird.py`

 * *Files identical despite different names*

