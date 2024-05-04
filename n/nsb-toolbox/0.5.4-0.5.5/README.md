# Comparing `tmp/nsb_toolbox-0.5.4.tar.gz` & `tmp/nsb_toolbox-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsb_toolbox-0.5.4.tar", max compression
+gzip compressed data, was "nsb_toolbox-0.5.5.tar", max compression
```

## Comparing `nsb_toolbox-0.5.4.tar` & `nsb_toolbox-0.5.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1074 2023-10-13 20:02:31.400071 nsb_toolbox-0.5.4/LICENSE.txt
--rw-r--r--   0        0        0    15644 2023-10-13 20:02:31.400071 nsb_toolbox-0.5.4/README.md
--rw-r--r--   0        0        0        2 2023-10-13 20:02:31.404071 nsb_toolbox-0.5.4/nsb_toolbox/__init__.py
--rw-r--r--   0        0        0     4563 2023-10-13 20:02:31.404071 nsb_toolbox-0.5.4/nsb_toolbox/_base_questions.py
--rw-r--r--   0        0        0    10499 2023-10-13 20:02:31.404071 nsb_toolbox-0.5.4/nsb_toolbox/assign.py
--rw-r--r--   0        0        0     3629 2023-10-13 20:02:31.404071 nsb_toolbox-0.5.4/nsb_toolbox/classes.py
--rw-r--r--   0        0        0     3148 2023-10-13 20:02:31.404071 nsb_toolbox-0.5.4/nsb_toolbox/cli.py
--rw-r--r--   0        0        0     8468 2023-10-13 20:02:31.404071 nsb_toolbox-0.5.4/nsb_toolbox/docx_utils.py
--rw-r--r--   0        0        0      972 2023-10-13 20:02:31.404071 nsb_toolbox-0.5.4/nsb_toolbox/importers.py
--rw-r--r--   0        0        0    20066 2023-10-13 20:02:31.404071 nsb_toolbox-0.5.4/nsb_toolbox/tables.py
--rw-r--r--   0        0        0     9971 2023-10-13 20:02:31.404071 nsb_toolbox-0.5.4/nsb_toolbox/yamlparsers.py
--rw-r--r--   0        0        0      912 2023-10-13 20:02:31.404071 nsb_toolbox-0.5.4/pyproject.toml
--rw-r--r--   0        0        0    16192 1970-01-01 00:00:00.000000 nsb_toolbox-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-04 22:37:01.729772 nsb_toolbox-0.5.5/LICENSE.txt
+-rw-r--r--   0        0        0    15644 2024-05-04 22:37:01.729772 nsb_toolbox-0.5.5/README.md
+-rw-r--r--   0        0        0        2 2024-05-04 22:37:01.733772 nsb_toolbox-0.5.5/nsb_toolbox/__init__.py
+-rw-r--r--   0        0        0     4563 2024-05-04 22:37:01.733772 nsb_toolbox-0.5.5/nsb_toolbox/_base_questions.py
+-rw-r--r--   0        0        0    10499 2024-05-04 22:37:01.733772 nsb_toolbox-0.5.5/nsb_toolbox/assign.py
+-rw-r--r--   0        0        0     3629 2024-05-04 22:37:01.733772 nsb_toolbox-0.5.5/nsb_toolbox/classes.py
+-rw-r--r--   0        0        0     3148 2024-05-04 22:37:01.733772 nsb_toolbox-0.5.5/nsb_toolbox/cli.py
+-rw-r--r--   0        0        0     8468 2024-05-04 22:37:01.733772 nsb_toolbox-0.5.5/nsb_toolbox/docx_utils.py
+-rw-r--r--   0        0        0      972 2024-05-04 22:37:01.733772 nsb_toolbox-0.5.5/nsb_toolbox/importers.py
+-rw-r--r--   0        0        0    20074 2024-05-04 22:37:01.733772 nsb_toolbox-0.5.5/nsb_toolbox/tables.py
+-rw-r--r--   0        0        0     9971 2024-05-04 22:37:01.733772 nsb_toolbox-0.5.5/nsb_toolbox/yamlparsers.py
+-rw-r--r--   0        0        0      917 2024-05-04 22:37:01.733772 nsb_toolbox-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0    16243 1970-01-01 00:00:00.000000 nsb_toolbox-0.5.5/PKG-INFO
```

### Comparing `nsb_toolbox-0.5.4/LICENSE.txt` & `nsb_toolbox-0.5.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nsb_toolbox-0.5.4/README.md` & `nsb_toolbox-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `nsb_toolbox-0.5.4/nsb_toolbox/_base_questions.py` & `nsb_toolbox-0.5.5/nsb_toolbox/_base_questions.py`

 * *Files identical despite different names*

### Comparing `nsb_toolbox-0.5.4/nsb_toolbox/assign.py` & `nsb_toolbox-0.5.5/nsb_toolbox/assign.py`

 * *Files identical despite different names*

### Comparing `nsb_toolbox-0.5.4/nsb_toolbox/classes.py` & `nsb_toolbox-0.5.5/nsb_toolbox/classes.py`

 * *Files identical despite different names*

### Comparing `nsb_toolbox-0.5.4/nsb_toolbox/cli.py` & `nsb_toolbox-0.5.5/nsb_toolbox/cli.py`

 * *Files identical despite different names*

### Comparing `nsb_toolbox-0.5.4/nsb_toolbox/docx_utils.py` & `nsb_toolbox-0.5.5/nsb_toolbox/docx_utils.py`

 * *Files identical despite different names*

### Comparing `nsb_toolbox-0.5.4/nsb_toolbox/importers.py` & `nsb_toolbox-0.5.5/nsb_toolbox/importers.py`

 * *Files identical despite different names*

### Comparing `nsb_toolbox-0.5.4/nsb_toolbox/tables.py` & `nsb_toolbox-0.5.5/nsb_toolbox/tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -546,15 +546,15 @@
     q_type_run.text, q_type_run.italic = _q_type.value, True
     return _q_type
 
 
 def _format_answer_line(
     para: Paragraph, test_choice_match: re.Match, choices: Dict[int, Paragraph]
 ):
-    choice_num = CHOICES.index(test_choice_match.group(1) + ")")
+    choice_num = CHOICES.index(test_choice_match.group(1).upper() + ")")
     # if answer line is a single letter with an optional ), copy the
     # text of the correct choice over to the answer line
     if test_choice_match.span()[1] <= test_choice_match.span(1)[1] + 1:
         correct_para = choices[choice_num]
         para.text = "ANSWER: "
         for run in correct_para.runs:
             run_copy = deepcopy(run._r)
```

### Comparing `nsb_toolbox-0.5.4/nsb_toolbox/yamlparsers.py` & `nsb_toolbox-0.5.5/nsb_toolbox/yamlparsers.py`

 * *Files identical despite different names*

### Comparing `nsb_toolbox-0.5.4/pyproject.toml` & `nsb_toolbox-0.5.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nsb-toolbox"
-version = "0.5.4"
+version = "0.5.5"
 repository = "https://github.com/rishi-kulkarni/nsbtoolbox"
 description = "Utilities for editing Science Bowl questions"
 authors = ["Rishi Kulkarni <rishi@kulkarni.science>"]
 license = "LICENSE.txt"
 readme = "README.md"
 packages = [{include = "nsb_toolbox"}]
 classifiers = [
@@ -21,15 +21,15 @@
 python = "^3.8.1"
 python-docx = "^0.8.11"
 pyyaml = "^6.0"
 scipy = "^1.8.0"
 typing-extensions = "^4.2.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.12.0"
+black = ">=22.12,<25.0"
 flake8 = "^6.0.0"
 ipython = "^8.8.0"
 pytest = "^7.2.1"
 
 [tool.pytest.ini_options]
 addopts = "-v"
```

### Comparing `nsb_toolbox-0.5.4/PKG-INFO` & `nsb_toolbox-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: nsb-toolbox
-Version: 0.5.4
+Version: 0.5.5
 Summary: Utilities for editing Science Bowl questions
 Home-page: https://github.com/rishi-kulkarni/nsbtoolbox
 License: LICENSE.txt
 Author: Rishi Kulkarni
 Author-email: rishi@kulkarni.science
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: python-docx (>=0.8.11,<0.9.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: scipy (>=1.8.0,<2.0.0)
 Requires-Dist: typing-extensions (>=4.2.0,<5.0.0)
 Project-URL: Repository, https://github.com/rishi-kulkarni/nsbtoolbox
 Description-Content-Type: text/markdown
```

