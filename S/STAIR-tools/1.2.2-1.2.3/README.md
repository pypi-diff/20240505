# Comparing `tmp/STAIR-tools-1.2.2.tar.gz` & `tmp/STAIR-tools-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "STAIR-tools-1.2.2.tar", last modified: Sun May  5 05:48:49 2024, max compression
+gzip compressed data, was "STAIR-tools-1.2.3.tar", last modified: Sun May  5 07:24:47 2024, max compression
```

## Comparing `STAIR-tools-1.2.2.tar` & `STAIR-tools-1.2.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-05 05:48:49.110392 STAIR-tools-1.2.2/
--rw-r--r--   0 yuanyuan   (501) staff       (20)      253 2024-05-05 05:48:49.110134 STAIR-tools-1.2.2/PKG-INFO
--rwxr-xr-x   0 yuanyuan   (501) staff       (20)     1320 2023-12-25 02:00:08.000000 STAIR-tools-1.2.2/README.md
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-05 05:48:49.105486 STAIR-tools-1.2.2/STAIR/
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8661 2023-12-23 11:23:09.000000 STAIR-tools-1.2.2/STAIR/ABA_annotation.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-05 05:48:49.105811 STAIR-tools-1.2.2/STAIR/ABAanno/
--rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.2.2/STAIR/ABAanno/__init__.py
--rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.2.2/STAIR/__init__.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    18517 2024-04-26 11:02:07.000000 STAIR-tools-1.2.2/STAIR/emb_alignment.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-05 05:48:49.107712 STAIR-tools-1.2.2/STAIR/embedding/
--rw-------   0 yuanyuan   (501) staff       (20)      120 2024-04-25 02:41:10.000000 STAIR-tools-1.2.2/STAIR/embedding/__init__.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     3804 2024-05-04 11:27:47.000000 STAIR-tools-1.2.2/STAIR/embedding/dataset_ae.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     3980 2024-05-05 05:48:21.000000 STAIR-tools-1.2.2/STAIR/embedding/dataset_hgat.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)      988 2023-12-23 11:23:12.000000 STAIR-tools-1.2.2/STAIR/embedding/loss.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     5493 2023-12-23 11:23:12.000000 STAIR-tools-1.2.2/STAIR/embedding/module_ae.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8658 2023-12-23 11:23:12.000000 STAIR-tools-1.2.2/STAIR/embedding/module_hgat.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     6954 2023-12-23 11:23:12.000000 STAIR-tools-1.2.2/STAIR/embedding/module_hgat1.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    12320 2024-04-29 06:21:03.000000 STAIR-tools-1.2.2/STAIR/loc_alignment.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    14364 2024-04-28 11:59:13.000000 STAIR-tools-1.2.2/STAIR/loc_prediction.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-05 05:48:49.109344 STAIR-tools-1.2.2/STAIR/location/
--rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.2.2/STAIR/location/__init__.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     7819 2023-12-23 11:23:12.000000 STAIR-tools-1.2.2/STAIR/location/align_fine.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    11236 2023-12-23 11:23:13.000000 STAIR-tools-1.2.2/STAIR/location/align_init.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8534 2023-12-23 11:23:13.000000 STAIR-tools-1.2.2/STAIR/location/edge_detection.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     9354 2023-12-23 11:23:13.000000 STAIR-tools-1.2.2/STAIR/location/edge_detection1.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2298 2023-12-23 11:23:13.000000 STAIR-tools-1.2.2/STAIR/location/transformation.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2821 2023-12-23 11:23:13.000000 STAIR-tools-1.2.2/STAIR/utils.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-05 05:48:49.109939 STAIR-tools-1.2.2/STAIR_tools.egg-info/
--rw-r--r--   0 yuanyuan   (501) staff       (20)      253 2024-05-05 05:48:49.000000 STAIR-tools-1.2.2/STAIR_tools.egg-info/PKG-INFO
--rw-r--r--   0 yuanyuan   (501) staff       (20)      702 2024-05-05 05:48:49.000000 STAIR-tools-1.2.2/STAIR_tools.egg-info/SOURCES.txt
--rw-r--r--   0 yuanyuan   (501) staff       (20)        1 2024-05-05 05:48:49.000000 STAIR-tools-1.2.2/STAIR_tools.egg-info/dependency_links.txt
--rw-r--r--   0 yuanyuan   (501) staff       (20)        6 2024-05-05 05:48:49.000000 STAIR-tools-1.2.2/STAIR_tools.egg-info/top_level.txt
--rw-r--r--   0 yuanyuan   (501) staff       (20)       38 2024-05-05 05:48:49.110442 STAIR-tools-1.2.2/setup.cfg
--rw-------   0 yuanyuan   (501) staff       (20)      489 2024-05-05 05:48:41.000000 STAIR-tools-1.2.2/setup.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-05 07:24:47.221502 STAIR-tools-1.2.3/
+-rw-r--r--   0 yuanyuan   (501) staff       (20)      253 2024-05-05 07:24:47.221194 STAIR-tools-1.2.3/PKG-INFO
+-rwxr-xr-x   0 yuanyuan   (501) staff       (20)     1320 2023-12-25 02:00:08.000000 STAIR-tools-1.2.3/README.md
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-05 07:24:47.216073 STAIR-tools-1.2.3/STAIR/
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8661 2023-12-23 11:23:09.000000 STAIR-tools-1.2.3/STAIR/ABA_annotation.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-05 07:24:47.216379 STAIR-tools-1.2.3/STAIR/ABAanno/
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.2.3/STAIR/ABAanno/__init__.py
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.2.3/STAIR/__init__.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    18519 2024-05-05 07:24:21.000000 STAIR-tools-1.2.3/STAIR/emb_alignment.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-05 07:24:47.218731 STAIR-tools-1.2.3/STAIR/embedding/
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2024-04-25 02:41:10.000000 STAIR-tools-1.2.3/STAIR/embedding/__init__.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     3804 2024-05-04 11:27:47.000000 STAIR-tools-1.2.3/STAIR/embedding/dataset_ae.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     3980 2024-05-05 05:48:21.000000 STAIR-tools-1.2.3/STAIR/embedding/dataset_hgat.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)      988 2023-12-23 11:23:12.000000 STAIR-tools-1.2.3/STAIR/embedding/loss.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     5493 2023-12-23 11:23:12.000000 STAIR-tools-1.2.3/STAIR/embedding/module_ae.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8658 2023-12-23 11:23:12.000000 STAIR-tools-1.2.3/STAIR/embedding/module_hgat.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     6954 2023-12-23 11:23:12.000000 STAIR-tools-1.2.3/STAIR/embedding/module_hgat1.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    12320 2024-04-29 06:21:03.000000 STAIR-tools-1.2.3/STAIR/loc_alignment.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    14364 2024-04-28 11:59:13.000000 STAIR-tools-1.2.3/STAIR/loc_prediction.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-05 07:24:47.220378 STAIR-tools-1.2.3/STAIR/location/
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.2.3/STAIR/location/__init__.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     7819 2023-12-23 11:23:12.000000 STAIR-tools-1.2.3/STAIR/location/align_fine.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    11236 2023-12-23 11:23:13.000000 STAIR-tools-1.2.3/STAIR/location/align_init.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8534 2023-12-23 11:23:13.000000 STAIR-tools-1.2.3/STAIR/location/edge_detection.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     9354 2023-12-23 11:23:13.000000 STAIR-tools-1.2.3/STAIR/location/edge_detection1.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2298 2023-12-23 11:23:13.000000 STAIR-tools-1.2.3/STAIR/location/transformation.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2821 2023-12-23 11:23:13.000000 STAIR-tools-1.2.3/STAIR/utils.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-05 07:24:47.220985 STAIR-tools-1.2.3/STAIR_tools.egg-info/
+-rw-r--r--   0 yuanyuan   (501) staff       (20)      253 2024-05-05 07:24:47.000000 STAIR-tools-1.2.3/STAIR_tools.egg-info/PKG-INFO
+-rw-r--r--   0 yuanyuan   (501) staff       (20)      702 2024-05-05 07:24:47.000000 STAIR-tools-1.2.3/STAIR_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 yuanyuan   (501) staff       (20)        1 2024-05-05 07:24:47.000000 STAIR-tools-1.2.3/STAIR_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 yuanyuan   (501) staff       (20)        6 2024-05-05 07:24:47.000000 STAIR-tools-1.2.3/STAIR_tools.egg-info/top_level.txt
+-rw-r--r--   0 yuanyuan   (501) staff       (20)       38 2024-05-05 07:24:47.221557 STAIR-tools-1.2.3/setup.cfg
+-rw-------   0 yuanyuan   (501) staff       (20)      489 2024-05-05 07:24:43.000000 STAIR-tools-1.2.3/setup.py
```

### Comparing `STAIR-tools-1.2.2/README.md` & `STAIR-tools-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.2/STAIR/ABA_annotation.py` & `STAIR-tools-1.2.3/STAIR/ABA_annotation.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.2/STAIR/emb_alignment.py` & `STAIR-tools-1.2.3/STAIR/emb_alignment.py`

 * *Files 2% similar despite different names*

```diff
@@ -279,15 +279,15 @@
     
     def prepare_hgat(self,
                      slice_key = None,
                      slice_order = None,
                      spatial_key = 'spatial',
                      n_neigh_hom = 10, 
                      c_neigh_het = 0.9,
-                     kernal_thresh = 0.):
+                     kernal_thresh = None):
         '''
         Construct heterogeneous graph for HAT module.
 
         Parameters
         ----------
         slice_key
             Key of slice information in .obs.
```

### Comparing `STAIR-tools-1.2.2/STAIR/embedding/dataset_ae.py` & `STAIR-tools-1.2.3/STAIR/embedding/dataset_ae.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.2/STAIR/embedding/dataset_hgat.py` & `STAIR-tools-1.2.3/STAIR/embedding/dataset_hgat.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.2/STAIR/embedding/loss.py` & `STAIR-tools-1.2.3/STAIR/embedding/loss.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.2/STAIR/embedding/module_ae.py` & `STAIR-tools-1.2.3/STAIR/embedding/module_ae.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.2/STAIR/embedding/module_hgat.py` & `STAIR-tools-1.2.3/STAIR/embedding/module_hgat.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.2/STAIR/embedding/module_hgat1.py` & `STAIR-tools-1.2.3/STAIR/embedding/module_hgat1.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.2/STAIR/loc_alignment.py` & `STAIR-tools-1.2.3/STAIR/loc_alignment.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.2/STAIR/loc_prediction.py` & `STAIR-tools-1.2.3/STAIR/loc_prediction.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.2/STAIR/location/align_fine.py` & `STAIR-tools-1.2.3/STAIR/location/align_fine.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.2/STAIR/location/align_init.py` & `STAIR-tools-1.2.3/STAIR/location/align_init.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.2/STAIR/location/edge_detection.py` & `STAIR-tools-1.2.3/STAIR/location/edge_detection.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.2/STAIR/location/edge_detection1.py` & `STAIR-tools-1.2.3/STAIR/location/edge_detection1.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.2/STAIR/location/transformation.py` & `STAIR-tools-1.2.3/STAIR/location/transformation.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.2/STAIR/utils.py` & `STAIR-tools-1.2.3/STAIR/utils.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.2/STAIR_tools.egg-info/SOURCES.txt` & `STAIR-tools-1.2.3/STAIR_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

