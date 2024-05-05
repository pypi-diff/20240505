# Comparing `tmp/dtPyAppFramework-1.1.tar.gz` & `tmp/dtpyappframework-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtPyAppFramework-1.1.tar", last modified: Tue Mar  5 11:23:54 2024, max compression
+gzip compressed data, was "dtpyappframework-1.2.tar", last modified: Sun May  5 07:17:37 2024, max compression
```

## Comparing `dtPyAppFramework-1.1.tar` & `dtpyappframework-1.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:23:54.994757 dtPyAppFramework-1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-05 11:23:49.000000 dtPyAppFramework-1.1/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-05 11:23:49.000000 dtPyAppFramework-1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-03-05 11:23:54.994757 dtPyAppFramework-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-03-05 11:23:49.000000 dtPyAppFramework-1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-03-05 11:23:49.000000 dtPyAppFramework-1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-05 11:23:49.000000 dtPyAppFramework-1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 11:23:54.994757 dtPyAppFramework-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-05 11:23:49.000000 dtPyAppFramework-1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:23:54.990757 dtPyAppFramework-1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:23:54.990757 dtPyAppFramework-1.1/src/dtPyAppFramework/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-05 11:23:49.000000 dtPyAppFramework-1.1/src/dtPyAppFramework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-03-05 11:23:49.000000 dtPyAppFramework-1.1/src/dtPyAppFramework/application.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:23:54.994757 dtPyAppFramework-1.1/src/dtPyAppFramework/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-03-05 11:23:49.000000 dtPyAppFramework-1.1/src/dtPyAppFramework/decorators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:23:54.994757 dtPyAppFramework-1.1/src/dtPyAppFramework/logging/
--rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-03-05 11:23:49.000000 dtPyAppFramework-1.1/src/dtPyAppFramework/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-03-05 11:23:49.000000 dtPyAppFramework-1.1/src/dtPyAppFramework/logging/default_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:23:54.994757 dtPyAppFramework-1.1/src/dtPyAppFramework/misc/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-05 11:23:49.000000 dtPyAppFramework-1.1/src/dtPyAppFramework/misc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:23:54.994757 dtPyAppFramework-1.1/src/dtPyAppFramework/paths/
--rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-03-05 11:23:49.000000 dtPyAppFramework-1.1/src/dtPyAppFramework/paths/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:23:54.994757 dtPyAppFramework-1.1/src/dtPyAppFramework/process/
--rw-r--r--   0 runner    (1001) docker     (127)     7666 2024-03-05 11:23:49.000000 dtPyAppFramework-1.1/src/dtPyAppFramework/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-03-05 11:23:49.000000 dtPyAppFramework-1.1/src/dtPyAppFramework/process/multiprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:23:54.994757 dtPyAppFramework-1.1/src/dtPyAppFramework/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-03-05 11:23:49.000000 dtPyAppFramework-1.1/src/dtPyAppFramework/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:23:54.994757 dtPyAppFramework-1.1/src/dtPyAppFramework/settings/
--rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-03-05 11:23:49.000000 dtPyAppFramework-1.1/src/dtPyAppFramework/settings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:23:54.994757 dtPyAppFramework-1.1/src/dtPyAppFramework/settings/secrets/
--rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-03-05 11:23:49.000000 dtPyAppFramework-1.1/src/dtPyAppFramework/settings/secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-03-05 11:23:49.000000 dtPyAppFramework-1.1/src/dtPyAppFramework/settings/secrets/aws_secret_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-03-05 11:23:49.000000 dtPyAppFramework-1.1/src/dtPyAppFramework/settings/secrets/azure_secret_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     6096 2024-03-05 11:23:49.000000 dtPyAppFramework-1.1/src/dtPyAppFramework/settings/secrets/local_secret_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-03-05 11:23:49.000000 dtPyAppFramework-1.1/src/dtPyAppFramework/settings/secrets/secret_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-03-05 11:23:49.000000 dtPyAppFramework-1.1/src/dtPyAppFramework/settings/settings_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-03-05 11:23:49.000000 dtPyAppFramework-1.1/src/dtPyAppFramework/version.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:23:54.994757 dtPyAppFramework-1.1/src/dtPyAppFramework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-03-05 11:23:54.000000 dtPyAppFramework-1.1/src/dtPyAppFramework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-03-05 11:23:54.000000 dtPyAppFramework-1.1/src/dtPyAppFramework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 11:23:54.000000 dtPyAppFramework-1.1/src/dtPyAppFramework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-05 11:23:54.000000 dtPyAppFramework-1.1/src/dtPyAppFramework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-05 11:23:54.000000 dtPyAppFramework-1.1/src/dtPyAppFramework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:17:37.754488 dtpyappframework-1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-05 07:17:33.000000 dtpyappframework-1.2/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-05 07:17:33.000000 dtpyappframework-1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6405 2024-05-05 07:17:37.754488 dtpyappframework-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-05 07:17:33.000000 dtpyappframework-1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-05 07:17:33.000000 dtpyappframework-1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-05 07:17:33.000000 dtpyappframework-1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 07:17:37.754488 dtpyappframework-1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-05 07:17:33.000000 dtpyappframework-1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:17:37.750488 dtpyappframework-1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:17:37.750488 dtpyappframework-1.2/src/dtPyAppFramework/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-05 07:17:33.000000 dtpyappframework-1.2/src/dtPyAppFramework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-05-05 07:17:33.000000 dtpyappframework-1.2/src/dtPyAppFramework/application.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:17:37.750488 dtpyappframework-1.2/src/dtPyAppFramework/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-05 07:17:33.000000 dtpyappframework-1.2/src/dtPyAppFramework/decorators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:17:37.754488 dtpyappframework-1.2/src/dtPyAppFramework/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-05-05 07:17:33.000000 dtpyappframework-1.2/src/dtPyAppFramework/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-05 07:17:33.000000 dtpyappframework-1.2/src/dtPyAppFramework/logging/default_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:17:37.754488 dtpyappframework-1.2/src/dtPyAppFramework/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-05 07:17:33.000000 dtpyappframework-1.2/src/dtPyAppFramework/misc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:17:37.754488 dtpyappframework-1.2/src/dtPyAppFramework/paths/
+-rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-05 07:17:33.000000 dtpyappframework-1.2/src/dtPyAppFramework/paths/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:17:37.754488 dtpyappframework-1.2/src/dtPyAppFramework/process/
+-rw-r--r--   0 runner    (1001) docker     (127)     7876 2024-05-05 07:17:33.000000 dtpyappframework-1.2/src/dtPyAppFramework/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-05-05 07:17:33.000000 dtpyappframework-1.2/src/dtPyAppFramework/process/multiprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:17:37.754488 dtpyappframework-1.2/src/dtPyAppFramework/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-05 07:17:33.000000 dtpyappframework-1.2/src/dtPyAppFramework/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:17:37.754488 dtpyappframework-1.2/src/dtPyAppFramework/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-05-05 07:17:33.000000 dtpyappframework-1.2/src/dtPyAppFramework/settings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:17:37.754488 dtpyappframework-1.2/src/dtPyAppFramework/settings/secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)     6549 2024-05-05 07:17:33.000000 dtpyappframework-1.2/src/dtPyAppFramework/settings/secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-05 07:17:33.000000 dtpyappframework-1.2/src/dtPyAppFramework/settings/secrets/aws_secret_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-05-05 07:17:33.000000 dtpyappframework-1.2/src/dtPyAppFramework/settings/secrets/azure_secret_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6096 2024-05-05 07:17:33.000000 dtpyappframework-1.2/src/dtPyAppFramework/settings/secrets/local_secret_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-05 07:17:33.000000 dtpyappframework-1.2/src/dtPyAppFramework/settings/secrets/secret_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-05 07:17:33.000000 dtpyappframework-1.2/src/dtPyAppFramework/settings/settings_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-05 07:17:33.000000 dtpyappframework-1.2/src/dtPyAppFramework/version.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:17:37.754488 dtpyappframework-1.2/src/dtPyAppFramework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6405 2024-05-05 07:17:37.000000 dtpyappframework-1.2/src/dtPyAppFramework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-05 07:17:37.000000 dtpyappframework-1.2/src/dtPyAppFramework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 07:17:37.000000 dtpyappframework-1.2/src/dtPyAppFramework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-05 07:17:37.000000 dtpyappframework-1.2/src/dtPyAppFramework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-05 07:17:37.000000 dtpyappframework-1.2/src/dtPyAppFramework.egg-info/top_level.txt
```

### Comparing `dtPyAppFramework-1.1/LICENCE.txt` & `dtpyappframework-1.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `dtPyAppFramework-1.1/PKG-INFO` & `dtpyappframework-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtPyAppFramework
-Version: 1.1
+Version: 1.2
 Summary: A Python library for common features in application development.
 Author-email: Digital-Thought <dev@digital-thought.org>
 Maintainer-email: Digital-Thought <dev@digital-thought.org>
 License: MIT License
         
         Copyright (c) 2024 Digital-Thought
         
@@ -85,15 +85,15 @@
 ## Getting Started
 ### AbstractApp Class ###
 The **`AbstractApp`** class serves as a base class for creating Python applications. It handles common initialisation tasks and provides a structure for defining command-line arguments and the main application logic.
 
 
 To create a simple Python application using dtPyAppFramework:
 ```python
-from dtPyAppFramework.app import AbstractApp
+from dtPyAppFramework.application import AbstractApp
 from dtPyAppFramework import settings
 
 import logging
 
 class MyApplication(AbstractApp):
 
     def define_args(self, arg_parser):
```

### Comparing `dtPyAppFramework-1.1/README.md` & `dtpyappframework-1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ## Getting Started
 ### AbstractApp Class ###
 The **`AbstractApp`** class serves as a base class for creating Python applications. It handles common initialisation tasks and provides a structure for defining command-line arguments and the main application logic.
 
 
 To create a simple Python application using dtPyAppFramework:
 ```python
-from dtPyAppFramework.app import AbstractApp
+from dtPyAppFramework.application import AbstractApp
 from dtPyAppFramework import settings
 
 import logging
 
 class MyApplication(AbstractApp):
 
     def define_args(self, arg_parser):
```

### Comparing `dtPyAppFramework-1.1/pyproject.toml` & `dtpyappframework-1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dtPyAppFramework-1.1/src/dtPyAppFramework/application.py` & `dtpyappframework-1.2/src/dtPyAppFramework/application.py`

 * *Files identical despite different names*

### Comparing `dtPyAppFramework-1.1/src/dtPyAppFramework/decorators/__init__.py` & `dtpyappframework-1.2/src/dtPyAppFramework/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `dtPyAppFramework-1.1/src/dtPyAppFramework/logging/__init__.py` & `dtpyappframework-1.2/src/dtPyAppFramework/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `dtPyAppFramework-1.1/src/dtPyAppFramework/logging/default_logging.py` & `dtpyappframework-1.2/src/dtPyAppFramework/logging/default_logging.py`

 * *Files identical despite different names*

### Comparing `dtPyAppFramework-1.1/src/dtPyAppFramework/paths/__init__.py` & `dtpyappframework-1.2/src/dtPyAppFramework/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `dtPyAppFramework-1.1/src/dtPyAppFramework/process/__init__.py` & `dtpyappframework-1.2/src/dtPyAppFramework/process/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,24 +80,27 @@
                 self.application_settings = settings.Settings(application_paths=self.application_paths,
                                                               app_short_name=self.short_name)
                 self.resource_manager = resources.ResourceManager(application_paths=self.application_paths)
                 self.log_path = app_logging.initialise_logging(redirect_console=not self.console_app,
                                                                spawned_process=True,
                                                                job_id=job_id, worker_id=worker_id,
                                                                parent_log_path=parent_log_path)
+                self.application_settings.init_settings_readers()
+                self.application_settings.secret_manager.load_cloud_stores()
 
                 self.__initialise_stdout_capt__()
 
                 header_message = f'SPAWNED PROCESS --- {self.full_name} ({self.short_name}), ' \
                                  f'Version: {self.version}. '
                 logging.info(header_message)
                 print(header_message)
 
                 self.load_config()
 
+
         except Exception as ex:
             logging.exception(ex)
             if not self.console_app:
                 self.stdout_txt_file.close()
                 self.stderr_txt_file.close()
 
     def __initialise_stdout_capt__(self):
@@ -123,26 +126,27 @@
         self.multiprocessing_manager = MultiProcessingManager()
         try:
             if not is_multiprocess_spawned_instance():
                 self.application_paths = paths.ApplicationPaths(app_short_name=self.short_name)
                 self.application_settings = settings.Settings(application_paths=self.application_paths)
                 self.resource_manager = resources.ResourceManager(application_paths=self.application_paths)
                 self.log_path = app_logging.initialise_logging(redirect_console=not self.console_app)
-
+                self.application_settings.init_settings_readers()
                 self.application_settings.secret_manager.load_cloud_stores()
                 self.__initialise_stdout_capt__()
 
                 header_message = f'{self.full_name} ({self.short_name}), ' \
                                  f'Version: {self.version}. Process ID: {os.getpid()}'
                 logging.info(header_message)
                 print(header_message)
                 if self.log_path is not None:
                     print(f'Log Path: {self.log_path}')
                     self.multiprocessing_manager.set_log_path(self.log_path)
                 args = arg_parser.parse_args()
+
                 if args.add_secret:
                     self.__add_secret__(args)
                 else:
                     self.__main__(args)
 
         except KeyboardInterrupt as kbi:
             logging.warning('(KeyboardInterrupt) Exiting application.')
```

### Comparing `dtPyAppFramework-1.1/src/dtPyAppFramework/process/multiprocessing.py` & `dtpyappframework-1.2/src/dtPyAppFramework/process/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `dtPyAppFramework-1.1/src/dtPyAppFramework/resources/__init__.py` & `dtpyappframework-1.2/src/dtPyAppFramework/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `dtPyAppFramework-1.1/src/dtPyAppFramework/settings/__init__.py` & `dtpyappframework-1.2/src/dtPyAppFramework/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `dtPyAppFramework-1.1/src/dtPyAppFramework/settings/secrets/__init__.py` & `dtpyappframework-1.2/src/dtPyAppFramework/settings/secrets/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,17 +104,20 @@
         Returns:
             Secret value if found, else default_value.
         """
         value = None
         if key.startswith("Secret#"):
             elements = key.split("#")
             store_name = elements[1]
+        else:
+            elements = key.split(".")
+            store_name = elements[0]
 
         for store in self.stores:
-            if store_name and store_name == store.store_name():
+            if store_name and store_name == store.store_name:
                 value = store.get_secret(key, None)
                 break
             elif not store_name:
                 value = store.get_secret(key, None)
                 if value:
                     break
```

### Comparing `dtPyAppFramework-1.1/src/dtPyAppFramework/settings/secrets/aws_secret_store.py` & `dtpyappframework-1.2/src/dtPyAppFramework/settings/secrets/aws_secret_store.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import json
+
 from .secret_store import AbstractSecretStore, SecretsStoreException
 from shutil import which
 from ...misc import run_cmd
 import boto3
 import logging
 
 class AWSSecretsStore(AbstractSecretStore):
@@ -41,14 +43,16 @@
         # Get AWS region
         self.aws_region = self.get_store_setting('aws_region')
         if not self.aws_region:
             raise SecretsStoreException('AWS Secrets Store is missing required aws_region parameter.')
 
         self.aws_session = None
 
+        self.secret_name = self.get_store_setting('secret_name')
+
         # Initialize AWS session based on profile type
         if self.aws_profile == 'key':
             aws_access_key_id = self.get_store_setting('aws_access_key_id')
             aws_secret_access_key = self.get_store_setting('aws_secret_access_key')
             if not aws_access_key_id or not aws_secret_access_key:
                 raise SecretsStoreException('AWS Secrets Store of type key requires both aws_access_key_id and aws_secret_access_key parameters.')
             self.aws_session = boto3.session.Session(region_name=self.aws_region, aws_access_key_id=aws_access_key_id,
@@ -68,29 +72,45 @@
         self.aws_secretsmanager = self.aws_session.client('secretsmanager')
         try:
             # Check if AWS Secrets Manager is accessible
             self.aws_secretsmanager.list_secrets()
         except Exception as ex:
             raise SecretsStoreException(f'AWS Secrets Store, Not Available. Error: {str(ex)}')
 
+        logging.info(f'Initialised AWS Secrets Manager {store_name}')
+
     def get_secret(self, key, default_value=None):
         """
         Get a secret from the AWS Secrets Manager.
 
         Args:
             key (str): Key of the secret.
             default_value: Default value to return if the secret is not found.
 
         Returns:
             Secret value if found, else default_value.
         """
         try:
-            entry = self.aws_secretsmanager.get_secret_value(SecretId=key)['SecretString']
+            if self.secret_name is not None:
+                entry = self.aws_secretsmanager.get_secret_value(SecretId=self.secret_name)['SecretString']
+            else:
+                entry = self.aws_secretsmanager.get_secret_value(SecretId=key)['SecretString']
+            if entry.startswith('{'):
+                entry = json.loads(entry)
+
+            if len(key.split('.')) == 0:
+                return entry
+            elif len(key.split('.')) == 2:
+                return entry[key.split('.')[1]]
+            elif len(key.split('.')) == 1 and key == self.store_name:
+                return entry
+            else:
+                raise SecretsStoreException(f'Unrecognised AWS Key of secret {key}')
         except Exception as ex:
-            logging.error(str(ex))
+            logging.error(f'{str(ex)} KEY: {key}')
             entry = None
 
         if not entry:
             entry = default_value
 
         return entry
```

### Comparing `dtPyAppFramework-1.1/src/dtPyAppFramework/settings/secrets/azure_secret_store.py` & `dtpyappframework-1.2/src/dtPyAppFramework/settings/secrets/azure_secret_store.py`

 * *Files identical despite different names*

### Comparing `dtPyAppFramework-1.1/src/dtPyAppFramework/settings/secrets/local_secret_store.py` & `dtpyappframework-1.2/src/dtPyAppFramework/settings/secrets/local_secret_store.py`

 * *Files identical despite different names*

### Comparing `dtPyAppFramework-1.1/src/dtPyAppFramework/settings/secrets/secret_store.py` & `dtpyappframework-1.2/src/dtPyAppFramework/settings/secrets/secret_store.py`

 * *Files identical despite different names*

### Comparing `dtPyAppFramework-1.1/src/dtPyAppFramework/settings/settings_reader.py` & `dtpyappframework-1.2/src/dtPyAppFramework/settings/settings_reader.py`

 * *Files identical despite different names*

### Comparing `dtPyAppFramework-1.1/src/dtPyAppFramework.egg-info/PKG-INFO` & `dtpyappframework-1.2/src/dtPyAppFramework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtPyAppFramework
-Version: 1.1
+Version: 1.2
 Summary: A Python library for common features in application development.
 Author-email: Digital-Thought <dev@digital-thought.org>
 Maintainer-email: Digital-Thought <dev@digital-thought.org>
 License: MIT License
         
         Copyright (c) 2024 Digital-Thought
         
@@ -85,15 +85,15 @@
 ## Getting Started
 ### AbstractApp Class ###
 The **`AbstractApp`** class serves as a base class for creating Python applications. It handles common initialisation tasks and provides a structure for defining command-line arguments and the main application logic.
 
 
 To create a simple Python application using dtPyAppFramework:
 ```python
-from dtPyAppFramework.app import AbstractApp
+from dtPyAppFramework.application import AbstractApp
 from dtPyAppFramework import settings
 
 import logging
 
 class MyApplication(AbstractApp):
 
     def define_args(self, arg_parser):
```

### Comparing `dtPyAppFramework-1.1/src/dtPyAppFramework.egg-info/SOURCES.txt` & `dtpyappframework-1.2/src/dtPyAppFramework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

