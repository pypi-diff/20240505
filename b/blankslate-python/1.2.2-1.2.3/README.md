# Comparing `tmp/blankslate_python-1.2.2.tar.gz` & `tmp/blankslate_python-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blankslate_python-1.2.2.tar", max compression
+gzip compressed data, was "blankslate_python-1.2.3.tar", max compression
```

## Comparing `blankslate_python-1.2.2.tar` & `blankslate_python-1.2.3.tar`

### file list

```diff
@@ -1,44 +1,46 @@
--rw-r--r--   0        0        0     1092 2024-05-02 10:19:51.904181 blankslate_python-1.2.2/LICENSE
--rw-r--r--   0        0        0     2866 2024-05-05 12:47:21.875813 blankslate_python-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     2245 2024-05-04 17:20:48.274142 blankslate_python-1.2.2/README.md
--rw-r--r--   0        0        0        0 2024-05-02 10:44:42.812685 blankslate_python-1.2.2/source/blankslate/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.2.2/source/blankslate/config/__init__.py
--rw-r--r--   0        0        0      603 2024-05-02 11:13:24.933968 blankslate_python-1.2.2/source/blankslate/config/constants.py
--rw-r--r--   0        0        0     1370 2024-05-04 22:07:28.201885 blankslate_python-1.2.2/source/blankslate/config/paths.py
--rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.2.2/source/blankslate/generation/__init__.py
--rw-r--r--   0        0        0     2703 2024-05-04 21:50:23.783020 blankslate_python-1.2.2/source/blankslate/generation/folder_generation.py
--rw-r--r--   0        0        0     7172 2024-05-04 21:45:47.045260 blankslate_python-1.2.2/source/blankslate/generation/project_generation.py
--rw-r--r--   0        0        0     1927 2024-05-05 12:20:11.191034 blankslate_python-1.2.2/source/blankslate/generation/template_rendering.py
--rw-r--r--   0        0        0     3237 2024-05-04 16:12:56.451075 blankslate_python-1.2.2/source/blankslate/generation/templates/.gitignore.j2
--rw-r--r--   0        0        0     1063 2024-05-04 16:23:15.585858 blankslate_python-1.2.2/source/blankslate/generation/templates/.pre-commit-config.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-25 00:35:55.069192 blankslate_python-1.2.2/source/blankslate/generation/templates/__init__.py.j2
--rw-r--r--   0        0        0        0 2024-05-04 16:23:28.152760 blankslate_python-1.2.2/source/blankslate/generation/templates/CHANGELOG.md.j2
--rw-r--r--   0        0        0      317 2024-05-04 16:12:34.560332 blankslate_python-1.2.2/source/blankslate/generation/templates/command_line.py.j2
--rw-r--r--   0        0        0      264 2024-05-04 16:24:45.758933 blankslate_python-1.2.2/source/blankslate/generation/templates/conf.py.j2
--rw-r--r--   0        0        0      603 2024-05-04 16:17:49.390745 blankslate_python-1.2.2/source/blankslate/generation/templates/constants.py.j2
--rw-r--r--   0        0        0     3382 2024-05-04 20:50:51.262514 blankslate_python-1.2.2/source/blankslate/generation/templates/continuous_integration.yml.j2
--rw-r--r--   0        0        0     3292 2024-05-04 17:06:59.156818 blankslate_python-1.2.2/source/blankslate/generation/templates/CONTRIBUTING.md.j2
--rw-r--r--   0        0        0       84 2024-05-04 16:21:59.690182 blankslate_python-1.2.2/source/blankslate/generation/templates/extensions.json.j2
--rw-r--r--   0        0        0     1702 2024-05-04 17:14:07.452271 blankslate_python-1.2.2/source/blankslate/generation/templates/index.rst.j2
--rw-r--r--   0        0        0     1112 2024-04-24 16:37:27.384880 blankslate_python-1.2.2/source/blankslate/generation/templates/LICENSE.j2
--rw-r--r--   0        0        0      538 2024-05-04 22:16:16.909317 blankslate_python-1.2.2/source/blankslate/generation/templates/main.py.j2
--rw-r--r--   0        0        0     1450 2024-05-04 22:08:31.773848 blankslate_python-1.2.2/source/blankslate/generation/templates/paths.py.j2
--rw-r--r--   0        0        0        0 2024-05-04 16:22:44.594900 blankslate_python-1.2.2/source/blankslate/generation/templates/py.typed.j2
--rw-r--r--   0        0        0     2854 2024-05-04 16:15:25.176062 blankslate_python-1.2.2/source/blankslate/generation/templates/pyproject.toml.j2
--rw-r--r--   0        0        0     1134 2024-05-04 17:05:19.122602 blankslate_python-1.2.2/source/blankslate/generation/templates/README.md.j2
--rw-r--r--   0        0        0     1330 2024-05-04 16:22:21.707040 blankslate_python-1.2.2/source/blankslate/generation/templates/release.sh.j2
--rw-r--r--   0        0        0      297 2024-05-04 16:25:54.086216 blankslate_python-1.2.2/source/blankslate/generation/templates/requirements-dev.txt.j2
--rw-r--r--   0        0        0       28 2024-05-04 16:16:50.883961 blankslate_python-1.2.2/source/blankslate/generation/templates/requirements.txt.j2
--rw-r--r--   0        0        0      297 2024-05-04 16:16:41.782308 blankslate_python-1.2.2/source/blankslate/generation/templates/requirements_dev.txt.j2
--rw-r--r--   0        0        0     1879 2024-05-04 16:17:23.522577 blankslate_python-1.2.2/source/blankslate/generation/templates/setup_logging.py.j2
--rw-r--r--   0        0        0      261 2024-05-04 16:21:46.396690 blankslate_python-1.2.2/source/blankslate/generation/templates/todo_to_issue.yml.j2
--rw-r--r--   0        0        0     2791 2024-05-04 16:26:45.870722 blankslate_python-1.2.2/source/blankslate/generation/templates/tox.ini.j2
--rw-r--r--   0        0        0        5 2024-05-02 09:28:19.986550 blankslate_python-1.2.2/source/blankslate/generation/templates/VERSION.j2
--rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.2.2/source/blankslate/interface/__init__.py
--rw-r--r--   0        0        0     3690 2024-05-04 21:03:09.221224 blankslate_python-1.2.2/source/blankslate/interface/command_line.py
--rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.2.2/source/blankslate/logs/__init__.py
--rw-r--r--   0        0        0     1879 2024-05-04 14:22:34.495627 blankslate_python-1.2.2/source/blankslate/logs/setup_logging.py
--rw-r--r--   0        0        0      752 2024-05-04 19:52:11.294674 blankslate_python-1.2.2/source/blankslate/main.py
--rw-r--r--   0        0        0        0 2024-05-02 11:03:08.486123 blankslate_python-1.2.2/source/blankslate/py.typed
--rw-r--r--   0        0        0        6 2024-05-05 12:47:23.763417 blankslate_python-1.2.2/source/blankslate/VERSION
--rw-r--r--   0        0        0     3143 1970-01-01 00:00:00.000000 blankslate_python-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-05-02 10:19:51.904181 blankslate_python-1.2.3/LICENSE
+-rw-r--r--   0        0        0     2866 2024-05-05 13:53:12.838114 blankslate_python-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2292 2024-05-05 13:26:10.987045 blankslate_python-1.2.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-02 10:44:42.812685 blankslate_python-1.2.3/source/blankslate/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.2.3/source/blankslate/config/__init__.py
+-rw-r--r--   0        0        0      603 2024-05-02 11:13:24.933968 blankslate_python-1.2.3/source/blankslate/config/constants.py
+-rw-r--r--   0        0        0     1370 2024-05-04 22:07:28.201885 blankslate_python-1.2.3/source/blankslate/config/paths.py
+-rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.2.3/source/blankslate/generation/__init__.py
+-rw-r--r--   0        0        0     2703 2024-05-04 21:50:23.783020 blankslate_python-1.2.3/source/blankslate/generation/folder_generation.py
+-rw-r--r--   0        0        0     7394 2024-05-05 13:29:06.558176 blankslate_python-1.2.3/source/blankslate/generation/project_generation.py
+-rw-r--r--   0        0        0     1927 2024-05-05 12:20:11.191034 blankslate_python-1.2.3/source/blankslate/generation/template_rendering.py
+-rw-r--r--   0        0        0     3237 2024-05-04 16:12:56.451075 blankslate_python-1.2.3/source/blankslate/generation/templates/.gitignore.j2
+-rw-r--r--   0        0        0     1063 2024-05-04 16:23:15.585858 blankslate_python-1.2.3/source/blankslate/generation/templates/.pre-commit-config.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-25 00:35:55.069192 blankslate_python-1.2.3/source/blankslate/generation/templates/__init__.py.j2
+-rw-r--r--   0        0        0        0 2024-05-04 16:23:28.152760 blankslate_python-1.2.3/source/blankslate/generation/templates/CHANGELOG.md.j2
+-rw-r--r--   0        0        0      317 2024-05-04 16:12:34.560332 blankslate_python-1.2.3/source/blankslate/generation/templates/command_line.py.j2
+-rw-r--r--   0        0        0      264 2024-05-04 16:24:45.758933 blankslate_python-1.2.3/source/blankslate/generation/templates/conf.py.j2
+-rw-r--r--   0        0        0      603 2024-05-04 16:17:49.390745 blankslate_python-1.2.3/source/blankslate/generation/templates/constants.py.j2
+-rw-r--r--   0        0        0     3393 2024-05-05 13:27:07.390679 blankslate_python-1.2.3/source/blankslate/generation/templates/continuous_integration.yml.j2
+-rw-r--r--   0        0        0     3292 2024-05-04 17:06:59.156818 blankslate_python-1.2.3/source/blankslate/generation/templates/CONTRIBUTING.md.j2
+-rw-r--r--   0        0        0       84 2024-05-04 16:21:59.690182 blankslate_python-1.2.3/source/blankslate/generation/templates/extensions.json.j2
+-rw-r--r--   0        0        0     1702 2024-05-04 17:14:07.452271 blankslate_python-1.2.3/source/blankslate/generation/templates/index.rst.j2
+-rw-r--r--   0        0        0     1112 2024-04-24 16:37:27.384880 blankslate_python-1.2.3/source/blankslate/generation/templates/LICENSE.j2
+-rw-r--r--   0        0        0      538 2024-05-04 22:16:16.909317 blankslate_python-1.2.3/source/blankslate/generation/templates/main.py.j2
+-rw-r--r--   0        0        0      804 2024-05-05 13:29:20.897846 blankslate_python-1.2.3/source/blankslate/generation/templates/make.bat.j2
+-rw-r--r--   0        0        0      658 2024-05-05 13:29:36.112070 blankslate_python-1.2.3/source/blankslate/generation/templates/Makefile.j2
+-rw-r--r--   0        0        0     1450 2024-05-04 22:08:31.773848 blankslate_python-1.2.3/source/blankslate/generation/templates/paths.py.j2
+-rw-r--r--   0        0        0        0 2024-05-04 16:22:44.594900 blankslate_python-1.2.3/source/blankslate/generation/templates/py.typed.j2
+-rw-r--r--   0        0        0     2854 2024-05-04 16:15:25.176062 blankslate_python-1.2.3/source/blankslate/generation/templates/pyproject.toml.j2
+-rw-r--r--   0        0        0     1134 2024-05-04 17:05:19.122602 blankslate_python-1.2.3/source/blankslate/generation/templates/README.md.j2
+-rw-r--r--   0        0        0     1330 2024-05-04 16:22:21.707040 blankslate_python-1.2.3/source/blankslate/generation/templates/release.sh.j2
+-rw-r--r--   0        0        0      297 2024-05-04 16:25:54.086216 blankslate_python-1.2.3/source/blankslate/generation/templates/requirements-dev.txt.j2
+-rw-r--r--   0        0        0       28 2024-05-04 16:16:50.883961 blankslate_python-1.2.3/source/blankslate/generation/templates/requirements.txt.j2
+-rw-r--r--   0        0        0      297 2024-05-04 16:16:41.782308 blankslate_python-1.2.3/source/blankslate/generation/templates/requirements_dev.txt.j2
+-rw-r--r--   0        0        0     1879 2024-05-04 16:17:23.522577 blankslate_python-1.2.3/source/blankslate/generation/templates/setup_logging.py.j2
+-rw-r--r--   0        0        0      261 2024-05-04 16:21:46.396690 blankslate_python-1.2.3/source/blankslate/generation/templates/todo_to_issue.yml.j2
+-rw-r--r--   0        0        0     2810 2024-05-05 13:26:45.432480 blankslate_python-1.2.3/source/blankslate/generation/templates/tox.ini.j2
+-rw-r--r--   0        0        0        5 2024-05-02 09:28:19.986550 blankslate_python-1.2.3/source/blankslate/generation/templates/VERSION.j2
+-rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.2.3/source/blankslate/interface/__init__.py
+-rw-r--r--   0        0        0     3690 2024-05-04 21:03:09.221224 blankslate_python-1.2.3/source/blankslate/interface/command_line.py
+-rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.2.3/source/blankslate/logs/__init__.py
+-rw-r--r--   0        0        0     1879 2024-05-04 14:22:34.495627 blankslate_python-1.2.3/source/blankslate/logs/setup_logging.py
+-rw-r--r--   0        0        0      752 2024-05-04 19:52:11.294674 blankslate_python-1.2.3/source/blankslate/main.py
+-rw-r--r--   0        0        0        0 2024-05-02 11:03:08.486123 blankslate_python-1.2.3/source/blankslate/py.typed
+-rw-r--r--   0        0        0        6 2024-05-05 13:53:15.439890 blankslate_python-1.2.3/source/blankslate/VERSION
+-rw-r--r--   0        0        0     3190 1970-01-01 00:00:00.000000 blankslate_python-1.2.3/PKG-INFO
```

### Comparing `blankslate_python-1.2.2/LICENSE` & `blankslate_python-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.2/pyproject.toml` & `blankslate_python-1.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "blankslate-python"
-version = "1.2.2"
+version = "1.2.3"
 description = "A blank slate for Python projects"
 authors = ["William Fayers <wills@fayers.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "blankslate", from = "source"}]
 homepage = "https://github.com/unkokaeru/blankslate"
 repository = "https://github.com/unkokaeru/blankslate"
```

### Comparing `blankslate_python-1.2.2/README.md` & `blankslate_python-1.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 Follow the prompts to specify your project details. Blankslate will create the project in your designated directory. You can then push this project to GitHub and start programming in the `source/PROJECT_NAME/` directory.
 
 ## Features
 
 - **Automatic Project Structure Creation**: Sets up a GitHub-ready Python project with best practices.
 - **Semantic Versioning**: Use the script `./scripts/release.sh VERSION_NUMBER` to auto-version and generate a changelog. Ensure `VERSION_NUMBER` follows [semantic versioning](https://semver.org). Note that this will automatically build and publish the project to PyPi, too.
 - **Commit Style**: Commits should follow the [Angular commit style](https://gist.github.com/brianclements/841ea7bffdb01346392c#commit-message-header).
-- **Documentation**: Automatically generates and pushes documentation to GitHub pages. Make sure your GitHub repository is configured under `Settings -> Pages`.
+- **Documentation**: Automatically generates and pushes documentation to GitHub pages. Make sure your GitHub repository is configured under `Settings -> Pages` and set the deployment branch to `docs/(root)`.
 - **TODO to GitHub Issues**: Converts `# TODO` comments in your Python code into GitHub issues. Configure this in `Settings -> Actions (General) -> Workflow permissions` and enable "Read and write permissions".
 
 ## Extensions
 
 Enhance your Blankslate experience with the [Blankslate Extension Pack](https://marketplace.visualstudio.com/items?itemName=unkokaeru.blankslate-extension-pack) for [VS Code](https://code.visualstudio.com/download).
 
 ## Contributing
```

### Comparing `blankslate_python-1.2.2/source/blankslate/config/constants.py` & `blankslate_python-1.2.3/source/blankslate/config/constants.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.2/source/blankslate/config/paths.py` & `blankslate_python-1.2.3/source/blankslate/config/paths.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.2/source/blankslate/generation/folder_generation.py` & `blankslate_python-1.2.3/source/blankslate/generation/folder_generation.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.2/source/blankslate/generation/project_generation.py` & `blankslate_python-1.2.3/source/blankslate/generation/project_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,15 +192,25 @@
                 "continuous_integration.yml": None,
                 "todo_to_issue.yml": None,
             },
         },
         ".vscode": {
             "extensions.json": None,
         },
-        "docs": {},
+        "docs": {
+            "build": {},
+            "source": {
+                "_static": {},
+                "_templates": {},
+                "conf.py": None,
+                "index.rst": None,
+            },
+            "make.bat": None,
+            "Makefile": None,
+        },
         "scripts": {"release.sh"},
         "source": {
             project_name: {
                 "config": {
                     "__init__.py": None,
                     "constants.py": None,
                     "paths.py": None,
@@ -218,17 +228,15 @@
                 "VERSION": None,
             },
         },
         "tests": {},
         ".gitignore": None,
         ".pre-commit-config.yaml": None,
         "CHANGELOG.md": None,
-        "conf.py": None,
         "CONTRIBUTING.md": None,
-        "index.rst": None,
         "LICENSE": None,
         "pyproject.toml": None,
         "README.md": None,
         "requirements-dev.txt": None,
         "requirements.txt": None,
         "tox.ini": None,
     }
```

### Comparing `blankslate_python-1.2.2/source/blankslate/generation/template_rendering.py` & `blankslate_python-1.2.3/source/blankslate/generation/template_rendering.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.2/source/blankslate/generation/templates/.gitignore.j2` & `blankslate_python-1.2.3/source/blankslate/generation/templates/.gitignore.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.2/source/blankslate/generation/templates/.pre-commit-config.yaml.j2` & `blankslate_python-1.2.3/source/blankslate/generation/templates/.pre-commit-config.yaml.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.2/source/blankslate/generation/templates/constants.py.j2` & `blankslate_python-1.2.3/source/blankslate/generation/templates/constants.py.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.2/source/blankslate/generation/templates/continuous_integration.yml.j2` & `blankslate_python-1.2.3/source/blankslate/generation/templates/continuous_integration.yml.j2`

 * *Files 1% similar despite different names*

```diff
@@ -115,8 +115,8 @@
           pull: '--rebase --autostash'
           message: "@auto Update docs"
 
       - name: Deploy new docs if they've been updated
         uses: JamesIves/github-pages-deploy-action@v4.3.3
         with:
           branch: docs
-          folder: docs
+          folder: docs/build/html
```

### Comparing `blankslate_python-1.2.2/source/blankslate/generation/templates/CONTRIBUTING.md.j2` & `blankslate_python-1.2.3/source/blankslate/generation/templates/CONTRIBUTING.md.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.2/source/blankslate/generation/templates/index.rst.j2` & `blankslate_python-1.2.3/source/blankslate/generation/templates/index.rst.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.2/source/blankslate/generation/templates/LICENSE.j2` & `blankslate_python-1.2.3/source/blankslate/generation/templates/LICENSE.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.2/source/blankslate/generation/templates/main.py.j2` & `blankslate_python-1.2.3/source/blankslate/generation/templates/main.py.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.2/source/blankslate/generation/templates/paths.py.j2` & `blankslate_python-1.2.3/source/blankslate/generation/templates/paths.py.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.2/source/blankslate/generation/templates/pyproject.toml.j2` & `blankslate_python-1.2.3/source/blankslate/generation/templates/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.2/source/blankslate/generation/templates/README.md.j2` & `blankslate_python-1.2.3/source/blankslate/generation/templates/README.md.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.2/source/blankslate/generation/templates/release.sh.j2` & `blankslate_python-1.2.3/source/blankslate/generation/templates/release.sh.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.2/source/blankslate/generation/templates/setup_logging.py.j2` & `blankslate_python-1.2.3/source/blankslate/generation/templates/setup_logging.py.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.2/source/blankslate/generation/templates/tox.ini.j2` & `blankslate_python-1.2.3/source/blankslate/generation/templates/tox.ini.j2`

 * *Files 3% similar despite different names*

```diff
@@ -66,16 +66,16 @@
 description = docs: Use Sphinx to generate documentation
 setenv =
     {[testenv]setenv}
     DOCSDIR = {toxinidir}/docs
 deps =
     sphinx
 commands =
-    sphinx-apidoc -f -o "{env:DOCSDIR}/source" "{env:SOURCEDIR}"
-    sphinx-build -b html "{toxinidir}" "{env:DOCSDIR}"
+    sphinx-apidoc -f -o "{env:DOCSDIR}/source/" "{env:SOURCEDIR}/"
+    sphinx-build -M html "{env:DOCSDIR}/source/" "{env:DOCSDIR}/build/"
 
 
 [testenv:release]
 description = Build a new tag and push it to the remote repository
 skip_install = True
 deps =
 	gitchangelog
```

### Comparing `blankslate_python-1.2.2/source/blankslate/interface/command_line.py` & `blankslate_python-1.2.3/source/blankslate/interface/command_line.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.2/source/blankslate/logs/setup_logging.py` & `blankslate_python-1.2.3/source/blankslate/logs/setup_logging.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.2/source/blankslate/main.py` & `blankslate_python-1.2.3/source/blankslate/main.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.2.2/PKG-INFO` & `blankslate_python-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blankslate-python
-Version: 1.2.2
+Version: 1.2.3
 Summary: A blank slate for Python projects
 Home-page: https://github.com/unkokaeru/blankslate
 License: MIT
 Author: William Fayers
 Author-email: wills@fayers.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -51,15 +51,15 @@
 Follow the prompts to specify your project details. Blankslate will create the project in your designated directory. You can then push this project to GitHub and start programming in the `source/PROJECT_NAME/` directory.
 
 ## Features
 
 - **Automatic Project Structure Creation**: Sets up a GitHub-ready Python project with best practices.
 - **Semantic Versioning**: Use the script `./scripts/release.sh VERSION_NUMBER` to auto-version and generate a changelog. Ensure `VERSION_NUMBER` follows [semantic versioning](https://semver.org). Note that this will automatically build and publish the project to PyPi, too.
 - **Commit Style**: Commits should follow the [Angular commit style](https://gist.github.com/brianclements/841ea7bffdb01346392c#commit-message-header).
-- **Documentation**: Automatically generates and pushes documentation to GitHub pages. Make sure your GitHub repository is configured under `Settings -> Pages`.
+- **Documentation**: Automatically generates and pushes documentation to GitHub pages. Make sure your GitHub repository is configured under `Settings -> Pages` and set the deployment branch to `docs/(root)`.
 - **TODO to GitHub Issues**: Converts `# TODO` comments in your Python code into GitHub issues. Configure this in `Settings -> Actions (General) -> Workflow permissions` and enable "Read and write permissions".
 
 ## Extensions
 
 Enhance your Blankslate experience with the [Blankslate Extension Pack](https://marketplace.visualstudio.com/items?itemName=unkokaeru.blankslate-extension-pack) for [VS Code](https://code.visualstudio.com/download).
 
 ## Contributing
```

