# Comparing `tmp/drafter-1.1.4.tar.gz` & `tmp/drafter-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drafter-1.1.4.tar", last modified: Fri May  3 16:34:43 2024, max compression
+gzip compressed data, was "drafter-1.2.0.tar", last modified: Sun May  5 15:26:13 2024, max compression
```

## Comparing `drafter-1.1.4.tar` & `drafter-1.2.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 16:34:43.387336 drafter-1.1.4/
--rw-rw-rw-   0        0        0     1075 2021-09-26 08:48:54.000000 drafter-1.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0      766 2024-05-03 16:34:43.386342 drafter-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       57 2023-09-04 16:32:22.000000 drafter-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 16:34:43.371337 drafter-1.1.4/drafter/
--rw-rw-rw-   0        0        0      431 2024-05-03 16:34:38.000000 drafter-1.1.4/drafter/__init__.py
--rw-rw-rw-   0        0        0    12946 2024-04-26 19:40:44.000000 drafter-1.1.4/drafter/components.py
--rw-rw-rw-   0        0        0      190 2024-04-26 19:36:49.000000 drafter-1.1.4/drafter/constants.py
--rw-rw-rw-   0        0        0     6808 2024-04-25 03:04:30.000000 drafter-1.1.4/drafter/debug.py
--rw-rw-rw-   0        0        0     1000 2024-04-28 15:20:07.000000 drafter-1.1.4/drafter/deploy.py
--rw-rw-rw-   0        0        0     7129 2024-04-28 15:34:19.000000 drafter-1.1.4/drafter/files.py
--rw-rw-rw-   0        0        0     4868 2024-04-26 19:41:14.000000 drafter-1.1.4/drafter/history.py
--rw-rw-rw-   0        0        0     1980 2024-04-28 15:16:39.000000 drafter-1.1.4/drafter/page.py
--rw-rw-rw-   0        0        0      437 2024-04-25 00:00:05.000000 drafter-1.1.4/drafter/routes.py
--rw-rw-rw-   0        0        0    18995 2024-05-03 16:15:17.000000 drafter-1.1.4/drafter/server.py
--rw-rw-rw-   0        0        0      893 2024-04-24 23:42:42.000000 drafter-1.1.4/drafter/setup.py
--rw-rw-rw-   0        0        0     3205 2024-04-24 23:45:48.000000 drafter-1.1.4/drafter/styling.py
--rw-rw-rw-   0        0        0     2911 2024-05-03 16:34:10.000000 drafter-1.1.4/drafter/testing.py
--rw-rw-rw-   0        0        0     2210 2024-04-25 03:03:35.000000 drafter-1.1.4/drafter/urls.py
-drwxrwxrwx   0        0        0        0 2024-05-03 16:34:43.386342 drafter-1.1.4/drafter.egg-info/
--rw-rw-rw-   0        0        0      766 2024-05-03 16:34:43.000000 drafter-1.1.4/drafter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2024-05-03 16:34:43.000000 drafter-1.1.4/drafter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 16:34:43.000000 drafter-1.1.4/drafter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-03 16:34:43.000000 drafter-1.1.4/drafter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-03 16:34:43.000000 drafter-1.1.4/drafter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       80 2023-08-30 14:30:23.000000 drafter-1.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-03 16:34:43.387336 drafter-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1218 2024-04-29 15:35:39.000000 drafter-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:26:13.580046 drafter-1.2.0/
+-rw-rw-rw-   0        0        0     1075 2021-09-26 08:48:54.000000 drafter-1.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      766 2024-05-05 15:26:13.579086 drafter-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       57 2023-09-04 16:32:22.000000 drafter-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 15:26:13.563909 drafter-1.2.0/drafter/
+-rw-rw-rw-   0        0        0      431 2024-05-05 15:17:16.000000 drafter-1.2.0/drafter/__init__.py
+-rw-rw-rw-   0        0        0    13266 2024-05-05 15:23:42.000000 drafter-1.2.0/drafter/components.py
+-rw-rw-rw-   0        0        0     1017 2024-05-05 15:22:30.000000 drafter-1.2.0/drafter/configuration.py
+-rw-rw-rw-   0        0        0      190 2024-04-26 19:36:49.000000 drafter-1.2.0/drafter/constants.py
+-rw-rw-rw-   0        0        0     6808 2024-04-25 03:04:30.000000 drafter-1.2.0/drafter/debug.py
+-rw-rw-rw-   0        0        0     1000 2024-04-28 15:20:07.000000 drafter-1.2.0/drafter/deploy.py
+-rw-rw-rw-   0        0        0     7129 2024-04-28 15:34:19.000000 drafter-1.2.0/drafter/files.py
+-rw-rw-rw-   0        0        0     4868 2024-04-26 19:41:14.000000 drafter-1.2.0/drafter/history.py
+-rw-rw-rw-   0        0        0     2105 2024-05-05 15:14:02.000000 drafter-1.2.0/drafter/page.py
+-rw-rw-rw-   0        0        0      437 2024-04-25 00:00:05.000000 drafter-1.2.0/drafter/routes.py
+-rw-rw-rw-   0        0        0    18138 2024-05-05 15:22:59.000000 drafter-1.2.0/drafter/server.py
+-rw-rw-rw-   0        0        0      893 2024-04-24 23:42:42.000000 drafter-1.2.0/drafter/setup.py
+-rw-rw-rw-   0        0        0     3205 2024-04-24 23:45:48.000000 drafter-1.2.0/drafter/styling.py
+-rw-rw-rw-   0        0        0     2911 2024-05-03 16:34:10.000000 drafter-1.2.0/drafter/testing.py
+-rw-rw-rw-   0        0        0     2210 2024-04-25 03:03:35.000000 drafter-1.2.0/drafter/urls.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:26:13.579086 drafter-1.2.0/drafter.egg-info/
+-rw-rw-rw-   0        0        0      766 2024-05-05 15:26:13.000000 drafter-1.2.0/drafter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      481 2024-05-05 15:26:13.000000 drafter-1.2.0/drafter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 15:26:13.000000 drafter-1.2.0/drafter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-05 15:26:13.000000 drafter-1.2.0/drafter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-05 15:26:13.000000 drafter-1.2.0/drafter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       80 2023-08-30 14:30:23.000000 drafter-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-05 15:26:13.580046 drafter-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1218 2024-04-29 15:35:39.000000 drafter-1.2.0/setup.py
```

### Comparing `drafter-1.1.4/LICENSE.txt` & `drafter-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `drafter-1.1.4/PKG-INFO` & `drafter-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drafter
-Version: 1.1.4
+Version: 1.2.0
 Summary: Student-friendly full stack web development library.
 Home-page: https://github.com/drafter-edu/drafter
 Author: acbart
 Author-email: acbart@udel.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Education
```

### Comparing `drafter-1.1.4/drafter/components.py` & `drafter-1.2.0/drafter/components.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,17 @@
         self.extra_settings[f"style_{style}"] = value
         return self
 
     def update_attr(self, attr, value):
         self.extra_settings[attr] = value
         return self
 
+    def render(self, current_state, configuration):
+        return str(self)
+
 
 class LinkContent:
     def _handle_url(self, url, external=None):
         if callable(url):
             url = url.__name__
         if external is None:
             external = check_invalid_external_url(url) != ""
@@ -136,24 +139,29 @@
     height: int
 
     def __init__(self, url: str, width=None, height=None, **kwargs):
         self.url = url
         self.width = width
         self.height = height
         self.extra_settings = kwargs
+        self.base_image_folder = BASE_IMAGE_FOLDER
+
+    def render(self, current_state, configuration):
+        self.base_image_folder = configuration.deploy_image_path
+        return super().render(current_state, configuration)
 
     def __str__(self) -> str:
         extra_settings = {}
         if self.width is not None:
             extra_settings['width'] = self.width
         if self.height is not None:
             extra_settings['height'] = self.height
         url, external = self._handle_url(self.url)
         if not external:
-            url = BASE_IMAGE_FOLDER + url
+            url = self.base_image_folder + url
         parsed_settings = self.parse_extra_settings(**extra_settings)
         return f"<img src='{url}' {parsed_settings}>"
 
 
 @dataclass
 class TextBox(PageContent):
     name: str
```

### Comparing `drafter-1.1.4/drafter/debug.py` & `drafter-1.2.0/drafter/debug.py`

 * *Files identical despite different names*

### Comparing `drafter-1.1.4/drafter/deploy.py` & `drafter-1.2.0/drafter/deploy.py`

 * *Files identical despite different names*

### Comparing `drafter-1.1.4/drafter/files.py` & `drafter-1.2.0/drafter/files.py`

 * *Files identical despite different names*

### Comparing `drafter-1.1.4/drafter/history.py` & `drafter-1.2.0/drafter/history.py`

 * *Files identical despite different names*

### Comparing `drafter-1.1.4/drafter/page.py` & `drafter-1.2.0/drafter/page.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from dataclasses import dataclass
 from typing import Any
 
+from drafter.configuration import ServerConfiguration
 from drafter.constants import RESTORABLE_STATE_KEY
 from drafter.components import PageContent, Link
 
 
 @dataclass
 class Page:
     state: Any
@@ -23,28 +24,28 @@
         else:
             for index, chunk in enumerate(content):
                 if not isinstance(chunk, (str, PageContent)):
                     incorrect_type = type(chunk).__name__
                     raise ValueError("The content of a page must be a list of strings or components."
                                      f" Found {incorrect_type} at index {index} instead.")
 
-    def render_content(self, current_state, framed: bool, title: str) -> str:
+    def render_content(self, current_state, configuration: ServerConfiguration) -> str:
         # TODO: Decide if we want to dump state on the page
         chunked = [
             # f'<input type="hidden" name="{RESTORABLE_STATE_KEY}" value={current_state!r}/>'
         ]
         for chunk in self.content:
             if isinstance(chunk, str):
                 chunked.append(f"<p>{chunk}</p>")
             else:
-                chunked.append(str(chunk))
+                chunked.append(chunk.render(current_state, configuration))
         content = "\n".join(chunked)
         content = f"<form>{content}</form>"
-        if framed:
-            content = (f"<div class='container btlw-header'>{title}</div>"
+        if configuration.framed:
+            content = (f"<div class='container btlw-header'>{configuration.title}</div>"
                        f"<div class='container btlw-container'>{content}</div>")
         return content
 
     def verify_content(self, server) -> bool:
         for chunk in self.content:
             if isinstance(chunk, Link):
                 chunk.verify(server)
```

### Comparing `drafter-1.1.4/drafter/server.py` & `drafter-1.2.0/drafter/server.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,68 +4,27 @@
 from dataclasses import dataclass, asdict, replace, field
 from functools import wraps
 from typing import Any
 import json
 import inspect
 
 from drafter import friendly_urls, PageContent
+from drafter.configuration import ServerConfiguration
 from drafter.constants import RESTORABLE_STATE_KEY, SUBMIT_BUTTON_KEY, PREVIOUSLY_PRESSED_BUTTON
 from drafter.debug import DebugInformation
-from drafter.setup import DEFAULT_BACKEND, Bottle, abort, request, static_file
+from drafter.setup import Bottle, abort, request, static_file
 from drafter.history import VisitedPage, rehydrate_json, dehydrate_json, ConversionRecord, UnchangedRecord, get_params, \
     remap_hidden_form_parameters
 from drafter.page import Page
 from drafter.files import TEMPLATE_200, TEMPLATE_404, TEMPLATE_500, INCLUDE_STYLES, TEMPLATE_200_WITHOUT_HEADER
 from drafter.urls import remove_url_query_params
 
 import logging
 logger = logging.getLogger('drafter')
 
-"""
-Images folder
-    Specific folder
-    Any adjacent file
-Current page title
-CSS style (skeleton, bootstrap, etc.)
-    Additional CSS Files
-    Additional JS Files
-    Additional header content
-Frame style (full, embed)
-
-TODO:
-Custom Error pages
-Shareable link to get a link to the current page
-Download/upload state button
-"""
-
-
-@dataclass
-class ServerConfiguration:
-    # Launch parameters
-    host: str = "localhost"
-    port: int = 8080
-    debug: bool = True
-    # "none", "flask", etc.
-    backend: str = DEFAULT_BACKEND
-    reloader: bool = False
-    # This makes the server not run (e.g., to only run tests)
-    skip: bool = os.environ.get('DRAFTER_SKIP', False)
-
-    # Website configuration
-    title: str = "Drafter Website"
-    framed: bool = True
-    skulpt: bool = os.environ.get('DRAFTER_SKULPT', True)
-
-    # Page configuration
-    style: str = 'skeleton'
-    additional_header_content: list[str] = field(default_factory=list)
-    additional_css_content: list[str] = field(default_factory=list)
-
-
-
 
 class Server:
     _page_history: list[tuple[VisitedPage, Any]]
 
     def __init__(self, **kwargs):
         self.routes = {}
         self._handle_route = {}
@@ -74,15 +33,14 @@
         self._initial_state = None
         self._state_history = []
         self._state_frozen_history = []
         self._page_history = []
         self._conversion_record = []
         self.original_routes = []
         self.app = None
-        self.image_folder = '__images'
 
     def reset(self):
         self.routes.clear()
 
     def dump_state(self):
         return json.dumps(dehydrate_json(self._state))
 
@@ -196,18 +154,19 @@
         # Final return result
         representation = [repr(arg) for arg in args] + [
             f"{key}={value!r}" if show_names.get(key, False) else repr(value)
             for key, value in sorted(kwargs.items(), key=lambda item: expected_parameters.index(item[0]))]
         return args, kwargs, ", ".join(representation), button_pressed
 
     def handle_images(self):
-        self.app.route(f'/{self.image_folder}/<path:path>', 'GET', self.serve_image)
+        if self.configuration.deploy_image_path:
+            self.app.route(f"/{self.configuration.deploy_image_path}/<path:path>", 'GET', self.serve_image)
 
     def serve_image(self, path):
-        return static_file(path, root='./', mimetype='image/png')
+        return static_file(path, root='./' + self.configuration.src_image_folder, mimetype='image/png')
 
     def convert_parameter(self, param, val, expected_types):
         if param in expected_types:
             expected_type = expected_types[param]
             if expected_type == inspect.Parameter.empty:
                 self._conversion_record.append(UnchangedRecord(param, val, expected_types[param]))
                 return val
@@ -258,15 +217,15 @@
                 page.verify_content(self)
             except Exception as e:
                 return self.make_error_page("Error verifying content", e, original_function)
             self._state_history.append(page.state)
             self._state = page.state
             visiting_page.update("Rendering Page Content")
             try:
-                content = page.render_content(self.dump_state(), self.configuration.framed, self.configuration.title)
+                content = page.render_content(self.dump_state(), self.configuration)
             except Exception as e:
                 return self.make_error_page("Error rendering content", e, original_function)
             visiting_page.finish("Finished Page Load")
             if self.configuration.debug:
                 content = content + self.make_debug_page()
             content = self.wrap_page(content)
             return content
@@ -377,13 +336,17 @@
         content = DebugInformation(self._page_history, self._state, self.routes, self._conversion_record)
         return content.generate()
 
 
 MAIN_SERVER = Server()
 
 
+def get_server_setting(key, default=None, server=MAIN_SERVER):
+    return getattr(server.configuration, key, default)
+
+
 def start_server(initial_state=None, server: Server = MAIN_SERVER, skip=False, **kwargs):
     if server.configuration.skip or skip:
         logger.info("Skipping server setup and execution")
         return
     server.setup(initial_state)
     server.run(**kwargs)
```

### Comparing `drafter-1.1.4/drafter/setup.py` & `drafter-1.2.0/drafter/setup.py`

 * *Files identical despite different names*

### Comparing `drafter-1.1.4/drafter/styling.py` & `drafter-1.2.0/drafter/styling.py`

 * *Files identical despite different names*

### Comparing `drafter-1.1.4/drafter/testing.py` & `drafter-1.2.0/drafter/testing.py`

 * *Files identical despite different names*

### Comparing `drafter-1.1.4/drafter/urls.py` & `drafter-1.2.0/drafter/urls.py`

 * *Files identical despite different names*

### Comparing `drafter-1.1.4/drafter.egg-info/PKG-INFO` & `drafter-1.2.0/drafter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drafter
-Version: 1.1.4
+Version: 1.2.0
 Summary: Student-friendly full stack web development library.
 Home-page: https://github.com/drafter-edu/drafter
 Author: acbart
 Author-email: acbart@udel.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Education
```

### Comparing `drafter-1.1.4/setup.py` & `drafter-1.2.0/setup.py`

 * *Files identical despite different names*

