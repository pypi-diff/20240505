# Comparing `tmp/snowflake-dbml-generator-0.1.0.tar.gz` & `tmp/snowflake-dbml-generator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowflake-dbml-generator-0.1.0.tar", last modified: Thu May  2 18:40:36 2024, max compression
+gzip compressed data, was "snowflake-dbml-generator-0.1.1.tar", last modified: Sun May  5 21:09:57 2024, max compression
```

## Comparing `snowflake-dbml-generator-0.1.0.tar` & `snowflake-dbml-generator-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2024-05-02 18:40:36.297748 snowflake-dbml-generator-0.1.0/
--rw-r--r--   0 ryan       (501) staff       (20)     1068 2024-04-24 14:03:50.000000 snowflake-dbml-generator-0.1.0/LICENSE
--rw-r--r--   0 ryan       (501) staff       (20)    11538 2024-05-02 18:40:36.297595 snowflake-dbml-generator-0.1.0/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)    11121 2024-05-02 18:37:51.000000 snowflake-dbml-generator-0.1.0/README.md
--rw-r--r--   0 ryan       (501) staff       (20)       38 2024-05-02 18:40:36.297796 snowflake-dbml-generator-0.1.0/setup.cfg
--rw-r--r--   0 ryan       (501) staff       (20)     1017 2024-05-02 18:37:51.000000 snowflake-dbml-generator-0.1.0/setup.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2024-05-02 18:40:36.296618 snowflake-dbml-generator-0.1.0/snowflake_dbml/
--rw-r--r--   0 ryan       (501) staff       (20)      142 2024-05-02 18:37:51.000000 snowflake-dbml-generator-0.1.0/snowflake_dbml/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     2305 2024-05-02 18:37:51.000000 snowflake-dbml-generator-0.1.0/snowflake_dbml/config.py
--rw-r--r--   0 ryan       (501) staff       (20)    19754 2024-05-02 18:37:51.000000 snowflake-dbml-generator-0.1.0/snowflake_dbml/generator.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2024-05-02 18:40:36.297387 snowflake-dbml-generator-0.1.0/snowflake_dbml_generator.egg-info/
--rw-r--r--   0 ryan       (501) staff       (20)    11538 2024-05-02 18:40:36.000000 snowflake-dbml-generator-0.1.0/snowflake_dbml_generator.egg-info/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      396 2024-05-02 18:40:36.000000 snowflake-dbml-generator-0.1.0/snowflake_dbml_generator.egg-info/SOURCES.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2024-05-02 18:40:36.000000 snowflake-dbml-generator-0.1.0/snowflake_dbml_generator.egg-info/dependency_links.txt
--rw-r--r--   0 ryan       (501) staff       (20)       65 2024-05-02 18:40:36.000000 snowflake-dbml-generator-0.1.0/snowflake_dbml_generator.egg-info/entry_points.txt
--rw-r--r--   0 ryan       (501) staff       (20)       70 2024-05-02 18:40:36.000000 snowflake-dbml-generator-0.1.0/snowflake_dbml_generator.egg-info/requires.txt
--rw-r--r--   0 ryan       (501) staff       (20)       15 2024-05-02 18:40:36.000000 snowflake-dbml-generator-0.1.0/snowflake_dbml_generator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:09:57.671314 snowflake-dbml-generator-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-05 21:09:43.000000 snowflake-dbml-generator-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-05-05 21:09:57.671314 snowflake-dbml-generator-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-05-05 21:09:43.000000 snowflake-dbml-generator-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 21:09:57.671314 snowflake-dbml-generator-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-05 21:09:43.000000 snowflake-dbml-generator-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:09:57.667314 snowflake-dbml-generator-0.1.1/snowflake_dbml/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-05 21:09:43.000000 snowflake-dbml-generator-0.1.1/snowflake_dbml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-05 21:09:43.000000 snowflake-dbml-generator-0.1.1/snowflake_dbml/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21445 2024-05-05 21:09:43.000000 snowflake-dbml-generator-0.1.1/snowflake_dbml/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-05 21:09:52.000000 snowflake-dbml-generator-0.1.1/snowflake_dbml/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:09:57.671314 snowflake-dbml-generator-0.1.1/snowflake_dbml_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-05-05 21:09:57.000000 snowflake-dbml-generator-0.1.1/snowflake_dbml_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-05 21:09:57.000000 snowflake-dbml-generator-0.1.1/snowflake_dbml_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 21:09:57.000000 snowflake-dbml-generator-0.1.1/snowflake_dbml_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-05 21:09:57.000000 snowflake-dbml-generator-0.1.1/snowflake_dbml_generator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-05 21:09:57.000000 snowflake-dbml-generator-0.1.1/snowflake_dbml_generator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-05 21:09:57.000000 snowflake-dbml-generator-0.1.1/snowflake_dbml_generator.egg-info/top_level.txt
```

### Comparing `snowflake-dbml-generator-0.1.0/LICENSE` & `snowflake-dbml-generator-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake-dbml-generator-0.1.0/setup.py` & `snowflake-dbml-generator-0.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from setuptools import setup, find_packages
+from snowflake_dbml.version import __version__
+
 
 setup(
     name='snowflake-dbml-generator',
-    version='0.1.0',
+    version=__version__,
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'snowflake-dbml=snowflake_dbml.generator:main',
         ],
     },
     author='Ryan Rozich',
```

### Comparing `snowflake-dbml-generator-0.1.0/snowflake_dbml/config.py` & `snowflake-dbml-generator-0.1.1/snowflake_dbml/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         'user': os.getenv('SNOWFLAKE_USER'),
         'password': os.getenv('SNOWFLAKE_PASSWORD'),
         'account': os.getenv('SNOWFLAKE_ACCOUNT'),
         'warehouse': os.getenv('SNOWFLAKE_WAREHOUSE'),
         'database': os.getenv('SNOWFLAKE_DATABASE'),
         'role': os.getenv('SNOWFLAKE_ROLE'),
 
-        'primary_key_hints_path': os.getenv('PRIMARY_KEY_HINTS_PATH'),
+        'config_file': os.getenv('CONFIG_FILE'),
 
         'included_schemas': os.getenv('INCLUDED_SCHEMAS'),  # Schemas to include
         'excluded_schemas': os.getenv('EXCLUDED_SCHEMAS'),  # Schemas to exclude
         
         'table_color': os.getenv('TABLE_COLOR', default_table_color),
         'view_color': os.getenv('VIEW_COLOR', default_view_color), 
         'dynamic_table_color': os.getenv('DYNAMIC_TABLE_COLOR', default_dynamic_table_color)
```

### Comparing `snowflake-dbml-generator-0.1.0/snowflake_dbml/generator.py` & `snowflake-dbml-generator-0.1.1/snowflake_dbml/generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from datetime import datetime
 from collections import defaultdict
 import snowflake.connector
 from pydbml import PyDBML, Database
 from pydbml.classes import Project, Table, Column, Reference, Note, TableGroup
 from snowflake.connector import DictCursor
 from snowflake_dbml.config import load_config, load_primary_key_hints, load_visualization_params
+from snowflake_dbml.version import __version__
 
 import logging
 
 # Configure the logger for the module
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)  # Set the default logging level
 
@@ -87,14 +88,30 @@
         'primary_keys': filtered_pks,
         'foreign_keys': filtered_fks
     }
 
     return data
 
 def generate_dbml(data, connection_params=None, primary_key_hints=None, visualization_params=None):
+    """
+    Generates a DBML representation of a Snowflake database based on the provided data.
+
+    Args:
+        data (dict): The data containing information about the tables, columns, primary keys, and foreign keys.
+        connection_params (dict, optional): The connection parameters for the Snowflake database. Defaults to None.
+        primary_key_hints (dict, optional): The primary key hints for inferring relationships. Defaults to None.
+        visualization_params (dict, optional): The visualization parameters for customizing the DBML output. Defaults to None.
+
+    Returns:
+        str: The DBML representation of the Snowflake database.
+
+    Raises:
+        None
+
+    """
     db = Database()
 
     # Load visualization params, primary key hints, and connection params
     vis_params_default = load_visualization_params()
     if visualization_params:
         for key in vis_params_default:
             if key in visualization_params and visualization_params[key]:
@@ -340,21 +357,38 @@
             for key, value in config.items():
                 if value:  # Only save non-empty values
                     f.write(f"{key.upper()}={value}\n")
         print("Configuration saved to .env file in the current directory.")
     else:
         print("Configuration not saved.")
 
+def mask_sensitive_info(conn_params):
+    """
+    Masks sensitive information in connection parameters.
+    """
+    masked_params = conn_params.copy()
+    if 'password' in masked_params:
+        masked_params['password'] = '****'
+    return masked_params
+
 
 def main():
+    # Configure logging
+    logging.basicConfig(filename='snowflake-dbml.log', level=logging.INFO, format='%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+
     # Setup Argument Parser with more options
     parser = argparse.ArgumentParser(
-        description="Reverese engineer ER diagrams files from Snowflake databases using DBML",
+        description=f"Reverese engineer ER diagrams files from Snowflake databases using DBML (version {__version__})",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter  # This will show default values in the help message
     )
+
+    # Version argument
+    parser.add_argument('-v', '--version', action='version', version=f'%(prog)s {__version__}',
+                        help="Show version number and exit.")
+
     parser.add_argument('--user', type=str, help='Snowflake user name')
     parser.add_argument('--password', type=str, help='Snowflake password')
     parser.add_argument('--account', type=str, help='Snowflake account identifier')
     parser.add_argument('--warehouse', type=str, help='Snowflake warehouse')
     parser.add_argument('--database', type=str, help='Snowflake database name')
     parser.add_argument('--role', type=str, help='Snowflake role')
     parser.add_argument('--config-file', type=str, help='Path to the config JSON file (contains primary/foreign key hints)')
@@ -380,15 +414,15 @@
             'password': args.password or config['password'],
             'account': args.account or config['account'],
             'warehouse': args.warehouse or config['warehouse'],
             'database': args.database or config['database'],
             'role': args.role or config['role'],
         }
 
-        primary_key_hints = load_primary_key_hints(args.config_file or config.get('config-file'))
+        primary_key_hints = load_primary_key_hints(args.config_file or config.get('config_file'))
 
         if args.included_schemas:
             config['included_schemas'] = args.included_schemas
         if args.excluded_schemas:
             config['excluded_schemas'] = args.excluded_schemas
 
         visualization_params = load_visualization_params()
@@ -396,23 +430,29 @@
         if args.table_color:
             visualization_params['table_color'] = args.table_color
         if args.view_color:
             visualization_params['view_color'] = args.view_color
         if args.dynamic_table_color:
             visualization_params['dynamic_table_color'] = args.dynamic_table_color
 
-    logging.debug(f"Generating DBML")
-    logging.debug(f"Connection Params: {connection_params}")
-    logging.debug(f"Primary Key Hints: {primary_key_hints}")
-    logging.debug(f"Visualization Params: {visualization_params}")
+    logger.debug(f"Generating DBML")
+    masked_params = mask_sensitive_info(connection_params)
+    logger.debug(f"Connection Params: {masked_params}")
+    logger.debug(f"Primary Key Hints: {primary_key_hints}")
+    logger.debug(f"Visualization Params: {visualization_params}")
 
+    logger.info(f"Fetching data from Snowflake starting.")
     data = fetch_data(connection_params, config['included_schemas'], config['excluded_schemas'])
+    logger.info(f"Fetching data from Snowflake complete.")
 
-    logging.debug(f"Fetched data from Snowflake: {len(data)} rows")
+    # Logging the number of results for each key in the data dictionary
+    for key, value in data.items():
+        logger.info(f"Number of results for {key}: {len(value)}")
 
 
     dbml_output = generate_dbml(data, connection_params=connection_params, primary_key_hints=primary_key_hints, visualization_params=visualization_params)
     print(dbml_output)
+    logger.info("Snowflake DBML generator complete.")
 
 if __name__ == "__main__":
 
     main()
```

