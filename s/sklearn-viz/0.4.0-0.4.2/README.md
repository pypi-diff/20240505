# Comparing `tmp/sklearn_viz-0.4.0.tar.gz` & `tmp/sklearn_viz-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklearn_viz-0.4.0.tar", max compression
+gzip compressed data, was "sklearn_viz-0.4.2.tar", max compression
```

## Comparing `sklearn_viz-0.4.0.tar` & `sklearn_viz-0.4.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0        0 2023-08-27 06:10:46.929402 sklearn_viz-0.4.0/elphick/sklearn_viz/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 12:00:29.935280 sklearn_viz-0.4.0/elphick/sklearn_viz/components/__init__.py
--rw-r--r--   0        0        0     4482 2024-04-08 12:00:29.940581 sklearn_viz-0.4.0/elphick/sklearn_viz/components/estimators.py
--rw-r--r--   0        0        0      334 2023-09-18 13:02:51.287832 sklearn_viz-0.4.0/elphick/sklearn_viz/features/__init__.py
--rw-r--r--   0        0        0     8495 2024-04-08 12:00:29.951129 sklearn_viz-0.4.0/elphick/sklearn_viz/features/importance.py
--rw-r--r--   0        0        0     4738 2024-03-30 11:59:00.677281 sklearn_viz-0.4.0/elphick/sklearn_viz/features/outlier_detection.py
--rw-r--r--   0        0        0     2471 2024-03-30 11:59:00.682932 sklearn_viz-0.4.0/elphick/sklearn_viz/features/parallel_coordinates.py
--rw-r--r--   0        0        0    16988 2024-03-30 11:59:00.688949 sklearn_viz-0.4.0/elphick/sklearn_viz/features/principal_components.py
--rw-r--r--   0        0        0      668 2023-09-18 11:19:59.559906 sklearn_viz-0.4.0/elphick/sklearn_viz/features/scatter_matrix.py
--rw-r--r--   0        0        0      131 2023-09-18 13:02:51.313708 sklearn_viz-0.4.0/elphick/sklearn_viz/model_selection/__init__.py
--rw-r--r--   0        0        0     6246 2023-09-11 12:55:18.110947 sklearn_viz-0.4.0/elphick/sklearn_viz/model_selection/learning_curve.py
--rw-r--r--   0        0        0     1622 2024-04-08 12:00:29.961992 sklearn_viz-0.4.0/elphick/sklearn_viz/model_selection/metrics.py
--rw-r--r--   0        0        0    21106 2024-04-08 12:00:29.972985 sklearn_viz-0.4.0/elphick/sklearn_viz/model_selection/model_selection.py
--rw-r--r--   0        0        0     2552 2023-09-11 12:55:18.114966 sklearn_viz-0.4.0/elphick/sklearn_viz/model_selection/models.py
--rw-r--r--   0        0        0      526 2024-04-08 12:00:29.983221 sklearn_viz-0.4.0/elphick/sklearn_viz/model_selection/scorers.py
--rw-r--r--   0        0        0       22 2023-09-17 08:40:15.220711 sklearn_viz-0.4.0/elphick/sklearn_viz/residuals/__init__.py
--rw-r--r--   0        0        0     2120 2023-09-05 09:52:35.543294 sklearn_viz-0.4.0/elphick/sklearn_viz/residuals/error.py
--rw-r--r--   0        0        0       28 2023-08-27 06:10:46.931314 sklearn_viz-0.4.0/elphick/sklearn_viz/utils/__init__.py
--rw-r--r--   0        0        0     3191 2023-08-27 06:10:46.931314 sklearn_viz-0.4.0/elphick/sklearn_viz/utils/timer.py
--rw-r--r--   0        0        0     1090 2023-08-27 06:10:46.917578 sklearn_viz-0.4.0/LICENSE
--rw-r--r--   0        0        0      819 2024-04-08 12:00:29.999523 sklearn_viz-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      362 2023-08-27 06:10:46.918992 sklearn_viz-0.4.0/README.md
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 sklearn_viz-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-27 06:10:46.929402 sklearn_viz-0.4.2/elphick/sklearn_viz/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 02:07:15.153023 sklearn_viz-0.4.2/elphick/sklearn_viz/components/__init__.py
+-rw-r--r--   0        0        0     4482 2024-04-24 02:07:15.158894 sklearn_viz-0.4.2/elphick/sklearn_viz/components/estimators.py
+-rw-r--r--   0        0        0      833 2024-05-05 05:33:50.775128 sklearn_viz-0.4.2/elphick/sklearn_viz/components/kfold.py
+-rw-r--r--   0        0        0      334 2023-09-18 13:02:51.287832 sklearn_viz-0.4.2/elphick/sklearn_viz/features/__init__.py
+-rw-r--r--   0        0        0     8495 2024-04-24 02:07:15.169404 sklearn_viz-0.4.2/elphick/sklearn_viz/features/importance.py
+-rw-r--r--   0        0        0     4738 2024-03-30 11:59:00.677281 sklearn_viz-0.4.2/elphick/sklearn_viz/features/outlier_detection.py
+-rw-r--r--   0        0        0     2471 2024-03-30 11:59:00.682932 sklearn_viz-0.4.2/elphick/sklearn_viz/features/parallel_coordinates.py
+-rw-r--r--   0        0        0    16988 2024-03-30 11:59:00.688949 sklearn_viz-0.4.2/elphick/sklearn_viz/features/principal_components.py
+-rw-r--r--   0        0        0      668 2023-09-18 11:19:59.559906 sklearn_viz-0.4.2/elphick/sklearn_viz/features/scatter_matrix.py
+-rw-r--r--   0        0        0      131 2023-09-18 13:02:51.313708 sklearn_viz-0.4.2/elphick/sklearn_viz/model_selection/__init__.py
+-rw-r--r--   0        0        0     6246 2023-09-11 12:55:18.110947 sklearn_viz-0.4.2/elphick/sklearn_viz/model_selection/learning_curve.py
+-rw-r--r--   0        0        0     1622 2024-04-24 02:07:15.180268 sklearn_viz-0.4.2/elphick/sklearn_viz/model_selection/metrics.py
+-rw-r--r--   0        0        0    21968 2024-05-05 05:33:50.780670 sklearn_viz-0.4.2/elphick/sklearn_viz/model_selection/model_selection.py
+-rw-r--r--   0        0        0     2552 2023-09-11 12:55:18.114966 sklearn_viz-0.4.2/elphick/sklearn_viz/model_selection/models.py
+-rw-r--r--   0        0        0      526 2024-04-24 02:07:15.200590 sklearn_viz-0.4.2/elphick/sklearn_viz/model_selection/scorers.py
+-rw-r--r--   0        0        0       22 2023-09-17 08:40:15.220711 sklearn_viz-0.4.2/elphick/sklearn_viz/residuals/__init__.py
+-rw-r--r--   0        0        0     2120 2023-09-05 09:52:35.543294 sklearn_viz-0.4.2/elphick/sklearn_viz/residuals/error.py
+-rw-r--r--   0        0        0       28 2023-08-27 06:10:46.931314 sklearn_viz-0.4.2/elphick/sklearn_viz/utils/__init__.py
+-rw-r--r--   0        0        0     3191 2023-08-27 06:10:46.931314 sklearn_viz-0.4.2/elphick/sklearn_viz/utils/timer.py
+-rw-r--r--   0        0        0     1090 2023-08-27 06:10:46.917578 sklearn_viz-0.4.2/LICENSE
+-rw-r--r--   0        0        0      772 2024-05-05 07:42:05.636098 sklearn_viz-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      362 2023-08-27 06:10:46.918992 sklearn_viz-0.4.2/README.md
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 sklearn_viz-0.4.2/PKG-INFO
```

### Comparing `sklearn_viz-0.4.0/elphick/sklearn_viz/components/estimators.py` & `sklearn_viz-0.4.2/elphick/sklearn_viz/components/estimators.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.4.0/elphick/sklearn_viz/features/importance.py` & `sklearn_viz-0.4.2/elphick/sklearn_viz/features/importance.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.4.0/elphick/sklearn_viz/features/outlier_detection.py` & `sklearn_viz-0.4.2/elphick/sklearn_viz/features/outlier_detection.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.4.0/elphick/sklearn_viz/features/parallel_coordinates.py` & `sklearn_viz-0.4.2/elphick/sklearn_viz/features/parallel_coordinates.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.4.0/elphick/sklearn_viz/features/principal_components.py` & `sklearn_viz-0.4.2/elphick/sklearn_viz/features/principal_components.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.4.0/elphick/sklearn_viz/features/scatter_matrix.py` & `sklearn_viz-0.4.2/elphick/sklearn_viz/features/scatter_matrix.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.4.0/elphick/sklearn_viz/model_selection/learning_curve.py` & `sklearn_viz-0.4.2/elphick/sklearn_viz/model_selection/learning_curve.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.4.0/elphick/sklearn_viz/model_selection/metrics.py` & `sklearn_viz-0.4.2/elphick/sklearn_viz/model_selection/metrics.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.4.0/elphick/sklearn_viz/model_selection/model_selection.py` & `sklearn_viz-0.4.2/elphick/sklearn_viz/model_selection/model_selection.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,17 @@
 
     return ModelSelection(algorithms=algorithms, datasets=datasets, target=target, pre_processor=pre_processor,
                           k_folds=k_folds).plot(title=title)
 
 
 class ModelSelection:
     def __init__(self,
-                 algorithms: Union[sklearn.base.RegressorMixin, sklearn.base.ClassifierMixin, Dict],
-                 datasets: Union[pd.DataFrame, Dict],
+                 algorithms: Union[
+                     sklearn.base.RegressorMixin, sklearn.base.ClassifierMixin, Dict[str, sklearn.base.BaseEstimator]],
+                 datasets: Union[pd.DataFrame, Dict[str, pd.DataFrame]],
                  target: str,
                  pre_processor: Optional[Pipeline] = None,
                  k_folds: int = 10,
                  scorer: Optional[Union[str, Callable]] = None,
                  metrics: Optional[Dict[str, Callable]] = None,
                  group: Optional[pd.Series] = None,
                  random_state: Optional[int] = None):
@@ -151,14 +152,19 @@
     def plot(self,
              metrics: Optional[Union[str, List[str]]] = None,
              show_group: bool = False,
              title: Optional[str] = None,
              col_wrap: Optional[int] = None) -> go.Figure:
         """Create the plot
 
+        The plot will show the cross-validation scores for each algorithm and dataset.  The first panel is used to show
+        the scorer, that is the metric used to fit the model.  If multiple metrics are supplied, each metric will be
+        shown in a separate panel.  If a show_group is true, the metrics will be grouped by the group variable.
+        col_wrap allows the width of the plot to be controlled by wrapping the columns to new rows.
+
         KUDOS: https://towardsdatascience.com/applying-a-custom-colormap-with-plotly-boxplots-5d3acf59e193
 
         Args:
             metrics: The metric or metrics to plot in addition to the scorer.  Each metric will be plotted in a
              separate panel.
             show_group: If True (and a group variable has been set), plot by group.
             title: Title of the plot
@@ -183,58 +189,63 @@
             metrics = []
 
         if self._num_algorithms > 1:
             x_index = 'algo_key'
         else:
             x_index = 'data_key'
 
+        # define the color map for the scorer
         vmin, vmax = data.min().min(), data.max().max()
         norm = matplotlib.colors.Normalize(vmin=vmin, vmax=vmax)
         cmap = matplotlib.cm.get_cmap('RdYlGn')
 
         subtitle: str = f'Cross Validation folds={self.k_folds}'
         if title is None:
             title = subtitle
         else:
             title = title + '<br>' + subtitle
 
+        # create the plot, managing the shape.
         num_plots: int = len(metrics) + 1 if len(metrics) > 0 else 1
         num_cols: int = num_plots if col_wrap is None else col_wrap
         num_rows, _ = subplot_index(len(metrics), col_wrap=num_cols)
         fig = make_subplots(rows=num_rows, cols=num_cols, subplot_titles=[f'{self.scorer} (scorer)'] + metrics)
 
-        # scorer
+        # Add the scorer subplot
         for col in data.columns:
             # For the scorer build the plot by column to color individually based on score
             median = np.median(data[col])  # find the median
             color = 'rgb' + str(cmap(norm(median))[0:3])  # normalize
             fig.add_trace(go.Box(y=data[col], name=col, boxpoints='all', notched=True, fillcolor=color,
                                  line={"color": "grey"}, marker={"color": "grey"}, showlegend=False,
                                  offsetgroup='A'), row=1, col=1)
 
-        # metrics
+        # add the metric subplots
         for i, metric in enumerate(metrics):
             row, col = subplot_index(i + 1, col_wrap=num_cols)
             if show_group:
-                colorscale = colors.qualitative.Plotly
+                colorscale = colors.qualitative.Plotly + colors.qualitative.Dark24
                 add_to_legend = True if i == 0 else False
                 df_metric: pd.DataFrame = metric_data.query('metric==@metric').drop(columns=['metric'])
                 x = df_metric.index.get_level_values(x_index)
                 for g, grp in enumerate(df_metric.columns):
+                    if len(df_metric.columns) > len(colorscale):
+                        raise ValueError("Too many groups to plot")
                     fig.add_trace(go.Box(x=x, y=df_metric[grp], name=grp, boxpoints='all', notched=True,
                                          legendgroup=self.group.name,
                                          showlegend=add_to_legend,
                                          line={"color": colorscale[g]}, marker={"color": colorscale[g]},
                                          offsetgroup=str(g)), row=row, col=col)
             else:
                 df_metric: pd.DataFrame = metric_data.query('metric==@metric').drop(columns=['metric'])
                 x = list(df_metric.index.get_level_values(x_index))
                 fig.add_trace(go.Box(x=x, y=df_metric.values.ravel(), name=metric, boxpoints='all', notched=True,
                                      line={"color": "grey"}, marker={"color": "grey"}), row=row, col=col)
 
+        # finalise some display elements
         fig.update_layout(title=title, showlegend=False)
         if show_group:
             fig.update_layout(boxmode='group', showlegend=True, legend_title=self.group.name,
                               boxgroupgap=0.5, boxgap=0
                               )
 
         return fig
```

### Comparing `sklearn_viz-0.4.0/elphick/sklearn_viz/model_selection/models.py` & `sklearn_viz-0.4.2/elphick/sklearn_viz/model_selection/models.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.4.0/elphick/sklearn_viz/model_selection/scorers.py` & `sklearn_viz-0.4.2/elphick/sklearn_viz/model_selection/scorers.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.4.0/elphick/sklearn_viz/residuals/error.py` & `sklearn_viz-0.4.2/elphick/sklearn_viz/residuals/error.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.4.0/elphick/sklearn_viz/utils/timer.py` & `sklearn_viz-0.4.2/elphick/sklearn_viz/utils/timer.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.4.0/LICENSE` & `sklearn_viz-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.4.0/PKG-INFO` & `sklearn_viz-0.4.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklearn-viz
-Version: 0.4.0
+Version: 0.4.2
 Summary: 
 Author: Greg
 Author-email: 11791585+elphick@users.noreply.github.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

