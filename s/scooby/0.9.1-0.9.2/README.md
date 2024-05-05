# Comparing `tmp/scooby-0.9.1.tar.gz` & `tmp/scooby-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scooby-0.9.1.tar", last modified: Sat Oct 21 00:18:38 2023, max compression
+gzip compressed data, was "scooby-0.9.2.tar", last modified: Sat Oct 21 00:34:36 2023, max compression
```

## Comparing `scooby-0.9.1.tar` & `scooby-0.9.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 00:18:38.518021 scooby-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2023-10-21 00:18:04.000000 scooby-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15327 2023-10-21 00:18:38.518021 scooby-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14687 2023-10-21 00:18:04.000000 scooby-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 00:18:38.518021 scooby-0.9.1/scooby/
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2023-10-21 00:18:04.000000 scooby-0.9.1/scooby/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2023-10-21 00:18:04.000000 scooby-0.9.1/scooby/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2023-10-21 00:18:04.000000 scooby-0.9.1/scooby/knowledge.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 00:18:04.000000 scooby-0.9.1/scooby/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    18016 2023-10-21 00:18:04.000000 scooby-0.9.1/scooby/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2023-10-21 00:18:04.000000 scooby-0.9.1/scooby/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-21 00:18:38.000000 scooby-0.9.1/scooby/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 00:18:38.518021 scooby-0.9.1/scooby.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15327 2023-10-21 00:18:38.000000 scooby-0.9.1/scooby.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      335 2023-10-21 00:18:38.000000 scooby-0.9.1/scooby.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-21 00:18:38.000000 scooby-0.9.1/scooby.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-10-21 00:18:38.000000 scooby-0.9.1/scooby.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-10-21 00:18:38.000000 scooby-0.9.1/scooby.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-10-21 00:18:38.000000 scooby-0.9.1/scooby.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-21 00:18:38.518021 scooby-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2023-10-21 00:18:04.000000 scooby-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 00:34:36.066035 scooby-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2023-10-21 00:34:19.000000 scooby-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15327 2023-10-21 00:34:36.066035 scooby-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14687 2023-10-21 00:34:19.000000 scooby-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 00:34:36.062035 scooby-0.9.2/scooby/
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2023-10-21 00:34:19.000000 scooby-0.9.2/scooby/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2023-10-21 00:34:19.000000 scooby-0.9.2/scooby/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2023-10-21 00:34:19.000000 scooby-0.9.2/scooby/knowledge.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 00:34:19.000000 scooby-0.9.2/scooby/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    17568 2023-10-21 00:34:19.000000 scooby-0.9.2/scooby/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2023-10-21 00:34:19.000000 scooby-0.9.2/scooby/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-21 00:34:35.000000 scooby-0.9.2/scooby/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 00:34:36.066035 scooby-0.9.2/scooby.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15327 2023-10-21 00:34:35.000000 scooby-0.9.2/scooby.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2023-10-21 00:34:36.000000 scooby-0.9.2/scooby.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-21 00:34:35.000000 scooby-0.9.2/scooby.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2023-10-21 00:34:35.000000 scooby-0.9.2/scooby.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2023-10-21 00:34:35.000000 scooby-0.9.2/scooby.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-10-21 00:34:35.000000 scooby-0.9.2/scooby.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-21 00:34:36.066035 scooby-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2023-10-21 00:34:19.000000 scooby-0.9.2/setup.py
```

### Comparing `scooby-0.9.1/LICENSE` & `scooby-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scooby-0.9.1/PKG-INFO` & `scooby-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scooby
-Version: 0.9.1
+Version: 0.9.2
 Summary: A Great Dane turned Python environment detective
 Home-page: https://github.com/banesullivan/scooby
 Author: Dieter Werthmüller, Bane Sullivan, Alex Kaszynski, and contributors
 Author-email: info@pyvista.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `scooby-0.9.1/README.md` & `scooby-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `scooby-0.9.1/scooby/__init__.py` & `scooby-0.9.2/scooby/__init__.py`

 * *Files identical despite different names*

### Comparing `scooby-0.9.1/scooby/__main__.py` & `scooby-0.9.2/scooby/__main__.py`

 * *Files identical despite different names*

### Comparing `scooby-0.9.1/scooby/knowledge.py` & `scooby-0.9.2/scooby/knowledge.py`

 * *Files identical despite different names*

### Comparing `scooby-0.9.1/scooby/report.py` & `scooby-0.9.2/scooby/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -433,44 +433,36 @@
 
         return out
 
 
 class AutoReport(Report):
     """Auto-generate a scooby.Report for a package.
 
-    This will check if the specified package has a ``Report`` class and use that or
-    fallback to generating a report based on the distribution requirements of the package.
+    This will generate a report based on the distribution requirements of the package.
     """
 
     def __init__(self, module, additional=None, ncol=3, text_width=80, sort=False):
         """Initialize."""
         if not isinstance(module, (str, ModuleType)):
             raise TypeError("Cannot generate report for type " "({})".format(type(module)))
 
         if isinstance(module, ModuleType):
             module = module.__name__
 
-        try:
-            package = importlib.import_module(module)
-            if issubclass(package.Report, Report):
-                package.Report.__init__(
-                    self, additional=additional, ncol=ncol, text_width=text_width, sort=sort
-                )
-        except (AttributeError, ImportError):
-            # Autogenerate from distribution requirements
-            core = [module, *get_distribution_dependencies(module)]
-            Report.__init__(
-                self,
-                additional=additional,
-                core=core,
-                optional=[],
-                ncol=ncol,
-                text_width=text_width,
-                sort=sort,
-            )
+        # Autogenerate from distribution requirements
+        core = [module, *get_distribution_dependencies(module)]
+        Report.__init__(
+            self,
+            additional=additional,
+            core=core,
+            optional=[],
+            ncol=ncol,
+            text_width=text_width,
+            sort=sort,
+        )
 
 
 # This functionaliy might also be of interest on its own.
 def get_version(module: Union[str, ModuleType]) -> Tuple[str, Optional[str]]:
     """Get the version of ``module`` by passing the package or it's name.
 
     Parameters
```

### Comparing `scooby-0.9.1/scooby/tracker.py` & `scooby-0.9.2/scooby/tracker.py`

 * *Files identical despite different names*

### Comparing `scooby-0.9.1/scooby.egg-info/PKG-INFO` & `scooby-0.9.2/scooby.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scooby
-Version: 0.9.1
+Version: 0.9.2
 Summary: A Great Dane turned Python environment detective
 Home-page: https://github.com/banesullivan/scooby
 Author: Dieter Werthmüller, Bane Sullivan, Alex Kaszynski, and contributors
 Author-email: info@pyvista.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `scooby-0.9.1/setup.py` & `scooby-0.9.2/setup.py`

 * *Files identical despite different names*

