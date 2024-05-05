# Comparing `tmp/distrifuser-0.0.1b0.tar.gz` & `tmp/distrifuser-0.0.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "distrifuser-0.0.1b0.tar", last modified: Wed Apr 24 19:29:10 2024, max compression
+gzip compressed data, was "distrifuser-0.0.1b1.tar", last modified: Sun May  5 03:21:08 2024, max compression
```

## Comparing `distrifuser-0.0.1b0.tar` & `distrifuser-0.0.1b1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2024-04-24 19:29:10.597840 distrifuser-0.0.1b0/
--rw-r--r--   0 lmxyy      (501) staff       (20)     1068 2024-02-28 21:20:49.000000 distrifuser-0.0.1b0/LICENSE.txt
--rw-r--r--   0 lmxyy      (501) staff       (20)    10759 2024-04-24 19:29:10.597610 distrifuser-0.0.1b0/PKG-INFO
--rw-r--r--   0 lmxyy      (501) staff       (20)    10213 2024-04-24 19:18:01.000000 distrifuser-0.0.1b0/README.md
-drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2024-04-24 19:29:10.592328 distrifuser-0.0.1b0/distrifuser/
--rw-r--r--   0 lmxyy      (501) staff       (20)        0 2023-12-12 16:42:09.000000 distrifuser-0.0.1b0/distrifuser/__init__.py
--rw-r--r--   0 lmxyy      (501) staff       (20)       27 2024-04-24 18:40:16.000000 distrifuser-0.0.1b0/distrifuser/__version__.py
-drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2024-04-24 19:29:10.594329 distrifuser-0.0.1b0/distrifuser/models/
--rw-r--r--   0 lmxyy      (501) staff       (20)        0 2024-02-04 21:34:52.000000 distrifuser-0.0.1b0/distrifuser/models/__init__.py
--rw-r--r--   0 lmxyy      (501) staff       (20)     1774 2024-02-06 06:15:38.000000 distrifuser-0.0.1b0/distrifuser/models/base_model.py
--rw-r--r--   0 lmxyy      (501) staff       (20)    10944 2024-04-24 18:20:45.000000 distrifuser-0.0.1b0/distrifuser/models/distri_sdxl_unet_pp.py
--rw-r--r--   0 lmxyy      (501) staff       (20)    10171 2024-04-24 18:19:27.000000 distrifuser-0.0.1b0/distrifuser/models/distri_sdxl_unet_tp.py
--rw-r--r--   0 lmxyy      (501) staff       (20)    10866 2024-04-24 18:36:01.000000 distrifuser-0.0.1b0/distrifuser/models/naive_patch_sdxl.py
-drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2024-04-24 19:29:10.594664 distrifuser-0.0.1b0/distrifuser/modules/
--rw-r--r--   0 lmxyy      (501) staff       (20)        0 2023-12-12 18:11:45.000000 distrifuser-0.0.1b0/distrifuser/modules/__init__.py
--rw-r--r--   0 lmxyy      (501) staff       (20)      670 2024-02-06 06:15:38.000000 distrifuser-0.0.1b0/distrifuser/modules/base_module.py
-drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2024-04-24 19:29:10.595589 distrifuser-0.0.1b0/distrifuser/modules/pp/
--rw-r--r--   0 lmxyy      (501) staff       (20)        0 2024-02-06 06:15:38.000000 distrifuser-0.0.1b0/distrifuser/modules/pp/__init__.py
--rw-r--r--   0 lmxyy      (501) staff       (20)     7309 2024-02-28 17:20:17.000000 distrifuser-0.0.1b0/distrifuser/modules/pp/attn.py
--rw-r--r--   0 lmxyy      (501) staff       (20)     5242 2024-02-14 05:29:38.000000 distrifuser-0.0.1b0/distrifuser/modules/pp/conv2d.py
--rw-r--r--   0 lmxyy      (501) staff       (20)     4880 2024-04-24 19:10:39.000000 distrifuser-0.0.1b0/distrifuser/modules/pp/groupnorm.py
-drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2024-04-24 19:29:10.597208 distrifuser-0.0.1b0/distrifuser/modules/tp/
--rw-r--r--   0 lmxyy      (501) staff       (20)        0 2024-02-06 06:15:38.000000 distrifuser-0.0.1b0/distrifuser/modules/tp/__init__.py
--rw-r--r--   0 lmxyy      (501) staff       (20)     7032 2024-02-14 06:26:15.000000 distrifuser-0.0.1b0/distrifuser/modules/tp/attention.py
--rw-r--r--   0 lmxyy      (501) staff       (20)     2209 2024-02-14 06:26:15.000000 distrifuser-0.0.1b0/distrifuser/modules/tp/conv2d.py
--rw-r--r--   0 lmxyy      (501) staff       (20)     3533 2024-02-14 06:26:15.000000 distrifuser-0.0.1b0/distrifuser/modules/tp/feed_forward.py
--rw-r--r--   0 lmxyy      (501) staff       (20)     7627 2024-02-14 06:26:15.000000 distrifuser-0.0.1b0/distrifuser/modules/tp/resnet.py
--rw-r--r--   0 lmxyy      (501) staff       (20)    11405 2024-04-24 19:18:01.000000 distrifuser-0.0.1b0/distrifuser/pipelines.py
--rw-r--r--   0 lmxyy      (501) staff       (20)     7172 2024-04-24 19:07:33.000000 distrifuser-0.0.1b0/distrifuser/utils.py
-drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2024-04-24 19:29:10.593118 distrifuser-0.0.1b0/distrifuser.egg-info/
--rw-r--r--   0 lmxyy      (501) staff       (20)    10759 2024-04-24 19:29:10.000000 distrifuser-0.0.1b0/distrifuser.egg-info/PKG-INFO
--rw-r--r--   0 lmxyy      (501) staff       (20)      866 2024-04-24 19:29:10.000000 distrifuser-0.0.1b0/distrifuser.egg-info/SOURCES.txt
--rw-r--r--   0 lmxyy      (501) staff       (20)        1 2024-04-24 19:29:10.000000 distrifuser-0.0.1b0/distrifuser.egg-info/dependency_links.txt
--rw-r--r--   0 lmxyy      (501) staff       (20)       47 2024-04-24 19:29:10.000000 distrifuser-0.0.1b0/distrifuser.egg-info/requires.txt
--rw-r--r--   0 lmxyy      (501) staff       (20)       12 2024-04-24 19:29:10.000000 distrifuser-0.0.1b0/distrifuser.egg-info/top_level.txt
--rw-r--r--   0 lmxyy      (501) staff       (20)       38 2024-04-24 19:29:10.597887 distrifuser-0.0.1b0/setup.cfg
--rw-r--r--   0 lmxyy      (501) staff       (20)     1079 2024-04-24 18:09:21.000000 distrifuser-0.0.1b0/setup.py
+drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2024-05-05 03:21:08.814567 distrifuser-0.0.1b1/
+-rw-r--r--   0 lmxyy      (501) staff       (20)     1068 2024-02-28 21:20:49.000000 distrifuser-0.0.1b1/LICENSE.txt
+-rw-r--r--   0 lmxyy      (501) staff       (20)    10758 2024-05-05 03:21:08.814403 distrifuser-0.0.1b1/PKG-INFO
+-rw-r--r--   0 lmxyy      (501) staff       (20)    10212 2024-05-05 02:47:17.000000 distrifuser-0.0.1b1/README.md
+drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2024-05-05 03:21:08.808559 distrifuser-0.0.1b1/distrifuser/
+-rw-r--r--   0 lmxyy      (501) staff       (20)        0 2023-12-12 16:42:09.000000 distrifuser-0.0.1b1/distrifuser/__init__.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)       27 2024-05-05 03:19:09.000000 distrifuser-0.0.1b1/distrifuser/__version__.py
+drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2024-05-05 03:21:08.810921 distrifuser-0.0.1b1/distrifuser/models/
+-rw-r--r--   0 lmxyy      (501) staff       (20)        0 2024-02-04 21:34:52.000000 distrifuser-0.0.1b1/distrifuser/models/__init__.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)     1774 2024-02-06 06:15:38.000000 distrifuser-0.0.1b1/distrifuser/models/base_model.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)    10944 2024-05-05 02:56:33.000000 distrifuser-0.0.1b1/distrifuser/models/distri_sdxl_unet_pp.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)    10171 2024-04-24 18:19:27.000000 distrifuser-0.0.1b1/distrifuser/models/distri_sdxl_unet_tp.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)    10866 2024-04-24 18:36:01.000000 distrifuser-0.0.1b1/distrifuser/models/naive_patch_sdxl.py
+drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2024-05-05 03:21:08.811542 distrifuser-0.0.1b1/distrifuser/modules/
+-rw-r--r--   0 lmxyy      (501) staff       (20)        0 2023-12-12 18:11:45.000000 distrifuser-0.0.1b1/distrifuser/modules/__init__.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)      670 2024-02-06 06:15:38.000000 distrifuser-0.0.1b1/distrifuser/modules/base_module.py
+drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2024-05-05 03:21:08.812541 distrifuser-0.0.1b1/distrifuser/modules/pp/
+-rw-r--r--   0 lmxyy      (501) staff       (20)        0 2024-02-06 06:15:38.000000 distrifuser-0.0.1b1/distrifuser/modules/pp/__init__.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)     7309 2024-02-28 17:20:17.000000 distrifuser-0.0.1b1/distrifuser/modules/pp/attn.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)     5242 2024-02-14 05:29:38.000000 distrifuser-0.0.1b1/distrifuser/modules/pp/conv2d.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)     4880 2024-04-24 19:10:39.000000 distrifuser-0.0.1b1/distrifuser/modules/pp/groupnorm.py
+drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2024-05-05 03:21:08.814035 distrifuser-0.0.1b1/distrifuser/modules/tp/
+-rw-r--r--   0 lmxyy      (501) staff       (20)        0 2024-02-06 06:15:38.000000 distrifuser-0.0.1b1/distrifuser/modules/tp/__init__.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)     7032 2024-02-14 06:26:15.000000 distrifuser-0.0.1b1/distrifuser/modules/tp/attention.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)     2209 2024-02-14 06:26:15.000000 distrifuser-0.0.1b1/distrifuser/modules/tp/conv2d.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)     3533 2024-02-14 06:26:15.000000 distrifuser-0.0.1b1/distrifuser/modules/tp/feed_forward.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)     7627 2024-02-14 06:26:15.000000 distrifuser-0.0.1b1/distrifuser/modules/tp/resnet.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)    11837 2024-05-05 03:07:38.000000 distrifuser-0.0.1b1/distrifuser/pipelines.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)     7172 2024-04-24 19:07:33.000000 distrifuser-0.0.1b1/distrifuser/utils.py
+drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2024-05-05 03:21:08.809399 distrifuser-0.0.1b1/distrifuser.egg-info/
+-rw-r--r--   0 lmxyy      (501) staff       (20)    10758 2024-05-05 03:21:08.000000 distrifuser-0.0.1b1/distrifuser.egg-info/PKG-INFO
+-rw-r--r--   0 lmxyy      (501) staff       (20)      866 2024-05-05 03:21:08.000000 distrifuser-0.0.1b1/distrifuser.egg-info/SOURCES.txt
+-rw-r--r--   0 lmxyy      (501) staff       (20)        1 2024-05-05 03:21:08.000000 distrifuser-0.0.1b1/distrifuser.egg-info/dependency_links.txt
+-rw-r--r--   0 lmxyy      (501) staff       (20)       47 2024-05-05 03:21:08.000000 distrifuser-0.0.1b1/distrifuser.egg-info/requires.txt
+-rw-r--r--   0 lmxyy      (501) staff       (20)       12 2024-05-05 03:21:08.000000 distrifuser-0.0.1b1/distrifuser.egg-info/top_level.txt
+-rw-r--r--   0 lmxyy      (501) staff       (20)       38 2024-05-05 03:21:08.814610 distrifuser-0.0.1b1/setup.cfg
+-rw-r--r--   0 lmxyy      (501) staff       (20)     1079 2024-04-24 18:09:21.000000 distrifuser-0.0.1b1/setup.py
```

### Comparing `distrifuser-0.0.1b0/LICENSE.txt` & `distrifuser-0.0.1b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `distrifuser-0.0.1b0/PKG-INFO` & `distrifuser-0.0.1b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: distrifuser
-Version: 0.0.1b0
+Version: 0.0.1b1
 Summary: DistriFusion: Distributed Parallel Inference for High-Resolution Diffusion Models
 Home-page: https://github.com/mit-han-lab/distrifuser
 Author: Muyang Li, Tianle Cai, Jiaxin Cao, Qinsheng Zhang, Han Cai, Junjie Bai, Yangqing Jia, Ming-Yu Liu, Kai Li and Song Han
 Author-email: muyangli@mit.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -52,15 +52,15 @@
 * Parallel Sampling of Diffusion Models, Shih *et al.*, NeurIPS 2023
 * SDXL: Improving Latent Diffusion Models for High-Resolution Image Synthesis, Podell *et al.*, ICLR 2024
 
 ## Prerequisites
 
 * Python3
 * NVIDIA GPU + CUDA >= 12.0 and corresponding CuDNN
-* [PyTorch](https://pytorch.org) >= 2.2.
+* [PyTorch](https://pytorch.org) = 2.2.
 
 ## Getting Started
 
 ### Installation
 
 After installing [PyTorch](https://pytorch.org), you should be able to install `distrifuser` with PyPI
```

### Comparing `distrifuser-0.0.1b0/README.md` & `distrifuser-0.0.1b1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 * Parallel Sampling of Diffusion Models, Shih *et al.*, NeurIPS 2023
 * SDXL: Improving Latent Diffusion Models for High-Resolution Image Synthesis, Podell *et al.*, ICLR 2024
 
 ## Prerequisites
 
 * Python3
 * NVIDIA GPU + CUDA >= 12.0 and corresponding CuDNN
-* [PyTorch](https://pytorch.org) >= 2.2.
+* [PyTorch](https://pytorch.org) = 2.2.
 
 ## Getting Started
 
 ### Installation
 
 After installing [PyTorch](https://pytorch.org), you should be able to install `distrifuser` with PyPI
```

### Comparing `distrifuser-0.0.1b0/distrifuser/models/base_model.py` & `distrifuser-0.0.1b1/distrifuser/models/base_model.py`

 * *Files identical despite different names*

### Comparing `distrifuser-0.0.1b0/distrifuser/models/distri_sdxl_unet_pp.py` & `distrifuser-0.0.1b1/distrifuser/models/distri_sdxl_unet_pp.py`

 * *Files identical despite different names*

### Comparing `distrifuser-0.0.1b0/distrifuser/models/distri_sdxl_unet_tp.py` & `distrifuser-0.0.1b1/distrifuser/models/distri_sdxl_unet_tp.py`

 * *Files identical despite different names*

### Comparing `distrifuser-0.0.1b0/distrifuser/models/naive_patch_sdxl.py` & `distrifuser-0.0.1b1/distrifuser/models/naive_patch_sdxl.py`

 * *Files identical despite different names*

### Comparing `distrifuser-0.0.1b0/distrifuser/modules/base_module.py` & `distrifuser-0.0.1b1/distrifuser/modules/base_module.py`

 * *Files identical despite different names*

### Comparing `distrifuser-0.0.1b0/distrifuser/modules/pp/attn.py` & `distrifuser-0.0.1b1/distrifuser/modules/pp/attn.py`

 * *Files identical despite different names*

### Comparing `distrifuser-0.0.1b0/distrifuser/modules/pp/conv2d.py` & `distrifuser-0.0.1b1/distrifuser/modules/pp/conv2d.py`

 * *Files identical despite different names*

### Comparing `distrifuser-0.0.1b0/distrifuser/modules/pp/groupnorm.py` & `distrifuser-0.0.1b1/distrifuser/modules/pp/groupnorm.py`

 * *Files identical despite different names*

### Comparing `distrifuser-0.0.1b0/distrifuser/modules/tp/attention.py` & `distrifuser-0.0.1b1/distrifuser/modules/tp/attention.py`

 * *Files identical despite different names*

### Comparing `distrifuser-0.0.1b0/distrifuser/modules/tp/conv2d.py` & `distrifuser-0.0.1b1/distrifuser/modules/tp/conv2d.py`

 * *Files identical despite different names*

### Comparing `distrifuser-0.0.1b0/distrifuser/modules/tp/feed_forward.py` & `distrifuser-0.0.1b1/distrifuser/modules/tp/feed_forward.py`

 * *Files identical despite different names*

### Comparing `distrifuser-0.0.1b0/distrifuser/modules/tp/resnet.py` & `distrifuser-0.0.1b1/distrifuser/modules/tp/resnet.py`

 * *Files identical despite different names*

### Comparing `distrifuser-0.0.1b0/distrifuser/pipelines.py` & `distrifuser-0.0.1b1/distrifuser/pipelines.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,19 @@
         self.pipeline.set_progress_bar_config(**kwargs)
 
     @torch.no_grad()
     def __call__(self, *args, **kwargs):
         assert "height" not in kwargs, "height should not be in kwargs"
         assert "width" not in kwargs, "width should not be in kwargs"
         config = self.distri_config
+        if not config.do_classifier_free_guidance:
+            if "guidance_scale" not in kwargs:
+                kwargs["guidance_scale"] = 1
+            else:
+                assert kwargs["guidance_scale"] == 1
         self.pipeline.unet.set_counter(0)
         return self.pipeline(height=config.height, width=config.width, *args, **kwargs)
 
     @torch.no_grad()
     def prepare(self, **kwargs):
         distri_config = self.distri_config
 
@@ -198,14 +203,19 @@
         self.pipeline.set_progress_bar_config(**kwargs)
 
     @torch.no_grad()
     def __call__(self, *args, **kwargs):
         assert "height" not in kwargs, "height should not be in kwargs"
         assert "width" not in kwargs, "width should not be in kwargs"
         config = self.distri_config
+        if not config.do_classifier_free_guidance:
+            if not "guidance_scale" not in kwargs:
+                kwargs["guidance_scale"] = 1
+            else:
+                assert kwargs["guidance_scale"] == 1
         self.pipeline.unet.set_counter(0)
         return self.pipeline(height=config.height, width=config.width, *args, **kwargs)
 
     @torch.no_grad()
     def prepare(self, **kwargs):
         distri_config = self.distri_config
```

### Comparing `distrifuser-0.0.1b0/distrifuser/utils.py` & `distrifuser-0.0.1b1/distrifuser/utils.py`

 * *Files identical despite different names*

### Comparing `distrifuser-0.0.1b0/distrifuser.egg-info/PKG-INFO` & `distrifuser-0.0.1b1/distrifuser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: distrifuser
-Version: 0.0.1b0
+Version: 0.0.1b1
 Summary: DistriFusion: Distributed Parallel Inference for High-Resolution Diffusion Models
 Home-page: https://github.com/mit-han-lab/distrifuser
 Author: Muyang Li, Tianle Cai, Jiaxin Cao, Qinsheng Zhang, Han Cai, Junjie Bai, Yangqing Jia, Ming-Yu Liu, Kai Li and Song Han
 Author-email: muyangli@mit.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -52,15 +52,15 @@
 * Parallel Sampling of Diffusion Models, Shih *et al.*, NeurIPS 2023
 * SDXL: Improving Latent Diffusion Models for High-Resolution Image Synthesis, Podell *et al.*, ICLR 2024
 
 ## Prerequisites
 
 * Python3
 * NVIDIA GPU + CUDA >= 12.0 and corresponding CuDNN
-* [PyTorch](https://pytorch.org) >= 2.2.
+* [PyTorch](https://pytorch.org) = 2.2.
 
 ## Getting Started
 
 ### Installation
 
 After installing [PyTorch](https://pytorch.org), you should be able to install `distrifuser` with PyPI
```

### Comparing `distrifuser-0.0.1b0/distrifuser.egg-info/SOURCES.txt` & `distrifuser-0.0.1b1/distrifuser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `distrifuser-0.0.1b0/setup.py` & `distrifuser-0.0.1b1/setup.py`

 * *Files identical despite different names*

