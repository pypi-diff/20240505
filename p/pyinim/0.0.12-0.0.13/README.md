# Comparing `tmp/pyinim-0.0.12.tar.gz` & `tmp/pyinim-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinim-0.0.12.tar", last modified: Sun May  5 13:15:02 2024, max compression
+gzip compressed data, was "pyinim-0.0.13.tar", last modified: Sun May  5 13:41:00 2024, max compression
```

## Comparing `pyinim-0.0.12.tar` & `pyinim-0.0.13.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 bertulla (1473677006) 52240112        0 2024-05-05 13:15:02.930033 pyinim-0.0.12/
--rw-r--r--   0 bertulla (1473677006) 52240112    35149 2024-04-27 20:46:49.000000 pyinim-0.0.12/LICENSE
--rw-r--r--   0 bertulla (1473677006) 52240112     3318 2024-05-05 13:15:02.929940 pyinim-0.0.12/PKG-INFO
--rw-r--r--   0 bertulla (1473677006) 52240112     2693 2024-05-05 13:13:10.000000 pyinim-0.0.12/README.md
--rw-r--r--   0 bertulla (1473677006) 52240112      621 2024-05-05 13:13:10.000000 pyinim-0.0.12/pyproject.toml
--rw-r--r--   0 bertulla (1473677006) 52240112      418 2024-05-05 13:15:02.930280 pyinim-0.0.12/setup.cfg
-drwxr-xr-x   0 bertulla (1473677006) 52240112        0 2024-05-05 13:15:02.926796 pyinim-0.0.12/src/
-drwxr-xr-x   0 bertulla (1473677006) 52240112        0 2024-05-05 13:15:02.929643 pyinim-0.0.12/src/pyinim.egg-info/
--rw-r--r--   0 bertulla (1473677006) 52240112     3318 2024-05-05 13:15:02.000000 pyinim-0.0.12/src/pyinim.egg-info/PKG-INFO
--rw-r--r--   0 bertulla (1473677006) 52240112      571 2024-05-05 13:15:02.000000 pyinim-0.0.12/src/pyinim.egg-info/SOURCES.txt
--rw-r--r--   0 bertulla (1473677006) 52240112        1 2024-05-05 13:15:02.000000 pyinim-0.0.12/src/pyinim.egg-info/dependency_links.txt
--rw-r--r--   0 bertulla (1473677006) 52240112       53 2024-05-05 13:15:02.000000 pyinim-0.0.12/src/pyinim.egg-info/requires.txt
--rw-r--r--   0 bertulla (1473677006) 52240112       14 2024-05-05 13:15:02.000000 pyinim-0.0.12/src/pyinim.egg-info/top_level.txt
-drwxr-xr-x   0 bertulla (1473677006) 52240112        0 2024-05-05 13:15:02.928378 pyinim-0.0.12/src/pyinim_nidble/
--rw-r--r--   0 bertulla (1473677006) 52240112        0 2024-04-27 20:46:49.000000 pyinim-0.0.12/src/pyinim_nidble/__init__.py
-drwxr-xr-x   0 bertulla (1473677006) 52240112        0 2024-05-05 13:15:02.928772 pyinim-0.0.12/src/pyinim_nidble/cloud/
--rw-r--r--   0 bertulla (1473677006) 52240112        0 2024-04-27 20:46:49.000000 pyinim-0.0.12/src/pyinim_nidble/cloud/__init__.py
--rw-r--r--   0 bertulla (1473677006) 52240112     2215 2024-05-05 13:11:55.000000 pyinim-0.0.12/src/pyinim_nidble/cloud/abc.py
--rw-r--r--   0 bertulla (1473677006) 52240112     2169 2024-05-05 13:11:55.000000 pyinim-0.0.12/src/pyinim_nidble/cloud/resolver.py
-drwxr-xr-x   0 bertulla (1473677006) 52240112        0 2024-05-05 13:15:02.929183 pyinim-0.0.12/src/pyinim_nidble/cloud/types/
--rw-r--r--   0 bertulla (1473677006) 52240112        0 2024-04-27 20:46:49.000000 pyinim-0.0.12/src/pyinim_nidble/cloud/types/__init__.py
--rw-r--r--   0 bertulla (1473677006) 52240112     2304 2024-04-27 20:46:49.000000 pyinim-0.0.12/src/pyinim_nidble/cloud/types/devices.py
--rw-r--r--   0 bertulla (1473677006) 52240112      489 2024-04-27 20:46:49.000000 pyinim-0.0.12/src/pyinim_nidble/cloud/types/token.py
-drwxr-xr-x   0 bertulla (1473677006) 52240112        0 2024-05-05 13:15:02.929457 pyinim-0.0.12/src/pyinim_nidble/examples/
--rw-r--r--   0 bertulla (1473677006) 52240112        0 2024-04-28 08:28:37.000000 pyinim-0.0.12/src/pyinim_nidble/examples/__init__.py
--rw-r--r--   0 bertulla (1473677006) 52240112     1390 2024-05-05 13:11:55.000000 pyinim-0.0.12/src/pyinim_nidble/examples/poc.py
--rw-r--r--   0 bertulla (1473677006) 52240112     1584 2024-05-05 13:11:55.000000 pyinim-0.0.12/src/pyinim_nidble/inim_cloud.py
+drwxr-xr-x   0 bertulla (1473677006) 52240112        0 2024-05-05 13:41:00.680981 pyinim-0.0.13/
+-rw-r--r--   0 bertulla (1473677006) 52240112    35149 2024-04-27 20:46:49.000000 pyinim-0.0.13/LICENSE
+-rw-r--r--   0 bertulla (1473677006) 52240112     3318 2024-05-05 13:41:00.680911 pyinim-0.0.13/PKG-INFO
+-rw-r--r--   0 bertulla (1473677006) 52240112     2693 2024-05-05 13:40:54.000000 pyinim-0.0.13/README.md
+-rw-r--r--   0 bertulla (1473677006) 52240112      621 2024-05-05 13:40:54.000000 pyinim-0.0.13/pyproject.toml
+-rw-r--r--   0 bertulla (1473677006) 52240112      418 2024-05-05 13:41:00.681255 pyinim-0.0.13/setup.cfg
+drwxr-xr-x   0 bertulla (1473677006) 52240112        0 2024-05-05 13:41:00.675963 pyinim-0.0.13/src/
+drwxr-xr-x   0 bertulla (1473677006) 52240112        0 2024-05-05 13:41:00.680538 pyinim-0.0.13/src/pyinim.egg-info/
+-rw-r--r--   0 bertulla (1473677006) 52240112     3318 2024-05-05 13:41:00.000000 pyinim-0.0.13/src/pyinim.egg-info/PKG-INFO
+-rw-r--r--   0 bertulla (1473677006) 52240112      571 2024-05-05 13:41:00.000000 pyinim-0.0.13/src/pyinim.egg-info/SOURCES.txt
+-rw-r--r--   0 bertulla (1473677006) 52240112        1 2024-05-05 13:41:00.000000 pyinim-0.0.13/src/pyinim.egg-info/dependency_links.txt
+-rw-r--r--   0 bertulla (1473677006) 52240112       53 2024-05-05 13:41:00.000000 pyinim-0.0.13/src/pyinim.egg-info/requires.txt
+-rw-r--r--   0 bertulla (1473677006) 52240112       14 2024-05-05 13:41:00.000000 pyinim-0.0.13/src/pyinim.egg-info/top_level.txt
+drwxr-xr-x   0 bertulla (1473677006) 52240112        0 2024-05-05 13:41:00.678235 pyinim-0.0.13/src/pyinim_nidble/
+-rw-r--r--   0 bertulla (1473677006) 52240112        0 2024-04-27 20:46:49.000000 pyinim-0.0.13/src/pyinim_nidble/__init__.py
+drwxr-xr-x   0 bertulla (1473677006) 52240112        0 2024-05-05 13:41:00.679269 pyinim-0.0.13/src/pyinim_nidble/cloud/
+-rw-r--r--   0 bertulla (1473677006) 52240112        0 2024-04-27 20:46:49.000000 pyinim-0.0.13/src/pyinim_nidble/cloud/__init__.py
+-rw-r--r--   0 bertulla (1473677006) 52240112     2215 2024-05-05 13:11:55.000000 pyinim-0.0.13/src/pyinim_nidble/cloud/abc.py
+-rw-r--r--   0 bertulla (1473677006) 52240112     2169 2024-05-05 13:11:55.000000 pyinim-0.0.13/src/pyinim_nidble/cloud/resolver.py
+drwxr-xr-x   0 bertulla (1473677006) 52240112        0 2024-05-05 13:41:00.679914 pyinim-0.0.13/src/pyinim_nidble/cloud/types/
+-rw-r--r--   0 bertulla (1473677006) 52240112        0 2024-04-27 20:46:49.000000 pyinim-0.0.13/src/pyinim_nidble/cloud/types/__init__.py
+-rw-r--r--   0 bertulla (1473677006) 52240112     2304 2024-04-27 20:46:49.000000 pyinim-0.0.13/src/pyinim_nidble/cloud/types/devices.py
+-rw-r--r--   0 bertulla (1473677006) 52240112      489 2024-04-27 20:46:49.000000 pyinim-0.0.13/src/pyinim_nidble/cloud/types/token.py
+drwxr-xr-x   0 bertulla (1473677006) 52240112        0 2024-05-05 13:41:00.680177 pyinim-0.0.13/src/pyinim_nidble/examples/
+-rw-r--r--   0 bertulla (1473677006) 52240112        0 2024-04-28 08:28:37.000000 pyinim-0.0.13/src/pyinim_nidble/examples/__init__.py
+-rw-r--r--   0 bertulla (1473677006) 52240112     1390 2024-05-05 13:11:55.000000 pyinim-0.0.13/src/pyinim_nidble/examples/poc.py
+-rw-r--r--   0 bertulla (1473677006) 52240112     1584 2024-05-05 13:11:55.000000 pyinim-0.0.13/src/pyinim_nidble/inim_cloud.py
```

### Comparing `pyinim-0.0.12/LICENSE` & `pyinim-0.0.13/LICENSE`

 * *Files identical despite different names*

### Comparing `pyinim-0.0.12/PKG-INFO` & `pyinim-0.0.13/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinim
-Version: 0.0.12
+Version: 0.0.13
 Summary: A Inim Cloud API client
 Home-page: https://github.com/nidble/pyinim
 Author: Antonino Bertulla
 Author-email: Antonino Bertulla <abertulla@email.address>
 Project-URL: Homepage, https://github.com/nidble/pyinim
 Project-URL: Issues, https://github.com/nidble/pyinim/issues
 Classifier: Programming Language :: Python :: 3
@@ -22,15 +22,15 @@
 ## Usage
 
 ```sh
 python3 -m venv venv
 source venv/bin/activate.fish
 python3 -m pip install aiohttp==3.9.5
 # python3 -m pip install python-dotenv==1.0.1
-python3 -m pip install --index-url https://test.pypi.org/simple/ pyinim-nidble==0.0.12
+python3 -m pip install --index-url https://test.pypi.org/simple/ pyinim-nidble==0.0.13
 # python3 -m pip uninstall pyinim-nidble
 ```
 
 ## Development
 
 ### Environment preparation
 ```sh
```

### Comparing `pyinim-0.0.12/README.md` & `pyinim-0.0.13/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ## Usage
 
 ```sh
 python3 -m venv venv
 source venv/bin/activate.fish
 python3 -m pip install aiohttp==3.9.5
 # python3 -m pip install python-dotenv==1.0.1
-python3 -m pip install --index-url https://test.pypi.org/simple/ pyinim-nidble==0.0.12
+python3 -m pip install --index-url https://test.pypi.org/simple/ pyinim-nidble==0.0.13
 # python3 -m pip uninstall pyinim-nidble
 ```
 
 ## Development
 
 ### Environment preparation
 ```sh
```

### Comparing `pyinim-0.0.12/pyproject.toml` & `pyinim-0.0.13/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyinim"
-version = "0.0.12"
+version = "0.0.13"
 authors = [
   { name="Antonino Bertulla", email="abertulla@email.address" },
 ]
 description = "A Inim Cloud API client"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pyinim-0.0.12/src/pyinim.egg-info/PKG-INFO` & `pyinim-0.0.13/src/pyinim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinim
-Version: 0.0.12
+Version: 0.0.13
 Summary: A Inim Cloud API client
 Home-page: https://github.com/nidble/pyinim
 Author: Antonino Bertulla
 Author-email: Antonino Bertulla <abertulla@email.address>
 Project-URL: Homepage, https://github.com/nidble/pyinim
 Project-URL: Issues, https://github.com/nidble/pyinim/issues
 Classifier: Programming Language :: Python :: 3
@@ -22,15 +22,15 @@
 ## Usage
 
 ```sh
 python3 -m venv venv
 source venv/bin/activate.fish
 python3 -m pip install aiohttp==3.9.5
 # python3 -m pip install python-dotenv==1.0.1
-python3 -m pip install --index-url https://test.pypi.org/simple/ pyinim-nidble==0.0.12
+python3 -m pip install --index-url https://test.pypi.org/simple/ pyinim-nidble==0.0.13
 # python3 -m pip uninstall pyinim-nidble
 ```
 
 ## Development
 
 ### Environment preparation
 ```sh
```

### Comparing `pyinim-0.0.12/src/pyinim.egg-info/SOURCES.txt` & `pyinim-0.0.13/src/pyinim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyinim-0.0.12/src/pyinim_nidble/cloud/abc.py` & `pyinim-0.0.13/src/pyinim_nidble/cloud/abc.py`

 * *Files identical despite different names*

### Comparing `pyinim-0.0.12/src/pyinim_nidble/cloud/resolver.py` & `pyinim-0.0.13/src/pyinim_nidble/cloud/resolver.py`

 * *Files identical despite different names*

### Comparing `pyinim-0.0.12/src/pyinim_nidble/cloud/types/devices.py` & `pyinim-0.0.13/src/pyinim_nidble/cloud/types/devices.py`

 * *Files identical despite different names*

### Comparing `pyinim-0.0.12/src/pyinim_nidble/examples/poc.py` & `pyinim-0.0.13/src/pyinim_nidble/examples/poc.py`

 * *Files identical despite different names*

### Comparing `pyinim-0.0.12/src/pyinim_nidble/inim_cloud.py` & `pyinim-0.0.13/src/pyinim_nidble/inim_cloud.py`

 * *Files identical despite different names*

