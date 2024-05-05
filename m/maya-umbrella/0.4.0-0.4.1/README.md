# Comparing `tmp/maya_umbrella-0.4.0.tar.gz` & `tmp/maya_umbrella-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maya_umbrella-0.4.0.tar", max compression
+gzip compressed data, was "maya_umbrella-0.4.1.tar", max compression
```

## Comparing `maya_umbrella-0.4.0.tar` & `maya_umbrella-0.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1060 2024-05-05 17:10:04.248802 maya_umbrella-0.4.0/LICENSE
--rw-r--r--   0        0        0     5624 2024-05-05 17:10:04.248802 maya_umbrella-0.4.0/README.md
--rw-r--r--   0        0        0      106 2024-05-05 17:10:04.272802 maya_umbrella-0.4.0/maya_umbrella/__init__.py
--rw-r--r--   0        0        0       22 2024-05-05 17:10:04.272802 maya_umbrella-0.4.0/maya_umbrella/__version__.py
--rw-r--r--   0        0        0      130 2024-05-05 17:10:04.272802 maya_umbrella-0.4.0/maya_umbrella/constants.py
--rw-r--r--   0        0        0     4098 2024-05-05 17:10:04.272802 maya_umbrella-0.4.0/maya_umbrella/core.py
--rw-r--r--   0        0        0     4140 2024-05-05 17:10:04.272802 maya_umbrella-0.4.0/maya_umbrella/filesystem.py
--rw-r--r--   0        0        0        0 2024-05-05 17:10:04.272802 maya_umbrella-0.4.0/maya_umbrella/hooks/__init__.py
--rw-r--r--   0        0        0      734 2024-05-05 17:10:04.272802 maya_umbrella-0.4.0/maya_umbrella/hooks/delete_turtle.py
--rw-r--r--   0        0        0     1246 2024-05-05 17:10:04.272802 maya_umbrella-0.4.0/maya_umbrella/hooks/delete_unknown_plugin_node.py
--rw-r--r--   0        0        0      546 2024-05-05 17:10:04.272802 maya_umbrella-0.4.0/maya_umbrella/hooks/fix_model_panel.py
--rw-r--r--   0        0        0      457 2024-05-05 17:10:04.272802 maya_umbrella-0.4.0/maya_umbrella/hooks/fix_on_model_change_3dc.py
--rw-r--r--   0        0        0     1338 2024-05-05 17:10:04.272802 maya_umbrella-0.4.0/maya_umbrella/log.py
--rw-r--r--   0        0        0     7075 2024-05-05 17:10:04.272802 maya_umbrella-0.4.0/maya_umbrella/vaccine.py
--rw-r--r--   0        0        0        0 2024-05-05 17:10:04.272802 maya_umbrella-0.4.0/maya_umbrella/vaccines/__init__.py
--rw-r--r--   0        0        0      430 2024-05-05 17:10:04.272802 maya_umbrella-0.4.0/maya_umbrella/vaccines/vaccine1.py
--rw-r--r--   0        0        0     2526 2024-05-05 17:10:04.272802 maya_umbrella-0.4.0/maya_umbrella/vaccines/vaccine2.py
--rw-r--r--   0        0        0     3061 2024-05-05 17:10:04.272802 maya_umbrella-0.4.0/maya_umbrella/vaccines/vaccine3.py
--rw-r--r--   0        0        0     3837 2024-05-05 17:10:04.272802 maya_umbrella-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     6675 1970-01-01 00:00:00.000000 maya_umbrella-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-05-05 17:37:22.477592 maya_umbrella-0.4.1/LICENSE
+-rw-r--r--   0        0        0     5659 2024-05-05 17:37:22.477592 maya_umbrella-0.4.1/README.md
+-rw-r--r--   0        0        0      106 2024-05-05 17:37:22.501592 maya_umbrella-0.4.1/maya_umbrella/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-05 17:37:22.501592 maya_umbrella-0.4.1/maya_umbrella/__version__.py
+-rw-r--r--   0        0        0      130 2024-05-05 17:37:22.501592 maya_umbrella-0.4.1/maya_umbrella/constants.py
+-rw-r--r--   0        0        0     4112 2024-05-05 17:37:22.501592 maya_umbrella-0.4.1/maya_umbrella/core.py
+-rw-r--r--   0        0        0     4125 2024-05-05 17:37:22.501592 maya_umbrella-0.4.1/maya_umbrella/filesystem.py
+-rw-r--r--   0        0        0        0 2024-05-05 17:37:22.501592 maya_umbrella-0.4.1/maya_umbrella/hooks/__init__.py
+-rw-r--r--   0        0        0      734 2024-05-05 17:37:22.501592 maya_umbrella-0.4.1/maya_umbrella/hooks/delete_turtle.py
+-rw-r--r--   0        0        0     1246 2024-05-05 17:37:22.501592 maya_umbrella-0.4.1/maya_umbrella/hooks/delete_unknown_plugin_node.py
+-rw-r--r--   0        0        0      546 2024-05-05 17:37:22.501592 maya_umbrella-0.4.1/maya_umbrella/hooks/fix_model_panel.py
+-rw-r--r--   0        0        0      457 2024-05-05 17:37:22.505591 maya_umbrella-0.4.1/maya_umbrella/hooks/fix_on_model_change_3dc.py
+-rw-r--r--   0        0        0     1338 2024-05-05 17:37:22.505591 maya_umbrella-0.4.1/maya_umbrella/log.py
+-rw-r--r--   0        0        0     7033 2024-05-05 17:37:22.505591 maya_umbrella-0.4.1/maya_umbrella/vaccine.py
+-rw-r--r--   0        0        0        0 2024-05-05 17:37:22.505591 maya_umbrella-0.4.1/maya_umbrella/vaccines/__init__.py
+-rw-r--r--   0        0        0      430 2024-05-05 17:37:22.505591 maya_umbrella-0.4.1/maya_umbrella/vaccines/vaccine1.py
+-rw-r--r--   0        0        0     2526 2024-05-05 17:37:22.505591 maya_umbrella-0.4.1/maya_umbrella/vaccines/vaccine2.py
+-rw-r--r--   0        0        0     3053 2024-05-05 17:37:22.505591 maya_umbrella-0.4.1/maya_umbrella/vaccines/vaccine3.py
+-rw-r--r--   0        0        0     3849 2024-05-05 17:37:22.505591 maya_umbrella-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     6710 1970-01-01 00:00:00.000000 maya_umbrella-0.4.1/PKG-INFO
```

### Comparing `maya_umbrella-0.4.0/LICENSE` & `maya_umbrella-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.4.0/README.md` & `maya_umbrella-0.4.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 Check and fix maya virus.
 
 
 # 发开环境设置
 
-python 版本 3.9
+通过虚拟环境去设置开发环境, 推荐python-3.8以上的版本
 
 ```shell
 pip install nox poetry
 ```
 
 # 开发调试
 
@@ -56,17 +56,15 @@
 继承`from maya_umbrella.vaccine import AbstractVaccine`并且class名字叫`Vaccine`即可, 然后去写具体的收集病毒逻辑
 
 ## 代码检查
 
 我们可以利用封装好的`nox`命令去执行进行代码检查
 
 ```shell
-nox -s lint
-nox -s black
-nox -s isort
+nox -s ruff_check
 ```
 
 # 环境变量
 
 我们可以通过下列环境变量去修改maya_umbrella的一些设置，方便有pipeline的公司可以更好的集成
 
 修改maya umbrella的日志保存目录，默认是windows temp目录
```

#### html2text {}

```diff
@@ -18,28 +18,29 @@
 green)](https://img.shields.io/badge/maya-2021-green) [![maya-2020](https://
 img.shields.io/badge/maya-2020-green)](https://img.shields.io/badge/maya-2020-
 green) [![maya-2019](https://img.shields.io/badge/maya-2019-green)](https://
 img.shields.io/badge/maya-2019-green) [![maya-2018](https://img.shields.io/
 badge/maya-2018-green)](https://img.shields.io/badge/maya-2018-green) [![All
 Contributors](https://img.shields.io/badge/all_contributors-4-
 orange.svg?style=flat-square)](#contributors-) Check and fix maya virus. #
-åå¼ç¯å¢è®¾ç½® python çæ¬ 3.9 ```shell pip install nox poetry ``` #
-å¼åè°è¯ ```shell nox -s maya-2020 ``` ## å¨mayaä¸­æµè¯ éè¿`nox -
-s maya-xxx`, å¯å¨maya. noxä¼å¨ææ ¹æ®ä½ æ¬å°å®è£å¾mayaå»æ³¨ånox
-session, æ¯å¦ä½ æ¬å°å®è£äº`maya-2020`ï¼é£ä¹éè¿`nox -s maya-2018`
+åå¼ç¯å¢è®¾ç½® éè¿èæç¯å¢å»è®¾ç½®å¼åç¯å¢, æ¨èpython-
+3.8ä»¥ä¸ççæ¬ ```shell pip install nox poetry ``` # å¼åè°è¯ ```shell
+nox -s maya-2020 ``` ## å¨mayaä¸­æµè¯ éè¿`nox -s maya-xxx`, å¯å¨maya.
+noxä¼å¨ææ ¹æ®ä½ æ¬å°å®è£å¾mayaå»æ³¨ånox session,
+æ¯å¦ä½ æ¬å°å®è£äº`maya-2020`ï¼é£ä¹éè¿`nox -s maya-2018`
 å¯å¨mayaåå¨èæ¬ç¼è¾å¨ä¸­æ§è¡ä¸é¢å¾ä»£ç ï¼å°±ä¼å¨æçä»`/
 tests/virus/`éé¢å»open maæä»¶å»è¿è¡æµè¯. ```python import
 manual_test_in_maya manual_test_in_maya.start() ``` ## å¢å æ°çç«è å¨`/
 maya_umbrella/vaccines/` æ°å»ºä¸ä¸ªpy,
 å ä¸ºæå¾å¤çæ¯æ²¡æå·ä½çåå­ä»£å·ï¼æä»¬ç»ä¸ä»¥`vaccine.py`
 ç»§æ¿`from maya_umbrella.vaccine import
 AbstractVaccine`å¹¶ä¸classåå­å«`Vaccine`å³å¯,
 ç¶åå»åå·ä½çæ¶éçæ¯é»è¾ ## ä»£ç æ£æ¥
 æä»¬å¯ä»¥å©ç¨å°è£å¥½ç`nox`å½ä»¤å»æ§è¡è¿è¡ä»£ç æ£æ¥ ```shell
-nox -s lint nox -s black nox -s isort ``` # ç¯å¢åé
+nox -s ruff_check ``` # ç¯å¢åé
 æä»¬å¯ä»¥éè¿ä¸åç¯å¢åéå»ä¿®æ¹maya_umbrellaçä¸äºè®¾ç½®ï¼æ¹ä¾¿æpipelineçå¬å¸å¯ä»¥æ´å¥½çéæ
 ä¿®æ¹maya umbrellaçæ¥å¿ä¿å­ç®å½ï¼é»è®¤æ¯windows tempç®å½ ```shell
 MAYA_UMBRELLA_LOG_ROOT ``` ä¿®æ¹maya umbrellaçæ¥å¿æä»¶åç§°,
 é»è®¤æ¯`maya_umbrella` ```shell MAYA_UMBRELLA_LOG_NAME ```
 è®¾ç½®æ¥å¿çº§å«ï¼é»è®¤æ¯info,
 å¯ä»¥æ¯debugå¯ä»¥çå°æ´å¤çæ¥å¿ä¿¡æ¯ ```shell
 MAYA_UMBRELLA_LOG_LEVEL ``` ## Contributors â¨ Thanks goes to these wonderful
```

### Comparing `maya_umbrella-0.4.0/maya_umbrella/core.py` & `maya_umbrella-0.4.1/maya_umbrella/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
     def run_hooks(self):
         """Run all hooks, only works in non-batch mode."""
         if not cmds.about(batch=True):
             for hook_file in get_hooks():
                 self.logger.debug("run_hook: %s", hook_file)
                 try:
-                    load_hook(hook_file).hook(self.virus_cleaner)
+                    load_hook(hook_file).hook(virus_cleaner=self.virus_cleaner)
                 except Exception as e:
                     self.logger.error("Error running hook: %s", e)
 
     def collect(self):
         """Collect all issues related to the Maya virus."""
         for vaccine in self.vaccines:
             vaccine.collect_issues()
```

### Comparing `maya_umbrella-0.4.0/maya_umbrella/filesystem.py` & `maya_umbrella-0.4.1/maya_umbrella/filesystem.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,37 +106,34 @@
 def get_hooks():
     """Return a list of paths to all hook files in the 'hooks' directory."""
     pattern = os.path.join(this_root(), "hooks", "*.py")
     return [hook for hook in glob.glob(pattern) if "__init__" not in hook]
 
 
 def get_vaccines():
-    """
-    Get a list of all vaccine files.
+    """Get a list of all vaccine files.
 
     Returns:
         list: A list of vaccine files.
     """
     pattern = os.path.join(this_root(), "vaccines", "*.py")
     return [vaccine for vaccine in glob.glob(pattern) if "__init__" not in vaccine]
 
 
 def get_log_root():
-    """
-    Get the log root directory.
+    """Get the log root directory.
 
     Returns:
         str: The log root directory.
     """
     return os.getenv("MAYA_UMBRELLA_LOG_ROOT", tempfile.gettempdir())
 
 
 def get_log_file():
-    """
-    Get the path of the log file.
+    """Get the path of the log file.
 
     Returns:
         str: The path of the log file.
     """
     root = get_log_root()
     try:
         os.makedirs(root)
```

### Comparing `maya_umbrella-0.4.0/maya_umbrella/hooks/delete_turtle.py` & `maya_umbrella-0.4.1/maya_umbrella/hooks/delete_turtle.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.4.0/maya_umbrella/hooks/delete_unknown_plugin_node.py` & `maya_umbrella-0.4.1/maya_umbrella/hooks/delete_unknown_plugin_node.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.4.0/maya_umbrella/hooks/fix_model_panel.py` & `maya_umbrella-0.4.1/maya_umbrella/hooks/fix_model_panel.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.4.0/maya_umbrella/log.py` & `maya_umbrella-0.4.1/maya_umbrella/log.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.4.0/maya_umbrella/vaccine.py` & `maya_umbrella-0.4.1/maya_umbrella/vaccine.py`

 * *Files 11% similar despite different names*

```diff
@@ -146,27 +146,27 @@
         self._fix_funcs.append(func)
 
     # fix
 
     def fix_script_jobs(self):
         for script_job in self.bad_script_jobs:
             script_num = int(script_job.split(":", 1)[0])
-            self.logger.info("Kill script job {}".format(script_job))
+            self.logger.info("Kill script job %s", script_job)
             cmds.scriptJob(kill=script_num, force=True)
             self._bad_script_jobs.remove(script_job)
 
     def fix_bad_files(self):
         for file_ in self.bad_files:
             if os.path.exists(file_):
                 if os.path.isfile(file_):
-                    self.logger.info("Removing {}".format(file_))
+                    self.logger.info("Removing %s", file_)
                     safe_remove_file(file_)
                     self._bad_files.remove(file_)
                 else:
-                    self.logger.info("Removing folder {}".format(file_))
+                    self.logger.info("Removing folder %s", file_)
                     safe_rmtree(file_)
                     self._bad_files.remove(file_)
 
     def fix_bad_nodes(self):
         for node in self.bad_nodes:
             self.logger.info("Deleting %s", node)
             try:
@@ -185,17 +185,17 @@
         self.fix_bad_nodes()
         self.fix_script_jobs()
         for func in self._fix_funcs:
             func()
 
     def report_all_issues(self):
         """Report all issues related to the Maya virus."""
-        self.logger.info("Bad files: {}".format(self.bad_files))
-        self.logger.info("Bad nodes: {}".format(self.bad_nodes))
-        self.logger.info("Bad script jobs: {}".format(self.bad_script_jobs))
+        self.logger.info("Bad files: %s", self.bad_files)
+        self.logger.info("Bad nodes: %s", self.bad_nodes)
+        self.logger.info("Bad script jobs: %s", self.bad_script_jobs)
 
     def reset_all_issues(self):
         """Reset all issues related to the Maya virus."""
         self._bad_files = []
         self._bad_nodes = []
         self._bad_script_nodes = []
         self._bad_script_jobs = []
```

### Comparing `maya_umbrella-0.4.0/maya_umbrella/vaccines/vaccine2.py` & `maya_umbrella-0.4.1/maya_umbrella/vaccines/vaccine2.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.4.0/maya_umbrella/vaccines/vaccine3.py` & `maya_umbrella-0.4.1/maya_umbrella/vaccines/vaccine3.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
                 check = re.findall(self.hik_regex, data)
             except TypeError:
                 check = []
             if len(check) > 0:
                 self.report_issue(hik_mel)
                 with open(hik_mel, "wb") as f:
                     f.write(re.sub(self.hik_regex, "", data))
-                self.logger.debug("Remove virus code from {}".format(hik_mel))
+                self.logger.info("Remove virus code from %s", hik_mel)
 
     def collect_issues(self):
         """Collect all issues related to the virus."""
         self.api.add_bad_file(os.path.join(os.getenv("APPDATA"), "syssst"))
         self.collect_bad_mel_files()
         self.collect_bad_nodes()
         self.api.add_fix_function(self.fix_bad_hik_files)
```

### Comparing `maya_umbrella-0.4.0/pyproject.toml` & `maya_umbrella-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "maya_umbrella"
-version = "0.4.0"
+version = "0.4.1"
 description = "Check and fix maya virus."
 homepage = "https://github.com/loonghao/maya_umbrella"
 repository = "https://github.com/loonghao/maya_umbrella"
 documentation = "https://github.com/loonghao/maya_umbrella"
 keywords = ["notifiers", "python", "Maya", "dcc"]
 authors = ["longhao <hal.long@outlook.com>"]
 license = "MIT"
@@ -30,15 +30,15 @@
 python = ">=2.7,<2.8 || >=3.6.0"
 
 [tool.poetry.dev-dependencies]
 nox = {version = "^2024.3.2", python = ">=3.8.1,<3.11"}
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.4.0"
+version = "0.4.1"
 tag_format = "v$version"
 version_files = [
     "pyproject.toml:version",
     "maya_umbrella/__version__.py"
 ]
 
 [build-system]
@@ -138,14 +138,15 @@
     "I",
     "D",
     "DTZ005", # https://docs.astral.sh/ruff/rules/call-datetime-now-without-tzinfo/
 ] # add "T" to disallow prints
 flake8-quotes = { inline-quotes = "double", multiline-quotes = "double" }
 mccabe = { max-complexity = 14 }
 ignore = [
+    "I001",
     "D107", # ignore missing docstring in __init__ methods
     "D100", # ignore missing docstring in module
     "D104", # ignore missing docstring in public package
     "D105", # ignore missing docstring in magic methods
     "C901", # ignore too complex functions, doesn't seem to be worth it
     "UP032",
     "UP004",
```

### Comparing `maya_umbrella-0.4.0/PKG-INFO` & `maya_umbrella-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maya_umbrella
-Version: 0.4.0
+Version: 0.4.1
 Summary: Check and fix maya virus.
 Home-page: https://github.com/loonghao/maya_umbrella
 License: MIT
 Keywords: notifiers,python,Maya,dcc
 Author: longhao
 Author-email: hal.long@outlook.com
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
@@ -46,15 +46,15 @@
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 Check and fix maya virus.
 
 
 # 发开环境设置
 
-python 版本 3.9
+通过虚拟环境去设置开发环境, 推荐python-3.8以上的版本
 
 ```shell
 pip install nox poetry
 ```
 
 # 开发调试
 
@@ -81,17 +81,15 @@
 继承`from maya_umbrella.vaccine import AbstractVaccine`并且class名字叫`Vaccine`即可, 然后去写具体的收集病毒逻辑
 
 ## 代码检查
 
 我们可以利用封装好的`nox`命令去执行进行代码检查
 
 ```shell
-nox -s lint
-nox -s black
-nox -s isort
+nox -s ruff_check
 ```
 
 # 环境变量
 
 我们可以通过下列环境变量去修改maya_umbrella的一些设置，方便有pipeline的公司可以更好的集成
 
 修改maya umbrella的日志保存目录，默认是windows temp目录
```

