# Comparing `tmp/pytrivialsql-0.1.4.tar.gz` & `tmp/pytrivialsql-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrivialsql-0.1.4.tar", last modified: Sat May  4 03:59:59 2024, max compression
+gzip compressed data, was "pytrivialsql-0.1.5.tar", last modified: Sun May  5 21:22:13 2024, max compression
```

## Comparing `pytrivialsql-0.1.4.tar` & `pytrivialsql-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:59.811452 pytrivialsql-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-04 03:59:44.000000 pytrivialsql-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-04 03:59:59.811452 pytrivialsql-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-04 03:59:44.000000 pytrivialsql-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-04 03:59:44.000000 pytrivialsql-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 03:59:59.811452 pytrivialsql-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:59.807453 pytrivialsql-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:59.811452 pytrivialsql-0.1.4/src/pytrivialsql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:44.000000 pytrivialsql-0.1.4/src/pytrivialsql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-05-04 03:59:44.000000 pytrivialsql-0.1.4/src/pytrivialsql/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     5439 2024-05-04 03:59:44.000000 pytrivialsql-0.1.4/src/pytrivialsql/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-05-04 03:59:44.000000 pytrivialsql-0.1.4/src/pytrivialsql/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:59.811452 pytrivialsql-0.1.4/src/pytrivialsql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-04 03:59:59.000000 pytrivialsql-0.1.4/src/pytrivialsql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-04 03:59:59.000000 pytrivialsql-0.1.4/src/pytrivialsql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 03:59:59.000000 pytrivialsql-0.1.4/src/pytrivialsql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-04 03:59:59.000000 pytrivialsql-0.1.4/src/pytrivialsql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-04 03:59:59.000000 pytrivialsql-0.1.4/src/pytrivialsql.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:59.811452 pytrivialsql-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-04 03:59:44.000000 pytrivialsql-0.1.4/tests/test_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     7369 2024-05-04 03:59:44.000000 pytrivialsql-0.1.4/tests/test_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-04 03:59:44.000000 pytrivialsql-0.1.4/tests/test_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:22:13.844227 pytrivialsql-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-05 21:21:57.000000 pytrivialsql-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-05 21:22:13.844227 pytrivialsql-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-05 21:21:57.000000 pytrivialsql-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-05 21:21:57.000000 pytrivialsql-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 21:22:13.844227 pytrivialsql-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:22:13.844227 pytrivialsql-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:22:13.844227 pytrivialsql-0.1.5/src/pytrivialsql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 21:21:57.000000 pytrivialsql-0.1.5/src/pytrivialsql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-05-05 21:21:57.000000 pytrivialsql-0.1.5/src/pytrivialsql/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-05 21:21:57.000000 pytrivialsql-0.1.5/src/pytrivialsql/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-05-05 21:21:57.000000 pytrivialsql-0.1.5/src/pytrivialsql/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:22:13.844227 pytrivialsql-0.1.5/src/pytrivialsql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-05 21:22:13.000000 pytrivialsql-0.1.5/src/pytrivialsql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-05 21:22:13.000000 pytrivialsql-0.1.5/src/pytrivialsql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 21:22:13.000000 pytrivialsql-0.1.5/src/pytrivialsql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-05 21:22:13.000000 pytrivialsql-0.1.5/src/pytrivialsql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-05 21:22:13.000000 pytrivialsql-0.1.5/src/pytrivialsql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:22:13.844227 pytrivialsql-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-05 21:21:57.000000 pytrivialsql-0.1.5/tests/test_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-05-05 21:21:57.000000 pytrivialsql-0.1.5/tests/test_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-05 21:21:57.000000 pytrivialsql-0.1.5/tests/test_sqlite.py
```

### Comparing `pytrivialsql-0.1.4/LICENSE` & `pytrivialsql-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytrivialsql-0.1.4/PKG-INFO` & `pytrivialsql-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrivialsql
-Version: 0.1.4
+Version: 0.1.5
 Summary: A trivial set of QOL bindings for SQL in Python
 Author-email: inaimathi <leo.zovic@gmail.com>
 Project-URL: Homepage, https://github.com/inaimathi/pytrivialsql
 Project-URL: Issues, https://github.com/inaimathi/pytrivialsql/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pytrivialsql-0.1.4/pyproject.toml` & `pytrivialsql-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytrivialsql"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="inaimathi", email="leo.zovic@gmail.com" },
 ]
 description = "A trivial set of QOL bindings for SQL in Python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pytrivialsql-0.1.4/src/pytrivialsql/postgres.py` & `pytrivialsql-0.1.5/src/pytrivialsql/postgres.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,26 +58,29 @@
 
     def create(self, table_name, props):
         with self._conn.cursor() as cur:
             cur.execute(sql.create_q(table_name, props))
             self._commit()
             return True
 
-    def select(self, table_name, columns, where=None, order_by=None, transform=None):
+    def select(
+        self, table_name, columns, where=None, order_by=None, limit=None, transform=None
+    ):
         try:
             with self._conn.cursor() as cur:
                 if columns is None:
                     columns = "*"
                 if isinstance(columns, str):
                     columns = [columns]
                 query, args = sql.select_q(
                     table_name,
                     columns,
                     where=where,
                     order_by=order_by,
+                    limit=limit,
                     placeholder="%s",
                 )
                 cur.execute(query, args)
                 cols = [col.name for col in cur.description]
                 res = (dict(zip(cols, vals)) for vals in cur.fetchall())
                 if transform is not None:
                     return [transform(el) for el in res]
```

### Comparing `pytrivialsql-0.1.4/src/pytrivialsql/sql.py` & `pytrivialsql-0.1.5/src/pytrivialsql/sql.py`

 * *Files 5% similar despite different names*

```diff
@@ -125,28 +125,36 @@
     return (
         f"INSERT INTO {table_name} ({', '.join(ks)}) VALUES ({', '.join([placeholder for v in vs])}){ret_clause}",
         tuple(vs),
     )
 
 
 def select_q(
-    table_name, columns, where=None, join=None, order_by=None, placeholder=None
+    table_name,
+    columns,
+    where=None,
+    join=None,
+    order_by=None,
+    limit=None,
+    placeholder=None,
 ):
     if placeholder is None:
         placeholder = "?"
     query = f"SELECT {', '.join(columns)} FROM {table_name}"
     args = ()
     if join is not None:
         query += join_to_string(join)
     if where is not None:
         where_str, where_args = where_to_string(where, placeholder)
         query += where_str
         args = where_args
     if order_by is not None:
         query += f" ORDER BY {order_by}"
+    if limit is not None:
+        query += f" LIMIT {limit}"
     return (query, args)
 
 
 def update_q(table_name, **kwargs):
     placeholder = kwargs.get("placeholder", "?")
     if "placeholder" in kwargs:
         del kwargs["placeholder"]
```

### Comparing `pytrivialsql-0.1.4/src/pytrivialsql/sqlite.py` & `pytrivialsql-0.1.5/src/pytrivialsql/sqlite.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,28 +79,30 @@
         try:
             with self._conn as cur:
                 cur.execute(sql.create_q(table_name, props))
                 return True
         except Exception:
             return False
 
-    def select(self, table_name, columns, where=None, order_by=None, transform=None):
+    def select(
+        self, table_name, columns, where=None, order_by=None, transform=None, limit=None
+    ):
         with self._conn as cur:
             c = cur.cursor()
             if columns is None or columns == "*":
                 columns = [
                     el[1]
                     for el in c.execute(f"PRAGMA table_info({table_name})").fetchall()
                 ]
             if not columns:
                 raise Exception(f"No such table {table_name}")
             elif isinstance(columns, str):
                 columns = [columns]
             query, args = sql.select_q(
-                table_name, columns, where=where, order_by=order_by
+                table_name, columns, where=where, order_by=order_by, limit=limit
             )
             c.execute(query, args)
             res = (dict(zip(columns, vals)) for vals in c.fetchall())
             if transform is not None:
                 return [transform(el) for el in res]
             return list(res)
```

### Comparing `pytrivialsql-0.1.4/src/pytrivialsql.egg-info/PKG-INFO` & `pytrivialsql-0.1.5/src/pytrivialsql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrivialsql
-Version: 0.1.4
+Version: 0.1.5
 Summary: A trivial set of QOL bindings for SQL in Python
 Author-email: inaimathi <leo.zovic@gmail.com>
 Project-URL: Homepage, https://github.com/inaimathi/pytrivialsql
 Project-URL: Issues, https://github.com/inaimathi/pytrivialsql/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pytrivialsql-0.1.4/tests/test_postgres.py` & `pytrivialsql-0.1.5/tests/test_postgres.py`

 * *Files identical despite different names*

### Comparing `pytrivialsql-0.1.4/tests/test_sql.py` & `pytrivialsql-0.1.5/tests/test_sql.py`

 * *Files 3% similar despite different names*

```diff
@@ -207,7 +207,15 @@
     def test_order_by(self):
         self.assertEqual(
             sql.select_q(
                 "table_name", ["id", "prop", "propb"], where={"a": 1}, order_by="prop"
             ),
             ("SELECT id, prop, propb FROM table_name WHERE a=? ORDER BY prop", (1,)),
         )
+
+    def test_limit(self):
+        self.assertEqual(
+            sql.select_q(
+                "table_name", ["id", "prop", "propb"], where={"a": 1}, limit=2
+            ),
+            ("SELECT id, prop, propb FROM table_name WHERE a=? LIMIT 2", (1,)),
+        )
```

### Comparing `pytrivialsql-0.1.4/tests/test_sqlite.py` & `pytrivialsql-0.1.5/tests/test_sqlite.py`

 * *Files identical despite different names*

