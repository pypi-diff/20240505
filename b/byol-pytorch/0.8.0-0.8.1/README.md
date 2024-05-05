# Comparing `tmp/byol-pytorch-0.8.0.tar.gz` & `tmp/byol_pytorch-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byol-pytorch-0.8.0.tar", last modified: Thu Nov 16 19:20:53 2023, max compression
+gzip compressed data, was "byol_pytorch-0.8.1.tar", last modified: Sun May  5 17:28:49 2024, max compression
```

## Comparing `byol-pytorch-0.8.0.tar` & `byol_pytorch-0.8.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 19:20:53.234938 byol-pytorch-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-11-16 19:20:43.000000 byol-pytorch-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      722 2023-11-16 19:20:53.234938 byol-pytorch-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7564 2023-11-16 19:20:43.000000 byol-pytorch-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 19:20:53.234938 byol-pytorch-0.8.0/byol_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-11-16 19:20:43.000000 byol-pytorch-0.8.0/byol_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9190 2023-11-16 19:20:43.000000 byol-pytorch-0.8.0/byol_pytorch/byol_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2023-11-16 19:20:43.000000 byol-pytorch-0.8.0/byol_pytorch/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 19:20:53.234938 byol-pytorch-0.8.0/byol_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      722 2023-11-16 19:20:53.000000 byol-pytorch-0.8.0/byol_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      283 2023-11-16 19:20:53.000000 byol-pytorch-0.8.0/byol_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-16 19:20:53.000000 byol-pytorch-0.8.0/byol_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-11-16 19:20:53.000000 byol-pytorch-0.8.0/byol_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-11-16 19:20:53.000000 byol-pytorch-0.8.0/byol_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-16 19:20:53.234938 byol-pytorch-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      865 2023-11-16 19:20:43.000000 byol-pytorch-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:28:49.262894 byol_pytorch-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-05 17:28:45.000000 byol_pytorch-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-05 17:28:49.262894 byol_pytorch-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7564 2024-05-05 17:28:45.000000 byol_pytorch-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:28:49.258893 byol_pytorch-0.8.1/byol_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-05 17:28:45.000000 byol_pytorch-0.8.1/byol_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9190 2024-05-05 17:28:45.000000 byol_pytorch-0.8.1/byol_pytorch/byol_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-05 17:28:45.000000 byol_pytorch-0.8.1/byol_pytorch/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:28:49.262894 byol_pytorch-0.8.1/byol_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-05 17:28:49.000000 byol_pytorch-0.8.1/byol_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-05 17:28:49.000000 byol_pytorch-0.8.1/byol_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 17:28:49.000000 byol_pytorch-0.8.1/byol_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-05 17:28:49.000000 byol_pytorch-0.8.1/byol_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-05 17:28:49.000000 byol_pytorch-0.8.1/byol_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 17:28:49.262894 byol_pytorch-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-05 17:28:45.000000 byol_pytorch-0.8.1/setup.py
```

### Comparing `byol-pytorch-0.8.0/LICENSE` & `byol_pytorch-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `byol-pytorch-0.8.0/PKG-INFO` & `byol_pytorch-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byol-pytorch
-Version: 0.8.0
+Version: 0.8.1
 Summary: Self-supervised contrastive learning made simple
 Home-page: https://github.com/lucidrains/byol-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: self-supervised learning,artificial intelligence
 Classifier: Development Status :: 4 - Beta
```

### Comparing `byol-pytorch-0.8.0/README.md` & `byol_pytorch-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `byol-pytorch-0.8.0/byol_pytorch/byol_pytorch.py` & `byol_pytorch-0.8.1/byol_pytorch/byol_pytorch.py`

 * *Files identical despite different names*

### Comparing `byol-pytorch-0.8.0/byol_pytorch/trainer.py` & `byol_pytorch-0.8.1/byol_pytorch/trainer.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,21 @@
 
 from byol_pytorch.byol_pytorch import BYOL
 
 from beartype import beartype
 from beartype.typing import Optional
 
 from accelerate import Accelerator
+from accelerate.utils import DistributedDataParallelKwargs
+
+# constants
+
+DEFAULT_DDP_KWARGS = DistributedDataParallelKwargs(
+    find_unused_parameters = True
+)
 
 # functions
 
 def exists(v):
     return v is not None
 
 def cycle(dl):
@@ -56,14 +63,18 @@
         checkpoint_every: int = 1000,
         checkpoint_folder: str = './checkpoints',
         byol_kwargs: dict = dict(),
         optimizer_kwargs: dict = dict(),
         accelerator_kwargs: dict = dict(),
     ):
         super().__init__()
+
+        if 'kwargs_handlers' not in accelerator_kwargs:
+            accelerator_kwargs['kwargs_handlers'] = [DEFAULT_DDP_KWARGS]
+
         self.accelerator = Accelerator(**accelerator_kwargs)
 
         if dist.is_initialized() and dist.get_world_size() > 1:
             net = SyncBatchNorm.convert_sync_batchnorm(net)
 
         self.net = net
```

### Comparing `byol-pytorch-0.8.0/byol_pytorch.egg-info/PKG-INFO` & `byol_pytorch-0.8.1/byol_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byol-pytorch
-Version: 0.8.0
+Version: 0.8.1
 Summary: Self-supervised contrastive learning made simple
 Home-page: https://github.com/lucidrains/byol-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: self-supervised learning,artificial intelligence
 Classifier: Development Status :: 4 - Beta
```

### Comparing `byol-pytorch-0.8.0/setup.py` & `byol_pytorch-0.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'byol-pytorch',
   packages = find_packages(exclude=['examples']),
-  version = '0.8.0',
+  version = '0.8.1',
   license='MIT',
   description = 'Self-supervised contrastive learning made simple',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/byol-pytorch',
   long_description_content_type = 'text/markdown',
   keywords = [
```

