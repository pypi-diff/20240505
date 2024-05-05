# Comparing `tmp/pyyaml-include-2.0b2.tar.gz` & `tmp/pyyaml_include-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyyaml-include-2.0b2.tar", last modified: Wed Mar 27 03:52:18 2024, max compression
+gzip compressed data, was "pyyaml_include-2.1.tar", last modified: Sun May  5 08:21:15 2024, max compression
```

## Comparing `pyyaml-include-2.0b2.tar` & `pyyaml_include-2.1.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 03:52:18.249694 pyyaml-include-2.0b2/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-27 03:52:11.000000 pyyaml-include-2.0b2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-03-27 03:52:11.000000 pyyaml-include-2.0b2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-03-27 03:52:11.000000 pyyaml-include-2.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-27 03:52:11.000000 pyyaml-include-2.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    18477 2024-03-27 03:52:18.249694 pyyaml-include-2.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16929 2024-03-27 03:52:11.000000 pyyaml-include-2.0b2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-03-27 03:52:11.000000 pyyaml-include-2.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 03:52:18.249694 pyyaml-include-2.0b2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 03:52:18.245694 pyyaml-include-2.0b2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 03:52:18.249694 pyyaml-include-2.0b2/src/pyyaml_include.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18477 2024-03-27 03:52:18.000000 pyyaml-include-2.0b2/src/pyyaml_include.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-27 03:52:18.000000 pyyaml-include-2.0b2/src/pyyaml_include.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 03:52:18.000000 pyyaml-include-2.0b2/src/pyyaml_include.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-27 03:52:18.000000 pyyaml-include-2.0b2/src/pyyaml_include.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-27 03:52:18.000000 pyyaml-include-2.0b2/src/pyyaml_include.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 03:52:18.249694 pyyaml-include-2.0b2/src/yaml_include/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-27 03:52:11.000000 pyyaml-include-2.0b2/src/yaml_include/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-27 03:52:11.000000 pyyaml-include-2.0b2/src/yaml_include/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-27 03:52:18.000000 pyyaml-include-2.0b2/src/yaml_include/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    15763 2024-03-27 03:52:11.000000 pyyaml-include-2.0b2/src/yaml_include/constructor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-03-27 03:52:11.000000 pyyaml-include-2.0b2/src/yaml_include/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-03-27 03:52:11.000000 pyyaml-include-2.0b2/src/yaml_include/funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-03-27 03:52:11.000000 pyyaml-include-2.0b2/src/yaml_include/representer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-03-27 03:52:11.000000 pyyaml-include-2.0b2/src/yaml_include/yaml_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-03-27 03:52:11.000000 pyyaml-include-2.0b2/src/yaml_include/yaml_types_backward.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:21:15.776553 pyyaml_include-2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-05 08:21:04.000000 pyyaml_include-2.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-05-05 08:21:04.000000 pyyaml_include-2.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-05 08:21:04.000000 pyyaml_include-2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-05 08:21:04.000000 pyyaml_include-2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18769 2024-05-05 08:21:15.776553 pyyaml_include-2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16918 2024-05-05 08:21:04.000000 pyyaml_include-2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-05 08:21:04.000000 pyyaml_include-2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 08:21:15.776553 pyyaml_include-2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:21:15.772553 pyyaml_include-2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:21:15.776553 pyyaml_include-2.1/src/pyyaml_include.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18769 2024-05-05 08:21:15.000000 pyyaml_include-2.1/src/pyyaml_include.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-05 08:21:15.000000 pyyaml_include-2.1/src/pyyaml_include.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 08:21:15.000000 pyyaml_include-2.1/src/pyyaml_include.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-05 08:21:15.000000 pyyaml_include-2.1/src/pyyaml_include.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-05 08:21:15.000000 pyyaml_include-2.1/src/pyyaml_include.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:21:15.776553 pyyaml_include-2.1/src/yaml_include/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-05 08:21:04.000000 pyyaml_include-2.1/src/yaml_include/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-05 08:21:04.000000 pyyaml_include-2.1/src/yaml_include/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-05 08:21:15.000000 pyyaml_include-2.1/src/yaml_include/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17582 2024-05-05 08:21:04.000000 pyyaml_include-2.1/src/yaml_include/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-05 08:21:04.000000 pyyaml_include-2.1/src/yaml_include/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-05-05 08:21:04.000000 pyyaml_include-2.1/src/yaml_include/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 08:21:04.000000 pyyaml_include-2.1/src/yaml_include/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-05 08:21:04.000000 pyyaml_include-2.1/src/yaml_include/representer.py
```

### Comparing `pyyaml-include-2.0b2/CHANGELOG.md` & `pyyaml_include-2.1/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,34 @@
-# Changelog
+# CHANGELOG
+
+## 2.1
+
+> 📅 **Date** 2024-5-5
+
+- Better type hints
+- Some optimizations and bugfix
+
+## 2.0.2
+
+> 📅 **Date** 2024-4-20
+
+- Remove custom PyYAML types definition module, use that from `types-PyYAML` instead.
+- Add [mypy](https://www.mypy-lang.org/) hook in pre-commit
+- Better type hints/annotations
+
+## 2.0.1
+
+> 📅 **Date** 2024-4-9
+
+- 🆕 New Features:
+  - #44: Add `py.typed` file, make the package PEP-561 friendly
+
+## 2.0
+
+> 📅 **Date** 2024-3-31
 
 ## 2.0b2
 
 > 📅 **Date** 2024-3-27
 
 - ❎ Breaking Changes:
   - data-class attribute order changed in `yaml_include.Constructor`
```

### Comparing `pyyaml-include-2.0b2/LICENSE` & `pyyaml_include-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyyaml-include-2.0b2/PKG-INFO` & `pyyaml_include-2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,78 +1,84 @@
 Metadata-Version: 2.1
 Name: pyyaml-include
-Version: 2.0b2
+Version: 2.1
 Summary: An extending constructor of PyYAML: include other YAML files into current YAML document
 Author-email: liu xue yan <liu_xue_yan@foxmail.com>
 License: GPLv3+
 Project-URL: Homepage, https://github.com/tanbro/pyyaml-include
 Project-URL: Repository, https://github.com/tanbro/pyyaml-include.git
 Project-URL: Documentation, https://pyyaml-include.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/tanbro/pyyaml-include/issues
 Project-URL: Changelog, https://github.com/tanbro/pyyaml-include/blob/main/CHANGELOG.md
 Keywords: yaml,PyYAML,include,yml
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
-Requires-Dist: PyYAML<7.0,>=6.0
+Requires-Dist: PyYAML~=6.0
 Requires-Dist: fsspec>=2021.04.0
 Requires-Dist: typing-extensions; python_version < "3.11"
 
 # pyyaml-include
 
 [![GitHub tag](https://img.shields.io/github/tag/tanbro/pyyaml-include.svg)](https://github.com/tanbro/pyyaml-include)
 [![Python Package](https://github.com/tanbro/pyyaml-include/workflows/Python%20package/badge.svg)](https://github.com/tanbro/pyyaml-include/actions?query=workflow%3A%22Python+package%22)
 [![Documentation Status](https://readthedocs.org/projects/pyyaml-include/badge/?version=latest)](https://pyyaml-include.readthedocs.io/en/latest/)
 [![PyPI](https://img.shields.io/pypi/v/pyyaml-include.svg)](https://pypi.org/project/pyyaml-include/)
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=tanbro_pyyaml-include&metric=alert_status)](https://sonarcloud.io/dashboard?id=tanbro_pyyaml-include)
 
 An extending constructor of [PyYAML][]: include other [YAML][] files into current [YAML][] document.
 
-With [fsspec][], we can even include files by HTTP, SFTP, S3 ...
+In version `2.0`, [fsspec][] was introduced. With it, we can even include files by HTTP, SFTP, S3 ...
+
+> ⚠️ **Warning** \
+> “pyyaml-include” `2.0` is **NOT compatible** with `1.0`
 
 ## Install
 
 ```bash
-pip install --pre "pyyaml-include>=2.0"
+pip install "pyyaml-include"
 ```
 
 Since we are using [fsspec][] to open including files from v2.0, an installation can be performed like below, if want to open remote files:
 
 - for files on website:
 
   ```bash
-  pip install --pre "pyyaml-include>=2.0" fsspec[http]
+  pip install "pyyaml-include" fsspec[http]
   ```
 
 - for files on S3:
 
   ```bash
-  pip install --pre "pyyaml-include>=2.0" fsspec[s3]
+  pip install "pyyaml-include" fsspec[s3]
   ```
 
 - see [fsspec][]'s documentation for more
 
 > 🔖 **Tip** \
->
-> - “pyyaml-include” depends on [fsspec][], which will be installed no matter including local or remote files.
-> - It's advised to use the library on Python version `>=3.8`, early versions are not guaranteed.
+> “pyyaml-include” depends on [fsspec][], it will be installed no matter including local or remote files.
 
 ## Basic usages
 
 Consider we have such [YAML][] files:
 
 ```
 ├── 0.yml
@@ -446,15 +452,15 @@
 
 the actual URL to access is `http://$HOST:$PORT/sub_1/sub_1_1/xyz.yml`
 
 ### Serialization
 
 When load [YAML][] string with include statement, the including files are default parsed into python objects. Thant is, if we call `yaml.dump()` on the object, what dumped is the parsed python object, and can not serialize the include statement itself.
 
-To serialize the statement, we shall first create an `yaml_include.Constructor` object whose `autoload` is `False`:
+To serialize the statement, we shall first create an `yaml_include.Constructor` object whose **`autoload` is `False`**:
 
 ```python
 import yaml
 import yaml_include
 
 ctor = yaml_include.Constructor(autoload=False)
 ```
```

### Comparing `pyyaml-include-2.0b2/README.md` & `pyyaml_include-2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,42 +4,43 @@
 [![Python Package](https://github.com/tanbro/pyyaml-include/workflows/Python%20package/badge.svg)](https://github.com/tanbro/pyyaml-include/actions?query=workflow%3A%22Python+package%22)
 [![Documentation Status](https://readthedocs.org/projects/pyyaml-include/badge/?version=latest)](https://pyyaml-include.readthedocs.io/en/latest/)
 [![PyPI](https://img.shields.io/pypi/v/pyyaml-include.svg)](https://pypi.org/project/pyyaml-include/)
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=tanbro_pyyaml-include&metric=alert_status)](https://sonarcloud.io/dashboard?id=tanbro_pyyaml-include)
 
 An extending constructor of [PyYAML][]: include other [YAML][] files into current [YAML][] document.
 
-With [fsspec][], we can even include files by HTTP, SFTP, S3 ...
+In version `2.0`, [fsspec][] was introduced. With it, we can even include files by HTTP, SFTP, S3 ...
+
+> ⚠️ **Warning** \
+> “pyyaml-include” `2.0` is **NOT compatible** with `1.0`
 
 ## Install
 
 ```bash
-pip install --pre "pyyaml-include>=2.0"
+pip install "pyyaml-include"
 ```
 
 Since we are using [fsspec][] to open including files from v2.0, an installation can be performed like below, if want to open remote files:
 
 - for files on website:
 
   ```bash
-  pip install --pre "pyyaml-include>=2.0" fsspec[http]
+  pip install "pyyaml-include" fsspec[http]
   ```
 
 - for files on S3:
 
   ```bash
-  pip install --pre "pyyaml-include>=2.0" fsspec[s3]
+  pip install "pyyaml-include" fsspec[s3]
   ```
 
 - see [fsspec][]'s documentation for more
 
 > 🔖 **Tip** \
->
-> - “pyyaml-include” depends on [fsspec][], which will be installed no matter including local or remote files.
-> - It's advised to use the library on Python version `>=3.8`, early versions are not guaranteed.
+> “pyyaml-include” depends on [fsspec][], it will be installed no matter including local or remote files.
 
 ## Basic usages
 
 Consider we have such [YAML][] files:
 
 ```
 ├── 0.yml
@@ -413,15 +414,15 @@
 
 the actual URL to access is `http://$HOST:$PORT/sub_1/sub_1_1/xyz.yml`
 
 ### Serialization
 
 When load [YAML][] string with include statement, the including files are default parsed into python objects. Thant is, if we call `yaml.dump()` on the object, what dumped is the parsed python object, and can not serialize the include statement itself.
 
-To serialize the statement, we shall first create an `yaml_include.Constructor` object whose `autoload` is `False`:
+To serialize the statement, we shall first create an `yaml_include.Constructor` object whose **`autoload` is `False`**:
 
 ```python
 import yaml
 import yaml_include
 
 ctor = yaml_include.Constructor(autoload=False)
 ```
```

### Comparing `pyyaml-include-2.0b2/pyproject.toml` & `pyyaml_include-2.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -7,41 +7,46 @@
 description = "An extending constructor of PyYAML: include other YAML files into current YAML document"
 name = "pyyaml-include"
 readme = "README.md"
 
 requires-python = ">=3.8"
 
 dependencies = [
-  "PyYAML>=6.0,<7.0",
+  "PyYAML~=6.0",
   "fsspec>=2021.04.0",
   "typing-extensions; python_version<'3.11'",
 ]
 
 keywords = ["yaml", "PyYAML", "include", "yml"]
 
 license = { text = "GPLv3+" }
 
 classifiers = [
   "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
   # "Development Status :: 1 - Planning",
   # "Development Status :: 2 - Pre-Alpha",
   # "Development Status :: 3 - Alpha",
-  "Development Status :: 4 - Beta",
-  # "Development Status :: 5 - Production/Stable",
+  # "Development Status :: 4 - Beta",
+  "Development Status :: 5 - Production/Stable",
   # "Development Status :: 6 - Mature",
   # "Development Status :: 7 - Inactive",
   "Intended Audience :: Developers",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.7",
+  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: 3.13",
+  "Programming Language :: Python :: Implementation :: CPython",
+  "Programming Language :: Python :: Implementation :: PyPy",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Topic :: Text Processing :: Markup",
 ]
 
 dynamic = ["version"]
 
 [project.urls]
@@ -50,9 +55,12 @@
 Documentation = "https://pyyaml-include.readthedocs.io/en/latest/"
 Issues = "https://github.com/tanbro/pyyaml-include/issues"
 Changelog = "https://github.com/tanbro/pyyaml-include/blob/main/CHANGELOG.md"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
+[tool.setuptools.package-data]
+pyyaml_include = ["yaml_include/py.typed"]
+
 [tool.setuptools_scm]
 write_to = "src/yaml_include/_version.py"
```

### Comparing `pyyaml-include-2.0b2/src/pyyaml_include.egg-info/PKG-INFO` & `pyyaml_include-2.1/src/pyyaml_include.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,78 +1,84 @@
 Metadata-Version: 2.1
 Name: pyyaml-include
-Version: 2.0b2
+Version: 2.1
 Summary: An extending constructor of PyYAML: include other YAML files into current YAML document
 Author-email: liu xue yan <liu_xue_yan@foxmail.com>
 License: GPLv3+
 Project-URL: Homepage, https://github.com/tanbro/pyyaml-include
 Project-URL: Repository, https://github.com/tanbro/pyyaml-include.git
 Project-URL: Documentation, https://pyyaml-include.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/tanbro/pyyaml-include/issues
 Project-URL: Changelog, https://github.com/tanbro/pyyaml-include/blob/main/CHANGELOG.md
 Keywords: yaml,PyYAML,include,yml
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
-Requires-Dist: PyYAML<7.0,>=6.0
+Requires-Dist: PyYAML~=6.0
 Requires-Dist: fsspec>=2021.04.0
 Requires-Dist: typing-extensions; python_version < "3.11"
 
 # pyyaml-include
 
 [![GitHub tag](https://img.shields.io/github/tag/tanbro/pyyaml-include.svg)](https://github.com/tanbro/pyyaml-include)
 [![Python Package](https://github.com/tanbro/pyyaml-include/workflows/Python%20package/badge.svg)](https://github.com/tanbro/pyyaml-include/actions?query=workflow%3A%22Python+package%22)
 [![Documentation Status](https://readthedocs.org/projects/pyyaml-include/badge/?version=latest)](https://pyyaml-include.readthedocs.io/en/latest/)
 [![PyPI](https://img.shields.io/pypi/v/pyyaml-include.svg)](https://pypi.org/project/pyyaml-include/)
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=tanbro_pyyaml-include&metric=alert_status)](https://sonarcloud.io/dashboard?id=tanbro_pyyaml-include)
 
 An extending constructor of [PyYAML][]: include other [YAML][] files into current [YAML][] document.
 
-With [fsspec][], we can even include files by HTTP, SFTP, S3 ...
+In version `2.0`, [fsspec][] was introduced. With it, we can even include files by HTTP, SFTP, S3 ...
+
+> ⚠️ **Warning** \
+> “pyyaml-include” `2.0` is **NOT compatible** with `1.0`
 
 ## Install
 
 ```bash
-pip install --pre "pyyaml-include>=2.0"
+pip install "pyyaml-include"
 ```
 
 Since we are using [fsspec][] to open including files from v2.0, an installation can be performed like below, if want to open remote files:
 
 - for files on website:
 
   ```bash
-  pip install --pre "pyyaml-include>=2.0" fsspec[http]
+  pip install "pyyaml-include" fsspec[http]
   ```
 
 - for files on S3:
 
   ```bash
-  pip install --pre "pyyaml-include>=2.0" fsspec[s3]
+  pip install "pyyaml-include" fsspec[s3]
   ```
 
 - see [fsspec][]'s documentation for more
 
 > 🔖 **Tip** \
->
-> - “pyyaml-include” depends on [fsspec][], which will be installed no matter including local or remote files.
-> - It's advised to use the library on Python version `>=3.8`, early versions are not guaranteed.
+> “pyyaml-include” depends on [fsspec][], it will be installed no matter including local or remote files.
 
 ## Basic usages
 
 Consider we have such [YAML][] files:
 
 ```
 ├── 0.yml
@@ -446,15 +452,15 @@
 
 the actual URL to access is `http://$HOST:$PORT/sub_1/sub_1_1/xyz.yml`
 
 ### Serialization
 
 When load [YAML][] string with include statement, the including files are default parsed into python objects. Thant is, if we call `yaml.dump()` on the object, what dumped is the parsed python object, and can not serialize the include statement itself.
 
-To serialize the statement, we shall first create an `yaml_include.Constructor` object whose `autoload` is `False`:
+To serialize the statement, we shall first create an `yaml_include.Constructor` object whose **`autoload` is `False`**:
 
 ```python
 import yaml
 import yaml_include
 
 ctor = yaml_include.Constructor(autoload=False)
 ```
```

### Comparing `pyyaml-include-2.0b2/src/yaml_include/constructor.py` & `pyyaml_include-2.1/src/yaml_include/constructor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,61 @@
 """
 Include other YAML files in YAML
 """
 
+from __future__ import annotations
+
 import re
 import sys
 from contextlib import contextmanager
 from dataclasses import dataclass, field
 from itertools import chain
 from os import PathLike
 from pathlib import Path
-from typing import Any, Callable, Generator, Optional, Union
+from typing import TYPE_CHECKING, Any, Callable, Generator, Iterable, Mapping, Optional, Sequence, Type, TypeVar, Union
+from urllib.parse import urlsplit, urlunsplit
 
-if sys.version_info < (3, 11):  # pragma: no cover
-    from typing_extensions import Self
+if sys.version_info >= (3, 10):  # pragma: no cover
+    from typing import TypeGuard
 else:  # pragma: no cover
-    from typing import Self
+    from typing_extensions import TypeGuard
 
-from urllib.parse import urlsplit, urlunsplit
+if sys.version_info >= (3, 11):  # pragma: no cover
+    from typing import Self
+else:  # pragma: no cover
+    from typing_extensions import Self
 
-import fsspec
+import fsspec  # type: ignore[import-untyped]
 import yaml
 
 from .data import Data
 
-if sys.version_info < (3, 12):  # pragma: no cover
-    from .yaml_types_backward import TYamlLoaderTypes
-else:  # pragma: no cover
-    from .yaml_types import TYamlLoaderTypes
+if TYPE_CHECKING:  # pragma: no cover
+    from yaml import Node
+    from yaml.constructor import _Scalar
+    from yaml.cyaml import _CLoader
+    from yaml.loader import _Loader
+    from yaml.reader import _ReadStream
+
+    _TOpenFile = TypeVar("_TOpenFile", bound=_ReadStream)
+    _TLoaderType = TypeVar("_TLoaderType", bound=Type[Union[_Loader, _CLoader]])
+
 
 __all__ = ["Constructor"]
 
 WILDCARDS_PATTERN = re.compile(
     r"^(.*)([\*\?\[\]]+)(.*)$"
 )  # We support "**", "?" and "[..]". We do not support "^" for pattern negation.
 
 
 def load_open_file(
-    file,
-    loader_type: TYamlLoaderTypes,
+    file: _TOpenFile,
+    loader_type: _TLoaderType,
     path: str,
-    custom_loader: Optional[Callable[[str, Any, TYamlLoaderTypes], Any]] = None,
+    custom_loader: Optional[Callable[[str, _TOpenFile, _TLoaderType], Any]] = None,
 ) -> Any:
     if custom_loader is None:
         return yaml.load(file, loader_type)
     return custom_loader(path, file, loader_type)
 
 
 @dataclass
@@ -61,44 +73,42 @@
 
             yaml.add_constructor("!inc", yaml_include.Constructor(), yaml.Loader)
 
         #. In a YAML file, write ``!inc`` tags to include other YAML files. We can:
 
             * include file in local file system, absolute or relative
 
-                .. code:: yaml
+                .. code-block:: yaml
 
                     file: !inc /absolute/dir/of/foo/baz.yml
 
-                .. code:: yaml
+                .. code-block:: yaml
 
                     file: !inc ../../foo/baz.yml
 
             * include file from a website
 
-                .. code:: yaml
+                .. code-block:: yaml
 
                     file: !inc http://localhost:8080/foo/baz.yml
 
             * include file by wildcards
 
-                .. code:: yaml
+                .. code-block:: yaml
 
                     files: !inc foo/**/*.yml
 
         #. load the YAML in python::
 
             data = yaml.load(yaml_string, yaml.Loader)
 
            The variable ``data`` containers the parsed Python object(s) from including file(s)
     """
 
-    fs: fsspec.AbstractFileSystem = field(
-        default_factory=lambda: fsspec.filesystem("file"),
-    )
+    fs: fsspec.AbstractFileSystem = field(default_factory=lambda: fsspec.filesystem("file"))
     """:mod:`fsspec` File-system object to parse path/url and open including files. `LocalFileSystem` by default."""
 
     base_dir: Union[str, PathLike, Callable[[], Union[str, PathLike]], None] = None
     """Base directory to which open or search including YAML files in relative mode.
 
     * If it is ``None``, the actual base directory was decided by the :mod:`fsspec` file-system implementation in use.
       For example, the ``base_dir`` is default to be ``cwd`` for ``LocalFileSystem``, and be the value of ``client_kwargs.base_url`` for ``HTTPFileSystem``.
@@ -111,15 +121,15 @@
 
     * If ``True``:
       open including file(s) then parse its/their content with current PyYAML Loader, and returns the parsed result.
     * If ``False``:
       will **NOT** open including file(s), the return value is a :class:`.Data` object stores include statement.
     """
 
-    custom_loader: Optional[Callable[[str, Any, TYamlLoaderTypes], Any]] = None
+    custom_loader: Optional[Callable[[str, _ReadStream, Type[Union[_Loader, _CLoader]]], Any]] = None
     """Custom loader/parser function called when an including file is about to parse.
 
     If ``None``, parse the file as ordinary YAML with current `Loader` class.
 
     Else it shall be a callable object, as the replacement of ordinary YAML `Loader`.
 
     Example:
@@ -143,178 +153,180 @@
 
             * Original url/path string defined in YAML, in the case of:
                 * neither wildcard nor scheme exists in the include statement (eg: ``!inc foo/baz.yml``),
                 * either wildcard and scheme exists in the include statement (eg: ``!inc http://host/foo/*.yml``)
             * Each file name returned by :meth:`fsspec.spec.AbstractFileSystem.glob`,
               if there be wildcard and no scheme in the include statement (eg: ``!inc foobar/**/*.yml``).
 
-        arg2(typing.Any):
-            What returned by :func:`fsspec.open` or member of :func:`fsspec.open_files`'s returned list will be passed to the argument.
+        arg2(bytes | str | SupportsRead[bytes | str]):
+            What returned by :func:`fsspec.open`, or member of :func:`fsspec.open_files`'s returned list, will be set to the argument.
+
+            The parameter may later be used in :func:`yaml.load`, it could be:
 
-            Type of the parameter is usually one of:
+            * :class:`bytes` or :class:`str`
 
-            * Subclass of :class:`io.IOBase`
-            * Subclass of :class:`fsspec.spec.AbstractBufferedFile`
+            * An object implements ::
+
+                class SupportsRead(bytes | str):
+                    def read(self, length: int = ..., /) -> bytes | str: ...
 
             Tip:
-                **The type is NOT certain** however, because ``open`` methods of different :mod:`fsspec` file-system implementations are variable.
+                The ``open`` method of :mod:`fsspec` file-system implementations usually returns a :class:`fsspec.spec.AbstractBufferedFile` object.
+                However, **the type is NOT certain**, because ``open`` methods of different :mod:`fsspec` file-system implementations are variable.
 
         arg3(typing.Type):
-            Type of `PyYAML`'s Loader class in use.
+            Type (**not instance**) of `PyYAML`'s Loader currently in use.
 
     Returns:
         typing.Any: Parsed result
     """
 
     @contextmanager
-    def managed_autoload(self, autoload: bool) -> Generator[Self, Any, None]:
+    def managed_autoload(self, autoload: bool) -> Generator[Self, None, None]:
         """``with`` statement context manager for :attr:`autoload`
 
         Args:
             autoload: Temporary value of :attr:`autoload` to be set inside the ``with`` statement
         """
         saved, self.autoload = self.autoload, bool(autoload)
         try:
             yield self
         finally:
             self.autoload = saved
 
-    def __call__(self, loader, node):
-        if isinstance(node, yaml.ScalarNode):
-            params = loader.construct_scalar(node)
-            data = Data(params)
-        elif isinstance(node, yaml.SequenceNode):
-            params = loader.construct_sequence(node)
-            data = Data(params[0], sequence_params=params[1:])
-        elif isinstance(node, yaml.MappingNode):
-            params = loader.construct_mapping(node)
-            data = Data(
-                params["urlpath"],
-                mapping_params={k: v for k, v in params.items() if k != "urlpath"},
-            )
+    def __call__(self, loader: Union[_Loader, _CLoader], node: Node) -> Union[Data, Any]:
+        val: Union[_Scalar, Sequence, Mapping]
+        if is_yaml_scalar_node(node):
+            val = loader.construct_scalar(node)
+            if isinstance(val, str):
+                data = Data(val)
+            else:  # pragma: no cover
+                raise TypeError(f"{type(val)}")
+        elif is_yaml_sequence_node(node):
+            val = loader.construct_sequence(node)
+            data = Data(val[0], sequence_params=val[1:])
+        elif is_yaml_mapping_node(node):
+            val = loader.construct_mapping(node)
+            if is_mapping_all_key_str(val):
+                data = Data(val["urlpath"], mapping_params={k: v for k, v in val.items() if k != "urlpath"})
+            else:  # pragma: no cover
+                raise ValueError("not all key of the YAML mapping node is `str`")
         else:  # pragma: no cover
-            raise ValueError(f"PyYAML node {node!r} is not supported by {type(self)}")
+            raise TypeError(f"{type(node)}")
         if self.autoload:
             return self.load(type(loader), data)
         else:
             return data
 
-    def load(self, loader_type: TYamlLoaderTypes, data: Data) -> Any:
+    def load(self, loader_type: Type[Union[_Loader, _CLoader]], data: Data) -> Any:
         """The method will be invoked once the PyYAML's Loader class call the constructor.
         It happens when an include state tag(eg: ``"!inc"``) is met.
 
         Args:
             loader_type: Type of current in-use PyYAML Loader class
             data: The data class of the include statement
 
         Returns:
             Data from the actual included YAML file, which is parsed by a PyYAML's Loader class.
 
-        Danger:
+        Caution:
             It's mainly invoked in :func:`yaml.load`, and **NOT advised to call it yourself**.
 
         Note:
             Additional positional or named parameters in YAML include statement are passed to ``*args`` and ``**kwargs`` in :attr:`.Data.sequence_params` and :attr:`.Data.mapping_params`.
             The class will pass them to :mod:`fsspec`'s :mod:`fsspec` File-system as implementation specific options.
 
-            Note:
-                To use positional in YAML include statement is discouraged.
-
-            * If there is a protocol/scheme, and no wildcard defined in YAML including,
-              ``*args`` and ``**kwargs`` will be passed to :func:`fsspec.open`.
-
-              Example:
+        Note:
+            To use positional in YAML include statement is discouraged.
 
-                  The YAML
+        The function works as blow description:
 
-                  .. code:: yaml
+        * If there is a protocol/scheme, and no wildcard defined in YAML including,
+          ``*args`` and ``**kwargs`` will be passed to :func:`fsspec.open`.
 
-                      key: !inc {urlpath: s3://my-bucket/my-file.yml.gz, compression: gzip}
+            Example:
+                The YAML
 
-                  means::
+                .. code-block:: yaml
 
-                      with fsspec.open("s3://my-bucket/my-file.yml.gz", compression="gzip") as f:
-                          yaml.load(f, Loader)
+                    key: !inc {urlpath: s3://my-bucket/my-file.yml.gz, compression: gzip}
 
+                means::
 
-            * If there is a protocol/scheme, and also wildcard defined in YAML including,
-              :attr:`.Data.sequence_params` and :attr:`.Data.mapping_params` of ``data`` will be passed to :func:`fsspec.open_files` as ``*args`` and ``**kwargs``
+                    with fsspec.open("s3://my-bucket/my-file.yml.gz", compression="gzip") as f:
+                        yaml.load(f, Loader)
 
-              Example:
+        * If there is a protocol/scheme, and also wildcard defined in YAML including,
+          :attr:`.Data.sequence_params` and :attr:`.Data.mapping_params` of ``data`` will be passed to :func:`fsspec.open_files` as it's ``*args`` and ``**kwargs`` arguments.
 
+            Example:
                 The YAML
 
-                .. code:: yaml
+                .. code-block:: yaml
 
                     key: !inc {urlpath: s3://my-bucket/*.yml.gz, compression: gzip}
 
                 means::
 
                     with fsspec.open_files("s3://my-bucket/*.yml.gz", compression="gzip") as files:
                         for file in files:
                             yaml.load(file, Loader)
 
-            * If there is no protocol/scheme, and no wildcard defined in YAML including,
-              :attr:`.Data.sequence_params` and :attr:`.Data.mapping_params` of ``data`` will be passed to :mod:`fsspec` file-system implementation's ``open`` function (derive from :meth:`fsspec.spec.AbstractFileSystem.open`) as ``*args`` and ``**kwargs``
+        * If there is no protocol/scheme, and no wildcard defined in YAML including,
+          :attr:`.Data.sequence_params` and :attr:`.Data.mapping_params` of ``data`` will be passed to :mod:`fsspec` file-system implementation's ``open`` function (derive from :meth:`fsspec.spec.AbstractFileSystem.open`) as ``*args`` and ``**kwargs``
 
-            * If there is no protocol/scheme, and also wildcard defined in YAML including, the situation is complex:
-                * If the include statement is in a positional-parameter form:
-                    * If count of argument is one,
-                        it will be passed to of :meth:`fsspec.spec.AbstractFileSystem.glob`'s  ``maxdepth`` argument;
-                    * If count of argument is more than one:
-                        # First of them will be passed to :mod:`fsspec` file system implementation's ``glob`` method (derived from :meth:`fsspec.spec.AbstractFileSystem.glob`)
-                        # Second of them will be passed to :mod:`fsspec` file system implementation's ``open`` method (derived from :meth:`fsspec.spec.AbstractFileSystem.open`)
-                        # Others will be ignored
-                * If the include statement is in a named-parameter form, the class will:
-                    * Find a key named `glob`, then pass the corresponding data to :mod:`fsspec` file system implementation's ``glob`` method (derived from :meth:`fsspec.spec.AbstractFileSystem.glob`)
-                    * Find a key named `open`, then pass the corresponding data to :mod:`fsspec` file system implementation's ``open`` method (derived from :meth:`fsspec.spec.AbstractFileSystem.open`)
+        * If there is no protocol/scheme, and also wildcard defined in YAML including, the situation is complex:
+            * If the include statement is in a positional-parameter form:
+                * If count of argument is one,
+                    it will be passed to of :meth:`fsspec.spec.AbstractFileSystem.glob`'s  ``maxdepth`` argument;
+                * If count of argument is more than one:
+                    * First of them will be passed to :mod:`fsspec` file system implementation's ``glob`` method (derived from :meth:`fsspec.spec.AbstractFileSystem.glob`)
+                    * Second of them will be passed to :mod:`fsspec` file system implementation's ``open`` method (derived from :meth:`fsspec.spec.AbstractFileSystem.open`)
+                    * Others will be ignored
+            * If the include statement is in a named-parameter form, the class will:
+                * Find a key named `glob`, then pass the corresponding data to :mod:`fsspec` file system implementation's ``glob`` method (derived from :meth:`fsspec.spec.AbstractFileSystem.glob`)
+                * Find a key named `open`, then pass the corresponding data to :mod:`fsspec` file system implementation's ``open`` method (derived from :meth:`fsspec.spec.AbstractFileSystem.open`)
 
-                Example:
-
-                    * The YAML
+            Example:
+                The YAML
 
-                        .. code:: yaml
+                .. code-block:: yaml
 
-                            key: !inc [foo/**/*.yml, 2]
+                    key: !inc [foo/**/*.yml, 2]
 
-                        means::
+                means::
 
-                            for file in fs.glob("foo/**/*.yml", maxdepth=2):
-                                with fs.open(file) as fp:
-                                    yaml.load(fp, Loader)
+                    for file in fs.glob("foo/**/*.yml", maxdepth=2):
+                        with fs.open(file) as fp:
+                            yaml.load(fp, Loader)
 
-                    * The YAML
+            Example:
+                The YAML
 
-                        .. code:: yaml
+                .. code-block:: yaml
 
-                            key: !inc {urlpath: foo/**/*.yml.gz, glob: {maxdepth: 2}, open: {compression: gzip}}
+                    key: !inc {urlpath: foo/**/*.yml.gz, glob: {maxdepth: 2}, open: {compression: gzip}}
 
-                        means::
+                means::
 
-                            for file in fs.glob("foo/**/*.yml.gz", maxdepth=2):
-                                with fs.open(file, compression=gzip) as fp:
-                                    yaml.load(fp, Loader)
+                    for file in fs.glob("foo/**/*.yml.gz", maxdepth=2):
+                        with fs.open(file, compression=gzip) as fp:
+                            yaml.load(fp, Loader)
         """
         base_dir = self.base_dir
         urlpath = data.urlpath
 
         url_sr = urlsplit(urlpath)
         if base_dir is not None:
             if callable(base_dir):
                 base_dir = Path(base_dir())
             else:
                 base_dir = Path(base_dir)
             if url_sr.scheme:
-                urlpath = urlunsplit(
-                    chain(
-                        url_sr[:2],
-                        (base_dir.joinpath(url_sr[2]).as_posix(),),
-                        url_sr[3:],
-                    )
-                )
+                urlpath = urlunsplit(chain(url_sr[:2], (base_dir.joinpath(url_sr[2]).as_posix(),), url_sr[3:]))
             else:
                 urlpath = base_dir.joinpath(urlpath).as_posix()
 
         # If protocol/scheme in path, we shall open it directly with fs's default open method
         if url_sr.scheme:
             if WILDCARDS_PATTERN.match(urlpath):
                 # if wildcards in path, return a Sequence/List
@@ -322,64 +334,85 @@
                 with fsspec.open_files(urlpath, *data.sequence_params, **data.mapping_params) as ofs:
                     for of_ in ofs:
                         data = load_open_file(of_, loader_type, urlpath, self.custom_loader)
                         result.append(data)
                 return result
             # else if no wildcard, returns a single object
             with fsspec.open(urlpath, *data.sequence_params, **data.mapping_params) as of_:
-                assert not isinstance(of_, list)
+                if isinstance(of_, list):  # pragma: no cover
+                    raise RuntimeError(f"`fsspec.open()` returns a `list` ({of_})")
                 result = load_open_file(of_, loader_type, urlpath, self.custom_loader)
                 return result
 
         # if no protocol / scheme in path, we shall use the `fs` object
         if WILDCARDS_PATTERN.match(urlpath):
             urlpath = Path(urlpath).as_posix()
             # if wildcard in path, returns a List
-            glob_params = open_params = None
+            glob_params: Union[Mapping[str, Any], Iterable, None] = None
+            open_params: Union[Mapping[str, Any], Iterable, None] = None
             if data.sequence_params:
                 if len(data.sequence_params) > 1:
                     glob_params, open_params = data.sequence_params[:2]
                 elif len(data.sequence_params) == 1:
                     glob_params = data.sequence_params[0]
-            if data.mapping_params:
+            elif data.mapping_params:
                 glob_params = data.mapping_params.get("glob")
                 open_params = data.mapping_params.get("open")
 
             if glob_params is None:
                 glob_fn = lambda: self.fs.glob(urlpath)  # noqa: E731
-            elif isinstance(glob_params, dict):
+            elif isinstance(glob_params, Mapping):
                 # special for maxdepth, because PyYAML sometimes treat number as string for constructor's parameter
-                if "maxdepth" in glob_params:
-                    glob_params["maxdepth"] = int(glob_params["maxdepth"])
-                glob_fn = lambda: self.fs.glob(urlpath, **glob_params)  # noqa: E731
-            elif isinstance(glob_params, (list, set)):
+                kv_args = {**glob_params}
+                if "maxdepth" in kv_args:
+                    kv_args["maxdepth"] = int(kv_args["maxdepth"])
+                glob_fn = lambda: self.fs.glob(urlpath, **kv_args)  # noqa: E731
+            elif isinstance(glob_params, Iterable) and not isinstance(glob_params, (str, bytes)):
                 # special for maxdepth, because PyYAML sometimes treat number as string for constructor's parameter
-                glob_params = list(glob_params)
-                if glob_params:
-                    glob_params[0] = int(glob_params[0])
-                glob_fn = lambda: self.fs.glob(urlpath, *glob_params)  # noqa: E731
+                pos_args = list(glob_params)
+                if pos_args:
+                    pos_args[0] = int(pos_args[0])
+                glob_fn = lambda: self.fs.glob(urlpath, *pos_args)  # noqa: E731
             else:
                 # special for maxdepth, because PyYAML sometimes treat number as string for constructor's parameter
                 maxdepth = int(glob_params)
-                glob_fn = lambda: self.fs.glob(urlpath, maxdepth)  # noqa: E731
+                glob_fn = lambda: self.fs.glob(urlpath, maxdepth=maxdepth)  # noqa: E731
 
             if open_params is None:
                 open_fn = lambda x: self.fs.open(x)  # noqa: E731
-            elif isinstance(open_params, dict):
+            elif isinstance(open_params, Mapping):
                 open_fn = lambda x: self.fs.open(x, **open_params)  # noqa: E731
-            elif isinstance(open_params, (list, set)):
+            elif isinstance(open_params, Iterable) and not isinstance(open_params, (str, bytes)):
                 open_fn = lambda x: self.fs.open(x, *open_params)  # noqa: E731
-            else:
-                open_fn = lambda x: self.fs.open(x, open_params)  # noqa: E731
+            elif isinstance(open_params, str):
+                mode = str(open_params)
+                open_fn = lambda x: self.fs.open(x, mode=mode)  # noqa: E731
 
             result = []
             for file in glob_fn():
-                assert isinstance(file, str)
+                if not isinstance(file, str):  # pragma: no cover
+                    raise RuntimeError(f"`fs.glob()` function does not return a `str` ({file})")
                 with open_fn(file) as of_:
                     data = load_open_file(of_, loader_type, file, self.custom_loader)
                     result.append(data)
             return result
 
         # else if no wildcards, return a single object
         with self.fs.open(urlpath, *data.sequence_params, **data.mapping_params) as of_:
             result = load_open_file(of_, loader_type, urlpath, self.custom_loader)
             return result
+
+
+def is_yaml_scalar_node(node) -> TypeGuard[yaml.ScalarNode]:
+    return isinstance(node, yaml.ScalarNode)
+
+
+def is_yaml_sequence_node(node) -> TypeGuard[yaml.SequenceNode]:
+    return isinstance(node, yaml.SequenceNode)
+
+
+def is_yaml_mapping_node(node) -> TypeGuard[yaml.MappingNode]:
+    return isinstance(node, yaml.MappingNode)
+
+
+def is_mapping_all_key_str(val) -> TypeGuard[Mapping[str, Any]]:
+    return all(isinstance(k, str) for k in val)
```

### Comparing `pyyaml-include-2.0b2/src/yaml_include/data.py` & `pyyaml_include-2.1/src/yaml_include/data.py`

 * *Files identical despite different names*

### Comparing `pyyaml-include-2.0b2/src/yaml_include/funcs.py` & `pyyaml_include-2.1/src/yaml_include/funcs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,81 +1,78 @@
-import sys
-from typing import Any, Generator, Mapping, MutableMapping, MutableSequence, Sequence
+from __future__ import annotations
 
-if sys.version_info < (3, 12):  # pragma: no cover
-    from .yaml_types_backward import TYamlLoaderTypes
-else:  # pragma: no cover
-    from .yaml_types import TYamlLoaderTypes
+from typing import TYPE_CHECKING, Any, Generator, Mapping, MutableMapping, MutableSequence, Sequence, Type, Union
 
 from .constructor import Constructor
 from .data import Data
 
+if TYPE_CHECKING:  # pragma: no cover
+    from yaml.cyaml import _CLoader
+    from yaml.loader import _Loader
+
 
 __all__ = ["load", "lazy_load"]
 
 
 def load(
     obj: Any,
-    loader_type: TYamlLoaderTypes,
+    loader_type: Type[Union[_Loader, _CLoader]],
     constructor: Constructor,
     inplace: bool = False,
     nested: bool = False,
 ) -> Any:
     """Recursively load and parse all :class:`.Data` instances inside ``obj``.
 
     If :attr:`.Constructor.autoload` is ``False``, :func:`yaml.load` will not cause including files to be opened or read,
     in the situation, what returned by :func:`yaml.load` is an object with :class:`.Data` in it, and the files won't be processed.
     Thus we use the function to open and parse those including files represented by :class:`.Data` instances inside `obj`.
 
     Args:
         obj: object containers :class:`.Data`
         loader_type: use this type of `PyYAML` Loader to parse string in including file(s)
         constructor: use this :class:`.Constructor` to find/open/read including file(s)
-        inplace: whether if make a in-place replacement for :class:`.Constructor` tags of including file(s) into ``obj`` argument
-        nested: whether if parse and load include statement(s) inside including file(s)
+        inplace: whether to make a in-place replacement for every :class:`.Constructor` instance in ``obj``
+        nested: whether to parse and load lower level include statement(s) inside :class:`.Constructor` instance
 
-    Return:
+    Returns:
         Parsed object
     """
     if isinstance(obj, Data):
         d = constructor.load(loader_type, obj)
         if nested:
             return load(d, loader_type, constructor, inplace, nested)
         else:
             return d
     elif isinstance(obj, Mapping):
         if inplace:
-            if not isinstance(obj, MutableMapping):
+            if not isinstance(obj, MutableMapping):  # pragma: no cover
                 raise ValueError(f"{obj} is not mutable")
             for k, v in obj.items():
                 obj[k] = load(v, loader_type, constructor, inplace, nested)
         else:
             return {k: load(v, loader_type, constructor, inplace, nested) for k, v in obj.items()}
     elif isinstance(obj, Sequence) and not isinstance(obj, (bytearray, bytes, memoryview, str)):
         if inplace:
-            if not isinstance(obj, MutableSequence):
+            if not isinstance(obj, MutableSequence):  # pragma: no cover
                 raise ValueError(f"{obj} is not mutable")
             for i, v in enumerate(obj):
                 obj[i] = load(v, loader_type, constructor, inplace, nested)
         else:
             return [load(m, loader_type, constructor, inplace, nested) for m in obj]
     return obj
 
 
 def lazy_load(
-    obj: Any,
-    loader_type: TYamlLoaderTypes,
-    constructor: Constructor,
-    nested: bool = False,
-) -> Generator:
+    obj: Any, loader_type: Type[Union[_Loader, _CLoader]], constructor: Constructor, nested: bool = False
+) -> Generator[Any, None, Any]:
     """Recursively load and parse all :class:`.Data` inside ``obj`` in generative mode.
 
     Almost the same as :func:`.load`, except that:
 
-    * The function returns a generator, it yield at every :class:`.Data` object found.
+    * The function returns a :term:`generator`, it yields at every :class:`.Data` instance found in side ``obj``.
     * It only applies an in-place parsing and replacement, and will not return parsed object.
     """
     if isinstance(obj, Data):
         d = constructor.load(loader_type, obj)
         if nested:
             return (yield from lazy_load(d, loader_type, constructor, nested))
         else:
```

### Comparing `pyyaml-include-2.0b2/src/yaml_include/representer.py` & `pyyaml_include-2.1/src/yaml_include/representer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,17 @@
+from __future__ import annotations
+
 from dataclasses import dataclass
+from itertools import chain
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:  # pragma: no cover
+    from yaml import Dumper, Node
 
-from .data import Data  # noqa: F401
+from .data import Data
 
 __all__ = ["Representer"]
 
 
 @dataclass
 class Representer:
     """Representer for :class:`.Data`
@@ -24,17 +31,16 @@
 
     Attention:
         Custom YAML tag's name starts with ``"!"``.
         But we **MUST NOT** put a ``"!"`` at the beginning here,
         because :func:`yaml.add_representer` will add the symbol itself.
     """
 
-    def __call__(self, dumper, data):
+    def __call__(self, dumper: Dumper, data) -> Node:
+        if not isinstance(data, Data):  # pragma: no cover
+            raise TypeError(f"{type(data)}")
+        tag = "!" + self.tag
         if data.mapping_params:
-            params = {"urlpath": data.urlpath}
-            params.update(data.mapping_params)
-            return dumper.represent_mapping(f"!{self.tag}", params)
+            return dumper.represent_mapping(tag, {**{"urlpath": data.urlpath}, **data.mapping_params})
         if data.sequence_params:
-            params = [data.urlpath]
-            params.extend(data.sequence_params)
-            return dumper.represent_sequence(f"!{self.tag}", params)
-        return dumper.represent_scalar(f"!{self.tag}", data.urlpath)
+            return dumper.represent_sequence(tag, chain((data.urlpath,), data.sequence_params))
+        return dumper.represent_scalar(tag, data.urlpath)
```

