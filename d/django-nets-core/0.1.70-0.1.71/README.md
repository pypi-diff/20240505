# Comparing `tmp/django-nets-core-0.1.70.tar.gz` & `tmp/django_nets_core-0.1.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-nets-core-0.1.70.tar", last modified: Sun May  5 15:45:41 2024, max compression
+gzip compressed data, was "django_nets_core-0.1.71.tar", last modified: Sun May  5 15:47:18 2024, max compression
```

## Comparing `django-nets-core-0.1.70.tar` & `django_nets_core-0.1.71.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:45:41.811035 django-nets-core-0.1.70/
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/LICENSE
--rw-rw-r--   0 dev       (1001) dev       (1001)      254 2024-05-05 15:45:38.000000 django-nets-core-0.1.70/MANIFEST.in
--rw-rw-r--   0 dev       (1001) dev       (1001)     8702 2024-05-05 15:45:41.811035 django-nets-core-0.1.70/PKG-INFO
--rw-rw-r--   0 dev       (1001) dev       (1001)     7653 2024-05-05 05:21:24.000000 django-nets-core-0.1.70/README.rst
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:45:41.807036 django-nets-core-0.1.70/django_nets_core.egg-info/
--rw-r--r--   0 dev       (1001) dev       (1001)     8702 2024-05-05 15:45:41.000000 django-nets-core-0.1.70/django_nets_core.egg-info/PKG-INFO
--rw-rw-r--   0 dev       (1001) dev       (1001)     1836 2024-05-05 15:45:41.000000 django-nets-core-0.1.70/django_nets_core.egg-info/SOURCES.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)        1 2024-05-05 15:45:41.000000 django-nets-core-0.1.70/django_nets_core.egg-info/dependency_links.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)      286 2024-05-05 15:45:41.000000 django-nets-core-0.1.70/django_nets_core.egg-info/requires.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)       10 2024-05-05 15:45:41.000000 django-nets-core-0.1.70/django_nets_core.egg-info/top_level.txt
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:45:41.807036 django-nets-core-0.1.70/nets_core/
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/__init__.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      206 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/apps.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      807 2024-05-05 05:05:51.000000 django-nets-core-0.1.70/nets_core/asgi.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      537 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/auth_urls.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      229 2024-05-05 05:05:51.000000 django-nets-core-0.1.70/nets_core/celery.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3270 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/decorators.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3276 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/firebase_messages.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     6465 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/handlers.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     2477 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/listeners.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     4402 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/mail.py
--rwxrwxr-x   0 dev       (1001) dev       (1001)      665 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/manage.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:45:41.803036 django-nets-core-0.1.70/nets_core/management/
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:45:41.807036 django-nets-core-0.1.70/nets_core/management/commands/
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-05 02:03:24.000000 django-nets-core-0.1.70/nets_core/management/commands/__init__.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:45:41.807036 django-nets-core-0.1.70/nets_core/management/commands/__pycache__/
--rw-rw-r--   0 dev       (1001) dev       (1001)      165 2024-05-05 02:44:07.000000 django-nets-core-0.1.70/nets_core/management/commands/__pycache__/__init__.cpython-312.pyc
--rw-rw-r--   0 dev       (1001) dev       (1001)    28055 2024-05-05 05:05:51.000000 django-nets-core-0.1.70/nets_core/management/commands/__pycache__/nets-settings.cpython-312.pyc
--rw-rw-r--   0 dev       (1001) dev       (1001)    23169 2024-05-05 05:05:47.000000 django-nets-core-0.1.70/nets_core/management/commands/nets-settings.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:45:41.807036 django-nets-core-0.1.70/nets_core/middleware/
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:45:41.811035 django-nets-core-0.1.70/nets_core/middleware/__pycache__/
--rw-rw-r--   0 dev       (1001) dev       (1001)     3004 2024-05-05 04:39:30.000000 django-nets-core-0.1.70/nets_core/middleware/__pycache__/auth_token.cpython-312.pyc
--rw-rw-r--   0 dev       (1001) dev       (1001)     2003 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/middleware/auth_token.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:45:41.811035 django-nets-core-0.1.70/nets_core/migrations/
--rw-rw-r--   0 dev       (1001) dev       (1001)     5274 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/migrations/0001_initial.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      422 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/migrations/0002_alter_verificationcode_token.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     2208 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/migrations/0003_userdevice.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      360 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/migrations/0004_remove_userdevice_device_id_userdevice_uuid.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      480 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/migrations/0005_userdevice_uuid.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      454 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/migrations/0006_verificationcode_device.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      533 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/migrations/0007_alter_verificationcode_device.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     2056 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      455 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/migrations/0009_userdevice_ip.py
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/migrations/__init__.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     8055 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/models.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     6425 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/params.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      902 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/responses.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3055 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/security.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3471 2024-05-05 05:01:32.000000 django-nets-core-0.1.70/nets_core/settings.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     1820 2024-05-05 05:05:51.000000 django-nets-core-0.1.70/nets_core/settings_nets.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      753 2024-05-05 05:16:02.000000 django-nets-core-0.1.70/nets_core/tasks.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:45:41.803036 django-nets-core-0.1.70/nets_core/templates/
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:45:41.811035 django-nets-core-0.1.70/nets_core/templates/nets_core/
--rw-rw-r--   0 dev       (1001) dev       (1001)     6978 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/templates/nets_core/base.html
--rw-rw-r--   0 dev       (1001) dev       (1001)     1954 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/templates/nets_core/delete_account.html
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:45:41.811035 django-nets-core-0.1.70/nets_core/templates/nets_core/email/
--rw-rw-r--   0 dev       (1001) dev       (1001)    16103 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/templates/nets_core/email/base_email.html
--rw-rw-r--   0 dev       (1001) dev       (1001)     1032 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/templates/nets_core/email/new_login.html
--rw-rw-r--   0 dev       (1001) dev       (1001)      316 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/templates/nets_core/email/verification_code.html
--rw-rw-r--   0 dev       (1001) dev       (1001)      824 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/urls.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     1709 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/utils.py
--rw-rw-r--   0 dev       (1001) dev       (1001)    11692 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/views.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      395 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/nets_core/wsgi.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      100 2024-05-05 00:47:40.000000 django-nets-core-0.1.70/pyproject.toml
--rw-rw-r--   0 dev       (1001) dev       (1001)      181 2024-05-05 01:49:02.000000 django-nets-core-0.1.70/requirements.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)     1334 2024-05-05 15:45:41.811035 django-nets-core-0.1.70/setup.cfg
--rw-rw-r--   0 dev       (1001) dev       (1001)       38 2024-05-04 23:43:26.000000 django-nets-core-0.1.70/setup.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:47:18.403283 django_nets_core-0.1.71/
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/LICENSE
+-rw-rw-r--   0 dev       (1001) dev       (1001)      304 2024-05-05 15:47:07.000000 django_nets_core-0.1.71/MANIFEST.in
+-rw-r--r--   0 dev       (1001) dev       (1001)     9178 2024-05-05 15:47:18.403283 django_nets_core-0.1.71/PKG-INFO
+-rw-rw-r--   0 dev       (1001) dev       (1001)     7653 2024-05-05 05:21:24.000000 django_nets_core-0.1.71/README.rst
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:47:18.403283 django_nets_core-0.1.71/django_nets_core.egg-info/
+-rw-r--r--   0 dev       (1001) dev       (1001)     9178 2024-05-05 15:47:18.000000 django_nets_core-0.1.71/django_nets_core.egg-info/PKG-INFO
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1836 2024-05-05 15:47:18.000000 django_nets_core-0.1.71/django_nets_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)        1 2024-05-05 15:47:18.000000 django_nets_core-0.1.71/django_nets_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)      286 2024-05-05 15:47:18.000000 django_nets_core-0.1.71/django_nets_core.egg-info/requires.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)       10 2024-05-05 15:47:18.000000 django_nets_core-0.1.71/django_nets_core.egg-info/top_level.txt
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:47:18.399283 django_nets_core-0.1.71/nets_core/
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/__init__.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      206 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/apps.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      807 2024-05-05 05:05:51.000000 django_nets_core-0.1.71/nets_core/asgi.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      537 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/auth_urls.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      229 2024-05-05 05:05:51.000000 django_nets_core-0.1.71/nets_core/celery.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3270 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/decorators.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3276 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/firebase_messages.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     6465 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/handlers.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2477 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/listeners.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     4402 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/mail.py
+-rwxrwxr-x   0 dev       (1001) dev       (1001)      665 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/manage.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:47:18.395283 django_nets_core-0.1.71/nets_core/management/
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:47:18.399283 django_nets_core-0.1.71/nets_core/management/commands/
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-05 02:03:24.000000 django_nets_core-0.1.71/nets_core/management/commands/__init__.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:47:18.399283 django_nets_core-0.1.71/nets_core/management/commands/__pycache__/
+-rw-rw-r--   0 dev       (1001) dev       (1001)      165 2024-05-05 02:44:07.000000 django_nets_core-0.1.71/nets_core/management/commands/__pycache__/__init__.cpython-312.pyc
+-rw-rw-r--   0 dev       (1001) dev       (1001)    28055 2024-05-05 05:05:51.000000 django_nets_core-0.1.71/nets_core/management/commands/__pycache__/nets-settings.cpython-312.pyc
+-rw-rw-r--   0 dev       (1001) dev       (1001)    23169 2024-05-05 05:05:47.000000 django_nets_core-0.1.71/nets_core/management/commands/nets-settings.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:47:18.399283 django_nets_core-0.1.71/nets_core/middleware/
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:47:18.399283 django_nets_core-0.1.71/nets_core/middleware/__pycache__/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3004 2024-05-05 04:39:30.000000 django_nets_core-0.1.71/nets_core/middleware/__pycache__/auth_token.cpython-312.pyc
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2003 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/middleware/auth_token.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:47:18.403283 django_nets_core-0.1.71/nets_core/migrations/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     5274 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/migrations/0001_initial.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      422 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/migrations/0002_alter_verificationcode_token.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2208 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/migrations/0003_userdevice.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      360 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/migrations/0004_remove_userdevice_device_id_userdevice_uuid.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      480 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/migrations/0005_userdevice_uuid.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      454 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/migrations/0006_verificationcode_device.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      533 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/migrations/0007_alter_verificationcode_device.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2056 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      455 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/migrations/0009_userdevice_ip.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/migrations/__init__.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     8055 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/models.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     6425 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/params.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      902 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/responses.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3055 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/security.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3471 2024-05-05 05:01:32.000000 django_nets_core-0.1.71/nets_core/settings.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1820 2024-05-05 05:05:51.000000 django_nets_core-0.1.71/nets_core/settings_nets.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      753 2024-05-05 05:16:02.000000 django_nets_core-0.1.71/nets_core/tasks.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:47:18.395283 django_nets_core-0.1.71/nets_core/templates/
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:47:18.403283 django_nets_core-0.1.71/nets_core/templates/nets_core/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     6978 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/templates/nets_core/base.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1954 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/templates/nets_core/delete_account.html
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:47:18.403283 django_nets_core-0.1.71/nets_core/templates/nets_core/email/
+-rw-rw-r--   0 dev       (1001) dev       (1001)    16103 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/templates/nets_core/email/base_email.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1032 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/templates/nets_core/email/new_login.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)      316 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/templates/nets_core/email/verification_code.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)      824 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/urls.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1709 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/utils.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)    11692 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/views.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      395 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/wsgi.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      100 2024-05-05 00:47:40.000000 django_nets_core-0.1.71/pyproject.toml
+-rw-rw-r--   0 dev       (1001) dev       (1001)      181 2024-05-05 01:49:02.000000 django_nets_core-0.1.71/requirements.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1334 2024-05-05 15:47:18.403283 django_nets_core-0.1.71/setup.cfg
+-rw-rw-r--   0 dev       (1001) dev       (1001)       38 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/setup.py
```

### Comparing `django-nets-core-0.1.70/PKG-INFO` & `django_nets_core-0.1.71/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: django-nets-core
-Version: 0.1.70
+Version: 0.1.71
 Summary: A lazy API rest request handler.
 Home-page: https://github.com/esbozos/django-nets-core
 Author: Norman Torres
 Author-email: norman.nets@gmail.com
 License: BSD-3-Clause
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -21,14 +20,28 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: Django>=5.0.4
+Requires-Dist: pytz>=2024.1
+Requires-Dist: python-dateutil>=2.9.0.post0
+Requires-Dist: shortuuid>=1.0.13
+Requires-Dist: django-oauth-toolkit>=2.3.0
+Requires-Dist: firebase-admin>=6.5.0
+Requires-Dist: celery>=5.4.0
+Requires-Dist: django_celery_beat>=2.6.0
+Requires-Dist: django-cors-headers>=4.3.1
+Requires-Dist: pymemcache>=4.0.0
+Requires-Dist: python-memcached>=1.62
+Requires-Dist: django-memcached>=0.1.2
+Requires-Dist: channels>=4.1.0
+Requires-Dist: daphne>=4.1.2
 
 =========
 NETS CORE
 =========
 
 And set of lazy API request handlers and common tasks. 
 Just use it if you are really sure that you don't want to 
@@ -283,9 +296,7 @@
 Authentication
 ______________
 
     from nets_core.security import authenticate
     authenticate(user, code, client_id, client_secret)
 
 Just to be lazy.
-
-
```

### Comparing `django-nets-core-0.1.70/README.rst` & `django_nets_core-0.1.71/README.rst`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.70/django_nets_core.egg-info/PKG-INFO` & `django_nets_core-0.1.71/django_nets_core.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: django-nets-core
-Version: 0.1.70
+Version: 0.1.71
 Summary: A lazy API rest request handler.
 Home-page: https://github.com/esbozos/django-nets-core
 Author: Norman Torres
 Author-email: norman.nets@gmail.com
 License: BSD-3-Clause
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -21,14 +20,28 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: Django>=5.0.4
+Requires-Dist: pytz>=2024.1
+Requires-Dist: python-dateutil>=2.9.0.post0
+Requires-Dist: shortuuid>=1.0.13
+Requires-Dist: django-oauth-toolkit>=2.3.0
+Requires-Dist: firebase-admin>=6.5.0
+Requires-Dist: celery>=5.4.0
+Requires-Dist: django_celery_beat>=2.6.0
+Requires-Dist: django-cors-headers>=4.3.1
+Requires-Dist: pymemcache>=4.0.0
+Requires-Dist: python-memcached>=1.62
+Requires-Dist: django-memcached>=0.1.2
+Requires-Dist: channels>=4.1.0
+Requires-Dist: daphne>=4.1.2
 
 =========
 NETS CORE
 =========
 
 And set of lazy API request handlers and common tasks. 
 Just use it if you are really sure that you don't want to 
@@ -283,9 +296,7 @@
 Authentication
 ______________
 
     from nets_core.security import authenticate
     authenticate(user, code, client_id, client_secret)
 
 Just to be lazy.
-
-
```

### Comparing `django-nets-core-0.1.70/django_nets_core.egg-info/SOURCES.txt` & `django_nets_core-0.1.71/django_nets_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.70/nets_core/asgi.py` & `django_nets_core-0.1.71/nets_core/asgi.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.70/nets_core/auth_urls.py` & `django_nets_core-0.1.71/nets_core/auth_urls.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.70/nets_core/decorators.py` & `django_nets_core-0.1.71/nets_core/decorators.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.70/nets_core/firebase_messages.py` & `django_nets_core-0.1.71/nets_core/firebase_messages.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.70/nets_core/handlers.py` & `django_nets_core-0.1.71/nets_core/handlers.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.70/nets_core/listeners.py` & `django_nets_core-0.1.71/nets_core/listeners.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.70/nets_core/mail.py` & `django_nets_core-0.1.71/nets_core/mail.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.70/nets_core/manage.py` & `django_nets_core-0.1.71/nets_core/manage.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.70/nets_core/management/commands/__pycache__/nets-settings.cpython-312.pyc` & `django_nets_core-0.1.71/nets_core/management/commands/__pycache__/nets-settings.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.70/nets_core/management/commands/nets-settings.py` & `django_nets_core-0.1.71/nets_core/management/commands/nets-settings.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.70/nets_core/middleware/__pycache__/auth_token.cpython-312.pyc` & `django_nets_core-0.1.71/nets_core/middleware/__pycache__/auth_token.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.70/nets_core/middleware/auth_token.py` & `django_nets_core-0.1.71/nets_core/middleware/auth_token.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.70/nets_core/migrations/0001_initial.py` & `django_nets_core-0.1.71/nets_core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.70/nets_core/migrations/0003_userdevice.py` & `django_nets_core-0.1.71/nets_core/migrations/0003_userdevice.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.70/nets_core/migrations/0007_alter_verificationcode_device.py` & `django_nets_core-0.1.71/nets_core/migrations/0007_alter_verificationcode_device.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.70/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py` & `django_nets_core-0.1.71/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.70/nets_core/models.py` & `django_nets_core-0.1.71/nets_core/models.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.70/nets_core/params.py` & `django_nets_core-0.1.71/nets_core/params.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.70/nets_core/responses.py` & `django_nets_core-0.1.71/nets_core/responses.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.70/nets_core/security.py` & `django_nets_core-0.1.71/nets_core/security.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.70/nets_core/settings.py` & `django_nets_core-0.1.71/nets_core/settings.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.70/nets_core/settings_nets.py` & `django_nets_core-0.1.71/nets_core/settings_nets.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.70/nets_core/tasks.py` & `django_nets_core-0.1.71/nets_core/tasks.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.70/nets_core/templates/nets_core/base.html` & `django_nets_core-0.1.71/nets_core/templates/nets_core/base.html`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.70/nets_core/templates/nets_core/delete_account.html` & `django_nets_core-0.1.71/nets_core/templates/nets_core/delete_account.html`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.70/nets_core/templates/nets_core/email/base_email.html` & `django_nets_core-0.1.71/nets_core/templates/nets_core/email/base_email.html`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.70/nets_core/templates/nets_core/email/new_login.html` & `django_nets_core-0.1.71/nets_core/templates/nets_core/email/new_login.html`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.70/nets_core/urls.py` & `django_nets_core-0.1.71/nets_core/urls.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.70/nets_core/utils.py` & `django_nets_core-0.1.71/nets_core/utils.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.70/nets_core/views.py` & `django_nets_core-0.1.71/nets_core/views.py`

 * *Files identical despite different names*

### Comparing `django-nets-core-0.1.70/setup.cfg` & `django_nets_core-0.1.71/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-nets-core
-version = 0.1.70
+version = 0.1.71
 description = A lazy API rest request handler.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/esbozos/django-nets-core
 author = Norman Torres
 author_email = norman.nets@gmail.com
 license = BSD-3-Clause
```

