# Comparing `tmp/cae_cli-0.0.1.tar.gz` & `tmp/cae_cli-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cae_cli-0.0.1.tar", last modified: Sun May  5 05:49:44 2024, max compression
+gzip compressed data, was "cae_cli-0.0.2.tar", last modified: Sun May  5 05:55:04 2024, max compression
```

## Comparing `cae_cli-0.0.1.tar` & `cae_cli-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 05:49:44.431594 cae_cli-0.0.1/
--rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      422 2024-05-05 05:49:44.430594 cae_cli-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 05:49:44.408595 cae_cli-0.0.1/cae_cli/
--rw-rw-rw-   0        0        0     7618 2024-05-05 04:35:29.000000 cae_cli-0.0.1/cae_cli/ArchFlowJavaWeb.py
--rw-rw-rw-   0        0        0      311 2024-05-05 04:41:52.000000 cae_cli-0.0.1/cae_cli/main.py
-drwxrwxrwx   0        0        0        0 2024-05-05 05:49:44.429595 cae_cli-0.0.1/cae_cli.egg-info/
--rw-rw-rw-   0        0        0      422 2024-05-05 05:49:44.000000 cae_cli-0.0.1/cae_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2024-05-05 05:49:44.000000 cae_cli-0.0.1/cae_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 05:49:44.000000 cae_cli-0.0.1/cae_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-05-05 05:49:44.000000 cae_cli-0.0.1/cae_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-05 05:49:44.000000 cae_cli-0.0.1/cae_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-05 05:49:44.431594 cae_cli-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      622 2024-05-05 05:49:38.000000 cae_cli-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 05:55:04.807978 cae_cli-0.0.2/
+-rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      422 2024-05-05 05:55:04.805977 cae_cli-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 05:55:04.787969 cae_cli-0.0.2/cae/
+-rw-rw-rw-   0        0        0     7618 2024-05-05 04:35:29.000000 cae_cli-0.0.2/cae/ArchFlowJavaWeb.py
+-rw-rw-rw-   0        0        0      311 2024-05-05 04:41:52.000000 cae_cli-0.0.2/cae/main.py
+drwxrwxrwx   0        0        0        0 2024-05-05 05:55:04.804980 cae_cli-0.0.2/cae_cli.egg-info/
+-rw-rw-rw-   0        0        0      422 2024-05-05 05:55:04.000000 cae_cli-0.0.2/cae_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2024-05-05 05:55:04.000000 cae_cli-0.0.2/cae_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 05:55:04.000000 cae_cli-0.0.2/cae_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-05 05:55:04.000000 cae_cli-0.0.2/cae_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-05 05:55:04.000000 cae_cli-0.0.2/cae_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-05 05:55:04.807978 cae_cli-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      614 2024-05-05 05:54:59.000000 cae_cli-0.0.2/setup.py
```

### Comparing `cae_cli-0.0.1/LICENSE` & `cae_cli-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cae_cli-0.0.1/README.md` & `cae_cli-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cae_cli-0.0.1/cae_cli/ArchFlowJavaWeb.py` & `cae_cli-0.0.2/cae/ArchFlowJavaWeb.py`

 * *Files identical despite different names*

### Comparing `cae_cli-0.0.1/setup.py` & `cae_cli-0.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup
 
 
 setup(name='cae-cli',
-    version='0.0.1',
+    version='0.0.2',
     license='Apache License',
     author='Carlos Vinicius Da Silva',
     long_description="teste da aplicação ainda",
     long_description_content_type="text/markdown",
     author_email='vini989073599@gmail.com',
     keywords='cae-cli',
     description=u'o cae tem como objetivo facilitar a utilização de projeto com arquitetura limpa',
-    packages=['cae_cli', 'cae_cli.templates'],
+    packages=['cae', 'cae.templates'],
     install_requires=[
         'arch-flow>=0.1.4',  # Dependência do cae-cli
         'colorama>=0.4.4'  # Dependência do arch-flow
       ],
 )
```

