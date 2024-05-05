# Comparing `tmp/Dash_tooltip-0.3.9.tar.gz` & `tmp/Dash_tooltip-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Dash_tooltip-0.3.9.tar", last modified: Wed Mar 27 04:02:26 2024, max compression
+gzip compressed data, was "Dash_tooltip-0.4.0.tar", last modified: Sun May  5 16:54:42 2024, max compression
```

## Comparing `Dash_tooltip-0.3.9.tar` & `Dash_tooltip-0.4.0.tar`

### file list

```diff
@@ -1,42 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 04:02:26.076007 Dash_tooltip-0.3.9/
--rw-rw-rw-   0        0        0       66 2023-08-23 22:05:16.000000 Dash_tooltip-0.3.9/.gitattributes
-drwxrwxrwx   0        0        0        0 2024-03-27 04:02:26.032967 Dash_tooltip-0.3.9/.github/
-drwxrwxrwx   0        0        0        0 2024-03-27 04:02:26.056828 Dash_tooltip-0.3.9/.github/workflows/
--rw-rw-rw-   0        0        0      958 2024-03-27 02:01:04.000000 Dash_tooltip-0.3.9/.github/workflows/Pytest.yml
--rw-rw-rw-   0        0        0     3555 2023-11-01 20:33:12.000000 Dash_tooltip-0.3.9/.github/workflows/codeql.yml
--rw-rw-rw-   0        0        0     2921 2023-09-30 22:16:50.000000 Dash_tooltip-0.3.9/.gitignore
--rw-rw-rw-   0        0        0     1884 2024-03-27 03:20:13.000000 Dash_tooltip-0.3.9/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0        8 2024-03-27 03:15:54.000000 Dash_tooltip-0.3.9/.python-version
-drwxrwxrwx   0        0        0        0 2024-03-27 04:02:26.061830 Dash_tooltip-0.3.9/Dash_tooltip.egg-info/
--rw-rw-rw-   0        0        0     6379 2024-03-27 04:02:25.000000 Dash_tooltip-0.3.9/Dash_tooltip.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      853 2024-03-27 04:02:26.000000 Dash_tooltip-0.3.9/Dash_tooltip.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 04:02:25.000000 Dash_tooltip-0.3.9/Dash_tooltip.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-03-27 04:02:25.000000 Dash_tooltip-0.3.9/Dash_tooltip.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-03-27 04:02:25.000000 Dash_tooltip-0.3.9/Dash_tooltip.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1081 2023-08-24 19:37:19.000000 Dash_tooltip-0.3.9/LICENSE
--rw-rw-rw-   0        0        0     6379 2024-03-27 04:02:26.076007 Dash_tooltip-0.3.9/PKG-INFO
--rw-rw-rw-   0        0        0     5667 2024-03-27 03:20:13.000000 Dash_tooltip-0.3.9/README.md
--rw-rw-rw-   0        0        0     4744 2024-03-27 02:01:04.000000 Dash_tooltip-0.3.9/dash_qt_demo.py
--rw-rw-rw-   0        0        0     5588 2024-03-27 04:02:03.000000 Dash_tooltip-0.3.9/dash_qt_demo2.py
-drwxrwxrwx   0        0        0        0 2024-03-27 04:02:26.064827 Dash_tooltip-0.3.9/dash_tooltip/
--rw-rw-rw-   0        0        0     6035 2023-11-01 20:33:12.000000 Dash_tooltip-0.3.9/dash_tooltip/__init__.py
--rw-rw-rw-   0        0        0      824 2023-10-01 01:59:27.000000 Dash_tooltip-0.3.9/dash_tooltip/config.py
--rw-rw-rw-   0        0        0     9607 2024-03-27 02:01:04.000000 Dash_tooltip-0.3.9/dash_tooltip/utils.py
--rw-rw-rw-   0        0        0    36452 2024-03-27 02:01:04.000000 Dash_tooltip-0.3.9/dash_tooltip_demo.py
--rw-rw-rw-   0        0        0      328 2023-09-30 22:16:50.000000 Dash_tooltip-0.3.9/mypy.ini
--rw-rw-rw-   0        0        0      738 2023-10-01 01:59:27.000000 Dash_tooltip-0.3.9/noxfile.py
--rw-rw-rw-   0        0        0      448 2024-03-27 03:20:13.000000 Dash_tooltip-0.3.9/requirements.txt
--rw-rw-rw-   0        0        0      216 2024-03-27 04:02:26.077225 Dash_tooltip-0.3.9/setup.cfg
--rw-rw-rw-   0        0        0     1222 2024-01-25 00:36:21.000000 Dash_tooltip-0.3.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-27 04:02:26.076007 Dash_tooltip-0.3.9/tests/
--rw-rw-rw-   0        0        0        0 2023-09-29 22:18:19.000000 Dash_tooltip-0.3.9/tests/__init__.py
--rw-rw-rw-   0        0        0     4288 2024-03-27 03:20:13.000000 Dash_tooltip-0.3.9/tests/test_11_direct_figure_in_dcc_graph.py
--rw-rw-rw-   0        0        0     3773 2024-03-27 02:01:04.000000 Dash_tooltip-0.3.9/tests/test_1_tooltip_function.py
--rw-rw-rw-   0        0        0     4941 2024-03-27 02:01:04.000000 Dash_tooltip-0.3.9/tests/test_2_tooltip_configuration.py
--rw-rw-rw-   0        0        0     5164 2024-03-27 03:20:13.000000 Dash_tooltip-0.3.9/tests/test_3_template_formating.py
--rw-rw-rw-   0        0        0     3171 2024-03-27 02:01:04.000000 Dash_tooltip-0.3.9/tests/test_4a_multiple_graph.py
--rw-rw-rw-   0        0        0     5261 2024-03-27 02:01:04.000000 Dash_tooltip-0.3.9/tests/test_4b_multiple_graph.py
--rw-rw-rw-   0        0        0      420 2023-09-29 22:32:34.000000 Dash_tooltip-0.3.9/tests/test_6_invalid_graph_id.py
--rw-rw-rw-   0        0        0     5291 2024-03-27 02:01:04.000000 Dash_tooltip-0.3.9/tests/test_7_tooltip_removal.py
--rw-rw-rw-   0        0        0     3989 2024-03-27 02:01:04.000000 Dash_tooltip-0.3.9/tests/test_8__display_click_data.py
--rw-rw-rw-   0        0        0       42 2023-09-29 22:32:34.000000 Dash_tooltip-0.3.9/tests/test_dummy.py
+drwxrwxrwx   0        0        0        0 2024-05-05 16:54:42.826097 Dash_tooltip-0.4.0/
+-rw-rw-rw-   0        0        0       66 2023-08-23 22:05:16.000000 Dash_tooltip-0.4.0/.gitattributes
+drwxrwxrwx   0        0        0        0 2024-05-05 16:54:42.793028 Dash_tooltip-0.4.0/.github/
+drwxrwxrwx   0        0        0        0 2024-05-05 16:54:42.809979 Dash_tooltip-0.4.0/.github/workflows/
+-rw-rw-rw-   0        0        0      958 2024-03-27 02:01:04.000000 Dash_tooltip-0.4.0/.github/workflows/Pytest.yml
+-rw-rw-rw-   0        0        0     3555 2023-11-01 20:33:12.000000 Dash_tooltip-0.4.0/.github/workflows/codeql.yml
+-rw-rw-rw-   0        0        0     2921 2023-09-30 22:16:50.000000 Dash_tooltip-0.4.0/.gitignore
+-rw-rw-rw-   0        0        0     1900 2024-05-05 16:49:56.000000 Dash_tooltip-0.4.0/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0        8 2024-05-05 16:49:56.000000 Dash_tooltip-0.4.0/.python-version
+drwxrwxrwx   0        0        0        0 2024-05-05 16:54:42.814114 Dash_tooltip-0.4.0/Dash_tooltip.egg-info/
+-rw-rw-rw-   0        0        0    10351 2024-05-05 16:54:42.000000 Dash_tooltip-0.4.0/Dash_tooltip.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1007 2024-05-05 16:54:42.000000 Dash_tooltip-0.4.0/Dash_tooltip.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 16:54:42.000000 Dash_tooltip-0.4.0/Dash_tooltip.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-05-05 16:54:42.000000 Dash_tooltip-0.4.0/Dash_tooltip.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-05 16:54:42.000000 Dash_tooltip-0.4.0/Dash_tooltip.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1081 2023-08-24 19:37:19.000000 Dash_tooltip-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0    10351 2024-05-05 16:54:42.826097 Dash_tooltip-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9639 2024-05-05 16:49:56.000000 Dash_tooltip-0.4.0/README.md
+-rw-rw-rw-   0        0        0     4812 2024-03-28 18:53:44.000000 Dash_tooltip-0.4.0/dash_qt_demo.py
+-rw-rw-rw-   0        0        0     5690 2024-05-05 16:49:56.000000 Dash_tooltip-0.4.0/dash_qt_demo2.py
+drwxrwxrwx   0        0        0        0 2024-05-05 16:54:42.816150 Dash_tooltip-0.4.0/dash_tooltip/
+-rw-rw-rw-   0        0        0     8349 2024-05-05 16:49:56.000000 Dash_tooltip-0.4.0/dash_tooltip/__init__.py
+-rw-rw-rw-   0        0        0      824 2023-10-01 01:59:27.000000 Dash_tooltip-0.4.0/dash_tooltip/config.py
+-rw-rw-rw-   0        0        0      343 2024-05-05 16:49:56.000000 Dash_tooltip-0.4.0/dash_tooltip/custom_figure.py
+-rw-rw-rw-   0        0        0    10410 2024-05-05 16:49:56.000000 Dash_tooltip-0.4.0/dash_tooltip/utils.py
+-rw-rw-rw-   0        0        0    39815 2024-05-05 16:49:56.000000 Dash_tooltip-0.4.0/dash_tooltip_demo.py
+-rw-rw-rw-   0        0        0      328 2023-09-30 22:16:50.000000 Dash_tooltip-0.4.0/mypy.ini
+-rw-rw-rw-   0        0        0      738 2023-10-01 01:59:27.000000 Dash_tooltip-0.4.0/noxfile.py
+-rw-rw-rw-   0        0        0      464 2024-05-05 16:49:56.000000 Dash_tooltip-0.4.0/requirements.txt
+-rw-rw-rw-   0        0        0      247 2024-05-05 16:54:42.827151 Dash_tooltip-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1222 2024-01-25 00:36:21.000000 Dash_tooltip-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 16:54:42.825103 Dash_tooltip-0.4.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-09-29 22:18:19.000000 Dash_tooltip-0.4.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     4288 2024-03-28 00:58:55.000000 Dash_tooltip-0.4.0/tests/test_11_direct_figure_in_dcc_graph.py
+-rw-rw-rw-   0        0        0     3566 2024-03-28 00:42:16.000000 Dash_tooltip-0.4.0/tests/test_12_go_scatter.py
+-rw-rw-rw-   0        0        0     3623 2024-03-28 00:42:16.000000 Dash_tooltip-0.4.0/tests/test_13_go_scatter_line.py
+-rw-rw-rw-   0        0        0     3469 2024-03-28 00:42:16.000000 Dash_tooltip-0.4.0/tests/test_14_go_bar_chart.py
+-rw-rw-rw-   0        0        0     3958 2024-05-05 16:49:56.000000 Dash_tooltip-0.4.0/tests/test_16_update_template.py
+-rw-rw-rw-   0        0        0     3773 2024-03-27 02:01:04.000000 Dash_tooltip-0.4.0/tests/test_1_tooltip_function.py
+-rw-rw-rw-   0        0        0     4941 2024-03-27 02:01:04.000000 Dash_tooltip-0.4.0/tests/test_2_tooltip_configuration.py
+-rw-rw-rw-   0        0        0     5296 2024-05-05 16:49:56.000000 Dash_tooltip-0.4.0/tests/test_3_template_formating.py
+-rw-rw-rw-   0        0        0     3171 2024-03-27 02:01:04.000000 Dash_tooltip-0.4.0/tests/test_4a_multiple_graph.py
+-rw-rw-rw-   0        0        0     5265 2024-05-05 16:49:56.000000 Dash_tooltip-0.4.0/tests/test_4b_multiple_graph.py
+-rw-rw-rw-   0        0        0      420 2023-09-29 22:32:34.000000 Dash_tooltip-0.4.0/tests/test_6_invalid_graph_id.py
+-rw-rw-rw-   0        0        0     5292 2024-05-05 16:49:56.000000 Dash_tooltip-0.4.0/tests/test_7_tooltip_removal.py
+-rw-rw-rw-   0        0        0     3963 2024-05-05 16:49:56.000000 Dash_tooltip-0.4.0/tests/test_8__display_click_data.py
+-rw-rw-rw-   0        0        0       42 2023-09-29 22:32:34.000000 Dash_tooltip-0.4.0/tests/test_dummy.py
```

### Comparing `Dash_tooltip-0.3.9/.github/workflows/Pytest.yml` & `Dash_tooltip-0.4.0/.github/workflows/Pytest.yml`

 * *Files identical despite different names*

### Comparing `Dash_tooltip-0.3.9/.github/workflows/codeql.yml` & `Dash_tooltip-0.4.0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `Dash_tooltip-0.3.9/.gitignore` & `Dash_tooltip-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `Dash_tooltip-0.3.9/.pre-commit-config.yaml` & `Dash_tooltip-0.4.0/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,68 +1,68 @@
 repos:
 -   repo: local
     hooks:
+    - id: ruff
+      name: ruff
+      description: "Run 'ruff' for extremely fast Python linting"
+      entry: ruff check --force-exclude
+      language: python
+      types_or: [python, pyi]
+      args: []
+      require_serial: true
+      additional_dependencies: []
+      minimum_pre_commit_version: "2.9.2"
+
+    - id: ruff-format
+      name: ruff-format
+      description: "Run 'ruff format' for extremely fast Python formatting"
+      entry: ruff format --force-exclude
+      language: python
+      types_or: [python, pyi]
+      args: []
+      require_serial: true
+      additional_dependencies: []
+      minimum_pre_commit_version: "2.9.2"
+
     -   id: black-fix
         name: black (auto format)
         entry: ./env/Scripts/black.exe
         language: system
         types: [python]
         
     -   id: isort-fix
         name: isort (auto sort)
         entry: ./env/Scripts/isort.exe
         language: system
         types: [python]
         
-    -   id: pytest-selenium
-        name: pytest (selenium tests)
-        entry: ./env/Scripts/pytest.exe
-        args: ['tests/', '-k', 'selenium', '--webdriver', 'Firefox']
-        language: system
-        pass_filenames: false
-        
-    -   id: pytest-non-selenium
-        name: pytest (non-selenium tests)
-        entry: ./env/Scripts/pytest.exe
-        args: ['tests/', '-k', 'not selenium']
-        language: system
-        pass_filenames: false
-
     -   id: black
         name: black
         entry: ./env/Scripts/black.exe
         language: system
         types: [python]
 
     -   id: isort
         name: isort
         entry: ./env/Scripts/isort.exe
         language: system
         types: [python]
 
-    - id: ruff
-      name: ruff
-      description: "Run 'ruff' for extremely fast Python linting"
-      entry: ruff check --force-exclude
-      language: python
-      types_or: [python, pyi]
-      args: []
-      require_serial: true
-      additional_dependencies: []
-      minimum_pre_commit_version: "2.9.2"
-
-    - id: ruff-format
-      name: ruff-format
-      description: "Run 'ruff format' for extremely fast Python formatting"
-      entry: ruff format --force-exclude
-      language: python
-      types_or: [python, pyi]
-      args: []
-      require_serial: true
-      additional_dependencies: []
-      minimum_pre_commit_version: "2.9.2"
-
     -   id: mypy
         name: mypy
         entry: ./env/Scripts/mypy.exe
         language: system
         types: [python]
+
+    -   id: pytest-selenium
+        name: pytest (selenium tests)
+        entry: ./env/Scripts/pytest.exe
+        args: ['tests/', '-k', 'selenium', '--webdriver', 'Firefox', '--testmon']
+        language: system
+        pass_filenames: false
+
+    -   id: pytest-non-selenium
+        name: pytest (non-selenium tests)
+        entry: ./env/Scripts/pytest.exe
+        args: ['tests/', '-k', 'not selenium', '--testmon']
+        language: system
+        pass_filenames: false
```

### Comparing `Dash_tooltip-0.3.9/Dash_tooltip.egg-info/SOURCES.txt` & `Dash_tooltip-0.4.0/Dash_tooltip.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -17,17 +17,22 @@
 Dash_tooltip.egg-info/PKG-INFO
 Dash_tooltip.egg-info/SOURCES.txt
 Dash_tooltip.egg-info/dependency_links.txt
 Dash_tooltip.egg-info/requires.txt
 Dash_tooltip.egg-info/top_level.txt
 dash_tooltip/__init__.py
 dash_tooltip/config.py
+dash_tooltip/custom_figure.py
 dash_tooltip/utils.py
 tests/__init__.py
 tests/test_11_direct_figure_in_dcc_graph.py
+tests/test_12_go_scatter.py
+tests/test_13_go_scatter_line.py
+tests/test_14_go_bar_chart.py
+tests/test_16_update_template.py
 tests/test_1_tooltip_function.py
 tests/test_2_tooltip_configuration.py
 tests/test_3_template_formating.py
 tests/test_4a_multiple_graph.py
 tests/test_4b_multiple_graph.py
 tests/test_6_invalid_graph_id.py
 tests/test_7_tooltip_removal.py
```

### Comparing `Dash_tooltip-0.3.9/LICENSE` & `Dash_tooltip-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Dash_tooltip-0.3.9/dash_qt_demo.py` & `Dash_tooltip-0.4.0/dash_qt_demo.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,15 @@
                     "data": [
                         {
                             "x": x,
                             "y": y,
                             "type": "scatter",
                             "mode": "lines",
                             "name": "sin(x)",
+                            "meta": ["some meta info"],
                         },
                         {
                             "x": x,
                             "y": y1,
                             "type": "scatter",
                             "mode": "lines",
                             "name": "cos(x)",
@@ -114,15 +115,15 @@
         ],
         style={
             "width": "95vw",
             "height": "95vh",
             "overflow": "hidden",
         },  # Full viewport width and height
     )
-    template = "%{label},<br>x: %{x:.2f},<br>y: %{y:.3f}"
+    template = "%{name}<br>%{meta[0]}<br>x: %{x:.2f}<br>y: %{y:.3f}"
     tooltip(app, template=template)
     return app
 
 
 def run_dash():
     """
     Run the Dash app server.
```

### Comparing `Dash_tooltip-0.3.9/dash_qt_demo2.py` & `Dash_tooltip-0.4.0/dash_qt_demo2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import http.client
-import threading
 import os
 import sys
+import threading
 import time
 
 import dash
 import numpy as np
+import plotly.graph_objects as go
 from dash import dcc, html
 from PyQt6.QtCore import QUrl
 from PyQt6.QtWebEngineWidgets import QWebEngineView
 from PyQt6.QtWidgets import QApplication, QFileDialog, QMainWindow
-import plotly.graph_objects as go
+
 from dash_tooltip import tooltip
 
 dash_port = 8050
 
 
 class MyApp(QMainWindow):
     """
@@ -85,28 +86,28 @@
         "height": "100%",
         # "border": "2px solid red",
     }
 
     layout_margin = {"l": 25, "r": 25, "t": 25, "b": 25}
 
     # Creating a grid of x and y values
-    x = np.linspace(0, 10, 100)
-    y = np.linspace(0, 10, 100)
+    x = np.linspace(0, 10, 400)
+    y = np.linspace(0, 10, 400)
     X, Y = np.meshgrid(x, y)
 
     # Calculate Z as a function of X and Y
     Z = np.sin(X) * np.cos(Y)
 
     # Create a heatmap
     fig2 = go.Figure(
         data=go.Heatmap(
             z=Z,
             x=x,
             y=y,
-            colorscale="Viridis"
+            colorscale="Viridis",
             # You can change the colorscale as needed
         ),
         layout=go.Layout(margin=layout_margin),
     )
 
     # Define scatter data
     x = np.linspace(0, 10, 100)
@@ -147,15 +148,18 @@
         },  # Full viewport width and height
     )
 
     # Add the tooltip functionality to the app
     template1 = "x: %{x:.2f},<br>y: %{y:.2f}"
     tooltip(app, template=template1, graph_ids=["example-graph1"])
     template2 = "x: %{x:.2f},<br>y: %{y:.2f},<br>z: %{z:.3f}"
-    tooltip(app, template=template2, graph_ids=["example-graph2"])
+    tooltip_style = {
+        "bgcolor": "rgba(255, 255, 255, 0.2)",
+    }
+    tooltip(app, style=tooltip_style, template=template2, graph_ids=["example-graph2"])
     return app
 
 
 def run_dash():
     """
     Run the Dash app server.
     """
```

### Comparing `Dash_tooltip-0.3.9/dash_tooltip/__init__.py` & `Dash_tooltip-0.4.0/dash_tooltip/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import logging
 from string import Template
 from typing import Any, Dict, List, Optional, Union
 
 import plotly.graph_objs as go
 from dash import Input, Output, State, dash
 
-from .config import DEFAULT_ANNOTATION_CONFIG
+from .config import DEFAULT_ANNOTATION_CONFIG, DEFAULT_TEMPLATE
+from .custom_figure import CustomFigure
 from .utils import _display_click_data, _find_all_graph_ids, add_annotation_store
 
 # Logger setup
 logger = logging.getLogger("dash_tooltip")
 logger.setLevel(logging.DEBUG)
 
 # File handler setup
@@ -25,132 +26,178 @@
 
 # Prevent logs from being propagated to the root logger
 logger.propagate = False
 
 # Now, you can log messages
 logger.debug("dash_tooltip log active")
 
-DEFAULT_TEMPLATE = "x: %{x},<br>y: %{y}"
+registered_callbacks = set()
+
+
+class TooltipManager:
+    def __init__(
+        self,
+        app: dash.Dash,
+        style: Dict[Any, Any],
+        template: str,
+        graph_ids: List[str],
+        apply_log_fix: bool,
+        debug: bool,
+    ):
+        self.figures = {graph_id: CustomFigure() for graph_id in graph_ids}
+        self.templates = {graph_id: template for graph_id in graph_ids}
+        self.style = style
+        self.apply_log_fix = apply_log_fix
+        self.debug = debug
+        self.app = app
+        self.graph_ids = graph_ids
+        self.tooltip_active = True  # Default to active
+        self.initialize_callbacks()
+
+    def update_template(self, graph_id: str, template: str):
+        if graph_id in self.figures:
+            self.templates[graph_id] = template
+            self.figures[graph_id].update_template(template)
+
+    def initialize_callbacks(self):
+        for graph_id in self.graph_ids:
+            callback_identifier = (graph_id, "figure")
+            if callback_identifier in registered_callbacks:
+                # Skip reattaching if already registered
+                continue
+            registered_callbacks.add(callback_identifier)
+
+            # Check for valid graph ID and add annotation store
+            if graph_id not in self.app.layout:
+                raise ValueError(f"Invalid graph ID provided: {graph_id}")
+            add_annotation_store(self.app.layout, graph_id)
+
+            @self.app.callback(
+                Output(component_id=graph_id, component_property="figure"),
+                Input(component_id=graph_id, component_property="clickData"),
+                State(component_id=graph_id, component_property="figure"),
+            )
+            def display_click_data(
+                clickData: Dict[str, Any],
+                figure: Union[CustomFigure, Dict[str, Any]],
+            ) -> CustomFigure:
+                """Display data on click event."""
+                if not self.tooltip_active:
+                    raise dash.PreventUpdate
+
+                if figure is None:
+                    figure = CustomFigure()
+
+                template = self.templates[graph_id]
+                if isinstance(figure, CustomFigure):
+                    return _display_click_data(clickData, figure, template, self.style)
+                # Check if figure is a dictionary
+                elif isinstance(figure, dict):
+                    # Extract data and layout from the figure dictionary
+                    raw_data = figure.get("data", [])
+                    layout = figure.get("layout", {})
+
+                    # Convert dictionary representations of traces into actual trace objects
+                    data = []
+                    for trace in raw_data:
+                        trace_type = trace.pop("type")
+                        trace_class = getattr(go, trace_type.capitalize())
+                        data.append(trace_class(**trace))
+
+                    # Construct the CustomFigure(go.Figure) using data and layout
+                    custom_figure = CustomFigure(data=data, layout=layout)
+                    return _display_click_data(
+                        clickData, custom_figure, template, self.style
+                    )
+                else:
+                    custom_figure = CustomFigure(figure)
+                    return _display_click_data(
+                        clickData, custom_figure, template, self.style
+                    )
+
+            @self.app.callback(
+                Output(graph_id, "figure", allow_duplicate=True),
+                Input(f"tooltip-annotations-to-remove-{graph_id}", "data"),
+                State(graph_id, "figure"),
+                prevent_initial_call=True,
+            )
+            def remove_empty_annotations(
+                indices_to_remove: List[int], current_figure: Dict[str, Any]
+            ) -> Union[Dict[str, Any], dash._callback.NoUpdate]:
+                """Remove annotations that have been deleted by the user."""
+                if indices_to_remove:
+                    annotations = current_figure["layout"].get("annotations", [])
+                    logger.debug(f"Original Annotations: {annotations}")
+                    updated_annotations = [
+                        anno
+                        for idx, anno in enumerate(annotations)
+                        if idx not in indices_to_remove
+                    ]
+                    logger.debug(f"Indices to Remove: {indices_to_remove}")
+                    logger.debug(f"Updated Annotations: {updated_annotations}")
+                    current_figure["layout"]["annotations"] = updated_annotations
+                    return current_figure
+                return dash.no_update
+
+            # Client-side callback to identify annotations to remove
+            dbg_str = "console.log(relayoutData);" if self.debug else ""
+            self.app.clientside_callback(
+                Template(
+                    """
+                    function(relayoutData) {
+                        $dbg_str
+                        var annotationPattern = /annotations\\[(\\d+)\\].text/;
+                        var indicesToRemove = [];
+                        for (var key in relayoutData) {
+                            var match = key.match(annotationPattern);
+                            if (match && relayoutData[key] === "") {
+                                indicesToRemove.push(parseInt(match[1]));
+                            }
+                        }
+                        return indicesToRemove;
+                    }
+                    """
+                ).substitute(dbg_str=dbg_str),
+                Output(f"tooltip-annotations-to-remove-{graph_id}", "data"),
+                Input(graph_id, "relayoutData"),
+            )
 
 
 def tooltip(
     app: dash.Dash,
     style: Dict[Any, Any] = DEFAULT_ANNOTATION_CONFIG,
     template: str = DEFAULT_TEMPLATE,
     graph_ids: Optional[List[str]] = None,
     apply_log_fix: bool = True,
     debug: bool = False,
-) -> None:
+) -> TooltipManager:
     """
     Add tooltip functionality to Dash graph components.
 
     Args:
-    - app (dash.Dash): The Dash app instance.
-    - style (dict): Configuration for the tooltip appearance. Users can provide any
-                    valid Plotly annotation style options.
-                    Default values are set in DEFAULT_ANNOTATION_CONFIG.
-    - template (str): A string defining how the tooltip should be displayed using
-                    Plotly's template syntax. Users can modify this template to
-                    customize the tooltip content.
-    - graph_ids (list, optional): List of graph component IDs for the tooltip
-                    functionality. If None, function will try to find graph IDs
-                    automatically.
-    - apply_log_fix (bool): If True, applies a logarithmic transformation fix for
-                    log axes due to a long-standing Plotly bug.
-                    More details can be found at:
-                    https://github.com/plotly/plotly.py/issues/2580
-                    Default is True.
-    - debug (bool): If True, debug information will be written to a log file
-                    (tooltip.log).
-
-    Example:
-    tooltip(app,
-            style={'text_color': 'red'},
-            template="x: %{x},<br>y: %{y}<br>ID: %{pointNumber}",
-            graph_ids=['graph-1'])
+        app (dash.Dash): The Dash app instance.
+        style (dict): Configuration for the tooltip appearance.
+                      Users can provide any valid Plotly annotation style options.
+        template (str): The default annotation template.
+                        Default is a basic string template.
+        graph_ids (list, optional): List of graph IDs to apply tooltips to.
+                                    If not provided, will try to auto-detect from the layout.
+        apply_log_fix (bool): If True, applies a fix for logging issues.
+        debug (bool): If True, enables debugging mode.
+
+    Returns:
+        TooltipManager: An instance of TooltipManager class.
     """
     if graph_ids is None:
         graph_ids = _find_all_graph_ids(app.layout)
         if not graph_ids:
             raise ValueError(
                 "No graphs found in the app layout. Please provide a graph ID."
             )
-
-    for graph_id in graph_ids:
-        if graph_id not in app.layout:
-            raise ValueError(f"Invalid graph ID provided: {graph_id}")
-        add_annotation_store(app.layout, graph_id)
-
-        @app.callback(  # type: ignore
-            Output(component_id=graph_id, component_property="figure"),
-            Input(component_id=graph_id, component_property="clickData"),
-            State(component_id=graph_id, component_property="figure"),
-        )
-        def display_click_data(
-            clickData: Dict[str, Any], figure: go.Figure
-        ) -> go.Figure:
-            return _display_click_data(
-                clickData, figure, app, template, style, apply_log_fix, debug
-            )
-
-        dbg_str = "console.log(relayoutData);"
-
-        app.clientside_callback(
-            Template(
-                r"""
-                function(relayoutData) {
-                    $dbg_str
-                    var annotationPattern = /annotations\[(\d+)\].text/;
-                    var indicesToRemove = [];
-                    for (var key in relayoutData) {
-                        var match = key.match(annotationPattern);
-                        if (match && relayoutData[key] === "") {
-                            indicesToRemove.push(parseInt(match[1]));
-                        }
-                    }
-                    return indicesToRemove;
-                }
-            """
-            ).substitute(dbg_str=dbg_str),
-            Output(f"tooltip-annotations-to-remove-{graph_id}", "data"),
-            Input(graph_id, "relayoutData"),
-        )
-
-        @app.callback(  # type: ignore
-            Output(graph_id, "figure", allow_duplicate=True),
-            Input(f"tooltip-annotations-to-remove-{graph_id}", "data"),
-            State(graph_id, "figure"),
-            prevent_initial_call=True,
-        )
-        def remove_empty_annotations(
-            indices_to_remove: List[int], current_figure: Dict[str, Any]
-        ) -> Union[Dict[str, Any], dash._callback.NoUpdate]:
-            """Remove annotations that have been deleted by the user."""
-            if indices_to_remove:
-                annotations = current_figure["layout"].get("annotations", [])
-
-                # Log the original annotations
-                logger.debug(f"Original Annotations: {annotations}")
-
-                updated_annotations = [
-                    anno
-                    for idx, anno in enumerate(annotations)
-                    if idx not in indices_to_remove
-                ]
-
-                # Log the indices being removed
-                logger.debug(f"Indices to Remove: {indices_to_remove}")
-
-                # Log the updated annotations
-                logger.debug(f"Updated Annotations: {updated_annotations}")
-
-                current_figure["layout"]["annotations"] = updated_annotations
-                return current_figure  # update figure with new annotations list
-            return dash.no_update  # prevent undesired update when no change is done
-            # (also prevents breaking)
+    return TooltipManager(app, style, template, graph_ids, apply_log_fix, debug)
 
 
 __all__ = [
     "tooltip",
     "add_annotation_store",
     "DEFAULT_ANNOTATION_CONFIG",
     "DEFAULT_TEMPLATE",
```

### Comparing `Dash_tooltip-0.3.9/dash_tooltip/config.py` & `Dash_tooltip-0.4.0/dash_tooltip/config.py`

 * *Files identical despite different names*

### Comparing `Dash_tooltip-0.3.9/dash_tooltip/utils.py` & `Dash_tooltip-0.4.0/dash_tooltip/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,40 +5,40 @@
 from typing import Any, Dict, List, Optional, Union
 
 import dash
 import plotly.graph_objs as go
 from dash import dcc
 from dash.html import Div
 
-from dash_tooltip import DEFAULT_ANNOTATION_CONFIG
+from .config import DEFAULT_ANNOTATION_CONFIG
+from .custom_figure import CustomFigure
 
 logger = logging.getLogger("dash_tooltip")
 
 
 def add_annotation_store(layout: Div, graph_id: Optional[str] = None) -> str:
     """
     Adds a dcc.Store component to the layout to store annotations for tooltips.
 
     Args:
-    - layout (dash.html.Div): The Dash app layout.
-    - graph_id (str, optional): The ID of the graph component to which the store is
-    linked.
+        layout (dash.html.Div): The Dash app layout.
+        graph_id (str, optional): The ID of the graph component to which the store is linked.
 
     Returns:
-    - str: The ID of the added dcc.Store component.
+        str: The ID of the added dcc.Store component.
     """
     store_id = "tooltip-annotations-to-remove"
     if graph_id:
         store_id += f"-{graph_id}"
 
     if not any(
         isinstance(child, dcc.Store) and child.id == store_id
         for child in layout.children
     ):
-        if isinstance(layout.children, List):
+        if isinstance(layout.children, list):
             layout.children.append(dcc.Store(id=store_id))
 
     return store_id
 
 
 def _find_all_graph_ids(layout: Div) -> List[str]:
     """Recursively search for all graph component IDs in the app layout."""
@@ -57,15 +57,15 @@
     return graph_ids
 
 
 def extract_value_from_point(point: Dict[str, Any], key: str) -> Any:
     """Extracts the value from the point dictionary using a dot notation key."""
     try:
         parts = key.split(".")
-        temp: Any = point  # fix type hint issue
+        temp: Any = point
         for part in parts:
             match = re.match(r"(\w+)\[(\d+)\]", part)
             if match:
                 name, index = match.groups()
                 index = int(index)
                 if temp and isinstance(temp, dict) and name in temp:
                     temp = temp.get(name, [])[index]
@@ -74,29 +74,28 @@
             else:
                 if temp and isinstance(temp, dict):
                     temp = temp.get(part)
                 else:
                     return None
         return temp
     except Exception as e:
-        print(f"Error extracting value with key {key}. Error: {e}")
+        logger.error(f"Error extracting value with key {key}. Error: {e}")
         return None
 
 
 def truncate_json_arrays(json_str: str, limit: int) -> str:
     """
-    Truncate arrays in a JSON string representation to a specified limit, both at top
-    level and nested.
+    Truncate arrays in a JSON string representation to a specified limit, both at top level and nested.
 
     Parameters:
-    - json_str (str): The JSON string representation to be processed.
-    - limit (int): The maximum number of elements to keep in any array.
+        json_str (str): The JSON string representation to be processed.
+        limit (int): The maximum number of elements to keep in any array.
 
     Returns:
-    - str: The processed JSON string with arrays truncated.
+        str: The processed JSON string with arrays truncated.
     """
 
     def truncate_arrays(data: Any) -> Any:
         """
         Recursively truncate arrays in a data structure (dicts or lists).
         """
         if isinstance(data, list):
@@ -129,150 +128,173 @@
 
 
 def get_axis_type(fig: go.Figure, axis: str) -> str:
     """
     Determines the type of the specified axis in a Plotly figure.
 
     Parameters:
-    fig (Union[Figure, dict]): The Plotly figure object or dictionary.
-    axis (str): The axis identifier, e.g., 'x', 'y', 'x2', 'y2', etc.
+        fig (go.Figure): The Plotly figure object.
+        axis (str): The axis identifier, e.g., 'x', 'y', 'x2', 'y2', etc.
 
     Returns:
-    str: The type of the specified axis, e.g., 'linear' or 'log'.
+        str: The type of the specified axis, e.g., 'linear' or 'log'.
     """
     # Check if the axis identifier has a number at the end
     axis_number = axis[-1]
     if axis_number.isnumeric():
         axis_key = axis[:-1] + "axis" + axis_number
     else:
         axis_key = axis + "axis"
 
-    axis_type = fig.layout[axis_key].type
-    return axis_type
+    return fig.layout[axis_key].type
 
 
 def _display_click_data(
     clickData: Dict[str, Any],
-    figure: Union[go.Figure, Dict[str, Any]],  # Allow both go.Figure and dictionary
-    app: dash.Dash,
+    figure: Union[CustomFigure, Dict[str, Any]],  # Allow both go.Figure and dictionary
     template: str,
     config: Dict[Any, Any],
     apply_log_fix: bool = True,
     debug: bool = False,
-) -> go.Figure:
-    """Displays the tooltip on the graph when a data point is clicked."""
+) -> CustomFigure:
+    """
+    Displays the tooltip on the graph when a data point is clicked.
+
+    Args:
+        clickData (Dict[str, Any]): The data from the click event.
+        figure (Union[CustomFigure, Dict[str, Any]]): The figure to update.
+        template (str): The template for the tooltip.
+        config (Dict[Any, Any]): The configuration for the tooltip.
+        apply_log_fix (bool, optional): Whether to apply the log axis fix. Defaults to True.
+        debug (bool, optional): Whether to enable debugging. Defaults to False.
 
+    Returns:
+        CustomFigure: The updated figure.
+    """
     xaxis, yaxis = "x", "y"  # Default values
 
+    if figure is None:
+        raise ValueError("The figure provided is None.")
+
     # Check if figure is a dictionary
     if isinstance(figure, dict):
         # Extract data and layout from the figure dictionary
         raw_data = figure.get("data", [])
         layout = figure.get("layout", {})
 
         # Convert dictionary representations of traces into actual trace objects
         data = []
         for trace in raw_data:
             trace_type = trace.pop("type")
             trace_class = getattr(go, trace_type.capitalize())
             data.append(trace_class(**trace))
 
         # Construct the go.Figure using data and layout
-        fig = go.Figure(data=data, layout=layout)
-    else:
+        fig = CustomFigure(data=data, layout=layout)
+    elif isinstance(figure, CustomFigure):
         fig = figure
+    else:
+        raise TypeError(
+            "The figure provided must be of type 'CustomFigure' or a dictionary."
+        )
+
+    fig.update_template(template)
 
     merged_config = deep_merge_dicts(DEFAULT_ANNOTATION_CONFIG.copy(), config)
 
-    if not getattr(app, "tooltip_active", True):
+    if not dash.callback_context:
         raise dash.exceptions.PreventUpdate
 
     if clickData:
         point = clickData["points"][0]
         x_val = point["x"]
         y_val = point["y"]
 
         try:
             # Extract the clicked axis information from the curve data
-            if "xaxis" in figure["data"][point["curveNumber"]]:
-                xaxis = figure["data"][point["curveNumber"]]["xaxis"]
+            if "xaxis" in fig["data"][point["curveNumber"]]:
+                xaxis = fig["data"][point["curveNumber"]]["xaxis"]
             else:
                 xaxis = "x"
 
-            if "yaxis" in figure["data"][point["curveNumber"]]:
-                yaxis = figure["data"][point["curveNumber"]]["yaxis"]
+            if "yaxis" in fig["data"][point["curveNumber"]]:
+                yaxis = fig["data"][point["curveNumber"]]["yaxis"]
             else:
                 yaxis = "y"
 
-            # Extract label from the curve data
-            point["label"] = figure["data"][point["curveNumber"]]["name"]
+            if "meta" in fig["data"][point["curveNumber"]]:
+                point["meta"] = fig["data"][point["curveNumber"]]["meta"]
+
+            if "name" in fig["data"][point["curveNumber"]]:
+                point["name"] = fig["data"][point["curveNumber"]]["name"]
 
             # If the x-axis is logarithmic, adjust `x_val`
-            # This is a fix for longstanding Plotly bug
-            # https://github.com/plotly/plotly.py/issues/2580
             if apply_log_fix and get_axis_type(fig, xaxis) == "log":
                 x_val = math.log10(x_val)
 
             # If the y-axis is logarithmic, adjust `y_val`
             if apply_log_fix and get_axis_type(fig, yaxis) == "log":
                 y_val = math.log10(y_val)
 
         except KeyError as e:
             logger.error(f"Error: {e}, key not found")
         except Exception as e:
             logger.error(f"An unexpected error occurred: {e}")
 
         if debug:
             logger.debug(
-                f"clickData: {truncate_json_arrays(json.dumps(clickData, indent=4),2)}"
+                f"clickData: {truncate_json_arrays(json.dumps(clickData, indent=4), 2)}"
             )
             logger.debug(
-                f"figure: {truncate_json_arrays(json.dumps(figure, indent=4),2)}"
+                f"figure: {truncate_json_arrays(json.dumps(fig, indent=4), 2)}"
             )
             logger.debug(
                 "Point data:\n%s", truncate_json_arrays(json.dumps(point, indent=4), 2)
             )
             logger.debug(
                 "Trace data:\n%s",
                 truncate_json_arrays(
-                    json.dumps(figure["data"][point["curveNumber"]], indent=4), 2
+                    json.dumps(fig["data"][point["curveNumber"]], indent=4), 2
                 ),
             )
 
-        placeholders = re.findall(r"%{(.*?)}", template)
+        placeholders = re.findall(r"%{(.*?)}", fig.layout._tooltip_template)
 
         template_data = {}
         for placeholder in placeholders:
             parts = placeholder.split(":")
             var_name = parts[0]
             format_spec = parts[1] if len(parts) > 1 else None
 
             value = extract_value_from_point(point, var_name)
             if value is not None:
                 if format_spec:
                     try:
                         # Applying the format specifier directly
                         template_data[placeholder] = f"{value:{format_spec}}"
                     except ValueError as e:
-                        # Fallback to string representation if formatting fails
                         logger.error(
-                            f"Error formatting value {value}, with format {format_spec}"
-                            f" properties in {merged_config}. Error: {e}"
+                            f"Error formatting value {value}, with format {format_spec}. Error: {e}"
                         )
                         template_data[placeholder] = str(value)
                 else:
                     template_data[placeholder] = str(value)
 
+        tooltip_template = fig.layout._tooltip_template
         for placeholder, value in template_data.items():
-            template = template.replace(f"%{{{placeholder}}}", value)
+            tooltip_template = tooltip_template.replace(f"%{{{placeholder}}}", value)
 
         try:
             fig.add_annotation(
-                x=x_val, y=y_val, xref=xaxis, yref=yaxis, text=template, **merged_config
+                x=x_val,
+                y=y_val,
+                xref=xaxis,
+                yref=yaxis,
+                text=tooltip_template,
+                **merged_config,
             )
         except ValueError as e:
             logger.error(
-                f"Failed to add annotation due to invalid"
-                f" properties in {merged_config}. Error: {e}"
+                f"Failed to add annotation due to invalid properties in {merged_config}. Error: {e}"
             )
             raise e
     return fig
```

### Comparing `Dash_tooltip-0.3.9/dash_tooltip_demo.py` & `Dash_tooltip-0.4.0/dash_tooltip_demo.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,22 +23,21 @@
 # %% jupyter={"source_hidden": true}
 import warnings
 
 import dash
 import dash_bootstrap_components as dbc
 
 # ---- Imports ----
-import ipywidgets as widgets
 import numpy as np
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objects as go
 import plotly.io as pio
-from dash import Dash, dcc, html
-from IPython.display import display
+from dash import Dash, Input, Output, dcc, html
+from dash.exceptions import PreventUpdate
 from plotly.subplots import make_subplots
 from plotly_resampler import FigureResampler
 from trace_updater import TraceUpdater  # Assuming you've imported this module
 
 from dash_tooltip import add_annotation_store, tooltip
 
 pio.templates.default = "none"
@@ -232,15 +231,15 @@
 
 # Add the tooltip functionality to the app3
 tooltip(app3)
 
 if __name__ == "__main__":
     app3.run(debug=True, port=8083)
 
-# %%
+# %% jupyter={"source_hidden": true}
 # ---- Test 4: Multiple Traces with Tooltips ----
 app4 = Dash(__name__)
 
 # Random data for three traces
 np.random.seed(0)
 y1 = np.random.normal(0, 10, 50)
 custom_labels4_1 = [f"A {i}" for i in range(50)]
@@ -314,14 +313,15 @@
 tooltip(app4, style=custom_style, template=template)
 
 if __name__ == "__main__":
     app4.run(debug=True, port=8084)
 
 # %% jupyter={"source_hidden": true}
 # ---- Test 5: Multiple Traces with Toggable Tooltip function ----
+# ---- Test 5: Multiple Traces with Toggable Tooltip function ----
 app5 = Dash(__name__)
 
 # Random data for three traces
 np.random.seed(0)
 y1 = np.random.normal(0, 10, 50)
 custom_labels1 = [f"A {i}" for i in range(50)]
 y2 = np.random.normal(5, 5, 50)
@@ -361,71 +361,73 @@
             ]
         ),
         dbc.Row(
             [
                 dbc.Col(
                     [
                         dcc.Graph(
-                            id="multi-trace-graph",
+                            id="multi-trace-graph5",
                             figure=fig5,
                             config={
                                 "editable": True,
                                 "edits": {
                                     "shapePosition": True,
                                     "annotationPosition": True,
                                 },
                             },
                         )
                     ]
                 )
             ]
         ),
+        dbc.Row(
+            [
+                dbc.Col(
+                    dbc.Switch(
+                        id="tooltip-switch",
+                        label="Enable Tooltip",
+                        value=False,
+                        className="mt-3",
+                    ),
+                )
+            ]
+        ),
+        html.Div(id="dummy-output-for-callback", style={"display": "none"}),
     ]
 )
 
 # Add the tooltip functionality to the app
 custom_style = {
     "font": {"size": 10},
     "arrowcolor": "blue",
     "arrowsize": 2.5,
     # ... any other customization
 }
 template = "x: %{x},<br>y: %{y},<br>%{customdata[0]}"
-tooltip(app5, style=custom_style, template=template)
-
-app5.tooltip_active = False
-
-if __name__ == "__main__":
-    app5.run(debug=True, port=8085)
+tooltip_instance5 = tooltip(app5, style=custom_style, template=template)
 
+tooltip_instance5.tooltip_active = False
 
-# %% jupyter={"source_hidden": true}
-# ---- Test 6: Two Traces with Multiple Custom Data ----
-def toggle_tooltip(change):
-    app5.tooltip_active = change["new"]
 
-
-# Create a toggle button
-toggle = widgets.ToggleButton(
-    value=app5.tooltip_active,
-    description="Toggle Tooltip",
-    disabled=False,
-    button_style="",  # 'success', 'info', 'warning', 'danger' or ''
-    tooltip="Toggle Tooltip Active Status",
-    icon="check",  # (FontAwesome names without the `fa-` prefix)
+# Create a callback to toggle the tooltip
+@app5.callback(
+    Output("dummy-output-for-callback", "children"),  # We don't need a real output
+    Input("tooltip-switch", "value"),
 )
+def toggle_tooltip(value: bool):
+    tooltip_instance5.tooltip_active = value
+    return ""
 
-# Display the button
-display(toggle)
 
-# Link the button action to the function
-toggle.observe(toggle_tooltip, "value")
+if __name__ == "__main__":
+    app5.run(debug=False, port=8085)
+
 
 # %% jupyter={"source_hidden": true}
-# Two Traces with Multiple Custom Data
+# ---- Test 6: Two Traces with Multiple Custom Data ----
 
 app6 = Dash(__name__)
 
 # Random data for two traces
 np.random.seed(0)
 y1 = np.random.normal(0, 10, 50)
 custom_labels6_1 = [[f"A {i}", f"X {i * 2}"] for i in range(50)]
@@ -457,15 +459,15 @@
             ]
         ),
         dbc.Row(
             [
                 dbc.Col(
                     [
                         dcc.Graph(
-                            id="double-customdata-graph",
+                            id="double-customdata-graph6",
                             figure=fig6,
                             config={
                                 "editable": True,
                                 "edits": {
                                     "shapePosition": True,
                                     "annotationPosition": True,
                                 },
@@ -754,15 +756,15 @@
 template10 = template
 tooltip(app10, graph_ids=["graph-id"], template=template10, debug=True)
 
 # Register the callback with FigureResampler
 fig10.register_update_graph_callback(app10, "graph-id", "trace-updater")
 
 # Show the Dash app
-app10.run(debug=True, port=8090, jupyter_height=500)
+app10.run(debug=False, port=8090, jupyter_height=500)
 
 
 # %% jupyter={"source_hidden": true}
 # wrapper function
 def interactive_plot(fig, graphid, template):
     """
     Creates a Dash app with an interactive plot.
@@ -831,15 +833,15 @@
     trace.customdata = np.column_stack(
         (np.repeat(df.columns[i], len(df)), np.repeat("#{}".format(i + 1), len(df)))
     )
     trace.hovertemplate = template
 
 app11, fig11 = interactive_plot(fig11, graphid_11, template)
 if __name__ == "__main__":
-    app11.run(debug=True, port=8091)
+    app11.run(debug=False, port=8091)
 
 # %% jupyter={"source_hidden": true}
 # ---- Test 12: 2x2 Subplot with 2 traces on each subplot (Organized like Test 10) ----
 
 # Generate random time series data
 date_rng = pd.date_range(start="2020-01-01", end="2020-12-31", freq="m")
 
@@ -926,15 +928,15 @@
 fig12.update_layout(title_text="2x2 Subplots with 2 Traces Each")
 
 # Register the callback with FigureResampler
 fig12.register_update_graph_callback(app12, "graph-id12", "trace-updater12")
 
 # Code to run the Dash app
 # (commented out for now, but can be used in a local environment)
-app12.run(debug=True, port=8092)
+app12.run(debug=False, port=8092)
 
 # %% jupyter={"source_hidden": true}
 # ---- Test 13: Direct Data Injection into dcc.Graph with Draggable Annotations ----
 graphid_1 = "graph1"
 
 np.random.seed(20)
 y1 = np.random.normal(0, 10, 50)
@@ -948,21 +950,21 @@
 app13.layout = dbc.Container(
     [
         dbc.Row(
             [
                 dbc.Col(
                     [
                         dcc.Graph(
-                            id="example-graph",
+                            id="example-graph13",
                             figure={
                                 "data": [
                                     {
                                         "x": x1,
                                         "y": y1,
-                                        "type": "line",
+                                        "type": "scatter",
                                         "mode": "lines",
                                         "name": "sin(x)",
                                     }
                                 ],
                                 "layout": {
                                     "title": "Direct Data Injection into "
                                     "dcc.Graph with Draggable Annotations"
@@ -983,15 +985,15 @@
     ]
 )
 
 # Add the tooltip functionality to the app
 tooltip(app13, debug=True)
 
 if __name__ == "__main__":
-    app13.run(debug=True, port=8093)
+    app13.run(debug=False, port=8093)
 
 # %% jupyter={"source_hidden": true}
 # ---- Test 14: log axis ----
 
 # Generate exponential data
 x_data = np.linspace(1, 100, 100)  # Generating 100 points from 1 to 100
 
@@ -1095,15 +1097,15 @@
 fig14.update_layout(title_text="2x2 Subplots with 2 Traces Each", height=800)
 
 # Register the callback with FigureResampler
 fig14.register_update_graph_callback(app14, "graph-id14", "trace-updater14")
 
 # Code to run the Dash app
 # (commented out for now, but can be used in a local environment)
-app14.run(debug=True, port=8094, jupyter_height=800)
+app14.run(debug=False, port=8094, jupyter_height=800)
 
 
 # %% jupyter={"source_hidden": true}
 # ---- Test 15: log axis (placement should fail if Plotly bug still present)----
 
 # Plotly bug https://github.com/plotly/plotly.py/issues/2580
 
@@ -1214,11 +1216,117 @@
 )
 
 # Register the callback with FigureResampler
 fig15.register_update_graph_callback(app15, "graph-id15", "trace-updater15")
 
 # Code to run the Dash app
 # (commented out for now, but can be used in a local environment)
-app15.run(debug=True, port=8095, jupyter_height=800)
+app15.run(debug=False, port=8095, jupyter_height=800)
+
 
+# %%
+# ---- Test 16: update tooltip template----
+GRAPH_ID = "scatter-plot16a"
+
+# Sample DataFrame with DatetimeIndex
+date_range = pd.date_range(start="2025-01-01", periods=5)
+df = pd.DataFrame(
+    {
+        "x": [1, 2, 3, 4, 5],
+        "y": [2, 4, 6, 8, 10],
+        "z": [3, 6, 9, 12, 15],
+        "a": [4, 8, 12, 16, 20],
+        "b": [5, 10, 15, 20, 25],
+    },
+    index=date_range,
+)
+
+# Initialize the Dash app
+app16 = dash.Dash(__name__)
+
+# Define the layout
+app16.layout = html.Div(
+    [
+        html.Label("Select X and Y columns:"),
+        dcc.Dropdown(
+            id="x-column",
+            options=[{"label": col, "value": col} for col in df.columns],
+            placeholder="Select X axis data",
+        ),
+        dcc.Dropdown(
+            id="y-column",
+            options=[{"label": col, "value": col} for col in df.columns],
+            placeholder="Select Y axis data",
+        ),
+        dcc.Graph(
+            id=GRAPH_ID,
+            style={"width": "600px", "height": "600px"},
+            config={
+                "editable": True,
+                "edits": {"shapePosition": True, "annotationPosition": True},
+            },
+        ),
+    ]
+)
+
+tooltip_instance16 = tooltip(app16, debug=True, graph_ids=[GRAPH_ID])
+
+
+# Define callback to update the scatter plot
+@app16.callback(
+    Output(GRAPH_ID, "figure", allow_duplicate=True),
+    [Input("x-column", "value"), Input("y-column", "value")],
+    prevent_initial_call=True,
+)
+def update_scatter_plot(x_column, y_column):
+    if not x_column or not y_column:
+        raise PreventUpdate  # Prevent update if either dropdown is not selected
+
+    non_selected_columns = [
+        col for col in df.columns if col not in [x_column, y_column]
+    ]
+    customdata = df[non_selected_columns].apply(
+        lambda row: "<br>".join(
+            f"{col}: {val}" for col, val in zip(non_selected_columns, row)
+        ),
+        axis=1,
+    )
+    # gives (depending on selected entries):
+    # 2022-01-01     x: 1<br>z: 3<br>b: 5
+    # 2022-01-02     x: 2<br>z: 6<br>b: 10
+    # ...
+
+    template = (
+        "<b>Date</b>: %{customdata}<br>"
+        + f"<b>{x_column}: %{{x}}<br>"
+        + f"{y_column}: %{{y}}</b><br>"
+    )
+    # gives (depending on selected entries):
+    # <b>Date</b>: %{customdata}<br><b>x: %{x}<br><b>a</b>: %{y}<br>
+
+    tooltip_instance16.update_template(graph_id=GRAPH_ID, template=template)
+
+    trace = go.Scatter(
+        x=df[x_column],
+        y=df[y_column],
+        mode="markers",
+        marker=dict(color="blue"),
+        customdata=df.index.strftime("%Y-%m-%d %H:%M:%S") + "<br>" + customdata,
+        # Include date and time with other data
+        hovertemplate=template,
+    )
+    layout = go.Layout(
+        title="Scatter Plot",
+        xaxis=dict(title=x_column),
+        yaxis=dict(title=y_column),
+        hovermode="closest",
+        height=800,
+        width=800,
+    )
+    return {"data": [trace], "layout": layout}
+
+
+# Run the app
+if __name__ == "__main__":
+    app16.run_server(debug=False, port=8196)
 
 # %% jupyter={"source_hidden": true}
```

### Comparing `Dash_tooltip-0.3.9/noxfile.py` & `Dash_tooltip-0.4.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `Dash_tooltip-0.3.9/setup.py` & `Dash_tooltip-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `Dash_tooltip-0.3.9/tests/test_11_direct_figure_in_dcc_graph.py` & `Dash_tooltip-0.4.0/tests/test_11_direct_figure_in_dcc_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from dash_tooltip import tooltip
 
 app13 = Dash(__name__)
 
 np.random.seed(20)
 y1 = np.random.normal(0, 10, 50)
-x1 = np.arange(0, 30)
+x1 = np.arange(0, 15)
 
 app13.layout = dbc.Container(
     [
         dbc.Row(
             [
                 dbc.Col(
                     [
```

### Comparing `Dash_tooltip-0.3.9/tests/test_1_tooltip_function.py` & `Dash_tooltip-0.4.0/tests/test_1_tooltip_function.py`

 * *Files identical despite different names*

### Comparing `Dash_tooltip-0.3.9/tests/test_2_tooltip_configuration.py` & `Dash_tooltip-0.4.0/tests/test_2_tooltip_configuration.py`

 * *Files identical despite different names*

### Comparing `Dash_tooltip-0.3.9/tests/test_3_template_formating.py` & `Dash_tooltip-0.4.0/tests/test_3_template_formating.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,32 +20,32 @@
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.ui import WebDriverWait
 
 from dash_tooltip import tooltip
 
 app = dash.Dash(__name__)
-graphid_2 = "graph2"
+graphid_3 = "graph3"
 
 
 @app.callback(Output("output-div", "children"), Input("graph-input", "clickData"))
 def display_click_data(clickData: Dict[str, Any]) -> str:
     if clickData:
         point = clickData["points"][0]
         return f'You clicked on point {point["x"]}, {point["y"]}'
     return "Click on a point to see its data."
 
 
 np.random.seed(42)
-y2 = np.random.normal(0, 10, 50)
-x2 = np.arange(0, 50)
-custom_labels = [f"Label {i}" for i in range(50)]
-fig2 = px.scatter(x=x2, y=y2, custom_data=[custom_labels, y2 * 2])
-fig2.update_traces(name="LABEL")
-fig2.update_layout(title_text="Editable Title", title_x=0.5)
+y2 = np.random.normal(0, 10, 25)
+x2 = np.arange(0, 25)
+custom_labels = [f"Label {i}" for i in range(25)]
+fig3 = px.scatter(x=x2, y=y2, custom_data=[custom_labels, y2 * 2])
+fig3.update_traces(name="LABEL", meta=["META0", "META1"])
+fig3.update_layout(title_text="Editable Title", title_x=0.5)
 
 app.layout = dbc.Container(
     [
         dbc.Row(
             [
                 dbc.Col(
                     [
@@ -58,16 +58,16 @@
             ]
         ),
         dbc.Row(
             [
                 dbc.Col(
                     [
                         dcc.Graph(
-                            id=graphid_2,
-                            figure=fig2,
+                            id=graphid_3,
+                            figure=fig3,
                             config={
                                 "editable": True,
                                 "edits": {
                                     "shapePosition": True,
                                     "annotationPosition": True,
                                 },
                             },
@@ -76,15 +76,18 @@
                 )
             ]
         ),
     ]
 )
 
 # Tooltip template from dash_tooltip_demo.py
-tooltip_template = "%{label},<br>x: %{x},<br>y: %{y:.2f},<br>%{customdata[0]},<br>2y=%{customdata[1]:.3f}"
+tooltip_template = (
+    "%{name},<br>%{meta[1]},<br>x: %{x},<br>y: %{y:.2f},<br>%{"
+    "customdata[0]},<br>2y=%{customdata[1]:.3f}"
+)
 tooltip(app, template=tooltip_template, debug=True)
 
 
 @pytest.mark.selenium
 def test_customdata_tooltip(dash_duo: Any) -> None:
     driver = dash_duo.driver
     wait = WebDriverWait(driver, 30)
@@ -94,18 +97,20 @@
     expected_custom_label = custom_labels[idx]
 
     # Extract x and y values directly from the data
     x_value = x2[idx]
     y_value = y2[idx]
     expected_custom_label2 = y_value * 2
     expected_label = "LABEL"
+    expected_meta = "META1"
 
     expected_annotation_text = (
         tooltip_template.replace("<br>", "")
-        .replace("%{label}", expected_label)
+        .replace("%{name}", expected_label)
+        .replace("%{meta[1]}", expected_meta)
         .replace("%{x}", str(x_value))
         .replace("%{y:.2f}", f"{y_value:.2f}")
         .replace("%{customdata[0]}", expected_custom_label)
         .replace("%{customdata[1]:.3f}", f"{expected_custom_label2:.3f}")
     )
 
     # Start the Dash app
```

### Comparing `Dash_tooltip-0.3.9/tests/test_4a_multiple_graph.py` & `Dash_tooltip-0.4.0/tests/test_4a_multiple_graph.py`

 * *Files identical despite different names*

### Comparing `Dash_tooltip-0.3.9/tests/test_4b_multiple_graph.py` & `Dash_tooltip-0.4.0/tests/test_4b_multiple_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,16 +76,16 @@
         "annotationTail": True,
         "annotationText": True,
     },
 }
 
 app.layout = html.Div(
     [
-        dcc.Graph(id="graph-1", figure=fig1, config=editable_config),
-        dcc.Graph(id="graph-2", figure=fig2, config=editable_config),
+        dcc.Graph(id="graph-1b", figure=fig1, config=editable_config),
+        dcc.Graph(id="graph-2b", figure=fig2, config=editable_config),
         dcc.Graph(id="subplot-graph", figure=fig, config=editable_config),
     ]
 )
 
 # Apply tooltips to both graphs
 tooltip(app, debug=True)
 
@@ -111,15 +111,15 @@
             if element.is_displayed():
                 success = True
                 break
 
         return success
 
     # For each graph, interact with a data point to trigger the tooltip
-    for graph_id in ["graph-1", "graph-2", "subplot-graph"]:
+    for graph_id in ["graph-1b", "graph-2b", "subplot-graph"]:
         if graph_id == "subplot-graph":
             # Handle subplots differently. Interact with each subplot.
             subplots = ["xy", "x2y2", "x3y3", "x4y4"]
 
             for subplot in subplots:
                 # Interact with a data point in the current subplot
                 element = WebDriverWait(driver, 1).until(
```

### Comparing `Dash_tooltip-0.3.9/tests/test_7_tooltip_removal.py` & `Dash_tooltip-0.4.0/tests/test_7_tooltip_removal.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.expected_conditions import staleness_of
 from selenium.webdriver.support.ui import WebDriverWait
 
 from dash_tooltip import tooltip
 
 app = Dash(__name__)
-graph_id = "graph-input"
+graph_id = "graph-input7"
 
 
 @app.callback(Output("output-div", "children"), Input(graph_id, "clickData"))
 def display_click_data(clickData: Dict[str, Any]) -> str:
     if clickData:
         point = clickData["points"][0]
         return f'You clicked on point ({point["x"]}, {point["y"]})'
```

### Comparing `Dash_tooltip-0.3.9/tests/test_8__display_click_data.py` & `Dash_tooltip-0.4.0/tests/test_8__display_click_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 from typing import Dict, List, Union
 
 import dash
 import plotly.graph_objs as go
 
 from dash_tooltip import (  # Adjust the import based on where the function is defined.
+    CustomFigure,
     _display_click_data,
 )
 
 # Assuming these constants are defined elsewhere in your code or test environment.
 SAMPLE_APP = dash.Dash(__name__)
 DEFAULT_TEMPLATE = "x: %{x},<br>y: %{y}"
 DEFAULT_ANNOTATION_CONFIG = {
@@ -50,48 +51,46 @@
     "font": {"color": "black", "family": "Arial", "size": 12},
     "showarrow": True,
     "xanchor": "left",
 }
 
 
 def test_display_click_data_no_click() -> None:
-    fig_before = go.Figure(data=[go.Scatter(x=[1, 2, 3], y=[1, 3, 2])])
+    fig_before = CustomFigure(data=[go.Scatter(x=[1, 2, 3], y=[1, 3, 2])])
 
     # Use an empty dictionary as the dummy clickData
     dummy_click_data: Dict[str, List[Dict[str, Union[int, float]]]] = {}
 
     fig_after = _display_click_data(
         dummy_click_data,
         fig_before,
-        SAMPLE_APP,
         DEFAULT_TEMPLATE,
         DEFAULT_ANNOTATION_CONFIG,
         True,
         False,
     )
 
     assert fig_before == fig_after, "Figures should be identical with no click data."
 
 
 def test_display_click_data_with_click() -> None:
-    fig_before = go.Figure(data=[go.Scatter(x=[1, 2, 3], y=[1, 3, 2])])
+    fig_before = CustomFigure(data=[go.Scatter(x=[1, 2, 3], y=[1, 3, 2])])
     click_data = {
         "points": [
             {
                 "x": 2,
                 "y": 3,
                 "curveNumber": 0,
                 # ... other potential attributes
             }
         ]
     }
     fig_after = _display_click_data(
         click_data,
         fig_before,
-        SAMPLE_APP,
         DEFAULT_TEMPLATE,
         DEFAULT_ANNOTATION_CONFIG,
         True,
         False,
     )
     assert len(fig_after.layout.annotations) == 1, "One annotation should be added."
     assert fig_after.layout.annotations[0].text == "x: 2,<br>y: 3"
@@ -100,24 +99,24 @@
 def test_display_click_data_custom_style() -> None:
     custom_style = {
         "arrowcolor": "red",
         "font": {"color": "green", "size": 15, "family": "Verdana"},
         "arrowhead": 4,
         "bordercolor": "blue",
     }
-    fig_before = go.Figure(data=[go.Scatter(x=[1, 2, 3], y=[1, 3, 2])])
+    fig_before = CustomFigure(data=[go.Scatter(x=[1, 2, 3], y=[1, 3, 2])])
     click_data = {
         "points": [
             {
                 "x": 2,
                 "y": 3,
                 "curveNumber": 0,
                 # ... other potential attributes
             }
         ]
     }
     fig_after = _display_click_data(
-        click_data, fig_before, SAMPLE_APP, DEFAULT_TEMPLATE, custom_style, True, False
+        click_data, fig_before, DEFAULT_TEMPLATE, custom_style, True, False
     )
     annotation = fig_after.layout.annotations[0]
     assert annotation.arrowcolor == "red", "Arrow color mismatch."
     # Add additional assertions for other styles.
```

