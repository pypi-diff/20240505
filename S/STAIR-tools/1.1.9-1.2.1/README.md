# Comparing `tmp/STAIR-tools-1.1.9.tar.gz` & `tmp/STAIR-tools-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "STAIR-tools-1.1.9.tar", last modified: Sun Apr 28 04:04:36 2024, max compression
+gzip compressed data, was "STAIR-tools-1.2.1.tar", last modified: Sat May  4 11:28:10 2024, max compression
```

## Comparing `STAIR-tools-1.1.9.tar` & `STAIR-tools-1.2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-28 04:04:36.173136 STAIR-tools-1.1.9/
--rw-r--r--   0 yuanyuan   (501) staff       (20)      173 2024-04-28 04:04:36.172929 STAIR-tools-1.1.9/PKG-INFO
--rwxr-xr-x   0 yuanyuan   (501) staff       (20)     1320 2023-12-25 02:00:08.000000 STAIR-tools-1.1.9/README.md
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-28 04:04:36.167302 STAIR-tools-1.1.9/STAIR/
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8661 2023-12-23 11:23:09.000000 STAIR-tools-1.1.9/STAIR/ABA_annotation.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-28 04:04:36.167669 STAIR-tools-1.1.9/STAIR/ABAanno/
--rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.1.9/STAIR/ABAanno/__init__.py
--rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.1.9/STAIR/__init__.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    18517 2024-04-26 11:02:07.000000 STAIR-tools-1.1.9/STAIR/emb_alignment.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-28 04:04:36.170111 STAIR-tools-1.1.9/STAIR/embedding/
--rw-------   0 yuanyuan   (501) staff       (20)      120 2024-04-25 02:41:10.000000 STAIR-tools-1.1.9/STAIR/embedding/__init__.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     3013 2023-12-23 11:23:11.000000 STAIR-tools-1.1.9/STAIR/embedding/dataset_ae.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     3891 2024-04-25 06:09:45.000000 STAIR-tools-1.1.9/STAIR/embedding/dataset_hgat.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)      988 2023-12-23 11:23:12.000000 STAIR-tools-1.1.9/STAIR/embedding/loss.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     5493 2023-12-23 11:23:12.000000 STAIR-tools-1.1.9/STAIR/embedding/module_ae.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8658 2023-12-23 11:23:12.000000 STAIR-tools-1.1.9/STAIR/embedding/module_hgat.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     6954 2023-12-23 11:23:12.000000 STAIR-tools-1.1.9/STAIR/embedding/module_hgat1.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    12324 2024-04-25 02:44:23.000000 STAIR-tools-1.1.9/STAIR/loc_alignment.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    14202 2024-04-25 02:44:36.000000 STAIR-tools-1.1.9/STAIR/loc_prediction.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-28 04:04:36.172025 STAIR-tools-1.1.9/STAIR/location/
--rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.1.9/STAIR/location/__init__.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     7819 2023-12-23 11:23:12.000000 STAIR-tools-1.1.9/STAIR/location/align_fine.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    11236 2023-12-23 11:23:13.000000 STAIR-tools-1.1.9/STAIR/location/align_init.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8534 2023-12-23 11:23:13.000000 STAIR-tools-1.1.9/STAIR/location/edge_detection.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     9354 2023-12-23 11:23:13.000000 STAIR-tools-1.1.9/STAIR/location/edge_detection1.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2298 2023-12-23 11:23:13.000000 STAIR-tools-1.1.9/STAIR/location/transformation.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2821 2023-12-23 11:23:13.000000 STAIR-tools-1.1.9/STAIR/utils.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-28 04:04:36.172719 STAIR-tools-1.1.9/STAIR_tools.egg-info/
--rw-r--r--   0 yuanyuan   (501) staff       (20)      173 2024-04-28 04:04:36.000000 STAIR-tools-1.1.9/STAIR_tools.egg-info/PKG-INFO
--rw-r--r--   0 yuanyuan   (501) staff       (20)      702 2024-04-28 04:04:36.000000 STAIR-tools-1.1.9/STAIR_tools.egg-info/SOURCES.txt
--rw-r--r--   0 yuanyuan   (501) staff       (20)        1 2024-04-28 04:04:36.000000 STAIR-tools-1.1.9/STAIR_tools.egg-info/dependency_links.txt
--rw-r--r--   0 yuanyuan   (501) staff       (20)        6 2024-04-28 04:04:36.000000 STAIR-tools-1.1.9/STAIR_tools.egg-info/top_level.txt
--rw-r--r--   0 yuanyuan   (501) staff       (20)       38 2024-04-28 04:04:36.173186 STAIR-tools-1.1.9/setup.cfg
--rw-------   0 yuanyuan   (501) staff       (20)      426 2024-04-28 04:04:25.000000 STAIR-tools-1.1.9/setup.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-04 11:28:10.265141 STAIR-tools-1.2.1/
+-rw-r--r--   0 yuanyuan   (501) staff       (20)      253 2024-05-04 11:28:10.264854 STAIR-tools-1.2.1/PKG-INFO
+-rwxr-xr-x   0 yuanyuan   (501) staff       (20)     1320 2023-12-25 02:00:08.000000 STAIR-tools-1.2.1/README.md
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-04 11:28:10.260366 STAIR-tools-1.2.1/STAIR/
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8661 2023-12-23 11:23:09.000000 STAIR-tools-1.2.1/STAIR/ABA_annotation.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-04 11:28:10.260594 STAIR-tools-1.2.1/STAIR/ABAanno/
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.2.1/STAIR/ABAanno/__init__.py
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.2.1/STAIR/__init__.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    18517 2024-04-26 11:02:07.000000 STAIR-tools-1.2.1/STAIR/emb_alignment.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-04 11:28:10.262354 STAIR-tools-1.2.1/STAIR/embedding/
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2024-04-25 02:41:10.000000 STAIR-tools-1.2.1/STAIR/embedding/__init__.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     3804 2024-05-04 11:27:47.000000 STAIR-tools-1.2.1/STAIR/embedding/dataset_ae.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     3891 2024-04-25 06:09:45.000000 STAIR-tools-1.2.1/STAIR/embedding/dataset_hgat.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)      988 2023-12-23 11:23:12.000000 STAIR-tools-1.2.1/STAIR/embedding/loss.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     5493 2023-12-23 11:23:12.000000 STAIR-tools-1.2.1/STAIR/embedding/module_ae.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8658 2023-12-23 11:23:12.000000 STAIR-tools-1.2.1/STAIR/embedding/module_hgat.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     6954 2023-12-23 11:23:12.000000 STAIR-tools-1.2.1/STAIR/embedding/module_hgat1.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    12320 2024-04-29 06:21:03.000000 STAIR-tools-1.2.1/STAIR/loc_alignment.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    14364 2024-04-28 11:59:13.000000 STAIR-tools-1.2.1/STAIR/loc_prediction.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-04 11:28:10.264041 STAIR-tools-1.2.1/STAIR/location/
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.2.1/STAIR/location/__init__.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     7819 2023-12-23 11:23:12.000000 STAIR-tools-1.2.1/STAIR/location/align_fine.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    11236 2023-12-23 11:23:13.000000 STAIR-tools-1.2.1/STAIR/location/align_init.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8534 2023-12-23 11:23:13.000000 STAIR-tools-1.2.1/STAIR/location/edge_detection.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     9354 2023-12-23 11:23:13.000000 STAIR-tools-1.2.1/STAIR/location/edge_detection1.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2298 2023-12-23 11:23:13.000000 STAIR-tools-1.2.1/STAIR/location/transformation.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2821 2023-12-23 11:23:13.000000 STAIR-tools-1.2.1/STAIR/utils.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-04 11:28:10.264649 STAIR-tools-1.2.1/STAIR_tools.egg-info/
+-rw-r--r--   0 yuanyuan   (501) staff       (20)      253 2024-05-04 11:28:10.000000 STAIR-tools-1.2.1/STAIR_tools.egg-info/PKG-INFO
+-rw-r--r--   0 yuanyuan   (501) staff       (20)      702 2024-05-04 11:28:10.000000 STAIR-tools-1.2.1/STAIR_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 yuanyuan   (501) staff       (20)        1 2024-05-04 11:28:10.000000 STAIR-tools-1.2.1/STAIR_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 yuanyuan   (501) staff       (20)        6 2024-05-04 11:28:10.000000 STAIR-tools-1.2.1/STAIR_tools.egg-info/top_level.txt
+-rw-r--r--   0 yuanyuan   (501) staff       (20)       38 2024-05-04 11:28:10.265208 STAIR-tools-1.2.1/setup.cfg
+-rw-------   0 yuanyuan   (501) staff       (20)      489 2024-05-04 11:28:04.000000 STAIR-tools-1.2.1/setup.py
```

### Comparing `STAIR-tools-1.1.9/README.md` & `STAIR-tools-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.9/STAIR/ABA_annotation.py` & `STAIR-tools-1.2.1/STAIR/ABA_annotation.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.9/STAIR/emb_alignment.py` & `STAIR-tools-1.2.1/STAIR/emb_alignment.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.9/STAIR/embedding/dataset_hgat.py` & `STAIR-tools-1.2.1/STAIR/embedding/dataset_hgat.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.9/STAIR/embedding/loss.py` & `STAIR-tools-1.2.1/STAIR/embedding/loss.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.9/STAIR/embedding/module_ae.py` & `STAIR-tools-1.2.1/STAIR/embedding/module_ae.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.9/STAIR/embedding/module_hgat.py` & `STAIR-tools-1.2.1/STAIR/embedding/module_hgat.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.9/STAIR/embedding/module_hgat1.py` & `STAIR-tools-1.2.1/STAIR/embedding/module_hgat1.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.9/STAIR/loc_alignment.py` & `STAIR-tools-1.2.1/STAIR/loc_alignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         make_log = True, 
         result_path = '.'
     ):
         super(Loc_Align, self).__init__()
 
         self.batch_key = batch_key
         
-        if batch_order is None:
+        if not batch_order:
             batch_order = list(adata.obs[batch_key].value_counts().sort_index().index)
         
         self.batch_n = len(batch_order)
         self.adata_list = [adata[adata.obs[batch_key]==key].copy() for key in batch_order]
 
         self.make_log = make_log
         self.result_path = result_path
```

### Comparing `STAIR-tools-1.1.9/STAIR/loc_prediction.py` & `STAIR-tools-1.2.1/STAIR/loc_prediction.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from STAIR.location.transformation import best_fit_transform, transform
 from STAIR.location.edge_detection import alpha_shape
 from STAIR.location.align_fine import fine_alignment
 from STAIR.utils import MakeLogClass
 
 
-def sort_slices(atte, return_tree=False):
+def sort_slices(atte, start=None, return_tree=False):
     
     import networkx as nx
     
     matrix = 1 - (atte + atte.T)/2
     keys_use = atte.index.tolist()
 
     G = nx.Graph()
@@ -29,15 +29,20 @@
     minimum_spanning_tree = nx.minimum_spanning_tree(G)
 
     # 输出最小生成树的边
 #     for edge in minimum_spanning_tree.edges(data=True):
 #         print(edge)
 
     result = list(minimum_spanning_tree.edges(data=True))
-    dists = {result[0][0]:0.}
+
+    if start:
+        dists = {start:0.} 
+    else:
+        dists = {result[0][0]:0.} 
+
     un_calcu = []
 
     for edge in minimum_spanning_tree.edges(data=True):
         vert1, vert2, weight = edge
         weight = weight['weight']
         if vert1 in dists.keys() and vert2 in dists.keys():
             pass
@@ -56,20 +61,24 @@
             pass
         elif vert1 in dists.keys():
             dists[vert2] = dists[vert1] + weight
         elif vert2 in dists.keys():
             dists[vert1] = dists[vert2] - weight
         else:
             un_calcu.append(edge)
-
     
+    for key in keys_use:
+        if dists[key] < 0:
+            dists[key] = - dists[key]
+
     if return_tree:
         return dists, minimum_spanning_tree
     return dists
 
+
 def loc_predict_z(adata, 
                   atte, 
                   querys, 
                   loc_key, 
                   batch_key, 
                   knowns = None, 
                   num_mnn = 3):
```

### Comparing `STAIR-tools-1.1.9/STAIR/location/align_fine.py` & `STAIR-tools-1.2.1/STAIR/location/align_fine.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.9/STAIR/location/align_init.py` & `STAIR-tools-1.2.1/STAIR/location/align_init.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.9/STAIR/location/edge_detection.py` & `STAIR-tools-1.2.1/STAIR/location/edge_detection.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.9/STAIR/location/edge_detection1.py` & `STAIR-tools-1.2.1/STAIR/location/edge_detection1.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.9/STAIR/location/transformation.py` & `STAIR-tools-1.2.1/STAIR/location/transformation.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.9/STAIR/utils.py` & `STAIR-tools-1.2.1/STAIR/utils.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.9/STAIR_tools.egg-info/SOURCES.txt` & `STAIR-tools-1.2.1/STAIR_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

