# Comparing `tmp/mmdit-0.0.4.tar.gz` & `tmp/mmdit-0.0.5.tar.gz`

## Comparing `mmdit-0.0.4.tar` & `mmdit-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0   149158 2020-02-02 00:00:00.000000 mmdit-0.0.4/mmdit.png
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 mmdit-0.0.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 mmdit-0.0.4/mmdit/__init__.py
--rw-r--r--   0        0        0     9344 2020-02-02 00:00:00.000000 mmdit-0.0.4/mmdit/mmdit_pytorch.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 mmdit-0.0.4/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 mmdit-0.0.4/LICENSE
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 mmdit-0.0.4/README.md
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mmdit-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 mmdit-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0   149158 2020-02-02 00:00:00.000000 mmdit-0.0.5/mmdit.png
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 mmdit-0.0.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 mmdit-0.0.5/mmdit/__init__.py
+-rw-r--r--   0        0        0     9366 2020-02-02 00:00:00.000000 mmdit-0.0.5/mmdit/mmdit_pytorch.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 mmdit-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 mmdit-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 mmdit-0.0.5/README.md
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mmdit-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 mmdit-0.0.5/PKG-INFO
```

### Comparing `mmdit-0.0.4/mmdit.png` & `mmdit-0.0.5/mmdit.png`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.4/.github/workflows/python-publish.yml` & `mmdit-0.0.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.4/mmdit/mmdit_pytorch.py` & `mmdit-0.0.5/mmdit/mmdit_pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         self.gamma = nn.Parameter(torch.ones(heads, 1, dim))
 
     def forward(self, x):
         return F.normalize(x, dim = -1) * self.gamma * self.scale
 
 # attention
 
-class Attention(Module):
+class JointAttention(Module):
     def __init__(
         self,
         *,
         dim,
         dim_inputs: Tuple[int, ...],
         dim_head = 64,
         heads = 8,
@@ -200,15 +200,15 @@
         self.image_attn_layernorm = nn.LayerNorm(dim_image, elementwise_affine = not has_cond)
 
         self.text_ff_layernorm = nn.LayerNorm(dim_text, elementwise_affine = not has_cond)
         self.image_ff_layernorm = nn.LayerNorm(dim_image, elementwise_affine = not has_cond)
 
         # attention and feedforward
 
-        self.attn = Attention(
+        self.joint_attn = JointAttention(
             dim = dim_joint_attn,
             dim_inputs = (dim_text, dim_image),
             dim_head = dim_head,
             heads = heads,
             flash = flash_attn
         )
 
@@ -251,15 +251,15 @@
 
         if self.has_cond:
             text_tokens = text_tokens * text_pre_attn_gamma + text_pre_attn_beta
             image_tokens = image_tokens * image_pre_attn_gamma + image_pre_attn_beta
 
         # attention
 
-        text_tokens, image_tokens = self.attn(
+        text_tokens, image_tokens = self.joint_attn(
             inputs = (text_tokens, image_tokens),
             masks = (text_mask, None)
         )
 
         # condition attention output
 
         if self.has_cond:
```

### Comparing `mmdit-0.0.4/.gitignore` & `mmdit-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.4/LICENSE` & `mmdit-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.4/README.md` & `mmdit-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.4/pyproject.toml` & `mmdit-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mmdit"
-version = "0.0.4"
+version = "0.0.5"
 description = "MMDiT"
 authors = [
     { name = "Phil Wang", email = "lucidrains@gmail.com" }
 ]
 readme = "README.md"
 requires-python = ">= 3.9"
 license = { file = "LICENSE" }
```

### Comparing `mmdit-0.0.4/PKG-INFO` & `mmdit-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mmdit
-Version: 0.0.4
+Version: 0.0.5
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
-Metadata-Version: 2.3 Name: mmdit Version: 0.0.4 Summary: MMDiT Project-URL:
+Metadata-Version: 2.3 Name: mmdit Version: 0.0.5 Summary: MMDiT Project-URL:
 Homepage, https://pypi.org/project/mmdit/ Project-URL: Repository, https://
 github.com/lucidrains/mmdit Author-email: Phil Wang
 gmail.com> License: MIT License Copyright (c) 2024 Phil Wang Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
```

