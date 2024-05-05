# Comparing `tmp/gravitino-0.5.0.dev5.tar.gz` & `tmp/gravitino-0.5.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravitino-0.5.0.dev5.tar", last modified: Sat May  4 02:42:24 2024, max compression
+gzip compressed data, was "gravitino-0.5.0.dev6.tar", last modified: Sun May  5 07:14:17 2024, max compression
```

## Comparing `gravitino-0.5.0.dev5.tar` & `gravitino-0.5.0.dev6.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:42:23.999420 gravitino-0.5.0.dev5/
--rw-r--r--   0 xun        (501) staff       (20)     3774 2024-05-04 02:42:23.999280 gravitino-0.5.0.dev5/PKG-INFO
--rw-r--r--   0 xun        (501) staff       (20)     3484 2024-05-04 02:27:17.000000 gravitino-0.5.0.dev5/README.md
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:42:23.976213 gravitino-0.5.0.dev5/gravitino/
--rw-r--r--   0 xun        (501) staff       (20)      244 2024-04-08 10:35:22.000000 gravitino-0.5.0.dev5/gravitino/__init__.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:42:23.985647 gravitino-0.5.0.dev5/gravitino/api/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev5/gravitino/api/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)      942 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev5/gravitino/api/audit.py
--rw-r--r--   0 xun        (501) staff       (20)      440 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev5/gravitino/api/auditable.py
--rw-r--r--   0 xun        (501) staff       (20)     4113 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev5/gravitino/api/catalog.py
--rw-r--r--   0 xun        (501) staff       (20)     8759 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/api/catalog_change.py
--rw-r--r--   0 xun        (501) staff       (20)     3556 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/api/fileset.py
--rw-r--r--   0 xun        (501) staff       (20)     9226 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/api/fileset_change.py
--rw-r--r--   0 xun        (501) staff       (20)     1155 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/api/metalake.py
--rw-r--r--   0 xun        (501) staff       (20)     3403 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/api/metalake_change.py
--rw-r--r--   0 xun        (501) staff       (20)     1044 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/api/schema.py
--rw-r--r--   0 xun        (501) staff       (20)     4847 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/api/schema_change.py
--rw-r--r--   0 xun        (501) staff       (20)     3870 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/api/supports_schemas.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:42:23.986452 gravitino-0.5.0.dev5/gravitino/catalog/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev5/gravitino/catalog/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)     7079 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/catalog/base_schema_catalog.py
--rw-r--r--   0 xun        (501) staff       (20)     7344 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/catalog/fileset_catalog.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:42:23.987842 gravitino-0.5.0.dev5/gravitino/client/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev5/gravitino/client/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)     4651 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/client/gravitino_admin_client.py
--rw-r--r--   0 xun        (501) staff       (20)     2739 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/client/gravitino_client.py
--rw-r--r--   0 xun        (501) staff       (20)     2483 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/client/gravitino_client_base.py
--rw-r--r--   0 xun        (501) staff       (20)     7664 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/client/gravitino_metalake.py
--rw-r--r--   0 xun        (501) staff       (20)      408 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev5/gravitino/client/gravitino_version.py
--rw-r--r--   0 xun        (501) staff       (20)      119 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev5/gravitino/constants.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:42:23.990659 gravitino-0.5.0.dev5/gravitino/dto/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev5/gravitino/dto/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)     1753 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev5/gravitino/dto/audit_dto.py
--rw-r--r--   0 xun        (501) staff       (20)     1590 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev5/gravitino/dto/catalog_dto.py
--rw-r--r--   0 xun        (501) staff       (20)     3019 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/dto/dto_converters.py
--rw-r--r--   0 xun        (501) staff       (20)     1313 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/dto/fileset_dto.py
--rw-r--r--   0 xun        (501) staff       (20)     1883 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/dto/metalake_dto.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:42:23.992785 gravitino-0.5.0.dev5/gravitino/dto/requests/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev5/gravitino/dto/requests/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)     1560 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/dto/requests/catalog_create_request.py
--rw-r--r--   0 xun        (501) staff       (20)     2534 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/dto/requests/catalog_update_request.py
--rw-r--r--   0 xun        (501) staff       (20)     1065 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/dto/requests/catalog_updates_request.py
--rw-r--r--   0 xun        (501) staff       (20)     1438 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/dto/requests/fileset_create_request.py
--rw-r--r--   0 xun        (501) staff       (20)     4267 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/dto/requests/fileset_update_request.py
--rw-r--r--   0 xun        (501) staff       (20)      750 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/dto/requests/fileset_updates_request.py
--rw-r--r--   0 xun        (501) staff       (20)     1070 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/dto/requests/metalake_create_request.py
--rw-r--r--   0 xun        (501) staff       (20)     4145 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/dto/requests/metalake_update_request.py
--rw-r--r--   0 xun        (501) staff       (20)     1029 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/dto/requests/metalake_updates_request.py
--rw-r--r--   0 xun        (501) staff       (20)      908 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/dto/requests/schema_create_request.py
--rw-r--r--   0 xun        (501) staff       (20)     2519 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/dto/requests/schema_update_request.py
--rw-r--r--   0 xun        (501) staff       (20)      990 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/dto/requests/schema_updates_request.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:42:23.994679 gravitino-0.5.0.dev5/gravitino/dto/responses/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev5/gravitino/dto/responses/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)      683 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/dto/responses/base_response.py
--rw-r--r--   0 xun        (501) staff       (20)      573 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/dto/responses/catalog_list_response.py
--rw-r--r--   0 xun        (501) staff       (20)     1051 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev5/gravitino/dto/responses/catalog_response.py
--rw-r--r--   0 xun        (501) staff       (20)      476 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev5/gravitino/dto/responses/drop_response.py
--rw-r--r--   0 xun        (501) staff       (20)      871 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/dto/responses/entity_list_response.py
--rw-r--r--   0 xun        (501) staff       (20)     1061 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/dto/responses/fileset_response.py
--rw-r--r--   0 xun        (501) staff       (20)     1162 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/dto/responses/metalake_list_response.py
--rw-r--r--   0 xun        (501) staff       (20)     1063 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/dto/responses/metalake_response.py
--rw-r--r--   0 xun        (501) staff       (20)     1058 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/dto/responses/schema_response.py
--rw-r--r--   0 xun        (501) staff       (20)     1382 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/dto/schema_dto.py
--rw-r--r--   0 xun        (501) staff       (20)      431 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev5/gravitino/dto/version_dto.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:42:23.995609 gravitino-0.5.0.dev5/gravitino/exceptions/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev5/gravitino/exceptions/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)      302 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/exceptions/gravitino_runtime_exception.py
--rw-r--r--   0 xun        (501) staff       (20)      363 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/exceptions/illegal_name_identifier_exception.py
--rw-r--r--   0 xun        (501) staff       (20)      352 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/exceptions/illegal_namespace_exception.py
--rw-r--r--   0 xun        (501) staff       (20)      288 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/exceptions/no_such_metalake_exception.py
--rw-r--r--   0 xun        (501) staff       (20)      323 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/exceptions/not_found_exception.py
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev5/gravitino/exceptions.py
--rw-r--r--   0 xun        (501) staff       (20)     4404 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev5/gravitino/gravitino_client.py
--rw-r--r--   0 xun        (501) staff       (20)     9268 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/name_identifier.py
--rw-r--r--   0 xun        (501) staff       (20)     7603 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/namespace.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:42:23.995986 gravitino-0.5.0.dev5/gravitino/rest/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev5/gravitino/rest/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)     1198 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev5/gravitino/rest/rest_message.py
--rw-r--r--   0 xun        (501) staff       (20)     2430 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev5/gravitino/service.py
--rw-r--r--   0 xun        (501) staff       (20)      318 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev5/gravitino/typing.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:42:23.996636 gravitino-0.5.0.dev5/gravitino/utils/
--rw-r--r--   0 xun        (501) staff       (20)      175 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev5/gravitino/utils/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)     2692 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/utils/exceptions.py
--rw-r--r--   0 xun        (501) staff       (20)     5479 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/gravitino/utils/http_client.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:42:23.982342 gravitino-0.5.0.dev5/gravitino.egg-info/
--rw-r--r--   0 xun        (501) staff       (20)     3774 2024-05-04 02:42:23.000000 gravitino-0.5.0.dev5/gravitino.egg-info/PKG-INFO
--rw-r--r--   0 xun        (501) staff       (20)     3047 2024-05-04 02:42:23.000000 gravitino-0.5.0.dev5/gravitino.egg-info/SOURCES.txt
--rw-r--r--   0 xun        (501) staff       (20)        1 2024-05-04 02:42:23.000000 gravitino-0.5.0.dev5/gravitino.egg-info/dependency_links.txt
--rw-r--r--   0 xun        (501) staff       (20)       72 2024-05-04 02:42:23.000000 gravitino-0.5.0.dev5/gravitino.egg-info/requires.txt
--rw-r--r--   0 xun        (501) staff       (20)       16 2024-05-04 02:42:23.000000 gravitino-0.5.0.dev5/gravitino.egg-info/top_level.txt
--rw-r--r--   0 xun        (501) staff       (20)       38 2024-05-04 02:42:23.999468 gravitino-0.5.0.dev5/setup.cfg
--rw-r--r--   0 xun        (501) staff       (20)      627 2024-05-04 02:42:18.000000 gravitino-0.5.0.dev5/setup.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:42:23.997770 gravitino-0.5.0.dev5/tests/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev5/tests/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)     3607 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev5/tests/fixtures.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:42:23.998937 gravitino-0.5.0.dev5/tests/integration/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev5/tests/integration/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)     3768 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/tests/integration/integration_test_env.py
--rw-r--r--   0 xun        (501) staff       (20)     7086 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/tests/integration/test_fileset_catalog.py
--rw-r--r--   0 xun        (501) staff       (20)     6653 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/tests/integration/test_metalake.py
--rw-r--r--   0 xun        (501) staff       (20)     6058 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev5/tests/integration/test_schema.py
--rw-r--r--   0 xun        (501) staff       (20)     2175 2024-04-13 14:55:38.000000 gravitino-0.5.0.dev5/tests/test_gravitino_client.py
--rw-r--r--   0 xun        (501) staff       (20)     1323 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev5/tests/utils.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-05 07:14:17.268108 gravitino-0.5.0.dev6/
+-rw-r--r--   0 xun        (501) staff       (20)     4397 2024-05-05 07:14:17.267849 gravitino-0.5.0.dev6/PKG-INFO
+-rw-r--r--   0 xun        (501) staff       (20)     3484 2024-05-04 02:43:48.000000 gravitino-0.5.0.dev6/README.md
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-05 07:14:17.248032 gravitino-0.5.0.dev6/gravitino/
+-rw-r--r--   0 xun        (501) staff       (20)      648 2024-05-05 07:11:52.000000 gravitino-0.5.0.dev6/gravitino/__init__.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-05 07:14:17.252548 gravitino-0.5.0.dev6/gravitino/api/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev6/gravitino/api/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)      942 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev6/gravitino/api/audit.py
+-rw-r--r--   0 xun        (501) staff       (20)      440 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev6/gravitino/api/auditable.py
+-rw-r--r--   0 xun        (501) staff       (20)     4113 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev6/gravitino/api/catalog.py
+-rw-r--r--   0 xun        (501) staff       (20)     8759 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/api/catalog_change.py
+-rw-r--r--   0 xun        (501) staff       (20)     3556 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/api/fileset.py
+-rw-r--r--   0 xun        (501) staff       (20)     9226 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/api/fileset_change.py
+-rw-r--r--   0 xun        (501) staff       (20)     1155 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/api/metalake.py
+-rw-r--r--   0 xun        (501) staff       (20)     3403 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/api/metalake_change.py
+-rw-r--r--   0 xun        (501) staff       (20)     1044 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/api/schema.py
+-rw-r--r--   0 xun        (501) staff       (20)     4847 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/api/schema_change.py
+-rw-r--r--   0 xun        (501) staff       (20)     3870 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/api/supports_schemas.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-05 07:14:17.253355 gravitino-0.5.0.dev6/gravitino/catalog/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev6/gravitino/catalog/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     7055 2024-05-05 07:09:37.000000 gravitino-0.5.0.dev6/gravitino/catalog/base_schema_catalog.py
+-rw-r--r--   0 xun        (501) staff       (20)     7323 2024-05-05 07:10:44.000000 gravitino-0.5.0.dev6/gravitino/catalog/fileset_catalog.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-05 07:14:17.255264 gravitino-0.5.0.dev6/gravitino/client/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev6/gravitino/client/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     4651 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/client/gravitino_admin_client.py
+-rw-r--r--   0 xun        (501) staff       (20)     2739 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/client/gravitino_client.py
+-rw-r--r--   0 xun        (501) staff       (20)     2483 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/client/gravitino_client_base.py
+-rw-r--r--   0 xun        (501) staff       (20)     7664 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/client/gravitino_metalake.py
+-rw-r--r--   0 xun        (501) staff       (20)      408 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev6/gravitino/client/gravitino_version.py
+-rw-r--r--   0 xun        (501) staff       (20)      119 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev6/gravitino/constants.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-05 07:14:17.257384 gravitino-0.5.0.dev6/gravitino/dto/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev6/gravitino/dto/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     1753 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev6/gravitino/dto/audit_dto.py
+-rw-r--r--   0 xun        (501) staff       (20)     1590 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev6/gravitino/dto/catalog_dto.py
+-rw-r--r--   0 xun        (501) staff       (20)     3019 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/dto/dto_converters.py
+-rw-r--r--   0 xun        (501) staff       (20)     1313 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/dto/fileset_dto.py
+-rw-r--r--   0 xun        (501) staff       (20)     1883 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/dto/metalake_dto.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-05 07:14:17.259971 gravitino-0.5.0.dev6/gravitino/dto/requests/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev6/gravitino/dto/requests/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     1560 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/dto/requests/catalog_create_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     2534 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/dto/requests/catalog_update_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     1065 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/dto/requests/catalog_updates_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     1438 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/dto/requests/fileset_create_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     4267 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/dto/requests/fileset_update_request.py
+-rw-r--r--   0 xun        (501) staff       (20)      750 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/dto/requests/fileset_updates_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     1070 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/dto/requests/metalake_create_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     4145 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/dto/requests/metalake_update_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     1029 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/dto/requests/metalake_updates_request.py
+-rw-r--r--   0 xun        (501) staff       (20)      908 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/dto/requests/schema_create_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     2519 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/dto/requests/schema_update_request.py
+-rw-r--r--   0 xun        (501) staff       (20)      990 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/dto/requests/schema_updates_request.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-05 07:14:17.262083 gravitino-0.5.0.dev6/gravitino/dto/responses/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev6/gravitino/dto/responses/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)      683 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/dto/responses/base_response.py
+-rw-r--r--   0 xun        (501) staff       (20)      573 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/dto/responses/catalog_list_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1051 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev6/gravitino/dto/responses/catalog_response.py
+-rw-r--r--   0 xun        (501) staff       (20)      476 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev6/gravitino/dto/responses/drop_response.py
+-rw-r--r--   0 xun        (501) staff       (20)      871 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/dto/responses/entity_list_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1061 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/dto/responses/fileset_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1162 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/dto/responses/metalake_list_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1063 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/dto/responses/metalake_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1058 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/dto/responses/schema_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1382 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/dto/schema_dto.py
+-rw-r--r--   0 xun        (501) staff       (20)      431 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev6/gravitino/dto/version_dto.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-05 07:14:17.263208 gravitino-0.5.0.dev6/gravitino/exceptions/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev6/gravitino/exceptions/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)      302 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/exceptions/gravitino_runtime_exception.py
+-rw-r--r--   0 xun        (501) staff       (20)      363 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/exceptions/illegal_name_identifier_exception.py
+-rw-r--r--   0 xun        (501) staff       (20)      352 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/exceptions/illegal_namespace_exception.py
+-rw-r--r--   0 xun        (501) staff       (20)      288 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/exceptions/no_such_metalake_exception.py
+-rw-r--r--   0 xun        (501) staff       (20)      323 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/exceptions/not_found_exception.py
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev6/gravitino/exceptions.py
+-rw-r--r--   0 xun        (501) staff       (20)     4404 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev6/gravitino/gravitino_client.py
+-rw-r--r--   0 xun        (501) staff       (20)     9268 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/name_identifier.py
+-rw-r--r--   0 xun        (501) staff       (20)     7603 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/namespace.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-05 07:14:17.263680 gravitino-0.5.0.dev6/gravitino/rest/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev6/gravitino/rest/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     1198 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev6/gravitino/rest/rest_message.py
+-rw-r--r--   0 xun        (501) staff       (20)     2430 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev6/gravitino/service.py
+-rw-r--r--   0 xun        (501) staff       (20)      318 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev6/gravitino/typing.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-05 07:14:17.264410 gravitino-0.5.0.dev6/gravitino/utils/
+-rw-r--r--   0 xun        (501) staff       (20)      175 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev6/gravitino/utils/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     2692 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/utils/exceptions.py
+-rw-r--r--   0 xun        (501) staff       (20)     5479 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/gravitino/utils/http_client.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-05 07:14:17.248828 gravitino-0.5.0.dev6/gravitino.egg-info/
+-rw-r--r--   0 xun        (501) staff       (20)     4397 2024-05-05 07:14:17.000000 gravitino-0.5.0.dev6/gravitino.egg-info/PKG-INFO
+-rw-r--r--   0 xun        (501) staff       (20)     3047 2024-05-05 07:14:17.000000 gravitino-0.5.0.dev6/gravitino.egg-info/SOURCES.txt
+-rw-r--r--   0 xun        (501) staff       (20)        1 2024-05-05 07:14:17.000000 gravitino-0.5.0.dev6/gravitino.egg-info/dependency_links.txt
+-rw-r--r--   0 xun        (501) staff       (20)       72 2024-05-05 07:14:17.000000 gravitino-0.5.0.dev6/gravitino.egg-info/requires.txt
+-rw-r--r--   0 xun        (501) staff       (20)       16 2024-05-05 07:14:17.000000 gravitino-0.5.0.dev6/gravitino.egg-info/top_level.txt
+-rw-r--r--   0 xun        (501) staff       (20)       38 2024-05-05 07:14:17.268163 gravitino-0.5.0.dev6/setup.cfg
+-rw-r--r--   0 xun        (501) staff       (20)     1108 2024-05-05 07:13:17.000000 gravitino-0.5.0.dev6/setup.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-05 07:14:17.265537 gravitino-0.5.0.dev6/tests/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev6/tests/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     3607 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev6/tests/fixtures.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-05 07:14:17.266863 gravitino-0.5.0.dev6/tests/integration/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev6/tests/integration/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     3768 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev6/tests/integration/integration_test_env.py
+-rw-r--r--   0 xun        (501) staff       (20)     7189 2024-05-05 00:25:38.000000 gravitino-0.5.0.dev6/tests/integration/test_fileset_catalog.py
+-rw-r--r--   0 xun        (501) staff       (20)     6498 2024-05-05 00:28:28.000000 gravitino-0.5.0.dev6/tests/integration/test_metalake.py
+-rw-r--r--   0 xun        (501) staff       (20)     5843 2024-05-05 07:12:19.000000 gravitino-0.5.0.dev6/tests/integration/test_schema.py
+-rw-r--r--   0 xun        (501) staff       (20)     2192 2024-05-05 00:35:45.000000 gravitino-0.5.0.dev6/tests/test_gravitino_client.py
+-rw-r--r--   0 xun        (501) staff       (20)     1323 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev6/tests/utils.py
```

### Comparing `gravitino-0.5.0.dev5/PKG-INFO` & `gravitino-0.5.0.dev6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: gravitino
-Version: 0.5.0.dev5
-Summary: Python lib/client for Gravitino
-Home-page: https://github.com/datastrato/gravitino
-Author: datastrato
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
 <!-- 
 - Copyright 2024 Datastrato Pvt Ltd.
 - This software is licensed under the Apache License version 2. 
 -->
 [![License](https://img.shields.io/github/license/datastrato/gravitino)](https://github.com/datastrato/gravitino/blob/main/LICENSE)
 
 ## Introduction
@@ -55,15 +43,15 @@
 pip install requests dataclasses-json gravitino
 ```
 
 
 ```python
 import gravitino
 
-gravitino_admin_client = GravitinoAdminClient(uri="http://localhost:8090")
+gravitino_admin_client = GravitinoAdminClient(uri="http://gravitino:8090")
 metalake = gravitino_admin_client.create_metalake(
     ident=NameIdentifier.of("default"),
     comment="metalake comment", properties={})
 
 catalog = gravitino_client.create_catalog(
             ident=NameIdentifier.of("default", "testCatalog"),
             type=CatalogDTO.Type.FILESET,
@@ -116,9 +104,7 @@
 + Playground with Docker: https://github.com/datastrato/gravitino-playground
 + User documentation: https://datastrato.ai/docs/
 + Videos on Youtube: https://www.youtube.com/@Datastrato
 + Twitter: https://twitter.com/datastrato
 + Linkedin: https://www.linkedin.com/company/datastrato
 + Slack Community: [https://join.slack.com/t/datastrato-community](https://join.slack.com/t/datastrato-community/shared_invite/zt-2a8vsjoch-cU_uUwHA_QU6Ab50thoq8w)
 + Discourse Community: https://gravitino.discourse.group/
-
-
```

### Comparing `gravitino-0.5.0.dev5/README.md` & `gravitino-0.5.0.dev6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: gravitino
+Version: 0.5.0.dev6
+Summary: Python lib/client for Gravitino
+Home-page: https://github.com/datastrato/gravitino
+Author: datastrato
+Author-email: support@datastrato.com
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Requires-Dist: requests
+Requires-Dist: dataclasses-json
+Provides-Extra: dev
+Requires-Dist: requests; extra == "dev"
+Requires-Dist: dataclasses-json; extra == "dev"
+Requires-Dist: pylint; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+
 <!-- 
 - Copyright 2024 Datastrato Pvt Ltd.
 - This software is licensed under the Apache License version 2. 
 -->
 [![License](https://img.shields.io/github/license/datastrato/gravitino)](https://github.com/datastrato/gravitino/blob/main/LICENSE)
 
 ## Introduction
@@ -43,15 +68,15 @@
 pip install requests dataclasses-json gravitino
 ```
 
 
 ```python
 import gravitino
 
-gravitino_admin_client = GravitinoAdminClient(uri="http://localhost:8090")
+gravitino_admin_client = GravitinoAdminClient(uri="http://gravitino:8090")
 metalake = gravitino_admin_client.create_metalake(
     ident=NameIdentifier.of("default"),
     comment="metalake comment", properties={})
 
 catalog = gravitino_client.create_catalog(
             ident=NameIdentifier.of("default", "testCatalog"),
             type=CatalogDTO.Type.FILESET,
```

### Comparing `gravitino-0.5.0.dev5/gravitino/api/audit.py` & `gravitino-0.5.0.dev6/gravitino/api/audit.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/api/catalog.py` & `gravitino-0.5.0.dev6/gravitino/api/catalog.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/api/catalog_change.py` & `gravitino-0.5.0.dev6/gravitino/api/catalog_change.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/api/fileset.py` & `gravitino-0.5.0.dev6/gravitino/api/fileset.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/api/fileset_change.py` & `gravitino-0.5.0.dev6/gravitino/api/fileset_change.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/api/metalake.py` & `gravitino-0.5.0.dev6/gravitino/api/metalake.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/api/metalake_change.py` & `gravitino-0.5.0.dev6/gravitino/api/metalake_change.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/api/schema.py` & `gravitino-0.5.0.dev6/gravitino/api/schema.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/api/schema_change.py` & `gravitino-0.5.0.dev6/gravitino/api/schema_change.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/api/supports_schemas.py` & `gravitino-0.5.0.dev6/gravitino/api/supports_schemas.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/catalog/base_schema_catalog.py` & `gravitino-0.5.0.dev6/gravitino/catalog/base_schema_catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,23 +147,22 @@
         try:
             params = {"cascade": str(cascade)}
             resp = self.rest_client.delete(
                 BaseSchemaCatalog.format_schema_request_path(ident.namespace()) + "/" + ident.name(), params=params)
             drop_resp = DropResponse.from_json(resp.body, infer_missing=True)
             drop_resp.validate()
             return drop_resp.dropped()
-        except Exception as e:
-            logger.warning(f"Failed to drop schema {ident}")
+        except Exception:
+            logger.warning("Failed to drop schema %s", ident)
             return False
 
     @staticmethod
     def format_schema_request_path(ns: Namespace):
         return "api/metalakes/" + ns.level(0) + "/catalogs/" + ns.level(1) + "/schemas"
 
     @staticmethod
     def to_schema_update_request(change: SchemaChange):
         if isinstance(change, SchemaChange.SetProperty):
             return SchemaUpdateRequest.SetSchemaPropertyRequest(change.property(), change.value())
-        elif isinstance(change, SchemaChange.RemoveProperty):
+        if isinstance(change, SchemaChange.RemoveProperty):
             return SchemaUpdateRequest.RemoveSchemaPropertyRequest(change.property())
-        else:
-            raise ValueError(f"Unknown change type: {type(change).__name__}")
+        raise ValueError(f"Unknown change type: {type(change).__name__}")
```

### Comparing `gravitino-0.5.0.dev5/gravitino/catalog/fileset_catalog.py` & `gravitino-0.5.0.dev6/gravitino/catalog/fileset_catalog.py`

 * *Files 4% similar despite different names*

```diff
@@ -159,27 +159,26 @@
                 f"{self.format_fileset_request_path(ident.namespace())}/{ident.name()}",
             )
             drop_resp = DropResponse.from_json(resp.body, infer_missing=True)
             drop_resp.validate()
 
             return drop_resp.dropped()
         except Exception as e:
-            logger.warning(f"Failed to drop fileset {ident}: {e}")
+            logger.warning("Failed to drop fileset %s: %s", ident, e)
             return False
 
     @staticmethod
     def format_fileset_request_path(namespace: Namespace) -> str:
         schema_ns = Namespace.of(namespace.level(0), namespace.level(1))
         return f"{BaseSchemaCatalog.format_schema_request_path(schema_ns)}/{namespace.level(2)}/filesets"
 
     @staticmethod
     def to_fileset_update_request(change: FilesetChange):
         if isinstance(change, FilesetChange.RenameFileset):
             return FilesetUpdateRequest.RenameFilesetRequest(change.new_name())
-        elif isinstance(change, FilesetChange.UpdateFilesetComment):
+        if isinstance(change, FilesetChange.UpdateFilesetComment):
             return FilesetUpdateRequest.UpdateFilesetCommentRequest(change.new_comment())
-        elif isinstance(change, FilesetChange.SetProperty):
+        if isinstance(change, FilesetChange.SetProperty):
             return FilesetUpdateRequest.SetFilesetPropertyRequest(change.property(), change.value())
-        elif isinstance(change, FilesetChange.RemoveProperty):
+        if isinstance(change, FilesetChange.RemoveProperty):
             return FilesetUpdateRequest.RemoveFilesetPropertyRequest(change.property())
-        else:
-            raise ValueError(f"Unknown change type: {type(change).__name__}")
+        raise ValueError(f"Unknown change type: {type(change).__name__}")
```

### Comparing `gravitino-0.5.0.dev5/gravitino/client/gravitino_admin_client.py` & `gravitino-0.5.0.dev6/gravitino/client/gravitino_admin_client.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/client/gravitino_client.py` & `gravitino-0.5.0.dev6/gravitino/client/gravitino_client.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/client/gravitino_client_base.py` & `gravitino-0.5.0.dev6/gravitino/client/gravitino_client_base.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/client/gravitino_metalake.py` & `gravitino-0.5.0.dev6/gravitino/client/gravitino_metalake.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/dto/audit_dto.py` & `gravitino-0.5.0.dev6/gravitino/dto/audit_dto.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/dto/catalog_dto.py` & `gravitino-0.5.0.dev6/gravitino/dto/catalog_dto.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/dto/dto_converters.py` & `gravitino-0.5.0.dev6/gravitino/dto/dto_converters.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/dto/fileset_dto.py` & `gravitino-0.5.0.dev6/gravitino/dto/fileset_dto.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/dto/metalake_dto.py` & `gravitino-0.5.0.dev6/gravitino/dto/metalake_dto.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/dto/requests/catalog_create_request.py` & `gravitino-0.5.0.dev6/gravitino/dto/requests/catalog_create_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/dto/requests/catalog_update_request.py` & `gravitino-0.5.0.dev6/gravitino/dto/requests/catalog_update_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/dto/requests/catalog_updates_request.py` & `gravitino-0.5.0.dev6/gravitino/dto/requests/catalog_updates_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/dto/requests/fileset_create_request.py` & `gravitino-0.5.0.dev6/gravitino/dto/requests/fileset_create_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/dto/requests/fileset_update_request.py` & `gravitino-0.5.0.dev6/gravitino/dto/requests/fileset_update_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/dto/requests/fileset_updates_request.py` & `gravitino-0.5.0.dev6/gravitino/dto/requests/fileset_updates_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/dto/requests/metalake_create_request.py` & `gravitino-0.5.0.dev6/gravitino/dto/requests/metalake_create_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/dto/requests/metalake_update_request.py` & `gravitino-0.5.0.dev6/gravitino/dto/requests/metalake_update_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/dto/requests/metalake_updates_request.py` & `gravitino-0.5.0.dev6/gravitino/dto/requests/metalake_updates_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/dto/requests/schema_create_request.py` & `gravitino-0.5.0.dev6/gravitino/dto/requests/schema_create_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/dto/requests/schema_update_request.py` & `gravitino-0.5.0.dev6/gravitino/dto/requests/schema_update_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/dto/requests/schema_updates_request.py` & `gravitino-0.5.0.dev6/gravitino/dto/requests/schema_updates_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/dto/responses/base_response.py` & `gravitino-0.5.0.dev6/gravitino/dto/responses/base_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/dto/responses/catalog_list_response.py` & `gravitino-0.5.0.dev6/gravitino/dto/responses/catalog_list_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/dto/responses/catalog_response.py` & `gravitino-0.5.0.dev6/gravitino/dto/responses/catalog_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/dto/responses/entity_list_response.py` & `gravitino-0.5.0.dev6/gravitino/dto/responses/entity_list_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/dto/responses/fileset_response.py` & `gravitino-0.5.0.dev6/gravitino/dto/responses/fileset_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/dto/responses/metalake_list_response.py` & `gravitino-0.5.0.dev6/gravitino/dto/responses/metalake_list_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/dto/responses/metalake_response.py` & `gravitino-0.5.0.dev6/gravitino/dto/responses/metalake_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/dto/responses/schema_response.py` & `gravitino-0.5.0.dev6/gravitino/dto/responses/schema_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/dto/schema_dto.py` & `gravitino-0.5.0.dev6/gravitino/dto/schema_dto.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/gravitino_client.py` & `gravitino-0.5.0.dev6/gravitino/gravitino_client.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/name_identifier.py` & `gravitino-0.5.0.dev6/gravitino/name_identifier.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/namespace.py` & `gravitino-0.5.0.dev6/gravitino/namespace.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/rest/rest_message.py` & `gravitino-0.5.0.dev6/gravitino/rest/rest_message.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/service.py` & `gravitino-0.5.0.dev6/gravitino/service.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/utils/exceptions.py` & `gravitino-0.5.0.dev6/gravitino/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino/utils/http_client.py` & `gravitino-0.5.0.dev6/gravitino/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/gravitino.egg-info/PKG-INFO` & `gravitino-0.5.0.dev6/gravitino.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,31 @@
 Metadata-Version: 2.1
 Name: gravitino
-Version: 0.5.0.dev5
+Version: 0.5.0.dev6
 Summary: Python lib/client for Gravitino
 Home-page: https://github.com/datastrato/gravitino
 Author: datastrato
-License: UNKNOWN
-Platform: UNKNOWN
+Author-email: support@datastrato.com
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Requires-Dist: requests
+Requires-Dist: dataclasses-json
 Provides-Extra: dev
+Requires-Dist: requests; extra == "dev"
+Requires-Dist: dataclasses-json; extra == "dev"
+Requires-Dist: pylint; extra == "dev"
+Requires-Dist: twine; extra == "dev"
 
 <!-- 
 - Copyright 2024 Datastrato Pvt Ltd.
 - This software is licensed under the Apache License version 2. 
 -->
 [![License](https://img.shields.io/github/license/datastrato/gravitino)](https://github.com/datastrato/gravitino/blob/main/LICENSE)
 
@@ -55,15 +68,15 @@
 pip install requests dataclasses-json gravitino
 ```
 
 
 ```python
 import gravitino
 
-gravitino_admin_client = GravitinoAdminClient(uri="http://localhost:8090")
+gravitino_admin_client = GravitinoAdminClient(uri="http://gravitino:8090")
 metalake = gravitino_admin_client.create_metalake(
     ident=NameIdentifier.of("default"),
     comment="metalake comment", properties={})
 
 catalog = gravitino_client.create_catalog(
             ident=NameIdentifier.of("default", "testCatalog"),
             type=CatalogDTO.Type.FILESET,
@@ -116,9 +129,7 @@
 + Playground with Docker: https://github.com/datastrato/gravitino-playground
 + User documentation: https://datastrato.ai/docs/
 + Videos on Youtube: https://www.youtube.com/@Datastrato
 + Twitter: https://twitter.com/datastrato
 + Linkedin: https://www.linkedin.com/company/datastrato
 + Slack Community: [https://join.slack.com/t/datastrato-community](https://join.slack.com/t/datastrato-community/shared_invite/zt-2a8vsjoch-cU_uUwHA_QU6Ab50thoq8w)
 + Discourse Community: https://gravitino.discourse.group/
-
-
```

### Comparing `gravitino-0.5.0.dev5/gravitino.egg-info/SOURCES.txt` & `gravitino-0.5.0.dev6/gravitino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/tests/fixtures.py` & `gravitino-0.5.0.dev6/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/tests/integration/integration_test_env.py` & `gravitino-0.5.0.dev6/tests/integration/integration_test_env.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev5/tests/integration/test_fileset_catalog.py` & `gravitino-0.5.0.dev6/tests/integration/test_fileset_catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,30 @@
 Copyright 2024 Datastrato Pvt Ltd.
 This software is licensed under the Apache License version 2.
 """
 import logging
 from random import randint
 from typing import Dict, List
 
-from gravitino.api.fileset import Fileset
-from gravitino.api.fileset_change import FilesetChange
-from gravitino.client.gravitino_admin_client import GravitinoAdminClient
-from gravitino.client.gravitino_client import GravitinoClient
-from gravitino.dto.catalog_dto import CatalogDTO
-from gravitino.name_identifier import NameIdentifier
+from gravitino import NameIdentifier, GravitinoAdminClient, GravitinoClient, Catalog, Fileset, FilesetChange
+# from gravitino.api.catalog import Catalog
+# from gravitino.api.fileset import Fileset
+# from gravitino.api.fileset_change import FilesetChange
+# from gravitino.client.gravitino_admin_client import GravitinoAdminClient
+# from gravitino.client.gravitino_client import GravitinoClient
+# from gravitino.name_identifier import NameIdentifier
 from tests.integration.integration_test_env import IntegrationTestEnv
 
 logger = logging.getLogger(__name__)
 
 
 class TestFilesetCatalog(IntegrationTestEnv):
     metalake_name: str = "TestFilesetCatalog-metalake" + str(randint(1, 10000))
     catalog_name: str = "catalog"
-    catalog_location_pcatarop: str = "location"  # Fileset Catalog must set `location`
+    catalog_location_prop: str = "location"  # Fileset Catalog must set `location`
     catalog_provider: str = "hadoop"
 
     schema_name: str = "schema"
 
     fileset_name: str = "fileset"
     fileset_alter_name: str = fileset_name + "Alter"
     fileset_comment: str = "fileset_comment"
@@ -71,17 +72,17 @@
         except Exception as e:
             logger.error("Clean test data failed: %s", e)
 
     def init_test_env(self):
         self.gravitino_admin_client.create_metalake(ident=self.metalake_ident, comment="", properties={})
         self.gravitino_client = GravitinoClient(uri="http://localhost:8090", metalake_name=self.metalake_name)
         catalog = self.gravitino_client.create_catalog(ident=self.catalog_ident,
-                                                       type=CatalogDTO.Type.FILESET,
+                                                       type=Catalog.Type.FILESET,
                                                        provider=self.catalog_provider, comment="",
-                                                       properties={self.catalog_location_pcatarop: "/tmp/test1"})
+                                                       properties={self.catalog_location_prop: "/tmp/test1"})
         catalog.as_schemas().create_schema(ident=self.schema_ident, comment="", properties={})
 
     def create_fileset(self) -> Fileset:
         catalog = self.gravitino_client.load_catalog(ident=self.catalog_ident)
         return (catalog.as_fileset_catalog().create_fileset(ident=self.fileset_ident,
                                                             type=Fileset.Type.MANAGED,
                                                             comment=self.fileset_comment,
```

### Comparing `gravitino-0.5.0.dev5/tests/integration/test_metalake.py` & `gravitino-0.5.0.dev6/tests/integration/test_metalake.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 """
 Copyright 2024 Datastrato Pvt Ltd.
 This software is licensed under the Apache License version 2.
 """
 import logging
 from typing import Dict, List
 
-from gravitino.client.gravitino_admin_client import GravitinoAdminClient
-from gravitino.client.gravitino_metalake import GravitinoMetalake
+from gravitino import GravitinoAdminClient, GravitinoMetalake, MetalakeChange, NameIdentifier
 from gravitino.dto.dto_converters import DTOConverters
 from gravitino.dto.requests.metalake_updates_request import MetalakeUpdatesRequest
 from gravitino.dto.responses.metalake_response import MetalakeResponse
-from gravitino.api.metalake_change import MetalakeChange
-from gravitino.name_identifier import NameIdentifier
 from tests.integration.integration_test_env import IntegrationTestEnv
 
 logger = logging.getLogger(__name__)
 
 
 class TestMetalake(IntegrationTestEnv):
     metalake_name: str = "TestMetalake-metalake"
```

### Comparing `gravitino-0.5.0.dev5/tests/integration/test_schema.py` & `gravitino-0.5.0.dev6/tests/integration/test_schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,20 +2,16 @@
 Copyright 2024 Datastrato Pvt Ltd.
 This software is licensed under the Apache License version 2.
 """
 import logging
 from random import randint
 from typing import Dict, List
 
-from gravitino.api.catalog import Catalog
-from gravitino.api.schema import Schema
-from gravitino.api.schema_change import SchemaChange
-from gravitino.client.gravitino_admin_client import GravitinoAdminClient
-from gravitino.client.gravitino_client import GravitinoClient
-from gravitino.name_identifier import NameIdentifier
+from gravitino import NameIdentifier, GravitinoAdminClient, GravitinoClient, Catalog, SchemaChange, Schema
+
 from tests.integration.integration_test_env import IntegrationTestEnv
 
 logger = logging.getLogger(__name__)
 
 
 class TestSchema(IntegrationTestEnv):
     metalake_name: str = "TestSchema-metalake" + str(randint(1, 10000))
```

### Comparing `gravitino-0.5.0.dev5/tests/test_gravitino_client.py` & `gravitino-0.5.0.dev6/tests/test_gravitino_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Copyright 2024 Datastrato Pvt Ltd.
 This software is licensed under the Apache License version 2.
 """
 
 import unittest
 
-from gravitino import GravitinoClient, gravitino_metalake
+from gravitino.gravitino_client import gravitino_metalake, GravitinoClient
 from .utils import services_fixtures
 
 
 @services_fixtures
 class TestGravitinoClient(unittest.TestCase):
     def setUp(self):
         self.client = GravitinoClient("http://localhost:9000")
```

### Comparing `gravitino-0.5.0.dev5/tests/utils.py` & `gravitino-0.5.0.dev6/tests/utils.py`

 * *Files identical despite different names*

