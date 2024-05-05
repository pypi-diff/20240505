# Comparing `tmp/unnecessary-abstraction-1.0.0.tar.gz` & `tmp/unnecessary_abstraction-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unnecessary-abstraction-1.0.0.tar", last modified: Wed Apr 17 22:28:33 2024, max compression
+gzip compressed data, was "unnecessary_abstraction-1.0.1.tar", max compression
```

## Comparing `unnecessary-abstraction-1.0.0.tar` & `unnecessary_abstraction-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 22:28:33.566867 unnecessary-abstraction-1.0.0/
--rw-rw-rw-   0        0        0      380 2024-04-17 22:28:33.565866 unnecessary-abstraction-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-17 22:28:33.549839 unnecessary-abstraction-1.0.0/database_interface/
--rw-rw-rw-   0        0        0      306 2024-04-17 21:48:39.000000 unnecessary-abstraction-1.0.0/database_interface/__init__.py
--rw-rw-rw-   0        0        0     3789 2024-04-17 10:39:30.000000 unnecessary-abstraction-1.0.0/database_interface/database.py
--rw-rw-rw-   0        0        0    15397 2024-02-24 03:42:20.000000 unnecessary-abstraction-1.0.0/database_interface/database_interface.py
--rw-rw-rw-   0        0        0     1499 2024-04-09 10:09:47.000000 unnecessary-abstraction-1.0.0/database_interface/postgis_interface.py
--rw-rw-rw-   0        0        0    16525 2024-04-17 11:29:55.000000 unnecessary-abstraction-1.0.0/database_interface/postgres_interface.py
--rw-rw-rw-   0        0        0     3799 2024-04-14 22:47:31.000000 unnecessary-abstraction-1.0.0/database_interface/schema_objects.py
--rw-rw-rw-   0        0        0    12791 2024-04-17 09:35:00.000000 unnecessary-abstraction-1.0.0/database_interface/sqlite_interface.py
--rw-rw-rw-   0        0        0       42 2024-04-17 22:28:33.566867 unnecessary-abstraction-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      540 2024-04-17 22:27:59.000000 unnecessary-abstraction-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 22:28:33.564868 unnecessary-abstraction-1.0.0/unnecessary_abstraction.egg-info/
--rw-rw-rw-   0        0        0      380 2024-04-17 22:28:33.000000 unnecessary-abstraction-1.0.0/unnecessary_abstraction.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      502 2024-04-17 22:28:33.000000 unnecessary-abstraction-1.0.0/unnecessary_abstraction.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 22:28:33.000000 unnecessary-abstraction-1.0.0/unnecessary_abstraction.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-17 22:28:33.000000 unnecessary-abstraction-1.0.0/unnecessary_abstraction.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-17 22:28:33.000000 unnecessary-abstraction-1.0.0/unnecessary_abstraction.egg-info/top_level.txt
+-rw-r--r--   0        0        0      424 2024-05-05 12:25:40.569669 unnecessary_abstraction-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-05 12:17:36.486574 unnecessary_abstraction-1.0.1/README.md
+-rw-r--r--   0        0        0      306 2024-04-17 21:48:39.000000 unnecessary_abstraction-1.0.1/unnecessary-abstraction/__init__.py
+-rw-r--r--   0        0        0     3789 2024-04-17 10:39:30.000000 unnecessary_abstraction-1.0.1/unnecessary-abstraction/database.py
+-rw-r--r--   0        0        0    15397 2024-02-24 03:42:20.000000 unnecessary_abstraction-1.0.1/unnecessary-abstraction/database_interface.py
+-rw-r--r--   0        0        0     1499 2024-04-09 10:09:47.000000 unnecessary_abstraction-1.0.1/unnecessary-abstraction/postgis_interface.py
+-rw-r--r--   0        0        0    16687 2024-05-05 02:12:30.904945 unnecessary_abstraction-1.0.1/unnecessary-abstraction/postgres_interface.py
+-rw-r--r--   0        0        0     3801 2024-05-05 02:09:59.336969 unnecessary_abstraction-1.0.1/unnecessary-abstraction/schema_objects.py
+-rw-r--r--   0        0        0    12833 2024-05-05 02:09:29.709757 unnecessary_abstraction-1.0.1/unnecessary-abstraction/sqlite_interface.py
+-rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 unnecessary_abstraction-1.0.1/PKG-INFO
```

### Comparing `unnecessary-abstraction-1.0.0/database_interface/database.py` & `unnecessary_abstraction-1.0.1/unnecessary-abstraction/database.py`

 * *Files identical despite different names*

### Comparing `unnecessary-abstraction-1.0.0/database_interface/database_interface.py` & `unnecessary_abstraction-1.0.1/unnecessary-abstraction/database_interface.py`

 * *Files identical despite different names*

### Comparing `unnecessary-abstraction-1.0.0/database_interface/postgis_interface.py` & `unnecessary_abstraction-1.0.1/unnecessary-abstraction/postgis_interface.py`

 * *Files identical despite different names*

### Comparing `unnecessary-abstraction-1.0.0/database_interface/postgres_interface.py` & `unnecessary_abstraction-1.0.1/unnecessary-abstraction/postgres_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from .database import Database
 from typing import Literal
 import psycopg2
 import pathlib
 import json
 import csv
+from datetime import datetime
 
 from .schema_objects import SQLColumn, SQLSchema
 
 TABLE_ACTION = Literal["INSERT", "UPDATE", "DELETE"]
 FOR_EACH = Literal["ROW", "STATEMENT"]
 
 POSTGRES_TYPES = Literal["integer", "smallint", "bigint", "real", "double precision", "decimal", "numeric", "text", 
@@ -107,15 +108,15 @@
         if csv_name in self.list_tables():
             print(f"{csv_name} is already a table in the database. You can alternatively use append_csv() if this is intended")
             return
         self.table_from_records(csv_name, records, col_overrides, schema_override, postgresql_schema)
 
     def table_to_records(self, table_name:str, columns:str="*", where_clause:str="", postgresql_schema:str="public") -> list[dict]:
         schema:SQLSchema = self.get_schema(table_name, postgresql_schema)
-        table_data = self.get_table(table_name, columns, where_clause)
+        table_data = self.get_table(table_name, columns, where_clause, postgresql_schema)
 
         if columns != "*":
             schema.filter_columns(columns.split(", "))
             
         records = []
         for row in table_data:
             record_row = {}
@@ -131,17 +132,17 @@
         headers = headers.keys()
 
         with open(f"{save_path}\\{table_name}.csv", 'w', newline='') as csv_file:
             writer = csv.DictWriter(csv_file, fieldnames=headers)
             writer.writeheader()
             writer.writerows(table_records)
     
-    def drop_table(self, table_name:str) -> None:
+    def drop_table(self, table_name:str, postgresql_schema:str) -> None:
         cur = self.db_conn.cursor()
-        cur.execute(f"DROP TABLE IF EXISTS {table_name}")
+        cur.execute(f"DROP TABLE IF EXISTS {postgresql_schema}.{table_name}")
         self.db_conn.commit()
     
     def delete_all_records(self, table_name:str, postgresql_schema:str="public") -> None:
         cur = self.db_conn.cursor()
         cur.execute(f"DELETE FROM {postgresql_schema}.{table_name}")
         self.db_conn.commit()
 
@@ -244,15 +245,15 @@
                 if col_val:
                     d_type = self.infer_type(col_val)
                 else:
                     d_type = self.infer_type(find_non_null_record(records, col_name))
                 
                 schema.append(SQLColumn(name=col_name, data_type=d_type, position=pos))
             pos += 1
-        return SQLColumn(schema)
+        return SQLSchema(schema)
 
     def select_table_statement(self, table_name:str, columns:str="*", where_clause:str="") -> str:
         statement = f"SELECT {columns} FROM {table_name}"
         if where_clause:
             statement += f" {where_clause}"
         return statement
     
@@ -323,14 +324,16 @@
         if type(val) == int or type(val) == float:
             if type(val) == int:
                 return "integer"
             elif type(val) == float:
                 return "decimal"
         elif type(val) == bool:
             return "text"
+        elif type(val) == datetime:
+            return "timestamp"
         else:
             val:str
             split = val.split(".")
             if len(split) == 2:
                 if split[0].isnumeric() and split[1].isnumeric():
                     if len(split[1]) > 8:
                         return "double precision"
```

### Comparing `unnecessary-abstraction-1.0.0/database_interface/schema_objects.py` & `unnecessary_abstraction-1.0.1/unnecessary-abstraction/schema_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Literal, TypedDict
 
 TYPES = Literal["integer", "smallint", "bigint", "real", "double precision", "decimal", "numeric", "smallserial", 
                 "serial", "bigserial", "text", "timestamp with time zone", "timestamp", "date", "time with time zone", 
                 "time", "interval", "uuid", "json", "jsonb", "geometry"]
 
 class ForeignKey(TypedDict):
-    refences_table:str
+    references_table:str
     references_col:str
 
 
 class SQLColumn:
     __slots__ = ('name', 'data_type', 'position', 'nullable', 'is_primary_key', 'foreign_key', 'is_unique', 'check_constraint')
     def __init__(self, name:str, data_type:TYPES, position:int = 0, 
                  nullable=True, is_unique:bool=False, is_primary_key:bool = False,
```

### Comparing `unnecessary-abstraction-1.0.0/database_interface/sqlite_interface.py` & `unnecessary_abstraction-1.0.1/unnecessary-abstraction/sqlite_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .database import Database
 import sqlite3
 import csv
+from datetime import datetime
 from typing import Literal
 import pathlib
 
 from .schema_objects import SQLColumn, SQLSchema
 
 SQLITE_TYPES = Literal["text", "real", "integer", "numeric"]
 
@@ -61,15 +62,14 @@
             update_statement = self.create_update_statement(table_name, row, f"WHERE {unique_key_col}='{row[unique_key_col]}'")
             cur.execute(update_statement)
         self.db_conn.commit()
 
     def delete_rows(self, table_name:str, where_clause:str) -> None:
         cur = self.db_conn.cursor()
         delete_statement = self.create_delete_statement(table_name, where_clause)
-        print(delete_statement)
         cur.execute(delete_statement)
         self.db_conn.commit()
 
     def append_csv_to_table(self, table_name:str, csv_path:str) -> None:
         csv_path:pathlib.Path = pathlib.Path(csv_path)
         with open(csv_path, newline='') as csv_file:
             reader = csv.DictReader(csv_file)
@@ -81,15 +81,14 @@
         with open(f"{csv_path}\\{csv_name}.csv", "w", newline='') as f:
             writer = csv.DictWriter(f, headers)
             writer.writeheader()
             writer.writerows(records)
 
     def create_blank_table(self, table_name:str, schema:SQLSchema) -> None:
         sql = self.create_table_statement(table_name, schema)
-        print(sql)
         cur = self.db_conn.cursor()
         cur.execute(sql)
         
     def csv_to_records(self, csv_path:str) -> list[dict]:
         csv_path:pathlib.Path = pathlib.Path(csv_path)
         with open(csv_path, newline='') as csv_file:
             reader = csv.DictReader(csv_file)
@@ -193,14 +192,16 @@
         if type(val) == int or type(val) == float:
             if type(val) == int:
                 return "integer"
             elif type(val) == float:
                 return "real"
         elif type(val) == bool:
             return "text"
+        elif type(val) == datetime:
+            return "text"
         else:
             val:str
             split = val.split(".")
             if len(split) == 2:
                 if split[0].isnumeric() and split[1].isnumeric():
                     return "real"
                 else:
```

