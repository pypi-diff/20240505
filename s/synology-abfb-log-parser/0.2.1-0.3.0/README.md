# Comparing `tmp/synology_abfb_log_parser-0.2.1.tar.gz` & `tmp/synology_abfb_log_parser-0.3.0.tar.gz`

## Comparing `synology_abfb_log_parser-0.2.1.tar` & `synology_abfb_log_parser-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.2.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.2.1/.idea/.gitignore
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.2.1/.idea/misc.xml
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.2.1/.idea/modules.xml
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.2.1/.idea/synology_abfb_log_parser.iml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.2.1/.idea/vcs.xml
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.2.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     7108 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.2.1/examples/README.md
--rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.2.1/examples/trmm-example-1.py
--rw-r--r--   0        0        0    10818 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.2.1/examples/trmm-example-2.py
--rw-r--r--   0        0        0     9519 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.2.1/examples/trmm-example-3.py
--rwxr-xr-x   0        0        0      477 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.2.1/scripts/deploy.sh
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.2.1/src/synology_abfb_log_parser/__about__.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.2.1/src/synology_abfb_log_parser/__init__.py
--rw-r--r--   0        0        0    12507 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.2.1/src/synology_abfb_log_parser/abfb_log_parser.py
--rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.2.1/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.2.1/LICENSE.md
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.2.1/README.md
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.3.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.3.0/.idea/.gitignore
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.3.0/.idea/misc.xml
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.3.0/.idea/modules.xml
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.3.0/.idea/synology_abfb_log_parser.iml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.3.0/.idea/vcs.xml
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.3.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     7108 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.3.0/examples/README.md
+-rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.3.0/examples/trmm-synology_abfb_auto_update.py
+-rw-r--r--   0        0        0    11206 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.3.0/examples/trmm-synology_abfb_backup_days_ago.py
+-rw-r--r--   0        0        0     9145 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.3.0/examples/trmm-synology_abfb_error_check.py
+-rw-r--r--   0        0        0     9863 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.3.0/examples/trmm-synology_abfb_not_complete.py
+-rwxr-xr-x   0        0        0      477 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.3.0/scripts/deploy.sh
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.3.0/src/synology_abfb_log_parser/__about__.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.3.0/src/synology_abfb_log_parser/__init__.py
+-rw-r--r--   0        0        0    12660 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.3.0/src/synology_abfb_log_parser/abfb_log_parser.py
+-rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.3.0/LICENSE.md
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.3.0/README.md
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 synology_abfb_log_parser-0.3.0/PKG-INFO
```

### Comparing `synology_abfb_log_parser-0.2.1/.github/workflows/publish.yml` & `synology_abfb_log_parser-0.3.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `synology_abfb_log_parser-0.2.1/examples/README.md` & `synology_abfb_log_parser-0.3.0/examples/README.md`

 * *Files identical despite different names*

### Comparing `synology_abfb_log_parser-0.2.1/examples/trmm-example-1.py` & `synology_abfb_log_parser-0.3.0/examples/trmm-synology_abfb_error_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,20 +22,23 @@
 This example will return the ERRORs in the logs. The default is to search for the last hour. This can be adjusted by
 using the --ago-unit and --ago-value parameters.
     --ago-unit=hours --ago-value=12 -> Search the logs for the past 12 hours.
     --ago-unit=days --ago-value=1 -> Search the logs for the past 1 day.
     --ago-unit=days --ago-value=7 -> Search the logs for the past 7 days.
     --ago-unit=weeks --ago-value=1 -> Same as above. Search the logs for the past 1 week.
 
-$ python3 trmm-example-1.py --help
-usage: trmm-example-1.py [-h]
-                         [--log-level {debug,info,warning,error,critical}]
-                         [--log-path LOG_PATH] [--log-glob LOG_GLOB]
-                         [--ago-unit AGO_UNIT] [--ago-value AGO_VALUE]
-                         [--auto-upgrade]
+$ python3 trmm-synology_abfb_error_check.py --help
+usage: trmm-synology_abfb_error_check.py [-h]
+                                         [--log-level {debug,info,warning,error,critical}]
+                                         [--log-path LOG_PATH]
+                                         [--log-glob LOG_GLOB]
+                                         [--ago-unit AGO_UNIT]
+                                         [--ago-value AGO_VALUE]
+                                         [--auto-upgrade]
+
 Parse the Synology Active Backup for Business logs.
 
 optional arguments:
   -h, --help            show this help message and exit
   --log-level {debug,info,warning,error,critical}
                         set log level for the Synology Active Backup for
                         Business module
@@ -51,14 +54,17 @@
 import argparse
 import logging
 import pkg_resources
 import subprocess
 import sys
 import traceback
 
+# Import the local copy for debugging purposes.
+# sys.path.append('/home/dev/projects/niceguyit/synology_abfb_log_parser/src')
+# import synology_abfb_log_parser
 
 def pip_install_upgrade(modules, logger=logging.getLogger(), upgrade=False):
     """
     Install or upgrade the specified Python modules using 'pip install'.
     :param modules: set of modules to install/upgrade
     :param logger: logging instance of the root logger
     :param upgrade: Bool If True, upgrade the modules.
@@ -80,27 +86,27 @@
         exit(1)
 
 
 # Check if the modules are installed
 try:
     import datetime
     import glob
-    import synology_abfb_log_parser
+    # import synology_abfb_log_parser
 except ModuleNotFoundError:
     required = {'synology_abfb_log_parser'}
     installed = {pkg.key for pkg in pkg_resources.working_set}
     missing = required - installed
     if missing:
         pip_install_upgrade(**{
             'modules': missing
         })
         # Import the modules if they were just installed. Duplicate imports are ignored.
         import datetime
         import glob
-        import synology_abfb_log_parser
+        # import synology_abfb_log_parser
 
 
 def main(logger=logging.getLogger(), ago_unit='days', ago_value=1, log_path=None, log_glob='log.txt*'):
     """
     Main program
     :param logger: logging instance of the root logger
     :param ago_unit: string Units of datetime.timedelta. One of ['weeks', 'days', 'hours', 'minutes', 'seconds']
@@ -162,17 +168,17 @@
 
             # Any [ERROR] record found indicates an error.
             errors_found = True
 
             # Always print the output, so it's visible to the users.
             print(f"{ts}: {event['priority']} {event['message']}")
         except TypeError as err:
-            logging.warning(f'Failed to check for key before using. Skipping this event. ERR: {err}')
-            logging.warning(traceback.format_exc())
-            logging.warning(f'Event: {event}')
+            logger.warning(f'Failed to check for key before using. Skipping this event. ERR: {err}')
+            logger.warning(traceback.format_exc())
+            logger.warning(f'Event: {event}')
             continue
 
     if errors_found:
         # Errors found. Exit with failure
         exit(1)
     else:
         # No errors found. Exit successful
```

### Comparing `synology_abfb_log_parser-0.2.1/examples/trmm-example-2.py` & `synology_abfb_log_parser-0.3.0/examples/trmm-synology_abfb_backup_days_ago.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,21 +21,23 @@
 
 This example will return logs where the "last_backup_status" is "complete" and "last_success_time" was more than
 '--complete-days-ago'. For example:
     --ago-unit=hours --ago-value=12 --complete-days-ago=3 -> Search the logs for the past 12 hours and return entries
         where the "backup_result.last_backup_status" is "complete" and "backup_result.last_success_time" was more than
         3 days ago.
 
-$ python3 trmm-example-2.py --help
-usage: trmm-example-2.py [-h]
-                         [--log-level {debug,info,warning,error,critical}]
-                         [--log-path LOG_PATH] [--log-glob LOG_GLOB]
-                         [--ago-unit AGO_UNIT] [--ago-value AGO_VALUE]
-                         [--complete-days-ago COMPLETE_DAYS_AGO]
-                         [--auto-upgrade]
+$ python3 trmm-synology_abfb_backup_days_ago.py --help
+usage: trmm-synology_abfb_backup_days_ago.py [-h]
+                                             [--log-level {debug,info,warning,error,critical}]
+                                             [--log-path LOG_PATH]
+                                             [--log-glob LOG_GLOB]
+                                             [--ago-unit AGO_UNIT]
+                                             [--ago-value AGO_VALUE]
+                                             [--complete-days-ago COMPLETE_DAYS_AGO]
+                                             [--auto-upgrade]
 
 Parse the Synology Active Backup for Business logs.
 
 optional arguments:
   -h, --help            show this help message and exit
   --log-level {debug,info,warning,error,critical}
                         set log level for the Synology Active Backup for
@@ -54,14 +56,17 @@
 import argparse
 import logging
 import pkg_resources
 import subprocess
 import sys
 import traceback
 
+# Import the local copy for debugging purposes.
+# sys.path.append('/home/dev/projects/niceguyit/synology_abfb_log_parser/src')
+# import synology_abfb_log_parser
 
 def pip_install_upgrade(modules, logger=logging.getLogger(), upgrade=False):
     """
     Install or upgrade the specified Python modules using 'pip install'.
     :param modules: set of modules to install/upgrade
     :param logger: logging instance of the root logger
     :param upgrade: Bool If True, upgrade the modules.
@@ -194,17 +199,17 @@
                     if 'transfered_bytes' in event['json']['running_task_result']:
                         transferred = event['json']['running_task_result']['transfered_bytes']
 
                 # Always print the output, so it's visible to the users.
                 print(f"{ts}: {event['json']['backup_result']}    Task name: '{task_name}'    Transferred: '{transferred}'    Days/Hours ago: {delta_backup}")
 
         except TypeError as err:
-            logging.warning(f'Failed to check for key before using. Skipping this event. ERR: {err}')
-            logging.warning(traceback.format_exc())
-            logging.warning(f'Event: {event}')
+            logger.warning(f'Failed to check for key before using. Skipping this event. ERR: {err}')
+            logger.warning(traceback.format_exc())
+            logger.warning(f'Event: {event}')
             continue
 
     if errors_found:
         # Errors found. Exit with failure
         exit(1)
     else:
         # No errors found. Exit successful
```

### Comparing `synology_abfb_log_parser-0.2.1/examples/trmm-example-3.py` & `synology_abfb_log_parser-0.3.0/examples/trmm-synology_abfb_not_complete.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,20 +19,22 @@
   --ago-unit hours --ago-value 3
 
 
 This example will return logs where the "last_backup_status" is *not* "complete". For example:
     --ago-unit=hours --ago-value=12 -> Search the logs for the past 12 hours and return entries
         where the "backup_result.last_backup_status" is not "complete".
 
-$ python3 trmm-example-3.py --help
-usage: trmm-example-3.py [-h]
-                         [--log-level {debug,info,warning,error,critical}]
-                         [--log-path LOG_PATH] [--log-glob LOG_GLOB]
-                         [--ago-unit AGO_UNIT] [--ago-value AGO_VALUE]
-                         [--auto-upgrade]
+$ python3 trmm-synology_abfb_not_complete.py --help
+usage: trmm-synology_abfb_not_complete.py [-h]
+                                          [--log-level {debug,info,warning,error,critical}]
+                                          [--log-path LOG_PATH]
+                                          [--log-glob LOG_GLOB]
+                                          [--ago-unit AGO_UNIT]
+                                          [--ago-value AGO_VALUE]
+                                          [--auto-upgrade]
 
 Parse the Synology Active Backup for Business logs.
 
 optional arguments:
   -h, --help            show this help message and exit
   --log-level {debug,info,warning,error,critical}
                         set log level for the Synology Active Backup for
@@ -49,14 +51,17 @@
 import argparse
 import logging
 import pkg_resources
 import subprocess
 import sys
 import traceback
 
+# Import the local copy for debugging purposes.
+# sys.path.append('/home/dev/projects/niceguyit/synology_abfb_log_parser/src')
+# import synology_abfb_log_parser
 
 def pip_install_upgrade(modules, logger=logging.getLogger(), upgrade=False):
     """
     Install or upgrade the specified Python modules using 'pip install'.
     :param modules: set of modules to install/upgrade
     :param logger: logging instance of the root logger
     :param upgrade: Bool If True, upgrade the modules.
@@ -179,17 +184,17 @@
             if event['json']['backup_result']['last_backup_status'] != 'complete':
                 errors_found = True
 
                 # Always print the output, so it's visible to the users.
                 print(f"{ts}: {event['json']['backup_result']}    Days/Hours ago: {delta_backup}")
 
         except TypeError as err:
-            logging.warning(f'Failed to check for key before using. Skipping this event. ERR: {err}')
-            logging.warning(traceback.format_exc())
-            logging.warning(f'Event: {event}')
+            logger.warning(f'Failed to check for key before using. Skipping this event. ERR: {err}')
+            logger.warning(traceback.format_exc())
+            logger.warning(f'Event: {event}')
             continue
 
     if errors_found:
         # Errors found. Exit with failure
         exit(1)
     else:
         # No errors found. Exit successful
```

### Comparing `synology_abfb_log_parser-0.2.1/src/synology_abfb_log_parser/abfb_log_parser.py` & `synology_abfb_log_parser-0.3.0/src/synology_abfb_log_parser/abfb_log_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,17 @@
         elif sys.platform == 'win32':
             self.__log_path = 'C:\\ProgramData\\ActiveBackupForBusinessAgent\\log'
         # Log path was provided
         if log_path:
             self.__log_path = log_path
 
         # __re_timestamp is a regular expression to extract the timestamp from the beginning of the logs.
-        self.__re_log_entry = re.compile(r'^(?P<month>\w{3}) (?P<day>\d+) (?P<time>[\d:]{8}) \[(?P<priority>\w+)] (?P<method_name>[\w.-]+) \((?P<method_num>\d+)\): ?(?P<message>.*)$')
+        # Note: timezone is optional and not used.
+        # TODO: Should the timezone be used when calculating the timestamp?
+        self.__re_log_entry = re.compile(r'^(?P<month>\w{3}) (?P<day>\d+) (?P<time>[\d:]{8}) (?P<timezone>[\d-]{5,})? ?\[(?P<priority>\w+)] (?P<method_name>[\w.-]+) \((?P<method_num>\d+)\): ?(?P<message>.*)$')
 
         # __now is a timestamp used to determine if the log entry is after "now". 1 minute is added for
         # processing time.
         self.__now = datetime.datetime.now() + datetime.timedelta(minutes=1)
 
         # __current_year is the current year and used to determine if the log entry is for this year or last year.
         # The logs do not contain the year.
```

### Comparing `synology_abfb_log_parser-0.2.1/.gitignore` & `synology_abfb_log_parser-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `synology_abfb_log_parser-0.2.1/LICENSE.md` & `synology_abfb_log_parser-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `synology_abfb_log_parser-0.2.1/pyproject.toml` & `synology_abfb_log_parser-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `synology_abfb_log_parser-0.2.1/PKG-INFO` & `synology_abfb_log_parser-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: synology_abfb_log_parser
-Version: 0.2.1
+Version: 0.3.0
 Summary: Synology Active Backup for Business log parser
 Project-URL: Homepage, https://github.com/NiceGuyIT/synology_abfb_log_parser
 Project-URL: Repository, https://github.com/NiceGuyIT/synology_abfb_log_parser
 Project-URL: Documentation, https://github.com/NiceGuyIT/synology_abfb_log_parser
 Project-URL: Bug Tracker, https://github.com/NiceGuyIT/synology_abfb_log_parser/issues
 Author-email: David Randall <David@NiceGuyIT.biz>
 License: Copyright (c) 2022 Nice Guy IT, LLC
@@ -57,7 +57,24 @@
     "method_num": "56",
     "message": "Worker (0): get event '1: routine {\"subaction\": \"heart_beat\"}', start processing",
     "json": {
         "subaction": "heart_beat"
     },
 }
 ```
+
+A simple script to print all ERRORs in the last 3 hours.
+```Python
+import datetime
+import synology_abfb_log_parser
+
+after = datetime.timedelta(**{"hours": 3})
+find = {
+    'priority': 'ERROR',
+}
+synology = synology_abfb_log_parser.abfb_log_parser.ActiveBackupLogParser(
+    after=after,
+)
+synology.load()
+found = synology.search(find=find)
+print(found)
+```
```

