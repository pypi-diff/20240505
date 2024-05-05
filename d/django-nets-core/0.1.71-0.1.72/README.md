# Comparing `tmp/django_nets_core-0.1.71.tar.gz` & `tmp/django_nets_core-0.1.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_nets_core-0.1.71.tar", last modified: Sun May  5 15:47:18 2024, max compression
+gzip compressed data, was "django_nets_core-0.1.72.tar", last modified: Sun May  5 18:59:45 2024, max compression
```

## Comparing `django_nets_core-0.1.71.tar` & `django_nets_core-0.1.72.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:47:18.403283 django_nets_core-0.1.71/
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/LICENSE
--rw-rw-r--   0 dev       (1001) dev       (1001)      304 2024-05-05 15:47:07.000000 django_nets_core-0.1.71/MANIFEST.in
--rw-r--r--   0 dev       (1001) dev       (1001)     9178 2024-05-05 15:47:18.403283 django_nets_core-0.1.71/PKG-INFO
--rw-rw-r--   0 dev       (1001) dev       (1001)     7653 2024-05-05 05:21:24.000000 django_nets_core-0.1.71/README.rst
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:47:18.403283 django_nets_core-0.1.71/django_nets_core.egg-info/
--rw-r--r--   0 dev       (1001) dev       (1001)     9178 2024-05-05 15:47:18.000000 django_nets_core-0.1.71/django_nets_core.egg-info/PKG-INFO
--rw-rw-r--   0 dev       (1001) dev       (1001)     1836 2024-05-05 15:47:18.000000 django_nets_core-0.1.71/django_nets_core.egg-info/SOURCES.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)        1 2024-05-05 15:47:18.000000 django_nets_core-0.1.71/django_nets_core.egg-info/dependency_links.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)      286 2024-05-05 15:47:18.000000 django_nets_core-0.1.71/django_nets_core.egg-info/requires.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)       10 2024-05-05 15:47:18.000000 django_nets_core-0.1.71/django_nets_core.egg-info/top_level.txt
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:47:18.399283 django_nets_core-0.1.71/nets_core/
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/__init__.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      206 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/apps.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      807 2024-05-05 05:05:51.000000 django_nets_core-0.1.71/nets_core/asgi.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      537 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/auth_urls.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      229 2024-05-05 05:05:51.000000 django_nets_core-0.1.71/nets_core/celery.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3270 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/decorators.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3276 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/firebase_messages.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     6465 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/handlers.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     2477 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/listeners.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     4402 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/mail.py
--rwxrwxr-x   0 dev       (1001) dev       (1001)      665 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/manage.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:47:18.395283 django_nets_core-0.1.71/nets_core/management/
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:47:18.399283 django_nets_core-0.1.71/nets_core/management/commands/
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-05 02:03:24.000000 django_nets_core-0.1.71/nets_core/management/commands/__init__.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:47:18.399283 django_nets_core-0.1.71/nets_core/management/commands/__pycache__/
--rw-rw-r--   0 dev       (1001) dev       (1001)      165 2024-05-05 02:44:07.000000 django_nets_core-0.1.71/nets_core/management/commands/__pycache__/__init__.cpython-312.pyc
--rw-rw-r--   0 dev       (1001) dev       (1001)    28055 2024-05-05 05:05:51.000000 django_nets_core-0.1.71/nets_core/management/commands/__pycache__/nets-settings.cpython-312.pyc
--rw-rw-r--   0 dev       (1001) dev       (1001)    23169 2024-05-05 05:05:47.000000 django_nets_core-0.1.71/nets_core/management/commands/nets-settings.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:47:18.399283 django_nets_core-0.1.71/nets_core/middleware/
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:47:18.399283 django_nets_core-0.1.71/nets_core/middleware/__pycache__/
--rw-rw-r--   0 dev       (1001) dev       (1001)     3004 2024-05-05 04:39:30.000000 django_nets_core-0.1.71/nets_core/middleware/__pycache__/auth_token.cpython-312.pyc
--rw-rw-r--   0 dev       (1001) dev       (1001)     2003 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/middleware/auth_token.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:47:18.403283 django_nets_core-0.1.71/nets_core/migrations/
--rw-rw-r--   0 dev       (1001) dev       (1001)     5274 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/migrations/0001_initial.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      422 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/migrations/0002_alter_verificationcode_token.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     2208 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/migrations/0003_userdevice.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      360 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/migrations/0004_remove_userdevice_device_id_userdevice_uuid.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      480 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/migrations/0005_userdevice_uuid.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      454 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/migrations/0006_verificationcode_device.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      533 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/migrations/0007_alter_verificationcode_device.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     2056 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      455 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/migrations/0009_userdevice_ip.py
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/migrations/__init__.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     8055 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/models.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     6425 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/params.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      902 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/responses.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3055 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/security.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3471 2024-05-05 05:01:32.000000 django_nets_core-0.1.71/nets_core/settings.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     1820 2024-05-05 05:05:51.000000 django_nets_core-0.1.71/nets_core/settings_nets.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      753 2024-05-05 05:16:02.000000 django_nets_core-0.1.71/nets_core/tasks.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:47:18.395283 django_nets_core-0.1.71/nets_core/templates/
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:47:18.403283 django_nets_core-0.1.71/nets_core/templates/nets_core/
--rw-rw-r--   0 dev       (1001) dev       (1001)     6978 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/templates/nets_core/base.html
--rw-rw-r--   0 dev       (1001) dev       (1001)     1954 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/templates/nets_core/delete_account.html
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 15:47:18.403283 django_nets_core-0.1.71/nets_core/templates/nets_core/email/
--rw-rw-r--   0 dev       (1001) dev       (1001)    16103 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/templates/nets_core/email/base_email.html
--rw-rw-r--   0 dev       (1001) dev       (1001)     1032 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/templates/nets_core/email/new_login.html
--rw-rw-r--   0 dev       (1001) dev       (1001)      316 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/templates/nets_core/email/verification_code.html
--rw-rw-r--   0 dev       (1001) dev       (1001)      824 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/urls.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     1709 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/utils.py
--rw-rw-r--   0 dev       (1001) dev       (1001)    11692 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/views.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      395 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/nets_core/wsgi.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      100 2024-05-05 00:47:40.000000 django_nets_core-0.1.71/pyproject.toml
--rw-rw-r--   0 dev       (1001) dev       (1001)      181 2024-05-05 01:49:02.000000 django_nets_core-0.1.71/requirements.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)     1334 2024-05-05 15:47:18.403283 django_nets_core-0.1.71/setup.cfg
--rw-rw-r--   0 dev       (1001) dev       (1001)       38 2024-05-04 23:43:26.000000 django_nets_core-0.1.71/setup.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 18:59:45.402663 django_nets_core-0.1.72/
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.72/LICENSE
+-rw-rw-r--   0 dev       (1001) dev       (1001)      304 2024-05-05 15:47:07.000000 django_nets_core-0.1.72/MANIFEST.in
+-rw-r--r--   0 dev       (1001) dev       (1001)    13678 2024-05-05 18:59:45.402663 django_nets_core-0.1.72/PKG-INFO
+-rw-rw-r--   0 dev       (1001) dev       (1001)    12153 2024-05-05 18:59:42.000000 django_nets_core-0.1.72/README.rst
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 18:59:45.402663 django_nets_core-0.1.72/django_nets_core.egg-info/
+-rw-r--r--   0 dev       (1001) dev       (1001)    13678 2024-05-05 18:59:45.000000 django_nets_core-0.1.72/django_nets_core.egg-info/PKG-INFO
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1891 2024-05-05 18:59:45.000000 django_nets_core-0.1.72/django_nets_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)        1 2024-05-05 18:59:45.000000 django_nets_core-0.1.72/django_nets_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)      286 2024-05-05 18:59:45.000000 django_nets_core-0.1.72/django_nets_core.egg-info/requires.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)       10 2024-05-05 18:59:45.000000 django_nets_core-0.1.72/django_nets_core.egg-info/top_level.txt
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 18:59:45.402663 django_nets_core-0.1.72/nets_core/
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.72/nets_core/__init__.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      206 2024-05-04 23:43:26.000000 django_nets_core-0.1.72/nets_core/apps.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      807 2024-05-05 05:05:51.000000 django_nets_core-0.1.72/nets_core/asgi.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      537 2024-05-04 23:43:26.000000 django_nets_core-0.1.72/nets_core/auth_urls.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      229 2024-05-05 05:05:51.000000 django_nets_core-0.1.72/nets_core/celery.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     4901 2024-05-05 18:50:21.000000 django_nets_core-0.1.72/nets_core/decorators.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3276 2024-05-04 23:43:26.000000 django_nets_core-0.1.72/nets_core/firebase_messages.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     6465 2024-05-04 23:43:26.000000 django_nets_core-0.1.72/nets_core/handlers.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2477 2024-05-04 23:43:26.000000 django_nets_core-0.1.72/nets_core/listeners.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     4460 2024-05-05 18:01:33.000000 django_nets_core-0.1.72/nets_core/mail.py
+-rwxrwxr-x   0 dev       (1001) dev       (1001)      665 2024-05-04 23:43:26.000000 django_nets_core-0.1.72/nets_core/manage.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 18:59:45.398663 django_nets_core-0.1.72/nets_core/management/
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 18:59:45.402663 django_nets_core-0.1.72/nets_core/management/commands/
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-05 02:03:24.000000 django_nets_core-0.1.72/nets_core/management/commands/__init__.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 18:59:45.402663 django_nets_core-0.1.72/nets_core/management/commands/__pycache__/
+-rw-rw-r--   0 dev       (1001) dev       (1001)      165 2024-05-05 02:44:07.000000 django_nets_core-0.1.72/nets_core/management/commands/__pycache__/__init__.cpython-312.pyc
+-rw-rw-r--   0 dev       (1001) dev       (1001)    28055 2024-05-05 05:05:51.000000 django_nets_core-0.1.72/nets_core/management/commands/__pycache__/nets-settings.cpython-312.pyc
+-rw-rw-r--   0 dev       (1001) dev       (1001)    22911 2024-05-05 16:06:29.000000 django_nets_core-0.1.72/nets_core/management/commands/nets-settings.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 18:59:45.402663 django_nets_core-0.1.72/nets_core/middleware/
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 18:59:45.402663 django_nets_core-0.1.72/nets_core/middleware/__pycache__/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3004 2024-05-05 04:39:30.000000 django_nets_core-0.1.72/nets_core/middleware/__pycache__/auth_token.cpython-312.pyc
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2003 2024-05-04 23:43:26.000000 django_nets_core-0.1.72/nets_core/middleware/auth_token.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 18:59:45.402663 django_nets_core-0.1.72/nets_core/migrations/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     5274 2024-05-04 23:43:26.000000 django_nets_core-0.1.72/nets_core/migrations/0001_initial.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      422 2024-05-04 23:43:26.000000 django_nets_core-0.1.72/nets_core/migrations/0002_alter_verificationcode_token.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2208 2024-05-04 23:43:26.000000 django_nets_core-0.1.72/nets_core/migrations/0003_userdevice.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      360 2024-05-04 23:43:26.000000 django_nets_core-0.1.72/nets_core/migrations/0004_remove_userdevice_device_id_userdevice_uuid.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      480 2024-05-04 23:43:26.000000 django_nets_core-0.1.72/nets_core/migrations/0005_userdevice_uuid.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      454 2024-05-04 23:43:26.000000 django_nets_core-0.1.72/nets_core/migrations/0006_verificationcode_device.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      533 2024-05-04 23:43:26.000000 django_nets_core-0.1.72/nets_core/migrations/0007_alter_verificationcode_device.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2056 2024-05-04 23:43:26.000000 django_nets_core-0.1.72/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      455 2024-05-04 23:43:26.000000 django_nets_core-0.1.72/nets_core/migrations/0009_userdevice_ip.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.72/nets_core/migrations/__init__.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)    13274 2024-05-05 18:21:54.000000 django_nets_core-0.1.72/nets_core/models.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     6425 2024-05-04 23:43:26.000000 django_nets_core-0.1.72/nets_core/params.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      902 2024-05-04 23:43:26.000000 django_nets_core-0.1.72/nets_core/responses.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3055 2024-05-04 23:43:26.000000 django_nets_core-0.1.72/nets_core/security.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3387 2024-05-05 18:22:43.000000 django_nets_core-0.1.72/nets_core/settings.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1820 2024-05-05 05:05:51.000000 django_nets_core-0.1.72/nets_core/settings_nets.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      753 2024-05-05 05:16:02.000000 django_nets_core-0.1.72/nets_core/tasks.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 18:59:45.398663 django_nets_core-0.1.72/nets_core/templates/
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 18:59:45.402663 django_nets_core-0.1.72/nets_core/templates/nets_core/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     6978 2024-05-04 23:43:26.000000 django_nets_core-0.1.72/nets_core/templates/nets_core/base.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1954 2024-05-04 23:43:26.000000 django_nets_core-0.1.72/nets_core/templates/nets_core/delete_account.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-05 18:03:29.000000 django_nets_core-0.1.72/nets_core/templates/nets_core/delete_account_info.html
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 18:59:45.402663 django_nets_core-0.1.72/nets_core/templates/nets_core/email/
+-rw-rw-r--   0 dev       (1001) dev       (1001)    16103 2024-05-04 23:43:26.000000 django_nets_core-0.1.72/nets_core/templates/nets_core/email/base_email.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1032 2024-05-04 23:43:26.000000 django_nets_core-0.1.72/nets_core/templates/nets_core/email/new_login.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)      316 2024-05-04 23:43:26.000000 django_nets_core-0.1.72/nets_core/templates/nets_core/email/verification_code.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)      824 2024-05-04 23:43:26.000000 django_nets_core-0.1.72/nets_core/urls.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3003 2024-05-05 18:49:07.000000 django_nets_core-0.1.72/nets_core/utils.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)    11727 2024-05-05 18:04:42.000000 django_nets_core-0.1.72/nets_core/views.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      395 2024-05-04 23:43:26.000000 django_nets_core-0.1.72/nets_core/wsgi.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      100 2024-05-05 00:47:40.000000 django_nets_core-0.1.72/pyproject.toml
+-rw-rw-r--   0 dev       (1001) dev       (1001)      181 2024-05-05 01:49:02.000000 django_nets_core-0.1.72/requirements.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1334 2024-05-05 18:59:45.402663 django_nets_core-0.1.72/setup.cfg
+-rw-rw-r--   0 dev       (1001) dev       (1001)       38 2024-05-04 23:43:26.000000 django_nets_core-0.1.72/setup.py
```

### Comparing `django_nets_core-0.1.71/django_nets_core.egg-info/SOURCES.txt` & `django_nets_core-0.1.72/django_nets_core.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -46,10 +46,11 @@
 nets_core/migrations/0006_verificationcode_device.py
 nets_core/migrations/0007_alter_verificationcode_device.py
 nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py
 nets_core/migrations/0009_userdevice_ip.py
 nets_core/migrations/__init__.py
 nets_core/templates/nets_core/base.html
 nets_core/templates/nets_core/delete_account.html
+nets_core/templates/nets_core/delete_account_info.html
 nets_core/templates/nets_core/email/base_email.html
 nets_core/templates/nets_core/email/new_login.html
 nets_core/templates/nets_core/email/verification_code.html
```

### Comparing `django_nets_core-0.1.71/nets_core/asgi.py` & `django_nets_core-0.1.72/nets_core/asgi.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.71/nets_core/auth_urls.py` & `django_nets_core-0.1.72/nets_core/auth_urls.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.71/nets_core/firebase_messages.py` & `django_nets_core-0.1.72/nets_core/firebase_messages.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.71/nets_core/handlers.py` & `django_nets_core-0.1.72/nets_core/handlers.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.71/nets_core/listeners.py` & `django_nets_core-0.1.72/nets_core/listeners.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.71/nets_core/mail.py` & `django_nets_core-0.1.72/nets_core/mail.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,46 +8,46 @@
 from nets_core.models import EmailNotification
 
 from django.utils.module_loading import import_string
 from django.core.mail.backends.smtp import EmailBackend
 
 exclude_domains = []
 try:
-    exclude_domains = settings.NS_EMAIL_EXCLUDE_DOMAINS
+    exclude_domains = settings.NETS_CORE_EMAIL_EXCLUDE_DOMAINS
 except:
     pass
 
 footer_enabled = True
 try:
-    footer_enabled = settings.NS_EMAIL_FOOTER_ENABLED
+    footer_enabled = settings.NETS_CORE_EMAIL_FOOTER_ENABLED
 except:
     pass
 
 footer = "<span><i class=\"small\">{}</i></span>".format(
-        _("NETS CORE footer email, you can customize this message in settings.NS_EMAIL_FOOTER"))
+        _("NETS CORE footer email, you can customize this message in settings.NETS_CORE_EMAIL_FOOTER"))
 try:
-    footer = f"<span><i class=\"small\">{settings.NS_EMAIL_FOOTER}</i></span>"
+    footer = f"<span><i class=\"small\">{settings.NETS_CORE_EMAIL_FOOTER}</i></span>"
 except:
     pass
 
 footer_template = None
 try:
-    footer_template = settings.NS_EMAIL_FOOTER_TEMPLATE
+    footer_template = settings.NETS_CORE_EMAIL_FOOTER_TEMPLATE
 except:
     pass
 
 try:
     SmsService = import_string(settings.NOTIFY['SMS_SERVICE'])
     sms = SmsService()
 except:
     sms = None
 
 mail_debug_enabled = False
 try:
-    mail_debug_enabled = settings.NS_EMAIL_DEBUG_ENABLED
+    mail_debug_enabled = settings.NETS_CORE_EMAIL_DEBUG_ENABLED
 except:
     pass
 
 
 def send_email(subject: str, email: str|list[str], template: str, context: dict, 
     txt_template: str = None, to_queued: bool = True, force=False, html: str =None):
     """
@@ -58,22 +58,22 @@
     if settings.DEBUG and not mail_debug_enabled and not force:
         return (False, _("emails are disabled while debug is true in settings"))
 
     # Exclude emails from exclude_domain
     if(isinstance(email, str)):
         email_domain = email.split('@')
         if email_domain in exclude_domains:
-            return (False, f'{_("Email domain is in NS_MAIL_EXCLUDE_DOMAINS ")} {email_domain}')
+            return (False, f'{_("Email domain is in NETS_CORE_EMAIL_EXCLUDE_DOMAINS ")} {email_domain}')
 
     elif isinstance(email, list):
         for e in email:
             email_domain = e.split('@')
             if email_domain in exclude_domains:
                 email.pop(email.index(e))
-                print(f"{_('Email domain is in NS_MAIL_EXCLUDE_DOMAINS')} {email_domain}")
+                print(f"{_('Email domain is in NETS_CORE_EMAIL_EXCLUDE_DOMAINS')} {email_domain}")
     
     if not email:
         return (False, _("email is empty"))
     
     full_context = context
     # full_context.update(context)
     content_txt = None
```

### Comparing `django_nets_core-0.1.71/nets_core/manage.py` & `django_nets_core-0.1.72/nets_core/manage.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.71/nets_core/management/commands/__pycache__/nets-settings.cpython-312.pyc` & `django_nets_core-0.1.72/nets_core/management/commands/__pycache__/nets-settings.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.71/nets_core/management/commands/nets-settings.py` & `django_nets_core-0.1.72/nets_core/management/commands/nets-settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,19 +127,15 @@
         except Exception as e:
             self.stdout.write(self.style.ERROR('INSTALLED_APPS not found in settings.py file.'))
             pass
         
         
         # check for ROOT_URLCONF
                        
-        try:
-            root_urlconf = settings.ROOT_URLCONF
-            if 'nets_core.auth_urls' not in root_urlconf:
-                self.stdout.write(self.style.ERROR('nets_core.auth_urls not found in ROOT_URLCONF in settings.py file.'))
-        except Exception as e:
+        if not hasattr(settings, 'ROOT_URLCONF'):
             self.stdout.write(self.style.ERROR('ROOT_URLCONF not found in settings.py file.'))
             pass
         # check for MIDDLEWARE
         
         try:
             middleware = settings.MIDDLEWARE
             if 'corsheaders.middleware.CorsMiddleware' not in middleware:
@@ -228,17 +224,17 @@
             settings.INSTALLED_APPS.append('corsheaders')
             
         if 'nets_core' not in settings.INSTALLED_APPS:
             self.stdout.write(self.style.NOTICE('Adding nets_core to INSTALLED_APPS in settings.py file.'))
             settings.INSTALLED_APPS.append('nets_core')
             
         # check for ROOT_URLCONF
-        if 'nets_core.auth_urls' not in settings.ROOT_URLCONF:
-            self.stdout.write(self.style.NOTICE('Adding nets_core.auth_urls to ROOT_URLCONF in settings.py file.'))
-            settings.ROOT_URLCONF = 'nets_core.auth_urls'
+        if not hasattr(settings, 'ROOT_URLCONF'):
+            self.stdout.write(self.style.NOTICE('Adding ROOT_URLCONF to settings.py file.'))
+            settings.ROOT_URLCONF = f'{project_name}.urls'
             
         # check for MIDDLEWARE
         if 'corsheaders.middleware.CorsMiddleware' not in settings.MIDDLEWARE:
             self.stdout.write(self.style.NOTICE('Adding corsheaders.middleware.CorsMiddleware to MIDDLEWARE in settings.py file.'))
             settings.MIDDLEWARE.append('corsheaders.middleware.CorsMiddleware')
             
         if 'oauth2_provider.middleware.OAuth2TokenMiddleware' not in settings.MIDDLEWARE:
```

### Comparing `django_nets_core-0.1.71/nets_core/middleware/__pycache__/auth_token.cpython-312.pyc` & `django_nets_core-0.1.72/nets_core/middleware/__pycache__/auth_token.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.71/nets_core/middleware/auth_token.py` & `django_nets_core-0.1.72/nets_core/middleware/auth_token.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.71/nets_core/migrations/0001_initial.py` & `django_nets_core-0.1.72/nets_core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.71/nets_core/migrations/0003_userdevice.py` & `django_nets_core-0.1.72/nets_core/migrations/0003_userdevice.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.71/nets_core/migrations/0007_alter_verificationcode_device.py` & `django_nets_core-0.1.72/nets_core/migrations/0007_alter_verificationcode_device.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.71/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py` & `django_nets_core-0.1.72/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.71/nets_core/params.py` & `django_nets_core-0.1.72/nets_core/params.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.71/nets_core/responses.py` & `django_nets_core-0.1.72/nets_core/responses.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.71/nets_core/security.py` & `django_nets_core-0.1.72/nets_core/security.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.71/nets_core/settings.py` & `django_nets_core-0.1.72/nets_core/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -123,12 +123,11 @@
 # https://docs.djangoproject.com/en/4.1/ref/settings/#default-auto-field
 
 DEFAULT_AUTO_FIELD = 'django.db.models.BigAutoField'
 
 
 try:
     from .settings_nets import *
-    print(f"Installe apps: {INSTALLED_APPS}")
-    print(f"ASGI: {ASGI_APPLICATION}")
+
 except ImportError:
     print('No settings_nets.py file found')
     pass
```

### Comparing `django_nets_core-0.1.71/nets_core/settings_nets.py` & `django_nets_core-0.1.72/nets_core/settings_nets.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.71/nets_core/tasks.py` & `django_nets_core-0.1.72/nets_core/tasks.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.71/nets_core/templates/nets_core/base.html` & `django_nets_core-0.1.72/nets_core/templates/nets_core/base.html`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.71/nets_core/templates/nets_core/delete_account.html` & `django_nets_core-0.1.72/nets_core/templates/nets_core/delete_account.html`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.71/nets_core/templates/nets_core/email/base_email.html` & `django_nets_core-0.1.72/nets_core/templates/nets_core/email/base_email.html`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.71/nets_core/templates/nets_core/email/new_login.html` & `django_nets_core-0.1.72/nets_core/templates/nets_core/email/new_login.html`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.71/nets_core/urls.py` & `django_nets_core-0.1.72/nets_core/urls.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.71/nets_core/views.py` & `django_nets_core-0.1.72/nets_core/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -142,17 +142,18 @@
                     device = UserDevice.objects.create(**device_data)
 
         # create verification code, listeners will send email/sms and devices notifications
         # with firebase
         VerificationCode.objects.create(user=new_user, ip=request.ip, device=device)
 
         return success_response(
-            _("CODE SENT"), extra={
-                "device_uuid": device.uuid if device else None,    
-            }
+            _("CODE SENT"),
+            extra={
+                "device_uuid": device.uuid if device else None,
+            },
         )
 
     except IntegrityError as e:
         print(e)
         return error_response(_("Username not available"), 400)
 
     except Exception as e:
@@ -209,15 +210,15 @@
         msg = e.__str__()
         return error_response(msg)
 
 
 @request_handler()
 def auth_logout(request):
     params = request.params
-    if hasattr(params, 'device_uuid'):
+    if hasattr(params, "device_uuid"):
         try:
             device = UserDevice.objects.get(uuid=params.device_uuid, user=request.user)
             device.delete()
         except UserDevice.DoesNotExist:
             pass
     # get Bearer token
     try:
@@ -310,48 +311,53 @@
         return error_response(e.__str__())
 
     return success_response(user.to_json())
 
 
 @request_handler(public=True)
 def request_delete_user_account(request):
-    if not hasattr(settings, "NETS_CORE_DELETE_ACCOUNT_EMAIL_TEMPLATE"):
-        raise ImproperlyConfigured(
-            "NETS_CORE_DELETE_ACCOUNT_EMAIL_TEMPLATE not found in settings"
-        )
-    
-    return render(request, "nets_core/delete_account.html", {
-        "title": _("Delete Account"),
-        "info_template": settings.NETS_CORE_DELETE_ACCOUNT_EMAIL_TEMPLATE,
-        "user": request.user
-        })
+    if not hasattr(settings, "NETS_CORE_DELETE_ACCOUNT_TEMPLATE"):
+        info_template = "nets_core/delete_account_info.html"
+    else:
+        info_template = settings.NETS_CORE_DELETE_ACCOUNT_TEMPLATE
+
+    return render(
+        request,
+        "nets_core/delete_account.html",
+        {
+            "title": _("Delete Account"),
+            "info_template": info_template,
+            "user": request.user,
+        },
+    )
 
 
 @request_handler(
     params=[RequestParam("sure", bool, default=False), RequestParam("code", str)],
 )
 def delete_user_account(request):
     if not request.params.sure:
         return error_response(_("Are you sure?"), 400)
 
     if not request.params.code:
         return error_response(_("Invalid code"), 400)
 
     try:
-        code = VerificationCode.objects.get(
-            user=request.user, verified=False
-        ).order_by("-created").first()
-        
+        code = (
+            VerificationCode.objects.get(user=request.user, verified=False)
+            .order_by("-created")
+            .first()
+        )
 
         if code.validate(request.params.code):
             # delete user
             user = request.user
             user.delete()
             return success_response(_("Account deleted successfully"))
 
     except VerificationCode.DoesNotExist:
         return error_response(_("Invalid code"), 400)
-    
+
     except Exception as e:
         return error_response(e.__str__())
-    
+
     return error_response(_("Invalid code"), 400)
```

### Comparing `django_nets_core-0.1.71/setup.cfg` & `django_nets_core-0.1.72/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-nets-core
-version = 0.1.71
+version = 0.1.72
 description = A lazy API rest request handler.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/esbozos/django-nets-core
 author = Norman Torres
 author_email = norman.nets@gmail.com
 license = BSD-3-Clause
```

