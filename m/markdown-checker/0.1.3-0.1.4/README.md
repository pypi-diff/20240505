# Comparing `tmp/markdown-checker-0.1.3.tar.gz` & `tmp/markdown_checker-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown-checker-0.1.3.tar", last modified: Thu Mar 14 23:27:36 2024, max compression
+gzip compressed data, was "markdown_checker-0.1.4.tar", last modified: Sun May  5 21:49:51 2024, max compression
```

## Comparing `markdown-checker-0.1.3.tar` & `markdown_checker-0.1.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 23:27:36.691621 markdown-checker-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-14 23:27:23.000000 markdown-checker-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-14 23:27:23.000000 markdown-checker-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-03-14 23:27:36.691621 markdown-checker-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-03-14 23:27:23.000000 markdown-checker-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 23:27:36.691621 markdown-checker-0.1.3/markdown_checker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 23:27:23.000000 markdown-checker-0.1.3/markdown_checker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-03-14 23:27:23.000000 markdown-checker-0.1.3/markdown_checker/check_markdown.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 23:27:36.691621 markdown-checker-0.1.3/markdown_checker/generators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 23:27:23.000000 markdown-checker-0.1.3/markdown_checker/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-03-14 23:27:23.000000 markdown-checker-0.1.3/markdown_checker/generators/md_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 23:27:36.691621 markdown-checker-0.1.3/markdown_checker/inputs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 23:27:23.000000 markdown-checker-0.1.3/markdown_checker/inputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-03-14 23:27:23.000000 markdown-checker-0.1.3/markdown_checker/inputs/input_arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 23:27:36.691621 markdown-checker-0.1.3/markdown_checker/links/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 23:27:23.000000 markdown-checker-0.1.3/markdown_checker/links/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-03-14 23:27:23.000000 markdown-checker-0.1.3/markdown_checker/links/link_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 23:27:36.691621 markdown-checker-0.1.3/markdown_checker/paths/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 23:27:23.000000 markdown-checker-0.1.3/markdown_checker/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-03-14 23:27:23.000000 markdown-checker-0.1.3/markdown_checker/paths/files_paths_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-03-14 23:27:23.000000 markdown-checker-0.1.3/markdown_checker/validate_markdown.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 23:27:36.691621 markdown-checker-0.1.3/markdown_checker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-03-14 23:27:36.000000 markdown-checker-0.1.3/markdown_checker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-03-14 23:27:36.000000 markdown-checker-0.1.3/markdown_checker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 23:27:36.000000 markdown-checker-0.1.3/markdown_checker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-14 23:27:36.000000 markdown-checker-0.1.3/markdown_checker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-14 23:27:36.000000 markdown-checker-0.1.3/markdown_checker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-14 23:27:36.000000 markdown-checker-0.1.3/markdown_checker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-14 23:27:23.000000 markdown-checker-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-03-14 23:27:36.691621 markdown-checker-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 23:27:23.000000 markdown-checker-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 23:27:36.691621 markdown-checker-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-03-14 23:27:23.000000 markdown-checker-0.1.3/tests/test_markdown_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:49:51.675028 markdown_checker-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-05 21:49:42.000000 markdown_checker-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-05-05 21:49:51.675028 markdown_checker-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-05 21:49:42.000000 markdown_checker-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-05 21:49:42.000000 markdown_checker-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 21:49:51.675028 markdown_checker-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:49:51.667028 markdown_checker-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:49:51.671028 markdown_checker-0.1.4/src/markdown_checker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 21:49:42.000000 markdown_checker-0.1.4/src/markdown_checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-05-05 21:49:42.000000 markdown_checker-0.1.4/src/markdown_checker/check_markdown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:49:51.671028 markdown_checker-0.1.4/src/markdown_checker/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 21:49:42.000000 markdown_checker-0.1.4/src/markdown_checker/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-05-05 21:49:42.000000 markdown_checker-0.1.4/src/markdown_checker/generators/md_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:49:51.671028 markdown_checker-0.1.4/src/markdown_checker/inputs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 21:49:42.000000 markdown_checker-0.1.4/src/markdown_checker/inputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-05 21:49:42.000000 markdown_checker-0.1.4/src/markdown_checker/inputs/input_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:49:51.675028 markdown_checker-0.1.4/src/markdown_checker/links/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 21:49:42.000000 markdown_checker-0.1.4/src/markdown_checker/links/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-05-05 21:49:42.000000 markdown_checker-0.1.4/src/markdown_checker/links/link_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:49:51.675028 markdown_checker-0.1.4/src/markdown_checker/paths/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 21:49:42.000000 markdown_checker-0.1.4/src/markdown_checker/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-05 21:49:42.000000 markdown_checker-0.1.4/src/markdown_checker/paths/files_paths_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 21:49:42.000000 markdown_checker-0.1.4/src/markdown_checker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-05 21:49:42.000000 markdown_checker-0.1.4/src/markdown_checker/validate_markdown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:49:51.675028 markdown_checker-0.1.4/src/markdown_checker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-05-05 21:49:51.000000 markdown_checker-0.1.4/src/markdown_checker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-05 21:49:51.000000 markdown_checker-0.1.4/src/markdown_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 21:49:51.000000 markdown_checker-0.1.4/src/markdown_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-05 21:49:51.000000 markdown_checker-0.1.4/src/markdown_checker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-05 21:49:51.000000 markdown_checker-0.1.4/src/markdown_checker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-05 21:49:51.000000 markdown_checker-0.1.4/src/markdown_checker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:49:51.675028 markdown_checker-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-05 21:49:42.000000 markdown_checker-0.1.4/tests/test_markdown_checker.py
```

### Comparing `markdown-checker-0.1.3/LICENSE` & `markdown_checker-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown-checker-0.1.3/PKG-INFO` & `markdown_checker-0.1.4/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,88 +1,93 @@
-Metadata-Version: 2.1
-Name: markdown-checker
-Version: 0.1.3
-Summary: A markdown validation reporting tool
-Home-page: https://github.com/john0isaac/markdown-checker
-Author: John Aziz
-Author-email: johnaziz269@gmail.com
-Maintainer: John Aziz
-Maintainer-email: johnaziz269@gmail.com
-License: MIT
-Project-URL: Bug Tracker, https://github.com/john0isaac/markdown-checker/issues
-Project-URL: Contributing, https://github.com/john0isaac/markdown-checker/pulls
-Project-URL: Source Code, https://github.com/john0isaac/markdown-checker
-Project-URL: Releases, https://github.com/john0isaac/markdown-checker/releases
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-
 [![PyPi](https://img.shields.io/pypi/v/markdown-checker)](https://pypi.org/project/markdown-checker/)
+[![Documentation Status](https://readthedocs.org/projects/markdown-checker/badge/?version=latest)](https://markdown-checker.readthedocs.io/en/latest/?badge=latest)
 [![Downloads](https://img.shields.io/pypi/dm/markdown-checker)](https://pypi.org/project/markdown-checker/)
 
 [![GitHub issues](https://img.shields.io/badge/issue_tracking-github-blue.svg)](https://github.com/john0isaac/markdown-checker/issues)
 [![Contributing](https://img.shields.io/badge/PR-Welcome-%23FF8300.svg?)](https://github.com/john0isaac/markdown-checker/pulls)
 
-markdown-checker is a markdown validation reporting tool.
+markdown-checker is a markdown link validation reporting tool. It provides a couple of functions to validate relative paths and web URLs.
+
+## Installation
+
+Install the package:
+
+```bash
+pip install markdown-checker
+```
+
+### Documentation
+
+- [Full documentation](https://markdown-checker.readthedocs.io/en/latest/).
 
-# How To
+## 1, 2, 3 - How To
 
 1. Run `pip install markdown-checker`.
-2. Run `markdown-checker -d {src} -f {func} -gu {url}`. Replace `{src}` with the directory you want to analyze, {func} with the available functions like check_broken_paths, {gu} with your contribution guidance full URL.
+2. Run `markdown-checker -d {src} -f {func} -gu {url}`. Replace `{src}` with the directory you want to analyze, `{func}` with the available functions like `check_broken_paths`, `{gu}` with your contribution guidance full URL.
 3. The output will be displayed in the terminal and in a `comments.md` file.
 
-# Using markdown-checker in GitHub Actions
+## Using `markdown-checker` in GitHub Actions
 
-The tool has been designed to be run within a GitHub workflow using the [action-check-markdown](https://github.com/marketplace/actions/check-markdown) GitHub action. The action will automatically post the output of the tool to your GitHub pull request as a comment.
+You can run this tool within a GitHub workflow using the [action-check-markdown](https://github.com/marketplace/actions/check-markdown) GitHub action.
 
-# Supported Functions
+The action will automatically post the output of the tool to your GitHub pull request as a comment.
 
-## Check broken relative paths
-This function ensures that any relative path in your files is working.
+# Usage
+
+The library provides the following functions:
+
+- [Usage](#usage)
+  - [`check_broken_paths`](#check_broken_paths)
+  - [`check_broken_urls`](#check_broken_urls)
+  - [`check_urls_locale`](#check_urls_locale)
+  - [`check_paths_tracking`](#check_paths_tracking)
+  - [`check_urls_tracking`](#check_urls_tracking)
+
+## `check_broken_paths`
+
+This function ensures that any relative path in your files are working.
 
 Example:
 
 ```bash
 markdown-checker -d . -f check_broken_paths -gu https://github.com/john0isaac/markdown-checker/blob/main/CONTRIBUTING.md
 ```
 
-## Check broken URLs
+## `check_broken_urls`
+
 This function ensures that any web URL in your files is working and returning 200 status code.
 
 Example:
 
 ```bash
 markdown-checker -d . -f check_broken_urls -gu https://github.com/john0isaac/markdown-checker/blob/main/CONTRIBUTING.md
 ```
 
-## Check country locale present in URLs
-This function ensures that any relative path in your files is working. 
+## `check_urls_locale`
+
+This function checks if country specific locale is present in URLs.
 
 Example:
 
 ```bash
 markdown-checker -d . -f check_urls_locale -gu https://github.com/john0isaac/markdown-checker/blob/main/CONTRIBUTING.md
 ```
 
-## Check Contributor ID missing from paths
+## `check_paths_tracking`
+
 This function ensures that any relative path has tracking in it.
 
 Example:
 
 ```bash
 markdown-checker -d . -f check_paths_tracking -gu https://github.com/john0isaac/markdown-checker/blob/main/CONTRIBUTING.md
 ```
 
-## Check Contributor ID missing from URLs
+## `check_urls_tracking`
+
 This function ensures that any URL has tracking in it.
 
 Example:
 
 ```bash
 markdown-checker -d . -f check_urls_tracking -gu https://github.com/john0isaac/markdown-checker/blob/main/CONTRIBUTING.md
 ```
```

### Comparing `markdown-checker-0.1.3/markdown_checker/check_markdown.py` & `markdown_checker-0.1.4/src/markdown_checker/check_markdown.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """
 Module providing automatic checks functionality to markdown files
 following some Guidelines
 """
 
+from typing import List
+
 from markdown_checker.links.link_operations import (
     check_paths_exists,
     check_url_alive,
     check_url_locale,
     check_url_tracking,
     get_links_from_file,
     get_paths_from_links,
@@ -53,22 +55,23 @@
                     formatted_output += format_links(country_locale_urls)
                     return formatted_output
             elif check_type == "broken" and len(urls) > 0:
                 dead_urls = check_url_alive(urls)
                 if len(dead_urls) > 0:
                     formatted_output += format_links(dead_urls)
                     return formatted_output
+    return ""
 
 
-def format_links(links: list) -> str:
+def format_links(links: List[str]) -> str:
     """
-    Formats a list of links into a string with numbered bullets.
+    Formats a List of links into a string with numbered bullets.
 
     Args:
-        links (list): A list of links.
+        links (List): A List of links.
 
     Returns:
         str: The formatted string with numbered bullets.
     """
     formatted_links = ""
     i = 1
     for link in links:
```

### Comparing `markdown-checker-0.1.3/markdown_checker/generators/md_generator.py` & `markdown_checker-0.1.4/src/markdown_checker/generators/md_generator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,72 +1,64 @@
 CHECK_BROKEN_PATHS = """# Check Broken Paths
 
-We have automatically detected the following broken relative paths in your files. Review and fix the paths to resolve this issue.
+We have automatically detected the following broken relative paths in your files.
+Review and fix the paths to resolve this issue.
 
 Check the file paths and associated broken paths inside them."""
 CHECK_BROKEN_URLS = """# Check Broken URLs
 
 We have automatically detected the following broken URLs in your files. Review and fix the paths to resolve this issue.
 
 Check the file paths and associated broken URLs inside them."""
 CHECK_PATHS_TRACKING = """# Check Missing Tracking from Paths
 
-We have automatically detected missing tracking IDs from the following relative paths in your files. Review and add tracking to paths to resolve this issue.
+We have automatically detected missing tracking IDs from the following relative paths in your files.
+Review and add tracking to paths to resolve this issue.
 
 Check the file paths and associated paths inside them."""
 CHECK_URLS_TRACKING = """# Check Missing Tracking from URLs
 
-We have automatically detected missing tracking IDs from the following URLs in your files. Review and add tracking to URLs to resolve this issue.
+We have automatically detected missing tracking IDs from the following URLs in your files.
+Review and add tracking to URLs to resolve this issue.
 
 Check the file paths and associated URLs inside them."""
 CHECK_URLS_LOCALE = """# Check Country Locale in URLs
 
-We have automatically detected added country locale to URLs in your files. Review and remove country-specific locale from URLs to resolve this issue.
+We have automatically detected added country locale to URLs in your files.
+Review and remove country-specific locale from URLs to resolve this issue.
 
 Check the file paths and associated URLs inside them."""
 
 
 def write_md_file(generated_md: str) -> None:
     """Write the formatted output to a markdown file"""
     with open("comment.md", "w", encoding="utf-8") as file:
         file.write(generated_md)
 
 
-def generate_md(
-    formatted_output: str, function_name: str, contributing_guide_url: str
-) -> None:
+def generate_md(formatted_output: str, function_name: str, contributing_guide_url: str) -> None:
     """Generate markdown file based on the formatted output, function name, and contributing guide URL.
 
     Args:
         formatted_output (str): The formatted output to be written to the markdown file.
         function_name (str): The name of the function to determine the header for the markdown file.
         contributing_guide_url (str): The URL of the contributing guide to be included in the markdown file.
 
     Raises:
         ValueError: If an invalid function name is provided.
 
     """
     contributing_guide_line = f" For more details, check our [Contributing Guide]({contributing_guide_url}).\n\n"
     if function_name == "check_broken_paths":
-        formatted_output = (
-            CHECK_BROKEN_PATHS + contributing_guide_line + formatted_output
-        )
+        formatted_output = CHECK_BROKEN_PATHS + contributing_guide_line + formatted_output
     elif function_name == "check_broken_urls":
-        formatted_output = (
-            CHECK_BROKEN_URLS + contributing_guide_line + formatted_output
-        )
+        formatted_output = CHECK_BROKEN_URLS + contributing_guide_line + formatted_output
     elif function_name == "check_paths_tracking":
-        formatted_output = (
-            CHECK_PATHS_TRACKING + contributing_guide_line + formatted_output
-        )
+        formatted_output = CHECK_PATHS_TRACKING + contributing_guide_line + formatted_output
     elif function_name == "check_urls_tracking":
-        formatted_output = (
-            CHECK_URLS_TRACKING + contributing_guide_line + formatted_output
-        )
+        formatted_output = CHECK_URLS_TRACKING + contributing_guide_line + formatted_output
     elif function_name == "check_urls_locale":
-        formatted_output = (
-            CHECK_URLS_LOCALE + contributing_guide_line + formatted_output
-        )
+        formatted_output = CHECK_URLS_LOCALE + contributing_guide_line + formatted_output
     else:
         raise ValueError("Invalid function name")
 
     write_md_file(formatted_output)
```

### Comparing `markdown-checker-0.1.3/markdown_checker/inputs/input_arguments.py` & `markdown_checker-0.1.4/src/markdown_checker/inputs/input_arguments.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Module providing automatic checks functionality to markdown files
 following some Guidelines
 """
 
 import argparse
 
 
-def get_input_args() -> None:
+def get_input_args() -> argparse.Namespace:
     """
     Retrieves and parses the 2 command line arguments provided by the user when
     they run the program from a terminal window. This function uses Python's
     argparse module to created and defined these 2 command line arguments. If
     the user fails to provide some or all of the 2 arguments, then the default
     values are used for the missing arguments.
     Command Line Arguments:
```

### Comparing `markdown-checker-0.1.3/markdown_checker/links/link_operations.py` & `markdown_checker-0.1.4/src/markdown_checker/links/link_operations.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import os
 import re
+from typing import List
 
 
-def get_links_from_file(file_path: str) -> list:
+def get_links_from_file(file_path: str) -> List[str]:
     """function to get an array of markdown links from a file
     flags markdown links captures the part inside () that comes right after []
     """
     all_links = []
-    with open(file_path, "r", encoding="utf-8") as file:
+    with open(file_path, encoding="utf-8") as file:
         data = file.read()
         link_pattern = re.compile(r"\]\((.*?)\)| \)")
         matches = re.finditer(link_pattern, data)
         for matched_group in matches:
             if matched_group.group(1):
                 all_links.append(matched_group.group(1))
     return all_links
 
 
-def get_urls_from_links(all_links: list) -> list:
-    """function to get an array of urls from a list"""
+def get_urls_from_links(all_links: List[str]) -> List[str]:
+    """function to get an array of urls from a List"""
     urls = []
     url_pattern = re.compile(
         r"https?:\/\/(www\.)?[-a-zA-Z0-9@:%._\+~#=]{1,256}\.[a-zA-Z0-9]{1,6}\b([-a-zA-Z0-9@:%_\+.~#?&\/\/=]*)"
     )
     allowed_list = [
         "github.com",
         "microsoft.com",
@@ -34,76 +35,71 @@
         matches = re.findall(url_pattern, link)
 
         if matches and any(allowed in link.lower() for allowed in allowed_list):
             urls.append(link)
     return urls
 
 
-def get_paths_from_links(all_links: list) -> list:
-    """function to get relative paths from a list
+def get_paths_from_links(all_links: List[str]) -> List[str]:
+    """function to get relative paths from a List
     flags paths that start with ./ or ../
     """
     paths = []
     path_pattern = re.compile(r"(\.{1,2}\/)+([A-Za-z0-9-]+\/)*(.+\.[A-Za-z]+)")
 
     for link in all_links:
         link = link.split(" ")[0]
         matches = re.findall(path_pattern, link)
         if matches:
             paths.append(link.split("#")[0])
     return paths
 
 
-def check_paths_exists(file_path: str, paths: list) -> list:
+def check_paths_exists(file_path: str, paths: List[str]) -> List[str]:
     """function checks if a path exist if not return non existent paths
     flags any relative path that can't be accessed
     """
     broken_path = []
     for path in paths:
         path = re.sub(r"(\?|\&)(WT|wt)\.mc_id=.*", "", path)
-        if not os.path.exists(
-            os.path.normpath(os.path.join(os.path.dirname(file_path), path))
-        ):
+        if not os.path.exists(os.path.normpath(os.path.join(os.path.dirname(file_path), path))):
             broken_path.append(path)
     return broken_path
 
 
-def check_url_locale(urls: list) -> list:
+def check_url_locale(urls: List[str]) -> List[str]:
     """function checks if a url has country locale
     flags urls that have ==> /en-us/
     """
     country_locale = []
     for url in urls:
-        if (
-            "video-embed.html" in url
-            or "https://www.microsoft.com/en-us/security/blog" in url
-        ):
+        if "video-embed.html" in url or "https://www.microsoft.com/en-us/security/blog" in url:
             continue
         locale_pattern = re.compile(r"\/[a-z]{2}-[a-z]{2}\/")
         matches = re.findall(locale_pattern, url)
         if matches:
             country_locale.append(url)
     return country_locale
 
 
-def check_url_tracking(urls: list) -> list:
+def check_url_tracking(urls: List[str]) -> List[str]:
     """function checks if a url has tracking id
     flags urls missing ==> (? or &) plus WT.mc_id= or wt.mc_id=
     """
     tracking_id = []
     for url in urls:
         tracking_pattern = re.compile(r"(\?|\&)(WT|wt)\.mc_id=")
         matches = re.findall(tracking_pattern, url)
         if not matches:
             tracking_id.append(url)
     return tracking_id
 
 
-def check_url_alive(urls: list) -> list:
-    import requests
+def check_url_alive(urls: List[str]) -> List[str]:
+    import requests  # type: ignore
 
     broken_urls = []
     for url in urls:
         if "https://vscode.dev/redirect?url=" in url:
             continue
         try:
             response = requests.get(url, timeout=10)
@@ -112,33 +108,31 @@
         except requests.exceptions.RequestException:
             broken_urls.append(url)
             continue
     return broken_urls
 
 
 # DEPRECATED
-def get_urls_from_file(file_path: str) -> list:
+def get_urls_from_file(file_path: str) -> List[str]:
     """function to get an array of urls from a file"""
     urls = []
-    with open(file_path, "r", encoding="utf-8") as file:
+    with open(file_path, encoding="utf-8") as file:
         data = file.read()
         url_pattern = re.compile(
             r"https?:\/\/(www\.)?[-a-zA-Z0-9@:%._\+~#=]{1,256}\.[a-zA-Z0-9]{1,6}\b([-a-zA-Z0-9@:%_\+.~#?&\/\/=]*)"
         )
         matches = re.finditer(url_pattern, data)
         for matched_group in matches:
             urls.append(matched_group.group())
     return urls
 
 
-def get_paths_from_file(file_path: str) -> list:
+def get_paths_from_file(file_path: str) -> List[str]:
     """function to get relative paths from a file"""
     paths = []
-    with open(file_path, "r", encoding="utf-8") as file:
+    with open(file_path, encoding="utf-8") as file:
         data = file.read()
-        path_pattern = re.compile(
-            r"(\.{1,2}\/)+([A-Za-z0-9-]+\/)*([A-Za-z0-9]+\.[A-Za-z]+)"
-        )
+        path_pattern = re.compile(r"(\.{1,2}\/)+([A-Za-z0-9-]+\/)*([A-Za-z0-9]+\.[A-Za-z]+)")
         matches = re.finditer(path_pattern, data)
         for matched_group in matches:
             paths.append(matched_group.group())
     return paths
```

### Comparing `markdown-checker-0.1.3/markdown_checker/paths/files_paths_reader.py` & `markdown_checker-0.1.4/src/markdown_checker/paths/files_paths_reader.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 """
 This module contains a function to get a list of file paths from a root directory and
 its subdirectories, filtered by file extension.
 
 The main function in this module is `get_files_paths_list`.
 
 Functions:
-- get_files_paths_list(root_path: str, extension: list = None) -> list
+- get_files_paths_list(root_path: str, extension: list = []) -> list
 """
 
 import os
+from typing import List, Tuple
 
 
-def get_files_paths_list(root_path: str, extensions: list = None) -> list:
+def get_files_paths_list(root_path: str, extensions: List[str] = []) -> Tuple[List[str], List[str]]:
     """
     function returns a list of files in a directory and its subdirectories,
     filtered by file extensions.
 
     Keyword arguments:
     root_path (str): The root directory from which to start the search.
     extensions (list, optional): A list of file extensions to filter by.
     Defaults to [".md", ".ipynb"].
 
     Returns:
     list: A list of file paths that match the given file extensions.
     """
-    if extensions is None:
+    if len(extensions) == 0:
         extensions = [".md", ".ipynb"]
 
-    sub_folders, files_paths = [], []
+    sub_folders: List[str] = []
+    files_paths: List[str] = []
 
     for f in os.scandir(root_path):
         if f.is_dir():
             sub_folders.append(f.path)
         if f.is_file():
             if os.path.splitext(f.name)[1].lower() in extensions:
                 files_paths.append(f.path)
 
     for directory in list(sub_folders):
-        sf, f = get_files_paths_list(directory, extensions)
-        sub_folders.extend(sf)
-        files_paths.extend(f)
+        sub_dir_sub_folders, sub_dir_file_paths = get_files_paths_list(directory, extensions)
+        sub_folders.extend(sub_dir_sub_folders)
+        files_paths.extend(sub_dir_file_paths)
     return sub_folders, files_paths
```

### Comparing `markdown-checker-0.1.3/markdown_checker/validate_markdown.py` & `markdown_checker-0.1.4/src/markdown_checker/validate_markdown.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     in_arg = get_input_args()
 
     _, files_paths = get_files_paths_list(in_arg.dir)
 
     pass_list = [
         "./CODE_OF_CONDUCT.md",
         "./SECURITY.md",
-        ".\CODE_OF_CONDUCT.md",
-        ".\SECURITY.md",
+        ".\\CODE_OF_CONDUCT.md",
+        ".\\SECURITY.md",
     ]
     files_paths = [file_path for file_path in files_paths if file_path not in pass_list]
 
     formatted_output = ""
 
     # iterate over the files to validate the content
     for file_path in files_paths:
@@ -47,16 +47,14 @@
             if urls_locale:
                 formatted_output += urls_locale
         if "check_broken_urls" in in_arg.func:
             broken_urls = check_broken_links(file_path, "url", "broken")
             if broken_urls:
                 formatted_output += broken_urls
     if formatted_output != "":
-        formatted_output = (
-            "| File Full Path | Issues |\n|--------|--------|\n" + formatted_output
-        )
+        formatted_output = "| File Full Path | Issues |\n|--------|--------|\n" + formatted_output
         print(formatted_output)
         generate_md(formatted_output, in_arg.func, in_arg.guide_url)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `markdown-checker-0.1.3/markdown_checker.egg-info/SOURCES.txt` & `markdown_checker-0.1.4/src/markdown_checker.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 LICENSE
-MANIFEST.in
 README.md
 pyproject.toml
-setup.cfg
-setup.py
-markdown_checker/__init__.py
-markdown_checker/check_markdown.py
-markdown_checker/validate_markdown.py
-markdown_checker.egg-info/PKG-INFO
-markdown_checker.egg-info/SOURCES.txt
-markdown_checker.egg-info/dependency_links.txt
-markdown_checker.egg-info/entry_points.txt
-markdown_checker.egg-info/requires.txt
-markdown_checker.egg-info/top_level.txt
-markdown_checker/generators/__init__.py
-markdown_checker/generators/md_generator.py
-markdown_checker/inputs/__init__.py
-markdown_checker/inputs/input_arguments.py
-markdown_checker/links/__init__.py
-markdown_checker/links/link_operations.py
-markdown_checker/paths/__init__.py
-markdown_checker/paths/files_paths_reader.py
+src/markdown_checker/__init__.py
+src/markdown_checker/check_markdown.py
+src/markdown_checker/py.typed
+src/markdown_checker/validate_markdown.py
+src/markdown_checker.egg-info/PKG-INFO
+src/markdown_checker.egg-info/SOURCES.txt
+src/markdown_checker.egg-info/dependency_links.txt
+src/markdown_checker.egg-info/entry_points.txt
+src/markdown_checker.egg-info/requires.txt
+src/markdown_checker.egg-info/top_level.txt
+src/markdown_checker/generators/__init__.py
+src/markdown_checker/generators/md_generator.py
+src/markdown_checker/inputs/__init__.py
+src/markdown_checker/inputs/input_arguments.py
+src/markdown_checker/links/__init__.py
+src/markdown_checker/links/link_operations.py
+src/markdown_checker/paths/__init__.py
+src/markdown_checker/paths/files_paths_reader.py
 tests/test_markdown_checker.py
```

### Comparing `markdown-checker-0.1.3/tests/test_markdown_checker.py` & `markdown_checker-0.1.4/tests/test_markdown_checker.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Module to check paths in markdown files.
 """
 
 import subprocess
 
 
-def check_broken_paths():
+def check_broken_paths() -> None:
     """
     Function to check for broken paths.
     """
     print("check_broken_paths was called")
     subprocess.run(
         [
             "markdown-checker",
@@ -20,15 +20,15 @@
             "-gu",
             "https://github.com/john0isaac/markdown-checker/blob/main/CONTRIBUTING.md",
         ],
         check=False,
     )
 
 
-def check_broken_urls():
+def check_broken_urls() -> None:
     """
     Function to check for broken paths.
     """
     print("check_broken_urls was called")
     subprocess.run(
         [
             "markdown-checker",
@@ -39,15 +39,15 @@
             "-gu",
             "https://github.com/john0isaac/markdown-checker/blob/main/CONTRIBUTING.md",
         ],
         check=False,
     )
 
 
-def check_paths_tracking():
+def check_paths_tracking() -> None:
     """
     Function to check paths tracking.
     """
     print("check_paths_tracking was called")
     subprocess.run(
         [
             "markdown-checker",
@@ -58,15 +58,15 @@
             "-gu",
             "https://github.com/john0isaac/markdown-checker/blob/main/CONTRIBUTING.md",
         ],
         check=False,
     )
 
 
-def check_urls_tracking():
+def check_urls_tracking() -> None:
     """
     Function to check URLs tracking.
     """
     print("check_urls_tracking was called")
     subprocess.run(
         [
             "markdown-checker",
@@ -77,15 +77,15 @@
             "-gu",
             "https://github.com/john0isaac/markdown-checker/blob/main/CONTRIBUTING.md",
         ],
         check=False,
     )
 
 
-def check_urls_locale():
+def check_urls_locale() -> None:
     """
     Function to check URLs locale.
     """
     print("check_urls_locale was called")
     subprocess.run(
         [
             "markdown-checker",
@@ -109,19 +109,27 @@
 }
 
 try:
     choices = list(
         map(
             int,
             input(
-                "Do you want to: \n(1) Run check_broken_paths \n(2) Run check_broken_urls \n(3) Run check_paths_tracking \n(4) Run check_urls_tracking \n(5) Run check_urls_locale \n"
+                """
+                Do you want to:
+                (1) Run check_broken_paths
+                (2) Run check_broken_urls
+                (3) Run check_paths_tracking
+                (4) Run check_urls_tracking
+                (5) Run check_urls_locale
+
+                """
             ).split(),
         )
     )
 except ValueError:
-    print("Please input number")
+    print("Please input number.")
 
 for choice in choices:
     if 0 < choice and choice < 6:
         mydict[choice]()
     else:
         print("That is not between 1 and 5! Try again:")
```

