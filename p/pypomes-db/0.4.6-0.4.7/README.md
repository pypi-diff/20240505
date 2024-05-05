# Comparing `tmp/pypomes_db-0.4.6.tar.gz` & `tmp/pypomes_db-0.4.7.tar.gz`

## Comparing `pypomes_db-0.4.6.tar` & `pypomes_db-0.4.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 pypomes_db-0.4.6/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 pypomes_db-0.4.6/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    19681 2020-02-02 00:00:00.000000 pypomes_db-0.4.6/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.6/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    12254 2020-02-02 00:00:00.000000 pypomes_db-0.4.6/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    10382 2020-02-02 00:00:00.000000 pypomes_db-0.4.6/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    10501 2020-02-02 00:00:00.000000 pypomes_db-0.4.6/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.4.6/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.4.6/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.6/README.md
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pypomes_db-0.4.6/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 pypomes_db-0.4.7/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0     7815 2020-02-02 00:00:00.000000 pypomes_db-0.4.7/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    19681 2020-02-02 00:00:00.000000 pypomes_db-0.4.7/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.7/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    12532 2020-02-02 00:00:00.000000 pypomes_db-0.4.7/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    10382 2020-02-02 00:00:00.000000 pypomes_db-0.4.7/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    10670 2020-02-02 00:00:00.000000 pypomes_db-0.4.7/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.4.7/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.4.7/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.7/README.md
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pypomes_db-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.4.7/PKG-INFO
```

### Comparing `pypomes_db-0.4.6/src/pypomes_db/__init__.py` & `pypomes_db-0.4.7/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.6/src/pypomes_db/db_common.py` & `pypomes_db-0.4.7/src/pypomes_db/db_common.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,15 +49,24 @@
     elif engine == "sqlserver":
         _db_data["driver"] = env_get_str(f"{APP_PREFIX}_{_tag}_DRIVER")
     _DB_CONN_DATA[engine] = _db_data
 
 
 def _assert_engine(errors: list[str],
                    engine: str) -> str:
+    """
+    Verify if *engine* is in the list of supported engines.
+
+    If *engine* is a supported engine, it is returned. If its value is 'None',
+    the first engine in the list of supported engines (the default engine) is returned.
 
+    :param errors: incidental errors
+    :param engine: the database engine to verify
+    :return: the validated engine or the default engine
+    """
     # initialize the return valiable
     result: str | None = None
 
     if not engine and _DB_ENGINES:
         result = _DB_ENGINES[0]
     elif engine in _DB_ENGINES:
         result = engine
@@ -71,15 +80,15 @@
 def _assert_query_quota(errors: list[str],
                         query: str,
                         where_vals: tuple,
                         count: int,
                         require_min: int,
                         require_max: int) -> bool:
     """
-    Veriy whether the number of tuples returned is compliant with the constraints specified.
+    Verify whether the number of tuples returned is compliant with the constraints specified.
 
     :param errors:  incidental error messages
     :param query: the query statement used
     :param where_vals: the bind values used in the query
     :param count: the number of tuples returned
     :param require_min: optionally defines the minimum number of tuples to be returned
     :param require_max: optionally defines the maximum number of tuples to be returned
@@ -114,29 +123,35 @@
 
     return result
 
 def _db_get_params(engine: str) -> tuple:
     """
     Return the current connection parameters being used for *engine*.
 
-    The connection parameters are returned as a *tuple*, with the elements:
-    (*name*, *user*, *pwd*, *host*, *port*).
-
+    The connection parameters are returned as a *tuple*, with the elements
+    *name*, *user*, *pwd*, *host*, *port*.
     The meaning of some parameters may vary between different database engines.
 
     :param engine: the database engine
     :return: the current connection parameters for the engine
     """
     name: str = _DB_CONN_DATA[engine]["name"]
     user: str = _DB_CONN_DATA[engine]["user"]
     pwd: str = _DB_CONN_DATA[engine]["pwd"]
     host: str = _DB_CONN_DATA[engine]["host"]
     port: str = _DB_CONN_DATA[engine]["port"]
 
-    return name, user, pwd, host, port
+    result: tuple
+    if engine == "sqlserver":
+        driver: str = _DB_CONN_DATA[engine]["driver"]
+        result = (name, user, pwd, host, port, driver)
+    else:
+        result = (name, user, pwd, host, port)
+
+    return result
 
 
 def _db_except_msg(exception: Exception,
                    engine: str) -> str:
     """
     Format and return the error message corresponding to the exception raised while accessing the database.
```

### Comparing `pypomes_db-0.4.6/src/pypomes_db/db_pomes.py` & `pypomes_db-0.4.7/src/pypomes_db/db_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.6/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.4.7/src/pypomes_db/oracle_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,14 +124,18 @@
 def db_bulk_insert(errors: list[str],
                    insert_stmt: str,
                    insert_vals: list[tuple],
                    logger: Logger = None) -> int:
     """
     Insert the tuples, with values defined in *insert_vals*, into the database.
 
+    The binding must be done by position. Thus, the *VALUES* clause in *insert_stmt*
+    must contain as many ':n' placeholders as there are elements in the tuples found in the
+    list provided in *insert_vals*, where 'n' is the 1-based position of the data in the tuple.
+
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the list of values to be inserted
     :param logger: optional logger
     :return: the number of inserted tuples, or None if an error occurred
     """
     # initialize the return variable
```

### Comparing `pypomes_db-0.4.6/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.4.7/src/pypomes_db/postgres_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.6/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.4.7/src/pypomes_db/sqlserver_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,14 +112,17 @@
 def db_bulk_insert(errors: list[str],
                    insert_stmt: str,
                    insert_vals: list[tuple],
                    logger: Logger = None) -> int:
     """
     Insert the tuples, with values defined in *insert_vals*, into the database.
 
+    The *VALUES* clause in *insert_stmt* must contain as many '%s' placeholders
+    as there are elements in the tuples found in the list provided in *insert_vals*.
+
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the list of values to be inserted
     :param logger: optional logger
     :return: the number of inserted tuples, or None if an error occurred
     """
     # initialize the return variable
```

### Comparing `pypomes_db-0.4.6/LICENSE` & `pypomes_db-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.6/pyproject.toml` & `pypomes_db-0.4.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.4.6"
+version = "0.4.7"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -19,15 +19,15 @@
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "pip>=24.0",
 #   "oracledb>=2.1.2",
 #   "psycopg2-binary>=2.9.9",
 #   "pyodbc>=5.1.0",
-    "pypomes_core>=0.9.6",
+    "pypomes_core>=0.9.7",
     "setuptools>=68.0.0",
     "wheel>=0.42.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-DB"
 "Bug Tracker" = "https://github.com/TheWiseCoder/PyPomes-DB/issues"
```

### Comparing `pypomes_db-0.4.6/PKG-INFO` & `pypomes_db-0.4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.4.6
+Version: 0.4.7
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: pip>=24.0
-Requires-Dist: pypomes-core>=0.9.6
+Requires-Dist: pypomes-core>=0.9.7
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.42.0
```

