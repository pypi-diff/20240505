# Comparing `tmp/pypomes_db-0.4.5.tar.gz` & `tmp/pypomes_db-0.4.6.tar.gz`

## Comparing `pypomes_db-0.4.5.tar` & `pypomes_db-0.4.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 pypomes_db-0.4.5/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 pypomes_db-0.4.5/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    19681 2020-02-02 00:00:00.000000 pypomes_db-0.4.5/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.5/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    12254 2020-02-02 00:00:00.000000 pypomes_db-0.4.5/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    10382 2020-02-02 00:00:00.000000 pypomes_db-0.4.5/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    10501 2020-02-02 00:00:00.000000 pypomes_db-0.4.5/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.4.5/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.4.5/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.5/README.md
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pypomes_db-0.4.5/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 pypomes_db-0.4.6/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 pypomes_db-0.4.6/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    19681 2020-02-02 00:00:00.000000 pypomes_db-0.4.6/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.6/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    12254 2020-02-02 00:00:00.000000 pypomes_db-0.4.6/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    10382 2020-02-02 00:00:00.000000 pypomes_db-0.4.6/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    10501 2020-02-02 00:00:00.000000 pypomes_db-0.4.6/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.4.6/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.4.6/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.6/README.md
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pypomes_db-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.4.6/PKG-INFO
```

### Comparing `pypomes_db-0.4.5/src/pypomes_db/__init__.py` & `pypomes_db-0.4.6/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.5/src/pypomes_db/db_common.py` & `pypomes_db-0.4.6/src/pypomes_db/db_common.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.5/src/pypomes_db/db_pomes.py` & `pypomes_db-0.4.6/src/pypomes_db/db_pomes.py`

 * *Files 0% similar despite different names*

```diff
@@ -362,15 +362,15 @@
         result = sqlserver_pomes.db_bulk_insert(errors, insert_stmt, insert_vals, logger)
 
     return result
 
 
 def db_execute(errors: list[str] | None,
                exc_stmt: str,
-               bind_vals: tuple | None,
+               bind_vals: tuple = None,
                engine: str = None,
                logger: Logger = None) -> int:
     """
     Execute the command *exc_stmt* on the database.
 
     This command might be a DML ccommand modifying the database, such as
     inserting, updating or deleting tuples, or it might be a DDL statement,
```

### Comparing `pypomes_db-0.4.5/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.4.6/src/pypomes_db/oracle_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.5/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.4.6/src/pypomes_db/postgres_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.5/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.4.6/src/pypomes_db/sqlserver_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.5/LICENSE` & `pypomes_db-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.5/pyproject.toml` & `pypomes_db-0.4.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.4.5"
+version = "0.4.6"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.4.5/PKG-INFO` & `pypomes_db-0.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.4.5
+Version: 0.4.6
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

