# Comparing `tmp/podman-init-1.0.0.tar.gz` & `tmp/podman_init-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podman-init-1.0.0.tar", last modified: Sat Mar 30 12:44:56 2024, max compression
+gzip compressed data, was "podman_init-1.0.1.tar", last modified: Sun May  5 16:46:45 2024, max compression
```

## Comparing `podman-init-1.0.0.tar` & `podman_init-1.0.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:44:56.488616 podman-init-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-30 12:44:41.000000 podman-init-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-03-30 12:44:56.488616 podman-init-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-03-30 12:44:41.000000 podman-init-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:44:56.488616 podman-init-1.0.0/podman_init.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-03-30 12:44:56.000000 podman-init-1.0.0/podman_init.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-03-30 12:44:56.000000 podman-init-1.0.0/podman_init.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 12:44:56.000000 podman-init-1.0.0/podman_init.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-30 12:44:56.000000 podman-init-1.0.0/podman_init.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-30 12:44:56.000000 podman-init-1.0.0/podman_init.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-30 12:44:56.000000 podman-init-1.0.0/podman_init.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 12:44:56.488616 podman-init-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-30 12:44:41.000000 podman-init-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:44:56.484616 podman-init-1.0.0/src/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-30 12:44:41.000000 podman-init-1.0.0/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-03-30 12:44:41.000000 podman-init-1.0.0/src/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:44:56.484616 podman-init-1.0.0/src/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:44:56.484616 podman-init-1.0.0/src/templates/c#/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-30 12:44:41.000000 podman-init-1.0.0/src/templates/c#/Dockerfile.j2
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-30 12:44:41.000000 podman-init-1.0.0/src/templates/c#/docker-compose.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:44:56.488616 podman-init-1.0.0/src/templates/go/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-30 12:44:41.000000 podman-init-1.0.0/src/templates/go/Dockerfile.j2
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-03-30 12:44:41.000000 podman-init-1.0.0/src/templates/go/docker-compose.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:44:56.488616 podman-init-1.0.0/src/templates/java/
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-03-30 12:44:41.000000 podman-init-1.0.0/src/templates/java/Dockerfile.j2
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-30 12:44:41.000000 podman-init-1.0.0/src/templates/java/docker-compose.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:44:56.488616 podman-init-1.0.0/src/templates/node/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-30 12:44:41.000000 podman-init-1.0.0/src/templates/node/Dockerfile.j2
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-03-30 12:44:41.000000 podman-init-1.0.0/src/templates/node/docker-compose.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:44:56.488616 podman-init-1.0.0/src/templates/python/
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-30 12:44:41.000000 podman-init-1.0.0/src/templates/python/Dockerfile.j2
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-30 12:44:41.000000 podman-init-1.0.0/src/templates/python/docker-compose.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:44:56.488616 podman-init-1.0.0/src/templates/rust/
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-03-30 12:44:41.000000 podman-init-1.0.0/src/templates/rust/Dockerfile.j2
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-30 12:44:41.000000 podman-init-1.0.0/src/templates/rust/docker-compose.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:44:56.488616 podman-init-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7765 2024-03-30 12:44:41.000000 podman-init-1.0.0/tests/test_podman_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:46:45.435912 podman_init-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-05 16:46:37.000000 podman_init-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-05 16:46:45.435912 podman_init-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-05 16:46:37.000000 podman_init-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:46:45.435912 podman_init-1.0.1/podman_init.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-05 16:46:45.000000 podman_init-1.0.1/podman_init.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-05 16:46:45.000000 podman_init-1.0.1/podman_init.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 16:46:45.000000 podman_init-1.0.1/podman_init.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-05 16:46:45.000000 podman_init-1.0.1/podman_init.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-05 16:46:45.000000 podman_init-1.0.1/podman_init.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-05 16:46:45.000000 podman_init-1.0.1/podman_init.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 16:46:45.435912 podman_init-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-05 16:46:37.000000 podman_init-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:46:45.431912 podman_init-1.0.1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-05 16:46:37.000000 podman_init-1.0.1/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5056 2024-05-05 16:46:37.000000 podman_init-1.0.1/src/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:46:45.431912 podman_init-1.0.1/src/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:46:45.431912 podman_init-1.0.1/src/templates/c#/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-05 16:46:37.000000 podman_init-1.0.1/src/templates/c#/Dockerfile.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-05 16:46:37.000000 podman_init-1.0.1/src/templates/c#/docker-compose.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:46:45.435912 podman_init-1.0.1/src/templates/go/
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-05 16:46:37.000000 podman_init-1.0.1/src/templates/go/Dockerfile.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-05 16:46:37.000000 podman_init-1.0.1/src/templates/go/docker-compose.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:46:45.435912 podman_init-1.0.1/src/templates/java/
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-05 16:46:37.000000 podman_init-1.0.1/src/templates/java/Dockerfile.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-05 16:46:37.000000 podman_init-1.0.1/src/templates/java/docker-compose.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:46:45.435912 podman_init-1.0.1/src/templates/node/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-05 16:46:37.000000 podman_init-1.0.1/src/templates/node/Dockerfile.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-05 16:46:37.000000 podman_init-1.0.1/src/templates/node/docker-compose.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:46:45.435912 podman_init-1.0.1/src/templates/python/
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-05 16:46:37.000000 podman_init-1.0.1/src/templates/python/Dockerfile.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-05 16:46:37.000000 podman_init-1.0.1/src/templates/python/docker-compose.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:46:45.435912 podman_init-1.0.1/src/templates/rust/
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-05 16:46:37.000000 podman_init-1.0.1/src/templates/rust/Dockerfile.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-05 16:46:37.000000 podman_init-1.0.1/src/templates/rust/docker-compose.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:46:45.435912 podman_init-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10123 2024-05-05 16:46:37.000000 podman_init-1.0.1/tests/test_podman_init.py
```

### Comparing `podman-init-1.0.0/LICENSE` & `podman_init-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `podman-init-1.0.0/PKG-INFO` & `podman_init-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podman-init
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python command-line tool that automates the process of initializing Docker-related files for your projects.
 Home-page: https://github.com/suriya-mca/Podman_Init_Cli
 Author: Suriya
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `podman-init-1.0.0/README.md` & `podman_init-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `podman-init-1.0.0/podman_init.egg-info/PKG-INFO` & `podman_init-1.0.1/podman_init.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podman-init
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python command-line tool that automates the process of initializing Docker-related files for your projects.
 Home-page: https://github.com/suriya-mca/Podman_Init_Cli
 Author: Suriya
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `podman-init-1.0.0/podman_init.egg-info/SOURCES.txt` & `podman_init-1.0.1/podman_init.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `podman-init-1.0.0/setup.py` & `podman_init-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='podman-init',
-    version='1.0.0',
+    version='1.0.1',
     packages=find_packages(),
     package_data={'': ['templates/**/*.j2']},
     include_package_data=True,
     install_requires=[
         'click',
         'jinja2'
     ],
```

### Comparing `podman-init-1.0.0/src/main.py` & `podman_init-1.0.1/src/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,89 +16,107 @@
 
     match language:
         case "python":       
             framework = click.prompt('Choose framework', 
                                       type=click.Choice(['django', 'fastapi', 'flask', 'exit'], case_sensitive=False), 
                                       show_choices=True)
 
+            port = click.prompt('Choose port', 
+                                 type=int)
+
             if framework == 'exit':
                 click.echo(style("Exiting...", fg='red'))
                 sys.exit()
 
             template_dir = os.path.join(os.path.dirname(__file__), 'templates', language)
 
         case "java":        
             framework = click.prompt('Choose framework', 
                                       type=click.Choice(['spring', 'quarkus', 'micronaut', 'vertx', 'exit'], case_sensitive=False), 
                                       show_choices=True)
 
+            port = click.prompt('Choose port', 
+                                 type=int)
+
             if framework == 'exit':
                 click.echo(style("Exiting...", fg='red'))
                 sys.exit()
 
             template_dir = os.path.join(os.path.dirname(__file__), 'templates', language)
 
         case "go" :
             framework = click.prompt('Choose framework', 
                                       type=click.Choice(['gin', 'echo', 'chi', 'fiber', 'exit'], case_sensitive=False), 
                                       show_choices=True)
 
+            port = click.prompt('Choose port', 
+                                 type=int)
+
             if framework == 'exit':
                 click.echo(style("Exiting...", fg='red'))
                 sys.exit()
 
             template_dir = os.path.join(os.path.dirname(__file__), 'templates', language)
 
         case "node" :
             framework = click.prompt('Choose framework', 
                                       type=click.Choice(['express', 'nest', 'koa', 'fastify', 'exit'], case_sensitive=False), 
                                       show_choices=True)
 
+            port = click.prompt('Choose port', 
+                                 type=int)
+
             if framework == 'exit':
                 click.echo(style("Exiting...", fg='red'))
                 sys.exit()
 
             template_dir = os.path.join(os.path.dirname(__file__), 'templates', language)
 
         case "c#" :
             framework = click.prompt('Choose framework', 
                                       type=click.Choice(['.net core', 'blazor'], case_sensitive=False), 
                                       show_choices=True)
 
+            port = click.prompt('Choose port', 
+                                 type=int)
+
             if framework == 'exit':
                 click.echo(style("Exiting...", fg='red'))
                 sys.exit()
 
             template_dir = os.path.join(os.path.dirname(__file__), 'templates', language)
 
         case "rust" :
             framework = click.prompt('Choose framework', 
                                       type=click.Choice(['actix', 'axum', 'rocket', 'warp', 'tide', 'exit'], case_sensitive=False), 
                                       show_choices=True)
 
+            port = click.prompt('Choose port', 
+                                 type=int)
+
             if framework == 'exit':
                 click.echo(style("Exiting...", fg='red'))
                 sys.exit()
 
             template_dir = os.path.join(os.path.dirname(__file__), 'templates', language)
 
         case _:
             click.echo("Invalid language selected.")
             return
 
     load_jinja_env = Environment(loader=FileSystemLoader(template_dir))
 
     dockerfile_template = load_jinja_env.get_template('Dockerfile.j2')
-    dockerfile_content = dockerfile_template.render(project_name=project_name, framework=framework)
+    dockerfile_content = dockerfile_template.render(project_name=project_name, framework=framework, port=port)
 
     with open('Dockerfile', 'w') as f:
         f.write(dockerfile_content)
 
     compose_template = load_jinja_env.get_template('docker-compose.yml.j2')
-    compose_content = compose_template.render(project_name=project_name, framework=framework)
+    compose_content = compose_template.render(project_name=project_name, framework=framework, port=port)
 
     with open('docker-compose.yml', 'w') as f:
         f.write(compose_content)
 
     with open('.dockerignore', 'w') as f:
         f.write("*.pyc\n__pycache__/\n.git\n.gitignore\n*.env\n.vscode/\n.idea/\n")
```

### Comparing `podman-init-1.0.0/src/templates/c#/Dockerfile.j2` & `podman_init-1.0.1/src/templates/c#/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `podman-init-1.0.0/src/templates/go/Dockerfile.j2` & `podman_init-1.0.1/src/templates/go/Dockerfile.j2`

 * *Files 19% similar despite different names*

```diff
@@ -20,13 +20,11 @@
 # Start fresh from a smaller image
 FROM alpine:latest
 
 # Copy the pre-built binary from the previous stage
 COPY --from=build /app/main .
 
 # Expose port 3000 to the outside world
-{% if framework == 'gin' or framework == 'echo' %}EXPOSE 8080
-{% elif framework == 'chi' %}EXPOSE 3333
-{% elif framework == 'fiber' %}EXPOSE 3000
-{% endif %}
+EXPOSE {{ port }}
+
 # Command to run the executable
 CMD ["./main"]
```

### Comparing `podman-init-1.0.0/src/templates/java/Dockerfile.j2` & `podman_init-1.0.1/src/templates/java/Dockerfile.j2`

 * *Files 3% similar despite different names*

```diff
@@ -4,11 +4,11 @@
 # Set the working directory inside the container
 WORKDIR /src
 
 # Copy the packaged JAR file from the local filesystem to the container
 COPY target/*.jar /src/app.jar
 
 # Expose port 8080 to allow external access to the application
-EXPOSE 8080
+EXPOSE {{ port }}
 
 # Define the entry point to execute the application when the container starts
 ENTRYPOINT ["java", "-jar" , "app.jar"]
```

### Comparing `podman-init-1.0.0/src/templates/node/docker-compose.yml.j2` & `podman_init-1.0.1/src/templates/node/docker-compose.yml.j2`

 * *Files 22% similar despite different names*

```diff
@@ -6,14 +6,14 @@
       context: .
       dockerfile: Dockerfile
     {% if framework == 'express' %}container_name: express
     {% elif framework == 'nest' %}container_name: nest
     {% elif framework == 'koa' %}container_name: koa
     {% elif framework == 'fastify' %}container_name: fastify
     {% endif %}ports:
-      - "3000:3000"
+      - "{{ port }}:{{ port }}"
     volumes:
       - .:/usr/src/app     
     environment:
       NODE_ENV: development
 
     # Add additional configurations as needed
```

### Comparing `podman-init-1.0.0/src/templates/python/Dockerfile.j2` & `podman_init-1.0.1/src/templates/python/Dockerfile.j2`

 * *Files 8% similar despite different names*

```diff
@@ -14,22 +14,20 @@
 COPY . /app
 
 # Install dependencies
 RUN pip install --upgrade pip && \
 	pip install --no-cache-dir --upgrade -r requirements.txt && \
 
 # Expose ports and define startup commands based on selected framework
-{% if framework == 'django' %}EXPOSE 8000
-
+EXPOSE {{ port }}
+{% if framework == 'django' %}
 # Specify the entry point
 CMD ["python", "manage.py", "runserver"]
 
-{% elif framework == 'fastapi' %}EXPOSE 8000
-
-# # Specify the entry point (Replace "mail" with your actual file name)
+{% elif framework == 'fastapi' %}
+# Specify the entry point (Replace "mail" with your actual file name)
 CMD ["uvicorn", "main:app", "--host=0.0.0.0", "--reload"]
 
-{% elif framework == 'flask' %}EXPOSE 5000
-
+{% elif framework == 'flask' %}
 # Specify the entry point
 CMD ["flask", "run"]
 {% endif %}
```

### Comparing `podman-init-1.0.0/src/templates/rust/Dockerfile.j2` & `podman_init-1.0.1/src/templates/rust/Dockerfile.j2`

 * *Files 22% similar despite different names*

```diff
@@ -23,14 +23,11 @@
 # Create a new, lightweight image containing only the built application
 FROM debian:buster-slim
 
 # Copy the built application from the builder stage to the final image
 COPY --from=builder /usr/src/myapp/target/release/myapp .
 
 # Expose the port the Actix Web application will listen on
-{% if framework == 'actix' %}EXPOSE 8080
-{% elif framework == 'axum' %}EXPOSE 3000
-{% elif framework == 'rocket' or framework == 'tide' %}EXPOSE 8000
-{% elif framework == 'warp' %}EXPOSE 3030
-{% endif %}
+Expose {{ port }}
+
 # Command to run the application
 CMD ["./myapp"]
```

### Comparing `podman-init-1.0.0/tests/test_podman_init.py` & `podman_init-1.0.1/tests/test_podman_init.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,191 +2,246 @@
 import sys
 sys.path.append(os.path.join(os.path.dirname(__file__), '..', 'src'))
 from click.testing import CliRunner
 from main import podman_init
 
 def test_podman_init_python_flask():
     runner = CliRunner()
-    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'python'], input='flask\n')
+    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'python'], input='flask\n8000\n')
     assert result.exit_code == 0
     assert os.path.isfile('Dockerfile')
     assert os.path.isfile('docker-compose.yml')
     assert os.path.isfile('.dockerignore')
     os.remove('Dockerfile')
     os.remove('docker-compose.yml')
     os.remove('.dockerignore')
 
 def test_podman_init_python_fastapi():
     runner = CliRunner()
-    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'python'], input='fastapi\n')
+    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'python'], input='fastapi\n8000\n')
     assert result.exit_code == 0
     assert os.path.isfile('Dockerfile')
     assert os.path.isfile('docker-compose.yml')
     assert os.path.isfile('.dockerignore')
     os.remove('Dockerfile')
     os.remove('docker-compose.yml')
     os.remove('.dockerignore')
 
 def test_podman_init_python_django():
     runner = CliRunner()
-    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'python'], input='django\n')
+    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'python'], input='django\n8000\n')
     assert result.exit_code == 0
     assert os.path.isfile('Dockerfile')
     assert os.path.isfile('docker-compose.yml')
     assert os.path.isfile('.dockerignore')
     os.remove('Dockerfile')
     os.remove('docker-compose.yml')
     os.remove('.dockerignore')
 
 def test_podman_init_java_spring():
     runner = CliRunner()
-    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'java'], input='spring\n')
+    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'java'], input='spring\n8000\n')
     assert result.exit_code == 0
     assert os.path.isfile('Dockerfile')
     assert os.path.isfile('docker-compose.yml')
     assert os.path.isfile('.dockerignore')
     os.remove('Dockerfile')
     os.remove('docker-compose.yml')
     os.remove('.dockerignore')
 
 def test_podman_init_java_quarkus():
     runner = CliRunner()
-    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'java'], input='quarkus\n')
+    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'java'], input='quarkus\n8000\n')
     assert result.exit_code == 0
     assert os.path.isfile('Dockerfile')
     assert os.path.isfile('docker-compose.yml')
     assert os.path.isfile('.dockerignore')
     os.remove('Dockerfile')
     os.remove('docker-compose.yml')
     os.remove('.dockerignore')
 
 def test_podman_init_java_micronaut():
     runner = CliRunner()
-    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'java'], input='micronaut\n')
+    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'java'], input='micronaut\n8000\n')
     assert result.exit_code == 0
     assert os.path.isfile('Dockerfile')
     assert os.path.isfile('docker-compose.yml')
     assert os.path.isfile('.dockerignore')
     os.remove('Dockerfile')
     os.remove('docker-compose.yml')
     os.remove('.dockerignore')
 
 def test_podman_init_java_vertx():
     runner = CliRunner()
-    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'java'], input='vertx\n')
+    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'java'], input='vertx\n8000\n')
     assert result.exit_code == 0
     assert os.path.isfile('Dockerfile')
     assert os.path.isfile('docker-compose.yml')
     assert os.path.isfile('.dockerignore')
     os.remove('Dockerfile')
     os.remove('docker-compose.yml')
     os.remove('.dockerignore')
 
 def test_podman_init_go_gin():
     runner = CliRunner()
-    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'go'], input='gin\n')
+    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'go'], input='gin\n8000\n')
     assert result.exit_code == 0
     assert os.path.isfile('Dockerfile')
     assert os.path.isfile('docker-compose.yml')
     assert os.path.isfile('.dockerignore')
     os.remove('Dockerfile')
     os.remove('docker-compose.yml')
     os.remove('.dockerignore')
 
 def test_podman_init_go_echo():
     runner = CliRunner()
-    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'go'], input='echo\n')
+    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'go'], input='echo\n8000\n')
     assert result.exit_code == 0
     assert os.path.isfile('Dockerfile')
     assert os.path.isfile('docker-compose.yml')
     assert os.path.isfile('.dockerignore')
     os.remove('Dockerfile')
     os.remove('docker-compose.yml')
     os.remove('.dockerignore')
 
 def test_podman_init_go_chi():
     runner = CliRunner()
-    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'go'], input='chi\n')
+    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'go'], input='chi\n8000\n')
     assert result.exit_code == 0
     assert os.path.isfile('Dockerfile')
     assert os.path.isfile('docker-compose.yml')
     assert os.path.isfile('.dockerignore')
     os.remove('Dockerfile')
     os.remove('docker-compose.yml')
     os.remove('.dockerignore')
 
 def test_podman_init_go_fiber():
     runner = CliRunner()
-    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'go'], input='fiber\n')
+    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'go'], input='fiber\n8000\n')
     assert result.exit_code == 0
     assert os.path.isfile('Dockerfile')
     assert os.path.isfile('docker-compose.yml')
     assert os.path.isfile('.dockerignore')
     os.remove('Dockerfile')
     os.remove('docker-compose.yml')
     os.remove('.dockerignore')
 
 def test_podman_init_node_express():
     runner = CliRunner()
-    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'node'], input='express\n')
+    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'node'], input='express\n8000\n')
     assert result.exit_code == 0
     assert os.path.isfile('Dockerfile')
     assert os.path.isfile('docker-compose.yml')
     assert os.path.isfile('.dockerignore')
     os.remove('Dockerfile')
     os.remove('docker-compose.yml')
     os.remove('.dockerignore')
 
 def test_podman_init_node_nest():
     runner = CliRunner()
-    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'node'], input='nest\n')
+    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'node'], input='nest\n8000\n')
     assert result.exit_code == 0
     assert os.path.isfile('Dockerfile')
     assert os.path.isfile('docker-compose.yml')
     assert os.path.isfile('.dockerignore')
     os.remove('Dockerfile')
     os.remove('docker-compose.yml')
     os.remove('.dockerignore') 
 
 def test_podman_init_node_koa():
     runner = CliRunner()
-    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'node'], input='koa\n')
+    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'node'], input='koa\n8000\n')
     assert result.exit_code == 0
     assert os.path.isfile('Dockerfile')
     assert os.path.isfile('docker-compose.yml')
     assert os.path.isfile('.dockerignore')
     os.remove('Dockerfile')
     os.remove('docker-compose.yml')
     os.remove('.dockerignore') 
 
 def test_podman_init_node_fastify():
     runner = CliRunner()
-    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'node'], input='fastify\n')
+    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'node'], input='fastify\n8000\n')
     assert result.exit_code == 0
     assert os.path.isfile('Dockerfile')
     assert os.path.isfile('docker-compose.yml')
     assert os.path.isfile('.dockerignore')
     os.remove('Dockerfile')
     os.remove('docker-compose.yml')
     os.remove('.dockerignore')  
 
 def test_podman_init_chash_dotnet_core():
     runner = CliRunner()
-    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'c#'], input='.net core\n')
+    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'c#'], input='.net core\n8000\n')
     assert result.exit_code == 0
     assert os.path.isfile('Dockerfile')
     assert os.path.isfile('docker-compose.yml')
     assert os.path.isfile('.dockerignore')
     os.remove('Dockerfile')
     os.remove('docker-compose.yml')
     os.remove('.dockerignore')  
 
 def test_podman_init_chash_blazor():
     runner = CliRunner()
-    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'c#'], input='blazor\n')
+    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'c#'], input='blazor\n8000\n')
+    assert result.exit_code == 0
+    assert os.path.isfile('Dockerfile')
+    assert os.path.isfile('docker-compose.yml')
+    assert os.path.isfile('.dockerignore')
+    os.remove('Dockerfile')
+    os.remove('docker-compose.yml')
+    os.remove('.dockerignore')
+
+def test_podman_init_rust_actix():
+    runner = CliRunner()
+    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'rust'], input='actix\n8000\n')
+    assert result.exit_code == 0
+    assert os.path.isfile('Dockerfile')
+    assert os.path.isfile('docker-compose.yml')
+    assert os.path.isfile('.dockerignore')
+    os.remove('Dockerfile')
+    os.remove('docker-compose.yml')
+    os.remove('.dockerignore')
+
+def test_podman_init_rust_axum():
+    runner = CliRunner()
+    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'rust'], input='axum\n8000\n')
+    assert result.exit_code == 0
+    assert os.path.isfile('Dockerfile')
+    assert os.path.isfile('docker-compose.yml')
+    assert os.path.isfile('.dockerignore')
+    os.remove('Dockerfile')
+    os.remove('docker-compose.yml')
+    os.remove('.dockerignore')
+
+def test_podman_init_rust_rocket():
+    runner = CliRunner()
+    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'rust'], input='rocket\n8000\n')
+    assert result.exit_code == 0
+    assert os.path.isfile('Dockerfile')
+    assert os.path.isfile('docker-compose.yml')
+    assert os.path.isfile('.dockerignore')
+    os.remove('Dockerfile')
+    os.remove('docker-compose.yml')
+    os.remove('.dockerignore')
+
+def test_podman_init_rust_warp():
+    runner = CliRunner()
+    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'rust'], input='warp\n8000\n')
+    assert result.exit_code == 0
+    assert os.path.isfile('Dockerfile')
+    assert os.path.isfile('docker-compose.yml')
+    assert os.path.isfile('.dockerignore')
+    os.remove('Dockerfile')
+    os.remove('docker-compose.yml')
+    os.remove('.dockerignore')
+
+def test_podman_init_rust_tide():
+    runner = CliRunner()
+    result = runner.invoke(podman_init, ['--project-name', 'test_project', '--language', 'rust'], input='tide\n8000\n')
     assert result.exit_code == 0
     assert os.path.isfile('Dockerfile')
     assert os.path.isfile('docker-compose.yml')
     assert os.path.isfile('.dockerignore')
     os.remove('Dockerfile')
     os.remove('docker-compose.yml')
     os.remove('.dockerignore')
```

