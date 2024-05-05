# Comparing `tmp/ableton-control-surface-scripts-0.0.1.tar.gz` & `tmp/ableton-control-surface-scripts-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/sahlen/repositories/oslo1989/ableton-controlsurface-toolkit/ableton-control-surface-scripts/dist/.tmp-fjjokjow/ableton-c", last modified: Sun May  5 12:05:46 2024, max compression
+gzip compressed data, was "/Users/sahlen/repositories/oslo1989/ableton-controlsurface-toolkit/ableton-control-surface-scripts/dist/.tmp-plwc4s_0/ableton-c", last modified: Sun May  5 14:24:02 2024, max compression
```

## Comparing `ableton-control-surface-scripts-0.0.1.tar` & `ableton-control-surface-scripts-0.0.2.tar`

### file list

```diff
@@ -1,1076 +1,1076 @@
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/
--rw-r--r--   0 sahlen     (501) staff       (20)      572 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/PKG-INFO
--rw-r--r--   0 sahlen     (501) staff       (20)      742 2024-05-05 11:53:58.000000 ableton-control-surface-scripts-0.0.1/pyproject.toml
--rw-r--r--   0 sahlen     (501) staff       (20)       38 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/setup.cfg
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/ADVANCE/
--rw-r--r--   0 sahlen     (501) staff       (20)     2650 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/ADVANCE/Advance.py
--rw-r--r--   0 sahlen     (501) staff       (20)      894 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/ADVANCE/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/AIRA_MX_1/
--rw-r--r--   0 sahlen     (501) staff       (20)      802 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/AIRA_MX_1/Colors.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1255 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/AIRA_MX_1/ControlElementUtils.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1322 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/AIRA_MX_1/NotifyingMixerComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4343 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/AIRA_MX_1/NotifyingSessionComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5516 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/AIRA_MX_1/RolandMX1.py
--rw-r--r--   0 sahlen     (501) staff       (20)      910 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/AIRA_MX_1/SkinDefault.py
--rw-r--r--   0 sahlen     (501) staff       (20)      818 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/AIRA_MX_1/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/APC20/
--rw-r--r--   0 sahlen     (501) staff       (20)     7672 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/APC20/APC20.py
--rw-r--r--   0 sahlen     (501) staff       (20)      811 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/APC20/BackgroundComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7676 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/APC20/ShiftableSelectorComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3261 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/APC20/ShiftableZoomingComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2471 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/APC20/SliderModesComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)      839 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/APC20/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)      398 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/APC20/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/APC40/
--rw-r--r--   0 sahlen     (501) staff       (20)    14531 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/APC40/APC40.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1220 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.1/src/APC40/SessionComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1956 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/APC40/TransportComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)      839 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/APC40/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/APC40_MkII/
--rw-r--r--   0 sahlen     (501) staff       (20)    16634 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/APC40_MkII/APC40_MkII.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1093 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.1/src/APC40_MkII/BankToggleComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4045 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/APC40_MkII/Colors.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4257 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/APC40_MkII/MixerComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2005 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/APC40_MkII/QuantizationComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1523 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/APC40_MkII/TransportComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)      942 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/APC40_MkII/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/APC64/
--rw-r--r--   0 sahlen     (501) staff       (20)     3917 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/APC64/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3962 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/APC64/colors.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3327 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/APC64/device.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3857 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/APC64/display.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5996 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/APC64/elements.py
--rw-r--r--   0 sahlen     (501) staff       (20)      958 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/APC64/firmware_mode.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1649 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/APC64/global_quantization.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8182 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/APC64/mappings.py
--rw-r--r--   0 sahlen     (501) staff       (20)      901 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/APC64/midi.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1901 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/APC64/mixer.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1249 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/APC64/recording.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6149 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/APC64/render_to_clip.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2830 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/APC64/session.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3916 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/APC64/settings.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3600 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/APC64/skin.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4299 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/APC64/touch_strip.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1569 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/APC64/transport.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/APC_Key_25/
--rw-r--r--   0 sahlen     (501) staff       (20)    10529 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/APC_Key_25/APC_Key_25.py
--rw-r--r--   0 sahlen     (501) staff       (20)      953 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/APC_Key_25/MixerComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1051 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/APC_Key_25/SendToggleComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)      858 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/APC_Key_25/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/APC_Key_25_mk2/
--rw-r--r--   0 sahlen     (501) staff       (20)     1562 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/APC_Key_25_mk2/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1880 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/APC_Key_25_mk2/colors.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1522 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/APC_Key_25_mk2/elements.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3554 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/APC_Key_25_mk2/mappings.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/APC_mini/
--rw-r--r--   0 sahlen     (501) staff       (20)     1426 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/APC_mini/APC_mini.py
--rw-r--r--   0 sahlen     (501) staff       (20)      848 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/APC_mini/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/APC_mini_mk2/
--rw-r--r--   0 sahlen     (501) staff       (20)     2485 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/APC_mini_mk2/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2291 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/APC_mini_mk2/colors.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1730 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/APC_mini_mk2/elements.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3575 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/APC_mini_mk2/mappings.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/ATOM/
--rw-r--r--   0 sahlen     (501) staff       (20)     2572 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/ATOM/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4483 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/ATOM/colors.py
--rw-r--r--   0 sahlen     (501) staff       (20)      896 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/ATOM/drum_group.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2522 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/ATOM/elements.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1642 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/ATOM/keyboard.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5204 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/ATOM/mappings.py
--rw-r--r--   0 sahlen     (501) staff       (20)      541 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/ATOM/midi.py
--rw-r--r--   0 sahlen     (501) staff       (20)      799 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/ATOM/note_pad.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2662 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/ATOM/skin.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/ATOMSQ/
--rw-r--r--   0 sahlen     (501) staff       (20)     3331 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/ATOMSQ/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4700 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/ATOMSQ/colors.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2636 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/ATOMSQ/display.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4936 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/ATOMSQ/elements.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2228 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/ATOMSQ/launch_and_stop.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4454 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/ATOMSQ/mappings.py
--rw-r--r--   0 sahlen     (501) staff       (20)      782 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/ATOMSQ/midi.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1712 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/ATOMSQ/skin.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1872 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/ATOMSQ/touch_strip.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/
--rw-r--r--   0 sahlen     (501) staff       (20)      853 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)    22171 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/akai_force_mpc.py
--rw-r--r--   0 sahlen     (501) staff       (20)      643 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/background.py
--rw-r--r--   0 sahlen     (501) staff       (20)    16644 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/channel_strip.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2208 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/clip_actions.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4054 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/clip_slot.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2840 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/control.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2737 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/device.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4342 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/device_navigation.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7630 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/device_parameters.py
--rw-r--r--   0 sahlen     (501) staff       (20)    35476 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/elements.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2516 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/live_colors.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4318 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/mixer.py
--rw-r--r--   0 sahlen     (501) staff       (20)      819 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/mode.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1272 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/multi_element.py
--rw-r--r--   0 sahlen     (501) staff       (20)      896 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/physical_display.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1921 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/ping_pong.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3397 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/scene.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1861 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/scene_list.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8367 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/session.py
--rw-r--r--   0 sahlen     (501) staff       (20)      962 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/session_navigation.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1058 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/session_recording.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2322 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/skin.py
--rw-r--r--   0 sahlen     (501) staff       (20)      787 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/sysex.py
--rw-r--r--   0 sahlen     (501) staff       (20)      579 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/sysex_element.py
--rw-r--r--   0 sahlen     (501) staff       (20)    10215 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/transport.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Alesis_V/
--rw-r--r--   0 sahlen     (501) staff       (20)     1483 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Alesis_V/Alesis_V.py
--rw-r--r--   0 sahlen     (501) staff       (20)      862 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Alesis_V/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Alesis_VI/
--rw-r--r--   0 sahlen     (501) staff       (20)     2408 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Alesis_VI/Alesis_VI.py
--rw-r--r--   0 sahlen     (501) staff       (20)      916 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Alesis_VI/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Alesis_VX/
--rw-r--r--   0 sahlen     (501) staff       (20)      416 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/Alesis_VX/Alesis_VX.py
--rw-r--r--   0 sahlen     (501) staff       (20)      842 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Alesis_VX/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Axiom/
--rw-r--r--   0 sahlen     (501) staff       (20)      786 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Axiom/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1519 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Axiom/config.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1872 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Axiom/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/AxiomPro/
--rw-r--r--   0 sahlen     (501) staff       (20)    10734 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/AxiomPro/AxiomPro.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5190 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/AxiomPro/DisplayingMixerComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5192 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/AxiomPro/EncoderMixerModeSelector.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6656 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/AxiomPro/MixerOrDeviceModeSelector.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2842 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/AxiomPro/NotifyingMixerComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)    10420 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/AxiomPro/PageableDeviceComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1390 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/AxiomPro/PeekableEncoderElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3499 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/AxiomPro/SelectButtonModeSelector.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2132 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/AxiomPro/TransportViewModeSelector.py
--rw-r--r--   0 sahlen     (501) staff       (20)      897 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/AxiomPro/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_25_Classic/
--rw-r--r--   0 sahlen     (501) staff       (20)     4762 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_25_Classic/Axiom.py
--rw-r--r--   0 sahlen     (501) staff       (20)      747 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_25_Classic/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_49_61_Classic/
--rw-r--r--   0 sahlen     (501) staff       (20)     4773 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_49_61_Classic/Axiom.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3903 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_49_61_Classic/SliderSection.py
--rw-r--r--   0 sahlen     (501) staff       (20)      449 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_49_61_Classic/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/
--rw-r--r--   0 sahlen     (501) staff       (20)    33436 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/Axiom_AIR_25_49_61.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2323 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/BestBankDeviceComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3465 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/ConfigurableButtonElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2547 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/DeviceNavComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4485 2024-01-08 19:05:13.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/DisplayingChanStripComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3956 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/EncoderModeSelector.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3556 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/FaderButtonModeSelector.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3709 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/FaderModeSelector.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3705 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/IdentifyingEncoderElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3232 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/MainModeSelector.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1844 2024-01-08 19:05:13.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/NumericalDisplayElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1581 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/NumericalDisplaySegment.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2657 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/SingleFaderButtonModeSelector.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1600 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/SpecialMixerComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4415 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/SpecialSessionComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2152 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/TransportViewModeSelector.py
--rw-r--r--   0 sahlen     (501) staff       (20)      973 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2267 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_Mini32/
--rw-r--r--   0 sahlen     (501) staff       (20)     4927 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_Mini32/AxiomAirMini32.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2423 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_Mini32/DeviceNavComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1605 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_Mini32/EncoderMixerModeSelector.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3753 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_Mini32/MixerOrDeviceModeSelector.py
--rw-r--r--   0 sahlen     (501) staff       (20)      948 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_Mini32/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_DirectLink/
--rw-r--r--   0 sahlen     (501) staff       (20)    16087 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_DirectLink/Axiom_DirectLink.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2895 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_DirectLink/BestBankDeviceComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2819 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_DirectLink/DetailViewCntrlComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1398 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_DirectLink/PeekableEncoderElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5865 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_DirectLink/ShiftableMixerComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2592 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_DirectLink/ShiftableSessionComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1747 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_DirectLink/ShiftableTransportComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2140 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_DirectLink/TransportViewModeSelector.py
--rw-r--r--   0 sahlen     (501) staff       (20)      887 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Axiom_DirectLink/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/BCF2000/
--rw-r--r--   0 sahlen     (501) staff       (20)      745 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/BCF2000/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1650 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/BCF2000/config.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1831 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/BCF2000/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/BCR2000/
--rw-r--r--   0 sahlen     (501) staff       (20)     1029 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/BCR2000/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1475 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/BCR2000/config.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1835 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/BCR2000/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/BLOCKS/
--rw-r--r--   0 sahlen     (501) staff       (20)      926 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/BLOCKS/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)    10244 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/BLOCKS/blocks.py
--rw-r--r--   0 sahlen     (501) staff       (20)      688 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/BLOCKS/button.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4628 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/BLOCKS/colors.py
--rw-r--r--   0 sahlen     (501) staff       (20)      957 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/BLOCKS/element_translator.py
--rw-r--r--   0 sahlen     (501) staff       (20)      706 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/BLOCKS/mode.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1410 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/BLOCKS/skin.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2903 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/BLOCKS/target_track_provider.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/BeatStep/
--rw-r--r--   0 sahlen     (501) staff       (20)     7147 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/BeatStep/BeatStep.py
--rw-r--r--   0 sahlen     (501) staff       (20)      810 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/BeatStep/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Blackstar_Live_Logic/
--rw-r--r--   0 sahlen     (501) staff       (20)     1003 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Blackstar_Live_Logic/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1536 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Blackstar_Live_Logic/blackstar_live_logic.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1388 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Blackstar_Live_Logic/clip_util.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1476 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Blackstar_Live_Logic/elements.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3680 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Blackstar_Live_Logic/footswitch_row_control.py
--rw-r--r--   0 sahlen     (501) staff       (20)    11296 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Blackstar_Live_Logic/looper.py
--rw-r--r--   0 sahlen     (501) staff       (20)      567 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Blackstar_Live_Logic/midi.py
--rw-r--r--   0 sahlen     (501) staff       (20)      627 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Blackstar_Live_Logic/skin.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2704 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/Blackstar_Live_Logic/time_display.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4522 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Blackstar_Live_Logic/track_util.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/CTRL49/
--rw-r--r--   0 sahlen     (501) staff       (20)     1088 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/CTRL49/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)      533 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.1/src/CTRL49/ctrl49.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Code_Series/
--rw-r--r--   0 sahlen     (501) staff       (20)     1171 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Code_Series/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4660 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Code_Series/code.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1018 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Code_Series/element_utils.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1484 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Code_Series/mixer_navigation.py
--rw-r--r--   0 sahlen     (501) staff       (20)      879 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Code_Series/skin_default.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/FANTOM/
--rw-r--r--   0 sahlen     (501) staff       (20)     2564 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/FANTOM/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1505 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/FANTOM/colors.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1151 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/FANTOM/control.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4901 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/FANTOM/elements.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2517 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/FANTOM/mappings.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2619 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/FANTOM/mixer.py
--rw-r--r--   0 sahlen     (501) staff       (20)      903 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/FANTOM/scene_name_display.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2089 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/FANTOM/session.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1853 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/FANTOM/simple_display.py
--rw-r--r--   0 sahlen     (501) staff       (20)      861 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/FANTOM/sysex.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2038 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/FANTOM/track_info_display.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1534 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/FANTOM/transport.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Faderport/
--rw-r--r--   0 sahlen     (501) staff       (20)      861 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Faderport/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Faderport_16/
--rw-r--r--   0 sahlen     (501) staff       (20)      865 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Faderport_16/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Faderport_16_XT/
--rw-r--r--   0 sahlen     (501) staff       (20)      970 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Faderport_16_XT/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Faderport_8/
--rw-r--r--   0 sahlen     (501) staff       (20)      863 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Faderport_8/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/FireOne/
--rw-r--r--   0 sahlen     (501) staff       (20)     9332 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/FireOne/FireOne.py
--rw-r--r--   0 sahlen     (501) staff       (20)      443 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/FireOne/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Hammer_88_Pro/
--rw-r--r--   0 sahlen     (501) staff       (20)     1059 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Hammer_88_Pro/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)      448 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/Hammer_88_Pro/hammer_88_pro.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/KONTROL49/
--rw-r--r--   0 sahlen     (501) staff       (20)      747 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/KONTROL49/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2045 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/KONTROL49/config.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1833 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/KONTROL49/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/KeyFadr/
--rw-r--r--   0 sahlen     (501) staff       (20)      541 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/KeyFadr/KeyFadr.py
--rw-r--r--   0 sahlen     (501) staff       (20)      802 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/KeyFadr/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab/
--rw-r--r--   0 sahlen     (501) staff       (20)     1308 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab/DeviceNavigationComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1905 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab/DisplayElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)    10304 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab/KeyLab.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1977 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab/MixerComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)      594 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab/SessionComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)      878 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_88/
--rw-r--r--   0 sahlen     (501) staff       (20)     1070 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_88/KeyLab88.py
--rw-r--r--   0 sahlen     (501) staff       (20)      804 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_88/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential/
--rw-r--r--   0 sahlen     (501) staff       (20)     1114 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1065 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential/arrangement.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1035 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential/channel_strip.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1877 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential/clip_slot.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1658 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential/control_element_utils.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2074 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential/hardware_settings.py
--rw-r--r--   0 sahlen     (501) staff       (20)    10304 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential/keylab_essential.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1596 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential/ringed_encoder.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1059 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential/ringed_mapped_encoder_control.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2998 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential/session.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1532 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential/skin_default.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1855 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential/sysex.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1901 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential/transport.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1360 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential/undo.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1116 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential/view_control.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential_mk3/
--rw-r--r--   0 sahlen     (501) staff       (20)     2982 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential_mk3/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3564 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential_mk3/colors.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1547 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential_mk3/device_bank_toggle.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6251 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential_mk3/display.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6349 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential_mk3/elements.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2117 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential_mk3/mappings.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1747 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential_mk3/midi.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1744 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential_mk3/mixer.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_mkII/
--rw-r--r--   0 sahlen     (501) staff       (20)     1091 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_mkII/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1076 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_mkII/channel_strip.py
--rw-r--r--   0 sahlen     (501) staff       (20)      553 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_mkII/clip_slot.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1000 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_mkII/hardware_settings.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7663 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_mkII/keylab_mkii.py
--rw-r--r--   0 sahlen     (501) staff       (20)      811 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_mkII/mixer.py
--rw-r--r--   0 sahlen     (501) staff       (20)      728 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_mkII/session.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1384 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/KeyLab_mkII/view_control.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/KeyPad/
--rw-r--r--   0 sahlen     (501) staff       (20)     1491 2024-01-08 19:05:13.000000 ableton-control-surface-scripts-0.0.1/src/KeyPad/CombinedButtonsElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2373 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.1/src/KeyPad/CuePointControlComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7695 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/KeyPad/KeyPad.py
--rw-r--r--   0 sahlen     (501) staff       (20)      797 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/KeyPad/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Keystage/
--rw-r--r--   0 sahlen     (501) staff       (20)     2576 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Keystage/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1879 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Keystage/display.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2532 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Keystage/elements.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1041 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Keystage/mappings.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Keystation_Pro_88/
--rw-r--r--   0 sahlen     (501) staff       (20)      778 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Keystation_Pro_88/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1631 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Keystation_Pro_88/config.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1847 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Keystation_Pro_88/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_A/
--rw-r--r--   0 sahlen     (501) staff       (20)      694 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_A/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1518 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_A/komplete_kontrol_a.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1103 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_A/view_control_component.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk2/
--rw-r--r--   0 sahlen     (501) staff       (20)      686 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk2/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3611 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk2/channel_strip_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4299 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk2/komplete_kontrol_s_mk2.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1684 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk2/meter_display_element.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2312 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk2/mixer_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1679 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk2/session_ring_navigation_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2298 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk2/view_control_component.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk3/
--rw-r--r--   0 sahlen     (501) staff       (20)     2937 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk3/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3946 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk3/display.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4646 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk3/elements.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1677 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk3/focus_follow.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1995 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk3/launch_and_stop.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2308 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk3/mappings.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1014 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk3/midi.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1644 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk3/session_navigation.py
--rw-r--r--   0 sahlen     (501) staff       (20)      618 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk3/skin.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1843 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk3/view_control.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/LPD8/
--rw-r--r--   0 sahlen     (501) staff       (20)     1008 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/LPD8/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1465 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/LPD8/config.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1836 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/LPD8/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/LV1_LX1/
--rw-r--r--   0 sahlen     (501) staff       (20)     1195 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/LV1_LX1/LV1_LX1.py
--rw-r--r--   0 sahlen     (501) staff       (20)      443 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.1/src/LV1_LX1/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/LV2_LX2_LC2_LD2/
--rw-r--r--   0 sahlen     (501) staff       (20)    20891 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/LV2_LX2_LC2_LD2/Devices.py
--rw-r--r--   0 sahlen     (501) staff       (20)      929 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/LV2_LX2_LC2_LD2/DevicesXY.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1682 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/LV2_LX2_LC2_LD2/FaderfoxComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)    14782 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/LV2_LX2_LC2_LD2/FaderfoxDeviceController.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8221 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/LV2_LX2_LC2_LD2/FaderfoxHelper.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9182 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/LV2_LX2_LC2_LD2/FaderfoxMixerController.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4628 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/LV2_LX2_LC2_LD2/FaderfoxScript.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8656 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/LV2_LX2_LC2_LD2/FaderfoxTransportController.py
--rw-r--r--   0 sahlen     (501) staff       (20)      684 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/LV2_LX2_LC2_LD2/LV2DeviceController.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6362 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/LV2_LX2_LC2_LD2/LV2MixerController.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5825 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/LV2_LX2_LC2_LD2/LV2TransportController.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1316 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/LV2_LX2_LC2_LD2/LV2_LX2_LC2_LD2.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3029 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/LV2_LX2_LC2_LD2/ParamMap.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1811 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/LV2_LX2_LC2_LD2/Params.py
--rw-r--r--   0 sahlen     (501) staff       (20)      475 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.1/src/LV2_LX2_LC2_LD2/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3397 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/LV2_LX2_LC2_LD2/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Launch_Control/
--rw-r--r--   0 sahlen     (501) staff       (20)      548 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launch_Control/ButtonSysexControl.py
--rw-r--r--   0 sahlen     (501) staff       (20)      668 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.1/src/Launch_Control/Colors.py
--rw-r--r--   0 sahlen     (501) staff       (20)      707 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launch_Control/ConfigurableButtonElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1839 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Launch_Control/DeviceNavigationComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)    11940 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Launch_Control/LaunchControl.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3918 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launch_Control/SpecialMixerComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)      758 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launch_Control/SpecialSessionComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)      638 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launch_Control/Sysex.py
--rw-r--r--   0 sahlen     (501) staff       (20)      824 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launch_Control/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Launch_Control_XL/
--rw-r--r--   0 sahlen     (501) staff       (20)     1162 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/Launch_Control_XL/ButtonElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2847 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Launch_Control_XL/DeviceComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8826 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Launch_Control_XL/LaunchControlXL.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4494 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Launch_Control_XL/MixerComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1165 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launch_Control_XL/SkinDefault.py
--rw-r--r--   0 sahlen     (501) staff       (20)      917 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launch_Control_XL/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey/
--rw-r--r--   0 sahlen     (501) staff       (20)    10443 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey/Launchkey.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4212 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey/SessionNavigationComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2686 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey/SpecialMixerComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1815 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey/TransportViewModeSelector.py
--rw-r--r--   0 sahlen     (501) staff       (20)      917 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1019 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_MK2/
--rw-r--r--   0 sahlen     (501) staff       (20)      741 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_MK2/BackgroundComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5519 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_MK2/Colors.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1302 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_MK2/ControlElementUtils.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3538 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_MK2/DeviceComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)      895 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_MK2/InControlStatusComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)    14504 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_MK2/Launchkey_MK2.py
--rw-r--r--   0 sahlen     (501) staff       (20)      579 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_MK2/MixerComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2878 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_MK2/ModeUtils.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1801 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_MK2/SessionComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1657 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_MK2/Skin.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1047 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_MK2/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)      801 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_MK2/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_MK3/
--rw-r--r--   0 sahlen     (501) staff       (20)     1277 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_MK3/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3573 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_MK3/channel_strip.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1215 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_MK3/clip_actions.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1354 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_MK3/control.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3604 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_MK3/device.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5893 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_MK3/elements.py
--rw-r--r--   0 sahlen     (501) staff       (20)    17250 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_MK3/launchkey_mk3.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1172 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_MK3/midi.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2814 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_MK3/mixer.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1309 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_MK3/notification.py
--rw-r--r--   0 sahlen     (501) staff       (20)      700 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_MK3/rgb_button.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2341 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_MK3/simple_display.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1089 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_MK3/skin.py
--rw-r--r--   0 sahlen     (501) staff       (20)      683 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_MK3/transport.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_Mini/
--rw-r--r--   0 sahlen     (501) staff       (20)     1490 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_Mini/LaunchkeyMini.py
--rw-r--r--   0 sahlen     (501) staff       (20)      916 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_Mini/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_Mini_MK3/
--rw-r--r--   0 sahlen     (501) staff       (20)     1056 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_Mini_MK3/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)      793 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_Mini_MK3/elements.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9392 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_Mini_MK3/launchkey_mini_mk3.py
--rw-r--r--   0 sahlen     (501) staff       (20)      449 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_Mini_MK3/midi.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1024 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_Mini_MK3/skin.py
--rw-r--r--   0 sahlen     (501) staff       (20)      393 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.1/src/Launchkey_Mini_MK3/sysex_ids.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad/
--rw-r--r--   0 sahlen     (501) staff       (20)     2792 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad/ConfigurableButtonElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)    12801 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad/DefChannelStripComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7575 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad/Launchpad.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9692 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad/MainSelectorComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5407 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad/PreciseButtonSliderElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3313 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad/SpecialMixerComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1415 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad/SpecialSessionComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)    11632 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad/SubSelectorComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)      831 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_MK2/
--rw-r--r--   0 sahlen     (501) staff       (20)     1121 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_MK2/BackgroundComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7160 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_MK2/ChannelStripComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5461 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_MK2/Colors.py
--rw-r--r--   0 sahlen     (501) staff       (20)      625 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_MK2/ComponentUtils.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2046 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_MK2/ControlElementUtils.py
--rw-r--r--   0 sahlen     (501) staff       (20)    17088 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_MK2/Launchpad_MK2.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6133 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_MK2/MixerComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3085 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_MK2/ModeUtils.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3032 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_MK2/SessionComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1252 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_MK2/SessionZoomingComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2698 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_MK2/Skin.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2057 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_MK2/SliderElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1588 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_MK2/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)      868 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_MK2/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Mini_MK3/
--rw-r--r--   0 sahlen     (501) staff       (20)     1056 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Mini_MK3/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1433 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Mini_MK3/elements.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5515 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Mini_MK3/launchpad_mini_mk3.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1076 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Mini_MK3/notifying_background.py
--rw-r--r--   0 sahlen     (501) staff       (20)      815 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Mini_MK3/skin.py
--rw-r--r--   0 sahlen     (501) staff       (20)      414 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Mini_MK3/sysex_ids.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/
--rw-r--r--   0 sahlen     (501) staff       (20)     2922 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/ActionsComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1823 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/BackgroundComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5542 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/ClipActionsComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5461 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/Colors.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2643 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/ConfigurableButtonElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1405 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/DeviceNavigationComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)    15830 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/DrumGroupComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2920 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/DrumGroupFinderComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)    45677 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/Launchpad_Pro.py
--rw-r--r--   0 sahlen     (501) staff       (20)      590 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/LedLightingComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2403 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/MultiButtonElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4030 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/SkinDefault.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3774 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/SlideComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2326 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/SliderElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1108 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/SpecialDeviceComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3412 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/SpecialMidiMap.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6818 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/SpecialMixerComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2109 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/SpecialModesComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)    14385 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/SpecialSessionComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2654 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/SpecialSessionRecordingComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2730 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/TargetTrackComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1449 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/TranslationComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)      729 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/UserMatrixComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)      995 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2048 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro_MK3/
--rw-r--r--   0 sahlen     (501) staff       (20)     1112 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro_MK3/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1050 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro_MK3/channel_strip.py
--rw-r--r--   0 sahlen     (501) staff       (20)      632 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro_MK3/control.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3064 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro_MK3/drum_group.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7058 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro_MK3/elements.py
--rw-r--r--   0 sahlen     (501) staff       (20)    19941 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro_MK3/launchpad_pro_mk3.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3239 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro_MK3/mixer.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4119 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro_MK3/session.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1960 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro_MK3/simple_device.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1376 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro_MK3/skin.py
--rw-r--r--   0 sahlen     (501) staff       (20)      578 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro_MK3/sysex_ids.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1006 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro_MK3/transport.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_X/
--rw-r--r--   0 sahlen     (501) staff       (20)     1021 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_X/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1162 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_X/channel_strip.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3026 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_X/elements.py
--rw-r--r--   0 sahlen     (501) staff       (20)    11925 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_X/launchpad_x.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1935 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_X/session_recording.py
--rw-r--r--   0 sahlen     (501) staff       (20)      885 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_X/skin.py
--rw-r--r--   0 sahlen     (501) staff       (20)      392 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/Launchpad_X/sysex_ids.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/MIDI_Mix/
--rw-r--r--   0 sahlen     (501) staff       (20)     1227 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/MIDI_Mix/ControlElementUtils.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3655 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/MIDI_Mix/MIDI_Mix.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1440 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MIDI_Mix/MixerComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)      801 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MIDI_Mix/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/MPD18/
--rw-r--r--   0 sahlen     (501) staff       (20)      765 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/MPD18/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2015 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MPD18/config.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1837 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MPD18/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/MPD218/
--rw-r--r--   0 sahlen     (501) staff       (20)      602 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MPD218/MPD218.py
--rw-r--r--   0 sahlen     (501) staff       (20)      817 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MPD218/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/MPD226/
--rw-r--r--   0 sahlen     (501) staff       (20)     2065 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/MPD226/MPD226.py
--rw-r--r--   0 sahlen     (501) staff       (20)      817 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MPD226/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/MPD232/
--rw-r--r--   0 sahlen     (501) staff       (20)     1789 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/MPD232/MPD232.py
--rw-r--r--   0 sahlen     (501) staff       (20)      817 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MPD232/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/MPD24/
--rw-r--r--   0 sahlen     (501) staff       (20)     1157 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/MPD24/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1853 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/MPD24/config.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1835 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/MPD24/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/MPD32/
--rw-r--r--   0 sahlen     (501) staff       (20)     1180 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/MPD32/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2046 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MPD32/config.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1842 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MPD32/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/MPK225/
--rw-r--r--   0 sahlen     (501) staff       (20)     2484 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MPK225/MPK225.py
--rw-r--r--   0 sahlen     (501) staff       (20)      838 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MPK225/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/MPK249/
--rw-r--r--   0 sahlen     (501) staff       (20)     2922 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MPK249/MPK249.py
--rw-r--r--   0 sahlen     (501) staff       (20)      838 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MPK249/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/MPK25/
--rw-r--r--   0 sahlen     (501) staff       (20)     1186 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/MPK25/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1959 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/MPK25/config.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1842 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/MPK25/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/MPK261/
--rw-r--r--   0 sahlen     (501) staff       (20)     2922 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MPK261/MPK261.py
--rw-r--r--   0 sahlen     (501) staff       (20)      838 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MPK261/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/MPK49/
--rw-r--r--   0 sahlen     (501) staff       (20)     1206 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/MPK49/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1970 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/MPK49/config.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1842 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MPK49/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/MPK61/
--rw-r--r--   0 sahlen     (501) staff       (20)      765 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/MPK61/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2046 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MPK61/config.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1842 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MPK61/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/MPK88/
--rw-r--r--   0 sahlen     (501) staff       (20)      765 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/MPK88/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2046 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MPK88/config.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1842 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MPK88/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/MPK_mini_mkI/
--rw-r--r--   0 sahlen     (501) staff       (20)     1020 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/MPK_mini_mkI/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1653 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MPK_mini_mkI/config.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1852 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MPK_mini_mkI/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/MPK_mini_mkII/
--rw-r--r--   0 sahlen     (501) staff       (20)     1022 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/MPK_mini_mkII/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1654 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MPK_mini_mkII/config.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1853 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MPK_mini_mkII/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/MPK_mini_mkIII/
--rw-r--r--   0 sahlen     (501) staff       (20)     1023 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/MPK_mini_mkIII/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1655 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MPK_mini_mkIII/config.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1846 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MPK_mini_mkIII/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/MackieControl/
--rw-r--r--   0 sahlen     (501) staff       (20)    20059 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/MackieControl/ChannelStrip.py
--rw-r--r--   0 sahlen     (501) staff       (20)    51253 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/MackieControl/ChannelStripController.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9648 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MackieControl/MackieControl.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1626 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MackieControl/MackieControlComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2113 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MackieControl/MainDisplay.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8600 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/MackieControl/MainDisplayController.py
--rw-r--r--   0 sahlen     (501) staff       (20)    12013 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MackieControl/SoftwareController.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2884 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MackieControl/TimeDisplay.py
--rw-r--r--   0 sahlen     (501) staff       (20)    23493 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/MackieControl/Transport.py
--rw-r--r--   0 sahlen     (501) staff       (20)      962 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MackieControl/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5917 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MackieControl/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/MackieControlXT/
--rw-r--r--   0 sahlen     (501) staff       (20)     6055 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/MackieControlXT/MackieControlXT.py
--rw-r--r--   0 sahlen     (501) staff       (20)      475 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/MackieControlXT/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/MackieControl_Classic/
--rw-r--r--   0 sahlen     (501) staff       (20)    19836 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/MackieControl_Classic/ChannelStrip.py
--rw-r--r--   0 sahlen     (501) staff       (20)    50602 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/MackieControl_Classic/ChannelStripController.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9656 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MackieControl_Classic/MackieControl.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1634 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/MackieControl_Classic/MackieControlComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2121 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/MackieControl_Classic/MainDisplay.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8608 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/MackieControl_Classic/MainDisplayController.py
--rw-r--r--   0 sahlen     (501) staff       (20)    12021 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/MackieControl_Classic/SoftwareController.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2892 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/MackieControl_Classic/TimeDisplay.py
--rw-r--r--   0 sahlen     (501) staff       (20)    23501 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/MackieControl_Classic/Transport.py
--rw-r--r--   0 sahlen     (501) staff       (20)      475 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/MackieControl_Classic/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5925 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/MackieControl_Classic/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/MasterControl/
--rw-r--r--   0 sahlen     (501) staff       (20)      522 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/MasterControl/MasterControl.py
--rw-r--r--   0 sahlen     (501) staff       (20)      467 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/MasterControl/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/MaxForLive/
--rw-r--r--   0 sahlen     (501) staff       (20)      837 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/MaxForLive/MaxForLive.py
--rw-r--r--   0 sahlen     (501) staff       (20)      602 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/MaxForLive/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/MidAir25/
--rw-r--r--   0 sahlen     (501) staff       (20)      745 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/MidAir25/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1251 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/MidAir25/config.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1838 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/MidAir25/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/MiniLab/
--rw-r--r--   0 sahlen     (501) staff       (20)     6446 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/MiniLab/MiniLab.py
--rw-r--r--   0 sahlen     (501) staff       (20)      805 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/MiniLab/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/MiniLab_3/
--rw-r--r--   0 sahlen     (501) staff       (20)     2587 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MiniLab_3/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3702 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/MiniLab_3/analog_lab.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2553 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MiniLab_3/colors.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4151 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/MiniLab_3/display.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2638 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MiniLab_3/display_util.py
--rw-r--r--   0 sahlen     (501) staff       (20)      799 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MiniLab_3/drum_group.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2547 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/MiniLab_3/elements.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2584 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MiniLab_3/encoder.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2823 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/MiniLab_3/mappings.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1604 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MiniLab_3/midi.py
--rw-r--r--   0 sahlen     (501) staff       (20)      733 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MiniLab_3/sysex.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1704 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/MiniLab_3/transport.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/MiniLab_mkII/
--rw-r--r--   0 sahlen     (501) staff       (20)     1449 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MiniLab_mkII/HardwareSettingsComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4149 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/MiniLab_mkII/MiniLabMk2.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2546 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/MiniLab_mkII/SessionComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)      882 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/MiniLab_mkII/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Novation_Impulse/
--rw-r--r--   0 sahlen     (501) staff       (20)     4893 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Novation_Impulse/EncoderModeSelector.py
--rw-r--r--   0 sahlen     (501) staff       (20)    15697 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Novation_Impulse/Novation_Impulse.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1398 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Novation_Impulse/PeekableEncoderElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1747 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Novation_Impulse/ShiftableTransportComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5862 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Novation_Impulse/SpecialMixerComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2140 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Novation_Impulse/TransportViewModeSelector.py
--rw-r--r--   0 sahlen     (501) staff       (20)      852 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Novation_Impulse/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/O2/
--rw-r--r--   0 sahlen     (501) staff       (20)      762 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/O2/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1401 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/O2/config.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1833 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/O2/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/OpenLabs/
--rw-r--r--   0 sahlen     (501) staff       (20)     4589 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/OpenLabs/OpenLabs.py
--rw-r--r--   0 sahlen     (501) staff       (20)      600 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/OpenLabs/SpecialDeviceComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2978 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/OpenLabs/SpecialTransportComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)      447 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.1/src/OpenLabs/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen49_61/
--rw-r--r--   0 sahlen     (501) staff       (20)      771 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen49_61/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1418 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen49_61/config.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1876 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen49_61/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen8/
--rw-r--r--   0 sahlen     (501) staff       (20)     1033 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen8/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1433 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen8/config.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1839 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen8/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen8v2/
--rw-r--r--   0 sahlen     (501) staff       (20)      769 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen8v2/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1447 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen8v2/config.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1839 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen8v2/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen_3rd_Gen/
--rw-r--r--   0 sahlen     (501) staff       (20)     4773 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen_3rd_Gen/Oxygen_3rd_Gen.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3031 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen_3rd_Gen/SpecialMixerComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2138 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen_3rd_Gen/TransportViewModeSelector.py
--rw-r--r--   0 sahlen     (501) staff       (20)      471 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen_3rd_Gen/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen_4th_Gen/
--rw-r--r--   0 sahlen     (501) staff       (20)      470 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen_4th_Gen/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen_5th_Gen/
--rw-r--r--   0 sahlen     (501) staff       (20)     1088 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen_5th_Gen/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)      763 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen_5th_Gen/oxygen_5th_gen.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen_Pro/
--rw-r--r--   0 sahlen     (501) staff       (20)     1136 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen_Pro/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)      552 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen_Pro/channel_strip.py
--rw-r--r--   0 sahlen     (501) staff       (20)      609 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen_Pro/colors.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5630 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen_Pro/elements.py
--rw-r--r--   0 sahlen     (501) staff       (20)      760 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen_Pro/midi.py
--rw-r--r--   0 sahlen     (501) staff       (20)      783 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen_Pro/mode.py
--rw-r--r--   0 sahlen     (501) staff       (20)    10948 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen_Pro/oxygen_pro.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1140 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen_Pro/session.py
--rw-r--r--   0 sahlen     (501) staff       (20)      956 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen_Pro/session_navigation.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1300 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen_Pro/skin.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen_Pro_Mini/
--rw-r--r--   0 sahlen     (501) staff       (20)     1071 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen_Pro_Mini/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)      902 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen_Pro_Mini/oxygen_pro_mini.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1167 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Oxygen_Pro_Mini/simple_device.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Ozone/
--rw-r--r--   0 sahlen     (501) staff       (20)     1004 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Ozone/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1603 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Ozone/config.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1836 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Ozone/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Ozonic/
--rw-r--r--   0 sahlen     (501) staff       (20)      766 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Ozonic/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1427 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Ozonic/config.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1870 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Ozonic/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Photon_25/
--rw-r--r--   0 sahlen     (501) staff       (20)      747 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Photon_25/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1616 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Photon_25/config.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1840 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Photon_25/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Photon_X25/
--rw-r--r--   0 sahlen     (501) staff       (20)      748 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Photon_X25/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1657 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Photon_X25/config.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1850 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Photon_X25/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/ProjectMixIO/
--rw-r--r--   0 sahlen     (501) staff       (20)     7079 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/ProjectMixIO/ProjectMixIO.py
--rw-r--r--   0 sahlen     (501) staff       (20)      463 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/ProjectMixIO/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Push/
--rw-r--r--   0 sahlen     (501) staff       (20)     1208 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Push/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5872 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Push/actions.py
--rw-r--r--   0 sahlen     (501) staff       (20)    18060 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Push/browser_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8865 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Push/browser_model.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4188 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push/browser_model_factory.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3480 2024-01-08 19:12:03.000000 ableton-control-surface-scripts-0.0.1/src/Push/browser_query.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1885 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Push/device_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)    11719 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Push/device_navigation_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)      708 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Push/drum_group_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3503 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push/elements.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1488 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Push/firmware_handling.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1489 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/Push/global_pad_parameters.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6086 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Push/handshake_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4281 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Push/mode_behaviours.py
--rw-r--r--   0 sahlen     (501) staff       (20)      921 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Push/multi_entry_mode.py
--rw-r--r--   0 sahlen     (501) staff       (20)    20813 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Push/navigation_node.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6723 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push/notification_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1187 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Push/pad_sensitivity.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7684 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Push/parameter_mapping_sensitivities.py
--rw-r--r--   0 sahlen     (501) staff       (20)    38899 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push/push.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3180 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Push/quantization_settings.py
--rw-r--r--   0 sahlen     (501) staff       (20)    17028 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push/scales_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1083 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Push/selected_track_parameter_provider.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3654 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push/settings.py
--rw-r--r--   0 sahlen     (501) staff       (20)    13146 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Push/special_chan_strip_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6358 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Push/special_mixer_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3244 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Push/special_physical_display.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3508 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Push/sysex.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5029 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/Push/user_settings_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)      821 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Push/with_priority.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Push2/
--rw-r--r--   0 sahlen     (501) staff       (20)     1261 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/Push2/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1981 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/actions.py
--rw-r--r--   0 sahlen     (501) staff       (20)      692 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Push2/amp.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4696 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/analog.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3266 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Push2/auto_filter.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5304 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Push2/automation.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6736 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/bank_selection_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)      937 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Push2/beatrepeat.py
--rw-r--r--   0 sahlen     (501) staff       (20)    39626 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Push2/browser_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2254 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Push2/browser_item.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3614 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Push2/browser_list.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4502 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Push2/browser_modes.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3796 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/cccontrol.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3253 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/chain_selection_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2440 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Push2/channel_eq.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3873 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/chorus2.py
--rw-r--r--   0 sahlen     (501) staff       (20)    41212 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Push2/clip_control.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8008 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/clip_decoration.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2398 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/collision.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3456 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/color_chooser.py
--rw-r--r--   0 sahlen     (501) staff       (20)    13616 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Push2/colors.py
--rw-r--r--   0 sahlen     (501) staff       (20)    11092 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/compressor.py
--rw-r--r--   0 sahlen     (501) staff       (20)    19234 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Push2/convert.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3552 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/corpus.py
--rw-r--r--   0 sahlen     (501) staff       (20)   401313 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/Push2/custom_bank_definitions.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2784 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Push2/decoration.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4555 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/delay.py
--rw-r--r--   0 sahlen     (501) staff       (20)    10563 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Push2/device_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8166 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Push2/device_component_provider.py
--rw-r--r--   0 sahlen     (501) staff       (20)    15784 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/device_decoration.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3829 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Push2/device_decorator_factory.py
--rw-r--r--   0 sahlen     (501) staff       (20)    24545 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Push2/device_navigation.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4871 2024-01-08 19:12:03.000000 ableton-control-surface-scripts-0.0.1/src/Push2/device_options.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1972 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Push2/device_parameter_bank_with_options.py
--rw-r--r--   0 sahlen     (501) staff       (20)    38924 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/Push2/device_parameter_icons.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1042 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Push2/device_util.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5171 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/device_view_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)    12828 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Push2/drift.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9421 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/drum_group_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6164 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Push2/drum_pad_parameter_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1083 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/drumcell.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9946 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/echo.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2930 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/elements.py
--rw-r--r--   0 sahlen     (501) staff       (20)      892 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Push2/eq3.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4824 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/eq8.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1511 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Push2/filterdelay.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6557 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Push2/firmware.py
--rw-r--r--   0 sahlen     (501) staff       (20)      702 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Push2/graindelay.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3771 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Push2/hardware_settings_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)    20626 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Push2/hybrid_reverb.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1482 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Push2/item_lister.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1723 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/Push2/master_track.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9928 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/meld.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1172 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Push2/mixable_utilities.py
--rw-r--r--   0 sahlen     (501) staff       (20)    11977 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Push2/mixer_control_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1919 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Push2/mode_collector.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Push2/model/
--rw-r--r--   0 sahlen     (501) staff       (20)    24525 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Push2/model/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6885 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Push2/model/declaration.py
--rw-r--r--   0 sahlen     (501) staff       (20)    18509 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/model/generation.py
--rw-r--r--   0 sahlen     (501) staff       (20)    23935 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/model/repr.py
--rw-r--r--   0 sahlen     (501) staff       (20)      534 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/Push2/model/uniqueid.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9819 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/Push2/mute_solo_stop.py
--rw-r--r--   0 sahlen     (501) staff       (20)      677 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Push2/note_editor.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5115 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Push2/note_settings.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2868 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Push2/notification_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9254 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/operator.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1231 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Push2/pad_sensitivity.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5870 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/Push2/pad_velocity_curve.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7585 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Push2/parameter_mapping_sensitivities.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1632 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/phasernew.py
--rw-r--r--   0 sahlen     (501) staff       (20)    61958 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Push2/push2.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2836 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Push2/push2_model.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2721 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/real_time_channel.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1045 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/redux2.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1421 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/resonator.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2555 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/reverb.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6687 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/roar.py
--rw-r--r--   0 sahlen     (501) staff       (20)    36539 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Push2/routing.py
--rw-r--r--   0 sahlen     (501) staff       (20)      765 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Push2/saturator.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7512 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Push2/scales_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1084 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Push2/selected_track_parameter_provider.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5083 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Push2/session_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)      618 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Push2/session_ring_selection_linking.py
--rw-r--r--   0 sahlen     (501) staff       (20)      899 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/settings.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9356 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/setup_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6220 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Push2/shifter.py
--rw-r--r--   0 sahlen     (501) staff       (20)      888 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Push2/simple_mode_switcher.py
--rw-r--r--   0 sahlen     (501) staff       (20)    20015 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/simpler.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7938 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Push2/skin_default.py
--rw-r--r--   0 sahlen     (501) staff       (20)      950 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Push2/sliced_simpler.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1704 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/spectral.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4659 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/sysex.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3302 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/tension.py
--rw-r--r--   0 sahlen     (501) staff       (20)    42336 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Push2/timeline_navigation.py
--rw-r--r--   0 sahlen     (501) staff       (20)    16759 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Push2/track_list.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6702 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/track_mixer_control_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)    11567 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Push2/track_selection.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3925 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Push2/transmute.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2934 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Push2/transport_state.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1801 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Push2/user_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1180 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Push2/vinyl.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3651 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Push2/visualisation_settings.py
--rw-r--r--   0 sahlen     (501) staff       (20)    29969 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Push2/wavetable.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Radium49_61/
--rw-r--r--   0 sahlen     (501) staff       (20)      748 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Radium49_61/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1262 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Radium49_61/config.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1841 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Radium49_61/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/RemoteSL/
--rw-r--r--   0 sahlen     (501) staff       (20)     5232 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/RemoteSL/DisplayController.py
--rw-r--r--   0 sahlen     (501) staff       (20)    15180 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/RemoteSL/EffectController.py
--rw-r--r--   0 sahlen     (501) staff       (20)    22227 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/RemoteSL/MixerController.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6397 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/RemoteSL/RemoteSL.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1414 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/RemoteSL/RemoteSLComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)      844 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/RemoteSL/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3791 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/RemoteSL/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/RemoteSL_Classic/
--rw-r--r--   0 sahlen     (501) staff       (20)     5240 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/RemoteSL_Classic/DisplayController.py
--rw-r--r--   0 sahlen     (501) staff       (20)    14974 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/RemoteSL_Classic/EffectController.py
--rw-r--r--   0 sahlen     (501) staff       (20)    22235 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/RemoteSL_Classic/MixerController.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6405 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/RemoteSL_Classic/RemoteSL.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1422 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/RemoteSL_Classic/RemoteSLComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)      927 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/RemoteSL_Classic/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3799 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/RemoteSL_Classic/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Roland_A_PRO/
--rw-r--r--   0 sahlen     (501) staff       (20)     1314 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Roland_A_PRO/DeviceNavigationComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1514 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/Roland_A_PRO/MixerComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6687 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/Roland_A_PRO/Roland_A_PRO.py
--rw-r--r--   0 sahlen     (501) staff       (20)      996 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Roland_A_PRO/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Roland_FA/
--rw-r--r--   0 sahlen     (501) staff       (20)      947 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Roland_FA/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)      847 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Roland_FA/control_element_utils.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5651 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/Roland_FA/fa.py
--rw-r--r--   0 sahlen     (501) staff       (20)      748 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Roland_FA/navigation.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1515 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Roland_FA/scroll.py
--rw-r--r--   0 sahlen     (501) staff       (20)      757 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/Roland_FA/skin.py
--rw-r--r--   0 sahlen     (501) staff       (20)      718 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/Roland_FA/transport.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/SL_MkIII/
--rw-r--r--   0 sahlen     (501) staff       (20)     1107 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/SL_MkIII/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3802 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/SL_MkIII/actions.py
--rw-r--r--   0 sahlen     (501) staff       (20)      858 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/SL_MkIII/caching_control_element.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6866 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/SL_MkIII/channel_strip.py
--rw-r--r--   0 sahlen     (501) staff       (20)      625 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/SL_MkIII/color_sysex_element.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2226 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/SL_MkIII/control.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2361 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/SL_MkIII/device.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5361 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/SL_MkIII/device_navigation.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2161 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/SL_MkIII/device_parameters.py
--rw-r--r--   0 sahlen     (501) staff       (20)      793 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/SL_MkIII/drum_group.py
--rw-r--r--   0 sahlen     (501) staff       (20)    13516 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/SL_MkIII/elements.py
--rw-r--r--   0 sahlen     (501) staff       (20)      746 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/SL_MkIII/message.py
--rw-r--r--   0 sahlen     (501) staff       (20)      467 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/SL_MkIII/messenger.py
--rw-r--r--   0 sahlen     (501) staff       (20)      935 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/SL_MkIII/midi_message_cache.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6190 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/SL_MkIII/mixer.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4181 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/SL_MkIII/mode.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9543 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/SL_MkIII/parameter_mapping_sensitivities.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1897 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/SL_MkIII/physical_display.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1215 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/SL_MkIII/session.py
--rw-r--r--   0 sahlen     (501) staff       (20)      763 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/SL_MkIII/session_navigation.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3222 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/SL_MkIII/session_ring_selection_linking.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3141 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/SL_MkIII/skin.py
--rw-r--r--   0 sahlen     (501) staff       (20)    28158 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/SL_MkIII/sl_mkiii.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2018 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/SL_MkIII/sysex.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1977 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/SL_MkIII/transport.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1348 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/SL_MkIII/util.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/Tranzport/
--rw-r--r--   0 sahlen     (501) staff       (20)    43921 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/Tranzport/Tranzport.py
--rw-r--r--   0 sahlen     (501) staff       (20)      483 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/Tranzport/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2844 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/Tranzport/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/TriggerFinger/
--rw-r--r--   0 sahlen     (501) staff       (20)      774 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/TriggerFinger/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1796 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/TriggerFinger/config.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1844 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/TriggerFinger/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/UC33e/
--rw-r--r--   0 sahlen     (501) staff       (20)     1072 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/UC33e/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1709 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/UC33e/config.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1829 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/UC33e/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/VCM600/
--rw-r--r--   0 sahlen     (501) staff       (20)     1602 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/VCM600/MixerComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7398 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/VCM600/TrackEQComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3853 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/VCM600/TrackFilterComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)      668 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/VCM600/TransportComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6428 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/VCM600/VCM600.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6605 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/VCM600/ViewTogglerComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)      729 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/VCM600/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/ZERO8/
--rw-r--r--   0 sahlen     (501) staff       (20)      765 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/ZERO8/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1758 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/ZERO8/config.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1837 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/ZERO8/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/_APC/
--rw-r--r--   0 sahlen     (501) staff       (20)     7554 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/_APC/APC.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1594 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/_APC/ControlElementUtils.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4148 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/_APC/DetailViewCntrlComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)      858 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/_APC/DeviceBankButtonElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1669 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/_APC/DeviceComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1830 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/_APC/MixerComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3014 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/_APC/RingedEncoderElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)      752 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/_APC/SessionComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2363 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/_APC/SkinDefault.py
--rw-r--r--   0 sahlen     (501) staff       (20)      345 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/_APC/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/_Arturia/
--rw-r--r--   0 sahlen     (501) staff       (20)     5250 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/_Arturia/ArturiaControlSurface.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2560 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/_Arturia/MixerComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1079 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.1/src/_Arturia/ScrollComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2210 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.1/src/_Arturia/SessionComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)      349 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.1/src/_Arturia/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/_Axiom/
--rw-r--r--   0 sahlen     (501) staff       (20)     8334 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/_Axiom/Encoders.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2092 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/_Axiom/Pads.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4207 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/_Axiom/Transport.py
--rw-r--r--   0 sahlen     (501) staff       (20)      347 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/_Axiom/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2048 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/_Axiom/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/_Komplete_Kontrol/
--rw-r--r--   0 sahlen     (501) staff       (20)      358 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/_Komplete_Kontrol/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4506 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/_Komplete_Kontrol/channel_strip_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1319 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/_Komplete_Kontrol/clip_launch_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1723 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/_Komplete_Kontrol/control_element_util.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2163 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/_Komplete_Kontrol/detail_clip_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2418 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/_Komplete_Kontrol/focus_follow_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)    13732 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/_Komplete_Kontrol/komplete_kontrol_base.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2336 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/_Komplete_Kontrol/mixer_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)      777 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/_Komplete_Kontrol/physical_display_element.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1119 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/_Komplete_Kontrol/selection_linked_session_ring_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)      861 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/_Komplete_Kontrol/skin.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1045 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/_Komplete_Kontrol/sysex.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2616 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/_Komplete_Kontrol/transport_component.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/_MPDMkIIBase/
--rw-r--r--   0 sahlen     (501) staff       (20)      892 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/_MPDMkIIBase/ControlElementUtils.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2761 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/_MPDMkIIBase/MPDMkIIBase.py
--rw-r--r--   0 sahlen     (501) staff       (20)      372 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/_MPDMkIIBase/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/ableton_control_surface_scripts.egg-info/
--rw-r--r--   0 sahlen     (501) staff       (20)      572 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/ableton_control_surface_scripts.egg-info/PKG-INFO
--rw-r--r--   0 sahlen     (501) staff       (20)    29772 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/ableton_control_surface_scripts.egg-info/SOURCES.txt
--rw-r--r--   0 sahlen     (501) staff       (20)        1 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/ableton_control_surface_scripts.egg-info/dependency_links.txt
--rw-r--r--   0 sahlen     (501) staff       (20)       36 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/ableton_control_surface_scripts.egg-info/requires.txt
--rw-r--r--   0 sahlen     (501) staff       (20)     1474 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/ableton_control_surface_scripts.egg-info/top_level.txt
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/iRig_Keys_IO/
--rw-r--r--   0 sahlen     (501) staff       (20)      958 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/iRig_Keys_IO/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3815 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/iRig_Keys_IO/irig_keys_io.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2735 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/iRig_Keys_IO/mixer.py
--rw-r--r--   0 sahlen     (501) staff       (20)      963 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/iRig_Keys_IO/scroll.py
--rw-r--r--   0 sahlen     (501) staff       (20)      750 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.1/src/iRig_Keys_IO/session_recording.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1201 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/iRig_Keys_IO/session_ring.py
--rw-r--r--   0 sahlen     (501) staff       (20)      853 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/iRig_Keys_IO/skin.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/microKONTROL/
--rw-r--r--   0 sahlen     (501) staff       (20)     1173 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/microKONTROL/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2094 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/microKONTROL/config.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1836 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/microKONTROL/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/novation/
--rw-r--r--   0 sahlen     (501) staff       (20)      349 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.1/src/novation/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2322 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/novation/blinking_button.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1829 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.1/src/novation/channel_strip.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2399 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/novation/clip_actions.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1039 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/novation/clip_slot.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5452 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/novation/colors.py
--rw-r--r--   0 sahlen     (501) staff       (20)      749 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/novation/configurable_playable.py
--rw-r--r--   0 sahlen     (501) staff       (20)      867 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/novation/drum_group.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3685 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/novation/fixed_length.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1231 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/novation/fixed_length_recording.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1028 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/novation/fixed_radio_button_group.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3354 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/novation/instrument_control.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2027 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/novation/launchkey_drum_group.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3634 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/novation/launchkey_elements.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5936 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/novation/launchpad_elements.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1814 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/novation/mixer.py
--rw-r--r--   0 sahlen     (501) staff       (20)      834 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/novation/mode.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5264 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/novation/novation_base.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6368 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/novation/print_to_clip.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1769 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/novation/quantization.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2064 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/novation/session_modes.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1066 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/novation/session_navigation.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6339 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/novation/simple_device.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1382 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/novation/simple_device_navigation.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4065 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/novation/skin.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1033 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.1/src/novation/sysex.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3096 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/novation/track_recording.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1935 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/novation/transport.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1183 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.1/src/novation/util.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3635 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/novation/view_control.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/padKONTROL/
--rw-r--r--   0 sahlen     (501) staff       (20)     1190 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/padKONTROL/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1818 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/padKONTROL/config.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1842 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/padKONTROL/consts.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 12:05:46.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/
--rw-r--r--   0 sahlen     (501) staff       (20)      349 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7102 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/action_with_options_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)    17528 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/actions.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4803 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/auto_arm_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6811 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/automation_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4661 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/browser_modes.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1648 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/browser_util.py
--rw-r--r--   0 sahlen     (501) staff       (20)    27879 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/clip_control_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8980 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/colors.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9792 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/consts.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1432 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/control_element_factory.py
--rw-r--r--   0 sahlen     (501) staff       (20)      859 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/device_chain_utils.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3313 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/device_parameter_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7737 2024-01-08 19:12:03.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/drum_group_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)    10018 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/elements.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8224 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/fixed_length.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1917 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/grid_resolution.py
--rw-r--r--   0 sahlen     (501) staff       (20)    23474 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/instrument_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2787 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/internal_parameter.py
--rw-r--r--   0 sahlen     (501) staff       (20)    19297 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/loop_selector_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)      852 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/matrix_maps.py
--rw-r--r--   0 sahlen     (501) staff       (20)    14305 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/melodic_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5592 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/melodic_pattern.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5897 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/message_box_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2038 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/messenger_mode_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)      647 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/mixer_utils.py
--rw-r--r--   0 sahlen     (501) staff       (20)    32041 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/note_editor_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2397 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/note_editor_paginator.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3728 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/note_layout_switcher.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6174 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/note_repeat_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)    22399 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/note_settings_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1394 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/pad_button_element.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1386 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/pad_control.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2900 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/pad_sensitivity.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3333 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/playhead_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)    73106 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/push_base.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7031 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/quantization_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)    17033 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/scrollable_list.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9469 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/scrollable_list_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4019 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/select_playing_clip_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2752 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/selected_track_parameter_provider.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2012 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/selection.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8761 2024-01-08 19:12:03.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/session_recording_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3340 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/setting.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5445 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/skin_default.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9133 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/sliced_simpler_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5562 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/slideable_touch_strip_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1012 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/song_utils.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9187 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/special_session_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5138 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/step_duplicator.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8379 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/step_seq_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)      374 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/sysex.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2859 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/touch_encoder_element.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4972 2024-01-08 19:05:13.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/touch_strip_controller.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5176 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/touch_strip_element.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1233 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/track_frozen_mode.py
--rw-r--r--   0 sahlen     (501) staff       (20)      637 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/transport_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1306 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/undo_step_handler.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2503 2024-01-08 19:05:13.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/user_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8105 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/value_component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5656 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.1/src/pushbase/velocity_levels_component.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:02.000000 ableton-control-surface-scripts-0.0.2/
+-rw-r--r--   0 sahlen     (501) staff       (20)      715 2024-05-05 14:24:02.000000 ableton-control-surface-scripts-0.0.2/PKG-INFO
+-rw-r--r--   0 sahlen     (501) staff       (20)      876 2024-05-05 13:48:24.000000 ableton-control-surface-scripts-0.0.2/pyproject.toml
+-rw-r--r--   0 sahlen     (501) staff       (20)       38 2024-05-05 14:24:02.000000 ableton-control-surface-scripts-0.0.2/setup.cfg
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/ADVANCE/
+-rw-r--r--   0 sahlen     (501) staff       (20)     2650 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/ADVANCE/Advance.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      894 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/ADVANCE/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/AIRA_MX_1/
+-rw-r--r--   0 sahlen     (501) staff       (20)      802 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/AIRA_MX_1/Colors.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1255 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/AIRA_MX_1/ControlElementUtils.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1322 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/AIRA_MX_1/NotifyingMixerComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4343 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/AIRA_MX_1/NotifyingSessionComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5516 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/AIRA_MX_1/RolandMX1.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      910 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/AIRA_MX_1/SkinDefault.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      818 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/AIRA_MX_1/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/APC20/
+-rw-r--r--   0 sahlen     (501) staff       (20)     7672 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/APC20/APC20.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      811 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/APC20/BackgroundComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     7676 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/APC20/ShiftableSelectorComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3261 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/APC20/ShiftableZoomingComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2471 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/APC20/SliderModesComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      839 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/APC20/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      398 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/APC20/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/APC40/
+-rw-r--r--   0 sahlen     (501) staff       (20)    14531 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/APC40/APC40.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1220 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.2/src/APC40/SessionComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1956 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/APC40/TransportComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      839 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/APC40/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/APC40_MkII/
+-rw-r--r--   0 sahlen     (501) staff       (20)    16634 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/APC40_MkII/APC40_MkII.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1093 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.2/src/APC40_MkII/BankToggleComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4045 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/APC40_MkII/Colors.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4257 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/APC40_MkII/MixerComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2005 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/APC40_MkII/QuantizationComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1523 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/APC40_MkII/TransportComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      942 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/APC40_MkII/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/APC64/
+-rw-r--r--   0 sahlen     (501) staff       (20)     3917 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/APC64/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3962 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/APC64/colors.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3327 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/APC64/device.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3857 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/APC64/display.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5996 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/APC64/elements.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      958 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/APC64/firmware_mode.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1649 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/APC64/global_quantization.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8182 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/APC64/mappings.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      901 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/APC64/midi.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1901 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/APC64/mixer.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1249 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/APC64/recording.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6149 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/APC64/render_to_clip.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2830 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/APC64/session.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3916 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/APC64/settings.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3600 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/APC64/skin.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4299 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/APC64/touch_strip.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1569 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/APC64/transport.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/APC_Key_25/
+-rw-r--r--   0 sahlen     (501) staff       (20)    10529 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/APC_Key_25/APC_Key_25.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      953 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/APC_Key_25/MixerComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1051 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/APC_Key_25/SendToggleComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      858 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/APC_Key_25/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/APC_Key_25_mk2/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1562 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/APC_Key_25_mk2/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1880 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/APC_Key_25_mk2/colors.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1522 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/APC_Key_25_mk2/elements.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3554 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/APC_Key_25_mk2/mappings.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/APC_mini/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1426 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/APC_mini/APC_mini.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      848 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/APC_mini/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/APC_mini_mk2/
+-rw-r--r--   0 sahlen     (501) staff       (20)     2485 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/APC_mini_mk2/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2291 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/APC_mini_mk2/colors.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1730 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/APC_mini_mk2/elements.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3575 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/APC_mini_mk2/mappings.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/ATOM/
+-rw-r--r--   0 sahlen     (501) staff       (20)     2572 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/ATOM/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4483 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/ATOM/colors.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      896 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/ATOM/drum_group.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2522 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/ATOM/elements.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1642 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/ATOM/keyboard.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5204 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/ATOM/mappings.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      541 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/ATOM/midi.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      799 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/ATOM/note_pad.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2662 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/ATOM/skin.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/ATOMSQ/
+-rw-r--r--   0 sahlen     (501) staff       (20)     3331 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/ATOMSQ/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4700 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/ATOMSQ/colors.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2636 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/ATOMSQ/display.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4936 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/ATOMSQ/elements.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2228 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/ATOMSQ/launch_and_stop.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4454 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/ATOMSQ/mappings.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      782 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/ATOMSQ/midi.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1712 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/ATOMSQ/skin.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1872 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/ATOMSQ/touch_strip.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/
+-rw-r--r--   0 sahlen     (501) staff       (20)      853 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    22171 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/akai_force_mpc.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      643 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/background.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    16644 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/channel_strip.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2208 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/clip_actions.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4054 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/clip_slot.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2840 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/control.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2737 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/device.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4342 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/device_navigation.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     7630 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/device_parameters.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    35476 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/elements.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2516 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/live_colors.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4318 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/mixer.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      819 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/mode.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1272 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/multi_element.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      896 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/physical_display.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1921 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/ping_pong.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3397 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/scene.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1861 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/scene_list.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8367 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/session.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      962 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/session_navigation.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1058 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/session_recording.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2322 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/skin.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      787 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/sysex.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      579 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/sysex_element.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    10215 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/transport.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Alesis_V/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1483 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Alesis_V/Alesis_V.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      862 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Alesis_V/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Alesis_VI/
+-rw-r--r--   0 sahlen     (501) staff       (20)     2408 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Alesis_VI/Alesis_VI.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      916 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Alesis_VI/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Alesis_VX/
+-rw-r--r--   0 sahlen     (501) staff       (20)      416 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/Alesis_VX/Alesis_VX.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      842 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Alesis_VX/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Axiom/
+-rw-r--r--   0 sahlen     (501) staff       (20)      786 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Axiom/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1519 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Axiom/config.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1872 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Axiom/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/AxiomPro/
+-rw-r--r--   0 sahlen     (501) staff       (20)    10734 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/AxiomPro/AxiomPro.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5190 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/AxiomPro/DisplayingMixerComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5192 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/AxiomPro/EncoderMixerModeSelector.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6656 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/AxiomPro/MixerOrDeviceModeSelector.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2842 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/AxiomPro/NotifyingMixerComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    10420 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/AxiomPro/PageableDeviceComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1390 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/AxiomPro/PeekableEncoderElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3499 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/AxiomPro/SelectButtonModeSelector.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2132 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/AxiomPro/TransportViewModeSelector.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      897 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/AxiomPro/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_25_Classic/
+-rw-r--r--   0 sahlen     (501) staff       (20)     4762 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_25_Classic/Axiom.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      747 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_25_Classic/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_49_61_Classic/
+-rw-r--r--   0 sahlen     (501) staff       (20)     4773 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_49_61_Classic/Axiom.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3903 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_49_61_Classic/SliderSection.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      449 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_49_61_Classic/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/
+-rw-r--r--   0 sahlen     (501) staff       (20)    33436 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/Axiom_AIR_25_49_61.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2323 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/BestBankDeviceComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3465 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/ConfigurableButtonElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2547 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/DeviceNavComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4485 2024-01-08 19:05:13.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/DisplayingChanStripComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3956 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/EncoderModeSelector.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3556 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/FaderButtonModeSelector.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3709 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/FaderModeSelector.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3705 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/IdentifyingEncoderElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3232 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/MainModeSelector.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1844 2024-01-08 19:05:13.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/NumericalDisplayElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1581 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/NumericalDisplaySegment.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2657 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/SingleFaderButtonModeSelector.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1600 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/SpecialMixerComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4415 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/SpecialSessionComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2152 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/TransportViewModeSelector.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      973 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2267 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_Mini32/
+-rw-r--r--   0 sahlen     (501) staff       (20)     4927 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_Mini32/AxiomAirMini32.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2423 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_Mini32/DeviceNavComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1605 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_Mini32/EncoderMixerModeSelector.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3753 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_Mini32/MixerOrDeviceModeSelector.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      948 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_Mini32/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_DirectLink/
+-rw-r--r--   0 sahlen     (501) staff       (20)    16087 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_DirectLink/Axiom_DirectLink.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2895 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_DirectLink/BestBankDeviceComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2819 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_DirectLink/DetailViewCntrlComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1398 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_DirectLink/PeekableEncoderElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5865 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_DirectLink/ShiftableMixerComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2592 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_DirectLink/ShiftableSessionComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1747 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_DirectLink/ShiftableTransportComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2140 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_DirectLink/TransportViewModeSelector.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      887 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Axiom_DirectLink/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/BCF2000/
+-rw-r--r--   0 sahlen     (501) staff       (20)      745 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/BCF2000/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1650 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/BCF2000/config.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1831 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/BCF2000/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/BCR2000/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1029 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/BCR2000/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1475 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/BCR2000/config.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1835 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/BCR2000/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/BLOCKS/
+-rw-r--r--   0 sahlen     (501) staff       (20)      926 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/BLOCKS/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    10244 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/BLOCKS/blocks.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      688 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/BLOCKS/button.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4628 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/BLOCKS/colors.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      957 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/BLOCKS/element_translator.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      706 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/BLOCKS/mode.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1410 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/BLOCKS/skin.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2903 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/BLOCKS/target_track_provider.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/BeatStep/
+-rw-r--r--   0 sahlen     (501) staff       (20)     7147 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/BeatStep/BeatStep.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      810 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/BeatStep/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Blackstar_Live_Logic/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1003 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Blackstar_Live_Logic/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1536 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Blackstar_Live_Logic/blackstar_live_logic.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1388 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Blackstar_Live_Logic/clip_util.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1476 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Blackstar_Live_Logic/elements.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3680 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Blackstar_Live_Logic/footswitch_row_control.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    11296 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Blackstar_Live_Logic/looper.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      567 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Blackstar_Live_Logic/midi.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      627 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Blackstar_Live_Logic/skin.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2704 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/Blackstar_Live_Logic/time_display.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4522 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Blackstar_Live_Logic/track_util.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/CTRL49/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1088 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/CTRL49/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      533 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.2/src/CTRL49/ctrl49.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Code_Series/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1171 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Code_Series/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4660 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Code_Series/code.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1018 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Code_Series/element_utils.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1484 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Code_Series/mixer_navigation.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      879 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Code_Series/skin_default.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/FANTOM/
+-rw-r--r--   0 sahlen     (501) staff       (20)     2564 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/FANTOM/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1505 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/FANTOM/colors.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1151 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/FANTOM/control.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4901 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/FANTOM/elements.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2517 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/FANTOM/mappings.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2619 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/FANTOM/mixer.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      903 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/FANTOM/scene_name_display.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2089 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/FANTOM/session.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1853 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/FANTOM/simple_display.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      861 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/FANTOM/sysex.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2038 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/FANTOM/track_info_display.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1534 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/FANTOM/transport.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Faderport/
+-rw-r--r--   0 sahlen     (501) staff       (20)      861 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Faderport/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Faderport_16/
+-rw-r--r--   0 sahlen     (501) staff       (20)      865 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Faderport_16/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Faderport_16_XT/
+-rw-r--r--   0 sahlen     (501) staff       (20)      970 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Faderport_16_XT/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Faderport_8/
+-rw-r--r--   0 sahlen     (501) staff       (20)      863 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Faderport_8/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/FireOne/
+-rw-r--r--   0 sahlen     (501) staff       (20)     9332 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/FireOne/FireOne.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      443 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/FireOne/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Hammer_88_Pro/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1059 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Hammer_88_Pro/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      448 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/Hammer_88_Pro/hammer_88_pro.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/KONTROL49/
+-rw-r--r--   0 sahlen     (501) staff       (20)      747 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/KONTROL49/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2045 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/KONTROL49/config.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1833 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/KONTROL49/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/KeyFadr/
+-rw-r--r--   0 sahlen     (501) staff       (20)      541 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/KeyFadr/KeyFadr.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      802 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/KeyFadr/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1308 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab/DeviceNavigationComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1905 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab/DisplayElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    10304 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab/KeyLab.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1977 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab/MixerComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      594 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab/SessionComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      878 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_88/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1070 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_88/KeyLab88.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      804 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_88/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1114 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1065 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential/arrangement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1035 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential/channel_strip.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1877 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential/clip_slot.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1658 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential/control_element_utils.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2074 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential/hardware_settings.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    10304 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential/keylab_essential.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1596 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential/ringed_encoder.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1059 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential/ringed_mapped_encoder_control.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2998 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential/session.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1532 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential/skin_default.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1855 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential/sysex.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1901 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential/transport.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1360 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential/undo.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1116 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential/view_control.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential_mk3/
+-rw-r--r--   0 sahlen     (501) staff       (20)     2982 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential_mk3/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3564 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential_mk3/colors.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1547 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential_mk3/device_bank_toggle.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6251 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential_mk3/display.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6349 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential_mk3/elements.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2117 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential_mk3/mappings.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1747 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential_mk3/midi.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1744 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential_mk3/mixer.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_mkII/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1091 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_mkII/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1076 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_mkII/channel_strip.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      553 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_mkII/clip_slot.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1000 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_mkII/hardware_settings.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     7663 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_mkII/keylab_mkii.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      811 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_mkII/mixer.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      728 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_mkII/session.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1384 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/KeyLab_mkII/view_control.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/KeyPad/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1491 2024-01-08 19:05:13.000000 ableton-control-surface-scripts-0.0.2/src/KeyPad/CombinedButtonsElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2373 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.2/src/KeyPad/CuePointControlComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     7695 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/KeyPad/KeyPad.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      797 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/KeyPad/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Keystage/
+-rw-r--r--   0 sahlen     (501) staff       (20)     2576 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Keystage/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1879 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Keystage/display.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2532 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Keystage/elements.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1041 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Keystage/mappings.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Keystation_Pro_88/
+-rw-r--r--   0 sahlen     (501) staff       (20)      778 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Keystation_Pro_88/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1631 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Keystation_Pro_88/config.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1847 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Keystation_Pro_88/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_A/
+-rw-r--r--   0 sahlen     (501) staff       (20)      694 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_A/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1518 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_A/komplete_kontrol_a.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1103 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_A/view_control_component.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk2/
+-rw-r--r--   0 sahlen     (501) staff       (20)      686 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk2/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3611 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk2/channel_strip_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4299 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk2/komplete_kontrol_s_mk2.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1684 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk2/meter_display_element.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2312 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk2/mixer_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1679 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk2/session_ring_navigation_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2298 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk2/view_control_component.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk3/
+-rw-r--r--   0 sahlen     (501) staff       (20)     2937 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk3/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3946 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk3/display.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4646 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk3/elements.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1677 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk3/focus_follow.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1995 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk3/launch_and_stop.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2308 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk3/mappings.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1014 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk3/midi.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1644 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk3/session_navigation.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      618 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk3/skin.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1843 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk3/view_control.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/LPD8/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1008 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/LPD8/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1465 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/LPD8/config.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1836 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/LPD8/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/LV1_LX1/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1195 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/LV1_LX1/LV1_LX1.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      443 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.2/src/LV1_LX1/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/LV2_LX2_LC2_LD2/
+-rw-r--r--   0 sahlen     (501) staff       (20)    20891 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/LV2_LX2_LC2_LD2/Devices.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      929 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/LV2_LX2_LC2_LD2/DevicesXY.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1682 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/LV2_LX2_LC2_LD2/FaderfoxComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    14782 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/LV2_LX2_LC2_LD2/FaderfoxDeviceController.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8221 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/LV2_LX2_LC2_LD2/FaderfoxHelper.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9182 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/LV2_LX2_LC2_LD2/FaderfoxMixerController.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4628 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/LV2_LX2_LC2_LD2/FaderfoxScript.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8656 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/LV2_LX2_LC2_LD2/FaderfoxTransportController.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      684 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/LV2_LX2_LC2_LD2/LV2DeviceController.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6362 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/LV2_LX2_LC2_LD2/LV2MixerController.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5825 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/LV2_LX2_LC2_LD2/LV2TransportController.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1316 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/LV2_LX2_LC2_LD2/LV2_LX2_LC2_LD2.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3029 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/LV2_LX2_LC2_LD2/ParamMap.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1811 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/LV2_LX2_LC2_LD2/Params.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      475 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.2/src/LV2_LX2_LC2_LD2/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3397 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/LV2_LX2_LC2_LD2/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Launch_Control/
+-rw-r--r--   0 sahlen     (501) staff       (20)      548 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launch_Control/ButtonSysexControl.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      668 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.2/src/Launch_Control/Colors.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      707 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launch_Control/ConfigurableButtonElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1839 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Launch_Control/DeviceNavigationComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    11940 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Launch_Control/LaunchControl.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3918 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launch_Control/SpecialMixerComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      758 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launch_Control/SpecialSessionComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      638 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launch_Control/Sysex.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      824 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launch_Control/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Launch_Control_XL/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1162 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/Launch_Control_XL/ButtonElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2847 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Launch_Control_XL/DeviceComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8826 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Launch_Control_XL/LaunchControlXL.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4494 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Launch_Control_XL/MixerComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1165 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launch_Control_XL/SkinDefault.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      917 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launch_Control_XL/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey/
+-rw-r--r--   0 sahlen     (501) staff       (20)    10443 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey/Launchkey.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4212 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey/SessionNavigationComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2686 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey/SpecialMixerComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1815 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey/TransportViewModeSelector.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      917 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1019 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_MK2/
+-rw-r--r--   0 sahlen     (501) staff       (20)      741 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_MK2/BackgroundComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5519 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_MK2/Colors.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1302 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_MK2/ControlElementUtils.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3538 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_MK2/DeviceComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      895 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_MK2/InControlStatusComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    14504 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_MK2/Launchkey_MK2.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      579 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_MK2/MixerComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2878 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_MK2/ModeUtils.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1801 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_MK2/SessionComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1657 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_MK2/Skin.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1047 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_MK2/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      801 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_MK2/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_MK3/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1277 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_MK3/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3573 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_MK3/channel_strip.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1215 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_MK3/clip_actions.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1354 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_MK3/control.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3604 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_MK3/device.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5893 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_MK3/elements.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    17250 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_MK3/launchkey_mk3.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1172 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_MK3/midi.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2814 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_MK3/mixer.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1309 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_MK3/notification.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      700 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_MK3/rgb_button.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2341 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_MK3/simple_display.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1089 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_MK3/skin.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      683 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_MK3/transport.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_Mini/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1490 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_Mini/LaunchkeyMini.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      916 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_Mini/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_Mini_MK3/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1056 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_Mini_MK3/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      793 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_Mini_MK3/elements.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9392 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_Mini_MK3/launchkey_mini_mk3.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      449 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_Mini_MK3/midi.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1024 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_Mini_MK3/skin.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      393 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.2/src/Launchkey_Mini_MK3/sysex_ids.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad/
+-rw-r--r--   0 sahlen     (501) staff       (20)     2792 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad/ConfigurableButtonElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    12801 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad/DefChannelStripComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     7575 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad/Launchpad.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9692 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad/MainSelectorComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5407 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad/PreciseButtonSliderElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3313 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad/SpecialMixerComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1415 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad/SpecialSessionComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    11632 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad/SubSelectorComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      831 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_MK2/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1121 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_MK2/BackgroundComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     7160 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_MK2/ChannelStripComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5461 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_MK2/Colors.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      625 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_MK2/ComponentUtils.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2046 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_MK2/ControlElementUtils.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    17088 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_MK2/Launchpad_MK2.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6133 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_MK2/MixerComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3085 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_MK2/ModeUtils.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3032 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_MK2/SessionComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1252 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_MK2/SessionZoomingComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2698 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_MK2/Skin.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2057 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_MK2/SliderElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1588 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_MK2/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      868 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_MK2/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Mini_MK3/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1056 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Mini_MK3/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1433 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Mini_MK3/elements.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5515 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Mini_MK3/launchpad_mini_mk3.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1076 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Mini_MK3/notifying_background.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      815 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Mini_MK3/skin.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      414 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Mini_MK3/sysex_ids.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/
+-rw-r--r--   0 sahlen     (501) staff       (20)     2922 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/ActionsComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1823 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/BackgroundComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5542 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/ClipActionsComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5461 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/Colors.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2643 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/ConfigurableButtonElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1405 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/DeviceNavigationComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    15830 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/DrumGroupComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2920 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/DrumGroupFinderComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    45677 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/Launchpad_Pro.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      590 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/LedLightingComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2403 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/MultiButtonElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4030 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/SkinDefault.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3774 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/SlideComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2326 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/SliderElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1108 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/SpecialDeviceComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3412 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/SpecialMidiMap.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6818 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/SpecialMixerComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2109 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/SpecialModesComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    14385 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/SpecialSessionComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2654 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/SpecialSessionRecordingComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2730 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/TargetTrackComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1449 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/TranslationComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      729 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/UserMatrixComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      995 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2048 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro_MK3/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1112 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro_MK3/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1050 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro_MK3/channel_strip.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      632 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro_MK3/control.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3064 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro_MK3/drum_group.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     7058 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro_MK3/elements.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    19941 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro_MK3/launchpad_pro_mk3.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3239 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro_MK3/mixer.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4119 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro_MK3/session.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1960 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro_MK3/simple_device.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1376 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro_MK3/skin.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      578 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro_MK3/sysex_ids.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1006 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro_MK3/transport.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_X/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1021 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_X/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1162 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_X/channel_strip.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3026 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_X/elements.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    11925 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_X/launchpad_x.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1935 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_X/session_recording.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      885 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_X/skin.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      392 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/Launchpad_X/sysex_ids.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/MIDI_Mix/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1227 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/MIDI_Mix/ControlElementUtils.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3655 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/MIDI_Mix/MIDI_Mix.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1440 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MIDI_Mix/MixerComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      801 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MIDI_Mix/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/MPD18/
+-rw-r--r--   0 sahlen     (501) staff       (20)      765 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/MPD18/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2015 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MPD18/config.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1837 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MPD18/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/MPD218/
+-rw-r--r--   0 sahlen     (501) staff       (20)      602 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MPD218/MPD218.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      817 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MPD218/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/MPD226/
+-rw-r--r--   0 sahlen     (501) staff       (20)     2065 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/MPD226/MPD226.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      817 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MPD226/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/MPD232/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1789 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/MPD232/MPD232.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      817 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MPD232/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/MPD24/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1157 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/MPD24/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1853 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/MPD24/config.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1835 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/MPD24/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/MPD32/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1180 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/MPD32/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2046 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MPD32/config.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1842 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MPD32/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/MPK225/
+-rw-r--r--   0 sahlen     (501) staff       (20)     2484 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MPK225/MPK225.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      838 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MPK225/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/MPK249/
+-rw-r--r--   0 sahlen     (501) staff       (20)     2922 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MPK249/MPK249.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      838 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MPK249/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/MPK25/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1186 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/MPK25/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1959 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/MPK25/config.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1842 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/MPK25/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/MPK261/
+-rw-r--r--   0 sahlen     (501) staff       (20)     2922 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MPK261/MPK261.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      838 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MPK261/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/MPK49/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1206 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/MPK49/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1970 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/MPK49/config.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1842 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MPK49/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/MPK61/
+-rw-r--r--   0 sahlen     (501) staff       (20)      765 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/MPK61/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2046 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MPK61/config.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1842 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MPK61/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/MPK88/
+-rw-r--r--   0 sahlen     (501) staff       (20)      765 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/MPK88/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2046 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MPK88/config.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1842 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MPK88/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/MPK_mini_mkI/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1020 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/MPK_mini_mkI/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1653 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MPK_mini_mkI/config.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1852 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MPK_mini_mkI/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/MPK_mini_mkII/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1022 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/MPK_mini_mkII/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1654 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MPK_mini_mkII/config.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1853 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MPK_mini_mkII/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/MPK_mini_mkIII/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1023 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/MPK_mini_mkIII/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1655 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MPK_mini_mkIII/config.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1846 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MPK_mini_mkIII/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/MackieControl/
+-rw-r--r--   0 sahlen     (501) staff       (20)    20059 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/MackieControl/ChannelStrip.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    51253 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/MackieControl/ChannelStripController.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9648 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MackieControl/MackieControl.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1626 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MackieControl/MackieControlComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2113 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MackieControl/MainDisplay.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8600 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/MackieControl/MainDisplayController.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    12013 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MackieControl/SoftwareController.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2884 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MackieControl/TimeDisplay.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    23493 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/MackieControl/Transport.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      962 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MackieControl/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5917 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MackieControl/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/MackieControlXT/
+-rw-r--r--   0 sahlen     (501) staff       (20)     6055 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/MackieControlXT/MackieControlXT.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      475 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/MackieControlXT/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/MackieControl_Classic/
+-rw-r--r--   0 sahlen     (501) staff       (20)    19836 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/MackieControl_Classic/ChannelStrip.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    50602 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/MackieControl_Classic/ChannelStripController.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9656 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MackieControl_Classic/MackieControl.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1634 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/MackieControl_Classic/MackieControlComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2121 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/MackieControl_Classic/MainDisplay.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8608 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/MackieControl_Classic/MainDisplayController.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    12021 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/MackieControl_Classic/SoftwareController.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2892 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/MackieControl_Classic/TimeDisplay.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    23501 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/MackieControl_Classic/Transport.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      475 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/MackieControl_Classic/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5925 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/MackieControl_Classic/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/MasterControl/
+-rw-r--r--   0 sahlen     (501) staff       (20)      522 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/MasterControl/MasterControl.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      467 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/MasterControl/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/MaxForLive/
+-rw-r--r--   0 sahlen     (501) staff       (20)      837 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/MaxForLive/MaxForLive.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      602 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/MaxForLive/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/MidAir25/
+-rw-r--r--   0 sahlen     (501) staff       (20)      745 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/MidAir25/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1251 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/MidAir25/config.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1838 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/MidAir25/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/MiniLab/
+-rw-r--r--   0 sahlen     (501) staff       (20)     6446 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/MiniLab/MiniLab.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      805 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/MiniLab/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/MiniLab_3/
+-rw-r--r--   0 sahlen     (501) staff       (20)     2587 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MiniLab_3/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3702 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/MiniLab_3/analog_lab.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2553 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MiniLab_3/colors.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4151 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/MiniLab_3/display.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2638 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MiniLab_3/display_util.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      799 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MiniLab_3/drum_group.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2547 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/MiniLab_3/elements.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2584 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MiniLab_3/encoder.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2823 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/MiniLab_3/mappings.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1604 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MiniLab_3/midi.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      733 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MiniLab_3/sysex.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1704 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/MiniLab_3/transport.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/MiniLab_mkII/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1449 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MiniLab_mkII/HardwareSettingsComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4149 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/MiniLab_mkII/MiniLabMk2.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2546 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/MiniLab_mkII/SessionComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      882 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/MiniLab_mkII/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Novation_Impulse/
+-rw-r--r--   0 sahlen     (501) staff       (20)     4893 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Novation_Impulse/EncoderModeSelector.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    15697 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Novation_Impulse/Novation_Impulse.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1398 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Novation_Impulse/PeekableEncoderElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1747 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Novation_Impulse/ShiftableTransportComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5862 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Novation_Impulse/SpecialMixerComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2140 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Novation_Impulse/TransportViewModeSelector.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      852 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Novation_Impulse/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/O2/
+-rw-r--r--   0 sahlen     (501) staff       (20)      762 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/O2/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1401 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/O2/config.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1833 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/O2/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/OpenLabs/
+-rw-r--r--   0 sahlen     (501) staff       (20)     4589 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/OpenLabs/OpenLabs.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      600 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/OpenLabs/SpecialDeviceComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2978 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/OpenLabs/SpecialTransportComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      447 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.2/src/OpenLabs/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen49_61/
+-rw-r--r--   0 sahlen     (501) staff       (20)      771 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen49_61/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1418 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen49_61/config.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1876 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen49_61/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen8/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1033 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen8/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1433 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen8/config.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1839 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen8/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen8v2/
+-rw-r--r--   0 sahlen     (501) staff       (20)      769 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen8v2/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1447 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen8v2/config.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1839 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen8v2/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen_3rd_Gen/
+-rw-r--r--   0 sahlen     (501) staff       (20)     4773 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen_3rd_Gen/Oxygen_3rd_Gen.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3031 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen_3rd_Gen/SpecialMixerComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2138 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen_3rd_Gen/TransportViewModeSelector.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      471 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen_3rd_Gen/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen_4th_Gen/
+-rw-r--r--   0 sahlen     (501) staff       (20)      470 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen_4th_Gen/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen_5th_Gen/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1088 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen_5th_Gen/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      763 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen_5th_Gen/oxygen_5th_gen.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen_Pro/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1136 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen_Pro/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      552 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen_Pro/channel_strip.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      609 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen_Pro/colors.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5630 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen_Pro/elements.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      760 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen_Pro/midi.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      783 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen_Pro/mode.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    10948 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen_Pro/oxygen_pro.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1140 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen_Pro/session.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      956 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen_Pro/session_navigation.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1300 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen_Pro/skin.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen_Pro_Mini/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1071 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen_Pro_Mini/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      902 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen_Pro_Mini/oxygen_pro_mini.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1167 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Oxygen_Pro_Mini/simple_device.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Ozone/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1004 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Ozone/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1603 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Ozone/config.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1836 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Ozone/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Ozonic/
+-rw-r--r--   0 sahlen     (501) staff       (20)      766 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Ozonic/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1427 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Ozonic/config.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1870 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Ozonic/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Photon_25/
+-rw-r--r--   0 sahlen     (501) staff       (20)      747 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Photon_25/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1616 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Photon_25/config.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1840 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Photon_25/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Photon_X25/
+-rw-r--r--   0 sahlen     (501) staff       (20)      748 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Photon_X25/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1657 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Photon_X25/config.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1850 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Photon_X25/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/ProjectMixIO/
+-rw-r--r--   0 sahlen     (501) staff       (20)     7079 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/ProjectMixIO/ProjectMixIO.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      463 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/ProjectMixIO/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/Push/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1208 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Push/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5872 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Push/actions.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    18060 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Push/browser_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8865 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Push/browser_model.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4188 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push/browser_model_factory.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3480 2024-01-08 19:12:03.000000 ableton-control-surface-scripts-0.0.2/src/Push/browser_query.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1885 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Push/device_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    11719 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Push/device_navigation_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      708 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Push/drum_group_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3503 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push/elements.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1488 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Push/firmware_handling.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1489 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/Push/global_pad_parameters.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6086 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Push/handshake_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4281 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Push/mode_behaviours.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      921 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Push/multi_entry_mode.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    20813 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Push/navigation_node.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6723 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push/notification_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1187 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Push/pad_sensitivity.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     7684 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Push/parameter_mapping_sensitivities.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    38899 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push/push.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3180 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Push/quantization_settings.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    17028 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push/scales_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1083 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Push/selected_track_parameter_provider.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3654 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push/settings.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    13146 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Push/special_chan_strip_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6358 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Push/special_mixer_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3244 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Push/special_physical_display.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3508 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Push/sysex.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5029 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/Push/user_settings_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      821 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Push/with_priority.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1261 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/Push2/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1981 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/actions.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      692 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Push2/amp.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4696 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/analog.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3266 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Push2/auto_filter.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5304 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Push2/automation.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6736 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/bank_selection_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      937 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Push2/beatrepeat.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    39626 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Push2/browser_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2254 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Push2/browser_item.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3614 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Push2/browser_list.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4502 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Push2/browser_modes.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3796 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/cccontrol.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3253 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/chain_selection_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2440 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Push2/channel_eq.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3873 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/chorus2.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    41212 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Push2/clip_control.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8008 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/clip_decoration.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2398 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/collision.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3456 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/color_chooser.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    13616 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Push2/colors.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    11092 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/compressor.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    19234 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Push2/convert.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3552 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/corpus.py
+-rw-r--r--   0 sahlen     (501) staff       (20)   401313 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/Push2/custom_bank_definitions.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2784 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Push2/decoration.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4555 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/delay.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    10563 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Push2/device_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8166 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Push2/device_component_provider.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    15784 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/device_decoration.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3829 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Push2/device_decorator_factory.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    24545 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Push2/device_navigation.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4871 2024-01-08 19:12:03.000000 ableton-control-surface-scripts-0.0.2/src/Push2/device_options.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1972 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Push2/device_parameter_bank_with_options.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    38924 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/Push2/device_parameter_icons.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1042 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Push2/device_util.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5171 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/device_view_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    12828 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Push2/drift.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9421 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/drum_group_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6164 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Push2/drum_pad_parameter_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1083 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/drumcell.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9946 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/echo.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2930 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/elements.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      892 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Push2/eq3.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4824 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/eq8.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1511 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Push2/filterdelay.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6557 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Push2/firmware.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      702 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Push2/graindelay.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3771 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Push2/hardware_settings_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    20626 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Push2/hybrid_reverb.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1482 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Push2/item_lister.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1723 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/Push2/master_track.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9928 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/meld.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1172 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Push2/mixable_utilities.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    11977 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Push2/mixer_control_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1919 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Push2/mode_collector.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/model/
+-rw-r--r--   0 sahlen     (501) staff       (20)    24525 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Push2/model/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6885 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Push2/model/declaration.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    18509 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/model/generation.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    23935 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/model/repr.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      534 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/Push2/model/uniqueid.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9819 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/Push2/mute_solo_stop.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      677 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Push2/note_editor.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5115 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Push2/note_settings.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2868 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Push2/notification_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9254 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/operator.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1231 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Push2/pad_sensitivity.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5870 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/Push2/pad_velocity_curve.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     7585 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Push2/parameter_mapping_sensitivities.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1632 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/phasernew.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    61958 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Push2/push2.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2836 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Push2/push2_model.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2721 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/real_time_channel.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1045 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/redux2.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1421 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/resonator.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2555 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/reverb.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6687 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/roar.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    36539 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Push2/routing.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      765 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Push2/saturator.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     7512 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Push2/scales_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1084 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Push2/selected_track_parameter_provider.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5083 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Push2/session_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      618 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Push2/session_ring_selection_linking.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      899 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/settings.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9356 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/setup_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6220 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Push2/shifter.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      888 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Push2/simple_mode_switcher.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    20015 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/simpler.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     7938 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Push2/skin_default.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      950 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Push2/sliced_simpler.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1704 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/spectral.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4659 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/sysex.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3302 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/tension.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    42336 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Push2/timeline_navigation.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    16759 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Push2/track_list.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6702 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/track_mixer_control_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    11567 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Push2/track_selection.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3925 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Push2/transmute.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2934 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Push2/transport_state.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1801 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Push2/user_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1180 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Push2/vinyl.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3651 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Push2/visualisation_settings.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    29969 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Push2/wavetable.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:02.000000 ableton-control-surface-scripts-0.0.2/src/Radium49_61/
+-rw-r--r--   0 sahlen     (501) staff       (20)      748 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Radium49_61/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1262 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Radium49_61/config.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1841 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Radium49_61/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:02.000000 ableton-control-surface-scripts-0.0.2/src/RemoteSL/
+-rw-r--r--   0 sahlen     (501) staff       (20)     5232 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/RemoteSL/DisplayController.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    15180 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/RemoteSL/EffectController.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    22227 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/RemoteSL/MixerController.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6397 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/RemoteSL/RemoteSL.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1414 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/RemoteSL/RemoteSLComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      844 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/RemoteSL/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3791 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/RemoteSL/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:02.000000 ableton-control-surface-scripts-0.0.2/src/RemoteSL_Classic/
+-rw-r--r--   0 sahlen     (501) staff       (20)     5240 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/RemoteSL_Classic/DisplayController.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    14974 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/RemoteSL_Classic/EffectController.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    22235 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/RemoteSL_Classic/MixerController.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6405 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/RemoteSL_Classic/RemoteSL.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1422 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/RemoteSL_Classic/RemoteSLComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      927 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/RemoteSL_Classic/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3799 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/RemoteSL_Classic/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:02.000000 ableton-control-surface-scripts-0.0.2/src/Roland_A_PRO/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1314 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Roland_A_PRO/DeviceNavigationComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1514 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/Roland_A_PRO/MixerComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6687 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/Roland_A_PRO/Roland_A_PRO.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      996 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Roland_A_PRO/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:02.000000 ableton-control-surface-scripts-0.0.2/src/Roland_FA/
+-rw-r--r--   0 sahlen     (501) staff       (20)      947 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Roland_FA/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      847 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Roland_FA/control_element_utils.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5651 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/Roland_FA/fa.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      748 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Roland_FA/navigation.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1515 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Roland_FA/scroll.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      757 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/Roland_FA/skin.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      718 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/Roland_FA/transport.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:02.000000 ableton-control-surface-scripts-0.0.2/src/SL_MkIII/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1107 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/SL_MkIII/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3802 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/SL_MkIII/actions.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      858 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/SL_MkIII/caching_control_element.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6866 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/SL_MkIII/channel_strip.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      625 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/SL_MkIII/color_sysex_element.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2226 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/SL_MkIII/control.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2361 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/SL_MkIII/device.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5361 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/SL_MkIII/device_navigation.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2161 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/SL_MkIII/device_parameters.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      793 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/SL_MkIII/drum_group.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    13516 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/SL_MkIII/elements.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      746 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/SL_MkIII/message.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      467 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/SL_MkIII/messenger.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      935 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/SL_MkIII/midi_message_cache.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6190 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/SL_MkIII/mixer.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4181 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/SL_MkIII/mode.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9543 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/SL_MkIII/parameter_mapping_sensitivities.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1897 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/SL_MkIII/physical_display.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1215 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/SL_MkIII/session.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      763 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/SL_MkIII/session_navigation.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3222 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/SL_MkIII/session_ring_selection_linking.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3141 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/SL_MkIII/skin.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    28158 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/SL_MkIII/sl_mkiii.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2018 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/SL_MkIII/sysex.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1977 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/SL_MkIII/transport.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1348 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/SL_MkIII/util.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:02.000000 ableton-control-surface-scripts-0.0.2/src/Tranzport/
+-rw-r--r--   0 sahlen     (501) staff       (20)    43921 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/Tranzport/Tranzport.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      483 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/Tranzport/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2844 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/Tranzport/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:02.000000 ableton-control-surface-scripts-0.0.2/src/TriggerFinger/
+-rw-r--r--   0 sahlen     (501) staff       (20)      774 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/TriggerFinger/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1796 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/TriggerFinger/config.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1844 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/TriggerFinger/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:02.000000 ableton-control-surface-scripts-0.0.2/src/UC33e/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1072 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/UC33e/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1709 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/UC33e/config.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1829 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/UC33e/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:02.000000 ableton-control-surface-scripts-0.0.2/src/VCM600/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1602 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/VCM600/MixerComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     7398 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/VCM600/TrackEQComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3853 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/VCM600/TrackFilterComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      668 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/VCM600/TransportComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6428 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/VCM600/VCM600.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6605 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/VCM600/ViewTogglerComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      729 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/VCM600/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:02.000000 ableton-control-surface-scripts-0.0.2/src/ZERO8/
+-rw-r--r--   0 sahlen     (501) staff       (20)      765 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/ZERO8/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1758 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/ZERO8/config.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1837 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/ZERO8/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:02.000000 ableton-control-surface-scripts-0.0.2/src/_APC/
+-rw-r--r--   0 sahlen     (501) staff       (20)     7554 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/_APC/APC.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1594 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/_APC/ControlElementUtils.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4148 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/_APC/DetailViewCntrlComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      858 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/_APC/DeviceBankButtonElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1669 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/_APC/DeviceComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1830 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/_APC/MixerComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3014 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/_APC/RingedEncoderElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      752 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/_APC/SessionComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2363 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/_APC/SkinDefault.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      345 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/_APC/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:02.000000 ableton-control-surface-scripts-0.0.2/src/_Arturia/
+-rw-r--r--   0 sahlen     (501) staff       (20)     5250 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/_Arturia/ArturiaControlSurface.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2560 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/_Arturia/MixerComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1079 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.2/src/_Arturia/ScrollComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2210 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.2/src/_Arturia/SessionComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      349 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.2/src/_Arturia/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:02.000000 ableton-control-surface-scripts-0.0.2/src/_Axiom/
+-rw-r--r--   0 sahlen     (501) staff       (20)     8334 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/_Axiom/Encoders.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2092 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/_Axiom/Pads.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4207 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/_Axiom/Transport.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      347 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/_Axiom/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2048 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/_Axiom/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:02.000000 ableton-control-surface-scripts-0.0.2/src/_Komplete_Kontrol/
+-rw-r--r--   0 sahlen     (501) staff       (20)      358 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/_Komplete_Kontrol/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4506 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/_Komplete_Kontrol/channel_strip_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1319 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/_Komplete_Kontrol/clip_launch_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1723 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/_Komplete_Kontrol/control_element_util.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2163 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/_Komplete_Kontrol/detail_clip_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2418 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/_Komplete_Kontrol/focus_follow_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    13732 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/_Komplete_Kontrol/komplete_kontrol_base.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2336 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/_Komplete_Kontrol/mixer_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      777 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/_Komplete_Kontrol/physical_display_element.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1119 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/_Komplete_Kontrol/selection_linked_session_ring_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      861 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/_Komplete_Kontrol/skin.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1045 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/_Komplete_Kontrol/sysex.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2616 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/_Komplete_Kontrol/transport_component.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:02.000000 ableton-control-surface-scripts-0.0.2/src/_MPDMkIIBase/
+-rw-r--r--   0 sahlen     (501) staff       (20)      892 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/_MPDMkIIBase/ControlElementUtils.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2761 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/_MPDMkIIBase/MPDMkIIBase.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      372 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/_MPDMkIIBase/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:02.000000 ableton-control-surface-scripts-0.0.2/src/ableton_control_surface_scripts.egg-info/
+-rw-r--r--   0 sahlen     (501) staff       (20)      715 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/ableton_control_surface_scripts.egg-info/PKG-INFO
+-rw-r--r--   0 sahlen     (501) staff       (20)    29772 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/ableton_control_surface_scripts.egg-info/SOURCES.txt
+-rw-r--r--   0 sahlen     (501) staff       (20)        1 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/ableton_control_surface_scripts.egg-info/dependency_links.txt
+-rw-r--r--   0 sahlen     (501) staff       (20)       36 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/ableton_control_surface_scripts.egg-info/requires.txt
+-rw-r--r--   0 sahlen     (501) staff       (20)     1474 2024-05-05 14:24:01.000000 ableton-control-surface-scripts-0.0.2/src/ableton_control_surface_scripts.egg-info/top_level.txt
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:02.000000 ableton-control-surface-scripts-0.0.2/src/iRig_Keys_IO/
+-rw-r--r--   0 sahlen     (501) staff       (20)      958 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/iRig_Keys_IO/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3815 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/iRig_Keys_IO/irig_keys_io.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2735 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/iRig_Keys_IO/mixer.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      963 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/iRig_Keys_IO/scroll.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      750 2024-01-08 18:43:23.000000 ableton-control-surface-scripts-0.0.2/src/iRig_Keys_IO/session_recording.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1201 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/iRig_Keys_IO/session_ring.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      853 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/iRig_Keys_IO/skin.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:02.000000 ableton-control-surface-scripts-0.0.2/src/microKONTROL/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1173 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/microKONTROL/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2094 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/microKONTROL/config.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1836 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/microKONTROL/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:02.000000 ableton-control-surface-scripts-0.0.2/src/novation/
+-rw-r--r--   0 sahlen     (501) staff       (20)      349 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.2/src/novation/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2322 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/novation/blinking_button.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1829 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.2/src/novation/channel_strip.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2399 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/novation/clip_actions.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1039 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/novation/clip_slot.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5452 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/novation/colors.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      749 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/novation/configurable_playable.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      867 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/novation/drum_group.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3685 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/novation/fixed_length.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1231 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/novation/fixed_length_recording.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1028 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/novation/fixed_radio_button_group.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3354 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/novation/instrument_control.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2027 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/novation/launchkey_drum_group.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3634 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/novation/launchkey_elements.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5936 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/novation/launchpad_elements.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1814 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/novation/mixer.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      834 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/novation/mode.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5264 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/novation/novation_base.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6368 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/novation/print_to_clip.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1769 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/novation/quantization.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2064 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/novation/session_modes.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1066 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/novation/session_navigation.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6339 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/novation/simple_device.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1382 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/novation/simple_device_navigation.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4065 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/novation/skin.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1033 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.2/src/novation/sysex.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3096 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/novation/track_recording.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1935 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/novation/transport.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1183 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.2/src/novation/util.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3635 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/novation/view_control.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:02.000000 ableton-control-surface-scripts-0.0.2/src/padKONTROL/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1190 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/padKONTROL/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1818 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/padKONTROL/config.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1842 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/padKONTROL/consts.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:24:02.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/
+-rw-r--r--   0 sahlen     (501) staff       (20)      349 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     7102 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/action_with_options_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    17528 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/actions.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4803 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/auto_arm_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6811 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/automation_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4661 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/browser_modes.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1648 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/browser_util.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    27879 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/clip_control_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8980 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/colors.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9792 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/consts.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1432 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/control_element_factory.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      859 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/device_chain_utils.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3313 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/device_parameter_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     7737 2024-01-08 19:12:03.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/drum_group_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    10018 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/elements.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8224 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/fixed_length.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1917 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/grid_resolution.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    23474 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/instrument_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2787 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/internal_parameter.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    19297 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/loop_selector_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      852 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/matrix_maps.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    14305 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/melodic_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5592 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/melodic_pattern.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5897 2024-01-08 19:05:12.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/message_box_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2038 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/messenger_mode_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      647 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/mixer_utils.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    32041 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/note_editor_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2397 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/note_editor_paginator.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3728 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/note_layout_switcher.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6174 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/note_repeat_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    22399 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/note_settings_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1394 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/pad_button_element.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1386 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/pad_control.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2900 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/pad_sensitivity.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3333 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/playhead_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    73106 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/push_base.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     7031 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/quantization_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    17033 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/scrollable_list.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9469 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/scrollable_list_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4019 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/select_playing_clip_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2752 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/selected_track_parameter_provider.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2012 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/selection.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8761 2024-01-08 19:12:03.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/session_recording_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3340 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/setting.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5445 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/skin_default.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9133 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/sliced_simpler_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5562 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/slideable_touch_strip_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1012 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/song_utils.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9187 2024-01-08 19:11:24.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/special_session_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5138 2024-01-08 19:11:02.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/step_duplicator.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8379 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/step_seq_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      374 2024-01-08 18:43:24.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/sysex.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2859 2024-01-08 18:49:34.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/touch_encoder_element.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4972 2024-01-08 19:05:13.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/touch_strip_controller.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5176 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/touch_strip_element.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1233 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/track_frozen_mode.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      637 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/transport_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1306 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/undo_step_handler.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2503 2024-01-08 19:05:13.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/user_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8105 2024-01-08 18:49:35.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/value_component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5656 2024-01-09 19:53:39.000000 ableton-control-surface-scripts-0.0.2/src/pushbase/velocity_levels_component.py
```

### Comparing `ableton-control-surface-scripts-0.0.1/pyproject.toml` & `ableton-control-surface-scripts-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ableton-control-surface-scripts"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     {name = "Martin Sahlen", email = "martin8900@gmail.com"}
 ]
 description = "Decompiled control surface scripts from Ableton Live's Python API to help with reverse engineering and how other well known interfaces work."
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
+    "Development Status :: 3 - Alpha",
+    "Topic :: Multimedia :: Sound/Audio :: MIDI"
 ]
 dependencies = [
     "ableton-control-surface-core == 1.0.0"
 ]
+
 [project.urls]
-Homepage = "https://github.com/pypa/sampleproject"
-Issues = "https://github.com/pypa/sampleproject/issues"
+Homepage = "https://github.com/oslo1989/ableton-control-surface-toolkit"
+Issues = "https://github.com/oslo1989/ableton-control-surface-toolkit/issues"
```

### Comparing `ableton-control-surface-scripts-0.0.1/src/ADVANCE/Advance.py` & `ableton-control-surface-scripts-0.0.2/src/ADVANCE/Advance.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/ADVANCE/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/ADVANCE/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/AIRA_MX_1/Colors.py` & `ableton-control-surface-scripts-0.0.2/src/AIRA_MX_1/Colors.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/AIRA_MX_1/ControlElementUtils.py` & `ableton-control-surface-scripts-0.0.2/src/AIRA_MX_1/ControlElementUtils.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/AIRA_MX_1/NotifyingMixerComponent.py` & `ableton-control-surface-scripts-0.0.2/src/AIRA_MX_1/NotifyingMixerComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/AIRA_MX_1/NotifyingSessionComponent.py` & `ableton-control-surface-scripts-0.0.2/src/AIRA_MX_1/NotifyingSessionComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/AIRA_MX_1/RolandMX1.py` & `ableton-control-surface-scripts-0.0.2/src/AIRA_MX_1/RolandMX1.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/AIRA_MX_1/SkinDefault.py` & `ableton-control-surface-scripts-0.0.2/src/AIRA_MX_1/SkinDefault.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/AIRA_MX_1/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/AIRA_MX_1/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC20/APC20.py` & `ableton-control-surface-scripts-0.0.2/src/APC20/APC20.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC20/BackgroundComponent.py` & `ableton-control-surface-scripts-0.0.2/src/APC20/BackgroundComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC20/ShiftableSelectorComponent.py` & `ableton-control-surface-scripts-0.0.2/src/APC20/ShiftableSelectorComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC20/ShiftableZoomingComponent.py` & `ableton-control-surface-scripts-0.0.2/src/APC20/ShiftableZoomingComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC20/SliderModesComponent.py` & `ableton-control-surface-scripts-0.0.2/src/APC20/SliderModesComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC20/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/APC20/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC40/APC40.py` & `ableton-control-surface-scripts-0.0.2/src/APC40/APC40.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC40/SessionComponent.py` & `ableton-control-surface-scripts-0.0.2/src/APC40/SessionComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC40/TransportComponent.py` & `ableton-control-surface-scripts-0.0.2/src/APC40/TransportComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC40/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/APC40/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC40_MkII/APC40_MkII.py` & `ableton-control-surface-scripts-0.0.2/src/APC40_MkII/APC40_MkII.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC40_MkII/BankToggleComponent.py` & `ableton-control-surface-scripts-0.0.2/src/APC40_MkII/BankToggleComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC40_MkII/Colors.py` & `ableton-control-surface-scripts-0.0.2/src/APC40_MkII/Colors.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC40_MkII/MixerComponent.py` & `ableton-control-surface-scripts-0.0.2/src/APC40_MkII/MixerComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC40_MkII/QuantizationComponent.py` & `ableton-control-surface-scripts-0.0.2/src/APC40_MkII/QuantizationComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC40_MkII/TransportComponent.py` & `ableton-control-surface-scripts-0.0.2/src/APC40_MkII/TransportComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC40_MkII/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/APC40_MkII/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC64/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/APC64/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC64/colors.py` & `ableton-control-surface-scripts-0.0.2/src/APC64/colors.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC64/device.py` & `ableton-control-surface-scripts-0.0.2/src/APC64/device.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC64/display.py` & `ableton-control-surface-scripts-0.0.2/src/APC64/display.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC64/elements.py` & `ableton-control-surface-scripts-0.0.2/src/APC64/elements.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC64/firmware_mode.py` & `ableton-control-surface-scripts-0.0.2/src/APC64/firmware_mode.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC64/global_quantization.py` & `ableton-control-surface-scripts-0.0.2/src/APC64/global_quantization.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC64/mappings.py` & `ableton-control-surface-scripts-0.0.2/src/APC64/mappings.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC64/midi.py` & `ableton-control-surface-scripts-0.0.2/src/APC64/midi.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC64/mixer.py` & `ableton-control-surface-scripts-0.0.2/src/APC64/mixer.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC64/recording.py` & `ableton-control-surface-scripts-0.0.2/src/APC64/recording.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC64/render_to_clip.py` & `ableton-control-surface-scripts-0.0.2/src/APC64/render_to_clip.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC64/session.py` & `ableton-control-surface-scripts-0.0.2/src/APC64/session.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC64/settings.py` & `ableton-control-surface-scripts-0.0.2/src/APC64/settings.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC64/skin.py` & `ableton-control-surface-scripts-0.0.2/src/APC64/skin.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC64/touch_strip.py` & `ableton-control-surface-scripts-0.0.2/src/APC64/touch_strip.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC64/transport.py` & `ableton-control-surface-scripts-0.0.2/src/APC64/transport.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC_Key_25/APC_Key_25.py` & `ableton-control-surface-scripts-0.0.2/src/APC_Key_25/APC_Key_25.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC_Key_25/MixerComponent.py` & `ableton-control-surface-scripts-0.0.2/src/APC_Key_25/MixerComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC_Key_25/SendToggleComponent.py` & `ableton-control-surface-scripts-0.0.2/src/APC_Key_25/SendToggleComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC_Key_25/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/APC_Key_25/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC_Key_25_mk2/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/APC_Key_25_mk2/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC_Key_25_mk2/colors.py` & `ableton-control-surface-scripts-0.0.2/src/APC_Key_25_mk2/colors.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC_Key_25_mk2/elements.py` & `ableton-control-surface-scripts-0.0.2/src/APC_Key_25_mk2/elements.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC_Key_25_mk2/mappings.py` & `ableton-control-surface-scripts-0.0.2/src/APC_Key_25_mk2/mappings.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC_mini/APC_mini.py` & `ableton-control-surface-scripts-0.0.2/src/APC_mini/APC_mini.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC_mini/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/APC_mini/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC_mini_mk2/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/APC_mini_mk2/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC_mini_mk2/colors.py` & `ableton-control-surface-scripts-0.0.2/src/APC_mini_mk2/colors.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC_mini_mk2/elements.py` & `ableton-control-surface-scripts-0.0.2/src/APC_mini_mk2/elements.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/APC_mini_mk2/mappings.py` & `ableton-control-surface-scripts-0.0.2/src/APC_mini_mk2/mappings.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/ATOM/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/ATOM/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/ATOM/colors.py` & `ableton-control-surface-scripts-0.0.2/src/ATOM/colors.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/ATOM/drum_group.py` & `ableton-control-surface-scripts-0.0.2/src/ATOM/drum_group.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/ATOM/elements.py` & `ableton-control-surface-scripts-0.0.2/src/ATOM/elements.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/ATOM/keyboard.py` & `ableton-control-surface-scripts-0.0.2/src/ATOM/keyboard.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/ATOM/mappings.py` & `ableton-control-surface-scripts-0.0.2/src/ATOM/mappings.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/ATOM/midi.py` & `ableton-control-surface-scripts-0.0.2/src/ATOM/midi.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/ATOM/note_pad.py` & `ableton-control-surface-scripts-0.0.2/src/ATOM/note_pad.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/ATOM/skin.py` & `ableton-control-surface-scripts-0.0.2/src/ATOM/skin.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/ATOMSQ/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/ATOMSQ/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/ATOMSQ/colors.py` & `ableton-control-surface-scripts-0.0.2/src/ATOMSQ/colors.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/ATOMSQ/display.py` & `ableton-control-surface-scripts-0.0.2/src/ATOMSQ/display.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/ATOMSQ/elements.py` & `ableton-control-surface-scripts-0.0.2/src/ATOMSQ/elements.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/ATOMSQ/launch_and_stop.py` & `ableton-control-surface-scripts-0.0.2/src/ATOMSQ/launch_and_stop.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/ATOMSQ/mappings.py` & `ableton-control-surface-scripts-0.0.2/src/ATOMSQ/mappings.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/ATOMSQ/midi.py` & `ableton-control-surface-scripts-0.0.2/src/ATOMSQ/midi.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/ATOMSQ/skin.py` & `ableton-control-surface-scripts-0.0.2/src/ATOMSQ/skin.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/ATOMSQ/touch_strip.py` & `ableton-control-surface-scripts-0.0.2/src/ATOMSQ/touch_strip.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/akai_force_mpc.py` & `ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/akai_force_mpc.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/background.py` & `ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/background.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/channel_strip.py` & `ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/channel_strip.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/clip_actions.py` & `ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/clip_actions.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/clip_slot.py` & `ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/clip_slot.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/control.py` & `ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/control.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/device.py` & `ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/device.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/device_navigation.py` & `ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/device_navigation.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/device_parameters.py` & `ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/device_parameters.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/elements.py` & `ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/elements.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/live_colors.py` & `ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/live_colors.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/mixer.py` & `ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/mixer.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/mode.py` & `ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/mode.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/multi_element.py` & `ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/multi_element.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/physical_display.py` & `ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/physical_display.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/ping_pong.py` & `ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/ping_pong.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/scene.py` & `ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/scene.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/scene_list.py` & `ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/scene_list.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/session.py` & `ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/session.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/session_navigation.py` & `ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/session_navigation.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/session_recording.py` & `ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/session_recording.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/skin.py` & `ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/skin.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/sysex.py` & `ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/sysex.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/sysex_element.py` & `ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/sysex_element.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Akai_Force_MPC/transport.py` & `ableton-control-surface-scripts-0.0.2/src/Akai_Force_MPC/transport.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Alesis_V/Alesis_V.py` & `ableton-control-surface-scripts-0.0.2/src/Alesis_V/Alesis_V.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Alesis_V/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Alesis_V/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Alesis_VI/Alesis_VI.py` & `ableton-control-surface-scripts-0.0.2/src/Alesis_VI/Alesis_VI.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Alesis_VI/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Alesis_VI/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Alesis_VX/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Alesis_VX/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom/config.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom/config.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom/consts.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/AxiomPro/AxiomPro.py` & `ableton-control-surface-scripts-0.0.2/src/AxiomPro/AxiomPro.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/AxiomPro/DisplayingMixerComponent.py` & `ableton-control-surface-scripts-0.0.2/src/AxiomPro/DisplayingMixerComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/AxiomPro/EncoderMixerModeSelector.py` & `ableton-control-surface-scripts-0.0.2/src/AxiomPro/EncoderMixerModeSelector.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/AxiomPro/MixerOrDeviceModeSelector.py` & `ableton-control-surface-scripts-0.0.2/src/AxiomPro/MixerOrDeviceModeSelector.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/AxiomPro/NotifyingMixerComponent.py` & `ableton-control-surface-scripts-0.0.2/src/AxiomPro/NotifyingMixerComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/AxiomPro/PageableDeviceComponent.py` & `ableton-control-surface-scripts-0.0.2/src/AxiomPro/PageableDeviceComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/AxiomPro/PeekableEncoderElement.py` & `ableton-control-surface-scripts-0.0.2/src/AxiomPro/PeekableEncoderElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/AxiomPro/SelectButtonModeSelector.py` & `ableton-control-surface-scripts-0.0.2/src/AxiomPro/SelectButtonModeSelector.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/AxiomPro/TransportViewModeSelector.py` & `ableton-control-surface-scripts-0.0.2/src/AxiomPro/TransportViewModeSelector.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/AxiomPro/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/AxiomPro/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_25_Classic/Axiom.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_25_Classic/Axiom.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_25_Classic/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_25_Classic/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_49_61_Classic/Axiom.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_49_61_Classic/Axiom.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_49_61_Classic/SliderSection.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_49_61_Classic/SliderSection.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/Axiom_AIR_25_49_61.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/Axiom_AIR_25_49_61.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/BestBankDeviceComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/BestBankDeviceComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/ConfigurableButtonElement.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/ConfigurableButtonElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/DeviceNavComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/DeviceNavComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/DisplayingChanStripComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/DisplayingChanStripComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/EncoderModeSelector.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/EncoderModeSelector.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/FaderButtonModeSelector.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/FaderButtonModeSelector.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/FaderModeSelector.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/FaderModeSelector.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/IdentifyingEncoderElement.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/IdentifyingEncoderElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/MainModeSelector.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/MainModeSelector.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/NumericalDisplayElement.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/NumericalDisplayElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/NumericalDisplaySegment.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/NumericalDisplaySegment.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/SingleFaderButtonModeSelector.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/SingleFaderButtonModeSelector.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/SpecialMixerComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/SpecialMixerComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/SpecialSessionComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/SpecialSessionComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/TransportViewModeSelector.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/TransportViewModeSelector.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_25_49_61/consts.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_25_49_61/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_Mini32/AxiomAirMini32.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_Mini32/AxiomAirMini32.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_Mini32/DeviceNavComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_Mini32/DeviceNavComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_Mini32/EncoderMixerModeSelector.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_Mini32/EncoderMixerModeSelector.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_Mini32/MixerOrDeviceModeSelector.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_Mini32/MixerOrDeviceModeSelector.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_AIR_Mini32/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_AIR_Mini32/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_DirectLink/Axiom_DirectLink.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_DirectLink/Axiom_DirectLink.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_DirectLink/BestBankDeviceComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_DirectLink/BestBankDeviceComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_DirectLink/DetailViewCntrlComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_DirectLink/DetailViewCntrlComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_DirectLink/PeekableEncoderElement.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_DirectLink/PeekableEncoderElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_DirectLink/ShiftableMixerComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_DirectLink/ShiftableMixerComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_DirectLink/ShiftableSessionComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_DirectLink/ShiftableSessionComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_DirectLink/ShiftableTransportComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_DirectLink/ShiftableTransportComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_DirectLink/TransportViewModeSelector.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_DirectLink/TransportViewModeSelector.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Axiom_DirectLink/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Axiom_DirectLink/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/BCF2000/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/BCF2000/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/BCF2000/config.py` & `ableton-control-surface-scripts-0.0.2/src/BCF2000/config.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/BCF2000/consts.py` & `ableton-control-surface-scripts-0.0.2/src/BCF2000/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/BCR2000/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/BCR2000/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/BCR2000/config.py` & `ableton-control-surface-scripts-0.0.2/src/BCR2000/config.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/BCR2000/consts.py` & `ableton-control-surface-scripts-0.0.2/src/BCR2000/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/BLOCKS/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/BLOCKS/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/BLOCKS/blocks.py` & `ableton-control-surface-scripts-0.0.2/src/BLOCKS/blocks.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/BLOCKS/button.py` & `ableton-control-surface-scripts-0.0.2/src/BLOCKS/button.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/BLOCKS/colors.py` & `ableton-control-surface-scripts-0.0.2/src/BLOCKS/colors.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/BLOCKS/element_translator.py` & `ableton-control-surface-scripts-0.0.2/src/BLOCKS/element_translator.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/BLOCKS/mode.py` & `ableton-control-surface-scripts-0.0.2/src/BLOCKS/mode.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/BLOCKS/skin.py` & `ableton-control-surface-scripts-0.0.2/src/BLOCKS/skin.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/BLOCKS/target_track_provider.py` & `ableton-control-surface-scripts-0.0.2/src/BLOCKS/target_track_provider.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/BeatStep/BeatStep.py` & `ableton-control-surface-scripts-0.0.2/src/BeatStep/BeatStep.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/BeatStep/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/BeatStep/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Blackstar_Live_Logic/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Blackstar_Live_Logic/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Blackstar_Live_Logic/blackstar_live_logic.py` & `ableton-control-surface-scripts-0.0.2/src/Blackstar_Live_Logic/blackstar_live_logic.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Blackstar_Live_Logic/clip_util.py` & `ableton-control-surface-scripts-0.0.2/src/Blackstar_Live_Logic/clip_util.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Blackstar_Live_Logic/elements.py` & `ableton-control-surface-scripts-0.0.2/src/Blackstar_Live_Logic/elements.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Blackstar_Live_Logic/footswitch_row_control.py` & `ableton-control-surface-scripts-0.0.2/src/Blackstar_Live_Logic/footswitch_row_control.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Blackstar_Live_Logic/looper.py` & `ableton-control-surface-scripts-0.0.2/src/Blackstar_Live_Logic/looper.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Blackstar_Live_Logic/midi.py` & `ableton-control-surface-scripts-0.0.2/src/Blackstar_Live_Logic/midi.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Blackstar_Live_Logic/skin.py` & `ableton-control-surface-scripts-0.0.2/src/Blackstar_Live_Logic/skin.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Blackstar_Live_Logic/time_display.py` & `ableton-control-surface-scripts-0.0.2/src/Blackstar_Live_Logic/time_display.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Blackstar_Live_Logic/track_util.py` & `ableton-control-surface-scripts-0.0.2/src/Blackstar_Live_Logic/track_util.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/CTRL49/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/CTRL49/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/CTRL49/ctrl49.py` & `ableton-control-surface-scripts-0.0.2/src/CTRL49/ctrl49.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Code_Series/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Code_Series/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Code_Series/code.py` & `ableton-control-surface-scripts-0.0.2/src/Code_Series/code.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Code_Series/element_utils.py` & `ableton-control-surface-scripts-0.0.2/src/Code_Series/element_utils.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Code_Series/mixer_navigation.py` & `ableton-control-surface-scripts-0.0.2/src/Code_Series/mixer_navigation.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Code_Series/skin_default.py` & `ableton-control-surface-scripts-0.0.2/src/Code_Series/skin_default.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/FANTOM/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/FANTOM/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/FANTOM/colors.py` & `ableton-control-surface-scripts-0.0.2/src/FANTOM/colors.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/FANTOM/control.py` & `ableton-control-surface-scripts-0.0.2/src/FANTOM/control.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/FANTOM/elements.py` & `ableton-control-surface-scripts-0.0.2/src/FANTOM/elements.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/FANTOM/mappings.py` & `ableton-control-surface-scripts-0.0.2/src/FANTOM/mappings.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/FANTOM/mixer.py` & `ableton-control-surface-scripts-0.0.2/src/FANTOM/mixer.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/FANTOM/scene_name_display.py` & `ableton-control-surface-scripts-0.0.2/src/FANTOM/scene_name_display.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/FANTOM/session.py` & `ableton-control-surface-scripts-0.0.2/src/FANTOM/session.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/FANTOM/simple_display.py` & `ableton-control-surface-scripts-0.0.2/src/FANTOM/simple_display.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/FANTOM/sysex.py` & `ableton-control-surface-scripts-0.0.2/src/FANTOM/sysex.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/FANTOM/track_info_display.py` & `ableton-control-surface-scripts-0.0.2/src/FANTOM/track_info_display.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/FANTOM/transport.py` & `ableton-control-surface-scripts-0.0.2/src/FANTOM/transport.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Faderport/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Faderport/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Faderport_16/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Faderport_16/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Faderport_16_XT/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Faderport_16_XT/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Faderport_8/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Faderport_8/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/FireOne/FireOne.py` & `ableton-control-surface-scripts-0.0.2/src/FireOne/FireOne.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Hammer_88_Pro/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Hammer_88_Pro/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KONTROL49/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/KONTROL49/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KONTROL49/config.py` & `ableton-control-surface-scripts-0.0.2/src/KONTROL49/config.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KONTROL49/consts.py` & `ableton-control-surface-scripts-0.0.2/src/KONTROL49/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyFadr/KeyFadr.py` & `ableton-control-surface-scripts-0.0.2/src/KeyFadr/KeyFadr.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyFadr/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/KeyFadr/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab/DeviceNavigationComponent.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab/DeviceNavigationComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab/DisplayElement.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab/DisplayElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab/KeyLab.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab/KeyLab.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab/MixerComponent.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab/MixerComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab/SessionComponent.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab/SessionComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab_88/KeyLab88.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab_88/KeyLab88.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab_88/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab_88/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential/arrangement.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential/arrangement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential/channel_strip.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential/channel_strip.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential/clip_slot.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential/clip_slot.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential/control_element_utils.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential/control_element_utils.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential/hardware_settings.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential/hardware_settings.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential/keylab_essential.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential/keylab_essential.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential/ringed_encoder.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential/ringed_encoder.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential/ringed_mapped_encoder_control.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential/ringed_mapped_encoder_control.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential/session.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential/session.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential/skin_default.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential/skin_default.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential/sysex.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential/sysex.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential/transport.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential/transport.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential/undo.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential/undo.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential/view_control.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential/view_control.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential_mk3/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential_mk3/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential_mk3/colors.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential_mk3/colors.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential_mk3/device_bank_toggle.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential_mk3/device_bank_toggle.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential_mk3/display.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential_mk3/display.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential_mk3/elements.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential_mk3/elements.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential_mk3/mappings.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential_mk3/mappings.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential_mk3/midi.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential_mk3/midi.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab_Essential_mk3/mixer.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab_Essential_mk3/mixer.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab_mkII/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab_mkII/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab_mkII/channel_strip.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab_mkII/channel_strip.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab_mkII/clip_slot.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab_mkII/clip_slot.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab_mkII/hardware_settings.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab_mkII/hardware_settings.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab_mkII/keylab_mkii.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab_mkII/keylab_mkii.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab_mkII/mixer.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab_mkII/mixer.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab_mkII/session.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab_mkII/session.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyLab_mkII/view_control.py` & `ableton-control-surface-scripts-0.0.2/src/KeyLab_mkII/view_control.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyPad/CombinedButtonsElement.py` & `ableton-control-surface-scripts-0.0.2/src/KeyPad/CombinedButtonsElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyPad/CuePointControlComponent.py` & `ableton-control-surface-scripts-0.0.2/src/KeyPad/CuePointControlComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyPad/KeyPad.py` & `ableton-control-surface-scripts-0.0.2/src/KeyPad/KeyPad.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/KeyPad/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/KeyPad/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Keystage/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Keystage/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Keystage/display.py` & `ableton-control-surface-scripts-0.0.2/src/Keystage/display.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Keystage/elements.py` & `ableton-control-surface-scripts-0.0.2/src/Keystage/elements.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Keystage/mappings.py` & `ableton-control-surface-scripts-0.0.2/src/Keystage/mappings.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Keystation_Pro_88/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Keystation_Pro_88/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Keystation_Pro_88/config.py` & `ableton-control-surface-scripts-0.0.2/src/Keystation_Pro_88/config.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Keystation_Pro_88/consts.py` & `ableton-control-surface-scripts-0.0.2/src/Keystation_Pro_88/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_A/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_A/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_A/komplete_kontrol_a.py` & `ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_A/komplete_kontrol_a.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_A/view_control_component.py` & `ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_A/view_control_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk2/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk2/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk2/channel_strip_component.py` & `ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk2/channel_strip_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk2/komplete_kontrol_s_mk2.py` & `ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk2/komplete_kontrol_s_mk2.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk2/meter_display_element.py` & `ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk2/meter_display_element.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk2/mixer_component.py` & `ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk2/mixer_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk2/session_ring_navigation_component.py` & `ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk2/session_ring_navigation_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk2/view_control_component.py` & `ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk2/view_control_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk3/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk3/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk3/display.py` & `ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk3/display.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk3/elements.py` & `ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk3/elements.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk3/focus_follow.py` & `ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk3/focus_follow.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk3/launch_and_stop.py` & `ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk3/launch_and_stop.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk3/mappings.py` & `ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk3/mappings.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk3/midi.py` & `ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk3/midi.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk3/session_navigation.py` & `ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk3/session_navigation.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk3/skin.py` & `ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk3/skin.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Komplete_Kontrol_S_Mk3/view_control.py` & `ableton-control-surface-scripts-0.0.2/src/Komplete_Kontrol_S_Mk3/view_control.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/LPD8/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/LPD8/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/LPD8/config.py` & `ableton-control-surface-scripts-0.0.2/src/LPD8/config.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/LPD8/consts.py` & `ableton-control-surface-scripts-0.0.2/src/LPD8/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/LV1_LX1/LV1_LX1.py` & `ableton-control-surface-scripts-0.0.2/src/LV1_LX1/LV1_LX1.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/LV2_LX2_LC2_LD2/Devices.py` & `ableton-control-surface-scripts-0.0.2/src/LV2_LX2_LC2_LD2/Devices.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/LV2_LX2_LC2_LD2/DevicesXY.py` & `ableton-control-surface-scripts-0.0.2/src/LV2_LX2_LC2_LD2/DevicesXY.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/LV2_LX2_LC2_LD2/FaderfoxComponent.py` & `ableton-control-surface-scripts-0.0.2/src/LV2_LX2_LC2_LD2/FaderfoxComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/LV2_LX2_LC2_LD2/FaderfoxDeviceController.py` & `ableton-control-surface-scripts-0.0.2/src/LV2_LX2_LC2_LD2/FaderfoxDeviceController.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/LV2_LX2_LC2_LD2/FaderfoxHelper.py` & `ableton-control-surface-scripts-0.0.2/src/LV2_LX2_LC2_LD2/FaderfoxHelper.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/LV2_LX2_LC2_LD2/FaderfoxMixerController.py` & `ableton-control-surface-scripts-0.0.2/src/LV2_LX2_LC2_LD2/FaderfoxMixerController.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/LV2_LX2_LC2_LD2/FaderfoxScript.py` & `ableton-control-surface-scripts-0.0.2/src/LV2_LX2_LC2_LD2/FaderfoxScript.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/LV2_LX2_LC2_LD2/FaderfoxTransportController.py` & `ableton-control-surface-scripts-0.0.2/src/LV2_LX2_LC2_LD2/FaderfoxTransportController.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/LV2_LX2_LC2_LD2/LV2DeviceController.py` & `ableton-control-surface-scripts-0.0.2/src/LV2_LX2_LC2_LD2/LV2DeviceController.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/LV2_LX2_LC2_LD2/LV2MixerController.py` & `ableton-control-surface-scripts-0.0.2/src/LV2_LX2_LC2_LD2/LV2MixerController.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/LV2_LX2_LC2_LD2/LV2TransportController.py` & `ableton-control-surface-scripts-0.0.2/src/LV2_LX2_LC2_LD2/LV2TransportController.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/LV2_LX2_LC2_LD2/LV2_LX2_LC2_LD2.py` & `ableton-control-surface-scripts-0.0.2/src/LV2_LX2_LC2_LD2/LV2_LX2_LC2_LD2.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/LV2_LX2_LC2_LD2/ParamMap.py` & `ableton-control-surface-scripts-0.0.2/src/LV2_LX2_LC2_LD2/ParamMap.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/LV2_LX2_LC2_LD2/Params.py` & `ableton-control-surface-scripts-0.0.2/src/LV2_LX2_LC2_LD2/Params.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/LV2_LX2_LC2_LD2/consts.py` & `ableton-control-surface-scripts-0.0.2/src/LV2_LX2_LC2_LD2/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launch_Control/ButtonSysexControl.py` & `ableton-control-surface-scripts-0.0.2/src/Launch_Control/ButtonSysexControl.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launch_Control/Colors.py` & `ableton-control-surface-scripts-0.0.2/src/Launch_Control/Colors.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launch_Control/ConfigurableButtonElement.py` & `ableton-control-surface-scripts-0.0.2/src/Launch_Control/ConfigurableButtonElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launch_Control/DeviceNavigationComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launch_Control/DeviceNavigationComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launch_Control/LaunchControl.py` & `ableton-control-surface-scripts-0.0.2/src/Launch_Control/LaunchControl.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launch_Control/SpecialMixerComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launch_Control/SpecialMixerComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launch_Control/SpecialSessionComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launch_Control/SpecialSessionComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launch_Control/Sysex.py` & `ableton-control-surface-scripts-0.0.2/src/Launch_Control/Sysex.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launch_Control/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Launch_Control/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launch_Control_XL/ButtonElement.py` & `ableton-control-surface-scripts-0.0.2/src/Launch_Control_XL/ButtonElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launch_Control_XL/DeviceComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launch_Control_XL/DeviceComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launch_Control_XL/LaunchControlXL.py` & `ableton-control-surface-scripts-0.0.2/src/Launch_Control_XL/LaunchControlXL.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launch_Control_XL/MixerComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launch_Control_XL/MixerComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launch_Control_XL/SkinDefault.py` & `ableton-control-surface-scripts-0.0.2/src/Launch_Control_XL/SkinDefault.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launch_Control_XL/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Launch_Control_XL/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey/Launchkey.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey/Launchkey.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey/SessionNavigationComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey/SessionNavigationComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey/SpecialMixerComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey/SpecialMixerComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey/TransportViewModeSelector.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey/TransportViewModeSelector.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey/consts.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey_MK2/BackgroundComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey_MK2/BackgroundComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey_MK2/Colors.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey_MK2/Colors.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey_MK2/ControlElementUtils.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey_MK2/ControlElementUtils.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey_MK2/DeviceComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey_MK2/DeviceComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey_MK2/InControlStatusComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey_MK2/InControlStatusComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey_MK2/Launchkey_MK2.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey_MK2/Launchkey_MK2.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey_MK2/MixerComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey_MK2/MixerComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey_MK2/ModeUtils.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey_MK2/ModeUtils.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey_MK2/SessionComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey_MK2/SessionComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey_MK2/Skin.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey_MK2/Skin.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey_MK2/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey_MK2/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey_MK2/consts.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey_MK2/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey_MK3/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey_MK3/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey_MK3/channel_strip.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey_MK3/channel_strip.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey_MK3/clip_actions.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey_MK3/clip_actions.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey_MK3/control.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey_MK3/control.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey_MK3/device.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey_MK3/device.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey_MK3/elements.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey_MK3/elements.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey_MK3/launchkey_mk3.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey_MK3/launchkey_mk3.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey_MK3/midi.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey_MK3/midi.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey_MK3/mixer.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey_MK3/mixer.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey_MK3/notification.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey_MK3/notification.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey_MK3/rgb_button.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey_MK3/rgb_button.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey_MK3/simple_display.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey_MK3/simple_display.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey_MK3/skin.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey_MK3/skin.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey_MK3/transport.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey_MK3/transport.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey_Mini/LaunchkeyMini.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey_Mini/LaunchkeyMini.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey_Mini/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey_Mini/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey_Mini_MK3/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey_Mini_MK3/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey_Mini_MK3/elements.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey_Mini_MK3/elements.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey_Mini_MK3/launchkey_mini_mk3.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey_Mini_MK3/launchkey_mini_mk3.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchkey_Mini_MK3/skin.py` & `ableton-control-surface-scripts-0.0.2/src/Launchkey_Mini_MK3/skin.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad/ConfigurableButtonElement.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad/ConfigurableButtonElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad/DefChannelStripComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad/DefChannelStripComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad/Launchpad.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad/Launchpad.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad/MainSelectorComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad/MainSelectorComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad/PreciseButtonSliderElement.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad/PreciseButtonSliderElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad/SpecialMixerComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad/SpecialMixerComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad/SpecialSessionComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad/SpecialSessionComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad/SubSelectorComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad/SubSelectorComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_MK2/BackgroundComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_MK2/BackgroundComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_MK2/ChannelStripComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_MK2/ChannelStripComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_MK2/Colors.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_MK2/Colors.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_MK2/ComponentUtils.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_MK2/ComponentUtils.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_MK2/ControlElementUtils.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_MK2/ControlElementUtils.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_MK2/Launchpad_MK2.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_MK2/Launchpad_MK2.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_MK2/MixerComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_MK2/MixerComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_MK2/ModeUtils.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_MK2/ModeUtils.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_MK2/SessionComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_MK2/SessionComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_MK2/SessionZoomingComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_MK2/SessionZoomingComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_MK2/Skin.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_MK2/Skin.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_MK2/SliderElement.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_MK2/SliderElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_MK2/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_MK2/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_MK2/consts.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_MK2/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Mini_MK3/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Mini_MK3/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Mini_MK3/elements.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Mini_MK3/elements.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Mini_MK3/launchpad_mini_mk3.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Mini_MK3/launchpad_mini_mk3.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Mini_MK3/notifying_background.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Mini_MK3/notifying_background.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Mini_MK3/skin.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Mini_MK3/skin.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/ActionsComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/ActionsComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/BackgroundComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/BackgroundComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/ClipActionsComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/ClipActionsComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/Colors.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/Colors.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/ConfigurableButtonElement.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/ConfigurableButtonElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/DeviceNavigationComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/DeviceNavigationComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/DrumGroupComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/DrumGroupComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/DrumGroupFinderComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/DrumGroupFinderComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/Launchpad_Pro.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/Launchpad_Pro.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/LedLightingComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/LedLightingComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/MultiButtonElement.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/MultiButtonElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/SkinDefault.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/SkinDefault.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/SlideComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/SlideComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/SliderElement.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/SliderElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/SpecialDeviceComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/SpecialDeviceComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/SpecialMidiMap.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/SpecialMidiMap.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/SpecialMixerComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/SpecialMixerComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/SpecialModesComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/SpecialModesComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/SpecialSessionComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/SpecialSessionComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/SpecialSessionRecordingComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/SpecialSessionRecordingComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/TargetTrackComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/TargetTrackComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/TranslationComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/TranslationComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/UserMatrixComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/UserMatrixComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro/consts.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro_MK3/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro_MK3/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro_MK3/channel_strip.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro_MK3/channel_strip.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro_MK3/control.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro_MK3/control.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro_MK3/drum_group.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro_MK3/drum_group.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro_MK3/elements.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro_MK3/elements.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro_MK3/launchpad_pro_mk3.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro_MK3/launchpad_pro_mk3.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro_MK3/mixer.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro_MK3/mixer.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro_MK3/session.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro_MK3/session.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro_MK3/simple_device.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro_MK3/simple_device.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro_MK3/skin.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro_MK3/skin.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro_MK3/sysex_ids.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro_MK3/sysex_ids.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_Pro_MK3/transport.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_Pro_MK3/transport.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_X/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_X/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_X/channel_strip.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_X/channel_strip.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_X/elements.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_X/elements.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_X/launchpad_x.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_X/launchpad_x.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_X/session_recording.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_X/session_recording.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Launchpad_X/skin.py` & `ableton-control-surface-scripts-0.0.2/src/Launchpad_X/skin.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MIDI_Mix/ControlElementUtils.py` & `ableton-control-surface-scripts-0.0.2/src/MIDI_Mix/ControlElementUtils.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MIDI_Mix/MIDI_Mix.py` & `ableton-control-surface-scripts-0.0.2/src/MIDI_Mix/MIDI_Mix.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MIDI_Mix/MixerComponent.py` & `ableton-control-surface-scripts-0.0.2/src/MIDI_Mix/MixerComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MIDI_Mix/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/MIDI_Mix/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPD18/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/MPD18/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPD18/config.py` & `ableton-control-surface-scripts-0.0.2/src/MPD18/config.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPD18/consts.py` & `ableton-control-surface-scripts-0.0.2/src/MPD18/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPD218/MPD218.py` & `ableton-control-surface-scripts-0.0.2/src/MPD218/MPD218.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPD218/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/MPD218/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPD226/MPD226.py` & `ableton-control-surface-scripts-0.0.2/src/MPD226/MPD226.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPD226/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/MPD226/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPD232/MPD232.py` & `ableton-control-surface-scripts-0.0.2/src/MPD232/MPD232.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPD232/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/MPD232/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPD24/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/MPD24/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPD24/config.py` & `ableton-control-surface-scripts-0.0.2/src/MPD24/config.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPD24/consts.py` & `ableton-control-surface-scripts-0.0.2/src/MPD24/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPD32/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/MPD32/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPD32/config.py` & `ableton-control-surface-scripts-0.0.2/src/MPD32/config.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPD32/consts.py` & `ableton-control-surface-scripts-0.0.2/src/MPD32/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPK225/MPK225.py` & `ableton-control-surface-scripts-0.0.2/src/MPK225/MPK225.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPK225/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/MPK225/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPK249/MPK249.py` & `ableton-control-surface-scripts-0.0.2/src/MPK249/MPK249.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPK249/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/MPK249/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPK25/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/MPK25/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPK25/config.py` & `ableton-control-surface-scripts-0.0.2/src/MPK25/config.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPK25/consts.py` & `ableton-control-surface-scripts-0.0.2/src/MPK25/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPK261/MPK261.py` & `ableton-control-surface-scripts-0.0.2/src/MPK261/MPK261.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPK261/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/MPK261/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPK49/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/MPK49/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPK49/config.py` & `ableton-control-surface-scripts-0.0.2/src/MPK49/config.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPK49/consts.py` & `ableton-control-surface-scripts-0.0.2/src/MPK49/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPK61/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/MPK61/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPK61/config.py` & `ableton-control-surface-scripts-0.0.2/src/MPK61/config.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPK61/consts.py` & `ableton-control-surface-scripts-0.0.2/src/MPK61/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPK88/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/MPK88/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPK88/config.py` & `ableton-control-surface-scripts-0.0.2/src/MPK88/config.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPK88/consts.py` & `ableton-control-surface-scripts-0.0.2/src/MPK88/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPK_mini_mkI/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/MPK_mini_mkI/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPK_mini_mkI/config.py` & `ableton-control-surface-scripts-0.0.2/src/MPK_mini_mkI/config.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPK_mini_mkI/consts.py` & `ableton-control-surface-scripts-0.0.2/src/MPK_mini_mkI/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPK_mini_mkII/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/MPK_mini_mkII/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPK_mini_mkII/config.py` & `ableton-control-surface-scripts-0.0.2/src/MPK_mini_mkII/config.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPK_mini_mkII/consts.py` & `ableton-control-surface-scripts-0.0.2/src/MPK_mini_mkII/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPK_mini_mkIII/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/MPK_mini_mkIII/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPK_mini_mkIII/config.py` & `ableton-control-surface-scripts-0.0.2/src/MPK_mini_mkIII/config.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MPK_mini_mkIII/consts.py` & `ableton-control-surface-scripts-0.0.2/src/MPK_mini_mkIII/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MackieControl/ChannelStrip.py` & `ableton-control-surface-scripts-0.0.2/src/MackieControl/ChannelStrip.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MackieControl/ChannelStripController.py` & `ableton-control-surface-scripts-0.0.2/src/MackieControl/ChannelStripController.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MackieControl/MackieControl.py` & `ableton-control-surface-scripts-0.0.2/src/MackieControl/MackieControl.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MackieControl/MackieControlComponent.py` & `ableton-control-surface-scripts-0.0.2/src/MackieControl/MackieControlComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MackieControl/MainDisplay.py` & `ableton-control-surface-scripts-0.0.2/src/MackieControl/MainDisplay.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MackieControl/MainDisplayController.py` & `ableton-control-surface-scripts-0.0.2/src/MackieControl/MainDisplayController.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MackieControl/SoftwareController.py` & `ableton-control-surface-scripts-0.0.2/src/MackieControl/SoftwareController.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MackieControl/TimeDisplay.py` & `ableton-control-surface-scripts-0.0.2/src/MackieControl/TimeDisplay.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MackieControl/Transport.py` & `ableton-control-surface-scripts-0.0.2/src/MackieControl/Transport.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MackieControl/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/MackieControl/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MackieControl/consts.py` & `ableton-control-surface-scripts-0.0.2/src/MackieControl/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MackieControlXT/MackieControlXT.py` & `ableton-control-surface-scripts-0.0.2/src/MackieControlXT/MackieControlXT.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MackieControl_Classic/ChannelStrip.py` & `ableton-control-surface-scripts-0.0.2/src/MackieControl_Classic/ChannelStrip.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MackieControl_Classic/ChannelStripController.py` & `ableton-control-surface-scripts-0.0.2/src/MackieControl_Classic/ChannelStripController.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MackieControl_Classic/MackieControl.py` & `ableton-control-surface-scripts-0.0.2/src/MackieControl_Classic/MackieControl.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MackieControl_Classic/MackieControlComponent.py` & `ableton-control-surface-scripts-0.0.2/src/MackieControl_Classic/MackieControlComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MackieControl_Classic/MainDisplay.py` & `ableton-control-surface-scripts-0.0.2/src/MackieControl_Classic/MainDisplay.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MackieControl_Classic/MainDisplayController.py` & `ableton-control-surface-scripts-0.0.2/src/MackieControl_Classic/MainDisplayController.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MackieControl_Classic/SoftwareController.py` & `ableton-control-surface-scripts-0.0.2/src/MackieControl_Classic/SoftwareController.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MackieControl_Classic/TimeDisplay.py` & `ableton-control-surface-scripts-0.0.2/src/MackieControl_Classic/TimeDisplay.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MackieControl_Classic/Transport.py` & `ableton-control-surface-scripts-0.0.2/src/MackieControl_Classic/Transport.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MackieControl_Classic/consts.py` & `ableton-control-surface-scripts-0.0.2/src/MackieControl_Classic/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MasterControl/MasterControl.py` & `ableton-control-surface-scripts-0.0.2/src/MasterControl/MasterControl.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MaxForLive/MaxForLive.py` & `ableton-control-surface-scripts-0.0.2/src/MaxForLive/MaxForLive.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MaxForLive/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/MaxForLive/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MidAir25/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/MidAir25/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MidAir25/config.py` & `ableton-control-surface-scripts-0.0.2/src/MidAir25/config.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MidAir25/consts.py` & `ableton-control-surface-scripts-0.0.2/src/MidAir25/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MiniLab/MiniLab.py` & `ableton-control-surface-scripts-0.0.2/src/MiniLab/MiniLab.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MiniLab/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/MiniLab/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MiniLab_3/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/MiniLab_3/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MiniLab_3/analog_lab.py` & `ableton-control-surface-scripts-0.0.2/src/MiniLab_3/analog_lab.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MiniLab_3/colors.py` & `ableton-control-surface-scripts-0.0.2/src/MiniLab_3/colors.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MiniLab_3/display.py` & `ableton-control-surface-scripts-0.0.2/src/MiniLab_3/display.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MiniLab_3/display_util.py` & `ableton-control-surface-scripts-0.0.2/src/MiniLab_3/display_util.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MiniLab_3/drum_group.py` & `ableton-control-surface-scripts-0.0.2/src/MiniLab_3/drum_group.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MiniLab_3/elements.py` & `ableton-control-surface-scripts-0.0.2/src/MiniLab_3/elements.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MiniLab_3/encoder.py` & `ableton-control-surface-scripts-0.0.2/src/MiniLab_3/encoder.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MiniLab_3/mappings.py` & `ableton-control-surface-scripts-0.0.2/src/MiniLab_3/mappings.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MiniLab_3/midi.py` & `ableton-control-surface-scripts-0.0.2/src/MiniLab_3/midi.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MiniLab_3/sysex.py` & `ableton-control-surface-scripts-0.0.2/src/MiniLab_3/sysex.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MiniLab_3/transport.py` & `ableton-control-surface-scripts-0.0.2/src/MiniLab_3/transport.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MiniLab_mkII/HardwareSettingsComponent.py` & `ableton-control-surface-scripts-0.0.2/src/MiniLab_mkII/HardwareSettingsComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MiniLab_mkII/MiniLabMk2.py` & `ableton-control-surface-scripts-0.0.2/src/MiniLab_mkII/MiniLabMk2.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MiniLab_mkII/SessionComponent.py` & `ableton-control-surface-scripts-0.0.2/src/MiniLab_mkII/SessionComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/MiniLab_mkII/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/MiniLab_mkII/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Novation_Impulse/EncoderModeSelector.py` & `ableton-control-surface-scripts-0.0.2/src/Novation_Impulse/EncoderModeSelector.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Novation_Impulse/Novation_Impulse.py` & `ableton-control-surface-scripts-0.0.2/src/Novation_Impulse/Novation_Impulse.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Novation_Impulse/PeekableEncoderElement.py` & `ableton-control-surface-scripts-0.0.2/src/Novation_Impulse/PeekableEncoderElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Novation_Impulse/ShiftableTransportComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Novation_Impulse/ShiftableTransportComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Novation_Impulse/SpecialMixerComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Novation_Impulse/SpecialMixerComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Novation_Impulse/TransportViewModeSelector.py` & `ableton-control-surface-scripts-0.0.2/src/Novation_Impulse/TransportViewModeSelector.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Novation_Impulse/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Novation_Impulse/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/O2/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/O2/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/O2/config.py` & `ableton-control-surface-scripts-0.0.2/src/O2/config.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/O2/consts.py` & `ableton-control-surface-scripts-0.0.2/src/O2/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/OpenLabs/OpenLabs.py` & `ableton-control-surface-scripts-0.0.2/src/OpenLabs/OpenLabs.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/OpenLabs/SpecialDeviceComponent.py` & `ableton-control-surface-scripts-0.0.2/src/OpenLabs/SpecialDeviceComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/OpenLabs/SpecialTransportComponent.py` & `ableton-control-surface-scripts-0.0.2/src/OpenLabs/SpecialTransportComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Oxygen49_61/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Oxygen49_61/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Oxygen49_61/config.py` & `ableton-control-surface-scripts-0.0.2/src/Oxygen49_61/config.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Oxygen49_61/consts.py` & `ableton-control-surface-scripts-0.0.2/src/Oxygen49_61/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Oxygen8/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Oxygen8/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Oxygen8/config.py` & `ableton-control-surface-scripts-0.0.2/src/Oxygen8/config.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Oxygen8/consts.py` & `ableton-control-surface-scripts-0.0.2/src/Oxygen8/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Oxygen8v2/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Oxygen8v2/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Oxygen8v2/config.py` & `ableton-control-surface-scripts-0.0.2/src/Oxygen8v2/config.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Oxygen8v2/consts.py` & `ableton-control-surface-scripts-0.0.2/src/Oxygen8v2/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Oxygen_3rd_Gen/Oxygen_3rd_Gen.py` & `ableton-control-surface-scripts-0.0.2/src/Oxygen_3rd_Gen/Oxygen_3rd_Gen.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Oxygen_3rd_Gen/SpecialMixerComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Oxygen_3rd_Gen/SpecialMixerComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Oxygen_3rd_Gen/TransportViewModeSelector.py` & `ableton-control-surface-scripts-0.0.2/src/Oxygen_3rd_Gen/TransportViewModeSelector.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Oxygen_5th_Gen/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Oxygen_5th_Gen/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Oxygen_5th_Gen/oxygen_5th_gen.py` & `ableton-control-surface-scripts-0.0.2/src/Oxygen_5th_Gen/oxygen_5th_gen.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Oxygen_Pro/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Oxygen_Pro/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Oxygen_Pro/channel_strip.py` & `ableton-control-surface-scripts-0.0.2/src/Oxygen_Pro/channel_strip.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Oxygen_Pro/colors.py` & `ableton-control-surface-scripts-0.0.2/src/Oxygen_Pro/colors.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Oxygen_Pro/elements.py` & `ableton-control-surface-scripts-0.0.2/src/Oxygen_Pro/elements.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Oxygen_Pro/midi.py` & `ableton-control-surface-scripts-0.0.2/src/Oxygen_Pro/midi.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Oxygen_Pro/mode.py` & `ableton-control-surface-scripts-0.0.2/src/Oxygen_Pro/mode.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Oxygen_Pro/oxygen_pro.py` & `ableton-control-surface-scripts-0.0.2/src/Oxygen_Pro/oxygen_pro.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Oxygen_Pro/session.py` & `ableton-control-surface-scripts-0.0.2/src/Oxygen_Pro/session.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Oxygen_Pro/session_navigation.py` & `ableton-control-surface-scripts-0.0.2/src/Oxygen_Pro/session_navigation.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Oxygen_Pro/skin.py` & `ableton-control-surface-scripts-0.0.2/src/Oxygen_Pro/skin.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Oxygen_Pro_Mini/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Oxygen_Pro_Mini/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Oxygen_Pro_Mini/oxygen_pro_mini.py` & `ableton-control-surface-scripts-0.0.2/src/Oxygen_Pro_Mini/oxygen_pro_mini.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Oxygen_Pro_Mini/simple_device.py` & `ableton-control-surface-scripts-0.0.2/src/Oxygen_Pro_Mini/simple_device.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Ozone/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Ozone/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Ozone/config.py` & `ableton-control-surface-scripts-0.0.2/src/Ozone/config.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Ozone/consts.py` & `ableton-control-surface-scripts-0.0.2/src/Ozone/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Ozonic/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Ozonic/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Ozonic/config.py` & `ableton-control-surface-scripts-0.0.2/src/Ozonic/config.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Ozonic/consts.py` & `ableton-control-surface-scripts-0.0.2/src/Ozonic/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Photon_25/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Photon_25/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Photon_25/config.py` & `ableton-control-surface-scripts-0.0.2/src/Photon_25/config.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Photon_25/consts.py` & `ableton-control-surface-scripts-0.0.2/src/Photon_25/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Photon_X25/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Photon_X25/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Photon_X25/config.py` & `ableton-control-surface-scripts-0.0.2/src/Photon_X25/config.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Photon_X25/consts.py` & `ableton-control-surface-scripts-0.0.2/src/Photon_X25/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/ProjectMixIO/ProjectMixIO.py` & `ableton-control-surface-scripts-0.0.2/src/ProjectMixIO/ProjectMixIO.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Push/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push/actions.py` & `ableton-control-surface-scripts-0.0.2/src/Push/actions.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push/browser_component.py` & `ableton-control-surface-scripts-0.0.2/src/Push/browser_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push/browser_model.py` & `ableton-control-surface-scripts-0.0.2/src/Push/browser_model.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push/browser_model_factory.py` & `ableton-control-surface-scripts-0.0.2/src/Push/browser_model_factory.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push/browser_query.py` & `ableton-control-surface-scripts-0.0.2/src/Push/browser_query.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push/device_component.py` & `ableton-control-surface-scripts-0.0.2/src/Push/device_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push/device_navigation_component.py` & `ableton-control-surface-scripts-0.0.2/src/Push/device_navigation_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push/drum_group_component.py` & `ableton-control-surface-scripts-0.0.2/src/Push/drum_group_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push/elements.py` & `ableton-control-surface-scripts-0.0.2/src/Push/elements.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push/firmware_handling.py` & `ableton-control-surface-scripts-0.0.2/src/Push/firmware_handling.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push/global_pad_parameters.py` & `ableton-control-surface-scripts-0.0.2/src/Push/global_pad_parameters.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push/handshake_component.py` & `ableton-control-surface-scripts-0.0.2/src/Push/handshake_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push/mode_behaviours.py` & `ableton-control-surface-scripts-0.0.2/src/Push/mode_behaviours.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push/multi_entry_mode.py` & `ableton-control-surface-scripts-0.0.2/src/Push/multi_entry_mode.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push/navigation_node.py` & `ableton-control-surface-scripts-0.0.2/src/Push/navigation_node.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push/notification_component.py` & `ableton-control-surface-scripts-0.0.2/src/Push/notification_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push/pad_sensitivity.py` & `ableton-control-surface-scripts-0.0.2/src/Push/pad_sensitivity.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push/parameter_mapping_sensitivities.py` & `ableton-control-surface-scripts-0.0.2/src/Push/parameter_mapping_sensitivities.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push/push.py` & `ableton-control-surface-scripts-0.0.2/src/Push/push.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push/quantization_settings.py` & `ableton-control-surface-scripts-0.0.2/src/Push/quantization_settings.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push/scales_component.py` & `ableton-control-surface-scripts-0.0.2/src/Push/scales_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push/selected_track_parameter_provider.py` & `ableton-control-surface-scripts-0.0.2/src/Push/selected_track_parameter_provider.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push/settings.py` & `ableton-control-surface-scripts-0.0.2/src/Push/settings.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push/special_chan_strip_component.py` & `ableton-control-surface-scripts-0.0.2/src/Push/special_chan_strip_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push/special_mixer_component.py` & `ableton-control-surface-scripts-0.0.2/src/Push/special_mixer_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push/special_physical_display.py` & `ableton-control-surface-scripts-0.0.2/src/Push/special_physical_display.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push/sysex.py` & `ableton-control-surface-scripts-0.0.2/src/Push/sysex.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push/user_settings_component.py` & `ableton-control-surface-scripts-0.0.2/src/Push/user_settings_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push/with_priority.py` & `ableton-control-surface-scripts-0.0.2/src/Push/with_priority.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/actions.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/actions.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/amp.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/amp.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/analog.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/analog.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/auto_filter.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/auto_filter.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/automation.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/automation.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/bank_selection_component.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/bank_selection_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/beatrepeat.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/beatrepeat.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/browser_component.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/browser_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/browser_item.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/browser_item.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/browser_list.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/browser_list.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/browser_modes.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/browser_modes.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/cccontrol.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/cccontrol.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/chain_selection_component.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/chain_selection_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/channel_eq.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/channel_eq.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/chorus2.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/chorus2.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/clip_control.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/clip_control.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/clip_decoration.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/clip_decoration.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/collision.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/collision.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/color_chooser.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/color_chooser.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/colors.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/colors.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/compressor.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/compressor.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/convert.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/convert.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/corpus.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/corpus.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/custom_bank_definitions.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/custom_bank_definitions.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/decoration.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/decoration.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/delay.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/delay.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/device_component.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/device_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/device_component_provider.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/device_component_provider.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/device_decoration.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/device_decoration.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/device_decorator_factory.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/device_decorator_factory.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/device_navigation.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/device_navigation.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/device_options.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/device_options.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/device_parameter_bank_with_options.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/device_parameter_bank_with_options.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/device_parameter_icons.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/device_parameter_icons.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/device_util.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/device_util.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/device_view_component.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/device_view_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/drift.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/drift.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/drum_group_component.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/drum_group_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/drum_pad_parameter_component.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/drum_pad_parameter_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/drumcell.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/drumcell.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/echo.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/echo.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/elements.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/elements.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/eq3.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/eq3.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/eq8.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/eq8.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/filterdelay.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/filterdelay.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/firmware.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/firmware.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/graindelay.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/graindelay.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/hardware_settings_component.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/hardware_settings_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/hybrid_reverb.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/hybrid_reverb.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/item_lister.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/item_lister.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/master_track.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/master_track.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/meld.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/meld.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/mixable_utilities.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/mixable_utilities.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/mixer_control_component.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/mixer_control_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/mode_collector.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/mode_collector.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/model/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/model/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/model/declaration.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/model/declaration.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/model/generation.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/model/generation.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/model/repr.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/model/repr.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/model/uniqueid.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/model/uniqueid.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/mute_solo_stop.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/mute_solo_stop.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/note_editor.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/note_editor.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/note_settings.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/note_settings.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/notification_component.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/notification_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/operator.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/operator.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/pad_sensitivity.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/pad_sensitivity.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/pad_velocity_curve.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/pad_velocity_curve.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/parameter_mapping_sensitivities.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/parameter_mapping_sensitivities.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/phasernew.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/phasernew.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/push2.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/push2.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/push2_model.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/push2_model.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/real_time_channel.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/real_time_channel.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/redux2.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/redux2.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/resonator.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/resonator.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/reverb.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/reverb.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/roar.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/roar.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/routing.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/routing.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/saturator.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/saturator.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/scales_component.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/scales_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/selected_track_parameter_provider.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/selected_track_parameter_provider.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/session_component.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/session_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/session_ring_selection_linking.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/session_ring_selection_linking.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/settings.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/settings.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/setup_component.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/setup_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/shifter.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/shifter.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/simple_mode_switcher.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/simple_mode_switcher.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/simpler.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/simpler.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/skin_default.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/skin_default.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/sliced_simpler.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/sliced_simpler.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/spectral.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/spectral.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/sysex.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/sysex.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/tension.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/tension.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/timeline_navigation.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/timeline_navigation.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/track_list.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/track_list.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/track_mixer_control_component.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/track_mixer_control_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/track_selection.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/track_selection.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/transmute.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/transmute.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/transport_state.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/transport_state.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/user_component.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/user_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/vinyl.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/vinyl.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/visualisation_settings.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/visualisation_settings.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Push2/wavetable.py` & `ableton-control-surface-scripts-0.0.2/src/Push2/wavetable.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Radium49_61/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Radium49_61/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Radium49_61/config.py` & `ableton-control-surface-scripts-0.0.2/src/Radium49_61/config.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Radium49_61/consts.py` & `ableton-control-surface-scripts-0.0.2/src/Radium49_61/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/RemoteSL/DisplayController.py` & `ableton-control-surface-scripts-0.0.2/src/RemoteSL/DisplayController.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/RemoteSL/EffectController.py` & `ableton-control-surface-scripts-0.0.2/src/RemoteSL/EffectController.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/RemoteSL/MixerController.py` & `ableton-control-surface-scripts-0.0.2/src/RemoteSL/MixerController.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/RemoteSL/RemoteSL.py` & `ableton-control-surface-scripts-0.0.2/src/RemoteSL/RemoteSL.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/RemoteSL/RemoteSLComponent.py` & `ableton-control-surface-scripts-0.0.2/src/RemoteSL/RemoteSLComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/RemoteSL/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/RemoteSL/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/RemoteSL/consts.py` & `ableton-control-surface-scripts-0.0.2/src/RemoteSL/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/RemoteSL_Classic/DisplayController.py` & `ableton-control-surface-scripts-0.0.2/src/RemoteSL_Classic/DisplayController.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/RemoteSL_Classic/EffectController.py` & `ableton-control-surface-scripts-0.0.2/src/RemoteSL_Classic/EffectController.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/RemoteSL_Classic/MixerController.py` & `ableton-control-surface-scripts-0.0.2/src/RemoteSL_Classic/MixerController.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/RemoteSL_Classic/RemoteSL.py` & `ableton-control-surface-scripts-0.0.2/src/RemoteSL_Classic/RemoteSL.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/RemoteSL_Classic/RemoteSLComponent.py` & `ableton-control-surface-scripts-0.0.2/src/RemoteSL_Classic/RemoteSLComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/RemoteSL_Classic/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/RemoteSL_Classic/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/RemoteSL_Classic/consts.py` & `ableton-control-surface-scripts-0.0.2/src/RemoteSL_Classic/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Roland_A_PRO/DeviceNavigationComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Roland_A_PRO/DeviceNavigationComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Roland_A_PRO/MixerComponent.py` & `ableton-control-surface-scripts-0.0.2/src/Roland_A_PRO/MixerComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Roland_A_PRO/Roland_A_PRO.py` & `ableton-control-surface-scripts-0.0.2/src/Roland_A_PRO/Roland_A_PRO.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Roland_A_PRO/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Roland_A_PRO/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Roland_FA/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/Roland_FA/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Roland_FA/control_element_utils.py` & `ableton-control-surface-scripts-0.0.2/src/Roland_FA/control_element_utils.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Roland_FA/fa.py` & `ableton-control-surface-scripts-0.0.2/src/Roland_FA/fa.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Roland_FA/navigation.py` & `ableton-control-surface-scripts-0.0.2/src/Roland_FA/navigation.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Roland_FA/scroll.py` & `ableton-control-surface-scripts-0.0.2/src/Roland_FA/scroll.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Roland_FA/skin.py` & `ableton-control-surface-scripts-0.0.2/src/Roland_FA/skin.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Roland_FA/transport.py` & `ableton-control-surface-scripts-0.0.2/src/Roland_FA/transport.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/SL_MkIII/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/SL_MkIII/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/SL_MkIII/actions.py` & `ableton-control-surface-scripts-0.0.2/src/SL_MkIII/actions.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/SL_MkIII/caching_control_element.py` & `ableton-control-surface-scripts-0.0.2/src/SL_MkIII/caching_control_element.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/SL_MkIII/channel_strip.py` & `ableton-control-surface-scripts-0.0.2/src/SL_MkIII/channel_strip.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/SL_MkIII/color_sysex_element.py` & `ableton-control-surface-scripts-0.0.2/src/SL_MkIII/color_sysex_element.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/SL_MkIII/control.py` & `ableton-control-surface-scripts-0.0.2/src/SL_MkIII/control.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/SL_MkIII/device.py` & `ableton-control-surface-scripts-0.0.2/src/SL_MkIII/device.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/SL_MkIII/device_navigation.py` & `ableton-control-surface-scripts-0.0.2/src/SL_MkIII/device_navigation.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/SL_MkIII/device_parameters.py` & `ableton-control-surface-scripts-0.0.2/src/SL_MkIII/device_parameters.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/SL_MkIII/drum_group.py` & `ableton-control-surface-scripts-0.0.2/src/SL_MkIII/drum_group.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/SL_MkIII/elements.py` & `ableton-control-surface-scripts-0.0.2/src/SL_MkIII/elements.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/SL_MkIII/message.py` & `ableton-control-surface-scripts-0.0.2/src/SL_MkIII/message.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/SL_MkIII/midi_message_cache.py` & `ableton-control-surface-scripts-0.0.2/src/SL_MkIII/midi_message_cache.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/SL_MkIII/mixer.py` & `ableton-control-surface-scripts-0.0.2/src/SL_MkIII/mixer.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/SL_MkIII/mode.py` & `ableton-control-surface-scripts-0.0.2/src/SL_MkIII/mode.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/SL_MkIII/parameter_mapping_sensitivities.py` & `ableton-control-surface-scripts-0.0.2/src/SL_MkIII/parameter_mapping_sensitivities.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/SL_MkIII/physical_display.py` & `ableton-control-surface-scripts-0.0.2/src/SL_MkIII/physical_display.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/SL_MkIII/session.py` & `ableton-control-surface-scripts-0.0.2/src/SL_MkIII/session.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/SL_MkIII/session_navigation.py` & `ableton-control-surface-scripts-0.0.2/src/SL_MkIII/session_navigation.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/SL_MkIII/session_ring_selection_linking.py` & `ableton-control-surface-scripts-0.0.2/src/SL_MkIII/session_ring_selection_linking.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/SL_MkIII/skin.py` & `ableton-control-surface-scripts-0.0.2/src/SL_MkIII/skin.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/SL_MkIII/sl_mkiii.py` & `ableton-control-surface-scripts-0.0.2/src/SL_MkIII/sl_mkiii.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/SL_MkIII/sysex.py` & `ableton-control-surface-scripts-0.0.2/src/SL_MkIII/sysex.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/SL_MkIII/transport.py` & `ableton-control-surface-scripts-0.0.2/src/SL_MkIII/transport.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/SL_MkIII/util.py` & `ableton-control-surface-scripts-0.0.2/src/SL_MkIII/util.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Tranzport/Tranzport.py` & `ableton-control-surface-scripts-0.0.2/src/Tranzport/Tranzport.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/Tranzport/consts.py` & `ableton-control-surface-scripts-0.0.2/src/Tranzport/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/TriggerFinger/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/TriggerFinger/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/TriggerFinger/config.py` & `ableton-control-surface-scripts-0.0.2/src/TriggerFinger/config.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/TriggerFinger/consts.py` & `ableton-control-surface-scripts-0.0.2/src/TriggerFinger/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/UC33e/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/UC33e/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/UC33e/config.py` & `ableton-control-surface-scripts-0.0.2/src/UC33e/config.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/UC33e/consts.py` & `ableton-control-surface-scripts-0.0.2/src/UC33e/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/VCM600/MixerComponent.py` & `ableton-control-surface-scripts-0.0.2/src/VCM600/MixerComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/VCM600/TrackEQComponent.py` & `ableton-control-surface-scripts-0.0.2/src/VCM600/TrackEQComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/VCM600/TrackFilterComponent.py` & `ableton-control-surface-scripts-0.0.2/src/VCM600/TrackFilterComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/VCM600/TransportComponent.py` & `ableton-control-surface-scripts-0.0.2/src/VCM600/TransportComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/VCM600/VCM600.py` & `ableton-control-surface-scripts-0.0.2/src/VCM600/VCM600.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/VCM600/ViewTogglerComponent.py` & `ableton-control-surface-scripts-0.0.2/src/VCM600/ViewTogglerComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/VCM600/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/VCM600/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/ZERO8/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/ZERO8/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/ZERO8/config.py` & `ableton-control-surface-scripts-0.0.2/src/ZERO8/config.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/ZERO8/consts.py` & `ableton-control-surface-scripts-0.0.2/src/ZERO8/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/_APC/APC.py` & `ableton-control-surface-scripts-0.0.2/src/_APC/APC.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/_APC/ControlElementUtils.py` & `ableton-control-surface-scripts-0.0.2/src/_APC/ControlElementUtils.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/_APC/DetailViewCntrlComponent.py` & `ableton-control-surface-scripts-0.0.2/src/_APC/DetailViewCntrlComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/_APC/DeviceBankButtonElement.py` & `ableton-control-surface-scripts-0.0.2/src/_APC/DeviceBankButtonElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/_APC/DeviceComponent.py` & `ableton-control-surface-scripts-0.0.2/src/_APC/DeviceComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/_APC/MixerComponent.py` & `ableton-control-surface-scripts-0.0.2/src/_APC/MixerComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/_APC/RingedEncoderElement.py` & `ableton-control-surface-scripts-0.0.2/src/_APC/RingedEncoderElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/_APC/SessionComponent.py` & `ableton-control-surface-scripts-0.0.2/src/_APC/SessionComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/_APC/SkinDefault.py` & `ableton-control-surface-scripts-0.0.2/src/_APC/SkinDefault.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/_Arturia/ArturiaControlSurface.py` & `ableton-control-surface-scripts-0.0.2/src/_Arturia/ArturiaControlSurface.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/_Arturia/MixerComponent.py` & `ableton-control-surface-scripts-0.0.2/src/_Arturia/MixerComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/_Arturia/ScrollComponent.py` & `ableton-control-surface-scripts-0.0.2/src/_Arturia/ScrollComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/_Arturia/SessionComponent.py` & `ableton-control-surface-scripts-0.0.2/src/_Arturia/SessionComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/_Axiom/Encoders.py` & `ableton-control-surface-scripts-0.0.2/src/_Axiom/Encoders.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/_Axiom/Pads.py` & `ableton-control-surface-scripts-0.0.2/src/_Axiom/Pads.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/_Axiom/Transport.py` & `ableton-control-surface-scripts-0.0.2/src/_Axiom/Transport.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/_Axiom/consts.py` & `ableton-control-surface-scripts-0.0.2/src/_Axiom/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/_Komplete_Kontrol/channel_strip_component.py` & `ableton-control-surface-scripts-0.0.2/src/_Komplete_Kontrol/channel_strip_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/_Komplete_Kontrol/clip_launch_component.py` & `ableton-control-surface-scripts-0.0.2/src/_Komplete_Kontrol/clip_launch_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/_Komplete_Kontrol/control_element_util.py` & `ableton-control-surface-scripts-0.0.2/src/_Komplete_Kontrol/control_element_util.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/_Komplete_Kontrol/detail_clip_component.py` & `ableton-control-surface-scripts-0.0.2/src/_Komplete_Kontrol/detail_clip_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/_Komplete_Kontrol/focus_follow_component.py` & `ableton-control-surface-scripts-0.0.2/src/_Komplete_Kontrol/focus_follow_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/_Komplete_Kontrol/komplete_kontrol_base.py` & `ableton-control-surface-scripts-0.0.2/src/_Komplete_Kontrol/komplete_kontrol_base.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/_Komplete_Kontrol/mixer_component.py` & `ableton-control-surface-scripts-0.0.2/src/_Komplete_Kontrol/mixer_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/_Komplete_Kontrol/physical_display_element.py` & `ableton-control-surface-scripts-0.0.2/src/_Komplete_Kontrol/physical_display_element.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/_Komplete_Kontrol/selection_linked_session_ring_component.py` & `ableton-control-surface-scripts-0.0.2/src/_Komplete_Kontrol/selection_linked_session_ring_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/_Komplete_Kontrol/skin.py` & `ableton-control-surface-scripts-0.0.2/src/_Komplete_Kontrol/skin.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/_Komplete_Kontrol/sysex.py` & `ableton-control-surface-scripts-0.0.2/src/_Komplete_Kontrol/sysex.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/_Komplete_Kontrol/transport_component.py` & `ableton-control-surface-scripts-0.0.2/src/_Komplete_Kontrol/transport_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/_MPDMkIIBase/ControlElementUtils.py` & `ableton-control-surface-scripts-0.0.2/src/_MPDMkIIBase/ControlElementUtils.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/_MPDMkIIBase/MPDMkIIBase.py` & `ableton-control-surface-scripts-0.0.2/src/_MPDMkIIBase/MPDMkIIBase.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/ableton_control_surface_scripts.egg-info/SOURCES.txt` & `ableton-control-surface-scripts-0.0.2/src/ableton_control_surface_scripts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/ableton_control_surface_scripts.egg-info/top_level.txt` & `ableton-control-surface-scripts-0.0.2/src/ableton_control_surface_scripts.egg-info/top_level.txt`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/iRig_Keys_IO/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/iRig_Keys_IO/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/iRig_Keys_IO/irig_keys_io.py` & `ableton-control-surface-scripts-0.0.2/src/iRig_Keys_IO/irig_keys_io.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/iRig_Keys_IO/mixer.py` & `ableton-control-surface-scripts-0.0.2/src/iRig_Keys_IO/mixer.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/iRig_Keys_IO/scroll.py` & `ableton-control-surface-scripts-0.0.2/src/iRig_Keys_IO/scroll.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/iRig_Keys_IO/session_recording.py` & `ableton-control-surface-scripts-0.0.2/src/iRig_Keys_IO/session_recording.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/iRig_Keys_IO/session_ring.py` & `ableton-control-surface-scripts-0.0.2/src/iRig_Keys_IO/session_ring.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/iRig_Keys_IO/skin.py` & `ableton-control-surface-scripts-0.0.2/src/iRig_Keys_IO/skin.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/microKONTROL/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/microKONTROL/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/microKONTROL/config.py` & `ableton-control-surface-scripts-0.0.2/src/microKONTROL/config.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/microKONTROL/consts.py` & `ableton-control-surface-scripts-0.0.2/src/microKONTROL/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/novation/blinking_button.py` & `ableton-control-surface-scripts-0.0.2/src/novation/blinking_button.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/novation/channel_strip.py` & `ableton-control-surface-scripts-0.0.2/src/novation/channel_strip.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/novation/clip_actions.py` & `ableton-control-surface-scripts-0.0.2/src/novation/clip_actions.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/novation/clip_slot.py` & `ableton-control-surface-scripts-0.0.2/src/novation/clip_slot.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/novation/colors.py` & `ableton-control-surface-scripts-0.0.2/src/novation/colors.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/novation/configurable_playable.py` & `ableton-control-surface-scripts-0.0.2/src/novation/configurable_playable.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/novation/drum_group.py` & `ableton-control-surface-scripts-0.0.2/src/novation/drum_group.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/novation/fixed_length.py` & `ableton-control-surface-scripts-0.0.2/src/novation/fixed_length.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/novation/fixed_length_recording.py` & `ableton-control-surface-scripts-0.0.2/src/novation/fixed_length_recording.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/novation/fixed_radio_button_group.py` & `ableton-control-surface-scripts-0.0.2/src/novation/fixed_radio_button_group.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/novation/instrument_control.py` & `ableton-control-surface-scripts-0.0.2/src/novation/instrument_control.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/novation/launchkey_drum_group.py` & `ableton-control-surface-scripts-0.0.2/src/novation/launchkey_drum_group.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/novation/launchkey_elements.py` & `ableton-control-surface-scripts-0.0.2/src/novation/launchkey_elements.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/novation/launchpad_elements.py` & `ableton-control-surface-scripts-0.0.2/src/novation/launchpad_elements.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/novation/mixer.py` & `ableton-control-surface-scripts-0.0.2/src/novation/mixer.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/novation/mode.py` & `ableton-control-surface-scripts-0.0.2/src/novation/mode.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/novation/novation_base.py` & `ableton-control-surface-scripts-0.0.2/src/novation/novation_base.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/novation/print_to_clip.py` & `ableton-control-surface-scripts-0.0.2/src/novation/print_to_clip.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/novation/quantization.py` & `ableton-control-surface-scripts-0.0.2/src/novation/quantization.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/novation/session_modes.py` & `ableton-control-surface-scripts-0.0.2/src/novation/session_modes.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/novation/session_navigation.py` & `ableton-control-surface-scripts-0.0.2/src/novation/session_navigation.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/novation/simple_device.py` & `ableton-control-surface-scripts-0.0.2/src/novation/simple_device.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/novation/simple_device_navigation.py` & `ableton-control-surface-scripts-0.0.2/src/novation/simple_device_navigation.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/novation/skin.py` & `ableton-control-surface-scripts-0.0.2/src/novation/skin.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/novation/sysex.py` & `ableton-control-surface-scripts-0.0.2/src/novation/sysex.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/novation/track_recording.py` & `ableton-control-surface-scripts-0.0.2/src/novation/track_recording.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/novation/transport.py` & `ableton-control-surface-scripts-0.0.2/src/novation/transport.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/novation/util.py` & `ableton-control-surface-scripts-0.0.2/src/novation/util.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/novation/view_control.py` & `ableton-control-surface-scripts-0.0.2/src/novation/view_control.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/padKONTROL/__init__.py` & `ableton-control-surface-scripts-0.0.2/src/padKONTROL/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/padKONTROL/config.py` & `ableton-control-surface-scripts-0.0.2/src/padKONTROL/config.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/padKONTROL/consts.py` & `ableton-control-surface-scripts-0.0.2/src/padKONTROL/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/action_with_options_component.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/action_with_options_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/actions.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/actions.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/auto_arm_component.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/auto_arm_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/automation_component.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/automation_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/browser_modes.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/browser_modes.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/browser_util.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/browser_util.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/clip_control_component.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/clip_control_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/colors.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/colors.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/consts.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/control_element_factory.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/control_element_factory.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/device_chain_utils.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/device_chain_utils.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/device_parameter_component.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/device_parameter_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/drum_group_component.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/drum_group_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/elements.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/elements.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/fixed_length.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/fixed_length.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/grid_resolution.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/grid_resolution.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/instrument_component.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/instrument_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/internal_parameter.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/internal_parameter.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/loop_selector_component.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/loop_selector_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/matrix_maps.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/matrix_maps.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/melodic_component.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/melodic_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/melodic_pattern.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/melodic_pattern.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/message_box_component.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/message_box_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/messenger_mode_component.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/messenger_mode_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/mixer_utils.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/mixer_utils.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/note_editor_component.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/note_editor_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/note_editor_paginator.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/note_editor_paginator.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/note_layout_switcher.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/note_layout_switcher.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/note_repeat_component.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/note_repeat_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/note_settings_component.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/note_settings_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/pad_button_element.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/pad_button_element.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/pad_control.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/pad_control.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/pad_sensitivity.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/pad_sensitivity.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/playhead_component.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/playhead_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/push_base.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/push_base.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/quantization_component.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/quantization_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/scrollable_list.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/scrollable_list.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/scrollable_list_component.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/scrollable_list_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/select_playing_clip_component.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/select_playing_clip_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/selected_track_parameter_provider.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/selected_track_parameter_provider.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/selection.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/selection.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/session_recording_component.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/session_recording_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/setting.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/setting.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/skin_default.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/skin_default.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/sliced_simpler_component.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/sliced_simpler_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/slideable_touch_strip_component.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/slideable_touch_strip_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/song_utils.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/song_utils.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/special_session_component.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/special_session_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/step_duplicator.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/step_duplicator.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/step_seq_component.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/step_seq_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/touch_encoder_element.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/touch_encoder_element.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/touch_strip_controller.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/touch_strip_controller.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/touch_strip_element.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/touch_strip_element.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/track_frozen_mode.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/track_frozen_mode.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/transport_component.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/transport_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/undo_step_handler.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/undo_step_handler.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/user_component.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/user_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/value_component.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/value_component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-scripts-0.0.1/src/pushbase/velocity_levels_component.py` & `ableton-control-surface-scripts-0.0.2/src/pushbase/velocity_levels_component.py`

 * *Files identical despite different names*
