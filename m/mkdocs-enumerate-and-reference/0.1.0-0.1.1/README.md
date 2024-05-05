# Comparing `tmp/mkdocs_enumerate_and_reference-0.1.0.tar.gz` & `tmp/mkdocs_enumerate_and_reference-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_enumerate_and_reference-0.1.0.tar", max compression
+gzip compressed data, was "mkdocs_enumerate_and_reference-0.1.1.tar", max compression
```

## Comparing `mkdocs_enumerate_and_reference-0.1.0.tar` & `mkdocs_enumerate_and_reference-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2024-05-03 18:02:55.372146 mkdocs_enumerate_and_reference-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     1902 2024-05-03 18:02:55.372146 mkdocs_enumerate_and_reference-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-03 18:02:55.376146 mkdocs_enumerate_and_reference-0.1.0/mkdocs_enumerate_and_reference/__init__.py
--rw-r--r--   0        0        0     2153 2024-05-03 18:02:55.376146 mkdocs_enumerate_and_reference-0.1.0/mkdocs_enumerate_and_reference/enumerate.py
--rw-r--r--   0        0        0     4075 2024-05-03 18:02:55.376146 mkdocs_enumerate_and_reference-0.1.0/mkdocs_enumerate_and_reference/plugin.py
--rw-r--r--   0        0        0     1239 2024-05-03 18:02:55.376146 mkdocs_enumerate_and_reference-0.1.0/mkdocs_enumerate_and_reference/reference.py
--rw-r--r--   0        0        0      908 2024-05-03 18:02:55.376146 mkdocs_enumerate_and_reference-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2518 1970-01-01 00:00:00.000000 mkdocs_enumerate_and_reference-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-05 10:55:11.707388 mkdocs_enumerate_and_reference-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     1902 2024-05-05 10:55:11.707388 mkdocs_enumerate_and_reference-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-05 10:55:11.707388 mkdocs_enumerate_and_reference-0.1.1/mkdocs_enumerate_and_reference/__init__.py
+-rw-r--r--   0        0        0     2153 2024-05-05 10:55:11.707388 mkdocs_enumerate_and_reference-0.1.1/mkdocs_enumerate_and_reference/enumerate.py
+-rw-r--r--   0        0        0     4076 2024-05-05 10:55:11.707388 mkdocs_enumerate_and_reference-0.1.1/mkdocs_enumerate_and_reference/plugin.py
+-rw-r--r--   0        0        0     1239 2024-05-05 10:55:11.707388 mkdocs_enumerate_and_reference-0.1.1/mkdocs_enumerate_and_reference/reference.py
+-rw-r--r--   0        0        0      908 2024-05-05 10:55:11.711388 mkdocs_enumerate_and_reference-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2518 1970-01-01 00:00:00.000000 mkdocs_enumerate_and_reference-0.1.1/PKG-INFO
```

### Comparing `mkdocs_enumerate_and_reference-0.1.0/LICENSE.txt` & `mkdocs_enumerate_and_reference-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mkdocs_enumerate_and_reference-0.1.0/README.md` & `mkdocs_enumerate_and_reference-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_enumerate_and_reference-0.1.0/mkdocs_enumerate_and_reference/enumerate.py` & `mkdocs_enumerate_and_reference-0.1.1/mkdocs_enumerate_and_reference/enumerate.py`

 * *Files identical despite different names*

### Comparing `mkdocs_enumerate_and_reference-0.1.0/mkdocs_enumerate_and_reference/plugin.py` & `mkdocs_enumerate_and_reference-0.1.1/mkdocs_enumerate_and_reference/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         for page in nav.pages:
             source = read_source(page)
             tag_ids = re.findall(r'@tag\((.+?)\)', source)
             self.config.tags_paths.update({k: page.url for k in tag_ids})
             # next line is to prevent reading source twice
             # config.sources.update({page.file.src_path: source})
     
-    def on_page_markdown(self, markdown, page, config  **kwargs):
+    def on_page_markdown(self, markdown, page, config,  **kwargs):
         if self.config.number_headings.enabled:
             activated, lowest_level = self.get_number_headings_params(page.meta)
             if activated:
                 markdown = add_section_numbers(markdown, lowest_level=lowest_level)
 
         cnumber = page.cnumber if hasattr(page, "cnumber") else None
         markdown = refactor_admonitions(markdown, cnumber)
```

### Comparing `mkdocs_enumerate_and_reference-0.1.0/mkdocs_enumerate_and_reference/reference.py` & `mkdocs_enumerate_and_reference-0.1.1/mkdocs_enumerate_and_reference/reference.py`

 * *Files identical despite different names*

### Comparing `mkdocs_enumerate_and_reference-0.1.0/pyproject.toml` & `mkdocs_enumerate_and_reference-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mkdocs-enumerate-and-reference"
-version = "0.1.0"
+version = "0.1.1"
 description = "Mkdocs plugin for numbering and referencing"
 authors = ["Raphaël Mammeri <raphael.mammeri@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `mkdocs_enumerate_and_reference-0.1.0/PKG-INFO` & `mkdocs_enumerate_and_reference-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-enumerate-and-reference
-Version: 0.1.0
+Version: 0.1.1
 Summary: Mkdocs plugin for numbering and referencing
 License: MIT
 Author: Raphaël Mammeri
 Author-email: raphael.mammeri@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

