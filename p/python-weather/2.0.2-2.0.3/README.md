# Comparing `tmp/python_weather-2.0.2.tar.gz` & `tmp/python_weather-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_weather-2.0.2.tar", last modified: Thu Apr 25 16:44:59 2024, max compression
+gzip compressed data, was "python_weather-2.0.3.tar", last modified: Sun May  5 08:24:47 2024, max compression
```

## Comparing `python_weather-2.0.2.tar` & `python_weather-2.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 16:44:59.950542 python_weather-2.0.2/
--rw-rw-rw-   0        0        0     1080 2024-04-25 12:21:32.000000 python_weather-2.0.2/LICENSE
--rw-rw-rw-   0        0        0      181 2024-04-25 12:21:32.000000 python_weather-2.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3702 2024-04-25 16:44:59.950542 python_weather-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1892 2024-04-25 12:38:46.000000 python_weather-2.0.2/README.md
--rw-rw-rw-   0        0        0     1592 2024-04-25 16:20:00.000000 python_weather-2.0.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-25 16:44:59.809916 python_weather-2.0.2/python_weather/
--rw-rw-rw-   0        0        0      439 2024-04-25 16:20:30.000000 python_weather-2.0.2/python_weather/__init__.py
--rw-rw-rw-   0        0        0     3875 2024-04-25 12:21:32.000000 python_weather-2.0.2/python_weather/base.py
--rw-rw-rw-   0        0        0     3998 2024-04-25 12:21:32.000000 python_weather-2.0.2/python_weather/client.py
--rw-rw-rw-   0        0        0      912 2024-04-25 12:21:32.000000 python_weather-2.0.2/python_weather/constants.py
--rw-rw-rw-   0        0        0     9679 2024-04-25 12:21:32.000000 python_weather-2.0.2/python_weather/enums.py
--rw-rw-rw-   0        0        0      126 2024-04-25 12:21:32.000000 python_weather-2.0.2/python_weather/errors.py
--rw-rw-rw-   0        0        0     8681 2024-04-25 12:21:32.000000 python_weather-2.0.2/python_weather/forecast.py
-drwxrwxrwx   0        0        0        0 2024-04-25 16:44:59.950542 python_weather-2.0.2/python_weather.egg-info/
--rw-rw-rw-   0        0        0     3702 2024-04-25 16:44:59.000000 python_weather-2.0.2/python_weather.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      412 2024-04-25 16:44:59.000000 python_weather-2.0.2/python_weather.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 16:44:59.000000 python_weather-2.0.2/python_weather.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-25 16:44:59.000000 python_weather-2.0.2/python_weather.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-25 16:44:59.000000 python_weather-2.0.2/python_weather.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 16:44:59.950542 python_weather-2.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-05 08:24:47.811486 python_weather-2.0.3/
+-rw-rw-rw-   0        0        0     1080 2024-04-25 12:21:32.000000 python_weather-2.0.3/LICENSE
+-rw-rw-rw-   0        0        0      181 2024-04-25 12:21:32.000000 python_weather-2.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3702 2024-05-05 08:24:47.808472 python_weather-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1892 2024-04-25 12:38:46.000000 python_weather-2.0.3/README.md
+-rw-rw-rw-   0        0        0     1592 2024-05-05 08:04:47.000000 python_weather-2.0.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-05 08:24:47.729470 python_weather-2.0.3/python_weather/
+-rw-rw-rw-   0        0        0      439 2024-05-05 08:04:55.000000 python_weather-2.0.3/python_weather/__init__.py
+-rw-rw-rw-   0        0        0     3875 2024-04-25 12:21:32.000000 python_weather-2.0.3/python_weather/base.py
+-rw-rw-rw-   0        0        0     3932 2024-05-05 07:56:30.000000 python_weather-2.0.3/python_weather/client.py
+-rw-rw-rw-   0        0        0      912 2024-05-05 07:02:51.000000 python_weather-2.0.3/python_weather/constants.py
+-rw-rw-rw-   0        0        0     9679 2024-05-05 07:06:06.000000 python_weather-2.0.3/python_weather/enums.py
+-rw-rw-rw-   0        0        0      126 2024-04-25 12:21:32.000000 python_weather-2.0.3/python_weather/errors.py
+-rw-rw-rw-   0        0        0     8681 2024-04-25 12:21:32.000000 python_weather-2.0.3/python_weather/forecast.py
+drwxrwxrwx   0        0        0        0 2024-05-05 08:24:47.803471 python_weather-2.0.3/python_weather.egg-info/
+-rw-rw-rw-   0        0        0     3702 2024-05-05 08:24:47.000000 python_weather-2.0.3/python_weather.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      412 2024-05-05 08:24:47.000000 python_weather-2.0.3/python_weather.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 08:24:47.000000 python_weather-2.0.3/python_weather.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-05 08:24:47.000000 python_weather-2.0.3/python_weather.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-05 08:24:47.000000 python_weather-2.0.3/python_weather.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-05 08:24:47.812473 python_weather-2.0.3/setup.cfg
```

### Comparing `python_weather-2.0.2/LICENSE` & `python_weather-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_weather-2.0.2/PKG-INFO` & `python_weather-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-weather
-Version: 2.0.2
+Version: 2.0.3
 Summary: A free and asynchronous weather API wrapper made in Python, for Python.
 Author: null8626
 License: MIT
 Project-URL: Donations, https://ko-fi.com/null8626
 Project-URL: Changelog, https://python-weather.readthedocs.io/en/latest/changelog.html
 Project-URL: Homepage, https://python-weather.readthedocs.io/en/latest/
 Project-URL: Documentation, https://python-weather.readthedocs.io/en/latest/
```

### Comparing `python_weather-2.0.2/README.md` & `python_weather-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `python_weather-2.0.2/pyproject.toml` & `python_weather-2.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 
 [project]
 name = "python-weather"
-version = "2.0.2"
+version = "2.0.3"
 description = "A free and asynchronous weather API wrapper made in Python, for Python."
 readme = "README.md"
 license = { text = "MIT" }
 authors = [{ name = "null8626" }]
 keywords = ["weather", "forecast", "weather-api", "weather-forecast"]
 dependencies = ["aiohttp==3.9.5"]
 classifiers = [
```

### Comparing `python_weather-2.0.2/python_weather/base.py` & `python_weather-2.0.3/python_weather/base.py`

 * *Files identical despite different names*

### Comparing `python_weather-2.0.2/python_weather/client.py` & `python_weather-2.0.3/python_weather/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,31 +75,28 @@
     if not isinstance(unit, _Unit):
       unit = self._CustomizableBase__unit
 
     if not isinstance(locale, Locale):
       locale = self._CustomizableBase__locale
 
     subdomain = f'{locale.value}.' if locale != Locale.ENGLISH else ''
-    delay = 0
+    delay = 0.5
 
     while True:
-      if delay != 0:
-        await sleep(delay)
-        delay *= 2
-
       async with self.__session.get(
         f'https://{subdomain}wttr.in/{quote_plus(location)}?format=j1'
       ) as resp:
         try:
           return Forecast(await resp.json(), unit, locale)
         except Exception as e:
-          if delay == 4:
+          if delay == 2:
             raise e  # okay, that's too much requests - just raise the error
-          elif delay == 0:
-            delay = 0.5
+
+          await sleep(delay)
+          delay *= 2
 
   async def close(self):
     """Closes the :class:`Client` object. Nothing will happen if it's already closed."""
 
     if not self.__session.closed:
       await self.__session.close()
```

### Comparing `python_weather-2.0.2/python_weather/constants.py` & `python_weather-2.0.3/python_weather/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,9 +31,9 @@
   def __repr__(self) -> str:
     return f'<Unit [{self.temperature}, {self.velocity}]>'
 
 
 METRIC = _Unit('C', 'Kmph', '', 'MM', '', 1)
 IMPERIAL = _Unit('F', 'Miles', 'Inches', 'Inches', 'Miles', 2.54)
 
-WIND_DIRECTION_EMOJIS = ['↓', '↙', '←', '↖', '↑', '↗', '→', '↘']
+WIND_DIRECTION_EMOJIS = ('↓', '↙', '←', '↖', '↑', '↗', '→', '↘')
 LATLON_REGEX = compile(r'^Lat (\-?[\d\.]+) and Lon (\-?[\d\.]+)$')
```

### Comparing `python_weather-2.0.2/python_weather/enums.py` & `python_weather-2.0.3/python_weather/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,15 +398,15 @@
 
     if self is self.NEW_MOON:
       return '🌑'
     elif self is self.WAXING_CRESCENT:
       return '🌒'
     elif self is self.FIRST_QUARTER:
       return '🌓'
-    elif self is self.Waxing_GIBBOUS:
+    elif self is self.WAXING_GIBBOUS:
       return '🌔'
     elif self is self.FULL_MOON:
       return '🌕'
     elif self is self.WANING_GIBBOUS:
       return '🌖'
     elif self is self.LAST_QUARTER:
       return '🌗'
```

### Comparing `python_weather-2.0.2/python_weather/forecast.py` & `python_weather-2.0.3/python_weather/forecast.py`

 * *Files identical despite different names*

### Comparing `python_weather-2.0.2/python_weather.egg-info/PKG-INFO` & `python_weather-2.0.3/python_weather.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-weather
-Version: 2.0.2
+Version: 2.0.3
 Summary: A free and asynchronous weather API wrapper made in Python, for Python.
 Author: null8626
 License: MIT
 Project-URL: Donations, https://ko-fi.com/null8626
 Project-URL: Changelog, https://python-weather.readthedocs.io/en/latest/changelog.html
 Project-URL: Homepage, https://python-weather.readthedocs.io/en/latest/
 Project-URL: Documentation, https://python-weather.readthedocs.io/en/latest/
```

