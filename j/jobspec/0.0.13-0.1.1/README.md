# Comparing `tmp/jobspec-0.0.13.tar.gz` & `tmp/jobspec-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobspec-0.0.13.tar", last modified: Thu Mar 21 08:12:11 2024, max compression
+gzip compressed data, was "jobspec-0.1.1.tar", last modified: Sun May  5 18:39:17 2024, max compression
```

## Comparing `jobspec-0.0.13.tar` & `jobspec-0.1.1.tar`

### file list

```diff
@@ -1,44 +1,50 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-03-21 08:12:11.118698 jobspec-0.0.13/
--rw-r--r--   0 vanessa   (1000) vanessa   (1000)     1108 2024-03-18 02:06:39.000000 jobspec-0.0.13/LICENSE
--rw-r--r--   0 vanessa   (1000) vanessa   (1000)      135 2024-03-18 01:36:51.000000 jobspec-0.0.13/MANIFEST.in
--rw-r--r--   0 vanessa   (1000) vanessa   (1000)     1167 2024-03-18 02:06:33.000000 jobspec-0.0.13/NOTICE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12034 2024-03-21 08:12:11.118698 jobspec-0.0.13/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    11167 2024-03-19 22:33:15.000000 jobspec-0.0.13/README.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-03-21 08:12:11.118698 jobspec-0.0.13/jobspec/
--rw-r--r--   0 vanessa   (1000) vanessa   (1000)        0 2024-03-18 01:10:49.000000 jobspec-0.0.13/jobspec/__init__.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-03-21 08:12:11.118698 jobspec-0.0.13/jobspec/cli/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2595 2024-03-18 21:29:51.000000 jobspec-0.0.13/jobspec/cli/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      603 2024-03-18 21:29:51.000000 jobspec-0.0.13/jobspec/cli/run.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-03-21 08:12:11.118698 jobspec-0.0.13/jobspec/core/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      381 2024-03-18 21:29:51.000000 jobspec-0.0.13/jobspec/core/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2684 2024-03-18 01:10:49.000000 jobspec-0.0.13/jobspec/core/converter.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2357 2024-03-18 21:29:51.000000 jobspec-0.0.13/jobspec/core/core.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       55 2024-03-19 22:33:15.000000 jobspec-0.0.13/jobspec/defaults.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5612 2024-03-18 21:29:51.000000 jobspec-0.0.13/jobspec/logger.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-03-21 08:12:11.118698 jobspec-0.0.13/jobspec/plugin/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      247 2024-03-18 21:29:51.000000 jobspec-0.0.13/jobspec/plugin/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3389 2024-03-18 21:29:51.000000 jobspec-0.0.13/jobspec/plugin/registry.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4532 2024-03-19 22:33:15.000000 jobspec-0.0.13/jobspec/runner.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     9974 2024-03-21 08:11:54.000000 jobspec-0.0.13/jobspec/schema.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-03-21 08:12:11.118698 jobspec-0.0.13/jobspec/steps/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       60 2024-03-18 22:39:54.000000 jobspec-0.0.13/jobspec/steps/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2407 2024-03-18 22:39:54.000000 jobspec-0.0.13/jobspec/steps/base.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      294 2024-03-18 22:39:54.000000 jobspec-0.0.13/jobspec/steps/empty.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1407 2024-03-19 01:17:39.000000 jobspec-0.0.13/jobspec/steps/fileio.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      627 2024-03-18 22:39:54.000000 jobspec-0.0.13/jobspec/steps/helpers.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-03-21 08:12:11.118698 jobspec-0.0.13/jobspec/transformer/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       78 2024-03-18 21:29:51.000000 jobspec-0.0.13/jobspec/transformer/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4477 2024-03-19 22:33:15.000000 jobspec-0.0.13/jobspec/transformer/flux.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2311 2024-03-19 22:33:15.000000 jobspec-0.0.13/jobspec/utils.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      608 2024-03-21 08:11:54.000000 jobspec-0.0.13/jobspec/version.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-03-21 08:12:11.118698 jobspec-0.0.13/jobspec.egg-info/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12034 2024-03-21 08:12:11.000000 jobspec-0.0.13/jobspec.egg-info/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      767 2024-03-21 08:12:11.000000 jobspec-0.0.13/jobspec.egg-info/SOURCES.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2024-03-21 08:12:11.000000 jobspec-0.0.13/jobspec.egg-info/dependency_links.txt
--rw-r--r--   0 vanessa   (1000) vanessa   (1000)       52 2024-03-21 08:12:11.000000 jobspec-0.0.13/jobspec.egg-info/entry_points.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2024-03-18 01:37:11.000000 jobspec-0.0.13/jobspec.egg-info/not-zip-safe
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       43 2024-03-21 08:12:11.000000 jobspec-0.0.13/jobspec.egg-info/requires.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        8 2024-03-21 08:12:11.000000 jobspec-0.0.13/jobspec.egg-info/top_level.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      168 2024-03-18 01:10:50.000000 jobspec-0.0.13/pyproject.toml
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      152 2024-03-21 08:12:11.118698 jobspec-0.0.13/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3433 2024-03-18 21:29:51.000000 jobspec-0.0.13/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:39:17.479181 jobspec-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-05 18:38:50.000000 jobspec-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-05 18:38:50.000000 jobspec-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-05 18:38:50.000000 jobspec-0.1.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-05 18:39:17.479181 jobspec-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-05 18:38:50.000000 jobspec-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:39:17.475181 jobspec-0.1.1/jobspec/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:39:17.479181 jobspec-0.1.1/jobspec/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/cli/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:39:17.479181 jobspec-0.1.1/jobspec/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/core/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/core/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/core/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:39:17.479181 jobspec-0.1.1/jobspec/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/plugin/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7192 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:39:17.479181 jobspec-0.1.1/jobspec/steps/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/steps/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/steps/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/steps/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/steps/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:39:17.479181 jobspec-0.1.1/jobspec/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/transformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:39:17.479181 jobspec-0.1.1/jobspec/transformer/flux/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/transformer/flux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/transformer/flux/steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/transformer/flux/workload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/transformer/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-05 18:38:50.000000 jobspec-0.1.1/jobspec/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:39:17.475181 jobspec-0.1.1/jobspec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-05 18:39:17.000000 jobspec-0.1.1/jobspec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-05 18:39:17.000000 jobspec-0.1.1/jobspec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 18:39:17.000000 jobspec-0.1.1/jobspec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-05 18:39:17.000000 jobspec-0.1.1/jobspec.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 18:39:17.000000 jobspec-0.1.1/jobspec.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-05 18:39:17.000000 jobspec-0.1.1/jobspec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-05 18:39:17.000000 jobspec-0.1.1/jobspec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-05 18:38:50.000000 jobspec-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-05 18:39:17.479181 jobspec-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-05 18:38:50.000000 jobspec-0.1.1/setup.py
```

### Comparing `jobspec-0.0.13/LICENSE` & `jobspec-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jobspec-0.0.13/NOTICE` & `jobspec-0.1.1/NOTICE`

 * *Files identical despite different names*

### Comparing `jobspec-0.0.13/jobspec/cli/__init__.py` & `jobspec-0.1.1/jobspec/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `jobspec-0.0.13/jobspec/cli/run.py` & `jobspec-0.1.1/jobspec/cli/run.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 #!/usr/bin/env python
 
-import json
+import os
+import sys
 
-import jobspec.utils as utils
 
-
-def main(args, extra):
+def main(args, _):
     """
     Run an extraction. This can be converted to a proper function
     if needed.
     """
     from jobspec.plugin import get_transformer_registry
 
     registry = get_transformer_registry()
 
     # This raises an error if not found
     # This would be what we put in a Python script
     # that is in a cronjob, for loop receiver, etc.
     # We can add additional options to the init here
     plugin = registry.get_plugin(args.transform)()
 
+    # The jobspec needs to exist as a file here
+    if not os.path.exists(args.jobspec):
+        sys.exit(f"JobSpec {args.jobspec} does not exist.")
+
     # Run the plugin with the jobspec
     plugin.run(args.jobspec)
```

### Comparing `jobspec-0.0.13/jobspec/core/converter.py` & `jobspec-0.1.1/jobspec/core/converter.py`

 * *Files identical despite different names*

### Comparing `jobspec-0.0.13/jobspec/core/core.py` & `jobspec-0.1.1/jobspec/core/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,79 +1,100 @@
-# Note that jsonschema used to be a part of flux core but was dropped
-# https://github.com/flux-framework/flux-core/pull/5678/files
-
-import json
-import os
-
 import jsonschema
-import yaml
 
 import jobspec.schema as schema
-import jobspec.utils as utils
+
+from .base import ResourceBase
+from .resources import find_resources
 
 
-class Jobspec:
-    def __init__(self, filename, validate=True, schema=schema.jobspec_v2):
+class Jobspec(ResourceBase):
+    def __init__(self, filename, validate=True, schema=schema.jobspec_nextgen):
         """
-        Load in and validate a Flux Jobspec
+        Load in and validate a Jobspec
         """
         # This should typically be loaded from jobspec.core
         if not hasattr(self, "schema") or not self.schema:
             self.schema = schema
         self.filename = filename
-        self.jobspec = None
+        self.data = None
         self.load(filename)
         if validate:
             self.validate()
 
-    def to_str(self):
+    def validate(self):
         """
-        Convert to string, which is needed for the submit.
+        Validate the jsonschema
         """
-        return json.dumps(self.jobspec)
+        jsonschema.validate(self.data, self.schema)
 
-    def to_yaml(self):
+        # Require at least one of command or steps, unless it is a group
+        for task in self.data.get("tasks", []):
+            if "group" not in task and ("command" not in task and "steps" not in task):
+                raise ValueError("Jobspec is not valid, each task must have a command or steps")
+
+
+class Resources(ResourceBase):
+    def __init__(self, data, slot=None):
         """
-        Dump the jobspec to yaml string
+        Interact with loaded resources.
         """
-        return yaml.dump(self.jobspec)
+        self.data = data
+        self.slot = slot
 
-    @property
-    def name(self):
-        try:
-            return self.jobspec.get("tasks", {})[0]["command"][0]
-        except Exception:
-            return "app"
-
-    def load(self, filename):
+    def flatten_slot(self, slot=None):
         """
-        Load the jobspec
+        Find the task slot, flatten it, and return
         """
-        # Case 1: given a raw filename
-        if isinstance(filename, str) and os.path.exists(filename):
-            self.filename = os.path.abspath(filename)
+        slot = slot or self.slot
 
-            try:
-                self.jobspec = utils.read_json(self.filename)
-            except:
-                self.jobspec = utils.read_yaml(self.filename)
+        # Traverse each section. There is usually only one I guess
+        flat = {}
+        find_resources(flat, self.data, slot)
+        return flat
 
-        # Case 2: jobspec as dict (that we just want to validate)
-        elif isinstance(filename, dict):
-            self.jobspec = filename
-        # Case 3: jobspec as string
-        else:
-            self.jobspec = json.loads(filename)
 
-        # Case 4: wtf are you giving me? :X
-        if not self.jobspec:
-            raise ValueError("Unrecognized input format for jobspec.")
+class Attributes(ResourceBase):
+    """
+    Job attributes, not formally defined yet.
+    """
 
-    def validate(self):
+    pass
+
+
+class Requires(ResourceBase):
+    """
+    Requires are nested groups
+    """
+
+    def update(self, requires):
         """
-        Validate the jsonschema
+        Update specific groups. This is assumed
+        at the level of the attribute, not the group.
+        E.g., this at the global level:
+
+        requires:
+          io:
+            fieldA: valueA
+            fieldB: valueB
+
+        Updated with this:
+        requires:
+          io:
+            fieldB: valueC
+
+        Results in this:
+        requires:
+          io:
+            fieldA: valueA
+            fieldB: valueC
         """
-        jsonschema.validate(self.jobspec, self.schema)
-        # Require at least one of command, batch, or script
-        for task in self.jobspec.get("tasks", []):
-            if "command" not in task and "batch" not in task and "script" not in task:
-                raise ValueError("Jobspec is not valid, task is missing a command|script|batch")
+        if not requires:
+            return
+        for group, fields in requires.items():
+            # If we don't have the group at all, we can add all and continue!
+            if group not in self.data:
+                self.data[group] = fields
+                continue
+
+            # If we have the group, update on the level of fields
+            self.data[group].update(fields)
+        return self
```

### Comparing `jobspec-0.0.13/jobspec/logger.py` & `jobspec-0.1.1/jobspec/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -163,15 +163,14 @@
 def setup_logger(
     quiet=False,
     printshellcmds=False,
     nocolor=False,
     stdout=False,
     debug=False,
     use_threads=False,
-    wms_monitor=None,
 ):
     # console output only if no custom logger was specified
     stream_handler = ColorizingStreamHandler(
         nocolor=nocolor,
         stream=sys.stdout if stdout else sys.stderr,
         use_threads=use_threads,
     )
```

### Comparing `jobspec-0.0.13/jobspec/plugin/registry.py` & `jobspec-0.1.1/jobspec/plugin/registry.py`

 * *Files identical despite different names*

### Comparing `jobspec-0.0.13/jobspec/runner.py` & `jobspec-0.1.1/jobspec/runner.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-import copy
 import os
-import sys
 
 # This imports the latest version
 import jobspec.core as js
 import jobspec.defaults as defaults
-import jobspec.utils as utils
-from jobspec.logger import LogColors
+import jobspec.steps.runner as step_runner
 
 
 class TransformerBase:
     """
-    A Jobspec Transformer can load a Jobspec and transform for a particular environment.
+    A Transformer base is the core of a JobSpec
+
+    It loads a Jobspec and transforms for a particular environment
+    (which typically means a workload manager or similar). This is most
+    relevant for submit and batch commands, along with custom steps.
     """
 
     steps = {}
 
     def __init__(self, **options):
         """
-        Create a new graph backend, accepting any options type.
+        Create a new transformer backend, accepting any options type.
 
         Validation of transformers is done by the registry
         """
         # Set options as attributes
         for key, value in options.items():
             setattr(self, key, value)
 
@@ -37,102 +38,60 @@
         name = name or step.name
         cls.steps[name] = step
 
     def update_settings(self, settings, typ, step):
         """
         Update settings, either set or unset
         """
-        if "key" not in step or "value" not in step:
+        if "name" not in step or "value" not in step:
             return
         if not step["key"]:
             return
         # This is important for typos, etc.
         if step["key"] not in defaults.valid_settings:
             raise ValueError(f"{step['key']} is not a known setting.")
         if typ == "set":
             settings[step["key"]] = step["value"]
         elif typ == "unset" and step["key"] in settings:
             del settings[step["key"]]
 
     def parse(self, jobspec):
         """
-        parse validates transform logic and returns steps.
+        parse validates logic and returns a series of steps, which
+        will depend on the underlying transformer. It might be:
 
-        We also look for global variables for steps.
+        - a batch that includes logic to write a script and then run it
+        - one or more submit commands
         """
-        # We will return a listing of steps to complete
-        # Each step is provided all settings that are provided
-        # before it
-        steps = []
-
-        # Each filename directive must have a matching script
-        # It could be the case it exists (and we might mark that)
-        # but not for the time being
-        task = jobspec.jobspec.get("task")
-
-        # Global set settings
-        settings = {"sharedfs": defaults.sharedfs}
-
-        # Validate each step
-        for i, step in enumerate(task.get("transform")):
-            # The step must be known to the transformer
-            name = step.get("step")
-            if not name:
-                raise ValueError(f"Step in index {i} is missing a name")
-
-            # If it's a set or unset, add to settings
-            if name == "set" or name == "unset":
-                self.update_settings(settings, name, step)
-                continue
-
-            if name not in self.steps:
-                raise ValueError(f"Step {name} is not known to transformer {self.name}")
-
-            # This ensures we get the exact state of settings at this level
-            step["settings"] = copy.deepcopy(settings)
-
-            # Instantiate the new step (does extra validation), provided entire jobspec
-            new_step = self.steps[name](jobspec.jobspec, step)
-            steps.append(new_step)
-        return steps
+        raise NotImplementedError
+
+    def announce(self):
+        pass
+
+    def flatten(self, filename):
+        raise NotImplementedError
 
     def run(self, filename):
         """
         Run the transformer
         """
         # Load the jobspec
         jobspec = self.load_jobspec(filename)
 
         # Get validated transformation steps
+        # These will depend on the transformer logic
         steps = self.parse(jobspec)
-
-        # Create a temporary staging directory
-        stage = utils.get_tmpdir(prefix="jobspec-")
+        self.announce()
 
         # Run each step to submit the job, and that's it.
         for step in steps:
-            step_stage = stage or step["settings"].get("stage")
-            self.run_step(step, step_stage)
-
-    def run_step(self, step, stage):
-        """
-        Run a single step. Make it pretty.
-        """
-        prefix = f"step {step.name}".ljust(15)
-        print(f"=> {LogColors.OKCYAN}{prefix}{LogColors.ENDC}", end="")
-        try:
-            out = (step.run(stage) or "").ljust(25)
-            print(f"{LogColors.OKBLUE}{out}{LogColors.ENDC} {LogColors.OKGREEN}OK{LogColors.ENDC}")
-        except Exception as e:
-            print(f"\n{LogColors.RED}{str(e)}{LogColors.ENDC}")
-            sys.exit()
+            step_runner.run(self.name, step)
 
     def load_jobspec(self, filename):
         """
         Load and transform a jobspec.
 
         This function should be able to load it in some raw format
         and convert into correct directives given the transformer.
         """
         filename = os.path.abspath(filename)
-        jobspec = js.Jobspec(filename)
-        return jobspec
+        return js.Jobspec(filename)
```

### Comparing `jobspec-0.0.13/jobspec/steps/base.py` & `jobspec-0.1.1/jobspec/steps/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-import jobspec.steps.helpers as helpers
-
-
 class StepBase:
     """
     A base step describes the design of a step.
     """
 
     required = []
 
-    def __init__(self, js, options):
+    def __init__(self, js, **kwargs):
         """
         A step takes a task definition and custom options
+
+        Note that we aren't using options now, but could be.
         """
         self.jobspec = js
-        self.options = options
         if not hasattr(self, "name"):
             raise ValueError(f"Step {self} is missing a name")
 
+        # Each step can take custom options (the keyword arguments)
+        self.options = kwargs
+
         # Shared validation
         self._validate()
 
-        # Custom validation
+        # Custom validation and setup
         self.validate()
+        self.setup(**kwargs)
 
     def _validate(self):
         """
         Shared validation functions
         """
         # Required fields are all... required.
         for field in self.required:
@@ -36,52 +38,22 @@
 
     def validate(self):
         """
         Validate the step
         """
         pass
 
-    def flatten_slot(self):
-        """
-        Find the task slot, flatten it, and return
+    def setup(self, **kwargs):
         """
-        slot = self.jobspec["task"]["slot"]
-        resources = self.jobspec.get("resources", [])
-
-        # Traverse each section. There is usually only one I guess
-        for resource in resources:
-            flat = {}
-            if helpers.find_resources(flat, resource, slot):
-                break
+        Custom setup
 
-        return flat
-
-    @property
-    def scripts(self):
-        """
-        Return a lookup of scripts
-
-        Many steps will have need for this.
+        Akin to overriding init, but easier to write.
         """
-        if hasattr(self, "_scripts") and self._scripts is not None:
-            return self._scripts
-
-        # Task scripts must have a name and content
-        task = self.jobspec.get("task")
-        scripts = {}
-        if task:
-            for script in task.get("scripts"):
-                if "name" not in script:
-                    raise ValueError(f"Script {script} is missing a name.")
-                if "content" not in script:
-                    raise ValueError(f"Script {script} is missing content.")
-                scripts[script["name"]] = script
-        self._scripts = scripts
-        return scripts
+        pass
 
-    def run(self, stage, *args, **kwargs):
+    def run(self, *args, **kwargs):
         """
         Run a step.
 
         This is the argument structure that should be used.
         """
         raise NotImplementedError
```

### Comparing `jobspec-0.0.13/jobspec/steps/fileio.py` & `jobspec-0.1.1/jobspec/steps/fileio.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,23 +27,26 @@
 
         # 1. All filename directives must be defined in scripts
         if filename and filename not in names:
             raise ValueError(
                 f"Filename {filename} is defined for a {self.name} step but not in task scripts"
             )
 
-    def run(self, stage, *args, **kwargs):
+    def run(self, *args, **kwargs):
         """
-        write some content to a filename
+        write some content to a filename.
+
+        This is currently not used, as we can represent the same logic in a task.
 
         step: write
         filename: install.sh
         executable: true
         """
         filename = self.options.get("filename")
+        stage = self.options.get("stage")
         fullpath = os.path.join(stage, filename)
         utils.write_file(self.scripts[filename]["content"], fullpath)
 
         executable = self.options.get("executable") is True
         # Execute / search permissions for the user and others
         if executable:
             st = os.stat(fullpath)
```

### Comparing `jobspec-0.0.13/jobspec/utils.py` & `jobspec-0.1.1/jobspec/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,20 +19,37 @@
     Read in a file content
     """
     with open(filename, "r") as fd:
         content = fd.read()
     return content
 
 
+def get_tmpfile(tmpdir=None, prefix=""):
+    """
+    Get a temporary file with an optional prefix.
+    """
+    # First priority for the base goes to the user requested.
+    tmpdir = get_tmpdir(tmpdir)
+
+    # If tmpdir is set, add to prefix
+    if tmpdir:
+        prefix = os.path.join(tmpdir, os.path.basename(prefix))
+
+    fd, tmp_file = tempfile.mkstemp(prefix=prefix)
+    os.close(fd)
+
+    return tmp_file
+
+
 def get_tmpdir(tmpdir=None, prefix="", create=True):
     """
     Get a temporary directory for an operation.
     """
     tmpdir = tmpdir or tempfile.gettempdir()
-    prefix = prefix or "shpc-tmp"
+    prefix = prefix or "jobspec-"
     prefix = "%s.%s" % (prefix, next(tempfile._get_candidate_names()))
     tmpdir = os.path.join(tmpdir, prefix)
 
     if not os.path.exists(tmpdir) and create is True:
         os.mkdir(tmpdir)
 
     return tmpdir
```

### Comparing `jobspec-0.0.13/jobspec/version.py` & `jobspec-0.1.1/jobspec/version.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.13"
+__version__ = "0.1.1"
 AUTHOR = "Vanessa Sochat"
 AUTHOR_EMAIL = "vsoch@users.noreply.github.com"
 NAME = "jobspec"
 PACKAGE_URL = "https://github.com/compspec/jobspec"
 KEYWORDS = "cluster, orchestration, transformer, jobspec, flux"
 DESCRIPTION = "Jobspec specification and translation layer for cluster work"
 LICENSE = "LICENSE"
```

### Comparing `jobspec-0.0.13/setup.py` & `jobspec-0.1.1/setup.py`

 * *Files identical despite different names*

