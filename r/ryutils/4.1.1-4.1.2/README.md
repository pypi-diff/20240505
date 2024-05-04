# Comparing `tmp/ryutils-4.1.1.tar.gz` & `tmp/ryutils-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryutils-4.1.1.tar", last modified: Sat Apr 20 22:58:57 2024, max compression
+gzip compressed data, was "ryutils-4.1.2.tar", last modified: Sat May  4 23:13:57 2024, max compression
```

## Comparing `ryutils-4.1.1.tar` & `ryutils-4.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:58:57.894649 ryutils-4.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-20 22:58:53.000000 ryutils-4.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-20 22:58:53.000000 ryutils-4.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-20 22:58:57.894649 ryutils-4.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-20 22:58:53.000000 ryutils-4.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-20 22:58:53.000000 ryutils-4.1.1/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-20 22:58:53.000000 ryutils-4.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-20 22:58:53.000000 ryutils-4.1.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:58:57.890649 ryutils-4.1.1/ryutils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 22:58:53.000000 ryutils-4.1.1/ryutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-20 22:58:53.000000 ryutils-4.1.1/ryutils/async_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-20 22:58:53.000000 ryutils-4.1.1/ryutils/csv_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-20 22:58:53.000000 ryutils-4.1.1/ryutils/dict_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-20 22:58:53.000000 ryutils-4.1.1/ryutils/email_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-20 22:58:53.000000 ryutils-4.1.1/ryutils/file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-20 22:58:53.000000 ryutils-4.1.1/ryutils/fmt_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    12462 2024-04-20 22:58:53.000000 ryutils-4.1.1/ryutils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-20 22:58:53.000000 ryutils-4.1.1/ryutils/proxies.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 22:58:53.000000 ryutils-4.1.1/ryutils/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-20 22:58:53.000000 ryutils-4.1.1/ryutils/short_url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:58:57.890649 ryutils-4.1.1/ryutils/sms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 22:58:53.000000 ryutils-4.1.1/ryutils/sms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-20 22:58:53.000000 ryutils-4.1.1/ryutils/sms/telegram_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-20 22:58:53.000000 ryutils-4.1.1/ryutils/sms/twilio_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-20 22:58:53.000000 ryutils-4.1.1/ryutils/wait.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-20 22:58:53.000000 ryutils-4.1.1/ryutils/web2_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:58:57.890649 ryutils-4.1.1/ryutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-20 22:58:57.000000 ryutils-4.1.1/ryutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-20 22:58:57.000000 ryutils-4.1.1/ryutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 22:58:57.000000 ryutils-4.1.1/ryutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-20 22:58:57.000000 ryutils-4.1.1/ryutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-20 22:58:57.000000 ryutils-4.1.1/ryutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 22:58:57.894649 ryutils-4.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-20 22:58:53.000000 ryutils-4.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 23:13:57.309081 ryutils-4.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-04 23:13:53.000000 ryutils-4.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-04 23:13:53.000000 ryutils-4.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-04 23:13:57.309081 ryutils-4.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-04 23:13:53.000000 ryutils-4.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-04 23:13:53.000000 ryutils-4.1.2/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-04 23:13:53.000000 ryutils-4.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-04 23:13:53.000000 ryutils-4.1.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 23:13:57.309081 ryutils-4.1.2/ryutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 23:13:53.000000 ryutils-4.1.2/ryutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-04 23:13:53.000000 ryutils-4.1.2/ryutils/async_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-04 23:13:53.000000 ryutils-4.1.2/ryutils/csv_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-04 23:13:53.000000 ryutils-4.1.2/ryutils/dict_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-04 23:13:53.000000 ryutils-4.1.2/ryutils/email_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-04 23:13:53.000000 ryutils-4.1.2/ryutils/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-04 23:13:53.000000 ryutils-4.1.2/ryutils/fmt_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12476 2024-05-04 23:13:53.000000 ryutils-4.1.2/ryutils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-04 23:13:53.000000 ryutils-4.1.2/ryutils/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 23:13:53.000000 ryutils-4.1.2/ryutils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-04 23:13:53.000000 ryutils-4.1.2/ryutils/short_url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 23:13:57.309081 ryutils-4.1.2/ryutils/sms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 23:13:53.000000 ryutils-4.1.2/ryutils/sms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-04 23:13:53.000000 ryutils-4.1.2/ryutils/sms/telegram_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-05-04 23:13:53.000000 ryutils-4.1.2/ryutils/sms/twilio_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-04 23:13:53.000000 ryutils-4.1.2/ryutils/wait.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-04 23:13:53.000000 ryutils-4.1.2/ryutils/web2_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 23:13:57.309081 ryutils-4.1.2/ryutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-04 23:13:57.000000 ryutils-4.1.2/ryutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-04 23:13:57.000000 ryutils-4.1.2/ryutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 23:13:57.000000 ryutils-4.1.2/ryutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-04 23:13:57.000000 ryutils-4.1.2/ryutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-04 23:13:57.000000 ryutils-4.1.2/ryutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 23:13:57.309081 ryutils-4.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-04 23:13:53.000000 ryutils-4.1.2/setup.py
```

### Comparing `ryutils-4.1.1/LICENSE` & `ryutils-4.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ryutils-4.1.1/PKG-INFO` & `ryutils-4.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryutils
-Version: 4.1.1
+Version: 4.1.2
 Summary: A collection of utilities for Python
 Author: Ross Yeager
 Author-email: ryeager12@email.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ryutils-4.1.1/pyproject.toml` & `ryutils-4.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ryutils-4.1.1/requirements.txt` & `ryutils-4.1.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `ryutils-4.1.1/ryutils/async_utils.py` & `ryutils-4.1.2/ryutils/async_utils.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.1.1/ryutils/csv_logger.py` & `ryutils-4.1.2/ryutils/csv_logger.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.1.1/ryutils/dict_util.py` & `ryutils-4.1.2/ryutils/dict_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.1.1/ryutils/email_util.py` & `ryutils-4.1.2/ryutils/email_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.1.1/ryutils/fmt_util.py` & `ryutils-4.1.2/ryutils/fmt_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.1.1/ryutils/log.py` & `ryutils-4.1.2/ryutils/log.py`

 * *Files 6% similar despite different names*

```diff
@@ -141,20 +141,24 @@
         MultiHandler(
             new_log_dir,
             ["ThreadPool", "MainThread"],
         )
     )
 
 
+def get_downsample_count() -> int:
+    return _DOWNSAMPLE_COUNT
+
+
 def make_formatter_printer(
     color: str,
     log_level: int = logging.INFO,
     prefix: str = "",
     return_formatter: bool = False,
-    downsample: int = 1,
+    downsample: bool = False,
 ) -> T.Callable:
     logger = logging.getLogger(__name__)
 
     def formatter(message, *args, **kwargs):
         message = str(message)
 
         if args or kwargs:
@@ -178,20 +182,22 @@
             return formatted_text.encode("utf-8").decode(sys.stdout.encoding, errors="ignore")
 
         return formatted_text
 
     def printer(message, *args, **kwargs):
         is_logger_in_use = logging.getLogger().hasHandlers()
 
+        downsample_val = get_downsample_count() if downsample else 1
+
         # obtain the backtrace of the caller to use as the key
         frame = sys._getframe(1)  # pylint: disable=protected-access
         key = frame.f_code.co_filename + frame.f_code.co_name + str(frame.f_lineno)
-        if key not in _DOWNSAMPLER and downsample > 1:
-            # set the count to downsample - 1 so that the first message is always printed
-            _DOWNSAMPLER[key] = {"downsample": downsample, "count": downsample - 1}
+        if key not in _DOWNSAMPLER and downsample_val > 1:
+            # set the count to downsample_val - 1 so that the first message is always printed
+            _DOWNSAMPLER[key] = {"downsample": downsample_val, "count": downsample_val - 1}
 
         if _ALWAYS_PRINT:
             print(formatter(message, *args, **kwargs))
         elif key in _DOWNSAMPLER:
             _DOWNSAMPLER[key]["count"] += 1
             if _DOWNSAMPLER[key]["count"] % _DOWNSAMPLER[key]["downsample"] == 0:
                 print(formatter(message, *args, **kwargs))
@@ -288,57 +294,57 @@
 print_bold = make_formatter_printer(Colors.BOLD.value, log_level=logging.CRITICAL)
 print_normal = make_formatter_printer(Colors.ENDC.value, log_level=logging.DEBUG)
 print_normal_arrow = make_formatter_printer(
     Colors.ENDC.value, prefix=Prefixes.ARROW.value, log_level=logging.DEBUG
 )
 
 print_ok_blue_slow = make_formatter_printer(
-    Colors.OKBLUE.value, log_level=logging.INFO, downsample=_DOWNSAMPLE_COUNT
+    Colors.OKBLUE.value, log_level=logging.INFO, downsample=True
 )
 print_ok_blue_arrow_slow = make_formatter_printer(
     Colors.OKBLUE.value,
     prefix=Prefixes.ARROW.value,
     log_level=logging.INFO,
-    downsample=_DOWNSAMPLE_COUNT,
+    downsample=True,
 )
 print_ok_slow = make_formatter_printer(
-    Colors.OKGREEN.value, log_level=logging.CRITICAL, downsample=_DOWNSAMPLE_COUNT
+    Colors.OKGREEN.value, log_level=logging.CRITICAL, downsample=True
 )
 print_ok_arrow_slow = make_formatter_printer(
     Colors.OKGREEN.value,
     prefix=Prefixes.ARROW.value,
     log_level=logging.CRITICAL,
-    downsample=_DOWNSAMPLE_COUNT,
+    downsample=True,
 )
 print_bright_slow = make_formatter_printer(
-    Colors.OKCYAN.value, log_level=logging.WARNING, downsample=_DOWNSAMPLE_COUNT
+    Colors.OKCYAN.value, log_level=logging.WARNING, downsample=True
 )
 print_warn_slow = make_formatter_printer(
-    Colors.WARNING.value, log_level=logging.WARNING, downsample=_DOWNSAMPLE_COUNT
+    Colors.WARNING.value, log_level=logging.WARNING, downsample=True
 )
 print_fail_slow = make_formatter_printer(
-    Colors.FAIL.value, log_level=logging.CRITICAL, downsample=_DOWNSAMPLE_COUNT
+    Colors.FAIL.value, log_level=logging.CRITICAL, downsample=True
 )
 print_fail_arrow_slow = make_formatter_printer(
     Colors.FAIL.value,
     prefix=Prefixes.ARROW.value,
     log_level=logging.CRITICAL,
-    downsample=_DOWNSAMPLE_COUNT,
+    downsample=True,
 )
 print_bold_slow = make_formatter_printer(
-    Colors.BOLD.value, log_level=logging.CRITICAL, downsample=_DOWNSAMPLE_COUNT
+    Colors.BOLD.value, log_level=logging.CRITICAL, downsample=True
 )
 print_normal_slow = make_formatter_printer(
-    Colors.ENDC.value, log_level=logging.DEBUG, downsample=_DOWNSAMPLE_COUNT
+    Colors.ENDC.value, log_level=logging.DEBUG, downsample=True
 )
 print_normal_arrow_slow = make_formatter_printer(
     Colors.ENDC.value,
     prefix=Prefixes.ARROW.value,
     log_level=logging.DEBUG,
-    downsample=_DOWNSAMPLE_COUNT,
+    downsample=True,
 )
 
 
 format_ok_blue = make_formatter_printer(Colors.OKBLUE.value, return_formatter=True)
 format_ok = make_formatter_printer(Colors.OKGREEN.value, return_formatter=True)
 format_bright = make_formatter_printer(Colors.OKCYAN.value, return_formatter=True)
 format_warn = make_formatter_printer(Colors.WARNING.value, return_formatter=True)
```

### Comparing `ryutils-4.1.1/ryutils/proxies.py` & `ryutils-4.1.2/ryutils/proxies.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.1.1/ryutils/sms/telegram_util.py` & `ryutils-4.1.2/ryutils/sms/telegram_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.1.1/ryutils/sms/twilio_util.py` & `ryutils-4.1.2/ryutils/sms/twilio_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.1.1/ryutils/web2_client.py` & `ryutils-4.1.2/ryutils/web2_client.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.1.1/ryutils.egg-info/PKG-INFO` & `ryutils-4.1.2/ryutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryutils
-Version: 4.1.1
+Version: 4.1.2
 Summary: A collection of utilities for Python
 Author: Ross Yeager
 Author-email: ryeager12@email.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ryutils-4.1.1/ryutils.egg-info/SOURCES.txt` & `ryutils-4.1.2/ryutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ryutils-4.1.1/setup.py` & `ryutils-4.1.2/setup.py`

 * *Files identical despite different names*

