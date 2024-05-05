# Comparing `tmp/mmdit-0.0.3.tar.gz` & `tmp/mmdit-0.0.4.tar.gz`

## Comparing `mmdit-0.0.3.tar` & `mmdit-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0   149158 2020-02-02 00:00:00.000000 mmdit-0.0.3/mmdit.png
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 mmdit-0.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 mmdit-0.0.3/mmdit/__init__.py
--rw-r--r--   0        0        0     9339 2020-02-02 00:00:00.000000 mmdit-0.0.3/mmdit/mmdit_pytorch.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 mmdit-0.0.3/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 mmdit-0.0.3/LICENSE
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 mmdit-0.0.3/README.md
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mmdit-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 mmdit-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0   149158 2020-02-02 00:00:00.000000 mmdit-0.0.4/mmdit.png
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 mmdit-0.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 mmdit-0.0.4/mmdit/__init__.py
+-rw-r--r--   0        0        0     9344 2020-02-02 00:00:00.000000 mmdit-0.0.4/mmdit/mmdit_pytorch.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 mmdit-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 mmdit-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 mmdit-0.0.4/README.md
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mmdit-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 mmdit-0.0.4/PKG-INFO
```

### Comparing `mmdit-0.0.3/mmdit.png` & `mmdit-0.0.4/mmdit.png`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.3/.github/workflows/python-publish.yml` & `mmdit-0.0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.3/mmdit/mmdit_pytorch.py` & `mmdit-0.0.4/mmdit/mmdit_pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 # attention
 
 class Attention(Module):
     def __init__(
         self,
         *,
         dim,
-        dim_inputs: Tuple[int],
+        dim_inputs: Tuple[int, ...],
         dim_head = 64,
         heads = 8,
         qk_rmsnorm = False,
         flash = False,
         attend_kwargs: dict = dict()
     ):
         super().__init__()
```

### Comparing `mmdit-0.0.3/.gitignore` & `mmdit-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.3/LICENSE` & `mmdit-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.3/README.md` & `mmdit-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.3/pyproject.toml` & `mmdit-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mmdit"
-version = "0.0.3"
+version = "0.0.4"
 description = "MMDiT"
 authors = [
     { name = "Phil Wang", email = "lucidrains@gmail.com" }
 ]
 readme = "README.md"
 requires-python = ">= 3.9"
 license = { file = "LICENSE" }
```

### Comparing `mmdit-0.0.3/PKG-INFO` & `mmdit-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mmdit
-Version: 0.0.3
+Version: 0.0.4
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
-Metadata-Version: 2.3 Name: mmdit Version: 0.0.3 Summary: MMDiT Project-URL:
+Metadata-Version: 2.3 Name: mmdit Version: 0.0.4 Summary: MMDiT Project-URL:
 Homepage, https://pypi.org/project/mmdit/ Project-URL: Repository, https://
 github.com/lucidrains/mmdit Author-email: Phil Wang
 gmail.com> License: MIT License Copyright (c) 2024 Phil Wang Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
```

