# Comparing `tmp/ramp_packer-2.5.7.tar.gz` & `tmp/ramp_packer-2.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ramp_packer-2.5.7.tar", max compression
+gzip compressed data, was "ramp_packer-2.5.8.tar", max compression
```

## Comparing `ramp_packer-2.5.7.tar` & `ramp_packer-2.5.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1310 2023-10-06 08:36:38.430001 ramp_packer-2.5.7/LICENSE
--rw-r--r--   0        0        0        0 2023-10-06 08:36:38.430001 ramp_packer-2.5.7/RAMP/__init__.py
--rw-r--r--   0        0        0     4138 2023-10-06 08:36:38.434001 ramp_packer-2.5.7/RAMP/commands_discovery.py
--rw-r--r--   0        0        0      920 2023-10-06 08:36:38.434001 ramp_packer-2.5.7/RAMP/common.py
--rw-r--r--   0        0        0      310 2023-10-06 08:36:38.434001 ramp_packer-2.5.7/RAMP/config.py
--rw-r--r--   0        0        0     3196 2023-10-06 08:36:38.434001 ramp_packer-2.5.7/RAMP/disposableredis/__init__.py
--rw-r--r--   0        0        0     3708 2023-10-06 08:36:38.434001 ramp_packer-2.5.7/RAMP/module_metadata.py
--rw-r--r--   0        0        0     7156 2023-10-06 08:36:38.434001 ramp_packer-2.5.7/RAMP/packer.py
--rwxr-xr-x   0        0        0     4974 2023-10-06 08:36:38.434001 ramp_packer-2.5.7/RAMP/ramp.py
--rw-r--r--   0        0        0     6829 2023-10-06 08:36:38.434001 ramp_packer-2.5.7/RAMP/unpacker.py
--rw-r--r--   0        0        0      127 2023-10-06 08:36:38.434001 ramp_packer-2.5.7/RAMP/version.py
--rw-r--r--   0        0        0     4962 2023-10-06 08:36:38.434001 ramp_packer-2.5.7/README.md
--rw-r--r--   0        0        0     1020 2023-10-06 08:36:39.322018 ramp_packer-2.5.7/pyproject.toml
--rw-r--r--   0        0        0     5905 1970-01-01 00:00:00.000000 ramp_packer-2.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1310 2023-10-31 10:59:56.324970 ramp_packer-2.5.8/LICENSE
+-rw-r--r--   0        0        0        0 2023-10-31 10:59:56.324970 ramp_packer-2.5.8/RAMP/__init__.py
+-rw-r--r--   0        0        0     4138 2023-10-31 10:59:56.324970 ramp_packer-2.5.8/RAMP/commands_discovery.py
+-rw-r--r--   0        0        0      920 2023-10-31 10:59:56.324970 ramp_packer-2.5.8/RAMP/common.py
+-rw-r--r--   0        0        0      310 2023-10-31 10:59:56.324970 ramp_packer-2.5.8/RAMP/config.py
+-rw-r--r--   0        0        0     3196 2023-10-31 10:59:56.324970 ramp_packer-2.5.8/RAMP/disposableredis/__init__.py
+-rw-r--r--   0        0        0     3708 2023-10-31 10:59:56.324970 ramp_packer-2.5.8/RAMP/module_metadata.py
+-rw-r--r--   0        0        0     7156 2023-10-31 10:59:56.328970 ramp_packer-2.5.8/RAMP/packer.py
+-rwxr-xr-x   0        0        0     4974 2023-10-31 10:59:56.328970 ramp_packer-2.5.8/RAMP/ramp.py
+-rw-r--r--   0        0        0     6829 2023-10-31 10:59:56.328970 ramp_packer-2.5.8/RAMP/unpacker.py
+-rw-r--r--   0        0        0      127 2023-10-31 10:59:56.328970 ramp_packer-2.5.8/RAMP/version.py
+-rw-r--r--   0        0        0     4962 2023-10-31 10:59:56.328970 ramp_packer-2.5.8/README.md
+-rw-r--r--   0        0        0     1020 2023-10-31 10:59:57.249021 ramp_packer-2.5.8/pyproject.toml
+-rw-r--r--   0        0        0     5905 1970-01-01 00:00:00.000000 ramp_packer-2.5.8/PKG-INFO
```

### Comparing `ramp_packer-2.5.7/LICENSE` & `ramp_packer-2.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ramp_packer-2.5.7/RAMP/commands_discovery.py` & `ramp_packer-2.5.8/RAMP/commands_discovery.py`

 * *Files identical despite different names*

### Comparing `ramp_packer-2.5.7/RAMP/common.py` & `ramp_packer-2.5.8/RAMP/common.py`

 * *Files identical despite different names*

### Comparing `ramp_packer-2.5.7/RAMP/disposableredis/__init__.py` & `ramp_packer-2.5.8/RAMP/disposableredis/__init__.py`

 * *Files identical despite different names*

### Comparing `ramp_packer-2.5.7/RAMP/module_metadata.py` & `ramp_packer-2.5.8/RAMP/module_metadata.py`

 * *Files identical despite different names*

### Comparing `ramp_packer-2.5.7/RAMP/packer.py` & `ramp_packer-2.5.8/RAMP/packer.py`

 * *Files identical despite different names*

### Comparing `ramp_packer-2.5.7/RAMP/ramp.py` & `ramp_packer-2.5.8/RAMP/ramp.py`

 * *Files identical despite different names*

### Comparing `ramp_packer-2.5.7/RAMP/unpacker.py` & `ramp_packer-2.5.8/RAMP/unpacker.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
                                    error_code="module_name_missing")
 
     if not metadata["module_file"]:
         raise UnpackerPackageError(message=INVALID_METADATA,
                                    reason="Empty module file name",
                                    error_code="module_file_missing")
 
-    if metadata["architecture"] not in {"x86_64", "arm64v8"}:
+    if metadata["architecture"] not in {"x86_64", "aarch64"}:
         raise UnpackerPackageError(message=INVALID_METADATA,
                                    reason="Architecture must be 64 bits",
                                    error_code="module_architecture_not_supported")
 
     if not metadata["version"]:
         raise UnpackerPackageError(message=INVALID_METADATA,
                                    reason="Missing version",
```

### Comparing `ramp_packer-2.5.7/README.md` & `ramp_packer-2.5.8/README.md`

 * *Files identical despite different names*

### Comparing `ramp_packer-2.5.7/pyproject.toml` & `ramp_packer-2.5.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ramp-packer"
-version = "2.5.7"
+version = "2.5.8"
 description = "Packs for Redis modules into a distributable format"
 authors = [ "Redis OSS <oss@redis.com>" ]
 license = "BSD-2-Clause"
 readme = "README.md"
 classifiers = [
   "Topic :: Database",
   "Programming Language :: Python",
```

### Comparing `ramp_packer-2.5.7/PKG-INFO` & `ramp_packer-2.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ramp-packer
-Version: 2.5.7
+Version: 2.5.8
 Summary: Packs for Redis modules into a distributable format
 License: BSD-2-Clause
 Author: Redis OSS
 Author-email: oss@redis.com
 Requires-Python: >=3.7,<4
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

