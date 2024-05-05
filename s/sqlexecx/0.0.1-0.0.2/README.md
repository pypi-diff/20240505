# Comparing `tmp/sqlexecx-0.0.1.tar.gz` & `tmp/sqlexecx-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlexecx-0.0.1.tar", last modified: Sat May  4 04:37:36 2024, max compression
+gzip compressed data, was "sqlexecx-0.0.2.tar", last modified: Sat May  4 09:35:30 2024, max compression
```

## Comparing `sqlexecx-0.0.1.tar` & `sqlexecx-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-04 04:37:36.093242 sqlexecx-0.0.1/
--rw-r--r--   0 summy      (501) staff       (20)    11357 2024-01-23 07:49:56.000000 sqlexecx-0.0.1/LICENSE
--rw-r--r--   0 summy      (501) staff       (20)     7491 2024-05-04 04:37:36.091309 sqlexecx-0.0.1/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)     6974 2024-03-29 02:19:13.000000 sqlexecx-0.0.1/README.rst
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-04 04:37:36.093515 sqlexecx-0.0.1/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1297 2024-05-04 04:37:27.000000 sqlexecx-0.0.1/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-04 04:37:36.078645 sqlexecx-0.0.1/sqlexecx/
--rw-r--r--   0 summy      (501) staff       (20)     1841 2024-05-04 04:35:20.000000 sqlexecx-0.0.1/sqlexecx/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)      641 2024-04-26 08:01:55.000000 sqlexecx-0.0.1/sqlexecx/constant.py
--rw-r--r--   0 summy      (501) staff       (20)     8883 2024-05-04 04:35:51.000000 sqlexecx-0.0.1/sqlexecx/dialect.py
--rw-r--r--   0 summy      (501) staff       (20)    14036 2024-05-04 04:35:42.000000 sqlexecx-0.0.1/sqlexecx/exec.py
--rw-r--r--   0 summy      (501) staff       (20)     1936 2024-04-25 04:18:32.000000 sqlexecx-0.0.1/sqlexecx/loader.py
--rw-r--r--   0 summy      (501) staff       (20)      822 2024-05-04 04:35:42.000000 sqlexecx-0.0.1/sqlexecx/log_support.py
--rw-r--r--   0 summy      (501) staff       (20)     1933 2024-03-27 08:41:08.000000 sqlexecx-0.0.1/sqlexecx/page_exec.py
--rw-r--r--   0 summy      (501) staff       (20)    12135 2024-05-04 04:35:20.000000 sqlexecx-0.0.1/sqlexecx/sql_exec.py
--rw-r--r--   0 summy      (501) staff       (20)     3076 2024-05-04 04:36:08.000000 sqlexecx-0.0.1/sqlexecx/sql_support.py
--rw-r--r--   0 summy      (501) staff       (20)    18462 2024-05-04 04:35:20.000000 sqlexecx-0.0.1/sqlexecx/table_exec.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-04 04:37:36.088818 sqlexecx-0.0.1/sqlexecx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)     7491 2024-05-04 04:37:35.000000 sqlexecx-0.0.1/sqlexecx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      442 2024-05-04 04:37:35.000000 sqlexecx-0.0.1/sqlexecx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-04 04:37:35.000000 sqlexecx-0.0.1/sqlexecx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-04 04:37:35.000000 sqlexecx-0.0.1/sqlexecx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)       20 2024-05-04 04:37:35.000000 sqlexecx-0.0.1/sqlexecx.egg-info/requires.txt
--rw-r--r--   0 summy      (501) staff       (20)        9 2024-05-04 04:37:35.000000 sqlexecx-0.0.1/sqlexecx.egg-info/top_level.txt
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-04 04:37:36.089709 sqlexecx-0.0.1/test/
--rw-r--r--   0 summy      (501) staff       (20)     1192 2024-04-08 10:07:10.000000 sqlexecx-0.0.1/test/test.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-04 09:35:30.323068 sqlexecx-0.0.2/
+-rw-r--r--   0 summy      (501) staff       (20)    11357 2024-01-23 07:49:56.000000 sqlexecx-0.0.2/LICENSE
+-rw-r--r--   0 summy      (501) staff       (20)     7473 2024-05-04 09:35:30.322106 sqlexecx-0.0.2/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)     6974 2024-03-29 02:19:13.000000 sqlexecx-0.0.2/README.rst
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-04 09:35:30.323393 sqlexecx-0.0.2/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1273 2024-05-04 06:13:13.000000 sqlexecx-0.0.2/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-04 09:35:30.309202 sqlexecx-0.0.2/sqlexecx/
+-rw-r--r--   0 summy      (501) staff       (20)     2411 2024-05-04 06:26:02.000000 sqlexecx-0.0.2/sqlexecx/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)      641 2024-04-26 08:01:55.000000 sqlexecx-0.0.2/sqlexecx/constant.py
+-rw-r--r--   0 summy      (501) staff       (20)     8883 2024-05-04 04:35:51.000000 sqlexecx-0.0.2/sqlexecx/dialect.py
+-rw-r--r--   0 summy      (501) staff       (20)    18625 2024-05-04 08:51:07.000000 sqlexecx-0.0.2/sqlexecx/exec.py
+-rw-r--r--   0 summy      (501) staff       (20)     1936 2024-04-25 04:18:32.000000 sqlexecx-0.0.2/sqlexecx/loader.py
+-rw-r--r--   0 summy      (501) staff       (20)      822 2024-05-04 04:35:42.000000 sqlexecx-0.0.2/sqlexecx/log_support.py
+-rw-r--r--   0 summy      (501) staff       (20)     1933 2024-03-27 08:41:08.000000 sqlexecx-0.0.2/sqlexecx/page_exec.py
+-rw-r--r--   0 summy      (501) staff       (20)    15899 2024-05-04 09:35:22.000000 sqlexecx-0.0.2/sqlexecx/sql_exec.py
+-rw-r--r--   0 summy      (501) staff       (20)     3076 2024-05-04 04:36:08.000000 sqlexecx-0.0.2/sqlexecx/sql_support.py
+-rw-r--r--   0 summy      (501) staff       (20)    18462 2024-05-04 04:35:20.000000 sqlexecx-0.0.2/sqlexecx/table_exec.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-04 09:35:30.317620 sqlexecx-0.0.2/sqlexecx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)     7473 2024-05-04 09:35:30.000000 sqlexecx-0.0.2/sqlexecx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      442 2024-05-04 09:35:30.000000 sqlexecx-0.0.2/sqlexecx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-04 09:35:30.000000 sqlexecx-0.0.2/sqlexecx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-04 04:37:35.000000 sqlexecx-0.0.2/sqlexecx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)       20 2024-05-04 09:35:30.000000 sqlexecx-0.0.2/sqlexecx.egg-info/requires.txt
+-rw-r--r--   0 summy      (501) staff       (20)        9 2024-05-04 09:35:30.000000 sqlexecx-0.0.2/sqlexecx.egg-info/top_level.txt
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-04 09:35:30.318677 sqlexecx-0.0.2/test/
+-rw-r--r--   0 summy      (501) staff       (20)     1192 2024-04-08 10:07:10.000000 sqlexecx-0.0.2/test/test.py
```

### Comparing `sqlexecx-0.0.1/LICENSE` & `sqlexecx-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.0.1/PKG-INFO` & `sqlexecx-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: sqlexecx
-Version: 0.0.1
+Version: 0.0.2
 Summary: A thread safe sql executor for Python with connection pool. It helps you automatically manage connections and transactions. Support MySQL, PostgreSQL, SQLite etc.
 Home-page: https://gitee.com/summry/sqlexecx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
-Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python,RDB
+Keywords: SQL,MySQL,PostgreSQL,SQLite,Database,Python,RDB
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Usage Sample
 ''''''''''''
```

### Comparing `sqlexecx-0.0.1/README.rst` & `sqlexecx-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.0.1/setup.py` & `sqlexecx-0.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 
 setup(
     name='sqlexecx',
     packages=['sqlexecx'],
     description="A thread safe sql executor for Python with connection pool. It helps you automatically manage connections and transactions. Support MySQL, PostgreSQL, SQLite etc.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.0.1',
+    version='0.0.2',
     install_requires=[
-        'sqlexecutorx>=0.0.2',
+        'sqlexecutorx>=0.0.3',
     ],
     url='https://gitee.com/summry/sqlexecx',
     author='summy',
     author_email='xiazhongbiao@126.com',
-    keywords=['SQL', 'MySQL', 'PostgreSQL', 'SQLite', 'Oracle', 'SQL Server', 'Database', 'Python', 'RDB'],
+    keywords=['SQL', 'MySQL', 'PostgreSQL', 'SQLite', 'Database', 'Python', 'RDB'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
     },
     include_package_data=True,
     python_requires='>=3.6',
     zip_safe=False
```

### Comparing `sqlexecx-0.0.1/sqlexecx/constant.py` & `sqlexecx-0.0.2/sqlexecx/constant.py`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.0.1/sqlexecx/dialect.py` & `sqlexecx-0.0.2/sqlexecx/dialect.py`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.0.1/sqlexecx/exec.py` & `sqlexecx-0.0.2/sqlexecx/exec.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,49 +8,82 @@
     save as _save, batch_execute as _batch_execute, get as _get, query as _query, query_one as _query_one
 
 
 def execute(sql: str, *args, **kwargs):
     """
     Execute sql return effect rowcount
 
-    sql: INSERT INTO person(name, age) VALUES(?, ?)  -->  args: ('张三', 20)
-         INSERT INTO person(name, age) VALUES(:name,:age)  -->  kwargs: {'name': '张三', 'age': 20}
+    Examples
+    --------
+    >>> import sqlexecx as db
+    >>> sql = 'INSERT INTO person(name, age) VALUES(?, ?)'
+    >>> db.execute(sql, '张三', 20)
+    1
+    >>> sql = 'INSERT INTO person(name, age) VALUES(:name, :age)'
+    >>> db.execute(sql, name='张三', age=20)
+    1
     """
+
     sql, args = sql_support.try_mapping('sqlexecx.execute', sql, *args, **kwargs)
     return do_execute(sql, *args)
 
 
 def insert(table_name: str, **kwargs):
     """
     Insert data into table, return effect rowcount.
 
     :param table_name: table name
     :param kwargs: {name='张三', age=20}
     return: Effect rowcount
+
+    Examples
+    --------
+    >>> import sqlexecx as db
+    >>> db.insert('person', name='李四', age=18)
+    1
     """
+
     insert_log('insert', table_name, **kwargs)
     sql, args = sql_support.insert_sql_args(table_name.strip(), **kwargs)
     return do_execute(sql, *args)
 
 
 def save(table_name: str, **kwargs):
     """
     Insert data into table, return primary key.
+
+    Examples
+    --------
+    >>> import sqlexecx as db
+    >>> db.save('person', name='李四', age=18)
+    4
     """
+
     try:
         select_key = Dialect.get_select_key(table_name=table_name)
     except NotImplementedError:
         raise DBError(f"Expect 'select_key' but not. you may should use 'save_select_key' func with 'select_key'.")
     return save_select_key(select_key, table_name, **kwargs)
 
 
 def save_sql(sql: str, *args, **kwargs):
     """
     Insert data into table, return primary key.
+
+    Examples
+    --------
+    >>> import sqlexecx as db
+    >>> sql = 'INSERT INTO person(name, age) VALUES(?, ?)'
+    >>> db.save_sql(sql, '张三', 20)
+    3
+    >>> sql = 'INSERT INTO person(name, age) VALUES(:name, :age)'
+    >>> db.save_sql(sql, name='张三', age=20)
+    3
     """
+
     try:
         select_key = Dialect.get_select_key(sql=sql)
     except NotImplementedError:
         raise DBError(f"Expect 'select_key' but not. you may should use 'save_sql_select_key' func with 'select_key'.")
     return save_sql_select_key(select_key, sql, *args, **kwargs)
 
 
@@ -58,110 +91,178 @@
     """
     Insert data into table, return primary key.
 
     :param select_key: sql for select primary key
     :param table_name: table name
     :param kwargs: {name='张三', age=20}
     :return: Primary key
+
+    Examples
+    --------
+    >>> import sqlexecx as db
+    >>> db.save_select_key('SELECT LAST_INSERT_ID()', 'person', name='李四', age=18)
+    4
     """
+
     save_log('save_select_key', select_key, table_name, **kwargs)
     sql, args = sql_support.insert_sql_args(table_name.strip(), **kwargs)
     return save_sql_select_key(select_key, sql, *args)
 
 
 def save_sql_select_key(select_key: str, sql: str, *args, **kwargs):
     """
     Insert data into table, return primary key.
 
-    sql: INSERT INTO person(name, age) VALUES(?, ?)  -->  args: ('张三', 20)
-         INSERT INTO person(name, age) VALUES(:name,:age)  -->  kwargs: {'name': '张三', 'age': 20}
-
     :param select_key: sql for select primary key
     :param sql: SQL
     :return: Primary key
+
+    Examples
+    --------
+    >>> import sqlexecx as db
+    >>> select_key = 'SELECT LAST_INSERT_ID()'
+    >>> sql = 'INSERT INTO person(name, age) VALUES(?, ?)'
+    >>> db.save_sql_select_key(select_key, sql, '张三', 20)
+    3
+    >>> sql = 'INSERT INTO person(name, age) VALUES(:name, :age)'
+    >>> db.save_sql_select_key(select_key, sql, name='张三', age=20)
+    3
     """
+
     logger.debug("Exec func 'sqlexecx.%s', 'select_key': %s \n\t sql: %s \n\t args: %s \n\t kwargs: %s" % ('save_sql', select_key, sql, args, kwargs))
     sql, args = sql_support.get_mapping_sql_args(sql, *args, **kwargs)
     return do_save_sql_select_key(select_key, sql, *args)
 
 
 def get(sql: str, *args, **kwargs):
     """
     Execute select SQL and expected one int and only one int result, SQL contain 'limit'.
 
     MultiColumnsError: Expect only one column.
-    sql: SELECT count(1) FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
-         SELECT count(1) FROM person WHERE name=:name and age=:age limit 1  --> kwargs: {'name': '张三', 'age': 20}
+
+    Examples
+    --------
+    >>> import sqlexecx as db
+    >>> sql = 'SELECT count(1) FROM person WHERE name=? and age=? LIMIT 1'
+    >>> db.get(sql, '张三', 20)
+    1
+    >>> sql = 'SELECT count(1) FROM person WHERE name=:name and age=:age LIMIT 1'
+    >>> db.get(sql, name='张三', age=20)
+    1
     """
+
     sql, args = sql_support.try_mapping('sqlexecx.get', sql, *args, **kwargs)
     return do_get(sql, *args)
 
 
 def select(sql: str, *args, **kwargs):
     """
-    execute select SQL and return unique result or list results(tuple).
+    Execute select SQL and return unique result or list results(tuple).
 
-    sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
-         SELECT * FROM person WHERE name=:name and age=:age --> kwargs: {'name': '张三', 'age': 20}
+    Examples
+    --------
+    >>> import sqlexecx as db
+    >>> sql = 'SELECT id, name, age FROM person WHERE name=? and age=?'
+    >>> db.select(sql, '张三', 20)
+    [(3, '张三', 20)]
+    >>> sql = 'SELECT id, name, age FROM person WHERE name=:name and age=:age '
+    >>> db.get(sql, name='张三', age=20)
+    [(3, '张三', 20)]
     """
+
     sql, args = sql_support.try_mapping('sqlexecx.select', sql, *args, **kwargs)
     return do_select(sql, *args)
 
 
 def select_one(sql: str, *args, **kwargs):
     """
     Execute select SQL and return unique result(tuple), SQL contain 'limit'.
 
-    sql: SELECT * FROM person WHERE name=? and age=? limit 1 -->  args: ('张三', 20)
-         SELECT * FROM person WHERE name=:name and age=:age limit 1 --> kwargs: {'name': '张三', 'age': 20}
+    Examples
+    --------
+    >>> import sqlexecx as db
+    >>> sql = 'SELECT id, name, age FROM person WHERE name=? and age=? LIMIT 1'
+    >>> db.select_one(sql, '张三', 20)
+    (3, '张三', 20)
+    >>> sql = 'SELECT id, name, age FROM person WHERE name=:name and age=:age LIMIT 1'
+    >>> db.select_one(sql, name='张三', age=20)
+    (3, '张三', 20)
     """
+
     sql, args = sql_support.try_mapping('sqlexecx.select_one', sql, *args, **kwargs)
     return do_select_one(sql, *args)
 
 
 def query(sql: str, *args, **kwargs):
     """
     Execute select SQL and return list results(dict).
-    sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
-         SELECT * FROM person WHERE name=:name and age=:age --> kwargs: {'name': '张三', 'age': 20}
+
+    Examples
+    --------
+    >>> import sqlexecx as db
+    >>> sql = 'SELECT id, name, age FROM person WHERE name=? and age=?'
+    >>> db.query(sql, '张三', 20)
+    [{'id': 3, 'name': '张三', 'age': 20}]
+    >>> sql = 'SELECT id, name, age FROM person WHERE name=:name and age=:age '
+    >>> db.query(sql, name='张三', age=20)
+    [{'id': 3, 'name': '张三', 'age': 20}]
     """
     sql, args = sql_support.try_mapping('sqlexecx.query', sql, *args, **kwargs)
     return do_query(sql, *args)
 
 
 def query_one(sql: str, *args, **kwargs):
     """
-    execute select SQL and return unique result(dict), SQL contain 'limit'.
+    Execute select SQL and return unique result(dict), SQL contain 'limit'.
 
-    sql: SELECT * FROM person WHERE name=? and age=? limit 1 -->  args: ('张三', 20)
-         SELECT * FROM person WHERE name=:name and age=:age limit 1 --> kwargs: {'name': '张三', 'age': 20}
+    Examples
+    --------
+    >>> import sqlexecx as db
+    >>> sql = 'SELECT id, name, age FROM person WHERE name=? and age=? LIMIT 1'
+    >>> db.query_one(sql, '张三', 20)
+    {'id': 3, 'name': '张三', 'age': 20}
+    >>> sql = 'SELECT id, name, age FROM person WHERE name=:name and age=:age LIMIT 1'
+    >>> db.query_one(sql, name='张三', age=20)
+    {'id': 3, 'name': '张三', 'age': 20}
     """
     sql, args = sql_support.try_mapping('sqlexecx.query_one', sql, *args, **kwargs)
     return do_query_one(sql, *args)
 
 
 def do_execute(sql: str, *args):
     """
     Execute sql return effect rowcount
 
-    sql: insert into person(name, age) values(?, ?)  -->  args: ('张三', 20)
+    Examples
+    --------
+    >>> import sqlexecx as db
+    >>> sql = 'INSERT INTO person(name, age) VALUES(?, ?)'
+    >>> db.do_execute(sql, '张三', 20)
+    1
     """
     sql = Dialect.before_execute(sql)
     return _execute(sql, *args)
 
 
 def do_save_sql(sql: str, *args):
     """
     Insert data into table, return primary key.
 
-    :param select_key: sql for select primary key
     :param sql: SQL
     :param args:
     :return: Primary key
+
+    Examples
+    --------
+    >>> import sqlexecx as db
+    >>> sql = 'INSERT INTO person(name, age) VALUES(?, ?)'
+    >>> db.do_save_sql(sql, '张三', 20)
+    3
     """
+
     try:
         select_key = Dialect.get_select_key(sql=sql)
     except NotImplementedError:
         raise DBError(f"Expect 'select_key' but not. you may should use 'save_sql_select_key' func with 'select_key'.")
     return do_save_sql_select_key(select_key, sql, *args)
 
 
@@ -169,165 +270,285 @@
     """
     Insert data into table, return primary key.
 
     :param select_key: sql for select primary key
     :param sql: SQL
     :param args:
     :return: Primary key
+
+    Examples
+    --------
+    >>> import sqlexecx as db
+    >>> select_key = 'SELECT LAST_INSERT_ID()'
+    >>> sql = 'INSERT INTO person(name, age) VALUES(?, ?)'
+    >>> db.do_save_sql_select_key(select_key, sql, '张三', 20)
+    3
     """
+
     sql = Dialect.before_execute(sql)
     return _save(select_key, sql, *args)
 
 
 def do_get(sql: str, *args):
     """
     Execute select SQL and expected one int and only one int result, SQL contain 'limit'.
+
     MultiColumnsError: Expect only one column.
 
-    sql: SELECT count(1) FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
+    Examples
+    --------
+    >>> import sqlexecx as db
+    >>> sql = 'SELECT count(1) FROM person WHERE name=? and age=? LIMIT 1'
+    >>> db.do_get(sql, '张三', 20)
+    1
     """
+
     sql, args = sql_support.limit_one_sql_args(sql, *args)
     sql = Dialect.before_execute(sql)
     return _get(sql, *args)
 
 
 def do_select(sql: str, *args):
     """
-    execute select SQL and return unique result or list results(tuple).
-    sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
+    Execute select SQL and return unique result or list results(tuple).
+
+    Examples
+    --------
+    >>> import sqlexecx as db
+    >>> sql = 'SELECT id, name, age FROM person WHERE name=? and age=?'
+    >>> db.do_select(sql, '张三', 20)
+    [(3, '张三', 20)]
     """
+
     sql = Dialect.before_execute(sql)
     return _select(sql, *args)
 
 
 def do_select_one(sql: str, *args):
     """
     Execute select SQL and return unique result(tuple), SQL contain 'limit'.
-    sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
+
+    Examples
+    --------
+    >>> import sqlexecx as db
+    >>> sql = 'SELECT id, name, age FROM person WHERE name=? and age=? LIMIT 1'
+    >>> db.do_select_one(sql, '张三', 20)
+    (3, '张三', 20)
     """
+
     sql, args = sql_support.limit_one_sql_args(sql, *args)
     sql = Dialect.before_execute(sql)
     return _select_one(sql, *args)
 
 
 def do_query(sql: str, *args):
     """
     Execute select SQL and return list results(dict).
-    sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
+
+    Examples
+    --------
+    >>> import sqlexecx as db
+    >>> sql = 'SELECT id, name, age FROM person WHERE name=? and age=?'
+    >>> db.do_query(sql, '张三', 20)
+    [{'id': 3, 'name': '张三', 'age': 20}]
     """
+
     sql = Dialect.before_execute(sql)
     return _query(sql, *args)
 
 
 def do_query_one(sql: str, *args):
     """
-    execute select SQL and return unique result(dict), SQL contain 'limit'.
-    sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
+    Execute select SQL and return unique result(dict), SQL contain 'limit'.
+
+    Examples
+    --------
+    >>> import sqlexecx as db
+    >>> sql = 'SELECT id, name, age FROM person WHERE name=? and age=? LIMIT 1'
+    >>> db.do_query_one(sql, '张三', 20)
+    {'id': 3, 'name': '张三', 'age': 20}
     """
+
     sql, args = sql_support.limit_one_sql_args(sql, *args)
     sql = Dialect.before_execute(sql)
     return _query_one(sql, *args)
 
 
 def select_page(sql: str, page_num=1, page_size=10, *args, **kwargs):
     """
-    Execute select SQL and return list(tuple) or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
-    sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
-         SELECT * FROM user WHERE name=:name and age=:age   -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
+    Execute select SQL and return list(tuple) or empty list if no result.
+
+    Automatically add 'limit ?,?' after sql statement if not.
+
+    Examples
+    --------
+    >>> import sqlexecx as db
+    >>> sql = 'SELECT id, name, age FROM person WHERE name=? and age=?'
+    >>> db.select_page(sql, 1, 10, '张三', 20)
+    [(3, '张三', 20)]
+    >>> sql = 'SELECT id, name, age FROM person WHERE name=:name and age=:age '
+    >>> db.select_page(sql, 1, 10, name='张三', age=20)
+    [(3, '张三', 20)]
     """
+
     sql, args = sql_support.try_mapping('select_page', sql, *args, **kwargs)
     return do_select_page(sql, page_num, page_size, *args)
 
 
 def query_page(sql: str, page_num=1, page_size=10, *args, **kwargs):
     """
-    Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
-    sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
-         SELECT * FROM user WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
+    Execute select SQL and return list or empty list if no result.
+
+    Automatically add 'limit ?,?' after sql statement if not.
+
+    Examples
+    --------
+    >>> import sqlexecx as db
+    >>> sql = 'SELECT id, name, age FROM person WHERE name=? and age=?'
+    >>> db.query_page(sql, 1, 10, '张三', 20)
+    [{'id': 3, 'name': '张三', 'age': 20}]
+    >>> sql = 'SELECT id, name, age FROM person WHERE name=:name and age=:age '
+    >>> db.query_page(sql, 1, 10, name='张三', age=20)
+    [{'id': 3, 'name': '张三', 'age': 20}]
     """
     sql, args = sql_support.try_mapping('query_page', sql, *args, **kwargs)
     return do_query_page(sql, page_num, page_size, *args)
 
 
 def do_select_page(sql: str, page_num=1, page_size=10, *args):
     """
     Execute select SQL and return list results(dict).
-    sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
+
+    Examples
+    --------
+    >>> import sqlexecx as db
+    >>> sql = 'SELECT id, name, age FROM person WHERE name=? and age=?'
+    >>> db.do_select_page(sql, 1, 10, '张三', 20)
+    [(3, '张三', 20)]
     """
+
     sql, args = Dialect.get_page_sql_args(sql, page_num, page_size, *args)
     return do_select(sql, *args)
 
 
 def do_query_page(sql: str, page_num=1, page_size=10, *args):
     """
     Execute select SQL and return list results(dict).
-    sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
+
+    Examples
+    --------
+    >>> import sqlexecx as db
+    >>> sql = 'SELECT id, name, age FROM person WHERE name=? and age=?'
+    >>> db.do_query_page(sql, 1, 10, '张三', 20)
+    [{'id': 3, 'name': '张三', 'age': 20}]
     """
+
     sql, args = Dialect.get_page_sql_args(sql, page_num, page_size, *args)
     return do_query(sql, *args)
 
 
 def batch_execute(sql: str, *args):
     """
     Batch execute
-    :param sql: insert into person(name, age) values(?, ?)  -->  args: [('张三', 20), ('李四', 28)]
+
+    :param sql: SQL to execute
     :param args: All number must have same size.
     :return: Effect row count
+
+    Examples
+    --------
+    >>> import sqlexecx as db
+    >>> args = [('张三', 20), ('李四', 28)]
+    >>> sql = 'INSERT INTO person(name, age) VALUES(?, ?)'
+    >>> db.batch_execute(sql, *args)
+    2
+    >>> args =  [{'name': '张三', 'age': 20}, {'name': '李四', 'age': 28}]
+    >>> sql = 'INSERT INTO person(name, age) VALUES(:name, :age)'
+    >>> db.batch_execute(sql, *args)
+    2
     """
+
     assert args, "*args must not be empty."
     if isinstance(args[0], dict):
         sql, args = sql_support.batch_named_sql_args(sql, *args)
     sql = Dialect.before_execute(sql)
     args = sql_support.get_batch_args(*args)
     return _batch_execute(sql, *args)
 
 
 def batch_insert(table_name: str, *args):
     """
     Batch insert
+
     :param table_name: table name
     :param args: All number must have same key. [{'name': '张三', 'age': 20}, {'name': '李四', 'age': 28}]
     :return: Effect row count
+
+    Examples
+    --------
+    >>> import sqlexecx as db
+    >>> args =  [{'name': '张三', 'age': 20}, {'name': '李四', 'age': 28}]
+    >>> db.batch_execute(sql, *args)
+    2
     """
     logger.debug("Exec func 'sqlexecx.%s' \n\t Table: '%s', args: %s" % ('batch_insert', table_name, args))
     sql, args = sql_support.batch_insert_sql_args(table_name, *args)
     return batch_execute(sql, *args)
 
 
 def load(sql: str, *args, **kwargs) -> Loader:
     """
-    Execute select SQL and save a csv
+    Execute select SQL and return Loader instance
 
-    sqlexecx.load('select id, name, age from person WHERE name=:name', name='张三')
-
-    :param sql: SELECT * FROM person WHERE name=? and age=? limit 1 -->  args: ('张三', 20)
-                SELECT * FROM person WHERE name=:name and age=:age limit 1 --> kwargs: {'name': '张三', 'age': 20}
+    :param sql: SQL to be executed
     :return: Loader
+
+    Examples
+    --------
+    >>> import sqlexecx as db
+    >>> sql = 'SELECT id, name, age FROM person WHERE name=? and age=?'
+    >>> db.load(sql, '张三', 20)
+    Lodder()
+    >>> sql = 'SELECT id, name, age FROM person WHERE name=:name and age=:age'
+    >>> db.load(sql, name='张三', age=20)
+    Lodder()
     """
     sql, args = sql_support.try_mapping('sqlexecx.csv', sql, *args, **kwargs)
     return do_load(sql, *args)
 
 
 def do_load(sql: str, *args) -> Loader:
     """
-    Execute select SQL and save a csv
+    Execute select SQL and return Loader instance
 
-    sqlexecx.do_load('select id, name, age from person WHERE name = ?', '张三')
-
-    :param sql: SELECT * FROM person WHERE name=? and age=? limit 1 -->  args: ('张三', 20)
+    :param sql: SQL to be executed
     :return: Loader
+
+    Examples
+    --------
+    >>> import sqlexecx as db
+    >>> sql = 'SELECT id, name, age FROM person WHERE name=? and age=?'
+    >>> db.do_load(sql, '张三', 20)
+    Lodder()
     """
+
     sql = Dialect.before_execute(sql)
     return Loader(*_do_select(sql, *args))
 
 
 def insert_from_csv(file_name: str, table_name: str, delimiter=',', header=True, columns: Collection[str] = None, encoding='utf-8') -> int:
     """
-    sqlexecx.insert_from_csv('test.csv', 'person')
+    Read data from csv file, and insert into table
+
+    Examples
+    --------
+    >>> import sqlexecx as db
+    >>> db.insert_from_csv('test.csv', 'person')
     """
+
     import csv
     sql = None
     if columns and len(columns) > 0:
         sql = sql_support.insert_sql(table_name.strip(), columns)
     elif not header:
         raise ValueError("Expected one of 'header' and 'columns'.")
 
@@ -347,31 +568,43 @@
         lines = lines[1:]
 
     return batch_execute(sql, lines)
 
 
 def insert_from_df(df, table_name: str, columns: Collection[str] = None) -> int:
     """
-    sqlexecx.insert_from_df(df, 'person')
+    Insert data into table from pandas DataFrame
+
+    Examples
+    --------
+    >>> import sqlexecx as db
+    >>> db.insert_from_df(df, 'person')
     """
+
     columns = columns if columns and len(columns) > 0 else df.columns.tolist()
     sql = sql_support.insert_sql(table_name.strip(), columns)
     return batch_execute(sql, df.values.tolist())
 
 
 def insert_from_json(file_name: str, table_name: str, encoding='utf-8') -> int:
     """
-    sqlexecx.insert_from_json('test.json', 'person')
+    Read data from json file, and insert into table
+
+    Examples
+    --------
+    >>> import sqlexecx as db
+    >>> db.insert_from_json('test.json', 'person')
 
     many rows json file example:
     [{"id": 1, "name": "张三", "age": 55}, ...]
 
     one row json file example:
     {"id": 1, "name": "张三", "age": 55}
     """
+
     import json
 
     with open(file_name, encoding=encoding) as f:
         data = json.load(f)
 
     if isinstance(data, dict):
         return insert(table_name, **data)
@@ -379,19 +612,40 @@
         return batch_insert(table_name, data)
     else:
         logger.info("Exec func 'sqlexecx.%s' \n\t Table: '%s' insert 0 rows." % ('insert_from_json', table_name))
         return 0
 
 
 def truncate_table(table_name: str) -> int:
-    """ sqlexecx.truncate_table('person') """
+    """
+    Truncate table
+
+    Examples
+    --------
+    >>> import sqlexecx as db
+    >>> db.truncate_table('person')
+    """
     return Dialect.truncate_table(table_name)
 
 
 def drop_table(table_name: str) -> int:
-    """ sqlexecx.drop_table('person') """
+    """
+    Drop table
+
+    Examples
+    --------
+    >>> import sqlexecx as db
+    >>> db.drop_table('person')
+    """
     return _execute('DROP TABLE IF EXISTS %s' % Dialect.get_dialect_str(table_name))
 
 
 def show_tables(schema: str = None):
-    """ sqlexecx.show_tables() """
+    """
+    Show tables
+
+    Examples
+    --------
+    >>> import sqlexecx as db
+    >>> db.show_tables()
+    """
     return Dialect.show_tables(schema)
```

### Comparing `sqlexecx-0.0.1/sqlexecx/loader.py` & `sqlexecx-0.0.2/sqlexecx/loader.py`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.0.1/sqlexecx/log_support.py` & `sqlexecx-0.0.2/sqlexecx/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.0.1/sqlexecx/page_exec.py` & `sqlexecx-0.0.2/sqlexecx/page_exec.py`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.0.1/sqlexecx/sql_exec.py` & `sqlexecx-0.0.2/sqlexecx/sql_exec.py`

 * *Files 22% similar despite different names*

```diff
@@ -110,209 +110,358 @@
         """
         sqlexecx.sql('SELECT * FROM person WHERE name=? and age=? limit 1').param('张三', 18).query_one()
         """
         return self.sql_exec.query_one(*self.args, **self.kwargs)
 
     def to_csv(self, file_name: str, delimiter=',', header=True, encoding='utf-8'):
         """
-        sqlexecx.sql('SELECT * FROM person WHERE name=? and age=?').param('张三', 18).to_csv('test.csv')
+        Execute select SQL and sava as a csv file.
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.sql('SELECT * FROM person WHERE name=? and age=?').param('张三', 18).to_csv('test.csv')
         """
         self.sql_exec.load(*self.args, **self.kwargs).to_csv(file_name, delimiter, header, encoding)
 
     def to_df(self):
         """
-        sqlexecx.sql('SELECT * FROM person WHERE name=? and age=?').param('张三', 18).to_df()
+        Execute select SQL and return pandas DataFrame instance.
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.sql('SELECT * FROM person WHERE name=? and age=?').param('张三', 18).to_df()
+        pd.DataFrame()
         """
         return self.sql_exec.load(*self.args, **self.kwargs).to_df()
 
     def to_json(self, file_name: str, encoding='utf-8'):
         """
-        sqlexecx.sql('SELECT * FROM person WHERE name=? and age=?').param('张三', 18).to_json('test.json')
+        Execute select SQL and sava as a json file.
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=?').param('张三', 18).to_json('test.json')
         """
         self.sql_exec.load(*self.args, **self.kwargs).to_json(file_name, encoding)
 
     def page(self, page_num=1, page_size=10) -> ParamPageExec:
+        """
+        Execute select SQL and return ParamPageExec instance.
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=?').param('张三', 18).page(1, 10)
+        ParamPageExec()
+        """
         return ParamPageExec(self.sql_exec.page(page_num, page_size), *self.args, **self.kwargs)
 
 
 class SqlExec:
 
     def __init__(self, _exec, sql: str):
         self.exec = _exec
         self.sql = sql
 
     def execute(self, *args, **kwargs) -> int:
         """
-        Execute sql return effect rowcount
+        Execute sql return effected rowcount
 
-        sql: INSERT INTO person(name, age) VALUES(?, ?)  -->  args: ('张三', 20)
-             INSERT INTO person(name, age) VALUES(:name,:age)  -->  kwargs: {'name': '张三', 'age': 20}
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.sql('INSERT INTO person(name, age) VALUES(?, ?)').execute('张三', 20)
+        1
+        >>> db.sql('INSERT INTO person(name, age) VALUES(:name, :age)').execute(name='张三', age=20)
+        1
         """
+
         return self.exec.execute(self.sql, *args, **kwargs)
 
     def save(self, *args, **kwargs):
         """
         Insert data into table, return primary key.
 
-        :param select_key: sql for select primary key
         :param args:
         :return: Primary key
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.sql('INSERT INTO person(name, age) VALUES(?, ?)').save('张三', 20)
+        3
+        >>> db.sql('INSERT INTO person(name, age) VALUES(:name, :age)').save(name='张三', age=20)
+        3
         """
+
         return self.exec.save_sql(self.sql, *args, **kwargs)
 
     def save_select_key(self, select_key: str, *args, **kwargs):
         """
         Insert data into table, return primary key.
 
         :param select_key: sql for select primary key
         :param args:
         :return: Primary key
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> select_key = 'SELECT LAST_INSERT_ID()'
+        >>> db.sql('INSERT INTO person(name, age) VALUES(?, ?)').save_select_key(select_key, '张三', 20)
+        3
+        >>> db.sql('INSERT INTO person(name, age) VALUES(:name, :age)').save_select_key(select_key, name='张三', age=20)
+        3
         """
+
         return self.exec.save_sql_select_key(select_key, self.sql, *args, **kwargs)
 
     def get(self, *args, **kwargs):
         """
         Execute select SQL and expected one int and only one int result, SQL contain 'limit'.
+
         MultiColumnsError: Expect only one column.
 
-        sql: SELECT count(1) FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
-             SELECT count(1) FROM person WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.sql('SELECT count(1) FROM person WHERE name=? and age=? LIMIT 1').get('张三', 20)
+        1
+        >>> db.sql('SELECT count(1) FROM person WHERE name=:name and age=:age LIMIT 1').get(name='张三', age=20)
+        1
         """
         return self.exec.get(self.sql, *args, **kwargs)
 
     def select(self, *args, **kwargs):
         """
-        execute select SQL and return unique result or list results(tuple).
+        Execute select SQL and return unique result or list results(tuple).
 
-        sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
-             SELECT * FROM person WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=?').select('张三', 20)
+        [(3, '张三', 20)]
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=:name and age=:age').select(name='张三', age=20)
+        [(3, '张三', 20)]
         """
         return self.exec.select(self.sql, *args, **kwargs)
 
     def select_one(self, *args, **kwargs):
         """
         Execute select SQL and return unique result(tuple), SQL contain 'limit'.
 
-        sql: SELECT * FROM person WHERE name=? and age=? limit 1 -->  args: ('张三', 20)
-             SELECT * FROM person WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=? LIMIT 1').select_one('张三', 20)
+        (3, '张三', 20)
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=:name and age=:age LIMIT 1').select_one(name='张三', age=20)
+        (3, '张三', 20)
         """
         return self.exec.select_one(self.sql, *args, **kwargs)
 
     def query(self, *args, **kwargs):
         """
         Execute select SQL and return list results(dict).
 
-        sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
-             SELECT * FROM person WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=?').query('张三', 20)
+        [{'id': 3, 'name': '张三', 'age': 20}]
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=:name and age=:age').query(name='张三', age=20)
+        [{'id': 3, 'name': '张三', 'age': 20}]
         """
         return self.exec.query(self.sql, *args, **kwargs)
 
     def query_one(self, *args, **kwargs):
         """
         execute select SQL and return unique result(dict), SQL contain 'limit'.
 
-        sql: SELECT * FROM person WHERE name=? and age=? limit 1 -->  args: ('张三', 20)
-             SELECT * FROM person WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=?').query_one('张三', 20)
+        {'id': 3, 'name': '张三', 'age': 20}
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=:name and age=:age').query_one(name='张三', age=20)
+        {'id': 3, 'name': '张三', 'age': 20}
         """
         return self.exec.query_one(self.sql, *args, **kwargs)
 
     def do_execute(self, *args):
         """
-        Execute sql return effect rowcount
+        Execute sql return effected rowcount
 
-        sql: insert into person(name, age) values(?, ?)  -->  args: ('张三', 20)
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.sql('INSERT INTO person(name, age) VALUES(?, ?)').do_execute('张三', 20)
+        1
         """
         return self.exec.do_execute(None, self.sql, *args)
 
     def do_save_sql(self, select_key: str, *args):
         """
         Insert data into table, return primary key.
 
         :param select_key: sql for select primary key
         :param args:
         :return: Primary key
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> select_key = 'SELECT LAST_INSERT_ID()'
+        >>> db.sql('INSERT INTO person(name, age) VALUES(?, ?)').do_save_sql(select_key, '张三', 20)
+        3
         """
         return self.exec.do_save_sql(select_key, self.sql, *args)
 
     def do_get(self, *args):
         """
         Execute select SQL and expected one int and only one int result, SQL contain 'limit'.
+
         MultiColumnsError: Expect only one column.
 
-        sql: SELECT count(1) FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.sql('SELECT count(1) FROM person WHERE name=? and age=? LIMIT 1').do_get('张三', 20)
+        1
         """
         return self.exec.do_get(self.sql, *args)
 
     def do_select(self, *args):
         """
-        execute select SQL and return unique result or list results(tuple).
+        Execute select SQL and return unique result or list results(tuple).
 
-        sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=? LIMIT 1').do_select('张三', 20)
+        (3, '张三', 20)
         """
         return self.exec.do_select(self.sql, *args)
 
     def do_select_one(self, *args):
         """
         Execute select SQL and return unique result(tuple), SQL contain 'limit'.
 
-        sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=? LIMIT 1').do_select_one('张三', 20)
+        (3, '张三', 20)
         """
         return self.exec.do_select_one(self.sql, *args)
 
     def do_query(self, *args):
         """
         Execute select SQL and return list results(dict).
 
-        sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=?').do_query('张三', 20)
+        [{'id': 3, 'name': '张三', 'age': 20}]
         """
         return self.exec.do_query(self.sql, *args)
 
     def do_query_one(self, *args):
         """
         execute select SQL and return unique result(dict), SQL contain 'limit'.
 
-        sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=?').do_query_one('张三', 20)
+        {'id': 3, 'name': '张三', 'age': 20}
         """
         return self.exec.do_query_one(self.sql, *args)
 
     def batch_execute(self, *args):
         """
-        Batch execute sql return effect rowcount
-
-        sql: insert into person(name, age) values(?, ?)  -->  args: [('张三', 20), ('李四', 28)]
+        Batch execute sql return effected rowcount
 
         :param args: All number must have same size.
         :return: Effect rowcount
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> args = [('张三', 20), ('李四', 28)]
+        >>> db.sql('INSERT INTO person(name, age) VALUES(?, ?)').batch_execute(*args)
+        2
+        >>> args =  [{'name': '张三', 'age': 20}, {'name': '李四', 'age': 28}]
+        >>> db.sql('INSERT INTO person(name, age) VALUES(:name, :age)').batch_execute(sql, *args)
+        2
         """
         return self.exec.batch_execute(self.sql, *args)
 
     def load(self, *args, **kwargs) -> Loader:
         """
-        sqlexecx.sql('select id, name, age from person WHERE name = :name').load(name='张三')
-        sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
-             SELECT * FROM person WHERE name = :name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
+        Execute select SQL and return Loader instance
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=?').load('张三', 20)
+        Lodder()
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=:name and age=:age').load(name='张三', age=20)
+        Lodder()
         """
         return self.exec.load(self.sql, *args, **kwargs)
 
     def do_load(self, *args) -> Loader:
         """
-        sqlexecx.sql('select id, name, age from person WHERE name = ?').do_load('张三')
-        sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
+        Execute select SQL and return Loader instance
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=?').load('张三', 20)
+        Lodder()
         """
         return self.exec.do_load(self.sql, *args)
 
     def param(self, *args, **kwargs) -> Param:
         """
-        sqlexecx.sql('select id, name, age from person WHERE name = :name').param(name='张三')
-        sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
-             SELECT * FROM person WHERE name = :name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
+        Execute select SQL and return Param instance
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=?').param('张三', 20)
+        Param()
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=:name and age=:age').param(name='张三', age=20)
+        Param()
         """
         return Param(self, *args, **kwargs)
 
     def page(self, page_num=1, page_size=10) -> SqlPageExec:
+        """
+        Execute select SQL and return SqlPageExec instance
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=?').page(1, 10)
+        SqlPageExec()
+        """
         return SqlPageExec(self.sql, PageExec(self.exec, page_num=page_num, page_size=page_size))
 
 
 def sql(sql_text: str) -> SqlExec:
+    """
+    Get a SqlExec instance
+
+    Examples
+    --------
+    >>> import sqlexecx as db
+    >>> db.sql('SELECT id, name, age FROM person')
+    """
     sql_text = sql_text.strip()
     assert sql_text, "Parameter 'sql' must not be none"
     return SqlExec(exec, sql_text)
```

### Comparing `sqlexecx-0.0.1/sqlexecx/sql_support.py` & `sqlexecx-0.0.2/sqlexecx/sql_support.py`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.0.1/sqlexecx/table_exec.py` & `sqlexecx-0.0.2/sqlexecx/table_exec.py`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.0.1/sqlexecx.egg-info/PKG-INFO` & `sqlexecx-0.0.2/sqlexecx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: sqlexecx
-Version: 0.0.1
+Version: 0.0.2
 Summary: A thread safe sql executor for Python with connection pool. It helps you automatically manage connections and transactions. Support MySQL, PostgreSQL, SQLite etc.
 Home-page: https://gitee.com/summry/sqlexecx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
-Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python,RDB
+Keywords: SQL,MySQL,PostgreSQL,SQLite,Database,Python,RDB
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Usage Sample
 ''''''''''''
```

### Comparing `sqlexecx-0.0.1/test/test.py` & `sqlexecx-0.0.2/test/test.py`

 * *Files identical despite different names*

