# Comparing `tmp/fasterapi-1.0.1.tar.gz` & `tmp/fasterapi-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fasterapi-1.0.1.tar", max compression
+gzip compressed data, was "fasterapi-1.0.2.tar", max compression
```

## Comparing `fasterapi-1.0.1.tar` & `fasterapi-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     6953 2024-05-05 09:54:31.561607 fasterapi-1.0.1/FasterAPI/__init__.py
--rw-r--r--   0        0        0       65 2024-05-05 09:54:31.562608 fasterapi-1.0.1/FasterAPI/__main__.py
--rw-r--r--   0        0        0      191 2024-05-05 09:54:31.562608 fasterapi-1.0.1/FasterAPI/cli/__init__.py
--rw-r--r--   0        0        0     7762 2024-05-05 09:54:31.562608 fasterapi-1.0.1/FasterAPI/cli/module.py
--rw-r--r--   0        0        0     5072 2024-05-05 09:54:31.563608 fasterapi-1.0.1/FasterAPI/cli/project.py
--rw-r--r--   0        0        0      877 2024-05-05 09:54:31.563608 fasterapi-1.0.1/FasterAPI/cli/templates/config.yaml.j2
--rw-r--r--   0        0        0      751 2024-05-05 09:54:31.564607 fasterapi-1.0.1/FasterAPI/cli/templates/module/__init__.py.j2
--rw-r--r--   0        0        0      150 2024-05-05 09:54:31.564607 fasterapi-1.0.1/FasterAPI/cli/templates/module/config.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-05 09:54:31.565610 fasterapi-1.0.1/FasterAPI/cli/templates/module/dependencies.py.j2
--rw-r--r--   0        0        0      932 2024-05-05 09:54:31.566041 fasterapi-1.0.1/FasterAPI/cli/templates/module/router.py.j2
--rw-r--r--   0        0        0      240 2024-05-05 09:54:31.566041 fasterapi-1.0.1/FasterAPI/cli/templates/module/schema.py.j2
--rw-r--r--   0        0        0      737 2024-05-05 09:54:31.566041 fasterapi-1.0.1/FasterAPI/cli/templates/module/utils.py.j2
--rw-r--r--   0        0        0      260 2024-05-05 09:54:31.567056 fasterapi-1.0.1/FasterAPI/cli/templates/serve.py.j2
--rw-r--r--   0        0        0     2921 2024-05-05 09:54:31.567056 fasterapi-1.0.1/FasterAPI/cli/templates/user/__init__.py.j2
--rw-r--r--   0        0        0      424 2024-05-05 09:54:31.568055 fasterapi-1.0.1/FasterAPI/cli/templates/user/config.yaml.j2
--rw-r--r--   0        0        0     3305 2024-05-05 09:54:31.569064 fasterapi-1.0.1/FasterAPI/cli/templates/user/dependencies.py.j2
--rw-r--r--   0        0        0     8394 2024-05-05 09:54:31.569064 fasterapi-1.0.1/FasterAPI/cli/templates/user/router.py.j2
--rw-r--r--   0        0        0      908 2024-05-05 09:54:31.570054 fasterapi-1.0.1/FasterAPI/cli/templates/user/schemas.py.j2
--rw-r--r--   0        0        0     6058 2024-05-05 09:54:31.570054 fasterapi-1.0.1/FasterAPI/cli/templates/user/utils.py.j2
--rw-r--r--   0        0        0      956 2024-05-05 09:54:57.502346 fasterapi-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3603 2024-03-22 03:27:35.126041 fasterapi-1.0.1/README.md
--rw-r--r--   0        0        0     4759 1970-01-01 00:00:00.000000 fasterapi-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6953 2024-05-05 09:54:31.561607 fasterapi-1.0.2/FasterAPI/__init__.py
+-rw-r--r--   0        0        0       90 2024-05-05 09:58:17.606890 fasterapi-1.0.2/FasterAPI/__main__.py
+-rw-r--r--   0        0        0      191 2024-05-05 09:54:31.562608 fasterapi-1.0.2/FasterAPI/cli/__init__.py
+-rw-r--r--   0        0        0     7762 2024-05-05 09:54:31.562608 fasterapi-1.0.2/FasterAPI/cli/module.py
+-rw-r--r--   0        0        0     5072 2024-05-05 09:54:31.563608 fasterapi-1.0.2/FasterAPI/cli/project.py
+-rw-r--r--   0        0        0      877 2024-05-05 09:54:31.563608 fasterapi-1.0.2/FasterAPI/cli/templates/config.yaml.j2
+-rw-r--r--   0        0        0      751 2024-05-05 09:54:31.564607 fasterapi-1.0.2/FasterAPI/cli/templates/module/__init__.py.j2
+-rw-r--r--   0        0        0      150 2024-05-05 09:54:31.564607 fasterapi-1.0.2/FasterAPI/cli/templates/module/config.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-05 09:54:31.565610 fasterapi-1.0.2/FasterAPI/cli/templates/module/dependencies.py.j2
+-rw-r--r--   0        0        0      932 2024-05-05 09:54:31.566041 fasterapi-1.0.2/FasterAPI/cli/templates/module/router.py.j2
+-rw-r--r--   0        0        0      240 2024-05-05 09:54:31.566041 fasterapi-1.0.2/FasterAPI/cli/templates/module/schema.py.j2
+-rw-r--r--   0        0        0      737 2024-05-05 09:54:31.566041 fasterapi-1.0.2/FasterAPI/cli/templates/module/utils.py.j2
+-rw-r--r--   0        0        0      260 2024-05-05 09:54:31.567056 fasterapi-1.0.2/FasterAPI/cli/templates/serve.py.j2
+-rw-r--r--   0        0        0     2921 2024-05-05 09:54:31.567056 fasterapi-1.0.2/FasterAPI/cli/templates/user/__init__.py.j2
+-rw-r--r--   0        0        0      424 2024-05-05 09:54:31.568055 fasterapi-1.0.2/FasterAPI/cli/templates/user/config.yaml.j2
+-rw-r--r--   0        0        0     3305 2024-05-05 09:54:31.569064 fasterapi-1.0.2/FasterAPI/cli/templates/user/dependencies.py.j2
+-rw-r--r--   0        0        0     8394 2024-05-05 09:54:31.569064 fasterapi-1.0.2/FasterAPI/cli/templates/user/router.py.j2
+-rw-r--r--   0        0        0      908 2024-05-05 09:54:31.570054 fasterapi-1.0.2/FasterAPI/cli/templates/user/schemas.py.j2
+-rw-r--r--   0        0        0     6058 2024-05-05 09:54:31.570054 fasterapi-1.0.2/FasterAPI/cli/templates/user/utils.py.j2
+-rw-r--r--   0        0        0      965 2024-05-05 09:58:21.836850 fasterapi-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3603 2024-03-22 03:27:35.126041 fasterapi-1.0.2/README.md
+-rw-r--r--   0        0        0     4759 1970-01-01 00:00:00.000000 fasterapi-1.0.2/PKG-INFO
```

### Comparing `fasterapi-1.0.1/FasterAPI/__init__.py` & `fasterapi-1.0.2/FasterAPI/__init__.py`

 * *Files identical despite different names*

### Comparing `fasterapi-1.0.1/FasterAPI/cli/module.py` & `fasterapi-1.0.2/FasterAPI/cli/module.py`

 * *Files identical despite different names*

### Comparing `fasterapi-1.0.1/FasterAPI/cli/project.py` & `fasterapi-1.0.2/FasterAPI/cli/project.py`

 * *Files identical despite different names*

### Comparing `fasterapi-1.0.1/FasterAPI/cli/templates/config.yaml.j2` & `fasterapi-1.0.2/FasterAPI/cli/templates/config.yaml.j2`

 * *Files identical despite different names*

### Comparing `fasterapi-1.0.1/FasterAPI/cli/templates/module/__init__.py.j2` & `fasterapi-1.0.2/FasterAPI/cli/templates/module/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `fasterapi-1.0.1/FasterAPI/cli/templates/module/router.py.j2` & `fasterapi-1.0.2/FasterAPI/cli/templates/module/router.py.j2`

 * *Files identical despite different names*

### Comparing `fasterapi-1.0.1/FasterAPI/cli/templates/module/utils.py.j2` & `fasterapi-1.0.2/FasterAPI/cli/templates/module/utils.py.j2`

 * *Files identical despite different names*

### Comparing `fasterapi-1.0.1/FasterAPI/cli/templates/user/__init__.py.j2` & `fasterapi-1.0.2/FasterAPI/cli/templates/user/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `fasterapi-1.0.1/FasterAPI/cli/templates/user/dependencies.py.j2` & `fasterapi-1.0.2/FasterAPI/cli/templates/user/dependencies.py.j2`

 * *Files identical despite different names*

### Comparing `fasterapi-1.0.1/FasterAPI/cli/templates/user/router.py.j2` & `fasterapi-1.0.2/FasterAPI/cli/templates/user/router.py.j2`

 * *Files identical despite different names*

### Comparing `fasterapi-1.0.1/FasterAPI/cli/templates/user/schemas.py.j2` & `fasterapi-1.0.2/FasterAPI/cli/templates/user/schemas.py.j2`

 * *Files identical despite different names*

### Comparing `fasterapi-1.0.1/FasterAPI/cli/templates/user/utils.py.j2` & `fasterapi-1.0.2/FasterAPI/cli/templates/user/utils.py.j2`

 * *Files identical despite different names*

### Comparing `fasterapi-1.0.1/pyproject.toml` & `fasterapi-1.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "FasterAPI"
-version = "1.0.1"
+version = "1.0.2"
 description = ""
 authors = ["ulfaric <ryf0510@live.com>"]
 readme = "README.md"
 urls = { github = "https://github.com/ulfaric/FasterAPI/issues", documentation = "https://ulfaric.github.io/FasterAPI/" }
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -24,8 +24,8 @@
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-FasterAPI = "FasterAPI:main"
+FasterAPI = "FasterAPI.__main__:main"
```

### Comparing `fasterapi-1.0.1/README.md` & `fasterapi-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `fasterapi-1.0.1/PKG-INFO` & `fasterapi-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FasterAPI
-Version: 1.0.1
+Version: 1.0.2
 Summary: 
 Author: ulfaric
 Author-email: ryf0510@live.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

