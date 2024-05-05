# Comparing `tmp/avn-0.4.0.tar.gz` & `tmp/avn-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avn-0.4.0.tar", max compression
+gzip compressed data, was "avn-0.5.0.tar", max compression
```

## Comparing `avn-0.4.0.tar` & `avn-0.5.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0       23 2024-04-01 15:26:16.987651 avn-0.4.0/avn/__init__.py
--rw-r--r--   0        0        0    54839 2023-03-10 20:46:13.255520 avn-0.4.0/avn/acoustics.py
--rw-r--r--   0        0        0        0 2021-05-05 18:05:55.900000 avn-0.4.0/avn/avn.py
--rw-r--r--   0        0        0     7864 2023-12-14 19:33:37.323506 avn-0.4.0/avn/dataloading.py
--rw-r--r--   0        0        0    14928 2021-11-04 18:21:52.806620 avn-0.4.0/avn/plotting.py
--rw-r--r--   0        0        0    83983 2023-03-02 15:05:22.932147 avn-0.4.0/avn/segmentation.py
--rw-r--r--   0        0        0    90270 2023-03-10 20:40:35.473692 avn-0.4.0/avn/syntax.py
--rw-r--r--   0        0        0    34081 2023-12-15 21:05:06.690502 avn-0.4.0/avn/timing.py
--rw-r--r--   0        0        0        2 2021-04-28 15:46:50.000000 avn-0.4.0/LICENSE
--rw-r--r--   0        0        0      878 2024-04-01 15:25:39.847897 avn-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1275 2021-05-13 15:54:00.000000 avn-0.4.0/README.md
--rw-r--r--   0        0        0     2170 1970-01-01 00:00:00.000000 avn-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       23 2024-05-05 18:50:43.847140 avn-0.5.0/avn/__init__.py
+-rw-r--r--   0        0        0    54839 2024-05-03 17:23:44.188360 avn-0.5.0/avn/acoustics.py
+-rw-r--r--   0        0        0        0 2021-05-05 18:05:55.900000 avn-0.5.0/avn/avn.py
+-rw-r--r--   0        0        0     7864 2024-05-03 19:22:15.718186 avn-0.5.0/avn/dataloading.py
+-rw-r--r--   0        0        0    14928 2021-11-04 18:21:52.806620 avn-0.5.0/avn/plotting.py
+-rw-r--r--   0        0        0    83983 2023-03-02 15:05:22.932147 avn-0.5.0/avn/segmentation.py
+-rw-r--r--   0        0        0    16984 2024-05-04 22:06:46.883614 avn-0.5.0/avn/similarity.py
+-rw-r--r--   0        0        0    90270 2023-03-10 20:40:35.473692 avn-0.5.0/avn/syntax.py
+-rw-r--r--   0        0        0    34081 2024-05-03 19:22:15.719186 avn-0.5.0/avn/timing.py
+-rw-r--r--   0        0        0        2 2021-04-28 15:46:50.000000 avn-0.5.0/LICENSE
+-rw-r--r--   0        0        0      871 2024-05-05 18:50:23.387488 avn-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1373 2024-05-03 19:22:15.717198 avn-0.5.0/README.md
+-rw-r--r--   0        0        0     2260 1970-01-01 00:00:00.000000 avn-0.5.0/PKG-INFO
```

### Comparing `avn-0.4.0/avn/acoustics.py` & `avn-0.5.0/avn/acoustics.py`

 * *Files identical despite different names*

### Comparing `avn-0.4.0/avn/dataloading.py` & `avn-0.5.0/avn/dataloading.py`

 * *Files identical despite different names*

### Comparing `avn-0.4.0/avn/plotting.py` & `avn-0.5.0/avn/plotting.py`

 * *Files identical despite different names*

### Comparing `avn-0.4.0/avn/segmentation.py` & `avn-0.5.0/avn/segmentation.py`

 * *Files identical despite different names*

### Comparing `avn-0.4.0/avn/syntax.py` & `avn-0.5.0/avn/syntax.py`

 * *Files identical despite different names*

### Comparing `avn-0.4.0/avn/timing.py` & `avn-0.5.0/avn/timing.py`

 * *Files identical despite different names*

### Comparing `avn-0.4.0/pyproject.toml` & `avn-0.5.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "avn"
-version = "0.4.0"
+version = "0.5.0"
 description = "Package for zebra finch song analysis."
 authors = ["Therese Koch"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 documentation = "https://avn.readthedocs.io/en/latest/"
 homepage = "https://github.com/theresekoch/avn"
 repository = "https://github.com/theresekoch/avn"
 
 [tool.poetry.dependencies]
 python = ">=3.7.1,<3.10"
 pandas = ">=1.3.3"
-numpy = ">=1.20.2,<1.21.0"
+numpy = ">=1.20.2"
 scikit-learn = "^0.24.2"
 matplotlib = "^3.4.1"
 scipy = "^1.6.3"
-librosa = "0.8.0"
+librosa = "0.10.2"
 seaborn = "^0.11.2"
 more_itertools = "^8.5.0"
 
 [tool.poetry.dev-dependencies]
 Sphinx = "^4.0.1"
 nbsphinx = "^0.8.4"
 ipykernel = "^5.5.4"
```

### Comparing `avn-0.4.0/README.md` & `avn-0.5.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # avn 
 
 [![Python](https://img.shields.io/badge/python-3.9-blue)]()
 [![codecov](https://codecov.io/gh/theresekoch/avn/branch/main/graph/badge.svg)](https://codecov.io/gh/theresekoch/avn)
 [![Documentation Status](https://readthedocs.org/projects/avn/badge/?version=latest)](https://avn.readthedocs.io/en/latest/?badge=latest)
+[![DOI](https://zenodo.org/badge/362525428.svg)](https://zenodo.org/doi/10.5281/zenodo.10938742)
 
 `avn` (Avian Vocalization Network, pronounced 'avian') is a python package for zebra finch song analysis. It currently provides functions
 necessary for threshold-based song segmentation into syllables, with plans for more features in the future. 
 
 ## Installation
 
 ```bash
```

### Comparing `avn-0.4.0/PKG-INFO` & `avn-0.5.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: avn
-Version: 0.4.0
+Version: 0.5.0
 Summary: Package for zebra finch song analysis.
 Home-page: https://github.com/theresekoch/avn
 License: GNU General Public License v3.0
 Author: Therese Koch
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: librosa (==0.8.0)
+Requires-Dist: librosa (==0.10.2)
 Requires-Dist: matplotlib (>=3.4.1,<4.0.0)
 Requires-Dist: more_itertools (>=8.5.0,<9.0.0)
-Requires-Dist: numpy (>=1.20.2,<1.21.0)
+Requires-Dist: numpy (>=1.20.2)
 Requires-Dist: pandas (>=1.3.3)
 Requires-Dist: scikit-learn (>=0.24.2,<0.25.0)
 Requires-Dist: scipy (>=1.6.3,<2.0.0)
 Requires-Dist: seaborn (>=0.11.2,<0.12.0)
 Project-URL: Documentation, https://avn.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/theresekoch/avn
 Description-Content-Type: text/markdown
 
 # avn 
 
 [![Python](https://img.shields.io/badge/python-3.9-blue)]()
 [![codecov](https://codecov.io/gh/theresekoch/avn/branch/main/graph/badge.svg)](https://codecov.io/gh/theresekoch/avn)
 [![Documentation Status](https://readthedocs.org/projects/avn/badge/?version=latest)](https://avn.readthedocs.io/en/latest/?badge=latest)
+[![DOI](https://zenodo.org/badge/362525428.svg)](https://zenodo.org/doi/10.5281/zenodo.10938742)
 
 `avn` (Avian Vocalization Network, pronounced 'avian') is a python package for zebra finch song analysis. It currently provides functions
 necessary for threshold-based song segmentation into syllables, with plans for more features in the future. 
 
 ## Installation
 
 ```bash
```

