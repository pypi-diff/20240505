# Comparing `tmp/saic_ismart_client_ng-0.2.1.tar.gz` & `tmp/saic_ismart_client_ng-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saic_ismart_client_ng-0.2.1.tar", last modified: Wed Apr 17 18:53:25 2024, max compression
+gzip compressed data, was "saic_ismart_client_ng-0.2.2.tar", last modified: Sun May  5 07:56:02 2024, max compression
```

## Comparing `saic_ismart_client_ng-0.2.1.tar` & `saic_ismart_client_ng-0.2.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:53:25.860362 saic_ismart_client_ng-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-17 18:53:25.860362 saic_ismart_client_ng-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 18:53:25.860362 saic_ismart_client_ng-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:53:25.852362 saic_ismart_client_ng-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:53:25.852362 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:53:25.856362 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10047 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:53:25.856362 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/message/
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/message/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/serialization_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:53:25.856362 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/user/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/user/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:53:25.856362 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/vehicle/
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/vehicle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:53:25.856362 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/vehicle/alarm/
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/vehicle/alarm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/vehicle/alarm/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:53:25.856362 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/vehicle/climate/
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/vehicle/climate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:53:25.856362 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/vehicle/locks/
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/vehicle/locks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/vehicle/locks/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/vehicle/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:53:25.856362 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/vehicle/windows/
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/vehicle/windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/vehicle/windows/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:53:25.856362 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/vehicle_charging/
--rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/vehicle_charging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15718 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/vehicle_charging/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/crypto_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:53:25.856362 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/net/
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:53:25.860362 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/net/client/
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/net/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/net/client/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/net/client/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/net/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/net/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:53:25.860362 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-17 18:53:25.000000 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-17 18:53:25.000000 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 18:53:25.000000 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-17 18:53:25.000000 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-17 18:53:25.000000 saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:53:25.860362 saic_ismart_client_ng-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/tests/test_charge_info_resp.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/tests/test_charging_setting_resp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/tests/test_decode_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/tests/test_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-17 18:53:21.000000 saic_ismart_client_ng-0.2.1/tests/test_vehicle_control_resp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:56:02.198877 saic_ismart_client_ng-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-05 07:56:02.198877 saic_ismart_client_ng-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 07:56:02.198877 saic_ismart_client_ng-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:56:02.190878 saic_ismart_client_ng-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:56:02.194877 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:56:02.194877 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10047 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:56:02.194877 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/message/
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/message/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/serialization_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:56:02.194877 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/user/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:56:02.194877 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/vehicle/
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/vehicle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:56:02.194877 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/vehicle/alarm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/vehicle/alarm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/vehicle/alarm/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:56:02.198877 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/vehicle/climate/
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/vehicle/climate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:56:02.198877 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/vehicle/locks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/vehicle/locks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/vehicle/locks/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/vehicle/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:56:02.198877 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/vehicle/windows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/vehicle/windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/vehicle/windows/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:56:02.198877 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/vehicle_charging/
+-rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/vehicle_charging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15718 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/vehicle_charging/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/crypto_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:56:02.198877 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/net/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:56:02.198877 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/net/client/
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/net/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/net/client/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/net/client/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/net/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/net/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:56:02.198877 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-05 07:56:02.000000 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-05 07:56:02.000000 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 07:56:02.000000 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-05 07:56:02.000000 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-05 07:56:02.000000 saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:56:02.198877 saic_ismart_client_ng-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/tests/test_charge_info_resp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/tests/test_charging_setting_resp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/tests/test_decode_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/tests/test_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-05 07:55:58.000000 saic_ismart_client_ng-0.2.2/tests/test_vehicle_control_resp.py
```

### Comparing `saic_ismart_client_ng-0.2.1/LICENSE` & `saic_ismart_client_ng-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.2.1/PKG-INFO` & `saic_ismart_client_ng-0.2.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saic_ismart_client_ng
-Version: 0.2.1
+Version: 0.2.2
 Summary: SAIC next gen client library (MG iSMART)
 Author-email: Giovanni Condello <saic-python-client@nanomad.net>
 Project-URL: Homepage, https://github.com/SAIC-iSmart-API/saic-python-client-ng
 Project-URL: Bug Tracker, https://github.com/SAIC-iSmart-API/saic-python-client-ng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `saic_ismart_client_ng-0.2.1/pyproject.toml` & `saic_ismart_client_ng-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "saic_ismart_client_ng"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
     { name = "Giovanni Condello", email = "saic-python-client@nanomad.net" },
 ]
 dependencies = [
     "pycryptodome>=3.20.0",
     "httpx>=0.26.0",
     "tenacity>=8.2.3",
```

### Comparing `saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/__init__.py` & `saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/__init__.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/base.py` & `saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/base.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/message/__init__.py` & `saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/message/__init__.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/message/schema.py` & `saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/message/schema.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/schema.py` & `saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/schema.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/serialization_utils.py` & `saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/serialization_utils.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/vehicle/__init__.py` & `saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/vehicle/__init__.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/vehicle/alarm/__init__.py` & `saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/vehicle/alarm/__init__.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/vehicle/alarm/schema.py` & `saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/vehicle/alarm/schema.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/vehicle/climate/__init__.py` & `saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/vehicle/climate/__init__.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/vehicle/locks/__init__.py` & `saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/vehicle/locks/__init__.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/vehicle/schema.py` & `saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/vehicle/schema.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/vehicle/windows/__init__.py` & `saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/vehicle/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/vehicle_charging/__init__.py` & `saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/vehicle_charging/__init__.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/api/vehicle_charging/schema.py` & `saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/api/vehicle_charging/schema.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/crypto_utils.py` & `saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/crypto_utils.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/exceptions.py` & `saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/exceptions.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/model.py` & `saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/net/client/__init__.py` & `saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/net/client/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,35 +28,35 @@
         try:
             body = None
             if request.content:
                 try:
 
                     body = request.content.decode("utf-8")
                 except Exception as e:
-                    self.__logger.warning(f"Error decoding request content: {e}")
+                    self.__logger.warning(f"Error decoding request content: {e}", exc_info=e)
 
             await self.__listener.on_request(
                 path=str(request.url).replace(self.configuration.base_uri, "/"),
                 body=body,
                 headers=dict(request.headers),
             )
         except Exception as e:
-            self.__logger.warning(f"Error invoking request listener: {e}")
+            self.__logger.warning(f"Error invoking request listener: {e}", exc_info=e)
 
     async def invoke_response_listener(self, response: httpx.Response):
         if not self.__listener:
             return
         try:
             body = await response.aread()
             if body:
                 try:
                     body = body.decode("utf-8")
                 except Exception as e:
-                    self.__logger.warning(f"Error decoding request content: {e}")
+                    self.__logger.warning(f"Error decoding request content: {e}", exc_info=e)
 
             await self.__listener.on_response(
                 path=str(response.url).replace(self.configuration.base_uri, "/"),
                 body=body,
                 headers=dict(response.headers),
             )
         except Exception as e:
-            self.__logger.warning(f"Error invoking request listener: {e}")
+            self.__logger.warning(f"Error invoking request listener: {e}", exc_info=e)
```

### Comparing `saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/net/client/api.py` & `saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/net/client/api.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/net/client/login.py` & `saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/net/client/login.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng/net/security.py` & `saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng/net/security.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng.egg-info/PKG-INFO` & `saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saic_ismart_client_ng
-Version: 0.2.1
+Version: 0.2.2
 Summary: SAIC next gen client library (MG iSMART)
 Author-email: Giovanni Condello <saic-python-client@nanomad.net>
 Project-URL: Homepage, https://github.com/SAIC-iSmart-API/saic-python-client-ng
 Project-URL: Bug Tracker, https://github.com/SAIC-iSmart-API/saic-python-client-ng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `saic_ismart_client_ng-0.2.1/src/saic_ismart_client_ng.egg-info/SOURCES.txt` & `saic_ismart_client_ng-0.2.2/src/saic_ismart_client_ng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.2.1/tests/test_charge_info_resp.py` & `saic_ismart_client_ng-0.2.2/tests/test_charge_info_resp.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.2.1/tests/test_charging_setting_resp.py` & `saic_ismart_client_ng-0.2.2/tests/test_charging_setting_resp.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.2.1/tests/test_decode_messages.py` & `saic_ismart_client_ng-0.2.2/tests/test_decode_messages.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.2.1/tests/test_listener.py` & `saic_ismart_client_ng-0.2.2/tests/test_listener.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.2.1/tests/test_model.py` & `saic_ismart_client_ng-0.2.2/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.2.1/tests/test_vehicle_control_resp.py` & `saic_ismart_client_ng-0.2.2/tests/test_vehicle_control_resp.py`

 * *Files identical despite different names*

