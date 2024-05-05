# Comparing `tmp/delaunay_triangulation_and_its_dual_2d-0.1.0.tar.gz` & `tmp/delaunay_triangulation_and_its_dual_2d-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delaunay_triangulation_and_its_dual_2d-0.1.0.tar", last modified: Sun May  5 03:35:31 2024, max compression
+gzip compressed data, was "delaunay_triangulation_and_its_dual_2d-0.1.1.tar", last modified: Sun May  5 03:49:32 2024, max compression
```

## Comparing `delaunay_triangulation_and_its_dual_2d-0.1.0.tar` & `delaunay_triangulation_and_its_dual_2d-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 03:35:31.091246 delaunay_triangulation_and_its_dual_2d-0.1.0/
--rw-rw-rw-   0        0        0     3318 2024-05-05 03:33:40.000000 delaunay_triangulation_and_its_dual_2d-0.1.0/.gitignore
--rw-rw-rw-   0        0        0     1086 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     6089 2024-05-05 03:35:31.090246 delaunay_triangulation_and_its_dual_2d-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4084 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 03:35:31.071400 delaunay_triangulation_and_its_dual_2d-0.1.0/assets/
--rw-rw-rw-   0        0        0    66443 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.0/assets/time_to_compute_voronoi_tessellation.png
-drwxrwxrwx   0        0        0        0 2024-05-05 03:35:31.075739 delaunay_triangulation_and_its_dual_2d-0.1.0/delaunay_triangulation_and_its_dual_2d/
--rw-rw-rw-   0        0        0       32 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.0/delaunay_triangulation_and_its_dual_2d/__init__.py
--rw-rw-rw-   0        0        0      427 2024-05-05 03:35:30.000000 delaunay_triangulation_and_its_dual_2d-0.1.0/delaunay_triangulation_and_its_dual_2d/_version.py
--rw-rw-rw-   0        0        0    17840 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.0/delaunay_triangulation_and_its_dual_2d/delaunay.py
--rw-rw-rw-   0        0        0       58 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.0/delaunay_triangulation_and_its_dual_2d/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-05 03:35:31.086248 delaunay_triangulation_and_its_dual_2d-0.1.0/delaunay_triangulation_and_its_dual_2d/geometry/
--rw-rw-rw-   0        0        0      142 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.0/delaunay_triangulation_and_its_dual_2d/geometry/__init__.py
--rw-rw-rw-   0        0        0     1673 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.0/delaunay_triangulation_and_its_dual_2d/geometry/bounding_box_2d.py
--rw-rw-rw-   0        0        0      220 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.0/delaunay_triangulation_and_its_dual_2d/geometry/centroid.py
--rw-rw-rw-   0        0        0     2758 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.0/delaunay_triangulation_and_its_dual_2d/geometry/circumcircle.py
-drwxrwxrwx   0        0        0        0 2024-05-05 03:35:31.087247 delaunay_triangulation_and_its_dual_2d-0.1.0/delaunay_triangulation_and_its_dual_2d/util/
--rw-rw-rw-   0        0        0       65 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.0/delaunay_triangulation_and_its_dual_2d/util/__init__.py
--rw-rw-rw-   0        0        0      865 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.0/delaunay_triangulation_and_its_dual_2d/util/scipy_spatial_mocked.py
-drwxrwxrwx   0        0        0        0 2024-05-05 03:35:31.089246 delaunay_triangulation_and_its_dual_2d-0.1.0/delaunay_triangulation_and_its_dual_2d.egg-info/
--rw-rw-rw-   0        0        0     6089 2024-05-05 03:35:30.000000 delaunay_triangulation_and_its_dual_2d-0.1.0/delaunay_triangulation_and_its_dual_2d.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1066 2024-05-05 03:35:31.000000 delaunay_triangulation_and_its_dual_2d-0.1.0/delaunay_triangulation_and_its_dual_2d.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 03:35:30.000000 delaunay_triangulation_and_its_dual_2d-0.1.0/delaunay_triangulation_and_its_dual_2d.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2024-05-05 03:35:30.000000 delaunay_triangulation_and_its_dual_2d-0.1.0/delaunay_triangulation_and_its_dual_2d.egg-info/requires.txt
--rw-rw-rw-   0        0        0       39 2024-05-05 03:35:30.000000 delaunay_triangulation_and_its_dual_2d-0.1.0/delaunay_triangulation_and_its_dual_2d.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1319 2024-05-05 03:33:48.000000 delaunay_triangulation_and_its_dual_2d-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-05 03:35:31.091246 delaunay_triangulation_and_its_dual_2d-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-05 03:35:31.064247 delaunay_triangulation_and_its_dual_2d-0.1.0/tests/
-drwxrwxrwx   0        0        0        0 2024-05-05 03:35:31.089246 delaunay_triangulation_and_its_dual_2d-0.1.0/tests/delaunay/
--rw-rw-rw-   0        0        0     2484 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.0/tests/delaunay/performance.py
--rw-rw-rw-   0        0        0      481 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.0/tests/delaunay/profiling.py
--rw-rw-rw-   0        0        0     6111 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.0/tests/delaunay/test_all.py
+drwxrwxrwx   0        0        0        0 2024-05-05 03:49:32.885347 delaunay_triangulation_and_its_dual_2d-0.1.1/
+-rw-rw-rw-   0        0        0     3318 2024-05-05 03:33:40.000000 delaunay_triangulation_and_its_dual_2d-0.1.1/.gitignore
+-rw-rw-rw-   0        0        0     1086 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     6062 2024-05-05 03:49:32.884345 delaunay_triangulation_and_its_dual_2d-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4084 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 03:49:32.869367 delaunay_triangulation_and_its_dual_2d-0.1.1/assets/
+-rw-rw-rw-   0        0        0    66443 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.1/assets/time_to_compute_voronoi_tessellation.png
+drwxrwxrwx   0        0        0        0 2024-05-05 03:49:32.873339 delaunay_triangulation_and_its_dual_2d-0.1.1/delaunay_triangulation_and_its_dual_2d/
+-rw-rw-rw-   0        0        0       32 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.1/delaunay_triangulation_and_its_dual_2d/__init__.py
+-rw-rw-rw-   0        0        0      427 2024-05-05 03:49:32.000000 delaunay_triangulation_and_its_dual_2d-0.1.1/delaunay_triangulation_and_its_dual_2d/_version.py
+-rw-rw-rw-   0        0        0    17840 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.1/delaunay_triangulation_and_its_dual_2d/delaunay.py
+-rw-rw-rw-   0        0        0       58 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.1/delaunay_triangulation_and_its_dual_2d/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-05 03:49:32.880339 delaunay_triangulation_and_its_dual_2d-0.1.1/delaunay_triangulation_and_its_dual_2d/geometry/
+-rw-rw-rw-   0        0        0      142 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.1/delaunay_triangulation_and_its_dual_2d/geometry/__init__.py
+-rw-rw-rw-   0        0        0     1673 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.1/delaunay_triangulation_and_its_dual_2d/geometry/bounding_box_2d.py
+-rw-rw-rw-   0        0        0      220 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.1/delaunay_triangulation_and_its_dual_2d/geometry/centroid.py
+-rw-rw-rw-   0        0        0     2758 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.1/delaunay_triangulation_and_its_dual_2d/geometry/circumcircle.py
+drwxrwxrwx   0        0        0        0 2024-05-05 03:49:32.881339 delaunay_triangulation_and_its_dual_2d-0.1.1/delaunay_triangulation_and_its_dual_2d/util/
+-rw-rw-rw-   0        0        0       65 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.1/delaunay_triangulation_and_its_dual_2d/util/__init__.py
+-rw-rw-rw-   0        0        0      865 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.1/delaunay_triangulation_and_its_dual_2d/util/scipy_spatial_mocked.py
+drwxrwxrwx   0        0        0        0 2024-05-05 03:49:32.883347 delaunay_triangulation_and_its_dual_2d-0.1.1/delaunay_triangulation_and_its_dual_2d.egg-info/
+-rw-rw-rw-   0        0        0     6062 2024-05-05 03:49:32.000000 delaunay_triangulation_and_its_dual_2d-0.1.1/delaunay_triangulation_and_its_dual_2d.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1066 2024-05-05 03:49:32.000000 delaunay_triangulation_and_its_dual_2d-0.1.1/delaunay_triangulation_and_its_dual_2d.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 03:49:32.000000 delaunay_triangulation_and_its_dual_2d-0.1.1/delaunay_triangulation_and_its_dual_2d.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2024-05-05 03:49:32.000000 delaunay_triangulation_and_its_dual_2d-0.1.1/delaunay_triangulation_and_its_dual_2d.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       39 2024-05-05 03:49:32.000000 delaunay_triangulation_and_its_dual_2d-0.1.1/delaunay_triangulation_and_its_dual_2d.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1305 2024-05-05 03:40:21.000000 delaunay_triangulation_and_its_dual_2d-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-05 03:49:32.885347 delaunay_triangulation_and_its_dual_2d-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-05 03:49:32.866334 delaunay_triangulation_and_its_dual_2d-0.1.1/tests/
+drwxrwxrwx   0        0        0        0 2024-05-05 03:49:32.883347 delaunay_triangulation_and_its_dual_2d-0.1.1/tests/delaunay/
+-rw-rw-rw-   0        0        0     2484 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.1/tests/delaunay/performance.py
+-rw-rw-rw-   0        0        0      481 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.1/tests/delaunay/profiling.py
+-rw-rw-rw-   0        0        0     6180 2024-05-05 03:48:22.000000 delaunay_triangulation_and_its_dual_2d-0.1.1/tests/delaunay/test_all.py
```

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.0/.gitignore` & `delaunay_triangulation_and_its_dual_2d-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.0/LICENSE` & `delaunay_triangulation_and_its_dual_2d-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.0/PKG-INFO` & `delaunay_triangulation_and_its_dual_2d-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delaunay-triangulation-and-its-dual-2d
-Version: 0.1.0
+Version: 0.1.1
 License: MIT License
         
         Copyright (c) 2024 M.H. Luk
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -24,15 +24,14 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/dailyideas/delaunay-triangulation-and-its-dual-2d
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: scipy>=0.12.0
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Provides-Extra: dist
 Requires-Dist: build; extra == "dist"
 Requires-Dist: twine; extra == "dist"
```

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.0/README.md` & `delaunay_triangulation_and_its_dual_2d-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.0/assets/time_to_compute_voronoi_tessellation.png` & `delaunay_triangulation_and_its_dual_2d-0.1.1/assets/time_to_compute_voronoi_tessellation.png`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.0/delaunay_triangulation_and_its_dual_2d/delaunay.py` & `delaunay_triangulation_and_its_dual_2d-0.1.1/delaunay_triangulation_and_its_dual_2d/delaunay.py`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.0/delaunay_triangulation_and_its_dual_2d/geometry/bounding_box_2d.py` & `delaunay_triangulation_and_its_dual_2d-0.1.1/delaunay_triangulation_and_its_dual_2d/geometry/bounding_box_2d.py`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.0/delaunay_triangulation_and_its_dual_2d/geometry/circumcircle.py` & `delaunay_triangulation_and_its_dual_2d-0.1.1/delaunay_triangulation_and_its_dual_2d/geometry/circumcircle.py`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.0/delaunay_triangulation_and_its_dual_2d/util/scipy_spatial_mocked.py` & `delaunay_triangulation_and_its_dual_2d-0.1.1/delaunay_triangulation_and_its_dual_2d/util/scipy_spatial_mocked.py`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.0/delaunay_triangulation_and_its_dual_2d.egg-info/PKG-INFO` & `delaunay_triangulation_and_its_dual_2d-0.1.1/delaunay_triangulation_and_its_dual_2d.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delaunay-triangulation-and-its-dual-2d
-Version: 0.1.0
+Version: 0.1.1
 License: MIT License
         
         Copyright (c) 2024 M.H. Luk
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -24,15 +24,14 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/dailyideas/delaunay-triangulation-and-its-dual-2d
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: scipy>=0.12.0
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Provides-Extra: dist
 Requires-Dist: build; extra == "dist"
 Requires-Dist: twine; extra == "dist"
```

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.0/delaunay_triangulation_and_its_dual_2d.egg-info/SOURCES.txt` & `delaunay_triangulation_and_its_dual_2d-0.1.1/delaunay_triangulation_and_its_dual_2d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.0/pyproject.toml` & `delaunay_triangulation_and_its_dual_2d-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools>=64", "setuptools_scm>=8"]
 
 [project]
 classifiers = ["Programming Language :: Python :: 3"]
-dependencies = ["matplotlib", "numpy", "scipy>=0.12.0"]
+dependencies = ["numpy", "scipy>=0.12.0"]
 dynamic = ["version"]
 license = { file = "LICENSE" }
 name = "delaunay-triangulation-and-its-dual-2d"
 readme = "README.md"
 requires-python = ">=3.8"
 
 [project.optional-dependencies]
```

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.0/tests/delaunay/performance.py` & `delaunay_triangulation_and_its_dual_2d-0.1.1/tests/delaunay/performance.py`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.0/tests/delaunay/test_all.py` & `delaunay_triangulation_and_its_dual_2d-0.1.1/tests/delaunay/test_all.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 from numpy.typing import NDArray
 import pytest
 import scipy
 import scipy.spatial
 
 import delaunay_triangulation_and_its_dual_2d
+import delaunay_triangulation_and_its_dual_2d.exceptions
 
 
 def _sort_rows(array: NDArray) -> NDArray:
     return array[np.lexsort(array.T[::-1])]
 
 
 def _sort_columns_of_each_row_then_sort_rows(array: NDArray) -> NDArray:
@@ -190,10 +191,10 @@
 def test_compute_voronoi_diagram_raises_duplicated_circumcenters_error():
     points = np.array(
         [[0, 0], [1, 0], [1, 1], [0, 1]],
         dtype=np.float32,
     )
     delaunay = delaunay_triangulation_and_its_dual_2d.Delaunay(points=points)
     with pytest.raises(
-        delaunay_triangulation_and_its_dual_2d.DuplicatedCircumcentersError
+        delaunay_triangulation_and_its_dual_2d.exceptions.DuplicatedCircumcentersError
     ):
         delaunay.compute_voronoi_tessellation()
```

