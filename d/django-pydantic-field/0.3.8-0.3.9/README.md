# Comparing `tmp/django_pydantic_field-0.3.8.tar.gz` & `tmp/django_pydantic_field-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pydantic_field-0.3.8.tar", last modified: Tue Apr 23 13:46:24 2024, max compression
+gzip compressed data, was "django_pydantic_field-0.3.9.tar", last modified: Sun May  5 20:09:51 2024, max compression
```

## Comparing `django_pydantic_field-0.3.8.tar` & `django_pydantic_field-0.3.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:46:24.173186 django_pydantic_field-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12985 2024-04-23 13:46:24.173186 django_pydantic_field-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8555 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:46:24.165186 django_pydantic_field-0.3.8/django_pydantic_field/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/_migration_serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:46:24.165186 django_pydantic_field-0.3.8/django_pydantic_field/compat/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/compat/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11859 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/compat/django.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/compat/functools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/compat/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/compat/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/compat/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/fields.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/forms.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/rest_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/rest_framework.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:46:24.169186 django_pydantic_field-0.3.8/django_pydantic_field/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v1/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7232 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v1/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v1/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v1/rest_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v1/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:46:24.169186 django_pydantic_field-0.3.8/django_pydantic_field/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11019 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v2/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v2/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:46:24.169186 django_pydantic_field-0.3.8/django_pydantic_field/v2/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v2/rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v2/rest_framework/coreapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v2/rest_framework/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v2/rest_framework/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v2/rest_framework/openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v2/rest_framework/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v2/rest_framework/renderers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9101 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v2/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:46:24.173186 django_pydantic_field-0.3.8/django_pydantic_field.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12985 2024-04-23 13:46:24.000000 django_pydantic_field-0.3.8/django_pydantic_field.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-23 13:46:24.000000 django_pydantic_field-0.3.8/django_pydantic_field.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:46:24.000000 django_pydantic_field-0.3.8/django_pydantic_field.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-23 13:46:24.000000 django_pydantic_field-0.3.8/django_pydantic_field.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 13:46:24.000000 django_pydantic_field-0.3.8/django_pydantic_field.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 13:46:24.173186 django_pydantic_field-0.3.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:46:24.173186 django_pydantic_field-0.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/tests/test_e2e_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11489 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/tests/test_migration_serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/tests/test_model_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/tests/test_sample_app_migrations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:09:51.096223 django_pydantic_field-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12947 2024-05-05 20:09:51.096223 django_pydantic_field-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8555 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:09:51.088223 django_pydantic_field-0.3.9/django_pydantic_field/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/django_pydantic_field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/django_pydantic_field/_migration_serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:09:51.088223 django_pydantic_field-0.3.9/django_pydantic_field/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/django_pydantic_field/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/django_pydantic_field/compat/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11873 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/django_pydantic_field/compat/django.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/django_pydantic_field/compat/functools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/django_pydantic_field/compat/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/django_pydantic_field/compat/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/django_pydantic_field/compat/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/django_pydantic_field/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/django_pydantic_field/fields.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/django_pydantic_field/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/django_pydantic_field/forms.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/django_pydantic_field/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/django_pydantic_field/rest_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/django_pydantic_field/rest_framework.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:09:51.088223 django_pydantic_field-0.3.9/django_pydantic_field/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/django_pydantic_field/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/django_pydantic_field/v1/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7737 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/django_pydantic_field/v1/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/django_pydantic_field/v1/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/django_pydantic_field/v1/rest_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/django_pydantic_field/v1/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:09:51.088223 django_pydantic_field-0.3.9/django_pydantic_field/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/django_pydantic_field/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11430 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/django_pydantic_field/v2/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/django_pydantic_field/v2/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:09:51.092223 django_pydantic_field-0.3.9/django_pydantic_field/v2/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/django_pydantic_field/v2/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/django_pydantic_field/v2/rest_framework/coreapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/django_pydantic_field/v2/rest_framework/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/django_pydantic_field/v2/rest_framework/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/django_pydantic_field/v2/rest_framework/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/django_pydantic_field/v2/rest_framework/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/django_pydantic_field/v2/rest_framework/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9101 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/django_pydantic_field/v2/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/django_pydantic_field/v2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:09:51.092223 django_pydantic_field-0.3.9/django_pydantic_field.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12947 2024-05-05 20:09:51.000000 django_pydantic_field-0.3.9/django_pydantic_field.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-05 20:09:51.000000 django_pydantic_field-0.3.9/django_pydantic_field.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 20:09:51.000000 django_pydantic_field-0.3.9/django_pydantic_field.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-05 20:09:51.000000 django_pydantic_field-0.3.9/django_pydantic_field.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-05 20:09:51.000000 django_pydantic_field-0.3.9/django_pydantic_field.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 20:09:51.096223 django_pydantic_field-0.3.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:09:51.092223 django_pydantic_field-0.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/tests/test_e2e_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11678 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/tests/test_migration_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/tests/test_model_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-05 20:09:46.000000 django_pydantic_field-0.3.9/tests/test_sample_app_migrations.py
```

### Comparing `django_pydantic_field-0.3.8/LICENSE` & `django_pydantic_field-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django_pydantic_field-0.3.8/PKG-INFO` & `django_pydantic_field-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pydantic-field
-Version: 0.3.8
+Version: 0.3.9
 Summary: Django JSONField with Pydantic models as a Schema
 Author-email: Savva Surenkov <savva@surenkov.space>
 License: MIT License
         
         Copyright (c) 2024 Savva Surenkov and django-pydantic-field contributors.
         See the contributors at https://github.com/surenkov/django-pydantic-field/contributors
         
@@ -66,16 +66,15 @@
 Requires-Dist: inflection; extra == "openapi"
 Provides-Extra: coreapi
 Requires-Dist: coreapi; extra == "coreapi"
 Provides-Extra: jsonform
 Requires-Dist: django_jsonform<3,>=2.0; extra == "jsonform"
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: isort; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest~=7.4; extra == "dev"
 Requires-Dist: djangorestframework<4,>=3.11; extra == "dev"
 Requires-Dist: django-stubs[compatible-mypy]~=4.2; extra == "dev"
 Requires-Dist: djangorestframework-stubs[compatible-mypy]~=3.14; extra == "dev"
 Requires-Dist: pytest-django<5,>=4.5; extra == "dev"
```

### Comparing `django_pydantic_field-0.3.8/README.md` & `django_pydantic_field-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `django_pydantic_field-0.3.8/django_pydantic_field/compat/deprecation.py` & `django_pydantic_field-0.3.9/django_pydantic_field/compat/deprecation.py`

 * *Files identical despite different names*

### Comparing `django_pydantic_field-0.3.8/django_pydantic_field/compat/django.py` & `django_pydantic_field-0.3.9/django_pydantic_field/compat/django.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
             return value
         if PYDANTIC_V1:
             return FieldInfo(**value.kwargs)
 
         origin = GenericContainer.unwrap(value.origin)
         metadata = tuple(map(BaseContainer.unwrap, value.metadata))
         try:
-            annotated_args = (origin, *metadata)
+            annotated_args = (origin, *metadata)  # noqa: F841
             annotation = te.Annotated[annotated_args]
         except TypeError:
             annotation = None
 
         return FieldInfo(annotation=annotation, **value.kwargs)
 
     def __eq__(self, other):
```

### Comparing `django_pydantic_field-0.3.8/django_pydantic_field/compat/imports.py` & `django_pydantic_field-0.3.9/django_pydantic_field/compat/imports.py`

 * *Files identical despite different names*

### Comparing `django_pydantic_field-0.3.8/django_pydantic_field/fields.pyi` & `django_pydantic_field-0.3.9/django_pydantic_field/fields.pyi`

 * *Files identical despite different names*

### Comparing `django_pydantic_field-0.3.8/django_pydantic_field/forms.pyi` & `django_pydantic_field-0.3.9/django_pydantic_field/forms.pyi`

 * *Files identical despite different names*

### Comparing `django_pydantic_field-0.3.8/django_pydantic_field/rest_framework.pyi` & `django_pydantic_field-0.3.9/django_pydantic_field/rest_framework.pyi`

 * *Files identical despite different names*

### Comparing `django_pydantic_field-0.3.8/django_pydantic_field/v1/base.py` & `django_pydantic_field-0.3.9/django_pydantic_field/v1/base.py`

 * *Files identical despite different names*

### Comparing `django_pydantic_field-0.3.8/django_pydantic_field/v1/fields.py` & `django_pydantic_field-0.3.9/django_pydantic_field/v1/fields.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,16 +33,22 @@
 
     field: "PydanticSchemaField"
 
     def __set__(self, obj, value):
         obj.__dict__[self.field.attname] = self.field.to_python(value)
 
 
+class UninitializedSchemaAttribute(SchemaAttribute):
+    def __set__(self, obj, value):
+        if value is not None:
+            value = self.field.to_python(value)
+        obj.__dict__[self.field.attname] = value
+
+
 class PydanticSchemaField(JSONField, t.Generic[base.ST]):
-    descriptor_class = SchemaAttribute
     _is_prepared_schema: bool = False
 
     def __init__(
         self,
         *args,
         schema: t.Union[t.Type["base.ST"], "BaseContainer", "t.ForwardRef", str, None] = None,
         config: t.Optional["base.ConfigType"] = None,
@@ -57,16 +63,18 @@
     def __copy__(self):
         _, _, args, kwargs = self.deconstruct()
         copied = type(self)(*args, **kwargs)
         copied.set_attributes_from_name(self.name)
         return copied
 
     def get_default(self):
-        value = super().get_default()
-        return self.to_python(value)
+        default_value = super().get_default()
+        if self.has_default():
+            return self.to_python(default_value)
+        return default_value
 
     def to_python(self, value) -> "base.SchemaT":
         # Attempt to resolve forward referencing schema if it was not succesful
         # during `.contribute_to_class` call
         if not self._is_prepared_schema:
             self._prepare_model_schema()
         try:
@@ -100,14 +108,20 @@
         self._deconstruct_config(kwargs)
 
         kwargs.pop("decoder")
         kwargs.pop("encoder")
 
         return name, path, args, kwargs
 
+    @staticmethod
+    def descriptor_class(field: "PydanticSchemaField") -> DeferredAttribute:
+        if field.has_default():
+            return SchemaAttribute(field)
+        return UninitializedSchemaAttribute(field)
+
     def contribute_to_class(self, cls, name, private_only=False):
         if self.schema is None:
             self._resolve_schema_from_type_hints(cls, name)
 
         try:
             self._prepare_model_schema(cls)
         except NameError:
@@ -158,16 +172,15 @@
         cls = cls or getattr(self, "model", None)
         if cls is not None:
             base.prepare_schema(self.serializer_schema, cls)
             self._is_prepared_schema = True
 
     def _deconstruct_default(self, kwargs):
         default = kwargs.get("default", NOT_PROVIDED)
-
-        if not (default is NOT_PROVIDED or callable(default)):
+        if default is not NOT_PROVIDED and not callable(default):
             if self._is_prepared_schema:
                 default = self.get_prep_value(default)
             kwargs.update(default=default)
 
     def _deconstruct_schema(self, kwargs):
         kwargs.update(schema=GenericContainer.wrap(self.schema))
 
@@ -198,10 +211,10 @@
     default: "t.Union[base.SchemaT, t.Callable[[], base.SchemaT]]" = ...,
     *args,
     null: "t.Literal[False]" = ...,
     **kwargs,
 ) -> "base.ST": ...
 
 
-def SchemaField(schema=None, config=None, default=None, *args, **kwargs) -> t.Any:
+def SchemaField(schema=None, config=None, default=NOT_PROVIDED, *args, **kwargs) -> t.Any:  # type: ignore
     kwargs.update(schema=schema, config=config, default=default)
     return PydanticSchemaField(*args, **kwargs)
```

### Comparing `django_pydantic_field-0.3.8/django_pydantic_field/v1/forms.py` & `django_pydantic_field-0.3.9/django_pydantic_field/v1/forms.py`

 * *Files identical despite different names*

### Comparing `django_pydantic_field-0.3.8/django_pydantic_field/v1/rest_framework.py` & `django_pydantic_field-0.3.9/django_pydantic_field/v1/rest_framework.py`

 * *Files identical despite different names*

### Comparing `django_pydantic_field-0.3.8/django_pydantic_field/v1/utils.py` & `django_pydantic_field-0.3.9/django_pydantic_field/v1/utils.py`

 * *Files identical despite different names*

### Comparing `django_pydantic_field-0.3.8/django_pydantic_field/v2/fields.py` & `django_pydantic_field-0.3.9/django_pydantic_field/v2/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,16 +59,22 @@
     def __set_name__(self, owner, name):
         self.field.adapter.bind(owner, name)
 
     def __set__(self, obj, value):
         obj.__dict__[self.field.attname] = self.field.to_python(value)
 
 
+class UninitializedSchemaAttribute(SchemaAttribute):
+    def __set__(self, obj, value):
+        if value is not None:
+            value = self.field.to_python(value)
+        obj.__dict__[self.field.attname] = value
+
+
 class PydanticSchemaField(JSONField, ty.Generic[types.ST]):
-    descriptor_class: type[DeferredAttribute] = SchemaAttribute
     adapter: types.SchemaAdapter
 
     def __init__(
         self,
         *args,
         schema: type[types.ST] | te.Annotated[type[types.ST], ...] | BaseContainer | ty.ForwardRef | str | None = None,
         config: pydantic.ConfigDict | None = None,
@@ -98,14 +104,20 @@
             kwargs["default"] = self._prepare_raw_value(default, include=None, exclude=None, round_trip=True)
 
         prep_schema = GenericContainer.wrap(self.adapter.prepared_schema)
         kwargs.update(schema=prep_schema, config=self.config, **self.export_kwargs)
 
         return field_name, import_path, args, kwargs
 
+    @staticmethod
+    def descriptor_class(field: PydanticSchemaField) -> DeferredAttribute:
+        if field.has_default():
+            return SchemaAttribute(field)
+        return UninitializedSchemaAttribute(field)
+
     def contribute_to_class(self, cls: types.DjangoModelType, name: str, private_only: bool = False) -> None:
         self.adapter.bind(cls, name)
         super().contribute_to_class(cls, name, private_only)
 
     def check(self, **kwargs: ty.Any) -> list[checks.CheckMessage]:
         # Remove checks of using mutable datastructure instances as `default` values, since they'll be adapted anyway.
         performed_checks = [check for check in super().check(**kwargs) if check.id != "fields.E010"]
@@ -114,15 +126,16 @@
             self.adapter.validate_schema()
         except types.ImproperlyConfiguredSchema as exc:
             message = f"Cannot resolve the schema. Original error: \n{exc.args[0]}"
             performed_checks.append(checks.Error(message, obj=self, id="pydantic.E001"))
 
         try:
             # Test that the default value conforms to the schema.
-            self.get_prep_value(self.get_default())
+            if self.has_default():
+                self.get_prep_value(self.get_default())
         except pydantic.ValidationError as exc:
             message = f"Default value cannot be adapted to the schema. Pydantic error: \n{str(exc)}"
             performed_checks.append(checks.Error(message, obj=self, id="pydantic.E002"))
 
         if {"include", "exclude"} & self.export_kwargs.keys():
             # Try to prepare the default value to test export ability against it.
             schema_default = self.get_default()
```

### Comparing `django_pydantic_field-0.3.8/django_pydantic_field/v2/forms.py` & `django_pydantic_field-0.3.9/django_pydantic_field/v2/forms.py`

 * *Files identical despite different names*

### Comparing `django_pydantic_field-0.3.8/django_pydantic_field/v2/rest_framework/__init__.py` & `django_pydantic_field-0.3.9/django_pydantic_field/v2/rest_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `django_pydantic_field-0.3.8/django_pydantic_field/v2/rest_framework/coreapi.py` & `django_pydantic_field-0.3.9/django_pydantic_field/v2/rest_framework/coreapi.py`

 * *Files identical despite different names*

### Comparing `django_pydantic_field-0.3.8/django_pydantic_field/v2/rest_framework/fields.py` & `django_pydantic_field-0.3.9/django_pydantic_field/v2/rest_framework/fields.py`

 * *Files identical despite different names*

### Comparing `django_pydantic_field-0.3.8/django_pydantic_field/v2/rest_framework/mixins.py` & `django_pydantic_field-0.3.9/django_pydantic_field/v2/rest_framework/mixins.py`

 * *Files identical despite different names*

### Comparing `django_pydantic_field-0.3.8/django_pydantic_field/v2/rest_framework/openapi.py` & `django_pydantic_field-0.3.9/django_pydantic_field/v2/rest_framework/openapi.py`

 * *Files identical despite different names*

### Comparing `django_pydantic_field-0.3.8/django_pydantic_field/v2/rest_framework/parsers.py` & `django_pydantic_field-0.3.9/django_pydantic_field/v2/rest_framework/parsers.py`

 * *Files identical despite different names*

### Comparing `django_pydantic_field-0.3.8/django_pydantic_field/v2/rest_framework/renderers.py` & `django_pydantic_field-0.3.9/django_pydantic_field/v2/rest_framework/renderers.py`

 * *Files identical despite different names*

### Comparing `django_pydantic_field-0.3.8/django_pydantic_field/v2/types.py` & `django_pydantic_field-0.3.9/django_pydantic_field/v2/types.py`

 * *Files identical despite different names*

### Comparing `django_pydantic_field-0.3.8/django_pydantic_field/v2/utils.py` & `django_pydantic_field-0.3.9/django_pydantic_field/v2/utils.py`

 * *Files identical despite different names*

### Comparing `django_pydantic_field-0.3.8/django_pydantic_field.egg-info/PKG-INFO` & `django_pydantic_field-0.3.9/django_pydantic_field.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pydantic-field
-Version: 0.3.8
+Version: 0.3.9
 Summary: Django JSONField with Pydantic models as a Schema
 Author-email: Savva Surenkov <savva@surenkov.space>
 License: MIT License
         
         Copyright (c) 2024 Savva Surenkov and django-pydantic-field contributors.
         See the contributors at https://github.com/surenkov/django-pydantic-field/contributors
         
@@ -66,16 +66,15 @@
 Requires-Dist: inflection; extra == "openapi"
 Provides-Extra: coreapi
 Requires-Dist: coreapi; extra == "coreapi"
 Provides-Extra: jsonform
 Requires-Dist: django_jsonform<3,>=2.0; extra == "jsonform"
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: isort; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest~=7.4; extra == "dev"
 Requires-Dist: djangorestframework<4,>=3.11; extra == "dev"
 Requires-Dist: django-stubs[compatible-mypy]~=4.2; extra == "dev"
 Requires-Dist: djangorestframework-stubs[compatible-mypy]~=3.14; extra == "dev"
 Requires-Dist: pytest-django<5,>=4.5; extra == "dev"
```

### Comparing `django_pydantic_field-0.3.8/django_pydantic_field.egg-info/SOURCES.txt` & `django_pydantic_field-0.3.9/django_pydantic_field.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_pydantic_field-0.3.8/django_pydantic_field.egg-info/requires.txt` & `django_pydantic_field-0.3.9/django_pydantic_field.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 psycopg[binary]<4,>=3.1
 
 [coreapi]
 coreapi
 
 [dev]
 build
-black
-isort
+ruff
 mypy
 pre-commit
 pytest~=7.4
 djangorestframework<4,>=3.11
 django-stubs[compatible-mypy]~=4.2
 djangorestframework-stubs[compatible-mypy]~=3.14
 pytest-django<5,>=4.5
```

### Comparing `django_pydantic_field-0.3.8/pyproject.toml` & `django_pydantic_field-0.3.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django-pydantic-field"
-version = "0.3.8"
+version = "0.3.9"
 description = "Django JSONField with Pydantic models as a Schema"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [
     { name = "Savva Surenkov", email = "savva@surenkov.space" },
 ]
 
@@ -49,16 +49,15 @@
 
 [project.optional-dependencies]
 openapi = ["uritemplate", "inflection"]
 coreapi = ["coreapi"]
 jsonform = ["django_jsonform>=2.0,<3"]
 dev = [
     "build",
-    "black",
-    "isort",
+    "ruff",
     "mypy",
     "pre-commit",
     "pytest~=7.4",
     "djangorestframework>=3.11,<4",
     "django-stubs[compatible-mypy]~=4.2",
     "djangorestframework-stubs[compatible-mypy]~=3.14",
     "pytest-django>=4.5,<5",
@@ -78,34 +77,16 @@
 
 [project.urls]
 Homepage = "https://github.com/surenkov/django-pydantic-field"
 Documentation = "https://github.com/surenkov/django-pydantic-field"
 Source = "https://github.com/surenkov/django-pydantic-field"
 Changelog = "https://github.com/surenkov/django-pydantic-field/releases"
 
-[tool.isort]
-py_version = 311
-profile = "black"
-line_length = 120
-multi_line_output = 3
-include_trailing_comma = true
-force_alphabetical_sort_within_sections = true
-force_grid_wrap = 0
-use_parentheses = true
-
-[tool.black]
-target-version = ["py38", "py39", "py310", "py311", "py312"]
+[tool.ruff]
 line-length = 120
-exclude = '''
-/(
-    \.pytest_cache
-  | \.venv
-  | venv
-)/
-'''
 
 [tool.mypy]
 plugins = [
     "mypy_django_plugin.main",
     "mypy_drf_plugin.main"
 ]
 exclude = [".env", ".venv", "tests"]
```

### Comparing `django_pydantic_field-0.3.8/tests/test_e2e_models.py` & `django_pydantic_field-0.3.9/tests/test_e2e_models.py`

 * *Files identical despite different names*

### Comparing `django_pydantic_field-0.3.8/tests/test_fields.py` & `django_pydantic_field-0.3.9/tests/test_fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,7 +310,14 @@
 
 def test_copy_field():
     copied = copy(Building.meta.field)
 
     assert copied.name == Building.meta.field.name
     assert copied.attname == Building.meta.field.attname
     assert copied.concrete == Building.meta.field.concrete
+
+
+def test_model_init_no_default():
+    try:
+        SampleModel()
+    except Exception:
+        pytest.fail("Model with schema field without a default value should be able to initialize")
```

### Comparing `django_pydantic_field-0.3.8/tests/test_imports.py` & `django_pydantic_field-0.3.9/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `django_pydantic_field-0.3.8/tests/test_migration_serializers.py` & `django_pydantic_field-0.3.9/tests/test_migration_serializers.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from django.db.migrations.writer import MigrationWriter
 import pytest
 
 import django_pydantic_field
 try:
     from django_pydantic_field.compat.django import GenericContainer
 except ImportError:
-    from django_pydantic_field._migration_serializers import GenericContainer
+    from django_pydantic_field._migration_serializers import GenericContainer  # noqa
 
 if sys.version_info < (3, 9):
     test_types = [
         str,
         list,
         t.List[str],
         t.Union[te.Literal["foo"], t.List[str]],
```

### Comparing `django_pydantic_field-0.3.8/tests/test_model_admin.py` & `django_pydantic_field-0.3.9/tests/test_model_admin.py`

 * *Files identical despite different names*

### Comparing `django_pydantic_field-0.3.8/tests/test_sample_app_migrations.py` & `django_pydantic_field-0.3.9/tests/test_sample_app_migrations.py`

 * *Files identical despite different names*

