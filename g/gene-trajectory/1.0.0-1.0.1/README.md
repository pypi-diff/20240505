# Comparing `tmp/gene_trajectory-1.0.0.tar.gz` & `tmp/gene_trajectory-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gene_trajectory-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gene_trajectory-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gene_trajectory-1.0.0.tar` & `gene_trajectory-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0     1070 2024-04-07 18:01:15.531167 gene_trajectory-1.0.0/LICENSE
--rw-r--r--   0        0        0     3275 2024-04-07 18:01:15.531167 gene_trajectory-1.0.0/README.md
--rw-r--r--   0        0        0        0 2024-04-07 18:01:15.599167 gene_trajectory-1.0.0/gene_trajectory/__init__.py
--rw-r--r--   0        0        0     1861 2024-04-07 18:01:15.599167 gene_trajectory-1.0.0/gene_trajectory/add_gene_bin_score.py
--rw-r--r--   0        0        0     4642 2024-04-07 18:01:15.599167 gene_trajectory-1.0.0/gene_trajectory/coarse_grain.py
--rw-r--r--   0        0        0     2846 2024-04-07 18:01:15.599167 gene_trajectory-1.0.0/gene_trajectory/compute_gene_distance_cmd.py
--rw-r--r--   0        0        0     2337 2024-04-07 18:01:15.599167 gene_trajectory-1.0.0/gene_trajectory/diffusion_map.py
--rw-r--r--   0        0        0     5578 2024-04-07 18:01:15.599167 gene_trajectory-1.0.0/gene_trajectory/extract_gene_trajectory.py
--rw-r--r--   0        0        0     3845 2024-04-07 18:01:15.599167 gene_trajectory-1.0.0/gene_trajectory/gene_distance_shared.py
--rw-r--r--   0        0        0     1497 2024-04-07 18:01:15.599167 gene_trajectory-1.0.0/gene_trajectory/get_graph_distance.py
--rw-r--r--   0        0        0        0 2024-04-07 18:01:15.599167 gene_trajectory-1.0.0/gene_trajectory/plot/__init__.py
--rw-r--r--   0        0        0     2806 2024-04-07 18:01:15.599167 gene_trajectory-1.0.0/gene_trajectory/plot/gene_trajectory_plots.py
--rw-r--r--   0        0        0     1593 2024-04-07 18:01:15.599167 gene_trajectory-1.0.0/gene_trajectory/run_dm.py
--rw-r--r--   0        0        0        0 2024-04-07 18:01:15.599167 gene_trajectory-1.0.0/gene_trajectory/util/__init__.py
--rw-r--r--   0        0        0     1331 2024-04-07 18:01:15.599167 gene_trajectory-1.0.0/gene_trajectory/util/download_file.py
--rw-r--r--   0        0        0     3053 2024-04-07 18:01:15.599167 gene_trajectory-1.0.0/gene_trajectory/util/shared_array.py
--rw-r--r--   0        0        0     1317 2024-04-07 18:01:15.599167 gene_trajectory-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4504 1970-01-01 00:00:00.000000 gene_trajectory-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-05 11:42:36.815260 gene_trajectory-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3441 2024-05-05 11:42:36.815260 gene_trajectory-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-05 11:42:36.859261 gene_trajectory-1.0.1/gene_trajectory/__init__.py
+-rw-r--r--   0        0        0     1861 2024-05-05 11:42:36.859261 gene_trajectory-1.0.1/gene_trajectory/add_gene_bin_score.py
+-rw-r--r--   0        0        0     4642 2024-05-05 11:42:36.859261 gene_trajectory-1.0.1/gene_trajectory/coarse_grain.py
+-rw-r--r--   0        0        0     2846 2024-05-05 11:42:36.859261 gene_trajectory-1.0.1/gene_trajectory/compute_gene_distance_cmd.py
+-rw-r--r--   0        0        0     2337 2024-05-05 11:42:36.859261 gene_trajectory-1.0.1/gene_trajectory/diffusion_map.py
+-rw-r--r--   0        0        0     5583 2024-05-05 11:42:36.859261 gene_trajectory-1.0.1/gene_trajectory/extract_gene_trajectory.py
+-rw-r--r--   0        0        0     3845 2024-05-05 11:42:36.859261 gene_trajectory-1.0.1/gene_trajectory/gene_distance_shared.py
+-rw-r--r--   0        0        0     1497 2024-05-05 11:42:36.859261 gene_trajectory-1.0.1/gene_trajectory/get_graph_distance.py
+-rw-r--r--   0        0        0        0 2024-05-05 11:42:36.859261 gene_trajectory-1.0.1/gene_trajectory/plot/__init__.py
+-rw-r--r--   0        0        0     3531 2024-05-05 11:42:36.859261 gene_trajectory-1.0.1/gene_trajectory/plot/gene_trajectory_plots.py
+-rw-r--r--   0        0        0     1593 2024-05-05 11:42:36.859261 gene_trajectory-1.0.1/gene_trajectory/run_dm.py
+-rw-r--r--   0        0        0        0 2024-05-05 11:42:36.859261 gene_trajectory-1.0.1/gene_trajectory/util/__init__.py
+-rw-r--r--   0        0        0     1331 2024-05-05 11:42:36.859261 gene_trajectory-1.0.1/gene_trajectory/util/download_file.py
+-rw-r--r--   0        0        0     3053 2024-05-05 11:42:36.859261 gene_trajectory-1.0.1/gene_trajectory/util/shared_array.py
+-rw-r--r--   0        0        0       95 2024-05-05 11:42:36.859261 gene_trajectory-1.0.1/gene_trajectory/widgets/__init__.py
+-rw-r--r--   0        0        0     5024 2024-05-05 11:42:36.859261 gene_trajectory-1.0.1/gene_trajectory/widgets/extract_gene_trajectory_widget.py
+-rw-r--r--   0        0        0     1359 2024-05-05 11:42:36.887261 gene_trajectory-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4790 1970-01-01 00:00:00.000000 gene_trajectory-1.0.1/PKG-INFO
```

### Comparing `gene_trajectory-1.0.0/LICENSE` & `gene_trajectory-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gene_trajectory-1.0.0/README.md` & `gene_trajectory-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,27 +9,33 @@
 
 
 Note that, although the implementation is equivalent, it will produce slightly different results to the R implementation
 because the signs of eigenvectors may differ and because of the randomness of K-means during the `coarse_grain` step. 
 
 
 # Install #
-The development version of the package can be installed as 
+The main version of the package can be installed as 
 ```
 pip install gene-trajectory
 ```
 
+If you are planning to run the tool in [Jupyter Notebook](https://jupyter.org/), the additional dependencies can be 
+installed as
+```
+pip install 'gene-trajectory[widgets]'
+```
+
 The development version of the package can be installed as 
 ```
 pip install git+https://github.com/Klugerlab/GeneTrajectory-python.git
 ```
 
 # Tutorials #
 There are tutorials in Jupyter Notebook format in the [online documentation](https://genetrajectory-python.readthedocs.io) 
-and the [notebooks](https://github.com/KlugerLab/GeneTrajectory-python/tree/main/docs/notebooks) folder of the GitHub project. 
+and the [notebooks](https://github.com/KlugerLab/GeneTrajectory-python/tree/main/notebooks) folder of the GitHub project. 
 
 
 # How to cite Gene Trajectory #
 If you use this tool in your research and find it useful, you can cite the following reference from our paper
 [Gene trajectory inference for single-cell data by optimal transport metrics](https://doi.org/10.1038/s41587-024-02186-3).
 In Bibtex format:
 ```bibtex
```

### Comparing `gene_trajectory-1.0.0/gene_trajectory/add_gene_bin_score.py` & `gene_trajectory-1.0.1/gene_trajectory/add_gene_bin_score.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-1.0.0/gene_trajectory/coarse_grain.py` & `gene_trajectory-1.0.1/gene_trajectory/coarse_grain.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-1.0.0/gene_trajectory/compute_gene_distance_cmd.py` & `gene_trajectory-1.0.1/gene_trajectory/compute_gene_distance_cmd.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-1.0.0/gene_trajectory/diffusion_map.py` & `gene_trajectory-1.0.1/gene_trajectory/diffusion_map.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-1.0.0/gene_trajectory/extract_gene_trajectory.py` & `gene_trajectory-1.0.1/gene_trajectory/extract_gene_trajectory.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     pseudoorder_all[subset] = pseudoorder
     return pseudoorder_all
 
 
 def extract_gene_trajectory(
         gene_embedding: pd.DataFrame,
         dist_mat: np.array,
-        gene_names: list,
+        gene_names: list[str],
         t_list: Union[float, np.array, list],
         n: Optional[int] = None,
         dims=5,
         k=10,
         quantile=0.02,
         other: str = 'Other',
 ) -> pd.DataFrame:
```

### Comparing `gene_trajectory-1.0.0/gene_trajectory/gene_distance_shared.py` & `gene_trajectory-1.0.1/gene_trajectory/gene_distance_shared.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-1.0.0/gene_trajectory/get_graph_distance.py` & `gene_trajectory-1.0.1/gene_trajectory/get_graph_distance.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-1.0.0/gene_trajectory/plot/gene_trajectory_plots.py` & `gene_trajectory-1.0.1/gene_trajectory/plot/gene_trajectory_plots.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 import seaborn as sns
 from typing import Iterable, Any
 
 
 def plot_gene_trajectory_3d(
         gene_trajectory: pd.DataFrame,
         s: int = 1,
+        label_genes: Iterable[str] = None,
         **kwargs: Any
 ) -> None:
     """
     Generate a 3D plot of a gene-trajectory object
 
     :param gene_trajectory: a gene trajectory result
     :param s: scatterplot point size (default: 1)
+    :param label_genes: Gene labels to plot (default: None)
     :param kwargs: plot arguments that will be passed to Axes.scatter
     """
     for c in 'DM_1', 'DM_2', 'DM_3', 'selected':
         if c not in gene_trajectory.columns:
             raise ValueError(f'Column {c} is not present in gene trajectory DataFrame')
 
     ax = plt.axes(projection='3d')
@@ -28,55 +30,74 @@
         idxs = selections == c
         ax.scatter(xs=gene_trajectory['DM_1'][idxs],
                    ys=gene_trajectory['DM_2'][idxs],
                    zs=gene_trajectory['DM_3'][idxs],
                    s=s,
                    label=c,
                    **kwargs)
+
+    if label_genes:
+        for g in label_genes:
+            ax.text(x=gene_trajectory['DM_1'][g],
+                    y=gene_trajectory['DM_2'][g],
+                    z=gene_trajectory['DM_3'][g],
+                    s=g)
     ax.legend()
 
 
 def plot_gene_trajectory_2d(
         gene_trajectory: pd.DataFrame,
         s: int = 1,
+        label_genes: Iterable[str] = None,
         **kwargs: Any
 ) -> None:
     """
     Generate a 2D plot of a gene-trajectory object
 
     :param gene_trajectory: a gene trajectory result
     :param s: scatterplot point size (default: 1)
+    :param label_genes: Gene labels to plot (default: None)
     :param kwargs: plot arguments that will be passed to sns.scatterplot
     """
     for c in 'DM_1', 'DM_2', 'selected':
         if c not in gene_trajectory.columns:
             raise ValueError(f'Column {c} is not present in gene trajectory DataFrame')
     sns.scatterplot(data=gene_trajectory,
                     x='DM_1',
                     y='DM_2',
                     hue='selected',
                     s=s,
                     **kwargs)
+    if label_genes:
+        ax = plt.gca()
+        for g in label_genes:
+            ax.text(x=gene_trajectory['DM_1'][g],
+                    y=gene_trajectory['DM_2'][g],
+                    s=g)
 
 
 def plot_gene_trajectory_umap(
         adata: sc.AnnData,
         trajectory: str = 'Trajectory1',
         other_panels: Iterable[str] = (),
+        reverse: bool = False,
         cmap: str = 'RdYlBu_r',
         **kwargs: Any,
 ) -> None:
     """
     Generate a series of umap plot for gene trajectory bins
 
     :param adata: a dataset with gene trajectory metadata
     :param trajectory: the name of the trajectory
     :param other_panels: other panels to be added to the umap
+    :param reverse: reverse the order of the panels
     :param cmap: colormap to be used
     :param kwargs: plot arguments that will be passed to scanpy.pl.umap
     """
     other_panels = [other_panels] if isinstance(other_panels, str) else other_panels
     trajectory_panels = [k for k in adata.obs_keys() if k.startswith(trajectory)]
     if not trajectory_panels:
         raise ValueError(f'No obj metadata found for {trajectory}')
-    panels = [*(k for k in adata.obs_keys() if k.startswith(trajectory)), *other_panels]
+    if reverse:
+        trajectory_panels.reverse()
+    panels = [*trajectory_panels, *other_panels]
     sc.pl.umap(adata, color=panels, cmap=cmap, **kwargs)
```

### Comparing `gene_trajectory-1.0.0/gene_trajectory/run_dm.py` & `gene_trajectory-1.0.1/gene_trajectory/run_dm.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-1.0.0/gene_trajectory/util/download_file.py` & `gene_trajectory-1.0.1/gene_trajectory/util/download_file.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-1.0.0/gene_trajectory/util/shared_array.py` & `gene_trajectory-1.0.1/gene_trajectory/util/shared_array.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-1.0.0/pyproject.toml` & `gene_trajectory-1.0.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "gene-trajectory"
-version = "1.0.0"
+version = "1.0.1"
 description = "Compute gene trajectories"
 license = {file = "LICENSE"}
 readme = "README.md"
 
 authors = [
     {name = "Francesco Strino", email = "francesco.strino@pcmgf.com"},
     {name = "Rihao Qu", email = "rihao.qu@yale.edu"},
@@ -39,13 +39,13 @@
     "scipy>=1.8",
     "seaborn>=0.13",
     "tqdm>=4.64.1",
 ]
 
 [project.optional-dependencies]
 dev = ["pytest", "twine"]
-
+widget = ["ipywidgets>8", "jupyterlab>=4"]
 
 [project.urls]
 Documentation = "https://github.com/KlugerLab/GeneTrajectory-python.git"
 Repository = "https://github.com/KlugerLab/GeneTrajectory-python.git"
 "Bug Tracker" = "https://github.com/KlugerLab/GeneTrajectory-python/issues"
```

### Comparing `gene_trajectory-1.0.0/PKG-INFO` & `gene_trajectory-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gene-trajectory
-Version: 1.0.0
+Version: 1.0.1
 Summary: Compute gene trajectories
 Keywords: Gene trajectory,scRNA-seq
 Author-email: Francesco Strino <francesco.strino@pcmgf.com>, Rihao Qu <rihao.qu@yale.edu>
 Maintainer-email: Francesco Strino <francesco.strino@pcmgf.com>, Rihao Qu <rihao.qu@yale.edu>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
@@ -20,18 +20,21 @@
 Requires-Dist: scikit-misc>=0.1.3
 Requires-Dist: scikit-learn>=0.24
 Requires-Dist: scipy>=1.8
 Requires-Dist: seaborn>=0.13
 Requires-Dist: tqdm>=4.64.1
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: twine ; extra == "dev"
+Requires-Dist: ipywidgets>8 ; extra == "widget"
+Requires-Dist: jupyterlab>=4 ; extra == "widget"
 Project-URL: Bug Tracker, https://github.com/KlugerLab/GeneTrajectory-python/issues
 Project-URL: Documentation, https://github.com/KlugerLab/GeneTrajectory-python.git
 Project-URL: Repository, https://github.com/KlugerLab/GeneTrajectory-python.git
 Provides-Extra: dev
+Provides-Extra: widget
 
 # Python Gene Trajectory
 This package is a Python implementation of GeneTrajectory. 
 The method is described in detail in the article [
 Gene trajectory inference for single-cell data by optimal transport metrics](
 https://doi.org/10.1038/s41587-024-02186-3).
 
@@ -40,27 +43,33 @@
 
 
 Note that, although the implementation is equivalent, it will produce slightly different results to the R implementation
 because the signs of eigenvectors may differ and because of the randomness of K-means during the `coarse_grain` step. 
 
 
 # Install #
-The development version of the package can be installed as 
+The main version of the package can be installed as 
 ```
 pip install gene-trajectory
 ```
 
+If you are planning to run the tool in [Jupyter Notebook](https://jupyter.org/), the additional dependencies can be 
+installed as
+```
+pip install 'gene-trajectory[widgets]'
+```
+
 The development version of the package can be installed as 
 ```
 pip install git+https://github.com/Klugerlab/GeneTrajectory-python.git
 ```
 
 # Tutorials #
 There are tutorials in Jupyter Notebook format in the [online documentation](https://genetrajectory-python.readthedocs.io) 
-and the [notebooks](https://github.com/KlugerLab/GeneTrajectory-python/tree/main/docs/notebooks) folder of the GitHub project. 
+and the [notebooks](https://github.com/KlugerLab/GeneTrajectory-python/tree/main/notebooks) folder of the GitHub project. 
 
 
 # How to cite Gene Trajectory #
 If you use this tool in your research and find it useful, you can cite the following reference from our paper
 [Gene trajectory inference for single-cell data by optimal transport metrics](https://doi.org/10.1038/s41587-024-02186-3).
 In Bibtex format:
 ```bibtex
```

