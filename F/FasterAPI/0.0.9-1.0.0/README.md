# Comparing `tmp/FasterAPI-0.0.9.tar.gz` & `tmp/fasterapi-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FasterAPI-0.0.9.tar", last modified: Mon Dec 18 08:16:00 2023, max compression
+gzip compressed data, was "fasterapi-1.0.0.tar", max compression
```

## Comparing `FasterAPI-0.0.9.tar` & `fasterapi-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-12-18 08:16:00.868338 FasterAPI-0.0.9/
-drwxrwxrwx   0        0        0        0 2023-12-18 08:16:00.850026 FasterAPI-0.0.9/FasterAPI/
--rw-rw-rw-   0        0        0     2618 2023-12-18 02:22:32.000000 FasterAPI-0.0.9/FasterAPI/__init__.py
--rw-rw-rw-   0        0        0     1891 2023-12-18 08:14:47.000000 FasterAPI-0.0.9/FasterAPI/app.py
--rw-rw-rw-   0        0        0      702 2023-12-01 07:11:05.000000 FasterAPI-0.0.9/FasterAPI/models.py
--rw-rw-rw-   0        0        0     5381 2023-12-01 16:48:01.000000 FasterAPI-0.0.9/FasterAPI/router.py
--rw-rw-rw-   0        0        0      451 2023-12-01 06:34:20.000000 FasterAPI-0.0.9/FasterAPI/schemas.py
--rw-rw-rw-   0        0        0     4816 2023-12-18 02:22:32.000000 FasterAPI-0.0.9/FasterAPI/utils.py
-drwxrwxrwx   0        0        0        0 2023-12-18 08:16:00.864337 FasterAPI-0.0.9/FasterAPI.egg-info/
--rw-rw-rw-   0        0        0     3814 2023-12-18 08:16:00.000000 FasterAPI-0.0.9/FasterAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-12-18 08:16:00.000000 FasterAPI-0.0.9/FasterAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-18 08:16:00.000000 FasterAPI-0.0.9/FasterAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      105 2023-12-18 08:16:00.000000 FasterAPI-0.0.9/FasterAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-12-18 08:16:00.000000 FasterAPI-0.0.9/FasterAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3814 2023-12-18 08:16:00.866335 FasterAPI-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     3075 2023-12-18 02:22:32.000000 FasterAPI-0.0.9/README.md
--rw-rw-rw-   0        0        0      748 2023-12-18 08:15:04.000000 FasterAPI-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-12-18 08:16:00.868338 FasterAPI-0.0.9/setup.cfg
+-rw-r--r--   0        0        0     6953 2024-05-05 06:48:45.103852 fasterapi-1.0.0/FasterAPI/__init__.py
+-rw-r--r--   0        0        0       65 2024-05-05 04:36:07.878626 fasterapi-1.0.0/FasterAPI/__main__.py
+-rw-r--r--   0        0        0      191 2024-05-05 04:36:07.878626 fasterapi-1.0.0/FasterAPI/cli/__init__.py
+-rw-r--r--   0        0        0     7762 2024-05-05 06:04:07.228983 fasterapi-1.0.0/FasterAPI/cli/module.py
+-rw-r--r--   0        0        0     5072 2024-05-05 06:36:10.832521 fasterapi-1.0.0/FasterAPI/cli/project.py
+-rw-r--r--   0        0        0      877 2024-05-05 05:54:18.620311 fasterapi-1.0.0/FasterAPI/cli/templates/config.yaml.j2
+-rw-r--r--   0        0        0      751 2024-05-05 04:52:56.067937 fasterapi-1.0.0/FasterAPI/cli/templates/module/__init__.py.j2
+-rw-r--r--   0        0        0      150 2024-05-05 06:49:11.341428 fasterapi-1.0.0/FasterAPI/cli/templates/module/config.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-05 04:36:07.880626 fasterapi-1.0.0/FasterAPI/cli/templates/module/dependencies.py.j2
+-rw-r--r--   0        0        0      932 2024-05-05 04:36:07.888176 fasterapi-1.0.0/FasterAPI/cli/templates/module/router.py.j2
+-rw-r--r--   0        0        0      240 2024-05-05 04:36:07.888176 fasterapi-1.0.0/FasterAPI/cli/templates/module/schema.py.j2
+-rw-r--r--   0        0        0      737 2024-05-05 04:45:10.064787 fasterapi-1.0.0/FasterAPI/cli/templates/module/utils.py.j2
+-rw-r--r--   0        0        0      260 2024-05-05 04:36:07.889181 fasterapi-1.0.0/FasterAPI/cli/templates/serve.py.j2
+-rw-r--r--   0        0        0     2921 2024-05-05 04:36:07.890181 fasterapi-1.0.0/FasterAPI/cli/templates/user/__init__.py.j2
+-rw-r--r--   0        0        0      424 2024-05-05 06:49:01.521624 fasterapi-1.0.0/FasterAPI/cli/templates/user/config.yaml.j2
+-rw-r--r--   0        0        0     3305 2024-05-05 04:36:07.891182 fasterapi-1.0.0/FasterAPI/cli/templates/user/dependencies.py.j2
+-rw-r--r--   0        0        0     8394 2024-05-05 04:36:07.891182 fasterapi-1.0.0/FasterAPI/cli/templates/user/router.py.j2
+-rw-r--r--   0        0        0      908 2024-05-05 04:36:07.892181 fasterapi-1.0.0/FasterAPI/cli/templates/user/schemas.py.j2
+-rw-r--r--   0        0        0     6058 2024-05-05 04:41:18.312086 fasterapi-1.0.0/FasterAPI/cli/templates/user/utils.py.j2
+-rw-r--r--   0        0        0      903 2024-05-05 07:12:06.257147 fasterapi-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3603 2024-03-22 03:27:35.126041 fasterapi-1.0.0/README.md
+-rw-r--r--   0        0        0     4759 1970-01-01 00:00:00.000000 fasterapi-1.0.0/PKG-INFO
```

### Comparing `FasterAPI-0.0.9/FasterAPI.egg-info/PKG-INFO` & `fasterapi-1.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,103 +1,110 @@
-Metadata-Version: 2.1
-Name: FasterAPI
-Version: 0.0.9
-Summary: Just a FasterAPI starting point with JWT user authentication.
-Author-email: Yifei Ren <ryf0510@live.com>
-Project-URL: Homepage, https://github.com/ulfaric/FasterAPI
-Project-URL: Bug Tracker, https://github.com/ulfaric/FasterAPI/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Requires-Dist: fastapi[all]
-Requires-Dist: sqlalchemy
-Requires-Dist: colorlog
-Requires-Dist: python-jose[cryptography]
-Requires-Dist: bcrypt==4.0.1
-Requires-Dist: passlib[bcrypt]
-Requires-Dist: psycopg2-binary
-
 # FasterAPI
 
 This is a simple start point for backend application based on FastAPI with JWT user authentication built for you. :)
 
 ## How to use
 
 First install it with pip. You do not need to install FastAPI seperately. All related libaray has been added as dependencies.
 
-```
+```bash
 pip install FasterAPI
 ```
+
 Then, you have to create a "auth-config.yaml" file, please make sure the file name is excat the same. This file should contains:
+
 ```yaml
 SQLALCHEMY_DATABASE_URL: "postgresql://postgres:postgres@127.0.0.1:5432/postgres" # url to your postgresql
 SECRET_KEY: "8cfba7f89fca29a5f86cd8e02cb5381070690e378fc26cce4a311f84ce93672a" # create with openssl rand -hex 32
 ALGORITHM: "HS256" # encryption algorithm
 TOKEN_URL: "login" # url for login
 TOKEN_EXPIRATION_TIME: 1 # token expiration time in minutes.
-ALLOW_SELF_REGISTRATION: True # if ture, anyone could register a user account. Otherwise, only superuser could.
-
+ALLOW_SELF_REGISTRATION: True # if true, anyone could register a user account. Otherwise, only superuser could.
+ALLOW_MULTI_SESSIONS: False # if true, same user can login from different client. Otherwise, only one client is allowed.
 # if any following configuration is missing, lowest security config will used for faster development!
 # for non-website (include web app) you may want to use the default settings so your request won't be blocked.
 ALLOW_CREDENTIALS: False # Here goes your choice for whether allow credential for CSRF protection
 ALLOWED_ORIGINS: # Here goes your allowed origns for CSRF protection
   - "*"
 ALLOWED_METHODS: # Here goes your allowed method for CSRF protection
   - "*"
 ALLOWED_HEADERS: # Here goes your allowed headers for CSRF protection
   - "*"
 ```
+
 Now, create a "main.py" file:
+
 ```python
 import uvicorn
 from FasterAPI.utils import init_migration, create_superuser
 
 if __name__ == "__main__":
-    # must run at first which creates all tables within the database.
-    init_migration()
     # create a superuser, optional
     create_superuser(
         username="admin",
         password="admin",
         first_name="admin",
         last_name="admin",
         email="admin@admin.com"
     )
     # start the fastapi app
-    uvicorn.run("FasterAPI.app:app", host="127.0.0.1", log_level="info", reload=True)
+    uvicorn.run("FasterAPI:app", host="127.0.0.1", log_level="info", reload=True)
 ```
+
 Finally, you could start the application by simply run the main.py.
 
 ## Add additonal models and routes
+
 If you need more models, you have to reference the base created inside FasterAPI:
+
 ```python
 from FasterAPI import Base
 ```
+
 For your additional route, you have to reference the FasterAPI app instance like:
+
 ```python
 from FasterAPI.app import app
 
 @app.get("/)
 # your function goes here
 ```
+
 Note that you will have to create a python module, place main.py and auth-config.yaml like following:
+
 ```python
 your_module:
   -- __init__.py
   -- models.py # your additional models
   -- schemas.py # your schemas
   -- routes.py # your addtional routes
 main.py
 auth_config.yaml
 ```
 
-## New! Now you can add meta data with "meta_config.yaml".
+## You can add meta data with "meta_config.yaml"
 
 For example, the following "meta_config.yaml" will change the title and version, as well as enable the debug.
+
 ```yaml
 DEBUG: True
 TITLE: "My API"
+DESCRIPTION: "This is a description of my API"
 VERSION: "0.0.2"
+OPENAPI_URL: "/openapi.json"
+DOCS_URL: "/docs"
+REDOC_URL: "/redoc"
+TERMS_OF_SERVICE: ""
+CONTACT: ""
+SUMMARY: "This is a summary of my API"
 ```
+
 All the key words here is simply one to one mapping of FastAPI() constructor!
+
+## New! Now also built in with Opentelemetries for Tracing!, simple configure the following in meta_config.yaml
+
+```yaml
+JAEGER_SVC_NAME: "my-api" # service name
+JAEGER_TRACE: True # enable tracing
+JAEGER_HOST: "localhost" # Jaeger host
+JAEGER_PORT: "6831" # Jaeger host port
+```
```

