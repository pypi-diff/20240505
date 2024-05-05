# Comparing `tmp/blankslate_python-1.3.0.tar.gz` & `tmp/blankslate_python-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blankslate_python-1.3.0.tar", max compression
+gzip compressed data, was "blankslate_python-1.3.1.tar", max compression
```

## Comparing `blankslate_python-1.3.0.tar` & `blankslate_python-1.3.1.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0     1092 2024-05-02 10:19:51.904181 blankslate_python-1.3.0/LICENSE
--rw-r--r--   0        0        0     2866 2024-05-05 16:19:32.183090 blankslate_python-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     2292 2024-05-05 13:26:10.987045 blankslate_python-1.3.0/README.md
--rw-r--r--   0        0        0        0 2024-05-02 10:44:42.812685 blankslate_python-1.3.0/source/blankslate/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.3.0/source/blankslate/config/__init__.py
--rw-r--r--   0        0        0      603 2024-05-02 11:13:24.933968 blankslate_python-1.3.0/source/blankslate/config/constants.py
--rw-r--r--   0        0        0     1370 2024-05-04 22:07:28.201885 blankslate_python-1.3.0/source/blankslate/config/paths.py
--rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.3.0/source/blankslate/generation/__init__.py
--rw-r--r--   0        0        0     2703 2024-05-04 21:50:23.783020 blankslate_python-1.3.0/source/blankslate/generation/folder_generation.py
--rw-r--r--   0        0        0     7441 2024-05-05 16:17:22.206799 blankslate_python-1.3.0/source/blankslate/generation/project_generation.py
--rw-r--r--   0        0        0     1927 2024-05-05 12:20:11.191034 blankslate_python-1.3.0/source/blankslate/generation/template_rendering.py
--rw-r--r--   0        0        0     3237 2024-05-04 16:12:56.451075 blankslate_python-1.3.0/source/blankslate/generation/templates/.gitignore.j2
--rw-r--r--   0        0        0     1063 2024-05-04 16:23:15.585858 blankslate_python-1.3.0/source/blankslate/generation/templates/.pre-commit-config.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-25 00:35:55.069192 blankslate_python-1.3.0/source/blankslate/generation/templates/__init__.py.j2
--rw-r--r--   0        0        0        0 2024-05-04 16:23:28.152760 blankslate_python-1.3.0/source/blankslate/generation/templates/CHANGELOG.md.j2
--rw-r--r--   0        0        0      317 2024-05-04 16:12:34.560332 blankslate_python-1.3.0/source/blankslate/generation/templates/command_line.py.j2
--rw-r--r--   0        0        0      264 2024-05-04 16:24:45.758933 blankslate_python-1.3.0/source/blankslate/generation/templates/conf.py.j2
--rw-r--r--   0        0        0      603 2024-05-04 16:17:49.390745 blankslate_python-1.3.0/source/blankslate/generation/templates/constants.py.j2
--rw-r--r--   0        0        0     3393 2024-05-05 13:27:07.390679 blankslate_python-1.3.0/source/blankslate/generation/templates/continuous_integration.yml.j2
--rw-r--r--   0        0        0     3292 2024-05-04 17:06:59.156818 blankslate_python-1.3.0/source/blankslate/generation/templates/CONTRIBUTING.md.j2
--rw-r--r--   0        0        0       84 2024-05-04 16:21:59.690182 blankslate_python-1.3.0/source/blankslate/generation/templates/extensions.json.j2
--rw-r--r--   0        0        0     1702 2024-05-04 17:14:07.452271 blankslate_python-1.3.0/source/blankslate/generation/templates/index.rst.j2
--rw-r--r--   0        0        0     1112 2024-04-24 16:37:27.384880 blankslate_python-1.3.0/source/blankslate/generation/templates/LICENSE.j2
--rw-r--r--   0        0        0      538 2024-05-04 22:16:16.909317 blankslate_python-1.3.0/source/blankslate/generation/templates/main.py.j2
--rw-r--r--   0        0        0      804 2024-05-05 13:29:20.897846 blankslate_python-1.3.0/source/blankslate/generation/templates/make.bat.j2
--rw-r--r--   0        0        0      658 2024-05-05 13:29:36.112070 blankslate_python-1.3.0/source/blankslate/generation/templates/Makefile.j2
--rw-r--r--   0        0        0     1450 2024-05-04 22:08:31.773848 blankslate_python-1.3.0/source/blankslate/generation/templates/paths.py.j2
--rw-r--r--   0        0        0        0 2024-05-04 16:22:44.594900 blankslate_python-1.3.0/source/blankslate/generation/templates/py.typed.j2
--rw-r--r--   0        0        0     2835 2024-05-05 14:38:44.495340 blankslate_python-1.3.0/source/blankslate/generation/templates/pyproject.toml.j2
--rw-r--r--   0        0        0     1016 2024-05-05 14:35:17.971966 blankslate_python-1.3.0/source/blankslate/generation/templates/README.md.j2
--rw-r--r--   0        0        0     1330 2024-05-04 16:22:21.707040 blankslate_python-1.3.0/source/blankslate/generation/templates/release.sh.j2
--rw-r--r--   0        0        0      297 2024-05-04 16:25:54.086216 blankslate_python-1.3.0/source/blankslate/generation/templates/requirements-dev.txt.j2
--rw-r--r--   0        0        0       13 2024-05-05 14:38:29.079891 blankslate_python-1.3.0/source/blankslate/generation/templates/requirements.txt.j2
--rw-r--r--   0        0        0     1879 2024-05-04 16:17:23.522577 blankslate_python-1.3.0/source/blankslate/generation/templates/setup_logging.py.j2
--rw-r--r--   0        0        0      448 2024-05-05 16:17:52.211617 blankslate_python-1.3.0/source/blankslate/generation/templates/test_main.py.j2
--rw-r--r--   0        0        0      261 2024-05-04 16:21:46.396690 blankslate_python-1.3.0/source/blankslate/generation/templates/todo_to_issue.yml.j2
--rw-r--r--   0        0        0     2810 2024-05-05 13:26:45.432480 blankslate_python-1.3.0/source/blankslate/generation/templates/tox.ini.j2
--rw-r--r--   0        0        0        5 2024-05-02 09:28:19.986550 blankslate_python-1.3.0/source/blankslate/generation/templates/VERSION.j2
--rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.3.0/source/blankslate/interface/__init__.py
--rw-r--r--   0        0        0     3690 2024-05-04 21:03:09.221224 blankslate_python-1.3.0/source/blankslate/interface/command_line.py
--rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.3.0/source/blankslate/logs/__init__.py
--rw-r--r--   0        0        0     1879 2024-05-04 14:22:34.495627 blankslate_python-1.3.0/source/blankslate/logs/setup_logging.py
--rw-r--r--   0        0        0      752 2024-05-04 19:52:11.294674 blankslate_python-1.3.0/source/blankslate/main.py
--rw-r--r--   0        0        0        0 2024-05-02 11:03:08.486123 blankslate_python-1.3.0/source/blankslate/py.typed
--rw-r--r--   0        0        0        6 2024-05-05 16:19:39.125564 blankslate_python-1.3.0/source/blankslate/VERSION
--rw-r--r--   0        0        0     3190 1970-01-01 00:00:00.000000 blankslate_python-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-05-02 10:19:51.904181 blankslate_python-1.3.1/LICENSE
+-rw-r--r--   0        0        0     2866 2024-05-05 16:51:21.025643 blankslate_python-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2292 2024-05-05 16:49:57.766569 blankslate_python-1.3.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-02 10:44:42.812685 blankslate_python-1.3.1/source/blankslate/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.3.1/source/blankslate/config/__init__.py
+-rw-r--r--   0        0        0      603 2024-05-02 11:13:24.933968 blankslate_python-1.3.1/source/blankslate/config/constants.py
+-rw-r--r--   0        0        0     1370 2024-05-04 22:07:28.201885 blankslate_python-1.3.1/source/blankslate/config/paths.py
+-rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.3.1/source/blankslate/generation/__init__.py
+-rw-r--r--   0        0        0     2703 2024-05-04 21:50:23.783020 blankslate_python-1.3.1/source/blankslate/generation/folder_generation.py
+-rw-r--r--   0        0        0     7458 2024-05-05 16:50:23.878225 blankslate_python-1.3.1/source/blankslate/generation/project_generation.py
+-rw-r--r--   0        0        0     1927 2024-05-05 12:20:11.191034 blankslate_python-1.3.1/source/blankslate/generation/template_rendering.py
+-rw-r--r--   0        0        0     3237 2024-05-04 16:12:56.451075 blankslate_python-1.3.1/source/blankslate/generation/templates/.gitignore.j2
+-rw-r--r--   0        0        0        0 2024-05-05 16:50:31.130211 blankslate_python-1.3.1/source/blankslate/generation/templates/.nojekyll.j2
+-rw-r--r--   0        0        0     1063 2024-05-04 16:23:15.585858 blankslate_python-1.3.1/source/blankslate/generation/templates/.pre-commit-config.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-25 00:35:55.069192 blankslate_python-1.3.1/source/blankslate/generation/templates/__init__.py.j2
+-rw-r--r--   0        0        0        0 2024-05-04 16:23:28.152760 blankslate_python-1.3.1/source/blankslate/generation/templates/CHANGELOG.md.j2
+-rw-r--r--   0        0        0      317 2024-05-04 16:12:34.560332 blankslate_python-1.3.1/source/blankslate/generation/templates/command_line.py.j2
+-rw-r--r--   0        0        0      264 2024-05-04 16:24:45.758933 blankslate_python-1.3.1/source/blankslate/generation/templates/conf.py.j2
+-rw-r--r--   0        0        0      603 2024-05-04 16:17:49.390745 blankslate_python-1.3.1/source/blankslate/generation/templates/constants.py.j2
+-rw-r--r--   0        0        0     3393 2024-05-05 13:27:07.390679 blankslate_python-1.3.1/source/blankslate/generation/templates/continuous_integration.yml.j2
+-rw-r--r--   0        0        0     3292 2024-05-04 17:06:59.156818 blankslate_python-1.3.1/source/blankslate/generation/templates/CONTRIBUTING.md.j2
+-rw-r--r--   0        0        0       84 2024-05-04 16:21:59.690182 blankslate_python-1.3.1/source/blankslate/generation/templates/extensions.json.j2
+-rw-r--r--   0        0        0     1702 2024-05-04 17:14:07.452271 blankslate_python-1.3.1/source/blankslate/generation/templates/index.rst.j2
+-rw-r--r--   0        0        0     1112 2024-04-24 16:37:27.384880 blankslate_python-1.3.1/source/blankslate/generation/templates/LICENSE.j2
+-rw-r--r--   0        0        0      538 2024-05-04 22:16:16.909317 blankslate_python-1.3.1/source/blankslate/generation/templates/main.py.j2
+-rw-r--r--   0        0        0      804 2024-05-05 13:29:20.897846 blankslate_python-1.3.1/source/blankslate/generation/templates/make.bat.j2
+-rw-r--r--   0        0        0      658 2024-05-05 13:29:36.112070 blankslate_python-1.3.1/source/blankslate/generation/templates/Makefile.j2
+-rw-r--r--   0        0        0     1450 2024-05-04 22:08:31.773848 blankslate_python-1.3.1/source/blankslate/generation/templates/paths.py.j2
+-rw-r--r--   0        0        0        0 2024-05-04 16:22:44.594900 blankslate_python-1.3.1/source/blankslate/generation/templates/py.typed.j2
+-rw-r--r--   0        0        0     2835 2024-05-05 14:38:44.495340 blankslate_python-1.3.1/source/blankslate/generation/templates/pyproject.toml.j2
+-rw-r--r--   0        0        0     1016 2024-05-05 14:35:17.971966 blankslate_python-1.3.1/source/blankslate/generation/templates/README.md.j2
+-rw-r--r--   0        0        0     1330 2024-05-04 16:22:21.707040 blankslate_python-1.3.1/source/blankslate/generation/templates/release.sh.j2
+-rw-r--r--   0        0        0      297 2024-05-04 16:25:54.086216 blankslate_python-1.3.1/source/blankslate/generation/templates/requirements-dev.txt.j2
+-rw-r--r--   0        0        0       13 2024-05-05 14:38:29.079891 blankslate_python-1.3.1/source/blankslate/generation/templates/requirements.txt.j2
+-rw-r--r--   0        0        0     1879 2024-05-04 16:17:23.522577 blankslate_python-1.3.1/source/blankslate/generation/templates/setup_logging.py.j2
+-rw-r--r--   0        0        0      448 2024-05-05 16:17:52.211617 blankslate_python-1.3.1/source/blankslate/generation/templates/test_main.py.j2
+-rw-r--r--   0        0        0      261 2024-05-04 16:21:46.396690 blankslate_python-1.3.1/source/blankslate/generation/templates/todo_to_issue.yml.j2
+-rw-r--r--   0        0        0     2810 2024-05-05 13:26:45.432480 blankslate_python-1.3.1/source/blankslate/generation/templates/tox.ini.j2
+-rw-r--r--   0        0        0        5 2024-05-02 09:28:19.986550 blankslate_python-1.3.1/source/blankslate/generation/templates/VERSION.j2
+-rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.3.1/source/blankslate/interface/__init__.py
+-rw-r--r--   0        0        0     3690 2024-05-04 21:03:09.221224 blankslate_python-1.3.1/source/blankslate/interface/command_line.py
+-rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.3.1/source/blankslate/logs/__init__.py
+-rw-r--r--   0        0        0     1879 2024-05-04 14:22:34.495627 blankslate_python-1.3.1/source/blankslate/logs/setup_logging.py
+-rw-r--r--   0        0        0      752 2024-05-04 19:52:11.294674 blankslate_python-1.3.1/source/blankslate/main.py
+-rw-r--r--   0        0        0        0 2024-05-02 11:03:08.486123 blankslate_python-1.3.1/source/blankslate/py.typed
+-rw-r--r--   0        0        0        6 2024-05-05 16:51:23.560344 blankslate_python-1.3.1/source/blankslate/VERSION
+-rw-r--r--   0        0        0     3190 1970-01-01 00:00:00.000000 blankslate_python-1.3.1/PKG-INFO
```

### Comparing `blankslate_python-1.3.0/LICENSE` & `blankslate_python-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.0/pyproject.toml` & `blankslate_python-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "blankslate-python"
-version = "1.3.0"
+version = "1.3.1"
 description = "A blank slate for Python projects"
 authors = ["William Fayers <wills@fayers.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "blankslate", from = "source"}]
 homepage = "https://github.com/unkokaeru/blankslate"
 repository = "https://github.com/unkokaeru/blankslate"
```

### Comparing `blankslate_python-1.3.0/README.md` & `blankslate_python-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.0/source/blankslate/config/constants.py` & `blankslate_python-1.3.1/source/blankslate/config/constants.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.0/source/blankslate/config/paths.py` & `blankslate_python-1.3.1/source/blankslate/config/paths.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.0/source/blankslate/generation/folder_generation.py` & `blankslate_python-1.3.1/source/blankslate/generation/folder_generation.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.0/source/blankslate/generation/project_generation.py` & `blankslate_python-1.3.1/source/blankslate/generation/project_generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,15 +193,15 @@
                 "todo_to_issue.yml": None,
             },
         },
         ".vscode": {
             "extensions.json": None,
         },
         "docs": {
-            "build": {},
+            "build": {".nojekyll": None},
             "source": {
                 "_static": {},
                 "_templates": {},
                 "conf.py": None,
                 "index.rst": None,
             },
             "make.bat": None,
```

### Comparing `blankslate_python-1.3.0/source/blankslate/generation/template_rendering.py` & `blankslate_python-1.3.1/source/blankslate/generation/template_rendering.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.0/source/blankslate/generation/templates/.gitignore.j2` & `blankslate_python-1.3.1/source/blankslate/generation/templates/.gitignore.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.0/source/blankslate/generation/templates/.pre-commit-config.yaml.j2` & `blankslate_python-1.3.1/source/blankslate/generation/templates/.pre-commit-config.yaml.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.0/source/blankslate/generation/templates/constants.py.j2` & `blankslate_python-1.3.1/source/blankslate/generation/templates/constants.py.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.0/source/blankslate/generation/templates/continuous_integration.yml.j2` & `blankslate_python-1.3.1/source/blankslate/generation/templates/continuous_integration.yml.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.0/source/blankslate/generation/templates/CONTRIBUTING.md.j2` & `blankslate_python-1.3.1/source/blankslate/generation/templates/CONTRIBUTING.md.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.0/source/blankslate/generation/templates/index.rst.j2` & `blankslate_python-1.3.1/source/blankslate/generation/templates/index.rst.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.0/source/blankslate/generation/templates/LICENSE.j2` & `blankslate_python-1.3.1/source/blankslate/generation/templates/LICENSE.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.0/source/blankslate/generation/templates/main.py.j2` & `blankslate_python-1.3.1/source/blankslate/generation/templates/main.py.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.0/source/blankslate/generation/templates/make.bat.j2` & `blankslate_python-1.3.1/source/blankslate/generation/templates/make.bat.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.0/source/blankslate/generation/templates/Makefile.j2` & `blankslate_python-1.3.1/source/blankslate/generation/templates/Makefile.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.0/source/blankslate/generation/templates/paths.py.j2` & `blankslate_python-1.3.1/source/blankslate/generation/templates/paths.py.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.0/source/blankslate/generation/templates/pyproject.toml.j2` & `blankslate_python-1.3.1/source/blankslate/generation/templates/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.0/source/blankslate/generation/templates/README.md.j2` & `blankslate_python-1.3.1/source/blankslate/generation/templates/README.md.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.0/source/blankslate/generation/templates/release.sh.j2` & `blankslate_python-1.3.1/source/blankslate/generation/templates/release.sh.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.0/source/blankslate/generation/templates/setup_logging.py.j2` & `blankslate_python-1.3.1/source/blankslate/generation/templates/setup_logging.py.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.0/source/blankslate/generation/templates/tox.ini.j2` & `blankslate_python-1.3.1/source/blankslate/generation/templates/tox.ini.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.0/source/blankslate/interface/command_line.py` & `blankslate_python-1.3.1/source/blankslate/interface/command_line.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.0/source/blankslate/logs/setup_logging.py` & `blankslate_python-1.3.1/source/blankslate/logs/setup_logging.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.0/source/blankslate/main.py` & `blankslate_python-1.3.1/source/blankslate/main.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.0/PKG-INFO` & `blankslate_python-1.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blankslate-python
-Version: 1.3.0
+Version: 1.3.1
 Summary: A blank slate for Python projects
 Home-page: https://github.com/unkokaeru/blankslate
 License: MIT
 Author: William Fayers
 Author-email: wills@fayers.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```
