# Comparing `tmp/pypomes_db-0.4.3.tar.gz` & `tmp/pypomes_db-0.4.4.tar.gz`

## Comparing `pypomes_db-0.4.3.tar` & `pypomes_db-0.4.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 pypomes_db-0.4.3/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0     7187 2020-02-02 00:00:00.000000 pypomes_db-0.4.3/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    18569 2020-02-02 00:00:00.000000 pypomes_db-0.4.3/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.3/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    12321 2020-02-02 00:00:00.000000 pypomes_db-0.4.3/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    10232 2020-02-02 00:00:00.000000 pypomes_db-0.4.3/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    10351 2020-02-02 00:00:00.000000 pypomes_db-0.4.3/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.4.3/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.4.3/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.3/README.md
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pypomes_db-0.4.3/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 pypomes_db-0.4.4/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 pypomes_db-0.4.4/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    19562 2020-02-02 00:00:00.000000 pypomes_db-0.4.4/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.4/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    12106 2020-02-02 00:00:00.000000 pypomes_db-0.4.4/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    10232 2020-02-02 00:00:00.000000 pypomes_db-0.4.4/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    10351 2020-02-02 00:00:00.000000 pypomes_db-0.4.4/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.4.4/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.4.4/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.4/README.md
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pypomes_db-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.4.4/PKG-INFO
```

### Comparing `pypomes_db-0.4.3/src/pypomes_db/__init__.py` & `pypomes_db-0.4.4/src/pypomes_db/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from .db_pomes import (
     db_setup, db_get_engines, db_get_params,
-    db_connect, db_exists, db_select_one, db_select_all,
-    db_update, db_delete, db_insert, db_bulk_insert,
+    db_assert_connection, db_connect, db_exists,
+    db_select_one, db_select_all, db_update,
+    db_delete, db_insert, db_bulk_insert,
     db_call_function, db_call_procedure,
 )
 
 __all__ = [
     # db_pomes
     "db_setup", "db_get_engines", "db_get_params",
-    "db_connect", "db_exists", "db_select_one", "db_select_all",
-    "db_update", "db_delete", "db_insert", "db_bulk_insert",
+    "db_assert_connection", "db_connect", "db_exists",
+    "db_select_one", "db_select_all", "db_update",
+    "db_delete", "db_insert", "db_bulk_insert",
     "db_call_function", "db_call_procedure",
 ]
 
 from importlib.metadata import version
 __version__ = version("pypomes_db")
 __version_info__ = tuple(int(i) for i in __version__.split(".") if i.isdigit())
```

### Comparing `pypomes_db-0.4.3/src/pypomes_db/db_common.py` & `pypomes_db-0.4.4/src/pypomes_db/db_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 from logging import Logger
 from pypomes_core import (
     APP_PREFIX,
     env_get_int, env_get_str, str_sanitize, str_get_positional
 )
 
 # the preferred way to specify database connection parameters is dynamically with 'db_setup_params'
```

### Comparing `pypomes_db-0.4.3/src/pypomes_db/db_pomes.py` & `pypomes_db-0.4.4/src/pypomes_db/db_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,43 @@
 
     :param engine: the database engine
     :return: the current connection parameters for the engine
     """
     return _DB_CONN_DATA.get(engine or _DB_ENGINES[0])
 
 
+def db_assert_connection(errors: list[str] | None,
+                         engine: str = None,
+                         logger: Logger = None) -> bool:
+    """
+    Determine whether the *engine*'s current configuration allows for a safe connection.
+
+    :param errors: incidental errors
+    :param engine: the database engine to use (uses the default engine, if not specified)
+    :param logger: optional logger
+    :return: True if the trial connection succeeded, False otherwise
+    """
+    # initialize the return variable
+    result: bool = False
+
+    curr_engine: str = _assert_engine(errors, engine)
+    proceed: bool = True
+    if curr_engine == "oracle":
+        from . import oracle_pomes
+        # noinspection PyProtectedMember
+        proceed = oracle_pomes._initialize(errors, logger)
+    if proceed:
+        conn: Any = db_connect(errors, curr_engine, logger)
+        if conn:
+            conn.close()
+            result = True
+
+    return result
+
+
 def db_connect(errors: list[str] | None,
                engine: str = None,
                logger: Logger = None) -> Any:
     """
     Obtain and return a connection to the database, or *None* if the connection cannot be obtained.
 
     The target database engine, default or specified, must have been previously configured.
```

### Comparing `pypomes_db-0.4.3/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.4.4/src/pypomes_db/oracle_pomes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from logging import Logger
-from oracledb import Connection, connect
+from oracledb import Connection, connect, init_oracle_client
 
 from .db_common import (
-    _assert_query_quota, _db_get_params, _db_log, _db_except_msg
+    _DB_CONN_DATA, _assert_query_quota, _db_get_params, _db_log, _db_except_msg
 )
 
 # TODO: db_call_function, db_call_procedure
 
 
 def db_connect(errors: list[str],
                logger: Logger = None) -> Connection:
@@ -171,65 +171,31 @@
             query_stmt=insert_stmt,
             bind_vals=insert_vals[0])
 
     return result
 
 
 # TODO: see https://python-oracledb.readthedocs.io/en/latest/user_guide/plsql_execution.html
+# noinspection PyUnusedLocal
 def db_call_function(errors: list[str] | None,
                      func_name: str,
                      func_vals: tuple,
                      logger: Logger = None) -> list[tuple]:
     """
     Execute the stored function *func_name* in the database, with the parameters given in *func_vals*.
 
     :param errors: incidental error messages
     :param func_name: name of the stored function
     :param func_vals: parameters for the stored function
     :param logger: optional logger
     :return: the data returned by the function
     """
     # initialize the return variable
-    # noinspection DuplicatedCode
     result: list[tuple] = []
 
-    # retrieve the connection parameters
-    name, user, pwd, host, port = _db_get_params("oracle")
-
-    # execute the stored procedure
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
-            # obtain a cursor and perform the operation
-            with conn.cursor() as cursor:
-                cursor.callproc(name=func_name,
-                                parameters=func_vals)
-                # yes, retrieve the returned tuples
-                result = list(cursor)
-            # commit the transaction
-            conn.commit()
-    except Exception as e:
-        err_msg = _db_except_msg(exception=e,
-                                 engine="oracle")
-
-    # log the results
-    _db_log(errors, err_msg, logger, func_name, func_vals)
-    _db_log(errors=errors,
-            err_msg=err_msg,
-            logger=logger,
-            query_stmt=func_name,
-            bind_vals=func_vals)
-
     return result
 
 
 # TODO: see https://python-oracledb.readthedocs.io/en/latest/user_guide/plsql_execution.html
 def db_call_procedure(errors: list[str] | None,
                       proc_name: str,
                       proc_vals: tuple,
@@ -323,15 +289,47 @@
             # commit the transaction
             conn.commit()
     except Exception as e:
         err_msg = _db_except_msg(exception=e,
                                  engine="oracle")
 
     # log the results
-    _db_log(errors, err_msg, logger, modify_stmt, bind_vals)
     _db_log(errors=errors,
             err_msg=err_msg,
             logger=logger,
             query_stmt=modify_stmt,
             bind_vals=bind_vals)
 
     return result
+
+__is_initialized: str | None = None
+
+def _initialize(errors: list[str] | None,
+                logger: Logger) -> bool:
+    """
+    Setup the oracle engine to access the database throught the installed client software.
+
+    :param errors: incidental error messages
+    :param logger: optional logger
+    :return: False if an error happened, True otherwise
+    """
+    # initialize the return variable
+    result: bool = True
+
+    global __is_initialized
+    if not __is_initialized:
+        err_msg: str | None = None
+        client: str = _DB_CONN_DATA["oracle"]["client"]
+        try:
+            init_oracle_client(client)
+            __is_initialized = True
+        except Exception as e:
+            result = False
+            err_msg = _db_except_msg(exception=e,
+                                     engine="oracle")
+        # log the results
+        _db_log(errors=errors,
+                err_msg=err_msg,
+                logger=logger,
+                query_stmt="Initializing the client")
+
+    return result
```

### Comparing `pypomes_db-0.4.3/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.4.4/src/pypomes_db/postgres_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.3/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.4.4/src/pypomes_db/sqlserver_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.3/LICENSE` & `pypomes_db-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.3/pyproject.toml` & `pypomes_db-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.4.3"
+version = "0.4.4"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.4.3/PKG-INFO` & `pypomes_db-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.4.3
+Version: 0.4.4
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

