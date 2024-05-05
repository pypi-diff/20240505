# Comparing `tmp/mehditor-0.1.6.tar.gz` & `tmp/mehditor-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mehditor-0.1.6.tar", max compression
+gzip compressed data, was "mehditor-0.2.0.tar", max compression
```

## Comparing `mehditor-0.1.6.tar` & `mehditor-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1464 2024-02-21 17:02:00.739053 mehditor-0.1.6/README.md
--rw-r--r--   0        0        0        0 2024-02-21 17:02:00.739053 mehditor-0.1.6/mehditor/__init__.py
--rw-r--r--   0        0        0     2517 2024-02-21 17:02:00.739053 mehditor-0.1.6/mehditor/app_commands.py
--rw-r--r--   0        0        0     3006 2024-02-21 17:02:00.739053 mehditor-0.1.6/mehditor/config.py
--rw-r--r--   0        0        0      450 2024-02-21 17:02:00.739053 mehditor-0.1.6/mehditor/main.py
--rw-r--r--   0        0        0        0 2024-02-21 17:02:00.739053 mehditor-0.1.6/mehditor/screens/__init__.py
--rw-r--r--   0        0        0     1619 2024-02-21 17:02:00.739053 mehditor-0.1.6/mehditor/screens/about.py
--rw-r--r--   0        0        0     6330 2024-02-21 17:02:00.739053 mehditor-0.1.6/mehditor/screens/app_menu.py
--rw-r--r--   0        0        0     1336 2024-02-21 17:02:00.739053 mehditor-0.1.6/mehditor/screens/chooser.py
--rw-r--r--   0        0        0     1354 2024-02-21 17:02:00.739053 mehditor-0.1.6/mehditor/screens/confirm_dialog.py
--rw-r--r--   0        0        0     3822 2024-02-21 17:02:00.739053 mehditor-0.1.6/mehditor/screens/file_chooser.py
--rw-r--r--   0        0        0      176 2024-02-21 17:02:00.739053 mehditor-0.1.6/mehditor/screens/file_open.py
--rw-r--r--   0        0        0      311 2024-02-21 17:02:00.739053 mehditor-0.1.6/mehditor/screens/file_save.py
--rw-r--r--   0        0        0     1721 2024-02-21 17:02:00.739053 mehditor-0.1.6/mehditor/screens/file_settings.py
--rw-r--r--   0        0        0      783 2024-02-21 17:02:00.739053 mehditor-0.1.6/mehditor/screens/hotkeys.py
--rw-r--r--   0        0        0     1098 2024-02-21 17:02:00.739053 mehditor-0.1.6/mehditor/screens/input_prompt.py
--rw-r--r--   0        0        0    13750 2024-02-21 17:02:00.739053 mehditor-0.1.6/mehditor/screens/mehditor_app.py
--rw-r--r--   0        0        0     1728 2024-02-21 17:02:00.739053 mehditor-0.1.6/mehditor/screens/quit_screen.py
--rw-r--r--   0        0        0     2003 2024-02-21 17:02:00.739053 mehditor-0.1.6/mehditor/screens/shortcuts.py
--rw-r--r--   0        0        0      692 2024-02-21 17:02:00.739053 mehditor-0.1.6/mehditor/validators.py
--rw-r--r--   0        0        0        0 2024-02-21 17:02:00.739053 mehditor-0.1.6/mehditor/widgets/__init__.py
--rw-r--r--   0        0        0     3267 2024-02-21 17:02:00.739053 mehditor-0.1.6/mehditor/widgets/better_text_area.py
--rw-r--r--   0        0        0      525 2024-02-21 17:02:00.739053 mehditor-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2012 1970-01-01 00:00:00.000000 mehditor-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1464 2024-05-05 09:58:29.061414 mehditor-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-05 09:58:29.061414 mehditor-0.2.0/mehditor/__init__.py
+-rw-r--r--   0        0        0     2517 2024-05-05 09:58:29.061414 mehditor-0.2.0/mehditor/app_commands.py
+-rw-r--r--   0        0        0     3006 2024-05-05 09:58:29.061414 mehditor-0.2.0/mehditor/config.py
+-rw-r--r--   0        0        0      450 2024-05-05 09:58:29.061414 mehditor-0.2.0/mehditor/main.py
+-rw-r--r--   0        0        0        0 2024-05-05 09:58:29.061414 mehditor-0.2.0/mehditor/screens/__init__.py
+-rw-r--r--   0        0        0     1619 2024-05-05 09:58:29.061414 mehditor-0.2.0/mehditor/screens/about.py
+-rw-r--r--   0        0        0     6330 2024-05-05 09:58:29.061414 mehditor-0.2.0/mehditor/screens/app_menu.py
+-rw-r--r--   0        0        0     1336 2024-05-05 09:58:29.061414 mehditor-0.2.0/mehditor/screens/chooser.py
+-rw-r--r--   0        0        0     1354 2024-05-05 09:58:29.061414 mehditor-0.2.0/mehditor/screens/confirm_dialog.py
+-rw-r--r--   0        0        0     3822 2024-05-05 09:58:29.061414 mehditor-0.2.0/mehditor/screens/file_chooser.py
+-rw-r--r--   0        0        0      176 2024-05-05 09:58:29.065414 mehditor-0.2.0/mehditor/screens/file_open.py
+-rw-r--r--   0        0        0      311 2024-05-05 09:58:29.065414 mehditor-0.2.0/mehditor/screens/file_save.py
+-rw-r--r--   0        0        0     1721 2024-05-05 09:58:29.065414 mehditor-0.2.0/mehditor/screens/file_settings.py
+-rw-r--r--   0        0        0      783 2024-05-05 09:58:29.065414 mehditor-0.2.0/mehditor/screens/hotkeys.py
+-rw-r--r--   0        0        0     1098 2024-05-05 09:58:29.065414 mehditor-0.2.0/mehditor/screens/input_prompt.py
+-rw-r--r--   0        0        0    14418 2024-05-05 09:58:29.065414 mehditor-0.2.0/mehditor/screens/mehditor_app.py
+-rw-r--r--   0        0        0     1728 2024-05-05 09:58:29.065414 mehditor-0.2.0/mehditor/screens/quit_screen.py
+-rw-r--r--   0        0        0     2003 2024-05-05 09:58:29.065414 mehditor-0.2.0/mehditor/screens/shortcuts.py
+-rw-r--r--   0        0        0      692 2024-05-05 09:58:29.065414 mehditor-0.2.0/mehditor/validators.py
+-rw-r--r--   0        0        0        0 2024-05-05 09:58:29.065414 mehditor-0.2.0/mehditor/widgets/__init__.py
+-rw-r--r--   0        0        0     3267 2024-05-05 09:58:29.065414 mehditor-0.2.0/mehditor/widgets/better_text_area.py
+-rw-r--r--   0        0        0      525 2024-05-05 09:58:29.065414 mehditor-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2012 1970-01-01 00:00:00.000000 mehditor-0.2.0/PKG-INFO
```

### Comparing `mehditor-0.1.6/README.md` & `mehditor-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Modern but simple text editor
 
 Mehditor is a modern but simple text editor. I made it because I needed a quick editor (like Pico or Nano) on servers,
-but wanted a more modern and friendly itnerface. Meditor is written in Python and uses the excellent
+but wanted a more modern and friendly interface. Meditor is written in Python and uses the excellent
  [Textual](https://textual.textualize.io) for its user interface. I wrote it in a weekend.
 
 ![Mehditor screenshot showing application in terminal window](https://github.com/kkinder/mehditor/blob/main/screenshots/meh-1.png)
 
 ![Mehditor screenshot showing application in terminal window](https://github.com/kkinder/mehditor/blob/main/screenshots/meh-2.png)
 
 ![Mehditor screenshot showing application in terminal window](https://github.com/kkinder/mehditor/blob/main/screenshots/meh-3.png)
```

### Comparing `mehditor-0.1.6/mehditor/app_commands.py` & `mehditor-0.2.0/mehditor/app_commands.py`

 * *Files identical despite different names*

### Comparing `mehditor-0.1.6/mehditor/config.py` & `mehditor-0.2.0/mehditor/config.py`

 * *Files identical despite different names*

### Comparing `mehditor-0.1.6/mehditor/screens/about.py` & `mehditor-0.2.0/mehditor/screens/about.py`

 * *Files identical despite different names*

### Comparing `mehditor-0.1.6/mehditor/screens/app_menu.py` & `mehditor-0.2.0/mehditor/screens/app_menu.py`

 * *Files identical despite different names*

### Comparing `mehditor-0.1.6/mehditor/screens/chooser.py` & `mehditor-0.2.0/mehditor/screens/chooser.py`

 * *Files identical despite different names*

### Comparing `mehditor-0.1.6/mehditor/screens/confirm_dialog.py` & `mehditor-0.2.0/mehditor/screens/confirm_dialog.py`

 * *Files identical despite different names*

### Comparing `mehditor-0.1.6/mehditor/screens/file_chooser.py` & `mehditor-0.2.0/mehditor/screens/file_chooser.py`

 * *Files identical despite different names*

### Comparing `mehditor-0.1.6/mehditor/screens/file_settings.py` & `mehditor-0.2.0/mehditor/screens/file_settings.py`

 * *Files identical despite different names*

### Comparing `mehditor-0.1.6/mehditor/screens/hotkeys.py` & `mehditor-0.2.0/mehditor/screens/hotkeys.py`

 * *Files identical despite different names*

### Comparing `mehditor-0.1.6/mehditor/screens/input_prompt.py` & `mehditor-0.2.0/mehditor/screens/input_prompt.py`

 * *Files identical despite different names*

### Comparing `mehditor-0.1.6/mehditor/screens/mehditor_app.py` & `mehditor-0.2.0/mehditor/screens/mehditor_app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import functools
 from pathlib import Path
 
 from textual import on
 from textual.app import App, ComposeResult
+from textual.notifications import Notification
 from textual.reactive import reactive
 from textual.screen import ModalScreen
 from textual.widgets import Header, Input, Footer
 from textual.widgets._text_area import ThemeDoesNotExist
 
 from mehditor import config
 from mehditor.app_commands import AppCommands
@@ -28,14 +30,28 @@
 }
 
 known_light_themes = {
     "github_light"
 }
 
 
+def handle_os_error_decorator(error_message, severity="error", timeout=Notification.timeout):
+    def decorator(func):
+        @functools.wraps(func)
+        def wrapper(self, *args, **kwargs):
+            try:
+                return func(self, *args, **kwargs)
+            except OSError as e:
+                self.notify(title=error_message, message=str(e), severity=severity, timeout=timeout)
+
+        return wrapper
+
+    return decorator
+
+
 class MeheditorApp(App):
     BINDINGS = [
         config.generate_binding("menu"),
         config.generate_binding("quit"),
         config.generate_binding("save_file"),
         config.generate_binding("new_file"),
         config.generate_binding("goto_line"),
@@ -92,14 +108,15 @@
     def new_file(self):
         self.query_one("#text-buffer").load_text("")
         self.query_one("#text-buffer").history.clear()
         self.file = None
         self.title = '(Untitled)'
         self.file_unsaved = False
 
+    @handle_os_error_decorator("Error Opening File")
     def open_file(self, file):
         file = Path(file)
         if file.exists():
             try:
                 text = file.read_text()
             except UnicodeDecodeError as e:
                 self.notify(f'Error decoding file (is it a text file?): {e}', severity="error", timeout=20)
@@ -109,14 +126,15 @@
 
         self.query_one("#text-buffer").load_text(text)
         self.query_one("#text-buffer").history.clear()
         self.file = Path(file).resolve() if file else None
         self.title = self.file.name
         self.file_unsaved = False
 
+    @handle_os_error_decorator("Error Saving Settings")
     def save_settings(self):
         config.settings['editing']['indent_type'] = self.indent_type
         config.settings['editing']['indent_width'] = str(self.indent_width)
         config.settings['editing']['theme'] = self.theme
         config.settings['editing']['dark_mode'] = 'Yes' if self.dark else 'No'
         config.settings['editing']['show_line_numbers'] = 'Yes' if self.show_line_numbers else 'No'
         config.settings['editing']['soft_wrap'] = 'Yes' if self.soft_wrap else 'No'
@@ -202,15 +220,17 @@
     def action_paste(self):
         if self.clipboard:
             tb: BetterTextArea = self.query_one("#text-buffer")
             tb.replace(self.clipboard, tb.selection.start, tb.selection.end)
         else:
             self.notify("Nothing to paste", severity="error")
 
+    @handle_os_error_decorator("Error Saving File")
     def action_save_file(self) -> None:
+
         if self.file:
             self.file.write_text(self.query_one("#text-buffer").text)
             self.file_unsaved = False
             self.notify("File saved")
         else:
             self.action_save_file_as()
 
@@ -318,21 +338,19 @@
         self.push_screen(
             InputPrompt(
                 "Choose indentation level",
                 str(self.indent_width)
             ),
             check_result)
 
-
     def action_change_theme(self):
         def check_result(result):
             self.theme = result
             self.save_settings()
 
-
         self.push_screen(
             Chooser(
                 "Choose Theme",
                 [(l, l) for l in self.query_one("#text-buffer").available_themes],
                 default=self.theme
             ),
             check_result)
```

### Comparing `mehditor-0.1.6/mehditor/screens/quit_screen.py` & `mehditor-0.2.0/mehditor/screens/quit_screen.py`

 * *Files identical despite different names*

### Comparing `mehditor-0.1.6/mehditor/screens/shortcuts.py` & `mehditor-0.2.0/mehditor/screens/shortcuts.py`

 * *Files identical despite different names*

### Comparing `mehditor-0.1.6/mehditor/validators.py` & `mehditor-0.2.0/mehditor/validators.py`

 * *Files identical despite different names*

### Comparing `mehditor-0.1.6/mehditor/widgets/better_text_area.py` & `mehditor-0.2.0/mehditor/widgets/better_text_area.py`

 * *Files identical despite different names*

### Comparing `mehditor-0.1.6/pyproject.toml` & `mehditor-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "mehditor"
-version = "0.1.6"
+version = "0.2.0"
 description = "A text editor for twentieth century computing."
 authors = ["Ken Kinder <ken+github@kkinder.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-textual = {extras = ["syntax"], version = "^0.52.1"}
+textual = {extras = ["syntax"], version = "^0.58.0"}
 
 [tool.poetry.group.dev.dependencies]
 textual-dev = "^1.5.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mehditor-0.1.6/PKG-INFO` & `mehditor-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: mehditor
-Version: 0.1.6
+Version: 0.2.0
 Summary: A text editor for twentieth century computing.
 License: MIT
 Author: Ken Kinder
 Author-email: ken+github@kkinder.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: textual[syntax] (>=0.52.1,<0.53.0)
+Requires-Dist: textual[syntax] (>=0.58.0,<0.59.0)
 Description-Content-Type: text/markdown
 
 # Modern but simple text editor
 
 Mehditor is a modern but simple text editor. I made it because I needed a quick editor (like Pico or Nano) on servers,
-but wanted a more modern and friendly itnerface. Meditor is written in Python and uses the excellent
+but wanted a more modern and friendly interface. Meditor is written in Python and uses the excellent
  [Textual](https://textual.textualize.io) for its user interface. I wrote it in a weekend.
 
 ![Mehditor screenshot showing application in terminal window](https://github.com/kkinder/mehditor/blob/main/screenshots/meh-1.png)
 
 ![Mehditor screenshot showing application in terminal window](https://github.com/kkinder/mehditor/blob/main/screenshots/meh-2.png)
 
 ![Mehditor screenshot showing application in terminal window](https://github.com/kkinder/mehditor/blob/main/screenshots/meh-3.png)
```

