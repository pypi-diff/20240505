# Comparing `tmp/pyloggermanager-0.1.3-py3-none-any.whl.zip` & `tmp/pyloggermanager-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,15 @@
-Zip file size: 41277 bytes, number of entries: 15
--rw-r--r--  2.0 unx     2329 b- defN 24-Apr-11 19:41 pyloggermanager/__init__.py
--rw-r--r--  2.0 unx    95596 b- defN 24-Apr-11 19:41 pyloggermanager/__main__.py
--rw-r--r--  2.0 unx     1287 b- defN 24-Apr-11 19:41 pyloggermanager/formatters/__init__.py
--rw-r--r--  2.0 unx    13717 b- defN 24-Apr-11 19:41 pyloggermanager/formatters/__main__.py
--rw-r--r--  2.0 unx     1200 b- defN 24-Apr-11 19:41 pyloggermanager/handlers/__init__.py
--rw-r--r--  2.0 unx    19044 b- defN 24-Apr-11 19:41 pyloggermanager/handlers/__main__.py
--rw-r--r--  2.0 unx     1321 b- defN 24-Apr-11 19:41 pyloggermanager/streams/__init__.py
--rw-r--r--  2.0 unx     3223 b- defN 24-Apr-11 19:41 pyloggermanager/streams/__main__.py
--rw-r--r--  2.0 unx     1108 b- defN 24-Apr-11 19:41 pyloggermanager/textstyles/__init__.py
--rw-r--r--  2.0 unx    11157 b- defN 24-Apr-11 19:41 pyloggermanager/textstyles/__main__.py
--rw-r--r--  2.0 unx     1069 b- defN 24-Apr-11 19:41 pyloggermanager-0.1.3.dist-info/LICENSE
--rw-r--r--  2.0 unx    54172 b- defN 24-Apr-11 19:41 pyloggermanager-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-11 19:41 pyloggermanager-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 24-Apr-11 19:41 pyloggermanager-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1349 b- defN 24-Apr-11 19:41 pyloggermanager-0.1.3.dist-info/RECORD
-15 files, 206680 bytes uncompressed, 39021 bytes compressed:  81.1%
+Zip file size: 35807 bytes, number of entries: 13
+-rw-r--r--  2.0 unx     2238 b- defN 24-May-05 09:18 pyloggermanager/__init__.py
+-rw-r--r--  2.0 unx    86923 b- defN 24-May-05 09:18 pyloggermanager/__main__.py
+-rw-r--r--  2.0 unx     1287 b- defN 24-May-05 09:18 pyloggermanager/formatters/__init__.py
+-rw-r--r--  2.0 unx    13717 b- defN 24-May-05 09:18 pyloggermanager/formatters/__main__.py
+-rw-r--r--  2.0 unx     1200 b- defN 24-May-05 09:18 pyloggermanager/handlers/__init__.py
+-rw-r--r--  2.0 unx    19281 b- defN 24-May-05 09:18 pyloggermanager/handlers/__main__.py
+-rw-r--r--  2.0 unx     1321 b- defN 24-May-05 09:18 pyloggermanager/streams/__init__.py
+-rw-r--r--  2.0 unx     3223 b- defN 24-May-05 09:18 pyloggermanager/streams/__main__.py
+-rw-r--r--  2.0 unx     1069 b- defN 24-May-05 09:18 pyloggermanager-0.1.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx    44916 b- defN 24-May-05 09:18 pyloggermanager-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-05 09:18 pyloggermanager-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 24-May-05 09:18 pyloggermanager-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1158 b- defN 24-May-05 09:18 pyloggermanager-0.1.4.dist-info/RECORD
+13 files, 176441 bytes uncompressed, 33855 bytes compressed:  80.8%
```

## zipnote {}

```diff
@@ -18,29 +18,23 @@
 
 Filename: pyloggermanager/streams/__init__.py
 Comment: 
 
 Filename: pyloggermanager/streams/__main__.py
 Comment: 
 
-Filename: pyloggermanager/textstyles/__init__.py
+Filename: pyloggermanager-0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: pyloggermanager/textstyles/__main__.py
+Filename: pyloggermanager-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: pyloggermanager-0.1.3.dist-info/LICENSE
+Filename: pyloggermanager-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: pyloggermanager-0.1.3.dist-info/METADATA
+Filename: pyloggermanager-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: pyloggermanager-0.1.3.dist-info/WHEEL
-Comment: 
-
-Filename: pyloggermanager-0.1.3.dist-info/top_level.txt
-Comment: 
-
-Filename: pyloggermanager-0.1.3.dist-info/RECORD
+Filename: pyloggermanager-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyloggermanager/__init__.py

```diff
@@ -1,10 +1,9 @@
 __all__ = [
     "CallerFrame",
-    "Colorization",
     "FileMode",
     "Lock",
     "LogLevel",
     "Record",
     "Logger",
     "Manager",
     "Registry",
@@ -18,15 +17,14 @@
     "warning",
     "log",
     "disable",
     "shutdown",
     "formatters",
     "handlers",
     "streams",
-    "textstyles",
     "__author__",
     "__description__",
     "__name__",
     "__version__"
 ]
 __author__ = "coldsofttech"
 __description__ = """
@@ -43,15 +41,14 @@
 
 Beyond technical capabilities, the pyloggermanager package contributes to the reliability and maintainability of Python
 applications. It establishes consistent logging practices, simplifying collaboration, code reviews, and issue
 resolution across development teams. Overall, the pyloggermanager package is an invaluable asset for developers aiming
 to implement robust logging solutions, ensuring efficient and resilient application performance.
 """
 __name__ = "pyloggermanager"
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 
 from pyloggermanager import formatters
 from pyloggermanager import handlers
 from pyloggermanager import streams
-from pyloggermanager import textstyles
-from pyloggermanager.__main__ import CallerFrame, Colorization, FileMode, Lock, LogLevel, Record, Logger, Manager, \
+from pyloggermanager.__main__ import CallerFrame, FileMode, Lock, LogLevel, Record, Logger, Manager, \
     Registry, RootLogger, load_config, get_logger, critical, debug, error, info, warning, log, disable, shutdown
```

## pyloggermanager/__main__.py

```diff
@@ -1,25 +1,23 @@
 import inspect
 import io
 import json
 import os
 import random
-import re
 import string
 import sys
 import threading
 import traceback
 from datetime import datetime
 from types import FrameType, TracebackType, NoneType
 from typing import Any, Optional, Tuple, Type, Union
 
 from pyloggermanager.formatters import Formatter, DefaultFormatter, DEFAULT_FORMAT, DATE_FORMAT
 from pyloggermanager.handlers import Handler, StderrHandler, FileHandler, StreamHandler
 from pyloggermanager.streams import Stream
-from pyloggermanager.textstyles import TextColor, TextBackgroundColor, TextEffect
 
 
 class CallerFrame:
     """
     This class represents caller details such as class name, file name, function name,
     module name, and path name based on the caller's frame information. It provides a
     method to retrieve caller details from a given frame.
@@ -61,238 +59,14 @@
                 break
 
             frame = frame.f_back
 
         return caller_frame
 
 
-class Colorization:
-    """
-    This class provides functionality to colorize messages based on specified
-    keywords and associated colorization options. It supports setting keyword-color
-    mappings, retrieving mappings, checking if colorization is supported, and
-    colorizing messages.
-    """
-
-    RESET: str = "\033[0m"  # Reset sequence to revert color and style changes
-
-    _KEYWORDS = 'keywords'
-    _COLORIZATION = 'colorization'
-    _TEXT_COLOR = 'text_color'
-    _TEXT_BACKGROUND_COLOR = 'text_background_color'
-    _TEXT_EFFECT = 'text_effect'
-
-    # Dictionary containing keyword-color mappings
-    _mappings = {}
-
-    @classmethod
-    def colorize_message(cls, message: str) -> str:
-        """
-        Colorizes the provided message based on keyword-color mappings.
-
-        :param message: The message to be colorized
-        :type message: str
-        :return: The colorized message
-        :rtype: str
-        """
-        if not isinstance(message, str):
-            raise TypeError('message should be a string.')
-
-        if not cls.is_colorization_supported() or not cls._mappings:
-            return message
-
-        colorized_message = message
-
-        for key, value in cls._mappings.items():
-            keywords = value.get(cls._KEYWORDS, [])
-            colorization = value.get(cls._COLORIZATION, {})
-
-            for keyword_pattern in keywords:
-                if re.search(keyword_pattern, message, re.IGNORECASE):
-                    text_color = colorization.get(cls._TEXT_COLOR, '')
-                    text_background_color = colorization.get(cls._TEXT_BACKGROUND_COLOR, '')
-                    text_effect = colorization.get(cls._TEXT_EFFECT, '')
-                    colorized_sequence = (
-                        f'{text_color if text_color is not None else ""}'
-                        f'{text_background_color if text_background_color is not None else ""}'
-                        f'{text_effect if text_effect is not None else ""}'
-                    )
-                    colorized_message = f'{colorized_sequence}{colorized_message}{cls.RESET}'
-
-        return colorized_message
-
-    @classmethod
-    def get_keyword_color_mapping(cls, name: str) -> dict:
-        """
-        Retrieves the colorization mapping for the specified keyword.
-
-        :param name: The name of the keyword
-        :type name: str
-        :return: The colorization mapping for the keyword
-        :rtype: dict
-        """
-        if not isinstance(name, str):
-            raise TypeError('name should be a string.')
-
-        result = cls._mappings.get(name.upper())
-        if result is None:
-            raise ValueError(f'Mapping "{name}" is not a valid value.')
-        return result
-
-    @classmethod
-    def get_keyword_color_mappings(cls) -> dict:
-        """
-        Retrieves all keyword-color mappings.
-
-        :return: All keyword-color mappings
-        :rtype: dict
-        """
-        return dict(sorted(cls._mappings.items()))
-
-    @classmethod
-    def is_colorization_supported(cls) -> bool:
-        """
-        Checks if colorization is supported based on the current environment.
-
-        :return: True if colorization is supported, False otherwise
-        :rtype: bool
-        """
-        file_name = 'lm_color.temp'
-        # Check for Windows operating systems
-        if sys.platform == 'win32':
-            major, minor = sys.getwindowsversion().major, sys.getwindowsversion().minor
-            return major > 10 or (major == 10 and minor >= 0)
-
-        # Check for Linux-based operating systems
-        term = os.environ.get('TERM')
-        if term is None:
-            return False
-
-        if 'color' in os.popen('tput colors').read():
-            return True
-
-        try:
-            with open(file_name, 'w') as f:
-                os.system('tput setaf 1', stdout=f, stderr=f)
-                os.system('tput setab 0', stdout=f, stderr=f)
-                os.system('echo -n "\033[1;31m"', stdout=f, stderr=f)
-                os.system('echo -n "\033[0m', stdout=f, stderr=f)
-
-            with open(file_name, 'r') as f:
-                content = f.read()
-                return '\033[1;31m' in content
-        finally:
-            os.remove(file_name)
-
-    @classmethod
-    def is_valid_mapping(cls, name: str) -> bool:
-        """
-        Checks if the specified keyword has a valid colorization mapping.
-
-        :param name: The name of the keyword
-        :type name: str
-        :return: True if the mapping is valid, False otherwise
-        :rtype: bool
-        """
-        if not isinstance(name, str):
-            raise TypeError('name should be a string.')
-
-        try:
-            return cls.get_keyword_color_mapping(name) is not None
-        except ValueError:
-            return False
-
-    @classmethod
-    def remove_keyword_color_mapping(cls, name: str) -> None:
-        """
-        Removes the colorization mapping for the specified keyword.
-
-        :param name: The name of the keyword to remove
-        :type name: str
-        :return: None
-        """
-        if not isinstance(name, str):
-            raise TypeError('name should be a string.')
-
-        name_upper = name.upper()
-        if name_upper in cls._mappings:
-            del cls._mappings[name_upper]
-        else:
-            raise ValueError(f'No mapping found for keyword "{name}".')
-
-    @classmethod
-    def set_keyword_color_mapping(
-            cls,
-            name: str,
-            keywords: str | list[str],
-            text_color: Optional[str] = None,
-            text_background_color: Optional[str] = None,
-            text_effect: Optional[str] = None
-    ) -> None:
-        """
-        Sets the colorization mapping for the specified keyword.
-
-        :param name: The name of the keyword
-        :type name: str
-        :param keywords: The keyword(s) to be associated with the mapping
-        :type keywords: str | list[str]
-        :param text_color: The text color for the mapping (optional)
-        :type text_color: str
-        :param text_background_color: The text background color for the mapping (optional)
-        :type text_background_color: str
-        :param text_effect: The text effect for the mapping (optional)
-        :type text_effect: str
-        :return: None
-        """
-        if not isinstance(name, str):
-            raise TypeError('name should be a string.')
-        elif not isinstance(text_color, Union[str, NoneType]):
-            raise TypeError('text_color should be a string.')
-        elif not isinstance(text_background_color, Union[str, NoneType]):
-            raise TypeError('text_background_color should be a string.')
-        elif not isinstance(text_effect, Union[str, NoneType]):
-            raise TypeError('text_effect should be a string.')
-
-        # Validate and process input values
-        for color, value in {
-            cls._TEXT_COLOR: text_color,
-            cls._TEXT_BACKGROUND_COLOR: text_background_color,
-            cls._TEXT_EFFECT: text_effect
-        }.items():
-            if value and color.startswith('text_col') and not TextColor.is_valid_color(value):
-                raise ValueError(f'TextColor "{value}" is an invalid value.')
-            elif value and color.startswith('text_bac') and not TextBackgroundColor.is_valid_color(value):
-                raise ValueError(f'TextBackgroundColor "{value}" is an invalid value.')
-            elif value and color.startswith('text_eff') and not TextEffect.is_valid_effect(value):
-                raise ValueError(f'TextEffect "{value}" is an invalid value.')
-
-        if not isinstance(keywords, (str, list)):
-            raise TypeError('Keywords should be either a string or list of strings.')
-        elif isinstance(keywords, list) and not all(isinstance(keyword, str) for keyword in keywords):
-            raise TypeError('Keywords should be either a string or list of strings.')
-
-        name_upper = name.upper()
-        if name_upper in cls._mappings:
-            cls._mappings[name_upper][cls._KEYWORDS] = [keywords] if isinstance(keywords, str) else keywords
-            cls._mappings[name_upper][cls._COLORIZATION] = {
-                cls._TEXT_COLOR: text_color,
-                cls._TEXT_BACKGROUND_COLOR: text_background_color,
-                cls._TEXT_EFFECT: text_effect
-            }
-        else:
-            cls._mappings[name_upper] = {
-                cls._KEYWORDS: [keywords] if isinstance(keywords, str) else keywords,
-                cls._COLORIZATION: {
-                    cls._TEXT_COLOR: text_color,
-                    cls._TEXT_BACKGROUND_COLOR: text_background_color,
-                    cls._TEXT_EFFECT: text_effect
-                }
-            }
-
-
 class FileMode:
     """
     This class represents file modes supported by the Python open() function
     for reading, writing, and appending to the files. It provides methods to retrieve
     default file mode, get the file mode mappings, check if a mode is valid, set
     default file mode, and get readable and writable modes.
     """
@@ -2357,15 +2131,15 @@
 
 def _create_default_handlers(
         file_name: str = None,
         file_mode: str = None,
         level: int = None,
         format_str: str = None,
         date_format: str = None,
-        colorization: Colorization = None,
+        colorization=None,
         stream: Stream = None,
         encoding: str = None
 ) -> list:
     """
     This method creates and returns a list containing the default handler for logging,
     either a FileHandler if file_name is specified, or a StreamHandler if file_name is None.
 
@@ -2376,33 +2150,35 @@
     :param level: The logging level for the handler.
     :type level: int
     :param format_str: The format string for formatting log messages.
     :type format_str: str
     :param date_format: The format string for formatting log message timestamps.
     :type date_format: str
     :param colorization: The colorization settings for log messages.
-    :type colorization: Colorization
+    :type colorization: pycolorecho.ColorMapper
     :param stream: The stream to log to, if not logging to a file.
     :type stream: Stream
     :param encoding: The encoding to use for the log file.
     :type encoding: str
     :return: A list containing the default handler configured based on the provided parameters.
     :rtype: list
     """
+    from pycolorecho import ColorMapper
+
     if not isinstance(file_name, Union[str, NoneType]):
         raise TypeError('file_name should be a string.')
     elif not isinstance(file_mode, Union[str, NoneType]):
         raise TypeError('file_mode should be a string.')
     elif not isinstance(level, Union[int, NoneType]):
         raise TypeError('level should be an integer.')
     elif not isinstance(format_str, Union[str, NoneType]):
         raise TypeError('format_str should be a string.')
     elif not isinstance(date_format, Union[str, NoneType]):
         raise TypeError('date_format should be a string.')
-    elif not isinstance(colorization, Union[Colorization, NoneType]):
+    elif not isinstance(colorization, Union[ColorMapper, NoneType]):
         raise TypeError('colorization should be of Colorization type.')
     elif not isinstance(encoding, Union[str, NoneType]):
         raise TypeError('encoding should be a string.')
 
     if stream:
         if not issubclass(type(stream), Stream):
             raise TypeError('stream should be a subclass of Stream class.')
@@ -2460,15 +2236,15 @@
         file_name: str = 'default.log',
         file_mode: str = FileMode.APPEND,
         level: int = LogLevel.INFO,
         format_str: str = DEFAULT_FORMAT,
         date_format: str = DATE_FORMAT,
         stream: Stream = None,
         handlers: list = None,
-        colorization: Colorization = None,
+        colorization=None,
         encoding: str = 'UTF-8'
 ) -> None:
     """
     This method loads the logging configuration based on the provided parameters.
     It acquires a lock for thread safety, configures default handlers if no handlers
     are specified, configures the formatter and level for each handler, and adds the
     handlers to the root logger. Finally, it releases the lock.
@@ -2484,32 +2260,34 @@
     :param date_format: The format string for formatting log message timestamps. Defaults to DATE_FORMAT.
     :type date_format: str
     :param stream: The stream to log to, if not logging to a file. Defaults to None.
     :type stream: Stream
     :param handlers: A list of handlers to configure. Defaults to None.
     :type handlers: list
     :param colorization: The colorization settings for log messages. Defaults to None.
-    :type colorization: Colorization
+    :type colorization: pycolorecho.ColorMapper
     :param encoding: The encoding to use for the log file. Defaults to 'UTF-8'.
     :type encoding: str
     :return: None
     """
+    from pycolorecho import ColorMapper
+
     if not isinstance(file_name, Union[str, NoneType]):
         raise TypeError('file_name should be a string.')
     elif not isinstance(file_mode, Union[str, NoneType]):
         raise TypeError('file_mode should be a string.')
     elif not isinstance(level, int):
         raise TypeError('level should be an integer.')
     elif not isinstance(format_str, str):
         raise TypeError('format_str should be a string.')
     elif not isinstance(date_format, str):
         raise TypeError('date_format should be a string.')
     elif not isinstance(handlers, Union[list, NoneType]):
         raise TypeError('handlers should be a list.')
-    elif not isinstance(colorization, Union[Colorization, NoneType]):
+    elif not isinstance(colorization, Union[ColorMapper, NoneType]):
         raise TypeError('colorization should be of Colorization type.')
     elif not isinstance(encoding, Union[str, NoneType]):
         raise TypeError('encoding should be a string.')
 
     if stream:
         if not issubclass(type(stream), Stream):
             raise TypeError('stream should be a subclass of Stream class.')
```

## pyloggermanager/handlers/__main__.py

```diff
@@ -31,24 +31,26 @@
         Initializes the handler with optional attributes.
 
         :param name: Handle name.
         :type name: str
         :param level: Handler log level.
         :type level: int
         :param colorization: Colorization object for the handler.
-        :type colorization: Colorization
+        :type colorization: pycolorecho.ColorMapper
         :param formatter: Formatter object for formatting log records.
         :type formatter: Formatter
         """
+        from pycolorecho import ColorMapper
+
         if not isinstance(name, Union[str, NoneType]):
             raise TypeError('name should be a string.')
         elif not isinstance(level, int):
             raise TypeError('level should be an integer.')
-        elif not isinstance(colorization, Union[pyloggermanager.Colorization, NoneType]):
-            raise TypeError('colorization should be of Colorization type.')
+        elif not isinstance(colorization, Union[ColorMapper, NoneType]):
+            raise TypeError('colorization should be of pycolorecho.ColorMapper type.')
         elif not issubclass(type(formatter), Formatter):
             raise TypeError('formatter should be subclass of Formatter.')
 
         self._name = name
         self._level = pyloggermanager.LogLevel.check_level(level)
         self._colorization = colorization
         self._formatter = formatter
@@ -70,16 +72,18 @@
     @colorization.setter
     def colorization(self, value) -> None:
         """
         Sets the colorization object for the handler.
 
         :param value: Colorization object for the handler.
         """
-        if not isinstance(value, Union[pyloggermanager.Colorization, NoneType]):
-            raise TypeError('colorization should be of Colorization type.')
+        from pycolorecho import ColorMapper
+
+        if not isinstance(value, Union[ColorMapper, NoneType]):
+            raise TypeError('colorization should be of pycolorecho.ColorMapper type.')
 
         self._colorization = value
 
     @property
     def formatter(self) -> Formatter:
         """
         Gets the formatter object for formatting log records.
@@ -250,15 +254,15 @@
         Initializes a ConsoleHandler instance.
 
         :param name: Handle name.
         :type name: str
         :param level: Handler log level.
         :type level: int
         :param colorization: Colorization object for the handler.
-        :type colorization: Colorization
+        :type colorization: pycolorecho.ColorMapper
         :param formatter: Formatter object for formatting log records.
         :type formatter: Formatter
         :param stream: Stream object for the handler.
         :type stream: Stream
         """
         if not issubclass(type(stream), Stream):
             raise TypeError('stream should be subclass of Stream.')
@@ -302,19 +306,20 @@
         Emits the log record by formatting it, colorizing the message, and writing it to the stream.
 
         :param record: Log record to emit.
         :type record: Record
         :param ignore_display: Flag to indicate if log message should be displayed on terminal.
         :type ignore_display: bool
         """
+        import pycolorecho
+
         formatted_record = self.format(record)
-        colored_message = (
-            self.colorization.colorize_message(formatted_record)
-            if self.colorization is not None else formatted_record
-        )
+        colored_message = pycolorecho.get_colorized_message_by_mappings(
+            formatted_record, mappings=self.colorization
+        ) if self.colorization else formatted_record
         self._stream.write(colored_message)
 
     def flush(self) -> None:
         """
         Flushes the stream if it has a flush method.
         """
         if hasattr(self._stream, 'flush'):
@@ -344,15 +349,15 @@
         Initializes a StreamHandler instance.
 
         :param name: Handle name.
         :type name: str
         :param level: Handler log level.
         :type level: int
         :param colorization: Colorization object for the handler.
-        :type colorization: Colorization
+        :type colorization: pycolorecho.ColorMapper
         :param formatter: Formatter object for formatting log records.
         :type formatter: Formatter
         :param stream: Stream object for the handler.
         :type stream: Stream
         """
         if not issubclass(type(stream), Stream):
             raise TypeError('stream should be subclass of Stream.')
@@ -401,23 +406,24 @@
         Emits a log record to the stream.
 
         :param record: Log record to emit.
         :type record: Record
         :param ignore_display: Flag to indicate if log message should be displayed on terminal.
         :type ignore_display: bool
         """
+        import pycolorecho
+
         formatted_record = self.format(record)
         self._stream.write(formatted_record + self.TERMINATOR)
         self.flush()
 
         if not ignore_display:
-            colored_message = (
-                self.colorization.colorize_message(formatted_record)
-                if self.colorization is not None else formatted_record
-            )
+            colored_message = pycolorecho.get_colorized_message_by_mappings(
+                formatted_record, mappings=self.colorization
+            ) if self.colorization else formatted_record
             print(colored_message)
 
     def flush(self) -> None:
         """
         Flushes the stream if it has a flush method.
         """
         self._acquire_lock()
@@ -451,15 +457,15 @@
         Initializes a FileHandler object.
 
         :param name: Handle name.
         :type name: str
         :param level: Handler log level.
         :type level: int | LogLevel
         :param colorization: Colorization object for the handler.
-        :type colorization: Colorization
+        :type colorization: pycolorecho.ColorMapper
         :param formatter: Formatter object for formatting log records.
         :type formatter: Formatter
         :param file_name: Name of the log file. Defaults to 'default.log'.
         :type file_name: str
         :param file_mode: File mode for opening the log file. Defaults to 'a'.
         :type file_mode: int | FileMode
         :param encoding: Encoding to be used for writing to the log file. Defaults to 'UTF-8'.
@@ -581,29 +587,30 @@
         Emits a log record by writing it to the log file.
 
         :param record: Log record to emit.
         :type record: Record
         :param ignore_display: Flag to indicate if log message should be displayed on terminal.
         :type ignore_display: bool
         """
+        import pycolorecho
+
         formatted_record = self.format(record)
         self._open_file_stream()
         self._acquire_lock()
         try:
             self._file_stream.write(formatted_record + self.TERMINATOR)
             self._file_stream.flush()
         finally:
             self._release_lock()
             self._close_file_stream()
 
         if not ignore_display:
-            colored_message = (
-                self.colorization.colorize_message(formatted_record)
-                if self.colorization is not None else formatted_record
-            )
+            colored_message = pycolorecho.get_colorized_message_by_mappings(
+                formatted_record, mappings=self.colorization
+            ) if self.colorization else formatted_record
             print(colored_message)
 
     def flush(self) -> None:
         """
         Flushes the file stream used for writing log records.
         """
         self._acquire_lock()
```

## Comparing `pyloggermanager-0.1.3.dist-info/LICENSE` & `pyloggermanager-0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyloggermanager-0.1.3.dist-info/METADATA` & `pyloggermanager-0.1.4.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyloggermanager
-Version: 0.1.3
+Version: 0.1.4
 Summary: The pyloggermanager package is a vital logging framework for Python applications, providing developers with essential
 Home-page: https://github.com/coldsofttech/pyloggermanager
 Author: coldsofttech
 License: MIT
 Keywords: logger,logging,logging-framework,logger-manager
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: Topic :: System :: Logging
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pycolorecho
 
 # `pyloggermanager`
 
 The 'pyloggermanager' package is a vital logging framework for Python applications, providing developers with essential
 tools to streamline logging operations. Its primary function is to simplify the recording and organization of log
 messages, including critical information, debugging messages, errors, and warnings. By offering a centralized interface
 and robust functionalities, the package facilitates efficient monitoring and troubleshooting processes.
@@ -139,58 +140,14 @@
 # Caller Class: Unknown Class
 # Caller File: example
 # Caller Function: test_function
 # Caller Module: example
 # Caller Path: /path/to/example.py
 ````
 
-### `Colorization`
-
-The Colorization class provides functionality to colorize messages based on specified keywords and associated
-colorization options. It supports setting keyword-color mappings, retrieving mappings, checking if colorization is
-supported, and colorizing messages.
-
-#### Attributes
-
-- `RESET`: Represents the reset sequence to revert color and style changes.
-
-#### Methods
-
-- `colorize_message(message: str) -> str`: Colorizes the provided message based on keyword-color mappings.
-- `get_keyword_color_mapping(name: str) -> dict`: Retrieves the colorization mapping for the specified keyword.
-- `get_keyword_color_mappings() -> dict`: Retrieves all keyword-color mappings.
-- `is_colorization_supported() -> bool`: Checks if colorization is supported based on the current environment.
-- `is_valid_mapping(name: str) -> bool`: Checks if the specified keyword has a valid colorization mapping.
-- `remove_keyword_color_mapping(name: str) -> None`: Removes the colorization mapping for the specified keyword.
-- `set_keyword_color_mapping(name: str, keywords: str | list[str], text_color: Optional[str] = None, text_background_color: Optional[str] = None, text_effect: Optional[str] = None) -> None`:
-  Sets the colorization mapping for the specified keyword.
-
-#### Usage
-
-````python
-# Import the Colorization class
-import pyloggermanager
-from pyloggermanager.textstyles import TextColor
-
-# Set up colorization mappings
-pyloggermanager.Colorization.set_keyword_color_mapping(
-    name='ERROR',
-    keywords=['error', 'exception'],
-    text_color=TextColor.RED
-)
-
-# Colorize a message
-message = 'An error occurred!'
-colorized_message = pyloggermanager.Colorization.colorize_message(message)
-print(colorized_message)
-
-# Output
-# An error occurred!
-````
-
 ### `FileMode`
 
 The FileMode class represents file modes supported by the Python open() function for reading, writing, and appending to
 files. It provides methods to retrieve the default file mode, get the file mode mappings, check if a mode is valid, set
 the default file mode, and get readable and writable modes.
 
 #### Constants
@@ -862,15 +819,15 @@
 - `colorization`: Gets or sets the colorization object for the handler.
 - `formatter`: Gets or sets the formatter object for formatting log records.
 - `level`: Gets or sets the log level for the handler.
 - `name`: Gets or sets the name of the handler.
 
 #### Methods
 
-- `__init__(name: str = None, level: int = 20, colorization: 'Colorization' = None, formatter: Formatter = DefaultFormatter())` -
+- `__init__(name: str = None, level: int = 20, colorization: pycolorecho.ColorMapper = None, formatter: Formatter = DefaultFormatter())` -
   Initializes the handler with optional attributes.
 - `close()`: Closes the handler.
 - `emit(record: 'Record', ignore_display: bool) -> None`: Abstract method to emit a log record.
 - `format(record: 'Record') -> str`: Formats a log record using the handler's formatter.
 - `flush()`: Flushes buffered records.
 - `get_handlers() -> list[Any]`: Retrieves a list of all handlers.
 - `handle(record: 'Record', ignore_display: bool) -> None`: Handles a log record.
@@ -900,15 +857,15 @@
 
 #### Properties
 
 - `stream`: Gets or sets the stream of the handler.
 
 #### Methods
 
-- `__init__(name: str = None, level: int = 20, colorization: 'Colorization' = None, formatter: Formatter = DefaultFormatter(), stream: Stream = TerminalStream())` -
+- `__init__(name: str = None, level: int = 20, colorization: pycolorecho.ColorMapper = None, formatter: Formatter = DefaultFormatter(), stream: Stream = TerminalStream())` -
   Initializes a ConsoleHandler instance with optional attributes
 - `close()`: Closes the stream if it has a close method.
 - `emit(record: 'Record', ignore_display: bool = True) -> None`: Emits the log record by formatting it, colorizing the
   message, and writing it to the stream.
 - `flush()`: Flushes the stream if it has a flush method.
 
 #### Usage
@@ -942,15 +899,15 @@
 
 #### Properties
 
 - `stream`: Gets or sets the stream of the handler.
 
 #### Methods
 
-- `__init__(name: str = None, level: int = 20, colorization: 'Colorization' = None, formatter: Formatter = DefaultFormatter(), stream: Stream = StdoutStream())` -
+- `__init__(name: str = None, level: int = 20, colorization: pycolorecho.ColorMapper = None, formatter: Formatter = DefaultFormatter(), stream: Stream = StdoutStream())` -
   Initializes a StreamHandler instance with optional attributes.
 - `close()`: Closes the stream if it has a close method.
 - `emit(record: 'Record', ignore_display: bool) -> None`: Emits a log record to the stream.
 - `flush()`: Flushes the stream if it has a flush method.
 
 #### Usage
 
@@ -985,15 +942,15 @@
 
 - `encoding`: Gets or sets the encoding of the handler.
 - `filemode`: Gets or sets the file mode for opening the file handler.
 - `filename`: Gets or sets the file name of the handler.
 
 #### Methods
 
-- `__init__(name: str = None, level: int = 20, colorization: 'Colorization' = None, formatter: Formatter = DefaultFormatter(), file_name: str = 'default.log', file_mode: str = 'a', encoding: str = 'UTF-8')` -
+- `__init__(name: str = None, level: int = 20, colorization: pycolorecho.ColorMapper = None, formatter: Formatter = DefaultFormatter(), file_name: str = 'default.log', file_mode: str = 'a', encoding: str = 'UTF-8')` -
   Initializes a FileHandler object with optional attributes.
 - `close()`: Closes the file stream used for writing log records.
 - `emit(record: 'Record', ignore_display: bool) -> None`: Emits a log record by writing it to the log file.
 - `flush()`: Flushes the file stream used for writing log records.
 
 #### Usage
 
@@ -1140,187 +1097,21 @@
 # Flush the terminal buffer (No operation required)
 terminal_stream.flush()
 
 # Output
 # This is a message to the terminal
 ````
 
-## `pyloggermanager.textstyles`
-
-The 'pyloggermanager.textstyles' package provides utilities for defining and applying text styles to log messages within
-the logger manager framework. It includes classes for specifying text colors, background colors, and text effects,
-allowing users to customize the appearance of log messages according to their preferences.
-
-This package is designed to enhance the visual representation of log messages by providing a flexible and intuitive way
-to apply various text styles. By incorporating these text styles into log messages, users can improve readability,
-emphasize important information, and differentiate between different types of log entries.
-
-Overall, the 'pyloggermanager.textstyles' package complements the logger manager framework by offering tools for
-creating visually appealing and informative log messages, contributing to a more effective logging experience.
-
-### TextBackgroundColor
-
-The TextBackgroundColor class represents text background color for styling console text. It provides methods to add
-custom colors, retrieve color mappings, get color codes, and check if a color is valid.
-
-#### Attributes
-
-| Color                                                            | Name            | Description                                   |
-|------------------------------------------------------------------|-----------------|-----------------------------------------------|
-| [![Black](https://via.placeholder.com/15x15/000000?text=+)](#)   | `BLACK` (str)   | Constant representing the black color code.   |
-| [![Red](https://via.placeholder.com/15x15/FF0000?text=+)](#)     | `RED` (str)     | Constant representing the red color code.     |
-| [![Green](https://via.placeholder.com/15x15/00FF00?text=+)](#)   | `GREEN` (str)   | Constant representing the green color code.   |
-| [![Yellow](https://via.placeholder.com/15x15/FFFF00?text=+)](#)  | `YELLOW` (str)  | Constant representing the yellow color code.  |
-| [![Blue](https://via.placeholder.com/15x15/0000FF?text=+)](#)    | `BLUE` (str)    | Constant representing the blue color code.    |
-| [![Magenta](https://via.placeholder.com/15x15/FF00FF?text=+)](#) | `MAGENTA` (str) | Constant representing the magenta color code. |
-| [![Cyan](https://via.placeholder.com/15x15/00FFFF?text=+)](#)    | `CYAN` (str)    | Constant representing the cyan color code.    |
-| [![White](https://via.placeholder.com/15x15/FFFFFF?text=+)](#)   | `WHITE` (str)   | Constant representing the white color code.   |
-
-#### Methods
-
-- `add_color(name: str, code: str) -> None`: Adds a custom color with the provided name and code.
-- `get_colors() -> dict`: Returns a dictionary mapping color names to their corresponding codes, sorted alphabetically.
-- `get_color(color_str: str) -> str`: Returns the color code for the provided color name or code string.
-- `is_valid_color(color: str) -> bool`: Checks if the provided color name or code is valid.
-- `remove_color(name: str) -> None`: Removes the color mapping for the specified color name.
-
-#### Usage
-
-````python
-from pyloggermanager.textstyles import TextBackgroundColor
-
-# Add a custom color
-TextBackgroundColor.add_color("CUSTOM_COLOR", "\033[48;5;200m")
-
-# Get color mappings
-color_mappings = TextBackgroundColor.get_colors()
-print(color_mappings)
-
-# Check if a color is valid
-is_valid = TextBackgroundColor.is_valid_color("YELLOW")
-print(is_valid)  # Output: True
-
-# Remove a color
-TextBackgroundColor.remove_color("CUSTOM_COLOR")
-
-# Output
-# {
-#     'BLACK': '\x1b[40m', 
-#     'BLUE': '\x1b[44m', 
-#     'CUSTOM_COLOR': '\x1b[48;5;200m', 
-#     'CYAN': '\x1b[46m', 
-#     'GREEN': '\x1b[42m', 
-#     'MAGENTA': '\x1b[45m', 
-#     'RED': '\x1b[41m', 
-#     'WHITE': '\x1b[47m', 
-#     'YELLOW': '\x1b[43m'
-# }
-````
-
-### TextColor
-
-The TextColor class represents text color for styling console text. It provides methods to add custom colors, retrieve
-color mappings, get color codes, and check if a color is valid.
-
-#### Attributes
-
-| Color                                                            | Name            | Description                                   |
-|------------------------------------------------------------------|-----------------|-----------------------------------------------|
-| [![Black](https://via.placeholder.com/15x15/000000?text=+)](#)   | `BLACK` (str)   | Constant representing the black color code.   |
-| [![Red](https://via.placeholder.com/15x15/FF0000?text=+)](#)     | `RED` (str)     | Constant representing the red color code.     |
-| [![Green](https://via.placeholder.com/15x15/00FF00?text=+)](#)   | `GREEN` (str)   | Constant representing the green color code.   |
-| [![Yellow](https://via.placeholder.com/15x15/FFFF00?text=+)](#)  | `YELLOW` (str)  | Constant representing the yellow color code.  |
-| [![Blue](https://via.placeholder.com/15x15/0000FF?text=+)](#)    | `BLUE` (str)    | Constant representing the blue color code.    |
-| [![Magenta](https://via.placeholder.com/15x15/FF00FF?text=+)](#) | `MAGENTA` (str) | Constant representing the magenta color code. |
-| [![Cyan](https://via.placeholder.com/15x15/00FFFF?text=+)](#)    | `CYAN` (str)    | Constant representing the cyan color code.    |
-| [![White](https://via.placeholder.com/15x15/FFFFFF?text=+)](#)   | `WHITE` (str)   | Constant representing the white color code.   |
-
-#### Methods
-
-- `add_color(name: str, code: str) -> None`: Adds a custom color with the provided name and code.
-- `get_colors() -> dict`: Returns a dictionary mapping color names to their corresponding codes, sorted alphabetically.
-- `get_color(color_str: str) -> str`: Returns the color code for the provided color name or code string.
-- `is_valid_color(color: str) -> bool`: Checks if the provided color name or code is valid.
-- `remove_color(name: str) -> None`: Removes the color mapping for the specified color name.
-
-#### Usage
-
-````python
-from pyloggermanager.textstyles import TextColor
-
-# Add a custom color
-TextColor.add_color("CUSTOM_COLOR", "\033[38;5;200m")
-
-# Get color mappings
-color_mappings = TextColor.get_colors()
-print(color_mappings)
-
-# Check if a color is valid
-is_valid = TextColor.is_valid_color("RED")
-print(is_valid)  # Output: True
-
-# Remove a color
-TextColor.remove_color("CUSTOM_COLOR")
-
-# Output
-# {
-#     'BLACK': '\x1b[30m', 
-#     'BLUE': '\x1b[34m',
-#     'CUSTOM_COLOR': '\x1b[38;5;200m',
-#     'CYAN': '\x1b[36m',
-#     'GREEN': '\x1b[32m', 
-#     'MAGENTA': '\x1b[35m',
-#     'RED': '\x1b[31m',
-#     'WHITE': '\x1b[37m', 
-#     'YELLOW': '\x1b[33m'
-# }
-````
-
-### TextEffect
+# Text Styles
 
-The TextEffect class represents different text effects used in text formatting, such as bold, underline, and italics. It
-provides methods to add custom text effects, get text effect mappings, check if a text effect is valid, and retrieve the
-corresponding text effect for a given string representation.
+For text colorization and styling, this package utilizes the `pycolorecho` package. You can find additional details
+about its usage and features by following this
+link: [pycolorecho](https://github.com/coldsofttech/pycolorecho/blob/main/README.md) package.
 
-#### Attributes
+# License
 
-- `BOLD` (str): Constant representing the bold text effect.
-- `UNDERLINE` (str): Constant representing the underline text effect.
-- `ITALIC` (str): Constant representing the italic text effect.
+Please refer to the [MIT license](LICENSE) within the project for more information.
 
-#### Methods
-
-- `add_effect(name: str, code: str) -> None`: Adds a custom text effect with the provided name and code.
-- `get_effects() -> dict`: Returns a dictionary mapping text effect names to their corresponding codes, sorted
-  alphabetically.
-- `get_effect(effect_str: str) -> str`: Returns the text effect name corresponding to the given text effect code or
-  name.
-- `is_valid_effect(effect: str) -> bool`: Checks if the provided text effect is valid.
-- `remove_effect(name: str) -> None`: Removes the text effect mapping for the specified effect name.
+# Contributing
 
-#### Usage
-
-````python
-from pyloggermanager.textstyles import TextEffect
-
-# Add a custom effect
-TextEffect.add_effect("CUSTOM_EFFECT", "\033[10m")
-
-# Get effect mappings
-effect_mappings = TextEffect.get_effects()
-print(effect_mappings)
-
-# Check if an effect is valid
-is_valid = TextEffect.is_valid_effect("BOLD")
-print(is_valid)  # Output: True
-
-# Remove an effect
-TextEffect.remove_effect("CUSTOM_EFFECT")
-
-# Output
-# {
-#     'BOLD': '\x1b[1m',
-#     'CUSTOM_EFFECT': '\x1b[10m', 
-#     'ITALIC': '\x1b[3m',
-#     'UNDERLINE': '\x1b[4m'
-# }
-````
+We welcome contributions from the community! Whether you have ideas for new features, bug fixes, or enhancements, feel
+free to open an issue or submit a pull request on [GitHub](https://github.com/coldsofttech/pyloggermanager).
```

## Comparing `pyloggermanager-0.1.3.dist-info/RECORD` & `pyloggermanager-0.1.4.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-pyloggermanager/__init__.py,sha256=fTVDlhD1hzJDBWK4OCHB01gOdWIl9xJ5r_2Jl_1hUrA,2329
-pyloggermanager/__main__.py,sha256=73f6GrAYEHIdbDhHrCAKssU05FhSPBpu9YOF-flIKNk,95596
+pyloggermanager/__init__.py,sha256=GI6iVRyrh0B81TIwHMaAbXsn2J7R-cz7aG7ZDIHn7aM,2238
+pyloggermanager/__main__.py,sha256=vXwmXNQHu9-yTBLhPxs1DY02XI6dI4UDGU4zL4ueBsY,86923
 pyloggermanager/formatters/__init__.py,sha256=L9GHzxkUHF_wkIIzNNYIFQnq2O1ngXQ672ynB1hR4aY,1287
 pyloggermanager/formatters/__main__.py,sha256=B8Y9O-hapXpkQPuO-_HzciTg7iGYceSKU_t3lXcAVK4,13717
 pyloggermanager/handlers/__init__.py,sha256=yuwSKoswuFsJuD1fTd-40kKFDpkGl_Kc2DI1K4iC31g,1200
-pyloggermanager/handlers/__main__.py,sha256=vkce1d7Aql1LJhN1Wv6HXizQg180m788eORBHXQT6PU,19044
+pyloggermanager/handlers/__main__.py,sha256=FhUVEQM5-sp-6H7xHHHENvrA4YzkwSLaqw0AGlqo9MU,19281
 pyloggermanager/streams/__init__.py,sha256=Iw_CSn7pWt0s76rw_GhGbgEL4acKSh_7u89BNJQoyuI,1321
 pyloggermanager/streams/__main__.py,sha256=SlYG1Vpj_oQiVPGz2rWQpNP20Lv_TlFQlTJ7-ZjRX98,3223
-pyloggermanager/textstyles/__init__.py,sha256=Ma1KEXhSF-7acEjuTKJDzYg1VZQwBuqm94YNyLf2lNQ,1108
-pyloggermanager/textstyles/__main__.py,sha256=1wbOl-ipaJZJfNuQPY9Rha-iLCBwQYJa9viIIN9GoLY,11157
-pyloggermanager-0.1.3.dist-info/LICENSE,sha256=QDd-5ssO5cRVguOaD889uNuqyZlNg2DQS6VjttE-8Dk,1069
-pyloggermanager-0.1.3.dist-info/METADATA,sha256=iY6Hp9MAbK0xx15skuB-Y7cAurJTZWDcOJHQN-4yBXA,54172
-pyloggermanager-0.1.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-pyloggermanager-0.1.3.dist-info/top_level.txt,sha256=427AjoG4-piQ3UJzKdLsUN7od0ylEYhotMppwna1-sQ,16
-pyloggermanager-0.1.3.dist-info/RECORD,,
+pyloggermanager-0.1.4.dist-info/LICENSE,sha256=QDd-5ssO5cRVguOaD889uNuqyZlNg2DQS6VjttE-8Dk,1069
+pyloggermanager-0.1.4.dist-info/METADATA,sha256=BZmoKvZY17ztlE9fVWLK088Cu5zMa7GZN0r2rR56vjI,44916
+pyloggermanager-0.1.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pyloggermanager-0.1.4.dist-info/top_level.txt,sha256=427AjoG4-piQ3UJzKdLsUN7od0ylEYhotMppwna1-sQ,16
+pyloggermanager-0.1.4.dist-info/RECORD,,
```

