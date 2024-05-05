# Comparing `tmp/django-nets-core-0.1.69.tar.gz` & `tmp/django-nets-core-0.1.70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-nets-core-0.1.69.tar", last modified: Sun May  5 05:15:44 2024, max compression
+gzip compressed data, was "django-nets-core-0.1.70.tar", last modified: Sun May  5 15:45:41 2024, max compression
```

## Comparing `django-nets-core-0.1.69.tar` & `django-nets-core-0.1.70.tar`

### file list

```diff
@@ -1,61 +1,68 @@
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 05:15:44.923482 django-nets-core-0.1.69/
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/LICENSE
--rw-rw-r--   0 dev       (1001) dev       (1001)      213 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/MANIFEST.in
--rw-rw-r--   0 dev       (1001) dev       (1001)     8569 2024-05-05 05:15:44.923482 django-nets-core-0.1.69/PKG-INFO
--rw-rw-r--   0 dev       (1001) dev       (1001)     7520 2024-05-05 04:43:10.000000 django-nets-core-0.1.69/README.rst
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 05:15:44.919482 django-nets-core-0.1.69/django_nets_core.egg-info/
--rw-r--r--   0 dev       (1001) dev       (1001)     8569 2024-05-05 05:15:44.000000 django-nets-core-0.1.69/django_nets_core.egg-info/PKG-INFO
--rw-rw-r--   0 dev       (1001) dev       (1001)     1608 2024-05-05 05:15:44.000000 django-nets-core-0.1.69/django_nets_core.egg-info/SOURCES.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)        1 2024-05-05 05:15:44.000000 django-nets-core-0.1.69/django_nets_core.egg-info/dependency_links.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)      286 2024-05-05 05:15:44.000000 django-nets-core-0.1.69/django_nets_core.egg-info/requires.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)       10 2024-05-05 05:15:44.000000 django-nets-core-0.1.69/django_nets_core.egg-info/top_level.txt
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 05:15:44.919482 django-nets-core-0.1.69/nets_core/
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/__init__.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      206 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/apps.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      807 2024-05-05 05:05:51.000000 django-nets-core-0.1.69/nets_core/asgi.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      537 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/auth_urls.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      229 2024-05-05 05:05:51.000000 django-nets-core-0.1.69/nets_core/celery.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3270 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/decorators.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3276 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/firebase_messages.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     6465 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/handlers.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     2477 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/listeners.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     4402 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/mail.py
--rwxrwxr-x   0 dev       (1001) dev       (1001)      665 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/manage.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 05:15:44.923482 django-nets-core-0.1.69/nets_core/middleware/
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 05:15:44.923482 django-nets-core-0.1.69/nets_core/middleware/__pycache__/
--rw-rw-r--   0 dev       (1001) dev       (1001)     3004 2024-05-05 04:39:30.000000 django-nets-core-0.1.69/nets_core/middleware/__pycache__/auth_token.cpython-312.pyc
--rw-rw-r--   0 dev       (1001) dev       (1001)     2003 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/middleware/auth_token.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 05:15:44.923482 django-nets-core-0.1.69/nets_core/migrations/
--rw-rw-r--   0 dev       (1001) dev       (1001)     5274 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/migrations/0001_initial.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      422 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/migrations/0002_alter_verificationcode_token.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     2208 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/migrations/0003_userdevice.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      360 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/migrations/0004_remove_userdevice_device_id_userdevice_uuid.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      480 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/migrations/0005_userdevice_uuid.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      454 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/migrations/0006_verificationcode_device.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      533 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/migrations/0007_alter_verificationcode_device.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     2056 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      455 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/migrations/0009_userdevice_ip.py
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/migrations/__init__.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     8055 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/models.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     6425 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/params.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      902 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/responses.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3055 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/security.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3471 2024-05-05 05:01:32.000000 django-nets-core-0.1.69/nets_core/settings.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     1820 2024-05-05 05:05:51.000000 django-nets-core-0.1.69/nets_core/settings_nets.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      610 2024-05-05 01:49:38.000000 django-nets-core-0.1.69/nets_core/tasks.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 05:15:44.919482 django-nets-core-0.1.69/nets_core/templates/
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 05:15:44.923482 django-nets-core-0.1.69/nets_core/templates/nets_core/
--rw-rw-r--   0 dev       (1001) dev       (1001)     6978 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/templates/nets_core/base.html
--rw-rw-r--   0 dev       (1001) dev       (1001)     1954 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/templates/nets_core/delete_account.html
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 05:15:44.923482 django-nets-core-0.1.69/nets_core/templates/nets_core/email/
--rw-rw-r--   0 dev       (1001) dev       (1001)    16103 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/templates/nets_core/email/base_email.html
--rw-rw-r--   0 dev       (1001) dev       (1001)     1032 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/templates/nets_core/email/new_login.html
--rw-rw-r--   0 dev       (1001) dev       (1001)      316 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/templates/nets_core/email/verification_code.html
--rw-rw-r--   0 dev       (1001) dev       (1001)      824 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/urls.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     1709 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/utils.py
--rw-rw-r--   0 dev       (1001) dev       (1001)    11692 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/views.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      395 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/nets_core/wsgi.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      100 2024-05-05 00:47:40.000000 django-nets-core-0.1.69/pyproject.toml
--rw-rw-r--   0 dev       (1001) dev       (1001)      181 2024-05-05 01:49:02.000000 django-nets-core-0.1.69/requirements.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)     1334 2024-05-05 05:15:44.923482 django-nets-core-0.1.69/setup.cfg
--rw-rw-r--   0 dev       (1001) dev       (1001)       38 2024-05-04 23:43:26.000000 django-nets-core-0.1.69/setup.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:45:41.811035 django-nets-core-0.1.70/
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/LICENSE
+-rw-rw-r--   0 dev       (1001) dev       (1001)      254 2024-05-05 15:45:38.000000 django-nets-core-0.1.70/MANIFEST.in
+-rw-rw-r--   0 dev       (1001) dev       (1001)     8702 2024-05-05 15:45:41.811035 django-nets-core-0.1.70/PKG-INFO
+-rw-rw-r--   0 dev       (1001) dev       (1001)     7653 2024-05-05 05:21:24.000000 django-nets-core-0.1.70/README.rst
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:45:41.807036 django-nets-core-0.1.70/django_nets_core.egg-info/
+-rw-r--r--   0 dev       (1001) dev       (1001)     8702 2024-05-05 15:45:41.000000 django-nets-core-0.1.70/django_nets_core.egg-info/PKG-INFO
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1836 2024-05-05 15:45:41.000000 django-nets-core-0.1.70/django_nets_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)        1 2024-05-05 15:45:41.000000 django-nets-core-0.1.70/django_nets_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)      286 2024-05-05 15:45:41.000000 django-nets-core-0.1.70/django_nets_core.egg-info/requires.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)       10 2024-05-05 15:45:41.000000 django-nets-core-0.1.70/django_nets_core.egg-info/top_level.txt
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:45:41.807036 django-nets-core-0.1.70/nets_core/
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/__init__.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      206 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/apps.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      807 2024-05-05 05:05:51.000000 django-nets-core-0.1.70/nets_core/asgi.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      537 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/auth_urls.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      229 2024-05-05 05:05:51.000000 django-nets-core-0.1.70/nets_core/celery.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3270 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/decorators.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3276 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/firebase_messages.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     6465 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/handlers.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2477 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/listeners.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     4402 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/mail.py
+-rwxrwxr-x   0 dev       (1001) dev       (1001)      665 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/manage.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:45:41.803036 django-nets-core-0.1.70/nets_core/management/
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:45:41.807036 django-nets-core-0.1.70/nets_core/management/commands/
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-05 02:03:24.000000 django-nets-core-0.1.70/nets_core/management/commands/__init__.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:45:41.807036 django-nets-core-0.1.70/nets_core/management/commands/__pycache__/
+-rw-rw-r--   0 dev       (1001) dev       (1001)      165 2024-05-05 02:44:07.000000 django-nets-core-0.1.70/nets_core/management/commands/__pycache__/__init__.cpython-312.pyc
+-rw-rw-r--   0 dev       (1001) dev       (1001)    28055 2024-05-05 05:05:51.000000 django-nets-core-0.1.70/nets_core/management/commands/__pycache__/nets-settings.cpython-312.pyc
+-rw-rw-r--   0 dev       (1001) dev       (1001)    23169 2024-05-05 05:05:47.000000 django-nets-core-0.1.70/nets_core/management/commands/nets-settings.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:45:41.807036 django-nets-core-0.1.70/nets_core/middleware/
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:45:41.811035 django-nets-core-0.1.70/nets_core/middleware/__pycache__/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3004 2024-05-05 04:39:30.000000 django-nets-core-0.1.70/nets_core/middleware/__pycache__/auth_token.cpython-312.pyc
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2003 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/middleware/auth_token.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:45:41.811035 django-nets-core-0.1.70/nets_core/migrations/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     5274 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/migrations/0001_initial.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      422 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/migrations/0002_alter_verificationcode_token.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2208 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/migrations/0003_userdevice.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      360 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/migrations/0004_remove_userdevice_device_id_userdevice_uuid.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      480 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/migrations/0005_userdevice_uuid.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      454 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/migrations/0006_verificationcode_device.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      533 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/migrations/0007_alter_verificationcode_device.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2056 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      455 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/migrations/0009_userdevice_ip.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/migrations/__init__.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     8055 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/models.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     6425 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/params.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      902 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/responses.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3055 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/security.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3471 2024-05-05 05:01:32.000000 django-nets-core-0.1.70/nets_core/settings.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1820 2024-05-05 05:05:51.000000 django-nets-core-0.1.70/nets_core/settings_nets.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      753 2024-05-05 05:16:02.000000 django-nets-core-0.1.70/nets_core/tasks.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:45:41.803036 django-nets-core-0.1.70/nets_core/templates/
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:45:41.811035 django-nets-core-0.1.70/nets_core/templates/nets_core/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     6978 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/templates/nets_core/base.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1954 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/templates/nets_core/delete_account.html
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:45:41.811035 django-nets-core-0.1.70/nets_core/templates/nets_core/email/
+-rw-rw-r--   0 dev       (1001) dev       (1001)    16103 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/templates/nets_core/email/base_email.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1032 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/templates/nets_core/email/new_login.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)      316 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/templates/nets_core/email/verification_code.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)      824 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/urls.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1709 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/utils.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)    11692 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/views.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      395 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/wsgi.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      100 2024-05-05 00:47:40.000000 django-nets-core-0.1.70/pyproject.toml
+-rw-rw-r--   0 dev       (1001) dev       (1001)      181 2024-05-05 01:49:02.000000 django-nets-core-0.1.70/requirements.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1334 2024-05-05 15:45:41.811035 django-nets-core-0.1.70/setup.cfg
+-rw-rw-r--   0 dev       (1001) dev       (1001)       38 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/setup.py
```

### Comparing `django-nets-core-0.1.69/PKG-INFO` & `django-nets-core-0.1.70/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-nets-core
-Version: 0.1.69
+Version: 0.1.70
 Summary: A lazy API rest request handler.
 Home-page: https://github.com/esbozos/django-nets-core
 Author: Norman Torres
 Author-email: norman.nets@gmail.com
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -61,18 +61,36 @@
     - For firebase to work, you need to set up a firebase project and download the credentials file and set it in settings.py as FIREBASE_CONFIG = os.path.join(BASE_DIR, 'firebase-credentials.json') see https://firebase.google.com/docs/admin/setup
     - For django-oauth-toolkit to work, you need to set up the authentication backend in settings.py as AUTHENTICATION_BACKENDS = ['oauth2_provider.backends.OAuth2Backend'] see https://django-oauth-toolkit.readthedocs.io/en/latest/rest-framework/getting_started.html#step-1-configure-your-authentication-backends
     - For django-cors-headers to work, you need to set up the middleware in settings.py as MIDDLEWARE = ['corsheaders.middleware.CorsMiddleware', 'django.middleware.common.CommonMiddleware'] see
     
 
 COMMANDS:
 _________
+
+check if settings are set correctly
+.. code-block:: bash
     
-    -./manage.py nets-settings --create # create settings required for nets_core
-    -./manage.py nets-settings  # will check if settings are set correctly
-    -./manage.py nets-settings --create --force # force create settings required for nets_core and overwrite existing settings if any
+    ./manage.py nets-settings
+
+create settings required for nets_core
+.. code-block:: bash
+    
+    ./manage.py nets-settings --create 
+
+force create settings required for nets_core and overwrite existing settings if any
+.. code-block:: bash
+
+    ./manage.py nets-settings --create --force 
+
+create superuser
+.. code-block:: bash
+
+    ./manage.py createsuperuser
+
+
 
 
 INSTALLATION
 ____________
 
 .. code-block:: bash
```

### Comparing `django-nets-core-0.1.69/README.rst` & `django-nets-core-0.1.70/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -33,18 +33,36 @@
     - For firebase to work, you need to set up a firebase project and download the credentials file and set it in settings.py as FIREBASE_CONFIG = os.path.join(BASE_DIR, 'firebase-credentials.json') see https://firebase.google.com/docs/admin/setup
     - For django-oauth-toolkit to work, you need to set up the authentication backend in settings.py as AUTHENTICATION_BACKENDS = ['oauth2_provider.backends.OAuth2Backend'] see https://django-oauth-toolkit.readthedocs.io/en/latest/rest-framework/getting_started.html#step-1-configure-your-authentication-backends
     - For django-cors-headers to work, you need to set up the middleware in settings.py as MIDDLEWARE = ['corsheaders.middleware.CorsMiddleware', 'django.middleware.common.CommonMiddleware'] see
     
 
 COMMANDS:
 _________
+
+check if settings are set correctly
+.. code-block:: bash
     
-    -./manage.py nets-settings --create # create settings required for nets_core
-    -./manage.py nets-settings  # will check if settings are set correctly
-    -./manage.py nets-settings --create --force # force create settings required for nets_core and overwrite existing settings if any
+    ./manage.py nets-settings
+
+create settings required for nets_core
+.. code-block:: bash
+    
+    ./manage.py nets-settings --create 
+
+force create settings required for nets_core and overwrite existing settings if any
+.. code-block:: bash
+
+    ./manage.py nets-settings --create --force 
+
+create superuser
+.. code-block:: bash
+
+    ./manage.py createsuperuser
+
+
 
 
 INSTALLATION
 ____________
 
 .. code-block:: bash
```

### Comparing `django-nets-core-0.1.69/django_nets_core.egg-info/PKG-INFO` & `django-nets-core-0.1.70/django_nets_core.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-nets-core
-Version: 0.1.69
+Version: 0.1.70
 Summary: A lazy API rest request handler.
 Home-page: https://github.com/esbozos/django-nets-core
 Author: Norman Torres
 Author-email: norman.nets@gmail.com
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -61,18 +61,36 @@
     - For firebase to work, you need to set up a firebase project and download the credentials file and set it in settings.py as FIREBASE_CONFIG = os.path.join(BASE_DIR, 'firebase-credentials.json') see https://firebase.google.com/docs/admin/setup
     - For django-oauth-toolkit to work, you need to set up the authentication backend in settings.py as AUTHENTICATION_BACKENDS = ['oauth2_provider.backends.OAuth2Backend'] see https://django-oauth-toolkit.readthedocs.io/en/latest/rest-framework/getting_started.html#step-1-configure-your-authentication-backends
     - For django-cors-headers to work, you need to set up the middleware in settings.py as MIDDLEWARE = ['corsheaders.middleware.CorsMiddleware', 'django.middleware.common.CommonMiddleware'] see
     
 
 COMMANDS:
 _________
+
+check if settings are set correctly
+.. code-block:: bash
     
-    -./manage.py nets-settings --create # create settings required for nets_core
-    -./manage.py nets-settings  # will check if settings are set correctly
-    -./manage.py nets-settings --create --force # force create settings required for nets_core and overwrite existing settings if any
+    ./manage.py nets-settings
+
+create settings required for nets_core
+.. code-block:: bash
+    
+    ./manage.py nets-settings --create 
+
+force create settings required for nets_core and overwrite existing settings if any
+.. code-block:: bash
+
+    ./manage.py nets-settings --create --force 
+
+create superuser
+.. code-block:: bash
+
+    ./manage.py createsuperuser
+
+
 
 
 INSTALLATION
 ____________
 
 .. code-block:: bash
```

### Comparing `django-nets-core-0.1.69/django_nets_core.egg-info/SOURCES.txt` & `django-nets-core-0.1.70/django_nets_core.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -28,14 +28,18 @@
 nets_core/settings.py
 nets_core/settings_nets.py
 nets_core/tasks.py
 nets_core/urls.py
 nets_core/utils.py
 nets_core/views.py
 nets_core/wsgi.py
+nets_core/management/commands/__init__.py
+nets_core/management/commands/nets-settings.py
+nets_core/management/commands/__pycache__/__init__.cpython-312.pyc
+nets_core/management/commands/__pycache__/nets-settings.cpython-312.pyc
 nets_core/middleware/auth_token.py
 nets_core/middleware/__pycache__/auth_token.cpython-312.pyc
 nets_core/migrations/0001_initial.py
 nets_core/migrations/0002_alter_verificationcode_token.py
 nets_core/migrations/0003_userdevice.py
 nets_core/migrations/0004_remove_userdevice_device_id_userdevice_uuid.py
 nets_core/migrations/0005_userdevice_uuid.py
```

### Comparing `django-nets-core-0.1.69/nets_core/asgi.py` & `django-nets-core-0.1.70/nets_core/asgi.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.69/nets_core/auth_urls.py` & `django-nets-core-0.1.70/nets_core/auth_urls.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.69/nets_core/decorators.py` & `django-nets-core-0.1.70/nets_core/decorators.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.69/nets_core/firebase_messages.py` & `django-nets-core-0.1.70/nets_core/firebase_messages.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.69/nets_core/handlers.py` & `django-nets-core-0.1.70/nets_core/handlers.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.69/nets_core/listeners.py` & `django-nets-core-0.1.70/nets_core/listeners.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.69/nets_core/mail.py` & `django-nets-core-0.1.70/nets_core/mail.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.69/nets_core/manage.py` & `django-nets-core-0.1.70/nets_core/manage.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.69/nets_core/middleware/__pycache__/auth_token.cpython-312.pyc` & `django-nets-core-0.1.70/nets_core/middleware/__pycache__/auth_token.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.69/nets_core/middleware/auth_token.py` & `django-nets-core-0.1.70/nets_core/middleware/auth_token.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.69/nets_core/migrations/0001_initial.py` & `django-nets-core-0.1.70/nets_core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.69/nets_core/migrations/0003_userdevice.py` & `django-nets-core-0.1.70/nets_core/migrations/0003_userdevice.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.69/nets_core/migrations/0007_alter_verificationcode_device.py` & `django-nets-core-0.1.70/nets_core/migrations/0007_alter_verificationcode_device.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.69/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py` & `django-nets-core-0.1.70/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.69/nets_core/models.py` & `django-nets-core-0.1.70/nets_core/models.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.69/nets_core/params.py` & `django-nets-core-0.1.70/nets_core/params.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.69/nets_core/responses.py` & `django-nets-core-0.1.70/nets_core/responses.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.69/nets_core/security.py` & `django-nets-core-0.1.70/nets_core/security.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.69/nets_core/settings.py` & `django-nets-core-0.1.70/nets_core/settings.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.69/nets_core/settings_nets.py` & `django-nets-core-0.1.70/nets_core/settings_nets.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.69/nets_core/tasks.py` & `django-nets-core-0.1.70/nets_core/tasks.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,7 +10,11 @@
 def send_user_devices_notifications(user_id:  int, title: str, message: str, data: dict, channel: str=None):
     from nets_core.firebase_messages import send_user_device_notification
     user = User.objects.get(id=user_id)    
     # ensure data is a dict of strings
     data = {k: str(v) for k, v in data.items()}
     send_user_device_notification(user, title, message, data, channel)
 
+@shared_task
+def check_permissions(user_id: int, permission: str):
+    user = User.objects.get(id=user_id)
+    return user.has_perm(permission)
```

### Comparing `django-nets-core-0.1.69/nets_core/templates/nets_core/base.html` & `django-nets-core-0.1.70/nets_core/templates/nets_core/base.html`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.69/nets_core/templates/nets_core/delete_account.html` & `django-nets-core-0.1.70/nets_core/templates/nets_core/delete_account.html`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.69/nets_core/templates/nets_core/email/base_email.html` & `django-nets-core-0.1.70/nets_core/templates/nets_core/email/base_email.html`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.69/nets_core/templates/nets_core/email/new_login.html` & `django-nets-core-0.1.70/nets_core/templates/nets_core/email/new_login.html`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.69/nets_core/urls.py` & `django-nets-core-0.1.70/nets_core/urls.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.69/nets_core/utils.py` & `django-nets-core-0.1.70/nets_core/utils.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.69/nets_core/views.py` & `django-nets-core-0.1.70/nets_core/views.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.69/setup.cfg` & `django-nets-core-0.1.70/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-nets-core
-version = 0.1.69
+version = 0.1.70
 description = A lazy API rest request handler.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/esbozos/django-nets-core
 author = Norman Torres
 author_email = norman.nets@gmail.com
 license = BSD-3-Clause
```

