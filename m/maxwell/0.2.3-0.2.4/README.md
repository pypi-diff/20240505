# Comparing `tmp/maxwell-0.2.3.tar.gz` & `tmp/maxwell-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxwell-0.2.3.tar", last modified: Mon Apr 22 15:36:15 2024, max compression
+gzip compressed data, was "maxwell-0.2.4.tar", last modified: Sun May  5 14:29:45 2024, max compression
```

## Comparing `maxwell-0.2.3.tar` & `maxwell-0.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0 kbg       (1000) kbg       (1000)        0 2024-04-22 15:36:15.044494 maxwell-0.2.3/
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)    10802 2024-04-22 15:36:01.000000 maxwell-0.2.3/LICENSE.txt
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     5284 2024-04-22 15:36:15.039492 maxwell-0.2.3/PKG-INFO
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     4464 2024-04-22 15:36:01.000000 maxwell-0.2.3/README.md
-drwxrwxrwx   0 kbg       (1000) kbg       (1000)        0 2024-04-22 15:36:14.960441 maxwell-0.2.3/maxwell/
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)       47 2024-04-22 15:36:01.000000 maxwell-0.2.3/maxwell/__init__.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     3313 2024-04-22 15:36:01.000000 maxwell-0.2.3/maxwell/actions.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)    19177 2024-04-22 15:36:01.000000 maxwell-0.2.3/maxwell/sed.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     2089 2024-04-22 15:36:01.000000 maxwell-0.2.3/maxwell/train.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)      279 2024-04-22 15:36:01.000000 maxwell-0.2.3/maxwell/util.py
-drwxrwxrwx   0 kbg       (1000) kbg       (1000)        0 2024-04-22 15:36:15.034492 maxwell-0.2.3/maxwell.egg-info/
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     5284 2024-04-22 15:36:14.000000 maxwell-0.2.3/maxwell.egg-info/PKG-INFO
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)      329 2024-04-22 15:36:14.000000 maxwell-0.2.3/maxwell.egg-info/SOURCES.txt
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)        1 2024-04-22 15:36:14.000000 maxwell-0.2.3/maxwell.egg-info/dependency_links.txt
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)       53 2024-04-22 15:36:14.000000 maxwell-0.2.3/maxwell.egg-info/entry_points.txt
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)       27 2024-04-22 15:36:14.000000 maxwell-0.2.3/maxwell.egg-info/requires.txt
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)        8 2024-04-22 15:36:14.000000 maxwell-0.2.3/maxwell.egg-info/top_level.txt
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     1136 2024-04-22 15:36:01.000000 maxwell-0.2.3/pyproject.toml
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)       38 2024-04-22 15:36:15.045491 maxwell-0.2.3/setup.cfg
-drwxrwxrwx   0 kbg       (1000) kbg       (1000)        0 2024-04-22 15:36:15.022493 maxwell-0.2.3/tests/
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     3627 2024-04-22 15:36:01.000000 maxwell-0.2.3/tests/test_sed.py
+drwxr-xr-x   0 kbg        (501) staff       (20)        0 2024-05-05 14:29:45.949653 maxwell-0.2.4/
+-rw-r--r--   0 kbg        (501) staff       (20)    10802 2024-05-05 14:29:35.000000 maxwell-0.2.4/LICENSE.txt
+-rw-r--r--   0 kbg        (501) staff       (20)     5109 2024-05-05 14:29:45.949457 maxwell-0.2.4/PKG-INFO
+-rw-r--r--   0 kbg        (501) staff       (20)     4289 2024-05-05 14:29:35.000000 maxwell-0.2.4/README.md
+drwxr-xr-x   0 kbg        (501) staff       (20)        0 2024-05-05 14:29:45.948225 maxwell-0.2.4/maxwell/
+-rw-r--r--   0 kbg        (501) staff       (20)       47 2024-05-05 14:29:35.000000 maxwell-0.2.4/maxwell/__init__.py
+-rw-r--r--   0 kbg        (501) staff       (20)     3313 2024-05-05 14:29:35.000000 maxwell-0.2.4/maxwell/actions.py
+-rw-r--r--   0 kbg        (501) staff       (20)    21081 2024-05-05 14:29:35.000000 maxwell-0.2.4/maxwell/sed.py
+-rw-r--r--   0 kbg        (501) staff       (20)     2089 2024-05-05 14:29:35.000000 maxwell-0.2.4/maxwell/train.py
+-rw-r--r--   0 kbg        (501) staff       (20)      279 2024-05-05 14:29:35.000000 maxwell-0.2.4/maxwell/util.py
+drwxr-xr-x   0 kbg        (501) staff       (20)        0 2024-05-05 14:29:45.949208 maxwell-0.2.4/maxwell.egg-info/
+-rw-r--r--   0 kbg        (501) staff       (20)     5109 2024-05-05 14:29:45.000000 maxwell-0.2.4/maxwell.egg-info/PKG-INFO
+-rw-r--r--   0 kbg        (501) staff       (20)      329 2024-05-05 14:29:45.000000 maxwell-0.2.4/maxwell.egg-info/SOURCES.txt
+-rw-r--r--   0 kbg        (501) staff       (20)        1 2024-05-05 14:29:45.000000 maxwell-0.2.4/maxwell.egg-info/dependency_links.txt
+-rw-r--r--   0 kbg        (501) staff       (20)       53 2024-05-05 14:29:45.000000 maxwell-0.2.4/maxwell.egg-info/entry_points.txt
+-rw-r--r--   0 kbg        (501) staff       (20)       27 2024-05-05 14:29:45.000000 maxwell-0.2.4/maxwell.egg-info/requires.txt
+-rw-r--r--   0 kbg        (501) staff       (20)        8 2024-05-05 14:29:45.000000 maxwell-0.2.4/maxwell.egg-info/top_level.txt
+-rw-r--r--   0 kbg        (501) staff       (20)     1136 2024-05-05 14:29:35.000000 maxwell-0.2.4/pyproject.toml
+-rw-r--r--   0 kbg        (501) staff       (20)       38 2024-05-05 14:29:45.949692 maxwell-0.2.4/setup.cfg
+drwxr-xr-x   0 kbg        (501) staff       (20)        0 2024-05-05 14:29:45.949056 maxwell-0.2.4/tests/
+-rw-r--r--   0 kbg        (501) staff       (20)     3628 2024-05-05 14:29:35.000000 maxwell-0.2.4/tests/test_sed.py
```

### Comparing `maxwell-0.2.3/LICENSE.txt` & `maxwell-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maxwell-0.2.3/PKG-INFO` & `maxwell-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: maxwell
-Version: 0.2.3
-Summary: Stochastic Edit Distance aligenr for string transduction
+Version: 0.2.4
+Summary: Stochastic Edit Distance aligner for string transduction
 Author: Simon Clematide, Peter Makarov, Travis Bartley
 License: Apache 2.0
 Project-URL: homepage, https://github.com/CUNY-CL/maxwell
 Keywords: computational linguistics,morphology,natural language processing,language
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 4 - Beta
@@ -40,22 +40,17 @@
 
 First install dependencies:
 
     pip install -r requirements.txt
 
 Then install:
 
-    python setup.py install
+    pip install .
 
-Or:
-
-    python setup.py develop
-
-The latter creates a Python module in your environment that updates as you
-update the code. It can then be imported like a regular Python module:
+It can then be imported like a regular Python module:
 
 ```python
 import maxwell
 ```
 
 ## Usage
 
@@ -145,17 +140,15 @@
     symbol into string.
 4.  `delta_eos` A float value representing probability of terminating the
     string.
 
 In Python, these values may be accessed through a `StochasticEditDistance`
 object's `params` attribute.
 
-## Further reading
-
-For further reading, please see:
+## References
 
 Dempster, A., Laird, N., and Rubin, D. 1977. Maximum likelihood from incomplete
 data via the EM algorithm. *Journal of the Royal Statistical Society, Series B*
 30(1): 1-38.
 
 Ristad, E. S. and Yianilos, P. N. 1998. Learning string-edit distance. *IEEE
 Transactions on Pattern Analysis and Machine Intelligence* 20(5): 522-532.
```

### Comparing `maxwell-0.2.3/README.md` & `maxwell-0.2.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -19,22 +19,17 @@
 
 First install dependencies:
 
     pip install -r requirements.txt
 
 Then install:
 
-    python setup.py install
+    pip install .
 
-Or:
-
-    python setup.py develop
-
-The latter creates a Python module in your environment that updates as you
-update the code. It can then be imported like a regular Python module:
+It can then be imported like a regular Python module:
 
 ```python
 import maxwell
 ```
 
 ## Usage
 
@@ -124,17 +119,15 @@
     symbol into string.
 4.  `delta_eos` A float value representing probability of terminating the
     string.
 
 In Python, these values may be accessed through a `StochasticEditDistance`
 object's `params` attribute.
 
-## Further reading
-
-For further reading, please see:
+## References
 
 Dempster, A., Laird, N., and Rubin, D. 1977. Maximum likelihood from incomplete
 data via the EM algorithm. *Journal of the Royal Statistical Society, Series B*
 30(1): 1-38.
 
 Ristad, E. S. and Yianilos, P. N. 1998. Learning string-edit distance. *IEEE
 Transactions on Pattern Analysis and Machine Intelligence* 20(5): 522-532.
```

### Comparing `maxwell-0.2.3/maxwell/actions.py` & `maxwell-0.2.4/maxwell/actions.py`

 * *Files identical despite different names*

### Comparing `maxwell-0.2.3/maxwell/sed.py` & `maxwell-0.2.4/maxwell/sed.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 After:
 
     Ristad, E. S.and Yianilos, P. N. 1998. Learning string-edit distance. IEEE
     Transactions on Pattern Analysis and Machine Intelligence 20(5): 522-532.
 """
 
-
 from __future__ import annotations
 
 import abc
 import dataclasses
 import pickle
 from typing import Any, Dict, Iterable, List, Optional, Sequence, Tuple
 
@@ -95,14 +94,16 @@
         util.log_info(f"Restoring parameters from {filepath}")
         with open(filepath, "rb") as file:
             return pickle.load(file)
 
 
 class StochasticEditDistance(abc.ABC):
     params: ParamDict
+    _train_progress_bar: Optional[tqdm.tqdm]
+    _val_progress_bar: Optional[tqdm.tqdm]
 
     def __init__(self, params):
         """SED model.
 
         Uses character edits (insertions, deletions, substitutions)
         to convert strings. Edit weights are learned with
         expectation-maximization.
@@ -112,14 +113,16 @@
         """
         self.params = params
         # Default value for 0-probability unseen pairs.
         self.default = LARGE_NEG_CONST
         psum = self.params.sum()
         if not numpy.isclose(0.0, psum):
             raise SEDParameterError(f"Parameters do not sum to 1: {psum:.4f}")
+        self._train_progress_bar = None
+        self._val_progress_bar = None
 
     @classmethod
     def build_sed(
         cls,
         source_alphabet: Iterable[Any],
         target_alphabet: Iterable[Any],
         copy_probability: Optional[float] = 0.9,
@@ -295,48 +298,49 @@
 
     def log_likelihood(
         self,
         sources: Iterable[Sequence[Any]],
         targets: Iterable[Sequence[Any]],
     ) -> float:
         """Computes log likelihood."""
-        with tqdm.tqdm(
-            zip(sources, targets), total=len(sources), leave=False
-        ) as pbar:
-            ll = []
-            pbar.set_description("Calculating log-likelihood")
-            for source, target in pbar:
-                ll.append(self.forward_evaluate(source, target)[-1, -1])
-        return float(numpy.mean(ll))
+        loglikes = []
+        self.val_progress_bar.total = len(sources)
+        self.on_validation_start()
+        for source, target in zip(sources, targets):
+            loglikes.append(self.forward_evaluate(source, target)[-1, -1])
+            self.on_validation_step_end()
+        self.on_validation_epoch_end()
+        return numpy.mean(loglikes)
 
     def em(
         self,
         sources: Sequence[Any],
         targets: Sequence[Any],
         epochs: int = 10,
     ) -> None:
         """Update parameters using expectation-maximization.
 
         Args:
             sources (Sequence[Any]): source strings.
             targets (Sequence[Any]): target strings.
             epochs (int): number of EM epochs.
         """
-        loglike = numpy.NINF
         gammas = ParamDict.from_params(self.params)
-        with tqdm.tqdm(zip(sources, targets), total=len(sources)) as pbar:
-            for epoch in range(epochs):
-                pbar.set_description(f"Epoch {epoch}")
-                pbar.set_postfix(loglike=loglike)
-                for source, target in pbar:
-                    self.e_step(source, target, gammas)  # Updates gammas.
-                self.m_step(gammas)  # Updates gammas.
-                self.params.update_params(gammas)  # Updates model parameters.
-                loglike = self.log_likelihood(sources, targets)
-        util.log_info(f"Final log-likelihood: {loglike:.4f}")
+        self.train_progress_bar.total = len(sources)
+        for epoch in range(epochs):
+            self.on_train_epoch_start(epoch)
+            for source, target in zip(sources, targets):
+                self.e_step(source, target, gammas)  # Updates gammas.
+                self.on_train_step_end()
+            self.m_step(gammas)  # Updates gammas.
+            self.params.update_params(gammas)  # Updates model parameters.
+            loglike = self.log_likelihood(sources, targets)
+            self.on_train_epoch_end(loss=-loglike)
+        self.on_train_end()
+        self.on_validation_end()
 
     def e_step(
         self, source: Sequence[Any], target: Sequence[Any], gammas: ParamDict
     ) -> None:
         """Accumulates soft counts.
 
         Args:
@@ -520,7 +524,60 @@
         if isinstance(action, actions.End):
             return -self.params.delta_eos
         if isinstance(action, actions.Copy):
             return -self.params.delta_sub.get(
                 (action.old, action.old), self.default
             )
         raise SEDActionError(f"Unknown action: {action}")
+
+    # The progress bar implementation is based on:
+    #
+    #     https://github.com/Lightning-AI/pytorch-lightning/
+    #     blob/master/src/lightning/pytorch/callbacks/progress/tqdm_progress.py
+
+    BAR_FORMAT = (
+        "{l_bar}{bar}| {n_fmt}/{total_fmt} "
+        "[{elapsed}<{remaining}, {rate_noinv_fmt}{postfix}]"
+    )
+
+    @property
+    def train_progress_bar(self) -> tqdm.tqdm:
+        if self._train_progress_bar is None:
+            self._train_progress_bar = tqdm.tqdm(
+                position=0, leave=True, bar_format=self.BAR_FORMAT
+            )
+        return self._train_progress_bar
+
+    def on_train_epoch_start(self, epoch: int) -> None:
+        self.train_progress_bar.initial = 0
+        self.train_progress_bar.set_description(f"Epoch {epoch}")
+
+    def on_train_step_end(self) -> None:
+        self.train_progress_bar.update()
+
+    def on_train_epoch_end(self, loss: float) -> None:
+        self.train_progress_bar.set_postfix(loss=loss)
+        self.train_progress_bar.reset()
+
+    def on_train_end(self) -> None:
+        self.train_progress_bar.close()
+
+    @property
+    def val_progress_bar(self) -> tqdm.tqdm:
+        if self._val_progress_bar is None:
+            self._val_progress_bar = tqdm.tqdm(
+                position=1, leave=False, bar_format=self.BAR_FORMAT
+            )
+        return self._val_progress_bar
+
+    def on_validation_start(self) -> None:
+        self.val_progress_bar.initial = 0
+        self.val_progress_bar.set_description("Validating")
+
+    def on_validation_step_end(self) -> None:
+        self.val_progress_bar.update()
+
+    def on_validation_epoch_end(self) -> None:
+        self.val_progress_bar.reset()
+
+    def on_validation_end(self) -> None:
+        self.val_progress_bar.close()
```

### Comparing `maxwell-0.2.3/maxwell/train.py` & `maxwell-0.2.4/maxwell/train.py`

 * *Files identical despite different names*

### Comparing `maxwell-0.2.3/maxwell.egg-info/PKG-INFO` & `maxwell-0.2.4/maxwell.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: maxwell
-Version: 0.2.3
-Summary: Stochastic Edit Distance aligenr for string transduction
+Version: 0.2.4
+Summary: Stochastic Edit Distance aligner for string transduction
 Author: Simon Clematide, Peter Makarov, Travis Bartley
 License: Apache 2.0
 Project-URL: homepage, https://github.com/CUNY-CL/maxwell
 Keywords: computational linguistics,morphology,natural language processing,language
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 4 - Beta
@@ -40,22 +40,17 @@
 
 First install dependencies:
 
     pip install -r requirements.txt
 
 Then install:
 
-    python setup.py install
+    pip install .
 
-Or:
-
-    python setup.py develop
-
-The latter creates a Python module in your environment that updates as you
-update the code. It can then be imported like a regular Python module:
+It can then be imported like a regular Python module:
 
 ```python
 import maxwell
 ```
 
 ## Usage
 
@@ -145,17 +140,15 @@
     symbol into string.
 4.  `delta_eos` A float value representing probability of terminating the
     string.
 
 In Python, these values may be accessed through a `StochasticEditDistance`
 object's `params` attribute.
 
-## Further reading
-
-For further reading, please see:
+## References
 
 Dempster, A., Laird, N., and Rubin, D. 1977. Maximum likelihood from incomplete
 data via the EM algorithm. *Journal of the Royal Statistical Society, Series B*
 30(1): 1-38.
 
 Ristad, E. S. and Yianilos, P. N. 1998. Learning string-edit distance. *IEEE
 Transactions on Pattern Analysis and Machine Intelligence* 20(5): 522-532.
```

### Comparing `maxwell-0.2.3/pyproject.toml` & `maxwell-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 include-package-data = false
 
 [tool.setuptools.packages.find]
 include = ["maxwell*"]
 
 [project]
 name = "maxwell"
-version = "0.2.3"
-description = "Stochastic Edit Distance aligenr for string transduction"
+version = "0.2.4"
+description = "Stochastic Edit Distance aligner for string transduction"
 readme = "README.md"
 requires-python = "> 3.9"
 license = { text = "Apache 2.0" }
 authors = [
     {name = "Simon Clematide"},
     {name = "Peter Makarov"},
     {name = "Travis Bartley"},
```

### Comparing `maxwell-0.2.3/tests/test_sed.py` & `maxwell-0.2.4/tests/test_sed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Unit tests for sed.py."""
+
 import unittest
 
 import numpy
 
 from maxwell import actions, sed, util
 
 SOURCE_ALPHA = list("abcdefg")
```

