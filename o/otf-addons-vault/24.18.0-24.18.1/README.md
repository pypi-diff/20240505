# Comparing `tmp/otf_addons_vault-24.18.0.tar.gz` & `tmp/otf_addons_vault-24.18.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otf_addons_vault-24.18.0.tar", last modified: Sun May  5 14:13:00 2024, max compression
+gzip compressed data, was "otf_addons_vault-24.18.1.tar", last modified: Sun May  5 14:22:33 2024, max compression
```

## Comparing `otf_addons_vault-24.18.0.tar` & `otf_addons_vault-24.18.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-05 14:13:00.204866 otf_addons_vault-24.18.0/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       72 2024-05-05 14:07:00.000000 otf_addons_vault-24.18.0/AUTHORS
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    35149 2024-05-05 14:07:00.000000 otf_addons_vault-24.18.0/LICENSE
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       44 2024-05-05 14:07:00.000000 otf_addons_vault-24.18.0/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3705 2024-05-05 14:13:00.204866 otf_addons_vault-24.18.0/PKG-INFO
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2107 2024-05-05 14:07:00.000000 otf_addons_vault-24.18.0/README.md
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    14429 2024-05-05 14:07:00.000000 otf_addons_vault-24.18.0/pyproject.toml
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       38 2024-05-05 14:13:00.204866 otf_addons_vault-24.18.0/setup.cfg
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-05 14:13:00.196866 otf_addons_vault-24.18.0/src/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-05 14:13:00.196866 otf_addons_vault-24.18.0/src/opentaskpy/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-05 14:13:00.196866 otf_addons_vault-24.18.0/src/opentaskpy/plugins/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-05 14:13:00.196866 otf_addons_vault-24.18.0/src/opentaskpy/plugins/lookup/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-05 14:13:00.200866 otf_addons_vault-24.18.0/src/opentaskpy/plugins/lookup/hashicorp/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3654 2024-05-05 14:07:00.000000 otf_addons_vault-24.18.0/src/opentaskpy/plugins/lookup/hashicorp/vault.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-05 14:13:00.200866 otf_addons_vault-24.18.0/src/otf_addons_vault.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3705 2024-05-05 14:13:00.000000 otf_addons_vault-24.18.0/src/otf_addons_vault.egg-info/PKG-INFO
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      347 2024-05-05 14:13:00.000000 otf_addons_vault-24.18.0/src/otf_addons_vault.egg-info/SOURCES.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        1 2024-05-05 14:13:00.000000 otf_addons_vault-24.18.0/src/otf_addons_vault.egg-info/dependency_links.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      208 2024-05-05 14:13:00.000000 otf_addons_vault-24.18.0/src/otf_addons_vault.egg-info/requires.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       11 2024-05-05 14:13:00.000000 otf_addons_vault-24.18.0/src/otf_addons_vault.egg-info/top_level.txt
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-05 14:13:00.200866 otf_addons_vault-24.18.0/tests/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3984 2024-05-05 14:07:00.000000 otf_addons_vault-24.18.0/tests/test_plugin_vault.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-05 14:22:33.760862 otf_addons_vault-24.18.1/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       72 2024-05-05 14:07:00.000000 otf_addons_vault-24.18.1/AUTHORS
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    35149 2024-05-05 14:07:00.000000 otf_addons_vault-24.18.1/LICENSE
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       44 2024-05-05 14:07:00.000000 otf_addons_vault-24.18.1/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3705 2024-05-05 14:22:33.756862 otf_addons_vault-24.18.1/PKG-INFO
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2107 2024-05-05 14:07:00.000000 otf_addons_vault-24.18.1/README.md
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    14429 2024-05-05 14:21:41.000000 otf_addons_vault-24.18.1/pyproject.toml
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       38 2024-05-05 14:22:33.760862 otf_addons_vault-24.18.1/setup.cfg
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-05 14:22:33.752863 otf_addons_vault-24.18.1/src/
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-05 14:22:33.752863 otf_addons_vault-24.18.1/src/opentaskpy/
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-05 14:22:33.752863 otf_addons_vault-24.18.1/src/opentaskpy/plugins/
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-05 14:22:33.752863 otf_addons_vault-24.18.1/src/opentaskpy/plugins/lookup/
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-05 14:22:33.752863 otf_addons_vault-24.18.1/src/opentaskpy/plugins/lookup/hashicorp/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3654 2024-05-05 14:07:00.000000 otf_addons_vault-24.18.1/src/opentaskpy/plugins/lookup/hashicorp/vault.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-05 14:22:33.756862 otf_addons_vault-24.18.1/src/otf_addons_vault.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3705 2024-05-05 14:22:33.000000 otf_addons_vault-24.18.1/src/otf_addons_vault.egg-info/PKG-INFO
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      347 2024-05-05 14:22:33.000000 otf_addons_vault-24.18.1/src/otf_addons_vault.egg-info/SOURCES.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        1 2024-05-05 14:22:33.000000 otf_addons_vault-24.18.1/src/otf_addons_vault.egg-info/dependency_links.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      208 2024-05-05 14:22:33.000000 otf_addons_vault-24.18.1/src/otf_addons_vault.egg-info/requires.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       11 2024-05-05 14:22:33.000000 otf_addons_vault-24.18.1/src/otf_addons_vault.egg-info/top_level.txt
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-05 14:22:33.756862 otf_addons_vault-24.18.1/tests/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3984 2024-05-05 14:07:00.000000 otf_addons_vault-24.18.1/tests/test_plugin_vault.py
```

### Comparing `otf_addons_vault-24.18.0/LICENSE` & `otf_addons_vault-24.18.1/LICENSE`

 * *Files identical despite different names*

### Comparing `otf_addons_vault-24.18.0/PKG-INFO` & `otf_addons_vault-24.18.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: otf-addons-vault
-Version: 24.18.0
+Version: 24.18.1
 Summary: Addons for opentaskpy, giving it the ability to read variables from Hashicorp Vault
 Author-email: Adam McDonagh <adam@elitemonkey.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/adammcdonagh/otf-addons-vault
 Project-URL: Bug Tracker, https://github.com/adammcdonagh/otf-addons-vault/issues
 Project-URL: Changelog, https://github.com/adammcdonagh/otf-addons-vault/blob/main/CHANGELOG.md
 Keywords: automation,task,framework,hashicorp,vault,secrets,otf
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: boto3>=1.26
-Requires-Dist: opentaskpy>=v24.13.1
+Requires-Dist: hvac>=2.2.0
+Requires-Dist: opentaskpy>=v24.18.0
 Provides-Extra: dev
 Requires-Dist: pytest-shell; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
 Requires-Dist: types-python-dateutil; extra == "dev"
 Requires-Dist: black>=24.1.1; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
```

### Comparing `otf_addons_vault-24.18.0/README.md` & `otf_addons_vault-24.18.1/README.md`

 * *Files identical despite different names*

### Comparing `otf_addons_vault-24.18.0/pyproject.toml` & `otf_addons_vault-24.18.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "otf-addons-vault"
-version = "v24.18.0"
+version = "v24.18.1"
 authors = [{ name = "Adam McDonagh", email = "adam@elitemonkey.net" }]
 license = { text = "GPLv3" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: POSIX",
 ]
 keywords = ["automation", "task", "framework", "hashicorp", "vault", "secrets", "otf"]
-dependencies = ["boto3 >= 1.26", "opentaskpy >= v24.13.1"]
+dependencies = ["hvac >= 2.2.0", "opentaskpy >= v24.18.0"]
 description = "Addons for opentaskpy, giving it the ability to read variables from Hashicorp Vault"
 readme = "README.md"
 requires-python = ">=3.11"
 
 [project.optional-dependencies]
 dev = [
     "pytest-shell",
@@ -44,15 +44,15 @@
 "Bug Tracker" = "https://github.com/adammcdonagh/otf-addons-vault/issues"
 "Changelog" = "https://github.com/adammcdonagh/otf-addons-vault/blob/main/CHANGELOG.md"
 
 [tool.isort]
 profile = 'black'
 
 [tool.bumpver]
-current_version = "v24.18.0"
+current_version = "v24.18.1"
 version_pattern = "vYY.WW.PATCH[-TAG]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `otf_addons_vault-24.18.0/src/opentaskpy/plugins/lookup/hashicorp/vault.py` & `otf_addons_vault-24.18.1/src/opentaskpy/plugins/lookup/hashicorp/vault.py`

 * *Files identical despite different names*

### Comparing `otf_addons_vault-24.18.0/src/otf_addons_vault.egg-info/PKG-INFO` & `otf_addons_vault-24.18.1/src/otf_addons_vault.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: otf-addons-vault
-Version: 24.18.0
+Version: 24.18.1
 Summary: Addons for opentaskpy, giving it the ability to read variables from Hashicorp Vault
 Author-email: Adam McDonagh <adam@elitemonkey.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/adammcdonagh/otf-addons-vault
 Project-URL: Bug Tracker, https://github.com/adammcdonagh/otf-addons-vault/issues
 Project-URL: Changelog, https://github.com/adammcdonagh/otf-addons-vault/blob/main/CHANGELOG.md
 Keywords: automation,task,framework,hashicorp,vault,secrets,otf
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: boto3>=1.26
-Requires-Dist: opentaskpy>=v24.13.1
+Requires-Dist: hvac>=2.2.0
+Requires-Dist: opentaskpy>=v24.18.0
 Provides-Extra: dev
 Requires-Dist: pytest-shell; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
 Requires-Dist: types-python-dateutil; extra == "dev"
 Requires-Dist: black>=24.1.1; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
```

### Comparing `otf_addons_vault-24.18.0/tests/test_plugin_vault.py` & `otf_addons_vault-24.18.1/tests/test_plugin_vault.py`

 * *Files identical despite different names*

