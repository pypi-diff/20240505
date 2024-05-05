# Comparing `tmp/short_transformers-0.1.0.tar.gz` & `tmp/short_transformers-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "short_transformers-0.1.0.tar", max compression
+gzip compressed data, was "short_transformers-0.2.0.tar", max compression
```

## Comparing `short_transformers-0.1.0.tar` & `short_transformers-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     2202 2024-05-04 16:57:36.831925 short_transformers-0.1.0/README.md
--rw-r--r--   0        0        0      379 2024-05-04 08:36:19.137105 short_transformers-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       66 2024-05-04 09:30:34.812687 short_transformers-0.1.0/short_transformers/__init__.py
--rw-r--r--   0        0        0      748 2024-05-04 09:18:55.749638 short_transformers-0.1.0/short_transformers/dist.py
--rw-r--r--   0        0        0      864 2024-05-04 09:18:55.753638 short_transformers-0.1.0/short_transformers/graph.py
--rw-r--r--   0        0        0     6769 2024-05-04 16:49:11.336617 short_transformers-0.1.0/short_transformers/short_transformer.py
--rw-r--r--   0        0        0       95 2024-05-04 16:49:04.016627 short_transformers-0.1.0/short_transformers/utils.py
--rw-r--r--   0        0        0     2814 1970-01-01 00:00:00.000000 short_transformers-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4986 2024-05-04 22:43:54.503553 short_transformers-0.2.0/README.md
+-rw-r--r--   0        0        0      379 2024-05-05 07:31:37.664285 short_transformers-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       98 2024-05-04 22:49:29.887096 short_transformers-0.2.0/short_transformers/__init__.py
+-rw-r--r--   0        0        0      748 2024-05-04 09:18:55.749638 short_transformers-0.2.0/short_transformers/dist.py
+-rw-r--r--   0        0        0      945 2024-05-04 22:49:29.887096 short_transformers-0.2.0/short_transformers/graph.py
+-rw-r--r--   0        0        0      529 2024-05-04 22:49:29.887096 short_transformers-0.2.0/short_transformers/log.py
+-rw-r--r--   0        0        0     8463 2024-05-04 22:50:54.290980 short_transformers-0.2.0/short_transformers/short_transformer.py
+-rw-r--r--   0        0        0       76 2024-05-04 20:32:31.974305 short_transformers-0.2.0/short_transformers/utils.py
+-rw-r--r--   0        0        0     5598 1970-01-01 00:00:00.000000 short_transformers-0.2.0/PKG-INFO
```

### Comparing `short_transformers-0.1.0/short_transformers/dist.py` & `short_transformers-0.2.0/short_transformers/dist.py`

 * *Files identical despite different names*

### Comparing `short_transformers-0.1.0/short_transformers/graph.py` & `short_transformers-0.2.0/short_transformers/graph.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import matplotlib.pylab as plt
 import numpy as np
 import seaborn as sns
 
 
-def draw_diagram(input_file_path, output_file_path):
+def draw_diagram(input_file_path, output_file_path, title=None):
     plt.clf()
 
-    memory = np.load(input_file_path)
-
-    result = memory["result"]
-
+    result = np.load(input_file_path)["arr_0"]
     mask = np.zeros_like(result)
     mask[np.triu_indices_from(mask, k=1)] = True
     mask = np.flip(mask, axis=0)
 
+    # @TODO make row-wise normalization optional
     # rescale scores to 0-1 for each cut_layers value
     masked_result = np.ma.masked_array(result, mask)
     max_dist = np.ma.max(masked_result, axis=1)[:, np.newaxis]
     min_dist = np.ma.min(masked_result, axis=1)[:, np.newaxis]
 
     result = (result - min_dist) / (max_dist - min_dist)
 
     ax = sns.heatmap(result, linewidth=0.5, mask=mask, cmap="viridis_r")
     ax.invert_yaxis()
     ax.set_xticklabels(ax.get_xticklabels(), ha="left")
     ax.set_yticklabels(ax.get_yticklabels(), va="bottom")
 
+    if title:
+        ax.set_title(title)
+
     plt.savefig(output_file_path)
```

