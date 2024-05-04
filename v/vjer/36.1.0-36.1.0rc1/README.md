# Comparing `tmp/vjer-36.1.0.tar.gz` & `tmp/vjer-36.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vjer-36.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vjer-36.1.0rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vjer-36.1.0.tar` & `vjer-36.1.0rc1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     2311 2024-05-04 23:20:18.405294 vjer-36.1.0/.github/workflows/build.yml
--rw-r--r--   0        0        0     2359 2024-05-04 23:20:18.405294 vjer-36.1.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     5245 2024-05-04 23:20:18.405294 vjer-36.1.0/.gitignore
--rw-r--r--   0        0        0     4999 2024-05-04 23:20:18.405294 vjer-36.1.0/.p4ignore
--rw-r--r--   0        0        0       42 2024-05-04 23:20:18.405294 vjer-36.1.0/.readthedocs.yml
--rw-r--r--   0        0        0    41141 2024-05-04 23:20:18.405294 vjer-36.1.0/CHANGELOG.md
--rw-r--r--   0        0        0       64 2024-05-04 23:20:18.405294 vjer-36.1.0/DOCUMENTATION.md
--rw-r--r--   0        0        0     1072 2024-05-04 23:20:18.405294 vjer-36.1.0/LICENSE
--rw-r--r--   0        0        0       90 2024-05-04 23:20:18.409294 vjer-36.1.0/MANIFEST.in
--rw-r--r--   0        0        0      973 2024-05-04 23:20:18.409294 vjer-36.1.0/README.md
--rw-r--r--   0        0        0      634 2024-05-04 23:20:18.409294 vjer-36.1.0/docs/Makefile
--rw-r--r--   0        0        0     9167 2024-05-04 23:20:18.409294 vjer-36.1.0/docs/coding_standards.py
--rw-r--r--   0        0        0     2103 2024-05-04 23:20:18.409294 vjer-36.1.0/docs/conf.py
--rw-r--r--   0        0        0      795 2024-05-04 23:20:18.409294 vjer-36.1.0/docs/make.bat
--rw-r--r--   0        0        0       59 2024-05-04 23:20:18.409294 vjer-36.1.0/docs/modules.rst
--rw-r--r--   0        0        0      229 2024-05-04 23:20:18.409294 vjer-36.1.0/docs/requirements.txt
--rw-r--r--   0        0        0     2184 2024-05-04 23:20:37.617198 vjer-36.1.0/pyproject.toml
--rw-r--r--   0        0        0       90 2024-05-04 23:20:18.409294 vjer-36.1.0/tests/vjer.yml
--rw-r--r--   0        0        0      305 2024-05-04 23:20:18.409294 vjer-36.1.0/util/New-Env.ps1
--rw-r--r--   0        0        0      259 2024-05-04 23:20:18.409294 vjer-36.1.0/util/Update-Env.ps1
--rwxr-xr-x   0        0        0      293 2024-05-04 23:20:18.409294 vjer-36.1.0/util/new-env.sh
--rwxr-xr-x   0        0        0      234 2024-05-04 23:20:18.409294 vjer-36.1.0/util/update-env.sh
--rw-r--r--   0        0        0      476 2024-05-04 23:20:18.409294 vjer-36.1.0/vjer.yml
--rw-r--r--   0        0        0      654 2024-05-04 23:20:37.617198 vjer-36.1.0/vjer/__init__.py
--rw-r--r--   0        0        0      205 2024-05-04 23:20:18.409294 vjer-36.1.0/vjer/__main__.py
--rw-r--r--   0        0        0     5278 2024-05-04 23:20:18.409294 vjer-36.1.0/vjer/build.py
--rw-r--r--   0        0        0     1185 2024-05-04 23:20:18.409294 vjer-36.1.0/vjer/deploy.py
--rw-r--r--   0        0        0     2875 2024-05-04 23:20:18.409294 vjer-36.1.0/vjer/freeze.py
--rw-r--r--   0        0        0     1649 2024-05-04 23:20:18.409294 vjer-36.1.0/vjer/pre_release.py
--rw-r--r--   0        0        0        0 2024-05-04 23:20:18.409294 vjer-36.1.0/vjer/py.typed
--rw-r--r--   0        0        0     3170 2024-05-04 23:20:18.409294 vjer-36.1.0/vjer/release.py
--rw-r--r--   0        0        0      769 2024-05-04 23:20:18.409294 vjer-36.1.0/vjer/rollback.py
--rw-r--r--   0        0        0     3457 2024-05-04 23:20:18.409294 vjer-36.1.0/vjer/test.py
--rw-r--r--   0        0        0     3060 2024-05-04 23:20:18.409294 vjer-36.1.0/vjer/tool_reporter.py
--rw-r--r--   0        0        0    26644 2024-05-04 23:20:18.409294 vjer-36.1.0/vjer/utils.py
--rwxr-xr-x   0        0        0     3239 2024-05-04 23:20:18.409294 vjer-36.1.0/vjer/vjer.py
--rw-r--r--   0        0        0      880 1970-01-01 00:00:00.000000 vjer-36.1.0/setup.py
--rw-r--r--   0        0        0     1315 1970-01-01 00:00:00.000000 vjer-36.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2311 2024-05-04 22:47:19.081457 vjer-36.1.0rc1/.github/workflows/build.yml
+-rw-r--r--   0        0        0     2359 2024-05-04 22:47:19.081457 vjer-36.1.0rc1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     5245 2024-05-04 22:47:19.081457 vjer-36.1.0rc1/.gitignore
+-rw-r--r--   0        0        0     4999 2024-05-04 22:47:19.081457 vjer-36.1.0rc1/.p4ignore
+-rw-r--r--   0        0        0       42 2024-05-04 22:47:19.081457 vjer-36.1.0rc1/.readthedocs.yml
+-rw-r--r--   0        0        0    41141 2024-05-04 22:47:19.085457 vjer-36.1.0rc1/CHANGELOG.md
+-rw-r--r--   0        0        0       64 2024-05-04 22:47:19.085457 vjer-36.1.0rc1/DOCUMENTATION.md
+-rw-r--r--   0        0        0     1072 2024-05-04 22:47:19.085457 vjer-36.1.0rc1/LICENSE
+-rw-r--r--   0        0        0       90 2024-05-04 22:47:19.085457 vjer-36.1.0rc1/MANIFEST.in
+-rw-r--r--   0        0        0      973 2024-05-04 22:47:19.085457 vjer-36.1.0rc1/README.md
+-rw-r--r--   0        0        0      634 2024-05-04 22:47:19.085457 vjer-36.1.0rc1/docs/Makefile
+-rw-r--r--   0        0        0     9167 2024-05-04 22:47:19.085457 vjer-36.1.0rc1/docs/coding_standards.py
+-rw-r--r--   0        0        0     2103 2024-05-04 22:47:19.085457 vjer-36.1.0rc1/docs/conf.py
+-rw-r--r--   0        0        0      795 2024-05-04 22:47:19.085457 vjer-36.1.0rc1/docs/make.bat
+-rw-r--r--   0        0        0       59 2024-05-04 22:47:19.085457 vjer-36.1.0rc1/docs/modules.rst
+-rw-r--r--   0        0        0      229 2024-05-04 22:47:19.085457 vjer-36.1.0rc1/docs/requirements.txt
+-rw-r--r--   0        0        0     2187 2024-05-04 22:47:19.085457 vjer-36.1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0       90 2024-05-04 22:47:19.085457 vjer-36.1.0rc1/tests/vjer.yml
+-rw-r--r--   0        0        0      305 2024-05-04 22:47:19.085457 vjer-36.1.0rc1/util/New-Env.ps1
+-rw-r--r--   0        0        0      259 2024-05-04 22:47:19.085457 vjer-36.1.0rc1/util/Update-Env.ps1
+-rwxr-xr-x   0        0        0      293 2024-05-04 22:47:19.085457 vjer-36.1.0rc1/util/new-env.sh
+-rwxr-xr-x   0        0        0      234 2024-05-04 22:47:19.085457 vjer-36.1.0rc1/util/update-env.sh
+-rw-r--r--   0        0        0      476 2024-05-04 22:47:19.085457 vjer-36.1.0rc1/vjer.yml
+-rw-r--r--   0        0        0      657 2024-05-04 22:47:19.085457 vjer-36.1.0rc1/vjer/__init__.py
+-rw-r--r--   0        0        0      205 2024-05-04 22:47:19.085457 vjer-36.1.0rc1/vjer/__main__.py
+-rw-r--r--   0        0        0     5278 2024-05-04 22:47:19.085457 vjer-36.1.0rc1/vjer/build.py
+-rw-r--r--   0        0        0     1185 2024-05-04 22:47:19.085457 vjer-36.1.0rc1/vjer/deploy.py
+-rw-r--r--   0        0        0     2875 2024-05-04 22:47:19.085457 vjer-36.1.0rc1/vjer/freeze.py
+-rw-r--r--   0        0        0     1649 2024-05-04 22:47:19.085457 vjer-36.1.0rc1/vjer/pre_release.py
+-rw-r--r--   0        0        0        0 2024-05-04 22:47:19.085457 vjer-36.1.0rc1/vjer/py.typed
+-rw-r--r--   0        0        0     3170 2024-05-04 22:47:19.085457 vjer-36.1.0rc1/vjer/release.py
+-rw-r--r--   0        0        0      769 2024-05-04 22:47:19.085457 vjer-36.1.0rc1/vjer/rollback.py
+-rw-r--r--   0        0        0     3457 2024-05-04 22:47:19.085457 vjer-36.1.0rc1/vjer/test.py
+-rw-r--r--   0        0        0     3060 2024-05-04 22:47:19.085457 vjer-36.1.0rc1/vjer/tool_reporter.py
+-rw-r--r--   0        0        0    26644 2024-05-04 22:47:19.085457 vjer-36.1.0rc1/vjer/utils.py
+-rwxr-xr-x   0        0        0     3239 2024-05-04 22:47:19.085457 vjer-36.1.0rc1/vjer/vjer.py
+-rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 vjer-36.1.0rc1/setup.py
+-rw-r--r--   0        0        0     1318 1970-01-01 00:00:00.000000 vjer-36.1.0rc1/PKG-INFO
```

### Comparing `vjer-36.1.0/.github/workflows/build.yml` & `vjer-36.1.0rc1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `vjer-36.1.0/.github/workflows/publish.yml` & `vjer-36.1.0rc1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `vjer-36.1.0/.gitignore` & `vjer-36.1.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `vjer-36.1.0/.p4ignore` & `vjer-36.1.0rc1/.p4ignore`

 * *Files identical despite different names*

### Comparing `vjer-36.1.0/CHANGELOG.md` & `vjer-36.1.0rc1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `vjer-36.1.0/LICENSE` & `vjer-36.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `vjer-36.1.0/README.md` & `vjer-36.1.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `vjer-36.1.0/docs/Makefile` & `vjer-36.1.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vjer-36.1.0/docs/coding_standards.py` & `vjer-36.1.0rc1/docs/coding_standards.py`

 * *Files identical despite different names*

### Comparing `vjer-36.1.0/docs/conf.py` & `vjer-36.1.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `vjer-36.1.0/docs/make.bat` & `vjer-36.1.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `vjer-36.1.0/pyproject.toml` & `vjer-36.1.0rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = "xmlrunner.*"
 ignore_missing_imports = true
 
 [tool.bumpver]
-current_version = "v36.1.0"
+current_version = "v36.1.0rc1"
 version_pattern = "vMAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version} [skip ci]"
 commit = true
 tag = false
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `vjer-36.1.0/vjer/build.py` & `vjer-36.1.0rc1/vjer/build.py`

 * *Files identical despite different names*

### Comparing `vjer-36.1.0/vjer/deploy.py` & `vjer-36.1.0rc1/vjer/deploy.py`

 * *Files identical despite different names*

### Comparing `vjer-36.1.0/vjer/freeze.py` & `vjer-36.1.0rc1/vjer/freeze.py`

 * *Files identical despite different names*

### Comparing `vjer-36.1.0/vjer/pre_release.py` & `vjer-36.1.0rc1/vjer/pre_release.py`

 * *Files identical despite different names*

### Comparing `vjer-36.1.0/vjer/release.py` & `vjer-36.1.0rc1/vjer/release.py`

 * *Files identical despite different names*

### Comparing `vjer-36.1.0/vjer/rollback.py` & `vjer-36.1.0rc1/vjer/rollback.py`

 * *Files identical despite different names*

### Comparing `vjer-36.1.0/vjer/test.py` & `vjer-36.1.0rc1/vjer/test.py`

 * *Files identical despite different names*

### Comparing `vjer-36.1.0/vjer/tool_reporter.py` & `vjer-36.1.0rc1/vjer/tool_reporter.py`

 * *Files identical despite different names*

### Comparing `vjer-36.1.0/vjer/utils.py` & `vjer-36.1.0rc1/vjer/utils.py`

 * *Files identical despite different names*

### Comparing `vjer-36.1.0/vjer/vjer.py` & `vjer-36.1.0rc1/vjer/vjer.py`

 * *Files identical despite different names*

### Comparing `vjer-36.1.0/setup.py` & `vjer-36.1.0rc1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 extras_require = \
 {'dev': ['twine'], 'test': ['types-PyYAML', 'types-requests']}
 
 entry_points = \
 {'console_scripts': ['vjer = vjer.vjer:main']}
 
 setup(name='vjer',
-      version='36.1.0',
+      version='36.1.0rc1',
       description='Vjer CI/CD module.',
       author=None,
       author_email='"Jeffery G. Smith" <web@pobox.com>',
       url=None,
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `vjer-36.1.0/PKG-INFO` & `vjer-36.1.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vjer
-Version: 36.1.0
+Version: 36.1.0rc1
 Summary: Vjer CI/CD module.
 Keywords: python,programming,utilities
 Author-email: "Jeffery G. Smith" <web@pobox.com>
 Requires-Python: ~=3.11
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

