# Comparing `tmp/pypomes_db-0.4.7.tar.gz` & `tmp/pypomes_db-0.4.8.tar.gz`

## Comparing `pypomes_db-0.4.7.tar` & `pypomes_db-0.4.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 pypomes_db-0.4.7/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0     7815 2020-02-02 00:00:00.000000 pypomes_db-0.4.7/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    19681 2020-02-02 00:00:00.000000 pypomes_db-0.4.7/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.7/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    12532 2020-02-02 00:00:00.000000 pypomes_db-0.4.7/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    10382 2020-02-02 00:00:00.000000 pypomes_db-0.4.7/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    10670 2020-02-02 00:00:00.000000 pypomes_db-0.4.7/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.4.7/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.4.7/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.7/README.md
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pypomes_db-0.4.7/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 pypomes_db-0.4.8/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0     7853 2020-02-02 00:00:00.000000 pypomes_db-0.4.8/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    19681 2020-02-02 00:00:00.000000 pypomes_db-0.4.8/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.8/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    12532 2020-02-02 00:00:00.000000 pypomes_db-0.4.8/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    10382 2020-02-02 00:00:00.000000 pypomes_db-0.4.8/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    10670 2020-02-02 00:00:00.000000 pypomes_db-0.4.8/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.4.8/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.4.8/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.8/README.md
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pypomes_db-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.4.8/PKG-INFO
```

### Comparing `pypomes_db-0.4.7/src/pypomes_db/__init__.py` & `pypomes_db-0.4.8/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.7/src/pypomes_db/db_common.py` & `pypomes_db-0.4.8/src/pypomes_db/db_common.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,17 @@
 _DB_CONN_DATA: dict = {}
 _DB_ENGINES: list[str] = []
 if env_get_str(f"{APP_PREFIX}_DB_ENGINE",  None):
     _default_setup: bool = True
     _DB_ENGINES.append(env_get_str(f"{APP_PREFIX}_DB_ENGINE"))
 else:
     _default_setup: bool = False
-    _DB_ENGINES.extend(env_get_str(f"{APP_PREFIX}_DB_ENGINES", "").split(sep=","))
+    _engines = env_get_str(f"{APP_PREFIX}_DB_ENGINES", None)
+    if _engines:
+        _DB_ENGINES.extend(_engines.split(sep=","))
 for engine in _DB_ENGINES:
     if _default_setup:
         _tag = "DB"
         _default_setup = False
     else:
         _tag: str = str_get_positional(source=engine,
                                        list_origin=["mysql", "oracle", "postgres", "sqlserver"],
@@ -57,15 +59,15 @@
     Verify if *engine* is in the list of supported engines.
 
     If *engine* is a supported engine, it is returned. If its value is 'None',
     the first engine in the list of supported engines (the default engine) is returned.
 
     :param errors: incidental errors
     :param engine: the database engine to verify
-    :return: the validated engine or the default engine
+    :return: the validated or default engine
     """
     # initialize the return valiable
     result: str | None = None
 
     if not engine and _DB_ENGINES:
         result = _DB_ENGINES[0]
     elif engine in _DB_ENGINES:
@@ -134,15 +136,15 @@
     :param engine: the database engine
     :return: the current connection parameters for the engine
     """
     name: str = _DB_CONN_DATA[engine]["name"]
     user: str = _DB_CONN_DATA[engine]["user"]
     pwd: str = _DB_CONN_DATA[engine]["pwd"]
     host: str = _DB_CONN_DATA[engine]["host"]
-    port: str = _DB_CONN_DATA[engine]["port"]
+    port: int = _DB_CONN_DATA[engine]["port"]
 
     result: tuple
     if engine == "sqlserver":
         driver: str = _DB_CONN_DATA[engine]["driver"]
         result = (name, user, pwd, host, port, driver)
     else:
         result = (name, user, pwd, host, port)
```

### Comparing `pypomes_db-0.4.7/src/pypomes_db/db_pomes.py` & `pypomes_db-0.4.8/src/pypomes_db/db_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.7/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.4.8/src/pypomes_db/oracle_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.7/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.4.8/src/pypomes_db/postgres_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.7/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.4.8/src/pypomes_db/sqlserver_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.7/LICENSE` & `pypomes_db-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.7/pyproject.toml` & `pypomes_db-0.4.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.4.7"
+version = "0.4.8"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

