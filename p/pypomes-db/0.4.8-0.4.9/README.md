# Comparing `tmp/pypomes_db-0.4.8.tar.gz` & `tmp/pypomes_db-0.4.9.tar.gz`

## Comparing `pypomes_db-0.4.8.tar` & `pypomes_db-0.4.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 pypomes_db-0.4.8/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0     7853 2020-02-02 00:00:00.000000 pypomes_db-0.4.8/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    19681 2020-02-02 00:00:00.000000 pypomes_db-0.4.8/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.8/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    12532 2020-02-02 00:00:00.000000 pypomes_db-0.4.8/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    10382 2020-02-02 00:00:00.000000 pypomes_db-0.4.8/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    10670 2020-02-02 00:00:00.000000 pypomes_db-0.4.8/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.4.8/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.4.8/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.8/README.md
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pypomes_db-0.4.8/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 pypomes_db-0.4.9/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0     7853 2020-02-02 00:00:00.000000 pypomes_db-0.4.9/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    19806 2020-02-02 00:00:00.000000 pypomes_db-0.4.9/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.9/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    12532 2020-02-02 00:00:00.000000 pypomes_db-0.4.9/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    10382 2020-02-02 00:00:00.000000 pypomes_db-0.4.9/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    10670 2020-02-02 00:00:00.000000 pypomes_db-0.4.9/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.4.9/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.4.9/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.9/README.md
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pypomes_db-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.4.9/PKG-INFO
```

### Comparing `pypomes_db-0.4.8/src/pypomes_db/__init__.py` & `pypomes_db-0.4.9/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.8/src/pypomes_db/db_common.py` & `pypomes_db-0.4.9/src/pypomes_db/db_common.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.8/src/pypomes_db/db_pomes.py` & `pypomes_db-0.4.9/src/pypomes_db/db_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,16 @@
 
     The returned *dict* contains the keys *name*, *user*, *pwd*, *host*, *port*.
     The meaning of these parameters may vary between different database engines.
 
     :param engine: the database engine
     :return: the current connection parameters for the engine
     """
-    return _DB_CONN_DATA.get(engine or _DB_ENGINES[0])
+    curr_engine: str = _DB_ENGINES[0] if not engine and _DB_ENGINES else engine
+    return _DB_CONN_DATA.get(engine or curr_engine)
 
 
 def db_assert_connection(errors: list[str] | None,
                          engine: str = None,
                          logger: Logger = None) -> bool:
     """
     Determine whether the *engine*'s current configuration allows for a safe connection.
@@ -144,16 +145,16 @@
         result = sqlserver_pomes.db_connect(errors, logger)
 
     return result
 
 
 def db_exists(errors: list[str],
               table: str,
-              where_attrs: list[str],
-              where_vals: tuple,
+              where_attrs: list[str] = None,
+              where_vals: tuple = None,
               engine: str = None,
               logger: Logger = None) -> bool:
     """
     Determine whether the table *table* in the database contains at least one tuple.
 
     For this determination, *where_attrs* are made equal to *where_values* in the query, respectively.
     If more than one, the attributes are concatenated by the *AND* logical connector.
@@ -165,30 +166,30 @@
     :param where_vals: the values for the search attributes
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param logger: optional logger
     :return: True if at least one tuple was found
     """
     # noinspection PyDataSource
     sel_stmt: str = "SELECT * FROM " + table
-    if len(where_attrs) > 0:
+    if where_attrs:
         sel_stmt += " WHERE " + "".join(f"{attr} = %s AND " for attr in where_attrs)[0:-5]
     rec: tuple = db_select_one(errors=errors,
                                sel_stmt=sel_stmt,
                                where_vals=where_vals,
                                require_nonempty=False,
                                engine = engine,
                                logger=logger)
     result: bool = None if len(errors) > 0 else rec is not None
 
     return result
 
 
 def db_select_one(errors: list[str] | None,
                   sel_stmt: str,
-                  where_vals: tuple,
+                  where_vals: tuple = None,
                   require_nonempty: bool = False,
                   engine: str = None,
                   logger: Logger = None) -> tuple:
     """
     Search the database and return the first tuple that satisfies the *sel_stmt* search command.
 
     The command can optionally contain search criteria, with respective values given
@@ -281,16 +282,16 @@
     :return: the number of inserted tuples (0 ou 1), or None if an error occurred
     """
     return db_execute(errors, insert_stmt, insert_vals, engine, logger)
 
 
 def db_update(errors: list[str] | None,
               update_stmt: str,
-              update_vals: tuple,
-              where_vals: tuple,
+              update_vals: tuple = None,
+              where_vals: tuple = None,
               engine: str = None,
               logger: Logger = None) -> int:
     """
     Update one or more tuples in the database, as defined by the command *update_stmt*.
 
     The values for this update are in *update_vals*.
     The values for selecting the tuples to be updated are in *where_vals*.
@@ -305,15 +306,15 @@
     :return: the number of updated tuples, or None if an error occurred
     """
     return db_execute(errors, update_stmt, update_vals + where_vals, engine, logger)
 
 
 def db_delete(errors: list[str] | None,
               delete_stmt: str,
-              where_vals: tuple,
+              where_vals: tuple = None,
               engine: str = None,
               logger: Logger = None) -> int:
     """
     Delete one or more tuples in the database, as defined by the *delete_stmt* command.
 
     The values for selecting the tuples to be deleted are in *where_vals*.
     The target database engine, default or specified, must have been previously configured.
@@ -404,15 +405,15 @@
         result = sqlserver_pomes.db_execute(errors, exc_stmt, bind_vals, logger)
 
     return result
 
 
 def db_call_function(errors: list[str] | None,
                      func_name: str,
-                     func_vals: tuple,
+                     func_vals: tuple = None,
                      engine: str = None,
                      logger: Logger = None) -> list[tuple]:
     """
     Execute the stored function *func_name* in the database, with the parameters given in *func_vals*.
 
     The target database engine, default or specified, must have been previously configured.
 
@@ -440,15 +441,15 @@
         result = sqlserver_pomes.db_call_procedure(errors, func_name, func_vals, logger)
 
     return result
 
 
 def db_call_procedure(errors: list[str] | None,
                       proc_name: str,
-                      proc_vals: tuple,
+                      proc_vals: tuple = None,
                       engine: str = None,
                       logger: Logger = None) -> list[tuple]:
     """
     Execute the stored procedure *proc_name* in the database, with the parameters given in *proc_vals*.
 
     The target database engine, default or specified, must have been previously configured.
```

### Comparing `pypomes_db-0.4.8/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.4.9/src/pypomes_db/oracle_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.8/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.4.9/src/pypomes_db/postgres_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.8/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.4.9/src/pypomes_db/sqlserver_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.8/LICENSE` & `pypomes_db-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.8/pyproject.toml` & `pypomes_db-0.4.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.4.8"
+version = "0.4.9"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.4.8/PKG-INFO` & `pypomes_db-0.4.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.4.8
+Version: 0.4.9
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

