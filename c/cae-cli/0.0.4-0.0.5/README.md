# Comparing `tmp/cae_cli-0.0.4.tar.gz` & `tmp/cae_cli-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cae_cli-0.0.4.tar", last modified: Sun May  5 06:08:00 2024, max compression
+gzip compressed data, was "cae_cli-0.0.5.tar", last modified: Sun May  5 19:05:53 2024, max compression
```

## Comparing `cae_cli-0.0.4.tar` & `cae_cli-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 06:08:00.940879 cae_cli-0.0.4/
--rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      422 2024-05-05 06:08:00.939879 cae_cli-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 06:08:00.922879 cae_cli-0.0.4/cae/
--rw-rw-rw-   0        0        0     7618 2024-05-05 04:35:29.000000 cae_cli-0.0.4/cae/ArchFlowJavaWeb.py
--rw-rw-rw-   0        0        0       22 2024-05-05 06:06:31.000000 cae_cli-0.0.4/cae/__init__.py
--rw-rw-rw-   0        0        0      311 2024-05-05 04:41:52.000000 cae_cli-0.0.4/cae/main.py
-drwxrwxrwx   0        0        0        0 2024-05-05 06:08:00.938881 cae_cli-0.0.4/cae_cli.egg-info/
--rw-rw-rw-   0        0        0      422 2024-05-05 06:08:00.000000 cae_cli-0.0.4/cae_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2024-05-05 06:08:00.000000 cae_cli-0.0.4/cae_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 06:08:00.000000 cae_cli-0.0.4/cae_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-05-05 06:08:00.000000 cae_cli-0.0.4/cae_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-05 06:08:00.000000 cae_cli-0.0.4/cae_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-05 06:08:00.940879 cae_cli-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      614 2024-05-05 06:07:56.000000 cae_cli-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 19:05:53.144404 cae_cli-0.0.5/
+-rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      422 2024-05-05 19:05:53.143894 cae_cli-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 19:05:53.121826 cae_cli-0.0.5/cae/
+-rw-rw-rw-   0        0        0     7618 2024-05-05 04:35:29.000000 cae_cli-0.0.5/cae/ArchFlowJavaWeb.py
+-rw-rw-rw-   0        0        0       33 2024-05-05 18:54:25.000000 cae_cli-0.0.5/cae/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 19:05:53.143090 cae_cli-0.0.5/cae_cli.egg-info/
+-rw-rw-rw-   0        0        0      422 2024-05-05 19:05:53.000000 cae_cli-0.0.5/cae_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2024-05-05 19:05:53.000000 cae_cli-0.0.5/cae_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 19:05:53.000000 cae_cli-0.0.5/cae_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-05 19:05:53.000000 cae_cli-0.0.5/cae_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-05 19:05:53.000000 cae_cli-0.0.5/cae_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-05 19:05:53.145414 cae_cli-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      614 2024-05-05 19:05:47.000000 cae_cli-0.0.5/setup.py
```

### Comparing `cae_cli-0.0.4/LICENSE` & `cae_cli-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cae_cli-0.0.4/README.md` & `cae_cli-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `cae_cli-0.0.4/cae/ArchFlowJavaWeb.py` & `cae_cli-0.0.5/cae/ArchFlowJavaWeb.py`

 * *Files identical despite different names*

### Comparing `cae_cli-0.0.4/setup.py` & `cae_cli-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='cae-cli',
-    version='0.0.4',
+    version='0.0.5',
     license='Apache License',
     author='Carlos Vinicius Da Silva',
     long_description="teste da aplicação ainda",
     long_description_content_type="text/markdown",
     author_email='vini989073599@gmail.com',
     keywords='cae-cli',
     description=u'o cae tem como objetivo facilitar a utilização de projeto com arquitetura limpa',
```

