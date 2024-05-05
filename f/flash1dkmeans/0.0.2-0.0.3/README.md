# Comparing `tmp/flash1dkmeans-0.0.2.tar.gz` & `tmp/flash1dkmeans-0.0.3.tar.gz`

## Comparing `flash1dkmeans-0.0.2.tar` & `flash1dkmeans-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/.idea/.gitignore
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/.idea/flash1dkmeans.iml
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/.idea/misc.xml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/.idea/vcs.xml
--rw-r--r--   0        0        0     7327 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/.idea/workspace.xml
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/src/flash1dkmeans/__init__.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/src/flash1dkmeans/config.py
--rw-r--r--   0        0        0    13791 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/src/flash1dkmeans/k_cluster.py
--rw-r--r--   0        0        0    12364 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/src/flash1dkmeans/main.py
--rw-r--r--   0        0        0     7094 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/src/flash1dkmeans/two_cluster.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/src/flash1dkmeans/utils.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/tests/k_cluster.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/tests/two_cluster.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/LICENSE
--rw-r--r--   0        0        0     3467 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/README.md
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/.idea/.gitignore
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/.idea/flash1dkmeans.iml
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/.idea/misc.xml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/.idea/vcs.xml
+-rw-r--r--   0        0        0     7975 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/.idea/workspace.xml
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/src/flash1dkmeans/__init__.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/src/flash1dkmeans/config.py
+-rw-r--r--   0        0        0    18911 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/src/flash1dkmeans/k_cluster.py
+-rw-r--r--   0        0        0     9456 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/src/flash1dkmeans/main.py
+-rw-r--r--   0        0        0     9797 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/src/flash1dkmeans/two_cluster.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/src/flash1dkmeans/utils.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/tests/complex.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/tests/k_cluster.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/tests/two_cluster.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/README.md
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/PKG-INFO
```

### Comparing `flash1dkmeans-0.0.2/.idea/flash1dkmeans.iml` & `flash1dkmeans-0.0.3/.idea/flash1dkmeans.iml`

 * *Files identical despite different names*

### Comparing `flash1dkmeans-0.0.2/.idea/workspace.xml` & `flash1dkmeans-0.0.3/.idea/workspace.xml`

 * *Files 12% similar despite different names*

#### Comparing `flash1dkmeans-0.0.2/.idea/workspace.xml` & `flash1dkmeans-0.0.3/.idea/workspace.xml`

```diff
@@ -1,20 +1,19 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="1ba58836-480f-43dd-9244-0130cb4b0f23" name="Changes" comment="">
-      <change afterPath="$PROJECT_DIR$/tests/k_cluster.py" afterDir="false"/>
-      <change afterPath="$PROJECT_DIR$/tests/two_cluster.py" afterDir="false"/>
+      <change afterPath="$PROJECT_DIR$/tests/complex.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/flash1dkmeans/__init__.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/flash1dkmeans/__init__.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/flash1dkmeans/k_cluster.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/flash1dkmeans/k_cluster.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/flash1dkmeans/main.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/flash1dkmeans/main.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/flash1dkmeans/n_cluster.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/flash1dkmeans/k_cluster.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/flash1dkmeans/two_cluster.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/flash1dkmeans/two_cluster.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/flash1dkmeans/utils.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/flash1dkmeans/utils.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
@@ -79,15 +78,15 @@
       <option name="presentableId" value="Default"/>
       <updated>1714838079481</updated>
       <workItem from="1714838080524" duration="170000"/>
       <workItem from="1714838257640" duration="1013000"/>
       <workItem from="1714888190868" duration="167000"/>
       <workItem from="1714898221385" duration="481000"/>
       <workItem from="1714899699435" duration="2811000"/>
-      <workItem from="1714905466256" duration="19526000"/>
+      <workItem from="1714905466256" duration="28184000"/>
     </task>
     <task id="LOCAL-00001" summary="Drop start_idx and stop_idx">
       <option name="closed" value="true"/>
       <created>1714905994757</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
@@ -129,23 +128,41 @@
       <option name="closed" value="true"/>
       <created>1714922815609</created>
       <option name="number" value="00006"/>
       <option name="presentableId" value="LOCAL-00006"/>
       <option name="project" value="LOCAL"/>
       <updated>1714922815609</updated>
     </task>
-    <option name="localTasksCounter" value="7"/>
+    <task id="LOCAL-00007" summary="Cleanup">
+      <option name="closed" value="true"/>
+      <created>1714925358837</created>
+      <option name="number" value="00007"/>
+      <option name="presentableId" value="LOCAL-00007"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1714925358837</updated>
+    </task>
+    <task id="LOCAL-00008" summary="Drop numba for now">
+      <option name="closed" value="true"/>
+      <created>1714928130547</created>
+      <option name="number" value="00008"/>
+      <option name="presentableId" value="LOCAL-00008"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1714928130547</updated>
+    </task>
+    <option name="localTasksCounter" value="9"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="VcsManagerConfiguration">
     <MESSAGE value="Drop start_idx and stop_idx"/>
     <MESSAGE value="Fix logic and semantics"/>
     <MESSAGE value="Add back start_idx and stop_idx"/>
     <MESSAGE value="Implementation without start_idx and stop_idx"/>
     <MESSAGE value="Add start_idx and stop_idx"/>
     <MESSAGE value="Initial complete implementation"/>
-    <option name="LAST_COMMIT_MESSAGE" value="Initial complete implementation"/>
+    <MESSAGE value="Cleanup"/>
+    <MESSAGE value="Drop numba for now"/>
+    <option name="LAST_COMMIT_MESSAGE" value="Drop numba for now"/>
   </component>
 </project>
```

### Comparing `flash1dkmeans-0.0.2/.idea/inspectionProfiles/Project_Default.xml` & `flash1dkmeans-0.0.3/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `flash1dkmeans-0.0.2/src/flash1dkmeans/k_cluster.py` & `flash1dkmeans-0.0.3/src/flash1dkmeans/k_cluster.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,27 +7,26 @@
 - flash_1d_kmeans_n_cluster
 
 Inputs must be sorted in ascending order, no default values are provided, and no error checking is done.
 This is because this module is intended to be used internally.
 """
 
 import numba
-from .utils import query_prefix_sum, query_weights_prefix_sum
+from .utils import query_prefix_sum
 import numpy as np
 from .config import ARRAY_INDEX_DTYPE
 
 
+@numba.njit(cache=True)
 def flash_1d_kmeans_k_cluster(
         X,
         n_clusters,
         max_iter,
-        is_weighted,
         weights_prefix_sum, weighted_X_prefix_sum,
         weighted_X_squared_prefix_sum,
-        n_local_trials,  # This value is 2 + int(np.log(n_clusters)) in sklearn
         start_idx,
         stop_idx,
 ):
     """An optimized kmeans for 1D data with n clusters.
     Exploits the fact that the data is 1D to optimize the calculations.
     Time complexity: O(n_clusters * log(n_clusters) * log(len(X)) * n_clusters + max_iter * log(len(X)) * n_clusters)
                       = O(k ^ 2 * log(k) * log(n) + max_iter * log(n) * k)
@@ -35,49 +34,42 @@
     Args:
         X: np.ndarray
             The input data. Should be sorted in ascending order.
         n_clusters: int
             The number of clusters to generate
         max_iter: int
             The maximum number of iterations to run
-        is_weighted: bool
-            Whether the data is weighted. If True, the weighted versions of the arrays should be provided.
         weights_prefix_sum: np.ndarray
             The prefix sum of the weights. Should be None if the data is unweighted.
         weighted_X_prefix_sum: np.ndarray
             The prefix sum of the weighted X
         weighted_X_squared_prefix_sum: np.ndarray
             The prefix sum of the weighted X squared
-        n_local_trials: int
-            The number of local trials to run when choosing the next centroid
         start_idx: int
             The start index of the range to consider
         stop_idx: int
             The stop index of the range to consider
 
     Returns:
         centroids: np.ndarray
             The centroids of the clusters
         cluster_borders: np.ndarray
             The borders of the clusters
     """
-    if is_weighted:
-        assert weights_prefix_sum is not None, "weights_prefix_sum must be provided for weighted data"
-    else:
-        assert weights_prefix_sum is None, "weights_prefix_sum must not be provided for unweighted data"
+    assert weights_prefix_sum is not None, "weights_prefix_sum must be provided for weighted data"
 
     cluster_borders = np.empty(n_clusters + 1, dtype=ARRAY_INDEX_DTYPE)
     cluster_borders[0] = start_idx
     cluster_borders[-1] = stop_idx
 
     centroids = _kmeans_plusplus(
-        X, n_clusters, is_weighted,
+        X, n_clusters,
         weights_prefix_sum, weighted_X_prefix_sum,
         weighted_X_squared_prefix_sum,
-        n_local_trials, start_idx, stop_idx,
+        start_idx, stop_idx,
     )
     sorted_centroids = np.sort(centroids)
 
     for _ in range(max_iter):
         new_cluster_borders = _centroids_to_cluster_borders(X, sorted_centroids, start_idx, stop_idx)
 
         if np.array_equal(cluster_borders, new_cluster_borders):
@@ -91,25 +83,79 @@
             if cluster_end < cluster_start:
                 raise ValueError("Cluster end is less than cluster start")
 
             if cluster_start == cluster_end:
                 continue
 
             cluster_weighted_X_sum = query_prefix_sum(weighted_X_prefix_sum, cluster_start, cluster_end)
-            cluster_weight_sum = query_weights_prefix_sum(is_weighted, weights_prefix_sum, cluster_start, cluster_end)
+            cluster_weight_sum = query_prefix_sum(weights_prefix_sum, cluster_start, cluster_end)
+
+            if cluster_weight_sum == 0:
+                # if the sum of the weights is zero, we set the centroid to the mean of the cluster
+                sorted_centroids[i] = X[cluster_start:cluster_end].mean()
+            else:
+                sorted_centroids[i] = cluster_weighted_X_sum / cluster_weight_sum
+
+    return sorted_centroids, cluster_borders
+
+
+@numba.njit(cache=True)
+def flash_1d_kmeans_k_cluster_unweighted(
+        X,
+        n_clusters,
+        max_iter,
+        X_prefix_sum,
+        X_squared_prefix_sum,
+        start_idx,
+        stop_idx,
+):
+    """Unweighted version of flash_1d_kmeans_k_cluster"""
+
+    cluster_borders = np.empty(n_clusters + 1, dtype=ARRAY_INDEX_DTYPE)
+    cluster_borders[0] = start_idx
+    cluster_borders[-1] = stop_idx
+
+    centroids = _kmeans_plusplus_unweighted(
+        X, n_clusters,
+        X_prefix_sum,
+        X_squared_prefix_sum,
+        start_idx, stop_idx,
+    )
+    sorted_centroids = np.sort(centroids)
+
+    for _ in range(max_iter):
+        new_cluster_borders = _centroids_to_cluster_borders(X, sorted_centroids, start_idx, stop_idx)
+
+        if np.array_equal(cluster_borders, new_cluster_borders):
+            break
+
+        cluster_borders[:] = new_cluster_borders
+        for i in range(n_clusters):
+            cluster_start = cluster_borders[i]
+            cluster_end = cluster_borders[i + 1]
+
+            if cluster_end < cluster_start:
+                raise ValueError("Cluster end is less than cluster start")
+
+            if cluster_start == cluster_end:
+                continue
+
+            cluster_weighted_X_sum = query_prefix_sum(X_prefix_sum, cluster_start, cluster_end)
+            cluster_weight_sum = cluster_end - cluster_start
 
             if cluster_weight_sum == 0:
                 # if the sum of the weights is zero, we set the centroid to the mean of the cluster
                 sorted_centroids[i] = X[cluster_start:cluster_end].mean()
             else:
                 sorted_centroids[i] = cluster_weighted_X_sum / cluster_weight_sum
 
     return sorted_centroids, cluster_borders
 
 
+@numba.njit(cache=True)
 def _rand_choice_prefix_sum(arr, prob_prefix_sum, start_idx, stop_idx):
     """Randomly choose an element from arr according to the probability distribution given by prob_prefix_sum
     Time complexity: O(log(n))
 
     Args:
         arr: np.ndarray
             The array to choose from
@@ -132,14 +178,15 @@
 
     # Search for the index of the selector in the prefix sum, and add start_idx to get the index in the original array
     idx = np.searchsorted(prob_prefix_sum[start_idx:stop_idx], adjusted_selector) + start_idx
 
     return arr[idx]
 
 
+@numba.njit(cache=True)
 def _centroids_to_cluster_borders(X, sorted_centroids, start_idx, stop_idx):
     """Converts the centroids to cluster borders.
     The cluster borders are where the clusters are divided.
     The centroids must be sorted.
 
     Time complexity: O(log(len(X)) * len(centroids))
 
@@ -160,30 +207,29 @@
     cluster_borders = np.empty(len(sorted_centroids) + 1, dtype=ARRAY_INDEX_DTYPE)
     cluster_borders[0] = start_idx
     cluster_borders[-1] = stop_idx
     cluster_borders[1:-1] = np.searchsorted(X[start_idx:stop_idx], midpoints) + start_idx
     return cluster_borders
 
 
+@numba.njit(cache=True)
 def _calculate_inertia(sorted_centroids, centroid_ranges,
-                       is_weighted, weights_prefix_sum, weighted_X_prefix_sum, weighted_X_squared_prefix_sum,
+                       weights_prefix_sum, weighted_X_prefix_sum, weighted_X_squared_prefix_sum,
                        stop_idx):
     """Calculates the inertia of the clusters given the centroids.
     The inertia is the sum of the squared distances of each sample to the closest centroid.
     The calculations are done efficiently using prefix sums.
 
     Time complexity: O(len(centroids))
 
     Args:
         sorted_centroids: np.ndarray
             The centroids of the clusters
         centroid_ranges: np.ndarray
             The borders of the clusters
-        is_weighted: bool
-            Whether the data is weighted. If True, the weighted versions of the arrays should be provided.
         weights_prefix_sum: np.ndarray
             The prefix sum of the weights. Should be None if the data is unweighted.
         weighted_X_prefix_sum: np.ndarray
             The prefix sum of the weighted X
         weighted_X_squared_prefix_sum: np.ndarray
             The prefix sum of the weighted X squared
         stop_idx: int
@@ -205,24 +251,58 @@
             end = stop_idx
 
         if start == end:
             continue
 
         cluster_weighted_X_squared_sum = query_prefix_sum(weighted_X_squared_prefix_sum, start, end)
         cluster_weighted_X_sum = query_prefix_sum(weighted_X_prefix_sum, start, end)
-        cluster_weight_sum = query_weights_prefix_sum(is_weighted, weights_prefix_sum, start, end)
+        cluster_weight_sum = query_prefix_sum(weights_prefix_sum, start, end)
+
+        inertia += (cluster_weighted_X_squared_sum - 2 * sorted_centroids[i] * cluster_weighted_X_sum +
+                    sorted_centroids[i] ** 2 * cluster_weight_sum)
+
+    return inertia
+
+
+@numba.njit(cache=True)
+def _calculate_inertia_unweighted(sorted_centroids, centroid_ranges,
+                                  X_prefix_sum, X_squared_prefix_sum,
+                                  stop_idx):
+    """Unweighted version of _calculate_inertia"""
+    # inertia = sigma_i(w_i * abs(x_i - c)^2) = sigma_i(w_i * (x_i^2 - 2 * x_i * c + c^2))
+    #         = sigma_i(w_i * x_i^2) - 2 * c * sigma_i(w_i * x_i) + c^2 * sigma_i(w_i)
+    #         = sigma_i(weighted_X_squared) - 2 * c * sigma_i(weighted_X) + c^2 * sigma_i(weight)
+    #  Note that the centroid c is the CLOSEST centroid to x_i, so the above calculation must be done for each cluster
+
+    inertia = 0
+    for i in range(len(sorted_centroids)):
+        start = centroid_ranges[i]
+        end = centroid_ranges[i + 1]
+
+        if start >= stop_idx:
+            break
+        if end >= stop_idx:
+            end = stop_idx
+
+        if start == end:
+            continue
+
+        cluster_weighted_X_squared_sum = query_prefix_sum(X_squared_prefix_sum, start, end)
+        cluster_weighted_X_sum = query_prefix_sum(X_prefix_sum, start, end)
+        cluster_weight_sum = end - start
 
         inertia += (cluster_weighted_X_squared_sum - 2 * sorted_centroids[i] * cluster_weighted_X_sum +
                     sorted_centroids[i] ** 2 * cluster_weight_sum)
 
     return inertia
 
 
+@numba.njit(cache=True)
 def _rand_choice_centroids(X, centroids,
-                           is_weighted, weights_prefix_sum, weighted_X_prefix_sum, weighted_X_squared_prefix_sum,
+                           weights_prefix_sum, weighted_X_prefix_sum, weighted_X_squared_prefix_sum,
                            sample_size, start_idx, stop_idx):
     """Randomly choose sample_size elements from X, weighted by the distance to the closest centroid.
     The weighted logic is implemented efficiently by utilizing the _calculate_inertia function.
 
     Time complexity: O(sample_size * log(len(X)) * len(centroids))
 
     Args:
@@ -247,89 +327,152 @@
 
     Returns:
         np.ndarray: The chosen samples
     """
     sorted_centroids = np.sort(centroids)
     cluster_borders = _centroids_to_cluster_borders(X, sorted_centroids, start_idx, stop_idx)
     total_inertia = _calculate_inertia(sorted_centroids, cluster_borders,
-                                       is_weighted, weights_prefix_sum, weighted_X_prefix_sum,
+                                       weights_prefix_sum, weighted_X_prefix_sum,
                                        weighted_X_squared_prefix_sum, stop_idx)
     selectors = np.random.random_sample(sample_size) * total_inertia
     results = np.empty(sample_size, dtype=centroids.dtype)
 
     for i in range(sample_size):
         selector = selectors[i]
         floor = start_idx + 1
         ceiling = stop_idx
         while floor < ceiling:
             stop_idx_cand = (floor + ceiling) // 2
             inertia = _calculate_inertia(sorted_centroids, cluster_borders,
-                                         is_weighted, weights_prefix_sum, weighted_X_prefix_sum,
+                                         weights_prefix_sum, weighted_X_prefix_sum,
                                          weighted_X_squared_prefix_sum, stop_idx_cand)
             if inertia < selector:
                 floor = stop_idx_cand + 1
             else:
                 ceiling = stop_idx_cand
         results[i] = X[floor - 1]
 
     return results
 
 
+@numba.njit(cache=True)
+def _rand_choice_centroids_unweighted(X, centroids,
+                                      X_prefix_sum,
+                                      X_squared_prefix_sum,
+                                      sample_size, start_idx, stop_idx):
+    """Unweighted version of _rand_choice_centroids"""
+    sorted_centroids = np.sort(centroids)
+    cluster_borders = _centroids_to_cluster_borders(X, sorted_centroids, start_idx, stop_idx)
+    total_inertia = _calculate_inertia_unweighted(sorted_centroids, cluster_borders,
+                                                  X_prefix_sum, X_squared_prefix_sum, stop_idx)
+    selectors = np.random.random_sample(sample_size) * total_inertia
+    results = np.empty(sample_size, dtype=centroids.dtype)
+
+    for i in range(sample_size):
+        selector = selectors[i]
+        floor = start_idx + 1
+        ceiling = stop_idx
+        while floor < ceiling:
+            stop_idx_cand = (floor + ceiling) // 2
+            inertia = _calculate_inertia_unweighted(sorted_centroids, cluster_borders,
+                                                    X_prefix_sum, X_squared_prefix_sum, stop_idx_cand)
+            if inertia < selector:
+                floor = stop_idx_cand + 1
+            else:
+                ceiling = stop_idx_cand
+        results[i] = X[floor - 1]
+
+    return results
+
+
+@numba.njit(cache=True)
 def _kmeans_plusplus(X, n_clusters,
-                     is_weighted, weights_prefix_sum, weighted_X_prefix_sum, weighted_X_squared_prefix_sum,
-                     n_local_trials, start_idx, stop_idx):
+                     weights_prefix_sum, weighted_X_prefix_sum, weighted_X_squared_prefix_sum,
+                     start_idx, stop_idx):
     """An optimized version of the kmeans++ initialization algorithm for 1D data.
     The algorithm is optimized for 1D data and utilizes prefix sums for efficient calculations.
 
     Time complexity: O(n_clusters * log(n_clusters) * log(len(X)) * n_clusters)
                      = O(k ^ 2 * log(k) * log(n))
 
     Args:
         X: np.ndarray
             The input data
         n_clusters: int
             The number of clusters to choose
-        is_weighted: bool
-            Whether the data is weighted. If True, the weighted versions of the arrays should be provided.
         weights_prefix_sum: np.ndarray
             The prefix sum of the weights. Should be None if the data is unweighted.
         weighted_X_prefix_sum: np.ndarray
             The prefix sum of the weighted X
         weighted_X_squared_prefix_sum: np.ndarray
             The prefix sum of the weighted X squared
 
     Returns:
         np.ndarray: The chosen centroids
     """
     centroids = np.empty(n_clusters, dtype=X.dtype)
+    n_local_trials = 2 + int(np.log(n_clusters))
 
     # First centroid is chosen randomly according to sample_weight
-    if is_weighted:
-        centroids[0] = _rand_choice_prefix_sum(X, weights_prefix_sum, start_idx, stop_idx)
-    else:
-        centroids[0] = X[np.random.randint(start_idx, stop_idx)]
+    centroids[0] = _rand_choice_prefix_sum(X, weights_prefix_sum, start_idx, stop_idx)
 
     for c_id in range(1, n_clusters):
         # Choose the next centroid randomly according to the weighted distances
         # Sample n_local_trials candidates and choose the best one
         centroid_candidates = _rand_choice_centroids(
             X, centroids[:c_id],
-            is_weighted, weights_prefix_sum, weighted_X_prefix_sum,
+            weights_prefix_sum, weighted_X_prefix_sum,
             weighted_X_squared_prefix_sum, n_local_trials,
             start_idx, stop_idx
         )
 
         best_inertia = np.inf
         best_centroid = None
         for i in range(len(centroid_candidates)):
             centroids[c_id] = centroid_candidates[i]
             sorted_centroids = np.sort(centroids[:c_id + 1])
             centroid_ranges = _centroids_to_cluster_borders(X, sorted_centroids, start_idx, stop_idx)
             inertia = _calculate_inertia(sorted_centroids, centroid_ranges,
-                                         is_weighted, weights_prefix_sum, weighted_X_prefix_sum,
+                                         weights_prefix_sum, weighted_X_prefix_sum,
                                          weighted_X_squared_prefix_sum, stop_idx)
             if inertia < best_inertia:
                 best_inertia = inertia
                 best_centroid = centroid_candidates[i]
         centroids[c_id] = best_centroid
 
     return centroids
+
+
+@numba.njit(cache=True)
+def _kmeans_plusplus_unweighted(X, n_clusters,
+                                X_prefix_sum, X_squared_prefix_sum,
+                                start_idx, stop_idx):
+    """Unweighted version of _kmeans_plusplus"""
+    centroids = np.empty(n_clusters, dtype=X.dtype)
+    n_local_trials = 2 + int(np.log(n_clusters))
+
+    # First centroid is chosen randomly according to sample_weight
+    centroids[0] = X[np.random.randint(start_idx, stop_idx)]
+
+    for c_id in range(1, n_clusters):
+        # Choose the next centroid randomly according to the weighted distances
+        # Sample n_local_trials candidates and choose the best one
+        centroid_candidates = _rand_choice_centroids_unweighted(
+            X, centroids[:c_id], X_prefix_sum,
+            X_squared_prefix_sum, n_local_trials,
+            start_idx, stop_idx
+        )
+
+        best_inertia = np.inf
+        best_centroid = None
+        for i in range(len(centroid_candidates)):
+            centroids[c_id] = centroid_candidates[i]
+            sorted_centroids = np.sort(centroids[:c_id + 1])
+            centroid_ranges = _centroids_to_cluster_borders(X, sorted_centroids, start_idx, stop_idx)
+            inertia = _calculate_inertia_unweighted(sorted_centroids, centroid_ranges,
+                                                    X_prefix_sum, X_squared_prefix_sum, stop_idx)
+            if inertia < best_inertia:
+                best_inertia = inertia
+                best_centroid = centroid_candidates[i]
+        centroids[c_id] = best_centroid
+
+    return centroids
```

### Comparing `flash1dkmeans-0.0.2/src/flash1dkmeans/main.py` & `flash1dkmeans-0.0.3/src/flash1dkmeans/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,23 @@
-from .k_cluster import flash_1d_kmeans_k_cluster
-from .two_cluster import flash_1d_kmeans_two_cluster
+from .k_cluster import flash_1d_kmeans_k_cluster, flash_1d_kmeans_k_cluster_unweighted
+from .two_cluster import flash_1d_kmeans_two_cluster, flash_1d_kmeans_two_cluster_unweighted
 from .config import LABEL_DTYPE, PREFIX_SUM_DTYPE
 import numpy as np
 import logging
 import numba
 
 
-#@numba.njit
 def kmeans_1d(
         X,
         n_clusters,
         max_iter=300,
         is_sorted=False,
         sample_weights=None,
         n_local_trials=None,
         return_cluster_borders=False,
-        weights_prefix_sum=None,
-        weighted_X_prefix_sum=None,
-        weighted_X_squared_prefix_sum=None,
-        start_idx=None,
-        stop_idx=None,
 ):
     """An optimized kmeans for 1D data.
     Utilizes a binary search to find the optimal division points for 2 clusters,
     and an optimized kmeans++ initialization for more than 2 clusters.
 
     Exploits the fact that 1D data can be sorted.
 
@@ -46,109 +40,50 @@
         sample_weights: np.ndarray or list or None
             The sample weights. If None, all samples are weighted equally.
         n_local_trials: int
             The number of local trials for kmeans++ initialization. Only relevant for n_clusters > 2.
         return_cluster_borders: bool
             Whether to return the cluster border indices instead of the labels.
 
-        In the case of repeatedly calling kmeans on different ranges of the same data, the following arguments
-        can be provided to avoid redundant calculations. Make sure that the data is sorted if these are provided.
-
-        weights_prefix_sum: np.ndarray or list or None
-            The prefix sum of the sample weights. Should be None if the data is unweighted.
-        weighted_X_prefix_sum: np.ndarray or list or None
-            The prefix sum of (the weighted) X.
-        weighted_X_squared_prefix_sum: np.ndarray or list or None
-            The prefix sum of (weighted) X squared.
-        start_idx: int
-            The start index of the range to consider.
-        stop_idx: int
-            The stop index of the range to consider.
-
     Returns:
         centroids: np.ndarray
             The centroids of the clusters.
         labels: np.ndarray
             The labels of the samples. Only returned if return_cluster_borders is False.
         cluster_borders: np.ndarray
             The borders of the clusters. Only returned if return_cluster_borders is True.
     """
     # -------------- Input validation --------------
-    if weighted_X_prefix_sum is not None:
-        assert weighted_X_squared_prefix_sum is not None, \
-            "If weighted_X_prefix_sum is provided, weighted_X_squared_prefix_sum should also be provided."
-        # Note that weights_prefix_sum may be None if the data is unweighted
-
-    # Check if user provided both sample_weights and weights_prefix_sum
-    if sample_weights is not None and weights_prefix_sum is not None:
-        raise ValueError("Both sample_weights and weights_prefix_sum cannot be provided. Please provide only one.")
-
     # Check if data is weighted
-    if sample_weights is not None or weights_prefix_sum is not None:
+    if sample_weights is not None:
         is_weighted = True
     else:
         is_weighted = False
 
-    # Check that data is sorted if weighted_X_prefix_sum is provided
-    if weighted_X_prefix_sum is not None and not is_sorted:
-        raise ValueError("The data must be sorted if weighted_X_prefix_sum is provided.")
-
     # Check if all lengths are the same
     if sample_weights is not None:
         assert len(X) == len(sample_weights), "X and sample_weights must have the same length"
-    if weights_prefix_sum is not None:
-        assert len(X) == len(weights_prefix_sum), "X and weights_prefix_sum must have the same length"
-    if weighted_X_prefix_sum is not None:
-        assert len(X) == len(weighted_X_prefix_sum), "X and weighted_X_prefix_sum must have the same length"
-    if weighted_X_squared_prefix_sum is not None:
-        assert len(X) == len(weighted_X_squared_prefix_sum), \
-            "X and weighted_X_squared_prefix_sum must have the same length"
 
     # Check that return_cluster_borders is called with is_sorted=True, warn the user otherwise
     if return_cluster_borders:  # User requested cluster borders
         if not is_sorted:  # However, the user did not provide sorted data
             logging.warning(  # Warn the user that the data will be sorted
                 "The returned cluster borders will be indexed in the sorted order of X, not the original order.")
 
-    # Check if start_idx and stop_idx are given with sorted data
-    if not is_sorted:
-        assert start_idx is None and stop_idx is None, "start_idx and stop_idx are only valid if the data is sorted."
-
     # Check some values
     assert n_clusters >= 2, "n_clusters must be at least 2"
     assert max_iter >= 0, "max_iter must be non-negative"
     assert n_local_trials is None or n_local_trials > 0, "n_local_trials must be positive"
 
     # -------------- Convert all arrays to numpy arrays --------------
     X = np.asarray(X)
 
     if sample_weights is not None:
         sample_weights = np.asarray(sample_weights)
 
-    if weights_prefix_sum is not None:
-        weights_prefix_sum = np.asarray(weights_prefix_sum)
-
-    if weighted_X_prefix_sum is not None:
-        weighted_X_prefix_sum = np.asarray(weighted_X_prefix_sum)
-
-    if weighted_X_squared_prefix_sum is not None:
-        weighted_X_squared_prefix_sum = np.asarray(weighted_X_squared_prefix_sum)
-
-    # -------------- Setting up defaults --------------
-
-    if start_idx is None:
-        start_idx = 0
-    if stop_idx is None:
-        stop_idx = len(X)
-
-    assert 0 <= start_idx < stop_idx <= len(X), "Invalid start_idx and stop_idx"
-
-    if n_local_trials is None:
-        n_local_trials = 2 + int(np.log(n_clusters))
-
     # -------------- Sorting --------------
 
     # Sort the data if it is not already sorted
     # Note that we checked that start_idx and stop_idx are not given if the data is not sorted
     if not is_sorted:
         sorted_indices = np.argsort(X)
         sorted_X = X[sorted_indices]
@@ -156,27 +91,27 @@
     else:
         sorted_indices = None
         sorted_X = X
         sorted_sample_weights = sample_weights
 
     # -------------- Main algorithm --------------
 
-    centroids, cluster_borders = _sorted_kmeans_1d(
-        sorted_X,
-        n_clusters,
-        max_iter,
-        is_weighted,
-        sorted_sample_weights,
-        n_local_trials,
-        weights_prefix_sum,
-        weighted_X_prefix_sum,
-        weighted_X_squared_prefix_sum,
-        start_idx,
-        stop_idx,
-    )
+    if is_weighted:
+        centroids, cluster_borders = _sorted_kmeans_1d(
+            sorted_X,
+            n_clusters,
+            max_iter,
+            sorted_sample_weights,
+        )
+    else:
+        centroids, cluster_borders = _sorted_kmeans_1d_unweighted(
+            sorted_X,
+            n_clusters,
+            max_iter,
+        )
 
     # -------------- Post-processing --------------
 
     if return_cluster_borders:
         # We checked that the data is sorted if cluster borders are requested, so no post-processing is needed
         return centroids, cluster_borders
     else:
@@ -189,27 +124,77 @@
         if not is_sorted:
             assert sorted_indices is not None, "sorted_indices should be available here"
             labels = labels[np.argsort(sorted_indices)]
 
         return centroids, labels
 
 
-#@numba.njit
+@numba.njit(cache=True)
 def _sorted_kmeans_1d(
+        sorted_X,
+        n_clusters,
+        max_iter,
+        sample_weights,
+):
+    """Create the prefix sums and call the main algorithm, for weighted data"""
+    sample_weights_casted = sample_weights.astype(PREFIX_SUM_DTYPE)
+    weights_prefix_sum = np.cumsum(sample_weights_casted)
+
+    sorted_X_casted = sorted_X.astype(PREFIX_SUM_DTYPE)
+    weighted_X_prefix_sum = np.cumsum(sorted_X_casted * sample_weights_casted)
+    weighted_X_squared_prefix_sum = np.cumsum(sorted_X_casted ** 2 * sample_weights_casted)
+
+    centroids, cluster_borders = _sorted_kmeans_1d_prefix_sums(
+        sorted_X,
+        n_clusters,
+        max_iter,
+        weights_prefix_sum,
+        weighted_X_prefix_sum,
+        weighted_X_squared_prefix_sum,
+        start_idx=0,
+        stop_idx=len(sorted_X),
+    )
+
+    return centroids, cluster_borders
+
+
+@numba.njit(cache=True)
+def _sorted_kmeans_1d_unweighted(
+        sorted_X,
+        n_clusters,
+        max_iter,
+):
+    """Create the prefix sums and call the main algorithm, for unweighted data"""
+    X_casted = sorted_X.astype(PREFIX_SUM_DTYPE)
+    X_prefix_sum = np.cumsum(X_casted)
+    X_squared_prefix_sum = np.cumsum(X_casted ** 2)
+
+    centroids, cluster_borders = _sorted_kmeans_1d_prefix_sums_unweighted(
+        sorted_X,
+        n_clusters,
+        max_iter,
+        X_prefix_sum,
+        X_squared_prefix_sum,
+        start_idx=0,
+        stop_idx=len(sorted_X),
+    )
+
+    return centroids, cluster_borders
+
+
+@numba.njit(cache=True)
+def _sorted_kmeans_1d_prefix_sums(
         sorted_X,  # caller should ensure that X is sorted
         n_clusters,  # caller should ensure n_clusters >= 2
         max_iter,  # caller should ensure max_iter >= 0
-        is_weighted,
-        sample_weights,
-        n_local_trials,
         weights_prefix_sum,
         weighted_X_prefix_sum,
         weighted_X_squared_prefix_sum,
-        start_idx,  # caller should ensure 0 <= start_idx < stop_idx <= len(X)
-        stop_idx,  # caller should ensure 0 <= start_idx < stop_idx <= len(X)
+        start_idx=None,
+        stop_idx=None,
 ):
     """The main algorithm for flash_1d_kmeans.
     This function assumes that the input data is sorted, and all input is assumed to be valid.
 
     Time complexity:
         2 clusters:
             O(log(n)) (+ (O(n) for prefix sum calculation if not provided))
@@ -220,84 +205,78 @@
     Args:
         sorted_X: np.ndarray
             The input data. Should be sorted in ascending order.
         n_clusters: int
             The number of clusters.
         max_iter: int
             The maximum number of iterations.
-        is_weighted: bool
-            Whether the data is weighted.
-        sample_weights: np.ndarray or list or None
-            The sample weights.
-        n_local_trials: int
-            The number of local trials for kmeans++ initialization.
-        weights_prefix_sum: np.ndarray or list or None
+        weights_prefix_sum: np.ndarray
             The prefix sum of the sample weights.
-        weighted_X_prefix_sum: np.ndarray or list or None
-            The prefix sum of (the weighted) X.
-        weighted_X_squared_prefix_sum: np.ndarray or list or None
-            The prefix sum of (the squared weighted) X.
+        weighted_X_prefix_sum: np.ndarray
+            The prefix sum of X, weighted by the sample weights.
+        weighted_X_squared_prefix_sum: np.ndarray
+            The prefix sum of X squared, weighted by the sample weights.
         start_idx: int
             The start index of the range to consider.
         stop_idx: int
             The stop index of the range to consider.
 
     Returns:
         centroids: np.ndarray
             The centroids of the clusters.
         cluster_borders: np.ndarray
             The borders of the clusters.
     """
+
     if n_clusters == 2:
-        # If weighted_X_prefix_sum is not provided, neither is weights_prefix_sum (checked by the caller)
-        # They will be generated from sample_weights if needed
-        if weighted_X_prefix_sum is None:
-            sorted_X_casted = sorted_X.astype(PREFIX_SUM_DTYPE)
-            if is_weighted:
-                weights_casted = sample_weights.astype(PREFIX_SUM_DTYPE)
-                weights_prefix_sum = np.cumsum(weights_casted)
-
-                weighted_X_prefix_sum = np.cumsum(sorted_X_casted * weights_casted)
-            else:
-                weights_prefix_sum = None  # weights_prefix_sum is not needed
-                weighted_X_prefix_sum = np.cumsum(sorted_X_casted)  # no weighting needed
-        else:
-            pass  # weighted_X_prefix_sum and weights_prefix_sum are already provided
         centroids, cluster_borders = flash_1d_kmeans_two_cluster(
             sorted_X,
-            is_weighted,
             weighted_X_prefix_sum,
             weights_prefix_sum,
             start_idx,
             stop_idx,
         )
     else:
-        # If weighted_X_prefix_sum is not provided, neither is weights_prefix_sum and weighted_X_squared_prefix_sum
-        # They will be generated from sample_weights if needed
-        if weighted_X_prefix_sum is None:
-            sorted_X_casted = sorted_X.astype(PREFIX_SUM_DTYPE)
-            if is_weighted:
-                weights_casted = sample_weights.astype(PREFIX_SUM_DTYPE)
-                weights_prefix_sum = np.cumsum(weights_casted)
-
-                weighted_X_casted = sorted_X_casted * weights_casted
-                weighted_X_prefix_sum = np.cumsum(weighted_X_casted)
-                weighted_X_squared_prefix_sum = np.cumsum(weighted_X_casted * sorted_X_casted)
-            else:
-                weights_prefix_sum = None  # weights_prefix_sum is not needed
-                weighted_X_prefix_sum = np.cumsum(sorted_X_casted)
-                weighted_X_squared_prefix_sum = np.cumsum(sorted_X_casted ** 2)
-
         centroids, cluster_borders = flash_1d_kmeans_k_cluster(
             sorted_X,
             n_clusters,
             max_iter,
-            is_weighted,
             weights_prefix_sum,
             weighted_X_prefix_sum,
             weighted_X_squared_prefix_sum,
-            n_local_trials,
+            start_idx,
+            stop_idx,
+        )
+
+    return centroids, cluster_borders
+
+
+@numba.njit(cache=True)
+def _sorted_kmeans_1d_prefix_sums_unweighted(
+        sorted_X,
+        n_clusters,
+        max_iter,
+        X_prefix_sum,
+        X_squared_prefix_sum,
+        start_idx,
+        stop_idx,
+):
+    """The unweighted version of _sorted_kmeans_1d_prefix_sums"""
+    if n_clusters == 2:
+        centroids, cluster_borders = flash_1d_kmeans_two_cluster_unweighted(
+            sorted_X,
+            X_prefix_sum,
+            start_idx,
+            stop_idx,
+        )
+    else:
+        centroids, cluster_borders = flash_1d_kmeans_k_cluster_unweighted(
+            sorted_X,
+            n_clusters,
+            max_iter,
+            X_prefix_sum,
+            X_squared_prefix_sum,
             start_idx,
             stop_idx,
         )
 
     return centroids, cluster_borders
```

### Comparing `flash1dkmeans-0.0.2/src/flash1dkmeans/two_cluster.py` & `flash1dkmeans-0.0.3/src/flash1dkmeans/two_cluster.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,35 +8,33 @@
 
 Inputs must be sorted in ascending order, no default values are provided, and no error checking is done.
 This is because this module is intended to be used internally.
 """
 
 import numpy as np
 import numba
-from .utils import query_prefix_sum, query_weights_prefix_sum
+from .utils import query_prefix_sum
 from .config import PREFIX_SUM_DTYPE, ARRAY_INDEX_DTYPE
 
 
+@numba.njit(cache=True)
 def flash_1d_kmeans_two_cluster(
         X,
-        is_weighted,
         weighted_X_prefix_sum,
         sample_weight_prefix_sum,
         start_idx,
         stop_idx,
 ):
-    """An optimized kmeans for 1D data with 2 clusters.
+    """An optimized kmeans for 1D data with 2 clusters, weighted version.
     Utilizes a binary search to find the optimal division point.
     Time complexity: O(log(n))
 
     Args:
         X: np.ndarray
             The input data. Should be sorted in ascending order.
-        is_weighted: bool
-            Whether the data is weighted. If True, the weighted versions of the arrays should be provided.
         weighted_X_prefix_sum: np.ndarray
             The prefix sum of (the weighted) X.
         sample_weight_prefix_sum: np.ndarray
             The prefix sum of the sample weights. Should be None if the data is unweighted.
         start_idx: int
             The start index of the range to consider.
         stop_idx: int
@@ -46,18 +44,15 @@
         centroids: np.ndarray
             The centroids of the two clusters, shape (2,)
         cluster_borders: np.ndarray
             The borders of the two clusters, shape (3,)
 
     WARNING: X should be sorted in ascending order before calling this function.
     """
-    if is_weighted:
-        assert sample_weight_prefix_sum is not None, "sample_weight_prefix_sum must be provided for weighted data"
-    else:
-        assert sample_weight_prefix_sum is None, "sample_weight_prefix_sum must not be provided for unweighted data"
+    assert sample_weight_prefix_sum is not None, "sample_weight_prefix_sum must be provided for weighted data"
 
     size = stop_idx - start_idx
     centroids = np.empty(2, dtype=X.dtype)
     cluster_borders = np.empty(3, dtype=ARRAY_INDEX_DTYPE)
     cluster_borders[0] = start_idx
     cluster_borders[2] = stop_idx
     # Remember to set cluster_borders[1] as the division point
@@ -70,37 +65,36 @@
     if size == 2:
         centroids[0], centroids[1] = X[start_idx], X[start_idx + 1]
         cluster_borders[1] = start_idx + 1
         return centroids, cluster_borders
 
     # Now we know that there are at least 3 elements
 
-    if is_weighted:
-        # If the sum of the sample weight in the range is 0, we assume that the data is unweighted
-        if query_weights_prefix_sum(True, sample_weight_prefix_sum, start_idx, stop_idx) == 0:
-            is_weighted = False
-            # We need to recalculate the prefix sum, as previously it would have been all zeros
-            weighted_X_prefix_sum = np.cumsum(X, dtype=PREFIX_SUM_DTYPE)
-            sample_weight_prefix_sum = None
-        else:
-            # Check if there is only one nonzero sample weight
-            total_weight = query_weights_prefix_sum(True, sample_weight_prefix_sum, start_idx, stop_idx)
-            sample_weight_prefix_sum_within_range = sample_weight_prefix_sum[start_idx:stop_idx]
-            final_increase_idx = np.searchsorted(sample_weight_prefix_sum_within_range,
-                                                 sample_weight_prefix_sum_within_range[-1])
-            final_increase_amount = query_weights_prefix_sum(True, sample_weight_prefix_sum,
-                                                             start_idx + final_increase_idx,
-                                                             start_idx + final_increase_idx + 1)
-            if total_weight == final_increase_amount:
-                # If there is only one nonzero sample weight, we need to return the corresponding weight as the centroid
-                # and set all elements to the left cluster
-                nonzero_weight_index = start_idx + final_increase_idx
-                centroids[0], centroids[1] = X[nonzero_weight_index], X[nonzero_weight_index]
-                cluster_borders[1] = stop_idx
-                return centroids, cluster_borders
+    # If the sum of the sample weight in the range is 0, we assume that the data is unweighted
+    if query_prefix_sum(sample_weight_prefix_sum, start_idx, stop_idx) == 0:
+        # We need to recalculate the prefix sum, as previously it would have been all zeros
+        X_casted = X.astype(PREFIX_SUM_DTYPE)
+        X_prefix_sum = np.cumsum(X_casted)
+        return flash_1d_kmeans_two_cluster_unweighted(X, X_prefix_sum, start_idx, stop_idx)
+    else:
+        # Check if there is only one nonzero sample weight
+        total_weight = query_prefix_sum(sample_weight_prefix_sum, start_idx, stop_idx)
+        sample_weight_prefix_sum_within_range = sample_weight_prefix_sum[start_idx:stop_idx]
+        final_increase_idx = np.searchsorted(sample_weight_prefix_sum_within_range,
+                                             sample_weight_prefix_sum_within_range[-1])
+        final_increase_amount = query_prefix_sum(sample_weight_prefix_sum,
+                                                 start_idx + final_increase_idx,
+                                                 start_idx + final_increase_idx + 1)
+        if total_weight == final_increase_amount:
+            # If there is only one nonzero sample weight, we need to return the corresponding weight as the centroid
+            # and set all elements to the left cluster
+            nonzero_weight_index = start_idx + final_increase_idx
+            centroids[0], centroids[1] = X[nonzero_weight_index], X[nonzero_weight_index]
+            cluster_borders[1] = stop_idx
+            return centroids, cluster_borders
 
     # Now we know that there are at least 3 elements and at least 2 nonzero weights
 
     # KMeans with 2 clusters on 1D data is equivalent to finding a division point.
     # The division point can be found by doing a binary search on the prefix sum.
 
     # We will do a search for the division point,
@@ -111,19 +105,19 @@
     left_centroid = None
     right_centroid = None
     division_point = None
 
     while floor + 1 < ceiling:
         division_point = (floor + ceiling) // 2
         # If the left cluster has no weight, we need to move the floor up
-        left_weight_sum = query_weights_prefix_sum(is_weighted, sample_weight_prefix_sum, start_idx, division_point)
+        left_weight_sum = query_prefix_sum(sample_weight_prefix_sum, start_idx, division_point)
         if left_weight_sum == 0:
             floor = division_point
             continue
-        right_weight_sum = query_weights_prefix_sum(is_weighted, sample_weight_prefix_sum, division_point, stop_idx)
+        right_weight_sum = query_prefix_sum(sample_weight_prefix_sum, division_point, stop_idx)
         # If the right cluster has no weight, we need to move the ceiling down
         if right_weight_sum == 0:
             ceiling = division_point
             continue
 
         left_centroid = query_prefix_sum(weighted_X_prefix_sum, start_idx, division_point) / left_weight_sum
         right_centroid = query_prefix_sum(weighted_X_prefix_sum, division_point, stop_idx) / right_weight_sum
@@ -138,19 +132,100 @@
         else:
             ceiling = division_point
 
     # initialize variables in case the loop above does not run through
     if left_centroid is None:
         division_point = (floor + ceiling) // 2
         left_centroid = (query_prefix_sum(weighted_X_prefix_sum, start_idx, division_point) /
-                         query_weights_prefix_sum(is_weighted, sample_weight_prefix_sum, start_idx, division_point))
+                         query_prefix_sum(sample_weight_prefix_sum, start_idx, division_point))
     if right_centroid is None:
         division_point = (floor + ceiling) // 2
         right_centroid = (query_prefix_sum(weighted_X_prefix_sum, division_point, stop_idx) /
-                          query_weights_prefix_sum(is_weighted, sample_weight_prefix_sum, division_point, stop_idx))
+                          query_prefix_sum(sample_weight_prefix_sum, division_point, stop_idx))
+
+    # avoid using lists to allow numba.njit
+    centroids[0] = left_centroid
+    centroids[1] = right_centroid
+
+    cluster_borders[1] = division_point
+    return centroids, cluster_borders
+
+
+@numba.njit(cache=True)
+def flash_1d_kmeans_two_cluster_unweighted(
+        X,
+        X_prefix_sum,
+        start_idx,
+        stop_idx,
+):
+    """Unweighted version of flash_1d_kmeans_two_cluster."""
+    size = stop_idx - start_idx
+    centroids = np.empty(2, dtype=X.dtype)
+    cluster_borders = np.empty(3, dtype=ARRAY_INDEX_DTYPE)
+    cluster_borders[0] = start_idx
+    cluster_borders[2] = stop_idx
+    # Remember to set cluster_borders[1] as the division point
+
+    if size == 1:
+        centroids[0], centroids[1] = X[start_idx], X[start_idx]
+        cluster_borders[1] = start_idx + 1
+        return centroids, cluster_borders
+
+    if size == 2:
+        centroids[0], centroids[1] = X[start_idx], X[start_idx + 1]
+        cluster_borders[1] = start_idx + 1
+        return centroids, cluster_borders
+
+    # Now we know that there are at least 3 elements and at least 2 nonzero weights
+
+    # KMeans with 2 clusters on 1D data is equivalent to finding a division point.
+    # The division point can be found by doing a binary search on the prefix sum.
+
+    # We will do a search for the division point,
+    # where we search for the optimum number of elements in the first cluster
+    # We don't want empty clusters, so we set the floor and ceiling to start_idx + 1 and stop_idx - 1
+    floor = start_idx + 1
+    ceiling = stop_idx - 1
+    left_centroid = None
+    right_centroid = None
+    division_point = None
+
+    while floor + 1 < ceiling:
+        division_point = (floor + ceiling) // 2
+        # If the left cluster has no weight, we need to move the floor up
+        left_weight_sum = division_point - start_idx
+        if left_weight_sum == 0:
+            floor = division_point
+            continue
+        right_weight_sum = stop_idx - division_point
+        # If the right cluster has no weight, we need to move the ceiling down
+        if right_weight_sum == 0:
+            ceiling = division_point
+            continue
+
+        left_centroid = query_prefix_sum(X_prefix_sum, start_idx, division_point) / left_weight_sum
+        right_centroid = query_prefix_sum(X_prefix_sum, division_point, stop_idx) / right_weight_sum
+
+        new_division_point_value = (left_centroid + right_centroid) / 2
+        if X[division_point - 1] <= new_division_point_value:
+            if new_division_point_value <= X[division_point]:
+                # The new division point matches the previous one, so we can stop
+                break
+            else:
+                floor = division_point
+        else:
+            ceiling = division_point
+
+    # initialize variables in case the loop above does not run through
+    if left_centroid is None:
+        division_point = (floor + ceiling) // 2
+        left_centroid = query_prefix_sum(X_prefix_sum, start_idx, division_point) / (division_point - start_idx)
+    if right_centroid is None:
+        division_point = (floor + ceiling) // 2
+        right_centroid = query_prefix_sum(X_prefix_sum, division_point, stop_idx) / (stop_idx - division_point)
 
     # avoid using lists to allow numba.njit
     centroids[0] = left_centroid
     centroids[1] = right_centroid
 
     cluster_borders[1] = division_point
     return centroids, cluster_borders
```

### Comparing `flash1dkmeans-0.0.2/.gitignore` & `flash1dkmeans-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `flash1dkmeans-0.0.2/LICENSE` & `flash1dkmeans-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flash1dkmeans-0.0.2/README.md` & `flash1dkmeans-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # flash1dkmeans
 An optimized K-means implementation for the one-dimensional case
 
 Exploits the fact that one-dimensional data can be sorted.
 
-Numba acceleration is used, so callers can further use parallelization with Numba's `@njit(parallel=True)`
+For functions prefixed with `_`, Numba acceleration is used, so callers can further use parallelization with Numba's `@njit(parallel=True)`
 if multiple instances of the algorithm are run in parallel.
 
 ## Features
 
 ### Two clusters
 
 Guaranteed to find the optimal solution for two clusters.
@@ -57,22 +57,22 @@
 data = np.array([1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0, 8.0, 9.0, 10.0])
 weights = np.random.random_sample(data.shape)
 k = 3
 
 centroids, labels = kmeans_1d(
     data, k,
     sample_weights=weights,  # sample weights
-    n_local_trials=(2 + int(np.log(k))),  # number of local tries
     max_iter=100,  # maximum number of iterations
 )
 ```
 
 ### Even More Options
+The underlying Numba-accelerated function `_sorted_kmeans_1d` can be used directly for more control.
 ```python
-from flash1dkmeans import kmeans_1d
+from flash1dkmeans import _sorted_kmeans_1d_prefix_sums
 import numpy as np
 
 n, k = 1024, 4
 
 # Generate random data
 data = np.random.random_sample(n)
 data = np.sort(data)
@@ -86,27 +86,28 @@
 weighted_X_squared_prefix_sum = np.cumsum(data ** 2 * weights)
 
 middle_idx = n // 2
 
 # Providing prefix sums reduces redundant calculations
 # This is useful when the algorithm is run multiple times on different segments of the data
 for start_idx, stop_idx in [(0, middle_idx), (middle_idx, n)]:
-  centroids, cluster_borders = kmeans_1d(
-      data, k,  # Note how the sample weights are not provided when the prefix sums are provided
-      n_local_trials=(2 + int(np.log(k))),  # number of local tries
-      max_iter=100,  # maximum number of iterations
-      return_cluster_borders=True,  # return cluster borders instead of labels
-      weights_prefix_sum=weights_prefix_sum,  # prefix sum of the sample weights, leave empty for unwieghted data
-      weighted_X_prefix_sum=weighted_X_prefix_sum,  # prefix sum of the weighted data
-      weighted_X_squared_prefix_sum=weighted_X_squared_prefix_sum,  # prefix sum of the squared weighted data
-      start_idx=start_idx,  # start index of the data
-      stop_idx=stop_idx,  # stop index of the data
-  )
+    centroids, cluster_borders = _sorted_kmeans_1d_prefix_sums(
+        data, k,  # Note how the sample weights are not provided when the prefix sums are provided
+        max_iter=100,  # maximum number of iterations
+        is_sorted=True,
+        weights_prefix_sum=weights_prefix_sum,  # prefix sum of the sample weights, leave empty for unwieghted data
+        weighted_X_prefix_sum=weighted_X_prefix_sum,  # prefix sum of the weighted data
+        weighted_X_squared_prefix_sum=weighted_X_squared_prefix_sum,  # prefix sum of the squared weighted data
+        start_idx=start_idx,  # start index of the data
+        stop_idx=stop_idx,  # stop index of the data
+    )
 ```
 
+Refer to the docstrings for more information.
+
 ## Notes
 
 This repository has been created to be used in [Any-Precision-LLM](https://github.com/SNU-ARC/any-precision-llm) project,
 where multiple 1D K-means instances are run in parallel for LLM quantization.
 
-However the algorithm is general and can be used for any 1D K-means problem.
+However, the algorithm is general and can be used for any 1D K-means problem.
```

### Comparing `flash1dkmeans-0.0.2/pyproject.toml` & `flash1dkmeans-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "flash1dkmeans"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Jake Hyun", email="jake.hyun@hotmail.com" },
 ]
 description = "An optimized K-means implementation for the one-dimensional case."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `flash1dkmeans-0.0.2/PKG-INFO` & `flash1dkmeans-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: flash1dkmeans
-Version: 0.0.2
+Version: 0.0.3
 Summary: An optimized K-means implementation for the one-dimensional case.
 Project-URL: Homepage, https://github.com/SyphonArch/flash1dkmeans
 Project-URL: Issues, https://github.com/SyphonArch/flash1dkmeans/issues
 Author-email: Jake Hyun <jake.hyun@hotmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 Description-Content-Type: text/markdown
 
 # flash1dkmeans
 An optimized K-means implementation for the one-dimensional case
 
 Exploits the fact that one-dimensional data can be sorted.
 
-Numba acceleration is used, so callers can further use parallelization with Numba's `@njit(parallel=True)`
+For functions prefixed with `_`, Numba acceleration is used, so callers can further use parallelization with Numba's `@njit(parallel=True)`
 if multiple instances of the algorithm are run in parallel.
 
 ## Features
 
 ### Two clusters
 
 Guaranteed to find the optimal solution for two clusters.
@@ -73,22 +73,22 @@
 data = np.array([1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0, 8.0, 9.0, 10.0])
 weights = np.random.random_sample(data.shape)
 k = 3
 
 centroids, labels = kmeans_1d(
     data, k,
     sample_weights=weights,  # sample weights
-    n_local_trials=(2 + int(np.log(k))),  # number of local tries
     max_iter=100,  # maximum number of iterations
 )
 ```
 
 ### Even More Options
+The underlying Numba-accelerated function `_sorted_kmeans_1d` can be used directly for more control.
 ```python
-from flash1dkmeans import kmeans_1d
+from flash1dkmeans import _sorted_kmeans_1d_prefix_sums
 import numpy as np
 
 n, k = 1024, 4
 
 # Generate random data
 data = np.random.random_sample(n)
 data = np.sort(data)
@@ -102,27 +102,28 @@
 weighted_X_squared_prefix_sum = np.cumsum(data ** 2 * weights)
 
 middle_idx = n // 2
 
 # Providing prefix sums reduces redundant calculations
 # This is useful when the algorithm is run multiple times on different segments of the data
 for start_idx, stop_idx in [(0, middle_idx), (middle_idx, n)]:
-  centroids, cluster_borders = kmeans_1d(
-      data, k,  # Note how the sample weights are not provided when the prefix sums are provided
-      n_local_trials=(2 + int(np.log(k))),  # number of local tries
-      max_iter=100,  # maximum number of iterations
-      return_cluster_borders=True,  # return cluster borders instead of labels
-      weights_prefix_sum=weights_prefix_sum,  # prefix sum of the sample weights, leave empty for unwieghted data
-      weighted_X_prefix_sum=weighted_X_prefix_sum,  # prefix sum of the weighted data
-      weighted_X_squared_prefix_sum=weighted_X_squared_prefix_sum,  # prefix sum of the squared weighted data
-      start_idx=start_idx,  # start index of the data
-      stop_idx=stop_idx,  # stop index of the data
-  )
+    centroids, cluster_borders = _sorted_kmeans_1d_prefix_sums(
+        data, k,  # Note how the sample weights are not provided when the prefix sums are provided
+        max_iter=100,  # maximum number of iterations
+        is_sorted=True,
+        weights_prefix_sum=weights_prefix_sum,  # prefix sum of the sample weights, leave empty for unwieghted data
+        weighted_X_prefix_sum=weighted_X_prefix_sum,  # prefix sum of the weighted data
+        weighted_X_squared_prefix_sum=weighted_X_squared_prefix_sum,  # prefix sum of the squared weighted data
+        start_idx=start_idx,  # start index of the data
+        stop_idx=stop_idx,  # stop index of the data
+    )
 ```
 
+Refer to the docstrings for more information.
+
 ## Notes
 
 This repository has been created to be used in [Any-Precision-LLM](https://github.com/SNU-ARC/any-precision-llm) project,
 where multiple 1D K-means instances are run in parallel for LLM quantization.
 
-However the algorithm is general and can be used for any 1D K-means problem.
+However, the algorithm is general and can be used for any 1D K-means problem.
```

