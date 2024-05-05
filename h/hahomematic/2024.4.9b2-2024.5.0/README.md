# Comparing `tmp/hahomematic-2024.4.9b2.tar.gz` & `tmp/hahomematic-2024.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hahomematic-2024.4.9b2.tar", last modified: Wed Apr 17 09:22:17 2024, max compression
+gzip compressed data, was "hahomematic-2024.5.0.tar", last modified: Sun May  5 06:54:23 2024, max compression
```

## Comparing `hahomematic-2024.4.9b2.tar` & `hahomematic-2024.5.0.tar`

### file list

```diff
@@ -1,108 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:17.706777 hahomematic-2024.4.9b2/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-17 09:22:17.706777 hahomematic-2024.4.9b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:17.690777 hahomematic-2024.4.9b2/hahomematic/
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/async_support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:17.694777 hahomematic-2024.4.9b2/hahomematic/caches/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18623 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/caches/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)    17216 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/caches/persistent.py
--rw-r--r--   0 runner    (1001) docker     (127)    27542 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/caches/visibility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:17.694777 hahomematic-2024.4.9b2/hahomematic/central/
--rw-r--r--   0 runner    (1001) docker     (127)    54211 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/central/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/central/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/central/xml_rpc_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:17.694777 hahomematic-2024.4.9b2/hahomematic/client/
--rw-r--r--   0 runner    (1001) docker     (127)    42079 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34886 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/client/json_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/client/xml_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14686 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/hmcli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/performance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:17.694777 hahomematic-2024.4.9b2/hahomematic/platforms/
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:17.698777 hahomematic-2024.4.9b2/hahomematic/platforms/custom/
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26219 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/custom/climate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/custom/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    25593 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/custom/cover.py
--rw-r--r--   0 runner    (1001) docker     (127)    30029 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/custom/definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    12704 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/custom/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)    44592 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/custom/light.py
--rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/custom/lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/custom/siren.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/custom/support.py
--rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/custom/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    33530 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    29231 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:17.698777 hahomematic-2024.4.9b2/hahomematic/platforms/generic/
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/generic/action.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/generic/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/generic/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/generic/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/generic/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/generic/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/generic/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/generic/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/generic/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:17.698777 hahomematic-2024.4.9b2/hahomematic/platforms/hub/
--rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/hub/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/hub/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/hub/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/hub/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/hub/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/hub/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/hub/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/hub/text.py
--rw-r--r--   0 runner    (1001) docker     (127)    14073 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/support.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/update.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:17.702777 hahomematic-2024.4.9b2/hahomematic/rega_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/rega_scripts/fetch_all_device_data.fn
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/rega_scripts/get_serial.fn
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/rega_scripts/set_system_variable.fn
--rw-r--r--   0 runner    (1001) docker     (127)     9533 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:17.706777 hahomematic-2024.4.9b2/hahomematic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-17 09:22:17.000000 hahomematic-2024.4.9b2/hahomematic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-17 09:22:17.000000 hahomematic-2024.4.9b2/hahomematic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:22:17.000000 hahomematic-2024.4.9b2/hahomematic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:22:17.000000 hahomematic-2024.4.9b2/hahomematic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-17 09:22:17.000000 hahomematic-2024.4.9b2/hahomematic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-17 09:22:17.000000 hahomematic-2024.4.9b2/hahomematic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:17.702777 hahomematic-2024.4.9b2/hahomematic_support/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10649 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic_support/client_local.py
--rw-r--r--   0 runner    (1001) docker     (127)    18953 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-17 09:22:17.706777 hahomematic-2024.4.9b2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:17.706777 hahomematic-2024.4.9b2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_button.py
--rw-r--r--   0 runner    (1001) docker     (127)    26329 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_central.py
--rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_central_pydevccu.py
--rw-r--r--   0 runner    (1001) docker     (127)    14900 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_climate.py
--rw-r--r--   0 runner    (1001) docker     (127)    26891 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_cover.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_json_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    32422 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_siren.py
--rw-r--r--   0 runner    (1001) docker     (127)    15478 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:54:23.146227 hahomematic-2024.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-05 06:54:23.146227 hahomematic-2024.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:54:23.134227 hahomematic-2024.5.0/hahomematic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/async_support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:54:23.134227 hahomematic-2024.5.0/hahomematic/caches/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18130 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/caches/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17216 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/caches/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27542 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/caches/visibility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:54:23.134227 hahomematic-2024.5.0/hahomematic/central/
+-rw-r--r--   0 runner    (1001) docker     (127)    54833 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/central/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/central/command_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/central/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9173 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/central/xml_rpc_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:54:23.138227 hahomematic-2024.5.0/hahomematic/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    46091 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34886 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/client/json_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7684 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/client/xml_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14924 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/hmcli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/performance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:54:23.138227 hahomematic-2024.5.0/hahomematic/platforms/
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:54:23.138227 hahomematic-2024.5.0/hahomematic/platforms/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26229 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/custom/climate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/custom/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24631 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/custom/cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30099 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/custom/definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12859 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/custom/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44054 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/custom/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/custom/lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9526 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/custom/siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/custom/support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/custom/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33380 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30606 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:54:23.142227 hahomematic-2024.5.0/hahomematic/platforms/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/generic/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/generic/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/generic/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/generic/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/generic/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/generic/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/generic/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/generic/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/generic/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:54:23.142227 hahomematic-2024.5.0/hahomematic/platforms/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)     8981 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/hub/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/hub/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/hub/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/hub/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/hub/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/hub/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/hub/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/hub/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14073 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:54:23.142227 hahomematic-2024.5.0/hahomematic/rega_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/rega_scripts/fetch_all_device_data.fn
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/rega_scripts/get_serial.fn
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/rega_scripts/set_system_variable.fn
+-rw-r--r--   0 runner    (1001) docker     (127)     9705 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:54:23.146227 hahomematic-2024.5.0/hahomematic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-05 06:54:23.000000 hahomematic-2024.5.0/hahomematic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-05-05 06:54:23.000000 hahomematic-2024.5.0/hahomematic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 06:54:23.000000 hahomematic-2024.5.0/hahomematic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 06:54:22.000000 hahomematic-2024.5.0/hahomematic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-05 06:54:23.000000 hahomematic-2024.5.0/hahomematic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-05 06:54:23.000000 hahomematic-2024.5.0/hahomematic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:54:23.142227 hahomematic-2024.5.0/hahomematic_support/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11147 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic_support/client_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18951 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-05 06:54:23.146227 hahomematic-2024.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:54:23.146227 hahomematic-2024.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32324 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_central.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_central_pydevccu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16791 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_climate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33275 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_json_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39142 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17156 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_text.py
```

### Comparing `hahomematic-2024.4.9b2/LICENSE` & `hahomematic-2024.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b2/PKG-INFO` & `hahomematic-2024.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2024.4.9b2
+Version: 2024.5.0
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2024.4.9b2/README.md` & `hahomematic-2024.5.0/README.md`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b2/hahomematic/__init__.py` & `hahomematic-2024.5.0/hahomematic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b2/hahomematic/async_support.py` & `hahomematic-2024.5.0/hahomematic/async_support.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import asyncio
 from collections.abc import Callable, Collection, Coroutine
 from concurrent.futures import ThreadPoolExecutor
 from concurrent.futures._base import CancelledError
 from functools import wraps
 import logging
 from time import monotonic
-from typing import Any, Final, ParamSpec, TypeVar
+from typing import Any, Final, ParamSpec, TypeVar, cast
 
 from hahomematic.const import BLOCK_LOG_TIMEOUT
 from hahomematic.exceptions import HaHomematicException
 from hahomematic.support import debug_enabled, reduce_args
 
 _LOGGER: Final = logging.getLogger(__name__)
 _P = ParamSpec("_P")
@@ -142,8 +142,8 @@
             _LOGGER.warning(
                 "Method %s must run in the event_loop. No loop detected.", func.__name__
             )
 
         return return_value
 
     setattr(func, "_loop_check", True)
-    return wrapper_loop_check if debug_enabled() else func
+    return cast(Callable[_P, _R], wrapper_loop_check) if debug_enabled() else func
```

### Comparing `hahomematic-2024.4.9b2/hahomematic/caches/dynamic.py` & `hahomematic-2024.5.0/hahomematic/caches/dynamic.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,147 +10,119 @@
 from hahomematic import central as hmcu
 from hahomematic.config import (
     LAST_COMMAND_SEND_STORE_TIMEOUT,
     PING_PONG_MISMATCH_COUNT,
     PING_PONG_MISMATCH_COUNT_TTL,
 )
 from hahomematic.const import (
+    ENTITY_KEY,
     EVENT_DATA,
     EVENT_INSTANCE_NAME,
     EVENT_INTERFACE_ID,
     EVENT_PONG_MISMATCH_COUNT,
     EVENT_TYPE,
     INIT_DATETIME,
     MAX_CACHE_AGE,
     NO_CACHE_ENTRY,
     CallSource,
-    EventType,
+    HomematicEventType,
     InterfaceEventType,
     InterfaceName,
     ParamsetKey,
 )
 from hahomematic.converter import CONVERTABLE_PARAMETERS, convert_combined_parameter_to_paramset
 from hahomematic.platforms.device import HmDevice
-from hahomematic.support import changed_within_seconds, get_channel_no, get_device_address
+from hahomematic.support import changed_within_seconds, get_entity_key
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 
 class CommandCache:
     """Cache for send commands."""
 
     def __init__(self, interface_id: str) -> None:
         """Init command cache."""
         self._interface_id: Final = interface_id
         # (paramset_key, device_address, channel_no, parameter)
-        self._last_send_command: Final[
-            dict[tuple[str, str, int | None, str], tuple[Any, datetime]]
-        ] = {}
+        self._last_send_command: Final[dict[ENTITY_KEY, tuple[Any, datetime]]] = {}
 
     def add_set_value(
         self,
         channel_address: str,
         parameter: str,
         value: Any,
-    ) -> None:
+    ) -> set[ENTITY_KEY]:
         """Add data from set value command."""
         if parameter in CONVERTABLE_PARAMETERS:
-            self.add_combined_parameter(
+            return self.add_combined_parameter(
                 parameter=parameter, channel_address=channel_address, combined_parameter=value
             )
-            return
 
-        key = (
-            ParamsetKey.VALUES.value,
-            get_device_address(channel_address),
-            get_channel_no(channel_address),
-            parameter,
+        entity_key = get_entity_key(
+            channel_address=channel_address,
+            parameter=parameter,
         )
-        self._last_send_command[key] = (value, datetime.now())
+        self._last_send_command[entity_key] = (value, datetime.now())
+        return {entity_key}
 
     def add_put_paramset(
-        self,
-        channel_address: str,
-        paramset_key: str,
-        values: dict[str, Any],
-    ) -> None:
+        self, channel_address: str, paramset_key: str, values: dict[str, Any]
+    ) -> set[ENTITY_KEY]:
         """Add data from put paramset command."""
-
+        entity_keys: set[ENTITY_KEY] = set()
         for parameter, value in values.items():
-            key = (
-                paramset_key,
-                get_device_address(channel_address),
-                get_channel_no(channel_address),
-                parameter,
+            entity_key = get_entity_key(
+                channel_address=channel_address,
+                parameter=parameter,
             )
-            self._last_send_command[key] = (value, datetime.now())
+            self._last_send_command[entity_key] = (value, datetime.now())
+            entity_keys.add(entity_key)
+        return entity_keys
 
     def add_combined_parameter(
         self, parameter: str, channel_address: str, combined_parameter: str
-    ) -> None:
+    ) -> set[ENTITY_KEY]:
         """Add data from combined parameter."""
         if values := convert_combined_parameter_to_paramset(
             parameter=parameter, cpv=combined_parameter
         ):
-            self.add_put_paramset(
+            return self.add_put_paramset(
                 channel_address=channel_address,
-                paramset_key=ParamsetKey.VALUES.value,
+                paramset_key=ParamsetKey.VALUES,
                 values=values,
             )
+        return set()
 
     def get_last_value_send(
-        self,
-        paramset_key: str,
-        channel_address: str,
-        parameter: str,
-        max_age: int = LAST_COMMAND_SEND_STORE_TIMEOUT,
+        self, entity_key: ENTITY_KEY, max_age: int = LAST_COMMAND_SEND_STORE_TIMEOUT
     ) -> Any:
         """Return the last send values."""
-        key = (
-            paramset_key,
-            get_device_address(channel_address),
-            get_channel_no(channel_address),
-            parameter,
-        )
-        if result := self._last_send_command.get(key):
+        if result := self._last_send_command.get(entity_key):
             value, last_send_dt = result
             if last_send_dt and changed_within_seconds(last_change=last_send_dt, max_age=max_age):
                 return value
             self.remove_last_value_send(
-                paramset_key=paramset_key,
-                channel_address=channel_address,
-                parameter=parameter,
+                entity_key=entity_key,
                 max_age=max_age,
             )
         return None
 
     def remove_last_value_send(
         self,
-        paramset_key: str,
-        channel_address: str,
-        parameter: str,
+        entity_key: ENTITY_KEY,
         value: Any = None,
         max_age: int = LAST_COMMAND_SEND_STORE_TIMEOUT,
     ) -> None:
         """Remove the last send value."""
-        key = (
-            paramset_key,
-            get_device_address(channel_address),
-            get_channel_no(channel_address),
-            parameter,
-        )
-
-        if result := self._last_send_command.get(key):
+        if result := self._last_send_command.get(entity_key):
             stored_value, last_send_dt = result
-            if changed_within_seconds(last_change=last_send_dt, max_age=max_age) or (
-                value and stored_value != value
+            if not changed_within_seconds(last_change=last_send_dt, max_age=max_age) or (
+                value is not None and stored_value == value
             ):
-                return
-
-            del self._last_send_command[key]
+                del self._last_send_command[entity_key]
 
 
 class DeviceDetailsCache:
     """Cache for device/channel details."""
 
     def __init__(self, central: hmcu.CentralUnit) -> None:
         """Init the device details cache."""
@@ -446,16 +418,16 @@
 
     def _check_and_fire_pong_event(
         self, event_type: InterfaceEventType, pong_mismatch_count: int
     ) -> None:
         """Fire an event about the pong status."""
 
         def _fire_event(mismatch_count: int) -> None:
-            self._central.fire_ha_event_callback(
-                event_type=EventType.INTERFACE,
+            self._central.fire_homematic_callback(
+                event_type=HomematicEventType.INTERFACE,
                 event_data=cast(
                     dict[str, Any],
                     hmcu.INTERFACE_EVENT_SCHEMA(
                         {
                             EVENT_INTERFACE_ID: self._interface_id,
                             EVENT_TYPE: event_type,
                             EVENT_DATA: {
```

### Comparing `hahomematic-2024.4.9b2/hahomematic/caches/persistent.py` & `hahomematic-2024.5.0/hahomematic/caches/persistent.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b2/hahomematic/caches/visibility.py` & `hahomematic-2024.5.0/hahomematic/caches/visibility.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b2/hahomematic/central/__init__.py` & `hahomematic-2024.5.0/hahomematic/central/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 """
 
 from __future__ import annotations
 
 import asyncio
 from collections.abc import Callable, Coroutine, Mapping, Set as AbstractSet
 from datetime import datetime
+from functools import partial
 import logging
 import socket
 import threading
 from time import sleep
 from typing import Any, Final, cast
 
 from aiohttp import ClientSession
@@ -21,56 +22,59 @@
 
 from hahomematic import client as hmcl, config
 from hahomematic.async_support import Looper, loop_check
 from hahomematic.caches.dynamic import CentralDataCache, DeviceDetailsCache
 from hahomematic.caches.persistent import DeviceDescriptionCache, ParamsetDescriptionCache
 from hahomematic.caches.visibility import ParameterVisibilityCache
 from hahomematic.central import xml_rpc_server as xmlrpc
-from hahomematic.central.decorators import callback_event, callback_system_event
+from hahomematic.central.command_queue import CommandQueueHandler
+from hahomematic.central.decorators import callback_backend_system, callback_event
 from hahomematic.client.json_rpc import JsonRpcAioHttpClient
 from hahomematic.client.xml_rpc import XmlRpcProxy
 from hahomematic.const import (
+    CALLBACK_TYPE,
     DATETIME_FORMAT_MILLIS,
     DEFAULT_TLS,
     DEFAULT_VERIFY_TLS,
     ENTITY_EVENTS,
+    ENTITY_KEY,
     EVENT_AVAILABLE,
     EVENT_DATA,
     EVENT_INTERFACE_ID,
     EVENT_TYPE,
+    BackendSystemEvent,
     Description,
     DeviceFirmwareState,
-    EventType,
     HmPlatform,
+    HomematicEventType,
     InterfaceEventType,
     InterfaceName,
     Parameter,
     ParamsetKey,
     ProxyInitState,
-    SystemEvent,
     SystemInformation,
 )
 from hahomematic.exceptions import (
     BaseHomematicException,
     HaHomematicConfigException,
     HaHomematicException,
     NoClients,
     NoConnection,
 )
 from hahomematic.performance import measure_execution_time
 from hahomematic.platforms import create_entities_and_append_to_device
 from hahomematic.platforms.custom.entity import CustomEntity
 from hahomematic.platforms.device import HmDevice
-from hahomematic.platforms.entity import BaseEntity, CallbackEntity
+from hahomematic.platforms.entity import BaseParameterEntity, CallbackEntity
 from hahomematic.platforms.event import GenericEvent
 from hahomematic.platforms.generic.entity import GenericEntity
 from hahomematic.platforms.hub import Hub
 from hahomematic.platforms.hub.button import HmProgramButton
 from hahomematic.platforms.hub.entity import GenericHubEntity, GenericSystemVariable
-from hahomematic.support import check_config, get_device_address, reduce_args
+from hahomematic.support import check_config, get_device_address, get_entity_key, reduce_args
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 # {instance_name, central}
 CENTRAL_INSTANCES: Final[dict[str, CentralUnit]] = {}
 ConnectionProblemIssuer = JsonRpcAioHttpClient | XmlRpcProxy
 
@@ -126,38 +130,39 @@
         )
 
         self._primary_client: hmcl.Client | None = None
         # {interface_id, client}
         self._clients: Final[dict[str, hmcl.Client]] = {}
         # {{channel_address, parameter}, event_handle}
         self._entity_event_subscriptions: Final[
-            dict[tuple[str, str], list[Callable[[Any], Coroutine[Any, Any, None]]]]
+            dict[ENTITY_KEY, list[Callable[[Any], Coroutine[Any, Any, None]]]]
         ] = {}
         # {device_address, device}
         self._devices: Final[dict[str, HmDevice]] = {}
         # {sysvar_name, sysvar_entity}
         self._sysvar_entities: Final[dict[str, GenericSystemVariable]] = {}
         # {sysvar_name, program_button}U
         self._program_buttons: Final[dict[str, HmProgramButton]] = {}
         # store last event received datetime by interface
         self.last_events: Final[dict[str, datetime]] = {}
         # Signature: (name, *args)
         # e.g. DEVICES_CREATED, HUB_REFRESHED
-        self._system_event_callbacks: Final[set[Callable]] = set()
+        self._backend_system_callbacks: Final[set[Callable]] = set()
         # Signature: (interface_id, channel_address, parameter, value)
         # Re-Fired events from CCU for parameter updates
-        self._entity_event_callbacks: Final[set[Callable]] = set()
+        self._backend_parameter_callbacks: Final[set[Callable]] = set()
         # Signature: (event_type, event_data)
         # Events like INTERFACE, KEYPRESS, ...
-        self._ha_event_callbacks: Final[set[Callable]] = set()
+        self._homematic_callbacks: Final[set[Callable]] = set()
 
         self.json_rpc_client: Final[JsonRpcAioHttpClient] = central_config.create_json_rpc_client()
 
         CENTRAL_INSTANCES[self._name] = self
-        self._connection_checker: Final = ConnectionChecker(self)
+        self._connection_checker: Final = ConnectionChecker(central=self)
+        self._command_queue_handler: Final = CommandQueueHandler()
         self._hub: Hub = Hub(central=self)
         self._version: str | None = None
 
     @property
     def available(self) -> bool:
         """Return the availability of the central."""
         return all(client.available for client in self._clients.values())
@@ -228,14 +233,19 @@
 
     @property
     def name(self) -> str:
         """Return the name of the backend."""
         return self._name
 
     @property
+    def command_queue_handler(self) -> CommandQueueHandler:
+        """Return the que handler for send commands."""
+        return self._command_queue_handler
+
+    @property
     def started(self) -> bool:
         """Return if the central is started."""
         return self._started
 
     @property
     def supports_ping_pong(self) -> bool:
         """Return the backend supports ping pong."""
@@ -299,14 +309,15 @@
             if await self._create_clients():
                 for client in self._clients.values():
                     await self._refresh_device_descriptions(client=client)
         else:
             await self._start_clients()
             if self.config.enable_server:
                 self._start_connection_checker()
+
         self._started = True
 
     async def stop(self) -> None:
         """Stop processing of the central unit."""
         if not self._started:
             _LOGGER.debug("STOP: Central %s not started", self._name)
             return
@@ -328,14 +339,16 @@
                 "There is still another central instance registered"
             )
 
         _LOGGER.debug("STOP: Removing instance")
         if self._name in CENTRAL_INSTANCES:
             del CENTRAL_INSTANCES[self._name]
 
+        await self._command_queue_handler.stop()
+
         # wait until tasks are finished
         await self.looper.block_till_done()
 
         while self._has_active_threads:
             await asyncio.sleep(1)
         self._started = False
 
@@ -486,16 +499,16 @@
         data = data or {}
         event_data: dict[str, Any] = {
             EVENT_INTERFACE_ID: interface_id,
             EVENT_TYPE: interface_event_type,
             EVENT_DATA: data,
         }
 
-        self.fire_ha_event_callback(
-            event_type=EventType.INTERFACE,
+        self.fire_homematic_callback(
+            event_type=HomematicEventType.INTERFACE,
             event_data=cast(dict[str, Any], INTERFACE_EVENT_SCHEMA(event_data)),
         )
 
     async def _identify_callback_ip(self, port: int) -> str:
         """Identify local IP used for callbacks."""
 
         # Do not add: pylint disable=no-member
@@ -634,15 +647,15 @@
             he
             for he in (self.program_buttons + self.sysvar_entities)
             if (platform is None or he.platform == platform)
             and (registered is None or he.is_registered == registered)
         )
 
     def get_channel_events(
-        self, event_type: EventType, registered: bool | None = None
+        self, event_type: HomematicEventType, registered: bool | None = None
     ) -> tuple[list[GenericEvent], ...]:
         """Return all channel event entities."""
         hm_channel_events: list[list[GenericEvent]] = []
         for device in self.devices:
             for channel_events in device.get_channel_events(event_type=event_type).values():
                 if registered is None or (channel_events[0].is_registered == registered):
                     hm_channel_events.append(channel_events)
@@ -733,16 +746,16 @@
                         device_address,
                     )
         _LOGGER.debug("CREATE_DEVICES: Finished creating devices for %s", self._name)
 
         if new_devices:
             new_entities = _get_new_entities(new_devices=new_devices)
             new_channel_events = _get_new_channel_events(new_devices=new_devices)
-            self.fire_system_event_callback(
-                system_event=SystemEvent.DEVICES_CREATED,
+            self.fire_backend_system_callback(
+                system_event=BackendSystemEvent.DEVICES_CREATED,
                 new_entities=new_entities,
                 new_channel_events=new_channel_events,
             )
 
     async def delete_device(self, interface_id: str, device_address: str) -> None:
         """Delete devices from central."""
         _LOGGER.debug(
@@ -754,27 +767,27 @@
         if (device := self._devices.get(device_address)) is None:
             return
         addresses = device.channel_addresses
         addresses += (device_address,)
 
         await self.delete_devices(interface_id=interface_id, addresses=addresses)
 
-    @callback_system_event(system_event=SystemEvent.DELETE_DEVICES)
+    @callback_backend_system(system_event=BackendSystemEvent.DELETE_DEVICES)
     async def delete_devices(self, interface_id: str, addresses: tuple[str, ...]) -> None:
         """Delete devices from central."""
         _LOGGER.debug(
             "DELETE_DEVICES: interface_id = %s, addresses = %s",
             interface_id,
             str(addresses),
         )
         for address in addresses:
             if device := self._devices.get(address):
                 await self.remove_device(device=device)
 
-    @callback_system_event(system_event=SystemEvent.NEW_DEVICES)
+    @callback_backend_system(system_event=BackendSystemEvent.NEW_DEVICES)
     async def add_new_devices(
         self, interface_id: str, device_descriptions: tuple[dict[str, Any], ...]
     ) -> None:
         """Add new devices to central unit."""
         await self._add_new_devices(
             interface_id=interface_id, device_descriptions=device_descriptions
         )
@@ -846,17 +859,23 @@
                     and (client := self.get_client(interface_id=interface_id))
                     and client.supports_ping_pong
                 ):
                     client.ping_pong_cache.handle_received_pong(
                         pong_ts=datetime.strptime(v_timestamp, DATETIME_FORMAT_MILLIS)
                     )
             return
-        if (channel_address, parameter) in self._entity_event_subscriptions:
+
+        entity_key = get_entity_key(
+            channel_address=channel_address,
+            parameter=parameter,
+        )
+
+        if entity_key in self._entity_event_subscriptions:
             try:
-                for callback in self._entity_event_subscriptions[(channel_address, parameter)]:
+                for callback in self._entity_event_subscriptions[entity_key]:
                     await callback(value)
             except RuntimeError as rte:  # pragma: no cover
                 _LOGGER.debug(
                     "EVENT: RuntimeError [%s]. Failed to call callback for: %s, %s, %s",
                     reduce_args(args=rte.args),
                     interface_id,
                     channel_address,
@@ -867,34 +886,29 @@
                     "EVENT failed: Unable to call callback for: %s, %s, %s, %s",
                     interface_id,
                     channel_address,
                     parameter,
                     reduce_args(args=ex.args),
                 )
 
-    @callback_system_event(system_event=SystemEvent.LIST_DEVICES)
+    @callback_backend_system(system_event=BackendSystemEvent.LIST_DEVICES)
     def list_devices(self, interface_id: str) -> list[dict[str, Any]]:
         """Return already existing devices to CCU / Homegear."""
         result = self.device_descriptions.get_raw_device_descriptions(interface_id=interface_id)
         _LOGGER.debug(
             "LIST_DEVICES: interface_id = %s, channel_count = %i", interface_id, len(result)
         )
         return result
 
-    def add_event_subscription(self, entity: BaseEntity) -> None:
+    def add_event_subscription(self, entity: BaseParameterEntity) -> None:
         """Add entity to central event subscription."""
         if isinstance(entity, (GenericEntity, GenericEvent)) and entity.supports_events:
-            if (
-                entity.channel_address,
-                entity.parameter,
-            ) not in self._entity_event_subscriptions:
-                self._entity_event_subscriptions[(entity.channel_address, entity.parameter)] = []
-            self._entity_event_subscriptions[(entity.channel_address, entity.parameter)].append(
-                entity.event
-            )
+            if entity.entity_key not in self._entity_event_subscriptions:
+                self._entity_event_subscriptions[entity.entity_key] = []
+            self._entity_event_subscriptions[entity.entity_key].append(entity.event)
 
     async def remove_device(self, device: HmDevice) -> None:
         """Remove device to central collections."""
         if device.device_address not in self._devices:
             _LOGGER.debug(
                 "REMOVE_DEVICE: device %s not registered in central",
                 device.device_address,
@@ -903,22 +917,22 @@
         device.clear_collections()
 
         await self.device_descriptions.remove_device(device=device)
         await self.paramset_descriptions.remove_device(device=device)
         self.device_details.remove_device(device=device)
         del self._devices[device.device_address]
 
-    def remove_event_subscription(self, entity: BaseEntity) -> None:
+    def remove_event_subscription(self, entity: BaseParameterEntity) -> None:
         """Remove event subscription from central collections."""
         if (
             isinstance(entity, (GenericEntity, GenericEvent))
             and entity.supports_events
-            and (entity.channel_address, entity.parameter) in self._entity_event_subscriptions
+            and entity.entity_key in self._entity_event_subscriptions
         ):
-            del self._entity_event_subscriptions[(entity.channel_address, entity.parameter)]
+            del self._entity_event_subscriptions[entity.entity_key]
 
     async def execute_program(self, pid: str) -> bool:
         """Execute a program on CCU / Homegear."""
         if client := self.primary_client:
             return await client.execute_program(pid=pid)
         return False
 
@@ -974,15 +988,17 @@
         """Get the virtual remote for the Client."""
         for client in self._clients.values():
             virtual_remote = client.get_virtual_remote()
             if virtual_remote and virtual_remote.device_address == device_address:
                 return virtual_remote
         return None
 
-    def get_generic_entity(self, channel_address: str, parameter: str) -> GenericEntity | None:
+    def get_generic_entity(
+        self, channel_address: str, parameter: str, paramset_key: ParamsetKey = ParamsetKey.VALUES
+    ) -> GenericEntity | None:
         """Get entity by channel_address and parameter."""
         if device := self.get_device(address=channel_address):
             return device.get_generic_entity(channel_address=channel_address, parameter=parameter)
         return None
 
     def get_event(self, channel_address: str, parameter: str) -> GenericEvent | None:
         """Return the hm event."""
@@ -1012,88 +1028,96 @@
     async def clear_caches(self) -> None:
         """Clear all stored data."""
         await self.device_descriptions.clear()
         await self.paramset_descriptions.clear()
         self.device_details.clear()
         self.data_cache.clear()
 
-    def register_ha_event_callback(self, ha_event_callback: Callable) -> None:
+    def register_homematic_callback(self, cb: Callable) -> CALLBACK_TYPE:
         """Register ha_event callback in central."""
-        self._ha_event_callbacks.add(ha_event_callback)
+        self._homematic_callbacks.add(cb)
+        return partial(self._unregister_homematic_callback, cb)
 
-    def unregister_ha_event_callback(self, ha_event_callback: Callable) -> None:
+    def _unregister_homematic_callback(self, cb: Callable) -> None:
         """RUn register ha_event callback in central."""
-        if ha_event_callback in self._ha_event_callbacks:
-            self._ha_event_callbacks.remove(ha_event_callback)
+        if cb in self._homematic_callbacks:
+            self._homematic_callbacks.remove(cb)
 
     @loop_check
-    def fire_ha_event_callback(self, event_type: EventType, event_data: dict[str, str]) -> None:
+    def fire_homematic_callback(
+        self, event_type: HomematicEventType, event_data: dict[str, str]
+    ) -> None:
         """
-        Fire ha_event callback in central.
+        Fire homematic_callback in central.
 
         # Events like INTERFACE, KEYPRESS, ...
         """
-        for callback_handler in self._ha_event_callbacks:
+        for callback_handler in self._homematic_callbacks:
             try:
                 callback_handler(event_type, event_data)
             except Exception as ex:
                 _LOGGER.error(
-                    "FIRE_HA_EVENT_CALLBACK: Unable to call handler: %s", reduce_args(args=ex.args)
+                    "FIRE_HOMEMATIC_CALLBACK: Unable to call handler: %s",
+                    reduce_args(args=ex.args),
                 )
 
-    def register_entity_event_callback(self, entity_event_callback: Callable) -> None:
-        """Register entity_event callback in central."""
-        self._entity_event_callbacks.add(entity_event_callback)
-
-    def unregister_entity_event_callback(self, entity_event_callback: Callable) -> None:
-        """Un register entity_event callback in central."""
-        if entity_event_callback in self._entity_event_callbacks:
-            self._entity_event_callbacks.remove(entity_event_callback)
+    def register_backend_parameter_callback(self, cb: Callable) -> CALLBACK_TYPE:
+        """Register backend_parameter callback in central."""
+        self._backend_parameter_callbacks.add(cb)
+        return partial(self._unregister_backend_parameter_callback, cb)
+
+    def _unregister_backend_parameter_callback(self, cb: Callable) -> None:
+        """Un register backend_parameter callback in central."""
+        if cb in self._backend_parameter_callbacks:
+            self._backend_parameter_callbacks.remove(cb)
 
     @loop_check
-    def fire_entity_event_callback(
+    def fire_backend_parameter_callback(
         self, interface_id: str, channel_address: str, parameter: str, value: Any
     ) -> None:
         """
-        Fire entity callback in central.
+        Fire backend_parameter callback in central.
 
         Not used by HA.
         Re-Fired events from CCU for parameter updates.
         """
-        for callback_handler in self._entity_event_callbacks:
+        for callback_handler in self._backend_parameter_callbacks:
             try:
                 callback_handler(interface_id, channel_address, parameter, value)
             except Exception as ex:
                 _LOGGER.error(
-                    "FIRE_ENTITY_EVENT_CALLBACK: Unable to call handler: %s",
+                    "FIRE_BACKEND_PARAMETER_CALLBACK: Unable to call handler: %s",
                     reduce_args(args=ex.args),
                 )
 
-    def register_system_event_callback(self, system_event_callback: Callable) -> None:
+    def register_backend_system_callback(self, cb: Callable) -> CALLBACK_TYPE:
         """Register system_event callback in central."""
-        self._system_event_callbacks.add(system_event_callback)
+        self._backend_system_callbacks.add(cb)
+        return partial(self._unregister_backend_system_callback, cb)
 
-    def unregister_system_event_callback(self, system_event_callback: Callable) -> None:
+    def _unregister_backend_system_callback(self, cb: Callable) -> None:
         """Un register system_event callback in central."""
-        if system_event_callback in self._system_event_callbacks:
-            self._system_event_callbacks.remove(system_event_callback)
+        if cb in self._backend_system_callbacks:
+            self._backend_system_callbacks.remove(cb)
 
     @loop_check
-    def fire_system_event_callback(self, system_event: SystemEvent, **kwargs: Any) -> None:
+    def fire_backend_system_callback(
+        self, system_event: BackendSystemEvent, **kwargs: Any
+    ) -> None:
         """
         Fire system_event callback in central.
 
         e.g. DEVICES_CREATED, HUB_REFRESHED
         """
-        for callback_handler in self._system_event_callbacks:
+        for callback_handler in self._backend_system_callbacks:
             try:
                 callback_handler(system_event, **kwargs)
             except Exception as ex:
                 _LOGGER.error(
-                    "FIRE_SYSTEM_EVENT_CALLBACK: Unable to call handler: %s",
+                    "FIRE_BACKEND_SYSTEM_CALLBACK: Unable to call handler: %s",
                     reduce_args(args=ex.args),
                 )
 
     def __str__(self) -> str:
         """Provide some useful information."""
         return f"central name: {self.name}"
```

### Comparing `hahomematic-2024.4.9b2/hahomematic/central/decorators.py` & `hahomematic-2024.5.0/hahomematic/central/decorators.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,89 +7,91 @@
 from datetime import datetime
 from functools import wraps
 import logging
 from typing import Any, Final, ParamSpec, TypeVar, cast
 
 from hahomematic import central as hmcu, client as hmcl
 import hahomematic.central.xml_rpc_server as xmlrpc
-from hahomematic.const import SystemEvent
+from hahomematic.const import BackendSystemEvent
 from hahomematic.exceptions import HaHomematicException
 from hahomematic.support import reduce_args
 
 _LOGGER: Final = logging.getLogger(__name__)
 _P = ParamSpec("_P")
 _R = TypeVar("_R")
 
 _INTERFACE_ID: Final = "interface_id"
 
 
-def callback_system_event(system_event: SystemEvent) -> Callable:
-    """Check if system_event_callback is set and call it AFTER original function."""
+def callback_backend_system(system_event: BackendSystemEvent) -> Callable:
+    """Check if backend_system_callback is set and call it AFTER original function."""
 
-    def decorator_system_event_callback(
+    def decorator_backend_system_callback(
         func: Callable[_P, _R | Awaitable[_R]],
     ) -> Callable[_P, _R | Awaitable[_R]]:
         """Decorate callback system events."""
 
         @wraps(func)
-        async def async_wrapper_system_event_callback(*args: _P.args, **kwargs: _P.kwargs) -> _R:
+        async def async_wrapper_backend_system_callback(*args: _P.args, **kwargs: _P.kwargs) -> _R:
             """Wrap async callback system events."""
             return_value = cast(_R, await func(*args, **kwargs))  # type: ignore[misc]
-            await _exec_system_event_callback(*args, **kwargs)
+            await _exec_backend_system_callback(*args, **kwargs)
             return return_value
 
         @wraps(func)
-        def wrapper_system_event_callback(*args: _P.args, **kwargs: _P.kwargs) -> _R:
+        def wrapper_backend_system_callback(*args: _P.args, **kwargs: _P.kwargs) -> _R:
             """Wrap callback system events."""
             return_value = cast(_R, func(*args, **kwargs))
             try:
                 unit = args[0]
                 central: hmcu.CentralUnit | None = None
                 if isinstance(unit, hmcu.CentralUnit):
                     central = unit
                 if central is None and isinstance(unit, xmlrpc.RPCFunctions):
                     central = unit.get_central(interface_id=str(args[1]))
                 if central:
                     central.looper.create_task(
-                        _exec_system_event_callback(*args, **kwargs),
-                        name="wrapper_system_event_callback",
+                        _exec_backend_system_callback(*args, **kwargs),
+                        name="wrapper_backend_system_callback",
                     )
             except Exception as ex:
                 _LOGGER.warning(
-                    "EXEC_SYSTEM_EVENT_CALLBACK failed: Problem with identifying central: %s",
+                    "EXEC_BACKEND_SYSTEM_CALLBACK failed: Problem with identifying central: %s",
                     reduce_args(args=ex.args),
                 )
             return return_value
 
-        async def _exec_system_event_callback(*args: Any, **kwargs: Any) -> None:
+        async def _exec_backend_system_callback(*args: Any, **kwargs: Any) -> None:
             """Execute the callback for a system event."""
 
             if not ((len(args) > 1 and not kwargs) or (len(args) == 1 and kwargs)):
                 _LOGGER.warning(
-                    "EXEC_SYSTEM_EVENT_CALLBACK failed: *args not supported for callback_system_event"
+                    "EXEC_BACKEND_SYSTEM_CALLBACK failed: *args not supported for callback_system_event"
                 )
             try:
                 args = args[1:]
                 interface_id: str = args[0] if len(args) > 0 else str(kwargs[_INTERFACE_ID])
                 if client := hmcl.get_client(interface_id=interface_id):
                     client.last_updated = datetime.now()
-                    client.central.fire_system_event_callback(system_event=system_event, **kwargs)
+                    client.central.fire_backend_system_callback(
+                        system_event=system_event, **kwargs
+                    )
             except Exception as err:  # pragma: no cover
                 _LOGGER.warning(
-                    "EXEC_SYSTEM_EVENT_CALLBACK failed: Unable to reduce kwargs for system_event_callback"
+                    "EXEC_BACKEND_SYSTEM_CALLBACK failed: Unable to reduce kwargs for backend_system_callback"
                 )
                 raise HaHomematicException(
-                    f"args-exception system_event_callback [{reduce_args(args=err.args)}]"
+                    f"args-exception backend_system_callback [{reduce_args(args=err.args)}]"
                 ) from err
 
         if asyncio.iscoroutinefunction(func):
-            return async_wrapper_system_event_callback
-        return wrapper_system_event_callback
+            return async_wrapper_backend_system_callback
+        return wrapper_backend_system_callback
 
-    return decorator_system_event_callback
+    return decorator_backend_system_callback
 
 
 def callback_event(
     func: Callable[_P, _R],
 ) -> Callable:
     """Check if event_callback is set and call it AFTER original function."""
 
@@ -103,15 +105,15 @@
     def _exec_event_callback(*args: Any, **kwargs: Any) -> None:
         """Execute the callback for an entity event."""
         try:
             args = args[1:]
             interface_id: str = args[0] if len(args) > 1 else str(kwargs[_INTERFACE_ID])
             if client := hmcl.get_client(interface_id=interface_id):
                 client.last_updated = datetime.now()
-                client.central.fire_entity_event_callback(*args, **kwargs)
+                client.central.fire_backend_parameter_callback(*args, **kwargs)
         except Exception as err:  # pragma: no cover
             _LOGGER.warning(
                 "EXEC_ENTITY_EVENT_CALLBACK failed: Unable to reduce kwargs for event_callback"
             )
             raise HaHomematicException(
                 f"args-exception event_callback [{reduce_args(args=err.args)}]"
             ) from err
```

### Comparing `hahomematic-2024.4.9b2/hahomematic/central/xml_rpc_server.py` & `hahomematic-2024.5.0/hahomematic/central/xml_rpc_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 import logging
 import threading
 from typing import Any, Final
 from xmlrpc.server import SimpleXMLRPCRequestHandler, SimpleXMLRPCServer
 
 from hahomematic import central as hmcu
-from hahomematic.central.decorators import callback_system_event
-from hahomematic.const import IP_ANY_V4, PORT_ANY, SystemEvent
+from hahomematic.central.decorators import callback_backend_system
+from hahomematic.const import IP_ANY_V4, PORT_ANY, BackendSystemEvent
 from hahomematic.support import find_free_port
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 
 # pylint: disable=invalid-name
 class RPCFunctions:
@@ -37,15 +37,15 @@
                     channel_address=channel_address,
                     parameter=parameter,
                     value=value,
                 ),
                 name=f"event-{interface_id}-{channel_address}-{parameter}",
             )
 
-    @callback_system_event(system_event=SystemEvent.ERROR)
+    @callback_backend_system(system_event=BackendSystemEvent.ERROR)
     def error(self, interface_id: str, error_code: str, msg: str) -> None:
         """When some error occurs the CCU / Homegear will send its error message here."""
         _LOGGER.warning(
             "ERROR failed: interface_id = %s, error_code = %i, message = %s",
             interface_id,
             int(error_code),
             str(msg),
@@ -73,42 +73,42 @@
         central: hmcu.CentralUnit | None
         if central := self.get_central(interface_id):
             central.looper.create_task(
                 central.delete_devices(interface_id=interface_id, addresses=tuple(addresses)),
                 name=f"deleteDevices-{interface_id}",
             )
 
-    @callback_system_event(system_event=SystemEvent.UPDATE_DEVICE)
+    @callback_backend_system(system_event=BackendSystemEvent.UPDATE_DEVICE)
     def updateDevice(self, interface_id: str, address: str, hint: int) -> None:
         """
         Update a device.
 
         Irrelevant, as currently only changes to link
         partners are reported.
         """
         _LOGGER.debug(
             "UPDATEDEVICE: interface_id = %s, address = %s, hint = %s",
             interface_id,
             address,
             str(hint),
         )
 
-    @callback_system_event(system_event=SystemEvent.REPLACE_DEVICE)
+    @callback_backend_system(system_event=BackendSystemEvent.REPLACE_DEVICE)
     def replaceDevice(
         self, interface_id: str, old_device_address: str, new_device_address: str
     ) -> None:
         """Replace a device. Probably irrelevant for us."""
         _LOGGER.debug(
             "REPLACEDEVICE: interface_id = %s, oldDeviceAddress = %s, newDeviceAddress = %s",
             interface_id,
             old_device_address,
             new_device_address,
         )
 
-    @callback_system_event(system_event=SystemEvent.RE_ADDED_DEVICE)
+    @callback_backend_system(system_event=BackendSystemEvent.RE_ADDED_DEVICE)
     def readdedDevice(self, interface_id: str, addresses: list[str]) -> None:
         """
         Re-Add device from backend.
 
         Probably irrelevant for us.
         Gets called when a known devices is put into learn-mode
         while installation mode is active.
```

### Comparing `hahomematic-2024.4.9b2/hahomematic/client/__init__.py` & `hahomematic-2024.5.0/hahomematic/client/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,17 +7,19 @@
 from datetime import datetime
 import logging
 from typing import Any, Final, cast
 
 from hahomematic import central as hmcu
 from hahomematic.caches.dynamic import CommandCache, PingPongCache
 from hahomematic.client.xml_rpc import XmlRpcProxy
-from hahomematic.config import CALLBACK_WARN_INTERVAL, RECONNECT_WAIT
+from hahomematic.config import CALLBACK_WARN_INTERVAL, RECONNECT_WAIT, WAIT_FOR_CALLBACK
 from hahomematic.const import (
     DATETIME_FORMAT_MILLIS,
+    DEFAULT_CUSTOM_ID,
+    ENTITY_KEY,
     EVENT_AVAILABLE,
     EVENT_SECONDS_SINCE_LAST_EVENT,
     HOMEGEAR_SERIAL,
     INIT_DATETIME,
     VIRTUAL_REMOTE_TYPES,
     Backend,
     CallSource,
@@ -31,15 +33,21 @@
     ProxyInitState,
     SystemInformation,
     SystemVariableData,
 )
 from hahomematic.exceptions import BaseHomematicException, NoConnection
 from hahomematic.performance import measure_execution_time
 from hahomematic.platforms.device import HmDevice
-from hahomematic.support import build_headers, build_xml_rpc_uri, get_channel_no, reduce_args
+from hahomematic.support import (
+    build_headers,
+    build_xml_rpc_uri,
+    get_channel_no,
+    get_device_address,
+    reduce_args,
+)
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 _ADDRESS: Final = "address"
 _CHANNELS: Final = "channels"
 _ID: Final = "id"
 _INTERFACE: Final = "interface"
@@ -417,58 +425,74 @@
 
     @measure_execution_time
     async def _set_value(
         self,
         channel_address: str,
         parameter: str,
         value: Any,
+        wait_for_callback: int | None,
         rx_mode: str | None = None,
-    ) -> bool:
+    ) -> set[ENTITY_KEY]:
         """Set single value on paramset VALUES."""
         try:
             _LOGGER.debug("SET_VALUE: %s, %s, %s", channel_address, parameter, value)
             if rx_mode:
                 await self._proxy.setValue(channel_address, parameter, value, rx_mode)
             else:
                 await self._proxy.setValue(channel_address, parameter, value)
-            self._last_value_send_cache.add_set_value(
+            # store the send value in the last_value_send_cache
+            entity_keys = self._last_value_send_cache.add_set_value(
                 channel_address=channel_address, parameter=parameter, value=value
             )
+            if wait_for_callback is not None and (
+                device := self.central.get_device(
+                    address=get_device_address(address=channel_address)
+                )
+            ):
+                await wait_for_state_change_or_timeout(
+                    device=device,
+                    entity_keys=entity_keys,
+                    values={parameter: value},
+                    wait_for_callback=wait_for_callback,
+                )
+            return entity_keys  # noqa: TRY300
         except BaseHomematicException as ex:
             _LOGGER.warning(
                 "SET_VALUE failed with %s [%s]: %s, %s, %s",
                 ex.name,
                 reduce_args(args=ex.args),
                 channel_address,
                 parameter,
                 value,
             )
-            return False
-        return True
+            return set()
 
     async def set_value(
         self,
         channel_address: str,
         paramset_key: str,
         parameter: str,
         value: Any,
+        wait_for_callback: int | None = WAIT_FOR_CALLBACK,
         rx_mode: str | None = None,
-    ) -> bool:
+    ) -> set[ENTITY_KEY]:
         """Set single value on paramset VALUES."""
         if paramset_key == ParamsetKey.VALUES:
             return await self._set_value(
                 channel_address=channel_address,
                 parameter=parameter,
                 value=value,
+                wait_for_callback=wait_for_callback,
                 rx_mode=rx_mode,
             )
         return await self.put_paramset(
             channel_address=channel_address,
             paramset_key=paramset_key,
             values={parameter: value},
+            wait_for_callback=wait_for_callback,
             rx_mode=rx_mode,
         )
 
     async def get_paramset(self, address: str, paramset_key: str) -> dict[str, Any]:
         """
         Return a paramset from CCU.
 
@@ -494,42 +518,57 @@
 
     @measure_execution_time
     async def put_paramset(
         self,
         channel_address: str,
         paramset_key: str,
         values: dict[str, Any],
+        wait_for_callback: int | None = WAIT_FOR_CALLBACK,
         rx_mode: str | None = None,
-    ) -> bool:
+    ) -> set[ENTITY_KEY]:
         """
         Set paramsets manually.
 
         Address is usually the channel_address,
         but for bidcos devices there is a master paramset at the device.
         """
         try:
             _LOGGER.debug("PUT_PARAMSET: %s, %s, %s", channel_address, paramset_key, values)
             if rx_mode:
                 await self._proxy.putParamset(channel_address, paramset_key, values, rx_mode)
             else:
                 await self._proxy.putParamset(channel_address, paramset_key, values)
-            self._last_value_send_cache.add_put_paramset(
-                channel_address=channel_address, paramset_key=paramset_key, values=values
+            # store the send value in the last_value_send_cache
+            entity_keys = self._last_value_send_cache.add_put_paramset(
+                channel_address=channel_address,
+                paramset_key=paramset_key,
+                values=values,
             )
+            if wait_for_callback is not None and (
+                device := self.central.get_device(
+                    address=get_device_address(address=channel_address)
+                )
+            ):
+                await wait_for_state_change_or_timeout(
+                    device=device,
+                    entity_keys=entity_keys,
+                    values=values,
+                    wait_for_callback=wait_for_callback,
+                )
+            return entity_keys  # noqa: TRY300
         except BaseHomematicException as ex:
             _LOGGER.warning(
                 "PUT_PARAMSET failed: %s [%s] %s, %s, %s",
                 ex.name,
                 reduce_args(args=ex.args),
                 channel_address,
                 paramset_key,
                 values,
             )
-            return False
-        return True
+            return set()
 
     async def fetch_paramset_description(
         self, channel_address: str, paramset_key: str, save_to_file: bool = True
     ) -> None:
         """Fetch a specific paramset and add it to the known ones."""
         _LOGGER.debug("FETCH_PARAMSET_DESCRIPTION: %s for %s", paramset_key, channel_address)
 
@@ -1087,7 +1126,78 @@
 
 def get_client(interface_id: str) -> Client | None:
     """Return client by interface_id."""
     for central in hmcu.CENTRAL_INSTANCES.values():
         if central.has_client(interface_id=interface_id):
             return central.get_client(interface_id=interface_id)
     return None
+
+
+@measure_execution_time
+async def wait_for_state_change_or_timeout(
+    device: HmDevice, entity_keys: set[ENTITY_KEY], values: dict[str, Any], wait_for_callback: int
+) -> None:
+    """Wait for an entity to change state."""
+    waits = [
+        _track_single_entity_state_change_or_timeout(
+            device=device,
+            entity_key=entity_key,
+            value=values.get(entity_key[1]),
+            wait_for_callback=wait_for_callback,
+        )
+        for entity_key in entity_keys
+    ]
+    await asyncio.gather(*waits)
+
+
+@measure_execution_time
+async def _track_single_entity_state_change_or_timeout(
+    device: HmDevice, entity_key: ENTITY_KEY, value: Any, wait_for_callback: int
+) -> None:
+    """Wait for an entity to change state."""
+    ev = asyncio.Event()
+
+    def _async_event_changed(*args: Any, **kwargs: Any) -> None:
+        if entity:
+            _LOGGER.debug(
+                "TRACK_SINGLE_ENTITY_STATE_CHANGE_OR_TIMEOUT: Received event %s with value %s",
+                entity_key,
+                entity.value,
+            )
+            if _isclose(value, entity.value):
+                _LOGGER.debug(
+                    "TRACK_SINGLE_ENTITY_STATE_CHANGE_OR_TIMEOUT: Finished event %s with value %s",
+                    entity_key,
+                    entity.value,
+                )
+                ev.set()
+
+    channel_address, parameter = entity_key
+    if entity := device.get_generic_entity(channel_address=channel_address, parameter=parameter):
+        if not entity.supports_events:
+            _LOGGER.debug(
+                "TRACK_SINGLE_ENTITY_STATE_CHANGE_OR_TIMEOUT: Entity supports no events %s",
+                entity_key,
+            )
+            return
+        unsub = entity.register_entity_updated_callback(
+            cb=_async_event_changed, custom_id=DEFAULT_CUSTOM_ID
+        )
+
+        try:
+            async with asyncio.timeout(wait_for_callback):
+                await ev.wait()
+        except TimeoutError:
+            _LOGGER.debug(
+                "TRACK_SINGLE_ENTITY_STATE_CHANGE_OR_TIMEOUT: Timeout waiting for event %s with value %s",
+                entity_key,
+                entity.value,
+            )
+        finally:
+            unsub()
+
+
+def _isclose(value1: Any, value2: Any) -> bool:
+    """Check if the both values are close to each other."""
+    if isinstance(value1, float):
+        return bool(round(value1, 2) == round(value2, 2))
+    return bool(value1 == value2)
```

### Comparing `hahomematic-2024.4.9b2/hahomematic/client/json_rpc.py` & `hahomematic-2024.5.0/hahomematic/client/json_rpc.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b2/hahomematic/client/xml_rpc.py` & `hahomematic-2024.5.0/hahomematic/client/xml_rpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,21 +30,23 @@
 _VERIFY_TLS: Final = "verify_tls"
 
 
 class XmlRpcMethod(StrEnum):
     """Enum for homematic json rpc methods types."""
 
     GET_VERSION = "getVersion"
+    HOMEGEAR_INIT = "clientServerInitialized"
     INIT = "init"
     PING = "ping"
     SYSTEM_LIST_METHODS = "system.listMethods"
 
 
 _VALID_XMLRPC_COMMANDS_ON_NO_CONNECTION: Final[tuple[str, ...]] = (
     XmlRpcMethod.GET_VERSION,
+    XmlRpcMethod.HOMEGEAR_INIT,
     XmlRpcMethod.INIT,
     XmlRpcMethod.PING,
     XmlRpcMethod.SYSTEM_LIST_METHODS,
 )
 
 _SSL_ERROR_CODES: Final[dict[int, str]] = {
     errno.ENOEXEC: "EOF occurred in violation of protocol",
```

### Comparing `hahomematic-2024.4.9b2/hahomematic/const.py` & `hahomematic-2024.5.0/hahomematic/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """Constants used by hahomematic."""
 
 from __future__ import annotations
 
-from collections.abc import Mapping
+from collections.abc import Callable, Mapping
 from dataclasses import dataclass, field
 from datetime import datetime
 from enum import Enum, IntEnum, StrEnum
 from typing import Final
 
 DEFAULT_CONNECTION_CHECKER_INTERVAL: Final = 15  # check if connection is available via rpc ping
+DEFAULT_CUSTOM_ID: Final = "custom_id"
 DEFAULT_ENCODING: Final = "UTF-8"
 DEFAULT_JSON_SESSION_AGE: Final = 90
 DEFAULT_LAST_COMMAND_SEND_STORE_TIMEOUT: Final = 60
 DEFAULT_PING_PONG_MISMATCH_COUNT: Final = 15
 DEFAULT_PING_PONG_MISMATCH_COUNT_TTL: Final = 300
 DEFAULT_RECONNECT_WAIT: Final = 120  # wait with reconnect after a first ping was successful
 DEFAULT_TIMEOUT: Final = 60  # default timeout for a connection
 DEFAULT_TLS: Final = False
 DEFAULT_VERIFY_TLS: Final = False
+DEFAULT_WAIT_FOR_CALLBACK: Final[int | None] = None
 
 REGA_SCRIPT_FETCH_ALL_DEVICE_DATA: Final = "fetch_all_device_data.fn"
 REGA_SCRIPT_GET_SERIAL: Final = "get_serial.fn"
 REGA_SCRIPT_PATH: Final = "../rega_scripts"
 REGA_SCRIPT_SET_SYSTEM_VARIABLE: Final = "set_system_variable.fn"
 REGA_SCRIPT_SYSTEM_VARIABLES_EXT_MARKER: Final = "get_system_variables_ext_marker.fn"
 
@@ -67,23 +69,41 @@
 FILE_DEVICES: Final = "homematic_devices.json"
 FILE_PARAMSETS: Final = "homematic_paramsets.json"
 
 MAX_CACHE_AGE: Final = 60
 
 NO_CACHE_ENTRY: Final = "NO_CACHE_ENTRY"
 
+# channel_address, parameter
+ENTITY_KEY = tuple[str, str]
+CALLBACK_TYPE = Callable[[], None]
+
 
 class Backend(StrEnum):
     """Enum with supported hahomematic backends."""
 
     CCU = "CCU"
     HOMEGEAR = "Homegear"
     PYDEVCCU = "PyDevCCU"
 
 
+class BackendSystemEvent(StrEnum):
+    """Enum with hahomematic system events."""
+
+    DELETE_DEVICES = "deleteDevices"
+    DEVICES_CREATED = "devicesCreated"
+    ERROR = "error"
+    HUB_REFRESHED = "hubEntityRefreshed"
+    LIST_DEVICES = "listDevices"
+    NEW_DEVICES = "newDevices"
+    REPLACE_DEVICE = "replaceDevice"
+    RE_ADDED_DEVICE = "readdedDevice"
+    UPDATE_DEVICE = "updateDevice"
+
+
 class CallSource(StrEnum):
     """Enum with sources for calls."""
 
     HA_INIT = "ha_init"
     HM_INIT = "hm_init"
     MANUAL_OR_SCHEDULED = "manual_or_scheduled"
 
@@ -145,24 +165,14 @@
     CE_SECONDARY = "ce_secondary"
     CE_VISIBLE = "ce_visible"
     ENTITY = "entity"
     EVENT = "event"
     NO_CREATE = "entity_no_create"
 
 
-class EventType(StrEnum):
-    """Enum with hahomematic event types."""
-
-    DEVICE_AVAILABILITY = "homematic.device_availability"
-    DEVICE_ERROR = "homematic.device_error"
-    IMPULSE = "homematic.impulse"
-    INTERFACE = "homematic.interface"
-    KEYPRESS = "homematic.keypress"
-
-
 class Flag(IntEnum):
     """Enum with homematic flags."""
 
     VISIBLE = 1
     INTERNAL = 2
     TRANSFORM = 4  # not used
     SERVICE = 8
@@ -173,14 +183,24 @@
     """Enum with hahomematic event types."""
 
     FORCE_FALSE = "forced_not_available"
     FORCE_TRUE = "forced_available"
     NOT_SET = "not_set"
 
 
+class HomematicEventType(StrEnum):
+    """Enum with hahomematic event types."""
+
+    DEVICE_AVAILABILITY = "homematic.device_availability"
+    DEVICE_ERROR = "homematic.device_error"
+    IMPULSE = "homematic.impulse"
+    INTERFACE = "homematic.interface"
+    KEYPRESS = "homematic.keypress"
+
+
 class Manufacturer(StrEnum):
     """Enum with hahomematic system events."""
 
     EQ3 = "eQ-3"
     HB = "Homebrew"
     MOEHLENHOFF = "Möhlenhoff"
 
@@ -370,28 +390,14 @@
     INIT_FAILED = 0
     INIT_SUCCESS = 1
     DE_INIT_FAILED = 4
     DE_INIT_SUCCESS = 8
     DE_INIT_SKIPPED = 16
 
 
-class SystemEvent(StrEnum):
-    """Enum with hahomematic system events."""
-
-    DELETE_DEVICES = "deleteDevices"
-    DEVICES_CREATED = "devicesCreated"
-    ERROR = "error"
-    HUB_REFRESHED = "hubEntityRefreshed"
-    LIST_DEVICES = "listDevices"
-    NEW_DEVICES = "newDevices"
-    REPLACE_DEVICE = "replaceDevice"
-    RE_ADDED_DEVICE = "readdedDevice"
-    UPDATE_DEVICE = "updateDevice"
-
-
 class SysvarType(StrEnum):
     """Enum for homematic sysvar types."""
 
     ALARM = "ALARM"
     FLOAT = "FLOAT"
     INTEGER = "INTEGER"
     LIST = "LIST"
@@ -420,17 +426,17 @@
     Parameter.PRESS_LONG_START,
     Parameter.PRESS_SHORT,
     Parameter.PRESS_UNLOCK,
 )
 
 DEVICE_ERROR_EVENTS: Final[tuple[Parameter, ...]] = (Parameter.ERROR, Parameter.SENSOR_ERROR)
 
-ENTITY_EVENTS: Final[tuple[EventType, ...]] = (
-    EventType.IMPULSE,
-    EventType.KEYPRESS,
+ENTITY_EVENTS: Final[tuple[HomematicEventType, ...]] = (
+    HomematicEventType.IMPULSE,
+    HomematicEventType.KEYPRESS,
 )
 
 IMPULSE_EVENTS: Final[tuple[Parameter, ...]] = (Parameter.SEQUENCE_OK,)
 
 KEY_CHANNEL_OPERATION_MODE_VISIBILITY: Final[Mapping[str, tuple[str, ...]]] = {
     Parameter.STATE: ("BINARY_BEHAVIOR",),
     Parameter.PRESS_LONG: ("KEY_BEHAVIOR", "SWITCH_BEHAVIOR"),
```

### Comparing `hahomematic-2024.4.9b2/hahomematic/converter.py` & `hahomematic-2024.5.0/hahomematic/converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,44 @@
 """Converters used by hahomematic."""
 
 from __future__ import annotations
 
 import ast
+import logging
 from typing import Any, Final, cast
 
 from hahomematic.const import Parameter
+from hahomematic.support import reduce_args
+
+_LOGGER = logging.getLogger(__name__)
 
 
 def _convert_cpv_to_hm_level(cpv: Any) -> Any:
     """Convert combined parameter value for hm level."""
     if isinstance(cpv, str) and cpv.startswith("0x"):
         return ast.literal_eval(cpv) / 100 / 2
     return cpv
 
 
+def _convert_cpv_to_hmip_level(cpv: Any) -> Any:
+    """Convert combined parameter value for hmip level."""
+    return int(cpv) / 100
+
+
 def convert_hm_level_to_cpv(hm_level: Any) -> Any:
     """Convert hm level to combined parameter value."""
     return format(int(hm_level * 100 * 2), "#04x")
 
 
 CONVERTABLE_PARAMETERS: Final = (Parameter.COMBINED_PARAMETER, Parameter.LEVEL_COMBINED)
 
 _COMBINED_PARAMETER_TO_HM_CONVERTER: Final = {
     Parameter.LEVEL_COMBINED: _convert_cpv_to_hm_level,
+    Parameter.LEVEL: _convert_cpv_to_hmip_level,
+    Parameter.LEVEL_2: _convert_cpv_to_hmip_level,
 }
 
 _COMBINED_PARAMETER_NAMES: Final = {"L": Parameter.LEVEL, "L2": Parameter.LEVEL_2}
 
 
 def _convert_combined_parameter_to_paramset(cpv: str) -> dict[str, Any]:
     """Convert combined parameter to paramset."""
@@ -58,10 +69,18 @@
     Parameter.COMBINED_PARAMETER: _convert_combined_parameter_to_paramset,
     Parameter.LEVEL_COMBINED: _convert_level_combined_to_paramset,
 }
 
 
 def convert_combined_parameter_to_paramset(parameter: str, cpv: str) -> dict[str, Any]:
     """Convert combined parameter to paramset."""
-    if converter := _COMBINED_PARAMETER_TO_PARAMSET_CONVERTER.get(parameter):  # type: ignore[call-overload]
-        return cast(dict[str, Any], converter(cpv))
+    try:
+        if converter := _COMBINED_PARAMETER_TO_PARAMSET_CONVERTER.get(parameter):  # type: ignore[call-overload]
+            return cast(dict[str, Any], converter(cpv))
+        _LOGGER.debug(
+            "CONVERT_COMBINED_PARAMETER_TO_PARAMSET: No converter found for %s: %s", parameter, cpv
+        )
+    except Exception as ex:
+        _LOGGER.debug(
+            "CONVERT_COMBINED_PARAMETER_TO_PARAMSET: Convert failed %s", reduce_args(args=ex.args)
+        )
     return {}
```

### Comparing `hahomematic-2024.4.9b2/hahomematic/exceptions.py` & `hahomematic-2024.5.0/hahomematic/exceptions.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b2/hahomematic/hmcli.py` & `hahomematic-2024.5.0/hahomematic/hmcli.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b2/hahomematic/performance.py` & `hahomematic-2024.5.0/hahomematic/performance.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,19 +24,20 @@
         if is_enabled:
             start = datetime.now()
         try:
             return await func(*args, **kwargs)
         finally:
             if is_enabled:
                 delta = (datetime.now() - start).total_seconds()
+                arg = str(args[0]) if len(args) > 0 else ""
                 _LOGGER.info(
                     "Execution of %s took %ss (%s)",
                     func.__name__,
                     delta,
-                    str(args[0]),
+                    arg,
                 )
 
     @wraps(func)
     def wrapper(*args: Any, **kwargs: Any) -> Any:
         """Wrap method."""
         if is_enabled:
             start = datetime.now()
```

### Comparing `hahomematic-2024.4.9b2/hahomematic/platforms/__init__.py` & `hahomematic-2024.5.0/hahomematic/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b2/hahomematic/platforms/custom/__init__.py` & `hahomematic-2024.5.0/hahomematic/platforms/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b2/hahomematic/platforms/custom/climate.py` & `hahomematic-2024.5.0/hahomematic/platforms/custom/climate.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,15 +196,15 @@
     @property
     def _min_or_target_temperature(self) -> float:
         """Return the min or target temperature."""
         if (temperature := self.target_temperature or self.min_temp) < self.min_temp:
             return self.min_temp
         return temperature
 
-    @bind_collector
+    @bind_collector()
     async def set_temperature(
         self,
         temperature: float,
         collector: CallParameterCollector | None = None,
         do_validate: bool = True,
     ) -> None:
         """Set new target temperature."""
@@ -327,15 +327,15 @@
         )
 
     @config_property
     def supports_preset(self) -> bool:
         """Flag if climate supports preset."""
         return True
 
-    @bind_collector
+    @bind_collector()
     async def set_hvac_mode(
         self, hvac_mode: HvacMode, collector: CallParameterCollector | None = None
     ) -> None:
         """Set new target hvac mode."""
         if not self.is_state_change(hvac_mode=hvac_mode):
             return
         if hvac_mode == HvacMode.AUTO:
@@ -348,15 +348,15 @@
             await self._e_manu_mode.send_value(value=self.target_temperature, collector=collector)
             # Disable validation here to allow setting a value,
             # that is out of the validation range.
             await self.set_temperature(
                 temperature=_OFF_TEMPERATURE, collector=collector, do_validate=False
             )
 
-    @bind_collector
+    @bind_collector()
     async def set_preset_mode(
         self, preset_mode: PresetMode, collector: CallParameterCollector | None = None
     ) -> None:
         """Set new preset mode."""
         if not self.is_state_change(preset_mode=preset_mode):
             return
         if preset_mode == PresetMode.BOOST:
@@ -497,15 +497,15 @@
         return tuple(presets)
 
     @config_property
     def supports_preset(self) -> bool:
         """Flag if climate supports preset."""
         return True
 
-    @bind_collector
+    @bind_collector()
     async def set_hvac_mode(
         self, hvac_mode: HvacMode, collector: CallParameterCollector | None = None
     ) -> None:
         """Set new target hvac mode."""
         if not self.is_state_change(hvac_mode=hvac_mode):
             return
         # if switching hvac_mode then disable boost_mode
@@ -519,15 +519,15 @@
             await self.set_temperature(
                 temperature=self._min_or_target_temperature, collector=collector
             )
         elif hvac_mode == HvacMode.OFF:
             await self._e_control_mode.send_value(value=ModeHmIP.MANU, collector=collector)
             await self.set_temperature(temperature=_OFF_TEMPERATURE, collector=collector)
 
-    @bind_collector
+    @bind_collector()
     async def set_preset_mode(
         self, preset_mode: PresetMode, collector: CallParameterCollector | None = None
     ) -> None:
         """Set new preset mode."""
         if not self.is_state_change(preset_mode=preset_mode):
             return
         if preset_mode == PresetMode.BOOST:
```

### Comparing `hahomematic-2024.4.9b2/hahomematic/platforms/custom/const.py` & `hahomematic-2024.5.0/hahomematic/platforms/custom/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b2/hahomematic/platforms/custom/cover.py` & `hahomematic-2024.5.0/hahomematic/platforms/custom/cover.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from hahomematic.platforms.generic.select import HmSelect
 from hahomematic.platforms.generic.sensor import HmSensor
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 _CLOSED_LEVEL: Final[float] = 0.0  # must be float!
 _OPEN_LEVEL: Final[float] = 1.0  # must be float!
+_OPEN_TILT_LEVEL: Final[float] = 0.5  # must be float!
 _WD_CLOSED_LEVEL: Final[float] = -0.005  # must be float! HM-Sec-Win
 
 
 class StateChangeArg(StrEnum):
     """Enum with cover state change arguments."""
 
     CLOSE = "close"
@@ -110,15 +111,15 @@
         return self._e_level.value if self._e_level.value is not None else self._closed_level
 
     @value_property
     def current_position(self) -> int:
         """Return current position of cover."""
         return int(self._channel_level * 100)
 
-    @bind_collector
+    @bind_collector()
     async def set_position(
         self,
         position: int | None = None,
         tilt_position: int | None = None,
         collector: CallParameterCollector | None = None,
     ) -> None:
         """Move the cover to a specific position."""
@@ -153,29 +154,29 @@
     @value_property
     def is_closing(self) -> bool | None:
         """Return if the cover is closing."""
         if self._e_direction.value is not None:
             return str(self._e_direction.value) == CoverActivity.CLOSING
         return None
 
-    @bind_collector
+    @bind_collector()
     async def open(self, collector: CallParameterCollector | None = None) -> None:
         """Open the cover."""
         if not self.is_state_change(open=True):
             return
         await self._set_level(level=self._open_level, collector=collector)
 
-    @bind_collector
+    @bind_collector()
     async def close(self, collector: CallParameterCollector | None = None) -> None:
         """Close the cover."""
         if not self.is_state_change(close=True):
             return
         await self._set_level(level=self._closed_level, collector=collector)
 
-    @bind_collector
+    @bind_collector()
     async def stop(self, collector: CallParameterCollector | None = None) -> None:
         """Stop the device if in motion."""
         await self._e_stop.send_value(value=True, collector=collector)
 
     def is_state_change(self, **kwargs: Any) -> bool:
         """Check if the state changes due to kwargs."""
         if kwargs.get(StateChangeArg.OPEN) is not None and self._channel_level != self._open_level:
@@ -226,14 +227,16 @@
             wd_level = level
         await self._e_level.send_value(value=wd_level, collector=collector, do_validate=False)
 
 
 class CeBlind(CeCover):
     """Class for HomeMatic blind entities."""
 
+    _open_tilt_level: float = _OPEN_TILT_LEVEL
+
     def _init_entity_fields(self) -> None:
         """Init the entity fields."""
         super()._init_entity_fields()
         self._e_channel_level_2: HmSensor = self._get_entity(
             field=Field.CHANNEL_LEVEL_2, entity_type=HmSensor
         )
         self._e_level_2: HmFloat = self._get_entity(field=Field.LEVEL_2, entity_type=HmFloat)
@@ -249,29 +252,15 @@
         return self._e_level_2.value if self._e_level_2.value is not None else self._closed_level
 
     @value_property
     def current_tilt_position(self) -> int:
         """Return current tilt position of cover."""
         return int(self._channel_tilt_level * 100)
 
-    @property
-    def _target_level(self) -> float | None:
-        """Return the level of last service call."""
-        if (last_value_send := self._e_level.unconfirmed_last_value_send) is not None:
-            return float(last_value_send)
-        return None
-
-    @property
-    def _target_tilt_level(self) -> float | None:
-        """Return the tilt level of last service call."""
-        if (last_value_send := self._e_level_2.unconfirmed_last_value_send) is not None:
-            return float(last_value_send)
-        return None
-
-    @bind_collector
+    @bind_collector(use_command_queue=False)
     async def set_position(
         self,
         position: int | None = None,
         tilt_position: int | None = None,
         collector: CallParameterCollector | None = None,
     ) -> None:
         """Move the blind to a specific position."""
@@ -290,54 +279,62 @@
         collector: CallParameterCollector | None = None,
     ) -> None:
         """
         Move the cover to a specific tilt level. Value range is 0.0 to 1.01.
 
         1.01 means no change.
         """
-        if level is not None:
-            _level = level
-        elif (self.is_opening or self.is_closing) and self._target_level is not None:
-            # The blind moves and the target blind height is known
-            _level = self._target_level
-        else:  # The blind is at a standstill and no level is explicitly requested => we remain at the current level
-            _level = self._channel_level
-
-        if tilt_level is not None:
-            _tilt_level = tilt_level
-        elif (self.is_opening or self.is_closing) and self._target_tilt_level is not None:
-            # The blind moves and the target slat position is known
-            _tilt_level = self._target_tilt_level
-        else:  # The blind is at a standstill and no tilt is explicitly desired => we remain at the current angle
-            _tilt_level = self._channel_tilt_level
-
+        _level = level if level is not None else self.current_position / 100.0
+        _tilt_level = tilt_level if tilt_level is not None else self.current_tilt_position / 100.0
         if self._e_combined.is_hmtype and (
             combined_parameter := self._get_combined_value(level=_level, tilt_level=_tilt_level)
         ):
             await self._e_combined.send_value(value=combined_parameter, collector=collector)
             return
 
         await self._e_level_2.send_value(value=_tilt_level, collector=collector)
         await super()._set_level(level=_level, collector=collector)
 
-    @bind_collector
+    @bind_collector(use_command_queue=False)
+    async def open(self, collector: CallParameterCollector | None = None) -> None:
+        """Open the cover and open the tilt."""
+        if not self.is_state_change(open=True, tilt_open=True):
+            return
+        await self._set_level(
+            level=self._open_level,
+            tilt_level=self._open_tilt_level,
+            collector=collector,
+        )
+
+    @bind_collector(use_command_queue=False)
+    async def close(self, collector: CallParameterCollector | None = None) -> None:
+        """Close the cover and close the tilt."""
+        if not self.is_state_change(close=True, tilt_close=True):
+            return
+        await self._set_level(
+            level=self._closed_level,
+            tilt_level=self._closed_level,
+            collector=collector,
+        )
+
+    @bind_collector(use_command_queue=False)
     async def open_tilt(self, collector: CallParameterCollector | None = None) -> None:
         """Open the tilt."""
         if not self.is_state_change(tilt_open=True):
             return
-        await self._set_level(tilt_level=self._open_level, collector=collector)
+        await self._set_level(tilt_level=self._open_tilt_level, collector=collector)
 
-    @bind_collector
+    @bind_collector(use_command_queue=False)
     async def close_tilt(self, collector: CallParameterCollector | None = None) -> None:
         """Close the tilt."""
         if not self.is_state_change(tilt_close=True):
             return
         await self._set_level(tilt_level=self._closed_level, collector=collector)
 
-    @bind_collector
+    @bind_collector()
     async def stop_tilt(self, collector: CallParameterCollector | None = None) -> None:
         """Stop the device if in motion."""
         await self._e_stop.send_value(value=True, collector=collector)
 
     def is_state_change(self, **kwargs: Any) -> bool:
         """Check if the state changes due to kwargs."""
         if (
@@ -383,41 +380,19 @@
         self._e_channel_operation_mode: HmSelect = self._get_entity(
             field=Field.CHANNEL_OPERATION_MODE, entity_type=HmSelect
         )
         self._e_combined: HmAction = self._get_entity(
             field=Field.COMBINED_PARAMETER, entity_type=HmAction
         )
 
-    @value_property
+    @property
     def channel_operation_mode(self) -> str | None:
         """Return channel_operation_mode of cover."""
         return self._e_channel_operation_mode.value
 
-    @bind_collector
-    async def open(self, collector: CallParameterCollector | None = None) -> None:
-        """Open the cover and open the tilt."""
-        if not self.is_state_change(open=True, tilt_open=True):
-            return
-        await self._set_level(
-            level=self._open_level,
-            tilt_level=self._open_level,
-            collector=collector,
-        )
-
-    @bind_collector
-    async def close(self, collector: CallParameterCollector | None = None) -> None:
-        """Close the cover and close the tilt."""
-        if not self.is_state_change(close=True, tilt_close=True):
-            return
-        await self._set_level(
-            level=self._closed_level,
-            tilt_level=self._closed_level,
-            collector=collector,
-        )
-
     def _get_combined_value(
         self, level: float | None = None, tilt_level: float | None = None
     ) -> str | None:
         """Return the combined parameter."""
         if level is None and tilt_level is None:
             return None
         levels: list[str] = []
@@ -454,15 +429,15 @@
             return CoverPosition.OPEN
         if self._e_door_state.value == GarageDoorState.VENTILATION_POSITION:
             return CoverPosition.VENT
         if self._e_door_state.value == GarageDoorState.CLOSED:
             return CoverPosition.CLOSED
         return None
 
-    @bind_collector
+    @bind_collector()
     async def set_position(
         self,
         position: int | None = None,
         tilt_position: int | None = None,
         collector: CallParameterCollector | None = None,
     ) -> None:
         """Move the garage door to a specific position."""
@@ -492,34 +467,34 @@
     @value_property
     def is_closing(self) -> bool | None:
         """Return if the garage door is closing."""
         if self._e_section.value is not None:
             return int(self._e_section.value) == GarageDoorActivity.CLOSING
         return None
 
-    @bind_collector
+    @bind_collector()
     async def open(self, collector: CallParameterCollector | None = None) -> None:
         """Open the garage door."""
         if not self.is_state_change(open=True):
             return
         await self._e_door_command.send_value(value=GarageDoorCommand.OPEN, collector=collector)
 
-    @bind_collector
+    @bind_collector()
     async def close(self, collector: CallParameterCollector | None = None) -> None:
         """Close the garage door."""
         if not self.is_state_change(close=True):
             return
         await self._e_door_command.send_value(value=GarageDoorCommand.CLOSE, collector=collector)
 
-    @bind_collector
+    @bind_collector()
     async def stop(self, collector: CallParameterCollector | None = None) -> None:
         """Stop the device if in motion."""
         await self._e_door_command.send_value(value=GarageDoorCommand.STOP, collector=collector)
 
-    @bind_collector
+    @bind_collector()
     async def vent(self, collector: CallParameterCollector | None = None) -> None:
         """Move the garage door to vent position."""
         if not self.is_state_change(vent=True):
             return
         await self._e_door_command.send_value(
             value=GarageDoorCommand.PARTIAL_OPEN, collector=collector
         )
```

### Comparing `hahomematic-2024.4.9b2/hahomematic/platforms/custom/definition.py` & `hahomematic-2024.5.0/hahomematic/platforms/custom/definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,14 +146,15 @@
         },
         DeviceProfile.IP_FIXED_COLOR_LIGHT: {
             ED.DEVICE_GROUP: {
                 ED.PRIMARY_CHANNEL: 1,
                 ED.SECONDARY_CHANNELS: (2, 3),
                 ED.REPEATABLE_FIELDS: {
                     Field.COLOR: Parameter.COLOR,
+                    Field.COLOR_BEHAVIOUR: Parameter.COLOR_BEHAVIOUR,
                     Field.LEVEL: Parameter.LEVEL,
                     Field.ON_TIME_UNIT: Parameter.DURATION_UNIT,
                     Field.ON_TIME_VALUE: Parameter.DURATION_VALUE,
                     Field.RAMP_TIME_UNIT: Parameter.RAMP_TIME_UNIT,
                     Field.RAMP_TIME_VALUE: Parameter.RAMP_TIME_VALUE,
                 },
                 ED.VISIBLE_FIELDS: {
@@ -165,20 +166,20 @@
             },
         },
         DeviceProfile.IP_SIMPLE_FIXED_COLOR_LIGHT_WIRED: {
             ED.DEVICE_GROUP: {
                 ED.PRIMARY_CHANNEL: 0,
                 ED.REPEATABLE_FIELDS: {
                     Field.COLOR: Parameter.COLOR,
+                    Field.COLOR_BEHAVIOUR: Parameter.COLOR_BEHAVIOUR,
                     Field.LEVEL: Parameter.LEVEL,
                     Field.ON_TIME_UNIT: Parameter.DURATION_UNIT,
                     Field.ON_TIME_VALUE: Parameter.DURATION_VALUE,
                     Field.RAMP_TIME_UNIT: Parameter.RAMP_TIME_UNIT,
                     Field.RAMP_TIME_VALUE: Parameter.RAMP_TIME_VALUE,
-                    Field.COLOR_BEHAVIOUR: Parameter.COLOR_BEHAVIOUR,
                 },
             },
         },
         DeviceProfile.IP_SIMPLE_FIXED_COLOR_LIGHT: {
             ED.DEVICE_GROUP: {
                 ED.PRIMARY_CHANNEL: 0,
                 ED.REPEATABLE_FIELDS: {
```

### Comparing `hahomematic-2024.4.9b2/hahomematic/platforms/custom/entity.py` & `hahomematic-2024.5.0/hahomematic/platforms/custom/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """Module with base class for custom entities."""
 
 from __future__ import annotations
 
-from abc import abstractmethod
 from collections.abc import Callable, Mapping
 from datetime import datetime
 import logging
 from typing import Any, Final, TypeVar, cast
 
-from hahomematic.const import INIT_DATETIME, CallSource, EntityUsage
+from hahomematic.const import ENTITY_KEY, INIT_DATETIME, CallSource, EntityUsage
 from hahomematic.platforms import device as hmd
 from hahomematic.platforms.custom import definition as hmed
 from hahomematic.platforms.custom.const import DeviceProfile, Field
 from hahomematic.platforms.custom.support import ExtendedConfig
-from hahomematic.platforms.decorators import config_property, value_property
+from hahomematic.platforms.decorators import config_property
 from hahomematic.platforms.entity import BaseEntity, CallParameterCollector
 from hahomematic.platforms.generic import entity as hmge
 from hahomematic.platforms.support import (
     EntityNameData,
     check_channel_is_the_only_primary_channel,
     get_custom_entity_name,
 )
@@ -59,30 +58,32 @@
         self._init_entity_fields()
 
     @config_property
     def base_channel_no(self) -> int | None:
         """Return the base channel no of the entity."""
         return self._base_channel_no
 
-    @abstractmethod
     def _init_entity_fields(self) -> None:
         """Init the entity fields."""
+        _LOGGER.debug(
+            "INIT_ENTITY_FIELDS: Initialising the custom entity fields for %s", self.full_name
+        )
 
-    @value_property
+    @property
     def last_updated(self) -> datetime:
         """Return the latest last_updated timestamp."""
         latest_update: datetime = INIT_DATETIME
         for entity in self._readable_entities:
             if (
                 entity_last_updated := entity.last_updated
             ) and entity_last_updated > latest_update:
                 latest_update = entity_last_updated
         return latest_update
 
-    @value_property
+    @property
     def last_refreshed(self) -> datetime:
         """Return the latest last_refreshed timestamp."""
         latest_refreshed: datetime = INIT_DATETIME
         for entity in self._readable_entities:
             if (
                 entity_last_refreshed := entity.last_refreshed
             ) and entity_last_refreshed > latest_refreshed:
@@ -99,20 +100,20 @@
         return unconfirmed_values
 
     @property
     def has_data_entities(self) -> bool:
         """Return if there are data entities."""
         return len(self._data_entities) > 0
 
-    @value_property
+    @property
     def is_valid(self) -> bool:
         """Return if the state is valid."""
         return all(entity.is_valid for entity in self._relevant_entities)
 
-    @value_property
+    @property
     def state_uncertain(self) -> bool:
         """Return, if the state is uncertain."""
         return any(entity.state_uncertain for entity in self._relevant_entities)
 
     @property
     def _readable_entities(self) -> tuple[hmge.GenericEntity, ...]:
         """Returns the list of readable entities."""
@@ -234,31 +235,23 @@
             return
         self.device.add_sub_device_channel(
             channel_no=self._channel_no, base_channel_no=self._base_channel_no
         )
         if is_visible:
             entity.set_usage(EntityUsage.CE_VISIBLE)
 
-        entity.register_internal_entity_updated_callback(
-            entity_updated_callback=self.fire_entity_updated_callback
-        )
+        entity.register_internal_entity_updated_callback(cb=self.fire_entity_updated_callback)
         self._data_entities[field] = entity
 
-    def unregister_entity_updated_callback(
-        self, entity_updated_callback: Callable, custom_id: str
-    ) -> None:
+    def _unregister_entity_updated_callback(self, cb: Callable, custom_id: str) -> None:
         """Unregister update callback."""
         for entity in self._data_entities.values():
-            entity.unregister_internal_entity_updated_callback(
-                update_callback=entity_updated_callback
-            )
+            entity.unregister_internal_entity_updated_callback(cb=cb)
 
-        super().unregister_entity_updated_callback(
-            entity_updated_callback=entity_updated_callback, custom_id=custom_id
-        )
+        super()._unregister_entity_updated_callback(cb=cb, custom_id=custom_id)
 
     def _mark_entities(self, entity_def: Mapping[int | tuple[int, ...], tuple[str, ...]]) -> None:
         """Mark entities to be created in HA."""
         if not entity_def:
             return
         for channel_nos, parameters in entity_def.items():
             if isinstance(channel_nos, int):
@@ -294,14 +287,21 @@
                 )
             return cast(entity_type, entity)  # type: ignore[valid-type]
         return cast(
             entity_type,  # type:ignore[valid-type]
             NoneTypeEntity(),
         )
 
+    def has_entity_key(self, entity_keys: set[ENTITY_KEY]) -> bool:
+        """Return if an entity with one of the entities is part of this entity."""
+        result = [
+            entity for entity in self._data_entities.values() if entity.entity_key in entity_keys
+        ]
+        return len(result) > 0
+
 
 class NoneTypeEntity:
     """Entity to return an empty value."""
 
     default: Any = None
     hmtype: Any = None
     is_valid: bool = False
```

### Comparing `hahomematic-2024.4.9b2/hahomematic/platforms/custom/light.py` & `hahomematic-2024.5.0/hahomematic/platforms/custom/light.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,15 +224,15 @@
         return None
 
     @value_property
     def effects(self) -> tuple[str, ...] | None:
         """Return the supported effects."""
         return None
 
-    @bind_collector
+    @bind_collector()
     async def turn_on(
         self, collector: CallParameterCollector | None = None, **kwargs: Unpack[LightOnArgs]
     ) -> None:
         """Turn the light on."""
         if not self.is_state_change(on=True, **kwargs):
             return
         if ramp_time := kwargs.get("ramp_time"):
@@ -241,27 +241,27 @@
             await self._set_on_time_value(on_time=on_time, collector=collector)
 
         if not (brightness := kwargs.get("brightness", self.brightness)):
             brightness = int(_MAX_BRIGHTNESS)
         level = brightness / _MAX_BRIGHTNESS
         await self._e_level.send_value(value=level, collector=collector)
 
-    @bind_collector
+    @bind_collector()
     async def turn_off(
         self, collector: CallParameterCollector | None = None, **kwargs: Unpack[LightOffArgs]
     ) -> None:
         """Turn the light off."""
         if not self.is_state_change(off=True, **kwargs):
             return
         if ramp_time := kwargs.get("ramp_time"):
             await self._set_ramp_time_off_value(ramp_time=ramp_time, collector=collector)
 
         await self._e_level.send_value(value=_DIMMER_OFF, collector=collector)
 
-    @bind_collector
+    @bind_collector()
     async def _set_on_time_value(
         self, on_time: float, collector: CallParameterCollector | None = None
     ) -> None:
         """Set the on time value in seconds."""
         await self._e_on_time_value.send_value(value=on_time, collector=collector)
 
     async def _set_ramp_time_on_value(
@@ -329,15 +329,15 @@
                 # For the sake of robustness we return "white" anyway.
                 return 0.0, 0.0
 
             # For all other colors we assume saturation of 1
             return color / 200 * 360, 100
         return 0.0, 0.0
 
-    @bind_collector
+    @bind_collector()
     async def turn_on(
         self, collector: CallParameterCollector | None = None, **kwargs: Unpack[LightOnArgs]
     ) -> None:
         """Turn the light on."""
         if not self.is_state_change(on=True, **kwargs):
             return
         if (hs_color := kwargs.get("hs_color")) is not None:
@@ -375,15 +375,15 @@
         return None
 
     @value_property
     def effects(self) -> tuple[str, ...] | None:
         """Return the supported effects."""
         return self._effects
 
-    @bind_collector
+    @bind_collector()
     async def turn_on(
         self, collector: CallParameterCollector | None = None, **kwargs: Unpack[LightOnArgs]
     ) -> None:
         """Turn the light on."""
         if not self.is_state_change(on=True, **kwargs):
             return
 
@@ -413,15 +413,15 @@
         )
 
     @value_property
     def color_temp(self) -> int | None:
         """Return the color temperature in mireds of this light between min/max mireds."""
         return int(_MAX_MIREDS - (_MAX_MIREDS - _MIN_MIREDS) * (self._e_color_level.value or 0.0))
 
-    @bind_collector
+    @bind_collector()
     async def turn_on(
         self, collector: CallParameterCollector | None = None, **kwargs: Unpack[LightOnArgs]
     ) -> None:
         """Turn the light on."""
         if not self.is_state_change(on=True, **kwargs):
             return
         if (color_temp := kwargs.get("color_temp")) is not None:
@@ -528,15 +528,15 @@
         return self._usage
 
     @value_property
     def effects(self) -> tuple[str, ...] | None:
         """Return the supported effects."""
         return self._e_effect.values or ()
 
-    @bind_collector
+    @bind_collector()
     async def turn_on(
         self, collector: CallParameterCollector | None = None, **kwargs: Unpack[LightOnArgs]
     ) -> None:
         """Turn the light on."""
         if not self.is_state_change(on=True, **kwargs):
             return
         if (hs_color := kwargs.get("hs_color")) is not None:
@@ -553,15 +553,15 @@
             # 111600 is a special value for NOT_USED
             await self._set_on_time_value(on_time=111600, collector=collector)
         if self.supports_effects and (effect := kwargs.get("effect")) is not None:
             await self._e_effect.send_value(value=effect, collector=collector)
 
         await super().turn_on(collector=collector, **kwargs)
 
-    @bind_collector
+    @bind_collector()
     async def _set_on_time_value(
         self, on_time: float, collector: CallParameterCollector | None = None
     ) -> None:
         """Set the on time value in seconds."""
         on_time, on_time_unit = _recalc_unit_timer(time=on_time)
         if on_time_unit:
             await self._e_on_time_unit.send_value(value=on_time_unit, collector=collector)
@@ -635,15 +635,15 @@
         return self._e_hue, self._e_level, self._e_saturation, self._e_color_temperature_kelvin
 
     @value_property
     def effects(self) -> tuple[str, ...] | None:
         """Return the supported effects."""
         return self._e_effect.values or ()
 
-    @bind_collector
+    @bind_collector()
     async def turn_on(
         self, collector: CallParameterCollector | None = None, **kwargs: Unpack[LightOnArgs]
     ) -> None:
         """Turn the light on."""
         if not self.is_state_change(on=True, **kwargs):
             return
         if (hs_color := kwargs.get("hs_color")) is not None:
@@ -660,15 +660,15 @@
             # 111600 is a special value for NOT_USED
             await self._set_on_time_value(on_time=111600, collector=collector)
         if self.supports_effects and (effect := kwargs.get("effect")) is not None:
             await self._e_effect.send_value(value=effect, collector=collector)
 
         await super().turn_on(collector=collector, **kwargs)
 
-    @bind_collector
+    @bind_collector()
     async def _set_on_time_value(
         self, on_time: float, collector: CallParameterCollector | None = None
     ) -> None:
         """Set the on time value in seconds."""
         on_time, on_time_unit = _recalc_unit_timer(time=on_time)
         if on_time_unit:
             await self._e_on_time_unit.send_value(value=on_time_unit, collector=collector)
@@ -719,14 +719,38 @@
         )
         self._e_on_time_unit: HmAction = self._get_entity(
             field=Field.ON_TIME_UNIT, entity_type=HmAction
         )
         self._e_ramp_time_unit: HmAction = self._get_entity(
             field=Field.RAMP_TIME_UNIT, entity_type=HmAction
         )
+        self._e_effect: HmSelect = self._get_entity(
+            field=Field.COLOR_BEHAVIOUR, entity_type=HmSelect
+        )
+        self._effect_list = (
+            tuple(
+                str(item)
+                for item in self._e_effect.values
+                if item not in _EXCLUDE_FROM_COLOR_BEHAVIOUR
+            )
+            if (self._e_effect and self._e_effect.values)
+            else ()
+        )
+
+    @value_property
+    def effect(self) -> str | None:
+        """Return the current effect."""
+        if (effect := self._e_effect.value) is not None and effect in self._effect_list:
+            return effect
+        return None
+
+    @value_property
+    def effects(self) -> tuple[str, ...] | None:
+        """Return the supported effects."""
+        return self._effect_list
 
     @value_property
     def hs_color(self) -> tuple[float, float] | None:
         """Return the hue and saturation color value [float, float]."""
         if (
             self._e_color.value is not None
             and (hs_color := _FIXED_COLOR_SWITCHER.get(self._e_color.value)) is not None
@@ -737,30 +761,36 @@
     @value_property
     def channel_hs_color(self) -> tuple[float, float] | None:
         """Return the channel hue and saturation color value [float, float]."""
         if self._e_channel_color.value is not None:
             return _FIXED_COLOR_SWITCHER.get(self._e_channel_color.value, (0.0, 0.0))
         return None
 
-    @bind_collector
+    @bind_collector()
     async def turn_on(
         self, collector: CallParameterCollector | None = None, **kwargs: Unpack[LightOnArgs]
     ) -> None:
         """Turn the light on."""
         if not self.is_state_change(on=True, **kwargs):
             return
         if (hs_color := kwargs.get("hs_color")) is not None:
             simple_rgb_color = _convert_color(hs_color)
             await self._e_color.send_value(value=simple_rgb_color, collector=collector)
         elif self.color_name in _NO_COLOR:
             await self._e_color.send_value(value=FixedColor.WHITE, collector=collector)
+        if (effect := kwargs.get("effect")) is not None and effect in self._effect_list:
+            await self._e_effect.send_value(value=effect, collector=collector)
+        elif self._e_effect.value not in self._effect_list:
+            await self._e_effect.send_value(value=ColorBehaviour.ON, collector=collector)
+        elif (color_behaviour := self._e_effect.value) is not None:
+            await self._e_effect.send_value(value=color_behaviour, collector=collector)
 
         await super().turn_on(collector=collector, **kwargs)
 
-    @bind_collector
+    @bind_collector()
     async def _set_on_time_value(
         self, on_time: float, collector: CallParameterCollector | None = None
     ) -> None:
         """Set the on time value in seconds."""
         on_time, on_time_unit = _recalc_unit_timer(time=on_time)
         if on_time_unit:
             await self._e_on_time_unit.send_value(value=on_time_unit, collector=collector)
@@ -772,63 +802,14 @@
         """Set the ramp time value in seconds."""
         ramp_time, ramp_time_unit = _recalc_unit_timer(time=ramp_time)
         if ramp_time_unit:
             await self._e_ramp_time_unit.send_value(value=ramp_time_unit, collector=collector)
         await self._e_ramp_time_value.send_value(value=float(ramp_time), collector=collector)
 
 
-class CeIpFixedColorLightWired(CeIpFixedColorLight):
-    """Class for HomematicIP HmIPW-WRC6 light entities."""
-
-    def _init_entity_fields(self) -> None:
-        """Init the entity fields."""
-        super()._init_entity_fields()
-        self._e_effect: HmSelect = self._get_entity(
-            field=Field.COLOR_BEHAVIOUR, entity_type=HmSelect
-        )
-        self._effect_list = (
-            tuple(
-                str(item)
-                for item in self._e_effect.values
-                if item not in _EXCLUDE_FROM_COLOR_BEHAVIOUR
-            )
-            if (self._e_effect and self._e_effect.values)
-            else ()
-        )
-
-    @value_property
-    def effect(self) -> str | None:
-        """Return the current effect."""
-        if (effect := self._e_effect.value) is not None and effect in self._effect_list:
-            return effect
-        return None
-
-    @value_property
-    def effects(self) -> tuple[str, ...] | None:
-        """Return the supported effects."""
-        return self._effect_list
-
-    @bind_collector
-    async def turn_on(
-        self, collector: CallParameterCollector | None = None, **kwargs: Unpack[LightOnArgs]
-    ) -> None:
-        """Turn the light on."""
-        if not self.is_state_change(on=True, **kwargs):
-            return
-
-        if (effect := kwargs.get("effect")) is not None and effect in self._effect_list:
-            await self._e_effect.send_value(value=effect, collector=collector)
-        elif self._e_effect.value not in self._effect_list:
-            await self._e_effect.send_value(value=ColorBehaviour.ON, collector=collector)
-        elif (color_behaviour := self._e_effect.value) is not None:
-            await self._e_effect.send_value(value=color_behaviour, collector=collector)
-
-        await super().turn_on(collector=collector, **kwargs)
-
-
 def _recalc_unit_timer(time: float) -> tuple[float, int | None]:
     """Recalculate unit and value of timer."""
     ramp_time_unit = TimeUnit.SECONDS
     if time == 111600:
         return time, None
     if time > 16343:
         time /= 60
@@ -986,15 +967,15 @@
     device: hmd.HmDevice,
     group_base_channels: tuple[int, ...],
     extended: ExtendedConfig | None = None,
 ) -> tuple[CustomEntity, ...]:
     """Create simple fixed color light entities like HmIPW-WRC6."""
     return hmed.make_custom_entity(
         device=device,
-        entity_class=CeIpFixedColorLightWired,
+        entity_class=CeIpFixedColorLight,
         device_profile=DeviceProfile.IP_SIMPLE_FIXED_COLOR_LIGHT_WIRED,
         group_base_channels=group_base_channels,
         extended=extended,
     )
 
 
 def make_ip_rgbw_light(
```

### Comparing `hahomematic-2024.4.9b2/hahomematic/platforms/custom/lock.py` & `hahomematic-2024.5.0/hahomematic/platforms/custom/lock.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,25 +112,25 @@
         return None
 
     @value_property
     def is_jammed(self) -> bool:
         """Return true if lock is jammed."""
         return False
 
-    @bind_collector
+    @bind_collector()
     async def lock(self, collector: CallParameterCollector | None = None) -> None:
         """Lock the lock."""
         await self._e_lock_target_level.send_value(value=LockState.LOCKED, collector=collector)
 
-    @bind_collector
+    @bind_collector()
     async def unlock(self, collector: CallParameterCollector | None = None) -> None:
         """Unlock the lock."""
         await self._e_lock_target_level.send_value(value=LockState.UNLOCKED, collector=collector)
 
-    @bind_collector
+    @bind_collector()
     async def open(self, collector: CallParameterCollector | None = None) -> None:
         """Open the lock."""
         await self._e_lock_target_level.send_value(value=LockState.OPEN, collector=collector)
 
 
 class CeRfLock(BaseLock):
     """Class for classic HomeMatic lock entities."""
@@ -163,25 +163,25 @@
         return None
 
     @value_property
     def is_jammed(self) -> bool:
         """Return true if lock is jammed."""
         return self._e_error.value is not None and self._e_error.value != LockState.NO_ERROR
 
-    @bind_collector
+    @bind_collector()
     async def lock(self, collector: CallParameterCollector | None = None) -> None:
         """Lock the lock."""
         await self._e_state.send_value(value=False, collector=collector)
 
-    @bind_collector
+    @bind_collector()
     async def unlock(self, collector: CallParameterCollector | None = None) -> None:
         """Unlock the lock."""
         await self._e_state.send_value(value=True, collector=collector)
 
-    @bind_collector
+    @bind_collector()
     async def open(self, collector: CallParameterCollector | None = None) -> None:
         """Open the lock."""
         await self._e_open.send_value(value=True, collector=collector)
 
 
 def make_ip_lock(
     device: hmd.HmDevice,
```

### Comparing `hahomematic-2024.4.9b2/hahomematic/platforms/custom/siren.py` & `hahomematic-2024.5.0/hahomematic/platforms/custom/siren.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
         return self._e_optical_alarm_selection.values
 
     @config_property
     def supports_duration(self) -> bool:
         """Flag if siren supports duration."""
         return True
 
-    @bind_collector
+    @bind_collector()
     async def turn_on(
         self,
         collector: CallParameterCollector | None = None,
         **kwargs: Unpack[SirenOnArgs],
     ) -> None:
         """Turn the device on."""
 
@@ -163,15 +163,15 @@
         await self._e_optical_alarm_selection.send_value(value=optical_alarm, collector=collector)
         await self._e_duration_unit.send_value(
             value=self._e_duration_unit.default, collector=collector
         )
         duration = kwargs.get("duration", self._e_duration.default)
         await self._e_duration.send_value(value=duration, collector=collector)
 
-    @bind_collector
+    @bind_collector()
     async def turn_off(self, collector: CallParameterCollector | None = None) -> None:
         """Turn the device off."""
         await self._e_acoustic_alarm_selection.send_value(
             value=self._e_acoustic_alarm_selection.default, collector=collector
         )
         await self._e_optical_alarm_selection.send_value(
             value=self._e_optical_alarm_selection.default, collector=collector
```

### Comparing `hahomematic-2024.4.9b2/hahomematic/platforms/custom/support.py` & `hahomematic-2024.5.0/hahomematic/platforms/custom/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b2/hahomematic/platforms/custom/switch.py` & `hahomematic-2024.5.0/hahomematic/platforms/custom/switch.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,26 +58,26 @@
         return self._e_channel_state.value
 
     @value_property
     def value(self) -> bool | None:
         """Return the current value of the switch."""
         return self._e_state.value
 
-    @bind_collector
+    @bind_collector()
     async def turn_on(
         self, collector: CallParameterCollector | None = None, on_time: float | None = None
     ) -> None:
         """Turn the switch on."""
         if not self.is_state_change(on=True, on_time=on_time):
             return
         if on_time is not None or (on_time := self.get_on_time_and_cleanup()):
             await self._e_on_time_value.send_value(value=float(on_time), collector=collector)
         await self._e_state.turn_on(collector=collector)
 
-    @bind_collector
+    @bind_collector()
     async def turn_off(self, collector: CallParameterCollector | None = None) -> None:
         """Turn the switch off."""
         if not self.is_state_change(off=True):
             return
         await self._e_state.turn_off(collector=collector)
 
     def is_state_change(self, **kwargs: Any) -> bool:
```

### Comparing `hahomematic-2024.4.9b2/hahomematic/platforms/decorators.py` & `hahomematic-2024.5.0/hahomematic/platforms/decorators.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b2/hahomematic/platforms/device.py` & `hahomematic-2024.5.0/hahomematic/platforms/device.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,55 +2,64 @@
 
 from __future__ import annotations
 
 import asyncio
 from collections.abc import Callable, Mapping, Set as AbstractSet
 from copy import copy
 from datetime import datetime
+from functools import partial
 import logging
 import os
 import random
 from typing import Any, Final
 
 import orjson
 
 from hahomematic import central as hmcu
 from hahomematic.async_support import loop_check
 from hahomematic.const import (
+    CALLBACK_TYPE,
     DEFAULT_DEVICE_DESCRIPTIONS_DIR,
     DEFAULT_PARAMSET_DESCRIPTIONS_DIR,
     ENTITY_EVENTS,
+    ENTITY_KEY,
     IDENTIFIER_SEPARATOR,
     INIT_DATETIME,
     NO_CACHE_ENTRY,
     PLATFORMS,
     RELEVANT_INIT_PARAMETERS,
     VIRTUAL_REMOTE_TYPES,
     CallSource,
     DataOperationResult,
     Description,
     DeviceFirmwareState,
     EntityUsage,
-    EventType,
     ForcedDeviceAvailability,
     HmPlatform,
+    HomematicEventType,
     Manufacturer,
     Parameter,
     ParamsetKey,
     ProductGroup,
 )
 from hahomematic.exceptions import BaseHomematicException
 from hahomematic.platforms.custom import definition as hmed, entity as hmce
 from hahomematic.platforms.decorators import config_property, value_property
-from hahomematic.platforms.entity import BaseEntity, CallbackEntity
+from hahomematic.platforms.entity import BaseParameterEntity, CallbackEntity
 from hahomematic.platforms.event import GenericEvent
 from hahomematic.platforms.generic.entity import GenericEntity
 from hahomematic.platforms.support import PayloadMixin, get_device_name
 from hahomematic.platforms.update import HmUpdate
-from hahomematic.support import CacheEntry, Channel, check_or_create_directory, reduce_args
+from hahomematic.support import (
+    CacheEntry,
+    Channel,
+    check_or_create_directory,
+    get_entity_key,
+    reduce_args,
+)
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 
 class HmDevice(PayloadMixin):
     """Object to hold information about a device and associated entities."""
 
@@ -71,16 +80,16 @@
         _LOGGER.debug(
             "__INIT__: Initializing device: %s, %s",
             interface_id,
             device_address,
         )
         # {channel_no, entity}
         self._custom_entities: Final[dict[int, hmce.CustomEntity]] = {}
-        self._generic_entities: Final[dict[tuple[str, str], GenericEntity]] = {}
-        self._generic_events: Final[dict[tuple[str, str], GenericEvent]] = {}
+        self._generic_entities: Final[dict[ENTITY_KEY, GenericEntity]] = {}
+        self._generic_events: Final[dict[ENTITY_KEY, GenericEvent]] = {}
         self._last_updated: datetime = INIT_DATETIME
         self._forced_availability: ForcedDeviceAvailability = ForcedDeviceAvailability.NOT_SET
         self._device_updated_callbacks: Final[list[Callable]] = []
         self._firmware_update_callbacks: Final[list[Callable]] = []
         self._device_type: Final = str(
             self.central.device_descriptions.get_device_parameter(
                 interface_id=interface_id,
@@ -343,39 +352,35 @@
 
     def get_sub_device_channel(self, channel_no: int) -> int | None:
         """Return the sub device channel."""
         return self._sub_device_channels.get(channel_no)
 
     def add_entity(self, entity: CallbackEntity) -> None:
         """Add a hm entity to a device."""
-        if isinstance(entity, BaseEntity):
+        if isinstance(entity, BaseParameterEntity):
             self.central.add_event_subscription(entity=entity)
         if isinstance(entity, GenericEntity):
-            self._generic_entities[(entity.channel_address, entity.parameter)] = entity
-            self.register_device_updated_callback(
-                device_updated_callback=entity.fire_entity_updated_callback
-            )
+            self._generic_entities[entity.entity_key] = entity
+            self._register_device_updated_callback(cb=entity.fire_entity_updated_callback)
         if isinstance(entity, hmce.CustomEntity):
             self._custom_entities[entity.channel_no] = entity
         if isinstance(entity, GenericEvent):
-            self._generic_events[(entity.channel_address, entity.parameter)] = entity
+            self._generic_events[entity.entity_key] = entity
 
     def remove_entity(self, entity: CallbackEntity) -> None:
         """Add a hm entity to a device."""
-        if isinstance(entity, BaseEntity):
+        if isinstance(entity, BaseParameterEntity):
             self.central.remove_event_subscription(entity=entity)
         if isinstance(entity, GenericEntity):
-            del self._generic_entities[(entity.channel_address, entity.parameter)]
-            self.unregister_device_updated_callback(
-                device_updated_callback=entity.fire_entity_updated_callback
-            )
+            del self._generic_entities[entity.entity_key]
+            self._unregister_device_updated_callback(cb=entity.fire_entity_updated_callback)
         if isinstance(entity, hmce.CustomEntity):
             del self._custom_entities[entity.channel_no]
         if isinstance(entity, GenericEvent):
-            del self._generic_events[(entity.channel_address, entity.parameter)]
+            del self._generic_events[entity.entity_key]
         entity.fire_device_removed_callback()
 
     def clear_collections(self) -> None:
         """Remove entities from collections and central."""
         for event in self.generic_events:
             self.remove_entity(event)
         self._generic_events.clear()
@@ -384,39 +389,35 @@
             self.remove_entity(entity)
         self._generic_entities.clear()
 
         for custom_entity in self.custom_entities:
             self.remove_entity(custom_entity)
         self._custom_entities.clear()
 
-    def register_device_updated_callback(self, device_updated_callback: Callable) -> None:
+    def _register_device_updated_callback(self, cb: Callable) -> CALLBACK_TYPE:
         """Register update callback."""
-        if (
-            callable(device_updated_callback)
-            and device_updated_callback not in self._device_updated_callbacks
-        ):
-            self._device_updated_callbacks.append(device_updated_callback)
+        if callable(cb) and cb not in self._device_updated_callbacks:
+            self._device_updated_callbacks.append(cb)
+        return partial(self._unregister_device_updated_callback, cb)
 
-    def unregister_device_updated_callback(self, device_updated_callback: Callable) -> None:
+    def _unregister_device_updated_callback(self, cb: Callable) -> None:
         """Remove update callback."""
-        if device_updated_callback in self._device_updated_callbacks:
-            self._device_updated_callbacks.remove(device_updated_callback)
+        if cb in self._device_updated_callbacks:
+            self._device_updated_callbacks.remove(cb)
 
-    def register_firmware_update_callback(self, firmware_update_callback: Callable) -> None:
+    def register_firmware_update_callback(self, cb: Callable) -> CALLBACK_TYPE:
         """Register firmware update callback."""
-        if (
-            callable(firmware_update_callback)
-            and firmware_update_callback not in self._firmware_update_callbacks
-        ):
-            self._firmware_update_callbacks.append(firmware_update_callback)
+        if callable(cb) and cb not in self._firmware_update_callbacks:
+            self._firmware_update_callbacks.append(cb)
+        return partial(self.unregister_firmware_update_callback, cb)
 
-    def unregister_firmware_update_callback(self, firmware_update_callback: Callable) -> None:
+    def unregister_firmware_update_callback(self, cb: Callable) -> None:
         """Remove firmware update callback."""
-        if firmware_update_callback in self._firmware_update_callbacks:
-            self._firmware_update_callbacks.remove(firmware_update_callback)
+        if cb in self._firmware_update_callbacks:
+            self._firmware_update_callbacks.remove(cb)
 
     def _set_last_updated(self) -> None:
         self._last_updated = datetime.now()
 
     def get_entities(
         self,
         platform: HmPlatform | None = None,
@@ -457,15 +458,15 @@
         ):
             if entity.platform in PLATFORMS:
                 entities_by_platform[entity.platform].add(entity)
 
         return entities_by_platform
 
     def get_channel_events(
-        self, event_type: EventType, registered: bool | None = None
+        self, event_type: HomematicEventType, registered: bool | None = None
     ) -> Mapping[int, list[GenericEvent]]:
         """Return a list of specific events of a channel."""
         event_dict: dict[int, list[GenericEvent]] = {}
         if event_type not in ENTITY_EVENTS:
             return event_dict
         for event in self.generic_events:
             if (
@@ -481,19 +482,23 @@
 
     def get_custom_entity(self, channel_no: int) -> hmce.CustomEntity | None:
         """Return an entity from device."""
         return self._custom_entities.get(channel_no)
 
     def get_generic_entity(self, channel_address: str, parameter: str) -> GenericEntity | None:
         """Return an entity from device."""
-        return self._generic_entities.get((channel_address, parameter))
+        return self._generic_entities.get(
+            get_entity_key(channel_address=channel_address, parameter=parameter)
+        )
 
     def get_generic_event(self, channel_address: str, parameter: str) -> GenericEvent | None:
         """Return a generic event from device."""
-        return self._generic_events.get((channel_address, parameter))
+        return self._generic_events.get(
+            get_entity_key(channel_address=channel_address, parameter=parameter)
+        )
 
     def get_readable_entities(self, paramset_key: ParamsetKey) -> tuple[GenericEntity, ...]:
         """Return the list of readable master entities."""
         return tuple(
             ge
             for ge in self._generic_entities.values()
             if ge.is_readable and ge.paramset_key == paramset_key
```

### Comparing `hahomematic-2024.4.9b2/hahomematic/platforms/entity.py` & `hahomematic-2024.5.0/hahomematic/platforms/entity.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 """Functions for entity creation."""
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from collections.abc import Callable, Mapping
 from datetime import datetime
-from functools import wraps
+from functools import partial, wraps
 from inspect import getfullargspec
 import logging
 from typing import Any, Final, Generic, TypeVar, cast
 
 import voluptuous as vol
 
 from hahomematic import central as hmcu, client as hmcl, support as hms
 from hahomematic.async_support import loop_check
+from hahomematic.config import WAIT_FOR_CALLBACK
 from hahomematic.const import (
+    CALLBACK_TYPE,
+    DEFAULT_CUSTOM_ID,
+    ENTITY_KEY,
     EVENT_ADDRESS,
     EVENT_CHANNEL_NO,
     EVENT_DEVICE_TYPE,
     EVENT_INTERFACE_ID,
     EVENT_PARAMETER,
     EVENT_VALUE,
     INIT_DATETIME,
@@ -39,28 +43,26 @@
 from hahomematic.platforms.decorators import config_property, value_property
 from hahomematic.platforms.support import (
     EntityNameData,
     PayloadMixin,
     convert_value,
     generate_channel_unique_id,
 )
-from hahomematic.support import reduce_args
+from hahomematic.support import get_entity_key, reduce_args
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 _CallableT = TypeVar("_CallableT", bound=Callable[..., Any])
 
 _CONFIGURABLE_CHANNEL: Final[tuple[str, ...]] = (
     "KEY_TRANSCEIVER",
     "MULTI_MODE_INPUT_TRANSMITTER",
 )
 _COLLECTOR_ARGUMENT_NAME = "collector"
 
-DEFAULT_CUSTOM_ID: Final = "custom_id"
-
 _FIX_UNIT_REPLACE: Final[Mapping[str, str]] = {
     '"': "",
     "100%": "%",
     "% rF": "%",
     "degree": "°C",
     "Lux": "lx",
     "m3": "m³",
@@ -117,15 +119,15 @@
     @property
     @abstractmethod
     def available(self) -> bool:
         """Return the availability of the device."""
 
     @property
     def custom_id(self) -> str | None:
-        """Return the central unit."""
+        """Return the custom id."""
         return self._custom_id
 
     @classmethod
     def default_platform(cls) -> HmPlatform:
         """Return, the platform of the entity."""
         return cls._platform
 
@@ -135,20 +137,20 @@
         return self._central
 
     @config_property
     @abstractmethod
     def full_name(self) -> str:
         """Return the full name of the entity."""
 
-    @value_property
+    @property
     def last_updated(self) -> datetime:
         """Return the last updated datetime value."""
         return self._last_updated
 
-    @value_property
+    @property
     def last_refreshed(self) -> datetime:
         """Return the last refreshed datetime value."""
         return self._last_refreshed
 
     @config_property
     @abstractmethod
     def name(self) -> str | None:
@@ -179,60 +181,52 @@
         )
 
     @property
     def is_registered(self) -> bool:
         """Return if entity is registered externally."""
         return self._custom_id is not None
 
-    def register_internal_entity_updated_callback(self, entity_updated_callback: Callable) -> None:
+    def register_internal_entity_updated_callback(self, cb: Callable) -> CALLBACK_TYPE:
         """Register internal entity updated callback."""
-        self.register_entity_updated_callback(
-            entity_updated_callback=entity_updated_callback, custom_id=DEFAULT_CUSTOM_ID
-        )
+        self.register_entity_updated_callback(cb=cb, custom_id=DEFAULT_CUSTOM_ID)
+        return partial(self.unregister_internal_entity_updated_callback, cb)
 
-    def register_entity_updated_callback(
-        self, entity_updated_callback: Callable, custom_id: str
-    ) -> None:
+    def register_entity_updated_callback(self, cb: Callable, custom_id: str) -> CALLBACK_TYPE:
         """Register entity updated callback."""
-        if callable(entity_updated_callback):
-            self._entity_updated_callbacks[entity_updated_callback] = custom_id
+        if callable(cb):
+            self._entity_updated_callbacks[cb] = custom_id
         if custom_id != DEFAULT_CUSTOM_ID:
             if self._custom_id is not None and self._custom_id != custom_id:
                 raise HaHomematicException(
                     f"REGISTER_entity_updated_CALLBACK failed: hm_entity: {self.full_name} is already registered by {self._custom_id}"
                 )
             self._custom_id = custom_id
+        return partial(self._unregister_entity_updated_callback, cb, custom_id)
 
-    def unregister_internal_entity_updated_callback(self, update_callback: Callable) -> None:
+    def unregister_internal_entity_updated_callback(self, cb: Callable) -> None:
         """Unregister entity updated callback."""
-        self.unregister_entity_updated_callback(
-            entity_updated_callback=update_callback, custom_id=DEFAULT_CUSTOM_ID
-        )
+        self._unregister_entity_updated_callback(cb=cb, custom_id=DEFAULT_CUSTOM_ID)
 
-    def unregister_entity_updated_callback(
-        self, entity_updated_callback: Callable, custom_id: str
-    ) -> None:
+    def _unregister_entity_updated_callback(self, cb: Callable, custom_id: str) -> None:
         """Unregister entity updated callback."""
-        if entity_updated_callback in self._entity_updated_callbacks:
-            del self._entity_updated_callbacks[entity_updated_callback]
+        if cb in self._entity_updated_callbacks:
+            del self._entity_updated_callbacks[cb]
         if self.custom_id == custom_id:
             self._custom_id = None
 
-    def register_device_removed_callback(self, device_removed_callback: Callable) -> None:
+    def register_device_removed_callback(self, cb: Callable) -> CALLBACK_TYPE:
         """Register the device removed callback."""
-        if (
-            callable(device_removed_callback)
-            and device_removed_callback not in self._device_removed_callbacks
-        ):
-            self._device_removed_callbacks.append(device_removed_callback)
+        if callable(cb) and cb not in self._device_removed_callbacks:
+            self._device_removed_callbacks.append(cb)
+        return partial(self._unregister_device_removed_callback, cb)
 
-    def unregister_device_removed_callback(self, device_removed_callback: Callable) -> None:
+    def _unregister_device_removed_callback(self, cb: Callable) -> None:
         """Unregister the device removed callback."""
-        if device_removed_callback in self._device_removed_callbacks:
-            self._device_removed_callbacks.remove(device_removed_callback)
+        if cb in self._device_removed_callbacks:
+            self._device_removed_callbacks.remove(cb)
 
     @loop_check
     def fire_entity_updated_callback(self, *args: Any, **kwargs: Any) -> None:
         """Do what is needed when the value of the entity has been updated/refreshed."""
         for callback_handler in self._entity_updated_callbacks:
             try:
                 callback_handler(*args, **kwargs)
@@ -480,14 +474,22 @@
 
     @config_property
     def is_un_ignored(self) -> bool:
         """Return if the parameter is un ignored."""
         return self._is_un_ignored
 
     @config_property
+    def entity_key(self) -> ENTITY_KEY:
+        """Return entity key value."""
+        return get_entity_key(
+            channel_address=self._channel_address,
+            parameter=self._parameter,
+        )
+
+    @config_property
     def max(self) -> ParameterT:
         """Return max value."""
         return self._max
 
     @config_property
     def min(self) -> ParameterT:
         """Return min value."""
@@ -519,57 +521,53 @@
         return self._is_forced_sensor
 
     @property
     def is_readable(self) -> bool:
         """Return, if entity is readable."""
         return bool(self._operations & Operations.READ)
 
-    @value_property
+    @property
     def is_valid(self) -> bool:
         """Return, if the value of the entity is valid based on the last updated datetime."""
         return self._last_refreshed > INIT_DATETIME
 
     @property
     def is_writeable(self) -> bool:
         """Return, if entity is writeable."""
         return False if self._is_forced_sensor else bool(self._operations & Operations.WRITE)
 
-    @value_property
+    @property
     def last_updated(self) -> datetime:
         """Return the last updated datetime value."""
         return self._last_updated
 
-    @value_property
+    @property
     def last_refreshed(self) -> datetime:
         """Return the last refreshed datetime value."""
         return self._last_refreshed
 
     @property
     def unconfirmed_last_value_send(self) -> ParameterT | None:
         """Return the unconfirmed value send for the entity."""
         return cast(
             ParameterT | None,
-            self._client.last_value_send_cache.get_last_value_send(
-                paramset_key=self.paramset_key,
-                channel_address=self.channel_address,
-                parameter=self.parameter,
-            ),
+            self._client.last_value_send_cache.get_last_value_send(entity_key=self.entity_key),
         )
 
-    @value_property
+    @property
     def old_value(self) -> ParameterT | None:
         """Return the old value of the entity."""
         return self._old_value
 
     @config_property
     def platform(self) -> HmPlatform:
         """Return, the platform of the entity."""
         return HmPlatform.SENSOR if self._is_forced_sensor else self._platform
 
-    @value_property
+    @property
     def state_uncertain(self) -> bool:
         """Return, if the state is uncertain."""
         return self._state_uncertain
 
     @value_property
     def value(self) -> ParameterT | None:
         """Return the value of the entity."""
@@ -602,15 +600,16 @@
         """Return the if entity is visible in ccu."""
         return self._visible
 
     @property
     def _channel_operation_mode(self) -> str | None:
         """Return the channel operation mode if available."""
         cop: BaseParameterEntity | None = self._device.get_generic_entity(
-            channel_address=self._channel_address, parameter=Parameter.CHANNEL_OPERATION_MODE
+            channel_address=self._channel_address,
+            parameter=Parameter.CHANNEL_OPERATION_MODE,
         )
         if cop and cop.value:
             return str(cop.value)
         return None
 
     @property
     def _enabled_by_channel_operation_mode(self) -> bool | None:
@@ -757,73 +756,103 @@
             event_data[EVENT_VALUE] = value
         return cast(dict[str, Any], EVENT_DATA_SCHEMA(event_data))
 
 
 class CallParameterCollector:
     """Create a Paramset based on given generic entities."""
 
-    def __init__(self, client: hmcl.Client) -> None:
+    def __init__(self, device: hmd.HmDevice) -> None:
         """Init the generator."""
-        self._client: Final = client
-        self._use_put_paramset: bool = True
+        self._device: Final = device
+        self._client: Final = device.client
         self._paramsets: Final[dict[int, dict[str, dict[str, Any]]]] = {}
 
     def add_entity(
         self,
         entity: BaseParameterEntity,
         value: Any,
         collector_order: int,
-        use_put_paramset: bool = True,
     ) -> None:
         """Add a generic entity."""
-        if use_put_paramset is False:
-            self._use_put_paramset = False
         if collector_order not in self._paramsets:
             self._paramsets[collector_order] = {}
         if entity.channel_address not in self._paramsets[collector_order]:
             self._paramsets[collector_order][entity.channel_address] = {}
         self._paramsets[collector_order][entity.channel_address][entity.parameter] = value
 
-    async def send_data(self) -> bool:
+    async def send_data(
+        self, wait_for_callback: int | None, use_command_queue: bool, use_put_paramset: bool
+    ) -> bool:
         """Send data to backend."""
         for paramset_no in dict(sorted(self._paramsets.items())).values():
             for channel_address, paramset in paramset_no.items():
-                if len(paramset.values()) == 1 or self._use_put_paramset is False:
+                if len(paramset.values()) == 1 or use_put_paramset is False:
                     for parameter, value in paramset.items():
-                        if not await self._client.set_value(
+                        set_value_command = partial(
+                            self._client.set_value,
                             channel_address=channel_address,
                             paramset_key=ParamsetKey.VALUES,
                             parameter=parameter,
                             value=value,
-                        ):
+                            wait_for_callback=wait_for_callback,
+                        )
+                        if use_command_queue:
+                            await self._device.central.command_queue_handler.put(
+                                device_address=self._device.device_address,
+                                command=set_value_command,
+                            )
+                        elif not await set_value_command():
                             return False  # pragma: no cover
-                elif not await self._client.put_paramset(
-                    channel_address=channel_address,
-                    paramset_key=ParamsetKey.VALUES,
-                    values=paramset,
-                ):
-                    return False  # pragma: no cover
+                else:
+                    put_paramset_command = partial(
+                        self._client.put_paramset,
+                        channel_address=channel_address,
+                        paramset_key=ParamsetKey.VALUES,
+                        values=paramset,
+                        wait_for_callback=wait_for_callback,
+                    )
+                    if use_command_queue:
+                        await self._device.central.command_queue_handler.put(
+                            device_address=self._device.device_address,
+                            command=put_paramset_command,
+                        )
+                    elif not await put_paramset_command():
+                        return False  # pragma: no cover
         return True
 
 
-def bind_collector(func: _CallableT) -> _CallableT:
+def bind_collector(
+    wait_for_callback: int | None = WAIT_FOR_CALLBACK,
+    use_command_queue: bool = False,
+    use_put_paramset: bool = True,
+) -> Callable:
     """Decorate function to automatically add collector if not set."""
-    argument_index = getfullargspec(func).args.index(_COLLECTOR_ARGUMENT_NAME)
 
-    @wraps(func)
-    async def wrapper_collector(*args: Any, **kwargs: Any) -> Any:
-        """Wrap method to add collector."""
-        try:
-            collector_exists = args[argument_index] is not None
-        except IndexError:
-            collector_exists = kwargs.get(_COLLECTOR_ARGUMENT_NAME) is not None
+    def decorator_bind_collector(func: _CallableT) -> _CallableT:
+        """Decorate function to automatically add collector if not set."""
+        argument_index = getfullargspec(func).args.index(_COLLECTOR_ARGUMENT_NAME)
+
+        @wraps(func)
+        async def wrapper_collector(*args: Any, **kwargs: Any) -> Any:
+            """Wrap method to add collector."""
 
-        if collector_exists:
-            return_value = await func(*args, **kwargs)
-        else:
-            collector = CallParameterCollector(client=args[0].device.client)
-            kwargs[_COLLECTOR_ARGUMENT_NAME] = collector
-            return_value = await func(*args, **kwargs)
-            await collector.send_data()
-        return return_value
+            try:
+                collector_exists = args[argument_index] is not None
+            except IndexError:
+                collector_exists = kwargs.get(_COLLECTOR_ARGUMENT_NAME) is not None
+
+            if collector_exists:
+                return_value = await func(*args, **kwargs)
+            else:
+                collector = CallParameterCollector(device=args[0].device)
+                kwargs[_COLLECTOR_ARGUMENT_NAME] = collector
+                return_value = await func(*args, **kwargs)
+                await collector.send_data(
+                    wait_for_callback=wait_for_callback,
+                    use_command_queue=use_command_queue,
+                    use_put_paramset=use_put_paramset,
+                )
+            return return_value
+
+        return wrapper_collector  # type: ignore[return-value]
 
-    return wrapper_collector  # type: ignore[return-value]
+    return decorator_bind_collector
```

### Comparing `hahomematic-2024.4.9b2/hahomematic/platforms/event.py` & `hahomematic-2024.5.0/hahomematic/platforms/event.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 from hahomematic.const import (
     CLICK_EVENTS,
     DEVICE_ERROR_EVENTS,
     ENTITY_EVENTS,
     IMPULSE_EVENTS,
     Description,
     EntityUsage,
-    EventType,
     HmPlatform,
+    HomematicEventType,
     Operations,
     ParamsetKey,
 )
 from hahomematic.platforms import device as hmd
 from hahomematic.platforms.decorators import config_property
 from hahomematic.platforms.entity import BaseParameterEntity
 from hahomematic.platforms.support import EntityNameData, generate_unique_id, get_event_name
@@ -28,15 +28,15 @@
 _LOGGER: Final = logging.getLogger(__name__)
 
 
 class GenericEvent(BaseParameterEntity[Any, Any]):
     """Base class for events."""
 
     _platform = HmPlatform.EVENT
-    _event_type: EventType
+    _event_type: HomematicEventType
 
     def __init__(
         self,
         device: hmd.HmDevice,
         unique_id: str,
         channel_address: str,
         parameter: str,
@@ -56,29 +56,29 @@
     def usage(self) -> EntityUsage:
         """Return the entity usage."""
         if (force_enabled := self._enabled_by_channel_operation_mode) is None:
             return self._usage
         return EntityUsage.EVENT if force_enabled else EntityUsage.NO_CREATE
 
     @config_property
-    def event_type(self) -> EventType:
+    def event_type(self) -> HomematicEventType:
         """Return the event_type of the event."""
         return self._event_type
 
     async def event(self, value: Any) -> None:
         """Handle event for which this handler has subscribed."""
         if self.event_type in ENTITY_EVENTS:
             self.fire_entity_updated_callback(parameter=self.parameter.lower())
         self._set_last_updated()
         self.fire_event(value)
 
     @loop_check
     def fire_event(self, value: Any) -> None:
         """Do what is needed to fire an event."""
-        self._central.fire_ha_event_callback(
+        self._central.fire_homematic_callback(
             event_type=self.event_type, event_data=self.get_event_data(value=value)
         )
 
     def _get_entity_name(self) -> EntityNameData:
         """Create the name for the entity."""
         return get_event_name(
             central=self._central,
@@ -91,21 +91,21 @@
         """Generate the usage for the entity."""
         return EntityUsage.EVENT
 
 
 class ClickEvent(GenericEvent):
     """class for handling click events."""
 
-    _event_type = EventType.KEYPRESS
+    _event_type = HomematicEventType.KEYPRESS
 
 
 class DeviceErrorEvent(GenericEvent):
     """class for handling device error events."""
 
-    _event_type = EventType.DEVICE_ERROR
+    _event_type = HomematicEventType.DEVICE_ERROR
 
     async def event(self, value: Any) -> None:
         """Handle event for which this handler has subscribed."""
 
         old_value, new_value = self.write_value(value=value)
 
         if (
@@ -123,15 +123,15 @@
         ):
             self.fire_event(value=new_value)
 
 
 class ImpulseEvent(GenericEvent):
     """class for handling impulse events."""
 
-    _event_type = EventType.IMPULSE
+    _event_type = HomematicEventType.IMPULSE
 
 
 def create_event_and_append_to_device(
     device: hmd.HmDevice, channel_address: str, parameter: str, parameter_data: Mapping[str, Any]
 ) -> None:
     """Create action event entity."""
     if device.central.parameter_visibility.parameter_is_ignored(
```

### Comparing `hahomematic-2024.4.9b2/hahomematic/platforms/generic/__init__.py` & `hahomematic-2024.5.0/hahomematic/platforms/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b2/hahomematic/platforms/generic/action.py` & `hahomematic-2024.5.0/hahomematic/platforms/generic/action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b2/hahomematic/platforms/generic/binary_sensor.py` & `hahomematic-2024.5.0/hahomematic/platforms/generic/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b2/hahomematic/platforms/generic/button.py` & `hahomematic-2024.5.0/hahomematic/platforms/generic/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b2/hahomematic/platforms/generic/entity.py` & `hahomematic-2024.5.0/hahomematic/platforms/generic/entity.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 
 from collections.abc import Mapping
 import logging
 from typing import Any, Final
 
-from hahomematic.const import CallSource, EntityUsage, EventType, Parameter, ParamsetKey
+from hahomematic.const import CallSource, EntityUsage, HomematicEventType, Parameter, ParamsetKey
 from hahomematic.platforms import device as hmd, entity as hme
 from hahomematic.platforms.decorators import config_property
 from hahomematic.platforms.support import EntityNameData, get_entity_name
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 
@@ -47,17 +47,15 @@
         if (force_enabled := self._enabled_by_channel_operation_mode) is None:
             return self._usage
         return EntityUsage.ENTITY if force_enabled else EntityUsage.NO_CREATE
 
     async def event(self, value: Any) -> None:
         """Handle event for which this entity has subscribed."""
         self.device.client.last_value_send_cache.remove_last_value_send(
-            paramset_key=self.paramset_key,
-            channel_address=self.channel_address,
-            parameter=self.parameter,
+            entity_key=self.entity_key,
             value=value,
         )
         old_value, new_value = self.write_value(value=value)
         if old_value == new_value:
             return
 
         # reload paramset_descriptions, if value has changed
@@ -75,16 +73,16 @@
 
         # send device availability events
         if self._parameter in (
             Parameter.UN_REACH,
             Parameter.STICKY_UN_REACH,
         ):
             self._device.fire_device_updated_callback(self._unique_id)
-            self._central.fire_ha_event_callback(
-                event_type=EventType.DEVICE_AVAILABILITY,
+            self._central.fire_homematic_callback(
+                event_type=HomematicEventType.DEVICE_AVAILABILITY,
                 event_data=self.get_event_data(new_value),
             )
 
     async def send_value(
         self,
         value: hme.InputParameterT,
         collector: hme.CallParameterCollector | None = None,
```

### Comparing `hahomematic-2024.4.9b2/hahomematic/platforms/generic/number.py` & `hahomematic-2024.5.0/hahomematic/platforms/generic/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b2/hahomematic/platforms/generic/select.py` & `hahomematic-2024.5.0/hahomematic/platforms/generic/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b2/hahomematic/platforms/generic/sensor.py` & `hahomematic-2024.5.0/hahomematic/platforms/generic/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b2/hahomematic/platforms/generic/switch.py` & `hahomematic-2024.5.0/hahomematic/platforms/generic/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b2/hahomematic/platforms/hub/__init__.py` & `hahomematic-2024.5.0/hahomematic/platforms/hub/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 import logging
 from typing import Final
 
 from hahomematic import central as hmcu
 from hahomematic.const import (
     HUB_PLATFORMS,
     Backend,
+    BackendSystemEvent,
     HmPlatform,
     ProgramData,
-    SystemEvent,
     SystemVariableData,
     SysvarType,
 )
 from hahomematic.platforms.hub.binary_sensor import HmSysvarBinarySensor
 from hahomematic.platforms.hub.button import HmProgramButton
 from hahomematic.platforms.hub.entity import GenericHubEntity, GenericSystemVariable
 from hahomematic.platforms.hub.number import HmSysvarNumber
@@ -80,16 +80,16 @@
         for program_data in programs:
             if entity := self._central.get_program_button(pid=program_data.pid):
                 entity.update_data(data=program_data)
             else:
                 new_programs.append(self._create_program(data=program_data))
 
         if new_programs:
-            self._central.fire_system_event_callback(
-                system_event=SystemEvent.HUB_REFRESHED,
+            self._central.fire_backend_system_callback(
+                system_event=BackendSystemEvent.HUB_REFRESHED,
                 new_hub_entities=_get_new_hub_entities(entities=new_programs),
             )
 
     async def _update_sysvar_entities(self, include_internal: bool = True) -> None:
         """Retrieve all variable data and update hmvariable values."""
         variables: tuple[SystemVariableData, ...] = ()
         if client := self._central.primary_client:
@@ -122,16 +122,16 @@
 
             if entity := self._central.get_sysvar_entity(name=name):
                 entity.write_value(value)
             else:
                 new_sysvars.append(self._create_system_variable(data=sysvar))
 
         if new_sysvars:
-            self._central.fire_system_event_callback(
-                system_event=SystemEvent.HUB_REFRESHED,
+            self._central.fire_backend_system_callback(
+                system_event=BackendSystemEvent.HUB_REFRESHED,
                 new_hub_entities=_get_new_hub_entities(entities=new_sysvars),
             )
 
     def _create_program(self, data: ProgramData) -> HmProgramButton:
         """Create program as entity."""
         program_button = HmProgramButton(central=self._central, data=data)
         self._central.add_program_button(program_button=program_button)
```

### Comparing `hahomematic-2024.4.9b2/hahomematic/platforms/hub/binary_sensor.py` & `hahomematic-2024.5.0/hahomematic/platforms/hub/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b2/hahomematic/platforms/hub/button.py` & `hahomematic-2024.5.0/hahomematic/platforms/hub/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b2/hahomematic/platforms/hub/entity.py` & `hahomematic-2024.5.0/hahomematic/platforms/hub/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         self._old_value: bool | float | int | str | None = None
 
     @property
     def available(self) -> bool:
         """Return the availability of the device."""
         return self.central.available
 
-    @value_property
+    @property
     def old_value(self) -> Any | None:
         """Return the old value."""
         return self._old_value
 
     @value_property
     def value(self) -> Any | None:
         """Return the value."""
```

### Comparing `hahomematic-2024.4.9b2/hahomematic/platforms/hub/number.py` & `hahomematic-2024.5.0/hahomematic/platforms/hub/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b2/hahomematic/platforms/hub/select.py` & `hahomematic-2024.5.0/hahomematic/platforms/hub/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b2/hahomematic/platforms/hub/sensor.py` & `hahomematic-2024.5.0/hahomematic/platforms/hub/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b2/hahomematic/platforms/hub/text.py` & `hahomematic-2024.5.0/hahomematic/platforms/hub/text.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b2/hahomematic/platforms/support.py` & `hahomematic-2024.5.0/hahomematic/platforms/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b2/hahomematic/platforms/update.py` & `hahomematic-2024.5.0/hahomematic/platforms/update.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 
 See https://www.home-assistant.io/integrations/update/.
 """
 
 from __future__ import annotations
 
 from collections.abc import Callable
+from functools import partial
 from typing import Final
 
-from hahomematic.const import HmPlatform
+from hahomematic.const import CALLBACK_TYPE, DEFAULT_CUSTOM_ID, HmPlatform
 from hahomematic.exceptions import HaHomematicException
 from hahomematic.platforms import device as hmd
 from hahomematic.platforms.decorators import config_property, value_property
-from hahomematic.platforms.entity import DEFAULT_CUSTOM_ID, CallbackEntity
+from hahomematic.platforms.entity import CallbackEntity
 from hahomematic.platforms.support import generate_unique_id
 
 
 class HmUpdate(CallbackEntity):
     """
     Implementation of a update.
 
@@ -68,31 +69,28 @@
         return self._device.available_firmware
 
     @value_property
     def firmware_update_state(self) -> str | None:
         """Latest version available for install."""
         return self._device.firmware_update_state
 
-    def register_entity_updated_callback(
-        self, entity_updated_callback: Callable, custom_id: str
-    ) -> None:
+    def register_entity_updated_callback(self, cb: Callable, custom_id: str) -> CALLBACK_TYPE:
         """Register update callback."""
-        self._device.register_firmware_update_callback(entity_updated_callback)
+        self._device.register_firmware_update_callback(cb)
         if custom_id != DEFAULT_CUSTOM_ID:
             if self._custom_id is not None:
                 raise HaHomematicException(
                     f"REGISTER_UPDATE_CALLBACK failed: hm_entity: {self.full_name} is already registered by {self._custom_id}"
                 )
             self._custom_id = custom_id
+        return partial(self._unregister_entity_updated_callback, cb, custom_id)
 
-    def unregister_entity_updated_callback(
-        self, entity_updated_callback: Callable, custom_id: str
-    ) -> None:
+    def _unregister_entity_updated_callback(self, cb: Callable, custom_id: str) -> None:
         """Unregister update callback."""
-        self._device.unregister_firmware_update_callback(entity_updated_callback)
+        self._device.unregister_firmware_update_callback(cb)
         if custom_id is not None:
             self._custom_id = None
 
     async def update_firmware(self, refresh_after_update_intervals: tuple[int, ...]) -> bool:
         """Turn the update on."""
         return await self._device.update_firmware(
             refresh_after_update_intervals=refresh_after_update_intervals
```

### Comparing `hahomematic-2024.4.9b2/hahomematic/rega_scripts/fetch_all_device_data.fn` & `hahomematic-2024.5.0/hahomematic/rega_scripts/fetch_all_device_data.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b2/hahomematic/rega_scripts/get_serial.fn` & `hahomematic-2024.5.0/hahomematic/rega_scripts/get_serial.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b2/hahomematic/rega_scripts/get_system_variables_ext_marker.fn` & `hahomematic-2024.5.0/hahomematic/rega_scripts/get_system_variables_ext_marker.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b2/hahomematic/support.py` & `hahomematic-2024.5.0/hahomematic/support.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import socket
 import ssl
 import sys
 from typing import Any, Final
 
 from hahomematic.const import (
     CCU_PASSWORD_PATTERN,
+    ENTITY_KEY,
     FILE_DEVICES,
     FILE_PARAMSETS,
     IDENTIFIER_SEPARATOR,
     INIT_DATETIME,
     MAX_CACHE_AGE,
     NO_CACHE_ENTRY,
     SysvarType,
@@ -166,14 +167,19 @@
 
 
 def get_channel_no(address: str) -> int | None:
     """Return the channel part of an address."""
     return get_split_channel_address(channel_address=address)[1]
 
 
+def get_entity_key(channel_address: str, parameter: str) -> ENTITY_KEY:
+    """Return an entity key."""
+    return (str(channel_address), str(parameter))
+
+
 @lru_cache(maxsize=2048)
 def get_split_channel_address(channel_address: str) -> tuple[str, int | None]:
     """Return the device part of an address."""
     if ":" in channel_address:
         device_address, channel_no = channel_address.split(":")
         if channel_no in (None, "None"):
             return device_address, None
```

### Comparing `hahomematic-2024.4.9b2/hahomematic.egg-info/PKG-INFO` & `hahomematic-2024.5.0/hahomematic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2024.4.9b2
+Version: 2024.5.0
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2024.4.9b2/hahomematic.egg-info/SOURCES.txt` & `hahomematic-2024.5.0/hahomematic.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 hahomematic.egg-info/requires.txt
 hahomematic.egg-info/top_level.txt
 hahomematic/caches/__init__.py
 hahomematic/caches/dynamic.py
 hahomematic/caches/persistent.py
 hahomematic/caches/visibility.py
 hahomematic/central/__init__.py
+hahomematic/central/command_queue.py
 hahomematic/central/decorators.py
 hahomematic/central/xml_rpc_server.py
 hahomematic/client/__init__.py
 hahomematic/client/json_rpc.py
 hahomematic/client/xml_rpc.py
 hahomematic/platforms/__init__.py
 hahomematic/platforms/decorators.py
```

### Comparing `hahomematic-2024.4.9b2/hahomematic_support/client_local.py` & `hahomematic-2024.5.0/hahomematic_support/client_local.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 import importlib.resources
 import os
 from typing import Any, Final, cast
 
 import orjson
 
 from hahomematic.client import _LOGGER, Client, _ClientConfig
+from hahomematic.config import WAIT_FOR_CALLBACK
 from hahomematic.const import (
     DEFAULT_ENCODING,
+    ENTITY_KEY,
     CallSource,
     InterfaceName,
     ProductGroup,
     ProgramData,
     ProxyInitState,
     SystemInformation,
     SystemVariableData,
@@ -191,22 +193,25 @@
 
     async def set_value(
         self,
         channel_address: str,
         paramset_key: str,
         parameter: str,
         value: Any,
+        wait_for_callback: int | None = WAIT_FOR_CALLBACK,
         rx_mode: str | None = None,
-    ) -> bool:
+    ) -> set[ENTITY_KEY]:
         """Set single value on paramset VALUES."""
-        await self.central.event(self.interface_id, channel_address, parameter, value)
-        self._last_value_send_cache.add_set_value(
+        # store the send value in the last_value_send_cache
+        result = self._last_value_send_cache.add_set_value(
             channel_address=channel_address, parameter=parameter, value=value
         )
-        return True
+        # fire an event to fake the state change for a simple parameter
+        await self.central.event(self.interface_id, channel_address, parameter, value)
+        return result
 
     async def get_paramset(self, address: str, paramset_key: str) -> Any:
         """
         Return a paramset from CCU.
 
         Address is usually the channel_address,
         but for bidcos devices there is a master paramset at the device.
@@ -242,30 +247,33 @@
         return self._paramset_descriptions_cache.get(address, {}).get(paramset_key)
 
     async def put_paramset(
         self,
         channel_address: str,
         paramset_key: str,
         values: Any,
+        wait_for_callback: int | None = WAIT_FOR_CALLBACK,
         rx_mode: str | None = None,
-    ) -> bool:
+    ) -> set[ENTITY_KEY]:
         """
         Set paramsets manually.
 
         Address is usually the channel_address,
         but for bidcos devices there is a master paramset at the device.
         """
+        # store the send value in the last_value_send_cache
+        result = self._last_value_send_cache.add_put_paramset(
+            channel_address=channel_address, paramset_key=paramset_key, values=values
+        )
+        # fire an event to fake the state change for the content of a paramset
         for parameter in values:
             await self.central.event(
                 self.interface_id, channel_address, parameter, values[parameter]
             )
-        self._last_value_send_cache.add_put_paramset(
-            channel_address=channel_address, paramset_key=paramset_key, values=values
-        )
-        return True
+        return result
 
     async def _load_all_json_files(
         self,
         anchor: str,
         resource: str,
         include_list: list[str] | None = None,
         exclude_list: list[str] | None = None,
```

### Comparing `hahomematic-2024.4.9b2/pyproject.toml` & `hahomematic-2024.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=69.2.0", "wheel~=0.43.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "hahomematic"
-version     = "2024.4.9b2"
+version     = "2024.5.0"
 license     = {text = "MIT License"}
 description = "Homematic interface for Home Assistant running on Python 3."
 readme      = "README.md"
 authors     = [
     {name = "Daniel Perna", email = "danielperna84@gmail.com"},
     {name = "SukramJ", email = "sukramj@icloud.com"},
 ]
```

### Comparing `hahomematic-2024.4.9b2/tests/test_action.py` & `hahomematic-2024.5.0/tests/test_action.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,49 @@
 """Tests for action entities of hahomematic."""
 
 from __future__ import annotations
 
 from typing import cast
-from unittest.mock import call
+from unittest.mock import Mock, call
 
 import pytest
 
+from hahomematic.central import CentralUnit
+from hahomematic.client import Client
 from hahomematic.const import EntityUsage
 from hahomematic.platforms.generic.action import HmAction
 
 from tests import helper
 
 TEST_DEVICES: dict[str, str] = {
     "VCU9724704": "HmIP-DLD.json",
 }
 
 # pylint: disable=protected-access
 
 
 @pytest.mark.asyncio()
-async def test_hmaction(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_hmaction(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test HmAction."""
-    central, mock_client = await factory.get_default_central(TEST_DEVICES)
+    central, mock_client, _ = central_client_factory
     action: HmAction = cast(
         HmAction,
         central.get_generic_entity("VCU9724704:1", "LOCK_TARGET_LEVEL"),
     )
     assert action.usage == EntityUsage.NO_CREATE
     assert action.is_readable is False
     assert action.value is None
```

### Comparing `hahomematic-2024.4.9b2/tests/test_binary_sensor.py` & `hahomematic-2024.5.0/tests/test_binary_sensor.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,50 @@
 """Tests for binary_sensor entities of hahomematic."""
 
 from __future__ import annotations
 
 from typing import cast
+from unittest.mock import Mock
 
 import pytest
 
+from hahomematic.central import CentralUnit
+from hahomematic.client import Client
 from hahomematic.const import EntityUsage
 from hahomematic.platforms.generic.binary_sensor import HmBinarySensor
 from hahomematic.platforms.hub.binary_sensor import HmSysvarBinarySensor
 
 from tests import const, helper
 
 TEST_DEVICES: dict[str, str] = {
     "VCU5864966": "HmIP-SWDO-I.json",
 }
 
 # pylint: disable=protected-access
 
 
 @pytest.mark.asyncio()
-async def test_hmbinarysensor(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_hmbinarysensor(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test HmBinarySensor."""
-    central, mock_client = await factory.get_default_central(TEST_DEVICES)
+    central, mock_client, _ = central_client_factory
     binary_sensor: HmBinarySensor = cast(
         HmBinarySensor,
         central.get_generic_entity("VCU5864966:1", "STATE"),
     )
     assert binary_sensor.usage == EntityUsage.ENTITY
     assert binary_sensor.value is False
     assert binary_sensor.is_writeable is False
@@ -40,17 +58,32 @@
 
     call_count = len(mock_client.method_calls)
     await binary_sensor.send_value(True)
     assert call_count == len(mock_client.method_calls)
 
 
 @pytest.mark.asyncio()
-async def test_hmsysvarbinarysensor(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        ({}, True, True, False, None, None),
+    ],
+)
+async def test_hmsysvarbinarysensor(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test HmSysvarBinarySensor."""
-    central, _ = await factory.get_default_central({}, add_sysvars=True)
+    central, _, _ = central_client_factory
     binary_sensor: HmSysvarBinarySensor = cast(
         HmSysvarBinarySensor,
         central.get_sysvar_entity("sv_logic"),
     )
     assert binary_sensor.name == "sv_logic"
     assert binary_sensor.full_name == "CentralTest_sv_logic"
     assert binary_sensor.value is False
```

### Comparing `hahomematic-2024.4.9b2/tests/test_button.py` & `hahomematic-2024.5.0/tests/test_button.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,50 @@
 """Tests for button entities of hahomematic."""
 
 from __future__ import annotations
 
 from typing import cast
-from unittest.mock import call
+from unittest.mock import Mock, call
 
 import pytest
 
+from hahomematic.central import CentralUnit
+from hahomematic.client import Client
 from hahomematic.const import EntityUsage, ProgramData
 from hahomematic.platforms.generic.button import HmButton
 from hahomematic.platforms.hub.button import HmProgramButton
 
 from tests import helper
 
 TEST_DEVICES: dict[str, str] = {
     "VCU1437294": "HmIP-SMI.json",
 }
 
 # pylint: disable=protected-access
 
 
 @pytest.mark.asyncio()
-async def test_hmbutton(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_hmbutton(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test HmButton."""
-    central, mock_client = await factory.get_default_central(TEST_DEVICES)
+    central, mock_client, _ = central_client_factory
     button: HmButton = cast(
         HmButton,
         central.get_generic_entity("VCU1437294:1", "RESET_MOTION"),
     )
     assert button.usage == EntityUsage.ENTITY
     assert button.available is True
     assert button.is_readable is False
@@ -44,17 +61,32 @@
 
     call_count = len(mock_client.method_calls)
     await button.press()
     assert (call_count + 1) == len(mock_client.method_calls)
 
 
 @pytest.mark.asyncio()
-async def test_hmprogrambutton(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        ({}, True, False, True, None, None),
+    ],
+)
+async def test_hmprogrambutton(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test HmProgramButton."""
-    central, mock_client = await factory.get_default_central({}, add_programs=True)
+    central, mock_client, _ = central_client_factory
     button: HmProgramButton = cast(HmProgramButton, central.get_program_button("pid1"))
     assert button.usage == EntityUsage.ENTITY
     assert button.available is True
     assert button.is_active is True
     assert button.is_internal is False
     assert button.ccu_program_name == "p1"
     assert button.name == "P_p1"
```

### Comparing `hahomematic-2024.4.9b2/tests/test_central.py` & `hahomematic-2024.5.0/tests/test_central.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """Test the HaHomematic central."""
 
 from __future__ import annotations
 
 from datetime import datetime
 from typing import Any
-from unittest.mock import call, patch
+from unittest.mock import Mock, call, patch
 
 import pytest
 
+from hahomematic.central import CentralUnit
+from hahomematic.client import Client
 from hahomematic.config import PING_PONG_MISMATCH_COUNT
 from hahomematic.const import (
     DATETIME_FORMAT_MILLIS,
     EVENT_AVAILABLE,
     EntityUsage,
-    EventType,
     HmPlatform,
+    HomematicEventType,
     InterfaceEventType,
     Parameter,
     ParamsetKey,
 )
 from hahomematic.exceptions import HaHomematicException, NoClients
 
 from tests import const, helper
@@ -28,54 +30,112 @@
     "VCU6354483": "HmIP-STHD.json",
 }
 
 # pylint: disable=protected-access
 
 
 @pytest.mark.asyncio()
-async def test_central_basics(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_central_basics(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test central basics."""
-    central, client = await factory.get_default_central(TEST_DEVICES)
+    central, client, _ = central_client_factory
     assert central.central_url == "http://127.0.0.1"
     assert central.is_alive is True
     assert central.system_information.serial == "0815_4711"
     assert central.version == "0"
     system_information = await central.validate_config_and_get_system_information()
     assert system_information.serial == "0815_4711"
     device = central.get_device("VCU2128127")
     assert device
     entities = central.get_readable_generic_entities()
     assert entities
 
 
 @pytest.mark.asyncio()
-async def test_device_get_entities(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, True, True, None, None),
+    ],
+)
+async def test_device_get_entities(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test central/device get_entities."""
-    central, _ = await factory.get_default_central(
-        TEST_DEVICES, add_sysvars=True, add_programs=True
-    )
+    central, _, _ = central_client_factory
     entities = central.get_entities()
     assert entities
 
     entities_reg = central.get_entities(registered=True)
     assert entities_reg == ()
 
 
 @pytest.mark.asyncio()
-async def test_device_export(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_device_export(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test device export."""
-    central, _ = await factory.get_default_central(TEST_DEVICES)
+    central, _, _ = central_client_factory
     device = central.get_device(address="VCU6354483")
     await device.export_device_definition()
 
 
 @pytest.mark.asyncio()
-async def test_identify_callback_ip(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_identify_callback_ip(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test identify_callback_ip."""
-    central, _ = await factory.get_default_central(TEST_DEVICES)
+    central, _, _ = central_client_factory
     assert await central._identify_callback_ip(port=54321) == "127.0.0.1"
     central.config.host = "no_host"
     assert await central._identify_callback_ip(port=54321) == "127.0.0.1"
 
 
 @pytest.mark.parametrize(
     ("line", "parameter", "channel_no", "paramset_key", "expected_result"),
@@ -107,26 +167,29 @@
     paramset_key: str,
     expected_result: bool,
 ) -> None:
     """Test device un ignore."""
     central, _ = await factory.get_default_central(
         {"VCU3609622": "HmIP-eTRV-2.json"}, un_ignore_list=[line]
     )
-    assert (
-        central.parameter_visibility.parameter_is_un_ignored(
-            device_type="HmIP-eTRV-2",
-            channel_no=channel_no,
-            paramset_key=paramset_key,
-            parameter=parameter,
-        )
-        is expected_result
-    )
-    generic_entity = central.get_generic_entity(f"VCU3609622:{channel_no}", parameter)
-    if generic_entity:
-        assert generic_entity.usage == EntityUsage.ENTITY
+    try:
+        assert (
+            central.parameter_visibility.parameter_is_un_ignored(
+                device_type="HmIP-eTRV-2",
+                channel_no=channel_no,
+                paramset_key=paramset_key,
+                parameter=parameter,
+            )
+            is expected_result
+        )
+        generic_entity = central.get_generic_entity(f"VCU3609622:{channel_no}", parameter)
+        if generic_entity:
+            assert generic_entity.usage == EntityUsage.ENTITY
+    finally:
+        await central.stop()
 
 
 @pytest.mark.parametrize(
     ("line", "parameter", "channel_no", "paramset_key", "expected_result"),
     [
         ("LEVEL", "LEVEL", 3, "VALUES", True),
         ("LEVEL@HmIP-BROLL:3:VALUES", "LEVEL", 3, "VALUES", False),
@@ -145,27 +208,30 @@
     paramset_key: str,
     expected_result: bool,
 ) -> None:
     """Test device un ignore."""
     central, _ = await factory.get_default_central(
         {"VCU8537918": "HmIP-BROLL.json"}, un_ignore_list=[line]
     )
-    assert (
-        central.parameter_visibility.parameter_is_un_ignored(
-            device_type="HmIP-BROLL",
-            channel_no=channel_no,
-            paramset_key=paramset_key,
-            parameter=parameter,
-        )
-        is expected_result
-    )
-    generic_entity = central.get_generic_entity(f"VCU8537918:{channel_no}", parameter)
-    if expected_result:
-        assert generic_entity
-        assert generic_entity.usage == EntityUsage.ENTITY
+    try:
+        assert (
+            central.parameter_visibility.parameter_is_un_ignored(
+                device_type="HmIP-BROLL",
+                channel_no=channel_no,
+                paramset_key=paramset_key,
+                parameter=parameter,
+            )
+            is expected_result
+        )
+        generic_entity = central.get_generic_entity(f"VCU8537918:{channel_no}", parameter)
+        if expected_result:
+            assert generic_entity
+            assert generic_entity.usage == EntityUsage.ENTITY
+    finally:
+        await central.stop()
 
 
 @pytest.mark.parametrize(
     ("line", "parameter", "channel_no", "paramset_key", "expected_result"),
     [
         (
             "GLOBAL_BUTTON_LOCK@HM-TC-IT-WM-W-EU:MASTER",
@@ -206,29 +272,32 @@
     paramset_key: str,
     expected_result: bool,
 ) -> None:
     """Test device un ignore."""
     central, _ = await factory.get_default_central(
         {"VCU0000341": "HM-TC-IT-WM-W-EU.json"}, un_ignore_list=[line]
     )
-    assert (
-        central.parameter_visibility.parameter_is_un_ignored(
-            device_type="HM-TC-IT-WM-W-EU",
-            channel_no=channel_no,
-            paramset_key=paramset_key,
-            parameter=parameter,
-        )
-        is expected_result
-    )
-    generic_entity = central.get_generic_entity(
-        f"VCU0000341:{channel_no}" if channel_no else "VCU0000341", parameter
-    )
-    if expected_result:
-        assert generic_entity
-        assert generic_entity.usage == EntityUsage.ENTITY
+    try:
+        assert (
+            central.parameter_visibility.parameter_is_un_ignored(
+                device_type="HM-TC-IT-WM-W-EU",
+                channel_no=channel_no,
+                paramset_key=paramset_key,
+                parameter=parameter,
+            )
+            is expected_result
+        )
+        generic_entity = central.get_generic_entity(
+            f"VCU0000341:{channel_no}" if channel_no else "VCU0000341", parameter
+        )
+        if expected_result:
+            assert generic_entity
+            assert generic_entity.usage == EntityUsage.ENTITY
+    finally:
+        await central.stop()
 
 
 @pytest.mark.parametrize(
     ("lines", "parameter", "channel_no", "paramset_key", "expected_result"),
     [
         (["DECISION_VALUE:VALUES@all:all"], "DECISION_VALUE", 3, "VALUES", True),
         (["INHIBIT:VALUES@HM-ES-PMSw1-Pl:1"], "INHIBIT", 1, "VALUES", True),
@@ -290,30 +359,32 @@
     paramset_key: str,
     expected_result: bool,
 ) -> None:
     """Test device un ignore."""
     central, _ = await factory.get_default_central(
         {"VCU0000137": "HM-ES-PMSw1-Pl.json"}, un_ignore_list=lines
     )
-
-    assert (
-        central.parameter_visibility.parameter_is_un_ignored(
-            device_type="HM-ES-PMSw1-Pl",
-            channel_no=channel_no,
-            paramset_key=paramset_key,
-            parameter=parameter,
-        )
-        is expected_result
-    )
-    generic_entity = central.get_generic_entity(
-        f"VCU0000137:{channel_no}" if channel_no else "VCU0000137", parameter
-    )
-    if expected_result:
-        assert generic_entity
-        assert generic_entity.usage == EntityUsage.ENTITY
+    try:
+        assert (
+            central.parameter_visibility.parameter_is_un_ignored(
+                device_type="HM-ES-PMSw1-Pl",
+                channel_no=channel_no,
+                paramset_key=paramset_key,
+                parameter=parameter,
+            )
+            is expected_result
+        )
+        generic_entity = central.get_generic_entity(
+            f"VCU0000137:{channel_no}" if channel_no else "VCU0000137", parameter
+        )
+        if expected_result:
+            assert generic_entity
+            assert generic_entity.usage == EntityUsage.ENTITY
+    finally:
+        await central.stop()
 
 
 @pytest.mark.parametrize(
     ("lines", "device_type", "address", "expected_result"),
     [
         (
             ["ignore_HmIP-BWTH"],
@@ -343,92 +414,146 @@
     address: str,
     expected_result: bool,
 ) -> None:
     """Test device un ignore."""
     central, _ = await factory.get_default_central(
         {"VCU1769958": "HmIP-BWTH.json", "VCU3609622": "HmIP-eTRV-2.json"}, un_ignore_list=lines
     )
-
-    assert (
-        central.parameter_visibility.device_type_is_ignored(device_type=device_type)
-        is expected_result
-    )
-    if device := central.get_device(address=address):
-        if expected_result:
-            assert len(device.custom_entities) == 0
-        else:
-            assert len(device.custom_entities) > 0
+    try:
+        assert (
+            central.parameter_visibility.device_type_is_ignored(device_type=device_type)
+            is expected_result
+        )
+        if device := central.get_device(address=address):
+            if expected_result:
+                assert len(device.custom_entities) == 0
+            else:
+                assert len(device.custom_entities) > 0
+    finally:
+        await central.stop()
 
 
 @pytest.mark.asyncio()
-async def test_all_parameters(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_all_parameters(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test all_parameters."""
-    central, _ = await factory.get_default_central(TEST_DEVICES)
+    central, _, _ = central_client_factory
     parameters = central.paramset_descriptions.get_all_readable_parameters()
     assert parameters
     assert len(parameters) == 43
 
 
 @pytest.mark.asyncio()
-async def test_entities_by_platform(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_entities_by_platform(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test entities_by_platform."""
-    central, _ = await factory.get_default_central(TEST_DEVICES)
+    central, _, _ = central_client_factory
     ebp_sensor = central.get_entities(platform=HmPlatform.SENSOR)
     assert ebp_sensor
     assert len(ebp_sensor) == 12
 
     def _device_changed(self, *args: Any, **kwargs: Any) -> None:
         """Handle device state changes."""
 
-    ebp_sensor[0].register_entity_updated_callback(
-        entity_updated_callback=_device_changed, custom_id="some_id"
-    )
+    ebp_sensor[0].register_entity_updated_callback(cb=_device_changed, custom_id="some_id")
     ebp_sensor2 = central.get_entities(platform=HmPlatform.SENSOR, registered=False)
     assert ebp_sensor2
     assert len(ebp_sensor2) == 11
 
 
 @pytest.mark.asyncio()
-async def test_hub_entities_by_platform(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        ({}, True, True, True, None, None),
+    ],
+)
+async def test_hub_entities_by_platform(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test hub_entities_by_platform."""
-    central, _ = await factory.get_default_central({}, add_programs=True, add_sysvars=True)
+    central, _, _ = central_client_factory
     ebp_sensor = central.get_hub_entities(platform=HmPlatform.HUB_SENSOR)
     assert ebp_sensor
     assert len(ebp_sensor) == 4
 
     def _device_changed(self, *args: Any, **kwargs: Any) -> None:
         """Handle device state changes."""
 
-    ebp_sensor[0].register_entity_updated_callback(
-        entity_updated_callback=_device_changed, custom_id="some_id"
-    )
+    ebp_sensor[0].register_entity_updated_callback(cb=_device_changed, custom_id="some_id")
     ebp_sensor2 = central.get_hub_entities(
         platform=HmPlatform.HUB_SENSOR,
         registered=False,
     )
     assert ebp_sensor2
     assert len(ebp_sensor2) == 3
 
     ebp_sensor3 = central.get_hub_entities(platform=HmPlatform.HUB_BUTTON)
     assert ebp_sensor3
     assert len(ebp_sensor3) == 2
-    ebp_sensor3[0].register_entity_updated_callback(
-        entity_updated_callback=_device_changed, custom_id="some_id"
-    )
+    ebp_sensor3[0].register_entity_updated_callback(cb=_device_changed, custom_id="some_id")
     ebp_sensor4 = central.get_hub_entities(platform=HmPlatform.HUB_BUTTON, registered=False)
     assert ebp_sensor4
     assert len(ebp_sensor4) == 1
 
 
 @pytest.mark.asyncio()
-async def test_add_device(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, ["HmIP-BSM.json"], None),
+    ],
+)
+async def test_add_device(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test add_device."""
-    central, _ = await factory.get_default_central(
-        TEST_DEVICES, ignore_devices_on_create=["HmIP-BSM.json"]
-    )
+    central, _, _ = central_client_factory
     assert len(central._devices) == 1
     assert len(central.get_entities(exclude_no_create=False)) == 24
     assert len(central.device_descriptions._raw_device_descriptions.get(const.INTERFACE_ID)) == 9
     assert (
         len(central.paramset_descriptions._raw_paramset_descriptions.get(const.INTERFACE_ID)) == 2
     )
     dev_desc = helper.load_device_description(central=central, filename="HmIP-BSM.json")
@@ -440,17 +565,32 @@
         len(central.paramset_descriptions._raw_paramset_descriptions.get(const.INTERFACE_ID)) == 11
     )
     await central.add_new_devices(interface_id="NOT_ANINTERFACE_ID", device_descriptions=dev_desc)
     assert len(central._devices) == 2
 
 
 @pytest.mark.asyncio()
-async def test_delete_device(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_delete_device(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test device delete_device."""
-    central, _ = await factory.get_default_central(TEST_DEVICES)
+    central, _, _ = central_client_factory
     assert len(central._devices) == 2
     assert len(central.get_entities(exclude_no_create=False)) == 55
     assert len(central.device_descriptions._raw_device_descriptions.get(const.INTERFACE_ID)) == 20
     assert (
         len(central.paramset_descriptions._raw_paramset_descriptions.get(const.INTERFACE_ID)) == 11
     )
 
@@ -460,23 +600,43 @@
     assert len(central.device_descriptions._raw_device_descriptions.get(const.INTERFACE_ID)) == 9
     assert (
         len(central.paramset_descriptions._raw_paramset_descriptions.get(const.INTERFACE_ID)) == 2
     )
 
 
 @pytest.mark.asyncio()
-async def test_virtual_remote_delete(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (
+            {
+                "VCU4264293": "HmIP-RCV-50.json",
+                "VCU0000057": "HM-RCV-50.json",
+                "VCU0000001": "HMW-RCV-50.json",
+            },
+            True,
+            False,
+            False,
+            None,
+            None,
+        ),
+    ],
+)
+async def test_virtual_remote_delete(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test device delete."""
-    central, _ = await factory.get_default_central(
-        {
-            "VCU4264293": "HmIP-RCV-50.json",
-            "VCU0000057": "HM-RCV-50.json",
-            "VCU0000001": "HMW-RCV-50.json",
-        },
-    )
+    central, _, _ = central_client_factory
     assert len(central.get_virtual_remotes()) == 1
 
     assert central._get_virtual_remote("VCU0000057")
 
     await central.delete_device(interface_id=const.INTERFACE_ID, device_address="NOT_A_DEVICE_ID")
 
     assert len(central._devices) == 3
@@ -494,32 +654,49 @@
     await central.delete_device(interface_id=const.INTERFACE_ID, device_address="NOT_A_DEVICE_ID")
 
 
 @pytest.mark.asyncio()
 async def test_central_not_alive(factory: helper.Factory) -> None:
     """Test central other methods."""
     central, client = await factory.get_unpatched_default_central({}, do_mock_client=False)
-    mock_client = helper.get_mock(instance=client, available=False)
-
-    assert central.system_information.serial is None
-    assert central.is_alive is True
-
-    mock_client.is_callback_alive.return_value = False
-    with patch("hahomematic.client.create_client", return_value=mock_client):
-        await central.start()
-
-    assert central.available is False
-    assert central.system_information.serial == "0815_4711"
-    assert central.is_alive is False
+    try:
+        mock_client = helper.get_mock(instance=client, available=False)
+        assert central.system_information.serial is None
+        assert central.is_alive is True
+
+        mock_client.is_callback_alive.return_value = False
+        with patch("hahomematic.client.create_client", return_value=mock_client):
+            await central.start()
+
+        assert central.available is False
+        assert central.system_information.serial == "0815_4711"
+        assert central.is_alive is False
+    finally:
+        await central.stop()
 
 
 @pytest.mark.asyncio()
-async def test_central_callbacks(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_central_callbacks(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test central other methods."""
-    central, _ = await factory.get_default_central(TEST_DEVICES)
+    central, _, factory = central_client_factory
     central.fire_interface_event(
         interface_id="SOME_ID",
         interface_event_type=InterfaceEventType.CALLBACK,
         data={EVENT_AVAILABLE: False},
     )
     assert factory.ha_event_mock.call_args_list[-1] == call(
         "homematic.interface",
@@ -528,19 +705,32 @@
             "type": "callback",
             "data": {EVENT_AVAILABLE: False},
         },
     )
 
 
 @pytest.mark.asyncio()
-async def test_central_services(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, True, True, None, None),
+    ],
+)
+async def test_central_services(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test central fetch sysvar and programs."""
-    central, mock_client = await factory.get_default_central(
-        TEST_DEVICES, add_programs=True, add_sysvars=True
-    )
+    central, mock_client, _ = central_client_factory
     await central.fetch_program_data()
     assert mock_client.method_calls[-1] == call.get_all_programs(include_internal=False)
 
     await central.fetch_sysvar_data()
     assert mock_client.method_calls[-1] == call.get_all_system_variables(include_internal=True)
 
     assert len(mock_client.method_calls) == 39
@@ -618,104 +808,151 @@
 
 @pytest.mark.asyncio()
 async def test_central_direct(factory: helper.Factory) -> None:
     """Test central other methods."""
     central, client = await factory.get_unpatched_default_central(
         TEST_DEVICES, do_mock_client=False
     )
-    mock_client = helper.get_mock(instance=client, available=False)
-
-    assert central.system_information.serial is None
-    assert central.is_alive is True
-
-    with patch("hahomematic.client.create_client", return_value=mock_client):
-        await central.start()
-    assert await central._create_clients() is False
-
-    assert central.available is False
-    assert central.system_information.serial == "0815_4711"
-    assert len(central._devices) == 2
-    assert len(central.get_entities(exclude_no_create=False)) == 55
-    await central.stop()
+    try:
+        mock_client = helper.get_mock(instance=client, available=False)
+        assert central.system_information.serial is None
+        assert central.is_alive is True
+
+        with patch("hahomematic.client.create_client", return_value=mock_client):
+            await central.start()
+        assert await central._create_clients() is False
+
+        assert central.available is False
+        assert central.system_information.serial == "0815_4711"
+        assert len(central._devices) == 2
+        assert len(central.get_entities(exclude_no_create=False)) == 55
+    finally:
+        await central.stop()
 
 
 @pytest.mark.asyncio()
 async def test_central_without_interface_config(factory: helper.Factory) -> None:
     """Test central other methods."""
     central = await factory.get_raw_central(interface_config=None)
-    assert central.has_clients is False
+    try:
+        assert central.has_clients is False
 
-    with pytest.raises(NoClients):
-        await central.validate_config_and_get_system_information()
+        with pytest.raises(NoClients):
+            await central.validate_config_and_get_system_information()
 
-    with pytest.raises(HaHomematicException):
-        central.get_client("NOT_A_VALID_INTERFACE_ID")
-
-    with pytest.raises(Exception):
-        await central._create_devices()
+        with pytest.raises(HaHomematicException):
+            central.get_client("NOT_A_VALID_INTERFACE_ID")
 
-    await central.start()
-    assert central.has_clients is False
-
-    assert central.available is True
-    assert central.system_information.serial is None
-    assert len(central._devices) == 0
-    assert len(central.get_entities()) == 0
+        with pytest.raises(Exception):
+            await central._create_devices()
 
-    assert await central.get_system_variable(name="SysVar_Name") is None
-    assert central._get_virtual_remote("VCU4264293") is None
+        await central.start()
+        assert central.has_clients is False
 
-    await central.stop()
+        assert central.available is True
+        assert central.system_information.serial is None
+        assert len(central._devices) == 0
+        assert len(central.get_entities()) == 0
+
+        assert await central.get_system_variable(name="SysVar_Name") is None
+        assert central._get_virtual_remote("VCU4264293") is None
+    finally:
+        await central.stop()
 
 
 @pytest.mark.asyncio()
-async def test_ping_pong(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, False, False, False, None, None),
+    ],
+)
+async def test_ping_pong(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test central other methods."""
-    central, client = await factory.get_default_central(TEST_DEVICES, do_mock_client=False)
+    central, client, _ = central_client_factory
     interface_id = client.interface_id
     await client.check_connection_availability(handle_ping_pong=True)
     assert client.ping_pong_cache.pending_pong_count == 1
     for ts_stored in list(client.ping_pong_cache._pending_pongs):
         await central.event(
             interface_id,
             "",
             Parameter.PONG,
             f"{interface_id}#{ts_stored.strftime(DATETIME_FORMAT_MILLIS)}",
         )
     assert client.ping_pong_cache.pending_pong_count == 0
 
 
 @pytest.mark.asyncio()
-async def test_pending_pong_failure(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, False, False, False, None, None),
+    ],
+)
+async def test_pending_pong_failure(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test central other methods."""
-    central, client = await factory.get_default_central(TEST_DEVICES, do_mock_client=False)
+    central, client, factory = central_client_factory
     count = 0
     max_count = PING_PONG_MISMATCH_COUNT + 1
     while count < max_count:
         await client.check_connection_availability(handle_ping_pong=True)
         count += 1
     assert client.ping_pong_cache.pending_pong_count == max_count
     assert factory.ha_event_mock.mock_calls[-1] == call(
-        EventType.INTERFACE,
+        HomematicEventType.INTERFACE,
         {
             "data": {
                 "instance_name": "CentralTest",
                 "pong_mismatch_count": 16,
             },
             "interface_id": "CentralTest-BidCos-RF",
             "type": InterfaceEventType.PENDING_PONG,
         },
     )
     assert len(factory.ha_event_mock.mock_calls) == 9
 
 
 @pytest.mark.asyncio()
-async def test_unknown_pong_failure(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, False, False, False, None, None),
+    ],
+)
+async def test_unknown_pong_failure(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test central other methods."""
-    central, client = await factory.get_default_central(TEST_DEVICES, do_mock_client=False)
+    central, client, _ = central_client_factory
     interface_id = client.interface_id
     count = 0
     max_count = PING_PONG_MISMATCH_COUNT + 1
     while count < max_count:
         await central.event(
             interface_id,
             "",
@@ -724,29 +961,59 @@
         )
         count += 1
 
     assert client.ping_pong_cache.unknown_pong_count == 16
 
 
 @pytest.mark.asyncio()
-async def test_central_caches(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_central_caches(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test central cache."""
-    central, client = await factory.get_default_central(TEST_DEVICES)
+    central, client, _ = central_client_factory
     assert len(central.device_descriptions._raw_device_descriptions[client.interface_id]) == 20
     assert len(central.paramset_descriptions._raw_paramset_descriptions[client.interface_id]) == 11
     await central.clear_caches()
     assert central.device_descriptions._raw_device_descriptions.get(client.interface_id) is None
     assert (
         central.paramset_descriptions._raw_paramset_descriptions.get(client.interface_id) is None
     )
 
 
 @pytest.mark.asyncio()
-async def test_central_getter(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_central_getter(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test central getter."""
-    central, _ = await factory.get_default_central(TEST_DEVICES)
+    central, _, _ = central_client_factory
     assert central.get_device("123") is None
     assert central.get_custom_entity("123", 1) is None
     assert central.get_generic_entity("123", 1) is None
     assert central.get_event("123", 1) is None
     assert central.get_program_button("123") is None
     assert central.get_sysvar_entity("123") is None
```

### Comparing `hahomematic-2024.4.9b2/tests/test_central_pydevccu.py` & `hahomematic-2024.5.0/tests/test_central_pydevccu.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b2/tests/test_climate.py` & `hahomematic-2024.5.0/tests/test_climate.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """Tests for climate entities of hahomematic."""
 
 from __future__ import annotations
 
 from datetime import datetime
 from typing import cast
-from unittest.mock import call
+from unittest.mock import Mock, call
 
 from freezegun import freeze_time
 import pytest
 
+from hahomematic.central import CentralUnit
+from hahomematic.client import Client
+from hahomematic.config import WAIT_FOR_CALLBACK
 from hahomematic.const import EntityUsage, ParamsetKey
 from hahomematic.platforms.custom.climate import (
     CeIpThermostat,
     CeRfThermostat,
     CeSimpleRfThermostat,
     HvacAction,
     HvacMode,
@@ -31,17 +34,32 @@
     "VCU0000050": "HM-CC-RT-DN.json",
 }
 
 # pylint: disable=protected-access
 
 
 @pytest.mark.asyncio()
-async def test_cesimplerfthermostat(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_cesimplerfthermostat(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test CeSimpleRfThermostat."""
-    central, mock_client = await factory.get_default_central(TEST_DEVICES)
+    central, mock_client, _ = central_client_factory
     climate: CeSimpleRfThermostat = cast(
         CeSimpleRfThermostat, helper.get_prepared_custom_entity(central, "VCU0000054", 1)
     )
     assert climate.usage == EntityUsage.CE_PRIMARY
 
     assert climate.is_valid is False
     assert climate.state_uncertain is False
@@ -58,14 +76,15 @@
     assert climate.target_temperature is None
     await climate.set_temperature(12.0)
     last_call = call.set_value(
         channel_address="VCU0000054:2",
         paramset_key="VALUES",
         parameter="SETPOINT",
         value=12.0,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert mock_client.method_calls[-2] == last_call
     assert climate.target_temperature == 12.0
 
     assert climate.current_temperature is None
     await central.event(const.INTERFACE_ID, "VCU0000054:1", "TEMPERATURE", 11.0)
     assert climate.current_temperature == 11.0
@@ -89,17 +108,32 @@
     )
     assert mock_client.method_calls[-4] == last_call
     await climate.disable_away_mode()
     assert mock_client.method_calls[-4] == last_call
 
 
 @pytest.mark.asyncio()
-async def test_cerfthermostat(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_cerfthermostat(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test CeRfThermostat."""
-    central, mock_client = await factory.get_default_central(TEST_DEVICES)
+    central, mock_client, _ = central_client_factory
     climate: CeRfThermostat = cast(
         CeRfThermostat, helper.get_prepared_custom_entity(central, "VCU0000050", 4)
     )
     assert climate.usage == EntityUsage.CE_PRIMARY
     assert climate.min_temp == 5.0
     assert climate.max_temp == 30.5
     assert climate.supports_preset is True
@@ -114,43 +148,53 @@
     assert climate.target_temperature is None
     await climate.set_temperature(12.0)
     assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU0000050:4",
         paramset_key="VALUES",
         parameter="SET_TEMPERATURE",
         value=12.0,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert climate.target_temperature == 12.0
 
     assert climate.current_temperature is None
     await central.event(const.INTERFACE_ID, "VCU0000050:4", "ACTUAL_TEMPERATURE", 11.0)
     assert climate.current_temperature == 11.0
 
     assert climate.hvac_mode == HvacMode.AUTO
     assert climate.hvac_modes == (HvacMode.AUTO, HvacMode.HEAT, HvacMode.OFF)
     await climate.set_hvac_mode(HvacMode.HEAT)
     assert mock_client.method_calls[-1] == call.set_value(
-        channel_address="VCU0000050:4", paramset_key="VALUES", parameter="MANU_MODE", value=12.0
+        channel_address="VCU0000050:4",
+        paramset_key="VALUES",
+        parameter="MANU_MODE",
+        value=12.0,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU0000050:4", "CONTROL_MODE", ModeHmIP.MANU.value)
     assert climate.hvac_mode == HvacMode.HEAT
 
     await climate.set_hvac_mode(HvacMode.OFF)
     assert mock_client.method_calls[-2] == call.put_paramset(
         channel_address="VCU0000050:4",
         paramset_key="VALUES",
         values={"MANU_MODE": 12.0, "SET_TEMPERATURE": 4.5},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
 
     assert climate.hvac_mode == HvacMode.OFF
     assert climate.hvac_action == HvacAction.OFF
 
     await climate.set_hvac_mode(HvacMode.AUTO)
     assert mock_client.method_calls[-1] == call.set_value(
-        channel_address="VCU0000050:4", paramset_key="VALUES", parameter="AUTO_MODE", value=True
+        channel_address="VCU0000050:4",
+        paramset_key="VALUES",
+        parameter="AUTO_MODE",
+        value=True,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU0000050:4", "CONTROL_MODE", 0)
     await central.event(const.INTERFACE_ID, "VCU0000050:4", "SET_TEMPERATURE", 24.0)
     assert climate.hvac_mode == HvacMode.AUTO
 
     assert climate.preset_mode == PresetMode.NONE
     assert climate.preset_modes == (
@@ -161,32 +205,35 @@
     )
     await climate.set_preset_mode(PresetMode.BOOST)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU0000050:4",
         paramset_key="VALUES",
         parameter="BOOST_MODE",
         value=True,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU0000050:4", "CONTROL_MODE", 3)
     assert climate.preset_mode == PresetMode.BOOST
     await central.event(const.INTERFACE_ID, "VCU0000050:4", "CONTROL_MODE", 2)
     assert climate.preset_mode == PresetMode.AWAY
     await climate.set_preset_mode(PresetMode.COMFORT)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU0000050:4",
         paramset_key="VALUES",
         parameter="COMFORT_MODE",
         value=True,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await climate.set_preset_mode(PresetMode.ECO)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU0000050:4",
         paramset_key="VALUES",
         parameter="LOWERING_MODE",
         value=True,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
 
     await central.event(const.INTERFACE_ID, "VCU0000050:4", "CONTROL_MODE", 3)
     call_count = len(mock_client.method_calls)
     await climate.set_preset_mode(PresetMode.BOOST)
     assert call_count == len(mock_client.method_calls)
 
@@ -222,17 +269,32 @@
         paramset_key=ParamsetKey.VALUES,
         parameter="PARTY_MODE_SUBMIT",
         value="12.0,1260,02,03,23,1320,02,03,23",
     )
 
 
 @pytest.mark.asyncio()
-async def test_ceipthermostat(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_ceipthermostat(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test CeIpThermostat."""
-    central, mock_client = await factory.get_default_central(TEST_DEVICES)
+    central, mock_client, _ = central_client_factory
     climate: CeIpThermostat = cast(
         CeIpThermostat, helper.get_prepared_custom_entity(central, "VCU1769958", 1)
     )
     assert climate.usage == EntityUsage.CE_PRIMARY
     assert climate.min_temp == 5.0
     assert climate.max_temp == 30.5
     assert climate.supports_preset is True
@@ -250,14 +312,15 @@
     assert climate.target_temperature is None
     await climate.set_temperature(12.0)
     assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU1769958:1",
         paramset_key="VALUES",
         parameter="SET_POINT_TEMPERATURE",
         value=12.0,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert climate.target_temperature == 12.0
 
     assert climate.current_temperature is None
     await central.event(const.INTERFACE_ID, "VCU1769958:1", "ACTUAL_TEMPERATURE", 11.0)
     assert climate.current_temperature == 11.0
 
@@ -266,44 +329,51 @@
     assert climate.preset_mode == PresetMode.NONE
 
     await climate.set_hvac_mode(HvacMode.OFF)
     assert mock_client.method_calls[-2] == call.put_paramset(
         channel_address="VCU1769958:1",
         paramset_key="VALUES",
         values={"CONTROL_MODE": 1, "SET_POINT_TEMPERATURE": 4.5},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert climate.hvac_mode == HvacMode.OFF
     assert climate.hvac_action == HvacAction.OFF
 
     await climate.set_hvac_mode(HvacMode.HEAT)
     assert mock_client.method_calls[-2] == call.put_paramset(
         channel_address="VCU1769958:1",
         paramset_key="VALUES",
         values={"CONTROL_MODE": 1, "SET_POINT_TEMPERATURE": 5.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU1769958:1", "SET_POINT_MODE", ModeHmIP.MANU.value)
     assert climate.hvac_mode == HvacMode.HEAT
 
     assert climate.preset_mode == PresetMode.NONE
     assert climate.preset_modes == (
         PresetMode.BOOST,
         PresetMode.NONE,
     )
     await climate.set_preset_mode(PresetMode.BOOST)
     assert mock_client.method_calls[-2] == call.set_value(
-        channel_address="VCU1769958:1", paramset_key="VALUES", parameter="BOOST_MODE", value=True
+        channel_address="VCU1769958:1",
+        paramset_key="VALUES",
+        parameter="BOOST_MODE",
+        value=True,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU1769958:1", "BOOST_MODE", 1)
     assert climate.preset_mode == PresetMode.BOOST
 
     await climate.set_hvac_mode(HvacMode.AUTO)
     assert mock_client.method_calls[-2] == call.put_paramset(
         channel_address="VCU1769958:1",
         paramset_key="VALUES",
         values={"BOOST_MODE": False, "CONTROL_MODE": 0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU1769958:1", "SET_POINT_MODE", ModeHmIP.AUTO.value)
     await central.event(const.INTERFACE_ID, "VCU1769958:1", "BOOST_MODE", 1)
     assert climate.hvac_mode == HvacMode.AUTO
     assert climate.preset_modes == (
         PresetMode.BOOST,
         PresetMode.NONE,
@@ -312,23 +382,31 @@
         "week_program_3",
         "week_program_4",
         "week_program_5",
         "week_program_6",
     )
     await climate.set_preset_mode(PresetMode.NONE)
     assert mock_client.method_calls[-2] == call.set_value(
-        channel_address="VCU1769958:1", paramset_key="VALUES", parameter="BOOST_MODE", value=False
+        channel_address="VCU1769958:1",
+        paramset_key="VALUES",
+        parameter="BOOST_MODE",
+        value=False,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU1769958:1", "SET_POINT_MODE", ModeHmIP.AWAY.value)
     assert climate.preset_mode == PresetMode.AWAY
 
     await central.event(const.INTERFACE_ID, "VCU1769958:1", "SET_POINT_MODE", ModeHmIP.AUTO.value)
     await climate.set_preset_mode(PresetMode.WEEK_PROGRAM_1)
     assert mock_client.method_calls[-2] == call.set_value(
-        channel_address="VCU1769958:1", paramset_key="VALUES", parameter="ACTIVE_PROFILE", value=1
+        channel_address="VCU1769958:1",
+        paramset_key="VALUES",
+        parameter="ACTIVE_PROFILE",
+        value=1,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert climate.preset_mode == PresetMode.WEEK_PROGRAM_1
 
     with freeze_time("2023-03-03 08:00:00"):
         await climate.enable_away_mode_by_duration(hours=100, away_temperature=17.0)
     assert mock_client.method_calls[-3] == call.put_paramset(
         channel_address="VCU1769958:1",
```

### Comparing `hahomematic-2024.4.9b2/tests/test_cover.py` & `hahomematic-2024.5.0/tests/test_cover.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 """Tests for cover entities of hahomematic."""
 
 from __future__ import annotations
 
 from typing import cast
-from unittest.mock import call
+from unittest.mock import Mock, call
 
 import pytest
 
+from hahomematic.central import CentralUnit
+from hahomematic.client import Client
+from hahomematic.config import WAIT_FOR_CALLBACK
 from hahomematic.const import EntityUsage
 from hahomematic.platforms.custom.cover import (
     _CLOSED_LEVEL,
     _OPEN_LEVEL,
+    _OPEN_TILT_LEVEL,
     _WD_CLOSED_LEVEL,
     CeBlind,
     CeCover,
     CeGarage,
     CeIpBlind,
     CeWindowDrive,
     GarageDoorActivity,
@@ -34,46 +38,64 @@
     "VCU8537918": "HmIP-BROLL.json",
 }
 
 # pylint: disable=protected-access
 
 
 @pytest.mark.asyncio()
-async def test_cecover(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_cecover(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test CeCover."""
-    central, mock_client = await factory.get_default_central(TEST_DEVICES)
+    central, mock_client, _ = central_client_factory
     cover: CeCover = cast(CeCover, helper.get_prepared_custom_entity(central, "VCU8537918", 4))
     assert cover.usage == EntityUsage.CE_PRIMARY
 
     assert cover.current_position == 0
     assert cover._channel_level == _CLOSED_LEVEL
     assert cover.is_closed is True
     await cover.set_position(position=81)
     assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU8537918:4",
         paramset_key="VALUES",
         parameter="LEVEL",
         value=0.81,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert cover.current_position == 81
     assert cover.is_closed is False
     await cover.open()
     assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU8537918:4",
         paramset_key="VALUES",
         parameter="LEVEL",
-        value=1.0,
+        value=_OPEN_LEVEL,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert cover.current_position == 100
     await cover.close()
     assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU8537918:4",
         paramset_key="VALUES",
         parameter="LEVEL",
         value=_CLOSED_LEVEL,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert cover.current_position == 0
 
     assert cover.is_opening is None
     assert cover.is_closing is None
     await central.event(const.INTERFACE_ID, "VCU8537918:3", "ACTIVITY_STATE", 1)
     assert cover.is_opening is True
@@ -81,66 +103,102 @@
     assert cover.is_closing is True
     await central.event(const.INTERFACE_ID, "VCU8537918:3", "ACTIVITY_STATE", 0)
 
     await central.event(const.INTERFACE_ID, "VCU8537918:3", "LEVEL", 0.5)
     assert cover._channel_level == 0.5
     assert cover.current_position == 50
 
-    await central.event(const.INTERFACE_ID, "VCU8537918:3", "LEVEL", 0.0)
+    await central.event(const.INTERFACE_ID, "VCU8537918:3", "LEVEL", _CLOSED_LEVEL)
     call_count = len(mock_client.method_calls)
     await cover.close()
     assert call_count == len(mock_client.method_calls)
 
-    await central.event(const.INTERFACE_ID, "VCU8537918:3", "LEVEL", 1.0)
+    await central.event(const.INTERFACE_ID, "VCU8537918:3", "LEVEL", _OPEN_LEVEL)
     call_count = len(mock_client.method_calls)
     await cover.open()
     assert call_count == len(mock_client.method_calls)
 
     await central.event(const.INTERFACE_ID, "VCU8537918:3", "LEVEL", 0.4)
     call_count = len(mock_client.method_calls)
     await cover.set_position(position=40)
     assert call_count == len(mock_client.method_calls)
 
 
 @pytest.mark.asyncio()
-async def test_ceipblind_dr(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_ceipblind_dr(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test CeIpBlind DIN Rail."""
-    central, mock_client = await factory.get_default_central(TEST_DEVICES)
+    central, mock_client, _ = central_client_factory
     cover: CeIpBlind = cast(CeIpBlind, helper.get_prepared_custom_entity(central, "VCU7807849", 2))
     assert cover.usage == EntityUsage.CE_PRIMARY
 
     assert cover.current_position == 0
     assert cover._channel_level == _CLOSED_LEVEL
     assert cover.channel_operation_mode == "SHUTTER"
     assert cover.is_closed is True
     await cover.set_position(position=81)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU7807849:2",
         paramset_key="VALUES",
         parameter="COMBINED_PARAMETER",
         value="L2=0,L=81",
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
+
+    # test unconfirmed values
+    assert cover._e_level.unconfirmed_last_value_send == 0.81
+    assert cover._e_level_2.unconfirmed_last_value_send == _CLOSED_LEVEL
+    await central.event(const.INTERFACE_ID, "VCU7807849:2", "LEVEL", 0.81)
+    await central.event(const.INTERFACE_ID, "VCU7807849:2", "LEVEL_2", _CLOSED_LEVEL)
+    assert cover._e_level.unconfirmed_last_value_send is None
+    assert cover._e_level_2.unconfirmed_last_value_send is None
+
     await central.event(const.INTERFACE_ID, "VCU7807849:1", "LEVEL", 0.81)
+    await central.event(const.INTERFACE_ID, "VCU7807849:1", "LEVEL_2", _CLOSED_LEVEL)
     assert cover.current_position == 81
     assert cover.is_closed is False
     await cover.open()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU7807849:2",
         paramset_key="VALUES",
         parameter="COMBINED_PARAMETER",
-        value="L2=100,L=100",
+        value="L2=50,L=100",
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
+    assert cover._e_level.unconfirmed_last_value_send == _OPEN_LEVEL
+    assert cover._e_level_2.unconfirmed_last_value_send == _OPEN_TILT_LEVEL
     await central.event(const.INTERFACE_ID, "VCU7807849:1", "LEVEL", _OPEN_LEVEL)
+    await central.event(const.INTERFACE_ID, "VCU7807849:1", "LEVEL_2", _OPEN_TILT_LEVEL)
+    await central.event(const.INTERFACE_ID, "VCU7807849:2", "LEVEL", _OPEN_LEVEL)
+    await central.event(const.INTERFACE_ID, "VCU7807849:2", "LEVEL_2", _OPEN_TILT_LEVEL)
+    assert cover._e_level.unconfirmed_last_value_send is None
+    assert cover._e_level_2.unconfirmed_last_value_send is None
     assert cover.current_position == 100
+    assert cover.current_tilt_position == 50
     await cover.close()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU7807849:2",
         paramset_key="VALUES",
         parameter="COMBINED_PARAMETER",
         value="L2=0,L=0",
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU7807849:1", "LEVEL", _CLOSED_LEVEL)
     assert cover.is_opening is None
     assert cover.is_closing is None
     await central.event(const.INTERFACE_ID, "VCU7807849:1", "ACTIVITY_STATE", 1)
     assert cover.is_opening is True
     await central.event(const.INTERFACE_ID, "VCU7807849:1", "ACTIVITY_STATE", 2)
@@ -148,173 +206,217 @@
 
     await central.event(const.INTERFACE_ID, "VCU7807849:1", "LEVEL", 0.5)
     assert cover._channel_level == 0.5
     assert cover.current_position == 50
 
 
 @pytest.mark.asyncio()
-async def test_cewindowdrive(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_cewindowdrive(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test CeWindowDrive."""
-    central, mock_client = await factory.get_default_central(TEST_DEVICES)
+    central, mock_client, _ = central_client_factory
     cover: CeWindowDrive = cast(
         CeWindowDrive, helper.get_prepared_custom_entity(central, "VCU0000350", 1)
     )
     assert cover.usage == EntityUsage.CE_PRIMARY
 
     assert cover.current_position == 0
     assert cover._channel_level == _WD_CLOSED_LEVEL
     assert cover.is_closed is True
     await cover.set_position(position=81)
     assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU0000350:1",
         paramset_key="VALUES",
         parameter="LEVEL",
         value=0.81,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert cover.current_position == 81
     assert cover.is_closed is False
 
     await cover.open()
     assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU0000350:1",
         paramset_key="VALUES",
         parameter="LEVEL",
         value=_OPEN_LEVEL,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert cover.current_position == 100
     await cover.close()
     assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU0000350:1",
         paramset_key="VALUES",
         parameter="LEVEL",
         value=_WD_CLOSED_LEVEL,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert cover.current_position == 0
     assert cover._channel_level == _WD_CLOSED_LEVEL
     assert cover.is_closed is True
 
     await cover.set_position(position=1)
     assert cover.current_position == 1
     assert cover._channel_level == _CLOSED_LEVEL
     assert cover.is_closed is False
 
-    await cover.set_position(position=0.0)
+    await cover.set_position(position=_WD_CLOSED_LEVEL)
     assert cover.current_position == 0
     assert cover._channel_level == _WD_CLOSED_LEVEL
     assert cover.is_closed is True
 
 
 @pytest.mark.asyncio()
-async def test_ceblind(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_ceblind(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test CeBlind."""
-    central, mock_client = await factory.get_default_central(TEST_DEVICES)
+    central, mock_client, _ = central_client_factory
     cover: CeBlind = cast(CeBlind, helper.get_prepared_custom_entity(central, "VCU0000145", 1))
     assert cover.usage == EntityUsage.CE_PRIMARY
     assert cover.current_position == 0
     assert cover.current_tilt_position == 0
 
     await cover.set_position(position=81)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU0000145:1",
         paramset_key="VALUES",
         parameter="LEVEL_COMBINED",
         value="0xa2,0x00",
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL", 0.81)
     assert cover.current_position == 81
     assert cover.current_tilt_position == 0
 
     await cover.open()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU0000145:1",
         paramset_key="VALUES",
         parameter="LEVEL_COMBINED",
-        value="0xc8,0x00",
+        value="0xc8,0x64",
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL", _OPEN_LEVEL)
+    await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _OPEN_TILT_LEVEL)
     assert cover.current_position == 100
-    assert cover.current_tilt_position == 0
+    assert cover.current_tilt_position == 50
 
     await cover.close()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU0000145:1",
         paramset_key="VALUES",
         parameter="LEVEL_COMBINED",
         value="0x00,0x00",
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL", _CLOSED_LEVEL)
+    await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _CLOSED_LEVEL)
     assert cover.current_position == 0
     assert cover.current_tilt_position == 0
 
     await cover.open_tilt()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU0000145:1",
         paramset_key="VALUES",
         parameter="LEVEL_COMBINED",
-        value="0x00,0xc8",
+        value="0x00,0x64",
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
-    await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _OPEN_LEVEL)
+    await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _OPEN_TILT_LEVEL)
     assert cover.current_position == 0
-    assert cover.current_tilt_position == 100
+    assert cover.current_tilt_position == 50
 
     await cover.set_position(tilt_position=45)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU0000145:1",
         paramset_key="VALUES",
         parameter="LEVEL_COMBINED",
         value="0x00,0x5a",
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", 0.45)
     assert cover.current_position == 0
     assert cover.current_tilt_position == 45
 
     await cover.close_tilt()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU0000145:1",
         paramset_key="VALUES",
         parameter="LEVEL_COMBINED",
         value="0x00,0x00",
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _CLOSED_LEVEL)
     assert cover.current_position == 0
     assert cover.current_tilt_position == 0
 
     await cover.set_position(position=10, tilt_position=20)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU0000145:1",
         paramset_key="VALUES",
         parameter="LEVEL_COMBINED",
         value="0x14,0x28",
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL", 0.1)
     await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", 0.2)
     assert cover.current_position == 10
     assert cover.current_tilt_position == 20
 
     await cover.stop()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU0000145:1",
         paramset_key="VALUES",
         parameter="STOP",
         value=True,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await cover.stop_tilt()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU0000145:1",
         paramset_key="VALUES",
         parameter="STOP",
         value=True,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
 
     await cover.open_tilt()
-    await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _OPEN_LEVEL)
+    await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _OPEN_TILT_LEVEL)
     call_count = len(mock_client.method_calls)
     await cover.open_tilt()
-    await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _OPEN_LEVEL)
-    assert call_count == len(mock_client.method_calls) - 1
+    await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _OPEN_TILT_LEVEL)
+    assert call_count == len(mock_client.method_calls) - 2
 
     await cover.close_tilt()
     await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _CLOSED_LEVEL)
     call_count = len(mock_client.method_calls)
     await cover.close_tilt()
     await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _CLOSED_LEVEL)
     assert call_count == len(mock_client.method_calls) - 1
@@ -322,97 +424,119 @@
     await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", 0.4)
     call_count = len(mock_client.method_calls)
     await cover.set_position(tilt_position=40)
     assert call_count == len(mock_client.method_calls)
 
 
 @pytest.mark.asyncio()
-async def test_ceipblind(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_ceipblind(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test CeIpBlind."""
-    central, mock_client = await factory.get_default_central(TEST_DEVICES)
+    central, mock_client, _ = central_client_factory
     cover: CeIpBlind = cast(CeIpBlind, helper.get_prepared_custom_entity(central, "VCU1223813", 4))
     assert cover.usage == EntityUsage.CE_PRIMARY
 
     assert cover.current_position == 0
     assert cover.current_tilt_position == 0
     await cover.set_position(position=81)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU1223813:4",
         paramset_key="VALUES",
         parameter="COMBINED_PARAMETER",
         value="L2=0,L=81",
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL", 0.81)
     assert cover.current_position == 81
     assert cover.current_tilt_position == 0
 
     await cover.open()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU1223813:4",
         paramset_key="VALUES",
         parameter="COMBINED_PARAMETER",
-        value="L2=100,L=100",
+        value="L2=50,L=100",
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
-    await central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL_2", 1.0)
-    await central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL", 1.0)
+    await central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL_2", _OPEN_TILT_LEVEL)
+    await central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL", _OPEN_LEVEL)
     assert cover.current_position == 100
-    assert cover.current_tilt_position == 100
+    assert cover.current_tilt_position == 50
 
     await cover.close()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU1223813:4",
         paramset_key="VALUES",
         parameter="COMBINED_PARAMETER",
         value="L2=0,L=0",
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
-    await central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL_2", 0.0)
-    await central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL", 0.0)
+    await central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL_2", _CLOSED_LEVEL)
+    await central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL", _CLOSED_LEVEL)
     assert cover.current_position == 0
     assert cover.current_tilt_position == 0
 
     await cover.open_tilt()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU1223813:4",
         paramset_key="VALUES",
         parameter="COMBINED_PARAMETER",
-        value="L2=100,L=0",
+        value="L2=50,L=0",
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL_2", 1.0)
     assert cover.current_position == 0
     assert cover.current_tilt_position == 100
 
     await cover.set_position(tilt_position=45)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU1223813:4",
         paramset_key="VALUES",
         parameter="COMBINED_PARAMETER",
         value="L2=45,L=0",
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL_2", 0.45)
     assert cover.current_position == 0
     assert cover.current_tilt_position == 45
 
     await cover.close_tilt()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU1223813:4",
         paramset_key="VALUES",
         parameter="COMBINED_PARAMETER",
         value="L2=0,L=0",
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
-    await central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL_2", 0.0)
-    await central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL", 0.0)
+    await central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL_2", _CLOSED_LEVEL)
+    await central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL", _CLOSED_LEVEL)
     assert cover.current_position == 0
     assert cover.current_tilt_position == 0
 
     await cover.set_position(position=10, tilt_position=20)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU1223813:4",
         paramset_key="VALUES",
         parameter="COMBINED_PARAMETER",
         value="L2=20,L=10",
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL", 0.1)
     await central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL_2", 0.2)
     assert cover.current_position == 10
     assert cover.current_tilt_position == 20
 
     await central.event(const.INTERFACE_ID, "VCU1223813:3", "LEVEL", 0.5)
@@ -439,95 +563,121 @@
 
     await central.event(const.INTERFACE_ID, "VCU1223813:3", "ACTIVITY_STATE", 3)
     assert cover.is_opening is False
     assert cover.is_closing is False
 
     await cover.stop()
     assert mock_client.method_calls[-1] == call.set_value(
-        channel_address="VCU1223813:4", paramset_key="VALUES", parameter="STOP", value=True
+        channel_address="VCU1223813:4",
+        paramset_key="VALUES",
+        parameter="STOP",
+        value=True,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
 
 
 @pytest.mark.asyncio()
-async def test_ceipblind_hdm(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_ceipblind_hdm(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test CeIpBlind HDM."""
-    central, mock_client = await factory.get_default_central(TEST_DEVICES)
+    central, mock_client, _ = central_client_factory
     cover: CeIpBlind = cast(CeIpBlind, helper.get_prepared_custom_entity(central, "VCU3560967", 1))
     assert cover.usage == EntityUsage.CE_PRIMARY
 
     assert cover.current_position == 0
     assert cover.current_tilt_position == 0
     await cover.set_position(position=81)
     assert mock_client.method_calls[-3] == call.put_paramset(
         channel_address="VCU3560967:1",
         paramset_key="VALUES",
-        values={"LEVEL_2": 0.0, "LEVEL": 0.81},
+        values={"LEVEL_2": _CLOSED_LEVEL, "LEVEL": 0.81},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL", 0.81)
     assert cover.current_position == 81
     assert cover.current_tilt_position == 0
 
     await cover.open()
     assert mock_client.method_calls[-3] == call.put_paramset(
         channel_address="VCU3560967:1",
         paramset_key="VALUES",
-        values={"LEVEL_2": 1.0, "LEVEL": 1.0},
+        values={"LEVEL_2": 0.5, "LEVEL": _OPEN_LEVEL},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
-    await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL_2", 1.0)
-    await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL", 1.0)
+    await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL_2", _OPEN_TILT_LEVEL)
+    await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL", _OPEN_LEVEL)
     assert cover.current_position == 100
-    assert cover.current_tilt_position == 100
+    assert cover.current_tilt_position == 50
 
     await cover.close()
     assert mock_client.method_calls[-3] == call.put_paramset(
         channel_address="VCU3560967:1",
         paramset_key="VALUES",
-        values={"LEVEL_2": 0.0, "LEVEL": 0.0},
+        values={"LEVEL_2": _CLOSED_LEVEL, "LEVEL": _CLOSED_LEVEL},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
-    await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL_2", 0.0)
-    await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL", 0.0)
+    await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL_2", _CLOSED_LEVEL)
+    await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL", _CLOSED_LEVEL)
     assert cover.current_position == 0
     assert cover.current_tilt_position == 0
 
     await cover.open_tilt()
     assert mock_client.method_calls[-3] == call.put_paramset(
         channel_address="VCU3560967:1",
         paramset_key="VALUES",
-        values={"LEVEL_2": 1.0, "LEVEL": 0.0},
+        values={"LEVEL_2": _OPEN_TILT_LEVEL, "LEVEL": _CLOSED_LEVEL},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL_2", 1.0)
     assert cover.current_position == 0
     assert cover.current_tilt_position == 100
 
     await cover.set_position(tilt_position=45)
     assert mock_client.method_calls[-3] == call.put_paramset(
         channel_address="VCU3560967:1",
         paramset_key="VALUES",
-        values={"LEVEL_2": 0.45, "LEVEL": 0.0},
+        values={"LEVEL_2": 0.45, "LEVEL": _CLOSED_LEVEL},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL_2", 0.45)
     assert cover.current_position == 0
     assert cover.current_tilt_position == 45
 
     await cover.close_tilt()
     assert mock_client.method_calls[-3] == call.put_paramset(
         channel_address="VCU3560967:1",
         paramset_key="VALUES",
-        values={"LEVEL_2": 0.0, "LEVEL": 0.0},
+        values={"LEVEL_2": _CLOSED_LEVEL, "LEVEL": _CLOSED_LEVEL},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
-    await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL_2", 0.0)
-    await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL", 0.0)
+    await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL_2", _CLOSED_LEVEL)
+    await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL", _CLOSED_LEVEL)
     assert cover.current_position == 0
     assert cover.current_tilt_position == 0
 
     await cover.set_position(position=10, tilt_position=20)
     assert mock_client.method_calls[-3] == call.put_paramset(
         channel_address="VCU3560967:1",
         paramset_key="VALUES",
         values={"LEVEL_2": 0.2, "LEVEL": 0.1},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL", 0.1)
     await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL_2", 0.2)
     assert cover.current_position == 10
     assert cover.current_tilt_position == 20
 
     await central.event(const.INTERFACE_ID, "VCU3560967:1", "ACTIVITY_STATE", 1)
@@ -538,78 +688,103 @@
 
     await central.event(const.INTERFACE_ID, "VCU3560967:1", "ACTIVITY_STATE", 3)
     assert cover.is_opening is False
     assert cover.is_closing is False
 
     await cover.stop()
     assert mock_client.method_calls[-1] == call.set_value(
-        channel_address="VCU3560967:1", paramset_key="VALUES", parameter="STOP", value=True
+        channel_address="VCU3560967:1",
+        paramset_key="VALUES",
+        parameter="STOP",
+        value=True,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
 
 
 @pytest.mark.asyncio()
-async def test_cegarageho(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_cegarageho(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test CeGarageHO."""
-    central, mock_client = await factory.get_default_central(TEST_DEVICES)
+    central, mock_client, _ = central_client_factory
     cover: CeGarage = cast(CeGarage, helper.get_prepared_custom_entity(central, "VCU3574044", 1))
     assert cover.usage == EntityUsage.CE_PRIMARY
 
     assert cover.current_position is None
     await cover.set_position(position=81)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU3574044:1",
         paramset_key="VALUES",
         parameter="DOOR_COMMAND",
         value=1,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU3574044:1", "DOOR_STATE", 1)
     assert cover.current_position == 100
     await cover.close()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU3574044:1",
         paramset_key="VALUES",
         parameter="DOOR_COMMAND",
         value=3,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU3574044:1", "DOOR_STATE", 0)
     assert cover.current_position == 0
     assert cover.is_closed is True
     await cover.set_position(position=11)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU3574044:1",
         paramset_key="VALUES",
         parameter="DOOR_COMMAND",
         value=4,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU3574044:1", "DOOR_STATE", 2)
     assert cover.current_position == 10
 
     await cover.set_position(position=5)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU3574044:1",
         paramset_key="VALUES",
         parameter="DOOR_COMMAND",
         value=3,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU3574044:1", "DOOR_STATE", 0)
     assert cover.current_position == 0
 
     await cover.open()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU3574044:1",
         paramset_key="VALUES",
         parameter="DOOR_COMMAND",
         value=1,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await cover.stop()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU3574044:1",
         paramset_key="VALUES",
         parameter="DOOR_COMMAND",
         value=2,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
 
     await central.event(const.INTERFACE_ID, "VCU3574044:1", "DOOR_STATE", 1)
     assert cover.current_position == 100
 
     await central.event(
         const.INTERFACE_ID, "VCU3574044:1", "SECTION", GarageDoorActivity.OPENING.value
@@ -640,73 +815,94 @@
     await central.event(const.INTERFACE_ID, "VCU3574044:1", "DOOR_STATE", 2)
     call_count = len(mock_client.method_calls)
     await cover.vent()
     assert call_count == len(mock_client.method_calls)
 
 
 @pytest.mark.asyncio()
-async def test_cegaragetm(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_cegaragetm(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test CeGarageTM."""
-    central, mock_client = await factory.get_default_central(TEST_DEVICES)
+    central, mock_client, _ = central_client_factory
     cover: CeGarage = cast(CeGarage, helper.get_prepared_custom_entity(central, "VCU6166407", 1))
     assert cover.usage == EntityUsage.CE_PRIMARY
 
     assert cover.current_position is None
     await cover.set_position(position=81)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU6166407:1",
         paramset_key="VALUES",
         parameter="DOOR_COMMAND",
         value=1,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU6166407:1", "DOOR_STATE", 1)
     assert cover.current_position == 100
     await cover.close()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU6166407:1",
         paramset_key="VALUES",
         parameter="DOOR_COMMAND",
         value=3,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU6166407:1", "DOOR_STATE", 0)
     assert cover.current_position == 0
     assert cover.is_closed is True
     await cover.set_position(position=11)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU6166407:1",
         paramset_key="VALUES",
         parameter="DOOR_COMMAND",
         value=4,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU6166407:1", "DOOR_STATE", 2)
     assert cover.current_position == 10
 
     await cover.set_position(position=5)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU6166407:1",
         paramset_key="VALUES",
         parameter="DOOR_COMMAND",
         value=3,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU6166407:1", "DOOR_STATE", 0)
     assert cover.current_position == 0
 
     await cover.open()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU6166407:1",
         paramset_key="VALUES",
         parameter="DOOR_COMMAND",
         value=1,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await cover.stop()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU6166407:1",
         paramset_key="VALUES",
         parameter="DOOR_COMMAND",
         value=2,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
 
     await central.event(const.INTERFACE_ID, "VCU6166407:1", "DOOR_STATE", 1)
     assert cover.current_position == 100
 
     await central.event(const.INTERFACE_ID, "VCU6166407:1", "SECTION", GarageDoorActivity.OPENING)
     assert cover.is_opening is True
```

### Comparing `hahomematic-2024.4.9b2/tests/test_decorator.py` & `hahomematic-2024.5.0/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b2/tests/test_device.py` & `hahomematic-2024.5.0/tests/test_device.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,48 @@
 """Tests for devices of hahomematic."""
 
 from __future__ import annotations
 
 import asyncio
+from unittest.mock import Mock
 
 import pytest
 
+from hahomematic.central import CentralUnit
+from hahomematic.client import Client
+
 from tests import const, helper
 
 TEST_DEVICES: dict[str, str] = {
     "VCU2128127": "HmIP-BSM.json",
     "VCU6354483": "HmIP-STHD.json",
 }
 
 # pylint: disable=protected-access
 
 
 @pytest.mark.asyncio()
-async def test_device_general(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_device_general(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test device availability."""
-    central, _ = await factory.get_default_central(TEST_DEVICES)
+    central, _, _ = central_client_factory
     device = central.get_device(address="VCU2128127")
     assert device.device_address == "VCU2128127"
     assert device.name == "HmIP-BSM_VCU2128127"
     assert (
         str(device) == "address: VCU2128127, "
         "type: 8, "
         "name: HmIP-BSM_VCU2128127, "
@@ -36,17 +55,32 @@
     assert device.interface_id == const.INTERFACE_ID
     assert device.has_custom_entity_definition is True
     assert len(device.custom_entities) == 3
     assert len(device.channels) == 11
 
 
 @pytest.mark.asyncio()
-async def test_device_availability(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_device_availability(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test device availability."""
-    central, _ = await factory.get_default_central(TEST_DEVICES)
+    central, _, _ = central_client_factory
     device = central.get_device(address="VCU6354483")
     assert device.available is True
     for generic_entity in device.generic_entities:
         assert generic_entity.available is True
     for custom_entity in device.custom_entities:
         assert custom_entity.available is True
 
@@ -62,17 +96,32 @@
     for generic_entity in device.generic_entities:
         assert generic_entity.available is True
     for custom_entity in device.custom_entities:
         assert custom_entity.available is True
 
 
 @pytest.mark.asyncio()
-async def test_device_config_pending(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_device_config_pending(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test device availability."""
-    central, _ = await factory.get_default_central(TEST_DEVICES)
+    central, _, _ = central_client_factory
     device = central.get_device(address="VCU2128127")
     assert device._e_config_pending.value is False
     last_save = central.paramset_descriptions.last_save
     await central.event(const.INTERFACE_ID, "VCU2128127:0", "CONFIG_PENDING", True)
     assert device._e_config_pending.value is True
     assert last_save == central.paramset_descriptions.last_save
     await central.event(const.INTERFACE_ID, "VCU2128127:0", "CONFIG_PENDING", False)
```

### Comparing `hahomematic-2024.4.9b2/tests/test_json_rpc.py` & `hahomematic-2024.5.0/tests/test_json_rpc.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b2/tests/test_light.py` & `hahomematic-2024.5.0/tests/test_light.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """Tests for light entities of hahomematic."""
 
 from __future__ import annotations
 
 from typing import cast
-from unittest.mock import call
+from unittest.mock import Mock, call
 
 import pytest
 
+from hahomematic.central import CentralUnit
+from hahomematic.client import Client
+from hahomematic.config import WAIT_FOR_CALLBACK
 from hahomematic.const import EntityUsage, ParamsetKey
 from hahomematic.platforms.custom.light import (
     CeColorDimmer,
     CeColorDimmerEffect,
     CeColorTempDimmer,
     CeDimmer,
     CeIpFixedColorLight,
@@ -33,17 +36,32 @@
     "VCU9973336": "HBW-LC-RGBWW-IN6-DR.json",
 }
 
 # pylint: disable=protected-access
 
 
 @pytest.mark.asyncio()
-async def test_cedimmer(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_cedimmer(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test CeDimmer."""
-    central, mock_client = await factory.get_default_central(TEST_DEVICES)
+    central, mock_client, _ = central_client_factory
     light: CeDimmer = cast(CeDimmer, helper.get_prepared_custom_entity(central, "VCU1399816", 4))
     assert light.usage == EntityUsage.CE_PRIMARY
     assert light.color_temp is None
     assert light.hs_color is None
     assert light.supports_brightness is True
     assert light.supports_color_temperature is False
     assert light.supports_effects is False
@@ -52,84 +70,112 @@
     assert light.effect is None
     assert light.effects is None
 
     assert light.brightness == 0
     assert light.brightness_pct == 0
     await light.turn_on()
     assert mock_client.method_calls[-2] == call.set_value(
-        channel_address="VCU1399816:4", paramset_key="VALUES", parameter="LEVEL", value=1.0
+        channel_address="VCU1399816:4",
+        paramset_key="VALUES",
+        parameter="LEVEL",
+        value=1.0,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.brightness == 255
     assert light.brightness_pct == 100
     await light.turn_on(brightness=28)
     assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU1399816:4",
         paramset_key="VALUES",
         parameter="LEVEL",
         value=0.10980392156862745,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.brightness == 28
     assert light.brightness_pct == 10
     assert light.is_on
 
     assert light.channel_brightness is None
     await central.event(const.INTERFACE_ID, "VCU1399816:3", "LEVEL", 0.4)
     assert light.channel_brightness == 102
 
     await light.turn_on(on_time=5.0, ramp_time=6.0)
     assert mock_client.method_calls[-2] == call.put_paramset(
         channel_address="VCU1399816:4",
         paramset_key="VALUES",
         values={"LEVEL": 0.10980392156862745, "RAMP_TIME": 6.0, "ON_TIME": 5.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await light.turn_on(on_time=5.0)
     assert mock_client.method_calls[-2] == call.put_paramset(
         channel_address="VCU1399816:4",
         paramset_key="VALUES",
         values={"ON_TIME": 5.0, "LEVEL": 0.10980392156862745},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
 
     await light.turn_off(ramp_time=6.0)
     assert mock_client.method_calls[-2] == call.put_paramset(
         channel_address="VCU1399816:4",
         paramset_key="VALUES",
         values={"RAMP_TIME": 6.0, "LEVEL": 0.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.brightness == 0
     await light.turn_on()
     assert light.brightness == 255
     await light.turn_off()
     assert mock_client.method_calls[-2] == call.set_value(
-        channel_address="VCU1399816:4", paramset_key="VALUES", parameter="LEVEL", value=0.0
+        channel_address="VCU1399816:4",
+        paramset_key="VALUES",
+        parameter="LEVEL",
+        value=0.0,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
 
     await light.turn_off()
     light.set_on_time(0.5)
     await light.turn_on()
     assert mock_client.method_calls[-2] == call.put_paramset(
         channel_address="VCU1399816:4",
         paramset_key="VALUES",
         values={"ON_TIME": 0.5, "LEVEL": 1.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
 
     await light.turn_on()
     call_count = len(mock_client.method_calls)
     await light.turn_on()
     assert call_count == len(mock_client.method_calls)
 
     await light.turn_off()
     call_count = len(mock_client.method_calls)
     await light.turn_off()
     assert call_count == len(mock_client.method_calls)
 
 
 @pytest.mark.asyncio()
-async def test_cecolordimmereffect(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_cecolordimmereffect(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test CeColorDimmerEffect."""
-    central, mock_client = await factory.get_default_central(TEST_DEVICES)
+    central, mock_client, _ = central_client_factory
     light: CeColorDimmerEffect = cast(
         CeColorDimmerEffect, helper.get_prepared_custom_entity(central, "VCU3747418", 1)
     )
     assert light.usage == EntityUsage.CE_PRIMARY
     assert light.color_temp is None
     assert light.hs_color == (0.0, 0.0)
     assert light.supports_brightness is True
@@ -147,57 +193,90 @@
         "Waterfall",
         "TV simulation",
     )
 
     assert light.brightness == 0
     await light.turn_on()
     assert mock_client.method_calls[-2] == call.set_value(
-        channel_address="VCU3747418:1", paramset_key="VALUES", parameter="LEVEL", value=1.0
+        channel_address="VCU3747418:1",
+        paramset_key="VALUES",
+        parameter="LEVEL",
+        value=1.0,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.brightness == 255
     await light.turn_on(brightness=28)
     assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU3747418:1",
         paramset_key="VALUES",
         parameter="LEVEL",
         value=0.10980392156862745,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.brightness == 28
     await light.turn_off()
     assert mock_client.method_calls[-2] == call.set_value(
-        channel_address="VCU3747418:1", paramset_key="VALUES", parameter="LEVEL", value=0.0
+        channel_address="VCU3747418:1",
+        paramset_key="VALUES",
+        parameter="LEVEL",
+        value=0.0,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.brightness == 0
 
     assert light.hs_color == (0.0, 0.0)
     await light.turn_on(hs_color=(44.4, 69.3))
     assert mock_client.method_calls[-4] == call.set_value(
-        channel_address="VCU3747418:2", paramset_key="VALUES", parameter="COLOR", value=25
+        channel_address="VCU3747418:2",
+        paramset_key="VALUES",
+        parameter="COLOR",
+        value=25,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert mock_client.method_calls[-2] == call.set_value(
-        channel_address="VCU3747418:1", paramset_key="VALUES", parameter="LEVEL", value=1.0
+        channel_address="VCU3747418:1",
+        paramset_key="VALUES",
+        parameter="LEVEL",
+        value=1.0,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.hs_color == (45.0, 100)
 
     await light.turn_on(hs_color=(0, 50))
     assert mock_client.method_calls[-4] == call.set_value(
-        channel_address="VCU3747418:2", paramset_key="VALUES", parameter="COLOR", value=0
+        channel_address="VCU3747418:2",
+        paramset_key="VALUES",
+        parameter="COLOR",
+        value=0,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert mock_client.method_calls[-2] == call.set_value(
-        channel_address="VCU3747418:1", paramset_key="VALUES", parameter="LEVEL", value=1.0
+        channel_address="VCU3747418:1",
+        paramset_key="VALUES",
+        parameter="LEVEL",
+        value=1.0,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.hs_color == (0.0, 100.0)
 
     await light.turn_on(effect="Slow color change")
 
     assert mock_client.method_calls[-4] == call.set_value(
-        channel_address="VCU3747418:1", paramset_key="VALUES", parameter="LEVEL", value=1.0
+        channel_address="VCU3747418:1",
+        paramset_key="VALUES",
+        parameter="LEVEL",
+        value=1.0,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert mock_client.method_calls[-2] == call.set_value(
-        channel_address="VCU3747418:3", paramset_key="VALUES", parameter="PROGRAM", value=1
+        channel_address="VCU3747418:3",
+        paramset_key="VALUES",
+        parameter="PROGRAM",
+        value=1,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
 
     assert light.effect == "Slow color change"
 
     await central.event(const.INTERFACE_ID, "VCU3747418:2", "COLOR", 201)
     assert light.hs_color == (0.0, 0.0)
     await central.event(const.INTERFACE_ID, "VCU3747418:2", "COLOR", None)
@@ -215,24 +294,44 @@
 
     await light.turn_on(brightness=28, effect="Slow color change")
     assert mock_client.method_calls[-4] == call.set_value(
         channel_address="VCU3747418:1",
         paramset_key="VALUES",
         parameter="LEVEL",
         value=0.10980392156862745,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert mock_client.method_calls[-2] == call.set_value(
-        channel_address="VCU3747418:3", paramset_key="VALUES", parameter="PROGRAM", value=1
+        channel_address="VCU3747418:3",
+        paramset_key="VALUES",
+        parameter="PROGRAM",
+        value=1,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
 
 
 @pytest.mark.asyncio()
-async def test_cecolortempdimmer(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_cecolortempdimmer(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test CeColorTempDimmer."""
-    central, mock_client = await factory.get_default_central(TEST_DEVICES)
+    central, mock_client, _ = central_client_factory
     light: CeColorTempDimmer = cast(
         CeColorTempDimmer, helper.get_prepared_custom_entity(central, "VCU0000115", 1)
     )
     assert light.usage == EntityUsage.CE_PRIMARY
     assert light.color_temp == 500
     assert light.hs_color is None
     assert light.supports_brightness is True
@@ -241,41 +340,55 @@
     assert light.supports_hs_color is False
     assert light.supports_transition is True
     assert light.effect is None
     assert light.effects is None
     assert light.brightness == 0
     await light.turn_on()
     assert mock_client.method_calls[-2] == call.set_value(
-        channel_address="VCU0000115:1", paramset_key="VALUES", parameter="LEVEL", value=1.0
+        channel_address="VCU0000115:1",
+        paramset_key="VALUES",
+        parameter="LEVEL",
+        value=1.0,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.brightness == 255
     await light.turn_on(brightness=28)
     assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU0000115:1",
         paramset_key="VALUES",
         parameter="LEVEL",
         value=0.10980392156862745,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.brightness == 28
     await light.turn_off()
     assert mock_client.method_calls[-2] == call.set_value(
-        channel_address="VCU0000115:1", paramset_key="VALUES", parameter="LEVEL", value=0.0
+        channel_address="VCU0000115:1",
+        paramset_key="VALUES",
+        parameter="LEVEL",
+        value=0.0,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.brightness == 0
 
     assert light.color_temp == 500
     await light.turn_on(color_temp=433)
     assert mock_client.method_calls[-4] == call.set_value(
         channel_address="VCU0000115:2",
         paramset_key="VALUES",
         parameter="LEVEL",
         value=0.1930835734870317,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert mock_client.method_calls[-2] == call.set_value(
-        channel_address="VCU0000115:1", paramset_key="VALUES", parameter="LEVEL", value=1.0
+        channel_address="VCU0000115:1",
+        paramset_key="VALUES",
+        parameter="LEVEL",
+        value=1.0,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.color_temp == 433
 
     await light.turn_on()
     call_count = len(mock_client.method_calls)
     await light.turn_on()
     assert call_count == len(mock_client.method_calls)
@@ -283,95 +396,139 @@
     await light.turn_off()
     call_count = len(mock_client.method_calls)
     await light.turn_off()
     assert call_count == len(mock_client.method_calls)
 
 
 @pytest.mark.asyncio()
-async def test_ceipfixedcolorlight(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_ceipfixedcolorlight(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test CeIpFixedColorLight."""
-    central, mock_client = await factory.get_default_central(TEST_DEVICES)
+    central, mock_client, _ = central_client_factory
     light: CeIpFixedColorLight = cast(
         CeIpFixedColorLight, helper.get_prepared_custom_entity(central, "VCU3716619", 8)
     )
     assert light.usage == EntityUsage.CE_PRIMARY
     assert light.color_temp is None
     assert light.hs_color == (0.0, 0.0)
     assert light.supports_brightness is True
     assert light.supports_color_temperature is False
     assert light.supports_effects is False
     assert light.supports_hs_color is True
     assert light.supports_transition is True
     assert light.effect is None
-    assert light.effects is None
+    assert light.effects == ()
     assert light.brightness == 0
     assert light.is_on is False
     assert light.color_name == FixedColor.BLACK
     assert light.channel_color_name is None
     assert light.channel_brightness is None
     assert light.channel_hs_color is None
     await light.turn_on()
     assert mock_client.method_calls[-3] == call.put_paramset(
-        channel_address="VCU3716619:8", paramset_key="VALUES", values={"COLOR": 7, "LEVEL": 1.0}
+        channel_address="VCU3716619:8",
+        paramset_key="VALUES",
+        values={"COLOR": 7, "LEVEL": 1.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.brightness == 255
     await light.turn_on(brightness=28)
     assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU3716619:8",
         paramset_key="VALUES",
         parameter="LEVEL",
         value=0.10980392156862745,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.brightness == 28
     await light.turn_off()
     assert mock_client.method_calls[-2] == call.set_value(
-        channel_address="VCU3716619:8", paramset_key="VALUES", parameter="LEVEL", value=0.0
+        channel_address="VCU3716619:8",
+        paramset_key="VALUES",
+        parameter="LEVEL",
+        value=0.0,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.brightness == 0
     assert light.color_name == FixedColor.WHITE
 
     await light.turn_on(hs_color=(350, 50))
     assert mock_client.method_calls[-3] == call.put_paramset(
-        channel_address="VCU3716619:8", paramset_key="VALUES", values={"COLOR": 4, "LEVEL": 1.0}
+        channel_address="VCU3716619:8",
+        paramset_key="VALUES",
+        values={"COLOR": 4, "LEVEL": 1.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.color_name == FixedColor.RED
 
     await light.turn_on(hs_color=(0.0, 0.0))
     assert mock_client.method_calls[-3] == call.put_paramset(
-        channel_address="VCU3716619:8", paramset_key="VALUES", values={"COLOR": 7, "LEVEL": 1.0}
+        channel_address="VCU3716619:8",
+        paramset_key="VALUES",
+        values={"COLOR": 7, "LEVEL": 1.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.color_name == FixedColor.WHITE
 
     await light.turn_on(hs_color=(60.0, 50.0))
     assert mock_client.method_calls[-3] == call.put_paramset(
-        channel_address="VCU3716619:8", paramset_key="VALUES", values={"COLOR": 6, "LEVEL": 1.0}
+        channel_address="VCU3716619:8",
+        paramset_key="VALUES",
+        values={"COLOR": 6, "LEVEL": 1.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.color_name == FixedColor.YELLOW
 
     await light.turn_on(hs_color=(120, 50))
     assert mock_client.method_calls[-3] == call.put_paramset(
-        channel_address="VCU3716619:8", paramset_key="VALUES", values={"COLOR": 2, "LEVEL": 1.0}
+        channel_address="VCU3716619:8",
+        paramset_key="VALUES",
+        values={"COLOR": 2, "LEVEL": 1.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.color_name == FixedColor.GREEN
 
     await light.turn_on(hs_color=(180, 50))
     assert mock_client.method_calls[-3] == call.put_paramset(
-        channel_address="VCU3716619:8", paramset_key="VALUES", values={"COLOR": 3, "LEVEL": 1.0}
+        channel_address="VCU3716619:8",
+        paramset_key="VALUES",
+        values={"COLOR": 3, "LEVEL": 1.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.color_name == FixedColor.TURQUOISE
 
     await light.turn_on(hs_color=(240, 50))
     assert mock_client.method_calls[-3] == call.put_paramset(
-        channel_address="VCU3716619:8", paramset_key="VALUES", values={"COLOR": 1, "LEVEL": 1.0}
+        channel_address="VCU3716619:8",
+        paramset_key="VALUES",
+        values={"COLOR": 1, "LEVEL": 1.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.color_name == FixedColor.BLUE
 
     await light.turn_on(hs_color=(300, 50))
     assert mock_client.method_calls[-3] == call.put_paramset(
-        channel_address="VCU3716619:8", paramset_key="VALUES", values={"COLOR": 5, "LEVEL": 1.0}
+        channel_address="VCU3716619:8",
+        paramset_key="VALUES",
+        values={"COLOR": 5, "LEVEL": 1.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.color_name == FixedColor.PURPLE
 
     await central.event(const.INTERFACE_ID, "VCU3716619:7", "LEVEL", 0.5)
     assert light.channel_brightness == 127
 
     await central.event(const.INTERFACE_ID, "VCU3716619:7", "COLOR", 1)
@@ -381,69 +538,90 @@
     await light.turn_off()
     light.set_on_time(18)
     await light.turn_on()
     assert mock_client.method_calls[-2] == call.put_paramset(
         channel_address="VCU3716619:8",
         paramset_key="VALUES",
         values={"DURATION_VALUE": 18, "LEVEL": 1.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
 
     await light.turn_off()
     light.set_on_time(17000)
     await light.turn_on()
     assert mock_client.method_calls[-2] == call.put_paramset(
         channel_address="VCU3716619:8",
         paramset_key="VALUES",
         values={"DURATION_UNIT": 1, "DURATION_VALUE": 283, "LEVEL": 1.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
 
     await light.turn_off()
     light.set_on_time(1000000)
     await light.turn_on()
     assert mock_client.method_calls[-2] == call.put_paramset(
         channel_address="VCU3716619:8",
         paramset_key="VALUES",
         values={"DURATION_UNIT": 2, "DURATION_VALUE": 277, "LEVEL": 1.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await light.turn_on(ramp_time=18)
     assert mock_client.method_calls[-2] == call.put_paramset(
         channel_address="VCU3716619:8",
         paramset_key="VALUES",
         values={"RAMP_TIME_VALUE": 18, "LEVEL": 1.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
 
     await light.turn_on(ramp_time=17000)
     assert mock_client.method_calls[-2] == call.put_paramset(
         channel_address="VCU3716619:8",
         paramset_key="VALUES",
         values={"RAMP_TIME_UNIT": 1, "RAMP_TIME_VALUE": 283, "LEVEL": 1.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
 
     await light.turn_on(ramp_time=1000000)
     assert mock_client.method_calls[-2] == call.put_paramset(
         channel_address="VCU3716619:8",
         paramset_key="VALUES",
         values={"RAMP_TIME_UNIT": 2, "RAMP_TIME_VALUE": 277, "LEVEL": 1.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
 
     await light.turn_on()
     call_count = len(mock_client.method_calls)
     await light.turn_on()
     assert call_count == len(mock_client.method_calls)
 
     await light.turn_off()
     call_count = len(mock_client.method_calls)
     await light.turn_off()
     assert call_count == len(mock_client.method_calls)
 
 
 @pytest.mark.asyncio()
-async def test_ceipfixedcolorlightwired(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_ceipfixedcolorlightwired(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test CeIpFixedColorLight."""
-    central, mock_client = await factory.get_default_central(TEST_DEVICES)
+    central, mock_client, _ = central_client_factory
     light: CeIpFixedColorLight = cast(
         CeIpFixedColorLight, helper.get_prepared_custom_entity(central, "VCU4704397", 8)
     )
     assert light.usage == EntityUsage.CE_PRIMARY
     assert light.color_temp is None
     assert light.hs_color == (0.0, 0.0)
     assert light.supports_brightness is True
@@ -468,101 +646,114 @@
     assert light.is_on is False
     assert light.color_name == FixedColor.BLACK
     await light.turn_on()
     assert mock_client.method_calls[-4] == call.put_paramset(
         channel_address="VCU4704397:8",
         paramset_key="VALUES",
         values={"COLOR_BEHAVIOUR": 1, "COLOR": 7, "LEVEL": 1.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.brightness == 255
     assert light.color_name == FixedColor.WHITE
 
     await light.turn_on(brightness=100)
     assert mock_client.method_calls[-3] == call.put_paramset(
         channel_address="VCU4704397:8",
         paramset_key="VALUES",
         values={"COLOR_BEHAVIOUR": 1, "LEVEL": 0.39215686274509803},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.brightness == 100
     assert light.color_name == FixedColor.WHITE
     assert light.effect == ColorBehaviour.ON
 
     await light.turn_off()
     assert mock_client.method_calls[-2] == call.set_value(
-        channel_address="VCU4704397:8", paramset_key="VALUES", parameter="LEVEL", value=0.0
+        channel_address="VCU4704397:8",
+        paramset_key="VALUES",
+        parameter="LEVEL",
+        value=0.0,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.brightness == 0
     assert light.color_name == FixedColor.WHITE
     assert light.effect == ColorBehaviour.ON
 
     await light.turn_on(hs_color=(350, 50))
     assert mock_client.method_calls[-4] == call.put_paramset(
         channel_address="VCU4704397:8",
         paramset_key="VALUES",
         values={"COLOR_BEHAVIOUR": 1, "COLOR": 4, "LEVEL": 1.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.brightness == 255
     assert light.color_name == FixedColor.RED
     assert light.effect == ColorBehaviour.ON
 
     await light.turn_on(hs_color=(0.0, 0.0))
     assert mock_client.method_calls[-4] == call.put_paramset(
         channel_address="VCU4704397:8",
         paramset_key="VALUES",
         values={"COLOR_BEHAVIOUR": 1, "COLOR": 7, "LEVEL": 1.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.brightness == 255
     assert light.color_name == FixedColor.WHITE
     assert light.effect == ColorBehaviour.ON
 
     await light.turn_on(hs_color=(60.0, 50.0))
     assert mock_client.method_calls[-4] == call.put_paramset(
         channel_address="VCU4704397:8",
         paramset_key="VALUES",
         values={"COLOR_BEHAVIOUR": 1, "COLOR": 6, "LEVEL": 1.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.brightness == 255
     assert light.color_name == FixedColor.YELLOW
     assert light.effect == ColorBehaviour.ON
 
     await light.turn_on(hs_color=(120, 50))
     assert mock_client.method_calls[-4] == call.put_paramset(
         channel_address="VCU4704397:8",
         paramset_key="VALUES",
         values={"COLOR_BEHAVIOUR": 1, "COLOR": 2, "LEVEL": 1.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.brightness == 255
     assert light.color_name == FixedColor.GREEN
     assert light.effect == ColorBehaviour.ON
 
     await light.turn_on(hs_color=(180, 50))
     assert mock_client.method_calls[-4] == call.put_paramset(
         channel_address="VCU4704397:8",
         paramset_key="VALUES",
         values={"COLOR_BEHAVIOUR": 1, "COLOR": 3, "LEVEL": 1.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.brightness == 255
     assert light.color_name == FixedColor.TURQUOISE
     assert light.effect == ColorBehaviour.ON
 
     await light.turn_on(hs_color=(240, 50))
     assert mock_client.method_calls[-4] == call.put_paramset(
         channel_address="VCU4704397:8",
         paramset_key="VALUES",
         values={"COLOR_BEHAVIOUR": 1, "COLOR": 1, "LEVEL": 1.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.brightness == 255
     assert light.color_name == FixedColor.BLUE
     assert light.effect == ColorBehaviour.ON
 
     await light.turn_on(hs_color=(300, 50))
     assert mock_client.method_calls[-4] == call.put_paramset(
         channel_address="VCU4704397:8",
         paramset_key="VALUES",
         values={"COLOR_BEHAVIOUR": 1, "COLOR": 5, "LEVEL": 1.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.brightness == 255
     assert light.color_name == FixedColor.PURPLE
     assert light.effect == ColorBehaviour.ON
 
     await light.turn_off()
     assert light.brightness == 0
@@ -570,95 +761,105 @@
     assert light.effect == ColorBehaviour.ON
 
     await light.turn_on(brightness=100)
     assert mock_client.method_calls[-3] == call.put_paramset(
         channel_address="VCU4704397:8",
         paramset_key="VALUES",
         values={"COLOR_BEHAVIOUR": 1, "LEVEL": 0.39215686274509803},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.brightness == 100
     assert light.color_name == FixedColor.PURPLE
     assert light.effect == ColorBehaviour.ON
 
     await light.turn_on(brightness=33)
     assert mock_client.method_calls[-3] == call.put_paramset(
         channel_address="VCU4704397:8",
         paramset_key="VALUES",
         values={"COLOR_BEHAVIOUR": 1, "LEVEL": 0.12941176470588237},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.brightness == 33
     assert light.color_name == FixedColor.PURPLE
     assert light.effect == ColorBehaviour.ON
 
     await light.turn_on(effect="FLASH_MIDDLE")
     assert mock_client.method_calls[-3] == call.put_paramset(
         channel_address="VCU4704397:8",
         paramset_key="VALUES",
         values={"COLOR_BEHAVIOUR": 6, "LEVEL": 0.12941176470588237},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.brightness == 33
     assert light.color_name == FixedColor.PURPLE
     assert light.effect == "FLASH_MIDDLE"
 
     await light.turn_on(brightness=66)
     assert mock_client.method_calls[-3] == call.put_paramset(
         channel_address="VCU4704397:8",
         paramset_key="VALUES",
         values={"COLOR_BEHAVIOUR": 6, "LEVEL": 0.25882352941176473},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.brightness == 66
     assert light.color_name == FixedColor.PURPLE
     assert light.effect == "FLASH_MIDDLE"
 
     await light.turn_off()
 
     light.set_on_time(18)
     await light.turn_on()
     assert mock_client.method_calls[-3] == call.put_paramset(
         channel_address="VCU4704397:8",
         paramset_key="VALUES",
         values={"COLOR_BEHAVIOUR": 6, "DURATION_VALUE": 18, "LEVEL": 1.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
 
     await light.turn_off()
     light.set_on_time(17000)
     await light.turn_on()
     assert mock_client.method_calls[-3] == call.put_paramset(
         channel_address="VCU4704397:8",
         paramset_key="VALUES",
         values={"COLOR_BEHAVIOUR": 6, "DURATION_UNIT": 1, "DURATION_VALUE": 283, "LEVEL": 1.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
 
     await light.turn_off()
     light.set_on_time(1000000)
     await light.turn_on()
     assert mock_client.method_calls[-3] == call.put_paramset(
         channel_address="VCU4704397:8",
         paramset_key="VALUES",
         values={"COLOR_BEHAVIOUR": 6, "DURATION_UNIT": 2, "DURATION_VALUE": 277, "LEVEL": 1.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await light.turn_on(ramp_time=18)
     assert mock_client.method_calls[-3] == call.put_paramset(
         channel_address="VCU4704397:8",
         paramset_key="VALUES",
         values={"COLOR_BEHAVIOUR": 6, "RAMP_TIME_VALUE": 18, "LEVEL": 1.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
 
     await light.turn_on(ramp_time=17000)
     assert mock_client.method_calls[-3] == call.put_paramset(
         channel_address="VCU4704397:8",
         paramset_key="VALUES",
         values={"COLOR_BEHAVIOUR": 6, "RAMP_TIME_UNIT": 1, "RAMP_TIME_VALUE": 283, "LEVEL": 1.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
 
     await light.turn_on(ramp_time=1000000)
     assert mock_client.method_calls[-3] == call.put_paramset(
         channel_address="VCU4704397:8",
         paramset_key="VALUES",
         values={"COLOR_BEHAVIOUR": 6, "RAMP_TIME_UNIT": 2, "RAMP_TIME_VALUE": 277, "LEVEL": 1.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
 
     await light.turn_on()
     call_count = len(mock_client.method_calls)
     await light.turn_on()
     assert call_count == len(mock_client.method_calls)
 
@@ -669,28 +870,46 @@
 
     await light.turn_off()
     await light.turn_on(effect="BLINKING_SLOW")
     assert mock_client.method_calls[-3] == call.put_paramset(
         channel_address="VCU4704397:8",
         paramset_key="VALUES",
         values={"COLOR_BEHAVIOUR": 2, "LEVEL": 1.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
 
     await light.turn_on(brightness=28)
     await light.turn_on(effect="FLASH_MIDDLE")
     assert mock_client.method_calls[-3] == call.put_paramset(
         channel_address="VCU4704397:8",
         paramset_key="VALUES",
         values={"COLOR_BEHAVIOUR": 6, "LEVEL": 0.10980392156862745},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
 
 
-async def test_ceiprgbwlight(factory: helper.Factory) -> None:
+@pytest.mark.asyncio()
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_ceiprgbwlight(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test CeIpRGBWLight."""
-    central, mock_client = await factory.get_default_central(TEST_DEVICES)
+    central, mock_client, _ = central_client_factory
     light: CeIpRGBWLight = cast(
         CeIpRGBWLight, helper.get_prepared_custom_entity(central, "VCU5629873", 1)
     )
     assert light.usage == EntityUsage.CE_PRIMARY
     assert light.color_temp is None
     assert light.hs_color is None
     assert light.supports_brightness is True
@@ -723,37 +942,47 @@
         "EFFECT_10_INTERRUPT_CURRENT_PROFILE",
     )
 
     assert light.brightness == 0
 
     await light.turn_on()
     assert mock_client.method_calls[-2] == call.set_value(
-        channel_address="VCU5629873:1", paramset_key="VALUES", parameter="LEVEL", value=1.0
+        channel_address="VCU5629873:1",
+        paramset_key="VALUES",
+        parameter="LEVEL",
+        value=1.0,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.brightness == 255
     await light.turn_on(brightness=28)
     assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU5629873:1",
         paramset_key="VALUES",
         parameter="LEVEL",
         value=0.10980392156862745,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.brightness == 28
     await light.turn_off()
     assert mock_client.method_calls[-2] == call.set_value(
-        channel_address="VCU5629873:1", paramset_key="VALUES", parameter="LEVEL", value=0.0
+        channel_address="VCU5629873:1",
+        paramset_key="VALUES",
+        parameter="LEVEL",
+        value=0.0,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.brightness == 0
 
     assert light.color_temp is None
     await light.turn_on(color_temp=300)
     assert mock_client.method_calls[-3] == call.put_paramset(
         channel_address="VCU5629873:1",
         paramset_key="VALUES",
         values={"COLOR_TEMPERATURE": 3333, "LEVEL": 1.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.color_temp == 300
 
     await light.turn_on()
     call_count = len(mock_client.method_calls)
     await light.turn_on()
     assert call_count == len(mock_client.method_calls)
@@ -765,47 +994,69 @@
 
     assert light.hs_color is None
     await light.turn_on(hs_color=(44.4, 69.3))
     assert mock_client.method_calls[-4] == call.put_paramset(
         channel_address="VCU5629873:1",
         paramset_key="VALUES",
         values={"HUE": 44, "SATURATION": 0.693, "LEVEL": 1.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.hs_color == (44, 69.3)
 
     await light.turn_on(hs_color=(0, 50))
     assert mock_client.method_calls[-4] == call.put_paramset(
         channel_address="VCU5629873:1",
         paramset_key="VALUES",
         values={"HUE": 0, "SATURATION": 0.5, "LEVEL": 1.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.hs_color == (0.0, 50.0)
 
     await light.turn_on(effect="EFFECT_01_END_CURRENT_PROFILE")
     assert mock_client.method_calls[-2] == call.put_paramset(
-        channel_address="VCU5629873:1", paramset_key="VALUES", values={"EFFECT": 1, "LEVEL": 1.0}
+        channel_address="VCU5629873:1",
+        paramset_key="VALUES",
+        values={"EFFECT": 1, "LEVEL": 1.0},
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
 
     await light.turn_on(hs_color=(44, 66), ramp_time=5)
     assert mock_client.method_calls[-4] == call.put_paramset(
         channel_address="VCU5629873:1",
         paramset_key=ParamsetKey.VALUES,
         values={
             "HUE": 44,
             "SATURATION": 0.66,
             "DURATION_VALUE": 111600,
             "RAMP_TIME_VALUE": 5,
             "LEVEL": 1.0,
         },
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
 
 
-async def test_cecolordimmer(factory: helper.Factory) -> None:
+@pytest.mark.asyncio()
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_cecolordimmer(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test CeColorDimmer."""
-    central, mock_client = await factory.get_default_central(TEST_DEVICES)
+    central, mock_client, _ = central_client_factory
     light: CeColorDimmer = cast(
         CeColorDimmer, helper.get_prepared_custom_entity(central, "VCU9973336", 13)
     )
     assert light.usage == EntityUsage.CE_PRIMARY
     assert light.color_temp is None
     assert light.hs_color == (0.0, 0.0)
     assert light.supports_brightness is True
@@ -815,55 +1066,88 @@
     assert light.supports_transition is True
     assert light.effect is None
 
     assert light.brightness == 0
     assert light.brightness_pct == 0
     await light.turn_on()
     assert mock_client.method_calls[-2] == call.set_value(
-        channel_address="VCU9973336:13", paramset_key="VALUES", parameter="LEVEL", value=1.0
+        channel_address="VCU9973336:13",
+        paramset_key="VALUES",
+        parameter="LEVEL",
+        value=1.0,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.brightness == 255
     await light.turn_on(brightness=28)
     assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU9973336:13",
         paramset_key="VALUES",
         parameter="LEVEL",
         value=0.10980392156862745,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.brightness == 28
     await light.turn_off()
     assert mock_client.method_calls[-2] == call.set_value(
-        channel_address="VCU9973336:13", paramset_key="VALUES", parameter="LEVEL", value=0.0
+        channel_address="VCU9973336:13",
+        paramset_key="VALUES",
+        parameter="LEVEL",
+        value=0.0,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.brightness == 0
 
     assert light.hs_color == (0.0, 0.0)
     await light.turn_on(hs_color=(44.4, 69.3))
     assert mock_client.method_calls[-4] == call.set_value(
-        channel_address="VCU9973336:15", paramset_key="VALUES", parameter="COLOR", value=25
+        channel_address="VCU9973336:15",
+        paramset_key="VALUES",
+        parameter="COLOR",
+        value=25,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert mock_client.method_calls[-2] == call.set_value(
-        channel_address="VCU9973336:13", paramset_key="VALUES", parameter="LEVEL", value=1.0
+        channel_address="VCU9973336:13",
+        paramset_key="VALUES",
+        parameter="LEVEL",
+        value=1.0,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.hs_color == (45.0, 100)
 
     await light.turn_on(hs_color=(0, 50))
     assert mock_client.method_calls[-4] == call.set_value(
-        channel_address="VCU9973336:15", paramset_key="VALUES", parameter="COLOR", value=0
+        channel_address="VCU9973336:15",
+        paramset_key="VALUES",
+        parameter="COLOR",
+        value=0,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert mock_client.method_calls[-2] == call.set_value(
-        channel_address="VCU9973336:13", paramset_key="VALUES", parameter="LEVEL", value=1.0
+        channel_address="VCU9973336:13",
+        paramset_key="VALUES",
+        parameter="LEVEL",
+        value=1.0,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.hs_color == (0.0, 100.0)
     await light.turn_on(hs_color=(0, 1))
     assert mock_client.method_calls[-4] == call.set_value(
-        channel_address="VCU9973336:15", paramset_key="VALUES", parameter="COLOR", value=200
+        channel_address="VCU9973336:15",
+        paramset_key="VALUES",
+        parameter="COLOR",
+        value=200,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert mock_client.method_calls[-2] == call.set_value(
-        channel_address="VCU9973336:13", paramset_key="VALUES", parameter="LEVEL", value=1.0
+        channel_address="VCU9973336:13",
+        paramset_key="VALUES",
+        parameter="LEVEL",
+        value=1.0,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert light.hs_color == (0.0, 0.0)
     await central.event(const.INTERFACE_ID, "VCU9973336:15", "COLOR", 201)
     assert light.hs_color == (0.0, 0.0)
     await central.event(const.INTERFACE_ID, "VCU9973336:15", "COLOR", None)
     assert light.hs_color == (0.0, 0.0)
```

### Comparing `hahomematic-2024.4.9b2/tests/test_lock.py` & `hahomematic-2024.5.0/tests/test_lock.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,80 @@
 """Tests for button entities of hahomematic."""
 
 from __future__ import annotations
 
 from typing import cast
-from unittest.mock import call
+from unittest.mock import Mock, call
 
 import pytest
 
+from hahomematic.central import CentralUnit
+from hahomematic.client import Client
+from hahomematic.config import WAIT_FOR_CALLBACK
 from hahomematic.const import EntityUsage
 from hahomematic.platforms.custom.lock import CeIpLock, CeRfLock
 
 from tests import const, helper
 
 TEST_DEVICES: dict[str, str] = {
     "VCU9724704": "HmIP-DLD.json",
     "VCU0000146": "HM-Sec-Key.json",
 }
 
 # pylint: disable=protected-access
 
 
 @pytest.mark.asyncio()
-async def test_cerflock(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_cerflock(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test CeRfLock."""
-    central, mock_client = await factory.get_default_central(TEST_DEVICES)
+    central, mock_client, _ = central_client_factory
     lock: CeRfLock = cast(CeRfLock, helper.get_prepared_custom_entity(central, "VCU0000146", 1))
     assert lock.usage == EntityUsage.CE_PRIMARY
 
     assert lock.is_locked is True
     await lock.unlock()
     assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU0000146:1",
         paramset_key="VALUES",
         parameter="STATE",
         value=True,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert lock.is_locked is False
     await lock.lock()
     assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU0000146:1",
         paramset_key="VALUES",
         parameter="STATE",
         value=False,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert lock.is_locked is True
     await lock.open()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU0000146:1",
         paramset_key="VALUES",
         parameter="OPEN",
         value=True,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
 
     assert lock.is_locking is None
     await central.event(const.INTERFACE_ID, "VCU0000146:1", "DIRECTION", 2)
     assert lock.is_locking is True
     await central.event(const.INTERFACE_ID, "VCU0000146:1", "DIRECTION", 0)
     assert lock.is_locking is False
@@ -73,45 +94,63 @@
     await lock.open()
     call_count = len(mock_client.method_calls)
     await lock.open()
     assert (call_count + 1) == len(mock_client.method_calls)
 
 
 @pytest.mark.asyncio()
-async def test_ceiplock(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_ceiplock(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test CeIpLock."""
-    central, mock_client = await factory.get_default_central(TEST_DEVICES)
+    central, mock_client, _ = central_client_factory
     lock: CeIpLock = cast(CeIpLock, helper.get_prepared_custom_entity(central, "VCU9724704", 1))
     assert lock.usage == EntityUsage.CE_PRIMARY
 
     assert lock.is_locked is False
     await lock.lock()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU9724704:1",
         paramset_key="VALUES",
         parameter="LOCK_TARGET_LEVEL",
         value=0,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU9724704:1", "LOCK_STATE", 1)
     assert lock.is_locked is True
     await lock.unlock()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU9724704:1",
         paramset_key="VALUES",
         parameter="LOCK_TARGET_LEVEL",
         value=1,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU9724704:1", "LOCK_STATE", 2)
     assert lock.is_locked is False
     await lock.open()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU9724704:1",
         paramset_key="VALUES",
         parameter="LOCK_TARGET_LEVEL",
         value=2,
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
 
     assert lock.is_locking is None
     await central.event(const.INTERFACE_ID, "VCU9724704:1", "ACTIVITY_STATE", 2)
     assert lock.is_locking is True
     await central.event(const.INTERFACE_ID, "VCU9724704:1", "ACTIVITY_STATE", 0)
     assert lock.is_locking is False
```

### Comparing `hahomematic-2024.4.9b2/tests/test_siren.py` & `hahomematic-2024.5.0/tests/test_siren.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,51 @@
 """Tests for siren entities of hahomematic."""
 
 from __future__ import annotations
 
 from typing import cast
-from unittest.mock import call
+from unittest.mock import Mock, call
 
 import pytest
 
+from hahomematic.central import CentralUnit
+from hahomematic.client import Client
+from hahomematic.config import WAIT_FOR_CALLBACK
 from hahomematic.const import EntityUsage
 from hahomematic.platforms.custom.siren import CeIpSiren, CeIpSirenSmoke
 
 from tests import const, helper
 
 TEST_DEVICES: dict[str, str] = {
     "VCU8249617": "HmIP-ASIR-2.json",
     "VCU2822385": "HmIP-SWSD.json",
 }
 
 # pylint: disable=protected-access
 
 
 @pytest.mark.asyncio()
-async def test_ceipsiren(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_ceipsiren(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test CeIpSiren."""
-    central, mock_client = await factory.get_default_central(TEST_DEVICES)
+    central, mock_client, _ = central_client_factory
     siren: CeIpSiren = cast(CeIpSiren, helper.get_prepared_custom_entity(central, "VCU8249617", 3))
     assert siren.usage == EntityUsage.CE_PRIMARY
 
     assert siren.is_on is False
     await central.event(const.INTERFACE_ID, "VCU8249617:3", "ACOUSTIC_ALARM_ACTIVE", 1)
     assert siren.is_on is True
     await central.event(const.INTERFACE_ID, "VCU8249617:3", "ACOUSTIC_ALARM_ACTIVE", 0)
@@ -47,14 +65,15 @@
         paramset_key="VALUES",
         values={
             "ACOUSTIC_ALARM_SELECTION": 3,
             "OPTICAL_ALARM_SELECTION": 1,
             "DURATION_UNIT": 0,
             "DURATION_VALUE": 30,
         },
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
 
     await siren.turn_on(
         acoustic_alarm="FREQUENCY_RISING_AND_FALLING",
         optical_alarm="BLINKING_ALTERNATELY_REPEATING",
         duration=30,
     )
@@ -63,14 +82,15 @@
         paramset_key="VALUES",
         values={
             "ACOUSTIC_ALARM_SELECTION": 3,
             "OPTICAL_ALARM_SELECTION": 1,
             "DURATION_UNIT": 0,
             "DURATION_VALUE": 30,
         },
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
 
     with pytest.raises(ValueError):
         await siren.turn_on(
             acoustic_alarm="not_in_list",
             optical_alarm="BLINKING_ALTERNATELY_REPEATING",
             duration=30,
@@ -89,26 +109,42 @@
         paramset_key="VALUES",
         values={
             "ACOUSTIC_ALARM_SELECTION": 0,
             "OPTICAL_ALARM_SELECTION": 0,
             "DURATION_UNIT": 0,
             "DURATION_VALUE": 0,
         },
+        wait_for_callback=WAIT_FOR_CALLBACK,
     )
 
     await siren.turn_off()
     call_count = len(mock_client.method_calls)
     await siren.turn_off()
     assert (call_count + 1) == len(mock_client.method_calls)
 
 
 @pytest.mark.asyncio()
-async def test_ceipsirensmoke(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_ceipsirensmoke(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test CeIpSirenSmoke."""
-    central, mock_client = await factory.get_default_central(TEST_DEVICES)
+    central, mock_client, _ = central_client_factory
     siren: CeIpSirenSmoke = cast(
         CeIpSirenSmoke, helper.get_prepared_custom_entity(central, "VCU2822385", 1)
     )
     assert siren.usage == EntityUsage.CE_PRIMARY
 
     assert siren.is_on is False
     await central.event(const.INTERFACE_ID, "VCU2822385:1", "SMOKE_DETECTOR_ALARM_STATUS", 1)
```

### Comparing `hahomematic-2024.4.9b2/tests/test_support.py` & `hahomematic-2024.5.0/tests/test_support.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """Tests for switch entities of hahomematic."""
 
 from __future__ import annotations
 
 from collections.abc import Callable
 from datetime import datetime, timedelta
 from typing import Any
-from unittest.mock import patch
+from unittest.mock import Mock, patch
 
 import pytest
 
 from hahomematic.caches.visibility import _get_value_from_dict_by_wildcard_key
+from hahomematic.central import CentralUnit
+from hahomematic.client import Client
 from hahomematic.const import INIT_DATETIME, EntityUsage, ParameterType, SysvarType
 from hahomematic.converter import _COMBINED_PARAMETER_TO_HM_CONVERTER, convert_hm_level_to_cpv
 from hahomematic.exceptions import HaHomematicException
 from hahomematic.platforms.support import (
     _check_channel_name_with_channel_no,
     convert_value,
     generate_unique_id,
@@ -43,17 +45,32 @@
     "VCU3609622": "HmIP-eTRV-2.json",
 }
 
 # pylint: disable=protected-access
 
 
 @pytest.mark.asyncio()
-async def test_generate_unique_id(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        ({}, True, False, False, None, None),
+    ],
+)
+async def test_generate_unique_id(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test generate_unique_id."""
-    central, _ = await factory.get_default_central({})
+    central, _, _ = central_client_factory
     assert (
         generate_unique_id(central=central, address="VCU2128127", parameter="LEVEL")
         == "vcu2128127_level"
     )
     assert (
         generate_unique_id(
             central=central, address="VCU2128127", parameter="LEVEL", prefix="PREFIX"
@@ -151,17 +168,32 @@
     assert to_bool(value="blabla") is False
     assert to_bool(value="2") is False
     with pytest.raises(TypeError):
         to_bool(value=2)
 
 
 @pytest.mark.asyncio()
-async def test_get_entity_name(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_get_entity_name(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test get_entity_name."""
-    central, _ = await factory.get_default_central(TEST_DEVICES)
+    central, _, _ = central_client_factory
     device = central.get_device(address="VCU2128127")
     name_data = get_entity_name(central=central, device=device, channel_no=4, parameter="LEVEL")
     assert name_data.full_name == "HmIP-BSM_VCU2128127 Level"
     assert name_data.entity_name == "Level"
 
     central.device_details.add_name(address=f"{device.device_address}:5", name="Roof")
     name_data = get_entity_name(central=central, device=device, channel_no=5, parameter="LEVEL")
@@ -176,17 +208,32 @@
             central=central, device=device, channel_no=5, parameter="LEVEL"
         )
         assert name_data.full_name == ""
         assert name_data.entity_name is None
 
 
 @pytest.mark.asyncio()
-async def test_get_event_name(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_get_event_name(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test get_event_name."""
-    central, _ = await factory.get_default_central(TEST_DEVICES)
+    central, _, _ = central_client_factory
     device = central.get_device(address="VCU2128127")
     name_data = get_event_name(central=central, device=device, channel_no=4, parameter="LEVEL")
     assert name_data.channel_name == "ch4"
     assert name_data.entity_name == "ch4 Level"
     assert name_data.full_name == "HmIP-BSM_VCU2128127 ch4 Level"
 
     central.device_details.add_name(address=f"{device.device_address}:5", name="Roof")
@@ -201,17 +248,32 @@
     ):
         name_data = get_event_name(central=central, device=device, channel_no=5, parameter="LEVEL")
         assert name_data.full_name == ""
         assert name_data.entity_name is None
 
 
 @pytest.mark.asyncio()
-async def test_custom_entity_name(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_custom_entity_name(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test get_custom_entity_name."""
-    central, _ = await factory.get_default_central(TEST_DEVICES)
+    central, _, _ = central_client_factory
     device = central.get_device(address="VCU2128127")
     name_data = get_custom_entity_name(
         central=central,
         device=device,
         channel_no=4,
         is_only_primary_channel=True,
         usage=EntityUsage.CE_PRIMARY,
@@ -262,17 +324,32 @@
             usage=EntityUsage.CE_SECONDARY,
         )
         assert name_data.full_name == ""
         assert name_data.entity_name is None
 
 
 @pytest.mark.asyncio()
-async def test_get_device_name(factory: helper.Factory) -> None:
+@pytest.mark.parametrize(
+    (
+        "address_device_translation",
+        "do_mock_client",
+        "add_sysvars",
+        "add_programs",
+        "ignore_devices_on_create",
+        "un_ignore_list",
+    ),
+    [
+        (TEST_DEVICES, True, False, False, None, None),
+    ],
+)
+async def test_get_device_name(
+    central_client_factory: tuple[CentralUnit, Client | Mock, helper.Factory],
+) -> None:
     """Test get_device_name."""
-    central, _ = await factory.get_default_central(TEST_DEVICES)
+    central, _, _ = central_client_factory
     assert (
         get_device_name(central=central, device_address="VCU2128127", device_type="HmIP-BSM")
         == "HmIP-BSM_VCU2128127"
     )
     central.device_details.add_name(address="VCU2128127", name="Roof")
     assert (
         get_device_name(central=central, device_address="VCU2128127", device_type="HmIP-BSM")
```

