# Comparing `tmp/cae_cli-0.0.9.tar.gz` & `tmp/cae_cli-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cae_cli-0.0.9.tar", last modified: Sun May  5 19:44:08 2024, max compression
+gzip compressed data, was "cae_cli-0.1.0.tar", last modified: Sun May  5 20:22:05 2024, max compression
```

## Comparing `cae_cli-0.0.9.tar` & `cae_cli-0.1.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 19:44:08.789946 cae_cli-0.0.9/
--rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.0.9/LICENSE
--rw-rw-rw-   0        0        0      408 2024-05-05 19:44:08.788945 cae_cli-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 19:44:08.756946 cae_cli-0.0.9/cae/
--rw-rw-rw-   0        0        0     7618 2024-05-05 04:35:29.000000 cae_cli-0.0.9/cae/ArchFlowJavaWeb.py
--rw-rw-rw-   0        0        0      344 2024-05-05 19:43:59.000000 cae_cli-0.0.9/cae/Run.py
--rw-rw-rw-   0        0        0       22 2024-05-05 19:42:37.000000 cae_cli-0.0.9/cae/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 19:44:08.771942 cae_cli-0.0.9/cae/templates/
--rw-rw-rw-   0        0        0     1034 2024-05-05 03:41:55.000000 cae_cli-0.0.9/cae/templates/assembler.txt
--rw-rw-rw-   0        0        0      328 2024-05-04 04:28:51.000000 cae_cli-0.0.9/cae/templates/dependency_wrapper.txt
--rw-rw-rw-   0        0        0      773 2024-05-05 03:55:59.000000 cae_cli-0.0.9/cae/templates/implementation_cuc.txt
--rw-rw-rw-   0        0        0      889 2024-05-05 03:57:58.000000 cae_cli-0.0.9/cae/templates/implementation_suc.txt
--rw-rw-rw-   0        0        0     1061 2024-05-04 02:53:55.000000 cae_cli-0.0.9/cae/templates/pom-adapters.txt
--rw-rw-rw-   0        0        0     1133 2024-05-04 03:01:34.000000 cae_cli-0.0.9/cae/templates/pom-assemblers.txt
--rw-rw-rw-   0        0        0     1288 2024-05-04 03:02:00.000000 cae_cli-0.0.9/cae/templates/pom-core.txt
--rw-rw-rw-   0        0        0      570 2024-05-04 04:12:40.000000 cae_cli-0.0.9/cae/templates/use_case.txt
--rw-rw-rw-   0        0        0      401 2024-05-05 04:01:36.000000 cae_cli-0.0.9/cae/templates/use_case_cuc.txt
--rw-rw-rw-   0        0        0     1128 2024-05-05 03:07:00.000000 cae_cli-0.0.9/cae/templates/use_case_factory.txt
--rw-rw-rw-   0        0        0     1058 2024-05-05 03:02:51.000000 cae_cli-0.0.9/cae/templates/use_case_implementation.txt
--rw-rw-rw-   0        0        0      387 2024-05-04 04:15:05.000000 cae_cli-0.0.9/cae/templates/use_case_input.txt
--rw-rw-rw-   0        0        0      397 2024-05-04 04:16:15.000000 cae_cli-0.0.9/cae/templates/use_case_output.txt
--rw-rw-rw-   0        0        0      410 2024-05-05 04:03:32.000000 cae_cli-0.0.9/cae/templates/use_case_suc.txt
-drwxrwxrwx   0        0        0        0 2024-05-05 19:44:08.787945 cae_cli-0.0.9/cae_cli.egg-info/
--rw-rw-rw-   0        0        0      408 2024-05-05 19:44:08.000000 cae_cli-0.0.9/cae_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      693 2024-05-05 19:44:08.000000 cae_cli-0.0.9/cae_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 19:44:08.000000 cae_cli-0.0.9/cae_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-05 19:44:08.000000 cae_cli-0.0.9/cae_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-05 19:44:08.000000 cae_cli-0.0.9/cae_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-05 19:44:08.789946 cae_cli-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      575 2024-05-05 19:44:06.000000 cae_cli-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 20:22:05.686971 cae_cli-0.1.0/
+-rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      408 2024-05-05 20:22:05.685971 cae_cli-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 20:22:05.646976 cae_cli-0.1.0/cae/
+-rw-rw-rw-   0        0        0     7618 2024-05-05 04:35:29.000000 cae_cli-0.1.0/cae/ArchFlowJavaWeb.py
+-rw-rw-rw-   0        0        0      345 2024-05-05 20:22:02.000000 cae_cli-0.1.0/cae/Run.py
+-rw-rw-rw-   0        0        0       22 2024-05-05 19:42:37.000000 cae_cli-0.1.0/cae/__init__.py
+-rw-rw-rw-   0        0        0     7302 2024-05-05 04:35:29.000000 cae_cli-0.1.0/cae/db.json
+drwxrwxrwx   0        0        0        0 2024-05-05 20:22:05.664925 cae_cli-0.1.0/cae/templates/
+-rw-rw-rw-   0        0        0     1034 2024-05-05 03:41:55.000000 cae_cli-0.1.0/cae/templates/assembler.txt
+-rw-rw-rw-   0        0        0      328 2024-05-04 04:28:51.000000 cae_cli-0.1.0/cae/templates/dependency_wrapper.txt
+-rw-rw-rw-   0        0        0      773 2024-05-05 03:55:59.000000 cae_cli-0.1.0/cae/templates/implementation_cuc.txt
+-rw-rw-rw-   0        0        0      889 2024-05-05 03:57:58.000000 cae_cli-0.1.0/cae/templates/implementation_suc.txt
+-rw-rw-rw-   0        0        0     1061 2024-05-04 02:53:55.000000 cae_cli-0.1.0/cae/templates/pom-adapters.txt
+-rw-rw-rw-   0        0        0     1133 2024-05-04 03:01:34.000000 cae_cli-0.1.0/cae/templates/pom-assemblers.txt
+-rw-rw-rw-   0        0        0     1288 2024-05-04 03:02:00.000000 cae_cli-0.1.0/cae/templates/pom-core.txt
+-rw-rw-rw-   0        0        0      570 2024-05-04 04:12:40.000000 cae_cli-0.1.0/cae/templates/use_case.txt
+-rw-rw-rw-   0        0        0      401 2024-05-05 04:01:36.000000 cae_cli-0.1.0/cae/templates/use_case_cuc.txt
+-rw-rw-rw-   0        0        0     1128 2024-05-05 03:07:00.000000 cae_cli-0.1.0/cae/templates/use_case_factory.txt
+-rw-rw-rw-   0        0        0     1058 2024-05-05 03:02:51.000000 cae_cli-0.1.0/cae/templates/use_case_implementation.txt
+-rw-rw-rw-   0        0        0      387 2024-05-04 04:15:05.000000 cae_cli-0.1.0/cae/templates/use_case_input.txt
+-rw-rw-rw-   0        0        0      397 2024-05-04 04:16:15.000000 cae_cli-0.1.0/cae/templates/use_case_output.txt
+-rw-rw-rw-   0        0        0      410 2024-05-05 04:03:32.000000 cae_cli-0.1.0/cae/templates/use_case_suc.txt
+drwxrwxrwx   0        0        0        0 2024-05-05 20:22:05.684970 cae_cli-0.1.0/cae_cli.egg-info/
+-rw-rw-rw-   0        0        0      408 2024-05-05 20:22:05.000000 cae_cli-0.1.0/cae_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      705 2024-05-05 20:22:05.000000 cae_cli-0.1.0/cae_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 20:22:05.000000 cae_cli-0.1.0/cae_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-05 20:22:05.000000 cae_cli-0.1.0/cae_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-05 20:22:05.000000 cae_cli-0.1.0/cae_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-05 20:22:05.686971 cae_cli-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      613 2024-05-05 20:22:02.000000 cae_cli-0.1.0/setup.py
```

### Comparing `cae_cli-0.0.9/LICENSE` & `cae_cli-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cae_cli-0.0.9/README.md` & `cae_cli-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cae_cli-0.0.9/cae/ArchFlowJavaWeb.py` & `cae_cli-0.1.0/cae/ArchFlowJavaWeb.py`

 * *Files identical despite different names*

### Comparing `cae_cli-0.0.9/cae/templates/assembler.txt` & `cae_cli-0.1.0/cae/templates/assembler.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.0.9/cae/templates/implementation_cuc.txt` & `cae_cli-0.1.0/cae/templates/implementation_cuc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.0.9/cae/templates/implementation_suc.txt` & `cae_cli-0.1.0/cae/templates/implementation_suc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.0.9/cae/templates/pom-adapters.txt` & `cae_cli-0.1.0/cae/templates/pom-adapters.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.0.9/cae/templates/pom-assemblers.txt` & `cae_cli-0.1.0/cae/templates/pom-assemblers.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.0.9/cae/templates/pom-core.txt` & `cae_cli-0.1.0/cae/templates/pom-core.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.0.9/cae/templates/use_case.txt` & `cae_cli-0.1.0/cae/templates/use_case.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.0.9/cae/templates/use_case_factory.txt` & `cae_cli-0.1.0/cae/templates/use_case_factory.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.0.9/cae/templates/use_case_implementation.txt` & `cae_cli-0.1.0/cae/templates/use_case_implementation.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.0.9/cae_cli.egg-info/SOURCES.txt` & `cae_cli-0.1.0/cae_cli.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 setup.py
 cae/ArchFlowJavaWeb.py
 cae/Run.py
 cae/__init__.py
+cae/db.json
 cae/templates/assembler.txt
 cae/templates/dependency_wrapper.txt
 cae/templates/implementation_cuc.txt
 cae/templates/implementation_suc.txt
 cae/templates/pom-adapters.txt
 cae/templates/pom-assemblers.txt
 cae/templates/pom-core.txt
```

### Comparing `cae_cli-0.0.9/setup.py` & `cae_cli-0.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from setuptools import setup
 
 
 setup(name='cae-cli',
-    version='0.0.9',
+    version='0.1.0',
     license='Apache License',
     author='Carlos Vinicius Da Silva',
     long_description="teste da aplicação ainda",
     long_description_content_type="text/markdown",
     author_email='vini989073599@gmail.com',
     keywords='cae-cli',
     description=u'o cae tem como objetivo facilitar a utilização de projeto com arquitetura limpa',
     packages=['cae'],
-    package_data={'cae': ['templates/*.txt']},
+    package_data={'cae': ['templates/*.txt'],
+                  'cae': ['*.json']},
     install_requires=[
         'arch-flow',
         'colorama'
       ],
 )
```

