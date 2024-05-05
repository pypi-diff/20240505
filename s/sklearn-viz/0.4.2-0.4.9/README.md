# Comparing `tmp/sklearn_viz-0.4.2.tar.gz` & `tmp/sklearn_viz-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklearn_viz-0.4.2.tar", max compression
+gzip compressed data, was "sklearn_viz-0.4.9.tar", max compression
```

## Comparing `sklearn_viz-0.4.2.tar` & `sklearn_viz-0.4.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0        0 2023-08-27 06:10:46.929402 sklearn_viz-0.4.2/elphick/sklearn_viz/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 02:07:15.153023 sklearn_viz-0.4.2/elphick/sklearn_viz/components/__init__.py
--rw-r--r--   0        0        0     4482 2024-04-24 02:07:15.158894 sklearn_viz-0.4.2/elphick/sklearn_viz/components/estimators.py
--rw-r--r--   0        0        0      833 2024-05-05 05:33:50.775128 sklearn_viz-0.4.2/elphick/sklearn_viz/components/kfold.py
--rw-r--r--   0        0        0      334 2023-09-18 13:02:51.287832 sklearn_viz-0.4.2/elphick/sklearn_viz/features/__init__.py
--rw-r--r--   0        0        0     8495 2024-04-24 02:07:15.169404 sklearn_viz-0.4.2/elphick/sklearn_viz/features/importance.py
--rw-r--r--   0        0        0     4738 2024-03-30 11:59:00.677281 sklearn_viz-0.4.2/elphick/sklearn_viz/features/outlier_detection.py
--rw-r--r--   0        0        0     2471 2024-03-30 11:59:00.682932 sklearn_viz-0.4.2/elphick/sklearn_viz/features/parallel_coordinates.py
--rw-r--r--   0        0        0    16988 2024-03-30 11:59:00.688949 sklearn_viz-0.4.2/elphick/sklearn_viz/features/principal_components.py
--rw-r--r--   0        0        0      668 2023-09-18 11:19:59.559906 sklearn_viz-0.4.2/elphick/sklearn_viz/features/scatter_matrix.py
--rw-r--r--   0        0        0      131 2023-09-18 13:02:51.313708 sklearn_viz-0.4.2/elphick/sklearn_viz/model_selection/__init__.py
--rw-r--r--   0        0        0     6246 2023-09-11 12:55:18.110947 sklearn_viz-0.4.2/elphick/sklearn_viz/model_selection/learning_curve.py
--rw-r--r--   0        0        0     1622 2024-04-24 02:07:15.180268 sklearn_viz-0.4.2/elphick/sklearn_viz/model_selection/metrics.py
--rw-r--r--   0        0        0    21968 2024-05-05 05:33:50.780670 sklearn_viz-0.4.2/elphick/sklearn_viz/model_selection/model_selection.py
--rw-r--r--   0        0        0     2552 2023-09-11 12:55:18.114966 sklearn_viz-0.4.2/elphick/sklearn_viz/model_selection/models.py
--rw-r--r--   0        0        0      526 2024-04-24 02:07:15.200590 sklearn_viz-0.4.2/elphick/sklearn_viz/model_selection/scorers.py
--rw-r--r--   0        0        0       22 2023-09-17 08:40:15.220711 sklearn_viz-0.4.2/elphick/sklearn_viz/residuals/__init__.py
--rw-r--r--   0        0        0     2120 2023-09-05 09:52:35.543294 sklearn_viz-0.4.2/elphick/sklearn_viz/residuals/error.py
--rw-r--r--   0        0        0       28 2023-08-27 06:10:46.931314 sklearn_viz-0.4.2/elphick/sklearn_viz/utils/__init__.py
--rw-r--r--   0        0        0     3191 2023-08-27 06:10:46.931314 sklearn_viz-0.4.2/elphick/sklearn_viz/utils/timer.py
--rw-r--r--   0        0        0     1090 2023-08-27 06:10:46.917578 sklearn_viz-0.4.2/LICENSE
--rw-r--r--   0        0        0      772 2024-05-05 07:42:05.636098 sklearn_viz-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      362 2023-08-27 06:10:46.918992 sklearn_viz-0.4.2/README.md
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 sklearn_viz-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-05 10:04:24.273292 sklearn_viz-0.4.9/LICENSE
+-rw-r--r--   0        0        0      354 2024-05-05 10:04:24.273292 sklearn_viz-0.4.9/README.md
+-rw-r--r--   0        0        0        0 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/components/__init__.py
+-rw-r--r--   0        0        0     4385 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/components/estimators.py
+-rw-r--r--   0        0        0      811 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/components/kfold.py
+-rw-r--r--   0        0        0      329 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/features/__init__.py
+-rw-r--r--   0        0        0     8306 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/features/importance.py
+-rw-r--r--   0        0        0     4633 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/features/outlier_detection.py
+-rw-r--r--   0        0        0     2403 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/features/parallel_coordinates.py
+-rw-r--r--   0        0        0    16590 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/features/principal_components.py
+-rw-r--r--   0        0        0      643 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/features/scatter_matrix.py
+-rw-r--r--   0        0        0      129 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/model_selection/__init__.py
+-rw-r--r--   0        0        0     6079 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/model_selection/learning_curve.py
+-rw-r--r--   0        0        0     1572 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/model_selection/metrics.py
+-rw-r--r--   0        0        0    21547 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/model_selection/model_selection.py
+-rw-r--r--   0        0        0     2497 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/model_selection/models.py
+-rw-r--r--   0        0        0      508 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/model_selection/scorers.py
+-rw-r--r--   0        0        0       21 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/residuals/__init__.py
+-rw-r--r--   0        0        0     2058 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/residuals/error.py
+-rw-r--r--   0        0        0       28 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/utils/__init__.py
+-rw-r--r--   0        0        0     3111 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/utils/timer.py
+-rw-r--r--   0        0        0      740 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 sklearn_viz-0.4.9/PKG-INFO
```

### Comparing `sklearn_viz-0.4.2/elphick/sklearn_viz/components/kfold.py` & `sklearn_viz-0.4.9/elphick/sklearn_viz/components/kfold.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from sklearn.model_selection import StratifiedKFold
-
-
-class FeatureStratifiedKFold:
-    """Strategy to split data into folds based on a feature column.
-
-    The standard StratifiedKFold class from scikit-learn supports stratification based on a feature column.
-    """
-
-    def __init__(self, n_splits=5, shuffle=True, random_state=42):
-        self.n_splits = n_splits
-        self.shuffle = shuffle
-        self.random_state = random_state
-        self.skfold = StratifiedKFold(n_splits=n_splits, shuffle=shuffle, random_state=random_state)
-
-    def split(self, X, y=None, groups=None):
-        if groups is None:
-            raise ValueError("The 'groups' parameter should not be None")
-        return self.skfold.split(X, groups)
-
-    def get_n_splits(self, X, y, groups=None):
-        return self.n_splits
+from sklearn.model_selection import StratifiedKFold
+
+
+class FeatureStratifiedKFold:
+    """Strategy to split data into folds based on a feature column.
+
+    The standard StratifiedKFold class from scikit-learn supports stratification based on a feature column.
+    """
+
+    def __init__(self, n_splits=5, shuffle=True, random_state=42):
+        self.n_splits = n_splits
+        self.shuffle = shuffle
+        self.random_state = random_state
+        self.skfold = StratifiedKFold(n_splits=n_splits, shuffle=shuffle, random_state=random_state)
+
+    def split(self, X, y=None, groups=None):
+        if groups is None:
+            raise ValueError("The 'groups' parameter should not be None")
+        return self.skfold.split(X, groups)
+
+    def get_n_splits(self, X, y, groups=None):
+        return self.n_splits
```

### Comparing `sklearn_viz-0.4.2/elphick/sklearn_viz/features/outlier_detection.py` & `sklearn_viz-0.4.9/elphick/sklearn_viz/features/outlier_detection.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-import logging
-from typing import Dict, Optional, Union
-
-import numpy as np
-import pandas as pd
-from scipy.stats import chi2
-import plotly.graph_objects as go
-
-from elphick.sklearn_viz.features import PrincipalComponents
-from elphick.sklearn_viz.features.principal_components import PCResults
-from elphick.sklearn_viz.features.scatter_matrix import plot_scatter_matrix
-from elphick.sklearn_viz.utils import log_timer
-
-
-def mahalanobis(x: pd.DataFrame, data: Optional[pd.DataFrame] = None, cov=None) -> pd.DataFrame:
-    if data is None:
-        data = x
-    x_mu = x - np.mean(data)
-    if not cov:
-        cov = np.cov(data.values.T)
-    inv_covmat = np.linalg.inv(cov)
-    left = np.dot(x_mu, inv_covmat)
-    mahal = np.dot(left, x_mu.T).diagonal()
-    pvals = 1 - chi2.cdf(mahal, len(x.columns) - 1)
-    res: pd.DataFrame = pd.DataFrame(np.vstack((mahal, pvals)).T, columns=['mahal_dist', 'p_val'], index=x.index)
-    return res
-
-
-def plot_outlier_matrix(x: pd.DataFrame, pca_spec: Union[float, int] = 0, p_val: float = 0.001,
-                        principal_components: bool = False) -> go.Figure:
-    """Detect and plot outliers
-
-    Args:
-        x: X values for outlier detection.
-        pca_spec: If zero, pca is not used.  For integers (n) > 0 outlier detection is performed on the
-         top n principal components. For values (f) < 1, outlier detection is performed on the number of
-         principal components that explain f% of the variance.
-        p_val: the p-value threshold for outlier detection.
-        principal_components: If True (and pca_spec is not 0) the principal components will be plotted.  Otherwise,
-         will plot in the original feature space.
-    """
-    return OutlierDetection(x=x, pca_spec=pca_spec, p_val=p_val).plot_outlier_matrix(
-        principal_components=principal_components)
-
-
-class OutlierDetection:
-    def __init__(self, x: pd.DataFrame, pca_spec: Union[float, int] = 0,
-                 standardise: bool = False, p_val: float = 0.001):
-        """
-
-        Args:
-            x: X values for outlier detection.
-            pca_spec: If zero, pca is not used.  For integers (n) > 0 outlier detection is performed on the
-             top n principal components. For values (f) < 1, outlier detection is performed on the number of
-             principal components that explain f% of the variance.
-            standardise: If True, standardise the data prior to PCA, where vectors are transformed to zero mean and
-             unit variance.
-            p_val: the p-value threshold for outlier detection.
-        """
-        self._logger = logging.getLogger(name=__class__.__name__)
-        self.x: pd.DataFrame = x
-        self.pca_spec: Union[float, int] = pca_spec
-        self.standardise: bool = standardise
-        self.p_val: float = p_val
-
-        self._data: Optional[Dict] = None
-
-    @property
-    @log_timer
-    def data(self) -> Optional[Dict]:
-        if self._data is not None:
-            res = self._data
-        else:
-            label: str = 'std' if self.standardise else 'raw'
-            res: Dict = {}
-            if self.pca_spec != 0:
-                res['pca'] = PrincipalComponents(self.x)
-                pca_data: PCResults = res['pca'].data[label]
-                if self.pca_spec >= 1:
-                    mahal = mahalanobis(x=pca_data.data.iloc[:, 0:self.pca_spec])
-                elif self.pca_spec < 1:
-                    num_required: int = next(i for i, v in
-                                             enumerate(pca_data.explained_variance.cumsum() / 100 >= self.pca_spec) if
-                                             v is True) + 1
-                    mahal = mahalanobis(x=pca_data.data.iloc[:, 0:num_required])
-                else:
-                    raise ValueError("pca_spec cannot be negative")
-            else:
-                mahal = mahalanobis(x=self.x)
-
-            res['mahal'] = mahal
-            res['outlier'] = pd.Series(res['mahal']['p_val'] < self.p_val, name='outlier')
-            self._data = res
-        return res
-
-    def plot_outlier_matrix(self, principal_components: bool = False) -> go.Figure:
-        if principal_components:
-            if 'pca' in self.data.keys():
-                fig = self.data['pca'].plot_scatter_matrix(original_features=True, y=self.data['outlier'])
-            else:
-                raise ValueError("Outliers not defined using PCA.  Try changing pca_spec.")
-        else:
-            fig = plot_scatter_matrix(x=pd.concat([self.x, self.data['outlier']], axis=1), color='outlier',
-                                      title="Outlier Scatter Matrix")
-        return fig
+import logging
+from typing import Dict, Optional, Union
+
+import numpy as np
+import pandas as pd
+from scipy.stats import chi2
+import plotly.graph_objects as go
+
+from elphick.sklearn_viz.features import PrincipalComponents
+from elphick.sklearn_viz.features.principal_components import PCResults
+from elphick.sklearn_viz.features.scatter_matrix import plot_scatter_matrix
+from elphick.sklearn_viz.utils import log_timer
+
+
+def mahalanobis(x: pd.DataFrame, data: Optional[pd.DataFrame] = None, cov=None) -> pd.DataFrame:
+    if data is None:
+        data = x
+    x_mu = x - np.mean(data)
+    if not cov:
+        cov = np.cov(data.values.T)
+    inv_covmat = np.linalg.inv(cov)
+    left = np.dot(x_mu, inv_covmat)
+    mahal = np.dot(left, x_mu.T).diagonal()
+    pvals = 1 - chi2.cdf(mahal, len(x.columns) - 1)
+    res: pd.DataFrame = pd.DataFrame(np.vstack((mahal, pvals)).T, columns=['mahal_dist', 'p_val'], index=x.index)
+    return res
+
+
+def plot_outlier_matrix(x: pd.DataFrame, pca_spec: Union[float, int] = 0, p_val: float = 0.001,
+                        principal_components: bool = False) -> go.Figure:
+    """Detect and plot outliers
+
+    Args:
+        x: X values for outlier detection.
+        pca_spec: If zero, pca is not used.  For integers (n) > 0 outlier detection is performed on the
+         top n principal components. For values (f) < 1, outlier detection is performed on the number of
+         principal components that explain f% of the variance.
+        p_val: the p-value threshold for outlier detection.
+        principal_components: If True (and pca_spec is not 0) the principal components will be plotted.  Otherwise,
+         will plot in the original feature space.
+    """
+    return OutlierDetection(x=x, pca_spec=pca_spec, p_val=p_val).plot_outlier_matrix(
+        principal_components=principal_components)
+
+
+class OutlierDetection:
+    def __init__(self, x: pd.DataFrame, pca_spec: Union[float, int] = 0,
+                 standardise: bool = False, p_val: float = 0.001):
+        """
+
+        Args:
+            x: X values for outlier detection.
+            pca_spec: If zero, pca is not used.  For integers (n) > 0 outlier detection is performed on the
+             top n principal components. For values (f) < 1, outlier detection is performed on the number of
+             principal components that explain f% of the variance.
+            standardise: If True, standardise the data prior to PCA, where vectors are transformed to zero mean and
+             unit variance.
+            p_val: the p-value threshold for outlier detection.
+        """
+        self._logger = logging.getLogger(name=__class__.__name__)
+        self.x: pd.DataFrame = x
+        self.pca_spec: Union[float, int] = pca_spec
+        self.standardise: bool = standardise
+        self.p_val: float = p_val
+
+        self._data: Optional[Dict] = None
+
+    @property
+    @log_timer
+    def data(self) -> Optional[Dict]:
+        if self._data is not None:
+            res = self._data
+        else:
+            label: str = 'std' if self.standardise else 'raw'
+            res: Dict = {}
+            if self.pca_spec != 0:
+                res['pca'] = PrincipalComponents(self.x)
+                pca_data: PCResults = res['pca'].data[label]
+                if self.pca_spec >= 1:
+                    mahal = mahalanobis(x=pca_data.data.iloc[:, 0:self.pca_spec])
+                elif self.pca_spec < 1:
+                    num_required: int = next(i for i, v in
+                                             enumerate(pca_data.explained_variance.cumsum() / 100 >= self.pca_spec) if
+                                             v is True) + 1
+                    mahal = mahalanobis(x=pca_data.data.iloc[:, 0:num_required])
+                else:
+                    raise ValueError("pca_spec cannot be negative")
+            else:
+                mahal = mahalanobis(x=self.x)
+
+            res['mahal'] = mahal
+            res['outlier'] = pd.Series(res['mahal']['p_val'] < self.p_val, name='outlier')
+            self._data = res
+        return res
+
+    def plot_outlier_matrix(self, principal_components: bool = False) -> go.Figure:
+        if principal_components:
+            if 'pca' in self.data.keys():
+                fig = self.data['pca'].plot_scatter_matrix(original_features=True, y=self.data['outlier'])
+            else:
+                raise ValueError("Outliers not defined using PCA.  Try changing pca_spec.")
+        else:
+            fig = plot_scatter_matrix(x=pd.concat([self.x, self.data['outlier']], axis=1), color='outlier',
+                                      title="Outlier Scatter Matrix")
+        return fig
```

### Comparing `sklearn_viz-0.4.2/elphick/sklearn_viz/features/parallel_coordinates.py` & `sklearn_viz-0.4.9/elphick/sklearn_viz/features/parallel_coordinates.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-from typing import Optional, List
-
-import pandas as pd
-
-import plotly.graph_objects as go
-
-
-def plot_parallel_coordinates(data: pd.DataFrame,
-                              color: Optional[str] = None,
-                              vars_include: Optional[List[str]] = None,
-                              vars_exclude: Optional[List[str]] = None,
-                              title: Optional[str] = None,
-                              ) -> go.Figure:
-    """Create an interactive parallel plot
-
-    Useful to explore multidimensional data like mass-composition data
-
-    Args:
-        data: The DataFrame to plot
-        color: The variable that sets the color, typically the target variable
-        vars_include: Optional List of variables to include in the plot
-        vars_exclude: Optional List of variables to exclude in the plot
-        title: Optional plot title
-
-    Returns:
-
-    """
-    df: pd.DataFrame = data.copy()
-    if vars_include is not None:
-        missing_vars = set(vars_include).difference(set(df.columns))
-        if len(missing_vars) > 0:
-            raise KeyError(f'vars_include provided contains variable not found in the data: {missing_vars}')
-        df = df[vars_include]
-    if vars_exclude:
-        df = df[[col for col in df.columns if col not in vars_exclude]]
-
-    # Kudos: https://stackoverflow.com/questions/72125802/parallel-coordinate-plot-in-plotly-with-continuous-
-    # and-categorical-data
-
-    categorical_columns = df.select_dtypes(include=['category', 'object'])
-    col_list = []
-
-    for col in df.columns:
-        if col in categorical_columns:  # categorical columns
-            cat_map: dict = dict(enumerate(df[col].cat.categories))
-            df[col] = df[col].cat.codes
-            col_dict = dict(
-                label=col,
-                tickvals=list(cat_map.keys()),
-                ticktext=list(cat_map.values()),
-                values=df[col],
-            )
-        else:  # continuous columns
-            col_dict = dict(
-                range=(df[col].min(), df[col].max()),
-                label=col,
-                values=df[col],
-            )
-        col_list.append(col_dict)
-
-    if color is None:
-        fig = go.Figure(data=go.Parcoords(dimensions=col_list))
-    else:
-        fig = go.Figure(data=go.Parcoords(dimensions=col_list, line=dict(color=df[color])))
-
-    fig.update_layout(title=title, height=700)
-
-    return fig
+from typing import Optional, List
+
+import pandas as pd
+
+import plotly.graph_objects as go
+
+
+def plot_parallel_coordinates(data: pd.DataFrame,
+                              color: Optional[str] = None,
+                              vars_include: Optional[List[str]] = None,
+                              vars_exclude: Optional[List[str]] = None,
+                              title: Optional[str] = None,
+                              ) -> go.Figure:
+    """Create an interactive parallel plot
+
+    Useful to explore multidimensional data like mass-composition data
+
+    Args:
+        data: The DataFrame to plot
+        color: The variable that sets the color, typically the target variable
+        vars_include: Optional List of variables to include in the plot
+        vars_exclude: Optional List of variables to exclude in the plot
+        title: Optional plot title
+
+    Returns:
+
+    """
+    df: pd.DataFrame = data.copy()
+    if vars_include is not None:
+        missing_vars = set(vars_include).difference(set(df.columns))
+        if len(missing_vars) > 0:
+            raise KeyError(f'vars_include provided contains variable not found in the data: {missing_vars}')
+        df = df[vars_include]
+    if vars_exclude:
+        df = df[[col for col in df.columns if col not in vars_exclude]]
+
+    # Kudos: https://stackoverflow.com/questions/72125802/parallel-coordinate-plot-in-plotly-with-continuous-
+    # and-categorical-data
+
+    categorical_columns = df.select_dtypes(include=['category', 'object'])
+    col_list = []
+
+    for col in df.columns:
+        if col in categorical_columns:  # categorical columns
+            cat_map: dict = dict(enumerate(df[col].cat.categories))
+            df[col] = df[col].cat.codes
+            col_dict = dict(
+                label=col,
+                tickvals=list(cat_map.keys()),
+                ticktext=list(cat_map.values()),
+                values=df[col],
+            )
+        else:  # continuous columns
+            col_dict = dict(
+                range=(df[col].min(), df[col].max()),
+                label=col,
+                values=df[col],
+            )
+        col_list.append(col_dict)
+
+    if color is None:
+        fig = go.Figure(data=go.Parcoords(dimensions=col_list))
+    else:
+        fig = go.Figure(data=go.Parcoords(dimensions=col_list, line=dict(color=df[color])))
+
+    fig.update_layout(title=title, height=700)
+
+    return fig
```

### Comparing `sklearn_viz-0.4.2/elphick/sklearn_viz/features/principal_components.py` & `sklearn_viz-0.4.9/elphick/sklearn_viz/features/principal_components.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,398 +1,398 @@
-"""
-Developed from the example here: https://plotly.com/python/pca-visualization/
-"""
-import dataclasses
-import logging
-from typing import Optional, List, Dict
-
-import numpy as np
-import pandas as pd
-import plotly.graph_objects as go
-import plotly.express as px
-from pandas.core.dtypes.common import is_numeric_dtype
-from sklearn.decomposition import PCA
-from sklearn.pipeline import make_pipeline
-from sklearn.preprocessing import StandardScaler
-
-from elphick.sklearn_viz.utils import log_timer
-
-
-def plot_principal_components(x: pd.DataFrame,
-                              color: Optional[pd.Series] = None,
-                              plot_3d: bool = True,
-                              loading_vectors: bool = True,
-                              standardised: bool = False,
-                              title: Optional[str] = None) -> go.Figure:
-    """
-
-    Args:
-        x: X values to transform and plot.
-        color: optional series by which to color the markers
-        plot_3d: If True plot the top 3 principal components in 3D, otherwise the top 2 in 2D.
-        loading_vectors: If True and plot_type is '2D'|'3D' loading vectors will be displayed.
-        standardised: If True, plot the standardised PCA, where vectors are transformed to zero mean and
-             unit variance.
-        title: Optional plot title
-
-    Returns:
-        a plotly GraphObjects.Figure
-
-    """
-
-    return PrincipalComponents(x=x, color=color).plot_principal_components(plot_3d=plot_3d,
-                                                                           loading_vectors=loading_vectors,
-                                                                           standardised=standardised,
-                                                                           title=title)
-
-
-def plot_explained_variance(x: pd.DataFrame, y: Optional[pd.Series] = None,
-                            title: Optional[str] = None) -> go.Figure:
-    """Plot the cumulative explained variance by principal component.
-
-    Args:
-        x: X values to transform and plot.
-        y: optional target vector
-        title: Optional plot title
-
-    Returns:
-
-    """
-    return PrincipalComponents(x=x, color=y).plot_explained_variance(title=title)
-
-
-def plot_scatter_matrix(x: pd.DataFrame, y: Optional[pd.Series] = None,
-                        original_features: bool = False, title: Optional[str] = None) -> go.Figure:
-    """Plot a scatter matrix
-
-    Args:
-        x: X values to transform and plot.
-        y: optional series by which to color the markers
-        original_features: If True, plot the original features, otherwise plot the principal components.
-        title: Optional plot title
-
-    Returns:
-
-    """
-    return PrincipalComponents(x=x, color=y).plot_scatter_matrix(original_features=original_features, title=title)
-
-
-def plot_loading_vectors(x: pd.DataFrame,
-                         color: Optional[pd.Series] = None,
-                         standardised: bool = False,
-                         title: Optional[str] = None) -> go.Figure:
-    """
-
-    Args:
-        x: X values to transform and plot.
-        color: optional series by which to color the markers
-        standardised: If True, plot the standardised PCA, where vectors are transformed to zero mean and
-             unit variance.
-        title: Optional plot title
-
-    Returns:
-        a plotly GraphObjects.Figure
-
-    """
-
-    return PrincipalComponents(x=x, color=color).plot_loading_vectors(standardised=standardised, title=title,
-                                                                      by_color=color is not None)
-
-
-def plot_correlation_circle(x: pd.DataFrame,
-                            color: Optional[pd.Series] = None,
-                            title: Optional[str] = None) -> go.Figure:
-    """
-
-    Args:
-        x: X values to transform and plot.
-        color: optional series by which to color the markers
-        title: Optional plot title
-
-    Returns:
-        a plotly GraphObjects.Figure
-
-    """
-
-    return PrincipalComponents(x=x, color=color).plot_loading_vectors(standardised=True, title=title,
-                                                                      by_color=color is not None)
-
-
-@dataclasses.dataclass
-class PCResults:
-    """Class to hold Principal Component results"""
-    data: pd.DataFrame
-    explained_variance: pd.Series
-    loadings: pd.DataFrame
-
-
-class PrincipalComponents:
-    def __init__(self, x: pd.DataFrame, color: Optional[pd.Series] = None):
-        """
-
-        Args:
-            x: X values to transform and plot.
-            color: the optional series by which to color the markers
-        """
-        self._logger = logging.getLogger(name=__class__.__name__)
-        self.x: pd.DataFrame = x
-        self.color: Optional[pd.Series] = color
-
-        self._data: Optional[Dict] = None
-
-    @property
-    @log_timer
-    def data(self) -> Optional[Dict]:
-        def get_pca_results(pipe, x):
-            xt: pd.DataFrame = pipe.fit_transform(x)
-            xt.columns = [f"PC{i + 1}" for i in range(len(x.columns))]
-            var: pd.Series = pd.Series(data=pipe['pca'].explained_variance_ratio_ * 100., name='explained_variance')
-            loadings = pd.DataFrame(data=pipe['pca'].components_.T * np.sqrt(pipe['pca'].explained_variance_),
-                                    index=x.columns, columns=xt.columns)
-            return PCResults(data=xt, explained_variance=var, loadings=loadings)
-
-        if self._data is not None:
-            res = self._data
-        else:
-            res: Dict = {}
-            self._logger.info("Commencing PCA")
-            pca = make_pipeline(PCA()).set_output(transform="pandas")
-            pca_std = make_pipeline(StandardScaler(), PCA()).set_output(transform="pandas")
-            for label, pipe in {'raw': pca, 'std': pca_std}.items():
-                res[label] = get_pca_results(pipe=pipe, x=self.x)
-                if (self.color is not None) & (not is_numeric_dtype(self.color)):
-                    for grp in self.color.unique():
-                        if 'group' not in res.keys():
-                            res['group'] = dict()
-                        if grp not in res['group'].keys():
-                            res['group'][grp] = dict()
-                        res['group'][grp][label] = get_pca_results(pipe=pipe, x=self.x.loc[self.color == grp, :])
-            self._data = res
-
-        return res
-
-    def plot_principal_components(self,
-                                  plot_3d: bool = False,
-                                  loading_vectors: bool = True,
-                                  standardised: bool = False,
-                                  title: Optional[str] = None) -> go.Figure:
-        """Create the pca plot
-
-        Args:
-            plot_3d: If True plot the top 3 principal components in 3D, otherwise the top 2 in 2D.
-            loading_vectors: If True and plot_type is '2D'|'3D' loading vectors will be displayed.
-            standardised: If True, plot the standardised PCA, where vectors are transformed to zero mean and
-             unit variance.
-            title: Optional plot title
-
-        Loading vectors are implemented manually rather than with annotations (lines with arrows),
-         the problem is described well here:
-         https://community.plotly.com/t/set-pca-loadings-aka-arrows-in-a-3d-scatter-plot/72905
-
-        Returns:
-            a plotly GraphObjects.Figure
-
-        """
-        label: str = 'std' if standardised else 'raw'
-        pca_data: pd.DataFrame = self.data[label].data
-        pca_loadings: pd.DataFrame = self.data[label].loadings
-        pca_variance: pd.DataFrame = self.data[label].explained_variance
-
-        df_plot: pd.DataFrame = pd.concat([pca_data, self.x], axis=1).reset_index()
-        if plot_3d:
-            fig = px.scatter_3d(df_plot, x='PC1', y='PC2', z='PC3',
-                                color=self.color, hover_data=list(self.x.reset_index().columns))
-            fig.update_traces(marker_size=4)
-            if loading_vectors:
-
-                annots: List = [dict(x=row.PC1, y=row.PC2, z=row.PC3,
-                                     text=i, showarrow=False,
-                                     xanchor="left", xshift=10, yshift=10, opacity=0.7) for i, row in
-                                pca_loadings.iterrows()]
-                fig.update_layout(scene=dict(annotations=annots))
-                for feature_name, row in pca_loadings.iterrows():
-                    # noinspection PyTypeChecker
-                    fig.add_trace(
-                        go.Scatter3d(x=(row.PC1,), y=(row.PC2,), z=(row.PC3,), mode='markers',
-                                     marker={'size': 6, 'line': dict(width=2, color='black')},
-                                     name=feature_name,
-                                     showlegend=True,
-                                     legendgroup="features",
-                                     legendgrouptitle_text="feature vectors",
-                                     ))
-                    fig.add_trace(
-                        go.Scatter3d(x=(0, row.PC1), y=(0, row.PC2), z=(0, row.PC3), mode='lines',
-                                     line={'width': 5, 'color': 'black'},
-                                     name=feature_name,
-                                     showlegend=False))
-                fig.update_layout(legend=dict(groupclick="toggleitem"))
-                title = (f"Top 3 Principal Components<br>Explained Variance = "
-                         f"{round(pca_variance.iloc[0:3].sum(), 1)}%") if title is None else title
-        else:  # 2D
-            fig = px.scatter(df_plot, x='PC1', y='PC2',
-                             color=self.color, hover_data=list(self.x.reset_index().columns))
-            fig.update_traces(marker_size=5)
-
-            if loading_vectors:
-                loadings = pca_loadings.iloc[:, 0:2]
-                self.add_loading_vectors(fig, loadings)
-            title = (f"Top 2 Principal Components<br>Explained Variance = "
-                     f"{round(pca_variance.iloc[0:2].sum(), 1)}%") if title is None else title
-
-        fig.update_layout(legend_title_text=self.color.name)
-        fig.update_layout(title=title,
-                          xaxis_title=f"PC1 ({round(self.data['std'].explained_variance.iloc[0], 1)}%)",
-                          yaxis_title=f"PC2 ({round(self.data['std'].explained_variance.iloc[1], 1)}%)")
-        if self.color is not None:
-            fig.update_layout(coloraxis_colorbar_title_text=self.color.name)
-
-        return fig
-
-    def plot_explained_variance(self,
-                                standardised: bool = False,
-                                title: Optional[str] = None) -> go.Figure:
-        """Plot the cumulative explained variance by principal component.
-
-        Args:
-            standardised: If True, plot the standardised PCA, where vectors are transformed to zero mean and
-             unit variance.
-            title: Optional plot title
-
-        Returns:
-
-        """
-        pca_variance: pd.DataFrame = self.data['std'].explained_variance if standardised else self.data[
-            'raw'].explained_variance
-        exp_var_cumul = np.cumsum(pca_variance)
-        fig = px.area(
-            x=range(1, exp_var_cumul.shape[0] + 1),
-            y=exp_var_cumul,
-            labels={"x": "# Components", "y": "Explained Variance"}
-        )
-        title = 'Cumulative Explained Variance by Principal Component' if title is None else title
-        fig.update_layout(title=title)
-        fig.update_xaxes(type='category')
-
-        return fig
-
-    def plot_scatter_matrix(self, original_features: bool = False, standardised: bool = False,
-                            title: Optional[str] = None) -> go.Figure:
-        """Plot a scatter matrix
-
-        Args:
-            original_features: If True, plot the original features, otherwise plot the principal components.
-            standardised: If True, plot the standardised PCA, where vectors are transformed to zero mean and
-             unit variance.
-            title: Optional plot title
-
-        Returns:
-
-        """
-        label: str = 'std' if standardised else 'raw'
-        y = self.color
-        if original_features:
-            x = self.x
-            title = 'Scatter Matrix - Original Feature Space' if title is None else title
-        else:
-            x = self.data[label].data
-            title = 'Scatter Matrix - All Principal Components' if title is None else title
-
-        if original_features:
-            df_plot: pd.DataFrame = pd.concat([x, y], axis=1).reset_index()
-            hover_data = ['index' if x.index.name is None else x.index.name]
-        else:
-            df_plot: pd.DataFrame = pd.concat([x, y, self.x], axis=1).reset_index()
-            hover_data = list(self.x.reset_index().columns)
-
-        fig = px.scatter_matrix(data_frame=df_plot, dimensions=list(x.columns),
-                                color=y.name, hover_data=hover_data)
-        fig.update_traces(diagonal_visible=False)
-        title = 'Top 3 Principal Components' if title is None else title
-        fig.update_layout(title=title)
-
-        return fig
-
-    def plot_loading_vectors(self, standardised: bool = False, by_color: bool = False,
-                             title: Optional[str] = None) -> go.Figure:
-        """plot the loading vectors.
-
-        Args:
-            standardised: If True, plot the standardised PCA, where vectors are transformed to zero mean and
-             unit variance.
-             by_color: If True, plot the loading vectors by color group.
-            title: Optional plot title
-
-        Returns:
-            a plotly GraphObjects.Figure
-
-        """
-        label: str = 'std' if standardised else 'raw'
-        if by_color:
-            chunks = []
-
-            for grp, d_label in self.data['group'].items():
-                chunks.append(self.data['group'][grp][label].loadings.assign(group=grp))
-            loadings = pd.concat(chunks, axis='index')
-            fig = px.scatter(loadings, x='PC1', y='PC2', color='group',
-                             hover_data=loadings.columns.tolist())
-
-        else:
-            loadings = self.data[label].loadings.iloc[:, 0:2]
-            fig = px.scatter(loadings, x='PC1', y='PC2', hover_data=loadings.columns.tolist())
-        fig.update_traces(marker=dict(size=1))
-
-        if standardised:
-            fig.add_shape(type="circle",
-                          xref="x", yref="y",
-                          x0=-1, y0=-1, x1=1, y1=1,
-                          line_color="gray")
-            title_main = "Correlation Circle"
-        else:
-            title_main = "Top 2 Principal Components"
-
-        fig = self.add_loading_vectors(fig, loadings)
-        title = (f"{title_main}<br>Explained Variance = "
-                 f"{round(self.data['std'].explained_variance.iloc[0:2].sum(), 1)}%") if title is None else title
-
-        fig.update_layout(title=title,
-                          xaxis_title=f"PC1 ({round(self.data['std'].explained_variance.iloc[0], 1)}%)",
-                          yaxis_title=f"PC2 ({round(self.data['std'].explained_variance.iloc[1], 1)}%)")
-        fig.update_yaxes(scaleanchor="x", scaleratio=1)
-        fig.update_layout(scene=dict(aspectmode="data"))
-
-        return fig
-
-    def add_loading_vectors(self, fig, loadings) -> go.Figure:
-        if 'group' in loadings.columns:
-            cm = px.colors.qualitative.Plotly
-            grp_colors = dict(zip(loadings['group'].unique(), cm[0:len(loadings['group'].unique())]))
-        for i, feature in enumerate(loadings.index):
-            if 'group' in loadings.columns:
-                grp = loadings.iloc[i, :]['group']
-                arrowcolor = grp_colors[grp]
-                font = dict(color=grp_colors[grp])
-            else:
-                arrowcolor = None
-                font = None
-            fig.add_annotation(
-                ax=0, ay=0,
-                axref="x", ayref="y",
-                x=loadings.iloc[i, 0],
-                y=loadings.iloc[i, 1],
-                showarrow=True,
-                arrowsize=2,
-                arrowhead=2,
-                xanchor="right",
-                yanchor="top",
-                arrowcolor=arrowcolor,
-            )
-            fig.add_annotation(
-                x=loadings.iloc[i, 0],
-                y=loadings.iloc[i, 1],
-                ax=0, ay=0,
-                xanchor="center",
-                yanchor="bottom",
-                text=feature,
-                yshift=5,
-                font=font
-            )
-        return fig
+"""
+Developed from the example here: https://plotly.com/python/pca-visualization/
+"""
+import dataclasses
+import logging
+from typing import Optional, List, Dict
+
+import numpy as np
+import pandas as pd
+import plotly.graph_objects as go
+import plotly.express as px
+from pandas.core.dtypes.common import is_numeric_dtype
+from sklearn.decomposition import PCA
+from sklearn.pipeline import make_pipeline
+from sklearn.preprocessing import StandardScaler
+
+from elphick.sklearn_viz.utils import log_timer
+
+
+def plot_principal_components(x: pd.DataFrame,
+                              color: Optional[pd.Series] = None,
+                              plot_3d: bool = True,
+                              loading_vectors: bool = True,
+                              standardised: bool = False,
+                              title: Optional[str] = None) -> go.Figure:
+    """
+
+    Args:
+        x: X values to transform and plot.
+        color: optional series by which to color the markers
+        plot_3d: If True plot the top 3 principal components in 3D, otherwise the top 2 in 2D.
+        loading_vectors: If True and plot_type is '2D'|'3D' loading vectors will be displayed.
+        standardised: If True, plot the standardised PCA, where vectors are transformed to zero mean and
+             unit variance.
+        title: Optional plot title
+
+    Returns:
+        a plotly GraphObjects.Figure
+
+    """
+
+    return PrincipalComponents(x=x, color=color).plot_principal_components(plot_3d=plot_3d,
+                                                                           loading_vectors=loading_vectors,
+                                                                           standardised=standardised,
+                                                                           title=title)
+
+
+def plot_explained_variance(x: pd.DataFrame, y: Optional[pd.Series] = None,
+                            title: Optional[str] = None) -> go.Figure:
+    """Plot the cumulative explained variance by principal component.
+
+    Args:
+        x: X values to transform and plot.
+        y: optional target vector
+        title: Optional plot title
+
+    Returns:
+
+    """
+    return PrincipalComponents(x=x, color=y).plot_explained_variance(title=title)
+
+
+def plot_scatter_matrix(x: pd.DataFrame, y: Optional[pd.Series] = None,
+                        original_features: bool = False, title: Optional[str] = None) -> go.Figure:
+    """Plot a scatter matrix
+
+    Args:
+        x: X values to transform and plot.
+        y: optional series by which to color the markers
+        original_features: If True, plot the original features, otherwise plot the principal components.
+        title: Optional plot title
+
+    Returns:
+
+    """
+    return PrincipalComponents(x=x, color=y).plot_scatter_matrix(original_features=original_features, title=title)
+
+
+def plot_loading_vectors(x: pd.DataFrame,
+                         color: Optional[pd.Series] = None,
+                         standardised: bool = False,
+                         title: Optional[str] = None) -> go.Figure:
+    """
+
+    Args:
+        x: X values to transform and plot.
+        color: optional series by which to color the markers
+        standardised: If True, plot the standardised PCA, where vectors are transformed to zero mean and
+             unit variance.
+        title: Optional plot title
+
+    Returns:
+        a plotly GraphObjects.Figure
+
+    """
+
+    return PrincipalComponents(x=x, color=color).plot_loading_vectors(standardised=standardised, title=title,
+                                                                      by_color=color is not None)
+
+
+def plot_correlation_circle(x: pd.DataFrame,
+                            color: Optional[pd.Series] = None,
+                            title: Optional[str] = None) -> go.Figure:
+    """
+
+    Args:
+        x: X values to transform and plot.
+        color: optional series by which to color the markers
+        title: Optional plot title
+
+    Returns:
+        a plotly GraphObjects.Figure
+
+    """
+
+    return PrincipalComponents(x=x, color=color).plot_loading_vectors(standardised=True, title=title,
+                                                                      by_color=color is not None)
+
+
+@dataclasses.dataclass
+class PCResults:
+    """Class to hold Principal Component results"""
+    data: pd.DataFrame
+    explained_variance: pd.Series
+    loadings: pd.DataFrame
+
+
+class PrincipalComponents:
+    def __init__(self, x: pd.DataFrame, color: Optional[pd.Series] = None):
+        """
+
+        Args:
+            x: X values to transform and plot.
+            color: the optional series by which to color the markers
+        """
+        self._logger = logging.getLogger(name=__class__.__name__)
+        self.x: pd.DataFrame = x
+        self.color: Optional[pd.Series] = color
+
+        self._data: Optional[Dict] = None
+
+    @property
+    @log_timer
+    def data(self) -> Optional[Dict]:
+        def get_pca_results(pipe, x):
+            xt: pd.DataFrame = pipe.fit_transform(x)
+            xt.columns = [f"PC{i + 1}" for i in range(len(x.columns))]
+            var: pd.Series = pd.Series(data=pipe['pca'].explained_variance_ratio_ * 100., name='explained_variance')
+            loadings = pd.DataFrame(data=pipe['pca'].components_.T * np.sqrt(pipe['pca'].explained_variance_),
+                                    index=x.columns, columns=xt.columns)
+            return PCResults(data=xt, explained_variance=var, loadings=loadings)
+
+        if self._data is not None:
+            res = self._data
+        else:
+            res: Dict = {}
+            self._logger.info("Commencing PCA")
+            pca = make_pipeline(PCA()).set_output(transform="pandas")
+            pca_std = make_pipeline(StandardScaler(), PCA()).set_output(transform="pandas")
+            for label, pipe in {'raw': pca, 'std': pca_std}.items():
+                res[label] = get_pca_results(pipe=pipe, x=self.x)
+                if (self.color is not None) & (not is_numeric_dtype(self.color)):
+                    for grp in self.color.unique():
+                        if 'group' not in res.keys():
+                            res['group'] = dict()
+                        if grp not in res['group'].keys():
+                            res['group'][grp] = dict()
+                        res['group'][grp][label] = get_pca_results(pipe=pipe, x=self.x.loc[self.color == grp, :])
+            self._data = res
+
+        return res
+
+    def plot_principal_components(self,
+                                  plot_3d: bool = False,
+                                  loading_vectors: bool = True,
+                                  standardised: bool = False,
+                                  title: Optional[str] = None) -> go.Figure:
+        """Create the pca plot
+
+        Args:
+            plot_3d: If True plot the top 3 principal components in 3D, otherwise the top 2 in 2D.
+            loading_vectors: If True and plot_type is '2D'|'3D' loading vectors will be displayed.
+            standardised: If True, plot the standardised PCA, where vectors are transformed to zero mean and
+             unit variance.
+            title: Optional plot title
+
+        Loading vectors are implemented manually rather than with annotations (lines with arrows),
+         the problem is described well here:
+         https://community.plotly.com/t/set-pca-loadings-aka-arrows-in-a-3d-scatter-plot/72905
+
+        Returns:
+            a plotly GraphObjects.Figure
+
+        """
+        label: str = 'std' if standardised else 'raw'
+        pca_data: pd.DataFrame = self.data[label].data
+        pca_loadings: pd.DataFrame = self.data[label].loadings
+        pca_variance: pd.DataFrame = self.data[label].explained_variance
+
+        df_plot: pd.DataFrame = pd.concat([pca_data, self.x], axis=1).reset_index()
+        if plot_3d:
+            fig = px.scatter_3d(df_plot, x='PC1', y='PC2', z='PC3',
+                                color=self.color, hover_data=list(self.x.reset_index().columns))
+            fig.update_traces(marker_size=4)
+            if loading_vectors:
+
+                annots: List = [dict(x=row.PC1, y=row.PC2, z=row.PC3,
+                                     text=i, showarrow=False,
+                                     xanchor="left", xshift=10, yshift=10, opacity=0.7) for i, row in
+                                pca_loadings.iterrows()]
+                fig.update_layout(scene=dict(annotations=annots))
+                for feature_name, row in pca_loadings.iterrows():
+                    # noinspection PyTypeChecker
+                    fig.add_trace(
+                        go.Scatter3d(x=(row.PC1,), y=(row.PC2,), z=(row.PC3,), mode='markers',
+                                     marker={'size': 6, 'line': dict(width=2, color='black')},
+                                     name=feature_name,
+                                     showlegend=True,
+                                     legendgroup="features",
+                                     legendgrouptitle_text="feature vectors",
+                                     ))
+                    fig.add_trace(
+                        go.Scatter3d(x=(0, row.PC1), y=(0, row.PC2), z=(0, row.PC3), mode='lines',
+                                     line={'width': 5, 'color': 'black'},
+                                     name=feature_name,
+                                     showlegend=False))
+                fig.update_layout(legend=dict(groupclick="toggleitem"))
+                title = (f"Top 3 Principal Components<br>Explained Variance = "
+                         f"{round(pca_variance.iloc[0:3].sum(), 1)}%") if title is None else title
+        else:  # 2D
+            fig = px.scatter(df_plot, x='PC1', y='PC2',
+                             color=self.color, hover_data=list(self.x.reset_index().columns))
+            fig.update_traces(marker_size=5)
+
+            if loading_vectors:
+                loadings = pca_loadings.iloc[:, 0:2]
+                self.add_loading_vectors(fig, loadings)
+            title = (f"Top 2 Principal Components<br>Explained Variance = "
+                     f"{round(pca_variance.iloc[0:2].sum(), 1)}%") if title is None else title
+
+        fig.update_layout(legend_title_text=self.color.name)
+        fig.update_layout(title=title,
+                          xaxis_title=f"PC1 ({round(self.data['std'].explained_variance.iloc[0], 1)}%)",
+                          yaxis_title=f"PC2 ({round(self.data['std'].explained_variance.iloc[1], 1)}%)")
+        if self.color is not None:
+            fig.update_layout(coloraxis_colorbar_title_text=self.color.name)
+
+        return fig
+
+    def plot_explained_variance(self,
+                                standardised: bool = False,
+                                title: Optional[str] = None) -> go.Figure:
+        """Plot the cumulative explained variance by principal component.
+
+        Args:
+            standardised: If True, plot the standardised PCA, where vectors are transformed to zero mean and
+             unit variance.
+            title: Optional plot title
+
+        Returns:
+
+        """
+        pca_variance: pd.DataFrame = self.data['std'].explained_variance if standardised else self.data[
+            'raw'].explained_variance
+        exp_var_cumul = np.cumsum(pca_variance)
+        fig = px.area(
+            x=range(1, exp_var_cumul.shape[0] + 1),
+            y=exp_var_cumul,
+            labels={"x": "# Components", "y": "Explained Variance"}
+        )
+        title = 'Cumulative Explained Variance by Principal Component' if title is None else title
+        fig.update_layout(title=title)
+        fig.update_xaxes(type='category')
+
+        return fig
+
+    def plot_scatter_matrix(self, original_features: bool = False, standardised: bool = False,
+                            title: Optional[str] = None) -> go.Figure:
+        """Plot a scatter matrix
+
+        Args:
+            original_features: If True, plot the original features, otherwise plot the principal components.
+            standardised: If True, plot the standardised PCA, where vectors are transformed to zero mean and
+             unit variance.
+            title: Optional plot title
+
+        Returns:
+
+        """
+        label: str = 'std' if standardised else 'raw'
+        y = self.color
+        if original_features:
+            x = self.x
+            title = 'Scatter Matrix - Original Feature Space' if title is None else title
+        else:
+            x = self.data[label].data
+            title = 'Scatter Matrix - All Principal Components' if title is None else title
+
+        if original_features:
+            df_plot: pd.DataFrame = pd.concat([x, y], axis=1).reset_index()
+            hover_data = ['index' if x.index.name is None else x.index.name]
+        else:
+            df_plot: pd.DataFrame = pd.concat([x, y, self.x], axis=1).reset_index()
+            hover_data = list(self.x.reset_index().columns)
+
+        fig = px.scatter_matrix(data_frame=df_plot, dimensions=list(x.columns),
+                                color=y.name, hover_data=hover_data)
+        fig.update_traces(diagonal_visible=False)
+        title = 'Top 3 Principal Components' if title is None else title
+        fig.update_layout(title=title)
+
+        return fig
+
+    def plot_loading_vectors(self, standardised: bool = False, by_color: bool = False,
+                             title: Optional[str] = None) -> go.Figure:
+        """plot the loading vectors.
+
+        Args:
+            standardised: If True, plot the standardised PCA, where vectors are transformed to zero mean and
+             unit variance.
+             by_color: If True, plot the loading vectors by color group.
+            title: Optional plot title
+
+        Returns:
+            a plotly GraphObjects.Figure
+
+        """
+        label: str = 'std' if standardised else 'raw'
+        if by_color:
+            chunks = []
+
+            for grp, d_label in self.data['group'].items():
+                chunks.append(self.data['group'][grp][label].loadings.assign(group=grp))
+            loadings = pd.concat(chunks, axis='index')
+            fig = px.scatter(loadings, x='PC1', y='PC2', color='group',
+                             hover_data=loadings.columns.tolist())
+
+        else:
+            loadings = self.data[label].loadings.iloc[:, 0:2]
+            fig = px.scatter(loadings, x='PC1', y='PC2', hover_data=loadings.columns.tolist())
+        fig.update_traces(marker=dict(size=1))
+
+        if standardised:
+            fig.add_shape(type="circle",
+                          xref="x", yref="y",
+                          x0=-1, y0=-1, x1=1, y1=1,
+                          line_color="gray")
+            title_main = "Correlation Circle"
+        else:
+            title_main = "Top 2 Principal Components"
+
+        fig = self.add_loading_vectors(fig, loadings)
+        title = (f"{title_main}<br>Explained Variance = "
+                 f"{round(self.data['std'].explained_variance.iloc[0:2].sum(), 1)}%") if title is None else title
+
+        fig.update_layout(title=title,
+                          xaxis_title=f"PC1 ({round(self.data['std'].explained_variance.iloc[0], 1)}%)",
+                          yaxis_title=f"PC2 ({round(self.data['std'].explained_variance.iloc[1], 1)}%)")
+        fig.update_yaxes(scaleanchor="x", scaleratio=1)
+        fig.update_layout(scene=dict(aspectmode="data"))
+
+        return fig
+
+    def add_loading_vectors(self, fig, loadings) -> go.Figure:
+        if 'group' in loadings.columns:
+            cm = px.colors.qualitative.Plotly
+            grp_colors = dict(zip(loadings['group'].unique(), cm[0:len(loadings['group'].unique())]))
+        for i, feature in enumerate(loadings.index):
+            if 'group' in loadings.columns:
+                grp = loadings.iloc[i, :]['group']
+                arrowcolor = grp_colors[grp]
+                font = dict(color=grp_colors[grp])
+            else:
+                arrowcolor = None
+                font = None
+            fig.add_annotation(
+                ax=0, ay=0,
+                axref="x", ayref="y",
+                x=loadings.iloc[i, 0],
+                y=loadings.iloc[i, 1],
+                showarrow=True,
+                arrowsize=2,
+                arrowhead=2,
+                xanchor="right",
+                yanchor="top",
+                arrowcolor=arrowcolor,
+            )
+            fig.add_annotation(
+                x=loadings.iloc[i, 0],
+                y=loadings.iloc[i, 1],
+                ax=0, ay=0,
+                xanchor="center",
+                yanchor="bottom",
+                text=feature,
+                yshift=5,
+                font=font
+            )
+        return fig
```

### Comparing `sklearn_viz-0.4.2/elphick/sklearn_viz/features/scatter_matrix.py` & `sklearn_viz-0.4.9/elphick/sklearn_viz/features/scatter_matrix.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from typing import Optional
-
-import pandas as pd
-import plotly.graph_objects as go
-import plotly.express as px
-
-
-def plot_scatter_matrix(x: pd.DataFrame, color: Optional[str] = None, title: Optional[str] = None) -> go.Figure:
-    """Plot a scatter matrix
-
-    Args:
-        x: X values to transform and plot.
-        color: optional target vector
-        title: Optional plot title
-
-    Returns:
-
-    """
-
-    fig = px.scatter_matrix(data_frame=x, dimensions=list(x.columns), color=color)
-    fig.update_traces(diagonal_visible=False)
-    title = 'Scatter Matrix' if title is None else title
-    fig.update_layout(title=title)
-
-    return fig
+from typing import Optional
+
+import pandas as pd
+import plotly.graph_objects as go
+import plotly.express as px
+
+
+def plot_scatter_matrix(x: pd.DataFrame, color: Optional[str] = None, title: Optional[str] = None) -> go.Figure:
+    """Plot a scatter matrix
+
+    Args:
+        x: X values to transform and plot.
+        color: optional target vector
+        title: Optional plot title
+
+    Returns:
+
+    """
+
+    fig = px.scatter_matrix(data_frame=x, dimensions=list(x.columns), color=color)
+    fig.update_traces(diagonal_visible=False)
+    title = 'Scatter Matrix' if title is None else title
+    fig.update_layout(title=title)
+
+    return fig
```

### Comparing `sklearn_viz-0.4.2/elphick/sklearn_viz/model_selection/learning_curve.py` & `sklearn_viz-0.4.9/elphick/sklearn_viz/model_selection/learning_curve.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,167 +1,167 @@
-import logging
-from typing import Union, Optional, Iterable, Any
-
-import matplotlib
-import numpy as np
-import pandas as pd
-import plotly.graph_objects as go
-from sklearn.base import is_classifier, is_regressor
-from sklearn.model_selection import learning_curve
-from sklearn.pipeline import Pipeline
-
-from elphick.sklearn_viz.utils import log_timer
-
-
-def plot_learning_curve(mdl,
-                        x: pd.DataFrame,
-                        y: Union[pd.DataFrame, pd.Series],
-                        cv: Union[int, Any] = 5,
-                        title: Optional[str] = None) -> go.Figure:
-    """
-
-    Args:
-        mdl: The scikit-learn model or pipeline.
-        x: X values provided to calculate the learning curve.
-        y: y values provided to calculate the learning curve.
-        cv: The number of cross validation folds or cv callable.
-        title: Optional plot title
-
-    Returns:
-        a plotly GraphObjects.Figure
-
-    """
-
-    return LearningCurve(mdl=mdl, x=x, y=y, cv=cv).plot(title=title)
-
-
-class LearningCurve:
-    def __init__(self,
-                 mdl,
-                 x: pd.DataFrame,
-                 y: Union[pd.DataFrame, pd.Series],
-                 train_sizes: Iterable = np.linspace(0.1, 1.0, 5),
-                 cv: Union[int, Any] = 5):
-        """
-
-        Args:
-            mdl: The scikit-learn model or pipeline.
-            x: X values provided to calculate the learning curve.
-            y: y values provided to calculate the learning curve.
-            train_sizes: list of training sample counts (or fractions if < 1)
-            cv: The number of cross validation folds or a cv callable.
-        """
-        self._logger = logging.getLogger(name=__class__.__name__)
-        self.mdl = mdl
-        self.X: Optional[pd.DataFrame] = x
-        self.y: Optional[Union[pd.DataFrame, pd.Series]] = y
-        self.train_sizes: Iterable = train_sizes
-        self.cv: int = cv
-        self._data: Optional[pd.DataFrame] = None
-        self.is_pipeline: bool = isinstance(mdl, Pipeline)
-        self.is_classifier: bool = is_classifier(mdl)
-        self.is_regressor: bool = is_regressor(mdl)
-        self.scorer = None
-
-        # check_is_fitted(mdl[-1]) if self.is_pipeline else check_is_fitted(mdl)
-
-    @property
-    @log_timer
-    def data(self) -> Optional[pd.DataFrame]:
-        if self._data is not None:
-            res = self._data
-        else:
-
-            if self.is_regressor:
-                self.scorer = 'neg_mean_squared_error'
-            elif self.is_classifier:
-                self.scorer = 'accuracy'
-            else:
-                raise NotImplementedError("Only Classifers and Regressors are supported.")
-
-            self._logger.info("Commencing Cross Validation")
-            train_size_abs, train_scores, val_scores = learning_curve(self.mdl, X=self.X, y=self.y,
-                                                                      train_sizes=self.train_sizes)
-            col_names = [f"train_count_{n}" for n in train_size_abs]
-            train: pd.DataFrame = pd.DataFrame(train_scores.T, columns=col_names).assign(dataset='training')
-            val: pd.DataFrame = pd.DataFrame(val_scores.T, columns=col_names).assign(dataset='validation')
-            res: pd.DataFrame = pd.concat([train, val], axis='index').reset_index(drop=True)
-
-            self._data = res
-
-        return res
-
-    def plot(self,
-             sort: bool = False,
-             title: Optional[str] = None) -> go.Figure:
-        """Create the plot
-
-        KUDOS: https://towardsdatascience.com/applying-a-custom-colormap-with-plotly-boxplots-5d3acf59e193
-
-        Args:
-            sort: If True, sort by decreasing importance
-            title: title for the plot
-
-        Returns:
-            a plotly GraphObjects.Figure
-
-        """
-        data_train = self.data.query('dataset=="training"').drop(columns=['dataset'])
-        data_val = self.data.query('dataset=="validation"').drop(columns=['dataset'])
-
-        subtitle: str = f'Cross Validation: {self.cv}'
-        if title is None:
-            title = subtitle
-        else:
-            title = title + '<br>' + subtitle
-
-        if sort:
-            pass
-
-        fig = go.Figure()
-        x = [int(col.split('_')[-1]) for col in data_train.columns]
-        y_train = list(data_train.mean())
-        train_sd = list(data_train.std())
-        y_val = list(data_val.mean())
-        val_sd = list(data_val.std())
-        y_train_upper = list(data_train.mean() + train_sd)
-        y_train_lower = list(data_train.mean() - train_sd)
-        y_val_upper = list(data_val.mean() + val_sd)
-        y_val_lower = list(data_val.mean() - val_sd)
-
-        fig.add_trace(go.Scatter(
-            x=x,
-            y=y_train,
-            line=dict(color='royalblue'),
-            mode='lines',
-            name='training',
-        ))
-        fig.add_trace(go.Scatter(
-            x=x,
-            y=y_val,
-            line=dict(color='orange'),
-            mode='lines',
-            name='validation',
-        ))
-        fig.add_trace(go.Scatter(
-            x=x + x[::-1],  # x, then x reversed
-            y=y_train_upper + y_train_lower[::-1],  # upper, then lower reversed
-            fill='toself',
-            fillcolor=f"rgba{str(matplotlib.colors.to_rgba('royalblue', 0.4))}",
-            line=dict(color='rgba(255,255,255,0)'),
-            hoverinfo="skip",
-            name='training error +/- 1SD'
-        ))
-        fig.add_trace(go.Scatter(
-            x=x + x[::-1],  # x, then x reversed
-            y=y_val_upper + y_val_lower[::-1],  # upper, then lower reversed
-            fill='toself',
-            # fillcolor=f"rgba{str(matplotlib.colors.to_rgba('orange', 0.5))}",
-            fillcolor="rgba(255, 165, 0, 0.5)",
-            line=dict(color='rgba(255,255,255,0)'),
-            hoverinfo="skip",
-            showlegend=True,
-            name='validation error +/- 1SD'
-        ))
-        fig.update_layout(title=title, showlegend=True, yaxis_title=self.scorer,
-                          xaxis_title='Number of samples in the training set')
-        return fig
+import logging
+from typing import Union, Optional, Iterable, Any
+
+import matplotlib
+import numpy as np
+import pandas as pd
+import plotly.graph_objects as go
+from sklearn.base import is_classifier, is_regressor
+from sklearn.model_selection import learning_curve
+from sklearn.pipeline import Pipeline
+
+from elphick.sklearn_viz.utils import log_timer
+
+
+def plot_learning_curve(mdl,
+                        x: pd.DataFrame,
+                        y: Union[pd.DataFrame, pd.Series],
+                        cv: Union[int, Any] = 5,
+                        title: Optional[str] = None) -> go.Figure:
+    """
+
+    Args:
+        mdl: The scikit-learn model or pipeline.
+        x: X values provided to calculate the learning curve.
+        y: y values provided to calculate the learning curve.
+        cv: The number of cross validation folds or cv callable.
+        title: Optional plot title
+
+    Returns:
+        a plotly GraphObjects.Figure
+
+    """
+
+    return LearningCurve(mdl=mdl, x=x, y=y, cv=cv).plot(title=title)
+
+
+class LearningCurve:
+    def __init__(self,
+                 mdl,
+                 x: pd.DataFrame,
+                 y: Union[pd.DataFrame, pd.Series],
+                 train_sizes: Iterable = np.linspace(0.1, 1.0, 5),
+                 cv: Union[int, Any] = 5):
+        """
+
+        Args:
+            mdl: The scikit-learn model or pipeline.
+            x: X values provided to calculate the learning curve.
+            y: y values provided to calculate the learning curve.
+            train_sizes: list of training sample counts (or fractions if < 1)
+            cv: The number of cross validation folds or a cv callable.
+        """
+        self._logger = logging.getLogger(name=__class__.__name__)
+        self.mdl = mdl
+        self.X: Optional[pd.DataFrame] = x
+        self.y: Optional[Union[pd.DataFrame, pd.Series]] = y
+        self.train_sizes: Iterable = train_sizes
+        self.cv: int = cv
+        self._data: Optional[pd.DataFrame] = None
+        self.is_pipeline: bool = isinstance(mdl, Pipeline)
+        self.is_classifier: bool = is_classifier(mdl)
+        self.is_regressor: bool = is_regressor(mdl)
+        self.scorer = None
+
+        # check_is_fitted(mdl[-1]) if self.is_pipeline else check_is_fitted(mdl)
+
+    @property
+    @log_timer
+    def data(self) -> Optional[pd.DataFrame]:
+        if self._data is not None:
+            res = self._data
+        else:
+
+            if self.is_regressor:
+                self.scorer = 'neg_mean_squared_error'
+            elif self.is_classifier:
+                self.scorer = 'accuracy'
+            else:
+                raise NotImplementedError("Only Classifers and Regressors are supported.")
+
+            self._logger.info("Commencing Cross Validation")
+            train_size_abs, train_scores, val_scores = learning_curve(self.mdl, X=self.X, y=self.y,
+                                                                      train_sizes=self.train_sizes)
+            col_names = [f"train_count_{n}" for n in train_size_abs]
+            train: pd.DataFrame = pd.DataFrame(train_scores.T, columns=col_names).assign(dataset='training')
+            val: pd.DataFrame = pd.DataFrame(val_scores.T, columns=col_names).assign(dataset='validation')
+            res: pd.DataFrame = pd.concat([train, val], axis='index').reset_index(drop=True)
+
+            self._data = res
+
+        return res
+
+    def plot(self,
+             sort: bool = False,
+             title: Optional[str] = None) -> go.Figure:
+        """Create the plot
+
+        KUDOS: https://towardsdatascience.com/applying-a-custom-colormap-with-plotly-boxplots-5d3acf59e193
+
+        Args:
+            sort: If True, sort by decreasing importance
+            title: title for the plot
+
+        Returns:
+            a plotly GraphObjects.Figure
+
+        """
+        data_train = self.data.query('dataset=="training"').drop(columns=['dataset'])
+        data_val = self.data.query('dataset=="validation"').drop(columns=['dataset'])
+
+        subtitle: str = f'Cross Validation: {self.cv}'
+        if title is None:
+            title = subtitle
+        else:
+            title = title + '<br>' + subtitle
+
+        if sort:
+            pass
+
+        fig = go.Figure()
+        x = [int(col.split('_')[-1]) for col in data_train.columns]
+        y_train = list(data_train.mean())
+        train_sd = list(data_train.std())
+        y_val = list(data_val.mean())
+        val_sd = list(data_val.std())
+        y_train_upper = list(data_train.mean() + train_sd)
+        y_train_lower = list(data_train.mean() - train_sd)
+        y_val_upper = list(data_val.mean() + val_sd)
+        y_val_lower = list(data_val.mean() - val_sd)
+
+        fig.add_trace(go.Scatter(
+            x=x,
+            y=y_train,
+            line=dict(color='royalblue'),
+            mode='lines',
+            name='training',
+        ))
+        fig.add_trace(go.Scatter(
+            x=x,
+            y=y_val,
+            line=dict(color='orange'),
+            mode='lines',
+            name='validation',
+        ))
+        fig.add_trace(go.Scatter(
+            x=x + x[::-1],  # x, then x reversed
+            y=y_train_upper + y_train_lower[::-1],  # upper, then lower reversed
+            fill='toself',
+            fillcolor=f"rgba{str(matplotlib.colors.to_rgba('royalblue', 0.4))}",
+            line=dict(color='rgba(255,255,255,0)'),
+            hoverinfo="skip",
+            name='training error +/- 1SD'
+        ))
+        fig.add_trace(go.Scatter(
+            x=x + x[::-1],  # x, then x reversed
+            y=y_val_upper + y_val_lower[::-1],  # upper, then lower reversed
+            fill='toself',
+            # fillcolor=f"rgba{str(matplotlib.colors.to_rgba('orange', 0.5))}",
+            fillcolor="rgba(255, 165, 0, 0.5)",
+            line=dict(color='rgba(255,255,255,0)'),
+            hoverinfo="skip",
+            showlegend=True,
+            name='validation error +/- 1SD'
+        ))
+        fig.update_layout(title=title, showlegend=True, yaxis_title=self.scorer,
+                          xaxis_title='Number of samples in the training set')
+        return fig
```

### Comparing `sklearn_viz-0.4.2/elphick/sklearn_viz/model_selection/metrics.py` & `sklearn_viz-0.4.9/elphick/sklearn_viz/model_selection/metrics.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-from functools import partial
-from typing import Literal
-
-import numpy as np
-from sklearn.metrics import r2_score, mean_absolute_error, mean_squared_error, f1_score
-
-
-def mean_error(y_true, y_est) -> float:
-    return float(np.mean(y_est - y_true))
-
-
-def moe_95(y_true, y_est, metric: Literal["moe", "lo", "hi"] = 'moe') -> float:
-    me = mean_error(y_true, y_est)
-    rmse = mean_squared_error(y_true, y_est, squared=False)
-    if metric == 'lo':
-        res = me - (rmse * 1.96)
-    elif metric == 'hi':
-        res = me + (rmse * 1.96)
-    elif metric == 'moe':
-        res = np.mean([(np.abs(me - (rmse * 1.96))), (me + (rmse * 1.96))])
-    else:
-        raise KeyError(f'Invalid metric supplied.  Allowed values are: {Literal["moe", "lo", "hi"]}')
-    return res
-
-
-def r2(y_true, y_est):
-    ssr = ((y_true - y_est) ** 2).sum()
-    sst = ((y_true - y_true.mean()) ** 2).sum()
-    return 1 - (ssr / sst)
-
-
-def r2_with_nan(y_true, y_est):
-    numerator = np.nansum((y_true - y_est) ** 2, axis=0, dtype=np.float64)
-    denominator = np.nansum((y_true - np.nanmean(y_true, axis=0)) ** 2, axis=0, dtype=np.float64)
-    return np.mean(1 - numerator / denominator)
-
-
-regression_metrics = {
-    # 'r2_nan': r2_with_nan,
-    'r2_score': r2_score,
-    'me': mean_error,
-    'r2': r2,
-    'mae': mean_absolute_error,
-    'mse': mean_squared_error,
-    'rmse': partial(mean_squared_error, squared=False),
-    'moe': partial(moe_95, metric='moe'),
-    'moe_lo': partial(moe_95, metric='lo'),
-    'moe_hi': partial(moe_95, metric='hi')}
-
-classification_metrics = {'f1': f1_score}
+from functools import partial
+from typing import Literal
+
+import numpy as np
+from sklearn.metrics import r2_score, mean_absolute_error, mean_squared_error, f1_score
+
+
+def mean_error(y_true, y_est) -> float:
+    return float(np.mean(y_est - y_true))
+
+
+def moe_95(y_true, y_est, metric: Literal["moe", "lo", "hi"] = 'moe') -> float:
+    me = mean_error(y_true, y_est)
+    rmse = mean_squared_error(y_true, y_est, squared=False)
+    if metric == 'lo':
+        res = me - (rmse * 1.96)
+    elif metric == 'hi':
+        res = me + (rmse * 1.96)
+    elif metric == 'moe':
+        res = np.mean([(np.abs(me - (rmse * 1.96))), (me + (rmse * 1.96))])
+    else:
+        raise KeyError(f'Invalid metric supplied.  Allowed values are: {Literal["moe", "lo", "hi"]}')
+    return res
+
+
+def r2(y_true, y_est):
+    ssr = ((y_true - y_est) ** 2).sum()
+    sst = ((y_true - y_true.mean()) ** 2).sum()
+    return 1 - (ssr / sst)
+
+
+def r2_with_nan(y_true, y_est):
+    numerator = np.nansum((y_true - y_est) ** 2, axis=0, dtype=np.float64)
+    denominator = np.nansum((y_true - np.nanmean(y_true, axis=0)) ** 2, axis=0, dtype=np.float64)
+    return np.mean(1 - numerator / denominator)
+
+
+regression_metrics = {
+    # 'r2_nan': r2_with_nan,
+    'r2_score': r2_score,
+    'me': mean_error,
+    'r2': r2,
+    'mae': mean_absolute_error,
+    'mse': mean_squared_error,
+    'rmse': partial(mean_squared_error, squared=False),
+    'moe': partial(moe_95, metric='moe'),
+    'moe_lo': partial(moe_95, metric='lo'),
+    'moe_hi': partial(moe_95, metric='hi')}
+
+classification_metrics = {'f1': f1_score}
```

### Comparing `sklearn_viz-0.4.2/elphick/sklearn_viz/model_selection/model_selection.py` & `sklearn_viz-0.4.9/elphick/sklearn_viz/model_selection/model_selection.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,421 +1,421 @@
-import logging
-from typing import Union, Optional, Dict, List, Callable, Tuple
-
-import matplotlib
-import numpy as np
-import pandas as pd
-import plotly.graph_objects as go
-import sklearn
-from plotly import colors
-from plotly.subplots import make_subplots
-from sklearn import model_selection
-from sklearn.base import is_classifier, is_regressor
-from sklearn.model_selection import cross_validate
-from sklearn.pipeline import Pipeline
-
-from elphick.sklearn_viz.model_selection.metrics import regression_metrics, classification_metrics
-from elphick.sklearn_viz.model_selection.scorers import classification_scorers, regression_scorers
-
-
-def subplot_index(idx: int, col_wrap: int) -> Tuple[int, int]:
-    col: int = int(idx % col_wrap + 1)
-    row: int = int(np.floor(idx / col_wrap) + 1)
-    return row, col
-
-
-def plot_model_selection(algorithms: Union[sklearn.base.RegressorMixin, sklearn.base.ClassifierMixin, Dict],
-                         datasets: Union[pd.DataFrame, Dict],
-                         target: str,
-                         pre_processor: Optional[Pipeline] = None,
-                         k_folds: int = 10,
-                         title: Optional[str] = None) -> go.Figure:
-    """
-
-    Args:
-            algorithms: sklearn estimator or a Dict of algorithms to cross-validate, keyed by string name/code.
-            datasets: pandas DataFrame or a dict of DataFrames, keyed by string name/code.
-            target: target column
-            pre_processor: Optional pipeline used to pre-process the datasets.
-            k_folds: The number of cross validation folds.
-            title: Optional plot title
-
-    Returns:
-        a plotly GraphObjects.Figure
-
-    """
-
-    return ModelSelection(algorithms=algorithms, datasets=datasets, target=target, pre_processor=pre_processor,
-                          k_folds=k_folds).plot(title=title)
-
-
-class ModelSelection:
-    def __init__(self,
-                 algorithms: Union[
-                     sklearn.base.RegressorMixin, sklearn.base.ClassifierMixin, Dict[str, sklearn.base.BaseEstimator]],
-                 datasets: Union[pd.DataFrame, Dict[str, pd.DataFrame]],
-                 target: str,
-                 pre_processor: Optional[Pipeline] = None,
-                 k_folds: int = 10,
-                 scorer: Optional[Union[str, Callable]] = None,
-                 metrics: Optional[Dict[str, Callable]] = None,
-                 group: Optional[pd.Series] = None,
-                 random_state: Optional[int] = None):
-        """
-
-        Args:
-            algorithms: sklearn estimator or a Dict of algorithms to cross-validate, keyed by string name/code.
-            datasets: pandas DataFrame or a dict of DataFrames, keyed by string name/code.
-            target: target column
-            pre_processor: Optional pipeline used to pre-process the datasets.
-            k_folds: The number of cross validation folds.
-            scorer: Optional callable scorers which the model will be fitted using
-            metrics: Optional Dict of callable metrics to calculate post-fitting
-            group: Optional group variable by which to partition/group metrics.  The same group applies across all
-             datasets, so is more useful when testing different algorithms.
-            random_state: Optional random seed
-        """
-        self._logger = logging.getLogger(name=__class__.__name__)
-        self.pre_processor: Pipeline = pre_processor
-        if isinstance(algorithms, sklearn.base.BaseEstimator):
-            self.algorithms = {algorithms.__class__.__name__: algorithms}
-        else:
-            self.algorithms = algorithms
-        if isinstance(datasets, pd.DataFrame):
-            self.datasets = {'Dataset': datasets}
-        else:
-            self.datasets = datasets
-        self.target = target
-        self.k_folds: int = k_folds
-
-        self.is_classifier: bool = is_classifier(list(self.algorithms.values())[0])
-        self.is_regressor: bool = is_regressor(list(self.algorithms.values())[0])
-        if scorer is not None:
-            self.scorer = scorer
-        else:
-            self.scorer = classification_scorers[list(classification_scorers.keys())[0]] if self.is_classifier else \
-                regression_scorers[list(regression_scorers.keys())[0]]
-
-        if metrics is not None:
-            self.metrics = metrics
-        else:
-            self.metrics = classification_metrics if self.is_classifier else regression_metrics
-
-        self.group: pd.Series = group
-        self.random_state: Optional[int] = random_state
-
-        self.features_in: List[str] = [col for col in self.datasets[list(self.datasets.keys())[0]] if
-                                       col != self.target]
-
-        self._data: Optional[Dict] = None
-        self._num_algorithms: int = len(list(self.algorithms.keys()))
-        self._num_datasets: int = len(list(self.datasets.keys()))
-
-        if self._num_algorithms > 1 and self._num_datasets > 1:
-            raise NotImplementedError("Cannot have multiple algorithms and multiple datasets.")
-
-    @property
-    def data(self) -> Optional[Dict]:
-        if self.metrics is None:
-            cv_kwargs: Dict = dict()
-        else:
-            cv_kwargs: Dict = dict(return_estimator=True, return_indices=True, error_score=np.nan)
-
-        if self._data is not None:
-            results = self._data
-        else:
-            results: Dict = {}
-            for data_key, data in self.datasets.items():
-                self._logger.info(f"Commencing Cross Validation for dataset {data_key}")
-                results[data_key] = {}
-                x: pd.DataFrame = data[self.features_in]
-                y: pd.DataFrame = data[self.target]
-                if self.pre_processor:
-                    x = self.pre_processor.set_output(transform="pandas").fit_transform(X=x)
-
-                for algo_key, algo in self.algorithms.items():
-                    kfold = model_selection.KFold(n_splits=self.k_folds, random_state=self.random_state, shuffle=True)
-                    res = cross_validate(algo, x, y, cv=kfold, scoring=self.scorer, **cv_kwargs)
-                    if self.metrics is not None:
-                        res['metrics'], res['metrics_group'] = self.calculate_metrics(x=x, y=y,
-                                                                                      estimators=res['estimator'],
-                                                                                      indices=res['indices'],
-                                                                                      group=self.group)
-                    results[data_key][algo_key] = res
-                    res_mean = res[f"test_score"].mean()
-                    res_std = res[f"test_score"].std()
-                    self._logger.info(f"CV Results for {algo_key}: Mean = {res_mean}, SD = {res_std}")
-
-            self._data = results
-
-        return results
-
-    def plot(self,
-             metrics: Optional[Union[str, List[str]]] = None,
-             show_group: bool = False,
-             title: Optional[str] = None,
-             col_wrap: Optional[int] = None) -> go.Figure:
-        """Create the plot
-
-        The plot will show the cross-validation scores for each algorithm and dataset.  The first panel is used to show
-        the scorer, that is the metric used to fit the model.  If multiple metrics are supplied, each metric will be
-        shown in a separate panel.  If a show_group is true, the metrics will be grouped by the group variable.
-        col_wrap allows the width of the plot to be controlled by wrapping the columns to new rows.
-
-        KUDOS: https://towardsdatascience.com/applying-a-custom-colormap-with-plotly-boxplots-5d3acf59e193
-
-        Args:
-            metrics: The metric or metrics to plot in addition to the scorer.  Each metric will be plotted in a
-             separate panel.
-            show_group: If True (and a group variable has been set), plot by group.
-            title: Title of the plot
-            col_wrap: If plotting multiple metrics, col_wrap will wrap columns to new rows, resulting in
-             col-wrap columns, and multiple rows.
-
-        Returns:
-            a plotly GraphObjects.Figure
-
-        """
-
-        data: pd.DataFrame = self.get_cv_scores()
-        data = data.droplevel(level=0, axis=1) if self._num_datasets == 1 else data.droplevel(level=1, axis=1)
-
-        metric_data: pd.DataFrame = pd.DataFrame()
-
-        if metrics is not None:
-            if isinstance(metrics, str):
-                metrics = [metrics]
-            metric_data = self.get_cv_metrics(metrics, show_group)
-        else:
-            metrics = []
-
-        if self._num_algorithms > 1:
-            x_index = 'algo_key'
-        else:
-            x_index = 'data_key'
-
-        # define the color map for the scorer
-        vmin, vmax = data.min().min(), data.max().max()
-        norm = matplotlib.colors.Normalize(vmin=vmin, vmax=vmax)
-        cmap = matplotlib.cm.get_cmap('RdYlGn')
-
-        subtitle: str = f'Cross Validation folds={self.k_folds}'
-        if title is None:
-            title = subtitle
-        else:
-            title = title + '<br>' + subtitle
-
-        # create the plot, managing the shape.
-        num_plots: int = len(metrics) + 1 if len(metrics) > 0 else 1
-        num_cols: int = num_plots if col_wrap is None else col_wrap
-        num_rows, _ = subplot_index(len(metrics), col_wrap=num_cols)
-        fig = make_subplots(rows=num_rows, cols=num_cols, subplot_titles=[f'{self.scorer} (scorer)'] + metrics)
-
-        # Add the scorer subplot
-        for col in data.columns:
-            # For the scorer build the plot by column to color individually based on score
-            median = np.median(data[col])  # find the median
-            color = 'rgb' + str(cmap(norm(median))[0:3])  # normalize
-            fig.add_trace(go.Box(y=data[col], name=col, boxpoints='all', notched=True, fillcolor=color,
-                                 line={"color": "grey"}, marker={"color": "grey"}, showlegend=False,
-                                 offsetgroup='A'), row=1, col=1)
-
-        # add the metric subplots
-        for i, metric in enumerate(metrics):
-            row, col = subplot_index(i + 1, col_wrap=num_cols)
-            if show_group:
-                colorscale = colors.qualitative.Plotly + colors.qualitative.Dark24
-                add_to_legend = True if i == 0 else False
-                df_metric: pd.DataFrame = metric_data.query('metric==@metric').drop(columns=['metric'])
-                x = df_metric.index.get_level_values(x_index)
-                for g, grp in enumerate(df_metric.columns):
-                    if len(df_metric.columns) > len(colorscale):
-                        raise ValueError("Too many groups to plot")
-                    fig.add_trace(go.Box(x=x, y=df_metric[grp], name=grp, boxpoints='all', notched=True,
-                                         legendgroup=self.group.name,
-                                         showlegend=add_to_legend,
-                                         line={"color": colorscale[g]}, marker={"color": colorscale[g]},
-                                         offsetgroup=str(g)), row=row, col=col)
-            else:
-                df_metric: pd.DataFrame = metric_data.query('metric==@metric').drop(columns=['metric'])
-                x = list(df_metric.index.get_level_values(x_index))
-                fig.add_trace(go.Box(x=x, y=df_metric.values.ravel(), name=metric, boxpoints='all', notched=True,
-                                     line={"color": "grey"}, marker={"color": "grey"}), row=row, col=col)
-
-        # finalise some display elements
-        fig.update_layout(title=title, showlegend=False)
-        if show_group:
-            fig.update_layout(boxmode='group', showlegend=True, legend_title=self.group.name,
-                              boxgroupgap=0.5, boxgap=0
-                              )
-
-        return fig
-
-    def plot_category_analysis(self,
-                               algorithm: Optional[str] = None,
-                               dataset: Optional[str] = None,
-                               metrics: Optional[Union[str, List[str]]] = None,
-                               title: Optional[str] = None,
-                               col_wrap: Optional[int] = None) -> go.Figure:
-        """Plot the category feature analysis
-
-        Args:
-            algorithm: If supplied, this will be the name of the algorithm tested.  If None the first algorithm is used.
-            dataset: If supplied, this will be the name of the dataset tested.  If None the first dataset is used.
-            metrics: The metric or metrics to show.  Each metric will be plotted in a
-             separate panel.
-            title: Title of the plot
-            col_wrap: If plotting multiple metrics, col_wrap will wrap columns to new rows, resulting in
-             col-wrap columns, and multiple rows.
-
-        Returns:
-            a plotly GraphObjects.Figure
-
-        """
-        algorithms: list[str] = list(self.algorithms.keys())
-        algorithm: str = algorithms[0] if algorithm is None else algorithm
-        if algorithm not in algorithms:
-            raise KeyError(f"Algorithm {algorithm} is not in the list of available algorithms: {algorithms}")
-
-        datasets: list[str] = list(self.datasets.keys())
-        dataset: str = datasets[0] if dataset is None else dataset
-        if dataset not in datasets:
-            raise KeyError(f"Dataset {dataset} is not in the list of available datasets: {datasets}")
-
-        metrics: list[str] = [list(self.metrics.keys())[0]] if metrics is None else metrics
-
-        baseline_metrics: pd.DataFrame = self.get_cv_metrics(metrics, by_group=True).loc[
-            (slice(None), dataset, algorithm)]
-        baseline_metrics = baseline_metrics.melt(id_vars=['metric'], value_vars=self.group.unique().tolist(),
-                                                 var_name='group',
-                                                 ignore_index=False).assign(model='baseline')
-
-        # cross-validate the individual models
-        by_group_metrics, by_group_scores = self.get_model_by_group_data(algorithm, dataset)
-        by_group_metrics = by_group_metrics.melt(id_vars=['group'], value_vars=metrics, var_name='metric',
-                                                 ignore_index=False).assign(model='by_group')
-        metric_data: pd.DataFrame = pd.concat([baseline_metrics, by_group_metrics]).sort_values(['model', 'metric'])
-        metric_data = metric_data.set_index(['metric', 'group'], append=True).pivot(columns='model',
-                                                                                    values='value').reset_index(
-            'metric')
-
-        if title is None:
-            title = f'Model by Group Test on {algorithm} with {self.k_folds} folds'
-
-        num_plots: int = len(metrics) if len(metrics) > 0 else 1
-        num_cols: int = num_plots if col_wrap is None else col_wrap
-        num_rows, _ = subplot_index(len(metrics) - 1, col_wrap=num_cols)
-        fig = make_subplots(rows=num_rows, cols=num_cols,
-                            subplot_titles=metrics)
-
-        # metrics
-        for i, metric in enumerate(metrics):
-            row, col = subplot_index(i, col_wrap=num_cols)
-            colorscale = colors.qualitative.Plotly
-            add_to_legend = True if i == 0 else False
-            df_metric: pd.DataFrame = metric_data.query('metric==@metric').drop(columns=['metric'])
-            x = df_metric.index.get_level_values('group')
-            for g, grp in enumerate(df_metric.columns):
-                fig.add_trace(go.Box(x=x, y=df_metric[grp], name=grp, boxpoints='all', notched=True,
-                                     legendgroup=self.group.name,
-                                     showlegend=add_to_legend,
-                                     line={"color": colorscale[g]}, marker={"color": colorscale[g]},
-                                     offsetgroup=str(g)), row=row, col=col)
-
-        fig.update_layout(title=title, showlegend=False)
-        fig.update_layout(boxmode='group', showlegend=True, legend_title='model',
-                          boxgroupgap=0.5, boxgap=0
-                          )
-
-        return fig
-
-    def get_model_by_group_data(self, algorithm, dataset):
-        results: dict = {}
-        by_group_score_chunks: list = []
-        by_group_metric_chunks: list = []
-        for grp in self.group.unique():
-            grp_index: pd.Index = self.group.loc[self.group == grp].index
-            x: pd.DataFrame = self.datasets[dataset][self.features_in].loc[grp_index]
-            y: pd.DataFrame = self.datasets[dataset][self.target].loc[grp_index]
-            if self.pre_processor:
-                x = self.pre_processor.set_output(transform="pandas").fit_transform(X=x)
-            kfold = model_selection.KFold(n_splits=self.k_folds, random_state=self.random_state, shuffle=True)
-            res = cross_validate(self.algorithms[algorithm], x, y, cv=kfold, scoring=self.scorer, return_estimator=True,
-                                 return_indices=True)
-            by_group_score_chunks.append(pd.Series(res['test_score'], name=grp))
-            if self.metrics is not None:
-                res['metrics'], _ = self.calculate_metrics(x=x, y=y,
-                                                           estimators=res['estimator'],
-                                                           indices=res['indices'],
-                                                           group=None)
-            results[grp] = res
-            by_group_metric_chunks.append(
-                pd.DataFrame(res['metrics']).assign(group=grp).rename_axis('fold', axis='index'))
-        by_group_metrics: pd.DataFrame = pd.concat(by_group_metric_chunks)
-        #                                   .reset_index().melt(id_vars=['fold', 'group'],
-        #                                                                                       value_vars=list(
-        #                                                                                           self.metrics.keys()),
-        #                                                                                       var_name='metric'))
-        # by_group_metrics = by_group_metrics.set_index(['fold', 'metric', 'group']).unstack(level=-1)
-        # by_group_metrics = by_group_metrics.droplevel(level=0, axis=1).reset_index(-1)
-        by_group_scores = pd.concat(by_group_score_chunks, axis=1)
-
-        return by_group_metrics, by_group_scores
-
-    def get_cv_scores(self) -> pd.DataFrame:
-        chunks: List = []
-        for data_key, data in self.datasets.items():
-            for algo_key, algo in self.algorithms.items():
-                chunks.append(pd.Series(self.data[data_key][algo_key][f"test_score"], name=(data_key, algo_key)))
-        return pd.concat(chunks, axis=1)
-
-    def get_cv_metrics(self, metrics, by_group: bool = False) -> pd.DataFrame:
-        chunks: List = []
-        metric_key = "metrics_group" if by_group else "metrics"
-        for data_key, data in self.datasets.items():
-            for algo_key, algo in self.algorithms.items():
-                for metric in metrics:
-                    chunks.append(pd.DataFrame(self.data[data_key][algo_key][metric_key][metric]).assign(
-                        **dict(data_key=data_key, algo_key=algo_key, metric=metric)))
-        res: pd.DataFrame = pd.concat(chunks, axis=0).set_index(['data_key', 'algo_key'], append=True).rename(
-            columns={0: 'value'})
-        res.index.names = ['fold', 'data_key', 'algo_key']
-        return res
-
-    def calculate_metrics(self, x, y, estimators, indices, group) -> Tuple[Dict, Dict]:
-        metric_results: Dict = {}
-        metric_results_group: Dict = {}
-
-        for k, fn_metric in self.metrics.items():
-            metric_values: List = []
-            metric_groups: Dict = {}
-            for estimator, test_indexes in zip(estimators, indices['test']):
-                y_true = y[y.index[test_indexes]]
-                y_est = estimator.predict(x.loc[x.index[test_indexes], :])
-                if isinstance(y_est, pd.DataFrame) and y_est.shape[1] == 1:
-                    y_est = y_est.iloc[:, 0]
-                metric_values.append(fn_metric(y_true, y_est))
-                if group is not None:
-                    # calculate the metric by each group in the group series.
-                    y_est = pd.merge(left=pd.Series(y_est, name='y_est', index=x.index[test_indexes]),
-                                     right=group, left_index=True, right_index=True)
-                    y_est_grouped = y_est.groupby([group.name])
-                    grouped_results = [y_est_grouped.get_group(x) for x in y_est_grouped.groups]
-                    for grp_res in grouped_results:
-                        group_value = str(grp_res[group.name].iloc[0])
-                        group_metric_results = fn_metric(y_true[grp_res.index], grp_res['y_est'].values)
-                        if group_value not in metric_groups.keys():
-                            metric_groups[group_value] = [group_metric_results]
-                        else:
-                            metric_groups[group_value].append(group_metric_results)
-            metric_results[k] = metric_values
-            if group is not None:
-                metric_results_group[k] = metric_groups
-
-        return metric_results, metric_results_group
-
-# if __name__ == '__main__':
-#
-#     for i in range(0, 7):
-#         print(subplot_index(i, col_wrap=3))
-#
-#     print('done')
+import logging
+from typing import Union, Optional, Dict, List, Callable, Tuple
+
+import matplotlib
+import numpy as np
+import pandas as pd
+import plotly.graph_objects as go
+import sklearn
+from plotly import colors
+from plotly.subplots import make_subplots
+from sklearn import model_selection
+from sklearn.base import is_classifier, is_regressor
+from sklearn.model_selection import cross_validate
+from sklearn.pipeline import Pipeline
+
+from elphick.sklearn_viz.model_selection.metrics import regression_metrics, classification_metrics
+from elphick.sklearn_viz.model_selection.scorers import classification_scorers, regression_scorers
+
+
+def subplot_index(idx: int, col_wrap: int) -> Tuple[int, int]:
+    col: int = int(idx % col_wrap + 1)
+    row: int = int(np.floor(idx / col_wrap) + 1)
+    return row, col
+
+
+def plot_model_selection(algorithms: Union[sklearn.base.RegressorMixin, sklearn.base.ClassifierMixin, Dict],
+                         datasets: Union[pd.DataFrame, Dict],
+                         target: str,
+                         pre_processor: Optional[Pipeline] = None,
+                         k_folds: int = 10,
+                         title: Optional[str] = None) -> go.Figure:
+    """
+
+    Args:
+            algorithms: sklearn estimator or a Dict of algorithms to cross-validate, keyed by string name/code.
+            datasets: pandas DataFrame or a dict of DataFrames, keyed by string name/code.
+            target: target column
+            pre_processor: Optional pipeline used to pre-process the datasets.
+            k_folds: The number of cross validation folds.
+            title: Optional plot title
+
+    Returns:
+        a plotly GraphObjects.Figure
+
+    """
+
+    return ModelSelection(algorithms=algorithms, datasets=datasets, target=target, pre_processor=pre_processor,
+                          k_folds=k_folds).plot(title=title)
+
+
+class ModelSelection:
+    def __init__(self,
+                 algorithms: Union[
+                     sklearn.base.RegressorMixin, sklearn.base.ClassifierMixin, Dict[str, sklearn.base.BaseEstimator]],
+                 datasets: Union[pd.DataFrame, Dict[str, pd.DataFrame]],
+                 target: str,
+                 pre_processor: Optional[Pipeline] = None,
+                 k_folds: int = 10,
+                 scorer: Optional[Union[str, Callable]] = None,
+                 metrics: Optional[Dict[str, Callable]] = None,
+                 group: Optional[pd.Series] = None,
+                 random_state: Optional[int] = None):
+        """
+
+        Args:
+            algorithms: sklearn estimator or a Dict of algorithms to cross-validate, keyed by string name/code.
+            datasets: pandas DataFrame or a dict of DataFrames, keyed by string name/code.
+            target: target column
+            pre_processor: Optional pipeline used to pre-process the datasets.
+            k_folds: The number of cross validation folds.
+            scorer: Optional callable scorers which the model will be fitted using
+            metrics: Optional Dict of callable metrics to calculate post-fitting
+            group: Optional group variable by which to partition/group metrics.  The same group applies across all
+             datasets, so is more useful when testing different algorithms.
+            random_state: Optional random seed
+        """
+        self._logger = logging.getLogger(name=__class__.__name__)
+        self.pre_processor: Pipeline = pre_processor
+        if isinstance(algorithms, sklearn.base.BaseEstimator):
+            self.algorithms = {algorithms.__class__.__name__: algorithms}
+        else:
+            self.algorithms = algorithms
+        if isinstance(datasets, pd.DataFrame):
+            self.datasets = {'Dataset': datasets}
+        else:
+            self.datasets = datasets
+        self.target = target
+        self.k_folds: int = k_folds
+
+        self.is_classifier: bool = is_classifier(list(self.algorithms.values())[0])
+        self.is_regressor: bool = is_regressor(list(self.algorithms.values())[0])
+        if scorer is not None:
+            self.scorer = scorer
+        else:
+            self.scorer = classification_scorers[list(classification_scorers.keys())[0]] if self.is_classifier else \
+                regression_scorers[list(regression_scorers.keys())[0]]
+
+        if metrics is not None:
+            self.metrics = metrics
+        else:
+            self.metrics = classification_metrics if self.is_classifier else regression_metrics
+
+        self.group: pd.Series = group
+        self.random_state: Optional[int] = random_state
+
+        self.features_in: List[str] = [col for col in self.datasets[list(self.datasets.keys())[0]] if
+                                       col != self.target]
+
+        self._data: Optional[Dict] = None
+        self._num_algorithms: int = len(list(self.algorithms.keys()))
+        self._num_datasets: int = len(list(self.datasets.keys()))
+
+        if self._num_algorithms > 1 and self._num_datasets > 1:
+            raise NotImplementedError("Cannot have multiple algorithms and multiple datasets.")
+
+    @property
+    def data(self) -> Optional[Dict]:
+        if self.metrics is None:
+            cv_kwargs: Dict = dict()
+        else:
+            cv_kwargs: Dict = dict(return_estimator=True, return_indices=True, error_score=np.nan)
+
+        if self._data is not None:
+            results = self._data
+        else:
+            results: Dict = {}
+            for data_key, data in self.datasets.items():
+                self._logger.info(f"Commencing Cross Validation for dataset {data_key}")
+                results[data_key] = {}
+                x: pd.DataFrame = data[self.features_in]
+                y: pd.DataFrame = data[self.target]
+                if self.pre_processor:
+                    x = self.pre_processor.set_output(transform="pandas").fit_transform(X=x)
+
+                for algo_key, algo in self.algorithms.items():
+                    kfold = model_selection.KFold(n_splits=self.k_folds, random_state=self.random_state, shuffle=True)
+                    res = cross_validate(algo, x, y, cv=kfold, scoring=self.scorer, **cv_kwargs)
+                    if self.metrics is not None:
+                        res['metrics'], res['metrics_group'] = self.calculate_metrics(x=x, y=y,
+                                                                                      estimators=res['estimator'],
+                                                                                      indices=res['indices'],
+                                                                                      group=self.group)
+                    results[data_key][algo_key] = res
+                    res_mean = res[f"test_score"].mean()
+                    res_std = res[f"test_score"].std()
+                    self._logger.info(f"CV Results for {algo_key}: Mean = {res_mean}, SD = {res_std}")
+
+            self._data = results
+
+        return results
+
+    def plot(self,
+             metrics: Optional[Union[str, List[str]]] = None,
+             show_group: bool = False,
+             title: Optional[str] = None,
+             col_wrap: Optional[int] = None) -> go.Figure:
+        """Create the plot
+
+        The plot will show the cross-validation scores for each algorithm and dataset.  The first panel is used to show
+        the scorer, that is the metric used to fit the model.  If multiple metrics are supplied, each metric will be
+        shown in a separate panel.  If a show_group is true, the metrics will be grouped by the group variable.
+        col_wrap allows the width of the plot to be controlled by wrapping the columns to new rows.
+
+        KUDOS: https://towardsdatascience.com/applying-a-custom-colormap-with-plotly-boxplots-5d3acf59e193
+
+        Args:
+            metrics: The metric or metrics to plot in addition to the scorer.  Each metric will be plotted in a
+             separate panel.
+            show_group: If True (and a group variable has been set), plot by group.
+            title: Title of the plot
+            col_wrap: If plotting multiple metrics, col_wrap will wrap columns to new rows, resulting in
+             col-wrap columns, and multiple rows.
+
+        Returns:
+            a plotly GraphObjects.Figure
+
+        """
+
+        data: pd.DataFrame = self.get_cv_scores()
+        data = data.droplevel(level=0, axis=1) if self._num_datasets == 1 else data.droplevel(level=1, axis=1)
+
+        metric_data: pd.DataFrame = pd.DataFrame()
+
+        if metrics is not None:
+            if isinstance(metrics, str):
+                metrics = [metrics]
+            metric_data = self.get_cv_metrics(metrics, show_group)
+        else:
+            metrics = []
+
+        if self._num_algorithms > 1:
+            x_index = 'algo_key'
+        else:
+            x_index = 'data_key'
+
+        # define the color map for the scorer
+        vmin, vmax = data.min().min(), data.max().max()
+        norm = matplotlib.colors.Normalize(vmin=vmin, vmax=vmax)
+        cmap = matplotlib.cm.get_cmap('RdYlGn')
+
+        subtitle: str = f'Cross Validation folds={self.k_folds}'
+        if title is None:
+            title = subtitle
+        else:
+            title = title + '<br>' + subtitle
+
+        # create the plot, managing the shape.
+        num_plots: int = len(metrics) + 1 if len(metrics) > 0 else 1
+        num_cols: int = num_plots if col_wrap is None else col_wrap
+        num_rows, _ = subplot_index(len(metrics), col_wrap=num_cols)
+        fig = make_subplots(rows=num_rows, cols=num_cols, subplot_titles=[f'{self.scorer} (scorer)'] + metrics)
+
+        # Add the scorer subplot
+        for col in data.columns:
+            # For the scorer build the plot by column to color individually based on score
+            median = np.median(data[col])  # find the median
+            color = 'rgb' + str(cmap(norm(median))[0:3])  # normalize
+            fig.add_trace(go.Box(y=data[col], name=col, boxpoints='all', notched=True, fillcolor=color,
+                                 line={"color": "grey"}, marker={"color": "grey"}, showlegend=False,
+                                 offsetgroup='A'), row=1, col=1)
+
+        # add the metric subplots
+        for i, metric in enumerate(metrics):
+            row, col = subplot_index(i + 1, col_wrap=num_cols)
+            if show_group:
+                colorscale = colors.qualitative.Plotly + colors.qualitative.Dark24
+                add_to_legend = True if i == 0 else False
+                df_metric: pd.DataFrame = metric_data.query('metric==@metric').drop(columns=['metric'])
+                x = df_metric.index.get_level_values(x_index)
+                for g, grp in enumerate(df_metric.columns):
+                    if len(df_metric.columns) > len(colorscale):
+                        raise ValueError("Too many groups to plot")
+                    fig.add_trace(go.Box(x=x, y=df_metric[grp], name=grp, boxpoints='all', notched=True,
+                                         legendgroup=self.group.name,
+                                         showlegend=add_to_legend,
+                                         line={"color": colorscale[g]}, marker={"color": colorscale[g]},
+                                         offsetgroup=str(g)), row=row, col=col)
+            else:
+                df_metric: pd.DataFrame = metric_data.query('metric==@metric').drop(columns=['metric'])
+                x = list(df_metric.index.get_level_values(x_index))
+                fig.add_trace(go.Box(x=x, y=df_metric.values.ravel(), name=metric, boxpoints='all', notched=True,
+                                     line={"color": "grey"}, marker={"color": "grey"}), row=row, col=col)
+
+        # finalise some display elements
+        fig.update_layout(title=title, showlegend=False)
+        if show_group:
+            fig.update_layout(boxmode='group', showlegend=True, legend_title=self.group.name,
+                              boxgroupgap=0.5, boxgap=0
+                              )
+
+        return fig
+
+    def plot_category_analysis(self,
+                               algorithm: Optional[str] = None,
+                               dataset: Optional[str] = None,
+                               metrics: Optional[Union[str, List[str]]] = None,
+                               title: Optional[str] = None,
+                               col_wrap: Optional[int] = None) -> go.Figure:
+        """Plot the category feature analysis
+
+        Args:
+            algorithm: If supplied, this will be the name of the algorithm tested.  If None the first algorithm is used.
+            dataset: If supplied, this will be the name of the dataset tested.  If None the first dataset is used.
+            metrics: The metric or metrics to show.  Each metric will be plotted in a
+             separate panel.
+            title: Title of the plot
+            col_wrap: If plotting multiple metrics, col_wrap will wrap columns to new rows, resulting in
+             col-wrap columns, and multiple rows.
+
+        Returns:
+            a plotly GraphObjects.Figure
+
+        """
+        algorithms: list[str] = list(self.algorithms.keys())
+        algorithm: str = algorithms[0] if algorithm is None else algorithm
+        if algorithm not in algorithms:
+            raise KeyError(f"Algorithm {algorithm} is not in the list of available algorithms: {algorithms}")
+
+        datasets: list[str] = list(self.datasets.keys())
+        dataset: str = datasets[0] if dataset is None else dataset
+        if dataset not in datasets:
+            raise KeyError(f"Dataset {dataset} is not in the list of available datasets: {datasets}")
+
+        metrics: list[str] = [list(self.metrics.keys())[0]] if metrics is None else metrics
+
+        baseline_metrics: pd.DataFrame = self.get_cv_metrics(metrics, by_group=True).loc[
+            (slice(None), dataset, algorithm)]
+        baseline_metrics = baseline_metrics.melt(id_vars=['metric'], value_vars=self.group.unique().tolist(),
+                                                 var_name='group',
+                                                 ignore_index=False).assign(model='baseline')
+
+        # cross-validate the individual models
+        by_group_metrics, by_group_scores = self.get_model_by_group_data(algorithm, dataset)
+        by_group_metrics = by_group_metrics.melt(id_vars=['group'], value_vars=metrics, var_name='metric',
+                                                 ignore_index=False).assign(model='by_group')
+        metric_data: pd.DataFrame = pd.concat([baseline_metrics, by_group_metrics]).sort_values(['model', 'metric'])
+        metric_data = metric_data.set_index(['metric', 'group'], append=True).pivot(columns='model',
+                                                                                    values='value').reset_index(
+            'metric')
+
+        if title is None:
+            title = f'Model by Group Test on {algorithm} with {self.k_folds} folds'
+
+        num_plots: int = len(metrics) if len(metrics) > 0 else 1
+        num_cols: int = num_plots if col_wrap is None else col_wrap
+        num_rows, _ = subplot_index(len(metrics) - 1, col_wrap=num_cols)
+        fig = make_subplots(rows=num_rows, cols=num_cols,
+                            subplot_titles=metrics)
+
+        # metrics
+        for i, metric in enumerate(metrics):
+            row, col = subplot_index(i, col_wrap=num_cols)
+            colorscale = colors.qualitative.Plotly
+            add_to_legend = True if i == 0 else False
+            df_metric: pd.DataFrame = metric_data.query('metric==@metric').drop(columns=['metric'])
+            x = df_metric.index.get_level_values('group')
+            for g, grp in enumerate(df_metric.columns):
+                fig.add_trace(go.Box(x=x, y=df_metric[grp], name=grp, boxpoints='all', notched=True,
+                                     legendgroup=self.group.name,
+                                     showlegend=add_to_legend,
+                                     line={"color": colorscale[g]}, marker={"color": colorscale[g]},
+                                     offsetgroup=str(g)), row=row, col=col)
+
+        fig.update_layout(title=title, showlegend=False)
+        fig.update_layout(boxmode='group', showlegend=True, legend_title='model',
+                          boxgroupgap=0.5, boxgap=0
+                          )
+
+        return fig
+
+    def get_model_by_group_data(self, algorithm, dataset):
+        results: dict = {}
+        by_group_score_chunks: list = []
+        by_group_metric_chunks: list = []
+        for grp in self.group.unique():
+            grp_index: pd.Index = self.group.loc[self.group == grp].index
+            x: pd.DataFrame = self.datasets[dataset][self.features_in].loc[grp_index]
+            y: pd.DataFrame = self.datasets[dataset][self.target].loc[grp_index]
+            if self.pre_processor:
+                x = self.pre_processor.set_output(transform="pandas").fit_transform(X=x)
+            kfold = model_selection.KFold(n_splits=self.k_folds, random_state=self.random_state, shuffle=True)
+            res = cross_validate(self.algorithms[algorithm], x, y, cv=kfold, scoring=self.scorer, return_estimator=True,
+                                 return_indices=True)
+            by_group_score_chunks.append(pd.Series(res['test_score'], name=grp))
+            if self.metrics is not None:
+                res['metrics'], _ = self.calculate_metrics(x=x, y=y,
+                                                           estimators=res['estimator'],
+                                                           indices=res['indices'],
+                                                           group=None)
+            results[grp] = res
+            by_group_metric_chunks.append(
+                pd.DataFrame(res['metrics']).assign(group=grp).rename_axis('fold', axis='index'))
+        by_group_metrics: pd.DataFrame = pd.concat(by_group_metric_chunks)
+        #                                   .reset_index().melt(id_vars=['fold', 'group'],
+        #                                                                                       value_vars=list(
+        #                                                                                           self.metrics.keys()),
+        #                                                                                       var_name='metric'))
+        # by_group_metrics = by_group_metrics.set_index(['fold', 'metric', 'group']).unstack(level=-1)
+        # by_group_metrics = by_group_metrics.droplevel(level=0, axis=1).reset_index(-1)
+        by_group_scores = pd.concat(by_group_score_chunks, axis=1)
+
+        return by_group_metrics, by_group_scores
+
+    def get_cv_scores(self) -> pd.DataFrame:
+        chunks: List = []
+        for data_key, data in self.datasets.items():
+            for algo_key, algo in self.algorithms.items():
+                chunks.append(pd.Series(self.data[data_key][algo_key][f"test_score"], name=(data_key, algo_key)))
+        return pd.concat(chunks, axis=1)
+
+    def get_cv_metrics(self, metrics, by_group: bool = False) -> pd.DataFrame:
+        chunks: List = []
+        metric_key = "metrics_group" if by_group else "metrics"
+        for data_key, data in self.datasets.items():
+            for algo_key, algo in self.algorithms.items():
+                for metric in metrics:
+                    chunks.append(pd.DataFrame(self.data[data_key][algo_key][metric_key][metric]).assign(
+                        **dict(data_key=data_key, algo_key=algo_key, metric=metric)))
+        res: pd.DataFrame = pd.concat(chunks, axis=0).set_index(['data_key', 'algo_key'], append=True).rename(
+            columns={0: 'value'})
+        res.index.names = ['fold', 'data_key', 'algo_key']
+        return res
+
+    def calculate_metrics(self, x, y, estimators, indices, group) -> Tuple[Dict, Dict]:
+        metric_results: Dict = {}
+        metric_results_group: Dict = {}
+
+        for k, fn_metric in self.metrics.items():
+            metric_values: List = []
+            metric_groups: Dict = {}
+            for estimator, test_indexes in zip(estimators, indices['test']):
+                y_true = y[y.index[test_indexes]]
+                y_est = estimator.predict(x.loc[x.index[test_indexes], :])
+                if isinstance(y_est, pd.DataFrame) and y_est.shape[1] == 1:
+                    y_est = y_est.iloc[:, 0]
+                metric_values.append(fn_metric(y_true, y_est))
+                if group is not None:
+                    # calculate the metric by each group in the group series.
+                    y_est = pd.merge(left=pd.Series(y_est, name='y_est', index=x.index[test_indexes]),
+                                     right=group, left_index=True, right_index=True)
+                    y_est_grouped = y_est.groupby([group.name])
+                    grouped_results = [y_est_grouped.get_group(x) for x in y_est_grouped.groups]
+                    for grp_res in grouped_results:
+                        group_value = str(grp_res[group.name].iloc[0])
+                        group_metric_results = fn_metric(y_true[grp_res.index], grp_res['y_est'].values)
+                        if group_value not in metric_groups.keys():
+                            metric_groups[group_value] = [group_metric_results]
+                        else:
+                            metric_groups[group_value].append(group_metric_results)
+            metric_results[k] = metric_values
+            if group is not None:
+                metric_results_group[k] = metric_groups
+
+        return metric_results, metric_results_group
+
+# if __name__ == '__main__':
+#
+#     for i in range(0, 7):
+#         print(subplot_index(i, col_wrap=3))
+#
+#     print('done')
```

### Comparing `sklearn_viz-0.4.2/elphick/sklearn_viz/model_selection/models.py` & `sklearn_viz-0.4.9/elphick/sklearn_viz/model_selection/models.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-from dataclasses import dataclass
-from enum import Enum
-from typing import Union, List, Dict
-
-import sklearn.base
-from sklearn.discriminant_analysis import LinearDiscriminantAnalysis
-from sklearn.ensemble import RandomForestRegressor, RandomForestClassifier
-from sklearn.linear_model import LogisticRegression, LinearRegression, LassoCV, RidgeCV, ElasticNetCV
-from sklearn.naive_bayes import GaussianNB
-from sklearn.neighbors import KNeighborsClassifier
-from sklearn.svm import SVC
-from sklearn.tree import DecisionTreeClassifier, DecisionTreeRegressor
-
-
-class ModelType(Enum):
-    REGRESSOR = 'regressor'
-    CLASSIFIER = 'classifier'
-
-
-@dataclass
-class Model:
-    code: str
-    model: Union[sklearn.base.RegressorMixin, sklearn.base.ClassifierMixin]
-    type: ModelType
-    fast: bool
-
-
-class Models:
-    def __init__(self):
-        self.LR_C = Model('LR', LogisticRegression(), ModelType.CLASSIFIER, True)
-        self.LDA = Model('LDA', LinearDiscriminantAnalysis(), ModelType.CLASSIFIER, True)
-        self.KNN = Model('KNN', KNeighborsClassifier(), ModelType.CLASSIFIER, True)
-        self.CART_C = Model('CART', DecisionTreeClassifier(), ModelType.CLASSIFIER, True)
-        self.NB = Model('NB', GaussianNB(), ModelType.CLASSIFIER, True)
-        self.SVM = Model('SVM', SVC(), ModelType.CLASSIFIER, True)
-        self.RF_C = Model('RF', RandomForestClassifier(), ModelType.REGRESSOR, False)
-        self.LR_R = Model('LR', LinearRegression(), ModelType.REGRESSOR, True)
-        self.LASSO = Model('LASSO', LassoCV(), ModelType.REGRESSOR, True)
-        self.RIDGE = Model('RIDGE', RidgeCV(), ModelType.REGRESSOR, True)
-        self.ELASTIC = Model('ELASTIC', ElasticNetCV(), ModelType.REGRESSOR, True)
-        self.CART_R = Model('CART', DecisionTreeRegressor(), ModelType.REGRESSOR, True)
-        self.RF_R = Model('RF', RandomForestRegressor(), ModelType.REGRESSOR, False)
-
-    def fast_classifiers(self) -> Dict:
-        return {v.code: v.model for k, v in self.__dict__.items() if
-                v.type == ModelType.CLASSIFIER and v.fast is True}
-
-    def all_classifiers(self) -> Dict:
-        return {v.code: v.model for k, v in self.__dict__.items() if v.type == ModelType.CLASSIFIER}
-
-    def fast_regressors(self) -> Dict:
-        return {v.code: v.model for k, v in self.__dict__.items() if v.type == ModelType.REGRESSOR and v.fast is True}
-
-    def all_regressors(self) -> Dict:
-        return {v.code: v.model for k, v in self.__dict__.items() if v.type == ModelType.REGRESSOR}
+from dataclasses import dataclass
+from enum import Enum
+from typing import Union, List, Dict
+
+import sklearn.base
+from sklearn.discriminant_analysis import LinearDiscriminantAnalysis
+from sklearn.ensemble import RandomForestRegressor, RandomForestClassifier
+from sklearn.linear_model import LogisticRegression, LinearRegression, LassoCV, RidgeCV, ElasticNetCV
+from sklearn.naive_bayes import GaussianNB
+from sklearn.neighbors import KNeighborsClassifier
+from sklearn.svm import SVC
+from sklearn.tree import DecisionTreeClassifier, DecisionTreeRegressor
+
+
+class ModelType(Enum):
+    REGRESSOR = 'regressor'
+    CLASSIFIER = 'classifier'
+
+
+@dataclass
+class Model:
+    code: str
+    model: Union[sklearn.base.RegressorMixin, sklearn.base.ClassifierMixin]
+    type: ModelType
+    fast: bool
+
+
+class Models:
+    def __init__(self):
+        self.LR_C = Model('LR', LogisticRegression(), ModelType.CLASSIFIER, True)
+        self.LDA = Model('LDA', LinearDiscriminantAnalysis(), ModelType.CLASSIFIER, True)
+        self.KNN = Model('KNN', KNeighborsClassifier(), ModelType.CLASSIFIER, True)
+        self.CART_C = Model('CART', DecisionTreeClassifier(), ModelType.CLASSIFIER, True)
+        self.NB = Model('NB', GaussianNB(), ModelType.CLASSIFIER, True)
+        self.SVM = Model('SVM', SVC(), ModelType.CLASSIFIER, True)
+        self.RF_C = Model('RF', RandomForestClassifier(), ModelType.REGRESSOR, False)
+        self.LR_R = Model('LR', LinearRegression(), ModelType.REGRESSOR, True)
+        self.LASSO = Model('LASSO', LassoCV(), ModelType.REGRESSOR, True)
+        self.RIDGE = Model('RIDGE', RidgeCV(), ModelType.REGRESSOR, True)
+        self.ELASTIC = Model('ELASTIC', ElasticNetCV(), ModelType.REGRESSOR, True)
+        self.CART_R = Model('CART', DecisionTreeRegressor(), ModelType.REGRESSOR, True)
+        self.RF_R = Model('RF', RandomForestRegressor(), ModelType.REGRESSOR, False)
+
+    def fast_classifiers(self) -> Dict:
+        return {v.code: v.model for k, v in self.__dict__.items() if
+                v.type == ModelType.CLASSIFIER and v.fast is True}
+
+    def all_classifiers(self) -> Dict:
+        return {v.code: v.model for k, v in self.__dict__.items() if v.type == ModelType.CLASSIFIER}
+
+    def fast_regressors(self) -> Dict:
+        return {v.code: v.model for k, v in self.__dict__.items() if v.type == ModelType.REGRESSOR and v.fast is True}
+
+    def all_regressors(self) -> Dict:
+        return {v.code: v.model for k, v in self.__dict__.items() if v.type == ModelType.REGRESSOR}
```

### Comparing `sklearn_viz-0.4.2/elphick/sklearn_viz/residuals/error.py` & `sklearn_viz-0.4.9/elphick/sklearn_viz/residuals/error.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-import logging
-from typing import Optional, Union
-
-import pandas as pd
-from sklearn.pipeline import Pipeline
-from sklearn.utils.validation import check_is_fitted
-import plotly.graph_objects as go
-import plotly.express as px
-
-
-class Errors:
-    def __init__(self,
-                 mdl,
-                 x_test: Optional[pd.DataFrame] = None,
-                 y_test: Optional[Union[pd.DataFrame, pd.Series]] = None):
-        """
-
-        Args:
-            mdl: The scikit-learn model or pipeline.
-            x_test: X values provided to calculate residuals.
-            y_test: y values provided to calculate residuals.
-        """
-        self._logger = logging.getLogger(name=__class__.__name__)
-        self.mdl = mdl
-        self.X_test: Optional[pd.DataFrame] = x_test
-        self.y_test: Optional[Union[pd.DataFrame, pd.Series]] = y_test
-        self._data: Optional[pd.DataFrame] = None
-        self.is_pipeline: bool = isinstance(mdl, Pipeline)
-
-        check_is_fitted(mdl[-1]) if self.is_pipeline else check_is_fitted(mdl)
-
-    def plot(self, color: Optional[str] = None, title: Optional[str] = 'Error Plot') -> go.Figure:
-        """
-
-        Args:
-            color: The variable name to color (group) by.
-            title: title for the plot
-
-        Returns:
-            a plotly GraphObjects.Figure
-
-        """
-        y_est = pd.Series(self.mdl.predict(self.X_test), name=f"{self.y_test.name}_est", index=self.X_test.index)
-        y = self.y_test
-        data = pd.concat([y, y_est], axis='columns')
-        lims = [data.min().min(), data.max().max()]
-        fig = px.scatter(
-            data,
-            x=y.name, y=y_est.name,
-            marginal_x='histogram', marginal_y='histogram',
-            color=color, trendline='ols'
-        )
-        fig.update_traces(histnorm='probability', selector={'type': 'histogram'})
-        fig.add_shape(
-            type="line", line=dict(dash='dash'),
-            x0=lims[0], y0=lims[0],
-            x1=lims[1], y1=lims[1]
-        )
-
-        fig.update_layout(title=title)
-
-        return fig
+import logging
+from typing import Optional, Union
+
+import pandas as pd
+from sklearn.pipeline import Pipeline
+from sklearn.utils.validation import check_is_fitted
+import plotly.graph_objects as go
+import plotly.express as px
+
+
+class Errors:
+    def __init__(self,
+                 mdl,
+                 x_test: Optional[pd.DataFrame] = None,
+                 y_test: Optional[Union[pd.DataFrame, pd.Series]] = None):
+        """
+
+        Args:
+            mdl: The scikit-learn model or pipeline.
+            x_test: X values provided to calculate residuals.
+            y_test: y values provided to calculate residuals.
+        """
+        self._logger = logging.getLogger(name=__class__.__name__)
+        self.mdl = mdl
+        self.X_test: Optional[pd.DataFrame] = x_test
+        self.y_test: Optional[Union[pd.DataFrame, pd.Series]] = y_test
+        self._data: Optional[pd.DataFrame] = None
+        self.is_pipeline: bool = isinstance(mdl, Pipeline)
+
+        check_is_fitted(mdl[-1]) if self.is_pipeline else check_is_fitted(mdl)
+
+    def plot(self, color: Optional[str] = None, title: Optional[str] = 'Error Plot') -> go.Figure:
+        """
+
+        Args:
+            color: The variable name to color (group) by.
+            title: title for the plot
+
+        Returns:
+            a plotly GraphObjects.Figure
+
+        """
+        y_est = pd.Series(self.mdl.predict(self.X_test), name=f"{self.y_test.name}_est", index=self.X_test.index)
+        y = self.y_test
+        data = pd.concat([y, y_est], axis='columns')
+        lims = [data.min().min(), data.max().max()]
+        fig = px.scatter(
+            data,
+            x=y.name, y=y_est.name,
+            marginal_x='histogram', marginal_y='histogram',
+            color=color, trendline='ols'
+        )
+        fig.update_traces(histnorm='probability', selector={'type': 'histogram'})
+        fig.add_shape(
+            type="line", line=dict(dash='dash'),
+            x0=lims[0], y0=lims[0],
+            x1=lims[1], y1=lims[1]
+        )
+
+        fig.update_layout(title=title)
+
+        return fig
```

### Comparing `sklearn_viz-0.4.2/elphick/sklearn_viz/utils/timer.py` & `sklearn_viz-0.4.9/elphick/sklearn_viz/utils/timer.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-"""
-REF: https://ankitbko.github.io/blog/2021/04/logging-in-python/
-"""
-
-import functools
-import logging
-from datetime import datetime
-from typing import Union
-
-
-class MyLogger:
-    def __init__(self):
-        logging.basicConfig(level=logging.INFO,
-                            format=' %(asctime)s - %(levelname)s - %(message)s')
-
-    def get_logger(self, name=None):
-        return logging.getLogger(name)
-
-
-def get_default_logger():
-    return MyLogger().get_logger()
-
-
-def log_timer(_func=None, *, my_logger: Union[MyLogger, logging.Logger] = None):
-    def decorator_log(func):
-        @functools.wraps(func)
-        def wrapper(*args, **kwargs):
-            logger = get_default_logger()
-            try:
-                if my_logger is None:
-                    first_args = next(iter(args), None)  # capture first arg to check for `self`
-                    logger_params = [  # does kwargs have any logger
-                                        x
-                                        for x in kwargs.values()
-                                        if isinstance(x, logging.Logger) or isinstance(x, MyLogger)
-                                    ] + [  # # does args have any logger
-                                        x
-                                        for x in args
-                                        if isinstance(x, logging.Logger) or isinstance(x, MyLogger)
-                                    ]
-                    if hasattr(first_args, "__dict__"):  # is first argument `self`
-                        logger_params = logger_params + [
-                            x
-                            for x in first_args.__dict__.values()  # does class (dict) members have any logger
-                            if isinstance(x, logging.Logger)
-                               or isinstance(x, MyLogger)
-                        ]
-                    h_logger = next(iter(logger_params), MyLogger())  # get the next/first/default logger
-                else:
-                    h_logger = my_logger  # logger is passed explicitly to the decorator
-
-                if isinstance(h_logger, MyLogger):
-                    logger = h_logger.get_logger(func.__name__)
-                else:
-                    logger = h_logger
-
-                # args_repr = [repr(a) for a in args]
-                # kwargs_repr = [f"{k}={v!r}" for k, v in kwargs.items()]
-                # signature = ", ".join(args_repr + kwargs_repr)
-                # logger.debug(f"function {func.__name__} called with args {signature}")
-
-            except Exception:
-                pass
-
-            try:
-                _tic = datetime.now()
-                result = func(*args, **kwargs)
-                _toc = datetime.now()
-                logger.info(f"Elapsed time for {func.__name__}: {_toc - _tic}")
-                return result
-            except Exception as e:
-                logger.exception(f"Exception raised in {func.__name__}. exception: {str(e)}")
-                raise e
-
-        return wrapper
-
-    if _func is None:
-        return decorator_log
-    else:
-        return decorator_log(_func)
+"""
+REF: https://ankitbko.github.io/blog/2021/04/logging-in-python/
+"""
+
+import functools
+import logging
+from datetime import datetime
+from typing import Union
+
+
+class MyLogger:
+    def __init__(self):
+        logging.basicConfig(level=logging.INFO,
+                            format=' %(asctime)s - %(levelname)s - %(message)s')
+
+    def get_logger(self, name=None):
+        return logging.getLogger(name)
+
+
+def get_default_logger():
+    return MyLogger().get_logger()
+
+
+def log_timer(_func=None, *, my_logger: Union[MyLogger, logging.Logger] = None):
+    def decorator_log(func):
+        @functools.wraps(func)
+        def wrapper(*args, **kwargs):
+            logger = get_default_logger()
+            try:
+                if my_logger is None:
+                    first_args = next(iter(args), None)  # capture first arg to check for `self`
+                    logger_params = [  # does kwargs have any logger
+                                        x
+                                        for x in kwargs.values()
+                                        if isinstance(x, logging.Logger) or isinstance(x, MyLogger)
+                                    ] + [  # # does args have any logger
+                                        x
+                                        for x in args
+                                        if isinstance(x, logging.Logger) or isinstance(x, MyLogger)
+                                    ]
+                    if hasattr(first_args, "__dict__"):  # is first argument `self`
+                        logger_params = logger_params + [
+                            x
+                            for x in first_args.__dict__.values()  # does class (dict) members have any logger
+                            if isinstance(x, logging.Logger)
+                               or isinstance(x, MyLogger)
+                        ]
+                    h_logger = next(iter(logger_params), MyLogger())  # get the next/first/default logger
+                else:
+                    h_logger = my_logger  # logger is passed explicitly to the decorator
+
+                if isinstance(h_logger, MyLogger):
+                    logger = h_logger.get_logger(func.__name__)
+                else:
+                    logger = h_logger
+
+                # args_repr = [repr(a) for a in args]
+                # kwargs_repr = [f"{k}={v!r}" for k, v in kwargs.items()]
+                # signature = ", ".join(args_repr + kwargs_repr)
+                # logger.debug(f"function {func.__name__} called with args {signature}")
+
+            except Exception:
+                pass
+
+            try:
+                _tic = datetime.now()
+                result = func(*args, **kwargs)
+                _toc = datetime.now()
+                logger.info(f"Elapsed time for {func.__name__}: {_toc - _tic}")
+                return result
+            except Exception as e:
+                logger.exception(f"Exception raised in {func.__name__}. exception: {str(e)}")
+                raise e
+
+        return wrapper
+
+    if _func is None:
+        return decorator_log
+    else:
+        return decorator_log(_func)
```

### Comparing `sklearn_viz-0.4.2/LICENSE` & `sklearn_viz-0.4.9/LICENSE`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Greg Elphick
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Greg Elphick
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `sklearn_viz-0.4.2/pyproject.toml` & `sklearn_viz-0.4.9/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-[tool.poetry]
-name = "sklearn-viz"
-version = "0.4.2"
-description = ""
-authors = ["Greg <11791585+elphick@users.noreply.github.com>"]
-readme = "README.md"
-packages = [{ include = "elphick/sklearn_viz" }]
-
-[[tool.poetry.source]]
-name = "PyPI"
-priority = "primary"
-
-[tool.poetry.dependencies]
-python = ">=3.8,<3.12"
-scikit-learn = ">=1.2.0"
-pandas = ">=1.3.0"
-matplotlib = "^3.7.2"
-plotly = "^5.15.0"
-statsmodels = "^0.14.0"
-
-[tool.poetry.group.dev.dependencies]
-pytest = "^7.1.3"
-sphinx = "^5.0.2"
-sphinx-rtd-theme = "^1.0.0"
-sphinx-gallery = "^0.11.1"
-sphinx-autodoc-typehints = "^1.18.3"
-myst-parser = "^0.18.0"
-kaleido = "0.2.1"  # For plotly thumbnails
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "sklearn-viz"
+version = "0.4.9"
+description = ""
+authors = ["Greg <11791585+elphick@users.noreply.github.com>"]
+readme = "README.md"
+packages = [{ include = "elphick/sklearn_viz" }]
+
+[[tool.poetry.source]]
+name = "PyPI"
+priority = "primary"
+
+[tool.poetry.dependencies]
+python = ">=3.8,<3.12"
+scikit-learn = ">=1.2.0"
+pandas = ">=1.3.0"
+matplotlib = "^3.7.2"
+plotly = "^5.15.0"
+statsmodels = "^0.14.0"
+
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.1.3"
+sphinx = "^5.0.2"
+sphinx-rtd-theme = "^1.0.0"
+sphinx-gallery = "^0.11.1"
+sphinx-autodoc-typehints = "^1.18.3"
+myst-parser = "^0.18.0"
+kaleido = "0.2.1"  # For plotly thumbnails
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `sklearn_viz-0.4.2/PKG-INFO` & `sklearn_viz-0.4.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklearn-viz
-Version: 0.4.2
+Version: 0.4.9
 Summary: 
 Author: Greg
 Author-email: 11791585+elphick@users.noreply.github.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

