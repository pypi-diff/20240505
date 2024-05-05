# Comparing `tmp/stacci-0.9.5.tar.gz` & `tmp/stacci-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stacci-0.9.5.tar", max compression
+gzip compressed data, was "stacci-0.9.6.tar", max compression
```

## Comparing `stacci-0.9.5.tar` & `stacci-0.9.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     6538 2024-04-12 08:06:34.968381 stacci-0.9.5/README.md
--rw-r--r--   0        0        0      166 2024-03-15 15:29:04.555776 stacci-0.9.5/STACCI/__init__.py
--rw-r--r--   0        0        0    39940 2024-03-15 15:22:41.667792 stacci-0.9.5/STACCI/ccci.py
--rw-r--r--   0        0        0    10212 2024-03-15 16:51:31.767571 stacci-0.9.5/STACCI/data_handler.py
--rw-r--r--   0        0        0     6378 2024-03-15 16:45:15.675586 stacci-0.9.5/STACCI/model.py
--rw-r--r--   0        0        0     6734 2024-03-29 08:19:04.442599 stacci-0.9.5/STACCI/pipeline.py
--rw-r--r--   0        0        0    65268 2024-03-15 15:22:41.667792 stacci-0.9.5/STACCI/pl.py
--rw-r--r--   0        0        0     5219 2024-03-15 15:22:41.667792 stacci-0.9.5/STACCI/tl.py
--rw-r--r--   0        0        0     3765 2024-03-15 16:46:00.507584 stacci-0.9.5/STACCI/trainer.py
--rw-r--r--   0        0        0    32812 2024-03-29 08:35:18.818558 stacci-0.9.5/STACCI/utils.py
--rw-r--r--   0        0        0      773 2024-04-12 07:48:02.180427 stacci-0.9.5/pyproject.toml
--rw-r--r--   0        0        0     7930 1970-01-01 00:00:00.000000 stacci-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0     6538 2024-05-05 11:26:32.981330 stacci-0.9.6/README.md
+-rw-r--r--   0        0        0      166 2024-03-15 15:29:04.555776 stacci-0.9.6/STACCI/__init__.py
+-rw-r--r--   0        0        0    39940 2024-03-15 15:22:41.667792 stacci-0.9.6/STACCI/ccci.py
+-rw-r--r--   0        0        0    10212 2024-03-15 16:51:31.767571 stacci-0.9.6/STACCI/data_handler.py
+-rw-r--r--   0        0        0     6378 2024-03-15 16:45:15.675586 stacci-0.9.6/STACCI/model.py
+-rw-r--r--   0        0        0     6734 2024-03-29 08:19:04.442599 stacci-0.9.6/STACCI/pipeline.py
+-rw-r--r--   0        0        0    65268 2024-03-15 15:22:41.667792 stacci-0.9.6/STACCI/pl.py
+-rw-r--r--   0        0        0     5434 2024-05-05 12:21:10.449194 stacci-0.9.6/STACCI/tl.py
+-rw-r--r--   0        0        0     3765 2024-03-15 16:46:00.507584 stacci-0.9.6/STACCI/trainer.py
+-rw-r--r--   0        0        0    32812 2024-03-29 08:35:18.818558 stacci-0.9.6/STACCI/utils.py
+-rw-r--r--   0        0        0      789 2024-05-05 12:47:33.277128 stacci-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0     7955 1970-01-01 00:00:00.000000 stacci-0.9.6/PKG-INFO
```

### Comparing `stacci-0.9.5/README.md` & `stacci-0.9.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
       `pip install torch_geometric`
 4. Install `mclust` in R environment
 
    Enter `R` in bash to enter the command line interactive interface and install `mclust` with this command:
    `install.packages("mclust")`
    During the installation process, select CRAN mirror: China (Beijing 3) [https].
 
-   After the installation is done, enter the command `library(mclust)` to load. If the `mclust` logo is displayed, it means the installation is successful. You can press `ctrl+d` to exit R.
+   After the installation is done, enter the command `library(mclust)` to load. If the `mclust` logo is displayed, it means the installation is successful. You can press `Ctrl+d` to exit R.
 5. `pip install STACCI`
 
 ## Usage Instructions
 
 After creating a new environment according to the installation instructions and installing the corresponding dependencies, place the .h5ad file of the dataset in the specified file structure, specifically, the desired file structure of the dataset is as follows:
 
 ```bash
```

### Comparing `stacci-0.9.5/STACCI/ccci.py` & `stacci-0.9.6/STACCI/ccci.py`

 * *Files identical despite different names*

### Comparing `stacci-0.9.5/STACCI/data_handler.py` & `stacci-0.9.6/STACCI/data_handler.py`

 * *Files identical despite different names*

### Comparing `stacci-0.9.5/STACCI/model.py` & `stacci-0.9.6/STACCI/model.py`

 * *Files identical despite different names*

### Comparing `stacci-0.9.5/STACCI/pipeline.py` & `stacci-0.9.6/STACCI/pipeline.py`

 * *Files identical despite different names*

### Comparing `stacci-0.9.5/STACCI/pl.py` & `stacci-0.9.6/STACCI/pl.py`

 * *Files identical despite different names*

### Comparing `stacci-0.9.5/STACCI/tl.py` & `stacci-0.9.6/STACCI/tl.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,23 @@
 import matplotlib.pyplot as plt
 from kneed import KneeLocator
 import seaborn as sns
 from scipy.stats import hypergeom
 
 ## A. inflection point finding
 def Inflection_point_finding(adata,  col='weight', vis=False):
-    df = adata.uns['LRP_weight']
+    # df = adata.uns['LRP_weight']
+    if isinstance(adata, str):
+        df = pd.read_csv(adata)
+        data = df[col].values
+    elif isinstance(adata, np.ndarray):
+        data = adata
+    else:
+        df = adata
+        data = df[col].values
     data = df[col].values
     data_idx = np.arange(len(data))
     kneedle = KneeLocator(data_idx,
                           data,
                           curve='convex',
                           direction='decreasing',
                           online=True)
```

### Comparing `stacci-0.9.5/STACCI/trainer.py` & `stacci-0.9.6/STACCI/trainer.py`

 * *Files identical despite different names*

### Comparing `stacci-0.9.5/STACCI/utils.py` & `stacci-0.9.6/STACCI/utils.py`

 * *Files identical despite different names*

### Comparing `stacci-0.9.5/pyproject.toml` & `stacci-0.9.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [tool.poetry]
 name = "STACCI"
-version = "0.9.5"
+version = "0.9.6"
 description = "STACCI for STCase"
 authors = ["Lzcstan <lzcstan@outlook.com>"]
 readme = "README.md"
 packages = [
   { include = "STACCI", from = "." },
 ]
 
 [tool.poetry.dependencies]
+ipykernel = "*"
 scipy = "*"
 scikit-learn = "*"
 scikit-misc = "*"
 anndata = "*"
 matplotlib = "*"
 pandas = "*"
 scanpy = "*"
```

### Comparing `stacci-0.9.5/PKG-INFO` & `stacci-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: STACCI
-Version: 0.9.5
+Version: 0.9.6
 Summary: STACCI for STCase
 Author: Lzcstan
 Author-email: lzcstan@outlook.com
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: anndata
 Requires-Dist: arboreto
 Requires-Dist: ctxcore
+Requires-Dist: ipykernel
 Requires-Dist: kneed
 Requires-Dist: leidenalg
 Requires-Dist: louvain
 Requires-Dist: matplotlib
 Requires-Dist: netgraph
 Requires-Dist: pandas
 Requires-Dist: plotnine
@@ -110,15 +111,15 @@
       `pip install torch_geometric`
 4. Install `mclust` in R environment
 
    Enter `R` in bash to enter the command line interactive interface and install `mclust` with this command:
    `install.packages("mclust")`
    During the installation process, select CRAN mirror: China (Beijing 3) [https].
 
-   After the installation is done, enter the command `library(mclust)` to load. If the `mclust` logo is displayed, it means the installation is successful. You can press `ctrl+d` to exit R.
+   After the installation is done, enter the command `library(mclust)` to load. If the `mclust` logo is displayed, it means the installation is successful. You can press `Ctrl+d` to exit R.
 5. `pip install STACCI`
 
 ## Usage Instructions
 
 After creating a new environment according to the installation instructions and installing the corresponding dependencies, place the .h5ad file of the dataset in the specified file structure, specifically, the desired file structure of the dataset is as follows:
 
 ```bash
```

