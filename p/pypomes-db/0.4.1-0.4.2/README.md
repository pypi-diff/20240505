# Comparing `tmp/pypomes_db-0.4.1.tar.gz` & `tmp/pypomes_db-0.4.2.tar.gz`

## Comparing `pypomes_db-0.4.1.tar` & `pypomes_db-0.4.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 pypomes_db-0.4.1/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 pypomes_db-0.4.1/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    16563 2020-02-02 00:00:00.000000 pypomes_db-0.4.1/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.1/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    12320 2020-02-02 00:00:00.000000 pypomes_db-0.4.1/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    10231 2020-02-02 00:00:00.000000 pypomes_db-0.4.1/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    10350 2020-02-02 00:00:00.000000 pypomes_db-0.4.1/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.4.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.4.1/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.1/README.md
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pypomes_db-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 pypomes_db-0.4.2/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 pypomes_db-0.4.2/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    19054 2020-02-02 00:00:00.000000 pypomes_db-0.4.2/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.2/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    12320 2020-02-02 00:00:00.000000 pypomes_db-0.4.2/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    10231 2020-02-02 00:00:00.000000 pypomes_db-0.4.2/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    10350 2020-02-02 00:00:00.000000 pypomes_db-0.4.2/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.4.2/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.4.2/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.2/README.md
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pypomes_db-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.4.2/PKG-INFO
```

### Comparing `pypomes_db-0.4.1/src/pypomes_db/__init__.py` & `pypomes_db-0.4.2/src/pypomes_db/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from .db_pomes import (
-    db_setup, db_get_params,
+    db_setup, db_get_engines, db_get_params,
     db_connect, db_exists, db_select_one, db_select_all,
     db_update, db_delete, db_insert, db_bulk_insert,
     db_call_function, db_call_procedure,
 )
 
 __all__ = [
     # db_pomes
-    "db_setup", "db_get_params",
+    "db_setup", "db_get_engines", "db_get_params",
     "db_connect", "db_exists", "db_select_one", "db_select_all",
     "db_update", "db_delete", "db_insert", "db_bulk_insert",
     "db_call_function", "db_call_procedure",
 ]
 
 from importlib.metadata import version
 __version__ = version("pypomes_db")
```

### Comparing `pypomes_db-0.4.1/src/pypomes_db/db_common.py` & `pypomes_db-0.4.2/src/pypomes_db/db_common.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.1/src/pypomes_db/db_pomes.py` & `pypomes_db-0.4.2/src/pypomes_db/db_pomes.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,77 +5,93 @@
 
 
 def db_setup(engine: str,
              db_name: str,
              db_user: str,
              db_pwd: str,
              db_host: str,
-             db_port: str,
+             db_port: int,
              db_client: str = None,
-             db_driver: str = None) -> None:
+             db_driver: str = None) -> bool:
     """
     Establish the provided parameters for access to *engine*.
 
     The meaning of some parameters may vary between different database engines.
+    All parameters, with the exception of *db_client* and *db_driver*, are required.
+    *db_client* may be provided for *oracle*, but not for the other engines.
+    *db_driver* is required for *sqlserver*, but is not accepted for the other engines.
 
     :param engine: the database engine (one of [mysql, oracle, postgres, sqlserver])
     :param db_name: the database or service name
     :param db_user: the logon user
     :param db_pwd: the logon password
     :param db_host: the host URL
-    :param db_port: the connection
+    :param db_port: the connection port (a positive integer)
     :param db_driver: the database driver (SQLServer only)
     :param db_client: the path to the client software (optional, Oracle only)
+    :return: True if data was accepted, False otherwise
     """
-    _DB_CONN_DATA[engine] = {
-        "name": db_name,
-        "user": db_user,
-        "pwd": db_pwd,
-        "host": db_host,
-        "port": db_port
-    }
-    if engine == "oracle":
-        _DB_CONN_DATA[engine]["client"] = db_client
-    elif engine == "sqlserver":
-        _DB_CONN_DATA[engine]["driver"] = db_driver
+    # initialize the return variable
+    result: bool = False
+
+    # are the parameters compliant ?
+    if (engine in ["mysql", "oracle", "postgres", "sqlserver"] and
+        db_name and db_user and db_pwd and db_host and
+        not (engine != "oracle" and db_client) and
+        not (engine != "sqlserver" and db_driver) and
+        not (engine == "sqlserver" and not db_driver) and
+        isinstance(db_port, int) and db_port > 0):
+        _DB_CONN_DATA[engine] = {
+            "name": db_name,
+            "user": db_user,
+            "pwd": db_pwd,
+            "host": db_host,
+            "port": db_port
+        }
+        if engine == "oracle":
+            _DB_CONN_DATA[engine]["client"] = db_client
+        elif engine == "sqlserver":
+            _DB_CONN_DATA[engine]["driver"] = db_driver
+        if engine not in _DB_ENGINES:
+            _DB_ENGINES.append(engine)
+        result = True
 
-    if engine not in _DB_ENGINES:
-        _DB_ENGINES.append(engine)
+    return result
 
 
 def db_get_engines() -> list[str]:
     """
-    Return the list of configured engines.
+    Retrieve and return the list of configured engines.
 
     This list may include any of the supported engines:
      *mysql*, *oracle*, *postgres*, *sqlserver*.
 
-    :return: the list of configure engines
+    :return: the list of configured engines
     """
     return _DB_ENGINES
 
 
 def db_get_params(engine: str = None) -> dict:
     """
     The connection parameters are returned as a *dict*, with the keys:
     *name*, *user*, *pwd*, *host*, *port*.
-
     The meaning of these parameters may vary between different database engines.
 
     :param engine: the database engine
     :return: the current connection parameters for the engine
     """
     return _DB_CONN_DATA.get(engine or _DB_ENGINES[0])
 
 
 def db_connect(errors: list[str] | None,
                engine: str = None,
                logger: Logger = None) -> Any:
     """
     Obtain and return a connection to the database, or *None* if the connection cannot be obtained.
+    The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param logger: optional logger
     :return: the connection to the database
     """
     # initialize the return variable
@@ -104,14 +120,15 @@
               engine: str = None,
               logger: Logger = None) -> bool:
     """
     Determine whether the table *table* in the database contains at least one tuple.
 
     For this determination, *where_attrs* are made equal to *where_values* in the query, respectively.
     If more than one, the attributes are concatenated by the *AND* logical connector.
+    The targer database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param table: the table to be searched
     :param where_attrs: the search attributes
     :param where_vals: the values for the search attributes
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param logger: optional logger
@@ -140,14 +157,15 @@
                   logger: Logger = None) -> tuple:
     """
     Search the database and return the first tuple that satisfies the *sel_stmt* search command.
 
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
     in a specific tuple. In case of error, or if the search is empty, *None* is returned.
+    The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: values to be associated with the search criteria
     :param require_nonempty: defines whether an empty search should be considered an error
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param logger: optional logger
@@ -175,90 +193,96 @@
     """
     Search the database and return all tuples that satisfy the *sel_stmt* search command.
 
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
     in a specific tuple. If not positive integers, *require_min* and *require_max* are ignored.
     If the search is empty, an empty list is returned.
+    The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: the values to be associated with the search criteria
     :param require_min: optionally defines the minimum number of tuples to be returned
     :param require_max: optionally defines the maximum number of tuples to be returned
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param logger: optional logger
     :return: list of tuples containing the search result, or [] if the search is empty
     """
     # initialize the return variable
     result: list[tuple] | None = None
 
-    curr_engine: str = engine or _DB_ENGINES[0]
-    if curr_engine == "mysql":
-        pass
-    elif curr_engine == "oracle":
-        from . import oracle_pomes
-        result = oracle_pomes.db_select_all(errors, sel_stmt, where_vals,
-                                            require_min, require_max,  logger)
-    elif curr_engine == "postgres":
-        from . import postgres_pomes
-        result = postgres_pomes.db_select_all(errors, sel_stmt, where_vals,
-                                              require_min, require_max, logger)
-    elif curr_engine == "sqlserver":
-        from . import sqlserver_pomes
-        result = sqlserver_pomes.db_select_all(errors, sel_stmt, where_vals,
-                                               require_min, require_max, logger)
+    curr_engine: str = _DB_ENGINES[0] if not engine and _DB_ENGINES else engine
+    if curr_engine in _DB_ENGINES:
+        if curr_engine == "mysql":
+            pass
+        elif curr_engine == "oracle":
+            from . import oracle_pomes
+            result = oracle_pomes.db_select_all(errors, sel_stmt, where_vals,
+                                                require_min, require_max,  logger)
+        elif curr_engine == "postgres":
+            from . import postgres_pomes
+            result = postgres_pomes.db_select_all(errors, sel_stmt, where_vals,
+                                                  require_min, require_max, logger)
+        elif curr_engine == "sqlserver":
+            from . import sqlserver_pomes
+            result = sqlserver_pomes.db_select_all(errors, sel_stmt, where_vals,
+                                                   require_min, require_max, logger)
 
     return result
 
 
 def db_modify(errors: list[str] | None,
               modify_stmt: str,
               bind_vals: tuple,
               engine: str = None,
               logger: Logger = None) -> int:
     """
     Modify the database, inserting, updating or deleting tuples, according to *modify_stmt* definitions.
 
     The values for this modification, followed by the values for selecting tuples are in *bind_vals*.
+    The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param modify_stmt: INSERT, UPDATE, or DELETE statement
     :param bind_vals: values for database modification, and for tuples selection
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param logger: optional logger
     :return: the number of inserted, modified, or deleted tuples, ou None if an error occurred
     """
     # initialize the return variable
     result: int | None = None
 
-    curr_engine: str = engine or _DB_ENGINES[0]
-    if curr_engine == "mysql":
-        pass
-    elif curr_engine == "oracle":
-        from . import oracle_pomes
-        result = oracle_pomes.db_modify(errors, modify_stmt, bind_vals, logger)
-    elif curr_engine == "postgres":
-        from . import postgres_pomes
-        result = postgres_pomes.db_modify(errors, modify_stmt, bind_vals, logger)
-    elif curr_engine == "sqlserver":
-        from . import sqlserver_pomes
-        result = sqlserver_pomes.db_modify(errors, modify_stmt, bind_vals, logger)
+    curr_engine: str = _DB_ENGINES[0] if not engine and _DB_ENGINES else engine
+    if curr_engine in _DB_ENGINES:
+        if curr_engine == "mysql":
+            pass
+        elif curr_engine == "oracle":
+            from . import oracle_pomes
+            result = oracle_pomes.db_modify(errors, modify_stmt, bind_vals, logger)
+        elif curr_engine == "postgres":
+            from . import postgres_pomes
+            result = postgres_pomes.db_modify(errors, modify_stmt, bind_vals, logger)
+        elif curr_engine == "sqlserver":
+            from . import sqlserver_pomes
+            result = sqlserver_pomes.db_modify(errors, modify_stmt, bind_vals, logger)
 
     return result
 
 
 def db_insert(errors: list[str] | None,
               insert_stmt: str,
               insert_vals: tuple,
               engine: str = None,
               logger: Logger = None) -> int:
     """
     Insert a tuple, with values defined in *insert_vals*, into the database.
 
+    The target database engine, default or specified, must have been previously configured.
+
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the values to be inserted
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param logger: optional logger
     :return: the number of inserted tuples (0 ou 1), or None if an error occurred
     """
@@ -272,14 +296,15 @@
               engine: str = None,
               logger: Logger = None) -> int:
     """
     Update one or more tuples in the database, as defined by the command *update_stmt*.
 
     The values for this update are in *update_vals*.
     The values for selecting the tuples to be updated are in *where_vals*.
+    The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param update_stmt: the UPDATE command
     :param update_vals: the values for the update operation
     :param where_vals: the values to be associated with the search criteria
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param logger: optional logger
@@ -293,14 +318,15 @@
               where_vals: tuple,
               engine: str = None,
               logger: Logger = None) -> int:
     """
     Delete one or more tuples in the database, as defined by the *delete_stmt* command.
 
     The values for selecting the tuples to be deleted are in *where_vals*.
+    The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param delete_stmt: the DELETE command
     :param where_vals: the values to be associated with the search criteria
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param logger: optional logger
     :return: the number of deleted tuples, or None if an error occurred
@@ -312,99 +338,108 @@
                    insert_stmt: str,
                    insert_vals: list[tuple],
                    engine: str = None,
                    logger: Logger = None) -> int:
     """
     Insert the tuples, with values defined in *insert_vals*, into the database.
 
+    The target database engine, default or specified, must have been previously configured.
+
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the list of values to be inserted
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param logger: optional logger
     :return: the number of inserted tuples, or None if an error occurred
     """
     # initialize the return variable
     result: int | None = None
 
-    curr_engine: str = engine or _DB_ENGINES[0]
-    if curr_engine == "mysql":
-        pass
-    elif curr_engine == "oracle":
-        from . import oracle_pomes
-        result = oracle_pomes.db_bulk_insert(errors, insert_stmt, insert_vals, logger)
-    elif curr_engine == "postgres":
-        from . import postgres_pomes
-        result = postgres_pomes.db_bulk_insert(errors, insert_stmt, insert_vals, logger)
-    elif curr_engine == "sqlserver":
-        from . import sqlserver_pomes
-        result = sqlserver_pomes.db_bulk_insert(errors, insert_stmt, insert_vals, logger)
+    curr_engine: str = _DB_ENGINES[0] if not engine and _DB_ENGINES else engine
+    if curr_engine in _DB_ENGINES:
+        if curr_engine == "mysql":
+            pass
+        elif curr_engine == "oracle":
+            from . import oracle_pomes
+            result = oracle_pomes.db_bulk_insert(errors, insert_stmt, insert_vals, logger)
+        elif curr_engine == "postgres":
+            from . import postgres_pomes
+            result = postgres_pomes.db_bulk_insert(errors, insert_stmt, insert_vals, logger)
+        elif curr_engine == "sqlserver":
+            from . import sqlserver_pomes
+            result = sqlserver_pomes.db_bulk_insert(errors, insert_stmt, insert_vals, logger)
 
     return result
 
 
 def db_call_function(errors: list[str] | None,
                      func_name: str,
                      func_vals: tuple,
                      engine: str = None,
                      logger: Logger = None) -> list[tuple]:
     """
     Execute the stored function *func_name* in the database, with the parameters given in *func_vals*.
 
+    The target database engine, default or specified, must have been previously configured.
+
     :param errors: incidental error messages
     :param func_name: name of the stored function
     :param func_vals: parameters for the stored function
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param logger: optional logger
     :return: the data returned by the function
     """
     # initialize the return variable
     result: Any = None
 
-    curr_engine: str = engine or _DB_ENGINES[0]
-    if curr_engine == "mysql":
-        pass
-    elif curr_engine == "oracle":
-        from . import oracle_pomes
-        result = oracle_pomes.db_call_function(errors, func_name, func_vals, logger)
-    elif curr_engine == "postgres":
-        from . import postgres_pomes
-        result = postgres_pomes.db_call_procedure(errors, func_name, func_vals, logger)
-    elif curr_engine == "sqlserver":
-        from . import sqlserver_pomes
-        result = sqlserver_pomes.db_call_procedure(errors, func_name, func_vals, logger)
+    curr_engine: str = _DB_ENGINES[0] if not engine and _DB_ENGINES else engine
+    if curr_engine in _DB_ENGINES:
+        if curr_engine == "mysql":
+            pass
+        elif curr_engine == "oracle":
+            from . import oracle_pomes
+            result = oracle_pomes.db_call_function(errors, func_name, func_vals, logger)
+        elif curr_engine == "postgres":
+            from . import postgres_pomes
+            result = postgres_pomes.db_call_procedure(errors, func_name, func_vals, logger)
+        elif curr_engine == "sqlserver":
+            from . import sqlserver_pomes
+            result = sqlserver_pomes.db_call_procedure(errors, func_name, func_vals, logger)
 
     return result
 
 
 def db_call_procedure(errors: list[str] | None,
                       proc_name: str,
                       proc_vals: tuple,
                       engine: str = None,
                       logger: Logger = None) -> list[tuple]:
     """
     Execute the stored procedure *proc_name* in the database, with the parameters given in *proc_vals*.
 
+    The target database engine, default or specified, must have been previously configured.
+
     :param errors: incidental error messages
     :param proc_name: name of the stored procedure
     :param proc_vals: parameters for the stored procedure
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param logger: optional logger
     :return: the data returned by the procedure
     """
     # initialize the return variable
     result: Any = None
 
-    curr_engine: str = engine or _DB_ENGINES[0]
-    if curr_engine == "mysql":
-        pass
-    elif curr_engine == "oracle":
-        from . import oracle_pomes
-        result = oracle_pomes.db_call_procedure(errors, proc_name, proc_vals, logger)
-    elif curr_engine == "postgres":
-        from . import postgres_pomes
-        result = postgres_pomes.db_call_procedure(errors, proc_name, proc_vals, logger)
-    elif curr_engine == "sqlserver":
-        from . import sqlserver_pomes
-        result = sqlserver_pomes.db_call_procedure(errors, proc_name, proc_vals, logger)
+    curr_engine: str = _DB_ENGINES[0] if not engine and _DB_ENGINES else engine
+    if curr_engine in _DB_ENGINES:
+        if curr_engine == "mysql":
+            pass
+        elif curr_engine == "oracle":
+            from . import oracle_pomes
+            result = oracle_pomes.db_call_procedure(errors, proc_name, proc_vals, logger)
+        elif curr_engine == "postgres":
+            from . import postgres_pomes
+            result = postgres_pomes.db_call_procedure(errors, proc_name, proc_vals, logger)
+        elif curr_engine == "sqlserver":
+            from . import sqlserver_pomes
+            result = sqlserver_pomes.db_call_procedure(errors, proc_name, proc_vals, logger)
 
     return result
```

### Comparing `pypomes_db-0.4.1/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.4.2/src/pypomes_db/oracle_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.1/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.4.2/src/pypomes_db/postgres_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.1/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.4.2/src/pypomes_db/sqlserver_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.1/LICENSE` & `pypomes_db-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.1/pyproject.toml` & `pypomes_db-0.4.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.4.1"
+version = "0.4.2"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.4.1/PKG-INFO` & `pypomes_db-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.4.1
+Version: 0.4.2
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

