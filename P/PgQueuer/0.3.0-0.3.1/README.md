# Comparing `tmp/pgqueuer-0.3.0.tar.gz` & `tmp/pgqueuer-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgqueuer-0.3.0.tar", last modified: Fri May  3 17:17:58 2024, max compression
+gzip compressed data, was "pgqueuer-0.3.1.tar", last modified: Sun May  5 09:27:00 2024, max compression
```

## Comparing `pgqueuer-0.3.0.tar` & `pgqueuer-0.3.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:58.042320 pgqueuer-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:58.034320 pgqueuer-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:58.034320 pgqueuer-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-03 17:17:48.000000 pgqueuer-0.3.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-03 17:17:48.000000 pgqueuer-0.3.0/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-03 17:17:48.000000 pgqueuer-0.3.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-03 17:17:48.000000 pgqueuer-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-03 17:17:48.000000 pgqueuer-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-03 17:17:58.042320 pgqueuer-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-05-03 17:17:48.000000 pgqueuer-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-03 17:17:48.000000 pgqueuer-0.3.0/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-03 17:17:48.000000 pgqueuer-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 17:17:58.042320 pgqueuer-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:58.034320 pgqueuer-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:58.038320 pgqueuer-0.3.0/src/PgQueuer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:48.000000 pgqueuer-0.3.0/src/PgQueuer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-03 17:17:48.000000 pgqueuer-0.3.0/src/PgQueuer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-03 17:17:48.000000 pgqueuer-0.3.0/src/PgQueuer/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-05-03 17:17:48.000000 pgqueuer-0.3.0/src/PgQueuer/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-03 17:17:48.000000 pgqueuer-0.3.0/src/PgQueuer/logconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-03 17:17:48.000000 pgqueuer-0.3.0/src/PgQueuer/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:48.000000 pgqueuer-0.3.0/src/PgQueuer/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-05-03 17:17:48.000000 pgqueuer-0.3.0/src/PgQueuer/qm.py
--rw-r--r--   0 runner    (1001) docker     (127)    12740 2024-05-03 17:17:48.000000 pgqueuer-0.3.0/src/PgQueuer/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-03 17:17:48.000000 pgqueuer-0.3.0/src/PgQueuer/tm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:58.038320 pgqueuer-0.3.0/src/PgQueuer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-03 17:17:58.000000 pgqueuer-0.3.0/src/PgQueuer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-03 17:17:58.000000 pgqueuer-0.3.0/src/PgQueuer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 17:17:58.000000 pgqueuer-0.3.0/src/PgQueuer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-03 17:17:58.000000 pgqueuer-0.3.0/src/PgQueuer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-03 17:17:58.000000 pgqueuer-0.3.0/src/PgQueuer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-03 17:17:57.000000 pgqueuer-0.3.0/src/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:58.038320 pgqueuer-0.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-03 17:17:48.000000 pgqueuer-0.3.0/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:58.038320 pgqueuer-0.3.0/test/db/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-03 17:17:48.000000 pgqueuer-0.3.0/test/db/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (127)      266 2024-05-03 17:17:48.000000 pgqueuer-0.3.0/test/db/init_db.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-03 17:17:48.000000 pgqueuer-0.3.0/test/test_qm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-05-03 17:17:48.000000 pgqueuer-0.3.0/test/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-03 17:17:48.000000 pgqueuer-0.3.0/test/test_tm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:17:58.038320 pgqueuer-0.3.0/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-03 17:17:48.000000 pgqueuer-0.3.0/tools/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:27:00.316751 pgqueuer-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:27:00.308751 pgqueuer-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:27:00.312751 pgqueuer-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-05 09:27:00.316751 pgqueuer-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 09:27:00.316751 pgqueuer-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:27:00.312751 pgqueuer-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:27:00.312751 pgqueuer-0.3.1/src/PgQueuer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/src/PgQueuer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/src/PgQueuer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/src/PgQueuer/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/src/PgQueuer/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/src/PgQueuer/logconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/src/PgQueuer/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/src/PgQueuer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/src/PgQueuer/qm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16173 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/src/PgQueuer/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/src/PgQueuer/tm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:27:00.316751 pgqueuer-0.3.1/src/PgQueuer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-05 09:27:00.000000 pgqueuer-0.3.1/src/PgQueuer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-05 09:27:00.000000 pgqueuer-0.3.1/src/PgQueuer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 09:27:00.000000 pgqueuer-0.3.1/src/PgQueuer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-05 09:27:00.000000 pgqueuer-0.3.1/src/PgQueuer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-05 09:27:00.000000 pgqueuer-0.3.1/src/PgQueuer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-05 09:27:00.000000 pgqueuer-0.3.1/src/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:27:00.316751 pgqueuer-0.3.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:27:00.316751 pgqueuer-0.3.1/test/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/test/db/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (127)      266 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/test/db/init_db.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/test/test_qm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/test/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/test/test_tm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:27:00.316751 pgqueuer-0.3.1/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-05 09:26:51.000000 pgqueuer-0.3.1/tools/benchmark.py
```

### Comparing `pgqueuer-0.3.0/.github/workflows/ci.yml` & `pgqueuer-0.3.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.0/.github/workflows/linting.yml` & `pgqueuer-0.3.1/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.0/.github/workflows/release.yml` & `pgqueuer-0.3.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.0/.gitignore` & `pgqueuer-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.0/LICENSE` & `pgqueuer-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.0/PKG-INFO` & `pgqueuer-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PgQueuer
-Version: 0.3.0
+Version: 0.3.1
 Summary: PgQueuer is a Python library leveraging PostgreSQL for efficient job queuing.
 Author: janbjorge
 License: MIT License
 Project-URL: Documentation, https://github.com/janbjorge/PgQueuer/
 Project-URL: Homepage, https://github.com/janbjorge/PgQueuer/
 Project-URL: Issues, https://github.com/janbjorge/PgQueuer/issues
 Project-URL: Repository, https://github.com/janbjorge/PgQueuer/
```

### Comparing `pgqueuer-0.3.0/README.md` & `pgqueuer-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.0/pyproject.toml` & `pgqueuer-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.0/src/PgQueuer/cli.py` & `pgqueuer-0.3.1/src/PgQueuer/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 from datetime import timedelta
 
 import asyncpg
 from tabulate import tabulate, tabulate_formats
 
 from PgQueuer.models import LogStatistics
-from PgQueuer.queries import Queries
+from PgQueuer.queries import Queries, QueryBuilder
 
 
 async def display_stats(
     log_stats: list[LogStatistics],
     tablefmt: str,
 ) -> None:
     print(
@@ -138,20 +138,34 @@
         required=True,
     )
 
     subparsers.add_parser(
         "install",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         parents=[common_arguments],
+    ).add_argument(
+        "--dry-run",
+        action="store_true",
+        help=(
+            "Prints the SQL statements that would be executed without actually "
+            " applying any changes to the database."
+        ),
     )
 
     subparsers.add_parser(
         "uninstall",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         parents=[common_arguments],
+    ).add_argument(
+        "--dry-run",
+        action="store_true",
+        help=(
+            "Prints the SQL statements that would be executed without "
+            "actually applying any changes to the database."
+        ),
     )
 
     dashboardparser = subparsers.add_parser(
         "dashboard",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         parents=[common_arguments],
     )
@@ -189,29 +203,35 @@
         "PGQUEUER_PREFIX" not in os.environ
         and isinstance(prefix := parsed.prefix, str)
         and prefix
     ):
         os.environ["PGQUEUER_PREFIX"] = prefix
 
     async with asyncpg.create_pool(
-        parsed.pg_dsn,
+        dsn=parsed.pg_dsn,
         database=parsed.pg_database,
         password=parsed.pg_password,
         port=parsed.pg_port,
         user=parsed.pg_user,
         host=parsed.pg_host,
         max_size=1,
         min_size=0,
     ) as pool:
         queries = Queries(pool)
         match parsed.command:
             case "install":
-                await queries.install()
+                if parsed.dry_run:
+                    print(QueryBuilder().create_install_query())
+                else:
+                    await queries.install()
             case "uninstall":
-                await queries.uninstall()
+                if parsed.dry_run:
+                    print(QueryBuilder().create_uninstall_query())
+                else:
+                    await queries.uninstall()
             case "dashboard":
                 await fetch_and_dispay(
                     queries,
                     parsed.interval,
                     parsed.tail,
                     parsed.table_format,
                 )
```

### Comparing `pgqueuer-0.3.0/src/PgQueuer/models.py` & `pgqueuer-0.3.1/src/PgQueuer/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     """
     Represents the number of jobs per entrypoint and priority in the queue.
     """
 
     count: int
     entrypoint: str
     priority: int
+    status: STATUS
 
 
 class LogStatistics(BaseModel):
     """
     Represents log statistics for jobs based on status, entrypoint, and priority.
     """
```

### Comparing `pgqueuer-0.3.0/src/PgQueuer/qm.py` & `pgqueuer-0.3.1/src/PgQueuer/qm.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,15 +81,18 @@
 
     def __post_init__(self) -> None:
         """
         Initializes database query handlers and validates pool size upon
         instance creation.
         """
         if self.pool.get_min_size() < 1:
-            raise ValueError("... min size must be gt 1.")
+            raise ValueError(
+                "The minimum pool size must be at least 1 to maintain a dedicated "
+                "connection for initialization, setup, and Pub/Sub operations."
+            )
         self.queries = Queries(self.pool)
 
     def entrypoint(self, name: str) -> Callable[[T], T]:
         """
         Registers a function as an entrypoint for handling specific
         job types. Ensures unique naming in the registry.
         """
```

### Comparing `pgqueuer-0.3.0/src/PgQueuer/queries.py` & `pgqueuer-0.3.1/src/PgQueuer/queries.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,174 +19,364 @@
 class DBSettings:
     """
     Stores database settings such as table names and SQL
     function names, dynamically appending prefixes from
     environment variables.
     """
 
+    # Channel name for PostgreSQL LISTEN/NOTIFY used to
+    # receive notifications about changes in the queue.
     channel: Final[str] = dataclasses.field(
         default_factory=lambda: add_prefix("ch_pgqueuer"),
         kw_only=True,
     )
+
+    # Name of the database function triggered by changes to the queue
+    # table, used to notify subscribers.
     function: Final[str] = dataclasses.field(
         default_factory=lambda: add_prefix("fn_pgqueuer_changed"),
         kw_only=True,
     )
+
+    # Name of the table that logs statistics about job processing,
+    # e.g., processing times and outcomes.
     statistics_table: Final[str] = dataclasses.field(
         default_factory=lambda: add_prefix("pgqueuer_statistics"),
     )
+
+    # Type of ENUM defining possible statuses for entries in the
+    # statistics table, such as 'exception' or 'successful'.
     statistics_table_status_type: Final[str] = dataclasses.field(
         default_factory=lambda: add_prefix("pgqueuer_statistics_status"),
         kw_only=True,
     )
+
+    # Type of ENUM defining statuses for queue jobs, such as 'queued' or 'picked'.
     queue_status_type: Final[str] = dataclasses.field(
         default_factory=lambda: add_prefix("pgqueuer_status"),
         kw_only=True,
     )
+
+    # Name of the main table where jobs are queued before being processed.
     queue_table: Final[str] = dataclasses.field(
         default_factory=lambda: add_prefix("pgqueuer"),
         kw_only=True,
     )
+
+    # Name of the trigger that invokes the function to notify changes, applied
+    # after DML operations on the queue table.
     trigger: Final[str] = dataclasses.field(
         default_factory=lambda: add_prefix("tg_pgqueuer_changed"),
         kw_only=True,
     )
 
 
 @dataclasses.dataclass
+class QueryBuilder:
+    """
+    Generates SQL queries for job queuing operations.
+    """
+
+    settings: DBSettings = dataclasses.field(default_factory=DBSettings)
+
+    def create_install_query(self) -> str:
+        """
+        Generates the SQL query string to create necessary database objects for
+        the job queue system.
+
+        This includes:
+
+        - Enums for job statuses (e.g., 'queued', 'picked') and log statuses
+            (e.g., 'exception', 'successful').
+        - Tables for storing job queue data and log statistics with appropriate fields
+            such as job ID,
+          priority, status, entrypoint, and payload.
+        - Indexes to improve the performance of querying these tables.
+        - A trigger function that emits notifications upon changes to the
+            job queue table, facilitating real-time update mechanisms using
+            PostgreSQL's LISTEN/NOTIFY system.
+        """
+
+        return f"""
+    CREATE TYPE {self.settings.queue_status_type} AS ENUM ('queued', 'picked');
+    CREATE TABLE {self.settings.queue_table} (
+        id SERIAL PRIMARY KEY,
+        priority INT NOT NULL,
+        created TIMESTAMP WITH TIME ZONE DEFAULT CURRENT_TIMESTAMP,
+        status {self.settings.queue_status_type} NOT NULL,
+        entrypoint TEXT NOT NULL,
+        payload BYTEA
+    );
+    CREATE INDEX ON {self.settings.queue_table} (priority ASC, id DESC)
+        INCLUDE (id) WHERE status = 'queued';
+
+    CREATE TYPE {self.settings.statistics_table_status_type} AS ENUM ('exception', 'successful');
+    CREATE TABLE {self.settings.statistics_table} (
+        id SERIAL PRIMARY KEY,
+        created TIMESTAMP WITH TIME ZONE NOT NULL DEFAULT DATE_TRUNC('sec', CURRENT_TIMESTAMP at time zone 'UTC'),
+        count BIGINT NOT NULL,
+        priority INT NOT NULL,
+        time_in_queue INTERVAL NOT NULL,
+        status {self.settings.statistics_table_status_type} NOT NULL,
+        entrypoint TEXT NOT NULL
+    );
+    CREATE UNIQUE INDEX unique_count ON {self.settings.statistics_table} (
+        priority,
+        DATE_TRUNC('sec', created at time zone 'UTC'),
+        DATE_TRUNC('sec', time_in_queue),
+        status,
+        entrypoint
+    );
+
+    CREATE FUNCTION {self.settings.function}() RETURNS TRIGGER AS $$
+    DECLARE
+        to_emit BOOLEAN := false;  -- Flag to decide whether to emit a notification
+    BEGIN
+        -- Check operation type and set the emit flag accordingly
+        IF TG_OP = 'UPDATE' AND OLD IS DISTINCT FROM NEW THEN
+            to_emit := true;
+        ELSIF TG_OP = 'DELETE' THEN
+            to_emit := true;
+        ELSIF TG_OP = 'INSERT' THEN
+            to_emit := true;
+        ELSIF TG_OP = 'TRUNCATE' THEN
+            to_emit := true;
+        END IF;
+
+        -- Perform notification if the emit flag is set
+        IF to_emit THEN
+            PERFORM pg_notify(
+                '{self.settings.channel}',
+                json_build_object(
+                    'channel', '{self.settings.channel}',
+                    'operation', lower(TG_OP),
+                    'sent_at', NOW(),
+                    'table', TG_TABLE_NAME
+                )::text
+            );
+        END IF;
+
+        -- Return appropriate value based on the operation
+        IF TG_OP IN ('INSERT', 'UPDATE') THEN
+            RETURN NEW;
+        ELSIF TG_OP = 'DELETE' THEN
+            RETURN OLD;
+        ELSE
+            RETURN NULL; -- For TRUNCATE and other non-row-specific contexts
+        END IF;
+
+    END;
+    $$ LANGUAGE plpgsql;
+
+    CREATE TRIGGER {self.settings.trigger}
+    AFTER INSERT OR UPDATE OR DELETE OR TRUNCATE ON {self.settings.queue_table}
+    EXECUTE FUNCTION {self.settings.function}();
+        """  # noqa: E501
+
+    def create_uninstall_query(self) -> str:
+        """
+        Generates the SQL query string to remove all database structures
+        related to the job queue system.
+        """
+
+        return f"""
+    DROP TRIGGER {self.settings.trigger};
+    DROP FUNCTION {self.settings.function};
+    DROP TABLE {self.settings.queue_table};
+    DROP TABLE {self.settings.statistics_table};
+    DROP TYPE {self.settings.queue_status_type};
+    DROP TYPE {self.settings.statistics_table_status_type};
+    """
+
+    def create_dequeue_query(self) -> str:
+        """
+        Generates the SQL query string to insert a new job into the queue.
+        This query sets the job status to 'queued' and includes parameters for priority,
+        entrypoint, and payload.
+        """
+        return f"""
+    WITH next_job AS (
+        SELECT id
+        FROM {self.settings.queue_table}
+        WHERE status = 'queued'
+        ORDER BY priority DESC, id ASC
+        FOR UPDATE SKIP LOCKED
+        LIMIT 1
+    )
+    UPDATE {self.settings.queue_table}
+    SET status = 'picked'
+    WHERE id = ANY(SELECT id FROM next_job)
+    RETURNING *;
+    """
+
+    def create_enqueue_query(self) -> str:
+        """
+        Generates the SQL query string to insert a new job into the queue.
+        This query sets the job status to 'queued' and includes parameters for priority,
+        entrypoint, and payload.
+        """
+        return f"""
+    INSERT INTO {self.settings.queue_table} (priority, status, entrypoint, payload)
+    VALUES ($1, 'queued', $2, $3)
+    """  # noqa: E501
+
+    def create_delete_from_queue_query(self) -> str:
+        """
+        Generates the SQL query string to delete jobs from the queue based on a
+        list of entrypoints. This query uses the ANY clause to match any of the
+        specified entrypoints for deletion.
+        """
+        return f"DELETE FROM {self.settings.queue_table} WHERE entrypoint = ANY($1)"
+
+    def create_truncate_queue_query(self) -> str:
+        """
+        Generates the SQL query string to truncate the job queue table,
+        effectively removing all jobs from the queue.
+        """
+        return f"TRUNCATE {self.settings.queue_table}"
+
+    def create_queue_size_query(self) -> str:
+        """
+        Generates the SQL query string to count the number of jobs in the queue,
+        grouped by entrypoint and priority. This helps in understanding the distribution
+        of jobs across different priorities and entrypoints.
+        """
+        return f"""
+    SELECT
+        count(*) AS count,
+        priority,
+        entrypoint,
+        status
+    FROM
+        {self.settings.queue_table}
+    GROUP BY entrypoint, priority, status
+    ORDER BY count, entrypoint, priority, status
+    """
+
+    def create_log_job_query(self) -> str:
+        """
+        Generates the SQL query string to move a completed or failed job from the
+        queue table to the log table, capturing details like job priority,
+        entrypoint, time in queue, creation time, and final status.
+        """
+        return f"""
+    WITH deleted AS (
+        DELETE FROM {self.settings.queue_table}
+        WHERE id = $1
+    )
+
+    INSERT INTO {self.settings.statistics_table} (
+        priority,
+        entrypoint,
+        time_in_queue,
+        created,
+        status,
+        count
+    )
+    VALUES (
+        $2,                                         -- priority
+        $3,                                         -- entrypoint
+        DATE_TRUNC('sec', NOW() - $4),              -- time_in_queue
+        DATE_TRUNC('sec', $4 at time zone 'UTC'),   -- created at time zone 'UTC'
+        $5,                                         -- status
+        1                                           -- start count
+    )
+    ON CONFLICT (
+        priority,
+        entrypoint,
+        DATE_TRUNC('sec', created at time zone 'UTC'),
+        DATE_TRUNC('sec', time_in_queue),
+        status
+    )
+    DO UPDATE
+        SET
+            count = {self.settings.statistics_table}.count + 1
+        WHERE
+                {self.settings.statistics_table}.priority = $2
+            AND {self.settings.statistics_table}.entrypoint = $3
+            AND DATE_TRUNC('sec', {self.settings.statistics_table}.time_in_queue) = DATE_TRUNC('sec', NOW() - $4)
+            AND DATE_TRUNC('sec', {self.settings.statistics_table}.created) = DATE_TRUNC('sec', $4 at time zone 'UTC')
+            AND {self.settings.statistics_table}.status = $5
+    """  # noqa: E501
+
+    def create_truncate_log_query(self) -> str:
+        """
+        Generates the SQL query string to truncate the job log table,
+        effectively removing all logged entries.
+        """
+        return f"""TRUNCATE {self.settings.statistics_table}"""
+
+    def create_delete_from_log_query(self) -> str:
+        """
+        Generates the SQL query string to delete entries from the job log table,
+        optionally filtered by a list of entrypoints. This allows selective clearing
+        of log entries based on their source entrypoints.
+        """
+        return f"""
+    DELETE FROM {self.settings.statistics_table}
+    WHERE entrypoint = ANY($1)
+    """
+
+    def create_log_statistics_query(self) -> str:
+        """
+        Generates the SQL query string to retrieve statistical data from the job
+        log table, including count of jobs, creation time, time in queue,
+        entrypoint, priority, and status, limited to a specified number of most
+        recent records defined by 'tail'.
+        """
+        return f"""
+    SELECT
+        count,
+        created,
+        time_in_queue,
+        entrypoint,
+        priority,
+        status
+    FROM {self.settings.statistics_table}
+    ORDER BY (
+        id, created, count, time_in_queue,
+        entrypoint, priority, status
+    ) DESC
+    LIMIT $1
+    """
+
+
+@dataclasses.dataclass
 class Queries:
     """
     Handles operations related to job queuing such as
     enqueueing, dequeueing, and querying the size of the queue.
     """
 
     pool: asyncpg.Pool
-    settings: DBSettings = dataclasses.field(default_factory=DBSettings)
+    qb: QueryBuilder = dataclasses.field(default_factory=QueryBuilder)
 
     async def install(self) -> None:
         """
         Creates necessary database structures such as enums,
         tables, and triggers for job queuing and logging.
         """
 
-        query = f"""
-            CREATE TYPE {self.settings.queue_status_type} AS ENUM ('queued', 'picked');
-            CREATE TABLE {self.settings.queue_table} (
-                id SERIAL PRIMARY KEY,
-                priority INT NOT NULL,
-                created TIMESTAMP WITH TIME ZONE DEFAULT CURRENT_TIMESTAMP,
-                status {self.settings.queue_status_type} NOT NULL,
-                entrypoint TEXT NOT NULL,
-                payload BYTEA
-            );
-            CREATE INDEX ON {self.settings.queue_table} (priority ASC, id DESC)
-                INCLUDE (id) WHERE status = 'queued';
-
-            CREATE TYPE {self.settings.statistics_table_status_type} AS ENUM ('exception', 'successful');
-            CREATE TABLE {self.settings.statistics_table} (
-                id SERIAL PRIMARY KEY,
-                created TIMESTAMP WITH TIME ZONE NOT NULL DEFAULT DATE_TRUNC('sec', CURRENT_TIMESTAMP at time zone 'UTC'),
-                count BIGINT NOT NULL,
-                priority INT NOT NULL,
-                time_in_queue INTERVAL NOT NULL,
-                status {self.settings.statistics_table_status_type} NOT NULL,
-                entrypoint TEXT NOT NULL
-            );
-            CREATE UNIQUE INDEX unique_count ON {self.settings.statistics_table} (
-                priority,
-                DATE_TRUNC('sec', created at time zone 'UTC'),
-                DATE_TRUNC('sec', time_in_queue),
-                status,
-                entrypoint
-            );
-
-            CREATE FUNCTION {self.settings.function}() RETURNS TRIGGER AS $$
-            DECLARE
-                to_emit BOOLEAN := false;  -- Flag to decide whether to emit a notification
-            BEGIN
-                -- Check operation type and set the emit flag accordingly
-                IF TG_OP = 'UPDATE' AND OLD IS DISTINCT FROM NEW THEN
-                    to_emit := true;
-                ELSIF TG_OP = 'DELETE' THEN
-                    to_emit := true;
-                ELSIF TG_OP = 'INSERT' THEN
-                    to_emit := true;
-                ELSIF TG_OP = 'TRUNCATE' THEN
-                    to_emit := true;
-                END IF;
-
-                -- Perform notification if the emit flag is set
-                IF to_emit THEN
-                    PERFORM pg_notify(
-                        '{self.settings.channel}',
-                        json_build_object(
-                            'channel', '{self.settings.channel}',
-                            'operation', lower(TG_OP),
-                            'sent_at', NOW(),
-                            'table', TG_TABLE_NAME
-                        )::text
-                    );
-                END IF;
-
-                -- Return appropriate value based on the operation
-                IF TG_OP IN ('INSERT', 'UPDATE') THEN
-                    RETURN NEW;
-                ELSIF TG_OP = 'DELETE' THEN
-                    RETURN OLD;
-                ELSE
-                    RETURN NULL; -- For TRUNCATE and other non-row-specific contexts
-                END IF;
-
-            END;
-            $$ LANGUAGE plpgsql;
-
-            CREATE TRIGGER {self.settings.trigger}
-            AFTER INSERT OR UPDATE OR DELETE OR TRUNCATE ON {self.settings.queue_table}
-            EXECUTE FUNCTION {self.settings.function}();
-        """  # noqa: E501
-
-        await self.pool.execute(query)
+        await self.pool.execute(self.qb.create_install_query())
 
     async def uninstall(self) -> None:
         """
         Drops all database structures related to job queuing
         and logging that were created by the install method.
         """
-        query = f"""
-            DROP TRIGGER {self.settings.trigger};
-            DROP FUNCTION {self.settings.function};
-            DROP TABLE {self.settings.queue_table};
-            DROP TABLE {self.settings.statistics_table};
-            DROP TYPE {self.settings.queue_status_type};
-            DROP TYPE {self.settings.statistics_table_status_type};
-        """
-        await self.pool.execute(query)
+        await self.pool.execute(self.qb.create_uninstall_query())
 
     async def dequeue(self) -> models.Job | None:
         """
         Retrieves and updates the next 'queued' job to 'picked'
         status, ensuring no two jobs with the same entrypoint
         are picked simultaneously.
         """
-        query = f"""
-            WITH next_job AS (
-                SELECT id
-                FROM {self.settings.queue_table}
-                WHERE status = 'queued'
-                ORDER BY priority DESC, id ASC
-                FOR UPDATE SKIP LOCKED
-                LIMIT 1
-            )
-            UPDATE {self.settings.queue_table}
-            SET status = 'picked'
-            WHERE id = ANY(SELECT id FROM next_job)
-            RETURNING *;
-        """
 
-        if row := await self.pool.fetchrow(query):
+        if row := await self.pool.fetchrow(self.qb.create_dequeue_query()):
             return models.Job.model_validate(dict(row))
         return None
 
     async def enqueue(
         self,
         entrypoint: str | list[str],
         payload: bytes | None | list[bytes] | list[None] | list[bytes | None],
@@ -203,151 +393,72 @@
         """
 
         # If they are not lists, create single-item lists for uniform processing
         normed_entrypoint = entrypoint if isinstance(entrypoint, list) else [entrypoint]
         normed_payload = payload if isinstance(payload, list) else [payload]
         normed_priority = priority if isinstance(priority, list) else [priority]
 
-        query = f"""
-            INSERT INTO {self.settings.queue_table} (priority, status, entrypoint, payload)
-            VALUES ($1, 'queued', $2, $3)
-        """  # noqa: E501
-
         await self.pool.executemany(
-            query,
+            self.qb.create_enqueue_query(),
             zip(
                 normed_priority,
                 normed_entrypoint,
                 normed_payload,
                 strict=True,
             ),
         )
 
     async def clear_queue(self, entrypoint: str | list[str] | None = None) -> None:
         """
         Clears jobs from the queue, optionally filtering by entrypoint if specified.
         """
-        if entrypoint:
-            query = (
-                f"DELETE FROM {self.settings.queue_table} WHERE entrypoint = ANY($1)"
-            )
-            await self.pool.execute(
-                query,
+        await (
+            self.pool.execute(
+                self.qb.create_delete_from_queue_query(),
                 [entrypoint] if isinstance(entrypoint, str) else entrypoint,
             )
-        else:
-            query = f"TRUNCATE {self.settings.queue_table}"
-            await self.pool.execute(query)
+            if entrypoint
+            else self.pool.execute(self.qb.create_truncate_queue_query())
+        )
 
     async def queue_size(self) -> list[models.QueueStatistics]:
         """
         Returns the number of jobs in the queue grouped by entrypoint and priority.
         """
-        query = f"""
-            SELECT
-                count(*) AS count,
-                priority,
-                entrypoint
-            FROM
-                {self.settings.queue_table}
-            GROUP BY entrypoint, priority
-            ORDER BY count, entrypoint, priority
-        """
         return [
             models.QueueStatistics.model_validate(dict(x))
-            for x in await self.pool.fetch(query)
+            for x in await self.pool.fetch(self.qb.create_queue_size_query())
         ]
 
     async def log_job(self, job: models.Job, status: models.STATUS_LOG) -> None:
         """
         Moves a completed or failed job from the queue table to the log
         table, recording its final status and duration.
         """
-
-        query = f"""
-            WITH deleted AS (
-                DELETE FROM {self.settings.queue_table}
-                WHERE id = $1
-            )
-
-            INSERT INTO {self.settings.statistics_table} (
-                priority,
-                entrypoint,
-                time_in_queue,
-                created,
-                status,
-                count
-            )
-            VALUES (
-                $2,                                         -- priority
-                $3,                                         -- entrypoint
-                DATE_TRUNC('sec', NOW() - $4),              -- time_in_queue
-                DATE_TRUNC('sec', $4 at time zone 'UTC'),   -- created at time zone 'UTC'
-                $5,                                         -- status
-                1                                           -- start count
-            )
-            ON CONFLICT (
-                priority,
-                entrypoint,
-                DATE_TRUNC('sec', created at time zone 'UTC'),
-                DATE_TRUNC('sec', time_in_queue),
-                status
-            )
-            DO UPDATE
-                SET
-                    count = {self.settings.statistics_table}.count + 1
-                WHERE
-                        {self.settings.statistics_table}.priority = $2
-                    AND DATE_TRUNC('sec', {self.settings.statistics_table}.time_in_queue) = DATE_TRUNC('sec', NOW() - $4)
-                    AND DATE_TRUNC('sec', {self.settings.statistics_table}.created) = DATE_TRUNC('sec', $4 at time zone 'UTC')
-                    AND {self.settings.statistics_table}.status = $5
-                    AND {self.settings.statistics_table}.entrypoint = $3
-
-         """  # noqa: E501
-
         await self.pool.execute(
-            query,
+            self.qb.create_log_job_query(),
             job.id,
             job.priority,
             job.entrypoint,
             job.created,
             status,
         )
 
     async def clear_log(self, entrypoint: str | list[str] | None = None) -> None:
         """
         Clears entries from the job log table, optionally filtering
         by entrypoint if specified.
         """
-        if entrypoint:
-            query = f"""
-                DELETE FROM {self.settings.statistics_table}
-                WHERE entrypoint = ANY($1)
-            """
-            await self.pool.execute(
-                query,
+        await (
+            self.pool.execute(
+                self.qb.create_delete_from_log_query(),
                 [entrypoint] if isinstance(entrypoint, str) else entrypoint,
             )
-        else:
-            query = f"TRUNCATE {self.settings.statistics_table}"
-            await self.pool.execute(query)
+            if entrypoint
+            else self.pool.execute(self.qb.create_truncate_log_query())
+        )
 
     async def log_statistics(self, tail: int) -> list[models.LogStatistics]:
-        query = f"""
-            SELECT
-                count,
-                created,
-                time_in_queue,
-                entrypoint,
-                priority,
-                status
-            FROM {self.settings.statistics_table}
-            ORDER BY (
-                id, created, count, time_in_queue,
-                entrypoint, priority, status
-            ) DESC
-            LIMIT $1
-        """
         return [
             models.LogStatistics.model_validate(dict(x))
-            for x in await self.pool.fetch(query, tail)
+            for x in await self.pool.fetch(self.qb.create_log_statistics_query(), tail)
         ]
```

### Comparing `pgqueuer-0.3.0/src/PgQueuer/tm.py` & `pgqueuer-0.3.1/src/PgQueuer/tm.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.0/src/PgQueuer.egg-info/PKG-INFO` & `pgqueuer-0.3.1/src/PgQueuer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PgQueuer
-Version: 0.3.0
+Version: 0.3.1
 Summary: PgQueuer is a Python library leveraging PostgreSQL for efficient job queuing.
 Author: janbjorge
 License: MIT License
 Project-URL: Documentation, https://github.com/janbjorge/PgQueuer/
 Project-URL: Homepage, https://github.com/janbjorge/PgQueuer/
 Project-URL: Issues, https://github.com/janbjorge/PgQueuer/issues
 Project-URL: Repository, https://github.com/janbjorge/PgQueuer/
```

### Comparing `pgqueuer-0.3.0/src/PgQueuer.egg-info/SOURCES.txt` & `pgqueuer-0.3.1/src/PgQueuer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.0/test/conftest.py` & `pgqueuer-0.3.1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.0/test/db/Dockerfile` & `pgqueuer-0.3.1/test/db/Dockerfile`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.0/test/test_qm.py` & `pgqueuer-0.3.1/test/test_qm.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.0/test/test_queries.py` & `pgqueuer-0.3.1/test/test_queries.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.0/test/test_tm.py` & `pgqueuer-0.3.1/test/test_tm.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.0/tools/benchmark.py` & `pgqueuer-0.3.1/tools/benchmark.py`

 * *Files identical despite different names*

