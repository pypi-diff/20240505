# Comparing `tmp/rofi_rbw-1.4.1.tar.gz` & `tmp/rofi_rbw-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rofi_rbw-1.4.1.tar", max compression
+gzip compressed data, was "rofi_rbw-1.4.2.tar", max compression
```

## Comparing `rofi_rbw-1.4.1.tar` & `rofi_rbw-1.4.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1075 2023-01-03 08:16:30.965044 rofi_rbw-1.4.1/LICENSE
--rw-r--r--   0        0        0     8619 2024-05-01 07:52:31.725921 rofi_rbw-1.4.1/README.md
--rw-r--r--   0        0        0     4528 2024-05-01 07:52:07.045951 rofi_rbw-1.4.1/docs/rofi-rbw.1
--rw-r--r--   0        0        0      748 2024-05-01 07:50:58.462700 rofi_rbw-1.4.1/pyproject.toml
--rw-r--r--   0        0        0      206 2022-12-22 13:31:28.675750 rofi_rbw-1.4.1/src/rofi_rbw/__init__.py
--rw-r--r--   0        0        0      105 2022-12-22 13:31:28.675750 rofi_rbw-1.4.1/src/rofi_rbw/__main__.py
--rw-r--r--   0        0        0      197 2022-12-22 13:31:28.675750 rofi_rbw-1.4.1/src/rofi_rbw/abstractionhelper.py
--rw-r--r--   0        0        0     4890 2024-04-19 16:55:25.616396 rofi_rbw-1.4.1/src/rofi_rbw/argument_parsing.py
--rw-r--r--   0        0        0     1182 2023-12-05 12:35:22.072945 rofi_rbw-1.4.1/src/rofi_rbw/cache.py
--rw-r--r--   0        0        0        0 2024-01-18 18:50:19.810170 rofi_rbw-1.4.1/src/rofi_rbw/clipboarder/__init__.py
--rw-r--r--   0        0        0     1194 2024-01-18 18:50:19.810170 rofi_rbw-1.4.1/src/rofi_rbw/clipboarder/clipboarder.py
--rw-r--r--   0        0        0      440 2024-01-18 18:50:32.079752 rofi_rbw-1.4.1/src/rofi_rbw/clipboarder/noop.py
--rw-r--r--   0        0        0      610 2024-01-18 18:50:37.116248 rofi_rbw-1.4.1/src/rofi_rbw/clipboarder/wlclip.py
--rw-r--r--   0        0        0     1106 2024-03-24 12:11:07.281774 rofi_rbw-1.4.1/src/rofi_rbw/clipboarder/xclip.py
--rw-r--r--   0        0        0     1210 2024-01-18 18:50:37.116248 rofi_rbw-1.4.1/src/rofi_rbw/clipboarder/xsel.py
--rw-r--r--   0        0        0     1592 2024-04-19 16:55:25.616396 rofi_rbw-1.4.1/src/rofi_rbw/credentials.py
--rw-r--r--   0        0        0      516 2023-12-05 12:35:22.072945 rofi_rbw-1.4.1/src/rofi_rbw/entry.py
--rw-r--r--   0        0        0     1473 2024-04-19 16:55:25.616396 rofi_rbw-1.4.1/src/rofi_rbw/models.py
--rw-r--r--   0        0        0      641 2023-12-05 12:35:22.072945 rofi_rbw-1.4.1/src/rofi_rbw/paths.py
--rw-r--r--   0        0        0     2512 2023-12-05 12:41:31.229807 rofi_rbw-1.4.1/src/rofi_rbw/rbw.py
--rwxr-xr-x   0        0        0     4442 2024-04-29 18:46:51.932565 rofi_rbw-1.4.1/src/rofi_rbw/rofi_rbw.py
--rw-r--r--   0        0        0        0 2024-01-18 18:50:19.810170 rofi_rbw-1.4.1/src/rofi_rbw/selector/__init__.py
--rw-r--r--   0        0        0     2506 2024-01-18 18:51:27.594529 rofi_rbw-1.4.1/src/rofi_rbw/selector/bemenu.py
--rw-r--r--   0        0        0     4627 2024-01-18 18:50:19.810170 rofi_rbw-1.4.1/src/rofi_rbw/selector/rofi.py
--rw-r--r--   0        0        0     3967 2024-03-21 18:01:21.271335 rofi_rbw-1.4.1/src/rofi_rbw/selector/selector.py
--rw-r--r--   0        0        0     2523 2024-01-18 18:50:19.810170 rofi_rbw-1.4.1/src/rofi_rbw/selector/wofi.py
--rw-r--r--   0        0        0        0 2024-01-18 18:50:19.810170 rofi_rbw-1.4.1/src/rofi_rbw/typer/__init__.py
--rw-r--r--   0        0        0      838 2024-04-19 16:55:25.616396 rofi_rbw-1.4.1/src/rofi_rbw/typer/dotool.py
--rw-r--r--   0        0        0      502 2024-04-19 16:55:25.616396 rofi_rbw-1.4.1/src/rofi_rbw/typer/noop.py
--rw-r--r--   0        0        0     1313 2024-04-19 16:55:25.616396 rofi_rbw-1.4.1/src/rofi_rbw/typer/typer.py
--rw-r--r--   0        0        0      800 2024-04-19 16:55:25.616396 rofi_rbw-1.4.1/src/rofi_rbw/typer/wtype.py
--rw-r--r--   0        0        0     1287 2024-04-29 18:46:51.932565 rofi_rbw-1.4.1/src/rofi_rbw/typer/xdotool.py
--rw-r--r--   0        0        0      861 2024-04-19 16:55:25.619729 rofi_rbw-1.4.1/src/rofi_rbw/typer/ydotool.py
--rw-r--r--   0        0        0     9361 1970-01-01 00:00:00.000000 rofi_rbw-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-01-03 08:16:30.965044 rofi_rbw-1.4.2/LICENSE
+-rw-r--r--   0        0        0     8619 2024-05-01 07:52:31.725921 rofi_rbw-1.4.2/README.md
+-rw-r--r--   0        0        0     4528 2024-05-05 07:41:25.060476 rofi_rbw-1.4.2/docs/rofi-rbw.1
+-rw-r--r--   0        0        0      748 2024-05-05 07:41:08.960464 rofi_rbw-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0      206 2022-12-22 13:31:28.675750 rofi_rbw-1.4.2/src/rofi_rbw/__init__.py
+-rw-r--r--   0        0        0      105 2022-12-22 13:31:28.675750 rofi_rbw-1.4.2/src/rofi_rbw/__main__.py
+-rw-r--r--   0        0        0      197 2022-12-22 13:31:28.675750 rofi_rbw-1.4.2/src/rofi_rbw/abstractionhelper.py
+-rw-r--r--   0        0        0     4890 2024-04-19 16:55:25.616396 rofi_rbw-1.4.2/src/rofi_rbw/argument_parsing.py
+-rw-r--r--   0        0        0     1182 2023-12-05 12:35:22.072945 rofi_rbw-1.4.2/src/rofi_rbw/cache.py
+-rw-r--r--   0        0        0        0 2024-01-18 18:50:19.810170 rofi_rbw-1.4.2/src/rofi_rbw/clipboarder/__init__.py
+-rw-r--r--   0        0        0     1194 2024-01-18 18:50:19.810170 rofi_rbw-1.4.2/src/rofi_rbw/clipboarder/clipboarder.py
+-rw-r--r--   0        0        0      440 2024-01-18 18:50:32.079752 rofi_rbw-1.4.2/src/rofi_rbw/clipboarder/noop.py
+-rw-r--r--   0        0        0      610 2024-01-18 18:50:37.116248 rofi_rbw-1.4.2/src/rofi_rbw/clipboarder/wlclip.py
+-rw-r--r--   0        0        0     1106 2024-03-24 12:11:07.281774 rofi_rbw-1.4.2/src/rofi_rbw/clipboarder/xclip.py
+-rw-r--r--   0        0        0     1210 2024-01-18 18:50:37.116248 rofi_rbw-1.4.2/src/rofi_rbw/clipboarder/xsel.py
+-rw-r--r--   0        0        0     1592 2024-04-19 16:55:25.616396 rofi_rbw-1.4.2/src/rofi_rbw/credentials.py
+-rw-r--r--   0        0        0      516 2023-12-05 12:35:22.072945 rofi_rbw-1.4.2/src/rofi_rbw/entry.py
+-rw-r--r--   0        0        0     1473 2024-04-19 16:55:25.616396 rofi_rbw-1.4.2/src/rofi_rbw/models.py
+-rw-r--r--   0        0        0      641 2023-12-05 12:35:22.072945 rofi_rbw-1.4.2/src/rofi_rbw/paths.py
+-rw-r--r--   0        0        0     2512 2023-12-05 12:41:31.229807 rofi_rbw-1.4.2/src/rofi_rbw/rbw.py
+-rwxr-xr-x   0        0        0     4442 2024-04-29 18:46:51.932565 rofi_rbw-1.4.2/src/rofi_rbw/rofi_rbw.py
+-rw-r--r--   0        0        0        0 2024-01-18 18:50:19.810170 rofi_rbw-1.4.2/src/rofi_rbw/selector/__init__.py
+-rw-r--r--   0        0        0     2506 2024-01-18 18:51:27.594529 rofi_rbw-1.4.2/src/rofi_rbw/selector/bemenu.py
+-rw-r--r--   0        0        0     4627 2024-01-18 18:50:19.810170 rofi_rbw-1.4.2/src/rofi_rbw/selector/rofi.py
+-rw-r--r--   0        0        0     3967 2024-03-21 18:01:21.271335 rofi_rbw-1.4.2/src/rofi_rbw/selector/selector.py
+-rw-r--r--   0        0        0     2523 2024-01-18 18:50:19.810170 rofi_rbw-1.4.2/src/rofi_rbw/selector/wofi.py
+-rw-r--r--   0        0        0        0 2024-01-18 18:50:19.810170 rofi_rbw-1.4.2/src/rofi_rbw/typer/__init__.py
+-rw-r--r--   0        0        0      838 2024-04-19 16:55:25.616396 rofi_rbw-1.4.2/src/rofi_rbw/typer/dotool.py
+-rw-r--r--   0        0        0      502 2024-04-19 16:55:25.616396 rofi_rbw-1.4.2/src/rofi_rbw/typer/noop.py
+-rw-r--r--   0        0        0     1313 2024-04-19 16:55:25.616396 rofi_rbw-1.4.2/src/rofi_rbw/typer/typer.py
+-rw-r--r--   0        0        0      895 2024-05-03 19:51:11.975344 rofi_rbw-1.4.2/src/rofi_rbw/typer/wtype.py
+-rw-r--r--   0        0        0     1287 2024-04-29 18:46:51.932565 rofi_rbw-1.4.2/src/rofi_rbw/typer/xdotool.py
+-rw-r--r--   0        0        0      861 2024-04-19 16:55:25.619729 rofi_rbw-1.4.2/src/rofi_rbw/typer/ydotool.py
+-rw-r--r--   0        0        0     9361 1970-01-01 00:00:00.000000 rofi_rbw-1.4.2/PKG-INFO
```

### Comparing `rofi_rbw-1.4.1/LICENSE` & `rofi_rbw-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.1/README.md` & `rofi_rbw-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.1/docs/rofi-rbw.1` & `rofi_rbw-1.4.2/docs/rofi-rbw.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Automatically generated by Pandoc 3.1.12.2
 .\"
-.TH "ROFI\-RBW" "1" "May 01, 2024" "Version 1.4.1" "Rofi Third\-party Add\-on Documentation"
+.TH "ROFI\-RBW" "1" "May 05, 2024" "Version 1.4.2" "Rofi Third\-party Add\-on Documentation"
 .SH NAME
 \f[B]rofi\-rbw\f[R] \- A rofi frontend for the alternative Bitwarden
 client rbw
 .SH SYNOPSIS
 .PP
 \f[B]rofi\-rbw\f[R] [\f[B]\-h\f[R]] [\f[B]\-\-version\f[R]]
 [\f[B]\-\-action\f[R] {\f[I]type\f[R],\f[I]copy\f[R],\f[I]print\f[R]}]
```

### Comparing `rofi_rbw-1.4.1/pyproject.toml` & `rofi_rbw-1.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rofi-rbw"
-version = "1.4.1"
+version = "1.4.2"
 description = "Rofi frontend for Bitwarden"
 authors = ["Fabian Winter <5821180+fdw@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/fdw/rofi-rbw"
 repository = "https://github.com/fdw/rofi-rbw"
 packages =[
```

### Comparing `rofi_rbw-1.4.1/src/rofi_rbw/argument_parsing.py` & `rofi_rbw-1.4.2/src/rofi_rbw/argument_parsing.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.1/src/rofi_rbw/cache.py` & `rofi_rbw-1.4.2/src/rofi_rbw/cache.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.1/src/rofi_rbw/clipboarder/clipboarder.py` & `rofi_rbw-1.4.2/src/rofi_rbw/clipboarder/clipboarder.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.1/src/rofi_rbw/clipboarder/wlclip.py` & `rofi_rbw-1.4.2/src/rofi_rbw/clipboarder/wlclip.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.1/src/rofi_rbw/clipboarder/xclip.py` & `rofi_rbw-1.4.2/src/rofi_rbw/clipboarder/xclip.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.1/src/rofi_rbw/clipboarder/xsel.py` & `rofi_rbw-1.4.2/src/rofi_rbw/clipboarder/xsel.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.1/src/rofi_rbw/credentials.py` & `rofi_rbw-1.4.2/src/rofi_rbw/credentials.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.1/src/rofi_rbw/entry.py` & `rofi_rbw-1.4.2/src/rofi_rbw/entry.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.1/src/rofi_rbw/models.py` & `rofi_rbw-1.4.2/src/rofi_rbw/models.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.1/src/rofi_rbw/paths.py` & `rofi_rbw-1.4.2/src/rofi_rbw/paths.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.1/src/rofi_rbw/rbw.py` & `rofi_rbw-1.4.2/src/rofi_rbw/rbw.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.1/src/rofi_rbw/rofi_rbw.py` & `rofi_rbw-1.4.2/src/rofi_rbw/rofi_rbw.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.1/src/rofi_rbw/selector/bemenu.py` & `rofi_rbw-1.4.2/src/rofi_rbw/selector/bemenu.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.1/src/rofi_rbw/selector/rofi.py` & `rofi_rbw-1.4.2/src/rofi_rbw/selector/rofi.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.1/src/rofi_rbw/selector/selector.py` & `rofi_rbw-1.4.2/src/rofi_rbw/selector/selector.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.1/src/rofi_rbw/selector/wofi.py` & `rofi_rbw-1.4.2/src/rofi_rbw/selector/wofi.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.1/src/rofi_rbw/typer/dotool.py` & `rofi_rbw-1.4.2/src/rofi_rbw/typer/dotool.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.1/src/rofi_rbw/typer/typer.py` & `rofi_rbw-1.4.2/src/rofi_rbw/typer/typer.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.1/src/rofi_rbw/typer/wtype.py` & `rofi_rbw-1.4.2/src/rofi_rbw/typer/wtype.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,21 @@
     def name() -> str:
         return "wtype"
 
     def get_active_window(self) -> str:
         return "not possible with wtype"
 
     def type_characters(self, characters: str, key_delay: int, active_window: str) -> None:
-        run(["wtype", "-d", str(key_delay), characters])
+        args = ['wtype']
+
+        if key_delay > 0:
+            args = args + ['-d', str(key_delay)]
+
+        args.append(characters)
+        run(args)
 
     def press_key(self, key: Key) -> None:
         if key == Key.ENTER:
             key_name = "return"
         elif key == Key.TAB:
             key_name = "tab"
         else:
```

### Comparing `rofi_rbw-1.4.1/src/rofi_rbw/typer/xdotool.py` & `rofi_rbw-1.4.2/src/rofi_rbw/typer/xdotool.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.1/src/rofi_rbw/typer/ydotool.py` & `rofi_rbw-1.4.2/src/rofi_rbw/typer/ydotool.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.1/PKG-INFO` & `rofi_rbw-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rofi-rbw
-Version: 1.4.1
+Version: 1.4.2
 Summary: Rofi frontend for Bitwarden
 Home-page: https://github.com/fdw/rofi-rbw
 License: MIT
 Author: Fabian Winter
 Author-email: 5821180+fdw@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

