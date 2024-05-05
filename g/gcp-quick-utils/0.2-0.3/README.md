# Comparing `tmp/gcp_quick_utils-0.2.tar.gz` & `tmp/gcp_quick_utils-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcp_quick_utils-0.2.tar", max compression
+gzip compressed data, was "gcp_quick_utils-0.3.tar", max compression
```

## Comparing `gcp_quick_utils-0.2.tar` & `gcp_quick_utils-0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2062 2024-05-04 16:44:51.351680 gcp_quick_utils-0.2/README.md
--rw-r--r--   0        0        0        0 2024-03-29 13:57:01.208519 gcp_quick_utils-0.2/gcpq/__init__.py
--rw-r--r--   0        0        0     1154 2024-05-04 16:58:05.551670 gcp_quick_utils-0.2/gcpq/cfg_service.py
--rw-r--r--   0        0        0     7746 2024-05-04 16:20:33.891700 gcp_quick_utils-0.2/gcpq/config/services.yaml
--rw-r--r--   0        0        0      182 2024-05-04 15:38:53.741731 gcp_quick_utils-0.2/gcpq/console_utils.py
--rw-r--r--   0        0        0     1104 2024-05-04 15:40:53.371728 gcp_quick_utils-0.2/gcpq/gcp_cli_service.py
--rw-r--r--   0        0        0      861 2024-05-04 16:45:04.981680 gcp_quick_utils-0.2/gcpq/gcp_sections_service.py
--rw-r--r--   0        0        0     2102 2024-05-04 16:45:04.981680 gcp_quick_utils-0.2/gcpq/main.py
--rw-r--r--   0        0        0      567 2024-05-04 16:44:51.351680 gcp_quick_utils-0.2/pyproject.toml
--rw-r--r--   0        0        0     2847 1970-01-01 00:00:00.000000 gcp_quick_utils-0.2/PKG-INFO
+-rw-r--r--   0        0        0     2100 2024-05-04 17:42:28.172187 gcp_quick_utils-0.3/README.md
+-rw-r--r--   0        0        0        0 2024-03-29 13:57:01.208519 gcp_quick_utils-0.3/gcpq/__init__.py
+-rw-r--r--   0        0        0     1862 2024-05-04 22:18:00.533922 gcp_quick_utils-0.3/gcpq/cfg_service.py
+-rw-r--r--   0        0        0     7746 2024-05-04 16:20:33.891700 gcp_quick_utils-0.3/gcpq/config/services.yaml
+-rw-r--r--   0        0        0      453 2024-05-04 22:57:37.353891 gcp_quick_utils-0.3/gcpq/console_utils.py
+-rw-r--r--   0        0        0     1504 2024-05-04 22:45:13.973900 gcp_quick_utils-0.3/gcpq/gcp_cli_service.py
+-rw-r--r--   0        0        0      861 2024-05-04 16:45:04.981680 gcp_quick_utils-0.3/gcpq/gcp_sections_service.py
+-rw-r--r--   0        0        0     2887 2024-05-04 22:51:17.573894 gcp_quick_utils-0.3/gcpq/main.py
+-rw-r--r--   0        0        0      567 2024-05-04 23:01:12.423876 gcp_quick_utils-0.3/pyproject.toml
+-rw-r--r--   0        0        0     2885 1970-01-01 00:00:00.000000 gcp_quick_utils-0.3/PKG-INFO
```

### Comparing `gcp_quick_utils-0.2/README.md` & `gcp_quick_utils-0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -11,78 +11,83 @@
 GCLOUD SDK has to be installed on your machine and you have to be logged in
 
 ## Usage
 
 ### Switch between projects
 If you want to list all projects before choosing one
 ```
-pgo s
+gcpq s
 ```
 
 If you want to search for a specific term in the project name or project id
 
 ```
-pgo s searchTerm
+gcpq s searchTerm
 ```
 
 You will see the following output to choose your project rom:
 
 ```
-$ pgo mycompanyName
+$ gcpq mycompanyName
 [0] : mycompany-380102 (mycompany)
 [1] : mycompany-airbyte (mycompany-airbyte)
 [2] : mycompany-chatbot (mycompany-chatbot)
 [3] : mycompany-etl (mycompany-etl)
 [4] : mycompany-ga4-lehoublon-flo (mycompany-ga4-lehoublon-flo)
 [5] : mycompany-guillaume-pde (mycompany-guillaume-pde)
 [6] : mycompany-n8n (mycompany-n8n)
 [7] : mycompany-terraform (mycompany-terraform)
 Enter project number to switch to: 
 ```
 
 If you want to automatically switch to the first found project
 ```
-pgo searchTerm -a
+gcpq searchTerm -a
 ```
 
 ### Opening Google Cloud Interface quickly
 
 If you want to open a service quickly. When you don't specify projects, the current Gcloud set project will be used
 
 ```
-pgo bq
+gcpq bq
 ```
 
 Open multiple services at the same time
 
 ```
-pgo bq,dataform,iam,build,gcs
+gcpq bq,dataform,iam,build,gcs
 ```
 
 Aliased have been created for the services. You can see them in the `services.yaml` file of the repo
 
 
 Open services on a specific project (you will be able to choose the project matching the search result)
 
 ```
-pgo bq myCompanyName
+gcpq bq myCompanyName
 ```
 
 Open services on a specific project automatically (Will open the first found project)
 
 ```
-pgo bq myCompanyName -a 
+gcpq bq myCompanyName -a 
 ```
 
 Create shortcuts of groups of services
 - Open your config file located in `~/.gcpq/config.yaml`
 - Add new groups of services in the file (follow current structure)
 
 
 ```
-pgo myGroupName 
+gcpq myGroupName 
 ```
 
 
 
-# Modifying GCPQU
-If you need to modify the package, you can test your modifications with poetry run pgo
+# Modifying GCPQ
+
+If you need to modify the package, you can test your modifications with poetry run gcpq
+
+```
+poetry run gcpq bq
+```
```

### Comparing `gcp_quick_utils-0.2/gcpq/cfg_service.py` & `gcp_quick_utils-0.3/gcpq/cfg_service.py`

 * *Files 27% similar despite different names*

```diff
@@ -17,22 +17,41 @@
     
     cfg_file_path = get_config_file_path()
     if not os.path.exists(cfg_file_path):
         with open(cfg_file_path, "w") as f:
             f.write(yaml.dump({"groups":{"dwh": ["bigquery", "dataform", "storage"] }}))
 
 def load_config():
-    #Get current file directory
-    print(os.path.dirname(__file__))
-    print(os.path.abspath(os.getcwd()))
-
     cfg_file_path = get_config_file_path()
     if not os.path.exists(cfg_file_path):
         install_command()
     config = yaml.load(open(cfg_file_path, "r"), Loader=yaml.SafeLoader)
     with open(f'{os.path.dirname(__file__)}/config/services.yaml', 'r') as f:
         services = yaml.load(f, Loader=yaml.SafeLoader)
     
     config["services"] = services
     return config
 
+def add_friendly_name(project):
+    cfg_file_path = get_config_file_path()
+    if not os.path.exists(cfg_file_path):
+        install_command()
+    personal_config = yaml.load(open(cfg_file_path, "r"), Loader=yaml.SafeLoader)
+    # check if key exists
+    if "projects" not in config:
+        personal_config["projects"] = []
+    
+    for proj in personal_config["projects"]:
+        if proj["projectId"] == project["projectId"]:
+            print("Project already exists in config - Updating")
+            proj.update(project)
+            with open(cfg_file_path, "w") as f:
+                f.write(yaml.dump(personal_config))
+            return
+
+    personal_config["projects"].append(project)
+    print(personal_config)
+    with open(cfg_file_path, "w") as f:
+        f.write(yaml.dump(personal_config))
+    return
+
 config = load_config()
```

### Comparing `gcp_quick_utils-0.2/gcpq/config/services.yaml` & `gcp_quick_utils-0.3/gcpq/config/services.yaml`

 * *Files identical despite different names*

### Comparing `gcp_quick_utils-0.2/gcpq/gcp_cli_service.py` & `gcp_quick_utils-0.3/gcpq/gcp_cli_service.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 # Description: This file contains the functions to interact with GCP projects through the CLI
 import os
 import subprocess
 import json
 
-def get_projects(search):
+def get_projects(search, projects_from_friendly=[]):
     command = 'gcloud projects list --format="json(name,projectId,parent.id)"'
     if search:
         command = f'{command} --filter={search}'
     pr = subprocess.check_output(command, shell=True)
     projects = json.loads(pr)
+    for friendly_project in projects_from_friendly:
+        try:
+            existing = next(item for item in projects if item["projectId"] == friendly_project["projectId"])
+        except:
+            existing = None
+        if existing:
+            existing["friendly_name"] = friendly_project["friendly_name"]
+        else:
+            projects.append(friendly_project)
     projects = sorted(projects, key=lambda x: x["name"])
     return projects
 
 def get_current_project_id():
     try:
         pr = subprocess.check_output('gcloud config get-value project', shell=True)
         return pr.decode("utf-8").strip()
```

### Comparing `gcp_quick_utils-0.2/gcpq/gcp_sections_service.py` & `gcp_quick_utils-0.3/gcpq/gcp_sections_service.py`

 * *Files identical despite different names*

### Comparing `gcp_quick_utils-0.2/gcpq/main.py` & `gcp_quick_utils-0.3/gcpq/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import click
 
 import gcpq.console_utils as console_utils
 import gcpq.gcp_cli_service as gcp_cli_service
 import gcpq.gcp_sections_service as gcp_sections_service
-from gcpq.cfg_service import config
+from gcpq.cfg_service import config, add_friendly_name
 
 
 def switch_command(search, auto):
-    projects = gcp_cli_service.get_projects(search)
+    projects_from_friendly = [x for x in config["projects"] if search.lower() in x["friendly_name"].lower()]
+    projects = gcp_cli_service.get_projects(search, projects_from_friendly)
     if not projects:
         print("No projects found")
         return
     if auto:
         projNum = 0
     else:
         projNum = console_utils.get_choice(projects)
@@ -19,15 +20,16 @@
 
 
 
 def open_service_command(services, search, auto, force):
     if not search and not force:
         projectId = gcp_cli_service.get_current_project_id()
     else:
-        projects = gcp_cli_service.get_projects(search)
+        projects_from_friendly = [x for x in config["projects"] if search.lower() in x["friendly_name"].lower()]
+        projects = gcp_cli_service.get_projects(search, projects_from_friendly)
 
         if not projects:
             print("No projects found")
             return
 
         if auto:
             projNum = 0
@@ -37,24 +39,44 @@
         projectId = projects[int(projNum)]["projectId"]
 
     for service in services:
         gcp_sections_service.open_service(service, projectId)
     return
 
 
+def add_friendly_name_command(search):
+    projects = gcp_cli_service.get_projects(search)
+
+    if not projects:
+        print("No projects found")
+        return
+    projNum = console_utils.get_choice(projects)
+    project = projects[int(projNum)]
+
+    friendly_name = input("Enter friendly name for project: ")
+    project["friendly_name"] = friendly_name
+
+    add_friendly_name(project)
+
+    return
+
 
 @click.command()
 @click.argument("command", default="", required=False)
 @click.argument("search", default="", required=False)
 @click.option('--auto/--choose', '-a', default=False, help="Will select the first found project")
 @click.option('--force/--noforce', '-f', default=False, help="Will force the project search even with an empty search string")
 def main(command, search, auto, force):
     
     gcp_cli_service.check_if_gcloud_is_installed()
     try:
+        if command == "a":
+            add_friendly_name_command(search)
+            return
+
         if command == "s":
             switch_command(search, auto)
             return
 
         services = gcp_sections_service.find_matching_services(command.split(","))
         if services:
             open_service_command(services, search, auto, force)
```

### Comparing `gcp_quick_utils-0.2/pyproject.toml` & `gcp_quick_utils-0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gcp-quick-utils"
-version = "0.2"
+version = "0.3"
 description = "Tools to help you navigate through GCP"
 authors = ["Guillaume W <guillaume.luc.wagner@gmail.com>"]
 readme = "README.md"
 packages = [{include = "gcpq"}]
 license = "MIT"
 homepage = "https://github.com/faahren/gcp-quick-utils.git"
```

### Comparing `gcp_quick_utils-0.2/PKG-INFO` & `gcp_quick_utils-0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcp-quick-utils
-Version: 0.2
+Version: 0.3
 Summary: Tools to help you navigate through GCP
 Home-page: https://github.com/faahren/gcp-quick-utils.git
 License: MIT
 Author: Guillaume W
 Author-email: guillaume.luc.wagner@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
@@ -32,78 +32,83 @@
 GCLOUD SDK has to be installed on your machine and you have to be logged in
 
 ## Usage
 
 ### Switch between projects
 If you want to list all projects before choosing one
 ```
-pgo s
+gcpq s
 ```
 
 If you want to search for a specific term in the project name or project id
 
 ```
-pgo s searchTerm
+gcpq s searchTerm
 ```
 
 You will see the following output to choose your project rom:
 
 ```
-$ pgo mycompanyName
+$ gcpq mycompanyName
 [0] : mycompany-380102 (mycompany)
 [1] : mycompany-airbyte (mycompany-airbyte)
 [2] : mycompany-chatbot (mycompany-chatbot)
 [3] : mycompany-etl (mycompany-etl)
 [4] : mycompany-ga4-lehoublon-flo (mycompany-ga4-lehoublon-flo)
 [5] : mycompany-guillaume-pde (mycompany-guillaume-pde)
 [6] : mycompany-n8n (mycompany-n8n)
 [7] : mycompany-terraform (mycompany-terraform)
 Enter project number to switch to: 
 ```
 
 If you want to automatically switch to the first found project
 ```
-pgo searchTerm -a
+gcpq searchTerm -a
 ```
 
 ### Opening Google Cloud Interface quickly
 
 If you want to open a service quickly. When you don't specify projects, the current Gcloud set project will be used
 
 ```
-pgo bq
+gcpq bq
 ```
 
 Open multiple services at the same time
 
 ```
-pgo bq,dataform,iam,build,gcs
+gcpq bq,dataform,iam,build,gcs
 ```
 
 Aliased have been created for the services. You can see them in the `services.yaml` file of the repo
 
 
 Open services on a specific project (you will be able to choose the project matching the search result)
 
 ```
-pgo bq myCompanyName
+gcpq bq myCompanyName
 ```
 
 Open services on a specific project automatically (Will open the first found project)
 
 ```
-pgo bq myCompanyName -a 
+gcpq bq myCompanyName -a 
 ```
 
 Create shortcuts of groups of services
 - Open your config file located in `~/.gcpq/config.yaml`
 - Add new groups of services in the file (follow current structure)
 
 
 ```
-pgo myGroupName 
+gcpq myGroupName 
 ```
 
 
 
-# Modifying GCPQU
-If you need to modify the package, you can test your modifications with poetry run pgo
+# Modifying GCPQ
+
+If you need to modify the package, you can test your modifications with poetry run gcpq
+
+```
+poetry run gcpq bq
+```
```

