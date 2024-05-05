# Comparing `tmp/genieutils_py-0.0.1.tar.gz` & `tmp/genieutils_py-0.0.3.tar.gz`

## Comparing `genieutils_py-0.0.1.tar` & `genieutils_py-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 genieutils_py-0.0.1/src/genieutils/__init__.py
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 genieutils_py-0.0.1/src/genieutils/civ.py
--rw-r--r--   0        0        0     5399 2020-02-02 00:00:00.000000 genieutils_py-0.0.1/src/genieutils/common.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 genieutils_py-0.0.1/src/genieutils/datatypes.py
--rw-r--r--   0        0        0     6692 2020-02-02 00:00:00.000000 genieutils_py-0.0.1/src/genieutils/datfile.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 genieutils_py-0.0.1/src/genieutils/effect.py
--rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 genieutils_py-0.0.1/src/genieutils/graphic.py
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 genieutils_py-0.0.1/src/genieutils/playercolour.py
--rw-r--r--   0        0        0    10880 2020-02-02 00:00:00.000000 genieutils_py-0.0.1/src/genieutils/randommaps.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 genieutils_py-0.0.1/src/genieutils/scripts.py
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 genieutils_py-0.0.1/src/genieutils/sound.py
--rw-r--r--   0        0        0     4323 2020-02-02 00:00:00.000000 genieutils_py-0.0.1/src/genieutils/task.py
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 genieutils_py-0.0.1/src/genieutils/tech.py
--rw-r--r--   0        0        0    11648 2020-02-02 00:00:00.000000 genieutils_py-0.0.1/src/genieutils/techtree.py
--rw-r--r--   0        0        0    10874 2020-02-02 00:00:00.000000 genieutils_py-0.0.1/src/genieutils/terrainblock.py
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 genieutils_py-0.0.1/src/genieutils/terrainrestriction.py
--rw-r--r--   0        0        0    35593 2020-02-02 00:00:00.000000 genieutils_py-0.0.1/src/genieutils/unit.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 genieutils_py-0.0.1/src/genieutils/unitheaders.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 genieutils_py-0.0.1/.gitignore
--rw-r--r--   0        0        0     7650 2020-02-02 00:00:00.000000 genieutils_py-0.0.1/LICENSE
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 genieutils_py-0.0.1/README.md
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 genieutils_py-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 genieutils_py-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 genieutils_py-0.0.3/src/genieutils/__init__.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 genieutils_py-0.0.3/src/genieutils/civ.py
+-rw-r--r--   0        0        0     9547 2020-02-02 00:00:00.000000 genieutils_py-0.0.3/src/genieutils/common.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 genieutils_py-0.0.3/src/genieutils/datatypes.py
+-rw-r--r--   0        0        0     6878 2020-02-02 00:00:00.000000 genieutils_py-0.0.3/src/genieutils/datfile.py
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 genieutils_py-0.0.3/src/genieutils/effect.py
+-rw-r--r--   0        0        0     6575 2020-02-02 00:00:00.000000 genieutils_py-0.0.3/src/genieutils/graphic.py
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 genieutils_py-0.0.3/src/genieutils/playercolour.py
+-rw-r--r--   0        0        0    10866 2020-02-02 00:00:00.000000 genieutils_py-0.0.3/src/genieutils/randommaps.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 genieutils_py-0.0.3/src/genieutils/scripts.py
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 genieutils_py-0.0.3/src/genieutils/sound.py
+-rw-r--r--   0        0        0     4323 2020-02-02 00:00:00.000000 genieutils_py-0.0.3/src/genieutils/task.py
+-rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 genieutils_py-0.0.3/src/genieutils/tech.py
+-rw-r--r--   0        0        0    11056 2020-02-02 00:00:00.000000 genieutils_py-0.0.3/src/genieutils/techtree.py
+-rw-r--r--   0        0        0    10900 2020-02-02 00:00:00.000000 genieutils_py-0.0.3/src/genieutils/terrainblock.py
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 genieutils_py-0.0.3/src/genieutils/terrainrestriction.py
+-rw-r--r--   0        0        0    35547 2020-02-02 00:00:00.000000 genieutils_py-0.0.3/src/genieutils/unit.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 genieutils_py-0.0.3/src/genieutils/unitheaders.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 genieutils_py-0.0.3/.gitignore
+-rw-r--r--   0        0        0     7650 2020-02-02 00:00:00.000000 genieutils_py-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 genieutils_py-0.0.3/README.md
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 genieutils_py-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 genieutils_py-0.0.3/PKG-INFO
```

### Comparing `genieutils_py-0.0.1/src/genieutils/civ.py` & `genieutils_py-0.0.3/src/genieutils/civ.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,21 +4,18 @@
 from genieutils.unit import Unit
 
 
 @dataclass
 class Civ(GenieClass):
     player_type: int
     name: str
-    resources_size: int
     tech_tree_id: int
     team_bonus_id: int
     resources: list[float]
     icon_set: int
-    units_size: int
-    unit_pointers: list[int]
     units: list[Unit | None]
 
     @classmethod
     def from_bytes(cls, content: ByteHandler) -> 'Civ':
         player_type = content.read_int_8()
         name = content.read_debug_string()
         resources_size = content.read_int_16()
@@ -28,30 +25,31 @@
         icon_set = content.read_int_8()
         units_size = content.read_int_16()
         unit_pointers = content.read_int_32_array(units_size)
         units = content.read_class_array_with_pointers(Unit, units_size, unit_pointers)
         return cls(
             player_type=player_type,
             name=name,
-            resources_size=resources_size,
             tech_tree_id=tech_tree_id,
             team_bonus_id=team_bonus_id,
             resources=resources,
             icon_set=icon_set,
-            units_size=units_size,
-            unit_pointers=unit_pointers,
             units=units,
         )
 
+    @property
+    def unit_pointers(self) -> list[int]:
+        return [(0 if u is None else 1) for u in self.units]
+
     def to_bytes(self) -> bytes:
         return b''.join([
             self.write_int_8(self.player_type),
             self.write_debug_string(self.name),
-            self.write_int_16(self.resources_size),
+            self.write_int_16(len(self.resources)),
             self.write_int_16(self.tech_tree_id),
             self.write_int_16(self.team_bonus_id),
             self.write_float_array(self.resources),
             self.write_int_8(self.icon_set),
-            self.write_int_16(self.units_size),
+            self.write_int_16(len(self.units)),
             self.write_int_32_array(self.unit_pointers),
-            self.write_class_array_with_pointers(self.unit_pointers, self.units),
+            self.write_class_array(self.units),
         ])
```

### Comparing `genieutils_py-0.0.1/src/genieutils/datatypes.py` & `genieutils_py-0.0.3/src/genieutils/datatypes.py`

 * *Files identical despite different names*

### Comparing `genieutils_py-0.0.1/src/genieutils/datfile.py` & `genieutils_py-0.0.3/src/genieutils/datfile.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,35 +16,25 @@
 from genieutils.terrainrestriction import TerrainRestriction
 from genieutils.unitheaders import UnitHeaders
 
 
 @dataclass
 class DatFile(GenieClass):
     version: str
-    terrain_restrictions_size: int
-    terrains_used_1: int
     float_ptr_terrain_tables: list[int]
     terrain_pass_graphic_pointers: list[int]
     terrain_restrictions: list[TerrainRestriction]
-    player_colours_size: int
     player_colours: list[PlayerColour]
-    sounds_size: int
     sounds: list[Sound]
-    graphics_size: int
-    graphic_pointers: list[int]
     graphics: list[Graphic | None]
     terrain_block: TerrainBlock
     random_maps: RandomMaps
-    effects_size: int
     effects: list[Effect]
-    unit_headers_size: int
     unit_headers: list[UnitHeaders]
-    civs_size: int
     civs: list[Civ]
-    techs_size: int
     techs: list[Tech]
     time_slice: int
     unit_kill_rate: int
     unit_kill_total: int
     unit_hit_point_rate: int
     unit_hit_point_total: int
     razing_kill_rate: int
@@ -94,71 +84,71 @@
         unit_kill_total = content.read_int_32()
         unit_hit_point_rate = content.read_int_32()
         unit_hit_point_total = content.read_int_32()
         razing_kill_rate = content.read_int_32()
         razing_kill_total = content.read_int_32()
         tech_tree = content.read_class(TechTree)
         return cls(
-            version,
-            terrain_restrictions_size,
-            terrains_used_1,
-            float_ptr_terrain_tables,
-            terrain_pass_graphic_pointers,
-            terrain_restrictions,
-            player_colours_size,
-            player_colours,
-            sounds_size,
-            sounds,
-            graphics_size,
-            graphic_pointers,
-            graphics,
-            terrain_block,
-            random_maps,
-            effects_size,
-            effects,
-            unit_headers_size,
-            unit_headers,
-            civs_size,
-            civs,
-            techs_size,
-            techs,
-            time_slice,
-            unit_kill_rate,
-            unit_kill_total,
-            unit_hit_point_rate,
-            unit_hit_point_total,
-            razing_kill_rate,
-            razing_kill_total,
-            tech_tree,
+            version=version,
+            float_ptr_terrain_tables=float_ptr_terrain_tables,
+            terrain_pass_graphic_pointers=terrain_pass_graphic_pointers,
+            terrain_restrictions=terrain_restrictions,
+            player_colours=player_colours,
+            sounds=sounds,
+            graphics=graphics,
+            terrain_block=terrain_block,
+            random_maps=random_maps,
+            effects=effects,
+            unit_headers=unit_headers,
+            civs=civs,
+            techs=techs,
+            time_slice=time_slice,
+            unit_kill_rate=unit_kill_rate,
+            unit_kill_total=unit_kill_total,
+            unit_hit_point_rate=unit_hit_point_rate,
+            unit_hit_point_total=unit_hit_point_total,
+            razing_kill_rate=razing_kill_rate,
+            razing_kill_total=razing_kill_total,
+            tech_tree=tech_tree,
         )
 
+    @property
+    def graphic_pointers(self) -> list[int]:
+        return [(0 if g is None else 1) for g in self.graphics]
+
     def to_bytes(self) -> bytes:
+        terrain_restrictions_size = len(self.terrain_restrictions)
+        assert len(self.float_ptr_terrain_tables) == len(self.terrain_pass_graphic_pointers) == terrain_restrictions_size
+        terrains_used = 0
+        if self.terrain_restrictions:
+            terrains_used = len(self.terrain_restrictions[0].passable_buildable_dmg_multiplier)
+
         return b''.join([
             self.write_string(8, self.version),
-            self.write_int_16(self.terrain_restrictions_size),
-            self.write_int_16(self.terrains_used_1),
+            self.write_int_16(terrain_restrictions_size),
+            self.write_int_16(terrains_used),
             self.write_int_32_array(self.float_ptr_terrain_tables),
             self.write_int_32_array(self.terrain_pass_graphic_pointers),
             self.write_class_array(self.terrain_restrictions),
-            self.write_int_16(self.player_colours_size),
+            self.write_int_16(len(self.player_colours)),
             self.write_class_array(self.player_colours),
-            self.write_int_16(self.sounds_size),
+            self.write_int_16(len(self.sounds)),
             self.write_class_array(self.sounds),
-            self.write_int_16(self.graphics_size),
+            self.write_int_16(len(self.graphics)),
             self.write_int_32_array(self.graphic_pointers),
-            self.write_class_array_with_pointers(self.graphic_pointers, self.graphics),
+            self.write_class_array(self.graphics),
             self.write_class(self.terrain_block),
             self.write_class(self.random_maps),
-            self.write_int_32(self.effects_size),
+            self.write_int_32(len(self.effects)),
             self.write_class_array(self.effects),
-            self.write_int_32(self.unit_headers_size),
+            self.write_int_32(len(self.unit_headers)),
             self.write_class_array(self.unit_headers),
-            self.write_int_16(self.civs_size),
+            self.write_int_16(len(self.civs)),
             self.write_class_array(self.civs),
-            self.write_int_16(self.techs_size),
+            self.write_int_16(len(self.techs)),
             self.write_class_array(self.techs),
             self.write_int_32(self.time_slice),
             self.write_int_32(self.unit_kill_rate),
             self.write_int_32(self.unit_kill_total),
             self.write_int_32(self.unit_hit_point_rate),
             self.write_int_32(self.unit_hit_point_total),
             self.write_int_32(self.razing_kill_rate),
```

### Comparing `genieutils_py-0.0.1/src/genieutils/effect.py` & `genieutils_py-0.0.3/src/genieutils/effect.py`

 * *Files 21% similar despite different names*

```diff
@@ -30,27 +30,25 @@
             self.write_float(self.d),
         ])
 
 
 @dataclass
 class Effect(GenieClass):
     name: str
-    effect_command_count: int
     effect_commands: list[EffectCommand]
 
     @classmethod
     def from_bytes(cls, content: ByteHandler) -> 'Effect':
         name = content.read_debug_string()
         effect_command_count = content.read_int_16()
         effect_commands = content.read_class_array(EffectCommand, effect_command_count)
         return cls(
             name=name,
-            effect_command_count=effect_command_count,
             effect_commands=effect_commands,
         )
 
     def to_bytes(self) -> bytes:
         return b''.join([
             self.write_debug_string(self.name),
-            self.write_int_16(self.effect_command_count),
+            self.write_int_16(len(self.effect_commands)),
             self.write_class_array(self.effect_commands),
         ])
```

### Comparing `genieutils_py-0.0.1/src/genieutils/graphic.py` & `genieutils_py-0.0.3/src/genieutils/graphic.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,16 +84,15 @@
     particle_effect_name: str
     slp: int
     is_loaded: int
     old_color_flag: int
     layer: int
     player_color: int
     transparent_selection: int
-    coordinates: list[int]
-    delta_count: int
+    coordinates: tuple[int, int, int, int]
     sound_id: int
     wwise_sound_id: int
     angle_sounds_used: int
     frame_count: int
     angle_count: int
     speed_multiplier: float
     frame_duration: float
@@ -112,15 +111,15 @@
         particle_effect_name = content.read_debug_string()
         slp = content.read_int_32()
         is_loaded = content.read_int_8()
         old_color_flag = content.read_int_8()
         layer = content.read_int_8()
         player_color = content.read_int_16()
         transparent_selection = content.read_int_8()
-        coordinates = content.read_int_16_array(4)
+        coordinates = content.read_int_16_array_4()
         delta_count = content.read_int_16()
         sound_id = content.read_int_16()
         wwise_sound_id = content.read_int_32()
         angle_sounds_used = content.read_int_8()
         frame_count = content.read_int_16()
         angle_count = content.read_int_16()
         speed_multiplier = content.read_float()
@@ -139,15 +138,14 @@
             slp=slp,
             is_loaded=is_loaded,
             old_color_flag=old_color_flag,
             layer=layer,
             player_color=player_color,
             transparent_selection=transparent_selection,
             coordinates=coordinates,
-            delta_count=delta_count,
             sound_id=sound_id,
             wwise_sound_id=wwise_sound_id,
             angle_sounds_used=angle_sounds_used,
             frame_count=frame_count,
             angle_count=angle_count,
             speed_multiplier=speed_multiplier,
             frame_duration=frame_duration,
@@ -168,15 +166,15 @@
             self.write_int_32(self.slp),
             self.write_int_8(self.is_loaded),
             self.write_int_8(self.old_color_flag),
             self.write_int_8(self.layer),
             self.write_int_16(self.player_color),
             self.write_int_8(self.transparent_selection),
             self.write_int_16_array(self.coordinates),
-            self.write_int_16(self.delta_count),
+            self.write_int_16(len(self.deltas)),
             self.write_int_16(self.sound_id),
             self.write_int_32(self.wwise_sound_id),
             self.write_int_8(self.angle_sounds_used),
             self.write_int_16(self.frame_count),
             self.write_int_16(self.angle_count),
             self.write_float(self.speed_multiplier),
             self.write_float(self.frame_duration),
```

### Comparing `genieutils_py-0.0.1/src/genieutils/playercolour.py` & `genieutils_py-0.0.3/src/genieutils/playercolour.py`

 * *Files identical despite different names*

### Comparing `genieutils_py-0.0.1/src/genieutils/randommaps.py` & `genieutils_py-0.0.3/src/genieutils/randommaps.py`

 * *Files 2% similar despite different names*

```diff
@@ -274,32 +274,31 @@
             self.write_int_32(self.map_elevations_ptr),
             self.write_class_array(self.map_elevations),
         ])
 
 
 @dataclass
 class RandomMaps(GenieClass):
-    random_map_count: int
     random_maps_ptr: int
     map_info_1: list[MapInfo]
     map_info_2: list[MapInfo]
 
     @classmethod
     def from_bytes(cls, content: ByteHandler) -> 'RandomMaps':
         random_map_count = content.read_int_32(signed=False)
         random_maps_ptr = content.read_int_32()
         map_info_1 = content.read_class_array(MapInfo, random_map_count)
         map_info_2 = content.read_class_array(MapInfo, random_map_count)
         return cls(
-            random_map_count=random_map_count,
             random_maps_ptr=random_maps_ptr,
             map_info_1=map_info_1,
             map_info_2=map_info_2,
         )
 
     def to_bytes(self) -> bytes:
+        assert len(self.map_info_1) == len(self.map_info_2)
         return b''.join([
-            self.write_int_32(self.random_map_count, signed=False),
+            self.write_int_32(len(self.map_info_1), signed=False),
             self.write_int_32(self.random_maps_ptr),
             self.write_class_array(self.map_info_1),
             self.write_class_array(self.map_info_2),
         ])
```

### Comparing `genieutils_py-0.0.1/src/genieutils/scripts.py` & `genieutils_py-0.0.3/src/genieutils/scripts.py`

 * *Files identical despite different names*

### Comparing `genieutils_py-0.0.1/src/genieutils/sound.py` & `genieutils_py-0.0.3/src/genieutils/sound.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,14 @@
         ])
 
 
 @dataclass
 class Sound(GenieClass):
     id: int
     play_delay: int
-    items_size: int
     cache_time: int
     total_probability: int
     items: list[SoundItem]
 
     @classmethod
     def from_bytes(cls, content: ByteHandler) -> 'Sound':
         id_ = content.read_int_16()
@@ -47,22 +46,21 @@
         items_size = content.read_int_16()
         cache_time = content.read_int_32()
         total_probability = content.read_int_16()
         items = content.read_class_array(SoundItem, items_size)
         return cls(
             id=id_,
             play_delay=play_delay,
-            items_size=items_size,
             cache_time=cache_time,
             total_probability=total_probability,
             items=items,
         )
 
     def to_bytes(self) -> bytes:
         return b''.join([
             self.write_int_16(self.id),
             self.write_int_16(self.play_delay),
-            self.write_int_16(self.items_size),
+            self.write_int_16(len(self.items)),
             self.write_int_32(self.cache_time),
             self.write_int_16(self.total_probability),
             self.write_class_array(self.items),
         ])
```

### Comparing `genieutils_py-0.0.1/src/genieutils/task.py` & `genieutils_py-0.0.3/src/genieutils/task.py`

 * *Files identical despite different names*

### Comparing `genieutils_py-0.0.1/src/genieutils/tech.py` & `genieutils_py-0.0.3/src/genieutils/tech.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,16 +23,16 @@
             self.write_int_16(self.amount),
             self.write_int_8(self.flag),
         ])
 
 
 @dataclass
 class Tech(GenieClass):
-    required_techs: list[int]
-    resource_costs: list[ResearchResourceCost]
+    required_techs: tuple[int, int, int, int, int, int]
+    resource_costs: tuple[ResearchResourceCost, ResearchResourceCost, ResearchResourceCost]
     required_tech_count: int
     civ: int
     full_tech_mode: int
     research_location: int
     language_dll_name: int
     language_dll_description: int
     research_time: int
@@ -45,16 +45,16 @@
     hot_key: int
     name: str
     repeatable: int
 
     @classmethod
     def from_bytes(cls, content: ByteHandler) -> 'Tech':
         return cls(
-            required_techs=content.read_int_16_array(6),
-            resource_costs=content.read_class_array(ResearchResourceCost, 3),
+            required_techs=content.read_int_16_array_6(),
+            resource_costs=content.read_class_array_3(ResearchResourceCost),
             required_tech_count=content.read_int_16(),
             civ=content.read_int_16(),
             full_tech_mode=content.read_int_16(),
             research_location=content.read_int_16(),
             language_dll_name=content.read_int_32(),
             language_dll_description=content.read_int_32(),
             research_time=content.read_int_16(),
```

### Comparing `genieutils_py-0.0.1/src/genieutils/techtree.py` & `genieutils_py-0.0.3/src/genieutils/techtree.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,47 +2,44 @@
 
 from genieutils.common import ByteHandler, GenieClass
 
 
 @dataclass
 class Common(GenieClass):
     slots_used: int
-    unit_research: list[int]
-    mode: list[int]
+    unit_research: tuple[int, int, int, int, int, int, int, int, int, int]
+    mode: tuple[int, int, int, int, int, int, int, int, int, int]
 
     @classmethod
     def from_bytes(cls, content: ByteHandler) -> 'Common':
         return cls(
             slots_used=content.read_int_32(),
-            unit_research=content.read_int_32_array(10),
-            mode=content.read_int_32_array(10),
+            unit_research=content.read_int_32_array_10(),
+            mode=content.read_int_32_array_10(),
         )
 
     def to_bytes(self) -> bytes:
         return b''.join([
             self.write_int_32(self.slots_used),
             self.write_int_32_array(self.unit_research),
             self.write_int_32_array(self.mode),
         ])
 
 
 @dataclass
 class TechTreeAge(GenieClass):
     id: int
     status: int
-    buildings_count: int
     buildings: list[int]
-    units_count: int
     units: list[int]
-    techs_count: int
     techs: list[int]
     common: Common
     num_building_levels: int
-    buildings_per_zone: list[int]
-    group_length_per_zone: list[int]
+    buildings_per_zone: tuple[int, int, int, int, int, int, int, int, int, int]
+    group_length_per_zone: tuple[int, int, int, int, int, int, int, int, int, int]
     max_age_length: int
     line_mode: int
 
     @classmethod
     def from_bytes(cls, content: ByteHandler) -> 'TechTreeAge':
         id_ = content.read_int_32()
         status = content.read_int_8()
@@ -50,68 +47,62 @@
         buildings = content.read_int_32_array(buildings_count)
         units_count = content.read_int_8()
         units = content.read_int_32_array(units_count)
         techs_count = content.read_int_8()
         techs = content.read_int_32_array(techs_count)
         common = content.read_class(Common)
         num_building_levels = content.read_int_8()
-        buildings_per_zone = content.read_int_8_array(10)
-        group_length_per_zone = content.read_int_8_array(10)
+        buildings_per_zone = content.read_int_8_array_10()
+        group_length_per_zone = content.read_int_8_array_10()
         max_age_length = content.read_int_8()
         line_mode = content.read_int_32()
         return cls(
             id=id_,
             status=status,
-            buildings_count=buildings_count,
             buildings=buildings,
-            units_count=units_count,
             units=units,
-            techs_count=techs_count,
             techs=techs,
             common=common,
             num_building_levels=num_building_levels,
             buildings_per_zone=buildings_per_zone,
             group_length_per_zone=group_length_per_zone,
             max_age_length=max_age_length,
             line_mode=line_mode,
         )
 
     def to_bytes(self) -> bytes:
         return b''.join([
             self.write_int_32(self.id),
             self.write_int_8(self.status),
-            self.write_int_8(self.buildings_count),
+            self.write_int_8(len(self.buildings)),
             self.write_int_32_array(self.buildings),
-            self.write_int_8(self.units_count),
+            self.write_int_8(len(self.units)),
             self.write_int_32_array(self.units),
-            self.write_int_8(self.techs_count),
+            self.write_int_8(len(self.techs)),
             self.write_int_32_array(self.techs),
             self.write_class(self.common),
             self.write_int_8(self.num_building_levels),
             self.write_int_8_array(self.buildings_per_zone),
             self.write_int_8_array(self.group_length_per_zone),
             self.write_int_8(self.max_age_length),
             self.write_int_32(self.line_mode),
         ])
 
 
 @dataclass
 class BuildingConnection(GenieClass):
     id: int
     status: int
-    buildings_count: int
     buildings: list[int]
-    units_count: int
     units: list[int]
-    techs_count: int
     techs: list[int]
     common: Common
     location_in_age: int
-    units_techs_total: list[int]
-    units_techs_first: list[int]
+    units_techs_total: tuple[int, int, int, int, int]
+    units_techs_first: tuple[int, int, int, int, int]
     line_mode: int
     enabling_research: int
 
     @classmethod
     def from_bytes(cls, content: ByteHandler) -> 'BuildingConnection':
         id_ = content.read_int_32()
         status = content.read_int_8()
@@ -119,44 +110,41 @@
         buildings = content.read_int_32_array(buildings_count)
         units_count = content.read_int_8()
         units = content.read_int_32_array(units_count)
         techs_count = content.read_int_8()
         techs = content.read_int_32_array(techs_count)
         common = content.read_class(Common)
         location_in_age = content.read_int_8()
-        units_techs_total = content.read_int_8_array(5)
-        units_techs_first = content.read_int_8_array(5)
+        units_techs_total = content.read_int_8_array_5()
+        units_techs_first = content.read_int_8_array_5()
         line_mode = content.read_int_32()
         enabling_research = content.read_int_32()
         return cls(
             id=id_,
             status=status,
-            buildings_count=buildings_count,
             buildings=buildings,
-            units_count=units_count,
             units=units,
-            techs_count=techs_count,
             techs=techs,
             common=common,
             location_in_age=location_in_age,
             units_techs_total=units_techs_total,
             units_techs_first=units_techs_first,
             line_mode=line_mode,
             enabling_research=enabling_research,
         )
 
     def to_bytes(self) -> bytes:
         return b''.join([
             self.write_int_32(self.id),
             self.write_int_8(self.status),
-            self.write_int_8(self.buildings_count),
+            self.write_int_8(len(self.buildings)),
             self.write_int_32_array(self.buildings),
-            self.write_int_8(self.units_count),
+            self.write_int_8(len(self.units)),
             self.write_int_32_array(self.units),
-            self.write_int_8(self.techs_count),
+            self.write_int_8(len(self.techs)),
             self.write_int_32_array(self.techs),
             self.write_class(self.common),
             self.write_int_8(self.location_in_age),
             self.write_int_8_array(self.units_techs_total),
             self.write_int_8_array(self.units_techs_first),
             self.write_int_32(self.line_mode),
             self.write_int_32(self.enabling_research),
@@ -166,15 +154,14 @@
 @dataclass
 class UnitConnection(GenieClass):
     id: int
     status: int
     upper_building: int
     common: Common
     vertical_line: int
-    units_count: int
     units: list[int]
     location_in_age: int
     required_research: int
     line_mode: int
     enabling_research: int
 
     @classmethod
@@ -192,48 +179,44 @@
         enabling_research = content.read_int_32()
         return cls(
             id=id_,
             status=status,
             upper_building=upper_building,
             common=common,
             vertical_line=vertical_line,
-            units_count=units_count,
             units=units,
             location_in_age=location_in_age,
             required_research=required_research,
             line_mode=line_mode,
             enabling_research=enabling_research,
         )
 
     def to_bytes(self) -> bytes:
         return b''.join([
             self.write_int_32(self.id),
             self.write_int_8(self.status),
             self.write_int_32(self.upper_building),
             self.write_class(self.common),
             self.write_int_32(self.vertical_line),
-            self.write_int_8(self.units_count),
+            self.write_int_8(len(self.units)),
             self.write_int_32_array(self.units),
             self.write_int_32(self.location_in_age),
             self.write_int_32(self.required_research),
             self.write_int_32(self.line_mode),
             self.write_int_32(self.enabling_research),
         ])
 
 
 @dataclass
 class ResearchConnection(GenieClass):
     id: int
     status: int
     upper_building: int
-    buildings_count: int
     buildings: list[int]
-    units_count: int
     units: list[int]
-    techs_count: int
     techs: list[int]
     common: Common
     vertical_line: int
     location_in_age: int
     line_mode: int
 
     @classmethod
@@ -251,50 +234,43 @@
         vertical_line = content.read_int_32()
         location_in_age = content.read_int_32()
         line_mode = content.read_int_32()
         return cls(
             id=id_,
             status=status,
             upper_building=upper_building,
-            buildings_count=buildings_count,
             buildings=buildings,
-            units_count=units_count,
             units=units,
-            techs_count=techs_count,
             techs=techs,
             common=common,
             vertical_line=vertical_line,
             location_in_age=location_in_age,
             line_mode=line_mode,
         )
 
     def to_bytes(self) -> bytes:
         return b''.join([
             self.write_int_32(self.id),
             self.write_int_8(self.status),
             self.write_int_32(self.upper_building),
-            self.write_int_8(self.buildings_count),
+            self.write_int_8(len(self.buildings)),
             self.write_int_32_array(self.buildings),
-            self.write_int_8(self.units_count),
+            self.write_int_8(len(self.units)),
             self.write_int_32_array(self.units),
-            self.write_int_8(self.techs_count),
+            self.write_int_8(len(self.techs)),
             self.write_int_32_array(self.techs),
             self.write_class(self.common),
             self.write_int_32(self.vertical_line),
             self.write_int_32(self.location_in_age),
             self.write_int_32(self.line_mode),
         ])
 
 
 @dataclass
 class TechTree(GenieClass):
-    age_count: int
-    building_count: int
-    unit_count: int
-    research_count: int
     total_unit_tech_groups: int
     tech_tree_ages: list[TechTreeAge]
     building_connections: list[BuildingConnection]
     unit_connections: list[UnitConnection]
     research_connections: list[ResearchConnection]
 
     @classmethod
@@ -305,30 +281,26 @@
         research_count = content.read_int_8()
         total_unit_tech_groups = content.read_int_32()
         tech_tree_ages = content.read_class_array(TechTreeAge, age_count)
         building_connections = content.read_class_array(BuildingConnection, building_count)
         unit_connections = content.read_class_array(UnitConnection, unit_count)
         research_connections = content.read_class_array(ResearchConnection, research_count)
         return cls(
-            age_count=age_count,
-            building_count=building_count,
-            unit_count=unit_count,
-            research_count=research_count,
             total_unit_tech_groups=total_unit_tech_groups,
             tech_tree_ages=tech_tree_ages,
             building_connections=building_connections,
             unit_connections=unit_connections,
             research_connections=research_connections,
         )
 
     def to_bytes(self) -> bytes:
         return b''.join([
-            self.write_int_8(self.age_count),
-            self.write_int_8(self.building_count),
-            self.write_int_8(self.unit_count),
-            self.write_int_8(self.research_count),
+            self.write_int_8(len(self.tech_tree_ages)),
+            self.write_int_8(len(self.building_connections)),
+            self.write_int_8(len(self.unit_connections)),
+            self.write_int_8(len(self.research_connections)),
             self.write_int_32(self.total_unit_tech_groups),
             self.write_class_array(self.tech_tree_ages),
             self.write_class_array(self.building_connections),
             self.write_class_array(self.unit_connections),
             self.write_class_array(self.research_connections),
         ])
```

### Comparing `genieutils_py-0.0.1/src/genieutils/terrainblock.py` & `genieutils_py-0.0.3/src/genieutils/terrainblock.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,31 +38,31 @@
     shape_ptr: int
     sound_id: int
     wwise_sound_id: int
     wwise_sound_stop_id: int
     blend_priority: int
     blend_type: int
     overlay_mask_name: str
-    colors: list[int]
-    cliff_colors: list[int]
+    colors: tuple[int, int, int]
+    cliff_colors: tuple[int, int]
     passable_terrain: int
     impassable_terrain: int
     is_animated: int
     animation_frames: int
     pause_frames: int
     interval: float
     pause_between_loops: float
     frame: int
     draw_frame: int
     animate_last: float
     frame_changed: int
     drawn: int
     frame_data: list[FrameData]
     terrain_to_draw: int
-    terrain_dimensions: list[int]
+    terrain_dimensions: tuple[int, int]
     terrain_unit_masked_density: list[int]
     terrain_unit_id: list[int]
     terrain_unit_density: list[int]
     terrain_unit_centering: list[int]
     number_of_terrain_units_used: int
     phantom: int
 
@@ -80,31 +80,31 @@
             shape_ptr=content.read_int_32(),
             sound_id=content.read_int_32(),
             wwise_sound_id=content.read_int_32(signed=False),
             wwise_sound_stop_id=content.read_int_32(signed=False),
             blend_priority=content.read_int_32(),
             blend_type=content.read_int_32(),
             overlay_mask_name=content.read_debug_string(),
-            colors=content.read_int_8_array(3),
-            cliff_colors=content.read_int_8_array(2),
+            colors=content.read_int_8_array_3(),
+            cliff_colors=content.read_int_8_array_2(),
             passable_terrain=content.read_int_8(),
             impassable_terrain=content.read_int_8(),
             is_animated=content.read_int_8(),
             animation_frames=content.read_int_16(),
             pause_frames=content.read_int_16(),
             interval=content.read_float(),
             pause_between_loops=content.read_float(),
             frame=content.read_int_16(),
             draw_frame=content.read_int_16(),
             animate_last=content.read_float(),
             frame_changed=content.read_int_8(),
             drawn=content.read_int_8(),
             frame_data=content.read_class_array(FrameData, TILE_TYPE_COUNT),
             terrain_to_draw=content.read_int_16(),
-            terrain_dimensions=content.read_int_16_array(2),
+            terrain_dimensions=content.read_int_16_array_2(),
             terrain_unit_masked_density=content.read_int_16_array(TERRAIN_UNITS_SIZE),
             terrain_unit_id=content.read_int_16_array(TERRAIN_UNITS_SIZE),
             terrain_unit_density=content.read_int_16_array(TERRAIN_UNITS_SIZE),
             terrain_unit_centering=content.read_int_8_array(TERRAIN_UNITS_SIZE),
             number_of_terrain_units_used=content.read_int_16(),
             phantom=content.read_int_16(),
         )
```

### Comparing `genieutils_py-0.0.1/src/genieutils/terrainrestriction.py` & `genieutils_py-0.0.3/src/genieutils/terrainrestriction.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,11 +37,12 @@
     def from_bytes_with_count(cls, content: ByteHandler, terrain_count: int) -> 'TerrainRestriction':
         return cls(
             passable_buildable_dmg_multiplier=content.read_float_array(terrain_count),
             terrain_pass_graphics=content.read_class_array(TerrainPassGraphic, terrain_count),
         )
 
     def to_bytes(self) -> bytes:
+        assert len(self.passable_buildable_dmg_multiplier) == len(self.terrain_pass_graphics)
         return b''.join([
             self.write_float_array(self.passable_buildable_dmg_multiplier),
             self.write_class_array(self.terrain_pass_graphics),
         ])
```

### Comparing `genieutils_py-0.0.1/src/genieutils/unit.py` & `genieutils_py-0.0.3/src/genieutils/unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,30 +104,29 @@
 
 
 @dataclass
 class Bird(GenieClass):
     default_task_id: int
     search_radius: float
     work_rate: float
-    drop_sites: list[int]
+    drop_sites: tuple[int, int, int]
     task_swap_group: int
     attack_sound: int
     move_sound: int
     wwise_attack_sound_id: int
     wwise_move_sound_id: int
     run_pattern: int
-    task_size: int
     tasks: list[Task]
 
     @classmethod
     def from_bytes(cls, content: ByteHandler) -> 'Bird':
         default_task_id = content.read_int_16()
         search_radius = content.read_float()
         work_rate = content.read_float()
-        drop_sites = content.read_int_16_array(3)
+        drop_sites = content.read_int_16_array_3()
         task_swap_group = content.read_int_8()
         attack_sound = content.read_int_16()
         move_sound = content.read_int_16()
         wwise_attack_sound_id = content.read_int_32()
         wwise_move_sound_id = content.read_int_32()
         run_pattern = content.read_int_8()
         task_size = content.read_int_16()
@@ -139,15 +138,14 @@
             drop_sites=drop_sites,
             task_swap_group=task_swap_group,
             attack_sound=attack_sound,
             move_sound=move_sound,
             wwise_attack_sound_id=wwise_attack_sound_id,
             wwise_move_sound_id=wwise_move_sound_id,
             run_pattern=run_pattern,
-            task_size=task_size,
             tasks=tasks,
         )
 
     def to_bytes(self) -> bytes:
         return b''.join([
             self.write_int_16(self.default_task_id),
             self.write_float(self.search_radius),
@@ -155,15 +153,15 @@
             self.write_int_16_array(self.drop_sites),
             self.write_int_8(self.task_swap_group),
             self.write_int_16(self.attack_sound),
             self.write_int_16(self.move_sound),
             self.write_int_32(self.wwise_attack_sound_id),
             self.write_int_32(self.wwise_move_sound_id),
             self.write_int_8(self.run_pattern),
-            self.write_int_16(self.task_size),
+            self.write_int_16(len(self.tasks)),
             self.write_class_array(self.tasks),
         ])
 
 
 @dataclass
 class AttackOrArmor(GenieClass):
     class_: int
@@ -182,28 +180,26 @@
             self.write_int_16(self.amount),
         ])
 
 
 @dataclass
 class Type50(GenieClass):
     base_armor: int
-    attack_count: int
     attacks: list[AttackOrArmor]
-    armour_count: int
     armours: list[AttackOrArmor]
     defense_terrain_bonus: int
     bonus_damage_resistance: float
     max_range: float
     blast_width: float
     reload_time: float
     projectile_unit_id: int
     accuracy_percent: int
     break_off_combat: int
     frame_delay: int
-    graphic_displacement: list[float]
+    graphic_displacement: tuple[float, float, float]
     blast_attack_level: int
     min_range: float
     accuracy_dispersion: float
     attack_graphic: int
     displayed_melee_armour: int
     displayed_attack: int
     displayed_range: float
@@ -222,29 +218,27 @@
         max_range = content.read_float()
         blast_width = content.read_float()
         reload_time = content.read_float()
         projectile_unit_id = content.read_int_16()
         accuracy_percent = content.read_int_16()
         break_off_combat = content.read_int_8()
         frame_delay = content.read_int_16()
-        graphic_displacement = content.read_float_array(3)
+        graphic_displacement = content.read_float_array_3()
         blast_attack_level = content.read_int_8()
         min_range = content.read_float()
         accuracy_dispersion = content.read_float()
         attack_graphic = content.read_int_16()
         displayed_melee_armour = content.read_int_16()
         displayed_attack = content.read_int_16()
         displayed_range = content.read_float()
         displayed_reload_time = content.read_float()
         blast_damage = content.read_float()
         return cls(
             base_armor=base_armor,
-            attack_count=attack_count,
             attacks=attacks,
-            armour_count=armour_count,
             armours=armours,
             defense_terrain_bonus=defense_terrain_bonus,
             bonus_damage_resistance=bonus_damage_resistance,
             max_range=max_range,
             blast_width=blast_width,
             reload_time=reload_time,
             projectile_unit_id=projectile_unit_id,
@@ -262,17 +256,17 @@
             displayed_reload_time=displayed_reload_time,
             blast_damage=blast_damage,
         )
 
     def to_bytes(self) -> bytes:
         return b''.join([
             self.write_int_16(self.base_armor),
-            self.write_int_16(self.attack_count),
+            self.write_int_16(len(self.attacks)),
             self.write_class_array(self.attacks),
-            self.write_int_16(self.armour_count),
+            self.write_int_16(len(self.armours)),
             self.write_class_array(self.armours),
             self.write_int_16(self.defense_terrain_bonus),
             self.write_float(self.bonus_damage_resistance),
             self.write_float(self.max_range),
             self.write_float(self.blast_width),
             self.write_float(self.reload_time),
             self.write_int_16(self.projectile_unit_id),
@@ -343,15 +337,15 @@
             self.write_int_16(self.amount),
             self.write_int_16(self.flag),
         ])
 
 
 @dataclass
 class Creatable(GenieClass):
-    resource_costs: list[ResourceCost]
+    resource_costs: tuple[ResourceCost, ResourceCost, ResourceCost]
     train_time: int
     train_location_id: int
     button_id: int
     rear_attack_modifier: float
     flank_attack_modifier: float
     creatable_type: int
     hero_mode: int
@@ -364,24 +358,24 @@
     charge_event: int
     charge_type: int
     min_conversion_time_mod: float
     max_conversion_time_mod: float
     conversion_chance_mod: float
     total_projectiles: float
     max_total_projectiles: int
-    projectile_spawning_area: list[float]
+    projectile_spawning_area: tuple[float, float, float]
     secondary_projectile_unit: int
     special_graphic: int
     special_ability: int
     displayed_pierce_armor: int
 
     @classmethod
     def from_bytes(cls, content: ByteHandler) -> 'Creatable':
         return cls(
-            resource_costs=content.read_class_array(ResourceCost, 3),
+            resource_costs=content.read_class_array_3(ResourceCost),
             train_time=content.read_int_16(),
             train_location_id=content.read_int_16(),
             button_id=content.read_int_8(),
             rear_attack_modifier=content.read_float(),
             flank_attack_modifier=content.read_float(),
             creatable_type=content.read_int_8(),
             hero_mode=content.read_int_8(),
@@ -394,15 +388,15 @@
             charge_event=content.read_int_16(),
             charge_type=content.read_int_16(),
             min_conversion_time_mod=content.read_float(),
             max_conversion_time_mod=content.read_float(),
             conversion_chance_mod=content.read_float(),
             total_projectiles=content.read_float(),
             max_total_projectiles=content.read_int_8(),
-            projectile_spawning_area=content.read_float_array(3),
+            projectile_spawning_area=content.read_float_array_3(),
             secondary_projectile_unit=content.read_int_32(),
             special_graphic=content.read_int_32(),
             special_ability=content.read_int_8(),
             displayed_pierce_armor=content.read_int_16(),
         )
 
     def to_bytes(self) -> bytes:
@@ -470,26 +464,26 @@
     graphics_angle: int
     disappears_when_built: int
     stack_unit_id: int
     foundation_terrain_id: int
     old_overlap_id: int
     tech_id: int
     can_burn: int
-    annexes: list[BuildingAnnex]
+    annexes: tuple[BuildingAnnex, BuildingAnnex, BuildingAnnex, BuildingAnnex]
     head_unit: int
     transform_unit: int
     transform_sound: int
     construction_sound: int
     wwise_transform_sound_id: int
     wwise_construction_sound_id: int
     garrison_type: int
     garrison_heal_rate: float
     garrison_repair_rate: float
     pile_unit: int
-    looting_table: list[int]
+    looting_table: tuple[int, int, int, int, int, int]
 
     @classmethod
     def from_bytes(cls, content: ByteHandler) -> 'Building':
         return cls(
             construction_graphic_id=content.read_int_16(),
             snow_graphic_id=content.read_int_16(),
             destruction_graphic_id=content.read_int_16(),
@@ -500,26 +494,26 @@
             graphics_angle=content.read_int_16(),
             disappears_when_built=content.read_int_8(),
             stack_unit_id=content.read_int_16(),
             foundation_terrain_id=content.read_int_16(),
             old_overlap_id=content.read_int_16(),
             tech_id=content.read_int_16(),
             can_burn=content.read_int_8(),
-            annexes=content.read_class_array(BuildingAnnex, 4),
+            annexes=content.read_class_array_4(BuildingAnnex),
             head_unit=content.read_int_16(),
             transform_unit=content.read_int_16(),
             transform_sound=content.read_int_16(),
             construction_sound=content.read_int_16(),
             wwise_transform_sound_id=content.read_int_32(),
             wwise_construction_sound_id=content.read_int_32(),
             garrison_type=content.read_int_8(),
             garrison_heal_rate=content.read_float(),
             garrison_repair_rate=content.read_float(),
             pile_unit=content.read_int_16(),
-            looting_table=content.read_int_8_array(6),
+            looting_table=content.read_int_8_array_6(),
         )
 
     def to_bytes(self) -> bytes:
         return b''.join([
             self.write_int_16(self.construction_graphic_id),
             self.write_int_16(self.snow_graphic_id),
             self.write_int_16(self.destruction_graphic_id),
@@ -552,15 +546,15 @@
 @dataclass
 class Unit(GenieClass):
     type: int
     id: int
     language_dll_name: int
     language_dll_creation: int
     class_: int
-    standing_graphic: list[int]
+    standing_graphic: tuple[int, int]
     dying_graphic: int
     undead_graphic: int
     undead_mode: int
     hit_points: int
     line_of_sight: float
     garrison_capacity: int
     collision_size_x: float
@@ -573,17 +567,17 @@
     sort_number: int
     can_be_built_on: int
     icon_id: int
     hide_in_editor: int
     old_portrait_pict: int
     enabled: int
     disabled: int
-    placement_side_terrain: list[int]
-    placement_terrain: list[int]
-    clearance_size: list[float]
+    placement_side_terrain: tuple[int, int]
+    placement_terrain: tuple[int, int]
+    clearance_size: tuple[float, float]
     hill_mode: int
     fog_visibility: int
     terrain_restriction: int
     fly_mode: int
     resource_capacity: int
     resource_decay: float
     blast_defense_level: int
@@ -609,16 +603,15 @@
     selection_effect: int
     editor_selection_colour: int
     outline_size_x: float
     outline_size_y: float
     outline_size_z: float
     scenario_triggers_1: int
     scenario_triggers_2: int
-    resource_storages: list[ResourceStorage]
-    damage_graphic_size: int
+    resource_storages: tuple[ResourceStorage, ResourceStorage, ResourceStorage]
     damage_graphics: list[DamageGraphic]
     selection_sound: int
     dying_sound: int
     wwise_train_sound_id: int
     wwise_damage_sound_id: int
     wwise_selection_sound_id: int
     wwise_dying_sound_id: int
@@ -638,15 +631,15 @@
     @classmethod
     def from_bytes(cls, content: ByteHandler) -> 'Unit':
         type_ = content.read_int_8()
         id_ = content.read_int_16()
         language_dll_name = content.read_int_32()
         language_dll_creation = content.read_int_32()
         class_ = content.read_int_16()
-        standing_graphic = content.read_int_16_array(2)
+        standing_graphic = content.read_int_16_array_2()
         dying_graphic = content.read_int_16()
         undead_graphic = content.read_int_16()
         undead_mode = content.read_int_8()
         hit_points = content.read_int_16()
         line_of_sight = content.read_float()
         garrison_capacity = content.read_int_8()
         collision_size_x = content.read_float()
@@ -659,17 +652,17 @@
         sort_number = content.read_int_8()
         can_be_built_on = content.read_int_8()
         icon_id = content.read_int_16()
         hide_in_editor = content.read_int_8()
         old_portrait_pict = content.read_int_16()
         enabled = content.read_int_8()
         disabled = content.read_int_8()
-        placement_side_terrain = content.read_int_16_array(2)
-        placement_terrain = content.read_int_16_array(2)
-        clearance_size = content.read_float_array(2)
+        placement_side_terrain = content.read_int_16_array_2()
+        placement_terrain = content.read_int_16_array_2()
+        clearance_size = content.read_float_array_2()
         hill_mode = content.read_int_8()
         fog_visibility = content.read_int_8()
         terrain_restriction = content.read_int_16()
         fly_mode = content.read_int_8()
         resource_capacity = content.read_int_16()
         resource_decay = content.read_float()
         blast_defense_level = content.read_int_8()
@@ -695,15 +688,15 @@
         selection_effect = content.read_int_8()
         editor_selection_colour = content.read_int_8()
         outline_size_x = content.read_float()
         outline_size_y = content.read_float()
         outline_size_z = content.read_float()
         scenario_triggers_1 = content.read_int_32()
         scenario_triggers_2 = content.read_int_32()
-        resource_storages = content.read_class_array(ResourceStorage, 3)
+        resource_storages = content.read_class_array_3(ResourceStorage)
         damage_graphic_size = content.read_int_8()
         damage_graphics = content.read_class_array(DamageGraphic, damage_graphic_size)
         selection_sound = content.read_int_16()
         dying_sound = content.read_int_16()
         wwise_train_sound_id = content.read_int_32()
         wwise_damage_sound_id = content.read_int_32()
         wwise_selection_sound_id = content.read_int_32()
@@ -796,15 +789,14 @@
             editor_selection_colour=editor_selection_colour,
             outline_size_x=outline_size_x,
             outline_size_y=outline_size_y,
             outline_size_z=outline_size_z,
             scenario_triggers_1=scenario_triggers_1,
             scenario_triggers_2=scenario_triggers_2,
             resource_storages=resource_storages,
-            damage_graphic_size=damage_graphic_size,
             damage_graphics=damage_graphics,
             selection_sound=selection_sound,
             dying_sound=dying_sound,
             wwise_train_sound_id=wwise_train_sound_id,
             wwise_damage_sound_id=wwise_damage_sound_id,
             wwise_selection_sound_id=wwise_selection_sound_id,
             wwise_dying_sound_id=wwise_dying_sound_id,
@@ -905,15 +897,15 @@
             self.write_int_8(self.editor_selection_colour),
             self.write_float(self.outline_size_x),
             self.write_float(self.outline_size_y),
             self.write_float(self.outline_size_z),
             self.write_int_32(self.scenario_triggers_1),
             self.write_int_32(self.scenario_triggers_2),
             self.write_class_array(self.resource_storages),
-            self.write_int_8(self.damage_graphic_size),
+            self.write_int_8(len(self.damage_graphics)),
             self.write_class_array(self.damage_graphics),
             self.write_int_16(self.selection_sound),
             self.write_int_16(self.dying_sound),
             self.write_int_32(self.wwise_train_sound_id),
             self.write_int_32(self.wwise_damage_sound_id),
             self.write_int_32(self.wwise_selection_sound_id),
             self.write_int_32(self.wwise_dying_sound_id),
```

### Comparing `genieutils_py-0.0.1/src/genieutils/unitheaders.py` & `genieutils_py-0.0.3/src/genieutils/unitheaders.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,31 +3,28 @@
 from genieutils.common import ByteHandler, GenieClass
 from genieutils.task import Task
 
 
 @dataclass
 class UnitHeaders(GenieClass):
     exists: int
-    task_count: int | None = None
     task_list: list[Task] | None = None
 
     @classmethod
     def from_bytes(cls, content: ByteHandler) -> 'UnitHeaders':
         super().__init__(content)
         exists = content.read_int_8()
-        task_count = None
         task_list = None
         if exists:
             task_count = content.read_int_16()
             task_list = content.read_class_array(Task, task_count)
         return cls(
             exists=exists,
-            task_count=task_count,
             task_list=task_list,
         )
 
     def to_bytes(self) -> bytes:
         return b''.join([
             self.write_int_8(self.exists),
-            self.write_int_16(self.task_count) if self.exists else b'',
+            self.write_int_16(len(self.task_list)) if self.exists else b'',
             self.write_class_array(self.task_list) if self.exists else b'',
         ])
```

### Comparing `genieutils_py-0.0.1/.gitignore` & `genieutils_py-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `genieutils_py-0.0.1/LICENSE` & `genieutils_py-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `genieutils_py-0.0.1/README.md` & `genieutils_py-0.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 ### Prevent Kings from garrisoning
 
 ```python
 from genieutils.datfile import DatFile
 
 data = DatFile.parse('path/to/empires2_x2_p1.dat')
 for civ in data.civs:
-    civ.units[434].bird.task_size -= 1
     civ.units[434].bird.tasks.pop()
 data.save('path/to/modded/empires2_x2_p1.dat')
 ```
 
 
 ## Authors
```

### Comparing `genieutils_py-0.0.1/pyproject.toml` & `genieutils_py-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/genieutils"]
 
 [project]
 name = "genieutils-py"
-version = "0.0.1"
+version = "0.0.3"
 authors = [
     { name = "SiegeEngineers", email = "genieutils@siegeengineers.org" },
 ]
 description = "Re-implementation of genieutils in Python"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `genieutils_py-0.0.1/PKG-INFO` & `genieutils_py-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genieutils-py
-Version: 0.0.1
+Version: 0.0.3
 Summary: Re-implementation of genieutils in Python
 Project-URL: Homepage, https://github.com/SiegeEngineers/genieutils-py
 Project-URL: Issues, https://github.com/SiegeEngineers/genieutils-py/issues
 Author-email: SiegeEngineers <genieutils@siegeengineers.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
@@ -54,15 +54,14 @@
 ### Prevent Kings from garrisoning
 
 ```python
 from genieutils.datfile import DatFile
 
 data = DatFile.parse('path/to/empires2_x2_p1.dat')
 for civ in data.civs:
-    civ.units[434].bird.task_size -= 1
     civ.units[434].bird.tasks.pop()
 data.save('path/to/modded/empires2_x2_p1.dat')
 ```
 
 
 ## Authors
```

