# Comparing `tmp/picle-0.5.2.tar.gz` & `tmp/picle-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picle-0.5.2.tar", max compression
+gzip compressed data, was "picle-0.5.3.tar", max compression
```

## Comparing `picle-0.5.2.tar` & `picle-0.5.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-01-01 02:30:45.840067 picle-0.5.2/LICENSE
--rw-r--r--   0        0        0       80 2024-04-05 01:13:50.673276 picle-0.5.2/picle/__init__.py
--rw-r--r--   0        0        0     4531 2024-03-16 10:14:19.744008 picle-0.5.2/picle/cache.py
--rw-r--r--   0        0        0     5267 2024-04-13 21:16:46.255110 picle-0.5.2/picle/models.py
--rw-r--r--   0        0        0    34002 2024-04-07 05:51:45.023230 picle-0.5.2/picle/picle.py
--rw-r--r--   0        0        0      354 2024-04-05 03:31:06.926191 picle-0.5.2/picle/utils.py
--rw-r--r--   0        0        0     1659 2024-04-13 21:17:02.565143 picle-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     1329 2024-03-19 10:44:18.402593 picle-0.5.2/README.md
--rw-r--r--   0        0        0     2816 1970-01-01 00:00:00.000000 picle-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-01-01 02:30:45.840067 picle-0.5.3/LICENSE
+-rw-r--r--   0        0        0       80 2024-04-05 01:13:50.673276 picle-0.5.3/picle/__init__.py
+-rw-r--r--   0        0        0     4531 2024-03-16 10:14:19.744008 picle-0.5.3/picle/cache.py
+-rw-r--r--   0        0        0     6675 2024-05-05 11:29:07.134178 picle-0.5.3/picle/models.py
+-rw-r--r--   0        0        0    34665 2024-05-05 11:29:07.290358 picle-0.5.3/picle/picle.py
+-rw-r--r--   0        0        0      354 2024-04-05 03:31:06.926191 picle-0.5.3/picle/utils.py
+-rw-r--r--   0        0        0     1659 2024-05-05 11:32:14.990040 picle-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     1329 2024-03-19 10:44:18.402593 picle-0.5.3/README.md
+-rw-r--r--   0        0        0     2816 1970-01-01 00:00:00.000000 picle-0.5.3/PKG-INFO
```

### Comparing `picle-0.5.2/LICENSE` & `picle-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `picle-0.5.2/picle/cache.py` & `picle-0.5.3/picle/cache.py`

 * *Files identical despite different names*

### Comparing `picle-0.5.2/picle/models.py` & `picle-0.5.3/picle/models.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 
     HAS_YAML = True
 except ImportError:
     HAS_YAML = False
 
 try:
     from rich.console import Console as rich_console
-    from rich.table import Table as rich_table
-    from rich.pretty import pprint as rich_pprint
+    from rich.table import Table as RICHTABLE
 
     RICHCONSOLE = rich_console()
     HAS_RICH = True
 except ImportError:
     HAS_RICH = False
 
 
@@ -131,14 +130,19 @@
         json_schema_extra={"function": "outputter_rich_json"},
     )
     rich_print: Any = Field(
         None,
         description="Pretty print output using Rich",
         json_schema_extra={"function": "outputter_rich_print"},
     )
+    rich_table: Any = Field(
+        None,
+        description="Pretty print table output using Rich",
+        json_schema_extra={"function": "outputter_rich_table"},
+    )
 
     @staticmethod
     def outputter_rich_json(data: Union[dict, list]) -> None:
         """
         Function to pretty print JSON string using Rich library
 
         :param data: any data to print
@@ -166,14 +170,52 @@
         :param data: any data to print
         """
         if HAS_RICH:
             RICHCONSOLE.print(data)
         else:
             print(data)
 
+    @staticmethod
+    def outputter_rich_table(
+        data: list[dict], headers: list = None, title: str = None, sortby: str = None
+    ):
+        """
+        Function to pretty print output in table format using Rich library
+
+        :param data: list of dictionaries to print
+        """
+        if not HAS_RICH or not isinstance(data, list):
+            print(data)
+            return
+
+        headers = headers or list(data[0].keys())
+        table = RICHTABLE(title=title, box=False)
+
+        # add table columns
+        for h in headers:
+            table.add_column(h, justify="left", no_wrap=True)
+
+        # sort the table
+        if sortby:
+            # form dictionary keyed by sortby value and index
+            items_to_sortby = {i[sortby]: index for index, i in enumerate(data)}
+            # form a list of sorted sortby values
+            sorted_keys = sorted(items_to_sortby.keys())
+            # for sorted data list
+            sorted_data = [data[items_to_sortby[key]] for key in sorted_keys]
+        else:
+            sorted_data = data
+
+        # add table rows
+        for item in sorted_data:
+            cells = [item.get(h, "") for h in headers]
+            table.add_row(*cells)
+
+        RICHCONSOLE.print(table)
+
 
 class PipeFunctionsModel(Filters, Formatters, Outputters):
     """
     Collection of common pipe functions to use in PICLE shell models
     """
 
     class PicleConfig:
```

### Comparing `picle-0.5.2/picle/picle.py` & `picle-0.5.3/picle/picle.py`

 * *Files 3% similar despite different names*

```diff
@@ -232,17 +232,18 @@
                             "model": current_model["model"].PicleConfig.pipe,
                             "fields": [],
                             "parameter": parameter,
                         }
                     models = [current_model]
                     ret.append(models)
                 else:
-                    raise SyntaxError(
+                    log.error(
                         f"'{current_model['model'].__name__}' does not support pipe handling"
                     )
+                    break
             # collect single quoted field value
             elif '"' in parameter and current_field:
                 value_items = [parameter.replace('"', "")]
                 # collect further values if first parameter not double quoted value e.g. "nrp1"
                 if parameter.count('"') != 2:
                     while parameters:
                         parameter = parameters.pop(0)
@@ -617,17 +618,37 @@
                         for f in model["fields"]
                         if f["values"] is not ...
                     }
                     # collect command defaults
                     command_defaults = {}
                     for model in command:
                         command_defaults.update(model.get("defaults", {}))
-                    # run model "run" function if it exits
                     model = command[-1]["model"]
-                    if command_arguments and hasattr(model, "run"):
+                    # check if model has subshell
+                    if (
+                        not command_arguments
+                        and hasattr(model, "PicleConfig")
+                        and getattr(model.PicleConfig, "subshell", None) is True
+                    ):
+                        # collect parent shells and defaults
+                        for item in command[:-1]:
+                            m = item["model"]
+                            self.defaults_update(m)  # store shell defaults
+                            if (
+                                hasattr(m, "PicleConfig")
+                                and getattr(m.PicleConfig, "subshell", None) is True
+                            ):
+                                if m not in self.shells:
+                                    self.shells.append(m)
+                        # update prompt value
+                        self.prompt = getattr(model.PicleConfig, "prompt", self.prompt)
+                        self.shell = model
+                        self.shells.append(self.shell)
+                    # run model "run" function if it exits
+                    elif hasattr(model, "run"):
                         # validate command argument values
                         self._validate_values(command)
                         # call first command using collected arguments only
                         if index == 0:
                             kw = {
                                 **self.shell_defaults,
                                 **command_defaults,
@@ -651,33 +672,17 @@
                                         ret = processor(ret)
                         # extract outputter from PicleConfig
                         if index == 0:
                             if hasattr(model, "PicleConfig") and hasattr(
                                 model.PicleConfig, "outputter"
                             ):
                                 outputter = model.PicleConfig.outputter
-                    # check if model has subshell
-                    elif (
-                        hasattr(model, "PicleConfig")
-                        and getattr(model.PicleConfig, "subshell", None) is True
-                    ):
-                        # collect parent shells and defaults
-                        for item in command[:-1]:
-                            m = item["model"]
-                            self.defaults_update(m)  # store shell defaults
-                            if (
-                                hasattr(m, "PicleConfig")
-                                and getattr(m.PicleConfig, "subshell", None) is True
-                            ):
-                                if m not in self.shells:
-                                    self.shells.append(m)
-                        # update prompt value
-                        self.prompt = getattr(model.PicleConfig, "prompt", self.prompt)
-                        self.shell = model
-                        self.shells.append(self.shell)
+                                outputter_kwargs = getattr(
+                                    model.PicleConfig, "outputter_kwargs", {}
+                                )
                     # run command using Callable or json_schema_extra["function"]
                     elif command[-1]["fields"]:
                         # validate command argument values
                         self._validate_values(command)
                         # extract last field
                         last_field_name = command[-1]["fields"][-1]["name"]
                         last_field = model.model_fields[last_field_name]
@@ -750,27 +755,35 @@
                                     if callable(processor):
                                         ret = processor(ret)
                         # extract outputter from first command
                         if index == 0:
                             # use outputter from Field definition
                             if json_schema_extra.get("outputter"):
                                 outputter = json_schema_extra["outputter"]
+                                outputter_kwargs = json_schema_extra.get(
+                                    "outputter_kwargs", {}
+                                )
                             # use PicleConfig outputter
                             elif hasattr(model, "PicleConfig") and hasattr(
                                 model.PicleConfig, "outputter"
                             ):
                                 outputter = model.PicleConfig.outputter
+                                outputter_kwargs = getattr(
+                                    model.PicleConfig, "outputter_kwargs", {}
+                                )
                     else:
+                        print(line)
+                        print(model)
                         self.defaults_pop(model)
                         ret = f"Incorrect command"
                         break
 
         # returning True will close the shell exit
         if ret is True:
             return True
         elif ret:
             # use specified outputter to output results
             if callable(outputter):
-                outputter(ret)
+                outputter(ret, **outputter_kwargs)
             # write to stdout by default
             else:
                 self.write(ret)
```

### Comparing `picle-0.5.2/pyproject.toml` & `picle-0.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "picle"
-version = "0.5.2"
+version = "0.5.3"
 description = "Python Interactive Command Line Shells"
 authors = ["Denis Mulyalin <d.mulyalin@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/dmulyalin/picle"
 repository = "https://github.com/dmulyalin/picle"
 documentation = "https://dmulyalin.github.io/picle/"
```

### Comparing `picle-0.5.2/README.md` & `picle-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `picle-0.5.2/PKG-INFO` & `picle-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picle
-Version: 0.5.2
+Version: 0.5.3
 Summary: Python Interactive Command Line Shells
 Home-page: https://github.com/dmulyalin/picle
 License: MIT
 Author: Denis Mulyalin
 Author-email: d.mulyalin@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

