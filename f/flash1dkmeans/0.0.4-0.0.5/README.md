# Comparing `tmp/flash1dkmeans-0.0.4.tar.gz` & `tmp/flash1dkmeans-0.0.5.tar.gz`

## Comparing `flash1dkmeans-0.0.4.tar` & `flash1dkmeans-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/.idea/.gitignore
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/.idea/flash1dkmeans.iml
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/.idea/misc.xml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/.idea/vcs.xml
--rw-r--r--   0        0        0     9005 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/.idea/workspace.xml
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/src/flash1dkmeans/__init__.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/src/flash1dkmeans/config.py
--rw-r--r--   0        0        0    19117 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/src/flash1dkmeans/k_cluster.py
--rw-r--r--   0        0        0     6861 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/src/flash1dkmeans/main.py
--rw-r--r--   0        0        0     9878 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/src/flash1dkmeans/two_cluster.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/src/flash1dkmeans/utils.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/tests/complex.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/tests/k_cluster.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/tests/two_cluster.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/LICENSE
--rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/README.md
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.5/.idea/.gitignore
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.5/.idea/flash1dkmeans.iml
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.5/.idea/misc.xml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.5/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.5/.idea/vcs.xml
+-rw-r--r--   0        0        0     9005 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.5/.idea/workspace.xml
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.5/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.5/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.5/src/flash1dkmeans/__init__.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.5/src/flash1dkmeans/config.py
+-rw-r--r--   0        0        0    19117 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.5/src/flash1dkmeans/k_cluster.py
+-rw-r--r--   0        0        0     6861 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.5/src/flash1dkmeans/main.py
+-rw-r--r--   0        0        0     9772 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.5/src/flash1dkmeans/two_cluster.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.5/src/flash1dkmeans/utils.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.5/tests/complex.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.5/tests/k_cluster.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.5/tests/two_cluster.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.5/README.md
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.5/PKG-INFO
```

### Comparing `flash1dkmeans-0.0.4/.idea/flash1dkmeans.iml` & `flash1dkmeans-0.0.5/.idea/flash1dkmeans.iml`

 * *Files identical despite different names*

### Comparing `flash1dkmeans-0.0.4/.idea/workspace.xml` & `flash1dkmeans-0.0.5/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `flash1dkmeans-0.0.4/.idea/inspectionProfiles/Project_Default.xml` & `flash1dkmeans-0.0.5/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `flash1dkmeans-0.0.4/src/flash1dkmeans/k_cluster.py` & `flash1dkmeans-0.0.5/src/flash1dkmeans/k_cluster.py`

 * *Files identical despite different names*

### Comparing `flash1dkmeans-0.0.4/src/flash1dkmeans/main.py` & `flash1dkmeans-0.0.5/src/flash1dkmeans/main.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -107,16 +107,16 @@
     if is_weighted:
         sample_weights_casted = sorted_sample_weights.astype(PREFIX_SUM_DTYPE)
         sample_weight_prefix_sum = np.cumsum(sample_weights_casted)
         weighted_X_prefix_sum = np.cumsum(sorted_X_casted * sample_weights_casted)
         if n_clusters == 2:
             centroids, cluster_borders = numba_kmeans_1d_two_cluster(
                 sorted_X=sorted_X,
-                weighted_X_prefix_sum=weighted_X_prefix_sum,
                 weights_prefix_sum=sample_weight_prefix_sum,
+                weighted_X_prefix_sum=weighted_X_prefix_sum,
                 start_idx=0,
                 stop_idx=len(sorted_X),
             )
         else:
             weighted_X_squared_prefix_sum = np.cumsum(sorted_X_casted ** 2 * sample_weights_casted)
             centroids, cluster_borders = numba_kmeans_1d_k_cluster(
                 sorted_X=sorted_X,
```

### Comparing `flash1dkmeans-0.0.4/src/flash1dkmeans/two_cluster.py` & `flash1dkmeans-0.0.5/src/flash1dkmeans/two_cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 from .utils import query_prefix_sum
 from .config import PREFIX_SUM_DTYPE, ARRAY_INDEX_DTYPE
 
 
 @numba.njit(cache=True)
 def numba_kmeans_1d_two_cluster(
         sorted_X,
-        weighted_X_prefix_sum,
         weights_prefix_sum,
+        weighted_X_prefix_sum,
         start_idx,
         stop_idx,
 ):
     """An optimized kmeans for 1D data with 2 clusters, weighted version.
     Utilizes a binary search to find the optimal division point.
     Time complexity: O(log(n))
 
@@ -44,16 +44,14 @@
         centroids: np.ndarray
             The centroids of the two clusters, shape (2,)
         cluster_borders: np.ndarray
             The borders of the two clusters, shape (3,)
 
     WARNING: X should be sorted in ascending order before calling this function.
     """
-    assert weights_prefix_sum is not None, "sample_weight_prefix_sum must be provided for weighted data"
-
     size = stop_idx - start_idx
     centroids = np.empty(2, dtype=sorted_X.dtype)
     cluster_borders = np.empty(3, dtype=ARRAY_INDEX_DTYPE)
     cluster_borders[0] = start_idx
     cluster_borders[2] = stop_idx
     # Remember to set cluster_borders[1] as the division point
```

### Comparing `flash1dkmeans-0.0.4/tests/complex.py` & `flash1dkmeans-0.0.5/tests/complex.py`

 * *Files identical despite different names*

### Comparing `flash1dkmeans-0.0.4/.gitignore` & `flash1dkmeans-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `flash1dkmeans-0.0.4/LICENSE` & `flash1dkmeans-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flash1dkmeans-0.0.4/README.md` & `flash1dkmeans-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `flash1dkmeans-0.0.4/pyproject.toml` & `flash1dkmeans-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "flash1dkmeans"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Jake Hyun", email="jake.hyun@hotmail.com" },
 ]
 description = "An optimized K-means implementation for the one-dimensional case."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `flash1dkmeans-0.0.4/PKG-INFO` & `flash1dkmeans-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: flash1dkmeans
-Version: 0.0.4
+Version: 0.0.5
 Summary: An optimized K-means implementation for the one-dimensional case.
 Project-URL: Homepage, https://github.com/SyphonArch/flash1dkmeans
 Project-URL: Issues, https://github.com/SyphonArch/flash1dkmeans/issues
 Author-email: Jake Hyun <jake.hyun@hotmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

