# Comparing `tmp/pyopenweathermap-0.0.8.tar.gz` & `tmp/pyopenweathermap-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopenweathermap-0.0.8.tar", max compression
+gzip compressed data, was "pyopenweathermap-0.0.9.tar", max compression
```

## Comparing `pyopenweathermap-0.0.8.tar` & `pyopenweathermap-0.0.9.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1063 2024-04-24 19:46:22.666091 pyopenweathermap-0.0.8/LICENSE
--rw-r--r--   0        0        0       77 2024-04-24 19:48:45.962832 pyopenweathermap-0.0.8/README.md
--rw-r--r--   0        0        0      568 2024-04-30 10:38:47.796234 pyopenweathermap-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      232 2024-04-26 09:04:44.323164 pyopenweathermap-0.0.8/src/pyopenweathermap/__init__.py
--rw-r--r--   0        0        0      143 2024-04-25 14:39:05.904017 pyopenweathermap-0.0.8/src/pyopenweathermap/exception.py
--rw-r--r--   0        0        0     3228 2024-04-30 10:38:43.544211 pyopenweathermap-0.0.8/src/pyopenweathermap/owm_client.py
--rw-r--r--   0        0        0     2534 2024-04-26 13:33:43.405295 pyopenweathermap-0.0.8/src/pyopenweathermap/weather.py
--rw-r--r--   0        0        0      593 1970-01-01 00:00:00.000000 pyopenweathermap-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-24 19:46:22.666091 pyopenweathermap-0.0.9/LICENSE
+-rw-r--r--   0        0        0       77 2024-04-24 19:48:45.962832 pyopenweathermap-0.0.9/README.md
+-rw-r--r--   0        0        0      547 2024-05-05 13:46:18.414796 pyopenweathermap-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      267 2024-05-05 12:28:04.334847 pyopenweathermap-0.0.9/src/pyopenweathermap/__init__.py
+-rw-r--r--   0        0        0     3230 2024-05-05 12:54:19.117186 pyopenweathermap-0.0.9/src/pyopenweathermap/data_converter.py
+-rw-r--r--   0        0        0      143 2024-04-25 14:39:05.904017 pyopenweathermap-0.0.9/src/pyopenweathermap/exception.py
+-rw-r--r--   0        0        0     3779 2024-05-05 12:28:04.334847 pyopenweathermap-0.0.9/src/pyopenweathermap/owm_client.py
+-rw-r--r--   0        0        0     1896 2024-05-05 12:28:04.334847 pyopenweathermap-0.0.9/src/pyopenweathermap/weather.py
+-rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 pyopenweathermap-0.0.9/PKG-INFO
```

### Comparing `pyopenweathermap-0.0.8/LICENSE` & `pyopenweathermap-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyopenweathermap-0.0.8/pyproject.toml` & `pyopenweathermap-0.0.9/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [tool.poetry]
 name = "pyopenweathermap"
-version = "0.0.8"
+version = "0.0.9"
 description = "lib for OpenWeatherMap for Home Assistant"
 authors = ["Evgeny <iam@freekode.org>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["homeassistant", "owm", "openweathermap"]
 packages = [
     { include = "pyopenweathermap", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 aiohttp = "^3.9.5"
-pydantic = "^1.10.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 pytest-asyncio = "^0.23.6"
 
 [build-system]
```

