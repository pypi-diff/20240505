# Comparing `tmp/heaserver-1.5.2.tar.gz` & `tmp/heaserver-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-1.5.2.tar", last modified: Fri May  3 22:08:46 2024, max compression
+gzip compressed data, was "heaserver-1.5.3.tar", last modified: Sun May  5 18:18:09 2024, max compression
```

## Comparing `heaserver-1.5.2.tar` & `heaserver-1.5.3.tar`

### file list

```diff
@@ -1,299 +1,299 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 22:08:46.510014 heaserver-1.5.2/
--rw-rw-rw-   0        0        0      261 2022-03-11 01:28:19.000000 heaserver-1.5.2/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-12-16 23:04:09.000000 heaserver-1.5.2/.gitignore
--rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:19.000000 heaserver-1.5.2/LICENSE
--rw-rw-rw-   0        0        0      243 2023-12-16 23:04:09.000000 heaserver-1.5.2/MANIFEST.in
--rw-rw-rw-   0        0        0     7629 2024-05-03 22:08:46.508450 heaserver-1.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     5634 2024-05-03 22:07:51.000000 heaserver-1.5.2/README.md
--rw-rw-rw-   0        0        0     1612 2023-12-16 23:04:09.000000 heaserver-1.5.2/RELEASING.md
-drwxrwxrwx   0        0        0        0 2024-05-03 22:08:46.024183 heaserver-1.5.2/awss3integrationtests/
-drwxrwxrwx   0        0        0        0 2024-05-03 22:08:46.024695 heaserver-1.5.2/awss3integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-03 22:08:46.053423 heaserver-1.5.2/awss3integrationtests/heaserver/awss3tests/
--rw-rw-rw-   0        0        0        0 2023-12-16 23:04:09.000000 heaserver-1.5.2/awss3integrationtests/heaserver/awss3tests/__init__.py
--rw-rw-rw-   0        0        0    34976 2024-04-01 23:40:09.000000 heaserver-1.5.2/awss3integrationtests/heaserver/awss3tests/awss3foldertestcase.py
--rw-rw-rw-   0        0        0     1416 2023-12-16 23:04:09.000000 heaserver-1.5.2/awss3integrationtests/heaserver/awss3tests/service.py
--rw-rw-rw-   0        0        0    19401 2024-04-08 18:06:35.000000 heaserver-1.5.2/awss3integrationtests/heaserver/awss3tests/test_all.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:08:46.054982 heaserver-1.5.2/awss3integrationtests/heaserver/awss3tests/wstl/
--rw-rw-rw-   0        0        0    16955 2023-12-16 23:04:09.000000 heaserver-1.5.2/awss3integrationtests/heaserver/awss3tests/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-05-03 22:08:46.026245 heaserver-1.5.2/awss3tests/
-drwxrwxrwx   0        0        0        0 2024-05-03 22:08:46.026253 heaserver-1.5.2/awss3tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-03 22:08:46.057051 heaserver-1.5.2/awss3tests/heaserver/awss3tests/
--rw-rw-rw-   0        0        0        0 2023-12-16 23:04:09.000000 heaserver-1.5.2/awss3tests/heaserver/awss3tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:08:46.065914 heaserver-1.5.2/awss3tests/heaserver/awss3tests/__pycache__/
--rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.5.2/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.16864
--rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.5.2/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.27996
--rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.5.2/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.5.2/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29888
--rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.5.2/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.35312
--rw-rw-rw-   0        0        0     3169 2023-12-16 23:04:09.000000 heaserver-1.5.2/awss3tests/heaserver/awss3tests/test_all.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:08:46.027282 heaserver-1.5.2/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-05-03 22:08:46.027801 heaserver-1.5.2/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-03 22:08:46.094193 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:08:46.130813 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/
--rw-rw-rw-   0        0        0     1722 2023-12-20 00:04:02.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.15624
--rw-rw-rw-   0        0        0     1722 2023-12-20 00:04:02.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160
--rw-rw-rw-   0        0        0      612 2023-12-20 00:04:02.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-310-pytest-7.4.0.pyc.28520
--rw-rw-rw-   0        0        0     1465 2023-12-20 00:04:02.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.15624
--rw-rw-rw-   0        0        0     1465 2023-12-20 00:04:02.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.41056
--rw-rw-rw-   0        0        0      630 2023-12-20 00:04:02.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624
--rw-rw-rw-   0        0        0      630 2023-12-20 00:04:02.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.35160
--rw-rw-rw-   0        0        0     3839 2023-12-20 00:04:02.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.15624
--rw-rw-rw-   0        0        0     3839 2023-12-20 00:04:02.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.41056
--rw-rw-rw-   0        0        0     6107 2024-05-03 03:20:50.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-311-pytest-7.4.4.pyc.29500
--rw-rw-rw-   0        0        0     6100 2024-04-16 21:05:42.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-311-pytest-7.4.4.pyc.40780
--rw-rw-rw-   0        0        0     1290 2023-12-20 00:04:02.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.28520
--rw-rw-rw-   0        0        0     1290 2023-12-20 00:04:02.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160
--rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.28520
--rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.35160
--rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.41056
--rw-rw-rw-   0        0        0     1723 2024-03-19 23:29:00.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.24968
--rw-rw-rw-   0        0        0     1043 2023-12-20 00:04:02.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.28520
--rw-rw-rw-   0        0        0     1043 2023-12-20 00:04:02.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.41056
--rw-rw-rw-   0        0        0      627 2023-12-20 00:04:02.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624
--rw-rw-rw-   0        0        0      627 2023-12-20 00:04:02.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.41056
--rw-rw-rw-   0        0        0     5996 2023-12-16 23:04:09.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/clienttestcase.py
--rw-rw-rw-   0        0        0     6620 2023-12-16 23:04:09.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/componentpermissionstestcase.py
--rw-rw-rw-   0        0        0     5992 2024-04-09 21:13:46.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/componenttestcase.py
--rw-rw-rw-   0        0        0     5775 2024-05-03 21:58:58.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/organizationpermissionstestcase.py
--rw-rw-rw-   0        0        0     5544 2024-05-03 21:58:58.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/organizationtestcase.py
--rw-rw-rw-   0        0        0    12856 2023-12-16 23:04:10.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/service.py
--rw-rw-rw-   0        0        0     1024 2023-12-16 23:04:10.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/test_client.py
--rw-rw-rw-   0        0        0     1193 2023-12-16 23:04:10.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/test_component_with_bad_permissions.py
--rw-rw-rw-   0        0        0      198 2023-12-16 23:04:10.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/test_delete_component.py
--rw-rw-rw-   0        0        0      194 2022-03-11 01:28:19.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/test_get_all_components.py
--rw-rw-rw-   0        0        0      888 2023-12-16 23:04:10.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/test_get_component.py
--rw-rw-rw-   0        0        0      207 2023-12-16 23:04:10.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/test_get_organization_permissions.py
--rw-rw-rw-   0        0        0     4749 2024-05-03 21:58:58.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/test_mongoservicelib.py
--rw-rw-rw-   0        0        0     1011 2023-12-16 23:04:10.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/test_organization_with_bad_permissions.py
--rw-rw-rw-   0        0        0      521 2023-12-16 23:04:10.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/test_post_component.py
--rw-rw-rw-   0        0        0      404 2023-12-16 23:04:10.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/test_put_component.py
--rw-rw-rw-   0        0        0      203 2023-12-16 23:04:10.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/test_put_organization_permissions.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:08:46.132813 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/wstl/
--rw-rw-rw-   0        0        0    16440 2023-12-16 23:04:10.000000 heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/wstl/all.json
--rw-rw-rw-   0        0        0      132 2023-12-16 23:04:10.000000 heaserver-1.5.2/pytest.ini
--rw-rw-rw-   0        0        0      237 2023-12-16 23:04:10.000000 heaserver-1.5.2/requirements_dev.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 22:08:46.510014 heaserver-1.5.2/setup.cfg
--rw-rw-rw-   0        0        0     2870 2024-05-03 22:08:11.000000 heaserver-1.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:08:46.029864 heaserver-1.5.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-03 22:08:46.029864 heaserver-1.5.2/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-03 22:08:46.188880 heaserver-1.5.2/src/heaserver/service/
--rw-rw-rw-   0        0        0     1176 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/__init__.py
--rw-rw-rw-   0        0        0     7213 2024-01-04 00:01:31.000000 heaserver-1.5.2/src/heaserver/service/activity.py
--rw-rw-rw-   0        0        0    14193 2024-05-03 21:58:58.000000 heaserver-1.5.2/src/heaserver/service/aiohttp.py
--rw-rw-rw-   0        0        0     1688 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/appfactory.py
--rw-rw-rw-   0        0        0      758 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/appproperty.py
--rw-rw-rw-   0        0        0     8521 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/backgroundtasks.py
--rw-rw-rw-   0        0        0     1497 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/caching.py
--rw-rw-rw-   0        0        0       64 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/caching_strategy.py
--rw-rw-rw-   0        0        0    24613 2024-05-03 21:59:07.000000 heaserver-1.5.2/src/heaserver/service/client.py
--rw-rw-rw-   0        0        0     2460 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/config.py
--rw-rw-rw-   0        0        0      256 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/customhdrs.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:08:46.201766 heaserver-1.5.2/src/heaserver/service/db/
--rw-rw-rw-   0        0        0      392 2022-03-11 01:28:19.000000 heaserver-1.5.2/src/heaserver/service/db/__init__.py
--rw-rw-rw-   0        0        0    27286 2024-05-03 21:58:58.000000 heaserver-1.5.2/src/heaserver/service/db/aws.py
--rw-rw-rw-   0        0        0    58921 2024-03-27 00:01:36.000000 heaserver-1.5.2/src/heaserver/service/db/awsservicelib.py
--rw-rw-rw-   0        0        0    31583 2024-05-03 21:58:58.000000 heaserver-1.5.2/src/heaserver/service/db/database.py
--rw-rw-rw-   0        0        0     6599 2022-03-11 01:28:19.000000 heaserver-1.5.2/src/heaserver/service/db/dbapi2.py
--rw-rw-rw-   0        0        0    31960 2024-05-03 21:58:58.000000 heaserver-1.5.2/src/heaserver/service/db/mongo.py
--rw-rw-rw-   0        0        0     4515 2024-04-05 18:40:52.000000 heaserver-1.5.2/src/heaserver/service/db/mongoexpr.py
--rw-rw-rw-   0        0        0    26453 2024-04-03 23:37:27.000000 heaserver-1.5.2/src/heaserver/service/db/mongoservicelib.py
--rw-rw-rw-   0        0        0      252 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/defaults.py
--rw-rw-rw-   0        0        0      150 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/error.py
--rw-rw-rw-   0        0        0     4709 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/expression.py
--rw-rw-rw-   0        0        0      773 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/functional.py
--rw-rw-rw-   0        0        0    19840 2024-03-21 03:54:08.000000 heaserver-1.5.2/src/heaserver/service/heaobjectsupport.py
--rw-rw-rw-   0        0        0      683 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/jsonschema.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:08:46.209815 heaserver-1.5.2/src/heaserver/service/jsonschemafiles/
--rw-rw-rw-   0        0        0      606 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/jsonschemafiles/__init__.py
--rw-rw-rw-   0        0        0      787 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/jsonschemafiles/cjtemplate.json
--rw-rw-rw-   0        0        0       87 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/jsonschemafiles/nvpjson.json
--rw-rw-rw-   0        0        0     2214 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/jsonschemafiles/wstl.json
--rw-rw-rw-   0        0        0     4970 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/jsonschemafiles/wstlaction.json
--rw-rw-rw-   0        0        0      987 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/jsonschemavalidator.py
--rw-rw-rw-   0        0        0    21655 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/messagebroker.py
--rw-rw-rw-   0        0        0      539 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/mimetypes.py
--rw-rw-rw-   0        0        0      639 2022-03-11 01:28:19.000000 heaserver-1.5.2/src/heaserver/service/oidcclaimhdrs.py
--rw-rw-rw-   0        0        0     1558 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/openapi.py
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.5.2/src/heaserver/service/py.typed
--rw-rw-rw-   0        0        0      103 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/registryproperty.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:08:46.221898 heaserver-1.5.2/src/heaserver/service/representor/
--rw-rw-rw-   0        0        0     1426 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/representor/__init__.py
--rw-rw-rw-   0        0        0    26065 2024-05-02 20:04:27.000000 heaserver-1.5.2/src/heaserver/service/representor/cj.py
--rw-rw-rw-   0        0        0      170 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/representor/error.py
--rw-rw-rw-   0        0        0     7259 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/representor/factory.py
--rw-rw-rw-   0        0        0     2231 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/representor/nvpjson.py
--rw-rw-rw-   0        0        0     3244 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/representor/representor.py
--rw-rw-rw-   0        0        0     1551 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/representor/wstljson.py
--rw-rw-rw-   0        0        0     1742 2024-03-19 23:15:41.000000 heaserver-1.5.2/src/heaserver/service/representor/xwwwformurlencoded.py
--rw-rw-rw-   0        0        0      114 2022-03-11 01:28:19.000000 heaserver-1.5.2/src/heaserver/service/requestproperty.py
--rw-rw-rw-   0        0        0    29114 2024-04-01 23:40:09.000000 heaserver-1.5.2/src/heaserver/service/response.py
--rw-rw-rw-   0        0        0    15617 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/runner.py
--rw-rw-rw-   0        0        0       32 2024-03-26 22:51:02.000000 heaserver-1.5.2/src/heaserver/service/sources.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:08:46.247531 heaserver-1.5.2/src/heaserver/service/testcase/
--rw-rw-rw-   0        0        0      167 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/testcase/__init__.py
--rw-rw-rw-   0        0        0     2123 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/testcase/aiohttptestcase.py
--rw-rw-rw-   0        0        0     1508 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/testcase/awsdockermongo.py
--rw-rw-rw-   0        0        0     3944 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/testcase/awss3microservicetestcase.py
--rw-rw-rw-   0        0        0    15471 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/testcase/collection.py
--rw-rw-rw-   0        0        0     6655 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/testcase/docker.py
--rw-rw-rw-   0        0        0     8062 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/testcase/dockermongo.py
--rw-rw-rw-   0        0        0    40481 2024-05-02 20:04:27.000000 heaserver-1.5.2/src/heaserver/service/testcase/expectedvalues.py
--rw-rw-rw-   0        0        0    17534 2024-04-01 23:40:09.000000 heaserver-1.5.2/src/heaserver/service/testcase/microservicetestcase.py
--rw-rw-rw-   0        0        0   130477 2024-04-01 23:40:09.000000 heaserver-1.5.2/src/heaserver/service/testcase/mixin.py
--rw-rw-rw-   0        0        0    18431 2024-05-03 21:58:58.000000 heaserver-1.5.2/src/heaserver/service/testcase/mockaws.py
--rw-rw-rw-   0        0        0      662 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/testcase/mockdatabase.py
--rw-rw-rw-   0        0        0    21242 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/testcase/mockmongo.py
--rw-rw-rw-   0        0        0      555 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/testcase/simpleaiohttptestcase.py
--rw-rw-rw-   0        0        0     7531 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/testcase/swaggerui.py
--rw-rw-rw-   0        0        0    29140 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/testcase/testenv.py
--rw-rw-rw-   0        0        0     2132 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/testcase/util.py
--rw-rw-rw-   0        0        0     2877 2023-12-16 23:04:10.000000 heaserver-1.5.2/src/heaserver/service/uritemplate.py
--rw-rw-rw-   0        0        0    11636 2024-01-04 00:01:31.000000 heaserver-1.5.2/src/heaserver/service/util.py
--rw-rw-rw-   0        0        0    36804 2024-04-01 23:40:09.000000 heaserver-1.5.2/src/heaserver/service/wstl.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:08:46.506244 heaserver-1.5.2/src/heaserver.egg-info/
--rw-rw-rw-   0        0        0     7629 2024-05-03 22:08:45.000000 heaserver-1.5.2/src/heaserver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    17709 2024-05-03 22:08:46.000000 heaserver-1.5.2/src/heaserver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 22:08:45.000000 heaserver-1.5.2/src/heaserver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      455 2024-05-03 22:08:45.000000 heaserver-1.5.2/src/heaserver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-03 22:08:45.000000 heaserver-1.5.2/src/heaserver.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-03 22:08:46.032455 heaserver-1.5.2/tests/
-drwxrwxrwx   0        0        0        0 2024-05-03 22:08:46.032976 heaserver-1.5.2/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-03 22:08:46.315825 heaserver-1.5.2/tests/heaserver/servicetest/
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.5.2/tests/heaserver/servicetest/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:08:46.370618 heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/
--rw-rw-rw-   0        0        0    11044 2024-03-19 23:09:55.000000 heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.19788
--rw-rw-rw-   0        0        0    11044 2024-03-19 23:09:55.000000 heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0     5139 2024-03-19 23:09:55.000000 heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_caching.cpython-311-pytest-7.4.4.pyc.29888
--rw-rw-rw-   0        0        0    13515 2024-03-19 23:09:55.000000 heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.29888
--rw-rw-rw-   0        0        0     2266 2024-03-19 23:09:55.000000 heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.19788
--rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     2605 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.35312
--rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0      826 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0    21674 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0     1870 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.27996
--rw-rw-rw-   0        0        0     1870 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35312
--rw-rw-rw-   0        0        0    18112 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0    18112 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0    12001 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0    12001 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.3836
-drwxrwxrwx   0        0        0        0 2024-05-03 22:08:46.372691 heaserver-1.5.2/tests/heaserver/servicetest/aiohttpdata/
--rw-rw-rw-   0        0        0      258 2023-12-16 23:04:10.000000 heaserver-1.5.2/tests/heaserver/servicetest/aiohttpdata/requirements_dev.txt
--rw-rw-rw-   0        0        0     6442 2023-12-16 23:04:10.000000 heaserver-1.5.2/tests/heaserver/servicetest/componentpermissionstestcase.py
--rw-rw-rw-   0        0        0    17429 2024-04-09 21:13:46.000000 heaserver-1.5.2/tests/heaserver/servicetest/componenttestcase.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:08:46.376349 heaserver-1.5.2/tests/heaserver/servicetest/db/
--rw-rw-rw-   0        0        0        0 2023-12-16 23:04:10.000000 heaserver-1.5.2/tests/heaserver/servicetest/db/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:08:46.387584 heaserver-1.5.2/tests/heaserver/servicetest/db/__pycache__/
--rw-rw-rw-   0        0        0     1344 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.27996
--rw-rw-rw-   0        0        0     1344 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0      551 2023-12-16 23:04:10.000000 heaserver-1.5.2/tests/heaserver/servicetest/db/test_mongo.py
--rw-rw-rw-   0        0        0     7303 2023-12-16 23:04:10.000000 heaserver-1.5.2/tests/heaserver/servicetest/db/test_mongoexpr.py
--rw-rw-rw-   0        0        0     5571 2024-05-03 21:58:58.000000 heaserver-1.5.2/tests/heaserver/servicetest/organizationpermissionstestcase.py
--rw-rw-rw-   0        0        0     5997 2024-05-03 21:58:58.000000 heaserver-1.5.2/tests/heaserver/servicetest/organizationtestcase.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:08:46.412357 heaserver-1.5.2/tests/heaserver/servicetest/representor/
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:08:46.501505 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/
--rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.27996
--rw-rw-rw-   0        0        0    62667 2024-04-03 18:03:31.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.28016
--rw-rw-rw-   0        0        0    54596 2024-03-29 23:13:01.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35228
--rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35312
--rw-rw-rw-   0        0        0    62667 2024-04-03 18:03:31.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35444
--rw-rw-rw-   0        0        0    62667 2024-04-03 18:03:31.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.37360
--rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.35312
--rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0     7286 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.19788
--rw-rw-rw-   0        0        0     7286 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11224
--rw-rw-rw-   0        0        0     6209 2024-03-29 23:04:43.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11864
--rw-rw-rw-   0        0        0     6209 2024-03-29 23:04:43.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13080
--rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13852
--rw-rw-rw-   0        0        0     6209 2024-03-29 23:04:43.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.15488
--rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.1816
--rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.19788
--rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.28016
--rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.30312
--rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.34620
--rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.37360
--rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.16864
--rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.19712
--rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.23624
--rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.29888
--rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.4904
--rw-rw-rw-   0        0        0      192 2022-03-11 01:28:19.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/all.json
--rw-rw-rw-   0        0        0      268 2022-03-11 01:28:19.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/all_cj_item_href.json
--rw-rw-rw-   0        0        0      268 2022-03-11 01:28:19.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/all_cj_item_link.json
--rw-rw-rw-   0        0        0      642 2022-03-11 01:28:19.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/all_cj_queries.json
--rw-rw-rw-   0        0        0     2670 2023-12-16 23:04:10.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/all_cj_template.json
--rw-rw-rw-   0        0        0      267 2022-03-11 01:28:19.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/all_cj_toplevel_link_for_item.json
--rw-rw-rw-   0        0        0      263 2022-03-11 01:28:19.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/all_cj_toplevel_link_for_list.json
--rw-rw-rw-   0        0        0    62769 2024-04-01 23:40:09.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/test_cj.py
--rw-rw-rw-   0        0        0     2671 2022-03-11 01:28:19.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/test_factory.py
--rw-rw-rw-   0        0        0     4181 2023-12-16 23:04:10.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/test_nvpjson.py
--rw-rw-rw-   0        0        0      281 2022-03-11 01:28:19.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/test_supports_links.py
--rw-rw-rw-   0        0        0     5676 2024-04-01 23:40:09.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/test_wstljson.py
--rw-rw-rw-   0        0        0     2396 2024-03-21 03:54:08.000000 heaserver-1.5.2/tests/heaserver/servicetest/representor/test_xwwwformurlencoded.py
--rw-rw-rw-   0        0        0    13067 2023-12-16 23:04:10.000000 heaserver-1.5.2/tests/heaserver/servicetest/service.py
--rw-rw-rw-   0        0        0     9455 2024-01-04 00:01:31.000000 heaserver-1.5.2/tests/heaserver/servicetest/test_activity.py
--rw-rw-rw-   0        0        0     3976 2023-12-16 23:04:10.000000 heaserver-1.5.2/tests/heaserver/servicetest/test_aiohttp.py
--rw-rw-rw-   0        0        0     5894 2023-12-16 23:04:10.000000 heaserver-1.5.2/tests/heaserver/servicetest/test_backgroundtasks.py
--rw-rw-rw-   0        0        0     2506 2023-12-16 23:04:10.000000 heaserver-1.5.2/tests/heaserver/servicetest/test_caching.py
--rw-rw-rw-   0        0        0     7131 2024-04-09 21:13:46.000000 heaserver-1.5.2/tests/heaserver/servicetest/test_client.py
--rw-rw-rw-   0        0        0     1193 2023-12-16 23:04:10.000000 heaserver-1.5.2/tests/heaserver/servicetest/test_component_with_bad_permissions.py
--rw-rw-rw-   0        0        0     1127 2023-12-16 23:04:10.000000 heaserver-1.5.2/tests/heaserver/servicetest/test_configuration.py
--rw-rw-rw-   0        0        0      819 2023-12-16 23:04:10.000000 heaserver-1.5.2/tests/heaserver/servicetest/test_database_classes.py
--rw-rw-rw-   0        0        0      204 2023-12-16 23:04:10.000000 heaserver-1.5.2/tests/heaserver/servicetest/test_delete_component.py
--rw-rw-rw-   0        0        0     6181 2023-12-16 23:04:10.000000 heaserver-1.5.2/tests/heaserver/servicetest/test_expression.py
--rw-rw-rw-   0        0        0      405 2023-12-16 23:04:10.000000 heaserver-1.5.2/tests/heaserver/servicetest/test_functional.py
--rw-rw-rw-   0        0        0      422 2023-12-16 23:04:10.000000 heaserver-1.5.2/tests/heaserver/servicetest/test_get_all_components.py
--rw-rw-rw-   0        0        0     3070 2023-12-16 23:04:10.000000 heaserver-1.5.2/tests/heaserver/servicetest/test_get_component.py
--rw-rw-rw-   0        0        0      209 2023-12-16 23:04:10.000000 heaserver-1.5.2/tests/heaserver/servicetest/test_get_organization_permissions.py
--rw-rw-rw-   0        0        0     5366 2024-04-09 21:13:46.000000 heaserver-1.5.2/tests/heaserver/servicetest/test_heaobjectsupport.py
--rw-rw-rw-   0        0        0     5746 2023-12-16 23:04:10.000000 heaserver-1.5.2/tests/heaserver/servicetest/test_jsonschemavalidator.py
--rw-rw-rw-   0        0        0      909 2023-12-16 23:04:10.000000 heaserver-1.5.2/tests/heaserver/servicetest/test_mimetypes.py
--rw-rw-rw-   0        0        0      331 2023-12-16 23:04:10.000000 heaserver-1.5.2/tests/heaserver/servicetest/test_not_imported.py
--rw-rw-rw-   0        0        0     1005 2023-12-16 23:04:10.000000 heaserver-1.5.2/tests/heaserver/servicetest/test_organization_with_bad_permissions.py
--rw-rw-rw-   0        0        0     1274 2023-12-16 23:04:10.000000 heaserver-1.5.2/tests/heaserver/servicetest/test_post_component.py
--rw-rw-rw-   0        0        0     1265 2023-12-16 23:04:10.000000 heaserver-1.5.2/tests/heaserver/servicetest/test_put_component.py
--rw-rw-rw-   0        0        0      253 2023-12-16 23:04:10.000000 heaserver-1.5.2/tests/heaserver/servicetest/test_put_organization_permissions.py
--rw-rw-rw-   0        0        0     2488 2023-12-16 23:04:10.000000 heaserver-1.5.2/tests/heaserver/servicetest/test_response.py
--rw-rw-rw-   0        0        0      570 2023-12-16 23:04:10.000000 heaserver-1.5.2/tests/heaserver/servicetest/test_testenv.py
--rw-rw-rw-   0        0        0     1929 2023-12-16 23:04:10.000000 heaserver-1.5.2/tests/heaserver/servicetest/test_uritemplate.py
--rw-rw-rw-   0        0        0     8782 2023-12-16 23:04:10.000000 heaserver-1.5.2/tests/heaserver/servicetest/test_util.py
--rw-rw-rw-   0        0        0     6255 2023-12-16 23:04:10.000000 heaserver-1.5.2/tests/heaserver/servicetest/test_wstl.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:08:46.504154 heaserver-1.5.2/tests/heaserver/servicetest/wstl/
--rw-rw-rw-   0        0        0    16436 2023-12-16 23:04:10.000000 heaserver-1.5.2/tests/heaserver/servicetest/wstl/all.json
--rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.5.2/tests/heaserver/servicetest/wstl_1.json
--rw-rw-rw-   0        0        0     1214 2022-03-11 01:28:19.000000 heaserver-1.5.2/tests/heaserver/servicetest/wstl_10a.json
--rw-rw-rw-   0        0        0     1240 2022-03-11 01:28:19.000000 heaserver-1.5.2/tests/heaserver/servicetest/wstl_10b.json
--rw-rw-rw-   0        0        0     2355 2022-03-11 01:28:19.000000 heaserver-1.5.2/tests/heaserver/servicetest/wstl_11.json
--rw-rw-rw-   0        0        0     1187 2022-03-11 01:28:19.000000 heaserver-1.5.2/tests/heaserver/servicetest/wstl_2.json
--rw-rw-rw-   0        0        0     1190 2022-03-11 01:28:19.000000 heaserver-1.5.2/tests/heaserver/servicetest/wstl_3.json
--rw-rw-rw-   0        0        0     1158 2022-03-11 01:28:19.000000 heaserver-1.5.2/tests/heaserver/servicetest/wstl_4.json
--rw-rw-rw-   0        0        0      269 2022-03-11 01:28:19.000000 heaserver-1.5.2/tests/heaserver/servicetest/wstl_5.json
--rw-rw-rw-   0        0        0      531 2022-03-11 01:28:19.000000 heaserver-1.5.2/tests/heaserver/servicetest/wstl_6.json
--rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.5.2/tests/heaserver/servicetest/wstl_7.json
--rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.5.2/tests/heaserver/servicetest/wstl_8.json
--rw-rw-rw-   0        0        0      204 2022-03-11 01:28:19.000000 heaserver-1.5.2/tests/heaserver/servicetest/wstl_9.json
+drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.995705 heaserver-1.5.3/
+-rw-rw-rw-   0        0        0      261 2022-03-11 01:28:19.000000 heaserver-1.5.3/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-12-16 23:04:09.000000 heaserver-1.5.3/.gitignore
+-rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:19.000000 heaserver-1.5.3/LICENSE
+-rw-rw-rw-   0        0        0      243 2023-12-16 23:04:09.000000 heaserver-1.5.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     7928 2024-05-05 18:18:08.993702 heaserver-1.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5933 2024-05-05 17:45:18.000000 heaserver-1.5.3/README.md
+-rw-rw-rw-   0        0        0     1612 2023-12-16 23:04:09.000000 heaserver-1.5.3/RELEASING.md
+drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.281294 heaserver-1.5.3/awss3integrationtests/
+drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.281294 heaserver-1.5.3/awss3integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.320908 heaserver-1.5.3/awss3integrationtests/heaserver/awss3tests/
+-rw-rw-rw-   0        0        0        0 2023-12-16 23:04:09.000000 heaserver-1.5.3/awss3integrationtests/heaserver/awss3tests/__init__.py
+-rw-rw-rw-   0        0        0    34976 2024-04-01 23:40:09.000000 heaserver-1.5.3/awss3integrationtests/heaserver/awss3tests/awss3foldertestcase.py
+-rw-rw-rw-   0        0        0     1416 2023-12-16 23:04:09.000000 heaserver-1.5.3/awss3integrationtests/heaserver/awss3tests/service.py
+-rw-rw-rw-   0        0        0    19401 2024-04-08 18:06:35.000000 heaserver-1.5.3/awss3integrationtests/heaserver/awss3tests/test_all.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.322529 heaserver-1.5.3/awss3integrationtests/heaserver/awss3tests/wstl/
+-rw-rw-rw-   0        0        0    16955 2023-12-16 23:04:09.000000 heaserver-1.5.3/awss3integrationtests/heaserver/awss3tests/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.282872 heaserver-1.5.3/awss3tests/
+drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.283396 heaserver-1.5.3/awss3tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.326177 heaserver-1.5.3/awss3tests/heaserver/awss3tests/
+-rw-rw-rw-   0        0        0        0 2023-12-16 23:04:09.000000 heaserver-1.5.3/awss3tests/heaserver/awss3tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.340959 heaserver-1.5.3/awss3tests/heaserver/awss3tests/__pycache__/
+-rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.5.3/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.16864
+-rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.5.3/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.27996
+-rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.5.3/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.5.3/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29888
+-rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.5.3/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.35312
+-rw-rw-rw-   0        0        0     3169 2023-12-16 23:04:09.000000 heaserver-1.5.3/awss3tests/heaserver/awss3tests/test_all.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.284957 heaserver-1.5.3/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.284957 heaserver-1.5.3/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.382415 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.433268 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/
+-rw-rw-rw-   0        0        0     1722 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.15624
+-rw-rw-rw-   0        0        0     1722 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160
+-rw-rw-rw-   0        0        0      612 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-310-pytest-7.4.0.pyc.28520
+-rw-rw-rw-   0        0        0     1465 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.15624
+-rw-rw-rw-   0        0        0     1465 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.41056
+-rw-rw-rw-   0        0        0      630 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624
+-rw-rw-rw-   0        0        0      630 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.35160
+-rw-rw-rw-   0        0        0     3839 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.15624
+-rw-rw-rw-   0        0        0     3839 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.41056
+-rw-rw-rw-   0        0        0     6107 2024-05-03 03:20:50.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-311-pytest-7.4.4.pyc.29500
+-rw-rw-rw-   0        0        0     6100 2024-04-16 21:05:42.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-311-pytest-7.4.4.pyc.40780
+-rw-rw-rw-   0        0        0     1290 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.28520
+-rw-rw-rw-   0        0        0     1290 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160
+-rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.28520
+-rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.35160
+-rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.41056
+-rw-rw-rw-   0        0        0     1723 2024-03-19 23:29:00.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.24968
+-rw-rw-rw-   0        0        0     1043 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.28520
+-rw-rw-rw-   0        0        0     1043 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.41056
+-rw-rw-rw-   0        0        0      627 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624
+-rw-rw-rw-   0        0        0      627 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.41056
+-rw-rw-rw-   0        0        0     5996 2023-12-16 23:04:09.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/clienttestcase.py
+-rw-rw-rw-   0        0        0     6620 2023-12-16 23:04:09.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/componentpermissionstestcase.py
+-rw-rw-rw-   0        0        0     5992 2024-04-09 21:13:46.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/componenttestcase.py
+-rw-rw-rw-   0        0        0     5775 2024-05-03 21:58:58.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/organizationpermissionstestcase.py
+-rw-rw-rw-   0        0        0     5544 2024-05-03 21:58:58.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/organizationtestcase.py
+-rw-rw-rw-   0        0        0    12856 2023-12-16 23:04:10.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/service.py
+-rw-rw-rw-   0        0        0     1024 2023-12-16 23:04:10.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/test_client.py
+-rw-rw-rw-   0        0        0     1193 2023-12-16 23:04:10.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/test_component_with_bad_permissions.py
+-rw-rw-rw-   0        0        0      198 2023-12-16 23:04:10.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/test_delete_component.py
+-rw-rw-rw-   0        0        0      194 2022-03-11 01:28:19.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/test_get_all_components.py
+-rw-rw-rw-   0        0        0      888 2023-12-16 23:04:10.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/test_get_component.py
+-rw-rw-rw-   0        0        0      207 2023-12-16 23:04:10.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/test_get_organization_permissions.py
+-rw-rw-rw-   0        0        0     4749 2024-05-03 21:58:58.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/test_mongoservicelib.py
+-rw-rw-rw-   0        0        0     1011 2023-12-16 23:04:10.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/test_organization_with_bad_permissions.py
+-rw-rw-rw-   0        0        0      521 2023-12-16 23:04:10.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/test_post_component.py
+-rw-rw-rw-   0        0        0      404 2023-12-16 23:04:10.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/test_put_component.py
+-rw-rw-rw-   0        0        0      203 2023-12-16 23:04:10.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/test_put_organization_permissions.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.435901 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/wstl/
+-rw-rw-rw-   0        0        0    16440 2023-12-16 23:04:10.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/wstl/all.json
+-rw-rw-rw-   0        0        0      132 2023-12-16 23:04:10.000000 heaserver-1.5.3/pytest.ini
+-rw-rw-rw-   0        0        0      237 2023-12-16 23:04:10.000000 heaserver-1.5.3/requirements_dev.txt
+-rw-rw-rw-   0        0        0       42 2024-05-05 18:18:08.995705 heaserver-1.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     2870 2024-05-05 18:17:14.000000 heaserver-1.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.287582 heaserver-1.5.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.288105 heaserver-1.5.3/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.532365 heaserver-1.5.3/src/heaserver/service/
+-rw-rw-rw-   0        0        0     1176 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/__init__.py
+-rw-rw-rw-   0        0        0     7213 2024-01-04 00:01:31.000000 heaserver-1.5.3/src/heaserver/service/activity.py
+-rw-rw-rw-   0        0        0    14193 2024-05-03 21:58:58.000000 heaserver-1.5.3/src/heaserver/service/aiohttp.py
+-rw-rw-rw-   0        0        0     1688 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/appfactory.py
+-rw-rw-rw-   0        0        0      758 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/appproperty.py
+-rw-rw-rw-   0        0        0     8521 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/backgroundtasks.py
+-rw-rw-rw-   0        0        0     1497 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/caching.py
+-rw-rw-rw-   0        0        0       64 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/caching_strategy.py
+-rw-rw-rw-   0        0        0    24613 2024-05-03 22:10:30.000000 heaserver-1.5.3/src/heaserver/service/client.py
+-rw-rw-rw-   0        0        0     2460 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/config.py
+-rw-rw-rw-   0        0        0      256 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/customhdrs.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.551367 heaserver-1.5.3/src/heaserver/service/db/
+-rw-rw-rw-   0        0        0      392 2022-03-11 01:28:19.000000 heaserver-1.5.3/src/heaserver/service/db/__init__.py
+-rw-rw-rw-   0        0        0    28250 2024-05-05 18:15:37.000000 heaserver-1.5.3/src/heaserver/service/db/aws.py
+-rw-rw-rw-   0        0        0    58921 2024-03-27 00:01:36.000000 heaserver-1.5.3/src/heaserver/service/db/awsservicelib.py
+-rw-rw-rw-   0        0        0    31583 2024-05-03 21:58:58.000000 heaserver-1.5.3/src/heaserver/service/db/database.py
+-rw-rw-rw-   0        0        0     6599 2022-03-11 01:28:19.000000 heaserver-1.5.3/src/heaserver/service/db/dbapi2.py
+-rw-rw-rw-   0        0        0    31960 2024-05-03 21:58:58.000000 heaserver-1.5.3/src/heaserver/service/db/mongo.py
+-rw-rw-rw-   0        0        0     4515 2024-04-05 18:40:52.000000 heaserver-1.5.3/src/heaserver/service/db/mongoexpr.py
+-rw-rw-rw-   0        0        0    26453 2024-04-03 23:37:27.000000 heaserver-1.5.3/src/heaserver/service/db/mongoservicelib.py
+-rw-rw-rw-   0        0        0      252 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/defaults.py
+-rw-rw-rw-   0        0        0      150 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/error.py
+-rw-rw-rw-   0        0        0     4709 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/expression.py
+-rw-rw-rw-   0        0        0      773 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/functional.py
+-rw-rw-rw-   0        0        0    19840 2024-03-21 03:54:08.000000 heaserver-1.5.3/src/heaserver/service/heaobjectsupport.py
+-rw-rw-rw-   0        0        0      683 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/jsonschema.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.565363 heaserver-1.5.3/src/heaserver/service/jsonschemafiles/
+-rw-rw-rw-   0        0        0      606 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/jsonschemafiles/__init__.py
+-rw-rw-rw-   0        0        0      787 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/jsonschemafiles/cjtemplate.json
+-rw-rw-rw-   0        0        0       87 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/jsonschemafiles/nvpjson.json
+-rw-rw-rw-   0        0        0     2214 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/jsonschemafiles/wstl.json
+-rw-rw-rw-   0        0        0     4970 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/jsonschemafiles/wstlaction.json
+-rw-rw-rw-   0        0        0      987 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/jsonschemavalidator.py
+-rw-rw-rw-   0        0        0    21655 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/messagebroker.py
+-rw-rw-rw-   0        0        0      539 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/mimetypes.py
+-rw-rw-rw-   0        0        0      639 2022-03-11 01:28:19.000000 heaserver-1.5.3/src/heaserver/service/oidcclaimhdrs.py
+-rw-rw-rw-   0        0        0     1558 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/openapi.py
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.5.3/src/heaserver/service/py.typed
+-rw-rw-rw-   0        0        0      103 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/registryproperty.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.592371 heaserver-1.5.3/src/heaserver/service/representor/
+-rw-rw-rw-   0        0        0     1426 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/representor/__init__.py
+-rw-rw-rw-   0        0        0    26065 2024-05-02 20:04:27.000000 heaserver-1.5.3/src/heaserver/service/representor/cj.py
+-rw-rw-rw-   0        0        0      170 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/representor/error.py
+-rw-rw-rw-   0        0        0     7259 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/representor/factory.py
+-rw-rw-rw-   0        0        0     2231 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/representor/nvpjson.py
+-rw-rw-rw-   0        0        0     3244 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/representor/representor.py
+-rw-rw-rw-   0        0        0     1551 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/representor/wstljson.py
+-rw-rw-rw-   0        0        0     1742 2024-03-19 23:15:41.000000 heaserver-1.5.3/src/heaserver/service/representor/xwwwformurlencoded.py
+-rw-rw-rw-   0        0        0      114 2022-03-11 01:28:19.000000 heaserver-1.5.3/src/heaserver/service/requestproperty.py
+-rw-rw-rw-   0        0        0    29114 2024-04-01 23:40:09.000000 heaserver-1.5.3/src/heaserver/service/response.py
+-rw-rw-rw-   0        0        0    15617 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/runner.py
+-rw-rw-rw-   0        0        0       32 2024-03-26 22:51:02.000000 heaserver-1.5.3/src/heaserver/service/sources.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.636627 heaserver-1.5.3/src/heaserver/service/testcase/
+-rw-rw-rw-   0        0        0      167 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/testcase/__init__.py
+-rw-rw-rw-   0        0        0     2123 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/testcase/aiohttptestcase.py
+-rw-rw-rw-   0        0        0     1508 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/testcase/awsdockermongo.py
+-rw-rw-rw-   0        0        0     3944 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/testcase/awss3microservicetestcase.py
+-rw-rw-rw-   0        0        0    15471 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/testcase/collection.py
+-rw-rw-rw-   0        0        0     6655 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/testcase/docker.py
+-rw-rw-rw-   0        0        0     8062 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/testcase/dockermongo.py
+-rw-rw-rw-   0        0        0    40481 2024-05-02 20:04:27.000000 heaserver-1.5.3/src/heaserver/service/testcase/expectedvalues.py
+-rw-rw-rw-   0        0        0    17534 2024-04-01 23:40:09.000000 heaserver-1.5.3/src/heaserver/service/testcase/microservicetestcase.py
+-rw-rw-rw-   0        0        0   130477 2024-04-01 23:40:09.000000 heaserver-1.5.3/src/heaserver/service/testcase/mixin.py
+-rw-rw-rw-   0        0        0    18431 2024-05-03 21:58:58.000000 heaserver-1.5.3/src/heaserver/service/testcase/mockaws.py
+-rw-rw-rw-   0        0        0      662 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/testcase/mockdatabase.py
+-rw-rw-rw-   0        0        0    21242 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/testcase/mockmongo.py
+-rw-rw-rw-   0        0        0      555 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/testcase/simpleaiohttptestcase.py
+-rw-rw-rw-   0        0        0     7531 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/testcase/swaggerui.py
+-rw-rw-rw-   0        0        0    29140 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/testcase/testenv.py
+-rw-rw-rw-   0        0        0     2132 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/testcase/util.py
+-rw-rw-rw-   0        0        0     2877 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/uritemplate.py
+-rw-rw-rw-   0        0        0    11636 2024-01-04 00:01:31.000000 heaserver-1.5.3/src/heaserver/service/util.py
+-rw-rw-rw-   0        0        0    36804 2024-04-01 23:40:09.000000 heaserver-1.5.3/src/heaserver/service/wstl.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.991711 heaserver-1.5.3/src/heaserver.egg-info/
+-rw-rw-rw-   0        0        0     7928 2024-05-05 18:18:08.000000 heaserver-1.5.3/src/heaserver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    17709 2024-05-05 18:18:08.000000 heaserver-1.5.3/src/heaserver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 18:18:08.000000 heaserver-1.5.3/src/heaserver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      455 2024-05-05 18:18:08.000000 heaserver-1.5.3/src/heaserver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-05 18:18:08.000000 heaserver-1.5.3/src/heaserver.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.290745 heaserver-1.5.3/tests/
+drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.291280 heaserver-1.5.3/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.751462 heaserver-1.5.3/tests/heaserver/servicetest/
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.815224 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/
+-rw-rw-rw-   0        0        0    11044 2024-03-19 23:09:55.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.19788
+-rw-rw-rw-   0        0        0    11044 2024-03-19 23:09:55.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0     5139 2024-03-19 23:09:55.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_caching.cpython-311-pytest-7.4.4.pyc.29888
+-rw-rw-rw-   0        0        0    13515 2024-03-19 23:09:55.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.29888
+-rw-rw-rw-   0        0        0     2266 2024-03-19 23:09:55.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.19788
+-rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     2605 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.35312
+-rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0      826 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0    21674 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0     1870 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.27996
+-rw-rw-rw-   0        0        0     1870 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35312
+-rw-rw-rw-   0        0        0    18112 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0    18112 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0    12001 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0    12001 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.3836
+drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.819219 heaserver-1.5.3/tests/heaserver/servicetest/aiohttpdata/
+-rw-rw-rw-   0        0        0      258 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/aiohttpdata/requirements_dev.txt
+-rw-rw-rw-   0        0        0     6442 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/componentpermissionstestcase.py
+-rw-rw-rw-   0        0        0    17429 2024-04-09 21:13:46.000000 heaserver-1.5.3/tests/heaserver/servicetest/componenttestcase.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.826212 heaserver-1.5.3/tests/heaserver/servicetest/db/
+-rw-rw-rw-   0        0        0        0 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/db/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.841295 heaserver-1.5.3/tests/heaserver/servicetest/db/__pycache__/
+-rw-rw-rw-   0        0        0     1344 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.27996
+-rw-rw-rw-   0        0        0     1344 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0      551 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/db/test_mongo.py
+-rw-rw-rw-   0        0        0     7303 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/db/test_mongoexpr.py
+-rw-rw-rw-   0        0        0     5571 2024-05-03 21:58:58.000000 heaserver-1.5.3/tests/heaserver/servicetest/organizationpermissionstestcase.py
+-rw-rw-rw-   0        0        0     5997 2024-05-03 21:58:58.000000 heaserver-1.5.3/tests/heaserver/servicetest/organizationtestcase.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.877504 heaserver-1.5.3/tests/heaserver/servicetest/representor/
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.983722 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/
+-rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.27996
+-rw-rw-rw-   0        0        0    62667 2024-04-03 18:03:31.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.28016
+-rw-rw-rw-   0        0        0    54596 2024-03-29 23:13:01.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35228
+-rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35312
+-rw-rw-rw-   0        0        0    62667 2024-04-03 18:03:31.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35444
+-rw-rw-rw-   0        0        0    62667 2024-04-03 18:03:31.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.37360
+-rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.35312
+-rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0     7286 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.19788
+-rw-rw-rw-   0        0        0     7286 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11224
+-rw-rw-rw-   0        0        0     6209 2024-03-29 23:04:43.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11864
+-rw-rw-rw-   0        0        0     6209 2024-03-29 23:04:43.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13080
+-rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13852
+-rw-rw-rw-   0        0        0     6209 2024-03-29 23:04:43.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.15488
+-rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.1816
+-rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.19788
+-rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.28016
+-rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.30312
+-rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.34620
+-rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.37360
+-rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.16864
+-rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.19712
+-rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.23624
+-rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.29888
+-rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.4904
+-rw-rw-rw-   0        0        0      192 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/all.json
+-rw-rw-rw-   0        0        0      268 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/all_cj_item_href.json
+-rw-rw-rw-   0        0        0      268 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/all_cj_item_link.json
+-rw-rw-rw-   0        0        0      642 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/all_cj_queries.json
+-rw-rw-rw-   0        0        0     2670 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/all_cj_template.json
+-rw-rw-rw-   0        0        0      267 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/all_cj_toplevel_link_for_item.json
+-rw-rw-rw-   0        0        0      263 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/all_cj_toplevel_link_for_list.json
+-rw-rw-rw-   0        0        0    62769 2024-04-01 23:40:09.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/test_cj.py
+-rw-rw-rw-   0        0        0     2671 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/test_factory.py
+-rw-rw-rw-   0        0        0     4181 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/test_nvpjson.py
+-rw-rw-rw-   0        0        0      281 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/test_supports_links.py
+-rw-rw-rw-   0        0        0     5676 2024-04-01 23:40:09.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/test_wstljson.py
+-rw-rw-rw-   0        0        0     2396 2024-03-21 03:54:08.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/test_xwwwformurlencoded.py
+-rw-rw-rw-   0        0        0    13067 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/service.py
+-rw-rw-rw-   0        0        0     9455 2024-01-04 00:01:31.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_activity.py
+-rw-rw-rw-   0        0        0     3976 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_aiohttp.py
+-rw-rw-rw-   0        0        0     5894 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_backgroundtasks.py
+-rw-rw-rw-   0        0        0     2506 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_caching.py
+-rw-rw-rw-   0        0        0     7131 2024-04-09 21:13:46.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_client.py
+-rw-rw-rw-   0        0        0     1193 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_component_with_bad_permissions.py
+-rw-rw-rw-   0        0        0     1127 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_configuration.py
+-rw-rw-rw-   0        0        0      819 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_database_classes.py
+-rw-rw-rw-   0        0        0      204 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_delete_component.py
+-rw-rw-rw-   0        0        0     6181 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_expression.py
+-rw-rw-rw-   0        0        0      405 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_functional.py
+-rw-rw-rw-   0        0        0      422 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_get_all_components.py
+-rw-rw-rw-   0        0        0     3070 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_get_component.py
+-rw-rw-rw-   0        0        0      209 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_get_organization_permissions.py
+-rw-rw-rw-   0        0        0     5366 2024-04-09 21:13:46.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_heaobjectsupport.py
+-rw-rw-rw-   0        0        0     5746 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_jsonschemavalidator.py
+-rw-rw-rw-   0        0        0      909 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_mimetypes.py
+-rw-rw-rw-   0        0        0      331 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_not_imported.py
+-rw-rw-rw-   0        0        0     1005 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_organization_with_bad_permissions.py
+-rw-rw-rw-   0        0        0     1274 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_post_component.py
+-rw-rw-rw-   0        0        0     1265 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_put_component.py
+-rw-rw-rw-   0        0        0      253 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_put_organization_permissions.py
+-rw-rw-rw-   0        0        0     2488 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_response.py
+-rw-rw-rw-   0        0        0      570 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_testenv.py
+-rw-rw-rw-   0        0        0     1929 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_uritemplate.py
+-rw-rw-rw-   0        0        0     8782 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_util.py
+-rw-rw-rw-   0        0        0     6255 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_wstl.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.987709 heaserver-1.5.3/tests/heaserver/servicetest/wstl/
+-rw-rw-rw-   0        0        0    16436 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/wstl/all.json
+-rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/wstl_1.json
+-rw-rw-rw-   0        0        0     1214 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/wstl_10a.json
+-rw-rw-rw-   0        0        0     1240 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/wstl_10b.json
+-rw-rw-rw-   0        0        0     2355 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/wstl_11.json
+-rw-rw-rw-   0        0        0     1187 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/wstl_2.json
+-rw-rw-rw-   0        0        0     1190 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/wstl_3.json
+-rw-rw-rw-   0        0        0     1158 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/wstl_4.json
+-rw-rw-rw-   0        0        0      269 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/wstl_5.json
+-rw-rw-rw-   0        0        0      531 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/wstl_6.json
+-rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/wstl_7.json
+-rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/wstl_8.json
+-rw-rw-rw-   0        0        0      204 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/wstl_9.json
```

### Comparing `heaserver-1.5.2/LICENSE` & `heaserver-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/PKG-INFO` & `heaserver-1.5.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver
-Version: 1.5.2
+Version: 1.5.3
 Summary: The server side of HEA.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -47,14 +47,19 @@
 Requires-Dist: types-cachetools~=5.3.0
 
 # HEA Server Framework
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Server Framework contains shared code for creating HEA microservices.
 
+## Version 1.5.3
+* When updating AWS temporary credentials, generate new headers rather than pass the headers from the HTTP request,
+possibly resulting in a Content-Length header that is shorter than the request body.
+* Make heaserver.service.db.aws.get_credentials raise the right exception.
+
 ## Version 1.5.2
 * Fixed TypeError regression in the heaserver.service.client module.
 
 ## Version 1.5.1
 * Ensure the Content-Type header is set to application/json in heaserver.service.client put and post calls.
 
 ## Version 1.5.0
```

### Comparing `heaserver-1.5.2/README.md` & `heaserver-1.5.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 # HEA Server Framework
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Server Framework contains shared code for creating HEA microservices.
 
+## Version 1.5.3
+* When updating AWS temporary credentials, generate new headers rather than pass the headers from the HTTP request,
+possibly resulting in a Content-Length header that is shorter than the request body.
+* Make heaserver.service.db.aws.get_credentials raise the right exception.
+
 ## Version 1.5.2
 * Fixed TypeError regression in the heaserver.service.client module.
 
 ## Version 1.5.1
 * Ensure the Content-Type header is set to application/json in heaserver.service.client put and post calls.
 
 ## Version 1.5.0
```

### Comparing `heaserver-1.5.2/RELEASING.md` & `heaserver-1.5.3/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/awss3integrationtests/heaserver/awss3tests/awss3foldertestcase.py` & `heaserver-1.5.3/awss3integrationtests/heaserver/awss3tests/awss3foldertestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/awss3integrationtests/heaserver/awss3tests/service.py` & `heaserver-1.5.3/awss3integrationtests/heaserver/awss3tests/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/awss3integrationtests/heaserver/awss3tests/test_all.py` & `heaserver-1.5.3/awss3integrationtests/heaserver/awss3tests/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/awss3integrationtests/heaserver/awss3tests/wstl/all.json` & `heaserver-1.5.3/awss3integrationtests/heaserver/awss3tests/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.16864` & `heaserver-1.5.3/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.16864`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.27996` & `heaserver-1.5.3/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.27996`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.5.3/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29888` & `heaserver-1.5.3/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29888`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.35312` & `heaserver-1.5.3/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.35312`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/awss3tests/heaserver/awss3tests/test_all.py` & `heaserver-1.5.3/awss3tests/heaserver/awss3tests/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.15624` & `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.15624`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160` & `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-310-pytest-7.4.0.pyc.28520` & `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-310-pytest-7.4.0.pyc.28520`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.15624` & `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.15624`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.41056` & `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.41056`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624` & `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.35160` & `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.35160`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.15624` & `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.15624`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.41056` & `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.41056`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-311-pytest-7.4.4.pyc.29500` & `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-311-pytest-7.4.4.pyc.29500`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-311-pytest-7.4.4.pyc.40780` & `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-311-pytest-7.4.4.pyc.40780`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.28520` & `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.28520`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160` & `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.28520` & `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.28520`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.35160` & `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.35160`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.41056` & `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.41056`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.24968` & `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.24968`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.28520` & `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.28520`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.41056` & `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.41056`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624` & `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.41056` & `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.41056`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/clienttestcase.py` & `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/clienttestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/componentpermissionstestcase.py` & `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/componentpermissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/componenttestcase.py` & `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/componenttestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/organizationpermissionstestcase.py` & `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/organizationpermissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/organizationtestcase.py` & `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/organizationtestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/service.py` & `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/test_client.py` & `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/test_client.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/test_component_with_bad_permissions.py` & `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/test_component_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/test_get_component.py` & `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/test_get_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/test_mongoservicelib.py` & `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/test_mongoservicelib.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/test_organization_with_bad_permissions.py` & `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/test_organization_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/test_post_component.py` & `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/test_post_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/integrationtests/heaserver/serviceintegrationtest/wstl/all.json` & `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/setup.py` & `heaserver-1.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='heaserver',
-      version='1.5.2',
+      version='1.5.3',
       description='The server side of HEA.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://risr.hci.utah.edu',
       author='Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT',
       author_email='Andrew.Post@hci.utah.edu',
       python_requires='>=3.10',
```

### Comparing `heaserver-1.5.2/src/heaserver/service/__init__.py` & `heaserver-1.5.3/src/heaserver/service/__init__.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/activity.py` & `heaserver-1.5.3/src/heaserver/service/activity.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/aiohttp.py` & `heaserver-1.5.3/src/heaserver/service/aiohttp.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/appfactory.py` & `heaserver-1.5.3/src/heaserver/service/appfactory.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/appproperty.py` & `heaserver-1.5.3/src/heaserver/service/appproperty.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/backgroundtasks.py` & `heaserver-1.5.3/src/heaserver/service/backgroundtasks.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/caching.py` & `heaserver-1.5.3/src/heaserver/service/caching.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/client.py` & `heaserver-1.5.3/src/heaserver/service/client.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/config.py` & `heaserver-1.5.3/src/heaserver/service/config.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/db/aws.py` & `heaserver-1.5.3/src/heaserver/service/db/aws.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from abc import ABC
 from functools import partial
 from aiohttp.web import Request
+from aiohttp import ClientResponseError
 import boto3
 import botocore
 from aiohttp import hdrs, web
 from botocore.exceptions import ClientError, ParamValidationError
 from mypy_boto3_s3 import S3Client, S3ServiceResource
 from mypy_boto3_sts import STSClient
 from mypy_boto3_account import AccountClient
@@ -74,16 +75,20 @@
         :returns: None if it succeeds otherwise it will raise ValueError or HTTPError
         :raises ValueError: if there was a problem accessing the registry service or the credentials service was not
         found.
         """
         if credentials.id is None:
             raise ValueError(f'credentials must have a non-None id attribute')
         resource_url = await type_to_resource_url(request, Credentials)
-        await client.put(app=request.app, url=URL(resource_url) / credentials.id, data=credentials,
-                         headers=request.headers)
+        headers = {SUB: request.headers.get(SUB, NONE_USER)}
+        try:
+            await client.put(app=request.app, url=URL(resource_url) / credentials.id, data=credentials,
+                            headers=headers)
+        except ClientResponseError as e:
+            raise ValueError(f'Updating credentials failed: {str(e)}') from e
 
     async def get_property(self, app: web.Application, name: str) -> Optional[Property]:
         """
         This is a wrapper function to be extended by tests
         Gets the Property with the given name from the HEA registry service.
 
         :param app: the aiohttp app.
@@ -201,15 +206,16 @@
 
     async def generate_cloud_credentials(self, request: Request, arn: str) -> AWSCredentials | None:
         """
         Create temporary credentials and return a newly created AWSCredentials object.
 
         :param request: the HTTP request (required).
         :param arn: The aws role arn that to be assumed
-        :returns the AWSCredentials populated with the resource's content, None if no such resource exists.
+        :returns an AWSCredentials object with the generated credentials, or None if the user doesn't have the provided
+        role.
         :raises ValueError: if an error occurs generating cloud credentials other than the user lacking permission.
         """
         return await _generate_cloud_credentials(request=request, arn=arn)
 
     async def get_credentials_from_volume(self, request: web.Request, volume_id: str) -> AWSCredentials | None:
         """
         Gets the volume's credentials.
@@ -294,14 +300,24 @@
 
         return account
 
     async def __get_resource_or_client(self, request: Request, service_name: str,
                                        creator: Callable[[str, str | None, str | None, str | None,
                                                           str | None], _S3Service],
                                        credentials: AWSCredentials | None) -> _S3Service:
+        """
+        Gets an S3 resource or client.
+
+        :param request: the HTTP request (required).
+        :param service_name: the name of the S3 service (required).
+        :param creator: the function for creating the resource or client (create_resource or create_client).
+        :param credentials: the AWSCredentials object, or None to let boto3 find the credentials.
+
+        :raises ValueError: if updating temporary credentials failed.
+        """
         logger = logging.getLogger(__name__)
         logger.debug("credentials retrieved from database checking if expired: %r", credentials)
         loop = asyncio.get_running_loop()
         if not credentials:  # delegate to boto3 to find the credentials
             return await loop.run_in_executor(None, creator, service_name)
         elif credentials.temporary:
             return await self.__get_temporary_credentials(request=request,
@@ -469,14 +485,16 @@
                   region_name: str | None = None,
                   aws_access_key_id: str | None = None,
                   aws_secret_access_key: str | None = None,
                   aws_session_token: str | None = None) -> S3Client | STSClient | AccountClient | OrganizationsClient:
     """
     Thread-safe boto client creation. Once created, clients are generally
     thread-safe.
+
+    :raises ValueError: if an error occurred getting the S3 client.
     """
     with _boto3_client_lock:
         return boto3.client(service_name,
                             region_name=region_name,
                             aws_access_key_id=aws_access_key_id,
                             aws_secret_access_key=aws_secret_access_key,
                             aws_session_token=aws_session_token,
@@ -487,30 +505,34 @@
                     region_name: str | None = None,
                     aws_access_key_id: str | None = None,
                     aws_secret_access_key: str | None = None,
                     aws_session_token: str | None = None) -> S3ServiceResource:
     """
     Thread-safe boto resource creation. Resources are generally NOT
     thread-safe!
+
+    :raises ValueError: if an error occurred getting the S3 resource.
     """
     with _boto3_resource_lock:
         return boto3.resource(service_name,
                               region_name=region_name,
                               aws_access_key_id=aws_access_key_id,
                               aws_secret_access_key=aws_secret_access_key,
-                              aws_session_token=aws_session_token)
+                              aws_session_token=aws_session_token,
+                              config=_boto3_client_config)
 
 
 async def _generate_cloud_credentials(request: Request, arn: str) -> AWSCredentials | None:
     """
     Create temporary credentials and return a newly created AWSCredentials object.
 
     :param request: the HTTP request (required).
     :param arn: The aws role arn that to be assumed
-    :returns the AWSCredentials populated with the resource's content, None if no such resource exists.
+    :returns an AWSCredentials object with the generated credentials, or None if the user doesn't have the provided
+    role.
     :raises ValueError: if an error occurs generating cloud credentials other than the user lacking permission.
     """
     logger = logging.getLogger(__name__)
     sub = request.headers.get(SUB, None)
     if sub is None:
         raise ValueError('OIDC SUB header is required')
     if not arn:
```

### Comparing `heaserver-1.5.2/src/heaserver/service/db/awsservicelib.py` & `heaserver-1.5.3/src/heaserver/service/db/awsservicelib.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/db/database.py` & `heaserver-1.5.3/src/heaserver/service/db/database.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/db/dbapi2.py` & `heaserver-1.5.3/src/heaserver/service/db/dbapi2.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/db/mongo.py` & `heaserver-1.5.3/src/heaserver/service/db/mongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/db/mongoexpr.py` & `heaserver-1.5.3/src/heaserver/service/db/mongoexpr.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/db/mongoservicelib.py` & `heaserver-1.5.3/src/heaserver/service/db/mongoservicelib.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/expression.py` & `heaserver-1.5.3/src/heaserver/service/expression.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/functional.py` & `heaserver-1.5.3/src/heaserver/service/functional.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/heaobjectsupport.py` & `heaserver-1.5.3/src/heaserver/service/heaobjectsupport.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/jsonschema.py` & `heaserver-1.5.3/src/heaserver/service/jsonschema.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/jsonschemafiles/__init__.py` & `heaserver-1.5.3/src/heaserver/service/jsonschemafiles/__init__.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/jsonschemafiles/cjtemplate.json` & `heaserver-1.5.3/src/heaserver/service/jsonschemafiles/cjtemplate.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/jsonschemafiles/wstl.json` & `heaserver-1.5.3/src/heaserver/service/jsonschemafiles/wstl.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/jsonschemafiles/wstlaction.json` & `heaserver-1.5.3/src/heaserver/service/jsonschemafiles/wstlaction.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/jsonschemavalidator.py` & `heaserver-1.5.3/src/heaserver/service/jsonschemavalidator.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/messagebroker.py` & `heaserver-1.5.3/src/heaserver/service/messagebroker.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/mimetypes.py` & `heaserver-1.5.3/src/heaserver/service/mimetypes.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/oidcclaimhdrs.py` & `heaserver-1.5.3/src/heaserver/service/oidcclaimhdrs.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/openapi.py` & `heaserver-1.5.3/src/heaserver/service/openapi.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/representor/__init__.py` & `heaserver-1.5.3/src/heaserver/service/representor/__init__.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/representor/cj.py` & `heaserver-1.5.3/src/heaserver/service/representor/cj.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/representor/factory.py` & `heaserver-1.5.3/src/heaserver/service/representor/factory.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/representor/nvpjson.py` & `heaserver-1.5.3/src/heaserver/service/representor/nvpjson.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/representor/representor.py` & `heaserver-1.5.3/src/heaserver/service/representor/representor.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/representor/wstljson.py` & `heaserver-1.5.3/src/heaserver/service/representor/wstljson.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/representor/xwwwformurlencoded.py` & `heaserver-1.5.3/src/heaserver/service/representor/xwwwformurlencoded.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/response.py` & `heaserver-1.5.3/src/heaserver/service/response.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/runner.py` & `heaserver-1.5.3/src/heaserver/service/runner.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/testcase/aiohttptestcase.py` & `heaserver-1.5.3/src/heaserver/service/testcase/aiohttptestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/testcase/awsdockermongo.py` & `heaserver-1.5.3/src/heaserver/service/testcase/awsdockermongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/testcase/awss3microservicetestcase.py` & `heaserver-1.5.3/src/heaserver/service/testcase/awss3microservicetestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/testcase/collection.py` & `heaserver-1.5.3/src/heaserver/service/testcase/collection.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/testcase/docker.py` & `heaserver-1.5.3/src/heaserver/service/testcase/docker.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/testcase/dockermongo.py` & `heaserver-1.5.3/src/heaserver/service/testcase/dockermongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/testcase/expectedvalues.py` & `heaserver-1.5.3/src/heaserver/service/testcase/expectedvalues.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/testcase/microservicetestcase.py` & `heaserver-1.5.3/src/heaserver/service/testcase/microservicetestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/testcase/mixin.py` & `heaserver-1.5.3/src/heaserver/service/testcase/mixin.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/testcase/mockaws.py` & `heaserver-1.5.3/src/heaserver/service/testcase/mockaws.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/testcase/mockdatabase.py` & `heaserver-1.5.3/src/heaserver/service/testcase/mockdatabase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/testcase/mockmongo.py` & `heaserver-1.5.3/src/heaserver/service/testcase/mockmongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/testcase/simpleaiohttptestcase.py` & `heaserver-1.5.3/src/heaserver/service/testcase/simpleaiohttptestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/testcase/swaggerui.py` & `heaserver-1.5.3/src/heaserver/service/testcase/swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/testcase/testenv.py` & `heaserver-1.5.3/src/heaserver/service/testcase/testenv.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/testcase/util.py` & `heaserver-1.5.3/src/heaserver/service/testcase/util.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/uritemplate.py` & `heaserver-1.5.3/src/heaserver/service/uritemplate.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/util.py` & `heaserver-1.5.3/src/heaserver/service/util.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver/service/wstl.py` & `heaserver-1.5.3/src/heaserver/service/wstl.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/src/heaserver.egg-info/PKG-INFO` & `heaserver-1.5.3/src/heaserver.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver
-Version: 1.5.2
+Version: 1.5.3
 Summary: The server side of HEA.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -47,14 +47,19 @@
 Requires-Dist: types-cachetools~=5.3.0
 
 # HEA Server Framework
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Server Framework contains shared code for creating HEA microservices.
 
+## Version 1.5.3
+* When updating AWS temporary credentials, generate new headers rather than pass the headers from the HTTP request,
+possibly resulting in a Content-Length header that is shorter than the request body.
+* Make heaserver.service.db.aws.get_credentials raise the right exception.
+
 ## Version 1.5.2
 * Fixed TypeError regression in the heaserver.service.client module.
 
 ## Version 1.5.1
 * Ensure the Content-Type header is set to application/json in heaserver.service.client put and post calls.
 
 ## Version 1.5.0
```

### Comparing `heaserver-1.5.2/src/heaserver.egg-info/SOURCES.txt` & `heaserver-1.5.3/src/heaserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.19788` & `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.19788`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_caching.cpython-311-pytest-7.4.4.pyc.29888` & `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_caching.cpython-311-pytest-7.4.4.pyc.29888`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.29888` & `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.29888`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.19788` & `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.19788`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.35312` & `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.35312`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.27996` & `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.27996`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35312` & `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35312`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/componentpermissionstestcase.py` & `heaserver-1.5.3/tests/heaserver/servicetest/componentpermissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/componenttestcase.py` & `heaserver-1.5.3/tests/heaserver/servicetest/componenttestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.27996` & `heaserver-1.5.3/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.27996`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.5.3/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.5.3/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.5.3/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.5.3/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/db/test_mongo.py` & `heaserver-1.5.3/tests/heaserver/servicetest/db/test_mongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/db/test_mongoexpr.py` & `heaserver-1.5.3/tests/heaserver/servicetest/db/test_mongoexpr.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/organizationpermissionstestcase.py` & `heaserver-1.5.3/tests/heaserver/servicetest/organizationpermissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/organizationtestcase.py` & `heaserver-1.5.3/tests/heaserver/servicetest/organizationtestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.27996` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.27996`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.28016` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.28016`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35228` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35228`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35312` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35312`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35444` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35444`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.37360` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.37360`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.35312` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.35312`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.19788` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.19788`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11224` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11224`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11864` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11864`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13080` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13080`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13852` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13852`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.15488` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.15488`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.1816` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.1816`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.19788` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.19788`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.28016` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.28016`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.30312` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.30312`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.34620` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.34620`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.37360` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.37360`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.16864` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.16864`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.19712` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.19712`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.23624` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.23624`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.29888` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.29888`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.4904` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.4904`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/all_cj_queries.json` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/all_cj_queries.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/all_cj_template.json` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/all_cj_template.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/test_cj.py` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/test_cj.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/test_factory.py` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/test_factory.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/test_nvpjson.py` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/test_nvpjson.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/test_wstljson.py` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/test_wstljson.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/representor/test_xwwwformurlencoded.py` & `heaserver-1.5.3/tests/heaserver/servicetest/representor/test_xwwwformurlencoded.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/service.py` & `heaserver-1.5.3/tests/heaserver/servicetest/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/test_activity.py` & `heaserver-1.5.3/tests/heaserver/servicetest/test_activity.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/test_aiohttp.py` & `heaserver-1.5.3/tests/heaserver/servicetest/test_aiohttp.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/test_backgroundtasks.py` & `heaserver-1.5.3/tests/heaserver/servicetest/test_backgroundtasks.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/test_caching.py` & `heaserver-1.5.3/tests/heaserver/servicetest/test_caching.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/test_client.py` & `heaserver-1.5.3/tests/heaserver/servicetest/test_client.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/test_component_with_bad_permissions.py` & `heaserver-1.5.3/tests/heaserver/servicetest/test_component_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/test_configuration.py` & `heaserver-1.5.3/tests/heaserver/servicetest/test_configuration.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/test_database_classes.py` & `heaserver-1.5.3/tests/heaserver/servicetest/test_database_classes.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/test_expression.py` & `heaserver-1.5.3/tests/heaserver/servicetest/test_expression.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/test_get_component.py` & `heaserver-1.5.3/tests/heaserver/servicetest/test_get_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/test_heaobjectsupport.py` & `heaserver-1.5.3/tests/heaserver/servicetest/test_heaobjectsupport.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/test_jsonschemavalidator.py` & `heaserver-1.5.3/tests/heaserver/servicetest/test_jsonschemavalidator.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/test_mimetypes.py` & `heaserver-1.5.3/tests/heaserver/servicetest/test_mimetypes.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/test_organization_with_bad_permissions.py` & `heaserver-1.5.3/tests/heaserver/servicetest/test_organization_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/test_post_component.py` & `heaserver-1.5.3/tests/heaserver/servicetest/test_post_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/test_put_component.py` & `heaserver-1.5.3/tests/heaserver/servicetest/test_put_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/test_response.py` & `heaserver-1.5.3/tests/heaserver/servicetest/test_response.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/test_testenv.py` & `heaserver-1.5.3/tests/heaserver/servicetest/test_testenv.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/test_uritemplate.py` & `heaserver-1.5.3/tests/heaserver/servicetest/test_uritemplate.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/test_util.py` & `heaserver-1.5.3/tests/heaserver/servicetest/test_util.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/test_wstl.py` & `heaserver-1.5.3/tests/heaserver/servicetest/test_wstl.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/wstl/all.json` & `heaserver-1.5.3/tests/heaserver/servicetest/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/wstl_1.json` & `heaserver-1.5.3/tests/heaserver/servicetest/wstl_1.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/wstl_10a.json` & `heaserver-1.5.3/tests/heaserver/servicetest/wstl_10a.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/wstl_10b.json` & `heaserver-1.5.3/tests/heaserver/servicetest/wstl_10b.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/wstl_11.json` & `heaserver-1.5.3/tests/heaserver/servicetest/wstl_11.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/wstl_2.json` & `heaserver-1.5.3/tests/heaserver/servicetest/wstl_2.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/wstl_3.json` & `heaserver-1.5.3/tests/heaserver/servicetest/wstl_3.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/wstl_4.json` & `heaserver-1.5.3/tests/heaserver/servicetest/wstl_4.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/wstl_6.json` & `heaserver-1.5.3/tests/heaserver/servicetest/wstl_6.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/wstl_7.json` & `heaserver-1.5.3/tests/heaserver/servicetest/wstl_7.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.2/tests/heaserver/servicetest/wstl_8.json` & `heaserver-1.5.3/tests/heaserver/servicetest/wstl_8.json`

 * *Files identical despite different names*

