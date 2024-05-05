# Comparing `tmp/goodwe-0.3.3.tar.gz` & `tmp/goodwe-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goodwe-0.3.3.tar", last modified: Sun Apr 14 20:20:43 2024, max compression
+gzip compressed data, was "goodwe-0.3.4.tar", last modified: Sun May  5 08:45:27 2024, max compression
```

## Comparing `goodwe-0.3.3.tar` & `goodwe-0.3.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:20:43.465417 goodwe-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-14 20:20:36.000000 goodwe-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-14 20:20:43.465417 goodwe-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-14 20:20:36.000000 goodwe-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 20:20:40.000000 goodwe-0.3.3/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:20:43.461417 goodwe-0.3.3/goodwe/
--rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-04-14 20:20:36.000000 goodwe-0.3.3/goodwe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-04-14 20:20:36.000000 goodwe-0.3.3/goodwe/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    10581 2024-04-14 20:20:36.000000 goodwe-0.3.3/goodwe/dt.py
--rw-r--r--   0 runner    (1001) docker     (127)    22434 2024-04-14 20:20:36.000000 goodwe-0.3.3/goodwe/es.py
--rw-r--r--   0 runner    (1001) docker     (127)    39228 2024-04-14 20:20:36.000000 goodwe-0.3.3/goodwe/et.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-14 20:20:36.000000 goodwe-0.3.3/goodwe/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10325 2024-04-14 20:20:36.000000 goodwe-0.3.3/goodwe/inverter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-14 20:20:36.000000 goodwe-0.3.3/goodwe/modbus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-14 20:20:36.000000 goodwe-0.3.3/goodwe/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13162 2024-04-14 20:20:36.000000 goodwe-0.3.3/goodwe/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    36845 2024-04-14 20:20:36.000000 goodwe-0.3.3/goodwe/sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:20:43.465417 goodwe-0.3.3/goodwe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-14 20:20:43.000000 goodwe-0.3.3/goodwe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-14 20:20:43.000000 goodwe-0.3.3/goodwe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 20:20:43.000000 goodwe-0.3.3/goodwe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-14 20:20:43.000000 goodwe-0.3.3/goodwe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-14 20:20:36.000000 goodwe-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-14 20:20:43.465417 goodwe-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:20:43.465417 goodwe-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    20434 2024-04-14 20:20:36.000000 goodwe-0.3.3/tests/test_dt.py
--rw-r--r--   0 runner    (1001) docker     (127)    29085 2024-04-14 20:20:36.000000 goodwe-0.3.3/tests/test_es.py
--rw-r--r--   0 runner    (1001) docker     (127)    66856 2024-04-14 20:20:36.000000 goodwe-0.3.3/tests/test_et.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-14 20:20:36.000000 goodwe-0.3.3/tests/test_modbus.py
--rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-04-14 20:20:36.000000 goodwe-0.3.3/tests/test_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    13867 2024-04-14 20:20:36.000000 goodwe-0.3.3/tests/test_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:45:27.356207 goodwe-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-05 08:45:19.000000 goodwe-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-05-05 08:45:27.356207 goodwe-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-05 08:45:19.000000 goodwe-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-05 08:45:24.000000 goodwe-0.3.4/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:45:27.356207 goodwe-0.3.4/goodwe/
+-rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-05-05 08:45:19.000000 goodwe-0.3.4/goodwe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-05-05 08:45:19.000000 goodwe-0.3.4/goodwe/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10581 2024-05-05 08:45:19.000000 goodwe-0.3.4/goodwe/dt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22650 2024-05-05 08:45:19.000000 goodwe-0.3.4/goodwe/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39703 2024-05-05 08:45:19.000000 goodwe-0.3.4/goodwe/et.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-05 08:45:19.000000 goodwe-0.3.4/goodwe/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10342 2024-05-05 08:45:19.000000 goodwe-0.3.4/goodwe/inverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-05-05 08:45:19.000000 goodwe-0.3.4/goodwe/modbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-05 08:45:19.000000 goodwe-0.3.4/goodwe/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13162 2024-05-05 08:45:19.000000 goodwe-0.3.4/goodwe/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36990 2024-05-05 08:45:19.000000 goodwe-0.3.4/goodwe/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:45:27.356207 goodwe-0.3.4/goodwe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-05-05 08:45:27.000000 goodwe-0.3.4/goodwe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-05 08:45:27.000000 goodwe-0.3.4/goodwe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 08:45:27.000000 goodwe-0.3.4/goodwe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-05 08:45:27.000000 goodwe-0.3.4/goodwe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-05 08:45:19.000000 goodwe-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-05 08:45:27.360207 goodwe-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:45:27.356207 goodwe-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    20437 2024-05-05 08:45:19.000000 goodwe-0.3.4/tests/test_dt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29085 2024-05-05 08:45:19.000000 goodwe-0.3.4/tests/test_es.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66871 2024-05-05 08:45:19.000000 goodwe-0.3.4/tests/test_et.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-05 08:45:19.000000 goodwe-0.3.4/tests/test_modbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-05-05 08:45:19.000000 goodwe-0.3.4/tests/test_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13861 2024-05-05 08:45:19.000000 goodwe-0.3.4/tests/test_sensor.py
```

### Comparing `goodwe-0.3.3/LICENSE` & `goodwe-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.3/PKG-INFO` & `goodwe-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goodwe
-Version: 0.3.3
+Version: 0.3.4
 Summary: Read data from GoodWe inverter via local network
 Home-page: https://github.com/marcelblijleven/goodwe
 Author: Martin Letenay, Marcel Blijleven
 Author-email: 'marcelblijleven@gmail.com
 License: MIT
 Keywords: GoodWe,Solar Panel,Inverter,Photovoltaics,PV
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `goodwe-0.3.3/README.md` & `goodwe-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.3/goodwe/__init__.py` & `goodwe-0.3.4/goodwe/__init__.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.3/goodwe/const.py` & `goodwe-0.3.4/goodwe/const.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.3/goodwe/dt.py` & `goodwe-0.3.4/goodwe/dt.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.3/goodwe/es.py` & `goodwe-0.3.4/goodwe/es.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         Byte("effective_work_mode", 77, "Effective Work Mode code"),
         Integer("effective_relay_control", 78, "Effective Relay Control", "", None),
         Byte("grid_in_out", 80, "On-grid Mode code", "", Kind.GRID),
         Enum("grid_in_out_label", 80, GRID_IN_OUT_MODES, "On-grid Mode", Kind.GRID),
         Power("pback_up", 81, "Back-up Power", Kind.UPS),
         # pload + pback_up
         Calculated("plant_power",
-                   lambda data: round(read_bytes2(data, 47) + read_bytes2(data, 81)),
+                   lambda data: round(read_bytes2(data, 47, 0) + read_bytes2(data, 81, 0)),
                    "Plant Power", "W", Kind.AC),
         Decimal("meter_power_factor", 83, 1000, "Meter Power Factor", "", Kind.GRID),  # modbus 0x531
         # Integer("xx85", 85, "Unknown sensor@85"),
         # Integer("xx87", 87, "Unknown sensor@87"),
         Long("diagnose_result", 89, "Diag Status Code"),
         EnumBitmap4("diagnose_result_label", 89, DIAG_STATUS_CODES, "Diag Status"),
         # Energy4("e_total_exp", 93, "Total Energy (export)", Kind.GRID),
@@ -131,15 +131,15 @@
         Integer("shadow_scan", 16, "Shadow Scan", "", Kind.PV),
         Integer("grid_export", 18, "Export Limit Enabled", "", Kind.GRID),
         Integer("capacity", 22, "Capacity"),
         Decimal("charge_v", 24, 10, "Charge Voltage", "V"),
         Integer("charge_i", 26, "Charge Current", "A", ),
         Integer("discharge_i", 28, "Discharge Current", "A", ),
         Decimal("discharge_v", 30, 10, "Discharge Voltage", "V"),
-        Calculated("dod", lambda data: 100 - read_bytes2(data, 32), "Depth of Discharge", "%"),
+        Calculated("dod", lambda data: 100 - read_bytes2(data, 32, 0), "Depth of Discharge", "%"),
         Integer("battery_activated", 34, "Battery Activated"),
         Integer("bp_off_grid_charge", 36, "BP Off-grid Charge"),
         Integer("bp_pv_discharge", 38, "BP PV Discharge"),
         Integer("bp_bms_protocol", 40, "BP BMS Protocol"),
         Integer("power_factor", 42, "Power Factor"),
         Integer("grid_export_limit", 52, "Grid Export Limit", "W", Kind.GRID),
         Integer("battery_soc_protection", 56, "Battery SoC Protection", "", Kind.BAT),
@@ -281,27 +281,33 @@
             await self._read_from_socket(
                 Aa55ProtocolCommand("033502" + "{:04x}".format(export_limit), "03b5")
             )
 
     async def get_operation_modes(self, include_emulated: bool) -> Tuple[OperationMode, ...]:
         result = [e for e in OperationMode]
         result.remove(OperationMode.PEAK_SHAVING)
+        result.remove(OperationMode.SELF_USE)
         if not include_emulated:
             result.remove(OperationMode.ECO_CHARGE)
             result.remove(OperationMode.ECO_DISCHARGE)
         return tuple(result)
 
     async def get_operation_mode(self) -> OperationMode:
-        mode = OperationMode(await self.read_setting('work_mode'))
+        mode_id = await self.read_setting('work_mode')
+        try:
+            mode = OperationMode(mode_id)
+        except ValueError:
+            logger.debug("Unknown work_mode value %d", mode_id)
+            return None
         if OperationMode.ECO != mode:
             return mode
-        ecomode = await self.read_setting('eco_mode_1')
-        if ecomode.is_eco_charge_mode():
+        eco_mode = await self.read_setting('eco_mode_1')
+        if eco_mode.is_eco_charge_mode():
             return OperationMode.ECO_CHARGE
-        elif ecomode.is_eco_discharge_mode():
+        elif eco_mode.is_eco_discharge_mode():
             return OperationMode.ECO_DISCHARGE
         else:
             return OperationMode.ECO
 
     async def set_operation_mode(self, operation_mode: OperationMode, eco_mode_power: int = 100,
                                  eco_mode_soc: int = 100) -> None:
         if operation_mode == OperationMode.GENERAL:
```

### Comparing `goodwe-0.3.3/goodwe/et.py` & `goodwe-0.3.4/goodwe/et.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,18 +31,18 @@
         Power4("ppv3", 35113, "PV3 Power", Kind.PV),
         Voltage("vpv4", 35115, "PV4 Voltage", Kind.PV),
         Current("ipv4", 35116, "PV4 Current", Kind.PV),
         Power4("ppv4", 35117, "PV4 Power", Kind.PV),
         # ppv1 + ppv2 + ppv3 + ppv4
         Calculated("ppv",
                    lambda data:
-                   max(0, read_bytes4(data, 35105)) +
-                   max(0, read_bytes4(data, 35109)) +
-                   max(0, read_bytes4(data, 35113)) +
-                   max(0, read_bytes4(data, 35117)),
+                   max(0, read_bytes4(data, 35105, 0)) +
+                   max(0, read_bytes4(data, 35109, 0)) +
+                   max(0, read_bytes4(data, 35113, 0)) +
+                   max(0, read_bytes4(data, 35117, 0)),
                    "PV Power", "W", Kind.PV),
         ByteH("pv4_mode", 35119, "PV4 Mode code", "", Kind.PV),
         EnumH("pv4_mode_label", 35119, PV_MODES, "PV4 Mode", Kind.PV),
         ByteL("pv3_mode", 35119, "PV3 Mode code", "", Kind.PV),
         EnumL("pv3_mode_label", 35119, PV_MODES, "PV3 Mode", Kind.PV),
         ByteH("pv2_mode", 35120, "PV2 Mode code", "", Kind.PV),
         EnumH("pv2_mode_label", 35120, PV_MODES, "PV2 Mode", Kind.PV),
@@ -141,18 +141,18 @@
         Energy4("e_bat_discharge_total", 35209, "Total Battery Discharge", Kind.BAT),
         Energy("e_bat_discharge_day", 35211, "Today Battery Discharge", Kind.BAT),
         Long("diagnose_result", 35220, "Diag Status Code"),
         EnumBitmap4("diagnose_result_label", 35220, DIAG_STATUS_CODES, "Diag Status"),
         # ppv1 + ppv2 + ppv3 + ppv4 + pbattery1 - active_power
         Calculated("house_consumption",
                    lambda data:
-                   read_bytes4(data, 35105) +
-                   read_bytes4(data, 35109) +
-                   read_bytes4(data, 35113) +
-                   read_bytes4(data, 35117) +
+                   read_bytes4(data, 35105, 0) +
+                   read_bytes4(data, 35109, 0) +
+                   read_bytes4(data, 35113, 0) +
+                   read_bytes4(data, 35117, 0) +
                    read_bytes4_signed(data, 35182) -
                    read_bytes2_signed(data, 35140),
                    "House Consumption", "W", Kind.AC),
     )
 
     # Modbus registers from offset 0x9088 (37000)
     __all_sensors_battery: Tuple[Sensor, ...] = (
@@ -600,27 +600,34 @@
         if export_limit >= 0:
             await self.write_setting('grid_export_limit', export_limit)
 
     async def get_operation_modes(self, include_emulated: bool) -> Tuple[OperationMode, ...]:
         result = [e for e in OperationMode]
         if not self._has_peak_shaving:
             result.remove(OperationMode.PEAK_SHAVING)
+        if not is_745_platform(self):
+            result.remove(OperationMode.SELF_USE)
         if not include_emulated:
             result.remove(OperationMode.ECO_CHARGE)
             result.remove(OperationMode.ECO_DISCHARGE)
         return tuple(result)
 
     async def get_operation_mode(self) -> OperationMode:
-        mode = OperationMode(await self.read_setting('work_mode'))
+        mode_id = await self.read_setting('work_mode')
+        try:
+            mode = OperationMode(mode_id)
+        except ValueError:
+            logger.debug("Unknown work_mode value %d", mode_id)
+            return None
         if OperationMode.ECO != mode:
             return mode
-        ecomode = await self.read_setting('eco_mode_1')
-        if ecomode.is_eco_charge_mode():
+        eco_mode = await self.read_setting('eco_mode_1')
+        if eco_mode.is_eco_charge_mode():
             return OperationMode.ECO_CHARGE
-        elif ecomode.is_eco_discharge_mode():
+        elif eco_mode.is_eco_discharge_mode():
             return OperationMode.ECO_DISCHARGE
         else:
             return OperationMode.ECO
 
     async def set_operation_mode(self, operation_mode: OperationMode, eco_mode_power: int = 100,
                                  eco_mode_soc: int = 100) -> None:
         if operation_mode == OperationMode.GENERAL:
@@ -640,14 +647,18 @@
         elif operation_mode == OperationMode.ECO:
             await self.write_setting('work_mode', 3)
             await self._set_offline(False)
         elif operation_mode == OperationMode.PEAK_SHAVING:
             await self.write_setting('work_mode', 4)
             await self._set_offline(False)
             await self._clear_battery_mode_param()
+        elif operation_mode == OperationMode.SELF_USE:
+            await self.write_setting('work_mode', 5)
+            await self._set_offline(False)
+            await self._clear_battery_mode_param()
         elif operation_mode in (OperationMode.ECO_CHARGE, OperationMode.ECO_DISCHARGE):
             if eco_mode_power < 0 or eco_mode_power > 100:
                 raise ValueError()
             if eco_mode_soc < 0 or eco_mode_soc > 100:
                 raise ValueError()
 
             eco_mode: EcoMode | Sensor = self._settings.get('eco_mode_1')
```

### Comparing `goodwe-0.3.3/goodwe/exceptions.py` & `goodwe-0.3.4/goodwe/exceptions.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.3/goodwe/inverter.py` & `goodwe-0.3.4/goodwe/inverter.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,16 +72,17 @@
     """
 
     GENERAL = 0
     OFF_GRID = 1
     BACKUP = 2
     ECO = 3
     PEAK_SHAVING = 4
-    ECO_CHARGE = 10
-    ECO_DISCHARGE = 11
+    SELF_USE = 5
+    ECO_CHARGE = 98
+    ECO_DISCHARGE = 99
 
 
 class Inverter(ABC):
     """
     Common superclass for various inverter models implementations.
     Represents the inverter state and its basic behavior
     """
```

### Comparing `goodwe-0.3.3/goodwe/modbus.py` & `goodwe-0.3.4/goodwe/modbus.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.3/goodwe/model.py` & `goodwe-0.3.4/goodwe/model.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.3/goodwe/protocol.py` & `goodwe-0.3.4/goodwe/protocol.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.3/goodwe/sensor.py` & `goodwe-0.3.4/goodwe/sensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,26 +179,26 @@
     """Sensor representing energy [kWh] value encoded in 2 bytes"""
 
     def __init__(self, id_: str, offset: int, name: str, kind: Optional[SensorKind]):
         super().__init__(id_, offset, name, 2, "kWh", kind)
 
     def read_value(self, data: ProtocolResponse):
         value = read_bytes2(data)
-        return float(value) / 10
+        return float(value) / 10 if value else None
 
 
 class Energy4(Sensor):
     """Sensor representing energy [kWh] value encoded in 4 bytes"""
 
     def __init__(self, id_: str, offset: int, name: str, kind: Optional[SensorKind]):
         super().__init__(id_, offset, name, 4, "kWh", kind)
 
     def read_value(self, data: ProtocolResponse):
         value = read_bytes4(data)
-        return float(value) / 10
+        return float(value) / 10 if value else None
 
 
 class Apparent(Sensor):
     """Sensor representing apparent power [VA] value encoded in 2 bytes"""
 
     def __init__(self, id_: str, offset: int, name: str, kind: Optional[SensorKind]):
         super().__init__(id_, offset, name, 2, "VA", kind)
@@ -304,15 +304,15 @@
 class Integer(Sensor):
     """Sensor representing unsigned int value encoded in 2 bytes"""
 
     def __init__(self, id_: str, offset: int, name: str, unit: str = "", kind: Optional[SensorKind] = None):
         super().__init__(id_, offset, name, 2, unit, kind)
 
     def read_value(self, data: ProtocolResponse):
-        return read_bytes2(data)
+        return read_bytes2(data, None, 0)
 
     def encode_value(self, value: Any, register_value: bytes = None) -> bytes:
         return int.to_bytes(int(value), length=2, byteorder="big", signed=False)
 
 
 class IntegerS(Sensor):
     """Sensor representing signed int value encoded in 2 bytes"""
@@ -330,15 +330,15 @@
 class Long(Sensor):
     """Sensor representing unsigned int value encoded in 4 bytes"""
 
     def __init__(self, id_: str, offset: int, name: str, unit: str = "", kind: Optional[SensorKind] = None):
         super().__init__(id_, offset, name, 4, unit, kind)
 
     def read_value(self, data: ProtocolResponse):
-        return read_bytes4(data)
+        return read_bytes4(data, None, 0)
 
     def encode_value(self, value: Any, register_value: bytes = None) -> bytes:
         return int.to_bytes(int(value), length=4, byteorder="big", signed=False)
 
 
 class LongS(Sensor):
     """Sensor representing signed int value encoded in 4 bytes"""
@@ -410,15 +410,15 @@
         self._labels: Dict = labels
 
     def read_value(self, data: ProtocolResponse):
         return self._labels.get(read_byte(data))
 
 
 class EnumL(Sensor):
-    """Sensor representing label from enumeration encoded in 1 bytes (low 8 bits of 16bit register)"""
+    """Sensor representing label from enumeration encoded in 1 byte (low 8 bits of 16bit register)"""
 
     def __init__(self, id_: str, offset: int, labels: Dict, name: str, kind: Optional[SensorKind] = None):
         super().__init__(id_, offset, name, 1, "", kind)
         self._labels: Dict = labels
 
     def read_value(self, data: ProtocolResponse):
         read_byte(data)
@@ -429,15 +429,15 @@
     """Sensor representing label from enumeration encoded in 2 bytes"""
 
     def __init__(self, id_: str, offset: int, labels: Dict, name: str, kind: Optional[SensorKind] = None):
         super().__init__(id_, offset, name, 2, "", kind)
         self._labels: Dict = labels
 
     def read_value(self, data: ProtocolResponse):
-        return self._labels.get(read_bytes2(data))
+        return self._labels.get(read_bytes2(data, None, 0))
 
 
 class EnumBitmap4(Sensor):
     """Sensor representing label from bitmap encoded in 4 bytes"""
 
     def __init__(self, id_: str, offset: int, labels: Dict, name: str, kind: Optional[SensorKind] = None):
         super().__init__(id_, offset, name, 4, "", kind)
@@ -460,15 +460,16 @@
         self._labels: Dict = labels
         self._offsetL: int = offsetL
 
     def read_value(self, data: ProtocolResponse) -> Any:
         raise NotImplementedError()
 
     def read(self, data: ProtocolResponse):
-        return decode_bitmap(read_bytes2(data, self.offset) << 16 + read_bytes2(data, self._offsetL), self._labels)
+        return decode_bitmap(read_bytes2(data, self.offset, 0) << 16 + read_bytes2(data, self._offsetL, 0),
+                             self._labels)
 
 
 class EnumCalculated(Sensor):
     """Sensor representing label from enumeration of calculated value"""
 
     def __init__(self, id_: str, getter: Callable[[ProtocolResponse], Any], labels: Dict, name: str,
                  kind: Optional[SensorKind] = None):
@@ -781,35 +782,35 @@
 def read_byte(buffer: ProtocolResponse, offset: int = None) -> int:
     """Retrieve single byte (signed int) value from buffer"""
     if offset is not None:
         buffer.seek(offset)
     return int.from_bytes(buffer.read(1), byteorder="big", signed=True)
 
 
-def read_bytes2(buffer: ProtocolResponse, offset: int = None) -> int:
+def read_bytes2(buffer: ProtocolResponse, offset: int = None, undef: int = None) -> int:
     """Retrieve 2 byte (unsigned int) value from buffer"""
     if offset is not None:
         buffer.seek(offset)
     value = int.from_bytes(buffer.read(2), byteorder="big", signed=False)
-    return value if value != 0xffff else 0
+    return undef if value == 0xffff else value
 
 
 def read_bytes2_signed(buffer: ProtocolResponse, offset: int = None) -> int:
     """Retrieve 2 byte (signed int) value from buffer"""
     if offset is not None:
         buffer.seek(offset)
     return int.from_bytes(buffer.read(2), byteorder="big", signed=True)
 
 
-def read_bytes4(buffer: ProtocolResponse, offset: int = None) -> int:
+def read_bytes4(buffer: ProtocolResponse, offset: int = None, undef: int = None) -> int:
     """Retrieve 4 byte (unsigned int) value from buffer"""
     if offset is not None:
         buffer.seek(offset)
     value = int.from_bytes(buffer.read(4), byteorder="big", signed=False)
-    return value if value != 0xffffffff else 0
+    return undef if value == 0xffffffff else value
 
 
 def read_bytes4_signed(buffer: ProtocolResponse, offset: int = None) -> int:
     """Retrieve 4 byte (signed int) value from buffer"""
     if offset is not None:
         buffer.seek(offset)
     return int.from_bytes(buffer.read(4), byteorder="big", signed=True)
```

### Comparing `goodwe-0.3.3/goodwe.egg-info/PKG-INFO` & `goodwe-0.3.4/goodwe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goodwe
-Version: 0.3.3
+Version: 0.3.4
 Summary: Read data from GoodWe inverter via local network
 Home-page: https://github.com/marcelblijleven/goodwe
 Author: Martin Letenay, Marcel Blijleven
 Author-email: 'marcelblijleven@gmail.com
 License: MIT
 Keywords: GoodWe,Solar Panel,Inverter,Photovoltaics,PV
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `goodwe-0.3.3/setup.cfg` & `goodwe-0.3.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.3/tests/test_dt.py` & `goodwe-0.3.4/tests/test_dt.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,16 +163,16 @@
         self.assertSensor('work_mode', 1, '', data)
         self.assertSensor('work_mode_label', 'Normal', '', data)
         self.assertSensor('error_codes', 0, '', data)
         self.assertSensor('warning_code', 0, '', data)
         self.assertSensor("apparent_power", 0, "VA", data),
         self.assertSensor("reactive_power", 0, "var", data),
         self.assertSensor('temperature', 45.3, 'C', data)
-        self.assertSensor('e_day', 0.0, 'kWh', data)
-        self.assertSensor('e_total', 0.0, 'kWh', data)
+        self.assertSensor('e_day', None, 'kWh', data)
+        self.assertSensor('e_total', None, 'kWh', data)
         self.assertSensor('h_total', 0, 'h', data)
         self.assertSensor('safety_country', 32, '', data)
         self.assertSensor('safety_country_label', '50Hz 230Vac Default', '', data)
         self.assertSensor('funbit', 512, '', data)
         self.assertSensor('vbus', 624.2, 'V', data)
         self.assertSensor('vnbus', 316.8, 'V', data)
         self.assertSensor('derating_mode', 0, '', data)
@@ -217,15 +217,15 @@
         self.assertSensor('work_mode', 0, '', data)
         self.assertSensor('work_mode_label', 'Wait Mode', '', data)
         self.assertSensor('error_codes', 0, '', data)
         self.assertSensor('warning_code', 0, '', data)
         self.assertSensor("apparent_power", -1, "VA", data),
         self.assertSensor("reactive_power", -1, "var", data),
         self.assertSensor('temperature', 1.4, 'C', data)
-        self.assertSensor('e_day', 0.0, 'kWh', data)
+        self.assertSensor('e_day', None, 'kWh', data)
         self.assertSensor('e_total', 881.7, 'kWh', data)
         self.assertSensor('h_total', 955, 'h', data)
         self.assertSensor('safety_country', 73, '', data)
         self.assertSensor('safety_country_label', 'Australia Victoria', '', data)
         self.assertSensor('funbit', 2400, '', data)
         self.assertSensor('vbus', 291.7, 'V', data)
         self.assertSensor('vnbus', 0, 'V', data)
```

### Comparing `goodwe-0.3.3/tests/test_es.py` & `goodwe-0.3.4/tests/test_es.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.3/tests/test_et.py` & `goodwe-0.3.4/tests/test_et.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
         self.assertSensor('errors', '', '', data)
         self.assertSensor("e_total", 6085.3, 'kWh', data)
         self.assertSensor("e_day", 12.5, 'kWh', data)
         self.assertSensor("e_total_exp", 4718.6, 'kWh', data)
         self.assertSensor('h_total', 9246, 'h', data)
         self.assertSensor("e_day_exp", 9.8, 'kWh', data)
         self.assertSensor("e_total_imp", 58.0, 'kWh', data)
-        self.assertSensor("e_day_imp", 0.0, 'kWh', data)
+        self.assertSensor("e_day_imp", None, 'kWh', data)
         self.assertSensor("e_load_total", 8820.2, 'kWh', data)
         self.assertSensor("e_load_day", 11.6, 'kWh', data)
         self.assertSensor("e_bat_charge_total", 2758.1, 'kWh', data)
         self.assertSensor("e_bat_charge_day", 5.3, 'kWh', data)
         self.assertSensor("e_bat_discharge_total", 2442.1, 'kWh', data)
         self.assertSensor("e_bat_discharge_day", 2.9, 'kWh', data)
         self.assertSensor('diagnose_result', 117442560, '', data)
@@ -453,22 +453,22 @@
         self.assertSensor('error_codes', 0, '', data)
         self.assertSensor('errors', '', '', data)
         self.assertSensor("e_total", 59.4, 'kWh', data)
         self.assertSensor("e_day", 22.0, 'kWh', data)
         self.assertSensor("e_total_exp", 58.6, 'kWh', data)
         self.assertSensor('h_total', 33, 'h', data)
         self.assertSensor("e_day_exp", 21.6, 'kWh', data)
-        self.assertSensor("e_total_imp", 0.0, 'kWh', data)
-        self.assertSensor("e_day_imp", 0.0, 'kWh', data)
+        self.assertSensor("e_total_imp", None, 'kWh', data)
+        self.assertSensor("e_day_imp", None, 'kWh', data)
         self.assertSensor("e_load_total", 70.1, 'kWh', data)
         self.assertSensor("e_load_day", 27.1, 'kWh', data)
-        self.assertSensor("e_bat_charge_total", 0.0, 'kWh', data)
-        self.assertSensor("e_bat_charge_day", 0.0, 'kWh', data)
-        self.assertSensor("e_bat_discharge_total", 0.0, 'kWh', data)
-        self.assertSensor("e_bat_discharge_day", 0.0, 'kWh', data)
+        self.assertSensor("e_bat_charge_total", None, 'kWh', data)
+        self.assertSensor("e_bat_charge_day", None, 'kWh', data)
+        self.assertSensor("e_bat_discharge_total", None, 'kWh', data)
+        self.assertSensor("e_bat_discharge_day", None, 'kWh', data)
         self.assertSensor('diagnose_result', 117983303, '', data)
         self.assertSensor('diagnose_result_label',
                           'Battery voltage low, Battery SOC low, Battery SOC in back, Discharge Driver On, Self-use load light, Battery Disconnected, Self-use off, Export power limit set, PF value set, Real power limit set',
                           '', data)
         self.assertSensor('house_consumption', 1712, 'W', data)
 
 
@@ -554,16 +554,16 @@
         self.assertSensor('error_codes', 0, '', data)
         self.assertSensor('errors', '', '', data)
         self.assertSensor('e_total', 10225.8, 'kWh', data)
         self.assertSensor('e_day', 23.1, 'kWh', data)
         self.assertSensor('e_total_exp', 10273.3, 'kWh', data)
         self.assertSensor('h_total', 3256, 'h', data)
         self.assertSensor('e_day_exp', 16.6, 'kWh', data)
-        self.assertSensor('e_total_imp', 0.0, 'kWh', data)
-        self.assertSensor('e_day_imp', 0.0, 'kWh', data)
+        self.assertSensor('e_total_imp', None, 'kWh', data)
+        self.assertSensor('e_day_imp', None, 'kWh', data)
         self.assertSensor('e_load_total', 4393.9, 'kWh', data)
         self.assertSensor('e_load_day', 10.7, 'kWh', data)
         self.assertSensor('e_bat_charge_total', 141.9, 'kWh', data)
         self.assertSensor('e_bat_charge_day', 9.6, 'kWh', data)
         self.assertSensor('e_bat_discharge_total', 117.5, 'kWh', data)
         self.assertSensor('e_bat_discharge_day', 2.6, 'kWh', data)
         self.assertSensor('diagnose_result', 33556864, '', data)
@@ -767,15 +767,15 @@
         self.assertSensor('e_total_imp', 14.8, 'kWh', data)
         self.assertSensor('e_day_imp', 1.0, 'kWh', data)
         self.assertSensor('e_load_total', 17.2, 'kWh', data)
         self.assertSensor('e_load_day', 0.2, 'kWh', data)
         self.assertSensor('e_bat_charge_total', 91.3, 'kWh', data)
         self.assertSensor('e_bat_charge_day', 11.0, 'kWh', data)
         self.assertSensor('e_bat_discharge_total', 69.6, 'kWh', data)
-        self.assertSensor('e_bat_discharge_day', 0.0, 'kWh', data)
+        self.assertSensor('e_bat_discharge_day', None, 'kWh', data)
         self.assertSensor('diagnose_result', 33816960, '', data)
         self.assertSensor('diagnose_result_label',
                           'BMS: Discharge current low, APP: Discharge current too low, BMS: Charge disabled, PF value set',
                           '', data)
         self.assertSensor('house_consumption', 503, 'W', data)
         self.assertSensor('battery_bms', 255, '', data)
         self.assertSensor('battery_index', 311, '', data)
@@ -1038,21 +1038,21 @@
         self.assertSensor('errors', '', '', data)
         self.assertSensor('e_total', 4562.3, 'kWh', data)
         self.assertSensor('e_day', 0.9, 'kWh', data)
         self.assertSensor('e_total_exp', 4489.7, 'kWh', data)
         self.assertSensor('h_total', 1175, 'h', data)
         self.assertSensor('e_day_exp', 1.2, 'kWh', data)
         self.assertSensor('e_total_imp', 8.7, 'kWh', data)
-        self.assertSensor('e_day_imp', 0.0, 'kWh', data)
+        self.assertSensor('e_day_imp', None, 'kWh', data)
         self.assertSensor('e_load_total', 10742.2, 'kWh', data)
         self.assertSensor('e_load_day', 43.8, 'kWh', data)
-        self.assertSensor('e_bat_charge_total', 0.0, 'kWh', data)
-        self.assertSensor('e_bat_charge_day', 0.0, 'kWh', data)
-        self.assertSensor('e_bat_discharge_total', 0.0, 'kWh', data)
-        self.assertSensor('e_bat_discharge_day', 0.0, 'kWh', data)
+        self.assertSensor('e_bat_charge_total', None, 'kWh', data)
+        self.assertSensor('e_bat_charge_day', None, 'kWh', data)
+        self.assertSensor('e_bat_discharge_total', None, 'kWh', data)
+        self.assertSensor('e_bat_discharge_day', None, 'kWh', data)
         self.assertSensor('diagnose_result', 33816782, '', data)
         self.assertSensor('diagnose_result_label',
                           'Battery SOC low, Battery SOC in back, BMS: Discharge disabled, '
                           'Discharge Driver On, BMS: Discharge current low, BMS: Charge disabled, PF value set',
                           '', data)
         self.assertSensor('house_consumption', 6950, 'W', data)
         self.assertSensor('commode', 0, '', data)
```

### Comparing `goodwe-0.3.3/tests/test_modbus.py` & `goodwe-0.3.4/tests/test_modbus.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.3/tests/test_protocol.py` & `goodwe-0.3.4/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.3/tests/test_sensor.py` & `goodwe-0.3.4/tests/test_sensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
         data = MockResponse("0000069f")
         self.assertEqual(1695, testee.read(data))
 
         data = MockResponse("fffffffd")
         self.assertEqual(4294967293, testee.read(data))
 
         data = MockResponse("ffffffff")
-        self.assertEqual(0, testee.read(data))
+        self.assertIsNone(testee.read(data))
 
     def test_power4_signed(self):
         testee = Power4S("", 0, "", None)
 
         data = MockResponse("0000069f")
         self.assertEqual(1695, testee.read(data))
 
@@ -149,15 +149,15 @@
 
     def test_energy4(self):
         testee = Energy4("", 0, "", None)
 
         data = MockResponse("00020972")
         self.assertEqual(13349.0, testee.read(data))
         data = MockResponse("ffffffff")
-        self.assertEqual(0.0, testee.read(data))
+        self.assertIsNone(testee.read(data))
 
     def test_timestamp(self):
         testee = Timestamp("", 0, "", None)
 
         data = MockResponse("160104121e19")
         self.assertEqual(datetime(2022, 1, 4, 18, 30, 25), testee.read(data))
         self.assertEqual("160104121e19", testee.encode_value(datetime(2022, 1, 4, 18, 30, 25)).hex())
```

