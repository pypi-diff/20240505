# Comparing `tmp/simple_gcp_project_switcher-0.1.8.tar.gz` & `tmp/simple_gcp_project_switcher-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_gcp_project_switcher-0.1.8.tar", max compression
+gzip compressed data, was "simple_gcp_project_switcher-0.1.9.tar", max compression
```

## Comparing `simple_gcp_project_switcher-0.1.8.tar` & `simple_gcp_project_switcher-0.1.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      417 2023-11-10 00:27:17.529514 simple_gcp_project_switcher-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-11-09 23:42:55.019056 simple_gcp_project_switcher-0.1.8/pswitch/__init__.py
--rw-r--r--   0        0        0      608 2023-11-10 00:22:22.848262 simple_gcp_project_switcher-0.1.8/pswitch/console.py
--rw-r--r--   0        0        0      502 2023-11-10 00:33:16.776912 simple_gcp_project_switcher-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1242 1970-01-01 00:00:00.000000 simple_gcp_project_switcher-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      929 2023-11-10 02:07:28.170539 simple_gcp_project_switcher-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-11-09 23:42:55.019056 simple_gcp_project_switcher-0.1.9/pswitch/__init__.py
+-rw-r--r--   0        0        0      782 2023-11-10 01:55:46.012815 simple_gcp_project_switcher-0.1.9/pswitch/console.py
+-rw-r--r--   0        0        0      502 2023-11-10 02:07:59.441737 simple_gcp_project_switcher-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1754 1970-01-01 00:00:00.000000 simple_gcp_project_switcher-0.1.9/PKG-INFO
```

### Comparing `simple_gcp_project_switcher-0.1.8/pswitch/console.py` & `simple_gcp_project_switcher-0.1.9/pswitch/console.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 import sys, json, os
 import subprocess
 
-def main():
+
+def switch_project():
     try:
         search = sys.argv[1]    
     except:
         search = ""
     pr = subprocess.check_output(f'gcloud projects list --filter={search} --format="json(name,projectId,parent.id)"', shell=True)
     projects = json.loads(pr)
     for id, project in enumerate(projects):
         print(f'[{id}] : {project["name"]} ({project["projectId"]})')
     projNum = input("Enter project number to switch to: ")
     try:
         os.system(f'gcloud config set project "{projects[int(projNum)]["projectId"]}"')
     except:
         print("Invalid Project Number")
+
+def main():
+    try:
+        switch_project()
+    except SystemExit:
+        print("Program exited")
+    except KeyboardInterrupt:
+        print("Program exited")
```

