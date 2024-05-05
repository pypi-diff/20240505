# Comparing `tmp/oda_reader-0.0.9.tar.gz` & `tmp/oda_reader-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oda_reader-0.0.9.tar", max compression
+gzip compressed data, was "oda_reader-0.2.0.tar", max compression
```

## Comparing `oda_reader-0.0.9.tar` & `oda_reader-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1069 2024-05-05 10:44:52.876307 oda_reader-0.0.9/LICENSE
--rw-r--r--   0        0        0      317 2024-05-05 10:44:52.876307 oda_reader-0.0.9/README.md
--rw-r--r--   0        0        0       22 2024-05-05 10:44:52.876307 oda_reader-0.0.9/oda_reader/__init__.py
--rw-r--r--   0        0        0     2769 2024-05-05 10:44:52.876307 oda_reader-0.0.9/oda_reader/common.py
--rw-r--r--   0        0        0     1263 2024-05-05 10:44:52.876307 oda_reader-0.0.9/oda_reader/dac1.py
--rw-r--r--   0        0        0     1266 2024-05-05 10:44:52.876307 oda_reader-0.0.9/oda_reader/dac2a.py
--rw-r--r--   0        0        0     2858 2024-05-05 10:44:52.876307 oda_reader-0.0.9/oda_reader/download_tools.py
--rw-r--r--   0        0        0     6304 2024-05-05 10:44:52.876307 oda_reader-0.0.9/oda_reader/query_builder.py
--rw-r--r--   0        0        0        0 2024-05-05 10:44:52.876307 oda_reader-0.0.9/oda_reader/schemas/__init__.py
--rw-r--r--   0        0        0      116 2024-05-05 10:44:52.876307 oda_reader-0.0.9/oda_reader/schemas/area_code_corrections.json
--rw-r--r--   0        0        0       38 2024-05-05 10:44:52.876307 oda_reader-0.0.9/oda_reader/schemas/code_prices_corrections.json
--rw-r--r--   0        0        0     8260 2024-05-05 10:44:52.876307 oda_reader-0.0.9/oda_reader/schemas/dac1_codes_area.json
--rw-r--r--   0        0        0       53 2024-05-05 10:44:52.876307 oda_reader-0.0.9/oda_reader/schemas/dac1_codes_flow_types.json
--rw-r--r--   0        0        0       30 2024-05-05 10:44:52.876307 oda_reader-0.0.9/oda_reader/schemas/dac1_codes_prices.json
--rw-r--r--   0        0        0     2984 2024-05-05 10:44:52.876307 oda_reader-0.0.9/oda_reader/schemas/dac1_dotstat.json
--rw-r--r--   0        0        0     2869 2024-05-05 10:44:52.876307 oda_reader-0.0.9/oda_reader/schemas/dac1_translation.py
--rw-r--r--   0        0        0     8544 2024-05-05 10:44:52.876307 oda_reader-0.0.9/oda_reader/schemas/dac2_codes_area.json
--rw-r--r--   0        0        0     1947 2024-05-05 10:44:52.876307 oda_reader-0.0.9/oda_reader/schemas/dac2_translation.py
--rw-r--r--   0        0        0     2790 2024-05-05 10:44:52.876307 oda_reader-0.0.9/oda_reader/schemas/dac2a_dotstat.json
--rw-r--r--   0        0        0     5075 2024-05-05 10:44:52.876307 oda_reader-0.0.9/oda_reader/schemas/schema_tools.py
--rw-r--r--   0        0        0     5173 2024-05-05 10:44:52.876307 oda_reader-0.0.9/oda_reader/schemas/xml_tools.py
--rw-r--r--   0        0        0      448 2024-05-05 10:44:52.876307 oda_reader-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      912 1970-01-01 00:00:00.000000 oda_reader-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-05 13:44:03.815870 oda_reader-0.2.0/LICENSE
+-rw-r--r--   0        0        0      317 2024-05-05 13:44:03.815870 oda_reader-0.2.0/README.md
+-rw-r--r--   0        0        0       22 2024-05-05 13:44:03.815870 oda_reader-0.2.0/oda_reader/__init__.py
+-rw-r--r--   0        0        0     2767 2024-05-05 13:44:03.815870 oda_reader-0.2.0/oda_reader/common.py
+-rw-r--r--   0        0        0     1263 2024-05-05 13:44:03.815870 oda_reader-0.2.0/oda_reader/dac1.py
+-rw-r--r--   0        0        0     1267 2024-05-05 13:44:03.815870 oda_reader-0.2.0/oda_reader/dac2a.py
+-rw-r--r--   0        0        0     2858 2024-05-05 13:44:03.815870 oda_reader-0.2.0/oda_reader/download_tools.py
+-rw-r--r--   0        0        0     8304 2024-05-05 13:44:03.815870 oda_reader-0.2.0/oda_reader/query_builder.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:44:03.815870 oda_reader-0.2.0/oda_reader/schemas/__init__.py
+-rw-r--r--   0        0        0      116 2024-05-05 13:44:03.815870 oda_reader-0.2.0/oda_reader/schemas/area_code_corrections.json
+-rw-r--r--   0        0        0       38 2024-05-05 13:44:03.815870 oda_reader-0.2.0/oda_reader/schemas/code_prices_corrections.json
+-rw-r--r--   0        0        0     8260 2024-05-05 13:44:03.815870 oda_reader-0.2.0/oda_reader/schemas/dac1_codes_area.json
+-rw-r--r--   0        0        0       53 2024-05-05 13:44:03.815870 oda_reader-0.2.0/oda_reader/schemas/dac1_codes_flow_types.json
+-rw-r--r--   0        0        0       30 2024-05-05 13:44:03.815870 oda_reader-0.2.0/oda_reader/schemas/dac1_codes_prices.json
+-rw-r--r--   0        0        0     2984 2024-05-05 13:44:03.815870 oda_reader-0.2.0/oda_reader/schemas/dac1_dotstat.json
+-rw-r--r--   0        0        0     2869 2024-05-05 13:44:03.815870 oda_reader-0.2.0/oda_reader/schemas/dac1_translation.py
+-rw-r--r--   0        0        0     8544 2024-05-05 13:44:03.815870 oda_reader-0.2.0/oda_reader/schemas/dac2_codes_area.json
+-rw-r--r--   0        0        0     1947 2024-05-05 13:44:03.815870 oda_reader-0.2.0/oda_reader/schemas/dac2_translation.py
+-rw-r--r--   0        0        0     2790 2024-05-05 13:44:03.815870 oda_reader-0.2.0/oda_reader/schemas/dac2a_dotstat.json
+-rw-r--r--   0        0        0     5075 2024-05-05 13:44:03.815870 oda_reader-0.2.0/oda_reader/schemas/schema_tools.py
+-rw-r--r--   0        0        0     5173 2024-05-05 13:44:03.815870 oda_reader-0.2.0/oda_reader/schemas/xml_tools.py
+-rw-r--r--   0        0        0      448 2024-05-05 13:44:03.815870 oda_reader-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      912 1970-01-01 00:00:00.000000 oda_reader-0.2.0/PKG-INFO
```

### Comparing `oda_reader-0.0.9/LICENSE` & `oda_reader-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oda_reader-0.0.9/oda_reader/common.py` & `oda_reader-0.2.0/oda_reader/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 logger = logging.getLogger("oda_importer")
 
 
 class ImporterPaths:
     """Class to store the paths to the data and output folders."""
 
     project = Path(__file__).resolve().parent.parent
-    scripts = project / "oda_importer"
+    scripts = project / "oda_reader"
     schemas = scripts / "schemas"
 
 
 def text_to_stringIO(response: requests.models.Response) -> StringIO:
     """Convert the content of a response to bytes.
 
     Args:
```

### Comparing `oda_reader-0.0.9/oda_reader/dac1.py` & `oda_reader-0.2.0/oda_reader/dac1.py`

 * *Files identical despite different names*

### Comparing `oda_reader-0.0.9/oda_reader/dac2a.py` & `oda_reader-0.2.0/oda_reader/dac2a.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     """
 
     # Inform download is about to start
     logger.info("Downloading DAC2A data. This may take a while...")
 
     df = download(
-        version="dac1",
+        version="dac2a",
         dataflow_id=DATAFLOW_ID,
         start_year=start_year,
         end_year=end_year,
         filters=filters,
         pre_process=pre_process,
         dotstat_codes=dotstat_codes,
     )
```

### Comparing `oda_reader-0.0.9/oda_reader/download_tools.py` & `oda_reader-0.2.0/oda_reader/download_tools.py`

 * *Files identical despite different names*

### Comparing `oda_reader-0.0.9/oda_reader/query_builder.py` & `oda_reader-0.2.0/oda_reader/query_builder.py`

 * *Files 19% similar despite different names*

```diff
@@ -119,27 +119,76 @@
         self,
         donor: str | list[str] | None = None,
         measure: str | list[str] | None = None,
         flow_type: str | list[str] | None = None,
         unit_measure: str | list[str] | None = None,
         price_base: str | list[str] | None = None,
     ) -> str:
+        """Build the filter string for the DAC1 dataflow.
+
+        The allowed filter follows the pattern:
+        {donor}.{measure}.{untied}.{flow_type}.{unit_measure}.{price_base}.{period}
+
+        Args:
+            donor (str | list[str] | None): The donor country code(s).
+            measure (str | list[str] | None): The measure code(s).
+            flow_type (str | list[str] | None): The flow type code(s).
+            unit_measure (str | list[str] | None): The unit of measure code(s).
+            price_base (str | list[str] | None): The price base code(s).
+
+        Returns:
+            str: The filter string for the query.
+        """
+
         # if any of the parameters are None, set them to the default value
         donor = self._to_filter_str(donor)
         measure = self._to_filter_str(measure)
         untied = self._to_filter_str(None)
         flow_type = self._to_filter_str(flow_type)
         unit_measure = self._to_filter_str(unit_measure)
         price_base = self._to_filter_str(price_base)
         period = self._to_filter_str(None)
 
         return ".".join(
             [donor, measure, untied, flow_type, unit_measure, price_base, period]
         )
 
+    def build_dac2a_filter(
+        self,
+        donor: str | list[str] | None = None,
+        recipient: str | list[str] | None = None,
+        measure: int | list[int] | None = None,
+        unit_measure: str | list[str] | None = None,
+        price_base: str | list[str] | None = None,
+    ) -> str:
+        """Build the filter string for the DAC2A dataflow.
+
+        The allowed filter follows the pattern:
+        {donor}.{recipient}.{measure}.{unit_measure}.{price_base}
+
+        Args:
+            donor (str | list[str] | None): The donor country code(s).
+            recipient (str | list[str] | None): The recipient country code(s).
+            measure (int | list[int] | None): The measure code(s).
+            unit_measure (str | list[str] | None): The unit of measure code(s).
+            price_base (str | list[str] | None): The price base code(s).
+
+        Returns:
+            str: The filter string for the query.
+
+        """
+        # if any of the parameters are None, set them to the default value
+        donor = self._to_filter_str(donor)
+        recipient = self._to_filter_str(recipient)
+        measure = self._to_filter_str(measure)
+        unit_measure = self._to_filter_str(unit_measure)
+        price_base = self._to_filter_str(price_base)
+
+        return ".".join([donor, recipient, measure, unit_measure, price_base])
+
     def set_filter(self, filter_string: str) -> "QueryBuilder":
         """Set the dimensions parameter for the query.
 
         Args:
             filter_string (str): The filter string for the query.
 
         Returns:
```

### Comparing `oda_reader-0.0.9/oda_reader/schemas/dac1_codes_area.json` & `oda_reader-0.2.0/oda_reader/schemas/dac1_codes_area.json`

 * *Files identical despite different names*

### Comparing `oda_reader-0.0.9/oda_reader/schemas/dac1_dotstat.json` & `oda_reader-0.2.0/oda_reader/schemas/dac1_dotstat.json`

 * *Files identical despite different names*

### Comparing `oda_reader-0.0.9/oda_reader/schemas/dac1_translation.py` & `oda_reader-0.2.0/oda_reader/schemas/dac1_translation.py`

 * *Files identical despite different names*

### Comparing `oda_reader-0.0.9/oda_reader/schemas/dac2_codes_area.json` & `oda_reader-0.2.0/oda_reader/schemas/dac2_codes_area.json`

 * *Files identical despite different names*

### Comparing `oda_reader-0.0.9/oda_reader/schemas/dac2_translation.py` & `oda_reader-0.2.0/oda_reader/schemas/dac2_translation.py`

 * *Files identical despite different names*

### Comparing `oda_reader-0.0.9/oda_reader/schemas/dac2a_dotstat.json` & `oda_reader-0.2.0/oda_reader/schemas/dac2a_dotstat.json`

 * *Files identical despite different names*

### Comparing `oda_reader-0.0.9/oda_reader/schemas/schema_tools.py` & `oda_reader-0.2.0/oda_reader/schemas/schema_tools.py`

 * *Files identical despite different names*

### Comparing `oda_reader-0.0.9/oda_reader/schemas/xml_tools.py` & `oda_reader-0.2.0/oda_reader/schemas/xml_tools.py`

 * *Files identical despite different names*

### Comparing `oda_reader-0.0.9/PKG-INFO` & `oda_reader-0.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oda_reader
-Version: 0.0.9
+Version: 0.2.0
 Summary: A simple package to import ODA data using the OECD Data API
 License: MIT
 Author: Jorge Rivera
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

