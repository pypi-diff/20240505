# Comparing `tmp/terminaltexteffects-0.8.0.tar.gz` & `tmp/terminaltexteffects-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminaltexteffects-0.8.0.tar", max compression
+gzip compressed data, was "terminaltexteffects-0.9.0.tar", max compression
```

## Comparing `terminaltexteffects-0.8.0.tar` & `terminaltexteffects-0.9.0.tar`

### file list

```diff
@@ -1,54 +1,55 @@
--rwxr-xr-x   0        0        0     1072 2023-08-13 20:34:07.346818 terminaltexteffects-0.8.0/LICENSE
--rwxr-xr-x   0        0        0    90261 2024-04-26 11:02:43.515814 terminaltexteffects-0.8.0/README.md
--rwxr-xr-x   0        0        0      474 2024-04-26 11:07:09.808701 terminaltexteffects-0.8.0/pyproject.toml
--rwxr-xr-x   0        0        0        0 2023-08-12 13:15:55.921216 terminaltexteffects-0.8.0/terminaltexteffects/__init__.py
--rwxr-xr-x   0        0        0     1998 2024-04-26 11:00:38.365918 terminaltexteffects-0.8.0/terminaltexteffects/__main__.py
--rwxr-xr-x   0        0        0    10163 2024-04-14 17:40:09.477328 terminaltexteffects-0.8.0/terminaltexteffects/base_character.py
--rwxr-xr-x   0        0        0     2332 2024-04-26 11:00:38.366147 terminaltexteffects-0.8.0/terminaltexteffects/base_effect.py
--rwxr-xr-x   0        0        0        0 2023-07-22 17:59:37.688921 terminaltexteffects-0.8.0/terminaltexteffects/effects/__init__.py
--rwxr-xr-x   0        0        0    17319 2024-04-26 11:00:38.366596 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_beams.py
--rwxr-xr-x   0        0        0    15730 2024-04-26 11:00:38.366968 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_binarypath.py
--rwxr-xr-x   0        0        0    18729 2024-04-26 11:00:38.367369 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_blackhole.py
--rwxr-xr-x   0        0        0    10997 2024-04-26 11:00:38.367709 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_bouncyballs.py
--rwxr-xr-x   0        0        0    17694 2024-04-26 11:00:38.368114 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_bubbles.py
--rwxr-xr-x   0        0        0     7957 2024-04-26 11:00:38.368431 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_burn.py
--rwxr-xr-x   0        0        0    11118 2024-04-26 11:00:38.368776 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_crumble.py
--rwxr-xr-x   0        0        0    11360 2024-04-26 11:00:38.369124 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_decrypt.py
--rwxr-xr-x   0        0        0    13783 2024-04-26 11:00:38.369493 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_errorcorrect.py
--rwxr-xr-x   0        0        0     8058 2024-04-26 11:00:38.369870 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_expand.py
--rwxr-xr-x   0        0        0    13898 2024-04-26 11:00:38.370244 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_fireworks.py
--rwxr-xr-x   0        0        0    10189 2024-04-26 11:00:38.370591 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_middleout.py
--rwxr-xr-x   0        0        0    16681 2024-04-26 11:00:38.371134 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_orbittingvolley.py
--rwxr-xr-x   0        0        0    10624 2024-04-26 11:00:38.371723 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_overflow.py
--rwxr-xr-x   0        0        0    11864 2024-04-26 11:00:38.372078 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_pour.py
--rwxr-xr-x   0        0        0    11543 2024-04-26 11:00:38.372424 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_print.py
--rwxr-xr-x   0        0        0     9773 2024-04-26 11:00:38.372770 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_rain.py
--rwxr-xr-x   0        0        0     7365 2024-04-26 11:00:38.373084 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_random_sequence.py
--rwxr-xr-x   0        0        0    19662 2024-04-26 11:00:38.373495 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_rings.py
--rwxr-xr-x   0        0        0     8232 2024-04-26 11:00:38.373825 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_scattered.py
--rwxr-xr-x   0        0        0    13156 2024-04-26 11:00:38.374184 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_slide.py
--rwxr-xr-x   0        0        0    13617 2024-04-26 11:00:38.374560 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_spotlights.py
--rwxr-xr-x   0        0        0    10790 2024-04-26 11:00:38.374892 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_spray.py
--rwxr-xr-x   0        0        0    14721 2024-04-26 11:00:38.375249 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_swarm.py
--rwxr-xr-x   0        0        0    19976 2024-04-26 11:00:38.375649 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_synthgrid.py
--rwxr-xr-x   0        0        0    13830 2024-04-26 11:00:38.376011 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_unstable.py
--rwxr-xr-x   0        0        0     8500 2024-04-26 11:00:38.376337 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_verticalslice.py
--rwxr-xr-x   0        0        0    23371 2024-04-26 11:00:38.376751 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_vhstape.py
--rwxr-xr-x   0        0        0    10187 2024-04-26 11:00:38.377087 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_waves.py
--rwxr-xr-x   0        0        0     8564 2024-04-26 11:00:38.377413 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_wipe.py
--rwxr-xr-x   0        0        0        0 2024-04-12 11:52:35.092907 terminaltexteffects-0.8.0/terminaltexteffects/py.typed
--rwxr-xr-x   0        0        0     4762 2024-04-26 11:00:38.377749 terminaltexteffects-0.8.0/terminaltexteffects/template/effect_template.py
--rwxr-xr-x   0        0        0        0 2023-07-22 17:59:26.632934 terminaltexteffects-0.8.0/terminaltexteffects/utils/__init__.py
--rwxr-xr-x   0        0        0    20910 2024-03-19 15:49:53.316772 terminaltexteffects-0.8.0/terminaltexteffects/utils/animation.py
--rwxr-xr-x   0        0        0     2294 2024-03-01 12:06:27.830757 terminaltexteffects-0.8.0/terminaltexteffects/utils/ansitools.py
--rwxr-xr-x   0        0        0    14137 2024-04-26 11:00:38.378147 terminaltexteffects-0.8.0/terminaltexteffects/utils/arg_validators.py
--rwxr-xr-x   0        0        0    11651 2024-04-26 11:00:38.378501 terminaltexteffects-0.8.0/terminaltexteffects/utils/argsdataclass.py
--rwxr-xr-x   0        0        0     2225 2024-03-19 15:49:53.401996 terminaltexteffects-0.8.0/terminaltexteffects/utils/colorterm.py
--rwxr-xr-x   0        0        0    12421 2024-03-19 15:49:53.423980 terminaltexteffects-0.8.0/terminaltexteffects/utils/easing.py
--rwxr-xr-x   0        0        0        0 2024-04-26 11:00:38.378584 terminaltexteffects-0.8.0/terminaltexteffects/utils/exceptions.py
--rwxr-xr-x   0        0        0     9515 2024-03-28 11:00:09.260352 terminaltexteffects-0.8.0/terminaltexteffects/utils/geometry.py
--rwxr-xr-x   0        0        0     9115 2024-04-08 16:59:01.111903 terminaltexteffects-0.8.0/terminaltexteffects/utils/graphics.py
--rwxr-xr-x   0        0        0     6861 2024-03-19 15:49:53.451057 terminaltexteffects-0.8.0/terminaltexteffects/utils/hexterm.py
--rwxr-xr-x   0        0        0    17326 2024-03-19 15:49:53.462026 terminaltexteffects-0.8.0/terminaltexteffects/utils/motion.py
--rwxr-xr-x   0        0        0    25355 2024-04-26 11:00:38.379138 terminaltexteffects-0.8.0/terminaltexteffects/utils/terminal.py
--rw-r--r--   0        0        0    90791 1970-01-01 00:00:00.000000 terminaltexteffects-0.8.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2023-08-13 20:34:07.346818 terminaltexteffects-0.9.0/LICENSE
+-rwxr-xr-x   0        0        0    11802 2024-05-05 17:40:35.415508 terminaltexteffects-0.9.0/README.md
+-rwxr-xr-x   0        0        0      474 2024-05-05 17:42:21.861321 terminaltexteffects-0.9.0/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-08-12 13:15:55.921216 terminaltexteffects-0.9.0/terminaltexteffects/__init__.py
+-rwxr-xr-x   0        0        0     2000 2024-05-05 17:33:51.712767 terminaltexteffects-0.9.0/terminaltexteffects/__main__.py
+-rwxr-xr-x   0        0        0        0 2023-07-22 17:59:37.688921 terminaltexteffects-0.9.0/terminaltexteffects/effects/__init__.py
+-rwxr-xr-x   0        0        0    18085 2024-05-05 17:33:51.713740 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_beams.py
+-rwxr-xr-x   0        0        0    16120 2024-05-05 17:33:51.714107 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_binarypath.py
+-rwxr-xr-x   0        0        0    19300 2024-05-05 17:33:51.714496 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_blackhole.py
+-rwxr-xr-x   0        0        0    11021 2024-05-05 17:33:51.714822 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_bouncyballs.py
+-rwxr-xr-x   0        0        0    17875 2024-05-05 17:33:51.715218 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_bubbles.py
+-rwxr-xr-x   0        0        0     8339 2024-05-05 17:33:51.715538 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_burn.py
+-rwxr-xr-x   0        0        0    11659 2024-05-05 17:33:51.715867 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_crumble.py
+-rwxr-xr-x   0        0        0    11586 2024-05-05 17:33:51.716195 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_decrypt.py
+-rwxr-xr-x   0        0        0    13939 2024-05-05 17:33:51.716552 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_errorcorrect.py
+-rwxr-xr-x   0        0        0     7902 2024-05-05 17:33:51.716878 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_expand.py
+-rwxr-xr-x   0        0        0    14326 2024-05-05 17:33:51.717255 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_fireworks.py
+-rwxr-xr-x   0        0        0    10710 2024-05-05 17:33:51.717659 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_middleout.py
+-rwxr-xr-x   0        0        0    17434 2024-05-05 17:33:51.718058 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_orbittingvolley.py
+-rwxr-xr-x   0        0        0    11316 2024-05-05 17:33:51.718406 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_overflow.py
+-rwxr-xr-x   0        0        0    12513 2024-05-05 17:33:51.718766 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_pour.py
+-rwxr-xr-x   0        0        0    12234 2024-05-05 17:33:51.719204 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_print.py
+-rwxr-xr-x   0        0        0    10173 2024-05-05 17:33:51.719565 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_rain.py
+-rwxr-xr-x   0        0        0     7981 2024-05-05 17:33:51.719877 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_random_sequence.py
+-rwxr-xr-x   0        0        0    19899 2024-05-05 17:33:51.720292 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_rings.py
+-rwxr-xr-x   0        0        0     8394 2024-05-05 17:33:51.720652 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_scattered.py
+-rwxr-xr-x   0        0        0    13977 2024-05-05 17:33:51.721014 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_slide.py
+-rwxr-xr-x   0        0        0    14420 2024-05-05 17:33:51.721447 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_spotlights.py
+-rwxr-xr-x   0        0        0    11432 2024-05-05 17:33:51.721806 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_spray.py
+-rwxr-xr-x   0        0        0    15385 2024-05-05 17:33:51.722171 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_swarm.py
+-rwxr-xr-x   0        0        0    20593 2024-05-05 17:33:51.722595 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_synthgrid.py
+-rwxr-xr-x   0        0        0    13959 2024-05-05 17:33:51.722984 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_unstable.py
+-rwxr-xr-x   0        0        0     8650 2024-05-05 17:33:51.723333 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_verticalslice.py
+-rwxr-xr-x   0        0        0    22923 2024-05-05 17:33:51.723759 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_vhstape.py
+-rwxr-xr-x   0        0        0    10624 2024-05-05 17:33:51.724110 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_waves.py
+-rwxr-xr-x   0        0        0     9791 2024-05-05 17:33:51.724444 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_wipe.py
+-rwxr-xr-x   0        0        0        0 2024-05-05 17:33:51.724578 terminaltexteffects-0.9.0/terminaltexteffects/engine/__init__.py
+-rwxr-xr-x   0        0        0    22748 2024-05-05 17:33:51.741057 terminaltexteffects-0.9.0/terminaltexteffects/engine/animation.py
+-rwxr-xr-x   0        0        0    11162 2024-05-05 17:33:51.752448 terminaltexteffects-0.9.0/terminaltexteffects/engine/base_character.py
+-rwxr-xr-x   0        0        0     3656 2024-05-05 17:33:51.798186 terminaltexteffects-0.9.0/terminaltexteffects/engine/base_effect.py
+-rwxr-xr-x   0        0        0    22354 2024-05-05 17:33:51.800192 terminaltexteffects-0.9.0/terminaltexteffects/engine/motion.py
+-rwxr-xr-x   0        0        0    30059 2024-05-05 17:33:51.801858 terminaltexteffects-0.9.0/terminaltexteffects/engine/terminal.py
+-rwxr-xr-x   0        0        0        0 2024-04-12 11:52:35.092907 terminaltexteffects-0.9.0/terminaltexteffects/py.typed
+-rwxr-xr-x   0        0        0     4931 2024-05-05 17:33:51.816796 terminaltexteffects-0.9.0/terminaltexteffects/template/effect_template.py
+-rwxr-xr-x   0        0        0        0 2023-07-22 17:59:26.632934 terminaltexteffects-0.9.0/terminaltexteffects/utils/__init__.py
+-rwxr-xr-x   0        0        0     2432 2024-05-05 17:33:51.818449 terminaltexteffects-0.9.0/terminaltexteffects/utils/ansitools.py
+-rwxr-xr-x   0        0        0    12883 2024-05-05 17:33:51.829129 terminaltexteffects-0.9.0/terminaltexteffects/utils/argsdataclass.py
+-rwxr-xr-x   0        0        0    15541 2024-05-05 17:33:51.830302 terminaltexteffects-0.9.0/terminaltexteffects/utils/argvalidators.py
+-rwxr-xr-x   0        0        0     2399 2024-05-05 17:33:51.832912 terminaltexteffects-0.9.0/terminaltexteffects/utils/colorterm.py
+-rwxr-xr-x   0        0        0    13639 2024-05-05 17:33:51.833389 terminaltexteffects-0.9.0/terminaltexteffects/utils/easing.py
+-rwxr-xr-x   0        0        0        0 2024-04-26 11:00:38.378584 terminaltexteffects-0.9.0/terminaltexteffects/utils/exceptions.py
+-rwxr-xr-x   0        0        0     9843 2024-05-05 17:33:51.833880 terminaltexteffects-0.9.0/terminaltexteffects/utils/geometry.py
+-rwxr-xr-x   0        0        0    10033 2024-05-05 17:33:51.834296 terminaltexteffects-0.9.0/terminaltexteffects/utils/graphics.py
+-rwxr-xr-x   0        0        0     7140 2024-05-05 17:33:51.847877 terminaltexteffects-0.9.0/terminaltexteffects/utils/hexterm.py
+-rw-r--r--   0        0        0    12332 1970-01-01 00:00:00.000000 terminaltexteffects-0.9.0/PKG-INFO
```

### Comparing `terminaltexteffects-0.8.0/LICENSE` & `terminaltexteffects-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/__main__.py` & `terminaltexteffects-0.9.0/terminaltexteffects/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse
 import importlib
 import pkgutil
 
 import terminaltexteffects.effects
-import terminaltexteffects.utils.terminal as term
+import terminaltexteffects.engine.terminal as term
+from terminaltexteffects.engine.terminal import TerminalConfig
 from terminaltexteffects.utils.argsdataclass import ArgsDataClass
-from terminaltexteffects.utils.terminal import TerminalConfig
 
 
 def main():
     parser = (argparse.ArgumentParser)(
         prog="terminaltexteffects",
         description="Apply visual effects to terminal text piped in from stdin.",
         epilog="Ex: ls -a | python -m terminaltexteffects --xterm-colors decrypt -a 0.002 --ciphertext-color 00ff00 --plaintext-color ff0000 --final-color 0000ff",
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/base_character.py` & `terminaltexteffects-0.9.0/terminaltexteffects/engine/base_character.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 """This module contains the EffectCharacter class and EventHandler class used to manage the state of a single character from the input data."""
 
 import typing
 from dataclasses import dataclass
 from enum import Enum, auto
 
-from terminaltexteffects.utils import animation, motion
+from terminaltexteffects.engine import animation, motion
 from terminaltexteffects.utils.geometry import Coord
 
 
 class EventHandler:
     """Register and handle events related to a character.
 
     Events related to character state changes (e.g. waypoint reached) can be registered with the EventHandler.
-    When an event is triggered, the EventHandler will take the specified action (e.g. activate a waypoint).
+    When an event is triggered, the EventHandler will take the specified action (e.g. activate a Path).
     The EventHandler is used by the EffectCharacter class to handle events related to the character.
 
     Attributes:
         character (EffectCharacter): The character that the EventHandler is handling events for.
         registered_events (dict[tuple[Event, str], list[tuple[Action, str]]]): A dictionary of registered events.
             The key is a tuple of the event and the subject_id (waypoint id/scene id).
             The value is a list of tuples of the action and the action target (waypoint id/scene id).
         layer (int): The layer of the character. The layer determines the order in which characters are printed.
+
+    Note:
+        SEGMENT_ENTERED/EXITED events will trigger the first time the character enters or exits a segment.
+        If looping, each loop will trigger the event, but not backwards motion as is possible with the bounce easing functions.
     """
 
     def __init__(self, character: "EffectCharacter"):
         """Initializes the instance with the EffectCharacter object.
 
         Args:
-            character (EffectCharacter): The character that the EventHandler is handling events for.
+            character (EffectCharacter): The character for which the EventHandler is handling events.
         """
         self.character = character
         self.layer: int = 0
         self.registered_events: dict[
             tuple[EventHandler.Event, animation.Scene | motion.Waypoint | motion.Path],
             list[
                 tuple[
@@ -40,16 +44,15 @@
                 ]
             ],
         ] = {}
 
     class Event(Enum):
         """An Event that can be registered with the EventHandler.
 
-        An Event is triggered when a character reaches a waypoint or an animation scene is activated. Register
-        Events with the EventHandler using the register_event method of the EventHandler class.
+        Register Events with the EventHandler using the register_event method of the EventHandler class.
 
         Attributes:
             SEGMENT_ENTERED (Event): A path segment has been entered.
             SEGMENT_EXITED (Event): A path segment has been exited.
             PATH_ACTIVATED (Event): A path has been activated.
             PATH_COMPLETE (Event): A path has been completed.
             PATH_HOLDING (Event): A path has entered the holding state.
@@ -91,23 +94,26 @@
 
     @dataclass(init=False)
     class Callback:
         """A callback action target that can be taken when an event is triggered.
 
         Register callback actions with the EventHandler using the register_event method of the EventHandler class.
 
-        Attributes:
-            callback (typing.Callable): The callback function to call.
-            args (tuple[typing.Any,...]): A tuple of arguments to pass to the callback function. The first argument will be the character, followed by any additional arguments.
         """
 
         callback: typing.Callable
         args: tuple[typing.Any, ...]
 
         def __init__(self, callback: typing.Callable, *args: typing.Any):
+            """Initializes the instance with the callback function and arguments.
+
+            Args:
+                callback (typing.Callable): The callback function to call.
+                args (tuple[typing.Any,...]): A tuple of arguments to pass to the callback function. The first argument will be the character, followed by any additional arguments.
+            """
             self.callback = callback
             self.args = args
 
     def register_event(
         self,
         event: Event,
         caller: animation.Scene | motion.Waypoint | motion.Path,
@@ -117,22 +123,26 @@
         """Registers an event to be handled by the EventHandler.
 
         Args:
             event (Event): The event to register.
             caller (animation.Scene | motion.Waypoint | motion.Path): The object that triggers the event.
             action (Action): The action to take when the event is triggered.
             target (animation.Scene | motion.Waypoint | motion.Path | int | Coord | Callback): The target of the action.
+
+        Example:
+            Register an event to activate a scene when a Path is complete:
+            `event_handler.register_event(EventHandler.Event.PATH_COMPLETE, some_path, EventHandler.Action.ACTIVATE_SCENE, some_scene)`
         """
         new_event = (event, caller)
         new_action = (action, target)
         if new_event not in self.registered_events:
             self.registered_events[new_event] = list()
         self.registered_events[new_event].append(new_action)
 
-    def handle_event(self, event: Event, caller: animation.Scene | motion.Waypoint | motion.Path) -> None:
+    def _handle_event(self, event: Event, caller: animation.Scene | motion.Waypoint | motion.Path) -> None:
         """Handles an event by taking the specified action.
 
         Args:
             event (Event): An event to handle. If the event is not registered, nothing happens.
             caller (animation.Scene | motion.Waypoint | motion.Path): The object triggering the call.
         """
         action_map = {
@@ -150,28 +160,36 @@
         for event_action in self.registered_events[(event, caller)]:
             action, target = event_action
             action_map[action](target)  # type: ignore
 
 
 class EffectCharacter:
     """
-    A class representing a single character from the input data.
+    A class representing a single character from the input data. EffectCharacters are managed by the Terminal and are used
+    to apply animations and effects to individual characters.
+
+    Add an EffectCharacter to the Terminal using the add_character method of the Terminal class.
+
+    Methods:
+        tick: Progress the character's animation and motion by one step.
 
     Attributes:
         input_symbol (str): The symbol for the character in the input data.
         input_coord (Coord): The coordinate of the character in the input data.
         symbol (str): The current symbol for the character, determined by the animation units.
+        character_id (int): The unique ID of the character, generated by the Terminal.
         animation (graphics.Animation): The animation object that controls the character's appearance.
         motion (motion.Motion): The motion object that controls the character's movement.
         event_handler (EventHandler): The event handler object that handles events related to the character.
         is_visible (bool): Whether the character is currently visible and should be printed to the terminal.
+        layer (int): The layer of the character. The layer determines the order in which characters are printed.
     """
 
     def __init__(self, character_id: int, symbol: str, input_column: int, input_row: int):
-        """Initializes the instance with the input values and the Terminal object.
+        """Initializes the character instance with the character ID, symbol, and input coordinates.
 
         Args:
             character_id (int): The unique ID of the character, generated by the Terminal.
             symbol (str): The symbol for the character in the input data.
             input_column (int): The column of the character in the input data.
             input_row (int): The row of the character in the input data.
         """
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_beams.py` & `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_synthgrid.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,324 +1,442 @@
+"""Create a grid which fills with characters dissolving into the final text.
+
+Classes:
+    SynthGrid: Create a grid which fills with characters dissolving into the final text.
+    SynthGridConfig: Configuration for the SynthGrid effect.
+    SynthGridIterator: Iterates over the effect. Does not normally need to be called directly.
+"""
+
 import random
 import typing
 from dataclasses import dataclass
 
-import terminaltexteffects.utils.arg_validators as arg_validators
-from terminaltexteffects.base_character import EffectCharacter
-from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
-from terminaltexteffects.utils import graphics
+from terminaltexteffects.engine.base_character import EffectCharacter, EventHandler
+from terminaltexteffects.engine.base_effect import BaseEffect, BaseEffectIterator
+from terminaltexteffects.engine.terminal import Terminal
+from terminaltexteffects.utils import argvalidators, geometry, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
-from terminaltexteffects.utils.terminal import Terminal
+from terminaltexteffects.utils.geometry import Coord
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
-    return Beams, BeamsConfig
+    return SynthGrid, SynthGridConfig
 
 
 @argclass(
-    name="beams",
-    help="Create beams which travel over the output area illuminating the characters behind them.",
-    description="beams | Create beams which travel over the output area illuminating the characters behind them.",
-    epilog="""Example: terminaltexteffects beams --beam-row-symbols ▂ ▁ _ --beam-column-symbols ▌ ▍ ▎ ▏ --beam-delay 10 --beam-row-speed-range 10-40 --beam-column-speed-range 6-10 --beam-gradient-stops ffffff 00D1FF 8A008A --beam-gradient-steps 2 8 --beam-gradient-frames 2 --final-gradient-stops 8A008A 00D1FF ffffff --final-gradient-steps 12 --final-gradient-frames 5 --final-gradient-direction vertical --final-wipe-speed 1""",
+    name="synthgrid",
+    help="Create a grid which fills with characters dissolving into the final text.",
+    description="synthgrid | Create a grid which fills with characters dissolving into the final text.",
+    epilog="""Example: terminaltexteffects synthgrid --grid-gradient-stops CC00CC ffffff --grid-gradient-steps 12 --text-gradient-stops 8A008A 00D1FF FFFFFF --text-gradient-steps 12 --grid-row-symbol ─ --grid-column-symbol "│" --text-generation-symbols ░ ▒ ▓ --max-active-blocks 0.1""",
 )
 @dataclass
-class BeamsConfig(ArgsDataClass):
-    """Configuration for the Beams effect.
+class SynthGridConfig(ArgsDataClass):
+    """Configuration for the SynthGrid effect.
 
     Attributes:
-        beam_row_symbols (tuple[str, ...]): Symbols to use for the beam effect when moving along a row. Strings will be used in sequence to create an animation.
-        beam_column_symbols (tuple[str, ...]): Symbols to use for the beam effect when moving along a column. Strings will be used in sequence to create an animation.
-        beam_delay (int): Number of frames to wait before adding the next group of beams. Beams are added in groups of size random(1, 5).
-        beam_row_speed_range (tuple[int, int]): Speed range of the beam when moving along a row.
-        beam_column_speed_range (tuple[int, int]): Speed range of the beam when moving along a column.
-        beam_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the beam, a gradient will be created between the colors.
-        beam_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation. Steps are paired with the colors in final-gradient-stops.
-        beam_gradient_frames (int): Number of frames to display each gradient step.
-        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the wipe gradient.
-        final_gradient_steps (tuple[int,]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation. Steps are paired with the colors in final-gradient-stops.
-        final_gradient_frames (int): Number of frames to display each gradient step.
-        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
-        final_wipe_speed (int): Speed of the final wipe as measured in diagonal groups activated per frame.
-    """
-
-    beam_row_symbols: tuple[str, ...] = ArgField(
-        cmd_name="--beam-row-symbols",
-        type_parser=arg_validators.Symbol.type_parser,
-        nargs="+",
-        default=("▂", "▁", "_"),
-        metavar=arg_validators.Symbol.METAVAR,
-        help="Symbols to use for the beam effect when moving along a row. Strings will be used in sequence to create an animation.",
-    )  # type: ignore[assignment]
-
-    "tuple[str, ...] : Symbols to use for the beam effect when moving along a row. Strings will be used in sequence to create an animation."
-
-    beam_column_symbols: tuple[str, ...] = ArgField(
-        cmd_name="--beam-column-symbols",
-        type_parser=arg_validators.Symbol.type_parser,
-        nargs="+",
-        default=("▌", "▍", "▎", "▏"),
-        metavar=arg_validators.Symbol.METAVAR,
-        help="Symbols to use for the beam effect when moving along a column. Strings will be used in sequence to create an animation.",
-    )  # type: ignore[assignment]
-
-    "tuple[str, ...] : Symbols to use for the beam effect when moving along a column. Strings will be used in sequence to create an animation."
-
-    beam_delay: int = ArgField(
-        cmd_name="--beam-delay",
-        type_parser=arg_validators.PositiveInt.type_parser,
-        default=10,
-        metavar=arg_validators.PositiveInt.METAVAR,
-        help="Number of frames to wait before adding the next group of beams. Beams are added in groups of size random(1, 5).",
-    )  # type: ignore[assignment]
-
-    "int : Number of frames to wait before adding the next group of beams. Beams are added in groups of size random(1, 5)."
-
-    beam_row_speed_range: tuple[int, int] = ArgField(
-        cmd_name="--beam-row-speed-range",
-        type_parser=arg_validators.IntRange.type_parser,
-        default=(10, 40),
-        metavar=arg_validators.IntRange.METAVAR,
-        help="Speed range of the beam when moving along a row.",
-    )  # type: ignore[assignment]
-
-    "tuple[int, int] : Speed range of the beam when moving along a row."
-
-    beam_column_speed_range: tuple[int, int] = ArgField(
-        cmd_name="--beam-column-speed-range",
-        type_parser=arg_validators.IntRange.type_parser,
-        default=(6, 10),
-        metavar=arg_validators.IntRange.METAVAR,
-        help="Speed range of the beam when moving along a column.",
-    )  # type: ignore[assignment]
-
-    "tuple[int, int] : Speed range of the beam when moving along a column."
-
-    beam_gradient_stops: tuple[graphics.Color, ...] = ArgField(
-        cmd_name="--beam-gradient-stops",
-        type_parser=arg_validators.Color.type_parser,
+        grid_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the grid gradient.
+        grid_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation. Valid values are n > 0.
+        grid_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the grid color.
+        text_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the text gradient.
+        text_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation. Valid values are n > 0.
+        text_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the text color.
+        grid_row_symbol (str): Symbol to use for grid row lines.
+        grid_column_symbol (str): Symbol to use for grid column lines.
+        text_generation_symbols (tuple[str, ...]): Tuple of characters for the text generation animation.
+        max_active_blocks (float): Maximum percentage of blocks to have active at any given time. For example, if set to 0.1, 10 percent of the blocks will be active at any given time. Valid values are 0 < n <= 1."""
+
+    grid_gradient_stops: tuple[graphics.Color, ...] = ArgField(
+        cmd_name=["--grid-gradient-stops"],
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
-        default=("ffffff", "00D1FF", "8A008A"),
-        metavar="(XTerm [0-255] OR RGB Hex [000000-ffffff])",
-        help="Space separated, unquoted, list of colors for the beam, a gradient will be created between the colors.",
-    )  # type: ignore[assignment]
-
-    "tuple[graphics.Color, ...] : Tuple of colors for the beam, a gradient will be created between the colors."
-
-    beam_gradient_steps: tuple[int, ...] = ArgField(
-        cmd_name="--beam-gradient-steps",
-        type_parser=arg_validators.PositiveInt.type_parser,
+        default=("CC00CC", "ffffff"),
+        metavar=argvalidators.ColorArg.METAVAR,
+        help="Space separated, unquoted, list of colors for the grid gradient.",
+    )  # type: ignore[assignment]
+    "tuple[graphics.Color, ...] : Tuple of colors for the grid gradient."
+
+    grid_gradient_steps: tuple[int, ...] = ArgField(
+        cmd_name="--grid-gradient-steps",
+        type_parser=argvalidators.PositiveInt.type_parser,
         nargs="+",
-        default=(2, 8),
-        metavar=arg_validators.PositiveInt.METAVAR,
-        help="Space separated, unquoted, numbers for the of gradient steps to use. More steps will create a smoother and longer gradient animation. Steps are paired with the colors in final-gradient-stops.",
-    )  # type: ignore[assignment]
-
-    "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation. Steps are paired with the colors in final-gradient-stops."
-
-    beam_gradient_frames: int = ArgField(
-        cmd_name="--beam-gradient-frames",
-        type_parser=arg_validators.PositiveInt.type_parser,
-        default=2,
-        metavar=arg_validators.PositiveInt.METAVAR,
-        help="Number of frames to display each gradient step.",
+        default=(12,),
+        metavar=argvalidators.PositiveInt.METAVAR,
+        help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
+    "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
 
-    "int : Number of frames to display each gradient step."
-
-    final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
-        cmd_name="--final-gradient-stops",
-        type_parser=arg_validators.Color.type_parser,
+    grid_gradient_direction: graphics.Gradient.Direction = ArgField(
+        cmd_name="--grid-gradient-direction",
+        type_parser=argvalidators.GradientDirection.type_parser,
+        default=graphics.Gradient.Direction.DIAGONAL,
+        metavar=argvalidators.GradientDirection.METAVAR,
+        help="Direction of the gradient for the grid color.",
+    )  # type: ignore[assignment]
+    "graphics.Gradient.Direction : Direction of the gradient for the grid color."
+
+    text_gradient_stops: tuple[graphics.Color, ...] = ArgField(
+        cmd_name=["--text-gradient-stops"],
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
-        default=("8A008A", "00D1FF", "ffffff"),
-        metavar=arg_validators.Color.METAVAR,
-        help="Space separated, unquoted, list of colors for the wipe gradient.",
-    )  # type: ignore[assignment]
-
-    "tuple[graphics.Color, ...] : Tuple of colors for the wipe gradient."
-
-    final_gradient_steps: tuple[int,] = ArgField(
-        cmd_name="--final-gradient-steps",
-        type_parser=arg_validators.PositiveInt.type_parser,
+        default=("8A008A", "00D1FF", "FFFFFF"),
+        metavar=argvalidators.ColorArg.METAVAR,
+        help="Space separated, unquoted, list of colors for the text gradient.",
+    )  # type: ignore[assignment]
+    "tuple[graphics.Color, ...] : Tuple of colors for the text gradient."
+
+    text_gradient_steps: tuple[int, ...] = ArgField(
+        cmd_name="--text-gradient-steps",
+        type_parser=argvalidators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
-        metavar=arg_validators.PositiveInt.METAVAR,
-        help="Space separated, unquoted, numbers for the of gradient steps to use. More steps will create a smoother and longer gradient animation. Steps are paired with the colors in final-gradient-stops.",
+        metavar=argvalidators.PositiveInt.METAVAR,
+        help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
+    "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
 
-    "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation. Steps are paired with the colors in final-gradient-stops."
-
-    final_gradient_frames: int = ArgField(
-        cmd_name="--final-gradient-frames",
-        type_parser=arg_validators.PositiveInt.type_parser,
-        default=5,
-        metavar=arg_validators.PositiveInt.METAVAR,
-        help="Number of frames to display each gradient step.",
-    )  # type: ignore[assignment]
-
-    "int : Number of frames to display each gradient step."
-
-    final_gradient_direction: graphics.Gradient.Direction = ArgField(
-        cmd_name="--final-gradient-direction",
-        type_parser=arg_validators.GradientDirection.type_parser,
+    text_gradient_direction: graphics.Gradient.Direction = ArgField(
+        cmd_name="--text-gradient-direction",
+        type_parser=argvalidators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.VERTICAL,
-        metavar=arg_validators.GradientDirection.METAVAR,
-        help="Direction of the gradient for the final color.",
+        metavar=argvalidators.GradientDirection.METAVAR,
+        help="Direction of the gradient for the text color.",
     )  # type: ignore[assignment]
+    "graphics.Gradient.Direction : Direction of the gradient for the text color."
 
-    "graphics.Gradient.Direction : Direction of the gradient for the final color."
-
-    final_wipe_speed: int = ArgField(
-        cmd_name="--final-wipe-speed",
-        type_parser=arg_validators.PositiveInt.type_parser,
-        default=1,
-        metavar=arg_validators.PositiveInt.METAVAR,
-        help="Speed of the final wipe as measured in diagonal groups activated per frame.",
+    grid_row_symbol: str = ArgField(
+        cmd_name="--grid-row-symbol",
+        type_parser=argvalidators.Symbol.type_parser,
+        default="─",
+        metavar=argvalidators.Symbol.METAVAR,
+        help="Symbol to use for grid row lines.",
+    )  # type: ignore[assignment]
+    "str : Symbol to use for grid row lines."
+
+    grid_column_symbol: str = ArgField(
+        cmd_name="--grid-column-symbol",
+        type_parser=argvalidators.Symbol.type_parser,
+        default="│",
+        metavar=argvalidators.Symbol.METAVAR,
+        help="Symbol to use for grid column lines.",
+    )  # type: ignore[assignment]
+    "str : Symbol to use for grid column lines."
+
+    text_generation_symbols: tuple[str, ...] = ArgField(
+        cmd_name="--text-generation-symbols",
+        type_parser=argvalidators.Symbol.type_parser,
+        nargs="+",
+        default=("░", "▒", "▓"),
+        metavar=argvalidators.Symbol.METAVAR,
+        help="Space separated, unquoted, list of characters for the text generation animation.",
+    )  # type: ignore[assignment]
+    "tuple[str, ...] : Tuple of characters for the text generation animation."
+
+    max_active_blocks: float = ArgField(
+        cmd_name="--max-active-blocks",
+        type_parser=argvalidators.PositiveFloat.type_parser,
+        default=0.1,
+        metavar=argvalidators.PositiveFloat.METAVAR,
+        help="Maximum percentage of blocks to have active at any given time. For example, if set to 0.1, 10 percent of the blocks will be active at any given time.",
     )  # type: ignore[assignment]
-
-    "int : Speed of the final wipe as measured in diagonal groups activated per frame."
+    "float : Maximum percentage of blocks to have active at any given time."
 
     @classmethod
     def get_effect_class(cls):
-        return Beams
+        return SynthGrid
+
 
+class _GridLine:
+    def __init__(
+        self,
+        terminal: Terminal,
+        args: SynthGridConfig,
+        origin: Coord,
+        direction: str,
+        grid_gradient_mapping: dict[geometry.Coord, graphics.Color],
+    ):
+        self.terminal = terminal
+        self.args = args
+        self.origin = origin
+        self.direction = direction
+        if self.direction == "horizontal":
+            self.grid_symbol = self.args.grid_row_symbol
+        elif self.direction == "vertical":
+            self.grid_symbol = self.args.grid_column_symbol
+        self.characters: list[EffectCharacter] = []
+        if direction == "horizontal":
+            for column_index in range(self.terminal.output_area.left, self.terminal.output_area.right + 1):
+                effect_char = self.terminal.add_character(self.grid_symbol, Coord(0, 0))
+                grid_scn = effect_char.animation.new_scene()
+                grid_scn.add_frame(
+                    self.grid_symbol, 1, color=grid_gradient_mapping[geometry.Coord(column_index, origin.row)]
+                )
+                effect_char.animation.activate_scene(grid_scn)
+                effect_char.layer = 2
+                effect_char.motion.set_coordinate(Coord(column_index, origin.row))
+                self.characters.append(effect_char)
+        elif direction == "vertical":
+            for row_index in range(self.terminal.output_area.bottom, self.terminal.output_area.top):
+                effect_char = self.terminal.add_character(self.grid_symbol, Coord(0, 0))
+                grid_scn = effect_char.animation.new_scene()
+                grid_scn.add_frame(
+                    self.grid_symbol, 1, color=grid_gradient_mapping[geometry.Coord(origin.column, row_index)]
+                )
+                effect_char.animation.activate_scene(grid_scn)
+                effect_char.layer = 2
+                effect_char.motion.set_coordinate(Coord(origin.column, row_index))
+                self.characters.append(effect_char)
+        self.collapsed_characters = [effect_char for effect_char in self.characters]
+        self.extended_characters: list[EffectCharacter] = []
+
+    def extend(self) -> None:
+        if self.direction == "horizontal":
+            count = 3
+        else:
+            count = 1
+        for _ in range(count):
+            if self.collapsed_characters:
+                next_char = self.collapsed_characters.pop(0)
+                self.terminal.set_character_visibility(next_char, True)
+                self.extended_characters.append(next_char)
+
+    def collapse(self) -> None:
+        if self.direction == "horizontal":
+            count = 3
+        else:
+            count = 1
+        if not self.collapsed_characters:
+            self.extended_characters = self.extended_characters[::-1]
+        for _ in range(count):
+            if self.extended_characters:
+                next_char = self.extended_characters.pop(0)
+                self.terminal.set_character_visibility(next_char, False)
+                self.collapsed_characters.append(next_char)
+
+    def is_extended(self) -> bool:
+        return not self.collapsed_characters
 
-class BeamsIterator(BaseEffectIterator[BeamsConfig]):
-    class _Group:
-        def __init__(self, characters: list[EffectCharacter], direction: str, terminal: Terminal, args: BeamsConfig):
-            self.characters = characters
-            self.direction: str = direction
-            self.terminal = terminal
-            direction_speed_range = {
-                "row": (args.beam_row_speed_range[0], args.beam_row_speed_range[1]),
-                "column": (args.beam_column_speed_range[0], args.beam_column_speed_range[1]),
-            }
-            self.speed = random.randint(direction_speed_range[direction][0], direction_speed_range[direction][1]) * 0.1
-            self.next_character_counter: float = 0
-            if self.direction == "row":
-                self.characters.sort(key=lambda character: character.input_coord.column)
-            elif self.direction == "column":
-                self.characters.sort(key=lambda character: character.input_coord.row)
-            if random.choice([True, False]):
-                self.characters.reverse()
-
-        def increment_next_character_counter(self) -> None:
-            self.next_character_counter += self.speed
-
-        def get_next_character(self) -> EffectCharacter | None:
-            self.next_character_counter -= 1
-            next_character = self.characters.pop(0)
-            if next_character.animation.active_scene:
-                next_character.animation.active_scene.reset_scene()
-                return_value = None
-            else:
-                self.terminal.set_character_visibility(next_character, True)
-                return_value = next_character
-            next_character.animation.activate_scene(next_character.animation.query_scene("beam_" + self.direction))
-            return return_value
+    def is_collapsed(self) -> bool:
+        return not self.extended_characters
 
-        def complete(self) -> bool:
-            return not self.characters
 
-    def __init__(self, effect: "Beams") -> None:
+class SynthGridIterator(BaseEffectIterator[SynthGridConfig]):
+    def __init__(self, effect: "SynthGrid") -> None:
         super().__init__(effect)
-        self._pending_groups: list[BeamsIterator._Group] = []
+        self._pending_groups: list[tuple[int, list[EffectCharacter]]] = []
         self._active_chars: list[EffectCharacter] = []
-        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-        self.active_groups: list[BeamsIterator._Group] = []
-        self.delay = 0
-        self.phase = "beams"
-        self.final_wipe_groups = self._terminal.get_characters_grouped(
-            Terminal.CharacterGroup.DIAGONAL_TOP_LEFT_TO_BOTTOM_RIGHT
-        )
+        self._grid_lines: list[_GridLine] = []
+        self._group_tracker: dict[int, int] = {}
         self._build()
 
+    def _find_even_gap(self, dimension: int) -> int:
+        """Find the closest even gap to 20% of the longest dimension.
+
+        Args:
+            dimension (int): The longest dimension.
+
+        Returns:
+            int: The gap that is closest to 20% of the dimension length.
+        """
+        potential_gaps: list[int] = []
+        dimension = dimension - 2
+        if dimension <= 0:
+            return 0
+        for i in range(dimension, 4, -1):
+            if dimension % i <= 1:
+                potential_gaps.append(i)
+        if not potential_gaps:
+            return 4
+        return min(potential_gaps, key=lambda x: abs(x - dimension // 5))
+
     def _build(self) -> None:
-        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
-        final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
+        grid_gradient = graphics.Gradient(*self._config.grid_gradient_stops, steps=self._config.grid_gradient_steps)
+        grid_gradient_mapping = grid_gradient.build_coordinate_color_mapping(
+            self._terminal.output_area.top, self._terminal.output_area.right, self._config.grid_gradient_direction
         )
-        for character in self._terminal.get_characters(fill_chars=True):
-            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        text_gradient = graphics.Gradient(*self._config.text_gradient_stops, steps=self._config.text_gradient_steps)
+        text_gradient_mapping = text_gradient.build_coordinate_color_mapping(
+            self._terminal.output_area.top, self._terminal.output_area.right, self._config.text_gradient_direction
+        )
+
+        self._grid_lines.append(
+            _GridLine(
+                self._terminal,
+                self._config,
+                Coord(self._terminal.output_area.left, self._terminal.output_area.bottom),
+                "horizontal",
+                grid_gradient_mapping,
+            )
+        )
+        self._grid_lines.append(
+            _GridLine(
+                self._terminal,
+                self._config,
+                Coord(self._terminal.output_area.left, self._terminal.output_area.top),
+                "horizontal",
+                grid_gradient_mapping,
+            )
+        )
+        self._grid_lines.append(
+            _GridLine(
+                self._terminal,
+                self._config,
+                Coord(self._terminal.output_area.left, self._terminal.output_area.bottom),
+                "vertical",
+                grid_gradient_mapping,
+            )
+        )
+        self._grid_lines.append(
+            _GridLine(
+                self._terminal,
+                self._config,
+                Coord(self._terminal.output_area.right, self._terminal.output_area.bottom),
+                "vertical",
+                grid_gradient_mapping,
+            )
+        )
+        column_indexes: list[int] = []
+        row_indexes: list[int] = []
+        if self._terminal.output_area.top > 2 * self._terminal.output_area.right:
+            row_gap = self._find_even_gap(self._terminal.output_area.top) + 1
+            column_gap = row_gap * 2
+        else:
+            column_gap = self._find_even_gap(self._terminal.output_area.right) + 1
+            row_gap = column_gap // 2
 
-        beam_gradient = graphics.Gradient(*self._config.beam_gradient_stops, steps=self._config.beam_gradient_steps)
-        groups: list[BeamsIterator._Group] = []
-        for row in self._terminal.get_characters_grouped(Terminal.CharacterGroup.ROW_TOP_TO_BOTTOM, fill_chars=True):
-            groups.append(BeamsIterator._Group(row, "row", self._terminal, self._config))
-        for column in self._terminal.get_characters_grouped(
-            Terminal.CharacterGroup.COLUMN_LEFT_TO_RIGHT, fill_chars=True
+        for row_index in range(
+            self._terminal.output_area.bottom + row_gap, self._terminal.output_area.top, max(row_gap, 1)
         ):
-            groups.append(BeamsIterator._Group(column, "column", self._terminal, self._config))
-        for group in groups:
-            for character in group.characters:
-                beam_row_scn = character.animation.new_scene(id="beam_row")
-                beam_column_scn = character.animation.new_scene(id="beam_column")
-                beam_row_scn.apply_gradient_to_symbols(
-                    beam_gradient, self._config.beam_row_symbols, self._config.beam_gradient_frames
-                )
-                beam_column_scn.apply_gradient_to_symbols(
-                    beam_gradient, self._config.beam_column_symbols, self._config.beam_gradient_frames
+            if self._terminal.output_area.top - row_index < 2:
+                continue
+            row_indexes.append(row_index)
+            self._grid_lines.append(
+                _GridLine(
+                    self._terminal,
+                    self._config,
+                    Coord(self._terminal.output_area.left, row_index),
+                    "horizontal",
+                    grid_gradient_mapping,
                 )
-                faded_color = character.animation.adjust_color_brightness(
-                    self._character_final_color_map[character], 0.3
+            )
+        for column_index in range(
+            self._terminal.output_area.left + column_gap, self._terminal.output_area.right, max(column_gap, 1)
+        ):
+            if self._terminal.output_area.right - column_index < 2:
+                continue
+            column_indexes.append(column_index)
+            self._grid_lines.append(
+                _GridLine(
+                    self._terminal,
+                    self._config,
+                    Coord(column_index, self._terminal.output_area.bottom),
+                    "vertical",
+                    grid_gradient_mapping,
                 )
-                fade_gradient = graphics.Gradient(self._character_final_color_map[character], faded_color, steps=10)
-                beam_row_scn.apply_gradient_to_symbols(fade_gradient, character.input_symbol, 5)
-                beam_column_scn.apply_gradient_to_symbols(fade_gradient, character.input_symbol, 5)
-                brighten_gradient = graphics.Gradient(faded_color, self._character_final_color_map[character], steps=10)
-                brigthen_scn = character.animation.new_scene(id="brighten")
-                brigthen_scn.apply_gradient_to_symbols(
-                    brighten_gradient, character.input_symbol, self._config.final_gradient_frames
+            )
+        row_indexes.append(self._terminal.output_area.top + 1)
+        column_indexes.append(self._terminal.output_area.right + 1)
+        prev_row_index = 1
+        for row_index in row_indexes:
+            prev_column_index = 1
+            for column_index in column_indexes:
+                coords_in_block: list[Coord] = []
+                if row_index == self._terminal.output_area.top:  # make sure the top row is included
+                    row_index += 1
+                for row in range(prev_row_index, row_index):
+                    for column in range(prev_column_index, column_index):
+                        coords_in_block.append(Coord(column, row))
+                characters_in_block: list[EffectCharacter] = []
+                for coord in coords_in_block:
+                    if coord in self._terminal.character_by_input_coord:
+                        characters_in_block.append(self._terminal.character_by_input_coord[coord])
+                if characters_in_block:
+                    self._pending_groups.append((len(self._pending_groups), characters_in_block))
+                prev_column_index = column_index
+            prev_row_index = row_index
+        for group_number, group in self._pending_groups:
+            self._group_tracker[group_number] = 0
+            for character in group:
+                dissolve_scn = character.animation.new_scene()
+                for _ in range(random.randint(15, 30)):
+                    dissolve_scn.add_frame(
+                        random.choice(self._config.text_generation_symbols),
+                        3,
+                        color=random.choice(text_gradient.spectrum),
+                    )
+                dissolve_scn.add_frame(character.input_symbol, 1, color=text_gradient_mapping[character.input_coord])
+                character.animation.activate_scene(dissolve_scn)
+                character.event_handler.register_event(
+                    EventHandler.Event.SCENE_COMPLETE,
+                    dissolve_scn,
+                    EventHandler.Action.CALLBACK,
+                    EventHandler.Callback(self._update_group_tracker, group_number),
                 )
-        self._pending_groups = groups
         random.shuffle(self._pending_groups)
+        self._phase = "grid_expand"
+        self._total_group_count = len(self._pending_groups)
+        if not self._total_group_count:
+            for character in self._terminal.get_characters():
+                self._terminal.set_character_visibility(character, True)
+                self._active_chars.append(character)
+        self._active_groups: int = 0
+
+    def _update_group_tracker(self, character: EffectCharacter, *args) -> None:
+        self._group_tracker[args[0]] -= 1
 
     def __next__(self) -> str:
-        if self.phase != "complete" or self._active_chars:
-            if self.phase == "beams":
-                if not self.delay:
-                    if self._pending_groups:
-                        for _ in range(random.randint(1, 5)):
-                            if self._pending_groups:
-                                self.active_groups.append(self._pending_groups.pop(0))
-                    self.delay = self._config.beam_delay
+        if self._pending_groups or self._active_chars or self._phase != "complete":
+            if self._phase == "grid_expand":
+                if not all([grid_line.is_extended() for grid_line in self._grid_lines]):
+                    for grid_line in self._grid_lines:
+                        if not grid_line.is_extended():
+                            grid_line.extend()
                 else:
-                    self.delay -= 1
-                for group in self.active_groups:
-                    group.increment_next_character_counter()
-                    if int(group.next_character_counter) > 1:
-                        for _ in range(int(group.next_character_counter)):
-                            if not group.complete():
-                                next_char = group.get_next_character()
-                                if next_char:
-                                    self._active_chars.append(next_char)
-                self.active_groups = [group for group in self.active_groups if not group.complete()]
-                if not self._pending_groups and not self.active_groups and not self._active_chars:
-                    self.phase = "final_wipe"
-            elif self.phase == "final_wipe":
-                if self.final_wipe_groups:
-                    for _ in range(self._config.final_wipe_speed):
-                        if not self.final_wipe_groups:
-                            break
-                        next_group = self.final_wipe_groups.pop(0)
-                        for character in next_group:
-                            character.animation.activate_scene(character.animation.query_scene("brighten"))
-                            self._terminal.set_character_visibility(character, True)
-                            self._active_chars.append(character)
+                    self._phase = "add_chars"
+            elif self._phase == "add_chars":
+                if (
+                    self._pending_groups
+                    and self._active_groups < self._total_group_count * self._config.max_active_blocks
+                ):
+                    group_number, next_group = self._pending_groups.pop(0)
+                    for char in next_group:
+                        self._terminal.set_character_visibility(char, True)
+                        self._active_chars.append(char)
+                        self._group_tracker[group_number] += 1
+                if not self._pending_groups and not self._active_chars and not self._active_groups:
+                    self._phase = "collapse"
+            elif self._phase == "collapse":
+                if not all([grid_line.is_collapsed() for grid_line in self._grid_lines]):
+                    for grid_line in self._grid_lines:
+                        if not grid_line.is_collapsed():
+                            grid_line.collapse()
                 else:
-                    self.phase = "complete"
-            next_frame = self._terminal.get_formatted_output_string()
+                    self._phase = "complete"
             for character in self._active_chars:
                 character.tick()
+
             self._active_chars = [character for character in self._active_chars if character.is_active]
-            return next_frame
+            self._active_groups = 0
+            for _, active_count in self._group_tracker.items():
+                if active_count:
+                    self._active_groups += 1
+            return self._terminal.get_formatted_output_string()
         else:
             raise StopIteration
 
 
-class Beams(BaseEffect[BeamsConfig]):
-    """Effect that creates beams which travel over the output area illuminated the characters behind them."""
+class SynthGrid(BaseEffect[SynthGridConfig]):
+    """Create a grid which fills with characters dissolving into the final text.
 
-    _config_cls = BeamsConfig
-    _iterator_cls = BeamsIterator
+    Attributes:
+        effect_config (SynthGridConfig): Configuration for the effect.
+        terminal_config (TerminalConfig): Configuration for the terminal.
+    """
+
+    _config_cls = SynthGridConfig
+    _iterator_cls = SynthGridIterator
 
     def __init__(self, input_data: str) -> None:
+        """Initialize the effect with the provided input data.
+
+        Args:
+            input_data (str): The input data to use for the effect."""
         super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_binarypath.py` & `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_binarypath.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,28 @@
+"""
+Decodes characters into their binary form. Characters travel from outside the output area towards their input coordinate, moving at right angles.
+
+Classes:
+    BinaryPath: Decodes characters into their binary form. Characters travel from outside the output area towards their input coordinate, moving at right angles.
+    BinaryPathConfig: Configuration for the BinaryPath effect.
+    BinaryPathIterator: Effect iterator for the BinaryPath effect. Does not normally need to be called directly.
+
+"""
+
 import random
 import typing
 from dataclasses import dataclass
 
-import terminaltexteffects.utils.arg_validators as arg_validators
-from terminaltexteffects.base_character import EffectCharacter
-from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
+import terminaltexteffects.utils.argvalidators as argvalidators
+from terminaltexteffects.engine.base_character import EffectCharacter
+from terminaltexteffects.engine.base_effect import BaseEffect, BaseEffectIterator
+from terminaltexteffects.engine.terminal import Terminal
 from terminaltexteffects.utils import easing, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 from terminaltexteffects.utils.geometry import Coord
-from terminaltexteffects.utils.terminal import Terminal
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
     return BinaryPath, BinaryPathConfig
 
 
 @argclass(
@@ -22,79 +32,79 @@
     epilog="""Example: terminaltexteffects binarypath --final-gradient-stops 00d500 007500 --final-gradient-steps 12 --final-gradient-direction vertical --binary-colors 044E29 157e38 45bf55 95ed87 --movement-speed 1.0 --active-binary-groups 0.05""",
 )
 @dataclass
 class BinaryPathConfig(ArgsDataClass):
     """Configuration for the BinaryPath effect.
 
     Attributes:
-        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
-        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
-        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation. Valid values are n > 0.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the final gradient.
         binary_colors (tuple[graphics.Color, ...]): Tuple of colors for the binary characters. Character color is randomly assigned from this list.
-        movement_speed (float): Speed of the binary groups as they travel around the terminal.
-        active_binary_groups (float): Maximum number of binary groups that are active at any given time as a percentage of the total number of binary groups. Lower this to improve performance."""
+        movement_speed (float): Speed of the binary groups as they travel around the terminal. Valid values are n > 0.
+        active_binary_groups (float): Maximum number of binary groups that are active at any given time as a percentage of the total number of binary groups. Lower this to improve performance. Valid values are 0 < n <= 1."""
 
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("00d500", "007500"),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
 
-    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+    "tuple[graphics.Color, ...] : Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color."
 
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name=["--final-gradient-steps"],
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
 
-    "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
+    "tuple[int, ...] : Tuple of the number (n > 0) of gradient steps to use. More steps will create a smoother and longer gradient animation."
 
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
-        type_parser=arg_validators.GradientDirection.type_parser,
+        type_parser=argvalidators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.CENTER,
-        metavar=arg_validators.GradientDirection.METAVAR,
-        help="Direction of the gradient for the final color.",
+        metavar=argvalidators.GradientDirection.METAVAR,
+        help="Direction of the final gradient.",
     )  # type: ignore[assignment]
 
-    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+    "graphics.Gradient.Direction : Direction of the final gradient."
 
     binary_colors: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--binary-colors"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("044E29", "157e38", "45bf55", "95ed87"),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the binary characters. Character color is randomly assigned from this list.",
     )  # type: ignore[assignment]
 
     "tuple[graphics.Color, ...] : Tuple of colors for the binary characters. Character color is randomly assigned from this list."
 
     movement_speed: float = ArgField(
         cmd_name="--movement-speed",
-        type_parser=arg_validators.PositiveFloat.type_parser,
+        type_parser=argvalidators.PositiveFloat.type_parser,
         default=1.0,
-        metavar=arg_validators.PositiveFloat.METAVAR,
+        metavar=argvalidators.PositiveFloat.METAVAR,
         help="Speed of the binary groups as they travel around the terminal.",
     )  # type: ignore[assignment]
 
     "float : Speed of the binary groups as they travel around the terminal."
 
     active_binary_groups: float = ArgField(
         cmd_name="--active-binary-groups",
-        type_parser=arg_validators.Ratio.type_parser,
+        type_parser=argvalidators.Ratio.type_parser,
         default=0.05,
-        metavar=arg_validators.Ratio.METAVAR,
+        metavar=argvalidators.Ratio.METAVAR,
         help="Maximum number of binary groups that are active at any given time as a percentage of the total number of binary groups. Lower this to improve performance.",
     )  # type: ignore[assignment]
 
     "float : Maximum number of binary groups that are active at any given time as a percentage of the total number of binary groups. Lower this to improve performance."
 
     @classmethod
     def get_effect_class(cls):
@@ -108,30 +118,23 @@
             self.terminal = terminal
             self.binary_string = format(ord(self.character.symbol), "08b")
             self.binary_characters: list[EffectCharacter] = []
             self.pending_binary_characters: list[EffectCharacter] = []
             self.input_coord = self.character.input_coord
             self.is_active = False
 
-        def travel_complete(self) -> bool:
-            """Determines if the binary representation has completed its travel, meaning all binary characters have reached their input coordinate.
-
-            Returns:
-                bool: True if the binary representation has completed its travel, False otherwise.
-            """
+        def _travel_complete(self) -> bool:
             return all(bin_char.motion.current_coord == self.input_coord for bin_char in self.binary_characters)
 
-        def deactivate(self) -> None:
-            """Deactivates the binary representation by deactivating all binary characters."""
+        def _deactivate(self) -> None:
             for bin_char in self.binary_characters:
                 self.terminal.set_character_visibility(bin_char, False)
             self.is_active = False
 
-        def activate_source_character(self) -> None:
-            """Activates the source character of the binary representation."""
+        def _activate_source_character(self) -> None:
             self.terminal.set_character_visibility(self.character, True)
             self.character.animation.activate_scene(self.character.animation.query_scene("collapse_scn"))
 
     def __init__(self, effect: "BinaryPath") -> None:
         super().__init__(effect)
         self._pending_chars: list[EffectCharacter] = []
         self._active_chars: list[EffectCharacter] = []
@@ -141,15 +144,14 @@
         self._active_binary_reps: list[BinaryPathIterator._BinaryRepresentation] = []
         self._complete = False
         self._phase = "travel"
         self._final_wipe_chars = self._terminal.get_characters_grouped(
             grouping=self._terminal.CharacterGroup.DIAGONAL_TOP_RIGHT_TO_BOTTOM_LEFT
         )
         self._max_active_binary_groups: int = 0
-
         self._build()
 
     def _build(self) -> None:
         final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
             self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
         )
@@ -185,15 +187,15 @@
                 max_column_distance = abs(last_coord.column - bin_rep.character.input_coord.column)
                 max_row_distance = abs(last_coord.row - bin_rep.character.input_coord.row)
                 if last_orientation == "col" and max_row_distance > 0:
                     next_coord = Coord(
                         last_coord.column,
                         last_coord.row
                         + (
-                            random.randint(1, min(max_row_distance, max(10, int(self._terminal.input_width * 0.2))))
+                            random.randint(1, min(max_row_distance, max(10, int(self._terminal._input_width * 0.2))))
                             * row_direction
                         ),
                     )
                     last_orientation = "row"
                 elif last_orientation == "row" and max_column_distance > 0:
                     next_coord = Coord(
                         last_coord.column + (random.randint(1, min(max_column_distance, 4)) * column_direction),
@@ -247,17 +249,17 @@
 
                 if self._active_binary_reps:
                     for active_rep in self._active_binary_reps:
                         if active_rep.pending_binary_characters:
                             next_char = active_rep.pending_binary_characters.pop(0)
                             self._active_chars.append(next_char)
                             self._terminal.set_character_visibility(next_char, True)
-                        elif active_rep.travel_complete():
-                            active_rep.deactivate()
-                            active_rep.activate_source_character()
+                        elif active_rep._travel_complete():
+                            active_rep._deactivate()
+                            active_rep._activate_source_character()
                             self._active_chars.append(active_rep.character)
 
                     self._active_binary_reps = [
                         binary_rep for binary_rep in self._active_binary_reps if binary_rep.is_active
                     ]
 
                 if not self._active_chars:
@@ -282,15 +284,25 @@
             self._last_frame_provided = True
             return self._terminal.get_formatted_output_string()
         else:
             raise StopIteration
 
 
 class BinaryPath(BaseEffect):
-    """Effect that decodes characters into their binary form. Characters travel from outside the output area towards their input coordinate,
-    moving at right angles."""
+    """Decodes characters into their binary form. Characters travel from outside the output area towards their input coordinate, moving at right angles.
+
+    Attributes:
+        effect_config (BinaryPathConfig): Configuration for the BinaryPath effect.
+        terminal_config (TerminalConfig): Configuration for the terminal.
+
+
+    """
 
     _config_cls = BinaryPathConfig
     _iterator_cls = BinaryPathIterator
 
     def __init__(self, input_data: str) -> None:
+        """Initializes the BinaryPath effect with the provided input data.
+
+        Args:
+            input_data (str): The input data to use for the BinaryPath effect."""
         super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_blackhole.py` & `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_blackhole.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,26 @@
+"""
+Creates a blackhole in a starfield, consumes the stars, explodes the input data back into position.
+
+Classes:
+    BlackholeConfig: Configuration for the Blackhole effect.
+    Blackhole: Creates a blackhole in a starfield, consumes the stars, explodes the input data back into position.
+    BlackholeIterator: Iterator for the Blackhole effect. Does not normally need to be called directly.
+
+"""
+
 import random
 import typing
 from dataclasses import dataclass
 
-import terminaltexteffects.utils.arg_validators as arg_validators
-from terminaltexteffects.base_character import EffectCharacter, EventHandler
-from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
-from terminaltexteffects.utils import animation, easing, geometry, graphics
+import terminaltexteffects.utils.argvalidators as argvalidators
+from terminaltexteffects.engine import animation
+from terminaltexteffects.engine.base_character import EffectCharacter, EventHandler
+from terminaltexteffects.engine.base_effect import BaseEffect, BaseEffectIterator
+from terminaltexteffects.utils import easing, geometry, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 from terminaltexteffects.utils.geometry import Coord
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
     return Blackhole, BlackholeConfig
 
@@ -23,70 +34,70 @@
 @dataclass
 class BlackholeConfig(ArgsDataClass):
     """Configuration for the Blackhole effect.
 
     Attributes:
         blackhole_color (graphics.Color): Color for the stars that comprise the blackhole border.
         star_colors (tuple[graphics.Color, ...]): Tuple of colors from which character colors will be chosen and applied after the explosion, but before the cooldown to final color.
-        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
-        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
-        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color."""
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient. If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation. Valid values are n > 0.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the final gradient."""
 
     blackhole_color: graphics.Color = ArgField(
         cmd_name=["--blackhole-color"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         default="ffffff",
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Color for the stars that comprise the blackhole border.",
     )  # type: ignore[assignment]
 
     "graphics.Color : Color for the stars that comprise the blackhole border."
 
     star_colors: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--star-colors"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("ffcc0d", "ff7326", "ff194d", "bf2669", "702a8c", "049dbf"),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="List of colors from which character colors will be chosen and applied after the explosion, but before the cooldown to final color.",
     )  # type: ignore[assignment]
 
     "tuple[graphics.Color, ...] : Tuple of colors from which character colors will be chosen and applied after the explosion, but before the cooldown to final color."
 
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("8A008A", "00D1FF", "ffffff"),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
 
-    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+    "tuple[graphics.Color, ...] : Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color."
 
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name=["--final-gradient-steps"],
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
 
     "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
 
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
-        type_parser=arg_validators.GradientDirection.type_parser,
+        type_parser=argvalidators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.DIAGONAL,
-        metavar=arg_validators.GradientDirection.METAVAR,
-        help="Direction of the gradient for the final color.",
+        metavar=argvalidators.GradientDirection.METAVAR,
+        help="Direction of the final gradient.",
     )  # type: ignore[assignment]
 
-    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+    "graphics.Gradient.Direction : Direction of the final gradient."
 
     @classmethod
     def get_effect_class(cls):
         return Blackhole
 
 
 class BlackholeIterator(BaseEffectIterator[BlackholeConfig]):
@@ -284,15 +295,14 @@
                 cooling_scn,
             )
             character.animation.activate_scene(explode_scn)
             character.motion.activate_path(nearby_path)
             self._active_chars.append(character)
 
     def _build(self) -> None:
-        """Prepares the data for the effect by creating the starfield, blackhole, and consumption scenes/waypoints."""
         final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
             self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
         )
         for character in self._terminal.get_characters():
             self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
         self._prepare_blackhole()
@@ -300,15 +310,14 @@
         self.f_delay = self.formation_delay
         self.next_char_consuming_delay = 0
         self.max_consume = max(min(int(0.1 * len(self._terminal._input_characters)), 15), 2)
         self.phase = "forming"
         self.awaiting_blackhole_chars = list(self._blackhole_chars)
 
     def __next__(self) -> str:
-        """Runs the effect."""
         if self._active_chars or self.phase != "complete":
             if self.phase == "forming":
                 if self.awaiting_blackhole_chars:
                     if not self.f_delay:
                         next_char = self.awaiting_blackhole_chars.pop(0)
                         next_char.motion.activate_path(next_char.motion.query_path("blackhole"))
                         next_char.animation.activate_scene(next_char.animation.query_scene("blackhole"))
@@ -360,14 +369,24 @@
             return next_frame
 
         else:
             raise StopIteration
 
 
 class Blackhole(BaseEffect[BlackholeConfig]):
-    """Effect that creates a blackhole in a starfield, consumes the stars, and explodes the input characters out to position."""
+    """Creates a blackhole in a starfield, consumes the stars, explodes the input data back into position.
+
+    Attributes:
+        effect_config (BlackholeConfig): Configuration for the Blackhole effect.
+        terminal_config (TerminalConfig): Configuration for the terminal.
+    """
 
     _config_cls = BlackholeConfig
     _iterator_cls = BlackholeIterator
 
     def __init__(self, input_data: str) -> None:
+        """Initializes the Blackhole effect with the provided input data.
+
+        Args:
+            input_data (str): The input data to use for the Blackhole effect.
+        """
         super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_bouncyballs.py` & `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_rain.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,200 +1,202 @@
+"""Rain characters from the top of the output area.
+
+Classes:
+    Rain: Rain characters from the top of the output area.
+    RainConfig: Configuration for the Rain effect.
+    RainIterator: Iterator for the Rain effect. Does not normally need to be called directly.
+
+"""
+
 import random
 import typing
 from dataclasses import dataclass
 
-import terminaltexteffects.utils.arg_validators as arg_validators
-from terminaltexteffects.base_character import EffectCharacter
-from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
+import terminaltexteffects.utils.argvalidators as argvalidators
+from terminaltexteffects.engine.base_character import EffectCharacter
+from terminaltexteffects.engine.base_effect import BaseEffect, BaseEffectIterator
 from terminaltexteffects.utils import easing, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 from terminaltexteffects.utils.geometry import Coord
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
-    return BouncyBalls, BouncyBallsConfig
+    return Rain, RainConfig
 
 
 @argclass(
-    name="bouncyballs",
-    help="Characters are bouncy balls falling from the top of the output area.",
-    description="bouncyballs | Characters are bouncy balls falling from the top of the output area.",
-    epilog=f"""{arg_validators.EASING_EPILOG}
-Example: terminaltexteffects bouncyballs --ball-colors d1f4a5 96e2a4 5acda9 --ball-symbols o "*" O 0 . --final-gradient-stops f8ffae 43c6ac --final-gradient-steps 12 --final-gradient-direction diagonal --ball-delay 7 --movement-speed 0.25 --easing OUT_BOUNCE""",
+    name="rain",
+    help="Rain characters from the top of the output area.",
+    description="rain | Rain characters from the top of the output area.",
+    epilog=f"""{argvalidators.EASING_EPILOG} 
+Example: terminaltexteffects rain --rain-symbols o . , "*" "|" --rain-colors 00315C 004C8F 0075DB 3F91D9 78B9F2 9AC8F5 B8D8F8 E3EFFC --final-gradient-stops 488bff b2e7de 57eaf7 --final-gradient-steps 12 --movement-speed 0.1-0.2 --easing IN_QUART""",
 )
 @dataclass
-class BouncyBallsConfig(ArgsDataClass):
-    """Configuration for the BouncyBalls effect.
+class RainConfig(ArgsDataClass):
+    """Configuration for the Rain effect.
 
     Attributes:
-        ball_colors (tuple[graphics.Color, ...]): Tuple of colors from which ball colors will be randomly selected. If no colors are provided, the colors are random.
-        ball_symbols (tuple[str, ...]): Tuple of symbols to use for the balls.
-        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
-        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
-        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
-        ball_delay (int): Number of animation steps between ball drops, increase to reduce ball drop rate.
-        movement_speed (float): Movement speed of the characters. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.
-        easing (typing.Callable): Easing function to use for character movement."""
-
-    ball_colors: tuple[graphics.Color, ...] = ArgField(
-        cmd_name=["--ball-colors"],
-        type_parser=arg_validators.Color.type_parser,
-        metavar=arg_validators.Color.METAVAR,
+        rain_colors (tuple[graphics.Color, ...]): Tuple of colors for the rain drops. Colors are randomly chosen from the tuple.
+        movement_speed (tuple[float, float]): Falling speed range of the rain drops. Valid values are n > 0.
+        rain_symbols (tuple[str, ...]): Tuple of symbols to use for the rain drops. Symbols are randomly chosen from the tuple.
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation. Valid values are n > 0.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the final gradient.
+        easing (easing.EasingFunction): Easing function to use for character movement."""
+
+    rain_colors: tuple[graphics.Color, ...] = ArgField(
+        cmd_name=["--rain-colors"],
+        type_parser=argvalidators.ColorArg.type_parser,
+        metavar=argvalidators.ColorArg.METAVAR,
         nargs="+",
-        default=("d1f4a5", "96e2a4", "5acda9"),
-        help="Space separated list of colors from which ball colors will be randomly selected. If no colors are provided, the colors are random.",
+        default=("00315C", "004C8F", "0075DB", "3F91D9", "78B9F2", "9AC8F5", "B8D8F8", "E3EFFC"),
+        help="List of colors for the rain drops. Colors are randomly chosen from the list.",
     )  # type: ignore[assignment]
-    "tuple[graphics.Color, ...] : Tuple of colors from which ball colors will be randomly selected. If no colors are provided, the colors are random."
+    "tuple[graphics.Color, ...] : Tuple of colors for the rain drops. Colors are randomly chosen from the tuple."
 
-    ball_symbols: tuple[str, ...] = ArgField(
-        cmd_name="--ball-symbols",
-        type_parser=arg_validators.Symbol.type_parser,
+    movement_speed: tuple[float, float] = ArgField(
+        cmd_name="--movement-speed",
+        type_parser=argvalidators.PositiveFloatRange.type_parser,
+        default=(0.1, 0.2),
+        metavar=argvalidators.PositiveFloatRange.METAVAR,
+        help="Falling speed range of the rain drops.",
+    )  # type: ignore[assignment]
+    "tuple[float, float] : Falling speed range of the rain drops."
+
+    rain_symbols: tuple[str, ...] = ArgField(
+        cmd_name="--rain-symbols",
+        type_parser=argvalidators.Symbol.type_parser,
         nargs="+",
-        default=("*", "o", "O", "0", "."),
-        metavar=arg_validators.Symbol.METAVAR,
-        help="Space separated list of symbols to use for the balls.",
+        default=("o", ".", ",", "*", "|"),
+        metavar=argvalidators.Symbol.METAVAR,
+        help="Space separated list of symbols to use for the rain drops. Symbols are randomly chosen from the list.",
     )  # type: ignore[assignment]
-    "tuple[str, ...] : Tuple of symbols to use for the balls."
+    "tuple[str, ...] : Tuple of symbols to use for the rain drops. Symbols are randomly chosen from the tuple."
 
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
-        cmd_name=["--final-gradient-stops"],
-        type_parser=arg_validators.Color.type_parser,
+        cmd_name="--final-gradient-stops",
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
-        default=("f8ffae", "43c6ac"),
-        metavar=arg_validators.Color.METAVAR,
+        default=("488bff", "b2e7de", "57eaf7"),
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
-    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+    "tuple[graphics.Color, ...] : Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color."
 
     final_gradient_steps: tuple[int, ...] = ArgField(
-        cmd_name=["--final-gradient-steps"],
-        type_parser=arg_validators.PositiveInt.type_parser,
+        cmd_name="--final-gradient-steps",
+        type_parser=argvalidators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
     "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
 
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
-        type_parser=arg_validators.GradientDirection.type_parser,
+        type_parser=argvalidators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.DIAGONAL,
-        metavar=arg_validators.GradientDirection.METAVAR,
-        help="Direction of the gradient for the final color.",
-    )  # type: ignore[assignment]
-    "graphics.Gradient.Direction : Direction of the gradient for the final color."
-    ball_delay: int = ArgField(
-        cmd_name="--ball-delay",
-        type_parser=arg_validators.NonNegativeInt.type_parser,
-        default=7,
-        metavar=arg_validators.NonNegativeInt.METAVAR,
-        help="Number of animation steps between ball drops, increase to reduce ball drop rate.",
+        metavar=argvalidators.GradientDirection.METAVAR,
+        help="Direction of the final gradient.",
     )  # type: ignore[assignment]
-    "int : Number of animation steps between ball drops, increase to reduce ball drop rate."
-
-    movement_speed: float = ArgField(
-        cmd_name="--movement-speed",
-        type_parser=arg_validators.PositiveFloat.type_parser,
-        default=0.25,
-        metavar=arg_validators.PositiveFloat.METAVAR,
-        help="Movement speed of the characters. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.",
-    )  # type: ignore[assignment]
-    "float : Movement speed of the characters. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect."
+    "graphics.Gradient.Direction : Direction of the final gradient."
 
     movement_easing: easing.EasingFunction = ArgField(
-        cmd_name="--movement-easing",
-        type_parser=arg_validators.Ease.type_parser,
-        default=easing.out_bounce,
+        cmd_name=["--movement-easing"],
+        default=easing.in_quart,
+        type_parser=argvalidators.Ease.type_parser,
+        metavar=argvalidators.Ease.METAVAR,
         help="Easing function to use for character movement.",
     )  # type: ignore[assignment]
     "easing.EasingFunction : Easing function to use for character movement."
 
     @classmethod
     def get_effect_class(cls):
-        return BouncyBalls
-
+        return Rain
 
-class BouncyBallsIterator(BaseEffectIterator[BouncyBallsConfig]):
-    """Effect that displays the text as bouncy balls falling from the top of the output area."""
 
-    def __init__(self, effect: "BouncyBalls"):
+class RainIterator(BaseEffectIterator[RainConfig]):
+    def __init__(self, effect: "Rain") -> None:
         super().__init__(effect)
         self._pending_chars: list[EffectCharacter] = []
         self._active_chars: list[EffectCharacter] = []
         self._group_by_row: dict[int, list[EffectCharacter | None]] = {}
         self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
         self._build()
 
     def _build(self) -> None:
-        """Prepares the data for the effect by assigning colors and waypoints and
-        organizing the characters by row."""
         final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
             self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
         )
         for character in self._terminal.get_characters():
             self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
-            color = random.choice(self._config.ball_colors)
-            symbol = random.choice(self._config.ball_symbols)
-            ball_scene = character.animation.new_scene()
-            ball_scene.add_frame(symbol, 1, color=color)
-            final_scene = character.animation.new_scene()
-            char_final_gradient = graphics.Gradient(color, self._character_final_color_map[character], steps=10)
-            final_scene.apply_gradient_to_symbols(char_final_gradient, character.input_symbol, 10)
-            character.motion.set_coordinate(
-                Coord(character.input_coord.column, int(self._terminal.output_area.top * random.uniform(1.0, 1.5)))
-            )
-            input_coord_path = character.motion.new_path(
-                speed=self._config.movement_speed, ease=self._config.movement_easing
+
+        for character in self._terminal.get_characters():
+            raindrop_color = random.choice(self._config.rain_colors)
+            rain_scn = character.animation.new_scene()
+            rain_scn.add_frame(random.choice(self._config.rain_symbols), 1, color=raindrop_color)
+            raindrop_gradient = graphics.Gradient(raindrop_color, self._character_final_color_map[character], steps=7)
+            fade_scn = character.animation.new_scene()
+            fade_scn.apply_gradient_to_symbols(raindrop_gradient, character.input_symbol, 5)
+            character.animation.activate_scene(rain_scn)
+            character.motion.set_coordinate(Coord(character.input_coord.column, self._terminal.output_area.top))
+            input_path = character.motion.new_path(
+                speed=random.uniform(self._config.movement_speed[0], self._config.movement_speed[1]),
+                ease=self._config.movement_easing,
             )
-            input_coord_path.new_waypoint(character.input_coord)
-            character.motion.activate_path(input_coord_path)
-            character.animation.activate_scene(ball_scene)
+            input_path.new_waypoint(character.input_coord)
+
             character.event_handler.register_event(
                 character.event_handler.Event.PATH_COMPLETE,
-                input_coord_path,
+                input_path,
                 character.event_handler.Action.ACTIVATE_SCENE,
-                final_scene,
+                fade_scn,
             )
+            character.motion.activate_path(input_path)
             self._pending_chars.append(character)
         for character in sorted(self._pending_chars, key=lambda c: c.input_coord.row):
             if character.input_coord.row not in self._group_by_row:
                 self._group_by_row[character.input_coord.row] = []
             self._group_by_row[character.input_coord.row].append(character)
         self._pending_chars.clear()
-        self.ball_delay = 0
 
     def __next__(self) -> str:
-        """Runs the effect."""
         if self._group_by_row or self._active_chars or self._pending_chars:
             if not self._pending_chars and self._group_by_row:
                 self._pending_chars.extend(self._group_by_row.pop(min(self._group_by_row.keys())))  # type: ignore
             if self._pending_chars:
-                if self.ball_delay == 0:
-                    for _ in range(random.randint(2, 6)):
-                        if self._pending_chars:
-                            next_character = self._pending_chars.pop(random.randint(0, len(self._pending_chars) - 1))
-                            self._terminal.set_character_visibility(next_character, True)
-                            self._active_chars.append(next_character)
-                        else:
-                            break
-                    self.ball_delay = self._config.ball_delay
-                else:
-                    self.ball_delay -= 1
+                for _ in range(random.randint(1, 3)):
+                    if self._pending_chars:
+                        next_character = self._pending_chars.pop(random.randint(0, len(self._pending_chars) - 1))
+                        self._terminal.set_character_visibility(next_character, True)
+                        self._active_chars.append(next_character)
 
+                    else:
+                        break
             for character in self._active_chars:
                 character.tick()
+
             self._active_chars = [character for character in self._active_chars if character.is_active]
             return self._terminal.get_formatted_output_string()
         else:
             raise StopIteration
 
 
-class BouncyBalls(BaseEffect[BouncyBallsConfig]):
-    """Effect that displays the text as bouncy balls falling from the top of the output area."""
+class Rain(BaseEffect[RainConfig]):
+    """Rain characters from the top of the output area.
+
+    Attributes:
+        effect_config (PourConfig): Configuration for the effect.
+        terminal_config (TerminalConfig): Configuration for the terminal.
+    """
 
-    _config_cls = BouncyBallsConfig
-    _iterator_cls = BouncyBallsIterator
+    _config_cls = RainConfig
+    _iterator_cls = RainIterator
 
     def __init__(self, input_data: str) -> None:
+        """Initialize the effect with the provided input data.
+
+        Args:
+            input_data (str): The input data to use for the effect."""
         super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_bubbles.py` & `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_bubbles.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,148 +1,154 @@
+"""Forms bubbles with the characters. Bubbles float down and pop.
+
+Classes:
+    Bubbles: Forms bubbles with the characters. Bubbles float down and pop.
+    BubblesConfig: Configuration for the Bubbles effect.
+    BubblesIterator: Iterates over the Bubbles effect. Does not normally need to be called directly.
+"""
+
 import random
 import typing
 from dataclasses import dataclass
 
-import terminaltexteffects.utils.arg_validators as arg_validators
-from terminaltexteffects.base_character import EffectCharacter, EventHandler
-from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
+import terminaltexteffects.utils.argvalidators as argvalidators
+from terminaltexteffects.engine.base_character import EffectCharacter, EventHandler
+from terminaltexteffects.engine.base_effect import BaseEffect, BaseEffectIterator
+from terminaltexteffects.engine.terminal import Terminal
 from terminaltexteffects.utils import easing, geometry, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 from terminaltexteffects.utils.geometry import Coord
-from terminaltexteffects.utils.terminal import Terminal
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
     return Bubbles, BubblesConfig
 
 
 @argclass(
     name="bubbles",
     help="Characters are formed into bubbles that float down and pop.",
     description="bubbles | Characters are formed into bubbles that float down and pop.",
-    epilog=f"""{arg_validators.EASING_EPILOG}
+    epilog=f"""{argvalidators.EASING_EPILOG}
 
 Example: terminaltexteffects bubbles --bubble-colors d33aff 7395c4 43c2a7 02ff7f --pop-color ffffff --final-gradient-stops d33aff 02ff7f --final-gradient-steps 12 --final-gradient-direction diagonal --bubble-speed 0.1 --bubble-delay 50 --pop-condition row --easing IN_OUT_SINE""",
 )
 @dataclass
 class BubblesConfig(ArgsDataClass):
     """Configuration for the Bubbles effect.
 
     Attributes:
         rainbow (bool): If set, the bubbles will be colored with a rotating rainbow gradient.
         bubble_colors (tuple[graphics.Color, ...]): Tuple of colors for the bubbles. Ignored if --no-rainbow is left as default False.
         pop_color (graphics.Color): Color for the spray emitted when a bubble pops.
-        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
-        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
-        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
-        bubble_speed (float): Speed of the floating bubbles. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.
-        bubble_delay (int): Number of animation steps between bubbles.
-        pop_condition (str): Condition for a bubble to pop. 'row' will pop the bubble when it reaches the the lowest row for which a character in the bubble originates. 'bottom' will pop the bubble at the bottom row of the terminal. 'anywhere' will pop the bubble randomly, or at the bottom of the terminal.
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation. Valid values are n > 0.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the final gradient.
+        bubble_speed (float): Speed of the floating bubbles. Valid values are n > 0.
+        bubble_delay (int): Number of frames between bubbles. Valid values are n >= 0.
+        pop_condition (typing.Literal["row", "bottom", "anywhere"]): Condition for a bubble to pop. 'row' will pop the bubble when it reaches the the lowest row for which a character in the bubble originates. 'bottom' will pop the bubble at the bottom row of the terminal. 'anywhere' will pop the bubble randomly, or at the bottom of the terminal.
         easing (typing.Callable): Easing function to use for character movement after a bubble pops.
     """
 
     rainbow: bool = ArgField(
         cmd_name="--rainbow",
         action="store_true",
         default=False,
         help="If set, the bubbles will be colored with a rotating rainbow gradient.",
     )  # type: ignore[assignment]
     "bool : If set, the bubbles will be colored with a rotating rainbow gradient."
 
     bubble_colors: tuple[graphics.Color, ...] = ArgField(
         cmd_name="--bubble-colors",
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("d33aff", "7395c4", "43c2a7", "02ff7f"),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the bubbles. Ignored if --no-rainbow is left as default False.",
     )  # type: ignore[assignment]
     "tuple[graphics.Color, ...] : Tuple of colors for the bubbles. Ignored if --no-rainbow is left as default False."
 
     pop_color: graphics.Color = ArgField(
         cmd_name="--pop-color",
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         default="ffffff",
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Color for the spray emitted when a bubble pops.",
     )  # type: ignore[assignment]
     "graphics.Color : Color for the spray emitted when a bubble pops."
 
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("d33aff", "02ff7f"),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
-    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+    "tuple[graphics.Color, ...] : Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color."
 
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name="--final-gradient-steps",
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
     "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
 
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
-        type_parser=arg_validators.GradientDirection.type_parser,
+        type_parser=argvalidators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.DIAGONAL,
-        metavar=arg_validators.GradientDirection.METAVAR,
-        help="Direction of the gradient for the final color.",
+        metavar=argvalidators.GradientDirection.METAVAR,
+        help="Direction of the final gradient.",
     )  # type: ignore[assignment]
-    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+    "graphics.Gradient.Direction : Direction of the final gradient."
 
     bubble_speed: float = ArgField(
         cmd_name="--bubble-speed",
-        type_parser=arg_validators.PositiveFloat.type_parser,
+        type_parser=argvalidators.PositiveFloat.type_parser,
         default=0.1,
-        metavar=arg_validators.PositiveFloat.METAVAR,
-        help="Speed of the floating bubbles. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.",
+        metavar=argvalidators.PositiveFloat.METAVAR,
+        help="Speed of the floating bubbles. ",
     )  # type: ignore[assignment]
-    "float : Speed of the floating bubbles. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect."
+    "float : Speed of the floating bubbles. "
 
     bubble_delay: int = ArgField(
         cmd_name="--bubble-delay",
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         default=50,
-        metavar=arg_validators.PositiveInt.METAVAR,
-        help="Number of animation steps between bubbles.",
+        metavar=argvalidators.PositiveInt.METAVAR,
+        help="Number of frames between bubbles.",
     )  # type: ignore[assignment]
-    "int : Number of animation steps between bubbles."
+    "int : Number of frames between bubbles."
 
-    pop_condition: str = ArgField(
+    pop_condition: typing.Literal["row", "bottom", "anywhere"] = ArgField(
         cmd_name="--pop-condition",
         default="row",
         choices=["row", "bottom", "anywhere"],
         help="Condition for a bubble to pop. 'row' will pop the bubble when it reaches the the lowest row for which a character in the bubble originates. 'bottom' will pop the bubble at the bottom row of the terminal. 'anywhere' will pop the bubble randomly, or at the bottom of the terminal.",
     )  # type: ignore[assignment]
-    "str : Condition for a bubble to pop. 'row' will pop the bubble when it reaches the the lowest row for which a character in the bubble originates. 'bottom' will pop the bubble at the bottom row of the terminal. 'anywhere' will pop the bubble randomly, or at the bottom of the terminal."
+    "typing.Literal['row', 'bottom', 'anywhere'] : Condition for a bubble to pop. 'row' will pop the bubble when it reaches the the lowest row for which a character in the bubble originates. 'bottom' will pop the bubble at the bottom row of the terminal. 'anywhere' will pop the bubble randomly, or at the bottom of the terminal."
 
     movement_easing: easing.EasingFunction = ArgField(
         cmd_name=["--movement-easing"],
         default=easing.in_out_sine,
-        type_parser=arg_validators.Ease.type_parser,
-        metavar=arg_validators.Ease.METAVAR,
+        type_parser=argvalidators.Ease.type_parser,
+        metavar=argvalidators.Ease.METAVAR,
         help="Easing function to use for character movement after a bubble pops.",
     )  # type: ignore[assignment]
     "easing.EasingFunction : Easing function to use for character movement after a bubble pops."
 
     @classmethod
     def get_effect_class(cls):
         return Bubbles
 
 
 class BubblesIterator(BaseEffectIterator[BubblesConfig]):
-    """Effect that forms circles with the characters. Circles float down and pop into the characters."""
-
     class _Bubble:
         def __init__(
             self,
             effect: "BubblesIterator",
             origin: Coord,
             characters: list[EffectCharacter],
             terminal: Terminal,
@@ -337,14 +343,23 @@
             self._active_chars = [character for character in self._active_chars if character.is_active]
             return next_frame
         else:
             raise StopIteration
 
 
 class Bubbles(BaseEffect[BubblesConfig]):
-    """Effect that forms circles with the characters. Circles float down and pop into the characters."""
+    """Forms bubbles with the characters. Bubbles float down and pop.
+
+    Attributes:
+        effect_config (BubblesConfig): Configuration for the effect.
+        terminal_config (TerminalConfig): Configuration for the terminal.
+    """
 
     _config_cls = BubblesConfig
     _iterator_cls = BubblesIterator
 
     def __init__(self, input_data: str) -> None:
+        """Initialize the effect with the provided input data.
+
+        Args:
+            input_data (str): The input data to use for the effect."""
         super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_burn.py` & `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_burn.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,23 @@
+"""Characters are ignited and burn up the screen.
+
+Classes:
+    Burn: Characters are ignited and burn up the screen.
+    BurnConfig: Configuration for the Burn effect.
+    BurnIterator: Iterates over the Burn effect. Does not normally need to be called directly.
+
+"""
+
 import random
 import typing
 from dataclasses import dataclass
 
-import terminaltexteffects.utils.arg_validators as arg_validators
-from terminaltexteffects.base_character import EffectCharacter, EventHandler
-from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
+import terminaltexteffects.utils.argvalidators as argvalidators
+from terminaltexteffects.engine.base_character import EffectCharacter, EventHandler
+from terminaltexteffects.engine.base_effect import BaseEffect, BaseEffectIterator
 from terminaltexteffects.utils import graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
     return Burn, BurnConfig
 
@@ -22,83 +31,80 @@
 @dataclass
 class BurnConfig(ArgsDataClass):
     """Configuration for the Burn effect.
 
     Attributes:
         starting_color (graphics.Color): Color of the characters before they start to burn.
         burn_colors (tuple[graphics.Color, ...]): Colors transitioned through as the characters burn.
-        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
-        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
-        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color."""
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation. Valid values are n > 0.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the final gradient."""
 
     starting_color: graphics.Color = ArgField(
         cmd_name="--starting-color",
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         default="837373",
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Color of the characters before they start to burn.",
     )  # type: ignore[assignment]
     "graphics.Color : Color of the characters before they start to burn."
 
     burn_colors: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--burn-colors"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         default=("ffffff", "fff75d", "fe650d", "8A003C", "510100"),
         nargs="+",
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Colors transitioned through as the characters burn.",
     )  # type: ignore[assignment]
     "tuple[graphics.Color, ...] : Colors transitioned through as the characters burn."
 
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("00c3ff", "ffff1c"),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
-    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+    "tuple[graphics.Color, ...] : Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color."
 
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name=["--final-gradient-steps"],
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
     "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
 
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
-        type_parser=arg_validators.GradientDirection.type_parser,
+        type_parser=argvalidators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.VERTICAL,
-        metavar=arg_validators.GradientDirection.METAVAR,
-        help="Direction of the gradient for the final color.",
+        metavar=argvalidators.GradientDirection.METAVAR,
+        help="Direction of the final gradient.",
     )  # type: ignore[assignment]
-    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+    "graphics.Gradient.Direction : Direction of the final gradient."
 
     @classmethod
     def get_effect_class(cls):
         return Burn
 
 
 class BurnIterator(BaseEffectIterator[BurnConfig]):
-    """Effect that burns up the screen."""
-
     def __init__(self, effect: "Burn"):
         super().__init__(effect)
         self._pending_chars: list[EffectCharacter] = []
         self._active_chars: list[EffectCharacter] = []
         self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
         self._build()
 
     def _build(self) -> None:
-        """Prepares the data for the effect by building the burn animation and organizing the data into columns."""
         vertical_build_order = [
             "'",
             ".",
             "▖",
             "▙",
             "█",
             "▜",
@@ -156,14 +162,23 @@
             self._active_chars = [character for character in self._active_chars if character.is_active]
             return self._terminal.get_formatted_output_string()
         else:
             raise StopIteration
 
 
 class Burn(BaseEffect[BurnConfig]):
-    """Effect that burns up the screen."""
+    """Characters are ignited and burn up the screen.
+
+    Attributes:
+        effect_config (BurnConfig): Configuration for the effect.
+        terminal_config (TerminalConfig): Configuration for the terminal.
+    """
 
     _config_cls = BurnConfig
     _iterator_cls = BurnIterator
 
     def __init__(self, input_data: str) -> None:
+        """Initialize the effect with the provided input data.
+
+        Args:
+            input_data (str): The input data to use for the effect."""
         super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_crumble.py` & `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_crumble.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,25 @@
+"""Characters crumble into dust before being vacuumed up and reformed.
+
+Classes:
+    Crumble: Characters crumble into dust before being vacuumed up and reformed.
+    CrumbleConfig: Configuration for the Crumble effect.
+    CrumbleIterator: Iterates over the Crumble effect. Does not normally need to be called directly.
+
+"""
+
 import random
 import typing
 from dataclasses import dataclass
 
-import terminaltexteffects.utils.arg_validators as arg_validators
-from terminaltexteffects.base_character import EffectCharacter, EventHandler
-from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
-from terminaltexteffects.utils import animation, easing, graphics
+import terminaltexteffects.utils.argvalidators as argvalidators
+from terminaltexteffects.engine import animation
+from terminaltexteffects.engine.base_character import EffectCharacter, EventHandler
+from terminaltexteffects.engine.base_effect import BaseEffect, BaseEffectIterator
+from terminaltexteffects.utils import easing, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 from terminaltexteffects.utils.geometry import Coord
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
     return Crumble, CrumbleConfig
 
@@ -21,55 +31,53 @@
     epilog="""Example: terminaltexteffects crumble --final-gradient-stops 5CE1FF FF8C00 --final-gradient-steps 12 --final-gradient-direction diagonal""",
 )
 @dataclass
 class CrumbleConfig(ArgsDataClass):
     """Configuration for the Crumble effect.
 
     Attributes:
-        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
-        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
-        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color."""
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation. Valid values are n > 0.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the final gradient."""
 
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("5CE1FF", "FF8C00"),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
-    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+    "tuple[graphics.Color, ...] : Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color."
 
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name="--final-gradient-steps",
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
     "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
 
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
-        type_parser=arg_validators.GradientDirection.type_parser,
+        type_parser=argvalidators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.DIAGONAL,
-        metavar=arg_validators.GradientDirection.METAVAR,
-        help="Direction of the gradient for the final color.",
+        metavar=argvalidators.GradientDirection.METAVAR,
+        help="Direction of the final gradient.",
     )  # type: ignore[assignment]
-    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+    "graphics.Gradient.Direction : Direction of the final gradient."
 
     @classmethod
     def get_effect_class(cls):
         return Crumble
 
 
 class CrumbleIterator(BaseEffectIterator[CrumbleConfig]):
-    """Characters crumble into dust before being vacuumed up and rebuilt."""
-
     def __init__(self, effect: "Crumble"):
         super().__init__(effect)
 
         self._pending_chars: list[EffectCharacter] = []
         self._active_chars: list[EffectCharacter] = []
         self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
         self._build()
@@ -196,14 +204,23 @@
             self._active_chars = [character for character in self._active_chars if character.is_active]
             return next_frame
         else:
             raise StopIteration
 
 
 class Crumble(BaseEffect[CrumbleConfig]):
-    """Characters crumble into dust before being vacuumed up and rebuilt."""
+    """Characters crumble into dust before being vacuumed up and reformed.
+
+    Attributes:
+        effect_config (CrumbleConfig): Configuration for the effect.
+        terminal_config (TerminalConfig): Configuration for the terminal.
+    """
 
     _config_cls = CrumbleConfig
     _iterator_cls = CrumbleIterator
 
     def __init__(self, input_data: str) -> None:
+        """Initialize the effect with the provided input data.
+
+        Args:
+            input_data (str): The input data to use for the effect."""
         super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_decrypt.py` & `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_decrypt.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,23 @@
+"""Movie style text decryption effect.
+
+Classes:
+    Decrypt: Movie style text decryption effect.
+    DecryptConfig: Configuration for the Decrypt effect.
+    DecryptIterator: Iterates over the Decrypt effect. Does not normally need to be called directly.
+"""
+
 import random
 import typing
 from dataclasses import dataclass
 
-from terminaltexteffects.base_character import EffectCharacter, EventHandler
-from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
-from terminaltexteffects.utils import animation, arg_validators, graphics
+from terminaltexteffects.engine import animation
+from terminaltexteffects.engine.base_character import EffectCharacter, EventHandler
+from terminaltexteffects.engine.base_effect import BaseEffect, BaseEffectIterator
+from terminaltexteffects.utils import argvalidators, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
     return Decrypt, DecryptConfig
 
 
@@ -23,76 +32,72 @@
     """Configuration for the Decrypt effect.
 
     Attributes:
         typing_speed (int): Number of characters typed per keystroke.
         ciphertext_colors (tuple[graphics.Color, ...]): Colors for the ciphertext. Color will be randomly selected for each character.
         final_gradient_stops (tuple[graphics.Color, ...]): Colors for the character gradient. If only one color is provided, the characters will be displayed in that color.
         final_gradient_steps (tuple[int, ...]): Number of gradient steps to use. More steps will create a smoother and longer gradient animation.
-        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color."""
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the final gradient."""
 
     typing_speed: int = ArgField(
         cmd_name="--typing-speed",
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         default=1,
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Number of characters typed per keystroke.",
     )  # type: ignore[assignment]
     "int : Number of characters typed per keystroke."
 
     ciphertext_colors: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--ciphertext-colors"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("008000", "00cb00", "00ff00"),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the ciphertext. Color will be randomly selected for each character.",
     )  # type: ignore[assignment]
     "tuple[graphics.Color, ...] : Colors for the ciphertext. Color will be randomly selected for each character."
 
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("eda000",),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
     "tuple[graphics.Color, ...] : Colors for the character gradient. If only one color is provided, the characters will be displayed in that color."
 
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name="--final-gradient-steps",
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
     "tuple[int, ...] : Number of gradient steps to use. More steps will create a smoother and longer gradient animation."
 
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
-        type_parser=arg_validators.GradientDirection.type_parser,
+        type_parser=argvalidators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.VERTICAL,
-        metavar=arg_validators.GradientDirection.METAVAR,
-        help="Direction of the gradient for the final color.",
+        metavar=argvalidators.GradientDirection.METAVAR,
+        help="Direction of the final gradient.",
     )  # type: ignore[assignment]
-    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+    "graphics.Gradient.Direction : Direction of the final gradient."
 
     @classmethod
     def get_effect_class(cls):
         return Decrypt
 
 
 class DecryptIterator(BaseEffectIterator[DecryptConfig]):
-    """Effect that shows a movie style text decryption effect."""
-
     @dataclass
     class _DecryptChars:
-        """Various decimal utf-8 character ranges."""
-
         keyboard = list(range(33, 127))
         blocks = list(range(9608, 9632))
         box_drawing = list(range(9472, 9599))
         misc = list(range(174, 452))
 
     def __init__(self, effect: "Decrypt") -> None:
         super().__init__(effect)
@@ -133,27 +138,25 @@
                 duration = random.randrange(5, 10)  # shorter duration creates flipping effect
             slow_decrypt_scene.add_frame(symbol, duration, color=color)
         discovered_scene = character.animation.new_scene(id="discovered")
         discovered_gradient = graphics.Gradient("ffffff", self._character_final_color_map[character], steps=10)
         discovered_scene.apply_gradient_to_symbols(discovered_gradient, character.input_symbol, 8)
 
     def _prepare_data_for_type_effect(self) -> None:
-        """Prepares the data for the effect by building the animation for each character."""
         for character in self._terminal.get_characters():
             typing_scene = character.animation.new_scene(id="typing")
             for block_char in ["▉", "▓", "▒", "░"]:
                 typing_scene.add_frame(block_char, 2, color=random.choice(self._config.ciphertext_colors))
 
             typing_scene.add_frame(
                 random.choice(self._encrypted_symbols), 2, color=random.choice(self._config.ciphertext_colors)
             )
             self._typing_pending_chars.append(character)
 
     def _prepare_data_for_decrypt_effect(self) -> None:
-        """Prepares the data for the effect by building the animation for each character."""
         for character in self._terminal.get_characters():
             self._make_decrypting_animation_scenes(character)
             character.event_handler.register_event(
                 EventHandler.Event.SCENE_COMPLETE,
                 character.animation.query_scene("fast_decrypt"),
                 EventHandler.Action.ACTIVATE_SCENE,
                 character.animation.query_scene("slow_decrypt"),
@@ -164,15 +167,14 @@
                 EventHandler.Action.ACTIVATE_SCENE,
                 character.animation.query_scene("discovered"),
             )
             character.animation.activate_scene(character.animation.query_scene("fast_decrypt"))
             self._decrypting_pending_chars.append(character)
 
     def _build(self) -> None:
-        """Builds the effect."""
         final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
             self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
         )
         for character in self._terminal.get_characters():
             self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
         self._prepare_data_for_type_effect()
@@ -208,17 +210,27 @@
             else:
                 raise StopIteration
         else:
             raise StopIteration
 
 
 class Decrypt(BaseEffect[DecryptConfig]):
-    """Effect that shows a movie style text decryption effect."""
+    """Movie style text decryption effect.
+
+    Attributes:
+        effect_config (DecryptConfig): Configuration for the effect.
+        terminal_config (TerminalConfig): Configuration for the terminal.
+
+    """
 
     _config_cls = DecryptConfig
     _iterator_cls = DecryptIterator
 
     def __init__(self, input_data: str) -> None:
+        """Initialize the effect with the provided input data.
+
+        Args:
+            input_data (str): The input data to use for the effect."""
         super().__init__(input_data)
 
     def __iter__(self) -> DecryptIterator:
         return DecryptIterator(self)
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_errorcorrect.py` & `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_errorcorrect.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,137 +1,143 @@
+"""Swaps characters from an incorrect initial position to the correct position.
+
+Classes:
+    ErrorCorrect: Swaps characters from an incorrect initial position to the correct position.
+    ErrorCorrectConfig: Configuration for the ErrorCorrect effect.
+    ErrorCorrectIterator: Iterates over the effect. Does not normally need to be called directly.
+"""
+
 import random
 import typing
 from dataclasses import dataclass
 
-import terminaltexteffects.utils.arg_validators as arg_validators
-from terminaltexteffects.base_character import EffectCharacter, EventHandler
-from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
-from terminaltexteffects.utils import animation, graphics
+import terminaltexteffects.utils.argvalidators as argvalidators
+from terminaltexteffects.engine import animation
+from terminaltexteffects.engine.base_character import EffectCharacter, EventHandler
+from terminaltexteffects.engine.base_effect import BaseEffect, BaseEffectIterator
+from terminaltexteffects.utils import graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
     return ErrorCorrect, ErrorCorrectConfig
 
 
 @argclass(
     name="errorcorrect",
     help="Some characters start in the wrong position and are corrected in sequence.",
     description="errorcorrect | Some characters start in the wrong position and are corrected in sequence.",
-    epilog=f"""{arg_validators.EASING_EPILOG}
+    epilog=f"""{argvalidators.EASING_EPILOG}
     
 Example: terminaltexteffects errorcorrect --error-pairs 0.1 --swap-delay 10 --error-color e74c3c --correct-color 45bf55 --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --movement-speed 0.5""",
 )
 @dataclass
 class ErrorCorrectConfig(ArgsDataClass):
     """Configuration for the ErrorCorrect effect.
 
     Attributes:
-        error_pairs (float): Percent of characters that are in the wrong position. This is a float between 0 and 1.0. 0.2 means 20 percent of the characters will be in the wrong position.
-        swap_delay (int): Number of animation steps between swaps.
+        error_pairs (float): Percent of characters that are in the wrong position. This is a float between 0 and 1.0. 0.2 means 20 percent of the characters will be in the wrong position. Valid values are 0 < n <= 1.0.
+        swap_delay (int): Number of frames between swaps. Valid values are n >= 0.
         error_color (graphics.Color): Color for the characters that are in the wrong position.
         correct_color (graphics.Color): Color for the characters once corrected, this is a gradient from error-color and fades to final-color.
-        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
-        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
-        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
-        movement_speed (float): Speed of the characters while moving to the correct position. Note: Speed effects the number of steps in the easing function."""
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation. Valid values are n > 0.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the final gradient.
+        movement_speed (float): Speed of the characters while moving to the correct position. Valid values are n > 0."""
 
     error_pairs: float = ArgField(
         cmd_name="--error-pairs",
-        type_parser=arg_validators.PositiveFloat.type_parser,
+        type_parser=argvalidators.PositiveFloat.type_parser,
         default=0.1,
         metavar="(int > 0)",
         help="Percent of characters that are in the wrong position. This is a float between 0 and 1.0. 0.2 means 20 percent of the characters will be in the wrong position.",
     )  # type: ignore[assignment]
     "float : Percent of characters that are in the wrong position. This is a float between 0 and 1.0. 0.2 means 20 percent of the characters will be in the wrong position."
 
     swap_delay: int = ArgField(
         cmd_name="--swap-delay",
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         default=10,
         metavar="(int > 0)",
-        help="Number of animation steps between swaps.",
+        help="Number of frames between swaps.",
     )  # type: ignore[assignment]
-    "int : Number of animation steps between swaps."
+    "int : Number of frames between swaps."
 
     error_color: graphics.Color = ArgField(
         cmd_name=["--error-color"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         default="e74c3c",
         metavar="(XTerm [0-255] OR RGB Hex [000000-ffffff])",
         help="Color for the characters that are in the wrong position.",
     )  # type: ignore[assignment]
     "graphics.Color : Color for the characters that are in the wrong position."
 
     correct_color: graphics.Color = ArgField(
         cmd_name=["--correct-color"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         default="45bf55",
         metavar="(XTerm [0-255] OR RGB Hex [000000-ffffff])",
         help="Color for the characters once corrected, this is a gradient from error-color and fades to final-color.",
     )  # type: ignore[assignment]
     "graphics.Color : Color for the characters once corrected, this is a gradient from error-color and fades to final-color."
 
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("8A008A", "00D1FF", "FFFFFF"),
         metavar="(XTerm [0-255] OR RGB Hex [000000-ffffff])",
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
-    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+    "tuple[graphics.Color, ...] : Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color."
 
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name="--final-gradient-steps",
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
         metavar="(int > 0)",
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
     "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
 
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
-        type_parser=arg_validators.GradientDirection.type_parser,
+        type_parser=argvalidators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.VERTICAL,
-        metavar=arg_validators.GradientDirection.METAVAR,
-        help="Direction of the gradient for the final color.",
+        metavar=argvalidators.GradientDirection.METAVAR,
+        help="Direction of the final gradient.",
     )  # type: ignore[assignment]
-    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+    "graphics.Gradient.Direction : Direction of the final gradient."
 
     movement_speed: float = ArgField(
         cmd_name="--movement-speed",
-        type_parser=arg_validators.PositiveFloat.type_parser,
+        type_parser=argvalidators.PositiveFloat.type_parser,
         default=0.5,
         metavar="(float > 0)",
-        help="Speed of the characters while moving to the correct position. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.",
+        help="Speed of the characters while moving to the correct position. ",
     )  # type: ignore[assignment]
-    "float : Speed of the characters while moving to the correct position. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect."
+    "float : Speed of the characters while moving to the correct position. "
 
     @classmethod
     def get_effect_class(cls):
         return ErrorCorrect
 
 
 class ErrorCorrectIterator(BaseEffectIterator[ErrorCorrectConfig]):
-    """Effect that swaps characters from an incorrect initial position to the correct position."""
-
     def __init__(self, effect: "ErrorCorrect") -> None:
         super().__init__(effect)
         self._pending_chars: list[EffectCharacter] = []
         self._active_chars: list[EffectCharacter] = []
         self._swapped: list[tuple[EffectCharacter, EffectCharacter]] = []
         self._swap_delay = 0
         self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
         self._build()
 
     def _build(self) -> None:
-        """Prepares the data for the effect by swapping positions and generating animations and waypoints."""
         final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
             self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
         )
         for character in self._terminal.get_characters():
             self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
         for character in self._terminal.get_characters():
@@ -238,14 +244,23 @@
             self._active_chars = [character for character in self._active_chars if character.is_active]
             return next_frame
         else:
             raise StopIteration
 
 
 class ErrorCorrect(BaseEffect[ErrorCorrectConfig]):
-    """Effect that swaps characters from an incorrect initial position to the correct position."""
+    """Swaps characters from an incorrect initial position to the correct position.
+
+    Attributes:
+        effect_config (ErrorCorrectConfig): Configuration for the effect.
+        terminal_config (TerminalConfig): Configuration for the terminal.
+    """
 
     _config_cls = ErrorCorrectConfig
     _iterator_cls = ErrorCorrectIterator
 
     def __init__(self, input_data: str) -> None:
+        """Initialize the effect with the provided input data.
+
+        Args:
+            input_data (str): The input data to use for the effect."""
         super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_expand.py` & `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_expand.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,117 +1,121 @@
+"""Characters expand from the center.
+
+Classes:
+    Expand: Characters expand from the center.
+    ExpandConfig: Configuration for the Expand effect.
+    ExpandIterator: Iterates over the effect. Does not normally need to be called directly.
+"""
+
 import typing
 from dataclasses import dataclass
 
-import terminaltexteffects.utils.arg_validators as arg_validators
-from terminaltexteffects.base_character import EffectCharacter, EventHandler
-from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
+import terminaltexteffects.utils.argvalidators as argvalidators
+from terminaltexteffects.engine.base_character import EffectCharacter, EventHandler
+from terminaltexteffects.engine.base_effect import BaseEffect, BaseEffectIterator
 from terminaltexteffects.utils import easing, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
     return Expand, ExpandConfig
 
 
 @argclass(
     name="expand",
     help="Expands the text from a single point.",
     description="expand | Expands the text from a single point.",
-    epilog=f"""{arg_validators.EASING_EPILOG}
+    epilog=f"""{argvalidators.EASING_EPILOG}
     
 Example: terminaltexteffects expand --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --final-gradient-frames 5 --movement-speed 0.35 --expand-easing IN_OUT_QUART""",
 )
 @dataclass
 class ExpandConfig(ArgsDataClass):
     """Configuration for the Expand effect.
 
     Attributes:
-        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
-        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation. Valid values are n > 0.
         final_gradient_frames (int): Number of frames to display each gradient step.
-        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
-        movement_speed (float): Movement speed of the characters. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.
-        expand_easing (typing.Callable): Easing function to use for character movement."""
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the final gradient.
+        movement_speed (float): Movement speed of the characters.
+        expand_easing (easing.EasingFunction): Easing function to use for character movement."""
 
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("8A008A", "00D1FF", "FFFFFF"),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
-    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+    "tuple[graphics.Color, ...] : Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color."
 
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name="--final-gradient-steps",
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
     "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
 
     final_gradient_frames: int = ArgField(
         cmd_name="--final-gradient-frames",
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         default=5,
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Number of frames to display each gradient step.",
     )  # type: ignore[assignment]
     "int : Number of frames to display each gradient step."
 
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
-        type_parser=arg_validators.GradientDirection.type_parser,
+        type_parser=argvalidators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.VERTICAL,
-        metavar=arg_validators.GradientDirection.METAVAR,
-        help="Direction of the gradient for the final color.",
+        metavar=argvalidators.GradientDirection.METAVAR,
+        help="Direction of the final gradient.",
     )  # type: ignore[assignment]
-    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+    "graphics.Gradient.Direction : Direction of the final gradient."
 
     movement_speed: float = ArgField(
         cmd_name="--movement-speed",
-        type_parser=arg_validators.PositiveFloat.type_parser,
+        type_parser=argvalidators.PositiveFloat.type_parser,
         default=0.35,
-        metavar=arg_validators.PositiveFloat.METAVAR,
-        help="Movement speed of the characters. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.",
+        metavar=argvalidators.PositiveFloat.METAVAR,
+        help="Movement speed of the characters. ",
     )  # type: ignore[assignment]
-    "float : Movement speed of the characters. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect."
+    "float : Movement speed of the characters. "
 
     expand_easing: easing.EasingFunction = ArgField(
         cmd_name="--expand-easing",
         default=easing.in_out_quart,
-        type_parser=arg_validators.Ease.type_parser,
+        type_parser=argvalidators.Ease.type_parser,
         help="Easing function to use for character movement.",
     )  # type: ignore[assignment]
     "easing.EasingFunction : Easing function to use for character movement."
 
     @classmethod
     def get_effect_class(cls):
         return Expand
 
 
 class ExpandIterator(BaseEffectIterator[ExpandConfig]):
-    """Effect that draws the characters expanding from a single point."""
-
     def __init__(
         self,
         effect: "Expand",
     ):
         super().__init__(effect)
         self._pending_chars: list[EffectCharacter] = []
         self._active_chars: list[EffectCharacter] = []
         self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
         self._build()
 
     def _build(self) -> None:
-        """Prepares the data for the effect by starting all of the characters from a point in the middle of the input data."""
-
         final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
             self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
         )
         for character in self._terminal.get_characters():
             self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
         for character in self._terminal.get_characters():
@@ -134,25 +138,34 @@
             gradient = graphics.Gradient(
                 final_gradient.spectrum[0], self._character_final_color_map[character], steps=10
             )
             gradient_scn.apply_gradient_to_symbols(gradient, character.input_symbol, self._config.final_gradient_frames)
             character.animation.activate_scene(gradient_scn)
 
     def __next__(self) -> str:
-        """Runs the effect."""
         if self._active_chars:
             for character in self._active_chars:
                 character.tick()
             self._active_chars = [character for character in self._active_chars if character.is_active]
             return self._terminal.get_formatted_output_string()
         else:
             raise StopIteration
 
 
 class Expand(BaseEffect[ExpandConfig]):
-    """Effect that draws the characters expanding from a single point."""
+    """Characters expand from the center.
+
+    Attributes:
+        effect_config (ExpandConfig): Configuration for the effect.
+        terminal_config (TerminalConfig): Configuration for the terminal.
+
+    """
 
     _config_cls = ExpandConfig
     _iterator_cls = ExpandIterator
 
     def __init__(self, input_data: str) -> None:
+        """Initialize the effect with the provided input data.
+
+        Args:
+            input_data (str): The input data to use for the effect."""
         super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_fireworks.py` & `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_fireworks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,22 @@
+"""Launches characters up the screen where they explode like fireworks and fall into place.
+
+Classes:
+    Fireworks: Characters explode like fireworks and fall into place.
+    FireworksConfig: Configuration for the Fireworks effect.
+    FireworksIterator: Iterates over the effect. Does not normally need to be called directly.
+"""
+
 import random
 import typing
 from dataclasses import dataclass
 
-from terminaltexteffects.base_character import EffectCharacter, EventHandler
-from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
-from terminaltexteffects.utils import arg_validators, easing, geometry, graphics
+from terminaltexteffects.engine.base_character import EffectCharacter, EventHandler
+from terminaltexteffects.engine.base_effect import BaseEffect, BaseEffectIterator
+from terminaltexteffects.utils import argvalidators, easing, geometry, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 from terminaltexteffects.utils.geometry import Coord
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
     return Fireworks, FireworksConfig
 
@@ -23,112 +31,110 @@
 class FireworksConfig(ArgsDataClass):
     """Configuration for the Fireworks effect.
 
     Attributes:
         explode_anywhere (bool): If set, fireworks explode anywhere in the output area. Otherwise, fireworks explode above highest settled row of text.
         firework_colors (tuple[graphics.Color, ...]): Tuple of colors from which firework colors will be randomly selected.
         firework_symbol (str): Symbol to use for the firework shell.
-        firework_volume (float): Percent of total characters in each firework shell.
-        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
-        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
-        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
-        launch_delay (int): Number of animation steps to wait between launching each firework shell. +/- 0-50 percent randomness is applied to this value.
-        explode_distance (float): Maximum distance from the firework shell origin to the explode waypoint as a percentage of the total output area width."""
+        firework_volume (float): Percent of total characters in each firework shell. Valid values are 0 < n <= 1.
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation. Valid values are n > 0.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the final gradient.
+        launch_delay (int): Number of frames to wait between launching each firework shell. +/- 0-50 percent randomness is applied to this value. Valid values are n >= 0.
+        explode_distance (float): Maximum distance from the firework shell origin to the explode waypoint as a percentage of the total output area width. Valid values are 0 < n <= 1."""
 
     explode_anywhere: bool = ArgField(
         cmd_name="--explode-anywhere",
         action="store_true",
         default=False,
         help="If set, fireworks explode anywhere in the output area. Otherwise, fireworks explode above highest settled row of text.",
     )  # type: ignore[assignment]
     "bool : If set, fireworks explode anywhere in the output area. Otherwise, fireworks explode above highest settled row of text."
 
     firework_colors: tuple[graphics.Color, ...] = ArgField(
         cmd_name="--firework-colors",
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("88F7E2", "44D492", "F5EB67", "FFA15C", "FA233E"),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated list of colors from which firework colors will be randomly selected.",
     )  # type: ignore[assignment]
     "tuple[graphics.Color, ...] : Tuple of colors from which firework colors will be randomly selected."
 
     firework_symbol: str = ArgField(
         cmd_name="--firework-symbol",
-        type_parser=arg_validators.Symbol.type_parser,
+        type_parser=argvalidators.Symbol.type_parser,
         default="o",
-        metavar=arg_validators.Symbol.METAVAR,
+        metavar=argvalidators.Symbol.METAVAR,
         help="Symbol to use for the firework shell.",
     )  # type: ignore[assignment]
     "str : Symbol to use for the firework shell."
 
     firework_volume: float = ArgField(
         cmd_name="--firework-volume",
-        type_parser=arg_validators.Ratio.type_parser,
+        type_parser=argvalidators.Ratio.type_parser,
         default=0.02,
-        metavar=arg_validators.Ratio.METAVAR,
+        metavar=argvalidators.Ratio.METAVAR,
         help="Percent of total characters in each firework shell.",
     )  # type: ignore[assignment]
     "float : Percent of total characters in each firework shell."
 
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name="--final-gradient-stops",
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("8A008A", "00D1FF", "FFFFFF"),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
-    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+    "tuple[graphics.Color, ...] : Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color."
 
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name="--final-gradient-steps",
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
     "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
 
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
-        type_parser=arg_validators.GradientDirection.type_parser,
+        type_parser=argvalidators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.HORIZONTAL,
-        metavar=arg_validators.GradientDirection.METAVAR,
-        help="Direction of the gradient for the final color.",
+        metavar=argvalidators.GradientDirection.METAVAR,
+        help="Direction of the final gradient.",
     )  # type: ignore[assignment]
-    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+    "graphics.Gradient.Direction : Direction of the final gradient."
 
     launch_delay: int = ArgField(
         cmd_name="--launch-delay",
-        type_parser=arg_validators.NonNegativeInt.type_parser,
+        type_parser=argvalidators.NonNegativeInt.type_parser,
         default=60,
-        metavar=arg_validators.NonNegativeInt.METAVAR,
-        help="Number of animation steps to wait between launching each firework shell. +/- 0-50 percent randomness is applied to this value.",
+        metavar=argvalidators.NonNegativeInt.METAVAR,
+        help="Number of frames to wait between launching each firework shell. +/- 0-50 percent randomness is applied to this value.",
     )  # type: ignore[assignment]
-    "int : Number of animation steps to wait between launching each firework shell. +/- 0-50 percent randomness is applied to this value."
+    "int : Number of frames to wait between launching each firework shell. +/- 0-50 percent randomness is applied to this value."
 
     explode_distance: float = ArgField(
         cmd_name="--explode-distance",
         default=0.1,
-        type_parser=arg_validators.Ratio.type_parser,
-        metavar=arg_validators.Ratio.METAVAR,
+        type_parser=argvalidators.Ratio.type_parser,
+        metavar=argvalidators.Ratio.METAVAR,
         help="Maximum distance from the firework shell origin to the explode waypoint as a percentage of the total output area width.",
     )  # type: ignore[assignment]
     "float : Maximum distance from the firework shell origin to the explode waypoint as a percentage of the total output area width."
 
     @classmethod
     def get_effect_class(cls):
         return Fireworks
 
 
 class FireworksIterator(BaseEffectIterator[FireworksConfig]):
-    """Effect that launches characters up the screen where they explode like fireworks and fall into place."""
-
     def __init__(self, effect: "Fireworks"):
         super().__init__(effect)
         self._pending_chars: list[EffectCharacter] = []
         self._active_chars: list[EffectCharacter] = []
         self._shells: list[list[EffectCharacter]] = []
         self._firework_volume = max(1, round(self._config.firework_volume * len(self._terminal._input_characters)))
         self._explode_distance = max(1, round(self._terminal.output_area.right * self._config.explode_distance))
@@ -221,15 +227,14 @@
                     EventHandler.Event.PATH_ACTIVATED,
                     character.motion.query_path("input_pth"),
                     EventHandler.Action.ACTIVATE_SCENE,
                     fall_scn,
                 )
 
     def _build(self) -> None:
-        """Prepares the data for the effect by building the firework shells and scenes."""
         self.prepare_waypoints()
         self.prepare_scenes()
 
     def __next__(self) -> str:
         if self._shells or self._active_chars:
             if self._shells and self._launch_delay == 0:
                 next_group = self._shells.pop()
@@ -245,14 +250,24 @@
             return next_frame
 
         else:
             raise StopIteration
 
 
 class Fireworks(BaseEffect[FireworksConfig]):
-    """Effect that launches characters up the screen where they explode like fireworks and fall into place."""
+    """Launches characters up the screen where they explode like fireworks and fall into place.
+
+    Attributes:
+        effect_config (FireworksConfig): Configuration for the effect.
+        terminal_config (TerminalConfig): Configuration for the terminal.
+
+    """
 
     _config_cls = FireworksConfig
     _iterator_cls = FireworksIterator
 
     def __init__(self, input_data: str):
+        """Initialize the effect with the provided input data.
+
+        Args:
+            input_data (str): The input data to use for the effect."""
         super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_middleout.py` & `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_middleout.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,117 +1,129 @@
+"""Text expands in a single row or column in the middle of the output area then out.
+
+Classes:
+    MiddleOut: Text expands in a single row or column in the middle of the output area then out.
+    MiddleOutConfig: Configuration for the Middleout effect.
+    MiddleOutIterator: Iterates over the effect's frames. Does not normally need to be called directly.
+
+"""
+
 import typing
 from dataclasses import dataclass
 
-import terminaltexteffects.utils.arg_validators as arg_validators
-from terminaltexteffects.base_character import EffectCharacter
-from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
+import terminaltexteffects.utils.argvalidators as argvalidators
+from terminaltexteffects.engine.base_character import EffectCharacter
+from terminaltexteffects.engine.base_effect import BaseEffect, BaseEffectIterator
 from terminaltexteffects.utils import easing, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 from terminaltexteffects.utils.geometry import Coord
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
     return MiddleOut, MiddleOutConfig
 
 
 @argclass(
     name="middleout",
     help="Text expands in a single row or column in the middle of the output area then out.",
     description="middleout | Text expands in a single row or column in the middle of the output area then out.",
-    epilog=f"""{arg_validators.EASING_EPILOG}
+    epilog=f"""{argvalidators.EASING_EPILOG}
 Example: terminaltexteffects middleout --starting-color 8A008A --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --expand-direction vertical --center-movement-speed 0.35 --full-movement-speed 0.35 --center-easing IN_OUT_SINE --full-easing IN_OUT_SINE""",
 )
 @dataclass
 class MiddleOutConfig(ArgsDataClass):
     """Configuration for the Middleout effect.
 
     Attributes:
         starting_color (graphics.Color): Color for the initial text in the center of the output area.
-        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
-        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
-        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
-        expand_direction (str): Direction the text will expand.
-        center_movement_speed (float): Speed of the characters during the initial expansion of the center vertical/horiztonal"""
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation. Valid values are n > 0.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the final gradient.
+        expand_direction (typing.Literal["vertical", "horizontal"]): Direction the text will expand. Choices: vertical, horizontal.
+        center_movement_speed (float): Speed of the characters during the initial expansion of the center vertical/horiztonal. Valid values are n > 0.
+        full_movement_speed (float): Speed of the characters during the final full expansion. Valid values are n > 0.
+        center_easing (easing.EasingFunction): Easing function to use for initial expansion.
+        full_easing (easing.EasingFunction): Easing function to use for full expansion."""
 
     starting_color: graphics.Color = ArgField(
         cmd_name="--starting-color",
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         default="ffffff",
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Color for the initial text in the center of the output area.",
     )  # type: ignore[assignment]
     "graphics.Color : Color for the initial text in the center of the output area."
 
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name="--final-gradient-stops",
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("8A008A", "00D1FF", "FFFFFF"),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
-    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+    "tuple[graphics.Color, ...] : Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color."
 
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name="--final-gradient-steps",
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
     "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
 
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
-        type_parser=arg_validators.GradientDirection.type_parser,
+        type_parser=argvalidators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.VERTICAL,
-        metavar=arg_validators.GradientDirection.METAVAR,
-        help="Direction of the gradient for the final color.",
+        metavar=argvalidators.GradientDirection.METAVAR,
+        help="Direction of the final gradient.",
     )  # type: ignore[assignment]
-    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+    "graphics.Gradient.Direction : Direction of the final gradient."
 
-    expand_direction: str = ArgField(
+    expand_direction: typing.Literal["vertical", "horizontal"] = ArgField(
         cmd_name="--expand-direction",
         default="vertical",
         choices=["vertical", "horizontal"],
         help="Direction the text will expand.",
     )  # type: ignore[assignment]
     "str : Direction the text will expand."
 
     center_movement_speed: float = ArgField(
         cmd_name="--center-movement-speed",
-        type_parser=arg_validators.PositiveFloat.type_parser,
+        type_parser=argvalidators.PositiveFloat.type_parser,
         default=0.35,
-        metavar=arg_validators.PositiveFloat.METAVAR,
-        help="Speed of the characters during the initial expansion of the center vertical/horiztonal line. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.",
+        metavar=argvalidators.PositiveFloat.METAVAR,
+        help="Speed of the characters during the initial expansion of the center vertical/horiztonal line. ",
     )  # type: ignore[assignment]
-    "float : Speed of the characters during the initial expansion of the center vertical/horiztonal line. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect."
+    "float : Speed of the characters during the initial expansion of the center vertical/horiztonal line. "
 
     full_movement_speed: float = ArgField(
         cmd_name="--full-movement-speed",
-        type_parser=arg_validators.PositiveFloat.type_parser,
+        type_parser=argvalidators.PositiveFloat.type_parser,
         default=0.35,
-        metavar=arg_validators.PositiveFloat.METAVAR,
-        help="Speed of the characters during the final full expansion. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.",
+        metavar=argvalidators.PositiveFloat.METAVAR,
+        help="Speed of the characters during the final full expansion. ",
     )  # type: ignore[assignment]
-    "float : Speed of the characters during the final full expansion. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect."
+    "float : Speed of the characters during the final full expansion. "
 
     center_easing: easing.EasingFunction = ArgField(
         cmd_name="--center-easing",
         default=easing.in_out_sine,
-        type_parser=arg_validators.Ease.type_parser,
+        type_parser=argvalidators.Ease.type_parser,
         help="Easing function to use for initial expansion.",
     )  # type: ignore[assignment]
     "easing.EasingFunction : Easing function to use for initial expansion."
 
     full_easing: easing.EasingFunction = ArgField(
         cmd_name="--full-easing",
         default=easing.in_out_sine,
-        type_parser=arg_validators.Ease.type_parser,
+        type_parser=argvalidators.Ease.type_parser,
         help="Easing function to use for full expansion.",
     )  # type: ignore[assignment]
     "easing.EasingFunction : Easing function to use for full expansion."
 
     @classmethod
     def get_effect_class(cls):
         return MiddleOut
@@ -179,14 +191,23 @@
                 self._active_chars = [character for character in self._active_chars if character.is_active]
             return self._terminal.get_formatted_output_string()
         else:
             raise StopIteration
 
 
 class MiddleOut(BaseEffect[MiddleOutConfig]):
-    """Text expands in a single row or column in the middle of the output area then out."""
+    """Text expands in a single row or column in the middle of the output area then out.
+
+    Attributes:
+        effect_config (MiddleOutConfig): Configuration for the effect.
+        terminal_config (TerminalConfig): Configuration for the terminal.
+    """
 
     _config_cls = MiddleOutConfig
     _iterator_cls = MiddleOutIterator
 
     def __init__(self, input_data: str) -> None:
+        """Initialize the effect with the provided input data.
+
+        Args:
+            input_data (str): The input data to use for the effect."""
         super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_orbittingvolley.py` & `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_orbittingvolley.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,156 +1,164 @@
+"""Four launchers orbit the output area firing volleys of characters inward to build the input text from the center out.
+
+Classes:
+    OrbittingVolley: Four launchers orbit the output area firing volleys of characters inward to build the input text from the center out.
+    OrbittingVolleyConfig: Configuration for the OrbittingVolley effect.
+    OrbittingVolleyIterator: Effect iterator for OrbittingVolley. Does not normally need to be called directly.
+"""
+
 import typing
 from dataclasses import dataclass
 from itertools import cycle
 
-import terminaltexteffects.utils.arg_validators as arg_validators
-from terminaltexteffects.base_character import EffectCharacter
-from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
+import terminaltexteffects.utils.argvalidators as argvalidators
+from terminaltexteffects.engine.base_character import EffectCharacter
+from terminaltexteffects.engine.base_effect import BaseEffect, BaseEffectIterator
+from terminaltexteffects.engine.terminal import Terminal
 from terminaltexteffects.utils import easing, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 from terminaltexteffects.utils.geometry import Coord
-from terminaltexteffects.utils.terminal import Terminal
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
     return OrbittingVolley, OrbittingVolleyConfig
 
 
 @argclass(
     name="orbittingvolley",
     help="Four launchers orbit the output area firing volleys of characters inward to build the input text from the center out.",
     description="orbittingvolley | Four launchers orbit the output area firing volleys of characters inward to build the input text from the center out.",
-    epilog=f"""{arg_validators.EASING_EPILOG}
+    epilog=f"""{argvalidators.EASING_EPILOG}
     
 Example: terminaltexteffects orbittingvolley --top-launcher-symbol █ --right-launcher-symbol █ --bottom-launcher-symbol █ --left-launcher-symbol █ --final-gradient-stops FFA15C 44D492 --final-gradient-steps 12 --launcher-movement-speed 0.5 --character-movement-speed 1 --volley-size 0.03 --launch-delay 50 --character-easing OUT_SINE""",
 )
 @dataclass
 class OrbittingVolleyConfig(ArgsDataClass):
     """Configuration for the OrbittingVolley effect.
 
     Attributes:
         top_launcher_symbol (str): Symbol for the top launcher.
         right_launcher_symbol (str): Symbol for the right launcher.
         bottom_launcher_symbol (str): Symbol for the bottom launcher.
         left_launcher_symbol (str): Symbol for the left launcher.
-        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
-        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
-        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
-        launcher_movement_speed (float): Orbitting speed of the launchers.
-        character_movement_speed (float): Speed of the launched characters.
-        volley_size (float): Percent of total input characters each launcher will fire per volley. Lower limit of one character.
-        launch_delay (int): Number of animation ticks to wait between volleys of characters.
-        character_easing (typing.Callable): Easing function to use for launched character movement."""
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation. Valid values are n > 0.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the final gradient.
+        launcher_movement_speed (float): Orbitting speed of the launchers. Valid values are n > 0.
+        character_movement_speed (float): Speed of the launched characters. Valid values are n > 0.
+        volley_size (float): Percent of total input characters each launcher will fire per volley. Lower limit of one character. Valid values are 0 < n <= 1.
+        launch_delay (int): Number of animation ticks to wait between volleys of characters. Valid values are n >= 0.
+        character_easing (easing.EasingFunction): Easing function to use for launched character movement."""
 
     top_launcher_symbol: str = ArgField(
         cmd_name="--top-launcher-symbol",
-        type_parser=arg_validators.Symbol.type_parser,
+        type_parser=argvalidators.Symbol.type_parser,
         default="█",
-        metavar=arg_validators.Symbol.METAVAR,
+        metavar=argvalidators.Symbol.METAVAR,
         help="Symbol for the top launcher.",
     )  # type: ignore[assignment]
     "str : Symbol for the top launcher."
 
     right_launcher_symbol: str = ArgField(
         cmd_name="--right-launcher-symbol",
-        type_parser=arg_validators.Symbol.type_parser,
+        type_parser=argvalidators.Symbol.type_parser,
         default="█",
-        metavar=arg_validators.Symbol.METAVAR,
+        metavar=argvalidators.Symbol.METAVAR,
         help="Symbol for the right launcher.",
     )  # type: ignore[assignment]
     "str : Symbol for the right launcher."
 
     bottom_launcher_symbol: str = ArgField(
         cmd_name="--bottom-launcher-symbol",
-        type_parser=arg_validators.Symbol.type_parser,
+        type_parser=argvalidators.Symbol.type_parser,
         default="█",
-        metavar=arg_validators.Symbol.METAVAR,
+        metavar=argvalidators.Symbol.METAVAR,
         help="Symbol for the bottom launcher.",
     )  # type: ignore[assignment]
     "str : Symbol for the bottom launcher."
 
     left_launcher_symbol: str = ArgField(
         cmd_name="--left-launcher-symbol",
-        type_parser=arg_validators.Symbol.type_parser,
+        type_parser=argvalidators.Symbol.type_parser,
         default="█",
-        metavar=arg_validators.Symbol.METAVAR,
+        metavar=argvalidators.Symbol.METAVAR,
         help="Symbol for the left launcher.",
     )  # type: ignore[assignment]
     "str : Symbol for the left launcher."
 
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name="--final-gradient-stops",
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("FFA15C", "44D492"),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
-    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+    "tuple[graphics.Color, ...] : Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color."
 
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name="--final-gradient-steps",
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
     "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
 
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
-        type_parser=arg_validators.GradientDirection.type_parser,
+        type_parser=argvalidators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.CENTER,
-        metavar=arg_validators.GradientDirection.METAVAR,
-        help="Direction of the gradient for the final color.",
+        metavar=argvalidators.GradientDirection.METAVAR,
+        help="Direction of the final gradient.",
     )  # type: ignore[assignment]
-    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+    "graphics.Gradient.Direction : Direction of the final gradient."
 
     launcher_movement_speed: float = ArgField(
         cmd_name="--launcher-movement-speed",
-        type_parser=arg_validators.PositiveFloat.type_parser,
+        type_parser=argvalidators.PositiveFloat.type_parser,
         default=0.5,
-        metavar=arg_validators.PositiveFloat.METAVAR,
+        metavar=argvalidators.PositiveFloat.METAVAR,
         help="Orbitting speed of the launchers.",
     )  # type: ignore[assignment]
     "float : Orbitting speed of the launchers."
 
     character_movement_speed: float = ArgField(
         cmd_name="--character-movement-speed",
-        type_parser=arg_validators.PositiveFloat.type_parser,
+        type_parser=argvalidators.PositiveFloat.type_parser,
         default=1,
-        metavar=arg_validators.PositiveFloat.METAVAR,
+        metavar=argvalidators.PositiveFloat.METAVAR,
         help="Speed of the launched characters.",
     )  # type: ignore[assignment]
     "float : Speed of the launched characters."
 
     volley_size: float = ArgField(
         cmd_name="--volley-size",
-        type_parser=arg_validators.Ratio.type_parser,
+        type_parser=argvalidators.Ratio.type_parser,
         default=0.03,
-        metavar=arg_validators.Ratio.METAVAR,
+        metavar=argvalidators.Ratio.METAVAR,
         help="Percent of total input characters each launcher will fire per volley. Lower limit of one character.",
     )  # type: ignore[assignment]
     "float : Percent of total input characters each launcher will fire per volley. Lower limit of one character."
 
     launch_delay: int = ArgField(
         cmd_name="--launch-delay",
-        type_parser=arg_validators.NonNegativeInt.type_parser,
+        type_parser=argvalidators.NonNegativeInt.type_parser,
         default=50,
-        metavar=arg_validators.NonNegativeInt.METAVAR,
+        metavar=argvalidators.NonNegativeInt.METAVAR,
         help="Number of animation ticks to wait between volleys of characters.",
     )  # type: ignore[assignment]
     "int : Number of animation ticks to wait between volleys of characters."
 
     character_easing: easing.EasingFunction = ArgField(
         cmd_name=["--character-easing"],
         default=easing.out_sine,
-        type_parser=arg_validators.Ease.type_parser,
-        metavar=arg_validators.Ease.METAVAR,
+        type_parser=argvalidators.Ease.type_parser,
+        metavar=argvalidators.Ease.METAVAR,
         help="Easing function to use for launched character movement.",
     )  # type: ignore[assignment]
     "easing.EasingFunction : Easing function to use for launched character movement."
 
     @classmethod
     def get_effect_class(cls):
         return OrbittingVolley
@@ -249,15 +257,14 @@
         for char_list in self._terminal.get_characters_grouped(Terminal.CharacterGroup.CENTER_TO_OUTSIDE_DIAMONDS):
             self._sorted_chars.extend(char_list)
         for launcher, character in zip(cycle(self._launchers), self._sorted_chars):
             launcher.magazine.append(character)
         self._delay = 0
 
     def _set_launcher_coordinates(self, parent: _Launcher, child: _Launcher) -> None:
-        """Sets the coordinates for the child launcher."""
         parent_progress = parent.character.motion.current_coord.column / self._terminal.output_area.right
         if child.character.input_coord == Coord(self._terminal.output_area.right, self._terminal.output_area.top):
             child_row = self._terminal.output_area.top - int((self._terminal.output_area.top * parent_progress))
             child.character.motion.set_coordinate(Coord(self._terminal.output_area.right, max(1, child_row)))
         elif child.character.input_coord == Coord(self._terminal.output_area.right, self._terminal.output_area.bottom):
             child_column = self._terminal.output_area.right - int((self._terminal.output_area.right * parent_progress))
             child.character.motion.set_coordinate(Coord(max(1, child_column), self._terminal.output_area.bottom))
@@ -307,14 +314,23 @@
                     self._terminal.set_character_visibility(launcher.character, False)
                 return self._terminal.get_formatted_output_string()
             else:
                 raise StopIteration
 
 
 class OrbittingVolley(BaseEffect[OrbittingVolleyConfig]):
-    """Four launchers orbit the output area firing volleys of characters inward to build the input text from the center out."""
+    """Four launchers orbit the output area firing volleys of characters inward to build the input text from the center out.
+
+    Attributes:
+        effect_config (OrbittingVolleyConfig): Configuration for the effect.
+        terminal_config (TerminalConfig): Configuration for the terminal.
+    """
 
     _config_cls = OrbittingVolleyConfig
     _iterator_cls = OrbittingVolleyIterator
 
     def __init__(self, input_data: str) -> None:
+        """Initialize the effect with the provided input data.
+
+        Args:
+            input_data (str): The input data to use for the effect."""
         super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_overflow.py` & `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_overflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,26 @@
+"""Input text overflows ands scrolls the terminal in a random order until eventually appearing ordered.
+
+Classes:
+    Overflow: Input text overflows ands scrolls the terminal in a random order until eventually appearing ordered.
+    OverflowConfig: Configuration for the Overflow effect.
+    OverflowIterator: Iterates over the effect. Does not normally need to be called directly.
+"""
+
 import random
 import typing
 from dataclasses import dataclass
 
-import terminaltexteffects.utils.arg_validators as arg_validators
-from terminaltexteffects.base_character import EffectCharacter
-from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
+import terminaltexteffects.utils.argvalidators as argvalidators
+from terminaltexteffects.engine.base_character import EffectCharacter
+from terminaltexteffects.engine.base_effect import BaseEffect, BaseEffectIterator
+from terminaltexteffects.engine.terminal import Terminal
 from terminaltexteffects.utils import graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 from terminaltexteffects.utils.geometry import Coord
-from terminaltexteffects.utils.terminal import Terminal
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
     return Overflow, OverflowConfig
 
 
 @argclass(
@@ -22,74 +30,74 @@
     epilog="""Example: terminaltexteffects overflow --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --overflow-gradient-stops f2ebc0 8dbfb3 f2ebc0 --overflow-cycles-range 2-4 --overflow-speed 3""",
 )
 @dataclass
 class OverflowConfig(ArgsDataClass):
     """Configuration for the Overflow effect.
 
     Attributes:
-        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
-        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
-        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation. Valid values are n > 0.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the final gradient.
         overflow_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the overflow gradient.
-        overflow_cycles_range (tuple[int, int]): Lower and upper range of the number of cycles to overflow the text.
-        overflow_speed (int): Speed of the overflow effect."""
+        overflow_cycles_range (tuple[int, int]): Lower and upper range of the number of cycles to overflow the text. Valid values are n >= 0.
+        overflow_speed (int): Speed of the overflow effect. Valid values are n > 0."""
 
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("8A008A", "00D1FF", "FFFFFF"),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
-    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+    "tuple[graphics.Color, ...] : Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color."
 
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name=["--final-gradient-steps"],
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
     "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
 
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
-        type_parser=arg_validators.GradientDirection.type_parser,
+        type_parser=argvalidators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.VERTICAL,
-        metavar=arg_validators.GradientDirection.METAVAR,
-        help="Direction of the gradient for the final color.",
+        metavar=argvalidators.GradientDirection.METAVAR,
+        help="Direction of the final gradient.",
     )  # type: ignore[assignment]
-    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+    "graphics.Gradient.Direction : Direction of the final gradient."
 
     overflow_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--overflow-gradient-stops"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("f2ebc0", "8dbfb3", "f2ebc0"),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the overflow gradient.",
     )  # type: ignore[assignment]
     "tuple[graphics.Color, ...] : Tuple of colors for the overflow gradient."
 
     overflow_cycles_range: tuple[int, int] = ArgField(
         cmd_name=["--overflow-cycles-range"],
-        type_parser=arg_validators.IntRange.type_parser,
+        type_parser=argvalidators.IntRange.type_parser,
         default=(2, 4),
-        metavar=arg_validators.IntRange.METAVAR,
+        metavar=argvalidators.IntRange.METAVAR,
         help="Number of cycles to overflow the text.",
     )  # type: ignore[assignment]
     "tuple[int, int] : Lower and upper range of the number of cycles to overflow the text."
 
     overflow_speed: int = ArgField(
         cmd_name=["--overflow-speed"],
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         default=3,
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Speed of the overflow effect.",
     )  # type: ignore[assignment]
     "int : Speed of the overflow effect."
 
     @classmethod
     def get_effect_class(cls):
         return Overflow
@@ -196,14 +204,23 @@
             self._active_chars = [character for character in self._active_chars if character.is_active]
             return next_frame
         else:
             raise StopIteration
 
 
 class Overflow(BaseEffect[OverflowConfig]):
-    """Input text overflows ands scrolls the terminal in a random order until eventually appearing ordered."""
+    """Input text overflows ands scrolls the terminal in a random order until eventually appearing ordered.
+
+    Attributes:
+        effect_config (OverflowConfig): Configuration for the effect.
+        terminal_config (TerminalConfig): Configuration for the terminal.
+    """
 
     _config_cls = OverflowConfig
     _iterator_cls = OverflowIterator
 
     def __init__(self, input_data: str) -> None:
+        """Initialize the effect with the provided input data.
+
+        Args:
+            input_data (str): The input data to use for the effect."""
         super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_pour.py` & `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_pour.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,190 +1,195 @@
-"""Effect that pours the characters into position from the top, bottom, left, or right."""
+"""Pours the characters back and forth from the top, bottom, left, or right.
+
+Classes:
+    Pour: Pours the characters back and forth from the top, bottom, left, or right.
+    PourConfig: Configuration for the Pour effect.
+    PourIterator: Iterates over the frames of the Pour effect. Does not normally need to be called directly.
+"""
 
 import typing
 from dataclasses import dataclass
 from enum import Enum, auto
 
-import terminaltexteffects.utils.arg_validators as arg_validators
-from terminaltexteffects.base_character import EffectCharacter
-from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
+import terminaltexteffects.utils.argvalidators as argvalidators
+from terminaltexteffects.engine.base_character import EffectCharacter
+from terminaltexteffects.engine.base_effect import BaseEffect, BaseEffectIterator
+from terminaltexteffects.engine.terminal import Terminal
 from terminaltexteffects.utils import easing, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 from terminaltexteffects.utils.geometry import Coord
-from terminaltexteffects.utils.terminal import Terminal
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
     return Pour, PourConfig
 
 
 @argclass(
     name="pour",
     help="Pours the characters into position from the given direction.",
     description="pour | Pours the characters into position from the given direction.",
-    epilog=f"""{arg_validators.EASING_EPILOG}
+    epilog=f"""{argvalidators.EASING_EPILOG}
 Example: terminaltexteffects pour --pour-direction down --movement-speed 0.2 --gap 1 --starting-color FFFFFF --final-gradient-stops 8A008A 00D1FF FFFFFF --easing IN_QUAD""",
 )
 @dataclass
 class PourConfig(ArgsDataClass):
     """Configuration for the Pour effect.
 
     Attributes:
-        pour_direction (str): Direction the text will pour.
-        pour_speed (int): Number of characters poured in per tick. Increase to speed up the effect.
-        movement_speed (float): Movement speed of the characters. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.
-        gap (int): Number of frames to wait between each character in the pour effect. Increase to slow down effect and create a more defined back and forth motion.
+        pour_direction (str): Direction the text will pour. Valid values are "up", "down", "left", and "right".
+        pour_speed (int): Number of characters poured in per tick. Increase to speed up the effect. Valid values are n > 0.
+        movement_speed (float): Movement speed of the characters. Valid values are n > 0.
+        gap (int): Number of frames to wait between each character in the pour effect. Increase to slow down effect and create a more defined back and forth motion. Valid values are n >= 0.
         starting_color (graphics.Color): Color of the characters before the gradient starts.
         final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient. If only one color is provided, the characters will be displayed in that color.
         final_gradient_steps (tuple[int, ...]): Number of gradient steps to use. More steps will create a smoother and longer gradient animation.
         final_gradient_frames (int): Number of frames to display each gradient step.
-        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
-        easing (typing.Callable): Easing function to use for character movement."""
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the final gradient.
+        easing (easing.EasingFunction): Easing function to use for character movement."""
 
-    pour_direction: str = ArgField(
+    pour_direction: typing.Literal["up", "down", "left", "right"] = ArgField(
         cmd_name=["--pour-direction"],
         default="down",
         choices=["up", "down", "left", "right"],
         help="Direction the text will pour.",
     )  # type: ignore[assignment]
-    "str : Direction the text will pour."
+    "typing.Literal['up', 'down', 'left', 'right'] : Direction the text will pour."
 
     pour_speed: int = ArgField(
         cmd_name="--pour-speed",
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         default=1,
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Number of characters poured in per tick. Increase to speed up the effect.",
     )  # type: ignore[assignment]
     "int : Number of characters poured in per tick. Increase to speed up the effect."
 
     movement_speed: float = ArgField(
         cmd_name="--movement-speed",
-        type_parser=arg_validators.PositiveFloat.type_parser,
+        type_parser=argvalidators.PositiveFloat.type_parser,
         default=0.2,
-        metavar=arg_validators.PositiveFloat.METAVAR,
-        help="Movement speed of the characters. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.",
+        metavar=argvalidators.PositiveFloat.METAVAR,
+        help="Movement speed of the characters. ",
     )  # type: ignore[assignment]
     "float : Movement speed of the characters."
 
     gap: int = ArgField(
         cmd_name="--gap",
-        type_parser=arg_validators.NonNegativeInt.type_parser,
+        type_parser=argvalidators.NonNegativeInt.type_parser,
         default=1,
-        metavar=arg_validators.NonNegativeInt.METAVAR,
+        metavar=argvalidators.NonNegativeInt.METAVAR,
         help="Number of frames to wait between each character in the pour effect. Increase to slow down effect and create a more defined back and forth motion.",
     )  # type: ignore[assignment]
     "int : Number of frames to wait between each character in the pour effect."
 
     starting_color: graphics.Color = ArgField(
         cmd_name=["--starting-color"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         default="ffffff",
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Color of the characters before the gradient starts.",
     )  # type: ignore[assignment]
     "graphics.Color : Color of the characters before the gradient starts."
 
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("8A008A", "00D1FF", "FFFFFF"),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient. If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
     "tuple[graphics.Color, ...] : Tuple of colors for the character gradient."
 
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name=["--final-gradient-steps"],
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         default=(12,),
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
     "tuple[int, ...] : Tuple of the number of gradient steps to use."
 
     final_gradient_frames: int = ArgField(
         cmd_name=["--final-gradient-frames"],
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         default=10,
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Number of frames to display each gradient step.",
     )  # type: ignore[assignment]
     "int : Number of frames to display each gradient step."
 
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
-        type_parser=arg_validators.GradientDirection.type_parser,
+        type_parser=argvalidators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.VERTICAL,
-        metavar=arg_validators.GradientDirection.METAVAR,
-        help="Direction of the gradient for the final color.",
+        metavar=argvalidators.GradientDirection.METAVAR,
+        help="Direction of the final gradient.",
     )  # type: ignore[assignment]
-    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+    "graphics.Gradient.Direction : Direction of the final gradient."
 
     movement_easing: easing.EasingFunction = ArgField(
         cmd_name="--movement-easing",
         default=easing.in_quad,
-        type_parser=arg_validators.Ease.type_parser,
+        type_parser=argvalidators.Ease.type_parser,
         help="Easing function to use for character movement.",
     )  # type: ignore[assignment]
     "easing.EasingFunction : Easing function to use for character movement."
 
     @classmethod
     def get_effect_class(cls):
         return Pour
 
 
-class PourDirection(Enum):
-    UP = auto()
-    DOWN = auto()
-    LEFT = auto()
-    RIGHT = auto()
-
-
 class PourIterator(BaseEffectIterator[PourConfig]):
+    class PourDirection(Enum):
+        UP = auto()
+        DOWN = auto()
+        LEFT = auto()
+        RIGHT = auto()
+
     def __init__(self, effect: "Pour") -> None:
         super().__init__(effect)
         self._pending_groups: list[list[EffectCharacter]] = []
         self._active_characters: list[EffectCharacter] = []
         self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
         self._build()
 
     def _build(self) -> None:
         self._pour_direction = {
-            "down": PourDirection.DOWN,
-            "up": PourDirection.UP,
-            "left": PourDirection.LEFT,
-            "right": PourDirection.RIGHT,
-        }.get(self._config.pour_direction, PourDirection.DOWN)
+            "down": PourIterator.PourDirection.DOWN,
+            "up": PourIterator.PourDirection.UP,
+            "left": PourIterator.PourDirection.LEFT,
+            "right": PourIterator.PourDirection.RIGHT,
+        }.get(self._config.pour_direction, PourIterator.PourDirection.DOWN)
         final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
             self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
         )
         for character in self._terminal.get_characters():
             self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
         sort_map = {
-            PourDirection.DOWN: Terminal.CharacterGroup.ROW_BOTTOM_TO_TOP,
-            PourDirection.UP: Terminal.CharacterGroup.ROW_TOP_TO_BOTTOM,
-            PourDirection.LEFT: Terminal.CharacterGroup.COLUMN_LEFT_TO_RIGHT,
-            PourDirection.RIGHT: Terminal.CharacterGroup.COLUMN_RIGHT_TO_LEFT,
+            PourIterator.PourDirection.DOWN: Terminal.CharacterGroup.ROW_BOTTOM_TO_TOP,
+            PourIterator.PourDirection.UP: Terminal.CharacterGroup.ROW_TOP_TO_BOTTOM,
+            PourIterator.PourDirection.LEFT: Terminal.CharacterGroup.COLUMN_LEFT_TO_RIGHT,
+            PourIterator.PourDirection.RIGHT: Terminal.CharacterGroup.COLUMN_RIGHT_TO_LEFT,
         }
         groups = self._terminal.get_characters_grouped(grouping=sort_map[self._pour_direction])
         for i, group in enumerate(groups):
             for character in group:
                 self._terminal.set_character_visibility(character, False)
-                if self._pour_direction == PourDirection.DOWN:
+                if self._pour_direction == PourIterator.PourDirection.DOWN:
                     character.motion.set_coordinate(Coord(character.input_coord.column, self._terminal.output_area.top))
-                elif self._pour_direction == PourDirection.UP:
+                elif self._pour_direction == PourIterator.PourDirection.UP:
                     character.motion.set_coordinate(
                         Coord(character.input_coord.column, self._terminal.output_area.bottom)
                     )
-                elif self._pour_direction == PourDirection.LEFT:
+                elif self._pour_direction == PourIterator.PourDirection.LEFT:
                     character.motion.set_coordinate(Coord(self._terminal.output_area.right, character.input_coord.row))
-                elif self._pour_direction == PourDirection.RIGHT:
+                elif self._pour_direction == PourIterator.PourDirection.RIGHT:
                     character.motion.set_coordinate(Coord(self._terminal.output_area.left, character.input_coord.row))
                 input_coord_path = character.motion.new_path(
                     speed=self._config.movement_speed,
                     ease=self._config.movement_easing,
                 )
                 input_coord_path.new_waypoint(character.input_coord)
                 character.motion.activate_path(input_coord_path)
@@ -227,14 +232,23 @@
             self._active_characters = [character for character in self._active_characters if character.is_active]
             return next_frame
         else:
             raise StopIteration
 
 
 class Pour(BaseEffect[PourConfig]):
-    """Effect that pours the characters into position from the top, bottom, left, or right."""
+    """Pours the characters back and forth from the top, bottom, left, or right.
+
+    Attributes:
+        effect_config (PourConfig): Configuration for the effect.
+        terminal_config (TerminalConfig): Configuration for the terminal.
+    """
 
     _config_cls = PourConfig
     _iterator_cls = PourIterator
 
     def __init__(self, input_data: str) -> None:
+        """Initialize the effect with the provided input data.
+
+        Args:
+            input_data (str): The input data to use for the effect."""
         super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_print.py` & `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_print.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,147 +1,154 @@
+"""Prints the input data one line at at time with a carriage return and line feed.
+
+Classes:
+    Print: Prints the input data one line at at time with a carriage return and line feed.
+    PrintConfig: Configuration for the Print effect.
+    PrintIterator: Effect iterator for the Print effect. Does not normally need to be called directly.
+"""
+
 import random
 import typing
 from dataclasses import dataclass
 
-import terminaltexteffects.utils.arg_validators as arg_validators
-from terminaltexteffects.base_character import EffectCharacter, EventHandler
-from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
+import terminaltexteffects.utils.argvalidators as argvalidators
+from terminaltexteffects.engine.base_character import EffectCharacter, EventHandler
+from terminaltexteffects.engine.base_effect import BaseEffect, BaseEffectIterator
 from terminaltexteffects.utils import easing, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 from terminaltexteffects.utils.geometry import Coord
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
     return Print, PrintConfig
 
 
 @argclass(
     name="print",
     help="Lines are printed one at a time following a print head. Print head performs line feed, carriage return.",
     description="print | Lines are printed one at a time following a print head. Print head performs line feed, carriage return.",
-    epilog=f"""{arg_validators.EASING_EPILOG}
+    epilog=f"""{argvalidators.EASING_EPILOG}
     
 Example: terminaltexteffects print --final-gradient-stops 02b8bd c1f0e3 00ffa0 --final-gradient-steps 12 --print-head-return-speed 1.25 --print-speed 1 --print-head-easing IN_OUT_QUAD""",
 )
 @dataclass
 class PrintConfig(ArgsDataClass):
     """Configuration for the Print effect.
 
     Attributes:
-        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
-        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
-        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation. Valid values are n > 0.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the final gradient.
         print_head_return_speed (float): Speed of the print head when performing a carriage return.
         print_speed (int): Speed of the print head when printing characters.
-        print_head_easing (typing.Callable): Easing function to use for print head movement."""
+        print_head_easing (easing.EasingFunction): Easing function to use for print head movement."""
 
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("02b8bd", "c1f0e3", "00ffa0"),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
-    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+    "tuple[graphics.Color, ...] : Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color."
 
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name=["--final-gradient-steps"],
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
     "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
 
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
-        type_parser=arg_validators.GradientDirection.type_parser,
+        type_parser=argvalidators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.DIAGONAL,
-        metavar=arg_validators.GradientDirection.METAVAR,
-        help="Direction of the gradient for the final color.",
+        metavar=argvalidators.GradientDirection.METAVAR,
+        help="Direction of the final gradient.",
     )  # type: ignore[assignment]
-    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+    "graphics.Gradient.Direction : Direction of the final gradient."
 
     print_head_return_speed: float = ArgField(
         cmd_name=["--print-head-return-speed"],
-        type_parser=arg_validators.PositiveFloat.type_parser,
+        type_parser=argvalidators.PositiveFloat.type_parser,
         default=1.25,
-        metavar=arg_validators.PositiveFloat.METAVAR,
+        metavar=argvalidators.PositiveFloat.METAVAR,
         help="Speed of the print head when performing a carriage return.",
     )  # type: ignore[assignment]
     "float : Speed of the print head when performing a carriage return."
 
     print_speed: int = ArgField(
         cmd_name=["--print-speed"],
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         default=1,
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Speed of the print head when printing characters.",
     )  # type: ignore[assignment]
     "int : Speed of the print head when printing characters."
 
     print_head_easing: easing.EasingFunction = ArgField(
         cmd_name=["--print-head-easing"],
         default=easing.in_out_quad,
-        type_parser=arg_validators.Ease.type_parser,
+        type_parser=argvalidators.Ease.type_parser,
         help="Easing function to use for print head movement.",
     )  # type: ignore[assignment]
     "easing.EasingFunction : Easing function to use for print head movement."
 
     @classmethod
     def get_effect_class(cls):
         return Print
 
 
-class _Row:
-    def __init__(
-        self,
-        characters: list[EffectCharacter],
-        character_final_color_map: dict[EffectCharacter, graphics.Color],
-        typing_head_color: str | int,
-    ):
-        self.untyped_chars: list[EffectCharacter] = []
-        self.typed_chars: list[EffectCharacter] = []
-        blank_row_accounted = False
-        for character in characters:
-            if character.input_symbol == " ":
-                if blank_row_accounted:
-                    continue
-                blank_row_accounted = True
-            character.motion.set_coordinate(Coord(character.input_coord.column, 1))
-            color_gradient = graphics.Gradient(typing_head_color, character_final_color_map[character], steps=5)
-            typed_animation = character.animation.new_scene()
-            typed_animation.apply_gradient_to_symbols(color_gradient, ("█", "▓", "▒", "░", character.input_symbol), 5)
-            character.animation.activate_scene(typed_animation)
-            self.untyped_chars.append(character)
-
-    def move_up(self):
-        for character in self.typed_chars:
-            current_row = character.motion.current_coord.row
-            character.motion.set_coordinate(Coord(character.motion.current_coord.column, current_row + 1))
-
-    def type_char(self) -> EffectCharacter | None:
-        if self.untyped_chars:
-            next_char = self.untyped_chars.pop(0)
-            self.typed_chars.append(next_char)
-            return next_char
-        return None
-
-
 class PrintIterator(BaseEffectIterator[PrintConfig]):
-    """Effect that moves a print head across the screen, printing characters, before performing a line feed and carriage return."""
+    class _Row:
+        def __init__(
+            self,
+            characters: list[EffectCharacter],
+            character_final_color_map: dict[EffectCharacter, graphics.Color],
+            typing_head_color: str | int,
+        ):
+            self.untyped_chars: list[EffectCharacter] = []
+            self.typed_chars: list[EffectCharacter] = []
+            blank_row_accounted = False
+            for character in characters:
+                if character.input_symbol == " ":
+                    if blank_row_accounted:
+                        continue
+                    blank_row_accounted = True
+                character.motion.set_coordinate(Coord(character.input_coord.column, 1))
+                color_gradient = graphics.Gradient(typing_head_color, character_final_color_map[character], steps=5)
+                typed_animation = character.animation.new_scene()
+                typed_animation.apply_gradient_to_symbols(
+                    color_gradient, ("█", "▓", "▒", "░", character.input_symbol), 5
+                )
+                character.animation.activate_scene(typed_animation)
+                self.untyped_chars.append(character)
+
+        def move_up(self):
+            for character in self.typed_chars:
+                current_row = character.motion.current_coord.row
+                character.motion.set_coordinate(Coord(character.motion.current_coord.column, current_row + 1))
+
+        def type_char(self) -> EffectCharacter | None:
+            if self.untyped_chars:
+                next_char = self.untyped_chars.pop(0)
+                self.typed_chars.append(next_char)
+                return next_char
+            return None
 
     def __init__(self, effect: "Print"):
         super().__init__(effect)
         self._pending_chars: list[EffectCharacter] = []
         self._active_chars: list[EffectCharacter] = []
-        self._pending_rows: list[_Row] = []
-        self._processed_rows: list[_Row] = []
+        self._pending_rows: list[PrintIterator._Row] = []
+        self._processed_rows: list[PrintIterator._Row] = []
         self._typing_head = self._terminal.add_character("█", Coord(1, 1))
         self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
         self._build()
 
     def _build(self) -> None:
         self.final_gradient = graphics.Gradient(
             *self._config.final_gradient_stops, steps=self._config.final_gradient_steps
@@ -152,21 +159,21 @@
         for character in self._terminal.get_characters(fill_chars=True):
             self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
         input_rows = self._terminal.get_characters_grouped(
             grouping=self._terminal.CharacterGroup.ROW_TOP_TO_BOTTOM, fill_chars=True
         )
         for input_row in input_rows:
             self._pending_rows.append(
-                _Row(
+                PrintIterator._Row(
                     input_row,
                     self._character_final_color_map,
                     self._character_final_color_map[input_row[-1]],
                 )
             )
-        self._current_row: _Row = self._pending_rows.pop(0)
+        self._current_row: PrintIterator._Row = self._pending_rows.pop(0)
         self._typing = True
         self._delay = 0
         self._last_column = 0
 
     def __next__(self) -> str:
         if self._active_chars or self._typing:
             if self._typing_head.motion.active_path:
@@ -221,14 +228,23 @@
             self._active_chars = [character for character in self._active_chars if character.is_active]
             return next_frame
         else:
             raise StopIteration
 
 
 class Print(BaseEffect[PrintConfig]):
-    """Prints the input data in a pouring fashion, one character at a time."""
+    """Prints the input data one line at at time with a carriage return and line feed.
+
+    Attributes:
+        effect_config (PrintConfig): Configuration for the effect.
+        terminal_config (TerminalConfig): Configuration for the terminal
+    """
 
     _config_cls = PrintConfig
     _iterator_cls = PrintIterator
 
     def __init__(self, input_data: str) -> None:
+        """Initialize the effect with the provided input data.
+
+        Args:
+            input_data (str): The input data to use for the effect."""
         super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_rain.py` & `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_wipe.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,185 +1,194 @@
-"""Creates a rain effect where characters fall from the top of the terminal."""
+"""Performs a wipe across the terminal to reveal characters.
+
+Classes:
+    Wipe: Performs a wipe across the terminal to reveal characters.
+    WipeConfig: Configuration for the Wipe effect.
+    WipeIterator: Effect iterator for the Wipe effect. Does not normally need to be called directly.
+"""
 
-import random
 import typing
 from dataclasses import dataclass
 
-import terminaltexteffects.utils.arg_validators as arg_validators
-from terminaltexteffects.base_character import EffectCharacter
-from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
-from terminaltexteffects.utils import easing, graphics
+import terminaltexteffects.utils.argvalidators as argvalidators
+from terminaltexteffects.engine.base_character import EffectCharacter
+from terminaltexteffects.engine.base_effect import BaseEffect, BaseEffectIterator
+from terminaltexteffects.utils import graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
-from terminaltexteffects.utils.geometry import Coord
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
-    return Rain, RainConfig
+    return Wipe, WipeConfig
 
 
 @argclass(
-    name="rain",
-    help="Rain characters from the top of the output area.",
-    description="rain | Rain characters from the top of the output area.",
-    epilog=f"""{arg_validators.EASING_EPILOG} 
-Example: terminaltexteffects rain --rain-symbols o . , "*" "|" --rain-colors 00315C 004C8F 0075DB 3F91D9 78B9F2 9AC8F5 B8D8F8 E3EFFC --final-gradient-stops 488bff b2e7de 57eaf7 --final-gradient-steps 12 --movement-speed 0.1-0.2 --easing IN_QUART""",
+    name="wipe",
+    help="Wipes the text across the terminal to reveal characters.",
+    description="wipe | Wipes the text across the terminal to reveal characters.",
+    epilog="""Example: terminaltexteffects wipe --wipe-direction diagonal_bottom_left_to_top_right --final-gradient-stops 833ab4 fd1d1d fcb045 --final-gradient-steps 12 --final-gradient-frames 5 --wipe-delay 0""",
 )
 @dataclass
-class RainConfig(ArgsDataClass):
-    """Configuration for the Rain effect.
+class WipeConfig(ArgsDataClass):
+    """Configuration for the Wipe effect.
 
     Attributes:
-        rain_colors (tuple[graphics.Color, ...]): Tuple of colors for the rain drops. Colors are randomly chosen from the tuple.
-        movement_speed (tuple[float, float]): Falling speed range of the rain drops.
-        rain_symbols (tuple[str, ...]): Tuple of symbols to use for the rain drops. Symbols are randomly chosen from the tuple.
-        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
-        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
-        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
-        easing (typing.Callable): Easing function to use for character movement."""
-
-    rain_colors: tuple[graphics.Color, ...] = ArgField(
-        cmd_name=["--rain-colors"],
-        type_parser=arg_validators.Color.type_parser,
-        metavar=arg_validators.Color.METAVAR,
-        nargs="+",
-        default=("00315C", "004C8F", "0075DB", "3F91D9", "78B9F2", "9AC8F5", "B8D8F8", "E3EFFC"),
-        help="List of colors for the rain drops. Colors are randomly chosen from the list.",
-    )  # type: ignore[assignment]
-    "tuple[graphics.Color, ...] : Tuple of colors for the rain drops. Colors are randomly chosen from the tuple."
-
-    movement_speed: tuple[float, float] = ArgField(
-        cmd_name="--movement-speed",
-        type_parser=arg_validators.PositiveFloatRange.type_parser,
-        default=(0.1, 0.2),
-        metavar=arg_validators.PositiveFloatRange.METAVAR,
-        help="Falling speed range of the rain drops.",
-    )  # type: ignore[assignment]
-    "tuple[float, float] : Falling speed range of the rain drops."
-
-    rain_symbols: tuple[str, ...] = ArgField(
-        cmd_name="--rain-symbols",
-        type_parser=arg_validators.Symbol.type_parser,
-        nargs="+",
-        default=("o", ".", ",", "*", "|"),
-        metavar=arg_validators.Symbol.METAVAR,
-        help="Space separated list of symbols to use for the rain drops. Symbols are randomly chosen from the list.",
+        wipe_direction (typing.Literal["column_left_to_right","row_top_to_bottom","row_bottom_to_top","diagonal_top_left_to_bottom_right","diagonal_bottom_left_to_top_right","diagonal_top_right_to_bottom_left","diagonal_bottom_right_to_top_left",]): Direction the text will wipe.
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the wipe gradient.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation. Valid values are n > 0.
+        final_gradient_frames (int): Number of frames to display each gradient step.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the final gradient.
+        wipe_delay (int): Number of frames to wait before adding the next character group. Increase, to slow down the effect. Valid values are n >= 0."""
+
+    wipe_direction: typing.Literal[
+        "column_left_to_right",
+        "row_top_to_bottom",
+        "row_bottom_to_top",
+        "diagonal_top_left_to_bottom_right",
+        "diagonal_bottom_left_to_top_right",
+        "diagonal_top_right_to_bottom_left",
+        "diagonal_bottom_right_to_top_left",
+    ] = ArgField(
+        cmd_name="--wipe-direction",
+        default="diagonal_bottom_left_to_top_right",
+        choices=[
+            "column_left_to_right",
+            "column_right_to_left",
+            "row_top_to_bottom",
+            "row_bottom_to_top",
+            "diagonal_top_left_to_bottom_right",
+            "diagonal_bottom_left_to_top_right",
+            "diagonal_top_right_to_bottom_left",
+            "diagonal_bottom_right_to_top_left",
+        ],
+        help="Direction the text will wipe.",
     )  # type: ignore[assignment]
-    "tuple[str, ...] : Tuple of symbols to use for the rain drops. Symbols are randomly chosen from the tuple."
+    "typing.Literal['column_left_to_right','row_top_to_bottom','row_bottom_to_top','diagonal_top_left_to_bottom_right','diagonal_bottom_left_to_top_right','diagonal_top_right_to_bottom_left','diagonal_bottom_right_to_top_left',] : Direction the text will wipe. Options: column_left_to_right, column_right_to_left, row_top_to_bottom, row_bottom_to_top, diagonal_top_left_to_bottom_right, diagonal_bottom_left_to_top_right, diagonal_top_right_to_bottom_left, diagonal_bottom_right_to_top_left."
 
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name="--final-gradient-stops",
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
-        default=("488bff", "b2e7de", "57eaf7"),
-        metavar=arg_validators.Color.METAVAR,
-        help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
+        default=("833ab4", "fd1d1d", "fcb045"),
+        metavar=argvalidators.ColorArg.METAVAR,
+        help="Space separated, unquoted, list of colors for the wipe gradient.",
     )  # type: ignore[assignment]
-    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+    "tuple[graphics.Color, ...] : Tuple of colors for the wipe gradient."
 
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name="--final-gradient-steps",
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
-        metavar=arg_validators.PositiveInt.METAVAR,
-        help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
+        metavar=argvalidators.PositiveInt.METAVAR,
+        help="Number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
     "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
 
+    final_gradient_frames: int = ArgField(
+        cmd_name="--final-gradient-frames",
+        type_parser=argvalidators.PositiveInt.type_parser,
+        default=5,
+        metavar=argvalidators.PositiveInt.METAVAR,
+        help="Number of frames to display each gradient step.",
+    )  # type: ignore[assignment]
+    "int : Number of frames to display each gradient step."
+
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
-        type_parser=arg_validators.GradientDirection.type_parser,
-        default=graphics.Gradient.Direction.DIAGONAL,
-        metavar=arg_validators.GradientDirection.METAVAR,
-        help="Direction of the gradient for the final color.",
-    )  # type: ignore[assignment]
-    "graphics.Gradient.Direction : Direction of the gradient for the final color."
-
-    movement_easing: easing.EasingFunction = ArgField(
-        cmd_name=["--movement-easing"],
-        default=easing.in_quart,
-        type_parser=arg_validators.Ease.type_parser,
-        metavar=arg_validators.Ease.METAVAR,
-        help="Easing function to use for character movement.",
+        type_parser=argvalidators.GradientDirection.type_parser,
+        default=graphics.Gradient.Direction.VERTICAL,
+        metavar=argvalidators.GradientDirection.METAVAR,
+        help="Direction of the final gradient.",
+    )  # type: ignore[assignment]
+    "graphics.Gradient.Direction : Direction of the final gradient."
+
+    wipe_delay: int = ArgField(
+        cmd_name="--wipe-delay",
+        type_parser=argvalidators.NonNegativeInt.type_parser,
+        default=0,
+        metavar=argvalidators.NonNegativeInt.METAVAR,
+        help="Number of frames to wait before adding the next character group. Increase, to slow down the effect.",
     )  # type: ignore[assignment]
-    "easing.EasingFunction : Easing function to use for character movement."
+    "int : Number of frames to wait before adding the next character group. Increase, to slow down the effect."
 
     @classmethod
     def get_effect_class(cls):
-        return Rain
+        return Wipe
 
 
-class RainIterator(BaseEffectIterator[RainConfig]):
-    def __init__(self, effect: "Rain") -> None:
+class WipeIterator(BaseEffectIterator[WipeConfig]):
+    def __init__(self, effect: "Wipe") -> None:
         super().__init__(effect)
-        self._pending_chars: list[EffectCharacter] = []
+        self._pending_groups: list[list[EffectCharacter]] = []
         self._active_chars: list[EffectCharacter] = []
-        self._group_by_row: dict[int, list[EffectCharacter | None]] = {}
         self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
         self._build()
 
     def _build(self) -> None:
-        """Prepares the data for the effect by setting all characters y position to the input height and sorting by target y."""
+        direction = self._config.wipe_direction
         final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
             self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
         )
         for character in self._terminal.get_characters():
             self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
-
-        for character in self._terminal.get_characters():
-            raindrop_color = random.choice(self._config.rain_colors)
-            rain_scn = character.animation.new_scene()
-            rain_scn.add_frame(random.choice(self._config.rain_symbols), 1, color=raindrop_color)
-            raindrop_gradient = graphics.Gradient(raindrop_color, self._character_final_color_map[character], steps=7)
-            fade_scn = character.animation.new_scene()
-            fade_scn.apply_gradient_to_symbols(raindrop_gradient, character.input_symbol, 5)
-            character.animation.activate_scene(rain_scn)
-            character.motion.set_coordinate(Coord(character.input_coord.column, self._terminal.output_area.top))
-            input_path = character.motion.new_path(
-                speed=random.uniform(self._config.movement_speed[0], self._config.movement_speed[1]),
-                ease=self._config.movement_easing,
-            )
-            input_path.new_waypoint(character.input_coord)
-
-            character.event_handler.register_event(
-                character.event_handler.Event.PATH_COMPLETE,
-                input_path,
-                character.event_handler.Action.ACTIVATE_SCENE,
-                fade_scn,
-            )
-            character.motion.activate_path(input_path)
-            self._pending_chars.append(character)
-        for character in sorted(self._pending_chars, key=lambda c: c.input_coord.row):
-            if character.input_coord.row not in self._group_by_row:
-                self._group_by_row[character.input_coord.row] = []
-            self._group_by_row[character.input_coord.row].append(character)
-        self._pending_chars.clear()
+        sort_map = {
+            "column_left_to_right": self._terminal.CharacterGroup.COLUMN_LEFT_TO_RIGHT,
+            "column_right_to_left": self._terminal.CharacterGroup.COLUMN_RIGHT_TO_LEFT,
+            "row_top_to_bottom": self._terminal.CharacterGroup.ROW_TOP_TO_BOTTOM,
+            "row_bottom_to_top": self._terminal.CharacterGroup.ROW_BOTTOM_TO_TOP,
+            "diagonal_top_left_to_bottom_right": self._terminal.CharacterGroup.DIAGONAL_TOP_LEFT_TO_BOTTOM_RIGHT,
+            "diagonal_bottom_left_to_top_right": self._terminal.CharacterGroup.DIAGONAL_BOTTOM_LEFT_TO_TOP_RIGHT,
+            "diagonal_top_right_to_bottom_left": self._terminal.CharacterGroup.DIAGONAL_TOP_RIGHT_TO_BOTTOM_LEFT,
+            "diagonal_bottom_right_to_top_left": self._terminal.CharacterGroup.DIAGONAL_BOTTOM_RIGHT_TO_TOP_LEFT,
+        }
+        for group in self._terminal.get_characters_grouped(sort_map[direction]):
+            for character in group:
+                wipe_scn = character.animation.new_scene()
+                wipe_gradient = graphics.Gradient(
+                    final_gradient.spectrum[0],
+                    self._character_final_color_map[character],
+                    steps=self._config.final_gradient_steps,
+                )
+                wipe_scn.apply_gradient_to_symbols(
+                    wipe_gradient, character.input_symbol, self._config.final_gradient_frames
+                )
+                character.animation.activate_scene(wipe_scn)
+            self._pending_groups.append(group)
+        self._wipe_delay = self._config.wipe_delay
 
     def __next__(self) -> str:
-        if self._group_by_row or self._active_chars or self._pending_chars:
-            if not self._pending_chars and self._group_by_row:
-                self._pending_chars.extend(self._group_by_row.pop(min(self._group_by_row.keys())))  # type: ignore
-            if self._pending_chars:
-                for _ in range(random.randint(1, 3)):
-                    if self._pending_chars:
-                        next_character = self._pending_chars.pop(random.randint(0, len(self._pending_chars) - 1))
-                        self._terminal.set_character_visibility(next_character, True)
-                        self._active_chars.append(next_character)
-
-                    else:
-                        break
+        if self._pending_groups or self._active_chars:
+            if not self._wipe_delay:
+                if self._pending_groups:
+                    next_group = self._pending_groups.pop(0)
+                    for character in next_group:
+                        self._terminal.set_character_visibility(character, True)
+                        self._active_chars.append(character)
+                self._wipe_delay = self._config.wipe_delay
+            else:
+                self._wipe_delay -= 1
             for character in self._active_chars:
                 character.tick()
-
             self._active_chars = [character for character in self._active_chars if character.is_active]
             return self._terminal.get_formatted_output_string()
         else:
             raise StopIteration
 
 
-class Rain(BaseEffect[RainConfig]):
-    _config_cls = RainConfig
-    _iterator_cls = RainIterator
+class Wipe(BaseEffect[WipeConfig]):
+    """Performs a wipe across the terminal to reveal characters.
+
+    Attributes:
+        effect_config (WipeConfig): Configuration for the effect.
+        terminal_config (TerminalConfig): Configuration for the terminal.
+    """
+
+    _config_cls = WipeConfig
+    _iterator_cls = WipeIterator
 
     def __init__(self, input_data: str) -> None:
+        """Initialize the effect with the provided input data.
+
+        Args:
+            input_data (str): The input data to use for the effect."""
         super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_rings.py` & `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_rings.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,24 @@
+"""Characters are dispersed and form into spinning rings.
+
+Classes:
+    Rings: Characters are dispersed and form into spinning rings.
+    RingsConfig: Configuration for the Rings effect.
+    RingsIterator: Iterates over the effect. Does not normally need to be called directly.
+"""
+
 import random
 import typing
 from dataclasses import dataclass
 
-import terminaltexteffects.utils.arg_validators as arg_validators
-from terminaltexteffects.base_character import EffectCharacter, EventHandler
-from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
-from terminaltexteffects.utils import easing, geometry, graphics, motion
+import terminaltexteffects.utils.argvalidators as argvalidators
+from terminaltexteffects.engine import motion
+from terminaltexteffects.engine.base_character import EffectCharacter, EventHandler
+from terminaltexteffects.engine.base_effect import BaseEffect, BaseEffectIterator
+from terminaltexteffects.utils import easing, geometry, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 from terminaltexteffects.utils.geometry import Coord
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
     return Rings, RingsConfig
 
@@ -22,106 +31,106 @@
 )
 @dataclass
 class RingsConfig(ArgsDataClass):
     """Configurations for the RingsEffect.
 
     Attributes:
         ring_colors (tuple[graphics.Color, ...]): Tuple of colors for the rings.
-        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color.
         final_gradient_steps (tuple[int, ...]): Number of gradient steps to use. More steps will create a smoother and longer gradient animation.
-        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
-        ring_gap (float): Distance between rings as a percent of the smallest output area dimension.
-        spin_duration (int): Number of animation steps for each cycle of the spin phase.
-        spin_speed (tuple[float, float]): Range of speeds for the rotation of the rings. The speed is randomly selected from this range for each ring.
-        disperse_duration (int): Number of animation steps spent in the dispersed state between spinning cycles.
-        spin_disperse_cycles (int): Number of times the animation will cycles between spinning rings and dispersed characters.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the final gradient.
+        ring_gap (float): Distance between rings as a percent of the smallest output area dimension. Valid values are 0 < n <= 1.
+        spin_duration (int): Number of frames for each cycle of the spin phase. Valid values are n >= 0.
+        spin_speed (tuple[float, float]): Range of speeds for the rotation of the rings. The speed is randomly selected from this range for each ring. Valid values are n > 0.
+        disperse_duration (int): Number of frames spent in the dispersed state between spinning cycles. Valid values are n >= 0.
+        spin_disperse_cycles (int): Number of times the animation will cycle between spinning rings and dispersed characters. Valid values are n > 0.
     """
 
     ring_colors: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--ring-colors"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("ab48ff", "e7b2b2", "fffebd"),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the rings.",
     )  # type: ignore[assignment]
 
     "tuple[graphics.Color] : Tuple of colors for the rings."
 
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("ab48ff", "e7b2b2", "fffebd"),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
 
-    "tuple[graphics.Color] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+    "tuple[graphics.Color] : Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color."
 
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name=["--final-gradient-steps"],
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
 
     "tuple[int, ...] : Number of gradient steps to use. More steps will create a smoother and longer gradient animation."
 
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
-        type_parser=arg_validators.GradientDirection.type_parser,
+        type_parser=argvalidators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.VERTICAL,
-        metavar=arg_validators.GradientDirection.METAVAR,
-        help="Direction of the gradient for the final color.",
+        metavar=argvalidators.GradientDirection.METAVAR,
+        help="Direction of the final gradient.",
     )  # type: ignore[assignment]
 
-    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+    "graphics.Gradient.Direction : Direction of the final gradient."
 
     ring_gap: float = ArgField(
         cmd_name=["--ring-gap"],
-        type_parser=arg_validators.PositiveFloat.type_parser,
+        type_parser=argvalidators.PositiveFloat.type_parser,
         default=0.1,
         help="Distance between rings as a percent of the smallest output area dimension.",
     )  # type: ignore[assignment]
 
     "float : Distance between rings as a percent of the smallest output area dimension."
     spin_duration: int = ArgField(
         cmd_name=["--spin-duration"],
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         default=200,
-        help="Number of animation steps for each cycle of the spin phase.",
+        help="Number of frames for each cycle of the spin phase.",
     )  # type: ignore[assignment]
 
-    "int : Number of animation steps for each cycle of the spin phase."
+    "int : Number of frames for each cycle of the spin phase."
 
     spin_speed: tuple[float, float] = ArgField(
         cmd_name=["--spin-speed"],
-        type_parser=arg_validators.PositiveFloatRange.type_parser,
+        type_parser=argvalidators.PositiveFloatRange.type_parser,
         default=(0.25, 1.0),
-        metavar=arg_validators.PositiveFloatRange.METAVAR,
+        metavar=argvalidators.PositiveFloatRange.METAVAR,
         help="Range of speeds for the rotation of the rings. The speed is randomly selected from this range for each ring.",
     )  # type: ignore[assignment]
 
     "tuple[float, float] : Range of speeds for the rotation of the rings. The speed is randomly selected from this range for each ring."
 
     disperse_duration: int = ArgField(
         cmd_name=["--disperse-duration"],
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         default=200,
-        help="Number of animation steps spent in the dispersed state between spinning cycles.",
+        help="Number of frames spent in the dispersed state between spinning cycles.",
     )  # type: ignore[assignment]
 
-    "int : Number of animation steps spent in the dispersed state between spinning cycles."
+    "int : Number of frames spent in the dispersed state between spinning cycles."
 
     spin_disperse_cycles: int = ArgField(
         cmd_name=["--spin-disperse-cycles"],
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         default=3,
         help="Number of times the animation will cycles between spinning rings and dispersed characters.",
     )  # type: ignore[assignment]
 
     "int : Number of times the animation will cycles between spinning rings and dispersed characters."
 
     @classmethod
@@ -177,32 +186,22 @@
             disperse_scn = character.animation.new_scene(is_looping=False, id="disperse")
             disperse_gradient = graphics.Gradient(self.ring_color, self.character_color_map[character], steps=8)
             disperse_scn.apply_gradient_to_symbols(disperse_gradient, character.input_symbol, 16)
             character.motion.chain_paths(ring_paths, loop=True)
             self.characters.append(character)
 
         def make_disperse_waypoints(self, character: EffectCharacter, origin: Coord) -> motion.Path:
-            """Make the Path for the character to follow when the ring disperses.
-
-            Args:
-                character (EffectCharacter): Character to disperse.
-                origin (Coord): Origin coordinate for the character.
-
-            Returns:
-                motion.Path: the Path to follow.
-            """
             disperse_coords = geometry.find_coords_in_rect(origin, self.ring_gap)
             character.motion.paths.pop("disperse", None)
             disperse_path = character.motion.new_path(speed=0.1, loop=True, id="disperse")
             for _ in range(5):
                 disperse_path.new_waypoint(disperse_coords[random.randrange(0, len(disperse_coords))])
             return disperse_path
 
         def disperse(self) -> None:
-            """Disperse the characters from the ring."""
             for character in self.characters:
                 if character.motion.active_path is not None:
                     self.character_last_ring_path[character] = character.motion.active_path
                 else:
                     self.character_last_ring_path[character] = character.motion.paths["0"]
                 character.motion.activate_path(self.make_disperse_waypoints(character, character.motion.current_coord))
                 character.animation.activate_scene(character.animation.query_scene("disperse"))
@@ -378,14 +377,23 @@
             self._active_chars = [character for character in self._active_chars if character.is_active]
             return next_frame
         else:
             raise StopIteration
 
 
 class Rings(BaseEffect[RingsConfig]):
-    """Characters are dispersed and form into spinning rings."""
+    """Characters are dispersed and form into spinning rings.
+
+    Attributes:
+        effect_config (RingsConfig): Configuration for the effect.
+        terminal_config (TerminalConfig): Configuration for the terminal.
+    """
 
     _config_cls = RingsConfig
     _iterator_cls = RingsIterator
 
     def __init__(self, input_data: str) -> None:
+        """Initialize the effect with the provided input data.
+
+        Args:
+            input_data (str): The input data to use for the effect."""
         super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_scattered.py` & `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_scattered.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,102 +1,108 @@
+"""Text is scattered across the output area and moves into position.
+
+Classes:
+    Scattered: Move the characters into place from random starting locations.
+    ScatteredConfig: Configuration for the Scattered effect.
+    ScatteredIterator: Effect iterator for the effect. Does not normally need to be called directly.
+"""
+
 import typing
 from dataclasses import dataclass
 
-from terminaltexteffects.base_character import EffectCharacter, EventHandler
-from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
-from terminaltexteffects.utils import arg_validators, easing, graphics
+from terminaltexteffects.engine.base_character import EffectCharacter, EventHandler
+from terminaltexteffects.engine.base_effect import BaseEffect, BaseEffectIterator
+from terminaltexteffects.utils import argvalidators, easing, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 from terminaltexteffects.utils.geometry import Coord
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
     return Scattered, ScatteredConfig
 
 
 @argclass(
     name="scattered",
-    help="Move the characters into place from random starting locations.",
-    description="scattered | Move the characters into place from random starting locations.",
-    epilog=f"""{arg_validators.EASING_EPILOG}
+    help="Text is scattered across the output area and moves into position.",
+    description="scattered | Text is scattered across the output area and moves into position.",
+    epilog=f"""{argvalidators.EASING_EPILOG}
 Example: terminaltexteffects scattered --final-gradient-stops ff9048 ab9dff bdffea --final-gradient-steps 12 --final-gradient-frames 12 --movement-speed 0.5 --movement-easing IN_OUT_BACK""",
 )
 @dataclass
 class ScatteredConfig(ArgsDataClass):
     """Configuration for the effect.
 
     Attributes:
         final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient. If only one color is provided, the characters will be displayed in that color.
-        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation. Valid values are n > 0.
         final_gradient_frames (int): Number of frames to display each gradient step.
-        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
-        movement_speed (float): Movement speed of the characters. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the final gradient.
+        movement_speed (float): Movement speed of the characters. Valid values are n > 0.
         movement_easing (easing.EasingFunction): Easing function to use for character movement."""
 
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("ff9048", "ab9dff", "bdffea"),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient. If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
     "tuple[graphics.Color, ...] : Tuple of colors for the character gradient. If only one color is provided, the characters will be displayed in that color."
 
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name="--final-gradient-steps",
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         default=(12,),
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
     "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
 
     final_gradient_frames: int = ArgField(
         cmd_name="--final-gradient-frames",
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         default=12,
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Number of frames to display each gradient step.",
     )  # type: ignore[assignment]
     "int : Number of frames to display each gradient step."
 
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
-        type_parser=arg_validators.GradientDirection.type_parser,
+        type_parser=argvalidators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.VERTICAL,
-        metavar=arg_validators.GradientDirection.METAVAR,
-        help="Direction of the gradient for the final color.",
+        metavar=argvalidators.GradientDirection.METAVAR,
+        help="Direction of the final gradient.",
     )  # type: ignore[assignment]
-    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+    "graphics.Gradient.Direction : Direction of the final gradient."
 
     movement_speed: float = ArgField(
         cmd_name="--movement-speed",
-        type_parser=arg_validators.PositiveFloat.type_parser,
+        type_parser=argvalidators.PositiveFloat.type_parser,
         default=0.3,
-        metavar=arg_validators.PositiveFloat.METAVAR,
-        help="Movement speed of the characters. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.",
+        metavar=argvalidators.PositiveFloat.METAVAR,
+        help="Movement speed of the characters. ",
     )  # type: ignore[assignment]
-    "float : Movement speed of the characters. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect."
+    "float : Movement speed of the characters. "
 
     movement_easing: easing.EasingFunction = ArgField(
         cmd_name="--movement-easing",
         default=easing.in_out_back,
-        type_parser=arg_validators.Ease.type_parser,
+        type_parser=argvalidators.Ease.type_parser,
         help="Easing function to use for character movement.",
     )  # type: ignore[assignment]
     "easing.EasingFunction : Easing function to use for character movement."
 
     @classmethod
     def get_effect_class(cls):
         return Scattered
 
 
 class ScatteredIterator(BaseEffectIterator[ScatteredConfig]):
-    """Effect that moves the characters into position from random starting locations."""
-
     def __init__(self, effect: "Scattered") -> None:
         super().__init__(effect)
         self._pending_chars: list[EffectCharacter] = []
         self._active_chars: list[EffectCharacter] = []
         self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
         self._build()
 
@@ -144,14 +150,23 @@
             self._active_chars = [character for character in self._active_chars if character.is_active]
             return self._terminal.get_formatted_output_string()
         else:
             raise StopIteration
 
 
 class Scattered(BaseEffect[ScatteredConfig]):
-    """Effect that moves the characters into position from random starting locations."""
+    """Text is scattered across the output area and moves into position.
+
+    Attributes:
+        effect_config (ScatteredConfig): Configuration for the effect.
+        terminal_config (TerminalConfig): Configuration for the terminal.
+    """
 
     _config_cls = ScatteredConfig
     _iterator_cls = ScatteredIterator
 
     def __init__(self, input_data: str) -> None:
+        """Initialize the effect with the provided input data.
+
+        Args:
+            input_data (str): The input data to use for the effect."""
         super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_slide.py` & `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_slide.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,101 +1,110 @@
+"""Slide characters into view from outside the terminal.
+
+Classes:
+    Slide: Slide characters into view from outside the terminal.
+    SlideConfig: Configuration for the Slide effect.
+    SlideIterator: Effect iterator for the Slide effect. Does not normally need to be called directly.
+"""
+
 import typing
 from dataclasses import dataclass
 
-import terminaltexteffects.utils.arg_validators as arg_validators
-from terminaltexteffects.base_character import EffectCharacter
-from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
+import terminaltexteffects.utils.argvalidators as argvalidators
+from terminaltexteffects.engine.base_character import EffectCharacter
+from terminaltexteffects.engine.base_effect import BaseEffect, BaseEffectIterator
 from terminaltexteffects.utils import easing, geometry, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
     return Slide, SlideConfig
 
 
 @argclass(
     name="slide",
     help="Slide characters into view from outside the terminal.",
     description="slide | Slide characters into view from outside the terminal, grouped by row, column, or diagonal.",
-    epilog=f"""{arg_validators.EASING_EPILOG}
+    epilog=f"""{argvalidators.EASING_EPILOG}
 Example: terminaltexteffects slide --movement-speed 0.5 --grouping row --final-gradient-stops 833ab4 fd1d1d fcb045 --final-gradient-steps 12 --final-gradient-frames 10 --final-gradient-direction vertical --gap 3 --reverse-direction --merge --movement-easing OUT_QUAD""",
 )
 @dataclass
 class SlideConfig(ArgsDataClass):
     """Configuration for the Slide effect.
 
     Attributes:
-        movement_speed (float): Speed of the characters.
-        grouping (str): Direction to group characters.
-        final_gradient_stops (tuple[int | str, ...]): Tuple of colors for the character gradient. If only one color is provided, the characters will be displayed in that color.
-        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
+        movement_speed (float): Speed of the characters. Valid values are n > 0.
+        grouping (typing.Literal["row", "column", "diagonal"]): Direction to group characters. Valid values are 'row', 'column', 'diagonal'.
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient. If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation. Valid values are n > 0.
         final_gradient_frames (int): Number of frames to display each gradient step.
         final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient.
-        gap (int): Number of frames to wait before adding the next group of characters. Increasing this value creates a more staggered effect.
+        gap (int): Number of frames to wait before adding the next group of characters. Increasing this value creates a more staggered effect. Valid values are n >= 0.
         reverse_direction (bool): Reverse the direction of the characters.
-        merge (bool): Merge the character groups originating"""
+        merge (bool): Merge the character groups originating.
+        movement_easing (easing.EasingFunction): Easing function to use for character movement."""
 
     movement_speed: float = ArgField(
         cmd_name="--movement-speed",
-        type_parser=arg_validators.PositiveFloat.type_parser,
+        type_parser=argvalidators.PositiveFloat.type_parser,
         default=0.5,
-        metavar=arg_validators.PositiveFloat.METAVAR,
+        metavar=argvalidators.PositiveFloat.METAVAR,
         help="Speed of the characters.",
     )  # type: ignore[assignment]
     "float : Speed of the characters."
 
-    grouping: str = ArgField(
+    grouping: typing.Literal["row", "column", "diagonal"] = ArgField(
         cmd_name="--grouping",
         default="row",
         choices=["row", "column", "diagonal"],
         help="Direction to group characters.",
     )  # type: ignore[assignment]
-    "str : Direction to group characters."
+    "typing.Literal['row', 'column', 'diagonal'] : Direction to group characters. Valid values are Literal['row', 'column', 'diagonal']."
 
-    final_gradient_stops: tuple[int | str, ...] = ArgField(
+    final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("833ab4", "fd1d1d", "fcb045"),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient. If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
-    "tuple[int | str, ...] : Tuple of colors for the character gradient. If only one color is provided, the characters will be displayed in that color."
+    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient. If only one color is provided, the characters will be displayed in that color."
 
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name="--final-gradient-steps",
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         default=(12,),
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
     "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
 
     final_gradient_frames: int = ArgField(
         cmd_name="--final-gradient-frames",
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         default=10,
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Number of frames to display each gradient step.",
     )  # type: ignore[assignment]
     "int : Number of frames to display each gradient step."
 
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
         default=graphics.Gradient.Direction.VERTICAL,
-        type_parser=arg_validators.GradientDirection.type_parser,
+        type_parser=argvalidators.GradientDirection.type_parser,
         help="Direction of the gradient (vertical, horizontal, diagonal, center).",
     )  # type: ignore[assignment]
     "graphics.Gradient.Direction : Direction of the gradient."
 
     gap: int = ArgField(
         cmd_name="--gap",
-        type_parser=arg_validators.NonNegativeInt.type_parser,
+        type_parser=argvalidators.NonNegativeInt.type_parser,
         default=3,
-        metavar=arg_validators.NonNegativeInt.METAVAR,
+        metavar=argvalidators.NonNegativeInt.METAVAR,
         help="Number of frames to wait before adding the next group of characters. Increasing this value creates a more staggered effect.",
     )  # type: ignore[assignment]
     "int : Number of frames to wait before adding the next group of characters. Increasing this value creates a more staggered effect."
 
     reverse_direction: bool = ArgField(
         cmd_name="--reverse-direction",
         action="store_true",
@@ -109,28 +118,26 @@
         help="Merge the character groups originating from either side of the terminal. (--reverse-direction is ignored when merging)",
     )  # type: ignore[assignment]
     "bool : Merge the character groups originating from either side of the terminal."
 
     movement_easing: easing.EasingFunction = ArgField(
         cmd_name=["--movement-easing"],
         default=easing.in_out_quad,
-        type_parser=arg_validators.Ease.type_parser,
-        metavar=arg_validators.Ease.METAVAR,
+        type_parser=argvalidators.Ease.type_parser,
+        metavar=argvalidators.Ease.METAVAR,
         help="Easing function to use for character movement.",
     )  # type: ignore[assignment]
     "easing.EasingFunction : Easing function to use for character movement."
 
     @classmethod
     def get_effect_class(cls):
         return Slide
 
 
 class SlideIterator(BaseEffectIterator[SlideConfig]):
-    """Effect that slides characters into view from outside the terminal. Characters are grouped by column, row, or diagonal."""
-
     def __init__(self, effect: "Slide") -> None:
         super().__init__(effect)
         self._pending_chars: list[EffectCharacter] = []
         self._active_chars: list[EffectCharacter] = []
         self._pending_groups: list[list[EffectCharacter]] = []
         self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
         self._build()
@@ -239,14 +246,23 @@
             self._active_chars = [character for character in self._active_chars if character.is_active]
             return self._terminal.get_formatted_output_string()
         else:
             raise StopIteration
 
 
 class Slide(BaseEffect[SlideConfig]):
-    """Effect that slides characters into view from outside the terminal. Characters are grouped by column, row, or diagonal."""
+    """Slides characters into view from outside the terminal.
+
+    Attributes:
+        effect_config (SlideConfig): Configuration for the effect.
+        terminal_config (TerminalConfig): Configuration for the terminal.
+    """
 
     _config_cls = SlideConfig
     _iterator_cls = SlideIterator
 
     def __init__(self, input_data: str) -> None:
+        """Initialize the effect with the provided input data.
+
+        Args:
+            input_data (str): The input data to use for the effect."""
         super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_spotlights.py` & `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_spotlights.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,115 +1,124 @@
+"""Spotlights search the text area, illuminating characters, before converging in the center and expanding.
+
+Classes:
+    Spotlights: Spotlights search the text area, illuminating characters, before converging in the center and expanding.
+    SpotlightsConfig: Configuration for the Spotlights effect.
+    SpotlightsIterator: Effect iterator for the Spotlights effect. Does not normally need to be called directly.
+"""
+
 import random
 import typing
 from dataclasses import dataclass
 
-import terminaltexteffects.utils.arg_validators as arg_validators
-from terminaltexteffects.base_character import EffectCharacter
-from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
-from terminaltexteffects.utils import animation, easing, geometry, graphics, motion
+import terminaltexteffects.utils.argvalidators as argvalidators
+from terminaltexteffects.engine import animation, motion
+from terminaltexteffects.engine.base_character import EffectCharacter
+from terminaltexteffects.engine.base_effect import BaseEffect, BaseEffectIterator
+from terminaltexteffects.utils import easing, geometry, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 from terminaltexteffects.utils.geometry import Coord
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
     return Spotlights, SpotlightsConfig
 
 
 @argclass(
     name="spotlights",
     help="Spotlights search the text area, illuminating characters, before converging in the center and expanding.",
     description="spotlights | Spotlights search the text area, illuminating characters, before converging in the center and expanding.",
-    epilog=f"""{arg_validators.EASING_EPILOG}
+    epilog=f"""{argvalidators.EASING_EPILOG}
 Example: terminaltexteffects spotlights --final-gradient-stops ab48ff e7b2b2 fffebd --final-gradient-steps 12 --beam-width-ratio 2.0 --beam-falloff 0.3 --search-duration 750 --search-speed-range 0.25-0.5 --spotlight-count 3""",
 )
 @dataclass
 class SpotlightsConfig(ArgsDataClass):
     """Configuration for the Spotlights effect.
 
     Attributes:
-        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
-        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
-        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
-        beam_width_ratio (float): Width of the beam of light as min(width, height) // n of the input text.
-        beam_falloff (float): Distance from the edge of the beam where the brightness begins to fall off, as a percentage of total beam width.
-        search_duration (int): Duration of the search phase, in animation steps, before the spotlights converge in the center.
-        search_speed_range (tuple[float, float]): Range of speeds for the spotlights during the search phase. The speed is a random value between the two provided values.
-        spotlight_count (int): Number of spotlights to use.
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation. Valid values are n > 0.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the final gradient.
+        beam_width_ratio (float): Width of the beam of light as min(width, height) // n of the input text. Valid values are n > 0.
+        beam_falloff (float): Distance from the edge of the beam where the brightness begins to fall off, as a percentage of total beam width. Valid values are 0 <= n <= 1.
+        search_duration (int): Duration of the search phase, in frames, before the spotlights converge in the center. Valid values are n > 0.
+        search_speed_range (tuple[float, float]): Range of speeds for the spotlights during the search phase. The speed is a random value between the two provided values. Valid values are n > 0.
+        spotlight_count (int): Number of spotlights to use. Valid values are n > 0.
     """
 
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("ab48ff", "e7b2b2", "fffebd"),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
-    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+    "tuple[graphics.Color, ...] : Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color."
 
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name="--final-gradient-steps",
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
     "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
 
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
-        type_parser=arg_validators.GradientDirection.type_parser,
+        type_parser=argvalidators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.VERTICAL,
-        metavar=arg_validators.GradientDirection.METAVAR,
-        help="Direction of the gradient for the final color.",
+        metavar=argvalidators.GradientDirection.METAVAR,
+        help="Direction of the final gradient.",
     )  # type: ignore[assignment]
-    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+    "graphics.Gradient.Direction : Direction of the final gradient."
 
     beam_width_ratio: float = ArgField(
         cmd_name="--beam-width-ratio",
-        type_parser=arg_validators.PositiveFloat.type_parser,
+        type_parser=argvalidators.PositiveFloat.type_parser,
         default=2.0,
-        metavar=arg_validators.PositiveFloat.METAVAR,
+        metavar=argvalidators.PositiveFloat.METAVAR,
         help="Width of the beam of light as min(width, height) // n of the input text.",
     )  # type: ignore[assignment]
     "float : Width of the beam of light as min(width, height) // n of the input text."
 
     beam_falloff: float = ArgField(
         cmd_name="--beam-falloff",
-        type_parser=arg_validators.NonNegativeFloat.type_parser,
+        type_parser=argvalidators.NonNegativeFloat.type_parser,
         default=0.3,
-        metavar=arg_validators.NonNegativeFloat.METAVAR,
+        metavar=argvalidators.NonNegativeFloat.METAVAR,
         help="Distance from the edge of the beam where the brightness begins to fall off, as a percentage of total beam width.",
     )  # type: ignore[assignment]
     "float : Distance from the edge of the beam where the brightness begins to fall off, as a percentage of total beam width."
 
     search_duration: int = ArgField(
         cmd_name="--search-duration",
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         default=750,
-        metavar=arg_validators.PositiveInt.METAVAR,
-        help="Duration of the search phase, in animation steps, before the spotlights converge in the center.",
+        metavar=argvalidators.PositiveInt.METAVAR,
+        help="Duration of the search phase, in frames, before the spotlights converge in the center.",
     )  # type: ignore[assignment]
-    "int : Duration of the search phase, in animation steps, before the spotlights converge in the center."
+    "int : Duration of the search phase, in frames, before the spotlights converge in the center."
 
     search_speed_range: tuple[float, float] = ArgField(
         cmd_name="--search-speed-range",
-        type_parser=arg_validators.PositiveFloatRange.type_parser,
+        type_parser=argvalidators.PositiveFloatRange.type_parser,
         default=(0.25, 0.5),
-        metavar=arg_validators.PositiveFloatRange.METAVAR,
+        metavar=argvalidators.PositiveFloatRange.METAVAR,
         help="Range of speeds for the spotlights during the search phase. The speed is a random value between the two provided values.",
     )  # type: ignore[assignment]
     "tuple[float, float] : Range of speeds for the spotlights during the search phase. The speed is a random value between the two provided values."
 
     spotlight_count: int = ArgField(
         cmd_name="--spotlight-count",
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         default=3,
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Number of spotlights to use.",
     )  # type: ignore[assignment]
     "int : Number of spotlights to use."
 
     @classmethod
     def get_effect_class(cls):
         return Spotlights
@@ -252,14 +261,23 @@
                 character.tick()
             return self._terminal.get_formatted_output_string()
         else:
             raise StopIteration
 
 
 class Spotlights(BaseEffect[SpotlightsConfig]):
-    """Spotlights search the text area, illuminating characters, before converging in the center and expanding."""
+    """Spotlights search the text area, illuminating characters, before converging in the center and expanding.
+
+    Attributes:
+        effect_config (SpotlightsConfig): Configuration for the effect.
+        terminal_config (TerminalConfig): Configuration for the terminal.
+    """
 
     _config_cls = SpotlightsConfig
     _iterator_cls = SpotlightsIterator
 
     def __init__(self, input_data: str) -> None:
+        """Initialize the effect with the provided input data.
+
+        Args:
+            input_data (str): The input data to use for the effect."""
         super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_spray.py` & `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_spray.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,118 +1,122 @@
-"""Effect that draws the characters spawning at varying rates from a single point."""
+"""Sprays the characters from a single point.
+
+Classes:
+    Spray: Sprays the characters from a single point.
+    SprayConfig: Configuration for the Spray effect.
+    SprayIterator: Iterates over the effect. Does not normally need to be called directly.
+"""
 
 import random
 import typing
 from dataclasses import dataclass
 from enum import Enum, auto
 
-import terminaltexteffects.utils.arg_validators as arg_validators
-from terminaltexteffects.base_character import EffectCharacter, EventHandler
-from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
+import terminaltexteffects.utils.argvalidators as argvalidators
+from terminaltexteffects.engine.base_character import EffectCharacter, EventHandler
+from terminaltexteffects.engine.base_effect import BaseEffect, BaseEffectIterator
 from terminaltexteffects.utils import easing, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 from terminaltexteffects.utils.geometry import Coord
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
     return Spray, SprayConfig
 
 
 @argclass(
     name="spray",
     help="Draws the characters spawning at varying rates from a single point.",
     description="spray | Draws the characters spawning at varying rates from a single point.",
-    epilog=f"""{arg_validators.EASING_EPILOG}    
+    epilog=f"""{argvalidators.EASING_EPILOG}    
 Example: terminaltexteffects spray --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --spray-position e --spray-volume 0.005 --movement-speed 0.4-1.0 --movement-easing OUT_EXPO""",
 )
 @dataclass
 class SprayConfig(ArgsDataClass):
     """Configuration for the Spray effect.
 
     Attributes:
-        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
-        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
-        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
-        spray_position (str): Position for the spray origin.
-        spray_volume (float): Number of characters to spray per tick as a percent of the total number of characters.
-        movement_speed (tuple[float, float]): Movement speed of the characters.
-        movement_easing (typing.Callable): Easing function to use for character movement."""
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation. Valid values are n > 0.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the final gradient.
+        spray_position (typing.Literal["n", "ne", "e", "se", "s", "sw", "w", "nw", "center"]): Position for the spray origin. Valid values are n, ne, e, se, s, sw, w, nw, center.
+        spray_volume (float): Number of characters to spray per tick as a percent of the total number of characters. Valid values are 0 < n <= 1.
+        movement_speed (tuple[float, float]): Movement speed of the characters. Valid values are n > 0.
+        movement_easing (easing.EasingFunction): Easing function to use for character movement."""
 
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("8A008A", "00D1FF", "FFFFFF"),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
-    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+    "tuple[graphics.Color, ...] : Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color."
 
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name=["--final-gradient-steps"],
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
     "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
 
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
-        type_parser=arg_validators.GradientDirection.type_parser,
+        type_parser=argvalidators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.VERTICAL,
-        metavar=arg_validators.GradientDirection.METAVAR,
-        help="Direction of the gradient for the final color.",
+        metavar=argvalidators.GradientDirection.METAVAR,
+        help="Direction of the final gradient.",
     )  # type: ignore[assignment]
-    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+    "graphics.Gradient.Direction : Direction of the final gradient."
 
-    spray_position: str = ArgField(
+    spray_position: typing.Literal["n", "ne", "e", "se", "s", "sw", "w", "nw", "center"] = ArgField(
         cmd_name="--spray-position",
         choices=["n", "ne", "e", "se", "s", "sw", "w", "nw", "center"],
         default="e",
         help="Position for the spray origin.",
     )  # type: ignore[assignment]
-    "str : Position for the spray origin."
+    "typing.Literal['n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw', 'center'] : Position for the spray origin."
 
     spray_volume: float = ArgField(
         cmd_name="--spray-volume",
-        type_parser=arg_validators.PositiveFloat.type_parser,
+        type_parser=argvalidators.PositiveFloat.type_parser,
         default=0.005,
-        metavar=arg_validators.PositiveFloat.METAVAR,
+        metavar=argvalidators.PositiveFloat.METAVAR,
         help="Number of characters to spray per tick as a percent of the total number of characters.",
     )  # type: ignore[assignment]
     "float : Number of characters to spray per tick as a percent of the total number of characters."
 
     movement_speed: tuple[float, float] = ArgField(
         cmd_name="--movement-speed",
-        type_parser=arg_validators.PositiveFloatRange.type_parser,
+        type_parser=argvalidators.PositiveFloatRange.type_parser,
         default=(0.4, 1.0),
-        metavar=arg_validators.PositiveFloatRange.METAVAR,
+        metavar=argvalidators.PositiveFloatRange.METAVAR,
         help="Movement speed of the characters.",
     )  # type: ignore[assignment]
     "tuple[float, float] : Movement speed of the characters."
 
     movement_easing: easing.EasingFunction = ArgField(
         cmd_name="--movement-easing",
-        type_parser=arg_validators.Ease.type_parser,
+        type_parser=argvalidators.Ease.type_parser,
         default=easing.out_expo,
         help="Easing function to use for character movement.",
     )  # type: ignore[assignment]
     "easing.EasingFunction : Easing function to use for character movement."
 
     @classmethod
     def get_effect_class(cls):
         return Spray
 
 
 class SprayIterator(BaseEffectIterator[SprayConfig]):
     class _SprayPosition(Enum):
-        """Position for the spray origin."""
-
         N = auto()
         NE = auto()
         E = auto()
         SE = auto()
         S = auto()
         SW = auto()
         W = auto()
@@ -207,14 +211,23 @@
             self._active_chars = [character for character in self._active_chars if character.is_active]
             return self._terminal.get_formatted_output_string()
         else:
             raise StopIteration
 
 
 class Spray(BaseEffect[SprayConfig]):
-    """Effect that draws the characters spawning at varying rates from a single point."""
+    """Sprays the characters from a single point.
+
+    Attributes:
+        effect_config (SprayConfig): Configuration for the effect.
+        terminal_config (TerminalConfig): Configuration for the terminal.
+    """
 
     _config_cls = SprayConfig
     _iterator_cls = SprayIterator
 
     def __init__(self, input_data: str) -> None:
+        """Initialize the effect with the provided input data.
+
+        Args:
+            input_data (str): The input data to use for the effect."""
         super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_swarm.py` & `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_swarm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,24 @@
+"""Characters are grouped into swarms and move around the terminal before settling into position.
+
+Classes:
+    Swarm: Characters are grouped into swarms and move around the terminal before settling into position.
+    SwarmConfig: Configuration for the Swarm effect.
+    SwarmIterator: Effect iterator for the Swarm effect. Does not normally need to be called directly.
+"""
+
 import random
 import typing
 from dataclasses import dataclass
 
-import terminaltexteffects.utils.arg_validators as arg_validators
-from terminaltexteffects.base_character import EffectCharacter, EventHandler
-from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
-from terminaltexteffects.utils import animation, easing, geometry, graphics
+import terminaltexteffects.utils.argvalidators as argvalidators
+from terminaltexteffects.engine import animation
+from terminaltexteffects.engine.base_character import EffectCharacter, EventHandler
+from terminaltexteffects.engine.base_effect import BaseEffect, BaseEffectIterator
+from terminaltexteffects.utils import easing, geometry, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 from terminaltexteffects.utils.geometry import Coord
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
     return Swarm, SwarmConfig
 
@@ -23,104 +32,102 @@
 @dataclass
 class SwarmConfig(ArgsDataClass):
     """Configuration for the Swarm effect.
 
     Attributes:
         base_color (tuple[graphics.Color, ...]): Tuple of colors for the swarms.
         flash_color (graphics.Color): Color for the character flash. Characters flash when moving.
-        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
-        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
-        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
-        swarm_size (float): Percent of total characters in each swarm.
-        swarm_coordination (float): Percent of characters in a swarm that move as a group.
-        swarm_area_count (tuple[int, int]): Range of the number of areas where characters will swarm."""
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation. Valid values are n > 0.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the final gradient.
+        swarm_size (float): Percent of total characters in each swarm. Valid values are 0 < n <= 1.
+        swarm_coordination (float): Percent of characters in a swarm that move as a group. Valid values are 0 < n <= 1.
+        swarm_area_count (tuple[int, int]): Range of the number of areas where characters will swarm. Valid values are n > 0."""
 
     base_color: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--base-color"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("31a0d4",),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the swarms",
     )  # type: ignore[assignment]
     """tuple[graphics.Color, ...] : Tuple of colors for the swarms"""
 
     flash_color: graphics.Color = ArgField(
         cmd_name=["--flash-color"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         default="f2ea79",
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Color for the character flash. Characters flash when moving.",
     )  # type: ignore[assignment]
     """graphics.Color : Color for the character flash. Characters flash when moving."""
 
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("31b900", "f0ff65"),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
-    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+    "tuple[graphics.Color, ...] : Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color."
 
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name=["--final-gradient-steps"],
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
     "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
 
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
-        type_parser=arg_validators.GradientDirection.type_parser,
+        type_parser=argvalidators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.HORIZONTAL,
-        metavar=arg_validators.GradientDirection.METAVAR,
-        help="Direction of the gradient for the final color.",
+        metavar=argvalidators.GradientDirection.METAVAR,
+        help="Direction of the final gradient.",
     )  # type: ignore[assignment]
-    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+    "graphics.Gradient.Direction : Direction of the final gradient."
 
     swarm_size: float = ArgField(
         cmd_name="--swarm-size",
-        type_parser=arg_validators.Ratio.type_parser,
-        metavar=arg_validators.Ratio.METAVAR,
+        type_parser=argvalidators.Ratio.type_parser,
+        metavar=argvalidators.Ratio.METAVAR,
         default=0.1,
         help="Percent of total characters in each swarm.",
     )  # type: ignore[assignment]
     "float : Percent of total characters in each swarm."
 
     swarm_coordination: float = ArgField(
         cmd_name="--swarm-coordination",
-        type_parser=arg_validators.Ratio.type_parser,
-        metavar=arg_validators.Ratio.METAVAR,
+        type_parser=argvalidators.Ratio.type_parser,
+        metavar=argvalidators.Ratio.METAVAR,
         default=0.80,
         help="Percent of characters in a swarm that move as a group.",
     )  # type: ignore[assignment]
     "float : Percent of characters in a swarm that move as a group."
 
     swarm_area_count: tuple[int, int] = ArgField(
         cmd_name="--swarm-area-count",
-        type_parser=arg_validators.IntRange.type_parser,
-        metavar=arg_validators.IntRange.METAVAR,
+        type_parser=argvalidators.IntRange.type_parser,
+        metavar=argvalidators.IntRange.METAVAR,
         default=(2, 4),
         help="Range of the number of areas where characters will swarm.",
     )  # type: ignore[assignment]
     "tuple[int, int] : Range of the number of areas where characters will swarm."
 
     @classmethod
     def get_effect_class(cls):
         return Swarm
 
 
 class SwarmIterator(BaseEffectIterator[SwarmConfig]):
-    """Characters behave with swarm characteristics before flying into position."""
-
     def __init__(
         self,
         effect: "Swarm",
     ) -> None:
         super().__init__(effect)
         self._pending_chars: list[EffectCharacter] = []
         self._active_chars: list[EffectCharacter] = []
@@ -263,14 +270,23 @@
             self._active_chars = [character for character in self._active_chars if character.is_active]
             return self._terminal.get_formatted_output_string()
         else:
             raise StopIteration
 
 
 class Swarm(BaseEffect[SwarmConfig]):
-    """Characters are grouped into swarms and move around the terminal before settling into position."""
+    """Characters are grouped into swarms and move around the terminal before settling into position.
+
+    Attributes:
+        effect_config (SwarmConfig): Configuration for the effect.
+        terminal_config (TerminalConfig): Configuration for the terminal.
+    """
 
     _config_cls = SwarmConfig
     _iterator_cls = SwarmIterator
 
     def __init__(self, input_data: str) -> None:
+        """Initialize the effect with the provided input data.
+
+        Args:
+            input_data (str): The input data to use for the effect."""
         super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_synthgrid.py` & `terminaltexteffects-0.9.0/terminaltexteffects/engine/motion.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,427 +1,530 @@
-import random
+"""This module provides classes and methods for managing and manipulating character motion.
+
+Classes:
+    Waypoint: A Waypoint comprises a coordinate, speed, and, optionally, bezier control point(s).
+    Segment: A segment of a path consisting of two waypoints and the distance between them.
+    Path: Represents a path consisting of multiple waypoints for motion.
+    Motion: Motion class for managing the movement of a character.
+"""
+
 import typing
 from dataclasses import dataclass
 
-from terminaltexteffects.base_character import EffectCharacter, EventHandler
-from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
-from terminaltexteffects.utils import arg_validators, geometry, graphics
-from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
+from terminaltexteffects.utils import easing, geometry
 from terminaltexteffects.utils.geometry import Coord
-from terminaltexteffects.utils.terminal import Terminal
 
+if typing.TYPE_CHECKING:
+    from terminaltexteffects.engine import base_character
+
+
+@dataclass
+class Waypoint:
+    """A Waypoint comprises a coordinate, speed, and, optionally, bezier control point(s).
+
+    Args:
+        waypoint_id (str): unique identifier for the waypoint
+        coord (Coord): coordinate
+        bezier_control (tuple[Coord, ...] | Coord | None): coordinate of the control point for a bezier curve. Defaults to None.
+    """
+
+    waypoint_id: str
+    coord: Coord
+    bezier_control: tuple[Coord, ...] | Coord | None = None
+
+    def __post_init__(self) -> None:
+        if self.bezier_control and isinstance(self.bezier_control, Coord):
+            self.bezier_control = (self.bezier_control,)
+
+    def __eq__(self, other: typing.Any) -> bool:
+        if not isinstance(other, Waypoint):
+            return NotImplemented
+        return self.coord == other.coord
 
-def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
-    return SynthGrid, SynthGridConfig
+    def __hash__(self):
+        return hash(self.waypoint_id)
 
 
-@argclass(
-    name="synthgrid",
-    help="Create a grid which fills with characters dissolving into the final text.",
-    description="synthgrid | Create a grid which fills with characters dissolving into the final text.",
-    epilog="""Example: terminaltexteffects synthgrid --grid-gradient-stops CC00CC ffffff --grid-gradient-steps 12 --text-gradient-stops 8A008A 00D1FF FFFFFF --text-gradient-steps 12 --grid-row-symbol ─ --grid-column-symbol "│" --text-generation-symbols ░ ▒ ▓ --max-active-blocks 0.1""",
-)
 @dataclass
-class SynthGridConfig(ArgsDataClass):
-    """Configuration for the SynthGrid effect.
+class Segment:
+    """A segment of a path consisting of two waypoints and the distance between them.
 
     Attributes:
-        grid_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the grid gradient.
-        grid_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
-        grid_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the grid color.
-        text_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the text gradient.
-        text_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
-        text_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the text color.
-        grid_row_symbol (str): Symbol to use for grid row lines.
-        grid_column_symbol (str): Symbol to use for grid column lines.
-        text_generation_symbols (tuple[str, ...]): Tuple of characters for the text generation animation.
-        max_active_blocks (float): Maximum percentage of blocks to have active at any given time. For example, if set to 0.1, 10 percent of the blocks will be active at any given time."""
-
-    grid_gradient_stops: tuple[graphics.Color, ...] = ArgField(
-        cmd_name=["--grid-gradient-stops"],
-        type_parser=arg_validators.Color.type_parser,
-        nargs="+",
-        default=("CC00CC", "ffffff"),
-        metavar=arg_validators.Color.METAVAR,
-        help="Space separated, unquoted, list of colors for the grid gradient.",
-    )  # type: ignore[assignment]
-    "tuple[graphics.Color, ...] : Tuple of colors for the grid gradient."
-
-    grid_gradient_steps: tuple[int, ...] = ArgField(
-        cmd_name="--grid-gradient-steps",
-        type_parser=arg_validators.PositiveInt.type_parser,
-        nargs="+",
-        default=(12,),
-        metavar=arg_validators.PositiveInt.METAVAR,
-        help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
-    )  # type: ignore[assignment]
-    "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
-
-    grid_gradient_direction: graphics.Gradient.Direction = ArgField(
-        cmd_name="--grid-gradient-direction",
-        type_parser=arg_validators.GradientDirection.type_parser,
-        default=graphics.Gradient.Direction.DIAGONAL,
-        metavar=arg_validators.GradientDirection.METAVAR,
-        help="Direction of the gradient for the grid color.",
-    )  # type: ignore[assignment]
-    "graphics.Gradient.Direction : Direction of the gradient for the grid color."
-
-    text_gradient_stops: tuple[graphics.Color, ...] = ArgField(
-        cmd_name=["--text-gradient-stops"],
-        type_parser=arg_validators.Color.type_parser,
-        nargs="+",
-        default=("8A008A", "00D1FF", "FFFFFF"),
-        metavar=arg_validators.Color.METAVAR,
-        help="Space separated, unquoted, list of colors for the text gradient.",
-    )  # type: ignore[assignment]
-    "tuple[graphics.Color, ...] : Tuple of colors for the text gradient."
-
-    text_gradient_steps: tuple[int, ...] = ArgField(
-        cmd_name="--text-gradient-steps",
-        type_parser=arg_validators.PositiveInt.type_parser,
-        nargs="+",
-        default=(12,),
-        metavar=arg_validators.PositiveInt.METAVAR,
-        help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
-    )  # type: ignore[assignment]
-    "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
-
-    text_gradient_direction: graphics.Gradient.Direction = ArgField(
-        cmd_name="--text-gradient-direction",
-        type_parser=arg_validators.GradientDirection.type_parser,
-        default=graphics.Gradient.Direction.VERTICAL,
-        metavar=arg_validators.GradientDirection.METAVAR,
-        help="Direction of the gradient for the text color.",
-    )  # type: ignore[assignment]
-    "graphics.Gradient.Direction : Direction of the gradient for the text color."
-
-    grid_row_symbol: str = ArgField(
-        cmd_name="--grid-row-symbol",
-        type_parser=arg_validators.Symbol.type_parser,
-        default="─",
-        metavar=arg_validators.Symbol.METAVAR,
-        help="Symbol to use for grid row lines.",
-    )  # type: ignore[assignment]
-    "str : Symbol to use for grid row lines."
-
-    grid_column_symbol: str = ArgField(
-        cmd_name="--grid-column-symbol",
-        type_parser=arg_validators.Symbol.type_parser,
-        default="│",
-        metavar=arg_validators.Symbol.METAVAR,
-        help="Symbol to use for grid column lines.",
-    )  # type: ignore[assignment]
-    "str : Symbol to use for grid column lines."
-
-    text_generation_symbols: tuple[str, ...] = ArgField(
-        cmd_name="--text-generation-symbols",
-        type_parser=arg_validators.Symbol.type_parser,
-        nargs="+",
-        default=("░", "▒", "▓"),
-        metavar=arg_validators.Symbol.METAVAR,
-        help="Space separated, unquoted, list of characters for the text generation animation.",
-    )  # type: ignore[assignment]
-    "tuple[str, ...] : Tuple of characters for the text generation animation."
-
-    max_active_blocks: float = ArgField(
-        cmd_name="--max-active-blocks",
-        type_parser=arg_validators.PositiveFloat.type_parser,
-        default=0.1,
-        metavar=arg_validators.PositiveFloat.METAVAR,
-        help="Maximum percentage of blocks to have active at any given time. For example, if set to 0.1, 10 percent of the blocks will be active at any given time.",
-    )  # type: ignore[assignment]
-    "float : Maximum percentage of blocks to have active at any given time."
-
-    @classmethod
-    def get_effect_class(cls):
-        return SynthGrid
+        start (Waypoint): start waypoint
+        end (Waypoint): end waypoint
+        distance (float): distance between the start and end waypoints
+
+    Methods:
+        get_coord_on_segment(distance_factor: float) -> Coord:
+            Returns the coordinate at the given distance along the segment.
+    """
+
+    start: Waypoint
+    end: Waypoint
+    distance: float
+
+    def __post_init__(self) -> None:
+        self.enter_event_triggered: bool = False
+        self.exit_event_triggered: bool = False
 
+    def get_coord_on_segment(self, distance_factor: float) -> Coord:
+        """Returns the coordinate at the given distance along the segment.
 
-class _GridLine:
-    def __init__(
-        self,
-        terminal: Terminal,
-        args: SynthGridConfig,
-        origin: Coord,
-        direction: str,
-        grid_gradient_mapping: dict[geometry.Coord, graphics.Color],
-    ):
-        self.terminal = terminal
-        self.args = args
-        self.origin = origin
-        self.direction = direction
-        if self.direction == "horizontal":
-            self.grid_symbol = self.args.grid_row_symbol
-        elif self.direction == "vertical":
-            self.grid_symbol = self.args.grid_column_symbol
-        self.characters: list[EffectCharacter] = []
-        if direction == "horizontal":
-            for column_index in range(self.terminal.output_area.left, self.terminal.output_area.right + 1):
-                effect_char = self.terminal.add_character(self.grid_symbol, Coord(0, 0))
-                grid_scn = effect_char.animation.new_scene()
-                grid_scn.add_frame(
-                    self.grid_symbol, 1, color=grid_gradient_mapping[geometry.Coord(column_index, origin.row)]
-                )
-                effect_char.animation.activate_scene(grid_scn)
-                effect_char.layer = 2
-                effect_char.motion.set_coordinate(Coord(column_index, origin.row))
-                self.characters.append(effect_char)
-        elif direction == "vertical":
-            for row_index in range(self.terminal.output_area.bottom, self.terminal.output_area.top):
-                effect_char = self.terminal.add_character(self.grid_symbol, Coord(0, 0))
-                grid_scn = effect_char.animation.new_scene()
-                grid_scn.add_frame(
-                    self.grid_symbol, 1, color=grid_gradient_mapping[geometry.Coord(origin.column, row_index)]
-                )
-                effect_char.animation.activate_scene(grid_scn)
-                effect_char.layer = 2
-                effect_char.motion.set_coordinate(Coord(origin.column, row_index))
-                self.characters.append(effect_char)
-        self.collapsed_characters = [effect_char for effect_char in self.characters]
-        self.extended_characters: list[EffectCharacter] = []
-
-    def extend(self) -> None:
-        if self.direction == "horizontal":
-            count = 3
-        else:
-            count = 1
-        for _ in range(count):
-            if self.collapsed_characters:
-                next_char = self.collapsed_characters.pop(0)
-                self.terminal.set_character_visibility(next_char, True)
-                self.extended_characters.append(next_char)
-
-    def collapse(self) -> None:
-        if self.direction == "horizontal":
-            count = 3
+        Args:
+            distance_factor (float): distance factor
+
+        Returns:
+            Coord: Coordinate at the given distance.
+        """
+        if self.start.bezier_control:
+            return geometry.find_coord_on_bezier_curve(
+                self.start.coord,
+                self.start.bezier_control,
+                self.end.coord,
+                distance_factor,
+            )
         else:
-            count = 1
-        if not self.collapsed_characters:
-            self.extended_characters = self.extended_characters[::-1]
-        for _ in range(count):
-            if self.extended_characters:
-                next_char = self.extended_characters.pop(0)
-                self.terminal.set_character_visibility(next_char, False)
-                self.collapsed_characters.append(next_char)
-
-    def is_extended(self) -> bool:
-        return not self.collapsed_characters
-
-    def is_collapsed(self) -> bool:
-        return not self.extended_characters
-
-
-class SynthGridIterator(BaseEffectIterator[SynthGridConfig]):
-    """Effect that creates a grid where blocks of characters dissolved into the input characters."""
-
-    def __init__(self, effect: "SynthGrid") -> None:
-        super().__init__(effect)
-        self._pending_groups: list[tuple[int, list[EffectCharacter]]] = []
-        self._active_chars: list[EffectCharacter] = []
-        self._grid_lines: list[_GridLine] = []
-        self._group_tracker: dict[int, int] = {}
-        self._build()
+            return geometry.find_coord_on_line(self.start.coord, self.end.coord, distance_factor)
+
+    def __eq__(self, other: typing.Any) -> bool:
+        if not isinstance(other, Segment):
+            return NotImplemented
+        return self.start == other.start and self.end == other.end
 
-    def _find_even_gap(self, dimension: int) -> int:
-        """Find the closest even gap to 20% of the longest dimension.
+    def __hash__(self):
+        return hash((self.start, self.end))
+
+
+@dataclass
+class Path:
+    """
+    Represents a path consisting of multiple waypoints for motion.
+
+    Attributes:
+        path_id (str): The unique identifier for the path.
+        speed (float): speed > 0
+        ease (easing.EasingFunction | None): easing function for character movement. Defaults to None.
+        layer (int | None): layer to move the character to, if None, layer is unchanged. Defaults to None.
+        hold_time (int): number of frames to hold the character at the end of the path. Defaults to 0.
+        loop (bool): Whether the path should loop back to the beginning. Default is False.
+
+    Methods:
+        new_waypoint(coord: Coord, bezier_control: tuple[Coord, ...] | Coord | None = None, id: str = "") -> Waypoint:
+            Creates a new Waypoint and appends adds it to the Path.
+        query_waypoint(waypoint_id: str) -> Waypoint:
+            Returns the waypoint with the given waypoint_id.
+        step(event_handler: base_character.EventHandler) -> Coord:
+            Progresses to the next step along the path and returns the coordinate at that step.
+    """
+
+    path_id: str
+    speed: float = 1.0
+    ease: easing.EasingFunction | None = None
+    layer: int | None = None
+    hold_time: int = 0
+    loop: bool = False
+
+    def __post_init__(self) -> None:
+        """
+        Initializes the Path object and calculates the total distance and maximum steps.
+        """
+        self.segments: list[Segment] = []
+        self.waypoints: list[Waypoint] = []
+        self.waypoint_lookup: dict[str, Waypoint] = {}
+        self.total_distance: float = 0
+        self.current_step: int = 0
+        self.max_steps: int = 0
+        self.hold_time_remaining = self.hold_time
+        self.last_distance_reached: float = 0  # used for animation syncing to distance
+        self.origin_segment: Segment | None = None
+        if self.speed <= 0:
+            raise ValueError(f"({self.speed=}) Speed must be greater than 0.")
+
+    def new_waypoint(
+        self,
+        coord: Coord,
+        *,
+        bezier_control: tuple[Coord, ...] | Coord | None = None,
+        id: str = "",
+    ) -> Waypoint:
+        """Creates a new Waypoint and appends adds it to the Path.
 
         Args:
-            dimension (int): The longest dimension.
+            id (str): Unique identifier for the waypoint. Used to query for the waypoint.
+            coord (Coord): coordinate
+            bezier_control (tuple[Coord, ...] | Coord | None): coordinate of the control point for a bezier curve. Defaults to None.
 
         Returns:
-            int: The gap that is closest to 20% of the dimension length.
+            Waypoint: The new waypoint.
         """
-        potential_gaps: list[int] = []
-        dimension = dimension - 2
-        if dimension <= 0:
-            return 0
-        for i in range(dimension, 4, -1):
-            if dimension % i <= 1:
-                potential_gaps.append(i)
-        if not potential_gaps:
-            return 4
-        return min(potential_gaps, key=lambda x: abs(x - dimension // 5))
-
-    def _build(self) -> None:
-        grid_gradient = graphics.Gradient(*self._config.grid_gradient_stops, steps=self._config.grid_gradient_steps)
-        grid_gradient_mapping = grid_gradient.build_coordinate_color_mapping(
-            self._terminal.output_area.top, self._terminal.output_area.right, self._config.grid_gradient_direction
-        )
-        text_gradient = graphics.Gradient(*self._config.text_gradient_stops, steps=self._config.text_gradient_steps)
-        text_gradient_mapping = text_gradient.build_coordinate_color_mapping(
-            self._terminal.output_area.top, self._terminal.output_area.right, self._config.text_gradient_direction
-        )
+        if not id:
+            found_unique = False
+            current_id = len(self.waypoints)
+            while not found_unique:
+                id = f"{len(self.waypoints)}"
+                if id not in self.waypoint_lookup:
+                    found_unique = True
+                else:
+                    current_id += 1
+        new_waypoint = Waypoint(id, coord, bezier_control=bezier_control)
+        self._add_waypoint_to_path(new_waypoint)
+        return new_waypoint
 
-        self._grid_lines.append(
-            _GridLine(
-                self._terminal,
-                self._config,
-                Coord(self._terminal.output_area.left, self._terminal.output_area.bottom),
-                "horizontal",
-                grid_gradient_mapping,
-            )
-        )
-        self._grid_lines.append(
-            _GridLine(
-                self._terminal,
-                self._config,
-                Coord(self._terminal.output_area.left, self._terminal.output_area.top),
-                "horizontal",
-                grid_gradient_mapping,
+    def _add_waypoint_to_path(self, waypoint: Waypoint) -> None:
+        """Adds a waypoint to the path and updates the total distance and maximum steps.
+
+        Args:
+            waypoint (Waypoint): waypoint to add
+        """
+        self.waypoint_lookup[waypoint.waypoint_id] = waypoint
+        self.waypoints.append(waypoint)
+        if len(self.waypoints) < 2:
+            return
+
+        if waypoint.bezier_control:
+            distance_from_previous = geometry.find_length_of_bezier_curve(
+                self.waypoints[-2].coord, waypoint.bezier_control, waypoint.coord
             )
-        )
-        self._grid_lines.append(
-            _GridLine(
-                self._terminal,
-                self._config,
-                Coord(self._terminal.output_area.left, self._terminal.output_area.bottom),
-                "vertical",
-                grid_gradient_mapping,
+        else:
+            distance_from_previous = geometry.find_length_of_line(
+                self.waypoints[-2].coord,
+                waypoint.coord,
             )
-        )
-        self._grid_lines.append(
-            _GridLine(
-                self._terminal,
-                self._config,
-                Coord(self._terminal.output_area.right, self._terminal.output_area.bottom),
-                "vertical",
-                grid_gradient_mapping,
+        self.total_distance += distance_from_previous
+        self.segments.append(Segment(self.waypoints[-2], waypoint, distance_from_previous))
+        self.max_steps = round(self.total_distance / self.speed)
+
+    def query_waypoint(self, waypoint_id: str) -> Waypoint:
+        """Returns the waypoint with the given waypoint_id.
+
+        Args:
+            waypoint_id (str): waypoint_id
+
+        Returns:
+            Waypoint: The waypoint with the given waypoint_id.
+        """
+        waypoint = self.waypoint_lookup.get(waypoint_id, None)
+        if not waypoint:
+            raise ValueError(f"Waypoint with id {waypoint_id} not found.")
+        return waypoint
+
+    def step(self, event_handler: "base_character.EventHandler") -> Coord:
+        """
+        Progresses to the next step along the path and returns the coordinate at that step.
+
+        This method is called by the Motion.move() method. It calculates the next coordinate based on the current step,
+        total distance, bezier control points, and the easing function if provided. It also handles the triggering of segment enter and exit events.
+
+        Args:
+            event_handler (base_character.EventHandler): The EventHandler for the character.
+
+        Returns:
+            Coord: The next coordinate on the path.
+        """
+        if not self.max_steps or self.current_step >= self.max_steps or not self.total_distance:
+            # if the path has zero distance or there are no more steps, return the coordinate of the final waypoint in the path
+            return self.segments[-1].end.coord
+        else:
+            self.current_step += 1
+        if self.ease:
+            distance_factor = self.ease(self.current_step / self.max_steps)
+        else:
+            distance_factor = self.current_step / self.max_steps
+
+        distance_to_travel = distance_factor * self.total_distance
+        self.last_distance_reached = distance_to_travel
+        for segment in self.segments:
+            if distance_to_travel <= segment.distance:
+                active_segment = segment
+                if not segment.enter_event_triggered:
+                    segment.enter_event_triggered = True
+                    event_handler._handle_event(event_handler.Event.SEGMENT_ENTERED, segment.end)
+                break
+            distance_to_travel -= segment.distance
+            if not segment.exit_event_triggered:
+                segment.exit_event_triggered = True
+                event_handler._handle_event(event_handler.Event.SEGMENT_EXITED, segment.end)
+        else:  # if the distance_to_travel is further than the last waypoint, preserve the distance from the start of the final segment
+            active_segment = self.segments[-1]
+            distance_to_travel += active_segment.distance
+        if active_segment.distance == 0:
+            segment_distance_to_travel_factor = 0.0
+        else:
+            segment_distance_to_travel_factor = distance_to_travel / active_segment.distance
+
+        if active_segment.end.bezier_control:
+            next_coord = geometry.find_coord_on_bezier_curve(
+                active_segment.start.coord,
+                active_segment.end.bezier_control,
+                active_segment.end.coord,
+                segment_distance_to_travel_factor,
             )
-        )
-        column_indexes: list[int] = []
-        row_indexes: list[int] = []
-        if self._terminal.output_area.top > 2 * self._terminal.output_area.right:
-            row_gap = self._find_even_gap(self._terminal.output_area.top) + 1
-            column_gap = row_gap * 2
         else:
-            column_gap = self._find_even_gap(self._terminal.output_area.right) + 1
-            row_gap = column_gap // 2
+            next_coord = geometry.find_coord_on_line(
+                active_segment.start.coord, active_segment.end.coord, segment_distance_to_travel_factor
+            )
+
+        return next_coord
+
+    def __eq__(self, other: typing.Any) -> bool:
+        if not isinstance(other, Path):
+            return NotImplemented
+        return self.path_id == other.path_id
+
+    def __hash__(self):
+        return hash(self.path_id)
+
+
+class Motion:
+    """Motion class for managing the movement of a character.
 
-        for row_index in range(
-            self._terminal.output_area.bottom + row_gap, self._terminal.output_area.top, max(row_gap, 1)
-        ):
-            if self._terminal.output_area.top - row_index < 2:
+    Attributes:
+        paths (dict[str, Path]): dictionary of paths
+        character (base_character.EffectCharacter): The EffectCharacter to move.
+        current_coord (Coord): current coordinate
+        previous_coord (Coord): previous coordinate
+        active_path (Path | None): active path
+
+    Methods:
+        set_coordinate(coord: Coord) -> None:
+            Sets the current coordinate to the given coordinate.
+        new_path(speed: float = 1, ease: easing.EasingFunction | None = None, layer: int | None = None, hold_time: int = 0, loop: bool = False, id: str = "") -> Path:
+            Creates a new Path and adds it to the Motion.paths dictionary with the path_id as key.
+        query_path(path_id: str) -> Path:
+            Returns the path with the given path_id.
+        movement_is_complete() -> bool:
+            Returns whether the character has an active path.
+        chain_paths(paths: list[Path], loop=False):
+            Creates a chain of paths by registering activation events for each path such
+            that paths[n] activates paths[n+1] when reached. If loop is True, paths[-1] activates
+            paths[0] when reached.
+        activate_path(path: Path) -> None:
+            Activates the first waypoint in the path.
+        deactivate_path(path: Path) -> None:
+            Unsets the current path if the current path is path.
+        move() -> None:
+            Moves the character one step closer to the target position based on an easing function if present, otherwise linearly."""
+
+    def __init__(self, character: "base_character.EffectCharacter"):
+        """Initializes the Motion object with the given EffectCharacter.
+
+        Args:
+            character (base_character.EffectCharacter): The EffectCharacter to move.
+        """
+        self.paths: dict[str, Path] = {}
+        self.character = character
+        self.current_coord: Coord = Coord(character.input_coord.column, character.input_coord.row)
+        self.previous_coord: Coord = Coord(-1, -1)
+        self.active_path: Path | None = None
+
+    def set_coordinate(self, coord: Coord) -> None:
+        """Sets the current coordinate to the given coordinate.
+
+        Args:
+            coord (Coord): coordinate
+        """
+        self.current_coord = coord
+
+    def new_path(
+        self,
+        *,
+        speed: float = 1,
+        ease: easing.EasingFunction | None = None,
+        layer: int | None = None,
+        hold_time: int = 0,
+        loop: bool = False,
+        id: str = "",
+    ) -> Path:
+        """Creates a new Path and adds it to the Motion.paths dictionary with the path_id as key.
+
+        Args:
+            speed (float, optional): speed > 0. Defaults to 1.
+            ease (easing.EasingFunction | None, optional): easing function for character movement. Defaults to None.
+            layer (int | None, optional): layer to move the character to, if None, layer is unchanged. Defaults to None.
+            hold_time (int, optional): number of frames to hold the character at the end of the path. Defaults to 0.
+            loop (bool, optional): Whether the path should loop back to the beginning. Default is False.
+            id (str, optional): Unique identifier for the path. Used to query for the path. Defaults to "".
+
+        Raises:
+            ValueError: If a path with the provided id already exists.
+
+        Returns:
+            Path: The new path.
+        """
+        if not id:
+            found_unique = False
+            current_id = len(self.paths)
+            while not found_unique:
+                id = f"{len(self.paths)}"
+                if id not in self.paths:
+                    found_unique = True
+                else:
+                    current_id += 1
+        if id in self.paths:
+            raise ValueError(f"Path with id {id} already exists.")
+        new_path = Path(id, speed, ease, layer, hold_time, loop)
+        self.paths[id] = new_path
+        return new_path
+
+    def query_path(self, path_id: str) -> Path:
+        """Returns the path with the given path_id.
+
+        Args:
+            path_id (str): path_id
+
+        Returns:
+            Path: The path with the given path_id.
+        """
+        path = self.paths.get(path_id, None)
+        if not path:
+            raise ValueError(f"Path with id {path_id} not found.")
+        return path
+
+    def movement_is_complete(self) -> bool:
+        """Returns whether the character has an active path.
+
+        Returns:
+            bool: True if the character has no active path, False otherwise.
+        """
+        if self.active_path is None:
+            return True
+        return False
+
+    def _get_easing_factor(self, easing_func: easing.EasingFunction) -> float:
+        """Returns the percentage of total distance that should be moved based on the easing function.
+
+        Args:
+            easing_func (easing.EasingFunction): The easing function to use.
+
+        Returns:
+            float: The percentage of total distance to move.
+        """
+        if not self.active_path:
+            raise ValueError("No active path.")
+        elapsed_step_ratio = self.active_path.current_step / self.active_path.max_steps
+        return easing_func(elapsed_step_ratio)
+
+    def chain_paths(self, paths: list[Path], loop=False):
+        """Creates a chain of paths by registering activation events for each path such
+        that paths[n] activates paths[n+1] when reached. If loop is True, paths[-1] activates
+        paths[0] when reached.
+
+        Args:
+            paths (list[Path]): list of paths to chain
+            loop (bool, optional): Whether the chain should loop. Defaults to False.
+        """
+        if len(paths) < 2:
+            return
+        for i, path in enumerate(paths):
+            if i == 0:
                 continue
-            row_indexes.append(row_index)
-            self._grid_lines.append(
-                _GridLine(
-                    self._terminal,
-                    self._config,
-                    Coord(self._terminal.output_area.left, row_index),
-                    "horizontal",
-                    grid_gradient_mapping,
-                )
+            self.character.event_handler.register_event(
+                self.character.event_handler.Event.PATH_COMPLETE,
+                paths[i - 1],
+                self.character.event_handler.Action.ACTIVATE_PATH,
+                path,
             )
-        for column_index in range(
-            self._terminal.output_area.left + column_gap, self._terminal.output_area.right, max(column_gap, 1)
-        ):
-            if self._terminal.output_area.right - column_index < 2:
-                continue
-            column_indexes.append(column_index)
-            self._grid_lines.append(
-                _GridLine(
-                    self._terminal,
-                    self._config,
-                    Coord(column_index, self._terminal.output_area.bottom),
-                    "vertical",
-                    grid_gradient_mapping,
-                )
+        if loop:
+            self.character.event_handler.register_event(
+                self.character.event_handler.Event.PATH_COMPLETE,
+                paths[-1],
+                self.character.event_handler.Action.ACTIVATE_PATH,
+                paths[0],
+            )
+
+    def activate_path(self, path: Path) -> None:
+        """
+        Activates the first waypoint in the given path and updates the path's properties accordingly.
+
+        This method sets the active path to the given path, calculates the distance to the first waypoint,
+        and updates the total distance of the path. If the path has an origin segment, it removes it from
+        the segments list and subtracts its distance from the total distance. Then, it creates a new origin
+        segment from the current coordinate to the first waypoint and inserts it at the beginning of the segments list.
+
+        The method also resets the current step, hold time remaining, and max steps of the path based on the total distance
+        and speed. It ensures that the enter and exit events for each segment are not triggered. If the path has a layer,
+        it sets the character's layer to it. Finally, it triggers the PATH_ACTIVATED event for the character.
+
+        Args:
+            path (Path): The path to activate.
+        """
+        self.active_path = path
+        first_waypoint = self.active_path.waypoints[0]
+        if first_waypoint.bezier_control:
+            distance_to_first_waypoint = geometry.find_length_of_bezier_curve(
+                self.current_coord, first_waypoint.bezier_control, first_waypoint.coord
             )
-        row_indexes.append(self._terminal.output_area.top + 1)
-        column_indexes.append(self._terminal.output_area.right + 1)
-        prev_row_index = 1
-        for row_index in row_indexes:
-            prev_column_index = 1
-            for column_index in column_indexes:
-                coords_in_block: list[Coord] = []
-                if row_index == self._terminal.output_area.top:  # make sure the top row is included
-                    row_index += 1
-                for row in range(prev_row_index, row_index):
-                    for column in range(prev_column_index, column_index):
-                        coords_in_block.append(Coord(column, row))
-                characters_in_block: list[EffectCharacter] = []
-                for coord in coords_in_block:
-                    if coord in self._terminal.character_by_input_coord:
-                        characters_in_block.append(self._terminal.character_by_input_coord[coord])
-                if characters_in_block:
-                    self._pending_groups.append((len(self._pending_groups), characters_in_block))
-                prev_column_index = column_index
-            prev_row_index = row_index
-        for group_number, group in self._pending_groups:
-            self._group_tracker[group_number] = 0
-            for character in group:
-                dissolve_scn = character.animation.new_scene()
-                for _ in range(random.randint(15, 30)):
-                    dissolve_scn.add_frame(
-                        random.choice(self._config.text_generation_symbols),
-                        3,
-                        color=random.choice(text_gradient.spectrum),
-                    )
-                dissolve_scn.add_frame(character.input_symbol, 1, color=text_gradient_mapping[character.input_coord])
-                character.animation.activate_scene(dissolve_scn)
-                character.event_handler.register_event(
-                    EventHandler.Event.SCENE_COMPLETE,
-                    dissolve_scn,
-                    EventHandler.Action.CALLBACK,
-                    EventHandler.Callback(self._update_group_tracker, group_number),
-                )
-        random.shuffle(self._pending_groups)
-        self._phase = "grid_expand"
-        self._total_group_count = len(self._pending_groups)
-        if not self._total_group_count:
-            for character in self._terminal.get_characters():
-                self._terminal.set_character_visibility(character, True)
-                self._active_chars.append(character)
-        self._active_groups: int = 0
-
-    def _update_group_tracker(self, character: EffectCharacter, *args) -> None:
-        self._group_tracker[args[0]] -= 1
-
-    def __next__(self) -> str:
-        if self._pending_groups or self._active_chars or self._phase != "complete":
-            if self._phase == "grid_expand":
-                if not all([grid_line.is_extended() for grid_line in self._grid_lines]):
-                    for grid_line in self._grid_lines:
-                        if not grid_line.is_extended():
-                            grid_line.extend()
-                else:
-                    self._phase = "add_chars"
-            elif self._phase == "add_chars":
-                if (
-                    self._pending_groups
-                    and self._active_groups < self._total_group_count * self._config.max_active_blocks
-                ):
-                    group_number, next_group = self._pending_groups.pop(0)
-                    for char in next_group:
-                        self._terminal.set_character_visibility(char, True)
-                        self._active_chars.append(char)
-                        self._group_tracker[group_number] += 1
-                if not self._pending_groups and not self._active_chars and not self._active_groups:
-                    self._phase = "collapse"
-            elif self._phase == "collapse":
-                if not all([grid_line.is_collapsed() for grid_line in self._grid_lines]):
-                    for grid_line in self._grid_lines:
-                        if not grid_line.is_collapsed():
-                            grid_line.collapse()
-                else:
-                    self._phase = "complete"
-            for character in self._active_chars:
-                character.tick()
-
-            self._active_chars = [character for character in self._active_chars if character.is_active]
-            self._active_groups = 0
-            for _, active_count in self._group_tracker.items():
-                if active_count:
-                    self._active_groups += 1
-            return self._terminal.get_formatted_output_string()
         else:
-            raise StopIteration
+            distance_to_first_waypoint = geometry.find_length_of_line(
+                self.current_coord,
+                first_waypoint.coord,
+            )
+        self.active_path.total_distance += distance_to_first_waypoint
+        if self.active_path.origin_segment:
+            self.active_path.segments.pop(0)
+            self.active_path.total_distance -= self.active_path.origin_segment.distance
+        self.active_path.origin_segment = Segment(
+            Waypoint("origin", self.current_coord), first_waypoint, distance_to_first_waypoint
+        )
+        self.active_path.segments.insert(0, self.active_path.origin_segment)
+        self.active_path.current_step = 0
+        self.active_path.hold_time_remaining = self.active_path.hold_time
+        self.active_path.max_steps = round(self.active_path.total_distance / self.active_path.speed)
+        for segment in self.active_path.segments:
+            segment.enter_event_triggered = False
+            segment.exit_event_triggered = False
+        if self.active_path.layer is not None:
+            self.character.layer = self.active_path.layer
+        self.character.event_handler._handle_event(self.character.event_handler.Event.PATH_ACTIVATED, self.active_path)
 
+    def deactivate_path(self, path: Path) -> None:
+        """Set the active path to None if the active path is the given path.
 
-class SynthGrid(BaseEffect[SynthGridConfig]):
-    """Effect that creates a grid where blocks of characters dissolved into the input characters."""
+        Args:
+            path (Path): the Path to deactivate
+        """
+        if self.active_path and self.active_path is path:
+            self.active_path = None
 
-    _config_cls = SynthGridConfig
-    _iterator_cls = SynthGridIterator
+    def move(self) -> None:
+        """
+        Moves the character along the active path.
 
-    def __init__(self, input_data: str) -> None:
-        super().__init__(input_data)
+        The character's current coordinate is updated to the next step in the active path. If the active path is completed,
+        an event is triggered based on whether the path is set to loop or not. If the path is set to loop, the path is
+        deactivated and then reactivated to start from the beginning. If not, the path is simply deactivated and a
+        PATH_COMPLETE event is triggered.
+
+        If the path has a hold time, the character will pause at the end of the path for the specified duration. During
+        this hold time, a PATH_HOLDING event is triggered on the first frame, and the hold time is decremented on each
+        subsequent frame until it reaches zero.
+
+        If there is no active path or if the active path has no segments, the character does not move.
+
+        The character's previous coordinate is preserved before moving to allow for clearing the location in the terminal.
+        """
+        # preserve previous coordinate to allow for clearing the location in the terminal
+        self.previous_coord = Coord(self.current_coord.column, self.current_coord.row)
+
+        if not self.active_path or not self.active_path.segments:
+            return
+        self.current_coord = self.active_path.step(self.character.event_handler)
+        if self.active_path.current_step == self.active_path.max_steps:
+            if self.active_path.hold_time and self.active_path.hold_time_remaining == self.active_path.hold_time:
+                self.character.event_handler._handle_event(
+                    self.character.event_handler.Event.PATH_HOLDING, self.active_path
+                )
+                self.active_path.hold_time_remaining -= 1
+                return
+            elif self.active_path.hold_time_remaining:
+                self.active_path.hold_time_remaining -= 1
+                return
+            if self.active_path.loop and len(self.active_path.segments) > 1:
+                looping_path = self.active_path
+                self.deactivate_path(self.active_path)
+                self.activate_path(looping_path)
+            else:
+                self.completed_path = self.active_path
+                self.deactivate_path(self.active_path)
+                self.character.event_handler._handle_event(
+                    self.character.event_handler.Event.PATH_COMPLETE, self.completed_path
+                )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_unstable.py` & `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_unstable.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,127 +1,132 @@
+"""Spawns characters jumbled, explodes them to the edge of the output area, then reassembles them.
+
+Classes:
+    Unstable: Spawns characters jumbled, explodes them to the edge of the output area, then reassembles them.
+    UnstableConfig: Configuration for the Unstable effect.
+    UnstableIterator: Effect iterator for the Unstable effect. Does not normally need to be called directly.
+"""
+
 import random
 import typing
 from dataclasses import dataclass
 
-import terminaltexteffects.utils.arg_validators as arg_validators
-from terminaltexteffects.base_character import EffectCharacter
-from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
+import terminaltexteffects.utils.argvalidators as argvalidators
+from terminaltexteffects.engine.base_character import EffectCharacter
+from terminaltexteffects.engine.base_effect import BaseEffect, BaseEffectIterator
 from terminaltexteffects.utils import easing, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 from terminaltexteffects.utils.geometry import Coord
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
     return Unstable, UnstableConfig
 
 
 @argclass(
     name="unstable",
     help="Spawn characters jumbled, explode them to the edge of the output area, then reassemble them in the correct layout.",
     description="unstable | Spawn characters jumbled, explode them to the edge of the output area, then reassemble them in the correct layout.",
-    epilog=f"""{arg_validators.EASING_EPILOG}
+    epilog=f"""{argvalidators.EASING_EPILOG}
     
     Example: terminaltexteffects unstable --unstable-color ff9200 --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --explosion-ease OUT_EXPO --explosion-speed 0.75 --reassembly-ease OUT_EXPO --reassembly-speed 0.75""",
 )
 @dataclass
 class UnstableConfig(ArgsDataClass):
     """Configuration for the Unstable effect.
 
     Attributes:
         unstable_color (graphics.Color): Color transitioned to as the characters become unstable.
-        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
-        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
-        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation. Valid values are n > 0.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the final gradient.
         explosion_ease (easing.EasingFunction): Easing function to use for character movement during the explosion.
-        explosion_speed (float): Speed of characters during explosion. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.
+        explosion_speed (float): Speed of characters during explosion. Valid values are n > 0.
         reassembly_ease (easing.EasingFunction): Easing function to use for character reassembly.
-        reassembly_speed (float): Speed of characters during reassembly.
+        reassembly_speed (float): Speed of characters during reassembly. Valid values are n > 0.
     """
 
     unstable_color: graphics.Color = ArgField(
         cmd_name=["--unstable-color"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         default="ff9200",
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Color transitioned to as the characters become unstable.",
     )  # type: ignore[assignment]
     "graphics.Color : Color transitioned to as the characters become unstable."
 
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("8A008A", "00D1FF", "FFFFFF"),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
-    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+    "tuple[graphics.Color, ...] : Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color."
 
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name=["--final-gradient-steps"],
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
     "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
 
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
-        type_parser=arg_validators.GradientDirection.type_parser,
+        type_parser=argvalidators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.VERTICAL,
-        metavar=arg_validators.GradientDirection.METAVAR,
-        help="Direction of the gradient for the final color.",
+        metavar=argvalidators.GradientDirection.METAVAR,
+        help="Direction of the final gradient.",
     )  # type: ignore[assignment]
-    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+    "graphics.Gradient.Direction : Direction of the final gradient."
 
     explosion_ease: easing.EasingFunction = ArgField(
         cmd_name=["--explosion-ease"],
-        type_parser=arg_validators.Ease.type_parser,
+        type_parser=argvalidators.Ease.type_parser,
         default=easing.out_expo,
         help="Easing function to use for character movement during the explosion.",
     )  # type: ignore[assignment]
     "easing.EasingFunction : Easing function to use for character movement during the explosion."
 
     explosion_speed: float = ArgField(
         cmd_name=["--explosion-speed"],
-        type_parser=arg_validators.PositiveFloat.type_parser,
+        type_parser=argvalidators.PositiveFloat.type_parser,
         default=0.75,
-        metavar=arg_validators.PositiveFloat.METAVAR,
-        help="Speed of characters during explosion. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.",
+        metavar=argvalidators.PositiveFloat.METAVAR,
+        help="Speed of characters during explosion. ",
     )  # type: ignore[assignment]
-    "float : Speed of characters during explosion. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect."
+    "float : Speed of characters during explosion. "
 
     reassembly_ease: easing.EasingFunction = ArgField(
         cmd_name=["--reassembly-ease"],
-        type_parser=arg_validators.Ease.type_parser,
+        type_parser=argvalidators.Ease.type_parser,
         default=easing.out_expo,
         help="Easing function to use for character reassembly.",
     )  # type: ignore[assignment]
     "easing.EasingFunction : Easing function to use for character reassembly."
 
     reassembly_speed: float = ArgField(
         cmd_name=["--reassembly-speed"],
-        type_parser=arg_validators.PositiveFloat.type_parser,
+        type_parser=argvalidators.PositiveFloat.type_parser,
         default=0.75,
-        metavar=arg_validators.PositiveFloat.METAVAR,
-        help="Speed of characters during reassembly. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.",
+        metavar=argvalidators.PositiveFloat.METAVAR,
+        help="Speed of characters during reassembly. ",
     )  # type: ignore[assignment]
     "float : Speed of characters during reassembly."
 
     @classmethod
     def get_effect_class(cls):
         return Unstable
 
 
 class UnstableIterator(BaseEffectIterator[UnstableConfig]):
-    """Effect that spawns characters jumbled, explodes them to the edge of the output area,
-    then reassembles them in the correct layout."""
-
     def __init__(self, effect: "Unstable") -> None:
         super().__init__(effect)
         self._pending_chars: list[EffectCharacter] = []
         self._active_chars: list[EffectCharacter] = []
         self._jumbled_coords: dict[EffectCharacter, Coord] = dict()
         self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
         self._build()
@@ -249,12 +254,23 @@
         if next_frame is not None:
             return next_frame
         else:
             raise StopIteration
 
 
 class Unstable(BaseEffect[UnstableConfig]):
+    """Spawns characters jumbled, explodes them to the edge of the output area, then reassembles them.
+
+    Attributes:
+        effect_config (UnstableConfig): Configuration for the effect.
+        terminal_config (TerminalConfig): Configuration for the terminal.
+    """
+
     _config_cls = UnstableConfig
     _iterator_cls = UnstableIterator
 
     def __init__(self, input_data: str) -> None:
+        """Initialize the effect with the provided input data.
+
+        Args:
+            input_data (str): The input data to use for the effect."""
         super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_verticalslice.py` & `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_verticalslice.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,95 +1,101 @@
+"""Slices the input in half vertically and slides it into place from opposite directions.
+
+Classes:
+    VerticalSlice: Slices the input in half vertically and slides it into place from opposite directions.
+    VerticalSliceConfig: Configuration for the VerticalSlice effect.
+    VerticalSliceIterator: Effect iterator for the effect. Does not normally need to be called directly.
+"""
+
 import typing
 from dataclasses import dataclass
 
-from terminaltexteffects.base_character import EffectCharacter
-from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
-from terminaltexteffects.utils import arg_validators, easing, graphics
+from terminaltexteffects.engine.base_character import EffectCharacter
+from terminaltexteffects.engine.base_effect import BaseEffect, BaseEffectIterator
+from terminaltexteffects.utils import argvalidators, easing, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 from terminaltexteffects.utils.geometry import Coord
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
     return VerticalSlice, VerticalSliceConfig
 
 
 @argclass(
     name="verticalslice",
     help="Slices the input in half vertically and slides it into place from opposite directions.",
     description="verticalslice | Slices the input in half vertically and slides it into place from opposite directions.",
-    epilog=f"""{arg_validators.EASING_EPILOG}
+    epilog=f"""{argvalidators.EASING_EPILOG}
     
 Example: terminaltexteffects verticalslice --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --movement-speed 0.15 --movement-easing IN_OUT_EXPO""",
 )
 @dataclass
 class VerticalSliceConfig(ArgsDataClass):
     """Configuration for the VerticalSlice effect.
 
     Attributes:
-        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
-        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
-        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
-        movement_speed (float): Movement speed of the characters. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation. Valid values are n > 0.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the final gradient.
+        movement_speed (float): Movement speed of the characters. Valid values are n > 0.
         movement_easing (easing.EasingFunction): Easing function to use for character movement.
     """
 
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("8A008A", "00D1FF", "FFFFFF"),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
-    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+    "tuple[graphics.Color, ...] : Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color."
 
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name="--final-gradient-steps",
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
     "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
 
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
-        type_parser=arg_validators.GradientDirection.type_parser,
+        type_parser=argvalidators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.VERTICAL,
-        metavar=arg_validators.GradientDirection.METAVAR,
-        help="Direction of the gradient for the final color.",
+        metavar=argvalidators.GradientDirection.METAVAR,
+        help="Direction of the final gradient.",
     )  # type: ignore[assignment]
-    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+    "graphics.Gradient.Direction : Direction of the final gradient."
 
     movement_speed: float = ArgField(
         cmd_name="--movement-speed",
-        type_parser=arg_validators.PositiveFloat.type_parser,
+        type_parser=argvalidators.PositiveFloat.type_parser,
         default=0.15,
-        metavar=arg_validators.PositiveFloat.METAVAR,
-        help="Movement speed of the characters. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.",
+        metavar=argvalidators.PositiveFloat.METAVAR,
+        help="Movement speed of the characters. ",
     )  # type: ignore[assignment]
-    "float : Movement speed of the characters. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect."
+    "float : Movement speed of the characters. "
 
     movement_easing: easing.EasingFunction = ArgField(
         cmd_name="--movement-easing",
-        type_parser=arg_validators.Ease.type_parser,
+        type_parser=argvalidators.Ease.type_parser,
         default=easing.in_out_expo,
         help="Easing function to use for character movement.",
     )  # type: ignore[assignment]
     "easing.EasingFunction : Easing function to use for character movement."
 
     @classmethod
     def get_effect_class(cls):
         return VerticalSlice
 
 
 class VerticalSliceIterator(BaseEffectIterator[VerticalSliceConfig]):
-    """Effect that slices the input in half vertically and slides it into place from opposite directions."""
-
     def __init__(self, effect: "VerticalSlice") -> None:
         super().__init__(effect)
         self._pending_chars: list[EffectCharacter] = []
         self._active_chars: list[EffectCharacter] = []
         self._new_rows: list[list[EffectCharacter]] = []
         self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
         self._build()
@@ -144,14 +150,23 @@
             self._active_chars = [character for character in self._active_chars if character.is_active]
             return self._terminal.get_formatted_output_string()
         else:
             raise StopIteration
 
 
 class VerticalSlice(BaseEffect[VerticalSliceConfig]):
-    """Effect that slices the input in half vertically and slides it into place from opposite directions."""
+    """Slices the input in half vertically and slides it into place from opposite directions.
+
+    Attributes:
+        effect_config (VerticalSliceConfig): Configuration for the effect.
+        terminal_config (TerminalConfig): Configuration for the terminal.
+    """
 
     _config_cls = VerticalSliceConfig
     _iterator_cls = VerticalSliceIterator
 
     def __init__(self, input_data: str) -> None:
+        """Initialize the effect with the provided input data.
+
+        Args:
+            input_data (str): The input data to use for the effect."""
         super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_vhstape.py` & `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_vhstape.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,24 @@
+"""Lines of characters glitch left and right and lose detail like an old VHS tape.
+
+Classes:
+    VHSTape: Lines of characters glitch left and right and lose detail like an old VHS tape.
+    VHSTapeConfig: Configuration for the VHSTape effect.
+    VHSTapeIterator: Effect iterator for the VHSTape effect. Does not normally need to be called directly.
+"""
+
 import random
 import typing
 from dataclasses import dataclass
 
-import terminaltexteffects.utils.arg_validators as arg_validators
-from terminaltexteffects.base_character import EffectCharacter, EventHandler
-from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
-from terminaltexteffects.utils import animation, graphics
+import terminaltexteffects.utils.argvalidators as argvalidators
+from terminaltexteffects.engine import animation
+from terminaltexteffects.engine.base_character import EffectCharacter, EventHandler
+from terminaltexteffects.engine.base_effect import BaseEffect, BaseEffectIterator
+from terminaltexteffects.utils import graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 from terminaltexteffects.utils.geometry import Coord
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
     return VHSTape, VHSTapeConfig
 
@@ -21,310 +30,262 @@
     epilog="""Example: terminaltexteffects vhstape --final-gradient-stops ab48ff e7b2b2 fffebd --final-gradient-steps 12 --glitch-line-colors ffffff ff0000 00ff00 0000ff ffffff --glitch-wave-colors ffffff ff0000 00ff00 0000ff ffffff --noise-colors 1e1e1f 3c3b3d 6d6c70 a2a1a6 cbc9cf ffffff --glitch-line-chance 0.05 --noise-chance 0.004 --total-glitch-time 1000""",
 )
 @dataclass
 class VHSTapeConfig(ArgsDataClass):
     """Configuration for the VHSTape effect.
 
     Attributes:
-        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
-        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
-        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation. Valid values are n > 0.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the final gradient.
         glitch_line_colors (tuple[graphics.Color, ...]): Tuple of colors for the characters when a single line is glitching. Colors are applied in order as an animation.
         glitch_wave_colors (tuple[graphics.Color, ...]): Tuple of colors for the characters in lines that are part of the glitch wave. Colors are applied in order as an animation.
         noise_colors (tuple[graphics.Color, ...]): Tuple of colors for the characters during the noise phase.
         glitch_line_chance (float): Chance that a line will glitch on any given frame.
-        noise_chance (float): Chance that all characters will experience noise on any given frame.
-        total_glitch_time (int): Total time, animation steps, that the glitching phase will last."""
+        noise_chance (float): Chance that all characters will experience noise on any given frame. Valid values are 0 <= n <= 1.
+        total_glitch_time (int): Total time, in frames, that the glitching phase will last. Valid values are n > 0."""
 
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("ab48ff", "e7b2b2", "fffebd"),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
-    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+    "tuple[graphics.Color, ...] : Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color."
 
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name="--final-gradient-steps",
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
     "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
 
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
-        type_parser=arg_validators.GradientDirection.type_parser,
+        type_parser=argvalidators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.VERTICAL,
-        metavar=arg_validators.GradientDirection.METAVAR,
-        help="Direction of the gradient for the final color.",
+        metavar=argvalidators.GradientDirection.METAVAR,
+        help="Direction of the final gradient.",
     )  # type: ignore[assignment]
-    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+    "graphics.Gradient.Direction : Direction of the final gradient."
 
     glitch_line_colors: tuple[graphics.Color, ...] = ArgField(
         cmd_name="--glitch-line-colors",
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("ffffff", "ff0000", "00ff00", "0000ff", "ffffff"),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the characters when a single line is glitching. Colors are applied in order as an animation.",
     )  # type: ignore[assignment]
     "tuple[graphics.Color, ...] : Tuple of colors for the characters when a single line is glitching. Colors are applied in order as an animation."
 
     glitch_wave_colors: tuple[graphics.Color, ...] = ArgField(
         cmd_name="--glitch-wave-colors",
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("ffffff", "ff0000", "00ff00", "0000ff", "ffffff"),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the characters in lines that are part of the glitch wave. Colors are applied in order as an animation.",
     )  # type: ignore[assignment]
     "tuple[graphics.Color, ...] : Tuple of colors for the characters in lines that are part of the glitch wave. Colors are applied in order as an animation."
 
     noise_colors: tuple[graphics.Color, ...] = ArgField(
         cmd_name="--noise-colors",
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("1e1e1f", "3c3b3d", "6d6c70", "a2a1a6", "cbc9cf", "ffffff"),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the characters during the noise phase.",
     )  # type: ignore[assignment]
     "tuple[graphics.Color, ...] : Tuple of colors for the characters during the noise phase."
 
     glitch_line_chance: float = ArgField(
         cmd_name="--glitch-line-chance",
-        type_parser=arg_validators.Ratio.type_parser,
+        type_parser=argvalidators.Ratio.type_parser,
         default=0.05,
-        metavar=arg_validators.Ratio.METAVAR,
+        metavar=argvalidators.Ratio.METAVAR,
         help="Chance that a line will glitch on any given frame.",
     )  # type: ignore[assignment]
     "float : Chance that a line will glitch on any given frame."
 
     noise_chance: float = ArgField(
         cmd_name="--noise-chance",
-        type_parser=arg_validators.Ratio.type_parser,
+        type_parser=argvalidators.Ratio.type_parser,
         default=0.004,
-        metavar=arg_validators.Ratio.METAVAR,
+        metavar=argvalidators.Ratio.METAVAR,
         help="Chance that all characters will experience noise on any given frame.",
     )  # type: ignore[assignment]
     "float : Chance that all characters will experience noise on any given frame."
 
     total_glitch_time: int = ArgField(
         cmd_name="--total-glitch-time",
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         default=1000,
-        metavar=arg_validators.PositiveInt.METAVAR,
-        help="Total time, animation steps, that the glitching phase will last.",
+        metavar=argvalidators.PositiveInt.METAVAR,
+        help="Total time, frames, that the glitching phase will last.",
     )  # type: ignore[assignment]
-    "int : Total time, animation steps, that the glitching phase will last."
+    "int : Total time, frames, that the glitching phase will last."
 
     @classmethod
     def get_effect_class(cls):
         return VHSTape
 
 
-class _Line:
-    """
-    Represents a line of characters with various effects.
-
-    Args:
-        characters (list[EffectCharacter]): List of EffectCharacter objects representing the characters in the line.
-        args (argparse.Namespace): Namespace object containing command-line arguments.
-
-    Attributes:
-        characters (list[EffectCharacter]): List of EffectCharacter objects representing the characters in the line.
-        args (argparse.Namespace): Namespace object containing command-line arguments.
-
-    Methods:
-        build_line_effects(): Builds the line effects for each character.
-        snow(): Activates the snow animation for each character.
-        set_hold_time(hold_time: int): Sets the hold time for glitch waypoints for each character.
-        glitch(final=False): Activates the glitch animation for each character.
-        restore(): Activates the restore animation for each character.
-        activate_waypoint(waypoint_id: str): Activates a specific waypoint for each character.
-        line_movement_complete(): Checks if the movement of all characters in the line is complete.
-
-    """
-
-    def __init__(
-        self,
-        characters: list[EffectCharacter],
-        args: VHSTapeConfig,
-        character_final_color_map: dict[EffectCharacter, graphics.Color],
-    ) -> None:
-        self.characters = characters
-        self.args = args
-        self.character_final_color_map = character_final_color_map
-        self.build_line_effects()
-
-    def build_line_effects(self) -> None:
-        glitch_line_colors = self.args.glitch_line_colors
-        snow_chars = ["#", "*", ".", ":"]
-        noise_colors = self.args.noise_colors
-        offset = random.randint(4, 25)
-        direction = random.choice((-1, 1))
-        hold_time = random.randint(1, 50)
-        for character in self.characters:
-            # make glitch and restore waypoints
-            glitch_path = character.motion.new_path(id="glitch", speed=2, hold_time=hold_time)
-            glitch_path.new_waypoint(
-                Coord(character.input_coord.column + (offset * direction), character.input_coord.row),
-                id="glitch",
-            )
-            restore_path = character.motion.new_path(id="restore", speed=2)
-            restore_path.new_waypoint(character.input_coord, id="restore")
-            # make glitch wave waypoints
-            glitch_wave_mid_path = character.motion.new_path(id="glitch_wave_mid", speed=2)
-            glitch_wave_mid_path.new_waypoint(
-                Coord(character.input_coord.column + 8, character.input_coord.row), id="glitch_wave_mid"
-            )
-            glitch_wave_end_path = character.motion.new_path(id="glitch_wave_end", speed=2)
-            glitch_wave_end_path.new_waypoint(
-                Coord(character.input_coord.column + 14, character.input_coord.row), id="glitch_wave_end"
-            )
-
-            # make glitch scenes
-            base_scn = character.animation.new_scene(id="base")
-            base_scn.add_frame(character.input_symbol, duration=1, color=self.character_final_color_map[character])
-            glitch_scn_forward = character.animation.new_scene(id="rgb_glitch_fwd", sync=animation.SyncMetric.STEP)
-            for color in glitch_line_colors:
-                glitch_scn_forward.add_frame(character.input_symbol, duration=1, color=color)
-            glitch_scn_backward = character.animation.new_scene(id="rgb_glitch_bwd", sync=animation.SyncMetric.STEP)
-            for color in glitch_line_colors[::-1]:
-                glitch_scn_backward.add_frame(character.input_symbol, duration=1, color=color)
-            snow_scn = character.animation.new_scene(id="snow")
-            for _ in range(25):
-                snow_scn.add_frame(random.choice(snow_chars), duration=2, color=random.choice(noise_colors))
-            snow_scn.add_frame(character.input_symbol, duration=1, color=self.character_final_color_map[character])
-            final_snow_scn = character.animation.new_scene(id="final_snow")
-            final_redraw_scn = character.animation.new_scene(id="final_redraw")
-            final_redraw_scn.add_frame("█", duration=10, color="ffffff")
-            final_redraw_scn.add_frame(
-                character.input_symbol, duration=1, color=self.character_final_color_map[character]
-            )
-
-            for _ in range(50):
-                final_snow_scn.add_frame(random.choice(snow_chars), duration=2, color=random.choice(noise_colors))
-            # register events
-            character.event_handler.register_event(
-                EventHandler.Event.PATH_COMPLETE, glitch_path, EventHandler.Action.ACTIVATE_PATH, restore_path
-            )
-            character.event_handler.register_event(
-                EventHandler.Event.PATH_ACTIVATED,
-                glitch_path,
-                EventHandler.Action.ACTIVATE_SCENE,
-                glitch_scn_forward,
-            )
-            character.event_handler.register_event(
-                EventHandler.Event.PATH_ACTIVATED,
-                restore_path,
-                EventHandler.Action.ACTIVATE_SCENE,
-                glitch_scn_backward,
-            )
-            character.event_handler.register_event(
-                EventHandler.Event.PATH_ACTIVATED,
-                glitch_wave_mid_path,
-                EventHandler.Action.ACTIVATE_SCENE,
-                glitch_scn_forward,
-            )
-            character.event_handler.register_event(
-                EventHandler.Event.PATH_ACTIVATED,
-                glitch_wave_end_path,
-                EventHandler.Action.ACTIVATE_SCENE,
-                glitch_scn_forward,
-            )
-            character.event_handler.register_event(
-                EventHandler.Event.SCENE_COMPLETE, glitch_scn_backward, EventHandler.Action.ACTIVATE_SCENE, base_scn
-            )
-
-    def snow(self) -> None:
-        """
-        Activates the snow animation for each character in the effect.
-        """
-        for character in self.characters:
-            character.animation.activate_scene(character.animation.query_scene("snow"))
-
-    def set_hold_time(self, hold_time: int) -> None:
-        """
-        Set the hold time for each character's glitch motion.
-
-        Args:
-            hold_time (int): The hold time in animation steps.
-
-        Returns:
-            None
-        """
-        for character in self.characters:
-            character.motion.paths["glitch"].hold_time = hold_time
-
-    def glitch(self, final=False) -> None:
-        """
-        Apply glitch effect to the characters.
-
-        Args:
-            final (bool): If True, set hold_time to 0 for glitch and restore waypoints.
+class VHSTapeIterator(BaseEffectIterator[VHSTapeConfig]):
+    class _Line:
+        def __init__(
+            self,
+            characters: list[EffectCharacter],
+            args: VHSTapeConfig,
+            character_final_color_map: dict[EffectCharacter, graphics.Color],
+        ) -> None:
+            self.characters = characters
+            self.args = args
+            self.character_final_color_map = character_final_color_map
+            self.build_line_effects()
+
+        def build_line_effects(self) -> None:
+            glitch_line_colors = self.args.glitch_line_colors
+            snow_chars = ["#", "*", ".", ":"]
+            noise_colors = self.args.noise_colors
+            offset = random.randint(4, 25)
+            direction = random.choice((-1, 1))
+            hold_time = random.randint(1, 50)
+            for character in self.characters:
+                # make glitch and restore waypoints
+                glitch_path = character.motion.new_path(id="glitch", speed=2, hold_time=hold_time)
+                glitch_path.new_waypoint(
+                    Coord(character.input_coord.column + (offset * direction), character.input_coord.row),
+                    id="glitch",
+                )
+                restore_path = character.motion.new_path(id="restore", speed=2)
+                restore_path.new_waypoint(character.input_coord, id="restore")
+                # make glitch wave waypoints
+                glitch_wave_mid_path = character.motion.new_path(id="glitch_wave_mid", speed=2)
+                glitch_wave_mid_path.new_waypoint(
+                    Coord(character.input_coord.column + 8, character.input_coord.row), id="glitch_wave_mid"
+                )
+                glitch_wave_end_path = character.motion.new_path(id="glitch_wave_end", speed=2)
+                glitch_wave_end_path.new_waypoint(
+                    Coord(character.input_coord.column + 14, character.input_coord.row), id="glitch_wave_end"
+                )
 
-        Returns:
-            None
-        """
-        for character in self.characters:
-            glitch_path = character.motion.query_path("glitch")
-            restore_path = character.motion.query_path("restore")
-            if final:
-                glitch_path.hold_time = 0
-                restore_path.hold_time = 0
-            glitch_path.speed = 40 / random.randint(20, 40)
-            restore_path.speed = 40 / random.randint(20, 40)
-            character.motion.activate_path(glitch_path)
-
-    def restore(self) -> None:
-        for character in self.characters:
-            restore_path = character.motion.query_path("restore")
-            restore_path.speed = 40 / random.randint(20, 40)
-            character.motion.activate_path(restore_path)
-
-    def activate_path(self, path_id: str) -> None:
-        for character in self.characters:
-            character.motion.activate_path(character.motion.query_path(path_id))
+                # make glitch scenes
+                base_scn = character.animation.new_scene(id="base")
+                base_scn.add_frame(character.input_symbol, duration=1, color=self.character_final_color_map[character])
+                glitch_scn_forward = character.animation.new_scene(id="rgb_glitch_fwd", sync=animation.SyncMetric.STEP)
+                for color in glitch_line_colors:
+                    glitch_scn_forward.add_frame(character.input_symbol, duration=1, color=color)
+                glitch_scn_backward = character.animation.new_scene(id="rgb_glitch_bwd", sync=animation.SyncMetric.STEP)
+                for color in glitch_line_colors[::-1]:
+                    glitch_scn_backward.add_frame(character.input_symbol, duration=1, color=color)
+                snow_scn = character.animation.new_scene(id="snow")
+                for _ in range(25):
+                    snow_scn.add_frame(random.choice(snow_chars), duration=2, color=random.choice(noise_colors))
+                snow_scn.add_frame(character.input_symbol, duration=1, color=self.character_final_color_map[character])
+                final_snow_scn = character.animation.new_scene(id="final_snow")
+                final_redraw_scn = character.animation.new_scene(id="final_redraw")
+                final_redraw_scn.add_frame("█", duration=10, color="ffffff")
+                final_redraw_scn.add_frame(
+                    character.input_symbol, duration=1, color=self.character_final_color_map[character]
+                )
 
-    def line_movement_complete(self):
-        return all(character.motion.movement_is_complete() for character in self.characters)
+                for _ in range(50):
+                    final_snow_scn.add_frame(random.choice(snow_chars), duration=2, color=random.choice(noise_colors))
+                # register events
+                character.event_handler.register_event(
+                    EventHandler.Event.PATH_COMPLETE, glitch_path, EventHandler.Action.ACTIVATE_PATH, restore_path
+                )
+                character.event_handler.register_event(
+                    EventHandler.Event.PATH_ACTIVATED,
+                    glitch_path,
+                    EventHandler.Action.ACTIVATE_SCENE,
+                    glitch_scn_forward,
+                )
+                character.event_handler.register_event(
+                    EventHandler.Event.PATH_ACTIVATED,
+                    restore_path,
+                    EventHandler.Action.ACTIVATE_SCENE,
+                    glitch_scn_backward,
+                )
+                character.event_handler.register_event(
+                    EventHandler.Event.PATH_ACTIVATED,
+                    glitch_wave_mid_path,
+                    EventHandler.Action.ACTIVATE_SCENE,
+                    glitch_scn_forward,
+                )
+                character.event_handler.register_event(
+                    EventHandler.Event.PATH_ACTIVATED,
+                    glitch_wave_end_path,
+                    EventHandler.Action.ACTIVATE_SCENE,
+                    glitch_scn_forward,
+                )
+                character.event_handler.register_event(
+                    EventHandler.Event.SCENE_COMPLETE, glitch_scn_backward, EventHandler.Action.ACTIVATE_SCENE, base_scn
+                )
 
+        def snow(self) -> None:
+            for character in self.characters:
+                character.animation.activate_scene(character.animation.query_scene("snow"))
+
+        def set_hold_time(self, hold_time: int) -> None:
+            for character in self.characters:
+                character.motion.paths["glitch"].hold_time = hold_time
+
+        def glitch(self, final=False) -> None:
+            for character in self.characters:
+                glitch_path = character.motion.query_path("glitch")
+                restore_path = character.motion.query_path("restore")
+                if final:
+                    glitch_path.hold_time = 0
+                    restore_path.hold_time = 0
+                glitch_path.speed = 40 / random.randint(20, 40)
+                restore_path.speed = 40 / random.randint(20, 40)
+                character.motion.activate_path(glitch_path)
+
+        def restore(self) -> None:
+            for character in self.characters:
+                restore_path = character.motion.query_path("restore")
+                restore_path.speed = 40 / random.randint(20, 40)
+                character.motion.activate_path(restore_path)
+
+        def activate_path(self, path_id: str) -> None:
+            for character in self.characters:
+                character.motion.activate_path(character.motion.query_path(path_id))
 
-class VHSTapeIterator(BaseEffectIterator[VHSTapeConfig]):
-    """
-    Represents a VHS tape effect for terminal text.
-    """
+        def line_movement_complete(self):
+            return all(character.motion.movement_is_complete() for character in self.characters)
 
     def __init__(self, effect: "VHSTape") -> None:
         super().__init__(effect)
         self._pending_chars: list[EffectCharacter] = []
         self._active_chars: list[EffectCharacter] = []
-        self._lines: dict[int, _Line] = {}
+        self._lines: dict[int, VHSTapeIterator._Line] = {}
         self._active_glitch_wave_top: int | None = None
-        self._active_glitch_wave_lines: list[_Line] = []
-        self._active_glitch_lines: list[_Line] = []
+        self._active_glitch_wave_lines: list[VHSTapeIterator._Line] = []
+        self._active_glitch_lines: list[VHSTapeIterator._Line] = []
         self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
         self.build()
 
     def build(self) -> None:
         final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
             self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
         )
         for character in self._terminal.get_characters():
             self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
         for row_index, characters in enumerate(
             self._terminal.get_characters_grouped(grouping=self._terminal.CharacterGroup.ROW_BOTTOM_TO_TOP)
         ):
-            self._lines[row_index] = _Line(characters, self._config, self._character_final_color_map)
+            self._lines[row_index] = VHSTapeIterator._Line(characters, self._config, self._character_final_color_map)
         for character in self._terminal.get_characters():
             self._terminal.set_character_visibility(character, True)
             character.animation.activate_scene(character.animation.query_scene("base"))
         self._glitching_steps_elapsed = 0
         self._phase = "glitching"
         self._to_redraw = list(self._lines.values())
         self._redrawing = False
@@ -352,15 +313,15 @@
                         wave_top_delta = -1
                 else:
                     wave_top_delta = 0
                 self._active_glitch_wave_top += wave_top_delta
                 # clamp wave top to output area
                 self._active_glitch_wave_top = max(2, min(self._active_glitch_wave_top, self._terminal.output_area.top))
             # get the lines for the wave
-            new_wave_lines: list[_Line] = []
+            new_wave_lines: list[VHSTapeIterator._Line] = []
             for line_index in range(self._active_glitch_wave_top - 2, self._active_glitch_wave_top + 1):
                 if line_index in self._lines:
                     new_wave_lines.append(self._lines[line_index])
 
             # restore any lines that are no longer part of the wave
             for line in self._active_glitch_wave_lines:
                 if line not in new_wave_lines:
@@ -393,15 +354,15 @@
                     self._glitch_wave()
                 # Remove completed glitch lines from active glitch lines
                 self._active_glitch_lines = [
                     line for line in self._active_glitch_lines if not line.line_movement_complete()
                 ]
                 # Randomly add new glitch lines
                 if random.random() < self._config.glitch_line_chance and len(self._active_glitch_lines) < 3:
-                    glitch_line: _Line = random.choice(list(self._lines.values()))
+                    glitch_line: VHSTapeIterator._Line = random.choice(list(self._lines.values()))
                     if (
                         glitch_line not in self._active_glitch_wave_lines
                         and glitch_line not in self._active_glitch_lines
                     ):
                         glitch_line.set_hold_time(random.randint(30, 120))
                         self._active_glitch_lines.append(glitch_line)
                         glitch_line.glitch()
@@ -448,14 +409,23 @@
             self._active_chars = [character for character in self._active_chars if character.is_active]
             return self._terminal.get_formatted_output_string()
         else:
             raise StopIteration
 
 
 class VHSTape(BaseEffect[VHSTapeConfig]):
-    """Lines of characters glitch left and right and lose detail like an old VHS tape."""
+    """Lines of characters glitch left and right and lose detail like an old VHS tape.
+
+    Attributes:
+        effect_config (VHSTapeConfig): Configuration for the effect.
+        terminal_config (TerminalConfig): Configuration for the terminal.
+    """
 
     _config_cls = VHSTapeConfig
     _iterator_cls = VHSTapeIterator
 
     def __init__(self, input_data: str) -> None:
+        """Initialize the effect with the provided input data.
+
+        Args:
+            input_data (str): The input data to use for the effect."""
         super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_waves.py` & `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_waves.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,133 +1,139 @@
+"""Waves travel across the terminal leaving behind the characters.
+
+Classes:
+    Waves: Creates waves that travel across the terminal, leaving behind the characters.
+    WavesConfig: Configuration for the Waves effect.
+    WavesIterator: Iterates over the effect. Does not normally need to be called directly.
+"""
+
 import typing
 from dataclasses import dataclass
 
-import terminaltexteffects.utils.arg_validators as arg_validators
-from terminaltexteffects.base_character import EffectCharacter, EventHandler
-from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
+import terminaltexteffects.utils.argvalidators as argvalidators
+from terminaltexteffects.engine.base_character import EffectCharacter, EventHandler
+from terminaltexteffects.engine.base_effect import BaseEffect, BaseEffectIterator
 from terminaltexteffects.utils import easing, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
     return Waves, WavesConfig
 
 
 @argclass(
     name="waves",
     help="Waves travel across the terminal leaving behind the characters.",
     description="waves | Waves travel across the terminal leaving behind the characters.",
-    epilog=f"""{arg_validators.EASING_EPILOG}
+    epilog=f"""{argvalidators.EASING_EPILOG}
 Example: terminaltexteffects waves --wave-symbols ▁ ▂ ▃ ▄ ▅ ▆ ▇ █ ▇ ▆ ▅ ▄ ▃ ▂ ▁ --wave-gradient-stops f0ff65 ffb102 31a0d4 ffb102 f0ff65 --wave-gradient-steps 6 --final-gradient-stops ffb102 31a0d4 f0ff65 --final-gradient-steps 12 --wave-count 7 --wave-length 2 --wave-easing IN_OUT_SINE""",
 )
 @dataclass
 class WavesConfig(ArgsDataClass):
     """Configuration for the Waves effect.
 
     Attributes:
         wave_symbols (tuple[str, ...]): Symbols to use for the wave animation. Multi-character strings will be used in sequence to create an animation.
-        wave_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
-        wave_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
-        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
-        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
-        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
-        wave_count (int): Number of waves to generate. n > 0."""
+        wave_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color.
+        wave_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation. Valid values are n > 0.
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation. Valid values are n > 0.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the final gradient.
+        wave_count (int): Number of waves to generate. Valid values are n > 0."""
 
     wave_symbols: tuple[str, ...] = ArgField(
         cmd_name="--wave-symbols",
-        type_parser=arg_validators.Symbol.type_parser,
+        type_parser=argvalidators.Symbol.type_parser,
         default=("▁", "▂", "▃", "▄", "▅", "▆", "▇", "█", "▇", "▆", "▅", "▄", "▃", "▂", "▁"),
         nargs="+",
-        metavar=arg_validators.Symbol.METAVAR,
+        metavar=argvalidators.Symbol.METAVAR,
         help="Symbols to use for the wave animation. Multi-character strings will be used in sequence to create an animation.",
     )  # type: ignore[assignment]
     "tuple[str, ...] : Symbols to use for the wave animation. Multi-character strings will be used in sequence to create an animation."
 
     wave_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name="--wave-gradient-stops",
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("f0ff65", "ffb102", "31a0d4", "ffb102", "f0ff65"),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
-    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+    "tuple[graphics.Color, ...] : Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color."
 
     wave_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name="--wave-gradient-steps",
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         nargs="+",
         default=(6,),
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
     "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
 
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name="--final-gradient-stops",
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("ffb102", "31a0d4", "f0ff65"),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
-    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+    "tuple[graphics.Color, ...] : Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color."
 
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name="--final-gradient-steps",
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
     "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
 
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
-        type_parser=arg_validators.GradientDirection.type_parser,
+        type_parser=argvalidators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.DIAGONAL,
-        metavar=arg_validators.GradientDirection.METAVAR,
-        help="Direction of the gradient for the final color.",
+        metavar=argvalidators.GradientDirection.METAVAR,
+        help="Direction of the final gradient.",
     )  # type: ignore[assignment]
-    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+    "graphics.Gradient.Direction : Direction of the final gradient."
 
     wave_count: int = ArgField(
         cmd_name="--wave-count",
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         default=7,
         help="Number of waves to generate. n > 0.",
     )  # type: ignore[assignment]
     "int : Number of waves to generate. n > 0."
 
     wave_length: int = ArgField(
         cmd_name="--wave-length",
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         default=2,
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="The number of frames for each step of the wave. Higher wave-lengths will create a slower wave.",
     )  # type: ignore[assignment]
     "int : The number of frames for each step of the wave. Higher wave-lengths will create a slower wave."
 
     wave_easing: easing.EasingFunction = ArgField(
         cmd_name="--wave-easing",
-        type_parser=arg_validators.Ease.type_parser,
+        type_parser=argvalidators.Ease.type_parser,
         default=easing.in_out_sine,
         help="Easing function to use for wave travel.",
     )  # type: ignore[assignment]
     "easing.EasingFunction : Easing function to use for wave travel."
 
     @classmethod
     def get_effect_class(cls):
         return Waves
 
 
 class WavesIterator(BaseEffectIterator[WavesConfig]):
-    """Effect that creates waves that travel across the terminal, leaving behind the characters."""
-
     def __init__(self, effect: "Waves") -> None:
         super().__init__(effect)
         self._pending_columns: list[list[EffectCharacter]] = []
         self._active_chars: list[EffectCharacter] = []
         self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
         self._build()
 
@@ -173,14 +179,23 @@
             self._active_chars = [character for character in self._active_chars if character.is_active]
             return self._terminal.get_formatted_output_string()
         else:
             raise StopIteration
 
 
 class Waves(BaseEffect[WavesConfig]):
-    """Effect that creates waves that travel across the terminal, leaving behind the characters."""
+    """Creates waves that travel across the terminal, leaving behind the characters.
+
+    Attributes:
+        effect_config (ExpandConfig): Configuration for the effect.
+        terminal_config (TerminalConfig): Configuration for the terminal.
+    """
 
     _config_cls = WavesConfig
     _iterator_cls = WavesIterator
 
     def __init__(self, input_data: str) -> None:
+        """Initialize the effect with the provided input data.
+
+        Args:
+            input_data (str): The input data to use for the effect."""
         super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_wipe.py` & `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_random_sequence.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,171 +1,163 @@
+"""Prints the input data in a random sequence, one character at a time.
+
+Classes:
+    RandomSequence: Prints the input data in a random sequence.
+    RandomSequenceConfig: Configuration for the RandomSequence effect.
+    RandomSequenceIterator: Iterator for the RandomSequence effect. Does not normally need to be called directly.
+"""
+
+import random
 import typing
 from dataclasses import dataclass
 
-import terminaltexteffects.utils.arg_validators as arg_validators
-from terminaltexteffects.base_character import EffectCharacter
-from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
+import terminaltexteffects.utils.argvalidators as argvalidators
+from terminaltexteffects.engine.base_character import EffectCharacter
+from terminaltexteffects.engine.base_effect import BaseEffect, BaseEffectIterator
 from terminaltexteffects.utils import graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
-    return Wipe, WipeConfig
+    return RandomSequence, RandomSequenceConfig
 
 
 @argclass(
-    name="wipe",
-    help="Wipes the text across the terminal to reveal characters.",
-    description="wipe | Wipes the text across the terminal to reveal characters.",
-    epilog="""Example: terminaltexteffects wipe --wipe-direction diagonal_bottom_left_to_top_right --final-gradient-stops 833ab4 fd1d1d fcb045 --final-gradient-steps 12 --final-gradient-frames 5 --wipe-delay 0""",
+    name="randomsequence",
+    help="Prints the input data in a random sequence.",
+    description="randomsequence | Prints the input data in a random sequence.",
+    epilog="Example: terminaltexteffects randomsequence --starting-color 000000 --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --final-gradient-frames 12 --speed 0.004",
 )
 @dataclass
-class WipeConfig(ArgsDataClass):
-    """Configuration for the Wipe effect.
+class RandomSequenceConfig(ArgsDataClass):
+    """Configuration for the RandomSequence effect.
 
     Attributes:
-        wipe_direction (str): Direction the text will wipe.
-        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the wipe gradient.
-        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
+        starting_color (graphics.Color): Color of the characters at spawn.
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation. Valid values are n > 0.
         final_gradient_frames (int): Number of frames to display each gradient step.
-        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
-        wipe_delay (int): Number of animation cycles to wait before adding the next character group. Increase, to slow down the effect."""
-
-    wipe_direction: str = ArgField(
-        cmd_name="--wipe-direction",
-        default="diagonal_bottom_left_to_top_right",
-        choices=[
-            "column_left_to_right",
-            "column_right_to_left",
-            "row_top_to_bottom",
-            "row_bottom_to_top",
-            "diagonal_top_left_to_bottom_right",
-            "diagonal_bottom_left_to_top_right",
-            "diagonal_top_right_to_bottom_left",
-            "diagonal_bottom_right_to_top_left",
-        ],
-        help="Direction the text will wipe.",
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the final gradient.
+        speed (float): Speed of the animation as a percentage of the total number of characters to reveal in each tick. Valid values are 0 < n <= 1.
+    """
+
+    starting_color: graphics.Color = ArgField(
+        cmd_name=["--starting-color"],
+        type_parser=argvalidators.ColorArg.type_parser,
+        default="000000",
+        metavar=argvalidators.ColorArg.METAVAR,
+        help="Color of the characters at spawn.",
     )  # type: ignore[assignment]
-    "str : Direction the text will wipe. Options: column_left_to_right, column_right_to_left, row_top_to_bottom, row_bottom_to_top, diagonal_top_left_to_bottom_right, diagonal_bottom_left_to_top_right, diagonal_top_right_to_bottom_left, diagonal_bottom_right_to_top_left."
 
+    "graphics.Color : Color of the characters at spawn."
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
-        cmd_name="--final-gradient-stops",
-        type_parser=arg_validators.Color.type_parser,
+        cmd_name=["--final-gradient-stops"],
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
-        default=("833ab4", "fd1d1d", "fcb045"),
-        metavar=arg_validators.Color.METAVAR,
-        help="Space separated, unquoted, list of colors for the wipe gradient.",
+        default=("8A008A", "00D1FF", "FFFFFF"),
+        metavar=argvalidators.ColorArg.METAVAR,
+        help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
-    "tuple[graphics.Color, ...] : Tuple of colors for the wipe gradient."
 
+    "tuple[graphics.Color, ...] : Tuple of colors for the final color gradient. If only one color is provided, the characters will be displayed in that color."
     final_gradient_steps: tuple[int, ...] = ArgField(
-        cmd_name="--final-gradient-steps",
-        type_parser=arg_validators.PositiveInt.type_parser,
+        cmd_name=["--final-gradient-steps"],
+        type_parser=argvalidators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
-        metavar=arg_validators.PositiveInt.METAVAR,
-        help="Number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
+        metavar=argvalidators.PositiveInt.METAVAR,
+        help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
-    "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
 
+    "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
     final_gradient_frames: int = ArgField(
-        cmd_name="--final-gradient-frames",
-        type_parser=arg_validators.PositiveInt.type_parser,
-        default=5,
-        metavar=arg_validators.PositiveInt.METAVAR,
+        cmd_name=["--final-gradient-frames"],
+        type_parser=argvalidators.PositiveInt.type_parser,
+        default=12,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Number of frames to display each gradient step.",
     )  # type: ignore[assignment]
-    "int : Number of frames to display each gradient step."
 
+    "int : Number of frames to display each gradient step."
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
-        type_parser=arg_validators.GradientDirection.type_parser,
+        type_parser=argvalidators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.VERTICAL,
-        metavar=arg_validators.GradientDirection.METAVAR,
-        help="Direction of the gradient for the final color.",
+        metavar=argvalidators.GradientDirection.METAVAR,
+        help="Direction of the final gradient.",
     )  # type: ignore[assignment]
-    "graphics.Gradient.Direction : Direction of the gradient for the final color."
 
-    wipe_delay: int = ArgField(
-        cmd_name="--wipe-delay",
-        type_parser=arg_validators.NonNegativeInt.type_parser,
-        default=0,
-        metavar=arg_validators.NonNegativeInt.METAVAR,
-        help="Number of animation cycles to wait before adding the next character group. Increase, to slow down the effect.",
+    "graphics.Gradient.Direction : Direction of the final gradient."
+    speed: float = ArgField(
+        cmd_name=["--speed"],
+        type_parser=argvalidators.PositiveFloat.type_parser,
+        default=0.004,
+        metavar=argvalidators.PositiveFloat.METAVAR,
+        help="Speed of the animation as a percentage of the total number of characters to reveal in each tick.",
     )  # type: ignore[assignment]
-    "int : Number of animation cycles to wait before adding the next character group. Increase, to slow down the effect."
+
+    "float : Speed of the animation as a percentage of the total number of characters to reveal in each tick."
 
     @classmethod
     def get_effect_class(cls):
-        return Wipe
-
+        return RandomSequence
 
-class WipeIterator(BaseEffectIterator[WipeConfig]):
-    """Effect that performs a wipe across the terminal to reveal characters."""
 
-    def __init__(self, effect: "Wipe") -> None:
+class RandomSequenceIterator(BaseEffectIterator[RandomSequenceConfig]):
+    def __init__(self, effect: "RandomSequence") -> None:
         super().__init__(effect)
-        self._pending_groups: list[list[EffectCharacter]] = []
+        self._pending_chars: list[EffectCharacter] = []
         self._active_chars: list[EffectCharacter] = []
         self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self._characters_per_tick = max(int(self._config.speed * len(self._terminal._input_characters)), 1)
         self._build()
 
     def _build(self) -> None:
-        direction = self._config.wipe_direction
         final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
             self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
         )
         for character in self._terminal.get_characters():
             self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
-        sort_map = {
-            "column_left_to_right": self._terminal.CharacterGroup.COLUMN_LEFT_TO_RIGHT,
-            "column_right_to_left": self._terminal.CharacterGroup.COLUMN_RIGHT_TO_LEFT,
-            "row_top_to_bottom": self._terminal.CharacterGroup.ROW_TOP_TO_BOTTOM,
-            "row_bottom_to_top": self._terminal.CharacterGroup.ROW_BOTTOM_TO_TOP,
-            "diagonal_top_left_to_bottom_right": self._terminal.CharacterGroup.DIAGONAL_TOP_LEFT_TO_BOTTOM_RIGHT,
-            "diagonal_bottom_left_to_top_right": self._terminal.CharacterGroup.DIAGONAL_BOTTOM_LEFT_TO_TOP_RIGHT,
-            "diagonal_top_right_to_bottom_left": self._terminal.CharacterGroup.DIAGONAL_TOP_RIGHT_TO_BOTTOM_LEFT,
-            "diagonal_bottom_right_to_top_left": self._terminal.CharacterGroup.DIAGONAL_BOTTOM_RIGHT_TO_TOP_LEFT,
-        }
-        for group in self._terminal.get_characters_grouped(sort_map[direction]):
-            for character in group:
-                wipe_scn = character.animation.new_scene()
-                wipe_gradient = graphics.Gradient(
-                    final_gradient.spectrum[0],
-                    self._character_final_color_map[character],
-                    steps=self._config.final_gradient_steps,
-                )
-                wipe_scn.apply_gradient_to_symbols(
-                    wipe_gradient, character.input_symbol, self._config.final_gradient_frames
-                )
-                character.animation.activate_scene(wipe_scn)
-            self._pending_groups.append(group)
-        self._wipe_delay = self._config.wipe_delay
+            self._terminal.set_character_visibility(character, False)
+            gradient_scn = character.animation.new_scene()
+            gradient = graphics.Gradient(
+                self._config.starting_color, self._character_final_color_map[character], steps=7
+            )
+            gradient_scn.apply_gradient_to_symbols(gradient, character.input_symbol, self._config.final_gradient_frames)
+            character.animation.activate_scene(gradient_scn)
+            self._pending_chars.append(character)
+        random.shuffle(self._pending_chars)
 
     def __next__(self) -> str:
-        if self._pending_groups or self._active_chars:
-            if not self._wipe_delay:
-                if self._pending_groups:
-                    next_group = self._pending_groups.pop(0)
-                    for character in next_group:
-                        self._terminal.set_character_visibility(character, True)
-                        self._active_chars.append(character)
-                self._wipe_delay = self._config.wipe_delay
-            else:
-                self._wipe_delay -= 1
+        if self._pending_chars or self._active_chars:
+            for _ in range(self._characters_per_tick):
+                if self._pending_chars:
+                    next_char = self._pending_chars.pop()
+                    self._terminal.set_character_visibility(next_char, True)
+                    self._active_chars.append(next_char)
             for character in self._active_chars:
                 character.tick()
+            next_frame = self._terminal.get_formatted_output_string()
+
             self._active_chars = [character for character in self._active_chars if character.is_active]
-            return self._terminal.get_formatted_output_string()
-        else:
-            raise StopIteration
+            return next_frame
+        raise StopIteration
 
 
-class Wipe(BaseEffect[WipeConfig]):
-    """Effect that performs a wipe across the terminal to reveal characters."""
+class RandomSequence(BaseEffect[RandomSequenceConfig]):
+    """Prints the input data in a random sequence, one character at a time.
 
-    _config_cls = WipeConfig
-    _iterator_cls = WipeIterator
+    Attributes:
+        effect_config (PourConfig): Configuration for the effect.
+        terminal_config (TerminalConfig): Configuration for the terminal.
+    """
+
+    _config_cls = RandomSequenceConfig
+    _iterator_cls = RandomSequenceIterator
 
     def __init__(self, input_data: str) -> None:
+        """Initialize the effect with the provided input data.
+
+        Args:
+            input_data (str): The input data to use for the effect."""
         super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/template/effect_template.py` & `terminaltexteffects-0.9.0/terminaltexteffects/template/effect_template.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,89 +1,89 @@
 import typing
 from dataclasses import dataclass
 
-import terminaltexteffects.utils.arg_validators as arg_validators
-from terminaltexteffects.base_character import EffectCharacter
-from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
+import terminaltexteffects.utils.argvalidators as argvalidators
+from terminaltexteffects.engine.base_character import EffectCharacter
+from terminaltexteffects.engine.base_effect import BaseEffect, BaseEffectIterator
 from terminaltexteffects.utils import easing, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 
 
 @argclass(
     name="namedeffect",
     help="effect_description",
     description="effect_description",
-    epilog=f"""{arg_validators.EASING_EPILOG}
+    epilog=f"""{argvalidators.EASING_EPILOG}
     """,
 )
 @dataclass
 class EffectConfig(ArgsDataClass):
     color_single: graphics.Color = ArgField(
         cmd_name=["--color-single"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         default=0,
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Color for the ___.",
     )  # type: ignore[assignment]
 
     color_list: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--color-list"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=0,
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the ___.",
     )  # type: ignore[assignment]
 
     final_color: graphics.Color = ArgField(
         cmd_name=["--final-color"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         default="ffffff",
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Color for the final character.",
     )  # type: ignore[assignment]
 
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
-        type_parser=arg_validators.Color.type_parser,
+        type_parser=argvalidators.ColorArg.type_parser,
         nargs="+",
         default=("8A008A", "00D1FF", "FFFFFF"),
-        metavar=arg_validators.Color.METAVAR,
+        metavar=argvalidators.ColorArg.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
 
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name="--final-gradient-steps",
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
 
     final_gradient_frames: int = ArgField(
         cmd_name="--final-gradient-frames",
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         default=5,
-        metavar=arg_validators.PositiveInt.METAVAR,
+        metavar=argvalidators.PositiveInt.METAVAR,
         help="Number of frames to display each gradient step.",
     )  # type: ignore[assignment]
 
     movement_speed: float = ArgField(
         cmd_name="--movement-speed",
-        type_parser=arg_validators.PositiveFloat.type_parser,
+        type_parser=argvalidators.PositiveFloat.type_parser,
         default=1,
-        metavar=arg_validators.PositiveFloat.METAVAR,
+        metavar=argvalidators.PositiveFloat.METAVAR,
         help="Speed of the ___.",
     )  # type: ignore[assignment]
 
     easing: typing.Callable = ArgField(
         cmd_name=["--easing"],
         default=easing.in_out_sine,
-        type_parser=arg_validators.Ease.type_parser,
+        type_parser=argvalidators.Ease.type_parser,
         help="Easing function to use for character movement.",
     )  # type: ignore[assignment]
 
     @classmethod
     def get_effect_class(cls):
         return NamedEffect
 
@@ -118,8 +118,12 @@
 class NamedEffect(BaseEffect[EffectConfig]):
     """Effect description."""
 
     _config_cls = EffectConfig
     _iterator_cls = NamedEffectIterator
 
     def __init__(self, input_data: str) -> None:
+        """Initialize the effect with the provided input data.
+
+        Args:
+            input_data (str): The input data to use for the effect."""
         super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/utils/animation.py` & `terminaltexteffects-0.9.0/terminaltexteffects/engine/animation.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import typing
 from dataclasses import dataclass
 from enum import Enum, auto
 
 from terminaltexteffects.utils import ansitools, colorterm, easing, graphics, hexterm
 
 if typing.TYPE_CHECKING:
-    from terminaltexteffects import base_character
+    from terminaltexteffects.engine import base_character
 
 
 class SyncMetric(Enum):
     """Enum for specifying the type of sync to use for a Scene.
 
     Attributes:
         DISTANCE (int): Sync to a Waypoint based on distance from the Waypoint
@@ -21,17 +21,14 @@
     STEP = auto()
 
 
 @dataclass
 class CharacterVisual:
     """A class for storing symbol, color, and terminal graphical modes for the character.
 
-    Supported graphical modes:
-    bold, dim, italic, underline, blink, inverse, hidden, strike
-
     Args:
         symbol (str): the symbol to show
         bold (bool): bold mode
         dim (bool): dim mode
         italic (bool): italic mode
         underline (bool): underline mode
         blink (bool): blink mode
@@ -63,15 +60,15 @@
         self.underline = False
         self.blink = False
         self.reverse = False
         self.hidden = False
         self.strike = False
 
     def format_symbol(self) -> None:
-        """Formats the symbol for printing."""
+        """Formats the symbol for printing by applying ANSI sequences for any active modes and color."""
         formatting_string = ""
         if self.bold:
             formatting_string += ansitools.APPLY_BOLD()
         if self.italic:
             formatting_string += ansitools.APPLY_ITALIC()
         if self.underline:
             formatting_string += ansitools.APPLY_UNDERLINE()
@@ -88,49 +85,60 @@
 
         self.symbol = f"{formatting_string}{self.symbol}{ansitools.RESET_ALL() if formatting_string else ''}"
 
 
 @dataclass
 class Frame:
     """A Frame is a CharacterVisual with a duration.
+
     Args:
         character_visual (CharacterVisual): a CharacterVisual object
-        duration (int): the number of animation steps to use the Frame
+        duration (int): the number of frames to use the Frame
     """
 
     character_visual: CharacterVisual
     duration: int
 
     def __post_init__(self):
         self.frames_played = 0
         self.symbol = self.character_visual.symbol
 
 
 class Scene:
-    """A Scene is a list of Frames.
+    """A Scene is a collection of Frames that can be played in sequence. Scenes can be looped and synced to movement.
 
-    Args:
-        scene_id (str): unique ID for the Scene
-        is_looping (bool): whether the Scene should loop
-        sync (SyncMetric): the sync metric to use
-        no_color (bool): whether to disable color
-        use_xterm_colors (bool): whether to use XTerm-256 colors
+    Methods:
+        add_frame: Adds a Frame to the Scene.
+        activate: Activates the Scene.
+        get_next_symbol: Returns the next symbol in the Scene.
+        apply_gradient_to_symbols: Applies a gradient effect to a sequence of symbols.
+        reset_scene: Resets the Scene.
     """
 
     xterm_color_map: dict[str, int] = {}
 
     def __init__(
         self,
         scene_id: str,
         is_looping: bool = False,
         sync: SyncMetric | None = None,
         ease: easing.EasingFunction | None = None,
         no_color: bool = False,
         use_xterm_colors: bool = False,
     ):
+        """Initializes a Scene.
+
+        Args:
+            scene_id (str): the ID of the Scene
+            is_looping (bool, optional): Whether the Scene should loop. Defaults to False.
+            sync (SyncMetric | None, optional): The type of sync to use for the Scene. Defaults to None.
+            ease (easing.EasingFunction | None, optional): The easing function to use for the Scene. Defaults to None.
+            no_color (bool, optional): Whether to colors should be ignored. Defaults to False.
+            use_xterm_colors (bool, optional): Whether to convert all colors to XTerm-256 colors. Defaults to False.
+        """
         self.scene_id = scene_id
         self.is_looping = is_looping
         self.sync: SyncMetric | None = sync
         self.ease: easing.EasingFunction | None = ease
         self.no_color = no_color
         self.use_xterm_colors = use_xterm_colors
         self.frames: list[Frame] = []
@@ -150,28 +158,29 @@
         italic=False,
         underline=False,
         blink=False,
         reverse=False,
         hidden=False,
         strike=False,
     ) -> None:
-        """Adds a Frame to the Scene.
+        """Adds a Frame to the Scene with the given symbol, duration, color, and graphical modes.
 
         Args:
             symbol (str): the symbol to show
             color (str | int): color code
-            duration (int): the number of animation steps to use the Frame
-            BOLD (bool): bold mode
-            DIM (bool): dim mode
-            ITALIC (bool): italic mode
-            UNDERLINE (bool): underline mode
-            BLINK (bool): blink mode
-            REVERSE (bool): reverse mode
-            HIDDEN (bool): hidden mode
-            STRIKE (bool): strike mode
+            duration (int): the number of frames to use the Frame
+            color (str | int | None, optional): the color to show. Defaults to None.
+            bold (bool, optional): bold mode. Defaults to False.
+            dim (bool, optional): dim mode. Defaults to False.
+            italic (bool, optional): italic mode. Defaults to False.
+            underline (bool, optional): underline mode. Defaults to False.
+            blink (bool, optional): blink mode. Defaults to False.
+            reverse (bool, optional): reverse mode. Defaults to False.
+            hidden (bool, optional): hidden mode. Defaults to False.
+            strike (bool, optional): strike mode. Defaults to False.
         """
         if not self.no_color and color is not None:
             if self.use_xterm_colors and isinstance(color, str):
                 if color in self.xterm_color_map:
                     color = self.xterm_color_map[color]
                 else:
                     xterm_color = hexterm.hex_to_xterm(color)
@@ -196,29 +205,37 @@
         frame = Frame(char_vis, duration)
         self.frames.append(frame)
         for _ in range(frame.duration):
             self.frame_index_map[self.easing_total_steps] = frame
             self.easing_total_steps += 1
 
     def activate(self) -> str:
-        """Activates the Scene.
+        """Activates the Scene by returning the first frame symbol. Called by the Animation object when the Scene is activated.
+
+        Raises:
+            ValueError: if the Scene has no sequences
 
         Returns:
             str: the next symbol in the Scene
         """
         if self.frames:
             return self.frames[0].symbol
         else:
             raise ValueError("Scene has no sequences.")
 
     def get_next_symbol(self) -> str:
-        """Returns the next symbol in the Scene.
+        """
+        This method is used to get the next symbol in the Scene. It first retrieves the current sequence from the frames list.
+        It then increments the 'frames_played' attribute of the current sequence. If the 'frames_played' equals the 'duration'
+        of the current sequence, it resets 'frames_played' to 0 and moves the current sequence from the frames list to the
+        'played_frames' list. If the Scene is set to loop and all frames have been played, it refills the frames list with the
+        sequences from 'played_frames' and clears 'played_frames'. Finally, it returns the symbol of the current sequence.
 
         Returns:
-            str: the next symbol in the Scene
+            str: The symbol of the current sequence in the Scene.
         """
 
         current_sequence = self.frames[0]
         next_symbol = current_sequence.symbol
         current_sequence.frames_played += 1
         if current_sequence.frames_played == current_sequence.duration:
             current_sequence.frames_played = 0
@@ -536,28 +553,28 @@
                 self.character.symbol = self.active_scene.get_next_symbol()
             if self.active_scene_is_complete():
                 completed_scene = self.active_scene
                 if not self.active_scene.is_looping:
                     self.active_scene.reset_scene()
                     self.active_scene = None
 
-                self.character.event_handler.handle_event(
+                self.character.event_handler._handle_event(
                     self.character.event_handler.Event.SCENE_COMPLETE, completed_scene
                 )
 
     def activate_scene(self, scene: Scene) -> None:
         """Sets the active scene.
 
         Args:
             scene (Scene): the Scene to set as active
         """
         self.active_scene = scene
         self.active_scene_current_step = 0
         self.character.symbol = self.active_scene.activate()
-        self.character.event_handler.handle_event(self.character.event_handler.Event.SCENE_ACTIVATED, scene)
+        self.character.event_handler._handle_event(self.character.event_handler.Event.SCENE_ACTIVATED, scene)
 
     def deactivate_scene(self, scene: Scene) -> None:
         """Deactivates a scene.
 
         Args:
             scene (Scene): the Scene to deactivate
         """
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/utils/ansitools.py` & `terminaltexteffects-0.9.0/terminaltexteffects/utils/ansitools.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-"""This file contains ANSI escape codes for terminal formatting."""
+"""This module provides a collection of functions that generate ANSI escape codes for various terminal formatting effects.
+These escape codes can be used to modify the appearance of text in a terminal.
+"""
 
 
 def DEC_SAVE_CURSOR_POSITION() -> str:
     """Saves the cursor position using DEC sequence.
 
     Returns:
         str: ANSI escape code
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/utils/arg_validators.py` & `terminaltexteffects-0.9.0/terminaltexteffects/utils/argvalidators.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,56 @@
+"""
+This module provides command line argument validators and METAVARs for consistent type parsing and help output.
+
+It includes a custom formatter for argparse, which combines the features of
+`argparse.ArgumentDefaultsHelpFormatter` and `argparse.RawDescriptionHelpFormatter`.
+
+Classes:
+    CustomFormatter: A custom formatter for argparse that combines the features of
+        `argparse.ArgumentDefaultsHelpFormatter` and `argparse.RawDescriptionHelpFormatter`.
+    GradientDirection: Argument type for gradient directions.
+    Color: Argument type for color values.
+    PositiveFloatRange: Argument type for float ranges.
+    IntRange: Argument type for integer ranges.
+    Symbol: Argument type for single ASCII/UTF-8 characters.
+    TerminalDimensions: Argument type for terminal dimensions.
+    PositiveInt: Argument type for positive integers.
+    Ease: Argument type for easing functions.
+    Ratio: Argument type for float values between zero and one.
+    PositiveFloat: Argument type for positive floats.
+    NonNegativeInt: Argument type for nonnegative integers.
+    NonNegativeFloat: Argument type for nonnegative floats.
+
+Functions:
+    is_ascii_or_utf8: Tests if the given string is either ASCII or UTF-8.
+
+Constants:
+    EASING_EPILOG (str): A detailed description of the easing functions supported.
+"""
+
 import argparse
 import typing
 
 from terminaltexteffects.utils import easing
 from terminaltexteffects.utils.graphics import Color as ColorType
 from terminaltexteffects.utils.graphics import Gradient
 
 EASING_EPILOG = """\
     Easing
     ------
-    Note: A prefix must be added to the function name.
+    Note: A prefix must be added to the function name (except LINEAR).
     
     All easing functions support the following prefixes:
         IN_  - Ease in
         OUT_ - Ease out
         IN_OUT_ - Ease in and out
         
     Easing Functions
     ----------------
+    LINEAR - Linear easing
     SINE   - Sine easing
     QUAD   - Quadratic easing
     CUBIC  - Cubic easing
     QUART  - Quartic easing
     QUINT  - Quintic easing
     EXPO   - Exponential easing
     CIRC   - Circular easing
@@ -28,92 +58,161 @@
     ELASTIC - Elastic easing
     BOUNCE - Bounce easing
     
     Visit: https://easings.net/ for visualizations of the easing functions.
 """
 
 
-class CustomFormatter(argparse.ArgumentDefaultsHelpFormatter, argparse.RawDescriptionHelpFormatter):
-    """Custom formatter for argparse that combines ArgumentDefaultsHelpFormatter and RawDescriptionHelpFormatter."""
+class PositiveInt:
+    """Argument type for positive integers.
 
-    pass
+    int(n) > 0
 
+    Raises:
+        argparse.ArgumentTypeError: Value is not a positive integer.
+    """
 
-class GradientDirection:
-    """Argument type for gradient directions.
+    METAVAR = "(int > 0)"
+
+    @staticmethod
+    def type_parser(arg: str) -> int:
+        """Validates that the given argument is a positive integer. n > 0.
+
+        Args:
+            arg (str): argument to validate
+
+        Returns:
+            int: validated positive integer
+        """
+        if int(arg) > 0:
+            return int(arg)
+        else:
+            raise argparse.ArgumentTypeError(f"invalid value: '{arg}' is not > 0.")
+
+
+class NonNegativeInt:
+    """Validates that the given argument is a nonnegative integer. n >= 0.
 
     Raises:
-        argparse.ArgumentTypeError: Argument value is not a valid gradient direction.
+        argparse.ArgumentTypeError: Value is not in range.
     """
 
-    METAVAR = "(diagonal, horizontal, vertical, center)"
+    METAVAR = "(int >= 0)"
 
     @staticmethod
-    def type_parser(arg: str) -> Gradient.Direction:
-        """Validates that the given argument is a valid gradient direction.
+    def type_parser(arg: str) -> int:
+        """Validates that the given argument is a nonnegative integer. n >= 0.
 
         Args:
             arg (str): argument to validate
 
+        Raises:
+            argparse.ArgumentTypeError: Value is not in range.
+
         Returns:
-            Gradient.Direction: validated gradient direction
+            int: validated gap value
+        """
+        if int(arg) < 0:
+            raise argparse.ArgumentTypeError(f"invalid value: '{arg}' Argument must be int >= 0.")
+        return int(arg)
+
+
+class IntRange:
+    """Argument type for integer ranges.
+
+    Integer ranges are a pair of integers separated by a hyphen. Ex: 1-10
+
+    Raises:
+        argparse.ArgumentTypeError: Value is not a valid range of integers.
+    """
+
+    METAVAR = "(hyphen separated int range e.g. '1-10')"
+
+    @staticmethod
+    def type_parser(arg: str) -> tuple[int, int]:
+        """Validates that the given argument is a valid range of integers n > 0.
+
+        Args:
+            arg (str): argument to validate
+
+        Returns:
+            tuple[int,int]: validated range
+        """
+        try:
+            start, end = map(int, arg.split("-"))
+            if start <= 0:
+                raise argparse.ArgumentTypeError(
+                    f"invalid range: '{arg}' is not a valid range of ints. Must be start > 0. Ex: 1-10"
+                )
+            if start > end:
+                raise argparse.ArgumentTypeError(
+                    f"invalid range: '{arg}' is not a valid range of ints. Must be start <= end. Ex: 1-10"
+                )
+            return start, end
+        except ValueError:
+            raise argparse.ArgumentTypeError(
+                f"invalid range: '{arg}' is not a valid range. Must be start-end. Ex: 1-10"
+            )
+
+
+class PositiveFloat:
+    """Validates that the given argument is a positive float. n > 0.
+
+    Raises:
+        argparse.ArgumentTypeError: Value is not in range.
+    """
+
+    METAVAR = "(float > 0)"
+
+    @staticmethod
+    def type_parser(arg: str) -> float:
+        """Validates that the given argument is a positive float. n > 0.
+
+        Args:
+            arg (str): argument to validate
 
         Raises:
-            argparse.ArgumentTypeError: Argument value is not a valid gradient direction.
+            argparse.ArgumentTypeError: value is not in range.
+
+        Returns:
+            float: validated positive float
         """
-        direction_map = {
-            "horizontal": Gradient.Direction.HORIZONTAL,
-            "vertical": Gradient.Direction.VERTICAL,
-            "diagonal": Gradient.Direction.DIAGONAL,
-            "center": Gradient.Direction.CENTER,
-        }
-        if arg.lower() in direction_map:
-            return direction_map[arg.lower()]
+        if float(arg) > 0:
+            return float(arg)
         else:
             raise argparse.ArgumentTypeError(
-                f"invalid gradient direction: '{arg}' is not a valid gradient direction. Choices are diagonal, horizontal, vertical, or center."
+                f"invalid value: '{arg}' is not a valid value. Argument must be a float > 0."
             )
 
 
-class Color:
-    """Argument type for color values.
-
-    Color values can be either an XTerm color value (0-255) or an RGB hex value (000000-ffffff).
+class NonNegativeFloat:
+    """Validates that the given argument is a valid animationrate value. n >= 0.
 
     Raises:
-        argparse.ArgumentTypeError: Value is not in range of valid XTerm colors or RGB hex colors.
+        argparse.ArgumentTypeError: Argument value is not in range.
     """
 
-    METAVAR = "(XTerm [0-255] OR RGB Hex [000000-ffffff])"
+    METAVAR = "(float >= 0)"
 
     @staticmethod
-    def type_parser(arg: str) -> ColorType:
-        """Validates that the given argument is a valid color value.
+    def type_parser(arg: str) -> float:
+        """Validates that the given argument is a valid animationrate value. n >= 0.
 
         Args:
             arg (str): argument to validate
 
         Raises:
-            argparse.ArgumentTypeError: Color value is not in range.
+            argparse.ArgumentTypeError: Argument value is not in range.
 
         Returns:
-            Color : validated color value
+            float: validated value
         """
-        xterm_min = 0
-        xterm_max = 255
-        if len(arg) == 6:
-            # Check if the hex value is a valid color
-            if not 0 <= int(arg, 16) <= 16777215:
-                raise argparse.ArgumentTypeError(f"invalid color value: {arg} is not a valid hex color.")
-            return arg
-        else:
-            # Check if the color is a valid xterm color
-            if not xterm_min <= int(arg) <= xterm_max:
-                raise argparse.ArgumentTypeError(f"invalid color value: {arg} is not a valid xterm color (0-255).")
-            return int(arg)
+        if float(arg) < 0:
+            raise argparse.ArgumentTypeError(f"invalid argument value: '{arg}' is out of range. Must be float >= 0.")
+        return float(arg)
 
 
 class PositiveFloatRange:
     """Argument type for float ranges.
 
     Float ranges are a pair of positive floats separated by a hyphen. Ex: 0.1-1.0
 
@@ -146,52 +245,124 @@
             return start, end
         except ValueError:
             raise argparse.ArgumentTypeError(
                 f"invalid range: '{arg}' is not a valid range. Must be start-end. Ex: 0.1-1.0"
             )
 
 
-class IntRange:
-    """Argument type for integer ranges.
+class Ratio:
+    """Validates that the given argument is a valid float value between zero and one.
 
-    Integer ranges are a pair of integers separated by a hyphen. Ex: 1-10
+    0 <= float(n) <= 1
 
     Raises:
-        argparse.ArgumentTypeError: Value is not a valid range of integers.
+        argparse.ArgumentTypeError: Value is not in range.
     """
 
-    METAVAR = "(hyphen separated int range e.g. '1-10')"
+    METAVAR = "(0 <= float(n) <= 1)"
 
     @staticmethod
-    def type_parser(arg: str) -> tuple[int, int]:
-        """Validates that the given argument is a valid range of integers n > 0.
+    def type_parser(arg: str) -> float:
+        """Validates that the given argument is a valid float value between zero and one.
 
         Args:
             arg (str): argument to validate
 
+        Raises:
+            argparse.ArgumentTypeError: Value is not in range.
+
         Returns:
-            tuple[int,int]: validated range
+            float: validated float value
         """
-        try:
-            start, end = map(int, arg.split("-"))
-            if start <= 0:
-                raise argparse.ArgumentTypeError(
-                    f"invalid range: '{arg}' is not a valid range of ints. Must be start > 0. Ex: 1-10"
-                )
-            if start > end:
-                raise argparse.ArgumentTypeError(
-                    f"invalid range: '{arg}' is not a valid range of ints. Must be start <= end. Ex: 1-10"
-                )
-            return start, end
-        except ValueError:
+        if 0 <= float(arg) <= 1:
+            return float(arg)
+        else:
+            raise argparse.ArgumentTypeError(f"invalid value: '{arg}' is not a float >= 0 and <= 1. Example: 0.5")
+
+
+class CustomFormatter(argparse.ArgumentDefaultsHelpFormatter, argparse.RawDescriptionHelpFormatter):
+    """Custom formatter for argparse that combines ArgumentDefaultsHelpFormatter and RawDescriptionHelpFormatter."""
+
+    pass
+
+
+class GradientDirection:
+    """Argument type for gradient directions.
+
+    Raises:
+        argparse.ArgumentTypeError: Argument value is not a valid gradient direction.
+    """
+
+    METAVAR = "(diagonal, horizontal, vertical, center)"
+
+    @staticmethod
+    def type_parser(arg: str) -> Gradient.Direction:
+        """Validates that the given argument is a valid gradient direction.
+
+        Args:
+            arg (str): argument to validate
+
+        Returns:
+            Gradient.Direction: validated gradient direction
+
+        Raises:
+            argparse.ArgumentTypeError: Argument value is not a valid gradient direction.
+        """
+        direction_map = {
+            "horizontal": Gradient.Direction.HORIZONTAL,
+            "vertical": Gradient.Direction.VERTICAL,
+            "diagonal": Gradient.Direction.DIAGONAL,
+            "center": Gradient.Direction.CENTER,
+        }
+        if arg.lower() in direction_map:
+            return direction_map[arg.lower()]
+        else:
             raise argparse.ArgumentTypeError(
-                f"invalid range: '{arg}' is not a valid range. Must be start-end. Ex: 1-10"
+                f"invalid gradient direction: '{arg}' is not a valid gradient direction. Choices are diagonal, horizontal, vertical, or center."
             )
 
 
+class ColorArg:
+    """Argument type for color values.
+
+    Color values can be either an XTerm color value (0-255) or an RGB hex value (000000-ffffff).
+
+    Raises:
+        argparse.ArgumentTypeError: Value is not in range of valid XTerm colors or RGB hex colors.
+    """
+
+    METAVAR = "(XTerm [0-255] OR RGB Hex [000000-ffffff])"
+
+    @staticmethod
+    def type_parser(arg: str) -> ColorType:
+        """Validates that the given argument is a valid color value.
+
+        Args:
+            arg (str): argument to validate
+
+        Raises:
+            argparse.ArgumentTypeError: Color value is not in range.
+
+        Returns:
+            Color : validated color value
+        """
+        xterm_min = 0
+        xterm_max = 255
+        if len(arg) == 6:
+            # Check if the hex value is a valid color
+            if not 0 <= int(arg, 16) <= 16777215:
+                raise argparse.ArgumentTypeError(f"invalid color value: {arg} is not a valid hex color.")
+            return arg
+        else:
+            # Check if the color is a valid xterm color
+            if not xterm_min <= int(arg) <= xterm_max:
+                raise argparse.ArgumentTypeError(f"invalid color value: {arg} is not a valid xterm color (0-255).")
+            return int(arg)
+
+
 class Symbol:
     """Argument type for single ASCII/UTF-8 characters.
 
     Raises:
         argparse.ArgumentTypeError: Value is not a valid symbol.
     """
 
@@ -245,41 +416,14 @@
             return dimension
         except ValueError:
             raise argparse.ArgumentTypeError(
                 f"invalid terminal dimensions: '{arg}' is not a valid terminal dimension. Must be >= 0."
             )
 
 
-class PositiveInt:
-    """Argument type for positive integers.
-
-    int(n) > 0
-
-    Raises:
-        argparse.ArgumentTypeError: Value is not a positive integer.
-    """
-
-    METAVAR = "(int > 0)"
-
-    @staticmethod
-    def type_parser(arg: str) -> int:
-        """Validates that the given argument is a positive integer. n > 0.
-
-        Args:
-            arg (str): argument to validate
-
-        Returns:
-            int: validated positive integer
-        """
-        if int(arg) > 0:
-            return int(arg)
-        else:
-            raise argparse.ArgumentTypeError(f"invalid value: '{arg}' is not > 0.")
-
-
 class Ease:
     """Argument type for easing functions.
 
     Easing functions are prefixed by "in", "out", or "in_out" and suffixed by a valid easing function.
 
     Raises:
         argparse.ArgumentTypeError: Value is not a valid easing function.
@@ -297,14 +441,15 @@
         Raises:
             argparse.ArgumentTypeError: Ease value is not a valid easing function.
 
         Returns:
             Ease: validated ease value
         """
         easing_func_map = {
+            "linear": easing.linear,
             "in_sine": easing.in_sine,
             "out_sine": easing.out_sine,
             "in_out_sine": easing.in_out_sine,
             "in_quad": easing.in_quad,
             "out_quad": easing.out_quad,
             "in_out_quad": easing.in_out_quad,
             "in_cubic": easing.in_cubic,
@@ -335,128 +480,14 @@
 
         try:
             return easing_func_map[arg.lower()]
         except KeyError:
             raise argparse.ArgumentTypeError(f"invalid ease value: '{arg}' is not a valid ease.")
 
 
-class Ratio:
-    """Validates that the given argument is a valid float value between zero and one.
-
-    0 <= float(n) <= 1
-
-    Raises:
-        argparse.ArgumentTypeError: Value is not in range.
-    """
-
-    METAVAR = "(0 <= float(n) <= 1)"
-
-    @staticmethod
-    def type_parser(arg: str) -> float:
-        """Validates that the given argument is a valid float value between zero and one.
-
-        Args:
-            arg (str): argument to validate
-
-        Raises:
-            argparse.ArgumentTypeError: Value is not in range.
-
-        Returns:
-            float: validated float value
-        """
-        if 0 <= float(arg) <= 1:
-            return float(arg)
-        else:
-            raise argparse.ArgumentTypeError(f"invalid value: '{arg}' is not a float >= 0 and <= 1. Example: 0.5")
-
-
-class PositiveFloat:
-    """Validates that the given argument is a positive float. n > 0.
-
-    Raises:
-        argparse.ArgumentTypeError: Value is not in range.
-    """
-
-    METAVAR = "(float > 0)"
-
-    @staticmethod
-    def type_parser(arg: str) -> float:
-        """Validates that the given argument is a positive float. n > 0.
-
-        Args:
-            arg (str): argument to validate
-
-        Raises:
-            argparse.ArgumentTypeError: value is not in range.
-
-        Returns:
-            float: validated positive float
-        """
-        if float(arg) > 0:
-            return float(arg)
-        else:
-            raise argparse.ArgumentTypeError(
-                f"invalid value: '{arg}' is not a valid value. Argument must be a float > 0."
-            )
-
-
-class NonNegativeInt:
-    """Validates that the given argument is a nonnegative integer. n >= 0.
-
-    Raises:
-        argparse.ArgumentTypeError: Value is not in range.
-    """
-
-    METAVAR = "(int >= 0)"
-
-    @staticmethod
-    def type_parser(arg: str) -> int:
-        """Validates that the given argument is a nonnegative integer. n >= 0.
-
-        Args:
-            arg (str): argument to validate
-
-        Raises:
-            argparse.ArgumentTypeError: Value is not in range.
-
-        Returns:
-            int: validated gap value
-        """
-        if int(arg) < 0:
-            raise argparse.ArgumentTypeError(f"invalid value: '{arg}' Argument must be int >= 0.")
-        return int(arg)
-
-
-class NonNegativeFloat:
-    """Validates that the given argument is a valid animationrate value. n >= 0.
-
-    Raises:
-        argparse.ArgumentTypeError: Argument value is not in range.
-    """
-
-    METAVAR = "(float >= 0)"
-
-    @staticmethod
-    def type_parser(arg: str) -> float:
-        """Validates that the given argument is a valid animationrate value. n >= 0.
-
-        Args:
-            arg (str): argument to validate
-
-        Raises:
-            argparse.ArgumentTypeError: Argument value is not in range.
-
-        Returns:
-            float: validated value
-        """
-        if float(arg) < 0:
-            raise argparse.ArgumentTypeError(f"invalid argument value: '{arg}' is out of range. Must be float >= 0.")
-        return float(arg)
-
-
 def is_ascii_or_utf8(s: str) -> bool:
     """Tests if the given string is either ASCII or UTF-8.
 
     Args:
         s (str): string to test
 
     Returns:
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/utils/argsdataclass.py` & `terminaltexteffects-0.9.0/terminaltexteffects/utils/argsdataclass.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,31 @@
+"""
+This module defines classes and functions designed to work with the argparse library and enable typed arguments to support interacting with terminaltexteffects as both a command line tool and a library.
+
+The ArgField class extends the built-in Field class to include additional metadata specific to command-line arguments.
+This metadata includes the command-line argument name, help text, type parser, metavar, nargs, action, required status,
+and choices.
+
+The ArgParserDescriptor dataclass contains required attributes to call the "add_parser()" method of the _argparse._SubParsersAction class.
+
+The ArgsDataClass dataclass represents command-line arguments and provides methods for handling them. It does not define any fields itself but is meant to be subclassed, with subclasses defining their own fields to represent the command-line arguments they expect.
+
+Classes:
+    ArgField: A subclass of the dataclasses.Field class that represents a command-line argument.
+    ArgParserDescriptor: A dataclass that contains required attributes to call "add_parser()" method of the _argparse._SubParsersAction" class.
+    ArgsDataClass: A dataclass that represents command-line arguments and provides methods for handling them.
+
+"""
+
 import argparse
 import inspect
 import typing
 from dataclasses import MISSING, Field, dataclass, fields
 
-from terminaltexteffects.utils.arg_validators import CustomFormatter
+from terminaltexteffects.utils.argvalidators import CustomFormatter
 
 
 class ArgField(Field):
     """
     A subclass of the dataclasses.Field class that represents a command-line argument.
 
     This class extends the built-in Field class to include additional metadata specific to command-line arguments.
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/utils/easing.py` & `terminaltexteffects-0.9.0/terminaltexteffects/utils/easing.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,470 +1,520 @@
+"""This module contains functions for easing calculations.
+
+Functions:
+    linear: Linear easing function.
+    in_sine: Ease in using a sine function.
+    out_sine: Ease out using a sine function.
+    in_out_sine: Ease in/out using a sine function.
+    in_quad: Ease in using a quadratic function.
+    out_quad: Ease out using a quadratic function.
+    in_out_quad: Ease in/out using a quadratic function.
+    in_cubic: Ease in using a cubic function.
+    out_cubic: Ease out using a cubic function.
+    in_out_cubic: Ease in/out using a cubic function.
+    in_quart: Ease in using a quartic function.
+    out_quart: Ease out using a quartic function.
+    in_out_quart: Ease in/out using a quartic function.
+    in_quint: Ease in using a quintic function.
+    out_quint: Ease out using a quintic function.
+    in_out_quint: Ease in/out using a quintic function.
+    in_expo: Ease in using an exponential function.
+    out_expo: Ease out using an exponential function.
+    in_out_expo: Ease in/out using an exponential function.
+    in_circ: Ease in using a circular function.
+    out_circ: Ease out using a circular function.
+    in_out_circ: Ease in/out using a circular function.
+    in_back: Ease in using a back function.
+    out_back: Ease out using a back function.
+    in_out_back: Ease in/out using a back function.
+    in_elastic: Ease in using an elastic function.
+    out_elastic: Ease out using an elastic function.
+    in_out_elastic: Ease in/out using an elastic function.
+    in_bounce: Ease in using a bounce function.
+    out_bounce: Ease out using a bounce function.
+    in_out_bounce: Ease in/out using a bounce function.
+"""
+
 import math
 import typing
 
 EasingFunction: typing.TypeAlias = typing.Callable[[float], float]
+"EasingFunctions are Callable[[float], float] functions that take a float between 0 and 1 and return a float between 0 and 1."
+
+
+def linear(progress_ratio: float) -> float:
+    """
+    Linear easing function.
+
+    Args:
+        progress_ratio (float): the ratio of the current step to the maximum steps
+
+    Returns:
+        float: 0 <= n <= 1 eased value
+    """
+    return progress_ratio
 
 
-def in_sine(step_ratio: float) -> float:
+def in_sine(progress_ratio: float) -> float:
     """
     Ease in using a sine function.
 
     Args:
-        step_ratio (float): the ratio of the current step to the maximum steps
+        progress_ratio (float): the ratio of the current step to the maximum steps
 
     Returns:
-        float: 0 <= n <= 1 representing the percent of the inter waypoint distance to travel
+        float: 0 <= n <= 1 eased value
     """
-    return 1 - math.cos((step_ratio * math.pi) / 2)
+    return 1 - math.cos((progress_ratio * math.pi) / 2)
 
 
-def out_sine(step_ratio: float) -> float:
+def out_sine(progress_ratio: float) -> float:
     """
     Ease out using a sine function.
 
     Args:
-        step_ratio (float): the ratio of the current step to the maximum steps
+        progress_ratio (float): the ratio of the current step to the maximum steps
 
     Returns:
-        float: 0 <= n <= 1 representing the percent of the inter waypoint distance to travel
+        float: 0 <= n <= 1 eased value
     """
-    return math.sin((step_ratio * math.pi) / 2)
+    return math.sin((progress_ratio * math.pi) / 2)
 
 
-def in_out_sine(step_ratio: float) -> float:
+def in_out_sine(progress_ratio: float) -> float:
     """
     Ease in/out using a sine function.
 
     Args:
-        step_ratio (float): the ratio of the current step to the maximum steps
+        progress_ratio (float): the ratio of the current step to the maximum steps
 
     Returns:
-        float: 0 <= n <= 1 representing the percent of the inter waypoint distance to travel
+        float: 0 <= n <= 1 eased value
     """
 
-    return -(math.cos(math.pi * step_ratio) - 1) / 2
+    return -(math.cos(math.pi * progress_ratio) - 1) / 2
 
 
-def in_quad(step_ratio: float) -> float:
+def in_quad(progress_ratio: float) -> float:
     """
     Ease in using a quadratic function.
 
     Args:
-        step_ratio (float): the ratio of the current step to the maximum steps
+        progress_ratio (float): the ratio of the current step to the maximum steps
 
     Returns:
-        float: 0 <= n <= 1 representing the percent of the inter waypoint distance to travel
+        float: 0 <= n <= 1 eased value
     """
 
-    return step_ratio**2
+    return progress_ratio**2
 
 
-def out_quad(step_ratio: float) -> float:
+def out_quad(progress_ratio: float) -> float:
     """
     Ease out using a quadratic function.
 
     Args:
-        step_ratio (float): the ratio of the current step to the maximum steps
+        progress_ratio (float): the ratio of the current step to the maximum steps
 
     Returns:
-        float: 0 <= n <= 1 representing the percent of the inter waypoint distance to travel
+        float: 0 <= n <= 1 eased value
 
     """
-    return 1 - (1 - step_ratio) * (1 - step_ratio)
+    return 1 - (1 - progress_ratio) * (1 - progress_ratio)
 
 
-def in_out_quad(step_ratio: float) -> float:
+def in_out_quad(progress_ratio: float) -> float:
     """
     Ease in/out using a quadratic function.
 
     Args:
-        step_ratio (float): the ratio of the current step to the maximum steps
+        progress_ratio (float): the ratio of the current step to the maximum steps
 
     Returns:
-        float: 0 <= n <= 1 representing the percent of the inter waypoint distance to travel
+        float: 0 <= n <= 1 eased value
 
     """
-    if step_ratio < 0.5:
-        return 2 * step_ratio**2
+    if progress_ratio < 0.5:
+        return 2 * progress_ratio**2
     else:
-        return 1 - (-2 * step_ratio + 2) ** 2 / 2
+        return 1 - (-2 * progress_ratio + 2) ** 2 / 2
 
 
-def in_cubic(step_ratio: float) -> float:
+def in_cubic(progress_ratio: float) -> float:
     """
     Ease in using a cubic function.
 
     Args:
-        step_ratio (float): the ratio of the current step to the maximum steps
+        progress_ratio (float): the ratio of the current step to the maximum steps
 
     Returns:
-        float: 0 <= n <= 1 representing the percent of the inter waypoint distance to travel
+        float: 0 <= n <= 1 eased value
     """
-    return step_ratio**3
+    return progress_ratio**3
 
 
-def out_cubic(step_ratio: float) -> float:
+def out_cubic(progress_ratio: float) -> float:
     """
     Ease out using a cubic function.
 
     Args:
-        step_ratio (float): the ratio of the current step to the maximum steps
+        progress_ratio (float): the ratio of the current step to the maximum steps
 
     Returns:
-        float: 0 <= n <= 1 representing the percent of the inter waypoint distance to travel
+        float: 0 <= n <= 1 eased value
     """
-    return 1 - (1 - step_ratio) ** 3
+    return 1 - (1 - progress_ratio) ** 3
 
 
-def in_out_cubic(step_ratio: float) -> float:
+def in_out_cubic(progress_ratio: float) -> float:
     """
     Ease in/out using a cubic function.
 
     Args:
-        step_ratio (float): the ratio of the current step to the maximum steps
+        progress_ratio (float): the ratio of the current step to the maximum steps
 
     Returns:
         float: 0 <= n <= 1 representing the percentage of the current waypoint speed to apply to the
         character
     """
-    if step_ratio < 0.5:
-        return 4 * step_ratio**3
+    if progress_ratio < 0.5:
+        return 4 * progress_ratio**3
     else:
-        return 1 - (-2 * step_ratio + 2) ** 3 / 2
+        return 1 - (-2 * progress_ratio + 2) ** 3 / 2
 
 
-def in_quart(step_ratio: float) -> float:
+def in_quart(progress_ratio: float) -> float:
     """
     Ease in using a quartic function.
 
     Args:
-        step_ratio (float): the ratio of the current step to the maximum steps
+        progress_ratio (float): the ratio of the current step to the maximum steps
 
     Returns:
         float: 0 <= n <= 1 representing the percentage
         of the current waypoint speed to apply to the character
     """
-    return step_ratio**4
+    return progress_ratio**4
 
 
-def out_quart(step_ratio: float) -> float:
+def out_quart(progress_ratio: float) -> float:
     """
     Ease out using a quartic function.
 
     Args:
-        step_ratio (float): the ratio of the current step to the maximum steps
+        progress_ratio (float): the ratio of the current step to the maximum steps
 
     Returns:
-        float: 0 <= n <= 1 representing the percent of the inter waypoint distance to travel
+        float: 0 <= n <= 1 eased value
     """
-    return 1 - (1 - step_ratio) ** 4
+    return 1 - (1 - progress_ratio) ** 4
 
 
-def in_out_quart(step_ratio: float) -> float:
+def in_out_quart(progress_ratio: float) -> float:
     """
     Ease in/out using a quartic function.
 
     Args:
-        step_ratio (float): the ratio of the current step to the maximum steps
+        progress_ratio (float): the ratio of the current step to the maximum steps
 
     Returns:
-        float: 0 <= n <= 1 representing the percent of the inter waypoint distance to travel
+        float: 0 <= n <= 1 eased value
     """
-    if step_ratio < 0.5:
-        return 8 * step_ratio**4
+    if progress_ratio < 0.5:
+        return 8 * progress_ratio**4
     else:
-        return 1 - (-2 * step_ratio + 2) ** 4 / 2
+        return 1 - (-2 * progress_ratio + 2) ** 4 / 2
 
 
-def in_quint(step_ratio: float) -> float:
+def in_quint(progress_ratio: float) -> float:
     """
     Ease in using a quintic function.
 
     Args:
-        step_ratio (float): the ratio of the current step to the maximum steps
+        progress_ratio (float): the ratio of the current step to the maximum steps
 
     Returns:
-        float: 0 <= n <= 1 representing the percent of the inter waypoint distance to travel
+        float: 0 <= n <= 1 eased value
     """
-    return step_ratio**5
+    return progress_ratio**5
 
 
-def out_quint(step_ratio: float) -> float:
+def out_quint(progress_ratio: float) -> float:
     """
     Ease out using a quintic function.
 
     Args:
-        step_ratio (float): the ratio of the current step to the maximum steps
+        progress_ratio (float): the ratio of the current step to the maximum steps
 
     Returns:
-        float: 0 <= n <= 1 representing the percent of the inter waypoint distance to travel
+        float: 0 <= n <= 1 eased value
     """
-    return 1 - (1 - step_ratio) ** 5
+    return 1 - (1 - progress_ratio) ** 5
 
 
-def in_out_quint(step_ratio: float) -> float:
+def in_out_quint(progress_ratio: float) -> float:
     """
     Ease in/out using a quintic function.
 
     Args:
-        step_ratio (float): the ratio of the current step to the maximum steps
+        progress_ratio (float): the ratio of the current step to the maximum steps
 
     Returns:
-        float: 0 <= n <= 1 representing the percent of the inter waypoint distance to travel
+        float: 0 <= n <= 1 eased value
     """
-    if step_ratio < 0.5:
-        return 16 * step_ratio**5
+    if progress_ratio < 0.5:
+        return 16 * progress_ratio**5
     else:
-        return 1 - (-2 * step_ratio + 2) ** 5 / 2
+        return 1 - (-2 * progress_ratio + 2) ** 5 / 2
 
 
-def in_expo(step_ratio: float) -> float:
+def in_expo(progress_ratio: float) -> float:
     """
     Ease in using an exponential function.
 
     Args:
-        step_ratio (float): the ratio of the current step to the maximum steps
+        progress_ratio (float): the ratio of the current step to the maximum steps
 
     Returns:
-        float: 0 <= n <= 1 representing the percent of the inter waypoint distance to travel
+        float: 0 <= n <= 1 eased value
     """
-    if step_ratio == 0:
+    if progress_ratio == 0:
         return 0
     else:
-        return 2 ** (10 * step_ratio - 10)
+        return 2 ** (10 * progress_ratio - 10)
 
 
-def out_expo(step_ratio: float) -> float:
+def out_expo(progress_ratio: float) -> float:
     """
     Ease out using an exponential function.
 
     Args:
-        step_ratio (float): the ratio of the current step to the maximum steps
+        progress_ratio (float): the ratio of the current step to the maximum steps
 
     Returns:
-        float: 0 <= n <= 1 representing the percent of the inter waypoint distance to travel
+        float: 0 <= n <= 1 eased value
     """
-    if step_ratio == 1:
+    if progress_ratio == 1:
         return 1
     else:
-        return 1 - 2 ** (-10 * step_ratio)
+        return 1 - 2 ** (-10 * progress_ratio)
 
 
-def in_out_expo(step_ratio: float) -> float:
+def in_out_expo(progress_ratio: float) -> float:
     """
     Ease in/out using an exponential function.
 
     Args:
-        step_ratio (float): the ratio of the current step to the maximum steps
+        progress_ratio (float): the ratio of the current step to the maximum steps
 
     Returns:
-        float: 0 <= n <= 1 representing the percent of the inter waypoint distance to travel
+        float: 0 <= n <= 1 eased value
     """
-    if step_ratio == 0:
+    if progress_ratio == 0:
         return 0
-    elif step_ratio == 1:
+    elif progress_ratio == 1:
         return 1
-    elif step_ratio < 0.5:
-        return 2 ** (20 * step_ratio - 10) / 2
+    elif progress_ratio < 0.5:
+        return 2 ** (20 * progress_ratio - 10) / 2
     else:
-        return (2 - 2 ** (-20 * step_ratio + 10)) / 2
+        return (2 - 2 ** (-20 * progress_ratio + 10)) / 2
 
 
-def in_circ(step_ratio: float) -> float:
+def in_circ(progress_ratio: float) -> float:
     """
     Ease in using a circular function.
 
     Args:
-        step_ratio (float): the ratio of the current step to the maximum steps
+        progress_ratio (float): the ratio of the current step to the maximum steps
 
     Returns:
-        float: 0 <= n <= 1 representing the percent of the inter waypoint distance to travel
+        float: 0 <= n <= 1 eased value
     """
-    return 1 - math.sqrt(1 - step_ratio**2)
+    return 1 - math.sqrt(1 - progress_ratio**2)
 
 
-def out_circ(step_ratio: float) -> float:
+def out_circ(progress_ratio: float) -> float:
     """
     Ease out using a circular function.
 
     Args:
-        step_ratio (float): the ratio of the current step to the maximum steps
+        progress_ratio (float): the ratio of the current step to the maximum steps
 
     Returns:
-        float: 0 <= n <= 1 representing the percent of the inter waypoint distance to travel
+        float: 0 <= n <= 1 eased value
     """
-    return math.sqrt(1 - (step_ratio - 1) ** 2)
+    return math.sqrt(1 - (progress_ratio - 1) ** 2)
 
 
-def in_out_circ(step_ratio: float) -> float:
+def in_out_circ(progress_ratio: float) -> float:
     """
     Ease in/out using a circular function.
 
     Args:
-        step_ratio (float): the ratio of the current step to the maximum steps
+        progress_ratio (float): the ratio of the current step to the maximum steps
 
     Returns:
-        float: 0 <= n <= 1 representing the percent of the inter waypoint distance to travel
+        float: 0 <= n <= 1 eased value
     """
-    if step_ratio < 0.5:
-        return (1 - math.sqrt(1 - (2 * step_ratio) ** 2)) / 2
+    if progress_ratio < 0.5:
+        return (1 - math.sqrt(1 - (2 * progress_ratio) ** 2)) / 2
     else:
-        return (math.sqrt(1 - (-2 * step_ratio + 2) ** 2) + 1) / 2
+        return (math.sqrt(1 - (-2 * progress_ratio + 2) ** 2) + 1) / 2
 
 
-def in_back(step_ratio: float) -> float:
+def in_back(progress_ratio: float) -> float:
     """
     Ease in using a back function.
 
     Args:
-        step_ratio (float): the ratio of the current step to the maximum steps
+        progress_ratio (float): the ratio of the current step to the maximum steps
 
     Returns:
-        float: 0 <= n <= 1 representing the percent of the inter waypoint distance to travel
+        float: 0 <= n <= 1 eased value
     """
     c1 = 1.70158
     c3 = c1 + 1
-    return c3 * step_ratio**3 - c1 * step_ratio**2
+    return c3 * progress_ratio**3 - c1 * progress_ratio**2
 
 
-def out_back(step_ratio: float) -> float:
+def out_back(progress_ratio: float) -> float:
     """
     Ease out using a back function.
 
     Args:
-        step_ratio (float): the ratio of the current step to the maximum steps
+        progress_ratio (float): the ratio of the current step to the maximum steps
 
     Returns:
-        float: 0 <= n <= 1 representing the percent of the inter waypoint distance to travel
+        float: 0 <= n <= 1 eased value
     """
     c1 = 1.70158
     c3 = c1 + 1
-    return 1 + c3 * (step_ratio - 1) ** 3 + c1 * (step_ratio - 1) ** 2
+    return 1 + c3 * (progress_ratio - 1) ** 3 + c1 * (progress_ratio - 1) ** 2
 
 
-def in_out_back(step_ratio: float) -> float:
+def in_out_back(progress_ratio: float) -> float:
     """
     Ease in/out using a back function.
 
     Args:
-        step_ratio (float): the ratio of the current step to the maximum steps
+        progress_ratio (float): the ratio of the current step to the maximum steps
 
     Returns:
-        float: 0 <= n <= 1 representing the percent of the inter waypoint distance to travel
+        float: 0 <= n <= 1 eased value
     """
     c1 = 1.70158
     c2 = c1 * 1.525
-    if step_ratio < 0.5:
-        return ((2 * step_ratio) ** 2 * ((c2 + 1) * 2 * step_ratio - c2)) / 2
+    if progress_ratio < 0.5:
+        return ((2 * progress_ratio) ** 2 * ((c2 + 1) * 2 * progress_ratio - c2)) / 2
     else:
-        return ((2 * step_ratio - 2) ** 2 * ((c2 + 1) * (step_ratio * 2 - 2) + c2) + 2) / 2
+        return ((2 * progress_ratio - 2) ** 2 * ((c2 + 1) * (progress_ratio * 2 - 2) + c2) + 2) / 2
 
 
-def in_elastic(step_ratio: float) -> float:
+def in_elastic(progress_ratio: float) -> float:
     """
     Ease in using an elastic function.
 
     Args:
-        step_ratio (float): the ratio of the current step to the maximum steps
+        progress_ratio (float): the ratio of the current step to the maximum steps
 
     Returns:
-        float: 0 <= n <= 1 representing the percent of the inter waypoint distance to travel
+        float: 0 <= n <= 1 eased value
     """
 
     c4 = (2 * math.pi) / 3
-    if step_ratio == 0:
+    if progress_ratio == 0:
         return 0
-    elif step_ratio == 1:
+    elif progress_ratio == 1:
         return 1
     else:
-        return -(2 ** (10 * step_ratio - 10)) * math.sin((step_ratio * 10 - 10.75) * c4)
+        return -(2 ** (10 * progress_ratio - 10)) * math.sin((progress_ratio * 10 - 10.75) * c4)
 
 
-def out_elastic(step_ratio: float) -> float:
+def out_elastic(progress_ratio: float) -> float:
     """
     Ease out using an elastic function.
 
     Args:
-        step_ratio (float): the ratio of the current step to the maximum steps
+        progress_ratio (float): the ratio of the current step to the maximum steps
 
     Returns:
         float: 0 <= n <= 1 representing the percentage of the current waypoint speed to apply to the character
     """
     c4 = (2 * math.pi) / 3
-    if step_ratio == 0:
+    if progress_ratio == 0:
         return 0
-    elif step_ratio == 1:
+    elif progress_ratio == 1:
         return 1
     else:
-        return 2 ** (-10 * step_ratio) * math.sin((step_ratio * 10 - 0.75) * c4) + 1
+        return 2 ** (-10 * progress_ratio) * math.sin((progress_ratio * 10 - 0.75) * c4) + 1
 
 
-def in_out_elastic(step_ratio: float) -> float:
+def in_out_elastic(progress_ratio: float) -> float:
     """
     Ease in/out using an elastic function.
 
     Args:
-        step_ratio (float): the ratio of the current step to the maximum steps
+        progress_ratio (float): the ratio of the current step to the maximum steps
 
     Returns:
         float: 0 <= n <= 1 representing the percentage of the current waypoint speed to apply to the character
     """
     c5 = (2 * math.pi) / 4.5
-    if step_ratio == 0:
+    if progress_ratio == 0:
         return 0
-    elif step_ratio == 1:
+    elif progress_ratio == 1:
         return 1
-    elif step_ratio < 0.5:
-        return -(2 ** (20 * step_ratio - 10) * math.sin((20 * step_ratio - 11.125) * c5)) / 2
+    elif progress_ratio < 0.5:
+        return -(2 ** (20 * progress_ratio - 10) * math.sin((20 * progress_ratio - 11.125) * c5)) / 2
     else:
-        return (2 ** (-20 * step_ratio + 10) * math.sin((20 * step_ratio - 11.125) * c5)) / 2 + 1
+        return (2 ** (-20 * progress_ratio + 10) * math.sin((20 * progress_ratio - 11.125) * c5)) / 2 + 1
 
 
-def in_bounce(step_ratio: float) -> float:
+def in_bounce(progress_ratio: float) -> float:
     """
     Ease in using a bounce function.
 
     Args:
-        step_ratio (float): the ratio of the current step to the maximum steps
+        progress_ratio (float): the ratio of the current step to the maximum steps
 
     Returns:
         float: 0 <= n <= 1 representing the percentage of the current waypoint speed to apply to the character
     """
-    return 1 - out_bounce(1 - step_ratio)
+    return 1 - out_bounce(1 - progress_ratio)
 
 
-def out_bounce(step_ratio: float) -> float:
+def out_bounce(progress_ratio: float) -> float:
     """
     Ease out using a bounce function.
 
     Args:
-        step_ratio (float): the ratio of the current step to the maximum steps
+        progress_ratio (float): the ratio of the current step to the maximum steps
 
     Returns:
-        float: 0 <= n <= 1 representing the percent of the inter waypoint distance to travel
+        float: 0 <= n <= 1 eased value
     """
     n1 = 7.5625
     d1 = 2.75
-    if step_ratio < 1 / d1:
-        return n1 * step_ratio**2
-    elif step_ratio < 2 / d1:
-        return n1 * (step_ratio - 1.5 / d1) ** 2 + 0.75
-    elif step_ratio < 2.5 / d1:
-        return n1 * (step_ratio - 2.25 / d1) ** 2 + 0.9375
+    if progress_ratio < 1 / d1:
+        return n1 * progress_ratio**2
+    elif progress_ratio < 2 / d1:
+        return n1 * (progress_ratio - 1.5 / d1) ** 2 + 0.75
+    elif progress_ratio < 2.5 / d1:
+        return n1 * (progress_ratio - 2.25 / d1) ** 2 + 0.9375
     else:
-        return n1 * (step_ratio - 2.625 / d1) ** 2 + 0.984375
+        return n1 * (progress_ratio - 2.625 / d1) ** 2 + 0.984375
 
 
-def in_out_bounce(step_ratio: float) -> float:
+def in_out_bounce(progress_ratio: float) -> float:
     """
     Ease in/out using a bounce function.
 
     Args:
-        step_ratio (float): the ratio of the current step to the maximum steps
+        progress_ratio (float): the ratio of the current step to the maximum steps
 
     Returns:
-        float: 0 <= n <= 1 representing the percent of the inter waypoint distance to travel
+        float: 0 <= n <= 1 eased value
     """
-    if step_ratio < 0.5:
-        return (1 - out_bounce(1 - 2 * step_ratio)) / 2
+    if progress_ratio < 0.5:
+        return (1 - out_bounce(1 - 2 * progress_ratio)) / 2
     else:
-        return (1 + out_bounce(2 * step_ratio - 1)) / 2
+        return (1 + out_bounce(2 * progress_ratio - 1)) / 2
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/utils/geometry.py` & `terminaltexteffects-0.9.0/terminaltexteffects/utils/geometry.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 """
 This module provides utility functions for geometric calculations and operations.
 
+The purpose of these functions is to find terminal coordinates that fall within certain regions or along certain paths. These functions are
+used by effects to enable more complex animations and movement paths.
+
 Functions:
-- find_coords_on_circle: Finds points on a circle given the origin, radius, and number of points.
-- find_coords_in_circle: Finds coordinates within an ellipse given the center and major axis length.
-- find_coords_in_rect: Finds coordinates within a rectangle given the origin and distance.
-- find_coord_at_distance: Finds the coordinate at a given distance along a line defined by two coordinates.
-- find_coord_on_bezier_curve: Finds points on a quadratic or cubic bezier curve.
-- find_coord_on_line: Finds points on a line.
-- find_length_of_bezier_curve: Finds the length of a quadratic or cubic bezier curve.
-- find_length_of_line: Finds the length of a line intersecting two coordinates.
+    find_coords_on_circle: Finds points on a circle given the origin, radius, and number of points.
+    find_coords_in_circle: Finds coordinates within an ellipse given the center and major axis length.
+    find_coords_in_rect: Finds coordinates within a rectangle given the origin and distance.
+    find_coord_at_distance: Finds the coordinate at a given distance along a line defined by two coordinates.
+    find_coord_on_bezier_curve: Finds points on a quadratic or cubic bezier curve.
+    find_coord_on_line: Finds points on a line.
+    find_length_of_bezier_curve: Finds the length of a quadratic or cubic bezier curve.
+    find_length_of_line: Finds the length of a line intersecting two coordinates.
+    find_normalized_distance_from_center: Returns the normalized distance from the center of the OutputArea.
 """
 
 import math
 from dataclasses import dataclass
 
 
 @dataclass(eq=True, frozen=True)
@@ -212,16 +216,15 @@
 def find_length_of_line(coord1: Coord, coord2: Coord, double_row_diff: bool = False) -> float:
     """Returns the length of the line intersecting coord1 and coord2. If double_row_diff is True, the distance is
     doubled to account for the terminal character height/width ratio.
 
     Args:
         coord1 (Coord): first coordinate.
         coord2 (Coord): second coordinate.
-        double_row_diff (bool, optional): whether to double the row difference to account for terminal character height/width ratio. Defaults to
-        False.
+        double_row_diff (bool, optional): whether to double the row difference to account for terminal character height/width ratio. Defaults to False.
 
     Returns:
         float: length of the line
     """
     column_diff = coord2.column - coord1.column
     row_diff = coord2.row - coord1.row
     if double_row_diff:
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/utils/graphics.py` & `terminaltexteffects-0.9.0/terminaltexteffects/utils/graphics.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,25 @@
-"""Classes for storing and manipulating character graphics."""
+"""Classes for storing and manipulating character graphics.
+
+Classes:
+    Gradient: A Gradient is a list of RGB hex color strings transitioning from one color to another.
+"""
 
 import itertools
 import typing
 from collections.abc import Iterator
 from enum import Enum, auto
 
-from terminaltexteffects.utils import colorterm, geometry, hexterm
+from terminaltexteffects.utils import ansitools, colorterm, geometry, hexterm
 
 if typing.TYPE_CHECKING:
     pass
 
 Color: typing.TypeAlias = int | str
+"Colors are either XTerm-256 color codes (int 0 -> 255) or RGB hex color strings (000000 -> ffffff)."
 
 
 class Gradient:
     """A Gradient is a list of RGB hex color strings transitioning from one color to another. The gradient color
     list is calculated using linear interpolation based on the provided start and end colors and the number of steps. Gradients
     can be iterated over to get the next color in the gradient color list. If there is only one color in the stops list,
     the gradient will be a list of the same color.
@@ -25,40 +30,55 @@
     Ex: stops = ("ffffff", "aaaaaa", "000000"), steps = (6, 3)
 
     "fffffff" -> (6 steps) -> "aaaaaa" -> (3 steps) -> "000000"
 
     The step count includes the stop for each pair. Total number of colors in the resulting gradient spectrum is the sum of the steps between
     each pair of stops plus 1.
 
-    Args:
-        *stops (Color): RGB hex color strings or XTerm-256 color codes. Each stop will have steps number of frames between it and the next stop.
-        steps tuple[int, ...] | int: Number of steps from the start to the end stop. If multiple steps are given, steps and stops will be paired.
-
     Attributes:
         spectrum (list[str]): List (length=sum(steps) + 1) of RGB hex color strings
 
     """
 
     class Direction(Enum):
         """Enum for specifying the direction of the gradient."""
 
         VERTICAL = auto()
         HORIZONTAL = auto()
         CENTER = auto()
         DIAGONAL = auto()
 
     def __init__(self, *stops: Color, steps: int | tuple[int, ...] = 1) -> None:
-        self.stops = stops
-        if len(self.stops) < 1:
+        """
+        Initializes a Graphics object.
+
+        Args:
+            stops (Color): Variable number of Color objects representing the color stops.
+            steps (int | tuple[int, ...], optional): Number of steps or a tuple of step values for generating the spectrum. Defaults to 1.
+
+        Raises:
+            ValueError: If no color stops are provided.
+
+        Attributes:
+            stops (tuple[Color]): Tuple of Color objects representing the color stops.
+            steps (int | tuple[int, ...]): Number of steps or a tuple of step values for generating the spectrum.
+            spectrum (list[str]): List of strings representing the generated spectrum.
+            index (int): Current index of the spectrum.
+
+        Returns:
+            None
+        """
+        self._stops = stops
+        if len(self._stops) < 1:
             raise ValueError("At least one stop must be provided.")
-        self.steps = steps
-        self.spectrum: list[str] = self._generate(self.steps)
-        self.index: int = 0
+        self._steps = steps
+        self.spectrum: list[str] = self._generate(self._steps)
+        self._index: int = 0
 
-    def get_color_at_fraction(self, fraction: float) -> Color:
+    def get_color_at_fraction(self, fraction: float) -> str:
         """Returns the color at a fraction of the gradient.
 
         Args:
             fraction (float): The fraction of the gradient to get the color for.
 
         Returns:
             str: The color at the fraction of the gradient.
@@ -89,22 +109,22 @@
         """
         if isinstance(steps, int):
             steps = (steps,)
             for step in steps:
                 if step < 1:
                     raise ValueError("Steps must be greater than 0.")
         spectrum: list[str] = []
-        if len(self.stops) == 1:
-            color = self.stops[0]
+        if len(self._stops) == 1:
+            color = self._stops[0]
             if isinstance(color, int):
                 color = hexterm.xterm_to_hex(color)
             for _ in range(steps[0]):
                 spectrum.append(color)
             return spectrum
-        color_pairs = list(itertools.pairwise(self.stops))
+        color_pairs = list(itertools.pairwise(self._stops))
         steps = steps[: len(color_pairs)]
         for color_pair, steps in itertools.zip_longest(color_pairs, steps, fillvalue=steps[-1]):
             start, end = color_pair
             # Convert start_color to hex if it's an XTerm-256 color code
             if isinstance(start, int):
                 start = hexterm.xterm_to_hex(start)
             # Convert end_color to hex if it's an XTerm-256 color code
@@ -140,14 +160,16 @@
         return spectrum
 
     def build_coordinate_color_mapping(
         self, max_row: int, max_column: int, direction: "Gradient.Direction"
     ) -> dict[geometry.Coord, Color]:
         """Builds a mapping of coordinates to colors based on the gradient and a direction.
 
+        For example, a vertical gradient will have the same color for each column in a row. When applied across all characters in the output area, the gradient will be visible as a vertical gradient.
+
         Args:
             max_row (int): The maximum row value.
             max_column (int): The maximum column value.
             direction (Gradient.Direction): The direction of the gradient.
 
         Returns:
             dict[Coord, str]: A mapping of coordinates to colors.
@@ -185,9 +207,9 @@
     def __iter__(self) -> Iterator[str]:
         yield from self.spectrum
 
     def __len__(self) -> int:
         return len(self.spectrum)
 
     def __str__(self) -> str:
-        color_blocks = [f"{colorterm.fg(color)}█{colorterm.RESET}" for color in self.spectrum]
-        return f"Gradient: Stops({self.stops}), Steps({self.steps})\n" + "".join(color_blocks)
+        color_blocks = [f"{colorterm.fg(color)}█{ansitools.RESET_ALL()}" for color in self.spectrum]
+        return f"Gradient: Stops({self._stops}), Steps({self._steps})\n" + "".join(color_blocks)
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/utils/hexterm.py` & `terminaltexteffects-0.9.0/terminaltexteffects/utils/hexterm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
-#!/usr/bin/python3
+"""This module contains a list of all XTerm-256 color codes and functions to convert between RGB Hex color strings and XTerm-256 color codes.
 
-"""Convert between RGB Hex color strings and XTerm-256 color codes."""
+Functions:
+    hex_to_xterm: Convert RGB Hex colors to their closest XTerm-256 color.
+    xterm_to_hex: Convert XTerm-256 color codes to RGB Hex colors.
+    is_valid_color: Check if the input is a valid RGB Hex color code.
+"""
 
 xterm_to_hex_map = {
     0: "#000000",
     1: "#800000",
     2: "#008000",
     3: "#808000",
     4: "#000080",
```

### Comparing `terminaltexteffects-0.8.0/terminaltexteffects/utils/terminal.py` & `terminaltexteffects-0.9.0/terminaltexteffects/engine/terminal.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,47 @@
-"""A module for managing the terminal state and output."""
+"""A module for managing the terminal state and output.
+
+Classes:
+    TerminalConfig: Configuration for the terminal.
+    OutputArea: Represents the output area in the terminal. The output area is the area defined by the dimensions of the input data, unless specified otherwise in the TerminalConfig.
+    Terminal: A class for managing the terminal state and output.
+"""
 
 import random
 import shutil
 import sys
 import time
 from dataclasses import dataclass
 from enum import Enum, auto
 
-import terminaltexteffects.utils.arg_validators as arg_validators
-from terminaltexteffects.base_character import EffectCharacter
+import terminaltexteffects.utils.argvalidators as argvalidators
+from terminaltexteffects.engine.base_character import EffectCharacter
 from terminaltexteffects.utils import ansitools
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass
 from terminaltexteffects.utils.geometry import Coord
 
 
 @dataclass
 class TerminalConfig(ArgsDataClass):
     """Configuration for the terminal.
 
     Attributes:
         tab_width (int): Number of spaces to use for a tab character.
         xterm_colors (bool): Convert any colors specified in RBG hex to the closest XTerm-256 color.
         no_color (bool): Disable all colors in the effect.
-        no_wrap (int): Disable wrapping of text.
-        animation_rate (float): Minimum time, in seconds, between animation steps.
-        use_terminal_dimensions (bool): Use the terminal dimensions to limit the size of the output area and support wrapping. If False, the output area is determined by the input data dimensions and may overflow the terminal width."""
+        wrap_text (bool): Wrap text wider than the output area width.
+        frame_rate (float): Target frame rate for the animation.
+        terminal_dimensions (tuple[int, int]): Terminal dimensions as (width, height), if set to (0,0) the terminal dimensions are detected automatically.
+        ignore_terminal_dimensions (bool): Ignore the terminal dimensions and use the input data dimensions for the output area.
+    """
 
     tab_width: int = ArgField(
         cmd_name=["--tab-width"],
-        type_parser=arg_validators.PositiveInt.type_parser,
-        metavar=arg_validators.PositiveInt.METAVAR,
+        type_parser=argvalidators.PositiveInt.type_parser,
+        metavar=argvalidators.PositiveInt.METAVAR,
         default=4,
         help="Number of spaces to use for a tab character.",
     )  # type: ignore[assignment]
 
     "int : Number of spaces to use for a tab character."
 
     xterm_colors: bool = ArgField(
@@ -54,24 +62,24 @@
     wrap_text: int = ArgField(
         cmd_name="--wrap-text", default=False, action="store_true", help="Wrap text wider than the output area width."
     )  # type: ignore[assignment]
     "bool : Wrap text wider than the output area width."
 
     frame_rate: float = ArgField(
         cmd_name="--frame-rate",
-        type_parser=arg_validators.PositiveInt.type_parser,
+        type_parser=argvalidators.PositiveInt.type_parser,
         default=100,
         help="""Target frame rate for the animation.""",
     )  # type: ignore[assignment]
 
-    "float : Minimum time, in seconds, between animation steps."
+    "float : Minimum time, in seconds, between frames."
 
     terminal_dimensions: tuple[int, int] = ArgField(
         cmd_name=["--terminal-dimensions"],
-        type_parser=arg_validators.TerminalDimensions.type_parser,
+        type_parser=argvalidators.TerminalDimensions.type_parser,
         nargs=2,
         default=(0, 0),
         help="Use the terminal dimensions to limit the size of the output area and support wrapping. If False, the output area is determined by the input data dimensions and may overflow the terminal width.",
     )  # type: ignore[assignment]
 
     "tuple(int,int) : Terminal dimensions as (width, height), if set to (0,0) the terminal dimensions are detected automatically."
 
@@ -82,22 +90,37 @@
         help="Ignore the terminal dimensions and use the input data dimensions for the output area.",
     )  # type: ignore[assignment]
     "bool : Ignore the terminal dimensions and use the input data dimensions for the output area."
 
 
 @dataclass
 class OutputArea:
-    """A class for storing the output area of an effect.
+    """Represents the output area in the terminal. The output area is the area defined
+    by the dimensions of the input data, unless specified otherwise in the TerminalConfig.
+
+    This class provides methods for working with the output area, such as checking if a coordinate is within the output area,
+    getting random coordinates within the output area, and getting a random coordinate outside the output area.
 
     Args:
         top (int): top row of the output area
         right (int): right column of the output area
         bottom (int): bottom row of the output area. Defaults to 1.
         left (int): left column of the output area. Defaults to 1.
 
+    Attributes:
+        center_row (int): row of the center of the output area
+        center_column (int): column of the center of the output area
+        center (Coord): coordinate of the center of the output area
+
+    Methods:
+        coord_is_in_output_area(coord: Coord) -> bool: Checks whether a coordinate is within the output area.
+        random_column() -> int: Get a random column position within the output area.
+        random_row() -> int: Get a random row position within the output area.
+        random_coord(outside_scope=False) -> Coord: Get a random coordinate within or outside the output area.
+
     """
 
     top: int
     right: int
     bottom: int = 1
     left: int = 1
 
@@ -146,75 +169,122 @@
             random_coord_right = Coord(self.right + 1, self.random_row())
             return random.choice([random_coord_above, random_coord_below, random_coord_left, random_coord_right])
         else:
             return Coord(self.random_column(), self.random_row())
 
 
 class Terminal:
-    """A class for managing the terminal state and output."""
+    """A class for managing the terminal state and output.
+
+    Attributes:
+        config (TerminalConfig): Configuration for the terminal.
+        output_area (OutputArea): The output area in the terminal.
+        character_by_input_coord (dict[Coord, EffectCharacter]): A dictionary of characters by their input coordinates.
+
+    Methods:
+        get_piped_input() -> str: Gets the piped input from stdin.
+        prep_outputarea(): Prepares the terminal for the effect by adding empty lines and hiding the cursor.
+        restore_cursor(): Restores the cursor visibility.
+        get_characters(input_characters: bool = True, fill_chars: bool = False, added_chars: bool = False, sort: CharacterSort = CharacterSort.TOP_TO_BOTTOM_LEFT_TO_RIGHT) -> list[EffectCharacter]: Get a list of all EffectCharacters in the terminal with an optional sort.
+        get_characters_grouped(grouping: CharacterGroup = CharacterGroup.ROW_TOP_TO_BOTTOM, input_characters: bool = True, fill_chars: bool = False, added_chars: bool = False) -> list[list[EffectCharacter]]: Get a list of all EffectCharacters grouped by the specified CharacterGroup grouping.
+        get_character_by_input_coord(coord: Coord) -> EffectCharacter | None: Get an EffectCharacter by its input coordinates.
+        set_character_visibility(character: EffectCharacter, is_visible: bool): Set the visibility of a character.
+        get_formatted_output_string() -> str: Get the formatted output string based on the current terminal state.
+        print(output_string: str, enforce_frame_rate: bool = True): Prints the current terminal state to stdout while preserving the cursor position.
+
+    """
 
     class CharacterGroup(Enum):
-        """An enum for grouping characters."""
+        """An enum specifying character groupings.
+
+        Attributes:
+            COLUMN_LEFT_TO_RIGHT: Group characters by column from left to right.
+            COLUMN_RIGHT_TO_LEFT: Group characters by column from right to left.
+            ROW_TOP_TO_BOTTOM: Group characters by row from top to bottom.
+            ROW_BOTTOM_TO_TOP: Group characters by row from bottom to top.
+            DIAGONAL_TOP_LEFT_TO_BOTTOM_RIGHT: Group characters by diagonal from top left to bottom right.
+            DIAGONAL_BOTTOM_LEFT_TO_TOP_RIGHT: Group characters by diagonal from bottom left to top right.
+            DIAGONAL_TOP_RIGHT_TO_BOTTOM_LEFT: Group characters by diagonal from top right to bottom left.
+            DIAGONAL_BOTTOM_RIGHT_TO_TOP_LEFT: Group characters by diagonal from bottom right to top left.
+            CENTER_TO_OUTSIDE_DIAMONDS: Group characters by distance from the center to the outside in diamond shapes.
+            OUTSIDE_TO_CENTER_DIAMONDS: Group characters by distance from the outside to the center in diamond shapes.
+        """
 
         COLUMN_LEFT_TO_RIGHT = auto()
         COLUMN_RIGHT_TO_LEFT = auto()
         ROW_TOP_TO_BOTTOM = auto()
         ROW_BOTTOM_TO_TOP = auto()
         DIAGONAL_TOP_LEFT_TO_BOTTOM_RIGHT = auto()
         DIAGONAL_BOTTOM_LEFT_TO_TOP_RIGHT = auto()
         DIAGONAL_TOP_RIGHT_TO_BOTTOM_LEFT = auto()
         DIAGONAL_BOTTOM_RIGHT_TO_TOP_LEFT = auto()
         CENTER_TO_OUTSIDE_DIAMONDS = auto()
         OUTSIDE_TO_CENTER_DIAMONDS = auto()
 
     class CharacterSort(Enum):
-        """An enum for sorting characters."""
+        """An enum for specifying character sorts.
+
+        Attributes:
+            RANDOM: Random order.
+            TOP_TO_BOTTOM_LEFT_TO_RIGHT: Top to bottom, left to right.
+            TOP_TO_BOTTOM_RIGHT_TO_LEFT: Top to bottom, right to left.
+            BOTTOM_TO_TOP_LEFT_TO_RIGHT: Bottom to top, left to right.
+            BOTTOM_TO_TOP_RIGHT_TO_LEFT: Bottom to top, right to left.
+            OUTSIDE_ROW_TO_MIDDLE: Outside row to middle.
+            MIDDLE_ROW_TO_OUTSIDE: Middle row to outside.
+        """
 
         RANDOM = auto()
         TOP_TO_BOTTOM_LEFT_TO_RIGHT = auto()
         TOP_TO_BOTTOM_RIGHT_TO_LEFT = auto()
         BOTTOM_TO_TOP_LEFT_TO_RIGHT = auto()
         BOTTOM_TO_TOP_RIGHT_TO_LEFT = auto()
         OUTSIDE_ROW_TO_MIDDLE = auto()
         MIDDLE_ROW_TO_OUTSIDE = auto()
 
     def __init__(self, input_data: str, config: TerminalConfig | None = None):
+        """Initializes the Terminal object.
+
+        Args:
+            input_data (str): The input data to be displayed in the terminal.
+            config (TerminalConfig, optional): Configuration for the terminal. Defaults to None.
+        """
         if config is None:
             self.config = TerminalConfig()
         else:
             self.config = config
         if not input_data:
             input_data = "No Input."
-        self.input_data = input_data.replace("\t", " " * self.config.tab_width)
+        self._input_data = input_data.replace("\t", " " * self.config.tab_width)
         if self.config.ignore_terminal_dimensions:
-            self.width = max([len(line) for line in self.input_data.splitlines()])
-            self.height = len(self.input_data.splitlines()) + 1
+            self._width = max([len(line) for line in self._input_data.splitlines()])
+            self._height = len(self._input_data.splitlines()) + 1
         elif self.config.terminal_dimensions == (0, 0):
-            self.width, self.height = self._get_terminal_dimensions()
+            self._width, self._height = self._get_terminal_dimensions()
         else:
-            self.width, self.height = self.config.terminal_dimensions
-        self.next_character_id = 0
+            self._width, self._height = self.config.terminal_dimensions
+        self._next_character_id = 0
         self._input_characters = self._decompose_input(self.config.xterm_colors, self.config.no_color)
         self._added_characters: list[EffectCharacter] = []
-        self.input_width = max([character.input_coord.column for character in self._input_characters])
-        self.input_height = max([character.input_coord.row for character in self._input_characters])
-        self.output_area = OutputArea(min(self.height - 1, self.input_height), self.input_width)
+        self._input_width = max([character.input_coord.column for character in self._input_characters])
+        self._input_height = max([character.input_coord.row for character in self._input_characters])
+        self.output_area = OutputArea(min(self._height - 1, self._input_height), self._input_width)
         self._input_characters = [
             character
             for character in self._input_characters
             if character.input_coord.row <= self.output_area.top
             and character.input_coord.column <= self.output_area.right
         ]
         self.character_by_input_coord: dict[Coord, EffectCharacter] = {
             (character.input_coord): character for character in self._input_characters
         }
         self._fill_characters = self._make_fill_characters()
-        self.visible_characters: set[EffectCharacter] = set()
-        self.frame_rate = self.config.frame_rate
-        self.last_time_printed = time.time()
+        self._visible_characters: set[EffectCharacter] = set()
+        self._frame_rate = self.config.frame_rate
+        self._last_time_printed = time.time()
         self._update_terminal_state()
 
     def _get_terminal_dimensions(self) -> tuple[int, int]:
         """Gets the terminal dimensions.
 
         Returns:
             tuple[int, int]: terminal width and height
@@ -253,17 +323,17 @@
             lines (list): The lines of text to be wrapped.
 
         Returns:
             list: The wrapped lines of text.
         """
         wrapped_lines = []
         for line in lines:
-            while len(line) > self.width:
-                wrapped_lines.append(line[: self.width])
-                line = line[self.width :]
+            while len(line) > self._width:
+                wrapped_lines.append(line[: self._width])
+                line = line[self._width :]
             wrapped_lines.append(line)
         return wrapped_lines
 
     def _decompose_input(self, use_xterm_colors: bool, no_color: bool) -> list[EffectCharacter]:
         """Decomposes the output into a list of Character objects containing the symbol and its row/column coordinates
         relative to the input display location.
 
@@ -273,71 +343,71 @@
         Args:
             use_xterm_colors (bool): whether to convert colors to the closest XTerm-256 color
 
         Returns:
             list[Character]: list of EffectCharacter objects
         """
         formatted_lines = []
-        if not self.input_data.strip():
-            self.input_data = "No Input."
-        lines = self.input_data.splitlines()
-        formatted_lines = self._wrap_lines(lines) if self.config.wrap_text else [line[: self.width] for line in lines]
+        if not self._input_data.strip():
+            self._input_data = "No Input."
+        lines = self._input_data.splitlines()
+        formatted_lines = self._wrap_lines(lines) if self.config.wrap_text else [line[: self._width] for line in lines]
         input_height = len(formatted_lines)
         input_characters = []
         for row, line in enumerate(formatted_lines):
             for column, symbol in enumerate(line):
                 if symbol != " ":
-                    character = EffectCharacter(self.next_character_id, symbol, column + 1, input_height - row)
+                    character = EffectCharacter(self._next_character_id, symbol, column + 1, input_height - row)
                     character.animation.use_xterm_colors = use_xterm_colors
                     character.animation.no_color = no_color
                     input_characters.append(character)
-                    self.next_character_id += 1
+                    self._next_character_id += 1
         return input_characters
 
     def _make_fill_characters(self) -> list[EffectCharacter]:
         """Creates a list of characters to fill the empty spaces in the output area. The characters input_symbol is a space.
         The fill characters are added to the character_by_input_coord dictionary.
 
         Returns:
             list[EffectCharacter]: list of characters
         """
         fill_characters = []
         for row in range(1, self.output_area.top + 1):
             for column in range(1, self.output_area.right + 1):
                 coord = Coord(column, row)
                 if coord not in self.character_by_input_coord:
-                    fill_char = EffectCharacter(self.next_character_id, " ", column, row)
+                    fill_char = EffectCharacter(self._next_character_id, " ", column, row)
                     fill_characters.append(fill_char)
                     self.character_by_input_coord[coord] = fill_char
-                    self.next_character_id += 1
+                    self._next_character_id += 1
         return fill_characters
 
     def add_character(self, symbol: str, coord: Coord) -> EffectCharacter:
         """Adds a character to the terminal for printing. Used to create characters that are not in the input data.
 
         Args:
             symbol (str): symbol to add
             coord: (Coord): set character's input coordinates
 
         Returns:
             EffectCharacter: the character that was added
         """
-        character = EffectCharacter(self.next_character_id, symbol, coord.column, coord.row)
+        character = EffectCharacter(self._next_character_id, symbol, coord.column, coord.row)
         character.animation.use_xterm_colors = self.config.xterm_colors
         character.animation.no_color = self.config.no_color
         self._added_characters.append(character)
-        self.next_character_id += 1
+        self._next_character_id += 1
         return character
 
     def _update_terminal_state(self):
         """Update the internal representation of the terminal state with the current position
         of all visible characters.
         """
         rows = [[" " for _ in range(self.output_area.right)] for _ in range(self.output_area.top)]
-        for character in sorted(self.visible_characters, key=lambda c: c.layer):
+        for character in sorted(self._visible_characters, key=lambda c: c.layer):
             row = character.motion.current_coord.row - 1
             column = character.motion.current_coord.column - 1
             if 0 <= row < self.output_area.top and 0 <= column < self.output_area.right:
                 rows[row][column] = character.symbol
         terminal_state = ["".join(row) for row in rows]
         self.terminal_state = terminal_state
 
@@ -527,17 +597,17 @@
 
         Args:
             character (EffectCharacter): the character to set visibility for
             is_visible (bool): whether the character should be visible
         """
         character._is_visible = is_visible
         if is_visible:
-            self.visible_characters.add(character)
+            self._visible_characters.add(character)
         else:
-            self.visible_characters.discard(character)
+            self._visible_characters.discard(character)
 
     def get_formatted_output_string(self) -> str:
         """Get the formatted output string based on the current terminal state.
 
         This method updates the internal terminal representation state before returning the formatted output string.
 
         Returns:
@@ -557,18 +627,18 @@
         Notes:
             This method includes animation timing to control the frame rate.
             If the time since the last print is less than required to limit the frame rate, the method will sleep for the remaining time
             to ensure a consistent animation speed.
 
         """
         if enforce_frame_rate:
-            frame_delay = 1 / self.frame_rate
-            time_since_last_print = time.time() - self.last_time_printed
+            frame_delay = 1 / self._frame_rate
+            time_since_last_print = time.time() - self._last_time_printed
             if time_since_last_print < frame_delay:
                 time.sleep(frame_delay - time_since_last_print)
         sys.stdout.write(ansitools.DEC_SAVE_CURSOR_POSITION())
         sys.stdout.write(ansitools.MOVE_CURSOR_UP(self.output_area.top))
         sys.stdout.write(ansitools.MOVE_CURSOR_TO_COLUMN(1))
         sys.stdout.write(output_string)
         sys.stdout.write(ansitools.DEC_RESTORE_CURSOR_POSITION())
         sys.stdout.flush()
-        self.last_time_printed = time.time()
+        self._last_time_printed = time.time()
```

