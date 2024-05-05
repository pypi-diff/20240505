# Comparing `tmp/flash1dkmeans-0.0.3.tar.gz` & `tmp/flash1dkmeans-0.0.4.tar.gz`

## Comparing `flash1dkmeans-0.0.3.tar` & `flash1dkmeans-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/.idea/.gitignore
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/.idea/flash1dkmeans.iml
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/.idea/misc.xml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/.idea/vcs.xml
--rw-r--r--   0        0        0     7975 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/.idea/workspace.xml
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/src/flash1dkmeans/__init__.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/src/flash1dkmeans/config.py
--rw-r--r--   0        0        0    18911 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/src/flash1dkmeans/k_cluster.py
--rw-r--r--   0        0        0     9456 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/src/flash1dkmeans/main.py
--rw-r--r--   0        0        0     9797 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/src/flash1dkmeans/two_cluster.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/src/flash1dkmeans/utils.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/tests/complex.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/tests/k_cluster.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/tests/two_cluster.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/LICENSE
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/README.md
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/.idea/.gitignore
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/.idea/flash1dkmeans.iml
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/.idea/misc.xml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/.idea/vcs.xml
+-rw-r--r--   0        0        0     9005 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/.idea/workspace.xml
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/src/flash1dkmeans/__init__.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/src/flash1dkmeans/config.py
+-rw-r--r--   0        0        0    19117 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/src/flash1dkmeans/k_cluster.py
+-rw-r--r--   0        0        0     6861 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/src/flash1dkmeans/main.py
+-rw-r--r--   0        0        0     9878 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/src/flash1dkmeans/two_cluster.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/src/flash1dkmeans/utils.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/tests/complex.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/tests/k_cluster.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/tests/two_cluster.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/README.md
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 flash1dkmeans-0.0.4/PKG-INFO
```

### Comparing `flash1dkmeans-0.0.3/.idea/flash1dkmeans.iml` & `flash1dkmeans-0.0.4/.idea/flash1dkmeans.iml`

 * *Files identical despite different names*

### Comparing `flash1dkmeans-0.0.3/.idea/workspace.xml` & `flash1dkmeans-0.0.4/.idea/workspace.xml`

 * *Files 10% similar despite different names*

#### Comparing `flash1dkmeans-0.0.3/.idea/workspace.xml` & `flash1dkmeans-0.0.4/.idea/workspace.xml`

```diff
@@ -1,21 +1,20 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="1ba58836-480f-43dd-9244-0130cb4b0f23" name="Changes" comment="">
-      <change afterPath="$PROJECT_DIR$/tests/complex.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/flash1dkmeans/__init__.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/flash1dkmeans/__init__.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/flash1dkmeans/k_cluster.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/flash1dkmeans/k_cluster.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/flash1dkmeans/main.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/flash1dkmeans/main.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/flash1dkmeans/two_cluster.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/flash1dkmeans/two_cluster.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/flash1dkmeans/utils.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/flash1dkmeans/utils.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/tests/complex.py" beforeDir="false" afterPath="$PROJECT_DIR$/tests/complex.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
@@ -78,15 +77,15 @@
       <option name="presentableId" value="Default"/>
       <updated>1714838079481</updated>
       <workItem from="1714838080524" duration="170000"/>
       <workItem from="1714838257640" duration="1013000"/>
       <workItem from="1714888190868" duration="167000"/>
       <workItem from="1714898221385" duration="481000"/>
       <workItem from="1714899699435" duration="2811000"/>
-      <workItem from="1714905466256" duration="28184000"/>
+      <workItem from="1714905466256" duration="31361000"/>
     </task>
     <task id="LOCAL-00001" summary="Drop start_idx and stop_idx">
       <option name="closed" value="true"/>
       <created>1714905994757</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
@@ -144,25 +143,52 @@
       <option name="closed" value="true"/>
       <created>1714928130547</created>
       <option name="number" value="00008"/>
       <option name="presentableId" value="LOCAL-00008"/>
       <option name="project" value="LOCAL"/>
       <updated>1714928130547</updated>
     </task>
-    <option name="localTasksCounter" value="9"/>
+    <task id="LOCAL-00009" summary="Make Numba work">
+      <option name="closed" value="true"/>
+      <created>1714934013878</created>
+      <option name="number" value="00009"/>
+      <option name="presentableId" value="LOCAL-00009"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1714934013878</updated>
+    </task>
+    <task id="LOCAL-00010" summary="Increment version">
+      <option name="closed" value="true"/>
+      <created>1714934049075</created>
+      <option name="number" value="00010"/>
+      <option name="presentableId" value="LOCAL-00010"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1714934049075</updated>
+    </task>
+    <task id="LOCAL-00011" summary="Update README">
+      <option name="closed" value="true"/>
+      <created>1714934232634</created>
+      <option name="number" value="00011"/>
+      <option name="presentableId" value="LOCAL-00011"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1714934232634</updated>
+    </task>
+    <option name="localTasksCounter" value="12"/>
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
     <MESSAGE value="Cleanup"/>
     <MESSAGE value="Drop numba for now"/>
-    <option name="LAST_COMMIT_MESSAGE" value="Drop numba for now"/>
+    <MESSAGE value="Make Numba work"/>
+    <MESSAGE value="Increment version"/>
+    <MESSAGE value="Update README"/>
+    <option name="LAST_COMMIT_MESSAGE" value="Update README"/>
   </component>
 </project>
```

### Comparing `flash1dkmeans-0.0.3/.idea/inspectionProfiles/Project_Default.xml` & `flash1dkmeans-0.0.4/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `flash1dkmeans-0.0.3/src/flash1dkmeans/k_cluster.py` & `flash1dkmeans-0.0.4/src/flash1dkmeans/k_cluster.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,30 +13,30 @@
 import numba
 from .utils import query_prefix_sum
 import numpy as np
 from .config import ARRAY_INDEX_DTYPE
 
 
 @numba.njit(cache=True)
-def flash_1d_kmeans_k_cluster(
-        X,
+def numba_kmeans_1d_k_cluster(
+        sorted_X,
         n_clusters,
         max_iter,
         weights_prefix_sum, weighted_X_prefix_sum,
         weighted_X_squared_prefix_sum,
         start_idx,
         stop_idx,
 ):
     """An optimized kmeans for 1D data with n clusters.
     Exploits the fact that the data is 1D to optimize the calculations.
     Time complexity: O(n_clusters * log(n_clusters) * log(len(X)) * n_clusters + max_iter * log(len(X)) * n_clusters)
                       = O(k ^ 2 * log(k) * log(n) + max_iter * log(n) * k)
 
     Args:
-        X: np.ndarray
+        sorted_X: np.ndarray
             The input data. Should be sorted in ascending order.
         n_clusters: int
             The number of clusters to generate
         max_iter: int
             The maximum number of iterations to run
         weights_prefix_sum: np.ndarray
             The prefix sum of the weights. Should be None if the data is unweighted.
@@ -51,30 +51,30 @@
 
     Returns:
         centroids: np.ndarray
             The centroids of the clusters
         cluster_borders: np.ndarray
             The borders of the clusters
     """
-    assert weights_prefix_sum is not None, "weights_prefix_sum must be provided for weighted data"
+    assert n_clusters > 2, "n_clusters must be greater than 2, for 2 clusters use the faster two cluster implementation"
 
     cluster_borders = np.empty(n_clusters + 1, dtype=ARRAY_INDEX_DTYPE)
     cluster_borders[0] = start_idx
     cluster_borders[-1] = stop_idx
 
     centroids = _kmeans_plusplus(
-        X, n_clusters,
+        sorted_X, n_clusters,
         weights_prefix_sum, weighted_X_prefix_sum,
         weighted_X_squared_prefix_sum,
         start_idx, stop_idx,
     )
     sorted_centroids = np.sort(centroids)
 
     for _ in range(max_iter):
-        new_cluster_borders = _centroids_to_cluster_borders(X, sorted_centroids, start_idx, stop_idx)
+        new_cluster_borders = _centroids_to_cluster_borders(sorted_X, sorted_centroids, start_idx, stop_idx)
 
         if np.array_equal(cluster_borders, new_cluster_borders):
             break
 
         cluster_borders[:] = new_cluster_borders
         for i in range(n_clusters):
             cluster_start = cluster_borders[i]
@@ -87,47 +87,48 @@
                 continue
 
             cluster_weighted_X_sum = query_prefix_sum(weighted_X_prefix_sum, cluster_start, cluster_end)
             cluster_weight_sum = query_prefix_sum(weights_prefix_sum, cluster_start, cluster_end)
 
             if cluster_weight_sum == 0:
                 # if the sum of the weights is zero, we set the centroid to the mean of the cluster
-                sorted_centroids[i] = X[cluster_start:cluster_end].mean()
+                sorted_centroids[i] = sorted_X[cluster_start:cluster_end].mean()
             else:
                 sorted_centroids[i] = cluster_weighted_X_sum / cluster_weight_sum
 
     return sorted_centroids, cluster_borders
 
 
 @numba.njit(cache=True)
-def flash_1d_kmeans_k_cluster_unweighted(
-        X,
+def numba_kmeans_1d_k_cluster_unweighted(
+        sorted_X,
         n_clusters,
         max_iter,
         X_prefix_sum,
         X_squared_prefix_sum,
         start_idx,
         stop_idx,
 ):
     """Unweighted version of flash_1d_kmeans_k_cluster"""
+    assert n_clusters > 2, "n_clusters must be greater than 2, for 2 clusters use the faster two cluster implementation"
 
     cluster_borders = np.empty(n_clusters + 1, dtype=ARRAY_INDEX_DTYPE)
     cluster_borders[0] = start_idx
     cluster_borders[-1] = stop_idx
 
     centroids = _kmeans_plusplus_unweighted(
-        X, n_clusters,
+        sorted_X, n_clusters,
         X_prefix_sum,
         X_squared_prefix_sum,
         start_idx, stop_idx,
     )
     sorted_centroids = np.sort(centroids)
 
     for _ in range(max_iter):
-        new_cluster_borders = _centroids_to_cluster_borders(X, sorted_centroids, start_idx, stop_idx)
+        new_cluster_borders = _centroids_to_cluster_borders(sorted_X, sorted_centroids, start_idx, stop_idx)
 
         if np.array_equal(cluster_borders, new_cluster_borders):
             break
 
         cluster_borders[:] = new_cluster_borders
         for i in range(n_clusters):
             cluster_start = cluster_borders[i]
@@ -140,15 +141,15 @@
                 continue
 
             cluster_weighted_X_sum = query_prefix_sum(X_prefix_sum, cluster_start, cluster_end)
             cluster_weight_sum = cluster_end - cluster_start
 
             if cluster_weight_sum == 0:
                 # if the sum of the weights is zero, we set the centroid to the mean of the cluster
-                sorted_centroids[i] = X[cluster_start:cluster_end].mean()
+                sorted_centroids[i] = sorted_X[cluster_start:cluster_end].mean()
             else:
                 sorted_centroids[i] = cluster_weighted_X_sum / cluster_weight_sum
 
     return sorted_centroids, cluster_borders
 
 
 @numba.njit(cache=True)
```

### Comparing `flash1dkmeans-0.0.3/src/flash1dkmeans/main.py` & `flash1dkmeans-0.0.4/src/flash1dkmeans/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-from .k_cluster import flash_1d_kmeans_k_cluster, flash_1d_kmeans_k_cluster_unweighted
-from .two_cluster import flash_1d_kmeans_two_cluster, flash_1d_kmeans_two_cluster_unweighted
+from .k_cluster import numba_kmeans_1d_k_cluster, numba_kmeans_1d_k_cluster_unweighted
+from .two_cluster import numba_kmeans_1d_two_cluster, numba_kmeans_1d_two_cluster_unweighted
 from .config import LABEL_DTYPE, PREFIX_SUM_DTYPE
 import numpy as np
 import logging
-import numba
 
 
 def kmeans_1d(
         X,
         n_clusters,
-        max_iter=300,
+        max_iter=None,
         is_sorted=False,
         sample_weights=None,
         n_local_trials=None,
         return_cluster_borders=False,
 ):
     """An optimized kmeans for 1D data.
     Utilizes a binary search to find the optimal division points for 2 clusters,
@@ -31,14 +30,15 @@
     Args:
         X: np.ndarray or list
             The input data. Should be sorted in ascending order if is_sorted is False.
         n_clusters: int
             The number of clusters.
         max_iter: int
             The maximum number of iterations. Only relevant for n_clusters > 2.
+            Default is None, which becomes 300 for n_clusters > 2.
         is_sorted: bool
             Whether the data is already sorted.
         sample_weights: np.ndarray or list or None
             The sample weights. If None, all samples are weighted equally.
         n_local_trials: int
             The number of local trials for kmeans++ initialization. Only relevant for n_clusters > 2.
         return_cluster_borders: bool
@@ -65,17 +65,24 @@
 
     # Check that return_cluster_borders is called with is_sorted=True, warn the user otherwise
     if return_cluster_borders:  # User requested cluster borders
         if not is_sorted:  # However, the user did not provide sorted data
             logging.warning(  # Warn the user that the data will be sorted
                 "The returned cluster borders will be indexed in the sorted order of X, not the original order.")
 
+    # max_iter is redundant if n_clusters == 2
+    if n_clusters == 2:
+        assert max_iter is None, "max_iter should not be provided for 2 clusters"
+    else:
+        if max_iter is None:
+            max_iter = 300
+
     # Check some values
     assert n_clusters >= 2, "n_clusters must be at least 2"
-    assert max_iter >= 0, "max_iter must be non-negative"
+    assert max_iter is None or max_iter >= 0, "max_iter must be non-negative"
     assert n_local_trials is None or n_local_trials > 0, "n_local_trials must be positive"
 
     # -------------- Convert all arrays to numpy arrays --------------
     X = np.asarray(X)
 
     if sample_weights is not None:
         sample_weights = np.asarray(sample_weights)
@@ -89,29 +96,62 @@
         sorted_X = X[sorted_indices]
         sorted_sample_weights = None if sample_weights is None else sample_weights[sorted_indices]
     else:
         sorted_indices = None
         sorted_X = X
         sorted_sample_weights = sample_weights
 
-    # -------------- Main algorithm --------------
+    # -------------- Calculate prefix sums & Execute main algorithm --------------
+
+    sorted_X_casted = sorted_X.astype(PREFIX_SUM_DTYPE)
 
     if is_weighted:
-        centroids, cluster_borders = _sorted_kmeans_1d(
-            sorted_X,
-            n_clusters,
-            max_iter,
-            sorted_sample_weights,
-        )
-    else:
-        centroids, cluster_borders = _sorted_kmeans_1d_unweighted(
-            sorted_X,
-            n_clusters,
-            max_iter,
-        )
+        sample_weights_casted = sorted_sample_weights.astype(PREFIX_SUM_DTYPE)
+        sample_weight_prefix_sum = np.cumsum(sample_weights_casted)
+        weighted_X_prefix_sum = np.cumsum(sorted_X_casted * sample_weights_casted)
+        if n_clusters == 2:
+            centroids, cluster_borders = numba_kmeans_1d_two_cluster(
+                sorted_X=sorted_X,
+                weighted_X_prefix_sum=weighted_X_prefix_sum,
+                weights_prefix_sum=sample_weight_prefix_sum,
+                start_idx=0,
+                stop_idx=len(sorted_X),
+            )
+        else:
+            weighted_X_squared_prefix_sum = np.cumsum(sorted_X_casted ** 2 * sample_weights_casted)
+            centroids, cluster_borders = numba_kmeans_1d_k_cluster(
+                sorted_X=sorted_X,
+                n_clusters=n_clusters,
+                max_iter=max_iter,
+                weights_prefix_sum=sample_weight_prefix_sum,
+                weighted_X_prefix_sum=weighted_X_prefix_sum,
+                weighted_X_squared_prefix_sum=weighted_X_squared_prefix_sum,
+                start_idx=0,
+                stop_idx=len(sorted_X),
+            )
+    else:
+        X_prefix_sum = np.cumsum(sorted_X_casted)
+        if n_clusters == 2:
+            centroids, cluster_borders = numba_kmeans_1d_two_cluster_unweighted(
+                sorted_X=sorted_X,
+                X_prefix_sum=X_prefix_sum,
+                start_idx=0,
+                stop_idx=len(sorted_X),
+            )
+        else:
+            X_squared_prefix_sum = np.cumsum(sorted_X_casted ** 2)
+            centroids, cluster_borders = numba_kmeans_1d_k_cluster_unweighted(
+                sorted_X=sorted_X,
+                n_clusters=n_clusters,
+                max_iter=max_iter,
+                X_prefix_sum=X_prefix_sum,
+                X_squared_prefix_sum=X_squared_prefix_sum,
+                start_idx=0,
+                stop_idx=len(sorted_X),
+            )
 
     # -------------- Post-processing --------------
 
     if return_cluster_borders:
         # We checked that the data is sorted if cluster borders are requested, so no post-processing is needed
         return centroids, cluster_borders
     else:
@@ -122,161 +162,7 @@
 
         # Unsort the labels if the data was not sorted
         if not is_sorted:
             assert sorted_indices is not None, "sorted_indices should be available here"
             labels = labels[np.argsort(sorted_indices)]
 
         return centroids, labels
-
-
-@numba.njit(cache=True)
-def _sorted_kmeans_1d(
-        sorted_X,
-        n_clusters,
-        max_iter,
-        sample_weights,
-):
-    """Create the prefix sums and call the main algorithm, for weighted data"""
-    sample_weights_casted = sample_weights.astype(PREFIX_SUM_DTYPE)
-    weights_prefix_sum = np.cumsum(sample_weights_casted)
-
-    sorted_X_casted = sorted_X.astype(PREFIX_SUM_DTYPE)
-    weighted_X_prefix_sum = np.cumsum(sorted_X_casted * sample_weights_casted)
-    weighted_X_squared_prefix_sum = np.cumsum(sorted_X_casted ** 2 * sample_weights_casted)
-
-    centroids, cluster_borders = _sorted_kmeans_1d_prefix_sums(
-        sorted_X,
-        n_clusters,
-        max_iter,
-        weights_prefix_sum,
-        weighted_X_prefix_sum,
-        weighted_X_squared_prefix_sum,
-        start_idx=0,
-        stop_idx=len(sorted_X),
-    )
-
-    return centroids, cluster_borders
-
-
-@numba.njit(cache=True)
-def _sorted_kmeans_1d_unweighted(
-        sorted_X,
-        n_clusters,
-        max_iter,
-):
-    """Create the prefix sums and call the main algorithm, for unweighted data"""
-    X_casted = sorted_X.astype(PREFIX_SUM_DTYPE)
-    X_prefix_sum = np.cumsum(X_casted)
-    X_squared_prefix_sum = np.cumsum(X_casted ** 2)
-
-    centroids, cluster_borders = _sorted_kmeans_1d_prefix_sums_unweighted(
-        sorted_X,
-        n_clusters,
-        max_iter,
-        X_prefix_sum,
-        X_squared_prefix_sum,
-        start_idx=0,
-        stop_idx=len(sorted_X),
-    )
-
-    return centroids, cluster_borders
-
-
-@numba.njit(cache=True)
-def _sorted_kmeans_1d_prefix_sums(
-        sorted_X,  # caller should ensure that X is sorted
-        n_clusters,  # caller should ensure n_clusters >= 2
-        max_iter,  # caller should ensure max_iter >= 0
-        weights_prefix_sum,
-        weighted_X_prefix_sum,
-        weighted_X_squared_prefix_sum,
-        start_idx=None,
-        stop_idx=None,
-):
-    """The main algorithm for flash_1d_kmeans.
-    This function assumes that the input data is sorted, and all input is assumed to be valid.
-
-    Time complexity:
-        2 clusters:
-            O(log(n)) (+ (O(n) for prefix sum calculation if not provided))
-        n clusters:
-            O(n_clusters * 2 + log(n_clusters) * log(n) + max_iter * log(n) * n_clusters)
-            (+ (O(n) for prefix sum calculation if not provided))
-
-    Args:
-        sorted_X: np.ndarray
-            The input data. Should be sorted in ascending order.
-        n_clusters: int
-            The number of clusters.
-        max_iter: int
-            The maximum number of iterations.
-        weights_prefix_sum: np.ndarray
-            The prefix sum of the sample weights.
-        weighted_X_prefix_sum: np.ndarray
-            The prefix sum of X, weighted by the sample weights.
-        weighted_X_squared_prefix_sum: np.ndarray
-            The prefix sum of X squared, weighted by the sample weights.
-        start_idx: int
-            The start index of the range to consider.
-        stop_idx: int
-            The stop index of the range to consider.
-
-    Returns:
-        centroids: np.ndarray
-            The centroids of the clusters.
-        cluster_borders: np.ndarray
-            The borders of the clusters.
-    """
-
-    if n_clusters == 2:
-        centroids, cluster_borders = flash_1d_kmeans_two_cluster(
-            sorted_X,
-            weighted_X_prefix_sum,
-            weights_prefix_sum,
-            start_idx,
-            stop_idx,
-        )
-    else:
-        centroids, cluster_borders = flash_1d_kmeans_k_cluster(
-            sorted_X,
-            n_clusters,
-            max_iter,
-            weights_prefix_sum,
-            weighted_X_prefix_sum,
-            weighted_X_squared_prefix_sum,
-            start_idx,
-            stop_idx,
-        )
-
-    return centroids, cluster_borders
-
-
-@numba.njit(cache=True)
-def _sorted_kmeans_1d_prefix_sums_unweighted(
-        sorted_X,
-        n_clusters,
-        max_iter,
-        X_prefix_sum,
-        X_squared_prefix_sum,
-        start_idx,
-        stop_idx,
-):
-    """The unweighted version of _sorted_kmeans_1d_prefix_sums"""
-    if n_clusters == 2:
-        centroids, cluster_borders = flash_1d_kmeans_two_cluster_unweighted(
-            sorted_X,
-            X_prefix_sum,
-            start_idx,
-            stop_idx,
-        )
-    else:
-        centroids, cluster_borders = flash_1d_kmeans_k_cluster_unweighted(
-            sorted_X,
-            n_clusters,
-            max_iter,
-            X_prefix_sum,
-            X_squared_prefix_sum,
-            start_idx,
-            stop_idx,
-        )
-
-    return centroids, cluster_borders
```

### Comparing `flash1dkmeans-0.0.3/src/flash1dkmeans/two_cluster.py` & `flash1dkmeans-0.0.4/src/flash1dkmeans/two_cluster.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,86 +13,86 @@
 import numpy as np
 import numba
 from .utils import query_prefix_sum
 from .config import PREFIX_SUM_DTYPE, ARRAY_INDEX_DTYPE
 
 
 @numba.njit(cache=True)
-def flash_1d_kmeans_two_cluster(
-        X,
+def numba_kmeans_1d_two_cluster(
+        sorted_X,
         weighted_X_prefix_sum,
-        sample_weight_prefix_sum,
+        weights_prefix_sum,
         start_idx,
         stop_idx,
 ):
     """An optimized kmeans for 1D data with 2 clusters, weighted version.
     Utilizes a binary search to find the optimal division point.
     Time complexity: O(log(n))
 
     Args:
-        X: np.ndarray
+        sorted_X: np.ndarray
             The input data. Should be sorted in ascending order.
         weighted_X_prefix_sum: np.ndarray
             The prefix sum of (the weighted) X.
-        sample_weight_prefix_sum: np.ndarray
+        weights_prefix_sum: np.ndarray
             The prefix sum of the sample weights. Should be None if the data is unweighted.
         start_idx: int
             The start index of the range to consider.
         stop_idx: int
             The stop index of the range to consider.
 
     Returns:
         centroids: np.ndarray
             The centroids of the two clusters, shape (2,)
         cluster_borders: np.ndarray
             The borders of the two clusters, shape (3,)
 
     WARNING: X should be sorted in ascending order before calling this function.
     """
-    assert sample_weight_prefix_sum is not None, "sample_weight_prefix_sum must be provided for weighted data"
+    assert weights_prefix_sum is not None, "sample_weight_prefix_sum must be provided for weighted data"
 
     size = stop_idx - start_idx
-    centroids = np.empty(2, dtype=X.dtype)
+    centroids = np.empty(2, dtype=sorted_X.dtype)
     cluster_borders = np.empty(3, dtype=ARRAY_INDEX_DTYPE)
     cluster_borders[0] = start_idx
     cluster_borders[2] = stop_idx
     # Remember to set cluster_borders[1] as the division point
 
     if size == 1:
-        centroids[0], centroids[1] = X[start_idx], X[start_idx]
+        centroids[0], centroids[1] = sorted_X[start_idx], sorted_X[start_idx]
         cluster_borders[1] = start_idx + 1
         return centroids, cluster_borders
 
     if size == 2:
-        centroids[0], centroids[1] = X[start_idx], X[start_idx + 1]
+        centroids[0], centroids[1] = sorted_X[start_idx], sorted_X[start_idx + 1]
         cluster_borders[1] = start_idx + 1
         return centroids, cluster_borders
 
     # Now we know that there are at least 3 elements
 
     # If the sum of the sample weight in the range is 0, we assume that the data is unweighted
-    if query_prefix_sum(sample_weight_prefix_sum, start_idx, stop_idx) == 0:
+    if query_prefix_sum(weights_prefix_sum, start_idx, stop_idx) == 0:
         # We need to recalculate the prefix sum, as previously it would have been all zeros
-        X_casted = X.astype(PREFIX_SUM_DTYPE)
+        X_casted = sorted_X.astype(PREFIX_SUM_DTYPE)
         X_prefix_sum = np.cumsum(X_casted)
-        return flash_1d_kmeans_two_cluster_unweighted(X, X_prefix_sum, start_idx, stop_idx)
+        return numba_kmeans_1d_two_cluster_unweighted(sorted_X, X_prefix_sum, start_idx, stop_idx)
     else:
         # Check if there is only one nonzero sample weight
-        total_weight = query_prefix_sum(sample_weight_prefix_sum, start_idx, stop_idx)
-        sample_weight_prefix_sum_within_range = sample_weight_prefix_sum[start_idx:stop_idx]
+        total_weight = query_prefix_sum(weights_prefix_sum, start_idx, stop_idx)
+        sample_weight_prefix_sum_within_range = weights_prefix_sum[start_idx:stop_idx]
         final_increase_idx = np.searchsorted(sample_weight_prefix_sum_within_range,
                                              sample_weight_prefix_sum_within_range[-1])
-        final_increase_amount = query_prefix_sum(sample_weight_prefix_sum,
+        final_increase_amount = query_prefix_sum(weights_prefix_sum,
                                                  start_idx + final_increase_idx,
                                                  start_idx + final_increase_idx + 1)
         if total_weight == final_increase_amount:
             # If there is only one nonzero sample weight, we need to return the corresponding weight as the centroid
             # and set all elements to the left cluster
             nonzero_weight_index = start_idx + final_increase_idx
-            centroids[0], centroids[1] = X[nonzero_weight_index], X[nonzero_weight_index]
+            centroids[0], centroids[1] = sorted_X[nonzero_weight_index], sorted_X[nonzero_weight_index]
             cluster_borders[1] = stop_idx
             return centroids, cluster_borders
 
     # Now we know that there are at least 3 elements and at least 2 nonzero weights
 
     # KMeans with 2 clusters on 1D data is equivalent to finding a division point.
     # The division point can be found by doing a binary search on the prefix sum.
@@ -105,77 +105,77 @@
     left_centroid = None
     right_centroid = None
     division_point = None
 
     while floor + 1 < ceiling:
         division_point = (floor + ceiling) // 2
         # If the left cluster has no weight, we need to move the floor up
-        left_weight_sum = query_prefix_sum(sample_weight_prefix_sum, start_idx, division_point)
+        left_weight_sum = query_prefix_sum(weights_prefix_sum, start_idx, division_point)
         if left_weight_sum == 0:
             floor = division_point
             continue
-        right_weight_sum = query_prefix_sum(sample_weight_prefix_sum, division_point, stop_idx)
+        right_weight_sum = query_prefix_sum(weights_prefix_sum, division_point, stop_idx)
         # If the right cluster has no weight, we need to move the ceiling down
         if right_weight_sum == 0:
             ceiling = division_point
             continue
 
         left_centroid = query_prefix_sum(weighted_X_prefix_sum, start_idx, division_point) / left_weight_sum
         right_centroid = query_prefix_sum(weighted_X_prefix_sum, division_point, stop_idx) / right_weight_sum
 
         new_division_point_value = (left_centroid + right_centroid) / 2
-        if X[division_point - 1] <= new_division_point_value:
-            if new_division_point_value <= X[division_point]:
+        if sorted_X[division_point - 1] <= new_division_point_value:
+            if new_division_point_value <= sorted_X[division_point]:
                 # The new division point matches the previous one, so we can stop
                 break
             else:
                 floor = division_point
         else:
             ceiling = division_point
 
     # initialize variables in case the loop above does not run through
     if left_centroid is None:
         division_point = (floor + ceiling) // 2
         left_centroid = (query_prefix_sum(weighted_X_prefix_sum, start_idx, division_point) /
-                         query_prefix_sum(sample_weight_prefix_sum, start_idx, division_point))
+                         query_prefix_sum(weights_prefix_sum, start_idx, division_point))
     if right_centroid is None:
         division_point = (floor + ceiling) // 2
         right_centroid = (query_prefix_sum(weighted_X_prefix_sum, division_point, stop_idx) /
-                          query_prefix_sum(sample_weight_prefix_sum, division_point, stop_idx))
+                          query_prefix_sum(weights_prefix_sum, division_point, stop_idx))
 
     # avoid using lists to allow numba.njit
     centroids[0] = left_centroid
     centroids[1] = right_centroid
 
     cluster_borders[1] = division_point
     return centroids, cluster_borders
 
 
 @numba.njit(cache=True)
-def flash_1d_kmeans_two_cluster_unweighted(
-        X,
+def numba_kmeans_1d_two_cluster_unweighted(
+        sorted_X,
         X_prefix_sum,
         start_idx,
         stop_idx,
 ):
     """Unweighted version of flash_1d_kmeans_two_cluster."""
     size = stop_idx - start_idx
-    centroids = np.empty(2, dtype=X.dtype)
+    centroids = np.empty(2, dtype=sorted_X.dtype)
     cluster_borders = np.empty(3, dtype=ARRAY_INDEX_DTYPE)
     cluster_borders[0] = start_idx
     cluster_borders[2] = stop_idx
     # Remember to set cluster_borders[1] as the division point
 
     if size == 1:
-        centroids[0], centroids[1] = X[start_idx], X[start_idx]
+        centroids[0], centroids[1] = sorted_X[start_idx], sorted_X[start_idx]
         cluster_borders[1] = start_idx + 1
         return centroids, cluster_borders
 
     if size == 2:
-        centroids[0], centroids[1] = X[start_idx], X[start_idx + 1]
+        centroids[0], centroids[1] = sorted_X[start_idx], sorted_X[start_idx + 1]
         cluster_borders[1] = start_idx + 1
         return centroids, cluster_borders
 
     # Now we know that there are at least 3 elements and at least 2 nonzero weights
 
     # KMeans with 2 clusters on 1D data is equivalent to finding a division point.
     # The division point can be found by doing a binary search on the prefix sum.
@@ -202,16 +202,16 @@
             ceiling = division_point
             continue
 
         left_centroid = query_prefix_sum(X_prefix_sum, start_idx, division_point) / left_weight_sum
         right_centroid = query_prefix_sum(X_prefix_sum, division_point, stop_idx) / right_weight_sum
 
         new_division_point_value = (left_centroid + right_centroid) / 2
-        if X[division_point - 1] <= new_division_point_value:
-            if new_division_point_value <= X[division_point]:
+        if sorted_X[division_point - 1] <= new_division_point_value:
+            if new_division_point_value <= sorted_X[division_point]:
                 # The new division point matches the previous one, so we can stop
                 break
             else:
                 floor = division_point
         else:
             ceiling = division_point
```

### Comparing `flash1dkmeans-0.0.3/tests/complex.py` & `flash1dkmeans-0.0.4/tests/complex.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from flash1dkmeans import _sorted_kmeans_1d_prefix_sums
+from flash1dkmeans import numba_kmeans_1d_k_cluster
 import numpy as np
 
 n, k = 1024, 4
 
 # Generate random data
 data = np.random.random_sample(n)
 data = np.sort(data)
@@ -18,15 +18,15 @@
 weighted_X_squared_prefix_sum = np.cumsum(data ** 2 * weights)
 
 middle_idx = n // 2
 
 # Providing prefix sums reduces redundant calculations
 # This is useful when the algorithm is run multiple times on different segments of the data
 for start_idx, stop_idx in [(0, middle_idx), (middle_idx, n)]:
-    centroids, cluster_borders = _sorted_kmeans_1d_prefix_sums(
+    centroids, cluster_borders = numba_kmeans_1d_k_cluster(
         data, k,  # Note how the sample weights are not provided when the prefix sums are provided
         max_iter=100,  # maximum number of iterations
         weights_prefix_sum=weights_prefix_sum,  # prefix sum of the sample weights, leave empty for unwieghted data
         weighted_X_prefix_sum=weighted_X_prefix_sum,  # prefix sum of the weighted data
         weighted_X_squared_prefix_sum=weighted_X_squared_prefix_sum,  # prefix sum of the squared weighted data
         start_idx=start_idx,  # start index of the data
         stop_idx=stop_idx,  # stop index of the data
```

### Comparing `flash1dkmeans-0.0.3/.gitignore` & `flash1dkmeans-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `flash1dkmeans-0.0.3/LICENSE` & `flash1dkmeans-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flash1dkmeans-0.0.3/README.md` & `flash1dkmeans-0.0.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # flash1dkmeans
 An optimized K-means implementation for the one-dimensional case
 
 Exploits the fact that one-dimensional data can be sorted.
 
-For functions prefixed with `_`, Numba acceleration is used, so callers can further use parallelization with Numba's `@njit(parallel=True)`
-if multiple instances of the algorithm are run in parallel.
+For the lower level functions prefixed with `numba_`, Numba acceleration is used,
+so callers can utilize these functions within their own Numba-accelerated functions.
 
 ## Features
 
 ### Two clusters
 
 Guaranteed to find the optimal solution for two clusters.
 
@@ -63,16 +63,26 @@
     sample_weights=weights,  # sample weights
     max_iter=100,  # maximum number of iterations
 )
 ```
 
 ### Even More Options
 The underlying Numba-accelerated function `_sorted_kmeans_1d` can be used directly for more control.
+
+This is useful when the algorithm is run multiple times on different segments of the data,
+or to use within another Numba-accelerated function.
+
+The list of available functions are as follows:
+- `numba_kmeans_1d_two_clusters`
+- `numba_kmeans_1d_two_clusters_unweighted`
+- `numba_kmeans_1d_k_cluster`
+- `numba_kmeans_1d_k_cluster_unweighted`
+
 ```python
-from flash1dkmeans import _sorted_kmeans_1d_prefix_sums
+from flash1dkmeans import numba_kmeans_1d_k_cluster
 import numpy as np
 
 n, k = 1024, 4
 
 # Generate random data
 data = np.random.random_sample(n)
 data = np.sort(data)
@@ -86,24 +96,24 @@
 weighted_X_squared_prefix_sum = np.cumsum(data ** 2 * weights)
 
 middle_idx = n // 2
 
 # Providing prefix sums reduces redundant calculations
 # This is useful when the algorithm is run multiple times on different segments of the data
 for start_idx, stop_idx in [(0, middle_idx), (middle_idx, n)]:
-    centroids, cluster_borders = _sorted_kmeans_1d_prefix_sums(
-        data, k,  # Note how the sample weights are not provided when the prefix sums are provided
-        max_iter=100,  # maximum number of iterations
-        is_sorted=True,
-        weights_prefix_sum=weights_prefix_sum,  # prefix sum of the sample weights, leave empty for unwieghted data
-        weighted_X_prefix_sum=weighted_X_prefix_sum,  # prefix sum of the weighted data
-        weighted_X_squared_prefix_sum=weighted_X_squared_prefix_sum,  # prefix sum of the squared weighted data
-        start_idx=start_idx,  # start index of the data
-        stop_idx=stop_idx,  # stop index of the data
-    )
+  centroids, cluster_borders = numba_kmeans_1d_k_cluster(
+    data, k,  # Note how the sample weights are not provided when the prefix sums are provided
+    max_iter=100,  # maximum number of iterations
+    is_sorted=True,
+    weights_prefix_sum=weights_prefix_sum,  # prefix sum of the sample weights, leave empty for unwieghted data
+    weighted_X_prefix_sum=weighted_X_prefix_sum,  # prefix sum of the weighted data
+    weighted_X_squared_prefix_sum=weighted_X_squared_prefix_sum,  # prefix sum of the squared weighted data
+    start_idx=start_idx,  # start index of the data
+    stop_idx=stop_idx,  # stop index of the data
+  )
 ```
 
 Refer to the docstrings for more information.
 
 ## Notes
 
 This repository has been created to be used in [Any-Precision-LLM](https://github.com/SNU-ARC/any-precision-llm) project,
```

### Comparing `flash1dkmeans-0.0.3/pyproject.toml` & `flash1dkmeans-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "flash1dkmeans"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Jake Hyun", email="jake.hyun@hotmail.com" },
 ]
 description = "An optimized K-means implementation for the one-dimensional case."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `flash1dkmeans-0.0.3/PKG-INFO` & `flash1dkmeans-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: flash1dkmeans
-Version: 0.0.3
+Version: 0.0.4
 Summary: An optimized K-means implementation for the one-dimensional case.
 Project-URL: Homepage, https://github.com/SyphonArch/flash1dkmeans
 Project-URL: Issues, https://github.com/SyphonArch/flash1dkmeans/issues
 Author-email: Jake Hyun <jake.hyun@hotmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,16 +15,16 @@
 Description-Content-Type: text/markdown
 
 # flash1dkmeans
 An optimized K-means implementation for the one-dimensional case
 
 Exploits the fact that one-dimensional data can be sorted.
 
-For functions prefixed with `_`, Numba acceleration is used, so callers can further use parallelization with Numba's `@njit(parallel=True)`
-if multiple instances of the algorithm are run in parallel.
+For the lower level functions prefixed with `numba_`, Numba acceleration is used,
+so callers can utilize these functions within their own Numba-accelerated functions.
 
 ## Features
 
 ### Two clusters
 
 Guaranteed to find the optimal solution for two clusters.
 
@@ -79,16 +79,26 @@
     sample_weights=weights,  # sample weights
     max_iter=100,  # maximum number of iterations
 )
 ```
 
 ### Even More Options
 The underlying Numba-accelerated function `_sorted_kmeans_1d` can be used directly for more control.
+
+This is useful when the algorithm is run multiple times on different segments of the data,
+or to use within another Numba-accelerated function.
+
+The list of available functions are as follows:
+- `numba_kmeans_1d_two_clusters`
+- `numba_kmeans_1d_two_clusters_unweighted`
+- `numba_kmeans_1d_k_cluster`
+- `numba_kmeans_1d_k_cluster_unweighted`
+
 ```python
-from flash1dkmeans import _sorted_kmeans_1d_prefix_sums
+from flash1dkmeans import numba_kmeans_1d_k_cluster
 import numpy as np
 
 n, k = 1024, 4
 
 # Generate random data
 data = np.random.random_sample(n)
 data = np.sort(data)
@@ -102,24 +112,24 @@
 weighted_X_squared_prefix_sum = np.cumsum(data ** 2 * weights)
 
 middle_idx = n // 2
 
 # Providing prefix sums reduces redundant calculations
 # This is useful when the algorithm is run multiple times on different segments of the data
 for start_idx, stop_idx in [(0, middle_idx), (middle_idx, n)]:
-    centroids, cluster_borders = _sorted_kmeans_1d_prefix_sums(
-        data, k,  # Note how the sample weights are not provided when the prefix sums are provided
-        max_iter=100,  # maximum number of iterations
-        is_sorted=True,
-        weights_prefix_sum=weights_prefix_sum,  # prefix sum of the sample weights, leave empty for unwieghted data
-        weighted_X_prefix_sum=weighted_X_prefix_sum,  # prefix sum of the weighted data
-        weighted_X_squared_prefix_sum=weighted_X_squared_prefix_sum,  # prefix sum of the squared weighted data
-        start_idx=start_idx,  # start index of the data
-        stop_idx=stop_idx,  # stop index of the data
-    )
+  centroids, cluster_borders = numba_kmeans_1d_k_cluster(
+    data, k,  # Note how the sample weights are not provided when the prefix sums are provided
+    max_iter=100,  # maximum number of iterations
+    is_sorted=True,
+    weights_prefix_sum=weights_prefix_sum,  # prefix sum of the sample weights, leave empty for unwieghted data
+    weighted_X_prefix_sum=weighted_X_prefix_sum,  # prefix sum of the weighted data
+    weighted_X_squared_prefix_sum=weighted_X_squared_prefix_sum,  # prefix sum of the squared weighted data
+    start_idx=start_idx,  # start index of the data
+    stop_idx=stop_idx,  # stop index of the data
+  )
 ```
 
 Refer to the docstrings for more information.
 
 ## Notes
 
 This repository has been created to be used in [Any-Precision-LLM](https://github.com/SNU-ARC/any-precision-llm) project,
```

