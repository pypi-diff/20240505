# Comparing `tmp/sophie-lang-0.0.6.tar.gz` & `tmp/sophie-lang-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sophie-lang-0.0.6.tar", last modified: Wed Mar 27 23:42:28 2024, max compression
+gzip compressed data, was "sophie-lang-0.0.7.tar", last modified: Sat May  4 22:11:51 2024, max compression
```

## Comparing `sophie-lang-0.0.6.tar` & `sophie-lang-0.0.7.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 23:42:28.172666 sophie-lang-0.0.6/
--rw-rw-rw-   0        0        0     1086 2022-10-16 03:53:26.000000 sophie-lang-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     5993 2024-03-27 23:42:28.171669 sophie-lang-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     5138 2024-03-27 23:32:26.000000 sophie-lang-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2024-03-27 23:42:28.172666 sophie-lang-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1379 2024-03-27 23:29:28.000000 sophie-lang-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-27 23:42:28.064983 sophie-lang-0.0.6/sophie/
--rw-rw-rw-   0        0        0    33667 2024-03-24 01:16:32.000000 sophie-lang-0.0.6/sophie/Sophie.automaton
--rw-rw-rw-   0        0        0        0 2022-10-09 04:11:54.000000 sophie-lang-0.0.6/sophie/__init__.py
--rw-rw-rw-   0        0        0       41 2023-07-01 03:52:18.000000 sophie-lang-0.0.6/sophie/__main__.py
-drwxrwxrwx   0        0        0        0 2024-03-27 23:42:28.110859 sophie-lang-0.0.6/sophie/adapters/
--rw-rw-rw-   0        0        0        0 2023-05-08 04:47:45.000000 sophie-lang-0.0.6/sophie/adapters/__init__.py
--rw-rw-rw-   0        0        0      459 2024-01-29 03:19:56.000000 sophie-lang-0.0.6/sophie/adapters/fs_adapter.py
--rw-rw-rw-   0        0        0     6622 2024-03-24 07:00:34.000000 sophie-lang-0.0.6/sophie/adapters/game_adapter.py
--rw-rw-rw-   0        0        0      482 2024-01-26 00:26:59.000000 sophie-lang-0.0.6/sophie/adapters/teletype_adapter.py
--rw-rw-rw-   0        0        0     1899 2023-12-22 05:00:24.000000 sophie-lang-0.0.6/sophie/adapters/turtle_adapter.py
--rw-rw-rw-   0        0        0      824 2024-03-05 02:21:52.000000 sophie-lang-0.0.6/sophie/adapters/yarn.py
--rw-rw-rw-   0        0        0    15412 2024-03-24 09:33:52.000000 sophie-lang-0.0.6/sophie/calculus.py
--rw-rw-rw-   0        0        0     2090 2024-02-19 07:02:27.000000 sophie-lang-0.0.6/sophie/cmdline.py
--rw-rw-rw-   0        0        0     6556 2024-03-07 05:18:41.000000 sophie-lang-0.0.6/sophie/demand.py
--rw-rw-rw-   0        0        0    16672 2024-03-24 06:20:55.000000 sophie-lang-0.0.6/sophie/diagnostics.py
--rw-rw-rw-   0        0        0     3825 2024-03-24 08:42:47.000000 sophie-lang-0.0.6/sophie/executive.py
--rw-rw-rw-   0        0        0     7522 2024-02-19 21:40:34.000000 sophie-lang-0.0.6/sophie/front_end.py
--rw-rw-rw-   0        0        0    25481 2024-03-26 06:48:28.000000 sophie-lang-0.0.6/sophie/intermediate.py
--rw-rw-rw-   0        0        0     3371 2023-09-08 05:15:09.000000 sophie-lang-0.0.6/sophie/modularity.py
--rw-rw-rw-   0        0        0     1705 2024-03-19 05:24:34.000000 sophie-lang-0.0.6/sophie/ontology.py
--rw-rw-rw-   0        0        0      613 2023-12-03 06:54:57.000000 sophie-lang-0.0.6/sophie/primitive.py
--rw-rw-rw-   0        0        0    23915 2024-03-24 08:42:32.000000 sophie-lang-0.0.6/sophie/resolution.py
--rw-rw-rw-   0        0        0    15705 2024-03-24 08:32:49.000000 sophie-lang-0.0.6/sophie/runtime.py
--rw-rw-rw-   0        0        0     6947 2024-02-19 07:03:05.000000 sophie-lang-0.0.6/sophie/scheduler.py
--rw-rw-rw-   0        0        0     3896 2024-02-18 03:02:06.000000 sophie-lang-0.0.6/sophie/stacking.py
--rw-rw-rw-   0        0        0    19869 2024-03-24 08:45:37.000000 sophie-lang-0.0.6/sophie/syntax.py
-drwxrwxrwx   0        0        0        0 2024-03-27 23:42:28.131774 sophie-lang-0.0.6/sophie/sys/
--rw-rw-rw-   0        0        0      736 2024-03-19 04:35:35.000000 sophie-lang-0.0.6/sophie/sys/complex.sg
--rw-rw-rw-   0        0        0     2914 2024-03-24 01:30:10.000000 sophie-lang-0.0.6/sophie/sys/game.sg
--rw-rw-rw-   0        0        0     8454 2024-03-07 04:05:00.000000 sophie-lang-0.0.6/sophie/sys/preamble.sg
--rw-rw-rw-   0        0        0     9153 2024-03-03 09:25:40.000000 sophie-lang-0.0.6/sophie/sys/tree.sg
--rw-rw-rw-   0        0        0      519 2023-06-24 06:27:18.000000 sophie-lang-0.0.6/sophie/sys/turtle.sg
--rw-rw-rw-   0        0        0    42627 2024-03-24 09:31:34.000000 sophie-lang-0.0.6/sophie/type_evaluator.py
-drwxrwxrwx   0        0        0        0 2024-03-27 23:42:28.170672 sophie-lang-0.0.6/sophie_lang.egg-info/
--rw-rw-rw-   0        0        0     5993 2024-03-27 23:42:27.000000 sophie-lang-0.0.6/sophie_lang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      907 2024-03-27 23:42:27.000000 sophie-lang-0.0.6/sophie_lang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 23:42:27.000000 sophie-lang-0.0.6/sophie_lang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-03-27 23:42:27.000000 sophie-lang-0.0.6/sophie_lang.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       35 2024-03-27 23:42:27.000000 sophie-lang-0.0.6/sophie_lang.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-27 23:42:27.000000 sophie-lang-0.0.6/sophie_lang.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 22:11:51.854997 sophie-lang-0.0.7/
+-rw-rw-rw-   0        0        0     1086 2022-10-16 03:53:26.000000 sophie-lang-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     6123 2024-05-04 22:11:51.854997 sophie-lang-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5268 2024-05-04 22:11:35.000000 sophie-lang-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-04 22:11:51.855992 sophie-lang-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1379 2024-05-04 21:08:57.000000 sophie-lang-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 22:11:51.747283 sophie-lang-0.0.7/sophie/
+-rw-rw-rw-   0        0        0    34063 2024-04-25 05:04:56.000000 sophie-lang-0.0.7/sophie/Sophie.automaton
+-rw-rw-rw-   0        0        0        0 2022-10-09 04:11:54.000000 sophie-lang-0.0.7/sophie/__init__.py
+-rw-rw-rw-   0        0        0       41 2023-07-01 03:52:18.000000 sophie-lang-0.0.7/sophie/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 22:11:51.788173 sophie-lang-0.0.7/sophie/adapters/
+-rw-rw-rw-   0        0        0        0 2023-05-08 04:47:45.000000 sophie-lang-0.0.7/sophie/adapters/__init__.py
+-rw-rw-rw-   0        0        0      489 2024-04-18 04:24:17.000000 sophie-lang-0.0.7/sophie/adapters/fs_adapter.py
+-rw-rw-rw-   0        0        0     6718 2024-05-02 03:47:21.000000 sophie-lang-0.0.7/sophie/adapters/game_adapter.py
+-rw-rw-rw-   0        0        0      512 2024-04-18 04:24:17.000000 sophie-lang-0.0.7/sophie/adapters/teletype_adapter.py
+-rw-rw-rw-   0        0        0     1871 2024-04-18 05:08:56.000000 sophie-lang-0.0.7/sophie/adapters/turtle_adapter.py
+-rw-rw-rw-   0        0        0      926 2024-04-01 05:01:32.000000 sophie-lang-0.0.7/sophie/adapters/yarn.py
+-rw-rw-rw-   0        0        0    16065 2024-04-28 23:39:32.000000 sophie-lang-0.0.7/sophie/calculus.py
+-rw-rw-rw-   0        0        0     2090 2024-02-19 07:02:27.000000 sophie-lang-0.0.7/sophie/cmdline.py
+-rw-rw-rw-   0        0        0     7009 2024-04-16 04:17:38.000000 sophie-lang-0.0.7/sophie/demand.py
+-rw-rw-rw-   0        0        0    17560 2024-04-29 00:10:22.000000 sophie-lang-0.0.7/sophie/diagnostics.py
+-rw-rw-rw-   0        0        0     3866 2024-04-28 23:39:32.000000 sophie-lang-0.0.7/sophie/executive.py
+-rw-rw-rw-   0        0        0     7525 2024-04-25 05:03:58.000000 sophie-lang-0.0.7/sophie/front_end.py
+-rw-rw-rw-   0        0        0    25923 2024-05-02 04:38:28.000000 sophie-lang-0.0.7/sophie/intermediate.py
+-rw-rw-rw-   0        0        0     3415 2024-04-05 01:52:46.000000 sophie-lang-0.0.7/sophie/modularity.py
+-rw-rw-rw-   0        0        0     1705 2024-03-19 05:24:34.000000 sophie-lang-0.0.7/sophie/ontology.py
+-rw-rw-rw-   0        0        0      568 2024-04-16 06:09:16.000000 sophie-lang-0.0.7/sophie/primitive.py
+-rw-rw-rw-   0        0        0    25427 2024-04-25 05:05:29.000000 sophie-lang-0.0.7/sophie/resolution.py
+-rw-rw-rw-   0        0        0    14979 2024-04-29 00:20:40.000000 sophie-lang-0.0.7/sophie/runtime.py
+-rw-rw-rw-   0        0        0     6947 2024-02-19 07:03:05.000000 sophie-lang-0.0.7/sophie/scheduler.py
+-rw-rw-rw-   0        0        0     3584 2024-04-29 00:28:56.000000 sophie-lang-0.0.7/sophie/stacking.py
+-rw-rw-rw-   0        0        0    19704 2024-05-01 05:08:07.000000 sophie-lang-0.0.7/sophie/syntax.py
+drwxrwxrwx   0        0        0        0 2024-05-04 22:11:51.827099 sophie-lang-0.0.7/sophie/sys/
+-rw-rw-rw-   0        0        0     1009 2024-05-04 04:03:55.000000 sophie-lang-0.0.7/sophie/sys/2d.sg
+-rw-rw-rw-   0        0        0      736 2024-03-19 04:35:35.000000 sophie-lang-0.0.7/sophie/sys/complex.sg
+-rw-rw-rw-   0        0        0     2025 2024-05-04 04:06:42.000000 sophie-lang-0.0.7/sophie/sys/game.sg
+-rw-rw-rw-   0        0        0     8496 2024-03-29 23:15:50.000000 sophie-lang-0.0.7/sophie/sys/preamble.sg
+-rw-rw-rw-   0        0        0     9153 2024-03-03 09:25:40.000000 sophie-lang-0.0.7/sophie/sys/tree.sg
+-rw-rw-rw-   0        0        0      526 2024-04-18 05:01:23.000000 sophie-lang-0.0.7/sophie/sys/turtle.sg
+-rw-rw-rw-   0        0        0    44899 2024-05-02 03:38:47.000000 sophie-lang-0.0.7/sophie/type_evaluator.py
+drwxrwxrwx   0        0        0        0 2024-05-04 22:11:51.853000 sophie-lang-0.0.7/sophie_lang.egg-info/
+-rw-rw-rw-   0        0        0     6123 2024-05-04 22:11:51.000000 sophie-lang-0.0.7/sophie_lang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      924 2024-05-04 22:11:51.000000 sophie-lang-0.0.7/sophie_lang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 22:11:51.000000 sophie-lang-0.0.7/sophie_lang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-04 22:11:51.000000 sophie-lang-0.0.7/sophie_lang.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       35 2024-05-04 22:11:51.000000 sophie-lang-0.0.7/sophie_lang.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-04 22:11:51.000000 sophie-lang-0.0.7/sophie_lang.egg-info/top_level.txt
```

### Comparing `sophie-lang-0.0.6/LICENSE` & `sophie-lang-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sophie-lang-0.0.6/PKG-INFO` & `sophie-lang-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sophie-lang
-Version: 0.0.6
+Version: 0.0.7
 Summary: A call-by-need strongly-static-duck-typed language named for French mathematician Sophie Germain
 Home-page: https://github.com/kjosib/sophie
 Author: Ian Kjos
 Author-email: kjosib@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
@@ -87,34 +87,35 @@
 
 There is now a [change log](https://github.com/kjosib/sophie/tree/main/CHANGELOG.md).
 
 Some things are going well:
 
 * A native-code [Virtual-Machine](https://github.com/kjosib/sophie/tree/main/vm) can run Sophie code at a respectable speed.
   It reads a "compiled" form which you can generate with a command-line like `sophie -x your/sophie/program.sg > program.is`.
-  It runs most of the examples just fine, but lags slightly behind on extensions.
 * Sophie has Turtle-graphics! (See [here](https://github.com/kjosib/sophie/blob/main/examples/turtle/turtle.sg) for examples.)
-* Sophie is interactive! See [this guessing game](https://github.com/kjosib/sophie/blob/main/examples/games/guess_the_number.sg) as an example.
+* Sophie is interactive! See [this guessing game](https://github.com/kjosib/sophie/blob/main/examples/games/guess_the_number.sg)
+  or this [Not-Quite-Pong game](https://github.com/kjosib/sophie/blob/main/examples/games/nqp.sg) as examples.
 * The type-checker gives excellent feedback and cannot be fooled.
   Through abstract interpretation it completely rules out *type* errors.
   (Domain errors, such as division by zero, are still possible.)
 * The module system got an upgrade: there is now a notion of a system-package and the beginnings of a standard library.
 * The FFI: Sophie can call Python; Python can call Sophie; and Python can install I/O drivers into Sophie.
   The same FFI directives on the Sophie side interact properly with the native-code VM.
 * Compile-time error display is generally clear and informative.
+* Operator overloading works via double-dispatch. Thus, the standard modules for complex-numbers and 2d vectors
+  both let you use ordinary arithmetic symbols to manipulate their respective data types.
 
 Some things are in progress:
 
 * SDL bindings (via PyGame for now). See for example this [graphical mouse-chaser](https://github.com/kjosib/sophie/blob/main/examples/games/mouse.sg).
-* Operator overloading.
 
-Certain things are not started yet:
+Certain things seem like nice ideas, but may not happen any time soon:
 
-* Variable-Arity Functions. (This may never happen.)
-* Ad-hoc polymorphic multi-methods. (This becomes less interesting once operator overloading gets finished.)
+* Variable-Arity Functions.
+* Ad-hoc polymorphic multi-methods.
 * List comprehension (expressions like `[expr FOR name IN expr]`) are removed from the syntax for now.
 
 ## Why not just use Language X, Y, or Z?
 
 Have you been paying attention?
 
 ## Long-Term Plans
```

### Comparing `sophie-lang-0.0.6/README.md` & `sophie-lang-0.0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -64,34 +64,35 @@
 
 There is now a [change log](https://github.com/kjosib/sophie/tree/main/CHANGELOG.md).
 
 Some things are going well:
 
 * A native-code [Virtual-Machine](https://github.com/kjosib/sophie/tree/main/vm) can run Sophie code at a respectable speed.
   It reads a "compiled" form which you can generate with a command-line like `sophie -x your/sophie/program.sg > program.is`.
-  It runs most of the examples just fine, but lags slightly behind on extensions.
 * Sophie has Turtle-graphics! (See [here](https://github.com/kjosib/sophie/blob/main/examples/turtle/turtle.sg) for examples.)
-* Sophie is interactive! See [this guessing game](https://github.com/kjosib/sophie/blob/main/examples/games/guess_the_number.sg) as an example.
+* Sophie is interactive! See [this guessing game](https://github.com/kjosib/sophie/blob/main/examples/games/guess_the_number.sg)
+  or this [Not-Quite-Pong game](https://github.com/kjosib/sophie/blob/main/examples/games/nqp.sg) as examples.
 * The type-checker gives excellent feedback and cannot be fooled.
   Through abstract interpretation it completely rules out *type* errors.
   (Domain errors, such as division by zero, are still possible.)
 * The module system got an upgrade: there is now a notion of a system-package and the beginnings of a standard library.
 * The FFI: Sophie can call Python; Python can call Sophie; and Python can install I/O drivers into Sophie.
   The same FFI directives on the Sophie side interact properly with the native-code VM.
 * Compile-time error display is generally clear and informative.
+* Operator overloading works via double-dispatch. Thus, the standard modules for complex-numbers and 2d vectors
+  both let you use ordinary arithmetic symbols to manipulate their respective data types.
 
 Some things are in progress:
 
 * SDL bindings (via PyGame for now). See for example this [graphical mouse-chaser](https://github.com/kjosib/sophie/blob/main/examples/games/mouse.sg).
-* Operator overloading.
 
-Certain things are not started yet:
+Certain things seem like nice ideas, but may not happen any time soon:
 
-* Variable-Arity Functions. (This may never happen.)
-* Ad-hoc polymorphic multi-methods. (This becomes less interesting once operator overloading gets finished.)
+* Variable-Arity Functions.
+* Ad-hoc polymorphic multi-methods.
 * List comprehension (expressions like `[expr FOR name IN expr]`) are removed from the syntax for now.
 
 ## Why not just use Language X, Y, or Z?
 
 Have you been paying attention?
 
 ## Long-Term Plans
```

### Comparing `sophie-lang-0.0.6/setup.py` & `sophie-lang-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 else:
 	make_tables(Path(__file__).parent / "sophie" / "Sophie.md")
 
 setuptools.setup(
 	name='sophie-lang',
 	author='Ian Kjos',
 	author_email='kjosib@gmail.com',
-	version='0.0.6',
+	version='0.0.7',
 	packages=['sophie', "sophie.adapters", ],
 	package_data={
 		'sophie': ["Sophie.automaton"]+["sys/"+f for f in os.listdir("sophie/sys")],
 	},
 	entry_points={
 		'console_scripts': ["sophie = sophie.cmdline:main"],
 	},
```

### Comparing `sophie-lang-0.0.6/sophie/adapters/game_adapter.py` & `sophie-lang-0.0.7/sophie/adapters/game_adapter.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 """
 import os
 os.environ["PYGAME_HIDE_SUPPORT_PROMPT"] = "1"
 import pygame
 from typing import Optional
 from pygame import draw, gfxdraw
 
-from ..runtime import iterate_list, force, Message, Action
+from ..runtime import iterate_list, force, ParametricMessage
 from ..scheduler import NativeObjectProxy
 
 linkage = {}
 
 def sophie_init(xy, mouse_event, button_event, key_event):
 	linkage['xy'] = xy
 	linkage['mouse_event'] = mouse_event
@@ -58,30 +58,30 @@
 	In concept you'd configure behavior by sending this messages.
 	A distinguished "play" message starts an event-loop on a dedicated thread.
 	
 	For now I'll stick to physical events, not logical ones like double-click or dragon-drop.
 	The alt-F4 quit-key combination comes across as a quit event, though.
 	"""
 	def __init__(self):
-		self._on_quit:Optional[Action] = None
-		self._on_mouse:Optional[Message] = None
-		self._on_button_down:Optional[Message] = None
-		self._on_button_up:Optional[Message] = None
-		self._on_key_down:Optional[Message] = None
-		self._on_key_up:Optional[Message] = None
-		self._on_tick:Optional[Message] = None
+		self._on_quit = None
+		self._on_mouse:Optional[ParametricMessage] = None
+		self._on_button_down:Optional[ParametricMessage] = None
+		self._on_button_up:Optional[ParametricMessage] = None
+		self._on_key_down:Optional[ParametricMessage] = None
+		self._on_key_up:Optional[ParametricMessage] = None
+		self._on_tick:Optional[ParametricMessage] = None
 	pass
 	
-	def on_quit(self, action:Action): self._on_quit = action
-	def on_mouse(self, message:Message): self._on_mouse = message
-	def on_button_down(self, message:Message): self._on_button_down = message
-	def on_button_up(self, message:Message): self._on_button_up = message
-	def on_key_down(self, message:Message): self._on_key_down = message
-	def on_key_up(self, message:Message): self._on_key_up = message
-	def on_tick(self, message:Message): self._on_tick = message
+	def on_quit(self, action): self._on_quit = action
+	def on_mouse(self, message:ParametricMessage): self._on_mouse = message
+	def on_button_down(self, message:ParametricMessage): self._on_button_down = message
+	def on_button_up(self, message:ParametricMessage): self._on_button_up = message
+	def on_key_down(self, message:ParametricMessage): self._on_key_down = message
+	def on_key_up(self, message:ParametricMessage): self._on_key_up = message
+	def on_tick(self, message:ParametricMessage): self._on_tick = message
 
 	def play(self, size, fps):
 		pygame.init()
 		width, height = force(size['x']), force(size['y'])
 		display = pygame.display.set_mode((width, height))
 		display_actor = NativeObjectProxy(DisplayProxy(display))
 
@@ -92,15 +92,15 @@
 					if self._on_quit is not None:
 						self._on_quit.perform()
 					return
 				elif event.type == pygame.MOUSEMOTION and self._on_mouse is not None:
 					self._on_mouse.dispatch_with(mouse_event(event))
 				elif event.type == pygame.MOUSEBUTTONDOWN and self._on_button_down is not None:
 					self._on_button_down.dispatch_with(button_event(event))
-				elif event.type == pygame.MOUSEBUTTONUP and self._on_button_down is not None:
+				elif event.type == pygame.MOUSEBUTTONUP and self._on_button_up is not None:
 					self._on_button_up.dispatch_with(button_event(event))
 				elif event.type == pygame.KEYDOWN and self._on_key_down is not None:
 					self._on_key_down.dispatch_with(key_event(event))
 				elif event.type == pygame.KEYUP and self._on_key_up is not None:
 					self._on_key_up.dispatch_with(key_event(event))
 
 			clock.tick(fps)
```

### Comparing `sophie-lang-0.0.6/sophie/adapters/turtle_adapter.py` & `sophie-lang-0.0.7/sophie/adapters/turtle_adapter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from ..runtime import force, iterate_list
 from ..scheduler import NativeObjectProxy, MAIN_QUEUE, SimpleTask
 import turtle, tkinter
 
-def sophie_init():
-	return {'drawing':some_turtle_graphics}
+def sophie_init(drawing):
+	return {drawing.key:some_turtle_graphics}
 
 def some_turtle_graphics(env, drawing):
-	task = SimpleTask(worker.accept_message, "draw", (env, drawing))
-	MAIN_QUEUE.execute(task)
+	worker.accept_message("draw", (env, drawing))
 
 class Worker:
 	@staticmethod
 	def draw(env, drawing):
 		tortoise.accept_message("begin", ())
 		stepCount = 0
 		block = []
@@ -42,15 +41,15 @@
 		t.screen.tracer(2 ^ 31)
 		t.screen.delay(0)
 		t.setheading(90)
 		
 	def block(self, steps):
 		t = self.yertle
 		for (tag, *args) in steps:
-			getattr(t, tag)(*args)
+			getattr(t, tag.nom.text)(*args)
 		t.screen.update()
 	
 	def finish(self, stepCount):
 		text = str(stepCount) + " turtle steps. Click the drawing or press any key to dismiss it."
 		print(text)
 		root = self.root
 		label = tkinter.Label(root, text=text)
```

### Comparing `sophie-lang-0.0.6/sophie/adapters/yarn.py` & `sophie-lang-0.0.7/sophie/adapters/yarn.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 """
 A host module for Sophie's nontrivial intrinsics, such as string functions,
 which have some impedance mismatch between the Sophie and Python conceptions.
 """
 
-from ..runtime import iterate_list
-
-nope = {"":"nope"}
+from ..runtime import iterate_list, as_sophie_list, sophie_nope, sophie_this
 
 def mid(aString, offset, size):
 	return aString[max(0, offset) : max(0, offset+size)]
 
 def val(aString):
 	try: answer = float(aString)
-	except ValueError: return nope
-	else: return {"":"this", "item":answer}
+	except ValueError: return sophie_nope()
+	else: return sophie_this(answer)
 
 def identity(x):
 	# This one's just for messing around with the type system.
 	# Something in the zoo-of-ok imports it across the FFI.
 	return x
 
 def join(xs):
@@ -26,7 +24,10 @@
 def is_match_at(offset, needle, haystack):
 	return offset >= 0 and needle == haystack[offset:offset+len(needle)]
 
 trim = str.strip
 ltrim = str.lstrip
 rtrim = str.rstrip
 
+def split_lines(s:str):
+	return as_sophie_list(s.splitlines(keepends=True))
+
```

### Comparing `sophie-lang-0.0.6/sophie/calculus.py` & `sophie-lang-0.0.7/sophie/calculus.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,29 @@
 """
 Part of the abstract-interpretation based type-checker.
 These bits represent the data over which the type-checker operates.
 To understand better, start by reading the "High-Order Type Checking"
 section at https://sophie.readthedocs.io/en/latest/mechanics.html
 
-This file is enumerates all kinds of types, which include first-order types like:
-	Type Variables (i.e. known-unknowns)
-	Nominal types (which refer back to symbols, and do by definition have exactly however many arguments as the symbol)
-	Arrow types (which generally have a product on the left)
-	Product types (which are generally found on the left side of an arrow)
-	Bottom (about which the algebraic laws are written at the link above)
-	Error: The type that means something went off the rails.
-	
-and also some additional type-operators:
-	FieldType: represents field-access as a function-like type.
-	UnionType: represents selection points which depend on run-time data, and a related concept with list syntax.
-	UDFType: Deals with user-defined functions which may be polymorphic in weird ways.
-	CallSiteType: Combines an arrow-type (or UDF) with an argument to get a result.
-
-I originally thought he type-numbering subsystem would mediate all interaction with concrete types.
+I originally thought the type-numbering subsystem would mediate all interaction with concrete types.
 Clients would call for what they mean to compose, and the subsystem would give back a type-number.
 Or, given a type-number, the subsystem could return a smart object.
 But then I remembered the rest of the world is only readable in terms of smart objects.
 Therefore, the present design maps all type-parameters to their exemplars,
 and uses type-numbering internally to make hash-checks and equality comparisons go fast.
 
 Conveniently, type-numbering is just an equivalence classification scheme.
 I can reuse the one from booze-tools.
 
 """
 from typing import Iterable
 from boozetools.support.foundation import EquivalenceClassifier
 from . import syntax
-from .ontology import Symbol
-from .stacking import Frame
+from .ontology import Symbol, SELF
+from .stacking import Frame, Activation
 
 TYPE_ENV = Frame["SophieType"]
 
 _type_numbering_subsystem = EquivalenceClassifier()
 
 class SophieType:
 	"""Value objects so they can play well with the classifier"""
@@ -54,60 +40,69 @@
 	def __eq__(self, other: "SophieType"): return type(self) is type(other) and self._key == other._key
 	def exemplar(self) -> "SophieType": return _type_numbering_subsystem.exemplars[self.number]
 	def __repr__(self) -> str:
 		it = self.visit(Render())
 		assert isinstance(it, str), (it, type(self))
 		return it
 
-class TypeVariable(SophieType):
+# Now, purely as an aid to understanding and recollection,
+# I divide the space of types into:
+# * Formal types, which exist independent of values in a simple Platonic algebra.
+# * Computed types, the projection of value-domain code into the realm of types.
+
+class FormalType(SophieType): pass
+class ComputedType(SophieType): pass
+
+class TypeVariable(FormalType):
 	"""Did I say value-object? Not for type variables! These have identity."""
 	def __init__(self):
 		super().__init__(len(_type_numbering_subsystem.catalog))
 	def visit(self, visitor:"TypeVisitor"): return visitor.on_variable(self)
 	def expected_arity(self) -> int: return -1  # Not callable
 
-class OpaqueType(SophieType):
+
+class OpaqueType(FormalType):
 	def __init__(self, symbol:syntax.Opaque):
 		assert type(symbol) is syntax.Opaque
 		self.symbol = symbol
 		super().__init__(symbol)
 	def visit(self, visitor:"TypeVisitor"): return visitor.on_opaque(self)
 	def expected_arity(self) -> int: return -1  # Not callable
 	def token(self): return self.symbol
 
 def _exemplargs(type_args: Iterable[SophieType], size) -> tuple[SophieType, ...]:
 	them = tuple(a.exemplar() for a in type_args)
 	assert len(them) == size, (len(them), size)
 	return them
 
-class RecordType(SophieType):
+class RecordType(FormalType):
 	def __init__(self, r:syntax.Record, type_args: Iterable[SophieType]):
 		assert type(r) is syntax.Record
 		self.symbol = r
 		self.type_args = _exemplargs(type_args, len(r.type_params))
 		super().__init__(self.symbol, *(a.number for a in self.type_args))
 	def visit(self, visitor:"TypeVisitor"): return visitor.on_record(self)
 	def expected_arity(self) -> int: return -1  # Not callable. (There's a constructor arrow made.)
 	def token(self): return self.symbol
 
-class SumType(SophieType):
+class SumType(FormalType):
 	""" Either a record directly, or a variant-type. Details are in the symbol table. """
 	# NB: The arguments here are actual arguments, not formal parameters.
 	#     The corresponding formal parameters are listed in the symbol,
 	#     itself being either a SubTypeSpec or a TypeDecl
 	def __init__(self, variant: syntax.Variant, type_args: Iterable[SophieType]):
 		assert isinstance(variant, syntax.Variant)
 		self.variant = variant
 		self.type_args = _exemplargs(type_args, len(variant.type_params))
 		super().__init__(self.variant, *(a.number for a in self.type_args))
 	def visit(self, visitor:"TypeVisitor"): return visitor.on_sum(self)
 	def expected_arity(self) -> int: return -1  # Not callable directly.
 	def token(self): return self.variant
 
-class SubType(SophieType):
+class SubType(FormalType):
 	st : syntax.SubTypeSpec
 	def expected_arity(self) -> int: return -1  # Not callable. (There's a constructor arrow made.)
 	def token(self): return self.st.variant
 
 class EnumType(SubType):
 	def __init__(self, st: syntax.SubTypeSpec):
 		assert st.body is None
@@ -122,56 +117,86 @@
 		assert isinstance(st.body, syntax.RecordSpec)
 		self.st = st
 		self.type_args = _exemplargs(type_args, len(st.variant.type_params))
 		super().__init__(st, *(a.number for a in self.type_args))
 	def visit(self, visitor:"TypeVisitor"): return visitor.on_tag_record(self)
 	def family(self) -> Symbol: return self.st.variant
 
-class ProductType(SophieType):
+class ProductType(FormalType):
 	def __init__(self, fields: Iterable[SophieType]):
 		self.fields = tuple(p.exemplar() for p in fields)
 		super().__init__(*(p.number for p in self.fields))
 	def visit(self, visitor:"TypeVisitor"): return visitor.on_product(self)
 	def expected_arity(self) -> int: return -1  # Not callable
 
-class ArrowType(SophieType):
+class ArrowType(FormalType):
 	def __init__(self, arg: ProductType, res: SophieType):
 		self.arg, self.res = arg.exemplar(), res.exemplar()
 		super().__init__(self.arg, self.res)
 	def visit(self, visitor:"TypeVisitor"): return visitor.on_arrow(self)
 	def expected_arity(self) -> int: return len(self.arg.fields)
 	def dispatch_signature(self) -> tuple[Symbol, ...]: return tuple(a.token() for a in self.arg.fields)
 
-class MessageType(SophieType):
+class MessageType(FormalType):
 	def __init__(self, arg: ProductType):
-		assert arg.fields
 		self.arg = arg
 		super().__init__(self.arg)
 	def visit(self, visitor: "TypeVisitor"): return visitor.on_message(self)
-	def expected_arity(self) -> int: return -1  # Not callable; sendable.
+	def expected_arity(self) -> int:
+		return len(self.arg.fields) or -1
 
-class UDFType(SophieType):
-	fn: syntax.UserFunction
+class InterfaceType(FormalType):
+	def __init__(self, symbol:syntax.Interface, type_args: Iterable[SophieType]):
+		assert type(symbol) is syntax.Interface
+		self.symbol = symbol
+		self.type_args = _exemplargs(type_args, len(symbol.type_params))
+		super().__init__(self.symbol, *(a.number for a in self.type_args))
+	def visit(self, visitor: "TypeVisitor"): return visitor.on_interface(self)
+	def expected_arity(self) -> int: return -1  # Not callable
+
+class SubroutineType(ComputedType):
+	"""
+	Supertype for those of procedures and functions,
+	because they have much structure in common.
+	"""
+	sub: syntax.Subroutine
 	static_link: TYPE_ENV
-	def visit(self, visitor:"TypeVisitor"): return visitor.on_udf(self)
-	def expected_arity(self) -> int: return len(self.fn.params)
-	def __init__(self, fn:syntax.UserFunction, static_link:TYPE_ENV):
-		self.fn = fn
+	
+	# Factoid: The static-link will contain a self-link in exactly the right cases,
+	# and then there's no need for separate task and message types.
+	# There's just a message type, always pointing to a UserProcType.
+	
+	def visit(self, visitor:"TypeVisitor"): return visitor.on_subroutine(self)
+	def expected_arity(self) -> int: return len(self.sub.params)
+	def __init__(self, sub:syntax.Subroutine, static_link:TYPE_ENV):
+		self.sub = sub
 		self.static_link = static_link
 		# NB: The uniqueness notion here is excessive, but there's a plan to deal with that.
 		#     Whatever instantiates a nested function must enter it in the static scope without duplication.
 		#     Performance hacking may make for an even better cache than that.
 		# TODO: It would be sufficient to key on the types captured in the lexical closure.
 		#       Only DeductionEngine.visit_Lookup creates these, so it could provide the capture.
 		super().__init__(object())
+
+class UserFnType(SubroutineType):
+	sub: syntax.UserFunction
+	def __init__(self, sub:syntax.UserFunction, static_link:TYPE_ENV):
+		assert isinstance(sub, syntax.UserFunction)
+		super().__init__(sub, static_link)
 	def dispatch_signature(self) -> tuple[Symbol, ...]:
-		assert isinstance(self.fn, syntax.UserOperator)
-		return self.fn.dispatch_vector()
+		assert isinstance(self.sub, syntax.UserOperator)
+		return self.sub.dispatch_vector()
+
+class UserProcType(SubroutineType):
+	sub: syntax.UserProcedure
+	def __init__(self, sub:syntax.UserProcedure, static_link:TYPE_ENV):
+		assert isinstance(sub, syntax.UserProcedure)
+		super().__init__(sub, static_link)
 
-class AdHocType(SophieType):
+class AdHocType(ComputedType):
 	def __init__(self, glyph:str, arity:int):
 		super().__init__(glyph, arity)
 		self.glyph = glyph
 		self._arity = arity
 		self._cases = {}
 	def visit(self, visitor:"TypeVisitor"): return visitor.on_ad_hoc(self)
 	def expected_arity(self) -> int: return self._arity
@@ -187,99 +212,98 @@
 		#  to the RoadMap object and make the resolver handle this.
 		arg_tokens = case.dispatch_signature()
 		if arg_tokens in self._cases: report.conflicting_overload()
 		elif not all(arg_tokens): report.unsuported_overrload()
 		elif len(arg_tokens) != self._arity: report.conflicting_overload()
 		else: self._cases[arg_tokens] = case
 
-class UserTaskType(SophieType):
-	""" The type of a task-ified user-defined (parametric) function. """
-	def __init__(self, udf_type:UDFType):
-		assert udf_type.fn.params
-		self.udf_type = udf_type.exemplar()
-		super().__init__(self.udf_type)
+class UserTaskType(ComputedType):
+	""" The type of a task-ified user-defined (maybe-parametric) procedure. """
+	def __init__(self, proc_type:UserProcType):
+		assert isinstance(proc_type.sub, syntax.UserProcedure), type(proc_type.sub)
+		self.proc_type = proc_type.exemplar()
+		super().__init__(self.proc_type)
 	def visit(self, visitor: "TypeVisitor"): return visitor.on_user_task(self)
-	def expected_arity(self) -> int: return self.udf_type.expected_arity()
+	def expected_arity(self) -> int: return self.proc_type.expected_arity()
 
-class InterfaceType(SophieType):
-	def __init__(self, symbol:syntax.Interface, type_args: Iterable[SophieType]):
-		assert type(symbol) is syntax.Interface
-		self.symbol = symbol
-		self.type_args = _exemplargs(type_args, len(symbol.type_params))
-		super().__init__(self.symbol, *(a.number for a in self.type_args))
-	def visit(self, visitor: "TypeVisitor"): return visitor.on_interface(self)
-	def expected_arity(self) -> int: return -1  # Not callable
-
-class _AgentDerived(SophieType):
-	def __init__(self, uda:syntax.UserAgent, args:ProductType, frame:TYPE_ENV):
+class _AgentDerived(ComputedType):
+	args:tuple[SophieType, ...]
+	
+	def __init__(self, uda:syntax.UserAgent, args:ProductType, global_env:TYPE_ENV):
+		assert isinstance(args, ProductType), type(args)
 		self.uda = uda
-		self.args = args
-		# By definition the static link for a template is its own module's global scope.
-		# For a UDAType the proper static link should be an extension with a SELF link.
-		self.frame = frame
+		self.args = args.fields
+		self.global_env = global_env
 		super().__init__(uda, args)
 
 class ParametricTemplateType(_AgentDerived):
 	def visit(self, visitor:"TypeVisitor"): return visitor.on_parametric_template(self)
-	def expected_arity(self) -> int: return len(self.uda.fields)
+	def expected_arity(self) -> int: return len(self.uda.members)
 
 class ConcreteTemplateType(_AgentDerived):
 	def visit(self, visitor:"TypeVisitor"): return visitor.on_concrete_template(self)
 	def expected_arity(self) -> int: return -1  # Not callable; instantiable.
+	def state_pairs(self):
+		return zip(self.uda.members, self.args)
 
-class UDAType(_AgentDerived):
+class UDAType(ComputedType):
+	"""
+	Has much in common with a subroutine type,
+	except that the environment link here is going to contain
+	the state of the actor itself. This is necessary because
+	assignment statements can possibly cause state to promote.
+	""" 
+	def __init__(self, template:ConcreteTemplateType, dynamic_link:TYPE_ENV):
+		self.uda = template.uda
+		frame = Activation(template.global_env, dynamic_link, None)
+		frame.assign(SELF, self)
+		frame.update(template.state_pairs())
+		self.frame = frame
+		super().__init__(template)
+		
 	def visit(self, visitor:"TypeVisitor"): return visitor.on_uda(self)
-	def expected_arity(self) -> int: return -1  # Not callable; instantiable.
-
-class BehaviorType(SophieType):
-	def __init__(self, uda_type:UDAType, behavior:syntax.Behavior):
-		self.uda_type = uda_type
-		self.behavior = behavior
-		super().__init__(uda_type, behavior)
-	def visit(self, visitor:"TypeVisitor"): return visitor.on_behavior(self)
-	def expected_arity(self) -> int: return len(self.behavior.params)
-
+	def expected_arity(self) -> int: return -1  # Not callable
 
-class _Bottom(SophieType):
+class _Bottom(FormalType):
 	"""
 	The completely unrestricted type:
 	It unifies with anything to become that other thing.
 	This does double duty as "I don't know" and "I don't care".
 	"""
 	def visit(self, visitor:"TypeVisitor"): return visitor.on_bottom()
 
-class _Error(SophieType):
+class _Error(FormalType):
 	""" The type of things that make no sense or otherwise do not compute. """
 	def visit(self, visitor:"TypeVisitor"): return visitor.on_error_type()
 
 BOTTOM = _Bottom(None)
 ERROR = _Error(None)
 EMPTY_PRODUCT = ProductType(())
+READY_MESSAGE = MessageType(EMPTY_PRODUCT).exemplar()
 
 ###################
 #
 
 class TypeVisitor:
 	def on_variable(self, v:TypeVariable): raise NotImplementedError(type(self))
 	def on_opaque(self, o: OpaqueType): raise NotImplementedError(type(self))
 	def on_record(self, r:RecordType): raise NotImplementedError(type(self))
 	def on_sum(self, s:SumType): raise NotImplementedError(type(self))
 	def on_tag_enum(self, e: EnumType): raise NotImplementedError(type(self))
 	def on_tag_record(self, t: TaggedRecord): raise NotImplementedError(type(self))
 	def on_arrow(self, a:ArrowType): raise NotImplementedError(type(self))
 	def on_product(self, p:ProductType): raise NotImplementedError(type(self))
-	def on_udf(self, f:UDFType): raise NotImplementedError(type(self))
+	def on_subroutine(self, sub:SubroutineType): raise NotImplementedError(type(self))
 	def on_ad_hoc(self, f:AdHocType): raise NotImplementedError(type(self))
 	def on_interface(self, it:InterfaceType): raise NotImplementedError(type(self))
 	def on_parametric_template(self, t:ParametricTemplateType): raise NotImplementedError(type(self))
 	def on_concrete_template(self, t:ConcreteTemplateType): raise NotImplementedError(type(self))
 	def on_uda(self, a:UDAType): raise NotImplementedError(type(self))
 	def on_message(self, m:MessageType): raise NotImplementedError(type(self))
 	def on_user_task(self, t:UserTaskType): raise NotImplementedError(type(self))
-	def on_behavior(self, t:BehaviorType): raise NotImplementedError(type(self))
 	def on_bottom(self): raise NotImplementedError(type(self))
 	def on_error_type(self): raise NotImplementedError(type(self))
 
 
 class Render(TypeVisitor):
 	""" Return a string representation of the term. """
 	def __init__(self):
@@ -302,33 +326,40 @@
 	def on_tag_enum(self, e: EnumType):
 		return e.st.nom.text
 	def on_tag_record(self, t: TaggedRecord):
 		return t.st.nom.text+self._generic(t.type_args)
 	def on_arrow(self, a: ArrowType):
 		return a.arg.visit(self)+"->"+a.res.visit(self)
 	def on_product(self, p: ProductType):
-		return "(%s)"%(",".join(t.visit(self) for t in p.fields))
-	def on_udf(self, f: UDFType):
-		return "<%s/%d>"%(f.fn.nom.text, f.expected_arity())
+		return self._args(p.fields)
+	def _args(self, args:Iterable[SophieType]):
+		return "(%s)"%(",".join(a.visit(self) for a in args))
+	def on_subroutine(self, sub: SubroutineType):
+		try:
+			layer = sub.static_link.chase(SELF)
+		except KeyError:
+			return "<%s/%d>"%(sub.sub.nom.text, sub.expected_arity())
+		else:
+			uda_type = layer.fetch(SELF)
+			return "<%s:%s/%d>" % (uda_type.uda.nom.text, sub.sub.nom.text, sub.expected_arity())
+			
 	def on_ad_hoc(self, f: AdHocType):
 		return "<%s/%d>"%(f.glyph, f.expected_arity())
 	def on_interface(self, it:InterfaceType):
 		return "<interface:%s>"%it.symbol.nom.text
 	def on_parametric_template(self, t: ParametricTemplateType):
 		return "<template:%s/%d>"%(t.uda.nom.text, t.expected_arity())
 	def on_concrete_template(self, t: ConcreteTemplateType):
-		return "<template:%s%s>"%(t.uda.nom.text, t.args.visit(self))
+		return "<template:%s%s>"%(t.uda.nom.text, self._args(t.args))
 	def on_uda(self, a: UDAType):
-		return "<agent:%s%s>"%(a.uda.nom.text, a.args.visit(self))
+		return "<agent:%s%s>"%(a.uda.nom.text, self._args(a.args))
 	def on_message(self, m: MessageType):
 		return "<message:%s>"%m.arg.visit(self)
 	def on_user_task(self, t: UserTaskType):
-		return "<task:%s>"%t.udf_type.visit(self)
-	def on_behavior(self, t: BehaviorType):
-		return "<%s:%s/%d>"%(t.uda_type.uda.nom.text, t.behavior.nom.text, t.expected_arity())
+		return "<task:%s>"%t.proc_type.visit(self)
 	def on_bottom(self):
 		return "?"
 	def on_error_type(self):
 		return "-/error/-"
 	
 def _name_variable(n):
 	name = ""
```

### Comparing `sophie-lang-0.0.6/sophie/cmdline.py` & `sophie-lang-0.0.7/sophie/cmdline.py`

 * *Files identical despite different names*

### Comparing `sophie-lang-0.0.6/sophie/demand.py` & `sophie-lang-0.0.7/sophie/demand.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+"""
+Just to be absolutely clear, this module does not have to be perfect.
+It has to be fit for its purpose, which is to find the clearly-demanded.
+This is allowed to underestimate. It's just not allowed to overestimate,
+as that could potentially change the run-time semantics away from what
+pure call-by-need (i.e. thunk-everything) would have done.
+"""
+
 from typing import Optional
 from boozetools.support.foundation import Visitor, strongly_connected_components_hashable
 from . import syntax
 from .resolution import RoadMap, TopDown
 
 
 def analyze_demand(roadmap:RoadMap):
@@ -22,34 +30,36 @@
 		self.analyze_module(roadmap.preamble)
 		for module in roadmap.each_module:
 			self.analyze_module(module)
 		
 		del self.graph[None]
 	
 	def analyze_module(self, module:syntax.Module):
-		for udf in module.all_functions:
-			self.graph[udf] = set()
-		self.tour(module.outer_functions)
+		for udf in module.all_fns:
+			if isinstance(udf, syntax.UserFunction):
+				self.graph[udf] = set()
+		self.tour(module.top_subs)
 		self.tour(module.agent_definitions)
 		for expr in module.main:
 			self.visit(expr, None)
 	
 	def tour(self, items):
 		for i in items:
 			self.visit(i)
 	
-	def visit_UserFunction(self, udf:syntax.UserFunction):
-		self.tour(udf.where)
-		self.visit(udf.expr, udf)
-	
-	def visit_UserAgent(self, uda:syntax.UserAgent):
-		self.tour(uda.behaviors)
-	
-	def visit_Behavior(self, b:syntax.Behavior):
-		self.visit(b.expr, None)
+	def visit_UserFunction(self, func:syntax.UserFunction):
+		self.tour(func.where)
+		self.visit(func.expr, func)
+	
+	def visit_UserAgent(self, actor:syntax.UserAgent):
+		self.tour(actor.behaviors)
+	
+	def visit_UserProcedure(self, proc:syntax.UserProcedure):
+		self.tour(proc.where)
+		self.visit(proc.expr, None)
 	
 	def visit_Call(self, call: syntax.Call, src):
 		if isinstance(call.fn_exp, syntax.Lookup):
 			target = call.fn_exp.ref.dfn
 			if isinstance(target, syntax.UserFunction):
 				self.graph[src].add(target)
 		elif isinstance(call.fn_exp, syntax.LambdaForm):
@@ -82,16 +92,16 @@
 	
 	def visit_DoBlock(self, do:syntax.DoBlock, src):
 		for agent in do.agents:
 			self.visit(agent.expr, src)
 		for step in do.steps:
 			self.visit(step, src)
 	
-	def visit_AssignField(self, af:syntax.AssignField, src):
-		self.visit(af.expr, src)
+	def visit_AssignMember(self, am:syntax.AssignMember, src):
+		self.visit(am.expr, src)
 
 EMPTY = set()
 
 def _possible(expr):
 	return not isinstance(expr, syntax.Absurdity)
 
 class DemandPass(Visitor):
@@ -187,15 +197,15 @@
 	def visit_BindMethod(self, expr:syntax.BindMethod):
 		return self.visit(expr.receiver)
 
 	def visit_FieldReference(self, fr:syntax.FieldReference):
 		return self.visit(fr.lhs)
 	
 	def visit_AsTask(self, task:syntax.AsTask):
-		return self.visit(task.sub)
+		return self.visit(task.proc_ref)
 
 	@staticmethod
 	def visit_Literal(_):
 		return EMPTY
 
 	@staticmethod
 	def visit_LambdaForm(_):
@@ -210,9 +220,9 @@
 		return EMPTY
 
 	@staticmethod
 	def visit_Absurdity(_):
 		assert False, "Absurd cases ought not influence demand analysis."
 	
 	@staticmethod
-	def visit_AssignField(_):
+	def visit_AssignMember(_):
 		assert False, "Only behaviors can assign fields, but only functions are subject to this analysis."
```

### Comparing `sophie-lang-0.0.6/sophie/diagnostics.py` & `sophie-lang-0.0.7/sophie/diagnostics.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys, random
 from typing import Sequence, Optional, Union, Any
-from traceback import TracebackException
+from traceback import TracebackException, format_stack
 from pathlib import Path
 from boozetools.support.failureprone import SourceText, Issue, Evidence, Severity, illustration
 from . import syntax
 from .ontology import Expr, Nom, Symbol, Reference, Term
 from .calculus import TYPE_ENV, SophieType
 from .stacking import Frame
 
@@ -86,19 +86,19 @@
 		evidence = {self._path: [Evidence(s, "") for s in guilty]}
 		self.issue(Issue(phase, Severity.ERROR, msg, evidence))
 
 	def complain_to_console(self):
 		""" Emit all the issues to the console. """
 		_bemoan(self._issues)
 			
-	def assert_no_issues(self):
+	def assert_no_issues(self, message):
 		""" Does what it says on the tin """
 		if self._issues:
 			self.complain_to_console()
-			assert False, "This is supposed to be impossible."
+			assert False, "This is supposed to be impossible. "+message
 	
 	# Methods the front-end is likely to call:
 	def generic_parse_error(self, path: Path, lookahead, node:Nom, hint: str):
 		intro = "Sophie got confused by %s." % lookahead
 		problem = [Annotation(path, node, "Sophie got confused here")]
 		self.issue(Pic(intro, problem))
 		self.issue(Pic(hint, []))
@@ -170,21 +170,26 @@
 		self._undefined.note(guilty)
 
 	def opaque_generic(self, guilty:Sequence[syntax.TypeParameter]):
 		admonition = "Opaque types are not to be made generic."
 		where = [g.head() for g in guilty]
 		self.error("Defining Types", where, admonition)
 	
-	def can_only_assign_within_behavior(self, af:syntax.AssignField):
-		intro = "You can only assign to state within an actor's behaviors."
-		self.issue(Pic(intro, [Annotation(self._path, af)]))
+	def can_only_see_member_within_behavior(self, nom:Nom):
+		intro = "You can only refer to an actor's state within that actor's own behaviors."
+		self.issue(Pic(intro, [Annotation(self._path, nom)]))
+	
+	def use_my_instead(self, env: TYPE_ENV, fr: syntax.FieldReference):
+		intro = "To read an actor's own private state, use `my %s` here." % fr.field_name.text
+		problem = [Annotation(env.path(), fr)]
+		self.issue(Pic(intro, problem))
 	
 	# Methods the Alias-checker calls
 	def these_are_not_types(self, non_types:Sequence[syntax.TypeCall]):
-		intro = "Words that get used like types, but refer to something else (e.g. variants or functions)."
+		intro = "Words that get used like types, but refer to something else (e.g. variants, functions, or agent definitions)."
 		problem = [Annotation(self._path, tc) for tc in non_types]
 		self.issue(Pic(intro, problem))
 	
 	def circular_type(self, scc:Sequence):
 		intro = "What we have here is a circular type-definition."
 		problem = [Annotation(self._path, node) for node in scc]
 		self.issue(Pic(intro, problem))
@@ -244,55 +249,68 @@
 		problem = [
 			Annotation(path, x1, str(t1)),
 			Annotation(path, x2, str(t2)),
 		]
 		self.issue(Pic(intro, problem))
 		self.issue(Pic("Here's how that happens:", trace_stack(env)))
 	
-	def wrong_arity(self, env:TYPE_ENV, site:syntax.ValExpr, arity:int, args:Sequence[syntax.ValExpr]):
-		if site not  in self._already_complained_about:
+	def wrong_arity(self, env:TYPE_ENV, site:syntax.ValExpr, callee_type:SophieType, args:Sequence[syntax.ValExpr]):
+		arity = callee_type.expected_arity()
+		if site not in self._already_complained_about:
 			self._already_complained_about.add(site)
 			if arity < 0:
-				intro = "This is not callable."
+				intro = "This %s is not callable."%callee_type
 			else:
 				plural = '' if arity == 1 else 's'
-				pattern = "This function takes %d argument%s, but got %d instead."
-				intro = pattern % (arity, plural, len(args))
-			problem = [Annotation(env.path(), site, "Here")]
-			self.issue(Pic(intro, problem))  # +trace_stack(env)
-
+				pattern = "This %s takes %d argument%s, but got %d instead."
+				intro = pattern % (callee_type, arity, plural, len(args))
+			problem = [Annotation(env.path(), site, intro)]
+			self.issue(Pic(intro, trace_stack(env) + problem))
+	
 	def bad_argument(self, env: TYPE_ENV, term:Term, param:syntax.FormalParameter, actual:SophieType, why:str):
 		assert isinstance(term, Term)
 		assert isinstance(param, syntax.FormalParameter)
 		assert isinstance(why, str)
 		intro = "Type-checking found a square peg in a round hole:"
 		caption = str(actual) + " does not apply because " + why
 		problem = [Annotation(term.source_path, param, caption)]
 		self.issue(Pic(intro, trace_stack(env)+problem))
 	
 	def bad_result(self, env: TYPE_ENV, fn:syntax.UserFunction, result_type, why):
-		intro = "Type-checking found a problem. Here's how it happens:"
+		intro = "Type-checking found a problematic result:"
 		produced = Annotation(fn.source_path, fn.expr, "Produced "+str(result_type))
 		caption = "Did not match because " + why
 		needed = Annotation(fn.source_path, fn.result_type_expr, caption)
 		self.issue(Pic(intro, trace_stack(env)+[produced, needed]))
 
 	def bad_type(self, env: TYPE_ENV, expr: syntax.ValExpr, need, got, why):
 		intro = "Type-checking found a problem. Here's how it happens:"
 		complaint = "This %s needs to be a(n) %s."%(got, need)
 		problem = [Annotation(env.path(), expr, complaint)]
 		self.issue(Pic(intro, trace_stack(env)+problem, (why,)))
 	
-	def does_not_express_behavior(self, env: TYPE_ENV, behavior:syntax.Behavior, got):
-		intro = "This definition express %s instead of behavior"%got
-		problem = [Annotation(env.path(), behavior)]
+	def bad_task(self, env: TYPE_ENV, expr: syntax.ValExpr, got):
+		intro = "I don't know how to convert %s into a task." % got
+		footer = "Typically you'll want a procedure here."
+		problem = [Annotation(env.path(), expr)]
+		self.issue(Pic(intro, trace_stack(env)+problem, (footer,)))
+
+	
+	def does_not_express_behavior(self, env: TYPE_ENV, procedure:syntax.UserProcedure, got):
+		intro = "This definition expresses %s instead of behavior"%got
+		problem = [Annotation(env.path(), procedure)]
 		self.issue(Pic(intro, trace_stack(env)+problem))
 
-	def bad_message(self, env:TYPE_ENV, expr:syntax.BindMethod, agent_type:SophieType):
-		intro = "This %s does not understand..."%agent_type
+	def must_not_express_behavior(self, env: TYPE_ENV, fn:syntax.UserFunction):
+		intro = "Procedural steps cannot happen within a pure function."
+		problem = [Annotation(env.path(), fn)]
+		self.issue(Pic(intro, trace_stack(env)+problem))
+
+	def bad_message(self, env:TYPE_ENV, expr:syntax.BindMethod, actor_type:SophieType):
+		intro = "This %s does not understand..." % actor_type
 		problem = [Annotation(env.path(), expr.method_name, "this message")]
 		self.issue(Pic(intro, trace_stack(env)+problem))
 	
 	def type_has_no_fields(self, env:TYPE_ENV, fr:syntax.FieldReference, lhs_type):
 		field = fr.field_name.text
 		intro = "Type-checking found an unsuitable source for field '%s' access."%field
 		complaint = "%s has no fields; in particular not '%s'."%(lhs_type, field)
@@ -307,17 +325,17 @@
 	def record_lacks_field(self, env:TYPE_ENV, fr:syntax.FieldReference, lhs_type:SophieType):
 		field = fr.field_name.text
 		intro = "Type-checking found an unsuitable source for field '%s' access."%field
 		complaint = "Type '%s' has fields, but not one called '%s'."%(lhs_type, field)
 		problem = [Annotation(env.path(), fr, complaint)]
 		self.issue(Pic(intro, trace_stack(env)+problem))
 	
-	def ill_founded_function(self, env:TYPE_ENV, udf:syntax.UserFunction):
-		intro = "This function's definition turned up circular, as in a=a."
-		problem = [Annotation(udf.source_path, udf, "This one.")]
+	def ill_founded_function(self, env:TYPE_ENV, sub:syntax.Subroutine):
+		intro = "This definition turned up circular, as in a=a."
+		problem = [Annotation(sub.source_path, sub, "This one.")]
 		self.issue(Pic(intro, trace_stack(env)+problem))
 
 	def no_applicable_method(self, env:TYPE_ENV, actual_types):
 		intro = "A type-directed operation goes off the rails. Here's how:"
 		footer = [
 			"This operator has no method for "+str(tuple(actual_types))+".",
 			"If these are the types you mean to operate on,",
@@ -328,55 +346,60 @@
 	def bogus_operator_arity(self, udf):
 		intro = "Define most operators for two arguments. Negation (-) can also be defined for only one."
 		problem = [Annotation(udf.source_path, udf, "This one.")]
 		self.issue(Pic(intro, problem))
 
 	# Some things for just in case:
 	
-	def drat(self, env:TYPE_ENV, expr:Expr, exception):
-		intro = _outburst()
-		problem = [Annotation(env.path(), expr, str(exception))]
-		self.issue(Pic(intro, trace_stack(env)+problem))
-		self.complain_to_console()
-		raise exception
+	def drat(self, env:TYPE_ENV, hint):
+		intro = "This code hits an unfinished part of the type-checker."
+		python_frames = map(str.rstrip, format_stack(limit=8)[:-1])
+		footer = [
+			"",
+			"Hint: "+str(hint),
+			"",
+			"Recent Python frames:",
+			*python_frames,
+		]
+		self.issue(Pic(intro, trace_stack(env), footer))
+		# self.complain_to_console()
 
 class Annotation:
 	path: Path
 	slice: slice
 	caption: str
 	def __init__(self, path:Path, node, caption:str=""):
 		self.path = path
 		self.slice = node.head()
 		self.caption = caption
-		assert isinstance(self.slice, slice), type(node)
+		assert isinstance(self.slice, slice), (type(node), "head method fails to return a slice.")
 
 def illustrate(source, span:slice, caption):
 	row, col = source.find_row_col(span.start)
 	single_line = source.line_of_text(row)
 	width = span.stop - span.start
 	return illustration(single_line, col, width, prefix='% 6d |' % row, caption=caption)
 
 class Tracer:
 	def __init__(self):
 		self.trace = []
-	def called_with(self, path, breadcrumb, args:dict):
-		bind_text = ', '.join("%s:%s" % (p.nom.text, t) for p, t in args.items())
-		self.trace.append(Annotation(path, breadcrumb, "with " + bind_text))
 	def called_from(self, path, pc):
-		self.trace.append(Annotation(path, pc, "calls:"))
+		self.trace.append(Annotation(path, pc))
 	def hit_bottom(self):
 		pass
-	def trace_frame(self, breadcrumb, bindings, pc):
-		path = breadcrumb.source_path
+	def trace_frame(self, path, breadcrumb, bindings):
 		args = {
 			k:v for k,v in bindings.items()
-			if isinstance(k, syntax.FormalParameter)
+			if isinstance(k, (syntax.FormalParameter, syntax.Subject))
 		}
-		if args: self.called_with(path, breadcrumb, args)
-		if pc is not None: self.called_from(path, pc)
+		if args:
+			bind_text = ', '.join("%s:%s" % (p.nom.text, t) for p, t in args.items())
+			self.trace.append(Annotation(path, breadcrumb, bind_text))
+
+		
 
 def trace_stack(env:Frame) -> list[Annotation]:
 	tracer = Tracer()
 	env.trace(tracer)
 	return tracer.trace
 
 class Pic:
```

### Comparing `sophie-lang-0.0.6/sophie/executive.py` & `sophie-lang-0.0.7/sophie/executive.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,58 +4,61 @@
 """
 import sys
 from collections import deque
 from . import syntax, primitive,  ontology
 from .stacking import Frame, RootFrame, Activation
 from .runtime import (
 	force, _strict, Constructor, Primitive, Thunk,
-	Action, ActorClass, ActorTemplate, iterate_list,
+	ActorClass, ActorTemplate, is_sophie_list, iterate_list,
 	reset, install_overrides
 )
 from .resolution import RoadMap
 from .scheduler import MAIN_QUEUE, SimpleTask
 
-def run_program(roadmap:RoadMap):
+DRIVERS = {}
 
-	drivers = {}
+def run_program(roadmap:RoadMap):
+	DRIVERS.clear()
 	_set_strictures(roadmap.preamble)
 	preamble_scope = roadmap.module_scopes[roadmap.preamble]
 	root = _dynamic_root(preamble_scope)
-	result = None
 	for module in roadmap.each_module:
 		_set_strictures(module)
 		env = Activation.for_module(root, module)
 		_prepare(env, roadmap.module_scopes[module])
 		for d in module.foreign:
 			if d.linkage is not None:
 				py_module = sys.modules[d.source.value]
 				linkage = [env.fetch(ref.dfn) for ref in d.linkage]
-				drivers.update(py_module.sophie_init(*linkage) or ())
+				DRIVERS.update(py_module.sophie_init(*linkage) or ())
 		install_overrides(env, module.user_operators)
 		for expr in module.main:
 			env.pc = expr
-			result = _strict(expr, env)
-			if isinstance(result, Action):
-				MAIN_QUEUE.execute(SimpleTask(result.perform))
-				continue
-			if isinstance(result, dict):
-				tag = result.get("")
-				if tag in drivers:
-					drivers[tag](env, result)
-					continue
-				dethunk(result)
-				if tag == 'cons':
-					result = list(iterate_list(result))
-			if result is not None:
-				print(result)
+			MAIN_QUEUE.execute(SimpleTask(_display, expr, env))
 		root.absorb(env)
-	return result
+
+def _display(expr, env):
+	result = _strict(expr, env)
+	if hasattr(result, "perform"):
+		result.perform(env)
+		return
+	if is_sophie_list(result):
+		result = list(iterate_list(result))
+	elif isinstance(result, dict):
+		tag = result.get("")
+		if tag in DRIVERS:
+			DRIVERS[tag](env, result)
+			return
+		dethunk(result)
+	if result is not None:
+		print(result)
+
 
 def _set_strictures(module):
-	for udf in module.all_functions:
+	for udf in module.all_fns + module.all_procs:
 		udf.strictures = tuple(i for i, p in enumerate(udf.params) if p.is_strict)
 
 def _dynamic_root(preamble_scope) -> RootFrame:
 	root = RootFrame()
 	_prepare(root, primitive.root_namespace)
 	_prepare(root, preamble_scope)
 	reset(lambda s:root.fetch(preamble_scope[s]))
@@ -72,18 +75,18 @@
 				env.assign(dfn, Constructor(dfn, dfn.body.field_names()))
 			elif dfn.body is None:
 				env.assign(dfn, {"": dfn})
 			else:
 				raise ValueError("Tagged scalars (%r) are not implemented."%key)
 		elif isinstance(dfn, syntax.FFI_Alias):
 			env.assign(dfn, _native_object(dfn))
-		elif isinstance(dfn, syntax.UserFunction):
+		elif isinstance(dfn, syntax.Subroutine):
 			env.declare(dfn)
 		elif isinstance(dfn, syntax.UserAgent):
-			env.assign(dfn, ActorClass(env, dfn) if dfn.fields else ActorTemplate(env, dfn, ()))
+			env.assign(dfn, ActorClass(env, dfn) if dfn.members else ActorTemplate(env, dfn, ()))
 		elif type(dfn) in _ignore_these:
 			pass
 		else:
 			raise ValueError("Don't know how to deal with %r %r"%(type(dfn), key))
 
 def _native_object(dfn:syntax.FFI_Alias):
 	if callable(dfn.val):
```

### Comparing `sophie-lang-0.0.6/sophie/front_end.py` & `sophie-lang-0.0.7/sophie/front_end.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,13 +173,13 @@
 	You cannot lose what you do not possess.
 	But this is a computer program.
 """)
 _hint("name formals : name ● ???", "It seems to cut off after perhaps a type-annotation?")
 _hint("name type_parameters IS ( name : name ● ???", "Anticipated a comma or perhaps open-square-bracket here.")
 _hint("WHEN expr ● ->", "WHEN goes with THEN. The arrow is for type matches.")
 _hint("TYPE : ??? round_list(simple_type) ● ;", "Might be a record missing field types, or the first part of a function-type (expecting '->' and a result-type ).")
-_hint("AGENT ??? semicolon_list(behavior) END ● ;", "End agents by name: AGENT foo ... END foo;")
-_hint("name formals annotation = expr WHERE semicolon_list(function) END ● ;", "End enclosing functions by name: foo(x) = ... WHERE ... END foo;")
+_hint("AGENT ??? semicolon_list(procedure) END ● ;", "End agents by name: AGENT foo ... END foo;")
+_hint("name formals annotation = expr WHERE semicolon_list(subroutine) END ● ;", "End enclosing functions by name: foo(x) = ... WHERE ... END foo;")
 _hint("TYPE : ??? ! ● name", "you have !foo and probably want !(foo) to represent a message/procedure of one argument.")
 
 assert _best_hint("export_section import_section TYPE : name square_list(name) IS".split(), 'OPAQUE')
```

### Comparing `sophie-lang-0.0.6/sophie/intermediate.py` & `sophie-lang-0.0.7/sophie/intermediate.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 implement lazy evaluation.
 
 You can invoke this code on a Sophie program using the -x command-line flag to the main
 Sophie interpreter. That still subjects your program to all normal syntax and type checks,
 but if that passes, then you get corresponding VM intermediate code on standard output.
 """
 
-from typing import Iterable, Optional, Sequence
+from typing import Iterable, Optional
 from boozetools.support.foundation import Visitor
 from . import syntax, ontology, primitive
 from .resolution import RoadMap
 
 class TooComplicated(Exception):
 	pass
 
@@ -109,22 +109,24 @@
 	def declare(self, symbol: ontology.Symbol):
 		raise NotImplementedError(type(self))
 	
 	def declare_several(self, symbols: Iterable[ontology.Symbol]):
 		for sym in symbols:
 			self.declare(sym)
 
-	def write_one_function(self, fn: syntax.UserFunction):
-		inner = VMFunctionScope(self, fn.nom.text, is_thunk=not fn.params)
-		inner.emit_preamble(fn.params, MANGLED[fn])
+	def write_one_subroutine(self, fn: syntax.Subroutine):
+		inner = VMFunctionScope(self, fn.nom.text, is_thunk=fn.is_thunk())
+		emit(len(fn.params), quote(MANGLED[fn]))
 		for param in fn.params:
+			inner.declare(param)
 			if param.is_strict:
 				inner.make_strict(param)
 		inner.write_inner_functions(fn.where)
-		TAIL.visit(fn.expr, inner)
+		context = LAST if isinstance(fn, syntax.UserProcedure) else TAIL
+		context.visit(fn.expr, inner)
 		inner.emit_epilogue()
 
 class VMGlobalScope(VMScope):
 	""" Mainly a null-object that encloses a nest of scopes without itself being enclosed. """
 	
 	def capture(self, symbol: ontology.Symbol) -> bool:
 		return False
@@ -132,69 +134,79 @@
 	def emit_captured(self, captives: list[ontology.Symbol]):
 		for sym in captives:
 			assert sym is None
 			emit("*")
 
 	def write_begin_expressions(self, module: syntax.Module):
 		inner = VMFunctionScope(self, "[BEGIN]", is_thunk=True)
-		for index, expr in enumerate(module.main):
+		for expr, performative in zip(module.main, module.performative):
 			inner.nl()
-			FORCE.visit(expr, inner)
-			inner.display()
+			if performative:
+				STEP.visit(expr, inner)
+				inner.emit_drain()
+			else:
+				FORCE.visit(expr, inner)
+				inner.emit_display()
 	
-	def write_outer_functions(self, fns:list[syntax.UserFunction]):
+	def write_outer_functions(self, fns:list[syntax.Subroutine]):
 		self.mangle_names(fns)
 		for fn in fns:
 			self.nl()
 			if isinstance(fn, syntax.UserOperator):
 				emit(OPERATOR_DIRECTIVE[fn.nom.key(), len(fn.params)])
 				for token in fn.dispatch_vector():
 					emit(quote(MANGLED[token]))
 			else:
 				emit(".fn")
-			self.write_one_function(fn)
+			self.write_one_subroutine(fn)
 	
 	def declare(self, symbol: ontology.Symbol):
 		pass
 	
 	def write_actors(self, agent_definitions:list[syntax.UserAgent]):
 		for dfn in agent_definitions:
 			last = dfn.behaviors[-1]
 			inner = VMActorScope(self, dfn)
 			for b in dfn.behaviors:
+				inner.nl()
 				inner.write_one_behavior(b)
 				emit(".end" if b is last else ";")
 			self.nl()
 		pass
 
 class VMActorScope(VMScope):
 	""" Specialized scope for the behaviors of an actor-definition """
 	def __init__(self, outer:VMScope, dfn:syntax.UserAgent):
 		super().__init__(outer._prefix + dfn.nom.text + ":")
 		self._outer = outer
 		self.indent = outer.indent+"  "
-		emit(".actor", *dfn.field_names(), quote(MANGLED[dfn]))
-		self._field_map = {field:i for i,field in enumerate(dfn.field_names())}
+		emit(".actor", *dfn.member_names(), quote(MANGLED[dfn]))
+		self._field_map = {field:i for i,field in enumerate(dfn.member_names())}
 
 	def capture(self, symbol: ontology.Symbol) -> bool:
 		return False
 
 	def emit_captured(self, captives: list[ontology.Symbol]):
 		assert not captives
 	
 	def member_number(self, field: str):
 		return self._field_map[field]
 
-	def write_one_behavior(self, b:syntax.Behavior):
+	def write_one_behavior(self, behavior:syntax.UserProcedure):
 		# The way this works is similar to a function.
 		# However, there's a special "self" object implicitly the first parameter.
 		# Also, access to self-dot-foo will use actor-specific instructions.
-		inner = VMFunctionScope(self, b.nom.text, is_thunk=False)
-		inner.emit_preamble([ontology.SELF] + b.params, b.nom.text)
-		LAST.visit(b.expr, inner)
+		inner = VMFunctionScope(self, behavior.nom.text, is_thunk=False)
+		emit(1 + len(behavior.params), quote(behavior.nom.text))
+		inner.declare(ontology.SELF)
+		inner.declare_several(behavior.params)
+		for member in behavior.reads_members:
+			inner.emit_reads_member(member)
+		inner.write_inner_functions(behavior.where)
+		LAST.visit(behavior.expr, inner)
 		inner.emit_epilogue()
 
 class VMFunctionScope(VMScope):
 	""" Encapsulates VM mechanics around the stack, parameters, closure capture, jumps, etc. """
 	
 	_captives : dict[Optional[ontology.Symbol], int]
 	
@@ -244,14 +256,15 @@
 		if symbol in self._local:
 			frame_offset = self._local[symbol]
 			assert frame_offset < self._depth
 			emit("LOCAL", frame_offset)
 		elif self.capture(symbol):
 			emit("CAPTIVE", self._captives[symbol])
 		else:
+			assert symbol in MANGLED, ("heck", symbol, self._prefix)
 			emit("GLOBAL", quote(MANGLED[symbol]))
 		self._push()
 
 	def constant(self, value):
 		if isinstance(value, bool):
 			self.emit_ALU(value)
 		else:
@@ -301,19 +314,14 @@
 		assert source is self, "Improper Come-From"
 		if self._depth is None:
 			self._depth = depth
 		else:
 			assert self._depth == depth, "Inconsistent Come-From %d != %d"%(self._depth, depth)
 		LABEL_QUEUE.append(label)
 
-	def emit_preamble(self, params:Sequence[syntax.FormalParameter], name:str):
-		emit(len(params))
-		emit(quote(name))
-		self.declare_several(params)
-
 	def make_strict(self, param):
 		emit("STRICT", self._local[param])
 	
 	def emit_epilogue(self):
 		# Consists of right brace, maximum number of locally-used stack slots,
 		# number of captures, and information about each capture.
 		if len(self._captives) > 255: raise TooComplicated("More than 255 captures in one function")
@@ -326,23 +334,30 @@
 			if sym in self._local:
 				emit("L", self._local[sym])
 			elif sym is None:
 				emit("*")
 			else:
 				emit(self._captives[sym])
 	
-	def display(self):
+	def emit_drain(self):
+		assert self._depth == 0, self.depth()
+		emit("DRAIN")
+	
+	def emit_display(self):
 		assert self._depth == 1, self.depth()
-		emit("DISPLAY")
 		self._pop()
+		emit("DISPLAY")
 	
 	def ascend_to(self, depth:int):
 		assert self._depth >= depth
-		if self._depth > depth:
-			emit("ASCEND", self._depth - depth)
+		nr_levels = self._depth - depth
+		if nr_levels == 1:
+			self._pop()
+		elif nr_levels > 1:
+			emit("ASCEND", nr_levels)
 			self._depth = depth
 	
 	def emit_call(self, arity):
 		emit("CALL")
 		self._depth -= arity
 	
 	def emit_pop(self):
@@ -363,29 +378,27 @@
 		self._pop()
 
 	def emit_skip(self):
 		emit("SKIP")
 		self._push()
 
 	def emit_return(self):
+		assert self._depth
 		emit("RETURN")
 		self._depth = None
 
 	def emit_force_return(self):
+		assert self._depth
 		emit("FORCE_RETURN")
 		self._depth = None
 
 	def emit_exec(self):
 		emit("EXEC")
 		self._depth = None
 
-	def emit_perform_exec(self):
-		emit("PERFORM_EXEC")
-		self._depth = None
-
 	def emit_nil(self):
 		emit("NIL")
 		self._push()
 	
 	def emit_snoc(self):
 		emit("SNOC")
 		self._pop()
@@ -413,29 +426,31 @@
 		emit("]")
 		self._push()
 	
 	def emit_assign_member(self, field: str):
 		emit("ASSIGN", self.member_number(field))
 		self._depth -= 2
 
-	def emit_read_member(self, field: str):
-		emit("MEMBER", self.member_number(field))
+	def emit_reads_member(self, member:syntax.FormalParameter):
+		assert isinstance(member, syntax.FormalParameter), type(member)
+		emit("MEMBER", self.member_number(member.nom.key()))
+		self.declare(member)
 		
 	def member_number(self, field: str):
 		return self._outer.member_number(field)
 
 	def write_inner_functions(self, fns):
 		if not fns: return
 		self.mangle_names(fns)
 		self.declare_several(fns)
 		emit("{")
 		self.nl()
 		last = fns[-1]
 		for fn in fns:
-			self.write_one_function(fn)
+			self.write_one_subroutine(fn)
 			emit("}" if fn is last else ";")
 			self.nl()
 
 _do_count = 0
 def _gensym():
 	global _do_count
 	_do_count += 1
@@ -496,20 +511,19 @@
 	@staticmethod
 	def visit_Absurdity(_: syntax.Absurdity, scope: VMFunctionScope):
 		scope.emit_panic()
 
 class LazyContext(Context):
 	@staticmethod
 	def visit_FieldReference(fr: syntax.FieldReference, scope: VMFunctionScope):
-		if fr.is_volatile or is_eager(fr.lhs): FORCE.visit(fr, scope)
+		if is_eager(fr.lhs): FORCE.visit(fr, scope)
 		else: scope.make_thunk(fr)
 	
 	@staticmethod
 	def _thunk_it(expr:syntax.ValExpr, scope: VMFunctionScope):
-		if expr.is_volatile: FORCE.visit(expr, scope)
 		scope.make_thunk(expr)
 	
 	visit_Call = _thunk_it
 	visit_BinExp = _thunk_it
 	visit_UnaryExp = _thunk_it
 	visit_ShortCutExp = _thunk_it
 	visit_Cond = _thunk_it
@@ -527,38 +541,34 @@
 	def _force_it(expr:syntax.ValExpr, scope: VMFunctionScope):
 		FORCE.visit(expr, scope)
 	
 	visit_Literal = _force_it
 	visit_LambdaForm = _force_it
 	visit_ExplicitList = _force_it
 
-def _delay(expr:syntax.ValExpr, scope: VMFunctionScope):
-	strict = expr.is_volatile  # There could be more reasons later, e.g. stricture analysis
-	(FORCE if strict else DELAY).visit(expr, scope)
-
 def _prepare_arguments_for_call(call: syntax.Call, scope: VMFunctionScope):
 	# If the thing we're calling is syntactically:
 	#     a function by name, then find and respect its strictness declarations.
 	#     a bound method, then evaluate all arguments eagerly.
 	#     anything else, then delay everything and rely on the calling convention.
 	# There's probably a way to break this out into a pass of its own, but meh.
 	
 	if isinstance(call.fn_exp, syntax.Lookup):
 		sym = call.fn_exp.ref.dfn
 		if isinstance(sym, syntax.UserFunction):
 			for param, arg in zip(sym.params, call.args):
 				if param.is_strict:
 					FORCE.visit(arg, scope)
 				else:
-					_delay(arg, scope)
+					DELAY.visit(arg, scope)
 			return
 	if isinstance(call.fn_exp, syntax.BindMethod):
 		for arg in call.args: FORCE.visit(arg, scope)
 		return
-	for arg in call.args: _delay(arg, scope)
+	for arg in call.args: DELAY.visit(arg, scope)
 
 class EagerContext(Context):
 	"""
 	The best way to compile something can depend on context.
 	Rather than pass a ton of flags around,
 	it's polymorphism to the rescue!
 	
@@ -589,184 +599,170 @@
 					scope.come_from(label)
 			self.visit(mx.otherwise, scope)
 			self.sequel(scope, depth, False)
 		for label in after:
 			scope.come_from(label)
 		pass
 	
-	@staticmethod
-	def sequel(scope:VMFunctionScope, depth:int, more:bool):
+	def sequel(self, scope:VMFunctionScope, depth:int, more:bool):
 		""" Called at the end of a consequence. """
-		raise NotImplementedError()
+		raise NotImplementedError(type(self))
+
+	def visit_BinExp(self, it: syntax.BinExp, scope:VMFunctionScope):
+		FORCE.visit(it.lhs, scope)
+		FORCE.visit(it.rhs, scope)
+		scope.emit_ALU(it.op.text)
+		self.answer(scope)
 
 	def visit_UnaryExp(self, ux:syntax.UnaryExp, scope:VMFunctionScope):
 		FORCE.visit(ux.arg, scope)
 		emit(UNARY_INSTRUCTION[ux.op.text])  # No change to stack depth
 		self.answer(scope)
 
 	def visit_ShortCutExp(self, it: syntax.ShortCutExp, scope: VMFunctionScope):
 		FORCE.visit(it.lhs, scope)
 		satisfied = SHORTCUTS[it.op.text]
 		label = scope.jump_if(satisfied)
 		self.visit(it.rhs, scope)
 		scope.come_from(label)
 		self.answer(scope)
 		
-	@staticmethod
-	def answer(scope: VMFunctionScope):
+	@classmethod
+	def answer(cls, scope: VMFunctionScope):
 		""" Answer is on stack; now what? """
-		raise NotImplementedError()
+		raise NotImplementedError(cls)
 	
 	def visit_Literal(self, expr: syntax.Literal, scope: VMFunctionScope):
 		scope.constant(expr.value)
 		self.answer(scope)
 	
-	@staticmethod
-	def visit_LambdaForm(lf:syntax.LambdaForm, scope: VMFunctionScope):
+	def visit_LambdaForm(self, lf:syntax.LambdaForm, scope: VMFunctionScope):
 		# Two steps:
 		# 1. Emit the function.
 		scope.mangle_names([lf.function])
 		scope.declare(lf.function)
 		emit("{")
-		scope.write_one_function(lf.function)
+		scope.write_one_subroutine(lf.function)
 		emit("}")
-		# 2. Emit the code to load that function onto the stack.
-		scope.load(lf.function)
-		
+		# No need to explicitly load the function;
+		# the assembler does it on account of the close-brace.
+		# do not call scope.load(lf.function)
+		self.answer(scope)
+
 	def visit_FieldReference(self, fr: syntax.FieldReference, scope: VMFunctionScope):
 		FORCE.visit(fr.lhs, scope)
-		if syntax.is_self_reference(fr.lhs):
-			scope.emit_read_member(fr.field_name.key())
-		else:
-			scope.emit_read_field(fr.field_name.key())
-			emit("FORCE")
+		scope.emit_read_field(fr.field_name.key())
+		emit("FORCE")
 		self.answer(scope)
 	
 	def visit_ExplicitList(self, el:syntax.ExplicitList, scope:VMFunctionScope):
 		scope.emit_nil()
 		for item in reversed(el.elts):
-			_delay(item, scope)
+			DELAY.visit(item, scope)
 			scope.emit_snoc()
 		self.answer(scope)
 	
 	def visit_BindMethod(self, expr:syntax.BindMethod, scope:VMFunctionScope):
 		FORCE.visit(expr.receiver, scope)
 		emit("BIND", quote(expr.method_name.key()))
 		self.answer(scope)
-
+	
+	def visit_Lookup(self, expr: syntax.Lookup, scope: VMFunctionScope):
+		sym = expr.ref.dfn
+		scope.load(sym)
+		if symbol_harbors_thunks(sym):
+			emit("FORCE")
+		self.answer(scope)
 
 class FunctionContext(EagerContext):
 
 	def visit_DoBlock(self, do:syntax.DoBlock, outer:VMFunctionScope):
-		inner = outer.enter_gensym()
-		LAST.visit(do, inner)
-		inner.emit_epilogue()
-		emit("}")
-		self.answer(outer)
+		assert False, outer._prefix+": This should be neither possible nore necessary anymore."
 	
 	def visit_AsTask(self, task:syntax.AsTask, scope:VMFunctionScope):
-		FORCE.visit(task.sub, scope)
+		FORCE.visit(task.proc_ref, scope)
 		emit("TASK")
 		self.answer(scope)
 	
 	def visit_Skip(self, _:syntax.Skip, scope:VMFunctionScope):
 		scope.emit_skip()
 		self.answer(scope)
 
 		
 class ForceContext(FunctionContext):
-	@staticmethod
-	def visit_Lookup(expr:syntax.Lookup, scope:VMFunctionScope):
-		sym = expr.ref.dfn
-		scope.load(sym)
-		if symbol_harbors_thunks(sym):
-			emit("FORCE")
-	
 	def call(self, scope: VMFunctionScope, arity:int):
 		scope.emit_call(arity)
 	
-	@staticmethod
-	def sequel(scope:VMFunctionScope, depth:int, more:bool):
+	def sequel(self, scope:VMFunctionScope, depth:int, more:bool):
 		scope.ascend_to(depth)
 		if more:
 			return scope.jump_always()
 	
-	@staticmethod
-	def visit_BinExp(it: syntax.BinExp, scope:VMFunctionScope):
-		FORCE.visit(it.lhs, scope)
-		FORCE.visit(it.rhs, scope)
-		scope.emit_ALU(it.op.text)
-
-	@staticmethod
-	def answer(scope: VMFunctionScope):
+	@classmethod
+	def answer(cls, scope: VMFunctionScope):
 		""" Just leave the answer on the stack. """
 		pass
 
-	@staticmethod
-	def visit_Cond(cond:syntax.Cond, scope:VMFunctionScope):
+	def visit_Cond(self, cond:syntax.Cond, scope:VMFunctionScope):
 		FORCE.visit(cond.if_part, scope)
 		label_else = scope.jump_if(False)
-		FORCE.visit(cond.then_part, scope)
+		self.visit(cond.then_part, scope)
 		after = scope.jump_always()
 		scope.come_from(label_else)
 		scope.emit_pop()
-		FORCE.visit(cond.else_part, scope)
+		self.visit(cond.else_part, scope)
 		scope.come_from(after)
 
 class TailContext(FunctionContext):
-	@staticmethod
-	def visit_Lookup(expr:syntax.Lookup, scope:VMFunctionScope):
+	def visit_Lookup(self, expr:syntax.Lookup, scope:VMFunctionScope):
 		sym = expr.ref.dfn
 		scope.load(sym)
 		if symbol_harbors_thunks(sym):
 			scope.emit_force_return()
 		else:
 			scope.emit_return()
 	
 	def call(self, scope: VMFunctionScope, arity:int):
 		scope.emit_exec()
 	
-	@staticmethod
-	def sequel(scope:VMFunctionScope, depth:int, more:bool):
+	def sequel(self, scope:VMFunctionScope, depth:int, more:bool):
+		# Nothing to do here because the alternatives all end with
+		# something that quits this scope.
 		pass
 	
-	@staticmethod
-	def visit_BinExp(it: syntax.BinExp, scope:VMFunctionScope):
+	def visit_BinExp(self, it: syntax.BinExp, scope:VMFunctionScope):
 		FORCE.visit(it.lhs, scope)
 		FORCE.visit(it.rhs, scope)
 		if it.op.text == "<=>":
-			emit("TAIL_CMP")
+			emit("CMP_EXEC")
 		else:
 			scope.emit_ALU(it.op.text)
 			scope.emit_return()
 
-	@staticmethod
-	def answer(scope:VMFunctionScope):
+	@classmethod
+	def answer(cls, scope:VMFunctionScope):
 		""" Have answer on stack; time to return it. """
 		scope.emit_return()
 
-	@staticmethod
-	def visit_Cond(cond:syntax.Cond, scope:VMFunctionScope):
+	def visit_Cond(self, cond:syntax.Cond, scope:VMFunctionScope):
 		FORCE.visit(cond.if_part, scope)
 		label_else = scope.jump_if(False)
-		TAIL.visit(cond.then_part, scope)
+		self.visit(cond.then_part, scope)
 		scope.come_from(label_else)
-		TAIL.visit(cond.else_part, scope)
+		self.visit(cond.else_part, scope)
 
 
 class ProcContext(EagerContext):
 	
-	def call(self, scope: VMFunctionScope, arity:int):
-		scope.emit_call(arity)
-		self.perform(scope)
-
-	def perform(self, scope: VMFunctionScope):
-		raise NotImplementedError(type(self))
-
 	def semicolon(self, scope: VMFunctionScope):
+		# This is a terrible name.
+		# The concept is to put whatever happens after
+		# assembling either an assignment or a skip,
+		# meaning not a transfer-of-control.
+		# In LastContext, that means a RETURN instruction.
 		raise NotImplementedError(type(self))
 
 	def visit_DoBlock(self, do: syntax.DoBlock, scope: VMFunctionScope):
 		for agent in do.agents:
 			scope.alias(agent)
 			FORCE.visit(agent.expr, scope)
 			# At this point a template is on the stack.
@@ -776,46 +772,49 @@
 		for step in do.steps[:-1]:
 			STEP.visit(step, scope)
 			assert scope.depth() == depth
 		self.visit(do.steps[-1], scope)
 		assert scope.depth() in (depth, None)
 		scope.emit_drop(len(do.agents))
 
-	def visit_AssignField(self, af:syntax.AssignField, scope:VMFunctionScope):
+	def visit_AssignMember(self, am:syntax.AssignMember, scope:VMFunctionScope):
 		scope.load(ontology.SELF)
-		FORCE.visit(af.expr, scope)
-		scope.emit_assign_member(af.nom.text)
+		FORCE.visit(am.expr, scope)
+		scope.emit_assign_member(am.nom.text)
 		self.semicolon(scope)
 	
 	def visit_Skip(self, _:syntax.Skip, scope:VMFunctionScope):
 		self.semicolon(scope)
 	
 class StepContext(ProcContext):
-	def perform(self, scope: VMFunctionScope):
+	def call(self, scope: VMFunctionScope, arity: int):
+		scope.emit_call(arity)
+		scope.emit_perform()
+	
+	def answer(self, scope: VMFunctionScope):
 		scope.emit_perform()
 
 	def semicolon(self, scope: VMFunctionScope):
 		pass
-
+	
+StepContext.visit_Cond = ForceContext.visit_Cond
+StepContext.sequel = ForceContext.sequel
 
 class LastContext(ProcContext):
 	""" The procedural context just before return-to-caller """
-	def perform(self, scope: VMFunctionScope):
-		scope.emit_perform_exec()
-		
+
 	def semicolon(self, scope: VMFunctionScope):
+		scope.emit_skip()
 		scope.emit_return()
+	
+LastContext.call = TailContext.call
+LastContext.answer = TailContext.answer
+LastContext.visit_Cond = TailContext.visit_Cond
+LastContext.sequel = TailContext.sequel
 
-	@staticmethod
-	def visit_Cond(cond:syntax.Cond, scope:VMFunctionScope):
-		FORCE.visit(cond.if_part, scope)
-		label_else = scope.jump_if(False)
-		LAST.visit(cond.then_part, scope)
-		scope.come_from(label_else)
-		LAST.visit(cond.else_part, scope)
 
 
 DELAY = LazyContext()
 FORCE = ForceContext()
 TAIL = TailContext()
 STEP = StepContext()
 LAST = LastContext()
@@ -878,15 +877,15 @@
 	for scope, module in each_piece(roadmap):
 		STRUCTURE.write_types(module.types, scope)
 		scope.mangle_names(module.agent_definitions)
 		mangle_foreign_symbols(module.foreign)
 
 	# Write all functions (including FFI):
 	for scope, module in each_piece(roadmap):
-		scope.write_outer_functions(module.outer_functions)
+		scope.write_outer_functions(module.top_subs)
 		scope.write_actors(module.agent_definitions)
 		write_ffi_init(module.foreign)
 	
 	# Delimiter so it's possible to start a begin-expression with a do-block:
 	emit(".begin")
 
 	# Write all begin-expressions:
```

### Comparing `sophie-lang-0.0.6/sophie/modularity.py` & `sophie-lang-0.0.7/sophie/modularity.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 				raise SophieImportError
 			if text is None:
 				assert report.sick()
 			else:
 				enter(abs_path)
 				module = parse_text(text, abs_path, report)
 				if module:
-					report.assert_no_issues()
+					report.assert_no_issues("Parser reported errors but failed to fail.")
 					module.source_path = abs_path
 					chase_the_imports(abs_path.parent, module.imports)
 					parsed_modules[abs_path] = module
 				else:
 					assert report.sick()
 					raise SophieParseError
 				leave()
```

### Comparing `sophie-lang-0.0.6/sophie/ontology.py` & `sophie-lang-0.0.7/sophie/ontology.py`

 * *Files identical despite different names*

### Comparing `sophie-lang-0.0.6/sophie/primitive.py` & `sophie-lang-0.0.7/sophie/primitive.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,11 +15,8 @@
 	root_namespace[name] = symbol
 	return term
 
 literal_number = _built_in_type("number")
 literal_string = _built_in_type("string")
 literal_flag = _built_in_type("flag")
 literal_act = _built_in_type("act")
-literal_msg = _built_in_type("message")
-
-
```

### Comparing `sophie-lang-0.0.6/sophie/resolution.py` & `sophie-lang-0.0.7/sophie/resolution.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 All the definition resolution stuff goes here.
 By the time this pass is finished, every name points to its symbol table entry,
 from which we can find the kind, type, and definition.
 """
 from importlib import import_module
 from pathlib import Path
 from traceback import TracebackException
-from typing import Union
+from typing import Union, Optional, Iterable
 from inspect import signature
 from boozetools.support.foundation import Visitor, strongly_connected_components_hashable
 from boozetools.support.symtab import NoSuchSymbol, SymbolAlreadyExists
 from . import syntax, primitive
 from .diagnostics import Report
 from .ontology import NS, Symbol, SELF
 from .modularity import Program, SophieParseError, SophieImportError
@@ -56,15 +56,15 @@
 			if report.sick(): raise Yuck("constructors")
 			
 			return module
 
 		try: program = Program(main_path, report)
 		except SophieParseError: raise Yuck("parse")
 		except SophieImportError: raise Yuck("import")
-		report.assert_no_issues()
+		report.assert_no_issues("Parser reported an error but failed to fail.")
 		self.import_map = program.import_map
 
 		self.preamble = register(primitive.root_namespace, program.preamble)
 		preamble_scope = self.module_scopes[self.preamble]
 		self.list_symbol = preamble_scope['list']
 		self.order_symbol = preamble_scope['order']
 		for path in program.module_sequence:
@@ -116,15 +116,15 @@
 		self.visit(expr.else_part, env)
 	
 	def visit_ExplicitList(self, expr: syntax.ExplicitList, env):
 		for e in expr.elts:
 			self.visit(e, env)
 	
 	def visit_AsTask(self, at: syntax.AsTask, env):
-		self.visit(at.sub, env)
+		self.visit(at.proc_ref, env)
 
 class _ResolutionPass(TopDown):
 	globals: NS
 	import_alias: NS
 
 	def __init__(self, roadmap: RoadMap, module:syntax.Module, report:Report):
 		self.roadmap = roadmap
@@ -133,14 +133,21 @@
 		self.globals = self.roadmap.module_scopes[module]
 		self.import_alias = self.roadmap.import_alias[module]
 		self.visit_Module()
 
 	def visit_Module(self):
 		raise NotImplementedError(type(self))
 
+	def _install(self, namespace: NS, dfn:Symbol):
+		try: namespace[dfn.nom.key()] = dfn
+		except SymbolAlreadyExists:
+			earlier = namespace[dfn.nom.key()]
+			self.report.redefined_name(earlier, dfn.nom)
+
+
 class _WordDefiner(_ResolutionPass):
 	"""
 	At the end of this phase:
 		Names used in declarations have an attached symbol table entry.
 		The entry is installed in all appropriate namespaces.
 
 	Attaches NameSpace objects in key places and install definitions.
@@ -155,28 +162,22 @@
 		module = self.module
 		for d in module.imports: self.visit_ImportModule(d)
 		for td in module.types: self.visit(td)
 		for d in module.foreign: self.visit_ImportForeign(d)
 		self.assume = NS(place=module.source_path)
 		for a in module.assumptions: self.visit_Assumption(a)
 		# Can't iterate all-functions yet; must build it first.
-		for fn in module.outer_functions:
+		for fn in module.top_subs:
 			self.visit(fn, self.globals)
 		for uda in module.agent_definitions:
-			self.visit(uda, self.globals)
+			self.visit_UserAgent(uda)
 		for expr in module.main:  # Might need to define some case-match symbols here.
 			self.visit(expr, self.globals)
 		pass
 
-	def _install(self, namespace: NS, dfn:Symbol):
-		try: namespace[dfn.nom.key()] = dfn
-		except SymbolAlreadyExists:
-			earlier = namespace[dfn.nom.key()]
-			self.report.redefined_name(earlier, dfn.nom)
-
 	def _declare_type(self, td:syntax.TypeDeclaration):
 		self._install(self.globals, td)
 		self._define_type_params(td)
 
 	def _define_type_params(self, item:Union[syntax.TypeDeclaration, syntax.FFI_Group]):
 		ps = item.param_space = self.globals.new_child(place=item)
 		for p in item.type_params:
@@ -222,44 +223,52 @@
 
 	def visit_Assumption(self, a:syntax.Assumption):
 		""" Update the self.assume namespace accordingly. """
 		for nom in a.names:
 			fp = syntax.FieldDefinition(nom, a.type_expr)
 			self._install(self.assume, fp)
 
+	def tour_where(self, fns:Iterable[syntax.Subroutine], env:NS):
+		for fn in fns:
+			self.visit(fn, env)
+
 	def visit_UserFunction(self, udf:syntax.UserFunction, env:NS):
 		udf.source_path = self.module.source_path
-		self.module.all_functions.append(udf)
+		self.module.all_fns.append(udf)
 		if not isinstance(udf, syntax.UserOperator):
 			self._install(env, udf)
 		inner = udf.namespace = env.new_child(udf)
 		for param in udf.params:
 			self.visit(param, inner)
 		if udf.result_type_expr is not None:
 			self.visit(udf.result_type_expr, inner)
-		for sub_fn in udf.where:
-			self.visit(sub_fn, inner)
+		self.tour_where(udf.where, inner)
 		self.visit(udf.expr, inner)
 
-	def visit_UserAgent(self, uda:syntax.UserAgent, env:NS):
+	def visit_UserAgent(self, uda:syntax.UserAgent):
 		uda.source_path = self.module.source_path
-		self._install(env, uda)
-		field_space = uda.field_space = env.new_child(uda)
-		for f in uda.fields:
-			self.visit(f, field_space)
-		message_space = uda.message_space = NS(place=uda)
+		self._install(self.globals, uda)
+		uda.member_space = self.globals.new_child(uda)
+		for f in uda.members:
+			self.visit(f, uda.member_space)
+		uda.message_space = NS(place=uda)
+		inner = self.globals.new_child(uda)
 		for behavior in uda.behaviors:
-			assert isinstance(behavior, syntax.Behavior)
-			behavior.source_path = self.module.source_path
-			self._install(message_space, behavior)
-			inner = behavior.namespace = env.new_child(behavior)
-			inner['SELF'] = SELF
-			for param in behavior.params:
-				self.visit(param, inner)
-			self.visit(behavior.expr, inner)
+			self._install(uda.message_space, behavior)
+			self.visit_UserProcedure(behavior, inner)
+	
+	def visit_UserProcedure(self, proc:syntax.UserProcedure, env:NS):
+		proc.source_path = self.module.source_path
+		self.module.all_procs.append(proc)
+		self._install(env, proc)
+		inner = proc.namespace = env.new_child(proc)
+		for param in proc.params:
+			self.visit(param, inner)
+		self.tour_where(proc.where, inner)
+		self.visit(proc.expr, inner)
 	
 	def visit_FormalParameter(self, fp:syntax.FormalParameter, env:NS):
 		self._install(env, fp)
 		if fp.type_expr is None and fp.nom.key() in self.assume.local:
 			fp.type_expr = self.assume.local[fp.nom.key()].type_expr
 		if fp.type_expr is not None:
 			self.visit(fp.type_expr, env)
@@ -274,38 +283,34 @@
 		self.visit(lf.function, env)
 	
 	def visit_DoBlock(self, db: syntax.DoBlock, env:NS):
 		if db.agents:
 			inner = env.new_child(db)
 			for new_agent in db.agents:
 				self.visit(new_agent.expr, env)
-				self._install(inner, new_agent)
+				# self._install(inner, new_agent) # Save for _WordResolver...
 		else:
 			inner = env
 		db.namespace = inner
 		for s in db.steps:
 			self.visit(s, inner)
 	
-	def visit_AssignField(self, af:syntax.AssignField, env:NS):
-		return self.visit(af.expr, env)
+	def visit_AssignMember(self, am:syntax.AssignMember, env:NS):
+		return self.visit(am.expr, env)
 
 	def visit_MatchExpr(self, mx:syntax.MatchExpr, env:NS):
 		self.visit(mx.subject.expr, env)
 		inner = mx.namespace = env.new_child(mx)
 		self._install(inner, mx.subject)
 		for alt in mx.alternatives:
-			self.visit(alt, inner)
+			self.tour_where(alt.where, inner)
+			self.visit(alt.sub_expr, inner)
 		if mx.otherwise is not None:
 			self.visit(mx.otherwise, inner)
 
-	def visit_Alternative(self, alt: syntax.Alternative, env: NS):
-		for sub_ex in alt.where:
-			self.visit(sub_ex, env)
-		self.visit(alt.sub_expr, env)
-
 	def visit_ImportModule(self, im:syntax.ImportModule):
 		source_module = self.roadmap.import_map[im]
 		source_namespace = self.roadmap.module_scopes[source_module]
 		if im.nom is not None:
 			self._install(self.import_alias, im)
 		for alias in im.vocab:
 			yonder, hither = alias.yonder, alias.hither or alias.yonder
@@ -347,14 +352,17 @@
 			self.report.undefined_name(sym.span_of_native_name())
 		else: self._install(self.globals, sym)
 	
 	def visit_FFI_Operator(self, sym:syntax.FFI_Operator, py_module):
 		self.visit_FFI_Alias(sym, py_module)
 		self.module.ffi_operators.append(sym)
 
+def _is_a_self_reference(expr:syntax.ValExpr) -> bool:
+	return isinstance(expr, syntax.Lookup) and expr.ref.dfn is SELF
+
 class _WordResolver(_ResolutionPass):
 	"""
 	At the end of this action, every name-reference in the source text is visible where it's used.
 	That is, a corresponding definition-object is in scope. It may not make sense,
 	or be the right kind of name, but at least it's not an obvious misspelling.
 	
 	There is a subtle open question: Do assumed-types share a common namespace for parameters,
@@ -367,31 +375,35 @@
 	Walk the tree looking for undefined words in each static scope.
 	Report on every such occurrence.
 	If this pass succeeds, every syntax.Name object is connected to its corresponding symbol table entry.
 	This is also a good place to pick up interesting lists of syntax objects, such as all match-cases.
 	"""
 	
 	dubious_constructors: list[syntax.Reference]
-	_current_uda = None
+	_current_uda : Optional[syntax.UserAgent] = None
+	_reads_members : set[Symbol] = set()
 	
 	def visit_Module(self):
 		self.dubious_constructors = []
 		module = self.module
 		for td in module.types:
 			self.visit(td)
 		for a in module.assumptions:
 			self.visit(a.type_expr, self.globals)
 		for item in module.foreign:
 			self.visit(item)
 		for item in module.agent_definitions:
-			self.visit(item)
-		for item in module.all_functions:
-			self.visit(item)
+			self.visit_UserAgent(item)
+		self.tour_where(module.top_subs)
 		for expr in module.main:
 			self.visit(expr, self.globals)
+	
+	def tour_where(self, fns:Iterable[syntax.Subroutine]):
+		for fn in fns:
+			self.visit(fn)
 
 	def visit_Variant(self, v:syntax.Variant):
 		for st in v.subtypes:
 			if st.body is not None:
 				self.visit(st.body, v.param_space)
 	
 	def visit_Record(self, r:syntax.Record):
@@ -408,29 +420,51 @@
 			self.visit(f.type_expr, env)
 	
 	def _lookup(self, nom:syntax.Nom, env:NS):
 		try: return env[nom.key()]
 		except NoSuchSymbol:
 			self.report.undefined_name(nom.head())
 			return Bogon(nom)
+	
+	def _lookup_member(self, nom:syntax.Nom):
+		if self._current_uda is None:
+			self.report.can_only_see_member_within_behavior(nom)
+			return Bogon(nom)
+		try:
+			return self._current_uda.member_space.local[nom.key()]
+		except KeyError:
+			self.report.undefined_name(nom.head())
+			return Bogon(nom)
 
 	def visit_PlainReference(self, ref:syntax.PlainReference, env:NS):
 		# This kind of reference searches the local-scoped name-space
 		ref.dfn = self._lookup(ref.nom, env)
 	
+	def visit_SelfReference(self, ref:syntax.SelfReference, env:NS):
+		if self._current_uda is None:
+			self.report.undefined_name(ref.nom.head())
+			return Bogon(ref.nom)
+		else:
+			ref.dfn = SELF
+
 	def visit_QualifiedReference(self, ref:syntax.QualifiedReference, env:NS):
 		# Search among imports.
 		im = self._lookup(ref.space, self.import_alias)
 		if isinstance(im, Bogon): ref.dfn = im
 		else:
 			assert isinstance(im, syntax.ImportModule)
 			target_module = self.roadmap.import_map[im]
 			target_namespace = self.roadmap.module_scopes[target_module]
 			ref.dfn = self._lookup(ref.nom, target_namespace)
 	
+	def visit_MemberReference(self, ref:syntax.MemberReference, env:NS):
+		# Search among the members of the actor-scope.
+		ref.dfn = self._lookup_member(ref.nom)
+		self._reads_members.add(ref.dfn)
+	
 	def visit_Interface(self, i:syntax.Interface):
 		for ms in i.spec:
 			assert isinstance(ms, syntax.MethodSpec)
 			self.visit(ms, i.param_space)
 	
 	def visit_MethodSpec(self, ms:syntax.MethodSpec, env:NS):
 		for tx in ms.type_exprs:
@@ -445,82 +479,89 @@
 		for p in tc.arguments:
 			self.visit(p, env)
 
 	def visit_ExplicitTypeVariable(self, gt:syntax.ExplicitTypeVariable, env:NS):
 		assert gt.nom.key() in env
 		gt.dfn = self._lookup(gt.nom, env)
 
-	def visit_UserFunction(self, sym:syntax.UserFunction):
-		for param in sym.params:
+	def visit_UserFunction(self, fn:syntax.UserFunction):
+		for param in fn.params:
 			if param.type_expr is not None:
-				self.visit(param.type_expr, sym.namespace)
-		if sym.result_type_expr is not None:
-			self.visit(sym.result_type_expr, sym.namespace)
-		self.visit(sym.expr, sym.namespace)
+				self.visit(param.type_expr, fn.namespace)
+		if fn.result_type_expr is not None:
+			self.visit(fn.result_type_expr, fn.namespace)
+		self.visit(fn.expr, fn.namespace)
+		self.tour_where(fn.where)
 
 	def visit_UserAgent(self, uda:syntax.UserAgent):
-		for f in uda.fields:
-			self.visit(f.type_expr, uda.field_space)
+		for f in uda.members:
+			if f.type_expr is not None:
+				self.visit(f.type_expr, uda.member_space)
 		self._current_uda = uda
 		for b in uda.behaviors:
-			self.visit(b, uda.field_space)
+			self._reads_members = b.reads_members = set()
+			self.visit_UserProcedure(b)
+			
 		self._current_uda = None
 	
-	def visit_Behavior(self, sym:syntax.Behavior, env:NS):
+	def visit_UserProcedure(self, sym:syntax.UserProcedure):
 		for param in sym.params:
 			if param.type_expr is not None:
 				self.visit(param.type_expr, sym.namespace)
 		self.visit(sym.expr, sym.namespace)
+		self.tour_where(sym.where)
 
 	def visit_MatchExpr(self, mx:syntax.MatchExpr, env:NS):
 		self.visit(mx.subject.expr, env)
 		if mx.hint is not None:
 			self.visit(mx.hint, env)
 		_build_match_dispatch(mx, self.globals, self.report)
 		for alt in mx.alternatives:
 			self.visit(alt.sub_expr, mx.namespace)
-			for sub_ex in alt.where:
-				self.visit(sub_ex)
+			self.tour_where(alt.where)
 		if mx.otherwise is not None:
 			self.visit(mx.otherwise, mx.namespace)
 			
 	def visit_Lookup(self, lu: syntax.Lookup, env: NS):
 		self.visit(lu.ref, env)
 		dfn = lu.ref.dfn
 		if isinstance(dfn, syntax.TypeAlias) or not dfn.has_value_domain():
 			self.dubious_constructors.append(lu.ref)
 	
+	def visit_FieldReference(self, expr: syntax.FieldReference, env):
+		super().visit_FieldReference(expr, env)
+		if _is_a_self_reference(expr):
+			self.report.use_my_instead(env, expr)
+	
 	def visit_LambdaForm(self, lf: syntax.LambdaForm, env: NS):
-		pass
+		self.visit_UserFunction(lf.function)
 	
 	def visit_DoBlock(self, db: syntax.DoBlock, env:NS):
 		for new_agent in db.agents:
-			self.visit(new_agent.expr, env)
+			self.visit(new_agent.expr, db.namespace)
+			self._install(db.namespace, new_agent)
 		for s in db.steps:
 			self.visit(s, db.namespace)
 
-	def visit_AssignField(self, af:syntax.AssignField, env:NS):
-		if self._current_uda is None:
-			self.report.can_only_assign_within_behavior(af)
-			af.dfn = Bogon(af.nom)
-		else:
-			af.dfn = self._lookup(af.nom, self._current_uda.field_space)
-		return self.visit(af.expr, env)
+	def visit_AssignMember(self, am:syntax.AssignMember, env:NS):
+		am.dfn = self._lookup_member(am.nom)
+		return self.visit(am.expr, env)
 	
 	def visit_ImportForeign(self, d:syntax.ImportForeign):
 		for ref in d.linkage or ():
 			self.visit(ref, self.globals)
 		for group in d.groups:
 			self.visit(group.type_expr, group.param_space)
 
 class Bogon(syntax.Symbol):
 	def has_value_domain(self) -> bool:
 		return False
 
 class _AliasChecker(Visitor):
+	# TODO: Split this into two separate passes.
 	"""
 	Check the arity of TypeCall forms.
 	Check for aliases being well-founded, up front before getting caught in a loop later:
 	There should be no cycles in the aliasing dependency graph, and no wrong-kind references.
 	Also re-orders type definitions in order of alias topology.
 	
 	Stop worrying about function cycles; I'll catch that problem in the type checker.
@@ -534,15 +575,15 @@
 		self.non_types = []
 		self.graph = {td:[] for td in module.types}
 		
 		self._tour(module.types)
 		self._tour(module.foreign)
 		self._tour(module.assumptions)
 		self._tour(module.agent_definitions)
-		self._tour(module.all_functions)
+		self._tour(module.all_fns)
 		if self.non_types:
 			self.report.these_are_not_types(self.non_types)
 		alias_order = []
 		ok = True
 		for scc in strongly_connected_components_hashable(self.graph):
 			if len(scc) == 1:
 				node = scc[0]
@@ -634,18 +675,18 @@
 
 	def visit_UserFunction(self, sym:syntax.UserFunction):
 		self._tour(sym.params, True)
 		if sym.result_type_expr:
 			self.visit(sym.result_type_expr, True)
 
 	def visit_UserAgent(self, sym:syntax.UserAgent):
-		self._tour(sym.fields, True)
+		self._tour(sym.members, True)
 		self._tour(sym.behaviors)
 	
-	def visit_Behavior(self, b:syntax.Behavior):
+	def visit_UserProcedure(self, b:syntax.UserProcedure):
 		self._tour(b.params, True)
 
 	def visit_ImportForeign(self, d:syntax.ImportForeign):
 		for group in d.groups:
 			self.visit(group.type_expr, False)
 
 def check_constructors(dubious_constructors:list[syntax.Reference], report:Report):
```

### Comparing `sophie-lang-0.0.6/sophie/runtime.py` & `sophie-lang-0.0.7/sophie/runtime.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,18 +2,14 @@
 from typing import Any, Union, Sequence, Optional, Reversible
 from . import syntax, primitive
 from .ontology import SELF
 from .stacking import Frame, Activation, RootFrame
 from .scheduler import Task, Actor
 from .diagnostics import trace_absurdity
 
-LESS:Optional[dict] = None # Gets replaced at runtime.
-SAME:Optional[dict] = None # Gets replaced at runtime.
-MORE:Optional[dict] = None # Gets replaced at runtime.
-
 def _compare(a,b):
 	if a < b: return LESS
 	if a == b: return SAME
 	return MORE
 
 PRIMITIVE_BINARY = {
 	"^"   : operator.pow,
@@ -85,14 +81,17 @@
 		self.value = ABSENT
 		
 	def __str__(self):
 		if self.value is ABSENT:
 			return "<Thunk: %s>"%self.expr
 		else:
 			return str(self.value)
+	
+	def perform(self, dynamic_env:ENV):
+		return force(self)
 
 def force(it:LAZY_VALUE) -> STRICT_VALUE:
 	"""
 	Force repeatedly until the result is no longer a thunk, then return that result.
 	This simulates tail-call elimination, now that closures promptly return thunks.
 	"""
 	while isinstance(it, Thunk):
@@ -115,16 +114,18 @@
 	static_env = dynamic_env.chase(sym)
 	try: return static_env.fetch(sym)
 	except KeyError:
 		if isinstance(sym, syntax.UserFunction):
 			if sym.params:
 				value = Closure(static_env, sym)
 			else:
-				inner = Activation.for_function(static_env, dynamic_env, sym, ())
+				inner = Activation.for_subroutine(static_env, dynamic_env, sym, ())
 				value = delay(sym.expr, inner)
+		elif isinstance(sym, syntax.UserProcedure):
+			value = Closure(static_env, sym)
 		elif isinstance(sym, syntax.TypeAlias):
 			value = _snap_type_alias(sym, static_env)
 		else:
 			assert False, type(sym)
 		return static_env.assign(sym, value)
 
 def _eval_lambda_form(expr:syntax.LambdaForm, dynamic_env:ENV):
@@ -176,42 +177,49 @@
 def _eval_match_expr(expr:syntax.MatchExpr, dynamic_env:ENV):
 	subject = dynamic_env.assign(expr.subject, _strict(expr.subject.expr, dynamic_env))
 	tag = subject[""]
 	try:
 		alternative = expr.dispatch[tag]
 	except KeyError:
 		branch = expr.otherwise
-		assert branch is not None, tag
+		assert branch is not None, (tag, type(tag))
 		return evaluate(branch, dynamic_env)
 	else:
 		for sub_fn in alternative.where:
 			dynamic_env.declare(sub_fn)
 		return evaluate(alternative.sub_expr, dynamic_env)
 
 def _eval_do_block(expr:syntax.DoBlock, dynamic_env:ENV):
-	return CompoundAction(expr, dynamic_env)
+	agents = expr.agents
+	if agents:
+		inner = Activation.for_do_block(dynamic_env)
+		for na in agents:
+			assert isinstance(na, syntax.NewAgent)
+			template = _strict(na.expr, inner)
+			inner.assign(na, template.instantiate())
+	else:
+		inner = dynamic_env
+	# TODO: Solve the tail-recursion problem.
+	for expr in expr.steps:
+		inner.pc = expr
+		perform(_strict(expr, inner), inner)
 
 def _eval_skip(expr:syntax.Skip, dynamic_env:ENV):
-	return Nop()
+	return
 
 def _eval_bind_method(expr:syntax.BindMethod, dynamic_env:ENV):
 	return BoundMethod(_strict(expr.receiver, dynamic_env), expr.method_name.text)
 
 def _eval_as_task(expr:syntax.AsTask, dynamic_env:ENV):
-	sub = _strict(expr.sub, dynamic_env)
-	if isinstance(sub, Closure):
-		return ClosureMessage(sub)
-	else:
-		assert isinstance(sub, Action), type(sub)
-		assert not isinstance(sub, BoundMethod)
-		return PlainTask(sub)
-
-def _eval_assign_field(expr:syntax.AssignField, dynamic_env:ENV):
-	state = dynamic_env.chase(SELF).fetch(SELF)
-	return AssignAction(state, expr.nom.key(), evaluate(expr.expr, dynamic_env))
+	sub = _strict(expr.proc_ref, dynamic_env)
+	return sub.as_task()
+
+def _eval_assign_member(expr:syntax.AssignMember, dynamic_env:ENV):
+	uda = dynamic_env.chase(SELF).fetch(SELF)
+	uda.state[expr.dfn] = _strict(expr.expr, dynamic_env)
 
 def _eval_absurdity(expr:syntax.Absurdity, dynamic_env:ENV):
 	trace_absurdity(dynamic_env, expr)
 	exit()
 	
 
 ###############################################################################
@@ -234,16 +242,14 @@
 	return fn(expr, dynamic_env)
 
 _NO_DELAY = {syntax.Literal, syntax.Lookup, syntax.DoBlock, syntax.LambdaForm}
 
 def delay(expr: syntax.ValExpr, dynamic_env: ENV) -> LAZY_VALUE:
 	# For certain kinds of expression, there is no profit to delay:
 	if type(expr) in _NO_DELAY: return evaluate(expr, dynamic_env)
-	# Volatile expressions (that depend on a field of SELF) must not delay:
-	if expr.is_volatile: return _strict(expr, dynamic_env)
 	# In less trivial cases, make a thunk and pass that instead.
 	return Thunk(expr, dynamic_env)
 
 EVALUATE = {}
 for _k, _v in list(globals().items()):
 	if _k.startswith("_eval_"):
 		_t = _v.__annotations__["expr"]
@@ -259,30 +265,37 @@
 		# lest various internal things fail to work,
 		# which things to not tie back to specific syntax objects.
 		# For example, explicit lists.
 		raise NotImplementedError
 
 class Closure(Function):
 	""" The run-time manifestation of a sub-function: a callable value tied to its natal environment. """
+	# For now, I'll use Closure for both functions and procedures.
 
-	def __init__(self, static_link:ENV, udf:syntax.UserFunction):
+	def __init__(self, static_link:ENV, udf:syntax.Subroutine):
 		assert hasattr(udf, "strictures"), udf
 		self._static_link = static_link
 		self._udf = udf
 	
 	def __str__(self):
 		return str(self._udf)
 	
 	def _name(self): return self._udf.nom.text
 
 	def apply(self, args: Sequence[LAZY_VALUE], dynamic_env:ENV) -> LAZY_VALUE:
 		for i in self._udf.strictures:
 			force(args[i])
-		inner_env = Activation.for_function(self._static_link, dynamic_env, self._udf, args)
+		inner_env = Activation.for_subroutine(self._static_link, dynamic_env, self._udf, args)
 		return delay(self._udf.expr, inner_env)
+	
+	def perform(self, dynamic_env:ENV) -> STRICT_VALUE:
+		return self.apply((), dynamic_env)
+	
+	def as_task(self):
+		return ParametricTask(self) if self._udf.params else PlainTask(self, ())
 
 class Primitive(Function):
 	""" All parameters to primitive procedures are strict. Also a kind of value, like a closure. """
 	def __init__(self, fn: callable):
 		self._fn = fn
 	
 	def apply(self, args: Sequence[LAZY_VALUE], dynamic_env:ENV) -> STRICT_VALUE:
@@ -306,163 +319,129 @@
 
 class ActorClass(Function):
 	def __init__(self, global_link:ENV, uda:syntax.UserAgent):
 		self._global_link = global_link
 		self._uda = uda
 		
 	def apply(self, args: Sequence[LAZY_VALUE], dynamic_env:ENV) -> "ActorTemplate":
-		assert len(args) == len(self._uda.fields)
+		assert len(args) == len(self._uda.members)
 		return ActorTemplate(self._global_link, self._uda, args)
 
 
 class ActorTemplate:
 	def __init__(self, global_link:ENV, uda:syntax.UserAgent, args: Sequence[LAZY_VALUE]):
 		self._global_link = global_link
 		self._uda = uda
 		self._args = args
 	
-	def instantiate(self, dynamic_link:ENV):
-		private_state = dict(zip(self._uda.field_names(), map(force, self._args)))
-		private_state[VTABLE] = self._uda.message_space.local
-		frame = Activation(self._global_link, dynamic_link, self._uda)
-		frame.assign(SELF, private_state)
-		return UserDefinedActor(frame)
-
-###############################################################################
+	def instantiate(self):
+		state = dict(zip(self._uda.members, map(force, self._args)))
+		vtable = self._uda.message_space.local
+		return UserDefinedActor(state, vtable, self._global_link)
 
-class Action:
-	def perform(self):
-		""" Do something here and now in the current thread. """
-		raise NotImplementedError(type(self))
-
-class Nop(Action):
-	def perform(self): pass
-
-class AssignAction(Action):
-	def __init__(self, state:dict[str,STRICT_VALUE], field_name:str, new_value:LAZY_VALUE):
-		self._state = state
-		self._field_name = field_name
-		self._new_value = new_value
-	def perform(self):
-		self._state[self._field_name] = force(self._new_value)
-
-class CompoundAction(Action):
-	def __init__(self, block:syntax.DoBlock, dynamic_env:ENV):
-		self._block = block
-		self._dynamic_env = dynamic_env
-	def perform(self):
-		agents = self._block.agents
-		if agents:
-			inner = Activation.for_do_block(self._dynamic_env)
-			for na in agents:
-				assert isinstance(na, syntax.NewAgent)
-				template = _strict(na.expr, self._dynamic_env)
-				inner.assign(na, template.instantiate(self._dynamic_env))
-		else:
-			inner = self._dynamic_env
-		# TODO: Solve the tail-recursion problem.
-		for expr in self._block.steps:
-			inner.pc = expr
-			action = _strict(expr, inner)
-			action.perform()
+class UserDefinedActor(Actor):
+	def __init__(self, state:dict, vtable:dict, global_env:ENV):
+		super().__init__()
+		self.state = state
+		self._vtable = vtable
+		self._global_env = global_env
+	
+	def handle(self, message, args):
+		behavior = self._vtable[message]
+		frame = Activation.for_subroutine(self._global_env, self._global_env, behavior, args)
+		frame.assign(SELF, self)
+		frame.update(self.state)
+		perform(evaluate(behavior.expr, frame), frame)
 
-class BoundMessage(Action):
-	def __init__(self, receiver, method_name, *args):
-		self._receiver = receiver
-		self._method_name = method_name
-		self._args = args
-		
-	def perform(self):
-		self._receiver.accept_message(self._method_name, self._args)
+###############################################################################
 
-class TaskAction(Action):
-	def __init__(self, task:Task):
-		self._task = task
-	def perform(self):
-		self._task.enqueue()
+def perform(action, dynamic_env:ENV):
+	while action is not None:
+		action = action.perform(dynamic_env)
 
 ###############################################################################
-
-class Message(Function):
+class ParametricMessage(Function):
 	""" Interface for things that, with arguments, become messages ready to send. """
 	def dispatch_with(self, *args):
-		self.apply(args, THREADED_ROOT).perform()
+		self.apply(args, THREADED_ROOT).perform(THREADED_ROOT)
+
+class ParametricTask(ParametricMessage):
+	def __init__(self, closure: Closure):
+		self._closure = closure
+
+	def apply(self, args: Sequence[LAZY_VALUE], dynamic_env:ENV) -> Any:
+		return PlainTask(self._closure, tuple(force(a) for a in args))
 
-class BoundMethod(Message, Action):
+class BoundMethod(ParametricMessage):
 	def __init__(self, receiver, method_name):
 		self._receiver = receiver
 		self._method_name = method_name
 
-	def apply(self, args: Sequence[LAZY_VALUE], dynamic_env:ENV) -> LAZY_VALUE:
-		return BoundMessage(self._receiver, self._method_name, *(force(a) for a in args))
-	
-	def perform(self):
-		""" Hack so that a single runtime class handles both parametric and non-parametric messages to actors """
-		self._receiver.accept_message(self._method_name, ())
-
-class ClosureMessage(Message):
-	def __init__(self, closure: Closure):
-		self._closure = closure
-
 	def apply(self, args: Sequence[LAZY_VALUE], dynamic_env:ENV) -> Any:
-		task = ParametricTask(self._closure, [force(a) for a in args])
-		return TaskAction(task)
+		return MessageTask(self._receiver, self._method_name, tuple(force(a) for a in args))
+
+	def perform(self, dynamic_env:ENV):
+		self._receiver.accept_message(self._method_name, ())
 	
-###############################################################################
+class MessageTask:
+	def __init__(self, receiver, method_name, args:Sequence[STRICT_VALUE]):
+		self._receiver = receiver
+		self._method_name = method_name
+		self._args = args
+		
+	def perform(self, dynamic_env:ENV):
+		self._receiver.accept_message(self._method_name, self._args)
 
 class PlainTask(Task):
-	def __init__(self, action:Action):
-		self._action = action
-	def proceed(self):
-		self._action.perform()
-
-class ParametricTask(Task):
 	def __init__(self, closure:Closure, args:Sequence[STRICT_VALUE]):
 		self._closure = closure
 		self._args = args
-	def proceed(self):
-		action = force(self._closure.apply(self._args, THREADED_ROOT))
-		assert isinstance(action, Action), type(action)
-		action.perform()
+	
+	def perform(self, dynamic_env:ENV):
+		self.enqueue()
 
-class UserDefinedActor(Actor):
-	def __init__(self, frame:ENV):
-		super().__init__()
-		self._frame = frame
+	def proceed(self):
+		it = self._closure.apply(self._args, THREADED_ROOT)
+		perform(it, THREADED_ROOT)
 	
-	def handle(self, message, args):
-		state = self._frame.fetch(SELF)
-		behavior = state[VTABLE][message]
-		assert isinstance(behavior, syntax.Behavior)
-		frame = Activation.for_behavior(self._frame, THREADED_ROOT, behavior, args)
-		_strict(behavior.expr, frame).perform()
 
 ###############################################################################
 
 NIL:Optional[dict] = None # Gets replaced at runtime.
+LESS:Optional[dict] = None # Gets replaced at runtime.
+SAME:Optional[dict] = None # Gets replaced at runtime.
+MORE:Optional[dict] = None # Gets replaced at runtime.
+NOPE:Optional[dict] = None # Gets replaced at runtime.
 CONS:Constructor
+THIS:Constructor
 
 def iterate_list(lst:LAZY_VALUE):
 	lst = force(lst)
 	while lst[""] == CONS.key:
 		yield force(lst['head'])
 		lst = force(lst['tail'])
 	assert lst[""] == NIL[""]
 
 def as_sophie_list(items:Reversible):
 	lst = NIL
 	for head in reversed(items):
-		lst = {"":"cons", "head":head, "tail":lst}
+		lst = {"":CONS.key, "head":head, "tail":lst}
 	return lst
 
+def is_sophie_list(it:STRICT_VALUE):
+	return isinstance(it, dict) and it[""] is CONS.key
+
+def sophie_nope(): return NOPE
+def sophie_this(item): return {"":THIS.key, "item":item}
+
 ###############################################################################
 
 def reset(fetch):
 	OVERLOAD.clear()
-	for k in 'nil', 'cons', 'less', 'same', 'more':
+	for k in 'nil', 'cons', 'less', 'same', 'more', 'this', 'nope':
 		globals()[k.upper()] = fetch(k)
 	for relation, cases in {
 		"<":("less",),
 		"==":("same",),
 		">":("more",),
 		"!=":("less", "more"),
 		"<=":("less", "same"),
```

### Comparing `sophie-lang-0.0.6/sophie/scheduler.py` & `sophie-lang-0.0.7/sophie/scheduler.py`

 * *Files identical despite different names*

### Comparing `sophie-lang-0.0.6/sophie/stacking.py` & `sophie-lang-0.0.7/sophie/stacking.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 """
 This is supposed to be a support module for anything that smells of executing code.
 Because Sophie's type-checking philosophy is "run the program over the types",
 that means these activation records get used in both the type-checker and the evaluator.
 
 Despite superficial similarity, this is not treated quite the same as a namespace.
-
-For now I've removed the complexity of tracking static depth.
-Sophie does run a little slower this way, but it's for a purpose.
-Upon this simplified foundation, I'll build as needed to properly reflect
-the upcoming message-passing semantics.
 """
 
-from typing import TypeVar, Generic, Union
+from typing import TypeVar, Generic, Union, Optional
 from pathlib import Path
 from .ontology import Symbol
-from .syntax import UserFunction, Behavior, ValExpr, Subject, Module
+from .syntax import Subroutine, ValExpr, Subject, Module
 
-CRUMB = Union[Symbol, Module]
+CRUMB = Union[Symbol, Module, None]
 
 T = TypeVar("T")
 
 PLACE_HOLDER = object()
 
 class Frame(Generic[T]):
 	_bindings : dict[Symbol, T]
@@ -30,14 +25,16 @@
 	def chase(self, key:Symbol) -> "Frame[T]": raise NotImplementedError(type(self))
 	def trace(self, tracer): raise NotImplementedError(type(self))
 	def declare(self, key:Symbol): self.assign(key, PLACE_HOLDER)
 	def holds(self, key:Symbol) -> bool: return key in self._bindings
 	def assign(self, key:Symbol, value:T):
 		self._bindings[key] = value
 		return value
+	def update(self, pairs):
+		self._bindings.update(pairs)
 	def fetch(self, key:Symbol) -> T:
 		item = self._bindings[key]
 		if item is PLACE_HOLDER: raise KeyError(key)
 		else: return item
 
 class RootFrame(Frame):
 	"""The runtime counterpart to primitive-root namespace"""
@@ -54,58 +51,55 @@
 	def absorb(self, other:Frame):
 		# This kludge allows imported symbols to work.
 		# The root-frame stands in for an inter-module linkage model.
 		self._bindings.update(other._bindings)
 
 class Activation(Frame):
 	def __init__(self, static_link: Frame[T], dynamic_link: Frame[T], breadcrumb:CRUMB):
-		assert hasattr(breadcrumb, 'source_path'), type(breadcrumb)
 		self._bindings = {}
 		self._static_link = static_link
 		self._dynamic_link = dynamic_link
 		self.breadcrumb = breadcrumb
 	
-	def path(self) -> Path:
-		return self.breadcrumb.source_path
+	def path(self) -> Optional[Path]:
+		if self.breadcrumb and hasattr(self.breadcrumb, 'source_path'):
+			return self.breadcrumb.source_path
+		else:
+			return self._static_link.path() 
 		
 	def chase(self, key:Symbol) -> Frame[T]:
 		return self if key in self._bindings else self._static_link.chase(key)
 
 	def trace(self, tracer):
 		self._dynamic_link.trace(tracer)
-		tracer.trace_frame(self.breadcrumb, self._bindings, self.pc)
-
+		if self.breadcrumb is not None:
+			tracer.trace_frame(self.path(), self.breadcrumb, self._bindings)
+		if self.pc is not None: tracer.called_from(self.path(), self.pc)
+	
 	@staticmethod
-	def for_function(static_link: Frame[T], dynamic_link: Frame[T], udf: UserFunction, arguments) -> "Activation[T]":
-		assert len(udf.params) == len(arguments)
-		ar = Activation(static_link, dynamic_link, udf)
-		ar._bindings.update(zip(udf.params, arguments))
-		for key in udf.where:
+	def for_subroutine(static_link: Frame[T], dynamic_link: Frame[T], sub: Subroutine, arguments) -> "Activation[T]":
+		assert len(sub.params) == len(arguments), (sub, arguments)
+		ar = Activation(static_link, dynamic_link, sub)
+		ar.update(zip(sub.params, arguments))
+		for key in sub.where:
 			ar.declare(key)
 		return ar
 
 	@staticmethod
-	def for_subject(static_link: Frame[T], subject:Subject) -> "Activation[T]":
-		ar = Activation(static_link, static_link, static_link.breadcrumb)
-		ar.declare(subject)
+	def for_subject(static_link: Frame[T], subject:Subject, value:T) -> "Activation[T]":
+		ar = Activation(static_link, static_link, subject)
+		ar.assign(subject, value)
 		return ar
 	
 	@staticmethod
 	def for_module(static_link: Frame[T], module:Module) -> "Activation[T]":
 		ar = Activation(static_link, RootFrame(), module)
-		for udf in module.outer_functions:
+		for udf in module.top_subs:
 			ar.declare(udf)
 		for uda in module.agent_definitions:
 			ar.declare(uda)
 		return ar
 
 	@staticmethod
 	def for_do_block(static_link: Frame[T]) -> "Activation[T]":
-		return Activation(static_link, static_link, static_link.breadcrumb)
-
-	@staticmethod
-	def for_behavior(static_link: Frame[T], dynamic_link: Frame[T], b:Behavior, arguments) -> "Activation[T]":
-		assert len(b.params) == len(arguments)
-		ar = Activation(static_link, dynamic_link, b)
-		ar._bindings.update(zip(b.params, arguments))
-		return ar
+		return Activation(static_link, static_link, None)
```

### Comparing `sophie-lang-0.0.6/sophie/syntax.py` & `sophie-lang-0.0.7/sophie/syntax.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,20 +42,27 @@
 
 
 class SimpleType(Expr):
 	def can_construct(self) -> bool: raise NotImplementedError(type(self))
 	def dispatch_token(self): raise NotImplementedError(type(self))
 
 class ValExpr(Expr):
-	is_volatile: bool
 	pass
 
 class PlainReference(Reference):
 	def head(self) -> slice: return self.nom.head()
-	def __str__(self): return "<ref:%s>"%self.nom.text
+	def __repr__(self): return "<ref:%s>"%self.nom.text
+
+class SelfReference(Reference):
+	def head(self) -> slice: return self.nom.head()
+	def __repr__(self): return "<SELF>"
+
+class MemberReference(Reference):
+	def head(self) -> slice: return self.nom.head()
+	def __repr__(self): return "<my %s>"%self.nom.text
 
 class QualifiedReference(Reference):
 	space: Nom
 	def __init__(self, nom:Nom, space:Nom):
 		super().__init__(nom)
 		self.space = space
 	def head(self) -> slice:
@@ -92,14 +99,16 @@
 		self.ref, self.arguments = ref, arguments or ()
 	def head(self) -> slice: return self.ref.head()
 	def can_construct(self) -> bool: return self.ref.dfn.has_value_domain()
 	def dispatch_token(self):
 		symbol = self.ref.dfn
 		assert isinstance(symbol, TypeDeclaration)
 		return symbol.as_token()
+	def __repr__(self):
+		return "%s[%s]"%(self.ref, self.arguments) if self.arguments else repr(self.ref)
 
 class ImplicitTypeVariable:
 	""" Stand-in as the relevant type-expression for when the syntax doesn't bother. """
 	def __init__(self, head:Nom):
 		self._head = head
 	def head(self) -> slice:
 		return self._head.head()
@@ -175,15 +184,15 @@
 	def has_value_domain(self) -> bool: return False
 	def as_token(self): return self
 
 class MethodSpec(Symbol):
 	interface_decl : "Interface"
 	def __init__(self, nom:Nom, type_exprs:Sequence[SimpleType]):
 		super().__init__(nom)
-		self.type_exprs = type_exprs
+		self.type_exprs = type_exprs or ()
 	def has_value_domain(self) -> bool: return False
 
 class Interface(TypeDeclaration):
 	method_space: NS
 	def __init__(self, nom: Nom, type_params:tuple[TypeParameter, ...], spec:Sequence[MethodSpec]):
 		super().__init__(nom, type_params)
 		self.spec = spec
@@ -205,48 +214,54 @@
 	def __repr__(self): return "<%s>"%self.nom.text
 	def as_token(self): return self.variant
 
 class Assumption(NamedTuple):
 	names: list[Nom]
 	type_expr: SimpleType
 
-def _bookend(head: Nom, coda: Nom):
-	if head.text != coda.text:
-		raise MismatchedBookendsError(head.head(), coda.head())
+def _bookend(head: Nom, where: Optional["WhereClause"]) -> Sequence["Subroutine"]:
+	if where is None: return ()
+	if head.text == where.coda.text:
+		return where.sub_fns
+	else:
+		raise MismatchedBookendsError(head.head(), where.coda.head())
+	
 
-class UserFunction(Term):
-	namespace: NS
+class Subroutine(Term):
 	params: Sequence[FormalParameter]
-	where: Sequence["UserFunction"]
+	expr: ValExpr
+	where: Sequence["Subroutine"]
 	strictures: tuple[int, ...] # Tree-walking runtime uses this.
+	def is_thunk(self) -> bool:
+		""" So the compiler can decide how to encode these things """
+		raise NotImplementedError(type(self))
+
+class UserFunction(Subroutine):
+	namespace: NS
 	
 	def __init__(
 			self,
 			nom: Nom,
 			params: Sequence[FormalParameter],
 			expr_type: Optional[ARGUMENT_TYPE],
 			expr: ValExpr,
 			where: Optional["WhereClause"]
 	):
 		super().__init__(nom)
 		self.params = params or ()
 		self.result_type_expr = expr_type
 		self.expr = expr
-		if where:
-			_bookend(nom, where.coda)
-			self.where = where.sub_fns
-		else:
-			self.where = ()
+		self.where = _bookend(nom, where)
 			
-	def has_volatility(self):
-		return self.expr.is_volatile or any(f.has_volatility() for f in self.where)
-	
 	def head(self) -> slice:
 		return self.nom.head()
 	
+	def is_thunk(self) -> bool:
+		return not self.params
+	
 	def __repr__(self):
 		p = ", ".join(map(str, self.params))
 		return "{fn|%s(%s)}" % (self.nom.text, p)
 
 class UserOperator(UserFunction):
 	"""
 	An operator is just a function with a funny name
@@ -257,58 +272,64 @@
 		for fp in self.params:
 			fp.is_strict = True
 	
 	def dispatch_vector(self):
 		return tuple(fp.dispatch_token() for fp in self.params)
 
 class WhereClause(NamedTuple):
-	sub_fns: Sequence[UserFunction]
+	sub_fns: Sequence[Subroutine]
 	coda: Nom
 
 class UserAgent(Term):
-	field_space: NS
-	fields: Sequence[FormalParameter]
+	member_space: NS
+	members: Sequence[FormalParameter]
 	message_space: NS
 	def head(self) -> slice: return self.nom.head()
 	def __init__(
 		self,
 		nom: Nom,
-		fields: Optional[Sequence[FormalParameter]],
-		behaviors: Sequence["Behavior"],
+		members: Optional[Sequence[FormalParameter]],
+		behaviors: Sequence["UserProcedure"],
 		coda: Nom,
 	):
 		super().__init__(nom)
-		self.fields = fields or ()
+		self.members = members or ()
 		self.behaviors = behaviors
-		_bookend(nom, coda)
+		if nom.text != coda.text:
+			raise MismatchedBookendsError(nom.head(), coda.head())
 
-	def field_names(self):
-		return [f.nom.text for f in self.fields]
+	def member_names(self):
+		return [f.nom.text for f in self.members]
 
 
-class Behavior(Term):
+class UserProcedure(Subroutine):
 	namespace: NS
+	reads_members: set[FormalParameter]  # Resolver must fill this.
+	
 	def head(self) -> slice: return self.nom.head()
 	def __repr__(self):
 		p = ", ".join(map(str, self.params))
 		return "{to %s(%s)}" % (self.nom.text, p)
 	def __init__(
 		self,
 		nom: Nom,
 		params: Sequence[FormalParameter],
 		expr: ValExpr,
+		where: Optional["WhereClause"]
 	):
 		super().__init__(nom)
 		self.params = params or ()
 		for p in self.params: p.is_strict = True
 		self.expr = expr
+		self.where = _bookend(nom, where)
+	
+	def is_thunk(self) -> bool:
+		return False
 
 class Literal(ValExpr):
-	is_volatile = False  # Not that this will ever be tested, but it's well to be consistent.
-	
 	def __init__(self, value: Any, a_slice: slice):
 		self.value, self._slice = value, a_slice
 	
 	def __str__(self):
 		return "<Literal %r>" % self.value
 	
 	def head(self) -> slice:
@@ -317,130 +338,106 @@
 def truth(a_slice:slice): return Literal(True, a_slice)
 def falsehood(a_slice:slice): return Literal(False, a_slice)
 
 class Lookup(ValExpr):
 	# Reminder: This AST node exists in opposition to TypeCall so I can write
 	# behavior for references in value context vs. references in type context.
 	ref:Reference
-	is_volatile = False
 	def __init__(self, ref: Reference): self.ref = ref
 	def head(self) -> slice: return self.ref.head()
 	def __str__(self): return str(self.ref)
 
-def is_self_reference(it):
-	if isinstance(it, Lookup):
-		if isinstance(it.ref, PlainReference):
-			return it.ref.nom.text == "SELF"
-	return False
-
 class FieldReference(ValExpr):
 	def __init__(self, lhs: ValExpr, field_name: Nom):
 		self.lhs, self.field_name = lhs, field_name
-		self.is_volatile = lhs.is_volatile or is_self_reference(lhs)
 	def __str__(self): return "(%s.%s)" % (self.lhs, self.field_name.text)
 	def head(self) -> slice: return self.field_name.head()
 
 class BindMethod(ValExpr):
 	def __init__(self, receiver: ValExpr, _bang:Nom, method_name: Nom):
 		self.receiver, self.method_name = receiver, method_name
 		self._head = _bang.head()
-		self.is_volatile = receiver.is_volatile
 	def __str__(self): return "(%s.%s)" % (self.receiver, self.method_name.text)
 	def head(self) -> slice: return self._head
 
 class AsTask(ValExpr):
-	is_volatile = False
-	def __init__(self, head:slice, sub:ValExpr):
+	def __init__(self, head:Nom, proc_ref:ValExpr):
 		self._head = head
-		self.sub = sub
-	def head(self) -> slice: return self._head
+		self.proc_ref = proc_ref
+	def head(self) -> slice: return self._head.head()
 
 class Skip(ValExpr):
-	is_volatile = False
-	def __init__(self, head: slice): self._head = head
-	def head(self) -> slice: return self._head
+	def __init__(self, head: Nom): self._head = head
+	def head(self) -> slice: return self._head.head()
 
 class Binary(ValExpr):
 	def __init__(self, lhs: ValExpr, op:Nom, rhs: ValExpr):
 		self.lhs, self.op, self.rhs = lhs, op, rhs
-		self.is_volatile = self.lhs.is_volatile or self.rhs.is_volatile
 	def head(self) -> slice: return self.op.head()
 
 class BinExp(Binary): pass
 class ShortCutExp(Binary): pass
 
 class UnaryExp(ValExpr):
 	def __init__(self, op:Nom, arg: ValExpr):
 		self.op, self.arg = op, arg
-		self.is_volatile = arg.is_volatile
 
 	def head(self) -> slice: return self.op.head()
 
 class Cond(ValExpr):
 	_kw: slice
 	def __init__(self, then_part: ValExpr, _kw, if_part: ValExpr, else_part: ValExpr):
 		self._kw = _kw
 		self.then_part, self.if_part, self.else_part = then_part, if_part, else_part
-		self.is_volatile = any(x.is_volatile for x in (then_part, if_part, else_part))
 	def head(self) -> slice:
 		return self._kw
 
 def CaseWhen(when_parts: list, else_part: ValExpr):
 	for _kw, test, then in reversed(when_parts):
 		else_part = Cond(then, _kw, test, else_part)
 	return else_part
 
 class Call(ValExpr):
 	def __init__(self, fn_exp: ValExpr, args: list[ValExpr]):
 		self.fn_exp, self.args = fn_exp, args
-		self.is_volatile = self.fn_exp.is_volatile or any(a.is_volatile for a in args)
 	
 	def __str__(self):
 		return "%s(%s)" % (self.fn_exp, ', '.join(map(str, self.args)))
 	
 	def head(self) -> slice: return self.fn_exp.head()
 
 def call_upon_list(fn_exp: ValExpr, list_arg: ValExpr):
 	return Call(fn_exp, [list_arg])
 
 class ExplicitList(ValExpr):
 	def __init__(self, elts: list[ValExpr]):
 		for e in elts:
 			assert isinstance(e, ValExpr), e
 		self.elts = elts
-		self.is_volatile = any(e.is_volatile for e in elts)
 		
 	def head(self) -> slice:
 		return slice(self.elts[0].head().start, self.elts[-1].head().stop)
 
 class Alternative:
 	pattern: Nom
 	dfn: SubTypeSpec  # Either the match-check pass or the type-checker fills this.
 	sub_expr: ValExpr
-	where: Sequence[UserFunction]
+	where: Sequence[Subroutine]
 	
 	namespace: NS  # WordDefiner fills
 
 	def __init__(self, pattern:Nom, _head:Nom, sub_expr:ValExpr, where:Optional[WhereClause]):
 		self.pattern = pattern
 		self._head = _head
 		self.sub_expr = sub_expr
-		if where:
-			_bookend(pattern, where.coda)
-			self.where = where.sub_fns
-		else:
-			self.where = ()
+		self.where = _bookend(pattern, where)
 	def head(self) -> slice:
 		return self._head.head()
 	
-	def has_volatility(self):
-		return self.sub_expr.is_volatile or any(f.has_volatility() for f in self.where)
-
 class Absurdity(ValExpr):
-	is_volatile = False
 	def __init__(self, head:Nom, reason:Optional[Literal]):
 		self._head = head
 		self.reason = reason
 	def head(self) -> slice:
 		it = self._head.head()
 		if self.reason:
 			return slice(it.start, self.reason.head().stop)
@@ -480,15 +477,14 @@
 	variant:Variant  # Match-Check fills these two.
 	dispatch: dict[Symbol:Alternative] # It is now part of the WordResolver pass.
 	
 	def __init__(self, subject, hint, alternatives, otherwise):
 		self.subject = subject
 		self.hint = hint
 		self.alternatives, self.otherwise = alternatives, otherwise
-		self.is_volatile = subject.expr.is_volatile or any(a.has_volatility() for a in alternatives) or (otherwise and otherwise.is_volatile)
 	
 	def head(self) -> slice:
 		return self.subject.head()
 
 class NewAgent(Term):
 	def __init__(self, nom:Nom, expr:ValExpr):
 		super().__init__(nom)
@@ -496,40 +492,37 @@
 
 class DoBlock(ValExpr):
 	namespace: NS  # WordDefiner fills
 	
 	# The value of a do-block does not depend on when it runs.
 	# Its consequence may so depend, but by definition steps run in sequence.
 
-	is_volatile = False
-
 	def __init__(self, agents:list[NewAgent], _head:Nom, steps:list[ValExpr]):
 		self.agents = agents
 		self.steps = steps
 		self._head = _head
 		
 	def head(self) -> slice:
 		return self._head.head()
 
-class AssignField(Reference):
+class AssignMember(Reference):
 	def __init__(self, nom:Nom, expr:ValExpr):
 		super().__init__(nom)
 		self.expr = expr
 	def head(self) -> slice:
 		return self.nom.head()
 
 class LambdaForm(ValExpr):
 	# This is essentially a special kind of literal constant.
 	# It happens to be connected to a function definition.
 	def __init__(self, left, params:list[FormalParameter], body:ValExpr, right):
 		assert params
 		self._slice = slice(left.head().start, right.head().stop)
 		nom = Nom(_gensym(), self._slice)
 		self.function = UserFunction(nom, params, None, body, None)
-		self.is_volatile = self.function.has_volatility()
 		
 	def head(self):
 		return self._slice
 
 class ImportSymbol(NamedTuple):
 	yonder : Nom
 	hither : Optional[Nom]
@@ -579,35 +572,39 @@
 
 ImportDirective = Union[ImportModule, ImportForeign]
 
 class Module:
 	imports: list[ImportModule]
 	foreign: list[ImportForeign]
 	assumptions: list[Assumption]
-	outer_functions: list[UserFunction]
+	top_subs: list[Subroutine]
 	agent_definitions: list[UserAgent]
 	user_operators: list[UserOperator]
 	
 	source_path: Path  # Module loader fills this.
-	all_functions: list[UserFunction]  # WordDefiner pass fills this.
+	all_fns: list[UserFunction]  # WordDefiner pass fills this.
+	all_procs: list[UserProcedure]  # WordDefiner pass fills this.
 	ffi_operators: list[FFI_Operator]  # WordDefiner fills this too.
+	
+	performative : list[bool]  # Type checker fills this in so compiler emits correctly.
 
-	def __init__(self, exports:list, imports:list[ImportDirective], types:list[TypeDeclaration], assumptions:list[Assumption], top_levels:list, main:list):
+	def __init__(self, exports:list, imports:list[ImportDirective], types:list[TypeDeclaration], assumptions:list[Assumption], top_levels:list, main:list[ValExpr]):
 		self.exports = exports
 		self.imports = [i for i in imports if isinstance(i, ImportModule)]
 		self.foreign = [i for i in imports if isinstance(i, ImportForeign)]
 		self.types = types
 		self.assumptions = assumptions
-		self.outer_functions = []
+		self.top_subs = []
 		self.agent_definitions = []
 		self.user_operators = []
-		self.all_functions = []
+		self.all_fns = []
+		self.all_procs = []
 		self.ffi_operators = []
 		for item in top_levels:
 			if isinstance(item, UserOperator): self.user_operators.append(item)
-			if isinstance(item, UserFunction): self.outer_functions.append(item)
+			if isinstance(item, Subroutine): self.top_subs.append(item)
 			elif isinstance(item, UserAgent): self.agent_definitions.append(item)
 			else: assert False, type(item)
 		self.main = main
 	
 	@staticmethod
 	def head(): return slice(0,0)
```

### Comparing `sophie-lang-0.0.6/sophie/sys/complex.sg` & `sophie-lang-0.0.7/sophie/sys/complex.sg`

 * *Files identical despite different names*

### Comparing `sophie-lang-0.0.6/sophie/sys/preamble.sg` & `sophie-lang-0.0.7/sophie/sys/preamble.sg`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 foreign "sophie.adapters.yarn" where
 	mid : (string, number, number) -> string;
 	val : (string) -> maybe[number];
 	join: (list[string]) -> string;
 	is_match_at: (number, string, string) -> flag;
 	trim, ltrim, rtrim : (string) -> string;
+	split_lines : (string) -> list[string];
 end;
 
 foreign "operator" where
 	strcat@"add" : (string, string) -> string;
 end;
 
 # A few of Python's standard math functions are trouble (currently).
```

### Comparing `sophie-lang-0.0.6/sophie/sys/tree.sg` & `sophie-lang-0.0.7/sophie/sys/tree.sg`

 * *Files identical despite different names*

### Comparing `sophie-lang-0.0.6/sophie/sys/turtle.sg` & `sophie-lang-0.0.7/sophie/sys/turtle.sg`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Bits for Turtle Graphics.
 
 # This moved out of the standard preamble to prove it could be done.
 
 import:
-foreign "sophie.adapters.turtle_adapter"();
+foreign "sophie.adapters.turtle_adapter"(drawing);
 
 type:
 
 	drawing is (steps: list[turtle_step]);
 
 	turtle_step is case:
 		forward(distance:number);
```

### Comparing `sophie-lang-0.0.6/sophie/type_evaluator.py` & `sophie-lang-0.0.7/sophie/type_evaluator.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 from .stacking import RootFrame, Activation
 from .syntax import ValExpr
 from .calculus import (
 	TYPE_ENV,
 	SophieType, TypeVisitor, AdHocType,
 	OpaqueType, ProductType, ArrowType, TypeVariable,
 	RecordType, SumType, SubType, TaggedRecord, EnumType,
-	UDFType, UDAType, InterfaceType, MessageType, UserTaskType,
-	ParametricTemplateType, ConcreteTemplateType, BehaviorType,
-	BOTTOM, ERROR, EMPTY_PRODUCT
+	SubroutineType, UserFnType, UserProcType, UDAType, UserTaskType,
+	InterfaceType, MessageType, ParametricTemplateType, ConcreteTemplateType,
+	BOTTOM, ERROR, EMPTY_PRODUCT, READY_MESSAGE
 )
 
 class DependencyPass(TopDown):
 	"""
 	Solve the problem of which-all formal parameters does the value (and thus, type)
 	of each user-defined function actually depend on. A simplistic answer would be to just
 	use the parameters of the outermost function in a given nest. But inner functions
@@ -60,15 +60,15 @@
 		# All manner of temp data, which should be cleaned afterward:
 		self._outer: dict[Symbol, set[syntax.FormalParameter]] = {}
 		self._parent: dict[Symbol, Symbol] = {}
 		self._outflows: dict[Symbol, set[Symbol]] = {}
 		self._overflowing = set()
 		
 	def visit_Module(self, module: syntax.Module):
-		self._walk_children(module.outer_functions, None)
+		self._walk_children(module.top_subs, None)
 		self._walk_children(module.agent_definitions, None)
 		for expr in module.main:
 			self.visit(expr, None)
 		self._flow_dependencies()
 		self._clean_up_after()
 
 	def _prepare(self, sym:Symbol, parent):
@@ -106,40 +106,37 @@
 		self._parent.clear()
 		self._outflows.clear()
 		self._overflowing.clear()
 
 	def _is_in_scope(self, param:syntax.FormalParameter, env:Symbol):
 		if env is None:
 			return False
-		if isinstance(env, (syntax.UserFunction, syntax.Behavior)):
+		if isinstance(env, syntax.Subroutine):
 			return param in env.params or self._is_in_scope(param, self._parent[env])
 		if isinstance(env, syntax.Subject):
 			return self._is_in_scope(param, self._parent[env])
 		if isinstance(env, syntax.UserAgent):
-			return param in env.fields or self._is_in_scope(param, self._parent[env])
+			assert self._parent[env] is None
+			return param in env.members
 		assert False, (param, env)
 
 	@staticmethod
 	def _is_non_local(param:syntax.FormalParameter, env:Symbol):
-		if isinstance(env, (syntax.UserFunction, syntax.Behavior)):
+		if isinstance(env, syntax.Subroutine):
 			return param not in env.params
 		if isinstance(env, syntax.Subject):
 			return True
 		assert False, type(env)
 
-	def visit_UserFunction(self, udf: syntax.UserFunction, env):
+	def visit_Subroutine(self, sub: syntax.Subroutine, env):
 		# Params refer to themselves in this arrangement.
 		# The "breadcrumb" serves to indicate the nearest enclosing symbol.
-		self._parent[udf] = env
-		self._walk_children(udf.where, udf)
-		self.visit(udf.expr, udf)
-	
-	def visit_Behavior(self, b:syntax.Behavior, env:syntax.UserAgent):
-		self._parent[b] = env
-		self.visit(b.expr, b)
+		self._parent[sub] = env
+		self._walk_children(sub.where, sub)
+		self.visit(sub.expr, sub)
 	
 	def visit_UserAgent(self, uda:syntax.UserAgent, env):
 		assert env is None
 		self._walk_children(uda.behaviors, uda)
 
 	def visit_Lookup(self, lu: syntax.Lookup, env):
 		self.visit(lu.ref, env)
@@ -156,36 +153,50 @@
 	def visit_PlainReference(self, ref: syntax.PlainReference, env:Symbol):
 		dfn = ref.dfn
 		if isinstance(dfn, syntax.FormalParameter):
 			self._insert(dfn, env)
 		elif self._is_relevant(dfn):
 			self._outflows[dfn].add(env)
 	
-	def visit_AssignField(self, af:syntax.AssignField, env:Symbol):
-		dfn = af.dfn
+	def visit_MemberReference(self, mr:syntax.MemberReference, env:Symbol):
+		dfn = mr.dfn
 		assert isinstance(dfn, syntax.FormalParameter)
 		self._insert(dfn, env)
-		self.visit(af.expr, env)
+	
+	def visit_AssignMember(self, am:syntax.AssignMember, env:Symbol):
+		dfn = am.dfn
+		assert isinstance(dfn, syntax.FormalParameter)
+		self._insert(dfn, env)
+		self.visit(am.expr, env)
 	
 	def visit_QualifiedReference(self, ref:syntax.QualifiedReference, env:Symbol):
 		pass
 
+	def visit_SelfReference(self, ref:syntax.SelfReference, env:Symbol):
+		"""
+		The SELF type need not participate here. Calling-conventions notwithstanding,
+		it's not a formal parameter for this purpose. Rather, SELF is completely
+		described by its agent-class and the types of the agent parameters.
+		These are already in the lexical scope, and they do the right things.
+		"""
+		pass
+
 	def visit_MatchExpr(self, mx: syntax.MatchExpr, env:Symbol):
 		self._prepare(mx.subject, env)
 		self._outflows[mx.subject].add(env)
 		self.visit(mx.subject.expr, env)
 		for alt in mx.alternatives:
 			self._walk_children(alt.where, mx.subject)
 			self.visit(alt.sub_expr, mx.subject)
 		if mx.otherwise is not None:
 			self.visit(mx.otherwise, mx.subject)
 
 	def visit_DoBlock(self, db: syntax.DoBlock, env:Symbol):
 		for new_agent in db.agents:
-			self._parent[new_agent] = env
+			self._prepare(new_agent, env)
 			self.visit(new_agent.expr, env)
 		for s in db.steps:
 			self.visit(s, env)
 
 
 class ArityError(Exception):
 	pass
@@ -257,27 +268,29 @@
 	def visit_ExplicitTypeVariable(self, tv:syntax.ExplicitTypeVariable):
 		return self._bind(tv.dfn)
 	
 	def visit_ArrowSpec(self, spec:syntax.ArrowSpec):
 		return ArrowType(self._make_product(spec.lhs), self.visit(spec.rhs))
 	
 	def visit_MessageSpec(self, ms:syntax.MessageSpec) -> SophieType:
-		if ms.type_exprs:
-			product = self._make_product(ms.type_exprs)
-			return MessageType(product).exemplar()
-		else:
-			return primitive.literal_msg
+		product = self._make_product(ms.type_exprs)
+		return MessageType(product).exemplar()
 		
 	def make_agent_template(self, uda:syntax.UserAgent, module_scope:TYPE_ENV):
-		if uda.fields:
-			product = self._make_product(field.type_expr for field in uda.fields)
+		if uda.members:
+			product = self._make_product(field.type_expr for field in uda.members)
 			return ParametricTemplateType(uda, product, module_scope)
 		else:
 			# In this case, we have a (stateless) template ready to go.
 			return ConcreteTemplateType(uda, EMPTY_PRODUCT, module_scope)
+	
+	@staticmethod
+	def visit_NoneType(_:None):
+		""" An ugly hack, but it gets progress made. """
+		return BOTTOM
 
 class Rewriter(TypeVisitor):
 	def __init__(self, gamma:dict):
 		self._gamma = gamma
 	def on_opaque(self, o: OpaqueType):
 		return o
 	def on_tag_record(self, t: TaggedRecord):
@@ -328,25 +341,35 @@
 	
 	def complain(self, report:diagnostics.Report):
 		report.bad_type(self._dynamic_link, *self._task, self.why)
 				
 	def bind(self, formal: SophieType, actual: SophieType):
 		if actual in TRIVIAL_TYPES or formal in TRIVIAL_TYPES or formal.number == actual.number:
 			return
+		if isinstance(actual, TypeVariable):
+			# This should not be possible during concrete type-checking -- for now.
+			# It can only happen during signature-checking when you've done something
+			# particularly informative with type annotations and higher-order functions.
+			# Because Sophie types are not (currently) part of a covariance hierarchy,
+			# we can just treat this as backwards type-equality, which is symmetric.
+			#
+			# Signature-checking is allowed to say "maybe", because the concrete
+			# check with *actual* actual types will catch any leftovers. Probably.
+			# (There might be corner-cases involving generic data constructors.)
+			self.visit_TypeVariable(actual, formal)
 		else:
 			self.visit(formal, actual)
 	
 	def visit_TypeVariable(self, formal: TypeVariable, actual: SophieType):
 		if formal in self.gamma:
 			union_finder = UnionFinder()
 			result = union_finder.do(self.gamma[formal], actual)
 			if result is ERROR:
 				self.fail("Unable to unify %s with %s"%(self.gamma[formal], actual))
-			else:
-				self.gamma[formal] = result
+			self.gamma[formal] = result
 		else:
 			self.gamma[formal] = actual
 	
 	def parallel(self, formal: Sequence[SophieType], actual: Sequence[SophieType]):
 		assert len(formal) == len(actual)
 		for f, a in zip(formal, actual): self.bind(f, a)
 	
@@ -366,15 +389,15 @@
 			self.gamma = dict(save_gamma)  # Generally fairly small, so asymptotic is NBD here.
 			self.bind(actual.arg, formal.arg)
 			# The actual-result could contain type-variables from the formal side,
 			# and these must be suitable as what the formal-result dictates.
 			result = actual.res.visit(Rewriter(self.gamma))
 			self.gamma = save_gamma
 			self.bind(formal.res, result)
-		elif isinstance(actual, UDFType):
+		elif isinstance(actual, UserFnType):
 			if actual.expected_arity() != len(formal.arg.fields):
 				self.fail("Arity mismatch between formal function and user-defined function.")
 			else:
 				result = self._engine.apply_UDF(actual, formal.arg.fields, self._dynamic_link)
 				self.bind(formal.res, result)
 		else:
 			self.fail("Using a %s where some sort of function is needed."%actual)
@@ -408,35 +431,30 @@
 			self.fail("Record %s is not %s"%(formal, actual))
 	
 	def visit_MessageType(self, formal: MessageType, actual: SophieType):
 		if isinstance(actual, MessageType):
 			return self.visit(formal.arg, actual.arg)
 		elif isinstance(actual, UserTaskType):
 			if actual.expected_arity() == len(formal.arg.fields):
-				result = self._engine.apply_UDF(actual.udf_type, formal.arg.fields, self._dynamic_link)
-				# At this point, either an act or another message will be acceptable.
-				if not _quacks_like_an_action(result):
-					self.fail("%s does not an action make."%result)
-			else:
-				self.fail("%s has different arity from %s"%(formal, actual))
-		elif isinstance(actual, BehaviorType):
-			if actual.expected_arity() == len(formal.arg.fields):
-				result = self._engine.apply_behavior(actual, formal.arg.fields, self._dynamic_link)
+				result = self._engine.apply_procedure(actual.proc_type, formal.arg.fields, self._dynamic_link)
 				# At this point, either an act or another message will be acceptable.
 				if not _quacks_like_an_action(result):
 					self.fail("%s does not an action make."%result)
 			else:
 				self.fail("%s has different arity from %s"%(formal, actual))
 		else:
 			self.fail("Not sure how to use a %s as a %s"%(actual, formal))
 
-def _quacks_like_an_action(result:SophieType) -> bool:
-	assert isinstance(result, SophieType), result
+def _quacks_like_an_action(typ:SophieType) -> bool:
+	assert isinstance(typ, SophieType), typ
+	if isinstance(typ, UserProcType): return not typ.sub.params
+	if isinstance(typ, UserTaskType): return not typ.proc_type.sub.params
+	if isinstance(typ, MessageType): return not typ.arg.fields
 	# Let ERROR quack to stop cascades of messages.
-	return result in (primitive.literal_act, primitive.literal_msg, ERROR)
+	return typ in (primitive.literal_act, ERROR)
 
 class UnionFinder(Visitor):
 	def __init__(self):
 		self._prototype = BOTTOM
 		self._expr = None
 	
 	def result(self):
@@ -455,14 +473,16 @@
 	def parallel(self, these:Sequence[SophieType], those:Sequence[SophieType]):
 		assert len(these) == len(those)
 		return [self.do(a, b) for a,b in zip(these, those)]
 	
 	def do(self, this: SophieType, that: SophieType):
 		if this.number == that.number or that is BOTTOM: return this
 		elif that is ERROR: return that
+		elif _quacks_like_an_action(this) and _quacks_like_an_action(that):
+			return primitive.literal_act
 		else:
 			typ = self.visit(this, that)
 			if typ is None:
 				return ERROR
 			else:
 				return typ
 
@@ -511,17 +531,17 @@
 		elif isinstance(that, TaggedRecord):
 			return self.visit_TaggedRecord(that, this)
 		elif isinstance(that, EnumType):
 			if this.st.variant is that.st.variant:
 				type_args = tuple(BOTTOM for _ in this.st.variant.type_params)
 				return SumType(this.st.variant, type_args)
 
-	def visit_UDFType(self, this:UDFType, that: SophieType):
-		if isinstance(that, UDFType):
-			if len(this.fn.params) == len(that.fn.params):
+	def visit_UDFType(self, this:UserFnType, that: SophieType):
+		if isinstance(that, UserFnType):
+			if len(this.sub.params) == len(that.sub.params):
 				# In principle, we take the intersection of the parameters to the union of the results.
 				# In practice, that means some sort of "try both" logic,
 				# and it's entirely too complicated for a five-minute hack session.
 				raise NotImplementedError("To do.")
 			else:
 				return None  # Non-matching arity is a definite error.
 		elif isinstance(that, ArrowType):
@@ -545,32 +565,31 @@
 	this has a relatively small API compared to the full decision engine.
 	"""
 	
 	def __init__(self, types:dict[Symbol,SophieType], report:diagnostics.Report):
 		self._types = types
 		self._report = report
 	
-	def apply_UDF(self, fn_type: UDFType, arg_types: Sequence[SophieType], env:TYPE_ENV) -> SophieType:
-		udf = fn_type.fn
+	def _apply_subroutine(self, subroutine_type: SubroutineType, arg_types: Sequence[SophieType], env:TYPE_ENV) -> SophieType:
+		symbol = subroutine_type.sub
 		binder = Binder(self, env)
-		for param, actual in zip(udf.params, arg_types):
+		for param, actual in zip(symbol.params, arg_types):
 			if param in self._types:
 				binder.bind(self._types[param], actual)
 				if not binder.ok:
-					self._report.bad_argument(env, udf, param, actual, binder.why)
+					self._report.bad_argument(env, symbol, param, actual, binder.why)
 					return ERROR
-		if udf in self._types:
-			return self._types[udf].visit(Rewriter(binder.gamma))
+		if symbol in self._types:
+			return self._types[symbol].visit(Rewriter(binder.gamma))
 		else:
 			return BOTTOM
 	
-	def apply_behavior(self, bt:BehaviorType, arg_types: Sequence[SophieType], env:TYPE_ENV) -> SophieType:
-		raise NotImplementedError("To do.")
-
-
+	apply_UDF = _apply_subroutine
+	apply_procedure = _apply_subroutine
+	
 class DeductionEngine(Visitor):
 	_types: dict[Symbol, SophieType]
 	
 	def __init__(self, roadmap:RoadMap, report:diagnostics.Report):
 		# self._trace_depth = 0
 		self._report = report  # .on_error("Checking Types")
 		self._types = {}
@@ -588,15 +607,15 @@
 		self._root = RootFrame()
 		self.visit_Module(roadmap.preamble)
 		for module in roadmap.each_module:
 			self.visit_Module(module)
 	
 	def _init_types(self):
 		
-		for ot in [primitive.literal_act, *_literal_type_map.values()]:
+		for ot in _literal_type_map.values():
 			self._types[ot.symbol] = ot
 		
 		def relop_type(src):
 			return _binop_type(src, primitive.literal_flag)
 		
 		math_op = _arrow_of(primitive.literal_number, 2)
 		
@@ -650,34 +669,44 @@
 			elif arity == 2: dispatch = self._binary_types
 			else:
 				self._report.bogus_operator_arity(udf)
 				continue
 			op_key = udf.nom.key()
 			try: adhoc = dispatch[op_key]
 			except KeyError: self._report.bogus_operator_arity(udf)
-			else: adhoc.append_case(UDFType(udf, local), self._report)
+			else: adhoc.append_case(UserFnType(udf, local), self._report)
 		for sym in module.ffi_operators:
-			pass
+			raise NotImplementedError("Hadn't been needed yet.", sym)
 	
 	def build_all_manifests(self, module, local):
-		builder = ManifestBuilder([], [])
-		for udf in module.all_functions:
-			for fp in udf.params:
+		def install_params(sub:syntax.Subroutine):
+			for fp in sub.params:
 				if fp.type_expr:
 					self._types[fp] = builder.visit(fp.type_expr)
+		builder = ManifestBuilder([], [])
+		for udf in module.all_fns:
+			install_params(udf)
 			if udf.result_type_expr:
 				self._types[udf] = builder.visit(udf.result_type_expr)
+		for udp in module.all_procs:
+			install_params(udp)
 		for uda in module.agent_definitions:
 			self._constructors[uda] = builder.make_agent_template(uda, local)
 	
+	def _trace_visit(self, expr, local):
+		self._report.trace(" -->", expr)
+		result = self.visit(expr, local)
+		self._report.info(result)
+		return result
+	
 	def visit_begin_block(self, module, local):
-		for expr in module.main:
-			self._report.trace(" -->", expr)
-			result = self.visit(expr, local)
-			self._report.info(result)
+		module.performative = [
+			_quacks_like_an_action(self._trace_visit(expr, local))
+			for expr in module.main
+		]
 
 	###############################################################################
 
 	def visit_Record(self, r: syntax.Record):
 		type_args = [TypeVariable() for _ in r.type_params]
 		self._types[r] = RecordType(r, type_args)
 		arg = ManifestBuilder(r.type_params, type_args).visit(r.spec)
@@ -726,98 +755,108 @@
 
 	###############################################################################
 
 	@staticmethod
 	def visit_Literal(expr: syntax.Literal, _env:TYPE_ENV) -> SophieType:
 		return _literal_type_map[type(expr.value)]
 	
-	def apply_UDF(self, fn_type: UDFType, arg_types: Sequence[SophieType], env:TYPE_ENV) -> SophieType:
-		udf = fn_type.fn
-		
+	def apply_UDF(self, fn_type: UserFnType, arg_types: Sequence[SophieType], env:TYPE_ENV) -> SophieType:
 		# Sanity-check the argument-types against any manifest-type expressions
 		checker = ManifestEngine(self._types, self._report)
 		expect = checker.apply_UDF(fn_type, arg_types, env)
 		if expect is ERROR: return ERROR
 		
+		udf = fn_type.sub
+		
 		# Evaluate the body-expression to determine the actual result-type
-		inner = Activation.for_function(fn_type.static_link, env, fn_type.fn, arg_types)
+		inner = Activation.for_subroutine(fn_type.static_link, env, udf, arg_types)
 		result_type = self.exec_UDF(udf, inner)
 		if result_type is ERROR: return ERROR
 		
 		# Sanity-check the result-type against its manifest-type.
 		if expect is not BOTTOM:
 			binder = Binder(checker, inner)
 			binder.bind(expect, result_type)
 			if not binder.ok:
 				self._report.bad_result(inner, udf, result_type, binder.why)
 				return ERROR
 		
+		if result_type == primitive.literal_act:
+			self._report.must_not_express_behavior(env, fn_type.sub)
+		
 		# If all went well:
 		return result_type
 	
-	def apply_behavior(self, bt:BehaviorType, arg_types: Sequence[SophieType], env:TYPE_ENV) -> SophieType:
-		env = Activation.for_behavior(bt.uda_type.frame, env, bt.behavior, arg_types)
-		memo_key = self._memo_key(bt.behavior, env)
+	def apply_procedure(self, proc_type:UserProcType, arg_types: Sequence[SophieType], env:TYPE_ENV) -> SophieType:
+		# TODO: There's probably a lot more that could be shared with apply_UDF.
+		# Sanity-check the argument-types against any manifest-type expressions
+		checker = ManifestEngine(self._types, self._report)
+		expect = checker.apply_procedure(proc_type, arg_types, env)
+		if expect is ERROR: return ERROR
+		
+		procedure = proc_type.sub
+		frame = Activation.for_subroutine(proc_type.static_link, env, procedure, arg_types)
+		memo_key = self._memo_key(procedure, frame)
 		if memo_key in self._memo:
 			return self._memo[memo_key]
 		elif memo_key in self._recursion:
-			return primitive.literal_msg
+			return primitive.literal_act
 		else:
 			self._recursion[memo_key] = False
-			got = self._memo[memo_key] = self.visit(bt.behavior.expr, env)
+			got = self._memo[memo_key] = self.visit(procedure.expr, frame)
 			self._recursion.pop(memo_key)
 			if _quacks_like_an_action(got):
 				return primitive.literal_act
 			else:
-				self._report.does_not_express_behavior(env, bt.behavior, got)
+				self._report.does_not_express_behavior(frame, procedure, got)
 				return ERROR
 	
 	def _memo_key(self, symbol:Symbol, env:TYPE_ENV):
 		# This definitely works for functions.
 		# Things are a bit more sketchy on the behavior side.
 		memo_symbols = self._deps_pass.depends[symbol]
 		assert all(isinstance(s, syntax.FormalParameter) for s in memo_symbols)
 		memo_types = tuple(
 			env.chase(p).fetch(p)  # .number
 			for p in memo_symbols
 		)
 		return symbol, memo_types
 	
-	def exec_UDF(self, fn:syntax.UserFunction, env:TYPE_ENV):
+	def exec_UDF(self, sub:syntax.Subroutine, env:TYPE_ENV):
 		# The part where memoization must happen.
-		memo_key = self._memo_key(fn, env)
+		memo_key = self._memo_key(sub, env)
 		if memo_key in self._memo:
 			return self._memo[memo_key]
 		elif memo_key in self._recursion:
 			self._recursion[memo_key] = True
 			# self._report.trace(">Recursive:", fn, dict(zip((s.nom.text for s in memo_symbols), memo_types)))
 			return BOTTOM
 		else:
 			# TODO: Pass around judgements, not just types.
 			self._recursion[memo_key] = False
-			self._memo[memo_key] = self.visit(fn.expr, env)
+			self._memo[memo_key] = self.visit(sub.expr, env)
 			if self._recursion.pop(memo_key):
 				prior = BOTTOM
 				while prior != self._memo[memo_key]:
 					prior = self._memo[memo_key]
-					self._memo[memo_key] = self.visit(fn.expr, env)
+					self._memo[memo_key] = self.visit(sub.expr, env)
 				if prior is BOTTOM:
-					self._report.ill_founded_function(env, fn)
+					self._report.ill_founded_function(env, sub)
 				# self._report.trace("<Resolved:", fn)
 					
 		return self._memo[memo_key]
 	
 	def _call_site(self, site: syntax.ValExpr, callee_type, args:Sequence[ValExpr], env:TYPE_ENV) -> SophieType:
 		actual_types = [self.visit(a, env) for a in args]
 		if ERROR in actual_types:
 			return ERROR
 		
 		env.pc = site
 		if callee_type.expected_arity() != len(args):
-			self._report.wrong_arity(env, site, callee_type.expected_arity(), args)
+			self._report.wrong_arity(env, site, callee_type, args)
 			return ERROR
 		
 		if isinstance(callee_type, AdHocType):
 			return self._call_dynamic(callee_type, actual_types, args, env)
 		else:
 			return self._call_static(callee_type, actual_types, args, env)
 		
@@ -846,27 +885,44 @@
 			binder = Binder(self, env).inputs(callee_type.arg.fields, actual_types, args)
 			if binder.ok:
 				return callee_type.res.visit(Rewriter(binder.gamma))
 			else:
 				binder.complain(self._report)
 				return ERROR
 		
-		elif isinstance(callee_type, UDFType):
+		elif isinstance(callee_type, MessageType):
+			binder = Binder(self, env).inputs(callee_type.arg.fields, actual_types, args)
+			if binder.ok:
+				return READY_MESSAGE
+			else:
+				binder.complain(self._report)
+				return ERROR
+		
+		elif isinstance(callee_type, UserFnType):
 			return self.apply_UDF(callee_type, actual_types, env)
 		
+		elif isinstance(callee_type, UserProcType):
+			return self.apply_procedure(callee_type, actual_types, env)
+		
+		elif isinstance(callee_type, UserTaskType):
+			pt = self.apply_procedure(callee_type.proc_type, actual_types, env)
+			if pt is ERROR: return ERROR
+			else: return READY_MESSAGE
+		
 		elif isinstance(callee_type, ParametricTemplateType):
-			binder = Binder(self, env).inputs(callee_type.args.fields, actual_types, args)
+			binder = Binder(self, env).inputs(callee_type.args, actual_types, args)
 			if binder.ok:
-				return ConcreteTemplateType(callee_type.uda, ProductType(actual_types), callee_type.frame)
+				return ConcreteTemplateType(callee_type.uda, ProductType(actual_types), callee_type.global_env)
 			else:
 				binder.complain(self._report)
 				return ERROR
 		
 		else:
-			raise NotImplementedError(type(callee_type))
+			self._report.drat(env, type(callee_type))
+			return ERROR
 	
 	def visit_Call(self, site: syntax.Call, env: TYPE_ENV) -> SophieType:
 		fn_type = self.visit(site.fn_exp, env)
 		if fn_type is ERROR: return ERROR
 		return self._call_site(site, fn_type, site.args, env)
 	
 	def visit_BinExp(self, expr:syntax.BinExp, env:TYPE_ENV) -> SophieType:
@@ -884,27 +940,31 @@
 			return self._constructors[target]  # Must succeed because of resolution.check_constructors
 		if isinstance(target, syntax.FFI_Alias):
 			return self._ffi[target]
 		
 		static_env = env.chase(target)
 		if isinstance(target, syntax.UserFunction):
 			if target.params:
-				return UDFType(target, static_env).exemplar()
+				return UserFnType(target, static_env).exemplar()
 			else:
-				inner = Activation.for_function(static_env, env, target, ())
+				inner = Activation.for_subroutine(static_env, env, target, ())
 				return self.exec_UDF(target, inner)
+		elif isinstance(target, syntax.UserProcedure):
+			# The concept here is not to call procedures upon mention,
+			# but only when they're expressly called or used as a step.
+			return UserProcType(target, static_env).exemplar()
 		else:
 			assert target is SELF or isinstance(target, (syntax.FormalParameter, syntax.Subject, syntax.NewAgent)), type(target)
 			return static_env.fetch(target)
 	
 	@staticmethod
 	def visit_LambdaForm(lf:syntax.LambdaForm, env:TYPE_ENV) -> SophieType:
 		# No need to chase to find a static environment:
 		# It's taken from the point-of-use by definition.
-		return UDFType(lf.function, env).exemplar()
+		return UserFnType(lf.function, env).exemplar()
 		
 	@staticmethod
 	def visit_Absurdity(_:syntax.Absurdity, _env:TYPE_ENV) -> SophieType:
 		return BOTTOM
 	
 	def visit_ExplicitList(self, el:syntax.ExplicitList, env:TYPE_ENV) -> SumType:
 		# Since there's guaranteed to be at least one value,
@@ -927,23 +987,21 @@
 		uf.unify_with(env, cond.then_part, self.visit(cond.then_part, env), self._report)
 		uf.unify_with(env, cond.else_part, self.visit(cond.else_part, env), self._report)
 		return uf.result()
 	
 	def visit_MatchExpr(self, mx:syntax.MatchExpr, env:TYPE_ENV) -> SophieType:
 		
 		def try_one_alternative(alt, subtype:SubType) -> SophieType:
-			inner = Activation.for_subject(env, mx.subject)
-			inner.assign(mx.subject, subtype)
+			inner = Activation.for_subject(env, mx.subject, subtype)
 			for sub in alt.where:
 				inner.declare(sub)
 			return self.visit(alt.sub_expr, inner)
 		
 		def try_otherwise():
-			inner = Activation.for_subject(env, mx.subject)
-			inner.assign(mx.subject, subject_type)
+			inner = Activation.for_subject(env, mx.subject, subject_type)
 			return self.visit(mx.otherwise, inner)
 		
 		def try_everything(type_args:Sequence[SophieType]):
 			uf = UnionFinder()
 			for alt in mx.alternatives:
 				subtype = _hypothesis(alt.dfn, type_args).exemplar()
 				case_result = try_one_alternative(alt, subtype)
@@ -951,14 +1009,15 @@
 					return ERROR
 			if mx.otherwise is not None:
 				if not uf.unify_with(env, mx.otherwise, try_otherwise(), self._report):
 					return ERROR
 			return uf.result()
 
 		subject_type = self.visit(mx.subject.expr, env)
+		env.pc = None
 		if subject_type is ERROR:
 			return ERROR
 
 		if isinstance(subject_type, SumType):
 			return try_everything(subject_type.type_args)
 		
 		elif subject_type is BOTTOM:
@@ -971,36 +1030,38 @@
 			else:
 				return try_otherwise()
 		
 		else:
 			self._report.bad_type(env, mx.subject.expr, mx.variant, subject_type, "Square Peg; Round Hole.")
 			return ERROR
 
-	def visit_AssignField(self, af:syntax.AssignField, env:TYPE_ENV) -> SophieType:
-		field_type = env.chase(af.dfn).fetch(af.dfn)
-		expr_type = self.visit(af.expr, env)
+	def visit_AssignMember(self, am:syntax.AssignMember, env:TYPE_ENV) -> SophieType:
+		field_scope = env.chase(am.dfn)
+		field_type = field_scope.fetch(am.dfn)
+		expr_type = self.visit(am.expr, env)
+		
 		if expr_type == field_type or expr_type is ERROR:
 			return primitive.literal_act
 		else:
-			self._report.bad_type(env, af.expr, field_type, expr_type, "Assignment must match field type exactly.")
-			return ERROR
+			uf = UnionFinder()
+			uf.unify_with(env, am.dfn, field_type, self._report)
+			uf.unify_with(env, am.expr, expr_type, self._report)
+			union = uf.result()
+			if union is ERROR:
+				self._report.bad_type(env, am.expr, field_type, expr_type, "Assignment must match field type exactly.")
+				return ERROR
+			else:
+				field_scope.assign(am.dfn, union)
+				return primitive.literal_act
 	
 	def visit_FieldReference(self, fr:syntax.FieldReference, env:TYPE_ENV) -> SophieType:
 		lhs_type = self.visit(fr.lhs, env)
 		if isinstance(lhs_type, UDAType):
-			if _is_a_self_reference(fr.lhs):
-				try: symbol = lhs_type.uda.field_space[fr.field_name.key()]
-				except KeyError:
-					self._report.record_lacks_field(env, fr, lhs_type)
-					return ERROR
-				else:
-					return lhs_type.frame.fetch(symbol)
-			else:
-				self._report.no_telepathy_allowed(env, fr, lhs_type)
-				return ERROR
+			self._report.no_telepathy_allowed(env, fr, lhs_type)
+			return ERROR
 		elif isinstance(lhs_type, RecordType):
 			spec = lhs_type.symbol.spec
 			parameters = lhs_type.symbol.type_params
 		elif isinstance(lhs_type, TaggedRecord):
 			spec = lhs_type.st.body
 			parameters = lhs_type.st.variant.type_params
 		elif lhs_type is BOTTOM:
@@ -1017,102 +1078,93 @@
 		except KeyError:
 			self._report.record_lacks_field(env, fr, lhs_type)
 			return ERROR
 		assert isinstance(field_spec, syntax.FormalParameter), field_spec
 		return ManifestBuilder(parameters, lhs_type.type_args).visit(field_spec.type_expr)
 
 	def visit_BindMethod(self, mr:syntax.BindMethod, env:TYPE_ENV) -> SophieType:
-		lhs_type = self.visit(mr.receiver, env)
-		if lhs_type is ERROR: return ERROR
-		if isinstance(lhs_type, InterfaceType):
+		actor_type = self.visit(mr.receiver, env)
+		if actor_type is ERROR: return ERROR
+		if isinstance(actor_type, InterfaceType):
 			try:
-				ms = lhs_type.symbol.method_space[mr.method_name.key()]
+				ms = actor_type.symbol.method_space[mr.method_name.key()]
 			except KeyError:
-				self._report.bad_message(env, mr, lhs_type)
+				self._report.bad_message(env, mr, actor_type)
 				return ERROR
 			else:
 				assert isinstance(ms, syntax.MethodSpec)
-				parameters = lhs_type.symbol.type_params
-				builder = ManifestBuilder(parameters, lhs_type.type_args)
-				if ms.type_exprs:
-					args = ProductType(builder.visit(tx) for tx in ms.type_exprs)
-					return ArrowType(args, primitive.literal_msg)
-				else:
-					return primitive.literal_act
-		elif isinstance(lhs_type, UDAType):
+				parameters = actor_type.symbol.type_params
+				builder = ManifestBuilder(parameters, actor_type.type_args)
+				args = ProductType(builder.visit(tx) for tx in ms.type_exprs)
+				return MessageType(args)
+		elif isinstance(actor_type, UDAType):
 			try:
-				behavior = lhs_type.uda.message_space[mr.method_name.key()]
+				procedure = actor_type.uda.message_space[mr.method_name.key()]
 			except KeyError:
-				self._report.bad_message(env, mr, lhs_type)
+				self._report.bad_message(env, mr, actor_type)
 				return ERROR
 			else:
-				assert isinstance(behavior, syntax.Behavior)
-				result = BehaviorType(lhs_type, behavior).exemplar()
-				if behavior.params:
-					return result
+				assert isinstance(procedure, syntax.UserProcedure)
+				proc_type = UserProcType(procedure, actor_type.frame)
+				if not proc_type.sub.params:
+					pt = self.apply_procedure(proc_type, (), env)
+					if pt is ERROR: return ERROR
+					else: return READY_MESSAGE
 				else:
-					return self.apply_behavior(result, (), env)
+					return UserTaskType(proc_type).exemplar()
 		else:
-			self._report.bad_message(env, mr, lhs_type)
+			self._report.bad_message(env, mr, actor_type)
 			return ERROR
 	
 	def visit_DoBlock(self, do:syntax.DoBlock, env:TYPE_ENV) -> SophieType:
 		# A bit verbose to pick up all errors, not just the first.
 		answer = primitive.literal_act
 		# 1. Make a scope to contain new-agents:
 		inner = Activation.for_do_block(env)
 		for na in do.agents:
 			assert isinstance(na, syntax.NewAgent)
-			tt = self.visit(na.expr, env)
-			if isinstance(tt, ConcreteTemplateType):
-				frame = Activation(tt.frame, inner, tt.uda)
-				agent_type = UDAType(tt.uda, tt.args, frame)
-				frame.assign(SELF, agent_type)
-				for f, t in zip(tt.uda.fields, tt.args.fields):
-					frame.assign(f, t)
+			template = self.visit(na.expr, inner)
+			if isinstance(template, ConcreteTemplateType):
+				agent_type = UDAType(template, inner)
 			else:
-				self._report.bad_type(env, na.expr, "Agent Template", tt, "Casting call will repeat next Thursday.")
+				if template is not ERROR:
+					self._report.bad_type(env, na.expr, "Agent Template", template, "Casting call will repeat next Thursday.")
 				agent_type = ERROR
 				answer = ERROR
 			inner.assign(na, agent_type)
 		# 2. Judge types of step in the new scope:
 		for step in do.steps:
 			inner.pc = step
 			step_type = self.visit(step, inner)
-			assert isinstance(step_type, SophieType)
+			assert isinstance(step_type, SophieType), step_type
 			if step_type is ERROR: answer = ERROR
 			elif step_type is BOTTOM:
 				if answer is not ERROR:
 					answer = BOTTOM
 			elif not _quacks_like_an_action(step_type):
 				self._report.bad_type(inner, step, primitive.literal_act, step_type, "Only actions can be steps in a process.")
 				answer = ERROR
 		return answer
 
 	@staticmethod
 	def visit_Skip(_s:syntax.Skip, _env:TYPE_ENV) -> SophieType:
 		return primitive.literal_act
 
 	def visit_AsTask(self, at:syntax.AsTask, env:TYPE_ENV) -> SophieType:
-		def is_act(t): return t.number == primitive.literal_act.number
-		inner = self.visit(at.sub, env)
-		if is_act(inner):
-			return primitive.literal_msg
-		elif isinstance(inner, ArrowType) and is_act(inner.res):
-			return MessageType(inner.arg).exemplar()
-		elif isinstance(inner, UDFType):
-			return UserTaskType(inner).exemplar()
-		else:
-			self._report.bad_type(env, at.sub, "procedure", inner, "Concurrent tasks cannot return a value.")
-			return ERROR
+		proc_type = self.visit(at.proc_ref, env)
+		if isinstance(proc_type, UserProcType):
+			return UserTaskType(proc_type).exemplar()
+		if isinstance(proc_type, ArrowType) and proc_type.res == primitive.literal_act:
+			return MessageType(proc_type.arg).exemplar()
+		if proc_type == primitive.literal_act:
+			return READY_MESSAGE
+		self._report.bad_task(env, at.proc_ref, proc_type)
+		return ERROR
 
 def _hypothesis(st:syntax.SubTypeSpec, type_args:Sequence[SophieType]) -> SubType:
 	assert isinstance(st, syntax.SubTypeSpec)
 	body = st.body
 	if body is None:
 		return EnumType(st)
 	if isinstance(body, syntax.RecordSpec):
 		return TaggedRecord(st, type_args)
 
-def _is_a_self_reference(expr:ValExpr) -> bool:
-	return isinstance(expr, syntax.Lookup) and expr.ref.dfn is SELF
-
```

### Comparing `sophie-lang-0.0.6/sophie_lang.egg-info/PKG-INFO` & `sophie-lang-0.0.7/sophie_lang.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sophie-lang
-Version: 0.0.6
+Version: 0.0.7
 Summary: A call-by-need strongly-static-duck-typed language named for French mathematician Sophie Germain
 Home-page: https://github.com/kjosib/sophie
 Author: Ian Kjos
 Author-email: kjosib@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
@@ -87,34 +87,35 @@
 
 There is now a [change log](https://github.com/kjosib/sophie/tree/main/CHANGELOG.md).
 
 Some things are going well:
 
 * A native-code [Virtual-Machine](https://github.com/kjosib/sophie/tree/main/vm) can run Sophie code at a respectable speed.
   It reads a "compiled" form which you can generate with a command-line like `sophie -x your/sophie/program.sg > program.is`.
-  It runs most of the examples just fine, but lags slightly behind on extensions.
 * Sophie has Turtle-graphics! (See [here](https://github.com/kjosib/sophie/blob/main/examples/turtle/turtle.sg) for examples.)
-* Sophie is interactive! See [this guessing game](https://github.com/kjosib/sophie/blob/main/examples/games/guess_the_number.sg) as an example.
+* Sophie is interactive! See [this guessing game](https://github.com/kjosib/sophie/blob/main/examples/games/guess_the_number.sg)
+  or this [Not-Quite-Pong game](https://github.com/kjosib/sophie/blob/main/examples/games/nqp.sg) as examples.
 * The type-checker gives excellent feedback and cannot be fooled.
   Through abstract interpretation it completely rules out *type* errors.
   (Domain errors, such as division by zero, are still possible.)
 * The module system got an upgrade: there is now a notion of a system-package and the beginnings of a standard library.
 * The FFI: Sophie can call Python; Python can call Sophie; and Python can install I/O drivers into Sophie.
   The same FFI directives on the Sophie side interact properly with the native-code VM.
 * Compile-time error display is generally clear and informative.
+* Operator overloading works via double-dispatch. Thus, the standard modules for complex-numbers and 2d vectors
+  both let you use ordinary arithmetic symbols to manipulate their respective data types.
 
 Some things are in progress:
 
 * SDL bindings (via PyGame for now). See for example this [graphical mouse-chaser](https://github.com/kjosib/sophie/blob/main/examples/games/mouse.sg).
-* Operator overloading.
 
-Certain things are not started yet:
+Certain things seem like nice ideas, but may not happen any time soon:
 
-* Variable-Arity Functions. (This may never happen.)
-* Ad-hoc polymorphic multi-methods. (This becomes less interesting once operator overloading gets finished.)
+* Variable-Arity Functions.
+* Ad-hoc polymorphic multi-methods.
 * List comprehension (expressions like `[expr FOR name IN expr]`) are removed from the syntax for now.
 
 ## Why not just use Language X, Y, or Z?
 
 Have you been paying attention?
 
 ## Long-Term Plans
```

### Comparing `sophie-lang-0.0.6/sophie_lang.egg-info/SOURCES.txt` & `sophie-lang-0.0.7/sophie_lang.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 sophie/type_evaluator.py
 sophie/adapters/__init__.py
 sophie/adapters/fs_adapter.py
 sophie/adapters/game_adapter.py
 sophie/adapters/teletype_adapter.py
 sophie/adapters/turtle_adapter.py
 sophie/adapters/yarn.py
+sophie/sys/2d.sg
 sophie/sys/complex.sg
 sophie/sys/game.sg
 sophie/sys/preamble.sg
 sophie/sys/tree.sg
 sophie/sys/turtle.sg
 sophie_lang.egg-info/PKG-INFO
 sophie_lang.egg-info/SOURCES.txt
```

