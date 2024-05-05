# Comparing `tmp/deep_river-0.2.5.tar.gz` & `tmp/deep_river-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deep_river-0.2.5.tar", last modified: Wed Aug 30 20:39:09 2023, max compression
+gzip compressed data, was "deep_river-0.2.6.tar", last modified: Sun May  5 21:04:05 2024, max compression
```

## Comparing `deep_river-0.2.5.tar` & `deep_river-0.2.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 20:39:09.879679 deep_river-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (999)     1522 2023-08-30 20:38:54.000000 deep_river-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)     6666 2023-08-30 20:39:09.879679 deep_river-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     5855 2023-08-30 20:38:54.000000 deep_river-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 20:39:09.875679 deep_river-0.2.5/deep_river/
--rw-r--r--   0 runner    (1001) docker     (999)      172 2023-08-30 20:38:54.000000 deep_river-0.2.5/deep_river/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)       77 2023-08-30 20:38:54.000000 deep_river-0.2.5/deep_river/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 20:39:09.875679 deep_river-0.2.5/deep_river/anomaly/
--rw-r--r--   0 runner    (1001) docker     (999)      507 2023-08-30 20:38:54.000000 deep_river-0.2.5/deep_river/anomaly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     8021 2023-08-30 20:38:54.000000 deep_river-0.2.5/deep_river/anomaly/ae.py
--rw-r--r--   0 runner    (1001) docker     (999)     6397 2023-08-30 20:38:54.000000 deep_river-0.2.5/deep_river/anomaly/probability_weighted_ae.py
--rw-r--r--   0 runner    (1001) docker     (999)     8123 2023-08-30 20:38:54.000000 deep_river-0.2.5/deep_river/anomaly/rolling_ae.py
--rw-r--r--   0 runner    (1001) docker     (999)     8292 2023-08-30 20:38:54.000000 deep_river-0.2.5/deep_river/anomaly/scaler.py
--rw-r--r--   0 runner    (1001) docker     (999)     7744 2023-08-30 20:38:54.000000 deep_river-0.2.5/deep_river/base.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 20:39:09.875679 deep_river-0.2.5/deep_river/classification/
--rw-r--r--   0 runner    (1001) docker     (999)      416 2023-08-30 20:38:54.000000 deep_river-0.2.5/deep_river/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    12899 2023-08-30 20:38:54.000000 deep_river-0.2.5/deep_river/classification/classifier.py
--rw-r--r--   0 runner    (1001) docker     (999)    23003 2023-08-30 20:38:54.000000 deep_river-0.2.5/deep_river/classification/rolling_classifier.py
--rw-r--r--   0 runner    (1001) docker     (999)     8414 2023-08-30 20:38:54.000000 deep_river-0.2.5/deep_river/classification/zoo.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 20:39:09.875679 deep_river-0.2.5/deep_river/regression/
--rw-r--r--   0 runner    (1001) docker     (999)      491 2023-08-30 20:38:54.000000 deep_river-0.2.5/deep_river/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     5982 2023-08-30 20:38:54.000000 deep_river-0.2.5/deep_river/regression/multioutput.py
--rw-r--r--   0 runner    (1001) docker     (999)     6513 2023-08-30 20:38:54.000000 deep_river-0.2.5/deep_river/regression/regressor.py
--rw-r--r--   0 runner    (1001) docker     (999)     6918 2023-08-30 20:38:54.000000 deep_river-0.2.5/deep_river/regression/rolling_regressor.py
--rw-r--r--   0 runner    (1001) docker     (999)     4821 2023-08-30 20:38:54.000000 deep_river-0.2.5/deep_river/regression/zoo.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 20:39:09.879679 deep_river-0.2.5/deep_river/utils/
--rw-r--r--   0 runner    (1001) docker     (999)      555 2023-08-30 20:38:54.000000 deep_river-0.2.5/deep_river/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      538 2023-08-30 20:38:54.000000 deep_river-0.2.5/deep_river/utils/estimator_checks.py
--rw-r--r--   0 runner    (1001) docker     (999)      541 2023-08-30 20:38:54.000000 deep_river-0.2.5/deep_river/utils/hooks.py
--rw-r--r--   0 runner    (1001) docker     (999)     4098 2023-08-30 20:38:54.000000 deep_river-0.2.5/deep_river/utils/params.py
--rw-r--r--   0 runner    (1001) docker     (999)     3923 2023-08-30 20:38:54.000000 deep_river-0.2.5/deep_river/utils/tensor_conversion.py
--rw-r--r--   0 runner    (1001) docker     (999)     1327 2023-08-30 20:38:54.000000 deep_river-0.2.5/deep_river/utils/test_estimators.py
--rw-r--r--   0 runner    (1001) docker     (999)     3052 2023-08-30 20:38:54.000000 deep_river-0.2.5/deep_river/utils/test_tensor_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 20:39:09.875679 deep_river-0.2.5/deep_river.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     6666 2023-08-30 20:39:09.000000 deep_river-0.2.5/deep_river.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     1025 2023-08-30 20:39:09.000000 deep_river-0.2.5/deep_river.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-30 20:39:09.000000 deep_river-0.2.5/deep_river.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)     1687 2023-08-30 20:39:09.000000 deep_river-0.2.5/deep_river.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       11 2023-08-30 20:39:09.000000 deep_river-0.2.5/deep_river.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)     1251 2023-08-30 20:38:54.000000 deep_river-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)      103 2023-08-30 20:39:09.879679 deep_river-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     3074 2023-08-30 20:38:54.000000 deep_river-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:05.950366 deep_river-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-05 21:03:59.000000 deep_river-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11211 2024-05-05 21:04:05.950366 deep_river-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-05-05 21:03:59.000000 deep_river-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:05.934366 deep_river-0.2.6/deep_river/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-05 21:03:59.000000 deep_river-0.2.6/deep_river/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-05 21:03:59.000000 deep_river-0.2.6/deep_river/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:05.938366 deep_river-0.2.6/deep_river/anomaly/
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-05 21:03:59.000000 deep_river-0.2.6/deep_river/anomaly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8004 2024-05-05 21:03:59.000000 deep_river-0.2.6/deep_river/anomaly/ae.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-05 21:03:59.000000 deep_river-0.2.6/deep_river/anomaly/probability_weighted_ae.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8123 2024-05-05 21:03:59.000000 deep_river-0.2.6/deep_river/anomaly/rolling_ae.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-05-05 21:03:59.000000 deep_river-0.2.6/deep_river/anomaly/scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-05-05 21:03:59.000000 deep_river-0.2.6/deep_river/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:05.938366 deep_river-0.2.6/deep_river/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-05 21:03:59.000000 deep_river-0.2.6/deep_river/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12887 2024-05-05 21:03:59.000000 deep_river-0.2.6/deep_river/classification/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22986 2024-05-05 21:03:59.000000 deep_river-0.2.6/deep_river/classification/rolling_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-05-05 21:03:59.000000 deep_river-0.2.6/deep_river/classification/zoo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:05.938366 deep_river-0.2.6/deep_river/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-05 21:03:59.000000 deep_river-0.2.6/deep_river/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-05-05 21:03:59.000000 deep_river-0.2.6/deep_river/regression/multioutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6513 2024-05-05 21:03:59.000000 deep_river-0.2.6/deep_river/regression/regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-05-05 21:03:59.000000 deep_river-0.2.6/deep_river/regression/rolling_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-05 21:03:59.000000 deep_river-0.2.6/deep_river/regression/zoo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:05.938366 deep_river-0.2.6/deep_river/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-05 21:03:59.000000 deep_river-0.2.6/deep_river/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-05 21:03:59.000000 deep_river-0.2.6/deep_river/utils/estimator_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-05 21:03:59.000000 deep_river-0.2.6/deep_river/utils/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-05-05 21:03:59.000000 deep_river-0.2.6/deep_river/utils/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-05 21:03:59.000000 deep_river-0.2.6/deep_river/utils/tensor_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-05 21:03:59.000000 deep_river-0.2.6/deep_river/utils/test_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-05 21:03:59.000000 deep_river-0.2.6/deep_river/utils/test_tensor_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:05.942366 deep_river-0.2.6/deep_river.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11211 2024-05-05 21:04:05.000000 deep_river-0.2.6/deep_river.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-05 21:04:05.000000 deep_river-0.2.6/deep_river.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 21:04:05.000000 deep_river-0.2.6/deep_river.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-05 21:04:05.000000 deep_river-0.2.6/deep_river.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-05 21:04:05.000000 deep_river-0.2.6/deep_river.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-05 21:03:59.000000 deep_river-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-05 21:04:05.950366 deep_river-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-05-05 21:03:59.000000 deep_river-0.2.6/setup.py
```

### Comparing `deep_river-0.2.5/LICENSE` & `deep_river-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `deep_river-0.2.5/PKG-INFO` & `deep_river-0.2.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: deep_river
-Version: 0.2.5
-Summary: Online Deep Learning for river
-Home-page: https://online-ml.github.io/deep-river/
-Author: Cedric Kulbach
-Author-email: cedric.kulbach@googlemail.com
-License: BSD-3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: docs
-Provides-Extra: all
-License-File: LICENSE
-
-
 <p align="center">
   <img height="150px" src="https://raw.githubusercontent.com/online-ml/deep-river/master/docs/img/logo.png" alt="incremental dl logo">
 </p>
 <p align="center">
     <img alt="PyPI" src="https://img.shields.io/pypi/v/deep-river">
     <a href="https://codecov.io/gh/online-ml/deep-river" > 
         <img src="https://codecov.io/gh/online-ml/deep-river/branch/master/graph/badge.svg?token=ZKUIISZAYA"/> 
@@ -94,18 +70,18 @@
 ... )
 
 >>> dataset = datasets.Phishing()
 >>> metric = metrics.Accuracy()
 
 >>> for x, y in dataset:
 ...     y_pred = model_pipeline.predict_one(x)  # make a prediction
-...     metric = metric.update(y, y_pred)  # update the metric
-...     model_pipeline = model_pipeline.learn_one(x, y)  # make the model learn
+...     metric.update(y, y_pred)  # update the metric
+...     model_pipeline.learn_one(x, y)  # make the model learn
 >>> print(f"Accuracy: {metric.get():.4f}")
-Accuracy: 0.6728
+Accuracy: 0.6736
 
 ```
 ### Multi Target Regression 
 ```python
 >>> from river import evaluate, compose
 >>> from river import metrics
 >>> from river import preprocessing
@@ -135,15 +111,15 @@
 ...         loss_fn='mse',
 ...         lr=0.3,
 ...         optimizer_fn='sgd',
 ...     ))
 >>> metric = metrics.multioutput.MicroAverage(metrics.MAE())
 >>> ev = evaluate.progressive_val_score(dataset, model, metric)
 >>> print(f"MicroAverage(MAE): {metric.get():.2f}")
-MicroAverage(MAE): 28.36
+MicroAverage(MAE): 34.31
 
 ```
 
 ### Anomaly Detection
 
 ```python
 >>> from deep_river.anomaly import Autoencoder
@@ -173,20 +149,24 @@
 
 >>> ae = Autoencoder(module=MyAutoEncoder, lr=0.005)
 >>> scaler = MinMaxScaler()
 >>> model = Pipeline(scaler, ae)
 
 >>> for x, y in dataset:
 ...     score = model.score_one(x)
-...     model = model.learn_one(x=x)
-...     metric = metric.update(y, score)
+...     model.learn_one(x=x)
+...     metric.update(y, score)
 ...
 >>> print(f"ROCAUC: {metric.get():.4f}")
-ROCAUC: 0.7447
+ROCAUC: 0.9017
 
 ```
 
 ## 🏫 Affiliations
 
 <p align="center">
     <img src="https://upload.wikimedia.org/wikipedia/de/thumb/4/44/Fzi_logo.svg/1200px-Fzi_logo.svg.png?raw=true" alt="FZI Logo" height="200"/>
 </p>
+
+<p align="center">
+    <img src="https://lieferbotnet.de/wp-content/uploads/2022/09/LieferBotNet-Logo.png?raw=true" alt="Lieferbot net" height="200"/>
+</p>
```

### Comparing `deep_river-0.2.5/deep_river/anomaly/ae.py` & `deep_river-0.2.6/deep_river/anomaly/ae.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,19 +85,19 @@
 
     >>> ae = Autoencoder(module=MyAutoEncoder, lr=0.005)
     >>> scaler = MinMaxScaler()
     >>> model = Pipeline(scaler, ae)
 
     >>> for x, y in dataset:
     ...    score = model.score_one(x)
-    ...    model = model.learn_one(x=x)
-    ...    metric = metric.update(y, score)
+    ...    model.learn_one(x=x)
+    ...    metric.update(y, score)
     ...
     >>> print(f"ROCAUC: {metric.get():.4f}")
-    ROCAUC: 0.7447
+    ROCAUC: 0.9017
     """
 
     def __init__(
         self,
         module: Type[torch.nn.Module],
         loss_fn: Union[str, Callable] = "mse",
         optimizer_fn: Union[str, Callable] = "sgd",
```

### Comparing `deep_river-0.2.5/deep_river/anomaly/probability_weighted_ae.py` & `deep_river-0.2.6/deep_river/anomaly/probability_weighted_ae.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,16 +79,16 @@
 
     >>> ae = ProbabilityWeightedAutoencoder(module=MyAutoEncoder, lr=0.005)
     >>> scaler = MinMaxScaler()
     >>> model = Pipeline(scaler, ae)
 
     >>> for x, y in dataset:
     ...    score = model.score_one(x)
-    ...    model = model.learn_one(x=x)
-    ...    metric = metric.update(y, score)
+    ...    model.learn_one(x=x)
+    ...    metric.update(y, score)
     ...
     >>> print(f"ROCAUC: {metric.get():.4f}")
     ROCAUC: 0.8599
     """
 
     def __init__(
         self,
```

### Comparing `deep_river-0.2.5/deep_river/anomaly/rolling_ae.py` & `deep_river-0.2.6/deep_river/anomaly/rolling_ae.py`

 * *Files identical despite different names*

### Comparing `deep_river-0.2.5/deep_river/anomaly/scaler.py` & `deep_river-0.2.6/deep_river/anomaly/scaler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import abc
 
 import numpy as np
 from river import base, utils
 from river.anomaly import HalfSpaceTrees
 from river.anomaly.base import AnomalyDetector
-from river.stats import Mean, Min
+from river.stats import Mean, Min, RollingMin
 
 
 class AnomalyScaler(base.Wrapper, AnomalyDetector):
     """Wrapper around an anomaly detector that scales the output of the model
     to account for drift in the wrapped model's anomaly scores.
 
     Parameters
@@ -255,20 +255,16 @@
         anomaly_detector: AnomalyDetector,
         rolling: bool = True,
         window_size: int = 250,
     ):
         super().__init__(anomaly_detector)
         self.rolling = rolling
         self.window_size = window_size
-        self.min = (
-            utils.Rolling(Min(), self.window_size) if self.rolling else Min()
-        )
-        self.max = (
-            utils.Rolling(Min(), self.window_size) if self.rolling else Min()
-        )
+        self.min = RollingMin(self.window_size) if self.rolling else Min()
+        self.max = RollingMin(self.window_size) if self.rolling else Min()
 
     def score_one(self, *args):
         """
         Return a scaled anomaly score based on raw score provided by the
         wrapped anomaly detector. Larger values indicate more
         anomalous examples.
```

### Comparing `deep_river-0.2.5/deep_river/base.py` & `deep_river-0.2.6/deep_river/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-import abc
 import collections
 import inspect
-from typing import Any, Callable, Deque, Optional, Type, Union, cast
+from typing import Any, Callable, Deque, Type, Union, cast
 
 import torch
 from river import base
 
 from deep_river.utils import get_loss_fn, get_optim_fn
 
 try:
@@ -66,35 +65,14 @@
         self.lr = lr
         self.device = device
         self.kwargs = kwargs
         self.seed = seed
         self.module_initialized = False
         torch.manual_seed(seed)
 
-    @abc.abstractmethod
-    def learn_one(
-        self, x: dict, y: Optional[Any], **kwargs
-    ) -> "DeepEstimator":
-        """
-        Performs one step of training with a single example.
-
-        Parameters
-        ----------
-        x
-            Input example.
-        y
-            Target value.
-
-        Returns
-        -------
-        DeepEstimator
-            The estimator itself.
-        """
-        raise NotImplementedError
-
     def _filter_kwargs(self, fn: Callable, override=None, **kwargs) -> dict:
         """Filters `net_params` and returns those in `fn`'s arguments.
 
         Parameters
         ----------
         fn
             Arbitrary function
@@ -147,15 +125,19 @@
 
         self.module.to(self.device)
         self.optimizer = self.optimizer_fn(
             self.module.parameters(), lr=self.lr
         )
         self.module_initialized = True
 
-    def clone(self, new_params: dict = {}, include_attributes=False):
+    def clone(
+        self,
+        new_params: dict[Any, Any] | None = None,
+        include_attributes=False,
+    ):
         """Clones the estimator.
 
         Parameters
         ----------
         new_params
             New parameters to be passed to the cloned estimator.
         include_attributes
```

### Comparing `deep_river-0.2.5/deep_river/classification/classifier.py` & `deep_river-0.2.6/deep_river/classification/classifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,19 +112,19 @@
 
 
     >>> dataset = datasets.Phishing()
     >>> metric = metrics.Accuracy()
 
     >>> for x, y in dataset:
     ...     y_pred = model_pipeline.predict_one(x)  # make a prediction
-    ...     metric = metric.update(y, y_pred)  # update the metric
-    ...     model_pipeline = model_pipeline.learn_one(x,y)
+    ...     metric.update(y, y_pred)  # update the metric
+    ...     model_pipeline.learn_one(x,y)
 
     >>> print(f'Accuracy: {metric.get()}')
-    Accuracy: 0.6728
+    Accuracy: 0.6736
     """
 
     def __init__(
         self,
         module: Type[torch.nn.Module],
         loss_fn: Union[str, Callable] = "binary_cross_entropy_with_logits",
         optimizer_fn: Union[str, Callable] = "sgd",
@@ -190,21 +190,21 @@
         }
 
     def _learn(self, x: torch.Tensor, y: Union[ClfTarget, List[ClfTarget]]):
         self.module.train()
         self.optimizer.zero_grad()
         y_pred = self.module(x)
         n_classes = y_pred.shape[-1]
-        y = labels2onehot(
+        y_onehot = labels2onehot(
             y=y,
             classes=self.observed_classes,
             n_classes=n_classes,
             device=self.device,
         )
-        loss = self.loss_fn(y_pred, y)
+        loss = self.loss_fn(y_pred, y_onehot)
         loss.backward()
         self.optimizer.step()
         return self
 
     def learn_one(self, x: dict, y: ClfTarget, **kwargs) -> "Classifier":
         """
         Performs one step of training with a single example.
```

### Comparing `deep_river-0.2.5/deep_river/classification/rolling_classifier.py` & `deep_river-0.2.6/deep_river/classification/rolling_classifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,18 +115,18 @@
     ...     lr=1e-2,
     ...     append_predict=True,
     ...     is_class_incremental=True
     ... )
 
     >>> for x, y in dataset.take(5000):
     ...     y_pred = model_pipeline.predict_one(x)  # make a prediction
-    ...     metric = metric.update(y, y_pred)  # update the metric
-    ...     model = model_pipeline.learn_one(x, y)  # make the model learn
+    ...     metric.update(y, y_pred)  # update the metric
+    ...     model_pipeline.learn_one(x, y)  # make the model learn
     >>> print(f'Accuracy: {metric.get()}')
-    Accuracy: 0.4552
+    Accuracy: 0.4548
     """
 
     def __init__(
         self,
         module: Type[torch.nn.Module],
         loss_fn: Union[str, Callable] = "binary_cross_entropy",
         optimizer_fn: Union[str, Callable] = "sgd",
```

### Comparing `deep_river-0.2.5/deep_river/classification/zoo.py` & `deep_river-0.2.6/deep_river/classification/zoo.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,16 +56,16 @@
     ... )
 
     >>> dataset = datasets.Phishing()
     >>> metric = metrics.Accuracy()
 
     >>> for x, y in dataset:
     ...     y_pred = model_pipeline.predict_one(x) # make a prediction
-    ...     metric = metric.update(y, y_pred) # update the metric
-    ...     model_pipeline = model_pipeline.learn_one(x, y) # update the model
+    ...     metric.update(y, y_pred) # update the metric
+    ...     model_pipeline.learn_one(x, y) # update the model
 
     >>> print(f"Accuracy: {metric.get():.2f}")
     Accuracy: 0.44
 
     """
 
     class LRModule(nn.Module):
@@ -177,16 +177,16 @@
     ... )
 
     >>> dataset = datasets.Phishing()
     >>> metric = metrics.Accuracy()
 
     >>> for x, y in dataset:
     ...     y_pred = model_pipeline.predict_one(x) # make a prediction
-    ...     metric = metric.update(y, y_pred) # update the metric
-    ...     model_pipeline = model_pipeline.learn_one(x, y) # update the model
+    ...     metric.update(y, y_pred) # update the metric
+    ...     model_pipeline.learn_one(x, y) # update the model
 
     >>> print(f"Accuracy: {metric.get():.2f}")
     Accuracy: 0.44
 
     """
 
     class MLPModule(nn.Module):
```

### Comparing `deep_river-0.2.5/deep_river/regression/multioutput.py` & `deep_river-0.2.6/deep_river/regression/multioutput.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 from collections import OrderedDict
 from typing import Callable, Type, Union
 
 import torch
 from river.base import MultiTargetRegressor as RiverMultiTargetRegressor
 from river.base.typing import FeatureName, RegTarget
 
-from deep_river.regression import Regressor
+from deep_river.base import DeepEstimator
 from deep_river.utils import dict2tensor, float2tensor
 
 
 class _TestModule(torch.nn.Module):
     def __init__(self, n_features, n_outputs):
         super().__init__()
         self.dense0 = torch.nn.Linear(n_features, n_outputs)
 
     def forward(self, X, **kwargs):
         return self.dense0(X)
 
 
-class MultiTargetRegressor(RiverMultiTargetRegressor, Regressor):
+class MultiTargetRegressor(RiverMultiTargetRegressor, DeepEstimator):
     """A Regressor that supports multiple targets.
 
     Parameters
     ----------
     module
         Torch Module that builds the autoencoder to be wrapped.
         The Module should accept parameter `n_features` so that the
@@ -78,15 +78,15 @@
     ...         loss_fn='mse',
     ...         lr=0.3,
     ...         optimizer_fn='sgd',
     ...     ))
     >>> metric = metrics.multioutput.MicroAverage(metrics.MAE())
     >>> ev = evaluate.progressive_val_score(dataset, model, metric)
     >>> print(f"MicroAverage(MAE): {metric.get():.2f}")
-    MicroAverage(MAE): 28.36
+    MicroAverage(MAE): 34.31
 
     """
 
     def __init__(
         self,
         module: Type[torch.nn.Module],
         loss_fn: Union[str, Callable] = "mse",
@@ -101,17 +101,17 @@
             loss_fn=loss_fn,
             device=device,
             optimizer_fn=optimizer_fn,
             lr=lr,
             seed=seed,
             **kwargs,
         )
-        self.observed_targets: OrderedDict[
-            FeatureName, RegTarget
-        ] = OrderedDict()
+        self.observed_targets: OrderedDict[FeatureName, RegTarget] = (
+            OrderedDict()
+        )
 
     @classmethod
     def _unit_test_params(cls):
         """
         Returns a dictionary of parameters to be used for unit
         testing the respective class.
 
@@ -146,18 +146,26 @@
             "check_disappearing_features",
             "check_predict_proba_one",
             "check_predict_proba_one_binary",
             "check_learn_one",
             "check_pickling",
         }
 
+    def _learn(self, x: torch.Tensor, y: torch.Tensor):
+        self.module.train()
+        self.optimizer.zero_grad()
+        y_pred = self.module(x)
+        loss = self.loss_fn(y_pred, y)
+        loss.backward()
+        self.optimizer.step()
+
     def learn_one(
         self,
         x: dict,
-        y: typing.Optional[typing.Dict[FeatureName, RegTarget]],
+        y: dict[FeatureName, RegTarget],
         **kwargs,
     ) -> "MultiTargetRegressor":
         if not self.module_initialized:
             self.kwargs["n_features"] = len(x)
             self.initialize_module(**self.kwargs)
         x_t = dict2tensor(x, self.device)
         self.observed_targets.update(y) if y is not None else None
```

### Comparing `deep_river-0.2.5/deep_river/regression/regressor.py` & `deep_river-0.2.6/deep_river/regression/regressor.py`

 * *Files identical despite different names*

### Comparing `deep_river-0.2.5/deep_river/regression/rolling_regressor.py` & `deep_river-0.2.6/deep_river/regression/rolling_regressor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Callable, List, Type, Union
+from typing import Callable, List, Type, Union
 
 import pandas as pd
 import torch
 from river.base.typing import RegTarget
 
 from deep_river.base import RollingDeepEstimator
 from deep_river.regression import Regressor
@@ -122,15 +122,15 @@
             "check_shuffle_features_no_impact",
             "check_emerging_features",
             "check_disappearing_features",
             "check_predict_proba_one",
             "check_predict_proba_one_binary",
         }
 
-    def learn_one(self, x: dict, y: RegTarget, **kwargs) -> "RollingRegressor":
+    def learn_one(self, x: dict, y: RegTarget, **kwargs) -> "Regressor":
         """
         Performs one step of training with the sliding
         window of the most recent examples.
 
         Parameters
         ----------
         x
@@ -152,30 +152,28 @@
         if len(self._x_window) == self.window_size:
             x_t = deque2rolling_tensor(self._x_window, device=self.device)
             y_t = float2tensor(y, device=self.device)
             self._learn(x_t, y_t)
 
         return self
 
-    def learn_many(
-        self, X: pd.DataFrame, y: List[Any]
-    ) -> "RollingDeepEstimator":
+    def learn_many(self, X: pd.DataFrame, y: pd.Series) -> "Regressor":
         if not self.module_initialized:
             self.kwargs["n_features"] = len(X.columns)
             self.initialize_module(**self.kwargs)
 
         self._x_window.extend(X.values.tolist())
         if len(self._x_window) == self.window_size:
             x_t = deque2rolling_tensor(self._x_window, device=self.device)
             y_t = torch.unsqueeze(torch.tensor(y, device=self.device), 1)
             self._learn(x_t, y_t)
 
         return self
 
-    def predict_one(self, x: dict) -> RegTarget:
+    def predict_one(self, x: dict):
         """
         Predicts the target value for the current sliding
         window of most recent examples.
 
         Parameters
         ----------
         x
```

### Comparing `deep_river-0.2.5/deep_river/regression/zoo.py` & `deep_river-0.2.6/deep_river/regression/zoo.py`

 * *Files identical despite different names*

### Comparing `deep_river-0.2.5/deep_river/utils/__init__.py` & `deep_river-0.2.6/deep_river/utils/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utility classes and functions."""
+
 from .estimator_checks import check_estimator
 from .params import get_activation_fn, get_init_fn, get_loss_fn, get_optim_fn
 from .tensor_conversion import (
     deque2rolling_tensor,
     df2tensor,
     dict2tensor,
     float2tensor,
```

### Comparing `deep_river-0.2.5/deep_river/utils/estimator_checks.py` & `deep_river-0.2.6/deep_river/utils/estimator_checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities for unit testing and sanity checking estimators."""
+
 import copy
 
 __all__ = ["check_estimator"]
 
 from river.checks import yield_checks
```

### Comparing `deep_river-0.2.5/deep_river/utils/hooks.py` & `deep_river-0.2.6/deep_river/utils/hooks.py`

 * *Files identical despite different names*

### Comparing `deep_river-0.2.5/deep_river/utils/params.py` & `deep_river-0.2.6/deep_river/utils/params.py`

 * *Files identical despite different names*

### Comparing `deep_river-0.2.5/deep_river/utils/tensor_conversion.py` & `deep_river-0.2.6/deep_river/utils/tensor_conversion.py`

 * *Files identical despite different names*

### Comparing `deep_river-0.2.5/deep_river/utils/test_estimators.py` & `deep_river-0.2.6/deep_river/utils/test_estimators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """General tests that all estimators need to pass."""
+
 import copy
 import importlib
 import inspect
 
 import pytest
 import river
```

### Comparing `deep_river-0.2.5/deep_river/utils/test_tensor_conversion.py` & `deep_river-0.2.6/deep_river/utils/test_tensor_conversion.py`

 * *Files identical despite different names*

### Comparing `deep_river-0.2.5/deep_river.egg-info/SOURCES.txt` & `deep_river-0.2.6/deep_river.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deep_river-0.2.5/pyproject.toml` & `deep_river-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deep_river-0.2.5/setup.py` & `deep_river-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 URL = "https://online-ml.github.io/deep-river/"
 EMAIL = "cedric.kulbach@googlemail.com"
 AUTHOR = "Cedric Kulbach"
 REQUIRES_PYTHON = ">=3.6.0"
 
 # Package requirements.
 base_packages = [
-    "scikit-learn~=1.3.0",
-    "torch~=2.0.1",
-    "pandas~=2.1.0",
-    "numpy~=1.25.2",
-    "river~=0.18.0",
-    "tqdm~=4.61.2",
+    "scikit-learn~=1.4.2",
+    "torch~=2.2.2",
+    "pandas~=2.2.2",
+    "numpy~=1.26.4",
+    "river~=0.21.1",
+    "tqdm~=4.66.4",
     "ordered-set~=4.1.0",
     "torchviz~=0.0.2",
 ]
 
 dev_packages = [
     "graphviz>=0.10.1",
     "matplotlib>=3.0.2",
```

