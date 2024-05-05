# Comparing `tmp/pycolorecho-0.1.0-py3-none-any.whl.zip` & `tmp/pycolorecho-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 56619 bytes, number of entries: 7
--rw-r--r--  2.0 unx      549 b- defN 24-Apr-28 18:20 pycolorecho/__init__.py
--rw-r--r--  2.0 unx   327724 b- defN 24-Apr-28 18:20 pycolorecho/__main__.py
--rw-r--r--  2.0 unx     1069 b- defN 24-Apr-28 18:20 pycolorecho-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    17610 b- defN 24-Apr-28 18:20 pycolorecho-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-28 18:20 pycolorecho-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 24-Apr-28 18:20 pycolorecho-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      568 b- defN 24-Apr-28 18:20 pycolorecho-0.1.0.dist-info/RECORD
-7 files, 347624 bytes uncompressed, 55615 bytes compressed:  84.0%
+Zip file size: 57046 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      885 b- defN 24-May-05 06:12 pycolorecho/__init__.py
+-rw-r--r--  2.0 unx   329114 b- defN 24-May-05 06:12 pycolorecho/__main__.py
+-rw-r--r--  2.0 unx     1069 b- defN 24-May-05 06:12 pycolorecho-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    19925 b- defN 24-May-05 06:12 pycolorecho-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-05 06:12 pycolorecho-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-May-05 06:12 pycolorecho-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      568 b- defN 24-May-05 06:12 pycolorecho-0.1.1.dist-info/RECORD
+7 files, 351665 bytes uncompressed, 56042 bytes compressed:  84.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: pycolorecho/__init__.py
 Comment: 
 
 Filename: pycolorecho/__main__.py
 Comment: 
 
-Filename: pycolorecho-0.1.0.dist-info/LICENSE
+Filename: pycolorecho-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: pycolorecho-0.1.0.dist-info/METADATA
+Filename: pycolorecho-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: pycolorecho-0.1.0.dist-info/WHEEL
+Filename: pycolorecho-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: pycolorecho-0.1.0.dist-info/top_level.txt
+Filename: pycolorecho-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pycolorecho-0.1.0.dist-info/RECORD
+Filename: pycolorecho-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pycolorecho/__init__.py

```diff
@@ -4,22 +4,28 @@
     "Color",
     "TextBackgroundColor",
     "TextColor",
     "TextEffect",
     "TextCase",
     "ColorMapper",
     "echo",
+    "is_colorization_supported",
+    "is_true_color_supported",
+    "get_colorized_message",
+    "get_colorized_message_by_regex_pattern",
+    "get_colorized_message_by_mappings",
     "HEXCodes",
     "__author__",
     "__description__",
     "__name__",
     "__version__"
 ]
 __author__ = "coldsofttech"
 __description__ = """
 Simple Python package for colorized terminal output
 """
 __name__ = "pycolorecho"
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 from pycolorecho.__main__ import RESET, Layer, Color, TextBackgroundColor, TextColor, TextEffect, TextCase, \
-    ColorMapper, echo, HEXCodes
+    ColorMapper, echo, HEXCodes, is_colorization_supported, is_true_color_supported, get_colorized_message, \
+    get_colorized_message_by_regex_pattern, get_colorized_message_by_mappings
```

## pycolorecho/__main__.py

```diff
@@ -3,15 +3,15 @@
 import sys
 from enum import Enum
 from typing import Optional, Union
 
 RESET: str = "\033[0m"
 
 
-def _is_colorization_supported() -> bool:
+def is_colorization_supported() -> bool:
     """
     Checks if the current operating system supports colorization.
     :return: True if colorization is supported, False otherwise.
     :rtype: bool
     """
     file_name = 'lm_color.temp'
     # Check for Windows operating systems
@@ -37,15 +37,15 @@
         with open(file_name, 'r') as f:
             content = f.read()
             return '\033[1;31m' in content
     finally:
         os.remove(file_name)
 
 
-def _is_true_color_supported() -> bool:
+def is_true_color_supported() -> bool:
     """
     Verifies whether the true color format is supported by the current operating system and terminal.
     :return: True if true color format is supported, False otherwise.
     :rtype: bool
     """
     if os.name == 'nt':
         true_color_support = True
@@ -3143,15 +3143,15 @@
         :type true_color: bool
         """
         Validate.validate_type(name, str, 'name should be a string.')
         Validate.validate_type(ansi_code, str, 'ansi_code should be a string.')
         Validate.validate_type(true_color, bool, 'true_color should be a boolean.')
         Validate.validate_ansi(ansi_code)
 
-        if true_color and not _is_true_color_supported():
+        if true_color and not is_true_color_supported():
             raise Warning('True colors are not supported by this terminal.')
 
         code = ansi_code[2:].rstrip('m')
         if true_color:
             pattern = (
                 rf'^{Layer.Background.value};2;'
                 r'(?:0|1?\d{1,2}|2[0-4]\d|25[0-5]);'
@@ -5091,15 +5091,15 @@
         :type true_color: bool
         """
         Validate.validate_type(name, str, 'name should be a string.')
         Validate.validate_type(ansi_code, str, 'ansi_code should be a string.')
         Validate.validate_type(true_color, bool, 'true_color should be a boolean.')
         Validate.validate_ansi(ansi_code)
 
-        if true_color and not _is_true_color_supported():
+        if true_color and not is_true_color_supported():
             raise Warning('True colors are not supported by this terminal.')
 
         code = ansi_code[2:].rstrip('m')
         if true_color:
             pattern = (
                 rf'^{Layer.Foreground.value};2;'
                 r'(?:0|1?\d{1,2}|2[0-4]\d|25[0-5]);'
@@ -5665,15 +5665,15 @@
         f'{text_color if text_color is not None else ""}'
         f'{text_background_color if text_background_color is not None else ""}'
         f'{text_effect if text_effect is not None else ""}'
     )
     return colorize_sequence
 
 
-def _get_colorized_message(
+def get_colorized_message(
         message: str,
         text_color: Optional[str] = None,
         text_background_color: Optional[str] = None,
         text_effect: Optional[str] = None,
         text_case: Optional[int] = TextCase.NONE
 ) -> str:
     """
@@ -5687,28 +5687,34 @@
     :param text_effect: The ANSI effect code for the effect.
     :type text_effect:str
     :param text_case: The case to be applied for the text.
     :type text_case: str
     :return: The generated colorized message.
     :rtype: str
     """
+    Validate.validate_type(message, str, 'message should be a string.')
+    Validate.validate_type(text_color, Union[str, None], 'text_color should be a string.')
+    Validate.validate_type(text_background_color, Union[str, None], 'text_background_color should be a string.')
+    Validate.validate_type(text_effect, Union[str, None], 'text_effect should be a string.')
+    Validate.validate_type(text_case, Union[int, None], 'text_case should be an integer.')
+
     if text_color is None and text_background_color is None and text_effect is None:
         return f'{TextCase.convert_text(message, text_case)}'
 
     colorize_sequence = _get_colorize_sequence(text_color, text_background_color, text_effect)
     return (
         f'{colorize_sequence}'
         f'{TextCase.convert_text(message, text_case)}'
         f'{RESET if colorize_sequence is not None else ""}'
     )
 
 
-def _get_colorized_message_by_regex_pattern(
+def get_colorized_message_by_regex_pattern(
         message: str,
-        regex_pattern: Optional[str] = None,
+        regex_pattern: str,
         text_color: Optional[str] = None,
         text_background_color: Optional[str] = None,
         text_effect: Optional[str] = None,
         text_case: Optional[int] = TextCase.NONE,
         color_match: Optional[bool] = False,
         ignore_case: Optional[bool] = False
 ) -> str:
@@ -5731,14 +5737,23 @@
     :type color_match: bool
     :param ignore_case: Flag to ignore case while performing match. If True, ignores the case
     (case-insensitive) and matches the content, else case-sensitive match is performed.
     :type ignore_case: bool
     :return: The generated colorized message.
     :rtype: str
     """
+    Validate.validate_type(message, str, 'message should be a string.')
+    Validate.validate_type(regex_pattern, str, 'regex_pattern should be a string.')
+    Validate.validate_type(text_color, Union[str, None], 'text_color should be a string.')
+    Validate.validate_type(text_background_color, Union[str, None], 'text_background_color should be a string.')
+    Validate.validate_type(text_effect, Union[str, None], 'text_effect should be a string.')
+    Validate.validate_type(text_case, Union[int, None], 'text_case should be an integer.')
+    Validate.validate_type(color_match, Union[bool, None], 'color_match should be a boolean.')
+    Validate.validate_type(ignore_case, Union[bool, None], 'ignore_case should be a boolean.')
+
     colorized_message = message
     colorize_sequence = _get_colorize_sequence(text_color, text_background_color, text_effect)
 
     if ignore_case:
         if color_match:
             colorized_message = re.sub(
                 regex_pattern,
@@ -5775,27 +5790,30 @@
                     f'{TextCase.convert_text(colorized_message, text_case)}'
                     f'{RESET if colorize_sequence is not None else ""}'
                 )
 
     return colorized_message
 
 
-def _get_colorized_message_by_mappings(
+def get_colorized_message_by_mappings(
         message: str,
-        mappings: Optional[ColorMapper] = None
+        mappings: ColorMapper
 ) -> str:
     """
     Generates a colorized message based on the provided mappings.
     :param message: The message to be colorized.
     :type message: str
     :param mappings: The mappings utilized for verifying and colorizing the matched text.
     :type mappings: ColorMapper
     :return: The generated colorized message.
     :rtype: str
     """
+    Validate.validate_type(message, str, 'message should be a string.')
+    Validate.validate_type(mappings, ColorMapper, 'mappings should be of ColorMapper type.')
+
     colorized_message = message
     for key, value in mappings.get_mappings().items():
         keywords = value.get('keywords', [])
         color_mappings = value.get('color_mapping', {})
         flags = value.get('flags', {})
 
         for keyword_pattern in keywords:
@@ -5902,24 +5920,26 @@
 
     if mappings is None:
         Validate.validate_type(text_color, Union[str, None], 'text_color should be a string.')
         Validate.validate_type(text_background_color, Union[str, None], 'text_background_color should be a string.')
         Validate.validate_type(text_effect, Union[str, None], 'text_effect should be a string.')
         Validate.validate_type(text_case, Union[int, None], 'text_case should be an integer.')
 
+    Validate.validate_type(message, str, 'message should be a string.')
+
     colorized_message = message
 
-    if _is_colorization_supported():
+    if is_colorization_supported():
         if mappings is not None:
-            colorized_message = _get_colorized_message_by_mappings(colorized_message, mappings)
+            colorized_message = get_colorized_message_by_mappings(colorized_message, mappings)
         elif regex_pattern is not None:
-            colorized_message = _get_colorized_message_by_regex_pattern(
+            colorized_message = get_colorized_message_by_regex_pattern(
                 colorized_message, regex_pattern,
                 text_color, text_background_color, text_effect, text_case,
                 color_match, ignore_case
             )
         else:
-            colorized_message = _get_colorized_message(
+            colorized_message = get_colorized_message(
                 colorized_message, text_color, text_background_color, text_effect, text_case
             )
 
     print(colorized_message)
```

## Comparing `pycolorecho-0.1.0.dist-info/LICENSE` & `pycolorecho-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pycolorecho-0.1.0.dist-info/METADATA` & `pycolorecho-0.1.1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycolorecho
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple Python package for colorized terminal output
 Home-page: https://github.com/coldsofttech/pycolorecho
 Author: coldsofttech
 License: MIT
 Keywords: color,text-color,text-background-color,text-effect,text-case,terminal,colorization,style,text
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -93,14 +93,45 @@
 
 - `echo(message: str, regex_pattern: Optional[str] = None, mappings: Optional[ColorMapper] = None, text_color: Optional[str] = None, text_background_color: Optional[str] = None, text_effect: Optional[str] = None, text_case: Optional[int] = TextCase.NONE, color_match: Optional[bool] = False, ignore_case: Optional[bool] = False)` -
   Printstext colorized within the terminal based on the provided inputs. Supports the following scenarios:
     1) Colorizing a message by specifying text foreground color, text background color, text effect, and text case.
     2) Colorizing a message by matching it with a regex pattern and specifying text foreground color, text background
        color, text effect, text case, ignore case, and color match.
     3) Colorizing a message by matching it with mappings (utilizing a ColorMapper) and specifying text foreground.
+- `get_colorized_message(message: str, text_color: Optional[str] = None, text_background_color: Optional[str] = None, text_effect: Optional[str] = None, text_case: Optional[int] = TextCase.NONE) -> str` -
+  Generates a colorized message based on the provided inputs.
+- `get_colorized_message_by_regex_pattern(message: str, regex_pattern: str, text_color: Optional[str] = None, text_background_color: Optional[str] = None, text_effect: Optional[str] = None, text_case: Optional[int] = TextCase.NONE, color_match: Optional[bool] = False, ignore_case: Optional[bool] = False) -> str` -
+  Generates a colorized message based on the provided regex pattern and inputs.
+- `get_colorized_message_by_mappings(message: str, mappings: Optional[ColorMapper] = None) -> str` - Generates a
+  colorized message based on the provided mappings.
+- `is_colorization_supported() -> bool` - Checks if the current operating system supports colorization. Returns True if
+  colorization is supported, False otherwise.
+- `is_true_color_supported() -> bool` - Verifies whether the true color format is supported by the current operating
+  system and terminal. Returns True if true color format is supported, False otherwise.
+
+#### Usage
+
+```python
+from pycolorecho import is_colorization_supported, is_true_color_supported, get_colorized_message, get_colorized_message_by_regex_pattern, get_colorized_message_by_mappings, TextColor, TextBackgroundColor, TextEffect, ColorMapper
+
+print(is_colorization_supported())  # Prints True if colorization is supported, False otherwise
+print(is_true_color_supported())  # Prints True if true color format is supported, False otherwise
+
+# Retrieving colorized message
+print(get_colorized_message('This is a test message', text_color=TextColor.RED))
+
+# Retrieving colorized message by regex pattern
+print(get_colorized_message_by_regex_pattern('This is a test message', regex_pattern=r'test', text_color=TextColor.RED,
+                                             text_background_color=TextBackgroundColor.ACID_GREEN))
+
+# Retrieving colorized message by mappings
+color_mappings = ColorMapper()
+color_mappings.add_mapping('error', [r'error'], text_color=TextColor.RED, text_effect=TextEffect.UNDERLINE)
+print(get_colorized_message_by_mappings('This is a test error message', mappings=color_mappings))
+```
 
 ### Layer
 
 Supplies enum-based options for different color layers within a terminal, such as Foreground and Background.
 
 #### Options
```

