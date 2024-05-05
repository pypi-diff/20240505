# Comparing `tmp/magpylib_force-0.1.6.tar.gz` & `tmp/magpylib_force-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magpylib_force-0.1.6.tar", last modified: Fri Apr 19 22:41:22 2024, max compression
+gzip compressed data, was "magpylib_force-0.1.7.tar", last modified: Sun May  5 05:57:04 2024, max compression
```

## Comparing `magpylib_force-0.1.6.tar` & `magpylib_force-0.1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:41:22.098961 magpylib_force-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-19 22:41:18.000000 magpylib_force-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-19 22:41:22.098961 magpylib_force-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-19 22:41:18.000000 magpylib_force-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:41:22.098961 magpylib_force-0.1.6/magpylib_force/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-19 22:41:18.000000 magpylib_force-0.1.6/magpylib_force/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-04-19 22:41:18.000000 magpylib_force-0.1.6/magpylib_force/force.py
--rw-r--r--   0 runner    (1001) docker     (127)     4881 2024-04-19 22:41:18.000000 magpylib_force-0.1.6/magpylib_force/mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-19 22:41:18.000000 magpylib_force-0.1.6/magpylib_force/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:41:22.098961 magpylib_force-0.1.6/magpylib_force.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-19 22:41:22.000000 magpylib_force-0.1.6/magpylib_force.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-19 22:41:22.000000 magpylib_force-0.1.6/magpylib_force.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 22:41:22.000000 magpylib_force-0.1.6/magpylib_force.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 22:41:22.000000 magpylib_force-0.1.6/magpylib_force.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-19 22:41:22.000000 magpylib_force-0.1.6/magpylib_force.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 22:41:22.098961 magpylib_force-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-19 22:41:18.000000 magpylib_force-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:41:22.098961 magpylib_force-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 22:41:18.000000 magpylib_force-0.1.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-19 22:41:18.000000 magpylib_force-0.1.6/tests/test_FEM.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-19 22:41:18.000000 magpylib_force-0.1.6/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-19 22:41:18.000000 magpylib_force-0.1.6/tests/test_meshing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-04-19 22:41:18.000000 magpylib_force-0.1.6/tests/test_physics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-04-19 22:41:18.000000 magpylib_force-0.1.6/tests/test_self_consistency.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 05:57:04.515523 magpylib_force-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-05 05:56:58.000000 magpylib_force-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-05 05:57:04.515523 magpylib_force-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-05 05:56:58.000000 magpylib_force-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 05:57:04.515523 magpylib_force-0.1.7/magpylib_force/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-05 05:56:58.000000 magpylib_force-0.1.7/magpylib_force/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-05-05 05:56:58.000000 magpylib_force-0.1.7/magpylib_force/force.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-05-05 05:56:58.000000 magpylib_force-0.1.7/magpylib_force/meshing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-05 05:56:58.000000 magpylib_force-0.1.7/magpylib_force/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 05:57:04.515523 magpylib_force-0.1.7/magpylib_force.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-05 05:57:04.000000 magpylib_force-0.1.7/magpylib_force.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-05 05:57:04.000000 magpylib_force-0.1.7/magpylib_force.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 05:57:04.000000 magpylib_force-0.1.7/magpylib_force.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-05 05:57:04.000000 magpylib_force-0.1.7/magpylib_force.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-05 05:57:04.000000 magpylib_force-0.1.7/magpylib_force.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 05:57:04.515523 magpylib_force-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-05 05:56:58.000000 magpylib_force-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 05:57:04.515523 magpylib_force-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 05:56:58.000000 magpylib_force-0.1.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13390 2024-05-05 05:56:58.000000 magpylib_force-0.1.7/tests/test_FEM.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-05 05:56:58.000000 magpylib_force-0.1.7/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-05 05:56:58.000000 magpylib_force-0.1.7/tests/test_meshing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-05-05 05:56:58.000000 magpylib_force-0.1.7/tests/test_physics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-05-05 05:56:58.000000 magpylib_force-0.1.7/tests/test_self_consistency.py
```

### Comparing `magpylib_force-0.1.6/LICENSE` & `magpylib_force-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `magpylib_force-0.1.6/PKG-INFO` & `magpylib_force-0.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: magpylib-force
-Version: 0.1.6
+Version: 0.1.7
 Summary: An extension to the Magpylib library, providing force computation
-Home-page: https://github.com/magpylib/magpylib-material-response
-Author: Alexandre Boisselet
+Home-page: https://github.com/magpylib/magpylib-force
+Author: Magpylib
 Author-email: magpylib@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
```

### Comparing `magpylib_force-0.1.6/README.md` & `magpylib_force-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `magpylib_force-0.1.6/magpylib_force/force.py` & `magpylib_force-0.1.7/magpylib_force/force.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,96 @@
 import numpy as np
 import magpylib as magpy
-from magpylib_force.mesh import mesh_cuboid
+from magpylib_force.meshing import mesh_cuboid
 from magpylib_force.utility import check_input_anchor
-from magpylib_force.utility import check_input_targets_Cuboid
-from magpylib_force.utility import check_input_targets_Polyline
+from magpylib_force.utility import check_input_targets
+from magpylib._src.obj_classes.class_current_Polyline import Polyline
+from magpylib._src.obj_classes.class_magnet_Cuboid import Cuboid
+
+
+def getFT(sources, targets, anchor=None, eps=1e-5, squeeze=True):
+    """
+    Compute force and torque between sources and targets.
+    SI units are assumed for all inputs and outputs.
+
+    Parameters
+    ----------
+    sources: source and collection objects or 1D list thereof
+        Sources that generate the magnetic field. Can be a single source (or collection)
+        or a 1D list of l sources and/or collection objects.
+
+    targets: single object or 1D list of t objects that are in [Cuboid, Polyline]
+        Force and Torque acting on targets in the magnetic field generated by the sources
+        will be computed. A target must have a valid `meshing` parameter.
+    
+    eps: float, default=1e-5
+        For magnet-targets the magnetic field gradient is computed using finite
+        differences (FD). `eps` is the FD step size. A good value
+        is 1e-5 * characteristic system size (magnet size, distance between sources
+        and targets, ...).
+
+    anchor: array_like, default=None
+        The Force adds to the Torque via the anchor point. For a freely floating magnet
+        this would be the barycenter. If `anchor=None`, this part of the Torque computation
+        is ommitted.
+
+    squeeze: bool, default=True
+        The output of the computation has the shape (n,3) where n corresponds to the number
+        of targets. By default this is reduced to (3,) when there is only one target.
+
+    Returns
+    -------
+    Force-Torque as ndarray of shape (2,3), of (t,2,3) when t targets are given
+    """
+    anchor = check_input_anchor(anchor)
+    targets = check_input_targets(targets)
+    # MISSING: allow Collections
+
+    n = len(targets)
+
+    cuboids, order_cub = [], []
+    polylines, order_poly = [], []
+    for i,t in enumerate(targets):
+        if isinstance(t, Cuboid):
+            cuboids.append(t)
+            order_cub.append(i)
+        elif isinstance(t, Polyline):
+            polylines.append(t)
+            order_poly.append(i)
+
+    FT = np.zeros((n, 2, 3))
+    if cuboids:
+        FT_cube = getFTcube(sources, cuboids, eps=eps, anchor=anchor, squeeze=False)
+        FT_cube = np.swapaxes(FT_cube, 0, 1)
+        for ft,o in zip(FT_cube, order_cub):
+            FT[o] = ft
+    if polylines:
+        FT_poly = getFTwire(sources, polylines, anchor=anchor, squeeze=False)
+        FT_poly = np.swapaxes(FT_poly, 0, 1)
+        for ft,o in zip(FT_poly, order_poly):
+            FT[o] = ft
+    #FT = np.swapaxes(FT, 0, 1)
+    if squeeze:
+        return np.squeeze(FT)
+    return FT
 
 
 def getFTcube(sources, targets, eps=1e-5, anchor=None, squeeze=True):
     """
     Compute force and torque acting on a Cuboid magnet.
 
     Parameters
     ----------
     sources: source and collection objects or 1D list thereof
         Sources that generate the magnetic field. Can be a single source (or collection)
         or a 1D list of l sources and/or collection objects.
 
     targets: Cuboid object or 1D list of Cuboid objects
         Force and Torque acting on targets in the magnetic field generated by the sources
-        will be computed. A target must have a valid mesh parameter.
+        will be computed. A target must have a valid `meshing` parameter.
     
     eps: float, default=1e-5
         The magnetic field gradient is computed using finite differences (FD). eps is
         the FD step size. A good value is 1e-5 * characteristic system size (magnet size,
         distance between sources and targets, ...).
     
     anchor: array_like, default=None
@@ -30,23 +98,20 @@
         this would be the barycenter. If `anchor=None`, this part of the Torque computation
         is ommitted.
 
     squeeze: bool, default=True
         The output of the computation has the shape (n,3) where n corresponds to the number
         of targets. By default this is reduced to (3,) when there is only one target.
     """
-    anchor = check_input_anchor(anchor)
-    targets = check_input_targets_Cuboid(targets)
-    # MISSING: allow Collections
 
     # number of Cuboids
     tgt_number = len(targets)
 
     # number of instances of each Cuboid
-    inst_numbers = np.array([np.prod(tgt.mesh) for tgt in targets])
+    inst_numbers = np.array([np.prod(tgt.meshing) for tgt in targets])
 
     # total number of instances
     no_inst = np.sum(inst_numbers)
 
     # cumsum of number of instances (used for indexing)
     insti = np.r_[0, np.cumsum(inst_numbers)]
 
@@ -81,40 +146,36 @@
     T = np.array([np.sum(Ts[insti[i]:insti[i+1]],axis=0) for i in range(tgt_number)])
     F = np.array([np.sum(Fs[insti[i]:insti[i+1]],axis=0) for i in range(tgt_number)])
 
     if squeeze:
         F = np.squeeze(F)
         T = np.squeeze(T)
 
-    return F, T
+    return np.array((F, T))
 
 
 
 def getFTwire(sources, targets, anchor=None, squeeze=True):
     """
     compute force acting on tgt Polyline
 
     info:
     targets = Polyline objects
     segements = linear segments within Polyline objects
-    instances = computation instances, each segment is split into `mesh` points
+    instances = computation instances, each segment is split into `meshing` points
     """
 
-    anchor = check_input_anchor(anchor)
-    targets = check_input_targets_Polyline(targets)
-    # MISSING: allow Collections
-
     # number of Polylines
     tgt_number = len(targets)
 
     # segments of each Polyline
     seg_numbers = np.array([len(tgt.vertices)-1 for tgt in targets])
 
     # number of mesh-points of each Polyline
-    mesh_numbers = np.array([tgt.mesh for tgt in targets])
+    mesh_numbers = np.array([tgt.meshing for tgt in targets])
 
     # number of instances of each Polyline
     inst_numbers = seg_numbers*mesh_numbers
 
     # total number of instances
     no_inst = np.sum(inst_numbers)
 
@@ -148,18 +209,18 @@
     F = (CURR * np.cross(LVEC, B).T).T
 
     # torque on every instance + sumup for every target
     if anchor is not None:
         T = np.cross(anchor - POSS, F)
         T = np.array([np.sum(T[insti[i]:insti[i+1]],axis=0) for i in range(tgt_number)])
     else:
-        T = np.zeros((tgt_number,))
+        T = np.zeros((tgt_number,3))
 
     # sumup force for every target
     F = np.array([np.sum(F[insti[i]:insti[i+1]],axis=0) for i in range(tgt_number)])
 
     # squeeze output
     if squeeze:
         F = np.squeeze(F)
         T = np.squeeze(T)
 
-    return F, T
+    return np.array((F, T))
```

### Comparing `magpylib_force-0.1.6/magpylib_force/mesh.py` & `magpylib_force-0.1.7/magpylib_force/meshing.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 def mesh_cuboid(object):
     """
     splits cuboid into given mesh
     returns grid positions relative to cuboid position
     """
     a,b,c = object.dimension
-    n1,n2,n3 = object.mesh
+    n1,n2,n3 = object.meshing
     xs = np.linspace(-a/2, a/2, n1+1)
     ys = np.linspace(-b/2, b/2, n2+1)
     zs = np.linspace(-c/2, c/2, n3+1)
 
     dx = xs[1] - xs[0] if len(xs)>1 else a
     dy = ys[1] - ys[0] if len(ys)>1 else b
     dz = zs[1] - zs[0] if len(zs)>1 else c
@@ -48,15 +48,15 @@
         Print resulting mesh parameters
 
     Returns
     -------
     grid positions: np.ndarray shape (m,3)
     """
     a,b,c = object.dimension
-    splitting = object.mesh
+    splitting = object.meshing
     if isinstance(splitting, (float, int)):
         x = (a*b*c/splitting)**(1/3)
         n1 = m.ceil(a/x)
         n2 = m.ceil(b/x)
         n3 = m.ceil(c/x)
     else:
         n1,n2,n3 = np.array(splitting)+1
```

### Comparing `magpylib_force-0.1.6/magpylib_force.egg-info/PKG-INFO` & `magpylib_force-0.1.7/magpylib_force.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: magpylib-force
-Version: 0.1.6
+Version: 0.1.7
 Summary: An extension to the Magpylib library, providing force computation
-Home-page: https://github.com/magpylib/magpylib-material-response
-Author: Alexandre Boisselet
+Home-page: https://github.com/magpylib/magpylib-force
+Author: Magpylib
 Author-email: magpylib@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
```

### Comparing `magpylib_force-0.1.6/setup.py` & `magpylib_force-0.1.7/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 
 setup(
     name="magpylib-force",
     version=version,
     description=_short_description,
     long_description=readme_text,
     long_description_content_type="text/markdown",
-    author="Alexandre Boisselet",
+    author="Magpylib",
     author_email="magpylib@gmail.com",
-    url=("https://github.com/" "magpylib/magpylib-material-response"),
+    url=("https://github.com/" "magpylib/magpylib-force"),
     license="MIT",
     packages=find_packages(),
     # include anything specified in Manifest.in
     install_requires=requirements,
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "License :: OSI Approved :: BSD License",
```

### Comparing `magpylib_force-0.1.6/tests/test_interface.py` & `magpylib_force-0.1.7/tests/test_interface.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 import numpy as np
 import magpylib as magpy
-from magpylib_force.force import getFTcube
-from magpylib_force.force import getFTwire
+from magpylib_force.force import getFT
 
-def test_getFTwire_target_inputs_01():
+
+def test_getFT_target_inputs_01():
     """
     check different target and source input formats give same
     """
     src1 = magpy.magnet.Sphere(polarization=(1,2,3), diameter=1)
     src2 = src1.copy()
     wire1 = magpy.current.Polyline(
         current=1,
         vertices=((2,0,0),(-2,2,2),(-2,-2,-2)),
     )
     wire2 = wire1.copy()
     wire3 = wire1.copy()
-    wire1.mesh=20
-    wire2.mesh=20
-    wire3.mesh=20
+    wire1.meshing=20
+    wire2.meshing=20
+    wire3.meshing=20
 
-    F1,T1 = getFTwire(src1, wire1, anchor=(0,0,0))
-    F2,T2 = getFTwire(src1, [wire1], anchor=(0,0,0))
-    F3,T3 = getFTwire(src1, [wire1,wire2,wire3], anchor=(0,0,0))
-    np.testing.assert_allclose(F1,F2)
-    np.testing.assert_allclose(F1,F3[0])
-    np.testing.assert_allclose(F1,F3[1])
-    np.testing.assert_allclose(F1,F3[2])
+    FT1 = getFT(src1, wire1, anchor=(0,0,0))
+    FT2 = getFT(src1, [wire1], anchor=(0,0,0))
+    FT3 = getFT(src1, [wire1,wire2,wire3], anchor=(0,0,0))
     
-    np.testing.assert_allclose(T1,T2)
-    np.testing.assert_allclose(T1,T3[0])
-    np.testing.assert_allclose(T1,T3[1])
-    np.testing.assert_allclose(T1,T3[2])
+    np.testing.assert_allclose(FT1,FT2)
+    np.testing.assert_allclose(FT1,FT3[0])
+    np.testing.assert_allclose(FT1,FT3[1])
+    np.testing.assert_allclose(FT1,FT3[2])
 
-    F4,T4 = getFTwire(src1, wire1, anchor=(0,0,0))
-    F5,T5 = getFTwire([src1, src2], wire1, anchor=(0,0,0))
+    FT4 = getFT(src1, wire1, anchor=(0,0,0))
+    FT5 = getFT([src1, src2], wire1, anchor=(0,0,0))
     
-    np.testing.assert_allclose(F4*2,F5)
-    np.testing.assert_allclose(T4*2,T5)
+    np.testing.assert_allclose(FT4*2,FT5)
+    np.testing.assert_allclose(FT4*2,FT5)
```

### Comparing `magpylib_force-0.1.6/tests/test_meshing.py` & `magpylib_force-0.1.7/tests/test_meshing.py`

 * *Files identical despite different names*

### Comparing `magpylib_force-0.1.6/tests/test_physics.py` & `magpylib_force-0.1.7/tests/test_physics.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import numpy as np
 import magpylib as magpy
-from magpylib_force.force import getFTcube
-from magpylib_force.force import getFTwire
+from magpylib_force.force import getFT
 
 
 # def test_physics_loop_torque():
 #     """
 #     for a current loop in a homogeneous field the following holds
 #     F = 0
 #     T = current * loop_surface * field_normal_component
@@ -13,50 +12,50 @@
 #     # circular loop
 #     ts = np.linspace(0,2*np.pi,300)
 #     verts = [(np.sin(t), np.cos(t), 0) for t in ts]
 #     cloop = magpy.current.Polyline(
 #         current=(1, "A"),
 #         vertices=(verts, "m"),
 #     )
-#     cloop.mesh = 1
+#     cloop.meshing = 1
 
 #     # homogeneous field
 #     def func(field, observers):
 #         return np.zeros_like(observers, dtype=float) + np.array((1,0,0))
 #     hom = magpy.misc.CustomSource(field_func=func)
 
 #     # without anchor
-#     F,T = getFTwire(hom, cloop, Tanch=None)
+#     F,T = getFT(hom, cloop, Tanch=None)
 #     assert np.amax(F.magnitude) < 1e-14
 #     assert T.magnitude == 0
 
 #     # with anchor
-#     F,T = getFTwire(hom, cloop, Tanch=cloop.position)
+#     F,T = getFT(hom, cloop, Tanch=cloop.position)
 #     assert np.amax(abs(F.magnitude)) < 1e-14
 #     assert abs(T[0].magnitude) < 1e-14
 #     assert abs(T[1].magnitude - np.pi ) < 1e-3
 #     assert abs(T[2].magnitude) < 1e-14
 
 #     ##############################################################
 
 #     # rectangular loop
 #     verts = [(-1,-1,0), (1,-1,0), (1,1,0), (-1,1,0), (-1,-1,0)]
 #     rloop = magpy.current.Polyline(
 #         current=(1, "A"),
 #         vertices=(verts, "m"),
 #     )
-#     rloop.mesh = 10
+#     rloop.meshing = 10
 
 #     # without anchor
-#     F,T = getFTwire(hom, rloop, Tanch=None)
+#     F,T = getFT(hom, rloop, Tanch=None)
 #     assert np.amax(F.magnitude) < 1e-14
 #     assert T.magnitude == 0
 
 #     # with anchor
-#     F,T = getFTwire(hom, rloop, Tanch=rloop.position)
+#     F,T = getFT(hom, rloop, Tanch=rloop.position)
 #     assert np.amax(abs(F.magnitude)) < 1e-14
 #     assert abs(T[0].magnitude) < 1e-14
 #     assert abs(T[1].magnitude + 4 ) < 1e-3
 #     assert abs(T[2].magnitude) < 1e-14
 
 def test_physics_loop_torque():
     """
@@ -67,50 +66,50 @@
     # circular loop
     ts = np.linspace(0,2*np.pi,300)
     verts = [(np.sin(t), np.cos(t), 0) for t in ts]
     cloop = magpy.current.Polyline(
         current=1,
         vertices=verts,
     )
-    cloop.mesh = 1
+    cloop.meshing = 1
 
     # homogeneous field
     def func(field, observers):
         return np.zeros_like(observers, dtype=float) + np.array((1,0,0))
     hom = magpy.misc.CustomSource(field_func=func)
 
     # without anchor
-    F,T = getFTwire(hom, cloop, anchor=None)
-    assert np.amax(F) < 1e-14
-    assert T == 0
+    F,T = getFT(hom, cloop, anchor=None)
+    assert np.amax(abs(F)) < 1e-14
+    assert np.amax(abs(T)) == 0
 
     # with anchor
-    F,T = getFTwire(hom, cloop, anchor=cloop.position)
+    F,T = getFT(hom, cloop, anchor=cloop.position)
     assert np.amax(abs(F)) < 1e-14
     assert abs(T[0]) < 1e-14
     assert abs(T[1] - np.pi ) < 1e-3
     assert abs(T[2]) < 1e-14
 
     ##############################################################
 
     # rectangular loop
     verts = [(-1,-1,0), (1,-1,0), (1,1,0), (-1,1,0), (-1,-1,0)]
     rloop = magpy.current.Polyline(
         current=1,
         vertices=verts,
     )
-    rloop.mesh = 10
+    rloop.meshing = 10
 
     # without anchor
-    F,T = getFTwire(hom, rloop, anchor=None)
-    assert np.amax(F) < 1e-14
-    assert T == 0
+    F,T = getFT(hom, rloop, anchor=None)
+    assert np.amax(abs(F)) < 1e-14
+    assert np.amax(abs(T)) == 0
 
     # with anchor
-    F,T = getFTwire(hom, rloop, anchor=rloop.position)
+    F,T = getFT(hom, rloop, anchor=rloop.position)
     assert np.amax(abs(F)) < 1e-14
     assert abs(T[0]) < 1e-14
     assert abs(T[1] + 4 ) < 1e-3
     assert abs(T[2]) < 1e-14
 
 
 # def test_physics_parallel_wires():
@@ -123,17 +122,17 @@
 #         vertices=([(-1000,0,0),(1000,0,0)], "m"),
 #     )
 #     tgt = magpy.current.Polyline(
 #         current=(1, "A"),
 #         vertices=([(-1000,0,0),(0,0,0),(1000,0,0)], "m"),
 #         position=((0,0,1), "m"),
 #     )
-#     tgt.mesh = 1000
+#     tgt.meshing = 1000
 
-#     F,_ = getFTwire(src, tgt)
+#     F,_ = getFT(src, tgt)
 
 #     Fanalytic = 2*magpy.mu_0/4/np.pi*2000
 
 #     assert abs(F[0].magnitude) < 1e-14
 #     assert abs(F[1].magnitude) < 1e-14
 #     assert abs((F[2].magnitude + Fanalytic)/Fanalytic) < 1e-3
 
@@ -143,17 +142,17 @@
     F = 2*mu0/4/pi * i1*i2/r
     """
     wire1 = magpy.current.Polyline(
         current=1,
         vertices=[(-1000,0,0),(1000,0,0)],
     )
     wire2 = wire1.copy(position=(0,0,1))
-    wire2.mesh = 1000
+    wire2.meshing = 1000
 
-    F,_ = getFTwire(wire1, wire2)
+    F,_ = getFT(wire1, wire2)
 
     Fanalytic = 2*magpy.mu_0/4/np.pi*2000
 
     assert abs(F[0]) < 1e-14
     assert abs(F[1]) < 1e-14
     assert abs((F[2]+Fanalytic)/Fanalytic) < 1e-3
 
@@ -167,18 +166,18 @@
 #         vertices=([(-1000,0,0),(1000,0,0)], "m"),
 #     )
 #     tgt = magpy.current.Polyline(
 #         current=(1, "A"),
 #         vertices=([(0,-1000,0),(0,0,0),(0,1000,0)], "m"),
 #         position=((0,0,1), "m"),
 #     )
-#     tgt.mesh = 1000
+#     tgt.meshing = 1000
 
 #     ureg=src.current._REGISTRY
-#     F,T = getFTwire(src, tgt)
+#     F,T = getFT(src, tgt)
 
 #     assert np.max(abs(F.magnitude)) < 1e-14
 
 
 
 def test_physics_perpendicular_wires():
     """
@@ -189,17 +188,17 @@
         vertices=[(-1000,0,0),(1000,0,0)],
     )
     wire2 = magpy.current.Polyline(
         current=1,
         vertices=[(0,-1000,0),(0,0,0),(0,1000,0)],
         position=(0,0,1),
     )
-    wire2.mesh = 1000
+    wire2.meshing = 1000
 
-    F,T = getFTwire(wire1, wire2)
+    F,T = getFT(wire1, wire2)
 
     assert np.max(abs(F)) < 1e-14
 
 
 def test_cube_loop_replacement():
     """
     A magnet sees the same force as a respective current replacement
@@ -209,26 +208,24 @@
         dimension=(1,1,1)
     )
     cube = magpy.magnet.Cuboid(
         polarization=(0,0,1),
         dimension=(2,2,2),
         position=(1,2,3)
     )
-    cube.mesh=(20,20,20)
+    cube.meshing=(20,20,20)
     nn=150
     currs = []
     for z in np.linspace(-1,1,nn):
         loop = magpy.current.Polyline(
             current=1e7/4/np.pi*2/nn,
             vertices=((-1,-1,z),(1,-1,z),(1,1,z),(-1,1,z),(-1,-1,z)),
             position=(1,2,3)
         )
-        loop.mesh = nn
+        loop.meshing = nn
         currs.append(loop)
 
-    F1,T1 = getFTcube(gen, cube, anchor=np.array((0,0,0)))
-    F2,T2 = getFTwire(gen, currs, anchor=np.array((0,0,0)))
-    F2 = np.sum(F2,axis=0)
-    T2 = np.sum(T2,axis=0)
+    F1,T1 = getFT(gen, cube, anchor=np.array((0,0,0)))
+    F2,T2 = np.sum(getFT(gen, currs, anchor=np.array((0,0,0))), axis=0)
 
     assert np.amax(abs((F1-F2)/(F1+F2)*2))<1e-2
     assert np.amax(abs((T1-T2)/(T1+T2)*2))<1e-2
```

### Comparing `magpylib_force-0.1.6/tests/test_self_consistency.py` & `magpylib_force-0.1.7/tests/test_self_consistency.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import numpy as np
 import magpylib as magpy
-from magpylib_force.force import getFTcube
-from magpylib_force.force import getFTwire
+from magpylib_force.force import getFT
 
 
 # def test_consistency_cube_cube():
 #     """
 #     consistency between 2 cuboids with aligned axes
 #     """
 #     cube1 = magpy.magnet.Cuboid(
@@ -13,26 +12,26 @@
 #         polarization=((1,2,3), "T"),
 #     )
 #     cube2 = magpy.magnet.Cuboid(
 #         dimension=((1,1,2), "mm"),
 #         polarization=((3,2,1), "T"),
 #         position=((2,2,.5), "mm")
 #     )
-#     cube1.mesh = (20,10,10)
-#     cube2.mesh = (10,10,20)
+#     cube1.meshing = (20,10,10)
+#     cube2.meshing = (10,10,20)
 
-#     F1,_ = getFTcube(cube1, cube2)
-#     F2,_ = getFTcube(cube2, cube1)
+#     F1,_ = getFT(cube1, cube2)
+#     F2,_ = getFT(cube2, cube1)
 #     errF = 2*(np.linalg.norm(F1+F2)/np.linalg.norm(F1-F2))
 #     assert errF < 1e-4
 
 #     ureg = cube1.dimension._REGISTRY
 #     Tanch = np.array([0,0,0]) * ureg.meter
-#     F1,T1 = getFTcube(cube1, cube2, Tanch=Tanch)
-#     F2,T2 = getFTcube(cube2, cube1, Tanch=Tanch)
+#     F1,T1 = getFT(cube1, cube2, Tanch=Tanch)
+#     F2,T2 = getFT(cube2, cube1, Tanch=Tanch)
 
 #     errF = 2*(np.linalg.norm(F1+F2)/np.linalg.norm(F1-F2))
 #     errT = 2*(np.linalg.norm(T1+T2)/np.linalg.norm(T1-T2))
 #     assert errF < 1e-4
 #     assert errT < 1e-4
 
 def test_consistency_cube_cube():
@@ -44,24 +43,24 @@
         polarization=(1,2,3),
     )
     cube2 = magpy.magnet.Cuboid(
         dimension=(1,1,2),
         polarization=(3,2,1),
         position=(2,2,.5)
     )
-    cube1.mesh = (20,10,10)
-    cube2.mesh = (10,10,20)
+    cube1.meshing = (20,10,10)
+    cube2.meshing = (10,10,20)
 
-    #F1,_ = getFTcube(cube1, cube2)
-    #F2,_ = getFTcube(cube2, cube1)
+    #F1,_ = getFT(cube1, cube2)
+    #F2,_ = getFT(cube2, cube1)
     #errF = 2*(np.linalg.norm(F1+F2)/np.linalg.norm(F1-F2))
     #assert errF < 1e-4
 
-    F1,T1 = getFTcube(cube1, cube2, anchor=np.array((0,0,0)))
-    F2,T2 = getFTcube(cube2, cube1, anchor=np.array((0,0,0)))
+    F1,T1 = getFT(cube1, cube2, anchor=np.array((0,0,0)))
+    F2,T2 = getFT(cube2, cube1, anchor=np.array((0,0,0)))
 
     errF = 2*(np.linalg.norm(F1+F2)/np.linalg.norm(F1-F2))
     errT = 2*(np.linalg.norm(T1+T2)/np.linalg.norm(T1-T2))
     assert errF < 1e-4
     assert errT < 1e-4
 
 
@@ -69,104 +68,104 @@
 #     """
 #     consistency between 2 arbitrary current loops
 #     """
 #     wire1 = magpy.current.Polyline(
 #         current=(1, "A"),
 #         vertices=([(1,0,0),(0,1,.2), (-1,0,0), (0,-1,.5), (1,0,0)], "m"),
 #     )
-#     wire1.mesh=(200)
+#     wire1.meshing=(200)
 #     wire2 = magpy.current.Polyline(
 #         current=(1, "A"),
 #         vertices=([(-1,-1,.5), (-1,1,1), (1,1,2), (1,-1,1), (-1,-1,.5)], "m"),
 #     )
-#     wire2.mesh=(200)
-#     F1a,_ = getFTwire(wire1, wire2)
-#     F2a,_ = getFTwire(wire2, wire1)
+#     wire2.meshing=(200)
+#     F1a,_ = getFT(wire1, wire2)
+#     F2a,_ = getFT(wire2, wire1)
 #     errFa = np.linalg.norm(F1a+F2a) / np.linalg.norm(F1a-F2a)
 #     assert errFa < 1e-5
 
 #     ureg = wire1.current._REGISTRY
-#     F1b,T1b = getFTwire(wire1, wire2, Tanch=np.array((0,0,0))*ureg.meter)
-#     F2b,T2b = getFTwire(wire2, wire1, Tanch=np.array((0,0,0))*ureg.meter)
+#     F1b,T1b = getFT(wire1, wire2, Tanch=np.array((0,0,0))*ureg.meter)
+#     F2b,T2b = getFT(wire2, wire1, Tanch=np.array((0,0,0))*ureg.meter)
 #     errFb = np.linalg.norm(F1b+F2b) / np.linalg.norm(F1b-F2b)
 #     errTb = np.linalg.norm(T1b+T2b) / np.linalg.norm(T1b-T2b)
 #     assert errFb < 1e-5
 #     assert errTb < 1e-4
 
 def test_consistency_loop_loop():
     """
     consistency between 2 arbitrary current loops
     """
     wire1 = magpy.current.Polyline(
         current=1,
         vertices=[(1,0,0),(0,1,.2), (-1,0,0), (0,-1,.5), (1,0,0)],
     )
-    wire1.mesh=(200)
+    wire1.meshing=(200)
     wire2 = magpy.current.Polyline(
         current=1,
         vertices=[(-1,-1,.5), (-1,1,1), (1,1,2), (1,-1,1), (-1,-1,.5)],
     )
-    wire2.mesh=(200)
-    F1a,_ = getFTwire(wire1, wire2)
-    F2a,_ = getFTwire(wire2, wire1)
+    wire2.meshing=(200)
+    F1a,_ = getFT(wire1, wire2)
+    F2a,_ = getFT(wire2, wire1)
     errFa = np.linalg.norm(F1a+F2a) / np.linalg.norm(F1a-F2a)
     assert errFa < 1e-5
 
-    F1b,T1b = getFTwire(wire1, wire2, anchor=np.array((0,0,0)))
-    F2b,T2b = getFTwire(wire2, wire1, anchor=np.array((0,0,0)))
+    F1b,T1b = getFT(wire1, wire2, anchor=np.array((0,0,0)))
+    F2b,T2b = getFT(wire2, wire1, anchor=np.array((0,0,0)))
     errFb = np.linalg.norm(F1b+F2b) / np.linalg.norm(F1b-F2b)
     errTb = np.linalg.norm(T1b+T2b) / np.linalg.norm(T1b-T2b)
     assert errFb < 1e-5
     assert errTb < 1e-4
 
 
 # def test_consistency_cube_loop():
 #     """
 #     consistency between a current loop and a cuboid magnet
 #     """
 #     magnet = magpy.magnet.Cuboid(
 #         polarization=((1,2,3), "T"),
 #         dimension=((.6,.4,.2), "m"),
 #     )
-#     magnet.mesh=(30,20,10)
+#     magnet.meshing=(30,20,10)
 #     wire = magpy.current.Polyline(
 #         current=(1, "A"),
 #         vertices=([(-1,-1,.5), (-1,1,1), (1,1,.1), (1,-1,1), (-1,-1,.5)], "m"),
 #     )
-#     wire.mesh=(200)
-#     F1a,_ = getFTcube(wire, magnet)
-#     F2a,_ = getFTwire(magnet, wire)
+#     wire.meshing=(200)
+#     F1a,_ = getFT(wire, magnet)
+#     F2a,_ = getFT(magnet, wire)
 #     errFa = np.linalg.norm(F1a+F2a) / np.linalg.norm(F1a-F2a)*2
 #     assert errFa < 1e-5
 
 #     ureg = wire.current._REGISTRY
-#     F1b,T1b = getFTcube(wire, magnet, Tanch=np.array((0,0,0))*ureg.meter)
-#     F2b,T2b = getFTwire(magnet, wire, Tanch=np.array((0,0,0))*ureg.meter)
+#     F1b,T1b = getFT(wire, magnet, Tanch=np.array((0,0,0))*ureg.meter)
+#     F2b,T2b = getFT(magnet, wire, Tanch=np.array((0,0,0))*ureg.meter)
 #     errFb = np.linalg.norm(F1b+F2b) / np.linalg.norm(F1b-F2b)*2
 #     assert errFb < 1e-5
 #     errTb = np.linalg.norm(T1b+T2b) / np.linalg.norm(T1b-T2b)*2
 #     assert errTb < 1e-5
 def test_consistency_cube_loop():
     """
     consistency between a current loop and a cuboid magnet
     """
     magnet = magpy.magnet.Cuboid(
         polarization=(1,2,3),
         dimension=(.6,.4,.2),
     )
-    magnet.mesh=(30,20,10)
+    magnet.meshing=(30,20,10)
     wire = magpy.current.Polyline(
         current=1,
         vertices=[(-1,-1,.5), (-1,1,1), (1,1,.1), (1,-1,1), (-1,-1,.5)],
     )
-    wire.mesh=(200)
-    #F1a,_ = getFTcube(wire, magnet)
-    #F2a,_ = getFTwire(magnet, wire)
+    wire.meshing=(200)
+    #F1a,_ = getFT(wire, magnet)
+    #F2a,_ = getFT(magnet, wire)
     #errFa = np.linalg.norm(F1a+F2a) / np.linalg.norm(F1a-F2a)*2
     #assert errFa < 1e-5
 
-    F1b,T1b = getFTcube(wire, magnet, anchor=np.array((0,0,0)))
-    F2b,T2b = getFTwire(magnet, wire, anchor=np.array((0,0,0)))
+    F1b,T1b = getFT(wire, magnet, anchor=np.array((0,0,0)))
+    F2b,T2b = getFT(magnet, wire, anchor=np.array((0,0,0)))
     errFb = np.linalg.norm(F1b+F2b) / np.linalg.norm(F1b-F2b)*2
     assert errFb < 1e-5
     errTb = np.linalg.norm(T1b+T2b) / np.linalg.norm(T1b-T2b)*2
     assert errTb < 1e-5
```

