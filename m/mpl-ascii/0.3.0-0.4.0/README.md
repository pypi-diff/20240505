# Comparing `tmp/mpl_ascii-0.3.0.tar.gz` & `tmp/mpl_ascii-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpl_ascii-0.3.0.tar", last modified: Tue Apr 30 17:43:44 2024, max compression
+gzip compressed data, was "mpl_ascii-0.4.0.tar", last modified: Sun May  5 16:04:28 2024, max compression
```

## Comparing `mpl_ascii-0.3.0.tar` & `mpl_ascii-0.4.0.tar`

### file list

```diff
@@ -1,49 +1,21 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-30 17:43:44.744003 mpl_ascii-0.3.0/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-30 17:43:44.736003 mpl_ascii-0.3.0/.github/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-30 17:43:44.736003 mpl_ascii-0.3.0/.github/workflows/
--rw-rw-r--   0 chris     (1000) chris     (1000)      992 2024-04-25 17:23:19.000000 mpl_ascii-0.3.0/.github/workflows/python-package.yml
--rw-rw-r--   0 chris     (1000) chris     (1000)     3107 2024-04-25 16:48:20.000000 mpl_ascii-0.3.0/.gitignore
--rw-rw-r--   0 chris     (1000) chris     (1000)     1066 2024-04-25 16:42:37.000000 mpl_ascii-0.3.0/LICENSE
--rw-rw-r--   0 chris     (1000) chris     (1000)     1472 2024-04-27 12:42:39.000000 mpl_ascii-0.3.0/Makefile
--rw-r--r--   0 chris     (1000) chris     (1000)     5590 2024-04-30 17:43:44.744003 mpl_ascii-0.3.0/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)     5253 2024-04-30 17:38:47.000000 mpl_ascii-0.3.0/README.md
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-30 17:43:44.744003 mpl_ascii-0.3.0/examples/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1306 2024-04-25 16:44:32.000000 mpl_ascii-0.3.0/examples/bar_chart.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      827 2024-04-28 08:03:54.000000 mpl_ascii-0.3.0/examples/bar_color.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      903 2024-04-25 16:44:32.000000 mpl_ascii-0.3.0/examples/bar_label_1.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1011 2024-04-25 16:44:32.000000 mpl_ascii-0.3.0/examples/bar_label_2.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1084 2024-04-25 16:44:32.000000 mpl_ascii-0.3.0/examples/bar_label_3.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      675 2024-04-25 16:44:32.000000 mpl_ascii-0.3.0/examples/bar_label_4.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      669 2024-04-25 16:44:32.000000 mpl_ascii-0.3.0/examples/bar_label_5.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1012 2024-04-25 16:44:32.000000 mpl_ascii-0.3.0/examples/bar_stacked.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1036 2024-04-25 16:44:32.000000 mpl_ascii-0.3.0/examples/barh.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      736 2024-04-25 16:44:32.000000 mpl_ascii-0.3.0/examples/categorical_variables.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1069 2024-04-25 16:44:32.000000 mpl_ascii-0.3.0/examples/cohere.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      998 2024-04-25 16:44:32.000000 mpl_ascii-0.3.0/examples/cohere_single_plot.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1286 2024-04-25 16:44:32.000000 mpl_ascii-0.3.0/examples/csd_demo.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      747 2024-04-28 08:04:51.000000 mpl_ascii-0.3.0/examples/double_plot.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1124 2024-04-25 16:44:32.000000 mpl_ascii-0.3.0/examples/hist_best_fit_line.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1019 2024-04-25 16:44:32.000000 mpl_ascii-0.3.0/examples/hist_simple.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1665 2024-04-25 16:44:32.000000 mpl_ascii-0.3.0/examples/hist_simple_colors.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1188 2024-04-25 16:44:32.000000 mpl_ascii-0.3.0/examples/lines_multi_color.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1218 2024-04-28 08:05:08.000000 mpl_ascii-0.3.0/examples/scatter_multi_color.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      627 2024-04-25 16:44:32.000000 mpl_ascii-0.3.0/examples/simple_plot.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-30 17:43:44.744003 mpl_ascii-0.3.0/mpl_ascii/
--rw-rw-r--   0 chris     (1000) chris     (1000)     3413 2024-04-30 16:42:51.000000 mpl_ascii-0.3.0/mpl_ascii/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1239 2024-04-30 16:43:02.000000 mpl_ascii-0.3.0/mpl_ascii/ascii_canvas.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2055 2024-04-30 16:45:38.000000 mpl_ascii-0.3.0/mpl_ascii/color_map.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     9879 2024-04-30 16:42:27.000000 mpl_ascii-0.3.0/mpl_ascii/draw.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1342 2024-04-30 16:37:32.000000 mpl_ascii-0.3.0/mpl_ascii/overlay.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      274 2024-04-25 16:43:43.000000 mpl_ascii-0.3.0/mpl_ascii/tools.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-30 17:43:44.744003 mpl_ascii-0.3.0/mpl_ascii.egg-info/
--rw-r--r--   0 chris     (1000) chris     (1000)     5590 2024-04-30 17:43:44.000000 mpl_ascii-0.3.0/mpl_ascii.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      945 2024-04-30 17:43:44.000000 mpl_ascii-0.3.0/mpl_ascii.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2024-04-30 17:43:44.000000 mpl_ascii-0.3.0/mpl_ascii.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       31 2024-04-30 17:43:44.000000 mpl_ascii-0.3.0/mpl_ascii.egg-info/requires.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       10 2024-04-30 17:43:44.000000 mpl_ascii-0.3.0/mpl_ascii.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      445 2024-04-30 17:39:29.000000 mpl_ascii-0.3.0/pyproject.toml
--rw-rw-r--   0 chris     (1000) chris     (1000)      144 2024-04-25 18:43:05.000000 mpl_ascii-0.3.0/requirements.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2024-04-30 17:43:44.744003 mpl_ascii-0.3.0/setup.cfg
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-30 17:43:44.744003 mpl_ascii-0.3.0/tests/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2024-04-25 16:45:15.000000 mpl_ascii-0.3.0/tests/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4510 2024-04-30 16:36:55.000000 mpl_ascii-0.3.0/tests/test_overlay.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-05 16:04:28.904389 mpl_ascii-0.4.0/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1066 2024-04-25 16:42:37.000000 mpl_ascii-0.4.0/LICENSE
+-rw-r--r--   0 chris     (1000) chris     (1000)     5652 2024-05-05 16:04:28.904389 mpl_ascii-0.4.0/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5253 2024-04-30 17:38:47.000000 mpl_ascii-0.4.0/README.md
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-05 16:04:28.904389 mpl_ascii-0.4.0/mpl_ascii/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3413 2024-05-04 12:09:44.000000 mpl_ascii-0.4.0/mpl_ascii/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1239 2024-04-30 16:43:02.000000 mpl_ascii-0.4.0/mpl_ascii/ascii_canvas.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2055 2024-04-30 16:45:38.000000 mpl_ascii-0.4.0/mpl_ascii/color_map.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    12382 2024-05-05 15:53:15.000000 mpl_ascii-0.4.0/mpl_ascii/draw.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1342 2024-04-30 16:37:32.000000 mpl_ascii-0.4.0/mpl_ascii/overlay.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      274 2024-04-25 16:43:43.000000 mpl_ascii-0.4.0/mpl_ascii/tools.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-05 16:04:28.904389 mpl_ascii-0.4.0/mpl_ascii.egg-info/
+-rw-r--r--   0 chris     (1000) chris     (1000)     5652 2024-05-05 16:04:28.000000 mpl_ascii-0.4.0/mpl_ascii.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      347 2024-05-05 16:04:28.000000 mpl_ascii-0.4.0/mpl_ascii.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2024-05-05 16:04:28.000000 mpl_ascii-0.4.0/mpl_ascii.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       31 2024-05-05 16:04:28.000000 mpl_ascii-0.4.0/mpl_ascii.egg-info/requires.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       10 2024-05-05 16:04:28.000000 mpl_ascii-0.4.0/mpl_ascii.egg-info/top_level.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)      513 2024-05-05 16:01:04.000000 mpl_ascii-0.4.0/pyproject.toml
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2024-05-05 16:04:28.904389 mpl_ascii-0.4.0/setup.cfg
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-05 16:04:28.904389 mpl_ascii-0.4.0/tests/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4510 2024-04-30 16:36:55.000000 mpl_ascii-0.4.0/tests/test_overlay.py
```

### Comparing `mpl_ascii-0.3.0/LICENSE` & `mpl_ascii-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.3.0/PKG-INFO` & `mpl_ascii-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: mpl_ascii
-Version: 0.3.0
+Version: 0.4.0
 Summary: A matplotlib backend that produces plots using only ASCII characters
 License: MIT License
+Project-URL: Homepage, https://github.com/chriscave/mpl_ascii
 Keywords: matplotlib,plotting,ASCII
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3.8.3
 Requires-Dist: rich>=13.7.1
```

### Comparing `mpl_ascii-0.3.0/README.md` & `mpl_ascii-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.3.0/mpl_ascii/__init__.py` & `mpl_ascii-0.4.0/mpl_ascii/__init__.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.3.0/mpl_ascii/ascii_canvas.py` & `mpl_ascii-0.4.0/mpl_ascii/ascii_canvas.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.3.0/mpl_ascii/color_map.py` & `mpl_ascii-0.4.0/mpl_ascii/color_map.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.3.0/mpl_ascii/draw.py` & `mpl_ascii-0.4.0/mpl_ascii/draw.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import math
 from matplotlib.collections import PathCollection
-from matplotlib.container import BarContainer
+from matplotlib.container import BarContainer, ErrorbarContainer
 from matplotlib.lines import Line2D
 from matplotlib.patches import Rectangle
 import numpy as np
 
 from mpl_ascii.ascii_canvas import AsciiCanvas
-from mpl_ascii.color_map import ax_color_map, std_color
+from mpl_ascii.color_map import Char, ax_color_map, std_color
 from mpl_ascii.tools import linear_transform, scale_factor
 
 def draw_ax(ax, axes_height, axes_width):
     frame_buffer_left = 1
     frame_buffer_right = 1
     frame_buffer_top = 1
     frame_buffer_bottom = 1
@@ -59,34 +59,93 @@
             )
         )
         ascii_x_bar = round(linear_transform(bar.xy[0], x_min, x_max, 0, axes_width-1))
         ascii_y_bar = round(linear_transform(bar.xy[1], y_min, y_max, 1, axes_height))
 
         canvas = canvas.update(canvas_bar, (axes_height - ascii_y_bar - canvas_bar.shape[0]+1, ascii_x_bar))
 
+    errorbar_caplines = []
+    for container in ax.containers:
+        if not isinstance(container, ErrorbarContainer):
+            continue
+        _, caplines, _ = tuple(container)
+        errorbar_caplines += [*caplines]
+
 
+    lines_with_markers = []
     for line in ax.get_lines():
+        if line in errorbar_caplines:
+            continue
+        if line.get_marker() != "None":
+            lines_with_markers.append(line)
+
         char = color_to_ascii[std_color(line.get_color())]
         xy_data = line.get_xydata()
         x_data, y_data = [dat[0] for dat in xy_data], [dat[1] for dat in xy_data]
-
         line = AsciiCanvas(
                 draw_line(
                 width=axes_width,
                 height=axes_height,
                 x_data=x_data,
                 y_data=y_data,
                 x_range=x_range,
                 y_range=y_range,
-                char = char
+                char = char,
+                linestyle=line.get_linestyle()
             )
         )
 
         canvas = canvas.update(line, (0,0))
 
+    for container in ax.containers:
+        if not isinstance(container, ErrorbarContainer):
+            continue
+        _, _, barlinescols = tuple(container)
+
+        for collection in barlinescols:
+            for xy in collection.get_segments():
+                x_data = [p[0] for p in xy]
+                y_data = [p[1] for p in xy]
+                char = Char("-", "white")
+
+                if len(set(x_data)) == 1:
+                    char = Char("|", "white")
+
+                errorbar = AsciiCanvas(draw_line(
+                    width=axes_width,
+                    height=axes_height,
+                    x_data=x_data,
+                    y_data=y_data,
+                    x_range=x_range,
+                    y_range=y_range,
+                    char = char
+                ))
+                canvas = canvas.update(errorbar, (0,0))
+
+    for line in lines_with_markers:
+        marker = get_ascii_marker(line.get_marker())
+
+        color = color_to_ascii[std_color(line.get_color())].color
+        char = Char(marker.upper(), color)
+        xy_data = line.get_xydata()
+        x_data, y_data = [dat[0] for dat in xy_data], [dat[1] for dat in xy_data]
+        line = AsciiCanvas(
+                draw_line(
+                width=axes_width,
+                height=axes_height,
+                x_data=x_data,
+                y_data=y_data,
+                x_range=x_range,
+                y_range=y_range,
+                char = char,
+                linestyle="None"
+            )
+        )
+        canvas = canvas.update(line, (0,0))
+
     for collection in ax.collections:
         if not isinstance(collection, PathCollection):
             continue
         offsets = collection.get_offsets()
 
         color = collection.get_facecolors()[0]
         for point in offsets:
@@ -170,15 +229,15 @@
     frame[0,-1] = "+"
     frame[-1,0] = "+"
     frame[-1,-1] = "+"
 
     return frame
 
 
-def draw_line(height, width, x_data, y_data, x_range, y_range, char):
+def draw_line(height, width, x_data, y_data, x_range, y_range, char, linestyle="-"):
 
     x_min, x_max = x_range[0], x_range[1]
     y_min, y_max = y_range[0], y_range[1]
 
     plot_x = []
     plot_y = []
     for x,y in zip(x_data, y_data):
@@ -195,26 +254,30 @@
     ]
     ascii_y_data = [
         round(linear_transform(y, y_min, y_max, 1, height)) for y in plot_y if (y <= y_max and y >= y_min)
     ]
 
     line_canvas_arr = np.full((height, width), fill_value=" ", dtype="object")
 
+    for x, y in zip(ascii_x_data, ascii_y_data):
+        row = height - y
+        col = x
+        line_canvas_arr[row, col] = char
+
+    if linestyle == "None":
+        return line_canvas_arr
+
     start_points = zip(ascii_x_data[:-1], ascii_y_data[:-1])
     end_points = zip(ascii_x_data[1:], ascii_y_data[1:])
     join_line_points = []
     for start, end in zip(start_points, end_points):
         line_points = bresenham_line(start[0], start[1], end[0], end[1])
         if len(line_points) > 2:
             join_line_points += line_points[1:-1]
 
-    for x, y in zip(ascii_x_data, ascii_y_data):
-        row = height - y
-        col = x
-        line_canvas_arr[row, col] = char
 
     for x,y in join_line_points:
         row = height - y
         col = x
         line_canvas_arr[row, col] = char
 
     return line_canvas_arr
@@ -294,8 +357,25 @@
         error -= abs(dy)
         if error < 0:
             y += ystep
             error += dx
 
     return points
 
+def get_ascii_marker(marker):
+    if marker == "s":
+        marker = chr(9632)
+    if marker == "o":
+        marker = "O"
+    if marker == "v" or marker == "1":
+        marker = chr(9660)
+    if marker == "^" or marker == "2":
+        marker = chr(9650)
+    if marker == "<" or marker == "3":
+        marker = chr(9664)
+    if marker == ">" or marker == "4":
+        marker = chr(9654)
+
+    return marker
+
+
```

### Comparing `mpl_ascii-0.3.0/mpl_ascii/overlay.py` & `mpl_ascii-0.4.0/mpl_ascii/overlay.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.3.0/mpl_ascii.egg-info/PKG-INFO` & `mpl_ascii-0.4.0/mpl_ascii.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: mpl_ascii
-Version: 0.3.0
+Version: 0.4.0
 Summary: A matplotlib backend that produces plots using only ASCII characters
 License: MIT License
+Project-URL: Homepage, https://github.com/chriscave/mpl_ascii
 Keywords: matplotlib,plotting,ASCII
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3.8.3
 Requires-Dist: rich>=13.7.1
```

### Comparing `mpl_ascii-0.3.0/tests/test_overlay.py` & `mpl_ascii-0.4.0/tests/test_overlay.py`

 * *Files identical despite different names*

