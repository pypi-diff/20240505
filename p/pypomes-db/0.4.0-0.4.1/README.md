# Comparing `tmp/pypomes_db-0.4.0.tar.gz` & `tmp/pypomes_db-0.4.1.tar.gz`

## Comparing `pypomes_db-0.4.0.tar` & `pypomes_db-0.4.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 pypomes_db-0.4.0/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 pypomes_db-0.4.0/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    16482 2020-02-02 00:00:00.000000 pypomes_db-0.4.0/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.0/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    12320 2020-02-02 00:00:00.000000 pypomes_db-0.4.0/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    10231 2020-02-02 00:00:00.000000 pypomes_db-0.4.0/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    10350 2020-02-02 00:00:00.000000 pypomes_db-0.4.0/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.4.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.4.0/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.0/README.md
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pypomes_db-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 pypomes_db-0.4.1/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 pypomes_db-0.4.1/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    16563 2020-02-02 00:00:00.000000 pypomes_db-0.4.1/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.1/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    12320 2020-02-02 00:00:00.000000 pypomes_db-0.4.1/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    10231 2020-02-02 00:00:00.000000 pypomes_db-0.4.1/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    10350 2020-02-02 00:00:00.000000 pypomes_db-0.4.1/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.4.1/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.1/README.md
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pypomes_db-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.4.1/PKG-INFO
```

### Comparing `pypomes_db-0.4.0/src/pypomes_db/__init__.py` & `pypomes_db-0.4.1/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.0/src/pypomes_db/db_common.py` & `pypomes_db-0.4.1/src/pypomes_db/db_common.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.0/src/pypomes_db/db_pomes.py` & `pypomes_db-0.4.1/src/pypomes_db/db_pomes.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,20 +34,24 @@
         "port": db_port
     }
     if engine == "oracle":
         _DB_CONN_DATA[engine]["client"] = db_client
     elif engine == "sqlserver":
         _DB_CONN_DATA[engine]["driver"] = db_driver
 
+    if engine not in _DB_ENGINES:
+        _DB_ENGINES.append(engine)
+
 
 def db_get_engines() -> list[str]:
     """
-    Return a list of configured engines.
+    Return the list of configured engines.
 
-    This list may include one or more of the supported engines: mysql, oracle, postgres, sqlserver.
+    This list may include any of the supported engines:
+     *mysql*, *oracle*, *postgres*, *sqlserver*.
 
     :return: the list of configure engines
     """
     return _DB_ENGINES
 
 
 def db_get_params(engine: str = None) -> dict:
```

### Comparing `pypomes_db-0.4.0/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.4.1/src/pypomes_db/oracle_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.0/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.4.1/src/pypomes_db/postgres_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.0/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.4.1/src/pypomes_db/sqlserver_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.0/LICENSE` & `pypomes_db-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.0/pyproject.toml` & `pypomes_db-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.4.0"
+version = "0.4.1"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.4.0/PKG-INFO` & `pypomes_db-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.4.0
+Version: 0.4.1
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

