# Comparing `tmp/django_nets_core-0.1.66.tar.gz` & `tmp/django-nets-core-0.1.69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_nets_core-0.1.66.tar", last modified: Sun May  5 01:00:25 2024, max compression
+gzip compressed data, was "django-nets-core-0.1.69.tar", last modified: Sun May  5 05:15:44 2024, max compression
```

## Comparing `django_nets_core-0.1.66.tar` & `django-nets-core-0.1.69.tar`

### file list

```diff
@@ -1,57 +1,61 @@
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 01:00:25.811136 django_nets_core-0.1.66/
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/LICENSE
--rw-rw-r--   0 dev       (1001) dev       (1001)      213 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/MANIFEST.in
--rw-r--r--   0 dev       (1001) dev       (1001)     5601 2024-05-05 01:00:25.811136 django_nets_core-0.1.66/PKG-INFO
--rw-rw-r--   0 dev       (1001) dev       (1001)     4358 2024-05-05 00:56:29.000000 django_nets_core-0.1.66/README.rst
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 01:00:25.807136 django_nets_core-0.1.66/django_nets_core.egg-info/
--rw-r--r--   0 dev       (1001) dev       (1001)     5601 2024-05-05 01:00:25.000000 django_nets_core-0.1.66/django_nets_core.egg-info/PKG-INFO
--rw-rw-r--   0 dev       (1001) dev       (1001)     1501 2024-05-05 01:00:25.000000 django_nets_core-0.1.66/django_nets_core.egg-info/SOURCES.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)        1 2024-05-05 01:00:25.000000 django_nets_core-0.1.66/django_nets_core.egg-info/dependency_links.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)      124 2024-05-05 01:00:25.000000 django_nets_core-0.1.66/django_nets_core.egg-info/requires.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)       10 2024-05-05 01:00:25.000000 django_nets_core-0.1.66/django_nets_core.egg-info/top_level.txt
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 01:00:25.807136 django_nets_core-0.1.66/nets_core/
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/__init__.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      206 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/apps.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      395 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/asgi.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      537 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/auth_urls.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3270 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/decorators.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3276 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/firebase_messages.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     6465 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/handlers.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     2477 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/listeners.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     4402 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/mail.py
--rwxrwxr-x   0 dev       (1001) dev       (1001)      665 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/manage.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 01:00:25.807136 django_nets_core-0.1.66/nets_core/middleware/
--rw-rw-r--   0 dev       (1001) dev       (1001)     2003 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/middleware/auth_token.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 01:00:25.807136 django_nets_core-0.1.66/nets_core/migrations/
--rw-rw-r--   0 dev       (1001) dev       (1001)     5274 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/migrations/0001_initial.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      422 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/migrations/0002_alter_verificationcode_token.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     2208 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/migrations/0003_userdevice.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      360 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/migrations/0004_remove_userdevice_device_id_userdevice_uuid.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      480 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/migrations/0005_userdevice_uuid.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      454 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/migrations/0006_verificationcode_device.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      533 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/migrations/0007_alter_verificationcode_device.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     2056 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      455 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/migrations/0009_userdevice_ip.py
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/migrations/__init__.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     8055 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/models.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     6425 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/params.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      902 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/responses.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3055 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/security.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3269 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/settings.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      610 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/tasks.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 01:00:25.803136 django_nets_core-0.1.66/nets_core/templates/
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 01:00:25.807136 django_nets_core-0.1.66/nets_core/templates/nets_core/
--rw-rw-r--   0 dev       (1001) dev       (1001)     6978 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/templates/nets_core/base.html
--rw-rw-r--   0 dev       (1001) dev       (1001)     1954 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/templates/nets_core/delete_account.html
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 01:00:25.807136 django_nets_core-0.1.66/nets_core/templates/nets_core/email/
--rw-rw-r--   0 dev       (1001) dev       (1001)    16103 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/templates/nets_core/email/base_email.html
--rw-rw-r--   0 dev       (1001) dev       (1001)     1032 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/templates/nets_core/email/new_login.html
--rw-rw-r--   0 dev       (1001) dev       (1001)      316 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/templates/nets_core/email/verification_code.html
--rw-rw-r--   0 dev       (1001) dev       (1001)      824 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/urls.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     1709 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/utils.py
--rw-rw-r--   0 dev       (1001) dev       (1001)    11692 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/views.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      395 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/nets_core/wsgi.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      100 2024-05-05 00:47:40.000000 django_nets_core-0.1.66/pyproject.toml
--rw-rw-r--   0 dev       (1001) dev       (1001)      167 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/requirements.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)     1149 2024-05-05 01:00:25.811136 django_nets_core-0.1.66/setup.cfg
--rw-rw-r--   0 dev       (1001) dev       (1001)       38 2024-05-04 23:43:26.000000 django_nets_core-0.1.66/setup.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 05:15:44.923482 django-nets-core-0.1.69/
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/LICENSE
+-rw-rw-r--   0 dev       (1001) dev       (1001)      213 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/MANIFEST.in
+-rw-rw-r--   0 dev       (1001) dev       (1001)     8569 2024-05-05 05:15:44.923482 django-nets-core-0.1.69/PKG-INFO
+-rw-rw-r--   0 dev       (1001) dev       (1001)     7520 2024-05-05 04:43:10.000000 django-nets-core-0.1.69/README.rst
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 05:15:44.919482 django-nets-core-0.1.69/django_nets_core.egg-info/
+-rw-r--r--   0 dev       (1001) dev       (1001)     8569 2024-05-05 05:15:44.000000 django-nets-core-0.1.69/django_nets_core.egg-info/PKG-INFO
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1608 2024-05-05 05:15:44.000000 django-nets-core-0.1.69/django_nets_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)        1 2024-05-05 05:15:44.000000 django-nets-core-0.1.69/django_nets_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)      286 2024-05-05 05:15:44.000000 django-nets-core-0.1.69/django_nets_core.egg-info/requires.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)       10 2024-05-05 05:15:44.000000 django-nets-core-0.1.69/django_nets_core.egg-info/top_level.txt
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 05:15:44.919482 django-nets-core-0.1.69/nets_core/
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/__init__.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      206 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/apps.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      807 2024-05-05 05:05:51.000000 django-nets-core-0.1.69/nets_core/asgi.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      537 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/auth_urls.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      229 2024-05-05 05:05:51.000000 django-nets-core-0.1.69/nets_core/celery.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3270 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/decorators.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3276 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/firebase_messages.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     6465 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/handlers.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2477 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/listeners.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     4402 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/mail.py
+-rwxrwxr-x   0 dev       (1001) dev       (1001)      665 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/manage.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 05:15:44.923482 django-nets-core-0.1.69/nets_core/middleware/
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 05:15:44.923482 django-nets-core-0.1.69/nets_core/middleware/__pycache__/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3004 2024-05-05 04:39:30.000000 django-nets-core-0.1.69/nets_core/middleware/__pycache__/auth_token.cpython-312.pyc
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2003 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/middleware/auth_token.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 05:15:44.923482 django-nets-core-0.1.69/nets_core/migrations/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     5274 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/migrations/0001_initial.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      422 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/migrations/0002_alter_verificationcode_token.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2208 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/migrations/0003_userdevice.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      360 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/migrations/0004_remove_userdevice_device_id_userdevice_uuid.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      480 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/migrations/0005_userdevice_uuid.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      454 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/migrations/0006_verificationcode_device.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      533 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/migrations/0007_alter_verificationcode_device.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2056 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      455 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/migrations/0009_userdevice_ip.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/migrations/__init__.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     8055 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/models.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     6425 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/params.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      902 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/responses.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3055 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/security.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3471 2024-05-05 05:01:32.000000 django-nets-core-0.1.69/nets_core/settings.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1820 2024-05-05 05:05:51.000000 django-nets-core-0.1.69/nets_core/settings_nets.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      610 2024-05-05 01:49:38.000000 django-nets-core-0.1.69/nets_core/tasks.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 05:15:44.919482 django-nets-core-0.1.69/nets_core/templates/
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 05:15:44.923482 django-nets-core-0.1.69/nets_core/templates/nets_core/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     6978 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/templates/nets_core/base.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1954 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/templates/nets_core/delete_account.html
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 05:15:44.923482 django-nets-core-0.1.69/nets_core/templates/nets_core/email/
+-rw-rw-r--   0 dev       (1001) dev       (1001)    16103 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/templates/nets_core/email/base_email.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1032 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/templates/nets_core/email/new_login.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)      316 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/templates/nets_core/email/verification_code.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)      824 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/urls.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1709 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/utils.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)    11692 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/views.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      395 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/wsgi.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      100 2024-05-05 00:47:40.000000 django-nets-core-0.1.69/pyproject.toml
+-rw-rw-r--   0 dev       (1001) dev       (1001)      181 2024-05-05 01:49:02.000000 django-nets-core-0.1.69/requirements.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1334 2024-05-05 05:15:44.923482 django-nets-core-0.1.69/setup.cfg
+-rw-rw-r--   0 dev       (1001) dev       (1001)       38 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/setup.py
```

### Comparing `django_nets_core-0.1.66/PKG-INFO` & `django-nets-core-0.1.69/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,67 +1,105 @@
-Metadata-Version: 2.1
-Name: django-nets-core
-Version: 0.1.66
-Summary: A lazy API rest request handler.
-Home-page: https://github.com/esbozos/django-nets-core
-Author: Norman Torres
-Author-email: norman.nets@gmail.com
-License: BSD-3-Clause
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 5.0
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-Requires-Dist: Django>=5.0.4
-Requires-Dist: pytz>=2024.1
-Requires-Dist: python-dateutil>=2.9.0.post0
-Requires-Dist: shortuuid>=1.0.13
-Requires-Dist: django-oauth-toolkit>=2.3.0
-Requires-Dist: firebase-admin>=6.5.0
-
 =========
 NETS CORE
 =========
 
 And set of lazy API request handlers and common tasks. 
 Just use it if you are really sure that you don't want to 
 repeat common tasks in request from many sources.
 
+REQUIREMENTS
+____________
+This package requires the following packages that will be installed automatically:
+
+    Django
+    pytz 
+    python-dateutil
+    shortuuid 
+    django-oauth-toolkit 
+    firebase-admin 
+    django-cors-headers
+    celery
+    django-celery-beat
+    djando-cors-headers
+    django-memcached
+    python-memcached
+    pymemcache
+    channels['daphne']
+
+NOTES:
+______
+    - For celery to work, you need to set up a broker, for example, RabbitMQ or Redis. see https://docs.celeryq.dev/en/stable/getting-started/backends-and-brokers/index.html and set it in settings.py
+    - Create a celery.py file in your project folder and set up the celery app see https://docs.celeryproject.org/en/stable/django/first-steps-with-django.html
+    - For django-celery-beat to work, you need to set up a scheduler, for example, RabbitMQ or Redis. see https://docs.celeryproject.org/en/stable/userguide/periodic-tasks.html#starting-the-scheduler and set it in settings.py
+    - For firebase to work, you need to set up a firebase project and download the credentials file and set it in settings.py as FIREBASE_CONFIG = os.path.join(BASE_DIR, 'firebase-credentials.json') see https://firebase.google.com/docs/admin/setup
+    - For django-oauth-toolkit to work, you need to set up the authentication backend in settings.py as AUTHENTICATION_BACKENDS = ['oauth2_provider.backends.OAuth2Backend'] see https://django-oauth-toolkit.readthedocs.io/en/latest/rest-framework/getting_started.html#step-1-configure-your-authentication-backends
+    - For django-cors-headers to work, you need to set up the middleware in settings.py as MIDDLEWARE = ['corsheaders.middleware.CorsMiddleware', 'django.middleware.common.CommonMiddleware'] see
+    
+
+COMMANDS:
+_________
+    
+    -./manage.py nets-settings --create # create settings required for nets_core
+    -./manage.py nets-settings  # will check if settings are set correctly
+    -./manage.py nets-settings --create --force # force create settings required for nets_core and overwrite existing settings if any
+
+
+INSTALLATION
+____________
+
+.. code-block:: bash
+
+    pip install django-nets-core
+
+Add 'nets_core' to your INSTALLED_APPS setting like this:
+
+.. code-block:: python
+
+    INSTALLED_APPS = [
+        ...
+        'oauth2_provider', # required for authentication
+        'nets_core',
+    ]
+
+Include the nets_core URLconf in your project urls.py like this:
+
+.. code-block:: python
+
+    path("", include("nets_core.auth_urls", namespace="auth")),
+
+
+USAGE
+_____
+
 
 .. code-block:: python
 
     # this already include csrf_exempt for API requests
     from nets_core.decorators import request_handle
     from nets_core.params import RequestParam
     from django.http import JsonResponse
 
+    from .models import MyModel
+
     @request_handle(
+        MyModel, # model that you want to use if view requires it, this return 404 if not found and check ownership or permissions test in can_do param
+        index_field='id' # field that will be used to get object from model, default is 'id',
 
         # params list that you want to get from request
         # this will be validated and converted to python types
         # if something is missing or wrong type, error will be raised
         # if public is True, this will be public in API and auth is not required
         # ensure you set you authentication methods in settings include OAuth2
         params=[
             RequestParam('name', str, optional=False),
         ],
         public=False, # default is False
+        can_do=['action', 'module'], # this will be check permission for action and module, if this permission does not exist this will create it, add permissions to users in admin panel
+        perm_required=False, # default is False, this will check if user has permission to do action or is owner of object, if set to TRUE only acces will be granted if can_do is passed
+
     )
     def my_view(request):
         # do something
         return JsonResponse({'ok': True})
         
 
 Cache is required for verification code:
```

### Comparing `django_nets_core-0.1.66/django_nets_core.egg-info/SOURCES.txt` & `django-nets-core-0.1.69/django_nets_core.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -10,31 +10,34 @@
 django_nets_core.egg-info/dependency_links.txt
 django_nets_core.egg-info/requires.txt
 django_nets_core.egg-info/top_level.txt
 nets_core/__init__.py
 nets_core/apps.py
 nets_core/asgi.py
 nets_core/auth_urls.py
+nets_core/celery.py
 nets_core/decorators.py
 nets_core/firebase_messages.py
 nets_core/handlers.py
 nets_core/listeners.py
 nets_core/mail.py
 nets_core/manage.py
 nets_core/models.py
 nets_core/params.py
 nets_core/responses.py
 nets_core/security.py
 nets_core/settings.py
+nets_core/settings_nets.py
 nets_core/tasks.py
 nets_core/urls.py
 nets_core/utils.py
 nets_core/views.py
 nets_core/wsgi.py
 nets_core/middleware/auth_token.py
+nets_core/middleware/__pycache__/auth_token.cpython-312.pyc
 nets_core/migrations/0001_initial.py
 nets_core/migrations/0002_alter_verificationcode_token.py
 nets_core/migrations/0003_userdevice.py
 nets_core/migrations/0004_remove_userdevice_device_id_userdevice_uuid.py
 nets_core/migrations/0005_userdevice_uuid.py
 nets_core/migrations/0006_verificationcode_device.py
 nets_core/migrations/0007_alter_verificationcode_device.py
```

### Comparing `django_nets_core-0.1.66/nets_core/auth_urls.py` & `django-nets-core-0.1.69/nets_core/auth_urls.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.66/nets_core/decorators.py` & `django-nets-core-0.1.69/nets_core/decorators.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.66/nets_core/firebase_messages.py` & `django-nets-core-0.1.69/nets_core/firebase_messages.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.66/nets_core/handlers.py` & `django-nets-core-0.1.69/nets_core/handlers.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.66/nets_core/listeners.py` & `django-nets-core-0.1.69/nets_core/listeners.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.66/nets_core/mail.py` & `django-nets-core-0.1.69/nets_core/mail.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.66/nets_core/manage.py` & `django-nets-core-0.1.69/nets_core/manage.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.66/nets_core/middleware/auth_token.py` & `django-nets-core-0.1.69/nets_core/middleware/auth_token.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.66/nets_core/migrations/0001_initial.py` & `django-nets-core-0.1.69/nets_core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.66/nets_core/migrations/0003_userdevice.py` & `django-nets-core-0.1.69/nets_core/migrations/0003_userdevice.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.66/nets_core/migrations/0007_alter_verificationcode_device.py` & `django-nets-core-0.1.69/nets_core/migrations/0007_alter_verificationcode_device.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.66/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py` & `django-nets-core-0.1.69/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.66/nets_core/models.py` & `django-nets-core-0.1.69/nets_core/models.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.66/nets_core/params.py` & `django-nets-core-0.1.69/nets_core/params.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.66/nets_core/responses.py` & `django-nets-core-0.1.69/nets_core/responses.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.66/nets_core/security.py` & `django-nets-core-0.1.69/nets_core/security.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.66/nets_core/settings.py` & `django-nets-core-0.1.69/nets_core/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 https://docs.djangoproject.com/en/4.1/ref/settings/
 """
 
 from pathlib import Path
 
 # Build paths inside the project like this: BASE_DIR / 'subdir'.
 BASE_DIR = Path(__file__).resolve().parent.parent
-
+    
 
 # Quick-start development settings - unsuitable for production
 # See https://docs.djangoproject.com/en/4.1/howto/deployment/checklist/
 
 # SECURITY WARNING: keep the secret key used in production secret!
 SECRET_KEY = 'django-insecure-bjq1kg5hbrzsk^6t2zm07t5j=3dyn6hkn%^k-#!yk3obj2lqyj'
 
@@ -119,7 +119,16 @@
 
 STATIC_URL = 'static/'
 
 # Default primary key field type
 # https://docs.djangoproject.com/en/4.1/ref/settings/#default-auto-field
 
 DEFAULT_AUTO_FIELD = 'django.db.models.BigAutoField'
+
+
+try:
+    from .settings_nets import *
+    print(f"Installe apps: {INSTALLED_APPS}")
+    print(f"ASGI: {ASGI_APPLICATION}")
+except ImportError:
+    print('No settings_nets.py file found')
+    pass
```

### Comparing `django_nets_core-0.1.66/nets_core/tasks.py` & `django-nets-core-0.1.69/nets_core/tasks.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.66/nets_core/templates/nets_core/base.html` & `django-nets-core-0.1.69/nets_core/templates/nets_core/base.html`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.66/nets_core/templates/nets_core/delete_account.html` & `django-nets-core-0.1.69/nets_core/templates/nets_core/delete_account.html`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.66/nets_core/templates/nets_core/email/base_email.html` & `django-nets-core-0.1.69/nets_core/templates/nets_core/email/base_email.html`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.66/nets_core/templates/nets_core/email/new_login.html` & `django-nets-core-0.1.69/nets_core/templates/nets_core/email/new_login.html`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.66/nets_core/urls.py` & `django-nets-core-0.1.69/nets_core/urls.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.66/nets_core/utils.py` & `django-nets-core-0.1.69/nets_core/utils.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.66/nets_core/views.py` & `django-nets-core-0.1.69/nets_core/views.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.66/setup.cfg` & `django-nets-core-0.1.69/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-nets-core
-version = 0.1.66
+version = 0.1.69
 description = A lazy API rest request handler.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/esbozos/django-nets-core
 author = Norman Torres
 author_email = norman.nets@gmail.com
 license = BSD-3-Clause
@@ -32,12 +32,20 @@
 install_requires = 
 	Django >= 5.0.4
 	pytz >= 2024.1
 	python-dateutil >= 2.9.0.post0
 	shortuuid >= 1.0.13
 	django-oauth-toolkit >= 2.3.0
 	firebase-admin >=6.5.0
+	celery >=5.4.0
+	django_celery_beat >= 2.6.0
+	django-cors-headers >= 4.3.1
+	pymemcache >= 4.0.0
+	python-memcached >= 1.62
+	django-memcached >= 0.1.2
+	channels >= 4.1.0
+	daphne >= 4.1.2
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

