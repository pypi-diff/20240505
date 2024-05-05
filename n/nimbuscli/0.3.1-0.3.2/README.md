# Comparing `tmp/nimbuscli-0.3.1.tar.gz` & `tmp/nimbuscli-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nimbuscli-0.3.1.tar", max compression
+gzip compressed data, was "nimbuscli-0.3.2.tar", max compression
```

## Comparing `nimbuscli-0.3.1.tar` & `nimbuscli-0.3.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1076 2024-04-06 17:01:14.207734 nimbuscli-0.3.1/LICENSE
--rw-r--r--   0        0        0     5301 2024-05-01 13:53:13.104977 nimbuscli-0.3.1/README.md
--rw-r--r--   0        0        0     1713 2024-05-01 14:01:19.284886 nimbuscli-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-01 13:05:12.425472 nimbuscli-0.3.1/src/nimbuscli/__init__.py
--rw-r--r--   0        0        0      132 2024-05-01 13:44:37.705072 nimbuscli-0.3.1/src/nimbuscli/cli/__init__.py
--rw-r--r--   0        0        0     1523 2024-05-01 13:44:37.705072 nimbuscli-0.3.1/src/nimbuscli/cli/factory.py
--rw-r--r--   0        0        0     1356 2024-05-01 13:47:12.705050 nimbuscli-0.3.1/src/nimbuscli/cli/parser.py
--rw-r--r--   0        0        0     1189 2024-05-01 13:44:37.705072 nimbuscli-0.3.1/src/nimbuscli/cli/runner.py
--rw-r--r--   0        0        0      209 2024-05-01 13:44:37.705072 nimbuscli-0.3.1/src/nimbuscli/cmd/__init__.py
--rw-r--r--   0        0        0     5503 2024-05-01 13:44:37.705072 nimbuscli-0.3.1/src/nimbuscli/cmd/backup.py
--rw-r--r--   0        0        0     3118 2024-05-01 13:05:12.435472 nimbuscli-0.3.1/src/nimbuscli/cmd/command.py
--rw-r--r--   0        0        0     3131 2024-05-01 13:44:37.705072 nimbuscli-0.3.1/src/nimbuscli/cmd/deploy.py
--rw-r--r--   0        0        0     4446 2024-05-01 13:44:37.705072 nimbuscli-0.3.1/src/nimbuscli/cmd/factory.py
--rw-r--r--   0        0        0     5473 2024-05-01 13:05:12.435472 nimbuscli-0.3.1/src/nimbuscli/config.py
--rw-r--r--   0        0        0      314 2024-05-01 13:44:37.705072 nimbuscli-0.3.1/src/nimbuscli/core/__init__.py
--rw-r--r--   0        0        0     4585 2024-05-01 13:44:37.665072 nimbuscli-0.3.1/src/nimbuscli/core/archiver.py
--rw-r--r--   0        0        0     3783 2024-05-01 13:05:12.435472 nimbuscli-0.3.1/src/nimbuscli/core/runner.py
--rw-r--r--   0        0        0     3102 2024-05-01 13:44:37.315072 nimbuscli-0.3.1/src/nimbuscli/core/service.py
--rw-r--r--   0        0        0     6727 2024-05-01 13:05:12.435472 nimbuscli-0.3.1/src/nimbuscli/core/uploader.py
--rw-r--r--   0        0        0     2333 2024-05-01 13:44:38.285072 nimbuscli-0.3.1/src/nimbuscli/log.py
--rw-r--r--   0        0        0     4642 2024-05-01 13:44:38.255072 nimbuscli-0.3.1/src/nimbuscli/main.py
--rw-r--r--   0        0        0      192 2024-05-01 13:44:37.315072 nimbuscli-0.3.1/src/nimbuscli/notify/__init__.py
--rw-r--r--   0        0        0     4770 2024-05-01 13:44:37.315072 nimbuscli-0.3.1/src/nimbuscli/notify/discord.py
--rw-r--r--   0        0        0     1191 2024-05-01 13:44:37.315072 nimbuscli-0.3.1/src/nimbuscli/notify/factory.py
--rw-r--r--   0        0        0     1043 2024-05-01 13:44:37.315072 nimbuscli-0.3.1/src/nimbuscli/notify/notifier.py
--rw-r--r--   0        0        0      326 2024-05-01 13:44:37.315072 nimbuscli-0.3.1/src/nimbuscli/provider/__init__.py
--rw-r--r--   0        0        0      758 2024-05-01 13:44:37.285072 nimbuscli-0.3.1/src/nimbuscli/provider/directory.py
--rw-r--r--   0        0        0     2084 2024-05-01 13:05:12.435472 nimbuscli-0.3.1/src/nimbuscli/provider/resource.py
--rw-r--r--   0        0        0     1868 2024-05-01 13:05:12.435472 nimbuscli-0.3.1/src/nimbuscli/provider/secret.py
--rw-r--r--   0        0        0     3322 2024-05-01 13:44:37.275072 nimbuscli-0.3.1/src/nimbuscli/provider/service.py
--rw-r--r--   0        0        0      208 2024-05-01 13:44:37.095072 nimbuscli-0.3.1/src/nimbuscli/report/__init__.py
--rw-r--r--   0        0        0     2843 2024-05-01 13:44:37.095072 nimbuscli-0.3.1/src/nimbuscli/report/factory.py
--rw-r--r--   0        0        0     5712 2024-05-01 13:05:12.435472 nimbuscli-0.3.1/src/nimbuscli/report/format.py
--rw-r--r--   0        0        0    17618 2024-05-01 13:44:37.095072 nimbuscli-0.3.1/src/nimbuscli/report/reporter.py
--rw-r--r--   0        0        0     5275 2024-05-01 13:05:12.435472 nimbuscli-0.3.1/src/nimbuscli/report/writer.py
--rw-r--r--   0        0        0     5962 1970-01-01 00:00:00.000000 nimbuscli-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-05 12:53:29.436983 nimbuscli-0.3.2/LICENSE
+-rw-r--r--   0        0        0     5027 2024-05-05 12:53:29.436983 nimbuscli-0.3.2/README.md
+-rw-r--r--   0        0        0     2339 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/__init__.py
+-rw-r--r--   0        0        0      132 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/cli/__init__.py
+-rw-r--r--   0        0        0     1523 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/cli/factory.py
+-rw-r--r--   0        0        0     1356 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/cli/parser.py
+-rw-r--r--   0        0        0     1189 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/cli/runner.py
+-rw-r--r--   0        0        0      209 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/cmd/__init__.py
+-rw-r--r--   0        0        0     5528 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/cmd/backup.py
+-rw-r--r--   0        0        0     3118 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/cmd/command.py
+-rw-r--r--   0        0        0     3131 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/cmd/deploy.py
+-rw-r--r--   0        0        0     4471 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/cmd/factory.py
+-rw-r--r--   0        0        0     5473 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/config.py
+-rw-r--r--   0        0        0      314 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/core/__init__.py
+-rw-r--r--   0        0        0     4585 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/core/archiver.py
+-rw-r--r--   0        0        0     3783 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/core/runner.py
+-rw-r--r--   0        0        0     3102 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/core/service.py
+-rw-r--r--   0        0        0     6727 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/core/uploader.py
+-rw-r--r--   0        0        0     2333 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/log.py
+-rw-r--r--   0        0        0     4642 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/main.py
+-rw-r--r--   0        0        0      192 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/notify/__init__.py
+-rw-r--r--   0        0        0     4770 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/notify/discord.py
+-rw-r--r--   0        0        0     1191 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/notify/factory.py
+-rw-r--r--   0        0        0     1043 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/notify/notifier.py
+-rw-r--r--   0        0        0      326 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/provider/__init__.py
+-rw-r--r--   0        0        0      758 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/provider/directory.py
+-rw-r--r--   0        0        0     2084 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/provider/resource.py
+-rw-r--r--   0        0        0     1868 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/provider/secret.py
+-rw-r--r--   0        0        0     3322 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/provider/service.py
+-rw-r--r--   0        0        0      208 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/report/__init__.py
+-rw-r--r--   0        0        0     2843 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/report/factory.py
+-rw-r--r--   0        0        0     5712 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/report/format.py
+-rw-r--r--   0        0        0    17618 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/report/reporter.py
+-rw-r--r--   0        0        0     5275 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/report/writer.py
+-rw-r--r--   0        0        0     6316 1970-01-01 00:00:00.000000 nimbuscli-0.3.2/PKG-INFO
```

### Comparing `nimbuscli-0.3.1/LICENSE` & `nimbuscli-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.1/README.md` & `nimbuscli-0.3.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -33,31 +33,19 @@
 Install `ni` with [pipx](https://pipx.pypa.io/stable/) or `pip`:
 
 ```bash
 pip install nimbuscli
 ni --version
 ```
 
-Alternatively you can build it from source. Nimbus uses [poetry](https://python-poetry.org/) for dependency management and packaging.  
+To do something with nimbus you need to:
+  - Setup application configuration
+  - Install `docker`
+  - Install `rar`
 
-```bash
-pipx ensurepath
-pipx install poetry
-
-curl https://pyenv.run | bash
-
-pyenv install 3.12
-pyenv virtualenv 3.12 ni_env
-pyenv local ni_env
-
-poetry install
-ni --version
-```
-
-To do something with nimbus you need to setup the application configuration.
 For guidance and examples on setting up your configuration, please refer to the [configuration example](./docs/config.example.yaml).  
 
 ## Usage
 
 By default, Nimbus searches for its configuration file at the `~/.nimbus/config.yaml` path.  
 It is anticipated that all configurations for the application will be centralized within this file.
```

### Comparing `nimbuscli-0.3.1/pyproject.toml` & `nimbuscli-0.3.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,35 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nimbuscli"
-version = "0.3.1"
+version = "0.3.2"
 description = "Nimbus is engineered to optimize data backup processes and efficiently orchestrate service deployments."
+repository = "https://github.com/weak-head/nimbus"
 keywords = ["backup", "deploy", "administration"]
 authors = ["Oleksandr Zinchenko <zinchenko@live.com>"]
 readme = "README.md"
 license = "MIT"
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Environment :: Console",
+    "Intended Audience :: Developers",
+    "Intended Audience :: System Administrators",
+    "Intended Audience :: Information Technology",
+    "License :: OSI Approved :: MIT License",
+    "Natural Language :: English",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3.13",
+    "Topic :: System :: Archiving :: Backup",
+    "Topic :: System :: Systems Administration",
+    "Topic :: Utilities",
+]
 
 [tool.poetry.dependencies]
 python = "^3.12"
 boto3 = "^1.34"
 logdecorator = "^2.4"
 requests = "^2.31.0"
 strictyaml = "^1.7.3"
```

### Comparing `nimbuscli-0.3.1/src/nimbuscli/cli/factory.py` & `nimbuscli-0.3.2/src/nimbuscli/cli/factory.py`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.1/src/nimbuscli/cli/parser.py` & `nimbuscli-0.3.2/src/nimbuscli/cli/parser.py`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.1/src/nimbuscli/cli/runner.py` & `nimbuscli-0.3.2/src/nimbuscli/cli/runner.py`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.1/src/nimbuscli/cmd/backup.py` & `nimbuscli-0.3.2/src/nimbuscli/cmd/backup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,21 @@
 from datetime import datetime
 from pathlib import Path
 from typing import Any
 
 from logdecorator import log_on_end, log_on_start
 
 from nimbuscli.cmd.command import Action, ActionResult, Command
-from nimbuscli.core import ArchivalStatus, Archiver, Uploader, UploadProgress, UploadStatus
+from nimbuscli.core import (
+    ArchivalStatus,
+    Archiver,
+    Uploader,
+    UploadProgress,
+    UploadStatus,
+)
 from nimbuscli.provider import DirectoryProvider, DirectoryResource
 
 
 class Backup(Command):
     """
     Create and upload backups.
     """
```

### Comparing `nimbuscli-0.3.1/src/nimbuscli/cmd/command.py` & `nimbuscli-0.3.2/src/nimbuscli/cmd/command.py`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.1/src/nimbuscli/cmd/deploy.py` & `nimbuscli-0.3.2/src/nimbuscli/cmd/deploy.py`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.1/src/nimbuscli/cmd/factory.py` & `nimbuscli-0.3.2/src/nimbuscli/cmd/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,21 @@
 
 from logdecorator import log_on_end, log_on_error, log_on_start
 
 from nimbuscli.cmd.backup import Backup
 from nimbuscli.cmd.command import Command
 from nimbuscli.cmd.deploy import Down, Up
 from nimbuscli.config import Config
-from nimbuscli.core import Archiver, AwsUploader, RarArchiver, SubprocessRunner, Uploader
+from nimbuscli.core import (
+    Archiver,
+    AwsUploader,
+    RarArchiver,
+    SubprocessRunner,
+    Uploader,
+)
 from nimbuscli.provider import (
     DirectoryProvider,
     Secrets,
     SecretsProvider,
     ServiceFactory,
     ServiceProvider,
 )
```

### Comparing `nimbuscli-0.3.1/src/nimbuscli/config.py` & `nimbuscli-0.3.2/src/nimbuscli/config.py`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.1/src/nimbuscli/core/archiver.py` & `nimbuscli-0.3.2/src/nimbuscli/core/archiver.py`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.1/src/nimbuscli/core/runner.py` & `nimbuscli-0.3.2/src/nimbuscli/core/runner.py`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.1/src/nimbuscli/core/service.py` & `nimbuscli-0.3.2/src/nimbuscli/core/service.py`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.1/src/nimbuscli/core/uploader.py` & `nimbuscli-0.3.2/src/nimbuscli/core/uploader.py`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.1/src/nimbuscli/log.py` & `nimbuscli-0.3.2/src/nimbuscli/log.py`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.1/src/nimbuscli/main.py` & `nimbuscli-0.3.2/src/nimbuscli/main.py`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.1/src/nimbuscli/notify/discord.py` & `nimbuscli-0.3.2/src/nimbuscli/notify/discord.py`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.1/src/nimbuscli/notify/factory.py` & `nimbuscli-0.3.2/src/nimbuscli/notify/factory.py`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.1/src/nimbuscli/notify/notifier.py` & `nimbuscli-0.3.2/src/nimbuscli/notify/notifier.py`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.1/src/nimbuscli/provider/directory.py` & `nimbuscli-0.3.2/src/nimbuscli/provider/directory.py`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.1/src/nimbuscli/provider/resource.py` & `nimbuscli-0.3.2/src/nimbuscli/provider/resource.py`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.1/src/nimbuscli/provider/secret.py` & `nimbuscli-0.3.2/src/nimbuscli/provider/secret.py`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.1/src/nimbuscli/provider/service.py` & `nimbuscli-0.3.2/src/nimbuscli/provider/service.py`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.1/src/nimbuscli/report/factory.py` & `nimbuscli-0.3.2/src/nimbuscli/report/factory.py`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.1/src/nimbuscli/report/format.py` & `nimbuscli-0.3.2/src/nimbuscli/report/format.py`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.1/src/nimbuscli/report/reporter.py` & `nimbuscli-0.3.2/src/nimbuscli/report/reporter.py`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.1/src/nimbuscli/report/writer.py` & `nimbuscli-0.3.2/src/nimbuscli/report/writer.py`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.1/PKG-INFO` & `nimbuscli-0.3.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,36 @@
 Metadata-Version: 2.1
 Name: nimbuscli
-Version: 0.3.1
+Version: 0.3.2
 Summary: Nimbus is engineered to optimize data backup processes and efficiently orchestrate service deployments.
+Home-page: https://github.com/weak-head/nimbus
 License: MIT
 Keywords: backup,deploy,administration
 Author: Oleksandr Zinchenko
 Author-email: zinchenko@live.com
 Requires-Python: >=3.12,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
+Classifier: Topic :: System :: Archiving :: Backup
+Classifier: Topic :: System :: Systems Administration
+Classifier: Topic :: Utilities
 Requires-Dist: boto3 (>=1.34,<2.0)
 Requires-Dist: logdecorator (>=2.4,<3.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: strictyaml (>=1.7.3,<2.0.0)
+Project-URL: Repository, https://github.com/weak-head/nimbus
 Description-Content-Type: text/markdown
 
 <div align="center">
 
   <img src="https://raw.githubusercontent.com/weak-head/nimbus/main/docs/logo.png" width="450" />
   
   # nimbus <!-- omit from toc --> 
@@ -51,31 +64,19 @@
 Install `ni` with [pipx](https://pipx.pypa.io/stable/) or `pip`:
 
 ```bash
 pip install nimbuscli
 ni --version
 ```
 
-Alternatively you can build it from source. Nimbus uses [poetry](https://python-poetry.org/) for dependency management and packaging.  
+To do something with nimbus you need to:
+  - Setup application configuration
+  - Install `docker`
+  - Install `rar`
 
-```bash
-pipx ensurepath
-pipx install poetry
-
-curl https://pyenv.run | bash
-
-pyenv install 3.12
-pyenv virtualenv 3.12 ni_env
-pyenv local ni_env
-
-poetry install
-ni --version
-```
-
-To do something with nimbus you need to setup the application configuration.
 For guidance and examples on setting up your configuration, please refer to the [configuration example](./docs/config.example.yaml).  
 
 ## Usage
 
 By default, Nimbus searches for its configuration file at the `~/.nimbus/config.yaml` path.  
 It is anticipated that all configurations for the application will be centralized within this file.
```

