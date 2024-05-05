# Comparing `tmp/pytest_ditto-0.0.1.tar.gz` & `tmp/pytest_ditto-0.0.2.tar.gz`

## Comparing `pytest_ditto-0.0.1.tar` & `pytest_ditto-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pytest_ditto-0.0.1/ditto/__init__.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 pytest_ditto-0.0.1/ditto/_unittest.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pytest_ditto-0.0.1/ditto/_version.py
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 pytest_ditto-0.0.1/ditto/plugin.py
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 pytest_ditto-0.0.1/ditto/snapshot.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 pytest_ditto-0.0.1/ditto/io/__init__.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 pytest_ditto-0.0.1/ditto/io/_json.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pytest_ditto-0.0.1/ditto/io/_pandas_parquet.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 pytest_ditto-0.0.1/ditto/io/_pickle.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 pytest_ditto-0.0.1/ditto/io/_yaml.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 pytest_ditto-0.0.1/ditto/io/protocol.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pytest_ditto-0.0.1/.gitignore
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 pytest_ditto-0.0.1/README.md
--rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 pytest_ditto-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 pytest_ditto-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pytest_ditto-0.0.2/ditto/__init__.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 pytest_ditto-0.0.2/ditto/_unittest.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pytest_ditto-0.0.2/ditto/_version.py
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 pytest_ditto-0.0.2/ditto/plugin.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 pytest_ditto-0.0.2/ditto/snapshot.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 pytest_ditto-0.0.2/ditto/io/__init__.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 pytest_ditto-0.0.2/ditto/io/_json.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 pytest_ditto-0.0.2/ditto/io/_pandas_parquet.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 pytest_ditto-0.0.2/ditto/io/_pickle.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 pytest_ditto-0.0.2/ditto/io/_protocol.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 pytest_ditto-0.0.2/ditto/io/_yaml.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pytest_ditto-0.0.2/.gitignore
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 pytest_ditto-0.0.2/README.md
+-rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 pytest_ditto-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 pytest_ditto-0.0.2/PKG-INFO
```

### Comparing `pytest_ditto-0.0.1/ditto/_unittest.py` & `pytest_ditto-0.0.2/ditto/_unittest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 import inspect
 from typing import ClassVar
 from pathlib import Path
 
-from ditto.snapshot import Snapshot
+from ditto import Snapshot
 
 
 def _calling_test_path() -> Path:
     frame = inspect.currentframe()
     outer_frames = inspect.getouterframes(frame)
     # 2 calls back up the stack, index 1 of the frame has the calling filepath
     return Path(outer_frames[2][1]).parent
@@ -22,8 +22,8 @@
         path = _calling_test_path() / ".ditto"
         path.mkdir(exist_ok=True)
 
         return Snapshot(
             path=path,
             name=".".join(self.id().split(".")[-3:]),
             record=self.record,
-        )
+        )
```

### Comparing `pytest_ditto-0.0.1/pyproject.toml` & `pytest_ditto-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -45,25 +45,25 @@
 requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 
 [tool.hatch.build]
 hooks.vcs.version-file = "ditto/_version.py"
 hooks.vcs.template = "__version__ = {version!r}"
-
-[tool.hatch.build.targets.wheel]
-packages = ["ditto"]
-strict-naming = false
-
-[tool.hatch.build.targets.sdist]
-packages = ["ditto"]
-strict-naming = false
+targets.wheel.packages = ["ditto"]
+targets.wheel.strict-naming = false
+targets.sdist.packages = ["ditto"]
+targets.sdist.strict-naming = false
 
 [tool.hatch.version]
-source = "vcs"
+#source = "vcs"
+source = "code"
+path = "version_builder.py"
+expression = "_version()"
+
 
 [tool.hatch.envs.default]
 python = "3.10"
 dependencies = [
   "pytest",
 ]
 
@@ -82,15 +82,15 @@
     # note the use of single quote below to denote "raw" strings in TOML
     'ignore::DeprecationWarning',
 ]
 
 
 [tool.black]
 line-length = 88
-target-version = ['py38', 'py39', 'py310', 'py311', 'py312']
+target-version = ['py310', 'py311', 'py312']
 exclude = '''
 # A regex preceded with ^/ will apply only to files and directories
 # in the root of the project.
 ^/(
   (
       \.eggs
     | \.git
```

### Comparing `pytest_ditto-0.0.1/PKG-INFO` & `pytest_ditto-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pytest-ditto
-Version: 0.0.1
+Version: 0.0.2
 Author-email: Lachlan Taylor <lachlanbtaylor@proton.me>
 Maintainer-email: Lachlan Taylor <lachlanbtaylor@proton.me>
 License-Expression: MIT
 Keywords: pytest
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
```

