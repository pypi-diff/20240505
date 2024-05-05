# Comparing `tmp/mmdit-0.0.6.tar.gz` & `tmp/mmdit-0.0.7.tar.gz`

## Comparing `mmdit-0.0.6.tar` & `mmdit-0.0.7.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0   149158 2020-02-02 00:00:00.000000 mmdit-0.0.6/mmdit.png
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 mmdit-0.0.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 mmdit-0.0.6/mmdit/__init__.py
--rw-r--r--   0        0        0     9879 2020-02-02 00:00:00.000000 mmdit-0.0.6/mmdit/mmdit_pytorch.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 mmdit-0.0.6/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 mmdit-0.0.6/LICENSE
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 mmdit-0.0.6/README.md
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mmdit-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 mmdit-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0   149158 2020-02-02 00:00:00.000000 mmdit-0.0.7/mmdit.png
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 mmdit-0.0.7/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 mmdit-0.0.7/mmdit/__init__.py
+-rw-r--r--   0        0        0     5905 2020-02-02 00:00:00.000000 mmdit-0.0.7/mmdit/mmdit_generalized_pytorch.py
+-rw-r--r--   0        0        0     9938 2020-02-02 00:00:00.000000 mmdit-0.0.7/mmdit/mmdit_pytorch.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 mmdit-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 mmdit-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 mmdit-0.0.7/README.md
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mmdit-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 mmdit-0.0.7/PKG-INFO
```

### Comparing `mmdit-0.0.6/mmdit.png` & `mmdit-0.0.7/mmdit.png`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.6/.github/workflows/python-publish.yml` & `mmdit-0.0.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.6/mmdit/mmdit_pytorch.py` & `mmdit-0.0.7/mmdit/mmdit_pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,16 @@
         masks: Optional[Tuple[Optional[Tensor]]] = None
     ):
 
         device = self.dummy.device
 
         assert len(inputs) == self.num_inputs
 
+        masks = default(masks, (None,) * self.num_inputs)
+
         # project each modality separately for qkv
         # also handle masks, assume None means attend to all tokens
 
         all_qkvs = []
         all_masks = []
 
         for x, mask, to_qkv, q_rmsnorm, k_rmsnorm in zip(inputs, masks, self.to_qkv, self.q_rmsnorms, self.k_rmsnorms):
```

### Comparing `mmdit-0.0.6/.gitignore` & `mmdit-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.6/LICENSE` & `mmdit-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.6/README.md` & `mmdit-0.0.7/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -45,14 +45,48 @@
     time_cond = time_cond,
     text_tokens = text_tokens,
     text_mask = text_mask,
     image_tokens = image_tokens
 )
 ```
 
+A generalized version can be used as so
+
+```python
+import torch
+from mmdit.mmdit_generalized_pytorch import MMDiT
+
+mmdit = MMDiT(
+    depth = 2, 
+    dim_modalities = (768, 512, 384),
+    dim_joint_attn = 512,
+    dim_cond = 256,
+    qk_rmsnorm = True
+)
+
+# mock inputs
+
+time_cond = torch.randn(1, 256)
+
+text_tokens = torch.randn(1, 512, 768)
+text_mask = torch.ones((1, 512)).bool()
+
+video_tokens = torch.randn(1, 1024, 512)
+
+audio_tokens = torch.randn(1, 256, 384)
+
+# forward
+
+text_tokens, video_tokens, audio_tokens = mmdit(
+    modality_tokens = (text_tokens, video_tokens, audio_tokens),
+    modality_masks = (text_mask, None, None),
+    time_cond = time_cond,
+)
+```
+
 ## Citations
 
 ```bibtex
 @article{Esser2024ScalingRF,
     title   = {Scaling Rectified Flow Transformers for High-Resolution Image Synthesis},
     author  = {Patrick Esser and Sumith Kulal and A. Blattmann and Rahim Entezari and Jonas Muller and Harry Saini and Yam Levi and Dominik Lorenz and Axel Sauer and Frederic Boesel and Dustin Podell and Tim Dockhorn and Zion English and Kyle Lacey and Alex Goodwin and Yannik Marek and Robin Rombach},
     journal = {ArXiv},
```

#### html2text {}

```diff
@@ -6,16 +6,24 @@
 learned gating. ## Install ```bash $ pip install mmdit ``` ## Usage ```python
 import torch from mmdit import MMDiTBlock # define mm dit block block =
 MMDiTBlock( dim_joint_attn = 512, dim_cond = 256, dim_text = 768, dim_image =
 512, qk_rmsnorm = True ) # mock inputs time_cond = torch.randn(1, 256)
 text_tokens = torch.randn(1, 512, 768) text_mask = torch.ones((1, 512)).bool()
 image_tokens = torch.randn(1, 1024, 512) # single block forward
 text_tokens_next, image_tokens_next = block( time_cond = time_cond, text_tokens
-= text_tokens, text_mask = text_mask, image_tokens = image_tokens ) ``` ##
-Citations ```bibtex @article{Esser2024ScalingRF, title = {Scaling Rectified
-Flow Transformers for High-Resolution Image Synthesis}, author = {Patrick Esser
-and Sumith Kulal and A. Blattmann and Rahim Entezari and Jonas Muller and Harry
-Saini and Yam Levi and Dominik Lorenz and Axel Sauer and Frederic Boesel and
-Dustin Podell and Tim Dockhorn and Zion English and Kyle Lacey and Alex Goodwin
-and Yannik Marek and Robin Rombach}, journal = {ArXiv}, year = {2024}, volume =
-{abs/2403.03206}, url = {https://api.semanticscholar.org/CorpusID:268247980} }
-```
+= text_tokens, text_mask = text_mask, image_tokens = image_tokens ) ``` A
+generalized version can be used as so ```python import torch from
+mmdit.mmdit_generalized_pytorch import MMDiT mmdit = MMDiT( depth = 2,
+dim_modalities = (768, 512, 384), dim_joint_attn = 512, dim_cond = 256,
+qk_rmsnorm = True ) # mock inputs time_cond = torch.randn(1, 256) text_tokens =
+torch.randn(1, 512, 768) text_mask = torch.ones((1, 512)).bool() video_tokens =
+torch.randn(1, 1024, 512) audio_tokens = torch.randn(1, 256, 384) # forward
+text_tokens, video_tokens, audio_tokens = mmdit( modality_tokens =
+(text_tokens, video_tokens, audio_tokens), modality_masks = (text_mask, None,
+None), time_cond = time_cond, ) ``` ## Citations ```bibtex @article
+{Esser2024ScalingRF, title = {Scaling Rectified Flow Transformers for High-
+Resolution Image Synthesis}, author = {Patrick Esser and Sumith Kulal and A.
+Blattmann and Rahim Entezari and Jonas Muller and Harry Saini and Yam Levi and
+Dominik Lorenz and Axel Sauer and Frederic Boesel and Dustin Podell and Tim
+Dockhorn and Zion English and Kyle Lacey and Alex Goodwin and Yannik Marek and
+Robin Rombach}, journal = {ArXiv}, year = {2024}, volume = {abs/2403.03206},
+url = {https://api.semanticscholar.org/CorpusID:268247980} } ```
```

### Comparing `mmdit-0.0.6/pyproject.toml` & `mmdit-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mmdit"
-version = "0.0.6"
+version = "0.0.7"
 description = "MMDiT"
 authors = [
     { name = "Phil Wang", email = "lucidrains@gmail.com" }
 ]
 readme = "README.md"
 requires-python = ">= 3.9"
 license = { file = "LICENSE" }
```

### Comparing `mmdit-0.0.6/PKG-INFO` & `mmdit-0.0.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mmdit
-Version: 0.0.6
+Version: 0.0.7
 Summary: MMDiT
 Project-URL: Homepage, https://pypi.org/project/mmdit/
 Project-URL: Repository, https://github.com/lucidrains/mmdit
 Author-email: Phil Wang <lucidrains@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Phil Wang
@@ -87,14 +87,48 @@
     time_cond = time_cond,
     text_tokens = text_tokens,
     text_mask = text_mask,
     image_tokens = image_tokens
 )
 ```
 
+A generalized version can be used as so
+
+```python
+import torch
+from mmdit.mmdit_generalized_pytorch import MMDiT
+
+mmdit = MMDiT(
+    depth = 2, 
+    dim_modalities = (768, 512, 384),
+    dim_joint_attn = 512,
+    dim_cond = 256,
+    qk_rmsnorm = True
+)
+
+# mock inputs
+
+time_cond = torch.randn(1, 256)
+
+text_tokens = torch.randn(1, 512, 768)
+text_mask = torch.ones((1, 512)).bool()
+
+video_tokens = torch.randn(1, 1024, 512)
+
+audio_tokens = torch.randn(1, 256, 384)
+
+# forward
+
+text_tokens, video_tokens, audio_tokens = mmdit(
+    modality_tokens = (text_tokens, video_tokens, audio_tokens),
+    modality_masks = (text_mask, None, None),
+    time_cond = time_cond,
+)
+```
+
 ## Citations
 
 ```bibtex
 @article{Esser2024ScalingRF,
     title   = {Scaling Rectified Flow Transformers for High-Resolution Image Synthesis},
     author  = {Patrick Esser and Sumith Kulal and A. Blattmann and Rahim Entezari and Jonas Muller and Harry Saini and Yam Levi and Dominik Lorenz and Axel Sauer and Frederic Boesel and Dustin Podell and Tim Dockhorn and Zion English and Kyle Lacey and Alex Goodwin and Yannik Marek and Robin Rombach},
     journal = {ArXiv},
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: mmdit Version: 0.0.6 Summary: MMDiT Project-URL:
+Metadata-Version: 2.3 Name: mmdit Version: 0.0.7 Summary: MMDiT Project-URL:
 Homepage, https://pypi.org/project/mmdit/ Project-URL: Repository, https://
 github.com/lucidrains/mmdit Author-email: Phil Wang
 gmail.com> License: MIT License Copyright (c) 2024 Phil Wang Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -31,16 +31,24 @@
 learned gating. ## Install ```bash $ pip install mmdit ``` ## Usage ```python
 import torch from mmdit import MMDiTBlock # define mm dit block block =
 MMDiTBlock( dim_joint_attn = 512, dim_cond = 256, dim_text = 768, dim_image =
 512, qk_rmsnorm = True ) # mock inputs time_cond = torch.randn(1, 256)
 text_tokens = torch.randn(1, 512, 768) text_mask = torch.ones((1, 512)).bool()
 image_tokens = torch.randn(1, 1024, 512) # single block forward
 text_tokens_next, image_tokens_next = block( time_cond = time_cond, text_tokens
-= text_tokens, text_mask = text_mask, image_tokens = image_tokens ) ``` ##
-Citations ```bibtex @article{Esser2024ScalingRF, title = {Scaling Rectified
-Flow Transformers for High-Resolution Image Synthesis}, author = {Patrick Esser
-and Sumith Kulal and A. Blattmann and Rahim Entezari and Jonas Muller and Harry
-Saini and Yam Levi and Dominik Lorenz and Axel Sauer and Frederic Boesel and
-Dustin Podell and Tim Dockhorn and Zion English and Kyle Lacey and Alex Goodwin
-and Yannik Marek and Robin Rombach}, journal = {ArXiv}, year = {2024}, volume =
-{abs/2403.03206}, url = {https://api.semanticscholar.org/CorpusID:268247980} }
-```
+= text_tokens, text_mask = text_mask, image_tokens = image_tokens ) ``` A
+generalized version can be used as so ```python import torch from
+mmdit.mmdit_generalized_pytorch import MMDiT mmdit = MMDiT( depth = 2,
+dim_modalities = (768, 512, 384), dim_joint_attn = 512, dim_cond = 256,
+qk_rmsnorm = True ) # mock inputs time_cond = torch.randn(1, 256) text_tokens =
+torch.randn(1, 512, 768) text_mask = torch.ones((1, 512)).bool() video_tokens =
+torch.randn(1, 1024, 512) audio_tokens = torch.randn(1, 256, 384) # forward
+text_tokens, video_tokens, audio_tokens = mmdit( modality_tokens =
+(text_tokens, video_tokens, audio_tokens), modality_masks = (text_mask, None,
+None), time_cond = time_cond, ) ``` ## Citations ```bibtex @article
+{Esser2024ScalingRF, title = {Scaling Rectified Flow Transformers for High-
+Resolution Image Synthesis}, author = {Patrick Esser and Sumith Kulal and A.
+Blattmann and Rahim Entezari and Jonas Muller and Harry Saini and Yam Levi and
+Dominik Lorenz and Axel Sauer and Frederic Boesel and Dustin Podell and Tim
+Dockhorn and Zion English and Kyle Lacey and Alex Goodwin and Yannik Marek and
+Robin Rombach}, journal = {ArXiv}, year = {2024}, volume = {abs/2403.03206},
+url = {https://api.semanticscholar.org/CorpusID:268247980} } ```
```

