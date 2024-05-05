# Comparing `tmp/clump-python-0.3.0.tar.gz` & `tmp/clump-python-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clump-python-0.3.0.tar", last modified: Tue Apr 30 14:38:17 2024, max compression
+gzip compressed data, was "clump-python-0.3.1.tar", last modified: Sun May  5 10:19:15 2024, max compression
```

## Comparing `clump-python-0.3.0.tar` & `clump-python-0.3.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-30 14:38:17.440158 clump-python-0.3.0/
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-30 14:38:17.432158 clump-python-0.3.0/CLUMP/
--rw-rw-r--   0 utku      (1000) utku      (1000)     8025 2024-04-26 09:21:09.000000 clump-python-0.3.0/CLUMP/ExtractSurface.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     9244 2024-04-26 05:50:24.000000 clump-python-0.3.0/CLUMP/GenerateClump_Euclidean_3D.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     8714 2024-04-26 09:22:56.000000 clump-python-0.3.0/CLUMP/GenerateClump_Favier.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     8138 2024-04-26 09:22:56.000000 clump-python-0.3.0/CLUMP/GenerateClump_Ferellec_McDowell.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      241 2024-04-24 14:39:02.000000 clump-python-0.3.0/CLUMP/__init__.py
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-30 14:38:17.432158 clump-python-0.3.0/CLUMP/examples/
--rw-rw-r--   0 utku      (1000) utku      (1000)      812 2024-04-26 05:50:01.000000 clump-python-0.3.0/CLUMP/examples/Example_Euclidean_3D.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      937 2024-04-26 05:49:49.000000 clump-python-0.3.0/CLUMP/examples/Example_Euclidean_3D_Extended.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      675 2024-04-26 05:50:04.000000 clump-python-0.3.0/CLUMP/examples/Example_ExtractSurface.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      713 2024-04-26 05:50:07.000000 clump-python-0.3.0/CLUMP/examples/Example_Favier_automatic_generation.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      743 2024-04-26 05:50:11.000000 clump-python-0.3.0/CLUMP/examples/Example_Ferellec_McDowell.py
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-30 14:38:17.440158 clump-python-0.3.0/CLUMP/examples/ParticleGeometries/
--rw-rw-r--   0 utku      (1000) utku      (1000)     8351 2024-04-17 12:23:12.000000 clump-python-0.3.0/CLUMP/examples/ParticleGeometries/Binary_3D_Cube.mat
--rw-rw-r--   0 utku      (1000) utku      (1000)     4280 2024-04-17 12:23:12.000000 clump-python-0.3.0/CLUMP/examples/ParticleGeometries/Binary_3D_Cuboid.mat
--rw-rw-r--   0 utku      (1000) utku      (1000)  1024084 2022-11-01 09:30:38.000000 clump-python-0.3.0/CLUMP/examples/ParticleGeometries/Ellipsoid_R_2.0_1.0_1.0.stl
--rw-rw-r--   0 utku      (1000) utku      (1000)   153684 2024-04-17 12:23:12.000000 clump-python-0.3.0/CLUMP/examples/ParticleGeometries/Hexahedron.stl
--rw-rw-r--   0 utku      (1000) utku      (1000)  2670559 2024-04-17 12:23:12.000000 clump-python-0.3.0/CLUMP/examples/ParticleGeometries/Human_femur.stl
--rw-rw-r--   0 utku      (1000) utku      (1000)   102484 2024-04-17 12:23:12.000000 clump-python-0.3.0/CLUMP/examples/ParticleGeometries/Octahedron.stl
--rw-rw-r--   0 utku      (1000) utku      (1000)  2880084 2024-04-23 14:41:30.000000 clump-python-0.3.0/CLUMP/examples/ParticleGeometries/Torus.stl
--rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.3.0/CLUMP/examples/ParticleGeometries/__init__.py
--rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.3.0/CLUMP/examples/__init__.py
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-30 14:38:17.440158 clump-python-0.3.0/CLUMP/utils/
--rw-rw-r--   0 utku      (1000) utku      (1000)    15528 2024-04-26 05:50:40.000000 clump-python-0.3.0/CLUMP/utils/MyRobustCrust.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     2670 2024-04-26 05:57:34.000000 clump-python-0.3.0/CLUMP/utils/ParticlePlotter.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     2287 2024-04-26 05:54:26.000000 clump-python-0.3.0/CLUMP/utils/PatchNormals.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     9442 2024-04-23 16:28:34.000000 clump-python-0.3.0/CLUMP/utils/RigidBodyParameters.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     2293 2024-04-26 05:56:57.000000 clump-python-0.3.0/CLUMP/utils/STL_ReaderWriter.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     1330 2024-04-26 05:51:27.000000 clump-python-0.3.0/CLUMP/utils/VTK_Writer.py
--rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-17 12:23:12.000000 clump-python-0.3.0/CLUMP/utils/__init__.py
--rw-rw-r--   0 utku      (1000) utku      (1000)    35149 2022-11-01 09:30:38.000000 clump-python-0.3.0/LICENSE
--rw-r--r--   0 utku      (1000) utku      (1000)     6288 2024-04-30 14:38:17.440158 clump-python-0.3.0/PKG-INFO
--rw-rw-r--   0 utku      (1000) utku      (1000)     5524 2024-04-30 14:38:06.000000 clump-python-0.3.0/README.md
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-30 14:38:17.440158 clump-python-0.3.0/clump_python.egg-info/
--rw-r--r--   0 utku      (1000) utku      (1000)     6288 2024-04-30 14:38:17.000000 clump-python-0.3.0/clump_python.egg-info/PKG-INFO
--rw-rw-r--   0 utku      (1000) utku      (1000)     1230 2024-04-30 14:38:17.000000 clump-python-0.3.0/clump_python.egg-info/SOURCES.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)        1 2024-04-30 14:38:17.000000 clump-python-0.3.0/clump_python.egg-info/dependency_links.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)       49 2024-04-30 14:38:17.000000 clump-python-0.3.0/clump_python.egg-info/requires.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)        6 2024-04-30 14:38:17.000000 clump-python-0.3.0/clump_python.egg-info/top_level.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)       38 2024-04-30 14:38:17.440158 clump-python-0.3.0/setup.cfg
--rw-rw-r--   0 utku      (1000) utku      (1000)     1209 2024-04-30 14:38:06.000000 clump-python-0.3.0/setup.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-05-05 10:19:15.166063 clump-python-0.3.1/
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-05-05 10:19:15.154062 clump-python-0.3.1/CLUMP/
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8025 2024-04-26 09:21:09.000000 clump-python-0.3.1/CLUMP/ExtractSurface.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     9244 2024-04-26 05:50:24.000000 clump-python-0.3.1/CLUMP/GenerateClump_Euclidean_3D.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8714 2024-04-26 09:22:56.000000 clump-python-0.3.1/CLUMP/GenerateClump_Favier.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8138 2024-04-26 09:22:56.000000 clump-python-0.3.1/CLUMP/GenerateClump_Ferellec_McDowell.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      241 2024-04-24 14:39:02.000000 clump-python-0.3.1/CLUMP/__init__.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-05-05 10:19:15.158063 clump-python-0.3.1/CLUMP/examples/
+-rw-rw-r--   0 utku      (1000) utku      (1000)      812 2024-04-26 05:50:01.000000 clump-python-0.3.1/CLUMP/examples/Example_Euclidean_3D.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      937 2024-04-26 05:49:49.000000 clump-python-0.3.1/CLUMP/examples/Example_Euclidean_3D_Extended.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      675 2024-04-26 05:50:04.000000 clump-python-0.3.1/CLUMP/examples/Example_ExtractSurface.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      713 2024-04-26 05:50:07.000000 clump-python-0.3.1/CLUMP/examples/Example_Favier.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      743 2024-04-26 05:50:11.000000 clump-python-0.3.1/CLUMP/examples/Example_Ferellec_McDowell.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-05-05 10:19:15.162063 clump-python-0.3.1/CLUMP/examples/ParticleGeometries/
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8351 2024-04-17 12:23:12.000000 clump-python-0.3.1/CLUMP/examples/ParticleGeometries/Binary_3D_Cube.mat
+-rw-rw-r--   0 utku      (1000) utku      (1000)     4280 2024-04-17 12:23:12.000000 clump-python-0.3.1/CLUMP/examples/ParticleGeometries/Binary_3D_Cuboid.mat
+-rw-rw-r--   0 utku      (1000) utku      (1000)  1024084 2022-11-01 09:30:38.000000 clump-python-0.3.1/CLUMP/examples/ParticleGeometries/Ellipsoid_R_2.0_1.0_1.0.stl
+-rw-rw-r--   0 utku      (1000) utku      (1000)   153684 2024-04-17 12:23:12.000000 clump-python-0.3.1/CLUMP/examples/ParticleGeometries/Hexahedron.stl
+-rw-rw-r--   0 utku      (1000) utku      (1000)  2670559 2024-04-17 12:23:12.000000 clump-python-0.3.1/CLUMP/examples/ParticleGeometries/Human_femur.stl
+-rw-rw-r--   0 utku      (1000) utku      (1000)   102484 2024-04-17 12:23:12.000000 clump-python-0.3.1/CLUMP/examples/ParticleGeometries/Octahedron.stl
+-rw-rw-r--   0 utku      (1000) utku      (1000)  2880084 2024-04-23 14:41:30.000000 clump-python-0.3.1/CLUMP/examples/ParticleGeometries/Torus.stl
+-rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.3.1/CLUMP/examples/ParticleGeometries/__init__.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.3.1/CLUMP/examples/__init__.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-05-05 10:19:15.162063 clump-python-0.3.1/CLUMP/utils/
+-rw-rw-r--   0 utku      (1000) utku      (1000)    15528 2024-04-26 05:50:40.000000 clump-python-0.3.1/CLUMP/utils/MyRobustCrust.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     2691 2024-05-02 17:14:51.000000 clump-python-0.3.1/CLUMP/utils/ParticlePlotter.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     2287 2024-04-26 05:54:26.000000 clump-python-0.3.1/CLUMP/utils/PatchNormals.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     9442 2024-04-23 16:28:34.000000 clump-python-0.3.1/CLUMP/utils/RigidBodyParameters.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     2293 2024-04-26 05:56:57.000000 clump-python-0.3.1/CLUMP/utils/STL_ReaderWriter.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     1330 2024-04-26 05:51:27.000000 clump-python-0.3.1/CLUMP/utils/VTK_Writer.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-17 12:23:12.000000 clump-python-0.3.1/CLUMP/utils/__init__.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)    35149 2022-11-01 09:30:38.000000 clump-python-0.3.1/LICENSE
+-rw-r--r--   0 utku      (1000) utku      (1000)     6268 2024-05-05 10:19:15.166063 clump-python-0.3.1/PKG-INFO
+-rw-rw-r--   0 utku      (1000) utku      (1000)     5504 2024-05-05 10:11:43.000000 clump-python-0.3.1/README.md
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-05-05 10:19:15.166063 clump-python-0.3.1/clump_python.egg-info/
+-rw-r--r--   0 utku      (1000) utku      (1000)     6268 2024-05-05 10:19:15.000000 clump-python-0.3.1/clump_python.egg-info/PKG-INFO
+-rw-rw-r--   0 utku      (1000) utku      (1000)     1209 2024-05-05 10:19:15.000000 clump-python-0.3.1/clump_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)        1 2024-05-05 10:19:15.000000 clump-python-0.3.1/clump_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)       49 2024-05-05 10:19:15.000000 clump-python-0.3.1/clump_python.egg-info/requires.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)        6 2024-05-05 10:19:15.000000 clump-python-0.3.1/clump_python.egg-info/top_level.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)       38 2024-05-05 10:19:15.166063 clump-python-0.3.1/setup.cfg
+-rw-rw-r--   0 utku      (1000) utku      (1000)     1209 2024-05-05 10:10:10.000000 clump-python-0.3.1/setup.py
```

### Comparing `clump-python-0.3.0/CLUMP/ExtractSurface.py` & `clump-python-0.3.1/CLUMP/ExtractSurface.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.3.0/CLUMP/GenerateClump_Euclidean_3D.py` & `clump-python-0.3.1/CLUMP/GenerateClump_Euclidean_3D.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.3.0/CLUMP/GenerateClump_Favier.py` & `clump-python-0.3.1/CLUMP/GenerateClump_Favier.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.3.0/CLUMP/GenerateClump_Ferellec_McDowell.py` & `clump-python-0.3.1/CLUMP/GenerateClump_Ferellec_McDowell.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.3.0/CLUMP/examples/Example_Euclidean_3D.py` & `clump-python-0.3.1/CLUMP/examples/Example_Euclidean_3D.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.3.0/CLUMP/examples/Example_Euclidean_3D_Extended.py` & `clump-python-0.3.1/CLUMP/examples/Example_Euclidean_3D_Extended.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.3.0/CLUMP/examples/Example_ExtractSurface.py` & `clump-python-0.3.1/CLUMP/examples/Example_ExtractSurface.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.3.0/CLUMP/examples/Example_Favier_automatic_generation.py` & `clump-python-0.3.1/CLUMP/examples/Example_Favier.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.3.0/CLUMP/examples/Example_Ferellec_McDowell.py` & `clump-python-0.3.1/CLUMP/examples/Example_Ferellec_McDowell.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.3.0/CLUMP/examples/ParticleGeometries/Binary_3D_Cube.mat` & `clump-python-0.3.1/CLUMP/examples/ParticleGeometries/Binary_3D_Cube.mat`

 * *Files identical despite different names*

### Comparing `clump-python-0.3.0/CLUMP/examples/ParticleGeometries/Binary_3D_Cuboid.mat` & `clump-python-0.3.1/CLUMP/examples/ParticleGeometries/Binary_3D_Cuboid.mat`

 * *Files identical despite different names*

### Comparing `clump-python-0.3.0/CLUMP/examples/ParticleGeometries/Ellipsoid_R_2.0_1.0_1.0.stl` & `clump-python-0.3.1/CLUMP/examples/ParticleGeometries/Ellipsoid_R_2.0_1.0_1.0.stl`

 * *Files identical despite different names*

### Comparing `clump-python-0.3.0/CLUMP/examples/ParticleGeometries/Hexahedron.stl` & `clump-python-0.3.1/CLUMP/examples/ParticleGeometries/Hexahedron.stl`

 * *Files identical despite different names*

### Comparing `clump-python-0.3.0/CLUMP/examples/ParticleGeometries/Human_femur.stl` & `clump-python-0.3.1/CLUMP/examples/ParticleGeometries/Human_femur.stl`

 * *Files identical despite different names*

### Comparing `clump-python-0.3.0/CLUMP/examples/ParticleGeometries/Octahedron.stl` & `clump-python-0.3.1/CLUMP/examples/ParticleGeometries/Octahedron.stl`

 * *Files identical despite different names*

### Comparing `clump-python-0.3.0/CLUMP/examples/ParticleGeometries/Torus.stl` & `clump-python-0.3.1/CLUMP/examples/ParticleGeometries/Torus.stl`

 * *Files identical despite different names*

### Comparing `clump-python-0.3.0/CLUMP/utils/MyRobustCrust.py` & `clump-python-0.3.1/CLUMP/utils/MyRobustCrust.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.3.0/CLUMP/utils/ParticlePlotter.py` & `clump-python-0.3.1/CLUMP/utils/ParticlePlotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 import matplotlib.pyplot as plt
 import pyvista as pv
 import trimesh
 
 "2024 Python implementation by A.U. Canbolat and V. Angelidakis  <utku.canbolat@fau.de>"
 
+
 def clump_plotter(P, F, clump):
     """Plots 3D spheres using trisurf"""
     fig = plt.figure()
     ax = fig.add_subplot(111, projection='3d')
 
     # Create patch
     ax.plot_trisurf(P[:, 0], P[:, 1], P[:, 2], triangles=F, color=[0, 1, 0, 0.2], edgecolor='none')
@@ -51,15 +52,15 @@
 
 
 def mesh_plotter_trimesh(vertices, faces, spheresList, phi_res=50, theta_res=50):
     """Plots a wireframe mesh and spheres using trimesh and PyVista."""
     mesh = trimesh.Trimesh(vertices=vertices, faces=faces)
     pv_mesh = pv.wrap(mesh)
 
-    plotter = pv.Plotter()
+    plotter = pv.Plotter(window_title='CLUMP')
     plotter.add_mesh(pv_mesh, style='wireframe', color='black', line_width=2)
 
     for (x, y, z, r) in spheresList:
         add_sphere_to_plotter(plotter, (x, y, z), r, 'white', 0.5, phi_res, theta_res)
 
     plotter.camera_position = [
         (np.min(vertices[:, 0]) + np.max(vertices[:, 0])) / 2,
```

### Comparing `clump-python-0.3.0/CLUMP/utils/PatchNormals.py` & `clump-python-0.3.1/CLUMP/utils/PatchNormals.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.3.0/CLUMP/utils/RigidBodyParameters.py` & `clump-python-0.3.1/CLUMP/utils/RigidBodyParameters.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.3.0/CLUMP/utils/STL_ReaderWriter.py` & `clump-python-0.3.1/CLUMP/utils/STL_ReaderWriter.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.3.0/CLUMP/utils/VTK_Writer.py` & `clump-python-0.3.1/CLUMP/utils/VTK_Writer.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.3.0/LICENSE` & `clump-python-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clump-python-0.3.0/PKG-INFO` & `clump-python-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clump-python
-Version: 0.3.0
+Version: 0.3.1
 Summary: This Python library provides tools for creating and examining clumps using techniques: the Euclidean Distance Transform, Favier, and Ferellec-McDowell. It allows for the efficient generation of clumps and the extraction of their surfaces.
 Home-page: https://github.com/vsangelidakis/CLUMP
 Author: Utku Canbolat, Vasileios Angelidakis
 Author-email: utku.canbolat@fau.de
 License: GPL-3.0-only
 Keywords: Clump,Clump Generation,Euclidean Distance Transform,Favier,Ferellec-McDowell,Surface Extraction
 Description-Content-Type: text/markdown
@@ -65,30 +65,30 @@
 
 After the installation using ```pip install clump-python```, CLUMP can easily be imported as
 
 ```python
 import CLUMP
 ```
 
-The examples below illustrate various methods for creating clumps tailored to different target geometries. Each function includes documentation for the variables used.
+This following examples demonstrate different approaches to generate clumps for the different target geometry. The variables below are documented within each function. 
 
 ```python
 from CLUMP.examples import Example_Euclidean_3D
 ```
 
 ```python
 from CLUMP.examples import Example_Euclidean_3D_Extended
 ```
 
 ```python
 from CLUMP.examples import Example_Ferellec_McDowell
 ```
 
 ```python
-from CLUMP.examples import Example_Favier_automatic_generation
+from CLUMP.examples import Example_Favier
 ```
 
 The following example demonstrates the surface extraction method.
 
 ```python
 from CLUMP.examples import Example_ExtractSurface
 ```
```

### Comparing `clump-python-0.3.0/README.md` & `clump-python-0.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -47,30 +47,30 @@
 
 After the installation using ```pip install clump-python```, CLUMP can easily be imported as
 
 ```python
 import CLUMP
 ```
 
-The examples below illustrate various methods for creating clumps tailored to different target geometries. Each function includes documentation for the variables used.
+This following examples demonstrate different approaches to generate clumps for the different target geometry. The variables below are documented within each function. 
 
 ```python
 from CLUMP.examples import Example_Euclidean_3D
 ```
 
 ```python
 from CLUMP.examples import Example_Euclidean_3D_Extended
 ```
 
 ```python
 from CLUMP.examples import Example_Ferellec_McDowell
 ```
 
 ```python
-from CLUMP.examples import Example_Favier_automatic_generation
+from CLUMP.examples import Example_Favier
 ```
 
 The following example demonstrates the surface extraction method.
 
 ```python
 from CLUMP.examples import Example_ExtractSurface
 ```
```

### Comparing `clump-python-0.3.0/clump_python.egg-info/PKG-INFO` & `clump-python-0.3.1/clump_python.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clump-python
-Version: 0.3.0
+Version: 0.3.1
 Summary: This Python library provides tools for creating and examining clumps using techniques: the Euclidean Distance Transform, Favier, and Ferellec-McDowell. It allows for the efficient generation of clumps and the extraction of their surfaces.
 Home-page: https://github.com/vsangelidakis/CLUMP
 Author: Utku Canbolat, Vasileios Angelidakis
 Author-email: utku.canbolat@fau.de
 License: GPL-3.0-only
 Keywords: Clump,Clump Generation,Euclidean Distance Transform,Favier,Ferellec-McDowell,Surface Extraction
 Description-Content-Type: text/markdown
@@ -65,30 +65,30 @@
 
 After the installation using ```pip install clump-python```, CLUMP can easily be imported as
 
 ```python
 import CLUMP
 ```
 
-The examples below illustrate various methods for creating clumps tailored to different target geometries. Each function includes documentation for the variables used.
+This following examples demonstrate different approaches to generate clumps for the different target geometry. The variables below are documented within each function. 
 
 ```python
 from CLUMP.examples import Example_Euclidean_3D
 ```
 
 ```python
 from CLUMP.examples import Example_Euclidean_3D_Extended
 ```
 
 ```python
 from CLUMP.examples import Example_Ferellec_McDowell
 ```
 
 ```python
-from CLUMP.examples import Example_Favier_automatic_generation
+from CLUMP.examples import Example_Favier
 ```
 
 The following example demonstrates the surface extraction method.
 
 ```python
 from CLUMP.examples import Example_ExtractSurface
 ```
```

### Comparing `clump-python-0.3.0/clump_python.egg-info/SOURCES.txt` & `clump-python-0.3.1/clump_python.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 CLUMP/GenerateClump_Euclidean_3D.py
 CLUMP/GenerateClump_Favier.py
 CLUMP/GenerateClump_Ferellec_McDowell.py
 CLUMP/__init__.py
 CLUMP/examples/Example_Euclidean_3D.py
 CLUMP/examples/Example_Euclidean_3D_Extended.py
 CLUMP/examples/Example_ExtractSurface.py
-CLUMP/examples/Example_Favier_automatic_generation.py
+CLUMP/examples/Example_Favier.py
 CLUMP/examples/Example_Ferellec_McDowell.py
 CLUMP/examples/__init__.py
 CLUMP/examples/ParticleGeometries/Binary_3D_Cube.mat
 CLUMP/examples/ParticleGeometries/Binary_3D_Cuboid.mat
 CLUMP/examples/ParticleGeometries/Ellipsoid_R_2.0_1.0_1.0.stl
 CLUMP/examples/ParticleGeometries/Hexahedron.stl
 CLUMP/examples/ParticleGeometries/Human_femur.stl
```

### Comparing `clump-python-0.3.0/setup.py` & `clump-python-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="clump-python",
-    version="0.3.0",
+    version="0.3.1",
     packages=find_packages(),
     install_requires=[
         'matplotlib',
         'numpy',
         'numpy-stl',
         'pyvista',
         'scipy',
```

