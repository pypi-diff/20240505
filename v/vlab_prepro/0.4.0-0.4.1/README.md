# Comparing `tmp/vlab_prepro-0.4.0.tar.gz` & `tmp/vlab_prepro-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vlab_prepro-0.4.0.tar", max compression
+gzip compressed data, was "vlab_prepro-0.4.1.tar", max compression
```

## Comparing `vlab_prepro-0.4.0.tar` & `vlab_prepro-0.4.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1172 2021-05-18 16:46:20.874302 vlab_prepro-0.4.0/LICENSE
--rw-r--r--   0        0        0      513 2023-07-01 17:23:54.900706 vlab_prepro-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      160 2021-09-07 08:20:12.702045 vlab_prepro-0.4.0/vlab_prepro/__init__.py
--rw-r--r--   0        0        0     8098 2023-07-01 17:20:13.800915 vlab_prepro-0.4.0/vlab_prepro/preprocess.py
--rw-r--r--   0        0        0      429 1970-01-01 00:00:00.000000 vlab_prepro-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1172 2021-05-18 16:46:20.874302 vlab_prepro-0.4.1/LICENSE
+-rw-r--r--   0        0        0      513 2024-05-05 21:03:32.977874 vlab_prepro-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      160 2021-09-07 08:20:12.702045 vlab_prepro-0.4.1/vlab_prepro/__init__.py
+-rw-r--r--   0        0        0     8330 2024-05-05 21:03:14.910985 vlab_prepro-0.4.1/vlab_prepro/preprocess.py
+-rw-r--r--   0        0        0      480 1970-01-01 00:00:00.000000 vlab_prepro-0.4.1/PKG-INFO
```

### Comparing `vlab_prepro-0.4.0/LICENSE` & `vlab_prepro-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vlab_prepro-0.4.0/pyproject.toml` & `vlab_prepro-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vlab_prepro"
-version = "0.4.0"
+version = "0.4.1"
 description = ""
 authors = ["Nandan Rao <nandanmarkrao@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 toolz = "^0.11.1"
 pandas = "^2.0.3"
```

### Comparing `vlab_prepro-0.4.0/vlab_prepro/preprocess.py` & `vlab_prepro-0.4.1/vlab_prepro/preprocess.py`

 * *Files 5% similar despite different names*

```diff
@@ -148,15 +148,21 @@
         df = df.drop(self.form_df.columns, axis=1)
         self.keys = self.keys - set(self.form_df.columns)
         self.form_df = None
         return df
 
     @curry
     def add_metadata(self, keys, df):
+        question_refs = df.question_ref.unique()
         for key in keys:
+            if key in question_refs:
+                raise PreprocessingError(
+                    f"Trying to add metadata that already exists as a column: {key}"
+                )
+
             df[key] = df.metadata.map(lambda x: json.loads(x).get(key))
             self.keys.add(key)
         return df
 
     @curry
     def parse_timestamp(self, df):
         # NOTE: If ISO has TZ info, then it will be TZ aware, otherwise
```

