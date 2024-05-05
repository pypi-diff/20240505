# Comparing `tmp/ikpls-1.2.1.post2.tar.gz` & `tmp/ikpls-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ikpls-1.2.1.post2.tar", max compression
+gzip compressed data, was "ikpls-1.2.2.tar", max compression
```

## Comparing `ikpls-1.2.1.post2.tar` & `ikpls-1.2.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11433 2024-04-25 17:40:40.990097 ikpls-1.2.1.post2/LICENSE
--rw-r--r--   0        0        0     7650 2024-04-25 17:40:40.990097 ikpls-1.2.1.post2/README.md
--rw-r--r--   0        0        0       28 2024-04-25 17:40:40.990097 ikpls-1.2.1.post2/ikpls/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 17:40:40.990097 ikpls-1.2.1.post2/ikpls/fast_cross_validation/__init__.py
--rw-r--r--   0        0        0    23768 2024-04-25 17:40:40.990097 ikpls-1.2.1.post2/ikpls/fast_cross_validation/numpy_ikpls.py
--rw-r--r--   0        0        0    15583 2024-04-25 17:40:40.990097 ikpls-1.2.1.post2/ikpls/jax_ikpls_alg_1.py
--rw-r--r--   0        0        0    13495 2024-04-25 17:40:40.990097 ikpls-1.2.1.post2/ikpls/jax_ikpls_alg_2.py
--rw-r--r--   0        0        0    41664 2024-04-25 17:40:40.990097 ikpls-1.2.1.post2/ikpls/jax_ikpls_base.py
--rw-r--r--   0        0        0    10170 2024-04-25 17:40:40.990097 ikpls-1.2.1.post2/ikpls/numpy_ikpls.py
--rw-r--r--   0        0        0      558 2024-04-25 17:40:40.994097 ikpls-1.2.1.post2/pyproject.toml
--rw-r--r--   0        0        0     8578 1970-01-01 00:00:00.000000 ikpls-1.2.1.post2/PKG-INFO
+-rw-r--r--   0        0        0    11433 2024-05-05 17:41:39.329955 ikpls-1.2.2/LICENSE
+-rw-r--r--   0        0        0     7711 2024-05-05 17:41:39.329955 ikpls-1.2.2/README.md
+-rw-r--r--   0        0        0       22 2024-05-05 17:41:39.333955 ikpls-1.2.2/ikpls/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 17:41:39.333955 ikpls-1.2.2/ikpls/fast_cross_validation/__init__.py
+-rw-r--r--   0        0        0    25831 2024-05-05 17:41:39.333955 ikpls-1.2.2/ikpls/fast_cross_validation/numpy_ikpls.py
+-rw-r--r--   0        0        0    16854 2024-05-05 17:41:39.333955 ikpls-1.2.2/ikpls/jax_ikpls_alg_1.py
+-rw-r--r--   0        0        0    15324 2024-05-05 17:41:39.333955 ikpls-1.2.2/ikpls/jax_ikpls_alg_2.py
+-rw-r--r--   0        0        0    43872 2024-05-05 17:41:39.333955 ikpls-1.2.2/ikpls/jax_ikpls_base.py
+-rw-r--r--   0        0        0    10992 2024-05-05 17:41:39.333955 ikpls-1.2.2/ikpls/numpy_ikpls.py
+-rw-r--r--   0        0        0      552 2024-05-05 17:41:39.337955 ikpls-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     8633 1970-01-01 00:00:00.000000 ikpls-1.2.2/PKG-INFO
```

### Comparing `ikpls-1.2.1.post2/LICENSE` & `ikpls-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ikpls-1.2.1.post2/README.md` & `ikpls-1.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -39,20 +39,20 @@
 benefit both IKPLS Algorithms and especially Algorithm #2. The fast
 cross-validation algorithms are mathematically equivalent to the
 classical cross-validation algorithm. Still, they are much quicker if
 cross-validation splits exceed 3. The fast cross-validation algorithms
 correctly handle (column-wise) centering and scaling of the X and Y
 input matrices using training set means and standard deviations to avoid
 data leakage from the validation set. This centering and scaling can be
-enabled by setting the center parameter to True and the scale parameter
-to True, respectively. The fast cross-validation algorithms correctly
-handle row-wise preprocessing such as (row-wise) centering and scaling
-of the X and Y input matrices, convolution, or other preprocessing.
-Row-wise preprocessing can safely be applied before passing the data to
-the fast cross-validation algorithms.
+enabled or disabled independently from eachother and for X and Y by setting 
+the parameters `center_X`, `center_Y`, `scale_X`, and `scale_Y`, respectively.
+The fast cross-validation algorithms correctly handle row-wise preprocessing
+such as (row-wise) centering and scaling of the X and Y input matrices,
+convolution, or other preprocessing. Row-wise preprocessing can safely be
+applied before passing the data to the fast cross-validation algorithms.
 
 ## Pre-requisites
 
 The JAX implementations support running on both CPU, GPU, and TPU. To
 use the GPU or TPU, follow the instructions from the [JAX Installation
 Guide](https://jax.readthedocs.io/en/latest/installation.html).
```

### Comparing `ikpls-1.2.1.post2/ikpls/fast_cross_validation/numpy_ikpls.py` & `ikpls-1.2.2/ikpls/fast_cross_validation/numpy_ikpls.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,53 +26,74 @@
     Implements fast cross-validation with partial least-squares regression using
     Improved Kernel PLS by Dayal and MacGregor:
     https://arxiv.org/abs/2401.13185
     https://doi.org/10.1002/(SICI)1099-128X(199701)11:1%3C73::AID-CEM435%3E3.0.CO;2-%23
 
     Parameters
     ----------
-    center : bool, optional default=False
-            Whether to center `X` and `Y` before fitting by subtracting a mean row from
-            each. The centering is computed on the training set for each fold to avoid
-            data leakage. The centering is undone before returning predictions. Setting
-            this to True while using multiple jobs will increase the memory consumption
-            as each job will then have to keep its own copy of the data with its
-            specific centering.
-
-    scale : bool, optional default=False, only used if `center` is True
-        Whether to scale `X` and `Y` before fitting by dividing each row by its
-        standard deviation. The scaling is computed on the training set for each fold
-        to avoid data leakage. The scaling is undone before returning predictions.
-        Setting this to True while using multiple jobs will increase the memory
-        consumption as each job will then have to keep its own copy of the data with
-        its specific scaling.
+    center_X : bool, optional default=True
+        Whether to center `X` before fitting by subtracting its row of
+        column-wise means from each row. The row of column-wise means is computed on
+        the training set for each fold to avoid data leakage.
+    
+    center_Y : bool, optional default=True
+        Whether to center `Y` before fitting by subtracting its row of
+        column-wise means from each row. The row of column-wise means is computed on
+        the training set for each fold to avoid data leakage.
+    
+    scale_X : bool, optional default=True
+        Whether to scale `X` before fitting by dividing each row with the row of `X`'s
+        column-wise standard deviations. Bessel's correction for the unbiased estimate
+        of the sample standard deviation is used. The row of column-wise standard
+        deviations is computed on the training set for each fold to avoid data leakage.
+    
+    scale_Y : bool, optional default=True
+        Whether to scale `Y` before fitting by dividing each row with the row of `X`'s
+        column-wise standard deviations. Bessel's correction for the unbiased estimate
+        of the sample standard deviation is used. The row of column-wise standard
+        deviations is computed on the training set for each fold to avoid data leakage.
 
     algorithm : int, default=1
         Whether to use Improved Kernel PLS Algorithm #1 or #2.
 
     dtype : numpy.float, default=numpy.float64
         The float datatype to use in computation of the PLS algorithm. Using a lower
         precision than float64 will yield significantly worse results when using an
         increasing number of components due to propagation of numerical errors.
 
     Raises
     ------
     ValueError
         If `algorithm` is not 1 or 2.
+    
+    Notes
+    -----
+    Any centering and scaling is undone before returning predictions to ensure that
+    predictions are on the original scale. If both centering and scaling are True, then
+    the data is first centered and then scaled.
+
+    Setting either of `center_X`, `center_Y`, `scale_X`, or `scale_Y` to True, while
+    using multiple jobs, will increase the memory consumption as each job will then
+    have to keep its own copy of :math:`\mathbf{X}^{\mathbf{T}}\mathbf{X}` and
+    :math:`\mathbf{X}^{\mathbf{T}}\mathbf{Y}` with its specific centering and scaling.
     """
 
     def __init__(
         self,
-        center: bool = True,
-        scale: bool = True,
+        center_X: bool = True,
+        center_Y: bool = True,
+        scale_X: bool = True,
+        scale_Y: bool = True,
         algorithm: int = 1,
         dtype: np.float_ = np.float64,
     ) -> None:
-        self.center = center
-        self.scale = scale
+        self.center_X = center_X
+        self.center_Y = center_Y
+        self.scale_X = scale_X
+        self.scale_Y = scale_Y
         self.algorithm = algorithm
         self.dtype = dtype
         self.name = f"Improved Kernel PLS Algorithm #{algorithm}"
         if self.algorithm not in [1, 2]:
             raise ValueError(
                 f"Invalid algorithm: {self.algorithm}. Algorithm must be 1 or 2."
             )
@@ -205,98 +226,121 @@
         R = RT.T
 
         validation_size = validation_indices.size
         if self.algorithm == 1:
             TT = np.zeros(shape=(self.A, self.N - validation_size), dtype=self.dtype)
             T = TT.T
 
-        # Extract training XTY
+        # Extract training X and Y
         validation_X = self.X[validation_indices]
         validation_Y = self.Y[validation_indices]
-        if self.center:
+
+        if self.center_X or self.center_Y or self.scale_X or self.scale_Y:
             training_size = self.N - validation_size
             N_total_over_N_train = self.N / training_size
             N_val_over_N_train = validation_size / training_size
+
+        # Compute the training set means
+        if self.center_X or self.center_Y or self.scale_X:
             training_X_mean = (
                 N_total_over_N_train * self.X_mean
                 - N_val_over_N_train * np.mean(validation_X, axis=0, keepdims=True)
             )
+        if self.center_X or self.center_Y or self.scale_Y:
             training_Y_mean = (
                 N_total_over_N_train * self.Y_mean
                 - N_val_over_N_train * np.mean(validation_Y, axis=0, keepdims=True)
             )
-            if self.scale:
-                train_sum_X = self.sum_X - np.expand_dims(
-                    np.einsum("ij -> j", validation_X), axis=0
-                )
-                train_sum_sq_X = self.sum_sq_X - np.expand_dims(
-                    np.einsum("ij,ij -> j", validation_X, validation_X), axis=0
-                )
-                training_X_std = np.sqrt(
-                    1
-                    / (training_size - 1)
-                    * (
-                        -2 * training_X_mean * train_sum_X
-                        + training_size
-                        * np.einsum("ij,ij -> ij", training_X_mean, training_X_mean)
-                        + train_sum_sq_X
-                    )
-                )
-                training_X_std[training_X_std == 0] = 1
-                train_sum_Y = self.sum_Y - np.expand_dims(
-                    np.einsum("ij -> j", validation_Y), axis=0
-                )
-                train_sum_sq_Y = self.sum_sq_Y - np.expand_dims(
-                    np.einsum("ij,ij -> j", validation_Y, validation_Y), axis=0
+
+        # Compute the training set standard deviations for X
+        if self.scale_X:
+            train_sum_X = self.sum_X - np.expand_dims(
+                np.einsum("ij -> j", validation_X), axis=0
+            )
+            train_sum_sq_X = self.sum_sq_X - np.expand_dims(
+                np.einsum("ij,ij -> j", validation_X, validation_X), axis=0
+            )
+            training_X_std = np.sqrt(
+                1
+                / (training_size - 1)
+                * (
+                    -2 * training_X_mean * train_sum_X
+                    + training_size
+                    * np.einsum("ij,ij -> ij", training_X_mean, training_X_mean)
+                    + train_sum_sq_X
                 )
-                training_Y_std = np.sqrt(
-                    1
-                    / (training_size - 1)
-                    * (
-                        -2 * training_Y_mean * train_sum_Y
-                        + training_size
-                        * np.einsum("ij,ij -> ij", training_Y_mean, training_Y_mean)
-                        + train_sum_sq_Y
-                    )
+            )
+            training_X_std[training_X_std == 0] = 1
+
+        # Compute the training set standard deviations for Y
+        if self.scale_Y:
+            train_sum_Y = self.sum_Y - np.expand_dims(
+                np.einsum("ij -> j", validation_Y), axis=0
+            )
+            train_sum_sq_Y = self.sum_sq_Y - np.expand_dims(
+                np.einsum("ij,ij -> j", validation_Y, validation_Y), axis=0
+            )
+            training_Y_std = np.sqrt(
+                1
+                / (training_size - 1)
+                * (
+                    -2 * training_Y_mean * train_sum_Y
+                    + training_size
+                    * np.einsum("ij,ij -> ij", training_Y_mean, training_Y_mean)
+                    + train_sum_sq_Y
                 )
-                training_Y_std[training_Y_std == 0] = 1
-        # Subtract the validation set's contribution
+            )
+            training_Y_std[training_Y_std == 0] = 1
+
+        # Subtract the validation set's contribution from the total XTY
         training_XTY = self.XTY - validation_X.T @ validation_Y
-        if self.center:
+
+        # Apply the training set centering
+        if self.center_X or self.center_Y:
             # Apply the training set centering
             training_XTY = training_XTY - training_size * (
                 training_X_mean.T @ training_Y_mean
             )
-            if self.scale:
-                # Apply the training set scaling
-                training_XTY = training_XTY / (training_X_std.T @ training_Y_std)
+
+        # Apply the training set scaling
+        if self.scale_X and self.scale_Y:
+            divisor = training_X_std.T @ training_Y_std
+        elif self.scale_X:
+            divisor = training_X_std.T
+        elif self.scale_Y:
+            divisor = training_Y_std
+        if self.scale_X or self.scale_Y:
+            training_XTY = training_XTY / divisor
+
+        # If algorithm is 1, extract training set X
         if self.algorithm == 1:
             training_indices = np.setdiff1d(self.all_indices,
                                             validation_indices,
                                             assume_unique=True)
             training_X = self.X[training_indices]
-            if self.center:
+            if self.center_X:
                 # Apply the training set centering
                 training_X = training_X - training_X_mean
-                if self.scale:
-                    # Apply the training set scaling
-                    training_X = training_X / training_X_std
+            if self.scale_X:
+                # Apply the training set scaling
+                training_X = training_X / training_X_std
+
+        # If algorithm is 2, derive training set XTX from total XTX and validation XTX
         else:
-            # Used for algorithm #2
-            # Subtract the validation set's contribution
             training_XTX = self.XTX - validation_X.T @ validation_X
-            if self.center:
+            if self.center_X:
                 # Apply the training set centering
                 training_XTX = training_XTX - training_size * (
                     training_X_mean.T @ training_X_mean
                 )
-                if self.scale:
-                    # Apply the training set scaling
-                    training_XTX = training_XTX / (training_X_std.T @ training_X_std)
+            if self.scale_X:
+                # Apply the training set scaling
+                training_XTX = training_XTX / (training_X_std.T @ training_X_std)
 
+        # Execute Improved Kernel PLS steps 2-5
         for i in range(self.A):
             # Step 2
             if self.M == 1:
                 norm = la.norm(training_XTY, ord=2)
                 if np.isclose(norm, 0, atol=np.finfo(np.float64).eps, rtol=0):
                     self._weight_warning(i)
                     break
@@ -343,20 +387,27 @@
             QT[i] = q.squeeze()
 
             # Step 5
             training_XTY = training_XTY - (p @ q.T) * tTt
 
             # Compute regression coefficients
             B[i] = B[i - 1] + r @ q.T
-        if not self.center:
+
+        # Use additive and multiplicative identities for means and standard deviations
+        # for centering and scaling if they are not used
+        if not self.center_X:
             training_X_mean = np.zeros((1, self.K))
+        if not self.center_Y:
             training_Y_mean = np.zeros((1, self.M))
-        if not self.scale:
+        if not self.scale_X:
             training_X_std = np.ones((1, self.K))
+        if not self.scale_Y:
             training_Y_std = np.ones((1, self.M))
+
+        # Return PLS matrices and training set statistics
         if self.algorithm == 1:
             return (
                 B,
                 W,
                 P,
                 Q,
                 R,
@@ -399,52 +450,56 @@
             Integer array defining indices into X and Y corresponding to samples on
             which to predict.
 
         B : Array of shape (A, K, M)
             PLS regression coefficients tensor.
 
         training_X_mean : Array of shape (1, K)
-            Mean row of training X. If self.center is False, then this should be an
+            Mean row of training X. If self.center_X is False, then this should be an
             array of zeros.
 
         training_Y_mean : Array of shape (1, M)
-            Mean row of training Y. If self.center is False, then this should be an
+            Mean row of training Y. If self.center_Y is False, then this should be an
             array of zeros.
 
         training_X_std : Array of shape (1, K)
-            Sample standard deviation row of training X. If self.scale is False, then
+            Sample standard deviation row of training X. If self.scale_X is False, then
             this should be an array of ones. Any zero standard deviations should be
             replaced with ones.
 
         training_Y_std : Array of shape (1, M)
-            Sample standard deviation row of training Y. If self.scale is False, then
+            Sample standard deviation row of training Y. If self.scale_Y is False, then
             this should be an array of ones. Any zero standard deviations should be
             replaced with ones.
 
         n_components : int or None, optional
             Number of components in the PLS model. If None, then all number of
             components are used.
 
         Returns
         -------
         Y_pred : Array of shape (N_pred, M) or (A, N_pred, M)
             If `n_components` is an int, then an array of shape (N_pred, M) with the
             predictions for that specific number of components is used. If
             `n_components` is None, returns a prediction for each number of components
             up to `A`.
+        
+        Notes
+        -----
         """
 
         predictor_variables = self.X[indices]
-        # Apply the potential training set centering
+        # Apply the potential training set centering and scaling
         predictor_variables = (predictor_variables - training_X_mean) / training_X_std
         if n_components is None:
             Y_pred = predictor_variables @ B
         else:
             Y_pred = predictor_variables @ B[n_components - 1]
-        # Add the potential training set bias
+        # Multiply by the potential training set scale and add the potential training
+        # set bias
         return Y_pred * training_Y_std + training_Y_mean
 
     def _stateless_fit_predict_eval(
         self,
         validation_indices: npt.NDArray[np.int_],
         metric_function: Callable[
             [npt.NDArray[np.float_], npt.NDArray[np.float_]], Any
@@ -505,15 +560,15 @@
             A dictionary mapping each unique value in `cv_splits` to an array of
             validation indices.
         """
         index_dict = {}
         for i, num in enumerate(cv_splits):
             try:
                 index_dict[num].append(i)
-            except:
+            except KeyError:
                 index_dict[num] = [i]
         for key in index_dict:
             index_dict[key] = np.asarray(index_dict[key], dtype=int)
         return index_dict
 
     def cross_validate(
         self,
@@ -560,16 +615,16 @@
         Returns
         -------
         metrics : dict of Hashable to Any
             A dictionary mapping each unique value in `cv_splits` to the result of
             evaluating `metric_function` on the validation set corresponding to that
             value.
 
-        Notes:
-        ------
+        Notes
+        -----
         The order of cross-validation folds is determined by the order of the unique
         values in `cv_splits`. The keys and values of `metrics` will be sorted in the
         same order.
         """
 
         self.X = np.asarray(X, dtype=self.dtype)
         self.Y = np.asarray(Y, dtype=self.dtype)
@@ -589,28 +644,30 @@
 
         print(
             f"Cross-validating Improved Kernel PLS Algorithm {self.algorithm} with {A}"
             f" components on {num_splits} unique splits using {n_jobs} "
             f"parallel processes."
         )
 
-        if self.center:
-            # We can compute these once for the entire dataset and subtract the
-            # validation parts during cross-validation.
+        # We can compute these once for the entire dataset and subtract the
+        # validation parts during cross-validation.
+        if self.center_X or self.center_Y or self.scale_X:
             self.X_mean = np.mean(self.X, axis=0, keepdims=True)
+        if self.center_X or self.center_Y or self.scale_Y:
             self.Y_mean = np.mean(self.Y, axis=0, keepdims=True)
-            if self.scale:
-                self.sum_X = np.expand_dims(np.einsum("ij->j", self.X), axis=0)
-                self.sum_Y = np.expand_dims(np.einsum("ij->j", self.Y), axis=0)
-                self.sum_sq_X = np.expand_dims(
-                    np.einsum("ij,ij->j", self.X, self.X), axis=0
-                )
-                self.sum_sq_Y = np.expand_dims(
-                    np.einsum("ij,ij->j", self.Y, self.Y), axis=0
-                )
+        if self.scale_X:
+            self.sum_X = np.expand_dims(np.einsum("ij->j", self.X), axis=0)
+            self.sum_sq_X = np.expand_dims(
+                np.einsum("ij,ij->j", self.X, self.X), axis=0
+            )
+        if self.scale_Y:
+            self.sum_Y = np.expand_dims(np.einsum("ij->j", self.Y), axis=0)
+            self.sum_sq_Y = np.expand_dims(
+                np.einsum("ij,ij->j", self.Y, self.Y), axis=0
+            )
 
         if verbose > 0:
             print("Computing total XTY...")
         self.XTY = self.X.T @ self.Y
         if verbose > 0:
             print("Done!")
         if self.algorithm == 2:
@@ -630,9 +687,9 @@
 
         metrics_list = Parallel(n_jobs=n_jobs, verbose=verbose)(
             delayed(worker)(validation_indices, metric_function)
             for validation_indices in validation_indices_dict.values()
         )
 
         metrics_dict = dict(zip(validation_indices_dict.keys(), metrics_list))
- 
+
         return metrics_dict
```

### Comparing `ikpls-1.2.1.post2/ikpls/jax_ikpls_alg_1.py` & `ikpls-1.2.2/ikpls/jax_ikpls_alg_1.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,23 +24,31 @@
     """
     Implements partial least-squares regression using Improved Kernel PLS Algorithm #1
     by Dayal and MacGregor:
     https://doi.org/10.1002/(SICI)1099-128X(199701)11:1%3C73::AID-CEM435%3E3.0.CO;2-%23
 
     Parameters
     ----------
-    center : bool, optional, default=True
-        Whether to center the data before fitting. If True, then the mean of the
-        training data is subtracted from the data. If False, then the data is assumed
-        to be already centered.
-
-    scale : bool, optional, default=True
-        Whether to scale the data before fitting. If True, then the data is scaled
-        using Bessel's correction for the unbiased estimate of the sample standard
-        deviation. If False, then the data is assumed to be already scaled.
+    center_X : bool, default=True
+        Whether to center `X` before fitting by subtracting its row of
+        column-wise means from each row.
+    
+    center_Y : bool, default=True
+        Whether to center `Y` before fitting by subtracting its row of
+        column-wise means from each row.
+    
+    scale_X : bool, default=True
+        Whether to scale `X` before fitting by dividing each row with the row of `X`'s
+        column-wise standard deviations. Bessel's correction for the unbiased estimate
+        of the sample standard deviation is used.
+
+    scale_Y : bool, default=True
+        Whether to scale `Y` before fitting by dividing each row with the row of `X`'s
+        column-wise standard deviations. Bessel's correction for the unbiased estimate
+        of the sample standard deviation is used.
 
     copy : bool, optional, default=True
         Whether to copy `X` and `Y` in fit before potentially applying centering and
         scaling. If True, then the data is copied before fitting. If False, and `dtype`
         matches the type of `X` and `Y`, then centering and scaling is done inplace,
         modifying both arrays.
 
@@ -54,29 +62,39 @@
         differentiable version is slightly slower. Results among the two versions are
         identical.
 
     verbose : bool, optional, default=False
         If True, each sub-function will print when it will be JIT compiled. This can be
         useful to track if recompilation is triggered due to passing inputs with
         different shapes.
+
+    Notes
+    -----
+    Any centering and scaling is undone before returning predictions with `fit` to
+    ensure that predictions are on the original scale. If both centering and scaling
+    are True, then the data is first centered and then scaled.
     """
 
     def __init__(
         self,
-        center: bool = True,
-        scale: bool = True,
+        center_X: bool = True,
+        center_Y: bool = True,
+        scale_X: bool = True,
+        scale_Y: bool = True,
         copy: bool = True,
         dtype: DTypeLike = jnp.float64,
         reverse_differentiable: bool = False,
         verbose: bool = False,
     ) -> None:
         self.name = "Improved Kernel PLS Algorithm #1"
         super().__init__(
-            center=center,
-            scale=scale,
+            center_X=center_X,
+            center_Y=center_Y,
+            scale_X=scale_X,
+            scale_Y=scale_Y,
             copy=copy,
             dtype=dtype,
             reverse_differentiable=reverse_differentiable,
             verbose=verbose,
         )
         self.name += " #1"
         self.T = None
@@ -342,30 +360,41 @@
 
         See Also
         --------
         stateless_fit : Performs the same operation but returns the output matrices
         instead of storing them in the class instance.
         """
         self.B, W, P, Q, R, T, self.X_mean, self.Y_mean, self.X_std, self.Y_std = (
-            self.stateless_fit(X, Y, A, self.center, self.scale, self.copy)
+            self.stateless_fit(
+                X,
+                Y,
+                A,
+                self.center_X,
+                self.center_Y,
+                self.scale_X,
+                self.scale_Y,
+                self.copy,
+            )
         )
         self.W = W.T
         self.P = P.T
         self.Q = Q.T
         self.R = R.T
         self.T = T.T
 
-    @partial(jax.jit, static_argnums=(0, 3, 4, 5, 6))
+    @partial(jax.jit, static_argnums=(0, 3, 4, 5, 6, 7, 8))
     def stateless_fit(
         self,
         X: ArrayLike,
         Y: ArrayLike,
         A: int,
-        center: bool = True,
-        scale: bool = True,
+        center_X: bool = True,
+        center_Y: bool = True,
+        scale_X: bool = True,
+        scale_Y: bool = True,
         copy: bool = True,
     ) -> Tuple[jax.Array, jax.Array, jax.Array, jax.Array, jax.Array, jax.Array]:
         """
         Fits Improved Kernel PLS Algorithm #1 on `X` and `Y` using `A` components.
         Returns the internal matrices instead of storing them in the class instance.
 
         Parameters
@@ -377,23 +406,31 @@
         Y : Array of shape (N, M) or (N,)
             Response variables. Its dtype will be converted to float64 for reliable
             results.
 
         A : int
             Number of components in the PLS model.
 
-        center : bool, optional, default=True
-            Whether to center the data before fitting. If True, then the mean of the
-            training data is subtracted from the data. If False, then the data is
-            assumed to be already centered.
-
-        scale : bool, optional, default=True
-            Whether to scale the data before fitting. If True, then the data is scaled
-            using Bessel's correction for the unbiased estimate of the sample standard
-            deviation. If False, then the data is assumed to be already scaled.
+        center_X : bool, default=True
+            Whether to center `X` before fitting by subtracting its row of
+            column-wise means from each row.
+        
+        center_Y : bool, default=True
+            Whether to center `Y` before fitting by subtracting its row of
+            column-wise means from each row.
+        
+        scale_X : bool, default=True
+            Whether to scale `X` before fitting by dividing each row with the row of
+            `X`'s column-wise standard deviations. Bessel's correction for the unbiased
+            estimate of the sample standard deviation is used.
+
+        scale_Y : bool, default=True
+            Whether to scale `Y` before fitting by dividing each row with the row of
+            `X`'s column-wise standard deviations. Bessel's correction for the unbiased
+            estimate of the sample standard deviation is used.
 
         copy : bool, optional, default=True
             Whether to copy `X` and `Y` in fit before potentially applying centering
             and scaling. If True, then the data is copied before fitting. If False, and
             `dtype` matches the type of `X` and `Y`, then centering and scaling is done
             inplace, modifying both arrays.
 
@@ -447,15 +484,15 @@
         """
 
         if self.verbose:
             print(f"stateless_fit for {self.name} will be JIT compiled...")
 
         X, Y = self._initialize_input_matrices(X, Y)
         X, Y, X_mean, Y_mean, X_std, Y_std = self._center_scale_input_matrices(
-            X, Y, center, scale, copy
+            X, Y, center_X, center_Y, scale_X, scale_Y, copy
         )
 
         # Get shapes
         N, K = X.shape
         M = Y.shape[1]
 
         # Initialize matrices
```

### Comparing `ikpls-1.2.1.post2/ikpls/jax_ikpls_alg_2.py` & `ikpls-1.2.2/ikpls/jax_ikpls_alg_2.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,23 +24,31 @@
     """
     Implements partial least-squares regression using Improved Kernel PLS Algorithm #2
     by Dayal and MacGregor:
     https://doi.org/10.1002/(SICI)1099-128X(199701)11:1%3C73::AID-CEM435%3E3.0.CO;2-%23.
 
     Parameters
     ----------
-    center : bool, optional, default=True
-        Whether to center the data before fitting. If True, then the mean of the
-        training data is subtracted from the data. If False, then the data is assumed
-        to be already centered.
-
-    scale : bool, optional, default=True
-        Whether to scale the data before fitting. If True, then the data is scaled
-        using Bessel's correction for the unbiased estimate of the sample standard
-        deviation. If False, then the data is assumed to be already scaled.
+    center_X : bool, default=True
+        Whether to center `X` before fitting by subtracting its row of
+        column-wise means from each row.
+    
+    center_Y : bool, default=True
+        Whether to center `Y` before fitting by subtracting its row of
+        column-wise means from each row.
+    
+    scale_X : bool, default=True
+        Whether to scale `X` before fitting by dividing each row with the row of `X`'s
+        column-wise standard deviations. Bessel's correction for the unbiased estimate
+        of the sample standard deviation is used.
+
+    scale_Y : bool, default=True
+        Whether to scale `Y` before fitting by dividing each row with the row of `X`'s
+        column-wise standard deviations. Bessel's correction for the unbiased estimate
+        of the sample standard deviation is used.
 
     copy : bool, optional, default=True
         Whether to copy `X` and `Y` in fit before potentially applying centering and
         scaling. If True, then the data is copied before fitting. If False, and `dtype`
         matches the type of `X` and `Y`, then centering and scaling is done inplace,
         modifying both arrays.
 
@@ -54,28 +62,38 @@
         differentiable version is slightly slower. Results among the two versions are
         identical.
 
     verbose : bool, optional, default=False
         If True, each sub-function will print when it will be JIT compiled. This can be
         useful to track if recompilation is triggered due to passing inputs with
         different shapes.
+
+    Notes
+    -----
+    Any centering and scaling is undone before returning predictions with `fit` to
+    ensure that predictions are on the original scale. If both centering and scaling
+    are True, then the data is first centered and then scaled.
     """
 
     def __init__(
         self,
-        center: bool = True,
-        scale: bool = True,
+        center_X: bool = True,
+        center_Y: bool = True,
+        scale_X: bool = True,
+        scale_Y: bool = True,
         copy: bool = True,
         dtype: DTypeLike = jnp.float64,
         reverse_differentiable: bool = False,
         verbose: bool = False,
     ) -> None:
         super().__init__(
-            center=center,
-            scale=scale,
+            center_X=center_X,
+            center_Y=center_Y,
+            scale_X=scale_X,
+            scale_Y=scale_Y,
             copy=copy,
             dtype=dtype,
             reverse_differentiable=reverse_differentiable,
             verbose=verbose,
         )
         self.name += " #2"
 
@@ -319,29 +337,40 @@
 
         See Also
         --------
         stateless_fit : Performs the same operation but returns the output matrices
         instead of storing them in the class instance.
         """
         self.B, W, P, Q, R, self.X_mean, self.Y_mean, self.X_std, self.Y_std = (
-            self.stateless_fit(X, Y, A, self.center, self.scale, self.copy)
+            self.stateless_fit(
+                X,
+                Y,
+                A,
+                self.center_X,
+                self.center_Y,
+                self.scale_X,
+                self.scale_Y,
+                self.copy,
+            )
         )
         self.W = W.T
         self.P = P.T
         self.Q = Q.T
         self.R = R.T
 
-    @partial(jax.jit, static_argnums=(0, 3, 4, 5, 6))
+    @partial(jax.jit, static_argnums=(0, 3, 4, 5, 6, 7, 8))
     def stateless_fit(
         self,
         X: ArrayLike,
         Y: ArrayLike,
         A: int,
-        center: bool = True,
-        scale: bool = True,
+        center_X: bool = True,
+        center_Y: bool = True,
+        scale_X: bool = True,
+        scale_Y: bool = True,
         copy: bool = True,
     ) -> Tuple[jax.Array, jax.Array, jax.Array, jax.Array, jax.Array]:
         """
         Fits Improved Kernel PLS Algorithm #1 on `X` and `Y` using `A` components.
         Returns the internal matrices instead of storing them in the class instance.
 
         Parameters
@@ -353,14 +382,32 @@
         Y : Array of shape (N, M) or (N,)
             Response variables. Its dtype will be converted to float64 for reliable
             results.
 
         A : int
             Number of components in the PLS model.
 
+        center_X : bool, default=True
+            Whether to center `X` before fitting by subtracting its row of
+            column-wise means from each row.
+        
+        center_Y : bool, default=True
+            Whether to center `Y` before fitting by subtracting its row of
+            column-wise means from each row.
+        
+        scale_X : bool, default=True
+            Whether to scale `X` before fitting by dividing each row with the row of
+            `X`'s column-wise standard deviations. Bessel's correction for the unbiased
+            estimate of the sample standard deviation is used.
+
+        scale_Y : bool, default=True
+            Whether to scale `Y` before fitting by dividing each row with the row of
+            `X`'s column-wise standard deviations. Bessel's correction for the unbiased
+            estimate of the sample standard deviation is used.
+
         Returns
         -------
         B : Array of shape (A, K, M)
             PLS regression coefficients tensor.
 
         W : Array of shape (A, K)
             PLS weights matrix for X.
@@ -403,15 +450,15 @@
         (except B) is transposed from the usual representation.
         """
         if self.verbose:
             print(f"stateless_fit for {self.name} will be JIT compiled...")
 
         X, Y = self._initialize_input_matrices(X, Y)
         X, Y, X_mean, Y_mean, X_std, Y_std = self._center_scale_input_matrices(
-            X, Y, center, scale, copy
+            X, Y, center_X, center_Y, scale_X, scale_Y, copy
         )
 
         # Get shapes
         _N, K = X.shape
         M = Y.shape[1]
 
         # Initialize matrices
```

### Comparing `ikpls-1.2.1.post2/ikpls/jax_ikpls_base.py` & `ikpls-1.2.2/ikpls/jax_ikpls_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,23 +34,31 @@
     https://doi.org/10.1002/(SICI)1099-128X(199701)11:1%3C73::AID-CEM435%3E3.0.CO;2-%23
 
     Implementations of concrete classes exist for both Improved Kernel PLS Algorithm #1
     and Improved Kernel PLS Algorithm #2.
 
     Parameters
     ----------
-    center : bool, optional, default=True
-        Whether to center the data before fitting. If True, then the mean of the
-        training data is subtracted from the data. If False, then the data is assumed
-        to be already centered.
-
-    scale : bool, optional, default=True
-        Whether to scale the data before fitting. If True, then the data is scaled
-        using Bessel's correction for the unbiased estimate of the sample standard
-        deviation. If False, then the data is assumed to be already scaled.
+    center_X : bool, default=True
+        Whether to center the predictor variables (X) before fitting. If True, then the
+        mean of the training data is subtracted from the predictor variables.
+
+    center_Y : bool, default=True
+        Whether to center the response variables (Y) before fitting. If True, then the
+        mean of the training data is subtracted from the response variables.
+
+    scale_X : bool, default=True
+        Whether to scale the predictor variables (X) before fitting. If True, then the
+        data is scaled using Bessel's correction for the unbiased estimate of the
+        sample standard deviation.
+
+    scale_Y : bool, default=True
+        Whether to scale the response variables (Y) before fitting. If True, then the
+        data is scaled using Bessel's correction for the unbiased estimate of the
+        sample standard deviation.
 
     copy : bool, optional, default=True
         Whether to copy `X` and `Y` in fit before potentially applying centering and
         scaling. If True, then the data is copied before fitting. If False, and `dtype`
         matches the type of `X` and `Y`, then centering and scaling is done inplace,
         modifying both arrays.
 
@@ -64,27 +72,37 @@
         differentiable version is slightly slower. Results among the two versions are
         identical.
 
     verbose : bool, optional, default=False
         If True, each sub-function will print when it will be JIT compiled. This can be
         useful to track if recompilation is triggered due to passing inputs with
         different shapes.
+
+    Notes
+    -----
+    Any centering and scaling is undone before returning predictions with `fit` to
+    ensure that predictions are on the original scale. If both centering and scaling
+    are True, then the data is first centered and then scaled.
     """
 
     def __init__(
         self,
-        center: bool = True,
-        scale: bool = True,
+        center_X: bool = True,
+        center_Y: bool = True,
+        scale_X: bool = True,
+        scale_Y: bool = True,
         copy: bool = True,
         dtype: DTypeLike = jnp.float64,
         reverse_differentiable: bool = False,
         verbose: bool = False,
     ) -> None:
-        self.center = center
-        self.scale = scale
+        self.center_X = center_X
+        self.center_Y = center_Y
+        self.scale_X = scale_X
+        self.scale_Y = scale_Y
         self.copy = copy
         self.dtype = dtype
         self.reverse_differentiable = reverse_differentiable
         self.verbose = verbose
         self.name = "Improved Kernel PLS Algorithm"
         self.B = None
         self.W = None
@@ -175,121 +193,129 @@
         Y = jnp.asarray(Y, dtype=self.dtype)
 
         if Y.ndim == 1:
             Y = Y.reshape(-1, 1)
         return X, Y
 
     @partial(jax.jit, static_argnums=0)
-    def get_means(self, X: ArrayLike, Y: ArrayLike):
+    def get_mean(self, A: ArrayLike):
         """
-        Get the mean of the input matrices.
+        Get the mean of the a matrix.
 
         Parameters
         ----------
-        X : Array of shape (N, K)
-            Predictor variables matrix.
-
-        Y : Array of shape (N, M)
-            Response variables matrix.
+        A : Array of shape (N, K) or (N, M)
+            Predictor variables matrix or response variables matrix.
 
         Returns
         -------
-        X_mean : Array of shape (1, K)
-            Mean of the predictor variables.
-
-        Y_mean : Array of shape (1, M)
-            Mean of the response variables.
+        A_mean : Array of shape (1, K) or (1, M)
+            Mean of the predictor variables or response variables.
         """
         if self.verbose:
             print(f"get_means for {self.name} will be JIT compiled...")
 
-        X_mean = jnp.mean(X, axis=0, dtype=self.dtype, keepdims=True)
-        Y_mean = jnp.mean(Y, axis=0, dtype=self.dtype, keepdims=True)
-        return X_mean, Y_mean
+        A_mean = jnp.mean(A, axis=0, dtype=self.dtype, keepdims=True)
+        return A_mean
 
     @partial(jax.jit, static_argnums=0)
-    def get_stds(self, X: ArrayLike, Y: ArrayLike):
+    def get_std(self, A: ArrayLike):
         """
-        Get the standard deviation of the input matrices.
+        Get the standard deviation of a matrix.
 
         Parameters
         ----------
-        X : Array of shape (N, K)
-            Predictor variables matrix.
-
-        Y : Array of shape (N, M)
-            Response variables matrix.
+        A : Array of shape (N, K) or (N, M)
+            Predictor variables matrix or response variables matrix.
 
         Returns
         -------
-        X_std : Array of shape (1, K)
-            Sample standard deviation of the predictor variables.
-
-        Y_std : Array of shape (1, M)
-            Sample standard deviation of the response variables.
+        A_std : Array of shape (1, K) or (1, M)
+            Sample standard deviation of the predictor variables or response variables.
         """
         if self.verbose:
             print(f"get_stds for {self.name} will be JIT compiled...")
 
-        X_std = jnp.std(X, axis=0, dtype=self.dtype, keepdims=True, ddof=1)
-        Y_std = jnp.std(Y, axis=0, dtype=self.dtype, keepdims=True, ddof=1)
-        X_std = jnp.where(X_std == 0, 1, X_std)
-        Y_std = jnp.where(Y_std == 0, 1, Y_std)
-        return X_std, Y_std
+        A_std = jnp.std(A, axis=0, dtype=self.dtype, keepdims=True, ddof=1)
+        A_std = jnp.where(A_std == 0, 1, A_std)
+        return A_std
 
-    @partial(jax.jit, static_argnums=(0, 3, 4, 5))
+    @partial(jax.jit, static_argnums=(0, 3, 4, 5, 6, 7))
     def _center_scale_input_matrices(
-        self, X: jax.Array, Y: jax.Array, center: bool, scale: bool, copy: bool
+        self,
+        X: jax.Array,
+        Y: jax.Array,
+        center_X: bool,
+        center_Y: bool,
+        scale_X: bool,
+        scale_Y: bool,
+        copy: bool,
     ):
         """
         Preprocess the input matrices based on the centering and scaling parameters.
 
         Parameters
         ----------
         X : Array of shape (N, K)
             Predictor variables matrix.
 
         Y : Array of shape (N, M)
             Response variables matrix.
 
-        center : bool
-            Whether to center the data before fitting.
+        center_X : bool
+            Whether to center the predictor variables (X) before fitting.
+
+        center_Y : bool
+            Whether to center the response variables (Y) before fitting.
 
-        scale : bool
-            Whether to scale the data before fitting.
+        scale_X : bool
+            Whether to scale the predictor variables (X) before fitting.
+
+        scale_Y : bool
+            Whether to scale the response variables (Y) before fitting.
 
         Returns
         -------
         X : Array of shape (N, K)
             Potentially centered and potentially scaled variables matrix.
 
         Y : Array of shape (N, M)
             Potentially centered and potentially scaled response variables matrix.
         """
         if self.verbose:
             print(f"_preprocess_input_matrices for {self.name} will be JIT compiled...")
 
-        if (center or scale) and copy:
+        if (center_X or scale_X) and copy:
             X = X.copy()
+
+        if (center_Y or scale_Y) and copy:
             Y = Y.copy()
 
-        if center:
-            X_mean, Y_mean = self.get_means(X, Y)
+        if center_X:
+            X_mean = self.get_mean(X)
             X = X - X_mean
-            Y = Y - Y_mean
         else:
             X_mean = None
+
+        if center_Y:
+            Y_mean = self.get_mean(Y)
+            Y = Y - Y_mean
+        else:
             Y_mean = None
 
-        if scale:
-            X_std, Y_std = self.get_stds(X, Y)
+        if scale_X:
+            X_std = self.get_std(X)
             X = X / X_std
-            Y = Y / Y_std
         else:
             X_std = None
+
+        if scale_Y:
+            Y_std = self.get_std(Y)
+            Y = Y / Y_std
+        else:
             Y_std = None
 
         return X, Y, X_mean, Y_mean, X_std, Y_std
 
     @abc.abstractmethod
     @partial(jax.jit, static_argnums=(0, 1, 2, 3))
     def _get_initial_matrices(
@@ -463,15 +489,15 @@
 
         norm : float
             The l2 norm of the weight vector `w`.
 
         Notes
         -----
         This method computes the next weight vector `w` for the PLS algorithm and its
-        associated norm. It is an essential step in the PLS algorithm.
+        associated norm.
         """
         if self.verbose:
             print(f"_step_2 for {self.name} will be JIT compiled...")
         if M == 1:
             norm = jla.norm(XTY)
             w = XTY / norm
         else:
@@ -606,22 +632,24 @@
         Notes
         -----
         This method represents the main loop body of the PLS algorithm and should be
         implemented in concrete PLS classes.
         """
 
     @abc.abstractmethod
-    @partial(jax.jit, static_argnums=(0, 3))
+    @partial(jax.jit, static_argnums=(0, 3, 4, 5, 6, 7, 8))
     def stateless_fit(
         self,
         X: ArrayLike,
         Y: ArrayLike,
         A: int,
-        center: bool = True,
-        scale: bool = True,
+        center_X: bool = True,
+        center_Y: bool = True,
+        scale_X: bool = True,
+        scale_Y: bool = True,
         copy: bool = True,
     ) -> Union[
         Tuple[jax.Array, jax.Array, jax.Array, jax.Array, jax.Array],
         Tuple[jax.Array, jax.Array, jax.Array, jax.Array, jax.Array, jax.Array],
     ]:
         """
         Fits Improved Kernel PLS Algorithm #1 on `X` and `Y` using `A` components.
@@ -634,23 +662,31 @@
 
         Y : Array of shape (N, M) or (N,)
             Response variables.
 
         A : int
             Number of components in the PLS model.
 
-        center : bool, optional, default=True
-            Whether to center the data before fitting. If True, then the mean of the
-            training data is subtracted from the data. If False, then the data is
-            assumed to be already centered.
-
-        scale : bool, optional, default=True
-            Whether to scale the data before fitting. If True, then the data is scaled
-            using Bessel's correction for the unbiased estimate of the sample standard
-            deviation. If False, then the data is assumed to be already scaled.
+        center_X : bool, default=True
+            Whether to center `X` before fitting by subtracting its row of
+            column-wise means from each row.
+        
+        center_Y : bool, default=True
+            Whether to center `Y` before fitting by subtracting its row of
+            column-wise means from each row.
+        
+        scale_X : bool, default=True
+            Whether to scale `X` before fitting by dividing each row with the row of
+            `X`'s column-wise standard deviations. Bessel's correction for the unbiased
+            estimate of the sample standard deviation is used.
+
+        scale_Y : bool, default=True
+            Whether to scale `Y` before fitting by dividing each row with the row of
+            `X`'s column-wise standard deviations. Bessel's correction for the unbiased
+            estimate of the sample standard deviation is used.
 
         copy : bool, optional, default=True
             Whether to copy `X` and `Y` in fit before potentially applying centering
             and scaling. If True, then the data is copied before fitting. If False, and
             `dtype` matches the type of `X` and `Y`, then centering and scaling is done
             inplace, modifying both arrays.
 
@@ -671,25 +707,25 @@
         R : Array of shape (A, K)
             PLS weights matrix to compute scores T directly from original X.
 
         T : Array of shape (A, N)
             PLS scores matrix of X. Only Returned for Improved Kernel PLS Algorithm #1.
 
         X_mean : Array of shape (1, K) or None
-            Mean of the predictor variables `center` is True, otherwise None.
+            Mean of the predictor variables `center_X` is True, otherwise None.
 
         Y_mean : Array of shape (1, M) or None
-            Mean of the response variables `center` is True, otherwise None.
+            Mean of the response variables `center_Y` is True, otherwise None.
 
         X_std : Array of shape (1, K) or None
-            Sample standard deviation of the predictor variables `scale` is True,
+            Sample standard deviation of the predictor variables `scale_X` is True,
             otherwise None.
 
         Y_std : Array of shape (1, M) or None
-            Sample standard deviation of the response variables `scale` is True,
+            Sample standard deviation of the response variables `scale_Y` is True,
             otherwise None.
 
         Warns
         -----
         UserWarning.
             If at any point during iteration over the number of components `A`, the
             residual goes below machine epsilon.
@@ -783,27 +819,27 @@
 
         n_components : int or None, optional
             Number of components in the PLS model. If None, then all number of
             components are used.
 
         X_mean : Array of shape (1, K) or None, optional, default=None
             Mean of the predictor variables. If None, then no mean is subtracted from
-            the predictor variables.
+            `X`.
 
         X_std : Array of shape (1, K) or None, optional, default=None
             Sample standard deviation of the predictor variables. If None, then no
-            scaling is applied to the predictor variables.
+            scaling is applied to `X`.
 
         Y_mean : Array of shape (1, M) or None, optional, default=None
             Mean of the response variables. If None, then no mean is subtracted from
-            the response variables.
+            `Y`.
 
         Y_std : Array of shape (1, M) or None, optional, default=None
             Sample standard deviation of the response variables. If None, then no
-            scaling is applied to the response variables.
+            scaling is applied to `Y`.
 
         Returns
         -------
         Y_pred : Array of shape (N, M) or (A, N, M)
             If `n_components` is an int, then an array of shape (N, M) with the
             predictions for that specific number of components is used. If
             `n_components` is None, returns a prediction for each number of components
@@ -864,25 +900,27 @@
         `X_std`, `Y_mean`, and `Y_std` instead of the ones stored in the class
         instance.
         """
         return self.stateless_predict(
             X, self.B, n_components, self.X_mean, self.X_std, self.Y_mean, self.Y_std
         )
 
-    @partial(jax.jit, static_argnums=(0, 3, 6, 7, 8, 9))
+    @partial(jax.jit, static_argnums=(0, 3, 6, 7, 8, 9, 10, 11))
     def stateless_fit_predict_eval(
         self,
         X_train: ArrayLike,
         Y_train: ArrayLike,
         A: int,
         X_test: ArrayLike,
         Y_test: ArrayLike,
         metric_function: Callable[[jax.Array, jax.Array], Any],
-        center: bool = True,
-        scale: bool = True,
+        center_X: bool = True,
+        center_Y: bool = True,
+        scale_X: bool = True,
+        scale_Y: bool = True,
         copy: bool = True,
     ) -> Any:
         """
         Computes `B` with `stateless_fit`. Then computes `Y_pred` with
         `stateless_predict`. `Y_pred` is an array of shape (A, N, M). Then evaluates
         and returns the result of `metric_function(Y_test, Y_pred)`.
 
@@ -904,23 +942,31 @@
             Response variables.
 
         metric_function : Callable receiving arrays `Y_test` of shape (N, M) and
         `Y_pred` (A, N, M) and returns Any
             Computes a metric based on true values `Y_test` and predicted values
             `Y_pred`. `Y_pred` contains a prediction for all `A` components.
 
-        center : bool, optional, default=True
-            Whether to center the data before fitting. If True, then the mean of the
-            training data is subtracted from the data. If False, then the data is
-            assumed to be already centered.
-
-        scale : bool, optional, default=True
-            Whether to scale the data before fitting. If True, then the data is scaled
-            using Bessel's correction for the unbiased estimate of the sample standard
-            deviation. If False, then the data is assumed to be already scaled.
+        center_X : bool, default=True
+            Whether to center `X` before fitting by subtracting its row of
+            column-wise means from each row.
+        
+        center_Y : bool, default=True
+            Whether to center `Y` before fitting by subtracting its row of
+            column-wise means from each row.
+        
+        scale_X : bool, default=True
+            Whether to scale `X` before fitting by dividing each row with the row of
+            `X`'s column-wise standard deviations. Bessel's correction for the unbiased
+            estimate of the sample standard deviation is used.
+
+        scale_Y : bool, default=True
+            Whether to scale `Y` before fitting by dividing each row with the row of
+            `X`'s column-wise standard deviations. Bessel's correction for the unbiased
+            estimate of the sample standard deviation is used.
 
         copy : bool, optional, default=True
             Whether to copy `X_train` and `Y_train` in stateless_fit before potentially
             applying centering and scaling. If True, then the data is copied before
             fitting. If False, and `dtype` matches the type of `X` and `Y`, then
             centering and scaling is done inplace, modifying both arrays.
 
@@ -940,15 +986,22 @@
         if self.verbose:
             print(f"stateless_fit_predict_eval for {self.name} will be JIT compiled...")
 
         X_train, Y_train = self._initialize_input_matrices(X=X_train, Y=Y_train)
         X_test, Y_test = self._initialize_input_matrices(X=X_test, Y=Y_test)
 
         matrices = self.stateless_fit(
-            X=X_train, Y=Y_train, A=A, center=center, scale=scale, copy=copy
+            X=X_train,
+            Y=Y_train,
+            A=A,
+            center_X=center_X,
+            center_Y=center_Y,
+            scale_X=scale_X,
+            scale_Y=scale_Y,
+            copy=copy,
         )
         B = matrices[0]
         X_mean, Y_mean, X_std, Y_std = matrices[-4:]
         Y_pred = self.stateless_predict(
             X_test, B, X_mean=X_mean, X_std=X_std, Y_mean=Y_mean, Y_std=Y_std
         )
         return metric_function(Y_test, Y_pred)
@@ -966,17 +1019,18 @@
         metric_function: Callable[[jax.Array, jax.Array], Any],
         metric_names: list[str],
         show_progress=True,
     ) -> dict[str, Any]:
         """
         Performs cross-validation for the Partial Least-Squares (PLS) model on given
         data. `preprocessing_function` will be applied before any potential centering
-        and scaling as determined by `self.center` and `self.scale`. Any such potential
-        centering and scaling is applied for each split using training set statistics
-        to avoid data leakage from the validation set.
+        and scaling as determined by `self.center_X`, `self.center_Y`, `self.scale_X`,
+        and `self.scale_Y`. Any such potential centering and scaling is applied for
+        each split using training set statistics to avoid data leakage from the
+        validation set.
 
         Parameters
         ----------
         X : Array of shape (N, K)
             Predictor variables.
 
         Y : Array of shape (N, M) or (N,)
@@ -1044,38 +1098,42 @@
                 X=X,
                 Y=Y,
                 train_idxs=train_idxs,
                 val_idxs=val_idxs,
                 A=A,
                 preprocessing_function=preprocessing_function,
                 metric_function=metric_function,
-                center=self.center,
-                scale=self.scale,
+                center_X=self.center_X,
+                center_Y=self.center_Y,
+                scale_X=self.scale_X,
+                scale_Y=self.scale_Y,
                 copy=self.copy,
             )
             metric_value_lists = self._update_metric_value_lists(
                 metric_value_lists, metric_names, metric_values
             )
         return self._finalize_metric_values(metric_value_lists, metric_names)
 
-    @partial(jax.jit, static_argnums=(0, 5, 6, 7, 8, 9, 10))
+    @partial(jax.jit, static_argnums=(0, 5, 6, 7, 8, 9, 10, 11, 12))
     def _inner_cross_validate(
         self,
         X: ArrayLike,
         Y: ArrayLike,
         train_idxs: jax.Array,
         val_idxs: jax.Array,
         A: int,
         preprocessing_function: Callable[
             [jax.Array, jax.Array, jax.Array, jax.Array],
             Tuple[jax.Array, jax.Array, jax.Array, jax.Array],
         ],
         metric_function: Callable[[jax.Array, jax.Array], Any],
-        center: bool = True,
-        scale: bool = True,
+        center_X: bool = True,
+        center_Y: bool = True,
+        scale_X: bool = True,
+        scale_Y: bool = True,
         copy: bool = True,
     ):
         """
         Performs cross-validation for a single fold of the data and computes evaluation
         metrics.
 
         Parameters
@@ -1102,23 +1160,31 @@
             `X_val`, and `Y_val`.
 
         metric_function : Callable receiving arrays `Y_test` and `Y_pred` and returning
         Any
             Computes a metric based on true values `Y_test` and predicted values
             `Y_pred`. `Y_pred` contains a prediction for all `A` components.
 
-        center : bool, optional, default=True
-            Whether to center the data before fitting. If True, then the mean of the
-            training data is subtracted from the data. If False, then the data is
-            assumed to be already centered.
-
-        scale : bool, optional, default=True
-            Whether to scale the data before fitting. If True, then the data is scaled
-            using Bessel's correction for the unbiased estimate of the sample standard
-            deviation. If False, then the data is assumed to be already scaled.
+        center_X : bool, default=True
+            Whether to center `X` before fitting by subtracting its row of
+            column-wise means from each row.
+        
+        center_Y : bool, default=True
+            Whether to center `Y` before fitting by subtracting its row of
+            column-wise means from each row.
+        
+        scale_X : bool, default=True
+            Whether to scale `X` before fitting by dividing each row with the row of
+            `X`'s column-wise standard deviations. Bessel's correction for the unbiased
+            estimate of the sample standard deviation is used.
+
+        scale_Y : bool, default=True
+            Whether to scale `Y` before fitting by dividing each row with the row of
+            `X`'s column-wise standard deviations. Bessel's correction for the unbiased
+            estimate of the sample standard deviation is used.
 
         copy : bool, optional, default=True
             Whether to copy `X_train` and `Y_train` in stateless_fit before potentially
             applying centering and scaling. If True, then the data is copied before
             fitting. If False, and `dtype` matches the type of `X` and `Y`, then
             centering and scaling is done inplace, modifying both arrays.
 
@@ -1146,16 +1212,18 @@
         metric_values = self.stateless_fit_predict_eval(
             X_train=X_train,
             Y_train=Y_train,
             A=A,
             X_test=X_val,
             Y_test=Y_val,
             metric_function=metric_function,
-            center=center,
-            scale=scale,
+            center_X=center_X,
+            center_Y=center_Y,
+            scale_X=scale_X,
+            scale_Y=scale_Y,
             copy=copy,
         )
         return metric_values
 
     def _update_metric_value_lists(
         self,
         metric_value_lists: list[list[Any]],
```

### Comparing `ikpls-1.2.1.post2/ikpls/numpy_ikpls.py` & `ikpls-1.2.2/ikpls/numpy_ikpls.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,24 +25,32 @@
     MacGregor:
     https://doi.org/10.1002/(SICI)1099-128X(199701)11:1%3C73::AID-CEM435%3E3.0.CO;2-%23
 
     Parameters
     ----------
     algorithm : int, default=1
         Whether to use Improved Kernel PLS Algorithm #1 or #2.
-
-    center : bool, default=True
-        Whether to center the data before fitting. If True, then the mean of the
-        training data is subtracted from the data. If False, then the data is assumed
-        to be already centered.
-
-    scale : bool, default=True
-        Whether to scale the data before fitting. If True, then the data is scaled
-        using Bessel's correction for the unbiased estimate of the sample standard
-        deviation. If False, then the data is assumed to be already scaled.
+    
+    center_X : bool, default=True
+        Whether to center `X` before fitting by subtracting its row of
+        column-wise means from each row.
+    
+    center_Y : bool, default=True
+        Whether to center `Y` before fitting by subtracting its row of
+        column-wise means from each row.
+    
+    scale_X : bool, default=True
+        Whether to scale `X` before fitting by dividing each row with the row of `X`'s
+        column-wise standard deviations. Bessel's correction for the unbiased estimate
+        of the sample standard deviation is used.
+
+    scale_Y : bool, default=True
+        Whether to scale `Y` before fitting by dividing each row with the row of `X`'s
+        column-wise standard deviations. Bessel's correction for the unbiased estimate
+        of the sample standard deviation is used.
 
     copy : bool, default=True
         Whether to copy `X` and `Y` in fit before potentially applying centering and
         scaling. If True, then the data is copied before fitting. If False, and `dtype`
         matches the type of `X` and `Y`, then centering and scaling is done inplace,
         modifying both arrays.
 
@@ -51,27 +59,37 @@
         precision than float64 will yield significantly worse results when using an
         increasing number of components due to propagation of numerical errors.
 
     Raises
     ------
     ValueError
         If `algorithm` is not 1 or 2.
+
+    Notes
+    -----
+    Any centering and scaling is undone before returning predictions to ensure that
+    predictions are on the original scale. If both centering and scaling are True, then
+    the data is first centered and then scaled.
     """
 
     def __init__(
         self,
         algorithm: int = 1,
-        center: bool = True,
-        scale: bool = True,
+        center_X: bool = True,
+        center_Y: bool = True,
+        scale_X: bool = True,
+        scale_Y: bool = True,
         copy: bool = True,
         dtype: np.float_ = np.float64,
     ) -> None:
         self.algorithm = algorithm
-        self.center = center
-        self.scale = scale
+        self.center_X = center_X
+        self.center_Y = center_Y
+        self.scale_X = scale_X
+        self.scale_Y = scale_Y
         self.copy = copy
         self.dtype = dtype
         self.name = f"Improved Kernel PLS Algorithm #{algorithm}"
         if self.algorithm not in [1, 2]:
             raise ValueError(
                 f"Invalid algorithm: {self.algorithm}. Algorithm must be 1 or 2."
             )
@@ -169,30 +187,36 @@
         """
         X = np.asarray(X, dtype=self.dtype)
         Y = np.asarray(Y, dtype=self.dtype)
 
         if Y.ndim == 1:
             Y = Y.reshape(-1, 1)
 
-        if (self.center or self.scale) and self.copy:
+        if (self.center_X or self.scale_X) and self.copy:
             X = X.copy()
+
+        if (self.center_Y or self.scale_Y) and self.copy:
             Y = Y.copy()
 
-        if self.center:
+        if self.center_X:
             self.X_mean = X.mean(axis=0, dtype=self.dtype, keepdims=True)
-            self.Y_mean = Y.mean(axis=0, dtype=self.dtype, keepdims=True)
             X -= self.X_mean
+
+        if self.center_Y:
+            self.Y_mean = Y.mean(axis=0, dtype=self.dtype, keepdims=True)
             Y -= self.Y_mean
 
-        if self.scale:
+        if self.scale_X:
             self.X_std = X.std(axis=0, ddof=1, dtype=self.dtype, keepdims=True)
-            self.Y_std = Y.std(axis=0, ddof=1, dtype=self.dtype, keepdims=True)
             self.X_std[self.X_std == 0] = 1
-            self.Y_std[self.Y_std == 0] = 1
             X /= self.X_std
+
+        if self.scale_Y:
+            self.Y_std = Y.std(axis=0, ddof=1, dtype=self.dtype, keepdims=True)
+            self.Y_std[self.Y_std == 0] = 1
             Y /= self.Y_std
 
         N, K = X.shape
         M = Y.shape[1]
 
         self.B = np.zeros(shape=(A, K, M), dtype=self.dtype)
         W = np.zeros(shape=(A, K), dtype=self.dtype)
@@ -295,22 +319,22 @@
         Y_pred : Array of shape (N, M) or (A, N, M)
             If `n_components` is an int, then an array of shape (N, M) with the
             predictions for that specific number of components is used. If
             `n_components` is None, returns a prediction for each number of components
             up to `A`.
         """
         X = np.asarray(X, dtype=self.dtype)
-        if self.center:
+        if self.center_X:
             X = X - self.X_mean
-        if self.scale:
+        if self.scale_X:
             X = X / self.X_std
 
         if n_components is None:
             Y_pred = X @ self.B
         else:
             Y_pred = X @ self.B[n_components - 1]
 
-        if self.scale:
+        if self.scale_Y:
             Y_pred = Y_pred * self.Y_std
-        if self.center:
+        if self.center_Y:
             Y_pred = Y_pred + self.Y_mean
         return Y_pred
```

### Comparing `ikpls-1.2.1.post2/pyproject.toml` & `ikpls-1.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ikpls"
-version = "1.2.1.post2"
+version = "1.2.2"
 description = ""
 authors = ["Sm00thix <oleemail@icloud.com>"]
 maintainers = ["Sm00thix <oleemail@icloud.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://ikpls.readthedocs.io/en/latest/"
 repository = "https://github.com/Sm00thix/IKPLS"
```

### Comparing `ikpls-1.2.1.post2/PKG-INFO` & `ikpls-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ikpls
-Version: 1.2.1.post2
+Version: 1.2.2
 Summary: 
 Home-page: https://ikpls.readthedocs.io/en/latest/
 License: Apache-2.0
 Author: Sm00thix
 Author-email: oleemail@icloud.com
 Maintainer: Sm00thix
 Maintainer-email: oleemail@icloud.com
@@ -65,20 +65,20 @@
 benefit both IKPLS Algorithms and especially Algorithm #2. The fast
 cross-validation algorithms are mathematically equivalent to the
 classical cross-validation algorithm. Still, they are much quicker if
 cross-validation splits exceed 3. The fast cross-validation algorithms
 correctly handle (column-wise) centering and scaling of the X and Y
 input matrices using training set means and standard deviations to avoid
 data leakage from the validation set. This centering and scaling can be
-enabled by setting the center parameter to True and the scale parameter
-to True, respectively. The fast cross-validation algorithms correctly
-handle row-wise preprocessing such as (row-wise) centering and scaling
-of the X and Y input matrices, convolution, or other preprocessing.
-Row-wise preprocessing can safely be applied before passing the data to
-the fast cross-validation algorithms.
+enabled or disabled independently from eachother and for X and Y by setting 
+the parameters `center_X`, `center_Y`, `scale_X`, and `scale_Y`, respectively.
+The fast cross-validation algorithms correctly handle row-wise preprocessing
+such as (row-wise) centering and scaling of the X and Y input matrices,
+convolution, or other preprocessing. Row-wise preprocessing can safely be
+applied before passing the data to the fast cross-validation algorithms.
 
 ## Pre-requisites
 
 The JAX implementations support running on both CPU, GPU, and TPU. To
 use the GPU or TPU, follow the instructions from the [JAX Installation
 Guide](https://jax.readthedocs.io/en/latest/installation.html).
```

