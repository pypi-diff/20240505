# Comparing `tmp/pypomes_db-0.4.4.tar.gz` & `tmp/pypomes_db-0.4.5.tar.gz`

## Comparing `pypomes_db-0.4.4.tar` & `pypomes_db-0.4.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 pypomes_db-0.4.4/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 pypomes_db-0.4.4/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    19562 2020-02-02 00:00:00.000000 pypomes_db-0.4.4/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.4/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    12106 2020-02-02 00:00:00.000000 pypomes_db-0.4.4/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    10232 2020-02-02 00:00:00.000000 pypomes_db-0.4.4/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    10351 2020-02-02 00:00:00.000000 pypomes_db-0.4.4/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.4.4/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.4.4/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.4/README.md
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pypomes_db-0.4.4/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 pypomes_db-0.4.5/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 pypomes_db-0.4.5/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    19681 2020-02-02 00:00:00.000000 pypomes_db-0.4.5/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.5/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    12254 2020-02-02 00:00:00.000000 pypomes_db-0.4.5/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    10382 2020-02-02 00:00:00.000000 pypomes_db-0.4.5/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    10501 2020-02-02 00:00:00.000000 pypomes_db-0.4.5/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.4.5/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.4.5/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.5/README.md
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pypomes_db-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.4.5/PKG-INFO
```

### Comparing `pypomes_db-0.4.4/src/pypomes_db/__init__.py` & `pypomes_db-0.4.5/src/pypomes_db/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from .db_pomes import (
     db_setup, db_get_engines, db_get_params,
     db_assert_connection, db_connect, db_exists,
     db_select_one, db_select_all, db_update,
     db_delete, db_insert, db_bulk_insert,
-    db_call_function, db_call_procedure,
+    db_execute, db_call_function, db_call_procedure,
 )
 
 __all__ = [
     # db_pomes
     "db_setup", "db_get_engines", "db_get_params",
     "db_assert_connection", "db_connect", "db_exists",
     "db_select_one", "db_select_all", "db_update",
     "db_delete", "db_insert", "db_bulk_insert",
-    "db_call_function", "db_call_procedure",
+    "db_execute", "db_call_function", "db_call_procedure",
 ]
 
 from importlib.metadata import version
 __version__ = version("pypomes_db")
 __version_info__ = tuple(int(i) for i in __version__.split(".") if i.isdigit())
```

### Comparing `pypomes_db-0.4.4/src/pypomes_db/db_common.py` & `pypomes_db-0.4.5/src/pypomes_db/db_common.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.4/src/pypomes_db/db_pomes.py` & `pypomes_db-0.4.5/src/pypomes_db/db_pomes.py`

 * *Files 4% similar despite different names*

```diff
@@ -276,15 +276,15 @@
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the values to be inserted
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param logger: optional logger
     :return: the number of inserted tuples (0 ou 1), or None if an error occurred
     """
-    return _db_modify(errors, insert_stmt, insert_vals, engine, logger)
+    return db_execute(errors, insert_stmt, insert_vals, engine, logger)
 
 
 def db_update(errors: list[str] | None,
               update_stmt: str,
               update_vals: tuple,
               where_vals: tuple,
               engine: str = None,
@@ -300,15 +300,15 @@
     :param update_stmt: the UPDATE command
     :param update_vals: the values for the update operation
     :param where_vals: the values to be associated with the search criteria
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param logger: optional logger
     :return: the number of updated tuples, or None if an error occurred
     """
-    return _db_modify(errors, update_stmt, update_vals + where_vals, engine, logger)
+    return db_execute(errors, update_stmt, update_vals + where_vals, engine, logger)
 
 
 def db_delete(errors: list[str] | None,
               delete_stmt: str,
               where_vals: tuple,
               engine: str = None,
               logger: Logger = None) -> int:
@@ -321,15 +321,15 @@
     :param errors: incidental error messages
     :param delete_stmt: the DELETE command
     :param where_vals: the values to be associated with the search criteria
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param logger: optional logger
     :return: the number of deleted tuples, or None if an error occurred
     """
-    return _db_modify(errors, delete_stmt, where_vals, engine, logger)
+    return db_execute(errors, delete_stmt, where_vals, engine, logger)
 
 
 def db_bulk_insert(errors: list[str] | None,
                    insert_stmt: str,
                    insert_vals: list[tuple],
                    engine: str = None,
                    logger: Logger = None) -> int:
@@ -360,14 +360,56 @@
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
         result = sqlserver_pomes.db_bulk_insert(errors, insert_stmt, insert_vals, logger)
 
     return result
 
 
+def db_execute(errors: list[str] | None,
+               exc_stmt: str,
+               bind_vals: tuple | None,
+               engine: str = None,
+               logger: Logger = None) -> int:
+    """
+    Execute the command *exc_stmt* on the database.
+
+    This command might be a DML ccommand modifying the database, such as
+    inserting, updating or deleting tuples, or it might be a DDL statement,
+    or it might even be an environment-related command.
+    The optional bind values for this operation are in *bind_vals*.
+    The value returned is the value obtained from the execution of *exc_stmt*.
+    It might be the number of inserted, modified, or deleted tuples,
+    ou None if an error occurred.
+
+    :param errors: incidental error messages
+    :param exc_stmt: the command to execute
+    :param bind_vals: optional bind values
+    :param engine: the database engine to use (uses the default engine, if not specified)
+    :param logger: optional logger
+    :return: the return value from the command execution
+    """
+    # initialize the return variable
+    result: int | None = None
+
+    curr_engine: str = _assert_engine(errors, engine)
+    if curr_engine == "mysql":
+        pass
+    elif curr_engine == "oracle":
+        from . import oracle_pomes
+        result = oracle_pomes.db_execute(errors, exc_stmt, bind_vals, logger)
+    elif curr_engine == "postgres":
+        from . import postgres_pomes
+        result = postgres_pomes.db_execute(errors, exc_stmt, bind_vals, logger)
+    elif curr_engine == "sqlserver":
+        from . import sqlserver_pomes
+        result = sqlserver_pomes.db_execute(errors, exc_stmt, bind_vals, logger)
+
+    return result
+
+
 def db_call_function(errors: list[str] | None,
                      func_name: str,
                      func_vals: tuple,
                      engine: str = None,
                      logger: Logger = None) -> list[tuple]:
     """
     Execute the stored function *func_name* in the database, with the parameters given in *func_vals*.
@@ -430,44 +472,7 @@
         from . import postgres_pomes
         result = postgres_pomes.db_call_procedure(errors, proc_name, proc_vals, logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
         result = sqlserver_pomes.db_call_procedure(errors, proc_name, proc_vals, logger)
 
     return result
-
-
-def _db_modify(errors: list[str] | None,
-               modify_stmt: str,
-               bind_vals: tuple,
-               engine: str = None,
-               logger: Logger = None) -> int:
-    """
-    Modify the database, inserting, updating or deleting tuples, according to *modify_stmt* definitions.
-
-    The values for this modification, followed by the values for selecting tuples are in *bind_vals*.
-    The target database engine, default or specified, must have been previously configured.
-
-    :param errors: incidental error messages
-    :param modify_stmt: INSERT, UPDATE, or DELETE statement
-    :param bind_vals: values for database modification, and for tuples selection
-    :param engine: the database engine to use (uses the default engine, if not specified)
-    :param logger: optional logger
-    :return: the number of inserted, modified, or deleted tuples, ou None if an error occurred
-    """
-    # initialize the return variable
-    result: int | None = None
-
-    curr_engine: str = _assert_engine(errors, engine)
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
-
-    return result
```

### Comparing `pypomes_db-0.4.4/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.4.5/src/pypomes_db/oracle_pomes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from logging import Logger
 from oracledb import Connection, connect, init_oracle_client
 
 from .db_common import (
-    _DB_CONN_DATA, _assert_query_quota, _db_get_params, _db_log, _db_except_msg
+    _DB_CONN_DATA,
+    _assert_query_quota, _db_get_params, _db_log, _db_except_msg
 )
 
 # TODO: db_call_function, db_call_procedure
 
 
 def db_connect(errors: list[str],
                logger: Logger = None) -> Connection:
@@ -40,15 +41,15 @@
             err_msg=err_msg,
             logger=logger,
             query_stmt=f"Connecting to '{name}' at '{host}'")
 
     return result
 
 
-def db_select_all(errors: list[str] | None,
+def db_select_all(errors: list[str],
                   sel_stmt: str,
                   where_vals: tuple = None,
                   require_min: int = None,
                   require_max: int = None,
                   logger: Logger = None) -> list[tuple]:
     """
     Search the database and return all tuples that satisfy the *sel_stmt* search command.
@@ -116,15 +117,15 @@
             logger=logger,
             query_stmt=sel_stmt,
             bind_vals=where_vals)
 
     return result
 
 
-def db_bulk_insert(errors: list[str] | None,
+def db_bulk_insert(errors: list[str],
                    insert_stmt: str,
                    insert_vals: list[tuple],
                    logger: Logger = None) -> int:
     """
     Insert the tuples, with values defined in *insert_vals*, into the database.
 
     :param errors: incidental error messages
@@ -170,17 +171,75 @@
             logger=logger,
             query_stmt=insert_stmt,
             bind_vals=insert_vals[0])
 
     return result
 
 
+def db_execute(errors: list[str],
+               exc_stmt: str,
+               bind_vals: tuple,
+               logger: Logger) -> int:
+    """
+    Execute the command *exc_stmt* on the database.
+
+    This command might be a DML ccommand modifying the database, such as
+    inserting, updating or deleting tuples, or it might be a DDL statement,
+    or it might even be an environment-related command.
+    The optional bind values for this operation are in *bind_vals*.
+    The value returned is the value obtained from the execution of *exc_stmt*.
+    It might be the number of inserted, modified, or deleted tuples,
+    ou None if an error occurred.
+
+    :param errors: incidental error messages
+    :param exc_stmt: the command to execute
+    :param bind_vals: optional bind values
+    :param logger: optional logger
+    :return: the return value from the command execution
+    """
+    # initialize the return variable
+    result: int | None = None
+
+    # retrieve the connection parameters
+    name, user, pwd, host, port = _db_get_params("oracle")
+
+    err_msg: str | None = None
+    try:
+        # obtain a connection
+        with  connect(service_name=name,
+                      host=host,
+                      port=port,
+                      user=user,
+                      password=pwd) as conn:
+            # make sure the connection is not in autocommit mode
+            conn.autocommit = False
+            # obtain the cursor and execute the operation
+            with conn.cursor() as cursor:
+                cursor.execute(statement=exc_stmt,
+                               parameters=bind_vals)
+                result = cursor.rowcount
+            # commit the transaction
+            conn.commit()
+    except Exception as e:
+        err_msg = _db_except_msg(exception=e,
+                                 engine="oracle")
+
+    # log the results
+    _db_log(errors=errors,
+            err_msg=err_msg,
+            logger=logger,
+            query_stmt=exc_stmt,
+            bind_vals=bind_vals)
+
+    return result
+
+
 # TODO: see https://python-oracledb.readthedocs.io/en/latest/user_guide/plsql_execution.html
 # noinspection PyUnusedLocal
-def db_call_function(errors: list[str] | None,
+def db_call_function(errors: list[str],
                      func_name: str,
                      func_vals: tuple,
                      logger: Logger = None) -> list[tuple]:
     """
     Execute the stored function *func_name* in the database, with the parameters given in *func_vals*.
 
     :param errors: incidental error messages
@@ -192,15 +251,15 @@
     # initialize the return variable
     result: list[tuple] = []
 
     return result
 
 
 # TODO: see https://python-oracledb.readthedocs.io/en/latest/user_guide/plsql_execution.html
-def db_call_procedure(errors: list[str] | None,
+def db_call_procedure(errors: list[str],
                       proc_name: str,
                       proc_vals: tuple,
                       logger: Logger = None) -> list[tuple]:
     """
     Execute the stored procedure *proc_name* in the database, with the parameters given in *proc_vals*.
 
     :param errors: incidental error messages
@@ -245,69 +304,17 @@
             err_msg=err_msg,
             logger=logger,
             query_stmt=proc_name,
             bind_vals=proc_vals)
 
     return result
 
-
-def db_modify(errors: list[str] | None,
-              modify_stmt: str,
-              bind_vals: tuple | list[tuple],
-              logger: Logger) -> int:
-    """
-    Modify the database, inserting, updating or deleting tuples, according to the *modify_stmt* command definitions.
-
-    The values for this modification, followed by the values for selecting tuples are in *bind_vals*.
-
-    :param errors: incidental error messages
-    :param modify_stmt: INSERT, UPDATE, or DELETE command
-    :param bind_vals: values for database modification, and for tuples selection
-    :param logger: optional logger
-    :return: the number of inserted, modified, or deleted tuples, ou None if an error occurred
-    """
-    # initialize the return variable
-    result: int | None = None
-
-    # retrieve the connection parameters
-    name, user, pwd, host, port = _db_get_params("oracle")
-
-    err_msg: str | None = None
-    try:
-        # obtain a connection
-        with  connect(service_name=name,
-                      host=host,
-                      port=port,
-                      user=user,
-                      password=pwd) as conn:
-            # make sure the connection is not in autocommit mode
-            conn.autocommit = False
-            # obtain the cursor and execute the operation
-            with conn.cursor() as cursor:
-                cursor.execute(statement=modify_stmt,
-                               parameters=bind_vals)
-                result = cursor.rowcount
-            # commit the transaction
-            conn.commit()
-    except Exception as e:
-        err_msg = _db_except_msg(exception=e,
-                                 engine="oracle")
-
-    # log the results
-    _db_log(errors=errors,
-            err_msg=err_msg,
-            logger=logger,
-            query_stmt=modify_stmt,
-            bind_vals=bind_vals)
-
-    return result
-
 __is_initialized: str | None = None
 
-def _initialize(errors: list[str] | None,
+def _initialize(errors: list[str],
                 logger: Logger) -> bool:
     """
     Setup the oracle engine to access the database throught the installed client software.
 
     :param errors: incidental error messages
     :param logger: optional logger
     :return: False if an error happened, True otherwise
```

### Comparing `pypomes_db-0.4.4/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.4.5/src/pypomes_db/postgres_pomes.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from psycopg2._psycopg import connection
 
 from .db_common import (
     _assert_query_quota, _db_get_params, _db_log, _db_except_msg
 )
 
 
-def db_connect(errors: list[str] | None,
+def db_connect(errors: list[str],
                logger: Logger = None) -> connection:
     """
     Obtain and return a connection to the database, or *None* if the connection could not be obtained.
 
     :param errors: incidental error messages
     :param logger: optional logger
     :return: the connection to the database
@@ -40,15 +40,15 @@
             err_msg=err_msg,
             logger=logger,
             query_stmt=f"Connecting to '{name}' at '{host}'")
 
     return result
 
 
-def db_select_all(errors: list[str] | None,
+def db_select_all(errors: list[str],
                   sel_stmt: str,
                   where_vals: tuple = None,
                   require_min: int = None,
                   require_max: int = None,
                   logger: Logger = None) -> list[tuple]:
     """
     Search the database and return all tuples that satisfy the *sel_stmt* search command.
@@ -115,15 +115,15 @@
             logger=logger,
             query_stmt=sel_stmt,
             bind_vals=where_vals)
 
     return result
 
 
-def db_bulk_insert(errors: list[str] | None,
+def db_bulk_insert(errors: list[str],
                    insert_stmt: str,
                    insert_vals: list[tuple],
                    logger: Logger = None) -> int:
     """
     Insert the tuples, with values defined in *insert_vals*, into the database.
 
     The *VALUES* clause in *insert_stmt* must be simply *VALUES %s*.
@@ -170,113 +170,119 @@
             err_msg=err_msg,
             logger=logger,
             query_stmt=insert_stmt)
 
     return result
 
 
-def db_call_procedure(errors: list[str] | None,
-                      proc_name: str,
-                      proc_vals: tuple,
-                      logger: Logger = None) -> list[tuple]:
+def db_execute(errors: list[str],
+               exc_stmt: str,
+               bind_vals: tuple,
+               logger: Logger) -> int:
     """
-    Execute the stored procedure *proc_name*, with the arguments given in *proc_vals*.
+    Execute the command *exc_stmt* on the database.
 
-    :param errors:  incidental error messages
-    :param proc_name: the name of the sotred procedure
-    :param proc_vals: the arguments to be passed
+    This command might be a DML ccommand modifying the database, such as
+    inserting, updating or deleting tuples, or it might be a DDL statement,
+    or it might even be an environment-related command.
+    The optional bind values for this operation are in *bind_vals*.
+    The value returned is the value obtained from the execution of *exc_stmt*.
+    It might be the number of inserted, modified, or deleted tuples,
+    ou None if an error occurred.
+
+    :param errors: incidental error messages
+    :param exc_stmt: the command to execute
+    :param bind_vals: optional bind values
     :param logger: optional logger
-    :return: the data returned by the procedure
+    :return: the return value from the command execution
     """
     # initialize the return variable
-    result: list[tuple] = [()]
+    result: int | None = None
 
     # retrieve the connection parameters
     name, user, pwd, host, port = _db_get_params("postgres")
 
-    # build the command
-    proc_stmt: str = f"{proc_name}(" + "%s, " * (len(proc_vals) - 1) + "%s)"
-
-    # execute the stored procedure
     err_msg: str | None = None
     try:
         # obtain a connection
         with connect(host=host,
                      port=port,
                      database=name,
                      user=user,
                      password=pwd) as conn:
             # make sure the connection is not in autocommit mode
             conn.autocommit = False
-
-            # obtain a cursor and perform the operation
+            # obtain the cursor and execute the operation
             with conn.cursor() as cursor:
-                cursor.execute(query=proc_stmt,
-                               argslist=proc_vals)
-                # retrieve the returned tuples
-                result = list(cursor)
+                cursor.execute(query=f"{exc_stmt};",
+                               vars=bind_vals)
+                result = cursor.rowcount
             # commit the transaction
             conn.commit()
     except Exception as e:
         err_msg = _db_except_msg(exception=e,
                                  engine="postgres")
 
     # log the results
     _db_log(errors=errors,
             err_msg=err_msg,
             logger=logger,
-            query_stmt=proc_stmt,
-            bind_vals=proc_vals)
+            query_stmt=exc_stmt,
+            bind_vals=bind_vals)
 
     return result
 
 
-def db_modify(errors: list[str] | None,
-              modify_stmt: str,
-              bind_vals: tuple | list[tuple],
-              logger: Logger) -> int:
+def db_call_procedure(errors: list[str],
+                      proc_name: str,
+                      proc_vals: tuple,
+                      logger: Logger = None) -> list[tuple]:
     """
-    Modify the database, inserting, updating or deleting tuples, according to the *modify_stmt* command definitions.
-
-    The values for this modification, followed by the values for selecting tuples are in *bind_vals*.
+    Execute the stored procedure *proc_name*, with the arguments given in *proc_vals*.
 
-    :param errors: incidental error messages
-    :param modify_stmt: INSERT, UPDATE, or DELETE command
-    :param bind_vals: values for database modification, and for tuples selection
+    :param errors:  incidental error messages
+    :param proc_name: the name of the sotred procedure
+    :param proc_vals: the arguments to be passed
     :param logger: optional logger
-    :return: the number of inserted, modified, or deleted tuples, ou None if an error occurred
+    :return: the data returned by the procedure
     """
     # initialize the return variable
-    result: int | None = None
+    result: list[tuple] = [()]
 
     # retrieve the connection parameters
     name, user, pwd, host, port = _db_get_params("postgres")
 
+    # build the command
+    proc_stmt: str = f"{proc_name}(" + "%s, " * (len(proc_vals) - 1) + "%s)"
+
+    # execute the stored procedure
     err_msg: str | None = None
     try:
         # obtain a connection
         with connect(host=host,
                      port=port,
                      database=name,
                      user=user,
                      password=pwd) as conn:
             # make sure the connection is not in autocommit mode
             conn.autocommit = False
-            # obtain the cursor and execute the operation
+
+            # obtain a cursor and perform the operation
             with conn.cursor() as cursor:
-                cursor.execute(query=f"{modify_stmt};",
-                               vars=bind_vals)
-                result = cursor.rowcount
+                cursor.execute(query=proc_stmt,
+                               argslist=proc_vals)
+                # retrieve the returned tuples
+                result = list(cursor)
             # commit the transaction
             conn.commit()
     except Exception as e:
         err_msg = _db_except_msg(exception=e,
                                  engine="postgres")
 
     # log the results
     _db_log(errors=errors,
             err_msg=err_msg,
             logger=logger,
-            query_stmt=modify_stmt,
-            bind_vals=bind_vals)
+            query_stmt=proc_stmt,
+            bind_vals=proc_vals)
 
     return result
```

### Comparing `pypomes_db-0.4.4/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.4.5/src/pypomes_db/sqlserver_pomes.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pyodbc import connect, Connection, Row
 
 from .db_common import (
     _assert_query_quota, _db_get_params, _db_log, _db_except_msg
 )
 
 
-def db_connect(errors: list[str] | None,
+def db_connect(errors: list[str],
                logger: Logger = None) -> Connection:
     """
     Obtain and return a connection to the database, or *None* if the connection could not be obtained.
 
     :param errors: incidental error messages
     :param logger: optional logger
     :return: the connection to the database
@@ -35,15 +35,15 @@
             err_msg=err_msg,
             logger=logger,
             query_stmt=f"Connecting to '{name}' at '{host}'")
 
     return result
 
 
-def db_select_all(errors: list[str] | None,
+def db_select_all(errors: list[str],
                   sel_stmt: str,
                   where_vals: tuple = None,
                   require_min: int = None,
                   require_max: int = None,
                   logger: Logger = None) -> list[tuple]:
     """
     Search the database and return all tuples that satisfy the *sel_stmt* search command.
@@ -105,15 +105,15 @@
             logger=logger,
             query_stmt=sel_stmt,
             bind_vals=where_vals)
 
     return result
 
 
-def db_bulk_insert(errors: list[str] | None,
+def db_bulk_insert(errors: list[str],
                    insert_stmt: str,
                    insert_vals: list[tuple],
                    logger: Logger = None) -> int:
     """
     Insert the tuples, with values defined in *insert_vals*, into the database.
 
     :param errors: incidental error messages
@@ -155,119 +155,125 @@
             logger=logger,
             query_stmt=insert_stmt,
             bind_vals=insert_vals[0])
 
     return result
 
 
-def db_call_procedure(errors: list[str] | None,
-                      proc_name: str,
-                      proc_vals: tuple,
-                      require_min: int = None,
-                      require_max: int = None,
-                      logger: Logger = None) -> list[tuple]:
+def db_execute(errors: list[str],
+               exc_stmt: str,
+               bind_vals: tuple,
+               logger: Logger) -> int:
     """
-    Execute the stored procedure *proc_name* in the database, with the parameters given in *proc_vals*.
+    Execute the command *exc_stmt* on the database.
+
+    This command might be a DML ccommand modifying the database, such as
+    inserting, updating or deleting tuples, or it might be a DDL statement,
+    or it might even be an environment-related command.
+    The optional bind values for this operation are in *bind_vals*.
+    The value returned is the value obtained from the execution of *exc_stmt*.
+    It might be the number of inserted, modified, or deleted tuples,
+    ou None if an error occurred.
 
     :param errors: incidental error messages
-    :param proc_name: name of the stored procedure
-    :param proc_vals: parameters for the stored procedure
-    :param require_min: optionally defines the minimum number of tuples to be returned
-    :param require_max: optionally defines the maximum number of tuples to be returned
+    :param exc_stmt: the command to execute
+    :param bind_vals: optional bind values
     :param logger: optional logger
-    :return: the data returned by the procedure
+    :return: the return value from the command execution
     """
     # initialize the return variable
-    result: list[tuple] | None = None
+    result: int | None = None
 
     # obtain the connection string
     connection_kwargs: str = _get_connection_kwargs()
 
-    # build the command
-    proc_stmt: str | None = None
-
-    # execute the stored procedure
     err_msg: str | None = None
     try:
         # obtain a connection
         with connect(connection_kwargs) as conn:
             # make sure the connection is not in autocommit mode
             conn.autocommit = False
             # obtain the cursor and execute the operation
             with conn.cursor() as cursor:
-                proc_stmt = f"SET NOCOUNT ON; EXEC {proc_name} {','.join(('?',) * len(proc_vals))}"
-                cursor.execute(proc_stmt, proc_vals)
-                # obtain the number of tuples returned
-                count: int = cursor.rowcount
-
-                # has the query quota been satisfied ?
-                # noinspection PyTypeChecker
-                if _assert_query_quota(errors, proc_name, None, count, require_min, require_max):
-                    # yes, retrieve the returned tuples
-                    rows: list[Row] = cursor.fetchall()
-                    result = [tuple(row) for row in rows]
+                cursor.execute(exc_stmt, bind_vals)
+                result = cursor.rowcount
             # commit the transaction
             conn.commit()
     except Exception as e:
         err_msg = _db_except_msg(exception=e,
                                  engine="sqlserver")
 
     # log the results
     _db_log(errors=errors,
             err_msg=err_msg,
             logger=logger,
-            query_stmt=proc_stmt,
-            bind_vals=proc_vals)
+            query_stmt=exc_stmt,
+            bind_vals=bind_vals)
 
     return result
 
 
-def db_modify(errors: list[str] | None,
-              modify_stmt: str,
-              bind_vals: tuple | list[tuple],
-              logger: Logger) -> int:
+def db_call_procedure(errors: list[str],
+                      proc_name: str,
+                      proc_vals: tuple,
+                      require_min: int = None,
+                      require_max: int = None,
+                      logger: Logger = None) -> list[tuple]:
     """
-    Modify the database, inserting, updating or deleting tuples, according to the *modify_stmt* command definitions.
-
-    The values for this modification, followed by the values for selecting tuples are in *bind_vals*.
+    Execute the stored procedure *proc_name* in the database, with the parameters given in *proc_vals*.
 
     :param errors: incidental error messages
-    :param modify_stmt: INSERT, UPDATE, or DELETE command
-    :param bind_vals: values for database modification, and for tuples selection
+    :param proc_name: name of the stored procedure
+    :param proc_vals: parameters for the stored procedure
+    :param require_min: optionally defines the minimum number of tuples to be returned
+    :param require_max: optionally defines the maximum number of tuples to be returned
     :param logger: optional logger
-    :return: the number of inserted, modified, or deleted tuples, ou None if an error occurred
+    :return: the data returned by the procedure
     """
     # initialize the return variable
-    result: int | None = None
+    result: list[tuple] | None = None
 
     # obtain the connection string
     connection_kwargs: str = _get_connection_kwargs()
 
+    # build the command
+    proc_stmt: str | None = None
+
+    # execute the stored procedure
     err_msg: str | None = None
     try:
         # obtain a connection
         with connect(connection_kwargs) as conn:
             # make sure the connection is not in autocommit mode
             conn.autocommit = False
             # obtain the cursor and execute the operation
             with conn.cursor() as cursor:
-                cursor.execute(modify_stmt, bind_vals)
-                result = cursor.rowcount
+                proc_stmt = f"SET NOCOUNT ON; EXEC {proc_name} {','.join(('?',) * len(proc_vals))}"
+                cursor.execute(proc_stmt, proc_vals)
+                # obtain the number of tuples returned
+                count: int = cursor.rowcount
+
+                # has the query quota been satisfied ?
+                # noinspection PyTypeChecker
+                if _assert_query_quota(errors, proc_name, None, count, require_min, require_max):
+                    # yes, retrieve the returned tuples
+                    rows: list[Row] = cursor.fetchall()
+                    result = [tuple(row) for row in rows]
             # commit the transaction
             conn.commit()
     except Exception as e:
         err_msg = _db_except_msg(exception=e,
                                  engine="sqlserver")
 
     # log the results
     _db_log(errors=errors,
             err_msg=err_msg,
             logger=logger,
-            query_stmt=modify_stmt,
-            bind_vals=bind_vals)
+            query_stmt=proc_stmt,
+            bind_vals=proc_vals)
 
     return result
 
 
 def _get_connection_kwargs() -> str:
 
     # retrieve the connection parameters
```

### Comparing `pypomes_db-0.4.4/LICENSE` & `pypomes_db-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.4/pyproject.toml` & `pypomes_db-0.4.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.4.4"
+version = "0.4.5"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.4.4/PKG-INFO` & `pypomes_db-0.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.4.4
+Version: 0.4.5
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

