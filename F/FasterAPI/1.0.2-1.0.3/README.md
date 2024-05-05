# Comparing `tmp/fasterapi-1.0.2.tar.gz` & `tmp/fasterapi-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fasterapi-1.0.2.tar", max compression
+gzip compressed data, was "fasterapi-1.0.3.tar", max compression
```

## Comparing `fasterapi-1.0.2.tar` & `fasterapi-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     6953 2024-05-05 09:54:31.561607 fasterapi-1.0.2/FasterAPI/__init__.py
--rw-r--r--   0        0        0       90 2024-05-05 09:58:17.606890 fasterapi-1.0.2/FasterAPI/__main__.py
--rw-r--r--   0        0        0      191 2024-05-05 09:54:31.562608 fasterapi-1.0.2/FasterAPI/cli/__init__.py
--rw-r--r--   0        0        0     7762 2024-05-05 09:54:31.562608 fasterapi-1.0.2/FasterAPI/cli/module.py
--rw-r--r--   0        0        0     5072 2024-05-05 09:54:31.563608 fasterapi-1.0.2/FasterAPI/cli/project.py
--rw-r--r--   0        0        0      877 2024-05-05 09:54:31.563608 fasterapi-1.0.2/FasterAPI/cli/templates/config.yaml.j2
--rw-r--r--   0        0        0      751 2024-05-05 09:54:31.564607 fasterapi-1.0.2/FasterAPI/cli/templates/module/__init__.py.j2
--rw-r--r--   0        0        0      150 2024-05-05 09:54:31.564607 fasterapi-1.0.2/FasterAPI/cli/templates/module/config.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-05 09:54:31.565610 fasterapi-1.0.2/FasterAPI/cli/templates/module/dependencies.py.j2
--rw-r--r--   0        0        0      932 2024-05-05 09:54:31.566041 fasterapi-1.0.2/FasterAPI/cli/templates/module/router.py.j2
--rw-r--r--   0        0        0      240 2024-05-05 09:54:31.566041 fasterapi-1.0.2/FasterAPI/cli/templates/module/schema.py.j2
--rw-r--r--   0        0        0      737 2024-05-05 09:54:31.566041 fasterapi-1.0.2/FasterAPI/cli/templates/module/utils.py.j2
--rw-r--r--   0        0        0      260 2024-05-05 09:54:31.567056 fasterapi-1.0.2/FasterAPI/cli/templates/serve.py.j2
--rw-r--r--   0        0        0     2921 2024-05-05 09:54:31.567056 fasterapi-1.0.2/FasterAPI/cli/templates/user/__init__.py.j2
--rw-r--r--   0        0        0      424 2024-05-05 09:54:31.568055 fasterapi-1.0.2/FasterAPI/cli/templates/user/config.yaml.j2
--rw-r--r--   0        0        0     3305 2024-05-05 09:54:31.569064 fasterapi-1.0.2/FasterAPI/cli/templates/user/dependencies.py.j2
--rw-r--r--   0        0        0     8394 2024-05-05 09:54:31.569064 fasterapi-1.0.2/FasterAPI/cli/templates/user/router.py.j2
--rw-r--r--   0        0        0      908 2024-05-05 09:54:31.570054 fasterapi-1.0.2/FasterAPI/cli/templates/user/schemas.py.j2
--rw-r--r--   0        0        0     6058 2024-05-05 09:54:31.570054 fasterapi-1.0.2/FasterAPI/cli/templates/user/utils.py.j2
--rw-r--r--   0        0        0      965 2024-05-05 09:58:21.836850 fasterapi-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     3603 2024-03-22 03:27:35.126041 fasterapi-1.0.2/README.md
--rw-r--r--   0        0        0     4759 1970-01-01 00:00:00.000000 fasterapi-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     6953 2024-05-05 09:54:31.561607 fasterapi-1.0.3/FasterAPI/__init__.py
+-rw-r--r--   0        0        0       90 2024-05-05 09:58:17.606890 fasterapi-1.0.3/FasterAPI/__main__.py
+-rw-r--r--   0        0        0      191 2024-05-05 09:54:31.562608 fasterapi-1.0.3/FasterAPI/cli/__init__.py
+-rw-r--r--   0        0        0     7762 2024-05-05 09:54:31.562608 fasterapi-1.0.3/FasterAPI/cli/module.py
+-rw-r--r--   0        0        0     5072 2024-05-05 09:54:31.563608 fasterapi-1.0.3/FasterAPI/cli/project.py
+-rw-r--r--   0        0        0      877 2024-05-05 09:54:31.563608 fasterapi-1.0.3/FasterAPI/cli/templates/config.yaml.j2
+-rw-r--r--   0        0        0      751 2024-05-05 09:54:31.564607 fasterapi-1.0.3/FasterAPI/cli/templates/module/__init__.py.j2
+-rw-r--r--   0        0        0      150 2024-05-05 09:54:31.564607 fasterapi-1.0.3/FasterAPI/cli/templates/module/config.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-05 09:54:31.565610 fasterapi-1.0.3/FasterAPI/cli/templates/module/dependencies.py.j2
+-rw-r--r--   0        0        0      932 2024-05-05 09:54:31.566041 fasterapi-1.0.3/FasterAPI/cli/templates/module/router.py.j2
+-rw-r--r--   0        0        0      240 2024-05-05 09:54:31.566041 fasterapi-1.0.3/FasterAPI/cli/templates/module/schema.py.j2
+-rw-r--r--   0        0        0      737 2024-05-05 09:54:31.566041 fasterapi-1.0.3/FasterAPI/cli/templates/module/utils.py.j2
+-rw-r--r--   0        0        0      260 2024-05-05 09:54:31.567056 fasterapi-1.0.3/FasterAPI/cli/templates/serve.py.j2
+-rw-r--r--   0        0        0     2921 2024-05-05 09:54:31.567056 fasterapi-1.0.3/FasterAPI/cli/templates/user/__init__.py.j2
+-rw-r--r--   0        0        0      424 2024-05-05 09:54:31.568055 fasterapi-1.0.3/FasterAPI/cli/templates/user/config.yaml.j2
+-rw-r--r--   0        0        0     3305 2024-05-05 09:54:31.569064 fasterapi-1.0.3/FasterAPI/cli/templates/user/dependencies.py.j2
+-rw-r--r--   0        0        0     8394 2024-05-05 09:54:31.569064 fasterapi-1.0.3/FasterAPI/cli/templates/user/router.py.j2
+-rw-r--r--   0        0        0      908 2024-05-05 09:54:31.570054 fasterapi-1.0.3/FasterAPI/cli/templates/user/schemas.py.j2
+-rw-r--r--   0        0        0     6058 2024-05-05 09:54:31.570054 fasterapi-1.0.3/FasterAPI/cli/templates/user/utils.py.j2
+-rw-r--r--   0        0        0      984 2024-05-05 10:01:27.153898 fasterapi-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3603 2024-03-22 03:27:35.126041 fasterapi-1.0.3/README.md
+-rw-r--r--   0        0        0     4798 1970-01-01 00:00:00.000000 fasterapi-1.0.3/PKG-INFO
```

### Comparing `fasterapi-1.0.2/FasterAPI/__init__.py` & `fasterapi-1.0.3/FasterAPI/__init__.py`

 * *Files identical despite different names*

### Comparing `fasterapi-1.0.2/FasterAPI/cli/module.py` & `fasterapi-1.0.3/FasterAPI/cli/module.py`

 * *Files identical despite different names*

### Comparing `fasterapi-1.0.2/FasterAPI/cli/project.py` & `fasterapi-1.0.3/FasterAPI/cli/project.py`

 * *Files identical despite different names*

### Comparing `fasterapi-1.0.2/FasterAPI/cli/templates/config.yaml.j2` & `fasterapi-1.0.3/FasterAPI/cli/templates/config.yaml.j2`

 * *Files identical despite different names*

### Comparing `fasterapi-1.0.2/FasterAPI/cli/templates/module/__init__.py.j2` & `fasterapi-1.0.3/FasterAPI/cli/templates/module/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `fasterapi-1.0.2/FasterAPI/cli/templates/module/router.py.j2` & `fasterapi-1.0.3/FasterAPI/cli/templates/module/router.py.j2`

 * *Files identical despite different names*

### Comparing `fasterapi-1.0.2/FasterAPI/cli/templates/module/utils.py.j2` & `fasterapi-1.0.3/FasterAPI/cli/templates/module/utils.py.j2`

 * *Files identical despite different names*

### Comparing `fasterapi-1.0.2/FasterAPI/cli/templates/user/__init__.py.j2` & `fasterapi-1.0.3/FasterAPI/cli/templates/user/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `fasterapi-1.0.2/FasterAPI/cli/templates/user/dependencies.py.j2` & `fasterapi-1.0.3/FasterAPI/cli/templates/user/dependencies.py.j2`

 * *Files identical despite different names*

### Comparing `fasterapi-1.0.2/FasterAPI/cli/templates/user/router.py.j2` & `fasterapi-1.0.3/FasterAPI/cli/templates/user/router.py.j2`

 * *Files identical despite different names*

### Comparing `fasterapi-1.0.2/FasterAPI/cli/templates/user/schemas.py.j2` & `fasterapi-1.0.3/FasterAPI/cli/templates/user/schemas.py.j2`

 * *Files identical despite different names*

### Comparing `fasterapi-1.0.2/FasterAPI/cli/templates/user/utils.py.j2` & `fasterapi-1.0.3/FasterAPI/cli/templates/user/utils.py.j2`

 * *Files identical despite different names*

### Comparing `fasterapi-1.0.2/pyproject.toml` & `fasterapi-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "FasterAPI"
-version = "1.0.2"
+version = "1.0.3"
 description = ""
 authors = ["ulfaric <ryf0510@live.com>"]
 readme = "README.md"
 urls = { github = "https://github.com/ulfaric/FasterAPI/issues", documentation = "https://ulfaric.github.io/FasterAPI/" }
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -17,14 +17,15 @@
 opentelemetry-sdk = "^1.23.0"
 opentelemetry-api = "^1.23.0"
 opentelemetry-instrumentation = "^0.44b0"
 opentelemetry-instrumentation-fastapi = "^0.44b0"
 opentelemetry-exporter-jaeger = "^1.21.0"
 typer = {extras = ["all"], version = "^0.10.0"}
 alembic = "^1.13.1"
+pyyaml = "^6.0.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
```

### Comparing `fasterapi-1.0.2/README.md` & `fasterapi-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fasterapi-1.0.2/PKG-INFO` & `fasterapi-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FasterAPI
-Version: 1.0.2
+Version: 1.0.3
 Summary: 
 Author: ulfaric
 Author-email: ryf0510@live.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -18,14 +18,15 @@
 Requires-Dist: opentelemetry-api (>=1.23.0,<2.0.0)
 Requires-Dist: opentelemetry-exporter-jaeger (>=1.21.0,<2.0.0)
 Requires-Dist: opentelemetry-instrumentation (>=0.44b0,<0.45)
 Requires-Dist: opentelemetry-instrumentation-fastapi (>=0.44b0,<0.45)
 Requires-Dist: opentelemetry-sdk (>=1.23.0,<2.0.0)
 Requires-Dist: passlib[bcrypt] (>=1.7.4,<2.0.0)
 Requires-Dist: python-jose[cryptography] (>=3.3.0,<4.0.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: sqlalchemy (>=2.0.28,<3.0.0)
 Requires-Dist: typer[all] (>=0.10.0,<0.11.0)
 Project-URL: documentation, https://ulfaric.github.io/FasterAPI/
 Project-URL: github, https://github.com/ulfaric/FasterAPI/issues
 Description-Content-Type: text/markdown
 
 # FasterAPI
```

