# Comparing `tmp/gammarers.aws-secure-bucket-1.3.3.tar.gz` & `tmp/gammarers.aws-secure-bucket-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarers.aws-secure-bucket-1.3.3.tar", last modified: Sun Apr 28 17:14:20 2024, max compression
+gzip compressed data, was "gammarers.aws-secure-bucket-1.3.4.tar", last modified: Sun May  5 17:13:53 2024, max compression
```

## Comparing `gammarers.aws-secure-bucket-1.3.3.tar` & `gammarers.aws-secure-bucket-1.3.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:14:20.466430 gammarers.aws-secure-bucket-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-28 17:14:10.000000 gammarers.aws-secure-bucket-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-28 17:14:10.000000 gammarers.aws-secure-bucket-1.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-28 17:14:20.466430 gammarers.aws-secure-bucket-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-28 17:14:10.000000 gammarers.aws-secure-bucket-1.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-28 17:14:10.000000 gammarers.aws-secure-bucket-1.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 17:14:20.466430 gammarers.aws-secure-bucket-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-28 17:14:10.000000 gammarers.aws-secure-bucket-1.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:14:20.466430 gammarers.aws-secure-bucket-1.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:14:20.466430 gammarers.aws-secure-bucket-1.3.3/src/gammarers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:14:20.466430 gammarers.aws-secure-bucket-1.3.3/src/gammarers/aws_secure_bucket/
--rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-04-28 17:14:10.000000 gammarers.aws-secure-bucket-1.3.3/src/gammarers/aws_secure_bucket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:14:20.466430 gammarers.aws-secure-bucket-1.3.3/src/gammarers/aws_secure_bucket/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-28 17:14:10.000000 gammarers.aws-secure-bucket-1.3.3/src/gammarers/aws_secure_bucket/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33307 2024-04-28 17:14:10.000000 gammarers.aws-secure-bucket-1.3.3/src/gammarers/aws_secure_bucket/_jsii/aws-secure-bucket@1.3.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 17:14:10.000000 gammarers.aws-secure-bucket-1.3.3/src/gammarers/aws_secure_bucket/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:14:20.466430 gammarers.aws-secure-bucket-1.3.3/src/gammarers.aws_secure_bucket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-28 17:14:20.000000 gammarers.aws-secure-bucket-1.3.3/src/gammarers.aws_secure_bucket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-28 17:14:20.000000 gammarers.aws-secure-bucket-1.3.3/src/gammarers.aws_secure_bucket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 17:14:20.000000 gammarers.aws-secure-bucket-1.3.3/src/gammarers.aws_secure_bucket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-28 17:14:20.000000 gammarers.aws-secure-bucket-1.3.3/src/gammarers.aws_secure_bucket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-28 17:14:20.000000 gammarers.aws-secure-bucket-1.3.3/src/gammarers.aws_secure_bucket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:13:53.027154 gammarers.aws-secure-bucket-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-05 17:13:37.000000 gammarers.aws-secure-bucket-1.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-05 17:13:37.000000 gammarers.aws-secure-bucket-1.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-05 17:13:53.027154 gammarers.aws-secure-bucket-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-05 17:13:37.000000 gammarers.aws-secure-bucket-1.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-05 17:13:37.000000 gammarers.aws-secure-bucket-1.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 17:13:53.027154 gammarers.aws-secure-bucket-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-05 17:13:37.000000 gammarers.aws-secure-bucket-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:13:53.023154 gammarers.aws-secure-bucket-1.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:13:53.023154 gammarers.aws-secure-bucket-1.3.4/src/gammarers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:13:53.027154 gammarers.aws-secure-bucket-1.3.4/src/gammarers/aws_secure_bucket/
+-rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-05-05 17:13:37.000000 gammarers.aws-secure-bucket-1.3.4/src/gammarers/aws_secure_bucket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:13:53.027154 gammarers.aws-secure-bucket-1.3.4/src/gammarers/aws_secure_bucket/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-05 17:13:37.000000 gammarers.aws-secure-bucket-1.3.4/src/gammarers/aws_secure_bucket/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33305 2024-05-05 17:13:37.000000 gammarers.aws-secure-bucket-1.3.4/src/gammarers/aws_secure_bucket/_jsii/aws-secure-bucket@1.3.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 17:13:37.000000 gammarers.aws-secure-bucket-1.3.4/src/gammarers/aws_secure_bucket/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:13:53.023154 gammarers.aws-secure-bucket-1.3.4/src/gammarers.aws_secure_bucket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-05 17:13:52.000000 gammarers.aws-secure-bucket-1.3.4/src/gammarers.aws_secure_bucket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-05 17:13:52.000000 gammarers.aws-secure-bucket-1.3.4/src/gammarers.aws_secure_bucket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 17:13:52.000000 gammarers.aws-secure-bucket-1.3.4/src/gammarers.aws_secure_bucket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-05 17:13:52.000000 gammarers.aws-secure-bucket-1.3.4/src/gammarers.aws_secure_bucket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-05 17:13:52.000000 gammarers.aws-secure-bucket-1.3.4/src/gammarers.aws_secure_bucket.egg-info/top_level.txt
```

### Comparing `gammarers.aws-secure-bucket-1.3.3/LICENSE` & `gammarers.aws-secure-bucket-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarers.aws-secure-bucket-1.3.3/PKG-INFO` & `gammarers.aws-secure-bucket-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarers.aws-secure-bucket
-Version: 1.3.3
+Version: 1.3.4
 Summary: This is a Simple S3 Secure Bucket.
 Home-page: https://github.com/gammarers/aws-secure-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarers/aws-secure-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarers.aws-secure-bucket-1.3.3/README.md` & `gammarers.aws-secure-bucket-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `gammarers.aws-secure-bucket-1.3.3/setup.py` & `gammarers.aws-secure-bucket-1.3.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarers.aws-secure-bucket",
-    "version": "1.3.3",
+    "version": "1.3.4",
     "description": "This is a Simple S3 Secure Bucket.",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarers/aws-secure-bucket.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "gammarers.aws_secure_bucket",
         "gammarers.aws_secure_bucket._jsii"
     ],
     "package_data": {
         "gammarers.aws_secure_bucket._jsii": [
-            "aws-secure-bucket@1.3.3.jsii.tgz"
+            "aws-secure-bucket@1.3.4.jsii.tgz"
         ],
         "gammarers.aws_secure_bucket": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.80.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.97.0, <2.0.0",
+        "jsii>=1.98.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `gammarers.aws-secure-bucket-1.3.3/src/gammarers/aws_secure_bucket/__init__.py` & `gammarers.aws-secure-bucket-1.3.4/src/gammarers/aws_secure_bucket/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarers.aws-secure-bucket-1.3.3/src/gammarers.aws_secure_bucket.egg-info/PKG-INFO` & `gammarers.aws-secure-bucket-1.3.4/src/gammarers.aws_secure_bucket.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarers.aws-secure-bucket
-Version: 1.3.3
+Version: 1.3.4
 Summary: This is a Simple S3 Secure Bucket.
 Home-page: https://github.com/gammarers/aws-secure-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarers/aws-secure-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarers.aws-secure-bucket-1.3.3/src/gammarers.aws_secure_bucket.egg-info/SOURCES.txt` & `gammarers.aws-secure-bucket-1.3.4/src/gammarers.aws_secure_bucket.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarers.aws_secure_bucket.egg-info/SOURCES.txt
 src/gammarers.aws_secure_bucket.egg-info/dependency_links.txt
 src/gammarers.aws_secure_bucket.egg-info/requires.txt
 src/gammarers.aws_secure_bucket.egg-info/top_level.txt
 src/gammarers/aws_secure_bucket/__init__.py
 src/gammarers/aws_secure_bucket/py.typed
 src/gammarers/aws_secure_bucket/_jsii/__init__.py
-src/gammarers/aws_secure_bucket/_jsii/aws-secure-bucket@1.3.3.jsii.tgz
+src/gammarers/aws_secure_bucket/_jsii/aws-secure-bucket@1.3.4.jsii.tgz
```
