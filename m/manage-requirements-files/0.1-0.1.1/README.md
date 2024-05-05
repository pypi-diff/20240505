# Comparing `tmp/manage_requirements_files-0.1.tar.gz` & `tmp/manage_requirements_files-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manage_requirements_files-0.1.tar", last modified: Mon Apr  8 19:23:12 2024, max compression
+gzip compressed data, was "manage_requirements_files-0.1.1.tar", last modified: Sun May  5 13:42:54 2024, max compression
```

## Comparing `manage_requirements_files-0.1.tar` & `manage_requirements_files-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 guilherme.gouw   (503) staff       (20)        0 2024-04-08 19:23:12.355922 manage_requirements_files-0.1/
--rw-r--r--   0 guilherme.gouw   (503) staff       (20)     1070 2024-04-02 16:14:59.000000 manage_requirements_files-0.1/LICENSE
--rw-r--r--   0 guilherme.gouw   (503) staff       (20)     3233 2024-04-08 19:23:12.355222 manage_requirements_files-0.1/PKG-INFO
--rw-r--r--   0 guilherme.gouw   (503) staff       (20)     2707 2024-04-08 19:09:36.000000 manage_requirements_files-0.1/README.md
-drwxr-xr-x   0 guilherme.gouw   (503) staff       (20)        0 2024-04-08 19:23:12.349918 manage_requirements_files-0.1/manage_requirements_files/
--rw-r--r--   0 guilherme.gouw   (503) staff       (20)        0 2024-04-08 17:48:39.000000 manage_requirements_files-0.1/manage_requirements_files/__init__.py
--rw-r--r--   0 guilherme.gouw   (503) staff       (20)     2110 2024-04-08 18:08:46.000000 manage_requirements_files-0.1/manage_requirements_files/cli.py
-drwxr-xr-x   0 guilherme.gouw   (503) staff       (20)        0 2024-04-08 19:23:12.354584 manage_requirements_files-0.1/manage_requirements_files.egg-info/
--rw-r--r--   0 guilherme.gouw   (503) staff       (20)     3233 2024-04-08 19:23:12.000000 manage_requirements_files-0.1/manage_requirements_files.egg-info/PKG-INFO
--rw-r--r--   0 guilherme.gouw   (503) staff       (20)      345 2024-04-08 19:23:12.000000 manage_requirements_files-0.1/manage_requirements_files.egg-info/SOURCES.txt
--rw-r--r--   0 guilherme.gouw   (503) staff       (20)        1 2024-04-08 19:23:12.000000 manage_requirements_files-0.1/manage_requirements_files.egg-info/dependency_links.txt
--rw-r--r--   0 guilherme.gouw   (503) staff       (20)       75 2024-04-08 19:23:12.000000 manage_requirements_files-0.1/manage_requirements_files.egg-info/entry_points.txt
--rw-r--r--   0 guilherme.gouw   (503) staff       (20)       26 2024-04-08 19:23:12.000000 manage_requirements_files-0.1/manage_requirements_files.egg-info/top_level.txt
--rw-r--r--   0 guilherme.gouw   (503) staff       (20)       38 2024-04-08 19:23:12.356060 manage_requirements_files-0.1/setup.cfg
--rw-r--r--   0 guilherme.gouw   (503) staff       (20)      827 2024-04-08 18:18:00.000000 manage_requirements_files-0.1/setup.py
+drwxrwxr-x   0 guilhermegouw  (1000) guilhermegouw  (1000)        0 2024-05-05 13:42:54.183116 manage_requirements_files-0.1.1/
+-rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)     1070 2024-05-05 10:03:57.000000 manage_requirements_files-0.1.1/LICENSE
+-rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)     3270 2024-05-05 13:42:54.183116 manage_requirements_files-0.1.1/PKG-INFO
+-rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)     2722 2024-05-05 13:35:43.000000 manage_requirements_files-0.1.1/README.md
+drwxrwxr-x   0 guilhermegouw  (1000) guilhermegouw  (1000)        0 2024-05-05 13:42:54.183116 manage_requirements_files-0.1.1/manage_requirements_files/
+-rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)        0 2024-05-05 10:03:57.000000 manage_requirements_files-0.1.1/manage_requirements_files/__init__.py
+-rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)     2033 2024-05-05 13:10:13.000000 manage_requirements_files-0.1.1/manage_requirements_files/cli.py
+drwxrwxr-x   0 guilhermegouw  (1000) guilhermegouw  (1000)        0 2024-05-05 13:42:54.183116 manage_requirements_files-0.1.1/manage_requirements_files.egg-info/
+-rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)     3270 2024-05-05 13:42:54.000000 manage_requirements_files-0.1.1/manage_requirements_files.egg-info/PKG-INFO
+-rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)      381 2024-05-05 13:42:54.000000 manage_requirements_files-0.1.1/manage_requirements_files.egg-info/SOURCES.txt
+-rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)        1 2024-05-05 13:42:54.000000 manage_requirements_files-0.1.1/manage_requirements_files.egg-info/dependency_links.txt
+-rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)       76 2024-05-05 13:42:54.000000 manage_requirements_files-0.1.1/manage_requirements_files.egg-info/entry_points.txt
+-rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)       32 2024-05-05 13:42:54.000000 manage_requirements_files-0.1.1/manage_requirements_files.egg-info/top_level.txt
+-rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)       38 2024-05-05 13:42:54.183116 manage_requirements_files-0.1.1/setup.cfg
+-rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)      829 2024-05-05 13:34:38.000000 manage_requirements_files-0.1.1/setup.py
+drwxrwxr-x   0 guilhermegouw  (1000) guilhermegouw  (1000)        0 2024-05-05 13:42:54.183116 manage_requirements_files-0.1.1/tests/
+-rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)        0 2024-05-05 10:51:15.000000 manage_requirements_files-0.1.1/tests/__init__.py
+-rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)     7338 2024-05-05 13:24:19.000000 manage_requirements_files-0.1.1/tests/test_cli.py
```

### Comparing `manage_requirements_files-0.1/LICENSE` & `manage_requirements_files-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `manage_requirements_files-0.1/PKG-INFO` & `manage_requirements_files-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: manage_requirements_files
-Version: 0.1
+Version: 0.1.1
 Summary: A utility to manage project dependencies for development and production.
 Home-page: https://github.com/guilhermegouw/manage-requirements-files
 Author: Guilherme Gouw
 Author-email: guilherme.gouw@gmail.com
 License: MIT
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Manage Requirements Files
+# Manage Requirements Files Version: 0.1.1
 
 `manage-requirements-files` is a Python CLI tool designed to help developers efficiently manage their project dependencies. It automates the updating of `requirements.txt` and `requirements-dev.txt` by appending new dependencies from the activated Python environment.
 
 ## Features
 
 - Detects newly installed packages not listed in `requirements.txt` or `requirements-dev.txt`.
 - Appends new dependencies to the appropriate requirements file without duplicating entries.
@@ -84,7 +85,9 @@
 ## License
 
 Distributed under the MIT License. See LICENSE for more information.
 
 ## Contact
 
 Guilherme Gouw - guilherme.gouw@gmail.com
+
+
```

### Comparing `manage_requirements_files-0.1/README.md` & `manage_requirements_files-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Manage Requirements Files
+# Manage Requirements Files Version: 0.1.1
 
 `manage-requirements-files` is a Python CLI tool designed to help developers efficiently manage their project dependencies. It automates the updating of `requirements.txt` and `requirements-dev.txt` by appending new dependencies from the activated Python environment.
 
 ## Features
 
 - Detects newly installed packages not listed in `requirements.txt` or `requirements-dev.txt`.
 - Appends new dependencies to the appropriate requirements file without duplicating entries.
```

### Comparing `manage_requirements_files-0.1/manage_requirements_files/cli.py` & `manage_requirements_files-0.1.1/manage_requirements_files/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import argparse
 import subprocess
 import sys
 
 
 def main():
-    parser = argparse.ArgumentParser(description="Manage Python project dependencies.")
+    parser = argparse.ArgumentParser(
+        description="Manage Python project dependencies."
+    )
     parser.add_argument(
         "mode",
         choices=["prod", "dev"],
         help="Update production or development dependencies.",
     )
 
     args = parser.parse_args()
@@ -17,19 +19,24 @@
         update_requirements("requirements.txt", "requirements-dev.txt")
     else:  # dev
         update_requirements("requirements-dev.txt", "requirements.txt")
 
 
 def pip_freeze():
     """Get the output of pip freeze as a set of package=version strings."""
-    return set(subprocess.check_output(["pip", "freeze"], text=True).splitlines())
+    return set(
+        subprocess.check_output(
+            [sys.executable, "-m", "pip", "freeze"], text=True
+        ).splitlines()
+    )
 
 
 def read_requirements(filename):
-    """Read a requirements file and return its contents as a set, create if not exist."""
+    """Read a requirements file and return its contents as a set,\
+        automatically create if not exist."""
     try:
         with open(filename, "r") as file:
             return set(line.strip() for line in file if line.strip())
     except FileNotFoundError:
         open(filename, "a").close()  # Create the file if it does not exist
         return set()
 
@@ -38,27 +45,27 @@
     """Append new lines to a requirements file."""
     with open(filename, "a") as file:
         for line in new_lines:
             file.write(f"{line}\n")
 
 
 def update_requirements(target_file, other_file):
-    """Update the target requirements file with new dependencies, automatically creating files if they don't exist."""
-    # Step 1: Get current environment packages
+    """Update the target requirements file with new dependencies,\
+        automatically creating files if they don't exist."""
     current_packages = pip_freeze()
+    existing_deps = read_requirements(target_file) | read_requirements(
+        other_file
+    )
 
-    # Step 2: Read existing requirements from both files
-    existing_deps = read_requirements(target_file) | read_requirements(other_file)
-
-    # Step 3: Identify new dependencies
     new_dependencies = current_packages - existing_deps
 
-    # Step 4: Update the target requirements file with new dependencies
     if new_dependencies:
         write_requirements(target_file, new_dependencies)
-        print(f"Updated {target_file} with new dependencies: {new_dependencies}")
+        print(
+            f"Updated {target_file} with new dependencies: {new_dependencies}"
+        )
     else:
         print(f"No new dependencies to add to {target_file}.")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `manage_requirements_files-0.1/manage_requirements_files.egg-info/PKG-INFO` & `manage_requirements_files-0.1.1/manage_requirements_files.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
-Name: manage_requirements_files
-Version: 0.1
+Name: manage-requirements-files
+Version: 0.1.1
 Summary: A utility to manage project dependencies for development and production.
 Home-page: https://github.com/guilhermegouw/manage-requirements-files
 Author: Guilherme Gouw
 Author-email: guilherme.gouw@gmail.com
 License: MIT
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Manage Requirements Files
+# Manage Requirements Files Version: 0.1.1
 
 `manage-requirements-files` is a Python CLI tool designed to help developers efficiently manage their project dependencies. It automates the updating of `requirements.txt` and `requirements-dev.txt` by appending new dependencies from the activated Python environment.
 
 ## Features
 
 - Detects newly installed packages not listed in `requirements.txt` or `requirements-dev.txt`.
 - Appends new dependencies to the appropriate requirements file without duplicating entries.
@@ -84,7 +85,9 @@
 ## License
 
 Distributed under the MIT License. See LICENSE for more information.
 
 ## Contact
 
 Guilherme Gouw - guilherme.gouw@gmail.com
+
+
```

### Comparing `manage_requirements_files-0.1/setup.py` & `manage_requirements_files-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="manage_requirements_files",
-    version="0.1",
+    version="0.1.1",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "manage-dependencies=manage_requirements_files.cli:main",
         ],
     },
     author="Guilherme Gouw",
```

