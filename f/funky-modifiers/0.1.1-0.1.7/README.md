# Comparing `tmp/funky_modifiers-0.1.1.tar.gz` & `tmp/funky_modifiers-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funky_modifiers-0.1.1.tar", last modified: Sat Dec 23 18:06:53 2023, max compression
+gzip compressed data, was "funky_modifiers-0.1.7.tar", last modified: Sun May  5 21:37:34 2024, max compression
```

## Comparing `funky_modifiers-0.1.1.tar` & `funky_modifiers-0.1.7.tar`

### file list

```diff
@@ -1,34 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-12-23 18:06:53.812250 funky_modifiers-0.1.1/
--rw-rw-rw-   0        0        0     1525 2023-12-23 17:20:11.000000 funky_modifiers-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      421 2023-12-23 18:06:53.639102 funky_modifiers-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-12-23 13:32:31.000000 funky_modifiers-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-12-23 18:06:53.812250 funky_modifiers-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      563 2023-12-23 18:05:15.000000 funky_modifiers-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-23 18:06:53.437160 funky_modifiers-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-12-23 18:06:53.442664 funky_modifiers-0.1.1/src/funk_py/
--rw-rw-rw-   0        0        0        0 2023-12-23 16:24:57.000000 funky_modifiers-0.1.1/src/funk_py/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-23 18:06:53.477155 funky_modifiers-0.1.1/src/funk_py/modularity/
--rw-rw-rw-   0        0        0        0 2023-12-23 13:32:31.000000 funky_modifiers-0.1.1/src/funk_py/modularity/__init__.py
--rw-rw-rw-   0        0        0      661 2023-12-23 13:32:31.000000 funky_modifiers-0.1.1/src/funk_py/modularity/basic_structures.py
--rw-rw-rw-   0        0        0     3074 2023-12-23 13:32:31.000000 funky_modifiers-0.1.1/src/funk_py/modularity/bespoke_properties.py
-drwxrwxrwx   0        0        0        0 2023-12-23 18:06:53.504428 funky_modifiers-0.1.1/src/funk_py/modularity/decoration/
--rw-rw-rw-   0        0        0      107 2023-12-23 13:32:31.000000 funky_modifiers-0.1.1/src/funk_py/modularity/decoration/__init__.py
--rw-rw-rw-   0        0        0     9073 2023-12-23 13:32:31.000000 funky_modifiers-0.1.1/src/funk_py/modularity/decoration/init_modifiers.py
--rw-rw-rw-   0        0        0     2749 2023-12-23 13:32:31.000000 funky_modifiers-0.1.1/src/funk_py/modularity/decoration/transforming_list.py
--rw-rw-rw-   0        0        0     6365 2023-12-23 13:32:31.000000 funky_modifiers-0.1.1/src/funk_py/modularity/logging.py
--rw-rw-rw-   0        0        0    15548 2023-12-23 13:32:31.000000 funky_modifiers-0.1.1/src/funk_py/modularity/type_matching.py
-drwxrwxrwx   0        0        0        0 2023-12-23 18:06:53.573847 funky_modifiers-0.1.1/src/funk_py/super_dicts/
--rw-rw-rw-   0        0        0      581 2023-12-23 13:32:31.000000 funky_modifiers-0.1.1/src/funk_py/super_dicts/__init__.py
--rw-rw-rw-   0        0        0     8880 2023-12-23 13:32:31.000000 funky_modifiers-0.1.1/src/funk_py/super_dicts/drop_none_dict.py
--rw-rw-rw-   0        0        0     9089 2023-12-23 13:32:31.000000 funky_modifiers-0.1.1/src/funk_py/super_dicts/list_dict.py
--rw-rw-rw-   0        0        0    14753 2023-12-23 13:32:31.000000 funky_modifiers-0.1.1/src/funk_py/super_dicts/multi_key_dict.py
--rw-rw-rw-   0        0        0     5248 2023-12-23 13:32:31.000000 funky_modifiers-0.1.1/src/funk_py/super_dicts/multi_value_dict.py
--rw-rw-rw-   0        0        0     3549 2023-12-23 13:32:31.000000 funky_modifiers-0.1.1/src/funk_py/super_dicts/windowed_list.py
-drwxrwxrwx   0        0        0        0 2023-12-23 18:06:53.600628 funky_modifiers-0.1.1/src/funky_modifiers.egg-info/
--rw-rw-rw-   0        0        0      421 2023-12-23 18:06:53.000000 funky_modifiers-0.1.1/src/funky_modifiers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      865 2023-12-23 18:06:53.000000 funky_modifiers-0.1.1/src/funky_modifiers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-23 18:06:53.000000 funky_modifiers-0.1.1/src/funky_modifiers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-12-23 18:06:53.000000 funky_modifiers-0.1.1/src/funky_modifiers.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-12-23 18:06:53.608585 funky_modifiers-0.1.1/test/
--rw-rw-rw-   0        0        0     4840 2023-12-23 13:32:31.000000 funky_modifiers-0.1.1/test/test_drop_none_dict.py
--rw-rw-rw-   0        0        0    11169 2023-12-23 13:32:31.000000 funky_modifiers-0.1.1/test/test_logs_vars.py
+drwxrwxrwx   0        0        0        0 2024-05-05 21:37:33.999837 funky_modifiers-0.1.7/
+-rw-rw-rw-   0        0        0     1525 2024-02-25 05:24:52.000000 funky_modifiers-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0       37 2024-05-05 20:43:12.000000 funky_modifiers-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      474 2024-05-05 21:37:33.998845 funky_modifiers-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      131 2024-05-05 19:24:08.000000 funky_modifiers-0.1.7/README.md
+-rw-rw-rw-   0        0        0       13 2024-05-05 21:32:06.000000 funky_modifiers-0.1.7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-05 21:37:33.999837 funky_modifiers-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      711 2024-05-05 21:37:27.000000 funky_modifiers-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 21:37:33.967595 funky_modifiers-0.1.7/src/
+drwxrwxrwx   0        0        0        0 2024-05-05 21:37:33.972060 funky_modifiers-0.1.7/src/funk_py/
+-rw-rw-rw-   0        0        0       50 2023-12-27 12:08:10.000000 funky_modifiers-0.1.7/src/funk_py/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 21:37:33.975528 funky_modifiers-0.1.7/src/funk_py/modularity/
+-rw-rw-rw-   0        0        0        0 2023-12-26 12:23:31.000000 funky_modifiers-0.1.7/src/funk_py/modularity/__init__.py
+-rw-rw-rw-   0        0        0    39190 2024-05-05 15:25:24.000000 funky_modifiers-0.1.7/src/funk_py/modularity/basic_structures.py
+-rw-rw-rw-   0        0        0     4500 2024-05-03 11:21:07.000000 funky_modifiers-0.1.7/src/funk_py/modularity/bespoke_properties.py
+drwxrwxrwx   0        0        0        0 2024-05-05 21:37:33.978009 funky_modifiers-0.1.7/src/funk_py/modularity/decoration/
+-rw-rw-rw-   0        0        0      496 2024-02-24 19:47:42.000000 funky_modifiers-0.1.7/src/funk_py/modularity/decoration/__init__.py
+-rw-rw-rw-   0        0        0     1260 2024-04-24 10:42:19.000000 funky_modifiers-0.1.7/src/funk_py/modularity/decoration/enum_modifiers.py
+-rw-rw-rw-   0        0        0     9073 2024-02-25 05:13:05.000000 funky_modifiers-0.1.7/src/funk_py/modularity/decoration/init_modifiers.py
+-rw-rw-rw-   0        0        0     2749 2023-12-26 12:23:31.000000 funky_modifiers-0.1.7/src/funk_py/modularity/decoration/transforming_list.py
+-rw-rw-rw-   0        0        0     6475 2024-02-25 05:13:05.000000 funky_modifiers-0.1.7/src/funk_py/modularity/logging.py
+-rw-rw-rw-   0        0        0    34949 2024-05-02 10:31:37.000000 funky_modifiers-0.1.7/src/funk_py/modularity/type_matching.py
+drwxrwxrwx   0        0        0        0 2024-05-05 21:37:33.980494 funky_modifiers-0.1.7/src/funk_py/sorting/
+-rw-rw-rw-   0        0        0        0 2024-04-07 16:23:56.000000 funky_modifiers-0.1.7/src/funk_py/sorting/__init__.py
+-rw-rw-rw-   0        0        0    20021 2024-05-05 16:10:17.000000 funky_modifiers-0.1.7/src/funk_py/sorting/converters.py
+-rw-rw-rw-   0        0        0    18997 2024-05-05 11:30:10.000000 funky_modifiers-0.1.7/src/funk_py/sorting/dict_manip.py
+-rw-rw-rw-   0        0        0    14818 2024-05-04 18:39:41.000000 funky_modifiers-0.1.7/src/funk_py/sorting/pieces.py
+drwxrwxrwx   0        0        0        0 2024-05-05 21:37:33.982967 funky_modifiers-0.1.7/src/funk_py/super_dicts/
+-rw-rw-rw-   0        0        0     2139 2024-05-05 18:39:34.000000 funky_modifiers-0.1.7/src/funk_py/super_dicts/__init__.py
+-rw-rw-rw-   0        0        0     8330 2024-03-03 18:51:02.000000 funky_modifiers-0.1.7/src/funk_py/super_dicts/drop_none_dict.py
+-rw-rw-rw-   0        0        0     8942 2024-03-03 17:19:44.000000 funky_modifiers-0.1.7/src/funk_py/super_dicts/list_dict.py
+-rw-rw-rw-   0        0        0     3583 2023-12-30 12:27:19.000000 funky_modifiers-0.1.7/src/funk_py/super_dicts/windowed_list.py
+drwxrwxrwx   0        0        0        0 2024-05-05 21:37:33.998343 funky_modifiers-0.1.7/src/funky_modifiers.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-05 21:37:33.000000 funky_modifiers-0.1.7/src/funky_modifiers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1259 2024-05-05 21:37:33.000000 funky_modifiers-0.1.7/src/funky_modifiers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 21:37:33.000000 funky_modifiers-0.1.7/src/funky_modifiers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-05 21:37:33.000000 funky_modifiers-0.1.7/src/funky_modifiers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-05 21:37:33.000000 funky_modifiers-0.1.7/src/funky_modifiers.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-05 21:37:33.997853 funky_modifiers-0.1.7/test/
+-rw-rw-rw-   0        0        0    21040 2024-05-03 11:33:03.000000 funky_modifiers-0.1.7/test/test_check_dict_equality.py
+-rw-rw-rw-   0        0        0    27490 2024-05-03 11:33:03.000000 funky_modifiers-0.1.7/test/test_check_list_equality.py
+-rw-rw-rw-   0        0        0    21911 2024-04-27 15:34:29.000000 funky_modifiers-0.1.7/test/test_convert_tuplish_dict.py
+-rw-rw-rw-   0        0        0    15212 2024-05-05 16:22:23.000000 funky_modifiers-0.1.7/test/test_converters.py
+-rw-rw-rw-   0        0        0     3127 2024-04-24 10:25:16.000000 funky_modifiers-0.1.7/test/test_converts_enums.py
+-rw-rw-rw-   0        0        0    12426 2024-03-03 19:25:27.000000 funky_modifiers-0.1.7/test/test_drop_none_dict.py
+-rw-rw-rw-   0        0        0    26544 2024-03-03 19:25:27.000000 funky_modifiers-0.1.7/test/test_function_hash_and_equality.py
+-rw-rw-rw-   0        0        0    12013 2024-04-12 20:31:58.000000 funky_modifiers-0.1.7/test/test_logs_vars.py
+-rw-rw-rw-   0        0        0    35329 2024-05-02 11:24:45.000000 funky_modifiers-0.1.7/test/test_obj.py
+-rw-rw-rw-   0        0        0    68867 2024-05-05 18:36:38.000000 funky_modifiers-0.1.7/test/test_pick.py
```

### Comparing `funky_modifiers-0.1.1/LICENSE` & `funky_modifiers-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.1/setup.py` & `funky_modifiers-0.1.7/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from setuptools import setup, find_packages
 
+with open("requirements.txt", "r") as fh:
+    install_requires = fh.read()
 
 setup(
     name='funky_modifiers',
-    version='0.1.1',
+    version='0.1.7',
     description='A package containing tiny bits and bobs to remove boilerplate or just make things simpler.',
     url='https://github.com/Sparqzi/funk_py',
-    author='Sparqzi',
+    author='Erich Kopp',
     license='BSD 3-Clause',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     classifiers=[
         'Development Status :: 1 - Planning',
         'Operating System :: POSIX :: Linux',
-        'Programming Language :: Python :: 3.10'
-    ]
+        'Programming Language :: Python :: 3.7'
+    ],
+    python_requires='>3.6',
+    install_requires=install_requires
 )
```

### Comparing `funky_modifiers-0.1.1/src/funk_py/modularity/decoration/init_modifiers.py` & `funky_modifiers-0.1.7/src/funk_py/modularity/decoration/init_modifiers.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.1/src/funk_py/modularity/decoration/transforming_list.py` & `funky_modifiers-0.1.7/src/funk_py/modularity/decoration/transforming_list.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.1/src/funk_py/modularity/logging.py` & `funky_modifiers-0.1.7/src/funk_py/modularity/logging.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,35 +15,42 @@
 
 
 def make_logger(name: str, /, env_var: str = 'LOG_LEVEL', *,
                 log_to_file: str = None,
                 default_level: Union[str, int] = logging.INFO,
                 show_function: bool = False,
                 **custom_levels: int) -> logging.Logger:
-    r"""
+    """
     This creates a logger with a few default settings as well as some custom
     levels, if specified. The format of messages for this logger should be
-    '
+    ``'{levelname}: {name} - {message}'``
 
     :param name: The name of the logger.
     :param env_var: The environment variable it should be linked to.
     :param log_to_file: If this is specified, it should be the full file name
         for the logger to log to.
     :param default_level: This may be either a str or an int representing the
         desired log level.
         `per python docs <https://docs.python.org/3/library/logging.html#levels>`__,
-        the default available levels are: logging.notset = 0,
-        logging.debug = 10, logging.info = 20, logging.warning = 30,
-        logging.error = 40, and logging.CRITICAL = 50.
+        the default available levels are:
+
+        .. code-block:: python
+
+            logging.NOTSET = 0
+            logging.DEBUG = 10
+            logging.INFO = 20
+            logging.WARNING = 30
+            logging.ERROR = 40
+            logging.CRITICAL = 50
+
     :param show_function: Whether you want the function name that is being
         logged from to show up in the info.
     :param custom_levels: *Please note that this is global. If you define it for
         one logger, it exists for all loggers. Those loggers may not be set up
         to use it by default, though.*
-    :return:
     """
     logger = logging.getLogger(name)
 
     max_length = 8
 
     if len(custom_levels):
         for levelname, value in custom_levels.items():
@@ -54,15 +61,15 @@
                 max_length = t
 
     level = getenv(env_var, default_level)
     logger.setLevel(level if type(level) is int else level.upper())
 
     format_str = '%(levelname)-' + str(max_length) + 's: %(name)s - '
     if show_function:
-        format_str += '%funcName)s - %(message)s'
+        format_str += '%(funcName)s - %(message)s'
         formatter = logging.Formatter(format_str)
 
     else:
         format_str += '%(message)s'
         formatter = logging.Formatter(format_str)
 
     primary_handler = logging.StreamHandler(sys.stdout)
```

### Comparing `funky_modifiers-0.1.1/src/funk_py/super_dicts/drop_none_dict.py` & `funky_modifiers-0.1.7/src/funk_py/super_dicts/drop_none_dict.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, Union, Callable, Mapping
 
-from super_dicts import main_logger
-from modularity.logging import logs_vars
+from funk_py.super_dicts import main_logger
+from funk_py.modularity.logging import logs_vars
 
 
 class DropNoneDict(dict):
     class _NoneIfLater:
         @logs_vars(main_logger, 'i_self',
                    start_message='Creating new DropNoneDict._NoneIfLater...',
                    end_message='Created new DropNoneDict._NoneIfLater.',
@@ -14,145 +14,129 @@
                      plug_out: str = ...):
             i_self.value = value
             i_self.none_val = none_val
             i_self.plug_in = plug_in
             i_self.plug_out = plug_out
 
         @logs_vars(main_logger, 'i_self',
-                   start_message='Attempting to calculate result of'
-                                 ' DropNoneDict._NoneIfLater...')
+                   start_message='Attempting to calculate result of DropNoneDict._NoneIfLater...')
         def __call__(i_self, self) -> Any:
             main_logger.debug(f'Applied To: {self}')
             return DropNoneDict.none_if(self, i_self.value, i_self.none_val,
                                         plug_in=i_self.plug_in,
                                         plug_out=i_self.plug_out)
 
-    @logs_vars(main_logger, start_message='Calling DropNoneDict.none_if...')
-    def none_if(self, value: Any, none_val: Any = ..., *,
-                plug_in: Callable = ..., plug_out: str = ...) -> Any:
+    @logs_vars(main_logger,
+               start_message='Calling DropNoneDict.none_if...')
+    def none_if(self, value: Any, none_val: Any = ..., *, plug_in: Callable = ...,
+                plug_out: str = ...) -> Any:
         """
-        Changes a value to the correct "None" value of the containing dict if
-        it meets specified criteria.
+        Changes a value to the correct "None" value of the containing dict if it meets specified
+            criteria.
 
         :param value: The value that is being tested.
         :param none_val: The value that should also be "None".
-        :param plug_in: A function that should be enacted on the value if it
-            is not "None".
-        :param plug_out: A function of the value, which should be called
-            (without arguments) and the result of which should be returned
-            if the value is not "None".
+        :param plug_in: A function that should be enacted on the value if it is not "None".
+        :param plug_out: A function of the value, which should be called (without arguments) and the
+            result of which should be returned if the value is not "None".
         """
         if type(self) is not DropNoneDict:
-            # The below starts with self because of a messy situation which
-            # occurs when none_if is used in a dictionary that isn't yet
-            # constructed.
-            main_logger.trace(f'none_if is not being called on a DropNoneDict'
-                              f' instance, generating a'
-                              f' DropNoneDict._NoneIfLater...')
+            # The below starts with self because of a messy situation which occurs when none_if is
+            # used in a dictionary that isn't yet constructed.
+            main_logger.trace('none_if is not being called on a DropNoneDict instance, generating '
+                              'a DropNoneDict._NoneIfLater...')
             return DropNoneDict._NoneIfLater(self, value, plug_in=plug_in,
                                              plug_out=plug_out)
 
         if value == none_val:
             main_logger.trace(f'value is equal to none_val. Returning'
                               f' _none_condition ({self._none_condition})...')
             return self._none_condition
 
         elif plug_in is not ...:
-            main_logger.trace('plug_in is present, attempting plug_in with'
-                              ' value...')
+            main_logger.trace('plug_in is present, attempting plug_in with value...')
             try:
                 output = plug_in(value)
 
             except Exception:
-                main_logger.error(f'plug_in was attempted in none_if, but'
-                                  f' plugging {value} into {plug_in} raised an'
-                                  f' exception.')
+                main_logger.error(f'plug_in was attempted in none_if, but plugging {value} into '
+                                  f'{plug_in} raised an exception.')
                 raise
 
             main_logger.trace('Returning result...')
             return output
 
         elif plug_out is not ...:
-            main_logger.trace('plug_out is present, attempting plug_out on'
-                              ' value...')
+            main_logger.trace('plug_out is present, attempting plug_out on value...')
             try:
                 output = getattr(value, plug_out)()
 
             except AttributeError:
-                main_logger.error(f'plug_out was attempted in none_if, but'
-                                  f' {value} did not have the attribute'
-                                  f' {plug_out}')
+                main_logger.error(f'plug_out was attempted in none_if, but {value} did not have '
+                                  f'the attribute {plug_out}')
                 raise
 
             main_logger.trace('Returning result...')
             return output
 
-        main_logger.trace('value should not be equated to None, returning'
-                          ' value...')
+        main_logger.trace('value should not be equated to None, returning value...')
         return value
 
     def __set_check_func(self):
-        """Sets the check_func that the DropNoneDict will use to check if
-        values belong."""
+        """Sets the check_func that the DropNoneDict will use to check if values belong."""
         main_logger.debug('Setting the check_func for a DropNoneDict...')
         check_val = self._none_condition
         main_logger.debug(f'check_val = {check_val}')
         if check_val in [None, ..., True, False] or callable(check_val):
-            main_logger.trace('Since check_val is in [None, ..., True, False],'
-                              ' the check should be for the same item...')
-            main_logger.trace('Setting _check_func to -'
-                              ' lambda x: x is not check_val')
+            main_logger.trace('Since check_val is in [None, ..., True, False], the check should be '
+                              'for the same item...')
+            main_logger.trace('Setting _check_func to - lambda x: x is not check_val')
             self._check_func = lambda x: x is not check_val
 
         else:
-            main_logger.trace('Since check_val is not in [None, ..., True,'
-                              ' False], the check should be for value only...')
-            main_logger.trace('Setting _check_func to -'
-                              ' lambda x: x != check_val')
+            main_logger.trace('Since check_val is not in [None, ..., True, False], the check '
+                              'should be for value only...')
+            main_logger.trace('Setting _check_func to - lambda x: x != check_val')
             self._check_func = lambda x: x != check_val
 
         main_logger.debug('Done setting check_func for DropNoneDict.')
 
-    @logs_vars(main_logger, start_message='Creating a new DropNoneDict...',
+    @logs_vars(main_logger,
+               start_message='Creating a new DropNoneDict...',
                end_message='Created new DropNoneDict.',
                start_message_level='info', end_message_level='info')
-    def __init__(self, map_: Mapping = ..., *, none_condition: Any = None,
-                 **kwargs):
+    def __init__(self, map_: Mapping = ..., *, none_condition: Any = None, **kwargs):
         """
         A dictionary that will automatically drop values of None.
 
         :param map_: A Mapping to be used to instantiate the dictionary.
         :param none_condition: What value gets auto-dropped? Defaults to None.
-        :param kwargs: The kwargs representing key-val pairs to put in the
-            dict.
+        :param kwargs: The kwargs representing key-val pairs to put in the dict.
         """
         self._none_condition = none_condition
         self.__set_check_func()
         main_logger.trace('Setting values...')
         dict.__init__(self, self._handle_gen_args(map_, kwargs))
         main_logger.trace('Values set.')
 
     @property
-    def none_condition(self) -> Any:
-        return self._none_condition
+    def none_condition(self) -> Any: return self._none_condition
 
     @none_condition.setter
     def none_condition(self, value: Any):
         main_logger.info(f'Setting none_condition for a DropNoneDict to'
                          f' {value}...')
         self._none_condition = value
         self.__set_check_func()
 
     @logs_vars(main_logger,
-               start_message='Handling general arguments and forming dictionary'
-                             ' for DropNoneDict...',
+               start_message='Handling general arguments and forming dictionary for '
+                             'DropNoneDict...',
                end_message='General arguments handled.')
-    def _handle_gen_args(self,
-                         map_: Mapping = ...,
-                         kwargs: dict = ...) -> dict:
+    def _handle_gen_args(self, map_: Mapping = ..., kwargs: dict = ...) -> dict:
         """Handles the args at __init__."""
         output = {}
         if map_ is not ...:
             main_logger.trace('map_ exists. Parsing and updating output...')
             output.update(self._filter_map(map_))
 
         if kwargs is not ...:
@@ -164,35 +148,31 @@
     def _filter_map(self, map_: Union[Mapping, dict]) -> dict:
         """Filters out bad args from map_ and adds the rest."""
         main_logger.trace(f'Filtering out bad values from {map_}...')
 
         output = {}
         for key, val in map_.items():
             if type(val) is DropNoneDict._NoneIfLater:
-                main_logger.trace(f'{key} has a DropNoneDict._NoneIfLater as'
-                                  f' its value. Finalizing'
-                                  f' DropNoneDict._NoneIfLater...')
+                main_logger.trace(f'{key} has a DropNoneDict._NoneIfLater as its value. Finalizing '
+                                  f'DropNoneDict._NoneIfLater...')
                 val = val(self)
 
             if self._check_func(val):
-                main_logger.trace(f"{val} does not equate to the current"
-                                  f" DropNoneDict's None. Adding {key}: {val}"
-                                  f" to output...")
+                main_logger.trace(f'{val} does not equate to the current DropNoneDict\'s None. '
+                                  f'Adding {key}: {val} to output...')
                 output[key] = val
 
-        main_logger.trace('Finished filtering out bad values. Returning'
-                          ' filtered map...')
+        main_logger.trace('Finished filtering out bad values. Returning filtered map...')
         return output
 
     def __setitem__(self, k, v):
         main_logger.debug(f'Setting key {k} to {v} in DropNoneDict...')
 
         if not self._check_func(v):
-            main_logger.trace(f'Value is effectively None. Deleting key {k}'
-                              f' if it exists...')
+            main_logger.trace(f'Value is effectively None. Deleting key {k} if it exists...')
             if k in self:
                 del self[k]
 
         else:
             main_logger.trace('Value is not effectively None. Proceeding...')
             dict.__setitem__(self, k, v)
```

### Comparing `funky_modifiers-0.1.1/src/funk_py/super_dicts/list_dict.py` & `funky_modifiers-0.1.7/src/funk_py/super_dicts/list_dict.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 from typing import Union, Callable, Any, Tuple, Iterable
 
 
 class ListDict(list):
-    def __init__(self, key_function: Callable, values: Iterable = None):
+    def __init__(self, key_function: Callable, values: Iterable = ...):
         """
         A list that sort of acts like a dictionary...
 
-        :param key_function: The function that should be called on each item
-            to get its appropriate key.
+        :param key_function: The function that should be called on each item to get its appropriate
+            key.
         :param values: The values that should be put in the list.
         """
         list.__init__(self)
         self.__key_function = key_function
-        if values is not None:
+        if values is not ...:
             for item in values:
                 list.append(self, self.__process_item(item))
 
     def __process_item(self, item) -> tuple[Any, str]:
         """
-        An internal helper function used to apply the key_function to
-        incoming values.
+        An internal helper function used to apply the key_function to incoming values.
 
         :param item: The item that needs to be converted to a key-value pair.
         :return: A tuple consisting of the value and key for the item.
         """
         return item, self.__key_function(item)
 
-    def __locate_index(self,
-                       key: Union[str, int, slice, Tuple[str, int]]) -> int:
+    def __locate_index(self, key: Union[str, int, slice, Tuple[str, int]]) -> int:
         """
-        An internal helper function used to determine what index an item
-        should be at. Will throw an error if the key is invalid.
+        An internal helper function used to determine what index an item should be at. Will throw an
+            error if the key is invalid.
 
         :param key: The key/index that should be sought.
         :return: An integer indicating the item's index in the list.
         """
         if type(key) in [int, slice]:
             return key
 
@@ -50,131 +48,113 @@
             if list.__getitem__(self, i)[1] == key:
                 count += 1
                 if count == target_count:
                     return i
 
         raise KeyError(key)
 
-    def __setitem__(self, key: Union[str, int, slice, Tuple[str, int]],
-                    value) -> None:
+    def __setitem__(self, key: Union[str, int, slice, Tuple[str, int]], value) -> None:
         """
-        Sets an item in the ListDict. Will raise an exception if the item
-        index cannot be determined.
+        Sets an item in the ListDict. Will raise an exception if the item index cannot be
+            determined.
 
-        :param key: If key is a string, will attempt to find an item with
-            a matching key. Will raise an exception if said key cannot be
-            located. If key is an integer or a slice, normal list indexing
-            rules will be used to search. If key is a tuple consisting of
-            a string and an integer (n), will attempt to find items with
-            matching keys, then replaces the nth element with a matching key.
-        :param value: The value that should be assigned in place of the old
-            value.
+        :param key: If this is a ``str``, will attempt to find an item with a matching key. Will
+            raise an exception if it cannot be located. If this is an ``int`` or a ``slice``, normal
+            list indexing rules will be used to search. If this is a ``tuple`` consisting of a
+            ``str`` and an ``int`` (*n), it will attempt to find items with matching keys, then
+            replaces the *nth* element with a matching key.
+        :param value: The value that should be assigned in place of the old value.
         :return: Does not return anything.
         """
         index = self.__locate_index(key)
         if type(index) is slice:
-            list.__setitem__(self, index,
-                             [self.__process_item(val) for val in value])
+            list.__setitem__(self, index, [self.__process_item(val) for val in value])
 
         else:
             list.__setitem__(self, index, self.__process_item(value))
 
-    def __getitem__(self,
-                    key: Union[str, int, slice, Tuple[str, int]]) -> Any:
+    def __getitem__(self, key: Union[str, int, slice, Tuple[str, int]]) -> Any:
         """
-        Gets an item from the ListDict. Will raise an exception if the item
-        index cannot be determined.
+        Gets an item from the ListDict. Will raise an exception if the item index cannot be
+            determined.
 
-        :param key: If key is a string, will attempt to find an item with a
-            matching key. Will raise an exception if said key cannot be
-            located. If key is an integer or a slice, normal list indexing
-            rules will be used to search. If key is a tuple consisting of
-            a string and an integer (n), will attempt to find items with
-            matching keys, then return the nth element.
+        :param key: If this is a ``str``, will attempt to find an item with a matching key. Will
+            raise an exception if it cannot be located. If this is an ``int`` or a ``slice``, normal
+            list indexing rules will be used to search. If this is a ``tuple`` consisting of a
+            ``str`` and an ``int`` (*n*), will attempt to find items with matching keys, then return
+            the *nth* element with a matching key.
         :return: The item(s) at the desired key/index.
         """
         if type(key) is slice:
-            return self.__class__(
-                [t[0]
-                 for t
-                 in list.__getitem__(self, self.__locate_index(key))]
-            )
+            return self.__class__([t[0] for t in list.__getitem__(self, self.__locate_index(key))])
 
         return list.__getitem__(self, self.__locate_index(key))[0]
 
-    def get(self, key: Union[str, Tuple[str, int]],
-            default: Any = None) -> Any:
+    def get(self, key: Union[str, Tuple[str, int]], default: Any = None) -> Any:
         """
-        Gets an item from the ListDict by **key**. Will not raise an exception
-        if the **key** does not exist, but will instead return default.
+        Gets an item from the ``ListDict`` by *key*. Will not raise an exception if the *key*
+        does not exist, but will instead return default.
 
-        :param key: If key is a string, will attempt to find an item with a
-            matching key. If key is a tuple consisting of a string and an
-            integer (n), will attempt to find items with matching keys, then
-            return the nth element.
-        :param default: The default value to return if requested key does not
-        exist.
-        :return: The item at the desired key or - should the key not be
-            found - default.
+        :param key: If this is a ``str``, will attempt to find an item with a matching key. If this
+            is a ``tuple`` consisting of a ``str`` and an ``int`` (*n*), will attempt to find items
+            with matching keys, then return the *nth* element with a matching key.
+        :param default: The default value to return if requested key does not exist.
+        :return: The item at the desired key or - should the key not be found - default.
         """
         if type(key) in [int, slice]:
             raise KeyError(f'{repr(key)} is not a valid key for {type(self)}.')
 
         try:
             return list.__getitem__(self, self.__locate_index(key))
 
         except KeyError:
             return default
 
     def pop(self, key: Union[str, int, Tuple[str, int]] = ...) -> Any:
         """
-        Pops an item from the ListDict. Will raise an exception if the item
-        index cannot be determined.
+        Pops an item from the ``ListDict``. Will raise an exception if the item index cannot be
+            determined.
 
-        :param key: If key is a string, will attempt to find an item with a
-            matching key. Will raise an exception if said key cannot be
-            located. If key is an integer, normal list indexing rules will be
-            used to search. If key is a tuple consisting of a string and an
-            integer (n), will attempt to find items with matching keys, then
-            return the nth element. If omitted, the last item in the list
-            will be returned.
-        :return: The item at the desired key/index, will also delete from the
-            list.
+        :param key: If this is a ``str``, will attempt to find an item with a matching key. Will
+            raise an exception if it cannot be located. If this is an ``int``, normal list indexing
+            rules will be used to search. If this is a ``tuple`` consisting of a ``str`` and an
+            ``int`` (*n*), will attempt to find items with matching keys, then return the *nth*
+            element with a matching key. If omitted, the last item in the list will be returned.
+        :return: The item at the desired key/index, will also delete from the list.
         """
         if not len(self):
             raise IndexError('pop from empty list')
 
         if key is ...:
             return list.pop(self)
 
         else:
             return list.pop(self, self.__locate_index(key))
 
     def __delitem__(self, key) -> None:
         """
-        Deletes an item from the ListDict. Will raise an exception if the item
-        index cannot be determined.
+        Deletes an item from the ListDict. Will raise an exception if the item index cannot be
+            determined.
 
-        :param key: If key is a string, will attempt to find an item with a
-            matching key. Will raise an exception if said key cannot be
-            located. If key is an integer or a slice, normal list indexing
-            rules will be used to search. If key is a tuple consisting of a
-            string and an integer (n), will attempt to find items with
-            matching keys, then return the nth element.
+        :param key: If this is a ``str``, will attempt to find an item with a matching key. Will
+            raise an exception if it cannot be located. If this is an ``int`` or a ``slice``, normal
+            list indexing rules will be used to search. If this is a ``tuple`` consisting of a
+            ``str`` and an ``int`` (*n*), will attempt to find items with matching keys, then return
+            the *nth* element with a matching key.
         :return: No return.
         """
         list.__delitem__(self, self.__locate_index(key))
 
     def __contains__(self, item) -> bool:
         """
-        Figure out if an item is contained in the ListDict.
+        Figure out if an item is contained in the ``ListDict``.
 
-        :param item: If item is a string, a search for a key will be done.
-            Otherwise, a search for an exact match will be carried out.
-        :return: A bool indicating whether the item was found in the ListDict.
+        :param item: If this is a ``str``, a search for a key will be done. Otherwise, a search for
+            an exact match will be carried out.
+        :return: A bool indicating whether the item was found in the ``ListDict``.
         """
         if type(item) is str:
             for i in range(len(self)):
                 if list.__getitem__(self, i)[1] == item:
                     return True
 
         else:
```

### Comparing `funky_modifiers-0.1.1/src/funk_py/super_dicts/multi_key_dict.py` & `funky_modifiers-0.1.7/src/funk_py/sorting/pieces.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,395 +1,400 @@
-from typing import Any, Mapping, Iterable
+import json
+from enum import Enum
+from typing import Mapping, Any, Literal, Union, List, Tuple, Optional, Iterator, Generator, \
+    Callable
+from urllib.parse import parse_qs
+import yaml
+
+from funk_py.modularity.decoration.enum_modifiers import converts_enums
+from funk_py.modularity.logging import make_logger
+from funk_py.sorting.converters import csv_to_json, xml_to_json, wonky_json_to_json, jsonl_to_json
+from funk_py.sorting.dict_manip import convert_tuplish_dict
+
+main_logger = make_logger('pieces', 'PIECES_LOG_LEVEL', default_level='warning')
+
+main_logger.info('Setting up simple types...')
+OutputMapSpecifier = Literal['json', 'jsonl', 'json\'',
+                             'xml', 'xml-sa',
+                             'e-list', 'list',
+                             'csv',
+                             'yaml',
+                             'tuple-dict',
+                             'form-urlencoded',
+                             'combinatorial', 'tandem', 'reduce', 'accumulate']
+PickProcessFunc = Callable[[list, list, dict], None]
+PickFinalFunc = Callable[[list, dict], None]
+
+
+class PickType(Enum):
+    """``PickType`` is an enum containing the valid pick types for :func:`pick`."""
+    COMBINATORIAL = 'combinatorial'
+    TANDEM = 'tandem'
+    REDUCE = 'reduce'
+    ACCUMULATE = 'accumulate'
+
+
+class PickInstruction(Enum):
+    JSON = 'json'
+    JSONL = 'jsonl'
+    JSON_SINGLE_QUOTE = 'json\''
+    XML = 'xml'
+    XMLSA = 'xml-sa'
+    ELIST = 'e-list'
+    LIST = 'list'
+    CSV = 'csv'
+    YAML = 'yaml'
+    TUPLE_DICT = 'tuple-dict'
+    FORM = 'form-urlencoded'
+
+    COMBINATORIAL = 'combinatorial'
+    TANDEM = 'tandem'
+    REDUCE = 'reduce'
+    ACCUMULATE = 'accumulate'
+
+
+OutputMapType = Union[Mapping[str, Union[str, Mapping, PickInstruction]],
+                      List[Union[str, Mapping, PickInstruction]]]
+
+
+main_logger.info('Finished setting up simple types.')
+
+
+def _com_tan_start_and_list_func(ans: list, builder: list, static_builder: dict) -> None:
+    builder.extend(ans)
+
+
+def _acc_start_list_and_iter_func(ans: list, builder: list, static_builder: dict) -> None:
+    if not len(builder):
+        builder.extend(ans)
+
+    else:
+        for _ans in ans:
+            for k, v in _ans.items():
+                if k in builder[0]:
+                    if isinstance(v, list):
+                        builder[0][k].extend(v)
 
+                    else:
+                        builder[0][k].append(v)
 
-class MultiKeyDict(dict):
-    class __Holder(list):
-        """Holds and acts as a reference for values in the MultiKeyDict."""
-        class ValNode:
-            __slots__ = 'value', 'pos'
-
-            def __hash__(self):
-                return self.pos
-
-        def __init__(i_self):
-            list.__init__(i_self)
-
-        def append(i_self, object_: Any) -> bool:
-            """Appends a value to the __Holder."""
-            c = type(object_)
-            for obj in i_self:
-                if (c is type(obj.value) and object_ == obj.value) or \
-                        (obj.value is None and object_ is None):
-                    return True
-
-            list.append(i_self, i_self.ValNode())
-            list.__getitem__(i_self, -1).value = object_
-            list.__getitem__(i_self, -1).pos = len(i_self) - 1
-            return False
-
-        def index(i_self, value: Any, start: int = ...,
-                  stop: int = ...) -> int:
-            if value is None:
-                for i in range(len(i_self)):
-                    if list.__getitem__(i_self, i).value is None:
-                        return i
+                elif isinstance(v, list):
+                    builder[0][k] = v
 
-            else:
-                for i in range(len(i_self)):
-                    if list.__getitem__(i_self, i).value == value:
-                        return i
-
-            raise ValueError(f"'{value}' is not in __Holder")
-
-        def __contains__(i_self, item):
-            if item is None:
-                for obj in list.__iter__(i_self):
-                    if obj.value is None:
-                        return True
+                else:
+                    builder[0][k] = [v]
 
-            else:
-                for obj in list.__iter__(i_self):
-                    if obj.value == item:
-                        return True
-
-            return False
-
-        def __setitem__(i_self, index: int, value):
-            t = list.__getitem__(i_self, index)
-            t.value = value
-
-        def __getitem__(i_self, index: int):
-            return list.__getitem__(i_self, index)
-
-        def __delitem__(i_self, index: int):
-            for i in range(index + 1, len(i_self)):
-                list.__getitem__(i_self, i).pos -= 1
-
-            list.__delitem__(i_self, index)
-
-    class _ValuesView:
-        """An object used to view the values inside of a MultiKeyDict."""
-        def __init__(i_self, parent: 'MultiKeyDict'):
-            i_self.parent = parent
-            i_self._index = 0
-
-        def __iter__(i_self):
-            return i_self
-
-        def __next__(i_self):
-            h = i_self.parent._holder
-            if i_self._index < len(h):
-                i_self._index += 1
-                return h[i_self._index - 1].value
-
-            raise StopIteration
-
-    class _ItemsView:
-        """An object used to view the items inside of a MultiKeyDict."""
-        def __init__(i_self, parent: 'MultiKeyDict'):
-            i_self.parent = parent
-            i_self.keys = list(parent.keys())
-            i_self._index = 0
-
-        def __iter__(i_self):
-            return i_self
-
-        def __next__(i_self):
-            if i_self._index < len(i_self.keys):
-                i_self._index += 1
-                key = i_self.keys[i_self._index - 1]
-                return key, dict.__getitem__(i_self.parent, key).value
-
-            raise StopIteration
-
-    def __init__(self, map_: Mapping, **kwargs):
-        """
-        Checks a mapping for keys using the same value and assigns them a
-        reference to a holder for the value.
-
-        :param map_: A mapping
-        :param kwargs: Keywords to use to build a mapping or add on to a
-            mapping.
-        """
-        self._holder = self.__Holder()
-        dict.__init__(self)
-        temp_dict = dict(map_, **kwargs)
-        for key, val in temp_dict.items():
-            self._process_key_val_pair(key, val)
-
-    def _process_key_val_pair(self, keys: Iterable, value):
-        """
-        Internal method that processes a key-value pair.
-
-        :param keys: key will be iterated over to create new key-val pairs.
-        :param value: value will be searched for in existing values. If the
-            value is found, the _Holder reference of that value will be used to
-            represent it in generated key-val pairs. If not, a new _Holder
-            reference will be created to represent it in key-val pairs.
-        """
-        if not isinstance(keys, Iterable) or type(keys) is str:
-            keys = [keys]
-
-        i = self._holder.index(value) if self._holder.append(value) else -1
-        for key in keys:
-            dict.__setitem__(self, key, self._holder[i])
-
-    def __getitem__(self, key):
-        """
-        Used to get the value of a key from the MultiKeyDict.
-
-        :param key: This may be a tuple, and if it is, a list of the values for
-            the keys passed will be returned. Otherwise, the key passed will be
-            located, and its corresponding value returned. Will raise an
-            exception if the key is not in the MultiKeyDict.
-        :return: The value corresponding to the key if a single key was passed.
-            Otherwise, the values corresponding to the keys in the form of a
-            tuple.
-        """
-        if type(key) is tuple:
-            answer = tuple(dict.__getitem__(self, k).value for k in key)
-            if len(answer) == 1:
-                return answer[0]
 
-            else:
-                return answer
+def _com_iter_func(ans: list, builder: list, static_builder: dict) -> None:
+    if (t := len(ans)) >= 1:
+        for i in range(len(builder)):
+            for _ans in ans[1:]:
+                copier = builder[i].copy()
+                copier.update(_ans)
+                builder.append(copier)
 
-        return dict.__getitem__(self, key).value
+            builder[i].update(ans[0])
 
-    def __setitem__(self, key, value):
-        """
-        Used to set key-val pairs for the MultiKeyDict.
-
-        :param key: If anything other than a tuple is used for the key, it
-            will be converted to a list of one element. The keys passed will
-            then be assigned the appropriate values, and their old values will
-            be checked to ensure they are still needed. If any values become
-            unutilized, they will be deleted.
-        :param value: The value to assign to key(s).
-        """
-        self._process_key_val_pair(key, value)
-
-    def __delitem__(self, key):
-        """
-        Used to delete keys from the MultiKeyDict.
-
-        :param key: If anything other than a tuple is used as the key, it will
-            be converted to a list of one element. The keys passed will then be
-            deleted from the dictionary, and if any values become unutilized,
-            they will be deleted as well.
-        """
-        if type(key) is not tuple:
-            key = [key]
-
-        # construct a set of values possibly removed and remove keys
-        counter = set()
-        for k in key:
-            counter.add(dict.__getitem__(self, k))
-            dict.__delitem__(self, k)
-
-        # if any values are completely removed, delete them
-        val_list = set(dict.values(self))
-        for v in counter:
-            if v not in val_list:
-                del self._holder[v.pos]
-
-    def values(self) -> _ValuesView:
-        """
-        Returns an iterable to view the values in a MultiKeyDict. Values are
-        treated as unique.
-
-        :return: MultiKeyDict._ValuesView
-        """
-        return self._ValuesView(self)
-
-    def items(self) -> _ItemsView:
-        """
-        Returns an iterable to view items in a MultiKeyDict.
-
-        :return: MultiKeyDict._ItemsView
-        """
-        return self._ItemsView(self)
-
-    def pop(self, key, default=...):
-        """
-        Pop the value(s) corresponding to given key(s). A value will only be
-        fully-removed if there are no longer any keys referencing it.
-
-        :param key: If a single item is used as a key, it will be converted to
-            a list of one element for searches. The key(s) passed will be
-            located if possible, and their corresponding value(s) returned in a
-            list.
-        :param default: The default value used to fill in for keys that don't
-            exist.
-        :return: A tuple of the values corresponding to the keys if multiple
-            keys were sought. Otherwise the value corresponding to the key
-            sought.
-        """
-        if type(key) is not tuple:
-            key = [key]
-
-        # construct a set of values possibly removed and pop keys and values
-        output = []
-        # if default is ..., will have to test each key to verify it exists.
-        if default is ...:
-            for k in key:
-                if key not in self:
-                    raise KeyError(f"{repr(k)}")
+    elif t == 1:
+        for source in builder:
+            source.update(ans[0])
 
-                output.append(dict.pop(self, k))
 
-        # do not need to test if there is a default
-        else:
-            for k in key:
-                output.append(dict.pop(self, k, default))
+def _tan_iter_func(ans: list, builder: list, static_builder: dict) -> None:
+    if len(ans) == 0:
+        return
 
-        # if any values are completely removed, delete them
-        val_list = set(dict.values(self))
-        for v in output:
-            if v not in val_list:
-                del self._holder[v.pos]
-
-        return output[0].value if len(output) == 1 \
-            else tuple(v.value for v in output)
-
-    def pop_unique(self, key, default=...):
-        """
-        Pop the value(s) corresponding to given key(s). A value will only be
-        fully-removed if there are no longer any keys referencing it. Will
-        only return unique values.
-
-        :param key: If a single item is used as a key, it will be converted to
-            a list of one element for searches. The key(s) passed will be
-            located if possible, and their corresponding value(s) returned in a
-            list.
-        :param default: The default value used to fill in for keys that don't
-            exist.
-        :return: A tuple of the unique values corresponding to the keys if
-            multiple keys were sought. Otherwise the value corresponding
-            to the key sought.
-        """
-        if type(key) is not tuple:
-            key = [key]
-
-        # construct a set of values possibly removed and pop keys and values
-        counter = set()
-        # if default is ..., will have to test each key to verify it exists.
-        if default is ...:
-            for k in key:
-                if k not in self:
-                    raise KeyError(f"{repr(k)}")
+    if len(builder) >= len(ans):
+        for i in range(len(ans)):
+            builder[i].update(ans[i])
 
-                counter.add(dict.pop(self, k))
+    else:
+        for i in range(len(builder)):
+            builder[i].update(ans[i])
 
-        # do not need to test if there is a default
-        else:
-            for k in key:
-                counter.add(dict.pop(self, k, default))
+        for i in range(len(builder), len(ans)):
+            builder.append(ans[i])
+
+
+def _com_tan_final_func(builder: list, static_builder: dict) -> None:
+    for result in builder:
+        result.update(static_builder)
+
+
+def _acc_final_func(builder: list, static_builder: dict) -> None:
+    if not len(builder):
+        builder.append(static_builder)
 
-        # if any values are completely removed, delete them
-        val_list = set(dict.values(self))
-        for v in counter:
-            if v not in val_list:
-                del self._holder[v.pos]
-
-        return [v.value for v in counter]
-
-    def get(self, *keys, default=...) -> Any:
-        """
-        Used to get the value(s) of key(s) from the MultiKeyDict without the
-        likelihood of raising an exception. Will return values in a tuple
-        format, and will only return unique values.
-
-        :param keys: If a single item is used as a key, it will be converted to
-            a list of one element for searches. The key(s) passed will be
-            located if possible, and their corresponding value(s) returned in a
-            list.
-        :param default: The default value used to fill in for keys that don't
-            exist.
-        :return: A tuple of the values corresponding to the keys if multiple
-            keys were sought. Otherwise the value corresponding to the key
-            sought.
-        """
-        output = []
-        for k in keys:
-            if k not in self:
-                output.append(default)
-                continue
-
-            output.append(dict.__getitem__(self, k).value)
-
-        return output[0] if len(output) == 1 else tuple(output)
-
-    def get_items(self, keys: Iterable, default=...) -> dict:
-        """
-        Used to get the items corresponding to an Iterable of keys. Will
-        not raise an error for keys that don't exist.
-
-        :param keys: An Iterable which contains keys whose values are sought.
-        :param default: The default value for keys that don't exist. If not
-            specified, will omit keys that don't exist from the output
-            dictionary.
-        :return: A dictionary with the items that were found.
-        """
-        output = {}
-        for k in keys:
-            if k not in self:
-                if default is not ...:
-                    output[k] = default
-
-                continue
-
-            output[k] = dict.__getitem__(self, k).value
-
-        return output
-
-    def get_unique(self, *keys, default=...):
-        """
-        Used to get the value(s) of key(s) from the MultiKeyDict without the
-        likelihood of raising an exception. Will return values in a tuple
-        format, and will only return unique values.
-
-        :param keys: If a single item is used as a key, it will be converted to
-            a list of one element for searches. The key(s) passed will be
-            located if possible, and their corresponding value(s) returned in a
-            list.
-        :param default: The default value used to fill in for keys that don't
-            exist. If left empty, missing keys will not insert any value.
-        :return: A tuple of the unique values corresponding to the keys if
-            multiple keys were sought. Otherwise the value corresponding to
-            the key sought.
-        """
-        counter = set()
-        default_in = False
-        # if default is ..., will have to test each key to verify it exists.
-        if default is ...:
-            for k in keys:
-                if k in self:
-                    counter.add(dict.__getitem__(self, k))
+    else:
+        for k, v in static_builder.items():
+            if k in builder[0]:
+                if isinstance(v, list):
+                    builder[0][k].extend(v)
+
+                else:
+                    builder[0][k].append(v)
+
+            elif isinstance(v, list):
+                builder[0][k] = v
+
+            else:
+                builder[0][k] = [v]
+
+
+_PICK_TYPE_DEFS = {
+    PickType.COMBINATORIAL: (
+        _com_tan_start_and_list_func,
+        _com_tan_start_and_list_func,
+        _com_iter_func,
+        _com_tan_final_func,
+    ),
+    PickType.TANDEM: (
+        _com_tan_start_and_list_func,
+        _com_tan_start_and_list_func,
+        _tan_iter_func,
+        _com_tan_final_func,
+    ),
+    PickType.REDUCE: (
+        _com_tan_start_and_list_func,
+        _tan_iter_func,
+        _com_iter_func,
+        _com_tan_final_func,
+    ),
+    PickType.ACCUMULATE: (
+        _acc_start_list_and_iter_func,
+        _acc_start_list_and_iter_func,
+        _acc_start_list_and_iter_func,
+        _acc_final_func,
+    ),
+}
+_PICK_TYPE_NAMES = {
+    'combinatorial': _PICK_TYPE_DEFS[PickType.COMBINATORIAL],
+    'tandem': _PICK_TYPE_DEFS[PickType.TANDEM],
+    'reduce': _PICK_TYPE_DEFS[PickType.REDUCE],
+    'accumulate': _PICK_TYPE_DEFS[PickType.ACCUMULATE],
+}
+
+
+def pick(
+        output_map: OutputMapType,
+        _input: Any,
+        list_handling_method: PickType = PickType.COMBINATORIAL
+) -> list:
+    return _pick(output_map, _input, *_PICK_TYPE_DEFS[list_handling_method])
+
+
+def _pick_setup(
+        output_map: OutputMapType,
+        _input: Any
+) -> Tuple[Optional[OutputMapType], Any, list, bool, Optional[PickType]]:
+    if isinstance(output_map, list):
+        # If the output_map is a list, that should mean the user specified a type of conversion to
+        # enact on the input (as long as their output_map is valid).
+        if isinstance(_input, list) and output_map[0] != 'e-list':
+            # In the case that _input is a list, we should first check if the user specified e-list
+            # since that means "expected list". If they did specify that, we'll want to consume it,
+            # so this branch won't execute, and we'll move over to the next step. If they didn't, we
+            # continue on our mary way, and don't move forward on the output_map yet. We want to
+            # pass the non-mutated _input as well since there's no mutation to be performed on it.
+            return output_map, _input, [], False, None
 
-        # do not need to test if there is a default
         else:
-            for k in keys:
-                ans = dict.get(self, k, default)
-                if ans is default \
-                        or ans == default and type(default) == type(ans):
-                    default_in = True
+            # In the case that _input is not a list, we will just attempt to parse as the user
+            # expected.
+            try:
+                if (t := output_map[0]) in _PICK_TYPE_NAMES:
+                    # This should handle cases where the user specifies changing modes during
+                    # parsing.
+                    return output_map[-1], _input, [], False, _PICK_TYPE_NAMES[t]
+
+                worker = parse_type_as(output_map[0], _input, output_map[1:-1])
+
+            except Exception as e:
+                main_logger.warning(f'User\'s expected parsing method failed. Exception raised: '
+                                    f'{e}')
+                return None, None, [], True, None
+
+            return output_map[-1], worker, [], False, None
+
+    elif isinstance(output_map, str):
+        # Theoretically, we should never get here, but just in case, this line should catch
+        # instances where a key is immediately requested. Who knows, maybe a change down the line
+        # will cause this code to be needed.
+        return None, None, [{output_map: _input}], False, None
+
+    # If nothing caught, just pass everything back as-is.
+    return output_map, _input, [], False, None
+
+
+def _find_and_follow_first_path_in_pick(
+        output_map_iter: Iterator,
+        worker: Any,
+        builder: list,
+        static_builder: dict
+) -> Tuple[Optional[OutputMapType], Any, bool]:
+    while True:
+        try:
+            path, instruction = next(output_map_iter)
+            if path in worker:
+                if isinstance(instruction, str):
+                    if not isinstance(worker, dict):
+                        main_logger.warning(f'An unexpected value was encountered in pick attempt. '
+                                            f'a path has now been skipped. value = {worker}')
+                        return None, None, False
+
+                    static_builder[instruction] = worker[path]
+                    builder.append({})
+                    # The caller doesn't need to call anything, we did everything needed for the
+                    # first key.
+                    return None, None, False
 
                 else:
-                    counter.add(ans)
+                    # Rather than recursively calling a function from inside of this function, we
+                    # pass back the values that the caller needs to use to call the function itself.
+                    # This is done this way to limit how deep we go on the stack. It also means the
+                    # caller can decide which function to call on the values.
+                    if isinstance(worker, dict):
+                        return instruction, worker[path], False
+
+                    main_logger.warning(f'Path ended early. {repr(worker)} does not have keys.')
+
+        except StopIteration:
+            # Welp, the caller will have to return immediately, none of the paths requested were
+            # present.
+            return None, None, True
+
+
+def _pick_iter(
+        output_map_iter: Iterator,
+        worker: Any,
+        builder: list,
+        static_builder: dict,
+        func: Callable[[list, list, dict], None]
+) -> Generator[Tuple[Optional[OutputMapType], Any, bool], list, None]:
+    """
+    Finishes iterating after the first path was successfully followed. Expects the result of an
+    external function call to be sent to it if it yields an instruction.
+    """
+    if type(worker) is dict:
+        for path, instruction in output_map_iter:
+            if path in worker:
+                if isinstance(instruction, str):
+                    static_builder[instruction] = worker[path]
 
-        output = [v.value for v in counter]
-        if default_in:
-            output.append(default)
-
-        return output
-
-    def update(self, __m: Mapping = None, **kwargs) -> None:
-        """
-        Used to integrate another mapping into this one.
-
-        :param __m: The mapping to integrate.
-        :param kwargs: Keyword args to construct from.
-        """
-        d = dict(__m, **kwargs) if __m is not None else dict(**kwargs)
-        for key, val in d.items():
-            self._process_key_val_pair(key, val)
+                else:
+                    # Rather than recursively calling a function from inside of this function, we
+                    # pass back the values that the caller needs to use to call the function itself.
+                    # This is done this way to limit how deep we go on the stack. It also means the
+                    # caller can decide which function to call on the values.
+                    # The caller should send the result of the function back to us here so that we
+                    # can call func on it.
+                    result = yield instruction, worker[path], False
+                    try:
+                        func(result, builder, static_builder)
+
+                    except Exception as e:
+                        main_logger.warning(f'There was an error when attempting to process a '
+                                            f'result. Exception raised: {e}')
+
+    else:
+        main_logger.warning(f'Cannot follow a path in a non-dict. ({worker})')
+
+    yield None, None, True
+
+
+def _pick(
+        output_map: OutputMapType,
+        _input: Any,
+        start_func: PickProcessFunc,
+        list_func: PickProcessFunc,
+        iter_func: PickProcessFunc,
+        final_func: PickFinalFunc
+) -> list:
+    """
+    The core of :func:`pick`. All pick types run through this method.
+
+    :param output_map: The map which describes how incoming data should be parsed.
+    :param _input: The incoming data.
+    :param start_func: The function that should be used when parsing a list of results for ingestion
+        into the list being built.
+    :param iter_func: The function that should be used to parse a list of results during iteration
+        over the ``output_map``.
+    :param final_func: The function which should be called to finalize the result at the end of
+        retrieving all possible data.
+    :return:
+    """
+    static_builder = {}
+    output_map, worker, builder, fail, new_mode = _pick_setup(output_map, _input)
+    if fail or len(builder):
+        return builder
+
+    elif new_mode is not None:
+        start_func, list_func, iter_func, final_func = new_mode
+
+    __pick = lambda o_map, w: _pick(o_map, w, start_func, list_func, iter_func, final_func)  # noqa
+
+    if isinstance(worker, list):
+        for item in worker:
+            list_func(__pick(output_map, item), builder, static_builder)
+
+    else:
+        output_map_iter = iter(output_map.items())
+        *instruction, return_now = _find_and_follow_first_path_in_pick(
+            output_map_iter, worker, builder, static_builder)
+        if return_now:
+            return builder
+
+        elif instruction[0] is not None:
+            # If instructions were given by _find_and_follow_first_path_in_pick, then we need to
+            # recursively call this function with the results.
+            start_func(__pick(*instruction), builder, static_builder)
+
+        pick_iter = _pick_iter(output_map_iter, worker, builder, static_builder, iter_func)
+
+        for *instruction, return_now in pick_iter:
+            if instruction[0] is not None:
+                # If instructions were given by pick_iter, then we need to recursively call this
+                # function and pass the results back to pick_iter.
+                pick_iter.send(__pick(*instruction))
+
+        final_func(builder, static_builder)
+
+    return builder
+
+
+@converts_enums
+def parse_type_as(_type: PickInstruction, data: Any, args: list) -> Union[dict, list]:
+    switch = {
+        PickInstruction.JSON: lambda x: json.loads(x),
+        PickInstruction.JSONL: jsonl_to_json,
+        PickInstruction.JSON_SINGLE_QUOTE: wonky_json_to_json,
+        PickInstruction.XML: xml_to_json,
+        PickInstruction.XMLSA: lambda x: xml_to_json(x, True),
+        PickInstruction.ELIST: lambda x: x if isinstance(x, list) else [x],
+        PickInstruction.CSV: csv_to_json,
+        PickInstruction.LIST: lambda x: x.split(','),
+        PickInstruction.YAML: yaml.safe_load,
+        PickInstruction.FORM: parse_qs,
+    }
+
+    arg_switch = {
+        PickInstruction.TUPLE_DICT: _parse_and_execute_tuplish,
+    }
+
+    if _type in switch:
+        return switch[_type](data)
+
+    elif _type in arg_switch:
+        return switch[_type](data, args)
+
+    raise ValueError('Invalid type specified.')
+
+
+def _parse_and_execute_tuplish(data: Union[dict, list], args: list) -> dict:
+    if len(args):
+        args = args[0]
+        if isinstance(args, dict):
+            return convert_tuplish_dict(data, args.get('pair_name'),
+                                        args.get('key_name'), args.get('val_name'))
+
+        else:
+            raise ValueError('TUPLE_DICT given an invalid argument format.')
```

### Comparing `funky_modifiers-0.1.1/src/funk_py/super_dicts/windowed_list.py` & `funky_modifiers-0.1.7/src/funk_py/super_dicts/windowed_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Iterable
+from typing import Any, Dict, Collection
 
 
 class ListRefNode:
     class ListRefNodeIter:
         def __init__(self, parent: 'ListRefNode'):
             self.__start = True
             self.__next = parent
@@ -61,16 +61,16 @@
     def __del__(self):
         self.drop_out()
         self.lower_index()
         del self.source[self.index]
 
 
 class WindowedList:
-    def __init__(self, values: Iterable):
-        self._lookup = {}
+    def __init__(self, values: Collection):
+        self._lookup: Dict[int, ListRefNode] = {}
         self._on = {}
         if len(values):
             self._lookup[0] = ListRefNode(values, 0)
             self._on[0] = True
             for i in range(1, len(values)):
                 self._lookup[i] = ListRefNode(values, i, self._lookup[i - 1])
                 self._lookup[i - 1].next = self._lookup[i]
```

### Comparing `funky_modifiers-0.1.1/src/funky_modifiers.egg-info/SOURCES.txt` & `funky_modifiers-0.1.7/src/funky_modifiers.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,38 @@
 LICENSE
+MANIFEST.in
 README.md
+requirements.txt
 setup.py
 src/funk_py/__init__.py
 src/funk_py/modularity/__init__.py
 src/funk_py/modularity/basic_structures.py
 src/funk_py/modularity/bespoke_properties.py
 src/funk_py/modularity/logging.py
 src/funk_py/modularity/type_matching.py
 src/funk_py/modularity/decoration/__init__.py
+src/funk_py/modularity/decoration/enum_modifiers.py
 src/funk_py/modularity/decoration/init_modifiers.py
 src/funk_py/modularity/decoration/transforming_list.py
+src/funk_py/sorting/__init__.py
+src/funk_py/sorting/converters.py
+src/funk_py/sorting/dict_manip.py
+src/funk_py/sorting/pieces.py
 src/funk_py/super_dicts/__init__.py
 src/funk_py/super_dicts/drop_none_dict.py
 src/funk_py/super_dicts/list_dict.py
-src/funk_py/super_dicts/multi_key_dict.py
-src/funk_py/super_dicts/multi_value_dict.py
 src/funk_py/super_dicts/windowed_list.py
 src/funky_modifiers.egg-info/PKG-INFO
 src/funky_modifiers.egg-info/SOURCES.txt
 src/funky_modifiers.egg-info/dependency_links.txt
+src/funky_modifiers.egg-info/requires.txt
 src/funky_modifiers.egg-info/top_level.txt
+test/test_check_dict_equality.py
+test/test_check_list_equality.py
+test/test_convert_tuplish_dict.py
+test/test_converters.py
+test/test_converts_enums.py
 test/test_drop_none_dict.py
-test/test_logs_vars.py
+test/test_function_hash_and_equality.py
+test/test_logs_vars.py
+test/test_obj.py
+test/test_pick.py
```

### Comparing `funky_modifiers-0.1.1/test/test_logs_vars.py` & `funky_modifiers-0.1.7/test/test_logs_vars.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,69 @@
 import logging
+from logging import getLogger
 
 import pytest
 
-from modularity.logging import logs_vars
-from logging import getLogger
+from t_support import cov, cov_counter
+from funk_py.modularity.logging import logs_vars
+
+
+# The following manages whether the generated coverage instance from t_support should report. This
+# method of coverage is used so that coverage can be turned off to not interfere in timed tests.
+@pytest.fixture(scope='session', autouse=True)
+def c():
+    cov_counter.value += 1
+
+    yield cov
+
+    cov_counter.value -= 1
+
+    # We don't want to report till all test modules are completed...
+    if not cov_counter.value:
+        cov.stop()
+        cov.save()
+        cov.html_report()
 
 
 ARGUMENTS = 'Arguments:'
 LOGGER = getLogger('testy')
 ANSWER = 42
 LIFE = 'Bobbert'
 NAME = 'Stapler'
 BAD_NAME = 45
 AGE = 300
 
 
-LOG_NAME_LOOKUP = {'debug': logging.DEBUG, 'info': logging.INFO,
-                   'warning': logging.WARNING, 'error': logging.ERROR,
-                   'critical': logging.CRITICAL}
+LOG_NAME_LOOKUP = {'debug': logging.DEBUG, 'info': logging.INFO, 'warning': logging.WARNING,
+                   'error': logging.ERROR, 'critical': logging.CRITICAL}
+
+
+# Given this is testing a logging decorator, multiple thousands of tests are run with slight
+# differences, not just edge cases. If this breaks, it could mean endless headaches. It may be worth
+# it to later re-locate the logic for determining log level out of the decorator so that it can be
+# tested, separately, but to prevent silly mistakes like accidentally hard-coding a log level, it is
+# best to keep these tests.
 
 
 @pytest.fixture(params=['debug', 'info', 'warning', 'error', 'critical'])
-def different_str_levels(request):
-    return request.param
+def different_str_levels(request): return request.param
 
 
 @pytest.fixture(params=['upper', 'lower'])
 def all_different_str_levels(request, different_str_levels):
     return getattr(different_str_levels, request.param)()
 
 
-@pytest.fixture(params=[logging.DEBUG, logging.INFO, logging.WARNING,
-                        logging.ERROR, logging.CRITICAL])
-def different_int_levels(request):
-    return request.param
+@pytest.fixture(params=[logging.DEBUG, logging.INFO, logging.WARNING, logging.ERROR,
+                        logging.CRITICAL])
+def different_int_levels(request): return request.param
 
 
 @pytest.fixture(params=[None, 'This is a start message.', 42])
-def different_start_messages(request):
-    return request.param
+def different_start_messages(request): return request.param
 
 
 class MessageState:
     def __init__(self, start_message, end_message):
         self.start_message = start_message
         self.end_message = end_message
 
@@ -50,48 +71,45 @@
 @pytest.fixture(params=[None, 'This is an end message.', 24])
 def different_message_combos(request, different_start_messages):
     c = MessageState(different_start_messages, request.param)
     return c
 
 
 @pytest.fixture(params=[(), ('inner_self',)])
-def ignore_class(request):
-    return request.param
+def ignore_class(request): return request.param
 
 
 def append_class_args(builder, use_self):
     builder.append(ARGUMENTS)
     if not use_self:
         builder.append(lambda x: f'inner_self = {x}')
 
     builder.append(f'answer = {repr(ANSWER)}')
     builder.append(f'life = {repr(LIFE)}')
 
 
 class TestOnClassStr:
     @pytest.fixture
-    def t_class(self, different_str_levels, different_message_combos,
-                ignore_class):
+    def t_class(self, different_str_levels, different_message_combos, ignore_class):
         class Testy:
             @logs_vars(LOGGER, *ignore_class,
                        start_message=different_message_combos.start_message,
                        end_message=different_message_combos.end_message,
                        var_message_level=different_str_levels)
             def __init__(inner_self, answer, life):
                 inner_self.answer = answer
                 inner_self.life = life
 
-        return Testy, different_str_levels, different_message_combos, \
-               ignore_class
+        return Testy, different_str_levels, different_message_combos, ignore_class
 
     # Just making sure that it applies the decorator at least once.
     def test_not_break(self, t_class): pass
 
-    @pytest.fixture(params=[logging.DEBUG, logging.INFO, logging.WARNING,
-                            logging.ERROR, logging.CRITICAL])
+    @pytest.fixture(params=[logging.DEBUG, logging.INFO, logging.WARNING, logging.ERROR,
+                            logging.CRITICAL])
     def t_runs(self, request, t_class):
         if request.param == logging.DEBUG:
             builder = []
             if (t := t_class[2].start_message) is not None:
                 builder.append(t)
 
             append_class_args(builder, t_class[3])
@@ -128,33 +146,31 @@
         assert testy is not None
         assert testy.life == LIFE
         assert testy.answer == ANSWER
 
 
 class TestOnClassInt:
     @pytest.fixture
-    def t_class(self, different_int_levels, different_message_combos,
-                ignore_class):
+    def t_class(self, different_int_levels, different_message_combos, ignore_class):
         class Testy:
             @logs_vars(LOGGER, *ignore_class,
                        start_message=different_message_combos.start_message,
                        end_message=different_message_combos.end_message,
                        var_message_level=different_int_levels)
             def __init__(inner_self, answer, life):
                 inner_self.answer = answer
                 inner_self.life = life
 
-        return Testy, different_int_levels, different_message_combos, \
-               ignore_class
+        return Testy, different_int_levels, different_message_combos, ignore_class
 
     # Just making sure that it applies the decorator at least once.
     def test_not_break(self, t_class): pass
 
-    @pytest.fixture(params=[logging.DEBUG, logging.INFO, logging.WARNING,
-                            logging.ERROR, logging.CRITICAL])
+    @pytest.fixture(params=[logging.DEBUG, logging.INFO, logging.WARNING, logging.ERROR,
+                            logging.CRITICAL])
     def t_runs(self, request, t_class):
         if request.param == logging.DEBUG:
             builder = []
             if (t := t_class[2].start_message) is not None:
                 builder.append(t)
 
             append_class_args(builder, t_class[3])
@@ -197,30 +213,28 @@
     builder.append(ARGUMENTS)
     builder.append(f'name = {repr(NAME)}')
     builder.append(f'age = {repr(AGE)}')
 
 
 class TestFunctionStr:
     @pytest.fixture
-    def t_func(self, different_str_levels, different_message_combos,
-               ignore_class):
+    def t_func(self, different_str_levels, different_message_combos, ignore_class):
         @logs_vars(LOGGER, *ignore_class,
                    start_message=different_message_combos.start_message,
                    end_message=different_message_combos.end_message,
                    var_message_level=different_str_levels)
-        def testy(name, age):
-            return "Hi, I'm " + name + " and I'm " + str(age) + " years old."
+        def testy(name, age): return 'Hi, I\'m ' + name + ' and I\'m ' + str(age) + ' years old.'
 
         return testy, different_str_levels, different_message_combos
 
     # Just making sure that it applies the decorator at least once.
     def test_not_break(self, t_func): pass
 
-    @pytest.fixture(params=[logging.DEBUG, logging.INFO, logging.WARNING,
-                            logging.ERROR, logging.CRITICAL])
+    @pytest.fixture(params=[logging.DEBUG, logging.INFO, logging.WARNING, logging.ERROR,
+                            logging.CRITICAL])
     def t_runs(self, request, t_func):
         if request.param == logging.DEBUG:
             builder = []
             if (t := t_func[2].start_message) is not None:
                 builder.append(t)
 
             append_function_args(builder)
@@ -246,48 +260,47 @@
         for i in range(len(t_runs[2])):
             assert caplog.records[i].msg == t_runs[2][i]
 
     def test_result_unvoided(self, t_runs):
         LOGGER.setLevel(t_runs[1])
         ans = t_runs[0](NAME, AGE)
 
-        assert ans == f"Hi, I'm {NAME} and I'm {AGE} years old."
+        assert ans == f'Hi, I\'m {NAME} and I\'m {AGE} years old.'
 
     def test_logs_error(self, t_runs, caplog):
         caplog.set_level(logging.DEBUG)
 
         LOGGER.setLevel(logging.DEBUG)
         try:
             t_runs[0](BAD_NAME, AGE)
 
         except Exception as e:
             assert len(caplog.records) >= 2
-            assert caplog.records[-2].msg == 'A variable-logged function' \
-                                             ' failed to execute completely.'
+            assert caplog.records[-2].msg == ('A variable-logged function failed to execute '
+                                              'completely.')
             assert caplog.records[-1].msg == e
 
 
 class TestFunctionInt:
     @pytest.fixture
     def t_func(self, different_int_levels, different_message_combos,
                ignore_class):
         @logs_vars(LOGGER, *ignore_class,
                    start_message=different_message_combos.start_message,
                    end_message=different_message_combos.end_message,
                    var_message_level=different_int_levels)
-        def testy(name, age):
-            return "Hi, I'm " + name + " and I'm " + str(age) + " years old."
+        def testy(name, age): return 'Hi, I\'m ' + name + ' and I\'m ' + str(age) + ' years old.'
 
         return testy, different_int_levels, different_message_combos
 
     # Just making sure that it applies the decorator at least once.
     def test_not_break(self, t_func): pass
 
-    @pytest.fixture(params=[logging.DEBUG, logging.INFO, logging.WARNING,
-                            logging.ERROR, logging.CRITICAL])
+    @pytest.fixture(params=[logging.DEBUG, logging.INFO, logging.WARNING, logging.ERROR,
+                            logging.CRITICAL])
     def t_runs(self, request, t_func):
         if request.param == logging.DEBUG:
             builder = []
             if (t := t_func[2].start_message) is not None:
                 builder.append(t)
 
             append_function_args(builder)
@@ -309,25 +322,25 @@
         t_runs[0](NAME, AGE)
 
         assert len(caplog.records) == len(t_runs[2])
 
         for i in range(len(t_runs[2])):
             assert caplog.records[i].msg == t_runs[2][i]
 
-    def test_result_unvoided(self, t_runs):
+    def test_result_not_voided(self, t_runs):
         LOGGER.setLevel(t_runs[1])
         ans = t_runs[0](NAME, AGE)
 
-        assert ans == f"Hi, I'm {NAME} and I'm {AGE} years old."
+        assert ans == f'Hi, I\'m {NAME} and I\'m {AGE} years old.'
 
     def test_logs_error(self, t_runs, caplog):
         caplog.set_level(logging.DEBUG)
 
         LOGGER.setLevel(logging.DEBUG)
         try:
             t_runs[0](BAD_NAME, AGE)
 
         except Exception as e:
             assert len(caplog.records) >= 2
-            assert caplog.records[-2].msg == 'A variable-logged function' \
-                                             ' failed to execute completely.'
+            assert caplog.records[-2].msg == ('A variable-logged function failed to execute '
+                                              'completely.')
             assert caplog.records[-1].msg == e
```

