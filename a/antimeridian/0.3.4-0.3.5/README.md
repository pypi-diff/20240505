# Comparing `tmp/antimeridian-0.3.4.tar.gz` & `tmp/antimeridian-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antimeridian-0.3.4.tar", last modified: Fri Mar 29 13:06:05 2024, max compression
+gzip compressed data, was "antimeridian-0.3.5.tar", last modified: Sun May  5 13:13:46 2024, max compression
```

## Comparing `antimeridian-0.3.4.tar` & `antimeridian-0.3.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:06:05.808485 antimeridian-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)     9723 2024-03-29 13:06:02.000000 antimeridian-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-03-29 13:06:05.808485 antimeridian-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-03-29 13:06:02.000000 antimeridian-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-03-29 13:06:02.000000 antimeridian-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 13:06:05.808485 antimeridian-0.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:06:05.800485 antimeridian-0.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:06:05.804485 antimeridian-0.3.4/src/antimeridian/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-03-29 13:06:02.000000 antimeridian-0.3.4/src/antimeridian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-03-29 13:06:02.000000 antimeridian-0.3.4/src/antimeridian/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    24303 2024-03-29 13:06:02.000000 antimeridian-0.3.4/src/antimeridian/_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 13:06:02.000000 antimeridian-0.3.4/src/antimeridian/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:06:05.804485 antimeridian-0.3.4/src/antimeridian.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-03-29 13:06:05.000000 antimeridian-0.3.4/src/antimeridian.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-29 13:06:05.000000 antimeridian-0.3.4/src/antimeridian.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 13:06:05.000000 antimeridian-0.3.4/src/antimeridian.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-29 13:06:05.000000 antimeridian-0.3.4/src/antimeridian.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-29 13:06:05.000000 antimeridian-0.3.4/src/antimeridian.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-29 13:06:05.000000 antimeridian-0.3.4/src/antimeridian.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:06:05.804485 antimeridian-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-29 13:06:02.000000 antimeridian-0.3.4/tests/test_bbox.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-29 13:06:02.000000 antimeridian-0.3.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-03-29 13:06:02.000000 antimeridian-0.3.4/tests/test_geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-29 13:06:02.000000 antimeridian-0.3.4/tests/test_line_string.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-03-29 13:06:02.000000 antimeridian-0.3.4/tests/test_multi_polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-03-29 13:06:02.000000 antimeridian-0.3.4/tests/test_polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-29 13:06:02.000000 antimeridian-0.3.4/tests/test_segment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:13:46.101095 antimeridian-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     9723 2024-05-05 13:13:42.000000 antimeridian-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-05-05 13:13:46.101095 antimeridian-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-05 13:13:42.000000 antimeridian-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-05 13:13:42.000000 antimeridian-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 13:13:46.101095 antimeridian-0.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:13:46.093095 antimeridian-0.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:13:46.097095 antimeridian-0.3.5/src/antimeridian/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-05 13:13:42.000000 antimeridian-0.3.5/src/antimeridian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-05 13:13:42.000000 antimeridian-0.3.5/src/antimeridian/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25165 2024-05-05 13:13:42.000000 antimeridian-0.3.5/src/antimeridian/_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 13:13:42.000000 antimeridian-0.3.5/src/antimeridian/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:13:46.097095 antimeridian-0.3.5/src/antimeridian.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-05-05 13:13:46.000000 antimeridian-0.3.5/src/antimeridian.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-05 13:13:46.000000 antimeridian-0.3.5/src/antimeridian.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 13:13:46.000000 antimeridian-0.3.5/src/antimeridian.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-05 13:13:46.000000 antimeridian-0.3.5/src/antimeridian.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-05 13:13:46.000000 antimeridian-0.3.5/src/antimeridian.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-05 13:13:46.000000 antimeridian-0.3.5/src/antimeridian.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:13:46.097095 antimeridian-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-05 13:13:42.000000 antimeridian-0.3.5/tests/test_bbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-05 13:13:42.000000 antimeridian-0.3.5/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-05 13:13:42.000000 antimeridian-0.3.5/tests/test_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-05 13:13:42.000000 antimeridian-0.3.5/tests/test_line_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-05 13:13:42.000000 antimeridian-0.3.5/tests/test_multi_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-05 13:13:42.000000 antimeridian-0.3.5/tests/test_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-05 13:13:42.000000 antimeridian-0.3.5/tests/test_segment.py
```

### Comparing `antimeridian-0.3.4/LICENSE` & `antimeridian-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `antimeridian-0.3.4/PKG-INFO` & `antimeridian-0.3.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antimeridian
-Version: 0.3.4
+Version: 0.3.5
 Summary: Fix GeoJSON geometries that cross the antimeridian
 Author-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: Documentation, https://antimeridian.readthedocs.io
 Project-URL: Github, https://github.com/gadomski/antimeridian
 Project-URL: Changelog, https://github.com/gadomski/antimeridian/blob/main/CHANGELOG.md
 Keywords: geojson,antimeridian,shapely
@@ -14,22 +14,20 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.17.4
 Requires-Dist: shapely>=2.0
 Provides-Extra: cli
 Requires-Dist: click~=8.1.6; extra == "cli"
 Provides-Extra: dev
-Requires-Dist: black~=24.0; extra == "dev"
-Requires-Dist: blacken-docs~=1.13; extra == "dev"
 Requires-Dist: mypy~=1.2; extra == "dev"
 Requires-Dist: packaging~=24.0; extra == "dev"
 Requires-Dist: pre-commit~=3.2; extra == "dev"
 Requires-Dist: pytest~=8.0; extra == "dev"
 Requires-Dist: pytest-console-scripts~=1.3; extra == "dev"
-Requires-Dist: ruff==0.3.4; extra == "dev"
+Requires-Dist: ruff~=0.4.2; extra == "dev"
 Requires-Dist: tomli~=2.0; python_version < "3.11" and extra == "dev"
 Requires-Dist: typing_extensions; python_version < "3.10" and extra == "dev"
 Provides-Extra: docs
 Requires-Dist: cartopy~=0.21; extra == "docs"
 Requires-Dist: ipykernel~=6.22; extra == "docs"
 Requires-Dist: jupytext~=1.14; extra == "docs"
 Requires-Dist: nbsphinx~=0.9; extra == "docs"
```

### Comparing `antimeridian-0.3.4/README.md` & `antimeridian-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `antimeridian-0.3.4/pyproject.toml` & `antimeridian-0.3.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "antimeridian"
-version = "0.3.4"
+version = "0.3.5"
 authors = [{ name = "Pete Gadomski", email = "pete.gadomski@gmail.com" }]
 description = "Fix GeoJSON geometries that cross the antimeridian"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["geojson", "antimeridian", "shapely"]
 license = { text = "Apache-2.0" }
 classifiers = [
@@ -17,22 +17,20 @@
 Documentation = "https://antimeridian.readthedocs.io"
 Github = "https://github.com/gadomski/antimeridian"
 Changelog = "https://github.com/gadomski/antimeridian/blob/main/CHANGELOG.md"
 
 [project.optional-dependencies]
 cli = ["click~=8.1.6"]
 dev = [
-    "black~=24.0",
-    "blacken-docs~=1.13",
     "mypy~=1.2",
     "packaging~=24.0",
     "pre-commit~=3.2",
     "pytest~=8.0",
     "pytest-console-scripts~=1.3",
-    "ruff==0.3.4",
+    "ruff~=0.4.2",
     "tomli~=2.0; python_version<'3.11'",
     "typing_extensions; python_version<'3.10'",
 ]
 docs = [
     "cartopy~=0.21",
     "ipykernel~=6.22",
     "jupytext~=1.14",
@@ -58,11 +56,11 @@
 ]
 ignore_missing_imports = true
 
 [tool.pytest.ini_options]
 filterwarnings = ["error"]
 
 [tool.ruff]
-select = ["F", "E", "W", "I", "ERA", "RUF"]
+lint.select = ["F", "E", "W", "I", "ERA", "RUF"]
 
 [build-system]
 requires = ["setuptools >= 64"]
```

### Comparing `antimeridian-0.3.4/src/antimeridian/__init__.py` & `antimeridian-0.3.5/src/antimeridian/__init__.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.3.4/src/antimeridian/_cli.py` & `antimeridian-0.3.5/src/antimeridian/_cli.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.3.4/src/antimeridian/_implementation.py` & `antimeridian-0.3.5/src/antimeridian/_implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -377,16 +377,18 @@
 def fix_polygon_to_list(
     polygon: Polygon,
     *,
     force_north_pole: bool,
     force_south_pole: bool,
     fix_winding: bool,
 ) -> List[Polygon]:
-    segments = segment(list(polygon.exterior.coords))
+    exterior = normalize(list(polygon.exterior.coords))
+    segments = segment(exterior)
     if not segments:
+        polygon = Polygon(shell=exterior, holes=polygon.interiors)
         if fix_winding and (
             not shapely.is_ccw(polygon.exterior)
             or any(shapely.is_ccw(interior) for interior in polygon.interiors)
         ):
             FixWindingWarning.warn()
             return [shapely.geometry.polygon.orient(polygon)]
         else:
@@ -421,26 +423,48 @@
                 polygon_interiors = list(polygon.interiors)
                 polygon_interiors.append(interior)
                 polygons[i] = Polygon(polygon.exterior, polygon_interiors)
     assert not interiors
     return polygons
 
 
-def segment(coords: List[XY]) -> List[List[XY]]:
-    segment = []
-    segments = []
+def normalize(coords: List[XY]) -> List[XY]:
+    original = list(coords)
+    all_are_on_antimeridian = True
     for i, point in enumerate(coords):
         # Ensure all longitudes are between -180 and 180, and that tiny floating
         # point differences are ignored.
         if numpy.isclose(point[0], 180):
-            coords[i] = (180, point[1])
+            # https://github.com/gadomski/antimeridian/issues/81
+            if abs(coords[i][1]) != 90 and numpy.isclose(
+                coords[(i - 1) % len(coords)][0], -180
+            ):
+                coords[i] = (-180, point[1])
+            else:
+                coords[i] = (180, point[1])
         elif numpy.isclose(point[0], -180):
-            coords[i] = (-180, point[1])
+            # https://github.com/gadomski/antimeridian/issues/81
+            if abs(coords[i][1]) != 90 and numpy.isclose(
+                coords[(i - 1) % len(coords)][0], 180
+            ):
+                coords[i] = (180, point[1])
+            else:
+                coords[i] = (-180, point[1])
         else:
             coords[i] = (((point[0] + 180) % 360) - 180, point[1])
+            all_are_on_antimeridian = False
+    if all_are_on_antimeridian:
+        return original
+    else:
+        return coords
+
+
+def segment(coords: List[XY]) -> List[List[XY]]:
+    segment = []
+    segments = []
     for start, end in zip(coords, coords[1:]):
         segment.append(start)
         if (end[0] - start[0] > 180) and (end[0] - start[0] != 360):  # left
             latitude = crossing_latitude(start, end)
             segment.append((-180, latitude))
             segments.append(segment)
             segment = [(180, latitude)]
```

### Comparing `antimeridian-0.3.4/src/antimeridian.egg-info/PKG-INFO` & `antimeridian-0.3.5/src/antimeridian.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antimeridian
-Version: 0.3.4
+Version: 0.3.5
 Summary: Fix GeoJSON geometries that cross the antimeridian
 Author-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: Documentation, https://antimeridian.readthedocs.io
 Project-URL: Github, https://github.com/gadomski/antimeridian
 Project-URL: Changelog, https://github.com/gadomski/antimeridian/blob/main/CHANGELOG.md
 Keywords: geojson,antimeridian,shapely
@@ -14,22 +14,20 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.17.4
 Requires-Dist: shapely>=2.0
 Provides-Extra: cli
 Requires-Dist: click~=8.1.6; extra == "cli"
 Provides-Extra: dev
-Requires-Dist: black~=24.0; extra == "dev"
-Requires-Dist: blacken-docs~=1.13; extra == "dev"
 Requires-Dist: mypy~=1.2; extra == "dev"
 Requires-Dist: packaging~=24.0; extra == "dev"
 Requires-Dist: pre-commit~=3.2; extra == "dev"
 Requires-Dist: pytest~=8.0; extra == "dev"
 Requires-Dist: pytest-console-scripts~=1.3; extra == "dev"
-Requires-Dist: ruff==0.3.4; extra == "dev"
+Requires-Dist: ruff~=0.4.2; extra == "dev"
 Requires-Dist: tomli~=2.0; python_version < "3.11" and extra == "dev"
 Requires-Dist: typing_extensions; python_version < "3.10" and extra == "dev"
 Provides-Extra: docs
 Requires-Dist: cartopy~=0.21; extra == "docs"
 Requires-Dist: ipykernel~=6.22; extra == "docs"
 Requires-Dist: jupytext~=1.14; extra == "docs"
 Requires-Dist: nbsphinx~=0.9; extra == "docs"
```

### Comparing `antimeridian-0.3.4/src/antimeridian.egg-info/SOURCES.txt` & `antimeridian-0.3.5/src/antimeridian.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antimeridian-0.3.4/tests/test_cli.py` & `antimeridian-0.3.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.3.4/tests/test_geojson.py` & `antimeridian-0.3.5/tests/test_geojson.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.3.4/tests/test_line_string.py` & `antimeridian-0.3.5/tests/test_line_string.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.3.4/tests/test_multi_polygon.py` & `antimeridian-0.3.5/tests/test_multi_polygon.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.3.4/tests/test_polygon.py` & `antimeridian-0.3.5/tests/test_polygon.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 @pytest.mark.parametrize(
     ("name"),
     [
         "almost-180",
         "complex-split",
         "crossing-latitude",
         "extra-crossing",
+        "issues-81",
         "latitude-band",
         "north-pole",
         "one-hole",
         "over-180",
         "overlap",
         "point-on-antimeridian",
         "simple",
```

