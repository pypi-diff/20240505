# Comparing `tmp/mmdit-0.0.7.tar.gz` & `tmp/mmdit-0.0.8.tar.gz`

## Comparing `mmdit-0.0.7.tar` & `mmdit-0.0.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0   149158 2020-02-02 00:00:00.000000 mmdit-0.0.7/mmdit.png
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 mmdit-0.0.7/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 mmdit-0.0.7/mmdit/__init__.py
--rw-r--r--   0        0        0     5905 2020-02-02 00:00:00.000000 mmdit-0.0.7/mmdit/mmdit_generalized_pytorch.py
--rw-r--r--   0        0        0     9938 2020-02-02 00:00:00.000000 mmdit-0.0.7/mmdit/mmdit_pytorch.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 mmdit-0.0.7/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 mmdit-0.0.7/LICENSE
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 mmdit-0.0.7/README.md
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mmdit-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 mmdit-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0   149158 2020-02-02 00:00:00.000000 mmdit-0.0.8/mmdit.png
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 mmdit-0.0.8/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 mmdit-0.0.8/mmdit/__init__.py
+-rw-r--r--   0        0        0     5958 2020-02-02 00:00:00.000000 mmdit-0.0.8/mmdit/mmdit_generalized_pytorch.py
+-rw-r--r--   0        0        0     9957 2020-02-02 00:00:00.000000 mmdit-0.0.8/mmdit/mmdit_pytorch.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 mmdit-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 mmdit-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 mmdit-0.0.8/README.md
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mmdit-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 mmdit-0.0.8/PKG-INFO
```

### Comparing `mmdit-0.0.7/mmdit.png` & `mmdit-0.0.8/mmdit.png`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.7/.github/workflows/python-publish.yml` & `mmdit-0.0.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.7/mmdit/mmdit_generalized_pytorch.py` & `mmdit-0.0.8/mmdit/mmdit_generalized_pytorch.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Optional, Tuple
+from __future__ import annotations
+from typing import Tuple
 
 import torch
 from torch import nn
 from torch import Tensor
 import torch.nn.functional as F
 from torch.nn import Module, ModuleList
 
@@ -43,15 +44,17 @@
 
             self.to_cond = nn.Sequential(
                 nn.SiLU(),
                 cond_linear
             )
 
             nn.init.zeros_(cond_linear.weight)
-            nn.init.constant_(cond_linear.bias, 1.)
+
+            nn.init.constant_(cond_linear.bias[:dim], 1.)
+            nn.init.zeros_(cond_linear.bias[dim:])
 
     def forward(
         self,
         x,
         cond = None
     ):
         assert not (exists(cond) ^ self.has_cond), 'condition must be passed in if dim_cond is set at init. it should not be passed in if not set'
@@ -85,15 +88,15 @@
 
         # handle optional time conditioning
 
         has_cond = exists(dim_cond)
         self.has_cond = has_cond
 
         if has_cond:
-            cond_linear = nn.Linear(dim_cond, sum(dim_modalities) * self.num_modalities)
+            cond_linear = nn.Linear(dim_cond, sum(dim_modalities) * 2)
 
             self.to_post_branch_gammas = nn.Sequential(
                 nn.SiLU(),
                 cond_linear
             )
 
             nn.init.zeros_(cond_linear.weight)
@@ -120,15 +123,15 @@
         feedforwards = [FeedForward(dim, **ff_kwargs) for dim in dim_modalities]
         self.feedforwards = ModuleList(feedforwards)
 
     def forward(
         self,
         *,
         modality_tokens: Tuple[Tensor, ...],
-        modality_masks: Optional[Tuple[Optional[Tensor], ...]] = None,
+        modality_masks: Tuple[Tensor | None, ...] | None = None,
         time_cond = None
     ):
         assert len(modality_tokens) == self.num_modalities
         assert not (exists(time_cond) ^ self.has_cond), 'condition must be passed in if dim_cond is set at init. it should not be passed in if not set'
 
         ln_kwargs = dict()
 
@@ -193,15 +196,15 @@
         blocks = [MMDiTBlock(**block_kwargs) for _ in range(depth)]
         self.blocks = ModuleList(blocks)
 
     def forward(
         self,
         *,
         modality_tokens: Tuple[Tensor, ...],
-        modality_masks: Optional[Tuple[Optional[Tensor], ...]] = None,
+        modality_masks: Tuple[Tensor | None, ...] | None = None,
         time_cond = None
     ):
         for block in self.blocks:
             modality_tokens = block(
                 time_cond = time_cond,
                 modality_tokens = modality_tokens,
                 modality_masks = modality_masks
```

### Comparing `mmdit-0.0.7/mmdit/mmdit_pytorch.py` & `mmdit-0.0.8/mmdit/mmdit_pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Optional, Tuple
+from __future__ import annotations
+from typing import Tuple
 
 import torch
 from torch import nn
 from torch import Tensor
 import torch.nn.functional as F
 from torch.nn import Module, ModuleList
 
@@ -82,15 +83,15 @@
             self.k_rmsnorms = ModuleList([MultiHeadRMSNorm(dim_head, heads = heads) for _ in range(num_inputs)])
 
         self.register_buffer('dummy', torch.tensor(0), persistent = False)
 
     def forward(
         self,
         inputs: Tuple[Tensor],
-        masks: Optional[Tuple[Optional[Tensor]]] = None
+        masks: Tuple[Tensor | None] | None = None
     ):
 
         device = self.dummy.device
 
         assert len(inputs) == self.num_inputs
 
         masks = default(masks, (None,) * self.num_inputs)
```

### Comparing `mmdit-0.0.7/.gitignore` & `mmdit-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.7/LICENSE` & `mmdit-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.7/README.md` & `mmdit-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.7/pyproject.toml` & `mmdit-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mmdit"
-version = "0.0.7"
+version = "0.0.8"
 description = "MMDiT"
 authors = [
     { name = "Phil Wang", email = "lucidrains@gmail.com" }
 ]
 readme = "README.md"
 requires-python = ">= 3.9"
 license = { file = "LICENSE" }
```

### Comparing `mmdit-0.0.7/PKG-INFO` & `mmdit-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mmdit
-Version: 0.0.7
+Version: 0.0.8
 Summary: MMDiT
 Project-URL: Homepage, https://pypi.org/project/mmdit/
 Project-URL: Repository, https://github.com/lucidrains/mmdit
 Author-email: Phil Wang <lucidrains@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Phil Wang
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: mmdit Version: 0.0.7 Summary: MMDiT Project-URL:
+Metadata-Version: 2.3 Name: mmdit Version: 0.0.8 Summary: MMDiT Project-URL:
 Homepage, https://pypi.org/project/mmdit/ Project-URL: Repository, https://
 github.com/lucidrains/mmdit Author-email: Phil Wang
 gmail.com> License: MIT License Copyright (c) 2024 Phil Wang Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
```

