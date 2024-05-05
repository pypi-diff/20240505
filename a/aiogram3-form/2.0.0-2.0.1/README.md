# Comparing `tmp/aiogram3_form-2.0.0.tar.gz` & `tmp/aiogram3_form-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram3_form-2.0.0.tar", max compression
+gzip compressed data, was "aiogram3_form-2.0.1.tar", max compression
```

## Comparing `aiogram3_form-2.0.0.tar` & `aiogram3_form-2.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2024-03-07 12:57:37.589635 aiogram3_form-2.0.0/LICENSE
--rw-r--r--   0        0        0     1151 2024-03-12 23:29:50.534053 aiogram3_form-2.0.0/README.md
--rw-r--r--   0        0        0      520 2024-05-05 02:11:14.608700 aiogram3_form-2.0.0/aiogram3_form/__init__.py
--rw-r--r--   0        0        0     1308 2024-05-05 02:10:43.371085 aiogram3_form-2.0.0/aiogram3_form/field.py
--rw-r--r--   0        0        0     2832 2024-05-05 02:09:33.376424 aiogram3_form-2.0.0/aiogram3_form/filters.py
--rw-r--r--   0        0        0     7071 2024-05-05 02:12:28.234533 aiogram3_form-2.0.0/aiogram3_form/form.py
--rw-r--r--   0        0        0      392 2024-05-04 07:33:11.731995 aiogram3_form-2.0.0/aiogram3_form/utils.py
--rw-r--r--   0        0        0      505 2024-05-05 02:12:38.085043 aiogram3_form-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1744 1970-01-01 00:00:00.000000 aiogram3_form-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-03-07 12:57:37.589635 aiogram3_form-2.0.1/LICENSE
+-rw-r--r--   0        0        0     1151 2024-03-12 23:29:50.534053 aiogram3_form-2.0.1/README.md
+-rw-r--r--   0        0        0      520 2024-05-05 02:15:13.841401 aiogram3_form-2.0.1/aiogram3_form/__init__.py
+-rw-r--r--   0        0        0     1308 2024-05-05 02:10:43.371085 aiogram3_form-2.0.1/aiogram3_form/field.py
+-rw-r--r--   0        0        0     2832 2024-05-05 02:09:33.376424 aiogram3_form-2.0.1/aiogram3_form/filters.py
+-rw-r--r--   0        0        0     7146 2024-05-05 02:16:40.466887 aiogram3_form-2.0.1/aiogram3_form/form.py
+-rw-r--r--   0        0        0      392 2024-05-04 07:33:11.731995 aiogram3_form-2.0.1/aiogram3_form/utils.py
+-rw-r--r--   0        0        0      505 2024-05-05 02:16:44.438370 aiogram3_form-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1744 1970-01-01 00:00:00.000000 aiogram3_form-2.0.1/PKG-INFO
```

### Comparing `aiogram3_form-2.0.0/LICENSE` & `aiogram3_form-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiogram3_form-2.0.0/README.md` & `aiogram3_form-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `aiogram3_form-2.0.0/aiogram3_form/__init__.py` & `aiogram3_form-2.0.1/aiogram3_form/__init__.py`

 * *Files identical despite different names*

### Comparing `aiogram3_form-2.0.0/aiogram3_form/field.py` & `aiogram3_form-2.0.1/aiogram3_form/field.py`

 * *Files identical despite different names*

### Comparing `aiogram3_form-2.0.0/aiogram3_form/filters.py` & `aiogram3_form-2.0.1/aiogram3_form/filters.py`

 * *Files identical despite different names*

### Comparing `aiogram3_form-2.0.0/aiogram3_form/form.py` & `aiogram3_form-2.0.1/aiogram3_form/form.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,17 @@
 class FormSubmitData(NamedTuple):
     callback: SubmitCallback
     clear_state: bool
 
 
 class Form(ABC, metaclass=FormMeta):
     fields: tuple[FormFieldData, ...]
-    __submit_data: FormSubmitData
+
+    __submit_data: FormSubmitData = None  # type: ignore
+    # this should be set by the user via .submit()
 
     def __init__(self, bot: Bot, chat_id: int):
         self.bot = bot
         self.chat_id = chat_id
 
     @classmethod
     def submit(cls, *, router: Router, clear_state: bool = True):
```

### Comparing `aiogram3_form-2.0.0/PKG-INFO` & `aiogram3_form-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogram3-form
-Version: 2.0.0
+Version: 2.0.1
 Summary: A library to create forms in aiogram3
 License: MIT
 Author: TrixiS
 Author-email: oficialmorozov@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

