# Comparing `tmp/sqlexecutorx-0.0.3.tar.gz` & `tmp/sqlexecutorx-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlexecutorx-0.0.3.tar", last modified: Sat May  4 04:09:50 2024, max compression
+gzip compressed data, was "sqlexecutorx-0.0.5.tar", last modified: Sat May  4 08:21:48 2024, max compression
```

## Comparing `sqlexecutorx-0.0.3.tar` & `sqlexecutorx-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-04 04:09:50.159429 sqlexecutorx-0.0.3/
--rw-rw-r--   0 summy      (501) staff       (20)    11357 2024-03-14 05:16:15.000000 sqlexecutorx-0.0.3/LICENSE
--rw-r--r--   0 summy      (501) staff       (20)     2031 2024-05-04 04:09:50.157095 sqlexecutorx-0.0.3/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)     1577 2024-05-04 03:23:13.000000 sqlexecutorx-0.0.3/README.rst
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-04 04:09:50.160225 sqlexecutorx-0.0.3/setup.cfg
--rw-rw-r--   0 summy      (501) staff       (20)     1172 2024-05-04 04:09:43.000000 sqlexecutorx-0.0.3/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-04 04:09:50.145826 sqlexecutorx-0.0.3/sqlexecutorx/
--rw-rw-r--   0 summy      (501) staff       (20)      903 2024-05-04 04:09:24.000000 sqlexecutorx-0.0.3/sqlexecutorx/__init__.py
--rw-rw-r--   0 summy      (501) staff       (20)      209 2024-05-04 03:22:15.000000 sqlexecutorx-0.0.3/sqlexecutorx/constant.py
--rw-rw-r--   0 summy      (501) staff       (20)    11253 2024-05-04 04:09:24.000000 sqlexecutorx-0.0.3/sqlexecutorx/core.py
--rw-r--r--   0 summy      (501) staff       (20)      901 2024-03-23 15:57:10.000000 sqlexecutorx-0.0.3/sqlexecutorx/engine.py
--rw-rw-r--   0 summy      (501) staff       (20)     2042 2024-03-23 16:12:52.000000 sqlexecutorx-0.0.3/sqlexecutorx/init_import.py
--rw-rw-r--   0 summy      (501) staff       (20)      740 2024-03-25 03:02:59.000000 sqlexecutorx-0.0.3/sqlexecutorx/log_support.py
--rw-rw-r--   0 summy      (501) staff       (20)     1031 2024-05-04 03:22:15.000000 sqlexecutorx-0.0.3/sqlexecutorx/pooling.py
--rw-r--r--   0 summy      (501) staff       (20)      422 2024-03-29 05:50:43.000000 sqlexecutorx-0.0.3/sqlexecutorx/sql_support.py
--rw-rw-r--   0 summy      (501) staff       (20)     3892 2024-03-25 02:25:33.000000 sqlexecutorx-0.0.3/sqlexecutorx/support.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-04 04:09:50.154914 sqlexecutorx-0.0.3/sqlexecutorx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)     2031 2024-05-04 04:09:50.000000 sqlexecutorx-0.0.3/sqlexecutorx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      432 2024-05-04 04:09:50.000000 sqlexecutorx-0.0.3/sqlexecutorx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-04 04:09:50.000000 sqlexecutorx-0.0.3/sqlexecutorx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-04 03:23:57.000000 sqlexecutorx-0.0.3/sqlexecutorx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)       13 2024-05-04 04:09:50.000000 sqlexecutorx-0.0.3/sqlexecutorx.egg-info/top_level.txt
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-04 08:21:48.449402 sqlexecutorx-0.0.5/
+-rw-rw-r--   0 summy      (501) staff       (20)    11357 2024-03-14 05:16:15.000000 sqlexecutorx-0.0.5/LICENSE
+-rw-r--r--   0 summy      (501) staff       (20)     2031 2024-05-04 08:21:48.446714 sqlexecutorx-0.0.5/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)     1577 2024-05-04 03:23:13.000000 sqlexecutorx-0.0.5/README.rst
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-04 08:21:48.450069 sqlexecutorx-0.0.5/setup.cfg
+-rw-rw-r--   0 summy      (501) staff       (20)     1172 2024-05-04 08:21:33.000000 sqlexecutorx-0.0.5/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-04 08:21:48.437463 sqlexecutorx-0.0.5/sqlexecutorx/
+-rw-rw-r--   0 summy      (501) staff       (20)      903 2024-05-04 04:09:24.000000 sqlexecutorx-0.0.5/sqlexecutorx/__init__.py
+-rw-rw-r--   0 summy      (501) staff       (20)      209 2024-05-04 03:22:15.000000 sqlexecutorx-0.0.5/sqlexecutorx/constant.py
+-rw-rw-r--   0 summy      (501) staff       (20)    11271 2024-05-04 08:21:00.000000 sqlexecutorx-0.0.5/sqlexecutorx/core.py
+-rw-r--r--   0 summy      (501) staff       (20)      901 2024-03-23 15:57:10.000000 sqlexecutorx-0.0.5/sqlexecutorx/engine.py
+-rw-rw-r--   0 summy      (501) staff       (20)     2042 2024-03-23 16:12:52.000000 sqlexecutorx-0.0.5/sqlexecutorx/init_import.py
+-rw-rw-r--   0 summy      (501) staff       (20)      740 2024-03-25 03:02:59.000000 sqlexecutorx-0.0.5/sqlexecutorx/log_support.py
+-rw-rw-r--   0 summy      (501) staff       (20)     1031 2024-05-04 03:22:15.000000 sqlexecutorx-0.0.5/sqlexecutorx/pooling.py
+-rw-r--r--   0 summy      (501) staff       (20)      422 2024-03-29 05:50:43.000000 sqlexecutorx-0.0.5/sqlexecutorx/sql_support.py
+-rw-rw-r--   0 summy      (501) staff       (20)     3892 2024-03-25 02:25:33.000000 sqlexecutorx-0.0.5/sqlexecutorx/support.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-04 08:21:48.445452 sqlexecutorx-0.0.5/sqlexecutorx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)     2031 2024-05-04 08:21:48.000000 sqlexecutorx-0.0.5/sqlexecutorx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      432 2024-05-04 08:21:48.000000 sqlexecutorx-0.0.5/sqlexecutorx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-04 08:21:48.000000 sqlexecutorx-0.0.5/sqlexecutorx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-04 03:23:57.000000 sqlexecutorx-0.0.5/sqlexecutorx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)       13 2024-05-04 08:21:48.000000 sqlexecutorx-0.0.5/sqlexecutorx.egg-info/top_level.txt
```

### Comparing `sqlexecutorx-0.0.3/LICENSE` & `sqlexecutorx-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlexecutorx-0.0.3/PKG-INFO` & `sqlexecutorx-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlexecutorx
-Version: 0.0.3
+Version: 0.0.5
 Summary: A simple thread safe sql sqlexecutorx for Python with connection pool. Support MySQL, PostgreSQL, SQLite etc.
 Home-page: https://gitee.com/summry/sqlexecutorx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Database,Python,RDB
 Platform: UNKNOWN
```

### Comparing `sqlexecutorx-0.0.3/README.rst` & `sqlexecutorx-0.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `sqlexecutorx-0.0.3/setup.py` & `sqlexecutorx-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 setup(
     name='sqlexecutorx',
     packages=['sqlexecutorx'],
     description="A simple thread safe sql sqlexecutorx for Python with connection pool. Support MySQL, PostgreSQL, SQLite etc.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.0.3',
+    version='0.0.5',
     url='https://gitee.com/summry/sqlexecutorx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['SQL', 'MySQL', 'PostgreSQL', 'SQLite', 'Database', 'Python', 'RDB'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlexecutorx-0.0.3/sqlexecutorx/__init__.py` & `sqlexecutorx-0.0.5/sqlexecutorx/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlexecutorx-0.0.3/sqlexecutorx/core.py` & `sqlexecutorx-0.0.5/sqlexecutorx/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -98,14 +98,15 @@
     --------
     >>> from sqlexecutorx import with_connection
     >>> @with_connection
     >>> def foo(*args, **kw):
     >>>     f1()
     >>>     f2()
     """
+
     global _DB_CTX
 
     @functools.wraps(func)
     def _wrapper(*args, **kw):
         with ConnectionCtx(_DB_CTX):
             return func(*args, **kw)
     return _wrapper
@@ -120,14 +121,15 @@
     >>> from sqlexecutorx import with_connection
     >>> with transaction():
     >>>     pass
     >>> with transaction():
     >>>      insert(...)
     >>>      update(... )
     """
+
     global _DB_CTX
     return TransactionCtx(_DB_CTX)
 
 
 def with_transaction(func):
     """
     A decorator that makes function around transaction.
@@ -170,22 +172,23 @@
         _DB_CTX = None
 
 
 @with_connection
 def execute(sql: str, *args):
     """
     Execute sql return effect rowcount
+
     :param sql: SQL
     :param args:
     :return: Effect rowcount
 
     Examples
     --------
     >>> import sqlexecutorx as db
-    >>> sql = 'insert into person(name, age) values(%s, %s)'
+    >>> sql = 'INSERT INTO person(name, age) VALUES(%s, %s)'
     >>> db.execute(sql, '张三', 20)
     1
     """
 
     global _DB_CTX
     global _SHOW_SQL
     cursor = None
@@ -202,23 +205,24 @@
             cursor.close()
 
 
 @with_connection
 def save(select_key: str, sql: str, *args):
     """
     Execute sql return primary key
+
     :param select_key:
     :param sql: SQL
     :param args:
     :return: Primary key
 
     Examples
     --------
     >>> import sqlexecutorx as db
-    >>> sql = 'insert into person(name, age) values(%s, %s)'
+    >>> sql = 'INSERT INTO person(name, age) VALUES(%s, %s)'
     >>> db.save('SELECT LAST_INSERT_ID()', sql, '张三', 20)
     3
     """
 
     global _DB_CTX
     global _SHOW_SQL
     cursor = None
@@ -240,15 +244,15 @@
     """
     Execute select SQL and expected one int and only one int result, SQL contain 'limit'.
     MultiColumnsError: Expect only one column.
 
     Examples
     --------
     >>> import sqlexecutorx as db
-    >>> sql = 'SELECT count(1) FROM person WHERE name=%s and age=%s limit 1'
+    >>> sql = 'SELECT count(1) FROM person WHERE name=%s and age=%s LIMIT 1'
     >>> db.get(sql, '张三', 20)
     1
     """
 
     result = select_one(sql, *args)
     if result:
         if len(result) == 1:
@@ -272,15 +276,15 @@
 
 
 def select_one(sql: str, *args):
     """
     Examples
     --------
     >>> import sqlexecutorx as db
-    >>> sql = 'SELECT id, name, age FROM person WHERE name=%s and age=%s limit 1'
+    >>> sql = 'SELECT id, name, age FROM person WHERE name=%s and age=%s LIMIT 1'
     >>> db.select_one(sql, '张三', 20)
     (3, '张三', 20)
     """
     return do_select_one(sql, *args)[0]
 
 
 def query(sql: str, *args):
@@ -304,15 +308,15 @@
 def query_one(sql: str, *args):
     """
     Execute select SQL and return unique result(dict), SQL contain 'limit'.
 
     Examples
     --------
     >>> import sqlexecutorx as db
-    >>> sql = 'SELECT id, name, age FROM person WHERE name=%s and age=%s limit 1'
+    >>> sql = 'SELECT id, name, age FROM person WHERE name=%s and age=%s LIMIT 1'
     >>> db.query_one(sql, '张三', 20)
     {'id': 3, 'name': '张三', 'age': 20}
     """
 
     result, description = do_select_one(sql, *args)
     if result and description:
         names = list(map(lambda x: x[0], description))
@@ -379,24 +383,25 @@
         if cursor:
             cursor.close()
 
 
 @with_connection
 def batch_execute(sql: str, *args):
     """
-    Batch execute sql return effect rowcount
-    :param sql: SQL
+    Batch execute sql return effected rowcount
+
+    :param sql: SQL to execute
     :param args: All number must have same size.
     :return: Effect rowcount
 
     Examples
     --------
     >>> import sqlexecutorx as db
     >>> args = [('张三', 20), ('李四', 28)]
-    >>> sql = 'insert into person(name, age) values(%s, %s)'
+    >>> sql = 'INSERT INTO person(name, age) VALUES(%s, %s)'
     >>> db.batch_execute(sql, *args)
     2
     """
 
     global _DB_CTX
     global _SHOW_SQL
     cursor = None
```

### Comparing `sqlexecutorx-0.0.3/sqlexecutorx/engine.py` & `sqlexecutorx-0.0.5/sqlexecutorx/engine.py`

 * *Files identical despite different names*

### Comparing `sqlexecutorx-0.0.3/sqlexecutorx/init_import.py` & `sqlexecutorx-0.0.5/sqlexecutorx/init_import.py`

 * *Files identical despite different names*

### Comparing `sqlexecutorx-0.0.3/sqlexecutorx/log_support.py` & `sqlexecutorx-0.0.5/sqlexecutorx/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlexecutorx-0.0.3/sqlexecutorx/pooling.py` & `sqlexecutorx-0.0.5/sqlexecutorx/pooling.py`

 * *Files identical despite different names*

### Comparing `sqlexecutorx-0.0.3/sqlexecutorx/support.py` & `sqlexecutorx-0.0.5/sqlexecutorx/support.py`

 * *Files identical despite different names*

### Comparing `sqlexecutorx-0.0.3/sqlexecutorx.egg-info/PKG-INFO` & `sqlexecutorx-0.0.5/sqlexecutorx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlexecutorx
-Version: 0.0.3
+Version: 0.0.5
 Summary: A simple thread safe sql sqlexecutorx for Python with connection pool. Support MySQL, PostgreSQL, SQLite etc.
 Home-page: https://gitee.com/summry/sqlexecutorx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Database,Python,RDB
 Platform: UNKNOWN
```

