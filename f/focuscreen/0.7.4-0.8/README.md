# Comparing `tmp/focuscreen-0.7.4.tar.gz` & `tmp/focuscreen-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "focuscreen-0.7.4.tar", last modified: Tue Apr 30 03:24:20 2024, max compression
+gzip compressed data, was "focuscreen-0.8.tar", last modified: Sun May  5 05:59:32 2024, max compression
```

## Comparing `focuscreen-0.7.4.tar` & `focuscreen-0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:24:20.393055 focuscreen-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-30 03:24:20.393055 focuscreen-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-30 03:24:10.000000 focuscreen-0.7.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-30 03:24:10.000000 focuscreen-0.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 03:24:20.393055 focuscreen-0.7.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:24:20.389055 focuscreen-0.7.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:24:20.393055 focuscreen-0.7.4/src/focuscreen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 03:24:10.000000 focuscreen-0.7.4/src/focuscreen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-30 03:24:10.000000 focuscreen-0.7.4/src/focuscreen/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-30 03:24:10.000000 focuscreen-0.7.4/src/focuscreen/cursor_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-30 03:24:10.000000 focuscreen-0.7.4/src/focuscreen/focus_region_updater.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:24:20.393055 focuscreen-0.7.4/src/focuscreen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-30 03:24:20.000000 focuscreen-0.7.4/src/focuscreen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-30 03:24:20.000000 focuscreen-0.7.4/src/focuscreen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 03:24:20.000000 focuscreen-0.7.4/src/focuscreen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-30 03:24:20.000000 focuscreen-0.7.4/src/focuscreen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-30 03:24:20.000000 focuscreen-0.7.4/src/focuscreen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 05:59:32.449048 focuscreen-0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-05 05:59:32.449048 focuscreen-0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-05 05:59:22.000000 focuscreen-0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-05 05:59:22.000000 focuscreen-0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 05:59:32.449048 focuscreen-0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 05:59:32.449048 focuscreen-0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 05:59:32.449048 focuscreen-0.8/src/focuscreen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 05:59:22.000000 focuscreen-0.8/src/focuscreen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-05-05 05:59:22.000000 focuscreen-0.8/src/focuscreen/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-05 05:59:22.000000 focuscreen-0.8/src/focuscreen/cursor_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-05 05:59:22.000000 focuscreen-0.8/src/focuscreen/focus_region_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 05:59:32.449048 focuscreen-0.8/src/focuscreen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-05 05:59:32.000000 focuscreen-0.8/src/focuscreen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-05 05:59:32.000000 focuscreen-0.8/src/focuscreen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 05:59:32.000000 focuscreen-0.8/src/focuscreen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-05 05:59:32.000000 focuscreen-0.8/src/focuscreen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-05 05:59:32.000000 focuscreen-0.8/src/focuscreen.egg-info/top_level.txt
```

### Comparing `focuscreen-0.7.4/PKG-INFO` & `focuscreen-0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: focuscreen
-Version: 0.7.4
+Version: 0.8
 Summary: Snap screen by focusing on mouse and keyboard events
 Author: Hansimov
 Project-URL: Homepage, https://github.com/Hansimov/focuscreen
 Project-URL: Issues, https://github.com/Hansimov/focuscreen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `focuscreen-0.7.4/pyproject.toml` & `focuscreen-0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "focuscreen"
-version = "0.7.4"
+version = "0.8"
 authors = [
     { name="Hansimov" },
 ]
 description = "Snap screen by focusing on mouse and keyboard events"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `focuscreen-0.7.4/src/focuscreen/app.py` & `focuscreen-0.8/src/focuscreen/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,18 @@
     def setup_window(self):
         cv2.namedWindow(self.window_name, cv2.WINDOW_NORMAL)
         cv2.resizeWindow(self.window_name, self.window_width, self.window_height)
 
     def on_mouse_move(self, x, y):
         self.mouse_x, self.mouse_y = x, y
 
+    def on_mouse_click(self, x, y, button, pressed):
+        if pressed:
+            self.cursor_renderer.on_click()
+
     def detect_active_monitor(self):
         """detect active monitor, where the mouse is currently located"""
         self.active_monitor = None
         for idx, monitor in enumerate(self.monitors[1:]):
             if (
                 self.mouse_x >= monitor["left"]
                 and self.mouse_x <= monitor["left"] + monitor["width"]
@@ -93,15 +97,17 @@
             frame, self.mouse_x, self.mouse_y, self.region_x1, self.region_y1
         )
 
     def run(self):
         """use mss to capture screen, and use cv2 to real-time display each frame"""
         with mss() as sct:
             self.monitors = sct.monitors
-            with mouse.Listener(on_move=self.on_mouse_move) as listener:
+            with mouse.Listener(
+                on_move=self.on_mouse_move, on_click=self.on_mouse_click
+            ) as listener:
                 while True:
                     self.detect_active_monitor()
                     self.calc_focus_region()
                     frame = sct.grab(self.mouse_region)
                     frame_np = np.array(frame)
                     self.render_cursor_and_key_strokes(frame_np)
                     cv2.imshow(self.window_name, frame_np)
```

### Comparing `focuscreen-0.7.4/src/focuscreen/focus_region_updater.py` & `focuscreen-0.8/src/focuscreen/focus_region_updater.py`

 * *Files identical despite different names*

### Comparing `focuscreen-0.7.4/src/focuscreen.egg-info/PKG-INFO` & `focuscreen-0.8/src/focuscreen.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: focuscreen
-Version: 0.7.4
+Version: 0.8
 Summary: Snap screen by focusing on mouse and keyboard events
 Author: Hansimov
 Project-URL: Homepage, https://github.com/Hansimov/focuscreen
 Project-URL: Issues, https://github.com/Hansimov/focuscreen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

