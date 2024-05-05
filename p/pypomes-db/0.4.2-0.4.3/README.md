# Comparing `tmp/pypomes_db-0.4.2.tar.gz` & `tmp/pypomes_db-0.4.3.tar.gz`

## Comparing `pypomes_db-0.4.2.tar` & `pypomes_db-0.4.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 pypomes_db-0.4.2/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 pypomes_db-0.4.2/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    19054 2020-02-02 00:00:00.000000 pypomes_db-0.4.2/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.2/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    12320 2020-02-02 00:00:00.000000 pypomes_db-0.4.2/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    10231 2020-02-02 00:00:00.000000 pypomes_db-0.4.2/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    10350 2020-02-02 00:00:00.000000 pypomes_db-0.4.2/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.4.2/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.4.2/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.2/README.md
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pypomes_db-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 pypomes_db-0.4.3/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0     7187 2020-02-02 00:00:00.000000 pypomes_db-0.4.3/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    18569 2020-02-02 00:00:00.000000 pypomes_db-0.4.3/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.3/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    12321 2020-02-02 00:00:00.000000 pypomes_db-0.4.3/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    10232 2020-02-02 00:00:00.000000 pypomes_db-0.4.3/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    10351 2020-02-02 00:00:00.000000 pypomes_db-0.4.3/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.4.3/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.4.3/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.3/README.md
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pypomes_db-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.4.3/PKG-INFO
```

### Comparing `pypomes_db-0.4.2/src/pypomes_db/__init__.py` & `pypomes_db-0.4.3/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.2/src/pypomes_db/db_common.py` & `pypomes_db-0.4.3/src/pypomes_db/db_common.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,76 @@
 from logging import Logger
 from pypomes_core import (
     APP_PREFIX,
     env_get_int, env_get_str, str_sanitize, str_get_positional
 )
 
+# the preferred way to specify database connection parameters is dynamically with 'db_setup_params'
+# specifying database connection parameters with environment variables can be done in two ways:
+# 1. specify the set
+#   {APP_PREFIX}_DB_ENGINE (one of 'mysql', 'oracle', 'postgres', 'sqlserver')
+#   {APP_PREFIX}_DB_NAME
+#   {APP_PREFIX}_DB_USER
+#   {APP_PREFIX}_DB_PWD
+#   {APP_PREFIX}_DB_HOST
+#   {APP_PREFIX}_DB_PORT
+#   {APP_PREFIX}_DB_CLIENT  (for oracle)
+#   {APP_PREFIX}_DB_DRIVER  (for sqlserver)
+# 2. alternatively, specify a comma-separated list of engines in
+#   {APP_PREFIX}_DB_ENGINES
+#   and for each engine, specify the set above, replacing 'DB' with
+#   'MSQL', 'ORCL', 'PG', and 'SQLS', respectively for engines listed above
+
 _DB_CONN_DATA: dict = {}
 _DB_ENGINES: list[str] = []
 if env_get_str(f"{APP_PREFIX}_DB_ENGINE",  None):
     _default_setup: bool = True
     _DB_ENGINES.append(env_get_str(f"{APP_PREFIX}_DB_ENGINE"))
 else:
     _default_setup: bool = False
     _DB_ENGINES.extend(env_get_str(f"{APP_PREFIX}_DB_ENGINES", "").split(sep=","))
 for engine in _DB_ENGINES:
     if _default_setup:
+        _tag = "DB"
+        _default_setup = False
+    else:
         _tag: str = str_get_positional(source=engine,
                                        list_origin=["mysql", "oracle", "postgres", "sqlserver"],
                                        list_dest=["MSQL", "ORCL", "PG", "SQLS"])
-        _default_setup = False
-    else:
-        _tag = "DB"
     _db_data = {
         "name":  env_get_str(f"{APP_PREFIX}_{_tag}_NAME"),
         "user": env_get_str(f"{APP_PREFIX}_{_tag}_USER"),
         "pwd": env_get_str(f"{APP_PREFIX}_{_tag}_PWD"),
         "host": env_get_str(f"{APP_PREFIX}_{_tag}_HOST"),
         "port": env_get_int(f"{APP_PREFIX}_{_tag}_PORT")
     }
     if engine == "oracle":
         _db_data["client"] = env_get_str(f"{APP_PREFIX}_{_tag}_CLIENT", None)
     elif engine == "sqlserver":
         _db_data["driver"] = env_get_str(f"{APP_PREFIX}_{_tag}_DRIVER")
     _DB_CONN_DATA[engine] = _db_data
 
 
+def _assert_engine(errors: list[str],
+                   engine: str) -> str:
+
+    # initialize the return valiable
+    result: str | None = None
+
+    if not engine and _DB_ENGINES:
+        result = _DB_ENGINES[0]
+    elif engine in _DB_ENGINES:
+        result = engine
+    else:
+        err_msg = f"Database engine '{engine}' unknown or not configured"
+        errors.append(err_msg)
+
+    return result
+
+
 def _assert_query_quota(errors: list[str],
                         query: str,
                         where_vals: tuple,
                         count: int,
                         require_min: int,
                         require_max: int) -> bool:
     """
@@ -51,26 +84,31 @@
     :param require_max: optionally defines the maximum number of tuples to be returned
     :return: whether or not the number of tuples returned is compliant
     """
     # initialize the return variable
     result: bool = True
 
     # has an exact number of tuples been defined but not returned ?
-    if isinstance(require_min, int) and isinstance(require_max, int) and \
-            require_min == require_max and require_min != count:
+    if (isinstance(require_min, int) and
+        isinstance(require_max, int) and
+        require_min == require_max and
+        require_min != count):
         # yes, report the error, if applicable
+        result = False
         if isinstance(errors, list):
             errors.append(
-                f"{count} tuples returned, exactly {require_min} expected, "
+                f"{count} tuples returned, {require_min} expected, "
                 f"for '{_db_build_query_msg(query, where_vals)}'"
             )
-
     # has a minimum number of tuples been defined but not returned ?
-    elif isinstance(require_min, int) and require_min > 0 and count < require_min:
+    elif (isinstance(require_min, int) and
+          require_min > 0 and
+          count < require_min):
         # yes, report the error, if applicable
+        result = False
         if isinstance(errors, list):
             errors.append(
                 f"{count} tuples returned, at least {require_min} expected, "
                 f"for '{_db_build_query_msg(query, where_vals)}'"
             )
 
     return result
```

### Comparing `pypomes_db-0.4.2/src/pypomes_db/db_pomes.py` & `pypomes_db-0.4.3/src/pypomes_db/db_pomes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from logging import Logger
 from typing import Any
 
-from .db_common import _DB_ENGINES, _DB_CONN_DATA
+from .db_common import (
+    _DB_ENGINES, _DB_CONN_DATA, _assert_engine
+)
 
 
 def db_setup(engine: str,
              db_name: str,
              db_user: str,
              db_pwd: str,
              db_host: str,
@@ -68,40 +70,42 @@
     :return: the list of configured engines
     """
     return _DB_ENGINES
 
 
 def db_get_params(engine: str = None) -> dict:
     """
-    The connection parameters are returned as a *dict*, with the keys:
-    *name*, *user*, *pwd*, *host*, *port*.
+    Return the connection parameters a *dict*.
+
+    The returned *dict* contains the keys *name*, *user*, *pwd*, *host*, *port*.
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
+
     The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param logger: optional logger
     :return: the connection to the database
     """
     # initialize the return variable
     result: Any = None
 
-    curr_engine: str = engine or _DB_ENGINES[0]
+    curr_engine: str = _assert_engine(errors, engine)
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
         result = oracle_pomes.db_connect(errors, logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
@@ -207,68 +211,29 @@
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param logger: optional logger
     :return: list of tuples containing the search result, or [] if the search is empty
     """
     # initialize the return variable
     result: list[tuple] | None = None
 
-    curr_engine: str = _DB_ENGINES[0] if not engine and _DB_ENGINES else engine
-    if curr_engine in _DB_ENGINES:
-        if curr_engine == "mysql":
-            pass
-        elif curr_engine == "oracle":
-            from . import oracle_pomes
-            result = oracle_pomes.db_select_all(errors, sel_stmt, where_vals,
-                                                require_min, require_max,  logger)
-        elif curr_engine == "postgres":
-            from . import postgres_pomes
-            result = postgres_pomes.db_select_all(errors, sel_stmt, where_vals,
-                                                  require_min, require_max, logger)
-        elif curr_engine == "sqlserver":
-            from . import sqlserver_pomes
-            result = sqlserver_pomes.db_select_all(errors, sel_stmt, where_vals,
-                                                   require_min, require_max, logger)
-
-    return result
-
-
-def db_modify(errors: list[str] | None,
-              modify_stmt: str,
-              bind_vals: tuple,
-              engine: str = None,
-              logger: Logger = None) -> int:
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
-    curr_engine: str = _DB_ENGINES[0] if not engine and _DB_ENGINES else engine
-    if curr_engine in _DB_ENGINES:
-        if curr_engine == "mysql":
-            pass
-        elif curr_engine == "oracle":
-            from . import oracle_pomes
-            result = oracle_pomes.db_modify(errors, modify_stmt, bind_vals, logger)
-        elif curr_engine == "postgres":
-            from . import postgres_pomes
-            result = postgres_pomes.db_modify(errors, modify_stmt, bind_vals, logger)
-        elif curr_engine == "sqlserver":
-            from . import sqlserver_pomes
-            result = sqlserver_pomes.db_modify(errors, modify_stmt, bind_vals, logger)
+    curr_engine: str = _assert_engine(errors, engine)
+    if curr_engine == "mysql":
+        pass
+    elif curr_engine == "oracle":
+        from . import oracle_pomes
+        result = oracle_pomes.db_select_all(errors, sel_stmt, where_vals,
+                                            require_min, require_max,  logger)
+    elif curr_engine == "postgres":
+        from . import postgres_pomes
+        result = postgres_pomes.db_select_all(errors, sel_stmt, where_vals,
+                                              require_min, require_max, logger)
+    elif curr_engine == "sqlserver":
+        from . import sqlserver_pomes
+        result = sqlserver_pomes.db_select_all(errors, sel_stmt, where_vals,
+                                               require_min, require_max, logger)
 
     return result
 
 
 def db_insert(errors: list[str] | None,
               insert_stmt: str,
               insert_vals: tuple,
@@ -282,15 +247,15 @@
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the values to be inserted
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param logger: optional logger
     :return: the number of inserted tuples (0 ou 1), or None if an error occurred
     """
-    return db_modify(errors, insert_stmt, insert_vals, engine, logger)
+    return _db_modify(errors, insert_stmt, insert_vals, engine, logger)
 
 
 def db_update(errors: list[str] | None,
               update_stmt: str,
               update_vals: tuple,
               where_vals: tuple,
               engine: str = None,
@@ -306,15 +271,15 @@
     :param update_stmt: the UPDATE command
     :param update_vals: the values for the update operation
     :param where_vals: the values to be associated with the search criteria
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param logger: optional logger
     :return: the number of updated tuples, or None if an error occurred
     """
-    return db_modify(errors, update_stmt,  update_vals + where_vals, engine, logger)
+    return _db_modify(errors, update_stmt, update_vals + where_vals, engine, logger)
 
 
 def db_delete(errors: list[str] | None,
               delete_stmt: str,
               where_vals: tuple,
               engine: str = None,
               logger: Logger = None) -> int:
@@ -327,15 +292,15 @@
     :param errors: incidental error messages
     :param delete_stmt: the DELETE command
     :param where_vals: the values to be associated with the search criteria
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param logger: optional logger
     :return: the number of deleted tuples, or None if an error occurred
     """
-    return db_modify(errors, delete_stmt, where_vals, engine, logger)
+    return _db_modify(errors, delete_stmt, where_vals, engine, logger)
 
 
 def db_bulk_insert(errors: list[str] | None,
                    insert_stmt: str,
                    insert_vals: list[tuple],
                    engine: str = None,
                    logger: Logger = None) -> int:
@@ -350,27 +315,26 @@
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param logger: optional logger
     :return: the number of inserted tuples, or None if an error occurred
     """
     # initialize the return variable
     result: int | None = None
 
-    curr_engine: str = _DB_ENGINES[0] if not engine and _DB_ENGINES else engine
-    if curr_engine in _DB_ENGINES:
-        if curr_engine == "mysql":
-            pass
-        elif curr_engine == "oracle":
-            from . import oracle_pomes
-            result = oracle_pomes.db_bulk_insert(errors, insert_stmt, insert_vals, logger)
-        elif curr_engine == "postgres":
-            from . import postgres_pomes
-            result = postgres_pomes.db_bulk_insert(errors, insert_stmt, insert_vals, logger)
-        elif curr_engine == "sqlserver":
-            from . import sqlserver_pomes
-            result = sqlserver_pomes.db_bulk_insert(errors, insert_stmt, insert_vals, logger)
+    curr_engine: str = _assert_engine(errors, engine)
+    if curr_engine == "mysql":
+        pass
+    elif curr_engine == "oracle":
+        from . import oracle_pomes
+        result = oracle_pomes.db_bulk_insert(errors, insert_stmt, insert_vals, logger)
+    elif curr_engine == "postgres":
+        from . import postgres_pomes
+        result = postgres_pomes.db_bulk_insert(errors, insert_stmt, insert_vals, logger)
+    elif curr_engine == "sqlserver":
+        from . import sqlserver_pomes
+        result = sqlserver_pomes.db_bulk_insert(errors, insert_stmt, insert_vals, logger)
 
     return result
 
 
 def db_call_function(errors: list[str] | None,
                      func_name: str,
                      func_vals: tuple,
@@ -387,27 +351,26 @@
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param logger: optional logger
     :return: the data returned by the function
     """
     # initialize the return variable
     result: Any = None
 
-    curr_engine: str = _DB_ENGINES[0] if not engine and _DB_ENGINES else engine
-    if curr_engine in _DB_ENGINES:
-        if curr_engine == "mysql":
-            pass
-        elif curr_engine == "oracle":
-            from . import oracle_pomes
-            result = oracle_pomes.db_call_function(errors, func_name, func_vals, logger)
-        elif curr_engine == "postgres":
-            from . import postgres_pomes
-            result = postgres_pomes.db_call_procedure(errors, func_name, func_vals, logger)
-        elif curr_engine == "sqlserver":
-            from . import sqlserver_pomes
-            result = sqlserver_pomes.db_call_procedure(errors, func_name, func_vals, logger)
+    curr_engine: str = _assert_engine(errors, engine)
+    if curr_engine == "mysql":
+        pass
+    elif curr_engine == "oracle":
+        from . import oracle_pomes
+        result = oracle_pomes.db_call_function(errors, func_name, func_vals, logger)
+    elif curr_engine == "postgres":
+        from . import postgres_pomes
+        result = postgres_pomes.db_call_procedure(errors, func_name, func_vals, logger)
+    elif curr_engine == "sqlserver":
+        from . import sqlserver_pomes
+        result = sqlserver_pomes.db_call_procedure(errors, func_name, func_vals, logger)
 
     return result
 
 
 def db_call_procedure(errors: list[str] | None,
                       proc_name: str,
                       proc_vals: tuple,
@@ -424,22 +387,58 @@
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param logger: optional logger
     :return: the data returned by the procedure
     """
     # initialize the return variable
     result: Any = None
 
-    curr_engine: str = _DB_ENGINES[0] if not engine and _DB_ENGINES else engine
-    if curr_engine in _DB_ENGINES:
-        if curr_engine == "mysql":
-            pass
-        elif curr_engine == "oracle":
-            from . import oracle_pomes
-            result = oracle_pomes.db_call_procedure(errors, proc_name, proc_vals, logger)
-        elif curr_engine == "postgres":
-            from . import postgres_pomes
-            result = postgres_pomes.db_call_procedure(errors, proc_name, proc_vals, logger)
-        elif curr_engine == "sqlserver":
-            from . import sqlserver_pomes
-            result = sqlserver_pomes.db_call_procedure(errors, proc_name, proc_vals, logger)
+    curr_engine: str = _assert_engine(errors, engine)
+    if curr_engine == "mysql":
+        pass
+    elif curr_engine == "oracle":
+        from . import oracle_pomes
+        result = oracle_pomes.db_call_procedure(errors, proc_name, proc_vals, logger)
+    elif curr_engine == "postgres":
+        from . import postgres_pomes
+        result = postgres_pomes.db_call_procedure(errors, proc_name, proc_vals, logger)
+    elif curr_engine == "sqlserver":
+        from . import sqlserver_pomes
+        result = sqlserver_pomes.db_call_procedure(errors, proc_name, proc_vals, logger)
+
+    return result
+
+
+def _db_modify(errors: list[str] | None,
+               modify_stmt: str,
+               bind_vals: tuple,
+               engine: str = None,
+               logger: Logger = None) -> int:
+    """
+    Modify the database, inserting, updating or deleting tuples, according to *modify_stmt* definitions.
+
+    The values for this modification, followed by the values for selecting tuples are in *bind_vals*.
+    The target database engine, default or specified, must have been previously configured.
+
+    :param errors: incidental error messages
+    :param modify_stmt: INSERT, UPDATE, or DELETE statement
+    :param bind_vals: values for database modification, and for tuples selection
+    :param engine: the database engine to use (uses the default engine, if not specified)
+    :param logger: optional logger
+    :return: the number of inserted, modified, or deleted tuples, ou None if an error occurred
+    """
+    # initialize the return variable
+    result: int | None = None
+
+    curr_engine: str = _assert_engine(errors, engine)
+    if curr_engine == "mysql":
+        pass
+    elif curr_engine == "oracle":
+        from . import oracle_pomes
+        result = oracle_pomes.db_modify(errors, modify_stmt, bind_vals, logger)
+    elif curr_engine == "postgres":
+        from . import postgres_pomes
+        result = postgres_pomes.db_modify(errors, modify_stmt, bind_vals, logger)
+    elif curr_engine == "sqlserver":
+        from . import sqlserver_pomes
+        result = sqlserver_pomes.db_modify(errors, modify_stmt, bind_vals, logger)
 
     return result
```

### Comparing `pypomes_db-0.4.2/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.4.3/src/pypomes_db/oracle_pomes.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         err_msg = _db_except_msg(exception=e,
                                  engine="oracle")
 
     # log the results
     _db_log(errors=errors,
             err_msg=err_msg,
             logger=logger,
-            query_stmt=f"Connected to '{name}' at '{host}'")
+            query_stmt=f"Connecting to '{name}' at '{host}'")
 
     return result
 
 
 def db_select_all(errors: list[str] | None,
                   sel_stmt: str,
                   where_vals: tuple = None,
```

### Comparing `pypomes_db-0.4.2/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.4.3/src/pypomes_db/postgres_pomes.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     except Exception as e:
         err_msg = _db_except_msg(e, "postgres")
 
     # log the results
     _db_log(errors=errors,
             err_msg=err_msg,
             logger=logger,
-            query_stmt=f"Connected to '{name}' at '{host}'")
+            query_stmt=f"Connecting to '{name}' at '{host}'")
 
     return result
 
 
 def db_select_all(errors: list[str] | None,
                   sel_stmt: str,
                   where_vals: tuple = None,
```

### Comparing `pypomes_db-0.4.2/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.4.3/src/pypomes_db/sqlserver_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                                  engine="sqlserver")
 
     # log the results
     name, _user, _pwd, host, _port = _db_get_params("sqlserver")
     _db_log(errors=errors,
             err_msg=err_msg,
             logger=logger,
-            query_stmt=f"Connected to '{name}' at '{host}'")
+            query_stmt=f"Connecting to '{name}' at '{host}'")
 
     return result
 
 
 def db_select_all(errors: list[str] | None,
                   sel_stmt: str,
                   where_vals: tuple = None,
```

### Comparing `pypomes_db-0.4.2/LICENSE` & `pypomes_db-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.2/pyproject.toml` & `pypomes_db-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.4.2"
+version = "0.4.3"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.4.2/PKG-INFO` & `pypomes_db-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.4.2
+Version: 0.4.3
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

