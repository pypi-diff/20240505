# Comparing `tmp/shipyard_api-0.1.0.tar.gz` & `tmp/shipyard_api-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_api-0.1.0.tar", max compression
+gzip compressed data, was "shipyard_api-0.1.1a0.tar", max compression
```

## Comparing `shipyard_api-0.1.0.tar` & `shipyard_api-0.1.1a0.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0        0 2024-04-01 19:04:16.748551 shipyard_api-0.1.0/README.md
--rw-r--r--   0        0        0      500 2024-04-01 19:07:18.257559 shipyard_api-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       35 2024-04-01 19:04:16.750649 shipyard_api-0.1.0/shipyard_api/__init__.py
--rw-r--r--   0        0        0     1443 2024-04-01 19:07:37.465440 shipyard_api-0.1.0/shipyard_api/cli/get_logs.py
--rw-r--r--   0        0        0     4817 2024-04-01 19:20:08.795752 shipyard_api-0.1.0/shipyard_api/client.py
--rw-r--r--   0        0        0      927 2024-04-01 19:04:16.752038 shipyard_api-0.1.0/shipyard_api/errors.py
--rw-r--r--   0        0        0      529 1970-01-01 00:00:00.000000 shipyard_api-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-18 03:07:13.745323 shipyard_api-0.1.1a0/README.md
+-rw-r--r--   0        0        0      502 2024-05-04 16:19:05.680248 shipyard_api-0.1.1a0/pyproject.toml
+-rw-r--r--   0        0        0       35 2024-04-18 03:07:13.747259 shipyard_api-0.1.1a0/shipyard_api/__init__.py
+-rw-r--r--   0        0        0      695 2024-05-05 20:24:10.839576 shipyard_api-0.1.1a0/shipyard_api/cli/authtest.py
+-rw-r--r--   0        0        0     1443 2024-04-18 03:07:13.747671 shipyard_api-0.1.1a0/shipyard_api/cli/get_logs.py
+-rw-r--r--   0        0        0     2069 2024-05-05 20:24:10.874228 shipyard_api-0.1.1a0/shipyard_api/cli/trigger_fleet.py
+-rw-r--r--   0        0        0     5702 2024-05-05 20:24:10.896006 shipyard_api-0.1.1a0/shipyard_api/client.py
+-rw-r--r--   0        0        0      963 2024-05-04 16:10:17.090010 shipyard_api-0.1.1a0/shipyard_api/errors.py
+-rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 shipyard_api-0.1.1a0/PKG-INFO
```

### Comparing `shipyard_api-0.1.0/shipyard_api/cli/get_logs.py` & `shipyard_api-0.1.1a0/shipyard_api/cli/get_logs.py`

 * *Files identical despite different names*

### Comparing `shipyard_api-0.1.0/shipyard_api/client.py` & `shipyard_api-0.1.1a0/shipyard_api/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import requests
 import json
-from shipyard_bp_utils.files import create_folder_if_dne, combine_folder_and_file_name
 from shipyard_templates import ShipyardLogger, ExitCodeException
-from typing import Optional
+from typing import Optional, Dict, Any
 
 from shipyard_api.errors import (
     EXIT_CODE_LIST_FLEET_RUNS_ERROR,
     EXIT_CODE_VOYAGE_EXPORT_ERROR,
+    EXIT_CODE_TRIGGER_FLEET_ERROR,
     InvalidFileType,
     MissingProjectID,
     UnauthorizedAccess,
 )
 
 logger = ShipyardLogger.get_logger()
 
@@ -137,7 +137,35 @@
         except ExitCodeException:
             raise
 
         except Exception as e:
             raise ExitCodeException(
                 f"Error exporting voyages to file: {e}", EXIT_CODE_VOYAGE_EXPORT_ERROR
             )
+
+    def trigger_fleet(self, fleet_id: str) -> Dict[str, Any]:
+        """
+        Triggers a fleet run.
+
+        Args:
+            fleet_id (str): The ID of the fleet to trigger.
+
+        Returns:
+            dict: The response from the API.
+
+        Raises:
+            ExitCodeException: If an exit code exception occurs.
+        """
+        url = f"{self.base_url}/projects/{self.project_id}/fleets/{fleet_id}/fleetruns"
+        try:
+            response = requests.post(url, headers=self.headers)
+            logger.debug(f"Status code for fleet runs {response.status_code}")
+            response.raise_for_status()
+        except ExitCodeException:
+            raise
+        except Exception as e:
+            raise ExitCodeException(
+                f"Error trigger fleet {fleet_id} to run: {e}",
+                exit_code=EXIT_CODE_LIST_FLEET_RUNS_ERROR,
+            )
+        else:
+            return response.json()
```

### Comparing `shipyard_api-0.1.0/shipyard_api/errors.py` & `shipyard_api-0.1.1a0/shipyard_api/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 EXIT_CODE_MISSING_PROJECT_ID = 101
 EXIT_CODE_INVALID_FILE_TYPE = 102
 EXIT_CODE_UNAUTHORIZED_ACCESS = 103
 EXIT_CODE_LIST_FLEET_RUNS_ERROR = 104
 EXIT_CODE_LIST_VOYAGES_ERROR = 105
 EXIT_CODE_VOYAGE_EXPORT_ERROR = 106
+EXIT_CODE_TRIGGER_FLEET_ERROR = 107
 EXIT_CODE_UNKNOWN_ERROR = 249
 
 
 class MissingProjectID(ExitCodeException):
     def __init__(self):
         self.message = "Project ID is required in order to perform this operation"
         self.exit_code = EXIT_CODE_MISSING_PROJECT_ID
```

### Comparing `shipyard_api-0.1.0/PKG-INFO` & `shipyard_api-0.1.1a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-api
-Version: 0.1.0
+Version: 0.1.1a0
 Summary: 
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

