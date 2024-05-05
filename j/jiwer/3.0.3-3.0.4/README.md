# Comparing `tmp/jiwer-3.0.3.tar.gz` & `tmp/jiwer-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jiwer-3.0.3.tar", max compression
+gzip compressed data, was "jiwer-3.0.4.tar", max compression
```

## Comparing `jiwer-3.0.3.tar` & `jiwer-3.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11339 2023-08-31 18:25:58.864252 jiwer-3.0.3/LICENSE
--rw-r--r--   0        0        0     1729 2023-08-31 18:25:58.864252 jiwer-3.0.3/README.md
--rw-r--r--   0        0        0      145 2023-08-31 18:25:58.864252 jiwer-3.0.3/jiwer/__init__.py
--rw-r--r--   0        0        0     5971 2023-08-31 18:25:58.864252 jiwer-3.0.3/jiwer/alignment.py
--rw-r--r--   0        0        0     3731 2023-08-31 18:25:58.864252 jiwer-3.0.3/jiwer/cli.py
--rw-r--r--   0        0        0    15308 2023-08-31 18:25:58.864252 jiwer-3.0.3/jiwer/measures.py
--rw-r--r--   0        0        0    13422 2023-08-31 18:25:58.864252 jiwer-3.0.3/jiwer/process.py
--rw-r--r--   0        0        0     3670 2023-08-31 18:25:58.868252 jiwer-3.0.3/jiwer/transformations.py
--rw-r--r--   0        0        0    17834 2023-08-31 18:25:58.868252 jiwer-3.0.3/jiwer/transforms.py
--rw-r--r--   0        0        0      647 2023-08-31 18:25:58.868252 jiwer-3.0.3/pyproject.toml
--rw-r--r--   0        0        0     2553 1970-01-01 00:00:00.000000 jiwer-3.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11339 2024-05-05 08:14:27.707219 jiwer-3.0.4/LICENSE
+-rw-r--r--   0        0        0     1729 2024-05-05 08:14:27.707219 jiwer-3.0.4/README.md
+-rw-r--r--   0        0        0      145 2024-05-05 08:14:27.707219 jiwer-3.0.4/jiwer/__init__.py
+-rw-r--r--   0        0        0     5971 2024-05-05 08:14:27.707219 jiwer-3.0.4/jiwer/alignment.py
+-rw-r--r--   0        0        0     4130 2024-05-05 08:14:27.707219 jiwer-3.0.4/jiwer/cli.py
+-rw-r--r--   0        0        0    15308 2024-05-05 08:14:27.707219 jiwer-3.0.4/jiwer/measures.py
+-rw-r--r--   0        0        0    13422 2024-05-05 08:14:27.707219 jiwer-3.0.4/jiwer/process.py
+-rw-r--r--   0        0        0     3670 2024-05-05 08:14:27.707219 jiwer-3.0.4/jiwer/transformations.py
+-rw-r--r--   0        0        0    17834 2024-05-05 08:14:27.707219 jiwer-3.0.4/jiwer/transforms.py
+-rw-r--r--   0        0        0      647 2024-05-05 08:14:27.707219 jiwer-3.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2604 1970-01-01 00:00:00.000000 jiwer-3.0.4/PKG-INFO
```

### Comparing `jiwer-3.0.3/LICENSE` & `jiwer-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jiwer-3.0.3/README.md` & `jiwer-3.0.4/README.md`

 * *Files identical despite different names*

### Comparing `jiwer-3.0.3/jiwer/alignment.py` & `jiwer-3.0.4/jiwer/alignment.py`

 * *Files identical despite different names*

### Comparing `jiwer-3.0.3/jiwer/cli.py` & `jiwer-3.0.4/jiwer/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,40 +92,49 @@
     with hypothesis_file.open("r") as f:
         hypothesis_sentences = [
             ln.strip() for ln in f.readlines() if len(ln.strip()) > 1
         ]
 
     if not global_alignment and len(reference_sentences) != len(hypothesis_sentences):
         raise ValueError(
-            f"Number of sentences does not match. "
-            f"{reference_file} contains {len(reference_sentences)} lines."
-            f"{hypothesis_file} contains {len(hypothesis_sentences)} lines."
+            f"Number of reference sentences "
+            f"({len(reference_sentences)} in '{reference_file}') "
+            f"and hypothesis sentences "
+            f"({len(hypothesis_sentences)} in '{hypothesis_file}') "
+            f"do not match! "
+            f"Use the `--global` flag to compute the measures over a global alignment "
+            f"of the reference and hypothesis sentences."
         )
 
-    if global_alignment and compute_cer:
-        raise ValueError("--global and --cer are mutually exclusive.")
-
     if compute_cer:
-        out = jiwer.process_characters(
-            reference_sentences,
-            hypothesis_sentences,
-        )
+        if global_alignment:
+            out = jiwer.process_characters(
+                reference_sentences,
+                hypothesis_sentences,
+                reference_transform=jiwer.cer_contiguous,
+                hypothesis_transform=jiwer.cer_contiguous,
+            )
+        else:
+            out = jiwer.process_characters(
+                reference_sentences,
+                hypothesis_sentences,
+            )
     else:
         if global_alignment:
             out = jiwer.process_words(
                 reference_sentences,
                 hypothesis_sentences,
                 reference_transform=jiwer.wer_contiguous,
                 hypothesis_transform=jiwer.wer_contiguous,
             )
         else:
             out = jiwer.process_words(reference_sentences, hypothesis_sentences)
 
     if show_alignment:
-        print(jiwer.visualize_alignment(out, show_measures=True))
+        print(jiwer.visualize_alignment(out, show_measures=True), end="")
     else:
         if compute_cer:
             print(out.cer)
         else:
             print(out.wer)
```

### Comparing `jiwer-3.0.3/jiwer/measures.py` & `jiwer-3.0.4/jiwer/measures.py`

 * *Files identical despite different names*

### Comparing `jiwer-3.0.3/jiwer/process.py` & `jiwer-3.0.4/jiwer/process.py`

 * *Files identical despite different names*

### Comparing `jiwer-3.0.3/jiwer/transformations.py` & `jiwer-3.0.4/jiwer/transformations.py`

 * *Files identical despite different names*

### Comparing `jiwer-3.0.3/jiwer/transforms.py` & `jiwer-3.0.4/jiwer/transforms.py`

 * *Files identical despite different names*

### Comparing `jiwer-3.0.3/pyproject.toml` & `jiwer-3.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jiwer"
-version = "3.0.3"
+version = "3.0.4"
 description = "Evaluate your speech-to-text system with similarity measures such as word error rate (WER)"
 authors = ["Nik Vaessen <nikvaes@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 repository = "https://github.com/jitsi/jiwer"
 include = ["LICENCE"]
```

### Comparing `jiwer-3.0.3/PKG-INFO` & `jiwer-3.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: jiwer
-Version: 3.0.3
+Version: 3.0.4
 Summary: Evaluate your speech-to-text system with similarity measures such as word error rate (WER)
 Home-page: https://github.com/jitsi/jiwer
 License: Apache-2.0
 Author: Nik Vaessen
 Author-email: nikvaes@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: rapidfuzz (>=3,<4)
 Project-URL: Repository, https://github.com/jitsi/jiwer
 Description-Content-Type: text/markdown
 
 # JiWER
```

