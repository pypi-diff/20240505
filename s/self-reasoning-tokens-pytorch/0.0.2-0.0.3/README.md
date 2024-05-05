# Comparing `tmp/self_reasoning_tokens_pytorch-0.0.2.tar.gz` & `tmp/self_reasoning_tokens_pytorch-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "self_reasoning_tokens_pytorch-0.0.2.tar", last modified: Fri May  3 14:38:00 2024, max compression
+gzip compressed data, was "self_reasoning_tokens_pytorch-0.0.3.tar", last modified: Sun May  5 18:00:49 2024, max compression
```

## Comparing `self_reasoning_tokens_pytorch-0.0.2.tar` & `self_reasoning_tokens_pytorch-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:38:00.743528 self_reasoning_tokens_pytorch-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-03 14:37:52.000000 self_reasoning_tokens_pytorch-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-03 14:38:00.743528 self_reasoning_tokens_pytorch-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-03 14:37:52.000000 self_reasoning_tokens_pytorch-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:38:00.743528 self_reasoning_tokens_pytorch-0.0.2/self_reasoning_tokens_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-03 14:37:52.000000 self_reasoning_tokens_pytorch-0.0.2/self_reasoning_tokens_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-03 14:37:52.000000 self_reasoning_tokens_pytorch-0.0.2/self_reasoning_tokens_pytorch/attention_with_stop_graddable_qkv.py
--rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-05-03 14:37:52.000000 self_reasoning_tokens_pytorch-0.0.2/self_reasoning_tokens_pytorch/self_reasoning_tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:38:00.743528 self_reasoning_tokens_pytorch-0.0.2/self_reasoning_tokens_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-03 14:38:00.000000 self_reasoning_tokens_pytorch-0.0.2/self_reasoning_tokens_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-03 14:38:00.000000 self_reasoning_tokens_pytorch-0.0.2/self_reasoning_tokens_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 14:38:00.000000 self_reasoning_tokens_pytorch-0.0.2/self_reasoning_tokens_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-03 14:38:00.000000 self_reasoning_tokens_pytorch-0.0.2/self_reasoning_tokens_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-03 14:38:00.000000 self_reasoning_tokens_pytorch-0.0.2/self_reasoning_tokens_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 14:38:00.743528 self_reasoning_tokens_pytorch-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-03 14:37:52.000000 self_reasoning_tokens_pytorch-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:00:49.321954 self_reasoning_tokens_pytorch-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-05 18:00:45.000000 self_reasoning_tokens_pytorch-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-05 18:00:49.321954 self_reasoning_tokens_pytorch-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-05 18:00:45.000000 self_reasoning_tokens_pytorch-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:00:49.321954 self_reasoning_tokens_pytorch-0.0.3/self_reasoning_tokens_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-05 18:00:45.000000 self_reasoning_tokens_pytorch-0.0.3/self_reasoning_tokens_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-05 18:00:45.000000 self_reasoning_tokens_pytorch-0.0.3/self_reasoning_tokens_pytorch/attention_with_stop_graddable_qkv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7309 2024-05-05 18:00:45.000000 self_reasoning_tokens_pytorch-0.0.3/self_reasoning_tokens_pytorch/self_reasoning_tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:00:49.321954 self_reasoning_tokens_pytorch-0.0.3/self_reasoning_tokens_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-05 18:00:49.000000 self_reasoning_tokens_pytorch-0.0.3/self_reasoning_tokens_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-05 18:00:49.000000 self_reasoning_tokens_pytorch-0.0.3/self_reasoning_tokens_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 18:00:49.000000 self_reasoning_tokens_pytorch-0.0.3/self_reasoning_tokens_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-05 18:00:49.000000 self_reasoning_tokens_pytorch-0.0.3/self_reasoning_tokens_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-05 18:00:49.000000 self_reasoning_tokens_pytorch-0.0.3/self_reasoning_tokens_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 18:00:49.321954 self_reasoning_tokens_pytorch-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-05 18:00:45.000000 self_reasoning_tokens_pytorch-0.0.3/setup.py
```

### Comparing `self_reasoning_tokens_pytorch-0.0.2/LICENSE` & `self_reasoning_tokens_pytorch-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `self_reasoning_tokens_pytorch-0.0.2/PKG-INFO` & `self_reasoning_tokens_pytorch-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: self-reasoning-tokens-pytorch
-Version: 0.0.2
+Version: 0.0.3
 Summary: Self Reasoning Tokens
 Home-page: https://github.com/lucidrains/self-reasoning-tokens-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,adaptive computation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `self_reasoning_tokens_pytorch-0.0.2/self_reasoning_tokens_pytorch/attention_with_stop_graddable_qkv.py` & `self_reasoning_tokens_pytorch-0.0.3/self_reasoning_tokens_pytorch/attention_with_stop_graddable_qkv.py`

 * *Files 19% similar despite different names*

```diff
@@ -74,24 +74,37 @@
             q_stop_grad_mask,
             k_stop_grad_mask,
             v_stop_grad_mask
         ) = ctx.args
 
         q, k, v, p, o = ctx.saved_tensors
 
+        # stop grad masks are either type bool, with True indicating stop grad, or can be type float, in which case it will scale the gradients
+
+        if q_stop_grad_mask.dtype == torch.bool:
+            q_stop_grad_mask = (~q_stop_grad_mask).float()
+
+        if k_stop_grad_mask.dtype == torch.bool:
+            k_stop_grad_mask = (~k_stop_grad_mask).float()
+
+        print(v_stop_grad_mask.dtype)
+        if v_stop_grad_mask.dtype == torch.bool:
+            print('hmmm')
+            v_stop_grad_mask = (~v_stop_grad_mask).float()
+
         # softmax D
 
         D = (do * o).sum(dim = -1, keepdims = True)        
 
         # stop grad for values
 
         p_v = p
 
         if exists(v_stop_grad_mask):
-            p_v = p_v.masked_fill(v_stop_grad_mask, 0.)
+            p_v.mul_(v_stop_grad_mask)
 
         # dv
 
         dv = einsum(p_v, do, 'b h i j, b h i d -> b h j d')
 
         # prep for dq and dk
 
@@ -99,18 +112,18 @@
         ds = p * scale * (dp - D)
 
         # handle stop grad masking for queries and keys
 
         ds_q = ds_k = ds
 
         if exists(q_stop_grad_mask):
-            ds_q = ds_q.masked_fill(q_stop_grad_mask, 0.)
+            ds_q.mul_(q_stop_grad_mask)
 
         if exists(k_stop_grad_mask):            
-            ds_k = ds_k.masked_fill(k_stop_grad_mask, 0.)
+            ds_k.mul_(k_stop_grad_mask)
 
         # dq and dk
 
         dq = einsum(ds_q, k, 'b h i j, b h j d -> b h i d')
         dk = einsum(ds_k, q, 'b h i j, b h i d -> b h j d')
 
         return dq, dk, dv, None, None, None, None, None, None
```

### Comparing `self_reasoning_tokens_pytorch-0.0.2/self_reasoning_tokens_pytorch/self_reasoning_tokens.py` & `self_reasoning_tokens_pytorch-0.0.3/self_reasoning_tokens_pytorch/self_reasoning_tokens.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import torch
-from torch import nn, Tensor
+from torch import nn
 import torch.nn.functional as F
 from torch.nn import Module, ModuleList
 
 from einops import einsum, rearrange, repeat, reduce
 from einops.layers.torch import Rearrange
 
 from x_transformers import (
@@ -54,19 +54,27 @@
         stop_grad_attn_mask = None
     ):
         seq, device = x.shape[-2], x.device
 
         q, k, v = self.to_qkv(x)
 
         if exists(stop_grad_attn_mask):
+            if not isinstance(stop_grad_attn_mask, tuple):
+                stop_grad_attn_mask = (None, stop_grad_attn_mask, stop_grad_attn_mask)
+
+            assert len(stop_grad_attn_mask) == 3, 'stop_grad_attn_mask must be either a stop grad mask (implicit for key / values) or a tuple of 3 Tensor for individual stop grads of queries, keys, values'
+
+            q_stop_grad, k_stop_grad, v_stop_grad = stop_grad_attn_mask
+
             out = stop_graddable_attn(
                 q, k, v,
                 attn_mask = attn_mask,
-                k_stop_grad_mask = stop_grad_attn_mask,
-                v_stop_grad_mask = stop_grad_attn_mask
+                q_stop_grad_mask = q_stop_grad,
+                k_stop_grad_mask = k_stop_grad,
+                v_stop_grad_mask = v_stop_grad
             )
 
         else:
             q = q * self.scale
             sim = einsum(q, k, 'b h i d, b h j d -> b h i j')
 
             causal_mask = torch.ones((seq, seq), device = device, dtype = torch.bool).triu(1)
```

### Comparing `self_reasoning_tokens_pytorch-0.0.2/self_reasoning_tokens_pytorch.egg-info/PKG-INFO` & `self_reasoning_tokens_pytorch-0.0.3/self_reasoning_tokens_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: self-reasoning-tokens-pytorch
-Version: 0.0.2
+Version: 0.0.3
 Summary: Self Reasoning Tokens
 Home-page: https://github.com/lucidrains/self-reasoning-tokens-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,adaptive computation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `self_reasoning_tokens_pytorch-0.0.2/setup.py` & `self_reasoning_tokens_pytorch-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'self-reasoning-tokens-pytorch',
   packages = find_packages(exclude = []),
-  version = '0.0.2',
+  version = '0.0.3',
   license='MIT',
   description = 'Self Reasoning Tokens',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/self-reasoning-tokens-pytorch',
   keywords = [
```

