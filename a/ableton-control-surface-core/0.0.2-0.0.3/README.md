# Comparing `tmp/ableton-control-surface-core-0.0.2.tar.gz` & `tmp/ableton-control-surface-core-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/sahlen/repositories/oslo1989/ableton-controlsurface-toolkit/ableton-control-surface-core/dist/.tmp-g474kxmn/ableton-cont", last modified: Sun May  5 14:23:48 2024, max compression
+gzip compressed data, was "/Users/sahlen/repositories/oslo1989/ableton-controlsurface-toolkit/ableton-control-surface-core/dist/.tmp-ixv3uwcn/ableton-cont", last modified: Sun May  5 19:25:51 2024, max compression
```

## Comparing `ableton-control-surface-core-0.0.2.tar` & `ableton-control-surface-core-0.0.3.tar`

### file list

```diff
@@ -1,404 +1,404 @@
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/
--rw-r--r--   0 sahlen     (501) staff       (20)      677 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/PKG-INFO
--rw-r--r--   0 sahlen     (501) staff       (20)      775 2024-05-05 13:48:24.000000 ableton-control-surface-core-0.0.2/pyproject.toml
--rw-r--r--   0 sahlen     (501) staff       (20)       38 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/setup.cfg
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/Application/
--rw-r--r--   0 sahlen     (501) staff       (20)    33998 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/Application/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/Base/
--rw-r--r--   0 sahlen     (501) staff       (20)     7902 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/Base/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/Browser/
--rw-r--r--   0 sahlen     (501) staff       (20)    12899 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/Browser/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/CcControlDevice/
--rw-r--r--   0 sahlen     (501) staff       (20)    32941 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/CcControlDevice/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/Chain/
--rw-r--r--   0 sahlen     (501) staff       (20)    13722 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/Chain/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/ChainMixerDevice/
--rw-r--r--   0 sahlen     (501) staff       (20)     3237 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/ChainMixerDevice/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/Clip/
--rw-r--r--   0 sahlen     (501) staff       (20)    77137 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/Clip/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/ClipSlot/
--rw-r--r--   0 sahlen     (501) staff       (20)    15636 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/ClipSlot/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/CompressorDevice/
--rw-r--r--   0 sahlen     (501) staff       (20)    17945 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/CompressorDevice/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/Conversions/
--rw-r--r--   0 sahlen     (501) staff       (20)     5053 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/Conversions/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/Device/
--rw-r--r--   0 sahlen     (501) staff       (20)    12155 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/Device/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/DeviceIO/
--rw-r--r--   0 sahlen     (501) staff       (20)     7742 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/DeviceIO/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/DeviceParameter/
--rw-r--r--   0 sahlen     (501) staff       (20)    11899 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/DeviceParameter/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/DriftDevice/
--rw-r--r--   0 sahlen     (501) staff       (20)    36356 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/DriftDevice/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/DrumChain/
--rw-r--r--   0 sahlen     (501) staff       (20)    16427 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/DrumChain/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/DrumPad/
--rw-r--r--   0 sahlen     (501) staff       (20)     7070 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/DrumPad/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/Eq8Device/
--rw-r--r--   0 sahlen     (501) staff       (20)    18335 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/Eq8Device/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/Groove/
--rw-r--r--   0 sahlen     (501) staff       (20)     9819 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/Groove/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/GroovePool/
--rw-r--r--   0 sahlen     (501) staff       (20)     2695 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/GroovePool/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/HybridReverbDevice/
--rw-r--r--   0 sahlen     (501) staff       (20)    21543 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/HybridReverbDevice/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/Listener/
--rw-r--r--   0 sahlen     (501) staff       (20)     2671 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/Listener/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/LomObject/
--rw-r--r--   0 sahlen     (501) staff       (20)     1273 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/LomObject/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/MaxDevice/
--rw-r--r--   0 sahlen     (501) staff       (20)    19811 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/MaxDevice/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/MeldDevice/
--rw-r--r--   0 sahlen     (501) staff       (20)    16732 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/MeldDevice/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/MidiMap/
--rw-r--r--   0 sahlen     (501) staff       (20)     7319 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/MidiMap/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/MixerDevice/
--rw-r--r--   0 sahlen     (501) staff       (20)     8527 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/MixerDevice/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/PluginDevice/
--rw-r--r--   0 sahlen     (501) staff       (20)    14632 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/PluginDevice/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/RackDevice/
--rw-r--r--   0 sahlen     (501) staff       (20)    35755 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/RackDevice/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/RoarDevice/
--rw-r--r--   0 sahlen     (501) staff       (20)    14175 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/RoarDevice/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/Sample/
--rw-r--r--   0 sahlen     (501) staff       (20)    35677 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/Sample/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/Scene/
--rw-r--r--   0 sahlen     (501) staff       (20)    17944 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/Scene/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/ShifterDevice/
--rw-r--r--   0 sahlen     (501) staff       (20)    14278 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/ShifterDevice/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/SimplerDevice/
--rw-r--r--   0 sahlen     (501) staff       (20)    48147 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/SimplerDevice/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/Song/
--rw-r--r--   0 sahlen     (501) staff       (20)   107534 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/Song/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/SpectralResonatorDevice/
--rw-r--r--   0 sahlen     (501) staff       (20)    28621 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/SpectralResonatorDevice/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/Track/
--rw-r--r--   0 sahlen     (501) staff       (20)    83720 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/Track/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/Live/WavetableDevice/
--rw-r--r--   0 sahlen     (501) staff       (20)    42891 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/WavetableDevice/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)      917 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/Live/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/MidiRemoteScript/
--rw-r--r--   0 sahlen     (501) staff       (20)    32839 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.2/src/MidiRemoteScript/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/_Framework/
--rw-r--r--   0 sahlen     (501) staff       (20)     1833 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.2/src/_Framework/BackgroundComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3300 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/_Framework/ButtonElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3616 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/_Framework/ButtonMatrixElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4089 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.2/src/_Framework/ButtonSliderElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1761 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/_Framework/Capabilities.py
--rw-r--r--   0 sahlen     (501) staff       (20)    14786 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.2/src/_Framework/ChannelStripComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1472 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/_Framework/ChannelTranslationSelector.py
--rw-r--r--   0 sahlen     (501) staff       (20)      888 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.2/src/_Framework/ClipCreator.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9996 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/_Framework/ClipSlotComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)    10819 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.2/src/_Framework/ComboElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1728 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/_Framework/CompoundComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7910 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/_Framework/CompoundElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)    32387 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/_Framework/Control.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4548 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/_Framework/ControlElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)    23782 2024-01-08 19:11:24.000000 ableton-control-surface-core-0.0.2/src/_Framework/ControlSurface.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4675 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/_Framework/ControlSurfaceComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)      490 2024-01-08 18:43:23.000000 ableton-control-surface-core-0.0.2/src/_Framework/Defaults.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3273 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.2/src/_Framework/Dependency.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1414 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/_Framework/DeviceBankRegistry.py
--rw-r--r--   0 sahlen     (501) staff       (20)    17049 2024-01-09 19:53:39.000000 ableton-control-surface-core-0.0.2/src/_Framework/DeviceComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1843 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/_Framework/Disconnectable.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3030 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/_Framework/DisplayDataSource.py
--rw-r--r--   0 sahlen     (501) staff       (20)    12883 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/_Framework/DrumGroupComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2055 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/_Framework/DrumRackComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6554 2024-01-09 19:53:39.000000 ableton-control-surface-core-0.0.2/src/_Framework/EncoderElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2239 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/_Framework/IdentifiableControlSurface.py
--rw-r--r--   0 sahlen     (501) staff       (20)    14136 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/_Framework/InputControlElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4367 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.2/src/_Framework/Layer.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2234 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/_Framework/LogicalDisplaySegment.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6158 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/_Framework/MessageScheduler.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1904 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.2/src/_Framework/MidiMap.py
--rw-r--r--   0 sahlen     (501) staff       (20)    12257 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/_Framework/MixerComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4571 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/_Framework/ModeSelectorComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)    20978 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/_Framework/ModesComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1724 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.2/src/_Framework/MomentaryModeObserver.py
--rw-r--r--   0 sahlen     (501) staff       (20)      729 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.2/src/_Framework/NotifyingControlElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1072 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/_Framework/OptionalElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)    11654 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.2/src/_Framework/PhysicalDisplayElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1162 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/_Framework/Profile.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2296 2024-01-08 18:43:23.000000 ableton-control-surface-core-0.0.2/src/_Framework/Proxy.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7708 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/_Framework/Resource.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7057 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.2/src/_Framework/SceneComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4412 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/_Framework/ScrollComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)    24427 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/_Framework/SessionComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)    11946 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.2/src/_Framework/SessionRecordingComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)    13213 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/_Framework/SessionZoomingComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2258 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/_Framework/Signal.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1461 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.2/src/_Framework/Skin.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3749 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.2/src/_Framework/SlideComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)      622 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.2/src/_Framework/SliderElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)    11114 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/_Framework/SubjectSlot.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1063 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/_Framework/SysexValueControl.py
--rw-r--r--   0 sahlen     (501) staff       (20)    11460 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.2/src/_Framework/Task.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2889 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.2/src/_Framework/ToggleComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1708 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.2/src/_Framework/TrackArmState.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9300 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.2/src/_Framework/TransportComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)    11553 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/_Framework/Util.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5769 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/_Framework/ViewControlComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)      351 2024-01-08 18:43:23.000000 ableton-control-surface-core-0.0.2/src/_Framework/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/_Generic/
--rw-r--r--   0 sahlen     (501) staff       (20)    37607 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/_Generic/Devices.py
--rw-r--r--   0 sahlen     (501) staff       (20)    16385 2024-01-08 19:11:24.000000 ableton-control-surface-core-0.0.2/src/_Generic/GenericScript.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1089 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/_Generic/SelectChanStripComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)      792 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/_Generic/SpecialMixerComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)      349 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.2/src/_Generic/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1908 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/_Generic/util.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/_MxDCore/
--rw-r--r--   0 sahlen     (501) staff       (20)    10569 2024-01-08 19:11:24.000000 ableton-control-surface-core-0.0.2/src/_MxDCore/ControlSurfaceWrapper.py
--rw-r--r--   0 sahlen     (501) staff       (20)    39978 2024-01-08 19:11:24.000000 ableton-control-surface-core-0.0.2/src/_MxDCore/LomTypes.py
--rw-r--r--   0 sahlen     (501) staff       (20)    14200 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/_MxDCore/LomUtils.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6675 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/_MxDCore/MxDControlSurfaceAPI.py
--rw-r--r--   0 sahlen     (501) staff       (20)    61297 2024-01-08 19:11:24.000000 ableton-control-surface-core-0.0.2/src/_MxDCore/MxDCore.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6602 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/_MxDCore/MxDUtils.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1504 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.2/src/_MxDCore/NotesAPIUtils.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1512 2024-01-08 18:43:23.000000 ableton-control-surface-core-0.0.2/src/_MxDCore/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/_Tools/
--rw-r--r--   0 sahlen     (501) staff       (20)      347 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.2/src/_Tools/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/_Userscript/
--rw-r--r--   0 sahlen     (501) staff       (20)     4827 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/_Userscript/DeviceComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9889 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/_Userscript/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/ableton/
--rw-r--r--   0 sahlen     (501) staff       (20)      348 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.2/src/ableton/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/
--rw-r--r--   0 sahlen     (501) staff       (20)      351 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/base/
--rw-r--r--   0 sahlen     (501) staff       (20)     3343 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/base/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2330 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/base/abl_signal.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/base/collection/
--rw-r--r--   0 sahlen     (501) staff       (20)      433 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/base/collection/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1551 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/base/collection/indexed_dict.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3338 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/base/dependency.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2042 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/base/disconnectable.py
--rw-r--r--   0 sahlen     (501) staff       (20)    14798 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/base/event.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1340 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/base/gcutil.py
--rw-r--r--   0 sahlen     (501) staff       (20)      732 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/base/isclose.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1042 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/base/live_api_utils.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2297 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/base/proxy.py
--rw-r--r--   0 sahlen     (501) staff       (20)    11401 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/base/task.py
--rw-r--r--   0 sahlen     (501) staff       (20)    12769 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/base/util.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/
--rw-r--r--   0 sahlen     (501) staff       (20)     4994 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4084 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/banking_util.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1779 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/capabilities.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1203 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/clip_creator.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4633 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/component.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/
--rw-r--r--   0 sahlen     (501) staff       (20)     3574 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1391 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/accent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4234 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/auto_arm.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2028 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/background.py
--rw-r--r--   0 sahlen     (501) staff       (20)    15157 2024-01-08 19:05:13.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/channel_strip.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3305 2024-01-09 19:53:39.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/clip_actions.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9748 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/clip_slot.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5506 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/device.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7407 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/device_navigation.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5791 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/device_parameters.py
--rw-r--r--   0 sahlen     (501) staff       (20)    11832 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/drum_group.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9005 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/item_lister.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8917 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/mixer.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4324 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/playable.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8193 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/scene.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4225 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/scroll.py
--rw-r--r--   0 sahlen     (501) staff       (20)    11420 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/session.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5917 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/session_navigation.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6813 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/session_overview.py
--rw-r--r--   0 sahlen     (501) staff       (20)    13211 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/session_recording.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5390 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/session_ring.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3749 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/slide.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2966 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/target_track.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2838 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/toggle.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8721 2024-01-27 16:20:11.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/transport.py
--rw-r--r--   0 sahlen     (501) staff       (20)      874 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/undo_redo.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6121 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/view_control.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8705 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/compound_element.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/control/
--rw-r--r--   0 sahlen     (501) staff       (20)     2012 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/control/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)    10270 2024-01-08 19:05:13.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/control/button.py
--rw-r--r--   0 sahlen     (501) staff       (20)    10181 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/control/control.py
--rw-r--r--   0 sahlen     (501) staff       (20)    10920 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/control/control_list.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8999 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/control/encoder.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5216 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/control/mapped.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1991 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/control/radio_button.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1259 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/control/sysex.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1726 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/control/text_display.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2147 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/control/toggle_button.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5527 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/control_element.py
--rw-r--r--   0 sahlen     (501) staff       (20)    23211 2024-01-08 19:11:24.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/control_surface.py
--rw-r--r--   0 sahlen     (501) staff       (20)    12341 2024-01-08 19:11:24.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/decoration.py
--rw-r--r--   0 sahlen     (501) staff       (20)   244847 2024-01-08 19:05:13.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/default_bank_definitions.py
--rw-r--r--   0 sahlen     (501) staff       (20)      531 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/defaults.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4579 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/delay_decoration.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1516 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/device_bank_registry.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1564 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/device_chain_utils.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1779 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/device_decorator_factory.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6493 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/device_parameter_bank.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4720 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/device_provider.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2208 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/drift_decoration.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/elements/
--rw-r--r--   0 sahlen     (501) staff       (20)     2902 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/elements/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4180 2024-01-08 19:11:24.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/elements/button.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3805 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/elements/button_matrix.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4134 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/elements/button_slider.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3399 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/elements/color.py
--rw-r--r--   0 sahlen     (501) staff       (20)    10979 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/elements/combo.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3025 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/elements/display_data_source.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8390 2024-01-08 19:11:24.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/elements/encoder.py
--rw-r--r--   0 sahlen     (501) staff       (20)      666 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/elements/full_velocity_element.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2261 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/elements/logical_display_segment.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1077 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/elements/optional.py
--rw-r--r--   0 sahlen     (501) staff       (20)    11781 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/elements/physical_display.py
--rw-r--r--   0 sahlen     (501) staff       (20)      857 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/elements/playhead_element.py
--rw-r--r--   0 sahlen     (501) staff       (20)      630 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/elements/proxy_element.py
--rw-r--r--   0 sahlen     (501) staff       (20)      633 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/elements/slider.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2094 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/elements/sysex_element.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1041 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/elements/velocity_levels_element.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2403 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/identifiable_control_surface.py
--rw-r--r--   0 sahlen     (501) staff       (20)    15040 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/input_control_element.py
--rw-r--r--   0 sahlen     (501) staff       (20)    12428 2024-01-09 19:53:39.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/internal_parameter.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4936 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/layer.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6506 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/message_scheduler.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1683 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/midi.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1831 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/midi_map.py
--rw-r--r--   0 sahlen     (501) staff       (20)    16498 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/mode.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1924 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/parameter_provider.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5196 2024-01-08 19:05:13.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/parameter_slot_description.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3683 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/percussion_instrument_finder.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1178 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/profile.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7737 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/resource.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1215 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/roar_decoration.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1893 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/session_ring_selection_linking.py
--rw-r--r--   0 sahlen     (501) staff       (20)    14537 2024-01-08 19:11:24.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/simpler_decoration.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4011 2024-01-08 19:11:24.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/simpler_slice_nudging.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2587 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/skin.py
--rw-r--r--   0 sahlen     (501) staff       (20)    11861 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/wavetable_decoration.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/
--rw-r--r--   0 sahlen     (501) staff       (20)      351 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/base/
--rw-r--r--   0 sahlen     (501) staff       (20)     1791 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/base/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1674 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/base/util.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/
--rw-r--r--   0 sahlen     (501) staff       (20)     4373 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4680 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/banking_util.py
--rw-r--r--   0 sahlen     (501) staff       (20)      746 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/capabilities.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4179 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/colors.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4762 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3333 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/component_map.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/
--rw-r--r--   0 sahlen     (501) staff       (20)     4190 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1359 2024-01-08 18:43:23.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/accent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3465 2024-01-08 19:12:03.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/active_parameter.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3417 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/auto_arm.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3113 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/background.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8425 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/channel_strip.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5020 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/clip_actions.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7637 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/clip_slot.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2417 2024-01-08 18:43:23.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/clipboard.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9053 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/device.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5354 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/device_bank_navigation.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2336 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/device_parameters.py
--rw-r--r--   0 sahlen     (501) staff       (20)    14802 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/drum_group.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2087 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/drum_group_scroll.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2987 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/grid_resolution.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7049 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/loop_selector.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9585 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/mixer.py
--rw-r--r--   0 sahlen     (501) staff       (20)    17858 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/note_editor.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3459 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/page.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2116 2024-01-08 18:43:23.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/paginator.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4144 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/playable.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2733 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/playhead.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6702 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/recording.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4613 2024-01-08 18:43:23.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/scene.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4560 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/scroll.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9303 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/session.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5580 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/session_navigation.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4777 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/session_overview.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6395 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/session_ring.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2104 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/simple_device_navigation.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8492 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/sliced_simpler.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5588 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/step_sequence.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6721 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/target_track.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9883 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/transport.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1358 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/undo_redo.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5696 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/view_control.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2748 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/view_toggle.py
--rw-r--r--   0 sahlen     (501) staff       (20)      582 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/consts.py
--rw-r--r--   0 sahlen     (501) staff       (20)    14932 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/control_surface.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3959 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/control_surface_mapping.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2384 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/control_surface_specification.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/controls/
--rw-r--r--   0 sahlen     (501) staff       (20)     1775 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/controls/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2304 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/controls/button.py
--rw-r--r--   0 sahlen     (501) staff       (20)      662 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/controls/control.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2027 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/controls/control_list.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3614 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/controls/mapped.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1071 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/controls/toggle_button.py
--rw-r--r--   0 sahlen     (501) staff       (20)   110010 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/default_bank_definitions.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6838 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/default_skin.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2569 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/device_decorators.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/
--rw-r--r--   0 sahlen     (501) staff       (20)      913 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4884 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/display_specification.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/event_signal/
--rw-r--r--   0 sahlen     (501) staff       (20)      507 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/event_signal/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)      771 2024-01-08 19:25:27.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/event_signal/core.py
--rw-r--r--   0 sahlen     (501) staff       (20)      601 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/event_signal/type_decl.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/notifications/
--rw-r--r--   0 sahlen     (501) staff       (20)      515 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/notifications/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8662 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/notifications/all.py
--rw-r--r--   0 sahlen     (501) staff       (20)      552 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/notifications/default.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2117 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/notifications/meta.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1219 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/notifications/type_decl.py
--rw-r--r--   0 sahlen     (501) staff       (20)      767 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/notifications/util.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3710 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/renderable.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2339 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/state.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1819 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/text.py
--rw-r--r--   0 sahlen     (501) staff       (20)      736 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/type_decl.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1433 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/util.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/view/
--rw-r--r--   0 sahlen     (501) staff       (20)      618 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/view/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3422 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/view/notification.py
--rw-r--r--   0 sahlen     (501) staff       (20)      613 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/view/type_decl.py
--rw-r--r--   0 sahlen     (501) staff       (20)      686 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/view/util.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2799 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/view/view.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/elements/
--rw-r--r--   0 sahlen     (501) staff       (20)     1573 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/elements/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2709 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/elements/button.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1374 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/elements/button_matrix.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2154 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/elements/color.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1547 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/elements/discrete_values.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2261 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/elements/display_line.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7540 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/elements/encoder.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2216 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/elements/lockable_button.py
--rw-r--r--   0 sahlen     (501) staff       (20)      646 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/elements/lockable_combo.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3723 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/elements/sysex.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1493 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/elements/touch.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8328 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/elements_base.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6039 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/identification.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3490 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/instrument_finder.py
--rw-r--r--   0 sahlen     (501) staff       (20)      675 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/layer.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1159 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/legacy_bank_definitions.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1030 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/midi.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/mode/
--rw-r--r--   0 sahlen     (501) staff       (20)     1648 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/mode/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2180 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/mode/behaviour.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2531 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/mode/mode.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8687 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/mode/modes.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2584 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/mode/selector.py
--rw-r--r--   0 sahlen     (501) staff       (20)      918 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/parameter_info.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3521 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/parameter_mapping_sensitivities.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2617 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/session_ring_selection_linking.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2215 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/skin.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/live/
--rw-r--r--   0 sahlen     (501) staff       (20)     1986 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/live/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7661 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/live/action.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8159 2024-01-09 19:53:39.000000 ableton-control-surface-core-0.0.2/src/ableton/v3/live/util.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/ableton_control_surface_core.egg-info/
--rw-r--r--   0 sahlen     (501) staff       (20)      677 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/ableton_control_surface_core.egg-info/PKG-INFO
--rw-r--r--   0 sahlen     (501) staff       (20)    15098 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/ableton_control_surface_core.egg-info/SOURCES.txt
--rw-r--r--   0 sahlen     (501) staff       (20)        1 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/ableton_control_surface_core.egg-info/dependency_links.txt
--rw-r--r--   0 sahlen     (501) staff       (20)       78 2024-05-05 14:23:48.000000 ableton-control-surface-core-0.0.2/src/ableton_control_surface_core.egg-info/top_level.txt
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/
+-rw-r--r--   0 sahlen     (501) staff       (20)      677 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/PKG-INFO
+-rw-r--r--   0 sahlen     (501) staff       (20)      784 2024-05-05 19:25:30.000000 ableton-control-surface-core-0.0.3/pyproject.toml
+-rw-r--r--   0 sahlen     (501) staff       (20)       38 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/setup.cfg
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/Application/
+-rw-r--r--   0 sahlen     (501) staff       (20)    33998 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/Application/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/Base/
+-rw-r--r--   0 sahlen     (501) staff       (20)     7902 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/Base/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/Browser/
+-rw-r--r--   0 sahlen     (501) staff       (20)    12899 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/Browser/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/CcControlDevice/
+-rw-r--r--   0 sahlen     (501) staff       (20)    32941 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/CcControlDevice/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/Chain/
+-rw-r--r--   0 sahlen     (501) staff       (20)    13722 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/Chain/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/ChainMixerDevice/
+-rw-r--r--   0 sahlen     (501) staff       (20)     3237 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/ChainMixerDevice/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/Clip/
+-rw-r--r--   0 sahlen     (501) staff       (20)    77137 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/Clip/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/ClipSlot/
+-rw-r--r--   0 sahlen     (501) staff       (20)    15636 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/ClipSlot/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/CompressorDevice/
+-rw-r--r--   0 sahlen     (501) staff       (20)    17945 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/CompressorDevice/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/Conversions/
+-rw-r--r--   0 sahlen     (501) staff       (20)     5053 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/Conversions/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/Device/
+-rw-r--r--   0 sahlen     (501) staff       (20)    12155 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/Device/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/DeviceIO/
+-rw-r--r--   0 sahlen     (501) staff       (20)     7742 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/DeviceIO/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/DeviceParameter/
+-rw-r--r--   0 sahlen     (501) staff       (20)    11899 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/DeviceParameter/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/DriftDevice/
+-rw-r--r--   0 sahlen     (501) staff       (20)    36356 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/DriftDevice/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/DrumChain/
+-rw-r--r--   0 sahlen     (501) staff       (20)    16427 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/DrumChain/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/DrumPad/
+-rw-r--r--   0 sahlen     (501) staff       (20)     7070 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/DrumPad/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/Eq8Device/
+-rw-r--r--   0 sahlen     (501) staff       (20)    18335 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/Eq8Device/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/Groove/
+-rw-r--r--   0 sahlen     (501) staff       (20)     9819 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/Groove/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/GroovePool/
+-rw-r--r--   0 sahlen     (501) staff       (20)     2695 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/GroovePool/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/HybridReverbDevice/
+-rw-r--r--   0 sahlen     (501) staff       (20)    21543 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/HybridReverbDevice/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/Listener/
+-rw-r--r--   0 sahlen     (501) staff       (20)     2671 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/Listener/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/LomObject/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1273 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/LomObject/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/MaxDevice/
+-rw-r--r--   0 sahlen     (501) staff       (20)    19811 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/MaxDevice/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/MeldDevice/
+-rw-r--r--   0 sahlen     (501) staff       (20)    16732 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/MeldDevice/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/MidiMap/
+-rw-r--r--   0 sahlen     (501) staff       (20)     7319 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/MidiMap/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/MixerDevice/
+-rw-r--r--   0 sahlen     (501) staff       (20)     8527 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/MixerDevice/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/PluginDevice/
+-rw-r--r--   0 sahlen     (501) staff       (20)    14632 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/PluginDevice/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/RackDevice/
+-rw-r--r--   0 sahlen     (501) staff       (20)    35755 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/RackDevice/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/RoarDevice/
+-rw-r--r--   0 sahlen     (501) staff       (20)    14175 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/RoarDevice/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/Sample/
+-rw-r--r--   0 sahlen     (501) staff       (20)    35677 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/Sample/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/Scene/
+-rw-r--r--   0 sahlen     (501) staff       (20)    17944 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/Scene/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/ShifterDevice/
+-rw-r--r--   0 sahlen     (501) staff       (20)    14278 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/ShifterDevice/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/SimplerDevice/
+-rw-r--r--   0 sahlen     (501) staff       (20)    48147 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/SimplerDevice/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/Song/
+-rw-r--r--   0 sahlen     (501) staff       (20)   107534 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/Song/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/SpectralResonatorDevice/
+-rw-r--r--   0 sahlen     (501) staff       (20)    28621 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/SpectralResonatorDevice/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/Track/
+-rw-r--r--   0 sahlen     (501) staff       (20)    83720 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/Track/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/Live/WavetableDevice/
+-rw-r--r--   0 sahlen     (501) staff       (20)    42891 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/WavetableDevice/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      917 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/Live/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/MidiRemoteScript/
+-rw-r--r--   0 sahlen     (501) staff       (20)    32839 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.3/src/MidiRemoteScript/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/_Framework/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1833 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.3/src/_Framework/BackgroundComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3300 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/_Framework/ButtonElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3616 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/_Framework/ButtonMatrixElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4089 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.3/src/_Framework/ButtonSliderElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1761 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/_Framework/Capabilities.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    14782 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/_Framework/ChannelStripComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1472 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/_Framework/ChannelTranslationSelector.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      888 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.3/src/_Framework/ClipCreator.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9996 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/_Framework/ClipSlotComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    10819 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.3/src/_Framework/ComboElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1728 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/_Framework/CompoundComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     7910 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/_Framework/CompoundElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    32374 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/_Framework/Control.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4548 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/_Framework/ControlElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    23782 2024-01-08 19:11:24.000000 ableton-control-surface-core-0.0.3/src/_Framework/ControlSurface.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4675 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/_Framework/ControlSurfaceComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      490 2024-01-08 18:43:23.000000 ableton-control-surface-core-0.0.3/src/_Framework/Defaults.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3273 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.3/src/_Framework/Dependency.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1377 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/_Framework/DeviceBankRegistry.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    17045 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/_Framework/DeviceComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1843 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/_Framework/Disconnectable.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3030 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/_Framework/DisplayDataSource.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    12883 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/_Framework/DrumGroupComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2055 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/_Framework/DrumRackComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6553 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/_Framework/EncoderElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2152 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/_Framework/IdentifiableControlSurface.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    14136 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/_Framework/InputControlElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4367 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.3/src/_Framework/Layer.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2234 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/_Framework/LogicalDisplaySegment.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6158 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/_Framework/MessageScheduler.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1904 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.3/src/_Framework/MidiMap.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    12255 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/_Framework/MixerComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4571 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/_Framework/ModeSelectorComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    20978 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/_Framework/ModesComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1724 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.3/src/_Framework/MomentaryModeObserver.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      729 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.3/src/_Framework/NotifyingControlElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1072 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/_Framework/OptionalElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    11654 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.3/src/_Framework/PhysicalDisplayElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1160 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/_Framework/Profile.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2293 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/_Framework/Proxy.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     7708 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/_Framework/Resource.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     7057 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.3/src/_Framework/SceneComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4412 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/_Framework/ScrollComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    24427 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/_Framework/SessionComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    11946 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.3/src/_Framework/SessionRecordingComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    13213 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/_Framework/SessionZoomingComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2258 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/_Framework/Signal.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1456 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/_Framework/Skin.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3749 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.3/src/_Framework/SlideComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      622 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.3/src/_Framework/SliderElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    11114 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/_Framework/SubjectSlot.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1063 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/_Framework/SysexValueControl.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    11460 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.3/src/_Framework/Task.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2889 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.3/src/_Framework/ToggleComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1708 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.3/src/_Framework/TrackArmState.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9300 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.3/src/_Framework/TransportComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    11558 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/_Framework/Util.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5769 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/_Framework/ViewControlComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      351 2024-01-08 18:43:23.000000 ableton-control-surface-core-0.0.3/src/_Framework/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/_Generic/
+-rw-r--r--   0 sahlen     (501) staff       (20)    37606 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/_Generic/Devices.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    16384 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/_Generic/GenericScript.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1089 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/_Generic/SelectChanStripComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      792 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/_Generic/SpecialMixerComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      349 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.3/src/_Generic/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1908 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/_Generic/util.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/_MxDCore/
+-rw-r--r--   0 sahlen     (501) staff       (20)    10569 2024-01-08 19:11:24.000000 ableton-control-surface-core-0.0.3/src/_MxDCore/ControlSurfaceWrapper.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    39976 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/_MxDCore/LomTypes.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    14199 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/_MxDCore/LomUtils.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6675 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/_MxDCore/MxDControlSurfaceAPI.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    61272 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/_MxDCore/MxDCore.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6601 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/_MxDCore/MxDUtils.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1504 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.3/src/_MxDCore/NotesAPIUtils.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1512 2024-01-08 18:43:23.000000 ableton-control-surface-core-0.0.3/src/_MxDCore/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/_Tools/
+-rw-r--r--   0 sahlen     (501) staff       (20)      347 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.3/src/_Tools/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/_Userscript/
+-rw-r--r--   0 sahlen     (501) staff       (20)     4827 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/_Userscript/DeviceComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9889 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/_Userscript/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/ableton/
+-rw-r--r--   0 sahlen     (501) staff       (20)      348 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.3/src/ableton/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/
+-rw-r--r--   0 sahlen     (501) staff       (20)      351 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/base/
+-rw-r--r--   0 sahlen     (501) staff       (20)     3343 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/base/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2330 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/base/abl_signal.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/base/collection/
+-rw-r--r--   0 sahlen     (501) staff       (20)      433 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/base/collection/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1551 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/base/collection/indexed_dict.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3336 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/base/dependency.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2042 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/base/disconnectable.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    14794 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/base/event.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1340 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/base/gcutil.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      732 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/base/isclose.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1042 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/base/live_api_utils.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2295 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/base/proxy.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    11401 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/base/task.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    12775 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/base/util.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/
+-rw-r--r--   0 sahlen     (501) staff       (20)     4994 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4084 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/banking_util.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1779 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/capabilities.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1203 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/clip_creator.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4633 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/component.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/
+-rw-r--r--   0 sahlen     (501) staff       (20)     3574 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1391 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/accent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4234 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/auto_arm.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2028 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/background.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    15153 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/channel_strip.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3304 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/clip_actions.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9748 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/clip_slot.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5506 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/device.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     7407 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/device_navigation.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5791 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/device_parameters.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    11832 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/drum_group.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9005 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/item_lister.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8917 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/mixer.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4324 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/playable.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8193 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/scene.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4225 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/scroll.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    11420 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/session.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5917 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/session_navigation.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6813 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/session_overview.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    13211 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/session_recording.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5390 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/session_ring.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3749 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/slide.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2966 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/target_track.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2838 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/toggle.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8721 2024-01-27 16:20:11.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/transport.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      874 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/undo_redo.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6121 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/view_control.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8705 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/compound_element.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/control/
+-rw-r--r--   0 sahlen     (501) staff       (20)     2012 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/control/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    10270 2024-01-08 19:05:13.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/control/button.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    10181 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/control/control.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    10908 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/control/control_list.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8999 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/control/encoder.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5216 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/control/mapped.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1991 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/control/radio_button.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1259 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/control/sysex.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1726 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/control/text_display.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2147 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/control/toggle_button.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5527 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/control_element.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    23210 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/control_surface.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    12340 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/decoration.py
+-rw-r--r--   0 sahlen     (501) staff       (20)   244847 2024-01-08 19:05:13.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/default_bank_definitions.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      531 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/defaults.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4579 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/delay_decoration.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1479 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/device_bank_registry.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1564 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/device_chain_utils.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1779 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/device_decorator_factory.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6493 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/device_parameter_bank.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4720 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/device_provider.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2208 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/drift_decoration.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/elements/
+-rw-r--r--   0 sahlen     (501) staff       (20)     2902 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/elements/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4179 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/elements/button.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3805 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/elements/button_matrix.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4134 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/elements/button_slider.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3399 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/elements/color.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    10979 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/elements/combo.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3025 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/elements/display_data_source.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8383 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/elements/encoder.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      666 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/elements/full_velocity_element.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2261 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/elements/logical_display_segment.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1077 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/elements/optional.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    11781 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/elements/physical_display.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      857 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/elements/playhead_element.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      630 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/elements/proxy_element.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      633 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/elements/slider.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2094 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/elements/sysex_element.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1041 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/elements/velocity_levels_element.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2403 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/identifiable_control_surface.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    15040 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/input_control_element.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    12427 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/internal_parameter.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4936 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/layer.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6506 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/message_scheduler.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1683 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/midi.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1831 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/midi_map.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    16494 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/mode.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1924 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/parameter_provider.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5089 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/parameter_slot_description.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3683 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/percussion_instrument_finder.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1176 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/profile.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     7737 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/resource.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1215 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/roar_decoration.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1893 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/session_ring_selection_linking.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    14536 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/simpler_decoration.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4010 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/simpler_slice_nudging.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2582 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/skin.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    11861 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/wavetable_decoration.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/
+-rw-r--r--   0 sahlen     (501) staff       (20)      351 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/base/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1791 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/base/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1674 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/base/util.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/
+-rw-r--r--   0 sahlen     (501) staff       (20)     4373 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4680 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/banking_util.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      746 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/capabilities.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4179 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/colors.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4762 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3333 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/component_map.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/
+-rw-r--r--   0 sahlen     (501) staff       (20)     4190 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1359 2024-01-08 18:43:23.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/accent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3465 2024-01-08 19:12:03.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/active_parameter.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3417 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/auto_arm.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3113 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/background.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8425 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/channel_strip.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5020 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/clip_actions.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     7637 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/clip_slot.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2417 2024-01-08 18:43:23.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/clipboard.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9053 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/device.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5354 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/device_bank_navigation.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2336 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/device_parameters.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    14802 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/drum_group.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2087 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/drum_group_scroll.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2987 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/grid_resolution.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     7049 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/loop_selector.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9585 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/mixer.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    17858 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/note_editor.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3459 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/page.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2116 2024-01-08 18:43:23.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/paginator.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4144 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/playable.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2733 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/playhead.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6702 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/recording.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4613 2024-01-08 18:43:23.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/scene.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4560 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/scroll.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9303 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/session.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5580 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/session_navigation.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4777 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/session_overview.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6395 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/session_ring.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2104 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/simple_device_navigation.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8492 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/sliced_simpler.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5588 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/step_sequence.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6721 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/target_track.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9883 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/transport.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1358 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/undo_redo.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5696 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/view_control.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2748 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/view_toggle.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      582 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/consts.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    14932 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/control_surface.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3959 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/control_surface_mapping.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2384 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/control_surface_specification.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/controls/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1775 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/controls/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2304 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/controls/button.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      662 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/controls/control.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2021 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/controls/control_list.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3614 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/controls/mapped.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1071 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/controls/toggle_button.py
+-rw-r--r--   0 sahlen     (501) staff       (20)   110010 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/default_bank_definitions.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6838 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/default_skin.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2569 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/device_decorators.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/
+-rw-r--r--   0 sahlen     (501) staff       (20)      913 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4884 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/display_specification.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/event_signal/
+-rw-r--r--   0 sahlen     (501) staff       (20)      507 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/event_signal/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      771 2024-01-08 19:25:27.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/event_signal/core.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      601 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/event_signal/type_decl.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/notifications/
+-rw-r--r--   0 sahlen     (501) staff       (20)      515 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/notifications/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8662 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/notifications/all.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      552 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/notifications/default.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2117 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/notifications/meta.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1219 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/notifications/type_decl.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      767 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/notifications/util.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3710 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/renderable.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2339 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/state.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1819 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/text.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      736 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/type_decl.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1433 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/util.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/view/
+-rw-r--r--   0 sahlen     (501) staff       (20)      618 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/view/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3422 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/view/notification.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      613 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/view/type_decl.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      686 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/view/util.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2799 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/view/view.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/elements/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1573 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/elements/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2709 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/elements/button.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1374 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/elements/button_matrix.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2154 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/elements/color.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1547 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/elements/discrete_values.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2261 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/elements/display_line.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     7540 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/elements/encoder.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2216 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/elements/lockable_button.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      646 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/elements/lockable_combo.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3723 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/elements/sysex.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1493 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/elements/touch.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8328 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/elements_base.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6039 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/identification.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3490 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/instrument_finder.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      675 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/layer.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1160 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/legacy_bank_definitions.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1030 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/midi.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/mode/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1648 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/mode/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2180 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/mode/behaviour.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2531 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/mode/mode.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8685 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/mode/modes.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2584 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/mode/selector.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      918 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/parameter_info.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3521 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/parameter_mapping_sensitivities.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2617 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/session_ring_selection_linking.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2215 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/skin.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/live/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1986 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/live/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     7661 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/live/action.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8160 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.3/src/ableton/v3/live/util.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/ableton_control_surface_core.egg-info/
+-rw-r--r--   0 sahlen     (501) staff       (20)      677 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/ableton_control_surface_core.egg-info/PKG-INFO
+-rw-r--r--   0 sahlen     (501) staff       (20)    15098 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/ableton_control_surface_core.egg-info/SOURCES.txt
+-rw-r--r--   0 sahlen     (501) staff       (20)        1 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/ableton_control_surface_core.egg-info/dependency_links.txt
+-rw-r--r--   0 sahlen     (501) staff       (20)       78 2024-05-05 19:25:51.000000 ableton-control-surface-core-0.0.3/src/ableton_control_surface_core.egg-info/top_level.txt
```

### Comparing `ableton-control-surface-core-0.0.2/PKG-INFO` & `ableton-control-surface-core-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ableton-control-surface-core
-Version: 0.0.2
+Version: 0.0.3
 Summary: Decompiled core packages from Ableton Live's Python API to help developers build custom control surfaces.
 Author-email: Martin Sahlen <martin8900@gmail.com>
 Project-URL: Homepage, https://github.com/oslo1989/ableton-control-surface-toolkit
 Project-URL: Issues, https://github.com/oslo1989/ableton-control-surface-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ableton-control-surface-core-0.0.2/pyproject.toml` & `ableton-control-surface-core-0.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools"]
+requires = ["setuptools ~=68.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ableton-control-surface-core"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     {name = "Martin Sahlen", email = "martin8900@gmail.com"}
 ]
 description = "Decompiled core packages from Ableton Live's Python API to help developers build custom control surfaces."
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `ableton-control-surface-core-0.0.2/src/Live/Application/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/Application/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/Base/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/Base/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/Browser/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/Browser/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/CcControlDevice/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/CcControlDevice/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/Chain/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/Chain/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/ChainMixerDevice/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/ChainMixerDevice/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/Clip/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/Clip/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/ClipSlot/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/ClipSlot/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/CompressorDevice/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/CompressorDevice/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/Conversions/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/Conversions/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/Device/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/Device/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/DeviceIO/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/DeviceIO/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/DeviceParameter/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/DeviceParameter/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/DriftDevice/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/DriftDevice/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/DrumChain/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/DrumChain/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/DrumPad/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/DrumPad/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/Eq8Device/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/Eq8Device/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/Groove/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/Groove/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/GroovePool/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/GroovePool/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/HybridReverbDevice/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/HybridReverbDevice/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/Listener/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/Listener/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/LomObject/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/LomObject/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/MaxDevice/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/MaxDevice/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/MeldDevice/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/MeldDevice/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/MidiMap/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/MidiMap/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/MixerDevice/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/MixerDevice/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/PluginDevice/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/PluginDevice/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/RackDevice/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/RackDevice/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/RoarDevice/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/RoarDevice/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/Sample/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/Sample/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/Scene/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/Scene/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/ShifterDevice/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/ShifterDevice/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/SimplerDevice/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/SimplerDevice/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/Song/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/Song/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/SpectralResonatorDevice/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/SpectralResonatorDevice/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/Track/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/Track/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/WavetableDevice/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/WavetableDevice/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/Live/__init__.py` & `ableton-control-surface-core-0.0.3/src/Live/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/MidiRemoteScript/__init__.py` & `ableton-control-surface-core-0.0.3/src/MidiRemoteScript/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/BackgroundComponent.py` & `ableton-control-surface-core-0.0.3/src/_Framework/BackgroundComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/ButtonElement.py` & `ableton-control-surface-core-0.0.3/src/_Framework/ButtonElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/ButtonMatrixElement.py` & `ableton-control-surface-core-0.0.3/src/_Framework/ButtonMatrixElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/ButtonSliderElement.py` & `ableton-control-surface-core-0.0.3/src/_Framework/ButtonSliderElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/Capabilities.py` & `ableton-control-surface-core-0.0.3/src/_Framework/Capabilities.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/ChannelStripComponent.py` & `ableton-control-surface-core-0.0.3/src/_Framework/ChannelStripComponent.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,30 +65,30 @@
         self._invert_mute_feedback = False
         self._track_name_data_source = DisplayDataSource()
         self._update_track_name_data_source()
         self._empty_control_slots = self.register_slot_manager()
 
         def make_property_slot(name, alias=None):
             alias = alias or name
-            return self.register_slot(None, getattr(self, "_on_%s_changed" % alias), name)
+            return self.register_slot(None, getattr(self, f"_on_{alias}_changed"), name)
 
         self._track_property_slots = [
             make_property_slot("mute"),
             make_property_slot("solo"),
             make_property_slot("arm"),
             make_property_slot("input_routing_type", "input_routing"),
             make_property_slot("name", "track_name"),
         ]
         self._mixer_device_property_slots = [
             make_property_slot("crossfade_assign", "cf_assign"),
             make_property_slot("sends"),
         ]
 
         def make_button_slot(name):
-            return self.register_slot(None, getattr(self, "_%s_value" % name), "value")
+            return self.register_slot(None, getattr(self, f"_{name}_value"), "value")
 
         self._select_button_slot = make_button_slot("select")
         self._mute_button_slot = make_button_slot("mute")
         self._solo_button_slot = make_button_slot("solo")
         self._arm_button_slot = make_button_slot("arm")
         self._shift_button_slot = make_button_slot("shift")
         self._crossfade_toggle_slot = make_button_slot("crossfade_toggle")
```

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/ChannelTranslationSelector.py` & `ableton-control-surface-core-0.0.3/src/_Framework/ChannelTranslationSelector.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/ClipCreator.py` & `ableton-control-surface-core-0.0.3/src/_Framework/ClipCreator.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/ClipSlotComponent.py` & `ableton-control-surface-core-0.0.3/src/_Framework/ClipSlotComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/ComboElement.py` & `ableton-control-surface-core-0.0.3/src/_Framework/ComboElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/CompoundComponent.py` & `ableton-control-surface-core-0.0.3/src/_Framework/CompoundComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/CompoundElement.py` & `ableton-control-surface-core-0.0.3/src/_Framework/CompoundElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/Control.py` & `ableton-control-surface-core-0.0.3/src/_Framework/Control.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 # Decompiled from: Python 3.7.16 (default, Jan 17 2023, 09:28:58)
 # [Clang 14.0.6 ]
 # Embedded file name: output/Live/mac_universal_64_static/Release/python-bundle/MIDI Remote Scripts/_Framework/Control.py
 # Compiled at: 2023-11-21 10:21:18
 # Size of source mod 2**32: 34364 bytes
 from functools import partial
 
+from ableton.v2.base import old_hasattr
 from future.moves.itertools import zip_longest
 from past.utils import old_div
 
-from ableton.v2.base import old_hasattr
-
 from . import Task
 from .Defaults import MOMENTARY_DELAY
 from .SubjectSlot import SlotManager
 from .Util import clamp, first, flatten, is_matrix, lazy_attribute, mixin, nop, product, second
 
 
 class ControlManager(SlotManager):
@@ -826,22 +825,22 @@
 _control_list_classes = {}
 _control_matrix_classes = {}
 
 
 def control_list(control_type, *a, **k):
     if control_type == RadioButtonControl:
         return RadioButtonGroup(*a, **k)
-    c = _control_list_classes.get(control_type, None)
+    c = _control_list_classes.get(control_type)
     if not c:
         c = mixin(ControlList, control_type)
         c.State = mixin(ControlList.State, control_type.State)
         _control_list_classes[control_type] = c
     return c(control_type, *a, **k)
 
 
 def control_matrix(control_type, *a, **k):
-    m = _control_matrix_classes.get(control_type, None)
+    m = _control_matrix_classes.get(control_type)
     if not m:
         m = mixin(MatrixControl, control_type)
         m.State = mixin(MatrixControl.State, control_type.State)
         _control_matrix_classes[control_type] = m
     return m(control_type, *a, **k)
```

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/ControlElement.py` & `ableton-control-surface-core-0.0.3/src/_Framework/ControlElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/ControlSurface.py` & `ableton-control-surface-core-0.0.3/src/_Framework/ControlSurface.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/ControlSurfaceComponent.py` & `ableton-control-surface-core-0.0.3/src/_Framework/ControlSurfaceComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/Dependency.py` & `ableton-control-surface-core-0.0.3/src/_Framework/Dependency.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/DeviceBankRegistry.py` & `ableton-control-surface-core-0.0.3/src/_Framework/DeviceBankRegistry.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     def compact_registry(self):
         newreg = dict([k__ for k__ in list(self._device_bank_registry.items()) if k__[0] is not None])
         self._device_bank_registry = newreg
 
     def set_device_bank(self, device, bank):
         key = self._find_device_bank_key(device) or device
-        old = self._device_bank_registry[key] if key in self._device_bank_registry else 0
+        old = self._device_bank_registry.get(key, 0)
         if old != bank:
             self._device_bank_registry[key] = bank
             self.notify_device_bank(device, bank)
 
     def get_device_bank(self, device):
         return self._device_bank_registry.get(self._find_device_bank_key(device), 0)
```

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/DeviceComponent.py` & `ableton-control-surface-core-0.0.3/src/_Framework/DeviceComponent.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,23 +58,23 @@
         self._device_name_data_source = None
         self._bank_index = 0
         self._bank_name = "<No Bank>"
         self._locked_to_device = False
 
         def make_property_slot(name, alias=None):
             alias = alias or name
-            return self.register_slot(None, getattr(self, "_on_%s_changed" % alias), name)
+            return self.register_slot(None, getattr(self, f"_on_{alias}_changed"), name)
 
         self._on_off_property_slot = make_property_slot("value", alias="device_on_off")
         self._name_property_slot = make_property_slot("name", alias="device_name")
         self._parameters_property_slot = make_property_slot("parameters")
         self._device_bank_property_slot = make_property_slot("device_bank")
 
         def make_button_slot(name):
-            return self.register_slot(None, getattr(self, "_%s_value" % name), "value")
+            return self.register_slot(None, getattr(self, f"_{name}_value"), "value")
 
         self._bank_up_button_slot = make_button_slot("bank_up")
         self._bank_down_button_slot = make_button_slot("bank_down")
         self._lock_button_slot = make_button_slot("lock")
         self._on_off_button_slot = make_button_slot("on_off")
         song = self.song()
         view = song.view
```

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/Disconnectable.py` & `ableton-control-surface-core-0.0.3/src/_Framework/Disconnectable.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/DisplayDataSource.py` & `ableton-control-surface-core-0.0.3/src/_Framework/DisplayDataSource.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/DrumGroupComponent.py` & `ableton-control-surface-core-0.0.3/src/_Framework/DrumGroupComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/DrumRackComponent.py` & `ableton-control-surface-core-0.0.3/src/_Framework/DrumRackComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/EncoderElement.py` & `ableton-control-surface-core-0.0.3/src/_Framework/EncoderElement.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # decompyle3 version 3.9.0
 # Python bytecode version base 3.7.0 (3394)
 # Decompiled from: Python 3.7.16 (default, Jan 17 2023, 09:28:58)
 # [Clang 14.0.6 ]
 # Embedded file name: output/Live/mac_universal_64_static/Release/python-bundle/MIDI Remote Scripts/_Framework/EncoderElement.py
 # Compiled at: 2023-11-21 10:21:18
 # Size of source mod 2**32: 7712 bytes
-from past.utils import old_div
-
 import Live
+from past.utils import old_div
 
 from .ComboElement import WrapperElement
 from .CompoundElement import CompoundElement
 from .InputControlElement import MIDI_CC_TYPE, InputControlElement, InputSignal
 from .SubjectSlot import SubjectEvent, subject_slot
 from .Util import const, nop
```

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/IdentifiableControlSurface.py` & `ableton-control-surface-core-0.0.3/src/_Framework/IdentifiableControlSurface.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,18 +36,15 @@
             if product_id_bytes == self._product_id_bytes:
                 self._request_task.kill()
                 if self._identity_response_pending:
                     self.on_identified()
                     self._identity_response_pending = False
             else:
                 self.log_message(
-                    "MIDI device responded with wrong product id ({} != {}).".format(
-                        str(self._product_id_bytes),
-                        str(product_id_bytes),
-                    ),
+                    f"MIDI device responded with wrong product id ({self._product_id_bytes!s} != {product_id_bytes!s}).",
                 )
         else:
             super().handle_sysex(midi_bytes)
 
     def _is_identity_response(self, midi_bytes):
         return midi_bytes[3:5] == (6, 2)
```

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/InputControlElement.py` & `ableton-control-surface-core-0.0.3/src/_Framework/InputControlElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/Layer.py` & `ableton-control-surface-core-0.0.3/src/_Framework/Layer.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/LogicalDisplaySegment.py` & `ableton-control-surface-core-0.0.3/src/_Framework/LogicalDisplaySegment.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/MessageScheduler.py` & `ableton-control-surface-core-0.0.3/src/_Framework/MessageScheduler.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/MidiMap.py` & `ableton-control-surface-core-0.0.3/src/_Framework/MidiMap.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/MixerComponent.py` & `ableton-control-surface-core-0.0.3/src/_Framework/MixerComponent.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         self.set_track_offset(0)
         if auto_name:
             self._auto_name()
         self._on_return_tracks_changed.subject = self.song()
         self._on_return_tracks_changed()
 
         def make_button_slot(name):
-            return self.register_slot(None, getattr(self, "_%s_value" % name), "value")
+            return self.register_slot(None, getattr(self, f"_{name}_value"), "value")
 
         self._bank_up_button_slot = make_button_slot("bank_up")
         self._bank_down_button_slot = make_button_slot("bank_down")
         self._next_track_button_slot = make_button_slot("next_track")
         self._prev_track_button_slot = make_button_slot("prev_track")
 
     def disconnect(self):
```

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/ModeSelectorComponent.py` & `ableton-control-surface-core-0.0.3/src/_Framework/ModeSelectorComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/ModesComponent.py` & `ableton-control-surface-core-0.0.3/src/_Framework/ModesComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/MomentaryModeObserver.py` & `ableton-control-surface-core-0.0.3/src/_Framework/MomentaryModeObserver.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/NotifyingControlElement.py` & `ableton-control-surface-core-0.0.3/src/_Framework/NotifyingControlElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/OptionalElement.py` & `ableton-control-surface-core-0.0.3/src/_Framework/OptionalElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/PhysicalDisplayElement.py` & `ableton-control-surface-core-0.0.3/src/_Framework/PhysicalDisplayElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/Profile.py` & `ableton-control-surface-core-0.0.3/src/_Framework/Profile.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 def profile(fn):
     if ENABLE_PROFILING:
 
         @wraps(fn)
         def wrapper(self, *a, **k):
             if PROFILER:
                 return PROFILER.runcall(partial(fn, self, *a, **k))
-            print("Can not profile (%s), it is probably reloaded" % fn.__name__)
+            print(f"Can not profile ({fn.__name__}), it is probably reloaded")
             return fn(*a, **k)
 
         return wrapper
     return fn
 
 
 def dump(name="default"):
```

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/Proxy.py` & `ableton-control-surface-core-0.0.3/src/_Framework/Proxy.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # decompyle3 version 3.9.0
 # Python bytecode version base 3.7.0 (3394)
 # Decompiled from: Python 3.7.16 (default, Jan 17 2023, 09:28:58)
 # [Clang 14.0.6 ]
 # Embedded file name: output/Live/mac_universal_64_static/Release/python-bundle/MIDI Remote Scripts/_Framework/Proxy.py
 # Compiled at: 2023-11-21 10:21:18
 # Size of source mod 2**32: 3335 bytes
-from future.utils import raise_
-
 from ableton.v2.base import old_hasattr
+from future.utils import raise_
 
 from .Util import BooleanContext
 
 
 class ProxyBase:
     _skip_wrapper_lookup = None
 
@@ -27,15 +26,15 @@
         if not self._skip_wrapper_lookup:
             obj = self.proxied_object
             interface = self.proxied_interface
             if obj:
                 if old_hasattr(interface, name):
                     return getattr(obj, name)
             return getattr(interface, name)
-        raise_(AttributeError, "Does not have attribute %s" % name)
+        raise_(AttributeError, f"Does not have attribute {name}")
         return None
 
     def __setattr__(self, name, value):
         obj = self.proxied_object
         interface = self.proxied_interface
         if obj and old_hasattr(interface, name):
             if self.proxy_old_hasattr(name):
```

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/Resource.py` & `ableton-control-surface-core-0.0.3/src/_Framework/Resource.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/SceneComponent.py` & `ableton-control-surface-core-0.0.3/src/_Framework/SceneComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/ScrollComponent.py` & `ableton-control-surface-core-0.0.3/src/_Framework/ScrollComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/SessionComponent.py` & `ableton-control-surface-core-0.0.3/src/_Framework/SessionComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/SessionRecordingComponent.py` & `ableton-control-surface-core-0.0.3/src/_Framework/SessionRecordingComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/SessionZoomingComponent.py` & `ableton-control-surface-core-0.0.3/src/_Framework/SessionZoomingComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/Signal.py` & `ableton-control-surface-core-0.0.3/src/_Framework/Signal.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/Skin.py` & `ableton-control-surface-core-0.0.3/src/_Framework/Skin.py`

 * *Files 19% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                 else:
                     self._colors[pathname + k] = v
 
     def __getitem__(self, key):
         try:
             return self._colors[key]
         except KeyError:
-            raise_(SkinColorMissingError, "Skin color missing: %s" % str(key))
+            raise_(SkinColorMissingError, f"Skin color missing: {key!s}")
 
     def iteritems(self):
         return iter(self._colors.items())
 
 
 def merge_skins(*skins):
     skin = Skin()
```

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/SlideComponent.py` & `ableton-control-surface-core-0.0.3/src/_Framework/SlideComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/SliderElement.py` & `ableton-control-surface-core-0.0.3/src/_Framework/SliderElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/SubjectSlot.py` & `ableton-control-surface-core-0.0.3/src/_Framework/SubjectSlot.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/SysexValueControl.py` & `ableton-control-surface-core-0.0.3/src/_Framework/SysexValueControl.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/Task.py` & `ableton-control-surface-core-0.0.3/src/_Framework/Task.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/ToggleComponent.py` & `ableton-control-surface-core-0.0.3/src/_Framework/ToggleComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/TrackArmState.py` & `ableton-control-surface-core-0.0.3/src/_Framework/TrackArmState.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/TransportComponent.py` & `ableton-control-surface-core-0.0.3/src/_Framework/TransportComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/Util.py` & `ableton-control-surface-core-0.0.3/src/_Framework/Util.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,20 +6,19 @@
 # Compiled at: 2023-11-21 10:21:18
 # Size of source mod 2**32: 22318 bytes
 from contextlib import contextmanager, suppress
 from functools import partial, reduce, wraps
 from itertools import chain
 from numbers import Number
 
+from ableton.v2.base import old_hasattr
 from future import standard_library
 from future.moves.itertools import zip_longest
 from future.utils import raise_
 
-from ableton.v2.base import old_hasattr
-
 standard_library.install_aliases()
 
 
 def clamp(val, minv, maxv):
     return max(minv, min(val, maxv))
 
 
@@ -84,15 +83,15 @@
     return wrapper
 
 
 @memoize
 def mixin(*args):
     if len(args) == 1:
         return args[0]
-    name = "Mixin_%s" % "_".join(cls.__name__ for cls in args)
+    name = "Mixin_{}".format("_".join(cls.__name__ for cls in args))
     return type(str(name), args, {})
 
 
 def monkeypatch(target, name=None, override=False, doc=None):
     def patcher(func):
         patchname = func.__name__ if name is None else name
         if not override:
```

### Comparing `ableton-control-surface-core-0.0.2/src/_Framework/ViewControlComponent.py` & `ableton-control-surface-core-0.0.3/src/_Framework/ViewControlComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Generic/Devices.py` & `ableton-control-surface-core-0.0.3/src/_Generic/Devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 # Decompiled from: Python 3.7.16 (default, Jan 17 2023, 09:28:58)
 # [Clang 14.0.6 ]
 # Embedded file name: output/Live/mac_universal_64_static/Release/python-bundle/MIDI Remote Scripts/_Generic/Devices.py
 # Compiled at: 2023-12-21 15:35:35
 # Size of source mod 2**32: 42603 bytes
 from functools import partial
 
-from past.utils import old_div
-
 from _Framework.Util import group
+from past.utils import old_div
 
 RCK_BANK1 = ("Macro 1", "Macro 2", "Macro 3", "Macro 4", "Macro 5", "Macro 6", "Macro 7", "Macro 8")
 RCK_BANK2 = ("Macro 9", "Macro 10", "Macro 11", "Macro 12", "Macro 13", "Macro 14", "Macro 15", "Macro 16")
 RCK_BANKS = (RCK_BANK1, RCK_BANK2)
 RCK_BOBS = (RCK_BANK1,)
 RCK_BNK_NAMES = ("Macros", "Macros 2")
 ALG_BANK1 = (
```

### Comparing `ableton-control-surface-core-0.0.2/src/_Generic/GenericScript.py` & `ableton-control-surface-core-0.0.3/src/_Generic/GenericScript.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,28 +3,27 @@
 # Decompiled from: Python 3.7.16 (default, Jan 17 2023, 09:28:58)
 # [Clang 14.0.6 ]
 # Embedded file name: output/Live/mac_universal_64_static/Release/python-bundle/MIDI Remote Scripts/_Generic/GenericScript.py
 # Compiled at: 2023-11-21 10:21:18
 # Size of source mod 2**32: 16711 bytes
 from functools import partial
 
-from future.utils import iteritems
-
 import Live
 from _Framework import (
     ButtonElement,
     ButtonMatrixElement,
     ControlSurface,
     DeviceComponent,
     EncoderElement,
     Layer,
     TransportComponent,
 )
 from _Framework.InputControlElement import MIDI_CC_TYPE
 from _Framework.Util import NamedTuple
+from future.utils import iteritems
 
 from .SpecialMixerComponent import SpecialMixerComponent
 
 
 def is_valid_midi_channel(integer):
     return 0 <= integer < 16
```

### Comparing `ableton-control-surface-core-0.0.2/src/_Generic/SelectChanStripComponent.py` & `ableton-control-surface-core-0.0.3/src/_Generic/SelectChanStripComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Generic/SpecialMixerComponent.py` & `ableton-control-surface-core-0.0.3/src/_Generic/SpecialMixerComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Generic/util.py` & `ableton-control-surface-core-0.0.3/src/_Generic/util.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_MxDCore/ControlSurfaceWrapper.py` & `ableton-control-surface-core-0.0.3/src/_MxDCore/ControlSurfaceWrapper.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_MxDCore/LomTypes.py` & `ableton-control-surface-core-0.0.3/src/_MxDCore/LomTypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 # Embedded file name: output/Live/mac_universal_64_static/Release/python-bundle/MIDI Remote Scripts/_MxDCore/LomTypes.py
 # Compiled at: 2023-12-21 15:35:35
 # Size of source mod 2**32: 41914 bytes
 import ast
 import json
 from collections import namedtuple
 
-from past.builtins import basestring
-
 import Live
 from _Framework import ControlElement, ControlSurface, ControlSurfaceComponent
 from _Framework.Util import is_iterable
-from _MxDCore.ControlSurfaceWrapper import ControlProxy, ControlSurfaceWrapper
 from ableton.v2.base import old_hasattr
+from past.builtins import basestring
+
+from _MxDCore.ControlSurfaceWrapper import ControlProxy, ControlSurfaceWrapper
 
 
 class MFLPropertyFormats:
     Default, JSON = (0, 1)
 
 
 _MFLProperty = namedtuple("MFLProperty", "name format to_json from_json min_epii_version")
@@ -125,15 +125,15 @@
 
 def routing_channel_to_json(device):
     return routing_object_to_json(device, "routing_channel")
 
 
 def json_to_routing_object(obj, property_name, json_dict):
     verify_routings_available_for_object(obj, property_name)
-    objects = getattr(obj, "available_%ss" % property_name, [])
+    objects = getattr(obj, f"available_{property_name}s", [])
     identifier = json_to_data_dict(property_name, json_dict)["identifier"]
     for routing_object in objects:
         if hash(routing_object) == identifier:
             return routing_object
     return None
```

### Comparing `ableton-control-surface-core-0.0.2/src/_MxDCore/LomUtils.py` & `ableton-control-surface-core-0.0.3/src/_MxDCore/LomUtils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,16 @@
 # Embedded file name: output/Live/mac_universal_64_static/Release/python-bundle/MIDI Remote Scripts/_MxDCore/LomUtils.py
 # Compiled at: 2023-12-21 15:35:35
 # Size of source mod 2**32: 14785 bytes
 import contextlib
 import sys
 import types
 
-from past.builtins import basestring
-
 from ableton.v2.base import liveobj_valid, old_hasattr
+from past.builtins import basestring
 
 from .ControlSurfaceWrapper import is_real_control_surface
 from .LomTypes import (
     ENUM_TYPES,
     EXTRA_CS_FUNCTIONS,
     PROPERTY_TYPES,
     ROOT_KEYS,
@@ -38,15 +37,15 @@
 
 
 def create_lom_doc_string(lom_object):
     description = ""
     if old_hasattr(lom_object, "__doc__"):
         if isinstance(lom_object.__doc__, basestring):
             if len(lom_object.__doc__) > 0:
-                description = "description %s" % lom_object.__doc__.replace("\n", " ").replace(",", "\\,")
+                description = "description {}".format(lom_object.__doc__.replace("\n", " ").replace(",", "\\,"))
     return description
 
 
 class LomInformation:
     def __init__(self, lom_object, epii_version, *a, **k):
         (super().__init__)(*a, **k)
         self._lists_of_children = []
@@ -344,22 +343,22 @@
                             lom_object = tuple_wrapper.get_list()[index]
                         else:
                             lom_object = lom_object[index]
                     else:
                         lom_object = getattr(lom_object, component)
                     components.append(lom_object)
                 except IndexError:
-                    raise LomAttributeError("invalid index of component '%s'" % prev_component)
+                    raise LomAttributeError(f"invalid index of component '{prev_component}'")
                 except AttributeError:
-                    raise LomAttributeError("invalid path component '%s'" % component)
+                    raise LomAttributeError(f"invalid path component '{component}'")
                 else:
                     prev_component = component
 
             if not is_lom_object(lom_object, self._lom_classes):
-                raise LomObjectError("component '%s' is not an object" % prev_component)
+                raise LomObjectError(f"component '{prev_component}' is not an object")
             return lom_object
         return None
 
     def _calculate_object_from_path(self, path_components):
         lom_object = None
         if len(path_components) > 0:
             selector = (
```

### Comparing `ableton-control-surface-core-0.0.2/src/_MxDCore/MxDControlSurfaceAPI.py` & `ableton-control-surface-core-0.0.3/src/_MxDCore/MxDControlSurfaceAPI.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 # [Clang 14.0.6 ]
 # Embedded file name: output/Live/mac_universal_64_static/Release/python-bundle/MIDI Remote Scripts/_MxDCore/MxDControlSurfaceAPI.py
 # Compiled at: 2023-11-21 10:21:18
 # Size of source mod 2**32: 7323 bytes
 import contextlib
 from collections import namedtuple
 
+from ableton.v2.base import old_hasattr
 from future.utils import string_types
 
 from _MxDCore.ControlSurfaceWrapper import WrapperRegistry
 from _MxDCore.LomTypes import get_control_surfaces, is_control_surface
-from ableton.v2.base import old_hasattr
 
 RECEIVE_MIDI_TIMEOUT = 0.2
 
 
 def midi_byte_to_int(byte):
     if isinstance(byte, string_types):
         return int(byte, 0)
```

### Comparing `ableton-control-surface-core-0.0.2/src/_MxDCore/MxDCore.py` & `ableton-control-surface-core-0.0.3/src/_MxDCore/MxDCore.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,20 +6,19 @@
 # Compiled at: 2023-12-21 15:35:35
 # Size of source mod 2**32: 67065 bytes
 import contextlib
 import json
 import logging
 from functools import partial, reduce, wraps
 
-from future.utils import string_types
-
 import _Framework
 import Live.Base
 from _Framework import Disconnectable
 from ableton.v2.base import old_hasattr
+from future.utils import string_types
 
 from .LomTypes import (
     CONTROL_SURFACES,
     ENUM_TYPES,
     LIVE_APP,
     PROPERTY_TYPES,
     ROOT_KEYS,
@@ -466,19 +465,19 @@
             object_type = get_object_type_name(current_object)
         self.manager.send_message(device_id, object_id, "obj_type", str(object_type))
 
     def obj_get_info(self, device_id, object_id, parameters):
         current_object = self._get_current_lom_object(device_id, object_id)
         object_info = "No object"
         if current_object is not None:
-            object_info = "id %s\n" % str(self._get_lom_id_by_lom_object(current_object))
+            object_info = f"id {self._get_lom_id_by_lom_object(current_object)!s}\n"
             current_object = self._disambiguate_object(current_object)
             lom_info = LomInformation(current_object, self.epii_version)
-            object_info += "type %s\n" % str(get_object_type_name(current_object))
-            object_info += "%s\n" % lom_info.description
+            object_info += f"type {get_object_type_name(current_object)!s}\n"
+            object_info += f"{lom_info.description}\n"
             if not is_object_iterable(current_object):
 
                 def accumulate_info(info_list, label):
                     result = ""
                     if len(info_list) > 0:
                         str_format = "%s %s %s\n" if len(info_list[0]) > 1 else "%s %s\n"
                         formatter = lambda info: str_format % ((label, *info))
@@ -647,15 +646,15 @@
                     reason = "Invalid " + ("arguments" if isinstance(e, TypeError) else "syntax")
                     self._print_error(device_id, object_id, f"{reason}: '{to_str(param_comps)}'")
                 finally:
                     e = None
                     del e
 
         else:
-            self._print_error(device_id, object_id, "call %s: no valid object set" % to_str(param_comps))
+            self._print_error(device_id, object_id, f"call {to_str(param_comps)}: no valid object set")
 
     def obs_set_id(self, device_id, object_id, parameter):
         if self._is_integer(parameter) and self._lom_id_exists(device_id, int(parameter)):
             self.device_contexts[device_id][object_id][LAST_SENT_ID_KEY] = None
             self._set_current_lom_id(device_id, object_id, int(parameter), "obs")
         else:
             self._print_error(device_id, object_id, "set id: invalid id")
@@ -766,27 +765,27 @@
         self._uninstall_path_listeners(device_id, object_id)
         listener = partial(listener_callback, device_id, object_id)
         obj_attr_iter = self._object_attr_path_iter(device_id, object_id, path_components)
         for lom_object, attribute in obj_attr_iter:
             attribute = self._listenable_property_for(attribute)
             if lom_object is not None:
                 if old_hasattr(lom_object, attribute + "_has_listener"):
-                    getattr(lom_object, "add_%s_listener" % attribute)(listener)
+                    getattr(lom_object, f"add_{attribute}_listener")(listener)
                     new_listeners[(lom_object, attribute)] = listener
 
         object_context[PATH_LISTENER_KEY] = new_listeners
 
     def _uninstall_path_listeners(self, device_id, object_id):
         device_context = self.device_contexts[device_id]
         object_context = device_context[object_id]
         old_listeners = object_context[PATH_LISTENER_KEY]
         for (lom_object, attribute), listener in old_listeners.items():
             if lom_object is not None:
                 if getattr(lom_object, attribute + "_has_listener")(listener):
-                    getattr(lom_object, "remove_%s_listener" % attribute)(listener)
+                    getattr(lom_object, f"remove_{attribute}_listener")(listener)
 
     def _path_listener_callback(self, device_id, object_id):
         device_context = self.device_contexts[device_id]
         object_context = device_context[object_id]
         resulting_id = self._get_lom_id_by_lom_object(
             self._object_from_path(device_id, object_id, (object_context[PATH_KEY]), must_exist=False),
         )
@@ -1062,15 +1061,15 @@
 
             self._stop_note_operation(device_id, object_id)
         else:
             self._print_error(device_id, object_id, "no operation in progress")
 
     def _create_notes_output(self, notes):
         element_format = lambda el: str(int(el) if isinstance(el, bool) else el)
-        note_format = lambda note: "note %s\n" % concatenate_strings(list(map(element_format, note)))
+        note_format = lambda note: f"note {concatenate_strings(list(map(element_format, note)))}\n"
         return "notes %d\n%sdone" % (
             len(notes),
             concatenate_strings((list(map(note_format, notes))), string_format="%s%s"),
         )
 
     def _midi_note_vector_to_dict_output(self, notes, properties_to_return):
         return data_dict_to_json("notes", [midi_note_to_dict(note, properties_to_return) for note in notes])
@@ -1163,15 +1162,15 @@
         else:
             if current_object is not None:
                 if property_name != "":
                     object_context = self.device_contexts[device_id][object_id]
                     listener_callback = partial(self._observer_property_callback, device_id, object_id)
                     transl_prop_name = self._listenable_property_for(property_name)
                     if old_hasattr(current_object, transl_prop_name + "_has_listener"):
-                        getattr(current_object, "add_%s_listener" % transl_prop_name)(listener_callback)
+                        getattr(current_object, f"add_{transl_prop_name}_listener")(listener_callback)
                         object_context[PROP_LISTENER_KEY] = (listener_callback, current_object, property_name)
                         listener_callback()
                     else:
                         if old_hasattr(current_object, transl_prop_name):
                             self._print_warning(device_id, object_id, "property cannot be listened to")
 
     def _observer_uninstall_listener(self, device_id, object_id):
@@ -1179,15 +1178,15 @@
         object_context = device_context[object_id]
         self._uninstall_path_listeners(device_id, object_id)
         listener_callback, current_object, property_name = object_context[PROP_LISTENER_KEY]
         if current_object is not None:
             if listener_callback is not None:
                 transl_prop_name = self._listenable_property_for(property_name)
                 if getattr(current_object, transl_prop_name + "_has_listener")(listener_callback):
-                    getattr(current_object, "remove_%s_listener" % transl_prop_name)(listener_callback)
+                    getattr(current_object, f"remove_{transl_prop_name}_listener")(listener_callback)
         object_context[PROP_LISTENER_KEY] = (None, None, None)
 
     def _observer_property_message_type(self, prop, prop_info):
         prop_type = None
         if prop_info and prop_info.format == MFLPropertyFormats.JSON:
             prop_type = "obs_dict_val"
         else:
```

### Comparing `ableton-control-surface-core-0.0.2/src/_MxDCore/MxDUtils.py` & `ableton-control-surface-core-0.0.3/src/_MxDCore/MxDUtils.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 # Decompiled from: Python 3.7.16 (default, Jan 17 2023, 09:28:58)
 # [Clang 14.0.6 ]
 # Embedded file name: output/Live/mac_universal_64_static/Release/python-bundle/MIDI Remote Scripts/_MxDCore/MxDUtils.py
 # Compiled at: 2023-11-21 10:21:18
 # Size of source mod 2**32: 9496 bytes
 import logging
 
-from future.utils import string_types
-
 from ableton.v2.base import old_hasattr
+from future.utils import string_types
 
 logger = logging.getLogger(__name__)
 
 
 class TupleWrapper:
     _tuple_wrapper_registry = {}
```

### Comparing `ableton-control-surface-core-0.0.2/src/_MxDCore/NotesAPIUtils.py` & `ableton-control-surface-core-0.0.3/src/_MxDCore/NotesAPIUtils.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_MxDCore/__init__.py` & `ableton-control-surface-core-0.0.3/src/_MxDCore/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Userscript/DeviceComponent.py` & `ableton-control-surface-core-0.0.3/src/_Userscript/DeviceComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/_Userscript/__init__.py` & `ableton-control-surface-core-0.0.3/src/_Userscript/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/base/__init__.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/base/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/base/abl_signal.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/base/abl_signal.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/base/collection/indexed_dict.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/base/collection/indexed_dict.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/base/dependency.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/base/dependency.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 _global_injection_registry = InjectionRegistry()
 
 
 def get_dependency_for(name, default=None):
     accessor = _global_injection_registry.get(name, default)
     if accessor is not None:
         return accessor()
-    raise DependencyError("Required dependency %s not provided" % name)
+    raise DependencyError(f"Required dependency {name} not provided")
 
 
 class dependency:
     def __init__(self, **k):
         self._dependency_name, self._dependency_default = next(iter(k.items()))
 
     def __get__(self, _, cls=None):
```

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/base/disconnectable.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/base/disconnectable.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/base/event.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/base/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -358,26 +358,26 @@
         (super().__init__)(*a, **k)
         self._default_value = default_value
         self._property_name = None
         self._member_name = None
 
     def set_property_name(self, property_name):
         self._property_name = property_name
-        self._member_name = "__listenable_property_%s" % property_name
+        self._member_name = f"__listenable_property_{property_name}"
 
     def _get_value(self, obj):
         return getattr(obj, self._member_name, self._default_value)
 
     def __get__(self, obj, owner):
         return self._get_value(obj)
 
     def __set__(self, obj, value):
         if value != self._get_value(obj):
             setattr(obj, self._member_name, value)
-            getattr(obj, "notify_%s" % self._property_name)(value)
+            getattr(obj, f"notify_{self._property_name}")(value)
 
 
 class SerializableListenablePropertiesMeta(EventObjectMeta):
     def __new__(cls, name, bases, dct):
         listenable_properties = EventObjectMeta.collect_listenable_properties(dct)
 
         def getstate(self):
```

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/base/gcutil.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/base/gcutil.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/base/isclose.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/base/isclose.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/base/live_api_utils.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/base/live_api_utils.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/base/proxy.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/base/proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             interface = self.proxied_interface
             if obj:
                 if old_hasattr(interface, name):
                     return getattr(obj, name)
             if interface:
                 if old_hasattr(interface, name):
                     return getattr(interface, name)
-        raise AttributeError("Does not have attribute %s" % name)
+        raise AttributeError(f"Does not have attribute {name}")
 
     def __setattr__(self, name, value):
         obj = self.proxied_object
         interface = self.proxied_interface
         if obj and old_hasattr(interface, name):
             if self.proxy_old_hasattr(name):
                 raise AttributeError(f"Ambiguous set attribute: {name} proxied: {obj}")
```

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/base/task.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/base/task.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/base/util.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/base/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     return wrapper
 
 
 @memoize
 def mixin(*args):
     if len(args) == 1:
         return args[0]
-    name = "Mixin_%s" % "_".join(cls.__name__ for cls in args)
+    name = "Mixin_{}".format("_".join(cls.__name__ for cls in args))
     return type(str(name), args, {})
 
 
 def monkeypatch(target, name=None, override=False, doc=None):
     def patcher(func):
         patchname = func.__name__ if name is None else name
         if not override:
```

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/__init__.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/banking_util.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/banking_util.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/capabilities.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/capabilities.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/clip_creator.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/clip_creator.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/component.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/__init__.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/accent.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/accent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/auto_arm.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/auto_arm.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/background.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/background.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/channel_strip.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/channel_strip.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,30 +67,30 @@
         self._track_name_data_source = DisplayDataSource()
         self._update_track_name_data_source()
         self._empty_control_slots = self.register_disconnectable(EventObject())
         self._ChannelStripComponent__on_selected_track_changed.subject = self.song.view
 
         def make_property_slot(name, alias=None):
             alias = alias or name
-            return self.register_slot(None, getattr(self, "_on_%s_changed" % alias), name)
+            return self.register_slot(None, getattr(self, f"_on_{alias}_changed"), name)
 
         self._track_property_slots = [
             make_property_slot("mute"),
             make_property_slot("solo"),
             make_property_slot("arm"),
             make_property_slot("input_routing_type", "input_routing"),
             make_property_slot("name", "track_name"),
         ]
         self._mixer_device_property_slots = [
             make_property_slot("crossfade_assign", "cf_assign"),
             make_property_slot("sends"),
         ]
 
         def make_button_slot(name):
-            return self.register_slot(None, getattr(self, "_%s_value" % name), "value")
+            return self.register_slot(None, getattr(self, f"_{name}_value"), "value")
 
         self._mute_button_slot = make_button_slot("mute")
         self._solo_button_slot = make_button_slot("solo")
         self._arm_button_slot = make_button_slot("arm")
         self._shift_button_slot = make_button_slot("shift")
         self._crossfade_toggle_slot = make_button_slot("crossfade_toggle")
```

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/clip_actions.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/clip_actions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # decompyle3 version 3.9.0
 # Python bytecode version base 3.7.0 (3394)
 # Decompiled from: Python 3.7.16 (default, Jan 17 2023, 09:28:58)
 # [Clang 14.0.6 ]
 # Embedded file name: output/Live/mac_universal_64_static/Release/python-bundle/MIDI Remote Scripts/ableton/v2/control_surface/components/clip_actions.py
 # Compiled at: 2023-11-21 10:21:18
 # Size of source mod 2**32: 3021 bytes
-from control_surface.control import ButtonControl
-
 import Live
+from control_surface.control import ButtonControl
 
 from ...base import duplicate_clip_loop, listens, liveobj_valid
 from ...control_surface import Component
 
 
 class ClipActionsComponent(Component):
     delete_button = ButtonControl(color="Action.Available")
```

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/clip_slot.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/clip_slot.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/device.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/device.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/device_navigation.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/device_navigation.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/device_parameters.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/device_parameters.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/drum_group.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/drum_group.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/item_lister.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/item_lister.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/mixer.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/mixer.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/playable.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/playable.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/scene.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/scene.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/scroll.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/scroll.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/session.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/session.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/session_navigation.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/session_navigation.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/session_overview.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/session_overview.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/session_recording.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/session_recording.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/session_ring.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/session_ring.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/slide.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/slide.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/target_track.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/target_track.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/toggle.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/toggle.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/transport.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/transport.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/undo_redo.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/undo_redo.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/components/view_control.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/components/view_control.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/compound_element.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/compound_element.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/control/__init__.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/control/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/control/button.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/control/button.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/control/control.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/control/control.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/control/control_list.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/control/control_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,20 +261,20 @@
 _control_list_classes = {}
 _control_matrix_classes = {}
 
 
 def control_list(control_type, *a, **k):
     if control_type == RadioButtonControl:
         return RadioButtonGroup(*a, **k)
-    c = _control_list_classes.get(control_type, None)
+    c = _control_list_classes.get(control_type)
     if not c:
         c = mixin(ControlList, control_type)
         _control_list_classes[control_type] = c
     return c(control_type, *a, **k)
 
 
 def control_matrix(control_type, *a, **k):
-    m = _control_matrix_classes.get(control_type, None)
+    m = _control_matrix_classes.get(control_type)
     if not m:
         m = mixin(MatrixControl, control_type)
         _control_matrix_classes[control_type] = m
     return m(control_type, *a, **k)
```

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/control/encoder.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/control/encoder.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/control/mapped.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/control/mapped.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/control/radio_button.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/control/radio_button.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/control/sysex.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/control/sysex.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/control/text_display.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/control/text_display.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/control/toggle_button.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/control/toggle_button.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/control_element.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/control_element.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/control_surface.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/control_surface.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,17 +9,16 @@
 import traceback
 from collections import OrderedDict
 from contextlib import contextmanager
 from functools import partial
 from itertools import chain
 from pickle import dumps, loads
 
-from future.utils import iteritems, itervalues
-
 import Live
+from future.utils import iteritems, itervalues
 
 from ..base import (
     BooleanContext,
     EventObject,
     const,
     find_if,
     first,
```

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/decoration.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/decoration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # decompyle3 version 3.9.0
 # Python bytecode version base 3.7.0 (3394)
 # Decompiled from: Python 3.7.16 (default, Jan 17 2023, 09:28:58)
 # [Clang 14.0.6 ]
 # Embedded file name: output/Live/mac_universal_64_static/Release/python-bundle/MIDI Remote Scripts/ableton/v2/control_surface/decoration.py
 # Compiled at: 2023-11-21 10:21:18
 # Size of source mod 2**32: 13913 bytes
-from future.utils import iteritems
-
 import Live
+from future.utils import iteritems
 from Push2.device_options import DeviceOnOffOption, DeviceSwitchOption
 
 from ..base import (
     CompoundDisconnectable,
     EventObject,
     Proxy,
     clamp,
```

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/default_bank_definitions.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/default_bank_definitions.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/defaults.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/defaults.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/delay_decoration.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/delay_decoration.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/device_bank_registry.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/device_bank_registry.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     def compact_registry(self):
         newreg = dict(filter(lambda kv: liveobj_valid(kv[0]), self._device_bank_registry.items()))
         self._device_bank_registry = newreg
 
     def set_device_bank(self, device, bank):
         key = self._find_device_bank_key(device) or device
-        old = self._device_bank_registry[key] if key in self._device_bank_registry else 0
+        old = self._device_bank_registry.get(key, 0)
         if old != bank:
             self._device_bank_registry[key] = bank
             self.notify_device_bank(device, bank)
 
     def get_device_bank(self, device):
         if hasattr(device, "bank_index"):
             return device.bank_index
```

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/device_chain_utils.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/device_chain_utils.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/device_decorator_factory.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/device_decorator_factory.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/device_parameter_bank.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/device_parameter_bank.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/device_provider.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/device_provider.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/drift_decoration.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/drift_decoration.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/elements/__init__.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/elements/button.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/elements/button.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # decompyle3 version 3.9.0
 # Python bytecode version base 3.7.0 (3394)
 # Decompiled from: Python 3.7.16 (default, Jan 17 2023, 09:28:58)
 # [Clang 14.0.6 ]
 # Embedded file name: output/Live/mac_universal_64_static/Release/python-bundle/MIDI Remote Scripts/ableton/v2/control_surface/elements/button.py
 # Compiled at: 2023-11-21 10:21:18
 # Size of source mod 2**32: 4323 bytes
-from past.builtins import long
-
 import Live
+from past.builtins import long
 
 from ...base import BooleanContext, const, has_event, in_range, listens, old_hasattr
 from ..input_control_element import InputControlElement
 from ..skin import Skin
 from .color import Color
```

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/elements/button_matrix.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/elements/button_matrix.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/elements/button_slider.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/elements/button_slider.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/elements/color.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/elements/color.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/elements/combo.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/elements/combo.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/elements/display_data_source.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/elements/display_data_source.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/elements/encoder.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/elements/encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # decompyle3 version 3.9.0
 # Python bytecode version base 3.7.0 (3394)
 # Decompiled from: Python 3.7.16 (default, Jan 17 2023, 09:28:58)
 # [Clang 14.0.6 ]
 # Embedded file name: output/Live/mac_universal_64_static/Release/python-bundle/MIDI Remote Scripts/ableton/v2/control_surface/elements/encoder.py
 # Compiled at: 2023-11-21 10:21:18
 # Size of source mod 2**32: 9830 bytes
-from past.utils import old_div
-
 import Live
+from past.utils import old_div
 
 from ...base import Event, clamp, const, in_range, listens, nop
 from ..compound_element import CompoundElement
 from ..input_control_element import MIDI_CC_TYPE, InputControlElement, InputSignal
 from .combo import WrapperElement
 
 _map_modes = map_modes = Live.MidiMap.MapMode
@@ -85,15 +84,15 @@
             self.encoder_sensitivity = encoder_sensitivity
         if map_mode is _map_modes.absolute_14_bit and identifier > MAX_14_BIT_CC:
             self._map_mode = _map_modes.absolute
         else:
             self._map_mode = map_mode
         self._last_received_value = None
         self._value_normalizer = ENCODER_VALUE_NORMALIZER.get(map_mode, _not_implemented)
-        self._value_accumulator = ENCODER_VALUE_ACCUMULATOR.get(map_mode, None)
+        self._value_accumulator = ENCODER_VALUE_ACCUMULATOR.get(map_mode)
         self._half_value_range = self._max_value / 2
 
     def message_map_mode(self):
         return self._map_mode
 
     def receive_value(self, value):
         super().receive_value(value)
```

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/elements/full_velocity_element.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/elements/full_velocity_element.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/elements/logical_display_segment.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/elements/logical_display_segment.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/elements/optional.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/elements/optional.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/elements/physical_display.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/elements/physical_display.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/elements/playhead_element.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/elements/playhead_element.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/elements/proxy_element.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/elements/proxy_element.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/elements/slider.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/elements/slider.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/elements/sysex_element.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/elements/sysex_element.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/elements/velocity_levels_element.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/elements/velocity_levels_element.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/identifiable_control_surface.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/identifiable_control_surface.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/input_control_element.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/input_control_element.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/internal_parameter.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/internal_parameter.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 # Decompiled from: Python 3.7.16 (default, Jan 17 2023, 09:28:58)
 # [Clang 14.0.6 ]
 # Embedded file name: output/Live/mac_universal_64_static/Release/python-bundle/MIDI Remote Scripts/ableton/v2/control_surface/internal_parameter.py
 # Compiled at: 2023-11-21 10:21:18
 # Size of source mod 2**32: 14408 bytes
 import contextlib
 
-from past.builtins import unicode
-
 from Live import DeviceParameter
+from past.builtins import unicode
 
 from ..base import EventError, EventObject, Slot, clamp, listenable_property, liveobj_valid, nop
 
 
 def identity(value, _parent):
     return value
```

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/layer.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/layer.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/message_scheduler.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/message_scheduler.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/midi.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/midi.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/midi_map.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/midi_map.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/mode.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -442,29 +442,29 @@
             mode_color_basename = "Mode." + to_camel_case_name(mode_name)
             colors = {
                 "mode_selected_color": mode_color_basename + ".On",
                 "mode_unselected_color": mode_color_basename + ".Off",
                 "mode_group_active_color": mode_color_basename + ".On",
             }
         button_control = make_mode_button_control(self, mode_name, behaviour, **colors)
-        self.add_control("%s_button" % mode_name, button_control)
+        self.add_control(f"{mode_name}_button", button_control)
         self._update_mode_buttons(self.selected_mode)
 
     def _get_mode_behaviour(self, name):
         entry = self._mode_map.get(name, None)
         if entry is not None:
             return entry.behaviour
         return self.default_behaviour
 
     def get_mode(self, name):
         entry = self._mode_map.get(name, None)
         return entry and entry.mode
 
     def get_mode_button(self, name):
-        return getattr(self, "%s_button" % name)
+        return getattr(self, f"{name}_button")
 
     def _update_mode_buttons(self, selected):
         if self.is_enabled():
             for name, entry in iteritems(self._mode_map):
                 self._get_mode_behaviour(name).update_button(self, name, selected)
 
     @cycle_mode_button.pressed
```

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/parameter_provider.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/parameter_provider.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/parameter_slot_description.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/parameter_slot_description.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,19 +38,15 @@
     def _calc_content(self):
         parameter_name = self._default_parameter_name
         display_name_transformer = self._display_name_transformer
         for condition in self._conditions:
             result = True
             for subcond in condition[CONDITIONS_LIST_NAME_KEY]:
                 result = eval(
-                    "{} {} {}".format(
-                        result,
-                        subcond[OPERAND_NAME_KEY],
-                        subcond[PREDICATE_KEY](find_parameter(subcond[CONDITION_NAME_KEY], self._parameter_host)),
-                    ),
+                    f"{result} {subcond[OPERAND_NAME_KEY]} {subcond[PREDICATE_KEY](find_parameter(subcond[CONDITION_NAME_KEY], self._parameter_host))}",
                 )
                 if not result:
                     continue
 
             if result:
                 parameter_name = condition[RESULTING_NAME_KEY]
                 display_name_transformer = condition[DISPLAY_NAME_TRANSFORMER_KEY]
```

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/percussion_instrument_finder.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/percussion_instrument_finder.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/profile.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/profile.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 def profile(fn):
     if ENABLE_PROFILING:
 
         @wraps(fn)
         def wrapper(self, *a, **k):
             if PROFILER:
                 return PROFILER.runcall(partial(fn, self, *a, **k))
-            print("Can not profile (%s), it is probably reloaded" % fn.__name__)
+            print(f"Can not profile ({fn.__name__}), it is probably reloaded")
             return fn(*a, **k)
 
         return wrapper
     return fn
 
 
 def dump(name="default"):
```

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/resource.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/resource.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/roar_decoration.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/roar_decoration.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/session_ring_selection_linking.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/session_ring_selection_linking.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/simpler_decoration.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/simpler_decoration.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,19 @@
 # [Clang 14.0.6 ]
 # Embedded file name: output/Live/mac_universal_64_static/Release/python-bundle/MIDI Remote Scripts/ableton/v2/control_surface/simpler_decoration.py
 # Compiled at: 2023-11-21 10:21:18
 # Size of source mod 2**32: 14421 bytes
 from functools import partial
 from math import ceil, floor
 
+import Live
 from base.collection import IndexedDict
 from past.builtins import unicode
 from past.utils import old_div
 
-import Live
-
 from ..base import EventObject, clamp, listenable_property, listens, liveobj_valid, sign
 from .decoration import LiveObjectDecorator
 from .internal_parameter import (
     EnumWrappingParameter,
     IntegerParameter,
     RelativeInternalParameter,
     WrappingParameter,
```

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/simpler_slice_nudging.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/simpler_slice_nudging.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 # Decompiled from: Python 3.7.16 (default, Jan 17 2023, 09:28:58)
 # [Clang 14.0.6 ]
 # Embedded file name: output/Live/mac_universal_64_static/Release/python-bundle/MIDI Remote Scripts/ableton/v2/control_surface/simpler_slice_nudging.py
 # Compiled at: 2023-11-21 10:21:18
 # Size of source mod 2**32: 4529 bytes
 from contextlib import contextmanager
 
-from past.utils import old_div
-
 import Live
+from past.utils import old_div
 
 from ..base import EventObject, clamp, find_if, listens, liveobj_valid
 
 CENTERED_NUDGE_VALUE = 0.5
 MINIMUM_SLICE_DISTANCE = 2
```

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/skin.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/skin.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                         v = self._get_dynamic_color(v, song)
                     self._colors[pathname + k] = v
 
     def __getitem__(self, key):
         try:
             return self._colors[key]
         except KeyError:
-            raise SkinColorMissingError("Skin color missing: %s" % str(key))
+            raise SkinColorMissingError(f"Skin color missing: {key!s}")
 
     def iteritems(self):
         return iteritems(self._colors)
 
     def _get_dynamic_color(self, color_factory, song):
         if not liveobj_valid(song):
             raise DynamicColorNotAvailableError
```

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v2/control_surface/wavetable_decoration.py` & `ableton-control-surface-core-0.0.3/src/ableton/v2/control_surface/wavetable_decoration.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/base/__init__.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/base/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/base/util.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/base/util.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/__init__.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/banking_util.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/banking_util.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/capabilities.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/capabilities.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/colors.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/colors.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/component.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/component_map.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/component_map.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/__init__.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/accent.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/accent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/active_parameter.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/active_parameter.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/auto_arm.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/auto_arm.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/background.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/background.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/channel_strip.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/channel_strip.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/clip_actions.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/clip_actions.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/clip_slot.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/clip_slot.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/clipboard.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/clipboard.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/device.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/device.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/device_bank_navigation.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/device_bank_navigation.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/device_parameters.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/device_parameters.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/drum_group.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/drum_group.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/drum_group_scroll.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/drum_group_scroll.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/grid_resolution.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/grid_resolution.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/loop_selector.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/loop_selector.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/mixer.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/mixer.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/note_editor.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/note_editor.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/page.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/page.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/paginator.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/paginator.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/playable.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/playable.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/playhead.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/playhead.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/recording.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/recording.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/scene.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/scene.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/scroll.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/scroll.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/session.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/session.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/session_navigation.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/session_navigation.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/session_overview.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/session_overview.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/session_ring.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/session_ring.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/simple_device_navigation.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/simple_device_navigation.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/sliced_simpler.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/sliced_simpler.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/step_sequence.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/step_sequence.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/target_track.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/target_track.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/transport.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/transport.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/undo_redo.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/undo_redo.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/view_control.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/view_control.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/components/view_toggle.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/components/view_toggle.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/consts.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/control_surface.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/control_surface.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/control_surface_mapping.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/control_surface_mapping.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/control_surface_specification.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/control_surface_specification.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/controls/__init__.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/controls/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/controls/button.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/controls/button.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/controls/control.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/controls/control.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/controls/control_list.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/controls/control_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from ...base import mixin
 from . import RadioButtonGroup
 
 _control_list_types = {}
 
 
 def control_list(control_type, *a, **k):
-    factory = _control_list_types.get(control_type, None)
+    factory = _control_list_types.get(control_type)
     if not factory:
         factory = mixin(ControlList, control_type)
         _control_list_types[control_type] = factory
     return factory(control_type, *a, **k)
 
 
 class ControlList(ControlListBase):
```

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/controls/mapped.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/controls/mapped.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/controls/toggle_button.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/controls/toggle_button.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/default_bank_definitions.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/default_bank_definitions.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/default_skin.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/default_skin.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/device_decorators.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/device_decorators.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/__init__.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/display_specification.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/display_specification.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/event_signal/core.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/event_signal/core.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/event_signal/type_decl.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/event_signal/type_decl.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/notifications/__init__.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/notifications/all.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/notifications/all.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/notifications/default.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/notifications/default.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/notifications/meta.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/notifications/meta.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/notifications/type_decl.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/notifications/type_decl.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/notifications/util.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/notifications/util.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/renderable.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/renderable.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/state.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/state.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/text.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/text.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/type_decl.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/type_decl.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/util.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/util.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/view/__init__.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/view/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/view/notification.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/view/notification.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/view/type_decl.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/view/type_decl.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/view/util.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/view/util.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/display/view/view.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/display/view/view.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/elements/__init__.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/elements/button.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/elements/button.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/elements/button_matrix.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/elements/button_matrix.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/elements/color.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/elements/color.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/elements/discrete_values.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/elements/discrete_values.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/elements/display_line.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/elements/display_line.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/elements/encoder.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/elements/encoder.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/elements/lockable_button.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/elements/lockable_button.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/elements/lockable_combo.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/elements/lockable_combo.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/elements/sysex.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/elements/sysex.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/elements/touch.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/elements/touch.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/elements_base.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/elements_base.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/identification.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/identification.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/instrument_finder.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/instrument_finder.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/layer.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/layer.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/legacy_bank_definitions.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/legacy_bank_definitions.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Python bytecode version base 3.7.0 (3394)
 # Decompiled from: Python 3.7.16 (default, Jan 17 2023, 09:28:58)
 # [Clang 14.0.6 ]
 # Embedded file name: output/Live/mac_universal_64_static/Release/python-bundle/MIDI Remote Scripts/ableton/v3/control_surface/legacy_bank_definitions.py
 # Compiled at: 2023-11-21 10:21:18
 # Size of source mod 2**32: 1948 bytes
 from _Generic.Devices import BANK_NAME_DICT, DEVICE_BOB_DICT, DEVICE_DICT
+
 from ableton.v2.base.collection import IndexedDict
 
 from ..base import memoize
 from . import BANK_PARAMETERS_KEY
 
 BEST_OF_PARAMETERS_KEY = "Best of Parameters"
```

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/midi.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/midi.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/mode/__init__.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/mode/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/mode/behaviour.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/mode/behaviour.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/mode/mode.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/mode/mode.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/mode/modes.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/mode/modes.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             self._last_selected_mode = mode
 
     def get_mode(self, name):
         entry = self._mode_map.get(name, None)
         return entry and entry.mode
 
     def get_mode_button(self, name):
-        return getattr(self, "%s_button" % name)
+        return getattr(self, f"{name}_button")
 
     def get_mode_groups(self, name):
         entry = self._mode_map.get(name, None)
         if entry:
             return entry.groups
         return set()
```

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/mode/selector.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/mode/selector.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/parameter_info.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/parameter_info.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/parameter_mapping_sensitivities.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/parameter_mapping_sensitivities.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/session_ring_selection_linking.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/session_ring_selection_linking.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/control_surface/skin.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/control_surface/skin.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/live/__init__.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/live/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/live/action.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/live/action.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.2/src/ableton/v3/live/util.py` & `ableton-control-surface-core-0.0.3/src/ableton/v3/live/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 # Embedded file name: output/Live/mac_universal_64_static/Release/python-bundle/MIDI Remote Scripts/ableton/v3/live/util.py
 # Compiled at: 2023-11-21 10:21:18
 # Size of source mod 2**32: 12478 bytes
 from functools import singledispatch
 from typing import Any, Union
 
 import Live
+from Live import Clip, ClipSlot, DeviceParameter, MixerDevice, Scene
+
 from ableton.v2.base import liveobj_valid
 from ableton.v2.control_surface.components import find_nearest_color
 from ableton.v2.control_surface.internal_parameter import InternalParameterBase
-from Live import Clip, ClipSlot, DeviceParameter, MixerDevice, Scene
 
 from ..base import clamp, find_if, hex_to_rgb
 
 TRANSLATED_MIXER_PARAMETER_NAMES = {"Track Volume": "Volume", "Track Panning": "Pan"}
 UNDECLARED_QUANTIZED_PARAMETERS = {
     "AutoFilter": ("LFO Sync Rate",),
     "AutoPan": ("Sync Rate",),
```

### Comparing `ableton-control-surface-core-0.0.2/src/ableton_control_surface_core.egg-info/PKG-INFO` & `ableton-control-surface-core-0.0.3/src/ableton_control_surface_core.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ableton-control-surface-core
-Version: 0.0.2
+Version: 0.0.3
 Summary: Decompiled core packages from Ableton Live's Python API to help developers build custom control surfaces.
 Author-email: Martin Sahlen <martin8900@gmail.com>
 Project-URL: Homepage, https://github.com/oslo1989/ableton-control-surface-toolkit
 Project-URL: Issues, https://github.com/oslo1989/ableton-control-surface-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ableton-control-surface-core-0.0.2/src/ableton_control_surface_core.egg-info/SOURCES.txt` & `ableton-control-surface-core-0.0.3/src/ableton_control_surface_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

