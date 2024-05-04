# Comparing `tmp/mustache_hic-1.3.2.tar.gz` & `tmp/mustache_hic-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mustache_hic-1.3.2.tar", last modified: Tue Aug 29 17:54:08 2023, max compression
+gzip compressed data, was "mustache_hic-1.3.3.tar", last modified: Sat May  4 23:13:45 2024, max compression
```

## Comparing `mustache_hic-1.3.2.tar` & `mustache_hic-1.3.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 abbas      (501) staff       (20)        0 2023-08-29 17:54:08.865998 mustache_hic-1.3.2/
--rwxr-xr-x   0 abbas      (501) staff       (20)     1072 2023-08-29 17:48:08.000000 mustache_hic-1.3.2/LICENSE.txt
--rw-r--r--   0 abbas      (501) staff       (20)      565 2023-08-29 17:54:08.865880 mustache_hic-1.3.2/PKG-INFO
--rw-r--r--   0 abbas      (501) staff       (20)    11817 2023-08-29 17:48:08.000000 mustache_hic-1.3.2/README.md
-drwxr-xr-x   0 abbas      (501) staff       (20)        0 2023-08-29 17:54:08.864855 mustache_hic-1.3.2/mustache/
--rw-r--r--   0 abbas      (501) staff       (20)        0 2023-08-29 17:48:08.000000 mustache_hic-1.3.2/mustache/__init__.py
--rw-r--r--   0 abbas      (501) staff       (20)       33 2023-08-29 17:48:08.000000 mustache_hic-1.3.2/mustache/__main__.py
--rw-r--r--   0 abbas      (501) staff       (20)       22 2023-08-29 17:53:48.000000 mustache_hic-1.3.2/mustache/_version.py
--rwxr-xr-x   0 abbas      (501) staff       (20)    35462 2023-08-29 17:48:08.000000 mustache_hic-1.3.2/mustache/diff_mustache.py
--rwxr-xr-x   0 abbas      (501) staff       (20)    40302 2023-08-29 17:48:08.000000 mustache_hic-1.3.2/mustache/mustache.py
-drwxr-xr-x   0 abbas      (501) staff       (20)        0 2023-08-29 17:54:08.865727 mustache_hic-1.3.2/mustache_hic.egg-info/
--rw-r--r--   0 abbas      (501) staff       (20)      565 2023-08-29 17:54:08.000000 mustache_hic-1.3.2/mustache_hic.egg-info/PKG-INFO
--rw-r--r--   0 abbas      (501) staff       (20)      393 2023-08-29 17:54:08.000000 mustache_hic-1.3.2/mustache_hic.egg-info/SOURCES.txt
--rw-r--r--   0 abbas      (501) staff       (20)        1 2023-08-29 17:54:08.000000 mustache_hic-1.3.2/mustache_hic.egg-info/dependency_links.txt
--rw-r--r--   0 abbas      (501) staff       (20)       52 2023-08-29 17:54:08.000000 mustache_hic-1.3.2/mustache_hic.egg-info/entry_points.txt
--rw-r--r--   0 abbas      (501) staff       (20)        1 2023-08-29 17:54:08.000000 mustache_hic-1.3.2/mustache_hic.egg-info/not-zip-safe
--rw-r--r--   0 abbas      (501) staff       (20)       65 2023-08-29 17:54:08.000000 mustache_hic-1.3.2/mustache_hic.egg-info/requires.txt
--rw-r--r--   0 abbas      (501) staff       (20)        9 2023-08-29 17:54:08.000000 mustache_hic-1.3.2/mustache_hic.egg-info/top_level.txt
--rw-r--r--   0 abbas      (501) staff       (20)       38 2023-08-29 17:54:08.866040 mustache_hic-1.3.2/setup.cfg
--rw-r--r--   0 abbas      (501) staff       (20)     1148 2023-08-29 17:48:08.000000 mustache_hic-1.3.2/setup.py
+drwxr-xr-x   0 abbas      (501) staff       (20)        0 2024-05-04 23:13:45.875035 mustache_hic-1.3.3/
+-rwxr-xr-x   0 abbas      (501) staff       (20)     1072 2024-04-27 19:45:43.000000 mustache_hic-1.3.3/LICENSE.txt
+-rw-r--r--   0 abbas      (501) staff       (20)      584 2024-05-04 23:13:45.874909 mustache_hic-1.3.3/PKG-INFO
+-rw-r--r--   0 abbas      (501) staff       (20)    11817 2024-04-29 22:17:42.000000 mustache_hic-1.3.3/README.md
+drwxr-xr-x   0 abbas      (501) staff       (20)        0 2024-05-04 23:13:45.873345 mustache_hic-1.3.3/mustache/
+-rw-r--r--   0 abbas      (501) staff       (20)        0 2024-04-27 19:45:43.000000 mustache_hic-1.3.3/mustache/__init__.py
+-rw-r--r--   0 abbas      (501) staff       (20)       33 2024-04-27 19:45:43.000000 mustache_hic-1.3.3/mustache/__main__.py
+-rw-r--r--   0 abbas      (501) staff       (20)       22 2024-04-29 22:15:32.000000 mustache_hic-1.3.3/mustache/_version.py
+-rwxr-xr-x   0 abbas      (501) staff       (20)    35462 2024-04-27 19:45:43.000000 mustache_hic-1.3.3/mustache/diff_mustache.py
+-rwxr-xr-x   0 abbas      (501) staff       (20)    40561 2024-04-29 22:22:40.000000 mustache_hic-1.3.3/mustache/mustache.py
+drwxr-xr-x   0 abbas      (501) staff       (20)        0 2024-05-04 23:13:45.874722 mustache_hic-1.3.3/mustache_hic.egg-info/
+-rw-r--r--   0 abbas      (501) staff       (20)      584 2024-05-04 23:13:45.000000 mustache_hic-1.3.3/mustache_hic.egg-info/PKG-INFO
+-rw-r--r--   0 abbas      (501) staff       (20)      393 2024-05-04 23:13:45.000000 mustache_hic-1.3.3/mustache_hic.egg-info/SOURCES.txt
+-rw-r--r--   0 abbas      (501) staff       (20)        1 2024-05-04 23:13:45.000000 mustache_hic-1.3.3/mustache_hic.egg-info/dependency_links.txt
+-rw-r--r--   0 abbas      (501) staff       (20)       52 2024-05-04 23:13:45.000000 mustache_hic-1.3.3/mustache_hic.egg-info/entry_points.txt
+-rw-r--r--   0 abbas      (501) staff       (20)        1 2024-04-29 22:22:55.000000 mustache_hic-1.3.3/mustache_hic.egg-info/not-zip-safe
+-rw-r--r--   0 abbas      (501) staff       (20)       65 2024-05-04 23:13:45.000000 mustache_hic-1.3.3/mustache_hic.egg-info/requires.txt
+-rw-r--r--   0 abbas      (501) staff       (20)        9 2024-05-04 23:13:45.000000 mustache_hic-1.3.3/mustache_hic.egg-info/top_level.txt
+-rw-r--r--   0 abbas      (501) staff       (20)       38 2024-05-04 23:13:45.875085 mustache_hic-1.3.3/setup.cfg
+-rw-r--r--   0 abbas      (501) staff       (20)     1148 2024-04-27 19:45:43.000000 mustache_hic-1.3.3/setup.py
```

### Comparing `mustache_hic-1.3.2/LICENSE.txt` & `mustache_hic-1.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mustache_hic-1.3.2/PKG-INFO` & `mustache_hic-1.3.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: mustache_hic
-Version: 1.3.2
+Version: 1.3.3
 Summary: Mustache is a Hi-C analysis tool
 Home-page: http://github.com/ay-lab/mustache/
 Author: Ferhat Ay
 Author-email: ferhatay@lji.org
 License: MIT
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 License-File: LICENSE.txt
 
 Mustache is a tool for multi-scale detection of chromatin loops from Hi-C and Micro-C contact maps in high resolutions (10kbp all the way to 500bp and even more).
+
```

### Comparing `mustache_hic-1.3.2/README.md` & `mustache_hic-1.3.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Mustache <img src="images/mustache.png" width="100"> [![PyPI Latest Release](https://img.shields.io/badge/PYPI-v1.3.1-blue)](https://pypi.org/project/mustache-hic/) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4046958.svg)](https://doi.org/10.5281/zenodo.4046958)
+# Mustache <img src="images/mustache.png" width="100"> [![PyPI Latest Release](https://img.shields.io/badge/PYPI-v1.3.3-blue)](https://pypi.org/project/mustache-hic/) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4046958.svg)](https://doi.org/10.5281/zenodo.4046958)
 
 
 Mustache (Multi-scale Detection of Chromatin Loops from Hi-C and Micro-C Maps using Scale-Space Representation) is a tool by Abbas Roayaei Ardakany, Halil Tuvan Gezer, Stefano Lonardi and Ferhat Ay (ferhatay@lji.org).
 
 Mustache is a tool for multi-scale detection of chromatin loops from Hi-C and Micro-C contact maps in high resolutions (10kbp all the way to 500bp and even more). Mustache uses recent technical advances in scale-space theory in Computer Vision to detect chromatin loops caused by interaction of DNA segments with a variable size. Here is an example of Mustache loops detected for HFFc6 Micro-C in 1kb resolution (loops are enlarged):
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # Mustache [images/mustache.png][![PyPI Latest Release](https://img.shields.io/
-badge/PYPI-v1.3.1-blue)](https://pypi.org/project/mustache-hic/) [![License:
+badge/PYPI-v1.3.3-blue)](https://pypi.org/project/mustache-hic/) [![License:
 MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://
 opensource.org/licenses/MIT) [![DOI](https://zenodo.org/badge/DOI/10.5281/
 zenodo.4046958.svg)](https://doi.org/10.5281/zenodo.4046958) Mustache (Multi-
 scale Detection of Chromatin Loops from Hi-C and Micro-C Maps using Scale-Space
 Representation) is a tool by Abbas Roayaei Ardakany, Halil Tuvan Gezer, Stefano
 Lonardi and Ferhat Ay (ferhatay@lji.org). Mustache is a tool for multi-scale
 detection of chromatin loops from Hi-C and Micro-C contact maps in high
```

### Comparing `mustache_hic-1.3.2/mustache/diff_mustache.py` & `mustache_hic-1.3.3/mustache/diff_mustache.py`

 * *Files identical despite different names*

### Comparing `mustache_hic-1.3.2/mustache/mustache.py` & `mustache_hic-1.3.3/mustache/mustache.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,15 +306,19 @@
     """
     if not CHRM_SIZE:
         hic = hicstraw.HiCFile(f)
         chromosomes = hic.getChromosomes()
         chrSize_in_bp = {}
         for i in range(1, len(chromosomes)):
             chrSize_in_bp["chr" + str(chromosomes[i].name).replace("chr", '')] = chromosomes[i].length
-        CHRM_SIZE = chrSize_in_bp["chr" + chr1.replace("chr", '')]
+        chr_key = "chr" + chr1.replace("chr", '')
+        if chr_key in chrSize_in_bp:
+            CHRM_SIZE = chrSize_in_bp[chr_key]
+        else:
+            raise NameError('wrong chromosome name!')
 
     CHUNK_SIZE = max(2 * distance_in_bp / res, 2000)
     start = 0
     end = min(CHRM_SIZE, CHUNK_SIZE * res)  # CHUNK_SIZE*res
     result = []
     val = []
 
@@ -346,20 +350,26 @@
             to_add_list = list(cur_block - prev_block)
             del prev_block
             result[0] += [x[0] for x in to_add_list]
             result[1] += [x[1] for x in to_add_list]
             result[2] += [x[2] for x in to_add_list]
             prev_block = cur_block
             del cur_block
+
+
         start = min(start + CHUNK_SIZE * res - distance_in_bp, CHRM_SIZE)
         if end == CHRM_SIZE - 1:
             break
         else:
             end = min(end + CHUNK_SIZE * res - distance_in_bp, CHRM_SIZE - 1)
 
+    if len(result) == 0:
+        print(f'There is no contact in chrmosome {chr1} to work on.')
+        return [], [], []
+
     x = np.array(result[0]) // res
     y = np.array(result[1]) // res
     val = np.array(result[2])
 
     nan_indx = np.logical_or.reduce((np.isnan(result[0]), np.isnan(result[1]), np.isnan(result[2])))
     x = x[~nan_indx]
     y = y[~nan_indx]
```

### Comparing `mustache_hic-1.3.2/mustache_hic.egg-info/PKG-INFO` & `mustache_hic-1.3.3/mustache_hic.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: mustache-hic
-Version: 1.3.2
+Version: 1.3.3
 Summary: Mustache is a Hi-C analysis tool
 Home-page: http://github.com/ay-lab/mustache/
 Author: Ferhat Ay
 Author-email: ferhatay@lji.org
 License: MIT
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 License-File: LICENSE.txt
 
 Mustache is a tool for multi-scale detection of chromatin loops from Hi-C and Micro-C contact maps in high resolutions (10kbp all the way to 500bp and even more).
+
```

### Comparing `mustache_hic-1.3.2/setup.py` & `mustache_hic-1.3.3/setup.py`

 * *Files identical despite different names*

