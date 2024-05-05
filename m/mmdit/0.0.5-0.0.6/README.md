# Comparing `tmp/mmdit-0.0.5.tar.gz` & `tmp/mmdit-0.0.6.tar.gz`

## Comparing `mmdit-0.0.5.tar` & `mmdit-0.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0   149158 2020-02-02 00:00:00.000000 mmdit-0.0.5/mmdit.png
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 mmdit-0.0.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 mmdit-0.0.5/mmdit/__init__.py
--rw-r--r--   0        0        0     9366 2020-02-02 00:00:00.000000 mmdit-0.0.5/mmdit/mmdit_pytorch.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 mmdit-0.0.5/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 mmdit-0.0.5/LICENSE
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 mmdit-0.0.5/README.md
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mmdit-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 mmdit-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0   149158 2020-02-02 00:00:00.000000 mmdit-0.0.6/mmdit.png
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 mmdit-0.0.6/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 mmdit-0.0.6/mmdit/__init__.py
+-rw-r--r--   0        0        0     9879 2020-02-02 00:00:00.000000 mmdit-0.0.6/mmdit/mmdit_pytorch.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 mmdit-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 mmdit-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 mmdit-0.0.6/README.md
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mmdit-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 mmdit-0.0.6/PKG-INFO
```

### Comparing `mmdit-0.0.5/mmdit.png` & `mmdit-0.0.6/mmdit.png`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.5/.github/workflows/python-publish.yml` & `mmdit-0.0.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.5/mmdit/mmdit_pytorch.py` & `mmdit-0.0.6/mmdit/mmdit_pytorch.py`

 * *Files 8% similar despite different names*

```diff
@@ -217,15 +217,16 @@
 
     def forward(
         self,
         *,
         text_tokens,
         image_tokens,
         text_mask = None,
-        time_cond = None
+        time_cond = None,
+        feedforward_text_tokens = True
     ):
         assert not (exists(time_cond) ^ self.has_cond), 'time condition must be passed in if dim_cond is set at init. it should not be passed in if not set'
 
         if self.has_cond:
             (
                 text_pre_attn_gamma,
                 text_post_attn_gamma,
@@ -279,31 +280,46 @@
         text_tokens = self.text_attn_layernorm(text_tokens)
         image_tokens = self.image_attn_layernorm(image_tokens)
 
         if self.has_cond:
             text_tokens = text_tokens * text_pre_ff_gamma + text_pre_ff_beta
             image_tokens = image_tokens * image_pre_ff_gamma + image_pre_ff_beta
 
-        # feedforward
+        # images feedforward
 
-        text_tokens = self.text_ff(text_tokens)
         image_tokens = self.image_ff(image_tokens)
 
-        # condition feedforward output
+        # images condition feedforward output
 
         if self.has_cond:
-            text_tokens = text_tokens * text_post_ff_gamma
             image_tokens = image_tokens * image_post_ff_gamma
 
-        # add feedforward residual
+        # images feedforward residual
 
-        text_tokens = text_tokens + text_tokens_residual
         image_tokens = image_tokens + image_tokens_residual
 
-        # return output of block
+        # early return, for last block in mmdit
+
+        if not feedforward_text_tokens:
+            return text_tokens, image_tokens
+
+        # text feedforward
+
+        text_tokens = self.text_ff(text_tokens)
+
+        # text condition feedforward output
+
+        if self.has_cond:
+            text_tokens = text_tokens * text_post_ff_gamma
+
+        # text feedforward residual
+
+        text_tokens = text_tokens + text_tokens_residual
+
+        # return
 
         return text_tokens, image_tokens
 
 # mm dit transformer - simply many blocks
 
 class MMDiT(Module):
     def __init__(
@@ -321,18 +337,22 @@
 
     def forward(
         self,
         *,
         text_tokens,
         image_tokens,
         text_mask = None,
-        time_cond = None
+        time_cond = None,
+        omit_last_text_feedforward = True
     ):
-        for block in self.blocks:
+        for ind, block in enumerate(self.blocks):
+            is_last = ind == (len(self.blocks) - 1)
+
             text_tokens, image_tokens = block(
                 time_cond = time_cond,
                 text_tokens = text_tokens,
                 image_tokens = image_tokens,
-                text_mask = text_mask
+                text_mask = text_mask,
+                feedforward_text_tokens = not is_last and omit_last_text_feedforward
             )
 
         return text_tokens, image_tokens
```

### Comparing `mmdit-0.0.5/.gitignore` & `mmdit-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.5/LICENSE` & `mmdit-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.5/README.md` & `mmdit-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.5/pyproject.toml` & `mmdit-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mmdit"
-version = "0.0.5"
+version = "0.0.6"
 description = "MMDiT"
 authors = [
     { name = "Phil Wang", email = "lucidrains@gmail.com" }
 ]
 readme = "README.md"
 requires-python = ">= 3.9"
 license = { file = "LICENSE" }
```

### Comparing `mmdit-0.0.5/PKG-INFO` & `mmdit-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mmdit
-Version: 0.0.5
+Version: 0.0.6
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
-Metadata-Version: 2.3 Name: mmdit Version: 0.0.5 Summary: MMDiT Project-URL:
+Metadata-Version: 2.3 Name: mmdit Version: 0.0.6 Summary: MMDiT Project-URL:
 Homepage, https://pypi.org/project/mmdit/ Project-URL: Repository, https://
 github.com/lucidrains/mmdit Author-email: Phil Wang
 gmail.com> License: MIT License Copyright (c) 2024 Phil Wang Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
```

