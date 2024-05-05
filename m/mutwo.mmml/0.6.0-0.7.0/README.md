# Comparing `tmp/mutwo.mmml-0.6.0.tar.gz` & `tmp/mutwo_mmml-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutwo.mmml-0.6.0.tar", last modified: Sat Feb 24 22:03:20 2024, max compression
+gzip compressed data, was "mutwo_mmml-0.7.0.tar", last modified: Sun May  5 13:14:17 2024, max compression
```

## Comparing `mutwo.mmml-0.6.0.tar` & `mutwo_mmml-0.7.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-24 22:03:20.411440 mutwo.mmml-0.6.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    35149 2024-02-24 22:03:10.000000 mutwo.mmml-0.6.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2084 2024-02-24 22:03:20.411440 mutwo.mmml-0.6.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1481 2024-02-24 22:03:10.000000 mutwo.mmml-0.6.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-24 22:03:20.407440 mutwo.mmml-0.6.0/mutwo/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-24 22:03:20.407440 mutwo.mmml-0.6.0/mutwo/mmml_converters/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      943 2024-02-24 22:03:10.000000 mutwo.mmml-0.6.0/mutwo/mmml_converters/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      493 2024-02-24 22:03:10.000000 mutwo.mmml-0.6.0/mutwo/mmml_converters/backends.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4807 2024-02-24 22:03:10.000000 mutwo.mmml-0.6.0/mutwo/mmml_converters/codes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      181 2024-02-24 22:03:10.000000 mutwo.mmml-0.6.0/mutwo/mmml_converters/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8776 2024-02-24 22:03:10.000000 mutwo.mmml-0.6.0/mutwo/mmml_converters/frontends.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-24 22:03:20.407440 mutwo.mmml-0.6.0/mutwo/mmml_utilities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       47 2024-02-24 22:03:10.000000 mutwo.mmml-0.6.0/mutwo/mmml_utilities/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1709 2024-02-24 22:03:10.000000 mutwo.mmml-0.6.0/mutwo/mmml_utilities/codes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      593 2024-02-24 22:03:10.000000 mutwo.mmml-0.6.0/mutwo/mmml_utilities/exceptions.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-24 22:03:20.407440 mutwo.mmml-0.6.0/mutwo/mmml_version/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      142 2024-02-24 22:03:10.000000 mutwo.mmml-0.6.0/mutwo/mmml_version/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-24 22:03:20.407440 mutwo.mmml-0.6.0/mutwo.mmml.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2084 2024-02-24 22:03:20.000000 mutwo.mmml-0.6.0/mutwo.mmml.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      508 2024-02-24 22:03:20.000000 mutwo.mmml-0.6.0/mutwo.mmml.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-24 22:03:20.000000 mutwo.mmml-0.6.0/mutwo.mmml.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      100 2024-02-24 22:03:20.000000 mutwo.mmml-0.6.0/mutwo.mmml.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-02-24 22:03:20.000000 mutwo.mmml-0.6.0/mutwo.mmml.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2024-02-24 22:03:10.000000 mutwo.mmml-0.6.0/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-24 22:03:20.411440 mutwo.mmml-0.6.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1137 2024-02-24 22:03:10.000000 mutwo.mmml-0.6.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-05 13:14:17.209965 mutwo_mmml-0.7.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    35149 2024-05-05 13:14:06.000000 mutwo_mmml-0.7.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5643 2024-05-05 13:14:17.209965 mutwo_mmml-0.7.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5040 2024-05-05 13:14:06.000000 mutwo_mmml-0.7.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-05 13:14:17.205965 mutwo_mmml-0.7.0/mutwo/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-05 13:14:17.205965 mutwo_mmml-0.7.0/mutwo/mmml_converters/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      943 2024-05-05 13:14:06.000000 mutwo_mmml-0.7.0/mutwo/mmml_converters/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      493 2024-05-05 13:14:06.000000 mutwo_mmml-0.7.0/mutwo/mmml_converters/backends.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6156 2024-05-05 13:14:06.000000 mutwo_mmml-0.7.0/mutwo/mmml_converters/codes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      334 2024-05-05 13:14:06.000000 mutwo_mmml-0.7.0/mutwo/mmml_converters/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8124 2024-05-05 13:14:06.000000 mutwo_mmml-0.7.0/mutwo/mmml_converters/frontends.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-05 13:14:17.205965 mutwo_mmml-0.7.0/mutwo/mmml_utilities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       47 2024-05-05 13:14:06.000000 mutwo_mmml-0.7.0/mutwo/mmml_utilities/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1709 2024-05-05 13:14:06.000000 mutwo_mmml-0.7.0/mutwo/mmml_utilities/codes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      593 2024-05-05 13:14:06.000000 mutwo_mmml-0.7.0/mutwo/mmml_utilities/exceptions.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-05 13:14:17.205965 mutwo_mmml-0.7.0/mutwo/mmml_version/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      142 2024-05-05 13:14:06.000000 mutwo_mmml-0.7.0/mutwo/mmml_version/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-05 13:14:17.205965 mutwo_mmml-0.7.0/mutwo.mmml.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5643 2024-05-05 13:14:17.000000 mutwo_mmml-0.7.0/mutwo.mmml.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      508 2024-05-05 13:14:17.000000 mutwo_mmml-0.7.0/mutwo.mmml.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-05 13:14:17.000000 mutwo_mmml-0.7.0/mutwo.mmml.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      100 2024-05-05 13:14:17.000000 mutwo_mmml-0.7.0/mutwo.mmml.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-05-05 13:14:17.000000 mutwo_mmml-0.7.0/mutwo.mmml.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2024-05-05 13:14:06.000000 mutwo_mmml-0.7.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-05 13:14:17.209965 mutwo_mmml-0.7.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1137 2024-05-05 13:14:06.000000 mutwo_mmml-0.7.0/setup.py
```

### Comparing `mutwo.mmml-0.6.0/LICENSE` & `mutwo_mmml-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mutwo.mmml-0.6.0/mutwo/mmml_converters/__init__.py` & `mutwo_mmml-0.7.0/mutwo/mmml_converters/__init__.py`

 * *Files identical despite different names*

### Comparing `mutwo.mmml-0.6.0/mutwo/mmml_converters/codes.py` & `mutwo_mmml-0.7.0/mutwo/mmml_converters/codes.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import typing
 
 from mutwo import core_events
+from mutwo import core_parameters
 from mutwo import mmml_converters
 from mutwo import music_events
 from mutwo import music_parameters
 
 
 __all__ = ("register_decoder", "register_encoder")
 
@@ -41,15 +42,15 @@
         pitch,
         duration,
         volume=volume,
         playing_indicator_collection=playing_indicator_collection,
         notation_indicator_collection=notation_indicator_collection,
         lyric=lyric,
         instrument_list=instrument_list,
-        grace_note_sequential_event=core_events.SequentialEvent(event_tuple),
+        grace_note_consecution=core_events.Consecution(event_tuple),
     )
 
 
 @register_decoder
 def r(
     event_tuple: EventTuple,
     duration=1,
@@ -68,83 +69,128 @@
         [],
         duration,
         volume=volume,
         playing_indicator_collection=playing_indicator_collection,
         notation_indicator_collection=notation_indicator_collection,
         lyric=lyric,
         instrument_list=instrument_list,
-        grace_note_sequential_event=core_events.SequentialEvent(event_tuple),
+        grace_note_consecution=core_events.Consecution(event_tuple),
     )
 
 
 @register_decoder
-def seq(event_tuple: EventTuple, tag=None):
-    return core_events.TaggedSequentialEvent(event_tuple, tag=tag)
+def cns(event_tuple: EventTuple, tag=None):
+    return core_events.Consecution(event_tuple, tag=tag)
 
 
 @register_decoder
-def sim(event_tuple: EventTuple, tag=None):
-    return core_events.TaggedSimultaneousEvent(event_tuple, tag=tag)
+def cnc(event_tuple: EventTuple, tag=None):
+    return core_events.Concurrence(event_tuple, tag=tag)
 
 
 @register_encoder(music_events.NoteLike)
 def note_like(n: music_events.NoteLike):
-    d = str(n.duration.duration)
+    d = _parse_duration(n.duration)
+
+    pic = _parse_indicator_collection(n.playing_indicator_collection)
+    nic = _parse_indicator_collection(n.notation_indicator_collection)
+
     if n.pitch_list:
         p = ",".join([_parse_pitch(p) for p in n.pitch_list])
         v = _parse_volume(n.volume)
-        return f"n {d} {p} {v}"
+        header = f"n {d} {p} {v} {pic} {nic}"
+    else:
+        header = f"r {d} {pic} {nic}"
+
+    if n.grace_note_consecution:
+        block = "\n" + _compound_to_block(n.grace_note_consecution)
     else:
-        return f"r {d}"
+        block = ""
+
+    return f"{header}{block}"
+
+
+def _parse_duration(duration: core_parameters.abc.Duration):
+    match duration:
+        case core_parameters.DirectDuration():
+            d = duration.beat_count
+            if (intd := int(d)) == float(d):
+                d = intd
+            return str(d)
+        case core_parameters.RatioDuration():
+            return str(duration.ratio)
+        case _:
+            raise NotImplementedError(duration)
 
 
 def _parse_pitch(pitch: music_parameters.abc.Pitch):
     match pitch:
         case music_parameters.WesternPitch():
             return pitch.name
         case music_parameters.ScalePitch():
             return str(pitch.scale_degree + 1)
         case music_parameters.JustIntonationPitch():
-            return str(pitch.ratio)
+            r = str(pitch.ratio)
+            # Ensure we always render ratios with '/', otherwise
+            # the pitch parser of 'mutwo.music' won't be able to
+            # re-load them.
+            if "/" not in r:
+                r = f"{r}/1"
+            return r
         case _:
             raise NotImplementedError(pitch)
 
 
 def _parse_volume(volume: music_parameters.abc.Volume):
     match volume:
         case music_parameters.WesternVolume():
             return volume.name
         case _:
             raise NotImplementedError()
 
 
-@register_encoder(core_events.SequentialEvent, core_events.TaggedSequentialEvent)
-def sequential_event(
-    seq: core_events.SequentialEvent | core_events.TaggedSequentialEvent,
+def _parse_indicator_collection(indicator_collection):
+    mmml = ""
+    for name, indicator in indicator_collection.indicator_dict.items():
+        if indicator.is_active:
+            # XXX: This needs to be fixed in 'mutwo.music':
+            # ottava with 'octave_count=0' must be inactive.
+            if getattr(indicator, "octave_count", None) == 0:
+                continue
+            for k, v in indicator.get_arguments_dict().items():
+                if mmml:
+                    mmml += ";"
+                mmml += f"{name}.{k}={v}"
+    return mmml or mmml_converters.constants.IGNORE_MAGIC
+
+
+@register_encoder(core_events.Consecution)
+def consecution(
+    cns: core_events.Consecution,
 ):
-    tag = getattr(seq, "tag", None)
-    header = f"seq {tag}" if tag else "seq"
-    block = _complex_event_to_block(seq)
+    tag = cns.tag
+    header = f"cns {tag}" if tag else "cns"
+    block = _compound_to_block(cns)
     return f"{header}\n{block}"
 
 
-@register_encoder(core_events.SimultaneousEvent, core_events.TaggedSimultaneousEvent)
-def simultaneous_event(
-    sim: core_events.SimultaneousEvent | core_events.TaggedSimultaneousEvent,
+@register_encoder(core_events.Concurrence)
+def concurrence(
+    cnc: core_events.Concurrence,
 ):
-    tag = getattr(sim, "tag", None)
-    header = f"sim {tag}" if tag else "sim"
-    block = _complex_event_to_block(sim)
+    tag = getattr(cnc, "tag", None)
+    header = f"cnc {tag}" if tag else "cnc"
+    block = _compound_to_block(cnc)
     return f"{header}\n{block}"
 
 
-def _complex_event_to_block(complex_event: core_events.abc.ComplexEvent) -> str:
-    if not complex_event:
+def _compound_to_block(compound: core_events.abc.Compound) -> str:
+    if not compound:
         return ""
     block = [""]
-    for e in complex_event:
+    for e in compound:
         expression = mmml_converters.encode_event(e)
         for line in expression.split("\n"):
             line = f"{mmml_converters.constants.INDENTATION}{line}" if line else line
             block.append(line)
     block.append("")
     return "\n".join(block)
```

### Comparing `mutwo.mmml-0.6.0/mutwo/mmml_converters/frontends.py` & `mutwo_mmml-0.7.0/mutwo/mmml_converters/frontends.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,29 +17,33 @@
 
 class MMMLExpressionToEvent(core_converters.abc.Converter):
     """Convert a MMML expression to a mutwo event.
 
     **Example:**
 
     >>> from mutwo import mmml_converters
-    >>> c = mmml_converters.MMMLExpressionToEvent()
+    >>> c = mmml_converters.MMMLExpressionToEvent(use_defaults=True)
     >>> mmml = r'''
-    ... seq my-melody
+    ... cns my-melody
     ...     n 1/4 c
     ...     n 1/8 d ff
     ...     n 1/8 e
     ...     n 1/2 d
     ... '''
     >>> c.convert(mmml)
-    TaggedSequentialEvent([NoteLike(duration = DirectDuration(duration = 1/4), instrument_list = [], lyric = DirectLyric(phonetic_representation = ), pitch_list = [WesternPitch('c', 4)], tempo_envelope = TempoEnvelope([TempoEvent(curve_shape = 0, duration = DirectDuration(duration = 1), tempo_point = DirectTempoPoint(BPM = 60, reference = 1)), TempoEvent(curve_shape = 0, duration = DirectDuration(duration = 0), tempo_point = DirectTempoPoint(BPM = 60, reference = 1))]), volume = WesternVolume(amplitude = 0.12328467394420653)), NoteLike(duration = DirectDuration(duration = 1/8), instrument_list = [], lyric = DirectLyric(phonetic_representation = ), pitch_list = [WesternPitch('d', 4)], tempo_envelope = TempoEnvelope([TempoEvent(curve_shape = 0, duration = DirectDuration(duration = 1), tempo_point = DirectTempoPoint(BPM = 60, reference = 1)), TempoEvent(curve_shape = 0, duration = DirectDuration(duration = 0), tempo_point = DirectTempoPoint(BPM = 60, reference = 1))]), volume = WesternVolume(amplitude = 0.28480358684358004)), NoteLike(duration = DirectDuration(duration = 1/8), instrument_list = [], lyric = DirectLyric(phonetic_representation = ), pitch_list = [WesternPitch('e', 4)], tempo_envelope = TempoEnvelope([TempoEvent(curve_shape = 0, duration = DirectDuration(duration = 1), tempo_point = DirectTempoPoint(BPM = 60, reference = 1)), TempoEvent(curve_shape = 0, duration = DirectDuration(duration = 0), tempo_point = DirectTempoPoint(BPM = 60, reference = 1))]), volume = WesternVolume(amplitude = 0.28480358684358004)), NoteLike(duration = DirectDuration(duration = 1/2), instrument_list = [], lyric = DirectLyric(phonetic_representation = ), pitch_list = [WesternPitch('d', 4)], tempo_envelope = TempoEnvelope([TempoEvent(curve_shape = 0, duration = DirectDuration(duration = 1), tempo_point = DirectTempoPoint(BPM = 60, reference = 1)), TempoEvent(curve_shape = 0, duration = DirectDuration(duration = 0), tempo_point = DirectTempoPoint(BPM = 60, reference = 1))]), volume = WesternVolume(amplitude = 0.28480358684358004))])
+    Consecution([NoteLike(duration=RatioDuration(0.25), instrument_list=[], lyric=DirectLyric(), pitch_list=[WesternPitch('c', 4)], tag=None, tempo=DirectTempo(60.0), volume=WesternVolume(mf)), NoteLike(duration=RatioDuration(0.125), instrument_list=[], lyric=DirectLyric(), pitch_list=[WesternPitch('d', 4)], tag=None, tempo=DirectTempo(60.0), volume=WesternVolume(ff)), NoteLike(duration=RatioDuration(0.125), instrument_list=[], lyric=DirectLyric(), pitch_list=[WesternPitch('e', 4)], tag=None, tempo=DirectTempo(60.0), volume=WesternVolume(ff)), NoteLike(duration=RatioDuration(0.5), instrument_list=[], lyric=DirectLyric(), pitch_list=[WesternPitch('d', 4)], tag=None, tempo=DirectTempo(60.0), volume=WesternVolume(ff))])
     """
 
-    def __init__(self):
+    def __init__(self, use_defaults: bool = False):
+        self._use_defaults = use_defaults
+
         self._wrapped_decoder_dict = {}
+
         self.__decoder_default_dict = {}
+        self.__decoder_varnames_dict = {}
 
     def reset_defaults(self):
         self.__decoder_default_dict = {}
 
     def convert(self, expression: MMMLExpression, **kwargs) -> core_events.abc.Event:
         """Convert MMML expression to a mutwo event.
 
@@ -53,20 +57,21 @@
 
         **Example with mustache variables:**
 
         >>> from mutwo import mmml_converters
         >>> c = mmml_converters.MMMLExpressionToEvent()
         >>> expr = "n {{duration}} {{pitch}}"
         >>> c.convert(expr, duration='1/2', pitch='c')
-        NoteLike(duration = DirectDuration(duration = 1/2), instrument_list = [], lyric = DirectLyric(phonetic_representation = ), pitch_list = [WesternPitch('c', 4)], tempo_envelope = TempoEnvelope([TempoEvent(curve_shape = 0, duration = DirectDuration(duration = 1), tempo_point = DirectTempoPoint(BPM = 60, reference = 1)), TempoEvent(curve_shape = 0, duration = DirectDuration(duration = 0), tempo_point = DirectTempoPoint(BPM = 60, reference = 1))]), volume = WesternVolume(amplitude = 0.12328467394420653))
+        NoteLike(duration=RatioDuration(0.5), instrument_list=[], lyric=DirectLyric(), pitch_list=[WesternPitch('c', 4)], tag=None, tempo=DirectTempo(60.0), volume=WesternVolume(mf))
         """
         e = chevron.render(expression, dict(**kwargs))
         return self._process_expression(e)
 
     def _process_expression(self, expression: str) -> core_events.abc.Event:
+        expression = _drop_comments(expression)
         header, block = _split_to_header_and_block(expression)
         expression_name, arguments = self._process_header(header)
         event_tuple = self._process_block(block)
         try:
             wrapped_decoder = self._wrapped_decoder_dict[expression_name]
         except KeyError:
             try:
@@ -99,21 +104,34 @@
             seq
                 n 1/1 c fff
                 {{! The following note also has 'fff', because }}
                 {{! the previous NoteLike set it as its default. }}
                 n 1/1 c
         """
 
+        varnames = function.__code__.co_varnames
+        self.__decoder_varnames_dict[decoder_name] = varnames
+
         def _(*args):
-            self._set_decoder_default_args(decoder_name, args)
-            args = self._get_decoder_default_args(decoder_name, args)
-            return function(*args)
+            if self._use_defaults:
+                self._set_decoder_default_args(decoder_name, args)
+                args = self._get_decoder_default_args(decoder_name, args)
+            kwargs = self._args_to_kwargs(decoder_name, args)
+            return function(**kwargs)
 
         return _
 
+    def _args_to_kwargs(self, decoder_name: str, args: tuple) -> dict:
+        varnames = self.__decoder_varnames_dict[decoder_name]
+        return {
+            name: arg
+            for name, arg in zip(varnames, args)
+            if arg != mmml_converters.constants.IGNORE_MAGIC
+        }
+
     def _set_decoder_default_args(self, decoder_name: str, args: tuple):
         """Set currently defined arguments as new default values for decoder"""
         present_default = self.__decoder_default_dict.get(decoder_name, [])
         if len(args) > len(present_default):
             default = list(args)
         else:
             default = present_default
@@ -132,15 +150,17 @@
         return tuple(arg_list)
 
 
 def _split_to_header_and_block(expression: str):
     header, block = None, expression
     while not header:
         if not block:
-            raise mmml_utilities.MalformedMMML("No MMML expression found")
+            raise mmml_utilities.MalformedMMML(
+                f"No MMML expression found in expression '{expression}'"
+            )
         header, _, block = block.partition("\n")
     return header, block
 
 
 def _split_to_expression_tuple(mmml: str) -> tuple[list[str], ...]:
     lines = filter(bool, mmml.split("\n"))
 
@@ -163,7 +183,15 @@
         else:
             if expression_line_list:
                 expression_list.append(expression_line_list)
             expression_line_list = [line]
     if expression_line_list:
         expression_list.append(expression_line_list)
     return tuple("\n".join(e) for e in expression_list)
+
+
+def _drop_comments(expression: str):
+    def is_not_comment(line):
+        sline = line.strip()
+        return not (sline and sline[0] == mmml_converters.constants.COMMENT_MAGIC)
+
+    return "\n".join(filter(is_not_comment, expression.split("\n")))
```

### Comparing `mutwo.mmml-0.6.0/mutwo/mmml_utilities/codes.py` & `mutwo_mmml-0.7.0/mutwo/mmml_utilities/codes.py`

 * *Files identical despite different names*

### Comparing `mutwo.mmml-0.6.0/mutwo/mmml_utilities/exceptions.py` & `mutwo_mmml-0.7.0/mutwo/mmml_utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `mutwo.mmml-0.6.0/setup.py` & `mutwo_mmml-0.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,14 @@
     packages=[
         package
         for package in setuptools.find_namespace_packages(include=["mutwo.*"])
         if package[:5] != "tests"
     ],
     setup_requires=[],
     install_requires=[
-        "mutwo.core>=1.4.0, <2.0.0",
-        "mutwo.music>=0.24.0, <1.0.0",
+        "mutwo.core>=2.0.0, <3.0.0",
+        "mutwo.music>=0.27.0, <1.0.0",
         "chevron>=0.13.1, <1.0.0",
     ],
     extras_require=extras_require,
     python_requires=">=3.10, <4",
 )
```

