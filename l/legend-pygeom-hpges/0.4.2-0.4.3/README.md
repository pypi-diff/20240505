# Comparing `tmp/legend_pygeom_hpges-0.4.2.tar.gz` & `tmp/legend_pygeom_hpges-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "legend_pygeom_hpges-0.4.2.tar", last modified: Wed Feb  7 13:46:53 2024, max compression
+gzip compressed data, was "legend_pygeom_hpges-0.4.3.tar", last modified: Sun May  5 12:47:43 2024, max compression
```

## Comparing `legend_pygeom_hpges-0.4.2.tar` & `legend_pygeom_hpges-0.4.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:46:53.887097 legend_pygeom_hpges-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-07 13:46:35.000000 legend_pygeom_hpges-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    43649 2024-02-07 13:46:53.887097 legend_pygeom_hpges-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-02-07 13:46:35.000000 legend_pygeom_hpges-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-02-07 13:46:35.000000 legend_pygeom_hpges-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 13:46:53.887097 legend_pygeom_hpges-0.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:46:53.879097 legend_pygeom_hpges-0.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:46:53.883097 legend_pygeom_hpges-0.4.2/src/legend_pygeom_hpges.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    43649 2024-02-07 13:46:53.000000 legend_pygeom_hpges-0.4.2/src/legend_pygeom_hpges.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-02-07 13:46:53.000000 legend_pygeom_hpges-0.4.2/src/legend_pygeom_hpges.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 13:46:53.000000 legend_pygeom_hpges-0.4.2/src/legend_pygeom_hpges.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 13:46:53.000000 legend_pygeom_hpges-0.4.2/src/legend_pygeom_hpges.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-02-07 13:46:53.000000 legend_pygeom_hpges-0.4.2/src/legend_pygeom_hpges.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-07 13:46:53.000000 legend_pygeom_hpges-0.4.2/src/legend_pygeom_hpges.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:46:53.883097 legend_pygeom_hpges-0.4.2/src/legendhpges/
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-02-07 13:46:35.000000 legend_pygeom_hpges-0.4.2/src/legendhpges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-07 13:46:53.000000 legend_pygeom_hpges-0.4.2/src/legendhpges/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-02-07 13:46:35.000000 legend_pygeom_hpges-0.4.2/src/legendhpges/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-02-07 13:46:35.000000 legend_pygeom_hpges-0.4.2/src/legendhpges/bege.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-02-07 13:46:35.000000 legend_pygeom_hpges-0.4.2/src/legendhpges/draw.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-02-07 13:46:35.000000 legend_pygeom_hpges-0.4.2/src/legendhpges/invcoax.py
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-02-07 13:46:35.000000 legend_pygeom_hpges-0.4.2/src/legendhpges/make_hpge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-02-07 13:46:35.000000 legend_pygeom_hpges-0.4.2/src/legendhpges/materials.py
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-02-07 13:46:35.000000 legend_pygeom_hpges-0.4.2/src/legendhpges/p00664b.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-02-07 13:46:35.000000 legend_pygeom_hpges-0.4.2/src/legendhpges/ppc.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-02-07 13:46:35.000000 legend_pygeom_hpges-0.4.2/src/legendhpges/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-02-07 13:46:35.000000 legend_pygeom_hpges-0.4.2/src/legendhpges/semicoax.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-02-07 13:46:35.000000 legend_pygeom_hpges-0.4.2/src/legendhpges/v02160a.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-02-07 13:46:35.000000 legend_pygeom_hpges-0.4.2/src/legendhpges/v02162b.py
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-02-07 13:46:35.000000 legend_pygeom_hpges-0.4.2/src/legendhpges/v07646a.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:46:53.883097 legend_pygeom_hpges-0.4.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:46:53.883097 legend_pygeom_hpges-0.4.2/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-02-07 13:46:35.000000 legend_pygeom_hpges-0.4.2/tests/configs/P00664B.json
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-02-07 13:46:35.000000 legend_pygeom_hpges-0.4.2/tests/configs/V02160A.json
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-02-07 13:46:35.000000 legend_pygeom_hpges-0.4.2/tests/configs/V02162B.json
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-02-07 13:46:35.000000 legend_pygeom_hpges-0.4.2/tests/configs/V07646A.json
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-02-07 13:46:35.000000 legend_pygeom_hpges-0.4.2/tests/test_det_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-02-07 13:46:35.000000 legend_pygeom_hpges-0.4.2/tests/test_materials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:47:43.342078 legend_pygeom_hpges-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-05 12:47:32.000000 legend_pygeom_hpges-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    43649 2024-05-05 12:47:43.342078 legend_pygeom_hpges-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-05 12:47:32.000000 legend_pygeom_hpges-0.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-05 12:47:32.000000 legend_pygeom_hpges-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 12:47:43.342078 legend_pygeom_hpges-0.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:47:43.334078 legend_pygeom_hpges-0.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:47:43.338078 legend_pygeom_hpges-0.4.3/src/legend_pygeom_hpges.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    43649 2024-05-05 12:47:43.000000 legend_pygeom_hpges-0.4.3/src/legend_pygeom_hpges.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-05 12:47:43.000000 legend_pygeom_hpges-0.4.3/src/legend_pygeom_hpges.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 12:47:43.000000 legend_pygeom_hpges-0.4.3/src/legend_pygeom_hpges.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 12:47:43.000000 legend_pygeom_hpges-0.4.3/src/legend_pygeom_hpges.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-05 12:47:43.000000 legend_pygeom_hpges-0.4.3/src/legend_pygeom_hpges.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-05 12:47:43.000000 legend_pygeom_hpges-0.4.3/src/legend_pygeom_hpges.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:47:43.338078 legend_pygeom_hpges-0.4.3/src/legendhpges/
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-05 12:47:32.000000 legend_pygeom_hpges-0.4.3/src/legendhpges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-05 12:47:43.000000 legend_pygeom_hpges-0.4.3/src/legendhpges/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-05-05 12:47:32.000000 legend_pygeom_hpges-0.4.3/src/legendhpges/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-05 12:47:32.000000 legend_pygeom_hpges-0.4.3/src/legendhpges/bege.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-05 12:47:32.000000 legend_pygeom_hpges-0.4.3/src/legendhpges/draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-05 12:47:32.000000 legend_pygeom_hpges-0.4.3/src/legendhpges/invcoax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-05 12:47:32.000000 legend_pygeom_hpges-0.4.3/src/legendhpges/make_hpge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-05 12:47:32.000000 legend_pygeom_hpges-0.4.3/src/legendhpges/materials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-05-05 12:47:32.000000 legend_pygeom_hpges-0.4.3/src/legendhpges/p00664b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-05 12:47:32.000000 legend_pygeom_hpges-0.4.3/src/legendhpges/ppc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-05 12:47:32.000000 legend_pygeom_hpges-0.4.3/src/legendhpges/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-05 12:47:32.000000 legend_pygeom_hpges-0.4.3/src/legendhpges/semicoax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-05 12:47:32.000000 legend_pygeom_hpges-0.4.3/src/legendhpges/v02160a.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-05-05 12:47:32.000000 legend_pygeom_hpges-0.4.3/src/legendhpges/v02162b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-05-05 12:47:32.000000 legend_pygeom_hpges-0.4.3/src/legendhpges/v07646a.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:47:43.338078 legend_pygeom_hpges-0.4.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:47:43.338078 legend_pygeom_hpges-0.4.3/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-05 12:47:32.000000 legend_pygeom_hpges-0.4.3/tests/configs/P00664B.json
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-05 12:47:32.000000 legend_pygeom_hpges-0.4.3/tests/configs/V02160A.json
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-05 12:47:32.000000 legend_pygeom_hpges-0.4.3/tests/configs/V02162B.json
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-05 12:47:32.000000 legend_pygeom_hpges-0.4.3/tests/configs/V07646A.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-05 12:47:32.000000 legend_pygeom_hpges-0.4.3/tests/test_det_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-05 12:47:32.000000 legend_pygeom_hpges-0.4.3/tests/test_materials.py
```

### Comparing `legend_pygeom_hpges-0.4.2/LICENSE` & `legend_pygeom_hpges-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `legend_pygeom_hpges-0.4.2/PKG-INFO` & `legend_pygeom_hpges-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: legend_pygeom_hpges
-Version: 0.4.2
+Version: 0.4.3
 Summary: Geometry management for LEGEND HPGE detectors
 Author-email: Luigi Pertoldi <gipert@pm.me>
 Maintainer: The LEGEND Collaboration
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `legend_pygeom_hpges-0.4.2/README.md` & `legend_pygeom_hpges-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `legend_pygeom_hpges-0.4.2/pyproject.toml` & `legend_pygeom_hpges-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `legend_pygeom_hpges-0.4.2/src/legend_pygeom_hpges.egg-info/PKG-INFO` & `legend_pygeom_hpges-0.4.3/src/legend_pygeom_hpges.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: legend_pygeom_hpges
-Version: 0.4.2
+Version: 0.4.3
 Summary: Geometry management for LEGEND HPGE detectors
 Author-email: Luigi Pertoldi <gipert@pm.me>
 Maintainer: The LEGEND Collaboration
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `legend_pygeom_hpges-0.4.2/src/legend_pygeom_hpges.egg-info/SOURCES.txt` & `legend_pygeom_hpges-0.4.3/src/legend_pygeom_hpges.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `legend_pygeom_hpges-0.4.2/src/legendhpges/base.py` & `legend_pygeom_hpges-0.4.3/src/legendhpges/base.py`

 * *Files identical despite different names*

### Comparing `legend_pygeom_hpges-0.4.2/src/legendhpges/bege.py` & `legend_pygeom_hpges-0.4.3/src/legendhpges/bege.py`

 * *Files identical despite different names*

### Comparing `legend_pygeom_hpges-0.4.2/src/legendhpges/draw.py` & `legend_pygeom_hpges-0.4.3/src/legendhpges/draw.py`

 * *Files identical despite different names*

### Comparing `legend_pygeom_hpges-0.4.2/src/legendhpges/invcoax.py` & `legend_pygeom_hpges-0.4.3/src/legendhpges/invcoax.py`

 * *Files identical despite different names*

### Comparing `legend_pygeom_hpges-0.4.2/src/legendhpges/make_hpge.py` & `legend_pygeom_hpges-0.4.3/src/legendhpges/make_hpge.py`

 * *Files identical despite different names*

### Comparing `legend_pygeom_hpges-0.4.2/src/legendhpges/materials.py` & `legend_pygeom_hpges-0.4.3/src/legendhpges/materials.py`

 * *Files identical despite different names*

### Comparing `legend_pygeom_hpges-0.4.2/src/legendhpges/p00664b.py` & `legend_pygeom_hpges-0.4.3/src/legendhpges/p00664b.py`

 * *Files identical despite different names*

### Comparing `legend_pygeom_hpges-0.4.2/src/legendhpges/ppc.py` & `legend_pygeom_hpges-0.4.3/src/legendhpges/ppc.py`

 * *Files identical despite different names*

### Comparing `legend_pygeom_hpges-0.4.2/src/legendhpges/semicoax.py` & `legend_pygeom_hpges-0.4.3/src/legendhpges/semicoax.py`

 * *Files identical despite different names*

### Comparing `legend_pygeom_hpges-0.4.2/src/legendhpges/v02160a.py` & `legend_pygeom_hpges-0.4.3/src/legendhpges/v02160a.py`

 * *Files identical despite different names*

### Comparing `legend_pygeom_hpges-0.4.2/src/legendhpges/v02162b.py` & `legend_pygeom_hpges-0.4.3/src/legendhpges/v02162b.py`

 * *Files identical despite different names*

### Comparing `legend_pygeom_hpges-0.4.2/src/legendhpges/v07646a.py` & `legend_pygeom_hpges-0.4.3/src/legendhpges/v07646a.py`

 * *Files identical despite different names*

### Comparing `legend_pygeom_hpges-0.4.2/tests/configs/P00664B.json` & `legend_pygeom_hpges-0.4.3/tests/configs/P00664B.json`

 * *Files identical despite different names*

### Comparing `legend_pygeom_hpges-0.4.2/tests/configs/V02160A.json` & `legend_pygeom_hpges-0.4.3/tests/configs/V02160A.json`

 * *Files identical despite different names*

### Comparing `legend_pygeom_hpges-0.4.2/tests/configs/V02162B.json` & `legend_pygeom_hpges-0.4.3/tests/configs/V02162B.json`

 * *Files identical despite different names*

### Comparing `legend_pygeom_hpges-0.4.2/tests/configs/V07646A.json` & `legend_pygeom_hpges-0.4.3/tests/configs/V07646A.json`

 * *Files identical despite different names*

### Comparing `legend_pygeom_hpges-0.4.2/tests/test_det_profile.py` & `legend_pygeom_hpges-0.4.3/tests/test_det_profile.py`

 * *Files identical despite different names*

### Comparing `legend_pygeom_hpges-0.4.2/tests/test_materials.py` & `legend_pygeom_hpges-0.4.3/tests/test_materials.py`

 * *Files identical despite different names*

