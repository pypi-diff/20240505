# Comparing `tmp/jax_sysid-0.4.0.tar.gz` & `tmp/jax_sysid-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax_sysid-0.4.0.tar", last modified: Sat May  4 08:10:17 2024, max compression
+gzip compressed data, was "jax_sysid-0.4.1.tar", last modified: Sun May  5 08:18:06 2024, max compression
```

## Comparing `jax_sysid-0.4.0.tar` & `jax_sysid-0.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-05-04 08:10:17.025794 jax_sysid-0.4.0/
--rw-r--r--   0 bemporad   (501) staff       (20)    11345 2024-03-01 16:55:21.000000 jax_sysid-0.4.0/LICENSE.txt
--rw-r--r--   0 bemporad   (501) staff       (20)    14758 2024-05-04 08:10:17.025594 jax_sysid-0.4.0/PKG-INFO
--rw-r--r--   0 bemporad   (501) staff       (20)    13958 2024-05-04 08:02:06.000000 jax_sysid-0.4.0/README.md
--rw-r--r--   0 bemporad   (501) staff       (20)      801 2024-05-04 06:04:03.000000 jax_sysid-0.4.0/pyproject.toml
--rw-r--r--   0 bemporad   (501) staff       (20)       38 2024-05-04 08:10:17.025833 jax_sysid-0.4.0/setup.cfg
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-05-04 08:10:17.023730 jax_sysid-0.4.0/src/
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-05-04 08:10:17.024522 jax_sysid-0.4.0/src/jax_sysid/
--rw-r--r--   0 bemporad   (501) staff       (20)        0 2023-01-10 11:29:35.000000 jax_sysid-0.4.0/src/jax_sysid/__init__.py
--rw-r--r--   0 bemporad   (501) staff       (20)    73689 2024-05-04 07:53:55.000000 jax_sysid-0.4.0/src/jax_sysid/models.py
--rw-r--r--   0 bemporad   (501) staff       (20)    11403 2024-05-03 09:46:56.000000 jax_sysid-0.4.0/src/jax_sysid/utils.py
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-05-04 08:10:17.025399 jax_sysid-0.4.0/src/jax_sysid.egg-info/
--rw-r--r--   0 bemporad   (501) staff       (20)    14758 2024-05-04 08:10:17.000000 jax_sysid-0.4.0/src/jax_sysid.egg-info/PKG-INFO
--rw-r--r--   0 bemporad   (501) staff       (20)      314 2024-05-04 08:10:17.000000 jax_sysid-0.4.0/src/jax_sysid.egg-info/SOURCES.txt
--rw-r--r--   0 bemporad   (501) staff       (20)        1 2024-05-04 08:10:17.000000 jax_sysid-0.4.0/src/jax_sysid.egg-info/dependency_links.txt
--rw-r--r--   0 bemporad   (501) staff       (20)       49 2024-05-04 08:10:17.000000 jax_sysid-0.4.0/src/jax_sysid.egg-info/requires.txt
--rw-r--r--   0 bemporad   (501) staff       (20)       10 2024-05-04 08:10:17.000000 jax_sysid-0.4.0/src/jax_sysid.egg-info/top_level.txt
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-05-04 08:10:17.025246 jax_sysid-0.4.0/tests/
--rw-r--r--   0 bemporad   (501) staff       (20)     5280 2024-03-06 15:24:05.000000 jax_sysid-0.4.0/tests/test_models.py
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-05-05 08:18:06.960465 jax_sysid-0.4.1/
+-rw-r--r--   0 bemporad   (501) staff       (20)    11345 2024-03-01 16:55:21.000000 jax_sysid-0.4.1/LICENSE.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)    14758 2024-05-05 08:18:06.960272 jax_sysid-0.4.1/PKG-INFO
+-rw-r--r--   0 bemporad   (501) staff       (20)    13958 2024-05-04 08:02:06.000000 jax_sysid-0.4.1/README.md
+-rw-r--r--   0 bemporad   (501) staff       (20)      801 2024-05-05 08:15:45.000000 jax_sysid-0.4.1/pyproject.toml
+-rw-r--r--   0 bemporad   (501) staff       (20)       38 2024-05-05 08:18:06.960501 jax_sysid-0.4.1/setup.cfg
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-05-05 08:18:06.958312 jax_sysid-0.4.1/src/
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-05-05 08:18:06.959144 jax_sysid-0.4.1/src/jax_sysid/
+-rw-r--r--   0 bemporad   (501) staff       (20)        0 2023-01-10 11:29:35.000000 jax_sysid-0.4.1/src/jax_sysid/__init__.py
+-rw-r--r--   0 bemporad   (501) staff       (20)    73696 2024-05-05 08:14:08.000000 jax_sysid-0.4.1/src/jax_sysid/models.py
+-rw-r--r--   0 bemporad   (501) staff       (20)    11403 2024-05-03 09:46:56.000000 jax_sysid-0.4.1/src/jax_sysid/utils.py
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-05-05 08:18:06.960052 jax_sysid-0.4.1/src/jax_sysid.egg-info/
+-rw-r--r--   0 bemporad   (501) staff       (20)    14758 2024-05-05 08:18:06.000000 jax_sysid-0.4.1/src/jax_sysid.egg-info/PKG-INFO
+-rw-r--r--   0 bemporad   (501) staff       (20)      314 2024-05-05 08:18:06.000000 jax_sysid-0.4.1/src/jax_sysid.egg-info/SOURCES.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)        1 2024-05-05 08:18:06.000000 jax_sysid-0.4.1/src/jax_sysid.egg-info/dependency_links.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)       49 2024-05-05 08:18:06.000000 jax_sysid-0.4.1/src/jax_sysid.egg-info/requires.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)       10 2024-05-05 08:18:06.000000 jax_sysid-0.4.1/src/jax_sysid.egg-info/top_level.txt
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-05-05 08:18:06.959861 jax_sysid-0.4.1/tests/
+-rw-r--r--   0 bemporad   (501) staff       (20)     5280 2024-03-06 15:24:05.000000 jax_sysid-0.4.1/tests/test_models.py
```

### Comparing `jax_sysid-0.4.0/LICENSE.txt` & `jax_sysid-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jax_sysid-0.4.0/PKG-INFO` & `jax_sysid-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-sysid
-Version: 0.4.0
+Version: 0.4.1
 Summary: jax-sysid - A Python package for linear and nonlinear system identification and nonlinear regression using Jax.
 Author-email: Alberto Bemporad <alberto.bemporad@imtlucca.it>
 Project-URL: Homepage, http://cse.lab.imtlucca.it/~bemporad/jax-sysid
 Keywords: system identification,subspace identification,nonlinear regression
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `jax_sysid-0.4.0/README.md` & `jax_sysid-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `jax_sysid-0.4.0/pyproject.toml` & `jax_sysid-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jax-sysid"
-version = "0.4.0"
+version = "0.4.1"
 authors = [
   { name="Alberto Bemporad", email="alberto.bemporad@imtlucca.it" },
 ]
 description = "jax-sysid - A Python package for linear and nonlinear system identification and nonlinear regression using Jax."
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = ["numpy","scipy","jax","jaxopt","flax","tqdm","matplotlib","pmlb"]
```

### Comparing `jax_sysid-0.4.0/src/jax_sysid/models.py` & `jax_sysid-0.4.1/src/jax_sysid/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1788,15 +1788,15 @@
                         if isCustomReg:
                             cost += self.custom_regularization(th)
                         return cost
 
                     solver = jaxopt.ScipyBoundedMinimize(
                         fun=J, tol=self.lbfgs_tol, method="L-BFGS-B", maxiter=solver_iters, options=options)
                     bounds = get_bounds(
-                        z, epsil_lasso, self.params_min, self.params_max)
+                        z[0:nth], epsil_lasso, self.params_min, self.params_max)
                     z, state = solver.run(z, bounds=bounds)
                     z[0:nth] = [
                         z1 - z2 for (z1, z2) in zip(z[0:nth], z[nth:2 * nth])]
                     iter_num = state.iter_num
                     Jopt = state.fun_val
 
                 if self.iprint > -1:
```

### Comparing `jax_sysid-0.4.0/src/jax_sysid/utils.py` & `jax_sysid-0.4.1/src/jax_sysid/utils.py`

 * *Files identical despite different names*

### Comparing `jax_sysid-0.4.0/src/jax_sysid.egg-info/PKG-INFO` & `jax_sysid-0.4.1/src/jax_sysid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-sysid
-Version: 0.4.0
+Version: 0.4.1
 Summary: jax-sysid - A Python package for linear and nonlinear system identification and nonlinear regression using Jax.
 Author-email: Alberto Bemporad <alberto.bemporad@imtlucca.it>
 Project-URL: Homepage, http://cse.lab.imtlucca.it/~bemporad/jax-sysid
 Keywords: system identification,subspace identification,nonlinear regression
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `jax_sysid-0.4.0/tests/test_models.py` & `jax_sysid-0.4.1/tests/test_models.py`

 * *Files identical despite different names*

