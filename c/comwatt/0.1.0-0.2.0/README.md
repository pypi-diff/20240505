# Comparing `tmp/comwatt-0.1.0.tar.gz` & `tmp/comwatt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comwatt-0.1.0.tar", last modified: Sun Apr 16 19:15:23 2023, max compression
+gzip compressed data, was "comwatt-0.2.0.tar", last modified: Sun May  5 16:57:08 2024, max compression
```

## Comparing `comwatt-0.1.0.tar` & `comwatt-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 christophe  (1000) christophe  (1000)        0 2023-04-16 19:15:23.512564 comwatt-0.1.0/
--rw-r--r--   0 christophe  (1000) christophe  (1000)     1074 2023-04-15 15:46:41.000000 comwatt-0.1.0/LICENSE
--rw-r--r--   0 christophe  (1000) christophe  (1000)      254 2023-04-16 19:15:23.512564 comwatt-0.1.0/PKG-INFO
-drwxr-xr-x   0 christophe  (1000) christophe  (1000)        0 2023-04-16 19:15:23.512564 comwatt-0.1.0/comwatt/
--rwxr-xr-x   0 christophe  (1000) christophe  (1000)     3836 2023-04-15 15:47:02.000000 comwatt-0.1.0/comwatt/__init__.py
-drwxr-xr-x   0 christophe  (1000) christophe  (1000)        0 2023-04-16 19:15:23.512564 comwatt-0.1.0/comwatt.egg-info/
--rw-r--r--   0 christophe  (1000) christophe  (1000)      254 2023-04-16 19:15:23.000000 comwatt-0.1.0/comwatt.egg-info/PKG-INFO
--rw-r--r--   0 christophe  (1000) christophe  (1000)      205 2023-04-16 19:15:23.000000 comwatt-0.1.0/comwatt.egg-info/SOURCES.txt
--rw-r--r--   0 christophe  (1000) christophe  (1000)        1 2023-04-16 19:15:23.000000 comwatt-0.1.0/comwatt.egg-info/dependency_links.txt
--rw-r--r--   0 christophe  (1000) christophe  (1000)        9 2023-04-16 19:15:23.000000 comwatt-0.1.0/comwatt.egg-info/requires.txt
--rw-r--r--   0 christophe  (1000) christophe  (1000)        8 2023-04-16 19:15:23.000000 comwatt-0.1.0/comwatt.egg-info/top_level.txt
--rw-r--r--   0 christophe  (1000) christophe  (1000)       81 2023-04-16 19:12:44.000000 comwatt-0.1.0/pyproject.toml
--rw-r--r--   0 christophe  (1000) christophe  (1000)       38 2023-04-16 19:15:23.512564 comwatt-0.1.0/setup.cfg
--rw-r--r--   0 christophe  (1000) christophe  (1000)      375 2023-04-16 18:42:46.000000 comwatt-0.1.0/setup.py
+drwxr-xr-x   0 christophe  (1000) christophe  (1000)        0 2024-05-05 16:57:08.960744 comwatt-0.2.0/
+-rw-r--r--   0 christophe  (1000) christophe  (1000)     1074 2023-04-15 15:46:41.000000 comwatt-0.2.0/LICENSE
+-rw-r--r--   0 christophe  (1000) christophe  (1000)      273 2024-05-05 16:57:08.960744 comwatt-0.2.0/PKG-INFO
+drwxr-xr-x   0 christophe  (1000) christophe  (1000)        0 2024-05-05 16:57:08.960744 comwatt-0.2.0/comwatt/
+-rwxr-xr-x   0 christophe  (1000) christophe  (1000)     4341 2024-05-04 19:08:31.000000 comwatt-0.2.0/comwatt/__init__.py
+drwxr-xr-x   0 christophe  (1000) christophe  (1000)        0 2024-05-05 16:57:08.960744 comwatt-0.2.0/comwatt.egg-info/
+-rw-r--r--   0 christophe  (1000) christophe  (1000)      273 2024-05-05 16:57:08.000000 comwatt-0.2.0/comwatt.egg-info/PKG-INFO
+-rw-r--r--   0 christophe  (1000) christophe  (1000)      205 2024-05-05 16:57:08.000000 comwatt-0.2.0/comwatt.egg-info/SOURCES.txt
+-rw-r--r--   0 christophe  (1000) christophe  (1000)        1 2024-05-05 16:57:08.000000 comwatt-0.2.0/comwatt.egg-info/dependency_links.txt
+-rw-r--r--   0 christophe  (1000) christophe  (1000)        9 2024-05-05 16:57:08.000000 comwatt-0.2.0/comwatt.egg-info/requires.txt
+-rw-r--r--   0 christophe  (1000) christophe  (1000)        8 2024-05-05 16:57:08.000000 comwatt-0.2.0/comwatt.egg-info/top_level.txt
+-rw-r--r--   0 christophe  (1000) christophe  (1000)       81 2023-04-16 19:12:44.000000 comwatt-0.2.0/pyproject.toml
+-rw-r--r--   0 christophe  (1000) christophe  (1000)       38 2024-05-05 16:57:08.960744 comwatt-0.2.0/setup.cfg
+-rw-r--r--   0 christophe  (1000) christophe  (1000)      370 2024-05-05 16:56:44.000000 comwatt-0.2.0/setup.py
```

### Comparing `comwatt-0.1.0/LICENSE` & `comwatt-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `comwatt-0.1.0/comwatt/__init__.py` & `comwatt-0.2.0/comwatt/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import re
+
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.firefox.options import Options
 from selenium.webdriver.support.wait import WebDriverWait
 
 
@@ -37,54 +39,71 @@
         self.zone = None
         self.value_instant = 0
         self.initialized = False
 
 
 class PowerGEN4(webdriver.Firefox):
 
-    def __init__(self, debug):
+    def __init__(self, debug = False):
 
         options = Options()
 
         if not debug:
             options.add_argument("-headless")
 
         super().__init__(options=options)
     
         self.zones = []
 
+        self.default_site = None
+
     def login(self, email, password):
 
+        # Get the login page
         self.get('https://energy.comwatt.com/#/login/')
 
         WebDriverWait(self, timeout=20).until(lambda d: d.find_element(By.NAME, 'email'))
 
         elem = self.find_element(By.NAME, 'email')  # Find the search box
         elem.send_keys(email + Keys.RETURN)
 
         elem = self.find_element(By.NAME, 'password')  # Find the search box
         elem.send_keys(password + Keys.RETURN)
 
-    def meter(self):
+        # Wait home page
+        WebDriverWait(self, timeout=20).until(lambda d: d.find_element(By.CLASS_NAME, 'css-3kduam'))
+
+        m = re.match("https://energy.comwatt.com/#/sites/([abcdef0123456789]+)/home", self.current_url)
+        
+        self.default_site = m.group(1)
 
-        self.get('https://energy.comwatt.com/#/sites/a9d0ef7b/meter/')
+
+    def meter(self, site=None):
+
+        if not site:
+            site = self.default_site
+
+        self.get('https://energy.comwatt.com/#/sites/%s/meter/' % site)
         WebDriverWait(self, timeout=20).until(lambda d: d.find_element(By.CLASS_NAME, 'css-3kduam'))
 
         elem = self.find_element(By.CLASS_NAME, 'css-3kduam')
 
         data = elem.text
         assert data[-1] == "%"
         assert data[:-1].isdigit()
         return int(data[:-1])
 
-    def devices(self):
+    def devices(self, site=None):
+
+        if not site:
+            site = self.default_site
 
         self.zones = []
 
-        self.get('https://energy.comwatt.com/#/sites/a9d0ef7b/devices/')
+        self.get('https://energy.comwatt.com/#/sites/%s/devices/' % site)
         WebDriverWait(self, timeout=20).until(lambda d: d.find_element(By.CLASS_NAME, 'ZoneDevices-item'))
 
         for elt_zone in self.find_elements(By.CLASS_NAME, 'ZoneDevices-item'): 
 
             elem_title = elt_zone.find_element(By.CLASS_NAME, 'css-2bb7pl')
             zone = Zone(elem_title.text)
```

