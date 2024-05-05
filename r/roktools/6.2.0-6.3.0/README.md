# Comparing `tmp/roktools-6.2.0.tar.gz` & `tmp/roktools-6.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roktools-6.2.0.tar", max compression
+gzip compressed data, was "roktools-6.3.0.tar", max compression
```

## Comparing `roktools-6.2.0.tar` & `roktools-6.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1067 2024-05-03 10:04:56.539736 roktools-6.2.0/LICENSE
--rw-r--r--   0        0        0     1665 2024-05-03 10:04:56.539736 roktools-6.2.0/README.md
--rw-r--r--   0        0        0     1162 2024-05-03 10:04:56.539736 roktools-6.2.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-05-03 10:04:56.539736 roktools-6.2.0/roktools/__init__.py
--rw-r--r--   0        0        0     4509 2024-05-03 10:04:56.539736 roktools-6.2.0/roktools/cl.py
--rw-r--r--   0        0        0      133 2024-05-03 10:04:56.539736 roktools-6.2.0/roktools/constants.py
--rw-r--r--   0        0        0      491 2024-05-03 10:04:56.539736 roktools-6.2.0/roktools/decorator.py
--rw-r--r--   0        0        0      933 2024-05-03 10:04:56.539736 roktools-6.2.0/roktools/file.py
--rw-r--r--   0        0        0    33628 2024-05-03 10:04:56.539736 roktools-6.2.0/roktools/geodetic.py
--rw-r--r--   0        0        0        0 2024-05-03 10:04:56.583736 roktools-6.2.0/roktools/gnss/__init__.py
--rw-r--r--   0        0        0     1884 2024-05-03 10:04:56.539736 roktools-6.2.0/roktools/gnss/edit.py
--rw-r--r--   0        0        0     1644 2024-05-03 10:04:56.539736 roktools-6.2.0/roktools/gnss/observables.py
--rw-r--r--   0        0        0     1244 2024-05-03 10:04:56.539736 roktools-6.2.0/roktools/gnss/residuals.py
--rw-r--r--   0        0        0     9572 2024-05-03 10:04:56.539736 roktools-6.2.0/roktools/gnss/types.py
--rw-r--r--   0        0        0     1479 2024-05-03 10:04:56.539736 roktools-6.2.0/roktools/logger.py
--rw-r--r--   0        0        0        0 2024-05-03 10:04:56.583736 roktools-6.2.0/roktools/orbit/__init__.py
--rw-r--r--   0        0        0     1745 2024-05-03 10:04:56.539736 roktools-6.2.0/roktools/orbit/kepler.py
--rw-r--r--   0        0        0     5905 2024-05-03 10:04:56.539736 roktools-6.2.0/roktools/orbit/tle.py
--rw-r--r--   0        0        0        0 2024-05-03 10:04:56.583736 roktools-6.2.0/roktools/parsers/rtklib/__init__,py
--rw-r--r--   0        0        0     5459 2024-05-03 10:04:56.543736 roktools-6.2.0/roktools/parsers/rtklib/stats.py
--rw-r--r--   0        0        0    48895 2024-05-03 10:04:56.543736 roktools-6.2.0/roktools/rinex.py
--rwxr-xr-x   0        0        0     1084 2024-05-03 10:04:56.543736 roktools-6.2.0/roktools/stats.py
--rwxr-xr-x   0        0        0     1598 2024-05-03 10:04:56.543736 roktools-6.2.0/roktools/tensorial.py
--rw-r--r--   0        0        0    11178 2024-05-03 10:04:56.543736 roktools-6.2.0/roktools/time.py
--rw-r--r--   0        0        0     2181 1970-01-01 00:00:00.000000 roktools-6.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-05 08:08:57.792210 roktools-6.3.0/LICENSE
+-rw-r--r--   0        0        0     1665 2024-05-05 08:08:57.792210 roktools-6.3.0/README.md
+-rw-r--r--   0        0        0     1162 2024-05-05 08:08:57.792210 roktools-6.3.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-05 08:08:57.792210 roktools-6.3.0/roktools/__init__.py
+-rw-r--r--   0        0        0     4509 2024-05-05 08:08:57.792210 roktools-6.3.0/roktools/cl.py
+-rw-r--r--   0        0        0      133 2024-05-05 08:08:57.792210 roktools-6.3.0/roktools/constants.py
+-rw-r--r--   0        0        0      491 2024-05-05 08:08:57.792210 roktools-6.3.0/roktools/decorator.py
+-rw-r--r--   0        0        0      933 2024-05-05 08:08:57.792210 roktools-6.3.0/roktools/file.py
+-rw-r--r--   0        0        0    33628 2024-05-05 08:08:57.792210 roktools-6.3.0/roktools/geodetic.py
+-rw-r--r--   0        0        0        0 2024-05-05 08:08:57.844210 roktools-6.3.0/roktools/gnss/__init__.py
+-rw-r--r--   0        0        0     1884 2024-05-05 08:08:57.792210 roktools-6.3.0/roktools/gnss/edit.py
+-rw-r--r--   0        0        0     1644 2024-05-05 08:08:57.792210 roktools-6.3.0/roktools/gnss/observables.py
+-rw-r--r--   0        0        0     1244 2024-05-05 08:08:57.796210 roktools-6.3.0/roktools/gnss/residuals.py
+-rw-r--r--   0        0        0     9572 2024-05-05 08:08:57.796210 roktools-6.3.0/roktools/gnss/types.py
+-rw-r--r--   0        0        0     1479 2024-05-05 08:08:57.796210 roktools-6.3.0/roktools/logger.py
+-rw-r--r--   0        0        0        0 2024-05-05 08:08:57.844210 roktools-6.3.0/roktools/orbit/__init__.py
+-rw-r--r--   0        0        0     1745 2024-05-05 08:08:57.796210 roktools-6.3.0/roktools/orbit/kepler.py
+-rw-r--r--   0        0        0     5905 2024-05-05 08:08:57.796210 roktools-6.3.0/roktools/orbit/tle.py
+-rw-r--r--   0        0        0        0 2024-05-05 08:08:57.848209 roktools-6.3.0/roktools/parsers/rtklib/__init__,py
+-rw-r--r--   0        0        0     5459 2024-05-05 08:08:57.796210 roktools-6.3.0/roktools/parsers/rtklib/stats.py
+-rw-r--r--   0        0        0    61432 2024-05-05 08:08:57.796210 roktools-6.3.0/roktools/rinex.py
+-rwxr-xr-x   0        0        0     1084 2024-05-05 08:08:57.796210 roktools-6.3.0/roktools/stats.py
+-rwxr-xr-x   0        0        0     1598 2024-05-05 08:08:57.796210 roktools-6.3.0/roktools/tensorial.py
+-rw-r--r--   0        0        0    11178 2024-05-05 08:08:57.796210 roktools-6.3.0/roktools/time.py
+-rw-r--r--   0        0        0     2181 1970-01-01 00:00:00.000000 roktools-6.3.0/PKG-INFO
```

### Comparing `roktools-6.2.0/LICENSE` & `roktools-6.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `roktools-6.2.0/README.md` & `roktools-6.3.0/README.md`

 * *Files identical despite different names*

### Comparing `roktools-6.2.0/pyproject.toml` & `roktools-6.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "roktools"
-version = "6.2.0"
+version = "6.3.0"
 description = "Package with utilities and tools for GNSS data processing"
 authors = ["Rokubun <info@rokubun.cat>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 numpy = "^1.26.4"
```

### Comparing `roktools-6.2.0/roktools/cl.py` & `roktools-6.3.0/roktools/cl.py`

 * *Files identical despite different names*

### Comparing `roktools-6.2.0/roktools/file.py` & `roktools-6.3.0/roktools/file.py`

 * *Files identical despite different names*

### Comparing `roktools-6.2.0/roktools/geodetic.py` & `roktools-6.3.0/roktools/geodetic.py`

 * *Files identical despite different names*

### Comparing `roktools-6.2.0/roktools/gnss/edit.py` & `roktools-6.3.0/roktools/gnss/edit.py`

 * *Files identical despite different names*

### Comparing `roktools-6.2.0/roktools/gnss/observables.py` & `roktools-6.3.0/roktools/gnss/observables.py`

 * *Files identical despite different names*

### Comparing `roktools-6.2.0/roktools/gnss/residuals.py` & `roktools-6.3.0/roktools/gnss/residuals.py`

 * *Files identical despite different names*

### Comparing `roktools-6.2.0/roktools/gnss/types.py` & `roktools-6.3.0/roktools/gnss/types.py`

 * *Files identical despite different names*

### Comparing `roktools-6.2.0/roktools/logger.py` & `roktools-6.3.0/roktools/logger.py`

 * *Files identical despite different names*

### Comparing `roktools-6.2.0/roktools/orbit/kepler.py` & `roktools-6.3.0/roktools/orbit/kepler.py`

 * *Files identical despite different names*

### Comparing `roktools-6.2.0/roktools/orbit/tle.py` & `roktools-6.3.0/roktools/orbit/tle.py`

 * *Files identical despite different names*

### Comparing `roktools-6.2.0/roktools/parsers/rtklib/stats.py` & `roktools-6.3.0/roktools/parsers/rtklib/stats.py`

 * *Files identical despite different names*

### Comparing `roktools-6.2.0/roktools/rinex.py` & `roktools-6.3.0/roktools/rinex.py`

 * *Files 18% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     GAL_INAV = f'{ConstellationId.GALILEO.value}_INAV'
     GAL_FNAV = f'{ConstellationId.GALILEO.value}_FNAV'
     GLO_FDMA = f'{ConstellationId.GLONASS.value}_FDMA'
     QZS_LNAV = f'{ConstellationId.QZSS.value}_LNAV'
     QZS_CNAV = f'{ConstellationId.QZSS.value}_CNAV'
     QZS_CNV2 = f'{ConstellationId.QZSS.value}_CNV2'
     BDS_D1 = f'{ConstellationId.BEIDOU.value}_D1'
-    BDS_F2 = f'{ConstellationId.BEIDOU.value}_D2'
+    BDS_D2 = f'{ConstellationId.BEIDOU.value}_D2'
     BDS_CNV1 = f'{ConstellationId.BEIDOU.value}_CNV1'
     BDS_CNV2 = f'{ConstellationId.BEIDOU.value}_CNV2'
     BDS_CNV3 = f'{ConstellationId.BEIDOU.value}_CNV3'
     SBS = f'{ConstellationId.SBAS.value}_SBAS'
     IRN_LNAV = f'{ConstellationId.IRNSS.value}_LNAV'
     LEO = f'{ConstellationId.LEO.value}'
     SPIRE = f'{ConstellationId.SPIRE.value}'
@@ -826,14 +826,266 @@
         elif self.data_source & FNAV_MASK:
             return EphType.GAL_FNAV
 
         raise ValueError(f'Cannot extract the Galileo Eph type from the data sources [ {self.data_source} ]')
 
 
 @dataclass
+class BdsDNavBlock(NavBlock):
+    clock_bias_s: float
+    clock_drift_sps: float
+    clock_drift_rate_sps2: float
+
+    aode: int
+    crs: float
+    deltan: float
+    M0: float
+
+    cuc: float
+    e: float
+    cus: float
+    sqrtA: float
+
+    toe_bdt_tow: int
+    cic: float
+    OMEGA0: float
+    cis: float
+
+    i0: float
+    crc: float
+    omega: float
+    OMEGA_DOT: float
+
+    idot: float
+    toe_bdt_week: int
+
+    accuracy: float
+    satH1: int
+    tgd1: float
+    tgd2: float
+
+    tx_time_tow: float
+    aodc: int
+
+    eph_type: EphType
+
+    def csv_fields(self) -> str:
+        return f"{self.get_type().value},{_SAT_STR},{_EPOCH_STR},\
+{_CLK_BIAS_STR},{_CLK_DRIFT_STR},{_CLK_DRIFT_RATE_STR},\
+{_AODE_STR},{_CRS_STR},{_DELTAN_STR},{_M0_STR},\
+{_CUC_STR},{_E_STR},{_CUS_STR},{_SQRTA_STR},\
+{_TOE_BDT_TOW_STR},{_CIC_STR},{_OMEGA0_STR},{_CIS_STR},\
+{_I0_STR},{_CRC_STR},{_OMEGA_STR},{_OMEGA_DOT_STR},\
+{_IDOT_STR},{_TOE_BDT_WEEK_STR},\
+{_ACCURACY_STR},{_SATH1_STR},{_TGD1_STR},{_TGD2_STR},\
+{_TX_TIME_TOW_STR},{_AODC_STR}"
+
+    def get_type(self) -> EphType:
+        return self.eph_type
+
+
+@dataclass
+class BdsCnv1NavBlock(NavBlock):
+    """
+    BEIDOU Navigation message on Beidou-3 B1C signal
+    """
+    clock_bias_s: float
+    clock_drift_sps: float
+    clock_drift_rate_sps2: float
+
+    adot: float
+    crs: float
+    deltan: float
+    M0: float
+
+    cuc: float
+    e: float
+    cus: float
+    sqrtA: float
+
+    toe_bdt_tow: int
+    cic: float
+    OMEGA0: float
+    cis: float
+
+    i0: float
+    crc: float
+    omega: float
+    OMEGA_DOT: float
+
+    idot: float
+    deltan_dot: float
+    sattype: int
+    t_op: float
+
+    sisai_oe: float
+    sisai_ocb: float
+    sisai_oc1: float
+    sisai_oc2: float
+
+    isc_b1cd: float
+    tgd_b1cp: float
+    tgd_b2ap: float
+
+    sismai: float
+    health: int
+    b1c_integrity_flags: int
+    iodc: int
+
+    tx_time_tow: float
+    iode: int
+
+    def csv_fields(self) -> str:
+        return f"{self.get_type().value},{_SAT_STR},{_EPOCH_STR},\
+{_CLK_BIAS_STR},{_CLK_DRIFT_STR},{_CLK_DRIFT_RATE_STR},\
+{_ADOT_STR},{_CRS_STR},{_DELTAN_STR},{_M0_STR},\
+{_CUC_STR},{_E_STR},{_CUS_STR},{_SQRTA_STR},\
+{_TOE_BDT_TOW_STR},{_CIC_STR},{_OMEGA0_STR},{_CIS_STR},\
+{_I0_STR},{_CRC_STR},{_OMEGA_STR},{_OMEGA_DOT_STR},\
+{_IDOT_STR},{_DELTAN_DOT_STR},{_SAT_TYPE_STR},{_T_OP_STR},\
+{_SISAI_OE_STR},{_SISAI_OCB_STR},{_SISAI_OC1_STR},{_SISAI_OC2_STR},\
+{_ISC_B1CD_STR},{_TGD_B1CP},{_TGD_B2AP},\
+{_SISMAI_STR},{_HEALTH_STR},{_B1C_INTEGRITY_FLAGS_STR},{_IODC_STR},\
+{_TX_TIME_TOW_STR},{_IODE_STR}"
+
+    def get_type(self) -> EphType:
+        return EphType.BDS_CNV1
+
+
+@dataclass
+class BdsCnv2NavBlock(NavBlock):
+    """
+    BEIDOU Navigation message on Beidou-3 B2a signal
+    """
+    clock_bias_s: float
+    clock_drift_sps: float
+    clock_drift_rate_sps2: float
+
+    adot: float
+    crs: float
+    deltan: float
+    M0: float
+
+    cuc: float
+    e: float
+    cus: float
+    sqrtA: float
+
+    toe_bdt_tow: int
+    cic: float
+    OMEGA0: float
+    cis: float
+
+    i0: float
+    crc: float
+    omega: float
+    OMEGA_DOT: float
+
+    idot: float
+    deltan_dot: float
+    sattype: int
+    t_op: float
+
+    sisai_oe: float
+    sisai_ocb: float
+    sisai_oc1: float
+    sisai_oc2: float
+
+    isc_b2ad: float
+    tgd_b1cp: float
+    tgd_b2ap: float
+
+    sismai: float
+    health: int
+    b2a_integrity_flags: int
+    iodc: int
+
+    tx_time_tow: float
+    iode: int
+
+    def csv_fields(self) -> str:
+        return f"{self.get_type().value},{_SAT_STR},{_EPOCH_STR},\
+{_CLK_BIAS_STR},{_CLK_DRIFT_STR},{_CLK_DRIFT_RATE_STR},\
+{_ADOT_STR},{_CRS_STR},{_DELTAN_STR},{_M0_STR},\
+{_CUC_STR},{_E_STR},{_CUS_STR},{_SQRTA_STR},\
+{_TOE_BDT_TOW_STR},{_CIC_STR},{_OMEGA0_STR},{_CIS_STR},\
+{_I0_STR},{_CRC_STR},{_OMEGA_STR},{_OMEGA_DOT_STR},\
+{_IDOT_STR},{_DELTAN_DOT_STR},{_SAT_TYPE_STR},{_T_OP_STR},\
+{_SISAI_OE_STR},{_SISAI_OCB_STR},{_SISAI_OC1_STR},{_SISAI_OC2_STR},\
+{_ISC_B2AD_STR},{_TGD_B1CP},{_TGD_B2AP},\
+{_SISMAI_STR},{_HEALTH_STR},{_B2A_INTEGRITY_FLAGS_STR},{_IODC_STR},\
+{_TX_TIME_TOW_STR},{_IODE_STR}"
+
+    def get_type(self) -> EphType:
+        return EphType.BDS_CNV2
+
+
+@dataclass
+class BdsCnv3NavBlock(NavBlock):
+    """
+    BEIDOU Navigation message on Beidou-3 B2b signal
+    """
+    clock_bias_s: float
+    clock_drift_sps: float
+    clock_drift_rate_sps2: float
+
+    adot: float
+    crs: float
+    deltan: float
+    M0: float
+
+    cuc: float
+    e: float
+    cus: float
+    sqrtA: float
+
+    toe_bdt_tow: int
+    cic: float
+    OMEGA0: float
+    cis: float
+
+    i0: float
+    crc: float
+    omega: float
+    OMEGA_DOT: float
+
+    idot: float
+    deltan_dot: float
+    sattype: int
+    t_op: float
+
+    sisai_oe: float
+    sisai_ocb: float
+    sisai_oc1: float
+    sisai_oc2: float
+
+    sismai: float
+    health: int
+    b2b_integrity_flags: int
+    tgd_b2bi: int
+
+    tx_time_tow: float
+
+    def csv_fields(self) -> str:
+        return f"{self.get_type().value},{_SAT_STR},{_EPOCH_STR},\
+{_CLK_BIAS_STR},{_CLK_DRIFT_STR},{_CLK_DRIFT_RATE_STR},\
+{_ADOT_STR},{_CRS_STR},{_DELTAN_STR},{_M0_STR},\
+{_CUC_STR},{_E_STR},{_CUS_STR},{_SQRTA_STR},\
+{_TOE_BDT_TOW_STR},{_CIC_STR},{_OMEGA0_STR},{_CIS_STR},\
+{_I0_STR},{_CRC_STR},{_OMEGA_STR},{_OMEGA_DOT_STR},\
+{_IDOT_STR},{_DELTAN_DOT_STR},{_SAT_TYPE_STR},{_T_OP_STR},\
+{_SISAI_OE_STR},{_SISAI_OCB_STR},{_SISAI_OC1_STR},{_SISAI_OC2_STR},\
+{_SISMAI_STR},{_HEALTH_STR},{_B2B_INTEGRITY_FLAGS_STR},{_TGD_B2BI},\
+{_TX_TIME_TOW_STR},{_IODE_STR}"
+
+    def get_type(self) -> EphType:
+        return EphType.BDS_CNV2
+
+
+@dataclass
 class RawNavBlock(object):
     satellite: Satellite
     epoch: datetime.datetime
     lines: List[str]
 
     def __repr__(self):
         return '\n'.join(self.lines)
@@ -881,14 +1133,22 @@
             return self._to_GPS_LNAV()
         elif eph_type == EphType.GPS_CNAV:
             return self._to_GPS_CNAV()
         elif eph_type == EphType.GPS_CNV2:
             return self._to_GPS_CNV2()
         elif eph_type == EphType.GAL_FNAV or eph_type == EphType.GAL_INAV:
             return self._to_GAL()
+        elif eph_type == EphType.BDS_D1 or eph_type == EphType.BDS_D2:
+            return self._to_BDS_D(eph_type)
+        elif eph_type == EphType.BDS_CNV1:
+            return self._to_BDS_CNV1()
+        elif eph_type == EphType.BDS_CNV2:
+            return self._to_BDS_CNV2()
+        elif eph_type == EphType.BDS_CNV3:
+            return self._to_BDS_CNV3()
 
         raise ValueError(f'There is no NavBlock generator for [ {eph_type} ]')
 
     def _to_GPS_LNAV(self) -> GpsLnavNavBlock:
 
         sat_str, year, month, day, hour,  min, sec, clk_bias, clk_drift, clk_drift_rate = _parse_nav_epoch_line(self.lines[1])
         iode, crs, deltan, M0 = _parse_nav_orb_line(self.lines[2])
@@ -981,14 +1241,112 @@
                            cuc, e, cus, sqrtA,
                            toe_tow, cic, OMEGA0, cis,
                            i0, crc, omega, OMEGA_DOT,
                            idot, int(datasources), int(toe_week),
                            sisa, health, bgd_e5a, bgd_e5b,
                            tx_tm)
 
+    def _to_BDS_D(self, eph_type: EphType) -> BdsDNavBlock:
+
+        sat_str, year, month, day, hour,  min, sec, clk_bias, clk_drift, clk_drift_rate = _parse_nav_epoch_line(self.lines[1])
+        aode, crs, deltan, M0 = _parse_nav_orb_line(self.lines[2])
+        cuc, e, cus, sqrtA = _parse_nav_orb_line(self.lines[3])
+        toe_tow, cic, OMEGA0, cis = _parse_nav_orb_line(self.lines[4])
+        i0, crc, omega, OMEGA_DOT = _parse_nav_orb_line(self.lines[5])
+        idot, _, toe_week, _ = _parse_nav_orb_line(self.lines[6])
+        accuracy, satH1, tgd1, tgd2 = _parse_nav_orb_line(self.lines[7])
+        tx_tm, aodc, _, _ = _parse_nav_orb_line(self.lines[8])
+
+        return BdsDNavBlock(Satellite.from_string(sat_str),
+                            datetime.datetime(year, month, day, hour, min, sec),
+                            clk_bias, clk_drift, clk_drift_rate,
+                            int(aode), crs, deltan, M0,
+                            cuc, e, cus, sqrtA,
+                            toe_tow, cic, OMEGA0, cis,
+                            i0, crc, omega, OMEGA_DOT,
+                            idot, int(toe_week),
+                            accuracy, int(satH1), tgd1, tgd2,
+                            tx_tm, aodc, eph_type)
+
+    def _to_BDS_CNV1(self) -> BdsCnv1NavBlock:
+
+        sat_str, year, month, day, hour,  min, sec, clk_bias, clk_drift, clk_drift_rate = _parse_nav_epoch_line(self.lines[1])
+        adot, crs, deltan, M0 = _parse_nav_orb_line(self.lines[2])
+        cuc, e, cus, sqrtA = _parse_nav_orb_line(self.lines[3])
+        toe_tow, cic, OMEGA0, cis = _parse_nav_orb_line(self.lines[4])
+        i0, crc, omega, OMEGA_DOT = _parse_nav_orb_line(self.lines[5])
+        idot, deltan_dot, sattype, t_op = _parse_nav_orb_line(self.lines[6])
+        sisai_oe, sisai_ocb, sisai_oc1, sisai_oc2 = _parse_nav_orb_line(self.lines[7])
+        isc_b1cd, _, tgd_b1cp, tgd_b2ap = _parse_nav_orb_line(self.lines[8])
+        sismai, health, b1c_integrity_flags, iodc = _parse_nav_orb_line(self.lines[9])
+        tx_time_tow, _, _, iode = _parse_nav_orb_line(self.lines[10])
+
+        return BdsCnv1NavBlock(Satellite.from_string(sat_str),
+                               datetime.datetime(year, month, day, hour, min, sec),
+                               clk_bias, clk_drift, clk_drift_rate,
+                               adot, crs, deltan, M0,
+                               cuc, e, cus, sqrtA,
+                               toe_tow, cic, OMEGA0, cis,
+                               i0, crc, omega, OMEGA_DOT,
+                               idot, deltan_dot, int(sattype), t_op,
+                               sisai_oe, sisai_ocb, sisai_oc1, sisai_oc2,
+                               isc_b1cd, tgd_b1cp, tgd_b2ap,
+                               sismai, int(health), int(b1c_integrity_flags), int(iodc),
+                               tx_time_tow, int(iode))
+
+    def _to_BDS_CNV2(self) -> BdsCnv2NavBlock:
+
+        sat_str, year, month, day, hour,  min, sec, clk_bias, clk_drift, clk_drift_rate = _parse_nav_epoch_line(self.lines[1])
+        adot, crs, deltan, M0 = _parse_nav_orb_line(self.lines[2])
+        cuc, e, cus, sqrtA = _parse_nav_orb_line(self.lines[3])
+        toe_tow, cic, OMEGA0, cis = _parse_nav_orb_line(self.lines[4])
+        i0, crc, omega, OMEGA_DOT = _parse_nav_orb_line(self.lines[5])
+        idot, deltan_dot, sattype, t_op = _parse_nav_orb_line(self.lines[6])
+        sisai_oe, sisai_ocb, sisai_oc1, sisai_oc2 = _parse_nav_orb_line(self.lines[7])
+        isc_b2ad, _, tgd_b1cp, tgd_b2ap = _parse_nav_orb_line(self.lines[8])
+        sismai, health, b2a_integrity_flags, iodc = _parse_nav_orb_line(self.lines[9])
+        tx_time_tow, _, _, iode = _parse_nav_orb_line(self.lines[10])
+
+        return BdsCnv2NavBlock(Satellite.from_string(sat_str),
+                               datetime.datetime(year, month, day, hour, min, sec),
+                               clk_bias, clk_drift, clk_drift_rate,
+                               adot, crs, deltan, M0,
+                               cuc, e, cus, sqrtA,
+                               toe_tow, cic, OMEGA0, cis,
+                               i0, crc, omega, OMEGA_DOT,
+                               idot, deltan_dot, int(sattype), t_op,
+                               sisai_oe, sisai_ocb, sisai_oc1, sisai_oc2,
+                               isc_b2ad, tgd_b1cp, tgd_b2ap,
+                               sismai, int(health), int(b2a_integrity_flags), int(iodc),
+                               tx_time_tow, int(iode))
+
+    def _to_BDS_CNV3(self) -> BdsCnv3NavBlock:
+
+        sat_str, year, month, day, hour,  min, sec, clk_bias, clk_drift, clk_drift_rate = _parse_nav_epoch_line(self.lines[1])
+        adot, crs, deltan, M0 = _parse_nav_orb_line(self.lines[2])
+        cuc, e, cus, sqrtA = _parse_nav_orb_line(self.lines[3])
+        toe_tow, cic, OMEGA0, cis = _parse_nav_orb_line(self.lines[4])
+        i0, crc, omega, OMEGA_DOT = _parse_nav_orb_line(self.lines[5])
+        idot, deltan_dot, sattype, t_op = _parse_nav_orb_line(self.lines[6])
+        sisai_oe, sisai_ocb, sisai_oc1, sisai_oc2 = _parse_nav_orb_line(self.lines[7])
+        sismai, health, b2b_integrity_flags, tgd_b2ap = _parse_nav_orb_line(self.lines[8])
+        tx_time_tow, _, _, iode = _parse_nav_orb_line(self.lines[9])
+
+        return BdsCnv3NavBlock(Satellite.from_string(sat_str),
+                               datetime.datetime(year, month, day, hour, min, sec),
+                               clk_bias, clk_drift, clk_drift_rate,
+                               adot, crs, deltan, M0,
+                               cuc, e, cus, sqrtA,
+                               toe_tow, cic, OMEGA0, cis,
+                               i0, crc, omega, OMEGA_DOT,
+                               idot, deltan_dot, int(sattype), t_op,
+                               sisai_oe, sisai_ocb, sisai_oc1, sisai_oc2,
+                               sismai, int(health), int(b2b_integrity_flags), tgd_b2ap,
+                               tx_time_tow)
+
 
 class Nav(object):
     """
     Class that holds Rinex Navigation data
     """
 
     RINEX4_EPH_BLOCK_LINES_LEO = 6
@@ -1000,15 +1358,15 @@
         EphType.GAL_INAV: 8,
         EphType.GAL_FNAV: 8,
         EphType.GLO_FDMA: 5,
         EphType.QZS_LNAV: 8,
         EphType.QZS_CNAV: 9,
         EphType.QZS_CNV2: 10,
         EphType.BDS_D1: 8,
-        EphType.BDS_F2: 8,
+        EphType.BDS_D2: 8,
         EphType.BDS_CNV1: 10,
         EphType.BDS_CNV2: 10,
         EphType.BDS_CNV3: 9,
         EphType.SBS: 4,
         EphType.IRN_LNAV: 8,
         EphType.LEO: RINEX4_EPH_BLOCK_LINES_LEO,
         EphType.SPIRE: RINEX4_EPH_BLOCK_LINES_LEO,
@@ -1356,20 +1714,22 @@
     parser = argparse.ArgumentParser(description="Tool to convert an input file to RINEX navigation file",
                                      formatter_class=argparse.RawDescriptionHelpFormatter)  # for verbatim
 
     # Define the mutually exclusive group
     input_options = parser.add_mutually_exclusive_group(required=True)
 
     input_options.add_argument('--celestrak_file', metavar='<filename>', type=str,
-                               help='File from Celestrak with the TLE elements to convert to RINEX. Based on https://arxiv.org/abs/2401.17767')
+                               help='File from Celestrak with the TLE elements to convert to RINEX.' +
+                                    'Based on https://arxiv.org/abs/2401.17767')
 
     input_options.add_argument('--csv', metavar='<filename>', type=str,
                                help='CSV file with the description of ')
 
-    parser.add_argument('--rinex2', action='store_true', help='Output the format in Rinex 2 GPS format. Will skip satellites with PRN larger than 99')
+    parser.add_argument('--rinex2', action='store_true',
+                        help='Output the format in Rinex 2 GPS format. Will skip satellites with PRN larger than 99')
 
     # Parse the command-line arguments
     args = parser.parse_args()
 
     if args.celestrak_file:
         tle_list = read_celestrak(args.celestrak_file)
         Nav.write_from_tle(sys.stdout, tle_list, rinex2=args.rinex2)
@@ -1377,14 +1737,19 @@
     elif args.csv:
         df = pd.read_csv(args.csv, parse_dates=['epoch'])
         Nav.write_from_dataframe(sys.stdout, df, rinex2=args.rinex2)
 
 
 _ACCURACY_STR = "accuracy"
 _ADOT_STR = "Adot[m/s]"
+_AODC_STR = "aodc"
+_AODE_STR = "aode"
+_B1C_INTEGRITY_FLAGS_STR = "b1c_integrity_flags"
+_B2A_INTEGRITY_FLAGS_STR = "b2a_integrity_flags"
+_B2B_INTEGRITY_FLAGS_STR = "b2b_integrity_flags"
 _BGD_E5A_STR = "bgd_e5a_e1[s]"
 _BGD_E5B_STR = "bgd_e5b_e1[s]"
 _CIC_STR = "cic[rad]"
 _CIS_STR = "cis[rad]"
 _CLK_BIAS_STR = "clock_bias[s]"
 _CLK_DRIFT_RATE_STR = "clock_drift_rate[s/s2]"
 _CLK_DRIFT_STR = "clock_drift[s/s]"
@@ -1401,29 +1766,45 @@
 _FIT_INTERVAL_STR = "fit_interval"
 _HEALTH_STR = "health"
 _I0_STR = "i0[rad]"
 _IDOT_STR = "idot[rad/s]"
 _IODC_STR = "iodc"
 _IODE_STR = "iode"
 _IODNAV_STR = "iodnav"
+_ISC_B2AD_STR = "isc_b2ad[s]"
+_ISC_B1CD_STR = "isc_b1cd[s]"
 _ISC_L1CA_STR = "isc_L1CA[s]"
 _ISC_L1CD_STR = "isc_L1CD[s]"
 _ISC_L1CP_STR = "isc_L1CP[s]"
 _ISC_L2C_STR = "isc_L2C[s]"
 _ISC_L5I5_STR = "isc_L5I5[s]"
 _ISC_L5Q5_STR = "isc_L5Q5[s]"
 _L2PFLAG_STR = "l2p_flag"
 _M0_STR = "M0[rad]"
 _OMEGA0_STR = "OMEGA0[rad]"
 _OMEGA_DOT_STR = "OMEGA_DOT[rad/s]"
 _OMEGA_STR = "omega[rad]"
+_SATH1_STR = "sat_H1"
 _SAT_STR = "sat"
+_SAT_TYPE_STR = "sat_type"
+_SISAI_OC1_STR = "SISAI_oc1"
+_SISAI_OC2_STR = "SISAI_oc2"
+_SISAI_OCB_STR = "SISAI_ocb"
+_SISAI_OE_STR = "SISAI_oe"
 _SISA_STR = "sisa[m]"
+_SISMAI_STR = "SISMAI"
 _SQRTA_STR = "sqrtA[sqrt(m)]"
+_TGD1_STR = "tgd1[s]"
+_TGD2_STR = "tgd2[s]"
+_TGD_B1CP = "tgd_b1cp[s]"
+_TGD_B2AP = "tgd_b2ap[s]"
+_TGD_B2BI = "tgd_b2bi[s]"
 _TGD_STR = "tgd[s]"
+_TOE_BDT_TOW_STR = "toe_bdt_tow[s]"
+_TOE_BDT_WEEK_STR = "toe_bdt_week[week]"
 _TOE_GAL_TOW_STR = "toe_gal_tow[s]"
 _TOE_GAL_WEEK_STR = "toe_gal_week[week]"
 _TOE_SOW_STR = "toe[s]"
 _TOE_WEEK_STR = "toe[week]"
 _TX_TIME_TOW_STR = "tx_time[s]"
 _T_OP_STR = "t_op[s]"
 _URAI_ED_STR = "urai_ed"
```

### Comparing `roktools-6.2.0/roktools/stats.py` & `roktools-6.3.0/roktools/stats.py`

 * *Files identical despite different names*

### Comparing `roktools-6.2.0/roktools/tensorial.py` & `roktools-6.3.0/roktools/tensorial.py`

 * *Files identical despite different names*

### Comparing `roktools-6.2.0/roktools/time.py` & `roktools-6.3.0/roktools/time.py`

 * *Files identical despite different names*

### Comparing `roktools-6.2.0/PKG-INFO` & `roktools-6.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roktools
-Version: 6.2.0
+Version: 6.3.0
 Summary: Package with utilities and tools for GNSS data processing
 Author: Rokubun
 Author-email: info@rokubun.cat
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

