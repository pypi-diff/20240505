# Comparing `tmp/pd_extras-4.0.2.tar.gz` & `tmp/pd_extras-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pd_extras-4.0.2.tar", max compression
+gzip compressed data, was "pd_extras-5.0.2.tar", max compression
```

## Comparing `pd_extras-4.0.2.tar` & `pd_extras-5.0.2.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1069 2023-02-17 08:54:14.018072 pd_extras-4.0.2/LICENSE
--rw-r--r--   0        0        0     2278 2023-02-17 09:27:40.004601 pd_extras-4.0.2/README.md
--rw-r--r--   0        0        0        0 2023-02-17 08:54:14.018072 pd_extras-4.0.2/pd_extras/__init__.py
--rw-r--r--   0        0        0        0 2023-02-17 08:54:14.018072 pd_extras-4.0.2/pd_extras/check/__init__.py
--rw-r--r--   0        0        0     3245 2023-02-17 08:54:14.018072 pd_extras-4.0.2/pd_extras/check/sanitize.py
--rw-r--r--   0        0        0        0 2023-02-17 08:54:14.018072 pd_extras-4.0.2/pd_extras/extra/__init__.py
--rw-r--r--   0        0        0     3794 2023-02-17 08:54:14.018072 pd_extras-4.0.2/pd_extras/extra/flattener.py
--rw-r--r--   0        0        0     2635 2023-02-17 08:54:14.018072 pd_extras-4.0.2/pd_extras/extra/operations.py
--rw-r--r--   0        0        0        0 2023-02-17 08:54:14.018072 pd_extras-4.0.2/pd_extras/optimize/__init__.py
--rw-r--r--   0        0        0     1775 2023-02-17 08:54:14.018072 pd_extras-4.0.2/pd_extras/optimize/df_ops.py
--rw-r--r--   0        0        0        0 2023-02-17 08:54:14.018072 pd_extras-4.0.2/pd_extras/write/__init__.py
--rw-r--r--   0        0        0     1388 2023-02-17 08:54:14.018072 pd_extras-4.0.2/pd_extras/write/common.py
--rw-r--r--   0        0        0     5682 2023-02-17 08:54:14.018072 pd_extras-4.0.2/pd_extras/write/nosql_writer.py
--rw-r--r--   0        0        0     9667 2023-02-19 13:53:12.490252 pd_extras-4.0.2/pd_extras/write/sql_writer.py
--rw-r--r--   0        0        0     1443 2023-02-22 21:19:14.341637 pd_extras-4.0.2/pyproject.toml
--rw-r--r--   0        0        0     3220 1970-01-01 00:00:00.000000 pd_extras-4.0.2/setup.py
--rw-r--r--   0        0        0     3242 1970-01-01 00:00:00.000000 pd_extras-4.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-05 13:00:18.946226 pd_extras-5.0.2/LICENSE
+-rw-r--r--   0        0        0     2248 2024-05-05 13:00:18.946226 pd_extras-5.0.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-05 13:00:18.946226 pd_extras-5.0.2/pd_extras/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:00:18.946226 pd_extras-5.0.2/pd_extras/check/__init__.py
+-rw-r--r--   0        0        0     3245 2024-05-05 13:00:18.946226 pd_extras-5.0.2/pd_extras/check/sanitize.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:00:18.946226 pd_extras-5.0.2/pd_extras/extra/__init__.py
+-rw-r--r--   0        0        0     3794 2024-05-05 13:00:18.946226 pd_extras-5.0.2/pd_extras/extra/flattener.py
+-rw-r--r--   0        0        0     2635 2024-05-05 13:00:18.946226 pd_extras-5.0.2/pd_extras/extra/operations.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:00:18.946226 pd_extras-5.0.2/pd_extras/optimize/__init__.py
+-rw-r--r--   0        0        0     1775 2024-05-05 13:00:18.946226 pd_extras-5.0.2/pd_extras/optimize/df_ops.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:00:18.950226 pd_extras-5.0.2/pd_extras/write/__init__.py
+-rw-r--r--   0        0        0     1388 2024-05-05 13:00:18.950226 pd_extras-5.0.2/pd_extras/write/common.py
+-rw-r--r--   0        0        0     5682 2024-05-05 13:00:18.950226 pd_extras-5.0.2/pd_extras/write/nosql_writer.py
+-rw-r--r--   0        0        0     8962 2024-05-05 13:00:18.950226 pd_extras-5.0.2/pd_extras/write/sql_writer.py
+-rw-r--r--   0        0        0      724 2024-05-05 13:00:18.950226 pd_extras-5.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3262 1970-01-01 00:00:00.000000 pd_extras-5.0.2/PKG-INFO
```

### Comparing `pd_extras-4.0.2/LICENSE` & `pd_extras-5.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pd_extras-4.0.2/README.md` & `pd_extras-5.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 # Pandas Extras
 
 ![Build](https://github.com/proafxin/pandas-utils/actions/workflows/tox_build.yml/badge.svg)
-![Workflow for Codecov Action](https://github.com/proafxin/pd-extras/actions/workflows/codecov.yml/badge.svg)
-[![codecov](https://codecov.io/gh/proafxin/pd-extras/branch/develop/graph/badge.svg?token=AQA0IJY4N1)](https://codecov.io/gh/proafxin/pd-extras)[![Documentation Status](https://readthedocs.org/projects/pd-extras/badge/?version=latest)](https://pd-extras.readthedocs.io/en/latest/?badge=latest)
+[![codecov](https://codecov.io/gh/proafxin/pd-extras/graph/badge.svg?token=AQA0IJY4N1)](https://codecov.io/gh/proafxin/pd-extras)
+[![Documentation Status](https://readthedocs.org/projects/pd-extras/badge/?version=latest)](https://pd-extras.readthedocs.io/en/latest/?badge=latest)
 
 Some functions on top of pandas.
 
 ## Install Environment
 
 Run `python -m pip install -U pip` and `pip install -U pip poetry`. Then run `poetry install`. If you are facing issues installing `mysqlclient` or `psycopg2` on Ubuntu, it's because you are missing some libraries. Please check their pages. Usually for `psycopg2`, it's `libpq-dev` and for `mysqlclient`, it's `python3-dev default-libmysqlclient-dev build-essential`. Check the pages for more specific and accurate commands.
 
+## Testing
+
+Run `docker compose up` then `tox`. Obviously you need docker and tox installed.
+
 ## Generate Documentation Source Files
 
 You should not have to do this but in case you want to generate the source ReStructuredText files yourself, here is how. Skip to the next section to simply generate html documentation locally.
 
 Change to docs directory `cd docs/`. Run `sphinx-quickstart`. Choose `y` when it asks to seperate build and source directories.
 
 Change to `docs/source` directory. In `conf.py`, add the following lines at the start of the script.
```

### Comparing `pd_extras-4.0.2/pd_extras/check/sanitize.py` & `pd_extras-5.0.2/pd_extras/check/sanitize.py`

 * *Files identical despite different names*

### Comparing `pd_extras-4.0.2/pd_extras/extra/flattener.py` & `pd_extras-5.0.2/pd_extras/extra/flattener.py`

 * *Files identical despite different names*

### Comparing `pd_extras-4.0.2/pd_extras/extra/operations.py` & `pd_extras-5.0.2/pd_extras/extra/operations.py`

 * *Files identical despite different names*

### Comparing `pd_extras-4.0.2/pd_extras/optimize/df_ops.py` & `pd_extras-5.0.2/pd_extras/optimize/df_ops.py`

 * *Files identical despite different names*

### Comparing `pd_extras-4.0.2/pd_extras/write/common.py` & `pd_extras-5.0.2/pd_extras/write/common.py`

 * *Files identical despite different names*

### Comparing `pd_extras-4.0.2/pd_extras/write/nosql_writer.py` & `pd_extras-5.0.2/pd_extras/write/nosql_writer.py`

 * *Files identical despite different names*

### Comparing `pd_extras-4.0.2/pd_extras/write/sql_writer.py` & `pd_extras-5.0.2/pd_extras/write/sql_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Write a pandas dataframe to a SQL database table"""
 
-
 import pandas as pd
 from pandas.api.types import is_integer_dtype, is_numeric_dtype  # type: ignore
-from pd_extras.write.common import saved_values
 from sqlalchemy import (
     Column,
     Float,
     Integer,
     MetaData,
     String,
     Table,
     create_engine,
     text,
 )
 from sqlalchemy.orm import Session
 from sqlalchemy_utils import create_database, database_exists
 
+from pd_extras.write.common import saved_values
+
 
 class SQLDatabaseWriter:
     """Database connection object for SQL databases
     Only database name `dbname` is stored.
     Rest of the credentials are used only to retrieved the connection.
     Two connections are created: one for the specific database `dbname`
     and another generic connection with no database selected.
@@ -32,16 +32,20 @@
         dbtype: str,
         host: str,
         dbname: str,
         user: str,
         password: str,
         port: int,
     ):
-        assert dbtype in saved_values, f"{dbtype} not in {list(saved_values.keys())}"
-        assert dbname is not None, "`dbname` must be a valid database name"
+        if dbtype not in saved_values:
+            raise KeyError(f"{dbtype} not in {list(saved_values.keys())}")
+
+        if not dbname:
+            raise ValueError("`dbname` must be a valid database name")
+
         self.__dbtype = dbtype
         self.__dbname = dbname
         port = int(port)
 
         self.__engine = self._get_db_specific_engine(
             host=host,
             user=user,
@@ -60,40 +64,14 @@
             f"{dialect}{driver}://{user}:{password}@{host}:{port}/{self.__dbname}"
         )
 
         engine = create_engine(connection_string, future=True)
 
         return engine
 
-    def get_data_from_query(self, query: str):
-        """Execute a single query on the current database.
-
-        :param query: SQL statement to execute.
-        :type query: `str`
-        :return: Pandas dataframe with result of query.
-        :rtype: `pd.DataFrame`
-        """
-
-        with self.__engine.connect() as conn:
-            return pd.read_sql(sql=text(query), con=conn)
-
-    def get_list_of_database(self):
-        """Get list of databases.
-
-        :return: List containing database names.
-        :rtype: `list[str]`
-        """
-
-        query = saved_values[self.__dbtype]["query"]["db_list"]
-
-        res = self.get_data_from_query(query=query)
-        database_names = res[res.columns[0]].to_numpy()
-
-        return database_names
-
     def get_column_info(self, table_name: str):
         """Get table schema from database.
 
         :param table_name: Name of the table in database.
         :type table_name: ``str``
         :return: Pandas dataframe of table schema information.
         :rtype: ``pd.DataFrame``
```

### Comparing `pd_extras-4.0.2/setup.py` & `pd_extras-5.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,80 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pd-extras
+Version: 5.0.2
+Summary: Some utility functions on top of pandas.
+Home-page: https://github.com/proafxin/pd-extras
+License: MIT
+Author: Masum Billal
+Author-email: billalmasum93@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: mysqlclient (>=2.2.4,<3.0.0)
+Requires-Dist: pandas (>=1.5.3)
+Requires-Dist: psycopg2 (>=2.9.9,<3.0.0)
+Requires-Dist: pymongo (>=4.7.1,<5.0.0)
+Requires-Dist: pymssql (>=2.3.0,<3.0.0)
+Requires-Dist: sqlalchemy (>=1,<2)
+Requires-Dist: sqlalchemy-utils (>=0.41.2,<0.42.0)
+Project-URL: Documentation, https://pd-extras.readthedocs.io/en/latest/
+Project-URL: Repository, https://github.com/proafxin/pd-extras
+Description-Content-Type: text/markdown
 
-packages = \
-['pd_extras',
- 'pd_extras.check',
- 'pd_extras.extra',
- 'pd_extras.optimize',
- 'pd_extras.write']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['dnspython',
- 'mysqlclient',
- 'pandas>=1.5.3',
- 'psycopg2',
- 'pyarrow',
- 'pymongo',
- 'pymssql',
- 'pymysql',
- 'sqlalchemy-utils',
- 'sqlalchemy>=1.4.0,<2.0.0']
-
-setup_kwargs = {
-    'name': 'pd-extras',
-    'version': '4.0.2',
-    'description': 'Some utility functions on top of pandas.',
-    'long_description': '# Pandas Extras\n\n![Build](https://github.com/proafxin/pandas-utils/actions/workflows/tox_build.yml/badge.svg)\n![Workflow for Codecov Action](https://github.com/proafxin/pd-extras/actions/workflows/codecov.yml/badge.svg)\n[![codecov](https://codecov.io/gh/proafxin/pd-extras/branch/develop/graph/badge.svg?token=AQA0IJY4N1)](https://codecov.io/gh/proafxin/pd-extras)[![Documentation Status](https://readthedocs.org/projects/pd-extras/badge/?version=latest)](https://pd-extras.readthedocs.io/en/latest/?badge=latest)\n\nSome functions on top of pandas.\n\n## Install Environment\n\nRun `python -m pip install -U pip` and `pip install -U pip poetry`. Then run `poetry install`. If you are facing issues installing `mysqlclient` or `psycopg2` on Ubuntu, it\'s because you are missing some libraries. Please check their pages. Usually for `psycopg2`, it\'s `libpq-dev` and for `mysqlclient`, it\'s `python3-dev default-libmysqlclient-dev build-essential`. Check the pages for more specific and accurate commands.\n\n## Generate Documentation Source Files\n\nYou should not have to do this but in case you want to generate the source ReStructuredText files yourself, here is how. Skip to the next section to simply generate html documentation locally.\n\nChange to docs directory `cd docs/`. Run `sphinx-quickstart`. Choose `y` when it asks to seperate build and source directories.\n\nChange to `docs/source` directory. In `conf.py`, add the following lines at the start of the script.\n\n```python\nimport os\nimport sys\n\nsys.path.insert(0, os.path.abspath("../.."))\n```\n\nand save it. Add `"sphinx.ext.autodoc",` to the `extensions` list. Run `python -m pip install -U sphinx_rtd_theme` and set `html_theme = "sphinx_rtd_theme"` (or whatever theme you want).\n\nIn `index.rst`, add `modules` to toctree. The structure should look like this:\n\n```markdown\n.. toctree::\n:maxdepth: 2\n:caption: Contents:\n\nmodules\n```\n\nRun the following to generate the source files.\n\n```markdown\npoetry install --with docs\npoetry run sphinx-apidoc -f -o source/ ../ ../tests/\n```\n\n## Generating HTML Documentation\n\nChange to `docs/` using `cd ..` then run `.\\make clean` and `.\\make html`. Output should be built with no errors or warnings. You will get the html documenation in `docs/build/html` directory. Open `index.html`.\n',
-    'author': 'Masum Billal',
-    'author_email': 'billalmasum93@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/proafxin/pandas-utils',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
+# Pandas Extras
 
+![Build](https://github.com/proafxin/pandas-utils/actions/workflows/tox_build.yml/badge.svg)
+[![codecov](https://codecov.io/gh/proafxin/pd-extras/graph/badge.svg?token=AQA0IJY4N1)](https://codecov.io/gh/proafxin/pd-extras)
+[![Documentation Status](https://readthedocs.org/projects/pd-extras/badge/?version=latest)](https://pd-extras.readthedocs.io/en/latest/?badge=latest)
+
+Some functions on top of pandas.
+
+## Install Environment
+
+Run `python -m pip install -U pip` and `pip install -U pip poetry`. Then run `poetry install`. If you are facing issues installing `mysqlclient` or `psycopg2` on Ubuntu, it's because you are missing some libraries. Please check their pages. Usually for `psycopg2`, it's `libpq-dev` and for `mysqlclient`, it's `python3-dev default-libmysqlclient-dev build-essential`. Check the pages for more specific and accurate commands.
+
+## Testing
+
+Run `docker compose up` then `tox`. Obviously you need docker and tox installed.
+
+## Generate Documentation Source Files
+
+You should not have to do this but in case you want to generate the source ReStructuredText files yourself, here is how. Skip to the next section to simply generate html documentation locally.
+
+Change to docs directory `cd docs/`. Run `sphinx-quickstart`. Choose `y` when it asks to seperate build and source directories.
+
+Change to `docs/source` directory. In `conf.py`, add the following lines at the start of the script.
+
+```python
+import os
+import sys
+
+sys.path.insert(0, os.path.abspath("../.."))
+```
+
+and save it. Add `"sphinx.ext.autodoc",` to the `extensions` list. Run `python -m pip install -U sphinx_rtd_theme` and set `html_theme = "sphinx_rtd_theme"` (or whatever theme you want).
+
+In `index.rst`, add `modules` to toctree. The structure should look like this:
+
+```markdown
+.. toctree::
+:maxdepth: 2
+:caption: Contents:
+
+modules
+```
+
+Run the following to generate the source files.
+
+```markdown
+poetry install --with docs
+poetry run sphinx-apidoc -f -o source/ ../ ../tests/
+```
+
+## Generating HTML Documentation
+
+Change to `docs/` using `cd ..` then run `.\make clean` and `.\make html`. Output should be built with no errors or warnings. You will get the html documenation in `docs/build/html` directory. Open `index.html`.
 
-setup(**setup_kwargs)
```

