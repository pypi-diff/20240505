# Comparing `tmp/appthreat_chen-2.0.9.tar.gz` & `tmp/appthreat_chen-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appthreat_chen-2.0.9.tar", max compression
+gzip compressed data, was "appthreat_chen-2.1.0.tar", max compression
```

## Comparing `appthreat_chen-2.0.9.tar` & `appthreat_chen-2.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    12015 2024-04-29 10:57:54.663668 appthreat_chen-2.0.9/LICENSE
--rw-r--r--   0        0        0     9479 2024-04-29 10:57:54.663668 appthreat_chen-2.0.9/README.md
--rw-r--r--   0        0        0       85 2024-04-29 10:57:54.663668 appthreat_chen-2.0.9/chenpy/__init__.py
--rw-r--r--   0        0        0     9509 2024-04-29 10:57:54.663668 appthreat_chen-2.0.9/chenpy/cli.py
--rw-r--r--   0        0        0    15364 2024-04-29 10:57:54.663668 appthreat_chen-2.0.9/chenpy/client.py
--rw-r--r--   0        0        0      256 2024-04-29 10:57:54.663668 appthreat_chen-2.0.9/chenpy/config.py
--rw-r--r--   0        0        0       61 2024-04-29 10:57:54.663668 appthreat_chen-2.0.9/chenpy/detectors/__init__.py
--rw-r--r--   0        0        0      999 2024-04-29 10:57:54.663668 appthreat_chen-2.0.9/chenpy/detectors/c.py
--rw-r--r--   0        0        0    15079 2024-04-29 10:57:54.667668 appthreat_chen-2.0.9/chenpy/detectors/common.py
--rw-r--r--   0        0        0     6052 2024-04-29 10:57:54.667668 appthreat_chen-2.0.9/chenpy/detectors/java.py
--rw-r--r--   0        0        0     5077 2024-04-29 10:57:54.667668 appthreat_chen-2.0.9/chenpy/detectors/js.py
--rw-r--r--   0        0        0     2311 2024-04-29 10:57:54.667668 appthreat_chen-2.0.9/chenpy/detectors/python.py
--rw-r--r--   0        0        0    13262 2024-04-29 10:57:54.667668 appthreat_chen-2.0.9/chenpy/graph.py
--rw-r--r--   0        0        0     2100 2024-04-29 10:57:54.667668 appthreat_chen-2.0.9/chenpy/logger.py
--rw-r--r--   0        0        0        0 2024-04-29 10:57:54.667668 appthreat_chen-2.0.9/chenpy/source/__init__.py
--rw-r--r--   0        0        0     4002 2024-04-29 10:57:54.667668 appthreat_chen-2.0.9/chenpy/source/ghsa.py
--rw-r--r--   0        0        0    30127 2024-04-29 10:57:54.667668 appthreat_chen-2.0.9/chenpy/utils.py
--rw-r--r--   0        0        0     6496 2024-04-29 10:57:54.667668 appthreat_chen-2.0.9/chenpy/workspace.py
--rw-r--r--   0        0        0     2554 2024-04-29 10:57:54.755667 appthreat_chen-2.0.9/pyproject.toml
--rw-r--r--   0        0        0    11004 1970-01-01 00:00:00.000000 appthreat_chen-2.0.9/PKG-INFO
+-rw-r--r--   0        0        0    12015 2024-05-05 12:09:49.150955 appthreat_chen-2.1.0/LICENSE
+-rw-r--r--   0        0        0     9479 2024-05-05 12:09:49.150955 appthreat_chen-2.1.0/README.md
+-rw-r--r--   0        0        0       85 2024-05-05 12:09:49.150955 appthreat_chen-2.1.0/chenpy/__init__.py
+-rw-r--r--   0        0        0     9509 2024-05-05 12:09:49.150955 appthreat_chen-2.1.0/chenpy/cli.py
+-rw-r--r--   0        0        0    15364 2024-05-05 12:09:49.150955 appthreat_chen-2.1.0/chenpy/client.py
+-rw-r--r--   0        0        0      256 2024-05-05 12:09:49.150955 appthreat_chen-2.1.0/chenpy/config.py
+-rw-r--r--   0        0        0       61 2024-05-05 12:09:49.150955 appthreat_chen-2.1.0/chenpy/detectors/__init__.py
+-rw-r--r--   0        0        0      999 2024-05-05 12:09:49.150955 appthreat_chen-2.1.0/chenpy/detectors/c.py
+-rw-r--r--   0        0        0    15079 2024-05-05 12:09:49.150955 appthreat_chen-2.1.0/chenpy/detectors/common.py
+-rw-r--r--   0        0        0     6052 2024-05-05 12:09:49.150955 appthreat_chen-2.1.0/chenpy/detectors/java.py
+-rw-r--r--   0        0        0     5077 2024-05-05 12:09:49.150955 appthreat_chen-2.1.0/chenpy/detectors/js.py
+-rw-r--r--   0        0        0     2311 2024-05-05 12:09:49.150955 appthreat_chen-2.1.0/chenpy/detectors/python.py
+-rw-r--r--   0        0        0    13262 2024-05-05 12:09:49.150955 appthreat_chen-2.1.0/chenpy/graph.py
+-rw-r--r--   0        0        0     2100 2024-05-05 12:09:49.150955 appthreat_chen-2.1.0/chenpy/logger.py
+-rw-r--r--   0        0        0        0 2024-05-05 12:09:49.150955 appthreat_chen-2.1.0/chenpy/source/__init__.py
+-rw-r--r--   0        0        0     4002 2024-05-05 12:09:49.150955 appthreat_chen-2.1.0/chenpy/source/ghsa.py
+-rw-r--r--   0        0        0    30127 2024-05-05 12:09:49.154955 appthreat_chen-2.1.0/chenpy/utils.py
+-rw-r--r--   0        0        0     6496 2024-05-05 12:09:49.154955 appthreat_chen-2.1.0/chenpy/workspace.py
+-rw-r--r--   0        0        0     2554 2024-05-05 12:09:49.238955 appthreat_chen-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0    11004 1970-01-01 00:00:00.000000 appthreat_chen-2.1.0/PKG-INFO
```

### Comparing `appthreat_chen-2.0.9/LICENSE` & `appthreat_chen-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `appthreat_chen-2.0.9/README.md` & `appthreat_chen-2.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
 Once the download finishes, the command will display the download location along with the environment variables that need to be set to invoke `chennai` console. Example output below:
 
 ```shell
 [21:53:36] INFO     To run chennai console, add the following environment variables to your .zshrc or .bashrc:
 export JAVA_OPTS="-Xmx16G"
 export JAVA_TOOL_OPTIONS="-Dfile.encoding=UTF-8 -Djna.library.path=<lib dir>"
-export SCALAPY_PYTHON_LIBRARY=python3.11
+export SCALAPY_PYTHON_LIBRARY=python3.12
 export CHEN_HOME=/home/user/.local/share/chen
 export PATH=$PATH:/home/user/.local/share/chen/platform:/home/user/.local/share/chen/platform/bin:
 ```
 
 It is important to set these environment variables without which the console commands would fail with errors.
 
 ## Running the console
@@ -178,15 +178,15 @@
   | misspelt or if an import is missing.
    -----------------------------------------------------------------------------
 1 error found
 ```
 
 This error is mostly due to missing python .so (linux), .dll (windows) or .dylib (mac) file. Ensure the environment variables below are set correctly.
 
-- SCALAPY_PYTHON_LIBRARY - Use values such as python3.10, python3.11 based on the version installed. On Windows, there are no dots. python311
+- SCALAPY_PYTHON_LIBRARY - Use values such as python3.10, python3.11 based on the version installed. On Windows, there are no dots. python312
 - JAVA_TOOL_OPTIONS - jna.library.path must be set to the python lib directory
 - SCALAPY_PYTHON_PROGRAMNAME - Path to Python executable in case of virtual environments (Usually not required)
 
 ## Origin of chen
 
 chen is a fork of the popular [joern](https://github.com/joernio/joern) project. We deviate from the joern project in the following ways:
```

### Comparing `appthreat_chen-2.0.9/chenpy/cli.py` & `appthreat_chen-2.1.0/chenpy/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,19 +174,19 @@
     Install the required science modules
     """
     if check_command("conda"):
         LOG.info(
             "About to install the science pack using conda. A new environment called 'chenpy-local' will be created."
         )
         with Progress(transient=True) as progress:
-            conda_install_script = """conda create --name chenpy-local python=3.11 -y
+            conda_install_script = """conda create --name chenpy-local python=3.12 -y
 conda install -n chenpy-local conda-libmamba-solver -y
 conda install -n chenpy-local -c conda-forge networkx --solver=libmamba -y
 conda install -n chenpy-local -c pytorch pytorch torchtext cpuonly --solver=libmamba -y
-pip install pyg_lib -f https://data.pyg.org/whl/torch-2.1.0+cpu.html
+pip install pyg_lib -f https://data.pyg.org/whl/torch-2.3.0+cpu.html
 conda install -n chenpy-local -c conda-forge scipy numpy packageurl-python nbconvert jupyter_core jupyter_client notebook --solver=libmamba -y
 conda install -n chenpy-local -c conda-forge oras-py==0.1.26 httpx websockets orjson rich appdirs psutil gitpython --solver=libmamba -y"""
             for line in conda_install_script.split("\n"):
                 if line.strip():
                     task = progress.add_task(line, start=False, total=100)
                     subprocess.check_call(
                         line.split(" "),
```

### Comparing `appthreat_chen-2.0.9/chenpy/client.py` & `appthreat_chen-2.1.0/chenpy/client.py`

 * *Files identical despite different names*

### Comparing `appthreat_chen-2.0.9/chenpy/detectors/c.py` & `appthreat_chen-2.1.0/chenpy/detectors/c.py`

 * *Files identical despite different names*

### Comparing `appthreat_chen-2.0.9/chenpy/detectors/common.py` & `appthreat_chen-2.1.0/chenpy/detectors/common.py`

 * *Files identical despite different names*

### Comparing `appthreat_chen-2.0.9/chenpy/detectors/java.py` & `appthreat_chen-2.1.0/chenpy/detectors/java.py`

 * *Files identical despite different names*

### Comparing `appthreat_chen-2.0.9/chenpy/detectors/js.py` & `appthreat_chen-2.1.0/chenpy/detectors/js.py`

 * *Files identical despite different names*

### Comparing `appthreat_chen-2.0.9/chenpy/detectors/python.py` & `appthreat_chen-2.1.0/chenpy/detectors/python.py`

 * *Files identical despite different names*

### Comparing `appthreat_chen-2.0.9/chenpy/graph.py` & `appthreat_chen-2.1.0/chenpy/graph.py`

 * *Files identical despite different names*

### Comparing `appthreat_chen-2.0.9/chenpy/logger.py` & `appthreat_chen-2.1.0/chenpy/logger.py`

 * *Files identical despite different names*

### Comparing `appthreat_chen-2.0.9/chenpy/source/ghsa.py` & `appthreat_chen-2.1.0/chenpy/source/ghsa.py`

 * *Files identical despite different names*

### Comparing `appthreat_chen-2.0.9/chenpy/utils.py` & `appthreat_chen-2.1.0/chenpy/utils.py`

 * *Files identical despite different names*

### Comparing `appthreat_chen-2.0.9/chenpy/workspace.py` & `appthreat_chen-2.1.0/chenpy/workspace.py`

 * *Files identical despite different names*

### Comparing `appthreat_chen-2.0.9/pyproject.toml` & `appthreat_chen-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "appthreat-chen"
-version = "2.0.9"
+version = "2.1.0"
 description = "Code Hierarchy Exploration Net (chen)"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "chenpy"}]
 homepage = "https://github.com/AppThreat/chen"
 repository = "https://github.com/AppThreat/chen"
@@ -71,15 +71,15 @@
 notebook = "^7.1.3"
 
 [tool.poetry.group.database.dependencies]
 networkx = {extras = ["default", "extra"], version = "^3.1"}
 
 [[tool.poetry.source]]
 name = "pyg"
-url = "https://data.pyg.org/whl/torch-2.1.0+cpu.html"
+url = "https://data.pyg.org/whl/torch-2.3.0+cpu.html"
 priority = "explicit"
 
 
 [[tool.poetry.source]]
 name = "torch"
 url = "https://download.pytorch.org/whl/cpu"
 priority = "explicit"
```

### Comparing `appthreat_chen-2.0.9/PKG-INFO` & `appthreat_chen-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appthreat-chen
-Version: 2.0.9
+Version: 2.1.0
 Summary: Code Hierarchy Exploration Net (chen)
 Home-page: https://github.com/AppThreat/chen
 License: Apache-2.0
 Keywords: chen,code-analysis,static-analysis
 Author: Team AppThreat
 Author-email: cloud@appthreat.com
 Requires-Python: >=3.10,<3.13
@@ -114,15 +114,15 @@
 
 Once the download finishes, the command will display the download location along with the environment variables that need to be set to invoke `chennai` console. Example output below:
 
 ```shell
 [21:53:36] INFO     To run chennai console, add the following environment variables to your .zshrc or .bashrc:
 export JAVA_OPTS="-Xmx16G"
 export JAVA_TOOL_OPTIONS="-Dfile.encoding=UTF-8 -Djna.library.path=<lib dir>"
-export SCALAPY_PYTHON_LIBRARY=python3.11
+export SCALAPY_PYTHON_LIBRARY=python3.12
 export CHEN_HOME=/home/user/.local/share/chen
 export PATH=$PATH:/home/user/.local/share/chen/platform:/home/user/.local/share/chen/platform/bin:
 ```
 
 It is important to set these environment variables without which the console commands would fail with errors.
 
 ## Running the console
@@ -215,15 +215,15 @@
   | misspelt or if an import is missing.
    -----------------------------------------------------------------------------
 1 error found
 ```
 
 This error is mostly due to missing python .so (linux), .dll (windows) or .dylib (mac) file. Ensure the environment variables below are set correctly.
 
-- SCALAPY_PYTHON_LIBRARY - Use values such as python3.10, python3.11 based on the version installed. On Windows, there are no dots. python311
+- SCALAPY_PYTHON_LIBRARY - Use values such as python3.10, python3.11 based on the version installed. On Windows, there are no dots. python312
 - JAVA_TOOL_OPTIONS - jna.library.path must be set to the python lib directory
 - SCALAPY_PYTHON_PROGRAMNAME - Path to Python executable in case of virtual environments (Usually not required)
 
 ## Origin of chen
 
 chen is a fork of the popular [joern](https://github.com/joernio/joern) project. We deviate from the joern project in the following ways:
```

