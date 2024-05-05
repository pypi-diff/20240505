# Comparing `tmp/yamapan-0.0.2.tar.gz` & `tmp/yamapan-0.0.3.tar.gz`

## Comparing `yamapan-0.0.2.tar` & `yamapan-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 yamapan-0.0.2/.python-version
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 yamapan-0.0.2/requirements-dev.lock
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 yamapan-0.0.2/requirements.lock
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 yamapan-0.0.2/src/yamapan/__init__.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 yamapan-0.0.2/src/yamapan/__main__.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 yamapan-0.0.2/src/yamapan/alias.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 yamapan-0.0.2/src/yamapan/build.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 yamapan-0.0.2/src/yamapan/clean.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 yamapan-0.0.2/src/yamapan/config.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 yamapan-0.0.2/src/yamapan/init.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 yamapan-0.0.2/src/yamapan/resolve.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 yamapan-0.0.2/src/yamapan/ros2.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 yamapan-0.0.2/src/yamapan/rqt.py
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 yamapan-0.0.2/src/yamapan/util.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 yamapan-0.0.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 yamapan-0.0.2/LICENSE
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 yamapan-0.0.2/README.md
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 yamapan-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    13502 2020-02-02 00:00:00.000000 yamapan-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 yamapan-0.0.3/.python-version
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 yamapan-0.0.3/requirements-dev.lock
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 yamapan-0.0.3/requirements.lock
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 yamapan-0.0.3/src/yamapan/__init__.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 yamapan-0.0.3/src/yamapan/__main__.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 yamapan-0.0.3/src/yamapan/alias.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 yamapan-0.0.3/src/yamapan/build.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 yamapan-0.0.3/src/yamapan/clean.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 yamapan-0.0.3/src/yamapan/config.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 yamapan-0.0.3/src/yamapan/init.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 yamapan-0.0.3/src/yamapan/resolve.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 yamapan-0.0.3/src/yamapan/ros2.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 yamapan-0.0.3/src/yamapan/rqt.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 yamapan-0.0.3/src/yamapan/util.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 yamapan-0.0.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 yamapan-0.0.3/LICENSE
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 yamapan-0.0.3/README.md
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 yamapan-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0    13554 2020-02-02 00:00:00.000000 yamapan-0.0.3/PKG-INFO
```

### Comparing `yamapan-0.0.2/src/yamapan/__init__.py` & `yamapan-0.0.3/src/yamapan/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from argparse import ArgumentParser, Namespace
 from typing import Callable
 
 parser = ArgumentParser(
     prog="yamapan",
     description="Yet Another MetA worksPAce maNager for ROS 2",
 )
-parser.add_argument("-v", "--version", action="version", version="%(prog)s 0.0.2")
+parser.add_argument("-v", "--version", action="version", version="%(prog)s 0.0.3")
 subparsers = parser.add_subparsers()
 
 
 def subcommand(name: str):
-    def _subcommand(handler: Callable[[Namespace], int]):
+    def _subcommand(handler: Callable[[Namespace, list[str]], int]):
         parser = subparsers.add_parser(name)
         parser.set_defaults(handler=handler)
         return parser
 
     return _subcommand
 
 
 def main() -> int:
-    args = parser.parse_args()
-    if hasattr(args, "handler"):
-        return args.handler(args)
+    namespace, args = parser.parse_known_args()
+    if hasattr(namespace, "handler"):
+        return namespace.handler(namespace, args)
     else:
         parser.print_help()
         return 1
 
 
 import yamapan.alias as _
 import yamapan.build as _
```

### Comparing `yamapan-0.0.2/src/yamapan/alias.py` & `yamapan-0.0.3/src/yamapan/alias.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 from argparse import Namespace
 
 from yamapan import subcommand
 from yamapan.util import get_workspace_path, load_config, run_command
 
 
 @subcommand("alias")
-def alias(args: Namespace) -> int:
+def alias(namespace: Namespace, args: list[str]) -> int:
     workspace_path = get_workspace_path()
     config = load_config()
-    alias = config.aliases.get(args.name)
+    alias = config.aliases.get(namespace.name)
     if alias is None:
-        sys.exit(f"yamapan: alias not found: '{args.name}'")
+        sys.exit(f"yamapan: alias not found: '{namespace.name}'")
     return run_command(
-        f"{alias} {' '.join(args.args)}",
+        f"{alias} {' '.join(args)}",
         cwd=workspace_path,
     )
 
 
 alias.add_argument("name", help="alias name")
-alias.add_argument("args", nargs="*", help="passed to the aliased command")
```

### Comparing `yamapan-0.0.2/src/yamapan/config.py` & `yamapan-0.0.3/src/yamapan/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 from typing import Any
 
 from pydantic import BaseModel
 
 CONFIG_FILENAME = "yamapan.toml"
 CONFIG_TEMPLATE = """[aliases]
-# build = "yamapan build -- --cmake-args -DCMAKE_C_COMPILER_LAUNCHER=ccache -DCMAKE_CXX_COMPILER_LAUNCHER=ccache"
+# build = "yamapan build --cmake-args -DCMAKE_C_COMPILER_LAUNCHER=ccache -DCMAKE_CXX_COMPILER_LAUNCHER=ccache"
 
 [repositories]
 # "ext/voicevox_ros2" = { type = "git", url = "https://github.com/tutrobo/voicevox_ros2.git", version = "master" }
 """
 
 LOCAL_CONFIG_FILENAME = "yamapan.local.toml"
 LOCAL_CONFIG_TEMPLATE = """ros_install_prefix = "{}"
```

### Comparing `yamapan-0.0.2/src/yamapan/init.py` & `yamapan-0.0.3/src/yamapan/init.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,19 +8,19 @@
     GITIGNORE_TEMPLATE,
     LOCAL_CONFIG_FILENAME,
     LOCAL_CONFIG_TEMPLATE,
 )
 
 
 @subcommand("init")
-def init(args: Namespace) -> int:
+def init(namespace: Namespace, args: list[str]) -> int:
     with open(CONFIG_FILENAME, "w") as f:
         f.write(CONFIG_TEMPLATE)
     with open(LOCAL_CONFIG_FILENAME, "w") as f:
-        f.write(LOCAL_CONFIG_TEMPLATE.format(args.ros_install_prefix))
+        f.write(LOCAL_CONFIG_TEMPLATE.format(namespace.ros_install_prefix))
     with open(".gitignore", "w") as f:
         f.write(GITIGNORE_TEMPLATE)
     return 0
 
 
 init.add_argument(
     "--ros-install-prefix",
```

### Comparing `yamapan-0.0.2/src/yamapan/resolve.py` & `yamapan-0.0.3/src/yamapan/resolve.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import yaml
 
 from yamapan import subcommand
 from yamapan.util import get_workspace_path, load_config, run_command
 
 
 @subcommand("resolve")
-def resolve(_: Namespace) -> int:
+def resolve(namespace: Namespace, args: list[str]) -> int:
     workspace_path = get_workspace_path()
     config = load_config()
     ret = run_command(
         "vcs import",
         cwd=workspace_path,
         input=yaml.dump({"repositories": config.repositories}).encode(),
     )
```

### Comparing `yamapan-0.0.2/src/yamapan/util.py` & `yamapan-0.0.3/src/yamapan/util.py`

 * *Files identical despite different names*

### Comparing `yamapan-0.0.2/LICENSE` & `yamapan-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yamapan-0.0.2/pyproject.toml` & `yamapan-0.0.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "yamapan"
-version = "0.0.2"
+version = "0.0.3"
 description = "Yet Another MetA worksPAce maNager for ROS 2"
 license = {file = "LICENSE"}
 authors = [
     { name = "Rin Iwai", email = "rin@eyrin.jp" }
 ]
 dependencies = [
     "PyYAML>=6.0.1",
```

### Comparing `yamapan-0.0.2/PKG-INFO` & `yamapan-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: yamapan
-Version: 0.0.2
+Version: 0.0.3
 Summary: Yet Another MetA worksPAce maNager for ROS 2
 Project-URL: Repository, https://github.com/tutrobo/yamapan.git
 Author-email: Rin Iwai <rin@eyrin.jp>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -212,14 +212,20 @@
 Requires-Dist: tomli>=2.0.1
 Description-Content-Type: text/markdown
 
 # yamapan
 
 Yet Another MetA worksPAce maNager for ROS 2
 
+
+
 ## Getting Started
 
 ```sh
 pipx install yamapan
 cd <path-to-your-ros-2-workspace>
 yamapan init
 ```
+
+### Build the workspace
+
+### Clean the workspace
```

