# Comparing `tmp/l4v1-0.0.2.tar.gz` & `tmp/l4v1-0.1.0.tar.gz`

## Comparing `l4v1-0.0.2.tar` & `l4v1-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,24 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 l4v1-0.0.2/.python-version
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 l4v1-0.0.2/TESTING.py
--rw-r--r--   0        0        0     5170 2020-02-02 00:00:00.000000 l4v1-0.0.2/requirements-dev.lock
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 l4v1-0.0.2/requirements.lock
--rw-r--r--   0        0        0    42532 2020-02-02 00:00:00.000000 l4v1-0.0.2/data/supermarket_sales.parquet
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 l4v1-0.0.2/l4v1/__init__.py
--rw-r--r--   0        0        0    14772 2020-02-02 00:00:00.000000 l4v1-0.0.2/l4v1/impact_analysis.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 l4v1-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 l4v1-0.0.2/tests/test_price_volume_mix.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 l4v1-0.0.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 l4v1-0.0.2/LICENSE
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 l4v1-0.0.2/README.md
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 l4v1-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 l4v1-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 l4v1-0.1.0/.python-version
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 l4v1-0.1.0/.readthedocs.yml
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 l4v1-0.1.0/TESTING.py
+-rw-r--r--   0        0        0     5843 2020-02-02 00:00:00.000000 l4v1-0.1.0/requirements-dev.lock
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 l4v1-0.1.0/requirements.lock
+-rw-r--r--   0        0        0    42532 2020-02-02 00:00:00.000000 l4v1-0.1.0/data/supermarket_sales.parquet
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 l4v1-0.1.0/docs/Makefile
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 l4v1-0.1.0/docs/conf.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 l4v1-0.1.0/docs/documentation.rst
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 l4v1-0.1.0/docs/impact_analysis.rst
+-rw-r--r--   0        0        0    64866 2020-02-02 00:00:00.000000 l4v1-0.1.0/docs/impact_plot_example.png
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 l4v1-0.1.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 l4v1-0.1.0/docs/make.bat
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 l4v1-0.1.0/docs/requirements.txt
+-rw-r--r--   0        0        0  3744764 2020-02-02 00:00:00.000000 l4v1-0.1.0/docs/quick_start/quick_start.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 l4v1-0.1.0/l4v1/__init__.py
+-rw-r--r--   0        0        0    15002 2020-02-02 00:00:00.000000 l4v1-0.1.0/l4v1/impact_analysis.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 l4v1-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 l4v1-0.1.0/tests/test_price_volume_mix.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 l4v1-0.1.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 l4v1-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 l4v1-0.1.0/README.md
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 l4v1-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 l4v1-0.1.0/PKG-INFO
```

### Comparing `l4v1-0.0.2/TESTING.py` & `l4v1-0.1.0/TESTING.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,22 +4,25 @@
 df = pl.scan_parquet("data/supermarket_sales.parquet").with_columns(
     pl.col(pl.Categorical).cast(pl.Utf8)
 )
 
 sales_week5 = df.filter(pl.col("Datetime").dt.week() == 5)
 sales_week6 = df.filter(pl.col("Datetime").dt.week() == 6)
 
-impact_table_df = impact_table(
+impact_df = impact_table(
     df_primary=sales_week6,
     df_comparison=sales_week5,
-    group_by_columns=["Branch", "Product line"],
+    group_by_columns=["Product line"],
     volume_metric_name="Quantity",
     outcome_metric_name="Total",
 )
 
 impact_plot(
-    impact_table=impact_table_df,
-    format_data_labels="{:,.0f}",
-    primary_total_label="Test1",
-    comparison_total_label="Test2",
-    title="Detailed Impact Analysis"
+    impact_table=impact_df,
+    format_data_labels="{:,.0f}€", # Optional
+    primary_total_label="Revenue Week 2", # Optional
+    comparison_total_label="Revenue Week 1", # Optional
+    title="Impact Analysis Example", # Optional title
+    color_total="lightgray", # Optional for total colors
+    color_increase="#00AF00", # Optional for increase color
+    color_decrease="#FF0000" # Optional for decrease color
 )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `l4v1-0.0.2/requirements-dev.lock` & `l4v1-0.1.0/requirements-dev.lock`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 # last locked with the following flags:
 #   pre: false
 #   features: []
 #   all-features: false
 #   with-sources: false
 
 -e file:.
+alabaster==0.7.16
+    # via sphinx
 anyio==4.3.0
     # via httpx
     # via jupyter-server
 argon2-cffi==23.1.0
     # via jupyter-server
 argon2-cffi-bindings==21.2.0
     # via argon2-cffi
@@ -22,14 +24,15 @@
 async-lru==2.0.4
     # via jupyterlab
 attrs==23.2.0
     # via jsonschema
     # via referencing
 babel==2.14.0
     # via jupyterlab-server
+    # via sphinx
 beautifulsoup4==4.12.3
     # via nbconvert
 bleach==6.1.0
     # via nbconvert
 certifi==2024.2.2
     # via httpcore
     # via httpx
@@ -42,14 +45,17 @@
     # via ipykernel
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 defusedxml==0.7.1
     # via nbconvert
+docutils==0.21.1
+    # via nbsphinx
+    # via sphinx
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
 fqdn==1.5.1
     # via jsonschema
 h11==0.14.0
@@ -59,27 +65,32 @@
 httpx==0.27.0
     # via jupyterlab
 idna==3.7
     # via anyio
     # via httpx
     # via jsonschema
     # via requests
+imagesize==1.4.1
+    # via sphinx
+install==1.3.5
 ipykernel==6.29.4
     # via jupyterlab
 ipython==8.23.0
     # via ipykernel
 isoduration==20.11.0
     # via jsonschema
 jedi==0.19.1
     # via ipython
 jinja2==3.1.3
     # via jupyter-server
     # via jupyterlab
     # via jupyterlab-server
     # via nbconvert
+    # via nbsphinx
+    # via sphinx
 json5==0.9.25
     # via jupyterlab-server
 jsonpointer==2.4
     # via jsonschema
 jsonschema==4.21.1
     # via jupyter-events
     # via jupyterlab-server
@@ -122,31 +133,35 @@
     # via ipython
 mistune==3.0.2
     # via nbconvert
 nbclient==0.10.0
     # via nbconvert
 nbconvert==7.16.3
     # via jupyter-server
+    # via nbsphinx
 nbformat==5.10.4
     # via jupyter-server
     # via nbclient
     # via nbconvert
+    # via nbsphinx
+nbsphinx==0.9.3
 nest-asyncio==1.6.0
     # via ipykernel
 notebook-shim==0.2.4
     # via jupyterlab
 overrides==7.7.0
     # via jupyter-server
 packaging==24.0
     # via ipykernel
     # via jupyter-server
     # via jupyterlab
     # via jupyterlab-server
     # via nbconvert
     # via plotly
+    # via sphinx
 pandocfilters==1.5.1
     # via nbconvert
 parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
 platformdirs==4.2.0
@@ -167,14 +182,15 @@
 pure-eval==0.2.2
     # via stack-data
 pycparser==2.22
     # via cffi
 pygments==2.17.2
     # via ipython
     # via nbconvert
+    # via sphinx
 python-dateutil==2.9.0.post0
     # via arrow
     # via jupyter-client
 python-json-logger==2.0.7
     # via jupyter-events
 pyyaml==6.0.1
     # via jupyter-events
@@ -184,14 +200,15 @@
     # via jupyter-server
 referencing==0.34.0
     # via jsonschema
     # via jsonschema-specifications
     # via jupyter-events
 requests==2.31.0
     # via jupyterlab-server
+    # via sphinx
 rfc3339-validator==0.1.4
     # via jsonschema
     # via jupyter-events
 rfc3986-validator==0.1.1
     # via jsonschema
     # via jupyter-events
 rpds-py==0.18.0
@@ -203,16 +220,32 @@
     # via asttokens
     # via bleach
     # via python-dateutil
     # via rfc3339-validator
 sniffio==1.3.1
     # via anyio
     # via httpx
+snowballstemmer==2.2.0
+    # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
+sphinx==7.3.7
+    # via nbsphinx
+sphinxcontrib-applehelp==1.0.8
+    # via sphinx
+sphinxcontrib-devhelp==1.0.6
+    # via sphinx
+sphinxcontrib-htmlhelp==2.0.5
+    # via sphinx
+sphinxcontrib-jsmath==1.0.1
+    # via sphinx
+sphinxcontrib-qthelp==1.0.7
+    # via sphinx
+sphinxcontrib-serializinghtml==1.1.10
+    # via sphinx
 stack-data==0.6.3
     # via ipython
 tenacity==8.2.3
     # via plotly
 terminado==0.18.1
     # via jupyter-server
     # via jupyter-server-terminals
@@ -233,14 +266,15 @@
     # via jupyter-events
     # via jupyter-server
     # via jupyterlab
     # via matplotlib-inline
     # via nbclient
     # via nbconvert
     # via nbformat
+    # via nbsphinx
 types-python-dateutil==2.9.0.20240316
     # via arrow
 uri-template==1.3.0
     # via jsonschema
 urllib3==2.2.1
     # via requests
 wcwidth==0.2.13
```

### Comparing `l4v1-0.0.2/data/supermarket_sales.parquet` & `l4v1-0.1.0/data/supermarket_sales.parquet`

 * *Files identical despite different names*

### Comparing `l4v1-0.0.2/l4v1/impact_analysis.py` & `l4v1-0.1.0/l4v1/impact_analysis.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import polars as pl
 import polars.selectors as cs
 import plotly.graph_objects as go
-from typing import Any, Callable, Dict, List, Tuple, Union, Optional
+from typing import Callable
 
 
 def _group_dataframe(
     lf: pl.LazyFrame,
-    group_by_columns: List[str],
-    metric_names: List[str],
+    group_by_columns: list[str],
+    metric_names: list[str],
 ) -> pl.LazyFrame:
     transformed_cols = [
         pl.col(col_name).cast(pl.Utf8).alias(col_name) for col_name in group_by_columns
     ]
     agg_expressions = [pl.col(metric).sum().cast(pl.Float64) for metric in metric_names]
     return lf.group_by(transformed_cols).agg(agg_expressions)
 
 
-def _get_join_key_expression(group_by_columns: List[str]) -> pl.Expr:
+def _get_join_key_expression(group_by_columns: list[str]) -> pl.Expr:
     group_keys = list()
 
     for join_key in group_by_columns:
         temp_expr = (
             pl.when(pl.col(join_key).is_null())
             .then(pl.col(f"{join_key}_comparison"))
             .otherwise(join_key)
@@ -33,15 +33,15 @@
 
     return expr
 
 
 def _get_impact_expressions(
     volume_metric_name: str,
     outcome_metric_name: str,
-) -> Tuple[pl.Expr, pl.Expr, pl.Expr, pl.Expr, pl.Expr]:
+) -> tuple[pl.Expr, pl.Expr, pl.Expr, pl.Expr, pl.Expr]:
     # Volume
     volume_new = pl.col(volume_metric_name)
     volume_comparison = pl.col(f"{volume_metric_name}_comparison")
     volume_diff = volume_new - volume_comparison
 
     # Outcome
     outcome_new = pl.col(outcome_metric_name)
@@ -89,30 +89,30 @@
         mix_impact_expr,
         new_impact,
         old_impact,
     )
 
 
 def impact_table(
-    df_primary: Union[pl.LazyFrame, pl.DataFrame],
-    df_comparison: Union[pl.LazyFrame, pl.DataFrame],
-    group_by_columns: Union[str, List[str]],
+    df_primary: pl.LazyFrame | pl.DataFrame,
+    df_comparison: pl.LazyFrame | pl.DataFrame,
+    group_by_columns: str | list[str],
     volume_metric_name: str,
     outcome_metric_name: str,
 ) -> pl.DataFrame:
     """
     Generates a table with impact analysis results from primary and comparison data frames.
 
     Parameters
     ----------
-    df_primary : Union[pl.LazyFrame, pl.DataFrame]
+    df_primary : pl.LazyFrame | pl.DataFrame
         The primary dataset to analyze.
-    df_comparison : Union[pl.LazyFrame, pl.DataFrame]
+    df_comparison : pl.LazyFrame | pl.DataFrame
         The dataset to compare against the primary dataset.
-    group_by_columns : Union[str, List[str]]
+    group_by_columns : str | list[str]
         Column name(s) used to group data. Can be a single column name or a list of names.
     volume_metric_name : str
         The name of the column in the data frame that represents the volume metric.
     outcome_metric_name : str
         The name of the column in the data frame that represents the outcome metric.
 
     Returns
@@ -121,15 +121,35 @@
         A Polars DataFrame containing the results of the impact analysis.
 
     Raises
     ------
     TypeError
         If the input data frames are not Polars DataFrame or LazyFrame types.
     ValueError
-        If any of the parameters are missing or if the 'group_by_columns' contains non-string types.
+        If any of the parameters are incorrect or if the 'group_by_columns' contains non-string types.
+
+    Examples
+    --------
+    Here's how you can use the `impact_table` to compare sales data between two periods:
+
+    >>> import polars as pl
+    >>> from l4v1 import impact_table
+
+    >>> sales_week_1 = pl.read_csv("sales_week_1.csv")
+    >>> sales_week_2 = pl.read_csv("sales_week_2.csv")
+
+    >>> impact_df = impact_table(
+    >>>     df_primary=sales_week_2,
+    >>>     df_comparison=sales_week_1,
+    >>>     group_by_columns="product_category",
+    >>>     volume_metric_name="units_sold",
+    >>>     outcome_metric_name="total_revenue"
+    >>> )
+
+    >>> print(impact_df)
     """
     # Ensure polars df type and convert to lazy
     if not all(
         isinstance(item, (pl.LazyFrame, pl.DataFrame))
         for item in (df_primary, df_comparison)
     ):
         raise TypeError(
@@ -218,29 +238,29 @@
 
 
 def _prep_data_for_impact_plot(
     impact_table: pl.DataFrame,
     format_data_labels: Callable,
     primary_total_label: str,
     comparison_total_label: str,
-) -> Tuple[list, list, list, list]:
+) -> tuple[list, list, list, list]:
     _, outcome_metric_name = _parse_metric_column_names(impact_table)
     if format_data_labels is None:
         format_data_labels = lambda value: f"{value:,.0f}"
     primary_total_label = primary_total_label or outcome_metric_name
     comparison_total_label = (
         comparison_total_label or f"COMPARISON {outcome_metric_name}"
     )
 
     x_labels, y_values, data_labels, measure_list = [], [], [], []
     outcome_comparison = impact_table.get_column(
         f"{outcome_metric_name}_comparison"
     ).sum()
 
-    x_labels.append(f"<b>{comparison_total_label}</b>".upper())
+    x_labels.append(f"<b>{comparison_total_label}</b>")
     y_values.append(outcome_comparison)
     data_labels.append(f"<b>{format_data_labels(outcome_comparison)}</b>")
     measure_list.append("absolute")
 
     cumulative_sum = outcome_comparison
     previous_value = outcome_comparison
 
@@ -269,91 +289,99 @@
         data_labels.append(
             _create_data_label(cumulative_sum, previous_value, format_data_labels)
         )
         measure_list.append("absolute")
         previous_value = cumulative_sum
 
     outcome_new = impact_table.get_column(outcome_metric_name).sum()
-    x_labels.append(f"<b>{primary_total_label}</b>".upper())
+    x_labels.append(f"<b>{primary_total_label}</b>")
     y_values.append(outcome_new)
     data_labels.append(
         f"<b>{_create_data_label(outcome_new, outcome_comparison, format_data_labels)}</b>"
     )
     measure_list.append("total")
 
     return x_labels, y_values, data_labels, measure_list
 
 
 def impact_plot(
     impact_table: pl.DataFrame,
-    primary_total_label: Optional[str] = None,
-    comparison_total_label: Optional[str] = None,
-    format_data_labels: Optional[str] = "{:,.0f}",
-    title: Optional[str] = None,
-    color_increase: Optional[str] = "#00AF00",
-    color_decrease: Optional[str] = "#FF0000",
-    color_total: Optional[str] = "#F1F1F1",
-    text_font_size: Optional[int] = 8,
-    plot_height: Optional[int] = None,
-    plot_width: Optional[int] = 750,
-    plotly_template: Optional[str] = "plotly_white",
-    plotly_trace_settings: Optional[Dict[str, Any]] = None,
-    plotly_layout_settings: Optional[Dict[str, Any]] = None,
+    primary_total_label: str = None,
+    comparison_total_label: str = None,
+    format_data_labels: str = "{:,.0f}",
+    title: str = None,
+    color_increase: str = "#00AF00",
+    color_decrease: str = "#FF0000",
+    color_total: str = "#F1F1F1",
+    text_font_size: int = 8,
+    plot_height: int = None,
+    plot_width: int = 750,
+    plotly_template: str = "plotly_white",
+    plotly_trace_settings: dict[str, any] = None,
+    plotly_layout_settings: dict[str, any] = None,
 ) -> go.Figure:
     """
     Creates a waterfall plot visualizing the impact analysis results.
 
     Parameters
     ----------
     impact_table : pl.DataFrame
         The DataFrame containing impact analysis results, as returned by the `impact_table` function.
-    primary_total_label : str, optional
-        Label for the total of the primary data set in the plot. Defaults to the outcome metric name.
-    comparison_total_label : str, optional
-        Label for the total of the comparison data set in the plot. Defaults to "COMPARISON <outcome_metric_name>".
+    primary_total_label : str | None, optional
+        Label for the total of the primary dataset in the plot. Defaults to the outcome metric name.
+    comparison_total_label : str | None, optional
+        Label for the total of the comparison dataset in the plot. Defaults to "COMPARISON <outcome_metric_name>".
     format_data_labels : str, optional
-        Format specification for the data labels. Defaults to "{:,.0f}". This should be a string
-        following Python's string formatting syntax, which allows custom numeric formatting, e.g.,
-        "{:.2f}" for floating-point numbers with two decimals, or "{:,.2f}" for numbers with commas
-        as thousands separators and two decimals.
-    title : str, optional
+        Format specification for the data labels. Defaults to "{:,.0f}".
+    title : str | None, optional
         The title of the plot.
     color_increase : str, optional
-        Color for positive changes. Can be specified as a hexadecimal code (e.g., "#00AF00") or
-        a named Plotly color (e.g., "green"). Defaults to green "#00AF00".
+        Color for positive changes. Can be specified as a hexadecimal code or a named Plotly color.
     color_decrease : str, optional
-        Color for negative changes. Can be specified as a hexadecimal code (e.g., "#FF0000") or
-        a named Plotly color (e.g., "red"). Defaults to red "#FF0000".
+        Color for negative changes. Can be specified as a hexadecimal code or a named Plotly color.
     color_total : str, optional
-        Color for total columns. Can be specified as a hexadecimal code (e.g., "#F1F1F1") or
-        a named Plotly color (e.g., "grey"). Defaults to light gray "#F1F1F1".
+        Color for total columns. Can be specified as a hexadecimal code or a named Plotly color.
     text_font_size : int, optional
-        Font size of the text in the plot. Defaults to 8.
-    plot_height : int, optional
-        Height of the plot in pixels. Calculated based on the number of labels if not provided.
+        Font size of the text in the plot.
+    plot_height : int | None, optional
+        Height of the plot in pixels, calculated based on the number of labels if not provided.
     plot_width : int, optional
-        Width of the plot in pixels. Defaults to 750.
+        Width of the plot in pixels.
     plotly_template : str, optional
-        The Plotly template to use for the plot styling. Defaults to "plotly_white".
-    plotly_trace_settings : Dict[str, Any], optional
+        The Plotly template to use for the plot styling.
+    plotly_trace_settings : dict[str, any] | None, optional
         Additional trace settings for advanced customization using Plotly's trace options.
-    plotly_layout_settings : Dict[str, Any], optional
+    plotly_layout_settings : dict[str, any] | None, optional
         Additional layout settings for advanced customization using Plotly's layout options.
 
     Returns
     -------
     go.Figure
         A Plotly Figure object representing the impact analysis as a waterfall chart.
 
-    Raises
-    ------
-    TypeError
-        If `impact_table` is not a Polars DataFrame.
-    ValueError
-        If no columns with '_comparison' are found in `impact_table`.
+    Examples
+    --------
+    Here's how to visualize the impact of sales volume on revenue:
+
+    >>> import polars as pl
+    >>> from l4v1 import impact_table, impact_plot
+
+    >>> sales_week_1 = pl.read_csv("sales_week_1.csv")
+    >>> sales_week_2 = pl.read_csv("sales_week_2.csv")
+
+    >>> impact_df = impact_table(
+    >>>    df_primary=sales_week_2,
+    >>>    df_comparison=sales_week_1,
+    >>>    ["product_category"],
+    >>>    "units_sold",
+    >>>    "total_revenue",
+    >>> )
+
+    >>> fig = impact_plot(impact_df)
+    >>> fig.show()
     """
     if not isinstance(impact_table, pl.DataFrame):
         raise TypeError("impact_table must be Polars DataFrame")
 
     # Check for columns containing "_comparison" in the impact table
     comparison_columns = [col for col in impact_table.columns if "_comparison" in col]
     if not comparison_columns:
```

### Comparing `l4v1-0.0.2/tests/test_price_volume_mix.py` & `l4v1-0.1.0/tests/test_price_volume_mix.py`

 * *Files identical despite different names*

### Comparing `l4v1-0.0.2/.gitignore` & `l4v1-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `l4v1-0.0.2/LICENSE` & `l4v1-0.1.0/LICENSE`

 * *Files identical despite different names*

