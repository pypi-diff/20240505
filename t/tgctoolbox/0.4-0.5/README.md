# Comparing `tmp/tgctoolbox-0.4.tar.gz` & `tmp/tgctoolbox-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgctoolbox-0.4.tar", max compression
+gzip compressed data, was "tgctoolbox-0.5.tar", max compression
```

## Comparing `tgctoolbox-0.4.tar` & `tgctoolbox-0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      543 2024-05-05 12:03:28.350661 tgctoolbox-0.4/pyproject.toml
--rw-r--r--   0        0        0     1883 2024-05-05 11:34:10.191732 tgctoolbox-0.4/tgctoolbox/__init__.py
--rw-r--r--   0        0        0     2965 2024-04-14 10:00:56.065124 tgctoolbox-0.4/tgctoolbox/downloaders.py
--rw-r--r--   0        0        0     6398 2024-04-14 10:04:12.366063 tgctoolbox-0.4/tgctoolbox/ffmpeg.py
--rw-r--r--   0        0        0     3699 2024-04-04 14:07:33.674769 tgctoolbox-0.4/tgctoolbox/logger.py
--rw-r--r--   0        0        0      125 2024-04-04 14:07:33.502903 tgctoolbox-0.4/tgctoolbox/meta.py
--rw-r--r--   0        0        0     3532 2024-04-14 10:04:35.139755 tgctoolbox-0.4/tgctoolbox/operations.py
--rw-r--r--   0        0        0     2536 2024-04-14 10:05:13.288749 tgctoolbox-0.4/tgctoolbox/recorder.py
--rw-r--r--   0        0        0     7701 2024-05-05 12:02:01.085948 tgctoolbox-0.4/tgctoolbox/settings.py
--rw-r--r--   0        0        0     4338 2024-05-04 17:49:00.284883 tgctoolbox-0.4/tgctoolbox/sound.py
--rw-r--r--   0        0        0     2541 2024-04-14 10:05:55.801603 tgctoolbox-0.4/tgctoolbox/timing.py
--rw-r--r--   0        0        0     1787 2024-04-14 10:06:14.232604 tgctoolbox-0.4/tgctoolbox/vosk.py
--rw-r--r--   0        0        0     3415 2024-04-14 10:06:32.142449 tgctoolbox-0.4/tgctoolbox/wait_run.py
--rw-r--r--   0        0        0     2740 2024-04-13 22:34:12.249076 tgctoolbox-0.4/tgctoolbox/wrapper.py
--rw-r--r--   0        0        0      635 1970-01-01 00:00:00.000000 tgctoolbox-0.4/PKG-INFO
+-rw-r--r--   0        0        0      543 2024-05-05 13:10:16.372337 tgctoolbox-0.5/pyproject.toml
+-rw-r--r--   0        0        0     1883 2024-05-05 11:34:10.191732 tgctoolbox-0.5/tgctoolbox/__init__.py
+-rw-r--r--   0        0        0     2965 2024-04-14 10:00:56.065124 tgctoolbox-0.5/tgctoolbox/downloaders.py
+-rw-r--r--   0        0        0     6398 2024-04-14 10:04:12.366063 tgctoolbox-0.5/tgctoolbox/ffmpeg.py
+-rw-r--r--   0        0        0     3699 2024-04-04 14:07:33.674769 tgctoolbox-0.5/tgctoolbox/logger.py
+-rw-r--r--   0        0        0      125 2024-04-04 14:07:33.502903 tgctoolbox-0.5/tgctoolbox/meta.py
+-rw-r--r--   0        0        0     3532 2024-04-14 10:04:35.139755 tgctoolbox-0.5/tgctoolbox/operations.py
+-rw-r--r--   0        0        0     2536 2024-04-14 10:05:13.288749 tgctoolbox-0.5/tgctoolbox/recorder.py
+-rw-r--r--   0        0        0     7917 2024-05-05 13:08:07.389797 tgctoolbox-0.5/tgctoolbox/settings.py
+-rw-r--r--   0        0        0     4338 2024-05-04 17:49:00.284883 tgctoolbox-0.5/tgctoolbox/sound.py
+-rw-r--r--   0        0        0     2541 2024-04-14 10:05:55.801603 tgctoolbox-0.5/tgctoolbox/timing.py
+-rw-r--r--   0        0        0     1787 2024-04-14 10:06:14.232604 tgctoolbox-0.5/tgctoolbox/vosk.py
+-rw-r--r--   0        0        0     3415 2024-04-14 10:06:32.142449 tgctoolbox-0.5/tgctoolbox/wait_run.py
+-rw-r--r--   0        0        0     2740 2024-04-13 22:34:12.249076 tgctoolbox-0.5/tgctoolbox/wrapper.py
+-rw-r--r--   0        0        0      635 1970-01-01 00:00:00.000000 tgctoolbox-0.5/PKG-INFO
```

### Comparing `tgctoolbox-0.4/pyproject.toml` & `tgctoolbox-0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tgctoolbox"
-version = "0.4"
+version = "0.5"
 description = "Comprehensive toolbox with all of the utils and tools used in various TGC projects."
 authors = ["Jakub Muszyński <jakub.m.muszynski@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pytube = "*"
 moviepy = "*"
```

### Comparing `tgctoolbox-0.4/tgctoolbox/__init__.py` & `tgctoolbox-0.5/tgctoolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `tgctoolbox-0.4/tgctoolbox/downloaders.py` & `tgctoolbox-0.5/tgctoolbox/downloaders.py`

 * *Files identical despite different names*

### Comparing `tgctoolbox-0.4/tgctoolbox/ffmpeg.py` & `tgctoolbox-0.5/tgctoolbox/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `tgctoolbox-0.4/tgctoolbox/logger.py` & `tgctoolbox-0.5/tgctoolbox/logger.py`

 * *Files identical despite different names*

### Comparing `tgctoolbox-0.4/tgctoolbox/operations.py` & `tgctoolbox-0.5/tgctoolbox/operations.py`

 * *Files identical despite different names*

### Comparing `tgctoolbox-0.4/tgctoolbox/recorder.py` & `tgctoolbox-0.5/tgctoolbox/recorder.py`

 * *Files identical despite different names*

### Comparing `tgctoolbox-0.4/tgctoolbox/settings.py` & `tgctoolbox-0.5/tgctoolbox/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 class Settings(metaclass=SettingsMeta):
     """Class to manage application settings."""
 
     def __init__(
         self,
         load_predefined: bool = True,
         reload: bool = False,
-        load_env: bool = False,
         base_dir: Optional[str] = None,
         config_files: Optional[List[str]] = None,
         env_prefix: Optional[str] = None,
     ):
         """
         Initialize Settings object. Load settings from YAML files and environment variables.
 
@@ -44,15 +43,14 @@
         1. Predefined YAML files (base.yaml, local.yaml, production.yaml) - this setting is enabled by default and uses the APP_ENVIRONMENT environment variable to choose the YAML files based on convention
         2. Custom YAML files - pass the list of paths to the YAML files to load and set load_predefined to False
         3. Environment variables - set load_env to True to load settings from environment variables, which should be prefixed with 'VAR_' as per convention
 
         Args:
             load_predefined (bool): Load settings from predefined YAML files. Default is True.
             reload (bool): Whether to reload settings. Default is False.
-            load_env (bool): Load settings from environment variables. Default is False.
             base_dir (str): Path to the directory containing the YAML files. Default is 'configuration'.
             config_files (list): List of paths to the YAML files to load. By default, it loads 'base.yaml', 'local.yaml', and 'production.yaml'.
             env_prefix (str): Prefix for environment variables. Default is 'VAR_'.
         """
         BASE_DIR = base_dir or "configuration"
         BASE_FILES = [
             os.path.join(BASE_DIR, "base.yaml"),
@@ -67,21 +65,24 @@
             self.host = None
             self._settings = {}
             config_files = config_files or BASE_FILES
             if load_predefined:
                 self._load_from_yaml_predefined(BASE_DIR)
             else:
                 self._load_from_yaml(config_files)
-            if load_env:
-                self._load_from_env(env_prefix)
+            self._load_from_env(env_prefix)
             self._initialized = True
             self._set_settings(REQUIRED_SETTINGS)
 
     def _set_settings(self, req_settings: List[str]):
-        """Helper function to set required settings as named parameters of the class based on a setting dictionary."""
+        """Helper function to set required settings as named parameters of the class based on a setting dictionary.
+
+        Raises:
+            ValueError: If a required setting is not found.
+        """
         for setting in req_settings:
             if not self.get(setting):
                 raise ValueError(f"Setting '{setting}' is required")
             else:
                 setattr(self, setting, self.get(setting))
 
     def _load_from_yaml_predefined(self, dir_path: str):
@@ -89,19 +90,26 @@
 
         Note: This method chooses the YAML files based on the APP_ENVIRONMENT environment variable.
         APP_ENVIRONMENT can be 'local' or 'production'. If not set, 'local' is used by default.
         This method utilizes more general _load_from_yaml method to load the settings and provides top-level logic to choose the YAML files.
 
         Args:
             dir_path (str): Path to the directory containing the YAML files.
+
+        Raises:
+            ValueError: If APP_ENVIRONMENT is not 'local' or 'production'.
         """
         base_path = os.path.join(dir_path, "base.yaml")
         local_path = os.path.join(dir_path, "local.yaml")
         prod_path = os.path.join(dir_path, "production.yaml")
         app_env = os.environ.get("APP_ENVIRONMENT", "local")
+        if "APP_ENVIRONMENT" not in os.environ:
+            logger.warning(
+                "APP_ENVIRONMENT environment variable not set. Using 'local' by default."
+            )
         if app_env not in ["local", "production"]:
             raise ValueError(
                 "Invalid APP_ENVIRONMENT value. Use 'local' or 'production'."
             )
         FILES = [base_path, local_path if app_env == "local" else prod_path]
         self._load_from_yaml(FILES)
```

### Comparing `tgctoolbox-0.4/tgctoolbox/sound.py` & `tgctoolbox-0.5/tgctoolbox/sound.py`

 * *Files identical despite different names*

### Comparing `tgctoolbox-0.4/tgctoolbox/timing.py` & `tgctoolbox-0.5/tgctoolbox/timing.py`

 * *Files identical despite different names*

### Comparing `tgctoolbox-0.4/tgctoolbox/vosk.py` & `tgctoolbox-0.5/tgctoolbox/vosk.py`

 * *Files identical despite different names*

### Comparing `tgctoolbox-0.4/tgctoolbox/wait_run.py` & `tgctoolbox-0.5/tgctoolbox/wait_run.py`

 * *Files identical despite different names*

### Comparing `tgctoolbox-0.4/tgctoolbox/wrapper.py` & `tgctoolbox-0.5/tgctoolbox/wrapper.py`

 * *Files identical despite different names*

### Comparing `tgctoolbox-0.4/PKG-INFO` & `tgctoolbox-0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgctoolbox
-Version: 0.4
+Version: 0.5
 Summary: Comprehensive toolbox with all of the utils and tools used in various TGC projects.
 Author: Jakub Muszyński
 Author-email: jakub.m.muszynski@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

