# Comparing `tmp/inspy_logger-3.1.0.dev3.tar.gz` & `tmp/inspy_logger-3.1.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inspy_logger-3.1.0.dev3.tar", max compression
+gzip compressed data, was "inspy_logger-3.1.0.dev4.tar", max compression
```

## Comparing `inspy_logger-3.1.0.dev3.tar` & `inspy_logger-3.1.0.dev4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      501 2024-03-26 19:46:07.239938 inspy_logger-3.1.0.dev3/inspy_logger/__about__.py
--rw-r--r--   0        0        0     3516 2024-04-17 05:01:31.534752 inspy_logger-3.1.0.dev3/inspy_logger/__init__.py
--rw-r--r--   0        0        0     2503 2024-04-17 04:33:44.080244 inspy_logger-3.1.0.dev3/inspy_logger/common/__init__.py
--rw-r--r--   0        0        0     1067 2024-03-29 01:40:59.779229 inspy_logger-3.1.0.dev3/inspy_logger/common/meta.py
--rw-r--r--   0        0        0      211 2024-04-02 01:23:15.695772 inspy_logger-3.1.0.dev3/inspy_logger/config/__init__.py
--rw-r--r--   0        0        0     3754 2024-04-13 07:46:17.423404 inspy_logger-3.1.0.dev3/inspy_logger/config/dirs.py
--rw-r--r--   0        0        0      440 2024-04-02 01:25:49.145829 inspy_logger-3.1.0.dev3/inspy_logger/config/levels.py
--rw-r--r--   0        0        0      701 2024-04-18 02:24:15.649026 inspy_logger-3.1.0.dev3/inspy_logger/constants.py
--rw-r--r--   0        0        0    22753 2024-04-18 02:08:22.644940 inspy_logger-3.1.0.dev3/inspy_logger/engine/__init__.py
--rw-r--r--   0        0        0     1090 2024-04-01 23:37:24.100399 inspy_logger-3.1.0.dev3/inspy_logger/engine/errors.py
--rw-r--r--   0        0        0     1374 2024-01-06 00:11:42.646732 inspy_logger-3.1.0.dev3/inspy_logger/engine/handlers.py
--rw-r--r--   0        0        0     4239 2023-12-07 05:55:57.981004 inspy_logger-3.1.0.dev3/inspy_logger/errors/__init__.py
--rw-r--r--   0        0        0    15186 2024-04-04 10:49:26.067126 inspy_logger-3.1.0.dev3/inspy_logger/helpers/__init__.py
--rw-r--r--   0        0        0     5113 2024-04-18 00:57:14.681285 inspy_logger-3.1.0.dev3/inspy_logger/helpers/base_classes.py
--rw-r--r--   0        0        0     1094 2024-01-05 21:31:57.455076 inspy_logger-3.1.0.dev3/inspy_logger/helpers/command_line/__init__.py
--rw-r--r--   0        0        0        0 2023-12-21 18:01:40.981091 inspy_logger-3.1.0.dev3/inspy_logger/helpers/debug/__init__.py
--rw-r--r--   0        0        0     5054 2024-03-29 22:15:05.177429 inspy_logger-3.1.0.dev3/inspy_logger/helpers/debug/environment.py
--rw-r--r--   0        0        0        0 2023-12-24 09:42:32.088107 inspy_logger-3.1.0.dev3/inspy_logger/helpers/debug/system/__init__.py
--rw-r--r--   0        0        0     1650 2023-12-24 22:55:21.616920 inspy_logger-3.1.0.dev3/inspy_logger/helpers/debug/system/processor/__init__.py
--rw-r--r--   0        0        0      572 2023-12-24 22:25:41.517257 inspy_logger-3.1.0.dev3/inspy_logger/helpers/debug/system/winx/__init__.py
--rw-r--r--   0        0        0     9992 2024-04-18 02:13:36.979935 inspy_logger-3.1.0.dev3/inspy_logger/helpers/decorators.py
--rw-r--r--   0        0        0     9924 2024-03-29 22:36:21.862636 inspy_logger-3.1.0.dev3/inspy_logger/helpers/descriptors.py
--rw-r--r--   0        0        0    10631 2023-12-19 01:27:51.212244 inspy_logger-3.1.0.dev3/inspy_logger/helpers/network.py
--rw-r--r--   0        0        0     2175 2023-12-25 21:32:04.611127 inspy_logger-3.1.0.dev3/inspy_logger/helpers/units.py
--rw-r--r--   0        0        0      992 2023-12-07 05:54:44.333226 inspy_logger-3.1.0.dev3/inspy_logger/manifest.py
--rw-r--r--   0        0        0     2857 2024-03-25 23:00:48.439094 inspy_logger-3.1.0.dev3/inspy_logger/Scripts/main.py
--rw-r--r--   0        0        0      681 2024-03-29 22:07:26.428504 inspy_logger-3.1.0.dev3/inspy_logger/system/__init__.py
--rw-r--r--   0        0        0      424 2024-03-29 18:16:16.092498 inspy_logger-3.1.0.dev3/inspy_logger/system/linux.py
--rw-r--r--   0        0        0      243 2024-03-29 18:16:16.078641 inspy_logger-3.1.0.dev3/inspy_logger/system/mac_os.py
--rw-r--r--   0        0        0      960 2024-03-30 21:12:18.256135 inspy_logger-3.1.0.dev3/inspy_logger/system/win32.py
--rw-r--r--   0        0        0       57 2024-04-18 02:28:14.309687 inspy_logger-3.1.0.dev3/inspy_logger/tool/__init__.py
--rw-r--r--   0        0        0        0 2024-01-04 00:55:12.726772 inspy_logger-3.1.0.dev3/inspy_logger/tool/config/__init__.py
--rw-r--r--   0        0        0     2247 2024-01-06 00:31:51.966217 inspy_logger-3.1.0.dev3/inspy_logger/tool/config/arguments/__init__.py
--rw-r--r--   0        0        0     4305 2024-04-17 04:21:12.630792 inspy_logger-3.1.0.dev3/inspy_logger/types.py
--rw-r--r--   0        0        0    14877 2024-04-16 04:16:50.614788 inspy_logger-3.1.0.dev3/inspy_logger/version/__init__.py
--rw-r--r--   0        0        0       13 2024-04-17 04:33:44.061283 inspy_logger-3.1.0.dev3/inspy_logger/version/VERSION.txt
--rw-r--r--   0        0        0      885 2023-12-07 05:54:44.295896 inspy_logger-3.1.0.dev3/LICENSE.md
--rw-r--r--   0        0        0     2304 2024-04-15 23:22:34.276364 inspy_logger-3.1.0.dev3/pyproject.toml
--rw-r--r--   0        0        0     2500 2023-12-07 05:54:44.296909 inspy_logger-3.1.0.dev3/README.md
--rw-r--r--   0        0        0     4328 1970-01-01 00:00:00.000000 inspy_logger-3.1.0.dev3/PKG-INFO
+-rw-r--r--   0        0        0      525 2024-05-02 23:28:28.825169 inspy_logger-3.1.0.dev4/inspy_logger/__about__.py
+-rw-r--r--   0        0        0     3653 2024-05-02 23:28:28.825169 inspy_logger-3.1.0.dev4/inspy_logger/__init__.py
+-rw-r--r--   0        0        0     2503 2024-05-02 23:28:28.826174 inspy_logger-3.1.0.dev4/inspy_logger/common/__init__.py
+-rw-r--r--   0        0        0     1067 2024-04-30 21:33:35.911811 inspy_logger-3.1.0.dev4/inspy_logger/common/meta.py
+-rw-r--r--   0        0        0      211 2024-04-30 21:33:35.912812 inspy_logger-3.1.0.dev4/inspy_logger/config/__init__.py
+-rw-r--r--   0        0        0     3887 2024-05-02 23:28:28.826174 inspy_logger-3.1.0.dev4/inspy_logger/config/dirs.py
+-rw-r--r--   0        0        0      440 2024-04-30 21:33:35.912812 inspy_logger-3.1.0.dev4/inspy_logger/config/levels.py
+-rw-r--r--   0        0        0      701 2024-05-02 23:28:28.826174 inspy_logger-3.1.0.dev4/inspy_logger/constants.py
+-rw-r--r--   0        0        0    23698 2024-05-02 23:30:29.503037 inspy_logger-3.1.0.dev4/inspy_logger/engine/__init__.py
+-rw-r--r--   0        0        0     1090 2024-04-30 21:33:35.913812 inspy_logger-3.1.0.dev4/inspy_logger/engine/errors.py
+-rw-r--r--   0        0        0     1380 2024-05-02 23:28:28.827172 inspy_logger-3.1.0.dev4/inspy_logger/engine/handlers.py
+-rw-r--r--   0        0        0     4360 2024-04-30 21:33:35.914812 inspy_logger-3.1.0.dev4/inspy_logger/errors/__init__.py
+-rw-r--r--   0        0        0    15776 2024-05-02 23:28:28.827172 inspy_logger-3.1.0.dev4/inspy_logger/helpers/__init__.py
+-rw-r--r--   0        0        0     5228 2024-05-02 23:35:42.609841 inspy_logger-3.1.0.dev4/inspy_logger/helpers/base_classes.py
+-rw-r--r--   0        0        0     1094 2024-04-30 21:33:35.914812 inspy_logger-3.1.0.dev4/inspy_logger/helpers/command_line/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:33:35.916320 inspy_logger-3.1.0.dev4/inspy_logger/helpers/debug/__init__.py
+-rw-r--r--   0        0        0     5054 2024-04-30 21:33:35.916320 inspy_logger-3.1.0.dev4/inspy_logger/helpers/debug/environment.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:33:35.916320 inspy_logger-3.1.0.dev4/inspy_logger/helpers/debug/system/__init__.py
+-rw-r--r--   0        0        0     1650 2024-04-30 21:33:35.916320 inspy_logger-3.1.0.dev4/inspy_logger/helpers/debug/system/processor/__init__.py
+-rw-r--r--   0        0        0      572 2024-04-30 21:33:35.917327 inspy_logger-3.1.0.dev4/inspy_logger/helpers/debug/system/winx/__init__.py
+-rw-r--r--   0        0        0    10028 2024-05-02 23:28:28.828547 inspy_logger-3.1.0.dev4/inspy_logger/helpers/decorators.py
+-rw-r--r--   0        0        0     9924 2024-04-30 21:33:35.918329 inspy_logger-3.1.0.dev4/inspy_logger/helpers/descriptors.py
+-rw-r--r--   0        0        0    11031 2024-05-02 23:28:28.828547 inspy_logger-3.1.0.dev4/inspy_logger/helpers/network.py
+-rw-r--r--   0        0        0     2181 2024-05-02 23:28:28.829717 inspy_logger-3.1.0.dev4/inspy_logger/helpers/units.py
+-rw-r--r--   0        0        0     1032 2024-04-30 21:33:35.918329 inspy_logger-3.1.0.dev4/inspy_logger/manifest.py
+-rw-r--r--   0        0        0     2857 2024-05-02 23:28:28.824162 inspy_logger-3.1.0.dev4/inspy_logger/Scripts/main.py
+-rw-r--r--   0        0        0      681 2024-04-30 21:33:35.919336 inspy_logger-3.1.0.dev4/inspy_logger/system/__init__.py
+-rw-r--r--   0        0        0      424 2024-04-30 21:33:35.919336 inspy_logger-3.1.0.dev4/inspy_logger/system/linux.py
+-rw-r--r--   0        0        0      243 2024-04-30 21:33:35.919336 inspy_logger-3.1.0.dev4/inspy_logger/system/mac_os.py
+-rw-r--r--   0        0        0      960 2024-04-30 21:33:35.919336 inspy_logger-3.1.0.dev4/inspy_logger/system/win32.py
+-rw-r--r--   0        0        0       57 2024-05-02 23:28:28.829717 inspy_logger-3.1.0.dev4/inspy_logger/tool/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:33:35.920336 inspy_logger-3.1.0.dev4/inspy_logger/tool/config/__init__.py
+-rw-r--r--   0        0        0     2247 2024-04-30 21:33:35.920336 inspy_logger-3.1.0.dev4/inspy_logger/tool/config/arguments/__init__.py
+-rw-r--r--   0        0        0     4305 2024-05-02 23:28:28.829717 inspy_logger-3.1.0.dev4/inspy_logger/types.py
+-rw-r--r--   0        0        0    14877 2024-05-02 23:28:28.829717 inspy_logger-3.1.0.dev4/inspy_logger/version/__init__.py
+-rw-r--r--   0        0        0       13 2024-05-05 06:30:39.752532 inspy_logger-3.1.0.dev4/inspy_logger/version/VERSION.txt
+-rw-r--r--   0        0        0      905 2024-04-30 21:33:35.879233 inspy_logger-3.1.0.dev4/LICENSE.md
+-rw-r--r--   0        0        0     2377 2024-05-05 06:37:44.329415 inspy_logger-3.1.0.dev4/pyproject.toml
+-rw-r--r--   0        0        0     2554 2024-04-30 21:33:35.879233 inspy_logger-3.1.0.dev4/README.md
+-rw-r--r--   0        0        0     4370 1970-01-01 00:00:00.000000 inspy_logger-3.1.0.dev4/PKG-INFO
```

### Comparing `inspy_logger-3.1.0.dev3/inspy_logger/__init__.py` & `inspy_logger-3.1.0.dev4/inspy_logger/__init__.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,137 +1,137 @@
-#!/usr/bin/env python3
-import contextlib
-import sys
-import inspect
-import logging
-from pypattyrn.behavioral.null import Null
-from inspy_logger.common import PROG_NAME as ISL_PROG_NAME, DEFAULT_LOGGING_LEVEL, DEFAULT_LOG_FILE_PATH, LEVELS
-from inspy_logger.helpers import find_variable_in_call_stack, check_preemptive_level_set, find_argument_parser, determine_start_block, determine_level
-
-from inspy_logger.helpers import (
-    translate_to_logging_level,
-    clean_module_name,
-    CustomFormatter,
-    determine_client_prog_name,
-    determine_log_file_path
-)
-
-# Existing log record factory
-old_factory = logging.getLogRecordFactory()
-
-
-def record_factory(*args, **kwargs):
-    record = old_factory(*args, **kwargs)
-    # Set the file_name attribute to the name of the file where the log is called
-    frame = inspect.stack()[1]
-    record.file_name = frame.filename
-    return record
-
-
-logging.setLogRecordFactory(record_factory)
-
-
-from inspy_logger.engine import Logger
-
-__all__ = [
-    "clean_module_name",
-    "CustomFormatter",
-    "DEFAULT_LOGGING_LEVEL",
-    "determine_level",
-    "InspyLogger",
-    "LOG_DEVICE",
-    "Logger",
-    "ISL_PROG_NAME",
-    "translate_to_logging_level",
-]
-
-BLOCKED = determine_start_block()
-
-LOG_FILE = determine_log_file_path()
-
-LOG_DEVICE = None if BLOCKED else Logger(ISL_PROG_NAME)
-
-MODULE_OBJ = sys.modules[__name__]
-
-CLIENT_PROG_NAME = determine_client_prog_name()
-
-INIT_LOG_LEVEL = determine_level(CLIENT_PROG_NAME)
-
-INTERACTIVE_SESSION = find_variable_in_call_stack('INSPY_INTERACTIVE_SESSION', default=False)
-
-
-def start_logger(override_block=True):
-    """
-    Starts the logger.
-
-    Parameters:
-        override_block (Union[bool, None], optional):
-            A flag to override the block on the logger. Defaults to True.
-
-    Note:
-        You only need to run this function if you have blocked the logger from starting automatically.
-
-    Returns:
-
-    """
-    global LOG_DEVICE
-    global CLIENT_PROG_NAME
-    global INIT_LOG_LEVEL
-
-    if not BLOCKED or override_block:
-        LOG_DEVICE = Logger(ISL_PROG_NAME)
-        LOG_DEVICE.set_level(INIT_LOG_LEVEL)
-
-        if CLIENT_PROG_NAME:
-
-            prog_logger = Logger(
-                CLIENT_PROG_NAME,
-                LOG_DEVICE.console_level,
-                LOG_DEVICE.file_level,
-                file_name=DEFAULT_LOG_FILE_PATH.name,
-                file_path=DEFAULT_LOG_FILE_PATH.parent
-            )
-            __all__.append('PROG_LOGGER')
-
-        LOG_DEVICE.replay_and_setup_handlers()
-    elif CLIENT_PROG_NAME:
-        prog_logger = Null()
-
-    with contextlib.suppress(NameError):
-        global PROG_LOGGER
-
-        PROG_LOGGER = prog_logger
-
-        if isinstance(PROG_LOGGER, Null):
-            from rich import print
-            print("The logger has been blocked from starting. To start the logger, run `start_logger()`.")
-        
-
-InspyLogger = Logger
-
-
-def _get_loggable():
-    from inspy_logger.helpers.base_classes import Loggable
-    import bisect
-    # Add the `Loggable` class to `__all__` in alphabetical order.
-    bisect.insort(__all__, 'Loggable')
-
-    return Loggable
-
-
-Loggable = _get_loggable()
-
-
-start_logger(override_block=False)
-
-
-deprecation_warning_deliveries = 0
-
-
-def getLogger(*args, **kwargs):
-    global deprecation_warning_deliveries
-
-    if deprecation_warning_deliveries < 5:
-        LOG_DEVICE.warning('The `getLogger` function is deprecated. Use `InspyLogger` instead.')
-        deprecation_warning_deliveries += 1
-
-    return InspyLogger(*args, **kwargs)
+#!/usr/bin/env python3
+import contextlib
+import sys
+import inspect
+import logging
+from pypattyrn.behavioral.null import Null
+from inspy_logger.common import PROG_NAME as ISL_PROG_NAME, DEFAULT_LOGGING_LEVEL, DEFAULT_LOG_FILE_PATH, LEVELS
+from inspy_logger.helpers import find_variable_in_call_stack, check_preemptive_level_set, find_argument_parser, determine_start_block, determine_level
+
+from inspy_logger.helpers import (
+    translate_to_logging_level,
+    clean_module_name,
+    CustomFormatter,
+    determine_client_prog_name,
+    determine_log_file_path
+)
+
+# Existing log record factory
+old_factory = logging.getLogRecordFactory()
+
+
+def record_factory(*args, **kwargs):
+    record = old_factory(*args, **kwargs)
+    # Set the file_name attribute to the name of the file where the log is called
+    frame = inspect.stack()[1]
+    record.file_name = frame.filename
+    return record
+
+
+logging.setLogRecordFactory(record_factory)
+
+
+from inspy_logger.engine import Logger
+
+__all__ = [
+    "clean_module_name",
+    "CustomFormatter",
+    "DEFAULT_LOGGING_LEVEL",
+    "determine_level",
+    "InspyLogger",
+    "LOG_DEVICE",
+    "Logger",
+    "ISL_PROG_NAME",
+    "translate_to_logging_level",
+]
+
+BLOCKED = determine_start_block()
+
+LOG_FILE = determine_log_file_path()
+
+LOG_DEVICE = None if BLOCKED else Logger(ISL_PROG_NAME)
+
+MODULE_OBJ = sys.modules[__name__]
+
+CLIENT_PROG_NAME = determine_client_prog_name()
+
+INIT_LOG_LEVEL = determine_level(CLIENT_PROG_NAME)
+
+INTERACTIVE_SESSION = find_variable_in_call_stack('INSPY_INTERACTIVE_SESSION', default=False)
+
+
+def start_logger(override_block=True):
+    """
+    Starts the logger.
+
+    Parameters:
+        override_block (Union[bool, None], optional):
+            A flag to override the block on the logger. Defaults to True.
+
+    Note:
+        You only need to run this function if you have blocked the logger from starting automatically.
+
+    Returns:
+
+    """
+    global LOG_DEVICE
+    global CLIENT_PROG_NAME
+    global INIT_LOG_LEVEL
+
+    if not BLOCKED or override_block:
+        LOG_DEVICE = Logger(ISL_PROG_NAME)
+        LOG_DEVICE.set_level(INIT_LOG_LEVEL)
+
+        if CLIENT_PROG_NAME:
+
+            prog_logger = Logger(
+                CLIENT_PROG_NAME,
+                LOG_DEVICE.console_level,
+                LOG_DEVICE.file_level,
+                file_name=DEFAULT_LOG_FILE_PATH.name,
+                file_path=DEFAULT_LOG_FILE_PATH.parent
+            )
+            __all__.append('PROG_LOGGER')
+
+        LOG_DEVICE.replay_and_setup_handlers()
+    elif CLIENT_PROG_NAME:
+        prog_logger = Null()
+
+    with contextlib.suppress(NameError):
+        global PROG_LOGGER
+
+        PROG_LOGGER = prog_logger
+
+        if isinstance(PROG_LOGGER, Null):
+            from rich import print
+            print("The logger has been blocked from starting. To start the logger, run `start_logger()`.")
+        
+
+InspyLogger = Logger
+
+
+def _get_loggable():
+    from inspy_logger.helpers.base_classes import Loggable
+    import bisect
+    # Add the `Loggable` class to `__all__` in alphabetical order.
+    bisect.insort(__all__, 'Loggable')
+
+    return Loggable
+
+
+Loggable = _get_loggable()
+
+
+start_logger(override_block=False)
+
+
+deprecation_warning_deliveries = 0
+
+
+def getLogger(*args, **kwargs):
+    global deprecation_warning_deliveries
+
+    if deprecation_warning_deliveries < 5:
+        LOG_DEVICE.warning('The `getLogger` function is deprecated. Use `InspyLogger` instead.')
+        deprecation_warning_deliveries += 1
+
+    return InspyLogger(*args, **kwargs)
```

### Comparing `inspy_logger-3.1.0.dev3/inspy_logger/common/__init__.py` & `inspy_logger-3.1.0.dev4/inspy_logger/common/__init__.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev3/inspy_logger/common/meta.py` & `inspy_logger-3.1.0.dev4/inspy_logger/common/meta.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev3/inspy_logger/config/dirs.py` & `inspy_logger-3.1.0.dev4/inspy_logger/config/dirs.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-from platformdirs import user_log_path
-from pathlib import Path
-from inspy_logger.common.meta import *
-from inspy_logger.helpers import (
-    find_valid_vars_in_call_stack,
-    VALID_LOG_FILE_VARS,
-    VALID_PROG_NAME_VARS,
-    determine_log_file_path,
-    determine_client_prog_name,
-    VALID_DEV_NAME_VARS
-)
-
-from typing import Optional, Union
-
-
-INSPY_LOGGER_LOG_DIR_PATH = user_log_path(
-    appname=PROG_NAME or find_valid_vars_in_call_stack(VALID_PROG_NAME_VARS),
-    appauthor=SOFTWARE_ORG
-)
-
-INSPY_LOGGER_LOG_FILE_NAME = 'app.log'
-
-INSPY_LOGGER_LOG_FILE_PATH = INSPY_LOGGER_LOG_DIR_PATH.joinpath(INSPY_LOGGER_LOG_FILE_NAME)
-
-
-# def get_log_file_path(
-#         log_file_path: Union[str, Path] = None,
-#         prog_name: str = None,
-#         dev_name: str = None
-# ) -> Path:
-#     """
-#     Get the path to the log file.
-#
-#     Parameters:
-#         log_file_path (str, Path, optional):
-#                The path to the log file.
-#
-#         prog_name (str):
-#             The name of the program to be logged.
-#
-#         dev_name (str):
-#             The name of the developer of the app to be logged.
-#
-#     Note:
-#         The `log_file_name` is simply the name of the file to be logged to, not the full path.
-#
-#     Returns:
-#         Path:
-#             The path to the log file.
-#     """
-#     print(f'Found log-file path: {FOUND_LOG_FILE_VARS}')
-#     log_file_path = log_file_path or FOUND_LOG_FILE_VARS
-#     log_file_path = Path(log_file_path) if log_file_path else None
-#
-#     if not log_file_path:
-#         if not prog_name:
-#             prog_name = determine_client_prog_name()
-#             print(f'Found prog-name: {prog_name}')
-#         if prog_name and not dev_name:
-#             dev_name = find_valid_vars_in_call_stack(VALID_DEV_NAME_VARS.valid_vars)
-#
-#             if dev_name:
-#                 print(f'Found dev-name: {dev_name}')
-#
-#
-#
-#
-#     #if not log_file_path.suffix and log_file_path.is_dir() and INSPY_LOGGER_LOG_FILE_NAME:
-#     #    log_file_path = log_file_path.joinpath(INSPY_LOGGER_LOG_FILE_NAME)
-#
-#     if all(arg is None for arg in [
-#         log_file_path,
-#         prog_name,
-#         dev_name
-#     ]):
-#         return INSPY_LOGGER_LOG_FILE_PATH
-#
-#     return log_file_path
-
-
-def get_log_file_path(
-        log_file_path: Union[str, Path] = None,
-        prog_name: str = None,
-        dev_name: str = None
-) -> Path:
-    """
-    Get the path to the log file.
-
-    Parameters:
-        log_file_path (str, Path, optional):
-               The path to the log file.
-
-        prog_name (str):
-            The name of the program to be logged.
-
-        dev_name (str):
-            The name of the developer of the app to be logged.
-
-    Note:
-        The `log_file_name` is simply the name of the file to be logged to, not the full path.
-
-    Returns:
-        Path:
-            The path to the log file.
-    """
-    log_file_path = Path(log_file_path) if isinstance(log_file_path, str) else log_file_path
-
-    if log_file_path:
-        return log_file_path
-
-    log_file_path = find_valid_vars_in_call_stack(VALID_LOG_FILE_VARS)
-
-    if log_file_path:
-        log_file_path = Path(log_file_path)
-        return log_file_path
-
-    if not prog_name:
-        prog_name = determine_client_prog_name()
-
-    if not dev_name and prog_name:
-        dev_name = find_valid_vars_in_call_stack(VALID_DEV_NAME_VARS.valid_vars)
-
-    if prog_name:
-        file_name = f"{prog_name}.log"
-        if dev_name:
-            log_file_path = Path(user_log_path(appname=prog_name, appauthor=dev_name).joinpath(file_name))
-        else:
-            log_file_path = INSPY_LOGGER_LOG_DIR_PATH.joinpath(file_name)
-
-    return log_file_path or INSPY_LOGGER_LOG_FILE_PATH
-
-
-DEFAULT_LOG_FILE_PATH = get_log_file_path()
+from platformdirs import user_log_path
+from pathlib import Path
+from inspy_logger.common.meta import *
+from inspy_logger.helpers import (
+    find_valid_vars_in_call_stack,
+    VALID_LOG_FILE_VARS,
+    VALID_PROG_NAME_VARS,
+    determine_log_file_path,
+    determine_client_prog_name,
+    VALID_DEV_NAME_VARS
+)
+
+from typing import Optional, Union
+
+
+INSPY_LOGGER_LOG_DIR_PATH = user_log_path(
+    appname=PROG_NAME or find_valid_vars_in_call_stack(VALID_PROG_NAME_VARS),
+    appauthor=SOFTWARE_ORG
+)
+
+INSPY_LOGGER_LOG_FILE_NAME = 'app.log'
+
+INSPY_LOGGER_LOG_FILE_PATH = INSPY_LOGGER_LOG_DIR_PATH.joinpath(INSPY_LOGGER_LOG_FILE_NAME)
+
+
+# def get_log_file_path(
+#         log_file_path: Union[str, Path] = None,
+#         prog_name: str = None,
+#         dev_name: str = None
+# ) -> Path:
+#     """
+#     Get the path to the log file.
+#
+#     Parameters:
+#         log_file_path (str, Path, optional):
+#                The path to the log file.
+#
+#         prog_name (str):
+#             The name of the program to be logged.
+#
+#         dev_name (str):
+#             The name of the developer of the app to be logged.
+#
+#     Note:
+#         The `log_file_name` is simply the name of the file to be logged to, not the full path.
+#
+#     Returns:
+#         Path:
+#             The path to the log file.
+#     """
+#     print(f'Found log-file path: {FOUND_LOG_FILE_VARS}')
+#     log_file_path = log_file_path or FOUND_LOG_FILE_VARS
+#     log_file_path = Path(log_file_path) if log_file_path else None
+#
+#     if not log_file_path:
+#         if not prog_name:
+#             prog_name = determine_client_prog_name()
+#             print(f'Found prog-name: {prog_name}')
+#         if prog_name and not dev_name:
+#             dev_name = find_valid_vars_in_call_stack(VALID_DEV_NAME_VARS.valid_vars)
+#
+#             if dev_name:
+#                 print(f'Found dev-name: {dev_name}')
+#
+#
+#
+#
+#     #if not log_file_path.suffix and log_file_path.is_dir() and INSPY_LOGGER_LOG_FILE_NAME:
+#     #    log_file_path = log_file_path.joinpath(INSPY_LOGGER_LOG_FILE_NAME)
+#
+#     if all(arg is None for arg in [
+#         log_file_path,
+#         prog_name,
+#         dev_name
+#     ]):
+#         return INSPY_LOGGER_LOG_FILE_PATH
+#
+#     return log_file_path
+
+
+def get_log_file_path(
+        log_file_path: Union[str, Path] = None,
+        prog_name: str = None,
+        dev_name: str = None
+) -> Path:
+    """
+    Get the path to the log file.
+
+    Parameters:
+        log_file_path (str, Path, optional):
+               The path to the log file.
+
+        prog_name (str):
+            The name of the program to be logged.
+
+        dev_name (str):
+            The name of the developer of the app to be logged.
+
+    Note:
+        The `log_file_name` is simply the name of the file to be logged to, not the full path.
+
+    Returns:
+        Path:
+            The path to the log file.
+    """
+    log_file_path = Path(log_file_path) if isinstance(log_file_path, str) else log_file_path
+
+    if log_file_path:
+        return log_file_path
+
+    log_file_path = find_valid_vars_in_call_stack(VALID_LOG_FILE_VARS)
+
+    if log_file_path:
+        log_file_path = Path(log_file_path)
+        return log_file_path
+
+    if not prog_name:
+        prog_name = determine_client_prog_name()
+
+    if not dev_name and prog_name:
+        dev_name = find_valid_vars_in_call_stack(VALID_DEV_NAME_VARS.valid_vars)
+
+    if prog_name:
+        file_name = f"{prog_name}.log"
+        if dev_name:
+            log_file_path = Path(user_log_path(appname=prog_name, appauthor=dev_name).joinpath(file_name))
+        else:
+            log_file_path = INSPY_LOGGER_LOG_DIR_PATH.joinpath(file_name)
+
+    return log_file_path or INSPY_LOGGER_LOG_FILE_PATH
+
+
+DEFAULT_LOG_FILE_PATH = get_log_file_path()
```

### Comparing `inspy_logger-3.1.0.dev3/inspy_logger/constants.py` & `inspy_logger-3.1.0.dev4/inspy_logger/constants.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev3/inspy_logger/engine/__init__.py` & `inspy_logger-3.1.0.dev4/inspy_logger/engine/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,725 +1,729 @@
-import inspect
-import os
-import logging
-import sys
-
-from rich.logging import RichHandler
-
-from inspy_logger.config import DEFAULT_LOG_FILE_PATH
-from inspy_logger.constants import LEVELS, INTERACTIVE_SESSION, INTERNAL
-from inspy_logger.engine.handlers import BufferingHandler
-from inspy_logger.common import InspyLogger, DEFAULT_LOGGING_LEVEL
-from inspy_logger.helpers import translate_to_logging_level, CustomFormatter, get_level_name, RestrictedSetter
-from inspy_logger.helpers.decorators import add_aliases, method_alias, count_invocations, validate_type
-from typing import List, Union, Optional
-from pathlib import Path
-
-
-@add_aliases
-class Logger(InspyLogger):
-    """
-    A Singleton class responsible for managing the logging mechanisms of the application.
-    """
-
-    LEVELS = LEVELS
-    INTERACTIVE_SESSION = INTERACTIVE_SESSION
-    instances = {}  # A dictionary to hold instances of the Logger class.
-
-    # Set the file path for the log file.
-    file_path = RestrictedSetter('file_path', DEFAULT_LOG_FILE_PATH, allowed_types=(str, Path),preferred_type=Path)
-
-    def __new__(cls, name, *args, **kwargs):
-        """
-        Creates or returns an existing instance of the Logger class for the provided name.
-
-        Args:
-            name (str): The name of the logger instance.
-
-        Returns:
-            Logger: An instance of the Logger class.
-        """
-
-        if name not in cls.instances:
-            instance = super(Logger, cls).__new__(cls)
-            cls.instances[name] = instance
-            return instance
-        return cls.instances[name]
-
-    def __init__(
-            self,
-            name,
-            auto_set_up=True,
-            console_level=DEFAULT_LOGGING_LEVEL,
-            file_level=logging.DEBUG,
-            file_name="app.log",
-            file_path=DEFAULT_LOG_FILE_PATH.parent,
-            no_file_logging=False,
-            parent=None,
-            skip_interactive_check: bool=False
-    ):
-        """
-        Initializes a logger instance.
-
-        Parameters:
-            name (str):
-                The name of the logger instance.
-
-            auto_set_up (bool, optional):
-                Whether to automatically set up the handlers for the logger. Defaults to True.
-
-            console_level (str, optional):
-                The logging level for the console. Defaults to DEFAULT_LOGGING_LEVEL.
-
-            file_level (str, optional):
-                The logging level for the file. Defaults to logging.DEBUG.
-
-            file_name (str, optional):
-                The name of the log file. Defaults to "app.log".
-
-            no_file_logging (bool, optional):
-                Whether to disable file logging. Defaults to False.
-
-            parent (Logger, optional):
-                The parent logger instance. Defaults to None.
-        """
-        # Check if the logger has already been initialized.
-        if hasattr(self, 'logger'):
-            return
-
-        self.__call_counts = {}
-
-        self.__console_level = translate_to_logging_level(console_level)
-        self.__file_level = translate_to_logging_level(file_level)
-
-        self.__children = []
-
-        self.__name = name
-        self.__no_file_logging = None
-        self.__file_path = None
-
-
-        self.logger = logging.getLogger(name)
-        self.logger.setLevel(translate_to_logging_level(console_level))
-
-        self.logger.propagate = False
-        self.logger.start = self.start
-
-        if 'inSPy-Logger' in self.logger.name:
-            self.buffering_handler = BufferingHandler()
-            self.logger.addHandler(self.buffering_handler)
-            self.internal('Initializing logger with buffering handler.')
-        else:
-            self.internal('Initializing  logger without buffering handler.')
-
-        self.no_file_logging = no_file_logging
-
-        self.set_file_path = Path(file_path).expanduser().absolute().joinpath(file_name)
-
-        self.parent = parent
-
-        if not getattr(self, 'buffering_handler', None):
-            self.set_up_handlers()
-
-    @property
-    def call_counts(self):
-        """
-        Property to get the call counts of decorated methods.
-
-        Returns:
-            dict:
-                A dictionary containing the call counts of decorated methods.
-
-        """
-        return self.__call_counts
-
-    @property
-    def child_names(self):
-        return self.get_child_names()
-
-    @property
-    def children(self):
-        return self.__children
-
-    @children.deleter
-    def children(self):
-        self.__children = []
-
-    @property
-    def console_level(self):
-        """
-        Returns the logging level for the console.
-
-        Returns:
-            int:
-                The logging level for the console.
-        """
-        return self.__console_level
-
-    @console_level.setter
-    def console_level(self, level):
-        """
-        Sets the logging level for the console.
-
-        Args:
-            level:
-                The logging level for the console.
-
-        Returns:
-
-        """
-        self.set_level(console_level=translate_to_logging_level(level))
-
-    @property
-    def console_level_name(self):
-        self.internal('Test message')
-        return get_level_name(self.console_level)
-
-    @property
-    def device(self):
-        """
-        Returns the logger instance.
-
-        Returns:
-            Logger:
-                The logger instance.
-        """
-        logger = self
-        logger.start = self.start.__get__(logger)
-        return logger
-
-    @property
-    def file_level(self):
-        """
-        Returns the logging level for the file.
-
-        Returns:
-            int:
-                The logging level for the file.
-        """
-        return self.__file_level
-
-    @file_level.setter
-    def file_level(self, level):
-        """
-        Sets the logging level for the file.
-
-        Args:
-            level: The logging level for the file.
-
-        Returns:
-            None
-        """
-        self.set_level(file_level=translate_to_logging_level(level))
-
-    @property
-    def file_level_name(self):
-        return get_level_name(self.file_level)
-
-    #@property
-    #def file_path(self):
-    #    return self.__file_path
-
-    # @file_path.setter
-    # @validate_type(str, Path, preferred_type=Path)
-    # def file_path(self, new: Union[str, Path]) -> None:
-    #     """
-    #     Sets file-path for the log-file.
-    #
-    #     Args:
-    #         new (str, Path):
-    #             The new file-path for the log-file.
-    #
-    #     Returns:
-    #
-    #     """
-    #     print('I was called')
-    #
-    #     if not self.no_file_logging:
-    #         old = self.__file_path
-    #
-    #         self.__file_path = Path(new)
-    #
-    #         # We need to ensure that the
-    #         try:
-    #             new_path = Path(new)
-    #             self.ensure_log_file_path()
-    #         except Exception as e:
-    #             self.__file_path = old
-    #             raise e
-
-    @property
-    def interactive_session(self):
-        return hasattr(sys, 'ps1') and sys.ps1
-
-    @property
-    def name(self):
-        """
-        Returns the name of the logger instance.
-
-        Returns:
-            str:
-                The name of the logger instance.
-        """
-        return self.logger.name
-
-    @property
-    def no_file_logging(self):
-        return self.__no_file_logging
-
-    @no_file_logging.setter
-    @validate_type(bool)
-    def no_file_logging(self, new):
-        self.__no_file_logging = new
-
-    def __build_name_from_caller(self, caller: inspect.FrameInfo, name: str = None):
-        """
-        Builds a name for a child logger from the caller's frame.
-
-        Parameters:
-            caller (inspect.FrameInfo):
-                The frame of the caller.
-
-        Returns:
-            str:
-                The name of the child-logger.
-
-        """
-        if name is None:
-            name = caller.function
-
-        caller_self = caller.frame.f_locals.get("self", None)
-        separator = ":" if caller_self and hasattr(caller_self, name) else "."
-        return f"{self.logger.name}{separator}{name}"
-
-    def ensure_log_file_path(self):
-        """
-        Ensures that the log file path exists.
-        """
-        if not self.no_file_logging and not self.file_path.exists():
-            self.file_path.parent.mkdir(parents=True, exist_ok=True)
-
-            self.file_path.touch()
-
-    def get_file_handler(self):
-        """
-        Fetches the file-handler for the logger.
-
-        Returns:
-            logging.FileHandler:
-                The file handler for the logger.
-        """
-        for handler in self.logger.handlers:
-            if isinstance(handler, logging.FileHandler):
-
-                return handler
-
-    def has_child(self, name):
-        """
-        Checks if the logger has a child with the specified name.
-
-        Args:
-            name (str):
-                The name of the child logger.
-
-        Returns:
-            bool:
-                True if the logger has a child with the specified name, else False.
-        """
-
-        return name in self.child_names
-
-
-    @validate_type(str, Path, preferred_type=Path)
-    def set_file_path(self, file_path):
-        """
-        Sets the file path for the logger.
-
-        Args:
-            file_path (str):
-                The path to the log file.
-        """
-        try:
-            old = self.file_path
-            self.file_path = file_path
-            self.ensure_log_file_path()
-        except Exception as e:
-            self.file_path = old
-            raise
-
-    def set_up_console(self):
-        """
-        Configures and attaches a console handler to the logger.
-        """
-
-        self.internal("Setting up console handler")
-        console_handler = RichHandler(
-            show_level=True, markup=True, rich_tracebacks=True, tracebacks_show_locals=True
-        )
-        formatter = CustomFormatter(
-            f"[{self.logger.name}] %(message)s"
-        )
-        console_handler.setFormatter(formatter)
-        console_handler.setLevel(self.__console_level)
-        self.logger.addHandler(console_handler)
-
-    def set_up_file(self):
-        """
-        Configures and attaches a file handler to the logger.
-        """
-        self.ensure_log_file_path()
-        file_handler = logging.FileHandler(self.file_path)
-        file_handler.setLevel(self.__file_level)
-        formatter = CustomFormatter(
-            "%(asctime)s - [%(name)s] - %(levelname)s - %(message)s |-| %(file_name)s:%(lineno)d"
-        )
-        file_handler.setFormatter(formatter)
-        self.logger.addHandler(file_handler)
-
-    def set_level(self, console_level=None, file_level=None) -> None:
-        """
-        Updates the logging levels for both console and file handlers.
-
-        Args:
-            console_level:
-                The logging level for the console.
-
-            file_level:
-                The logging level for the file.
-
-        Returns:
-            None
-        """
-
-        self.internal("Setting log levels")
-
-        # If we received a console level, update the console level.
-        if console_level is not None:
-            console_level = translate_to_logging_level(console_level)
-
-            # Set the `console_level` property to the new value.
-            self.__console_level = console_level
-
-            # Iterate through the handlers to get the right one.
-            for handler in self.logger.handlers:
-                if isinstance(handler, RichHandler):
-                    handler.setLevel(console_level)
-
-        # If we received a file level, update the file level.
-        if file_level is not None:
-            file_level = translate_to_logging_level(file_level)
-
-            # Set the `file_level` property to the new value.
-            self.__file_level = file_level
-
-            # Iterate through the handlers to get the right one.
-            for handler in self.logger.handlers:
-                if isinstance(handler, logging.FileHandler):
-                    handler.setLevel(file_level)
-
-        # Set the logger level to the minimum of the console and file levels
-        self.logger.setLevel(min(self.__console_level, self.__file_level))
-
-        # Recursively update the levels of all child loggers.
-        for child in self.children:
-            child.set_level(console_level=console_level, file_level=file_level)
-
-    @method_alias('add_child', 'add_child_logger', 'get_child_logger')
-    def get_child(self, name=None, console_level=None, file_level=None) -> InspyLogger:
-        """
-        Retrieves a child logger with the specified name, console level, and file level.
-
-        Args:
-            name (str, optional):
-                The name of the child logger. Defaults to None.
-
-            console_level (int, optional):
-                The console log level for the child logger. Defaults to None.
-
-            file_level (int, optional):
-                The file log level for the child logger. Defaults to None.
-
-        Returns:
-            InspyLogger:
-                The child logger with the specified name, console level, and file level.
-        """
-        # Get the name of the calling function if no name is provided
-        caller_frame = inspect.stack()[1]
-
-        cl_name = self.__build_name_from_caller(caller_frame, name)
-
-        if found_child := self.find_child_by_name(cl_name, exact_match=True):
-            return found_child
-
-        # Determine the console level and file level for the child logger.
-
-        # If the console level is not provided, use the console level of the parent logger
-        console_level = console_level or self.console_level
-
-        # If the file level is not provided, use the file level of the parent logger
-        file_level = file_level or self.file_level
-
-        child_logger = Logger(name=cl_name, console_level=console_level, file_level=file_level, parent=self)
-
-        self.children.append(child_logger)
-
-        return child_logger
-
-    @method_alias('get_children_names', 'get_child_loggers')
-    def get_child_names(self) -> List:
-        """
-        Fetches the names of all child loggers associated with this logger instance.
-        """
-
-        self.internal("Getting child logger names")
-        return [child.logger.name for child in self.children]
-
-    def get_parent(self) -> InspyLogger:
-        """
-        Fetches the parent logger associated with this logger instance.
-        """
-
-        self.internal("Getting parent logger")
-        return self.parent
-
-    def find_child_by_name(self, name: str, case_sensitive=True, exact_match=False) -> (List, InspyLogger):
-        """
-        Searches for a child logger by its name.
-
-        Args:
-            name (str):
-                The name of the child logger to search for.
-
-            case_sensitive (bool, optional):
-                Whether the search should be case-sensitive. Defaults to True.
-
-            exact_match (bool, optional):
-                Whether the search should only return exact matches. Defaults to False.
-
-        Returns:
-            list or Logger: If exact_match is True, returns the Logger instance if found, else returns an empty list.
-                            If exact_match is False, returns a list of Logger instances whose names contain the
-                            search term.
-        """
-        self.internal(f'Searching for child with name: {name}')
-        results = []
-
-        if not case_sensitive:
-            name = name.lower()
-
-        for logger in self.children:
-            logger_name = logger.name if case_sensitive else logger.name.lower()
-            if exact_match and name == logger_name:
-                return logger
-            elif not exact_match and name in logger_name:
-                results.append(logger)
-
-        return results
-
-    @count_invocations
-    def debug(self, message, stack_level=3):
-        """
-        Logs a debug message.
-
-        Args:
-            message (str): The message to log.
-
-            stack_level (int, optional):
-                The stacklevel to use when logging. Defaults to 3.
-        """
-        self._log(logging.DEBUG, message, args=(), stacklevel=stack_level)
-
-    @count_invocations
-    def info(self, message):
-        """
-        Logs an info message.
-
-        Args:
-            message (str): The message to log.
-        """
-        self._log(logging.INFO, message, args=(), stacklevel=2)
-
-    def internal(self, message, *args, **kwargs):
-        """
-        Logs an internal message.
-
-        Args:
-            message (str): The message to log.
-        """
-        if self.logger.isEnabledFor(INTERNAL):
-            self._log(INTERNAL, message, args=args, stacklevel=2)
-
-    @count_invocations
-    def warning(self, message):
-        """
-        Logs a warning message.
-
-
-        Args:
-            message (str): The message to log.
-        """
-        self._log(logging.WARNING, message, args=(), stacklevel=2)
-
-    @count_invocations
-    def error(self, message):
-        """
-        Logs an error message.
-
-
-        Args:
-            message (str): The message to log.
-        """
-        self._log(logging.ERROR, message, args=(), stacklevel=2)
-
-    def __repr__(self):
-        name = self.name
-        hex_id = hex(id(self))
-        if self.parent is not None:
-            parent_part = f' | Parent Logger: {self.parent.name} |'
-            if self.children:
-                parent_part += f' | Number of children: {len(self.children)} |'
-        else:
-            parent_part = f' | This is a root logger with {len(self.children)} children. '
-
-        if parent_part.endswith('|'):
-            parent_part = str(parent_part[:-2])
-
-        return f'<Logger: {name} w/ levels {self.console_level_name}, {self.file_level_name} at {hex_id}{parent_part}>'
-
-    @classmethod
-    def create_logger_for_caller(cls):
-        """
-        Creates a logger for the module that calls this method.
-
-        Returns:
-            Logger: An instance of the Logger class for the calling module.
-        """
-        if 'ipkernel' in sys.modules or 'IPython' in sys.modules:
-            # We're running in an interactive environment, return a logger named 'interactive'
-            print(cls.instances)
-            if cls.instances.get('Interactive-Python'):
-                level = cls.instances.get('inSPy-Logger')
-            return cls('Interactive-Python')
-        frame = inspect.currentframe().f_back
-        if module_path := cls._determine_module_path(frame):
-            return cls(module_path)
-        raise ValueError("Unable to determine module path for logger creation.")
-
-    def replay_and_setup_handlers(self):
-        """
-        Replays the buffered logs and sets up the handlers for the logger.
-        """
-        if self.buffering_handler:
-            self.buffering_handler.replay_logs(self.logger)
-
-            # Remove the buffer handler
-            self.logger.removeHandler(self.buffering_handler)
-
-        # Set up the handlers
-        if not self.logger.handlers:
-            self.set_up_handlers()
-
-    def set_up_handlers(self) -> None:
-        """
-        Sets up the handlers for the logger.
-        """
-        self.set_up_console()
-        self.set_up_file()
-
-    def to_dict(self):
-        """
-        Converts the logger properties into a dictionary format.
-
-        Returns:
-            dict:
-                A dictionary containing the logger properties.
-
-        """
-        return {
-            'Name': self.name,
-            'Console Level': self.console_level_name,
-            'File Level': self.file_level_name,
-            'Parent': self.parent.name if self.parent else 'None',
-            'Children': {
-                'Count': len(self.children),
-                'Names': self.child_names,
-                'Loggers': [child.to_dict() for child in self.children]
-            },
-            'Handlers': {
-                'Count': len(self.logger.handlers),
-                'Handlers': self.logger.handlers
-            },
-            'Call Counts': self.call_counts,
-            'Buffering Handler': 'Yes' if getattr(self, 'buffering_handler', None) else 'No'
-        }
-
-    def start(self, *args, **kwargs):
-        """
-        Starts the logger.
-        """
-        self.warning('InspyLogger.start() is deprecated.')
-        if not self.logger.handlers:
-            self.set_up_handlers()
-
-        if hasattr(self, 'buffering_handler'):
-            self.replay_and_setup_handlers()
-
-        return self
-
-    @staticmethod
-    def _determine_module_path(frame):
-        """
-        Determines the in-project path of the module from the call frame.
-
-        Args:
-            frame:
-                The frame from which to determine the module path.
-
-        Returns:
-            str:
-                The in-project path of the module.
-        """
-        if module := inspect.getmodule(frame):
-            base_path = os.path.dirname(os.path.abspath(module.__file__))
-            relative_path = os.path.relpath(frame.f_code.co_filename, base_path)
-            return relative_path.replace(os.path.sep, '.').rstrip('.py')
-        return None
-
-    def _log(self, level, msg, args, exc_info=None, extra=None, stack_info=False, stacklevel=1):
-        """
-        Low-level logging implementation, passing stacklevel to findCaller.
-        """
-        #caller_frame = inspect.currentframe().f_back
-        #print(caller_frame.f_code.co_name)
-        if INTERACTIVE_SESSION:
-            stacklevel -= 1
-
-        if self.logger.isEnabledFor(level):
-            self.logger._log(level, msg, args, exc_info, extra, stack_info, stacklevel + 1)
-
-    def __rich__(self):
-        # Create a rich table with logger properties
-        from rich.table import Table
-        from rich import box
-
-        table = Table(title=f'[bold]Logger: {self.name}[/bold]', box=box.ASCII, padding=(0, 1, 0, 1))
-        table.add_column('Property', justify='right', style='cyan', no_wrap=True)
-        table.add_column('Value', justify='left', style='magenta', no_wrap=True)
-
-        table.add_row('Name', self.name)
-        table.add_row('Console Level', self.console_level_name)
-        table.add_row('File Level', self.file_level_name)
-        table.add_row('Parent', self.parent.name if self.parent else 'None')
-        table.add_row('Children', str(len(self.children)))
-        table.add_row('Handlers', str(len(self.logger.handlers)))
-
-        call_counts_str = ', '.join(f'{method}: {count}' for method, count in self.call_counts.items())
-
-        if call_counts_str:
-            table.add_row('Call Counts', call_counts_str)
-        else:
-            table.add_row('Call Counts', 'No method calls recorded')
-
-        if getattr(self, 'buffering_handler', None):
-            table.add_row('Buffering Handler', 'Yes' if self.buffering_handler else 'No')
-
-        return table
+import inspect
+import os
+import logging
+import sys
+
+from rich.logging import RichHandler
+
+from inspy_logger.config import DEFAULT_LOG_FILE_PATH
+from inspy_logger.constants import LEVELS, INTERACTIVE_SESSION, INTERNAL
+from inspy_logger.engine.handlers import BufferingHandler
+from inspy_logger.common import InspyLogger, DEFAULT_LOGGING_LEVEL
+from inspy_logger.helpers import translate_to_logging_level, CustomFormatter, get_level_name, RestrictedSetter
+from inspy_logger.helpers.decorators import add_aliases, method_alias, count_invocations, validate_type
+from typing import List, Union, Optional
+from pathlib import Path
+
+
+@add_aliases
+class Logger(InspyLogger):
+    """
+    A Singleton class responsible for managing the logging mechanisms of the application.
+    """
+
+    LEVELS = LEVELS
+    INTERACTIVE_SESSION = INTERACTIVE_SESSION
+    instances = {}  # A dictionary to hold instances of the Logger class.
+
+    # Set the file path for the log file.
+    file_path = RestrictedSetter('file_path', DEFAULT_LOG_FILE_PATH, allowed_types=(str, Path),preferred_type=Path)
+
+    def __new__(cls, name, *args, **kwargs):
+        """
+        Creates or returns an existing instance of the Logger class for the provided name.
+
+        Parameters:
+            name (str): The name of the logger instance.
+
+        Returns:
+            Logger: An instance of the Logger class.
+        """
+
+        if name not in cls.instances:
+            instance = super(Logger, cls).__new__(cls)
+            cls.instances[name] = instance
+            return instance
+        return cls.instances[name]
+
+    def __init__(
+            self,
+            name,
+            auto_set_up=True,
+            console_level=DEFAULT_LOGGING_LEVEL,
+            file_level=logging.DEBUG,
+            file_name="app.log",
+            file_path=DEFAULT_LOG_FILE_PATH.parent,
+            no_file_logging=False,
+            parent=None,
+            skip_interactive_check: bool=False
+    ):
+        """
+        Initializes a logger instance.
+
+        Parameters:
+            name (str):
+                The name of the logger instance.
+
+            auto_set_up (bool, optional):
+                Whether to automatically set up the handlers for the logger. Defaults to True.
+
+            console_level (str, optional):
+                The logging level for the console. Defaults to DEFAULT_LOGGING_LEVEL.
+
+            file_level (str, optional):
+                The logging level for the file. Defaults to logging.DEBUG.
+
+            file_name (str, optional):
+                The name of the log file. Defaults to "app.log".
+
+            no_file_logging (bool, optional):
+                Whether to disable file logging. Defaults to False.
+
+            parent (Logger, optional):
+                The parent logger instance. Defaults to None.
+        """
+        # Check if the logger has already been initialized.
+        if hasattr(self, 'logger'):
+            return
+
+        self.__call_counts = {}
+
+        self.__console_level = translate_to_logging_level(console_level)
+        self.__file_level = translate_to_logging_level(file_level)
+
+        self.__children = []
+
+        self.__name = name
+        self.__no_file_logging = None
+        self.__file_path = None
+
+
+        self.logger = logging.getLogger(name)
+        self.logger.setLevel(translate_to_logging_level(console_level))
+
+        self.logger.propagate = False
+        self.logger.start = self.start
+
+        if 'inSPy-Logger' in self.logger.name:
+            self.buffering_handler = BufferingHandler()
+            self.logger.addHandler(self.buffering_handler)
+            self.internal('Initializing logger with buffering handler.')
+        else:
+            self.internal('Initializing  logger without buffering handler.')
+
+        self.no_file_logging = no_file_logging
+
+        self.set_file_path = Path(file_path).expanduser().absolute().joinpath(file_name)
+
+        self.parent = parent
+
+        if not getattr(self, 'buffering_handler', None):
+            self.set_up_handlers()
+
+    @property
+    def call_counts(self):
+        """
+        Property to get the call counts of decorated methods.
+
+        Returns:
+            dict:
+                A dictionary containing the call counts of decorated methods.
+
+        """
+        return self.__call_counts
+
+    @property
+    def child_names(self):
+        return self.get_child_names()
+
+    @property
+    def children(self):
+        return self.__children
+
+    @children.deleter
+    def children(self):
+        self.__children = []
+
+    @property
+    def console_level(self):
+        """
+        Returns the logging level for the console.
+
+        Returns:
+            int:
+                The logging level for the console.
+        """
+        return self.__console_level
+
+    @console_level.setter
+    def console_level(self, level):
+        """
+        Sets the logging level for the console.
+
+        Parameters:
+            level:
+                The logging level for the console.
+
+        Returns:
+
+        """
+        self.set_level(console_level=translate_to_logging_level(level))
+
+    @property
+    def console_level_name(self):
+        self.internal('Test message')
+        return get_level_name(self.console_level)
+
+    @property
+    def device(self):
+        """
+        Returns the logger instance.
+
+        Returns:
+            Logger:
+                The logger instance.
+        """
+        logger = self
+        logger.start = self.start.__get__(logger)
+        return logger
+
+    @property
+    def file_level(self):
+        """
+        Returns the logging level for the file.
+
+        Returns:
+            int:
+                The logging level for the file.
+        """
+        return self.__file_level
+
+    @file_level.setter
+    def file_level(self, level):
+        """
+        Sets the logging level for the file.
+
+        Parameters:
+            level: The logging level for the file.
+
+        Returns:
+            None
+        """
+        self.set_level(file_level=translate_to_logging_level(level))
+
+    @property
+    def file_level_name(self):
+        return get_level_name(self.file_level)
+
+    #@property
+    #def file_path(self):
+    #    return self.__file_path
+
+    # @file_path.setter
+    # @validate_type(str, Path, preferred_type=Path)
+    # def file_path(self, new: Union[str, Path]) -> None:
+    #     """
+    #     Sets file-path for the log-file.
+    #
+    #     Parameters:
+    #         new (str, Path):
+    #             The new file-path for the log-file.
+    #
+    #     Returns:
+    #
+    #     """
+    #     print('I was called')
+    #
+    #     if not self.no_file_logging:
+    #         old = self.__file_path
+    #
+    #         self.__file_path = Path(new)
+    #
+    #         # We need to ensure that the
+    #         try:
+    #             new_path = Path(new)
+    #             self.ensure_log_file_path()
+    #         except Exception as e:
+    #             self.__file_path = old
+    #             raise e
+
+    @property
+    def interactive_session(self):
+        return hasattr(sys, 'ps1') and sys.ps1
+
+    @property
+    def name(self):
+        """
+        Returns the name of the logger instance.
+
+        Returns:
+            str:
+                The name of the logger instance.
+        """
+        return self.logger.name
+
+    @property
+    def no_file_logging(self):
+        return self.__no_file_logging
+
+    @no_file_logging.setter
+    @validate_type(bool)
+    def no_file_logging(self, new):
+        self.__no_file_logging = new
+
+    def __build_name_from_caller(self, caller: inspect.FrameInfo, name: str = None):
+        """
+        Builds a name for a child logger from the caller's frame.
+
+        Parameters:
+            caller (inspect.FrameInfo):
+                The frame of the caller.
+
+        Returns:
+            str:
+                The name of the child-logger.
+
+        """
+        if name is None:
+            name = caller.function
+
+        caller_self = caller.frame.f_locals.get("self", None)
+        separator = ":" if caller_self and hasattr(caller_self, name) else "."
+        return f"{self.logger.name}{separator}{name}"
+
+    def ensure_log_file_path(self):
+        """
+        Ensures that the log file path exists.
+        """
+        if not self.no_file_logging and not self.file_path.exists():
+            self.file_path.parent.mkdir(parents=True, exist_ok=True)
+
+            self.file_path.touch()
+
+    def get_file_handler(self):
+        """
+        Fetches the file-handler for the logger.
+
+        Returns:
+            logging.FileHandler:
+                The file handler for the logger.
+        """
+        for handler in self.logger.handlers:
+            if isinstance(handler, logging.FileHandler):
+
+                return handler
+
+    def has_child(self, name):
+        """
+        Checks if the logger has a child with the specified name.
+
+        Parameters:
+            name (str):
+                The name of the child logger.
+
+        Returns:
+            bool:
+                True if the logger has a child with the specified name, else False.
+        """
+
+        return name in self.child_names
+
+
+    @validate_type(str, Path, preferred_type=Path)
+    def set_file_path(self, file_path):
+        """
+        Sets the file path for the logger.
+
+        Parameters:
+            file_path (str):
+                The path to the log file.
+        """
+        try:
+            old = self.file_path
+            self.file_path = file_path
+            self.ensure_log_file_path()
+        except Exception as e:
+            self.file_path = old
+            raise
+
+    def set_up_console(self):
+        """
+        Configures and attaches a console handler to the logger.
+        """
+
+        self.internal("Setting up console handler")
+        console_handler = RichHandler(
+            show_level=True, markup=True, rich_tracebacks=True, tracebacks_show_locals=True
+        )
+        formatter = CustomFormatter(
+            f"[{self.logger.name}] %(message)s"
+        )
+        console_handler.setFormatter(formatter)
+        console_handler.setLevel(self.__console_level)
+        self.logger.addHandler(console_handler)
+
+    def set_up_file(self):
+        """
+        Configures and attaches a file handler to the logger.
+        """
+        
+        self.ensure_log_file_path()
+        file_handler = logging.FileHandler(self.file_path)
+        file_handler.setLevel(self.__file_level)
+        formatter = CustomFormatter(
+            "%(asctime)s - [%(name)s] - %(levelname)s - %(message)s |-| %(file_name)s:%(lineno)d"
+        )
+        file_handler.setFormatter(formatter)
+        self.logger.addHandler(file_handler)
+
+    def set_level(self, console_level=None, file_level=None, override=False) -> None:
+        """
+        Updates the logging levels for both console and file handlers.
+
+        Parameters:
+            console_level:
+                The logging level for the console.
+
+            file_level:
+                The logging level for the file.
+                
+            override (bool):
+                Whether to override the `no_file_logging` option. Defaults to `False`.
+
+        Returns:
+            None
+        """
+
+        self.internal("Setting log levels")
+
+        # If we received a console level, update the console level.
+        if console_level is not None:
+            console_level = translate_to_logging_level(console_level)
+
+            # Set the `console_level` property to the new value.
+            self.__console_level = console_level
+
+            # Iterate through the handlers to get the right one.
+            for handler in self.logger.handlers:
+                if isinstance(handler, RichHandler):
+                    handler.setLevel(console_level)
+
+        # If we received a file level, update the file level.
+        if file_level is not None:
+            file_level = translate_to_logging_level(file_level)
+
+            # Set the `file_level` property to the new value.
+            self.__file_level = file_level
+
+            # Iterate through the handlers to get the right one.
+            for handler in self.logger.handlers:
+                if isinstance(handler, logging.FileHandler):
+                    handler.setLevel(file_level)
+
+        # Set the logger level to the minimum of the console and file levels
+        self.logger.setLevel(min(self.__console_level, self.__file_level))
+
+        # Recursively update the levels of all child loggers.
+        for child in self.children:
+            child.set_level(console_level=console_level, file_level=file_level)
+
+    @method_alias('add_child', 'add_child_logger', 'get_child_logger')
+    def get_child(self, name=None, console_level=None, file_level=None) -> InspyLogger:
+        """
+        Retrieves a child logger with the specified name, console level, and file level.
+
+        Parameters:
+            name (str, optional):
+                The name of the child logger. Defaults to None.
+
+            console_level (int, optional):
+                The console log level for the child logger. Defaults to None.
+
+            file_level (int, optional):
+                The file log level for the child logger. Defaults to None.
+
+        Returns:
+            InspyLogger:
+                The child logger with the specified name, console level, and file level.
+        """
+        # Get the name of the calling function if no name is provided
+        caller_frame = inspect.stack()[1]
+
+        cl_name = self.__build_name_from_caller(caller_frame, name)
+
+        if found_child := self.find_child_by_name(cl_name, exact_match=True):
+            return found_child
+
+        # Determine the console level and file level for the child logger.
+
+        # If the console level is not provided, use the console level of the parent logger
+        console_level = console_level or self.console_level
+
+        # If the file level is not provided, use the file level of the parent logger
+        file_level = file_level or self.file_level
+
+        child_logger = Logger(name=cl_name, console_level=console_level, file_level=file_level, parent=self)
+
+        self.children.append(child_logger)
+
+        return child_logger
+
+    @method_alias('get_children_names', 'get_child_loggers')
+    def get_child_names(self) -> List:
+        """
+        Fetches the names of all child loggers associated with this logger instance.
+        """
+
+        self.internal("Getting child logger names")
+        return [child.logger.name for child in self.children]
+
+    def get_parent(self) -> InspyLogger:
+        """
+        Fetches the parent logger associated with this logger instance.
+        """
+
+        self.internal("Getting parent logger")
+        return self.parent
+
+    def find_child_by_name(self, name: str, case_sensitive=True, exact_match=False) -> (List, InspyLogger):
+        """
+        Searches for a child logger by its name.
+
+        Parameters:
+            name (str):
+                The name of the child logger to search for.
+
+            case_sensitive (bool, optional):
+                Whether the search should be case-sensitive. Defaults to True.
+
+            exact_match (bool, optional):
+                Whether the search should only return exact matches. Defaults to False.
+
+        Returns:
+            list or Logger: If exact_match is True, returns the Logger instance if found, else returns an empty list.
+                            If exact_match is False, returns a list of Logger instances whose names contain the
+                            search term.
+        """
+        self.internal(f'Searching for child with name: {name}')
+        results = []
+
+        if not case_sensitive:
+            name = name.lower()
+
+        for logger in self.children:
+            logger_name = logger.name if case_sensitive else logger.name.lower()
+            if exact_match and name == logger_name:
+                return logger
+            elif not exact_match and name in logger_name:
+                results.append(logger)
+
+        return results
+
+    @count_invocations
+    def debug(self, message, stack_level=3):
+        """
+        Logs a debug message.
+
+        Parameters:
+            message (str): The message to log.
+
+            stack_level (int, optional):
+                The stacklevel to use when logging. Defaults to 3.
+        """
+        self._log(logging.DEBUG, message, args=(), stacklevel=stack_level)
+
+    @count_invocations
+    def info(self, message):
+        """
+        Logs an info message.
+
+        Parameters:
+            message (str): The message to log.
+        """
+        self._log(logging.INFO, message, args=(), stacklevel=2)
+
+    def internal(self, message, *args, **kwargs):
+        """
+        Logs an internal message.
+
+        Parameters:
+            message (str): The message to log.
+        """
+        if self.logger.isEnabledFor(INTERNAL):
+            self._log(INTERNAL, message, args=args, stacklevel=2)
+
+    @count_invocations
+    def warning(self, message):
+        """
+        Logs a warning message.
+
+
+        Parameters:
+            message (str): The message to log.
+        """
+        self._log(logging.WARNING, message, args=(), stacklevel=2)
+
+    @count_invocations
+    def error(self, message):
+        """
+        Logs an error message.
+
+
+        Parameters:
+            message (str): The message to log.
+        """
+        self._log(logging.ERROR, message, args=(), stacklevel=2)
+
+    def __repr__(self):
+        name = self.name
+        hex_id = hex(id(self))
+        if self.parent is not None:
+            parent_part = f' | Parent Logger: {self.parent.name} |'
+            if self.children:
+                parent_part += f' | Number of children: {len(self.children)} |'
+        else:
+            parent_part = f' | This is a root logger with {len(self.children)} children. '
+
+        if parent_part.endswith('|'):
+            parent_part = str(parent_part[:-2])
+
+        return f'<Logger: {name} w/ levels {self.console_level_name}, {self.file_level_name} at {hex_id}{parent_part}>'
+
+    @classmethod
+    def create_logger_for_caller(cls):
+        """
+        Creates a logger for the module that calls this method.
+
+        Returns:
+            Logger: An instance of the Logger class for the calling module.
+        """
+        if 'ipkernel' in sys.modules or 'IPython' in sys.modules:
+            # We're running in an interactive environment, return a logger named 'interactive'
+
+            if cls.instances.get('Interactive-Python'):
+                level = cls.instances.get('inSPy-Logger')
+            return cls('Interactive-Python')
+        frame = inspect.currentframe().f_back
+        if module_path := cls._determine_module_path(frame):
+            return cls(module_path)
+        raise ValueError("Unable to determine module path for logger creation.")
+
+    def replay_and_setup_handlers(self):
+        """
+        Replays the buffered logs and sets up the handlers for the logger.
+        """
+        if self.buffering_handler:
+            self.buffering_handler.replay_logs(self.logger)
+
+            # Remove the buffer handler
+            self.logger.removeHandler(self.buffering_handler)
+
+        # Set up the handlers
+        if not self.logger.handlers:
+            self.set_up_handlers()
+
+    def set_up_handlers(self) -> None:
+        """
+        Sets up the handlers for the logger.
+        """
+        self.set_up_console()
+        self.set_up_file()
+
+    def to_dict(self):
+        """
+        Converts the logger properties into a dictionary format.
+
+        Returns:
+            dict:
+                A dictionary containing the logger properties.
+
+        """
+        return {
+            'Name': self.name,
+            'Console Level': self.console_level_name,
+            'File Level': self.file_level_name,
+            'Parent': self.parent.name if self.parent else 'None',
+            'Children': {
+                'Count': len(self.children),
+                'Names': self.child_names,
+                'Loggers': [child.to_dict() for child in self.children]
+            },
+            'Handlers': {
+                'Count': len(self.logger.handlers),
+                'Handlers': self.logger.handlers
+            },
+            'Call Counts': self.call_counts,
+            'Buffering Handler': 'Yes' if getattr(self, 'buffering_handler', None) else 'No'
+        }
+
+    def start(self, *args, **kwargs):
+        """
+        Starts the logger.
+        """
+        self.warning('InspyLogger.start() is deprecated.')
+        if not self.logger.handlers:
+            self.set_up_handlers()
+
+        if hasattr(self, 'buffering_handler'):
+            self.replay_and_setup_handlers()
+
+        return self
+
+    @staticmethod
+    def _determine_module_path(frame):
+        """
+        Determines the in-project path of the module from the call frame.
+
+        Parameters:
+            frame:
+                The frame from which to determine the module path.
+
+        Returns:
+            str:
+                The in-project path of the module.
+        """
+        if module := inspect.getmodule(frame):
+            base_path = os.path.dirname(os.path.abspath(module.__file__))
+            relative_path = os.path.relpath(frame.f_code.co_filename, base_path)
+            return relative_path.replace(os.path.sep, '.').rstrip('.py')
+        return None
+
+    def _log(self, level, msg, args, exc_info=None, extra=None, stack_info=False, stacklevel=1):
+        """
+        Low-level logging implementation, passing stacklevel to findCaller.
+        """
+        #caller_frame = inspect.currentframe().f_back
+        #print(caller_frame.f_code.co_name)
+        if INTERACTIVE_SESSION:
+            stacklevel -= 1
+
+        if self.logger.isEnabledFor(level):
+            self.logger._log(level, msg, args, exc_info, extra, stack_info, stacklevel + 1)
+
+    def __rich__(self):
+        # Create a rich table with logger properties
+        from rich.table import Table
+        from rich import box
+
+        table = Table(title=f'[bold]Logger: {self.name}[/bold]', box=box.ASCII, padding=(0, 1, 0, 1))
+        table.add_column('Property', justify='right', style='cyan', no_wrap=True)
+        table.add_column('Value', justify='left', style='magenta', no_wrap=True)
+
+        table.add_row('Name', self.name)
+        table.add_row('Console Level', self.console_level_name)
+        table.add_row('File Level', self.file_level_name)
+        table.add_row('Parent', self.parent.name if self.parent else 'None')
+        table.add_row('Children', str(len(self.children)))
+        table.add_row('Handlers', str(len(self.logger.handlers)))
+
+        call_counts_str = ', '.join(f'{method}: {count}' for method, count in self.call_counts.items())
+
+        if call_counts_str:
+            table.add_row('Call Counts', call_counts_str)
+        else:
+            table.add_row('Call Counts', 'No method calls recorded')
+
+        if getattr(self, 'buffering_handler', None):
+            table.add_row('Buffering Handler', 'Yes' if self.buffering_handler else 'No')
+
+        return table
```

### Comparing `inspy_logger-3.1.0.dev3/inspy_logger/engine/errors.py` & `inspy_logger-3.1.0.dev4/inspy_logger/engine/errors.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev3/inspy_logger/engine/handlers.py` & `inspy_logger-3.1.0.dev4/inspy_logger/engine/handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         if not self.replaying:
             self.buffer.append(record)
 
     def replay_logs(self, logger):
         """
         Replays the buffered logs and restores the original logging level of the logger.
 
-        Args:
+        Parameters:
             logger:
                 The logger instance to replay the logs to.
 
         Returns:
             None
 
         Examples:
```

### Comparing `inspy_logger-3.1.0.dev3/inspy_logger/helpers/base_classes.py` & `inspy_logger-3.1.0.dev4/inspy_logger/helpers/base_classes.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,150 +1,149 @@
-import inspect
-from inspy_logger import LOG_DEVICE, Logger
-
-
-class LoggableDescriptor:
-    """
-    Descriptor for accessing a logger specific to a class method.
-    """
-
-    def __get__(self, instance, owner):
-        if instance is None:
-            # Accessing through the class, not an instance
-            return owner.class_logger
-
-        # Determine the calling method's name
-        stack = inspect.stack()
-        # Start from 1 to skip the current __get__ frame
-        for frame_record in stack[1:]:
-            if 'self' in frame_record.frame.f_locals and frame_record.frame.f_locals['self'] is instance:
-                method_name = frame_record.function
-
-                break
-        else:
-            raise Exception("Could not determine the calling method's name.")
-
-        # Get a child logger named after the class and method
-        return instance.log_device.get_child(method_name)
-
-
-def _get_parent_logging_device():
-    """
-    Determines the parent logging device by inspecting the caller's log_device or parent_log_device attribute.
-
-    Returns:
-        Logger: The parent logging device.
-    """
-    LOG_DEVICE.debug("Determining parent logging device")
-    caller_frame = inspect.currentframe().f_back
-    caller_locals = caller_frame.f_locals
-
-    if "logger" in caller_locals:
-        return caller_locals["logger"]
-    elif "parent_log_device" in caller_locals:
-        return caller_locals["parent_log_device"]
-    else:
-        raise ValueError("Unable to determine the parent logging device.")
-
-
-class Loggable:
-    """
-    A metaclass to enhance classes with logging capabilities. Classes that inherit from
-    'Loggable' can instantly access a logger without manually setting it up. This logger
-    is derived from a parent logger, ensuring consistent logging behavior and hierarchy.
-
-    Attributes:
-        - log_device: The logger device associated with the instance of the class.
-    """
-    method_logger = LoggableDescriptor()
-    class_logger = None
-
-    def __init__(self, parent_log_device=None, **kwargs):
-        """
-        Initializes an instance of the class.
-
-        Args:
-            parent_log_device (optional): The parent log device. Defaults to None.
-            **kwargs: Additional keyword arguments.
-
-        Returns:
-            None
-        """
-        self.parent_log_device = parent_log_device
-        self.__log_name = self.__class__.__name__
-
-        if self.parent_log_device is not None:
-            self.__log_device = self.parent_log_device.get_child(self.__log_name)
-        else:
-            self.__log_device = _get_parent_logging_device().get_child()
-
-        # Set up class-level logger if it's not already set
-        if self.__class__.class_logger is None:
-            self.__class__.class_logger = self.__log_device
-
-        self.method_logger = self.__class__.method_logger.logger
-
-    @property
-    def log_device(self):
-        return self.__log_device
-
-    @log_device.setter
-    def log_device(self, new):
-        if not isinstance(new, Logger):
-            raise TypeError('log_device must be of type "Logger"')
-
-        self.__log_device = new
-
-    def create_child_logger(self, name=None, override=False):
-        """
-        Creates and returns a child logger of this object's logger.
-
-        Parameters:
-            name (str, optional): The name of the child logger.
-                If not provided, the name of the calling function is used.
-            override (bool, optional): A flag to override the membership check. Defaults to False.
-
-        Returns:
-            Logger: An instance of the Logger class that represents the child logger.
-        """
-        if name is None:
-            name = inspect.stack()[1][
-                3
-            ]
-        if self.log_device.has_child(name):
-            return self.log_device.find_child_by_name(name)
-        if not override:
-            self.__is_member__()
-
-        return self.log_device.get_child(name)
-
-    def __is_member__(self):
-        """
-        Checks whether the caller of this method is a member of the same class.
-
-        Raises:
-            PermissionError: If the caller of this method is not a member of the same class.
-        """
-        print(self.log_device.children)
-        log_name = f'{self.log_device.name}.__is_member__'
-
-
-        log_device = self.log_device.get_child("__is_member__")
-        log = log_device
-
-        current_frame = inspect.currentframe()
-        log.debug(f"Current frame: {current_frame}")
-
-        caller_frame = current_frame.f_back
-        log.debug(f"Caller frame: {caller_frame}")
-
-        caller_self = caller_frame.f_locals.get("self", None)
-        log.debug(f"Caller self: {caller_self}")
-
-        log.debug("Checking if caller is a member of this class...")
-        if not isinstance(caller_self, self.__class__):
-            raise PermissionError(
-                "Access denied.\n"
-                f"Method can only be accessed by members of the same class. {caller_self.__class__.__name__} is not such a member"
-            )
-
-        log.debug(f"Access granted to {caller_self.__class__.__name__}")
+import inspect
+from inspy_logger import LOG_DEVICE, Logger
+
+
+class LoggableDescriptor:
+    """
+    Descriptor for accessing a logger specific to a class method.
+    """
+
+    def __get__(self, instance, owner):
+        if instance is None:
+            # Accessing through the class, not an instance
+            return owner.class_logger
+
+        # Determine the calling method's name
+        stack = inspect.stack()
+        # Start from 1 to skip the current __get__ frame
+        for frame_record in stack[1:]:
+            if 'self' in frame_record.frame.f_locals and frame_record.frame.f_locals['self'] is instance:
+                method_name = frame_record.function
+
+                break
+        else:
+            raise Exception("Could not determine the calling method's name.")
+
+        # Get a child logger named after the class and method
+        return instance.log_device.get_child(method_name)
+
+
+def _get_parent_logging_device():
+    """
+    Determines the parent logging device by inspecting the caller's log_device or parent_log_device attribute.
+
+    Returns:
+        Logger: The parent logging device.
+    """
+    LOG_DEVICE.debug("Determining parent logging device")
+    caller_frame = inspect.currentframe().f_back
+    caller_locals = caller_frame.f_locals
+
+    if "logger" in caller_locals:
+        return caller_locals["logger"]
+    elif "parent_log_device" in caller_locals:
+        return caller_locals["parent_log_device"]
+    else:
+        raise ValueError("Unable to determine the parent logging device.")
+
+
+class Loggable:
+    """
+    A metaclass to enhance classes with logging capabilities. Classes that inherit from
+    'Loggable' can instantly access a logger without manually setting it up. This logger
+    is derived from a parent logger, ensuring consistent logging behavior and hierarchy.
+
+    Attributes:
+        - log_device: The logger device associated with the instance of the class.
+    """
+    method_logger = LoggableDescriptor()
+    class_logger = None
+
+    def __init__(self, parent_log_device=None, **kwargs):
+        """
+        Initializes an instance of the class.
+
+        Parameters:
+            parent_log_device (optional): The parent log device. Defaults to None.
+            **kwargs: Additional keyword arguments.
+
+        Returns:
+            None
+        """
+        self.parent_log_device = parent_log_device
+        self.__log_name = self.__class__.__name__
+
+        if self.parent_log_device is not None:
+            self.__log_device = self.parent_log_device.get_child(self.__log_name)
+        else:
+            self.__log_device = _get_parent_logging_device().get_child()
+
+        # Set up class-level logger if it's not already set
+        if self.__class__.class_logger is None:
+            self.__class__.class_logger = self.__log_device
+
+        self.method_logger = self.__class__.method_logger.logger
+
+    @property
+    def log_device(self):
+        return self.__log_device
+
+    @log_device.setter
+    def log_device(self, new):
+        if not isinstance(new, Logger):
+            raise TypeError('log_device must be of type "Logger"')
+
+        self.__log_device = new
+
+    def create_child_logger(self, name=None, override=False):
+        """
+        Creates and returns a child logger of this object's logger.
+
+        Parameters:
+            name (str, optional): The name of the child logger.
+                If not provided, the name of the calling function is used.
+            override (bool, optional): A flag to override the membership check. Defaults to False.
+
+        Returns:
+            Logger: An instance of the Logger class that represents the child logger.
+        """
+        if name is None:
+            name = inspect.stack()[1][
+                3
+            ]
+        if self.log_device.has_child(name):
+            return self.log_device.find_child_by_name(name)
+        if not override:
+            self.__is_member__()
+
+        return self.log_device.get_child(name)
+
+    def __is_member__(self):
+        """
+        Checks whether the caller of this method is a member of the same class.
+
+        Raises:
+            PermissionError: If the caller of this method is not a member of the same class.
+        """
+        log_name = f'{self.log_device.name}.__is_member__'
+
+
+        log_device = self.log_device.get_child("__is_member__")
+        log = log_device
+
+        current_frame = inspect.currentframe()
+        log.debug(f"Current frame: {current_frame}")
+
+        caller_frame = current_frame.f_back
+        log.debug(f"Caller frame: {caller_frame}")
+
+        caller_self = caller_frame.f_locals.get("self", None)
+        log.debug(f"Caller self: {caller_self}")
+
+        log.debug("Checking if caller is a member of this class...")
+        if not isinstance(caller_self, self.__class__):
+            raise PermissionError(
+                "Access denied.\n"
+                f"Method can only be accessed by members of the same class. {caller_self.__class__.__name__} is not such a member"
+            )
+
+        log.debug(f"Access granted to {caller_self.__class__.__name__}")
```

### Comparing `inspy_logger-3.1.0.dev3/inspy_logger/helpers/command_line/__init__.py` & `inspy_logger-3.1.0.dev4/inspy_logger/helpers/command_line/__init__.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev3/inspy_logger/helpers/debug/environment.py` & `inspy_logger-3.1.0.dev4/inspy_logger/helpers/debug/environment.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev3/inspy_logger/helpers/debug/system/processor/__init__.py` & `inspy_logger-3.1.0.dev4/inspy_logger/helpers/debug/system/processor/__init__.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev3/inspy_logger/helpers/debug/system/winx/__init__.py` & `inspy_logger-3.1.0.dev4/inspy_logger/helpers/debug/system/winx/__init__.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev3/inspy_logger/helpers/decorators.py` & `inspy_logger-3.1.0.dev4/inspy_logger/helpers/decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 
 
 def method_alias(*alias_names: (str, list[str])):
     """
     A decorator that allows you to add aliases to a class's method.
 
-    Args:
+    Parameters:
         *alias_names (str, list[str]):
             The name(s) of the alias(es) to add.
 
     Returns:
         method:
             The decorated method.
     """
@@ -67,15 +67,15 @@
     return method_decorator
 
 
 def method_logger(func):
     """
     A decorator to log a method's execution.
 
-    Args:
+    Parameters:
         func (method):
             The method to log.
 
     Returns:
         method:
             The decorated method.
     """
@@ -97,15 +97,15 @@
     return wrapper
 
 
 def add_aliases(cls):
     """
     A decorator to add aliases to a class's methods.
 
-    Args:
+    Parameters:
         cls (class):
             The class to add aliases to.
 
     Returns:
         class:
             The decorated class.
     """
@@ -116,15 +116,15 @@
     return cls
 
 
 def count_invocations(method):
     """
     Decorator that counts the number of invocations of the method it decorates.
 
-    Args:
+    Parameters:
         method (Callable):
             The method to count invocations for.
 
     Returns:
         Callable:
             The decorated method.
     """
@@ -142,15 +142,15 @@
 
 def validate_type(*allowed_types, preferred_type=None, allowed_values=None, case_sensitive=True):
     """
     A decorator for validating the type and optionally the value of a value passed to a class
     property setter, with an option to convert to a preferred type if specified and to enforce
     value restrictions.
 
-    Args:
+    Parameters:
         preferred_type (type, optional): The preferred type to which values should be converted
                                           if possible. If None, no conversion is attempted.
         *allowed_types: Variable length list of allowed types for the property value.
         allowed_values (iterable, optional): An iterable of values that are allowed. If None,
                                              all values of the correct type are allowed.
         case_sensitive (bool, optional): Specifies whether string comparisons should be case
                                          sensitive. Defaults to True. Ignored for non-string types.
@@ -211,15 +211,15 @@
 
 
 def validate_func_args(*validators):
     """
     A decorator for validating the type and optionally the value of arguments passed to a function.
     Each argument can have its own set of allowed types, a preferred type, and allowed values.
 
-    Args:
+    Parameters:
         *validators (dict): Each dictionary in validators specifies the validation rules for one argument.
                             The keys in the dictionary can be:
                             - 'allowed_types': A tuple of allowed types for the argument.
                             - 'preferred_type': The preferred type to which the argument should be converted if possible.
                             - 'allowed_values': A list of values that the argument is allowed to have.
                             - 'case_sensitive': Specifies whether string comparisons should be case sensitive.
```

### Comparing `inspy_logger-3.1.0.dev3/inspy_logger/helpers/descriptors.py` & `inspy_logger-3.1.0.dev4/inspy_logger/helpers/descriptors.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev3/inspy_logger/helpers/units.py` & `inspy_logger-3.1.0.dev4/inspy_logger/helpers/units.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     }
 
     @classmethod
     def convert(cls, value: float, from_unit: str, to_unit: str) -> float:
         """
         Converts the given value from one unit to another.
 
-        Args:
+        Parameters:
             value (float): The value to convert.
             from_unit (str): The unit to convert from. Must be one of the supported units.
             to_unit (str): The unit to convert to. Must be one of the supported units.
 
         Returns:
             float: The converted value in the target unit.
```

### Comparing `inspy_logger-3.1.0.dev3/inspy_logger/manifest.py` & `inspy_logger-3.1.0.dev4/inspy_logger/manifest.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-from time import time
-from logging import getLogger
-from box import Box
-
-
-class Manifest(object):
-    def __init__(self, root_name, root_device, calling_file, line_num):
-        self.name = root_name
-
-        self.contents = None
-        self.add(root_name, root_device, calling_file, line_num)
-
-    def check(self, name):
-
-        return self.contents[name]['device'] if name in self.contents.keys() else None
-
-
-    def add(self, name, logger_device, calling_file, line_num):
-        """
-
-        Add the provided logger to the manifest.
-
-        Parameters:
-          name (str): The logger name.
-          logger_device ()
-
-        """
-
-        entry = {
-                name: {
-                        'created-ts':  time(),
-                        'device':      logger_device,
-                        'caller_file': calling_file,
-                }
-        }
-
-        if self.contents is None:
-            self.contents = Box(entry)
-        else:
-            self.contents.update(entry)
+from time import time
+from logging import getLogger
+from box import Box
+
+
+class Manifest(object):
+    def __init__(self, root_name, root_device, calling_file, line_num):
+        self.name = root_name
+
+        self.contents = None
+        self.add(root_name, root_device, calling_file, line_num)
+
+    def check(self, name):
+
+        return self.contents[name]['device'] if name in self.contents.keys() else None
+
+
+    def add(self, name, logger_device, calling_file, line_num):
+        """
+
+        Add the provided logger to the manifest.
+
+        Parameters:
+          name (str): The logger name.
+          logger_device ()
+
+        """
+
+        entry = {
+                name: {
+                        'created-ts':  time(),
+                        'device':      logger_device,
+                        'caller_file': calling_file,
+                }
+        }
+
+        if self.contents is None:
+            self.contents = Box(entry)
+        else:
+            self.contents.update(entry)
```

### Comparing `inspy_logger-3.1.0.dev3/inspy_logger/Scripts/main.py` & `inspy_logger-3.1.0.dev4/inspy_logger/Scripts/main.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev3/inspy_logger/system/__init__.py` & `inspy_logger-3.1.0.dev4/inspy_logger/system/__init__.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev3/inspy_logger/system/win32.py` & `inspy_logger-3.1.0.dev4/inspy_logger/system/win32.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev3/inspy_logger/tool/config/arguments/__init__.py` & `inspy_logger-3.1.0.dev4/inspy_logger/tool/config/arguments/__init__.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev3/inspy_logger/types.py` & `inspy_logger-3.1.0.dev4/inspy_logger/types.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev3/inspy_logger/version/__init__.py` & `inspy_logger-3.1.0.dev4/inspy_logger/version/__init__.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.1.0.dev3/LICENSE.md` & `inspy_logger-3.1.0.dev4/LICENSE.md`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-### Do What the Fuck You Want To - Public License (v3.0 3, Sept. 2020)
-----
-----
-
-                    Copyright (C) 2020 Taylor-Jayde Blackstone <t.blackstone@inspyre.tech>
-
-----
-
- Everyone is permitted to copy and distribute verbatim or modified
- copies of this license document, and changing it is allowed as long
- as the name is changed. That's my name, you can't have it.
-            
-                                  DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
-                        TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION
-
-- You just **DO WHAT THE FUCK YOU WANT TO**.
-- You **don't** blame me for **shit**. _I don't care_ how much smoke your hard-drive spewed out.
-- If someone else did what the fuck they wanted to and you're _**triggered**_ I'm **not** responsible.
-
-                              Contact <dev.null@inspyre.tech> with any complaints.
+### Do What the Fuck You Want To - Public License (v3.0 3, Sept. 2020)
+----
+----
+
+                    Copyright (C) 2020 Taylor-Jayde Blackstone <t.blackstone@inspyre.tech>
+
+----
+
+ Everyone is permitted to copy and distribute verbatim or modified
+ copies of this license document, and changing it is allowed as long
+ as the name is changed. That's my name, you can't have it.
+            
+                                  DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
+                        TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION
+
+- You just **DO WHAT THE FUCK YOU WANT TO**.
+- You **don't** blame me for **shit**. _I don't care_ how much smoke your hard-drive spewed out.
+- If someone else did what the fuck they wanted to and you're _**triggered**_ I'm **not** responsible.
+
+                              Contact <dev.null@inspyre.tech> with any complaints.
```

### Comparing `inspy_logger-3.1.0.dev3/README.md` & `inspy_logger-3.1.0.dev4/README.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-# inSPy-Logger
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/Inspyre-Softworks/inSPy-Logger/CI?label=CI&logo=github&logoColor=9cf&style=for-the-badge) 
-![Codacy grade](https://img.shields.io/codacy/grade/7171eec682c549a88dee0da9cc9b92b3?logo=codacy&logoColor=9cf&style=for-the-badge) 
-![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/Inspyre-Softworks/inSPy-Logger?color=9cf&include_prereleases&label=Pre-Release&logo=pypi&logoColor=9cf&style=for-the-badge) 
-![PyPI](https://img.shields.io/pypi/v/inspy-logger?color=9cf&label=Latest&logo=pypi&logoColor=9cf&style=for-the-badge) 
-![GitHub issues](https://img.shields.io/github/issues/Inspyre-Softworks/inSPy-Logger?color=9cf&logo=github&logoColor=9cf&style=for-the-badge) 
-![PyPI - Format](https://img.shields.io/pypi/format/inSPy-Logger?logo=PyPi&style=for-the-badge)
-
-## Installation
-
-### Prerequisites:
-
-**Platform/Env**:
-  * **Python**: ^3.6.3
-  * **PIP**: (_If you want to install via PIP, that is_)
-  
-**inSPy-Logger Runtime Dependencies**:
-  I am providing this list of dependencies for transparency and for instances where one would not be able to install inSPy-Logger via PyPi's package manager. It is **highly** recommended you use `python3 -m pip install inspy_logger==<ver>` to install inSPy-Logger 2.0+
-  
-  * [colorlog](https://pypi.org/project/colorlog) (^4.2.1)
-  * [setuptools-autover](https://pypi.org/project/setuptools-autover) = (^1.0.2)
-  * [luddite](https://pypi.org/project/luddite) = (^1.0.1)
-  * [packaging](https://pypi.org/project/packaging) = (^20.4)
-
-### Installation via Pip on Python 3.6.3+ (recommended method):
-
-- `$> python3 -m pip install inspy_logger==<version>`
-
-#### Test out InspyLogger:
-
-```python3
-
-import inspy_logger
-
-# Set up a log device object. The first parameter is the root loggers name, and the second is the debug level
-log_device = inspy_logger.InspyLogger('LogName', 'debug')
-
-# Start a running log from that device
-log = log_device.start()
-
-# Output our own logger lines:
-log.debug('This is a debug log entry')
-log.info('This is an info log entry')
-log.warning('This is a warning log entry!')
-log.error('This is an error log entry!')
-log.exception('This is an exception log entry!')
-
-```
-
-If you run the code above you'll get output similar to this:
-
-![output1](https://github.com/Inspyre-Softworks/inSPy-Logger/blob/v2.0-alpha.6/examples/v2.0/output_screenies/v2.0.0a.6_screenie1.png)
-
-v2.0+ repository for inSPy-Logger
+# inSPy-Logger
+![GitHub Workflow Status](https://img.shields.io/github/workflow/status/Inspyre-Softworks/inSPy-Logger/CI?label=CI&logo=github&logoColor=9cf&style=for-the-badge) 
+![Codacy grade](https://img.shields.io/codacy/grade/7171eec682c549a88dee0da9cc9b92b3?logo=codacy&logoColor=9cf&style=for-the-badge) 
+![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/Inspyre-Softworks/inSPy-Logger?color=9cf&include_prereleases&label=Pre-Release&logo=pypi&logoColor=9cf&style=for-the-badge) 
+![PyPI](https://img.shields.io/pypi/v/inspy-logger?color=9cf&label=Latest&logo=pypi&logoColor=9cf&style=for-the-badge) 
+![GitHub issues](https://img.shields.io/github/issues/Inspyre-Softworks/inSPy-Logger?color=9cf&logo=github&logoColor=9cf&style=for-the-badge) 
+![PyPI - Format](https://img.shields.io/pypi/format/inSPy-Logger?logo=PyPi&style=for-the-badge)
+
+## Installation
+
+### Prerequisites:
+
+**Platform/Env**:
+  * **Python**: ^3.6.3
+  * **PIP**: (_If you want to install via PIP, that is_)
+  
+**inSPy-Logger Runtime Dependencies**:
+  I am providing this list of dependencies for transparency and for instances where one would not be able to install inSPy-Logger via PyPi's package manager. It is **highly** recommended you use `python3 -m pip install inspy_logger==<ver>` to install inSPy-Logger 2.0+
+  
+  * [colorlog](https://pypi.org/project/colorlog) (^4.2.1)
+  * [setuptools-autover](https://pypi.org/project/setuptools-autover) = (^1.0.2)
+  * [luddite](https://pypi.org/project/luddite) = (^1.0.1)
+  * [packaging](https://pypi.org/project/packaging) = (^20.4)
+
+### Installation via Pip on Python 3.6.3+ (recommended method):
+
+- `$> python3 -m pip install inspy_logger==<version>`
+
+#### Test out InspyLogger:
+
+```python3
+
+import inspy_logger
+
+# Set up a log device object. The first parameter is the root loggers name, and the second is the debug level
+log_device = inspy_logger.InspyLogger('LogName', 'debug')
+
+# Start a running log from that device
+log = log_device.start()
+
+# Output our own logger lines:
+log.debug('This is a debug log entry')
+log.info('This is an info log entry')
+log.warning('This is a warning log entry!')
+log.error('This is an error log entry!')
+log.exception('This is an exception log entry!')
+
+```
+
+If you run the code above you'll get output similar to this:
+
+![output1](https://github.com/Inspyre-Softworks/inSPy-Logger/blob/v2.0-alpha.6/examples/v2.0/output_screenies/v2.0.0a.6_screenie1.png)
+
+v2.0+ repository for inSPy-Logger
```

### Comparing `inspy_logger-3.1.0.dev3/PKG-INFO` & `inspy_logger-3.1.0.dev4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspy-logger
-Version: 3.1.0.dev3
+Version: 3.1.0.dev4
 Summary: Colorable, scalable logger for CLI
 Home-page: https://github.com/Inspyre-Softworks/inSPy-Logger
 License: MIT
 Keywords: cli,color,logging,log,terminal,console,colorama,colorlog,rich
 Author: Taylor-Jayde Blackstone
 Author-email: tayjaybabee@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -28,14 +28,15 @@
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: colorlog (>=6.8.2,<7.0.0)
 Requires-Dist: humanize (>=4.4.0,<5.0.0)
 Requires-Dist: luddite (>=1.0.4,<2.0.0)
 Requires-Dist: packaging (>=24.0,<25.0)
 Requires-Dist: platformdirs (>=4.2.0,<5.0.0)
 Requires-Dist: pypattyrn (>=1.2,<2.0)
+Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: python-box (>=7.1.1,<8.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: setuptools-autover (>=1.0.2,<2.0.0)
 Project-URL: Documentation, https://inspy-logger.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/Inspyre-Softworks/inSPy-Logger
 Description-Content-Type: text/markdown
```

