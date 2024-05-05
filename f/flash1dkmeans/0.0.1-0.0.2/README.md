# Comparing `tmp/flash1dkmeans-0.0.1.tar.gz` & `tmp/flash1dkmeans-0.0.2.tar.gz`

## Comparing `flash1dkmeans-0.0.1.tar` & `flash1dkmeans-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.1/.idea/.gitignore
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.1/.idea/flash1dkmeans.iml
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.1/.idea/misc.xml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.1/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.1/.idea/vcs.xml
--rw-r--r--   0        0        0     7327 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.1/.idea/workspace.xml
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.1/src/flash1dkmeans/__init__.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.1/src/flash1dkmeans/config.py
--rw-r--r--   0        0        0    13940 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.1/src/flash1dkmeans/k_cluster.py
--rw-r--r--   0        0        0    12325 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.1/src/flash1dkmeans/main.py
--rw-r--r--   0        0        0     7119 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.1/src/flash1dkmeans/two_cluster.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.1/src/flash1dkmeans/utils.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.1/tests/k_cluster.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.1/tests/two_cluster.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.1/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.1/LICENSE
--rw-r--r--   0        0        0     3467 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.1/README.md
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/.idea/.gitignore
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/.idea/flash1dkmeans.iml
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/.idea/misc.xml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/.idea/vcs.xml
+-rw-r--r--   0        0        0     7327 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/.idea/workspace.xml
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/src/flash1dkmeans/__init__.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/src/flash1dkmeans/config.py
+-rw-r--r--   0        0        0    13791 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/src/flash1dkmeans/k_cluster.py
+-rw-r--r--   0        0        0    12364 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/src/flash1dkmeans/main.py
+-rw-r--r--   0        0        0     7094 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/src/flash1dkmeans/two_cluster.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/src/flash1dkmeans/utils.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/tests/k_cluster.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/tests/two_cluster.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3467 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/README.md
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/PKG-INFO
```

### Comparing `flash1dkmeans-0.0.1/.idea/flash1dkmeans.iml` & `flash1dkmeans-0.0.2/.idea/flash1dkmeans.iml`

 * *Files identical despite different names*

### Comparing `flash1dkmeans-0.0.1/.idea/workspace.xml` & `flash1dkmeans-0.0.2/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `flash1dkmeans-0.0.1/.idea/inspectionProfiles/Project_Default.xml` & `flash1dkmeans-0.0.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `flash1dkmeans-0.0.1/src/flash1dkmeans/k_cluster.py` & `flash1dkmeans-0.0.2/src/flash1dkmeans/k_cluster.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 import numba
 from .utils import query_prefix_sum, query_weights_prefix_sum
 import numpy as np
 from .config import ARRAY_INDEX_DTYPE
 
 
-#@numba.njit(cache=True)
 def flash_1d_kmeans_k_cluster(
         X,
         n_clusters,
         max_iter,
         is_weighted,
         weights_prefix_sum, weighted_X_prefix_sum,
         weighted_X_squared_prefix_sum,
@@ -103,15 +102,14 @@
                 sorted_centroids[i] = X[cluster_start:cluster_end].mean()
             else:
                 sorted_centroids[i] = cluster_weighted_X_sum / cluster_weight_sum
 
     return sorted_centroids, cluster_borders
 
 
-@numba.njit(cache=True)
 def _rand_choice_prefix_sum(arr, prob_prefix_sum, start_idx, stop_idx):
     """Randomly choose an element from arr according to the probability distribution given by prob_prefix_sum
     Time complexity: O(log(n))
 
     Args:
         arr: np.ndarray
             The array to choose from
@@ -134,15 +132,14 @@
 
     # Search for the index of the selector in the prefix sum, and add start_idx to get the index in the original array
     idx = np.searchsorted(prob_prefix_sum[start_idx:stop_idx], adjusted_selector) + start_idx
 
     return arr[idx]
 
 
-#@numba.njit(cache=True)
 def _centroids_to_cluster_borders(X, sorted_centroids, start_idx, stop_idx):
     """Converts the centroids to cluster borders.
     The cluster borders are where the clusters are divided.
     The centroids must be sorted.
 
     Time complexity: O(log(len(X)) * len(centroids))
 
@@ -163,15 +160,14 @@
     cluster_borders = np.empty(len(sorted_centroids) + 1, dtype=ARRAY_INDEX_DTYPE)
     cluster_borders[0] = start_idx
     cluster_borders[-1] = stop_idx
     cluster_borders[1:-1] = np.searchsorted(X[start_idx:stop_idx], midpoints) + start_idx
     return cluster_borders
 
 
-#@numba.njit(cache=True)
 def _calculate_inertia(sorted_centroids, centroid_ranges,
                        is_weighted, weights_prefix_sum, weighted_X_prefix_sum, weighted_X_squared_prefix_sum,
                        stop_idx):
     """Calculates the inertia of the clusters given the centroids.
     The inertia is the sum of the squared distances of each sample to the closest centroid.
     The calculations are done efficiently using prefix sums.
 
@@ -217,15 +213,14 @@
 
         inertia += (cluster_weighted_X_squared_sum - 2 * sorted_centroids[i] * cluster_weighted_X_sum +
                     sorted_centroids[i] ** 2 * cluster_weight_sum)
 
     return inertia
 
 
-#@numba.njit(cache=True)
 def _rand_choice_centroids(X, centroids,
                            is_weighted, weights_prefix_sum, weighted_X_prefix_sum, weighted_X_squared_prefix_sum,
                            sample_size, start_idx, stop_idx):
     """Randomly choose sample_size elements from X, weighted by the distance to the closest centroid.
     The weighted logic is implemented efficiently by utilizing the _calculate_inertia function.
 
     Time complexity: O(sample_size * log(len(X)) * len(centroids))
@@ -275,15 +270,14 @@
             else:
                 ceiling = stop_idx_cand
         results[i] = X[floor - 1]
 
     return results
 
 
-#@numba.njit(cache=True)
 def _kmeans_plusplus(X, n_clusters,
                      is_weighted, weights_prefix_sum, weighted_X_prefix_sum, weighted_X_squared_prefix_sum,
                      n_local_trials, start_idx, stop_idx):
     """An optimized version of the kmeans++ initialization algorithm for 1D data.
     The algorithm is optimized for 1D data and utilizes prefix sums for efficient calculations.
 
     Time complexity: O(n_clusters * log(n_clusters) * log(len(X)) * n_clusters)
```

### Comparing `flash1dkmeans-0.0.1/src/flash1dkmeans/main.py` & `flash1dkmeans-0.0.2/src/flash1dkmeans/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from .k_cluster import flash_1d_kmeans_k_cluster
 from .two_cluster import flash_1d_kmeans_two_cluster
 from .config import LABEL_DTYPE, PREFIX_SUM_DTYPE
 import numpy as np
 import logging
+import numba
 
 
+#@numba.njit
 def kmeans_1d(
         X,
         n_clusters,
         max_iter=300,
         is_sorted=False,
         sample_weights=None,
         n_local_trials=None,
@@ -187,14 +189,15 @@
         if not is_sorted:
             assert sorted_indices is not None, "sorted_indices should be available here"
             labels = labels[np.argsort(sorted_indices)]
 
         return centroids, labels
 
 
+#@numba.njit
 def _sorted_kmeans_1d(
         sorted_X,  # caller should ensure that X is sorted
         n_clusters,  # caller should ensure n_clusters >= 2
         max_iter,  # caller should ensure max_iter >= 0
         is_weighted,
         sample_weights,
         n_local_trials,
```

### Comparing `flash1dkmeans-0.0.1/src/flash1dkmeans/two_cluster.py` & `flash1dkmeans-0.0.2/src/flash1dkmeans/two_cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 import numpy as np
 import numba
 from .utils import query_prefix_sum, query_weights_prefix_sum
 from .config import PREFIX_SUM_DTYPE, ARRAY_INDEX_DTYPE
 
 
-#@numba.njit(cache=True)
 def flash_1d_kmeans_two_cluster(
         X,
         is_weighted,
         weighted_X_prefix_sum,
         sample_weight_prefix_sum,
         start_idx,
         stop_idx,
```

### Comparing `flash1dkmeans-0.0.1/src/flash1dkmeans/utils.py` & `flash1dkmeans-0.0.2/src/flash1dkmeans/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import numba
 
 
-#@numba.njit(cache=True)
 def query_prefix_sum(arr_prefix_sum, start, stop):
     """Returns the sum of elements in the range [start, stop) of arr.
 
     Args:
         arr_prefix_sum: The prefix sum of the array arr.
         start: The start index of the range.
         stop: The stop index of the range.
 
     Returns:
         The sum of elements in the range [start, stop) of arr.
     """
     return arr_prefix_sum[stop - 1] - arr_prefix_sum[start - 1] if start > 0 else arr_prefix_sum[stop - 1]
 
 
-#@numba.njit(cache=True)
 def query_weights_prefix_sum(is_weighted, sample_weights, start, stop):
     """Returns the sum of sample_weights in the range [start, stop).
     If is_weighted is False, simply returns stop - start.
 
     Args:
         is_weighted: bool
             Whether the data is weighted. Unweighted data is equivalent to weights of all 1.
```

### Comparing `flash1dkmeans-0.0.1/.gitignore` & `flash1dkmeans-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `flash1dkmeans-0.0.1/LICENSE` & `flash1dkmeans-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flash1dkmeans-0.0.1/README.md` & `flash1dkmeans-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `flash1dkmeans-0.0.1/pyproject.toml` & `flash1dkmeans-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "flash1dkmeans"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Jake Hyun", email="jake.hyun@hotmail.com" },
 ]
 description = "An optimized K-means implementation for the one-dimensional case."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `flash1dkmeans-0.0.1/PKG-INFO` & `flash1dkmeans-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: flash1dkmeans
-Version: 0.0.1
+Version: 0.0.2
 Summary: An optimized K-means implementation for the one-dimensional case.
 Project-URL: Homepage, https://github.com/SyphonArch/flash1dkmeans
 Project-URL: Issues, https://github.com/SyphonArch/flash1dkmeans/issues
 Author-email: Jake Hyun <jake.hyun@hotmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

