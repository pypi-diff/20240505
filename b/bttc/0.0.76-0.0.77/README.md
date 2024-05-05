# Comparing `tmp/bttc-0.0.76.tar.gz` & `tmp/bttc-0.0.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bttc-0.0.76.tar", last modified: Sun Apr 28 06:24:06 2024, max compression
+gzip compressed data, was "bttc-0.0.77.tar", last modified: Sun May  5 01:23:20 2024, max compression
```

## Comparing `bttc-0.0.76.tar` & `bttc-0.0.77.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-28 06:24:06.265039 bttc-0.0.76/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1061 2023-08-09 04:39:34.000000 bttc-0.0.76/LICENSE
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2134 2024-04-28 06:24:06.265039 bttc-0.0.76/PKG-INFO
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1406 2024-04-28 06:23:45.000000 bttc-0.0.76/README.md
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-28 06:24:06.261039 bttc-0.0.76/bttc/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6836 2024-04-28 06:22:52.000000 bttc-0.0.76/bttc/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     9617 2024-04-15 06:13:29.000000 bttc-0.0.76/bttc/apk_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2389 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/ble_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     4752 2024-04-08 13:33:17.000000 bttc-0.0.76/bttc/ble_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1723 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/bt_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    16481 2024-04-28 06:22:01.000000 bttc-0.0.76/bttc/bt_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-28 06:24:06.261039 bttc-0.0.76/bttc/cli/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2100 2024-04-10 06:01:48.000000 bttc-0.0.76/bttc/cli/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1150 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/cli/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    22596 2024-04-15 06:24:35.000000 bttc-0.0.76/bttc/cli/main.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      976 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/common_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3956 2024-04-28 06:22:01.000000 bttc-0.0.76/bttc/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1351 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/core.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2199 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1182 2024-04-28 06:22:01.000000 bttc-0.0.76/bttc/general_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    32048 2024-04-28 06:22:01.000000 bttc-0.0.76/bttc/general_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1062 2024-04-28 06:22:01.000000 bttc-0.0.76/bttc/mc_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5053 2024-04-28 06:22:01.000000 bttc-0.0.76/bttc/mc_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-28 06:24:06.261039 bttc-0.0.76/bttc/mobly_android_device_lib/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    13864 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/mobly_android_device_lib/jsonrpc_client_base.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-28 06:24:06.261039 bttc-0.0.76/bttc/mobly_android_device_lib/services/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6408 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/mobly_android_device_lib/services/sl4a_client.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2295 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/mobly_android_device_lib/services/sl4a_service.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6095 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/mobly_android_device_lib/tl4a_snippet_client.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-28 06:24:06.257039 bttc-0.0.76/bttc/profiles/
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-28 06:24:06.261039 bttc-0.0.76/bttc/profiles/avrcp/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/profiles/avrcp/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3189 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/profiles/avrcp/avrcp_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5692 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/profiles/avrcp/avrcp_target_devices.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      915 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/profiles/avrcp/errors.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-28 06:24:06.261039 bttc-0.0.76/bttc/profiles/hfp/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1221 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/profiles/hfp/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      962 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/profiles/hfp/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      967 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/profiles/hfp/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1581 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/profiles/hfp/hfp_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     8250 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/profiles/hfp/hfp_devices.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5816 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/profiles/hfp/hfp_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3324 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/profiles/hfp/hfp_strategy.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1567 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/strategy.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-28 06:24:06.261039 bttc-0.0.76/bttc/utils/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1868 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/utils/ad_checker.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3932 2024-04-15 06:13:29.000000 bttc-0.0.76/bttc/utils/device_factory.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-28 06:24:06.261039 bttc-0.0.76/bttc/utils/iperf/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7860 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/utils/iperf/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      856 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/utils/iperf/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5144 2024-04-28 06:22:01.000000 bttc-0.0.76/bttc/utils/key_events_handler.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7826 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/utils/log_parser.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7268 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/utils/logcat.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-28 06:24:06.261039 bttc-0.0.76/bttc/utils/media_player/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1227 2024-04-28 06:22:01.000000 bttc-0.0.76/bttc/utils/media_player/media_player_agent_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     4968 2024-04-28 06:22:01.000000 bttc-0.0.76/bttc/utils/media_player/yt_player_agent.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    43699 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/utils/retry.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2249 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/utils/typing_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-28 06:24:06.265039 bttc-0.0.76/bttc/utils/ui_pages/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3877 2024-04-28 06:22:01.000000 bttc-0.0.76/bttc/utils/ui_pages/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1677 2024-04-28 06:22:01.000000 bttc-0.0.76/bttc/utils/ui_pages/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    16204 2024-04-28 06:22:01.000000 bttc-0.0.76/bttc/utils/ui_pages/ui_core.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7585 2024-04-28 06:22:01.000000 bttc-0.0.76/bttc/utils/ui_pages/ui_node.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2320 2024-04-28 06:22:01.000000 bttc-0.0.76/bttc/utils/ui_pages/utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2960 2024-04-28 06:22:01.000000 bttc-0.0.76/bttc/utils_loader.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5098 2024-03-30 03:00:32.000000 bttc-0.0.76/bttc/wifi_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-28 06:24:06.261039 bttc-0.0.76/bttc.egg-info/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2134 2024-04-28 06:24:06.000000 bttc-0.0.76/bttc.egg-info/PKG-INFO
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1587 2024-04-28 06:24:06.000000 bttc-0.0.76/bttc.egg-info/SOURCES.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)        1 2024-04-28 06:24:06.000000 bttc-0.0.76/bttc.egg-info/dependency_links.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      185 2024-04-28 06:24:06.000000 bttc-0.0.76/bttc.egg-info/requires.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)        5 2024-04-28 06:24:06.000000 bttc-0.0.76/bttc.egg-info/top_level.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)       38 2024-04-28 06:24:06.265039 bttc-0.0.76/setup.cfg
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1772 2024-04-28 06:22:01.000000 bttc-0.0.76/setup.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:23:20.940626 bttc-0.0.77/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1061 2023-08-09 04:39:34.000000 bttc-0.0.77/LICENSE
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2158 2024-05-05 01:23:20.940626 bttc-0.0.77/PKG-INFO
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1430 2024-05-05 01:23:10.000000 bttc-0.0.77/README.md
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:23:20.932626 bttc-0.0.77/bttc/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6836 2024-05-05 01:22:46.000000 bttc-0.0.77/bttc/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     9617 2024-04-15 06:13:29.000000 bttc-0.0.77/bttc/apk_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2389 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/ble_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     4752 2024-04-08 13:33:17.000000 bttc-0.0.77/bttc/ble_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1723 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/bt_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    16481 2024-04-28 06:22:01.000000 bttc-0.0.77/bttc/bt_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:23:20.936626 bttc-0.0.77/bttc/cli/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2100 2024-04-10 06:01:48.000000 bttc-0.0.77/bttc/cli/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1150 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/cli/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    22596 2024-04-15 06:24:35.000000 bttc-0.0.77/bttc/cli/main.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      976 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/common_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3956 2024-04-28 06:22:01.000000 bttc-0.0.77/bttc/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1351 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/core.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2199 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     4211 2024-05-05 01:21:12.000000 bttc-0.0.77/bttc/general_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    35298 2024-05-05 01:21:12.000000 bttc-0.0.77/bttc/general_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1062 2024-04-28 06:22:01.000000 bttc-0.0.77/bttc/mc_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5053 2024-04-28 06:22:01.000000 bttc-0.0.77/bttc/mc_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:23:20.936626 bttc-0.0.77/bttc/mobly_android_device_lib/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    13864 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/mobly_android_device_lib/jsonrpc_client_base.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:23:20.936626 bttc-0.0.77/bttc/mobly_android_device_lib/services/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6408 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/mobly_android_device_lib/services/sl4a_client.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2295 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/mobly_android_device_lib/services/sl4a_service.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6095 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/mobly_android_device_lib/tl4a_snippet_client.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:23:20.928626 bttc-0.0.77/bttc/profiles/
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:23:20.936626 bttc-0.0.77/bttc/profiles/avrcp/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/profiles/avrcp/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3189 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/profiles/avrcp/avrcp_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5692 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/profiles/avrcp/avrcp_target_devices.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      915 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/profiles/avrcp/errors.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:23:20.936626 bttc-0.0.77/bttc/profiles/hfp/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1221 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/profiles/hfp/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      962 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/profiles/hfp/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      967 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/profiles/hfp/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1581 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/profiles/hfp/hfp_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     8250 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/profiles/hfp/hfp_devices.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5816 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/profiles/hfp/hfp_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3324 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/profiles/hfp/hfp_strategy.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1567 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/strategy.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:23:20.936626 bttc-0.0.77/bttc/utils/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1868 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/utils/ad_checker.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3932 2024-04-15 06:13:29.000000 bttc-0.0.77/bttc/utils/device_factory.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:23:20.940626 bttc-0.0.77/bttc/utils/iperf/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7860 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/utils/iperf/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      856 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/utils/iperf/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5893 2024-05-05 01:21:12.000000 bttc-0.0.77/bttc/utils/key_events_handler.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    10543 2024-05-05 01:21:12.000000 bttc-0.0.77/bttc/utils/log_parser.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7268 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/utils/logcat.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:23:20.940626 bttc-0.0.77/bttc/utils/media_player/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1227 2024-04-28 06:22:01.000000 bttc-0.0.77/bttc/utils/media_player/media_player_agent_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5138 2024-05-05 01:21:12.000000 bttc-0.0.77/bttc/utils/media_player/yt_player_agent.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    43699 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/utils/retry.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2249 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/utils/typing_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:23:20.940626 bttc-0.0.77/bttc/utils/ui_pages/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3877 2024-04-28 06:22:01.000000 bttc-0.0.77/bttc/utils/ui_pages/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1677 2024-04-29 08:53:55.000000 bttc-0.0.77/bttc/utils/ui_pages/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    16204 2024-04-28 06:22:01.000000 bttc-0.0.77/bttc/utils/ui_pages/ui_core.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7585 2024-04-28 06:22:01.000000 bttc-0.0.77/bttc/utils/ui_pages/ui_node.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2320 2024-04-28 06:22:01.000000 bttc-0.0.77/bttc/utils/ui_pages/utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2960 2024-04-28 06:22:01.000000 bttc-0.0.77/bttc/utils_loader.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5098 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/wifi_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:23:20.932626 bttc-0.0.77/bttc.egg-info/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2158 2024-05-05 01:23:20.000000 bttc-0.0.77/bttc.egg-info/PKG-INFO
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1587 2024-05-05 01:23:20.000000 bttc-0.0.77/bttc.egg-info/SOURCES.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)        1 2024-05-05 01:23:20.000000 bttc-0.0.77/bttc.egg-info/dependency_links.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      185 2024-05-05 01:23:20.000000 bttc-0.0.77/bttc.egg-info/requires.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)        5 2024-05-05 01:23:20.000000 bttc-0.0.77/bttc.egg-info/top_level.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)       38 2024-05-05 01:23:20.940626 bttc-0.0.77/setup.cfg
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1772 2024-04-28 06:22:01.000000 bttc-0.0.77/setup.py
```

### Comparing `bttc-0.0.76/LICENSE` & `bttc-0.0.77/LICENSE`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/PKG-INFO` & `bttc-0.0.77/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bttc
-Version: 0.0.76
+Version: 0.0.77
 Summary: A package to provide common utilities for BT testing.
 Home-page: https://github.com/johnklee/bt_test_common
 Author: John Lee/Yuan Long Luo/Denny Chai
 Author-email: puremonkey2007@gmail.com
 License: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -61,14 +61,15 @@
 >>> import bttc
 >>> dut = bttc.get('07311JECB08252', {'wifi'})
 >>> dut.wifi.status()
 <WifiStatus.ENABLED: 'enabled'>
 ```
 
 ## Release info
+* Release v0.0.77: #202
 * Release v0.0.76: #198, #196, #194, #192
 * Release v0.0.75: #64
 * Release v0.0.74: #125, #159, #171, #173, #176, #178, #180
 * Release v0.0.73: #158, #163
 * Release v0.0.72: #153, #155, #51, #157
 * Release v0.0.71: #123, #134, #140
 * Release v0.0.70: #128, #132, #135
```

### Comparing `bttc-0.0.76/README.md` & `bttc-0.0.77/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 >>> import bttc
 >>> dut = bttc.get('07311JECB08252', {'wifi'})
 >>> dut.wifi.status()
 <WifiStatus.ENABLED: 'enabled'>
 ```
 
 ## Release info
+* Release v0.0.77: #202
 * Release v0.0.76: #198, #196, #194, #192
 * Release v0.0.75: #64
 * Release v0.0.74: #125, #159, #171, #173, #176, #178, #180
 * Release v0.0.73: #158, #163
 * Release v0.0.72: #153, #155, #51, #157
 * Release v0.0.71: #123, #134, #140
 * Release v0.0.70: #128, #132, #135
```

### Comparing `bttc-0.0.76/bttc/__init__.py` & `bttc-0.0.77/bttc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from bttc import utils_loader
 from bttc.utils import device_factory
 from ppadb import client
 import shlex
 from typing import Callable, TypeAlias
 
 
-__version__ = '0.0.76'
+__version__ = '0.0.77'
 __author__ = 'John Lee/Yuan Long Luo/Denny Chai'
 __credits__ = 'Google Pixel PQM'
 
 
 GeneralDevice: TypeAlias = android_device.AndroidDevice
```

### Comparing `bttc-0.0.76/bttc/apk_utils.py` & `bttc-0.0.77/bttc/apk_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/ble_data.py` & `bttc-0.0.77/bttc/ble_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/ble_utils.py` & `bttc-0.0.77/bttc/ble_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/bt_data.py` & `bttc-0.0.77/bttc/bt_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/bt_utils.py` & `bttc-0.0.77/bttc/bt_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/cli/__init__.py` & `bttc-0.0.77/bttc/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/cli/constants.py` & `bttc-0.0.77/bttc/cli/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/cli/main.py` & `bttc-0.0.77/bttc/cli/main.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/common_data.py` & `bttc-0.0.77/bttc/common_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/constants.py` & `bttc-0.0.77/bttc/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/core.py` & `bttc-0.0.77/bttc/core.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/errors.py` & `bttc-0.0.77/bttc/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/general_utils.py` & `bttc-0.0.77/bttc/general_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,22 +20,24 @@
 import logging
 import os
 import re
 import sys
 from subprocess import Popen, PIPE
 import time
 
+import bttc
 from bttc import bt_utils
 from bttc import constants
 from bttc import core
 from bttc import errors
 from bttc import general_data
 from bttc.cli.constants import warning
 from bttc.utils import device_factory
 from bttc.utils import key_events_handler
+from bttc.utils import log_parser
 from bttc.utils import typing_utils
 from mobly import utils
 
 from mobly.controllers import android_device
 from mobly.controllers.android_device_lib import adb
 from mobly.controllers.android_device_lib.errors import DeviceError
 
@@ -60,14 +62,17 @@
 
 # Pattern to match message of logcat service.
 _LOGCAT_MSG_PATTERN = constants.LOGTCAT_MSG_PATTERN
 
 # Command to retrieve SDK information.
 _CMD_GET_SDK_VERSION = "getprop ro.build.version.sdk"
 
+# The index of the setStreamVolume functio
+_FUNC_IDX_SETSTREAMVOL = '10'
+
 
 class DeviceConfig:
   """Utility class to handle device_config of DUT."""
 
   SettingPattern = re.compile(
       r'^(?P<setting_name>[ ._a-zA-Z0-9]+)='
       r'(?P<setting_value>.*)$')
@@ -352,18 +357,21 @@
     self._bind(enable_airplane_mode)
     self._bind(follow_logcat)
     self._bind(follow_logcat_within)
     self._bind(get_call_state)
     self._bind(get_current_activity)
     self._bind(get_device_time)
     self._bind(get_ui_xml)
+    self._bind(get_all_volume)
+    self._bind(get_volume)
     self._bind(is_apk_installed)
     self._bind(logcat_filter)
     self.props = Props(self._ad)
     self._bind(push_file)
+    self._bind(set_volume)
     self.shell = bt_utils.safe_adb_shell(ad)
     self._bind(take_screenshot)
 
   @property
   def airplane_mode(self) -> bool:
     """Gets the current airplane mode status of the device.
 
@@ -403,14 +411,20 @@
   @property
   def sim_operator(self):
     return get_sim_operator(self._ad)
 
   def quick_setting_page(self):
     return go_bt_quick_setting_page(self._ad)
 
+  def volume_down(self):
+    self.dut.ke.key_volume_down()
+
+  def volume_up(self):
+    self.dut.ke.key_volume_up()
+
 
 def bind(
     ad: Union[ANDROID_DEVICE, str],
     depress_error: bool = True,
     init_mbs: bool = False,
     init_sl4a: bool = False,
     init_snippet_uiautomator: bool = False,
@@ -972,14 +986,64 @@
     raise errors.MethodError(
         sys._getframe().f_code.co_name,
         'Failed to get XML content of current UI!')
 
   return ui_xml_content
 
 
+def get_all_volume(
+    ad: typing_utils.AdbDevice) -> dict[str, general_data.AudioStreamVolume]:
+  """Gets all the types of volume setting.
+
+  Args:
+    ad: Device to retrieve volume setting.
+
+  Returns:
+    The settings of all audio volume types with key as name; value as settings.
+  """
+  stdout, _, ret_code = bt_utils.safe_adb_shell(ad)('dumpsys audio')
+
+  if ret_code != 0:
+    raise adb.Error(
+        f'Failed to get volume with stdout: {stdout} (rt={ret_code})')
+
+  return log_parser.parse_audio_dump_for_volume_info(stdout)
+
+
+def get_volume(
+    ad: typing_utils.AdbDevice,
+    volume_type: general_data.VolumeType) -> general_data.VolumeSetting:
+  """Gets the setting of a certain volume type.
+
+  Args:
+    ad: Device to retrieve volume setting.
+    volume_type: Volume type to query on.
+
+  Returns:
+    The current volume setting.
+  """
+  key = volume_type.m.key or volume_type.m.stream_type
+  shell_cmd = f'settings get system {key}'
+  stdout, _, ret_code = bttc.safe_adb_shell(ad)(shell_cmd)
+  if ret_code != 0:
+    raise adb.Error(
+        f'Failed to get volume with stdout: {stdout} (rt={ret_code})')
+
+  stdout = stdout.strip()
+  if stdout == 'null':
+    raise adb.Error(
+        f'Failed to get volume by command: "{shell_cmd}"')
+
+  volume_level = int(stdout.strip())
+  return general_data.VolumeSetting(
+      level=volume_level,
+      is_max=volume_level >= volume_type.m.max,
+      is_min=volume_level <= volume_type.m.min)
+
+
 def is_apk_installed(
     device: typing_utils.AdbDevice, package_name: str, is_full: bool = False
 ) -> bool:
   """Checks if the given apk is installed.
 
   Below is the output of partial package:
   ```
@@ -1008,15 +1072,15 @@
   Returns:
     True iff the given APK package name installed.
   """
   command = (
       f'pm list packages {"-f" if is_full else ""} '
       f'| grep -w "package:{package_name}"'
   )
-  stdout, _, ret_code = bt_utils.safe_adb_shell(device)(command)
+  stdout, _, ret_code = bttc.safe_adb_shell(device)(command)
 
   return ret_code == 0 and package_name in stdout
 
 
 def logcat_filter(
     ad: typing_utils.AdbDevice,
     start_time: str | None = None,
@@ -1107,14 +1171,62 @@
         "Failed to copy %s to %s: %s", src_file_path, dst_file_path, out
     )
     return False
 
   return True
 
 
+def set_volume(
+    ad: typing_utils.AdbDevice,
+    volume_type: general_data.VolumeType,
+    level: int,
+    sync_wait_sec: int = 2) -> str:
+  """Sets the level of a certain volume type.
+
+  Passes value out of boundary will be adjusted to boudary value.
+
+  Via adb command (put) to update volume values in settings is not working.
+  Need to use Android Interface Definition Language (AIDL) instead.
+  Refer to: cs/frameworks/base/media/java/android/media/IAudioService.aidl
+  for further information.
+
+  Args:
+    ad: Device to set the volume.
+    volume_type: Volume type to qork on.
+    level: Level to set in.
+    sync_wait_sec: Time of second to wait after setting the volume level for the
+      device to sync up.
+
+  Returns:
+    adb shell command return value.
+
+  Raises:
+    ValueError: Giving invalid level value.
+  """
+  if level < volume_type.m.min:
+    raise ValueError(
+        f'Level={level} is less than the minimum level from {volume_type.m}')
+  elif level > volume_type.m.max:
+    raise ValueError(
+        f'Level={level} is higher than the maximum level from {volume_type.m}')
+
+  shell_cmd = ' '.join([
+      'service', 'call', 'audio', _FUNC_IDX_SETSTREAMVOL, 'i32',
+      volume_type.m.stream_type, 'i32',
+      str(level), 'i32', '1'])
+
+  stdout, _, ret_code = bttc.safe_adb_shell(ad)(shell_cmd)
+  if ret_code != 0:
+    raise adb.Error(
+        f'Failed to get volue with stdout: {stdout} (rt={ret_code})')
+
+  time.sleep(sync_wait_sec)
+  return stdout.strip()
+
+
 def take_screenshot(
     ad: typing_utils.AdbDevice, host_destination: str,
     file_name: str | None = None
 ) -> str:
   """Takes a screenshot of the device.
 
   Args:
```

### Comparing `bttc-0.0.76/bttc/mc_data.py` & `bttc-0.0.77/bttc/mc_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/mc_utils.py` & `bttc-0.0.77/bttc/mc_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/mobly_android_device_lib/jsonrpc_client_base.py` & `bttc-0.0.77/bttc/mobly_android_device_lib/jsonrpc_client_base.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/mobly_android_device_lib/services/sl4a_client.py` & `bttc-0.0.77/bttc/mobly_android_device_lib/services/sl4a_client.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/mobly_android_device_lib/services/sl4a_service.py` & `bttc-0.0.77/bttc/mobly_android_device_lib/services/sl4a_service.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/mobly_android_device_lib/tl4a_snippet_client.py` & `bttc-0.0.77/bttc/mobly_android_device_lib/tl4a_snippet_client.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/profiles/avrcp/__init__.py` & `bttc-0.0.77/bttc/profiles/avrcp/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/profiles/avrcp/avrcp_facade.py` & `bttc-0.0.77/bttc/profiles/avrcp/avrcp_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/profiles/avrcp/avrcp_target_devices.py` & `bttc-0.0.77/bttc/profiles/avrcp/avrcp_target_devices.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/profiles/avrcp/errors.py` & `bttc-0.0.77/bttc/profiles/avrcp/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/profiles/hfp/__init__.py` & `bttc-0.0.77/bttc/profiles/hfp/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/profiles/hfp/constants.py` & `bttc-0.0.77/bttc/profiles/hfp/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/profiles/hfp/errors.py` & `bttc-0.0.77/bttc/profiles/hfp/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/profiles/hfp/hfp_data.py` & `bttc-0.0.77/bttc/profiles/hfp/hfp_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/profiles/hfp/hfp_devices.py` & `bttc-0.0.77/bttc/profiles/hfp/hfp_devices.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/profiles/hfp/hfp_facade.py` & `bttc-0.0.77/bttc/profiles/hfp/hfp_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/profiles/hfp/hfp_strategy.py` & `bttc-0.0.77/bttc/profiles/hfp/hfp_strategy.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/strategy.py` & `bttc-0.0.77/bttc/strategy.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/utils/ad_checker.py` & `bttc-0.0.77/bttc/utils/ad_checker.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/utils/device_factory.py` & `bttc-0.0.77/bttc/utils/device_factory.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/utils/iperf/__init__.py` & `bttc-0.0.77/bttc/utils/iperf/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/utils/iperf/errors.py` & `bttc-0.0.77/bttc/utils/iperf/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/utils/key_events_handler.py` & `bttc-0.0.77/bttc/utils/key_events_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,14 +32,27 @@
   NEXT = 87
   PREVIOUS = 88
   PLAY = 126
   PAUSE = 127
 
 
 @enum.unique
+class VolumeKeyCode(enum.Enum):
+  """Volume related key codes."""
+  # https://developer.android.com/reference/android/view/KeyEvent#KEYCODE_VOLUME_DOWN
+  DOWN = 25
+
+  # https://developer.android.com/reference/android/view/KeyEvent#KEYCODE_VOLUME_MUTE
+  MUTE = 164
+
+  # https://developer.android.com/reference/android/view/KeyEvent#KEYCODE_VOLUME_UP
+  UP = 24
+
+
+@enum.unique
 class KeycodeNumPad(enum.Enum):
   """Enum class for Numpad key event."""
 
   NUM_0 = '0'
   NUM_1 = '1'
   NUM_2 = '2'
   NUM_3 = '3'
@@ -212,7 +225,19 @@
       numpad_str: Numpad as string.
     """
     enum_numpad = KeycodeNumPad.from_str(numpad_str)
     if enum_numpad is None:
       raise ValueError(f'Invalid numpad string="{numpad_str}"')
 
     self.key_numpad(enum_numpad)
+
+  def key_volume_down(self):
+    """Sends key event `KEYCODE_VOLUME_DOWN`."""
+    self.send_keycode(VolumeKeyCode.DOWN.value)
+
+  def key_volume_mute(self):
+    """Sends key event `KEYCODE_VOLUME_MUTE`."""
+    self.send_keycode(VolumeKeyCode.MUTE.value)
+
+  def key_volume_up(self):
+    """Sends key event `KEYCODE_VOLUME_UP`."""
+    self.send_keycode(VolumeKeyCode.UP.value)
```

### Comparing `bttc-0.0.76/bttc/utils/log_parser.py` & `bttc-0.0.77/bttc/utils/log_parser.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,28 +13,92 @@
 # limitations under the License.
 
 
 from dataclasses import fields
 from typing import Sequence
 from bttc import bt_data
 from bttc import constants
+from bttc import general_data
 from bttc import errors
 from bttc import ble_data
+import logging
 import re
 
 
 BondedDeviceInfo = bt_data.BondedDeviceInfo
 LeAudioServiceInfo = ble_data.LeAudioService
 ActiveGroupInfo = ble_data.ActiveGroupInfo
 GroupInfo = ble_data.GroupInfo
 DeviceInfo = ble_data.DeviceInfo
 StateMachineLog = ble_data.StateMachineLog
 LeAudioStateMachine = ble_data.LeAudioStateMachine
 
 
+def parse_audio_dump_for_volume_info(
+    log_content: str) -> dict[str, general_data.AudioStreamVolume]:
+  """Parses the audio dumps to retrieve the volume information."""
+  stream_header_pattern = re.compile('STREAM_([_A-Z0-9]+)')
+  log_lines = log_content.split('\n')
+  current_volume_setting_record: general_data.AudioStreamVolume | None = None
+  collected_volume_info: dict[str, general_data.AudioStreamVolume] = {}
+  for i, line in enumerate(log_lines):
+    if line.startswith('Stream volumes'):
+      # Start parsing
+      for line in log_lines[i+1:]:
+        line = line.strip()
+        if line.startswith('- '):
+          # New volume type. e.g.:
+          # - STREAM_VOICE_CALL:
+          #   Muted: false
+          #   Muted Internally: false
+          #   Min: 1
+          #   Max: 7
+          #   streamVolume:5
+          #   Current: 1 (earpiece): 5, 80 (bt_a2dp): 5, 40000000 (default): 5
+          #   Devices: earpiece(1)
+          #   Volume Group: AUDIO_STREAM_VOICE_CALL
+          mth = stream_header_pattern.search(line)
+          if not mth:
+            raise ValueError(f'Unknown stream header title: {line}')
+          current_volume_setting_record = (
+              general_data.AudioStreamVolume(name=mth.group(1)))
+        elif line.startswith('Muted:'):
+          current_volume_setting_record.is_muted = (
+              False if line.split(':')[1].strip() == 'false' else True)
+        elif line.startswith('Min:'):
+          try:
+            current_volume_setting_record.min_level = (
+                int(line.split(':')[1].strip().split()[0]))
+          except ValueError as ex:
+            logging.warning(
+                f'Unknown Min setting="{line}"! Use default 0 instead: {ex}')
+            current_volume_setting_record.min_level = 0
+        elif line.startswith('Max:'):
+          current_volume_setting_record.max_level = (
+              int(line.split(':')[1].strip()))
+        elif line.startswith('streamVolume:'):
+          current_volume_setting_record.stream_volume_level = (
+              int(line.split(':')[1].strip()))
+        elif line.startswith('Devices:'):
+          current_volume_setting_record.devices = line.split(':')[1].strip()
+        elif line.startswith('Current:'):
+          current_volume_setting_record.current = (
+              int(line.split(':')[1].strip().split()[0]))
+        elif line == '':
+          if current_volume_setting_record is None:
+            break
+
+          # Save the parsing record
+          collected_volume_info[current_volume_setting_record.name] = (
+              current_volume_setting_record)
+          current_volume_setting_record = None
+
+  return collected_volume_info
+
+
 def parse_bluetooth_crash_info(log_content: str) -> Sequence[str]:
   """Parses the BT manager log to collect crash information.
 
   For this function to work, we expect below log snippet from given log content:
 
   ===
   Bluetooth crashed 2 times
```

### Comparing `bttc-0.0.76/bttc/utils/logcat.py` & `bttc-0.0.77/bttc/utils/logcat.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/utils/media_player/media_player_agent_facade.py` & `bttc-0.0.77/bttc/utils/media_player/media_player_agent_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/utils/media_player/yt_player_agent.py` & `bttc-0.0.77/bttc/utils/media_player/yt_player_agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,15 +87,18 @@
     while not (is_done := self.is_main_page()) and retry_count > 0:
       self.log.info('Entering YTM page...retry=%s', retry_count)
       self._ad.adb.shell(f'am start {YT_MUSIC_PACKAGE}')
       retry_count -= 1
       time.sleep(2)
 
     if not is_done:
-      raise Exception('Failed to initialize YTM player agent!')
+      self.uip.refresh()
+      raise Exception(
+          'Failed to initialize YTM player agent:'
+          f'\n{self.uip.parsed_ui.ui_xml.toxml()}\n')
 
     self._ad.ui(
         textMatches='Device files only|DEVICE FILES ONLY').click.wait(10)
     self._ad.ui(textMatches='Allow|ALLOW').click.wait(10)
 
   def free(self):
     """Frees the media player agent resource."""
@@ -111,39 +114,43 @@
     """Plays media."""
     if self.is_main_page():
       self.log.info('Random select music to play...')
       self.uip.refresh()
       nodes = self.uip.get_all_nodes_by_attrs({'NAF': 'true'}, from_all=True)
       if len(nodes) < 3:
         raise Exception(
-            f'Unexpected UI page content:\n{self.uip.parsed_ui.ui_xml}\n')
+            f'Unexpected UI page content:\n'
+            f'{self.uip.parsed_ui.ui_xml.toxml()}\n')
       self.uip.click(nodes[2])
     elif self.is_play_page():
       self.log.info('Under play page and continue playing...')
       self._ad.mc.play()
 
     self._wait_playback_state(PlaybackState.PLAYING)
     self.uip.refresh()
 
   def pause(self):
     """Pauses media."""
     if not self.is_play_page():
-      raise Exception(f'Not in playing page:\n{self.uip.parsed_ui.ui_xml}\n')
+      raise Exception(
+          f'Not in playing page:\n{self.uip.parsed_ui.ui_xml.toxml()}\n')
     self._ad.mc.pause()
     self._wait_playback_state(PlaybackState.PAUSED)
     self.uip.refresh()
 
   def next_track(self):
     """Goes to next track."""
     if not self.is_play_page():
-      raise Exception(f'Not in playing page:\n{self.uip.parsed_ui.ui_xml}\n')
+      raise Exception(
+          f'Not in playing page:\n{self.uip.parsed_ui.ui_xml.toxml()}\n')
     self._ad.mc.next()
     self._wait_playback_state(PlaybackState.PLAYING)
     self.uip.refresh()
 
   def previous_track(self):
     """Goes to previous track."""
     if not self.is_play_page():
-      raise Exception(f'Not in playing page:\n{self.uip.parsed_ui.ui_xml}\n')
+      raise Exception(
+          f'Not in playing page:\n{self.uip.parsed_ui.ui_xml.toxml()}\n')
     self._ad.mc.previous()
     self._wait_playback_state(PlaybackState.PLAYING)
     self.uip.refresh()
```

### Comparing `bttc-0.0.76/bttc/utils/retry.py` & `bttc-0.0.77/bttc/utils/retry.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/utils/typing_utils.py` & `bttc-0.0.77/bttc/utils/typing_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/utils/ui_pages/__init__.py` & `bttc-0.0.77/bttc/utils/ui_pages/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/utils/ui_pages/errors.py` & `bttc-0.0.77/bttc/utils/ui_pages/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/utils/ui_pages/ui_core.py` & `bttc-0.0.77/bttc/utils/ui_pages/ui_core.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/utils/ui_pages/ui_node.py` & `bttc-0.0.77/bttc/utils/ui_pages/ui_node.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/utils/ui_pages/utils.py` & `bttc-0.0.77/bttc/utils/ui_pages/utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/utils_loader.py` & `bttc-0.0.77/bttc/utils_loader.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc/wifi_utils.py` & `bttc-0.0.77/bttc/wifi_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/bttc.egg-info/PKG-INFO` & `bttc-0.0.77/bttc.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bttc
-Version: 0.0.76
+Version: 0.0.77
 Summary: A package to provide common utilities for BT testing.
 Home-page: https://github.com/johnklee/bt_test_common
 Author: John Lee/Yuan Long Luo/Denny Chai
 Author-email: puremonkey2007@gmail.com
 License: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -61,14 +61,15 @@
 >>> import bttc
 >>> dut = bttc.get('07311JECB08252', {'wifi'})
 >>> dut.wifi.status()
 <WifiStatus.ENABLED: 'enabled'>
 ```
 
 ## Release info
+* Release v0.0.77: #202
 * Release v0.0.76: #198, #196, #194, #192
 * Release v0.0.75: #64
 * Release v0.0.74: #125, #159, #171, #173, #176, #178, #180
 * Release v0.0.73: #158, #163
 * Release v0.0.72: #153, #155, #51, #157
 * Release v0.0.71: #123, #134, #140
 * Release v0.0.70: #128, #132, #135
```

### Comparing `bttc-0.0.76/bttc.egg-info/SOURCES.txt` & `bttc-0.0.77/bttc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bttc-0.0.76/setup.py` & `bttc-0.0.77/setup.py`

 * *Files identical despite different names*

