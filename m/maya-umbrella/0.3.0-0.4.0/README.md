# Comparing `tmp/maya_umbrella-0.3.0.tar.gz` & `tmp/maya_umbrella-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maya_umbrella-0.3.0.tar", max compression
+gzip compressed data, was "maya_umbrella-0.4.0.tar", max compression
```

## Comparing `maya_umbrella-0.3.0.tar` & `maya_umbrella-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0     1060 2024-05-04 16:43:13.028399 maya_umbrella-0.3.0/LICENSE
--rw-r--r--   0        0        0     1767 2024-05-04 16:43:13.028399 maya_umbrella-0.3.0/README.md
--rw-r--r--   0        0        0       88 2024-05-04 16:43:13.052399 maya_umbrella-0.3.0/maya_umbrella/__init__.py
--rw-r--r--   0        0        0       22 2024-05-04 16:43:13.052399 maya_umbrella-0.3.0/maya_umbrella/__version__.py
--rw-r--r--   0        0        0     2512 2024-05-04 16:43:13.052399 maya_umbrella-0.3.0/maya_umbrella/core.py
--rw-r--r--   0        0        0     3434 2024-05-04 16:43:13.052399 maya_umbrella-0.3.0/maya_umbrella/filesystem.py
--rw-r--r--   0        0        0        0 2024-05-04 16:43:13.052399 maya_umbrella-0.3.0/maya_umbrella/hooks/__init__.py
--rw-r--r--   0        0        0      688 2024-05-04 16:43:13.052399 maya_umbrella-0.3.0/maya_umbrella/hooks/delete_turtle.py
--rw-r--r--   0        0        0     1170 2024-05-04 16:43:13.052399 maya_umbrella-0.3.0/maya_umbrella/hooks/delete_unknown_plugin_node.py
--rw-r--r--   0        0        0      513 2024-05-04 16:43:13.052399 maya_umbrella-0.3.0/maya_umbrella/hooks/fix_model_panel.py
--rw-r--r--   0        0        0      341 2024-05-04 16:43:13.052399 maya_umbrella-0.3.0/maya_umbrella/hooks/fix_on_model_change_3dc.py
--rw-r--r--   0        0        0     2045 2024-05-04 16:43:13.052399 maya_umbrella-0.3.0/maya_umbrella/vaccine.py
--rw-r--r--   0        0        0        0 2024-05-04 16:43:13.052399 maya_umbrella-0.3.0/maya_umbrella/vaccines/__init__.py
--rw-r--r--   0        0        0      460 2024-05-04 16:43:13.052399 maya_umbrella-0.3.0/maya_umbrella/vaccines/vaccine1.py
--rw-r--r--   0        0        0     2659 2024-05-04 16:43:13.052399 maya_umbrella-0.3.0/maya_umbrella/vaccines/vaccine2.py
--rw-r--r--   0        0        0     3756 2024-05-04 16:43:13.052399 maya_umbrella-0.3.0/maya_umbrella/vaccines/vaccine3.py
--rw-r--r--   0        0        0     2415 2024-05-04 16:43:13.052399 maya_umbrella-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2818 1970-01-01 00:00:00.000000 maya_umbrella-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-05-05 17:10:04.248802 maya_umbrella-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5624 2024-05-05 17:10:04.248802 maya_umbrella-0.4.0/README.md
+-rw-r--r--   0        0        0      106 2024-05-05 17:10:04.272802 maya_umbrella-0.4.0/maya_umbrella/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-05 17:10:04.272802 maya_umbrella-0.4.0/maya_umbrella/__version__.py
+-rw-r--r--   0        0        0      130 2024-05-05 17:10:04.272802 maya_umbrella-0.4.0/maya_umbrella/constants.py
+-rw-r--r--   0        0        0     4098 2024-05-05 17:10:04.272802 maya_umbrella-0.4.0/maya_umbrella/core.py
+-rw-r--r--   0        0        0     4140 2024-05-05 17:10:04.272802 maya_umbrella-0.4.0/maya_umbrella/filesystem.py
+-rw-r--r--   0        0        0        0 2024-05-05 17:10:04.272802 maya_umbrella-0.4.0/maya_umbrella/hooks/__init__.py
+-rw-r--r--   0        0        0      734 2024-05-05 17:10:04.272802 maya_umbrella-0.4.0/maya_umbrella/hooks/delete_turtle.py
+-rw-r--r--   0        0        0     1246 2024-05-05 17:10:04.272802 maya_umbrella-0.4.0/maya_umbrella/hooks/delete_unknown_plugin_node.py
+-rw-r--r--   0        0        0      546 2024-05-05 17:10:04.272802 maya_umbrella-0.4.0/maya_umbrella/hooks/fix_model_panel.py
+-rw-r--r--   0        0        0      457 2024-05-05 17:10:04.272802 maya_umbrella-0.4.0/maya_umbrella/hooks/fix_on_model_change_3dc.py
+-rw-r--r--   0        0        0     1338 2024-05-05 17:10:04.272802 maya_umbrella-0.4.0/maya_umbrella/log.py
+-rw-r--r--   0        0        0     7075 2024-05-05 17:10:04.272802 maya_umbrella-0.4.0/maya_umbrella/vaccine.py
+-rw-r--r--   0        0        0        0 2024-05-05 17:10:04.272802 maya_umbrella-0.4.0/maya_umbrella/vaccines/__init__.py
+-rw-r--r--   0        0        0      430 2024-05-05 17:10:04.272802 maya_umbrella-0.4.0/maya_umbrella/vaccines/vaccine1.py
+-rw-r--r--   0        0        0     2526 2024-05-05 17:10:04.272802 maya_umbrella-0.4.0/maya_umbrella/vaccines/vaccine2.py
+-rw-r--r--   0        0        0     3061 2024-05-05 17:10:04.272802 maya_umbrella-0.4.0/maya_umbrella/vaccines/vaccine3.py
+-rw-r--r--   0        0        0     3837 2024-05-05 17:10:04.272802 maya_umbrella-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6675 1970-01-01 00:00:00.000000 maya_umbrella-0.4.0/PKG-INFO
```

### Comparing `maya_umbrella-0.3.0/LICENSE` & `maya_umbrella-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.3.0/maya_umbrella/filesystem.py` & `maya_umbrella-0.4.0/maya_umbrella/filesystem.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,34 +2,38 @@
 import glob
 import importlib
 import io
 import os
 import random
 import shutil
 import string
+import tempfile
+
+# Import local modules
+from maya_umbrella.constants import PACKAGE_NAME
 
 
 def this_root():
     """Return the absolute path of the current file's directory."""
     return os.path.abspath(os.path.dirname(__file__))
 
 
 def safe_remove_file(file_path):
     """Remove the file at the given path without raising an error if the file does not exist."""
     try:
         os.remove(file_path)
-    except (IOError, OSError):
+    except OSError:
         pass
 
 
 def safe_rmtree(path):
     """Remove the directory at the given path without raising an error if the directory does not exist."""
     try:
         shutil.rmtree(path)
-    except (IOError, OSError):
+    except OSError:
         pass
 
 
 def read_file(path):
     """Read the content of the file at the given path."""
     with io.open(path, "r", encoding="utf-8") as file_:
         content = file_.read()
@@ -102,9 +106,41 @@
 def get_hooks():
     """Return a list of paths to all hook files in the 'hooks' directory."""
     pattern = os.path.join(this_root(), "hooks", "*.py")
     return [hook for hook in glob.glob(pattern) if "__init__" not in hook]
 
 
 def get_vaccines():
+    """
+    Get a list of all vaccine files.
+
+    Returns:
+        list: A list of vaccine files.
+    """
     pattern = os.path.join(this_root(), "vaccines", "*.py")
     return [vaccine for vaccine in glob.glob(pattern) if "__init__" not in vaccine]
+
+
+def get_log_root():
+    """
+    Get the log root directory.
+
+    Returns:
+        str: The log root directory.
+    """
+    return os.getenv("MAYA_UMBRELLA_LOG_ROOT", tempfile.gettempdir())
+
+
+def get_log_file():
+    """
+    Get the path of the log file.
+
+    Returns:
+        str: The path of the log file.
+    """
+    root = get_log_root()
+    try:
+        os.makedirs(root)
+    except OSError:
+        pass
+    name = os.getenv("MAYA_UMBRELLA_LOG_NAME", PACKAGE_NAME)
+    return os.path.join(root, "{name}.log".format(name=name))
```

### Comparing `maya_umbrella-0.3.0/maya_umbrella/hooks/delete_turtle.py` & `maya_umbrella-0.4.0/maya_umbrella/hooks/delete_turtle.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 # Import third-party modules
 import maya.cmds as cmds
 import maya.mel as mel
 
 
-def hook(logger):
+def hook(virus_cleaner):
     for plugin in ["Turtle.mll", "mayatomr.mll"]:
         if cmds.pluginInfo(plugin, q=1, loaded=1):
             cmds.unloadPlugin(plugin, f=1)
-    turtle_nodes = ["TurtleRenderOptions", "TurtleUIOptions", "TurtleBakeLayerManager", "TurtleDefaultBakeLayer"]
+    turtle_nodes = [
+        "TurtleRenderOptions",
+        "TurtleUIOptions",
+        "TurtleBakeLayerManager",
+        "TurtleDefaultBakeLayer",
+    ]
     for node in turtle_nodes:
         if cmds.objExists(node):
             cmds.lockNode(node, lock=1)
             cmds.delete(node)
     if not cmds.about(query=1, batch=1):
         shelves = cmds.tabLayout(mel.eval("$tmpVar=$gShelfTopLevel"), q=1, ca=1)
         if "TURTLE" in shelves:
```

### Comparing `maya_umbrella-0.3.0/maya_umbrella/hooks/delete_unknown_plugin_node.py` & `maya_umbrella-0.4.0/maya_umbrella/hooks/delete_unknown_plugin_node.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # Import third-party modules
 import maya.cmds as cmds
 
 
-def hook(logger):
+def hook(virus_cleaner):
     unknown_node = cmds.ls(type="unknown")
     unknown_plugin = cmds.unknownPlugin(query=True, l=True)
     if unknown_node:
         for nodeObj in unknown_node:
             if cmds.objExists(nodeObj):
                 if cmds.referenceQuery(nodeObj, isNodeReferenced=True):
-                    logger.warning("Node from reference, skip.  {}".format(nodeObj))
+                    virus_cleaner.logger.warning("Node from reference, skip. {}".format(nodeObj))
                     continue
                 if cmds.lockNode(nodeObj, query=True)[0]:
                     try:
                         cmds.lockNode(nodeObj, lock=False)
-                    except Exception as e:
-                        logger.warning("The node is locked and cannot be unlocked. skip  {}".format(nodeObj))
+                    except Exception:
+                        virus_cleaner.logger.warning(
+                            "The node is locked and cannot be unlocked. skip {}".format(nodeObj))
                         continue
                 try:
                     cmds.delete(nodeObj)
-                    logger.warning("Delete node :  {}".format(nodeObj))
-                except Exception as e:
+                    virus_cleaner.logger.warning("Delete node: {}".format(nodeObj))
+                except Exception:
                     pass
 
     if unknown_plugin:
         for plugObj in unknown_plugin:
             cmds.unknownPlugin(plugObj, remove=True)
-            logger.warning("Delete plug-in :  {}".format(plugObj))
+            virus_cleaner.logger.warning("Delete plug-in: {}".format(plugObj))
```

### Comparing `maya_umbrella-0.3.0/maya_umbrella/vaccines/vaccine2.py` & `maya_umbrella-0.4.0/maya_umbrella/vaccines/vaccine2.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,63 +3,58 @@
 
 # Import third-party modules
 import maya.cmds as cmds
 
 # Import local modules
 from maya_umbrella.filesystem import read_file
 from maya_umbrella.filesystem import rename
-from maya_umbrella.vaccine import BaseVaccine
+from maya_umbrella.vaccine import AbstractVaccine
 
 
-class Vaccine(BaseVaccine):
+class Vaccine(AbstractVaccine):
     virus_name = "zei jian kang"
-    _bad_files = []
 
-    def __init__(self, logger=None):
-        super(Vaccine, self).__init__(logger)
-
-    @property
-    def bad_files(self):
-        return [os.path.join(self.local_script_path, "vaccine.py"), os.path.join(self.local_script_path, "vaccine.pyc")]
-
-    def _get_nodes(self):
-        bad_script_nodes = []
+    def collect_bad_nodes(self):
+        """Collect all bad nodes related to the virus."""
         for script_node in cmds.ls(type="script"):
             if cmds.referenceQuery(script_node, isNodeReferenced=True):
                 continue
             script_before_string = cmds.getAttr("{}.before".format(script_node))
             script_after_string = cmds.getAttr("{}.after".format(script_node))
             for script_string in [script_before_string, script_after_string]:
                 if not script_string:
                     continue
                 if "internalVar" in script_string or "userSetup" in script_string or "fuckVirus" in script_string:
-                    self._logger.warning("script node {} has internalVar or userSetup or fuckVirus".format(script_node))
-                    bad_script_nodes.append(script_node)
-        return bad_script_nodes
-
-    @property
-    def bad_nodes(self):
-        return self._get_nodes()
+                    self.report_issue(script_node)
+                    self.api.add_bad_node(script_node)
 
-    def check_usersetup_py(self):
+    def collect_issues(self):
+        """Collect all issues related to the virus."""
+        self.api.add_bad_files(
+            [
+                os.path.join(self.api.local_script_path, "vaccine.py"),
+                os.path.join(self.api.local_script_path, "vaccine.pyc"),
+            ],
+        )
+        self.collect_bad_usersetup_py()
+        self.collect_bad_nodes()
+
+    def collect_bad_usersetup_py(self):
+        """Collect all bad userSetup.py files related to the virus."""
         for usersetup_py in [
-            os.path.join(self.local_script_path, "vaccine.py"),
-            os.path.join(self.user_script_path, "vaccine.py"),
-            os.path.join(self.local_script_path, "userSetup.py"),
-            os.path.join(self.user_script_path, "userSetup.py"),
+            os.path.join(self.api.local_script_path, "vaccine.py"),
+            os.path.join(self.api.user_script_path, "vaccine.py"),
+            os.path.join(self.api.local_script_path, "userSetup.py"),
+            os.path.join(self.api.user_script_path, "userSetup.py"),
         ]:
             if os.path.exists(usersetup_py):
                 data = read_file(usersetup_py)
                 if "petri_dish_path = cmds.internalVar(userAppDir=True) + 'scripts/userSetup.py" in data:
-                    self._logger.warning("vaccine.py found : Infected by Malware!")
-                    self._bad_files.append(rename(usersetup_py))
+                    self.report_issue("vaccine.py")
+                    self.api.add_bad_file(rename(usersetup_py))
 
                 if (
                     "cmds.evalDeferred('leukocyte = vaccine.phage()')" in data
                     and "cmds.evalDeferred('leukocyte.occupation()')" in data
                 ):
-                    self._logger.warning("userSetup.py : Infected by Malware!")
-                    self._bad_files.append(rename(usersetup_py))
-
-    def before_callback(self, *args, **kwargs):
-        self.check_usersetup_py()
-        super(Vaccine, self).before_callback(args, kwargs)
+                    self.report_issue("userSetup.py")
+                    self.api.add_bad_file(rename(usersetup_py))
```

### Comparing `maya_umbrella-0.3.0/maya_umbrella/vaccines/vaccine3.py` & `maya_umbrella-0.4.0/maya_umbrella/vaccines/vaccine3.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,106 +5,74 @@
 
 # Import third-party modules
 import maya.cmds as cmds
 
 # Import local modules
 from maya_umbrella.filesystem import read_file
 from maya_umbrella.filesystem import rename
-from maya_umbrella.vaccine import BaseVaccine
+from maya_umbrella.vaccine import AbstractVaccine
 
 
-class Vaccine(BaseVaccine):
+class Vaccine(AbstractVaccine):
     virus_name = "virus2024429"
     hik_regex = r"python\(\"import base64;\s*pyCode\s*=\s*base64\.urlsafe_b64decode\([\'\"].*?[\"\']\);\s*exec\s*\(\s*pyCode\s*\)\"\)\s*;"
-    _bad_files = []
 
-    def __init__(self, logger=None):
-        super(Vaccine, self).__init__(logger)
-
-    @property
-    def bad_files(self):
-        return self._bad_files
-
-    @property
-    def get_syssst_dir(self):
-        return os.path.join(os.getenv("APPDATA"), "syssst")
-
-    def _get_nodes(self):
-        bad_expression = []
+    def collect_bad_nodes(self):
+        """Collect all bad nodes related to the virus."""
         for script_node in cmds.ls(type="script"):
             if cmds.referenceQuery(script_node, isNodeReferenced=True):
                 continue
             # check uifiguration
             if cmds.objExists("{}.KGMScriptProtector".format(script_node)):
-                bad_expression.append(script_node)
+                self.api.add_bad_node(script_node)
             # check vaccine
             if "_gene" in script_node:
-                bad_expression.append(script_node)
-
-        return bad_expression
+                self.api.add_bad_node(script_node)
 
-    def check_usersetup_mel(self):
+    def collect_bad_mel_files(self):
+        """Collect all bad MEL files related to the virus."""
         # check usersetup.mel
         # C:/Users/hallong/Documents/maya/scripts/usersetup.mel
         # C:/Users/hallong/Documents/maya/xxxx/scripts/usersetup.mel
         for usersetup_mel in [
-            os.path.join(self.local_script_path, "usersetup.mel"),
-            os.path.join(self.user_script_path, "usersetup.mel"),
+            os.path.join(self.api.local_script_path, "usersetup.mel"),
+            os.path.join(self.api.user_script_path, "usersetup.mel"),
         ]:
             if os.path.exists(usersetup_mel):
                 data = read_file(usersetup_mel)
                 if "import base64; pyCode = base64.urlsafe_b64decode" in data:
-                    self._bad_files.append(rename(usersetup_mel))
+                    self.api.add_bad_file(rename(usersetup_mel))
 
-    @property
-    def bad_nodes(self):
-        return self._get_nodes()
-
-    def before_callback(self, *args, **kwargs):
-        self._bad_files.extend([self.get_syssst_dir])
-        self.check_usersetup_mel()
-        self.fix_hik_files()
-        self.fix_script_job()
-        super(Vaccine, self).before_callback(args, kwargs)
+    def collect_script_jobs(self):
+        """Collect all script jobs related to the virus."""
+        virus_gene = [
+            "leukocyte",
+            "execute",
+        ]
 
-    def fix_hik_files(self):
-        pattern = os.path.join(self.maya_install_root, "resources/l10n/*/plug-ins/mayaHIK.pres.mel")
+        for script_job in cmds.scriptJob(listJobs=True):
+            for virus in virus_gene:
+                if virus in script_job:
+                    self.api.add_bad_script_jobs(script_job)
+
+    def fix_bad_hik_files(self):
+        """Fix all bad HIK files related to the virus."""
+        pattern = os.path.join(self.api.maya_install_root, "resources/l10n/*/plug-ins/mayaHIK.pres.mel")
         for hik_mel in glob.glob(pattern):
             with open(hik_mel, "rb") as f:
                 data = f.read()
             try:
                 check = re.findall(self.hik_regex, data)
             except TypeError:
                 check = []
             if len(check) > 0:
+                self.report_issue(hik_mel)
                 with open(hik_mel, "wb") as f:
                     f.write(re.sub(self.hik_regex, "", data))
-                self._logger.warning("Remove virus code from {}".format(hik_mel))
-
-    def fix_script_job(self):
-        virus_gene = [
-            "leukocyte",
-            "execute",
-        ]
+                self.logger.debug("Remove virus code from {}".format(hik_mel))
 
-        def get_virus_script_jobs():
-            """Traverse the list of virus script job name.
-            Returns:
-                list: Malicious virus script job name.
-            """
-            return [
-                scriptjob
-                for scriptjob in cmds.scriptJob(listJobs=True)
-                for virus in virus_gene
-                if virus in scriptjob
-            ]
-
-        for script_job in get_virus_script_jobs():
-            script_num = int(script_job.split(":", 1)[0])
-            self._logger.info("Kill script job {}".format(script_job))
-            cmds.scriptJob(kill=script_num, force=True)
-
-    def after_callback(self, *args, **kwargs):
-        """After callback."""
-        self.check_usersetup_mel()
-        self.fix_hik_files()
-        super(Vaccine, self).after_callback(args, kwargs)
+    def collect_issues(self):
+        """Collect all issues related to the virus."""
+        self.api.add_bad_file(os.path.join(os.getenv("APPDATA"), "syssst"))
+        self.collect_bad_mel_files()
+        self.collect_bad_nodes()
+        self.api.add_fix_function(self.fix_bad_hik_files)
```

### Comparing `maya_umbrella-0.3.0/pyproject.toml` & `maya_umbrella-0.4.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "maya_umbrella"
-version = "0.3.0"
+version = "0.4.0"
 description = "Check and fix maya virus."
 homepage = "https://github.com/loonghao/maya_umbrella"
 repository = "https://github.com/loonghao/maya_umbrella"
 documentation = "https://github.com/loonghao/maya_umbrella"
 keywords = ["notifiers", "python", "Maya", "dcc"]
 authors = ["longhao <hal.long@outlook.com>"]
 license = "MIT"
@@ -30,28 +30,28 @@
 python = ">=2.7,<2.8 || >=3.6.0"
 
 [tool.poetry.dev-dependencies]
 nox = {version = "^2024.3.2", python = ">=3.8.1,<3.11"}
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.3.0"
+version = "0.4.0"
 tag_format = "v$version"
 version_files = [
     "pyproject.toml:version",
     "maya_umbrella/__version__.py"
 ]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
-target_version = ['py36']
+target-version = ['py36', 'py37', 'py38', 'py39']
 include = '\.pyi?$'
 exclude = '''
 
 (
   /(
       \.eggs         # exclude a few common directories in the
     | \.git          # root of the project
@@ -73,15 +73,15 @@
 [tool.isort]
 profile = "black"
 atomic = true
 include_trailing_comma = true
 lines_after_imports = 2
 lines_between_types = 1
 use_parentheses = true
-src_paths = ["maya_umbrella", "test"]
+src_paths = ["maya_umbrella", "tests"]
 filter_files = true
 known_first_party = "maya_umbrella"
 
 # Enforce import section headers.
 import_heading_future = "Import future modules"
 import_heading_stdlib = "Import built-in modules"
 import_heading_thirdparty = "Import third-party modules"
@@ -89,7 +89,76 @@
 
 force_sort_within_sections = true
 force_single_line = true
 
 # All project unrelated unknown imports belong to third-party.
 default_section = "THIRDPARTY"
 skip_glob = "*/docs/conf.py"
+
+
+# https://beta.ruff.rs/docs/configuration/
+[tool.ruff]
+exclude = [
+    ".bzr",
+    ".direnv",
+    ".eggs",
+    ".git",
+    ".git-rewrite",
+    ".hg",
+    ".ipynb_checkpoints",
+    ".mypy_cache",
+    ".nox",
+    ".pants.d",
+    ".pyenv",
+    ".pytest_cache",
+    ".pytype",
+    ".ruff_cache",
+    ".svn",
+    ".tox",
+    ".venv",
+    ".vscode",
+    "__pypackages__",
+    "_build",
+    "buck-out",
+    "build",
+    "dist",
+    "node_modules",
+    "site-packages",
+    "venv",
+    "dev",
+    "noxfile.py"
+]
+line-length = 120
+
+[tool.ruff.lint]
+extend-select = [
+    "Q",
+    "RUF100",
+    "C90",
+    "UP",
+    "I",
+    "D",
+    "DTZ005", # https://docs.astral.sh/ruff/rules/call-datetime-now-without-tzinfo/
+] # add "T" to disallow prints
+flake8-quotes = { inline-quotes = "double", multiline-quotes = "double" }
+mccabe = { max-complexity = 14 }
+ignore = [
+    "D107", # ignore missing docstring in __init__ methods
+    "D100", # ignore missing docstring in module
+    "D104", # ignore missing docstring in public package
+    "D105", # ignore missing docstring in magic methods
+    "C901", # ignore too complex functions, doesn't seem to be worth it
+    "UP032",
+    "UP004",
+]
+
+[tool.ruff.lint.pydocstyle]
+convention = "google"
+
+[tool.ruff.lint.per-file-ignores]
+"tests/**/*.py" = ["D"]
+"docs/*.py" = ["D"]
+"dev/*.py" = ["D"]
+
+[tool.ruff.format]
+docstring-code-format = true
+quote-style = "double"
```

