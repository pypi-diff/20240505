# Comparing `tmp/sphinxcontrib_lightbox2-0.1.1.tar.gz` & `tmp/sphinxcontrib_lightbox2-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib_lightbox2-0.1.1.tar", max compression
+gzip compressed data, was "sphinxcontrib_lightbox2-0.2.0.tar", max compression
```

## Comparing `sphinxcontrib_lightbox2-0.1.1.tar` & `sphinxcontrib_lightbox2-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      667 2024-05-04 18:47:26.840399 sphinxcontrib_lightbox2-0.1.1/README.md
--rw-r--r--   0        0        0     1289 2024-05-04 18:47:26.840399 sphinxcontrib_lightbox2-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4591 2024-05-04 18:47:26.840399 sphinxcontrib_lightbox2-0.1.1/sphinxcontrib/lightbox2/__init__.py
--rw-r--r--   0        0        0     2532 2024-05-04 18:47:26.840399 sphinxcontrib_lightbox2-0.1.1/sphinxcontrib/lightbox2/assets/css/lightbox.min.css
--rw-r--r--   0        0        0      280 2024-05-04 18:47:26.840399 sphinxcontrib_lightbox2-0.1.1/sphinxcontrib/lightbox2/assets/images/close.png
--rw-r--r--   0        0        0     8476 2024-05-04 18:47:26.840399 sphinxcontrib_lightbox2-0.1.1/sphinxcontrib/lightbox2/assets/images/loading.gif
--rw-r--r--   0        0        0     1350 2024-05-04 18:47:26.840399 sphinxcontrib_lightbox2-0.1.1/sphinxcontrib/lightbox2/assets/images/next.png
--rw-r--r--   0        0        0     1360 2024-05-04 18:47:26.840399 sphinxcontrib_lightbox2-0.1.1/sphinxcontrib/lightbox2/assets/images/prev.png
--rw-r--r--   0        0        0   100774 2024-05-04 18:47:26.840399 sphinxcontrib_lightbox2-0.1.1/sphinxcontrib/lightbox2/assets/js/lightbox-plus-jquery.min.js
--rw-r--r--   0        0        0   147284 2024-05-04 18:47:26.844399 sphinxcontrib_lightbox2-0.1.1/sphinxcontrib/lightbox2/assets/js/lightbox-plus-jquery.min.map
--rw-r--r--   0        0        0        0 2024-05-04 18:47:26.844399 sphinxcontrib_lightbox2-0.1.1/sphinxcontrib/lightbox2/py.typed
--rw-r--r--   0        0        0     1327 1970-01-01 00:00:00.000000 sphinxcontrib_lightbox2-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1811 2024-05-04 19:43:46.137811 sphinxcontrib_lightbox2-0.2.0/README.md
+-rw-r--r--   0        0        0     1289 2024-05-04 19:43:46.137811 sphinxcontrib_lightbox2-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6819 2024-05-04 19:43:46.137811 sphinxcontrib_lightbox2-0.2.0/sphinxcontrib/lightbox2/__init__.py
+-rw-r--r--   0        0        0     2532 2024-05-04 19:43:46.137811 sphinxcontrib_lightbox2-0.2.0/sphinxcontrib/lightbox2/assets/css/lightbox.min.css
+-rw-r--r--   0        0        0      280 2024-05-04 19:43:46.137811 sphinxcontrib_lightbox2-0.2.0/sphinxcontrib/lightbox2/assets/images/close.png
+-rw-r--r--   0        0        0     8476 2024-05-04 19:43:46.137811 sphinxcontrib_lightbox2-0.2.0/sphinxcontrib/lightbox2/assets/images/loading.gif
+-rw-r--r--   0        0        0     1350 2024-05-04 19:43:46.137811 sphinxcontrib_lightbox2-0.2.0/sphinxcontrib/lightbox2/assets/images/next.png
+-rw-r--r--   0        0        0     1360 2024-05-04 19:43:46.137811 sphinxcontrib_lightbox2-0.2.0/sphinxcontrib/lightbox2/assets/images/prev.png
+-rw-r--r--   0        0        0   100774 2024-05-04 19:43:46.141811 sphinxcontrib_lightbox2-0.2.0/sphinxcontrib/lightbox2/assets/js/lightbox-plus-jquery.min.js
+-rw-r--r--   0        0        0   147284 2024-05-04 19:43:46.141811 sphinxcontrib_lightbox2-0.2.0/sphinxcontrib/lightbox2/assets/js/lightbox-plus-jquery.min.map
+-rw-r--r--   0        0        0        0 2024-05-04 19:43:46.141811 sphinxcontrib_lightbox2-0.2.0/sphinxcontrib/lightbox2/py.typed
+-rw-r--r--   0        0        0     2471 1970-01-01 00:00:00.000000 sphinxcontrib_lightbox2-0.2.0/PKG-INFO
```

### Comparing `sphinxcontrib_lightbox2-0.1.1/pyproject.toml` & `sphinxcontrib_lightbox2-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphinxcontrib-lightbox2"
-version = "0.1.1"
+version = "0.2.0"
 description = "Sphinx extension to add lightbox2 to each figure and image added in HTML"
 authors = ["Jonas Ehrlich <jonas.ehrlich@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://sphinxcontrib-lightbox2.readthedocs.io/"
 packages = [{ include = "sphinxcontrib" }]
```

### Comparing `sphinxcontrib_lightbox2-0.1.1/sphinxcontrib/lightbox2/assets/css/lightbox.min.css` & `sphinxcontrib_lightbox2-0.2.0/sphinxcontrib/lightbox2/assets/css/lightbox.min.css`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_lightbox2-0.1.1/sphinxcontrib/lightbox2/assets/images/loading.gif` & `sphinxcontrib_lightbox2-0.2.0/sphinxcontrib/lightbox2/assets/images/loading.gif`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_lightbox2-0.1.1/sphinxcontrib/lightbox2/assets/images/next.png` & `sphinxcontrib_lightbox2-0.2.0/sphinxcontrib/lightbox2/assets/images/next.png`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_lightbox2-0.1.1/sphinxcontrib/lightbox2/assets/images/prev.png` & `sphinxcontrib_lightbox2-0.2.0/sphinxcontrib/lightbox2/assets/images/prev.png`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_lightbox2-0.1.1/sphinxcontrib/lightbox2/assets/js/lightbox-plus-jquery.min.js` & `sphinxcontrib_lightbox2-0.2.0/sphinxcontrib/lightbox2/assets/js/lightbox-plus-jquery.min.js`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_lightbox2-0.1.1/sphinxcontrib/lightbox2/assets/js/lightbox-plus-jquery.min.map` & `sphinxcontrib_lightbox2-0.2.0/sphinxcontrib/lightbox2/assets/js/lightbox-plus-jquery.min.map`

 * *Files identical despite different names*

