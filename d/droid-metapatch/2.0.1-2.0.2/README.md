# Comparing `tmp/droid_metapatch-2.0.1.tar.gz` & `tmp/droid_metapatch-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "droid_metapatch-2.0.1.tar", max compression
+gzip compressed data, was "droid_metapatch-2.0.2.tar", max compression
```

## Comparing `droid_metapatch-2.0.1.tar` & `droid_metapatch-2.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    35149 2024-04-29 12:55:58.994326 droid_metapatch-2.0.1/LICENSE
--rw-r--r--   0        0        0    22794 2024-04-29 12:55:58.994326 droid_metapatch-2.0.1/README.md
--rw-r--r--   0        0        0      366 2024-04-29 12:55:58.994326 droid_metapatch-2.0.1/metapatch/__init__.py
--rw-r--r--   0        0        0     2533 2024-04-29 12:55:58.994326 droid_metapatch-2.0.1/metapatch/base.py
--rw-r--r--   0        0        0     2029 2024-04-29 12:55:58.994326 droid_metapatch-2.0.1/metapatch/circuits/README.md
--rw-r--r--   0        0        0     2547 2024-04-29 12:55:58.994326 droid_metapatch-2.0.1/metapatch/circuits/__init__.py
--rw-r--r--   0        0        0     6255 2024-04-29 12:55:58.994326 droid_metapatch-2.0.1/metapatch/circuits/base.py
--rw-r--r--   0        0        0    15356 2024-04-29 12:55:58.994326 droid_metapatch-2.0.1/metapatch/circuits/clock.py
--rw-r--r--   0        0        0    53179 2024-04-29 12:55:58.994326 droid_metapatch-2.0.1/metapatch/circuits/cv.py
--rw-r--r--   0        0        0     9625 2024-04-29 12:55:58.994326 droid_metapatch-2.0.1/metapatch/circuits/deprecated.py
--rw-r--r--   0        0        0    23303 2024-04-29 12:55:58.994326 droid_metapatch-2.0.1/metapatch/circuits/logic.py
--rw-r--r--   0        0        0   178579 2024-04-29 12:55:58.998326 droid_metapatch-2.0.1/metapatch/circuits/midi.py
--rw-r--r--   0        0        0    22942 2024-04-29 12:55:58.998326 droid_metapatch-2.0.1/metapatch/circuits/modulation.py
--rw-r--r--   0        0        0    19455 2024-04-29 12:55:58.998326 droid_metapatch-2.0.1/metapatch/circuits/other.py
--rw-r--r--   0        0        0    37744 2024-04-29 12:55:58.998326 droid_metapatch-2.0.1/metapatch/circuits/pitch.py
--rw-r--r--   0        0        0   149008 2024-04-29 12:55:58.998326 droid_metapatch-2.0.1/metapatch/circuits/sequencing.py
--rw-r--r--   0        0        0   145502 2024-04-29 12:55:58.998326 droid_metapatch-2.0.1/metapatch/circuits/ui.py
--rwxr-xr-x   0        0        0     3473 2024-04-29 12:55:58.998326 droid_metapatch-2.0.1/metapatch/cli_util.py
--rw-r--r--   0        0        0      149 2024-04-29 12:55:58.998326 droid_metapatch-2.0.1/metapatch/factory/__init__.py
--rw-r--r--   0        0        0     6591 2024-04-29 12:55:58.998326 droid_metapatch-2.0.1/metapatch/factory/boilerplate.py
--rw-r--r--   0        0        0     3380 2024-04-29 12:55:58.998326 droid_metapatch-2.0.1/metapatch/factory/context.py
--rw-r--r--   0        0        0     4281 2024-04-29 12:55:58.998326 droid_metapatch-2.0.1/metapatch/factory/formatting.py
--rw-r--r--   0        0        0     7437 2024-04-29 12:55:58.998326 droid_metapatch-2.0.1/metapatch/factory/patch_factory.py
--rw-r--r--   0        0        0     4565 2024-04-29 12:55:58.998326 droid_metapatch-2.0.1/metapatch/factory/patch_parser.py
--rw-r--r--   0        0        0    19131 2024-04-29 12:55:58.998326 droid_metapatch-2.0.1/metapatch/metapatch.py
--rw-r--r--   0        0        0     7849 2024-04-29 12:55:58.998326 droid_metapatch-2.0.1/metapatch/options.py
--rw-r--r--   0        0        0      697 2024-04-29 12:55:58.998326 droid_metapatch-2.0.1/metapatch/utils.py
--rw-r--r--   0        0        0      822 2024-04-29 12:55:58.998326 droid_metapatch-2.0.1/pyproject.toml
--rw-r--r--   0        0        0    23594 1970-01-01 00:00:00.000000 droid_metapatch-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-05 07:25:44.339270 droid_metapatch-2.0.2/LICENSE
+-rw-r--r--   0        0        0    22794 2024-05-05 07:25:44.339270 droid_metapatch-2.0.2/README.md
+-rw-r--r--   0        0        0      366 2024-05-05 07:25:44.339270 droid_metapatch-2.0.2/metapatch/__init__.py
+-rw-r--r--   0        0        0     2533 2024-05-05 07:25:44.339270 droid_metapatch-2.0.2/metapatch/base.py
+-rw-r--r--   0        0        0     2029 2024-05-05 07:25:44.339270 droid_metapatch-2.0.2/metapatch/circuits/README.md
+-rw-r--r--   0        0        0     2547 2024-05-05 07:25:44.339270 droid_metapatch-2.0.2/metapatch/circuits/__init__.py
+-rw-r--r--   0        0        0     6255 2024-05-05 07:25:44.339270 droid_metapatch-2.0.2/metapatch/circuits/base.py
+-rw-r--r--   0        0        0    15356 2024-05-05 07:25:44.339270 droid_metapatch-2.0.2/metapatch/circuits/clock.py
+-rw-r--r--   0        0        0    53179 2024-05-05 07:25:44.339270 droid_metapatch-2.0.2/metapatch/circuits/cv.py
+-rw-r--r--   0        0        0     9625 2024-05-05 07:25:44.339270 droid_metapatch-2.0.2/metapatch/circuits/deprecated.py
+-rw-r--r--   0        0        0    23303 2024-05-05 07:25:44.339270 droid_metapatch-2.0.2/metapatch/circuits/logic.py
+-rw-r--r--   0        0        0   178579 2024-05-05 07:25:44.339270 droid_metapatch-2.0.2/metapatch/circuits/midi.py
+-rw-r--r--   0        0        0    22942 2024-05-05 07:25:44.339270 droid_metapatch-2.0.2/metapatch/circuits/modulation.py
+-rw-r--r--   0        0        0    19455 2024-05-05 07:25:44.339270 droid_metapatch-2.0.2/metapatch/circuits/other.py
+-rw-r--r--   0        0        0    37744 2024-05-05 07:25:44.343270 droid_metapatch-2.0.2/metapatch/circuits/pitch.py
+-rw-r--r--   0        0        0   149008 2024-05-05 07:25:44.343270 droid_metapatch-2.0.2/metapatch/circuits/sequencing.py
+-rw-r--r--   0        0        0   145502 2024-05-05 07:25:44.343270 droid_metapatch-2.0.2/metapatch/circuits/ui.py
+-rwxr-xr-x   0        0        0     3473 2024-05-05 07:25:44.343270 droid_metapatch-2.0.2/metapatch/cli_util.py
+-rw-r--r--   0        0        0      149 2024-05-05 07:25:44.343270 droid_metapatch-2.0.2/metapatch/factory/__init__.py
+-rw-r--r--   0        0        0     6591 2024-05-05 07:25:44.343270 droid_metapatch-2.0.2/metapatch/factory/boilerplate.py
+-rw-r--r--   0        0        0     3380 2024-05-05 07:25:44.343270 droid_metapatch-2.0.2/metapatch/factory/context.py
+-rw-r--r--   0        0        0     4281 2024-05-05 07:25:44.343270 droid_metapatch-2.0.2/metapatch/factory/formatting.py
+-rw-r--r--   0        0        0     7478 2024-05-05 07:25:44.343270 droid_metapatch-2.0.2/metapatch/factory/patch_factory.py
+-rw-r--r--   0        0        0     4565 2024-05-05 07:25:44.343270 droid_metapatch-2.0.2/metapatch/factory/patch_parser.py
+-rw-r--r--   0        0        0    19131 2024-05-05 07:25:44.343270 droid_metapatch-2.0.2/metapatch/metapatch.py
+-rw-r--r--   0        0        0     7859 2024-05-05 07:25:44.343270 droid_metapatch-2.0.2/metapatch/options.py
+-rw-r--r--   0        0        0      697 2024-05-05 07:25:44.343270 droid_metapatch-2.0.2/metapatch/utils.py
+-rw-r--r--   0        0        0      822 2024-05-05 07:25:44.343270 droid_metapatch-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0    23594 1970-01-01 00:00:00.000000 droid_metapatch-2.0.2/PKG-INFO
```

### Comparing `droid_metapatch-2.0.1/LICENSE` & `droid_metapatch-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `droid_metapatch-2.0.1/README.md` & `droid_metapatch-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `droid_metapatch-2.0.1/metapatch/base.py` & `droid_metapatch-2.0.2/metapatch/base.py`

 * *Files identical despite different names*

### Comparing `droid_metapatch-2.0.1/metapatch/circuits/README.md` & `droid_metapatch-2.0.2/metapatch/circuits/README.md`

 * *Files identical despite different names*

### Comparing `droid_metapatch-2.0.1/metapatch/circuits/__init__.py` & `droid_metapatch-2.0.2/metapatch/circuits/__init__.py`

 * *Files identical despite different names*

### Comparing `droid_metapatch-2.0.1/metapatch/circuits/base.py` & `droid_metapatch-2.0.2/metapatch/circuits/base.py`

 * *Files identical despite different names*

### Comparing `droid_metapatch-2.0.1/metapatch/circuits/clock.py` & `droid_metapatch-2.0.2/metapatch/circuits/clock.py`

 * *Files identical despite different names*

### Comparing `droid_metapatch-2.0.1/metapatch/circuits/cv.py` & `droid_metapatch-2.0.2/metapatch/circuits/cv.py`

 * *Files identical despite different names*

### Comparing `droid_metapatch-2.0.1/metapatch/circuits/deprecated.py` & `droid_metapatch-2.0.2/metapatch/circuits/deprecated.py`

 * *Files identical despite different names*

### Comparing `droid_metapatch-2.0.1/metapatch/circuits/logic.py` & `droid_metapatch-2.0.2/metapatch/circuits/logic.py`

 * *Files identical despite different names*

### Comparing `droid_metapatch-2.0.1/metapatch/circuits/midi.py` & `droid_metapatch-2.0.2/metapatch/circuits/midi.py`

 * *Files identical despite different names*

### Comparing `droid_metapatch-2.0.1/metapatch/circuits/modulation.py` & `droid_metapatch-2.0.2/metapatch/circuits/modulation.py`

 * *Files identical despite different names*

### Comparing `droid_metapatch-2.0.1/metapatch/circuits/other.py` & `droid_metapatch-2.0.2/metapatch/circuits/other.py`

 * *Files identical despite different names*

### Comparing `droid_metapatch-2.0.1/metapatch/circuits/pitch.py` & `droid_metapatch-2.0.2/metapatch/circuits/pitch.py`

 * *Files identical despite different names*

### Comparing `droid_metapatch-2.0.1/metapatch/circuits/sequencing.py` & `droid_metapatch-2.0.2/metapatch/circuits/sequencing.py`

 * *Files identical despite different names*

### Comparing `droid_metapatch-2.0.1/metapatch/circuits/ui.py` & `droid_metapatch-2.0.2/metapatch/circuits/ui.py`

 * *Files identical despite different names*

### Comparing `droid_metapatch-2.0.1/metapatch/cli_util.py` & `droid_metapatch-2.0.2/metapatch/cli_util.py`

 * *Files identical despite different names*

### Comparing `droid_metapatch-2.0.1/metapatch/factory/boilerplate.py` & `droid_metapatch-2.0.2/metapatch/factory/boilerplate.py`

 * *Files identical despite different names*

### Comparing `droid_metapatch-2.0.1/metapatch/factory/context.py` & `droid_metapatch-2.0.2/metapatch/factory/context.py`

 * *Files identical despite different names*

### Comparing `droid_metapatch-2.0.1/metapatch/factory/formatting.py` & `droid_metapatch-2.0.2/metapatch/factory/formatting.py`

 * *Files identical despite different names*

### Comparing `droid_metapatch-2.0.1/metapatch/factory/patch_factory.py` & `droid_metapatch-2.0.2/metapatch/factory/patch_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,16 @@
     return str(context)
 
 
 def _generate_circuit_params(circuit: TCircuitParams, level: int = 2) -> str:
     """Generate the parameters for a circuit."""
     context = TemplateContext(level)
     for key, value in circuit.items():
+        if not key:
+            continue
         if key.startswith("__"):
             continue
         if key in keyword.kwlist:
             key += "_"
         statement = context.eval_template(
             "fun_quoted_assignment", key=key, val=value, comma=True
         )
```

### Comparing `droid_metapatch-2.0.1/metapatch/factory/patch_parser.py` & `droid_metapatch-2.0.2/metapatch/factory/patch_parser.py`

 * *Files identical despite different names*

### Comparing `droid_metapatch-2.0.1/metapatch/metapatch.py` & `droid_metapatch-2.0.2/metapatch/metapatch.py`

 * *Files identical despite different names*

### Comparing `droid_metapatch-2.0.1/metapatch/options.py` & `droid_metapatch-2.0.2/metapatch/options.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,17 +56,17 @@
 
 class BoolOption(Option):
     """Boolean option."""
 
     def get_value(self) -> bool:
         """Return value."""
         if isinstance(self.value, str):
-            if self.value.lower() in ("false", "off", "no"):
+            if self.value.lower() in ("false", "off", "no", "0"):
                 return False
-            elif self.value.lower() in ("true", "on", "yes"):
+            elif self.value.lower() in ("true", "on", "yes", "1"):
                 return True
 
         return bool(self.value)
 
     @classmethod
     def from_default(cls) -> "BoolOption":
         """Instantiate with default value."""
```

### Comparing `droid_metapatch-2.0.1/metapatch/utils.py` & `droid_metapatch-2.0.2/metapatch/utils.py`

 * *Files identical despite different names*

### Comparing `droid_metapatch-2.0.1/pyproject.toml` & `droid_metapatch-2.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "droid-metapatch"
-version = "2.0.1"
+version = "2.0.2"
 description = "DROID patch generator"
 authors = ["Allan Eising <allan@eising.dk>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 documentation = "https://eising.github.io/droid-metapatch"
 repository = "https://github.com/Eising/droid-metapatch"
 packages = [{include = "metapatch"}]
```

### Comparing `droid_metapatch-2.0.1/PKG-INFO` & `droid_metapatch-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: droid-metapatch
-Version: 2.0.1
+Version: 2.0.2
 Summary: DROID patch generator
 Home-page: https://github.com/Eising/droid-metapatch
 License: GPL-3.0-only
 Author: Allan Eising
 Author-email: allan@eising.dk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

