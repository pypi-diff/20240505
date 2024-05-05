# Comparing `tmp/bttc-0.0.77.tar.gz` & `tmp/bttc-0.0.77.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bttc-0.0.77.tar", last modified: Sun May  5 01:23:20 2024, max compression
+gzip compressed data, was "bttc-0.0.77.1.tar", last modified: Sun May  5 01:34:13 2024, max compression
```

## Comparing `bttc-0.0.77.tar` & `bttc-0.0.77.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:23:20.940626 bttc-0.0.77/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1061 2023-08-09 04:39:34.000000 bttc-0.0.77/LICENSE
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2158 2024-05-05 01:23:20.940626 bttc-0.0.77/PKG-INFO
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1430 2024-05-05 01:23:10.000000 bttc-0.0.77/README.md
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:23:20.932626 bttc-0.0.77/bttc/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6836 2024-05-05 01:22:46.000000 bttc-0.0.77/bttc/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     9617 2024-04-15 06:13:29.000000 bttc-0.0.77/bttc/apk_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2389 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/ble_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     4752 2024-04-08 13:33:17.000000 bttc-0.0.77/bttc/ble_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1723 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/bt_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    16481 2024-04-28 06:22:01.000000 bttc-0.0.77/bttc/bt_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:23:20.936626 bttc-0.0.77/bttc/cli/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2100 2024-04-10 06:01:48.000000 bttc-0.0.77/bttc/cli/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1150 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/cli/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    22596 2024-04-15 06:24:35.000000 bttc-0.0.77/bttc/cli/main.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      976 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/common_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3956 2024-04-28 06:22:01.000000 bttc-0.0.77/bttc/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1351 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/core.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2199 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     4211 2024-05-05 01:21:12.000000 bttc-0.0.77/bttc/general_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    35298 2024-05-05 01:21:12.000000 bttc-0.0.77/bttc/general_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1062 2024-04-28 06:22:01.000000 bttc-0.0.77/bttc/mc_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5053 2024-04-28 06:22:01.000000 bttc-0.0.77/bttc/mc_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:23:20.936626 bttc-0.0.77/bttc/mobly_android_device_lib/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    13864 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/mobly_android_device_lib/jsonrpc_client_base.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:23:20.936626 bttc-0.0.77/bttc/mobly_android_device_lib/services/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6408 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/mobly_android_device_lib/services/sl4a_client.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2295 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/mobly_android_device_lib/services/sl4a_service.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6095 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/mobly_android_device_lib/tl4a_snippet_client.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:23:20.928626 bttc-0.0.77/bttc/profiles/
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:23:20.936626 bttc-0.0.77/bttc/profiles/avrcp/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/profiles/avrcp/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3189 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/profiles/avrcp/avrcp_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5692 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/profiles/avrcp/avrcp_target_devices.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      915 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/profiles/avrcp/errors.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:23:20.936626 bttc-0.0.77/bttc/profiles/hfp/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1221 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/profiles/hfp/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      962 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/profiles/hfp/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      967 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/profiles/hfp/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1581 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/profiles/hfp/hfp_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     8250 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/profiles/hfp/hfp_devices.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5816 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/profiles/hfp/hfp_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3324 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/profiles/hfp/hfp_strategy.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1567 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/strategy.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:23:20.936626 bttc-0.0.77/bttc/utils/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1868 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/utils/ad_checker.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3932 2024-04-15 06:13:29.000000 bttc-0.0.77/bttc/utils/device_factory.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:23:20.940626 bttc-0.0.77/bttc/utils/iperf/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7860 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/utils/iperf/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      856 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/utils/iperf/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5893 2024-05-05 01:21:12.000000 bttc-0.0.77/bttc/utils/key_events_handler.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    10543 2024-05-05 01:21:12.000000 bttc-0.0.77/bttc/utils/log_parser.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7268 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/utils/logcat.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:23:20.940626 bttc-0.0.77/bttc/utils/media_player/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1227 2024-04-28 06:22:01.000000 bttc-0.0.77/bttc/utils/media_player/media_player_agent_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5138 2024-05-05 01:21:12.000000 bttc-0.0.77/bttc/utils/media_player/yt_player_agent.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    43699 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/utils/retry.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2249 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/utils/typing_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:23:20.940626 bttc-0.0.77/bttc/utils/ui_pages/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3877 2024-04-28 06:22:01.000000 bttc-0.0.77/bttc/utils/ui_pages/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1677 2024-04-29 08:53:55.000000 bttc-0.0.77/bttc/utils/ui_pages/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    16204 2024-04-28 06:22:01.000000 bttc-0.0.77/bttc/utils/ui_pages/ui_core.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7585 2024-04-28 06:22:01.000000 bttc-0.0.77/bttc/utils/ui_pages/ui_node.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2320 2024-04-28 06:22:01.000000 bttc-0.0.77/bttc/utils/ui_pages/utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2960 2024-04-28 06:22:01.000000 bttc-0.0.77/bttc/utils_loader.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5098 2024-03-30 03:00:32.000000 bttc-0.0.77/bttc/wifi_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:23:20.932626 bttc-0.0.77/bttc.egg-info/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2158 2024-05-05 01:23:20.000000 bttc-0.0.77/bttc.egg-info/PKG-INFO
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1587 2024-05-05 01:23:20.000000 bttc-0.0.77/bttc.egg-info/SOURCES.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)        1 2024-05-05 01:23:20.000000 bttc-0.0.77/bttc.egg-info/dependency_links.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      185 2024-05-05 01:23:20.000000 bttc-0.0.77/bttc.egg-info/requires.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)        5 2024-05-05 01:23:20.000000 bttc-0.0.77/bttc.egg-info/top_level.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)       38 2024-05-05 01:23:20.940626 bttc-0.0.77/setup.cfg
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1772 2024-04-28 06:22:01.000000 bttc-0.0.77/setup.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:34:13.226623 bttc-0.0.77.1/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1061 2023-08-09 04:39:34.000000 bttc-0.0.77.1/LICENSE
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2160 2024-05-05 01:34:13.226623 bttc-0.0.77.1/PKG-INFO
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1430 2024-05-05 01:26:33.000000 bttc-0.0.77.1/README.md
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:34:13.218623 bttc-0.0.77.1/bttc/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6838 2024-05-05 01:34:00.000000 bttc-0.0.77.1/bttc/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     9617 2024-04-15 06:13:29.000000 bttc-0.0.77.1/bttc/apk_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2389 2024-03-30 03:00:32.000000 bttc-0.0.77.1/bttc/ble_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     4752 2024-04-08 13:33:17.000000 bttc-0.0.77.1/bttc/ble_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1723 2024-03-30 03:00:32.000000 bttc-0.0.77.1/bttc/bt_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    16481 2024-04-28 06:22:01.000000 bttc-0.0.77.1/bttc/bt_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:34:13.222623 bttc-0.0.77.1/bttc/cli/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2100 2024-04-10 06:01:48.000000 bttc-0.0.77.1/bttc/cli/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1150 2024-03-30 03:00:32.000000 bttc-0.0.77.1/bttc/cli/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    22596 2024-04-15 06:24:35.000000 bttc-0.0.77.1/bttc/cli/main.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      976 2024-03-30 03:00:32.000000 bttc-0.0.77.1/bttc/common_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3956 2024-04-28 06:22:01.000000 bttc-0.0.77.1/bttc/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1351 2024-03-30 03:00:32.000000 bttc-0.0.77.1/bttc/core.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2199 2024-03-30 03:00:32.000000 bttc-0.0.77.1/bttc/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     4211 2024-05-05 01:21:12.000000 bttc-0.0.77.1/bttc/general_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    35298 2024-05-05 01:21:12.000000 bttc-0.0.77.1/bttc/general_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1062 2024-04-28 06:22:01.000000 bttc-0.0.77.1/bttc/mc_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5053 2024-04-28 06:22:01.000000 bttc-0.0.77.1/bttc/mc_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:34:13.222623 bttc-0.0.77.1/bttc/mobly_android_device_lib/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    13864 2024-03-30 03:00:32.000000 bttc-0.0.77.1/bttc/mobly_android_device_lib/jsonrpc_client_base.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:34:13.222623 bttc-0.0.77.1/bttc/mobly_android_device_lib/services/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6408 2024-03-30 03:00:32.000000 bttc-0.0.77.1/bttc/mobly_android_device_lib/services/sl4a_client.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2295 2024-03-30 03:00:32.000000 bttc-0.0.77.1/bttc/mobly_android_device_lib/services/sl4a_service.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6095 2024-03-30 03:00:32.000000 bttc-0.0.77.1/bttc/mobly_android_device_lib/tl4a_snippet_client.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:34:13.210623 bttc-0.0.77.1/bttc/profiles/
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:34:13.222623 bttc-0.0.77.1/bttc/profiles/avrcp/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-03-30 03:00:32.000000 bttc-0.0.77.1/bttc/profiles/avrcp/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3189 2024-03-30 03:00:32.000000 bttc-0.0.77.1/bttc/profiles/avrcp/avrcp_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5692 2024-03-30 03:00:32.000000 bttc-0.0.77.1/bttc/profiles/avrcp/avrcp_target_devices.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      915 2024-03-30 03:00:32.000000 bttc-0.0.77.1/bttc/profiles/avrcp/errors.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:34:13.222623 bttc-0.0.77.1/bttc/profiles/hfp/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1221 2024-03-30 03:00:32.000000 bttc-0.0.77.1/bttc/profiles/hfp/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      962 2024-03-30 03:00:32.000000 bttc-0.0.77.1/bttc/profiles/hfp/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      967 2024-03-30 03:00:32.000000 bttc-0.0.77.1/bttc/profiles/hfp/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1581 2024-03-30 03:00:32.000000 bttc-0.0.77.1/bttc/profiles/hfp/hfp_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     8250 2024-03-30 03:00:32.000000 bttc-0.0.77.1/bttc/profiles/hfp/hfp_devices.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5816 2024-03-30 03:00:32.000000 bttc-0.0.77.1/bttc/profiles/hfp/hfp_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3324 2024-03-30 03:00:32.000000 bttc-0.0.77.1/bttc/profiles/hfp/hfp_strategy.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1567 2024-03-30 03:00:32.000000 bttc-0.0.77.1/bttc/strategy.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:34:13.226623 bttc-0.0.77.1/bttc/utils/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1868 2024-03-30 03:00:32.000000 bttc-0.0.77.1/bttc/utils/ad_checker.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3932 2024-04-15 06:13:29.000000 bttc-0.0.77.1/bttc/utils/device_factory.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:34:13.226623 bttc-0.0.77.1/bttc/utils/iperf/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7860 2024-03-30 03:00:32.000000 bttc-0.0.77.1/bttc/utils/iperf/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      856 2024-03-30 03:00:32.000000 bttc-0.0.77.1/bttc/utils/iperf/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5893 2024-05-05 01:21:12.000000 bttc-0.0.77.1/bttc/utils/key_events_handler.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    10543 2024-05-05 01:21:12.000000 bttc-0.0.77.1/bttc/utils/log_parser.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7268 2024-03-30 03:00:32.000000 bttc-0.0.77.1/bttc/utils/logcat.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:34:13.226623 bttc-0.0.77.1/bttc/utils/media_player/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1227 2024-04-28 06:22:01.000000 bttc-0.0.77.1/bttc/utils/media_player/media_player_agent_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5331 2024-05-05 01:33:18.000000 bttc-0.0.77.1/bttc/utils/media_player/yt_player_agent.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    43699 2024-03-30 03:00:32.000000 bttc-0.0.77.1/bttc/utils/retry.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2249 2024-03-30 03:00:32.000000 bttc-0.0.77.1/bttc/utils/typing_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:34:13.226623 bttc-0.0.77.1/bttc/utils/ui_pages/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3877 2024-04-28 06:22:01.000000 bttc-0.0.77.1/bttc/utils/ui_pages/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1677 2024-04-29 08:53:55.000000 bttc-0.0.77.1/bttc/utils/ui_pages/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    16204 2024-04-28 06:22:01.000000 bttc-0.0.77.1/bttc/utils/ui_pages/ui_core.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7585 2024-04-28 06:22:01.000000 bttc-0.0.77.1/bttc/utils/ui_pages/ui_node.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2320 2024-04-28 06:22:01.000000 bttc-0.0.77.1/bttc/utils/ui_pages/utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2960 2024-04-28 06:22:01.000000 bttc-0.0.77.1/bttc/utils_loader.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5098 2024-03-30 03:00:32.000000 bttc-0.0.77.1/bttc/wifi_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:34:13.218623 bttc-0.0.77.1/bttc.egg-info/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2160 2024-05-05 01:34:13.000000 bttc-0.0.77.1/bttc.egg-info/PKG-INFO
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1587 2024-05-05 01:34:13.000000 bttc-0.0.77.1/bttc.egg-info/SOURCES.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)        1 2024-05-05 01:34:13.000000 bttc-0.0.77.1/bttc.egg-info/dependency_links.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      185 2024-05-05 01:34:13.000000 bttc-0.0.77.1/bttc.egg-info/requires.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)        5 2024-05-05 01:34:13.000000 bttc-0.0.77.1/bttc.egg-info/top_level.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)       38 2024-05-05 01:34:13.226623 bttc-0.0.77.1/setup.cfg
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1772 2024-04-28 06:22:01.000000 bttc-0.0.77.1/setup.py
```

### Comparing `bttc-0.0.77/LICENSE` & `bttc-0.0.77.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/PKG-INFO` & `bttc-0.0.77.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bttc
-Version: 0.0.77
+Version: 0.0.77.1
 Summary: A package to provide common utilities for BT testing.
 Home-page: https://github.com/johnklee/bt_test_common
 Author: John Lee/Yuan Long Luo/Denny Chai
 Author-email: puremonkey2007@gmail.com
 License: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bttc-0.0.77/README.md` & `bttc-0.0.77.1/README.md`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/__init__.py` & `bttc-0.0.77.1/bttc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from bttc import utils_loader
 from bttc.utils import device_factory
 from ppadb import client
 import shlex
 from typing import Callable, TypeAlias
 
 
-__version__ = '0.0.77'
+__version__ = '0.0.77.1'
 __author__ = 'John Lee/Yuan Long Luo/Denny Chai'
 __credits__ = 'Google Pixel PQM'
 
 
 GeneralDevice: TypeAlias = android_device.AndroidDevice
```

### Comparing `bttc-0.0.77/bttc/apk_utils.py` & `bttc-0.0.77.1/bttc/apk_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/ble_data.py` & `bttc-0.0.77.1/bttc/ble_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/ble_utils.py` & `bttc-0.0.77.1/bttc/ble_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/bt_data.py` & `bttc-0.0.77.1/bttc/bt_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/bt_utils.py` & `bttc-0.0.77.1/bttc/bt_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/cli/__init__.py` & `bttc-0.0.77.1/bttc/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/cli/constants.py` & `bttc-0.0.77.1/bttc/cli/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/cli/main.py` & `bttc-0.0.77.1/bttc/cli/main.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/common_data.py` & `bttc-0.0.77.1/bttc/common_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/constants.py` & `bttc-0.0.77.1/bttc/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/core.py` & `bttc-0.0.77.1/bttc/core.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/errors.py` & `bttc-0.0.77.1/bttc/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/general_data.py` & `bttc-0.0.77.1/bttc/general_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/general_utils.py` & `bttc-0.0.77.1/bttc/general_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/mc_data.py` & `bttc-0.0.77.1/bttc/mc_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/mc_utils.py` & `bttc-0.0.77.1/bttc/mc_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/mobly_android_device_lib/jsonrpc_client_base.py` & `bttc-0.0.77.1/bttc/mobly_android_device_lib/jsonrpc_client_base.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/mobly_android_device_lib/services/sl4a_client.py` & `bttc-0.0.77.1/bttc/mobly_android_device_lib/services/sl4a_client.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/mobly_android_device_lib/services/sl4a_service.py` & `bttc-0.0.77.1/bttc/mobly_android_device_lib/services/sl4a_service.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/mobly_android_device_lib/tl4a_snippet_client.py` & `bttc-0.0.77.1/bttc/mobly_android_device_lib/tl4a_snippet_client.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/profiles/avrcp/__init__.py` & `bttc-0.0.77.1/bttc/profiles/avrcp/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/profiles/avrcp/avrcp_facade.py` & `bttc-0.0.77.1/bttc/profiles/avrcp/avrcp_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/profiles/avrcp/avrcp_target_devices.py` & `bttc-0.0.77.1/bttc/profiles/avrcp/avrcp_target_devices.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/profiles/avrcp/errors.py` & `bttc-0.0.77.1/bttc/profiles/avrcp/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/profiles/hfp/__init__.py` & `bttc-0.0.77.1/bttc/profiles/hfp/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/profiles/hfp/constants.py` & `bttc-0.0.77.1/bttc/profiles/hfp/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/profiles/hfp/errors.py` & `bttc-0.0.77.1/bttc/profiles/hfp/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/profiles/hfp/hfp_data.py` & `bttc-0.0.77.1/bttc/profiles/hfp/hfp_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/profiles/hfp/hfp_devices.py` & `bttc-0.0.77.1/bttc/profiles/hfp/hfp_devices.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/profiles/hfp/hfp_facade.py` & `bttc-0.0.77.1/bttc/profiles/hfp/hfp_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/profiles/hfp/hfp_strategy.py` & `bttc-0.0.77.1/bttc/profiles/hfp/hfp_strategy.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/strategy.py` & `bttc-0.0.77.1/bttc/strategy.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/utils/ad_checker.py` & `bttc-0.0.77.1/bttc/utils/ad_checker.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/utils/device_factory.py` & `bttc-0.0.77.1/bttc/utils/device_factory.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/utils/iperf/__init__.py` & `bttc-0.0.77.1/bttc/utils/iperf/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/utils/iperf/errors.py` & `bttc-0.0.77.1/bttc/utils/iperf/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/utils/key_events_handler.py` & `bttc-0.0.77.1/bttc/utils/key_events_handler.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/utils/log_parser.py` & `bttc-0.0.77.1/bttc/utils/log_parser.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/utils/logcat.py` & `bttc-0.0.77.1/bttc/utils/logcat.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/utils/media_player/media_player_agent_facade.py` & `bttc-0.0.77.1/bttc/utils/media_player/media_player_agent_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/utils/media_player/yt_player_agent.py` & `bttc-0.0.77.1/bttc/utils/media_player/yt_player_agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,15 +116,22 @@
       self.log.info('Random select music to play...')
       self.uip.refresh()
       nodes = self.uip.get_all_nodes_by_attrs({'NAF': 'true'}, from_all=True)
       if len(nodes) < 3:
         raise Exception(
             f'Unexpected UI page content:\n'
             f'{self.uip.parsed_ui.ui_xml.toxml()}\n')
-      self.uip.click(nodes[2])
+      for ni in range(2, 4):
+        try:
+          self.uip.click(nodes[ni])
+          self._wait_playback_state(PlaybackState.PLAYING)
+          break
+        except Exception:
+          self.uip.back()
+          continue
     elif self.is_play_page():
       self.log.info('Under play page and continue playing...')
       self._ad.mc.play()
 
     self._wait_playback_state(PlaybackState.PLAYING)
     self.uip.refresh()
```

### Comparing `bttc-0.0.77/bttc/utils/retry.py` & `bttc-0.0.77.1/bttc/utils/retry.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/utils/typing_utils.py` & `bttc-0.0.77.1/bttc/utils/typing_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/utils/ui_pages/__init__.py` & `bttc-0.0.77.1/bttc/utils/ui_pages/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/utils/ui_pages/errors.py` & `bttc-0.0.77.1/bttc/utils/ui_pages/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/utils/ui_pages/ui_core.py` & `bttc-0.0.77.1/bttc/utils/ui_pages/ui_core.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/utils/ui_pages/ui_node.py` & `bttc-0.0.77.1/bttc/utils/ui_pages/ui_node.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/utils/ui_pages/utils.py` & `bttc-0.0.77.1/bttc/utils/ui_pages/utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/utils_loader.py` & `bttc-0.0.77.1/bttc/utils_loader.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc/wifi_utils.py` & `bttc-0.0.77.1/bttc/wifi_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/bttc.egg-info/PKG-INFO` & `bttc-0.0.77.1/bttc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bttc
-Version: 0.0.77
+Version: 0.0.77.1
 Summary: A package to provide common utilities for BT testing.
 Home-page: https://github.com/johnklee/bt_test_common
 Author: John Lee/Yuan Long Luo/Denny Chai
 Author-email: puremonkey2007@gmail.com
 License: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bttc-0.0.77/bttc.egg-info/SOURCES.txt` & `bttc-0.0.77.1/bttc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77/setup.py` & `bttc-0.0.77.1/setup.py`

 * *Files identical despite different names*

