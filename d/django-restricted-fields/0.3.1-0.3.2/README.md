# Comparing `tmp/django_restricted_fields-0.3.1.tar.gz` & `tmp/django_restricted_fields-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_restricted_fields-0.3.1.tar", last modified: Tue Apr 16 22:24:06 2024, max compression
+gzip compressed data, was "django_restricted_fields-0.3.2.tar", last modified: Sun May  5 12:05:48 2024, max compression
```

## Comparing `django_restricted_fields-0.3.1.tar` & `django_restricted_fields-0.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 lannert   (4779) lannert   (4779)        0 2024-04-16 22:24:06.868534 django_restricted_fields-0.3.1/
--rw-r--r--   0 lannert   (4779) lannert   (4779)     1065 2024-04-16 17:11:06.000000 django_restricted_fields-0.3.1/LICENSE
--rw-r--r--   0 lannert   (4779) lannert   (4779)     4883 2024-04-16 22:24:06.868534 django_restricted_fields-0.3.1/PKG-INFO
--rw-r--r--   0 lannert   (4779) lannert   (4779)      909 2024-04-16 18:53:25.000000 django_restricted_fields-0.3.1/README.md
--rw-r--r--   0 lannert   (4779) lannert   (4779)      923 2024-04-16 18:10:11.000000 django_restricted_fields-0.3.1/README.rst
--rw-r--r--   0 lannert   (4779) lannert   (4779)     1544 2024-04-16 19:01:07.000000 django_restricted_fields-0.3.1/pyproject.toml
--rw-r--r--   0 lannert   (4779) lannert   (4779)     2509 2024-04-16 18:40:14.000000 django_restricted_fields-0.3.1/requirements-dev.txt
--rw-r--r--   0 lannert   (4779) lannert   (4779)       14 2024-04-16 16:44:11.000000 django_restricted_fields-0.3.1/requirements.in
--rw-r--r--   0 lannert   (4779) lannert   (4779)       38 2024-04-16 22:24:06.868534 django_restricted_fields-0.3.1/setup.cfg
-drwxr-xr-x   0 lannert   (4779) lannert   (4779)        0 2024-04-16 22:24:06.860535 django_restricted_fields-0.3.1/src/
-drwxr-xr-x   0 lannert   (4779) lannert   (4779)        0 2024-04-16 22:24:06.864534 django_restricted_fields-0.3.1/src/django_restricted_fields/
--rw-r--r--   0 lannert   (4779) lannert   (4779)        6 2024-04-16 21:54:42.000000 django_restricted_fields-0.3.1/src/django_restricted_fields/VERSION
--rw-r--r--   0 lannert   (4779) lannert   (4779)        8 2024-04-16 16:58:10.000000 django_restricted_fields-0.3.1/src/django_restricted_fields/__init__.py
--rw-r--r--   0 lannert   (4779) lannert   (4779)     6989 2024-04-16 22:18:44.000000 django_restricted_fields-0.3.1/src/django_restricted_fields/forms.py
-drwxr-xr-x   0 lannert   (4779) lannert   (4779)        0 2024-04-16 22:24:06.864534 django_restricted_fields-0.3.1/src/django_restricted_fields.egg-info/
--rw-r--r--   0 lannert   (4779) lannert   (4779)     4883 2024-04-16 22:24:06.000000 django_restricted_fields-0.3.1/src/django_restricted_fields.egg-info/PKG-INFO
--rw-r--r--   0 lannert   (4779) lannert   (4779)      455 2024-04-16 22:24:06.000000 django_restricted_fields-0.3.1/src/django_restricted_fields.egg-info/SOURCES.txt
--rw-r--r--   0 lannert   (4779) lannert   (4779)        1 2024-04-16 22:24:06.000000 django_restricted_fields-0.3.1/src/django_restricted_fields.egg-info/dependency_links.txt
--rw-r--r--   0 lannert   (4779) lannert   (4779)     1076 2024-04-16 22:24:06.000000 django_restricted_fields-0.3.1/src/django_restricted_fields.egg-info/requires.txt
--rw-r--r--   0 lannert   (4779) lannert   (4779)       25 2024-04-16 22:24:06.000000 django_restricted_fields-0.3.1/src/django_restricted_fields.egg-info/top_level.txt
+drwxr-xr-x   0 lannert   (4779) lannert   (4779)        0 2024-05-05 12:05:48.427671 django_restricted_fields-0.3.2/
+-rw-r--r--   0 lannert   (4779) lannert   (4779)     1065 2024-04-16 17:11:06.000000 django_restricted_fields-0.3.2/LICENSE
+-rw-r--r--   0 lannert   (4779) lannert   (4779)     4882 2024-05-05 12:05:48.427671 django_restricted_fields-0.3.2/PKG-INFO
+-rw-r--r--   0 lannert   (4779) lannert   (4779)      909 2024-04-16 18:53:25.000000 django_restricted_fields-0.3.2/README.md
+-rw-r--r--   0 lannert   (4779) lannert   (4779)      923 2024-04-16 18:10:11.000000 django_restricted_fields-0.3.2/README.rst
+-rw-r--r--   0 lannert   (4779) lannert   (4779)     1543 2024-05-05 11:44:40.000000 django_restricted_fields-0.3.2/pyproject.toml
+-rw-r--r--   0 lannert   (4779) lannert   (4779)     2509 2024-04-16 18:40:14.000000 django_restricted_fields-0.3.2/requirements-dev.txt
+-rw-r--r--   0 lannert   (4779) lannert   (4779)       14 2024-04-16 16:44:11.000000 django_restricted_fields-0.3.2/requirements.in
+-rw-r--r--   0 lannert   (4779) lannert   (4779)       38 2024-05-05 12:05:48.427671 django_restricted_fields-0.3.2/setup.cfg
+drwxr-xr-x   0 lannert   (4779) lannert   (4779)        0 2024-05-05 12:05:48.415671 django_restricted_fields-0.3.2/src/
+drwxr-xr-x   0 lannert   (4779) lannert   (4779)        0 2024-05-05 12:05:48.419671 django_restricted_fields-0.3.2/src/django_restricted_fields/
+-rw-r--r--   0 lannert   (4779) lannert   (4779)        6 2024-05-05 11:44:54.000000 django_restricted_fields-0.3.2/src/django_restricted_fields/VERSION
+-rw-r--r--   0 lannert   (4779) lannert   (4779)        8 2024-04-16 16:58:10.000000 django_restricted_fields-0.3.2/src/django_restricted_fields/__init__.py
+-rw-r--r--   0 lannert   (4779) lannert   (4779)     6989 2024-04-16 22:18:44.000000 django_restricted_fields-0.3.2/src/django_restricted_fields/forms.py
+drwxr-xr-x   0 lannert   (4779) lannert   (4779)        0 2024-05-05 12:05:48.419671 django_restricted_fields-0.3.2/src/django_restricted_fields.egg-info/
+-rw-r--r--   0 lannert   (4779) lannert   (4779)     4882 2024-05-05 12:05:48.000000 django_restricted_fields-0.3.2/src/django_restricted_fields.egg-info/PKG-INFO
+-rw-r--r--   0 lannert   (4779) lannert   (4779)      455 2024-05-05 12:05:48.000000 django_restricted_fields-0.3.2/src/django_restricted_fields.egg-info/SOURCES.txt
+-rw-r--r--   0 lannert   (4779) lannert   (4779)        1 2024-05-05 12:05:48.000000 django_restricted_fields-0.3.2/src/django_restricted_fields.egg-info/dependency_links.txt
+-rw-r--r--   0 lannert   (4779) lannert   (4779)     1076 2024-05-05 12:05:48.000000 django_restricted_fields-0.3.2/src/django_restricted_fields.egg-info/requires.txt
+-rw-r--r--   0 lannert   (4779) lannert   (4779)       25 2024-05-05 12:05:48.000000 django_restricted_fields-0.3.2/src/django_restricted_fields.egg-info/top_level.txt
```

### Comparing `django_restricted_fields-0.3.1/LICENSE` & `django_restricted_fields-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_restricted_fields-0.3.1/PKG-INFO` & `django_restricted_fields-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-restricted-fields
-Version: 0.3.1
+Version: 0.3.2
 Summary: Provides date and date/time fields with restrictions for Django forms.
 Author-email: Detlef Lannert <detlef@lannert.de>
 Maintainer-email: Detlef Lannert <detlef@lannert.de>
 Project-URL: Homepage, https://github.com/detlefla/django-restricted-fields
 Project-URL: Repository, https://github.com/detlefla/django-restricted-fields
 Project-URL: Issues, https://github.com/detlefla/django-restricted-fields/issues
 Keywords: web,django,forms
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Django
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: django>=4.0
 Provides-Extra: dev
 Requires-Dist: asgiref==3.8.1; extra == "dev"
 Requires-Dist: asttokens==2.4.1; extra == "dev"
 Requires-Dist: backports-tarfile==1.1.0; extra == "dev"
```

### Comparing `django_restricted_fields-0.3.1/README.md` & `django_restricted_fields-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `django_restricted_fields-0.3.1/README.rst` & `django_restricted_fields-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `django_restricted_fields-0.3.1/pyproject.toml` & `django_restricted_fields-0.3.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "django-restricted-fields"
 #dynamic = ["version", "readme", "dependencies"]
 dynamic = ["version", "readme", "dependencies", "optional-dependencies"]
 description = "Provides date and date/time fields with restrictions for Django forms."
 keywords = ["web", "django", "forms"]
-requires-python = ">= 3.10"
+requires-python = ">= 3.9"
 authors = [
   {name = "Detlef Lannert", email = "detlef@lannert.de"},
 ]
 maintainers = [
   {name = "Detlef Lannert", email = "detlef@lannert.de"},
 ]
 classifiers = [
```

### Comparing `django_restricted_fields-0.3.1/requirements-dev.txt` & `django_restricted_fields-0.3.2/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `django_restricted_fields-0.3.1/src/django_restricted_fields/forms.py` & `django_restricted_fields-0.3.2/src/django_restricted_fields/forms.py`

 * *Files identical despite different names*

### Comparing `django_restricted_fields-0.3.1/src/django_restricted_fields.egg-info/PKG-INFO` & `django_restricted_fields-0.3.2/src/django_restricted_fields.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-restricted-fields
-Version: 0.3.1
+Version: 0.3.2
 Summary: Provides date and date/time fields with restrictions for Django forms.
 Author-email: Detlef Lannert <detlef@lannert.de>
 Maintainer-email: Detlef Lannert <detlef@lannert.de>
 Project-URL: Homepage, https://github.com/detlefla/django-restricted-fields
 Project-URL: Repository, https://github.com/detlefla/django-restricted-fields
 Project-URL: Issues, https://github.com/detlefla/django-restricted-fields/issues
 Keywords: web,django,forms
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Django
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: django>=4.0
 Provides-Extra: dev
 Requires-Dist: asgiref==3.8.1; extra == "dev"
 Requires-Dist: asttokens==2.4.1; extra == "dev"
 Requires-Dist: backports-tarfile==1.1.0; extra == "dev"
```

### Comparing `django_restricted_fields-0.3.1/src/django_restricted_fields.egg-info/requires.txt` & `django_restricted_fields-0.3.2/src/django_restricted_fields.egg-info/requires.txt`

 * *Files identical despite different names*

