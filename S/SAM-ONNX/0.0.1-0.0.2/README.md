# Comparing `tmp/sam_onnx-0.0.1.tar.gz` & `tmp/sam_onnx-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Work\work\SAM_ONNX\SAM_ONNX\dist\.tmp-giqqecsy\sam_onnx-0.0.1.tar", last modified: Sat May  4 17:20:29 2024, max compression
+gzip compressed data, was "sam_onnx-0.0.2.tar", last modified: Sun May  5 07:03:04 2024, max compression
```

## Comparing `sam_onnx-0.0.1.tar` & `sam_onnx-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 17:20:29.302179 sam_onnx-0.0.1/
--rw-rw-rw-   0        0        0      939 2024-05-04 17:20:29.301316 sam_onnx-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      303 2024-05-04 16:39:41.000000 sam_onnx-0.0.1/README.md
--rw-rw-rw-   0        0        0      676 2024-05-04 16:39:41.000000 sam_onnx-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-04 17:20:29.302179 sam_onnx-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-04 17:20:29.269294 sam_onnx-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-04 17:20:29.299247 sam_onnx-0.0.1/src/SAM_ONNX.egg-info/
--rw-rw-rw-   0        0        0      939 2024-05-04 17:20:29.000000 sam_onnx-0.0.1/src/SAM_ONNX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2024-05-04 17:20:29.000000 sam_onnx-0.0.1/src/SAM_ONNX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 17:20:29.000000 sam_onnx-0.0.1/src/SAM_ONNX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2024-05-04 17:20:29.000000 sam_onnx-0.0.1/src/SAM_ONNX.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-04 17:20:29.000000 sam_onnx-0.0.1/src/SAM_ONNX.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-04 17:20:29.298234 sam_onnx-0.0.1/src/sam_onnx/
--rw-rw-rw-   0        0        0       23 2024-05-04 16:39:41.000000 sam_onnx-0.0.1/src/sam_onnx/__init__.py
--rw-rw-rw-   0        0        0    21788 2024-05-04 16:39:41.000000 sam_onnx-0.0.1/src/sam_onnx/sam_onnx.py
+drwxrwxrwx   0        0        0        0 2024-05-05 07:03:04.203161 sam_onnx-0.0.2/
+-rw-rw-rw-   0        0        0     1118 2024-05-05 07:03:04.203161 sam_onnx-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2024-05-05 06:53:41.000000 sam_onnx-0.0.2/README.md
+-rw-rw-rw-   0        0        0      676 2024-05-05 07:02:51.000000 sam_onnx-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-05 07:03:04.203161 sam_onnx-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-05 07:03:04.185644 sam_onnx-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-05 07:03:04.203161 sam_onnx-0.0.2/src/SAM_ONNX.egg-info/
+-rw-rw-rw-   0        0        0     1118 2024-05-05 07:03:04.000000 sam_onnx-0.0.2/src/SAM_ONNX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2024-05-05 07:03:04.000000 sam_onnx-0.0.2/src/SAM_ONNX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 07:03:04.000000 sam_onnx-0.0.2/src/SAM_ONNX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2024-05-05 07:03:04.000000 sam_onnx-0.0.2/src/SAM_ONNX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-05 07:03:04.000000 sam_onnx-0.0.2/src/SAM_ONNX.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-05 07:03:04.203161 sam_onnx-0.0.2/src/sam_onnx/
+-rw-rw-rw-   0        0        0       23 2024-05-04 16:39:41.000000 sam_onnx-0.0.2/src/sam_onnx/__init__.py
+-rw-rw-rw-   0        0        0    21788 2024-05-04 16:39:41.000000 sam_onnx-0.0.2/src/sam_onnx/sam_onnx.py
```

### Comparing `sam_onnx-0.0.1/PKG-INFO` & `sam_onnx-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 Metadata-Version: 2.1
 Name: SAM_ONNX
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple package for using SAM (ONNX format) without pytorch dependencies
 Author-email: Girin Chutia <girin.iitm@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: matplotlib>=3.8.3
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: onnxruntime==1.17.1
 Requires-Dist: opencv_python==4.9.0.80
 Requires-Dist: gdown==5.1.0
 Provides-Extra: dev
 Requires-Dist: jupyter; extra == "dev"
 
 # SAM ONNX 
 
-## Environment creation
+## Installation
+Get started quickly with SAM ONNX! Install it via pip:
 
-> python -m venv sam_onnx_env
+```bash
+pip install SAM-ONNX
+```
 
-- Use pip 24.0 or higher version 
+Or from root SAM_ONNX folder run,
+```bash
+python -m pip install -e .
+```
 
-## Installation
-In SAM_ONNX Folder
-> python -m pip install -e .
+## Documentation
+
+[Documentation](https://girinchutia.github.io/SAM_ONNX/)
 
 ## Usage
-![alt text](repo_assests/demo.png)
+Checkout the below demo
+
+![demo](https://github.com/GirinChutia/SAM_ONNX/blob/main/repo_assests/demo.png)
 
 ## License
 
 This project is licensed under the [MIT License](LICENSE).
```

### Comparing `sam_onnx-0.0.1/pyproject.toml` & `sam_onnx-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "SAM_ONNX"
-version = "0.0.1"
+version = "0.0.2"
 description = "A simple package for using SAM (ONNX format) without pytorch dependencies"
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.8"
 dependencies = ["matplotlib>=3.8.3", "numpy>=1.26.4","onnxruntime==1.17.1","opencv_python==4.9.0.80","gdown==5.1.0"]
 authors = [{ name = "Girin Chutia", email = "girin.iitm@gmail.com" }]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `sam_onnx-0.0.1/src/SAM_ONNX.egg-info/PKG-INFO` & `sam_onnx-0.0.2/src/SAM_ONNX.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 Metadata-Version: 2.1
 Name: SAM_ONNX
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple package for using SAM (ONNX format) without pytorch dependencies
 Author-email: Girin Chutia <girin.iitm@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: matplotlib>=3.8.3
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: onnxruntime==1.17.1
 Requires-Dist: opencv_python==4.9.0.80
 Requires-Dist: gdown==5.1.0
 Provides-Extra: dev
 Requires-Dist: jupyter; extra == "dev"
 
 # SAM ONNX 
 
-## Environment creation
+## Installation
+Get started quickly with SAM ONNX! Install it via pip:
 
-> python -m venv sam_onnx_env
+```bash
+pip install SAM-ONNX
+```
 
-- Use pip 24.0 or higher version 
+Or from root SAM_ONNX folder run,
+```bash
+python -m pip install -e .
+```
 
-## Installation
-In SAM_ONNX Folder
-> python -m pip install -e .
+## Documentation
+
+[Documentation](https://girinchutia.github.io/SAM_ONNX/)
 
 ## Usage
-![alt text](repo_assests/demo.png)
+Checkout the below demo
+
+![demo](https://github.com/GirinChutia/SAM_ONNX/blob/main/repo_assests/demo.png)
 
 ## License
 
 This project is licensed under the [MIT License](LICENSE).
```

### Comparing `sam_onnx-0.0.1/src/sam_onnx/sam_onnx.py` & `sam_onnx-0.0.2/src/sam_onnx/sam_onnx.py`

 * *Files identical despite different names*

