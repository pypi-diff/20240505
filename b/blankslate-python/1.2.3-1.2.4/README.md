# Comparing `tmp/blankslate_python-1.2.3.tar.gz` & `tmp/blankslate_python-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blankslate_python-1.2.3.tar", max compression
+gzip compressed data, was "blankslate_python-1.2.4.tar", max compression
```

## Comparing `blankslate_python-1.2.3.tar` & `blankslate_python-1.2.4.tar`

### file list

```diff
@@ -1,46 +1,45 @@
--rw-r--r--   0        0        0     1092 2024-05-02 10:19:51.904181 blankslate_python-1.2.3/LICENSE
--rw-r--r--   0        0        0     2866 2024-05-05 13:53:12.838114 blankslate_python-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     2292 2024-05-05 13:26:10.987045 blankslate_python-1.2.3/README.md
--rw-r--r--   0        0        0        0 2024-05-02 10:44:42.812685 blankslate_python-1.2.3/source/blankslate/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.2.3/source/blankslate/config/__init__.py
--rw-r--r--   0        0        0      603 2024-05-02 11:13:24.933968 blankslate_python-1.2.3/source/blankslate/config/constants.py
--rw-r--r--   0        0        0     1370 2024-05-04 22:07:28.201885 blankslate_python-1.2.3/source/blankslate/config/paths.py
--rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.2.3/source/blankslate/generation/__init__.py
--rw-r--r--   0        0        0     2703 2024-05-04 21:50:23.783020 blankslate_python-1.2.3/source/blankslate/generation/folder_generation.py
--rw-r--r--   0        0        0     7394 2024-05-05 13:29:06.558176 blankslate_python-1.2.3/source/blankslate/generation/project_generation.py
--rw-r--r--   0        0        0     1927 2024-05-05 12:20:11.191034 blankslate_python-1.2.3/source/blankslate/generation/template_rendering.py
--rw-r--r--   0        0        0     3237 2024-05-04 16:12:56.451075 blankslate_python-1.2.3/source/blankslate/generation/templates/.gitignore.j2
--rw-r--r--   0        0        0     1063 2024-05-04 16:23:15.585858 blankslate_python-1.2.3/source/blankslate/generation/templates/.pre-commit-config.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-25 00:35:55.069192 blankslate_python-1.2.3/source/blankslate/generation/templates/__init__.py.j2
--rw-r--r--   0        0        0        0 2024-05-04 16:23:28.152760 blankslate_python-1.2.3/source/blankslate/generation/templates/CHANGELOG.md.j2
--rw-r--r--   0        0        0      317 2024-05-04 16:12:34.560332 blankslate_python-1.2.3/source/blankslate/generation/templates/command_line.py.j2
--rw-r--r--   0        0        0      264 2024-05-04 16:24:45.758933 blankslate_python-1.2.3/source/blankslate/generation/templates/conf.py.j2
--rw-r--r--   0        0        0      603 2024-05-04 16:17:49.390745 blankslate_python-1.2.3/source/blankslate/generation/templates/constants.py.j2
--rw-r--r--   0        0        0     3393 2024-05-05 13:27:07.390679 blankslate_python-1.2.3/source/blankslate/generation/templates/continuous_integration.yml.j2
--rw-r--r--   0        0        0     3292 2024-05-04 17:06:59.156818 blankslate_python-1.2.3/source/blankslate/generation/templates/CONTRIBUTING.md.j2
--rw-r--r--   0        0        0       84 2024-05-04 16:21:59.690182 blankslate_python-1.2.3/source/blankslate/generation/templates/extensions.json.j2
--rw-r--r--   0        0        0     1702 2024-05-04 17:14:07.452271 blankslate_python-1.2.3/source/blankslate/generation/templates/index.rst.j2
--rw-r--r--   0        0        0     1112 2024-04-24 16:37:27.384880 blankslate_python-1.2.3/source/blankslate/generation/templates/LICENSE.j2
--rw-r--r--   0        0        0      538 2024-05-04 22:16:16.909317 blankslate_python-1.2.3/source/blankslate/generation/templates/main.py.j2
--rw-r--r--   0        0        0      804 2024-05-05 13:29:20.897846 blankslate_python-1.2.3/source/blankslate/generation/templates/make.bat.j2
--rw-r--r--   0        0        0      658 2024-05-05 13:29:36.112070 blankslate_python-1.2.3/source/blankslate/generation/templates/Makefile.j2
--rw-r--r--   0        0        0     1450 2024-05-04 22:08:31.773848 blankslate_python-1.2.3/source/blankslate/generation/templates/paths.py.j2
--rw-r--r--   0        0        0        0 2024-05-04 16:22:44.594900 blankslate_python-1.2.3/source/blankslate/generation/templates/py.typed.j2
--rw-r--r--   0        0        0     2854 2024-05-04 16:15:25.176062 blankslate_python-1.2.3/source/blankslate/generation/templates/pyproject.toml.j2
--rw-r--r--   0        0        0     1134 2024-05-04 17:05:19.122602 blankslate_python-1.2.3/source/blankslate/generation/templates/README.md.j2
--rw-r--r--   0        0        0     1330 2024-05-04 16:22:21.707040 blankslate_python-1.2.3/source/blankslate/generation/templates/release.sh.j2
--rw-r--r--   0        0        0      297 2024-05-04 16:25:54.086216 blankslate_python-1.2.3/source/blankslate/generation/templates/requirements-dev.txt.j2
--rw-r--r--   0        0        0       28 2024-05-04 16:16:50.883961 blankslate_python-1.2.3/source/blankslate/generation/templates/requirements.txt.j2
--rw-r--r--   0        0        0      297 2024-05-04 16:16:41.782308 blankslate_python-1.2.3/source/blankslate/generation/templates/requirements_dev.txt.j2
--rw-r--r--   0        0        0     1879 2024-05-04 16:17:23.522577 blankslate_python-1.2.3/source/blankslate/generation/templates/setup_logging.py.j2
--rw-r--r--   0        0        0      261 2024-05-04 16:21:46.396690 blankslate_python-1.2.3/source/blankslate/generation/templates/todo_to_issue.yml.j2
--rw-r--r--   0        0        0     2810 2024-05-05 13:26:45.432480 blankslate_python-1.2.3/source/blankslate/generation/templates/tox.ini.j2
--rw-r--r--   0        0        0        5 2024-05-02 09:28:19.986550 blankslate_python-1.2.3/source/blankslate/generation/templates/VERSION.j2
--rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.2.3/source/blankslate/interface/__init__.py
--rw-r--r--   0        0        0     3690 2024-05-04 21:03:09.221224 blankslate_python-1.2.3/source/blankslate/interface/command_line.py
--rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.2.3/source/blankslate/logs/__init__.py
--rw-r--r--   0        0        0     1879 2024-05-04 14:22:34.495627 blankslate_python-1.2.3/source/blankslate/logs/setup_logging.py
--rw-r--r--   0        0        0      752 2024-05-04 19:52:11.294674 blankslate_python-1.2.3/source/blankslate/main.py
--rw-r--r--   0        0        0        0 2024-05-02 11:03:08.486123 blankslate_python-1.2.3/source/blankslate/py.typed
--rw-r--r--   0        0        0        6 2024-05-05 13:53:15.439890 blankslate_python-1.2.3/source/blankslate/VERSION
--rw-r--r--   0        0        0     3190 1970-01-01 00:00:00.000000 blankslate_python-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-05-02 10:19:51.904181 blankslate_python-1.2.4/LICENSE
+-rw-r--r--   0        0        0     2866 2024-05-05 14:39:28.598641 blankslate_python-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2292 2024-05-05 13:26:10.987045 blankslate_python-1.2.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-02 10:44:42.812685 blankslate_python-1.2.4/source/blankslate/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.2.4/source/blankslate/config/__init__.py
+-rw-r--r--   0        0        0      603 2024-05-02 11:13:24.933968 blankslate_python-1.2.4/source/blankslate/config/constants.py
+-rw-r--r--   0        0        0     1370 2024-05-04 22:07:28.201885 blankslate_python-1.2.4/source/blankslate/config/paths.py
+-rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.2.4/source/blankslate/generation/__init__.py
+-rw-r--r--   0        0        0     2703 2024-05-04 21:50:23.783020 blankslate_python-1.2.4/source/blankslate/generation/folder_generation.py
+-rw-r--r--   0        0        0     7394 2024-05-05 13:29:06.558176 blankslate_python-1.2.4/source/blankslate/generation/project_generation.py
+-rw-r--r--   0        0        0     1927 2024-05-05 12:20:11.191034 blankslate_python-1.2.4/source/blankslate/generation/template_rendering.py
+-rw-r--r--   0        0        0     3237 2024-05-04 16:12:56.451075 blankslate_python-1.2.4/source/blankslate/generation/templates/.gitignore.j2
+-rw-r--r--   0        0        0     1063 2024-05-04 16:23:15.585858 blankslate_python-1.2.4/source/blankslate/generation/templates/.pre-commit-config.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-25 00:35:55.069192 blankslate_python-1.2.4/source/blankslate/generation/templates/__init__.py.j2
+-rw-r--r--   0        0        0        0 2024-05-04 16:23:28.152760 blankslate_python-1.2.4/source/blankslate/generation/templates/CHANGELOG.md.j2
+-rw-r--r--   0        0        0      317 2024-05-04 16:12:34.560332 blankslate_python-1.2.4/source/blankslate/generation/templates/command_line.py.j2
+-rw-r--r--   0        0        0      264 2024-05-04 16:24:45.758933 blankslate_python-1.2.4/source/blankslate/generation/templates/conf.py.j2
+-rw-r--r--   0        0        0      603 2024-05-04 16:17:49.390745 blankslate_python-1.2.4/source/blankslate/generation/templates/constants.py.j2
+-rw-r--r--   0        0        0     3393 2024-05-05 13:27:07.390679 blankslate_python-1.2.4/source/blankslate/generation/templates/continuous_integration.yml.j2
+-rw-r--r--   0        0        0     3292 2024-05-04 17:06:59.156818 blankslate_python-1.2.4/source/blankslate/generation/templates/CONTRIBUTING.md.j2
+-rw-r--r--   0        0        0       84 2024-05-04 16:21:59.690182 blankslate_python-1.2.4/source/blankslate/generation/templates/extensions.json.j2
+-rw-r--r--   0        0        0     1702 2024-05-04 17:14:07.452271 blankslate_python-1.2.4/source/blankslate/generation/templates/index.rst.j2
+-rw-r--r--   0        0        0     1112 2024-04-24 16:37:27.384880 blankslate_python-1.2.4/source/blankslate/generation/templates/LICENSE.j2
+-rw-r--r--   0        0        0      538 2024-05-04 22:16:16.909317 blankslate_python-1.2.4/source/blankslate/generation/templates/main.py.j2
+-rw-r--r--   0        0        0      804 2024-05-05 13:29:20.897846 blankslate_python-1.2.4/source/blankslate/generation/templates/make.bat.j2
+-rw-r--r--   0        0        0      658 2024-05-05 13:29:36.112070 blankslate_python-1.2.4/source/blankslate/generation/templates/Makefile.j2
+-rw-r--r--   0        0        0     1450 2024-05-04 22:08:31.773848 blankslate_python-1.2.4/source/blankslate/generation/templates/paths.py.j2
+-rw-r--r--   0        0        0        0 2024-05-04 16:22:44.594900 blankslate_python-1.2.4/source/blankslate/generation/templates/py.typed.j2
+-rw-r--r--   0        0        0     2835 2024-05-05 14:38:44.495340 blankslate_python-1.2.4/source/blankslate/generation/templates/pyproject.toml.j2
+-rw-r--r--   0        0        0     1016 2024-05-05 14:35:17.971966 blankslate_python-1.2.4/source/blankslate/generation/templates/README.md.j2
+-rw-r--r--   0        0        0     1330 2024-05-04 16:22:21.707040 blankslate_python-1.2.4/source/blankslate/generation/templates/release.sh.j2
+-rw-r--r--   0        0        0      297 2024-05-04 16:25:54.086216 blankslate_python-1.2.4/source/blankslate/generation/templates/requirements-dev.txt.j2
+-rw-r--r--   0        0        0       13 2024-05-05 14:38:29.079891 blankslate_python-1.2.4/source/blankslate/generation/templates/requirements.txt.j2
+-rw-r--r--   0        0        0     1879 2024-05-04 16:17:23.522577 blankslate_python-1.2.4/source/blankslate/generation/templates/setup_logging.py.j2
+-rw-r--r--   0        0        0      261 2024-05-04 16:21:46.396690 blankslate_python-1.2.4/source/blankslate/generation/templates/todo_to_issue.yml.j2
+-rw-r--r--   0        0        0     2810 2024-05-05 13:26:45.432480 blankslate_python-1.2.4/source/blankslate/generation/templates/tox.ini.j2
+-rw-r--r--   0        0        0        5 2024-05-02 09:28:19.986550 blankslate_python-1.2.4/source/blankslate/generation/templates/VERSION.j2
+-rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.2.4/source/blankslate/interface/__init__.py
+-rw-r--r--   0        0        0     3690 2024-05-04 21:03:09.221224 blankslate_python-1.2.4/source/blankslate/interface/command_line.py
+-rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.2.4/source/blankslate/logs/__init__.py
+-rw-r--r--   0        0        0     1879 2024-05-04 14:22:34.495627 blankslate_python-1.2.4/source/blankslate/logs/setup_logging.py
+-rw-r--r--   0        0        0      752 2024-05-04 19:52:11.294674 blankslate_python-1.2.4/source/blankslate/main.py
+-rw-r--r--   0        0        0        0 2024-05-02 11:03:08.486123 blankslate_python-1.2.4/source/blankslate/py.typed
+-rw-r--r--   0        0        0        6 2024-05-05 14:39:31.205304 blankslate_python-1.2.4/source/blankslate/VERSION
+-rw-r--r--   0        0        0     3190 1970-01-01 00:00:00.000000 blankslate_python-1.2.4/PKG-INFO
```

### Comparing `blankslate_python-1.2.3/LICENSE` & `blankslate_python-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.3/pyproject.toml` & `blankslate_python-1.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "blankslate-python"
-version = "1.2.3"
+version = "1.2.4"
 description = "A blank slate for Python projects"
 authors = ["William Fayers <wills@fayers.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "blankslate", from = "source"}]
 homepage = "https://github.com/unkokaeru/blankslate"
 repository = "https://github.com/unkokaeru/blankslate"
```

### Comparing `blankslate_python-1.2.3/README.md` & `blankslate_python-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.3/source/blankslate/config/constants.py` & `blankslate_python-1.2.4/source/blankslate/config/constants.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.3/source/blankslate/config/paths.py` & `blankslate_python-1.2.4/source/blankslate/config/paths.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.3/source/blankslate/generation/folder_generation.py` & `blankslate_python-1.2.4/source/blankslate/generation/folder_generation.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.3/source/blankslate/generation/project_generation.py` & `blankslate_python-1.2.4/source/blankslate/generation/project_generation.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.3/source/blankslate/generation/template_rendering.py` & `blankslate_python-1.2.4/source/blankslate/generation/template_rendering.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.3/source/blankslate/generation/templates/.gitignore.j2` & `blankslate_python-1.2.4/source/blankslate/generation/templates/.gitignore.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.3/source/blankslate/generation/templates/.pre-commit-config.yaml.j2` & `blankslate_python-1.2.4/source/blankslate/generation/templates/.pre-commit-config.yaml.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.3/source/blankslate/generation/templates/constants.py.j2` & `blankslate_python-1.2.4/source/blankslate/generation/templates/constants.py.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.3/source/blankslate/generation/templates/continuous_integration.yml.j2` & `blankslate_python-1.2.4/source/blankslate/generation/templates/continuous_integration.yml.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.3/source/blankslate/generation/templates/CONTRIBUTING.md.j2` & `blankslate_python-1.2.4/source/blankslate/generation/templates/CONTRIBUTING.md.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.3/source/blankslate/generation/templates/index.rst.j2` & `blankslate_python-1.2.4/source/blankslate/generation/templates/index.rst.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.3/source/blankslate/generation/templates/LICENSE.j2` & `blankslate_python-1.2.4/source/blankslate/generation/templates/LICENSE.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.3/source/blankslate/generation/templates/main.py.j2` & `blankslate_python-1.2.4/source/blankslate/generation/templates/main.py.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.3/source/blankslate/generation/templates/make.bat.j2` & `blankslate_python-1.2.4/source/blankslate/generation/templates/make.bat.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.3/source/blankslate/generation/templates/Makefile.j2` & `blankslate_python-1.2.4/source/blankslate/generation/templates/Makefile.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.3/source/blankslate/generation/templates/paths.py.j2` & `blankslate_python-1.2.4/source/blankslate/generation/templates/paths.py.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.3/source/blankslate/generation/templates/pyproject.toml.j2` & `blankslate_python-1.2.4/source/blankslate/generation/templates/pyproject.toml.j2`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 packages = [{include = "{{ project_name }}", from = "source"}]
 homepage = "https://github.com/{{ project_author_username }}/{{ project_name }}"
 repository = "https://github.com/{{ project_author_username }}/{{ project_name }}"
 include = ["LICENSE", "source/{{ project_name }}/py.typed", "source/{{ project_name }}/VERSION"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
-Jinja2 = "^3.0.0"
 rich = "^12.0.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.0"
 tox = "^3.27.0"
 
 [tool.poetry.group.lint.dependencies]
```

### Comparing `blankslate_python-1.2.3/source/blankslate/generation/templates/README.md.j2` & `blankslate_python-1.2.4/source/blankslate/generation/templates/README.md.j2`

 * *Files 16% similar despite different names*

```diff
@@ -10,24 +10,18 @@
 
 ```bash
 pip install {{ project_name }}
 ```
 
 ## Usage
 
-After installation, you can use the package by importing it in your project:
-
-```python
-import {{ project_name }}
-```
-
-Or, you can run the package as a script:
+After installation, you can use the package by executing:
 
 ```bash
-python -m {{ project_name }}
+{{ project_name }}
 ```
 
 ## Features
 
 - **Feature 1**: Description of feature 1.
 - **Feature 2**: Description of feature 2.
 - etc. - *to be filled in by the project maintainer*.
```

### Comparing `blankslate_python-1.2.3/source/blankslate/generation/templates/release.sh.j2` & `blankslate_python-1.2.4/source/blankslate/generation/templates/release.sh.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.3/source/blankslate/generation/templates/setup_logging.py.j2` & `blankslate_python-1.2.4/source/blankslate/generation/templates/setup_logging.py.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.3/source/blankslate/generation/templates/tox.ini.j2` & `blankslate_python-1.2.4/source/blankslate/generation/templates/tox.ini.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.3/source/blankslate/interface/command_line.py` & `blankslate_python-1.2.4/source/blankslate/interface/command_line.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.3/source/blankslate/logs/setup_logging.py` & `blankslate_python-1.2.4/source/blankslate/logs/setup_logging.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.3/source/blankslate/main.py` & `blankslate_python-1.2.4/source/blankslate/main.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.3/PKG-INFO` & `blankslate_python-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blankslate-python
-Version: 1.2.3
+Version: 1.2.4
 Summary: A blank slate for Python projects
 Home-page: https://github.com/unkokaeru/blankslate
 License: MIT
 Author: William Fayers
 Author-email: wills@fayers.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

