# Comparing `tmp/sde_simulator-0.1.91.tar.gz` & `tmp/sde_simulator-0.1.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sde_simulator-0.1.91.tar", last modified: Wed Feb 21 08:00:56 2024, max compression
+gzip compressed data, was "sde_simulator-0.1.92.tar", last modified: Sun May  5 09:50:16 2024, max compression
```

## Comparing `sde_simulator-0.1.91.tar` & `sde_simulator-0.1.92.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 odedwer   (1000) odedwer   (1000)        0 2024-02-21 08:00:56.257652 sde_simulator-0.1.91/
--rw-rw-r--   0 odedwer   (1000) odedwer   (1000)      828 2024-02-21 08:00:56.257652 sde_simulator-0.1.91/PKG-INFO
--rw-rw-r--   0 odedwer   (1000) odedwer   (1000)      338 2022-12-28 10:40:31.000000 sde_simulator-0.1.91/README.md
-drwxrwxr-x   0 odedwer   (1000) odedwer   (1000)        0 2024-02-21 08:00:56.257652 sde_simulator-0.1.91/sde_simulator/
--rw-rw-r--   0 odedwer   (1000) odedwer   (1000)       28 2022-12-28 10:40:31.000000 sde_simulator-0.1.91/sde_simulator/__init__.py
--rw-rw-r--   0 odedwer   (1000) odedwer   (1000)     3624 2024-02-21 07:59:17.000000 sde_simulator-0.1.91/sde_simulator/sde_simulator.py
-drwxrwxr-x   0 odedwer   (1000) odedwer   (1000)        0 2024-02-21 08:00:56.257652 sde_simulator-0.1.91/sde_simulator.egg-info/
--rw-rw-r--   0 odedwer   (1000) odedwer   (1000)      828 2024-02-21 08:00:56.000000 sde_simulator-0.1.91/sde_simulator.egg-info/PKG-INFO
--rw-rw-r--   0 odedwer   (1000) odedwer   (1000)      259 2024-02-21 08:00:56.000000 sde_simulator-0.1.91/sde_simulator.egg-info/SOURCES.txt
--rw-rw-r--   0 odedwer   (1000) odedwer   (1000)        1 2024-02-21 08:00:56.000000 sde_simulator-0.1.91/sde_simulator.egg-info/dependency_links.txt
--rw-rw-r--   0 odedwer   (1000) odedwer   (1000)       11 2024-02-21 08:00:56.000000 sde_simulator-0.1.91/sde_simulator.egg-info/requires.txt
--rw-rw-r--   0 odedwer   (1000) odedwer   (1000)       14 2024-02-21 08:00:56.000000 sde_simulator-0.1.91/sde_simulator.egg-info/top_level.txt
--rw-rw-r--   0 odedwer   (1000) odedwer   (1000)       38 2024-02-21 08:00:56.257652 sde_simulator-0.1.91/setup.cfg
--rw-rw-r--   0 odedwer   (1000) odedwer   (1000)     1028 2024-02-21 07:59:21.000000 sde_simulator-0.1.91/setup.py
+drwxrwxr-x   0 odedwer   (1000) odedwer   (1000)        0 2024-05-05 09:50:16.621609 sde_simulator-0.1.92/
+-rw-r--r--   0 odedwer   (1000) odedwer   (1000)      850 2024-05-05 09:50:16.621609 sde_simulator-0.1.92/PKG-INFO
+-rw-rw-r--   0 odedwer   (1000) odedwer   (1000)      338 2022-12-28 10:40:31.000000 sde_simulator-0.1.92/README.md
+drwxrwxr-x   0 odedwer   (1000) odedwer   (1000)        0 2024-05-05 09:50:16.621609 sde_simulator-0.1.92/sde_simulator/
+-rw-rw-r--   0 odedwer   (1000) odedwer   (1000)       28 2022-12-28 10:40:31.000000 sde_simulator-0.1.92/sde_simulator/__init__.py
+-rw-rw-r--   0 odedwer   (1000) odedwer   (1000)     3582 2024-05-05 09:32:35.000000 sde_simulator-0.1.92/sde_simulator/sde_simulator.py
+drwxrwxr-x   0 odedwer   (1000) odedwer   (1000)        0 2024-05-05 09:50:16.621609 sde_simulator-0.1.92/sde_simulator.egg-info/
+-rw-r--r--   0 odedwer   (1000) odedwer   (1000)      850 2024-05-05 09:50:16.000000 sde_simulator-0.1.92/sde_simulator.egg-info/PKG-INFO
+-rw-rw-r--   0 odedwer   (1000) odedwer   (1000)      259 2024-05-05 09:50:16.000000 sde_simulator-0.1.92/sde_simulator.egg-info/SOURCES.txt
+-rw-rw-r--   0 odedwer   (1000) odedwer   (1000)        1 2024-05-05 09:50:16.000000 sde_simulator-0.1.92/sde_simulator.egg-info/dependency_links.txt
+-rw-rw-r--   0 odedwer   (1000) odedwer   (1000)       11 2024-05-05 09:50:16.000000 sde_simulator-0.1.92/sde_simulator.egg-info/requires.txt
+-rw-rw-r--   0 odedwer   (1000) odedwer   (1000)       14 2024-05-05 09:50:16.000000 sde_simulator-0.1.92/sde_simulator.egg-info/top_level.txt
+-rw-rw-r--   0 odedwer   (1000) odedwer   (1000)       38 2024-05-05 09:50:16.621609 sde_simulator-0.1.92/setup.cfg
+-rw-rw-r--   0 odedwer   (1000) odedwer   (1000)     1028 2024-05-05 09:32:35.000000 sde_simulator-0.1.92/setup.py
```

### Comparing `sde_simulator-0.1.91/PKG-INFO` & `sde_simulator-0.1.92/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: sde_simulator
-Version: 0.1.91
+Version: 0.1.92
 Summary: General base class implementation of Rung-Kutta SDE solver
 Home-page: https://github.com/odedwer/sde_simulator
 Author: Oded Wertheimer
 Author-email: oded.wertheimer@mail.huji.ac.il
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: numpy
+Requires-Dist: tqdm
 
 This package provides a base class for simulating SDE using Rung-Kutta method.
 The base class implements the simulation and requires the override of the deterministic and stochastic methods of the model.
-
```

### Comparing `sde_simulator-0.1.91/sde_simulator/sde_simulator.py` & `sde_simulator-0.1.92/sde_simulator/sde_simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,19 +70,17 @@
     def time(self):
         return self._time
 
     @property
     def noise(self):
         return self._noise
 
-    @lru_cache(None)
     def dW(self, t):
         return self._generated_dw[t]
 
-    @lru_cache(None)
     def dWsquared(self, t):
         return self._generated_dw_squared[t]
 
     @abstractmethod
     def deterministic_func(self, y, i, **kwargs):
         pass
```

### Comparing `sde_simulator-0.1.91/sde_simulator.egg-info/PKG-INFO` & `sde_simulator-0.1.92/sde_simulator.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: sde-simulator
-Version: 0.1.91
+Name: sde_simulator
+Version: 0.1.92
 Summary: General base class implementation of Rung-Kutta SDE solver
 Home-page: https://github.com/odedwer/sde_simulator
 Author: Oded Wertheimer
 Author-email: oded.wertheimer@mail.huji.ac.il
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: numpy
+Requires-Dist: tqdm
 
 This package provides a base class for simulating SDE using Rung-Kutta method.
 The base class implements the simulation and requires the override of the deterministic and stochastic methods of the model.
-
```

### Comparing `sde_simulator-0.1.91/setup.py` & `sde_simulator-0.1.92/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='sde_simulator',
-    version='0.1.91',
+    version='0.1.92',
     description="General base class implementation of Rung-Kutta SDE solver",
     long_description="This package provides a base class for simulating SDE using Rung-Kutta method.\n"
                      "The base class implements the simulation and requires the override of the deterministic and "
                      "stochastic methods of the model.",
     author="Oded Wertheimer",
     author_email="oded.wertheimer@mail.huji.ac.il",
     packages=["sde_simulator"],
```

