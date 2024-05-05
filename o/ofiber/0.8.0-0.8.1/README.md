# Comparing `tmp/ofiber-0.8.0.tar.gz` & `tmp/ofiber-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofiber-0.8.0.tar", last modified: Tue Feb 13 23:39:55 2024, max compression
+gzip compressed data, was "ofiber-0.8.1.tar", last modified: Sun May  5 20:04:36 2024, max compression
```

## Comparing `ofiber-0.8.0.tar` & `ofiber-0.8.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 23:39:55.844250 ofiber-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-02-13 23:39:33.000000 ofiber-0.8.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-02-13 23:39:33.000000 ofiber-0.8.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-02-13 23:39:33.000000 ofiber-0.8.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-13 23:39:33.000000 ofiber-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-02-13 23:39:55.844250 ofiber-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-02-13 23:39:33.000000 ofiber-0.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 23:39:55.840250 ofiber-0.8.0/ofiber/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-02-13 23:39:33.000000 ofiber-0.8.0/ofiber/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-02-13 23:39:33.000000 ofiber-0.8.0/ofiber/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)    23794 2024-02-13 23:39:33.000000 ofiber-0.8.0/ofiber/cylinder_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-02-13 23:39:33.000000 ofiber-0.8.0/ofiber/dispersion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-02-13 23:39:33.000000 ofiber-0.8.0/ofiber/graded_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-02-13 23:39:33.000000 ofiber-0.8.0/ofiber/noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-02-13 23:39:33.000000 ofiber-0.8.0/ofiber/planar_parabolic.py
--rw-r--r--   0 runner    (1001) docker     (127)    11030 2024-02-13 23:39:33.000000 ofiber-0.8.0/ofiber/planar_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    30581 2024-02-13 23:39:33.000000 ofiber-0.8.0/ofiber/refraction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 23:39:55.844250 ofiber-0.8.0/ofiber.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-02-13 23:39:55.000000 ofiber-0.8.0/ofiber.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-02-13 23:39:55.000000 ofiber-0.8.0/ofiber.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 23:39:55.000000 ofiber-0.8.0/ofiber.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-13 23:39:55.000000 ofiber-0.8.0/ofiber.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-02-13 23:39:33.000000 ofiber-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-02-13 23:39:55.844250 ofiber-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-02-13 23:39:33.000000 ofiber-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 23:39:55.844250 ofiber-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-02-13 23:39:33.000000 ofiber-0.8.0/tests/test_all_notebooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:04:36.002664 ofiber-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-05 20:04:15.000000 ofiber-0.8.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-05 20:04:15.000000 ofiber-0.8.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-05 20:04:15.000000 ofiber-0.8.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-05 20:04:15.000000 ofiber-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-05-05 20:04:36.002664 ofiber-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-05-05 20:04:15.000000 ofiber-0.8.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:04:36.002664 ofiber-0.8.1/ofiber/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-05 20:04:15.000000 ofiber-0.8.1/ofiber/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8331 2024-05-05 20:04:15.000000 ofiber-0.8.1/ofiber/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30012 2024-05-05 20:04:15.000000 ofiber-0.8.1/ofiber/cylinder_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-05 20:04:15.000000 ofiber-0.8.1/ofiber/dispersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-05 20:04:15.000000 ofiber-0.8.1/ofiber/graded_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-05-05 20:04:15.000000 ofiber-0.8.1/ofiber/noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-05 20:04:15.000000 ofiber-0.8.1/ofiber/planar_parabolic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11144 2024-05-05 20:04:15.000000 ofiber-0.8.1/ofiber/planar_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30594 2024-05-05 20:04:15.000000 ofiber-0.8.1/ofiber/refraction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:04:36.002664 ofiber-0.8.1/ofiber.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-05-05 20:04:35.000000 ofiber-0.8.1/ofiber.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-05 20:04:35.000000 ofiber-0.8.1/ofiber.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 20:04:35.000000 ofiber-0.8.1/ofiber.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-05 20:04:35.000000 ofiber-0.8.1/ofiber.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-05 20:04:15.000000 ofiber-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-05 20:04:36.002664 ofiber-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-05 20:04:15.000000 ofiber-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:04:36.002664 ofiber-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-05 20:04:15.000000 ofiber-0.8.1/tests/test_all_notebooks.py
```

### Comparing `ofiber-0.8.0/CHANGELOG.rst` & `ofiber-0.8.1/CHANGELOG.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Changelog
 ==========
 
+0.8.1 (5/4/2024)
+-------------------
+* Implemented FF_node_polar_angle (@matt8s)
+* Added FF_node_polar_angle() example to 9-Far-field-irradiance.ipynb (@matt8s)
+* Modified _FF_polar_x to take argument kasin (@matt8s)
+* Improved configuration for ruff linting tool
+* Edited Jupyter notebooks
+* Added images and improved README
+
 0.8.0 (2/13/24)
 -------------------
 * add functions for far-field irradiance (thanks @matt8s)
 * improve calc of b for cylindrical step fibers for large V
 * add new notebook for far-field irradiance
 * enable use of arrays in `cylinder_step.LP_mode_value()`
```

### Comparing `ofiber-0.8.0/LICENSE.txt` & `ofiber-0.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ofiber-0.8.0/ofiber/__init__.py` & `ofiber-0.8.1/ofiber/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,18 +27,18 @@
 
     help(ofiber.planar_parabolic)
 
 Info about refractive index of glasses::
 
     help(ofiber.refraction)
 """
-__version__ = '0.8.0'
+__version__ = '0.8.1'
 __author__ = 'Scott Prahl'
 __email__ = 'scott.prahl@oit.edu'
-__copyright__ = '2018-23, Scott Prahl'
+__copyright__ = '2018-24, Scott Prahl'
 __license__ = 'MIT'
 __url__ = 'https://github.com/scottprahl/ofiber'
 
 from .basics import *
 from .cylinder_step import *
 from .dispersion import *
 from .graded_index import *
```

### Comparing `ofiber-0.8.0/ofiber/basics.py` & `ofiber-0.8.1/ofiber/basics.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
 def critical_angle(n_core, n_clad):
     """
     Calculate the angle (from the normal) for total internal reflection.
 
     Args:
         n_core : the index of refraction of the fiber core  [--]
-        n_core : the index of refraction of the fiber cladding  [--]
+        n_clad : the index of refraction of the fiber cladding  [--]
 
     Returns:
         angle of total internal reflection [radians]
     """
     return np.arcsin(n_clad / n_core)
 
 
@@ -115,15 +115,16 @@
 
 
 def esi_Delta(Delta, q):
     """
     Calculate equivalent step index (esi) Delta for a graded-index fiber.
 
     Args:
-        Delta :  relative refractive index     [-]
+        Delta :  relative refractive index         [-]
+        q :      parameter for graded index fiber  [-]
 
     Returns:
         equivalent relative refractive index   [-]
     """
     return q * (2 + q) / (1 + q)**2 * Delta
```

### Comparing `ofiber-0.8.0/ofiber/cylinder_step.py` & `ofiber-0.8.1/ofiber/cylinder_step.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 
 """
 Useful routines for step-index cylindrical waveguides.
 
 See <https://ofiber.readthedocs.io> for usage examples.
 
 Based on chapter 8 of A. Ghatak, K. Thyagarajan, An Introduction to Fiber
-Optics, Cambridge University Press, 1998
+Optics, Cambridge University Press, 1998 as well as Chen, Foundations for
+Guided-Wave Optics, Wiley-Interscience, 2007.
 
 Functions to calculate and plot modes for step index fibers.  Specifically::
 
     LP_mode_value(V, ell, em)
     LP_mode_values(V, ell)
     LP_core_irradiance(V, b, ell)
     LP_clad_irradiance(V, b, ell)
@@ -69,28 +70,30 @@
          'MFD',
          'PetermannW',
          'PetermannW_Approx',
          'V_d2bV_by_V',
          'V_d2bV_by_V_Approx',
          'FF_polar_irradiance_x',
          'FF_irradiance_x',
-          )
+         'FF_node_polar_angle',
+         )
 
 
 def _LHS_eqn_8_40(b, V, ell):
     """
     Calculate the left hand side of the eigenvalue eqn 8.40 in Ghatak.
 
     Also works for ell=0 (but is multiplied by -1 relative to eqn 8.41).
     This is private method that should not be needed outside this module.
 
     Args:
         b:      normalized propagation constant  [-]
         V:      V-parameter for fiber            [-]
         ell:    desired fiber mode               [-]
+
     Returns:
         LHS of equation 8.40                     [-]
     """
     U = V * np.sqrt(1 - b)
     return U * special.jv(ell - 1, U) / special.jv(ell, U)
 
 
@@ -101,14 +104,15 @@
     Also works for ell=0 (but is multiplied by -1 relative to eqn 8.41).
     This is private method that should not be needed outside this module.
 
     Args:
         b:      normalized propagation constant  [-]
         V:      V-parameter for fiber            [-]
         ell:    desired fiber mode               [-]
+
     Returns:
         RHS of equation 8.40                     [-]
     """
     W = V * np.sqrt(b)
     return -W * special.kn(ell - 1, W) / special.kn(ell, W)
 
 
@@ -117,16 +121,16 @@
     Return the difference of RHS and LHS of 8.40 in Ghatak.
 
     This function is zero when a guided mode exists in the step index fiber.
     This is a private function and should not be needed outside this module.
 
     Args:
         b:      normalized propagation constant  [-]
-        arg[0]: V-parameter for optical fiber    [-]
-        arg[1]: desired fiber mode               [-]
+        *args: two term array with arg[0] = V-parameter and arg[1]=desired fiber mode
+
     Returns:
         LHS-RHS of equation 8.40                 [-]
     """
     V = args[0]
     ell = args[1]
     g1 = _LHS_eqn_8_40(b, V, ell)
     g2 = _RHS_eqn_8_40(b, V, ell)
@@ -149,14 +153,15 @@
     For cylindrical fibers, em is a positive integer: thus there are modes
     LP_01, LP_02, but not LP_10.
 
     Args:
         V:   V-parameter for optical fiber    [-]
         ell: primary fiber mode   (integer)   [-]
         em:  secondary fiber mode (integer>0) [-]
+
     Returns:
         guided normalized propagation constant for mode (ell,em)  [-]
     """
     if ell < 0:
         ell *= -1   # negative ells are same as positive ones
 
     if em <= 0:
@@ -190,22 +195,23 @@
 def LP_mode_value(V, ell, em):
     """
     Calculate guided b for mode (ell,em) in a circular step-index fiber.
 
     b is the normalized propagation constant.  Each guided mode in an optical
     fiber has a specific value of b that depends on the fiber parameter V
     and the mode numbers ell and em.
-    
+
     This is a wrapper function that handles V, ell, or em being possible
     arrays.  See `LP_mode_value` for details.
 
     Args:
         V:   V-parameter for optical fiber    [-]
         ell: primary fiber mode   (integer)   [-]
         em:  secondary fiber mode (integer>0) [-]
+
     Returns:
         guided normalized propagation constant for mode (ell,em)  [-]
     """
     if em < 1:
         raise ValueError("The mode number 'em' must be one or greater.")
 
     if np.isscalar(V) + np.isscalar(ell) + np.isscalar(em) < 2:
@@ -239,14 +245,15 @@
     If there is no such mode, returns an empty array
 
     Note that in the returned array b[0] will correspond to LP_ell,1
 
     Args:
         V:   V-parameter for optical fiber    [-]
         ell: primary fiber mode   (integer)   [-]
+
     Returns:
         array of normalized propagation constant for mode ell  [-]
     """
     all_b = np.array([])
     for em in range(1, 10):
         b = LP_mode_value(V, ell, em)
         if b is None:
@@ -262,14 +269,15 @@
 
     The solutions correspond to places where the curves cross one another.  No
     crossing means that there is no guided mode for that mode value.
 
     Args:
         V:   V-parameter for optical fiber    [-]
         ell: primary fiber mode   (integer)   [-]
+
     Returns:
         graph for mode ell   [matplotlib.pyplot object]
     """
     abit = 1e-5
     pltmin = -2 * V
     pltmax = 2 * V
 
@@ -308,14 +316,15 @@
     See Ghatak equation 8.56.  The returned value is the total
     core power divided by the area of the core.
 
     Args:
         V:      V-parameter for fiber            [-]
         b:      normalized propagation constant  [-]
         ell:    desired fiber mode               [-]
+
     Returns:
         total core power over core area          [-]
     """
     U = V * np.sqrt(1 - b)
     return 1 - special.jv(ell + 1, U) * special.jv(ell - 1, U) / special.jv(ell, U)**2
 
 
@@ -326,14 +335,15 @@
     See Ghatak equation 8.57.  The returned value is the total
     cladding power divided by the area of the core.
 
     Args:
         V:      V-parameter for fiber            [-]
         b:      normalized propagation constant  [-]
         ell:    desired fiber mode               [-]
+
     Returns:
         total cladding power over core area      [-]
     """
     W = V * np.sqrt(b)
     return special.kn(ell + 1, W) * special.kn(ell - 1, W) / special.kn(ell, W)**2 - 1
 
 
@@ -344,14 +354,15 @@
     See Ghatak equation 8.58.  The returned value is the total
     power (cladding + core) divided by the area of the core.
 
     Args:
         V:      V-parameter for fiber            [-]
         b:      normalized propagation constant  [-]
         ell:    desired fiber mode               [-]
+
     Returns:
         total power over core area               [-]
     """
     U = V * np.sqrt(1 - b)
     W = V * np.sqrt(b)
     val = V**2 / U**2 * special.kn(ell + 1, W)
     val *= special.kn(ell - 1, W) / special.kn(ell, W)**2
@@ -363,14 +374,15 @@
     Calculate the normalized field in a step-index fiber.
 
     Args:
         V:        V-parameter for fiber            [-]
         b:        normalized propagation constant  [-]
         ell:      desired fiber mode               [-]
         r_over_a: (radial position)/(core radius)  [-]
+
     Returns:
         normalized field at point r_over_a         [-]
     """
     U = V * np.sqrt(1 - b)
     W = V * np.sqrt(b)
     r = abs(r_over_a)  # same value for negative radii
 
@@ -390,14 +402,15 @@
     2*np.trapz(LP(r_over_a)*r_over_a, r_over_a) =1
 
     Args:
         V:        V-parameter for fiber            [-]
         b:        normalized propagation constant  [-]
         ell:      desired fiber mode               [-]
         r_over_a: (radial position)/(core radius)  [-]
+
     Returns:
         normalized irradiance at points r_over_a   [-]
     """
     field = LP_radial_field(V, b, ell, r_over_a)
     return field**2
 
 
@@ -406,14 +419,15 @@
     Calculate the normalized irradiance in a step-index fiber.
 
     The normalization is done assuming
     the Gaussian envelope approximation for the LP_01 mode.
 
     Args:
         V:        V-parameter for fiber            [-]
+
     Returns:
         Omega_over_core_radius                     [-]
     """
     b = LP_mode_value(V, 0, 1)
     U = V * np.sqrt(1 - b)
     W = V * np.sqrt(b)
     Omega_over_a = special.jv(0, U) * V / U * special.kn(1, W) / special.kn(0, W)
@@ -428,14 +442,15 @@
     the Gaussian envelope approximation for the LP_01 mode. The result
     is normalized such that
     np.trapz(Gaussian(r_over_a)*r_over_a, r_over_a) = 1/2
 
     Args:
         V:        V-parameter for fiber            [-]
         r_over_a: (radial position)/(core radius)  [-]
+
     Returns:
         normalized irradiance at points r_over_a   [-]
     """
     Omega_over_a = gaussian_envelope_Omega(V)
     return 1 / Omega_over_a**2 * np.exp(-r_over_a**2 / Omega_over_a**2)
 
 
@@ -445,14 +460,15 @@
 
     See Ghatak eqn 8.69
 
     Args:
         w1:      mode field radius of first fiber  [m]
         w2:      mode field radius of second fiber [m]
         u:       transverse misalignment           [m]
+
     Returns:
         transverse misalignment loss in dB         [-]
     """
     sq = w1**2 + w2**2
     loss = (2 * w1 * w2 / sq)**2 * np.exp(-2 * u**2 / sq)
     return -10 * np.log10(loss)
 
@@ -460,39 +476,41 @@
 def angular_misalignment_loss_db(n, w, theta, lambda0):
     """
     Calculate the loss due to angular fiber misalignment.
 
     See Ghatak eqn 8.75
 
     Args:
-        n:        index between fiber ends [-]
-        w:        mode field radius        [m]
-        theta:    angular misalignment     [radians]
-        lambda0:  wavelength in vacuum     [m]
+        n:        index of medium between fiber ends [-]
+        w:        mode field radius                  [m]
+        theta:    angular misalignment               [radians]
+        lambda0:  wavelength in vacuum               [m]
+
     Returns:
         angular misalignment loss in dB    [-]
     """
     return 4.34 * (np.pi * w * theta * n / lambda0)**2
 
 
-def longitudinal_misalignment_loss_db(n1, w, D, lambda0):
+def longitudinal_misalignment_loss_db(n, w, D, lambda0):
     """
     Calculate the loss due to longitudinal fiber misalignment.
 
     See Ghatak eqn 8.81
 
     Args:
-        n:        index between fiber ends      [-]
-        w:        mode field radius             [m]
-        D:        longitudinal fiber separation [m]
-        lambda0:  wavelength in vacuum          [m]
+        n:        index of medium between fiber ends [-]
+        w:        mode field radius                  [m]
+        D:        longitudinal fiber separation      [m]
+        lambda0:  wavelength in vacuum               [m]
+
     Returns:
         longitudinal misalignment loss dB       [-]
     """
-    dhat = D * lambda0 / (2 * np.pi * n1 * w**2)
+    dhat = D * lambda0 / (2 * np.pi * n * w**2)
     return 10 * np.log10(1 + dhat**2)
 
 
 def _bending_loss_db_scalar(n1, Delta, a, Rc, lambda0):
     """
     Calculate the bending loss in dB/m.
 
@@ -501,14 +519,15 @@
 
     Args:
         a:        core radius                 [m]
         n1:       core index                  [-]
         Delta:    refractive index difference [-]
         Rc:       radius of curvature in      [m]
         lambda0:  wavelength in vacuum in     [m]
+
     Returns:
         bending loss in dB/m                  [1/m]
     """
     k0 = 2 * np.pi / lambda0
     V = k0 * a * n1 * np.sqrt(2 * Delta)
     b = LP_mode_value(V, 0, 1)
     if b is None:
@@ -530,14 +549,15 @@
 
     Args:
         a:        core radius                 [m]
         n1:       core index                  [-]
         Delta:    refractive index difference [-]
         Rc:       radius of curvature in      [m]
         lambda0:  wavelength in vacuum in     [m]
+
     Returns:
         bending loss in dB/m                  [1/m]
     """
     if np.isscalar(a):
         alpha = _bending_loss_db_scalar(n1, Delta, a, Rc, lambda0)
     else:
         alpha = np.empty_like(a)
@@ -554,42 +574,45 @@
     (V > 2.405), it applies to the fundamental mode.
 
     D. Marcuse, "Loss analysis of single-mode fiber splices", Bell Syst.
     Tech. J., 56, 703 (1977)
 
     Args:
         V:      V-parameter of the fiber                            [--]
+
     Returns:
         approximate mode field radius normalized by the core radius [--]
     """
     return 0.65 + 1.619 * V**-1.5 + 2.879 * V**-6
 
 
 def MFD(V):
     """
     Approximate the mode field diameter for a step-index single mode fiber.
 
     See MFR() for details.
 
     Args:
         V:      V-parameter of the fiber                              [--]
+
     Returns:
         approximate mode field diameter normalized by the core radius [--]
     """
     return 2 * MFR(V)
 
 
 def _PetermannW_scalar(V):
     """
     Calculate the Petermann-2 radius for a step-index fiber.
 
     This private method only works when V is a scalar.
 
     Args:
         V:      V-parameter of the fiber                          [--]
+
     Returns:
         approximate Petermann-2 radius normalized by core radius  [--]
     """
     b = LP_mode_value(V, 0, 1)
     if b is None:
         return np.nan
     U = V * np.sqrt(1 - b)
@@ -602,14 +625,15 @@
     """
     Calculate the Petermann-2 radius for a step-index fiber.
 
     This is a convenience function that works when V is an array.
 
     Args:
         V:      V-parameter of the fiber                          [--]
+
     Returns:
         approximate Petermann-2 radius normalized by core radius  [--]
     """
     if np.isscalar(V):
         wp = _PetermannW_scalar(V)
     else:
         wp = np.empty_like(V)
@@ -627,29 +651,32 @@
 
     C. D. Hussey and F. Martinez, “Approximate analytical forms for
        the propagation characteristics of single-mode optical fibres”,
        Electron. Lett. 21, 1103 (1985).
 
     Args:
         V:      V-parameter of the fiber                          [--]
+
     Returns:
         approximate Petermann-2 radius normalized by core radius  [--]
     """
     return MFR(V) - 0.016 - 1.567 * V**-7
 
 
 def _V_d2bV_by_V_scalar(V, ell):
     """
     Calculate V*d^2(bV)/dV^2 for mode ell of a step-index fiber.
 
     This private function only works for scalar values of V and ell. It
     finds V*d^2(bV)/dV^2 for mode ell of a step-index fiber using eqn 10.14
 
     Args:
-        V:      V-parameter of the fiber     [--]
+        V:   V-parameter of the fiber     [--]
+        ell: azimuthal mode number.
+
     Returns:
         V*d^2(bV)/dV^2                       [--]
     """
     b = LP_mode_value(V, ell, 1)
     if b is None:
         return 0
 
@@ -671,14 +698,16 @@
     Calculate V*d^2(bV)/dV^2 for mode ell of a step-index fiber.
 
     This value is needed to determine the waveguide dispersion.  This
     routine is a convenience function that works when V is an array.
 
     Args:
         V:      V-parameter of the fiber     [--]
+        ell: azimuthal mode number.
+
     Returns:
         V*d^2(bV)/dV^2                       [--]
     """
     if np.isscalar(V):
         return _V_d2bV_by_V_scalar(V, ell)
 
     v_by_v = np.empty_like(V)
@@ -694,76 +723,79 @@
 
     This value is needed to determine the waveguide dispersion.  This
     approximation is for the fundamental mode in the fiber and is good
     to 1% when 1.4<V<2.4.  Approximation by Marcuse (1979)
 
     Args:
         V:      V-parameter of the fiber     [--]
+
     Returns:
         V*d^2(bV)/dV^2                       [--]
     """
     return 0.080 + 0.549 * (2.834 - V)**2
 
 
-def _FF_polar_x(ell, ka, theta, V, b):
+def _FF_polar_x(kasin, V, ell, b):
     """
     Polar component of the far-field irradiance polarized in the x-direction.
-    
+
     This implements equation 10.13 from Chen, Foundations for Guided-Wave Optics,
     Wiley-Interscience, 2007.  Use FF_irradiance_x() below to get the far-field
     irradiance.
-    
+
     The polar angle is measured from the optical axis of the fiber.
-    
+
     The product ka is dimensionless and is the product k * a = 2𝜋a/λ
 
     Args:
         ell: azimuthal mode number.
-        ka: wavenumber * fiber radius
-        theta: polar angle to calculate the field (radians).
+        kasin: wavenumber * fiber radius * sin(theta), where
+              theta: polar angle to calculate the field (radians).
         V: normalized frequency parameter of the fiber.
         b: normalized propagation constant.
+
     Returns:
-        The calculated azimuthal field distribution
+        The calculated polar field distribution
     """
-    kasin = ka * np.sin(theta)
     Vb = V * np.sqrt(1 - b)
     ell1 = ell + 1
 
-    Flnumer = kasin * special.jv(ell1, kasin) - (special.jv(ell, kasin) \
-              / special.jv(ell, Vb)) * Vb * special.jv(ell1, Vb)
+    Flnumer = kasin * special.jv(ell1, kasin) - Vb * special.jv(ell1, Vb) * \
+        (special.jv(ell, kasin) / special.jv(ell, Vb))
     Fldenom = (Vb**2 - kasin**2) * (V**2 * b + kasin**2)
 
     return Flnumer / Fldenom
 
 
 def FF_irradiance_x(r, theta, phi, ell, lambda0, a, V, b):
     """
     Normalized far-field irradiance polarized in the x-direction.
 
-    This calculation is based eqn 10.12 for the far-field from Chen, 
-    Foundations for Guided-Wave Optics, Wiley-Interscience, 2007.  
+    This calculation is based eqn 10.12 for the far-field from Chen,
+    Foundations for Guided-Wave Optics, Wiley-Interscience, 2007.
 
     The magnitude of the field is squared and normalized by the square
     of the electric field magnitude.
 
     Args:
         r: radial distance from the fiber axis (microns).
         theta: polar angle in radians.
         phi: azimuthal angle in radians.
         ell: azimuthal mode number.
         lambda0: wavelength of light in the medium (microns).
         a: Radius of the fiber core (microns).
         V: normalized frequency parameter of the fiber.
         b: normalized propagation constant.
+
     Returns:
         The irradiance pattern as a function of r, theta, and phi.
     """
     k = 2 * np.pi / lambda0
-    FF_ell = _FF_polar_x(ell, k*a, theta, V, b)
+    kasin = k*a * np.sin(theta)
+    FF_ell = _FF_polar_x(kasin, V, ell, b)
     FF = FF_ell * (k * a * V)**2 * np.cos(ell * phi) / (k * r)
     return FF**2
 
 
 def FF_polar_irradiance_x(r, theta, ell, lambda0, a, V, b):
     """
     Integral of x-polarized far-field irradiance over all azimuthal angles.
@@ -777,13 +809,170 @@
         r: radial distance from the fiber axis (microns).
         theta: polar angle in radians.
         ell: azimuthal mode number.
         lambda0: Wavelength of light in the medium (microns).
         a: Radius of the fiber core (microns).
         V: Normalized frequency parameter of the fiber.
         b: Normalized propagation constant.
+
     Returns:
         Azimuthally integrated irradiance pattern.
     """
     k = 2 * np.pi / lambda0
-    FF_ell = _FF_polar_x(ell, k*a, theta, V, b)
+    kasin = k*a * np.sin(theta)
+    FF_ell = _FF_polar_x(kasin, V, ell, b)
     return np.pi * (FF_ell * (k * a * V)**2 / (k * r))**2
+
+
+def _FF_node_polar_angle(V, ell, em):
+    """
+    Calculate the smallest nonzero polar angle for scalar V, ell, and em.
+
+    Calculate the smallest nonzero polar angle Θ_N for which the far-field
+    field pattern has a node (zero), for LP mode (ell,em) in a circular
+    step-index fiber.
+
+    The polar angle-dependent factor in the far-field pattern is given by
+    eq. (10.13) in Chen, and here by the function _FF_polar_x.
+    This angle is a standard metric of the angular spread of an optical
+    fiber's output radiation.
+
+    This private function only works for scalar values of V, ell, and em.
+    The use of the public function FF_node_polar_angle is demonstrated in
+    9-Far-field-irradiance.ipynb.
+
+    b is the normalized propagation constant. Each guided mode in an optical
+    fiber has a specific value of b that depends on the fiber parameter V
+    and the mode numbers ell and em.
+
+    If no mode exists, a value of np.nan is returned.
+
+    The LP_lm is specified by (ell,em) to avoid confusion between the
+    number 1 and the letter l.
+
+    For cylindrical fibers, em is a positive integer: thus there are modes
+    LP_01, LP_02, but not LP_10. If em <= 0 or V <= 0, None is returned.
+
+    Implementation details:
+    Bracketing is used to find the zero angle. The initial angle is taken
+    to be just above 0, as fiber modes with ℓ≠0 have nodes at 0
+    itself. The first zero is searched using a bracket upper bound which is a
+    multiple of inc = 1E-2, up to ntry=3000 attempts. These search parameters
+    were found to work well for a realistic fiber, but may be altered to
+    improve efficiency or alternatively to avoid missing a node.
+
+    Args:
+        V:   generalized frequency V for optical fiber (real number)    [-]
+        ell: azimuthal mode number ℓ     (nonnegative integer)          [-]
+        em:  radial mode number m        (positive integer)             [-]
+
+    Returns:
+        polar angle Θ_N of first far-field zero for mode (ℓ,m)          [-]
+    """
+    if ell < 0:
+        ell *= -1   # negative ells are same as positive ones
+
+    if em <= 0:
+        return None    # modes start with 1, e.g., LP_01
+
+    if V <= 0:
+        return None    # V must be positive
+
+    b = LP_mode_value(V, ell, em)
+    if b is None:
+        return np.nan
+    # This occurs when the fiber does not support the (l,m) mode for the given V
+
+    # set up bounds for the zero search
+    lo = 1E-5
+    # kasin = 0 is the lower bound on the function domain.
+    # For ℓ≠0, the function is 0 at 0.
+    # So we start the search for the first nontrivial zero
+    # just above kasin = 0.
+
+    inc = 1E-2
+    hi = inc
+    # we use this as a cautious initial guess. Very few fibers would have
+    # their zero in this initial range. But more importantly, it seems likely no fibers
+    # would have multiple zeros in this range, which would lead to an error condition.
+
+    ntry = 3000
+    f1 = _FF_polar_x(lo, V, ell, b)
+    f2 = _FF_polar_x(hi, V, ell, b)
+
+    for j in range(ntry):
+        if f1*f2 < 0.0:
+            break
+        hi = (j+1)*inc
+        f2 = _FF_polar_x(hi, V, ell, b)
+    else:
+        raise StopIteration(r'No sign change in %d iterations' % ntry)
+
+    return scipy.optimize.brentq(_FF_polar_x, lo, hi, args=(V, ell, b))  # kasinThetaN
+    # We do not suppress any errors from this subroutine, as we want to know if it's working
+
+
+def FF_node_polar_angle(V, ell, em):
+    """
+    Calculate the smallest nonzero polar angle for V, ell, and em.
+
+    Calculate the smallest nonzero polar angle Θ_N for which the far-field
+    field pattern has a node (zero), for LP mode (ell,em) in a circular
+    step-index fiber.
+    The polar angle-dependent factor in the far-field pattern is given by
+    eq. (10.13) in Chen, and here by the function _FF_polar_x.
+    This angle is a standard metric of the angular spread of an optical
+    fiber's output radiation. Note however that the higher the radial
+    mode number m, the smaller the fraction of the irradiance is contained
+    within the first node.
+    The use of this function is demonstrated in
+    9-Far-field-irradiance.ipynb.
+
+    b is the normalized propagation constant. Each guided mode in an optical
+    fiber has a specific value of b that depends on the fiber parameter V
+    and the mode numbers ell and em.
+
+    If no mode exists, a value of np.nan is returned.
+
+    The LP_lm is specified by (ell,em) to avoid confusion between the
+    number 1 and the letter l.
+
+    For cylindrical fibers, em is a positive integer: thus there are modes
+    LP_01, LP_02, but not LP_10. If em <= 0 or V <= 0, None is returned.
+
+    This is a wrapper function that handles V, ell, or em being possible
+    arrays. The private function `_FF_node_polar_angle` contains the
+    details of the calculation itself.
+
+    Args:
+        V:   generalized frequency V for optical fiber (real number)    [-]
+        ell: azimuthal mode number ℓ     (nonnegative integer)          [-]
+        em:  radial mode number m        (positive integer)             [-]
+
+    Returns:
+        polar angle Θ_N of first far-field zero for mode (ℓ,m)          [-]
+    """
+    if em < 1:
+        raise ValueError("The mode number 'em' must be one or greater.")
+
+    if np.isscalar(V) + np.isscalar(ell) + np.isscalar(em) < 2:
+        raise ValueError("only one of V, ell, and em can be an array")
+
+    if not np.isscalar(V):
+        kasin = np.zeros_like(V)
+        for i, VV in enumerate(V):
+            kasin[i] = FF_node_polar_angle(VV, ell, em)
+        return kasin
+
+    if not np.isscalar(ell):
+        kasin = np.zeros_like(ell)
+        for i, ll in enumerate(ell):
+            kasin[i] = FF_node_polar_angle(V, ll, em)
+        return kasin
+
+    if not np.isscalar(em):
+        kasin = np.zeros_like(em)
+        for i, mm in enumerate(em):
+            kasin[i] = FF_node_polar_angle(V, ell, mm)
+        return kasin
+
+    return _FF_node_polar_angle(V, ell, em)
```

### Comparing `ofiber-0.8.0/ofiber/dispersion.py` & `ofiber-0.8.1/ofiber/dispersion.py`

 * *Files identical despite different names*

### Comparing `ofiber-0.8.0/ofiber/graded_index.py` & `ofiber-0.8.1/ofiber/graded_index.py`

 * *Files identical despite different names*

### Comparing `ofiber-0.8.0/ofiber/noise.py` & `ofiber-0.8.1/ofiber/noise.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,47 +26,51 @@
 def shot_noise(I0, Idark, bandwidth, M=1, x=0):
     """
     Return the noise current associated with shot/poisson noise.
 
     Args:
         I0:    current         (A)
         Idark:  dark current    (A)
+        bandwidth:  bandwidth   (Hz)
         M:      APD Gain factor (--)
         x:      excess noise (0.3 for Si, 0.7 for InGaAs, 1.0 for Ge APDs)
+
     Returns:
         shot_noise       (A)
     """
     q = 1.602e-19  # Coulomb
     return np.sqrt(2 * q * (I0 / M + Idark) * bandwidth * M**(2 + x))
 
 
 def thermal_noise(T, Rload, bandwidth):
     """
     Return the noise current associated with thermal processes.
 
     Args:
         T:      temperature (Kelvin)
         Rload:  resistance  (Ohms)
-        BW:     bandwidth   (Hz)
+        bandwidth:     bandwidth   (Hz)
+
     Returns:
         thermal_noise       (A)
     """
     k = 1.38e-23  # J/K
     return np.sqrt(4 * k * T * bandwidth / Rload)
 
 
 def NEP(Responsivity, Rload, Idark, T):
     """
     Return noise equivalent power.
 
     Args:
-        responsivity: photodetector response (A/W)
+        Responsivity: photodetector response (A/W)
         Rload:        resistance             (Ohms)
         Idark:        dark current           (A)
         T:            temperature            (Kelvin)
+
     Returns:
         power       (W/sqrt(Hz))
     """
     q = 1.602e-19  # Coulomb
     k = 1.38e-23   # J/K
     return 1 / Responsivity * np.sqrt(4 * k * T / Rload + 2 * q * Idark)
 
@@ -91,26 +95,28 @@
 
 def BER_at_SNR(snr):
     """
     Return the bit error rate for a particular signal-to-noise ratio.
 
     Args:
         snr: signal to noise ratio (--)
+
     Returns:
         bit error rate              (--)
     """
     return 0.5 * scipy.special.erfc(np.sqrt(snr / 8))
 
 
 def SNR_at_BER(ber):
     """
     Return the necessary signal-to-noise ratio to achieve specified BER.
 
     Args:
         ber: bit error rate (--)
+
     Returns:
         signal to noise ratio (--)
     """
     return 8 * scipy.special.erfcinv(2 * ber)**2
 
 
 def thermal_min_power(bitrate, responsivity, capacitance, T, snr):
@@ -121,14 +127,15 @@
 
     Args:
         bitrate:       bits per second           (Hz)
         responsivity:  photodetector response    (A/W)
         capacitance:   photodetector capacitance (Farads)
         T:             temperature               (Kelvin)
         snr:           signal to noise ratio     (--)
+
     Returns:
         optical power                            (W)
     """
     k = 1.38e-23  # J/K
     val = 2 * np.pi * k * T * capacitance * snr
     return bitrate / responsivity * np.sqrt(val)
 
@@ -137,14 +144,15 @@
     """
     Return the minimum optical power needed to achieve a bit error rate.
 
     Args:
         bitrate:   bits per second      (Hz)
         ber:       bit error rate       (--)
         lambda0:   wavelength in vacuum (m)
+
     Returns:
         optical power                   (W)
     """
     h = 6.626e-34     # J*s
     c = 2.998e8       # m/s
     nu = c / lambda0  # Hz
     Np = -np.log(2 * ber)
```

### Comparing `ofiber-0.8.0/ofiber/planar_parabolic.py` & `ofiber-0.8.1/ofiber/planar_parabolic.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,16 +55,16 @@
     """
     Calculate the waveguide propagation constant beta.
 
     Args:
         m: mode number                                  [-]
         lambda0: wavelength in vacuum                   [m]
         n1: centerline index of refraction of waveguide [-]
-        Delta: relative refractive index                [-]
         a: half thickness of the waveguide              [m]
+        V: the V-parameter for the waveguide
 
     Returns:
         beta for the mth mode
     """
     gamma = np.sqrt(V) / a
     k = 2 * np.pi * n1 / lambda0
     return np.sqrt(k**2 - gamma**2 * (2 * m + 1))
```

### Comparing `ofiber-0.8.0/ofiber/planar_step.py` & `ofiber-0.8.1/ofiber/planar_step.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,16 +121,15 @@
     in turn are needed to determine the propagation factor for a planar
     waveguide.
 
     The planar waveguide characteristics are passed as a 2-element array.
 
     Args:
         xi    : non-dimensional propagation value in waveguide
-        arg[0]: the V-parameter for the waveguide
-        arg[1]: the desired mode (even values are symmetric)
+        *args : array with arg[0]=V-parameter and arg[1]=desired mode
 
     Returns:
         the distance from a solution
     """
     V = args[0]
     mode = args[1]
     if mode % 2 == 0:
@@ -223,21 +222,24 @@
 
     The zeros of eigenvalue equation determine the eigenvalues which
     in turn are needed to determine the propagation factor for a planar
     waveguide.
 
     The planar waveguide characteristics are passed as a 4-element array.
 
-    Args:
-        xi    : non-dimensional propagation value in waveguide
+    The *args is an array with
         arg[0]: the V-parameter for the waveguide
         arg[1]: index of the planar waveguide
         arg[2]: index of the cladding
         arg[3]: the desired mode (even values are symmetric)
 
+    Args:
+        xi    : non-dimensional propagation value in waveguide
+        *args : array described above
+
     Returns:
         the distance from a solution
     """
     V = args[0]
     n1 = args[1]
     n2 = args[2]
     mode = args[3]
@@ -390,14 +392,16 @@
 
 def TM_propagation_constant(V, n1, n2, mode):
     """
     Calculate the propagation constants for TM modes in a planar waveguide.
 
     Args:
         V    : the V-parameter for the waveguide
+        n1   : index of waveguide
+        n2   : index of material next to waveguide
         mode : specific mode
 
     Returns:
         an array of propagation constants for each value of V
     """
     b = np.empty_like(V)
     for i, VV in enumerate(V):
```

### Comparing `ofiber-0.8.0/ofiber/refraction.py` & `ofiber-0.8.1/ofiber/refraction.py`

 * *Files 0% similar despite different names*

```diff
@@ -382,14 +382,15 @@
     The idea is that the glass a combination of silicon dioxide or
     germanium dioxide where x is the molar fraction of GeO_2. Thus
     (1-x) is the molar fraction of SiO_2.  The overall composition is
     x * GeO_2 : (1 - x) * SiO_2.
 
     Args:
         x: fraction of GeO_2 (0<=x<=1)
+
     Returns:
         Sellmeier coefficients for doped glass (array of six values)
     """
     SA = np.array([0.6961663, 0.4079426, 0.8974794])
     SL = np.array([0.0684043, 0.1162414, 9.896161])
     GA = np.array([0.80686642, 0.71815848, 0.85416831])
     GL = np.array([0.068972606, 0.15396605, 11.841931])
@@ -421,14 +422,15 @@
 
     This is intended as a private method.
 
     Args:
         b: array of three Sellmeier Coefficients  [--]
         c: array of three Sellmeier Coefficients  [microns**2]
         lambda0 : wavelength in vacuum             [m]
+
     Returns:
         returns the index of refraction at lambda0 [-]
     """
     lam2 = lambda0**2 * 1e12  # um**2
     nsq = 1
     for i in range(3):
         nsq += b[i] * lam2 / (lam2 - c[i])
@@ -442,14 +444,15 @@
 
     This is a private method.
 
     Args:
         b : array of three Sellmeier Coefficients  [--]
         c : array of three Sellmeier Coefficients  [microns**2]
         lambda0 : wavelength in vacuum             [m]
+
     Returns:
         returns the first derivative of the index of refraction at lambda0 [1/m]
     """
     n1 = _sellmeier(b, c, lambda0)
     lam = lambda0 * 1e6  # microns
     lam2 = lam**2
 
@@ -469,14 +472,15 @@
 
     This is a private method.
 
     Args:
         b : array of three Sellmeier Coefficients  [--]
         c : array of three Sellmeier Coefficients  [microns**2]
         lambda0 : wavelength in vacuum             [m]
+
     Returns:
         returns the second derivative of the refractive index at lambda0 [1/m]
     """
     nn = _sellmeier(b, c, lambda0)    # index of refraction
     lam = lambda0 * 1e6               # needed because Sellmeier uses [um]
     lam2 = lam**2                     # [um**2]
 
@@ -495,53 +499,57 @@
 def n(glass_coef, lambda0):
     """
     Calculate index of refraction for a glass at a wavelength.
 
     Args:
         glass_coef: array of Sellmeier coefficients obtained from glass(i)
         lambda0: wavelength in vacuum [m]
+
     Returns:
         index of refraction [--]
     """
     return _sellmeier(glass_coef[3:6], glass_coef[0:3], lambda0)
 
 
 def dn(glass_coef, lambda0):
     """
     Calculate the first derivative of the refractive index w.r.t. wavelength.
 
     Args:
         glass_coef: array of Sellmeier coefficients obtained from glass(i)
         lambda0: wavelength in vacuum [m]
+
     Returns:
         the first derivative of index of refraction [1/m]
     """
     return _d_sellmeier(glass_coef[3:6], glass_coef[0:3], lambda0)
 
 
 def d2n(glass_coef, lambda0):
     """
     Calculate the second derivative of the refractive index w.r.t. wavelength.
 
     Args:
         glass_coef: array of Sellmeier coefficients obtained from glass(i)
         lambda0: wavelength in vacuum [m]
+
     Returns:
         the second derivative of index of refraction [1/m**2]
     """
     return _d2_sellmeier(glass_coef[3:6], glass_coef[0:3], lambda0)
 
 
 def n_group(glass_coef, lambda0):
     """
     Calculate group index of refraction at a wavelength.
 
     Args:
-        glass: array of Sellmeier coefficients obtained from glass(i)
+        glass_coef: array of Sellmeier coefficients obtained from glass(i)
         lambda0: wavelength in vacuum [m]
+
     Returns:
         group index of refraction [--]
     """
     return n(glass_coef, lambda0) - lambda0 * dn(glass_coef, lambda0)
 
 
 def n_air(lambda0, temperature=15):
```

### Comparing `ofiber-0.8.0/setup.cfg` & `ofiber-0.8.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 classifiers = 
 	Development Status :: 3 - Alpha
 	License :: OSI Approved :: MIT License
 	Intended Audience :: Science/Research
 	Programming Language :: Python
 	Topic :: Scientific/Engineering :: Physics
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 keywords = 
 	refraction
 	Sellmeier
 	modes
 	dispersion
 	graded index
 	gradient index
```

### Comparing `ofiber-0.8.0/setup.py` & `ofiber-0.8.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Configure the ofiber module."""
 import re
 import os.path
 from setuptools import setup
 
 project = 'ofiber'
```

### Comparing `ofiber-0.8.0/tests/test_all_notebooks.py` & `ofiber-0.8.1/tests/test_all_notebooks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pylint: disable=invalid-name
 """
 This file is intended to be the target of a pytest run.
 
 It recursively finds all `.ipynb` files in the docs directory, ignoring
 directories that start with '.' and any files matching patterns found in the file
-`.testignore`
+`.testignore`.
 
 Sample invocations of pytest which make the output nicely readable::
 
     pytest --verbose --durations=5 test_all_notebooks.py
 
 If you install `pytest-xdist` you can run tests in parallel with::
 
@@ -44,15 +44,16 @@
 
 notebooks.sort()
 ids = [str(n) for n in notebooks]
 
 
 @pytest.mark.parametrize("notebook", notebooks, ids=ids)
 def test_run_notebook(notebook):
-    """Read and execute notebook
+    """
+    Read and execute notebook.
 
     The method here is directly from the nbconvert docs
 
     There is no error handling as any errors will be caught by pytest
     """
     with open(notebook, encoding='utf-8') as f:
         nb = nbformat.read(f, as_version=4)
```

