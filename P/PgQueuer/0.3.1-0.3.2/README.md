# Comparing `tmp/pgqueuer-0.3.1.tar.gz` & `tmp/pgqueuer-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgqueuer-0.3.1.tar", last modified: Sun May  5 09:27:00 2024, max compression
+gzip compressed data, was "pgqueuer-0.3.2.tar", last modified: Sun May  5 10:05:00 2024, max compression
```

## Comparing `pgqueuer-0.3.1.tar` & `pgqueuer-0.3.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:27:00.316751 pgqueuer-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:27:00.308751 pgqueuer-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:27:00.312751 pgqueuer-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-05 09:27:00.316751 pgqueuer-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 09:27:00.316751 pgqueuer-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:27:00.312751 pgqueuer-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:27:00.312751 pgqueuer-0.3.1/src/PgQueuer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/src/PgQueuer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/src/PgQueuer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/src/PgQueuer/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/src/PgQueuer/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/src/PgQueuer/logconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/src/PgQueuer/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/src/PgQueuer/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/src/PgQueuer/qm.py
--rw-r--r--   0 runner    (1001) docker     (127)    16173 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/src/PgQueuer/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/src/PgQueuer/tm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:27:00.316751 pgqueuer-0.3.1/src/PgQueuer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-05 09:27:00.000000 pgqueuer-0.3.1/src/PgQueuer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-05 09:27:00.000000 pgqueuer-0.3.1/src/PgQueuer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 09:27:00.000000 pgqueuer-0.3.1/src/PgQueuer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-05 09:27:00.000000 pgqueuer-0.3.1/src/PgQueuer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-05 09:27:00.000000 pgqueuer-0.3.1/src/PgQueuer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-05 09:27:00.000000 pgqueuer-0.3.1/src/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:27:00.316751 pgqueuer-0.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:27:00.316751 pgqueuer-0.3.1/test/db/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/test/db/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (127)      266 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/test/db/init_db.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/test/test_qm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/test/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/test/test_tm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:27:00.316751 pgqueuer-0.3.1/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/tools/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:05:00.227696 pgqueuer-0.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:05:00.219696 pgqueuer-0.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:05:00.219696 pgqueuer-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-05 10:04:49.000000 pgqueuer-0.3.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-05 10:04:49.000000 pgqueuer-0.3.2/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-05 10:04:49.000000 pgqueuer-0.3.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-05 10:04:49.000000 pgqueuer-0.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-05 10:04:49.000000 pgqueuer-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-05-05 10:05:00.227696 pgqueuer-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-05-05 10:04:49.000000 pgqueuer-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-05 10:04:49.000000 pgqueuer-0.3.2/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-05 10:04:49.000000 pgqueuer-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 10:05:00.227696 pgqueuer-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:05:00.219696 pgqueuer-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:05:00.223696 pgqueuer-0.3.2/src/PgQueuer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:04:49.000000 pgqueuer-0.3.2/src/PgQueuer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-05 10:04:49.000000 pgqueuer-0.3.2/src/PgQueuer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-05 10:04:49.000000 pgqueuer-0.3.2/src/PgQueuer/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-05-05 10:04:49.000000 pgqueuer-0.3.2/src/PgQueuer/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-05 10:04:49.000000 pgqueuer-0.3.2/src/PgQueuer/logconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-05 10:04:49.000000 pgqueuer-0.3.2/src/PgQueuer/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:04:49.000000 pgqueuer-0.3.2/src/PgQueuer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-05-05 10:04:49.000000 pgqueuer-0.3.2/src/PgQueuer/qm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16173 2024-05-05 10:04:49.000000 pgqueuer-0.3.2/src/PgQueuer/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-05 10:04:49.000000 pgqueuer-0.3.2/src/PgQueuer/tm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:05:00.223696 pgqueuer-0.3.2/src/PgQueuer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-05-05 10:05:00.000000 pgqueuer-0.3.2/src/PgQueuer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-05 10:05:00.000000 pgqueuer-0.3.2/src/PgQueuer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 10:05:00.000000 pgqueuer-0.3.2/src/PgQueuer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-05 10:05:00.000000 pgqueuer-0.3.2/src/PgQueuer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-05 10:05:00.000000 pgqueuer-0.3.2/src/PgQueuer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-05 10:05:00.000000 pgqueuer-0.3.2/src/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:05:00.223696 pgqueuer-0.3.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-05 10:04:49.000000 pgqueuer-0.3.2/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:05:00.223696 pgqueuer-0.3.2/test/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-05 10:04:49.000000 pgqueuer-0.3.2/test/db/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (127)      266 2024-05-05 10:04:49.000000 pgqueuer-0.3.2/test/db/init_db.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-05 10:04:49.000000 pgqueuer-0.3.2/test/test_qm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-05-05 10:04:49.000000 pgqueuer-0.3.2/test/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-05 10:04:49.000000 pgqueuer-0.3.2/test/test_tm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:05:00.223696 pgqueuer-0.3.2/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-05 10:04:49.000000 pgqueuer-0.3.2/tools/benchmark.py
```

### Comparing `pgqueuer-0.3.1/.github/workflows/ci.yml` & `pgqueuer-0.3.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.1/.github/workflows/linting.yml` & `pgqueuer-0.3.2/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.1/.github/workflows/release.yml` & `pgqueuer-0.3.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.1/.gitignore` & `pgqueuer-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.1/LICENSE` & `pgqueuer-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.1/PKG-INFO` & `pgqueuer-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: PgQueuer
-Version: 0.3.1
+Version: 0.3.2
 Summary: PgQueuer is a Python library leveraging PostgreSQL for efficient job queuing.
 Author: janbjorge
 License: MIT License
-Project-URL: Documentation, https://github.com/janbjorge/PgQueuer/
+Project-URL: Documentation, https://github.com/janbjorge/PgQueuer/wiki
 Project-URL: Homepage, https://github.com/janbjorge/PgQueuer/
 Project-URL: Issues, https://github.com/janbjorge/PgQueuer/issues
 Project-URL: Repository, https://github.com/janbjorge/PgQueuer/
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
```

### Comparing `pgqueuer-0.3.1/README.md` & `pgqueuer-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.1/pyproject.toml` & `pgqueuer-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     "asyncpg>=0.27.0",
     "pgcachewatch>=0.4",
     "pydantic>=2.0.0",
     "tabulate>=0.9.0",
 ]
 
 [project.urls]
-Documentation = "https://github.com/janbjorge/PgQueuer/"
+Documentation = "https://github.com/janbjorge/PgQueuer/wiki"
 Homepage = "https://github.com/janbjorge/PgQueuer/"
 Issues = "https://github.com/janbjorge/PgQueuer/issues"
 Repository = "https://github.com/janbjorge/PgQueuer/"
 
 [project.optional-dependencies]
 dev = [
     "asyncpg-stubs",
```

### Comparing `pgqueuer-0.3.1/src/PgQueuer/cli.py` & `pgqueuer-0.3.2/src/PgQueuer/cli.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.1/src/PgQueuer/models.py` & `pgqueuer-0.3.2/src/PgQueuer/models.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.1/src/PgQueuer/qm.py` & `pgqueuer-0.3.2/src/PgQueuer/qm.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.1/src/PgQueuer/queries.py` & `pgqueuer-0.3.2/src/PgQueuer/queries.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.1/src/PgQueuer/tm.py` & `pgqueuer-0.3.2/src/PgQueuer/tm.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.1/src/PgQueuer.egg-info/PKG-INFO` & `pgqueuer-0.3.2/src/PgQueuer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: PgQueuer
-Version: 0.3.1
+Version: 0.3.2
 Summary: PgQueuer is a Python library leveraging PostgreSQL for efficient job queuing.
 Author: janbjorge
 License: MIT License
-Project-URL: Documentation, https://github.com/janbjorge/PgQueuer/
+Project-URL: Documentation, https://github.com/janbjorge/PgQueuer/wiki
 Project-URL: Homepage, https://github.com/janbjorge/PgQueuer/
 Project-URL: Issues, https://github.com/janbjorge/PgQueuer/issues
 Project-URL: Repository, https://github.com/janbjorge/PgQueuer/
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
```

### Comparing `pgqueuer-0.3.1/src/PgQueuer.egg-info/SOURCES.txt` & `pgqueuer-0.3.2/src/PgQueuer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.1/test/conftest.py` & `pgqueuer-0.3.2/test/conftest.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.1/test/db/Dockerfile` & `pgqueuer-0.3.2/test/db/Dockerfile`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.1/test/test_qm.py` & `pgqueuer-0.3.2/test/test_qm.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.1/test/test_queries.py` & `pgqueuer-0.3.2/test/test_queries.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.1/test/test_tm.py` & `pgqueuer-0.3.2/test/test_tm.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.1/tools/benchmark.py` & `pgqueuer-0.3.2/tools/benchmark.py`

 * *Files identical despite different names*

