# Comparing `tmp/django_nets_core-0.1.76.tar.gz` & `tmp/django_nets_core-0.1.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_nets_core-0.1.76.tar", last modified: Sun May  5 19:36:11 2024, max compression
+gzip compressed data, was "django_nets_core-0.1.77.tar", last modified: Sun May  5 19:48:43 2024, max compression
```

## Comparing `django_nets_core-0.1.76.tar` & `django_nets_core-0.1.77.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 19:36:11.795626 django_nets_core-0.1.76/
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.76/LICENSE
--rw-rw-r--   0 dev       (1001) dev       (1001)      304 2024-05-05 15:47:07.000000 django_nets_core-0.1.76/MANIFEST.in
--rw-r--r--   0 dev       (1001) dev       (1001)    13678 2024-05-05 19:36:11.795626 django_nets_core-0.1.76/PKG-INFO
--rw-rw-r--   0 dev       (1001) dev       (1001)    12153 2024-05-05 18:59:42.000000 django_nets_core-0.1.76/README.rst
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 19:36:11.795626 django_nets_core-0.1.76/django_nets_core.egg-info/
--rw-r--r--   0 dev       (1001) dev       (1001)    13678 2024-05-05 19:36:11.000000 django_nets_core-0.1.76/django_nets_core.egg-info/PKG-INFO
--rw-rw-r--   0 dev       (1001) dev       (1001)     2015 2024-05-05 19:36:11.000000 django_nets_core-0.1.76/django_nets_core.egg-info/SOURCES.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)        1 2024-05-05 19:36:11.000000 django_nets_core-0.1.76/django_nets_core.egg-info/dependency_links.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)      286 2024-05-05 19:36:11.000000 django_nets_core-0.1.76/django_nets_core.egg-info/requires.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)       10 2024-05-05 19:36:11.000000 django_nets_core-0.1.76/django_nets_core.egg-info/top_level.txt
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 19:36:11.791625 django_nets_core-0.1.76/nets_core/
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.76/nets_core/__init__.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     2440 2024-05-05 19:35:20.000000 django_nets_core-0.1.76/nets_core/admin.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      206 2024-05-04 23:43:26.000000 django_nets_core-0.1.76/nets_core/apps.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      807 2024-05-05 05:05:51.000000 django_nets_core-0.1.76/nets_core/asgi.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      537 2024-05-04 23:43:26.000000 django_nets_core-0.1.76/nets_core/auth_urls.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      229 2024-05-05 05:05:51.000000 django_nets_core-0.1.76/nets_core/celery.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     4901 2024-05-05 18:50:21.000000 django_nets_core-0.1.76/nets_core/decorators.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3276 2024-05-04 23:43:26.000000 django_nets_core-0.1.76/nets_core/firebase_messages.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     6465 2024-05-04 23:43:26.000000 django_nets_core-0.1.76/nets_core/handlers.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     2477 2024-05-04 23:43:26.000000 django_nets_core-0.1.76/nets_core/listeners.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     4460 2024-05-05 18:01:33.000000 django_nets_core-0.1.76/nets_core/mail.py
--rwxrwxr-x   0 dev       (1001) dev       (1001)      665 2024-05-04 23:43:26.000000 django_nets_core-0.1.76/nets_core/manage.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 19:36:11.787625 django_nets_core-0.1.76/nets_core/management/
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 19:36:11.791625 django_nets_core-0.1.76/nets_core/management/commands/
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-05 02:03:24.000000 django_nets_core-0.1.76/nets_core/management/commands/__init__.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 19:36:11.791625 django_nets_core-0.1.76/nets_core/management/commands/__pycache__/
--rw-rw-r--   0 dev       (1001) dev       (1001)      165 2024-05-05 02:44:07.000000 django_nets_core-0.1.76/nets_core/management/commands/__pycache__/__init__.cpython-312.pyc
--rw-rw-r--   0 dev       (1001) dev       (1001)    28055 2024-05-05 05:05:51.000000 django_nets_core-0.1.76/nets_core/management/commands/__pycache__/nets-settings.cpython-312.pyc
--rw-rw-r--   0 dev       (1001) dev       (1001)    22911 2024-05-05 16:06:29.000000 django_nets_core-0.1.76/nets_core/management/commands/nets-settings.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 19:36:11.795626 django_nets_core-0.1.76/nets_core/middleware/
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 19:36:11.795626 django_nets_core-0.1.76/nets_core/middleware/__pycache__/
--rw-rw-r--   0 dev       (1001) dev       (1001)     3004 2024-05-05 04:39:30.000000 django_nets_core-0.1.76/nets_core/middleware/__pycache__/auth_token.cpython-312.pyc
--rw-rw-r--   0 dev       (1001) dev       (1001)     2003 2024-05-04 23:43:26.000000 django_nets_core-0.1.76/nets_core/middleware/auth_token.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 19:36:11.795626 django_nets_core-0.1.76/nets_core/migrations/
--rw-rw-r--   0 dev       (1001) dev       (1001)     5274 2024-05-04 23:43:26.000000 django_nets_core-0.1.76/nets_core/migrations/0001_initial.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      422 2024-05-04 23:43:26.000000 django_nets_core-0.1.76/nets_core/migrations/0002_alter_verificationcode_token.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     2208 2024-05-04 23:43:26.000000 django_nets_core-0.1.76/nets_core/migrations/0003_userdevice.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      360 2024-05-04 23:43:26.000000 django_nets_core-0.1.76/nets_core/migrations/0004_remove_userdevice_device_id_userdevice_uuid.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      480 2024-05-04 23:43:26.000000 django_nets_core-0.1.76/nets_core/migrations/0005_userdevice_uuid.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      454 2024-05-04 23:43:26.000000 django_nets_core-0.1.76/nets_core/migrations/0006_verificationcode_device.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      533 2024-05-04 23:43:26.000000 django_nets_core-0.1.76/nets_core/migrations/0007_alter_verificationcode_device.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     2056 2024-05-04 23:43:26.000000 django_nets_core-0.1.76/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      455 2024-05-04 23:43:26.000000 django_nets_core-0.1.76/nets_core/migrations/0009_userdevice_ip.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     6844 2024-05-05 19:06:27.000000 django_nets_core-0.1.76/nets_core/migrations/0010_permission_role_userrole_and_more.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      427 2024-05-05 19:35:28.000000 django_nets_core-0.1.76/nets_core/migrations/0011_role_enabled.py
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.76/nets_core/migrations/__init__.py
--rw-rw-r--   0 dev       (1001) dev       (1001)    12997 2024-05-05 19:21:33.000000 django_nets_core-0.1.76/nets_core/models.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     6425 2024-05-04 23:43:26.000000 django_nets_core-0.1.76/nets_core/params.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      902 2024-05-04 23:43:26.000000 django_nets_core-0.1.76/nets_core/responses.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3055 2024-05-04 23:43:26.000000 django_nets_core-0.1.76/nets_core/security.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3387 2024-05-05 18:22:43.000000 django_nets_core-0.1.76/nets_core/settings.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     1820 2024-05-05 05:05:51.000000 django_nets_core-0.1.76/nets_core/settings_nets.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      753 2024-05-05 05:16:02.000000 django_nets_core-0.1.76/nets_core/tasks.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 19:36:11.791625 django_nets_core-0.1.76/nets_core/templates/
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 19:36:11.795626 django_nets_core-0.1.76/nets_core/templates/nets_core/
--rw-rw-r--   0 dev       (1001) dev       (1001)     6978 2024-05-04 23:43:26.000000 django_nets_core-0.1.76/nets_core/templates/nets_core/base.html
--rw-rw-r--   0 dev       (1001) dev       (1001)     1954 2024-05-04 23:43:26.000000 django_nets_core-0.1.76/nets_core/templates/nets_core/delete_account.html
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-05 18:03:29.000000 django_nets_core-0.1.76/nets_core/templates/nets_core/delete_account_info.html
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 19:36:11.795626 django_nets_core-0.1.76/nets_core/templates/nets_core/email/
--rw-rw-r--   0 dev       (1001) dev       (1001)    16103 2024-05-04 23:43:26.000000 django_nets_core-0.1.76/nets_core/templates/nets_core/email/base_email.html
--rw-rw-r--   0 dev       (1001) dev       (1001)     1032 2024-05-04 23:43:26.000000 django_nets_core-0.1.76/nets_core/templates/nets_core/email/new_login.html
--rw-rw-r--   0 dev       (1001) dev       (1001)      316 2024-05-04 23:43:26.000000 django_nets_core-0.1.76/nets_core/templates/nets_core/email/verification_code.html
--rw-rw-r--   0 dev       (1001) dev       (1001)      824 2024-05-04 23:43:26.000000 django_nets_core-0.1.76/nets_core/urls.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3003 2024-05-05 18:49:07.000000 django_nets_core-0.1.76/nets_core/utils.py
--rw-rw-r--   0 dev       (1001) dev       (1001)    11727 2024-05-05 18:04:42.000000 django_nets_core-0.1.76/nets_core/views.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      395 2024-05-04 23:43:26.000000 django_nets_core-0.1.76/nets_core/wsgi.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      100 2024-05-05 00:47:40.000000 django_nets_core-0.1.76/pyproject.toml
--rw-rw-r--   0 dev       (1001) dev       (1001)      181 2024-05-05 01:49:02.000000 django_nets_core-0.1.76/requirements.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)     1334 2024-05-05 19:36:11.795626 django_nets_core-0.1.76/setup.cfg
--rw-rw-r--   0 dev       (1001) dev       (1001)       38 2024-05-04 23:43:26.000000 django_nets_core-0.1.76/setup.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 19:48:43.053340 django_nets_core-0.1.77/
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.77/LICENSE
+-rw-rw-r--   0 dev       (1001) dev       (1001)      304 2024-05-05 15:47:07.000000 django_nets_core-0.1.77/MANIFEST.in
+-rw-r--r--   0 dev       (1001) dev       (1001)    13678 2024-05-05 19:48:43.053340 django_nets_core-0.1.77/PKG-INFO
+-rw-rw-r--   0 dev       (1001) dev       (1001)    12153 2024-05-05 18:59:42.000000 django_nets_core-0.1.77/README.rst
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 19:48:43.053340 django_nets_core-0.1.77/django_nets_core.egg-info/
+-rw-r--r--   0 dev       (1001) dev       (1001)    13678 2024-05-05 19:48:43.000000 django_nets_core-0.1.77/django_nets_core.egg-info/PKG-INFO
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2015 2024-05-05 19:48:43.000000 django_nets_core-0.1.77/django_nets_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)        1 2024-05-05 19:48:43.000000 django_nets_core-0.1.77/django_nets_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)      286 2024-05-05 19:48:43.000000 django_nets_core-0.1.77/django_nets_core.egg-info/requires.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)       10 2024-05-05 19:48:43.000000 django_nets_core-0.1.77/django_nets_core.egg-info/top_level.txt
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 19:48:43.053340 django_nets_core-0.1.77/nets_core/
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.77/nets_core/__init__.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2440 2024-05-05 19:35:20.000000 django_nets_core-0.1.77/nets_core/admin.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      206 2024-05-04 23:43:26.000000 django_nets_core-0.1.77/nets_core/apps.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      807 2024-05-05 05:05:51.000000 django_nets_core-0.1.77/nets_core/asgi.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      537 2024-05-04 23:43:26.000000 django_nets_core-0.1.77/nets_core/auth_urls.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      229 2024-05-05 05:05:51.000000 django_nets_core-0.1.77/nets_core/celery.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     4901 2024-05-05 18:50:21.000000 django_nets_core-0.1.77/nets_core/decorators.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3276 2024-05-04 23:43:26.000000 django_nets_core-0.1.77/nets_core/firebase_messages.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     6465 2024-05-04 23:43:26.000000 django_nets_core-0.1.77/nets_core/handlers.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2477 2024-05-04 23:43:26.000000 django_nets_core-0.1.77/nets_core/listeners.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     4460 2024-05-05 18:01:33.000000 django_nets_core-0.1.77/nets_core/mail.py
+-rwxrwxr-x   0 dev       (1001) dev       (1001)      665 2024-05-04 23:43:26.000000 django_nets_core-0.1.77/nets_core/manage.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 19:48:43.049340 django_nets_core-0.1.77/nets_core/management/
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 19:48:43.053340 django_nets_core-0.1.77/nets_core/management/commands/
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-05 02:03:24.000000 django_nets_core-0.1.77/nets_core/management/commands/__init__.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 19:48:43.053340 django_nets_core-0.1.77/nets_core/management/commands/__pycache__/
+-rw-rw-r--   0 dev       (1001) dev       (1001)      165 2024-05-05 02:44:07.000000 django_nets_core-0.1.77/nets_core/management/commands/__pycache__/__init__.cpython-312.pyc
+-rw-rw-r--   0 dev       (1001) dev       (1001)    28055 2024-05-05 05:05:51.000000 django_nets_core-0.1.77/nets_core/management/commands/__pycache__/nets-settings.cpython-312.pyc
+-rw-rw-r--   0 dev       (1001) dev       (1001)    22911 2024-05-05 16:06:29.000000 django_nets_core-0.1.77/nets_core/management/commands/nets-settings.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 19:48:43.053340 django_nets_core-0.1.77/nets_core/middleware/
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 19:48:43.053340 django_nets_core-0.1.77/nets_core/middleware/__pycache__/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3004 2024-05-05 04:39:30.000000 django_nets_core-0.1.77/nets_core/middleware/__pycache__/auth_token.cpython-312.pyc
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2056 2024-05-05 19:48:36.000000 django_nets_core-0.1.77/nets_core/middleware/auth_token.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 19:48:43.053340 django_nets_core-0.1.77/nets_core/migrations/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     5274 2024-05-04 23:43:26.000000 django_nets_core-0.1.77/nets_core/migrations/0001_initial.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      422 2024-05-04 23:43:26.000000 django_nets_core-0.1.77/nets_core/migrations/0002_alter_verificationcode_token.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2208 2024-05-04 23:43:26.000000 django_nets_core-0.1.77/nets_core/migrations/0003_userdevice.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      360 2024-05-04 23:43:26.000000 django_nets_core-0.1.77/nets_core/migrations/0004_remove_userdevice_device_id_userdevice_uuid.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      480 2024-05-04 23:43:26.000000 django_nets_core-0.1.77/nets_core/migrations/0005_userdevice_uuid.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      454 2024-05-04 23:43:26.000000 django_nets_core-0.1.77/nets_core/migrations/0006_verificationcode_device.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      533 2024-05-04 23:43:26.000000 django_nets_core-0.1.77/nets_core/migrations/0007_alter_verificationcode_device.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2056 2024-05-04 23:43:26.000000 django_nets_core-0.1.77/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      455 2024-05-04 23:43:26.000000 django_nets_core-0.1.77/nets_core/migrations/0009_userdevice_ip.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     6844 2024-05-05 19:06:27.000000 django_nets_core-0.1.77/nets_core/migrations/0010_permission_role_userrole_and_more.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      427 2024-05-05 19:35:28.000000 django_nets_core-0.1.77/nets_core/migrations/0011_role_enabled.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.77/nets_core/migrations/__init__.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)    12997 2024-05-05 19:21:33.000000 django_nets_core-0.1.77/nets_core/models.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     6425 2024-05-04 23:43:26.000000 django_nets_core-0.1.77/nets_core/params.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      902 2024-05-04 23:43:26.000000 django_nets_core-0.1.77/nets_core/responses.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3055 2024-05-04 23:43:26.000000 django_nets_core-0.1.77/nets_core/security.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3387 2024-05-05 18:22:43.000000 django_nets_core-0.1.77/nets_core/settings.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1820 2024-05-05 05:05:51.000000 django_nets_core-0.1.77/nets_core/settings_nets.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      753 2024-05-05 05:16:02.000000 django_nets_core-0.1.77/nets_core/tasks.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 19:48:43.049340 django_nets_core-0.1.77/nets_core/templates/
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 19:48:43.053340 django_nets_core-0.1.77/nets_core/templates/nets_core/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     6978 2024-05-04 23:43:26.000000 django_nets_core-0.1.77/nets_core/templates/nets_core/base.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1954 2024-05-04 23:43:26.000000 django_nets_core-0.1.77/nets_core/templates/nets_core/delete_account.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-05 18:03:29.000000 django_nets_core-0.1.77/nets_core/templates/nets_core/delete_account_info.html
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-05 19:48:43.053340 django_nets_core-0.1.77/nets_core/templates/nets_core/email/
+-rw-rw-r--   0 dev       (1001) dev       (1001)    16103 2024-05-04 23:43:26.000000 django_nets_core-0.1.77/nets_core/templates/nets_core/email/base_email.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1032 2024-05-04 23:43:26.000000 django_nets_core-0.1.77/nets_core/templates/nets_core/email/new_login.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)      316 2024-05-04 23:43:26.000000 django_nets_core-0.1.77/nets_core/templates/nets_core/email/verification_code.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)      824 2024-05-04 23:43:26.000000 django_nets_core-0.1.77/nets_core/urls.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3003 2024-05-05 18:49:07.000000 django_nets_core-0.1.77/nets_core/utils.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)    11727 2024-05-05 18:04:42.000000 django_nets_core-0.1.77/nets_core/views.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      395 2024-05-04 23:43:26.000000 django_nets_core-0.1.77/nets_core/wsgi.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      100 2024-05-05 00:47:40.000000 django_nets_core-0.1.77/pyproject.toml
+-rw-rw-r--   0 dev       (1001) dev       (1001)      181 2024-05-05 01:49:02.000000 django_nets_core-0.1.77/requirements.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1334 2024-05-05 19:48:43.057340 django_nets_core-0.1.77/setup.cfg
+-rw-rw-r--   0 dev       (1001) dev       (1001)       38 2024-05-04 23:43:26.000000 django_nets_core-0.1.77/setup.py
```

### Comparing `django_nets_core-0.1.76/PKG-INFO` & `django_nets_core-0.1.77/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-nets-core
-Version: 0.1.76
+Version: 0.1.77
 Summary: A lazy API rest request handler.
 Home-page: https://github.com/esbozos/django-nets-core
 Author: Norman Torres
 Author-email: norman.nets@gmail.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django_nets_core-0.1.76/README.rst` & `django_nets_core-0.1.77/README.rst`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.76/django_nets_core.egg-info/PKG-INFO` & `django_nets_core-0.1.77/django_nets_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-nets-core
-Version: 0.1.76
+Version: 0.1.77
 Summary: A lazy API rest request handler.
 Home-page: https://github.com/esbozos/django-nets-core
 Author: Norman Torres
 Author-email: norman.nets@gmail.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django_nets_core-0.1.76/django_nets_core.egg-info/SOURCES.txt` & `django_nets_core-0.1.77/django_nets_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.76/nets_core/admin.py` & `django_nets_core-0.1.77/nets_core/admin.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.76/nets_core/asgi.py` & `django_nets_core-0.1.77/nets_core/asgi.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.76/nets_core/auth_urls.py` & `django_nets_core-0.1.77/nets_core/auth_urls.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.76/nets_core/decorators.py` & `django_nets_core-0.1.77/nets_core/decorators.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.76/nets_core/firebase_messages.py` & `django_nets_core-0.1.77/nets_core/firebase_messages.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.76/nets_core/handlers.py` & `django_nets_core-0.1.77/nets_core/handlers.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.76/nets_core/listeners.py` & `django_nets_core-0.1.77/nets_core/listeners.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.76/nets_core/mail.py` & `django_nets_core-0.1.77/nets_core/mail.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.76/nets_core/manage.py` & `django_nets_core-0.1.77/nets_core/manage.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.76/nets_core/management/commands/__pycache__/nets-settings.cpython-312.pyc` & `django_nets_core-0.1.77/nets_core/management/commands/__pycache__/nets-settings.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.76/nets_core/management/commands/nets-settings.py` & `django_nets_core-0.1.77/nets_core/management/commands/nets-settings.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.76/nets_core/middleware/__pycache__/auth_token.cpython-312.pyc` & `django_nets_core-0.1.77/nets_core/middleware/__pycache__/auth_token.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.76/nets_core/middleware/auth_token.py` & `django_nets_core-0.1.77/nets_core/middleware/auth_token.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     u = user or AnonymousUser()
 
     return u
 
 
 class AuthTokenMiddleware(BaseMiddleware):
     """
-    Token authorization middleware for Django Channels 3
+    Token authorization middleware for Django Channels 
     And OAUTH2 PROVIDER
     """
 
     def populate_scope(self, scope):
         if "user" not in scope:
             scope["user"] = UserLazyObject()
 
@@ -56,12 +56,13 @@
     async def __call__(self, scope, receive, send):
         scope = dict(scope)
         # Scope injection/mutation per this middleware's needs.
         self.populate_scope(scope)
         # Grab the finalized/resolved scope
         await self.resolve_scope(scope)
 
-        return await super().__call__(scope, receive, send)
+        return await self.app(scope, receive, send)
+        # return await super().__call__(scope, receive, send)
 
 
 def AuthTokenMiddlewareStack(inner): return (
     AuthMiddlewareStack(AuthTokenMiddleware(inner)))
```

### Comparing `django_nets_core-0.1.76/nets_core/migrations/0001_initial.py` & `django_nets_core-0.1.77/nets_core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.76/nets_core/migrations/0003_userdevice.py` & `django_nets_core-0.1.77/nets_core/migrations/0003_userdevice.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.76/nets_core/migrations/0007_alter_verificationcode_device.py` & `django_nets_core-0.1.77/nets_core/migrations/0007_alter_verificationcode_device.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.76/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py` & `django_nets_core-0.1.77/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.76/nets_core/migrations/0010_permission_role_userrole_and_more.py` & `django_nets_core-0.1.77/nets_core/migrations/0010_permission_role_userrole_and_more.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.76/nets_core/models.py` & `django_nets_core-0.1.77/nets_core/models.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.76/nets_core/params.py` & `django_nets_core-0.1.77/nets_core/params.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.76/nets_core/responses.py` & `django_nets_core-0.1.77/nets_core/responses.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.76/nets_core/security.py` & `django_nets_core-0.1.77/nets_core/security.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.76/nets_core/settings.py` & `django_nets_core-0.1.77/nets_core/settings.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.76/nets_core/settings_nets.py` & `django_nets_core-0.1.77/nets_core/settings_nets.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.76/nets_core/tasks.py` & `django_nets_core-0.1.77/nets_core/tasks.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.76/nets_core/templates/nets_core/base.html` & `django_nets_core-0.1.77/nets_core/templates/nets_core/base.html`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.76/nets_core/templates/nets_core/delete_account.html` & `django_nets_core-0.1.77/nets_core/templates/nets_core/delete_account.html`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.76/nets_core/templates/nets_core/email/base_email.html` & `django_nets_core-0.1.77/nets_core/templates/nets_core/email/base_email.html`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.76/nets_core/templates/nets_core/email/new_login.html` & `django_nets_core-0.1.77/nets_core/templates/nets_core/email/new_login.html`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.76/nets_core/urls.py` & `django_nets_core-0.1.77/nets_core/urls.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.76/nets_core/utils.py` & `django_nets_core-0.1.77/nets_core/utils.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.76/nets_core/views.py` & `django_nets_core-0.1.77/nets_core/views.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.76/setup.cfg` & `django_nets_core-0.1.77/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-nets-core
-version = 0.1.76
+version = 0.1.77
 description = A lazy API rest request handler.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/esbozos/django-nets-core
 author = Norman Torres
 author_email = norman.nets@gmail.com
 license = BSD-3-Clause
```

