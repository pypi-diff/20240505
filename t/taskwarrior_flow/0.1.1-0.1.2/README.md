# Comparing `tmp/taskwarrior_flow-0.1.1.tar.gz` & `tmp/taskwarrior_flow-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskwarrior_flow-0.1.1.tar", max compression
+gzip compressed data, was "taskwarrior_flow-0.1.2.tar", max compression
```

## Comparing `taskwarrior_flow-0.1.1.tar` & `taskwarrior_flow-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2024-05-04 09:20:20.622506 taskwarrior_flow-0.1.1/LICENSE
--rw-r--r--   0        0        0     1126 2024-05-04 09:20:20.622506 taskwarrior_flow-0.1.1/README.md
--rw-r--r--   0        0        0      868 2024-05-04 09:20:20.622506 taskwarrior_flow-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      868 2024-05-04 09:20:20.622506 taskwarrior_flow-0.1.1/tools/__init__.py
--rw-r--r--   0        0        0      761 2024-05-04 09:20:20.622506 taskwarrior_flow-0.1.1/tools/main.py
--rw-r--r--   0        0        0    13156 2024-05-04 09:20:20.622506 taskwarrior_flow-0.1.1/tools/utils.py
--rw-r--r--   0        0        0     1705 1970-01-01 00:00:00.000000 taskwarrior_flow-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-04 12:03:13.630859 taskwarrior_flow-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1126 2024-05-04 12:03:13.630859 taskwarrior_flow-0.1.2/README.md
+-rw-r--r--   0        0        0      868 2024-05-04 12:03:13.630859 taskwarrior_flow-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      868 2024-05-04 12:03:13.630859 taskwarrior_flow-0.1.2/tools/__init__.py
+-rw-r--r--   0        0        0      761 2024-05-04 12:03:13.630859 taskwarrior_flow-0.1.2/tools/main.py
+-rw-r--r--   0        0        0    13184 2024-05-04 12:03:13.630859 taskwarrior_flow-0.1.2/tools/utils.py
+-rw-r--r--   0        0        0     1705 1970-01-01 00:00:00.000000 taskwarrior_flow-0.1.2/PKG-INFO
```

### Comparing `taskwarrior_flow-0.1.1/LICENSE` & `taskwarrior_flow-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `taskwarrior_flow-0.1.1/README.md` & `taskwarrior_flow-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `taskwarrior_flow-0.1.1/pyproject.toml` & `taskwarrior_flow-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskwarrior_flow"
-version = "0.1.1"
+version = "0.1.2"
 description = "Set of helpers for improving Taskwarrior workflow"
 authors = ["Ben Trinh <huantrinh1802@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "tools" }]
 
 [tool.poetry.scripts]
 twf = 'tools.main:app'
```

### Comparing `taskwarrior_flow-0.1.1/tools/__init__.py` & `taskwarrior_flow-0.1.2/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `taskwarrior_flow-0.1.1/tools/main.py` & `taskwarrior_flow-0.1.2/tools/main.py`

 * *Files identical despite different names*

### Comparing `taskwarrior_flow-0.1.1/tools/utils.py` & `taskwarrior_flow-0.1.2/tools/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,24 +115,24 @@
         else:
             questions[name] = questionary.text(f"Enter {name}", instruction="Use ';' for list\n", style=question_style)
     answers = safe_ask(questionary.form(**questions))
     if answers is None:
         return
     parts = ""
     annotations: None | list[str] = None
-    for name, field in tw_config["add_templates"]["data"][0]["fields"].items():
+    for name, field in tw_config["add_templates"]["data"][chosen_template]["fields"].items():
         value = answers.get(name, "")
         if len(value) != 0 or answers[name] != " ":
             if name in "annotations":
                 annotations = [annotation for annotation in answers[name].split(";")]
             else:
                 parts += " " + " ".join(
                     field.replace("%s", item) if item != "" else "" for item in answers[name].split(";")
                 )
-    command = tw_config["add_templates"]["data"][0]["command"].replace("%s", parts)
+    command = tw_config["add_templates"]["data"][chosen_template]["command"].replace("%s", parts)
     confirm = safe_ask(questionary.confirm("Add task?", instruction=f"\n{command}\n", style=question_style))
     if confirm:
         uuid_compiled = re.compile(r"[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}")
         result = subprocess.run(
             f"{group_mappings[group]} task rc.verbose=new-uuid {command}",
             capture_output=True,
             text=True,
```

### Comparing `taskwarrior_flow-0.1.1/PKG-INFO` & `taskwarrior_flow-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskwarrior_flow
-Version: 0.1.1
+Version: 0.1.2
 Summary: Set of helpers for improving Taskwarrior workflow
 Author: Ben Trinh
 Author-email: huantrinh1802@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

